# Comparing `tmp/tox_uv-1.8.2.tar.gz` & `tmp/tox_uv-1.9.0.tar.gz`

## Comparing `tox_uv-1.8.2.tar` & `tox_uv-1.9.0.tar`

### file list

```diff
@@ -1,25 +1,25 @@
--rw-r--r--   0        0        0      149 2020-02-02 00:00:00.000000 tox_uv-1.8.2/src/tox_uv/__init__.py
--rw-r--r--   0        0        0     6376 2020-02-02 00:00:00.000000 tox_uv-1.8.2/src/tox_uv/_installer.py
--rw-r--r--   0        0        0      545 2020-02-02 00:00:00.000000 tox_uv-1.8.2/src/tox_uv/_package.py
--rw-r--r--   0        0        0      856 2020-02-02 00:00:00.000000 tox_uv-1.8.2/src/tox_uv/_run.py
--rw-r--r--   0        0        0     7175 2020-02-02 00:00:00.000000 tox_uv-1.8.2/src/tox_uv/_venv.py
--rw-r--r--   0        0        0      321 2020-02-02 00:00:00.000000 tox_uv-1.8.2/src/tox_uv/_venv_query.py
--rw-r--r--   0        0        0      730 2020-02-02 00:00:00.000000 tox_uv-1.8.2/src/tox_uv/plugin.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 tox_uv-1.8.2/src/tox_uv/py.typed
--rw-r--r--   0        0        0      411 2020-02-02 00:00:00.000000 tox_uv-1.8.2/src/tox_uv/version.py
--rw-r--r--   0        0        0      437 2020-02-02 00:00:00.000000 tox_uv-1.8.2/tests/conftest.py
--rw-r--r--   0        0        0      624 2020-02-02 00:00:00.000000 tox_uv-1.8.2/tests/test_tox_uv_api.py
--rw-r--r--   0        0        0     3459 2020-02-02 00:00:00.000000 tox_uv-1.8.2/tests/test_tox_uv_installer.py
--rw-r--r--   0        0        0     1783 2020-02-02 00:00:00.000000 tox_uv-1.8.2/tests/test_tox_uv_package.py
--rw-r--r--   0        0        0     5297 2020-02-02 00:00:00.000000 tox_uv-1.8.2/tests/test_tox_uv_venv.py
--rw-r--r--   0        0        0      352 2020-02-02 00:00:00.000000 tox_uv-1.8.2/tests/test_version.py
--rw-r--r--   0        0        0     4292 2020-02-02 00:00:00.000000 tox_uv-1.8.2/tests/demo_pkg_inline/build.py
--rw-r--r--   0        0        0      112 2020-02-02 00:00:00.000000 tox_uv-1.8.2/tests/demo_pkg_inline/pyproject.toml
--rw-r--r--   0        0        0       90 2020-02-02 00:00:00.000000 tox_uv-1.8.2/tests/demo_pkg_setuptools/pyproject.toml
--rw-r--r--   0        0        0       82 2020-02-02 00:00:00.000000 tox_uv-1.8.2/tests/demo_pkg_setuptools/setup.cfg
--rw-r--r--   0        0        0      117 2020-02-02 00:00:00.000000 tox_uv-1.8.2/tests/demo_pkg_setuptools/demo_pkg_setuptools/__init__.py
--rw-r--r--   0        0        0      116 2020-02-02 00:00:00.000000 tox_uv-1.8.2/.gitignore
--rw-r--r--   0        0        0     1023 2020-02-02 00:00:00.000000 tox_uv-1.8.2/LICENSE
--rw-r--r--   0        0        0     2278 2020-02-02 00:00:00.000000 tox_uv-1.8.2/README.md
--rw-r--r--   0        0        0     3892 2020-02-02 00:00:00.000000 tox_uv-1.8.2/pyproject.toml
--rw-r--r--   0        0        0     3964 2020-02-02 00:00:00.000000 tox_uv-1.8.2/PKG-INFO
+-rw-r--r--   0        0        0      149 2020-02-02 00:00:00.000000 tox_uv-1.9.0/src/tox_uv/__init__.py
+-rw-r--r--   0        0        0     6376 2020-02-02 00:00:00.000000 tox_uv-1.9.0/src/tox_uv/_installer.py
+-rw-r--r--   0        0        0      545 2020-02-02 00:00:00.000000 tox_uv-1.9.0/src/tox_uv/_package.py
+-rw-r--r--   0        0        0      856 2020-02-02 00:00:00.000000 tox_uv-1.9.0/src/tox_uv/_run.py
+-rw-r--r--   0        0        0     7277 2020-02-02 00:00:00.000000 tox_uv-1.9.0/src/tox_uv/_venv.py
+-rw-r--r--   0        0        0      321 2020-02-02 00:00:00.000000 tox_uv-1.9.0/src/tox_uv/_venv_query.py
+-rw-r--r--   0        0        0      730 2020-02-02 00:00:00.000000 tox_uv-1.9.0/src/tox_uv/plugin.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 tox_uv-1.9.0/src/tox_uv/py.typed
+-rw-r--r--   0        0        0      411 2020-02-02 00:00:00.000000 tox_uv-1.9.0/src/tox_uv/version.py
+-rw-r--r--   0        0        0      437 2020-02-02 00:00:00.000000 tox_uv-1.9.0/tests/conftest.py
+-rw-r--r--   0        0        0      624 2020-02-02 00:00:00.000000 tox_uv-1.9.0/tests/test_tox_uv_api.py
+-rw-r--r--   0        0        0     3459 2020-02-02 00:00:00.000000 tox_uv-1.9.0/tests/test_tox_uv_installer.py
+-rw-r--r--   0        0        0     1783 2020-02-02 00:00:00.000000 tox_uv-1.9.0/tests/test_tox_uv_package.py
+-rw-r--r--   0        0        0     5585 2020-02-02 00:00:00.000000 tox_uv-1.9.0/tests/test_tox_uv_venv.py
+-rw-r--r--   0        0        0      352 2020-02-02 00:00:00.000000 tox_uv-1.9.0/tests/test_version.py
+-rw-r--r--   0        0        0     4292 2020-02-02 00:00:00.000000 tox_uv-1.9.0/tests/demo_pkg_inline/build.py
+-rw-r--r--   0        0        0      112 2020-02-02 00:00:00.000000 tox_uv-1.9.0/tests/demo_pkg_inline/pyproject.toml
+-rw-r--r--   0        0        0       90 2020-02-02 00:00:00.000000 tox_uv-1.9.0/tests/demo_pkg_setuptools/pyproject.toml
+-rw-r--r--   0        0        0       82 2020-02-02 00:00:00.000000 tox_uv-1.9.0/tests/demo_pkg_setuptools/setup.cfg
+-rw-r--r--   0        0        0      117 2020-02-02 00:00:00.000000 tox_uv-1.9.0/tests/demo_pkg_setuptools/demo_pkg_setuptools/__init__.py
+-rw-r--r--   0        0        0      116 2020-02-02 00:00:00.000000 tox_uv-1.9.0/.gitignore
+-rw-r--r--   0        0        0     1023 2020-02-02 00:00:00.000000 tox_uv-1.9.0/LICENSE
+-rw-r--r--   0        0        0     2278 2020-02-02 00:00:00.000000 tox_uv-1.9.0/README.md
+-rw-r--r--   0        0        0     3860 2020-02-02 00:00:00.000000 tox_uv-1.9.0/pyproject.toml
+-rw-r--r--   0        0        0     3965 2020-02-02 00:00:00.000000 tox_uv-1.9.0/PKG-INFO
```

