# Comparing `tmp/pyanglianwater-0.3.0.tar.gz` & `tmp/pyanglianwater-0.3.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pyanglianwater-0.3.0.tar", last modified: Wed May  1 18:39:27 2024, max compression
+gzip compressed data, was "pyanglianwater-0.3.1.tar", last modified: Wed May 29 10:33:29 2024, max compression
```

## Comparing `pyanglianwater-0.3.0.tar` & `pyanglianwater-0.3.1.tar`

### file list

```diff
@@ -1,21 +1,21 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-01 18:39:27.963887 pyanglianwater-0.3.0/
--rw-r--r--   0 runner    (1001) docker     (127)     1071 2024-05-01 18:39:03.000000 pyanglianwater-0.3.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)     1796 2024-05-01 18:39:27.963887 pyanglianwater-0.3.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      950 2024-05-01 18:39:03.000000 pyanglianwater-0.3.0/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-01 18:39:27.959887 pyanglianwater-0.3.0/pyanglianwater/
--rw-r--r--   0 runner    (1001) docker     (127)     4453 2024-05-01 18:39:03.000000 pyanglianwater-0.3.0/pyanglianwater/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)       22 2024-05-01 18:39:03.000000 pyanglianwater-0.3.0/pyanglianwater/_version.py
--rw-r--r--   0 runner    (1001) docker     (127)     6998 2024-05-01 18:39:03.000000 pyanglianwater-0.3.0/pyanglianwater/api.py
--rw-r--r--   0 runner    (1001) docker     (127)     1020 2024-05-01 18:39:03.000000 pyanglianwater-0.3.0/pyanglianwater/const.py
--rw-r--r--   0 runner    (1001) docker     (127)      162 2024-05-01 18:39:03.000000 pyanglianwater-0.3.0/pyanglianwater/enum.py
--rw-r--r--   0 runner    (1001) docker     (127)      700 2024-05-01 18:39:03.000000 pyanglianwater-0.3.0/pyanglianwater/exceptions.py
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-01 18:39:03.000000 pyanglianwater-0.3.0/pyanglianwater/py.typed
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-01 18:39:27.959887 pyanglianwater-0.3.0/pyanglianwater.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     1796 2024-05-01 18:39:27.000000 pyanglianwater-0.3.0/pyanglianwater.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      406 2024-05-01 18:39:27.000000 pyanglianwater-0.3.0/pyanglianwater.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-01 18:39:27.000000 pyanglianwater-0.3.0/pyanglianwater.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)      120 2024-05-01 18:39:27.000000 pyanglianwater-0.3.0/pyanglianwater.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       15 2024-05-01 18:39:27.000000 pyanglianwater-0.3.0/pyanglianwater.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)      111 2024-05-01 18:39:03.000000 pyanglianwater-0.3.0/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-01 18:39:27.963887 pyanglianwater-0.3.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)     1514 2024-05-01 18:39:03.000000 pyanglianwater-0.3.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-29 10:33:29.950772 pyanglianwater-0.3.1/
+-rw-r--r--   0 runner    (1001) docker     (127)     1071 2024-05-29 10:33:08.000000 pyanglianwater-0.3.1/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)     1796 2024-05-29 10:33:29.950772 pyanglianwater-0.3.1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      950 2024-05-29 10:33:08.000000 pyanglianwater-0.3.1/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-29 10:33:29.950772 pyanglianwater-0.3.1/pyanglianwater/
+-rw-r--r--   0 runner    (1001) docker     (127)     4453 2024-05-29 10:33:08.000000 pyanglianwater-0.3.1/pyanglianwater/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)       22 2024-05-29 10:33:08.000000 pyanglianwater-0.3.1/pyanglianwater/_version.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6998 2024-05-29 10:33:08.000000 pyanglianwater-0.3.1/pyanglianwater/api.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1020 2024-05-29 10:33:08.000000 pyanglianwater-0.3.1/pyanglianwater/const.py
+-rw-r--r--   0 runner    (1001) docker     (127)      162 2024-05-29 10:33:08.000000 pyanglianwater-0.3.1/pyanglianwater/enum.py
+-rw-r--r--   0 runner    (1001) docker     (127)      700 2024-05-29 10:33:08.000000 pyanglianwater-0.3.1/pyanglianwater/exceptions.py
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-29 10:33:08.000000 pyanglianwater-0.3.1/pyanglianwater/py.typed
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-29 10:33:29.950772 pyanglianwater-0.3.1/pyanglianwater.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     1796 2024-05-29 10:33:29.000000 pyanglianwater-0.3.1/pyanglianwater.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      406 2024-05-29 10:33:29.000000 pyanglianwater-0.3.1/pyanglianwater.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-29 10:33:29.000000 pyanglianwater-0.3.1/pyanglianwater.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      120 2024-05-29 10:33:29.000000 pyanglianwater-0.3.1/pyanglianwater.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       15 2024-05-29 10:33:29.000000 pyanglianwater-0.3.1/pyanglianwater.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      111 2024-05-29 10:33:08.000000 pyanglianwater-0.3.1/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-29 10:33:29.950772 pyanglianwater-0.3.1/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)     1514 2024-05-29 10:33:08.000000 pyanglianwater-0.3.1/setup.py
```

### Comparing `pyanglianwater-0.3.0/LICENSE` & `pyanglianwater-0.3.1/LICENSE`

 * *Files identical despite different names*

### Comparing `pyanglianwater-0.3.0/PKG-INFO` & `pyanglianwater-0.3.1/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pyanglianwater
-Version: 0.3.0
+Version: 0.3.1
 Summary: A package to interact with Anglian Water
 Home-page: http://github.com/pantherale0/pyanglianwater
 Author: pantherale0
 License: MIT
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

