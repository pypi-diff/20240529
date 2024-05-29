# Comparing `tmp/pypas_cli-0.0.6.tar.gz` & `tmp/pypas_cli-0.0.7.tar.gz`

## Comparing `pypas_cli-0.0.6.tar` & `pypas_cli-0.0.7.tar`

### file list

```diff
@@ -1,17 +1,17 @@
--rw-r--r--   0        0        0      134 2020-02-02 00:00:00.000000 pypas_cli-0.0.6/CHANGELOG.md
--rw-r--r--   0        0        0      261 2020-02-02 00:00:00.000000 pypas_cli-0.0.6/justfile
--rw-r--r--   0        0        0       12 2020-02-02 00:00:00.000000 pypas_cli-0.0.6/requirements-dev.txt
--rw-r--r--   0        0        0      189 2020-02-02 00:00:00.000000 pypas_cli-0.0.6/src/pypas/__init__.py
--rw-r--r--   0        0        0     1683 2020-02-02 00:00:00.000000 pypas_cli-0.0.6/src/pypas/main.py
--rw-r--r--   0        0        0      464 2020-02-02 00:00:00.000000 pypas_cli-0.0.6/src/pypas/settings.py
--rw-r--r--   0        0        0      966 2020-02-02 00:00:00.000000 pypas_cli-0.0.6/src/pypas/lib/auth.py
--rw-r--r--   0        0        0      679 2020-02-02 00:00:00.000000 pypas_cli-0.0.6/src/pypas/lib/config.py
--rw-r--r--   0        0        0     1370 2020-02-02 00:00:00.000000 pypas_cli-0.0.6/src/pypas/lib/console.py
--rw-r--r--   0        0        0      366 2020-02-02 00:00:00.000000 pypas_cli-0.0.6/src/pypas/lib/decorators.py
--rw-r--r--   0        0        0     2693 2020-02-02 00:00:00.000000 pypas_cli-0.0.6/src/pypas/lib/exercise.py
--rw-r--r--   0        0        0     1936 2020-02-02 00:00:00.000000 pypas_cli-0.0.6/src/pypas/lib/utils.py
--rw-r--r--   0        0        0       62 2020-02-02 00:00:00.000000 pypas_cli-0.0.6/.gitignore
--rw-r--r--   0        0        0     1080 2020-02-02 00:00:00.000000 pypas_cli-0.0.6/LICENSE
--rw-r--r--   0        0        0       12 2020-02-02 00:00:00.000000 pypas_cli-0.0.6/README.md
--rw-r--r--   0        0        0      951 2020-02-02 00:00:00.000000 pypas_cli-0.0.6/pyproject.toml
--rw-r--r--   0        0        0     1975 2020-02-02 00:00:00.000000 pypas_cli-0.0.6/PKG-INFO
+-rw-r--r--   0        0        0      134 2020-02-02 00:00:00.000000 pypas_cli-0.0.7/CHANGELOG.md
+-rw-r--r--   0        0        0      261 2020-02-02 00:00:00.000000 pypas_cli-0.0.7/justfile
+-rw-r--r--   0        0        0       12 2020-02-02 00:00:00.000000 pypas_cli-0.0.7/requirements-dev.txt
+-rw-r--r--   0        0        0      189 2020-02-02 00:00:00.000000 pypas_cli-0.0.7/src/pypas/__init__.py
+-rw-r--r--   0        0        0     1683 2020-02-02 00:00:00.000000 pypas_cli-0.0.7/src/pypas/main.py
+-rw-r--r--   0        0        0      464 2020-02-02 00:00:00.000000 pypas_cli-0.0.7/src/pypas/settings.py
+-rw-r--r--   0        0        0      966 2020-02-02 00:00:00.000000 pypas_cli-0.0.7/src/pypas/lib/auth.py
+-rw-r--r--   0        0        0      679 2020-02-02 00:00:00.000000 pypas_cli-0.0.7/src/pypas/lib/config.py
+-rw-r--r--   0        0        0     1370 2020-02-02 00:00:00.000000 pypas_cli-0.0.7/src/pypas/lib/console.py
+-rw-r--r--   0        0        0      366 2020-02-02 00:00:00.000000 pypas_cli-0.0.7/src/pypas/lib/decorators.py
+-rw-r--r--   0        0        0     2698 2020-02-02 00:00:00.000000 pypas_cli-0.0.7/src/pypas/lib/exercise.py
+-rw-r--r--   0        0        0     1936 2020-02-02 00:00:00.000000 pypas_cli-0.0.7/src/pypas/lib/utils.py
+-rw-r--r--   0        0        0       62 2020-02-02 00:00:00.000000 pypas_cli-0.0.7/.gitignore
+-rw-r--r--   0        0        0     1080 2020-02-02 00:00:00.000000 pypas_cli-0.0.7/LICENSE
+-rw-r--r--   0        0        0       12 2020-02-02 00:00:00.000000 pypas_cli-0.0.7/README.md
+-rw-r--r--   0        0        0      951 2020-02-02 00:00:00.000000 pypas_cli-0.0.7/pyproject.toml
+-rw-r--r--   0        0        0     1975 2020-02-02 00:00:00.000000 pypas_cli-0.0.7/PKG-INFO
```

