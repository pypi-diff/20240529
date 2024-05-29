# Comparing `tmp/oasees_sdk-0.3.1.tar.gz` & `tmp/oasees_sdk-0.3.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "oasees_sdk-0.3.1.tar", max compression
+gzip compressed data, was "oasees_sdk-0.3.2.tar", max compression
```

## Comparing `oasees_sdk-0.3.1.tar` & `oasees_sdk-0.3.2.tar`

### file list

```diff
@@ -1,8 +1,13 @@
--rw-r--r--   0        0        0       10 2024-04-22 11:03:39.624851 oasees_sdk-0.3.1/README.md
--rw-r--r--   0        0        0      619 2024-05-24 13:02:49.008885 oasees_sdk-0.3.1/pyproject.toml
--rw-r--r--   0        0        0    33029 2024-05-24 13:03:46.672598 oasees_sdk-0.3.1/src/oasees_sdk/cli/cli.py
--rw-r--r--   0        0        0       18 2024-05-10 14:31:20.743803 oasees_sdk-0.3.1/src/oasees_sdk/oasees_sdk/__init__.py
--rw-r--r--   0        0        0      887 2024-05-10 14:31:20.755803 oasees_sdk-0.3.1/src/oasees_sdk/oasees_sdk/cluster_ipfs_upload.py
--rw-r--r--   0        0        0     1934 2024-05-10 14:31:20.699804 oasees_sdk-0.3.1/src/oasees_sdk/oasees_sdk/deploy_pipeline.py
--rw-r--r--   0        0        0    10095 2024-05-24 12:42:10.295086 oasees_sdk-0.3.1/src/oasees_sdk/oasees_sdk/sdk.py
--rw-r--r--   0        0        0     1074 1970-01-01 00:00:00.000000 oasees_sdk-0.3.1/PKG-INFO
+-rw-r--r--   0        0        0     4870 2024-05-28 16:04:12.456607 oasees_sdk-0.3.2/README.md
+-rw-r--r--   0        0        0      619 2024-05-29 10:42:55.900090 oasees_sdk-0.3.2/pyproject.toml
+-rw-r--r--   0        0        0    20827 2024-05-29 08:39:46.120797 oasees_sdk-0.3.2/src/oasees_sdk/cli/__pycache__/cli.cpython-310.pyc
+-rw-r--r--   0        0        0    33029 2024-05-24 13:19:35.008849 oasees_sdk-0.3.2/src/oasees_sdk/cli/cli.py
+-rw-r--r--   0        0        0       18 2024-05-10 14:31:20.743803 oasees_sdk-0.3.2/src/oasees_sdk/oasees_sdk/__init__.py
+-rw-r--r--   0        0        0      177 2024-05-29 10:17:44.127715 oasees_sdk-0.3.2/src/oasees_sdk/oasees_sdk/__pycache__/__init__.cpython-310.pyc
+-rw-r--r--   0        0        0     1263 2024-05-29 10:17:44.559713 oasees_sdk-0.3.2/src/oasees_sdk/oasees_sdk/__pycache__/cluster_ipfs_upload.cpython-310.pyc
+-rw-r--r--   0        0        0     1841 2024-05-29 10:17:44.555713 oasees_sdk-0.3.2/src/oasees_sdk/oasees_sdk/__pycache__/deploy_pipeline.cpython-310.pyc
+-rw-r--r--   0        0        0     9078 2024-05-29 10:33:09.879030 oasees_sdk-0.3.2/src/oasees_sdk/oasees_sdk/__pycache__/sdk.cpython-310.pyc
+-rw-r--r--   0        0        0      887 2024-05-10 14:31:20.755803 oasees_sdk-0.3.2/src/oasees_sdk/oasees_sdk/cluster_ipfs_upload.py
+-rw-r--r--   0        0        0     1934 2024-05-10 14:31:20.699804 oasees_sdk-0.3.2/src/oasees_sdk/oasees_sdk/deploy_pipeline.py
+-rw-r--r--   0        0        0    11113 2024-05-29 10:42:25.404243 oasees_sdk-0.3.2/src/oasees_sdk/oasees_sdk/sdk.py
+-rw-r--r--   0        0        0     5934 1970-01-01 00:00:00.000000 oasees_sdk-0.3.2/PKG-INFO
```

### Comparing `oasees_sdk-0.3.1/pyproject.toml` & `oasees_sdk-0.3.2/pyproject.toml`

 * *Files 18% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["poetry-core>=1.0.0"]
 build-backend = "poetry.core.masonry.api"
 
 [tool.poetry]
 name = "oasees_sdk"
-version = "0.3.1"
+version = "0.3.2"
 description = "Oasees SDK"
 authors = [
     "Example Author <author@example.com>",
 ]
 readme = "README.md"
 classifiers = [
     "Programming Language :: Python :: 3",
```

### Comparing `oasees_sdk-0.3.1/src/oasees_sdk/cli/cli.py` & `oasees_sdk-0.3.2/src/oasees_sdk/cli/cli.py`

 * *Files identical despite different names*

### Comparing `oasees_sdk-0.3.1/src/oasees_sdk/oasees_sdk/cluster_ipfs_upload.py` & `oasees_sdk-0.3.2/src/oasees_sdk/oasees_sdk/cluster_ipfs_upload.py`

 * *Files identical despite different names*

### Comparing `oasees_sdk-0.3.1/src/oasees_sdk/oasees_sdk/deploy_pipeline.py` & `oasees_sdk-0.3.2/src/oasees_sdk/oasees_sdk/deploy_pipeline.py`

 * *Files identical despite different names*

