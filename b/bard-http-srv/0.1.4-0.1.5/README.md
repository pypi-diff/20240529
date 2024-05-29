# Comparing `tmp/bard-http-srv-0.1.4.tar.gz` & `tmp/bard-http-srv-0.1.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "bard-http-srv-0.1.4.tar", last modified: Thu May  9 21:04:52 2024, max compression
+gzip compressed data, was "bard-http-srv-0.1.5.tar", last modified: Wed May 29 18:09:54 2024, max compression
```

## Comparing `bard-http-srv-0.1.4.tar` & `bard-http-srv-0.1.5.tar`

### file list

```diff
@@ -1,11 +1,11 @@
-drwxrwxrwx   0        0        0        0 2024-05-09 21:04:52.658639 bard-http-srv-0.1.4/
--rw-rw-rw-   0        0        0     1090 2024-02-22 04:30:03.000000 bard-http-srv-0.1.4/LICENSE
--rw-rw-rw-   0        0        0      938 2024-05-09 21:04:52.657535 bard-http-srv-0.1.4/PKG-INFO
-drwxrwxrwx   0        0        0        0 2024-05-09 21:04:52.654377 bard-http-srv-0.1.4/bard_http_srv.egg-info/
--rw-rw-rw-   0        0        0      938 2024-05-09 21:04:52.000000 bard-http-srv-0.1.4/bard_http_srv.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      200 2024-05-09 21:04:52.000000 bard-http-srv-0.1.4/bard_http_srv.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-05-09 21:04:52.000000 bard-http-srv-0.1.4/bard_http_srv.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       51 2024-05-09 21:04:52.000000 bard-http-srv-0.1.4/bard_http_srv.egg-info/requires.txt
--rw-rw-rw-   0        0        0        1 2024-05-09 21:04:52.000000 bard-http-srv-0.1.4/bard_http_srv.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2024-05-09 21:04:52.658639 bard-http-srv-0.1.4/setup.cfg
--rw-rw-rw-   0        0        0     1151 2024-05-09 21:03:07.000000 bard-http-srv-0.1.4/setup.py
+drwxrwxrwx   0        0        0        0 2024-05-29 18:09:54.435724 bard-http-srv-0.1.5/
+-rw-rw-rw-   0        0        0     1090 2024-02-22 04:30:03.000000 bard-http-srv-0.1.5/LICENSE
+-rw-rw-rw-   0        0        0      938 2024-05-29 18:09:54.434728 bard-http-srv-0.1.5/PKG-INFO
+drwxrwxrwx   0        0        0        0 2024-05-29 18:09:54.433264 bard-http-srv-0.1.5/bard_http_srv.egg-info/
+-rw-rw-rw-   0        0        0      938 2024-05-29 18:09:54.000000 bard-http-srv-0.1.5/bard_http_srv.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      200 2024-05-29 18:09:54.000000 bard-http-srv-0.1.5/bard_http_srv.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-05-29 18:09:54.000000 bard-http-srv-0.1.5/bard_http_srv.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       51 2024-05-29 18:09:54.000000 bard-http-srv-0.1.5/bard_http_srv.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        1 2024-05-29 18:09:54.000000 bard-http-srv-0.1.5/bard_http_srv.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2024-05-29 18:09:54.436025 bard-http-srv-0.1.5/setup.cfg
+-rw-rw-rw-   0        0        0     1151 2024-05-29 18:09:49.000000 bard-http-srv-0.1.5/setup.py
```

### Comparing `bard-http-srv-0.1.4/LICENSE` & `bard-http-srv-0.1.5/LICENSE`

 * *Files identical despite different names*

### Comparing `bard-http-srv-0.1.4/PKG-INFO` & `bard-http-srv-0.1.5/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: bard-http-srv
-Version: 0.1.4
+Version: 0.1.5
 Summary: bard http server
 Home-page: https://github.com/NullpointerW/bard-http-srv
 Author: vow1231a
 Author-email: voidmanwzp@gmail.com
 License: MIT
 Project-URL: Source, https://github.com/NullpointerW/bard-http-srv
 Classifier: Development Status :: 4 - Beta
```

### Comparing `bard-http-srv-0.1.4/bard_http_srv.egg-info/PKG-INFO` & `bard-http-srv-0.1.5/bard_http_srv.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: bard-http-srv
-Version: 0.1.4
+Version: 0.1.5
 Summary: bard http server
 Home-page: https://github.com/NullpointerW/bard-http-srv
 Author: vow1231a
 Author-email: voidmanwzp@gmail.com
 License: MIT
 Project-URL: Source, https://github.com/NullpointerW/bard-http-srv
 Classifier: Development Status :: 4 - Beta
```

### Comparing `bard-http-srv-0.1.4/setup.py` & `bard-http-srv-0.1.5/setup.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from setuptools import setup, find_packages
 
 setup(
     name="bard-http-srv",
-    version="0.1.4",
+    version="0.1.5",
     packages=find_packages(),
     install_requires=[
         # 在这里列出你的库所需的其他Python包
         'bardapi==0.1.23a0',
         'Flask==2.3.2',
         'configparser==7.0.0',
     ],
```

