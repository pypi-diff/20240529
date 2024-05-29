# Comparing `tmp/bus_user-0.3.0.tar.gz` & `tmp/bus_user-0.3.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "bus_user-0.3.0.tar", last modified: Mon May 27 14:42:29 2024, max compression
+gzip compressed data, was "bus_user-0.3.1.tar", last modified: Wed May 29 08:58:20 2024, max compression
```

## Comparing `bus_user-0.3.0.tar` & `bus_user-0.3.1.tar`

### file list

```diff
@@ -1,20 +1,20 @@
-drwxrwxrwx   0        0        0        0 2024-05-27 14:42:29.898213 bus_user-0.3.0/
--rw-rw-rw-   0        0        0     1082 2023-12-11 08:31:15.000000 bus_user-0.3.0/LICENSE
--rw-rw-rw-   0        0        0     4169 2024-05-27 14:42:29.897215 bus_user-0.3.0/PKG-INFO
--rw-rw-rw-   0        0        0     3204 2024-05-27 14:27:59.000000 bus_user-0.3.0/README.md
-drwxrwxrwx   0        0        0        0 2024-05-27 14:42:29.885728 bus_user-0.3.0/bus_user/
--rw-rw-rw-   0        0        0     2286 2024-05-24 09:30:08.000000 bus_user-0.3.0/bus_user/__init__.py
--rw-rw-rw-   0        0        0     3366 2023-12-14 12:44:59.000000 bus_user-0.3.0/bus_user/history.py
--rw-rw-rw-   0        0        0     3761 2024-05-24 09:30:08.000000 bus_user-0.3.0/bus_user/i2c_client.py
--rw-rw-rw-   0        0        0     2158 2024-05-24 09:19:18.000000 bus_user-0.3.0/bus_user/line_parser.py
--rw-rw-rw-   0        0        0    39994 2024-05-27 14:36:43.000000 bus_user-0.3.0/bus_user/serial_client.py
--rw-rw-rw-   0        0        0      711 2024-05-24 15:12:34.000000 bus_user-0.3.0/bus_user/serial_derivatives.py
--rw-rw-rw-   0        0        0    19389 2024-05-27 14:25:04.000000 bus_user-0.3.0/bus_user/serial_server.py
--rw-rw-rw-   0        0        0     6032 2024-05-24 09:11:17.000000 bus_user-0.3.0/bus_user/values.py
-drwxrwxrwx   0        0        0        0 2024-05-27 14:42:29.896219 bus_user-0.3.0/bus_user.egg-info/
--rw-rw-rw-   0        0        0     4169 2024-05-27 14:42:29.000000 bus_user-0.3.0/bus_user.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      354 2024-05-27 14:42:29.000000 bus_user-0.3.0/bus_user.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-05-27 14:42:29.000000 bus_user-0.3.0/bus_user.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0        9 2024-05-27 14:42:29.000000 bus_user-0.3.0/bus_user.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2024-05-27 14:42:29.899209 bus_user-0.3.0/setup.cfg
--rw-rw-rw-   0        0        0     2184 2024-01-30 14:09:01.000000 bus_user-0.3.0/setup.py
+drwxrwxrwx   0        0        0        0 2024-05-29 08:58:20.914990 bus_user-0.3.1/
+-rw-rw-rw-   0        0        0     1082 2023-12-11 08:31:15.000000 bus_user-0.3.1/LICENSE
+-rw-rw-rw-   0        0        0     4169 2024-05-29 08:58:20.914990 bus_user-0.3.1/PKG-INFO
+-rw-rw-rw-   0        0        0     3204 2024-05-29 08:58:04.000000 bus_user-0.3.1/README.md
+drwxrwxrwx   0        0        0        0 2024-05-29 08:58:20.909201 bus_user-0.3.1/bus_user/
+-rw-rw-rw-   0        0        0     2286 2024-05-24 09:30:08.000000 bus_user-0.3.1/bus_user/__init__.py
+-rw-rw-rw-   0        0        0     3366 2023-12-14 12:44:59.000000 bus_user-0.3.1/bus_user/history.py
+-rw-rw-rw-   0        0        0     3761 2024-05-24 09:30:08.000000 bus_user-0.3.1/bus_user/i2c_client.py
+-rw-rw-rw-   0        0        0     2158 2024-05-24 09:19:18.000000 bus_user-0.3.1/bus_user/line_parser.py
+-rw-rw-rw-   0        0        0    39890 2024-05-29 07:06:52.000000 bus_user-0.3.1/bus_user/serial_client.py
+-rw-rw-rw-   0        0        0      711 2024-05-24 15:12:34.000000 bus_user-0.3.1/bus_user/serial_derivatives.py
+-rw-rw-rw-   0        0        0    19438 2024-05-29 08:54:12.000000 bus_user-0.3.1/bus_user/serial_server.py
+-rw-rw-rw-   0        0        0     6032 2024-05-24 09:11:17.000000 bus_user-0.3.1/bus_user/values.py
+drwxrwxrwx   0        0        0        0 2024-05-29 08:58:20.913992 bus_user-0.3.1/bus_user.egg-info/
+-rw-rw-rw-   0        0        0     4169 2024-05-29 08:58:20.000000 bus_user-0.3.1/bus_user.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      354 2024-05-29 08:58:20.000000 bus_user-0.3.1/bus_user.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-05-29 08:58:20.000000 bus_user-0.3.1/bus_user.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0        9 2024-05-29 08:58:20.000000 bus_user-0.3.1/bus_user.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2024-05-29 08:58:20.915990 bus_user-0.3.1/setup.cfg
+-rw-rw-rw-   0        0        0     2184 2024-01-30 14:09:01.000000 bus_user-0.3.1/setup.py
```

### Comparing `bus_user-0.3.0/LICENSE` & `bus_user-0.3.1/LICENSE`

 * *Files identical despite different names*

### Comparing `bus_user-0.3.0/PKG-INFO` & `bus_user-0.3.1/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: bus_user
-Version: 0.3.0
+Version: 0.3.1
 Summary: work with equipment over buses like Serial/i2c/... as client and server
 Home-page: https://github.com/centroid457/
 Author: Andrei Starichenko
 Author-email: centroid@mail.ru
 Project-URL: Source, https://github.com/centroid457/bus_user
 Keywords: serial,serial bus,pyserial,serial port,com port,comport,rs232,UART,TTL,serial client,serial server,serial emulator,i2c
 Classifier: Topic :: Software Development :: Libraries :: Python Modules
