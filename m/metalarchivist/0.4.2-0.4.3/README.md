# Comparing `tmp/metalarchivist-0.4.2.tar.gz` & `tmp/metalarchivist-0.4.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "metalarchivist-0.4.2.tar", last modified: Mon May 20 23:39:30 2024, max compression
+gzip compressed data, was "metalarchivist-0.4.3.tar", last modified: Wed May 29 14:39:37 2024, max compression
```

## Comparing `metalarchivist-0.4.2.tar` & `metalarchivist-0.4.3.tar`

### file list

```diff
@@ -1,42 +1,42 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-20 23:39:30.820120 metalarchivist-0.4.2/
--rwxrwxrwx   0 root         (0) root         (0)      693 2024-05-20 23:39:17.000000 metalarchivist-0.4.2/LICENSE
--rw-r--r--   0 root         (0) root         (0)      702 2024-05-20 23:39:30.819120 metalarchivist-0.4.2/PKG-INFO
--rwxrwxrwx   0 root         (0) root         (0)      113 2024-05-20 23:39:17.000000 metalarchivist-0.4.2/README.md
--rwxrwxrwx   0 root         (0) root         (0)      677 2024-05-20 23:39:17.000000 metalarchivist-0.4.2/pyproject.toml
--rw-r--r--   0 root         (0) root         (0)       38 2024-05-20 23:39:30.820120 metalarchivist-0.4.2/setup.cfg
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-20 23:39:30.811120 metalarchivist-0.4.2/src/
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-20 23:39:30.813120 metalarchivist-0.4.2/src/metalarchivist/
--rwxrwxrwx   0 root         (0) root         (0)      107 2024-05-20 23:39:17.000000 metalarchivist-0.4.2/src/metalarchivist/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-20 23:39:30.815120 metalarchivist-0.4.2/src/metalarchivist/export/
--rwxrwxrwx   0 root         (0) root         (0)      257 2024-05-20 23:39:17.000000 metalarchivist-0.4.2/src/metalarchivist/export/__init__.py
--rwxrwxrwx   0 root         (0) root         (0)     4225 2024-05-20 23:39:17.000000 metalarchivist-0.4.2/src/metalarchivist/export/album.py
--rwxrwxrwx   0 root         (0) root         (0)     3679 2024-05-20 23:39:17.000000 metalarchivist-0.4.2/src/metalarchivist/export/band.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-20 23:39:30.815120 metalarchivist-0.4.2/src/metalarchivist/export/data/
--rw-rw-rw-   0 root         (0) root         (0)     1754 2024-05-20 23:39:17.000000 metalarchivist-0.4.2/src/metalarchivist/export/data/user-agents.json
--rw-rw-rw-   0 root         (0) root         (0)     2685 2024-05-20 23:39:17.000000 metalarchivist-0.4.2/src/metalarchivist/export/genre.py
--rw-rw-rw-   0 root         (0) root         (0)    10565 2024-05-20 23:39:17.000000 metalarchivist-0.4.2/src/metalarchivist/export/label.py
--rwxrwxrwx   0 root         (0) root         (0)     7075 2024-05-20 23:39:17.000000 metalarchivist-0.4.2/src/metalarchivist/export/util.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-20 23:39:30.817120 metalarchivist-0.4.2/src/metalarchivist/interface/
--rwxrwxrwx   0 root         (0) root         (0)     1378 2024-05-20 23:39:17.000000 metalarchivist-0.4.2/src/metalarchivist/interface/__init__.py
--rwxrwxrwx   0 root         (0) root         (0)     9056 2024-05-20 23:39:17.000000 metalarchivist-0.4.2/src/metalarchivist/interface/album.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-20 23:39:30.817120 metalarchivist-0.4.2/src/metalarchivist/interface/api/
--rw-rw-rw-   0 root         (0) root         (0)     3333 2024-05-20 23:39:17.000000 metalarchivist-0.4.2/src/metalarchivist/interface/api/base.py
--rw-rw-rw-   0 root         (0) root         (0)     4929 2024-05-20 23:39:17.000000 metalarchivist-0.4.2/src/metalarchivist/interface/api/page.py
--rwxrwxrwx   0 root         (0) root         (0)     8477 2024-05-20 23:39:17.000000 metalarchivist-0.4.2/src/metalarchivist/interface/band.py
--rw-rw-rw-   0 root         (0) root         (0)     7975 2024-05-20 23:39:17.000000 metalarchivist-0.4.2/src/metalarchivist/interface/genre.py
--rw-rw-rw-   0 root         (0) root         (0)     8163 2024-05-20 23:39:17.000000 metalarchivist-0.4.2/src/metalarchivist/interface/label.py
--rwxrwxrwx   0 root         (0) root         (0)      380 2024-05-20 23:39:17.000000 metalarchivist-0.4.2/src/metalarchivist/interface/search.py
--rw-rw-rw-   0 root         (0) root         (0)     7235 2024-05-20 23:39:17.000000 metalarchivist-0.4.2/src/metalarchivist/interface/theme.py
--rwxrwxrwx   0 root         (0) root         (0)     5991 2024-05-20 23:39:17.000000 metalarchivist-0.4.2/src/metalarchivist/report.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-20 23:39:30.819120 metalarchivist-0.4.2/src/metalarchivist.egg-info/
--rw-r--r--   0 root         (0) root         (0)      702 2024-05-20 23:39:30.000000 metalarchivist-0.4.2/src/metalarchivist.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)     1030 2024-05-20 23:39:30.000000 metalarchivist-0.4.2/src/metalarchivist.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2024-05-20 23:39:30.000000 metalarchivist-0.4.2/src/metalarchivist.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)       31 2024-05-20 23:39:30.000000 metalarchivist-0.4.2/src/metalarchivist.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)       20 2024-05-20 23:39:30.000000 metalarchivist-0.4.2/src/metalarchivist.egg-info/top_level.txt
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-20 23:39:30.819120 metalarchivist-0.4.2/src/test/
--rwxrwxrwx   0 root         (0) root         (0)    10205 2024-05-20 23:39:17.000000 metalarchivist-0.4.2/src/test/test_albums.py
--rwxrwxrwx   0 root         (0) root         (0)     5029 2024-05-20 23:39:17.000000 metalarchivist-0.4.2/src/test/test_bands.py
--rwxrwxrwx   0 root         (0) root         (0)     8506 2024-05-20 23:39:17.000000 metalarchivist-0.4.2/src/test/test_genres.py
--rw-rw-rw-   0 root         (0) root         (0)     5581 2024-05-20 23:39:17.000000 metalarchivist-0.4.2/src/test/test_labels.py
--rw-rw-rw-   0 root         (0) root         (0)     4108 2024-05-20 23:39:17.000000 metalarchivist-0.4.2/src/test/test_themes.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-29 14:39:37.050498 metalarchivist-0.4.3/
+-rwxrwxrwx   0 root         (0) root         (0)      693 2024-05-29 14:39:23.000000 metalarchivist-0.4.3/LICENSE
+-rw-r--r--   0 root         (0) root         (0)      702 2024-05-29 14:39:37.049497 metalarchivist-0.4.3/PKG-INFO
+-rwxrwxrwx   0 root         (0) root         (0)      113 2024-05-29 14:39:23.000000 metalarchivist-0.4.3/README.md
+-rwxrwxrwx   0 root         (0) root         (0)      677 2024-05-29 14:39:23.000000 metalarchivist-0.4.3/pyproject.toml
+-rw-r--r--   0 root         (0) root         (0)       38 2024-05-29 14:39:37.050498 metalarchivist-0.4.3/setup.cfg
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-29 14:39:37.042497 metalarchivist-0.4.3/src/
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-29 14:39:37.043498 metalarchivist-0.4.3/src/metalarchivist/
+-rwxrwxrwx   0 root         (0) root         (0)      107 2024-05-29 14:39:23.000000 metalarchivist-0.4.3/src/metalarchivist/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-29 14:39:37.046498 metalarchivist-0.4.3/src/metalarchivist/export/
+-rwxrwxrwx   0 root         (0) root         (0)      257 2024-05-29 14:39:23.000000 metalarchivist-0.4.3/src/metalarchivist/export/__init__.py
+-rwxrwxrwx   0 root         (0) root         (0)     4225 2024-05-29 14:39:23.000000 metalarchivist-0.4.3/src/metalarchivist/export/album.py
+-rwxrwxrwx   0 root         (0) root         (0)     3679 2024-05-29 14:39:23.000000 metalarchivist-0.4.3/src/metalarchivist/export/band.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-29 14:39:37.046498 metalarchivist-0.4.3/src/metalarchivist/export/data/
+-rw-rw-rw-   0 root         (0) root         (0)     1754 2024-05-29 14:39:23.000000 metalarchivist-0.4.3/src/metalarchivist/export/data/user-agents.json
+-rw-rw-rw-   0 root         (0) root         (0)     2685 2024-05-29 14:39:23.000000 metalarchivist-0.4.3/src/metalarchivist/export/genre.py
+-rw-rw-rw-   0 root         (0) root         (0)    10565 2024-05-29 14:39:23.000000 metalarchivist-0.4.3/src/metalarchivist/export/label.py
+-rwxrwxrwx   0 root         (0) root         (0)     7075 2024-05-29 14:39:23.000000 metalarchivist-0.4.3/src/metalarchivist/export/util.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-29 14:39:37.047498 metalarchivist-0.4.3/src/metalarchivist/interface/
+-rwxrwxrwx   0 root         (0) root         (0)     1378 2024-05-29 14:39:23.000000 metalarchivist-0.4.3/src/metalarchivist/interface/__init__.py
+-rwxrwxrwx   0 root         (0) root         (0)     9056 2024-05-29 14:39:23.000000 metalarchivist-0.4.3/src/metalarchivist/interface/album.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-29 14:39:37.048498 metalarchivist-0.4.3/src/metalarchivist/interface/api/
+-rw-rw-rw-   0 root         (0) root         (0)     3333 2024-05-29 14:39:23.000000 metalarchivist-0.4.3/src/metalarchivist/interface/api/base.py
+-rw-rw-rw-   0 root         (0) root         (0)     4929 2024-05-29 14:39:23.000000 metalarchivist-0.4.3/src/metalarchivist/interface/api/page.py
+-rwxrwxrwx   0 root         (0) root         (0)     8477 2024-05-29 14:39:23.000000 metalarchivist-0.4.3/src/metalarchivist/interface/band.py
+-rw-rw-rw-   0 root         (0) root         (0)     7975 2024-05-29 14:39:23.000000 metalarchivist-0.4.3/src/metalarchivist/interface/genre.py
+-rw-rw-rw-   0 root         (0) root         (0)     8163 2024-05-29 14:39:23.000000 metalarchivist-0.4.3/src/metalarchivist/interface/label.py
+-rwxrwxrwx   0 root         (0) root         (0)      380 2024-05-29 14:39:23.000000 metalarchivist-0.4.3/src/metalarchivist/interface/search.py
+-rw-rw-rw-   0 root         (0) root         (0)     7235 2024-05-29 14:39:23.000000 metalarchivist-0.4.3/src/metalarchivist/interface/theme.py
+-rwxrwxrwx   0 root         (0) root         (0)     6043 2024-05-29 14:39:23.000000 metalarchivist-0.4.3/src/metalarchivist/report.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-29 14:39:37.049497 metalarchivist-0.4.3/src/metalarchivist.egg-info/
+-rw-r--r--   0 root         (0) root         (0)      702 2024-05-29 14:39:37.000000 metalarchivist-0.4.3/src/metalarchivist.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)     1030 2024-05-29 14:39:37.000000 metalarchivist-0.4.3/src/metalarchivist.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2024-05-29 14:39:37.000000 metalarchivist-0.4.3/src/metalarchivist.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)       31 2024-05-29 14:39:37.000000 metalarchivist-0.4.3/src/metalarchivist.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)       20 2024-05-29 14:39:37.000000 metalarchivist-0.4.3/src/metalarchivist.egg-info/top_level.txt
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-29 14:39:37.049497 metalarchivist-0.4.3/src/test/
+-rwxrwxrwx   0 root         (0) root         (0)    10205 2024-05-29 14:39:23.000000 metalarchivist-0.4.3/src/test/test_albums.py
+-rwxrwxrwx   0 root         (0) root         (0)     5029 2024-05-29 14:39:23.000000 metalarchivist-0.4.3/src/test/test_bands.py
+-rwxrwxrwx   0 root         (0) root         (0)     8506 2024-05-29 14:39:23.000000 metalarchivist-0.4.3/src/test/test_genres.py
+-rw-rw-rw-   0 root         (0) root         (0)     5581 2024-05-29 14:39:23.000000 metalarchivist-0.4.3/src/test/test_labels.py
+-rw-rw-rw-   0 root         (0) root         (0)     4108 2024-05-29 14:39:23.000000 metalarchivist-0.4.3/src/test/test_themes.py
```

### Comparing `metalarchivist-0.4.2/LICENSE` & `metalarchivist-0.4.3/LICENSE`

 * *Files identical despite different names*

### Comparing `metalarchivist-0.4.2/PKG-INFO` & `metalarchivist-0.4.3/PKG-INFO`

 * *Files 15% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: metalarchivist
-Version: 0.4.2
+Version: 0.4.3
 Summary: A package for extracting data from metal-archives.com
 Author-email: z3c0 <z3c0@21337.tech>
 Project-URL: Homepage, https://gitlab.com/black-metal-book-club/metallum
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: GNU Lesser General Public License v3 (LGPLv3)
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.11
```

