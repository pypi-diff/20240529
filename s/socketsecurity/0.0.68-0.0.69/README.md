# Comparing `tmp/socketsecurity-0.0.68.tar.gz` & `tmp/socketsecurity-0.0.69.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "socketsecurity-0.0.68.tar", last modified: Mon May 20 13:38:41 2024, max compression
+gzip compressed data, was "socketsecurity-0.0.69.tar", last modified: Tue May 28 17:53:50 2024, max compression
```

## Comparing `socketsecurity-0.0.68.tar` & `socketsecurity-0.0.69.tar`

### file list

```diff
@@ -1,25 +1,25 @@
-drwxr-xr-x   0 douglascoburn   (501) staff       (20)        0 2024-05-20 13:38:41.032523 socketsecurity-0.0.68/
--rw-r--r--   0 douglascoburn   (501) staff       (20)     1066 2024-05-17 19:27:22.000000 socketsecurity-0.0.68/LICENSE
--rw-r--r--   0 douglascoburn   (501) staff       (20)     4907 2024-05-20 13:38:41.032335 socketsecurity-0.0.68/PKG-INFO
--rw-r--r--   0 douglascoburn   (501) staff       (20)     4136 2024-05-17 19:24:12.000000 socketsecurity-0.0.68/README.md
--rw-r--r--   0 douglascoburn   (501) staff       (20)     1025 2024-05-20 13:38:31.000000 socketsecurity-0.0.68/pyproject.toml
--rw-r--r--   0 douglascoburn   (501) staff       (20)       38 2024-05-20 13:38:41.032578 socketsecurity-0.0.68/setup.cfg
-drwxr-xr-x   0 douglascoburn   (501) staff       (20)        0 2024-05-20 13:38:41.016445 socketsecurity-0.0.68/socketsecurity/
--rw-r--r--   0 douglascoburn   (501) staff       (20)       98 2024-05-16 10:04:37.000000 socketsecurity-0.0.68/socketsecurity/__init__.py
-drwxr-xr-x   0 douglascoburn   (501) staff       (20)        0 2024-05-20 13:38:41.029808 socketsecurity-0.0.68/socketsecurity/core/
--rw-r--r--   0 douglascoburn   (501) staff       (20)    26247 2024-05-20 13:38:17.000000 socketsecurity-0.0.68/socketsecurity/core/__init__.py
--rw-r--r--   0 douglascoburn   (501) staff       (20)     9282 2024-05-16 08:29:16.000000 socketsecurity-0.0.68/socketsecurity/core/classes.py
--rw-r--r--   0 douglascoburn   (501) staff       (20)      785 2024-05-16 11:28:29.000000 socketsecurity-0.0.68/socketsecurity/core/exceptions.py
--rw-r--r--   0 douglascoburn   (501) staff       (20)    11342 2024-05-16 07:53:25.000000 socketsecurity-0.0.68/socketsecurity/core/github.py
--rw-r--r--   0 douglascoburn   (501) staff       (20)    11041 2024-05-16 11:03:01.000000 socketsecurity-0.0.68/socketsecurity/core/gitlab.py
--rw-r--r--   0 douglascoburn   (501) staff       (20)    68147 2024-05-16 10:03:15.000000 socketsecurity-0.0.68/socketsecurity/core/issues.py
--rw-r--r--   0 douglascoburn   (501) staff       (20) 17442610 2024-05-06 19:45:31.000000 socketsecurity-0.0.68/socketsecurity/core/licenses.py
--rw-r--r--   0 douglascoburn   (501) staff       (20)    11849 2024-05-15 05:15:37.000000 socketsecurity-0.0.68/socketsecurity/core/messages.py
--rw-r--r--   0 douglascoburn   (501) staff       (20)     5912 2024-05-17 19:20:19.000000 socketsecurity-0.0.68/socketsecurity/socketcli.py
-drwxr-xr-x   0 douglascoburn   (501) staff       (20)        0 2024-05-20 13:38:41.032034 socketsecurity-0.0.68/socketsecurity.egg-info/
--rw-r--r--   0 douglascoburn   (501) staff       (20)     4907 2024-05-20 13:38:41.000000 socketsecurity-0.0.68/socketsecurity.egg-info/PKG-INFO
--rw-r--r--   0 douglascoburn   (501) staff       (20)      568 2024-05-20 13:38:41.000000 socketsecurity-0.0.68/socketsecurity.egg-info/SOURCES.txt
--rw-r--r--   0 douglascoburn   (501) staff       (20)        1 2024-05-20 13:38:41.000000 socketsecurity-0.0.68/socketsecurity.egg-info/dependency_links.txt
--rw-r--r--   0 douglascoburn   (501) staff       (20)       59 2024-05-20 13:38:41.000000 socketsecurity-0.0.68/socketsecurity.egg-info/entry_points.txt
--rw-r--r--   0 douglascoburn   (501) staff       (20)       38 2024-05-20 13:38:41.000000 socketsecurity-0.0.68/socketsecurity.egg-info/requires.txt
--rw-r--r--   0 douglascoburn   (501) staff       (20)       15 2024-05-20 13:38:41.000000 socketsecurity-0.0.68/socketsecurity.egg-info/top_level.txt
+drwxr-xr-x   0 douglascoburn   (501) staff       (20)        0 2024-05-28 17:53:50.644332 socketsecurity-0.0.69/
+-rw-r--r--   0 douglascoburn   (501) staff       (20)     1066 2024-05-17 19:27:22.000000 socketsecurity-0.0.69/LICENSE
+-rw-r--r--   0 douglascoburn   (501) staff       (20)     4907 2024-05-28 17:53:50.644146 socketsecurity-0.0.69/PKG-INFO
+-rw-r--r--   0 douglascoburn   (501) staff       (20)     4136 2024-05-17 19:24:12.000000 socketsecurity-0.0.69/README.md
+-rw-r--r--   0 douglascoburn   (501) staff       (20)     1025 2024-05-28 17:53:31.000000 socketsecurity-0.0.69/pyproject.toml
+-rw-r--r--   0 douglascoburn   (501) staff       (20)       38 2024-05-28 17:53:50.644377 socketsecurity-0.0.69/setup.cfg
+drwxr-xr-x   0 douglascoburn   (501) staff       (20)        0 2024-05-28 17:53:50.633849 socketsecurity-0.0.69/socketsecurity/
+-rw-r--r--   0 douglascoburn   (501) staff       (20)       98 2024-05-16 10:04:37.000000 socketsecurity-0.0.69/socketsecurity/__init__.py
+drwxr-xr-x   0 douglascoburn   (501) staff       (20)        0 2024-05-28 17:53:50.643401 socketsecurity-0.0.69/socketsecurity/core/
+-rw-r--r--   0 douglascoburn   (501) staff       (20)    26372 2024-05-28 17:53:41.000000 socketsecurity-0.0.69/socketsecurity/core/__init__.py
+-rw-r--r--   0 douglascoburn   (501) staff       (20)     9282 2024-05-16 08:29:16.000000 socketsecurity-0.0.69/socketsecurity/core/classes.py
+-rw-r--r--   0 douglascoburn   (501) staff       (20)      785 2024-05-16 11:28:29.000000 socketsecurity-0.0.69/socketsecurity/core/exceptions.py
+-rw-r--r--   0 douglascoburn   (501) staff       (20)    11342 2024-05-16 07:53:25.000000 socketsecurity-0.0.69/socketsecurity/core/github.py
+-rw-r--r--   0 douglascoburn   (501) staff       (20)    11041 2024-05-22 14:37:48.000000 socketsecurity-0.0.69/socketsecurity/core/gitlab.py
+-rw-r--r--   0 douglascoburn   (501) staff       (20)    68147 2024-05-16 10:03:15.000000 socketsecurity-0.0.69/socketsecurity/core/issues.py
+-rw-r--r--   0 douglascoburn   (501) staff       (20) 17442610 2024-05-06 19:45:31.000000 socketsecurity-0.0.69/socketsecurity/core/licenses.py
+-rw-r--r--   0 douglascoburn   (501) staff       (20)    11849 2024-05-15 05:15:37.000000 socketsecurity-0.0.69/socketsecurity/core/messages.py
+-rw-r--r--   0 douglascoburn   (501) staff       (20)     5912 2024-05-17 19:20:19.000000 socketsecurity-0.0.69/socketsecurity/socketcli.py
+drwxr-xr-x   0 douglascoburn   (501) staff       (20)        0 2024-05-28 17:53:50.643687 socketsecurity-0.0.69/socketsecurity.egg-info/
+-rw-r--r--   0 douglascoburn   (501) staff       (20)     4907 2024-05-28 17:53:50.000000 socketsecurity-0.0.69/socketsecurity.egg-info/PKG-INFO
+-rw-r--r--   0 douglascoburn   (501) staff       (20)      568 2024-05-28 17:53:50.000000 socketsecurity-0.0.69/socketsecurity.egg-info/SOURCES.txt
+-rw-r--r--   0 douglascoburn   (501) staff       (20)        1 2024-05-28 17:53:50.000000 socketsecurity-0.0.69/socketsecurity.egg-info/dependency_links.txt
+-rw-r--r--   0 douglascoburn   (501) staff       (20)       59 2024-05-28 17:53:50.000000 socketsecurity-0.0.69/socketsecurity.egg-info/entry_points.txt
+-rw-r--r--   0 douglascoburn   (501) staff       (20)       38 2024-05-28 17:53:50.000000 socketsecurity-0.0.69/socketsecurity.egg-info/requires.txt
+-rw-r--r--   0 douglascoburn   (501) staff       (20)       15 2024-05-28 17:53:50.000000 socketsecurity-0.0.69/socketsecurity.egg-info/top_level.txt
```

### Comparing `socketsecurity-0.0.68/LICENSE` & `socketsecurity-0.0.69/LICENSE`

 * *Files identical despite different names*

### Comparing `socketsecurity-0.0.68/PKG-INFO` & `socketsecurity-0.0.69/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: socketsecurity
-Version: 0.0.68
+Version: 0.0.69
 Summary: Socket Security CLI for CI/CD
 Author-email: Douglas Coburn <douglas@socket.dev>
 Maintainer-email: Douglas Coburn <douglas@socket.dev>
 Project-URL: Homepage, https://socket.dev
 Keywords: socketsecurity,socket.dev,sca,oss,security
 Classifier: Development Status :: 4 - Beta
 Classifier: Intended Audience :: Developers
