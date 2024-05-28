# Comparing `tmp/fiftyone_db-1.1.2rc3.tar.gz` & `tmp/fiftyone_db-1.1.3rc1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "fiftyone_db-1.1.2rc3.tar", last modified: Wed Mar  6 19:44:13 2024, max compression
+gzip compressed data, was "fiftyone_db-1.1.3rc1.tar", last modified: Tue May 28 23:16:47 2024, max compression
```

## Comparing `fiftyone_db-1.1.2rc3.tar` & `fiftyone_db-1.1.3rc1.tar`

### file list

```diff
@@ -1,16 +1,16 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-06 19:44:13.960117 fiftyone_db-1.1.2rc3/
--rw-r--r--   0 runner    (1001) docker     (127)    11349 2024-03-06 19:44:03.000000 fiftyone_db-1.1.2rc3/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)     1278 2024-03-06 19:44:13.960117 fiftyone_db-1.1.2rc3/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)       70 2024-03-06 19:44:05.000000 fiftyone_db-1.1.2rc3/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-06 19:44:13.960117 fiftyone_db-1.1.2rc3/fiftyone_db.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     1278 2024-03-06 19:44:13.000000 fiftyone_db-1.1.2rc3/fiftyone_db.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      214 2024-03-06 19:44:13.000000 fiftyone_db-1.1.2rc3/fiftyone_db.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-03-06 19:44:13.000000 fiftyone_db-1.1.2rc3/fiftyone_db.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)        9 2024-03-06 19:44:13.000000 fiftyone_db-1.1.2rc3/fiftyone_db.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)      132 2024-03-06 19:44:05.000000 fiftyone_db-1.1.2rc3/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-03-06 19:44:13.960117 fiftyone_db-1.1.2rc3/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)    10024 2024-03-06 19:44:05.000000 fiftyone_db-1.1.2rc3/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-06 19:44:13.960117 fiftyone_db-1.1.2rc3/src/
--rw-r--r--   0 runner    (1001) docker     (127)      174 2024-03-06 19:44:05.000000 fiftyone_db-1.1.2rc3/src/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-06 19:44:13.960117 fiftyone_db-1.1.2rc3/tests/
--rw-r--r--   0 runner    (1001) docker     (127)      331 2024-03-06 19:44:05.000000 fiftyone_db-1.1.2rc3/tests/test_db.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-28 23:16:47.238535 fiftyone_db-1.1.3rc1/
+-rw-r--r--   0 runner    (1001) docker     (127)    11349 2024-05-28 23:16:39.000000 fiftyone_db-1.1.3rc1/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)     1278 2024-05-28 23:16:47.238535 fiftyone_db-1.1.3rc1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)       70 2024-05-28 23:16:42.000000 fiftyone_db-1.1.3rc1/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-28 23:16:47.238535 fiftyone_db-1.1.3rc1/fiftyone_db.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     1278 2024-05-28 23:16:47.000000 fiftyone_db-1.1.3rc1/fiftyone_db.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      214 2024-05-28 23:16:47.000000 fiftyone_db-1.1.3rc1/fiftyone_db.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-28 23:16:47.000000 fiftyone_db-1.1.3rc1/fiftyone_db.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        9 2024-05-28 23:16:47.000000 fiftyone_db-1.1.3rc1/fiftyone_db.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      132 2024-05-28 23:16:42.000000 fiftyone_db-1.1.3rc1/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-28 23:16:47.238535 fiftyone_db-1.1.3rc1/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)    10610 2024-05-28 23:16:42.000000 fiftyone_db-1.1.3rc1/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-28 23:16:47.238535 fiftyone_db-1.1.3rc1/src/
+-rw-r--r--   0 runner    (1001) docker     (127)      174 2024-05-28 23:16:42.000000 fiftyone_db-1.1.3rc1/src/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-28 23:16:47.238535 fiftyone_db-1.1.3rc1/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)      331 2024-05-28 23:16:42.000000 fiftyone_db-1.1.3rc1/tests/test_db.py
```

### Comparing `fiftyone_db-1.1.2rc3/LICENSE` & `fiftyone_db-1.1.3rc1/LICENSE`

 * *Files identical despite different names*

### Comparing `fiftyone_db-1.1.2rc3/PKG-INFO` & `fiftyone_db-1.1.3rc1/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: fiftyone_db
-Version: 1.1.2rc3
+Version: 1.1.3rc1
 Summary: FiftyOne DB
 Home-page: https://github.com/voxel51/fiftyone
 Author: Voxel51, Inc.
 Author-email: info@voxel51.com
 License: Apache
 Classifier: Development Status :: 4 - Beta
 Classifier: Intended Audience :: Developers
```

### Comparing `fiftyone_db-1.1.2rc3/fiftyone_db.egg-info/PKG-INFO` & `fiftyone_db-1.1.3rc1/fiftyone_db.egg-info/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: fiftyone_db
-Version: 1.1.2rc3
+Version: 1.1.3rc1
 Summary: FiftyOne DB
 Home-page: https://github.com/voxel51/fiftyone
 Author: Voxel51, Inc.
 Author-email: info@voxel51.com
 License: Apache
 Classifier: Development Status :: 4 - Beta
 Classifier: Intended Audience :: Developers
```

### Comparing `fiftyone_db-1.1.2rc3/setup.py` & `fiftyone_db-1.1.3rc1/setup.py`

 * *Files 3% similar despite different names*

```diff
@@ -33,14 +33,27 @@
             "x86_64": "https://fastdl.mongodb.org/linux/mongodb-linux-x86_64-amazon2-7.0.2.tgz",
         },
         "2023": {
             "aarch64": "https://fastdl.mongodb.org/linux/mongodb-linux-aarch64-amazon2023-7.0.2.tgz",
             "x86_64": "https://fastdl.mongodb.org/linux/mongodb-linux-x86_64-amazon2023-7.0.2.tgz",
         },
     },
+    "centos": {
+        "7": {
+            "x86_64": "https://fastdl.mongodb.org/linux/mongodb-linux-x86_64-rhel70-5.0.4.tgz",
+        },
+        "8": {
+            "aarch64": "https://fastdl.mongodb.org/linux/mongodb-linux-aarch64-rhel82-5.0.22.tgz",
+            "x86_64": "https://fastdl.mongodb.org/linux/mongodb-linux-x86_64-rhel80-5.0.4.tgz",
+        },
+        "9": {
+            "aarch64": "https://fastdl.mongodb.org/linux/mongodb-linux-aarch64-rhel90-7.0.2.tgz",
+            "x86_64": "https://fastdl.mongodb.org/linux/mongodb-linux-x86_64-rhel90-7.0.2.tgz",
+        },
+    },
     "debian": {
         "9": {
             "x86_64": "https://fastdl.mongodb.org/linux/mongodb-linux-x86_64-debian92-5.0.22.tgz",
         },
         "10": {
             "x86_64": "https://fastdl.mongodb.org/linux/mongodb-linux-x86_64-debian10-5.0.22.tgz"
         },
@@ -122,15 +135,15 @@
         pass
 
 
 # mongodb binaries to distribute
 MONGODB_BINARIES = ["mongod"]
 
 
-VERSION = "1.1.2"
+VERSION = "1.1.3"
 
 
 def get_version():
     if "RELEASE_VERSION" in os.environ:
         version = os.environ["RELEASE_VERSION"]
         if not version.startswith(VERSION):
             raise ValueError(
```

