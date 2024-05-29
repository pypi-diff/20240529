# Comparing `tmp/plyball-2.3.1.tar.gz` & `tmp/plyball-2.3.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "plyball-2.3.1.tar", max compression
+gzip compressed data, was "plyball-2.3.2.tar", max compression
```

## Comparing `plyball-2.3.1.tar` & `plyball-2.3.2.tar`

### file list

```diff
@@ -1,23 +1,23 @@
--rw-r--r--   0        0        0     1076 2024-05-29 12:33:34.480532 plyball-2.3.1/LICENSE.txt
--rw-r--r--   0        0        0      819 2024-05-29 12:33:34.480532 plyball-2.3.1/README.md
--rw-r--r--   0        0        0       22 2024-05-29 12:33:34.480532 plyball-2.3.1/plyball/__init__.py
--rw-r--r--   0        0        0       48 2024-05-29 12:33:34.480532 plyball-2.3.1/plyball/baseballreference/__init__.py
--rw-r--r--   0        0        0     9626 2024-05-29 12:33:34.480532 plyball-2.3.1/plyball/baseballreference/baseballreference.py
--rw-r--r--   0        0        0       33 2024-05-29 12:33:34.480532 plyball-2.3.1/plyball/fangraphs/__init__.py
--rw-r--r--   0        0        0    15578 2024-05-29 12:33:34.480532 plyball-2.3.1/plyball/fangraphs/fangraphs.py
--rw-r--r--   0        0        0       26 2024-05-29 12:33:34.480532 plyball-2.3.1/plyball/lahman/__init__.py
--rw-r--r--   0        0        0    10203 2024-05-29 12:33:34.480532 plyball-2.3.1/plyball/lahman/lahman.py
--rw-r--r--   0        0        0     6098 2024-05-29 12:33:34.480532 plyball-2.3.1/plyball/mlb/__init__.py
--rw-r--r--   0        0        0       28 2024-05-29 12:33:34.480532 plyball-2.3.1/plyball/ottoneu/__init__.py
--rw-r--r--   0        0        0    13950 2024-05-29 12:33:34.480532 plyball-2.3.1/plyball/ottoneu/ottoneu.py
--rw-r--r--   0        0        0        0 2024-05-29 12:33:34.480532 plyball-2.3.1/plyball/pipeline/__init__.py
--rw-r--r--   0        0        0     3019 2024-05-29 12:33:34.480532 plyball-2.3.1/plyball/pipeline/evaluation.py
--rw-r--r--   0        0        0     3517 2024-05-29 12:33:34.480532 plyball-2.3.1/plyball/player_id_lookup.py
--rw-r--r--   0        0        0      268 2024-05-29 12:33:34.480532 plyball-2.3.1/plyball/player_map.py
--rw-r--r--   0        0        0       35 2024-05-29 12:33:34.480532 plyball-2.3.1/plyball/retrosheet/__init__.py
--rw-r--r--   0        0        0     8085 2024-05-29 12:33:34.484532 plyball-2.3.1/plyball/retrosheet/retrosheet.py
--rw-r--r--   0        0        0       30 2024-05-29 12:33:34.484532 plyball-2.3.1/plyball/statcast/__init__.py
--rw-r--r--   0        0        0    14792 2024-05-29 12:33:34.484532 plyball-2.3.1/plyball/statcast/statcast.py
--rw-r--r--   0        0        0     4433 2024-05-29 12:33:34.484532 plyball-2.3.1/plyball/utils.py
--rw-r--r--   0        0        0     2974 2024-05-29 12:33:46.940553 plyball-2.3.1/pyproject.toml
--rw-r--r--   0        0        0     2596 1970-01-01 00:00:00.000000 plyball-2.3.1/PKG-INFO
+-rw-r--r--   0        0        0     1076 2024-05-29 12:48:11.336451 plyball-2.3.2/LICENSE.txt
+-rw-r--r--   0        0        0      819 2024-05-29 12:48:11.336451 plyball-2.3.2/README.md
+-rw-r--r--   0        0        0       22 2024-05-29 12:48:11.336451 plyball-2.3.2/plyball/__init__.py
+-rw-r--r--   0        0        0       48 2024-05-29 12:48:11.336451 plyball-2.3.2/plyball/baseballreference/__init__.py
+-rw-r--r--   0        0        0     9626 2024-05-29 12:48:11.336451 plyball-2.3.2/plyball/baseballreference/baseballreference.py
+-rw-r--r--   0        0        0       33 2024-05-29 12:48:11.336451 plyball-2.3.2/plyball/fangraphs/__init__.py
+-rw-r--r--   0        0        0    15578 2024-05-29 12:48:11.336451 plyball-2.3.2/plyball/fangraphs/fangraphs.py
+-rw-r--r--   0        0        0       26 2024-05-29 12:48:11.336451 plyball-2.3.2/plyball/lahman/__init__.py
+-rw-r--r--   0        0        0    10203 2024-05-29 12:48:11.336451 plyball-2.3.2/plyball/lahman/lahman.py
+-rw-r--r--   0        0        0     6098 2024-05-29 12:48:11.336451 plyball-2.3.2/plyball/mlb/__init__.py
+-rw-r--r--   0        0        0       28 2024-05-29 12:48:11.336451 plyball-2.3.2/plyball/ottoneu/__init__.py
+-rw-r--r--   0        0        0    13950 2024-05-29 12:48:11.336451 plyball-2.3.2/plyball/ottoneu/ottoneu.py
+-rw-r--r--   0        0        0        0 2024-05-29 12:48:11.336451 plyball-2.3.2/plyball/pipeline/__init__.py
+-rw-r--r--   0        0        0     3019 2024-05-29 12:48:11.336451 plyball-2.3.2/plyball/pipeline/evaluation.py
+-rw-r--r--   0        0        0     3517 2024-05-29 12:48:11.336451 plyball-2.3.2/plyball/player_id_lookup.py
+-rw-r--r--   0        0        0      268 2024-05-29 12:48:11.336451 plyball-2.3.2/plyball/player_map.py
+-rw-r--r--   0        0        0       35 2024-05-29 12:48:11.336451 plyball-2.3.2/plyball/retrosheet/__init__.py
+-rw-r--r--   0        0        0     8085 2024-05-29 12:48:11.336451 plyball-2.3.2/plyball/retrosheet/retrosheet.py
+-rw-r--r--   0        0        0       30 2024-05-29 12:48:11.336451 plyball-2.3.2/plyball/statcast/__init__.py
+-rw-r--r--   0        0        0    14792 2024-05-29 12:48:11.336451 plyball-2.3.2/plyball/statcast/statcast.py
+-rw-r--r--   0        0        0     4433 2024-05-29 12:48:11.336451 plyball-2.3.2/plyball/utils.py
+-rw-r--r--   0        0        0     2975 2024-05-29 12:48:22.284375 plyball-2.3.2/pyproject.toml
+-rw-r--r--   0        0        0     2604 1970-01-01 00:00:00.000000 plyball-2.3.2/PKG-INFO
```

### Comparing `plyball-2.3.1/LICENSE.txt` & `plyball-2.3.2/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `plyball-2.3.1/README.md` & `plyball-2.3.2/README.md`

 * *Files identical despite different names*

