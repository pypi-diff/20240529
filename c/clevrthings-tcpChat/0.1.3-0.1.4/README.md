# Comparing `tmp/clevrthings_tcpchat-0.1.3.tar.gz` & `tmp/clevrthings_tcpchat-0.1.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "clevrthings_tcpchat-0.1.3.tar", last modified: Wed May 29 01:18:53 2024, max compression
+gzip compressed data, was "clevrthings_tcpchat-0.1.4.tar", last modified: Wed May 29 15:02:14 2024, max compression
```

## Comparing `clevrthings_tcpchat-0.1.3.tar` & `clevrthings_tcpchat-0.1.4.tar`

### file list

```diff
@@ -1,14 +1,15 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-29 01:18:53.840021 clevrthings_tcpchat-0.1.3/
--rw-r--r--   0 runner    (1001) docker     (127)     1067 2024-05-29 01:18:49.000000 clevrthings_tcpchat-0.1.3/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)     1570 2024-05-29 01:18:53.840021 clevrthings_tcpchat-0.1.3/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     1047 2024-05-29 01:18:49.000000 clevrthings_tcpchat-0.1.3/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-29 01:18:53.840021 clevrthings_tcpchat-0.1.3/clevrthings_tcpChat.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     1570 2024-05-29 01:18:53.000000 clevrthings_tcpchat-0.1.3/clevrthings_tcpChat.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      237 2024-05-29 01:18:53.000000 clevrthings_tcpchat-0.1.3/clevrthings_tcpChat.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-29 01:18:53.000000 clevrthings_tcpchat-0.1.3/clevrthings_tcpChat.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)        8 2024-05-29 01:18:53.000000 clevrthings_tcpchat-0.1.3/clevrthings_tcpChat.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-29 01:18:53.840021 clevrthings_tcpchat-0.1.3/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)      706 2024-05-29 01:18:49.000000 clevrthings_tcpchat-0.1.3/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-29 01:18:53.840021 clevrthings_tcpchat-0.1.3/tcpChat/
--rw-r--r--   0 runner    (1001) docker     (127)       28 2024-05-29 01:18:49.000000 clevrthings_tcpchat-0.1.3/tcpChat/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     4235 2024-05-29 01:18:49.000000 clevrthings_tcpchat-0.1.3/tcpChat/tcpchat.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-29 15:02:14.607830 clevrthings_tcpchat-0.1.4/
+-rw-r--r--   0 runner    (1001) docker     (127)     1067 2024-05-29 15:02:10.000000 clevrthings_tcpchat-0.1.4/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)     1570 2024-05-29 15:02:14.607830 clevrthings_tcpchat-0.1.4/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     1047 2024-05-29 15:02:10.000000 clevrthings_tcpchat-0.1.4/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-29 15:02:14.607830 clevrthings_tcpchat-0.1.4/clevrthings_tcpChat.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     1570 2024-05-29 15:02:14.000000 clevrthings_tcpchat-0.1.4/clevrthings_tcpChat.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      256 2024-05-29 15:02:14.000000 clevrthings_tcpchat-0.1.4/clevrthings_tcpChat.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-29 15:02:14.000000 clevrthings_tcpchat-0.1.4/clevrthings_tcpChat.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        8 2024-05-29 15:02:14.000000 clevrthings_tcpchat-0.1.4/clevrthings_tcpChat.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-29 15:02:14.607830 clevrthings_tcpchat-0.1.4/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)      706 2024-05-29 15:02:10.000000 clevrthings_tcpchat-0.1.4/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-29 15:02:14.607830 clevrthings_tcpchat-0.1.4/tcpChat/
+-rw-r--r--   0 runner    (1001) docker     (127)       28 2024-05-29 15:02:10.000000 clevrthings_tcpchat-0.1.4/tcpChat/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      650 2024-05-29 15:02:10.000000 clevrthings_tcpchat-0.1.4/tcpChat/example.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4022 2024-05-29 15:02:10.000000 clevrthings_tcpchat-0.1.4/tcpChat/tcpchat.py
```

### Comparing `clevrthings_tcpchat-0.1.3/LICENSE` & `clevrthings_tcpchat-0.1.4/LICENSE`

 * *Files identical despite different names*

### Comparing `clevrthings_tcpchat-0.1.3/PKG-INFO` & `clevrthings_tcpchat-0.1.4/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: clevrthings-tcpChat
-Version: 0.1.3
+Version: 0.1.4
 Summary: A simple Python module for creating a TCP chat connection between two computers to send commands or information.
 Home-page: https://github.com/clevrthings/tcpChat
 Author: Clevrthings
 Author-email: info@clevrthings.com
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

