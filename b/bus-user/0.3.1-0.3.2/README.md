# Comparing `tmp/bus_user-0.3.1.tar.gz` & `tmp/bus_user-0.3.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "bus_user-0.3.1.tar", last modified: Wed May 29 08:58:20 2024, max compression
+gzip compressed data, was "bus_user-0.3.2.tar", last modified: Wed May 29 09:16:46 2024, max compression
```

## Comparing `bus_user-0.3.1.tar` & `bus_user-0.3.2.tar`

### file list

```diff
@@ -1,20 +1,20 @@
-drwxrwxrwx   0        0        0        0 2024-05-29 08:58:20.914990 bus_user-0.3.1/
--rw-rw-rw-   0        0        0     1082 2023-12-11 08:31:15.000000 bus_user-0.3.1/LICENSE
--rw-rw-rw-   0        0        0     4169 2024-05-29 08:58:20.914990 bus_user-0.3.1/PKG-INFO
--rw-rw-rw-   0        0        0     3204 2024-05-29 08:58:04.000000 bus_user-0.3.1/README.md
-drwxrwxrwx   0        0        0        0 2024-05-29 08:58:20.909201 bus_user-0.3.1/bus_user/
--rw-rw-rw-   0        0        0     2286 2024-05-24 09:30:08.000000 bus_user-0.3.1/bus_user/__init__.py
--rw-rw-rw-   0        0        0     3366 2023-12-14 12:44:59.000000 bus_user-0.3.1/bus_user/history.py
--rw-rw-rw-   0        0        0     3761 2024-05-24 09:30:08.000000 bus_user-0.3.1/bus_user/i2c_client.py
--rw-rw-rw-   0        0        0     2158 2024-05-24 09:19:18.000000 bus_user-0.3.1/bus_user/line_parser.py
--rw-rw-rw-   0        0        0    39890 2024-05-29 07:06:52.000000 bus_user-0.3.1/bus_user/serial_client.py
--rw-rw-rw-   0        0        0      711 2024-05-24 15:12:34.000000 bus_user-0.3.1/bus_user/serial_derivatives.py
--rw-rw-rw-   0        0        0    19438 2024-05-29 08:54:12.000000 bus_user-0.3.1/bus_user/serial_server.py
--rw-rw-rw-   0        0        0     6032 2024-05-24 09:11:17.000000 bus_user-0.3.1/bus_user/values.py
-drwxrwxrwx   0        0        0        0 2024-05-29 08:58:20.913992 bus_user-0.3.1/bus_user.egg-info/
--rw-rw-rw-   0        0        0     4169 2024-05-29 08:58:20.000000 bus_user-0.3.1/bus_user.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      354 2024-05-29 08:58:20.000000 bus_user-0.3.1/bus_user.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-05-29 08:58:20.000000 bus_user-0.3.1/bus_user.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0        9 2024-05-29 08:58:20.000000 bus_user-0.3.1/bus_user.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2024-05-29 08:58:20.915990 bus_user-0.3.1/setup.cfg
--rw-rw-rw-   0        0        0     2184 2024-01-30 14:09:01.000000 bus_user-0.3.1/setup.py
+drwxrwxrwx   0        0        0        0 2024-05-29 09:16:46.657928 bus_user-0.3.2/
+-rw-rw-rw-   0        0        0     1082 2023-12-11 08:31:15.000000 bus_user-0.3.2/LICENSE
+-rw-rw-rw-   0        0        0     4169 2024-05-29 09:16:46.657427 bus_user-0.3.2/PKG-INFO
+-rw-rw-rw-   0        0        0     3204 2024-05-29 09:16:20.000000 bus_user-0.3.2/README.md
+drwxrwxrwx   0        0        0        0 2024-05-29 09:16:46.648411 bus_user-0.3.2/bus_user/
+-rw-rw-rw-   0        0        0     2286 2024-05-24 09:30:08.000000 bus_user-0.3.2/bus_user/__init__.py
+-rw-rw-rw-   0        0        0     3366 2023-12-14 12:44:59.000000 bus_user-0.3.2/bus_user/history.py
+-rw-rw-rw-   0        0        0     3761 2024-05-24 09:30:08.000000 bus_user-0.3.2/bus_user/i2c_client.py
+-rw-rw-rw-   0        0        0     2158 2024-05-24 09:19:18.000000 bus_user-0.3.2/bus_user/line_parser.py
+-rw-rw-rw-   0        0        0    40053 2024-05-29 09:14:00.000000 bus_user-0.3.2/bus_user/serial_client.py
+-rw-rw-rw-   0        0        0      711 2024-05-24 15:12:34.000000 bus_user-0.3.2/bus_user/serial_derivatives.py
+-rw-rw-rw-   0        0        0    19438 2024-05-29 08:54:12.000000 bus_user-0.3.2/bus_user/serial_server.py
+-rw-rw-rw-   0        0        0     6032 2024-05-24 09:11:17.000000 bus_user-0.3.2/bus_user/values.py
+drwxrwxrwx   0        0        0        0 2024-05-29 09:16:46.655870 bus_user-0.3.2/bus_user.egg-info/
+-rw-rw-rw-   0        0        0     4169 2024-05-29 09:16:46.000000 bus_user-0.3.2/bus_user.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      354 2024-05-29 09:16:46.000000 bus_user-0.3.2/bus_user.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-05-29 09:16:46.000000 bus_user-0.3.2/bus_user.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0        9 2024-05-29 09:16:46.000000 bus_user-0.3.2/bus_user.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2024-05-29 09:16:46.659905 bus_user-0.3.2/setup.cfg
+-rw-rw-rw-   0        0        0     2184 2024-01-30 14:09:01.000000 bus_user-0.3.2/setup.py
```

### Comparing `bus_user-0.3.1/LICENSE` & `bus_user-0.3.2/LICENSE`

 * *Files identical despite different names*

### Comparing `bus_user-0.3.1/PKG-INFO` & `bus_user-0.3.2/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: bus_user
-Version: 0.3.1
+Version: 0.3.2
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
 
