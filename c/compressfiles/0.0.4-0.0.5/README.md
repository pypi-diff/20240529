# Comparing `tmp/compressfiles-0.0.4.tar.gz` & `tmp/compressfiles-0.0.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "compressfiles-0.0.4.tar", last modified: Wed Sep 20 22:24:50 2023, max compression
+gzip compressed data, was "compressfiles-0.0.5.tar", last modified: Wed May 29 21:10:45 2024, max compression
```

## Comparing `compressfiles-0.0.4.tar` & `compressfiles-0.0.5.tar`

### file list

```diff
@@ -1,15 +1,15 @@
-drwxrwxrwx   0        0        0        0 2023-09-20 22:24:50.897390 compressfiles-0.0.4/
--rw-rw-rw-   0        0        0     1082 2023-09-19 22:42:22.000000 compressfiles-0.0.4/License.txt
--rw-rw-rw-   0        0        0     1947 2023-09-20 22:24:50.895393 compressfiles-0.0.4/PKG-INFO
--rw-rw-rw-   0        0        0     1385 2023-09-20 00:03:23.000000 compressfiles-0.0.4/README.md
--rw-rw-rw-   0        0        0      181 2023-09-19 23:32:03.000000 compressfiles-0.0.4/pyproject.toml
--rw-rw-rw-   0        0        0      695 2023-09-20 22:24:50.901839 compressfiles-0.0.4/setup.cfg
-drwxrwxrwx   0        0        0        0 2023-09-20 22:24:50.802415 compressfiles-0.0.4/src/
-drwxrwxrwx   0        0        0        0 2023-09-20 22:24:50.832788 compressfiles-0.0.4/src/compressfiles/
--rw-rw-rw-   0        0        0       72 2023-09-20 22:06:57.000000 compressfiles-0.0.4/src/compressfiles/__init__.py
--rw-rw-rw-   0        0        0     3561 2023-09-19 23:17:37.000000 compressfiles-0.0.4/src/compressfiles/compressfiles.py
-drwxrwxrwx   0        0        0        0 2023-09-20 22:24:50.884585 compressfiles-0.0.4/src/compressfiles.egg-info/
--rw-rw-rw-   0        0        0     1947 2023-09-20 22:24:50.000000 compressfiles-0.0.4/src/compressfiles.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      275 2023-09-20 22:24:50.000000 compressfiles-0.0.4/src/compressfiles.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-09-20 22:24:50.000000 compressfiles-0.0.4/src/compressfiles.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       14 2023-09-20 22:24:50.000000 compressfiles-0.0.4/src/compressfiles.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2024-05-29 21:10:45.596823 compressfiles-0.0.5/
+-rw-rw-rw-   0        0        0     1082 2024-04-06 17:53:18.000000 compressfiles-0.0.5/License.txt
+-rw-rw-rw-   0        0        0     1947 2024-05-29 21:10:45.595822 compressfiles-0.0.5/PKG-INFO
+-rw-rw-rw-   0        0        0     1385 2024-04-06 17:53:18.000000 compressfiles-0.0.5/README.md
+-rw-rw-rw-   0        0        0      181 2024-04-06 17:53:18.000000 compressfiles-0.0.5/pyproject.toml
+-rw-rw-rw-   0        0        0      695 2024-05-29 21:10:45.597823 compressfiles-0.0.5/setup.cfg
+drwxrwxrwx   0        0        0        0 2024-05-29 21:10:45.580823 compressfiles-0.0.5/src/
+drwxrwxrwx   0        0        0        0 2024-05-29 21:10:45.587822 compressfiles-0.0.5/src/compressfiles/
+-rw-rw-rw-   0        0        0       74 2024-05-29 20:50:28.000000 compressfiles-0.0.5/src/compressfiles/__init__.py
+-rw-rw-rw-   0        0        0     3561 2024-04-06 17:53:18.000000 compressfiles-0.0.5/src/compressfiles/compressfiles.py
+drwxrwxrwx   0        0        0        0 2024-05-29 21:10:45.594822 compressfiles-0.0.5/src/compressfiles.egg-info/
+-rw-rw-rw-   0        0        0     1947 2024-05-29 21:10:45.000000 compressfiles-0.0.5/src/compressfiles.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      275 2024-05-29 21:10:45.000000 compressfiles-0.0.5/src/compressfiles.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-05-29 21:10:45.000000 compressfiles-0.0.5/src/compressfiles.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       14 2024-05-29 21:10:45.000000 compressfiles-0.0.5/src/compressfiles.egg-info/top_level.txt
```

### Comparing `compressfiles-0.0.4/License.txt` & `compressfiles-0.0.5/License.txt`

 * *Files identical despite different names*

### Comparing `compressfiles-0.0.4/PKG-INFO` & `compressfiles-0.0.5/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: compressfiles
-Version: 0.0.4
+Version: 0.0.5
 Summary: Library used to compress files using gzip but more simple
 Home-page: https://github.com/Alleexx129/txt-compressor
 Author: Alleexx
 Author-email: alleexx129@gmail.com
 Project-URL: Bug Tracker, https://github.com/Alleexx129/txt-compressor/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
```

### Comparing `compressfiles-0.0.4/README.md` & `compressfiles-0.0.5/README.md`

 * *Files identical despite different names*

### Comparing `compressfiles-0.0.4/setup.cfg` & `compressfiles-0.0.5/setup.cfg`

 * *Files 17% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 00000000: 5b6d 6574 6164 6174 615d 0d0a 6e61 6d65  [metadata]..name
 00000010: 203d 2063 6f6d 7072 6573 7366 696c 6573   = compressfiles
 00000020: 0d0a 7665 7273 696f 6e20 3d20 302e 302e  ..version = 0.0.
-00000030: 340d 0a61 7574 686f 7220 3d20 416c 6c65  4..author = Alle
+00000030: 350d 0a61 7574 686f 7220 3d20 416c 6c65  5..author = Alle
 00000040: 6578 780d 0a61 7574 686f 725f 656d 6169  exx..author_emai
 00000050: 6c20 3d20 616c 6c65 6578 7831 3239 4067  l = alleexx129@g
 00000060: 6d61 696c 2e63 6f6d 0d0a 6465 7363 7269  mail.com..descri
 00000070: 7074 696f 6e20 3d20 4c69 6272 6172 7920  ption = Library 
 00000080: 7573 6564 2074 6f20 636f 6d70 7265 7373  used to compress
 00000090: 2066 696c 6573 2075 7369 6e67 2067 7a69   files using gzi
 000000a0: 7020 6275 7420 6d6f 7265 2073 696d 706c  p but more simpl
```

### Comparing `compressfiles-0.0.4/src/compressfiles/compressfiles.py` & `compressfiles-0.0.5/src/compressfiles/compressfiles.py`

 * *Files identical despite different names*

### Comparing `compressfiles-0.0.4/src/compressfiles.egg-info/PKG-INFO` & `compressfiles-0.0.5/src/compressfiles.egg-info/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: compressfiles
-Version: 0.0.4
+Version: 0.0.5
 Summary: Library used to compress files using gzip but more simple
 Home-page: https://github.com/Alleexx129/txt-compressor
 Author: Alleexx
 Author-email: alleexx129@gmail.com
 Project-URL: Bug Tracker, https://github.com/Alleexx129/txt-compressor/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
```

