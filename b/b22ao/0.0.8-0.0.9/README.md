# Comparing `tmp/b22ao-0.0.8.tar.gz` & `tmp/b22ao-0.0.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/b22ao-0.0.8.tar", last modified: Tue Jul 21 07:30:26 2020, max compression
+gzip compressed data, was "dist/b22ao-0.0.9.tar", last modified: Wed Oct  7 17:20:57 2020, max compression
```

## Comparing `b22ao-0.0.8.tar` & `b22ao-0.0.9.tar`

### file list

```diff
@@ -1,17 +1,17 @@
-drwxr-xr-x   0 douglas   (1000) douglas   (1000)        0 2020-07-21 07:30:26.715630 b22ao-0.0.8/
--rw-r--r--   0 douglas   (1000) douglas   (1000)     1759 2020-07-21 07:30:26.715630 b22ao-0.0.8/PKG-INFO
--rw-r--r--   0 douglas   (1000) douglas   (1000)      993 2020-03-31 12:53:54.000000 b22ao-0.0.8/README.md
-drwxr-xr-x   0 douglas   (1000) douglas   (1000)        0 2020-07-21 07:30:26.715630 b22ao-0.0.8/b22ao/
--rw-r--r--   0 douglas   (1000) douglas   (1000)        0 2020-03-31 12:53:54.000000 b22ao-0.0.8/b22ao/__init__.py
--rw-r--r--   0 douglas   (1000) douglas   (1000)     2628 2020-06-15 09:12:22.000000 b22ao-0.0.8/b22ao/aosystem.py
--rw-r--r--   0 douglas   (1000) douglas   (1000)     2591 2020-03-31 12:53:54.000000 b22ao-0.0.8/b22ao/base.py
--rw-r--r--   0 douglas   (1000) douglas   (1000)      231 2020-03-31 12:53:54.000000 b22ao-0.0.8/b22ao/message.py
--rw-r--r--   0 douglas   (1000) douglas   (1000)      662 2020-06-15 10:19:45.000000 b22ao-0.0.8/b22ao/pvs.py
-drwxr-xr-x   0 douglas   (1000) douglas   (1000)        0 2020-07-21 07:30:26.715630 b22ao-0.0.8/b22ao.egg-info/
--rw-r--r--   0 douglas   (1000) douglas   (1000)     1759 2020-07-21 07:30:26.000000 b22ao-0.0.8/b22ao.egg-info/PKG-INFO
--rw-r--r--   0 douglas   (1000) douglas   (1000)      242 2020-07-21 07:30:26.000000 b22ao-0.0.8/b22ao.egg-info/SOURCES.txt
--rw-r--r--   0 douglas   (1000) douglas   (1000)        1 2020-07-21 07:30:26.000000 b22ao-0.0.8/b22ao.egg-info/dependency_links.txt
--rw-r--r--   0 douglas   (1000) douglas   (1000)       25 2020-07-21 07:30:26.000000 b22ao-0.0.8/b22ao.egg-info/requires.txt
--rw-r--r--   0 douglas   (1000) douglas   (1000)        6 2020-07-21 07:30:26.000000 b22ao-0.0.8/b22ao.egg-info/top_level.txt
--rw-r--r--   0 douglas   (1000) douglas   (1000)       38 2020-07-21 07:30:26.715630 b22ao-0.0.8/setup.cfg
--rw-r--r--   0 douglas   (1000) douglas   (1000)      712 2020-07-21 07:30:02.000000 b22ao-0.0.8/setup.py
+drwxr-xr-x   0 douglas   (1000) douglas   (1000)        0 2020-10-07 17:20:57.750653 b22ao-0.0.9/
+-rw-r--r--   0 douglas   (1000) douglas   (1000)     1759 2020-10-07 17:20:57.750653 b22ao-0.0.9/PKG-INFO
+-rw-r--r--   0 douglas   (1000) douglas   (1000)      993 2020-10-07 17:20:38.000000 b22ao-0.0.9/README.md
+drwxr-xr-x   0 douglas   (1000) douglas   (1000)        0 2020-10-07 17:20:57.747320 b22ao-0.0.9/b22ao/
+-rw-r--r--   0 douglas   (1000) douglas   (1000)        0 2020-10-07 17:20:38.000000 b22ao-0.0.9/b22ao/__init__.py
+-rw-r--r--   0 douglas   (1000) douglas   (1000)     2628 2020-10-07 17:20:38.000000 b22ao-0.0.9/b22ao/aosystem.py
+-rw-r--r--   0 douglas   (1000) douglas   (1000)     3006 2020-10-07 17:20:38.000000 b22ao-0.0.9/b22ao/base.py
+-rw-r--r--   0 douglas   (1000) douglas   (1000)      226 2020-10-07 17:20:38.000000 b22ao-0.0.9/b22ao/message.py
+-rw-r--r--   0 douglas   (1000) douglas   (1000)      662 2020-10-07 17:20:38.000000 b22ao-0.0.9/b22ao/pvs.py
+drwxr-xr-x   0 douglas   (1000) douglas   (1000)        0 2020-10-07 17:20:57.750653 b22ao-0.0.9/b22ao.egg-info/
+-rw-r--r--   0 douglas   (1000) douglas   (1000)     1759 2020-10-07 17:20:57.000000 b22ao-0.0.9/b22ao.egg-info/PKG-INFO
+-rw-r--r--   0 douglas   (1000) douglas   (1000)      242 2020-10-07 17:20:57.000000 b22ao-0.0.9/b22ao.egg-info/SOURCES.txt
+-rw-r--r--   0 douglas   (1000) douglas   (1000)        1 2020-10-07 17:20:57.000000 b22ao-0.0.9/b22ao.egg-info/dependency_links.txt
+-rw-r--r--   0 douglas   (1000) douglas   (1000)       25 2020-10-07 17:20:57.000000 b22ao-0.0.9/b22ao.egg-info/requires.txt
+-rw-r--r--   0 douglas   (1000) douglas   (1000)        6 2020-10-07 17:20:57.000000 b22ao-0.0.9/b22ao.egg-info/top_level.txt
+-rw-r--r--   0 douglas   (1000) douglas   (1000)       38 2020-10-07 17:20:57.750653 b22ao-0.0.9/setup.cfg
+-rw-r--r--   0 douglas   (1000) douglas   (1000)      712 2020-10-07 17:20:38.000000 b22ao-0.0.9/setup.py
```

### Comparing `b22ao-0.0.8/PKG-INFO` & `b22ao-0.0.9/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: b22ao
-Version: 0.0.8
+Version: 0.0.9
 Summary: API for B22 AO operations
 Home-page: https://gitlab.diamond.ac.uk/douglas/b22ao
 Author: Douglas Winter
 Author-email: douglas.winter@diamond.ac.uk
 License: UNKNOWN
 Description: # b22ao: API for B22 adaptive optics operations
