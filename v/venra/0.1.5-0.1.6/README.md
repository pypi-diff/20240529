# Comparing `tmp/venra-0.1.5.tar.gz` & `tmp/venra-0.1.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "venra-0.1.5.tar", last modified: Sat Aug 26 15:16:02 2023, max compression
+gzip compressed data, was "venra-0.1.6.tar", last modified: Wed May 29 20:06:09 2024, max compression
```

## Comparing `venra-0.1.5.tar` & `venra-0.1.6.tar`

### file list

```diff
@@ -1,22 +1,22 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-26 15:16:02.961942 venra-0.1.5/
--rw-r--r--   0 runner    (1001) docker     (123)     1079 2023-08-26 15:15:47.000000 venra-0.1.5/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)     3386 2023-08-26 15:16:02.961942 venra-0.1.5/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     2533 2023-08-26 15:15:47.000000 venra-0.1.5/README.md
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-08-26 15:16:02.961942 venra-0.1.5/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1201 2023-08-26 15:15:47.000000 venra-0.1.5/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-26 15:16:02.961942 venra-0.1.5/venra/
--rw-r--r--   0 runner    (1001) docker     (123)      983 2023-08-26 15:15:47.000000 venra-0.1.5/venra/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)       22 2023-08-26 15:15:47.000000 venra-0.1.5/venra/__version__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2486 2023-08-26 15:15:47.000000 venra-0.1.5/venra/client.py
--rw-r--r--   0 runner    (1001) docker     (123)     1233 2023-08-26 15:15:47.000000 venra-0.1.5/venra/config.py
--rw-r--r--   0 runner    (1001) docker     (123)     3817 2023-08-26 15:15:47.000000 venra-0.1.5/venra/document.py
--rw-r--r--   0 runner    (1001) docker     (123)      556 2023-08-26 15:15:47.000000 venra-0.1.5/venra/exceptions.py
--rw-r--r--   0 runner    (1001) docker     (123)     6113 2023-08-26 15:15:47.000000 venra-0.1.5/venra/query.py
--rw-r--r--   0 runner    (1001) docker     (123)     1935 2023-08-26 15:15:47.000000 venra-0.1.5/venra/system.py
--rw-r--r--   0 runner    (1001) docker     (123)     1957 2023-08-26 15:15:47.000000 venra-0.1.5/venra/visit.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-26 15:16:02.961942 venra-0.1.5/venra.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     3386 2023-08-26 15:16:02.000000 venra-0.1.5/venra.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      325 2023-08-26 15:16:02.000000 venra-0.1.5/venra.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-08-26 15:16:02.000000 venra-0.1.5/venra.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       19 2023-08-26 15:16:02.000000 venra-0.1.5/venra.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        6 2023-08-26 15:16:02.000000 venra-0.1.5/venra.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-29 20:06:09.636484 venra-0.1.6/
+-rw-r--r--   0 runner    (1001) docker     (127)     1079 2024-05-29 20:06:02.000000 venra-0.1.6/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)     3435 2024-05-29 20:06:09.636484 venra-0.1.6/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     2533 2024-05-29 20:06:02.000000 venra-0.1.6/README.md
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-29 20:06:09.636484 venra-0.1.6/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)     1201 2024-05-29 20:06:02.000000 venra-0.1.6/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-29 20:06:09.636484 venra-0.1.6/venra/
+-rw-r--r--   0 runner    (1001) docker     (127)      983 2024-05-29 20:06:02.000000 venra-0.1.6/venra/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)       22 2024-05-29 20:06:02.000000 venra-0.1.6/venra/__version__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2486 2024-05-29 20:06:02.000000 venra-0.1.6/venra/client.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1233 2024-05-29 20:06:02.000000 venra-0.1.6/venra/config.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4036 2024-05-29 20:06:02.000000 venra-0.1.6/venra/document.py
+-rw-r--r--   0 runner    (1001) docker     (127)      556 2024-05-29 20:06:02.000000 venra-0.1.6/venra/exceptions.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6130 2024-05-29 20:06:02.000000 venra-0.1.6/venra/query.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1950 2024-05-29 20:06:02.000000 venra-0.1.6/venra/system.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1972 2024-05-29 20:06:02.000000 venra-0.1.6/venra/visit.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-29 20:06:09.636484 venra-0.1.6/venra.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     3435 2024-05-29 20:06:09.000000 venra-0.1.6/venra.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      325 2024-05-29 20:06:09.000000 venra-0.1.6/venra.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-29 20:06:09.000000 venra-0.1.6/venra.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       19 2024-05-29 20:06:09.000000 venra-0.1.6/venra.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        6 2024-05-29 20:06:09.000000 venra-0.1.6/venra.egg-info/top_level.txt
```

### Comparing `venra-0.1.5/LICENSE` & `venra-0.1.6/LICENSE`

 * *Files identical despite different names*

### Comparing `venra-0.1.5/PKG-INFO` & `venra-0.1.6/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: venra
-Version: 0.1.5
+Version: 0.1.6
 Summary: Venra provides a simple, high-level api for vespa.ai.
 Home-page: https://github.com/codycollier/venra
 Author: Cody Collier
 Author-email: cody@telnet.org
 License: MIT
 Keywords: artificial intelligence,information retrieval,machine learning,search
 Classifier: Development Status :: 4 - Beta
