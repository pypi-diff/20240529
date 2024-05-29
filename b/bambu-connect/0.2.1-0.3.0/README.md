# Comparing `tmp/bambu-connect-0.2.1.tar.gz` & `tmp/bambu_connect-0.3.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "bambu-connect-0.2.1.tar", last modified: Sat Dec 23 23:31:26 2023, max compression
+gzip compressed data, was "bambu_connect-0.3.0.tar", last modified: Wed May 29 02:23:02 2024, max compression
```

## Comparing `bambu-connect-0.2.1.tar` & `bambu_connect-0.3.0.tar`

### file list

```diff
@@ -1,22 +1,22 @@
-drwxr-xr-x   0 mattcarroll   (501) staff       (20)        0 2023-12-23 23:31:26.363478 bambu-connect-0.2.1/
--rw-r--r--   0 mattcarroll   (501) staff       (20)        0 2023-12-16 05:30:12.000000 bambu-connect-0.2.1/LICENSE
--rw-r--r--   0 mattcarroll   (501) staff       (20)     2427 2023-12-23 23:31:26.363246 bambu-connect-0.2.1/PKG-INFO
--rw-r--r--   0 mattcarroll   (501) staff       (20)     1924 2023-12-18 22:14:21.000000 bambu-connect-0.2.1/README.md
-drwxr-xr-x   0 mattcarroll   (501) staff       (20)        0 2023-12-23 23:31:26.361765 bambu-connect-0.2.1/bambu_connect/
--rw-r--r--   0 mattcarroll   (501) staff       (20)     2042 2023-12-23 23:29:50.000000 bambu-connect-0.2.1/bambu_connect/BambuClient.py
--rw-r--r--   0 mattcarroll   (501) staff       (20)     3213 2023-12-16 05:30:12.000000 bambu-connect-0.2.1/bambu_connect/CameraClient.py
--rw-r--r--   0 mattcarroll   (501) staff       (20)     2308 2023-12-23 23:29:50.000000 bambu-connect-0.2.1/bambu_connect/ExecuteClient.py
--rw-r--r--   0 mattcarroll   (501) staff       (20)     1745 2023-12-17 06:15:49.000000 bambu-connect-0.2.1/bambu_connect/FileClient.py
--rw-r--r--   0 mattcarroll   (501) staff       (20)     1929 2023-12-16 05:30:12.000000 bambu-connect-0.2.1/bambu_connect/WatchClient.py
--rw-r--r--   0 mattcarroll   (501) staff       (20)       64 2023-12-17 06:09:49.000000 bambu-connect-0.2.1/bambu_connect/__init__.py
-drwxr-xr-x   0 mattcarroll   (501) staff       (20)        0 2023-12-23 23:31:26.362724 bambu-connect-0.2.1/bambu_connect/utils/
--rw-r--r--   0 mattcarroll   (501) staff       (20)        0 2023-12-16 05:30:12.000000 bambu-connect-0.2.1/bambu_connect/utils/__init__.py
--rw-r--r--   0 mattcarroll   (501) staff       (20)     7898 2023-12-23 23:29:53.000000 bambu-connect-0.2.1/bambu_connect/utils/models.py
-drwxr-xr-x   0 mattcarroll   (501) staff       (20)        0 2023-12-23 23:31:26.363032 bambu-connect-0.2.1/bambu_connect.egg-info/
--rw-r--r--   0 mattcarroll   (501) staff       (20)     2427 2023-12-23 23:31:26.000000 bambu-connect-0.2.1/bambu_connect.egg-info/PKG-INFO
--rw-r--r--   0 mattcarroll   (501) staff       (20)      451 2023-12-23 23:31:26.000000 bambu-connect-0.2.1/bambu_connect.egg-info/SOURCES.txt
--rw-r--r--   0 mattcarroll   (501) staff       (20)        1 2023-12-23 23:31:26.000000 bambu-connect-0.2.1/bambu_connect.egg-info/dependency_links.txt
--rw-r--r--   0 mattcarroll   (501) staff       (20)       10 2023-12-23 23:31:26.000000 bambu-connect-0.2.1/bambu_connect.egg-info/requires.txt
--rw-r--r--   0 mattcarroll   (501) staff       (20)       14 2023-12-23 23:31:26.000000 bambu-connect-0.2.1/bambu_connect.egg-info/top_level.txt
--rw-r--r--   0 mattcarroll   (501) staff       (20)      614 2023-12-23 23:30:52.000000 bambu-connect-0.2.1/pyproject.toml
--rw-r--r--   0 mattcarroll   (501) staff       (20)       38 2023-12-23 23:31:26.363530 bambu-connect-0.2.1/setup.cfg
+drwxr-xr-x   0 mattcarroll   (501) staff       (20)        0 2024-05-29 02:23:02.353213 bambu_connect-0.3.0/
+-rw-r--r--   0 mattcarroll   (501) staff       (20)        0 2023-12-16 05:30:12.000000 bambu_connect-0.3.0/LICENSE
+-rw-r--r--   0 mattcarroll   (501) staff       (20)     2427 2024-05-29 02:23:02.352969 bambu_connect-0.3.0/PKG-INFO
+-rw-r--r--   0 mattcarroll   (501) staff       (20)     1924 2023-12-18 22:14:21.000000 bambu_connect-0.3.0/README.md
+drwxr-xr-x   0 mattcarroll   (501) staff       (20)        0 2024-05-29 02:23:02.351261 bambu_connect-0.3.0/bambu_connect/
+-rw-r--r--   0 mattcarroll   (501) staff       (20)     2042 2024-05-29 02:19:40.000000 bambu_connect-0.3.0/bambu_connect/BambuClient.py
+-rw-r--r--   0 mattcarroll   (501) staff       (20)     3213 2023-12-16 05:30:12.000000 bambu_connect-0.3.0/bambu_connect/CameraClient.py
+-rw-r--r--   0 mattcarroll   (501) staff       (20)     2340 2024-05-29 02:19:42.000000 bambu_connect-0.3.0/bambu_connect/ExecuteClient.py
+-rw-r--r--   0 mattcarroll   (501) staff       (20)     1745 2023-12-17 06:15:49.000000 bambu_connect-0.3.0/bambu_connect/FileClient.py
+-rw-r--r--   0 mattcarroll   (501) staff       (20)     1961 2024-05-29 02:19:42.000000 bambu_connect-0.3.0/bambu_connect/WatchClient.py
+-rw-r--r--   0 mattcarroll   (501) staff       (20)       64 2023-12-17 06:09:49.000000 bambu_connect-0.3.0/bambu_connect/__init__.py
+drwxr-xr-x   0 mattcarroll   (501) staff       (20)        0 2024-05-29 02:23:02.352255 bambu_connect-0.3.0/bambu_connect/utils/
+-rw-r--r--   0 mattcarroll   (501) staff       (20)        0 2023-12-16 05:30:12.000000 bambu_connect-0.3.0/bambu_connect/utils/__init__.py
+-rw-r--r--   0 mattcarroll   (501) staff       (20)     7898 2024-05-29 02:19:40.000000 bambu_connect-0.3.0/bambu_connect/utils/models.py
+drwxr-xr-x   0 mattcarroll   (501) staff       (20)        0 2024-05-29 02:23:02.352629 bambu_connect-0.3.0/bambu_connect.egg-info/
+-rw-r--r--   0 mattcarroll   (501) staff       (20)     2427 2024-05-29 02:23:02.000000 bambu_connect-0.3.0/bambu_connect.egg-info/PKG-INFO
+-rw-r--r--   0 mattcarroll   (501) staff       (20)      451 2024-05-29 02:23:02.000000 bambu_connect-0.3.0/bambu_connect.egg-info/SOURCES.txt
+-rw-r--r--   0 mattcarroll   (501) staff       (20)        1 2024-05-29 02:23:02.000000 bambu_connect-0.3.0/bambu_connect.egg-info/dependency_links.txt
+-rw-r--r--   0 mattcarroll   (501) staff       (20)       10 2024-05-29 02:23:02.000000 bambu_connect-0.3.0/bambu_connect.egg-info/requires.txt
+-rw-r--r--   0 mattcarroll   (501) staff       (20)       14 2024-05-29 02:23:02.000000 bambu_connect-0.3.0/bambu_connect.egg-info/top_level.txt
+-rw-r--r--   0 mattcarroll   (501) staff       (20)      614 2024-05-29 02:19:52.000000 bambu_connect-0.3.0/pyproject.toml
+-rw-r--r--   0 mattcarroll   (501) staff       (20)       38 2024-05-29 02:23:02.353268 bambu_connect-0.3.0/setup.cfg
```

### Comparing `bambu-connect-0.2.1/PKG-INFO` & `bambu_connect-0.3.0/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: bambu-connect
-Version: 0.2.1
+Version: 0.3.0
 Summary: Connect with your bambu printer to send and receive mqtt messages and view the Camera
 Author-email: Matt Carroll <mwcarroll12@gmail.com>
 Project-URL: Homepage, https://github.com/mattcar15/bambu-connect
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Description-Content-Type: text/markdown
```

### Comparing `bambu-connect-0.2.1/README.md` & `bambu_connect-0.3.0/README.md`

 * *Files identical despite different names*

### Comparing `bambu-connect-0.2.1/bambu_connect/BambuClient.py` & `bambu_connect-0.3.0/bambu_connect/BambuClient.py`

 * *Files identical despite different names*

### Comparing `bambu-connect-0.2.1/bambu_connect/CameraClient.py` & `bambu_connect-0.3.0/bambu_connect/CameraClient.py`

 * *Files identical despite different names*

### Comparing `bambu-connect-0.2.1/bambu_connect/ExecuteClient.py` & `bambu_connect-0.3.0/bambu_connect/ExecuteClient.py`

 * *Files 3% similar despite different names*

```diff
@@ -9,15 +9,15 @@
     def __init__(self, hostname: str, access_code: str, serial: str):
         self.hostname = hostname
         self.access_code = access_code
         self.serial = serial
         self.client = self.__setup_mqtt_client()
 
     def __setup_mqtt_client(self):