### Comparing `pypas_cli-0.0.6/src/pypas/main.py` & `pypas_cli-0.0.7/src/pypas/main.py`

 * *Files identical despite different names*

### Comparing `pypas_cli-0.0.6/src/pypas/lib/auth.py` & `pypas_cli-0.0.7/src/pypas/lib/auth.py`

 * *Files identical despite different names*

### Comparing `pypas_cli-0.0.6/src/pypas/lib/config.py` & `pypas_cli-0.0.7/src/pypas/lib/config.py`

 * *Files identical despite different names*

### Comparing `pypas_cli-0.0.6/src/pypas/lib/console.py` & `pypas_cli-0.0.7/src/pypas/lib/console.py`

 * *Files identical despite different names*

### Comparing `pypas_cli-0.0.6/src/pypas/lib/exercise.py` & `pypas_cli-0.0.7/src/pypas/lib/exercise.py`

 * *Files 1% similar despite different names*

```diff
@@ -66,15 +66,15 @@
                 if backup and rel_file.exists() and str(rel_file) in self.config['todo']:
                     backup_file = rel_file.with_suffix(rel_file.suffix + '.bak')
                     console.debug(f'Backup {rel_file} → {backup_file}')
                     shutil.copy(rel_file, backup_file)
                 rel_file.parent.mkdir(parents=True, exist_ok=True)
                 shutil.copy(file, rel_file)
         shutil.rmtree(src_dir, ignore_errors=True)
-        console.success('Exercise is updated to last version!')
+        console.success('Exercise has been updated to last version')
 
     @classmethod
     def from_config(cls) -> Exercise:
         return cls(Exercise.load_config()['slug'])
 
     @staticmethod
     def load_config(filename: str = settings.EXERCISE_CONFIG_FILE):
```

### Comparing `pypas_cli-0.0.6/src/pypas/lib/utils.py` & `pypas_cli-0.0.7/src/pypas/lib/utils.py`

 * *Files identical despite different names*

### Comparing `pypas_cli-0.0.6/LICENSE` & `pypas_cli-0.0.7/LICENSE`

 * *Files identical despite different names*

### Comparing `pypas_cli-0.0.6/pyproject.toml` & `pypas_cli-0.0.7/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["hatchling"]
 build-backend = "hatchling.build"
 
 [project]
 name = "pypas-cli"
-version = "0.0.6"
+version = "0.0.7"
 license = { file = "LICENSE" }
 dependencies = [
     'setuptools',
     'typer',
     'prettyconf',
     'requests',
     'rich',
```

### Comparing `pypas_cli-0.0.6/PKG-INFO` & `pypas_cli-0.0.7/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.3
 Name: pypas-cli
-Version: 0.0.6
+Version: 0.0.7
 Summary: Python Practical Assignments
 Project-URL: homepage, https://pypas.es
 Project-URL: repository, https://github.com/sdelquin/pypas-cli
 Author: Sergio Delgado Quintero
 Author-email: sdelquin@gmail.com
 Maintainer-email: Sergio Delgado Quintero <sdelquin@gmail.com>
 License: MIT License
```

