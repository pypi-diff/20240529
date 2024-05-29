# Comparing `tmp/whataspp_message_inforu_local-0.0.15.tar.gz` & `tmp/whataspp_message_inforu_local-0.0.16.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "whataspp_message_inforu_local-0.0.15.tar", last modified: Wed May 29 10:24:34 2024, max compression
+gzip compressed data, was "whataspp_message_inforu_local-0.0.16.tar", last modified: Wed May 29 11:37:20 2024, max compression
```

## Comparing `whataspp_message_inforu_local-0.0.15.tar` & `whataspp_message_inforu_local-0.0.16.tar`

### file list

```diff
@@ -1,17 +1,17 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-29 10:24:34.255179 whataspp_message_inforu_local-0.0.15/
--rw-r--r--   0 runner    (1001) docker     (127)      703 2024-05-29 10:24:34.255179 whataspp_message_inforu_local-0.0.15/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     3259 2024-05-29 10:23:51.000000 whataspp_message_inforu_local-0.0.15/README.md
--rw-r--r--   0 runner    (1001) docker     (127)      732 2024-05-29 10:23:57.000000 whataspp_message_inforu_local-0.0.15/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-29 10:24:34.255179 whataspp_message_inforu_local-0.0.15/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)     1245 2024-05-29 10:23:51.000000 whataspp_message_inforu_local-0.0.15/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-29 10:24:34.251179 whataspp_message_inforu_local-0.0.15/whataspp_message_inforu_local/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-29 10:24:34.251179 whataspp_message_inforu_local-0.0.15/whataspp_message_inforu_local/src/
--rw-r--r--   0 runner    (1001) docker     (127)     1126 2024-05-29 10:23:51.000000 whataspp_message_inforu_local-0.0.15/whataspp_message_inforu_local/src/WhatsAppLocalConstants.py
--rw-r--r--   0 runner    (1001) docker     (127)     4137 2024-05-29 10:23:51.000000 whataspp_message_inforu_local-0.0.15/whataspp_message_inforu_local/src/WhatsAppMessageInforuLocal.py
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-29 10:23:51.000000 whataspp_message_inforu_local-0.0.15/whataspp_message_inforu_local/src/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-29 10:24:34.255179 whataspp_message_inforu_local-0.0.15/whataspp_message_inforu_local.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)      703 2024-05-29 10:24:34.000000 whataspp_message_inforu_local-0.0.15/whataspp_message_inforu_local.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      467 2024-05-29 10:24:34.000000 whataspp_message_inforu_local-0.0.15/whataspp_message_inforu_local.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-29 10:24:34.000000 whataspp_message_inforu_local-0.0.15/whataspp_message_inforu_local.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       88 2024-05-29 10:24:34.000000 whataspp_message_inforu_local-0.0.15/whataspp_message_inforu_local.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       30 2024-05-29 10:24:34.000000 whataspp_message_inforu_local-0.0.15/whataspp_message_inforu_local.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-29 11:37:20.244600 whataspp_message_inforu_local-0.0.16/
+-rw-r--r--   0 runner    (1001) docker     (127)      703 2024-05-29 11:37:20.240600 whataspp_message_inforu_local-0.0.16/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     3259 2024-05-29 11:36:48.000000 whataspp_message_inforu_local-0.0.16/README.md
+-rw-r--r--   0 runner    (1001) docker     (127)      732 2024-05-29 11:36:53.000000 whataspp_message_inforu_local-0.0.16/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-29 11:37:20.244600 whataspp_message_inforu_local-0.0.16/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)     1245 2024-05-29 11:36:48.000000 whataspp_message_inforu_local-0.0.16/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-29 11:37:20.236600 whataspp_message_inforu_local-0.0.16/whataspp_message_inforu_local/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-29 11:37:20.240600 whataspp_message_inforu_local-0.0.16/whataspp_message_inforu_local/src/
+-rw-r--r--   0 runner    (1001) docker     (127)     1126 2024-05-29 11:36:48.000000 whataspp_message_inforu_local-0.0.16/whataspp_message_inforu_local/src/WhatsAppLocalConstants.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4137 2024-05-29 11:36:48.000000 whataspp_message_inforu_local-0.0.16/whataspp_message_inforu_local/src/WhatsAppMessageInforuLocal.py
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-29 11:36:48.000000 whataspp_message_inforu_local-0.0.16/whataspp_message_inforu_local/src/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-29 11:37:20.240600 whataspp_message_inforu_local-0.0.16/whataspp_message_inforu_local.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)      703 2024-05-29 11:37:20.000000 whataspp_message_inforu_local-0.0.16/whataspp_message_inforu_local.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      467 2024-05-29 11:37:20.000000 whataspp_message_inforu_local-0.0.16/whataspp_message_inforu_local.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-29 11:37:20.000000 whataspp_message_inforu_local-0.0.16/whataspp_message_inforu_local.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       88 2024-05-29 11:37:20.000000 whataspp_message_inforu_local-0.0.16/whataspp_message_inforu_local.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       30 2024-05-29 11:37:20.000000 whataspp_message_inforu_local-0.0.16/whataspp_message_inforu_local.egg-info/top_level.txt
```

### Comparing `whataspp_message_inforu_local-0.0.15/PKG-INFO` & `whataspp_message_inforu_local-0.0.16/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: whataspp-message-inforu-local
-Version: 0.0.15
+Version: 0.0.16
 Summary: PyPI Package for Circles whataspp_inforu_local Python
 Home-page: https://github.com/circles-zone/whatsapp-message-inforu-local-python-package
 Author: Circles
 Author-email: info@circlez.ai
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: Other/Proprietary License
 Classifier: Operating System :: OS Independent
