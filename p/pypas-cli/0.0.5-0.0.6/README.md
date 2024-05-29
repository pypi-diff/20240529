# Comparing `tmp/pypas_cli-0.0.5.tar.gz` & `tmp/pypas_cli-0.0.6.tar.gz`

## Comparing `pypas_cli-0.0.5.tar` & `pypas_cli-0.0.6.tar`

### file list

```diff
@@ -1,15 +1,17 @@
--rw-r--r--   0        0        0      134 2020-02-02 00:00:00.000000 pypas_cli-0.0.5/CHANGELOG.md
--rw-r--r--   0        0        0      261 2020-02-02 00:00:00.000000 pypas_cli-0.0.5/justfile
--rw-r--r--   0        0        0       12 2020-02-02 00:00:00.000000 pypas_cli-0.0.5/requirements-dev.txt
--rw-r--r--   0        0        0      115 2020-02-02 00:00:00.000000 pypas_cli-0.0.5/src/pypas/__init__.py
--rw-r--r--   0        0        0     1433 2020-02-02 00:00:00.000000 pypas_cli-0.0.5/src/pypas/main.py
--rw-r--r--   0        0        0      278 2020-02-02 00:00:00.000000 pypas_cli-0.0.5/src/pypas/settings.py
--rw-r--r--   0        0        0      708 2020-02-02 00:00:00.000000 pypas_cli-0.0.5/src/pypas/lib/console.py
--rw-r--r--   0        0        0      366 2020-02-02 00:00:00.000000 pypas_cli-0.0.5/src/pypas/lib/decorators.py
--rw-r--r--   0        0        0     2746 2020-02-02 00:00:00.000000 pypas_cli-0.0.5/src/pypas/lib/exercise.py
--rw-r--r--   0        0        0     1936 2020-02-02 00:00:00.000000 pypas_cli-0.0.5/src/pypas/lib/utils.py
--rw-r--r--   0        0        0       62 2020-02-02 00:00:00.000000 pypas_cli-0.0.5/.gitignore
--rw-r--r--   0        0        0     1080 2020-02-02 00:00:00.000000 pypas_cli-0.0.5/LICENSE
--rw-r--r--   0        0        0       12 2020-02-02 00:00:00.000000 pypas_cli-0.0.5/README.md
--rw-r--r--   0        0        0      939 2020-02-02 00:00:00.000000 pypas_cli-0.0.5/pyproject.toml
--rw-r--r--   0        0        0     1955 2020-02-02 00:00:00.000000 pypas_cli-0.0.5/PKG-INFO
+-rw-r--r--   0        0        0      134 2020-02-02 00:00:00.000000 pypas_cli-0.0.6/CHANGELOG.md
+-rw-r--r--   0        0        0      261 2020-02-02 00:00:00.000000 pypas_cli-0.0.6/justfile
+-rw-r--r--   0        0        0       12 2020-02-02 00:00:00.000000 pypas_cli-0.0.6/requirements-dev.txt
+-rw-r--r--   0        0        0      189 2020-02-02 00:00:00.000000 pypas_cli-0.0.6/src/pypas/__init__.py
+-rw-r--r--   0        0        0     1683 2020-02-02 00:00:00.000000 pypas_cli-0.0.6/src/pypas/main.py
+-rw-r--r--   0        0        0      464 2020-02-02 00:00:00.000000 pypas_cli-0.0.6/src/pypas/settings.py
+-rw-r--r--   0        0        0      966 2020-02-02 00:00:00.000000 pypas_cli-0.0.6/src/pypas/lib/auth.py
+-rw-r--r--   0        0        0      679 2020-02-02 00:00:00.000000 pypas_cli-0.0.6/src/pypas/lib/config.py
+-rw-r--r--   0        0        0     1370 2020-02-02 00:00:00.000000 pypas_cli-0.0.6/src/pypas/lib/console.py
+-rw-r--r--   0        0        0      366 2020-02-02 00:00:00.000000 pypas_cli-0.0.6/src/pypas/lib/decorators.py
+-rw-r--r--   0        0        0     2693 2020-02-02 00:00:00.000000 pypas_cli-0.0.6/src/pypas/lib/exercise.py
+-rw-r--r--   0        0        0     1936 2020-02-02 00:00:00.000000 pypas_cli-0.0.6/src/pypas/lib/utils.py
+-rw-r--r--   0        0        0       62 2020-02-02 00:00:00.000000 pypas_cli-0.0.6/.gitignore
+-rw-r--r--   0        0        0     1080 2020-02-02 00:00:00.000000 pypas_cli-0.0.6/LICENSE
+-rw-r--r--   0        0        0       12 2020-02-02 00:00:00.000000 pypas_cli-0.0.6/README.md
+-rw-r--r--   0        0        0      951 2020-02-02 00:00:00.000000 pypas_cli-0.0.6/pyproject.toml
+-rw-r--r--   0        0        0     1975 2020-02-02 00:00:00.000000 pypas_cli-0.0.6/PKG-INFO
```

### Comparing `pypas_cli-0.0.5/src/pypas/main.py` & `pypas_cli-0.0.6/src/pypas/main.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,16 +1,16 @@
 import typer
 from rich.prompt import Confirm
 
-from pypas import Exercise, console
+from pypas import Exercise, User, config, console
 from pypas.lib.decorators import inside_exercise
 
 app = typer.Typer(
     add_completion=False,
-    help='✨ pypas → Python Practical Assignments',
+    help='pypas ⚘ Python Practical Assignments',
     no_args_is_help=True,
 )
 
 
 @app.command()
 def get(exercise_slug: str = typer.Argument(help='Slug of exercise')):
     """Get exercise."""
