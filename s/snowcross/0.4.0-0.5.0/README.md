# Comparing `tmp/snowcross-0.4.0.tar.gz` & `tmp/snowcross-0.5.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "snowcross-0.4.0.tar", last modified: Wed Mar 20 06:18:21 2024, max compression
+gzip compressed data, was "snowcross-0.5.0.tar", last modified: Tue May 28 03:47:33 2024, max compression
```

## Comparing `snowcross-0.4.0.tar` & `snowcross-0.5.0.tar`

### file list

```diff
@@ -1,31 +1,31 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-20 06:18:21.340275 snowcross-0.4.0/
--rw-r--r--   0 runner    (1001) docker     (127)    11357 2024-03-20 06:18:01.000000 snowcross-0.4.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)       88 2024-03-20 06:18:01.000000 snowcross-0.4.0/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (127)      575 2024-03-20 06:18:21.340275 snowcross-0.4.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      761 2024-03-20 06:18:01.000000 snowcross-0.4.0/README.md
--rw-r--r--   0 runner    (1001) docker     (127)      438 2024-03-20 06:18:01.000000 snowcross-0.4.0/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)       33 2024-03-20 06:18:01.000000 snowcross-0.4.0/requirements-locator.txt
--rw-r--r--   0 runner    (1001) docker     (127)      163 2024-03-20 06:18:01.000000 snowcross-0.4.0/requirements-test.txt
--rw-r--r--   0 runner    (1001) docker     (127)       52 2024-03-20 06:18:01.000000 snowcross-0.4.0/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-03-20 06:18:21.340275 snowcross-0.4.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)     1153 2024-03-20 06:18:01.000000 snowcross-0.4.0/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-20 06:18:21.340275 snowcross-0.4.0/snowcross/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-03-20 06:18:01.000000 snowcross-0.4.0/snowcross/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     7691 2024-03-20 06:18:01.000000 snowcross-0.4.0/snowcross/aws.py
--rw-r--r--   0 runner    (1001) docker     (127)      646 2024-03-20 06:18:01.000000 snowcross-0.4.0/snowcross/errors.py
--rw-r--r--   0 runner    (1001) docker     (127)     3057 2024-03-20 06:18:01.000000 snowcross-0.4.0/snowcross/locator.py
--rw-r--r--   0 runner    (1001) docker     (127)    10196 2024-03-20 06:18:01.000000 snowcross-0.4.0/snowcross/snowflake.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-20 06:18:21.340275 snowcross-0.4.0/snowcross.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)      575 2024-03-20 06:18:21.000000 snowcross-0.4.0/snowcross.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      511 2024-03-20 06:18:21.000000 snowcross-0.4.0/snowcross.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-03-20 06:18:21.000000 snowcross-0.4.0/snowcross.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)      255 2024-03-20 06:18:21.000000 snowcross-0.4.0/snowcross.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       16 2024-03-20 06:18:21.000000 snowcross-0.4.0/snowcross.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-20 06:18:21.336275 snowcross-0.4.0/tests/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-20 06:18:21.340275 snowcross-0.4.0/tests/fixtures/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-03-20 06:18:01.000000 snowcross-0.4.0/tests/fixtures/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     4133 2024-03-20 06:18:01.000000 snowcross-0.4.0/tests/fixtures/aws.py
--rw-r--r--   0 runner    (1001) docker     (127)     3398 2024-03-20 06:18:01.000000 snowcross-0.4.0/tests/fixtures/snowflake.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-20 06:18:21.340275 snowcross-0.4.0/tests/helpers/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-03-20 06:18:01.000000 snowcross-0.4.0/tests/helpers/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1256 2024-03-20 06:18:01.000000 snowcross-0.4.0/tests/helpers/docker.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-28 03:47:33.991887 snowcross-0.5.0/
+-rw-r--r--   0 runner    (1001) docker     (127)    11357 2024-05-28 03:47:14.000000 snowcross-0.5.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)       88 2024-05-28 03:47:14.000000 snowcross-0.5.0/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (127)      575 2024-05-28 03:47:33.991887 snowcross-0.5.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      761 2024-05-28 03:47:14.000000 snowcross-0.5.0/README.md
+-rw-r--r--   0 runner    (1001) docker     (127)      438 2024-05-28 03:47:14.000000 snowcross-0.5.0/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)       33 2024-05-28 03:47:14.000000 snowcross-0.5.0/requirements-locator.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      163 2024-05-28 03:47:14.000000 snowcross-0.5.0/requirements-test.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       52 2024-05-28 03:47:14.000000 snowcross-0.5.0/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-28 03:47:33.991887 snowcross-0.5.0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)     1153 2024-05-28 03:47:14.000000 snowcross-0.5.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-28 03:47:33.987887 snowcross-0.5.0/snowcross/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-28 03:47:14.000000 snowcross-0.5.0/snowcross/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8567 2024-05-28 03:47:14.000000 snowcross-0.5.0/snowcross/aws.py
+-rw-r--r--   0 runner    (1001) docker     (127)      646 2024-05-28 03:47:14.000000 snowcross-0.5.0/snowcross/errors.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3057 2024-05-28 03:47:14.000000 snowcross-0.5.0/snowcross/locator.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10196 2024-05-28 03:47:14.000000 snowcross-0.5.0/snowcross/snowflake.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-28 03:47:33.987887 snowcross-0.5.0/snowcross.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)      575 2024-05-28 03:47:33.000000 snowcross-0.5.0/snowcross.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      511 2024-05-28 03:47:33.000000 snowcross-0.5.0/snowcross.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-28 03:47:33.000000 snowcross-0.5.0/snowcross.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      255 2024-05-28 03:47:33.000000 snowcross-0.5.0/snowcross.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       16 2024-05-28 03:47:33.000000 snowcross-0.5.0/snowcross.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-28 03:47:33.987887 snowcross-0.5.0/tests/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-28 03:47:33.987887 snowcross-0.5.0/tests/fixtures/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-28 03:47:14.000000 snowcross-0.5.0/tests/fixtures/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4133 2024-05-28 03:47:14.000000 snowcross-0.5.0/tests/fixtures/aws.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3398 2024-05-28 03:47:14.000000 snowcross-0.5.0/tests/fixtures/snowflake.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-28 03:47:33.991887 snowcross-0.5.0/tests/helpers/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-28 03:47:14.000000 snowcross-0.5.0/tests/helpers/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1256 2024-05-28 03:47:14.000000 snowcross-0.5.0/tests/helpers/docker.py
```

### Comparing `snowcross-0.4.0/LICENSE` & `snowcross-0.5.0/LICENSE`

 * *Files identical despite different names*

### Comparing `snowcross-0.4.0/PKG-INFO` & `snowcross-0.5.0/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: snowcross
-Version: 0.4.0
+Version: 0.5.0
 Summary: Adaptors for tools and services in a Snowflake-centric data platform
 Home-page: UNKNOWN
 License: Apache License 2.0
 Platform: UNKNOWN
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3 :: Only
 Classifier: Programming Language :: Python :: 3.10
