# Comparing `tmp/beambusters-1.3.5.tar.gz` & `tmp/beambusters-1.3.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "beambusters-1.3.5.tar", max compression
+gzip compressed data, was "beambusters-1.3.6.tar", max compression
```

## Comparing `beambusters-1.3.5.tar` & `beambusters-1.3.6.tar`

### file list

```diff
@@ -1,8 +1,8 @@
--rw-r--r--   0        0        0    35149 2024-05-25 13:15:02.500218 beambusters-1.3.5/LICENSE
--rw-r--r--   0        0        0      630 2024-05-25 13:15:02.500218 beambusters-1.3.5/README.md
--rwxr-xr-x   0        0        0        0 2024-05-25 13:15:02.500218 beambusters-1.3.5/beambusters/__init__.py
--rw-r--r--   0        0        0    12068 2024-05-25 13:15:02.500218 beambusters-1.3.5/beambusters/main.py
--rwxr-xr-x   0        0        0     3562 2024-05-25 13:15:02.500218 beambusters-1.3.5/beambusters/settings.py
--rwxr-xr-x   0        0        0     1394 2024-05-25 13:15:02.500218 beambusters-1.3.5/beambusters/utils.py
--rw-r--r--   0        0        0     2026 2024-05-25 13:15:11.936194 beambusters-1.3.5/pyproject.toml
--rw-r--r--   0        0        0     3962 1970-01-01 00:00:00.000000 beambusters-1.3.5/PKG-INFO
+-rw-r--r--   0        0        0    35149 2024-05-29 13:22:14.704788 beambusters-1.3.6/LICENSE
+-rw-r--r--   0        0        0      630 2024-05-29 13:22:14.704788 beambusters-1.3.6/README.md
+-rwxr-xr-x   0        0        0        0 2024-05-29 13:22:14.704788 beambusters-1.3.6/beambusters/__init__.py
+-rw-r--r--   0        0        0    12068 2024-05-29 13:22:14.704788 beambusters-1.3.6/beambusters/main.py
+-rwxr-xr-x   0        0        0     3562 2024-05-29 13:22:14.704788 beambusters-1.3.6/beambusters/settings.py
+-rwxr-xr-x   0        0        0     1394 2024-05-29 13:22:14.704788 beambusters-1.3.6/beambusters/utils.py
+-rw-r--r--   0        0        0     2026 2024-05-29 13:22:22.524846 beambusters-1.3.6/pyproject.toml
+-rw-r--r--   0        0        0     3962 1970-01-01 00:00:00.000000 beambusters-1.3.6/PKG-INFO
```

### Comparing `beambusters-1.3.5/LICENSE` & `beambusters-1.3.6/LICENSE`

 * *Files identical despite different names*

### Comparing `beambusters-1.3.5/README.md` & `beambusters-1.3.6/README.md`

 * *Files identical despite different names*

### Comparing `beambusters-1.3.5/beambusters/main.py` & `beambusters-1.3.6/beambusters/main.py`

 * *Files identical despite different names*

### Comparing `beambusters-1.3.5/beambusters/settings.py` & `beambusters-1.3.6/beambusters/settings.py`

 * *Files identical despite different names*

### Comparing `beambusters-1.3.5/beambusters/utils.py` & `beambusters-1.3.6/beambusters/utils.py`

 * *Files identical despite different names*

### Comparing `beambusters-1.3.5/pyproject.toml` & `beambusters-1.3.6/pyproject.toml`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "beambusters"
-version = "1.3.5"
+version = "1.3.6"
 description = ""
 authors = ["Ana Rodrigues <anananacr@gmail.com>"]
 readme = "README.md"
 
 [tool.poetry.scripts]
 beambusters = "beambusters.main:app"
 
@@ -88,13 +88,13 @@
 tomlkit = "0.12.3"
 trove-classifiers = "2024.2.23"
 typing-extensions = "4.10.0"
 tzdata = "2024.1"
 urllib3 = "2.2.1"
 virtualenv = "20.25.1"
 zipp = "3.17.0"
-bblib = "2.1.3"
+bblib = "2.1.4"
 
 
 [build-system]
 requires = ["poetry-core"]
 build-backend = "poetry.core.masonry.api"
```

### Comparing `beambusters-1.3.5/PKG-INFO` & `beambusters-1.3.6/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,21 +1,21 @@
 Metadata-Version: 2.1
 Name: beambusters
-Version: 1.3.5
+Version: 1.3.6
 Summary: 
 Author: Ana Rodrigues
 Author-email: anananacr@gmail.com
 Requires-Python: >=3.10,<4.0
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: Python :: 3.12
 Requires-Dist: abstract (==2022.7.10)
 Requires-Dist: base32hex (==1.0.2)
-Requires-Dist: bblib (==2.1.3)
+Requires-Dist: bblib (==2.1.4)
 Requires-Dist: black (==24.1.1)
 Requires-Dist: build (==1.0.3)
 Requires-Dist: cachecontrol (==0.14.0)
 Requires-Dist: certifi (==2024.2.2)
 Requires-Dist: cffi (==1.16.0)
 Requires-Dist: charset-normalizer (==3.3.2)
 Requires-Dist: cleo (==2.1.0)
```

