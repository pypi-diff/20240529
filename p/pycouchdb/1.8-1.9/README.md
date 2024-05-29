# Comparing `tmp/pycouchdb-1.8.tar.gz` & `tmp/pycouchdb-1.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/pycouchdb-1.8.tar", last modified: Thu Jul 17 19:52:15 2014, max compression
+gzip compressed data, was "dist/pycouchdb-1.9.tar", last modified: Sat Aug 23 10:28:56 2014, max compression
```

## Comparing `pycouchdb-1.8.tar` & `pycouchdb-1.9.tar`

### file list

```diff
@@ -1,21 +1,21 @@
-drwxr-xr-x   0 niwi      (1000) users      (100)        0 2014-07-17 19:52:15.000000 pycouchdb-1.8/
-drwxr-xr-x   0 niwi      (1000) users      (100)        0 2014-07-17 19:52:15.000000 pycouchdb-1.8/pycouchdb/
--rw-r--r--   0 niwi      (1000) users      (100)       54 2013-12-15 10:39:36.000000 pycouchdb-1.8/pycouchdb/__init__.py
--rw-r--r--   0 niwi      (1000) users      (100)    21806 2014-07-04 23:57:16.000000 pycouchdb-1.8/pycouchdb/client.py
--rw-r--r--   0 niwi      (1000) users      (100)      371 2013-12-15 10:39:36.000000 pycouchdb-1.8/pycouchdb/exceptions.py
--rw-r--r--   0 niwi      (1000) users      (100)      978 2013-12-15 10:39:36.000000 pycouchdb-1.8/pycouchdb/feedreader.py
--rw-r--r--   0 niwi      (1000) users      (100)     4003 2014-07-04 23:57:16.000000 pycouchdb-1.8/pycouchdb/resource.py
--rw-r--r--   0 niwi      (1000) users      (100)     3882 2014-07-17 19:40:53.000000 pycouchdb-1.8/pycouchdb/utils.py
--rwxr-xr-x   0 niwi      (1000) users      (100)     6797 2013-12-15 10:39:36.000000 pycouchdb-1.8/pycouchdb/view.py
-drwxr-xr-x   0 niwi      (1000) users      (100)        0 2014-07-17 19:52:15.000000 pycouchdb-1.8/pycouchdb.egg-info/
--rw-r--r--   0 niwi      (1000) users      (100)      804 2014-07-17 19:52:15.000000 pycouchdb-1.8/pycouchdb.egg-info/PKG-INFO
--rw-r--r--   0 niwi      (1000) users      (100)      400 2014-07-17 19:52:15.000000 pycouchdb-1.8/pycouchdb.egg-info/SOURCES.txt
--rw-r--r--   0 niwi      (1000) users      (100)        1 2014-07-17 19:52:15.000000 pycouchdb-1.8/pycouchdb.egg-info/dependency_links.txt
--rw-r--r--   0 niwi      (1000) users      (100)       49 2014-07-17 19:52:15.000000 pycouchdb-1.8/pycouchdb.egg-info/entry_points.txt
--rw-r--r--   0 niwi      (1000) users      (100)        1 2013-12-15 10:47:44.000000 pycouchdb-1.8/pycouchdb.egg-info/not-zip-safe
--rw-r--r--   0 niwi      (1000) users      (100)        9 2014-07-17 19:52:15.000000 pycouchdb-1.8/pycouchdb.egg-info/requires.txt
--rw-r--r--   0 niwi      (1000) users      (100)       10 2014-07-17 19:52:15.000000 pycouchdb-1.8/pycouchdb.egg-info/top_level.txt
--rw-r--r--   0 niwi      (1000) users      (100)     1377 2014-07-05 00:10:07.000000 pycouchdb-1.8/README.rst
--rw-r--r--   0 niwi      (1000) users      (100)     1395 2014-07-17 19:51:12.000000 pycouchdb-1.8/setup.py
--rw-r--r--   0 niwi      (1000) users      (100)      804 2014-07-17 19:52:15.000000 pycouchdb-1.8/PKG-INFO
--rw-r--r--   0 niwi      (1000) users      (100)       59 2014-07-17 19:52:15.000000 pycouchdb-1.8/setup.cfg
+drwxr-xr-x   0 niwi      (1000) users      (100)        0 2014-08-23 10:28:56.000000 pycouchdb-1.9/
+drwxr-xr-x   0 niwi      (1000) users      (100)        0 2014-08-23 10:28:56.000000 pycouchdb-1.9/pycouchdb/
+-rw-r--r--   0 niwi      (1000) users      (100)       54 2013-12-15 10:39:36.000000 pycouchdb-1.9/pycouchdb/__init__.py
+-rw-r--r--   0 niwi      (1000) users      (100)    22146 2014-08-23 10:26:07.000000 pycouchdb-1.9/pycouchdb/client.py
+-rw-r--r--   0 niwi      (1000) users      (100)      371 2013-12-15 10:39:36.000000 pycouchdb-1.9/pycouchdb/exceptions.py
+-rw-r--r--   0 niwi      (1000) users      (100)      978 2013-12-15 10:39:36.000000 pycouchdb-1.9/pycouchdb/feedreader.py
+-rw-r--r--   0 niwi      (1000) users      (100)     4003 2014-08-23 10:26:07.000000 pycouchdb-1.9/pycouchdb/resource.py
+-rw-r--r--   0 niwi      (1000) users      (100)     3882 2014-08-23 10:26:07.000000 pycouchdb-1.9/pycouchdb/utils.py
+-rwxr-xr-x   0 niwi      (1000) users      (100)     6797 2013-12-15 10:39:36.000000 pycouchdb-1.9/pycouchdb/view.py
+drwxr-xr-x   0 niwi      (1000) users      (100)        0 2014-08-23 10:28:56.000000 pycouchdb-1.9/pycouchdb.egg-info/
+-rw-r--r--   0 niwi      (1000) users      (100)      804 2014-08-23 10:28:56.000000 pycouchdb-1.9/pycouchdb.egg-info/PKG-INFO
+-rw-r--r--   0 niwi      (1000) users      (100)      400 2014-08-23 10:28:56.000000 pycouchdb-1.9/pycouchdb.egg-info/SOURCES.txt
+-rw-r--r--   0 niwi      (1000) users      (100)        1 2014-08-23 10:28:56.000000 pycouchdb-1.9/pycouchdb.egg-info/dependency_links.txt
+-rw-r--r--   0 niwi      (1000) users      (100)       49 2014-08-23 10:28:56.000000 pycouchdb-1.9/pycouchdb.egg-info/entry_points.txt
+-rw-r--r--   0 niwi      (1000) users      (100)        1 2013-12-15 10:47:44.000000 pycouchdb-1.9/pycouchdb.egg-info/not-zip-safe
+-rw-r--r--   0 niwi      (1000) users      (100)        9 2014-08-23 10:28:56.000000 pycouchdb-1.9/pycouchdb.egg-info/requires.txt
+-rw-r--r--   0 niwi      (1000) users      (100)       10 2014-08-23 10:28:56.000000 pycouchdb-1.9/pycouchdb.egg-info/top_level.txt
+-rw-r--r--   0 niwi      (1000) users      (100)     1377 2014-08-23 10:26:07.000000 pycouchdb-1.9/README.rst
+-rw-r--r--   0 niwi      (1000) users      (100)     1292 2014-08-23 10:27:53.000000 pycouchdb-1.9/setup.py
+-rw-r--r--   0 niwi      (1000) users      (100)      804 2014-08-23 10:28:56.000000 pycouchdb-1.9/PKG-INFO
+-rw-r--r--   0 niwi      (1000) users      (100)       59 2014-08-23 10:28:56.000000 pycouchdb-1.9/setup.cfg
```

### Comparing `pycouchdb-1.8/pycouchdb/client.py` & `pycouchdb-1.9/pycouchdb/client.py`

 * *Files 2% similar despite different names*

```diff
@@ -385,14 +385,24 @@
         if flat is not None:
             wrapper = lambda doc: doc[flat]
 
         def _iterate():
             for row in result["rows"]:
                 yield wrapper(row['doc'])
 
