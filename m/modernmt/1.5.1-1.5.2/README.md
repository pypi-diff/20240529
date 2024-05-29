# Comparing `tmp/modernmt-1.5.1.tar.gz` & `tmp/modernmt-1.5.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "modernmt-1.5.1.tar", last modified: Fri Feb  9 09:14:47 2024, max compression
+gzip compressed data, was "modernmt-1.5.2.tar", last modified: Wed May 29 15:34:02 2024, max compression
```

## Comparing `modernmt-1.5.1.tar` & `modernmt-1.5.2.tar`

### file list

```diff
@@ -1,16 +1,16 @@
-drwxrwxr-x   0 davide    (1000) davide    (1000)        0 2024-02-09 09:14:47.123115 modernmt-1.5.1/
--rw-rw-r--   0 davide    (1000) davide    (1000)     1065 2021-05-05 13:02:28.000000 modernmt-1.5.1/LICENSE
--rw-r--r--   0 davide    (1000) davide    (1000)      735 2024-02-09 09:14:47.123115 modernmt-1.5.1/PKG-INFO
--rw-rw-r--   0 davide    (1000) davide    (1000)      197 2021-05-05 13:02:28.000000 modernmt-1.5.1/README.md
--rw-rw-r--   0 davide    (1000) davide    (1000)      105 2021-05-05 13:02:28.000000 modernmt-1.5.1/pyproject.toml
--rw-rw-r--   0 davide    (1000) davide    (1000)      655 2024-02-09 09:14:47.123115 modernmt-1.5.1/setup.cfg
-drwxrwxr-x   0 davide    (1000) davide    (1000)        0 2024-02-09 09:14:47.123115 modernmt-1.5.1/src/
-drwxrwxr-x   0 davide    (1000) davide    (1000)        0 2024-02-09 09:14:47.123115 modernmt-1.5.1/src/modernmt/
--rw-rw-r--   0 davide    (1000) davide    (1000)      166 2021-05-05 13:02:28.000000 modernmt-1.5.1/src/modernmt/__init__.py
--rw-rw-r--   0 davide    (1000) davide    (1000)    14510 2024-02-09 09:14:31.000000 modernmt-1.5.1/src/modernmt/modernmt.py
-drwxrwxr-x   0 davide    (1000) davide    (1000)        0 2024-02-09 09:14:47.123115 modernmt-1.5.1/src/modernmt.egg-info/
--rw-r--r--   0 davide    (1000) davide    (1000)      735 2024-02-09 09:14:47.000000 modernmt-1.5.1/src/modernmt.egg-info/PKG-INFO
--rw-rw-r--   0 davide    (1000) davide    (1000)      271 2024-02-09 09:14:47.000000 modernmt-1.5.1/src/modernmt.egg-info/SOURCES.txt
--rw-rw-r--   0 davide    (1000) davide    (1000)        1 2024-02-09 09:14:47.000000 modernmt-1.5.1/src/modernmt.egg-info/dependency_links.txt
--rw-rw-r--   0 davide    (1000) davide    (1000)       15 2024-02-09 09:14:47.000000 modernmt-1.5.1/src/modernmt.egg-info/requires.txt
--rw-rw-r--   0 davide    (1000) davide    (1000)        9 2024-02-09 09:14:47.000000 modernmt-1.5.1/src/modernmt.egg-info/top_level.txt
+drwxrwxr-x   0 davide    (1000) davide    (1000)        0 2024-05-29 15:34:02.130850 modernmt-1.5.2/
+-rw-rw-r--   0 davide    (1000) davide    (1000)     1065 2021-05-05 13:02:28.000000 modernmt-1.5.2/LICENSE
+-rw-r--r--   0 davide    (1000) davide    (1000)      735 2024-05-29 15:34:02.130850 modernmt-1.5.2/PKG-INFO
+-rw-rw-r--   0 davide    (1000) davide    (1000)      197 2021-05-05 13:02:28.000000 modernmt-1.5.2/README.md
+-rw-rw-r--   0 davide    (1000) davide    (1000)      105 2021-05-05 13:02:28.000000 modernmt-1.5.2/pyproject.toml
+-rw-rw-r--   0 davide    (1000) davide    (1000)      655 2024-05-29 15:34:02.130850 modernmt-1.5.2/setup.cfg
+drwxrwxr-x   0 davide    (1000) davide    (1000)        0 2024-05-29 15:34:02.126850 modernmt-1.5.2/src/
+drwxrwxr-x   0 davide    (1000) davide    (1000)        0 2024-05-29 15:34:02.126850 modernmt-1.5.2/src/modernmt/
+-rw-rw-r--   0 davide    (1000) davide    (1000)      166 2021-05-05 13:02:28.000000 modernmt-1.5.2/src/modernmt/__init__.py
+-rw-rw-r--   0 davide    (1000) davide    (1000)    14520 2024-05-29 15:33:22.000000 modernmt-1.5.2/src/modernmt/modernmt.py
+drwxrwxr-x   0 davide    (1000) davide    (1000)        0 2024-05-29 15:34:02.130850 modernmt-1.5.2/src/modernmt.egg-info/
+-rw-r--r--   0 davide    (1000) davide    (1000)      735 2024-05-29 15:34:02.000000 modernmt-1.5.2/src/modernmt.egg-info/PKG-INFO
+-rw-rw-r--   0 davide    (1000) davide    (1000)      271 2024-05-29 15:34:02.000000 modernmt-1.5.2/src/modernmt.egg-info/SOURCES.txt
+-rw-rw-r--   0 davide    (1000) davide    (1000)        1 2024-05-29 15:34:02.000000 modernmt-1.5.2/src/modernmt.egg-info/dependency_links.txt
+-rw-rw-r--   0 davide    (1000) davide    (1000)       15 2024-05-29 15:34:02.000000 modernmt-1.5.2/src/modernmt.egg-info/requires.txt
+-rw-rw-r--   0 davide    (1000) davide    (1000)        9 2024-05-29 15:34:02.000000 modernmt-1.5.2/src/modernmt.egg-info/top_level.txt
```

### Comparing `modernmt-1.5.1/LICENSE` & `modernmt-1.5.2/LICENSE`

 * *Files identical despite different names*

### Comparing `modernmt-1.5.1/PKG-INFO` & `modernmt-1.5.2/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: modernmt
-Version: 1.5.1
+Version: 1.5.2
 Summary: ModernMT API wrapper
 Home-page: https://github.com/modernmt/modernmt-python
 Author: ModernMT
 Author-email: info@modernmt.com
 Project-URL: Bug Tracker, https://github.com/modernmt/modernmt-python/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