@@ -15,14 +15,16 @@
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Requires-Python: >=3.8, <4
 Description-Content-Type: text/markdown
 License-File: LICENSE
+Requires-Dist: packaging
+Requires-Dist: requests
 
 ## venra
 
 [![Project Status: WIP](https://www.repostatus.org/badges/latest/wip.svg)](https://www.repostatus.org/#wip)
 ![Tests](https://github.com/codycollier/venra/workflows/Tests/badge.svg)
 ![Release](https://github.com/codycollier/venra/workflows/Python%20Package%20Release/badge.svg)
 [![PyPI version](https://badge.fury.io/py/venra.svg)](https://badge.fury.io/py/venra)
```

### Comparing `venra-0.1.5/README.md` & `venra-0.1.6/README.md`

 * *Files identical despite different names*

### Comparing `venra-0.1.5/setup.py` & `venra-0.1.6/setup.py`

 * *Files identical despite different names*

### Comparing `venra-0.1.5/venra/__init__.py` & `venra-0.1.6/venra/__init__.py`

 * *Files identical despite different names*

### Comparing `venra-0.1.5/venra/client.py` & `venra-0.1.6/venra/client.py`

 * *Files identical despite different names*

### Comparing `venra-0.1.5/venra/config.py` & `venra-0.1.6/venra/config.py`

 * *Files identical despite different names*

### Comparing `venra-0.1.5/venra/document.py` & `venra-0.1.6/venra/document.py`

 * *Files 12% similar despite different names*

```diff
@@ -35,67 +35,67 @@
         err = f"unexpected response\n"
         err += f"  response code: {response.status_code}\n"
         err += f"  response  url: {response.url}\n"
         err += f"  response body: {response.text}\n"
         raise exceptions.VespaRequestError(err)
 
 
-def _vespa_get(namespace, doctype, docid, fieldset="all"):
+def _vespa_http_get(namespace, doctype, docid, fieldset="all"):
     """Internal wrapper for document api and http get handling"""
     base_uri = f"{config.vespa_host_app}/document/v1/{namespace}/{doctype}/docid/{docid}?fieldSet=[{fieldset}]"
     vc = client.get_vespa_client()
     vr = vc.get(f"{base_uri}")
     _api_err_check(vr)
     vr = vr.json()
     return vr
 
 
-def _vespa_post(namespace, doctype, docid, doc):
+def _vespa_http_post(namespace, doctype, docid, doc):
     """Internal wrapper for document api and http post handling"""
     base_uri = f"{config.vespa_host_app}/document/v1/{namespace}/{doctype}/docid/{docid}"
     vc = client.get_vespa_client()
     vr = vc.post(f"{base_uri}", json=doc)
     _api_err_check(vr)
     return
 
 
-def _vespa_put(namespace, doctype, docid, update):
+def _vespa_http_put(namespace, doctype, docid, update):
     """Internal wrapper for document api and http put handling"""
     base_uri = f"{config.vespa_host_app}/document/v1/{namespace}/{doctype}/docid/{docid}"
     vc = client.get_vespa_client()
     vr = vc.put(f"{base_uri}", json=update)
     _api_err_check(vr)
     return
 
 
-def _vespa_delete(namespace, doctype, docid):
+def _vespa_http_delete(namespace, doctype, docid):
     """Internal wrapper for document api and http delete handling"""
     base_uri = f"{config.vespa_host_app}/document/v1/{namespace}/{doctype}/docid/{docid}"
     vc = client.get_vespa_client()
     vr = vc.delete(f"{base_uri}")
     _api_err_check(vr)
     return
 
 
 def get(namespace, doctype, docid, fieldset="all", fields_only=True):
     """Retrieve and return a document"""
-    doc = _vespa_get(namespace, doctype, docid, fieldset)
+    doc = _vespa_http_get(namespace, doctype, docid, fieldset)
     if fields_only:
         doc = doc["fields"]
     return doc
 
 
 def put(namespace, doctype, docid, doc):
     """Add or update a whole document"""
     doc_fields = {"fields": doc}
-    _vespa_post(namespace, doctype, docid, doc_fields)
+    _vespa_http_post(namespace, doctype, docid, doc_fields)
     return True
 
 
-def update(namespace, doctype, docid, operations):
+def update(namespace, doctype, docid, operations, condition=False, create=False):
     """Apply a partial update using the assign, add, or remove operator
 
     operations = [("assign", "field_name_here", "field_value_here"), ...]
 
     reference:
     * https://docs.vespa.ai/en/reference/document-json-format.html
 
@@ -104,20 +104,25 @@
     {
         "update": "id:mynamespace:food::example",
         "fields": {
             "my_food_scores{Strawberries}": { "assign": "Delicious!" }
         }
     }
     """
-    partial_update = {"fields": {}}
+    partial_update = {}
+    if create:
+        partial_update["create"] = True
+    if condition:
+        partial_update["condition"] = f"{condition}"
+    partial_update["fields"] = {}
     for operation, field_name, field_value in operations:
         partial_update["fields"][field_name] = {operation: field_value}
-    _vespa_put(namespace, doctype, docid, partial_update)
+    _vespa_http_put(namespace, doctype, docid, partial_update)
     return True
 
 
 def remove(namespace, doctype, docid):
     """Delete a document"""
-    _vespa_delete(namespace, doctype, docid)
+    _vespa_http_delete(namespace, doctype, docid)
     return True
```

### Comparing `venra-0.1.5/venra/exceptions.py` & `venra-0.1.6/venra/exceptions.py`

 * *Files identical despite different names*

### Comparing `venra-0.1.5/venra/query.py` & `venra-0.1.6/venra/query.py`

 * *Files 2% similar despite different names*

```diff
@@ -30,15 +30,15 @@
         err = f"unexpected response\n"
         err += f"  response code: {response.status_code}\n"
         err += f"  response  url: {response.url}\n"
         err += f"  response body: {response.text}\n"
         raise exceptions.VespaRequestError(err)
 
 
-def _vespa_post(qdata):
+def _vespa_http_post(qdata):
     """Internal wrapper for search api http call handling"""
     base_uri = f"{config.vespa_host_app}/search/"
     vc = client.get_vespa_client()
     vr = vc.post(f"{base_uri}", json=qdata)
     _api_err_check(vr)
     vr = vr.json()
     return vr
@@ -46,15 +46,15 @@
 
 def search(qdata):
     """Run a search with the given parameters and return the complete results
 
     The return val is the complete query response json loaded as a dictionary
     """
     qstarted = time.time()
-    qresults = _vespa_post(qdata)
+    qresults = _vespa_http_post(qdata)
     qstopped = time.time()
     elapsed = qstopped - qstarted
     qresults["venra"] = {"elapsed_ms": elapsed}
     return qresults
 
 
 def extract_metrics(qresults):
@@ -200,13 +200,13 @@
             yield d
 
         # stop if we reached the end of the results
         if doc_count >= total_results:
             break
 
         # get next page of results
-        qdata["offset"] += 1
+        qdata["offset"] = doc_count
         qresults = search(qdata)
 
     return
```

### Comparing `venra-0.1.5/venra/system.py` & `venra-0.1.6/venra/system.py`

 * *Files 5% similar despite different names*

```diff
@@ -32,15 +32,15 @@
         err = f"unexpected response\n"
         err += f"  response code: {response.status_code}\n"
         err += f"  response  url: {response.url}\n"
         err += f"  response body: {response.text}\n"
         raise exceptions.VespaRequestError(err)
 
 
-def _vespa_get(full_uri):
+def _vespa_http_get(full_uri):
     """Internal wrapper for system api http call handling"""
     vc = client.get_vespa_client()
     vr = vc.get(f"{full_uri}")
     _api_err_check(vr)
     vr = vr.json()
     return vr
 
@@ -50,24 +50,24 @@
 
     example:
     $ curl -s http://127.0.0.1:8080/state/v1/version | jq .
     {
         "version": "8.13.21"
     }
     """
-    vr = _vespa_get(f"{config.vespa_host_app}/state/v1/version")
+    vr = _vespa_http_get(f"{config.vespa_host_app}/state/v1/version")
     return vr["version"]
 
 
 def version_cfg():
     """Return the version string from the app server
 
     example:
     $ curl -s http://127.0.0.1:19071/state/v1/version | jq .
     {
         "version": "8.13.21"
     }
     """
-    vr = _vespa_get(f"{config.vespa_host_cfg}/state/v1/version")
+    vr = _vespa_http_get(f"{config.vespa_host_cfg}/state/v1/version")
     return vr["version"]
```

### Comparing `venra-0.1.5/venra/visit.py` & `venra-0.1.6/venra/visit.py`

 * *Files 2% similar despite different names*

```diff
@@ -20,15 +20,15 @@
     """Error handling for http responses unique to the visit api"""
 
     if response.status_code != 200:
         err = f"unexpected response {response.status_code} {response.url}"
         raise exceptions.VespaRequestError(err)
 
 
-def _vespa_get(namespace, doctype, selection=None, continuation=None):
+def _vespa_http_get(namespace, doctype, selection=None, continuation=None):
     """Internal wrapper for visit api http call handling"""
     base_uri = f"{config.vespa_host_app}/document/v1/{namespace}/{doctype}/docid"
 
     vc = client.get_vespa_client()
 
     if not selection and not continuation:
         vr = vc.get(f"{base_uri}")
@@ -50,15 +50,15 @@
 
 def feed(namespace, doctype, selection=None, fields_only=True):
     """Yield all docs of a given type and selection
 
     """
 
     # initial call
-    vr = _vespa_get(namespace, doctype, selection, None)
+    vr = _vespa_http_get(namespace, doctype, selection, None)
 
     # page through results
     while True:
 
         # yield each doc from the results
         for d in vr.get("documents", []):
             if fields_only:
@@ -67,11 +67,11 @@
 
         # check for continuation / more results
         continuation = vr.get("continuation", False)
         if not continuation:
             break
 
         # retrieve the next set of results
-        vr = _vespa_get(namespace, doctype, selection, continuation)
+        vr = _vespa_http_get(namespace, doctype, selection, continuation)
 
     return
```

### Comparing `venra-0.1.5/venra.egg-info/PKG-INFO` & `venra-0.1.6/venra.egg-info/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: venra
-Version: 0.1.5
+Version: 0.1.6
 Summary: Venra provides a simple, high-level api for vespa.ai.
 Home-page: https://github.com/codycollier/venra
 Author: Cody Collier
 Author-email: cody@telnet.org
 License: MIT
 Keywords: artificial intelligence,information retrieval,machine learning,search
 Classifier: Development Status :: 4 - Beta
@@ -15,14 +15,16 @@
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Requires-Python: >=3.8, <4
 Description-Content-Type: text/markdown
 License-File: LICENSE
+Requires-Dist: packaging
+Requires-Dist: requests
 
 ## venra
 
 [![Project Status: WIP](https://www.repostatus.org/badges/latest/wip.svg)](https://www.repostatus.org/#wip)
 ![Tests](https://github.com/codycollier/venra/workflows/Tests/badge.svg)
 ![Release](https://github.com/codycollier/venra/workflows/Python%20Package%20Release/badge.svg)
 [![PyPI version](https://badge.fury.io/py/venra.svg)](https://badge.fury.io/py/venra)
```

