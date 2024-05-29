# Comparing `tmp/poetry-lock-package-0.5.0.tar.gz` & `tmp/poetry_lock_package-0.5.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "poetry-lock-package-0.5.0.tar", last modified: Tue Dec 20 15:52:55 2022, max compression
+gzip compressed data, was "poetry_lock_package-0.5.1.tar", max compression
```

## Comparing `poetry-lock-package-0.5.0.tar` & `poetry_lock_package-0.5.1.tar`

### file list

```diff
@@ -1,7 +1,6 @@
--rw-r--r--   0        0        0     2769 2022-12-20 15:52:15.193765 poetry-lock-package-0.5.0/README.md
--rw-r--r--   0        0        0      171 2022-12-20 15:52:15.197764 poetry-lock-package-0.5.0/poetry_lock_package/__init__.py
--rw-r--r--   0        0        0    10151 2022-12-20 15:52:15.197764 poetry-lock-package-0.5.0/poetry_lock_package/app.py
--rw-r--r--   0        0        0     1375 2022-12-20 15:52:15.197764 poetry-lock-package-0.5.0/poetry_lock_package/util.py
--rw-r--r--   0        0        0     1215 2022-12-20 15:52:54.717460 poetry-lock-package-0.5.0/pyproject.toml
--rw-r--r--   0        0        0     3753 2022-12-20 15:52:55.210362 poetry-lock-package-0.5.0/setup.py
--rw-r--r--   0        0        0     3637 2022-12-20 15:52:55.210716 poetry-lock-package-0.5.0/PKG-INFO
+-rw-r--r--   0        0        0     2769 2024-05-29 17:52:16.993122 poetry_lock_package-0.5.1/README.md
+-rw-r--r--   0        0        0      171 2024-05-29 17:52:16.997122 poetry_lock_package-0.5.1/poetry_lock_package/__init__.py
+-rw-r--r--   0        0        0    10890 2024-05-29 17:52:16.997122 poetry_lock_package-0.5.1/poetry_lock_package/app.py
+-rw-r--r--   0        0        0     1453 2024-05-29 17:52:16.997122 poetry_lock_package-0.5.1/poetry_lock_package/util.py
+-rw-r--r--   0        0        0     1278 2024-05-29 17:52:28.197246 poetry_lock_package-0.5.1/pyproject.toml
+-rw-r--r--   0        0        0     3741 1970-01-01 00:00:00.000000 poetry_lock_package-0.5.1/PKG-INFO
```

### Comparing `poetry-lock-package-0.5.0/README.md` & `poetry_lock_package-0.5.1/README.md`

 * *Files identical despite different names*

### Comparing `poetry-lock-package-0.5.0/poetry_lock_package/app.py` & `poetry_lock_package-0.5.1/poetry_lock_package/app.py`

 * *Files 3% similar despite different names*

```diff
@@ -18,19 +18,19 @@
     read_toml,
 )
 
 MAX_RECURSION_DEPTH = 1000
 
 
 def collect_dependencies(
-    lock_toml,
+    lock_toml: MutableMapping[str, Any],
     root_package_names: List[str],
     allow_package_filter: Callable[[str], bool],
 ) -> Dict[str, Any]:
-    def read_lock_information(name: str):
+    def read_lock_information(name: str) -> MutableMapping[str, Any]:
         """select lock information for given dependency"""
         for locked_package in lock_toml["package"]:
             if locked_package["name"] == name or normalized_package_name(
                 locked_package["name"]
             ) == normalized_package_name(name):
                 return copy.deepcopy(locked_package)
         raise KeyError(f"Could not find '{name}' in lock file")
@@ -68,24 +68,35 @@
             for package_name in dependencies_to_lock.keys()
         }
 
         # merge dependencies (contains markers) and locks (contains versions)
         for package_name, dependency_attributes in dependencies_to_lock.items():
             # Root packages have their own markers, the rest inherits markers
             if package_name not in root_package_names:
-                if type(dependency_attributes) == str:
+                if isinstance(dependency_attributes, str):
                     # If this is only a version, ignore it
-                    dependency_attributes = {}
-                del_keys(dependency_attributes, ["version"])
-                lock_information[package_name].update(dependency_attributes)
+                    # because it is already in the lock file information
+                    continue
+                elif isinstance(dependency_attributes, list):
+                    # If we have multiple version constaints,
+                    # we ignore the markers because we already have a version
+                    # picked from the lock
+                    continue
+                elif isinstance(dependency_attributes, dict):
+                    del_keys(dependency_attributes, ["version"])
+                    lock_information[package_name].update(dependency_attributes)
+                else:
+                    logging.warning(
+                        f"Found dependency information for '{package_name}' of type {type(dependency_attributes)}, ignoring. Consider filing an issue."
+                    )
         collected.update(lock_information)
     return collected
 
 
