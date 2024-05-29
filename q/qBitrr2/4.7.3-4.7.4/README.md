# Comparing `tmp/qbitrr2-4.7.3.tar.gz` & `tmp/qbitrr2-4.7.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "qbitrr2-4.7.3.tar", last modified: Wed May 29 19:09:07 2024, max compression
+gzip compressed data, was "qbitrr2-4.7.4.tar", last modified: Wed May 29 19:19:50 2024, max compression
```

## Comparing `qbitrr2-4.7.3.tar` & `qbitrr2-4.7.4.tar`

### file list

```diff
@@ -1,28 +1,28 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-29 19:09:07.281145 qbitrr2-4.7.3/
--rw-r--r--   0 runner    (1001) docker     (127)     1066 2024-05-29 19:09:03.000000 qbitrr2-4.7.3/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)    11156 2024-05-29 19:09:07.281145 qbitrr2-4.7.3/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     8320 2024-05-29 19:09:03.000000 qbitrr2-4.7.3/README.md
--rw-r--r--   0 runner    (1001) docker     (127)      805 2024-05-29 19:09:03.000000 qbitrr2-4.7.3/pyproject.toml
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-29 19:09:07.277145 qbitrr2-4.7.3/qBitrr/
--rw-r--r--   0 runner    (1001) docker     (127)      405 2024-05-29 19:09:03.000000 qbitrr2-4.7.3/qBitrr/__init__.py
--rwxr-xr-x   0 runner    (1001) docker     (127)   232099 2024-05-29 19:09:03.000000 qbitrr2-4.7.3/qBitrr/arss.py
--rw-r--r--   0 runner    (1001) docker     (127)      190 2024-05-29 19:09:03.000000 qbitrr2-4.7.3/qBitrr/bundled_data.py
--rw-r--r--   0 runner    (1001) docker     (127)     5293 2024-05-29 19:09:03.000000 qbitrr2-4.7.3/qBitrr/config.py
--rw-r--r--   0 runner    (1001) docker     (127)     2150 2024-05-29 19:09:03.000000 qbitrr2-4.7.3/qBitrr/env_config.py
--rw-r--r--   0 runner    (1001) docker     (127)     1147 2024-05-29 19:09:03.000000 qbitrr2-4.7.3/qBitrr/errors.py
--rw-r--r--   0 runner    (1001) docker     (127)     4019 2024-05-29 19:09:03.000000 qbitrr2-4.7.3/qBitrr/ffprobe.py
--rwxr-xr-x   0 runner    (1001) docker     (127)    27032 2024-05-29 19:09:03.000000 qbitrr2-4.7.3/qBitrr/gen_config.py
--rw-r--r--   0 runner    (1001) docker     (127)      626 2024-05-29 19:09:03.000000 qbitrr2-4.7.3/qBitrr/home_path.py
--rw-r--r--   0 runner    (1001) docker     (127)     4501 2024-05-29 19:09:03.000000 qbitrr2-4.7.3/qBitrr/logger.py
--rw-r--r--   0 runner    (1001) docker     (127)     8483 2024-05-29 19:09:03.000000 qbitrr2-4.7.3/qBitrr/main.py
--rw-r--r--   0 runner    (1001) docker     (127)     2187 2024-05-29 19:09:03.000000 qbitrr2-4.7.3/qBitrr/tables.py
--rw-r--r--   0 runner    (1001) docker     (127)     5870 2024-05-29 19:09:03.000000 qbitrr2-4.7.3/qBitrr/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-29 19:09:07.277145 qbitrr2-4.7.3/qBitrr2.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)    11156 2024-05-29 19:09:07.000000 qbitrr2-4.7.3/qBitrr2.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      475 2024-05-29 19:09:07.000000 qbitrr2-4.7.3/qBitrr2.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-29 19:09:07.000000 qbitrr2-4.7.3/qBitrr2.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       43 2024-05-29 19:09:07.000000 qbitrr2-4.7.3/qBitrr2.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (127)      614 2024-05-29 19:09:07.000000 qbitrr2-4.7.3/qBitrr2.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)        7 2024-05-29 19:09:07.000000 qbitrr2-4.7.3/qBitrr2.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)     1942 2024-05-29 19:09:07.281145 qbitrr2-4.7.3/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-29 19:09:03.000000 qbitrr2-4.7.3/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-29 19:19:50.145100 qbitrr2-4.7.4/
+-rw-r--r--   0 runner    (1001) docker     (127)     1066 2024-05-29 19:19:45.000000 qbitrr2-4.7.4/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)    11156 2024-05-29 19:19:50.145100 qbitrr2-4.7.4/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     8320 2024-05-29 19:19:45.000000 qbitrr2-4.7.4/README.md
+-rw-r--r--   0 runner    (1001) docker     (127)      805 2024-05-29 19:19:45.000000 qbitrr2-4.7.4/pyproject.toml
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-29 19:19:50.141100 qbitrr2-4.7.4/qBitrr/
+-rw-r--r--   0 runner    (1001) docker     (127)      405 2024-05-29 19:19:45.000000 qbitrr2-4.7.4/qBitrr/__init__.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)   232099 2024-05-29 19:19:45.000000 qbitrr2-4.7.4/qBitrr/arss.py
+-rw-r--r--   0 runner    (1001) docker     (127)      190 2024-05-29 19:19:45.000000 qbitrr2-4.7.4/qBitrr/bundled_data.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5293 2024-05-29 19:19:45.000000 qbitrr2-4.7.4/qBitrr/config.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2150 2024-05-29 19:19:45.000000 qbitrr2-4.7.4/qBitrr/env_config.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1147 2024-05-29 19:19:45.000000 qbitrr2-4.7.4/qBitrr/errors.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4019 2024-05-29 19:19:45.000000 qbitrr2-4.7.4/qBitrr/ffprobe.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)    27032 2024-05-29 19:19:45.000000 qbitrr2-4.7.4/qBitrr/gen_config.py
+-rw-r--r--   0 runner    (1001) docker     (127)      626 2024-05-29 19:19:45.000000 qbitrr2-4.7.4/qBitrr/home_path.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4501 2024-05-29 19:19:45.000000 qbitrr2-4.7.4/qBitrr/logger.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8483 2024-05-29 19:19:45.000000 qbitrr2-4.7.4/qBitrr/main.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2187 2024-05-29 19:19:45.000000 qbitrr2-4.7.4/qBitrr/tables.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5870 2024-05-29 19:19:45.000000 qbitrr2-4.7.4/qBitrr/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-29 19:19:50.145100 qbitrr2-4.7.4/qBitrr2.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)    11156 2024-05-29 19:19:50.000000 qbitrr2-4.7.4/qBitrr2.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      475 2024-05-29 19:19:50.000000 qbitrr2-4.7.4/qBitrr2.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-29 19:19:50.000000 qbitrr2-4.7.4/qBitrr2.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       43 2024-05-29 19:19:50.000000 qbitrr2-4.7.4/qBitrr2.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      614 2024-05-29 19:19:50.000000 qbitrr2-4.7.4/qBitrr2.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        7 2024-05-29 19:19:50.000000 qbitrr2-4.7.4/qBitrr2.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)     1942 2024-05-29 19:19:50.149100 qbitrr2-4.7.4/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-29 19:19:45.000000 qbitrr2-4.7.4/setup.py
```

### Comparing `qbitrr2-4.7.3/LICENSE` & `qbitrr2-4.7.4/LICENSE`

 * *Files identical despite different names*

### Comparing `qbitrr2-4.7.3/PKG-INFO` & `qbitrr2-4.7.4/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: qBitrr2
-Version: 4.7.3
+Version: 4.7.4
 Summary: "A simple Python script to talk to qBittorrent and Arr's"
 Home-page: https://github.com/Feramance/qBitrr
 Author: Feramance
 Author-email: fera@fera.wtf
 License: MIT
 Project-URL: Issue Tracker, https://github.com/Feramance/qBitrr/issues
 Project-URL: Source Code, https://github.com/Feramance/qBitrr
