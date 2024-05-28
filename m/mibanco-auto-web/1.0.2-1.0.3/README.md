# Comparing `tmp/mibanco_auto_web-1.0.2.tar.gz` & `tmp/mibanco_auto_web-1.0.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "mibanco_auto_web-1.0.2.tar", last modified: Thu May 23 16:43:08 2024, max compression
+gzip compressed data, was "mibanco_auto_web-1.0.3.tar", last modified: Tue May 28 22:24:32 2024, max compression
```

## Comparing `mibanco_auto_web-1.0.2.tar` & `mibanco_auto_web-1.0.3.tar`

### file list

```diff
@@ -1,18 +1,18 @@
-drwxrwxrwx   0        0        0        0 2024-05-23 16:43:08.875437 mibanco_auto_web-1.0.2/
--rw-rw-rw-   0        0        0       46 2024-05-21 20:44:35.000000 mibanco_auto_web-1.0.2/MANIFEST.in
--rw-rw-rw-   0        0        0     3439 2024-05-23 16:43:08.875437 mibanco_auto_web-1.0.2/PKG-INFO
--rw-rw-rw-   0        0        0     2364 2024-05-23 16:28:02.000000 mibanco_auto_web-1.0.2/README.md
-drwxrwxrwx   0        0        0        0 2024-05-23 16:43:08.867915 mibanco_auto_web-1.0.2/mibanco_auto_web/
--rw-rw-rw-   0        0        0       63 2024-05-21 20:44:35.000000 mibanco_auto_web-1.0.2/mibanco_auto_web/__init__.py
--rw-rw-rw-   0        0        0     4936 2024-05-23 16:33:38.000000 mibanco_auto_web-1.0.2/mibanco_auto_web/functions.py
--rw-rw-rw-   0        0        0     1798 2024-05-23 16:22:52.000000 mibanco_auto_web-1.0.2/mibanco_auto_web/main.py
--rw-rw-rw-   0        0        0      102 2024-05-23 16:43:00.000000 mibanco_auto_web-1.0.2/mibanco_auto_web/variables.py
-drwxrwxrwx   0        0        0        0 2024-05-23 16:43:08.875437 mibanco_auto_web-1.0.2/mibanco_auto_web.egg-info/
--rw-rw-rw-   0        0        0     3439 2024-05-23 16:43:08.000000 mibanco_auto_web-1.0.2/mibanco_auto_web.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      386 2024-05-23 16:43:08.000000 mibanco_auto_web-1.0.2/mibanco_auto_web.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-05-23 16:43:08.000000 mibanco_auto_web-1.0.2/mibanco_auto_web.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       64 2024-05-23 16:43:08.000000 mibanco_auto_web-1.0.2/mibanco_auto_web.egg-info/entry_points.txt
--rw-rw-rw-   0        0        0      338 2024-05-23 16:43:08.000000 mibanco_auto_web-1.0.2/mibanco_auto_web.egg-info/requires.txt
--rw-rw-rw-   0        0        0       17 2024-05-23 16:43:08.000000 mibanco_auto_web-1.0.2/mibanco_auto_web.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2024-05-23 16:43:08.875437 mibanco_auto_web-1.0.2/setup.cfg
--rw-rw-rw-   0        0        0     1609 2024-05-21 20:47:45.000000 mibanco_auto_web-1.0.2/setup.py
+drwxrwxrwx   0        0        0        0 2024-05-28 22:24:32.550756 mibanco_auto_web-1.0.3/
+-rw-rw-rw-   0        0        0       46 2024-05-21 20:44:35.000000 mibanco_auto_web-1.0.3/MANIFEST.in
+-rw-rw-rw-   0        0        0     3439 2024-05-28 22:24:32.548099 mibanco_auto_web-1.0.3/PKG-INFO
+-rw-rw-rw-   0        0        0     2364 2024-05-23 16:28:02.000000 mibanco_auto_web-1.0.3/README.md
+drwxrwxrwx   0        0        0        0 2024-05-28 22:24:32.533920 mibanco_auto_web-1.0.3/mibanco_auto_web/
+-rw-rw-rw-   0        0        0       63 2024-05-21 20:44:35.000000 mibanco_auto_web-1.0.3/mibanco_auto_web/__init__.py
+-rw-rw-rw-   0        0        0     4936 2024-05-23 16:33:38.000000 mibanco_auto_web-1.0.3/mibanco_auto_web/functions.py
+-rw-rw-rw-   0        0        0     1798 2024-05-23 16:22:52.000000 mibanco_auto_web-1.0.3/mibanco_auto_web/main.py
+-rw-rw-rw-   0        0        0      102 2024-05-28 22:22:12.000000 mibanco_auto_web-1.0.3/mibanco_auto_web/variables.py
+drwxrwxrwx   0        0        0        0 2024-05-28 22:24:32.542564 mibanco_auto_web-1.0.3/mibanco_auto_web.egg-info/
+-rw-rw-rw-   0        0        0     3439 2024-05-28 22:24:32.000000 mibanco_auto_web-1.0.3/mibanco_auto_web.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      386 2024-05-28 22:24:32.000000 mibanco_auto_web-1.0.3/mibanco_auto_web.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-05-28 22:24:32.000000 mibanco_auto_web-1.0.3/mibanco_auto_web.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       64 2024-05-28 22:24:32.000000 mibanco_auto_web-1.0.3/mibanco_auto_web.egg-info/entry_points.txt
+-rw-rw-rw-   0        0        0      338 2024-05-28 22:24:32.000000 mibanco_auto_web-1.0.3/mibanco_auto_web.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       17 2024-05-28 22:24:32.000000 mibanco_auto_web-1.0.3/mibanco_auto_web.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2024-05-28 22:24:32.550756 mibanco_auto_web-1.0.3/setup.cfg
+-rw-rw-rw-   0        0        0     1609 2024-05-28 22:20:59.000000 mibanco_auto_web-1.0.3/setup.py
```

### Comparing `mibanco_auto_web-1.0.2/PKG-INFO` & `mibanco_auto_web-1.0.3/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: mibanco_auto_web
-Version: 1.0.2
+Version: 1.0.3
 Summary: A simple functional test library using Python and Selenium
 Author: Automation & Performance Team
 Keywords: selenium,testing,web,chrome
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3.12
@@ -13,15 +13,15 @@
 Requires-Dist: allure-python-commons==2.13.5
 Requires-Dist: behave==1.2.6
 Requires-Dist: behave-html-formatter==0.9.10
 Requires-Dist: behave2cucumber==1.0.3
 Requires-Dist: docxcompose==1.4.0
 Requires-Dist: docxtpl==0.16.8
 Requires-Dist: playwright==1.42.0
