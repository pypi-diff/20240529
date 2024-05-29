# Comparing `tmp/PyNIExp-0.27.3.tar.gz` & `tmp/pyniexp-0.28.post3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "D:\Projects\pyniexp\dist\tmpbt0i_se7\PyNIExp-0.27.3.tar", last modified: Mon Apr 25 16:29:42 2022, max compression
+gzip compressed data, was "pyniexp-0.28.post3.tar", last modified: Wed May 29 10:17:35 2024, max compression
```

## Comparing `PyNIExp-0.27.3.tar` & `pyniexp-0.28.post3.tar`

### file list

```diff
@@ -1,23 +1,53 @@
-drwxrwxrwx   0        0        0        0 2022-04-25 16:29:42.574375 PyNIExp-0.27.3/
--rw-rw-rw-   0        0        0    35823 2021-03-23 15:38:50.000000 PyNIExp-0.27.3/LICENSE
--rw-rw-rw-   0        0        0      702 2022-04-25 16:29:42.573378 PyNIExp-0.27.3/PKG-INFO
-drwxrwxrwx   0        0        0        0 2022-04-25 16:29:42.521518 PyNIExp-0.27.3/PyNIExp.egg-info/
--rw-rw-rw-   0        0        0      702 2022-04-25 16:29:41.000000 PyNIExp-0.27.3/PyNIExp.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      411 2022-04-25 16:29:42.000000 PyNIExp-0.27.3/PyNIExp.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2022-04-25 16:29:42.000000 PyNIExp-0.27.3/PyNIExp.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       60 2022-04-25 16:29:42.000000 PyNIExp-0.27.3/PyNIExp.egg-info/requires.txt
--rw-rw-rw-   0        0        0        8 2022-04-25 16:29:42.000000 PyNIExp-0.27.3/PyNIExp.egg-info/top_level.txt
--rw-rw-rw-   0        0        0      377 2022-04-10 07:37:38.000000 PyNIExp-0.27.3/README.md
-drwxrwxrwx   0        0        0        0 2022-04-25 16:29:42.573378 PyNIExp-0.27.3/pyniexp/
--rw-rw-rw-   0        0        0    12550 2021-03-23 15:38:50.000000 PyNIExp-0.27.3/pyniexp/connection.py
--rw-rw-rw-   0        0        0     1641 2021-03-23 15:38:50.000000 PyNIExp-0.27.3/pyniexp/kbutils.py
--rw-rw-rw-   0        0        0     2800 2022-04-09 10:51:40.000000 PyNIExp-0.27.3/pyniexp/mlplugins.py
--rw-rw-rw-   0        0        0    15625 2021-03-23 15:38:50.000000 PyNIExp-0.27.3/pyniexp/scannersynch.py
--rw-rw-rw-   0        0        0    14046 2021-03-23 15:38:50.000000 PyNIExp-0.27.3/pyniexp/scannersynch_deprecated.py
--rw-rw-rw-   0        0        0     8490 2022-04-25 16:26:20.000000 PyNIExp-0.27.3/pyniexp/stimulation.py
--rw-rw-rw-   0        0        0     6551 2021-03-23 15:38:50.000000 PyNIExp-0.27.3/pyniexp/stimulatordlg.py
--rw-rw-rw-   0        0        0    21024 2021-03-23 15:38:50.000000 PyNIExp-0.27.3/pyniexp/stimulatordlg.ui
--rw-rw-rw-   0        0        0      903 2021-03-23 15:38:50.000000 PyNIExp-0.27.3/pyniexp/triggers.py
--rw-rw-rw-   0        0        0      889 2021-03-23 15:38:50.000000 PyNIExp-0.27.3/pyniexp/utils.py
--rw-rw-rw-   0        0        0       42 2022-04-25 16:29:42.574375 PyNIExp-0.27.3/setup.cfg
--rw-rw-rw-   0        0        0      821 2022-04-25 16:26:32.000000 PyNIExp-0.27.3/setup.py
+drwxrwxrwx   0        0        0        0 2024-05-29 10:17:35.820134 pyniexp-0.28.post3/
+-rw-rw-rw-   0        0        0     1353 2024-05-28 10:49:10.000000 pyniexp-0.28.post3/.gitignore
+-rw-rw-rw-   0        0        0     1088 2024-05-28 11:57:22.000000 pyniexp-0.28.post3/LICENSE
+-rw-rw-rw-   0        0        0     2662 2024-05-29 10:17:35.815284 pyniexp-0.28.post3/PKG-INFO
+-rw-rw-rw-   0        0        0      747 2024-05-28 17:42:45.000000 pyniexp-0.28.post3/README.md
+drwxrwxrwx   0        0        0        0 2024-05-29 10:17:35.685610 pyniexp-0.28.post3/examples/
+-rw-rw-rw-   0        0        0      136 2024-05-28 10:49:10.000000 pyniexp-0.28.post3/examples/config_TES.json
+-rw-rw-rw-   0        0        0      138 2024-05-28 10:49:10.000000 pyniexp-0.28.post3/examples/config_TES_sim.json
+-rw-rw-rw-   0        0        0      499 2024-05-28 10:49:10.000000 pyniexp-0.28.post3/examples/config_TI.json
+-rw-rw-rw-   0        0        0     1164 2024-05-28 10:49:10.000000 pyniexp-0.28.post3/examples/config_scanner.json
+-rw-rw-rw-   0        0        0      847 2024-05-28 16:11:51.000000 pyniexp-0.28.post3/examples/example_TCPreceiver.py
+-rw-rw-rw-   0        0        0      522 2024-05-28 16:11:48.000000 pyniexp-0.28.post3/examples/example_TCPsender.py
+-rw-rw-rw-   0        0        0      123 2024-05-28 17:39:59.000000 pyniexp-0.28.post3/examples/example_TI.py
+-rw-rw-rw-   0        0        0      928 2024-05-28 16:11:55.000000 pyniexp-0.28.post3/examples/example_UDPreceiver.py
+-rw-rw-rw-   0        0        0      531 2024-05-28 16:11:58.000000 pyniexp-0.28.post3/examples/example_UDPsender.py
+-rw-rw-rw-   0        0        0      750 2024-05-28 16:01:20.000000 pyniexp-0.28.post3/examples/example_mlplugins.py
+-rw-rw-rw-   0        0        0     6597 2024-05-28 16:09:52.000000 pyniexp-0.28.post3/examples/example_scannersynch.py
+-rw-rw-rw-   0        0        0      683 2024-05-28 14:43:17.000000 pyniexp-0.28.post3/examples/example_stimulation.py
+-rw-rw-rw-   0        0        0      281 2024-05-28 15:54:26.000000 pyniexp-0.28.post3/examples/example_stimulatordlg.py
+-rw-rw-rw-   0        0        0      979 2024-05-29 10:17:12.000000 pyniexp-0.28.post3/pyproject.toml
+-rw-rw-rw-   0        0        0       89 2024-05-28 11:39:35.000000 pyniexp-0.28.post3/requirements.txt
+-rw-rw-rw-   0        0        0       42 2024-05-29 10:17:35.820134 pyniexp-0.28.post3/setup.cfg
+drwxrwxrwx   0        0        0        0 2024-05-29 10:17:35.581997 pyniexp-0.28.post3/src/
+drwxrwxrwx   0        0        0        0 2024-05-29 10:17:35.812282 pyniexp-0.28.post3/src/PyNIExp.egg-info/
+-rw-rw-rw-   0        0        0     2662 2024-05-29 10:17:35.000000 pyniexp-0.28.post3/src/PyNIExp.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0     1173 2024-05-29 10:17:35.000000 pyniexp-0.28.post3/src/PyNIExp.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-05-29 10:17:35.000000 pyniexp-0.28.post3/src/PyNIExp.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       82 2024-05-29 10:17:35.000000 pyniexp-0.28.post3/src/PyNIExp.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        8 2024-05-29 10:17:35.000000 pyniexp-0.28.post3/src/PyNIExp.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2024-05-29 10:17:35.730065 pyniexp-0.28.post3/src/pyniexp/
+-rw-rw-rw-   0        0        0       53 2024-05-28 17:39:25.000000 pyniexp-0.28.post3/src/pyniexp/__init__.py
+-rw-rw-rw-   0        0        0      430 2024-05-29 10:17:34.000000 pyniexp-0.28.post3/src/pyniexp/_version.py
+drwxrwxrwx   0        0        0        0 2024-05-29 10:17:35.740788 pyniexp-0.28.post3/src/pyniexp/kbutils/
+-rw-rw-rw-   0        0        0       33 2024-05-28 13:16:41.000000 pyniexp-0.28.post3/src/pyniexp/kbutils/__init__.py
+-rw-rw-rw-   0        0        0     1690 2024-05-28 13:12:37.000000 pyniexp-0.28.post3/src/pyniexp/kbutils/kbutils.py
+drwxrwxrwx   0        0        0        0 2024-05-29 10:17:35.750690 pyniexp-0.28.post3/src/pyniexp/mlplugins/
+-rw-rw-rw-   0        0        0       48 2024-05-28 16:00:56.000000 pyniexp-0.28.post3/src/pyniexp/mlplugins/__init__.py
+-rw-rw-rw-   0        0        0     2828 2024-05-28 16:00:27.000000 pyniexp-0.28.post3/src/pyniexp/mlplugins/mlplugins.py
+drwxrwxrwx   0        0        0        0 2024-05-29 10:17:35.760389 pyniexp-0.28.post3/src/pyniexp/network/
+-rw-rw-rw-   0        0        0       32 2024-05-28 16:11:38.000000 pyniexp-0.28.post3/src/pyniexp/network/__init__.py
+-rw-rw-rw-   0        0        0    14509 2024-05-28 16:12:47.000000 pyniexp-0.28.post3/src/pyniexp/network/connection.py
+drwxrwxrwx   0        0        0        0 2024-05-29 10:17:35.776389 pyniexp-0.28.post3/src/pyniexp/scanner/
+-rw-rw-rw-   0        0        0       95 2024-05-28 16:09:07.000000 pyniexp-0.28.post3/src/pyniexp/scanner/__init__.py
+-rw-rw-rw-   0        0        0    17571 2024-05-28 16:08:01.000000 pyniexp-0.28.post3/src/pyniexp/scanner/scannersynch.py
+-rw-rw-rw-   0        0        0      905 2024-05-28 16:07:32.000000 pyniexp-0.28.post3/src/pyniexp/scanner/triggers.py
+drwxrwxrwx   0        0        0        0 2024-05-29 10:17:35.795525 pyniexp-0.28.post3/src/pyniexp/stimulator/
+-rw-rw-rw-   0        0        0       84 2024-05-28 14:41:48.000000 pyniexp-0.28.post3/src/pyniexp/stimulator/__init__.py
+-rw-rw-rw-   0        0        0     8485 2024-05-28 14:41:40.000000 pyniexp-0.28.post3/src/pyniexp/stimulator/stimulation.py
+-rw-rw-rw-   0        0        0     6951 2024-05-28 15:03:31.000000 pyniexp-0.28.post3/src/pyniexp/stimulator/stimulatordlg.py
+-rw-rw-rw-   0        0        0    21024 2024-05-28 10:49:10.000000 pyniexp-0.28.post3/src/pyniexp/stimulator/stimulatordlg.ui
+drwxrwxrwx   0        0        0        0 2024-05-29 10:17:35.805596 pyniexp-0.28.post3/src/pyniexp/utils/
+-rw-rw-rw-   0        0        0       88 2024-05-28 13:16:26.000000 pyniexp-0.28.post3/src/pyniexp/utils/__init__.py
+-rw-rw-rw-   0        0        0     1434 2024-05-28 11:45:35.000000 pyniexp-0.28.post3/src/pyniexp/utils/utils.py
```

### Comparing `PyNIExp-0.27.3/pyniexp/connection.py` & `pyniexp-0.28.post3/src/pyniexp/network/connection.py`

 * *Files 23% similar despite different names*

```diff
@@ -1,17 +1,19 @@
 import socket, sys, struct
 from datetime import datetime
 from select import select
