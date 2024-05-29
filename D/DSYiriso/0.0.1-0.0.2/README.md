# Comparing `tmp/DSYiriso-0.0.1.tar.gz` & `tmp/DSYiriso-0.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "DSYiriso-0.0.1.tar", last modified: Wed May 29 05:04:40 2024, max compression
+gzip compressed data, was "DSYiriso-0.0.2.tar", last modified: Wed May 29 10:28:39 2024, max compression
```

## Comparing `DSYiriso-0.0.1.tar` & `DSYiriso-0.0.2.tar`

### file list

```diff
@@ -1,12 +1,12 @@
-drwxrwxrwx   0        0        0        0 2024-05-29 05:04:40.621578 DSYiriso-0.0.1/
-drwxrwxrwx   0        0        0        0 2024-05-29 05:04:40.614215 DSYiriso-0.0.1/DSYiriso.egg-info/
--rw-rw-rw-   0        0        0      429 2024-05-29 05:04:40.000000 DSYiriso-0.0.1/DSYiriso.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      159 2024-05-29 05:04:40.000000 DSYiriso-0.0.1/DSYiriso.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-05-29 05:04:40.000000 DSYiriso-0.0.1/DSYiriso.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0        1 2024-05-29 05:04:40.000000 DSYiriso-0.0.1/DSYiriso.egg-info/top_level.txt
--rw-rw-rw-   0        0        0      429 2024-05-29 05:04:40.620445 DSYiriso-0.0.1/PKG-INFO
--rw-rw-rw-   0        0        0       13 2024-05-28 13:33:46.000000 DSYiriso-0.0.1/README.md
--rw-rw-rw-   0        0        0       42 2024-05-29 05:04:40.621578 DSYiriso-0.0.1/setup.cfg
--rw-rw-rw-   0        0        0      819 2024-05-29 05:03:40.000000 DSYiriso-0.0.1/setup.py
-drwxrwxrwx   0        0        0        0 2024-05-29 05:04:40.617209 DSYiriso-0.0.1/test/
--rw-rw-rw-   0        0        0       26 2024-05-29 04:45:05.000000 DSYiriso-0.0.1/test/test.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-29 10:28:39.382349 DSYiriso-0.0.2/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-29 10:28:39.382349 DSYiriso-0.0.2/DSYiriso.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)      462 2024-05-29 10:28:39.000000 DSYiriso-0.0.2/DSYiriso.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      159 2024-05-29 10:28:39.000000 DSYiriso-0.0.2/DSYiriso.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-29 10:28:39.000000 DSYiriso-0.0.2/DSYiriso.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-29 10:28:39.000000 DSYiriso-0.0.2/DSYiriso.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      462 2024-05-29 10:28:39.382349 DSYiriso-0.0.2/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)       13 2024-05-29 10:28:34.000000 DSYiriso-0.0.2/README.md
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-29 10:28:39.382349 DSYiriso-0.0.2/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)      791 2024-05-29 10:28:34.000000 DSYiriso-0.0.2/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-29 10:28:39.382349 DSYiriso-0.0.2/test/
+-rw-r--r--   0 runner    (1001) docker     (127)       24 2024-05-29 10:28:34.000000 DSYiriso-0.0.2/test/test.py
```

### Comparing `DSYiriso-0.0.1/setup.py` & `DSYiriso-0.0.2/setup.py`

 * *Files 22% similar despite different names*

```diff
@@ -1,29 +1,29 @@
-import setuptools
-
-with open("README.md", "r", encoding='utf-8') as fh:
-    long_description = fh.read()
-
-
-setuptools.setup(
-    name="DSYiriso",
-    version="0.0.1",
-    author="yichi zhang",
-    author_email="kszyc1001@163.com",
-    description="Data structure in python.",
-    long_description=long_description,
-    long_description_content_type="text/markdown",
-    url="https://github.com/Yirios/Data-Structure", 
-    packages=setuptools.find_packages(),
-    classifiers=[
-        "Programming Language :: Python :: 3",
-        "License :: OSI Approved :: MIT License",  
-        "Operating System :: OS Independent",
-    ],
-    python_requires='>=3.8'
-)
-
-#   python setup.py sdist build
-#   twine upload dist/*  
-
-#   git tag [new version] -m "detail"
+import setuptools
+
+with open("README.md", "r", encoding='utf-8') as fh:
+    long_description = fh.read()
+
+
+setuptools.setup(
+    name="DSYiriso",
+    version="0.0.2",
+    author="yichi zhang",
+    author_email="kszyc1001@163.com",
+    description="Data structure in python.",
+    long_description=long_description,
+    long_description_content_type="text/markdown",
+    url="https://github.com/Yirios/Data-Structure", 
+    packages=setuptools.find_packages(),
+    classifiers=[
+        "Programming Language :: Python :: 3",
+        "License :: OSI Approved :: MIT License",  
+        "Operating System :: OS Independent",
+    ],
+    python_requires='>=3.8'
+)
+
+#   python setup.py sdist build
+#   twine upload dist/*  
+
+#   git tag [new version] -m "detail"
 #   git push origin [new version]
```