-def clean_dependencies(dependencies: Dict) -> Dict:
+def clean_dependencies(dependencies: Dict[str, Any]) -> Dict[str, Any]:
     dependencies = copy.deepcopy(dependencies)
     for _, metadata in dependencies.items():
         if not metadata.get("optional"):
             del_keys(metadata, ["optional"])
         if "python-versions" in metadata:
             metadata["python"] = metadata["python-versions"]
             del metadata["python-versions"]
@@ -148,15 +159,15 @@
         action="append",
         default=[],
     )
 
     return parser.parse_args()
 
 
-def main():
+def main() -> None:
     logging.basicConfig(format="%(levelname)s: %(message)s", level=logging.INFO)
 
     args = parse_arguments()
 
     wheel = args.wheel
     move = args.move
     clean = args.clean
@@ -252,16 +263,16 @@
                 os.path.join("dist", dist_filename),
             )
 
     if clean_up_project:
         shutil.rmtree(lock_project_path)
 
 
-def create_or_update(project, should_create_tests: bool) -> str:
-    lock_project_path = project["tool"]["poetry"]["name"]
+def create_or_update(project: Dict[str, Any], should_create_tests: bool) -> str:
+    lock_project_path: str = project["tool"]["poetry"]["name"]
     logging.info(f"Writing {lock_project_path}")
 
     # Create module folder
     module_path = os.path.join(
         lock_project_path,
         project["tool"]["poetry"]["name"].replace("-", "_"),
     )
```

### Comparing `poetry-lock-package-0.5.0/poetry_lock_package/util.py` & `poetry_lock_package-0.5.1/poetry_lock_package/util.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,16 +1,18 @@
 import os
 import re
 from contextlib import contextmanager
-from typing import Any, Callable, Dict, List, MutableMapping
+from typing import Any, Callable, Dict, Iterator, List, MutableMapping
 
 import toml
 
 
-def after(maximum_iterations: int, at_end_of_iteration: Callable[[], None]):
+def after(
+    maximum_iterations: int, at_end_of_iteration: Callable[[], None]
+) -> Iterator[int]:
     """
     Log a warning after maximum_iterations have been all consumed
     """
     counter = 0
     for counter in range(maximum_iterations):
         yield counter
     if counter == maximum_iterations - 1:
@@ -19,34 +21,34 @@
 
 def normalized_package_name(name: str) -> str:
     # TODO probably somewhere in poetry-core or poetry?
     # see https://www.python.org/dev/peps/pep-0426/
     return re.sub(r"[-_.]+", "-", name).lower()
 
 
-def del_keys(dictionary: Dict, keys: List[str]) -> None:
+def del_keys(dictionary: Dict[Any, Any], keys: List[str]) -> None:
     """In-place deletion of given keys"""
     for k in keys:
         if k in dictionary:
             del dictionary[k]
 
 
 def read_toml(filename: str) -> MutableMapping[str, Any]:
     with open(filename, "r") as project_file:
         return toml.load(project_file)
 
 
-def create_and_write(path, contents):
+def create_and_write(path: str, contents: str) -> None:
     if not os.path.exists(path):
         os.makedirs(os.path.dirname(path), exist_ok=True)
         with open(path, "w") as output_file:
             output_file.write(contents)
 
 
 @contextmanager
-def changed_directory(new_path: str):
+def changed_directory(new_path: str) -> Iterator[str]:
     old_path = os.getcwd()
     try:
         os.chdir(new_path)
         yield new_path
     finally:
         os.chdir(old_path)
```

### Comparing `poetry-lock-package-0.5.0/pyproject.toml` & `poetry_lock_package-0.5.1/pyproject.toml`

 * *Files 18% similar despite different names*

```diff
@@ -1,34 +1,33 @@
 [tool.poetry]
 name = "poetry-lock-package"
-version = "0.5.0"
+version = "0.5.1"
 description = "Poetry lock package generator"
 authors = ["Bram Neijt <bram@neijt.nl>"]
 readme = "README.md"
 repository = "https://github.com/bneijt/poetry-lock-package"
 classifiers = [
     "Environment :: Console",
     "Intended Audience :: Developers",
     "License :: OSI Approved :: GNU General Public License v3 (GPLv3)",
     "Topic :: Software Development :: Build Tools",
 ]
 
 [tool.poetry.dependencies]
