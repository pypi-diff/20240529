# Comparing `tmp/bus_user-0.3.2.tar.gz` & `tmp/bus_user-0.3.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "bus_user-0.3.2.tar", last modified: Wed May 29 09:16:46 2024, max compression
+gzip compressed data, was "bus_user-0.3.3.tar", last modified: Wed May 29 11:59:37 2024, max compression
```

## Comparing `bus_user-0.3.2.tar` & `bus_user-0.3.3.tar`

### file list

```diff
@@ -1,20 +1,20 @@
-drwxrwxrwx   0        0        0        0 2024-05-29 09:16:46.657928 bus_user-0.3.2/
--rw-rw-rw-   0        0        0     1082 2023-12-11 08:31:15.000000 bus_user-0.3.2/LICENSE
--rw-rw-rw-   0        0        0     4169 2024-05-29 09:16:46.657427 bus_user-0.3.2/PKG-INFO
--rw-rw-rw-   0        0        0     3204 2024-05-29 09:16:20.000000 bus_user-0.3.2/README.md
-drwxrwxrwx   0        0        0        0 2024-05-29 09:16:46.648411 bus_user-0.3.2/bus_user/
--rw-rw-rw-   0        0        0     2286 2024-05-24 09:30:08.000000 bus_user-0.3.2/bus_user/__init__.py
--rw-rw-rw-   0        0        0     3366 2023-12-14 12:44:59.000000 bus_user-0.3.2/bus_user/history.py
--rw-rw-rw-   0        0        0     3761 2024-05-24 09:30:08.000000 bus_user-0.3.2/bus_user/i2c_client.py
--rw-rw-rw-   0        0        0     2158 2024-05-24 09:19:18.000000 bus_user-0.3.2/bus_user/line_parser.py
--rw-rw-rw-   0        0        0    40053 2024-05-29 09:14:00.000000 bus_user-0.3.2/bus_user/serial_client.py
--rw-rw-rw-   0        0        0      711 2024-05-24 15:12:34.000000 bus_user-0.3.2/bus_user/serial_derivatives.py
--rw-rw-rw-   0        0        0    19438 2024-05-29 08:54:12.000000 bus_user-0.3.2/bus_user/serial_server.py
--rw-rw-rw-   0        0        0     6032 2024-05-24 09:11:17.000000 bus_user-0.3.2/bus_user/values.py
-drwxrwxrwx   0        0        0        0 2024-05-29 09:16:46.655870 bus_user-0.3.2/bus_user.egg-info/
--rw-rw-rw-   0        0        0     4169 2024-05-29 09:16:46.000000 bus_user-0.3.2/bus_user.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      354 2024-05-29 09:16:46.000000 bus_user-0.3.2/bus_user.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-05-29 09:16:46.000000 bus_user-0.3.2/bus_user.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0        9 2024-05-29 09:16:46.000000 bus_user-0.3.2/bus_user.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2024-05-29 09:16:46.659905 bus_user-0.3.2/setup.cfg
--rw-rw-rw-   0        0        0     2184 2024-01-30 14:09:01.000000 bus_user-0.3.2/setup.py
+drwxrwxrwx   0        0        0        0 2024-05-29 11:59:37.319361 bus_user-0.3.3/
+-rw-rw-rw-   0        0        0     1082 2023-12-11 08:31:15.000000 bus_user-0.3.3/LICENSE
+-rw-rw-rw-   0        0        0     4169 2024-05-29 11:59:37.318342 bus_user-0.3.3/PKG-INFO
+-rw-rw-rw-   0        0        0     3204 2024-05-29 11:53:12.000000 bus_user-0.3.3/README.md
+drwxrwxrwx   0        0        0        0 2024-05-29 11:59:37.312139 bus_user-0.3.3/bus_user/
+-rw-rw-rw-   0        0        0     2286 2024-05-24 09:30:08.000000 bus_user-0.3.3/bus_user/__init__.py
+-rw-rw-rw-   0        0        0     3366 2023-12-14 12:44:59.000000 bus_user-0.3.3/bus_user/history.py
+-rw-rw-rw-   0        0        0     3761 2024-05-24 09:30:08.000000 bus_user-0.3.3/bus_user/i2c_client.py
+-rw-rw-rw-   0        0        0     2158 2024-05-24 09:19:18.000000 bus_user-0.3.3/bus_user/line_parser.py
+-rw-rw-rw-   0        0        0    40705 2024-05-29 11:46:31.000000 bus_user-0.3.3/bus_user/serial_client.py
+-rw-rw-rw-   0        0        0      711 2024-05-24 15:12:34.000000 bus_user-0.3.3/bus_user/serial_derivatives.py
+-rw-rw-rw-   0        0        0    19410 2024-05-29 11:45:30.000000 bus_user-0.3.3/bus_user/serial_server.py
+-rw-rw-rw-   0        0        0     6032 2024-05-24 09:11:17.000000 bus_user-0.3.3/bus_user/values.py
+drwxrwxrwx   0        0        0        0 2024-05-29 11:59:37.318342 bus_user-0.3.3/bus_user.egg-info/
+-rw-rw-rw-   0        0        0     4169 2024-05-29 11:59:37.000000 bus_user-0.3.3/bus_user.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      354 2024-05-29 11:59:37.000000 bus_user-0.3.3/bus_user.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-05-29 11:59:37.000000 bus_user-0.3.3/bus_user.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0        9 2024-05-29 11:59:37.000000 bus_user-0.3.3/bus_user.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2024-05-29 11:59:37.319361 bus_user-0.3.3/setup.cfg
+-rw-rw-rw-   0        0        0     2184 2024-01-30 14:09:01.000000 bus_user-0.3.3/setup.py
```

### Comparing `bus_user-0.3.2/LICENSE` & `bus_user-0.3.3/LICENSE`

 * *Files identical despite different names*

### Comparing `bus_user-0.3.2/PKG-INFO` & `bus_user-0.3.3/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: bus_user
-Version: 0.3.2
+Version: 0.3.3
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
 
