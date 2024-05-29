# Comparing `tmp/medium_article_py-0.1.8.tar.gz` & `tmp/medium_article_py-0.1.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "medium_article_py-0.1.8.tar", last modified: Tue May 28 12:30:44 2024, max compression
+gzip compressed data, was "medium_article_py-0.1.9.tar", last modified: Tue May 28 14:04:31 2024, max compression
```

## Comparing `medium_article_py-0.1.8.tar` & `medium_article_py-0.1.9.tar`

### file list

```diff
@@ -1,16 +1,16 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-28 12:30:44.142281 medium_article_py-0.1.8/
--rw-r--r--   0 runner    (1001) docker     (127)     1071 2024-05-28 12:30:30.000000 medium_article_py-0.1.8/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)     2428 2024-05-28 12:30:44.142281 medium_article_py-0.1.8/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     1911 2024-05-28 12:30:30.000000 medium_article_py-0.1.8/README.rst
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-28 12:30:44.142281 medium_article_py-0.1.8/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)      814 2024-05-28 12:30:30.000000 medium_article_py-0.1.8/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-28 12:30:44.142281 medium_article_py-0.1.8/src/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-28 12:30:44.142281 medium_article_py-0.1.8/src/medium_article_py/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-28 12:30:30.000000 medium_article_py-0.1.8/src/medium_article_py/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     6019 2024-05-28 12:30:30.000000 medium_article_py-0.1.8/src/medium_article_py/medium.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-28 12:30:44.142281 medium_article_py-0.1.8/src/medium_article_py.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     2428 2024-05-28 12:30:44.000000 medium_article_py-0.1.8/src/medium_article_py.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      317 2024-05-28 12:30:44.000000 medium_article_py-0.1.8/src/medium_article_py.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-28 12:30:44.000000 medium_article_py-0.1.8/src/medium_article_py.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)        9 2024-05-28 12:30:44.000000 medium_article_py-0.1.8/src/medium_article_py.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       18 2024-05-28 12:30:44.000000 medium_article_py-0.1.8/src/medium_article_py.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-28 14:04:31.499418 medium_article_py-0.1.9/
+-rw-r--r--   0 runner    (1001) docker     (127)     1071 2024-05-28 14:04:26.000000 medium_article_py-0.1.9/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)     2452 2024-05-28 14:04:31.499418 medium_article_py-0.1.9/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     1935 2024-05-28 14:04:26.000000 medium_article_py-0.1.9/README.rst
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-28 14:04:31.499418 medium_article_py-0.1.9/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)      814 2024-05-28 14:04:26.000000 medium_article_py-0.1.9/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-28 14:04:31.499418 medium_article_py-0.1.9/src/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-28 14:04:31.499418 medium_article_py-0.1.9/src/medium_article_py/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-28 14:04:26.000000 medium_article_py-0.1.9/src/medium_article_py/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6019 2024-05-28 14:04:26.000000 medium_article_py-0.1.9/src/medium_article_py/medium.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-28 14:04:31.499418 medium_article_py-0.1.9/src/medium_article_py.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     2452 2024-05-28 14:04:31.000000 medium_article_py-0.1.9/src/medium_article_py.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      317 2024-05-28 14:04:31.000000 medium_article_py-0.1.9/src/medium_article_py.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-28 14:04:31.000000 medium_article_py-0.1.9/src/medium_article_py.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        9 2024-05-28 14:04:31.000000 medium_article_py-0.1.9/src/medium_article_py.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       18 2024-05-28 14:04:31.000000 medium_article_py-0.1.9/src/medium_article_py.egg-info/top_level.txt
```

### Comparing `medium_article_py-0.1.8/LICENSE` & `medium_article_py-0.1.9/LICENSE`

 * *Files identical despite different names*

### Comparing `medium_article_py-0.1.8/PKG-INFO` & `medium_article_py-0.1.9/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: medium-article-py
-Version: 0.1.8
+Version: 0.1.9
 Summary: A simple python library for Medium Articles APIs
 Download-URL: https://github.com/muhammad-usman-108/medium-article-py.git
 Author: Muhammad Usman
 Author-email: umuhammad202@yahoo.com
 Keywords: medium,medium-api,medium-article,api
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
@@ -32,18 +32,20 @@
 Usage
 ------------
 
 Here is a simple example to get you started:
 
 .. code-block:: python
 
-    from medium-article-py import MediumArticles
+    from medium_article_py.medium import MediumArticles
+    
     username = '<your-medium-username>'
+    md = MediumArticles()
 
-    print(MediumArticles.get_profile_url(username))      
+    print(md.get_profile_url(username))    
     # Output: https://medium.com/feed/@engrmuhammadusman108
 
 .. list-table::
    :widths: 20 80 20
    :header-rows: 1
 
    * - Function
```

### Comparing `medium_article_py-0.1.8/README.rst` & `medium_article_py-0.1.9/README.rst`

 * *Files 5% similar despite different names*

```diff
@@ -17,18 +17,20 @@
 Usage
 ------------
 
 Here is a simple example to get you started:
 
 .. code-block:: python
 
-    from medium-article-py import MediumArticles
+    from medium_article_py.medium import MediumArticles
+    
     username = '<your-medium-username>'
+    md = MediumArticles()
 
-    print(MediumArticles.get_profile_url(username))      
+    print(md.get_profile_url(username))    
     # Output: https://medium.com/feed/@engrmuhammadusman108
 
 .. list-table::
    :widths: 20 80 20
    :header-rows: 1
 
    * - Function
```

### Comparing `medium_article_py-0.1.8/setup.py` & `medium_article_py-0.1.9/setup.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 import setuptools
 
 with open("README.rst", "r", encoding="utf-8") as fh:
     long_description = fh.read()
 
 setuptools.setup(
     name='medium-article-py',
-    version='v0.1.8',
+    version='v0.1.9',
     description='A simple python library for Medium Articles APIs',
     long_description=long_description,
     author='Muhammad Usman',
     author_email='umuhammad202@yahoo.com',
     packages=setuptools.find_packages(where='src'),
     package_dir={'': 'src'},
     classifiers=[
```

### Comparing `medium_article_py-0.1.8/src/medium_article_py/medium.py` & `medium_article_py-0.1.9/src/medium_article_py/medium.py`

 * *Files identical despite different names*

### Comparing `medium_article_py-0.1.8/src/medium_article_py.egg-info/PKG-INFO` & `medium_article_py-0.1.9/src/medium_article_py.egg-info/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: medium-article-py
-Version: 0.1.8
+Version: 0.1.9
 Summary: A simple python library for Medium Articles APIs
 Download-URL: https://github.com/muhammad-usman-108/medium-article-py.git
 Author: Muhammad Usman
 Author-email: umuhammad202@yahoo.com
 Keywords: medium,medium-api,medium-article,api
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
@@ -32,18 +32,20 @@
 Usage
 ------------
 
 Here is a simple example to get you started:
 
 .. code-block:: python
 
-    from medium-article-py import MediumArticles
+    from medium_article_py.medium import MediumArticles
+    
     username = '<your-medium-username>'
+    md = MediumArticles()
 
-    print(MediumArticles.get_profile_url(username))      
+    print(md.get_profile_url(username))    
     # Output: https://medium.com/feed/@engrmuhammadusman108
 
 .. list-table::
    :widths: 20 80 20
    :header-rows: 1
 
    * - Function
```

