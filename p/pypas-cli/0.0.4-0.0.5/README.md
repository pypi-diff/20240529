# Comparing `tmp/pypas_cli-0.0.4.tar.gz` & `tmp/pypas_cli-0.0.5.tar.gz`

## Comparing `pypas_cli-0.0.4.tar` & `pypas_cli-0.0.5.tar`

### file list

```diff
@@ -1,15 +1,15 @@
--rw-r--r--   0        0        0      134 2020-02-02 00:00:00.000000 pypas_cli-0.0.4/CHANGELOG.md
--rw-r--r--   0        0        0      261 2020-02-02 00:00:00.000000 pypas_cli-0.0.4/justfile
--rw-r--r--   0        0        0       12 2020-02-02 00:00:00.000000 pypas_cli-0.0.4/requirements-dev.txt
--rw-r--r--   0        0        0      115 2020-02-02 00:00:00.000000 pypas_cli-0.0.4/src/pypas/__init__.py
--rw-r--r--   0        0        0     1034 2020-02-02 00:00:00.000000 pypas_cli-0.0.4/src/pypas/main.py
--rw-r--r--   0        0        0      278 2020-02-02 00:00:00.000000 pypas_cli-0.0.4/src/pypas/settings.py
--rw-r--r--   0        0        0      300 2020-02-02 00:00:00.000000 pypas_cli-0.0.4/src/pypas/lib/console.py
--rw-r--r--   0        0        0      366 2020-02-02 00:00:00.000000 pypas_cli-0.0.4/src/pypas/lib/decorators.py
--rw-r--r--   0        0        0     1990 2020-02-02 00:00:00.000000 pypas_cli-0.0.4/src/pypas/lib/exercise.py
--rw-r--r--   0        0        0     1936 2020-02-02 00:00:00.000000 pypas_cli-0.0.4/src/pypas/lib/utils.py
--rw-r--r--   0        0        0       62 2020-02-02 00:00:00.000000 pypas_cli-0.0.4/.gitignore
--rw-r--r--   0        0        0     1080 2020-02-02 00:00:00.000000 pypas_cli-0.0.4/LICENSE
--rw-r--r--   0        0        0       12 2020-02-02 00:00:00.000000 pypas_cli-0.0.4/README.md
--rw-r--r--   0        0        0      939 2020-02-02 00:00:00.000000 pypas_cli-0.0.4/pyproject.toml
--rw-r--r--   0        0        0     1955 2020-02-02 00:00:00.000000 pypas_cli-0.0.4/PKG-INFO
+-rw-r--r--   0        0        0      134 2020-02-02 00:00:00.000000 pypas_cli-0.0.5/CHANGELOG.md
+-rw-r--r--   0        0        0      261 2020-02-02 00:00:00.000000 pypas_cli-0.0.5/justfile
+-rw-r--r--   0        0        0       12 2020-02-02 00:00:00.000000 pypas_cli-0.0.5/requirements-dev.txt
+-rw-r--r--   0        0        0      115 2020-02-02 00:00:00.000000 pypas_cli-0.0.5/src/pypas/__init__.py
+-rw-r--r--   0        0        0     1433 2020-02-02 00:00:00.000000 pypas_cli-0.0.5/src/pypas/main.py
+-rw-r--r--   0        0        0      278 2020-02-02 00:00:00.000000 pypas_cli-0.0.5/src/pypas/settings.py
+-rw-r--r--   0        0        0      708 2020-02-02 00:00:00.000000 pypas_cli-0.0.5/src/pypas/lib/console.py
+-rw-r--r--   0        0        0      366 2020-02-02 00:00:00.000000 pypas_cli-0.0.5/src/pypas/lib/decorators.py
+-rw-r--r--   0        0        0     2746 2020-02-02 00:00:00.000000 pypas_cli-0.0.5/src/pypas/lib/exercise.py
+-rw-r--r--   0        0        0     1936 2020-02-02 00:00:00.000000 pypas_cli-0.0.5/src/pypas/lib/utils.py
+-rw-r--r--   0        0        0       62 2020-02-02 00:00:00.000000 pypas_cli-0.0.5/.gitignore
+-rw-r--r--   0        0        0     1080 2020-02-02 00:00:00.000000 pypas_cli-0.0.5/LICENSE
+-rw-r--r--   0        0        0       12 2020-02-02 00:00:00.000000 pypas_cli-0.0.5/README.md
+-rw-r--r--   0        0        0      939 2020-02-02 00:00:00.000000 pypas_cli-0.0.5/pyproject.toml
+-rw-r--r--   0        0        0     1955 2020-02-02 00:00:00.000000 pypas_cli-0.0.5/PKG-INFO
```

### Comparing `pypas_cli-0.0.4/src/pypas/main.py` & `pypas_cli-0.0.5/src/pypas/main.py`

 * *Files 22% similar despite different names*

