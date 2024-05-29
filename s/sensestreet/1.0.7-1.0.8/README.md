# Comparing `tmp/sensestreet-1.0.7.tar.gz` & `tmp/sensestreet-1.0.8.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "sensestreet-1.0.7.tar", last modified: Fri Apr 26 12:59:17 2024, max compression
+gzip compressed data, was "sensestreet-1.0.8.tar", last modified: Wed May 29 14:07:57 2024, max compression
```

## Comparing `sensestreet-1.0.7.tar` & `sensestreet-1.0.8.tar`

### file list

```diff
@@ -1,17 +1,17 @@
-drwxrwxr-x   0 michalg   (1001) michalg   (1001)        0 2024-04-26 12:59:17.351953 sensestreet-1.0.7/
--rw-rw-r--   0 michalg   (1001) michalg   (1001)    11327 2023-06-21 13:47:45.000000 sensestreet-1.0.7/LICENSE
--rw-rw-r--   0 michalg   (1001) michalg   (1001)     4047 2024-04-26 12:59:17.351953 sensestreet-1.0.7/PKG-INFO
--rw-rw-r--   0 michalg   (1001) michalg   (1001)     3778 2024-04-24 07:26:03.000000 sensestreet-1.0.7/README.md
--rw-rw-r--   0 michalg   (1001) michalg   (1001)      103 2024-04-26 12:59:17.355953 sensestreet-1.0.7/setup.cfg
--rw-rw-r--   0 michalg   (1001) michalg   (1001)      686 2024-04-26 12:57:22.000000 sensestreet-1.0.7/setup.py
-drwxrwxr-x   0 michalg   (1001) michalg   (1001)        0 2024-04-26 12:59:17.343954 sensestreet-1.0.7/src/
-drwxrwxr-x   0 michalg   (1001) michalg   (1001)        0 2024-04-26 12:59:17.351953 sensestreet-1.0.7/src/sensestreet/
--rw-rw-r--   0 michalg   (1001) michalg   (1001)      108 2024-04-24 07:26:03.000000 sensestreet-1.0.7/src/sensestreet/__init__.py
--rw-rw-r--   0 michalg   (1001) michalg   (1001)     5628 2024-04-26 12:54:47.000000 sensestreet-1.0.7/src/sensestreet/anonymise.py
--rw-rw-r--   0 michalg   (1001) michalg   (1001)    12370 2024-04-26 12:57:22.000000 sensestreet-1.0.7/src/sensestreet/sensestreet_client.py
-drwxrwxr-x   0 michalg   (1001) michalg   (1001)        0 2024-04-26 12:59:17.351953 sensestreet-1.0.7/src/sensestreet.egg-info/
--rw-rw-r--   0 michalg   (1001) michalg   (1001)     4047 2024-04-26 12:59:17.000000 sensestreet-1.0.7/src/sensestreet.egg-info/PKG-INFO
--rw-rw-r--   0 michalg   (1001) michalg   (1001)      325 2024-04-26 12:59:17.000000 sensestreet-1.0.7/src/sensestreet.egg-info/SOURCES.txt
--rw-rw-r--   0 michalg   (1001) michalg   (1001)        1 2024-04-26 12:59:17.000000 sensestreet-1.0.7/src/sensestreet.egg-info/dependency_links.txt
--rw-rw-r--   0 michalg   (1001) michalg   (1001)       39 2024-04-26 12:59:17.000000 sensestreet-1.0.7/src/sensestreet.egg-info/requires.txt
--rw-rw-r--   0 michalg   (1001) michalg   (1001)       12 2024-04-26 12:59:17.000000 sensestreet-1.0.7/src/sensestreet.egg-info/top_level.txt
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-29 14:07:57.839990 sensestreet-1.0.8/
+-rw-rw-rw-   0 root         (0) root         (0)    11327 2024-05-29 14:07:36.000000 sensestreet-1.0.8/LICENSE
+-rw-r--r--   0 root         (0) root         (0)     4125 2024-05-29 14:07:57.839990 sensestreet-1.0.8/PKG-INFO
+-rw-rw-rw-   0 root         (0) root         (0)     3778 2024-05-29 14:07:36.000000 sensestreet-1.0.8/README.md
+-rw-rw-rw-   0 root         (0) root         (0)      103 2024-05-29 14:07:57.839990 sensestreet-1.0.8/setup.cfg
+-rw-rw-rw-   0 root         (0) root         (0)      686 2024-05-29 14:07:36.000000 sensestreet-1.0.8/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-29 14:07:57.835991 sensestreet-1.0.8/src/
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-29 14:07:57.837990 sensestreet-1.0.8/src/sensestreet/
+-rw-rw-rw-   0 root         (0) root         (0)      108 2024-05-29 14:07:36.000000 sensestreet-1.0.8/src/sensestreet/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     5628 2024-05-29 14:07:36.000000 sensestreet-1.0.8/src/sensestreet/anonymise.py
+-rw-rw-rw-   0 root         (0) root         (0)    13101 2024-05-29 14:07:36.000000 sensestreet-1.0.8/src/sensestreet/sensestreet_client.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-29 14:07:57.838990 sensestreet-1.0.8/src/sensestreet.egg-info/
+-rw-r--r--   0 root         (0) root         (0)     4125 2024-05-29 14:07:57.000000 sensestreet-1.0.8/src/sensestreet.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)      325 2024-05-29 14:07:57.000000 sensestreet-1.0.8/src/sensestreet.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2024-05-29 14:07:57.000000 sensestreet-1.0.8/src/sensestreet.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)       39 2024-05-29 14:07:57.000000 sensestreet-1.0.8/src/sensestreet.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)       12 2024-05-29 14:07:57.000000 sensestreet-1.0.8/src/sensestreet.egg-info/top_level.txt
```

### Comparing `sensestreet-1.0.7/LICENSE` & `sensestreet-1.0.8/LICENSE`

 * *Files identical despite different names*

### Comparing `sensestreet-1.0.7/PKG-INFO` & `sensestreet-1.0.8/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,18 +1,21 @@
 Metadata-Version: 2.1
 Name: sensestreet