### Comparing `pyanglianwater-0.3.0/README.md` & `pyanglianwater-0.3.1/README.md`

 * *Files identical despite different names*

### Comparing `pyanglianwater-0.3.0/pyanglianwater/__init__.py` & `pyanglianwater-0.3.1/pyanglianwater/__init__.py`

 * *Files identical despite different names*

### Comparing `pyanglianwater-0.3.0/pyanglianwater/api.py` & `pyanglianwater-0.3.1/pyanglianwater/api.py`

 * *Ordering differences only*

 * *Files 0% similar despite different names*

```diff
@@ -163,24 +163,24 @@
             async with _session.request(
                 method=endpoint_map["method"],
                 url=API_BASEURL + endpoint_map["endpoint"],
                 headers=headers,
                 json=body
             ) as _response:
                 if not _response.ok:
-                    _LOGGER.error(">> Error sending request %s to Anglian Water (%s) - %s",
-                                  endpoint,
-                                  _response.status,
-                                  await _response.text())
                     if _response.status == 401:
                         self.access_token = None
                         raise ExpiredAccessTokenError()
                     if _response.status == 503:
                         self.access_token = None
                         raise ServiceUnavailableError()
+                    _LOGGER.error(">> Error sending request %s to Anglian Water (%s) - %s",
+                                  endpoint,
+                                  _response.status,
+                                  await _response.text())
                 # Check StatusCode in response body.
                 resp_body = await _response.json()
                 if resp_body["StatusCode"] == "0":
                     # Successful request
                     _LOGGER.debug(">> Request to %s successful.", endpoint)
                     return resp_body
                 if resp_body["StatusCode"] in API_RESPONSE_STATUS_CODE_MAPPING:
```

### Comparing `pyanglianwater-0.3.0/pyanglianwater/const.py` & `pyanglianwater-0.3.1/pyanglianwater/const.py`

 * *Files identical despite different names*

### Comparing `pyanglianwater-0.3.0/pyanglianwater/exceptions.py` & `pyanglianwater-0.3.1/pyanglianwater/exceptions.py`

 * *Files identical despite different names*

### Comparing `pyanglianwater-0.3.0/pyanglianwater.egg-info/PKG-INFO` & `pyanglianwater-0.3.1/pyanglianwater.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pyanglianwater
-Version: 0.3.0
+Version: 0.3.1
 Summary: A package to interact with Anglian Water
 Home-page: http://github.com/pantherale0/pyanglianwater
 Author: pantherale0
 License: MIT
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

### Comparing `pyanglianwater-0.3.0/setup.py` & `pyanglianwater-0.3.1/setup.py`

 * *Files identical despite different names*

