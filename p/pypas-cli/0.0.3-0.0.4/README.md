# Comparing `tmp/pypas_cli-0.0.3.tar.gz` & `tmp/pypas_cli-0.0.4.tar.gz`

## Comparing `pypas_cli-0.0.3.tar` & `pypas_cli-0.0.4.tar`

### file list

```diff
@@ -1,14 +1,15 @@
--rw-r--r--   0        0        0      134 2020-02-02 00:00:00.000000 pypas_cli-0.0.3/CHANGELOG.md
--rw-r--r--   0        0        0      261 2020-02-02 00:00:00.000000 pypas_cli-0.0.3/justfile
--rw-r--r--   0        0        0       12 2020-02-02 00:00:00.000000 pypas_cli-0.0.3/requirements-dev.txt
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 pypas_cli-0.0.3/src/pypas/__init__.py
--rw-r--r--   0        0        0      958 2020-02-02 00:00:00.000000 pypas_cli-0.0.3/src/pypas/main.py
--rw-r--r--   0        0        0      201 2020-02-02 00:00:00.000000 pypas_cli-0.0.3/src/pypas/settings.py
--rw-r--r--   0        0        0      254 2020-02-02 00:00:00.000000 pypas_cli-0.0.3/src/pypas/lib/console.py
--rw-r--r--   0        0        0        7 2020-02-02 00:00:00.000000 pypas_cli-0.0.3/src/pypas/lib/core.py
--rw-r--r--   0        0        0      777 2020-02-02 00:00:00.000000 pypas_cli-0.0.3/src/pypas/lib/utils.py
--rw-r--r--   0        0        0       62 2020-02-02 00:00:00.000000 pypas_cli-0.0.3/.gitignore
--rw-r--r--   0        0        0     1080 2020-02-02 00:00:00.000000 pypas_cli-0.0.3/LICENSE
--rw-r--r--   0        0        0       12 2020-02-02 00:00:00.000000 pypas_cli-0.0.3/README.md
--rw-r--r--   0        0        0      951 2020-02-02 00:00:00.000000 pypas_cli-0.0.3/pyproject.toml
--rw-r--r--   0        0        0     1975 2020-02-02 00:00:00.000000 pypas_cli-0.0.3/PKG-INFO
+-rw-r--r--   0        0        0      134 2020-02-02 00:00:00.000000 pypas_cli-0.0.4/CHANGELOG.md
+-rw-r--r--   0        0        0      261 2020-02-02 00:00:00.000000 pypas_cli-0.0.4/justfile
+-rw-r--r--   0        0        0       12 2020-02-02 00:00:00.000000 pypas_cli-0.0.4/requirements-dev.txt
+-rw-r--r--   0        0        0      115 2020-02-02 00:00:00.000000 pypas_cli-0.0.4/src/pypas/__init__.py
+-rw-r--r--   0        0        0     1034 2020-02-02 00:00:00.000000 pypas_cli-0.0.4/src/pypas/main.py
+-rw-r--r--   0        0        0      278 2020-02-02 00:00:00.000000 pypas_cli-0.0.4/src/pypas/settings.py
+-rw-r--r--   0        0        0      300 2020-02-02 00:00:00.000000 pypas_cli-0.0.4/src/pypas/lib/console.py
+-rw-r--r--   0        0        0      366 2020-02-02 00:00:00.000000 pypas_cli-0.0.4/src/pypas/lib/decorators.py
+-rw-r--r--   0        0        0     1990 2020-02-02 00:00:00.000000 pypas_cli-0.0.4/src/pypas/lib/exercise.py
+-rw-r--r--   0        0        0     1936 2020-02-02 00:00:00.000000 pypas_cli-0.0.4/src/pypas/lib/utils.py
+-rw-r--r--   0        0        0       62 2020-02-02 00:00:00.000000 pypas_cli-0.0.4/.gitignore
+-rw-r--r--   0        0        0     1080 2020-02-02 00:00:00.000000 pypas_cli-0.0.4/LICENSE
+-rw-r--r--   0        0        0       12 2020-02-02 00:00:00.000000 pypas_cli-0.0.4/README.md
+-rw-r--r--   0        0        0      939 2020-02-02 00:00:00.000000 pypas_cli-0.0.4/pyproject.toml
+-rw-r--r--   0        0        0     1955 2020-02-02 00:00:00.000000 pypas_cli-0.0.4/PKG-INFO
```

