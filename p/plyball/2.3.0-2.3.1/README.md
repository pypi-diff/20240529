# Comparing `tmp/plyball-2.3.0.tar.gz` & `tmp/plyball-2.3.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "plyball-2.3.0.tar", max compression
+gzip compressed data, was "plyball-2.3.1.tar", max compression
```

## Comparing `plyball-2.3.0.tar` & `plyball-2.3.1.tar`

### file list

```diff
@@ -1,23 +1,23 @@
--rw-r--r--   0        0        0     1076 2024-05-29 12:23:09.413401 plyball-2.3.0/LICENSE.txt
--rw-r--r--   0        0        0      819 2024-05-29 12:23:09.413401 plyball-2.3.0/README.md
--rw-r--r--   0        0        0       22 2024-05-29 12:23:09.417401 plyball-2.3.0/plyball/__init__.py
--rw-r--r--   0        0        0       48 2024-05-29 12:23:09.417401 plyball-2.3.0/plyball/baseballreference/__init__.py
--rw-r--r--   0        0        0     9626 2024-05-29 12:23:09.417401 plyball-2.3.0/plyball/baseballreference/baseballreference.py
--rw-r--r--   0        0        0       33 2024-05-29 12:23:09.417401 plyball-2.3.0/plyball/fangraphs/__init__.py
--rw-r--r--   0        0        0    15578 2024-05-29 12:23:09.417401 plyball-2.3.0/plyball/fangraphs/fangraphs.py
--rw-r--r--   0        0        0       26 2024-05-29 12:23:09.417401 plyball-2.3.0/plyball/lahman/__init__.py
--rw-r--r--   0        0        0    10203 2024-05-29 12:23:09.417401 plyball-2.3.0/plyball/lahman/lahman.py
--rw-r--r--   0        0        0     6098 2024-05-29 12:23:09.417401 plyball-2.3.0/plyball/mlb/__init__.py
--rw-r--r--   0        0        0       28 2024-05-29 12:23:09.417401 plyball-2.3.0/plyball/ottoneu/__init__.py
--rw-r--r--   0        0        0    13950 2024-05-29 12:23:09.417401 plyball-2.3.0/plyball/ottoneu/ottoneu.py
--rw-r--r--   0        0        0        0 2024-05-29 12:23:09.417401 plyball-2.3.0/plyball/pipeline/__init__.py
--rw-r--r--   0        0        0     3019 2024-05-29 12:23:09.417401 plyball-2.3.0/plyball/pipeline/evaluation.py
--rw-r--r--   0        0        0     3517 2024-05-29 12:23:09.417401 plyball-2.3.0/plyball/player_id_lookup.py
--rw-r--r--   0        0        0      268 2024-05-29 12:23:09.417401 plyball-2.3.0/plyball/player_map.py
--rw-r--r--   0        0        0       35 2024-05-29 12:23:09.417401 plyball-2.3.0/plyball/retrosheet/__init__.py
--rw-r--r--   0        0        0     8085 2024-05-29 12:23:09.417401 plyball-2.3.0/plyball/retrosheet/retrosheet.py
--rw-r--r--   0        0        0       30 2024-05-29 12:23:09.417401 plyball-2.3.0/plyball/statcast/__init__.py
--rw-r--r--   0        0        0    14792 2024-05-29 12:23:09.417401 plyball-2.3.0/plyball/statcast/statcast.py
--rw-r--r--   0        0        0     4433 2024-05-29 12:23:09.417401 plyball-2.3.0/plyball/utils.py
--rw-r--r--   0        0        0     2974 2024-05-29 12:23:20.445293 plyball-2.3.0/pyproject.toml
--rw-r--r--   0        0        0     2630 1970-01-01 00:00:00.000000 plyball-2.3.0/PKG-INFO
+-rw-r--r--   0        0        0     1076 2024-05-29 12:33:34.480532 plyball-2.3.1/LICENSE.txt
+-rw-r--r--   0        0        0      819 2024-05-29 12:33:34.480532 plyball-2.3.1/README.md
+-rw-r--r--   0        0        0       22 2024-05-29 12:33:34.480532 plyball-2.3.1/plyball/__init__.py
+-rw-r--r--   0        0        0       48 2024-05-29 12:33:34.480532 plyball-2.3.1/plyball/baseballreference/__init__.py
+-rw-r--r--   0        0        0     9626 2024-05-29 12:33:34.480532 plyball-2.3.1/plyball/baseballreference/baseballreference.py
+-rw-r--r--   0        0        0       33 2024-05-29 12:33:34.480532 plyball-2.3.1/plyball/fangraphs/__init__.py
+-rw-r--r--   0        0        0    15578 2024-05-29 12:33:34.480532 plyball-2.3.1/plyball/fangraphs/fangraphs.py
+-rw-r--r--   0        0        0       26 2024-05-29 12:33:34.480532 plyball-2.3.1/plyball/lahman/__init__.py
+-rw-r--r--   0        0        0    10203 2024-05-29 12:33:34.480532 plyball-2.3.1/plyball/lahman/lahman.py
+-rw-r--r--   0        0        0     6098 2024-05-29 12:33:34.480532 plyball-2.3.1/plyball/mlb/__init__.py
+-rw-r--r--   0        0        0       28 2024-05-29 12:33:34.480532 plyball-2.3.1/plyball/ottoneu/__init__.py
+-rw-r--r--   0        0        0    13950 2024-05-29 12:33:34.480532 plyball-2.3.1/plyball/ottoneu/ottoneu.py
+-rw-r--r--   0        0        0        0 2024-05-29 12:33:34.480532 plyball-2.3.1/plyball/pipeline/__init__.py
+-rw-r--r--   0        0        0     3019 2024-05-29 12:33:34.480532 plyball-2.3.1/plyball/pipeline/evaluation.py
+-rw-r--r--   0        0        0     3517 2024-05-29 12:33:34.480532 plyball-2.3.1/plyball/player_id_lookup.py
+-rw-r--r--   0        0        0      268 2024-05-29 12:33:34.480532 plyball-2.3.1/plyball/player_map.py
+-rw-r--r--   0        0        0       35 2024-05-29 12:33:34.480532 plyball-2.3.1/plyball/retrosheet/__init__.py
+-rw-r--r--   0        0        0     8085 2024-05-29 12:33:34.484532 plyball-2.3.1/plyball/retrosheet/retrosheet.py
+-rw-r--r--   0        0        0       30 2024-05-29 12:33:34.484532 plyball-2.3.1/plyball/statcast/__init__.py
+-rw-r--r--   0        0        0    14792 2024-05-29 12:33:34.484532 plyball-2.3.1/plyball/statcast/statcast.py
+-rw-r--r--   0        0        0     4433 2024-05-29 12:33:34.484532 plyball-2.3.1/plyball/utils.py
+-rw-r--r--   0        0        0     2974 2024-05-29 12:33:46.940553 plyball-2.3.1/pyproject.toml
+-rw-r--r--   0        0        0     2596 1970-01-01 00:00:00.000000 plyball-2.3.1/PKG-INFO
```

### Comparing `plyball-2.3.0/LICENSE.txt` & `plyball-2.3.1/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `plyball-2.3.0/README.md` & `plyball-2.3.1/README.md`

 * *Files identical despite different names*