```

### Comparing `modernmt-1.5.1/setup.cfg` & `modernmt-1.5.2/setup.cfg`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [metadata]
 name = modernmt
-version = 1.5.1
+version = 1.5.2
 author = ModernMT
 author_email = info@modernmt.com
 description = ModernMT API wrapper
 long_description = file: README.md
 long_description_content_type = text/markdown
 url = https://github.com/modernmt/modernmt-python
 project_urls =
```

### Comparing `modernmt-1.5.1/src/modernmt/modernmt.py` & `modernmt-1.5.2/src/modernmt/modernmt.py`

 * *Files 1% similar despite different names*

```diff
@@ -15,15 +15,15 @@
         self.message = message
 
         if metadata is not None:
             self.metadata = metadata
 
 
 class ModernMT(object):
-    def __init__(self, api_key, platform="modernmt-python", platform_version="1.5.1", api_client=None) -> None:
+    def __init__(self, api_key, platform="modernmt-python", platform_version="1.5.2", api_client=None) -> None:
         self.__batch_public_key = None
         self.__batch_public_key_timestamp_sec = 0
 
         self.__base_url = "https://api.modernmt.com"
         self.__headers = {
             "MMT-ApiKey": api_key,
             "MMT-Platform": platform,
@@ -229,15 +229,15 @@
                 return None
 
     def me(self):
         return self.__send("get", "/users/me", cls=User)
 
     def qe(self, source, target, sentence, translation):
         data = {"source": source, "target": target, "sentence": sentence, "translation": translation}
-        res = self.__send("get", "/qe", data=data)
+        res = self.__send("get", "/translate/qe", data=data)
 
         if not isinstance(res, list):
             return QualityEstimation(res)
 
         qes = []
         for el in res:
             qes.append(QualityEstimation(el))
```

### Comparing `modernmt-1.5.1/src/modernmt.egg-info/PKG-INFO` & `modernmt-1.5.2/src/modernmt.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: modernmt
-Version: 1.5.1
+Version: 1.5.2
 Summary: ModernMT API wrapper
 Home-page: https://github.com/modernmt/modernmt-python
 Author: ModernMT
 Author-email: info@modernmt.com
 Project-URL: Bug Tracker, https://github.com/modernmt/modernmt-python/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
```