-python = "^3.6.2"
+python = "^3.8.0"
 toml = "^0.10.1"
 importlib-metadata = { version = ">=0.22", python = "<3.8" }
 
-[tool.poetry.dev-dependencies]
-pytest = "^5.2"
-black = "^21.5b1"
-rope = "^0.18.0"
-twine = "^3.4.1"
-pre-commit = "^2.12.0"
-mypy = "^0.930"
-types-toml = "^0.10.1"
+[tool.poetry.group.dev.dependencies]
+pytest = "^7.2.0"
+rope = "^1.6.0"
+twine = "^4.0.2"
+pre-commit = "^2.20.0"
+mypy = "^0.991"
+types-toml = "^0.10.8.1"
 
 [tool.mypy]
 check_untyped_defs = true
 ignore_missing_imports = true
 warn_redundant_casts = true
 warn_unused_configs = true
 warn_unused_ignores = true
@@ -43,9 +42,12 @@
 [tool.poetry.scripts]
 poetry-lock-package = 'poetry_lock_package.app:main'
 
 [build-system]
 requires = ["poetry-core>=1.0.0"]
 build-backend = "poetry.core.masonry.api"
 
-[tool.isort]
-profile = "black"
+[tool.pytest.ini_options]
+addopts = ["--import-mode=importlib"]
+
+[tool.ruff.lint]
+extend-select = ["I"]
```

### Comparing `poetry-lock-package-0.5.0/setup.py` & `poetry_lock_package-0.5.1/PKG-INFO`

 * *Files 16% similar despite different names*

```diff
@@ -1,38 +1,91 @@
-# -*- coding: utf-8 -*-
-from setuptools import setup
+Metadata-Version: 2.1
+Name: poetry-lock-package
+Version: 0.5.1
+Summary: Poetry lock package generator
+Home-page: https://github.com/bneijt/poetry-lock-package
+Author: Bram Neijt
+Author-email: bram@neijt.nl
+Requires-Python: >=3.8.0,<4.0.0
+Classifier: Environment :: Console
+Classifier: Intended Audience :: Developers
+Classifier: License :: OSI Approved :: GNU General Public License v3 (GPLv3)
+Classifier: Programming Language :: Python :: 3
+Classifier: Programming Language :: Python :: 3.8
+Classifier: Programming Language :: Python :: 3.9
+Classifier: Programming Language :: Python :: 3.10
+Classifier: Programming Language :: Python :: 3.11
+Classifier: Programming Language :: Python :: 3.12
+Classifier: Topic :: Software Development :: Build Tools
+Requires-Dist: importlib-metadata (>=0.22) ; python_version < "3.8"
+Requires-Dist: toml (>=0.10.1,<0.11.0)
+Project-URL: Repository, https://github.com/bneijt/poetry-lock-package
+Description-Content-Type: text/markdown
 
-packages = \
-['poetry_lock_package']
+Poetry lock package generator
+=========================
 
-package_data = \
-{'': ['*']}
 