-        client = mqtt.Client()
+        client = mqtt.Client(mqtt.CallbackAPIVersion.VERSION1)
         client.username_pw_set("bblp", self.access_code)
         client.tls_set(tls_version=ssl.PROTOCOL_TLS, cert_reqs=ssl.CERT_NONE)
         client.tls_insecure_set(True)
         client.connect(self.hostname, 8883, 60)
         return client
 
     def disconnect(self):
```

### Comparing `bambu-connect-0.2.1/bambu_connect/FileClient.py` & `bambu_connect-0.3.0/bambu_connect/FileClient.py`

 * *Files identical despite different names*

### Comparing `bambu-connect-0.2.1/bambu_connect/WatchClient.py` & `bambu_connect-0.3.0/bambu_connect/WatchClient.py`

 * *Files 5% similar despite different names*

```diff
@@ -13,15 +13,15 @@
         self.serial = serial
         self.client = self.__setup_mqtt_client()
         self.values = {}
         self.printerStatus = None
         self.message_callback = None
 
     def __setup_mqtt_client(self) -> mqtt.Client:
-        client = mqtt.Client()
+        client = mqtt.Client(mqtt.CallbackAPIVersion.VERSION1)
         client.username_pw_set("bblp", self.access_code)
         client.tls_set(tls_version=ssl.PROTOCOL_TLS, cert_reqs=ssl.CERT_NONE)
         client.tls_insecure_set(True)
         client.on_connect = self.on_connect
         client.on_message = self.on_message
         return client
