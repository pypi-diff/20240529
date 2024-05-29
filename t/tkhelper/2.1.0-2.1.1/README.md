# Comparing `tmp/tkhelper-2.1.0.tar.gz` & `tmp/tkhelper-2.1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "tkhelper-2.1.0.tar", last modified: Mon Aug 14 11:11:44 2023, max compression
+gzip compressed data, was "tkhelper-2.1.1.tar", last modified: Wed May 29 10:55:18 2024, max compression
```

## Comparing `tkhelper-2.1.0.tar` & `tkhelper-2.1.1.tar`

### file list

```diff
@@ -1,23 +1,23 @@
-drwxrwxrwx   0        0        0        0 2023-08-14 11:11:44.356739 tkhelper-2.1.0/
--rw-rw-rw-   0        0        0     1071 2020-06-24 20:49:09.000000 tkhelper-2.1.0/LICENSE
--rw-rw-rw-   0        0        0     2456 2023-08-14 11:11:44.355726 tkhelper-2.1.0/PKG-INFO
--rw-rw-rw-   0        0        0     1902 2020-07-12 19:11:23.000000 tkhelper-2.1.0/README.md
--rw-rw-rw-   0        0        0     1335 2023-08-14 11:09:18.000000 tkhelper-2.1.0/pyproject.toml
--rw-rw-rw-   0        0        0       31 2023-08-06 09:22:40.000000 tkhelper-2.1.0/requirements.txt
--rw-rw-rw-   0        0        0       42 2023-08-14 11:11:44.356739 tkhelper-2.1.0/setup.cfg
-drwxrwxrwx   0        0        0        0 2023-08-14 11:11:44.333725 tkhelper-2.1.0/tests/
--rw-rw-rw-   0        0        0        0 2020-07-12 18:07:26.000000 tkhelper-2.1.0/tests/tests.py
-drwxrwxrwx   0        0        0        0 2023-08-14 11:11:44.337727 tkhelper-2.1.0/tkhelper/
--rw-rw-rw-   0        0        0        0 2020-07-12 15:55:13.000000 tkhelper-2.1.0/tkhelper/__init__.py
--rw-rw-rw-   0        0        0      116 2023-08-14 11:11:09.000000 tkhelper-2.1.0/tkhelper/package_info.py
-drwxrwxrwx   0        0        0        0 2023-08-14 11:11:44.353726 tkhelper-2.1.0/tkhelper/progressbars/
--rw-rw-rw-   0        0        0        0 2023-08-04 13:17:26.000000 tkhelper-2.1.0/tkhelper/progressbars/__init__.py
--rw-rw-rw-   0        0        0    39844 2023-08-08 06:42:14.000000 tkhelper-2.1.0/tkhelper/progressbars/circular.py
--rw-rw-rw-   0        0        0       70 2023-08-11 09:09:28.000000 tkhelper-2.1.0/tkhelper/py.typed
--rw-rw-rw-   0        0        0    50061 2023-08-14 06:00:45.000000 tkhelper-2.1.0/tkhelper/widgets.py
-drwxrwxrwx   0        0        0        0 2023-08-14 11:11:44.351726 tkhelper-2.1.0/tkhelper.egg-info/
--rw-rw-rw-   0        0        0     2456 2023-08-14 11:11:44.000000 tkhelper-2.1.0/tkhelper.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      375 2023-08-14 11:11:44.000000 tkhelper-2.1.0/tkhelper.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-08-14 11:11:44.000000 tkhelper-2.1.0/tkhelper.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       29 2023-08-14 11:11:44.000000 tkhelper-2.1.0/tkhelper.egg-info/requires.txt
--rw-rw-rw-   0        0        0        9 2023-08-14 11:11:44.000000 tkhelper-2.1.0/tkhelper.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2024-05-29 10:55:18.812788 tkhelper-2.1.1/
+-rw-rw-rw-   0        0        0     1092 2024-05-29 10:42:39.000000 tkhelper-2.1.1/LICENSE
+-rw-rw-rw-   0        0        0     2517 2024-05-29 10:55:18.809788 tkhelper-2.1.1/PKG-INFO
+-rw-rw-rw-   0        0        0     1902 2024-05-29 10:42:39.000000 tkhelper-2.1.1/README.md
+-rw-rw-rw-   0        0        0     1335 2024-05-29 10:42:39.000000 tkhelper-2.1.1/pyproject.toml
+-rw-rw-rw-   0        0        0       31 2024-05-29 10:48:41.000000 tkhelper-2.1.1/requirements.txt
+-rw-rw-rw-   0        0        0       42 2024-05-29 10:55:18.813786 tkhelper-2.1.1/setup.cfg
+drwxrwxrwx   0        0        0        0 2024-05-29 10:55:18.740592 tkhelper-2.1.1/tests/
+-rw-rw-rw-   0        0        0        0 2024-05-29 10:42:39.000000 tkhelper-2.1.1/tests/tests.py
+drwxrwxrwx   0        0        0        0 2024-05-29 10:55:18.750591 tkhelper-2.1.1/tkhelper/
+-rw-rw-rw-   0        0        0        0 2024-05-29 10:42:39.000000 tkhelper-2.1.1/tkhelper/__init__.py
+-rw-rw-rw-   0        0        0      116 2024-05-29 10:51:54.000000 tkhelper-2.1.1/tkhelper/package_info.py
+drwxrwxrwx   0        0        0        0 2024-05-29 10:55:18.801787 tkhelper-2.1.1/tkhelper/progressbars/
+-rw-rw-rw-   0        0        0        0 2024-05-29 10:42:39.000000 tkhelper-2.1.1/tkhelper/progressbars/__init__.py
+-rw-rw-rw-   0        0        0    39844 2024-05-29 10:42:39.000000 tkhelper-2.1.1/tkhelper/progressbars/circular.py
+-rw-rw-rw-   0        0        0       70 2024-05-29 10:42:39.000000 tkhelper-2.1.1/tkhelper/py.typed
+-rw-rw-rw-   0        0        0    50061 2024-05-29 10:42:39.000000 tkhelper-2.1.1/tkhelper/widgets.py
+drwxrwxrwx   0        0        0        0 2024-05-29 10:55:18.805789 tkhelper-2.1.1/tkhelper.egg-info/
+-rw-rw-rw-   0        0        0     2517 2024-05-29 10:55:18.000000 tkhelper-2.1.1/tkhelper.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      375 2024-05-29 10:55:18.000000 tkhelper-2.1.1/tkhelper.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-05-29 10:55:18.000000 tkhelper-2.1.1/tkhelper.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       29 2024-05-29 10:55:18.000000 tkhelper-2.1.1/tkhelper.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        9 2024-05-29 10:55:18.000000 tkhelper-2.1.1/tkhelper.egg-info/top_level.txt
```

### Comparing `tkhelper-2.1.0/PKG-INFO` & `tkhelper-2.1.1/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,20 +1,22 @@
 Metadata-Version: 2.1
 Name: tkhelper
