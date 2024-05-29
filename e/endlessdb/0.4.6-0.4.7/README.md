# Comparing `tmp/endlessdb-0.4.6.tar.gz` & `tmp/endlessdb-0.4.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "endlessdb-0.4.6.tar", last modified: Wed May 29 19:11:33 2024, max compression
+gzip compressed data, was "endlessdb-0.4.7.tar", last modified: Wed May 29 20:05:44 2024, max compression
```

## Comparing `endlessdb-0.4.6.tar` & `endlessdb-0.4.7.tar`

### file list

```diff
@@ -1,17 +1,17 @@
-drwxrwxrwx   0        0        0        0 2024-05-29 19:11:33.509070 endlessdb-0.4.6/
--rw-rw-rw-   0        0        0    11524 2024-05-20 13:50:18.000000 endlessdb-0.4.6/LICENSE.txt
--rw-rw-rw-   0        0        0    14363 2024-05-29 19:11:33.506069 endlessdb-0.4.6/PKG-INFO
--rw-rw-rw-   0        0        0      355 2024-05-29 01:30:15.000000 endlessdb-0.4.6/README.md
--rw-rw-rw-   0        0        0      886 2024-05-29 19:02:02.000000 endlessdb-0.4.6/pyproject.toml
--rw-rw-rw-   0        0        0       42 2024-05-29 19:11:33.510065 endlessdb-0.4.6/setup.cfg
-drwxrwxrwx   0        0        0        0 2024-05-29 19:11:33.480065 endlessdb-0.4.6/src/
--rw-rw-rw-   0        0        0       23 2024-05-28 22:01:22.000000 endlessdb-0.4.6/src/__init__.py
-drwxrwxrwx   0        0        0        0 2024-05-29 19:11:33.503068 endlessdb-0.4.6/src/endlessdb.egg-info/
--rw-rw-rw-   0        0        0    14363 2024-05-29 19:11:33.000000 endlessdb-0.4.6/src/endlessdb.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      278 2024-05-29 19:11:33.000000 endlessdb-0.4.6/src/endlessdb.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-05-29 19:11:33.000000 endlessdb-0.4.6/src/endlessdb.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       29 2024-05-29 19:11:33.000000 endlessdb-0.4.6/src/endlessdb.egg-info/requires.txt
--rw-rw-rw-   0        0        0       19 2024-05-29 19:11:33.000000 endlessdb-0.4.6/src/endlessdb.egg-info/top_level.txt
--rw-rw-rw-   0        0        0    40632 2024-05-29 19:10:53.000000 endlessdb-0.4.6/src/endlessdb.py
-drwxrwxrwx   0        0        0        0 2024-05-29 19:11:33.499061 endlessdb-0.4.6/tests/
--rw-rw-rw-   0        0        0    10866 2024-05-29 18:55:49.000000 endlessdb-0.4.6/tests/test_endlessddb.py
+drwxrwxrwx   0        0        0        0 2024-05-29 20:05:44.624713 endlessdb-0.4.7/
+-rw-rw-rw-   0        0        0    11524 2024-05-20 13:50:18.000000 endlessdb-0.4.7/LICENSE.txt
+-rw-rw-rw-   0        0        0    14363 2024-05-29 20:05:44.622710 endlessdb-0.4.7/PKG-INFO
+-rw-rw-rw-   0        0        0      355 2024-05-29 01:30:15.000000 endlessdb-0.4.7/README.md
+-rw-rw-rw-   0        0        0      886 2024-05-29 20:05:31.000000 endlessdb-0.4.7/pyproject.toml
+-rw-rw-rw-   0        0        0       42 2024-05-29 20:05:44.625714 endlessdb-0.4.7/setup.cfg
+drwxrwxrwx   0        0        0        0 2024-05-29 20:05:44.608300 endlessdb-0.4.7/src/
+-rw-rw-rw-   0        0        0       23 2024-05-28 22:01:22.000000 endlessdb-0.4.7/src/__init__.py
+drwxrwxrwx   0        0        0        0 2024-05-29 20:05:44.621709 endlessdb-0.4.7/src/endlessdb.egg-info/
+-rw-rw-rw-   0        0        0    14363 2024-05-29 20:05:44.000000 endlessdb-0.4.7/src/endlessdb.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      278 2024-05-29 20:05:44.000000 endlessdb-0.4.7/src/endlessdb.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-05-29 20:05:44.000000 endlessdb-0.4.7/src/endlessdb.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       29 2024-05-29 20:05:44.000000 endlessdb-0.4.7/src/endlessdb.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       19 2024-05-29 20:05:44.000000 endlessdb-0.4.7/src/endlessdb.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0    40991 2024-05-29 20:04:39.000000 endlessdb-0.4.7/src/endlessdb.py
+drwxrwxrwx   0        0        0        0 2024-05-29 20:05:44.619710 endlessdb-0.4.7/tests/
+-rw-rw-rw-   0        0        0    10866 2024-05-29 18:55:49.000000 endlessdb-0.4.7/tests/test_endlessddb.py
```

### Comparing `endlessdb-0.4.6/LICENSE.txt` & `endlessdb-0.4.7/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `endlessdb-0.4.6/PKG-INFO` & `endlessdb-0.4.7/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: endlessdb
-Version: 0.4.6
+Version: 0.4.7
 Summary: Endless Database with pyyaml and pymongo
 Author-email: Andrew Berlin <a.berlin@33solutions.company>
 Maintainer-email: Andrew Berlin <a.berlin@33solutions.company>
 License: Apache License
                                    Version 2.0, January 2004
                                 http://www.apache.org/licenses/
```

