# Comparing `tmp/aiorobonect-1.0.5.tar.gz` & `tmp/aiorobonect-1.0.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "aiorobonect-1.0.5.tar", last modified: Tue May 28 09:42:00 2024, max compression
+gzip compressed data, was "aiorobonect-1.0.6.tar", last modified: Tue May 28 12:54:06 2024, max compression
```

## Comparing `aiorobonect-1.0.5.tar` & `aiorobonect-1.0.6.tar`

### file list

```diff
@@ -1,17 +1,17 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-28 09:42:00.758483 aiorobonect-1.0.5/
--rw-r--r--   0 runner    (1001) docker     (127)     1071 2024-05-28 09:41:40.000000 aiorobonect-1.0.5/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)     3590 2024-05-28 09:42:00.758483 aiorobonect-1.0.5/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     3133 2024-05-28 09:41:40.000000 aiorobonect-1.0.5/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-28 09:42:00.754483 aiorobonect-1.0.5/aiorobonect/
--rw-r--r--   0 runner    (1001) docker     (127)       74 2024-05-28 09:41:40.000000 aiorobonect-1.0.5/aiorobonect/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     6061 2024-05-28 09:41:40.000000 aiorobonect-1.0.5/aiorobonect/client.py
--rw-r--r--   0 runner    (1001) docker     (127)       51 2024-05-28 09:41:40.000000 aiorobonect-1.0.5/aiorobonect/const.py
--rw-r--r--   0 runner    (1001) docker     (127)      406 2024-05-28 09:41:40.000000 aiorobonect-1.0.5/aiorobonect/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-28 09:42:00.758483 aiorobonect-1.0.5/aiorobonect.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     3590 2024-05-28 09:42:00.000000 aiorobonect-1.0.5/aiorobonect.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      298 2024-05-28 09:42:00.000000 aiorobonect-1.0.5/aiorobonect.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-28 09:42:00.000000 aiorobonect-1.0.5/aiorobonect.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       37 2024-05-28 09:42:00.000000 aiorobonect-1.0.5/aiorobonect.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       12 2024-05-28 09:42:00.000000 aiorobonect-1.0.5/aiorobonect.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)      891 2024-05-28 09:42:00.758483 aiorobonect-1.0.5/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)      776 2024-05-28 09:41:42.000000 aiorobonect-1.0.5/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-28 12:54:06.983022 aiorobonect-1.0.6/
+-rw-r--r--   0 runner    (1001) docker     (127)     1071 2024-05-28 12:53:43.000000 aiorobonect-1.0.6/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)     3590 2024-05-28 12:54:06.983022 aiorobonect-1.0.6/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     3133 2024-05-28 12:53:43.000000 aiorobonect-1.0.6/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-28 12:54:06.983022 aiorobonect-1.0.6/aiorobonect/
+-rw-r--r--   0 runner    (1001) docker     (127)       74 2024-05-28 12:53:43.000000 aiorobonect-1.0.6/aiorobonect/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6331 2024-05-28 12:53:43.000000 aiorobonect-1.0.6/aiorobonect/client.py
+-rw-r--r--   0 runner    (1001) docker     (127)       51 2024-05-28 12:53:43.000000 aiorobonect-1.0.6/aiorobonect/const.py
+-rw-r--r--   0 runner    (1001) docker     (127)      406 2024-05-28 12:53:43.000000 aiorobonect-1.0.6/aiorobonect/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-28 12:54:06.983022 aiorobonect-1.0.6/aiorobonect.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     3590 2024-05-28 12:54:06.000000 aiorobonect-1.0.6/aiorobonect.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      298 2024-05-28 12:54:06.000000 aiorobonect-1.0.6/aiorobonect.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-28 12:54:06.000000 aiorobonect-1.0.6/aiorobonect.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       37 2024-05-28 12:54:06.000000 aiorobonect-1.0.6/aiorobonect.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       12 2024-05-28 12:54:06.000000 aiorobonect-1.0.6/aiorobonect.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      891 2024-05-28 12:54:06.983022 aiorobonect-1.0.6/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)      776 2024-05-28 12:53:46.000000 aiorobonect-1.0.6/setup.py
```

### Comparing `aiorobonect-1.0.5/LICENSE` & `aiorobonect-1.0.6/LICENSE`

 * *Files identical despite different names*

### Comparing `aiorobonect-1.0.5/PKG-INFO` & `aiorobonect-1.0.6/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: aiorobonect
-Version: 1.0.5
+Version: 1.0.6
 Summary: Module to communicate to the Robonect API
 Home-page: https://github.com/geertmeersman/aiorobonect
 Author: Geert Meersman
 Author-email: geertmeersman@gmail.com
 License: MIT
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: Apache Software License
```

### Comparing `aiorobonect-1.0.5/README.md` & `aiorobonect-1.0.6/README.md`

 * *Files identical despite different names*

### Comparing `aiorobonect-1.0.5/aiorobonect/client.py` & `aiorobonect-1.0.6/aiorobonect/client.py`

 * *Files 3% similar despite different names*

```diff
@@ -94,14 +94,15 @@
         def create_url(scheme):
             return f"{scheme}://{self.host}/json?cmd={command}&{params}"
 
         if self.scheme is None:
             self.scheme = ["http", "https"]
 
         response = None
+        last_exception = None
 
         for scheme in self.scheme:
             url = create_url(scheme)
             _LOGGER.debug(f"Calling {url}")
             try:
                 response = await self.client.get(url)
                 if response.status_code == 200 or response.status_code >= 400:
@@ -110,17 +111,24 @@
                 elif 300 <= response.status_code < 400:
                     _LOGGER.debug(
                         f"Received redirect status code {response.status_code}, continuing to next scheme"
                     )
                     continue  # Continue loop on redirect (3xx)
             except httpx.RequestError as e:
                 _LOGGER.warning(
-                    f"Failed to connect using {scheme}://{self.host} - HTTP STATUS {response.status_code}, {e}"
+                    f"Failed to connect using {scheme}://{self.host}, error: {e}"
                 )
+                last_exception = e
                 continue  # Continue to the next scheme on connection error
+                continue  # Continue to the next scheme on connection error
+
+        if response is None:
+            raise last_exception or httpx.RequestError(
+                "Failed to get a response from the mower."
+            )
 
         if response and response.status_code == 200:
             result_text = response.text
             _LOGGER.debug(f"Rest API call result for {command}: {result_text}")
             result_json = json.loads(result_text)
             result_json["sync_time"] = datetime.now()
         elif response and response.status_code >= 400:
```

### Comparing `aiorobonect-1.0.5/aiorobonect.egg-info/PKG-INFO` & `aiorobonect-1.0.6/aiorobonect.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: aiorobonect
-Version: 1.0.5
+Version: 1.0.6
 Summary: Module to communicate to the Robonect API
 Home-page: https://github.com/geertmeersman/aiorobonect
 Author: Geert Meersman
 Author-email: geertmeersman@gmail.com
 License: MIT
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: Apache Software License
```

### Comparing `aiorobonect-1.0.5/setup.cfg` & `aiorobonect-1.0.6/setup.cfg`

 * *Files identical despite different names*

### Comparing `aiorobonect-1.0.5/setup.py` & `aiorobonect-1.0.6/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -17,9 +17,9 @@
     packages=setuptools.find_packages(),
     classifiers=[
         "Programming Language :: Python :: 3",
         "License :: OSI Approved :: Apache Software License",
         "Operating System :: OS Independent",
     ],
     install_requires=[val.strip() for val in open("requirements.txt")],
-    version="v1.0.5",
+    version="v1.0.6",
 )
```