### Comparing `tox_uv-1.8.2/src/tox_uv/_installer.py` & `tox_uv-1.9.0/src/tox_uv/_installer.py`

 * *Files identical despite different names*

### Comparing `tox_uv-1.8.2/src/tox_uv/_package.py` & `tox_uv-1.9.0/src/tox_uv/_package.py`

 * *Files identical despite different names*

### Comparing `tox_uv-1.8.2/src/tox_uv/_run.py` & `tox_uv-1.9.0/src/tox_uv/_run.py`

 * *Files identical despite different names*

### Comparing `tox_uv-1.8.2/src/tox_uv/_venv.py` & `tox_uv-1.9.0/src/tox_uv/_venv.py`

 * *Files 2% similar despite different names*

```diff
@@ -42,14 +42,15 @@
         super().register_config()
         desc = "add seed packages to the created venv"
         self.conf.add_config(keys=["uv_seed"], of_type=bool, default=False, desc=desc)
 
     def python_cache(self) -> dict[str, Any]:
         result = super().python_cache()
         result["seed"] = self.conf["uv_seed"]
+        result["venv"] = str(self.venv_dir.relative_to(self.env_dir))
         return result
 
     @property
     def executor(self) -> Execute:
         if self._executor is None:
             self._executor = LocalSubProcessExecutor(self.options.is_colored)
         return self._executor
@@ -101,15 +102,15 @@
 
     @property
     def uv(self) -> str:
         return find_uv_bin()
 
     @property
     def venv_dir(self) -> Path:
-        return cast(Path, self.conf["env_dir"]) / ".venv"
+        return cast(Path, self.conf["env_dir"])
 
     @property
     def environment_variables(self) -> dict[str, str]:
         env = super().environment_variables
         env["VIRTUAL_ENV"] = str(self.venv_dir)
         return env
 
@@ -124,15 +125,15 @@
     def create_python_env(self) -> None:
         base, imp = self.base_python.version_info, self.base_python.impl_lower
         if (base.major, base.minor) == sys.version_info[:2] and (sys.implementation.name.lower() == imp):
             version_spec = sys.executable
         else:
             uv_imp = "" if (imp and imp == "cpython") else imp
             version_spec = f"{uv_imp or ''}{base.major}.{base.minor}" if base.minor else f"{uv_imp or ''}{base.major}"
-        cmd: list[str] = [self.uv, "venv", "-p", version_spec]
+        cmd: list[str] = [self.uv, "venv", "-p", version_spec, "--allow-existing"]
         if self.options.verbosity > 2:  # noqa: PLR2004
             cmd.append("-v")
         if self.conf["uv_seed"]:
             cmd.append("--seed")
         cmd.append(str(self.venv_dir))
         outcome = self.execute(cmd, stdin=StdinSource.OFF, run_id="venv", show=None)
         outcome.assert_success()
@@ -141,15 +142,15 @@
     @property
     def _allow_externals(self) -> list[str]:
         result = super()._allow_externals
         result.append(self.uv)
         return result
 
     def prepend_env_var_path(self) -> list[Path]:
-        return [self.env_bin_dir()]
+        return [self.env_bin_dir(), Path(self.uv).parent]
 
     def env_bin_dir(self) -> Path:
         if sys.platform == "win32":  # pragma: win32 cover
             return self.venv_dir / "Scripts"
         else:  # pragma: win32 no cover # noqa: RET505
             return self.venv_dir / "bin"
```