-# bus_user (v0.3.2)
+# bus_user (v0.3.3)
 
 ## DESCRIPTION_SHORT
 work with equipment over buses like Serial/i2c/... as client and server
 
 ## DESCRIPTION_LONG
 ###
 NOTE: IT SEEMS THIS IS OLD DATA! see tests for actual usage!
```

### Comparing `bus_user-0.3.2/README.md` & `bus_user-0.3.3/README.md`

 * *Files 0% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# bus_user (v0.3.2)
+# bus_user (v0.3.3)
 
 ## DESCRIPTION_SHORT
 work with equipment over buses like Serial/i2c/... as client and server
 
 ## DESCRIPTION_LONG
 ###
 NOTE: IT SEEMS THIS IS OLD DATA! see tests for actual usage!
```

### Comparing `bus_user-0.3.2/bus_user/__init__.py` & `bus_user-0.3.3/bus_user/__init__.py`

 * *Files identical despite different names*

### Comparing `bus_user-0.3.2/bus_user/history.py` & `bus_user-0.3.3/bus_user/history.py`

 * *Files identical despite different names*

### Comparing `bus_user-0.3.2/bus_user/i2c_client.py` & `bus_user-0.3.3/bus_user/i2c_client.py`

 * *Files identical despite different names*

### Comparing `bus_user-0.3.2/bus_user/line_parser.py` & `bus_user-0.3.3/bus_user/line_parser.py`

 * *Files identical despite different names*

### Comparing `bus_user-0.3.2/bus_user/serial_client.py` & `bus_user-0.3.3/bus_user/serial_client.py`

 * *Files 2% similar despite different names*

