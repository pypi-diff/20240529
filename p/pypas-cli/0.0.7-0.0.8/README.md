# Comparing `tmp/pypas_cli-0.0.7.tar.gz` & `tmp/pypas_cli-0.0.8.tar.gz`

## Comparing `pypas_cli-0.0.7.tar` & `pypas_cli-0.0.8.tar`

### file list

```diff
@@ -1,17 +1,17 @@
--rw-r--r--   0        0        0      134 2020-02-02 00:00:00.000000 pypas_cli-0.0.7/CHANGELOG.md
--rw-r--r--   0        0        0      261 2020-02-02 00:00:00.000000 pypas_cli-0.0.7/justfile
--rw-r--r--   0        0        0       12 2020-02-02 00:00:00.000000 pypas_cli-0.0.7/requirements-dev.txt
--rw-r--r--   0        0        0      189 2020-02-02 00:00:00.000000 pypas_cli-0.0.7/src/pypas/__init__.py
--rw-r--r--   0        0        0     1683 2020-02-02 00:00:00.000000 pypas_cli-0.0.7/src/pypas/main.py
--rw-r--r--   0        0        0      464 2020-02-02 00:00:00.000000 pypas_cli-0.0.7/src/pypas/settings.py
--rw-r--r--   0        0        0      966 2020-02-02 00:00:00.000000 pypas_cli-0.0.7/src/pypas/lib/auth.py
--rw-r--r--   0        0        0      679 2020-02-02 00:00:00.000000 pypas_cli-0.0.7/src/pypas/lib/config.py
--rw-r--r--   0        0        0     1370 2020-02-02 00:00:00.000000 pypas_cli-0.0.7/src/pypas/lib/console.py
--rw-r--r--   0        0        0      366 2020-02-02 00:00:00.000000 pypas_cli-0.0.7/src/pypas/lib/decorators.py
--rw-r--r--   0        0        0     2698 2020-02-02 00:00:00.000000 pypas_cli-0.0.7/src/pypas/lib/exercise.py
--rw-r--r--   0        0        0     1936 2020-02-02 00:00:00.000000 pypas_cli-0.0.7/src/pypas/lib/utils.py
--rw-r--r--   0        0        0       62 2020-02-02 00:00:00.000000 pypas_cli-0.0.7/.gitignore
--rw-r--r--   0        0        0     1080 2020-02-02 00:00:00.000000 pypas_cli-0.0.7/LICENSE
--rw-r--r--   0        0        0       12 2020-02-02 00:00:00.000000 pypas_cli-0.0.7/README.md
--rw-r--r--   0        0        0      951 2020-02-02 00:00:00.000000 pypas_cli-0.0.7/pyproject.toml
--rw-r--r--   0        0        0     1975 2020-02-02 00:00:00.000000 pypas_cli-0.0.7/PKG-INFO
+-rw-r--r--   0        0        0      134 2020-02-02 00:00:00.000000 pypas_cli-0.0.8/CHANGELOG.md
+-rw-r--r--   0        0        0      261 2020-02-02 00:00:00.000000 pypas_cli-0.0.8/justfile
+-rw-r--r--   0        0        0       12 2020-02-02 00:00:00.000000 pypas_cli-0.0.8/requirements-dev.txt
+-rw-r--r--   0        0        0      189 2020-02-02 00:00:00.000000 pypas_cli-0.0.8/src/pypas/__init__.py
+-rw-r--r--   0        0        0     1683 2020-02-02 00:00:00.000000 pypas_cli-0.0.8/src/pypas/main.py
+-rw-r--r--   0        0        0      464 2020-02-02 00:00:00.000000 pypas_cli-0.0.8/src/pypas/settings.py
+-rw-r--r--   0        0        0      966 2020-02-02 00:00:00.000000 pypas_cli-0.0.8/src/pypas/lib/auth.py
+-rw-r--r--   0        0        0      679 2020-02-02 00:00:00.000000 pypas_cli-0.0.8/src/pypas/lib/config.py
+-rw-r--r--   0        0        0     1370 2020-02-02 00:00:00.000000 pypas_cli-0.0.8/src/pypas/lib/console.py
+-rw-r--r--   0        0        0      366 2020-02-02 00:00:00.000000 pypas_cli-0.0.8/src/pypas/lib/decorators.py
+-rw-r--r--   0        0        0     2698 2020-02-02 00:00:00.000000 pypas_cli-0.0.8/src/pypas/lib/exercise.py
+-rw-r--r--   0        0        0     1936 2020-02-02 00:00:00.000000 pypas_cli-0.0.8/src/pypas/lib/utils.py
+-rw-r--r--   0        0        0       62 2020-02-02 00:00:00.000000 pypas_cli-0.0.8/.gitignore
+-rw-r--r--   0        0        0     1080 2020-02-02 00:00:00.000000 pypas_cli-0.0.8/LICENSE
+-rw-r--r--   0        0        0       12 2020-02-02 00:00:00.000000 pypas_cli-0.0.8/README.md
+-rw-r--r--   0        0        0      951 2020-02-02 00:00:00.000000 pypas_cli-0.0.8/pyproject.toml
+-rw-r--r--   0        0        0     1975 2020-02-02 00:00:00.000000 pypas_cli-0.0.8/PKG-INFO
```