### Comparing `tox_uv-1.8.2/src/tox_uv/plugin.py` & `tox_uv-1.9.0/src/tox_uv/plugin.py`

 * *Files identical despite different names*

### Comparing `tox_uv-1.8.2/tests/test_tox_uv_api.py` & `tox_uv-1.9.0/tests/test_tox_uv_api.py`

 * *Files identical despite different names*

### Comparing `tox_uv-1.8.2/tests/test_tox_uv_installer.py` & `tox_uv-1.9.0/tests/test_tox_uv_installer.py`

 * *Files identical despite different names*

### Comparing `tox_uv-1.8.2/tests/test_tox_uv_package.py` & `tox_uv-1.9.0/tests/test_tox_uv_package.py`

 * *Files identical despite different names*

### Comparing `tox_uv-1.8.2/tests/test_tox_uv_venv.py` & `tox_uv-1.9.0/tests/test_tox_uv_venv.py`

 * *Files 6% similar despite different names*

```diff
@@ -3,14 +3,15 @@
 import importlib.util
 import os
 import os.path
 import pathlib
 import subprocess  # noqa: S404
 import sys
 from configparser import ConfigParser
+from importlib.metadata import version
 from typing import TYPE_CHECKING
 
 if TYPE_CHECKING:
     from tox.pytest import ToxProjectCreator
 
 
 def test_uv_venv_self(tox_project: ToxProjectCreator) -> None:
@@ -61,49 +62,58 @@
 
 
 def test_uv_env_bin_dir(tox_project: ToxProjectCreator) -> None:
     project = tox_project({"tox.ini": "[testenv]\npackage=skip\ncommands=python -c 'print(\"{env_bin_dir}\")'"})
     result = project.run("-vv")
     result.assert_success()
 
-    env_bin_dir = str(project.path / ".tox" / "py" / ".venv" / ("Scripts" if sys.platform == "win32" else "bin"))
+    env_bin_dir = str(project.path / ".tox" / "py" / ("Scripts" if sys.platform == "win32" else "bin"))
     assert env_bin_dir in result.out
 
 
+def test_uv_env_has_access_to_plugin_uv(tox_project: ToxProjectCreator) -> None:
+    project = tox_project({"tox.ini": "[testenv]\npackage=skip\ncommands=uv --version"})
+    result = project.run()
+
+    result.assert_success()
+    ver = version("uv")
+    assert f"uv {ver}" in result.out
+
+
 def test_uv_env_python(tox_project: ToxProjectCreator) -> None:
     project = tox_project({"tox.ini": "[testenv]\npackage=skip\ncommands=python -c 'print(\"{env_python}\")'"})
     result = project.run("-vv")
     result.assert_success()
 
     exe = "python.exe" if sys.platform == "win32" else "python"
-    env_bin_dir = str(project.path / ".tox" / "py" / ".venv" / ("Scripts" if sys.platform == "win32" else "bin") / exe)
+    env_bin_dir = str(project.path / ".tox" / "py" / ("Scripts" if sys.platform == "win32" else "bin") / exe)
     assert env_bin_dir in result.out
 
 
 def test_uv_env_site_package_dir_run(tox_project: ToxProjectCreator) -> None:
     project = tox_project({"tox.ini": "[testenv]\npackage=skip\ncommands=python -c 'print(\"{envsitepackagesdir}\")'"})
     result = project.run("-vv")
     result.assert_success()
 
-    env_dir = project.path / ".tox" / "py" / ".venv"
+    env_dir = project.path / ".tox" / "py"
     ver = sys.version_info
     if sys.platform == "win32":  # pragma: win32 cover
         path = str(env_dir / "Lib" / "site-packages")
     else:  # pragma: win32 no cover
         impl = "pypy" if sys.implementation.name.lower() == "pypy" else "python"
         path = str(env_dir / "lib" / f"{impl}{ver.major}.{ver.minor}" / "site-packages")
     assert path in result.out
 
 
 def test_uv_env_site_package_dir_conf(tox_project: ToxProjectCreator) -> None:
     project = tox_project({"tox.ini": "[testenv]\npackage=skip\ncommands={envsitepackagesdir}"})
     result = project.run("c", "-e", "py", "-k", "commands")
     result.assert_success()
 
-    env_dir = project.path / ".tox" / "py" / ".venv"
+    env_dir = project.path / ".tox" / "py"
     ver = sys.version_info
     if sys.platform == "win32":  # pragma: win32 cover
         path = str(env_dir / "Lib" / "site-packages")
     else:  # pragma: win32 no cover
         impl = "pypy" if sys.implementation.name.lower() == "pypy" else "python"
         path = str(env_dir / "lib" / f"{impl}{ver.major}.{ver.minor}" / "site-packages")
     assert path in result.out
```