### Comparing `metalarchivist-0.4.2/pyproject.toml` & `metalarchivist-0.4.3/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [project]
 name = "metalarchivist"
-version = "0.4.2"
+version = "0.4.3"
 authors = [ { name = "z3c0", email = "z3c0@21337.tech" } ]
 description = "A package for extracting data from metal-archives.com"
 readme = "README.md"
 requires-python = ">=3.11"
 dependencies = [ "rich", "lxml", "urllib3", "pycryptodome" ]
 classifiers = [
   "Programming Language :: Python :: 3",
```

### Comparing `metalarchivist-0.4.2/src/metalarchivist/export/album.py` & `metalarchivist-0.4.3/src/metalarchivist/export/album.py`

 * *Files identical despite different names*

### Comparing `metalarchivist-0.4.2/src/metalarchivist/export/band.py` & `metalarchivist-0.4.3/src/metalarchivist/export/band.py`

 * *Files identical despite different names*

### Comparing `metalarchivist-0.4.2/src/metalarchivist/export/data/user-agents.json` & `metalarchivist-0.4.3/src/metalarchivist/export/data/user-agents.json`

 * *Files identical despite different names*

### Comparing `metalarchivist-0.4.2/src/metalarchivist/export/genre.py` & `metalarchivist-0.4.3/src/metalarchivist/export/genre.py`

 * *Files identical despite different names*

### Comparing `metalarchivist-0.4.2/src/metalarchivist/export/label.py` & `metalarchivist-0.4.3/src/metalarchivist/export/label.py`

 * *Files identical despite different names*

### Comparing `metalarchivist-0.4.2/src/metalarchivist/export/util.py` & `metalarchivist-0.4.3/src/metalarchivist/export/util.py`

 * *Files identical despite different names*

### Comparing `metalarchivist-0.4.2/src/metalarchivist/interface/__init__.py` & `metalarchivist-0.4.3/src/metalarchivist/interface/__init__.py`

 * *Files identical despite different names*

### Comparing `metalarchivist-0.4.2/src/metalarchivist/interface/album.py` & `metalarchivist-0.4.3/src/metalarchivist/interface/album.py`

 * *Files identical despite different names*

### Comparing `metalarchivist-0.4.2/src/metalarchivist/interface/api/base.py` & `metalarchivist-0.4.3/src/metalarchivist/interface/api/base.py`

 * *Files identical despite different names*

### Comparing `metalarchivist-0.4.2/src/metalarchivist/interface/api/page.py` & `metalarchivist-0.4.3/src/metalarchivist/interface/api/page.py`

 * *Files identical despite different names*

### Comparing `metalarchivist-0.4.2/src/metalarchivist/interface/band.py` & `metalarchivist-0.4.3/src/metalarchivist/interface/band.py`

 * *Files identical despite different names*

### Comparing `metalarchivist-0.4.2/src/metalarchivist/interface/genre.py` & `metalarchivist-0.4.3/src/metalarchivist/interface/genre.py`

 * *Files identical despite different names*

### Comparing `metalarchivist-0.4.2/src/metalarchivist/interface/label.py` & `metalarchivist-0.4.3/src/metalarchivist/interface/label.py`

 * *Files identical despite different names*

### Comparing `metalarchivist-0.4.2/src/metalarchivist/interface/theme.py` & `metalarchivist-0.4.3/src/metalarchivist/interface/theme.py`

 * *Files identical despite different names*

### Comparing `metalarchivist-0.4.2/src/metalarchivist/report.py` & `metalarchivist-0.4.3/src/metalarchivist/report.py`

 * *Files 0% similar despite different names*

```diff
@@ -107,15 +107,16 @@
 
     label_url = where(label_link, 'link', lambda n: n is not None)
     label_url = series(label_url, 'link')
     label_url = [str(u) for u in label_url]
     label = get_label_profiles(label_url)
     label = rename(label, dict(profile='label_profile',
                                roster='label_roster',
-                               releases='label_releases'))
+                               releases='label_releases',
+                               links='label_links'))
     
     band = rename(band, dict(url='band_url', name='band'))
     release = drop(release, 'genres', 'band', 'album', 'release_type')
     
     album = drop(album, 'label')
     album = zip(album, band_key, label_key, release)
     album = [dict(**a, **b, **lb, **r) for a, b, lb, r in album]