### Comparing `plyball-2.3.1/plyball/baseballreference/baseballreference.py` & `plyball-2.3.2/plyball/baseballreference/baseballreference.py`

 * *Files identical despite different names*

### Comparing `plyball-2.3.1/plyball/fangraphs/fangraphs.py` & `plyball-2.3.2/plyball/fangraphs/fangraphs.py`

 * *Files identical despite different names*

### Comparing `plyball-2.3.1/plyball/lahman/lahman.py` & `plyball-2.3.2/plyball/lahman/lahman.py`

 * *Files identical despite different names*

### Comparing `plyball-2.3.1/plyball/mlb/__init__.py` & `plyball-2.3.2/plyball/mlb/__init__.py`

 * *Files identical despite different names*

### Comparing `plyball-2.3.1/plyball/ottoneu/ottoneu.py` & `plyball-2.3.2/plyball/ottoneu/ottoneu.py`

 * *Files identical despite different names*

### Comparing `plyball-2.3.1/plyball/pipeline/evaluation.py` & `plyball-2.3.2/plyball/pipeline/evaluation.py`

 * *Files identical despite different names*

### Comparing `plyball-2.3.1/plyball/player_id_lookup.py` & `plyball-2.3.2/plyball/player_id_lookup.py`

 * *Files identical despite different names*