### Comparing `pypas_cli-0.0.7/src/pypas/main.py` & `pypas_cli-0.0.8/src/pypas/main.py`

 * *Files identical despite different names*

### Comparing `pypas_cli-0.0.7/src/pypas/lib/auth.py` & `pypas_cli-0.0.8/src/pypas/lib/auth.py`

 * *Files 1% similar despite different names*

```diff
@@ -15,15 +15,15 @@
     def authenticate(self) -> bool:
         console.debug(f'Authenticating user at: [i]{self.token_validation_url}', end=' ')
         response = requests.get(self.token_validation_url)
         if response.status_code == HTTPStatus.OK:
             data = response.json()
             console.check()
             console.success(
-                f'Congratulations [i]{data['name']}[/i]. You have been successfully authenticated'
+                f'Congratulations [i]{data["name"]}[/i]. You have been successfully authenticated'
             )
             return True
         else:
             console.fail()
             console.error('User cannot be authenticated')
             console.debug('Check the access token with the administrator')
             return False
```

### Comparing `pypas_cli-0.0.7/src/pypas/lib/config.py` & `pypas_cli-0.0.8/src/pypas/lib/config.py`

 * *Files identical despite different names*

### Comparing `pypas_cli-0.0.7/src/pypas/lib/console.py` & `pypas_cli-0.0.8/src/pypas/lib/console.py`

 * *Files identical despite different names*

### Comparing `pypas_cli-0.0.7/src/pypas/lib/exercise.py` & `pypas_cli-0.0.8/src/pypas/lib/exercise.py`

 * *Files identical despite different names*

### Comparing `pypas_cli-0.0.7/src/pypas/lib/utils.py` & `pypas_cli-0.0.8/src/pypas/lib/utils.py`

 * *Files identical despite different names*

### Comparing `pypas_cli-0.0.7/LICENSE` & `pypas_cli-0.0.8/LICENSE`

 * *Files identical despite different names*

### Comparing `pypas_cli-0.0.7/pyproject.toml` & `pypas_cli-0.0.8/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["hatchling"]
 build-backend = "hatchling.build"
 
 [project]
 name = "pypas-cli"
-version = "0.0.7"
+version = "0.0.8"
 license = { file = "LICENSE" }
 dependencies = [
     'setuptools',
     'typer',
     'prettyconf',
     'requests',
     'rich',
```

### Comparing `pypas_cli-0.0.7/PKG-INFO` & `pypas_cli-0.0.8/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.3
 Name: pypas-cli
-Version: 0.0.7
+Version: 0.0.8
 Summary: Python Practical Assignments
 Project-URL: homepage, https://pypas.es
 Project-URL: repository, https://github.com/sdelquin/pypas-cli
 Author: Sergio Delgado Quintero
 Author-email: sdelquin@gmail.com
 Maintainer-email: Sergio Delgado Quintero <sdelquin@gmail.com>
 License: MIT License
```