-Version: 1.0.7
-Summary: UNKNOWN
+Version: 1.0.8
 Home-page: https://sensestreet.com
 Author: Sense Street
 Author-email: engineering@sensestreet.com
 License: Apache
-Platform: UNKNOWN
 Description-Content-Type: text/markdown
 License-File: LICENSE
+Requires-Dist: requests
+Requires-Dist: PyJWT
+Requires-Dist: cryptography
+Requires-Dist: lxml
+Requires-Dist: Faker
 
 # SenseStreetClient
 This is a Python client for Sense Street API.
 
 # Run the client
 In order to use the client, import SenseStreetClient from sensestreet:
 ```
@@ -125,8 +128,7 @@
 anonymise_bbg_xml(
     "./example.xml",
     "./test.xml",
     "./mapping.json",
     r"\bbank\b",
 )
 ```
-
```

### Comparing `sensestreet-1.0.7/README.md` & `sensestreet-1.0.8/README.md`

 * *Files identical despite different names*

### Comparing `sensestreet-1.0.7/setup.py` & `sensestreet-1.0.8/setup.py`

 * *Files 16% similar despite different names*

```diff
@@ -3,15 +3,15 @@
 from pathlib import Path
 this_directory = Path(__file__).parent
 long_description = (this_directory / "README.md").read_text()
 
 
 setup(
     name='sensestreet',
-    version='1.0.7',
+    version='1.0.8',
     license='Apache',
     packages=find_packages('src'),
     author="Sense Street",
     author_email="engineering@sensestreet.com",
     url="https://sensestreet.com",
     package_dir={'': 'src'},
     install_requires=[
```

### Comparing `sensestreet-1.0.7/src/sensestreet/anonymise.py` & `sensestreet-1.0.8/src/sensestreet/anonymise.py`

 * *Files identical despite different names*

### Comparing `sensestreet-1.0.7/src/sensestreet/sensestreet_client.py` & `sensestreet-1.0.8/src/sensestreet/sensestreet_client.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,17 +1,18 @@
 import json
 from datetime import datetime, timedelta
 import pathlib
 import re
 from typing import List
-
+import os
 import requests
 import jwt  # pip install pyjwt
 from cryptography.hazmat.primitives import serialization
-
+import shutil
+import tempfile
 """
 Tested on:
 python==3.8.10
 requests==2.28.1
 PyJWT==2.3.0
 cryptography==37.0.2
 """
@@ -68,15 +69,15 @@
     get_conv_file_status(file_id):
         Check if conversations sent in file with the file_id have already been processed.
 
 
 
     """
 
-    __version__ = "1.0.7"
+    __version__ = "1.0.8"
 
     def __init__(
         self,
         app_id,
         api_url,
         priv_key_path=None,
         pub_key_id="default.pub",
@@ -176,31 +177,48 @@
             timeout=self.req_timeout_sec,
             **self.request_args,
         )
         res.raise_for_status()
         res_json = json.loads(res.text)
         return res_json
 
-    def upload_files_with_conversations(self, files_paths):
+    def upload_files_with_conversations(self, files_paths, compress=True):
         """Uploads list of files with conversations to be processed by the server."""
         conv_upload_url = f"{self.api_url}/conversations"
         if not isinstance(files_paths, list):
             raise RuntimeError(
                 "Please provide list of filenames even if you're sending just one file"
             )
-            return
-        files = []
-        auth_headers = self._get_headers(True)
-        for file_path in files_paths:
-            file = pathlib.Path(file_path)
-            files.append(("files", file.open("rb")))
+            
+        try:
+            if compress:
+                tempdir = tempfile.mkdtemp()
+                archive_dir = tempfile.mkdtemp()
+                for file_path in files_paths:
+                    shutil.copy(file_path, os.path.join(tempdir, os.path.basename(file_path)))
+
+                tmp_archive = os.path.join(archive_dir, 'archive')
+                shutil.make_archive(tmp_archive, 'zip', tempdir)
+                tmp_archive += ".zip"
+                files_paths = [tmp_archive]
+
+            files = []
+            auth_headers = self._get_headers(True)
+            for file_path in files_paths:
+                file = pathlib.Path(file_path)
+                files.append(("files", file.open("rb")))
+
+            resp = requests.post(
+                url=conv_upload_url, files=files, headers=auth_headers, **self.request_args
+            )
+        finally:
+            if compress:
+                shutil.rmtree(archive_dir)
+                shutil.rmtree(tempdir)
 
-        resp = requests.post(
-            url=conv_upload_url, files=files, headers=auth_headers, **self.request_args
-        )
         return resp.json()
 
     def upload_file_with_bond_ref_data(self, file_path):
         """Uploads file with bond data to be added to the server."""
         bond_upload_url = f"{self.api_url}/bonds"
         file = pathlib.Path(file_path)
         resp = requests.post(
@@ -214,19 +232,20 @@
     def get_processed_conv_file(self, file_id, output_file_path):
         """Returns file with processed conversations."""
         url = f"{self.api_url}/conversations/file/{file_id}"
         get_response = requests.get(url=url, stream=True, headers=self._get_headers())
         if get_response.status_code != 200:
             return get_response.json()
         file_name = url.split("/")[-1]
-        with open(output_file_path, "wb") as f:
+        download_path = output_file_path+file_name+".json"
+        with open(download_path, "wb") as f:
             for chunk in get_response.iter_content(chunk_size=1024):
                 if chunk:
                     f.write(chunk)
-        return f"File saved under {output_file_path+file_name}.json"
+        return f"File saved under {download_path}"
 
     def get_conv_file_status(self, file_id):
         """Returns status of the conversations sent in a given file for the processing by the server."""
         url = f"{self.api_url}/conversations/status/{file_id}"
         resp = requests.get(url=url, headers=self._get_headers(), **self.request_args)
         return resp.json()
```

### Comparing `sensestreet-1.0.7/src/sensestreet.egg-info/PKG-INFO` & `sensestreet-1.0.8/src/sensestreet.egg-info/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,18 +1,21 @@
 Metadata-Version: 2.1
 Name: sensestreet
-Version: 1.0.7
-Summary: UNKNOWN
+Version: 1.0.8
 Home-page: https://sensestreet.com
 Author: Sense Street
 Author-email: engineering@sensestreet.com
 License: Apache
-Platform: UNKNOWN
 Description-Content-Type: text/markdown
 License-File: LICENSE
+Requires-Dist: requests
+Requires-Dist: PyJWT
+Requires-Dist: cryptography
+Requires-Dist: lxml
+Requires-Dist: Faker
 
 # SenseStreetClient
 This is a Python client for Sense Street API.
 
 # Run the client
 In order to use the client, import SenseStreetClient from sensestreet:
 ```
@@ -125,8 +128,7 @@
 anonymise_bbg_xml(
     "./example.xml",
     "./test.xml",
     "./mapping.json",
     r"\bbank\b",
 )
 ```
-
```