### Comparing `plyball-2.3.0/plyball/baseballreference/baseballreference.py` & `plyball-2.3.1/plyball/baseballreference/baseballreference.py`

 * *Files identical despite different names*

### Comparing `plyball-2.3.0/plyball/fangraphs/fangraphs.py` & `plyball-2.3.1/plyball/fangraphs/fangraphs.py`

 * *Files identical despite different names*

### Comparing `plyball-2.3.0/plyball/lahman/lahman.py` & `plyball-2.3.1/plyball/lahman/lahman.py`

 * *Files identical despite different names*

### Comparing `plyball-2.3.0/plyball/mlb/__init__.py` & `plyball-2.3.1/plyball/mlb/__init__.py`

 * *Files identical despite different names*

### Comparing `plyball-2.3.0/plyball/ottoneu/ottoneu.py` & `plyball-2.3.1/plyball/ottoneu/ottoneu.py`

 * *Files identical despite different names*

### Comparing `plyball-2.3.0/plyball/pipeline/evaluation.py` & `plyball-2.3.1/plyball/pipeline/evaluation.py`

 * *Files identical despite different names*

### Comparing `plyball-2.3.0/plyball/player_id_lookup.py` & `plyball-2.3.1/plyball/player_id_lookup.py`

 * *Files identical despite different names*