### Comparing `endlessdb-0.4.6/pyproject.toml` & `endlessdb-0.4.7/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [project]
 name = "endlessdb"
-version = "0.4.6"
+version = "0.4.7"
 requires-python = ">=3.8"
 description = "Endless Database with pyyaml and pymongo"
 readme = "README.md"
 license = {file = "LICENSE.txt"}
 
 classifiers = [
     "Development Status :: 4 - Beta",
```

### Comparing `endlessdb-0.4.6/src/endlessdb.egg-info/PKG-INFO` & `endlessdb-0.4.7/src/endlessdb.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: endlessdb
-Version: 0.4.6
+Version: 0.4.7
 Summary: Endless Database with pyyaml and pymongo
 Author-email: Andrew Berlin <a.berlin@33solutions.company>
 Maintainer-email: Andrew Berlin <a.berlin@33solutions.company>
 License: Apache License
                                    Version 2.0, January 2004
                                 http://www.apache.org/licenses/
```

### Comparing `endlessdb-0.4.6/src/endlessdb.py` & `endlessdb-0.4.7/src/endlessdb.py`

 * *Files 1% similar despite different names*

```diff
@@ -45,18 +45,24 @@
         self._logger.error(f"{self.name}: {msg}")
 
 class EndlessConfiguration():
     _override = {}
     
     def __init__(self) -> None:
         if type(self) == EndlessConfiguration:
-            self.CONFIG_COLLECTION = "config"
-            self.CONFIG_YML: str = "config.yml"
+            self.MONGO_HOST = os.environ.get("CORE_MONGO_HOST", "mongo")
+            self.MONGO_PORT = int(os.environ.get("CORE_MONGO_PORT", 27017))
+            self.MONGO_USER = os.environ.get("CORE_MONGO_USER", "root")
+            self.MONGO_PASSWORD = os.environ.get("CORE_MONGO_PASSWORD", "root")
+            self.MONGO_DATABASE = os.environ.get("CORE_MONGO_DATABASE", "endlessdb")
             self.MONGO_URI = "mongodb://localhost:27017/"
             self.MONGO_DATABASE = "endlessdb"
+            
+            self.CONFIG_COLLECTION = "config"
+            self.CONFIG_YML: str = "~/config.yml"            
         else:
             self.override()
     
     @classmethod
     def apply(cls):
         if issubclass(cls, EndlessConfiguration):
             if len(cls.__bases__) > 0 and issubclass(cls.__bases__[0], EndlessConfiguration):
@@ -661,16 +667,15 @@
     def __init__(self, _, url = None, host = "localhost", port = 27017, user = "", password = ""):
         self._cfg = EndlessConfiguration()
         self.debug = False
         self._ = _
         self.__ = _.__dict__          
         self._collections = {}
         self._documents = {}
-        path = Path(__file__).parent.parent.resolve()
-        self._defaults_collection = CollectionLogicContainer.from_yml(path/self._cfg.CONFIG_YML)
+        self._defaults_collection = CollectionLogicContainer.from_yml(self._cfg.CONFIG_YML)
         defaults = self.defaults()
         
         self._url = self.url_info(self._cfg.MONGO_URI)
         self._key = self._cfg.MONGO_DATABASE
         
         self._mongo = pymongo.MongoClient(self._cfg.MONGO_URI, connect=False)
         self._edb = self._mongo[self._key]
```

### Comparing `endlessdb-0.4.6/tests/test_endlessddb.py` & `endlessdb-0.4.7/tests/test_endlessddb.py`

 * *Files identical despite different names*