### Comparing `tox_uv-1.8.2/tests/demo_pkg_inline/build.py` & `tox_uv-1.9.0/tests/demo_pkg_inline/build.py`

 * *Files identical despite different names*

### Comparing `tox_uv-1.8.2/LICENSE` & `tox_uv-1.9.0/LICENSE`

 * *Files identical despite different names*

### Comparing `tox_uv-1.8.2/README.md` & `tox_uv-1.9.0/README.md`

 * *Files identical despite different names*

### Comparing `tox_uv-1.8.2/pyproject.toml` & `tox_uv-1.9.0/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -36,95 +36,94 @@
   "Topic :: Software Development :: Libraries",
   "Topic :: System",
 ]
 dynamic = [
   "version",
 ]
 dependencies = [
-  'importlib_resources>=6.4; python_version < "3.9"',
+  "importlib-resources>=6.4; python_version<'3.9'",
   "packaging>=24",
   "tox<5,>=4.15",
-  "uv<1,>=0.1.39",
+  "uv<1,>=0.2.5",
 ]
 optional-dependencies.test = [
   "covdefaults>=2.3",
   "devpi-process>=1",
-  "pytest>=8.2",
+  "pytest>=8.2.1",
   "pytest-cov>=5",
   "pytest-mock>=3.14",
 ]
 urls.Changelog = "https://github.com/tox-dev/tox-uv/releases"
 urls.Documentation = "https://github.com/tox-dev/tox-uv#tox-uv"
 urls.Homepage = "https://github.com/tox-dev/tox-uv"
 urls.Source = "https://github.com/tox-dev/tox-uv"
 urls.Tracker = "https://github.com/tox-dev/tox-uv/issues"
