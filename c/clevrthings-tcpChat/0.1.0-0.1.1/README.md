# Comparing `tmp/clevrthings_tcpchat-0.1.0.tar.gz` & `tmp/clevrthings_tcpchat-0.1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "clevrthings_tcpchat-0.1.0.tar", last modified: Tue May 28 21:55:44 2024, max compression
+gzip compressed data, was "clevrthings_tcpchat-0.1.1.tar", last modified: Tue May 28 22:04:49 2024, max compression
```

## Comparing `clevrthings_tcpchat-0.1.0.tar` & `clevrthings_tcpchat-0.1.1.tar`

### file list

```diff
@@ -1,14 +1,14 @@
-drwxr-xr-x   0 ricovanderhallen   (501) staff       (20)        0 2024-05-28 21:55:44.619773 clevrthings_tcpchat-0.1.0/
--rw-r--r--   0 ricovanderhallen   (501) staff       (20)     1067 2024-05-28 21:40:14.000000 clevrthings_tcpchat-0.1.0/LICENSE
--rw-r--r--   0 ricovanderhallen   (501) staff       (20)     1728 2024-05-28 21:55:44.619547 clevrthings_tcpchat-0.1.0/PKG-INFO
--rw-r--r--   0 ricovanderhallen   (501) staff       (20)     1205 2024-05-28 21:53:55.000000 clevrthings_tcpchat-0.1.0/README.md
-drwxr-xr-x   0 ricovanderhallen   (501) staff       (20)        0 2024-05-28 21:55:44.619294 clevrthings_tcpchat-0.1.0/clevrthings_tcpChat.egg-info/
--rw-r--r--   0 ricovanderhallen   (501) staff       (20)     1728 2024-05-28 21:55:44.000000 clevrthings_tcpchat-0.1.0/clevrthings_tcpChat.egg-info/PKG-INFO
--rw-r--r--   0 ricovanderhallen   (501) staff       (20)      237 2024-05-28 21:55:44.000000 clevrthings_tcpchat-0.1.0/clevrthings_tcpChat.egg-info/SOURCES.txt
--rw-r--r--   0 ricovanderhallen   (501) staff       (20)        1 2024-05-28 21:55:44.000000 clevrthings_tcpchat-0.1.0/clevrthings_tcpChat.egg-info/dependency_links.txt
--rw-r--r--   0 ricovanderhallen   (501) staff       (20)        8 2024-05-28 21:55:44.000000 clevrthings_tcpchat-0.1.0/clevrthings_tcpChat.egg-info/top_level.txt
--rw-r--r--   0 ricovanderhallen   (501) staff       (20)       38 2024-05-28 21:55:44.619813 clevrthings_tcpchat-0.1.0/setup.cfg
--rw-r--r--   0 ricovanderhallen   (501) staff       (20)      706 2024-05-28 21:54:41.000000 clevrthings_tcpchat-0.1.0/setup.py
-drwxr-xr-x   0 ricovanderhallen   (501) staff       (20)        0 2024-05-28 21:55:44.618951 clevrthings_tcpchat-0.1.0/tcpChat/
--rw-r--r--   0 ricovanderhallen   (501) staff       (20)       28 2024-05-28 21:26:49.000000 clevrthings_tcpchat-0.1.0/tcpChat/__init__.py
--rw-r--r--   0 ricovanderhallen   (501) staff       (20)     4235 2024-05-28 21:19:13.000000 clevrthings_tcpchat-0.1.0/tcpChat/tcpchat.py
+drwxr-xr-x   0 ricovanderhallen   (501) staff       (20)        0 2024-05-28 22:04:49.753762 clevrthings_tcpchat-0.1.1/
+-rw-r--r--   0 ricovanderhallen   (501) staff       (20)     1067 2024-05-28 21:40:14.000000 clevrthings_tcpchat-0.1.1/LICENSE
+-rw-r--r--   0 ricovanderhallen   (501) staff       (20)     1728 2024-05-28 22:04:49.753532 clevrthings_tcpchat-0.1.1/PKG-INFO
+-rw-r--r--   0 ricovanderhallen   (501) staff       (20)     1205 2024-05-28 22:03:24.000000 clevrthings_tcpchat-0.1.1/README.md
+drwxr-xr-x   0 ricovanderhallen   (501) staff       (20)        0 2024-05-28 22:04:49.753311 clevrthings_tcpchat-0.1.1/clevrthings_tcpChat.egg-info/
+-rw-r--r--   0 ricovanderhallen   (501) staff       (20)     1728 2024-05-28 22:04:49.000000 clevrthings_tcpchat-0.1.1/clevrthings_tcpChat.egg-info/PKG-INFO
+-rw-r--r--   0 ricovanderhallen   (501) staff       (20)      237 2024-05-28 22:04:49.000000 clevrthings_tcpchat-0.1.1/clevrthings_tcpChat.egg-info/SOURCES.txt
+-rw-r--r--   0 ricovanderhallen   (501) staff       (20)        1 2024-05-28 22:04:49.000000 clevrthings_tcpchat-0.1.1/clevrthings_tcpChat.egg-info/dependency_links.txt
+-rw-r--r--   0 ricovanderhallen   (501) staff       (20)        8 2024-05-28 22:04:49.000000 clevrthings_tcpchat-0.1.1/clevrthings_tcpChat.egg-info/top_level.txt
+-rw-r--r--   0 ricovanderhallen   (501) staff       (20)       38 2024-05-28 22:04:49.753805 clevrthings_tcpchat-0.1.1/setup.cfg
+-rw-r--r--   0 ricovanderhallen   (501) staff       (20)      706 2024-05-28 22:04:13.000000 clevrthings_tcpchat-0.1.1/setup.py
+drwxr-xr-x   0 ricovanderhallen   (501) staff       (20)        0 2024-05-28 22:04:49.753080 clevrthings_tcpchat-0.1.1/tcpChat/
+-rw-r--r--   0 ricovanderhallen   (501) staff       (20)       28 2024-05-28 21:26:49.000000 clevrthings_tcpchat-0.1.1/tcpChat/__init__.py
+-rw-r--r--   0 ricovanderhallen   (501) staff       (20)     4235 2024-05-28 21:19:13.000000 clevrthings_tcpchat-0.1.1/tcpChat/tcpchat.py
```

### Comparing `clevrthings_tcpchat-0.1.0/LICENSE` & `clevrthings_tcpchat-0.1.1/LICENSE`

 * *Files identical despite different names*

### Comparing `clevrthings_tcpchat-0.1.0/PKG-INFO` & `clevrthings_tcpchat-0.1.1/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
-Name: clevrthings_tcpChat
-Version: 0.1.0
+Name: clevrthings-tcpChat
+Version: 0.1.1
 Summary: A simple Python module for creating a TCP chat connection between two computers to send commands or information.
 Home-page: https://github.com/clevrthings/tcpChat
 Author: Clevrthings
 Author-email: info@clevrthings.com
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
@@ -19,15 +19,15 @@
 GitHub: [tcpChat](https://github.com/clevrthings/tcpChat)
 
 ## Installation
 
 Use the package manager [pip](https://pip.pypa.io/en/stable/) to install tcpChat.
 
 ```bash
-pip install clevrthings_tcpChat
+pip install clevrthings-tcpChat
 ```
 
 ## Usage
 ```python
 from tcpChat import tcpchat
 
 def callback_function(message):
```

### Comparing `clevrthings_tcpchat-0.1.0/README.md` & `clevrthings_tcpchat-0.1.1/README.md`

 * *Files 1% similar despite different names*

```diff
@@ -5,15 +5,15 @@
 GitHub: [tcpChat](https://github.com/clevrthings/tcpChat)
 
 ## Installation
 
 Use the package manager [pip](https://pip.pypa.io/en/stable/) to install tcpChat.
 
 ```bash
-pip install clevrthings_tcpChat
+pip install clevrthings-tcpChat
 ```
 
 ## Usage
 ```python
 from tcpChat import tcpchat
 
 def callback_function(message):
```

### Comparing `clevrthings_tcpchat-0.1.0/clevrthings_tcpChat.egg-info/PKG-INFO` & `clevrthings_tcpchat-0.1.1/clevrthings_tcpChat.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
-Name: clevrthings_tcpChat
-Version: 0.1.0
+Name: clevrthings-tcpChat
+Version: 0.1.1
 Summary: A simple Python module for creating a TCP chat connection between two computers to send commands or information.
 Home-page: https://github.com/clevrthings/tcpChat
 Author: Clevrthings
 Author-email: info@clevrthings.com
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
@@ -19,15 +19,15 @@
 GitHub: [tcpChat](https://github.com/clevrthings/tcpChat)
 
 ## Installation
 
 Use the package manager [pip](https://pip.pypa.io/en/stable/) to install tcpChat.
 
 ```bash
-pip install clevrthings_tcpChat
+pip install clevrthings-tcpChat
 ```
 
 ## Usage
 ```python
 from tcpChat import tcpchat
 
 def callback_function(message):
```

### Comparing `clevrthings_tcpchat-0.1.0/setup.py` & `clevrthings_tcpchat-0.1.1/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from setuptools import setup, find_packages
 
 setup(
-    name="clevrthings_tcpChat",
-    version="0.1.0",
+    name="clevrthings-tcpChat",
+    version="0.1.1",
     packages=find_packages(),
     install_requires=[],
     author="Clevrthings",
     author_email="info@clevrthings.com",
     description="A simple Python module for creating a TCP chat connection between two computers to send commands or information.",
     long_description=open("README.md").read(),
     long_description_content_type="text/markdown",
```

### Comparing `clevrthings_tcpchat-0.1.0/tcpChat/tcpchat.py` & `clevrthings_tcpchat-0.1.1/tcpChat/tcpchat.py`

 * *Files identical despite different names*

