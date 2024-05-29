# Comparing `tmp/httpauth-0.4.tar.gz` & `tmp/httpauth-0.4.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "httpauth-0.4.tar", last modified: Tue May 21 12:05:19 2024, max compression
+gzip compressed data, was "httpauth-0.4.1.tar", last modified: Wed May 29 09:46:59 2024, max compression
```

## Comparing `httpauth-0.4.tar` & `httpauth-0.4.1.tar`

### file list

```diff
@@ -1,12 +1,15 @@
-drwxr-xr-x   0 j          (501) wheel        (0)        0 2024-05-21 12:05:19.227639 httpauth-0.4/
--rw-r--r--   0 j          (501) wheel        (0)      748 2024-05-21 12:03:58.000000 httpauth-0.4/LICENSE
--rw-r--r--   0 j          (501) wheel        (0)      434 2024-05-21 12:05:19.227500 httpauth-0.4/PKG-INFO
--rw-r--r--   0 j          (501) wheel        (0)     1197 2024-05-21 12:03:58.000000 httpauth-0.4/README.rst
-drwxr-xr-x   0 j          (501) wheel        (0)        0 2024-05-21 12:05:19.227362 httpauth-0.4/httpauth.egg-info/
--rw-r--r--   0 j          (501) wheel        (0)      434 2024-05-21 12:05:19.000000 httpauth-0.4/httpauth.egg-info/PKG-INFO
--rw-r--r--   0 j          (501) wheel        (0)      167 2024-05-21 12:05:19.000000 httpauth-0.4/httpauth.egg-info/SOURCES.txt
--rw-r--r--   0 j          (501) wheel        (0)        1 2024-05-21 12:05:19.000000 httpauth-0.4/httpauth.egg-info/dependency_links.txt
--rw-r--r--   0 j          (501) wheel        (0)        9 2024-05-21 12:05:19.000000 httpauth-0.4/httpauth.egg-info/top_level.txt
--rw-r--r--   0 j          (501) wheel        (0)     6788 2024-05-21 12:03:58.000000 httpauth-0.4/httpauth.py
--rw-r--r--   0 j          (501) wheel        (0)       38 2024-05-21 12:05:19.227668 httpauth-0.4/setup.cfg
--rw-r--r--   0 j          (501) wheel        (0)      522 2024-05-21 12:05:13.000000 httpauth-0.4/setup.py
+drwxr-xr-x   0 j          (501) wheel        (0)        0 2024-05-29 09:46:59.965852 httpauth-0.4.1/
+-rw-r--r--   0 j          (501) wheel        (0)      748 2024-05-29 09:43:29.000000 httpauth-0.4.1/LICENSE
+-rw-r--r--   0 j          (501) wheel        (0)       42 2024-05-29 09:43:29.000000 httpauth-0.4.1/MANIFEST.in
+-rw-r--r--   0 j          (501) wheel        (0)       18 2024-05-29 09:43:29.000000 httpauth-0.4.1/Makefile
+-rw-r--r--   0 j          (501) wheel        (0)      436 2024-05-29 09:46:59.965705 httpauth-0.4.1/PKG-INFO
+-rw-r--r--   0 j          (501) wheel        (0)     1197 2024-05-29 09:43:29.000000 httpauth-0.4.1/README.rst
+drwxr-xr-x   0 j          (501) wheel        (0)        0 2024-05-29 09:46:59.965556 httpauth-0.4.1/httpauth.egg-info/
+-rw-r--r--   0 j          (501) wheel        (0)      436 2024-05-29 09:46:59.000000 httpauth-0.4.1/httpauth.egg-info/PKG-INFO
+-rw-r--r--   0 j          (501) wheel        (0)      205 2024-05-29 09:46:59.000000 httpauth-0.4.1/httpauth.egg-info/SOURCES.txt
+-rw-r--r--   0 j          (501) wheel        (0)        1 2024-05-29 09:46:59.000000 httpauth-0.4.1/httpauth.egg-info/dependency_links.txt
+-rw-r--r--   0 j          (501) wheel        (0)        9 2024-05-29 09:46:59.000000 httpauth-0.4.1/httpauth.egg-info/top_level.txt
+-rw-r--r--   0 j          (501) wheel        (0)     6788 2024-05-29 09:43:29.000000 httpauth-0.4.1/httpauth.py
+-rw-r--r--   0 j          (501) wheel        (0)       38 2024-05-29 09:46:59.965883 httpauth-0.4.1/setup.cfg
+-rw-r--r--   0 j          (501) wheel        (0)      524 2024-05-29 09:46:24.000000 httpauth-0.4.1/setup.py
+-rw-r--r--   0 j          (501) wheel        (0)     4324 2024-05-29 09:43:29.000000 httpauth-0.4.1/test_httpauth.py
```

### Comparing `httpauth-0.4/LICENSE` & `httpauth-0.4.1/LICENSE`

 * *Files identical despite different names*

### Comparing `httpauth-0.4/README.rst` & `httpauth-0.4.1/README.rst`

 * *Files identical despite different names*

### Comparing `httpauth-0.4/httpauth.py` & `httpauth-0.4.1/httpauth.py`

 * *Files identical despite different names*

### Comparing `httpauth-0.4/setup.py` & `httpauth-0.4.1/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from distutils.core import setup
 
 setup(
     name='httpauth',
-    version='0.4',
+    version='0.4.1',
     author='Jonas Haag',
     author_email='jonas@lophus.org',
     url='https://github.com/jonashaag/httpauth',
     license='2-clause BSD',
     description="WSGI HTTP Digest Authentication middleware",
     py_modules=['httpauth'],
     classifiers=[
```

