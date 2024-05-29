# Comparing `tmp/kumparanian-1.0.5rc6.tar.gz` & `tmp/kumparanian-1.1.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "kumparanian-1.0.5rc6.tar", max compression
+gzip compressed data, was "kumparanian-1.1.0.tar", max compression
```

## Comparing `kumparanian-1.0.5rc6.tar` & `kumparanian-1.1.0.tar`

### file list

```diff
@@ -1,14 +1,14 @@
--rw-r--r--   0        0        0     1486 2024-05-07 14:10:12.509016 kumparanian-1.0.5rc6/LICENSE
--rw-r--r--   0        0        0     2626 2024-05-07 14:10:12.509300 kumparanian-1.0.5rc6/README.md
--rw-r--r--   0        0        0        0 2024-05-07 14:10:12.509834 kumparanian-1.0.5rc6/kumparanian/__init__.py
--rw-r--r--   0        0        0       30 2024-05-09 08:24:12.247895 kumparanian-1.0.5rc6/kumparanian/__main__.py
--rw-r--r--   0        0        0     3183 2024-05-09 09:47:17.208675 kumparanian-1.0.5rc6/kumparanian/cli.py
--rw-r--r--   0        0        0      564 2024-05-09 09:47:17.184439 kumparanian-1.0.5rc6/kumparanian/de/__init__.py
--rw-r--r--   0        0        0     2264 2024-05-09 09:47:17.200158 kumparanian-1.0.5rc6/kumparanian/de/dataset.py
--rw-r--r--   0        0        0     1480 2024-05-07 14:10:12.510724 kumparanian-1.0.5rc6/kumparanian/de/help_text.py
--rw-r--r--   0        0        0     5446 2024-05-09 09:47:17.218676 kumparanian-1.0.5rc6/kumparanian/de/submission.py
--rw-r--r--   0        0        0      392 2024-05-09 09:47:17.187433 kumparanian-1.0.5rc6/kumparanian/ds/__init__.py
--rw-r--r--   0        0        0      647 2024-05-07 14:10:12.511170 kumparanian-1.0.5rc6/kumparanian/ds/help_text.py
--rw-r--r--   0        0        0     2322 2024-05-09 09:47:17.202032 kumparanian-1.0.5rc6/kumparanian/ds/model.py
--rw-r--r--   0        0        0      897 2024-05-09 09:49:47.051964 kumparanian-1.0.5rc6/pyproject.toml
--rw-r--r--   0        0        0     3447 1970-01-01 00:00:00.000000 kumparanian-1.0.5rc6/PKG-INFO
+-rw-r--r--   0        0        0     1486 2024-05-07 14:10:12.509016 kumparanian-1.1.0/LICENSE
+-rw-r--r--   0        0        0     2626 2024-05-07 14:10:12.509300 kumparanian-1.1.0/README.md
+-rw-r--r--   0        0        0        0 2024-05-07 14:10:12.509834 kumparanian-1.1.0/kumparanian/__init__.py
+-rw-r--r--   0        0        0       30 2024-05-09 08:24:12.247895 kumparanian-1.1.0/kumparanian/__main__.py
+-rw-r--r--   0        0        0     3183 2024-05-29 10:24:09.402664 kumparanian-1.1.0/kumparanian/cli.py
+-rw-r--r--   0        0        0      564 2024-05-29 10:24:09.403171 kumparanian-1.1.0/kumparanian/de/__init__.py
+-rw-r--r--   0        0        0     2264 2024-05-29 10:24:09.403627 kumparanian-1.1.0/kumparanian/de/dataset.py
+-rw-r--r--   0        0        0     1480 2024-05-07 14:10:12.510724 kumparanian-1.1.0/kumparanian/de/help_text.py
+-rw-r--r--   0        0        0     5446 2024-05-29 10:24:09.404362 kumparanian-1.1.0/kumparanian/de/submission.py
+-rw-r--r--   0        0        0      392 2024-05-29 10:24:09.404822 kumparanian-1.1.0/kumparanian/ds/__init__.py
+-rw-r--r--   0        0        0      647 2024-05-07 14:10:12.511170 kumparanian-1.1.0/kumparanian/ds/help_text.py
+-rw-r--r--   0        0        0     2322 2024-05-29 10:24:09.405263 kumparanian-1.1.0/kumparanian/ds/model.py
+-rw-r--r--   0        0        0      894 2024-05-29 10:24:09.405766 kumparanian-1.1.0/pyproject.toml
+-rw-r--r--   0        0        0     3444 1970-01-01 00:00:00.000000 kumparanian-1.1.0/PKG-INFO
```

### Comparing `kumparanian-1.0.5rc6/LICENSE` & `kumparanian-1.1.0/LICENSE`

 * *Files identical despite different names*

### Comparing `kumparanian-1.0.5rc6/README.md` & `kumparanian-1.1.0/README.md`

 * *Files identical despite different names*

### Comparing `kumparanian-1.0.5rc6/kumparanian/cli.py` & `kumparanian-1.1.0/kumparanian/cli.py`

 * *Files identical despite different names*

### Comparing `kumparanian-1.0.5rc6/kumparanian/de/__init__.py` & `kumparanian-1.1.0/kumparanian/de/__init__.py`

 * *Files identical despite different names*

### Comparing `kumparanian-1.0.5rc6/kumparanian/de/dataset.py` & `kumparanian-1.1.0/kumparanian/de/dataset.py`

 * *Files identical despite different names*

### Comparing `kumparanian-1.0.5rc6/kumparanian/de/help_text.py` & `kumparanian-1.1.0/kumparanian/de/help_text.py`

 * *Files identical despite different names*

### Comparing `kumparanian-1.0.5rc6/kumparanian/de/submission.py` & `kumparanian-1.1.0/kumparanian/de/submission.py`

 * *Files identical despite different names*

### Comparing `kumparanian-1.0.5rc6/kumparanian/ds/help_text.py` & `kumparanian-1.1.0/kumparanian/ds/help_text.py`

 * *Files identical despite different names*

### Comparing `kumparanian-1.0.5rc6/kumparanian/ds/model.py` & `kumparanian-1.1.0/kumparanian/ds/model.py`

 * *Files identical despite different names*

### Comparing `kumparanian-1.0.5rc6/pyproject.toml` & `kumparanian-1.1.0/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "kumparanian"
-version = "1.0.5rc6"
+version = "1.1.0"
 description = "Kumparanian CLI"
 authors = ["Zavli Juwantara <zavli.juwantara@kumparan.com>"]
 repository = "https://github.com/kumparan/kumparanian"
 maintainers = [
     "Bayu <bayualdiyansyah@gmail.com>",
     "Raden <radenmaharjo@gmail.com>",
     "Aslam <aslam.hadi@kumparan.com>",
```

### Comparing `kumparanian-1.0.5rc6/PKG-INFO` & `kumparanian-1.1.0/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: kumparanian
-Version: 1.0.5rc6
+Version: 1.1.0
 Summary: Kumparanian CLI
 Home-page: https://github.com/kumparan/kumparanian
 License: kumparan
 Author: Zavli Juwantara
 Author-email: zavli.juwantara@kumparan.com
 Maintainer: Bayu
 Maintainer-email: bayualdiyansyah@gmail.com
```