-# bus_user (v0.3.1)
+# bus_user (v0.3.2)
 
 ## DESCRIPTION_SHORT
 work with equipment over buses like Serial/i2c/... as client and server
 
 ## DESCRIPTION_LONG
 ###
 NOTE: IT SEEMS THIS IS OLD DATA! see tests for actual usage!
```

### Comparing `bus_user-0.3.1/README.md` & `bus_user-0.3.2/README.md`

 * *Files 1% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# bus_user (v0.3.1)
+# bus_user (v0.3.2)
 
 ## DESCRIPTION_SHORT
 work with equipment over buses like Serial/i2c/... as client and server
 
 ## DESCRIPTION_LONG
 ###
 NOTE: IT SEEMS THIS IS OLD DATA! see tests for actual usage!
```

### Comparing `bus_user-0.3.1/bus_user/__init__.py` & `bus_user-0.3.2/bus_user/__init__.py`

 * *Files identical despite different names*

### Comparing `bus_user-0.3.1/bus_user/history.py` & `bus_user-0.3.2/bus_user/history.py`

 * *Files identical despite different names*

### Comparing `bus_user-0.3.1/bus_user/i2c_client.py` & `bus_user-0.3.2/bus_user/i2c_client.py`

 * *Files identical despite different names*

### Comparing `bus_user-0.3.1/bus_user/line_parser.py` & `bus_user-0.3.2/bus_user/line_parser.py`

 * *Files identical despite different names*

### Comparing `bus_user-0.3.1/bus_user/serial_client.py` & `bus_user-0.3.2/bus_user/serial_client.py`

 * *Files 1% similar despite different names*