@@ -44,9 +44,17 @@
     """Update exercise."""
     exercise = Exercise.from_config()
     exercise.download()
     dir = exercise.unzip(to_tmp_dir=True)
     exercise.update(src_dir=dir, backup=not force)
 
 
+@app.command()
+def auth(token: str = typer.Argument(help='Access token')):
+    """Authenticate at pypas.es (token must be given by administrator)"""
+    if User(token).authenticate():
+        config['token'] = token
+        config.save()
+
+
 if __name__ == '__main__':
     app()
```

### Comparing `pypas_cli-0.0.5/src/pypas/lib/exercise.py` & `pypas_cli-0.0.6/src/pypas/lib/exercise.py`

 * *Files 8% similar despite different names*

```diff
@@ -3,15 +3,15 @@
 import os
 import shutil
 import tempfile
 import zipfile
 from pathlib import Path
 from urllib.parse import urljoin
 
-import tomllib
+import toml
 from pypas import settings
 
 from . import utils
 from .console import console
 
 
 class Exercise:
@@ -37,47 +37,46 @@
             self._cfg = Exercise.load_config()
         return self._cfg
 
     def folder_exists(self) -> bool:
         return self.folder.exists()
 
     def download(self) -> Path | None:
-        console.print(f'Getting exercise from: [italic]{self.url}')
+        console.debug(f'Getting exercise from: [italic]{self.url}')
         if downloaded_zip := utils.download(self.url, self.zipname, save_temp=True):
             self.downloaded_zip = downloaded_zip
         return downloaded_zip
 
     def unzip(self, to_tmp_dir: bool = False) -> Path:
         tmp_dir = tempfile.TemporaryDirectory(delete=False)
         target_dir = Path(tmp_dir.name) if to_tmp_dir else self.folder
         console.print('Inflating exercise bundle', end=' ')
         with zipfile.ZipFile(self.downloaded_zip) as zip_ref:
             zip_ref.extractall(target_dir)
-        console.done()
+        console.check()
         os.remove(self.downloaded_zip)
         return target_dir
 
     def open_docs(self):
         os.system(f'{utils.get_open_cmd()} docs/README.pdf')
 
     def update(self, src_dir: Path, backup: bool = True):
         for file in src_dir.glob('**/*'):
             if file.is_file():
                 rel_file = file.relative_to(src_dir)
                 if backup and rel_file.exists() and str(rel_file) in self.config['todo']:
                     backup_file = rel_file.with_suffix(rel_file.suffix + '.bak')
-                    console.print(f'Backup {rel_file} → {backup_file}', end=' ')
+                    console.debug(f'Backup {rel_file} → {backup_file}')
                     shutil.copy(rel_file, backup_file)
-                    console.done()
                 rel_file.parent.mkdir(parents=True, exist_ok=True)
                 shutil.copy(file, rel_file)
         shutil.rmtree(src_dir, ignore_errors=True)
-        console.great('Exercise is updated to last version!')
+        console.success('Exercise is updated to last version!')
 
     @classmethod
     def from_config(cls) -> Exercise:
         return cls(Exercise.load_config()['slug'])
 
     @staticmethod
     def load_config(filename: str = settings.EXERCISE_CONFIG_FILE):
-        with open(filename, 'rb') as f:
-            return tomllib.load(f)
+        with open(filename) as f:
+            return toml.load(f)
```

### Comparing `pypas_cli-0.0.5/src/pypas/lib/utils.py` & `pypas_cli-0.0.6/src/pypas/lib/utils.py`

 * *Files identical despite different names*

### Comparing `pypas_cli-0.0.5/LICENSE` & `pypas_cli-0.0.6/LICENSE`

 * *Files identical despite different names*

### Comparing `pypas_cli-0.0.5/pyproject.toml` & `pypas_cli-0.0.6/pyproject.toml`

 * *Files 14% similar despite different names*

```diff
@@ -1,22 +1,23 @@
 [build-system]
 requires = ["hatchling"]
 build-backend = "hatchling.build"
 
 [project]
 name = "pypas-cli"
-version = "0.0.5"
+version = "0.0.6"
 license = { file = "LICENSE" }
 dependencies = [
     'setuptools',
     'typer',
     'prettyconf',
     'requests',
     'rich',
     'pytest',
+    'toml',
 ]
 authors = [
     { email = "sdelquin@gmail.com" },
     { name = "Sergio Delgado Quintero" },
 ]
 maintainers = [
     { name = "Sergio Delgado Quintero", email = "sdelquin@gmail.com" },
```

### Comparing `pypas_cli-0.0.5/PKG-INFO` & `pypas_cli-0.0.6/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.3
 Name: pypas-cli
-Version: 0.0.5
+Version: 0.0.6
 Summary: Python Practical Assignments
 Project-URL: homepage, https://pypas.es
 Project-URL: repository, https://github.com/sdelquin/pypas-cli
 Author: Sergio Delgado Quintero
 Author-email: sdelquin@gmail.com
 Maintainer-email: Sergio Delgado Quintero <sdelquin@gmail.com>
 License: MIT License
@@ -34,11 +34,12 @@
 Classifier: Programming Language :: Python :: 3
 Requires-Python: >=3.10
 Requires-Dist: prettyconf
 Requires-Dist: pytest
 Requires-Dist: requests
 Requires-Dist: rich
 Requires-Dist: setuptools
+Requires-Dist: toml
 Requires-Dist: typer
 Description-Content-Type: text/markdown
 
 # pypas-cli
```

