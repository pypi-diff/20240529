# Comparing `tmp/grain_zip_deployer-2024.5.29.2.tar.gz` & `tmp/grain_zip_deployer-2024.5.29.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "grain_zip_deployer-2024.5.29.2.tar", last modified: Wed May 29 08:44:30 2024, max compression
+gzip compressed data, was "grain_zip_deployer-2024.5.29.3.tar", last modified: Wed May 29 08:47:17 2024, max compression
```

## Comparing `grain_zip_deployer-2024.5.29.2.tar` & `grain_zip_deployer-2024.5.29.3.tar`

### file list

```diff
@@ -1,17 +1,17 @@
-drwxrwxrwx   0        0        0        0 2024-05-29 08:44:30.793577 grain_zip_deployer-2024.5.29.2/
--rw-rw-rw-   0        0        0      304 2024-05-29 08:44:30.792580 grain_zip_deployer-2024.5.29.2/PKG-INFO
--rw-rw-rw-   0        0        0     6419 2024-05-28 11:50:17.000000 grain_zip_deployer-2024.5.29.2/README.md
-drwxrwxrwx   0        0        0        0 2024-05-29 08:44:30.777442 grain_zip_deployer-2024.5.29.2/grain_zip_deployer/
--rw-rw-rw-   0        0        0        0 2024-05-28 13:17:17.000000 grain_zip_deployer-2024.5.29.2/grain_zip_deployer/__init__.py
--rw-rw-rw-   0        0        0     6123 2024-05-29 08:44:24.000000 grain_zip_deployer-2024.5.29.2/grain_zip_deployer/main.py
--rw-rw-rw-   0        0        0       44 2024-05-28 11:55:32.000000 grain_zip_deployer-2024.5.29.2/grain_zip_deployer/settings.py
--rw-rw-rw-   0        0        0       27 2024-05-29 08:44:28.000000 grain_zip_deployer-2024.5.29.2/grain_zip_deployer/version.py
-drwxrwxrwx   0        0        0        0 2024-05-29 08:44:30.791577 grain_zip_deployer-2024.5.29.2/grain_zip_deployer.egg-info/
--rw-rw-rw-   0        0        0      304 2024-05-29 08:44:30.000000 grain_zip_deployer-2024.5.29.2/grain_zip_deployer.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      391 2024-05-29 08:44:30.000000 grain_zip_deployer-2024.5.29.2/grain_zip_deployer.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-05-29 08:44:30.000000 grain_zip_deployer-2024.5.29.2/grain_zip_deployer.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       66 2024-05-29 08:44:30.000000 grain_zip_deployer-2024.5.29.2/grain_zip_deployer.egg-info/entry_points.txt
--rw-rw-rw-   0        0        0       29 2024-05-29 08:44:30.000000 grain_zip_deployer-2024.5.29.2/grain_zip_deployer.egg-info/requires.txt
--rw-rw-rw-   0        0        0       19 2024-05-29 08:44:30.000000 grain_zip_deployer-2024.5.29.2/grain_zip_deployer.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2024-05-29 08:44:30.793577 grain_zip_deployer-2024.5.29.2/setup.cfg
--rw-rw-rw-   0        0        0     1122 2024-05-28 13:42:36.000000 grain_zip_deployer-2024.5.29.2/setup.py
+drwxrwxrwx   0        0        0        0 2024-05-29 08:47:17.050869 grain_zip_deployer-2024.5.29.3/
+-rw-rw-rw-   0        0        0      304 2024-05-29 08:47:17.049863 grain_zip_deployer-2024.5.29.3/PKG-INFO
+-rw-rw-rw-   0        0        0     6419 2024-05-28 11:50:17.000000 grain_zip_deployer-2024.5.29.3/README.md
+drwxrwxrwx   0        0        0        0 2024-05-29 08:47:17.037248 grain_zip_deployer-2024.5.29.3/grain_zip_deployer/
+-rw-rw-rw-   0        0        0        0 2024-05-28 13:17:17.000000 grain_zip_deployer-2024.5.29.3/grain_zip_deployer/__init__.py
+-rw-rw-rw-   0        0        0     6060 2024-05-29 08:47:08.000000 grain_zip_deployer-2024.5.29.3/grain_zip_deployer/main.py
+-rw-rw-rw-   0        0        0       44 2024-05-28 11:55:32.000000 grain_zip_deployer-2024.5.29.3/grain_zip_deployer/settings.py
+-rw-rw-rw-   0        0        0       27 2024-05-29 08:47:16.000000 grain_zip_deployer-2024.5.29.3/grain_zip_deployer/version.py
+drwxrwxrwx   0        0        0        0 2024-05-29 08:47:17.047503 grain_zip_deployer-2024.5.29.3/grain_zip_deployer.egg-info/
+-rw-rw-rw-   0        0        0      304 2024-05-29 08:47:16.000000 grain_zip_deployer-2024.5.29.3/grain_zip_deployer.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      391 2024-05-29 08:47:17.000000 grain_zip_deployer-2024.5.29.3/grain_zip_deployer.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-05-29 08:47:16.000000 grain_zip_deployer-2024.5.29.3/grain_zip_deployer.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       66 2024-05-29 08:47:16.000000 grain_zip_deployer-2024.5.29.3/grain_zip_deployer.egg-info/entry_points.txt
+-rw-rw-rw-   0        0        0       29 2024-05-29 08:47:16.000000 grain_zip_deployer-2024.5.29.3/grain_zip_deployer.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       19 2024-05-29 08:47:16.000000 grain_zip_deployer-2024.5.29.3/grain_zip_deployer.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2024-05-29 08:47:17.050869 grain_zip_deployer-2024.5.29.3/setup.cfg
+-rw-rw-rw-   0        0        0     1122 2024-05-28 13:42:36.000000 grain_zip_deployer-2024.5.29.3/setup.py
```

### Comparing `grain_zip_deployer-2024.5.29.2/README.md` & `grain_zip_deployer-2024.5.29.3/README.md`

 * *Files identical despite different names*

### Comparing `grain_zip_deployer-2024.5.29.2/grain_zip_deployer/main.py` & `grain_zip_deployer-2024.5.29.3/grain_zip_deployer/main.py`

 * *Files 7% similar despite different names*

```diff
@@ -43,31 +43,31 @@
     return parser
 
 def upload_to_bucket(bucket_name,
                      project_id,
                      file_name,
                      archive_stream):
 
-    # get short-lived access token and create credentials
-    access_token = get_access_token(lifetime_seconds=60)
+    # get short-lived (1 hour) access token and create credentials
+    access_token = get_access_token()
     credentials = Credentials(token=access_token)
 
     # Initialize the client with the credentials and the project
     client = storage.client.Client(project_id=project_id, credentials=credentials)
 
     bucket = client.get_bucket(bucket_name)
 
     blob_new = bucket.blob(file_name)
     blob_new.upload_from_string(archive_stream.getvalue())
 
-def get_access_token(lifetime_seconds):
+def get_access_token():
 
     # get a temporary access token from the command line that is valid for one minute
     result = subprocess.run(
-            ['gcloud', 'auth', 'print-access-token', '--lifetime', f'{lifetime_seconds}'],
+            ['gcloud', 'auth', 'print-access-token'],
             stdout=subprocess.PIPE,
             stderr=subprocess.PIPE,
             shell=True,
             text=True,
             check=True
         )
```

### Comparing `grain_zip_deployer-2024.5.29.2/setup.py` & `grain_zip_deployer-2024.5.29.3/setup.py`

 * *Files identical despite different names*

