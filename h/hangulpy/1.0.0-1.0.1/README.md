# Comparing `tmp/hangulpy-1.0.0.tar.gz` & `tmp/hangulpy-1.0.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "hangulpy-1.0.0.tar", last modified: Tue May 28 13:21:12 2024, max compression
+gzip compressed data, was "hangulpy-1.0.1.tar", last modified: Wed May 29 09:42:12 2024, max compression
```

## Comparing `hangulpy-1.0.0.tar` & `hangulpy-1.0.1.tar`

### file list

```diff
@@ -1,23 +1,23 @@
-drwxrwxrwx   0        0        0        0 2024-05-28 13:21:12.375050 hangulpy-1.0.0/
--rw-rw-rw-   0        0        0     1082 2024-05-28 13:19:52.000000 hangulpy-1.0.0/LICENSE
--rw-rw-rw-   0        0        0     3775 2024-05-28 13:21:12.373052 hangulpy-1.0.0/PKG-INFO
--rw-rw-rw-   0        0        0     3166 2024-05-28 12:54:09.000000 hangulpy-1.0.0/README.md
-drwxrwxrwx   0        0        0        0 2024-05-28 13:21:12.363052 hangulpy-1.0.0/hangulpy/
--rw-rw-rw-   0        0        0      520 2024-05-28 13:13:00.000000 hangulpy-1.0.0/hangulpy/__init__.py
--rw-rw-rw-   0        0        0     1053 2024-05-28 11:42:31.000000 hangulpy-1.0.0/hangulpy/chosung.py
--rw-rw-rw-   0        0        0      562 2024-05-28 12:34:27.000000 hangulpy-1.0.0/hangulpy/hangul_check.py
--rw-rw-rw-   0        0        0      872 2024-05-28 12:00:00.000000 hangulpy-1.0.0/hangulpy/hangul_contains.py
--rw-rw-rw-   0        0        0     1250 2024-05-28 12:30:57.000000 hangulpy-1.0.0/hangulpy/hangul_decompose.py
--rw-rw-rw-   0        0        0      674 2024-05-28 12:36:42.000000 hangulpy-1.0.0/hangulpy/hangul_ends_with_consonant.py
--rw-rw-rw-   0        0        0     2684 2024-05-28 12:37:16.000000 hangulpy-1.0.0/hangulpy/hangul_number.py
--rw-rw-rw-   0        0        0      626 2024-05-28 12:33:23.000000 hangulpy-1.0.0/hangulpy/hangul_role.py
--rw-rw-rw-   0        0        0     1282 2024-05-28 12:32:05.000000 hangulpy-1.0.0/hangulpy/hangul_split.py
--rw-rw-rw-   0        0        0     1513 2024-05-28 12:30:31.000000 hangulpy-1.0.0/hangulpy/josa.py
--rw-rw-rw-   0        0        0     3386 2024-05-28 12:37:01.000000 hangulpy-1.0.0/hangulpy/utils.py
-drwxrwxrwx   0        0        0        0 2024-05-28 13:21:12.372050 hangulpy-1.0.0/hangulpy.egg-info/
--rw-rw-rw-   0        0        0     3775 2024-05-28 13:21:12.000000 hangulpy-1.0.0/hangulpy.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      426 2024-05-28 13:21:12.000000 hangulpy-1.0.0/hangulpy.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-05-28 13:21:12.000000 hangulpy-1.0.0/hangulpy.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0        9 2024-05-28 13:21:12.000000 hangulpy-1.0.0/hangulpy.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2024-05-28 13:21:12.375050 hangulpy-1.0.0/setup.cfg
--rw-rw-rw-   0        0        0      677 2024-05-28 13:19:04.000000 hangulpy-1.0.0/setup.py
+drwxrwxrwx   0        0        0        0 2024-05-29 09:42:12.370072 hangulpy-1.0.1/
+-rw-rw-rw-   0        0        0     1082 2024-05-28 13:19:52.000000 hangulpy-1.0.1/LICENSE
+-rw-rw-rw-   0        0        0     3775 2024-05-29 09:42:12.368070 hangulpy-1.0.1/PKG-INFO
+-rw-rw-rw-   0        0        0     3166 2024-05-28 12:54:09.000000 hangulpy-1.0.1/README.md
+drwxrwxrwx   0        0        0        0 2024-05-29 09:42:12.356047 hangulpy-1.0.1/hangulpy/
+-rw-rw-rw-   0        0        0      520 2024-05-28 13:13:00.000000 hangulpy-1.0.1/hangulpy/__init__.py
+-rw-rw-rw-   0        0        0     1053 2024-05-28 11:42:31.000000 hangulpy-1.0.1/hangulpy/chosung.py
+-rw-rw-rw-   0        0        0      562 2024-05-28 12:34:27.000000 hangulpy-1.0.1/hangulpy/hangul_check.py
+-rw-rw-rw-   0        0        0      872 2024-05-28 12:00:00.000000 hangulpy-1.0.1/hangulpy/hangul_contains.py
+-rw-rw-rw-   0        0        0     1250 2024-05-28 12:30:57.000000 hangulpy-1.0.1/hangulpy/hangul_decompose.py
+-rw-rw-rw-   0        0        0      674 2024-05-28 12:36:42.000000 hangulpy-1.0.1/hangulpy/hangul_ends_with_consonant.py
+-rw-rw-rw-   0        0        0     2684 2024-05-28 12:37:16.000000 hangulpy-1.0.1/hangulpy/hangul_number.py
+-rw-rw-rw-   0        0        0      626 2024-05-28 12:33:23.000000 hangulpy-1.0.1/hangulpy/hangul_role.py
+-rw-rw-rw-   0        0        0     1282 2024-05-28 12:32:05.000000 hangulpy-1.0.1/hangulpy/hangul_split.py
+-rw-rw-rw-   0        0        0     3996 2024-05-29 09:41:28.000000 hangulpy-1.0.1/hangulpy/josa.py
+-rw-rw-rw-   0        0        0     3386 2024-05-28 12:37:01.000000 hangulpy-1.0.1/hangulpy/utils.py
+drwxrwxrwx   0        0        0        0 2024-05-29 09:42:12.367066 hangulpy-1.0.1/hangulpy.egg-info/
+-rw-rw-rw-   0        0        0     3775 2024-05-29 09:42:12.000000 hangulpy-1.0.1/hangulpy.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      426 2024-05-29 09:42:12.000000 hangulpy-1.0.1/hangulpy.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-05-29 09:42:12.000000 hangulpy-1.0.1/hangulpy.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0        9 2024-05-29 09:42:12.000000 hangulpy-1.0.1/hangulpy.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2024-05-29 09:42:12.370072 hangulpy-1.0.1/setup.cfg
+-rw-rw-rw-   0        0        0      677 2024-05-29 09:41:47.000000 hangulpy-1.0.1/setup.py
```

### Comparing `hangulpy-1.0.0/LICENSE` & `hangulpy-1.0.1/LICENSE`

 * *Files identical despite different names*

### Comparing `hangulpy-1.0.0/PKG-INFO` & `hangulpy-1.0.1/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: hangulpy
-Version: 1.0.0
+Version: 1.0.1
 Summary: A Python library for processing Hangul, inspired by es-hangul.
 Home-page: https://github.com/gaon12/hangulpy
 Author: Jeong Gaon
 Author-email: gokirito12@gmail.com
 License: MIT
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
```

### Comparing `hangulpy-1.0.0/README.md` & `hangulpy-1.0.1/README.md`

 * *Files identical despite different names*

### Comparing `hangulpy-1.0.0/hangulpy/__init__.py` & `hangulpy-1.0.1/hangulpy/__init__.py`

 * *Files identical despite different names*

### Comparing `hangulpy-1.0.0/hangulpy/chosung.py` & `hangulpy-1.0.1/hangulpy/chosung.py`

 * *Files identical despite different names*

### Comparing `hangulpy-1.0.0/hangulpy/hangul_check.py` & `hangulpy-1.0.1/hangulpy/hangul_check.py`

 * *Files identical despite different names*

### Comparing `hangulpy-1.0.0/hangulpy/hangul_contains.py` & `hangulpy-1.0.1/hangulpy/hangul_contains.py`

 * *Files identical despite different names*

### Comparing `hangulpy-1.0.0/hangulpy/hangul_decompose.py` & `hangulpy-1.0.1/hangulpy/hangul_decompose.py`

 * *Files identical despite different names*

### Comparing `hangulpy-1.0.0/hangulpy/hangul_ends_with_consonant.py` & `hangulpy-1.0.1/hangulpy/hangul_ends_with_consonant.py`

 * *Files identical despite different names*

### Comparing `hangulpy-1.0.0/hangulpy/hangul_number.py` & `hangulpy-1.0.1/hangulpy/hangul_number.py`

 * *Files identical despite different names*

### Comparing `hangulpy-1.0.0/hangulpy/hangul_role.py` & `hangulpy-1.0.1/hangulpy/hangul_role.py`

 * *Files identical despite different names*

### Comparing `hangulpy-1.0.0/hangulpy/hangul_split.py` & `hangulpy-1.0.1/hangulpy/hangul_split.py`

 * *Files identical despite different names*

### Comparing `hangulpy-1.0.0/hangulpy/utils.py` & `hangulpy-1.0.1/hangulpy/utils.py`

 * *Files identical despite different names*

### Comparing `hangulpy-1.0.0/hangulpy.egg-info/PKG-INFO` & `hangulpy-1.0.1/hangulpy.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: hangulpy
-Version: 1.0.0
+Version: 1.0.1
 Summary: A Python library for processing Hangul, inspired by es-hangul.
 Home-page: https://github.com/gaon12/hangulpy
 Author: Jeong Gaon
 Author-email: gokirito12@gmail.com
 License: MIT
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
```

### Comparing `hangulpy-1.0.0/setup.py` & `hangulpy-1.0.1/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from setuptools import setup, find_packages
 
 setup(
     name='hangulpy',
-    version='1.0.0',
+    version='1.0.1',
     description='A Python library for processing Hangul, inspired by es-hangul.',
     long_description=open('README.md', encoding='utf-8').read(),
     long_description_content_type='text/markdown',
     url='https://github.com/gaon12/hangulpy',
     author='Jeong Gaon',
     author_email='gokirito12@gmail.com',
     license='MIT',
```

