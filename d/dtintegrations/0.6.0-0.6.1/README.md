# Comparing `tmp/dtintegrations-0.6.0.tar.gz` & `tmp/dtintegrations-0.6.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dtintegrations-0.6.0.tar", last modified: Fri Aug  4 13:33:02 2023, max compression
+gzip compressed data, was "dtintegrations-0.6.1.tar", last modified: Wed May 29 12:06:37 2024, max compression
```

## Comparing `dtintegrations-0.6.0.tar` & `dtintegrations-0.6.1.tar`

### file list

```diff
@@ -1,21 +1,21 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-04 13:33:02.688609 dtintegrations-0.6.0/
--rw-r--r--   0 runner    (1001) docker     (123)     1092 2023-08-04 13:32:51.000000 dtintegrations-0.6.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)     3189 2023-08-04 13:33:02.688609 dtintegrations-0.6.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     2307 2023-08-04 13:32:51.000000 dtintegrations-0.6.0/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-04 13:33:02.688609 dtintegrations-0.6.0/dtintegrations/
--rw-r--r--   0 runner    (1001) docker     (123)      147 2023-08-04 13:32:51.000000 dtintegrations-0.6.0/dtintegrations/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-04 13:33:02.688609 dtintegrations-0.6.0/dtintegrations/data_connector/
--rw-r--r--   0 runner    (1001) docker     (123)       81 2023-08-04 13:32:51.000000 dtintegrations-0.6.0/dtintegrations/data_connector/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     5808 2023-08-04 13:32:51.000000 dtintegrations-0.6.0/dtintegrations/data_connector/http_push.py
--rw-r--r--   0 runner    (1001) docker     (123)      942 2023-08-04 13:32:51.000000 dtintegrations-0.6.0/dtintegrations/data_connector/metadata.py
--rw-r--r--   0 runner    (1001) docker     (123)     3262 2023-08-04 13:32:51.000000 dtintegrations-0.6.0/dtintegrations/outputs.py
--rw-r--r--   0 runner    (1001) docker     (123)     2439 2023-08-04 13:32:51.000000 dtintegrations-0.6.0/dtintegrations/provider.py
--rw-r--r--   0 runner    (1001) docker     (123)     1218 2023-08-04 13:32:51.000000 dtintegrations-0.6.0/dtintegrations/request.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-04 13:33:02.688609 dtintegrations-0.6.0/dtintegrations.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     3189 2023-08-04 13:33:02.000000 dtintegrations-0.6.0/dtintegrations.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      458 2023-08-04 13:33:02.000000 dtintegrations-0.6.0/dtintegrations.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-08-04 13:33:02.000000 dtintegrations-0.6.0/dtintegrations.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)      136 2023-08-04 13:33:02.000000 dtintegrations-0.6.0/dtintegrations.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       15 2023-08-04 13:33:02.000000 dtintegrations-0.6.0/dtintegrations.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)     1158 2023-08-04 13:33:02.692609 dtintegrations-0.6.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)       92 2023-08-04 13:32:51.000000 dtintegrations-0.6.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-29 12:06:37.334824 dtintegrations-0.6.1/
+-rw-r--r--   0 runner    (1001) docker     (127)     1092 2024-05-29 12:06:28.000000 dtintegrations-0.6.1/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)     3189 2024-05-29 12:06:37.334824 dtintegrations-0.6.1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     2307 2024-05-29 12:06:28.000000 dtintegrations-0.6.1/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-29 12:06:37.334824 dtintegrations-0.6.1/dtintegrations/
+-rw-r--r--   0 runner    (1001) docker     (127)      147 2024-05-29 12:06:28.000000 dtintegrations-0.6.1/dtintegrations/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-29 12:06:37.334824 dtintegrations-0.6.1/dtintegrations/data_connector/
+-rw-r--r--   0 runner    (1001) docker     (127)       81 2024-05-29 12:06:28.000000 dtintegrations-0.6.1/dtintegrations/data_connector/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5803 2024-05-29 12:06:28.000000 dtintegrations-0.6.1/dtintegrations/data_connector/http_push.py
+-rw-r--r--   0 runner    (1001) docker     (127)      942 2024-05-29 12:06:28.000000 dtintegrations-0.6.1/dtintegrations/data_connector/metadata.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3262 2024-05-29 12:06:28.000000 dtintegrations-0.6.1/dtintegrations/outputs.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2439 2024-05-29 12:06:28.000000 dtintegrations-0.6.1/dtintegrations/provider.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1218 2024-05-29 12:06:28.000000 dtintegrations-0.6.1/dtintegrations/request.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-29 12:06:37.334824 dtintegrations-0.6.1/dtintegrations.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     3189 2024-05-29 12:06:37.000000 dtintegrations-0.6.1/dtintegrations.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      458 2024-05-29 12:06:37.000000 dtintegrations-0.6.1/dtintegrations.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-29 12:06:37.000000 dtintegrations-0.6.1/dtintegrations.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      136 2024-05-29 12:06:37.000000 dtintegrations-0.6.1/dtintegrations.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       15 2024-05-29 12:06:37.000000 dtintegrations-0.6.1/dtintegrations.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)     1158 2024-05-29 12:06:37.334824 dtintegrations-0.6.1/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)       92 2024-05-29 12:06:28.000000 dtintegrations-0.6.1/setup.py
```

### Comparing `dtintegrations-0.6.0/LICENSE` & `dtintegrations-0.6.1/LICENSE`

 * *Files identical despite different names*

### Comparing `dtintegrations-0.6.0/PKG-INFO` & `dtintegrations-0.6.1/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: dtintegrations
-Version: 0.6.0
+Version: 0.6.1
 Summary: Disruptive Technologies Python Integrations.
 Home-page: https://github.com/disruptive-technologies/disruptive-dataconnector
 Author: Disruptive Technologies Research AS
 Author-email: developer-support@disruptive-technologies.com
 Keywords: disruptive,technologies,dt,integration,api
 Classifier: Natural Language :: English
 Classifier: License :: OSI Approved :: MIT License