-Version: 2.1.0
+Version: 2.1.1
 Summary: A module to display some customized tkinter modules
 Author-email: Erdogan Onal <erdoganonal@windowslive.com>
 Project-URL: Homepage, https://github.com/erdoganonal/tk_helper
 Project-URL: Bug Tracker, https://github.com/erdoganonal/tk_helper/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.6
 Description-Content-Type: text/markdown
 License-File: LICENSE
+Requires-Dist: colour>=0.1.5
+Requires-Dist: pillow>=10.3.0
 
 # Tkinter Helper
 
 A module to display some customized tkinter modules.
 
 ## Getting Started
```

### Comparing `tkhelper-2.1.0/README.md` & `tkhelper-2.1.1/README.md`

 * *Files identical despite different names*

### Comparing `tkhelper-2.1.0/pyproject.toml` & `tkhelper-2.1.1/pyproject.toml`

 * *Files identical despite different names*

### Comparing `tkhelper-2.1.0/tkhelper/progressbars/circular.py` & `tkhelper-2.1.1/tkhelper/progressbars/circular.py`

 * *Files identical despite different names*

### Comparing `tkhelper-2.1.0/tkhelper/widgets.py` & `tkhelper-2.1.1/tkhelper/widgets.py`

 * *Files identical despite different names*

### Comparing `tkhelper-2.1.0/tkhelper.egg-info/PKG-INFO` & `tkhelper-2.1.1/tkhelper.egg-info/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,20 +1,22 @@
 Metadata-Version: 2.1
 Name: tkhelper
-Version: 2.1.0
+Version: 2.1.1
 Summary: A module to display some customized tkinter modules
 Author-email: Erdogan Onal <erdoganonal@windowslive.com>
 Project-URL: Homepage, https://github.com/erdoganonal/tk_helper
 Project-URL: Bug Tracker, https://github.com/erdoganonal/tk_helper/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.6
 Description-Content-Type: text/markdown
 License-File: LICENSE
+Requires-Dist: colour>=0.1.5
+Requires-Dist: pillow>=10.3.0
 
 # Tkinter Helper
 
 A module to display some customized tkinter modules.
 
 ## Getting Started
```