-entry-points.tox = {"tox-uv" = "tox_uv.plugin"}
+entry-points.tox.tox-uv = "tox_uv.plugin"
 
 [tool.hatch]
 build.hooks.vcs.version-file = "src/tox_uv/version.py"
 build.targets.sdist.include = [
   "/src",
   "/tests",
 ]
 version.source = "vcs"
 
 [tool.black]
 line-length = 120
 
 [tool.ruff]
-line-length = 120
 target-version = "py38"
-lint.isort = { known-first-party = [
-  "tox_uv",
-  "tests",
-], required-imports = [
-  "from __future__ import annotations",
-] }
+line-length = 120
+format.preview = true
+format.docstring-code-line-length = 100
+format.docstring-code-format = true
 lint.select = [
   "ALL",
 ]
 lint.ignore = [
   "ANN101", # Missing type annotation for `self` in method
-  "D301",   #  Use `r"""` if any backslashes in a docstring
-  "D205",   # 1 blank line required between summary line and description
-  "D401",   # First line of docstring should be in imperative mood
-  "D203",   # `one-blank-line-before-class` (D203) and `no-blank-line-before-class` (D211) are incompatible
-  "D212",   # `multi-line-summary-first-line` (D212) and `multi-line-summary-second-line` (D213) are incompatible
-  "S104",   # Possible binding to all interface
   "COM812", # Conflict with formatter
-  "ISC001", # Conflict with formatter
   "CPY",    # No copyriuvt statements
   "D",      # no documentation for now
+  "D203",   # `one-blank-line-before-class` (D203) and `no-blank-line-before-class` (D211) are incompatible
+  "D205",   # 1 blank line required between summary line and description
+  "D212",   # `multi-line-summary-first-line` (D212) and `multi-line-summary-second-line` (D213) are incompatible
+  "D301",   #  Use `r"""` if any backslashes in a docstring
+  "D401",   # First line of docstring should be in imperative mood
+  "ISC001", # Conflict with formatter
+  "S104",   # Possible binding to all interface
 ]