```

### Comparing `snowcross-0.4.0/README.md` & `snowcross-0.5.0/README.md`

 * *Files identical despite different names*

### Comparing `snowcross-0.4.0/setup.py` & `snowcross-0.5.0/setup.py`

 * *Files identical despite different names*

### Comparing `snowcross-0.4.0/snowcross/aws.py` & `snowcross-0.5.0/snowcross/aws.py`

 * *Files 4% similar despite different names*

```diff
@@ -90,14 +90,42 @@
 
         for p in resp.get("Parameters", []):
             parameters[ssm_parameters[p["Name"]]] = p["Value"]
 
     return parameters
 
 
+def get_parameter(name: str) -> Optional[str]:
+    """Reads SSM parameter by name.
+
+    Args:
+        name (str): Parameter name.
+
+    Returns:
+        Optional[str]: Parameter value as string or none if not found.
+    """
+    try:
+        ssm = _client("ssm")
+        resp = ssm.get_parameter(Name=name, WithDecryption=True)
+        return resp["Parameter"]["Value"]
+    except ssm.exceptions.ParameterNotFound:
+        logger.error("Parameter %s not found", name)
+        return None
+
+
+def set_parameter(name: str, value: str):
+    """Writes SSM parameter.
+
+    Args:
+        name (str): Parameter name.
+        value (str): Parameter value.
+    """
+    _client("ssm").put_parameter(Name=name, Value=value, Overwrite=True)
+
+
 def environment_storage_bucket(environment: str, name: str) -> str:
     """Constructs environment-specific S3 bucket following convention.
 
     Args:
         environment (str): Environment name.
         name (str): Partial bucket name.
 
@@ -116,21 +144,20 @@
         bucket (str): Bucket name.
         key (str): Object key.
 
     Returns:
         Optional[botocore.response.StreamingBody]: An S3 object body stream or None.
     """
     try:
