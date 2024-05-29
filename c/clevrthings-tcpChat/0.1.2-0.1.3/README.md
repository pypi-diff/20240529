# Comparing `tmp/clevrthings_tcpchat-0.1.2.tar.gz` & `tmp/clevrthings_tcpchat-0.1.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "clevrthings_tcpchat-0.1.2.tar", last modified: Tue May 28 22:51:49 2024, max compression
+gzip compressed data, was "clevrthings_tcpchat-0.1.3.tar", last modified: Wed May 29 01:18:53 2024, max compression
```

## Comparing `clevrthings_tcpchat-0.1.2.tar` & `clevrthings_tcpchat-0.1.3.tar`

### file list

```diff
@@ -1,14 +1,14 @@
-drwxr-xr-x   0 ricovanderhallen   (501) staff       (20)        0 2024-05-28 22:51:49.673904 clevrthings_tcpchat-0.1.2/
--rw-r--r--   0 ricovanderhallen   (501) staff       (20)     1067 2024-05-28 21:40:14.000000 clevrthings_tcpchat-0.1.2/LICENSE
--rw-r--r--   0 ricovanderhallen   (501) staff       (20)     1570 2024-05-28 22:51:49.673678 clevrthings_tcpchat-0.1.2/PKG-INFO
--rw-r--r--   0 ricovanderhallen   (501) staff       (20)     1047 2024-05-28 22:37:33.000000 clevrthings_tcpchat-0.1.2/README.md
-drwxr-xr-x   0 ricovanderhallen   (501) staff       (20)        0 2024-05-28 22:51:49.673450 clevrthings_tcpchat-0.1.2/clevrthings_tcpChat.egg-info/
--rw-r--r--   0 ricovanderhallen   (501) staff       (20)     1570 2024-05-28 22:51:49.000000 clevrthings_tcpchat-0.1.2/clevrthings_tcpChat.egg-info/PKG-INFO
--rw-r--r--   0 ricovanderhallen   (501) staff       (20)      237 2024-05-28 22:51:49.000000 clevrthings_tcpchat-0.1.2/clevrthings_tcpChat.egg-info/SOURCES.txt
--rw-r--r--   0 ricovanderhallen   (501) staff       (20)        1 2024-05-28 22:51:49.000000 clevrthings_tcpchat-0.1.2/clevrthings_tcpChat.egg-info/dependency_links.txt
--rw-r--r--   0 ricovanderhallen   (501) staff       (20)        8 2024-05-28 22:51:49.000000 clevrthings_tcpchat-0.1.2/clevrthings_tcpChat.egg-info/top_level.txt
--rw-r--r--   0 ricovanderhallen   (501) staff       (20)       38 2024-05-28 22:51:49.673947 clevrthings_tcpchat-0.1.2/setup.cfg
--rw-rw-r--   0 ricovanderhallen   (501) staff       (20)      706 2024-05-28 22:50:29.000000 clevrthings_tcpchat-0.1.2/setup.py
-drwxr-xr-x   0 ricovanderhallen   (501) staff       (20)        0 2024-05-28 22:51:49.673138 clevrthings_tcpchat-0.1.2/tcpChat/
--rw-r--r--   0 ricovanderhallen   (501) staff       (20)       28 2024-05-28 21:26:49.000000 clevrthings_tcpchat-0.1.2/tcpChat/__init__.py
--rw-r--r--   0 ricovanderhallen   (501) staff       (20)     4235 2024-05-28 21:19:13.000000 clevrthings_tcpchat-0.1.2/tcpChat/tcpchat.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-29 01:18:53.840021 clevrthings_tcpchat-0.1.3/
+-rw-r--r--   0 runner    (1001) docker     (127)     1067 2024-05-29 01:18:49.000000 clevrthings_tcpchat-0.1.3/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)     1570 2024-05-29 01:18:53.840021 clevrthings_tcpchat-0.1.3/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     1047 2024-05-29 01:18:49.000000 clevrthings_tcpchat-0.1.3/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-29 01:18:53.840021 clevrthings_tcpchat-0.1.3/clevrthings_tcpChat.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     1570 2024-05-29 01:18:53.000000 clevrthings_tcpchat-0.1.3/clevrthings_tcpChat.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      237 2024-05-29 01:18:53.000000 clevrthings_tcpchat-0.1.3/clevrthings_tcpChat.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-29 01:18:53.000000 clevrthings_tcpchat-0.1.3/clevrthings_tcpChat.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        8 2024-05-29 01:18:53.000000 clevrthings_tcpchat-0.1.3/clevrthings_tcpChat.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-29 01:18:53.840021 clevrthings_tcpchat-0.1.3/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)      706 2024-05-29 01:18:49.000000 clevrthings_tcpchat-0.1.3/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-29 01:18:53.840021 clevrthings_tcpchat-0.1.3/tcpChat/
+-rw-r--r--   0 runner    (1001) docker     (127)       28 2024-05-29 01:18:49.000000 clevrthings_tcpchat-0.1.3/tcpChat/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4235 2024-05-29 01:18:49.000000 clevrthings_tcpchat-0.1.3/tcpChat/tcpchat.py
```

### Comparing `clevrthings_tcpchat-0.1.2/LICENSE` & `clevrthings_tcpchat-0.1.3/LICENSE`

 * *Files identical despite different names*

### Comparing `clevrthings_tcpchat-0.1.2/PKG-INFO` & `clevrthings_tcpchat-0.1.3/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: clevrthings-tcpChat
-Version: 0.1.2
+Version: 0.1.3
 Summary: A simple Python module for creating a TCP chat connection between two computers to send commands or information.
 Home-page: https://github.com/clevrthings/tcpChat
 Author: Clevrthings
 Author-email: info@clevrthings.com
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

### Comparing `clevrthings_tcpchat-0.1.2/README.md` & `clevrthings_tcpchat-0.1.3/README.md`

 * *Files identical despite different names*

### Comparing `clevrthings_tcpchat-0.1.2/clevrthings_tcpChat.egg-info/PKG-INFO` & `clevrthings_tcpchat-0.1.3/clevrthings_tcpChat.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: clevrthings-tcpChat
-Version: 0.1.2
+Version: 0.1.3
 Summary: A simple Python module for creating a TCP chat connection between two computers to send commands or information.
 Home-page: https://github.com/clevrthings/tcpChat
 Author: Clevrthings
 Author-email: info@clevrthings.com
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

### Comparing `clevrthings_tcpchat-0.1.2/setup.py` & `clevrthings_tcpchat-0.1.3/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from setuptools import setup, find_packages
 
 setup(
     name="clevrthings-tcpChat",
-    version="0.1.2",
+    version="0.1.3",
     packages=find_packages(),
     install_requires=[],
     author="Clevrthings",
     author_email="info@clevrthings.com",
     description="A simple Python module for creating a TCP chat connection between two computers to send commands or information.",
     long_description=open("README.md").read(),
     long_description_content_type="text/markdown",
```

### Comparing `clevrthings_tcpchat-0.1.2/tcpChat/tcpchat.py` & `clevrthings_tcpchat-0.1.3/tcpChat/tcpchat.py`

 * *Files identical despite different names*

