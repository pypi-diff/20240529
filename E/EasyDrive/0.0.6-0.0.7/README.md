# Comparing `tmp/easydrive-0.0.6.tar.gz` & `tmp/easydrive-0.0.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "easydrive-0.0.6.tar", last modified: Tue May 28 19:07:47 2024, max compression
+gzip compressed data, was "easydrive-0.0.7.tar", last modified: Tue May 28 23:59:32 2024, max compression
```

## Comparing `easydrive-0.0.6.tar` & `easydrive-0.0.7.tar`

### file list

```diff
@@ -1,19 +1,19 @@
-drwxrwxrwx   0        0        0        0 2024-05-28 19:07:47.831000 easydrive-0.0.6/
--rw-rw-rw-   0        0        0      630 2024-05-28 19:07:47.829491 easydrive-0.0.6/PKG-INFO
--rw-rw-rw-   0        0        0      153 2024-05-28 01:01:02.000000 easydrive-0.0.6/README.md
--rw-rw-rw-   0        0        0      562 2024-05-28 19:07:21.000000 easydrive-0.0.6/pyproject.toml
--rw-rw-rw-   0        0        0       70 2024-05-25 23:07:35.000000 easydrive-0.0.6/requirements.txt
--rw-rw-rw-   0        0        0       42 2024-05-28 19:07:47.831000 easydrive-0.0.6/setup.cfg
-drwxrwxrwx   0        0        0        0 2024-05-28 19:07:47.816457 easydrive-0.0.6/src/
-drwxrwxrwx   0        0        0        0 2024-05-28 19:07:47.823476 easydrive-0.0.6/src/EasyDrive/
--rw-rw-rw-   0        0        0     9692 2024-05-28 03:02:54.000000 easydrive-0.0.6/src/EasyDrive/Drives.py
--rw-rw-rw-   0        0        0      246 2024-05-27 23:52:34.000000 easydrive-0.0.6/src/EasyDrive/Exceptions.py
--rw-rw-rw-   0        0        0    11349 2024-05-28 01:22:34.000000 easydrive-0.0.6/src/EasyDrive/FileSystemTypes.py
--rw-rw-rw-   0        0        0     1677 2024-05-26 02:34:40.000000 easydrive-0.0.6/src/EasyDrive/MIMETypes.py
--rw-rw-rw-   0        0        0       60 2024-05-28 03:51:41.000000 easydrive-0.0.6/src/EasyDrive/__init__.py
-drwxrwxrwx   0        0        0        0 2024-05-28 19:07:47.829491 easydrive-0.0.6/src/EasyDrive.egg-info/
--rw-rw-rw-   0        0        0      630 2024-05-28 19:07:47.000000 easydrive-0.0.6/src/EasyDrive.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      363 2024-05-28 19:07:47.000000 easydrive-0.0.6/src/EasyDrive.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-05-28 19:07:47.000000 easydrive-0.0.6/src/EasyDrive.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       67 2024-05-28 19:07:47.000000 easydrive-0.0.6/src/EasyDrive.egg-info/requires.txt
--rw-rw-rw-   0        0        0       10 2024-05-28 19:07:47.000000 easydrive-0.0.6/src/EasyDrive.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2024-05-28 23:59:32.739029 easydrive-0.0.7/
+-rw-rw-rw-   0        0        0      593 2024-05-28 23:59:32.738021 easydrive-0.0.7/PKG-INFO
+-rw-rw-rw-   0        0        0      153 2024-05-28 01:01:02.000000 easydrive-0.0.7/README.md
+-rw-rw-rw-   0        0        0      562 2024-05-28 23:30:51.000000 easydrive-0.0.7/pyproject.toml
+-rw-rw-rw-   0        0        0       47 2024-05-28 23:34:18.000000 easydrive-0.0.7/requirements.txt
+-rw-rw-rw-   0        0        0       42 2024-05-28 23:59:32.739029 easydrive-0.0.7/setup.cfg
+drwxrwxrwx   0        0        0        0 2024-05-28 23:59:32.714821 easydrive-0.0.7/src/
+drwxrwxrwx   0        0        0        0 2024-05-28 23:59:32.727975 easydrive-0.0.7/src/EasyDrive/
+-rw-rw-rw-   0        0        0    11250 2024-05-28 23:52:18.000000 easydrive-0.0.7/src/EasyDrive/Drives.py
+-rw-rw-rw-   0        0        0      246 2024-05-27 23:52:34.000000 easydrive-0.0.7/src/EasyDrive/Exceptions.py
+-rw-rw-rw-   0        0        0    11347 2024-05-28 23:59:09.000000 easydrive-0.0.7/src/EasyDrive/FileSystemTypes.py
+-rw-rw-rw-   0        0        0     1677 2024-05-26 02:34:40.000000 easydrive-0.0.7/src/EasyDrive/MIMETypes.py
+-rw-rw-rw-   0        0        0       92 2024-05-28 23:45:55.000000 easydrive-0.0.7/src/EasyDrive/__init__.py
+drwxrwxrwx   0        0        0        0 2024-05-28 23:59:32.737522 easydrive-0.0.7/src/EasyDrive.egg-info/
+-rw-rw-rw-   0        0        0      593 2024-05-28 23:59:32.000000 easydrive-0.0.7/src/EasyDrive.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      363 2024-05-28 23:59:32.000000 easydrive-0.0.7/src/EasyDrive.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-05-28 23:59:32.000000 easydrive-0.0.7/src/EasyDrive.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       46 2024-05-28 23:59:32.000000 easydrive-0.0.7/src/EasyDrive.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       10 2024-05-28 23:59:32.000000 easydrive-0.0.7/src/EasyDrive.egg-info/top_level.txt
```

### Comparing `easydrive-0.0.6/pyproject.toml` & `easydrive-0.0.7/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["setuptools>=61.0"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "EasyDrive"
-version = "0.0.6"
+version = "0.0.7"
 authors = [
   { name = "RanchMonster", email = "ranchmonster06@outlook.com" }
 ]
 description = "EasyGoogle Drive access"
 readme = "README.md"
 requires-python = ">3.8"
 classifiers = [
```

### Comparing `easydrive-0.0.6/src/EasyDrive/Drives.py` & `easydrive-0.0.7/src/EasyDrive/Drives.py`

 * *Files 11% similar despite different names*

```diff
@@ -1,19 +1,30 @@
+from math import e
 from os import PathLike
 import os.path
 from typing import Union
 from .Exceptions import InvaildCredentials, DrivePathException
 from google.auth.transport.requests import Request
 from google.oauth2.credentials import Credentials
 from google_auth_oauthlib.flow import InstalledAppFlow
 from googleapiclient.discovery import build
 from googleapiclient.errors import HttpError
 from .FileSystemTypes import *
 from google.oauth2.credentials import Credentials
-
+def one_time_login(credentialsFile: str = "credentials.json")->Credentials:
+        SCOPES = [
+        'https://www.googleapis.com/auth/drive.metadata.readonly',
+        'https://www.googleapis.com/auth/docs',
+        'https://www.googleapis.com/auth/drive',
+        'https://www.googleapis.com/auth/drive.appdata',
+        'https://www.googleapis.com/auth/drive.file'
+    ]
+        flow = InstalledAppFlow.from_client_secrets_file(credentialsFile, SCOPES)
+        creds = flow.run_local_server(port=0)
+        return creds # type: ignore
 def login(tokenFile: str = "token.json", credentialsFile: str = "credentials.json") -> Credentials:
     """
     Logs in to the Google API and returns credentials.
 
     Args:
         tokenFile (PathLike): The path to the token file. Defaults to "token.json".
         credentialsFile (PathLike): The path to the credentials file. Defaults to "credentials.json".
@@ -86,15 +97,14 @@
 
         Returns:
             Folder object at the end of the path.
 
         Raises:
             DrivePathException: If the path is invalid.
         """
-        
         parts = path.split("/") 
         if path.startswith("/"):
             current_folder = self.__root
         else:
             current_folder = self.__currentFolder if not path.startswith("..") else self.__currentFolder.getParent()
         if parts[0] == "" or parts[0] == "..":
             parts.pop(0)
@@ -256,8 +266,31 @@
         path=""
         for folder in folders:
             path+="/"
             if isinstance(folder,RootFolder):continue
             path+=folder.name()
 
         return path
-            
+    def exists(self,path:str)->bool:
+        """
+        check if the path exist
+        Args:
+            path(str):the path you want to check
+        Returns:
+            True if the path exist else returns False
+        """
+        try:
+           folder=self.__transverse_path(path)
+           return True
+        except DrivePathException:
+            try:
+                parts=path.split("/")
+                if len(parts)==1:
+                    if path in [f.name() for f in self.__currentFolder.get_files()] or path in [f.name() for f in self.__currentFolder.get_folders()]:return True
+                    else: return False
+                file = parts.pop()
+                file = file if file !="" else parts.pop()
+                path = path.replace(file,"")
+                folder=self.__transverse_path(path)
+                if file in [f.name() for f in folder.get_files()]:return True
+                else:return False
+            except DrivePathException:return False
```

### Comparing `easydrive-0.0.6/src/EasyDrive/FileSystemTypes.py` & `easydrive-0.0.7/src/EasyDrive/FileSystemTypes.py`

 * *Files 1% similar despite different names*

```diff
@@ -70,15 +70,15 @@
             name(str)
         Returns:
             Folder or None if A folder was found return the folder
         """
         for folder in self.get_folders():
             if folder.name() == name:
                 return folder
-        return folder
+        return None
     
     def get_file_by_name(self, name:str)->Union['File',None]:
         """
         Gets a file by name
         Args:
             name(str)
         Returns:
```

### Comparing `easydrive-0.0.6/src/EasyDrive/MIMETypes.py` & `easydrive-0.0.7/src/EasyDrive/MIMETypes.py`

 * *Files identical despite different names*

