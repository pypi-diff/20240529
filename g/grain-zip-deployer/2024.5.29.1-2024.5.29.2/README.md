# Comparing `tmp/grain_zip_deployer-2024.5.29.1.tar.gz` & `tmp/grain_zip_deployer-2024.5.29.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "grain_zip_deployer-2024.5.29.1.tar", last modified: Wed May 29 08:36:54 2024, max compression
+gzip compressed data, was "grain_zip_deployer-2024.5.29.2.tar", last modified: Wed May 29 08:44:30 2024, max compression
```

## Comparing `grain_zip_deployer-2024.5.29.1.tar` & `grain_zip_deployer-2024.5.29.2.tar`

### file list

```diff
@@ -1,17 +1,17 @@
-drwxrwxrwx   0        0        0        0 2024-05-29 08:36:54.850927 grain_zip_deployer-2024.5.29.1/
--rw-rw-rw-   0        0        0      304 2024-05-29 08:36:54.847337 grain_zip_deployer-2024.5.29.1/PKG-INFO
--rw-rw-rw-   0        0        0     6419 2024-05-28 11:50:17.000000 grain_zip_deployer-2024.5.29.1/README.md
-drwxrwxrwx   0        0        0        0 2024-05-29 08:36:54.829647 grain_zip_deployer-2024.5.29.1/grain_zip_deployer/
--rw-rw-rw-   0        0        0        0 2024-05-28 13:17:17.000000 grain_zip_deployer-2024.5.29.1/grain_zip_deployer/__init__.py
--rw-rw-rw-   0        0        0     6119 2024-05-29 08:35:22.000000 grain_zip_deployer-2024.5.29.1/grain_zip_deployer/main.py
--rw-rw-rw-   0        0        0       44 2024-05-28 11:55:32.000000 grain_zip_deployer-2024.5.29.1/grain_zip_deployer/settings.py
--rw-rw-rw-   0        0        0       27 2024-05-29 08:36:09.000000 grain_zip_deployer-2024.5.29.1/grain_zip_deployer/version.py
-drwxrwxrwx   0        0        0        0 2024-05-29 08:36:54.845660 grain_zip_deployer-2024.5.29.1/grain_zip_deployer.egg-info/
--rw-rw-rw-   0        0        0      304 2024-05-29 08:36:54.000000 grain_zip_deployer-2024.5.29.1/grain_zip_deployer.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      391 2024-05-29 08:36:54.000000 grain_zip_deployer-2024.5.29.1/grain_zip_deployer.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-05-29 08:36:54.000000 grain_zip_deployer-2024.5.29.1/grain_zip_deployer.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       66 2024-05-29 08:36:54.000000 grain_zip_deployer-2024.5.29.1/grain_zip_deployer.egg-info/entry_points.txt
--rw-rw-rw-   0        0        0       29 2024-05-29 08:36:54.000000 grain_zip_deployer-2024.5.29.1/grain_zip_deployer.egg-info/requires.txt
--rw-rw-rw-   0        0        0       19 2024-05-29 08:36:54.000000 grain_zip_deployer-2024.5.29.1/grain_zip_deployer.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2024-05-29 08:36:54.852069 grain_zip_deployer-2024.5.29.1/setup.cfg
--rw-rw-rw-   0        0        0     1122 2024-05-28 13:42:36.000000 grain_zip_deployer-2024.5.29.1/setup.py
+drwxrwxrwx   0        0        0        0 2024-05-29 08:44:30.793577 grain_zip_deployer-2024.5.29.2/
+-rw-rw-rw-   0        0        0      304 2024-05-29 08:44:30.792580 grain_zip_deployer-2024.5.29.2/PKG-INFO
+-rw-rw-rw-   0        0        0     6419 2024-05-28 11:50:17.000000 grain_zip_deployer-2024.5.29.2/README.md
+drwxrwxrwx   0        0        0        0 2024-05-29 08:44:30.777442 grain_zip_deployer-2024.5.29.2/grain_zip_deployer/
+-rw-rw-rw-   0        0        0        0 2024-05-28 13:17:17.000000 grain_zip_deployer-2024.5.29.2/grain_zip_deployer/__init__.py
+-rw-rw-rw-   0        0        0     6123 2024-05-29 08:44:24.000000 grain_zip_deployer-2024.5.29.2/grain_zip_deployer/main.py
+-rw-rw-rw-   0        0        0       44 2024-05-28 11:55:32.000000 grain_zip_deployer-2024.5.29.2/grain_zip_deployer/settings.py
+-rw-rw-rw-   0        0        0       27 2024-05-29 08:44:28.000000 grain_zip_deployer-2024.5.29.2/grain_zip_deployer/version.py
+drwxrwxrwx   0        0        0        0 2024-05-29 08:44:30.791577 grain_zip_deployer-2024.5.29.2/grain_zip_deployer.egg-info/
+-rw-rw-rw-   0        0        0      304 2024-05-29 08:44:30.000000 grain_zip_deployer-2024.5.29.2/grain_zip_deployer.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      391 2024-05-29 08:44:30.000000 grain_zip_deployer-2024.5.29.2/grain_zip_deployer.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-05-29 08:44:30.000000 grain_zip_deployer-2024.5.29.2/grain_zip_deployer.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       66 2024-05-29 08:44:30.000000 grain_zip_deployer-2024.5.29.2/grain_zip_deployer.egg-info/entry_points.txt
+-rw-rw-rw-   0        0        0       29 2024-05-29 08:44:30.000000 grain_zip_deployer-2024.5.29.2/grain_zip_deployer.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       19 2024-05-29 08:44:30.000000 grain_zip_deployer-2024.5.29.2/grain_zip_deployer.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2024-05-29 08:44:30.793577 grain_zip_deployer-2024.5.29.2/setup.cfg
+-rw-rw-rw-   0        0        0     1122 2024-05-28 13:42:36.000000 grain_zip_deployer-2024.5.29.2/setup.py
```

### Comparing `grain_zip_deployer-2024.5.29.1/README.md` & `grain_zip_deployer-2024.5.29.2/README.md`

 * *Files identical despite different names*

### Comparing `grain_zip_deployer-2024.5.29.1/grain_zip_deployer/main.py` & `grain_zip_deployer-2024.5.29.2/grain_zip_deployer/main.py`

 * *Files 2% similar despite different names*

```diff
@@ -152,16 +152,16 @@
 
     parser = init_argparse()
     args = parser.parse_args()
     
     archive_name = args.name
     
     # get the directory with source files. Current working directory by default
-    if not args.path is None:
-        source_dir = args.path
+    if not args.folder is None:
+        source_dir = args.folder
     else:
         source_dir = Path.cwd()
 
     if args.upload:
 
         # when uploading, the bucket is mandatory
         if args.bucket is None:
```

### Comparing `grain_zip_deployer-2024.5.29.1/setup.py` & `grain_zip_deployer-2024.5.29.2/setup.py`

 * *Files identical despite different names*

