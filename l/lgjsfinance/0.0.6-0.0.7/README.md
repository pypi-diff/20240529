# Comparing `tmp/lgjsfinance-0.0.6.tar.gz` & `tmp/lgjsfinance-0.0.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "lgjsfinance-0.0.6.tar", last modified: Mon May 13 08:34:25 2024, max compression
+gzip compressed data, was "lgjsfinance-0.0.7.tar", last modified: Wed May 29 11:43:22 2024, max compression
```

## Comparing `lgjsfinance-0.0.6.tar` & `lgjsfinance-0.0.7.tar`

### file list

```diff
@@ -1,15 +1,15 @@
-drwxrwxrwx   0        0        0        0 2024-05-13 08:34:25.949371 lgjsfinance-0.0.6/
--rw-rw-rw-   0        0        0     1091 2024-05-13 07:32:41.000000 lgjsfinance-0.0.6/LICENSE
--rw-rw-rw-   0        0        0     1196 2024-05-13 08:34:25.948028 lgjsfinance-0.0.6/PKG-INFO
--rw-rw-rw-   0        0        0      378 2024-05-13 08:10:29.000000 lgjsfinance-0.0.6/README.md
-drwxrwxrwx   0        0        0        0 2024-05-13 08:34:25.915995 lgjsfinance-0.0.6/lgjsfinance/
--rw-rw-rw-   0        0        0      136 2024-05-13 08:34:09.000000 lgjsfinance-0.0.6/lgjsfinance/__init__.py
--rw-rw-rw-   0        0        0     1248 2024-05-13 08:34:05.000000 lgjsfinance-0.0.6/lgjsfinance/module.py
-drwxrwxrwx   0        0        0        0 2024-05-13 08:34:25.946030 lgjsfinance-0.0.6/lgjsfinance.egg-info/
--rw-rw-rw-   0        0        0     1196 2024-05-13 08:34:25.000000 lgjsfinance-0.0.6/lgjsfinance.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      246 2024-05-13 08:34:25.000000 lgjsfinance-0.0.6/lgjsfinance.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-05-13 08:34:25.000000 lgjsfinance-0.0.6/lgjsfinance.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       37 2024-05-13 08:34:25.000000 lgjsfinance-0.0.6/lgjsfinance.egg-info/requires.txt
--rw-rw-rw-   0        0        0       12 2024-05-13 08:34:25.000000 lgjsfinance-0.0.6/lgjsfinance.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2024-05-13 08:34:25.949371 lgjsfinance-0.0.6/setup.cfg
--rw-rw-rw-   0        0        0     1152 2024-05-13 08:33:28.000000 lgjsfinance-0.0.6/setup.py
+drwxrwxrwx   0        0        0        0 2024-05-29 11:43:22.422998 lgjsfinance-0.0.7/
+-rw-rw-rw-   0        0        0     1091 2024-05-13 07:32:41.000000 lgjsfinance-0.0.7/LICENSE
+-rw-rw-rw-   0        0        0     1196 2024-05-29 11:43:22.417000 lgjsfinance-0.0.7/PKG-INFO
+-rw-rw-rw-   0        0        0      378 2024-05-13 08:10:29.000000 lgjsfinance-0.0.7/README.md
+drwxrwxrwx   0        0        0        0 2024-05-29 11:43:22.354440 lgjsfinance-0.0.7/lgjsfinance/
+-rw-rw-rw-   0        0        0      136 2024-05-29 11:43:19.000000 lgjsfinance-0.0.7/lgjsfinance/__init__.py
+-rw-rw-rw-   0        0        0     1286 2024-05-29 11:42:41.000000 lgjsfinance-0.0.7/lgjsfinance/module.py
+drwxrwxrwx   0        0        0        0 2024-05-29 11:43:22.415003 lgjsfinance-0.0.7/lgjsfinance.egg-info/
+-rw-rw-rw-   0        0        0     1196 2024-05-29 11:43:22.000000 lgjsfinance-0.0.7/lgjsfinance.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      246 2024-05-29 11:43:22.000000 lgjsfinance-0.0.7/lgjsfinance.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-05-29 11:43:22.000000 lgjsfinance-0.0.7/lgjsfinance.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       37 2024-05-29 11:43:22.000000 lgjsfinance-0.0.7/lgjsfinance.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       12 2024-05-29 11:43:22.000000 lgjsfinance-0.0.7/lgjsfinance.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2024-05-29 11:43:22.422998 lgjsfinance-0.0.7/setup.cfg
+-rw-rw-rw-   0        0        0     1152 2024-05-29 11:43:13.000000 lgjsfinance-0.0.7/setup.py
```

### Comparing `lgjsfinance-0.0.6/LICENSE` & `lgjsfinance-0.0.7/LICENSE`

 * *Files identical despite different names*

### Comparing `lgjsfinance-0.0.6/PKG-INFO` & `lgjsfinance-0.0.7/PKG-INFO`

 * *Files 15% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: lgjsfinance
-Version: 0.0.6
+Version: 0.0.7
 Summary: LGJS Finance
 Home-page: https://liamgenjs.vercel.app
 Author: liamgen.js
 Author-email: liamgen.js@proton.me
 License: BSD 2-clause
 Classifier: Development Status :: 1 - Planning
 Classifier: Intended Audience :: Science/Research
```

### Comparing `lgjsfinance-0.0.6/lgjsfinance.egg-info/PKG-INFO` & `lgjsfinance-0.0.7/lgjsfinance.egg-info/PKG-INFO`

 * *Files 15% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: lgjsfinance
-Version: 0.0.6
+Version: 0.0.7
 Summary: LGJS Finance
 Home-page: https://liamgenjs.vercel.app
 Author: liamgen.js
 Author-email: liamgen.js@proton.me
 License: BSD 2-clause
 Classifier: Development Status :: 1 - Planning
 Classifier: Intended Audience :: Science/Research
```

### Comparing `lgjsfinance-0.0.6/setup.py` & `lgjsfinance-0.0.7/setup.py`

 * *Files 11% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 
 from pathlib import Path
 this_directory = Path(__file__).parent
 long_description = (this_directory / "README.md").read_text()
 
 setup(
     name='lgjsfinance',
-    version='0.0.6',    
+    version='0.0.7',    
     description='LGJS Finance',
     url='https://liamgenjs.vercel.app',
     author='liamgen.js',
     author_email='liamgen.js@proton.me',
     license='BSD 2-clause',
     packages=['lgjsfinance'],
     install_requires=['yfinance>=0.2.38',
```

