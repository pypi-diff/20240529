# Comparing `tmp/growcube-client-1.0.8.tar.gz` & `tmp/growcube-client-1.0.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "growcube-client-1.0.8.tar", last modified: Sun Sep 24 15:15:55 2023, max compression
+gzip compressed data, was "growcube-client-1.0.9.tar", last modified: Sat Nov  4 17:26:49 2023, max compression
```

## Comparing `growcube-client-1.0.8.tar` & `growcube-client-1.0.9.tar`

### file list

```diff
@@ -1,21 +1,21 @@
-drwxr-xr-x   0 jonny      (501) staff       (20)        0 2023-09-24 15:15:55.191770 growcube-client-1.0.8/
--rw-r--r--   0 jonny      (501) staff       (20)     1071 2023-05-12 18:21:08.000000 growcube-client-1.0.8/LICENSE
--rw-r--r--   0 jonny      (501) staff       (20)     1733 2023-09-24 15:15:55.191639 growcube-client-1.0.8/PKG-INFO
--rw-r--r--   0 jonny      (501) staff       (20)     3277 2023-09-23 17:21:16.000000 growcube-client-1.0.8/README.md
--rw-r--r--   0 jonny      (501) staff       (20)       38 2023-09-24 15:15:55.191820 growcube-client-1.0.8/setup.cfg
--rw-r--r--   0 jonny      (501) staff       (20)     1196 2023-09-24 15:15:37.000000 growcube-client-1.0.8/setup.py
-drwxr-xr-x   0 jonny      (501) staff       (20)        0 2023-09-24 15:15:55.188058 growcube-client-1.0.8/src/
-drwxr-xr-x   0 jonny      (501) staff       (20)        0 2023-09-24 15:15:55.190662 growcube-client-1.0.8/src/growcube_client/
--rw-r--r--   0 jonny      (501) staff       (20)      216 2023-09-19 18:39:27.000000 growcube-client-1.0.8/src/growcube_client/__init__.py
--rw-r--r--   0 jonny      (501) staff       (20)     5028 2023-09-24 15:15:37.000000 growcube-client-1.0.8/src/growcube_client/crowcubeclient.py
--rw-r--r--   0 jonny      (501) staff       (20)     7346 2023-09-23 17:07:08.000000 growcube-client-1.0.8/src/growcube_client/growcubecommand.py
--rw-r--r--   0 jonny      (501) staff       (20)     1801 2023-09-22 23:22:08.000000 growcube-client-1.0.8/src/growcube_client/growcubediscovery.py
--rw-r--r--   0 jonny      (501) staff       (20)      737 2023-09-23 16:01:01.000000 growcube-client-1.0.8/src/growcube_client/growcubeenums.py
--rw-r--r--   0 jonny      (501) staff       (20)     3693 2023-09-14 15:20:41.000000 growcube-client-1.0.8/src/growcube_client/growcubemessage.py
--rw-r--r--   0 jonny      (501) staff       (20)     1582 2023-09-23 15:23:15.000000 growcube-client-1.0.8/src/growcube_client/growcubeprotocol.py
--rw-r--r--   0 jonny      (501) staff       (20)    18809 2023-09-23 15:50:32.000000 growcube-client-1.0.8/src/growcube_client/growcubereport.py
-drwxr-xr-x   0 jonny      (501) staff       (20)        0 2023-09-24 15:15:55.191468 growcube-client-1.0.8/src/growcube_client.egg-info/
--rw-r--r--   0 jonny      (501) staff       (20)     1733 2023-09-24 15:15:55.000000 growcube-client-1.0.8/src/growcube_client.egg-info/PKG-INFO
--rw-r--r--   0 jonny      (501) staff       (20)      502 2023-09-24 15:15:55.000000 growcube-client-1.0.8/src/growcube_client.egg-info/SOURCES.txt
--rw-r--r--   0 jonny      (501) staff       (20)        1 2023-09-24 15:15:55.000000 growcube-client-1.0.8/src/growcube_client.egg-info/dependency_links.txt
--rw-r--r--   0 jonny      (501) staff       (20)       16 2023-09-24 15:15:55.000000 growcube-client-1.0.8/src/growcube_client.egg-info/top_level.txt
+drwxr-xr-x   0 jonny      (501) staff       (20)        0 2023-11-04 17:26:49.916360 growcube-client-1.0.9/
+-rw-r--r--   0 jonny      (501) staff       (20)     1071 2023-05-12 18:21:08.000000 growcube-client-1.0.9/LICENSE
+-rw-r--r--   0 jonny      (501) staff       (20)     1886 2023-11-04 17:26:49.916259 growcube-client-1.0.9/PKG-INFO
+-rw-r--r--   0 jonny      (501) staff       (20)     3624 2023-11-04 17:20:27.000000 growcube-client-1.0.9/README.md
+-rw-r--r--   0 jonny      (501) staff       (20)       38 2023-11-04 17:26:49.916396 growcube-client-1.0.9/setup.cfg
+-rw-r--r--   0 jonny      (501) staff       (20)     1346 2023-11-04 17:20:27.000000 growcube-client-1.0.9/setup.py
+drwxr-xr-x   0 jonny      (501) staff       (20)        0 2023-11-04 17:26:49.914110 growcube-client-1.0.9/src/
+drwxr-xr-x   0 jonny      (501) staff       (20)        0 2023-11-04 17:26:49.915679 growcube-client-1.0.9/src/growcube_client/
+-rw-r--r--   0 jonny      (501) staff       (20)      216 2023-09-19 18:39:27.000000 growcube-client-1.0.9/src/growcube_client/__init__.py
+-rw-r--r--   0 jonny      (501) staff       (20)     5028 2023-09-24 15:15:37.000000 growcube-client-1.0.9/src/growcube_client/crowcubeclient.py
+-rw-r--r--   0 jonny      (501) staff       (20)     7346 2023-09-23 17:07:08.000000 growcube-client-1.0.9/src/growcube_client/growcubecommand.py
+-rw-r--r--   0 jonny      (501) staff       (20)     1801 2023-09-22 23:22:08.000000 growcube-client-1.0.9/src/growcube_client/growcubediscovery.py
+-rw-r--r--   0 jonny      (501) staff       (20)      737 2023-09-23 16:01:01.000000 growcube-client-1.0.9/src/growcube_client/growcubeenums.py
+-rw-r--r--   0 jonny      (501) staff       (20)     3693 2023-09-14 15:20:41.000000 growcube-client-1.0.9/src/growcube_client/growcubemessage.py
+-rw-r--r--   0 jonny      (501) staff       (20)     1582 2023-09-23 15:23:15.000000 growcube-client-1.0.9/src/growcube_client/growcubeprotocol.py
+-rw-r--r--   0 jonny      (501) staff       (20)    18809 2023-09-23 15:50:32.000000 growcube-client-1.0.9/src/growcube_client/growcubereport.py
+drwxr-xr-x   0 jonny      (501) staff       (20)        0 2023-11-04 17:26:49.916109 growcube-client-1.0.9/src/growcube_client.egg-info/
+-rw-r--r--   0 jonny      (501) staff       (20)     1886 2023-11-04 17:26:49.000000 growcube-client-1.0.9/src/growcube_client.egg-info/PKG-INFO
+-rw-r--r--   0 jonny      (501) staff       (20)      502 2023-11-04 17:26:49.000000 growcube-client-1.0.9/src/growcube_client.egg-info/SOURCES.txt
+-rw-r--r--   0 jonny      (501) staff       (20)        1 2023-11-04 17:26:49.000000 growcube-client-1.0.9/src/growcube_client.egg-info/dependency_links.txt
+-rw-r--r--   0 jonny      (501) staff       (20)       16 2023-11-04 17:26:49.000000 growcube-client-1.0.9/src/growcube_client.egg-info/top_level.txt
```

### Comparing `growcube-client-1.0.8/LICENSE` & `growcube-client-1.0.9/LICENSE`

 * *Files identical despite different names*

### Comparing `growcube-client-1.0.8/PKG-INFO` & `growcube-client-1.0.9/PKG-INFO`

 * *Files 18% similar despite different names*

```diff
@@ -1,21 +1,24 @@
 Metadata-Version: 2.1
 Name: growcube-client
