# Comparing `tmp/djecorator-1.0.3.tar.gz` & `tmp/djecorator-1.1.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "djecorator-1.0.3.tar", last modified: Fri Jan  1 00:00:00 2016, max compression
+gzip compressed data, was "djecorator-1.1.0.tar", last modified: Fri Jan  1 00:00:00 2016, max compression
```

## Comparing `djecorator-1.0.3.tar` & `djecorator-1.1.0.tar`

### file list

```diff
@@ -1,6 +1,6 @@
--rw-r--r--   0        0        0     3078 2024-04-28 21:56:13.477752 djecorator-1.0.3/.gitignore
--rw-r--r--   0        0        0     1086 2024-04-28 21:38:12.088814 djecorator-1.0.3/LICENSE
--rw-r--r--   0        0        0      411 2024-04-29 02:05:48.209193 djecorator-1.0.3/README.md
--rw-r--r--   0        0        0     1293 2024-04-28 22:51:57.093817 djecorator-1.0.3/djecorator.py
--rw-r--r--   0        0        0      476 2024-04-29 19:31:16.724807 djecorator-1.0.3/pyproject.toml
--rw-r--r--   0        0        0      757 1970-01-01 00:00:00.000000 djecorator-1.0.3/PKG-INFO
+-rw-r--r--   0        0        0     3078 2024-05-29 02:16:48.914305 djecorator-1.1.0/.gitignore
+-rw-r--r--   0        0        0     1086 2024-05-29 02:16:48.914436 djecorator-1.1.0/LICENSE
+-rw-r--r--   0        0        0      411 2024-05-29 02:16:48.914566 djecorator-1.1.0/README.md
+-rw-r--r--   0        0        0     1245 2024-05-29 02:17:02.948464 djecorator-1.1.0/djecorator.py
+-rw-r--r--   0        0        0      476 2024-05-29 02:17:08.781613 djecorator-1.1.0/pyproject.toml
+-rw-r--r--   0        0        0      757 1970-01-01 00:00:00.000000 djecorator-1.1.0/PKG-INFO
```

### Comparing `djecorator-1.0.3/.gitignore` & `djecorator-1.1.0/.gitignore`

 * *Files identical despite different names*

### Comparing `djecorator-1.0.3/LICENSE` & `djecorator-1.1.0/LICENSE`

 * *Files identical despite different names*

### Comparing `djecorator-1.0.3/djecorator.py` & `djecorator-1.1.0/djecorator.py`

 * *Files 9% similar despite different names*

```diff
@@ -12,15 +12,14 @@
         self.name_prefix = name_prefix
         self.routes = {}
 
     def __call__(self, path=None, name=None):
         def wrapper(f):
             urlname = self.name_prefix + (name or f.__name__)
             urlpath = path or f.__name__
-            urlpath = urlpath.replace("_", "-")
             urlpath = self.url_prefix + "/" + urlpath.lstrip("/")
             
             # Check if f is a class with an as_view method
             if inspect.isclass(f) and hasattr(f, 'as_view'):
                 self.routes[urlname] = urlpath, f.as_view()
             else:
                 self.routes[urlname] = urlpath, f
```

### Comparing `djecorator-1.0.3/PKG-INFO` & `djecorator-1.1.0/PKG-INFO`

 * *Files 16% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: djecorator
-Version: 1.0.3
+Version: 1.1.0
 Summary: A flask-style decorator for Django views
 Author-email: Stephan Fitzpatrick <knowsuchagency@gmail.com>
 Description-Content-Type: text/markdown
 Classifier: License :: OSI Approved :: MIT License
 Requires-Dist: django
 Project-URL: Source, https://github.com/knowsuchagency/djecorator
```