-        s3_object = _client("s3").get_object(Bucket=bucket, Key=key)
+        s3 = _client("s3")
+        s3_object = s3.get_object(Bucket=bucket, Key=key)
         return s3_object["Body"]
-    except botocore.client.ClientError as ex:
-        if ex.response["Error"]["Code"] == "NoSuchKey":
-            logger.info("Object %s not found - returning None", key)
-            return None
-        raise
+    except s3.exceptions.NoSuchKey:
+        logger.warning("Object %s not found", key)
+        return None
 
 
 def download_storage_object(bucket: str, key: str, filename: str):
     """Downloads S3 object to file.
 
     Args:
         bucket (str): Bucket name.
@@ -203,14 +230,24 @@
     parsed = urllib.parse.urlparse(url)
     if parsed.scheme in ("s3", "s3a"):
         obj["bucket"] = parsed.netloc
         obj["key"] = parsed.path.lstrip("/")
     return obj
 
 
+def format_storage_url(bucket: str, key: str) -> str:
+    """Generates S3 URL to bucket key (using s3:// schema).
+
+    Args:
+        bucket (str): Bucket name.
+        key (str): Object key.
+    """
+    return f"s3://{bucket}/{key}"
+
+
 def run_workflow(name: str, properties: Optional[Dict[str, str]] = None) -> str:
     """Executes workflow and return its run ID.
 
     Args:
         name (str): Workflow name.
         properties (Dict[str, str], optional): Run properties. Defaults to None.
```

### Comparing `snowcross-0.4.0/snowcross/errors.py` & `snowcross-0.5.0/snowcross/errors.py`

 * *Files identical despite different names*

### Comparing `snowcross-0.4.0/snowcross/locator.py` & `snowcross-0.5.0/snowcross/locator.py`

 * *Files identical despite different names*

### Comparing `snowcross-0.4.0/snowcross/snowflake.py` & `snowcross-0.5.0/snowcross/snowflake.py`

 * *Files identical despite different names*

### Comparing `snowcross-0.4.0/snowcross.egg-info/PKG-INFO` & `snowcross-0.5.0/snowcross.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: snowcross
-Version: 0.4.0
+Version: 0.5.0
 Summary: Adaptors for tools and services in a Snowflake-centric data platform
 Home-page: UNKNOWN
 License: Apache License 2.0
 Platform: UNKNOWN
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3 :: Only
 Classifier: Programming Language :: Python :: 3.10
```

### Comparing `snowcross-0.4.0/tests/fixtures/aws.py` & `snowcross-0.5.0/tests/fixtures/aws.py`

 * *Files identical despite different names*

### Comparing `snowcross-0.4.0/tests/fixtures/snowflake.py` & `snowcross-0.5.0/tests/fixtures/snowflake.py`

 * *Files identical despite different names*

### Comparing `snowcross-0.4.0/tests/helpers/docker.py` & `snowcross-0.5.0/tests/helpers/docker.py`

 * *Files identical despite different names*