### Comparing `plyball-2.3.0/plyball/retrosheet/retrosheet.py` & `plyball-2.3.1/plyball/retrosheet/retrosheet.py`

 * *Files identical despite different names*

### Comparing `plyball-2.3.0/plyball/statcast/statcast.py` & `plyball-2.3.1/plyball/statcast/statcast.py`

 * *Files identical despite different names*

### Comparing `plyball-2.3.0/plyball/utils.py` & `plyball-2.3.1/plyball/utils.py`

 * *Files identical despite different names*

### Comparing `plyball-2.3.0/pyproject.toml` & `plyball-2.3.1/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "plyball"
-version = "2.3.0"
+version = "2.3.1"
 description = ""
 authors = ["W. Aaron Morris <waaronmorris@gmail.com>"]
 readme = "README.md"
 
 [tool.poetry.dependencies]
 python = "^3.11"
 alabaster = "0.7.13"
@@ -18,15 +18,14 @@
 idna = "3.4"
 imagesize = "1.4.1"
 jinja2 = "3.1.2"
 lxml = "4.9.2"
 keyring = "23.13.1"
 markupsafe = "2.1.2"
 numpy = "1.24.2"
-packaging = "23.1"
 pandas = "2.0.0"
 pkginfo = "1.9.6"
 pygments = "2.15.0"
 pyparsing = "3.0.9"
 python-dateutil = "2.8.2"
 readme-renderer = "37.3"
 requests = "2.31.0"
@@ -46,14 +45,15 @@
 twine = "3.1.1"
 urllib3 = "1.26.5"
 webencodings = "0.5.1"
 flake8 = "^7.0.0"
 
 [tool.poetry.dev-dependencies]
 python-semantic-release = "^9.7.3"
+packaging = "23.1"
 
 
 [tool.poetry.group.dev.dependencies]
 commitizen = "^3.26.0"
 
 [build-system]
 requires = ["poetry-core"]
```

### Comparing `plyball-2.3.0/PKG-INFO` & `plyball-2.3.1/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: plyball
-Version: 2.3.0
+Version: 2.3.1
 Summary: 
 Author: W. Aaron Morris
 Author-email: waaronmorris@gmail.com
 Requires-Python: >=3.11,<4.0
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: Python :: 3.12
@@ -20,15 +20,14 @@
 Requires-Dist: idna (==3.4)
 Requires-Dist: imagesize (==1.4.1)
 Requires-Dist: jinja2 (==3.1.2)
 Requires-Dist: keyring (==23.13.1)
 Requires-Dist: lxml (==4.9.2)
 Requires-Dist: markupsafe (==2.1.2)
 Requires-Dist: numpy (==1.24.2)
-Requires-Dist: packaging (==23.1)
 Requires-Dist: pandas (==2.0.0)
 Requires-Dist: pkginfo (==1.9.6)
 Requires-Dist: pygments (==2.15.0)
 Requires-Dist: pyparsing (==3.0.9)
 Requires-Dist: python-dateutil (==2.8.2)
 Requires-Dist: readme-renderer (==37.3)
 Requires-Dist: requests (==2.31.0)
```