```

### Comparing `whataspp_message_inforu_local-0.0.15/README.md` & `whataspp_message_inforu_local-0.0.16/README.md`

 * *Files identical despite different names*

### Comparing `whataspp_message_inforu_local-0.0.15/pyproject.toml` & `whataspp_message_inforu_local-0.0.16/pyproject.toml`

 * *Files identical despite different names*

### Comparing `whataspp_message_inforu_local-0.0.15/setup.py` & `whataspp_message_inforu_local-0.0.16/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 
 PACKAGE_NAME = "whataspp-message-inforu-local"
 # Since all PACAKGE_NAMEs are with an underscore, we don't need this. Why do we need it?
 package_dir = PACKAGE_NAME.replace("-", "_")
 
 setuptools.setup(
     name=PACKAGE_NAME,
-    version='0.0.15',  # update only the minor version each time # https://pypi.org/project/whataspp-inforu-local/
+    version='0.0.16',  # update only the minor version each time # https://pypi.org/project/whataspp-inforu-local/
     author="Circles",
     author_email="info@circlez.ai",
     description="PyPI Package for Circles whataspp_inforu_local Python",
     long_description="This is a package for sharing common whataspp_inforu_local function used in different repositories",
     long_description_content_type='text/markdown',
     url="https://github.com/circles-zone/whatsapp-message-inforu-local-python-package",
     # packages=setuptools.find_packages(),
```

### Comparing `whataspp_message_inforu_local-0.0.15/whataspp_message_inforu_local/src/WhatsAppLocalConstants.py` & `whataspp_message_inforu_local-0.0.16/whataspp_message_inforu_local/src/WhatsAppLocalConstants.py`

 * *Files identical despite different names*

### Comparing `whataspp_message_inforu_local-0.0.15/whataspp_message_inforu_local/src/WhatsAppMessageInforuLocal.py` & `whataspp_message_inforu_local-0.0.16/whataspp_message_inforu_local/src/WhatsAppMessageInforuLocal.py`

 * *Files identical despite different names*

### Comparing `whataspp_message_inforu_local-0.0.15/whataspp_message_inforu_local.egg-info/PKG-INFO` & `whataspp_message_inforu_local-0.0.16/whataspp_message_inforu_local.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: whataspp-message-inforu-local
-Version: 0.0.15
+Version: 0.0.16
 Summary: PyPI Package for Circles whataspp_inforu_local Python
 Home-page: https://github.com/circles-zone/whatsapp-message-inforu-local-python-package
 Author: Circles
 Author-email: info@circlez.ai
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: Other/Proprietary License
 Classifier: Operating System :: OS Independent
```