```diff
@@ -243,55 +243,57 @@
             self,
             address: Optional[str] = None,
             _raise: Optional[bool] = None,
             _touch_connection: bool | None = None    # no final connection! specially keep ability to connect without Emu on cls main perpose (search ports)!
     ) -> Union[bool, NoReturn]:
         msg = None
         exx = None
+        need_open = True
 
         # SETTINGS ---------------------------------
         if _raise is None:
             _raise = self.RAISE_CONNECT
 
         if address is None:
             address = self.ADDRESS
 
         # AUTOAPPLY ---------------------------------
-        if address is None:
-            msg = "Exx_SerialAddress_NotConfigured"
-            exx = Exx_SerialAddress_NotConfigured()
-
-        elif address == Type__AddressAutoAcceptVariant.FIRST_FREE:
+        if address == Type__AddressAutoAcceptVariant.FIRST_FREE:
             address = self.address_get__first_free()
         elif address == Type__AddressAutoAcceptVariant.FIRST_FREE__SHORTED:
             address = self.address_get__first_free__shorted()
         elif address == Type__AddressAutoAcceptVariant.FIRST_FREE__ANSWER_VALID:
             address = self.address_get__first_free__answer_valid()
         elif address == Type__AddressAutoAcceptVariant.FIRST_FREE__PAIRED:
             address = self.address_get__first_free__paired()
 
+        if address is None or isinstance(address, Type__AddressAutoAcceptVariant):
+            msg = "Exx_SerialAddress_NotConfigured"
+            exx = Exx_SerialAddress_NotConfigured()
+            need_open = False
+
         # need_open ==========================================================
         # CHANGE PORT OR USE SAME ---------------------------------
-        need_open = True
-        if self._SERIAL.port != address:
-            # close old
-            if self._SERIAL.is_open:
-                self._SERIAL.close()
-
-            # set new
-            self._SERIAL.port = address
-            if self._SERIAL.is_open:
-                self._SERIAL.port = None
-                msg = f"[ERROR] Attempt to connect to already opened port IN OTHER OBJECT {self._SERIAL}"
-                exx = Exx_SerialAddress_AlreadyOpened_InOtherObject(msg)
-
-                need_open = False
-        else:
-            if self._SERIAL.is_open:
-                need_open = False
+        if need_open:
+            if self._SERIAL.port != address:
+                # close old
+                if self._SERIAL.is_open:
+                    self._SERIAL.close()
+
+                # set new
+                self._SERIAL.port = address
+                if self._SERIAL.is_open:
+                    self._SERIAL.port = None
+                    msg = f"[ERROR] Attempt to connect to already opened port IN OTHER OBJECT {self._SERIAL}"
+                    exx = Exx_SerialAddress_AlreadyOpened_InOtherObject(msg)
+
+                    need_open = False
+            else:
+                if self._SERIAL.is_open:
+                    need_open = False
 
         # Try OPEN ===================================================================
         if need_open:
             try:
                 self._SERIAL.open()
             except Exception as _exx:
                 if not _touch_connection:
```

### Comparing `bus_user-0.3.1/bus_user/serial_derivatives.py` & `bus_user-0.3.2/bus_user/serial_derivatives.py`

 * *Files identical despite different names*

### Comparing `bus_user-0.3.1/bus_user/serial_server.py` & `bus_user-0.3.2/bus_user/serial_server.py`

 * *Files identical despite different names*

### Comparing `bus_user-0.3.1/bus_user/values.py` & `bus_user-0.3.2/bus_user/values.py`

 * *Files identical despite different names*

### Comparing `bus_user-0.3.1/bus_user.egg-info/PKG-INFO` & `bus_user-0.3.2/bus_user.egg-info/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: bus_user
-Version: 0.3.1
+Version: 0.3.2
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
 
-# bus_user (v0.3.1)
+# bus_user (v0.3.2)
 
 ## DESCRIPTION_SHORT
 work with equipment over buses like Serial/i2c/... as client and server
 
 ## DESCRIPTION_LONG
 ###
 NOTE: IT SEEMS THIS IS OLD DATA! see tests for actual usage!
```

### Comparing `bus_user-0.3.1/setup.py` & `bus_user-0.3.2/setup.py`

 * *Files identical despite different names*