-from pyniexp.utils import clock
+from ..utils import clock
 
-if sys.byteorder == 'little': byteorder = '<'
-elif sys.byteorder == 'big': byteorder = '>'
+if sys.byteorder == "little":
+    byteorder = "<"
+elif sys.byteorder == "big":
+    byteorder = ">"
 
 
-class __Connect(clock):
+class Connection(clock):
 
     @property
     def status(self):
         raise NotImplementedError("NYI")
 
     @property
     def status_for_sending(self):
@@ -20,317 +22,420 @@
     @property
     def status_for_receiving(self):
         raise NotImplementedError("NYI")
 
     @property
     def is_open(self):
         return bool(self._status)
- 
+
     @property
     def remote_address(self):
         if self._is_IP_confirmed:
             return self.IP + " (confirmed)"
         else:
             return self.IP + " (unconfirmed)"
-    
-    _control_signal = {'value': '', 'decode': '', 'n_bytes': 0}
+
+    _control_signal = {"value": "", "decode": "", "n_bytes": 0}
+
     @property
     def control_signal(self):
-        val = self._control_signal['value']
-        if type(val) != list: val = [val]
+        val = self._control_signal["value"]
+        if type(val) != list:
+            val = [val]
         return val
+
     @control_signal.setter
-    def control_signal(self,val):
-        self._control_signal['value'] = val
-        
+    def control_signal(self, val):
+        self._control_signal["value"] = val
+
         n = 1
         if type(val) == list:
             n = len(val)
             val = val[0]
-        
-        if type(val) == str: 
-            self._control_signal['n_bytes'] = n*1
-            self._control_signal['decode'] = lambda d: [d.decode(self.encoding)]
-        elif type(val) == int: 
-            self._control_signal['n_bytes'] = n*struct.calcsize('i')
-            self._control_signal['decode'] = lambda d: list(struct.unpack(byteorder+str(n)+'i',d))
-        elif type(val) == float: 
-            self._control_signal['n_bytes'] = n*struct.calcsize('f')
-            self._control_signal['decode'] = lambda d: list(struct.unpack(byteorder+str(n)+'f',d))
 
-    def __init__(self,IP='127.0.0.1',port=1234,encoding='UTF-8',control_signal='',timeout=20):
+        if type(val) == str:
+            self._control_signal["n_bytes"] = n * 1
+            self._control_signal["decode"] = lambda d: [d.decode(self.encoding)]
+        elif type(val) == int:
+            self._control_signal["n_bytes"] = n * struct.calcsize("i")
+            self._control_signal["decode"] = lambda d: list(
+                struct.unpack(byteorder + str(n) + "i", d)
+            )
+        elif type(val) == float:
+            self._control_signal["n_bytes"] = n * struct.calcsize("f")
+            self._control_signal["decode"] = lambda d: list(
+                struct.unpack(byteorder + str(n) + "f", d)
+            )
+
+    def __init__(
+        self, IP="127.0.0.1", port=1234, encoding="UTF-8", control_signal="", timeout=20
+    ):
         super().__init__()