```

### Comparing `bambu-connect-0.2.1/bambu_connect/utils/models.py` & `bambu_connect-0.3.0/bambu_connect/utils/models.py`

 * *Files identical despite different names*

### Comparing `bambu-connect-0.2.1/bambu_connect.egg-info/PKG-INFO` & `bambu_connect-0.3.0/bambu_connect.egg-info/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: bambu-connect
-Version: 0.2.1
+Version: 0.3.0
 Summary: Connect with your bambu printer to send and receive mqtt messages and view the Camera
 Author-email: Matt Carroll <mwcarroll12@gmail.com>
 Project-URL: Homepage, https://github.com/mattcar15/bambu-connect
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Description-Content-Type: text/markdown
```

### Comparing `bambu-connect-0.2.1/pyproject.toml` & `bambu_connect-0.3.0/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["setuptools", "wheel"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "bambu-connect"
-version = "0.2.1"
+version = "0.3.0"
 description = "Connect with your bambu printer to send and receive mqtt messages and view the Camera"
 readme = "README.md"
 license = { file = "LICENSE" }
 urls = { "Homepage" = "https://github.com/mattcar15/bambu-connect" }
 authors = [{ name = "Matt Carroll", email = "mwcarroll12@gmail.com" }]
 classifiers = [
     "Programming Language :: Python :: 3",
```