```

### Comparing `b22ao-0.0.8/README.md` & `b22ao-0.0.9/README.md`

 * *Files identical despite different names*

### Comparing `b22ao-0.0.8/b22ao/aosystem.py` & `b22ao-0.0.9/b22ao/aosystem.py`

 * *Files identical despite different names*

### Comparing `b22ao-0.0.8/b22ao/base.py` & `b22ao-0.0.9/b22ao/base.py`

 * *Files 8% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 from b22ao.message import Message, State
 
 
 class BaseOperation:
 
     """
     Base class for any adaptive optics routine.
-    Children implement #start and #halt, and can #deform the mirrors and #capture data from the camera at their leisure!
+    Children implement #start and #stop, and can #deform the mirrors and #capture data from the camera at their leisure!
     """
 
     def __init__(self):
 
         self.ao = AOSystem()
         self.config = None
         self.listener = None
@@ -57,27 +57,24 @@
         """
         return self.ao.capture()
 
     def run(self):
         """
         Do not override. Implement #start instead
         """
-        if self.listener:
-            self.listener.notify(Message(self, State.Started))
+        self.notify(Message(self, State.Running))
         self.start()
-        if self.listener:
-            self.listener.notify(Message(self, State.Finished))
+        self.notify(Message(self, State.Idle))
 
     def abort(self):
         """
-        Do not override. Implement #halt instead
+        Do not override. Implement #stop instead
         """
         self.stop()
-        if self.listener:
-            self.listener.notify(Message(self, State.Failed, "Aborted"))
+        self.notify(Message(self, State.Idle, "Aborted"))
 
     def start(self):
         """
         Starts the operation
 
         If a JSON configuration file was specified,
         implementations can now access the dictionary self.config
@@ -85,7 +82,23 @@
         raise NotImplementedError
 
     def stop(self):
         """
         Stops the operation
         """
         raise NotImplementedError
+
+    def report_progress(self, iteration, value, **other_stuff):
+        """
+        Inform a listening component (e.g. a live plot) of the latest result.
+        """
+        msg = dict({"iteration": iteration, "value": value}, **other_stuff)
+        self.notify(Message(self, State.Running, msg))
+
+    def report_error(self, message):
+        self.notify(Message(self, State.Error, message))
+
+    def notify(self, message):
+        try:
+            self.listener.notify(message)
+        except AttributeError:
+            print(message)
```

### Comparing `b22ao-0.0.8/b22ao/pvs.py` & `b22ao-0.0.9/b22ao/pvs.py`

 * *Files identical despite different names*

### Comparing `b22ao-0.0.8/b22ao.egg-info/PKG-INFO` & `b22ao-0.0.9/b22ao.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: b22ao
-Version: 0.0.8
+Version: 0.0.9
 Summary: API for B22 AO operations
 Home-page: https://gitlab.diamond.ac.uk/douglas/b22ao
 Author: Douglas Winter
 Author-email: douglas.winter@diamond.ac.uk
 License: UNKNOWN
 Description: # b22ao: API for B22 adaptive optics operations
```

### Comparing `b22ao-0.0.8/setup.py` & `b22ao-0.0.9/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 import setuptools
 
 with open("README.md", "r") as fh:
     long_description = fh.read()
 
 setuptools.setup(
     name="b22ao",
-    version="0.0.8",
+    version="0.0.9",
     author="Douglas Winter",
     author_email="douglas.winter@diamond.ac.uk",
     description="API for B22 AO operations",
     long_description=long_description,
     long_description_content_type="text/markdown",
     url="https://gitlab.diamond.ac.uk/douglas/b22ao",
     packages=setuptools.find_packages(),
```