```

### Comparing `socketsecurity-0.0.68/README.md` & `socketsecurity-0.0.69/README.md`

 * *Files identical despite different names*

### Comparing `socketsecurity-0.0.68/pyproject.toml` & `socketsecurity-0.0.69/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["setuptools >= 61.0"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "socketsecurity"
-version = "0.0.68"
+version = "0.0.69"
 requires-python = ">= 3.9"
 dependencies = [
     'requests',
     'mdutils',
     'prettytable',
     'argparse'
 ]
```

### Comparing `socketsecurity-0.0.68/socketsecurity/core/__init__.py` & `socketsecurity-0.0.69/socketsecurity/core/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -21,15 +21,15 @@
 )
 import platform
 from glob import glob
 import time
 
 
 __author__ = 'socket.dev'
-__version__ = '0.0.68'
+__version__ = '0.0.69'
 __all__ = [
     "Core",
     "log",
     "__version__"
 ]
 
 
@@ -321,14 +321,19 @@
             "golang": {
                 "go.mod": {
                     "pattern": "go.mod"
                 },
                 "go.sum": {
                     "pattern": "go.sum"
                 }
+            },
+            "java": {
+                "pom.xml": {
+                    "pattern": "pom.xml"
+                }
             }
         }
         all_files = []
         for ecosystem in socket_globs:
             patterns = socket_globs[ecosystem]
             for file_name in patterns:
                 pattern = patterns[file_name]["pattern"]