```

### Comparing `metalarchivist-0.4.2/src/metalarchivist.egg-info/PKG-INFO` & `metalarchivist-0.4.3/src/metalarchivist.egg-info/PKG-INFO`

 * *Files 15% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: metalarchivist
-Version: 0.4.2
+Version: 0.4.3
 Summary: A package for extracting data from metal-archives.com
 Author-email: z3c0 <z3c0@21337.tech>
 Project-URL: Homepage, https://gitlab.com/black-metal-book-club/metallum
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: GNU Lesser General Public License v3 (LGPLv3)
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.11
```

### Comparing `metalarchivist-0.4.2/src/metalarchivist.egg-info/SOURCES.txt` & `metalarchivist-0.4.3/src/metalarchivist.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `metalarchivist-0.4.2/src/test/test_albums.py` & `metalarchivist-0.4.3/src/test/test_albums.py`

 * *Files identical despite different names*

### Comparing `metalarchivist-0.4.2/src/test/test_bands.py` & `metalarchivist-0.4.3/src/test/test_bands.py`

 * *Files identical despite different names*

### Comparing `metalarchivist-0.4.2/src/test/test_genres.py` & `metalarchivist-0.4.3/src/test/test_genres.py`

 * *Files identical despite different names*

### Comparing `metalarchivist-0.4.2/src/test/test_labels.py` & `metalarchivist-0.4.3/src/test/test_labels.py`

 * *Files identical despite different names*

### Comparing `metalarchivist-0.4.2/src/test/test_themes.py` & `metalarchivist-0.4.3/src/test/test_themes.py`

 * *Files identical despite different names*

