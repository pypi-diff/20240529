# Comparing `tmp/vtjson-1.8.1.tar.gz` & `tmp/vtjson-1.8.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "vtjson-1.8.1.tar", last modified: Tue May 28 22:44:53 2024, max compression
+gzip compressed data, was "vtjson-1.8.2.tar", last modified: Wed May 29 02:06:14 2024, max compression
```

## Comparing `vtjson-1.8.1.tar` & `vtjson-1.8.2.tar`

### file list

```diff
@@ -1,13 +1,13 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-28 22:44:53.789933 vtjson-1.8.1/
--rw-r--r--   0 runner    (1001) docker     (127)     1077 2024-05-28 22:44:47.000000 vtjson-1.8.1/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)    20545 2024-05-28 22:44:53.789933 vtjson-1.8.1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)    19896 2024-05-28 22:44:47.000000 vtjson-1.8.1/README.md
--rw-r--r--   0 runner    (1001) docker     (127)      804 2024-05-28 22:44:47.000000 vtjson-1.8.1/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-28 22:44:53.789933 vtjson-1.8.1/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-28 22:44:53.789933 vtjson-1.8.1/vtjson.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)    20545 2024-05-28 22:44:53.000000 vtjson-1.8.1/vtjson.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      191 2024-05-28 22:44:53.000000 vtjson-1.8.1/vtjson.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-28 22:44:53.000000 vtjson-1.8.1/vtjson.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       44 2024-05-28 22:44:53.000000 vtjson-1.8.1/vtjson.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)        7 2024-05-28 22:44:53.000000 vtjson-1.8.1/vtjson.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)    35833 2024-05-28 22:44:47.000000 vtjson-1.8.1/vtjson.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-29 02:06:14.041240 vtjson-1.8.2/
+-rw-r--r--   0 runner    (1001) docker     (127)     1077 2024-05-29 02:06:03.000000 vtjson-1.8.2/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)    20545 2024-05-29 02:06:14.041240 vtjson-1.8.2/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)    19896 2024-05-29 02:06:03.000000 vtjson-1.8.2/README.md
+-rw-r--r--   0 runner    (1001) docker     (127)      804 2024-05-29 02:06:03.000000 vtjson-1.8.2/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-29 02:06:14.041240 vtjson-1.8.2/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-29 02:06:14.041240 vtjson-1.8.2/vtjson.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)    20545 2024-05-29 02:06:14.000000 vtjson-1.8.2/vtjson.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      191 2024-05-29 02:06:14.000000 vtjson-1.8.2/vtjson.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-29 02:06:14.000000 vtjson-1.8.2/vtjson.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       44 2024-05-29 02:06:14.000000 vtjson-1.8.2/vtjson.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        7 2024-05-29 02:06:14.000000 vtjson-1.8.2/vtjson.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)    35776 2024-05-29 02:06:03.000000 vtjson-1.8.2/vtjson.py
```

### Comparing `vtjson-1.8.1/LICENSE` & `vtjson-1.8.2/LICENSE`

 * *Files identical despite different names*

### Comparing `vtjson-1.8.1/PKG-INFO` & `vtjson-1.8.2/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: vtjson
-Version: 1.8.1
+Version: 1.8.2
 Summary: A lightweight package for validating JSON like Python objects
 Author-email: Michel Van den Bergh <michel.vandenbergh@uhasselt.be>
 Project-URL: Homepage, https://github.com/vdbergh/vtjson
 Project-URL: Bug Tracker, https://github.com/vdbergh/vtjson/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

### Comparing `vtjson-1.8.1/README.md` & `vtjson-1.8.2/README.md`

 * *Files identical despite different names*

### Comparing `vtjson-1.8.1/pyproject.toml` & `vtjson-1.8.2/pyproject.toml`

 * *Files identical despite different names*

### Comparing `vtjson-1.8.1/vtjson.egg-info/PKG-INFO` & `vtjson-1.8.2/vtjson.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: vtjson
-Version: 1.8.1
+Version: 1.8.2
 Summary: A lightweight package for validating JSON like Python objects
 Author-email: Michel Van den Bergh <michel.vandenbergh@uhasselt.be>
 Project-URL: Homepage, https://github.com/vdbergh/vtjson
 Project-URL: Bug Tracker, https://github.com/vdbergh/vtjson/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

### Comparing `vtjson-1.8.1/vtjson.py` & `vtjson-1.8.2/vtjson.py`

 * *Files 1% similar despite different names*

```diff
@@ -28,15 +28,15 @@
     from types import GenericAlias as _GenericAlias
 except ImportError:
     # For compatibility with older Pythons
     class _GenericAlias(type):
         pass
 
 
-__version__ = "1.8.1"
+__version__ = "1.8.2"
 
 
 _dns_resolver = None
 
 
 def _get_dns_resolver():
     global _dns_resolver
@@ -1115,40 +1115,41 @@
 
         for k in self.min_keys:
             name_ = f"{name}['{k}']"
             if k not in object:
                 return f"{name_} is missing"
 
         for k in object:
+            vals = []
             name_ = f"{name}['{k}']"
             if k in self.object_keys:
                 val = self.schema[k].__validate__(object[k], name=name_, strict=strict)
-                if val != "":
-                    return val
-                continue
-            else:
-                match = False
-                vals = []
-                for kk in self.other_keys:
-                    if kk.__validate__(k, name="key", strict=strict) == "":
-                        val = self.schema[kk].__validate__(
-                            object[k], name=name_, strict=strict
-                        )
-                        if val == "":
-                            match = True
-                            break
-                        else:
-                            vals.append(val)
-
-                if match:
+                if val == "":
                     continue
-                elif len(vals) > 0:
-                    return " and ".join(vals)
-                if strict:
-                    return f"{name_} is not in the schema"
+                else:
+                    vals.append(val)
+
+            match = False
+            for kk in self.other_keys:
+                if kk.__validate__(k, name="key", strict=strict) == "":
+                    val = self.schema[kk].__validate__(
+                        object[k], name=name_, strict=strict
+                    )
+                    if val == "":
+                        match = True
+                        break
+                    else:
+                        vals.append(val)
+
+            if match:
+                continue
+            elif len(vals) > 0:
+                return " and ".join(vals)
+            if strict:
+                return f"{name_} is not in the schema"
         return ""
 
     def __str__(self):
         return str(self.schema)
 
 
 # schema = {regex("[a-z]+"): "lc", regex("[A-Z]+"): "UC"}
```

