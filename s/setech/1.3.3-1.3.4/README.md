# Comparing `tmp/setech-1.3.3.tar.gz` & `tmp/setech-1.3.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "setech-1.3.3.tar", last modified: Thu May  9 11:04:35 2024, max compression
+gzip compressed data, was "setech-1.3.4.tar", last modified: Wed May 29 12:50:32 2024, max compression
```

## Comparing `setech-1.3.3.tar` & `setech-1.3.4.tar`

### file list

```diff
@@ -1,38 +1,38 @@
-drwxr-xr-x   0 eriks     (1000) eriks     (1000)        0 2024-05-09 11:04:35.664452 setech-1.3.3/
--rw-r--r--   0 eriks     (1000) eriks     (1000)     1059 2024-04-03 10:57:10.000000 setech-1.3.3/LICENCE
--rw-r--r--   0 eriks     (1000) eriks     (1000)     5375 2024-05-09 11:04:35.664452 setech-1.3.3/PKG-INFO
--rw-r--r--   0 eriks     (1000) eriks     (1000)     4473 2024-04-03 21:15:13.000000 setech-1.3.3/README.md
--rw-r--r--   0 eriks     (1000) eriks     (1000)     1932 2024-05-09 11:04:27.000000 setech-1.3.3/pyproject.toml
--rw-r--r--   0 eriks     (1000) eriks     (1000)       38 2024-05-09 11:04:35.664452 setech-1.3.3/setup.cfg
-drwxr-xr-x   0 eriks     (1000) eriks     (1000)        0 2024-05-09 11:04:35.661119 setech-1.3.3/src/
-drwxr-xr-x   0 eriks     (1000) eriks     (1000)        0 2024-05-09 11:04:35.661119 setech-1.3.3/src/setech/
--rw-r--r--   0 eriks     (1000) eriks     (1000)      117 2024-05-09 11:04:27.000000 setech-1.3.3/src/setech/__init__.py
-drwxr-xr-x   0 eriks     (1000) eriks     (1000)        0 2024-05-09 11:04:35.661119 setech-1.3.3/src/setech/api_client/
--rw-r--r--   0 eriks     (1000) eriks     (1000)      115 2024-04-03 13:03:49.000000 setech-1.3.3/src/setech/api_client/__init__.py
--rw-r--r--   0 eriks     (1000) eriks     (1000)     6771 2024-05-09 11:04:05.000000 setech-1.3.3/src/setech/api_client/_base.py
--rw-r--r--   0 eriks     (1000) eriks     (1000)     2332 2024-04-16 11:12:02.000000 setech-1.3.3/src/setech/api_client/async_client.py
--rw-r--r--   0 eriks     (1000) eriks     (1000)     2237 2024-04-16 11:12:02.000000 setech-1.3.3/src/setech/api_client/sync_client.py
-drwxr-xr-x   0 eriks     (1000) eriks     (1000)        0 2024-05-09 11:04:35.661119 setech-1.3.3/src/setech/constants/
--rw-r--r--   0 eriks     (1000) eriks     (1000)      125 2024-04-24 12:12:00.000000 setech-1.3.3/src/setech/constants/__init__.py
--rw-r--r--   0 eriks     (1000) eriks     (1000)      519 2024-04-24 12:12:00.000000 setech-1.3.3/src/setech/constants/date.py
-drwxr-xr-x   0 eriks     (1000) eriks     (1000)        0 2024-05-09 11:04:35.661119 setech-1.3.3/src/setech/logging/
--rw-r--r--   0 eriks     (1000) eriks     (1000)      138 2024-04-10 13:57:32.000000 setech-1.3.3/src/setech/logging/__init__.py
--rw-r--r--   0 eriks     (1000) eriks     (1000)     1394 2024-04-03 20:53:03.000000 setech-1.3.3/src/setech/logging/formatters.py
--rw-r--r--   0 eriks     (1000) eriks     (1000)     1718 2024-05-09 10:54:20.000000 setech-1.3.3/src/setech/logging/handlers.py
--rw-r--r--   0 eriks     (1000) eriks     (1000)        0 2024-03-19 14:21:21.000000 setech-1.3.3/src/setech/py.typed
-drwxr-xr-x   0 eriks     (1000) eriks     (1000)        0 2024-05-09 11:04:35.664452 setech-1.3.3/src/setech/utils/
--rw-r--r--   0 eriks     (1000) eriks     (1000)     1276 2024-04-24 12:12:00.000000 setech-1.3.3/src/setech/utils/__init__.py
--rw-r--r--   0 eriks     (1000) eriks     (1000)      878 2024-04-16 11:12:02.000000 setech-1.3.3/src/setech/utils/numeric.py
--rw-r--r--   0 eriks     (1000) eriks     (1000)     4031 2024-04-24 12:12:00.000000 setech-1.3.3/src/setech/utils/parse.py
--rw-r--r--   0 eriks     (1000) eriks     (1000)     5634 2024-04-24 12:12:00.000000 setech-1.3.3/src/setech/utils/ssn.py
--rw-r--r--   0 eriks     (1000) eriks     (1000)     2140 2024-04-24 12:12:00.000000 setech-1.3.3/src/setech/utils/text.py
--rw-r--r--   0 eriks     (1000) eriks     (1000)      264 2024-04-24 12:12:00.000000 setech-1.3.3/src/setech/utils/time.py
--rw-r--r--   0 eriks     (1000) eriks     (1000)     1082 2024-04-24 12:12:00.000000 setech-1.3.3/src/setech/utils/validators.py
--rw-r--r--   0 eriks     (1000) eriks     (1000)      318 2024-04-24 12:12:00.000000 setech-1.3.3/src/setech/utils/various.py
--rw-r--r--   0 eriks     (1000) eriks     (1000)     1336 2024-04-24 12:12:00.000000 setech-1.3.3/src/setech/utils/warnings.py
-drwxr-xr-x   0 eriks     (1000) eriks     (1000)        0 2024-05-09 11:04:35.664452 setech-1.3.3/src/setech.egg-info/
--rw-r--r--   0 eriks     (1000) eriks     (1000)     5375 2024-05-09 11:04:35.000000 setech-1.3.3/src/setech.egg-info/PKG-INFO
--rw-r--r--   0 eriks     (1000) eriks     (1000)      786 2024-05-09 11:04:35.000000 setech-1.3.3/src/setech.egg-info/SOURCES.txt
--rw-r--r--   0 eriks     (1000) eriks     (1000)        1 2024-05-09 11:04:35.000000 setech-1.3.3/src/setech.egg-info/dependency_links.txt
--rw-r--r--   0 eriks     (1000) eriks     (1000)       65 2024-05-09 11:04:35.000000 setech-1.3.3/src/setech.egg-info/requires.txt
--rw-r--r--   0 eriks     (1000) eriks     (1000)        7 2024-05-09 11:04:35.000000 setech-1.3.3/src/setech.egg-info/top_level.txt
+drwxr-xr-x   0 eriks     (1000) eriks     (1000)        0 2024-05-29 12:50:32.346548 setech-1.3.4/
+-rw-r--r--   0 eriks     (1000) eriks     (1000)     1059 2024-04-03 10:57:10.000000 setech-1.3.4/LICENCE
+-rw-r--r--   0 eriks     (1000) eriks     (1000)     5375 2024-05-29 12:50:32.346548 setech-1.3.4/PKG-INFO
+-rw-r--r--   0 eriks     (1000) eriks     (1000)     4473 2024-04-03 21:15:13.000000 setech-1.3.4/README.md
+-rw-r--r--   0 eriks     (1000) eriks     (1000)     1932 2024-05-29 12:50:26.000000 setech-1.3.4/pyproject.toml
+-rw-r--r--   0 eriks     (1000) eriks     (1000)       38 2024-05-29 12:50:32.346548 setech-1.3.4/setup.cfg
+drwxr-xr-x   0 eriks     (1000) eriks     (1000)        0 2024-05-29 12:50:32.346548 setech-1.3.4/src/
+drwxr-xr-x   0 eriks     (1000) eriks     (1000)        0 2024-05-29 12:50:32.346548 setech-1.3.4/src/setech/
+-rw-r--r--   0 eriks     (1000) eriks     (1000)      117 2024-05-29 12:50:26.000000 setech-1.3.4/src/setech/__init__.py
+drwxr-xr-x   0 eriks     (1000) eriks     (1000)        0 2024-05-29 12:50:32.346548 setech-1.3.4/src/setech/api_client/
+-rw-r--r--   0 eriks     (1000) eriks     (1000)      115 2024-04-03 13:03:49.000000 setech-1.3.4/src/setech/api_client/__init__.py
+-rw-r--r--   0 eriks     (1000) eriks     (1000)     6771 2024-05-09 11:04:05.000000 setech-1.3.4/src/setech/api_client/_base.py
+-rw-r--r--   0 eriks     (1000) eriks     (1000)     2332 2024-04-16 11:12:02.000000 setech-1.3.4/src/setech/api_client/async_client.py
+-rw-r--r--   0 eriks     (1000) eriks     (1000)     2237 2024-04-16 11:12:02.000000 setech-1.3.4/src/setech/api_client/sync_client.py
+drwxr-xr-x   0 eriks     (1000) eriks     (1000)        0 2024-05-29 12:50:32.346548 setech-1.3.4/src/setech/constants/
+-rw-r--r--   0 eriks     (1000) eriks     (1000)      125 2024-04-24 12:12:00.000000 setech-1.3.4/src/setech/constants/__init__.py
+-rw-r--r--   0 eriks     (1000) eriks     (1000)      519 2024-04-24 12:12:00.000000 setech-1.3.4/src/setech/constants/date.py
+drwxr-xr-x   0 eriks     (1000) eriks     (1000)        0 2024-05-29 12:50:32.346548 setech-1.3.4/src/setech/logging/
+-rw-r--r--   0 eriks     (1000) eriks     (1000)      138 2024-04-10 13:57:32.000000 setech-1.3.4/src/setech/logging/__init__.py
+-rw-r--r--   0 eriks     (1000) eriks     (1000)     1394 2024-04-03 20:53:03.000000 setech-1.3.4/src/setech/logging/formatters.py
+-rw-r--r--   0 eriks     (1000) eriks     (1000)     1718 2024-05-09 10:54:20.000000 setech-1.3.4/src/setech/logging/handlers.py
+-rw-r--r--   0 eriks     (1000) eriks     (1000)        0 2024-03-19 14:21:21.000000 setech-1.3.4/src/setech/py.typed
+drwxr-xr-x   0 eriks     (1000) eriks     (1000)        0 2024-05-29 12:50:32.346548 setech-1.3.4/src/setech/utils/
+-rw-r--r--   0 eriks     (1000) eriks     (1000)     1276 2024-04-24 12:12:00.000000 setech-1.3.4/src/setech/utils/__init__.py
+-rw-r--r--   0 eriks     (1000) eriks     (1000)     1084 2024-05-29 12:49:45.000000 setech-1.3.4/src/setech/utils/numeric.py
+-rw-r--r--   0 eriks     (1000) eriks     (1000)     4031 2024-04-24 12:12:00.000000 setech-1.3.4/src/setech/utils/parse.py
+-rw-r--r--   0 eriks     (1000) eriks     (1000)     5865 2024-05-29 12:49:45.000000 setech-1.3.4/src/setech/utils/ssn.py
+-rw-r--r--   0 eriks     (1000) eriks     (1000)     2140 2024-04-24 12:12:00.000000 setech-1.3.4/src/setech/utils/text.py
+-rw-r--r--   0 eriks     (1000) eriks     (1000)      264 2024-04-24 12:12:00.000000 setech-1.3.4/src/setech/utils/time.py
+-rw-r--r--   0 eriks     (1000) eriks     (1000)     1082 2024-04-24 12:12:00.000000 setech-1.3.4/src/setech/utils/validators.py
+-rw-r--r--   0 eriks     (1000) eriks     (1000)      318 2024-04-24 12:12:00.000000 setech-1.3.4/src/setech/utils/various.py
+-rw-r--r--   0 eriks     (1000) eriks     (1000)     1336 2024-04-24 12:12:00.000000 setech-1.3.4/src/setech/utils/warnings.py
+drwxr-xr-x   0 eriks     (1000) eriks     (1000)        0 2024-05-29 12:50:32.346548 setech-1.3.4/src/setech.egg-info/
+-rw-r--r--   0 eriks     (1000) eriks     (1000)     5375 2024-05-29 12:50:32.000000 setech-1.3.4/src/setech.egg-info/PKG-INFO
+-rw-r--r--   0 eriks     (1000) eriks     (1000)      786 2024-05-29 12:50:32.000000 setech-1.3.4/src/setech.egg-info/SOURCES.txt
+-rw-r--r--   0 eriks     (1000) eriks     (1000)        1 2024-05-29 12:50:32.000000 setech-1.3.4/src/setech.egg-info/dependency_links.txt
+-rw-r--r--   0 eriks     (1000) eriks     (1000)       65 2024-05-29 12:50:32.000000 setech-1.3.4/src/setech.egg-info/requires.txt
+-rw-r--r--   0 eriks     (1000) eriks     (1000)        7 2024-05-29 12:50:32.000000 setech-1.3.4/src/setech.egg-info/top_level.txt
```

### Comparing `setech-1.3.3/LICENCE` & `setech-1.3.4/LICENCE`

 * *Files identical despite different names*

### Comparing `setech-1.3.3/PKG-INFO` & `setech-1.3.4/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: setech
-Version: 1.3.3
+Version: 1.3.4
 Summary: Setech utilities
 Author-email: Eriks Karls <eriks.karls@sefinance.lv>
 Project-URL: Homepage, https://pypi.org/project/setech/
 Keywords: setech,logging,api-client,utility,utils
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: Developers
 Classifier: Programming Language :: Python :: 3