@@ -16,15 +16,15 @@
 Classifier: Intended Audience :: Developers
 Classifier: Natural Language :: English
 Classifier: Typing :: Typed
 Requires-Python: >=3.6
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
-# bus_user (v0.3.0)
+# bus_user (v0.3.1)
 
 ## DESCRIPTION_SHORT
 work with equipment over buses like Serial/i2c/... as client and server
 
 ## DESCRIPTION_LONG
 ###
 NOTE: IT SEEMS THIS IS OLD DATA! see tests for actual usage!
```

### Comparing `bus_user-0.3.0/README.md` & `bus_user-0.3.1/README.md`

 * *Files 1% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# bus_user (v0.3.0)
+# bus_user (v0.3.1)
 
 ## DESCRIPTION_SHORT
 work with equipment over buses like Serial/i2c/... as client and server
 
 ## DESCRIPTION_LONG
 ###
 NOTE: IT SEEMS THIS IS OLD DATA! see tests for actual usage!
```

### Comparing `bus_user-0.3.0/bus_user/__init__.py` & `bus_user-0.3.1/bus_user/__init__.py`

 * *Files identical despite different names*

### Comparing `bus_user-0.3.0/bus_user/history.py` & `bus_user-0.3.1/bus_user/history.py`

 * *Files identical despite different names*

### Comparing `bus_user-0.3.0/bus_user/i2c_client.py` & `bus_user-0.3.1/bus_user/i2c_client.py`

 * *Files identical despite different names*

### Comparing `bus_user-0.3.0/bus_user/line_parser.py` & `bus_user-0.3.1/bus_user/line_parser.py`

 * *Files identical despite different names*

### Comparing `bus_user-0.3.0/bus_user/serial_client.py` & `bus_user-0.3.1/bus_user/serial_client.py`

 * *Files 2% similar despite different names*

