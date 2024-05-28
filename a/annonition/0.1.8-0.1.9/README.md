# Comparing `tmp/annonition-0.1.8.tar.gz` & `tmp/annonition-0.1.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "annonition-0.1.8.tar", last modified: Mon May 27 19:59:50 2024, max compression
+gzip compressed data, was "annonition-0.1.9.tar", last modified: Mon May 27 20:00:32 2024, max compression
```

## Comparing `annonition-0.1.8.tar` & `annonition-0.1.9.tar`

### file list

```diff
@@ -1,16 +1,16 @@
-drwxrwxrwx   0        0        0        0 2024-05-27 19:59:50.570000 annonition-0.1.8/
--rw-rw-rw-   0        0        0     1089 2024-05-26 00:32:06.000000 annonition-0.1.8/LICENSE
--rw-rw-rw-   0        0        0     5532 2024-05-27 19:59:52.000000 annonition-0.1.8/PKG-INFO
--rw-rw-rw-   0        0        0     5122 2024-05-27 18:45:58.000000 annonition-0.1.8/README.md
-drwxrwxrwx   0        0        0        0 2024-05-27 19:59:50.590000 annonition-0.1.8/annonition/
--rw-rw-rw-   0        0        0       93 2024-05-26 00:15:56.000000 annonition-0.1.8/annonition/__init__.py
--rw-rw-rw-   0        0        0    12145 2024-05-27 19:59:14.000000 annonition-0.1.8/annonition/logger.py
--rw-rw-rw-   0        0        0      113 2024-05-26 00:15:48.000000 annonition-0.1.8/annonition/main.py
-drwxrwxrwx   0        0        0        0 2024-05-27 19:59:50.610000 annonition-0.1.8/annonition.egg-info/
--rw-rw-rw-   0        0        0     5532 2024-05-27 19:59:52.000000 annonition-0.1.8/annonition.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      258 2024-05-27 19:59:52.000000 annonition-0.1.8/annonition.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-05-27 19:59:52.000000 annonition-0.1.8/annonition.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       31 2024-05-27 19:59:52.000000 annonition-0.1.8/annonition.egg-info/requires.txt
--rw-rw-rw-   0        0        0       11 2024-05-27 19:59:52.000000 annonition-0.1.8/annonition.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2024-05-27 19:59:52.000000 annonition-0.1.8/setup.cfg
--rw-rw-rw-   0        0        0      750 2024-05-27 19:53:30.000000 annonition-0.1.8/setup.py
+drwxrwxrwx   0        0        0        0 2024-05-27 20:00:32.380000 annonition-0.1.9/
+-rw-rw-rw-   0        0        0     1089 2024-05-26 00:32:06.000000 annonition-0.1.9/LICENSE
+-rw-rw-rw-   0        0        0     5532 2024-05-27 20:00:34.000000 annonition-0.1.9/PKG-INFO
+-rw-rw-rw-   0        0        0     5122 2024-05-27 18:45:58.000000 annonition-0.1.9/README.md
+drwxrwxrwx   0        0        0        0 2024-05-27 20:00:32.400000 annonition-0.1.9/annonition/
+-rw-rw-rw-   0        0        0       93 2024-05-26 00:15:56.000000 annonition-0.1.9/annonition/__init__.py
+-rw-rw-rw-   0        0        0    12145 2024-05-27 19:59:14.000000 annonition-0.1.9/annonition/logger.py
+-rw-rw-rw-   0        0        0      113 2024-05-26 00:15:48.000000 annonition-0.1.9/annonition/main.py
+drwxrwxrwx   0        0        0        0 2024-05-27 20:00:32.420000 annonition-0.1.9/annonition.egg-info/
+-rw-rw-rw-   0        0        0     5532 2024-05-27 20:00:34.000000 annonition-0.1.9/annonition.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      258 2024-05-27 20:00:34.000000 annonition-0.1.9/annonition.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-05-27 20:00:34.000000 annonition-0.1.9/annonition.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       31 2024-05-27 20:00:34.000000 annonition-0.1.9/annonition.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       11 2024-05-27 20:00:34.000000 annonition-0.1.9/annonition.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2024-05-27 20:00:34.000000 annonition-0.1.9/setup.cfg
+-rw-rw-rw-   0        0        0      750 2024-05-27 20:00:22.000000 annonition-0.1.9/setup.py
```

### Comparing `annonition-0.1.8/LICENSE` & `annonition-0.1.9/LICENSE`

 * *Files identical despite different names*

### Comparing `annonition-0.1.8/PKG-INFO` & `annonition-0.1.9/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: annonition
-Version: 0.1.8
+Version: 0.1.9
 Summary: Log everything in style.
 Author: Abtin Turing
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Description-Content-Type: text/markdown
 License-File: LICENSE
```

### Comparing `annonition-0.1.8/README.md` & `annonition-0.1.9/README.md`

 * *Files identical despite different names*

### Comparing `annonition-0.1.8/annonition/logger.py` & `annonition-0.1.9/annonition/logger.py`

 * *Files identical despite different names*

### Comparing `annonition-0.1.8/annonition.egg-info/PKG-INFO` & `annonition-0.1.9/annonition.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: annonition
-Version: 0.1.8
+Version: 0.1.9
 Summary: Log everything in style.
 Author: Abtin Turing
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Description-Content-Type: text/markdown
 License-File: LICENSE
```

### Comparing `annonition-0.1.8/setup.py` & `annonition-0.1.9/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -4,15 +4,15 @@
 
 with open(path.join(working_dir, "README.md"), encoding="utf-8") as f:
     long_description = f.read()
 
 
 setup(
     name="annonition",
-    version="0.1.8",
+    version="0.1.9",
     author="Abtin Turing",
     description="Log everything in style.",
     long_description=long_description,
     long_description_content_type="text/markdown",
     packages=find_packages(),
     classifiers=[
         "Programming Language :: Python :: 3",
```

