# Comparing `tmp/dataverse_sdk-1.3.0.tar.gz` & `tmp/dataverse_sdk-1.3.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dataverse_sdk-1.3.0.tar", last modified: Wed May 22 09:09:49 2024, max compression
+gzip compressed data, was "dataverse_sdk-1.3.1.tar", last modified: Wed May 29 05:54:07 2024, max compression
```

## Comparing `dataverse_sdk-1.3.0.tar` & `dataverse_sdk-1.3.1.tar`

### file list

```diff
@@ -1,30 +1,30 @@
-drwxr-xr-x   0 yihsuanchen   (501) staff       (20)        0 2024-05-22 09:09:49.616184 dataverse_sdk-1.3.0/
--rw-r--r--   0 yihsuanchen   (501) staff       (20)    14596 2024-05-22 09:09:49.615946 dataverse_sdk-1.3.0/PKG-INFO
--rw-r--r--   0 yihsuanchen   (501) staff       (20)    14273 2024-05-22 09:09:19.000000 dataverse_sdk-1.3.0/README.md
-drwxr-xr-x   0 yihsuanchen   (501) staff       (20)        0 2024-05-22 09:09:49.612956 dataverse_sdk-1.3.0/dataverse_sdk/
--rw-r--r--   0 yihsuanchen   (501) staff       (20)      825 2023-12-21 03:02:11.000000 dataverse_sdk-1.3.0/dataverse_sdk/__init__.py
-drwxr-xr-x   0 yihsuanchen   (501) staff       (20)        0 2024-05-22 09:09:49.613904 dataverse_sdk-1.3.0/dataverse_sdk/apis/
--rw-r--r--   0 yihsuanchen   (501) staff       (20)        0 2023-12-21 03:02:11.000000 dataverse_sdk-1.3.0/dataverse_sdk/apis/__init__.py
--rw-r--r--   0 yihsuanchen   (501) staff       (20)    11552 2024-05-22 09:09:19.000000 dataverse_sdk-1.3.0/dataverse_sdk/apis/backend.py
--rw-r--r--   0 yihsuanchen   (501) staff       (20)    37893 2024-05-22 09:09:19.000000 dataverse_sdk-1.3.0/dataverse_sdk/client.py
--rw-r--r--   0 yihsuanchen   (501) staff       (20)     1872 2024-01-18 02:49:01.000000 dataverse_sdk-1.3.0/dataverse_sdk/connections.py
--rw-r--r--   0 yihsuanchen   (501) staff       (20)      776 2024-05-22 09:09:19.000000 dataverse_sdk-1.3.0/dataverse_sdk/constants.py
-drwxr-xr-x   0 yihsuanchen   (501) staff       (20)        0 2024-05-22 09:09:49.614192 dataverse_sdk-1.3.0/dataverse_sdk/exceptions/
--rw-r--r--   0 yihsuanchen   (501) staff       (20)        0 2023-12-21 03:02:11.000000 dataverse_sdk-1.3.0/dataverse_sdk/exceptions/__init__.py
--rw-r--r--   0 yihsuanchen   (501) staff       (20)      141 2024-05-20 09:34:51.000000 dataverse_sdk-1.3.0/dataverse_sdk/exceptions/client.py
-drwxr-xr-x   0 yihsuanchen   (501) staff       (20)        0 2024-05-22 09:09:49.615064 dataverse_sdk-1.3.0/dataverse_sdk/schemas/
--rw-r--r--   0 yihsuanchen   (501) staff       (20)        0 2023-12-21 03:02:11.000000 dataverse_sdk-1.3.0/dataverse_sdk/schemas/__init__.py
--rw-r--r--   0 yihsuanchen   (501) staff       (20)     3120 2023-12-21 03:02:11.000000 dataverse_sdk-1.3.0/dataverse_sdk/schemas/api.py
--rw-r--r--   0 yihsuanchen   (501) staff       (20)    12556 2024-01-18 02:49:01.000000 dataverse_sdk-1.3.0/dataverse_sdk/schemas/client.py
--rw-r--r--   0 yihsuanchen   (501) staff       (20)     1216 2024-05-21 02:03:44.000000 dataverse_sdk-1.3.0/dataverse_sdk/schemas/common.py
-drwxr-xr-x   0 yihsuanchen   (501) staff       (20)        0 2024-05-22 09:09:49.615413 dataverse_sdk-1.3.0/dataverse_sdk/utils/
--rw-r--r--   0 yihsuanchen   (501) staff       (20)        0 2023-12-21 03:02:11.000000 dataverse_sdk-1.3.0/dataverse_sdk/utils/__init__.py
--rw-r--r--   0 yihsuanchen   (501) staff       (20)      657 2023-12-21 03:02:11.000000 dataverse_sdk-1.3.0/dataverse_sdk/utils/utils.py
-drwxr-xr-x   0 yihsuanchen   (501) staff       (20)        0 2024-05-22 09:09:49.615733 dataverse_sdk-1.3.0/dataverse_sdk.egg-info/
--rw-r--r--   0 yihsuanchen   (501) staff       (20)    14596 2024-05-22 09:09:49.000000 dataverse_sdk-1.3.0/dataverse_sdk.egg-info/PKG-INFO
--rw-r--r--   0 yihsuanchen   (501) staff       (20)      629 2024-05-22 09:09:49.000000 dataverse_sdk-1.3.0/dataverse_sdk.egg-info/SOURCES.txt
--rw-r--r--   0 yihsuanchen   (501) staff       (20)        1 2024-05-22 09:09:49.000000 dataverse_sdk-1.3.0/dataverse_sdk.egg-info/dependency_links.txt
--rw-r--r--   0 yihsuanchen   (501) staff       (20)       37 2024-05-22 09:09:49.000000 dataverse_sdk-1.3.0/dataverse_sdk.egg-info/requires.txt
--rw-r--r--   0 yihsuanchen   (501) staff       (20)       14 2024-05-22 09:09:49.000000 dataverse_sdk-1.3.0/dataverse_sdk.egg-info/top_level.txt
--rw-r--r--   0 yihsuanchen   (501) staff       (20)       38 2024-05-22 09:09:49.616223 dataverse_sdk-1.3.0/setup.cfg
--rw-r--r--   0 yihsuanchen   (501) staff       (20)      636 2024-05-22 09:09:19.000000 dataverse_sdk-1.3.0/setup.py
+drwxr-xr-x   0 yihsuanchen   (501) staff       (20)        0 2024-05-29 05:54:07.938346 dataverse_sdk-1.3.1/
+-rw-r--r--   0 yihsuanchen   (501) staff       (20)    14596 2024-05-29 05:54:07.938132 dataverse_sdk-1.3.1/PKG-INFO
+-rw-r--r--   0 yihsuanchen   (501) staff       (20)    14273 2024-05-22 09:09:19.000000 dataverse_sdk-1.3.1/README.md
+drwxr-xr-x   0 yihsuanchen   (501) staff       (20)        0 2024-05-29 05:54:07.935176 dataverse_sdk-1.3.1/dataverse_sdk/
+-rw-r--r--   0 yihsuanchen   (501) staff       (20)      825 2023-12-21 03:02:11.000000 dataverse_sdk-1.3.1/dataverse_sdk/__init__.py
+drwxr-xr-x   0 yihsuanchen   (501) staff       (20)        0 2024-05-29 05:54:07.936095 dataverse_sdk-1.3.1/dataverse_sdk/apis/
+-rw-r--r--   0 yihsuanchen   (501) staff       (20)        0 2023-12-21 03:02:11.000000 dataverse_sdk-1.3.1/dataverse_sdk/apis/__init__.py
+-rw-r--r--   0 yihsuanchen   (501) staff       (20)    11553 2024-05-29 05:53:57.000000 dataverse_sdk-1.3.1/dataverse_sdk/apis/backend.py
+-rw-r--r--   0 yihsuanchen   (501) staff       (20)    37893 2024-05-22 09:09:19.000000 dataverse_sdk-1.3.1/dataverse_sdk/client.py
+-rw-r--r--   0 yihsuanchen   (501) staff       (20)     1872 2024-01-18 02:49:01.000000 dataverse_sdk-1.3.1/dataverse_sdk/connections.py
+-rw-r--r--   0 yihsuanchen   (501) staff       (20)      776 2024-05-22 09:09:19.000000 dataverse_sdk-1.3.1/dataverse_sdk/constants.py
+drwxr-xr-x   0 yihsuanchen   (501) staff       (20)        0 2024-05-29 05:54:07.936327 dataverse_sdk-1.3.1/dataverse_sdk/exceptions/
+-rw-r--r--   0 yihsuanchen   (501) staff       (20)        0 2023-12-21 03:02:11.000000 dataverse_sdk-1.3.1/dataverse_sdk/exceptions/__init__.py
+-rw-r--r--   0 yihsuanchen   (501) staff       (20)      141 2024-05-20 09:34:51.000000 dataverse_sdk-1.3.1/dataverse_sdk/exceptions/client.py
+drwxr-xr-x   0 yihsuanchen   (501) staff       (20)        0 2024-05-29 05:54:07.937161 dataverse_sdk-1.3.1/dataverse_sdk/schemas/
+-rw-r--r--   0 yihsuanchen   (501) staff       (20)        0 2023-12-21 03:02:11.000000 dataverse_sdk-1.3.1/dataverse_sdk/schemas/__init__.py
+-rw-r--r--   0 yihsuanchen   (501) staff       (20)     3120 2023-12-21 03:02:11.000000 dataverse_sdk-1.3.1/dataverse_sdk/schemas/api.py
+-rw-r--r--   0 yihsuanchen   (501) staff       (20)    12556 2024-01-18 02:49:01.000000 dataverse_sdk-1.3.1/dataverse_sdk/schemas/client.py
+-rw-r--r--   0 yihsuanchen   (501) staff       (20)     1216 2024-05-21 02:03:44.000000 dataverse_sdk-1.3.1/dataverse_sdk/schemas/common.py
+drwxr-xr-x   0 yihsuanchen   (501) staff       (20)        0 2024-05-29 05:54:07.937608 dataverse_sdk-1.3.1/dataverse_sdk/utils/
+-rw-r--r--   0 yihsuanchen   (501) staff       (20)        0 2023-12-21 03:02:11.000000 dataverse_sdk-1.3.1/dataverse_sdk/utils/__init__.py
+-rw-r--r--   0 yihsuanchen   (501) staff       (20)      657 2023-12-21 03:02:11.000000 dataverse_sdk-1.3.1/dataverse_sdk/utils/utils.py
+drwxr-xr-x   0 yihsuanchen   (501) staff       (20)        0 2024-05-29 05:54:07.937920 dataverse_sdk-1.3.1/dataverse_sdk.egg-info/
+-rw-r--r--   0 yihsuanchen   (501) staff       (20)    14596 2024-05-29 05:54:07.000000 dataverse_sdk-1.3.1/dataverse_sdk.egg-info/PKG-INFO
+-rw-r--r--   0 yihsuanchen   (501) staff       (20)      629 2024-05-29 05:54:07.000000 dataverse_sdk-1.3.1/dataverse_sdk.egg-info/SOURCES.txt
+-rw-r--r--   0 yihsuanchen   (501) staff       (20)        1 2024-05-29 05:54:07.000000 dataverse_sdk-1.3.1/dataverse_sdk.egg-info/dependency_links.txt
+-rw-r--r--   0 yihsuanchen   (501) staff       (20)       37 2024-05-29 05:54:07.000000 dataverse_sdk-1.3.1/dataverse_sdk.egg-info/requires.txt
+-rw-r--r--   0 yihsuanchen   (501) staff       (20)       14 2024-05-29 05:54:07.000000 dataverse_sdk-1.3.1/dataverse_sdk.egg-info/top_level.txt
+-rw-r--r--   0 yihsuanchen   (501) staff       (20)       38 2024-05-29 05:54:07.938391 dataverse_sdk-1.3.1/setup.cfg
+-rw-r--r--   0 yihsuanchen   (501) staff       (20)      636 2024-05-29 05:53:57.000000 dataverse_sdk-1.3.1/setup.py
```

### Comparing `dataverse_sdk-1.3.0/PKG-INFO` & `dataverse_sdk-1.3.1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: dataverse-sdk
-Version: 1.3.0
+Version: 1.3.1
 Summary: Dataverse SDK For Python
 Home-page: 
 Author: LinkerVision
 Classifier: Programming Language :: Python :: 3
 Requires-Python: >=3.10, <4
 Description-Content-Type: text/markdown
 Requires-Dist: pydantic==1.*