-Version: 1.0.8
+Version: 1.0.9
 Summary: A client for Elecrow Growcube plant watering devices
 Home-page: https://github.com/jonnybergdahl/Python-growcube-client
 Author: Jonny Bergdahl
 Author-email: github@bergdahl.it
 License: MIT
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Topic :: Home Automation
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.9
+Classifier: Programming Language :: Python :: 3.10
+Classifier: Programming Language :: Python :: 3.11
+Classifier: Programming Language :: Python :: 3.12
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
 This is an asyncio Python library to communicate with 
 [Elecrow Growcube](https://www.elecrow.com/growcube-gardening-plants-smart-watering-kit-device.html) devices.
 By using this library you can communicate directly with the device, without the need to use the phone app.
```

### Comparing `growcube-client-1.0.8/README.md` & `growcube-client-1.0.9/README.md`

 * *Files 16% similar despite different names*

```diff
@@ -1,9 +1,13 @@
 # Python-growcube-client
 
+[![PyPI version](https://badge.fury.io/py/growcube-client.svg)](https://badge.fury.io/py/growcube-client)
+[![PyPI pyversions](https://img.shields.io/pypi/pyversions/growcube-client.svg)](https://pypi.python.org/pypi/growcube-client/)
+[![PyPI license](https://img.shields.io/pypi/l/ansicolortags.svg)](https://pypi.python.org/pypi/ansicolortags/)
+
 This is an asyncio Python library to communicate with 
 [Elecrow Growcube](https://www.elecrow.com/growcube-gardening-plants-smart-watering-kit-device.html) devices.
 By using this library you can communicate directly with the device, without the need to use the phone app.
 
 Once connected to a device, the library will listen for messages from the device and use a callback function
 to return parsed messages to the application. The application can also send commands to the device.
```

### Comparing `growcube-client-1.0.8/setup.py` & `growcube-client-1.0.9/setup.py`

 * *Files 14% similar despite different names*

```diff
@@ -7,15 +7,15 @@
 
 # Get the long description from the README file
 with open(path.join(HERE, 'DESCRIPTION.md'), encoding='utf-8') as f:
     long_description = f.read()
 
 setup(
     name='growcube-client',
-    version='1.0.8',
+    version='1.0.9',
     description='A client for Elecrow Growcube plant watering devices',
     long_description=long_description,
     long_description_content_type="text/markdown",
     author='Jonny Bergdahl',
     author_email='github@bergdahl.it',
     url='https://github.com/jonnybergdahl/Python-growcube-client',
     license='MIT',
@@ -27,9 +27,12 @@
     classifiers=[
         'Development Status :: 5 - Production/Stable',
         'Intended Audience :: Developers',
         'License :: OSI Approved :: MIT License',
         'Topic :: Home Automation',
         'Programming Language :: Python :: 3',
         'Programming Language :: Python :: 3.9',
+        'Programming Language :: Python :: 3.10',
+        'Programming Language :: Python :: 3.11',
+        'Programming Language :: Python :: 3.12',
     ]
 )
```

### Comparing `growcube-client-1.0.8/src/growcube_client/crowcubeclient.py` & `growcube-client-1.0.9/src/growcube_client/crowcubeclient.py`

 * *Files identical despite different names*

### Comparing `growcube-client-1.0.8/src/growcube_client/growcubecommand.py` & `growcube-client-1.0.9/src/growcube_client/growcubecommand.py`

 * *Files identical despite different names*

### Comparing `growcube-client-1.0.8/src/growcube_client/growcubediscovery.py` & `growcube-client-1.0.9/src/growcube_client/growcubediscovery.py`

 * *Files identical despite different names*

### Comparing `growcube-client-1.0.8/src/growcube_client/growcubeenums.py` & `growcube-client-1.0.9/src/growcube_client/growcubeenums.py`

 * *Files identical despite different names*

### Comparing `growcube-client-1.0.8/src/growcube_client/growcubemessage.py` & `growcube-client-1.0.9/src/growcube_client/growcubemessage.py`

 * *Files identical despite different names*

### Comparing `growcube-client-1.0.8/src/growcube_client/growcubeprotocol.py` & `growcube-client-1.0.9/src/growcube_client/growcubeprotocol.py`

 * *Files identical despite different names*

### Comparing `growcube-client-1.0.8/src/growcube_client/growcubereport.py` & `growcube-client-1.0.9/src/growcube_client/growcubereport.py`

 * *Files identical despite different names*

### Comparing `growcube-client-1.0.8/src/growcube_client.egg-info/PKG-INFO` & `growcube-client-1.0.9/src/growcube_client.egg-info/PKG-INFO`

 * *Files 18% similar despite different names*

```diff
@@ -1,21 +1,24 @@
 Metadata-Version: 2.1
 Name: growcube-client
-Version: 1.0.8
+Version: 1.0.9
 Summary: A client for Elecrow Growcube plant watering devices
 Home-page: https://github.com/jonnybergdahl/Python-growcube-client
 Author: Jonny Bergdahl
 Author-email: github@bergdahl.it
 License: MIT
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Topic :: Home Automation
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.9
+Classifier: Programming Language :: Python :: 3.10
+Classifier: Programming Language :: Python :: 3.11
+Classifier: Programming Language :: Python :: 3.12
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
 This is an asyncio Python library to communicate with 
 [Elecrow Growcube](https://www.elecrow.com/growcube-gardening-plants-smart-watering-kit-device.html) devices.
 By using this library you can communicate directly with the device, without the need to use the phone app.
```