```

### Comparing `qbitrr2-4.7.3/README.md` & `qbitrr2-4.7.4/README.md`

 * *Files identical despite different names*

### Comparing `qbitrr2-4.7.3/pyproject.toml` & `qbitrr2-4.7.4/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -23,15 +23,15 @@
 
 [tool.black]
 line-length = 99
 target-version = ['py38']
 
 [tool.poetry]
 name = "pypi-public"
-version = "4.7.3"
+version = "4.7.4"
 description = "A simple script to monitor qBit and communicate with Radarr and Sonarr"
 authors = ["Drapersniper", "Feramance"]
 readme = "README.md"
 repository = "https://github.com/Feramance/qBitrr"
 url = "https://pypi.org/simple/"
 
 [tool.autopep8]
```

### Comparing `qbitrr2-4.7.3/qBitrr/arss.py` & `qbitrr2-4.7.4/qBitrr/arss.py`

 * *Files identical despite different names*

### Comparing `qbitrr2-4.7.3/qBitrr/config.py` & `qbitrr2-4.7.4/qBitrr/config.py`

 * *Files identical despite different names*

### Comparing `qbitrr2-4.7.3/qBitrr/env_config.py` & `qbitrr2-4.7.4/qBitrr/env_config.py`

 * *Files identical despite different names*

### Comparing `qbitrr2-4.7.3/qBitrr/errors.py` & `qbitrr2-4.7.4/qBitrr/errors.py`

 * *Files identical despite different names*

### Comparing `qbitrr2-4.7.3/qBitrr/ffprobe.py` & `qbitrr2-4.7.4/qBitrr/ffprobe.py`

 * *Files identical despite different names*

### Comparing `qbitrr2-4.7.3/qBitrr/gen_config.py` & `qbitrr2-4.7.4/qBitrr/gen_config.py`

 * *Files identical despite different names*

### Comparing `qbitrr2-4.7.3/qBitrr/home_path.py` & `qbitrr2-4.7.4/qBitrr/home_path.py`

 * *Files identical despite different names*

### Comparing `qbitrr2-4.7.3/qBitrr/logger.py` & `qbitrr2-4.7.4/qBitrr/logger.py`

 * *Files identical despite different names*

### Comparing `qbitrr2-4.7.3/qBitrr/main.py` & `qbitrr2-4.7.4/qBitrr/main.py`

 * *Files identical despite different names*

### Comparing `qbitrr2-4.7.3/qBitrr/tables.py` & `qbitrr2-4.7.4/qBitrr/tables.py`

 * *Files identical despite different names*

### Comparing `qbitrr2-4.7.3/qBitrr/utils.py` & `qbitrr2-4.7.4/qBitrr/utils.py`

 * *Files identical despite different names*

### Comparing `qbitrr2-4.7.3/qBitrr2.egg-info/PKG-INFO` & `qbitrr2-4.7.4/qBitrr2.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: qBitrr2
-Version: 4.7.3
+Version: 4.7.4
 Summary: "A simple Python script to talk to qBittorrent and Arr's"
 Home-page: https://github.com/Feramance/qBitrr
 Author: Feramance
 Author-email: fera@fera.wtf
 License: MIT
 Project-URL: Issue Tracker, https://github.com/Feramance/qBitrr/issues
 Project-URL: Source Code, https://github.com/Feramance/qBitrr
```

### Comparing `qbitrr2-4.7.3/qBitrr2.egg-info/requires.txt` & `qbitrr2-4.7.4/qBitrr2.egg-info/requires.txt`

 * *Files identical despite different names*

### Comparing `qbitrr2-4.7.3/setup.cfg` & `qbitrr2-4.7.4/setup.cfg`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [metadata]
 name = qBitrr2
-version = 4.7.3
+version = 4.7.4
 description = "A simple Python script to talk to qBittorrent and Arr's"
 long_description = file: README.md
 long_description_content_type = text/markdown
 url = https://github.com/Feramance/qBitrr
 author = Feramance
 author_email = fera@fera.wtf
 license = MIT
```