+        def _iterate_no_docs():
+            for row in result["rows"]:
+                doc = {"id": row['id'], "rev": row['value']['rev']}
+                yield wrapper(doc)
+
+        if params["include_docs"].upper() == "FALSE":
+            if as_list:
+                return list(_iterate_no_docs())
+            return _iterate_no_docs()
+
         if as_list:
             return list(_iterate())
         return _iterate()
 
     def cleanup(self):
         """
         Execute a cleanup operation.
```

### Comparing `pycouchdb-1.8/pycouchdb/feedreader.py` & `pycouchdb-1.9/pycouchdb/feedreader.py`

 * *Files identical despite different names*

### Comparing `pycouchdb-1.8/pycouchdb/resource.py` & `pycouchdb-1.9/pycouchdb/resource.py`

 * *Files identical despite different names*

### Comparing `pycouchdb-1.8/pycouchdb/utils.py` & `pycouchdb-1.9/pycouchdb/utils.py`

 * *Files identical despite different names*

### Comparing `pycouchdb-1.8/pycouchdb/view.py` & `pycouchdb-1.9/pycouchdb/view.py`

 * *Files identical despite different names*

### Comparing `pycouchdb-1.8/pycouchdb.egg-info/PKG-INFO` & `pycouchdb-1.9/pycouchdb.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 1.1
 Name: pycouchdb
-Version: 1.8
+Version: 1.9
 Summary: Modern pure python CouchDB Client.
 Home-page: https://github.com/niwibe/py-couchdb
 Author: Andrey Antukh
 Author-email: niwi@niwi.be
 License: UNKNOWN
 Description: UNKNOWN
 Platform: UNKNOWN
```

### Comparing `pycouchdb-1.8/README.rst` & `pycouchdb-1.9/README.rst`

 * *Files identical despite different names*

### Comparing `pycouchdb-1.8/setup.py` & `pycouchdb-1.9/setup.py`

 * *Files 8% similar despite different names*

```diff
@@ -8,25 +8,23 @@
     from distutils.command.build_py import build_py
 
 setup(
     name = "pycouchdb",
     url = "https://github.com/niwibe/py-couchdb",
     author = "Andrey Antukh",
     author_email = "niwi@niwi.be",
-    version="1.8",
+    version="1.9",
     packages = [
         "pycouchdb",
     ],
     description = description.strip(),
     zip_safe = False,
     include_package_data = True,
     classifiers = [
-        #"Development Status :: 5 - Production/Stable",
         "Development Status :: 4 - Beta",
-        #"Operating System :: OS Independent",
         "Environment :: Web Environment",
         "License :: OSI Approved :: BSD License",
         "Intended Audience :: Developers",
         "Programming Language :: Python",
         "Programming Language :: Python :: 2",
         "Programming Language :: Python :: 2.7",
         "Programming Language :: Python :: 3",
```

### Comparing `pycouchdb-1.8/PKG-INFO` & `pycouchdb-1.9/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 1.1
 Name: pycouchdb
-Version: 1.8
+Version: 1.9
 Summary: Modern pure python CouchDB Client.
 Home-page: https://github.com/niwibe/py-couchdb
 Author: Andrey Antukh
 Author-email: niwi@niwi.be
 License: UNKNOWN
 Description: UNKNOWN
 Platform: UNKNOWN
```