```diff
@@ -325,21 +325,21 @@
 
             if _raise:
                 raise exx
             else:
                 return False
 
         # OK -----------------------------
-        self.ADDRESS = self._SERIAL.port
-
         if not _touch_connection:
             if not self.connect__validation():
                 self.disconnect()
                 return False
+
             self.LOGGER.info(f"[{self._SERIAL.port}][OK] connected {self._SERIAL}")
+            self.ADDRESS = self._SERIAL.port
             self.emulator_start()
 
         self.cmd_prefix__set()
         return True
 
     def connect__validation(self) -> bool:
         """
@@ -487,26 +487,30 @@
         IDEA:
         1. this func will exec on every accessible address
         2. if this func return True - address would be accepted!
         3. raiseExx/NoReturn - equivalent as False!
         """
 
     def address__answer_validation__shorted(self) -> bool | None:
-        load = "EXPECT_ANSWER__SHORTED"
-        return self.write_read_line_last(load) == load
+        load = "FIND__SHORTED"
+        return self.write_read__last_validate(load, load)
 
     # DETECT PORTS ====================================================================================================
     pass
     pass
     pass
     pass
     pass
     pass
     pass
 
+    def address_check__resolved(self) -> bool:
+        return isinstance(self.ADDRESS, str)
+
+    # -----------------------------------------------------------------------------------------------------------------
     def address__check_exists(self) -> bool:
         try:
             self.connect(_raise=True, _touch_connection=True)
             self.disconnect()
         except Exx_SerialAddress_NotExists:
             return False
         except:
@@ -666,15 +670,15 @@
         for address in addresses__system:
             instance = cls(address)
             if instance.connect(_raise=False, _touch_connection=True):
                 instances_free.append(instance)
 
         while len(instances_free) > 1:
             main = instances_free.pop(0)
-            main._write_line(load)
+            main._write(load)
             main.disconnect()
 
             for index, slave in enumerate(instances_free):
                 if slave.read_line(_timeout=0.3) == load:
                     result.append((main.ADDRESS, slave.ADDRESS))
                     slave.disconnect()
                     instances_free.pop(index)
@@ -900,15 +904,15 @@
         data = self._bytes_eol__clear(data)
         data = self._data_ensure__string(data)
         self.history.add_output(data)
         self.answer_is_fail(data)
         return data
 
     # W ---------------------------------------------------------------------------------------------------------------
-    def _write_line(
+    def _write(
             self,
             data: Union[AnyStr, List[AnyStr]],
             prefix: Optional[str] = None,
             args: Optional[List] = None,
             kwargs: Optional[Dict] = None
     ) -> bool:
         """
@@ -924,15 +928,15 @@
 
         data = data or ""
 
         # LIST -----------------------
         if isinstance(data, (list, tuple, )):
             if len(data) > 1:
                 for data_i in data:
-                    if not self._write_line(data=data_i, prefix=prefix, args=args, kwargs=kwargs):
+                    if not self._write(data=data_i, prefix=prefix, args=args, kwargs=kwargs):
                         return False
                 return True
             else:
                 data = data[0]
 
         # SINGLE ---------------------
         data = self._create_cmd_line(cmd=data, prefix=prefix, args=args, kwargs=kwargs)
@@ -948,61 +952,78 @@
         if data_length > 0:
             return True
         else:
             msg = f"[ERROR] data not write"
             self.LOGGER.error(f"[{self._SERIAL.port}]{msg}")
             return False
 
-    def write_read_line(
+    def write_read(
             self,
             data: Union[AnyStr, List[AnyStr]],
             prefix: Optional[str] = None,
             args: Optional[List] = None,
             kwargs: Optional[Dict] = None,
     ) -> Union[HistoryIO, NoReturn]:
         """
         send data and return history
         """
         history = HistoryIO()
 
         # LIST -------------------------
         if isinstance(data, (list, tuple,)):
             for data_i in data:
-                history_i = self.write_read_line(data_i, prefix=prefix, args=args, kwargs=kwargs)
+                history_i = self.write_read(data_i, prefix=prefix, args=args, kwargs=kwargs)
                 history.add_history(history_i)
         else:
             # SINGLE LAST -----------------------
             data_o = ""
-            if self._write_line(data=data, prefix=prefix, args=args, kwargs=kwargs):
+            if self._write(data=data, prefix=prefix, args=args, kwargs=kwargs):
                 data_o = self.read_lines()
             history.add_io(self._data_ensure__string(data), data_o)
 
         # RESULT ----------------------------
         return history
 
-    def write_read_line_last(
+    def write_read__last(
             self,
             data: Union[AnyStr, List[AnyStr]],
             prefix: Optional[str] = None,
             args: Optional[List] = None,
             kwargs: Optional[Dict] = None,
     ) -> Union[str, NoReturn]:
         """
         it is created specially for single cmd usage! but decided leave multy cmd usage as feature.
         return always last_output
         """
-        return self.write_read_line(data=data, prefix=prefix, args=args, kwargs=kwargs).last_output
+        return self.write_read(data=data, prefix=prefix, args=args, kwargs=kwargs).last_output
+
+    def write_read__last_validate(
+            self,
+            input: Union[AnyStr, list[AnyStr]] | None,
+            expect: Union[str, list[str]],
+            prefix: Optional[str] = None,
+            args: Optional[List] = None,
+            kwargs: Optional[Dict] = None,
+    ) -> bool:
+        if input:
+            return self.write_read__last(data=input, prefix=prefix, args=args, kwargs=kwargs) == expect
+        else:
+            outputs = self.read_lines()
+            output_last = None
+            if outputs:
+                output_last = outputs[-1]
+            return output_last == expect
 
     def dump_cmds(self, cmds: List[str] = None) -> Union[HistoryIO, NoReturn]:
         """
         useful to get results for standard cmds list
         if you need to read all params from device!
         """
         cmds = cmds or self.CMDS_DUMP
-        history = self.write_read_line(cmds)
+        history = self.write_read(cmds)
         history.print_io()
         return history
 
     # =================================================================================================================
     def __getattr__(self, item: str) -> Callable[..., Union[str, NoReturn]]:
         """if no exists attr/meth
 
@@ -1027,20 +1048,16 @@
             dev.VIN("12 13")  # return answer for sent string in port "VIN 12 13"
             dev.VIN(12, 13)   # return answer for sent string in port "VIN 12 13" by args
             dev.VIN(CH1=12, CH2=13) # return answer for sent string in port "VIN CH1=12 CH2=13" by kwargs
             dev.VIN(12, CH2=13)     # return answer for sent string in port "VIN 12 CH2=13" by args/kwargs
         """
         if self._GETATTR_STARTSWITH__SEND and item.startswith(self._GETATTR_STARTSWITH__SEND):
             item = item.replace(self._GETATTR_STARTSWITH__SEND, "")
-        return lambda *args, **kwargs: self.write_read_line_last(data=self._create_cmd_line(cmd=item, args=args, kwargs=kwargs))
+        return lambda *args, **kwargs: self.write_read__last(data=self._create_cmd_line(cmd=item, args=args, kwargs=kwargs))
 
 
 # =====================================================================================================================
 if __name__ == "__main__":
-    # see/use tests
-    # ports = SerialClient.detect_available_ports()
-    # obj = SerialClient(address=ports[0])
-    # obj.connect()
     pass
 
 
 # =====================================================================================================================
```

