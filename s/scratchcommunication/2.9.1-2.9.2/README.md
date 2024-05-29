# Comparing `tmp/scratchcommunication-2.9.1.tar.gz` & `tmp/scratchcommunication-2.9.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "scratchcommunication-2.9.1.tar", last modified: Tue May 28 17:57:42 2024, max compression
+gzip compressed data, was "scratchcommunication-2.9.2.tar", last modified: Tue May 28 18:06:36 2024, max compression
```

## Comparing `scratchcommunication-2.9.1.tar` & `scratchcommunication-2.9.2.tar`

### file list

```diff
@@ -1,26 +1,27 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-28 17:57:42.767543 scratchcommunication-2.9.1/
--rw-r--r--   0 runner    (1001) docker     (127)     1056 2024-05-28 17:57:39.000000 scratchcommunication-2.9.1/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)    16512 2024-05-28 17:57:42.767543 scratchcommunication-2.9.1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)    15652 2024-05-28 17:57:39.000000 scratchcommunication-2.9.1/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-28 17:57:42.763543 scratchcommunication-2.9.1/scratchcommunication/
--rw-r--r--   0 runner    (1001) docker     (127)      358 2024-05-28 17:57:39.000000 scratchcommunication-2.9.1/scratchcommunication/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    18302 2024-05-28 17:57:39.000000 scratchcommunication-2.9.1/scratchcommunication/cloud.py
--rw-r--r--   0 runner    (1001) docker     (127)    14461 2024-05-28 17:57:39.000000 scratchcommunication-2.9.1/scratchcommunication/cloud_socket.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-28 17:57:42.767543 scratchcommunication-2.9.1/scratchcommunication/cloudrequests/
--rw-r--r--   0 runner    (1001) docker     (127)      110 2024-05-28 17:57:39.000000 scratchcommunication-2.9.1/scratchcommunication/cloudrequests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1016 2024-05-28 17:57:39.000000 scratchcommunication-2.9.1/scratchcommunication/cloudrequests/basetypes.py
--rw-r--r--   0 runner    (1001) docker     (127)    11413 2024-05-28 17:57:39.000000 scratchcommunication-2.9.1/scratchcommunication/cloudrequests/requests.py
--rw-r--r--   0 runner    (1001) docker     (127)      357 2024-05-28 17:57:39.000000 scratchcommunication-2.9.1/scratchcommunication/exceptions.py
--rw-r--r--   0 runner    (1001) docker     (127)      263 2024-05-28 17:57:39.000000 scratchcommunication-2.9.1/scratchcommunication/headers.py
--rw-r--r--   0 runner    (1001) docker     (127)     5605 2024-05-28 17:57:39.000000 scratchcommunication-2.9.1/scratchcommunication/security.py
--rw-r--r--   0 runner    (1001) docker     (127)     7688 2024-05-28 17:57:39.000000 scratchcommunication-2.9.1/scratchcommunication/session.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-28 17:57:42.767543 scratchcommunication-2.9.1/scratchcommunication.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)    16512 2024-05-28 17:57:42.000000 scratchcommunication-2.9.1/scratchcommunication.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      634 2024-05-28 17:57:42.000000 scratchcommunication-2.9.1/scratchcommunication.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-28 17:57:42.000000 scratchcommunication-2.9.1/scratchcommunication.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       72 2024-05-28 17:57:42.000000 scratchcommunication-2.9.1/scratchcommunication.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       21 2024-05-28 17:57:42.000000 scratchcommunication-2.9.1/scratchcommunication.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-28 17:57:42.767543 scratchcommunication-2.9.1/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)     1136 2024-05-28 17:57:39.000000 scratchcommunication-2.9.1/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-28 17:57:42.767543 scratchcommunication-2.9.1/tests/
--rw-r--r--   0 runner    (1001) docker     (127)      931 2024-05-28 17:57:39.000000 scratchcommunication-2.9.1/tests/test1.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-28 18:06:36.703259 scratchcommunication-2.9.2/
+-rw-r--r--   0 runner    (1001) docker     (127)     1056 2024-05-28 18:06:30.000000 scratchcommunication-2.9.2/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)    16512 2024-05-28 18:06:36.703259 scratchcommunication-2.9.2/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)    15652 2024-05-28 18:06:30.000000 scratchcommunication-2.9.2/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-28 18:06:36.703259 scratchcommunication-2.9.2/scratchcommunication/
+-rw-r--r--   0 runner    (1001) docker     (127)      358 2024-05-28 18:06:30.000000 scratchcommunication-2.9.2/scratchcommunication/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    18303 2024-05-28 18:06:30.000000 scratchcommunication-2.9.2/scratchcommunication/cloud.py
+-rw-r--r--   0 runner    (1001) docker     (127)    14461 2024-05-28 18:06:30.000000 scratchcommunication-2.9.2/scratchcommunication/cloud_socket.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-28 18:06:36.703259 scratchcommunication-2.9.2/scratchcommunication/cloudrequests/
+-rw-r--r--   0 runner    (1001) docker     (127)      110 2024-05-28 18:06:30.000000 scratchcommunication-2.9.2/scratchcommunication/cloudrequests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1016 2024-05-28 18:06:30.000000 scratchcommunication-2.9.2/scratchcommunication/cloudrequests/basetypes.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11441 2024-05-28 18:06:30.000000 scratchcommunication-2.9.2/scratchcommunication/cloudrequests/requests.py
+-rw-r--r--   0 runner    (1001) docker     (127)      357 2024-05-28 18:06:30.000000 scratchcommunication-2.9.2/scratchcommunication/exceptions.py
+-rw-r--r--   0 runner    (1001) docker     (127)      263 2024-05-28 18:06:30.000000 scratchcommunication-2.9.2/scratchcommunication/headers.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5605 2024-05-28 18:06:30.000000 scratchcommunication-2.9.2/scratchcommunication/security.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7688 2024-05-28 18:06:30.000000 scratchcommunication-2.9.2/scratchcommunication/session.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-28 18:06:36.703259 scratchcommunication-2.9.2/scratchcommunication.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)    16512 2024-05-28 18:06:36.000000 scratchcommunication-2.9.2/scratchcommunication.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      649 2024-05-28 18:06:36.000000 scratchcommunication-2.9.2/scratchcommunication.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-28 18:06:36.000000 scratchcommunication-2.9.2/scratchcommunication.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       72 2024-05-28 18:06:36.000000 scratchcommunication-2.9.2/scratchcommunication.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       21 2024-05-28 18:06:36.000000 scratchcommunication-2.9.2/scratchcommunication.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-28 18:06:36.703259 scratchcommunication-2.9.2/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)     1136 2024-05-28 18:06:30.000000 scratchcommunication-2.9.2/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-28 18:06:36.703259 scratchcommunication-2.9.2/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)      931 2024-05-28 18:06:30.000000 scratchcommunication-2.9.2/tests/test1.py
+-rw-r--r--   0 runner    (1001) docker     (127)      763 2024-05-28 18:06:30.000000 scratchcommunication-2.9.2/tests/test2.py
```

### Comparing `scratchcommunication-2.9.1/LICENSE` & `scratchcommunication-2.9.2/LICENSE`

 * *Files identical despite different names*

### Comparing `scratchcommunication-2.9.1/PKG-INFO` & `scratchcommunication-2.9.2/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: scratchcommunication
-Version: 2.9.1
+Version: 2.9.2
 Summary: A python module for communicating with scratch projects
 Home-page: https://github.com/thecommcraft/scratchcommunication
 Author: Simon Gilde
 Author-email: simon.c.gilde@gmail.com
 Keywords: scratch,api
 Classifier: Development Status :: 4 - Beta
 Classifier: Intended Audience :: Developers