```

### Comparing `socketsecurity-0.0.68/socketsecurity/core/classes.py` & `socketsecurity-0.0.69/socketsecurity/core/classes.py`

 * *Files identical despite different names*

### Comparing `socketsecurity-0.0.68/socketsecurity/core/exceptions.py` & `socketsecurity-0.0.69/socketsecurity/core/exceptions.py`

 * *Files identical despite different names*

### Comparing `socketsecurity-0.0.68/socketsecurity/core/github.py` & `socketsecurity-0.0.69/socketsecurity/core/github.py`

 * *Files identical despite different names*

### Comparing `socketsecurity-0.0.68/socketsecurity/core/gitlab.py` & `socketsecurity-0.0.69/socketsecurity/core/gitlab.py`

 * *Files 1% similar despite different names*

```diff
@@ -137,15 +137,15 @@
         self.pr_number = ci_merge_request_iid
         self.pr_name = pr_name
         self.commit_message = ci_commit_message
         self.committer = ci_commit_author
         self.api_token = gitlab_token
         self.project_id = ci_merge_request_project_id
         if self.api_token is None:
-            print("Unable to get gitlab API Token from GH_API_TOKEN")
+            print("Unable to get gitlab API Token from GITLAB_TOKEN")
             sys.exit(2)
 
     @staticmethod
     def check_event_type() -> str:
         if ci_pipeline_source.lower() == "push" or ci_pipeline_source.lower() == 'merge_request_event':
             if ci_merge_request_iid is None or ci_merge_request_iid == "":
                 event_type = "main"
```

### Comparing `socketsecurity-0.0.68/socketsecurity/core/issues.py` & `socketsecurity-0.0.69/socketsecurity/core/issues.py`

 * *Files identical despite different names*

### Comparing `socketsecurity-0.0.68/socketsecurity/core/licenses.py` & `socketsecurity-0.0.69/socketsecurity/core/licenses.py`

 * *Files identical despite different names*

### Comparing `socketsecurity-0.0.68/socketsecurity/core/messages.py` & `socketsecurity-0.0.69/socketsecurity/core/messages.py`

 * *Files identical despite different names*

### Comparing `socketsecurity-0.0.68/socketsecurity/socketcli.py` & `socketsecurity-0.0.69/socketsecurity/socketcli.py`

 * *Files identical despite different names*

### Comparing `socketsecurity-0.0.68/socketsecurity.egg-info/PKG-INFO` & `socketsecurity-0.0.69/socketsecurity.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: socketsecurity
-Version: 0.0.68
+Version: 0.0.69
 Summary: Socket Security CLI for CI/CD
 Author-email: Douglas Coburn <douglas@socket.dev>
 Maintainer-email: Douglas Coburn <douglas@socket.dev>
 Project-URL: Homepage, https://socket.dev
 Keywords: socketsecurity,socket.dev,sca,oss,security
 Classifier: Development Status :: 4 - Beta
 Classifier: Intended Audience :: Developers
```

### Comparing `socketsecurity-0.0.68/socketsecurity.egg-info/SOURCES.txt` & `socketsecurity-0.0.69/socketsecurity.egg-info/SOURCES.txt`

 * *Files identical despite different names*