### Comparing `bus_user-0.3.2/bus_user/serial_derivatives.py` & `bus_user-0.3.3/bus_user/serial_derivatives.py`

 * *Files identical despite different names*

### Comparing `bus_user-0.3.2/bus_user/serial_server.py` & `bus_user-0.3.3/bus_user/serial_server.py`

 * *Files 2% similar despite different names*

```diff
@@ -187,31 +187,31 @@
             print(msg)
             return
 
         if self.HELLO_MSG__SEND_ON_START:
             additional_line = f"Started on [{self.SERIAL_CLIENT._SERIAL.port}]"
             if additional_line not in self.HELLO_MSG:
                 self.HELLO_MSG.append(additional_line)
-            self.SERIAL_CLIENT._write_line("")
-            self.SERIAL_CLIENT._write_line("="*50)
+            self.SERIAL_CLIENT._write("")
+            self.SERIAL_CLIENT._write("=" * 50)
             # self._execute_line("hello")
-            self.SERIAL_CLIENT._write_line(self.HELLO_MSG)
+            self.SERIAL_CLIENT._write(self.HELLO_MSG)
 
         self._cycle__activate()
 
     def _cycle__activate(self) -> Never:
         self.logger.debug("")
 
         while True:
             self.CYCLE_ACTIVE = True
             line = None
             try:
                 line = self.SERIAL_CLIENT.read_line()
             except:
-                self.SERIAL_CLIENT._write_line(self.ANSWER.ERR__ENCODING_OR_DEVICE)
+                self.SERIAL_CLIENT._write(self.ANSWER.ERR__ENCODING_OR_DEVICE)
 
             if line:
                 self._execute_line(line)
 
     def connect(self) -> None:
         self.logger.debug("")
         self.start()
@@ -246,15 +246,15 @@
         line_parsed = LineParsed(line, _prefix_expected=self.SERIAL_CLIENT.PREFIX)
         cmd_result = self._cmd__(line_parsed)
 
         # blank line - SEND!!! because value may be BLANK!!!!
         # if not cmd_result:
         #     return True
 
-        write_result = self.SERIAL_CLIENT._write_line(cmd_result)
+        write_result = self.SERIAL_CLIENT._write(cmd_result)
         return write_result
 
     # CMD - ENTRY POINT -----------------------------------------------------------------------------------------------
     def _cmd__(self, line_parsed: LineParsed) -> TYPE__CMD_RESULT:
         self.logger.debug("")
 
         meth_name__expected = f"{self._STARTSWITH__CMD}{line_parsed.CMD}"
@@ -451,15 +451,15 @@
 # =====================================================================================================================
 class SerialServer_Echo(SerialServer_Base):
     HELLO_MSG: List[str] = [
         "SerialServer_Echo",
     ]
 
     def _execute_line(self, line: str) -> bool:
-        write_result = self.SERIAL_CLIENT._write_line(line)
+        write_result = self.SERIAL_CLIENT._write(line)
         return write_result
 
 
 # =====================================================================================================================
 class SerialServer_Example(SerialServer_Base):
     PARAMS = {
         "VAR": "",
```

### Comparing `bus_user-0.3.2/bus_user/values.py` & `bus_user-0.3.3/bus_user/values.py`

 * *Files identical despite different names*

### Comparing `bus_user-0.3.2/bus_user.egg-info/PKG-INFO` & `bus_user-0.3.3/bus_user.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: bus_user
-Version: 0.3.2
+Version: 0.3.3
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
 
-# bus_user (v0.3.2)
+# bus_user (v0.3.3)
 
 ## DESCRIPTION_SHORT
 work with equipment over buses like Serial/i2c/... as client and server
 
 ## DESCRIPTION_LONG
 ###
 NOTE: IT SEEMS THIS IS OLD DATA! see tests for actual usage!
```

### Comparing `bus_user-0.3.2/setup.py` & `bus_user-0.3.3/setup.py`

 * *Files identical despite different names*