```

### Comparing `scratchcommunication-2.9.1/README.md` & `scratchcommunication-2.9.2/README.md`

 * *Files identical despite different names*

### Comparing `scratchcommunication-2.9.1/scratchcommunication/cloud.py` & `scratchcommunication-2.9.2/scratchcommunication/cloud.py`

 * *Files 0% similar despite different names*

```diff
@@ -137,15 +137,15 @@
 
     def stop_thread(self):
         """
         Use for stopping the underlying thread.
         """
         self.thread_running = False
         self.data_reception.stop(StopException, 0.1)
-        self.data_reception.join()
+        self.data_reception.join(5)
 
     def enable_quickaccess(self):
         """
         Use for enabling the use of the object as a lookup table.
         """
         self.quickaccess = True
```

### Comparing `scratchcommunication-2.9.1/scratchcommunication/cloud_socket.py` & `scratchcommunication-2.9.2/scratchcommunication/cloud_socket.py`

 * *Files identical despite different names*

### Comparing `scratchcommunication-2.9.1/scratchcommunication/cloudrequests/basetypes.py` & `scratchcommunication-2.9.2/scratchcommunication/cloudrequests/basetypes.py`

 * *Files identical despite different names*

### Comparing `scratchcommunication-2.9.1/scratchcommunication/cloudrequests/requests.py` & `scratchcommunication-2.9.2/scratchcommunication/cloudrequests/requests.py`

 * *Files 1% similar despite different names*

```diff
@@ -120,14 +120,15 @@
         """
         Stop the request handler.
         """
         if self.uses_thread:
             raise NotUsingAThread("Can't stop a request handler that is not using a thread.")
         self.thread.stop(StopRequestHandler)
         self.cloud_socket.stop()
