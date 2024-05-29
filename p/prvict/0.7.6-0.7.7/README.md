# Comparing `tmp/prvict-0.7.6.tar.gz` & `tmp/prvict-0.7.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "prvict-0.7.6.tar", last modified: Tue May 28 14:28:37 2024, max compression
+gzip compressed data, was "prvict-0.7.7.tar", last modified: Wed May 29 04:21:20 2024, max compression
```

## Comparing `prvict-0.7.6.tar` & `prvict-0.7.7.tar`

### file list

```diff
@@ -1,15 +1,15 @@
-drwxrwxrwx   0        0        0        0 2024-05-28 14:28:37.656978 prvict-0.7.6/
--rw-rw-rw-   0        0        0    34817 2024-05-26 07:02:07.000000 prvict-0.7.6/LICENSE
--rw-rw-rw-   0        0        0     2162 2024-05-28 14:28:37.655975 prvict-0.7.6/PKG-INFO
--rw-rw-rw-   0        0        0     1606 2024-05-27 13:59:18.000000 prvict-0.7.6/README.md
--rw-rw-rw-   0        0        0      108 2024-05-28 13:04:48.000000 prvict-0.7.6/pyproject.toml
--rw-rw-rw-   0        0        0      695 2024-05-28 14:28:37.663976 prvict-0.7.6/setup.cfg
-drwxrwxrwx   0        0        0        0 2024-05-28 14:28:37.601982 prvict-0.7.6/src/
-drwxrwxrwx   0        0        0        0 2024-05-28 14:28:37.623975 prvict-0.7.6/src/prvict/
--rw-rw-rw-   0        0        0        0 2024-05-26 07:02:07.000000 prvict-0.7.6/src/prvict/__init__.py
--rw-rw-rw-   0        0        0     8992 2024-05-26 07:02:07.000000 prvict-0.7.6/src/prvict/main.py
-drwxrwxrwx   0        0        0        0 2024-05-28 14:28:37.653975 prvict-0.7.6/src/prvict.egg-info/
--rw-rw-rw-   0        0        0     2162 2024-05-28 14:28:37.000000 prvict-0.7.6/src/prvict.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      220 2024-05-28 14:28:37.000000 prvict-0.7.6/src/prvict.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-05-28 14:28:37.000000 prvict-0.7.6/src/prvict.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0        7 2024-05-28 14:28:37.000000 prvict-0.7.6/src/prvict.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2024-05-29 04:21:20.754484 prvict-0.7.7/
+-rw-rw-rw-   0        0        0    34817 2024-05-26 07:02:07.000000 prvict-0.7.7/LICENSE
+-rw-rw-rw-   0        0        0     2162 2024-05-29 04:21:20.753484 prvict-0.7.7/PKG-INFO
+-rw-rw-rw-   0        0        0     1606 2024-05-27 13:59:18.000000 prvict-0.7.7/README.md
+-rw-rw-rw-   0        0        0      108 2024-05-28 13:04:48.000000 prvict-0.7.7/pyproject.toml
+-rw-rw-rw-   0        0        0      695 2024-05-29 04:21:20.758485 prvict-0.7.7/setup.cfg
+drwxrwxrwx   0        0        0        0 2024-05-29 04:21:20.718484 prvict-0.7.7/src/
+drwxrwxrwx   0        0        0        0 2024-05-29 04:21:20.736483 prvict-0.7.7/src/prvict/
+-rw-rw-rw-   0        0        0     8992 2024-05-29 04:18:22.000000 prvict-0.7.7/src/prvict/__init__.py
+-rw-rw-rw-   0        0        0       22 2024-05-29 04:18:36.000000 prvict-0.7.7/src/prvict/main.py
+drwxrwxrwx   0        0        0        0 2024-05-29 04:21:20.751484 prvict-0.7.7/src/prvict.egg-info/
+-rw-rw-rw-   0        0        0     2162 2024-05-29 04:21:20.000000 prvict-0.7.7/src/prvict.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      220 2024-05-29 04:21:20.000000 prvict-0.7.7/src/prvict.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-05-29 04:21:20.000000 prvict-0.7.7/src/prvict.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0        7 2024-05-29 04:21:20.000000 prvict-0.7.7/src/prvict.egg-info/top_level.txt
```

### Comparing `prvict-0.7.6/LICENSE` & `prvict-0.7.7/LICENSE`

 * *Files identical despite different names*

### Comparing `prvict-0.7.6/PKG-INFO` & `prvict-0.7.7/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: prvict
-Version: 0.7.6
+Version: 0.7.7
 Summary: A library pioneering AI and computational based tech solutions.
 Home-page: https://github.com/VaidikKhurana/prvict
 Author: Vaidik Khurana
 Author-email: vaidikkhurana@gmail.com
 Project-URL: Bug Tracker, https://github.com/VaidikKhurana/prvict/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
```

### Comparing `prvict-0.7.6/README.md` & `prvict-0.7.7/README.md`

 * *Files identical despite different names*

### Comparing `prvict-0.7.6/setup.cfg` & `prvict-0.7.7/setup.cfg`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 00000000: 5b6d 6574 6164 6174 615d 0d0a 6e61 6d65  [metadata]..name
 00000010: 203d 2070 7276 6963 740d 0a76 6572 7369   = prvict..versi
-00000020: 6f6e 203d 2030 2e37 2e36 0d0a 6175 7468  on = 0.7.6..auth
+00000020: 6f6e 203d 2030 2e37 2e37 0d0a 6175 7468  on = 0.7.7..auth
 00000030: 6f72 203d 2056 6169 6469 6b20 4b68 7572  or = Vaidik Khur
 00000040: 616e 610d 0a61 7574 686f 725f 656d 6169  ana..author_emai
 00000050: 6c20 3d20 7661 6964 696b 6b68 7572 616e  l = vaidikkhuran
 00000060: 6140 676d 6169 6c2e 636f 6d0d 0a64 6573  a@gmail.com..des
 00000070: 6372 6970 7469 6f6e 203d 2041 206c 6962  cription = A lib
 00000080: 7261 7279 2070 696f 6e65 6572 696e 6720  rary pioneering 
 00000090: 4149 2061 6e64 2063 6f6d 7075 7461 7469  AI and computati
```

### Comparing `prvict-0.7.6/src/prvict/main.py` & `prvict-0.7.7/src/prvict/__init__.py`

 * *Files identical despite different names*

### Comparing `prvict-0.7.6/src/prvict.egg-info/PKG-INFO` & `prvict-0.7.7/src/prvict.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: prvict
-Version: 0.7.6
+Version: 0.7.7
 Summary: A library pioneering AI and computational based tech solutions.
 Home-page: https://github.com/VaidikKhurana/prvict
 Author: Vaidik Khurana
 Author-email: vaidikkhurana@gmail.com
 Project-URL: Bug Tracker, https://github.com/VaidikKhurana/prvict/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
```

