# Comparing `tmp/aws_boto3_sdk_helpers-1.0.1.tar.gz` & `tmp/aws_boto3_sdk_helpers-1.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "aws_boto3_sdk_helpers-1.0.1.tar", last modified: Wed May 29 10:52:23 2024, max compression
+gzip compressed data, was "aws_boto3_sdk_helpers-1.0.2.tar", last modified: Wed May 29 11:00:02 2024, max compression
```

## Comparing `aws_boto3_sdk_helpers-1.0.1.tar` & `aws_boto3_sdk_helpers-1.0.2.tar`

### file list

```diff
@@ -1,24 +1,24 @@
-drwxr-xr-x   0 ska       (1000) ska       (1000)        0 2024-05-29 10:52:23.720664 aws_boto3_sdk_helpers-1.0.1/
--rw-r--r--   0 ska       (1000) ska       (1000)     1070 2024-05-29 10:36:56.000000 aws_boto3_sdk_helpers-1.0.1/LICENSE
--rw-r--r--   0 ska       (1000) ska       (1000)      443 2024-05-29 10:52:23.720664 aws_boto3_sdk_helpers-1.0.1/PKG-INFO
--rw-r--r--   0 ska       (1000) ska       (1000)      681 2024-05-29 10:43:53.000000 aws_boto3_sdk_helpers-1.0.1/README.md
-drwxr-xr-x   0 ska       (1000) ska       (1000)        0 2024-05-29 10:52:23.720664 aws_boto3_sdk_helpers-1.0.1/aws_boto3_sdk_helpers.egg-info/
--rw-r--r--   0 ska       (1000) ska       (1000)      443 2024-05-29 10:52:23.000000 aws_boto3_sdk_helpers-1.0.1/aws_boto3_sdk_helpers.egg-info/PKG-INFO
--rw-r--r--   0 ska       (1000) ska       (1000)      509 2024-05-29 10:52:23.000000 aws_boto3_sdk_helpers-1.0.1/aws_boto3_sdk_helpers.egg-info/SOURCES.txt
--rw-r--r--   0 ska       (1000) ska       (1000)        1 2024-05-29 10:52:23.000000 aws_boto3_sdk_helpers-1.0.1/aws_boto3_sdk_helpers.egg-info/dependency_links.txt
--rw-r--r--   0 ska       (1000) ska       (1000)       15 2024-05-29 10:52:23.000000 aws_boto3_sdk_helpers-1.0.1/aws_boto3_sdk_helpers.egg-info/requires.txt
--rw-r--r--   0 ska       (1000) ska       (1000)       15 2024-05-29 10:52:23.000000 aws_boto3_sdk_helpers-1.0.1/aws_boto3_sdk_helpers.egg-info/top_level.txt
-drwxr-xr-x   0 ska       (1000) ska       (1000)        0 2024-05-29 10:52:23.720664 aws_boto3_sdk_helpers-1.0.1/buckets/
--rw-r--r--   0 ska       (1000) ska       (1000)       36 2024-05-08 02:08:32.000000 aws_boto3_sdk_helpers-1.0.1/buckets/__init__.py
--rw-r--r--   0 ska       (1000) ska       (1000)     2966 2024-05-08 02:08:32.000000 aws_boto3_sdk_helpers-1.0.1/buckets/delete_bucket_functions.py
--rw-r--r--   0 ska       (1000) ska       (1000)     1168 2024-05-08 02:08:32.000000 aws_boto3_sdk_helpers-1.0.1/buckets/get_bucket_functions.py
--rw-r--r--   0 ska       (1000) ska       (1000)     1671 2024-05-08 02:08:32.000000 aws_boto3_sdk_helpers-1.0.1/buckets/list_bucket_functions.py
--rw-r--r--   0 ska       (1000) ska       (1000)     1149 2024-05-07 17:17:30.000000 aws_boto3_sdk_helpers-1.0.1/buckets/s3funcs.py
--rw-r--r--   0 ska       (1000) ska       (1000)      651 2024-05-07 17:17:30.000000 aws_boto3_sdk_helpers-1.0.1/buckets/test_s3funcs.py
-drwxr-xr-x   0 ska       (1000) ska       (1000)        0 2024-05-29 10:52:23.720664 aws_boto3_sdk_helpers-1.0.1/common/
--rw-r--r--   0 ska       (1000) ska       (1000)       57 2024-05-08 02:08:32.000000 aws_boto3_sdk_helpers-1.0.1/common/__init__.py
--rw-r--r--   0 ska       (1000) ska       (1000)      848 2024-05-08 02:08:32.000000 aws_boto3_sdk_helpers-1.0.1/common/args.py
--rw-r--r--   0 ska       (1000) ska       (1000)     1070 2024-05-08 02:08:32.000000 aws_boto3_sdk_helpers-1.0.1/common/banners.py
--rw-r--r--   0 ska       (1000) ska       (1000)      182 2024-05-08 02:08:32.000000 aws_boto3_sdk_helpers-1.0.1/common/boto_client_declaration.py
--rw-r--r--   0 ska       (1000) ska       (1000)      587 2024-05-29 10:52:23.720664 aws_boto3_sdk_helpers-1.0.1/setup.cfg
--rw-r--r--   0 ska       (1000) ska       (1000)       38 2024-05-29 10:50:16.000000 aws_boto3_sdk_helpers-1.0.1/setup.py
+drwxr-xr-x   0 ska       (1000) ska       (1000)        0 2024-05-29 11:00:02.834310 aws_boto3_sdk_helpers-1.0.2/
+-rw-r--r--   0 ska       (1000) ska       (1000)     1070 2024-05-29 10:36:56.000000 aws_boto3_sdk_helpers-1.0.2/LICENSE
+-rw-r--r--   0 ska       (1000) ska       (1000)      452 2024-05-29 11:00:02.834310 aws_boto3_sdk_helpers-1.0.2/PKG-INFO
+-rw-r--r--   0 ska       (1000) ska       (1000)      681 2024-05-29 10:59:06.000000 aws_boto3_sdk_helpers-1.0.2/README.md
+drwxr-xr-x   0 ska       (1000) ska       (1000)        0 2024-05-29 11:00:02.834310 aws_boto3_sdk_helpers-1.0.2/aws_boto3_sdk_helpers.egg-info/
+-rw-r--r--   0 ska       (1000) ska       (1000)      452 2024-05-29 11:00:02.000000 aws_boto3_sdk_helpers-1.0.2/aws_boto3_sdk_helpers.egg-info/PKG-INFO
+-rw-r--r--   0 ska       (1000) ska       (1000)      509 2024-05-29 11:00:02.000000 aws_boto3_sdk_helpers-1.0.2/aws_boto3_sdk_helpers.egg-info/SOURCES.txt
+-rw-r--r--   0 ska       (1000) ska       (1000)        1 2024-05-29 11:00:02.000000 aws_boto3_sdk_helpers-1.0.2/aws_boto3_sdk_helpers.egg-info/dependency_links.txt
+-rw-r--r--   0 ska       (1000) ska       (1000)       15 2024-05-29 11:00:02.000000 aws_boto3_sdk_helpers-1.0.2/aws_boto3_sdk_helpers.egg-info/requires.txt
+-rw-r--r--   0 ska       (1000) ska       (1000)       15 2024-05-29 11:00:02.000000 aws_boto3_sdk_helpers-1.0.2/aws_boto3_sdk_helpers.egg-info/top_level.txt
+drwxr-xr-x   0 ska       (1000) ska       (1000)        0 2024-05-29 11:00:02.834310 aws_boto3_sdk_helpers-1.0.2/buckets/
+-rw-r--r--   0 ska       (1000) ska       (1000)       36 2024-05-08 02:08:32.000000 aws_boto3_sdk_helpers-1.0.2/buckets/__init__.py
+-rw-r--r--   0 ska       (1000) ska       (1000)     2966 2024-05-08 02:08:32.000000 aws_boto3_sdk_helpers-1.0.2/buckets/delete_bucket_functions.py
+-rw-r--r--   0 ska       (1000) ska       (1000)     1168 2024-05-08 02:08:32.000000 aws_boto3_sdk_helpers-1.0.2/buckets/get_bucket_functions.py
+-rw-r--r--   0 ska       (1000) ska       (1000)     1671 2024-05-08 02:08:32.000000 aws_boto3_sdk_helpers-1.0.2/buckets/list_bucket_functions.py
+-rw-r--r--   0 ska       (1000) ska       (1000)     1149 2024-05-07 17:17:30.000000 aws_boto3_sdk_helpers-1.0.2/buckets/s3funcs.py
+-rw-r--r--   0 ska       (1000) ska       (1000)      651 2024-05-07 17:17:30.000000 aws_boto3_sdk_helpers-1.0.2/buckets/test_s3funcs.py
+drwxr-xr-x   0 ska       (1000) ska       (1000)        0 2024-05-29 11:00:02.834310 aws_boto3_sdk_helpers-1.0.2/common/
+-rw-r--r--   0 ska       (1000) ska       (1000)       57 2024-05-08 02:08:32.000000 aws_boto3_sdk_helpers-1.0.2/common/__init__.py
+-rw-r--r--   0 ska       (1000) ska       (1000)      848 2024-05-08 02:08:32.000000 aws_boto3_sdk_helpers-1.0.2/common/args.py
+-rw-r--r--   0 ska       (1000) ska       (1000)     1070 2024-05-08 02:08:32.000000 aws_boto3_sdk_helpers-1.0.2/common/banners.py
+-rw-r--r--   0 ska       (1000) ska       (1000)      182 2024-05-08 02:08:32.000000 aws_boto3_sdk_helpers-1.0.2/common/boto_client_declaration.py
+-rw-r--r--   0 ska       (1000) ska       (1000)      581 2024-05-29 11:00:02.834310 aws_boto3_sdk_helpers-1.0.2/setup.cfg
+-rw-r--r--   0 ska       (1000) ska       (1000)       38 2024-05-29 10:59:06.000000 aws_boto3_sdk_helpers-1.0.2/setup.py
```

### Comparing `aws_boto3_sdk_helpers-1.0.1/LICENSE` & `aws_boto3_sdk_helpers-1.0.2/LICENSE`

 * *Files identical despite different names*

### Comparing `aws_boto3_sdk_helpers-1.0.1/README.md` & `aws_boto3_sdk_helpers-1.0.2/README.md`

 * *Files identical despite different names*

### Comparing `aws_boto3_sdk_helpers-1.0.1/buckets/delete_bucket_functions.py` & `aws_boto3_sdk_helpers-1.0.2/buckets/delete_bucket_functions.py`

 * *Files identical despite different names*

### Comparing `aws_boto3_sdk_helpers-1.0.1/buckets/get_bucket_functions.py` & `aws_boto3_sdk_helpers-1.0.2/buckets/get_bucket_functions.py`

 * *Files identical despite different names*

### Comparing `aws_boto3_sdk_helpers-1.0.1/buckets/list_bucket_functions.py` & `aws_boto3_sdk_helpers-1.0.2/buckets/list_bucket_functions.py`

 * *Files identical despite different names*

### Comparing `aws_boto3_sdk_helpers-1.0.1/buckets/s3funcs.py` & `aws_boto3_sdk_helpers-1.0.2/buckets/s3funcs.py`

 * *Files identical despite different names*

### Comparing `aws_boto3_sdk_helpers-1.0.1/buckets/test_s3funcs.py` & `aws_boto3_sdk_helpers-1.0.2/buckets/test_s3funcs.py`

 * *Files identical despite different names*

### Comparing `aws_boto3_sdk_helpers-1.0.1/common/args.py` & `aws_boto3_sdk_helpers-1.0.2/common/args.py`

 * *Files identical despite different names*

### Comparing `aws_boto3_sdk_helpers-1.0.1/common/banners.py` & `aws_boto3_sdk_helpers-1.0.2/common/banners.py`

 * *Files identical despite different names*

### Comparing `aws_boto3_sdk_helpers-1.0.1/setup.cfg` & `aws_boto3_sdk_helpers-1.0.2/setup.cfg`

 * *Files 27% similar despite different names*

```diff
@@ -1,19 +1,19 @@
 [metadata]
 name = aws-boto3-sdk-helpers
-version = 1.0.1
+version = 1.0.2
 description = Contains helper functions for the AWS Python sdk (Boto3) package.
-long_description = file: README.rst, CHANGELOG.rst, LICENSE.rst
+long_description = file: README.rst, LICENSE.rst
 long_description_content_type = text/markdown
 author = Yiskaneto
 license = MIT
 license_files = 
 	LICENSE
 project_urls = 
-	homepage = https://github.com/openwurl/boto3-helpers
+	homepage = https://github.com/yiskaneto/aws-boto3-sdk-helpers
 classifiers = 
 	Programming Language :: Python :: 3
 keywords = boto3, botocore, aws
 
 [options]
 packages = find:
 python_requires = >=3.8
```