```

### Comparing `dtintegrations-0.6.0/README.md` & `dtintegrations-0.6.1/README.md`

 * *Files identical despite different names*

### Comparing `dtintegrations-0.6.0/dtintegrations/data_connector/http_push.py` & `dtintegrations-0.6.1/dtintegrations/data_connector/http_push.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 import jwt
-import ast
+import json
 import hashlib
 from typing import Any, Optional
 
 import disruptive  # type: ignore
 
 from dtintegrations import request as dtrequest, outputs
 from dtintegrations.data_connector import metadata as metadata
@@ -141,15 +141,15 @@
         checksum_sha256 = m.digest().hex()
         if payload['checksum_sha256'] != checksum_sha256:
             raise disruptive.errors.ConfigurationError(
                 'Checksum mismatch.'
             )
 
         # Convert the body bytes string into a dictionary.
-        body_dict = ast.literal_eval(body.decode('utf-8'))
+        body_dict = json.loads(body.decode('utf-8'))
 
         return dict(body_dict)
 
     @staticmethod
     def from_provider(request: Any, provider: str, secret: str) -> Any:
         """
         Decodes the incoming event using a specified provider, first validating
```

### Comparing `dtintegrations-0.6.0/dtintegrations/data_connector/metadata.py` & `dtintegrations-0.6.1/dtintegrations/data_connector/metadata.py`

 * *Files identical despite different names*

### Comparing `dtintegrations-0.6.0/dtintegrations/outputs.py` & `dtintegrations-0.6.1/dtintegrations/outputs.py`

 * *Files identical despite different names*

### Comparing `dtintegrations-0.6.0/dtintegrations/provider.py` & `dtintegrations-0.6.1/dtintegrations/provider.py`

 * *Files identical despite different names*

### Comparing `dtintegrations-0.6.0/dtintegrations/request.py` & `dtintegrations-0.6.1/dtintegrations/request.py`

 * *Files identical despite different names*

### Comparing `dtintegrations-0.6.0/dtintegrations.egg-info/PKG-INFO` & `dtintegrations-0.6.1/dtintegrations.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: dtintegrations
-Version: 0.6.0
+Version: 0.6.1
 Summary: Disruptive Technologies Python Integrations.
 Home-page: https://github.com/disruptive-technologies/disruptive-dataconnector
 Author: Disruptive Technologies Research AS
 Author-email: developer-support@disruptive-technologies.com
 Keywords: disruptive,technologies,dt,integration,api
 Classifier: Natural Language :: English
 Classifier: License :: OSI Approved :: MIT License
```

### Comparing `dtintegrations-0.6.0/setup.cfg` & `dtintegrations-0.6.1/setup.cfg`

 * *Files identical despite different names*