```

### Comparing `setech-1.3.3/README.md` & `setech-1.3.4/README.md`

 * *Files identical despite different names*

### Comparing `setech-1.3.3/pyproject.toml` & `setech-1.3.4/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -37,15 +37,15 @@
 
 
 [tool.setuptools.dynamic]
 version = { attr = "setech.__version__" }
 
 
 [tool.bumpversion]
-current_version = "1.3.3"
+current_version = "1.3.4"
 commit = true
 tag = true
 tag_name = "v{new_version}"
 tag_message = "Bump version: {current_version} → {new_version}"
 allow_dirty = false
 parse = "(?P<major>\\d+)\\.(?P<minor>\\d+)\\.(?P<patch>\\d+)"
 serialize = ["{major}.{minor}.{patch}"]
```

### Comparing `setech-1.3.3/src/setech/api_client/_base.py` & `setech-1.3.4/src/setech/api_client/_base.py`

 * *Files identical despite different names*

### Comparing `setech-1.3.3/src/setech/api_client/async_client.py` & `setech-1.3.4/src/setech/api_client/async_client.py`

 * *Files identical despite different names*

### Comparing `setech-1.3.3/src/setech/api_client/sync_client.py` & `setech-1.3.4/src/setech/api_client/sync_client.py`

 * *Files identical despite different names*

### Comparing `setech-1.3.3/src/setech/constants/date.py` & `setech-1.3.4/src/setech/constants/date.py`

 * *Files identical despite different names*

### Comparing `setech-1.3.3/src/setech/logging/formatters.py` & `setech-1.3.4/src/setech/logging/formatters.py`

 * *Files identical despite different names*

### Comparing `setech-1.3.3/src/setech/logging/handlers.py` & `setech-1.3.4/src/setech/logging/handlers.py`

 * *Files identical despite different names*

### Comparing `setech-1.3.3/src/setech/utils/__init__.py` & `setech-1.3.4/src/setech/utils/__init__.py`

 * *Files identical despite different names*

### Comparing `setech-1.3.3/src/setech/utils/parse.py` & `setech-1.3.4/src/setech/utils/parse.py`

 * *Files identical despite different names*

### Comparing `setech-1.3.3/src/setech/utils/ssn.py` & `setech-1.3.4/src/setech/utils/ssn.py`

 * *Files 3% similar despite different names*

```diff
@@ -120,19 +120,28 @@
 
     @property
     def dashed(self) -> str:
         return f"{self.first_part}-{self.second_part}"
 
     @property
     def is_valid(self) -> bool:
+        if not self.is_new_type:
+            try:
+                _ = self.date_of_birth
+            except ValueError:
+                return False
         return str(self._get_checksum_digit()) == self.second_part[-1]
 
     @property
     def date_of_birth(self) -> datetime.date:
-        if int(self.first_part[:2]) > 31:
+        if self.is_new_type:
             raise ValueError("Unable to get date of birth for anonymous personal codes!")
         return datetime.date(
             (1800 if self.second_part[0] == "0" else 1900 if self.second_part[0] == "1" else 2000)
             + int(self.first_part[4:]),
             int(self.first_part[2:4]),
             int(self.first_part[:2]),
         )
+
+    @property
+    def is_new_type(self) -> bool:
+        return int(self.first_part[:2]) > 31
```

### Comparing `setech-1.3.3/src/setech/utils/text.py` & `setech-1.3.4/src/setech/utils/text.py`

 * *Files identical despite different names*

### Comparing `setech-1.3.3/src/setech/utils/validators.py` & `setech-1.3.4/src/setech/utils/validators.py`

 * *Files identical despite different names*

### Comparing `setech-1.3.3/src/setech/utils/warnings.py` & `setech-1.3.4/src/setech/utils/warnings.py`

 * *Files identical despite different names*

### Comparing `setech-1.3.3/src/setech.egg-info/PKG-INFO` & `setech-1.3.4/src/setech.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: setech
-Version: 1.3.3
+Version: 1.3.4
 Summary: Setech utilities
 Author-email: Eriks Karls <eriks.karls@sefinance.lv>
 Project-URL: Homepage, https://pypi.org/project/setech/
 Keywords: setech,logging,api-client,utility,utils
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: Developers
 Classifier: Programming Language :: Python :: 3
```

### Comparing `setech-1.3.3/src/setech.egg-info/SOURCES.txt` & `setech-1.3.4/src/setech.egg-info/SOURCES.txt`

 * *Files identical despite different names*

