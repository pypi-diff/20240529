# Comparing `tmp/grain_zip_deployer-2025.5.28.1.tar.gz` & `tmp/grain_zip_deployer-2025.5.28.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "grain_zip_deployer-2025.5.28.1.tar", last modified: Tue May 28 14:02:37 2024, max compression
+gzip compressed data, was "grain_zip_deployer-2025.5.28.2.tar", last modified: Tue May 28 14:04:21 2024, max compression
```

## Comparing `grain_zip_deployer-2025.5.28.1.tar` & `grain_zip_deployer-2025.5.28.2.tar`

### file list

```diff
@@ -1,17 +1,17 @@
-drwxrwxrwx   0        0        0        0 2024-05-28 14:02:37.122742 grain_zip_deployer-2025.5.28.1/
--rw-rw-rw-   0        0        0      304 2024-05-28 14:02:37.122742 grain_zip_deployer-2025.5.28.1/PKG-INFO
--rw-rw-rw-   0        0        0     6419 2024-05-28 11:50:17.000000 grain_zip_deployer-2025.5.28.1/README.md
-drwxrwxrwx   0        0        0        0 2024-05-28 14:02:37.105455 grain_zip_deployer-2025.5.28.1/grain_zip_deployer/
--rw-rw-rw-   0        0        0        0 2024-05-28 13:17:17.000000 grain_zip_deployer-2025.5.28.1/grain_zip_deployer/__init__.py
--rw-rw-rw-   0        0        0     4812 2024-05-28 14:01:48.000000 grain_zip_deployer-2025.5.28.1/grain_zip_deployer/main.py
--rw-rw-rw-   0        0        0       44 2024-05-28 11:55:32.000000 grain_zip_deployer-2025.5.28.1/grain_zip_deployer/settings.py
--rw-rw-rw-   0        0        0       27 2024-05-28 14:02:06.000000 grain_zip_deployer-2025.5.28.1/grain_zip_deployer/version.py
-drwxrwxrwx   0        0        0        0 2024-05-28 14:02:37.122742 grain_zip_deployer-2025.5.28.1/grain_zip_deployer.egg-info/
--rw-rw-rw-   0        0        0      304 2024-05-28 14:02:37.000000 grain_zip_deployer-2025.5.28.1/grain_zip_deployer.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      391 2024-05-28 14:02:37.000000 grain_zip_deployer-2025.5.28.1/grain_zip_deployer.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-05-28 14:02:37.000000 grain_zip_deployer-2025.5.28.1/grain_zip_deployer.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       66 2024-05-28 14:02:37.000000 grain_zip_deployer-2025.5.28.1/grain_zip_deployer.egg-info/entry_points.txt
--rw-rw-rw-   0        0        0       29 2024-05-28 14:02:37.000000 grain_zip_deployer-2025.5.28.1/grain_zip_deployer.egg-info/requires.txt
--rw-rw-rw-   0        0        0       19 2024-05-28 14:02:37.000000 grain_zip_deployer-2025.5.28.1/grain_zip_deployer.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2024-05-28 14:02:37.122742 grain_zip_deployer-2025.5.28.1/setup.cfg
--rw-rw-rw-   0        0        0     1122 2024-05-28 13:42:36.000000 grain_zip_deployer-2025.5.28.1/setup.py
+drwxrwxrwx   0        0        0        0 2024-05-28 14:04:21.032109 grain_zip_deployer-2025.5.28.2/
+-rw-rw-rw-   0        0        0      304 2024-05-28 14:04:21.030088 grain_zip_deployer-2025.5.28.2/PKG-INFO
+-rw-rw-rw-   0        0        0     6419 2024-05-28 11:50:17.000000 grain_zip_deployer-2025.5.28.2/README.md
+drwxrwxrwx   0        0        0        0 2024-05-28 14:04:21.015014 grain_zip_deployer-2025.5.28.2/grain_zip_deployer/
+-rw-rw-rw-   0        0        0        0 2024-05-28 13:17:17.000000 grain_zip_deployer-2025.5.28.2/grain_zip_deployer/__init__.py
+-rw-rw-rw-   0        0        0     4784 2024-05-28 14:04:10.000000 grain_zip_deployer-2025.5.28.2/grain_zip_deployer/main.py
+-rw-rw-rw-   0        0        0       44 2024-05-28 11:55:32.000000 grain_zip_deployer-2025.5.28.2/grain_zip_deployer/settings.py
+-rw-rw-rw-   0        0        0       27 2024-05-28 14:04:16.000000 grain_zip_deployer-2025.5.28.2/grain_zip_deployer/version.py
+drwxrwxrwx   0        0        0        0 2024-05-28 14:04:21.030088 grain_zip_deployer-2025.5.28.2/grain_zip_deployer.egg-info/
+-rw-rw-rw-   0        0        0      304 2024-05-28 14:04:20.000000 grain_zip_deployer-2025.5.28.2/grain_zip_deployer.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      391 2024-05-28 14:04:20.000000 grain_zip_deployer-2025.5.28.2/grain_zip_deployer.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-05-28 14:04:20.000000 grain_zip_deployer-2025.5.28.2/grain_zip_deployer.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       66 2024-05-28 14:04:20.000000 grain_zip_deployer-2025.5.28.2/grain_zip_deployer.egg-info/entry_points.txt
+-rw-rw-rw-   0        0        0       29 2024-05-28 14:04:20.000000 grain_zip_deployer-2025.5.28.2/grain_zip_deployer.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       19 2024-05-28 14:04:20.000000 grain_zip_deployer-2025.5.28.2/grain_zip_deployer.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2024-05-28 14:04:21.032109 grain_zip_deployer-2025.5.28.2/setup.cfg
+-rw-rw-rw-   0        0        0     1122 2024-05-28 13:42:36.000000 grain_zip_deployer-2025.5.28.2/setup.py
```

### Comparing `grain_zip_deployer-2025.5.28.1/README.md` & `grain_zip_deployer-2025.5.28.2/README.md`

 * *Files identical despite different names*

### Comparing `grain_zip_deployer-2025.5.28.1/grain_zip_deployer/main.py` & `grain_zip_deployer-2025.5.28.2/grain_zip_deployer/main.py`

 * *Files 2% similar despite different names*

```diff
@@ -36,22 +36,18 @@
 def upload_to_bucket(bucket_name,
                      file_name,
                      value):
 
     access_token = get_access_token()
     credentials = Credentials(token=access_token)
 
-    return
-
     # Initialize the client with the credentials
     client = storage.Client(credentials=credentials)
     bucket = client.get_bucket(bucket_name)
 
-    return
-
     blob_new = bucket.blob(file_name)
     blob_new.upload_from_string(value)
 
 def get_access_token():
 
     result = subprocess.run(
             ['gcloud', 'auth', 'print-access-token'],
```

### Comparing `grain_zip_deployer-2025.5.28.1/setup.py` & `grain_zip_deployer-2025.5.28.2/setup.py`

 * *Files identical despite different names*