-install_requires = \
-['toml>=0.10.1,<0.11.0']
-
-extras_require = \
-{':python_version < "3.8"': ['importlib-metadata>=0.22']}
-
-entry_points = \
-{'console_scripts': ['poetry-lock-package = poetry_lock_package.app:main']}
-
-setup_kwargs = {
-    'name': 'poetry-lock-package',
-    'version': '0.5.0',
-    'description': 'Poetry lock package generator',
-    'long_description': "Poetry lock package generator\n=========================\n\n\nSimple script that will take a `pyproject.toml` and a `poetry.lock` and generate a new poetry project where all the lock versions are pinned dependencies.\n\nIn theory this will allow you to transport your lock file to any system that is able to install python packages and dependencies.\n\nAfter installation, the command `poetry-lock-package` should be run next to your `pyproject.toml` and `poetry.lock` files and will generate a subdirectory with a `pyproject.toml` requiring all the dependencies of the lock file.\n\nSimply enter the subdirectory, build and publish the package and you have a '-lock' package that depends on all the exact versions from your lock file.\n\n\nExample workflow\n---------------\nThe example workflow below will add `poetry-lock-package` as a dev dependency, allowing `poetry run` to find the command.\n\nFirst create a new poetry project\n\n    poetry new example-package\n    cd example-package\n\nAdd some dependencies, and see what we have build so far\n\n    poetry add loguru click\n    poetry install\n    poetry build\n    ls dist\n\nAdd `poetry-lock-package` to allow for `poetry run` to find the entry point script:\n\n    poetry add --dev poetry-lock-package\n\nFinally build the lock package and see what we have gotten\n\n    poetry run poetry-lock-package --build\n    ls -al dist\n\nYou will now have two wheel files in your dist folder: one with the project code, one name `example-package-lock` which depends on the exact version of all the packages specified in your `poetry.lock` file.\n\nUsing `--no-root`\n-----------------\nDefault behavior is to have the lock package depend on the original package the lock was created for. If you have a private repository, this will allow you to publish both packages to the private repository and only require you to point at one package to install everything.\n\nIf you want to be able to install the dependencies, but not the package itself, you can use the `--no-root` command line argument to stop `poetry-lock-package` from adding your root project to the lock package dependencies.\n\nUsing `--ignore`\n----------------\nIf you want to allow pip to have freedom in selecting a package, or you expect to deploy in an environment that already has the right version installed, you can opt to use `--ignore` to remove that dependency from the lock package pinned dependencies.\n\nBecause `poetry-lock-package` is aware of the dependency graph, it will not only skip locking the dependency but also transitive dependencies.\n\nContributing code\n-----------------\n\n- Open an issue\n- Create an associated PR\n- Make sure to black format the proposed change\n\n    poetry run pre-commit install\n\n- Add tests where possible\n\nLicense\n-------\nGPLv3, use at your own risk.\n\n",
-    'author': 'Bram Neijt',
-    'author_email': 'bram@neijt.nl',
-    'maintainer': None,
-    'maintainer_email': None,
-    'url': 'https://github.com/bneijt/poetry-lock-package',
-    'packages': packages,
-    'package_data': package_data,
-    'install_requires': install_requires,
-    'extras_require': extras_require,
-    'entry_points': entry_points,
-    'python_requires': '>=3.6.2,<4.0.0',
-}
+Simple script that will take a `pyproject.toml` and a `poetry.lock` and generate a new poetry project where all the lock versions are pinned dependencies.
+
+In theory this will allow you to transport your lock file to any system that is able to install python packages and dependencies.
+
+After installation, the command `poetry-lock-package` should be run next to your `pyproject.toml` and `poetry.lock` files and will generate a subdirectory with a `pyproject.toml` requiring all the dependencies of the lock file.
+
+Simply enter the subdirectory, build and publish the package and you have a '-lock' package that depends on all the exact versions from your lock file.
+
+
+Example workflow
+---------------
+The example workflow below will add `poetry-lock-package` as a dev dependency, allowing `poetry run` to find the command.
+
+First create a new poetry project
+
+    poetry new example-package
+    cd example-package
+
+Add some dependencies, and see what we have build so far
+
+    poetry add loguru click
+    poetry install
+    poetry build
+    ls dist
+
+Add `poetry-lock-package` to allow for `poetry run` to find the entry point script:
+
+    poetry add --dev poetry-lock-package
+
+Finally build the lock package and see what we have gotten
+
+    poetry run poetry-lock-package --build
+    ls -al dist
+
+You will now have two wheel files in your dist folder: one with the project code, one name `example-package-lock` which depends on the exact version of all the packages specified in your `poetry.lock` file.
+
+Using `--no-root`
+-----------------
+Default behavior is to have the lock package depend on the original package the lock was created for. If you have a private repository, this will allow you to publish both packages to the private repository and only require you to point at one package to install everything.
+
+If you want to be able to install the dependencies, but not the package itself, you can use the `--no-root` command line argument to stop `poetry-lock-package` from adding your root project to the lock package dependencies.
+
+Using `--ignore`
+----------------
+If you want to allow pip to have freedom in selecting a package, or you expect to deploy in an environment that already has the right version installed, you can opt to use `--ignore` to remove that dependency from the lock package pinned dependencies.
+
+Because `poetry-lock-package` is aware of the dependency graph, it will not only skip locking the dependency but also transitive dependencies.
+
+Contributing code
+-----------------
+
+- Open an issue
+- Create an associated PR
+- Make sure to black format the proposed change
+
+    poetry run pre-commit install
+
+- Add tests where possible
+
+License
+-------
+GPLv3, use at your own risk.
 
 
-setup(**setup_kwargs)
```