-        
+
         self.IP = IP
         self.port = port
         self.encoding = encoding
         self.control_signal = control_signal
         self.timeout = timeout
 
         self._formats = {
-            'short': {
-                'format':'h',
-                'n_bytes': struct.calcsize('h'),
-                'encode': lambda d: struct.pack('<h',d),
-                'decode': lambda d: struct.unpack('<h',d)[0]
+            "short": {
+                "format": "h",
+                "n_bytes": struct.calcsize("h"),
+                "encode": lambda d: struct.pack("<h", d),
+                "decode": lambda d: struct.unpack("<h", d)[0],
             },
-            'ushort': {
-                'format':'H',
-                'n_bytes': struct.calcsize('H'),
-                'encode': lambda d: struct.pack('<H',d),
-                'decode': lambda d: struct.unpack('<H',d)[0]
+            "ushort": {
+                "format": "H",
+                "n_bytes": struct.calcsize("H"),
+                "encode": lambda d: struct.pack("<H", d),
+                "decode": lambda d: struct.unpack("<H", d)[0],
             },
-            'int': {
-                'format':'i',
-                'n_bytes': struct.calcsize('i'),
-                'encode': lambda d: struct.pack('<i',d),
-                'decode': lambda d: struct.unpack('<i',d)[0]
+            "int": {
+                "format": "i",
+                "n_bytes": struct.calcsize("i"),
+                "encode": lambda d: struct.pack("<i", d),
+                "decode": lambda d: struct.unpack("<i", d)[0],
             },
-            'uint': {
-                'format':'I',
-                'n_bytes': struct.calcsize('I'),
-                'encode': lambda d: struct.pack('<I',d),
-                'decode': lambda d: struct.unpack('<I',d)[0]
+            "uint": {
+                "format": "I",
+                "n_bytes": struct.calcsize("I"),
+                "encode": lambda d: struct.pack("<I", d),
+                "decode": lambda d: struct.unpack("<I", d)[0],
+            },
+            "float": {
+                "format": "f",
+                "n_bytes": struct.calcsize("f"),
+                "encode": lambda d: struct.pack("<f", d),
+                "decode": lambda d: struct.unpack("<f", d)[0],
             },
-            'float': {
-                'format':'f',
-                'n_bytes': struct.calcsize('f'),
-                'encode': lambda d: struct.pack('<f',d),
-                'decode': lambda d: struct.unpack('<f',d)[0]
-            }
         }
 
         self.sending_time_stamp = False
         self.wait_for_controlsignal = False
         self.quiet = False
 
         self._socket = None
-        self._status = 0 # 0 - closed; -1 - open for receiving; 1 - open for sending
+        self._status = 0  # 0 - closed; -1 - open for receiving; 1 - open for sending
         self._is_IP_confirmed = False
-    
+
     def __del__(self):
         self.close()
-    
+
     def info(self):
         print(self.__class__.__name__.upper(), "connection")
         print("\tIP:\t\t", self.IP)
         print("\tport:\t\t", self.port)
         print("\tTime out:\t", self.timeout)
         print("\tstatus:\t\t", self.status)
         print("Transfer")
         print("\tEncoding:\t\t", self.encoding)
         print("\tControl signal:\t", self.control_signal)
-    
-    def close(self,send_control_signal=True):
+
+    def close(self, send_control_signal=True):
         if self.is_open:
-            if len(self.control_signal) and send_control_signal: 
+            if len(self.control_signal) and send_control_signal:
                 self.sending_time_stamp = False
                 self.send_data(self.control_signal)
-            
-            if self.wait_for_controlsignal: pass
-        
+
+            if self.wait_for_controlsignal:
+                pass
+
             self._socket.close()
             self._status = 0
-            self.log('Connection closed with {:s}'.format(self.remote_address))
-    
+            self.log("Connection closed with {:s}".format(self.remote_address))
+
     def ready_to_receive(self):
-        return len(select([self._socket],[],[],0.001)[0]) > 0
+        return len(select([self._socket], [], [], 0.001)[0]) > 0
 
-    def send_data(self,dat):
-        if not(self.status_for_sending):
-            self.log('ERROR - Connection with {:s} is not ready for sending!'.format(self.remote_address))
+    def send_data(self, dat):
+        if not (self.status_for_sending):
+            self.log(
+                "ERROR - Connection with {:s} is not ready for sending!".format(
+                    self.remote_address
+                )
+            )
             return
-    
-        if type(dat) != list: dat = [dat]
-        
+
+        if type(dat) != list:
+            dat = [dat]
+
         t = datetime.now()
-        if self.sending_time_stamp: dat.insert(0,t.timestamp())
-        
+        if self.sending_time_stamp:
+            dat.insert(0, t.timestamp())
+
         for d in dat:
-            if type(d) == str: self._socket.send(bytes(d,self.encoding))
-            else: self._socket.send(self._formats[type(d).__name__]['encode'](d))
-            
-        return t, len(dat)-self.sending_time_stamp
+            if type(d) == str:
+                self._socket.send(bytes(d, self.encoding))
+            else:
+                self._socket.send(self._formats[type(d).__name__]["encode"](d))
+
+        return t, len(dat) - self.sending_time_stamp
 
     def flush(self):
         try:
             self._socket.recv(1024000000000)
         except:
             pass
 
-    def log(self,msg):
-        if ~self.quiet | any([msg.find(s) != -1 for s in ['ERROR','WARNING','USER']]):
-            print('[{:.3f}s] {:s}'.format(self.clock, msg))
+    def log(self, msg):
+        if ~self.quiet | any([msg.find(s) != -1 for s in ["ERROR", "WARNING", "USER"]]):
+            print("[{:.3f}s] {:s}".format(self.clock, msg))
+
 
+class Udp(Connection):
 
-class Udp(__Connect):
-    
     @property
     def status(self):
         if self._status == -1:
-            return 'ready for receiving'
+            return "ready for receiving"
         elif self._status == 1:
-            return 'ready for sending'
-        else: # 0
-            return 'closed'
+            return "ready for sending"
+        else:  # 0
+            return "closed"
 
     @property
     def status_for_sending(self):
-        return self.status == 'ready for sending'
+        return self.status == "ready for sending"
 
     @property
     def status_for_receiving(self):
-        return self.status == 'ready for receiving'
+        return self.status == "ready for receiving"
 
-    def __init__(self,IP='127.0.0.1',port=1234,encoding='UTF-8',control_signal='#',timeout=20):
-        super().__init__(IP,port,encoding,control_signal,timeout)
+    def __init__(
+        self,
+        IP="127.0.0.1",
+        port=1234,
+        encoding="UTF-8",
+        control_signal="#",
+        timeout=20,
+    ):
+        super().__init__(IP, port, encoding, control_signal, timeout)
 
         self._socket = socket.socket(socket.AF_INET, socket.SOCK_DGRAM)
 
     def connect_for_receiving(self):
         self._socket.bind((self.IP, self.port))
 
         if len(self.control_signal):
             data = [0]
             while chr(data[0]) != self.control_signal[0]:
-                while not(self.ready_to_receive()): pass
-                data, addr= self._socket.recvfrom(16)
+                while not (self.ready_to_receive()):
+                    pass
+                data, addr = self._socket.recvfrom(16)
                 self._is_IP_confirmed = addr[0] == self.IP
         self.IP = addr[0]
         self._status = -1
-        self.log('Connection with {:s} is {:s}'.format(self.remote_address,self.status))
-    
+        self.log(
+            "Connection with {:s} is {:s}".format(self.remote_address, self.status)
+        )
+
     def connect_for_sending(self):
         err = self._socket.connect_ex(((self.IP, self.port)))
-        if not(err):
+        if not (err):
             self._status = 1
             self._is_IP_confirmed = True
         else:
-            self.log('Establishing connection for sending with {:s} failed with error: {:s}'.format(self.remote_address,err))
+            self.log(
+                "Establishing connection for sending with {:s} failed with error: {:s}".format(
+                    self.remote_address, err
+                )
+            )
             return
 
-        if len(self.control_signal): 
+        if len(self.control_signal):
             self.sending_time_stamp = False
             self.send_data(self.control_signal)
-        self.log('Connection with {:s} is {:s}'.format(self.remote_address,self.status))
-
-    def reopen(self,operation='receiving'):
-        if not(self.is_open):
-            if operation == 'receiving':
+        self.log(
+            "Connection with {:s} is {:s}".format(self.remote_address, self.status)
+        )
+
+    def reopen(self, operation="receiving"):
+        if not (self.is_open):
+            if operation == "receiving":
                 self._socket = socket.socket(socket.AF_INET, socket.SOCK_DGRAM)
                 self.connect_for_receiving()
-            elif operation == 'sending':
+            elif operation == "sending":
                 self._socket = socket.socket(socket.AF_INET, socket.SOCK_DGRAM)
                 self.connect_for_sending()
             else:
-                self.log('ERROR - Unknown operation:{:s}'.format(operation))
+                self.log("ERROR - Unknown operation:{:s}".format(operation))
 
-    def receive_data(self,n=0,dtype='str'):
-        if not(self.status_for_receiving):
-            self.log('ERROR - Connection with {:s} is not ready for receiving!'.format(self.remote_address))
+    def receive_data(self, n=0, dtype="str"):
+        if not (self.status_for_receiving):
+            self.log(
+                "ERROR - Connection with {:s} is not ready for receiving!".format(
+                    self.remote_address
+                )
+            )
             return
-    
+
         dat = []
-        while not(n) or len(dat) < (n+self.sending_time_stamp):
+        while not (n) or len(dat) < (n + self.sending_time_stamp):
             if self.ready_to_receive():
 
                 # check for closing signal
                 try:
-                    if self._control_signal['decode'](self._socket.recv(self._control_signal['n_bytes'], socket.MSG_PEEK)) == self.control_signal:
+                    if (
+                        self._control_signal["decode"](
+                            self._socket.recv(
+                                self._control_signal["n_bytes"], socket.MSG_PEEK
+                            )
+                        )
+                        == self.control_signal
+                    ):
                         self.close(self.wait_for_controlsignal)
                         return dat
-                except: pass
+                except:
+                    pass
 
+                if self.sending_time_stamp and not (len(dat)):
+                    dat += [
+                        datetime.fromtimestamp(
+                            struct.unpack(byteorder + "1f", self._socket.recv(4))[0]
+                        )
+                    ]
 
-                if self.sending_time_stamp and not(len(dat)):
-                    dat += [datetime.fromtimestamp(struct.unpack(byteorder+'1f',self._socket.recv(4))[0])]
-           
                 d = self._socket.recv(1024)
-                if len(d) % 4: dtype = 'str' # Cave: No 4(-8-12-16-...)-char-long string is allowed
-                
-                if dtype == 'str': dat += [d.decode(self.encoding)]
-                elif dtype == 'int': dat += list(struct.unpack(byteorder+str(n)+'i',d))
-                elif dtype == 'float': dat += list(struct.unpack(byteorder+str(n)+'f',d))
+                if len(d) % 4:
+                    dtype = (
+                        "str"  # Cave: No 4(-8-12-16-...)-char-long string is allowed
+                    )
+
+                if dtype == "str":
+                    dat += [d.decode(self.encoding)]
+                elif dtype == "int":
+                    dat += list(struct.unpack(byteorder + str(n) + "i", d))
+                elif dtype == "float":
+                    dat += list(struct.unpack(byteorder + str(n) + "f", d))
 
             else:
                 t0 = datetime.now()
-                while not(self.ready_to_receive()) and ((datetime.now() - t0).total_seconds() < self.timeout): pass
-                if not(self.ready_to_receive()): break
+                while not (self.ready_to_receive()) and (
+                    (datetime.now() - t0).total_seconds() < self.timeout
+                ):
+                    pass
+                if not (self.ready_to_receive()):
+                    break
         return dat
 
-class Tcp(__Connect):
+
+class Tcp(Connection):
     @property
     def status(self):
         if self._status == -1:
-            return 'open as server'
+            return "open as server"
         elif self._status == 1:
-            return 'open as client'
-        else: # 0
-            return 'closed'
+            return "open as client"
+        else:  # 0
+            return "closed"
 
     @property
     def status_for_sending(self):
-        return self.status.find('open') != -1
+        return self.status.find("open") != -1
 
     @property
     def status_for_receiving(self):
-        return self.status.find('open') != -1
+        return self.status.find("open") != -1
 
-    def __init__(self,IP=None,port=1234,encoding='UTF-8',control_signal='',timeout=20):
-        super().__init__(IP,port,encoding,control_signal,timeout)
+    def __init__(
+        self, IP=None, port=1234, encoding="UTF-8", control_signal="", timeout=20
+    ):
+        super().__init__(IP, port, encoding, control_signal, timeout)
 
         self._socket = socket.socket(socket.AF_INET, socket.SOCK_STREAM)
-        
+
     def open_as_server(self):
-        self._socket.bind(('', self.port))
+        self._socket.bind(("", self.port))
         self._socket.listen(1)
         self._socket, addr = self._socket.accept()
         self._status = -1
-        if not(self.IP is None):
+        if not (self.IP is None):
             self._is_IP_confirmed = addr[0] == self.IP
         self.IP = addr[0]
-        self.log('{:s}; connected with client at {:s}:{:d}'.format(self.status,self.IP,addr[1]))
+        self.log(
+            "{:s}; connected with client at {:s}:{:d}".format(
+                self.status, self.IP, addr[1]
+            )
+        )
 
     def open_as_client(self):
         self._socket.connect((self.IP, self.port))
         self._status = 1
         self._is_IP_confirmed = True
-        self.log('{:s}; connected to server at {:s}:{:d}'.format(self.status,self.IP,self.port))
-    
-    def receive_data(self,n=0,dtype=None):
-        if not(self.status_for_receiving):
-            self.log('ERROR - Connection with {:s} is not ready for receiving!'.format(self.remote_address))
+        self.log(
+            "{:s}; connected to server at {:s}:{:d}".format(
+                self.status, self.IP, self.port
+            )
+        )
+
+    def receive_data(self, n=0, dtype=None):
+        if not (self.status_for_receiving):
+            self.log(
+                "ERROR - Connection with {:s} is not ready for receiving!".format(
+                    self.remote_address
+                )
+            )
             return
-    
-        if dtype == 'str': dat = ''
-        else: dat = []
+
+        if dtype == "str":
+            dat = ""
+        else:
+            dat = []
         n_received = 0
-        while not(n) or n_received < n:
+        while not (n) or n_received < n:
             if self.ready_to_receive():
 
                 # only at the beginning)
-                if not(n_received):
+                if not (n_received):
                     # - check for closing signal
                     try:
-                        if self._control_signal['decode'](self._socket.recv(self._control_signal['n_bytes'], socket.MSG_PEEK)) == self.control_signal:
+                        if (
+                            self._control_signal["decode"](
+                                self._socket.recv(
+                                    self._control_signal["n_bytes"], socket.MSG_PEEK
+                                )
+                            )
+                            == self.control_signal
+                        ):
                             self.close(self.wait_for_controlsignal)
                             return dat
-                    except: pass
+                    except:
+                        pass
 
                     # - check for time stamp
                     if self.sending_time_stamp:
-                        ts = [datetime.fromtimestamp(self._formats['float']['decode'](self._socket.recv(self._formats['float']['n_bytes'])))]
-           
-                if dtype is None: dat += [self._socket.recv(1)]
-                elif dtype == 'str': dat += self._socket.recv(1).decode(self.encoding)
-                else: dat += [self._formats[dtype]['decode'](self._socket.recv(self._formats[dtype]['n_bytes']))]
+                        ts = [
+                            datetime.fromtimestamp(
+                                self._formats["float"]["decode"](
+                                    self._socket.recv(self._formats["float"]["n_bytes"])
+                                )
+                            )
+                        ]
+
+                if dtype is None:
+                    dat += [self._socket.recv(1)]
+                elif dtype == "str":
+                    dat += self._socket.recv(1).decode(self.encoding)
+                else:
+                    dat += [
+                        self._formats[dtype]["decode"](
+                            self._socket.recv(self._formats[dtype]["n_bytes"])
+                        )
+                    ]
                 n_received += 1
             else:
                 t0 = datetime.now()
-                while not(self.ready_to_receive()) and ((datetime.now() - t0).total_seconds() < self.timeout): pass
-                if not(self.ready_to_receive()): break
-        
+                while not (self.ready_to_receive()) and (
+                    (datetime.now() - t0).total_seconds() < self.timeout
+                ):
+                    pass
+                if not (self.ready_to_receive()):
+                    break
+
         if self.sending_time_stamp:
-            if dtype == 'str': dat = ts + [dat]
-            else: dat = ts + dat
+            if dtype == "str":
+                dat = ts + [dat]
+            else:
+                dat = ts + dat
 
-        return dat
+        return dat
```

### Comparing `PyNIExp-0.27.3/pyniexp/kbutils.py` & `pyniexp-0.28.post3/src/pyniexp/kbutils/kbutils.py`

 * *Files 15% similar despite different names*

```diff
@@ -1,64 +1,71 @@
-import time
-
 try:
     import keyboard
 except ImportError:
     print('module "keyboard" is not installed')
     raise ImportError
 
 kbLayout = []
-if hasattr(keyboard._os_keyboard, 'official_virtual_keys'):
+if hasattr(keyboard._os_keyboard, "official_virtual_keys"):
     kbLayout = [k[0] for k in keyboard._os_keyboard.official_virtual_keys.values()]
 
 
 class Key:
-    name = ''
-    state = ''
+    name = ""
+    state = ""
     timeDown = 0
     timeUp = 0
+
     @property
     def time(self):
-        return max(self.timeDown,self.timeUp)
+        return max(self.timeDown, self.timeUp)
 
-    def __init__(self,name):
+    def __init__(self, name):
         self.name = name
-        self.state = 'up'
+        self.state = "up"
+
+    def eventTime(self, etype):
+        if etype == "down":
+            return self.timeDown
+        elif etype == "up":
+            return self.timeUp
+        else:
+            return -1
 
-    def eventTime(self,etype):
-        if etype == 'down': return self.timeDown
-        elif etype == 'up': return self.timeUp
-        else: return -1
-    
-    def update(self,etype,val):
+    def update(self, etype, val):
         self.state = etype
-        if self.state == 'down': self.timeDown = val
-        elif self.state == 'up': self.timeUp = val
-        
+        if self.state == "down":
+            self.timeDown = val
+        elif self.state == "up":
+            self.timeUp = val
+
+
 class Kb:
-    
-    @property 
+
+    @property
     def is_alive(self):
         return self.__is_alive
 
     def __init__(self):
         # Private property
         self.__keys = [Key(name) for name in kbLayout]
         self.__is_alive = False
-    
+
         self.start()
-        
+
     def start(self):
-        if not(self.is_alive): keyboard.hook(self.__store_keys)
+        if not (self.is_alive):
+            keyboard.hook(self.__store_keys)
         self.__is_alive = True
 
     def stop(self):
-        if self.is_alive: keyboard.unhook_all()
+        if self.is_alive:
+            keyboard.unhook_all()
         self.__is_alive = False
 
     def kbCheck(self):
         return [(k.name, k.state, k.time) for k in self.__keys]
 
-    def __store_keys(self,e):
-            K = [k for k in self.__keys if k.name == e.name]
-            if len(K):
-                K[0].update(e.event_type,e.time)
+    def __store_keys(self, e):
+        K = [k for k in self.__keys if k.name == e.name]
+        if len(K):
+            K[0].update(e.event_type, e.time)
```

### Comparing `PyNIExp-0.27.3/pyniexp/mlplugins.py` & `pyniexp-0.28.post3/src/pyniexp/mlplugins/mlplugins.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,17 +1,19 @@
 from numpy import array, prod, flip
 from multiprocessing import Process, Value, RawArray
-from loguru import logger
 from matlab import double
+from ..utils import getLogger
 
 SIG_NOTSTARTED = -1
 SIG_RUNNING = 1
 SIG_STOPPED = 0
 SIG_NEWIMAGE = 10
 
+logger = getLogger()
+
 class dataProcess:
     __process = Process()
 
     def __init__(self,data_size,autostart=True):
         self._buffer = RawArray('d',[0]*data_size)
         self._signal = Value('b',SIG_NOTSTARTED)
         if autostart: self.start_process()
```

### Comparing `PyNIExp-0.27.3/pyniexp/scannersynch.py` & `pyniexp-0.28.post3/src/pyniexp/scanner/scannersynch.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,396 +1,523 @@
 from math import inf
 import sys, json
 from time import time
-from multiprocessing import Process, Value, RawValue, RawArray
+from multiprocessing import Process, Value, RawArray
 
-import pyniexp.utils as utils
+from ..utils import binvec2dec, ismember
 
 try:
     import nidaqmx
 except ImportError:
-    print('WARNING: nidaqmx module is not available --> ', end='')
-    print('You can run ScannerSynch only in emulation mode')
+    print("WARNING: nidaqmx module is not available --> ", end="")
+    print("You can run ScannerSynch only in emulation mode")
 
 try:
     import pyniexp.kbutils as kbutils
 except ImportError:
-    print('WARNING: kbutils module is not available --> ', end='')
-    print('You cannot emulate buttons')
+    print("WARNING: kbutils module is not available --> ", end="")
+    print("You cannot emulate buttons")
+
 
 #### Main class
-class scanner_synch:
-    
-    ## Properties 
+class ScannerSynch:
+
+    ## Properties
     # Private properties
     __config = None
     __buttonbox_readout = False
     __process = Process()
 
-    __isDAQ = 'nidaqmx' in sys.modules
-    __isKb = 'pyniexp.kbutils' in sys.modules # Button emulation (keyboard)
+    __isDAQ = "nidaqmx" in sys.modules
+    __isKb = "pyniexp.kbutils" in sys.modules  # Button emulation (keyboard)
 
     # Public properties
-    buttonbox_timeout = inf # second (timeout for WaitForButtonPress)
+    buttonbox_timeout = inf  # second (timeout for WaitForButtonPress)
     is_inverted = False
 
     # Public read-only properties
     __emul_synch = 0
+
     @property
     def emul_synch(self):
-        return self.__emul_synch   
+        return self.__emul_synch
+
     __emul_buttons = 0
+
     @property
     def emul_buttons(self):
-        return self.__emul_buttons   
+        return self.__emul_buttons
+
+    __readout_time = [0.5, 0.5]  # sec to store data before refresh 1*n (default 0.5)
 
-    __readout_time = [0.5, 0.5] # sec to store data before refresh 1*n (default 0.5)
     @property
     def readout_time(self):
         return self.__readout_time
 
     # Dependent properties
     @property
     def is_valid(self):
         valid = True
         valid = valid and (self.__isDAQ or (self.emul_buttons and self.emul_buttons))
-        if (self.emul_synch == 1) and not(self.TR):
-            print('Emulation: Scanner synch pulse is not in use --> ', end='')
-            print('You need to set TR!')
+        if (self.emul_synch == 1) and not (self.TR):
+            print("Emulation: Scanner synch pulse is not in use --> ", end="")
+            print("You need to set TR!")
             valid = valid and False
-        if (self.emul_buttons == 1) and not(len(self.buttons)):
-            print('Emulation: Buttonbox is not in use           --> ', end='')
-            print('You need to set Buttons!')
+        if (self.emul_buttons == 1) and not (len(self.buttons)):
+            print("Emulation: Buttonbox is not in use           --> ", end="")
+            print("You need to set Buttons!")
             valid = valid and False
-        if (self.emul_buttons == 0) and not(len(self.__buttonbox)):
-            print('Buttonbox: none is configured                --> ', end='')
-            print('You need to add at least one buttonbox!')
+        if (self.emul_buttons == 0) and not (len(self.__buttonbox)):
+            print("Buttonbox: none is configured                --> ", end="")
+            print("You need to add at least one buttonbox!")
             valid = valid and False
-        
-        if not(valid): print('Validation: FAILED!')
+
+        if not (valid):
+            print("Validation: FAILED!")
 
         return valid
 
     ## Constructor
-    def __init__(self,config="config_scanner.json",emul_synch=False,emul_buttons=False):
+    def __init__(
+        self, config="config_scanner.json", emul_synch=False, emul_buttons=False
+    ):
         self.__buttonbox = []
 
-        print('Initialising Scanner Synch...')
-        if not(config is None):
+        print("Initialising Scanner Synch...")
+        if not (config is None):
             with open(config) as fid:
                 self.__config = json.load(fid)
         else:
-            if emul_synch != -1: emul_synch = 1
-            if emul_buttons != -1: emul_buttons = 1
+            if emul_synch != -1:
+                emul_synch = 1
+            if emul_buttons != -1:
+                emul_buttons = 1
             self.__isDAQ = False
 
         self.__emul_synch = emul_synch
         self.__emul_buttons = emul_buttons
 
         # test environment
         if (self.emul_synch == 0) or (self.emul_buttons == 0):
             try:
                 D = nidaqmx.system.System.local().devices
-                D = [d for d in D if d.name == self.__config['DAQ']['Hardware']]
+                D = [d for d in D if d.name == self.__config["DAQ"]["Hardware"]]
                 D = D[0]
                 D.self_test_device()
             except:
-                print('WARNING - DAQ card is not available:', sys.exc_info()[0])
+                print("WARNING - DAQ card is not available:", sys.exc_info()[0])
                 self.__isDAQ = False
-                if self.__emul_synch != -1: self.__emul_synch = 1
-                if self.__emul_buttons != -1: self.__emul_buttons = 1
-        else: self.__isDAQ = False
+                if self.__emul_synch != -1:
+                    self.__emul_synch = 1
+                if self.__emul_buttons != -1:
+                    self.__emul_buttons = 1
+        else:
+            self.__isDAQ = False
 
-        self._t0 = Value('d',time())      # internal timer
-        self._keep_running = Value('b',-1) # internal signal (-1: not started, 1: running)
+        self._t0 = Value("d", time())  # internal timer
+        self._keep_running = Value(
+            "b", -1
+        )  # internal signal (-1: not started, 1: running)
 
     ## Destructor
     def __del__(self):
         if self._keep_running.value:
             self._keep_running.value = 0
 
     ## Utils
     # Process
-    def start_process(self,max_pulses=None):
-        if self.__process.is_alive(): 
-            print('Process is already running')
+    def start_process(self, max_pulses=None):
+        if self.__process.is_alive():
+            print("Process is already running")
             return
 
-        if max_pulses is None: max_pulses = self.__config['DAQ']['BufferLength']
+        if max_pulses is None:
+            max_pulses = self.__config["DAQ"]["BufferLength"]
 
-        print('Starting process...')
+        print("Starting process...")
 
-        if not(self.is_valid): 
-            print('You have to start the process manually by calling <object>.start_process()!')
+        if not (self.is_valid):
+            print(
+                "You have to start the process manually by calling <object>.start_process()!"
+            )
             return
-        self._synchpulsetimes = RawArray('d', [-1]*max_pulses)
-        self._buttonstates = RawArray('b', [0]*self.number_of_buttons)
-        self._buttonpresstimes = [RawArray('d', [-1]*max_pulses) for n in range(0,self.number_of_buttons)]
-        self._select_buttons = RawArray('b',[1]*self.number_of_buttons) # record only selected buttons
-        self._button_record_period = RawArray('d',[0, inf])               # record buttons only in this period
-        self.__readout_time = [self.__readout_time[0]] + [self.__readout_time[1]]*self.number_of_buttons
-        self._control_buttonevent = RawArray('d', [0]*len(self.control_buttons))
+        self._synchpulsetimes = RawArray("d", [-1] * max_pulses)
+        self._buttonstates = RawArray("b", [0] * self.number_of_buttons)
+        self._buttonpresstimes = [
+            RawArray("d", [-1] * max_pulses) for n in range(0, self.number_of_buttons)
+        ]
+        self._select_buttons = RawArray(
+            "b", [1] * self.number_of_buttons
+        )  # record only selected buttons
+        self._button_record_period = RawArray(
+            "d", [0, inf]
+        )  # record buttons only in this period
+        self.__readout_time = [self.__readout_time[0]] + [
+            self.__readout_time[1]
+        ] * self.number_of_buttons
+        self._control_buttonevent = RawArray("d", [0] * len(self.control_buttons))
         self.__process = Process(target=self._run)
         self.__process.start()
-        while not(self.is_alive): pass
-        print('[{:.3f}s] - Process is running'.format(self.clock))
+        while not (self.is_alive):
+            pass
+        print("[{:.3f}s] - Process is running".format(self.clock))
 
     @property
     def is_alive(self):
         return self._keep_running.value == 1
 
     # Clock
     @property
     def clock(self):
         return time() - self._t0.value
 
     def reset_clock(self):
         self._t0.value = time()
 
     # TR
-    __TR = None    # emulated pulse frequency
+    __TR = None  # emulated pulse frequency
+
     @property
     def TR(self):
         return self.__TR
 
     @TR.setter
-    def TR(self,val):
+    def TR(self, val):
         if self.__process.is_alive():
             self.__process.terminate()
-        
+
         self.__TR = val
 
     # Buttons
-    def add_buttonbox(self,name='Nata'):
-        conf = [bbconf for bbconf in self.__config['ButtonBox'] if bbconf['Name'] == name]
-        if not(len(conf)): print('ERROR: no configuration found for \'{}\''.format(name)); return
-        elif len(conf) > 1:  print('ERROR: multiple matching configurations found {}'.format([c['Name'] for c in conf])); return
+    def add_buttonbox(self, name="Nata"):
+        conf = [
+            bbconf for bbconf in self.__config["ButtonBox"] if bbconf["Name"] == name
+        ]
+        if not (len(conf)):
+            print("ERROR: no configuration found for '{}'".format(name))
+            return
+        elif len(conf) > 1:
+            print(
+                "ERROR: multiple matching configurations found {}".format(
+                    [c["Name"] for c in conf]
+                )
+            )
+            return
         self.__buttonbox.append(conf[0])
 
     __buttons = []
+
     @property
     def buttons(self):
         return self.__buttons
 
     @buttons.setter
-    def buttons(self,val):
+    def buttons(self, val):
         if self.__isKb:
             if self.__process.is_alive():
                 self.__process.terminate()
-                
-            if not all(utils.ismember(val,kbutils.kbLayout)):
-                print('WARNING: Some buttons are not recognised in...')
+
+            if not all(ismember(val, kbutils.kbLayout)):
+                print("WARNING: Some buttons are not recognised in...")
                 print(kbutils.kbLayout)
                 return
 
             self.__buttons = val
-            self.__readout_time = [self.__readout_time[0]] + [self.__readout_time[1]]*(self.number_of_buttons)
+            self.__readout_time = [self.__readout_time[0]] + [
+                self.__readout_time[1]
+            ] * (self.number_of_buttons)
 
         else:
             print('WARNING: "kbutils" is not available')
-    
+
     @property
     def number_of_buttons(self):
-        if self.emul_buttons: return len(self.buttons)
-        else: return sum([len(c['ButtonCode']) for c in self.__buttonbox])
-    
+        if self.emul_buttons:
+            return len(self.buttons)
+        else:
+            return sum([len(c["ButtonCode"]) for c in self.__buttonbox])
+
     __control_buttons = []
+
     @property
     def control_buttons(self):
-        return self.__control_buttons    
+        return self.__control_buttons
+
     @control_buttons.setter
-    def control_buttons(self,val):
+    def control_buttons(self, val):
         if self.__isKb:
             if self.__process.is_alive():
                 self.__process.terminate()
-                
-            if not all(utils.ismember(val,kbutils.kbLayout)):
-                print('WARNING: Some buttons are not recognised in...')
+
+            if not all(ismember(val, kbutils.kbLayout)):
+                print("WARNING: Some buttons are not recognised in...")
                 print(kbutils.kbLayout)
                 return
 
             self.__control_buttons = val
 
         else:
             print('WARNING: "kbutils" is not available')
 
     ## Scanner Pulse
     @property
     def synch_count(self):
         return sum([i > -1 for i in self._synchpulsetimes])
 
     def reset_synch_count(self):
-        for n in range(0,len(self._synchpulsetimes)):
+        for n in range(0, len(self._synchpulsetimes)):
             self._synchpulsetimes[n] = -1
-    
+
     @property
     def synch_readout_time(self):
         return self.__readout_time[0]
 
-    def set_synch_readout_time(self,t):
+    def set_synch_readout_time(self, t):
         self.__readout_time[0] = t
-    
+
     def wait_for_synch(self):
-        if not(self.__process.is_alive()): 
-            print('Process is not running')
+        if not (self.__process.is_alive()):
+            print("Process is not running")
             return
 
         synch_count0 = self.synch_count
-        while not(self.synch_count > synch_count0): pass
-    
+        while not (self.synch_count > synch_count0):
+            pass
+
     @property
     def time_of_last_pulse(self):
-        return self._synchpulsetimes[self.synch_count-1]
-    
+        return self._synchpulsetimes[self.synch_count - 1]
+
     @property
     def measured_TR(self):
-        if self.synch_count > 1: return self.time_of_last_pulse - self._synchpulsetimes[self.synch_count-2] 
-        else: return 0
-    
+        if self.synch_count > 1:
+            return self.time_of_last_pulse - self._synchpulsetimes[self.synch_count - 2]
+        else:
+            return 0
+
     ## Buttons
-    def set_button_readout_time(self,t):
-        self.__readout_time = [self.__readout_time[0]] + [t]*(len(self.__readout_time)-1)
+    def set_button_readout_time(self, t):
+        self.__readout_time = [self.__readout_time[0]] + [t] * (
+            len(self.__readout_time) - 1
+        )
         self.__buttonbox_readout = False
-    
-    def set_buttonbox_readout_time(self,t):
-        self.__readout_time = [self.__readout_time[0]] + [t]*(len(self.__readout_time)-1)
+
+    def set_buttonbox_readout_time(self, t):
+        self.__readout_time = [self.__readout_time[0]] + [t] * (
+            len(self.__readout_time) - 1
+        )
         self.__buttonbox_readout = True
-    
+
     def reset_buttons(self):
-        for b in range(0,self.number_of_buttons): 
-            for n in range(0,len(self._buttonpresstimes[b])): 
+        for b in range(0, self.number_of_buttons):
+            for n in range(0, len(self._buttonpresstimes[b])):
                 self._buttonpresstimes[b][n] = -1
 
     @property
     def _last_button_indices(self):
-        return [sum([n > -1 for n in self._buttonpresstimes[b]])-1 for b in range(0,self.number_of_buttons)]
+        return [
+            sum([n > -1 for n in self._buttonpresstimes[b]]) - 1
+            for b in range(0, self.number_of_buttons)
+        ]
 
     @property
     def _time_of_last_buttonpresses(self):
-        return [self._buttonpresstimes[b][self._last_button_indices[b]] for b in range(0,self.number_of_buttons)]
+        return [
+            self._buttonpresstimes[b][self._last_button_indices[b]]
+            for b in range(0, self.number_of_buttons)
+        ]
 
     @property
     def buttonpresses(self):
-        e = [(b,n) for b in range(0,self.number_of_buttons) for n in self._buttonpresstimes[b] if n > self._button_record_period[0]]
+        e = [
+            (b, n)
+            for b in range(0, self.number_of_buttons)
+            for n in self._buttonpresstimes[b]
+            if n > self._button_record_period[0]
+        ]
         return sorted(e, key=lambda e: e[1])
 
-    def wait_for_button(self,timeout=None,ind_button=None,no_block=False,event_type='press'):
-        if not(self.__process.is_alive()): 
-            print('Process is not running')
+    def wait_for_button(
+        self, timeout=None, ind_button=None, no_block=False, event_type="press"
+    ):
+        if not (self.__process.is_alive()):
+            print("Process is not running")
             return
 
         BBoxQuery = self.clock
 
         # Onset
         self._button_record_period[0] = BBoxQuery
 
         # Offset
-        if timeout is None: timeout = self.buttonbox_timeout
-        wait = timeout < 0 # wait until timeout even in case of response
+        if timeout is None:
+            timeout = self.buttonbox_timeout
+        wait = timeout < 0  # wait until timeout even in case of response
         timeout = abs(timeout)
-        self._button_record_period[1] = self._button_record_period[0]+timeout
+        self._button_record_period[1] = self._button_record_period[0] + timeout
 
         # Select buttons
-        if type(ind_button) != list: ind_button = range(0,self.number_of_buttons)
-        for b in range(0,self.number_of_buttons):
+        if type(ind_button) != list:
+            ind_button = range(0, self.number_of_buttons)
+        for b in range(0, self.number_of_buttons):
             self._select_buttons[b] = any([b == n for n in ind_button])
 
-        if no_block: return
+        if no_block:
+            return
 
         while self.clock - BBoxQuery < timeout:
-            if wait: continue
-            if event_type == 'press' and any([e[1] > self._button_record_period[0] for e in self.buttonpresses]): break # (selected) button pressed
-            if event_type == 'release' and any([not(self._buttonstates[b]) 
-                for b in [e[0] for e in self.buttonpresses if e[1] > self._button_record_period[0]]]): break # (selected) button released                
-        
-        self._button_record_period[1] = self.clock # stop recording
-    
+            if wait:
+                continue
+            if event_type == "press" and any(
+                [e[1] > self._button_record_period[0] for e in self.buttonpresses]
+            ):
+                break  # (selected) button pressed
+            if event_type == "release" and any(
+                [
+                    not (self._buttonstates[b])
+                    for b in [
+                        e[0]
+                        for e in self.buttonpresses
+                        if e[1] > self._button_record_period[0]
+                    ]
+                ]
+            ):
+                break  # (selected) button released
+
+        self._button_record_period[1] = self.clock  # stop recording
+
     def control_buttonswith(self):
-        return [(self.control_buttons[b],self._control_buttonevent[b]) for b in range(len(self.control_buttons)) if self._control_buttonevent[b]]
-    
+        return [
+            (self.control_buttons[b], self._control_buttonevent[b])
+            for b in range(len(self.control_buttons))
+            if self._control_buttonevent[b]
+        ]
+
     def pressed_control_buttons(self):
         return [b[0] for b in self.control_buttonswith()]
-    
-    def control_button_time(self,cb):
+
+    def control_button_time(self, cb):
         return [b[1] for b in self.control_buttonswith() if b[0] == cb][0]
 
-    def reset_control_buttons(self,cb=[]):
+    def reset_control_buttons(self, cb=[]):
         if len(cb):
             cbs = [b in cb for b in self.control_buttons]
-        else: cbs = [False]*len(self.control_buttons)
+        else:
+            cbs = [False] * len(self.control_buttons)
         for b in range(len(self.control_buttons)):
             self._control_buttonevent[b] = self._control_buttonevent[b] * cbs[b]
 
     ## Low level methods
     def _run(self):
         # Start DAQ
         DAQ = []
-        if self.__isDAQ:            
+        if self.__isDAQ:
             DAQ.append(nidaqmx.Task())
             # Add channels for scanner pulse
-            DAQ[0].di_channels.add_di_chan(self.__config['DAQ']['Hardware'] + '/' + self.__config['SynchPulse']['Channel_Manual']) # manual
-            DAQ[0].di_channels.add_di_chan(self.__config['DAQ']['Hardware'] + '/' + self.__config['SynchPulse']['Channel_Scanner']) # scanner
+            DAQ[0].di_channels.add_di_chan(
+                self.__config["DAQ"]["Hardware"]
+                + "/"
+                + self.__config["SynchPulse"]["Channel_Manual"]
+            )  # manual
+            DAQ[0].di_channels.add_di_chan(
+                self.__config["DAQ"]["Hardware"]
+                + "/"
+                + self.__config["SynchPulse"]["Channel_Scanner"]
+            )  # scanner
 
             # Add channels for buttonbox(es)
             for bb in self.__buttonbox:
                 DAQ.append(nidaqmx.Task())
-                for ch in bb['Channels']:
-                    DAQ[-1].di_channels.add_di_chan(self.__config['DAQ']['Hardware'] + '/' + ch)
-        
+                for ch in bb["Channels"]:
+                    DAQ[-1].di_channels.add_di_chan(
+                        self.__config["DAQ"]["Hardware"] + "/" + ch
+                    )
+
         # Start KB
-        if self.emul_buttons or len(self.control_buttons): Kb = kbutils.Kb()
-    
+        if self.emul_buttons or len(self.control_buttons):
+            Kb = kbutils.Kb()
+
         self.reset_clock()
         t0 = self.clock
         while self._keep_running.value:
             t = self.clock
-            self.rate = t - t0; t0 = t # update rate (for self-diagnostics)
+            self.rate = t - t0
+            t0 = t  # update rate (for self-diagnostics)
 
             # Synch pulse
             if self.emul_synch != -1:
                 # - data
                 if self.emul_synch == 0:
-                    synch = any([d^self.is_inverted for d in DAQ[0].read()])
+                    synch = any([d ^ self.is_inverted for d in DAQ[0].read()])
                 elif self.emul_synch == 1:
-                    synch = not(self.synch_count) or (t-self.time_of_last_pulse >= self.TR)
+                    synch = not (self.synch_count) or (
+                        t - self.time_of_last_pulse >= self.TR
+                    )
                 # - process
-                if not(self.synch_count) or (t-self.time_of_last_pulse >= self.synch_readout_time):
-                    if synch: self._synchpulsetimes[self.synch_count] = t
-            
+                if not (self.synch_count) or (
+                    t - self.time_of_last_pulse >= self.synch_readout_time
+                ):
+                    if synch:
+                        self._synchpulsetimes[self.synch_count] = t
+
             # Buttons
             if self.emul_buttons != -1:
                 # - data
                 b_data = []
                 if self.emul_buttons == 0:
-                    for bb_ind in range(0,len(self.__buttonbox)):
-                        bb_code = utils.binvec2dec([d^self.is_inverted for d in DAQ[bb_ind+1].read()])
-                        if any([bb_code == ign for ign in self.__buttonbox[bb_ind]['Ignore']]): bb_code = -1 # ignore faulty signal
-                        b_data += utils.ismember(self.__buttonbox[bb_ind]['ButtonCode'],[bb_code])
+                    for bb_ind in range(0, len(self.__buttonbox)):
+                        bb_code = binvec2dec(
+                            [d ^ self.is_inverted for d in DAQ[bb_ind + 1].read()]
+                        )
+                        if any(
+                            [
+                                bb_code == ign
+                                for ign in self.__buttonbox[bb_ind]["Ignore"]
+                            ]
+                        ):
+                            bb_code = -1  # ignore faulty signal
+                        b_data += ismember(
+                            self.__buttonbox[bb_ind]["ButtonCode"], [bb_code]
+                        )
                 elif self.emul_buttons == 1:
-                    kb_data = Kb.kbCheck(); key_code = [k[0] for k in kb_data if k[1] == 'down']
-                    b_data = utils.ismember(self.buttons,key_code)
+                    kb_data = Kb.kbCheck()
+                    key_code = [k[0] for k in kb_data if k[1] == "down"]
+                    b_data = ismember(self.buttons, key_code)
                 # -process
-                if t >= self._button_record_period[0] and t <= self._button_record_period[1]:
+                if (
+                    t >= self._button_record_period[0]
+                    and t <= self._button_record_period[1]
+                ):
                     ToBp = self._time_of_last_buttonpresses
-                    if self.__buttonbox_readout: ToBp = [max(ToBp)]*self.number_of_buttons
-                    for n in range(0,self.number_of_buttons):
+                    if self.__buttonbox_readout:
+                        ToBp = [max(ToBp)] * self.number_of_buttons
+                    for n in range(0, self.number_of_buttons):
                         buttonstates0 = self._buttonstates[:]
-                        self._buttonstates[n] = b_data[n]*self._select_buttons[n]
-                        if self._buttonstates[n] and not(buttonstates0[n]) and (t-ToBp[n] > self.readout_time[n+1]):
-                            self._buttonpresstimes[n][self._last_button_indices[n]+1] = t
-            
+                        self._buttonstates[n] = b_data[n] * self._select_buttons[n]
+                        if (
+                            self._buttonstates[n]
+                            and not (buttonstates0[n])
+                            and (t - ToBp[n] > self.readout_time[n + 1])
+                        ):
+                            self._buttonpresstimes[n][
+                                self._last_button_indices[n] + 1
+                            ] = t
+
             # Control buttons
             if len(self.control_buttons):
-                kb_data = Kb.kbCheck(); key_code = [k[0] for k in kb_data if k[1] == 'down']
-                cb_data = utils.ismember(self.control_buttons,key_code)
+                kb_data = Kb.kbCheck()
+                key_code = [k[0] for k in kb_data if k[1] == "down"]
+                cb_data = ismember(self.control_buttons, key_code)
                 for b in range(len(self.control_buttons)):
-                    if cb_data[b]: self._control_buttonevent[b] = t
+                    if cb_data[b]:
+                        self._control_buttonevent[b] = t
 
-            if self._keep_running.value == -1: self._keep_running.value = 1
+            if self._keep_running.value == -1:
+                self._keep_running.value = 1
 
-        print('Scanner Synch is closing...')
+        print("Scanner Synch is closing...")
         if self.__isDAQ:
             [d.close() for d in DAQ]
-        if self.emul_buttons: 
+        if self.emul_buttons:
             Kb.stop()
-        print('Done')
-        print('Process rate (last iteration): {:.3f}s'.format(self.rate))
+        print("Done")
+        print("Process rate (last iteration): {:.3f}s".format(self.rate))
```

### Comparing `PyNIExp-0.27.3/pyniexp/stimulation.py` & `pyniexp-0.28.post3/src/pyniexp/stimulator/stimulation.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,14 +1,15 @@
 import nidaqmx, serial, json, sys
 from numpy import concatenate, vstack, arange, linspace, cos, pi, ones
 from nidaqmx.stream_writers import AnalogMultiChannelWriter
 import matplotlib.pyplot as plt
-from loguru import logger
 from time import sleep
-from pyniexp.utils import Status
+from ..utils import Status, getLogger
+
+logger = getLogger()
 
 class Waveform:
     SCALING = 2 # actual intensity (peak to trough) = amplitude * 2
 
     def __init__(self,amplitude = 1, frequency = 10, phase=0, duration = 20, rampUp = 4, rampDown = 4, samplingRate = 1000):
         
         self.amplitude = amplitude/self.SCALING 
@@ -49,15 +50,15 @@
         ax.plot(arange(0,self.duration,1/self.samplingRate) , self.signal, label='Waveform')
         ax.set(xlabel='time [s]', ylabel='intensity [mA]')
         ax.grid()
         ax.legend()
 
         plt.show()
 
-class Stimulator:
+class TES:
     isDAQ = False
     _DAQ = None
 
     @property
     def nChannels(self):
         if self.isDAQ:
             return len(self.__config['Channels'])
```

### Comparing `PyNIExp-0.27.3/pyniexp/stimulatordlg.py` & `pyniexp-0.28.post3/src/pyniexp/stimulator/stimulatordlg.py`

 * *Files 9% similar despite different names*

```diff
@@ -1,54 +1,58 @@
-import os, sys
-from multiprocessing import Process
-from time import time, sleep
-
-import pyniexp
-from pyniexp.stimulation import Waveform, Stimulator
-from pyniexp.utils import Status
+from importlib.resources import files
+from os.path import exists
+from time import time
+
+from .stimulation import Waveform, TES
+from ..utils import Status
 
 from numpy import arange, zeros
 
-from PyQt5.uic import loadUi
-from PyQt5.QtWidgets import QApplication, QWidget, QFileDialog
-from PyQt5.QtCore import Qt, QTimer
+from PyQt6.uic import loadUi
+from PyQt6.QtWidgets import QWidget, QFileDialog
+from PyQt6.QtCore import Qt, QTimer
 import pyqtgraph as pg
 
+
 class StimulatorApp(QWidget):
     _stimulator = None
     _t0 = None
     _timer = None
     _plot = [None, None]
     _waves = [None, None]
 
     def __init__(self):
-        super().__init__(parent=None, flags=Qt.Window)
-        loadUi(os.path.join(list(pyniexp.__path__)[0],'stimulatordlg.ui'), self)    
+        super().__init__(parent=None, flags=Qt.WindowType.Window)
+        loadUi(files(__package__).joinpath("stimulatordlg.ui"), self)
 
         configFile = None
-        if os.path.exists('config_stimulation.json'):
-            configFile = 'config_stimulation.json'
+        if exists("config_stimulation.json"):
+            configFile = "config_stimulation.json"
         self.loadConfig(configFile)
 
         for i in [0, 1]:
             self._plot[i] = pg.PlotWidget(self)
             self._plot[i].setBackground((255, 255, 255))
-            self.__getattribute__("plChannel{:d}".format(i+1)).addWidget(self._plot[i])
+            self.__getattribute__("plChannel{:d}".format(i + 1)).addWidget(
+                self._plot[i]
+            )
             p = self._plot[i].getPlotItem()
-            p.setLabel('bottom',"Time [s]")
-            p.setLabel('left', "Current [mA]")
+            p.setLabel("bottom", "Time [s]")
+            p.setLabel("left", "Current [mA]")
             p.setMenuEnabled(enableMenu=False)
             p.setMouseEnabled(x=False, y=False)
             p.showGrid(x=True, y=True, alpha=1)
             p.installEventFilter(self)
             p.disableAutoRange(axis=pg.ViewBox.YAxis)
             p.disableAutoRange(axis=pg.ViewBox.XAxis)
-            p.plot(x=arange(0,1,1/1000),
+            p.plot(
+                x=arange(0, 1, 1 / 1000),
                 y=zeros(1000),
-                pen=pg.mkPen(color='r', width=2))
+                pen=pg.mkPen(color="r", width=2),
+            )
 
         self.cbStimType.currentTextChanged.connect(self.updateDlg)
 
         self.sbIntensity1.valueChanged.connect(self.updatePlots)
         self.sbIntensity2.valueChanged.connect(self.updatePlots)
         self.sbFrequency1.valueChanged.connect(self.updatePlots)
         self.sbFrequency2.valueChanged.connect(self.updatePlots)
@@ -59,38 +63,40 @@
         self.sbRampDown.valueChanged.connect(self.updatePlots)
         self.sbSamplingRate.valueChanged.connect(self.updatePlots)
 
         self.btnLoadConfig.clicked.connect(lambda: self.loadConfig(None))
         self.btnLoadWaves.clicked.connect(self.loadWaves)
         self.btnRun.clicked.connect(self.run)
         self.btnStop.clicked.connect(self.stop)
-        
+
         self._timer = QTimer(self)
         self._timer.timeout.connect(self.updateOnTimer)
 
         self.updateDlg()
         self.updatePlots()
 
         self.setWindowTitle("Stimulator")
         self.show()
 
     def closeEvent(self, event):
         self.hide()
         self._stimulator = None
 
-    def loadConfig(self,configFile=None):
+    def loadConfig(self, configFile=None):
         if configFile is None:
             configFile = QFileDialog.getOpenFileName(
-                    caption="Select 'Configuration JSON file'", filter='ini files (*.json)')[0]
+                caption="Select 'Configuration JSON file'", filter="ini files (*.json)"
+            )[0]
         if len(configFile) == 0:
-                return
+            return
         self._stimulator = None
-        self._stimulator = Stimulator(configFile)
+        self._stimulator = TES(configFile)
         self.lblStatus.setText(self._stimulator.status.name)
-        if self._stimulator.status.value > 0: self.btnLoadWaves.setEnabled(True)
+        if self._stimulator.status.value > 0:
+            self.btnLoadWaves.setEnabled(True)
 
     def loadWaves(self):
         self._stimulator.loadWaveform(self._waves)
         self.btnRun.setEnabled(True)
         self.progressBar.setValue(0)
         self.lblStatus.setText(self._stimulator.status.name)
 
@@ -106,48 +112,74 @@
         self.btnRun.setEnabled(False)
         self.btnStop.setEnabled(False)
         self._timer.stop()
         self.progressBar.setValue(0)
         self.lblStatus.setText(self._stimulator.status.name)
 
     def updateDlg(self):
-        if self.cbStimType.currentText() == 'Dual-channel':
+        if self.cbStimType.currentText() == "Dual-channel":
             chs = [True, True]
         else:
             chs = [False, False]
-            chs[int(self.cbStimType.currentText()[-1:])-1] = True
+            chs[int(self.cbStimType.currentText()[-1:]) - 1] = True
         self.setChannel(chs)
 
     def updatePlots(self):
-        self._waves[0] = Waveform(amplitude = self.sbIntensity1.value(), frequency = self.sbFrequency1.value(), phase=self.sbPhase1.value(), 
-            duration = self.sbDuration.value(), rampUp = self.sbRampUp.value(), rampDown = self.sbRampDown.value(), 
-            samplingRate = self.sbSamplingRate.value())
-        self._waves[1] = Waveform(amplitude = self.sbIntensity2.value(), frequency = self.sbFrequency2.value(), phase=self.sbPhase2.value(), 
-            duration = self.sbDuration.value(), rampUp = self.sbRampUp.value(), rampDown = self.sbRampDown.value(), 
-            samplingRate = self.sbSamplingRate.value())
-
-        for i in [0,1]:
-            self._plot[i].getPlotItem().dataItems[0].setData(arange(0,self._waves[i].duration,1/self._waves[i].samplingRate),
-                self._waves[i].signal)
-            self._plot[i].getPlotItem().setXRange(0, self._waves[i].duration, padding=0.0)
-            self._plot[i].getPlotItem().setYRange(-self._waves[i].amplitude*2, self._waves[i].amplitude*2, padding=0.0)
+        self._waves[0] = Waveform(
+            amplitude=self.sbIntensity1.value(),
+            frequency=self.sbFrequency1.value(),
+            phase=self.sbPhase1.value(),
+            duration=self.sbDuration.value(),
+            rampUp=self.sbRampUp.value(),
+            rampDown=self.sbRampDown.value(),
+            samplingRate=self.sbSamplingRate.value(),
+        )
+        self._waves[1] = Waveform(
+            amplitude=self.sbIntensity2.value(),
+            frequency=self.sbFrequency2.value(),
+            phase=self.sbPhase2.value(),
+            duration=self.sbDuration.value(),
+            rampUp=self.sbRampUp.value(),
+            rampDown=self.sbRampDown.value(),
+            samplingRate=self.sbSamplingRate.value(),
+        )
+
+        for i in [0, 1]:
+            self._plot[i].getPlotItem().dataItems[0].setData(
+                arange(0, self._waves[i].duration, 1 / self._waves[i].samplingRate),
+                self._waves[i].signal,
+            )
+            self._plot[i].getPlotItem().setXRange(
+                0, self._waves[i].duration, padding=0.0
+            )
+            self._plot[i].getPlotItem().setYRange(
+                -self._waves[i].amplitude * 2, self._waves[i].amplitude * 2, padding=0.0
+            )
+
+        self.progressBar.setMaximum(self._waves[0].duration * 1000)
 
-        self.progressBar.setMaximum(self._waves[0].duration*1000)
-        
     def updateOnTimer(self):
         TOL = 10
-        self.progressBar.setValue(int((time()-self._t0)*1000))
+        self.progressBar.setValue(int((time() - self._t0) * 1000))
         if self._stimulator.status == Status.STOPPED:
             self.btnStop.setEnabled(False)
             self._timer.stop()
             self.progressBar.setValue(0)
         self.lblStatus.setText(self._stimulator.status.name)
 
-    def setChannel(self,isVisible=[0,0]):
+    def setChannel(self, isVisible=[0, 0]):
         for i in range(len(isVisible)):
             self._plot[i].setVisible(isVisible[i])
-            self.__getattribute__("lblFrequency{:d}".format(i+1)).setVisible(isVisible[i])
-            self.__getattribute__("sbFrequency{:d}".format(i+1)).setVisible(isVisible[i])
-            self.__getattribute__("lblPhase{:d}".format(i+1)).setVisible(isVisible[i])
-            self.__getattribute__("sbPhase{:d}".format(i+1)).setVisible(isVisible[i])
-            self.__getattribute__("lblIntensity{:d}".format(i+1)).setVisible(isVisible[i])
-            self.__getattribute__("sbIntensity{:d}".format(i+1)).setVisible(isVisible[i])
+            self.__getattribute__("lblFrequency{:d}".format(i + 1)).setVisible(
+                isVisible[i]
+            )
+            self.__getattribute__("sbFrequency{:d}".format(i + 1)).setVisible(
+                isVisible[i]
+            )
+            self.__getattribute__("lblPhase{:d}".format(i + 1)).setVisible(isVisible[i])
+            self.__getattribute__("sbPhase{:d}".format(i + 1)).setVisible(isVisible[i])
+            self.__getattribute__("lblIntensity{:d}".format(i + 1)).setVisible(
+                isVisible[i]
+            )
+            self.__getattribute__("sbIntensity{:d}".format(i + 1)).setVisible(
+                isVisible[i]
+            )
```

### Comparing `PyNIExp-0.27.3/pyniexp/stimulatordlg.ui` & `pyniexp-0.28.post3/src/pyniexp/stimulator/stimulatordlg.ui`

 * *Files identical despite different names*

### Comparing `PyNIExp-0.27.3/pyniexp/triggers.py` & `pyniexp-0.28.post3/src/pyniexp/scanner/triggers.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,11 @@
 import serial
-from pyniexp.utils import listSerial
-from loguru import logger
+from ..utils import getLogger, listSerial
+
+logger = getLogger()
 
 class BrainVision:
     _port = []
     _isConnected = False
 
     def isConnected(self):
         return self._isConnected
```