### Comparing `clevrthings_tcpchat-0.1.3/README.md` & `clevrthings_tcpchat-0.1.4/README.md`

 * *Files identical despite different names*

### Comparing `clevrthings_tcpchat-0.1.3/clevrthings_tcpChat.egg-info/PKG-INFO` & `clevrthings_tcpchat-0.1.4/clevrthings_tcpChat.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: clevrthings-tcpChat
-Version: 0.1.3
+Version: 0.1.4
 Summary: A simple Python module for creating a TCP chat connection between two computers to send commands or information.
 Home-page: https://github.com/clevrthings/tcpChat
 Author: Clevrthings
 Author-email: info@clevrthings.com
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

### Comparing `clevrthings_tcpchat-0.1.3/setup.py` & `clevrthings_tcpchat-0.1.4/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from setuptools import setup, find_packages
 
 setup(
     name="clevrthings-tcpChat",
-    version="0.1.3",
+    version="0.1.4",
     packages=find_packages(),
     install_requires=[],
     author="Clevrthings",
     author_email="info@clevrthings.com",
     description="A simple Python module for creating a TCP chat connection between two computers to send commands or information.",
     long_description=open("README.md").read(),
     long_description_content_type="text/markdown",
```

### Comparing `clevrthings_tcpchat-0.1.3/tcpChat/tcpchat.py` & `clevrthings_tcpchat-0.1.4/tcpChat/tcpchat.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,30 +1,27 @@
 import socket
 import threading
-import signal
 import sys
 import time
 
-class tcpchat:
+
+class TCPChat:
     def __init__(self, connect_to_ip: str, callback, port: int = 44785):
         self.server_address = (self.get_local_ip(), port)
         self.client_address = (connect_to_ip, port)
         self.callback = callback
         self.server_socket = socket.socket(socket.AF_INET, socket.SOCK_STREAM)
         self.server_socket.setsockopt(socket.SOL_SOCKET, socket.SO_REUSEADDR, 1)
         self.client_socket = None
         self.server_thread = None
         self.client_ready_event = threading.Event()
         self.connected_event = threading.Event()
         self.stop_event = threading.Event()
         self.retry_connection_interval = 5
 
-        signal.signal(signal.SIGINT, self.signal_handler)
-        signal.signal(signal.SIGTERM, self.signal_handler)
-
     def get_local_ip(self):
         s = socket.socket(socket.AF_INET, socket.SOCK_DGRAM)
         try:
             s.connect(("8.8.8.8", 80))
             ip = s.getsockname()[0]
         except Exception as e:
             print(f"Unable to get local IP address: {e}")
@@ -33,16 +30,15 @@
             s.close()
         return ip
 
     def handle_client_connection(self, connection, client_address):
         print(f"Connection from {client_address}")
         try:
             while not self.stop_event.is_set():
-                data = connection.recv(1024)
-                if data:
+                if data := connection.recv(1024):
                     self.callback(data.decode())
                 else:
                     break
         except Exception as e:
             if not self.stop_event.is_set():
                 print(f"An error occurred with client {client_address}: {e}")
         finally:
@@ -76,15 +72,15 @@
         while not self.connected_event.is_set() and not self.stop_event.is_set():
             try:
                 self.client_socket = socket.socket(socket.AF_INET, socket.SOCK_STREAM)
                 print(f"Connecting to {self.client_address}")
                 self.client_socket.connect(self.client_address)
                 self.connected_event.set()
             except ConnectionRefusedError:
-                print(f"Connection refused, retrying...")
+                print("Connection refused, retrying...")
                 self.client_socket.close()
                 self.client_socket = None
                 time.sleep(self.retry_connection_interval)
             except Exception as e:
                 if not self.stop_event.is_set():
                     print(f"An error occurred while connecting to server: {e}")
                 break
@@ -99,15 +95,13 @@
     def close_connections(self):
         self.stop_event.set()
         if self.server_socket:
             self.server_socket.close()
         if self.client_socket:
             self.client_socket.close()
 
-    def signal_handler(self, sig, frame):
-        print('Exiting gracefully...')
-        self.close_connections()
-        sys.exit(0)
-
     def start(self):
-        self.run_server()
-        self.connect_to_server()
+        try:
+            self.run_server()
+            self.connect_to_server()
+        finally:
+            self.close_connections()
```