### Comparing `pypas_cli-0.0.3/src/pypas/main.py` & `pypas_cli-0.0.4/src/pypas/main.py`

 * *Files 23% similar despite different names*

```diff
@@ -1,40 +1,43 @@
-import os
-import zipfile
-from urllib.parse import urljoin
-
 import typer
 from rich import print
+from rich.prompt import Confirm
 
-from pypas import settings
-from pypas.lib import utils
-from pypas.lib.console import console
+from pypas import Exercise, console
+from pypas.lib.decorators import inside_exercise
 
 app = typer.Typer(
     add_completion=False,
     help='✨ pypas',
     no_args_is_help=True,
 )
 
 
 @app.command()
-def run():
-    print('Hi there!')
+def get(exercise_slug: str):
+    if (exercise := Exercise(exercise_slug)).folder_exists():
+        console.print(f'Folder {exercise.cwd_folder} already exists!', style='warning')
+        console.print(
+            '[italic]If continue, files coming from server will [red]OVERWRITE[/red] your existing files'
+        )
+        if not Confirm.ask('Continue', default=False):
+            return
+    if exercise.download():
+        exercise.unzip()
+        console.print(f'Exercise is available at [note]{exercise.cwd_folder}[/note] [success]✔')
 
 
 @app.command()
-def get(exercise_slug: str):
-    exercise_url = urljoin(settings.PYPAS_EXERCISES_URLPATH, exercise_slug + '/')
-    console.print(f'Getting exercise from: {exercise_url}')
-    fname = utils.download(exercise_url, f'{exercise_slug}.zip', save_temp=True)
-    console.print('Inflating exercise bundle', end=' ')
-    with zipfile.ZipFile(fname) as zip_ref:
-        zip_ref.extractall()
-    console.print('✔', style='success')
-    os.remove(fname)
-    console.print(
-        f'Exercise is available at folder [info]./{exercise_slug}[/info] [success]✔[/success]'
-    )
+@inside_exercise
+def doc():
+    if exercise := Exercise.from_config():
+        exercise.open_docs()
+
+
+@app.command()
+@inside_exercise
+def update():
+    print('TODO!')
 
 
 if __name__ == '__main__':
     app()
```

### Comparing `pypas_cli-0.0.3/LICENSE` & `pypas_cli-0.0.4/LICENSE`

 * *Files identical despite different names*

### Comparing `pypas_cli-0.0.3/pyproject.toml` & `pypas_cli-0.0.4/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,22 +1,21 @@
 [build-system]
 requires = ["hatchling"]
 build-backend = "hatchling.build"
 
 [project]
 name = "pypas-cli"
-version = "0.0.3"
+version = "0.0.4"
 license = { file = "LICENSE" }
 dependencies = [
     'setuptools',
     'typer',
     'prettyconf',
     'requests',
     'rich',
-    'tqdm',
     'pytest',
 ]
 authors = [
     { email = "sdelquin@gmail.com" },
     { name = "Sergio Delgado Quintero" },
 ]
 maintainers = [
```

### Comparing `pypas_cli-0.0.3/PKG-INFO` & `pypas_cli-0.0.4/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.3
 Name: pypas-cli
-Version: 0.0.3
+Version: 0.0.4
 Summary: Python Practical Assignments
 Project-URL: homepage, https://pypas.es
 Project-URL: repository, https://github.com/sdelquin/pypas-cli
 Author: Sergio Delgado Quintero
 Author-email: sdelquin@gmail.com
 Maintainer-email: Sergio Delgado Quintero <sdelquin@gmail.com>
 License: MIT License
@@ -34,12 +34,11 @@
 Classifier: Programming Language :: Python :: 3
 Requires-Python: >=3.10
 Requires-Dist: prettyconf
 Requires-Dist: pytest
 Requires-Dist: requests
 Requires-Dist: rich
 Requires-Dist: setuptools
-Requires-Dist: tqdm
 Requires-Dist: typer
 Description-Content-Type: text/markdown
 
 # pypas-cli
```