```

### Comparing `dataverse_sdk-1.3.0/README.md` & `dataverse_sdk-1.3.1/README.md`

 * *Files identical despite different names*

### Comparing `dataverse_sdk-1.3.0/dataverse_sdk/__init__.py` & `dataverse_sdk-1.3.1/dataverse_sdk/__init__.py`

 * *Files identical despite different names*

### Comparing `dataverse_sdk-1.3.0/dataverse_sdk/apis/backend.py` & `dataverse_sdk-1.3.1/dataverse_sdk/apis/backend.py`

 * *Files 0% similar despite different names*

```diff
@@ -180,15 +180,15 @@
             headers=self.headers,
             data=data,
         )
         return resp.json()
 
     def get_project(self, project_id) -> dict:
         resp = self.send_request(
-            url=f"{self.host}/api/projects/{project_id}",
+            url=f"{self.host}/api/projects/{project_id}/",
             method="get",
             headers=self.headers,
         )
         return resp.json()
 
     def list_projects(
         self,
```

### Comparing `dataverse_sdk-1.3.0/dataverse_sdk/client.py` & `dataverse_sdk-1.3.1/dataverse_sdk/client.py`

 * *Files identical despite different names*

### Comparing `dataverse_sdk-1.3.0/dataverse_sdk/connections.py` & `dataverse_sdk-1.3.1/dataverse_sdk/connections.py`

 * *Files identical despite different names*

### Comparing `dataverse_sdk-1.3.0/dataverse_sdk/constants.py` & `dataverse_sdk-1.3.1/dataverse_sdk/constants.py`

 * *Files identical despite different names*

### Comparing `dataverse_sdk-1.3.0/dataverse_sdk/schemas/api.py` & `dataverse_sdk-1.3.1/dataverse_sdk/schemas/api.py`

 * *Files identical despite different names*

### Comparing `dataverse_sdk-1.3.0/dataverse_sdk/schemas/client.py` & `dataverse_sdk-1.3.1/dataverse_sdk/schemas/client.py`

 * *Files identical despite different names*

### Comparing `dataverse_sdk-1.3.0/dataverse_sdk/schemas/common.py` & `dataverse_sdk-1.3.1/dataverse_sdk/schemas/common.py`

 * *Files identical despite different names*

### Comparing `dataverse_sdk-1.3.0/dataverse_sdk/utils/utils.py` & `dataverse_sdk-1.3.1/dataverse_sdk/utils/utils.py`

 * *Files identical despite different names*

### Comparing `dataverse_sdk-1.3.0/dataverse_sdk.egg-info/PKG-INFO` & `dataverse_sdk-1.3.1/dataverse_sdk.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: dataverse-sdk
-Version: 1.3.0
+Version: 1.3.1
 Summary: Dataverse SDK For Python
 Home-page: 
 Author: LinkerVision
 Classifier: Programming Language :: Python :: 3
 Requires-Python: >=3.10, <4
 Description-Content-Type: text/markdown
 Requires-Dist: pydantic==1.*
```

### Comparing `dataverse_sdk-1.3.0/dataverse_sdk.egg-info/SOURCES.txt` & `dataverse_sdk-1.3.1/dataverse_sdk.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `dataverse_sdk-1.3.0/setup.py` & `dataverse_sdk-1.3.1/setup.py`

 * *Files 19% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from setuptools import find_packages, setup
 
 AUTHOR = "LinkerVision"
 PACKAGE_NAME = "dataverse-sdk"
-PACKAGE_VERSION = "1.3.0"
+PACKAGE_VERSION = "1.3.1"
 DESC = "Dataverse SDK For Python"
 with open("README.md", encoding="utf-8") as fh:
     long_description = fh.read()
 
 setup(
     name=PACKAGE_NAME,
     version=PACKAGE_VERSION,
```