-Requires-Dist: psutil==5.9.2
+Requires-Dist: psutil==5.9.8
 Requires-Dist: pillow==10.3.0
 Requires-Dist: openpyxl==3.1.2
 Requires-Dist: customtkinter==5.2.2
 Requires-Dist: PyPDF2==3.0.1
 Requires-Dist: python-docx==1.1.0
 Requires-Dist: pycparser==2.21
 Requires-Dist: screeninfo==0.8
```

### Comparing `mibanco_auto_web-1.0.2/README.md` & `mibanco_auto_web-1.0.3/README.md`

 * *Files identical despite different names*

### Comparing `mibanco_auto_web-1.0.2/mibanco_auto_web/functions.py` & `mibanco_auto_web-1.0.3/mibanco_auto_web/functions.py`

 * *Files identical despite different names*

### Comparing `mibanco_auto_web-1.0.2/mibanco_auto_web/main.py` & `mibanco_auto_web-1.0.3/mibanco_auto_web/main.py`

 * *Files identical despite different names*

### Comparing `mibanco_auto_web-1.0.2/mibanco_auto_web.egg-info/PKG-INFO` & `mibanco_auto_web-1.0.3/mibanco_auto_web.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: mibanco_auto_web
-Version: 1.0.2
+Version: 1.0.3
 Summary: A simple functional test library using Python and Selenium
 Author: Automation & Performance Team
 Keywords: selenium,testing,web,chrome
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3.12
@@ -13,15 +13,15 @@
 Requires-Dist: allure-python-commons==2.13.5
 Requires-Dist: behave==1.2.6
 Requires-Dist: behave-html-formatter==0.9.10
 Requires-Dist: behave2cucumber==1.0.3
 Requires-Dist: docxcompose==1.4.0
 Requires-Dist: docxtpl==0.16.8
 Requires-Dist: playwright==1.42.0
-Requires-Dist: psutil==5.9.2
+Requires-Dist: psutil==5.9.8
 Requires-Dist: pillow==10.3.0
 Requires-Dist: openpyxl==3.1.2
 Requires-Dist: customtkinter==5.2.2
 Requires-Dist: PyPDF2==3.0.1
 Requires-Dist: python-docx==1.1.0
 Requires-Dist: pycparser==2.21
 Requires-Dist: screeninfo==0.8
```

### Comparing `mibanco_auto_web-1.0.2/setup.py` & `mibanco_auto_web-1.0.3/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -17,15 +17,15 @@
         "allure-python-commons==2.13.5",
         "behave==1.2.6",
         "behave-html-formatter==0.9.10",
         "behave2cucumber==1.0.3",
         "docxcompose==1.4.0",
         "docxtpl==0.16.8",
         "playwright==1.42.0",
-        "psutil==5.9.2",
+        "psutil==5.9.8",
         "pillow==10.3.0",
         "openpyxl==3.1.2",
         "customtkinter==5.2.2",
         "PyPDF2==3.0.1",
         "python-docx==1.1.0",
         "pycparser==2.21",
         "screeninfo==0.8",
```