-lint.preview = true
-format.preview = true
-format.docstring-code-format = true
-format.docstring-code-line-length = 100
-[tool.ruff.lint.per-file-ignores]
-"tests/**/*.py" = [
-  "S101",    # asserts allowed in tests...
+lint.per-file-ignores."tests/**/*.py" = [
+  "D",       # don"t care about documentation in tests
   "FBT",     # don"t care about booleans as positional arguments in tests
   "INP001",  # no implicit namespace
-  "D",       # don"t care about documentation in tests
-  "S603",    # `subprocess` call: check for execution of untrusted input
   "PLR2004", # Magic value used in comparison, consider replacing with a constant variable
+  "S101",    # asserts allowed in tests...
+  "S603",    # `subprocess` call: check for execution of untrusted input
 ]
+lint.isort = { known-first-party = [
+  "tox_uv",
+  "tests",
+], required-imports = [
+  "from __future__ import annotations",
+] }
+lint.preview = true
 
 [tool.codespell]
 builtin = "clear,usage,en-GB_to_en-US"
 write-changes = true
 count = true
 
 [tool.coverage]
 html.show_contexts = true
 html.skip_covered = false
 paths.source = [
   "src",
-  ".tox/*/.venv/lib/*/site-packages",
-  ".tox\\*\\.venv\\Lib\\site-packages",
+  ".tox/*/lib/*/site-packages",
+  ".tox\\*\\Lib\\site-packages",
   "**/src",
   "**\\src",
 ]
 paths.other = [
   ".",
   "*/tox_uv",
   "*\\tox_uv",
```

### Comparing `tox_uv-1.8.2/PKG-INFO` & `tox_uv-1.9.0/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.3
 Name: tox-uv
-Version: 1.8.2
+Version: 1.9.0
 Summary: Integration of uv with tox.
 Project-URL: Changelog, https://github.com/tox-dev/tox-uv/releases
 Project-URL: Documentation, https://github.com/tox-dev/tox-uv#tox-uv
 Project-URL: Homepage, https://github.com/tox-dev/tox-uv
 Project-URL: Source, https://github.com/tox-dev/tox-uv
 Project-URL: Tracker, https://github.com/tox-dev/tox-uv/issues
 Maintainer-email: Bernát Gábor <gaborjbernat@gmail.com>
@@ -25,21 +25,21 @@
 Classifier: Topic :: Internet
 Classifier: Topic :: Software Development :: Libraries
 Classifier: Topic :: System
 Requires-Python: >=3.8
 Requires-Dist: importlib-resources>=6.4; python_version < '3.9'
 Requires-Dist: packaging>=24
 Requires-Dist: tox<5,>=4.15
-Requires-Dist: uv<1,>=0.1.39
+Requires-Dist: uv<1,>=0.2.5
 Provides-Extra: test
 Requires-Dist: covdefaults>=2.3; extra == 'test'
 Requires-Dist: devpi-process>=1; extra == 'test'
 Requires-Dist: pytest-cov>=5; extra == 'test'
 Requires-Dist: pytest-mock>=3.14; extra == 'test'
-Requires-Dist: pytest>=8.2; extra == 'test'
+Requires-Dist: pytest>=8.2.1; extra == 'test'
 Description-Content-Type: text/markdown
 
 # tox-uv
 
 [![PyPI version](https://badge.fury.io/py/tox-uv.svg)](https://badge.fury.io/py/tox-uv)
 [![PyPI Supported Python Versions](https://img.shields.io/pypi/pyversions/tox-uv.svg)](https://pypi.python.org/pypi/tox-uv/)
 [![check](https://github.com/tox-dev/tox-uv/actions/workflows/check.yml/badge.svg)](https://github.com/tox-dev/tox-uv/actions/workflows/check.yml)
```