+        self.thread.join(5)
                    
                    
 KW = Parameter.KEYWORD_ONLY
 KWPS = Parameter.POSITIONAL_OR_KEYWORD
 PS = Parameter.POSITIONAL_ONLY
 MKW = Parameter.VAR_KEYWORD
 MPS = Parameter.VAR_POSITIONAL
```

### Comparing `scratchcommunication-2.9.1/scratchcommunication/security.py` & `scratchcommunication-2.9.2/scratchcommunication/security.py`

 * *Files identical despite different names*

### Comparing `scratchcommunication-2.9.1/scratchcommunication/session.py` & `scratchcommunication-2.9.2/scratchcommunication/session.py`

 * *Files identical despite different names*

### Comparing `scratchcommunication-2.9.1/scratchcommunication.egg-info/PKG-INFO` & `scratchcommunication-2.9.2/scratchcommunication.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: scratchcommunication
-Version: 2.9.1
+Version: 2.9.2
 Summary: A python module for communicating with scratch projects
 Home-page: https://github.com/thecommcraft/scratchcommunication
 Author: Simon Gilde
 Author-email: simon.c.gilde@gmail.com
 Keywords: scratch,api
 Classifier: Development Status :: 4 - Beta
 Classifier: Intended Audience :: Developers
```

### Comparing `scratchcommunication-2.9.1/scratchcommunication.egg-info/SOURCES.txt` & `scratchcommunication-2.9.2/scratchcommunication.egg-info/SOURCES.txt`

 * *Files 14% similar despite different names*

```diff
@@ -12,8 +12,9 @@
 scratchcommunication.egg-info/SOURCES.txt
 scratchcommunication.egg-info/dependency_links.txt
 scratchcommunication.egg-info/requires.txt
 scratchcommunication.egg-info/top_level.txt
 scratchcommunication/cloudrequests/__init__.py
 scratchcommunication/cloudrequests/basetypes.py
 scratchcommunication/cloudrequests/requests.py
-tests/test1.py
+tests/test1.py
+tests/test2.py
```

### Comparing `scratchcommunication-2.9.1/setup.py` & `scratchcommunication-2.9.2/setup.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 from setuptools import setup, find_packages
 
 with open("README.md", encoding="utf-8") as f:
     long_description = f.read()
     
-VERSION = '2.9.1'
+VERSION = '2.9.2'
 
 setup(
     name='scratchcommunication',
     version=VERSION,
     author='Simon Gilde',
     author_email='simon.c.gilde@gmail.com',
     description='A python module for communicating with scratch projects',
```

### Comparing `scratchcommunication-2.9.1/tests/test1.py` & `scratchcommunication-2.9.2/tests/test1.py`

 * *Files identical despite different names*

