# Comparing `tmp/vns_explorer-1.0.2.tar.gz` & `tmp/vns_explorer-1.0.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "vns_explorer-1.0.2.tar", last modified: Wed May 29 07:00:40 2024, max compression
+gzip compressed data, was "vns_explorer-1.0.3.tar", last modified: Wed May 29 07:32:17 2024, max compression
```

## Comparing `vns_explorer-1.0.2.tar` & `vns_explorer-1.0.3.tar`

### file list

```diff
@@ -1,16 +1,16 @@
-drwxrwxrwx   0        0        0        0 2024-05-29 07:00:40.425590 vns_explorer-1.0.2/
--rw-rw-rw-   0        0        0      601 2024-05-29 07:00:40.424591 vns_explorer-1.0.2/PKG-INFO
--rw-rw-rw-   0        0        0       23 2024-05-29 04:11:37.000000 vns_explorer-1.0.2/README.md
--rw-rw-rw-   0        0        0      796 2024-05-29 06:58:20.000000 vns_explorer-1.0.2/pyproject.toml
--rw-rw-rw-   0        0        0      468 2024-05-29 07:00:40.431594 vns_explorer-1.0.2/setup.cfg
-drwxrwxrwx   0        0        0        0 2024-05-29 07:00:40.361199 vns_explorer-1.0.2/vns_explorer/
--rw-rw-rw-   0        0        0       64 2024-05-29 06:10:09.000000 vns_explorer-1.0.2/vns_explorer/__init__.py
--rw-rw-rw-   0        0        0     1446 2024-05-29 04:00:43.000000 vns_explorer-1.0.2/vns_explorer/agent.py
--rw-rw-rw-   0        0        0    10481 2024-05-29 06:58:14.000000 vns_explorer-1.0.2/vns_explorer/browser.py
--rw-rw-rw-   0        0        0     2293 2024-05-29 06:09:48.000000 vns_explorer-1.0.2/vns_explorer/env.py
-drwxrwxrwx   0        0        0        0 2024-05-29 07:00:40.420591 vns_explorer-1.0.2/vns_explorer.egg-info/
--rw-rw-rw-   0        0        0      601 2024-05-29 07:00:40.000000 vns_explorer-1.0.2/vns_explorer.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      304 2024-05-29 07:00:40.000000 vns_explorer-1.0.2/vns_explorer.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-05-29 07:00:40.000000 vns_explorer-1.0.2/vns_explorer.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       68 2024-05-29 07:00:40.000000 vns_explorer-1.0.2/vns_explorer.egg-info/requires.txt
--rw-rw-rw-   0        0        0       13 2024-05-29 07:00:40.000000 vns_explorer-1.0.2/vns_explorer.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2024-05-29 07:32:17.715870 vns_explorer-1.0.3/
+-rw-rw-rw-   0        0        0      601 2024-05-29 07:32:17.715870 vns_explorer-1.0.3/PKG-INFO
+-rw-rw-rw-   0        0        0       23 2024-05-29 04:11:37.000000 vns_explorer-1.0.3/README.md
+-rw-rw-rw-   0        0        0      796 2024-05-29 07:31:15.000000 vns_explorer-1.0.3/pyproject.toml
+-rw-rw-rw-   0        0        0      468 2024-05-29 07:32:17.722368 vns_explorer-1.0.3/setup.cfg
+drwxrwxrwx   0        0        0        0 2024-05-29 07:32:17.679380 vns_explorer-1.0.3/vns_explorer/
+-rw-rw-rw-   0        0        0       64 2024-05-29 06:10:09.000000 vns_explorer-1.0.3/vns_explorer/__init__.py
+-rw-rw-rw-   0        0        0     1446 2024-05-29 04:00:43.000000 vns_explorer-1.0.3/vns_explorer/agent.py
+-rw-rw-rw-   0        0        0    10483 2024-05-29 07:31:02.000000 vns_explorer-1.0.3/vns_explorer/browser.py
+-rw-rw-rw-   0        0        0     2293 2024-05-29 06:09:48.000000 vns_explorer-1.0.3/vns_explorer/env.py
+drwxrwxrwx   0        0        0        0 2024-05-29 07:32:17.713855 vns_explorer-1.0.3/vns_explorer.egg-info/
+-rw-rw-rw-   0        0        0      601 2024-05-29 07:32:17.000000 vns_explorer-1.0.3/vns_explorer.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      304 2024-05-29 07:32:17.000000 vns_explorer-1.0.3/vns_explorer.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-05-29 07:32:17.000000 vns_explorer-1.0.3/vns_explorer.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       68 2024-05-29 07:32:17.000000 vns_explorer-1.0.3/vns_explorer.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       13 2024-05-29 07:32:17.000000 vns_explorer-1.0.3/vns_explorer.egg-info/top_level.txt
```

### Comparing `vns_explorer-1.0.2/PKG-INFO` & `vns_explorer-1.0.3/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: vns_explorer
-Version: 1.0.2
+Version: 1.0.3
 Summary: Discover the Unseen
 Author: Thinh Vu
 Author-email: Thinh Vu <mrthinh@live.com>
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.10
```

### Comparing `vns_explorer-1.0.2/pyproject.toml` & `vns_explorer-1.0.3/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -5,15 +5,15 @@
     "wheel"
 ]
 build-backend = "setuptools.build_meta"
 
 # Metadata Information
 [project]
 name = "vns_explorer"
-version = "1.0.2"
+version = "1.0.3"
 description = "Discover the Unseen"
 authors = [
     { name = "Thinh Vu", email = "mrthinh@live.com" },
     ]
 license = { file = "LICENSE.md" }
 requires-python = ">=3.10"
 readme = { file = "README.md", content-type = "text/markdown" }
```

### Comparing `vns_explorer-1.0.2/vns_explorer/agent.py` & `vns_explorer-1.0.3/vns_explorer/agent.py`

 * *Files identical despite different names*

### Comparing `vns_explorer-1.0.2/vns_explorer/browser.py` & `vns_explorer-1.0.3/vns_explorer/browser.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 import time
 import random
-import pyautogui
+# import pyautogui
 import os
 from importlib.util import find_spec
 
 # Detect if running on Google Colab
 is_colab = "COLAB_GPU" in os.environ
 
 # Import the setup function from setup_selenium if in Colab
```

### Comparing `vns_explorer-1.0.2/vns_explorer/env.py` & `vns_explorer-1.0.3/vns_explorer/env.py`

 * *Files identical despite different names*

### Comparing `vns_explorer-1.0.2/vns_explorer.egg-info/PKG-INFO` & `vns_explorer-1.0.3/vns_explorer.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: vns_explorer
-Version: 1.0.2
+Version: 1.0.3
 Summary: Discover the Unseen
 Author: Thinh Vu
 Author-email: Thinh Vu <mrthinh@live.com>
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.10
```