```diff
@@ -438,37 +438,38 @@
         else:
             self.LOGGER.warn(msg)
 
         return result
 
     def address_get__first_free__paired(self) -> str | None:
         """
-        # FIXME: exists weakness - you need connect at once whole pair!
-            if you would use several pairs and delay connecting secondary devices - it will be incorrect pairing!
-            may be need using naming pairs! and set pair name with connecting first
-            first connects on free port, second connect by pair name??? feels good
+        connect only for first address!
+        need for occupy addresses by several servers before starting main process!!!
+        in case of any address we could occupy by two servers whole pair!
+
+        secondary address you should get by special methods for pair or by address_validating
+
         cls.pairs = {
             0: (COM1, COM2),
             1: (COM3, COM4),
         }
 
         cls.pairs = {
             "ATC": (COM1, COM2),    # change name
             1: (COM3, COM4),
         }
         """
         result = None
-        for pair in self.addresses_paired__detect():
-            for address in pair:
-                if self.connect(address=address, _raise=False, _touch_connection=True):
-                    result = address
-
-                self.disconnect()
-                if result:
-                    break
+        for address, _ in self.addresses_paired__detect():
+            if self.connect(address=address, _raise=False, _touch_connection=True):
+                result = address
+
+            self.disconnect()
+            if result:
+                break
 
         # FINISH -------------
         msg = f"[{result=}]address_get__first_free__paired"
         if result:
             self.LOGGER.info(msg)
         else:
             self.LOGGER.warn(msg)
```

### Comparing `bus_user-0.3.0/bus_user/serial_derivatives.py` & `bus_user-0.3.1/bus_user/serial_derivatives.py`

 * *Files identical despite different names*

### Comparing `bus_user-0.3.0/bus_user/serial_server.py` & `bus_user-0.3.1/bus_user/serial_server.py`

 * *Files 0% similar despite different names*

```diff
@@ -210,18 +210,20 @@
                 self.SERIAL_CLIENT._write_line(self.ANSWER.ERR__ENCODING_OR_DEVICE)
 
             if line:
                 self._execute_line(line)
 
     def connect(self) -> None:
         self.logger.debug("")
-
-        # if not self.isRunning():
         self.start()
-        self.wait__cycle_active()
+
+    def start(self, *args, **kwargs):
+        if not self.isRunning():
+            super().start()
+            self.wait__cycle_active()
 
     def disconnect(self):
         self.logger.debug("")
 
         self.terminate()
         # self.SERIAL_CLIENT.disconnect()
         # self.CYCLE_ACTIVE = False
@@ -446,15 +448,14 @@
     #     exit()
 
 
 # =====================================================================================================================
 class SerialServer_Echo(SerialServer_Base):
     HELLO_MSG: List[str] = [
         "SerialServer_Echo",
-        "started!",
     ]
 
     def _execute_line(self, line: str) -> bool:
         write_result = self.SERIAL_CLIENT._write_line(line)
         return write_result
```

### Comparing `bus_user-0.3.0/bus_user/values.py` & `bus_user-0.3.1/bus_user/values.py`

 * *Files identical despite different names*

### Comparing `bus_user-0.3.0/bus_user.egg-info/PKG-INFO` & `bus_user-0.3.1/bus_user.egg-info/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: bus_user
-Version: 0.3.0
+Version: 0.3.1
 Summary: work with equipment over buses like Serial/i2c/... as client and server
 Home-page: https://github.com/centroid457/
 Author: Andrei Starichenko
 Author-email: centroid@mail.ru
 Project-URL: Source, https://github.com/centroid457/bus_user
 Keywords: serial,serial bus,pyserial,serial port,com port,comport,rs232,UART,TTL,serial client,serial server,serial emulator,i2c
 Classifier: Topic :: Software Development :: Libraries :: Python Modules
@@ -16,15 +16,15 @@
 Classifier: Intended Audience :: Developers
 Classifier: Natural Language :: English
 Classifier: Typing :: Typed
 Requires-Python: >=3.6
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
-# bus_user (v0.3.0)
+# bus_user (v0.3.1)
 
 ## DESCRIPTION_SHORT
 work with equipment over buses like Serial/i2c/... as client and server
 
 ## DESCRIPTION_LONG
 ###
 NOTE: IT SEEMS THIS IS OLD DATA! see tests for actual usage!
```

### Comparing `bus_user-0.3.0/setup.py` & `bus_user-0.3.1/setup.py`

 * *Files identical despite different names*