```diff
@@ -1,23 +1,23 @@
 import typer
-from rich import print
 from rich.prompt import Confirm
 
 from pypas import Exercise, console
 from pypas.lib.decorators import inside_exercise
 
 app = typer.Typer(
     add_completion=False,
-    help='✨ pypas',
+    help='✨ pypas → Python Practical Assignments',
     no_args_is_help=True,
 )
 
 
 @app.command()
-def get(exercise_slug: str):
+def get(exercise_slug: str = typer.Argument(help='Slug of exercise')):
+    """Get exercise."""
     if (exercise := Exercise(exercise_slug)).folder_exists():
         console.print(f'Folder {exercise.cwd_folder} already exists!', style='warning')
         console.print(
             '[italic]If continue, files coming from server will [red]OVERWRITE[/red] your existing files'
         )
         if not Confirm.ask('Continue', default=False):
             return
@@ -25,19 +25,28 @@
         exercise.unzip()
         console.print(f'Exercise is available at [note]{exercise.cwd_folder}[/note] [success]✔')
 
 
 @app.command()
 @inside_exercise
 def doc():
-    if exercise := Exercise.from_config():
-        exercise.open_docs()
+    """Open documentation for exercise."""
+    exercise = Exercise.from_config()
+    exercise.open_docs()
 
 
 @app.command()
 @inside_exercise
-def update():
-    print('TODO!')
+def update(
+    force: bool = typer.Option(
+        False, '--force', '-f', help='Force update and omit backup of existing files'
+    ),
+):
+    """Update exercise."""
+    exercise = Exercise.from_config()
+    exercise.download()
+    dir = exercise.unzip(to_tmp_dir=True)
+    exercise.update(src_dir=dir, backup=not force)
 
 
 if __name__ == '__main__':
     app()
```

### Comparing `pypas_cli-0.0.4/src/pypas/lib/exercise.py` & `pypas_cli-0.0.5/src/pypas/lib/exercise.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,10 +1,12 @@
 from __future__ import annotations
 
 import os
+import shutil
+import tempfile
 import zipfile
 from pathlib import Path
 from urllib.parse import urljoin
 
 import tomllib
 from pypas import settings
 
@@ -40,31 +42,42 @@
 
     def download(self) -> Path | None:
         console.print(f'Getting exercise from: [italic]{self.url}')
         if downloaded_zip := utils.download(self.url, self.zipname, save_temp=True):
             self.downloaded_zip = downloaded_zip
         return downloaded_zip
 
-    def unzip(self):
+    def unzip(self, to_tmp_dir: bool = False) -> Path:
+        tmp_dir = tempfile.TemporaryDirectory(delete=False)
+        target_dir = Path(tmp_dir.name) if to_tmp_dir else self.folder
         console.print('Inflating exercise bundle', end=' ')
         with zipfile.ZipFile(self.downloaded_zip) as zip_ref:
-            zip_ref.extractall()
-        console.print('✔', style='success')
+            zip_ref.extractall(target_dir)
+        console.done()
         os.remove(self.downloaded_zip)
+        return target_dir
 
     def open_docs(self):
         os.system(f'{utils.get_open_cmd()} docs/README.pdf')
 
+    def update(self, src_dir: Path, backup: bool = True):
+        for file in src_dir.glob('**/*'):
+            if file.is_file():
+                rel_file = file.relative_to(src_dir)
+                if backup and rel_file.exists() and str(rel_file) in self.config['todo']:
+                    backup_file = rel_file.with_suffix(rel_file.suffix + '.bak')
+                    console.print(f'Backup {rel_file} → {backup_file}', end=' ')
+                    shutil.copy(rel_file, backup_file)
+                    console.done()
+                rel_file.parent.mkdir(parents=True, exist_ok=True)
+                shutil.copy(file, rel_file)
+        shutil.rmtree(src_dir, ignore_errors=True)
+        console.great('Exercise is updated to last version!')
+
     @classmethod
-    def from_config(cls) -> Exercise | None:
-        try:
-            return cls(Exercise.load_config()['slug'])
-        except KeyError:
-            console.print(
-                f'Config file {settings.EXERCISE_CONFIG_FILE} is corrupt!', style='danger'
-            )
-            return None
+    def from_config(cls) -> Exercise:
+        return cls(Exercise.load_config()['slug'])
 
     @staticmethod
     def load_config(filename: str = settings.EXERCISE_CONFIG_FILE):
         with open(filename, 'rb') as f:
             return tomllib.load(f)
```

### Comparing `pypas_cli-0.0.4/src/pypas/lib/utils.py` & `pypas_cli-0.0.5/src/pypas/lib/utils.py`

 * *Files identical despite different names*

### Comparing `pypas_cli-0.0.4/LICENSE` & `pypas_cli-0.0.5/LICENSE`

 * *Files identical despite different names*

### Comparing `pypas_cli-0.0.4/pyproject.toml` & `pypas_cli-0.0.5/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["hatchling"]
 build-backend = "hatchling.build"
 
 [project]
 name = "pypas-cli"
-version = "0.0.4"
+version = "0.0.5"
 license = { file = "LICENSE" }
 dependencies = [
     'setuptools',
     'typer',
     'prettyconf',
     'requests',
     'rich',
```

### Comparing `pypas_cli-0.0.4/PKG-INFO` & `pypas_cli-0.0.5/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.3
 Name: pypas-cli
-Version: 0.0.4
+Version: 0.0.5
 Summary: Python Practical Assignments
 Project-URL: homepage, https://pypas.es
 Project-URL: repository, https://github.com/sdelquin/pypas-cli
 Author: Sergio Delgado Quintero
 Author-email: sdelquin@gmail.com
 Maintainer-email: Sergio Delgado Quintero <sdelquin@gmail.com>
 License: MIT License
```