### Comparing `plyball-2.3.1/plyball/retrosheet/retrosheet.py` & `plyball-2.3.2/plyball/retrosheet/retrosheet.py`

 * *Files identical despite different names*

### Comparing `plyball-2.3.1/plyball/statcast/statcast.py` & `plyball-2.3.2/plyball/statcast/statcast.py`

 * *Files identical despite different names*

### Comparing `plyball-2.3.1/plyball/utils.py` & `plyball-2.3.2/plyball/utils.py`

 * *Files identical despite different names*

### Comparing `plyball-2.3.1/pyproject.toml` & `plyball-2.3.2/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "plyball"
-version = "2.3.1"
+version = "2.3.2"
 description = ""
 authors = ["W. Aaron Morris <waaronmorris@gmail.com>"]
 readme = "README.md"
 
 [tool.poetry.dependencies]
 python = "^3.11"
 alabaster = "0.7.13"
@@ -36,15 +36,15 @@
 sphinx = ">=6.1.3"
 sphinxcontrib-applehelp = ">=1.0.4"
 sphinxcontrib-devhelp = ">=1.0.2"
 sphinxcontrib-htmlhelp = ">=2.0.1"
 sphinxcontrib-jsmath = ">=1.0.1"
 sphinxcontrib-qthelp = ">=1.0.2"
 sphinxcontrib-serializinghtml = ">=1.1.3"
-structlog = "23.2.0"
+structlog = "^24.1.0"
 tqdm = "4.42.1"
 twine = "3.1.1"
 urllib3 = "1.26.5"
 webencodings = "0.5.1"
 flake8 = "^7.0.0"
 
 [tool.poetry.dev-dependencies]
```

### Comparing `plyball-2.3.1/PKG-INFO` & `plyball-2.3.2/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: plyball
-Version: 2.3.1
+Version: 2.3.2
 Summary: 
 Author: W. Aaron Morris
 Author-email: waaronmorris@gmail.com
 Requires-Python: >=3.11,<4.0
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: Python :: 3.12
@@ -38,15 +38,15 @@
 Requires-Dist: sphinx (>=6.1.3)
 Requires-Dist: sphinxcontrib-applehelp (>=1.0.4)
 Requires-Dist: sphinxcontrib-devhelp (>=1.0.2)
 Requires-Dist: sphinxcontrib-htmlhelp (>=2.0.1)
 Requires-Dist: sphinxcontrib-jsmath (>=1.0.1)
 Requires-Dist: sphinxcontrib-qthelp (>=1.0.2)
 Requires-Dist: sphinxcontrib-serializinghtml (>=1.1.3)
-Requires-Dist: structlog (==23.2.0)
+Requires-Dist: structlog (>=24.1.0,<25.0.0)
 Requires-Dist: tqdm (==4.42.1)
 Requires-Dist: twine (==3.1.1)
 Requires-Dist: urllib3 (==1.26.5)
 Requires-Dist: webencodings (==0.5.1)
 Description-Content-Type: text/markdown
 
 # Overview
```

