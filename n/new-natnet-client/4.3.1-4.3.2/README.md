# Comparing `tmp/new_natnet_client-4.3.1.tar.gz` & `tmp/new_natnet_client-4.3.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "new_natnet_client-4.3.1.tar", max compression
+gzip compressed data, was "new_natnet_client-4.3.2.tar", max compression
```

## Comparing `new_natnet_client-4.3.1.tar` & `new_natnet_client-4.3.2.tar`

### file list

```diff
@@ -1,8 +1,8 @@
--rw-r--r--   0        0        0      958 2024-05-11 18:54:03.498484 new_natnet_client-4.3.1/LICENSE
--rw-r--r--   0        0        0     1489 2024-05-14 21:27:27.319169 new_natnet_client-4.3.1/README.md
--rw-r--r--   0        0        0    16498 2024-05-16 01:09:37.920933 new_natnet_client-4.3.1/new_natnet_client/Client.py
--rw-r--r--   0        0        0     9381 2024-05-16 01:10:23.380136 new_natnet_client-4.3.1/new_natnet_client/NatNetTypes.py
--rw-r--r--   0        0        0    25548 2024-05-15 21:51:59.794498 new_natnet_client-4.3.1/new_natnet_client/Unpackers.py
--rw-r--r--   0        0        0        0 2024-05-11 18:54:03.498484 new_natnet_client-4.3.1/new_natnet_client/__init__.py
--rw-r--r--   0        0        0      464 2024-05-16 01:13:08.505084 new_natnet_client-4.3.1/pyproject.toml
--rw-r--r--   0        0        0     2026 1970-01-01 00:00:00.000000 new_natnet_client-4.3.1/PKG-INFO
+-rw-r--r--   0        0        0      958 2024-05-11 18:54:03.498484 new_natnet_client-4.3.2/LICENSE
+-rw-r--r--   0        0        0     1758 2024-05-16 01:55:55.789326 new_natnet_client-4.3.2/README.md
+-rw-r--r--   0        0        0    16555 2024-05-17 16:08:17.438026 new_natnet_client-4.3.2/new_natnet_client/Client.py
+-rw-r--r--   0        0        0     9381 2024-05-16 01:10:23.380136 new_natnet_client-4.3.2/new_natnet_client/NatNetTypes.py
+-rw-r--r--   0        0        0    25548 2024-05-16 02:29:37.345534 new_natnet_client-4.3.2/new_natnet_client/Unpackers.py
+-rw-r--r--   0        0        0        0 2024-05-11 18:54:03.498484 new_natnet_client-4.3.2/new_natnet_client/__init__.py
+-rw-r--r--   0        0        0      464 2024-05-17 16:09:07.777132 new_natnet_client-4.3.2/pyproject.toml
+-rw-r--r--   0        0        0     2295 1970-01-01 00:00:00.000000 new_natnet_client-4.3.2/PKG-INFO
```

### Comparing `new_natnet_client-4.3.1/LICENSE` & `new_natnet_client-4.3.2/LICENSE`

 * *Files identical despite different names*

### Comparing `new_natnet_client-4.3.1/README.md` & `new_natnet_client-4.3.2/README.md`

 * *Files 24% similar despite different names*

```diff
@@ -1,7 +1,12 @@
+[![Poetry](https://img.shields.io/endpoint?url=https://python-poetry.org/badge/v0.json)](https://python-poetry.org/)
+![PyPI - Python Version](https://img.shields.io/pypi/pyversions/new-natnet-client)
+![PyPI - License](https://img.shields.io/pypi/l/new-natnet-client)
+
+
 This package provides the client for using [Optitrack's](https://optitrack.com/) NatNet tracking system, with type hints for python.
 
 The NatNet SDK is a simple Client/Server networking SDK for sending and receiving
 data from Motive across networks.  NatNet uses the UDP protocol in conjunction
 with either multicasting or point-to-point unicasting for transmitting data.
 
 A list of changes made in each version can be found at the following website: https://www.optitrack.com/support/downloads/developer-tools.html
```

### Comparing `new_natnet_client-4.3.1/new_natnet_client/Client.py` & `new_natnet_client-4.3.2/new_natnet_client/Client.py`

 * *Files 1% similar despite different names*

```diff
@@ -118,15 +118,15 @@
     if type(self.__command_socket) == NoneType:
       logging.info(f"Command socket. Check Motive/Server mode requested mode agreement.  {self.use_multicast = } ")
       return False
     if self.use_multicast:
       # set to broadcast mode
       self.__command_socket.setsockopt(socket.SOL_SOCKET, socket.SO_BROADCAST, 1)
     return True
-    
+
   def __create__data_socket(self) -> bool:
     ip = ''
     proto = socket.IPPROTO_UDP
     port = 0
     if self.use_multicast:
       ip = self.local_ip_address
       proto = 0
@@ -176,25 +176,29 @@
       "multicast_address",
       "command_port",
       "data_port",
     ):
       raise FrozenInstanceError("This attribute can't be changed because client is already connected")
     super().__setattr__(name, value)
 
-  def __enter__(self) -> None:
+  def connect(self) -> None:
     if self.__running or not self.__create__command_socket() or not self.__create__data_socket(): return
     logging.info("Client connected")
     self.__running = True
     self.__data_thread = Thread(target=self.__data_thread_function)
     self.__data_thread.start()
     self.__command_thread = Thread(target=self.__command_thread_function)
     self.__command_thread.start()
     time.sleep(1) # wait to get threads running for receiving data
     self.send_request(NAT_Messages.CONNECT,"")
 
+  def __enter__(self):
+    self.connect()
+    return self
+
   def __exit__(self, exc_type: Optional[Type[BaseException]], exc_value: Optional[BaseException], traceback: Optional[TracebackType]) -> None:
     if self.__running:
       self.shutdown()
 
   def send_request(self, NAT_command: NAT_Messages, command: str) -> int:
     """
       Send request to server
```

### Comparing `new_natnet_client-4.3.1/new_natnet_client/NatNetTypes.py` & `new_natnet_client-4.3.2/new_natnet_client/NatNetTypes.py`

 * *Files identical despite different names*

### Comparing `new_natnet_client-4.3.1/new_natnet_client/Unpackers.py` & `new_natnet_client-4.3.2/new_natnet_client/Unpackers.py`

 * *Files identical despite different names*

### Comparing `new_natnet_client-4.3.1/PKG-INFO` & `new_natnet_client-4.3.2/PKG-INFO`

 * *Files 7% similar despite different names*

```diff
@@ -1,22 +1,27 @@
 Metadata-Version: 2.1
 Name: new-natnet-client
-Version: 4.3.1
+Version: 4.3.2
 Summary: natnet client for motive application for python
 Home-page: https://optitrack.com/
 License: GLWTPL
 Author: Ignacio de la Torre Arias
 Author-email: ignaciodlta@gmail.com
 Requires-Python: >=3.12,<4.0
 Classifier: License :: Other/Proprietary License
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.12
 Project-URL: Repository, https://github.com/IgnaciodelaTorreArias/natnet-client
 Description-Content-Type: text/markdown
 
+[![Poetry](https://img.shields.io/endpoint?url=https://python-poetry.org/badge/v0.json)](https://python-poetry.org/)
+![PyPI - Python Version](https://img.shields.io/pypi/pyversions/new-natnet-client)
+![PyPI - License](https://img.shields.io/pypi/l/new-natnet-client)
+
+
 This package provides the client for using [Optitrack's](https://optitrack.com/) NatNet tracking system, with type hints for python.
 
 The NatNet SDK is a simple Client/Server networking SDK for sending and receiving
 data from Motive across networks.  NatNet uses the UDP protocol in conjunction
 with either multicasting or point-to-point unicasting for transmitting data.
 
 A list of changes made in each version can be found at the following website: https://www.optitrack.com/support/downloads/developer-tools.html
```

