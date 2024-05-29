# Comparing `tmp/eltako14bus-0.0.53.tar.gz` & `tmp/eltako14bus-0.0.54.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "eltako14bus-0.0.53.tar", last modified: Fri Apr 19 21:50:25 2024, max compression
+gzip compressed data, was "eltako14bus-0.0.54.tar", last modified: Wed May 29 15:04:02 2024, max compression
```

## Comparing `eltako14bus-0.0.53.tar` & `eltako14bus-0.0.54.tar`

### file list

```diff
@@ -1,26 +1,26 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-19 21:50:25.492021 eltako14bus-0.0.53/
--rw-r--r--   0 runner    (1001) docker     (127)    35149 2024-04-19 21:50:17.000000 eltako14bus-0.0.53/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)     3174 2024-04-19 21:50:25.492021 eltako14bus-0.0.53/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     2412 2024-04-19 21:50:17.000000 eltako14bus-0.0.53/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-19 21:50:25.492021 eltako14bus-0.0.53/eltako14bus.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     3174 2024-04-19 21:50:25.000000 eltako14bus-0.0.53/eltako14bus.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      437 2024-04-19 21:50:25.000000 eltako14bus-0.0.53/eltako14bus.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-19 21:50:25.000000 eltako14bus-0.0.53/eltako14bus.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       91 2024-04-19 21:50:25.000000 eltako14bus-0.0.53/eltako14bus.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       16 2024-04-19 21:50:25.000000 eltako14bus-0.0.53/eltako14bus.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-19 21:50:25.492021 eltako14bus-0.0.53/eltakobus/
--rw-r--r--   0 runner    (1001) docker     (127)      468 2024-04-19 21:50:17.000000 eltako14bus-0.0.53/eltakobus/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     8533 2024-04-19 21:50:17.000000 eltako14bus-0.0.53/eltakobus/bus.py
--rw-r--r--   0 runner    (1001) docker     (127)     1100 2024-04-19 21:50:17.000000 eltako14bus-0.0.53/eltakobus/coap.py
--rw-r--r--   0 runner    (1001) docker     (127)    44511 2024-04-19 21:50:17.000000 eltako14bus-0.0.53/eltakobus/device.py
--rw-r--r--   0 runner    (1001) docker     (127)    43255 2024-04-19 21:50:17.000000 eltako14bus-0.0.53/eltakobus/eep.py
--rw-r--r--   0 runner    (1001) docker     (127)      955 2024-04-19 21:50:17.000000 eltako14bus-0.0.53/eltakobus/error.py
--rw-r--r--   0 runner    (1001) docker     (127)     2769 2024-04-19 21:50:17.000000 eltako14bus-0.0.53/eltakobus/locking.py
--rw-r--r--   0 runner    (1001) docker     (127)    19245 2024-04-19 21:50:17.000000 eltako14bus-0.0.53/eltakobus/message.py
--rw-r--r--   0 runner    (1001) docker     (127)    18067 2024-04-19 21:50:17.000000 eltako14bus-0.0.53/eltakobus/serial.py
--rw-r--r--   0 runner    (1001) docker     (127)     1812 2024-04-19 21:50:17.000000 eltako14bus-0.0.53/eltakobus/util.py
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-19 21:50:25.492021 eltako14bus-0.0.53/setup.cfg
--rwxr-xr-x   0 runner    (1001) docker     (127)     1108 2024-04-19 21:50:17.000000 eltako14bus-0.0.53/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-19 21:50:25.492021 eltako14bus-0.0.53/tests/
--rw-r--r--   0 runner    (1001) docker     (127)      100 2024-04-19 21:50:17.000000 eltako14bus-0.0.53/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1636 2024-04-19 21:50:17.000000 eltako14bus-0.0.53/tests/generic_eep_test.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-29 15:04:02.180960 eltako14bus-0.0.54/
+-rw-r--r--   0 runner    (1001) docker     (127)    35149 2024-05-29 15:03:54.000000 eltako14bus-0.0.54/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)     3174 2024-05-29 15:04:02.180960 eltako14bus-0.0.54/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     2412 2024-05-29 15:03:54.000000 eltako14bus-0.0.54/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-29 15:04:02.180960 eltako14bus-0.0.54/eltako14bus.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     3174 2024-05-29 15:04:02.000000 eltako14bus-0.0.54/eltako14bus.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      437 2024-05-29 15:04:02.000000 eltako14bus-0.0.54/eltako14bus.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-29 15:04:02.000000 eltako14bus-0.0.54/eltako14bus.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       91 2024-05-29 15:04:02.000000 eltako14bus-0.0.54/eltako14bus.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       16 2024-05-29 15:04:02.000000 eltako14bus-0.0.54/eltako14bus.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-29 15:04:02.180960 eltako14bus-0.0.54/eltakobus/
+-rw-r--r--   0 runner    (1001) docker     (127)      468 2024-05-29 15:03:54.000000 eltako14bus-0.0.54/eltakobus/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8533 2024-05-29 15:03:54.000000 eltako14bus-0.0.54/eltakobus/bus.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1100 2024-05-29 15:03:54.000000 eltako14bus-0.0.54/eltakobus/coap.py
+-rw-r--r--   0 runner    (1001) docker     (127)    45303 2024-05-29 15:03:54.000000 eltako14bus-0.0.54/eltakobus/device.py
+-rw-r--r--   0 runner    (1001) docker     (127)    43255 2024-05-29 15:03:54.000000 eltako14bus-0.0.54/eltakobus/eep.py
+-rw-r--r--   0 runner    (1001) docker     (127)      955 2024-05-29 15:03:54.000000 eltako14bus-0.0.54/eltakobus/error.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2769 2024-05-29 15:03:54.000000 eltako14bus-0.0.54/eltakobus/locking.py
+-rw-r--r--   0 runner    (1001) docker     (127)    19245 2024-05-29 15:03:54.000000 eltako14bus-0.0.54/eltakobus/message.py
+-rw-r--r--   0 runner    (1001) docker     (127)    18067 2024-05-29 15:03:54.000000 eltako14bus-0.0.54/eltakobus/serial.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1812 2024-05-29 15:03:54.000000 eltako14bus-0.0.54/eltakobus/util.py
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-29 15:04:02.180960 eltako14bus-0.0.54/setup.cfg
+-rwxr-xr-x   0 runner    (1001) docker     (127)     1108 2024-05-29 15:03:54.000000 eltako14bus-0.0.54/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-29 15:04:02.180960 eltako14bus-0.0.54/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)      100 2024-05-29 15:03:54.000000 eltako14bus-0.0.54/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1636 2024-05-29 15:03:54.000000 eltako14bus-0.0.54/tests/generic_eep_test.py
```

### Comparing `eltako14bus-0.0.53/LICENSE` & `eltako14bus-0.0.54/LICENSE`

 * *Files identical despite different names*

### Comparing `eltako14bus-0.0.53/PKG-INFO` & `eltako14bus-0.0.54/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: eltako14bus
-Version: 0.0.53
+Version: 0.0.54
 Summary: Library for participating in the Eltako Series 14 RS485 bus
 Home-page: https://github.com/grimmpp/eltako14bus
 Author: chrysn, grimmpp
 Author-email: chrysn@fsfe.org, grimmpp14@gmail.com
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: GNU Lesser General Public License v3 or later (LGPLv3+)
 Description-Content-Type: text/markdown
```

### Comparing `eltako14bus-0.0.53/README.md` & `eltako14bus-0.0.54/README.md`

 * *Files identical despite different names*

### Comparing `eltako14bus-0.0.53/eltako14bus.egg-info/PKG-INFO` & `eltako14bus-0.0.54/eltako14bus.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: eltako14bus
-Version: 0.0.53
+Version: 0.0.54
 Summary: Library for participating in the Eltako Series 14 RS485 bus
 Home-page: https://github.com/grimmpp/eltako14bus
 Author: chrysn, grimmpp
 Author-email: chrysn@fsfe.org, grimmpp14@gmail.com
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: GNU Lesser General Public License v3 or later (LGPLv3+)
 Description-Content-Type: text/markdown
```

### Comparing `eltako14bus-0.0.53/eltakobus/bus.py` & `eltako14bus-0.0.54/eltakobus/bus.py`

 * *Files identical despite different names*

### Comparing `eltako14bus-0.0.53/eltakobus/coap.py` & `eltako14bus-0.0.54/eltakobus/coap.py`

 * *Files identical despite different names*

### Comparing `eltako14bus-0.0.53/eltakobus/device.py` & `eltako14bus-0.0.54/eltakobus/device.py`

 * *Files 3% similar despite different names*

```diff
@@ -194,14 +194,15 @@
         self.channel = channel
         self.in_func_group = in_func_group
         self.memory_line = memory_line
     
 
 class BusObject:
     sensor_address_range = None
+    discovery_names = []
 
     def __init__(self, response: EltakoDiscoveryReply, *, bus=None):
         super().__init__()
 
         self.discovery_response = response
         if self.discovery_response.reported_size != self.size:
             # won't happen with the default size implementation, but another class may give a constant here
@@ -302,15 +303,15 @@
     async def get_all_sensors(self) -> list[SensorInfo]:
         return []
         # return await self.get_registered_sensors(self.sensor_address_range)
 
 
 class FAM14(BusObject):
     size = 1
-    discovery_name = bytes((0x07, 0xff))
+    discovery_names = [ bytes((0x07, 0xff)), bytes((0x08, 0xff)) ]
     sensor_address_range = range(0,0)
 
     @classmethod
     def annotate_memory(cls, mem):
         return {
             1: MemoryFileNibbleExplanationComment(
                     "AD DR ES S, -- -- -- --",
@@ -329,15 +330,14 @@
 
     async def get_base_id_in_int(self) -> int:
         """Gets base id from FAM14 memory."""
         mem_line = await self.read_mem_line(1)
         return int.from_bytes(mem_line[0:4], "big") 
 
 
-
 class DimmerStyle(BusObject):
     """Devices that work just the same as a FUD14. FSG14_1_10V appears to
     behave the same way in the known areas as that -- all GUIs options in the
     PCT tool even look the same."""
 
     def __init__(self, *args, **kwargs):
         super().__init__(*args, **kwargs)
@@ -476,15 +476,15 @@
                          "AD DR ES S, KY FN SP %%",
                          "key (5 = left, 6 = right), function (eg. 32 = A5-38-08), speed, percent"),
                     ],
                 }
 
 class FUD14(DimmerStyle):
     size = 1
-    discovery_name = bytes((0x04, 0x04))
+    discovery_names = [ bytes((0x04, 0x04)) ]
     has_subchannels = False
     sensor_address_range = range(8, 127)
     range_func_group_1 = range(8,9)
     range_func_group_2 = range(9,12)
     range_func_group_3 = range(12,127)
 
     def __init__(self, *args, **kwargs):
@@ -497,15 +497,15 @@
         result.extend( await self.get_registered_sensors(self.range_func_group_1, 1 ))
         result.extend( await self.get_registered_sensors(self.range_func_group_2, 2 ))
         result.extend( await self.get_registered_sensors(self.range_func_group_3, 3 ))
         return result
 
 class FUD14_800W(FUD14):
     size = 1
-    discovery_name = bytes((0x04, 0x05))
+    discovery_names = [ bytes((0x04, 0x05)) ]
     has_subchannels = False
 
     def __init__(self, *args, **kwargs):
         super().__init__(*args, **kwargs)
         self.programmable_dimmer = (12, self.memory_size)
         self.gfvs_code = KeyFunction.DIMMING_VALUE_FROM_CONTROLLER
 
@@ -693,32 +693,32 @@
     async def get_all_sensors(self) -> list[SensorInfo]:
         result = []
         result.extend( await self.get_registered_sensors(self.sensors_func_group_1, 1) )
         result.extend( await self.get_registered_sensors(self.sensors_func_group_2, 2) )
         return result
 
 class FSR14_1x(FSR14):
-    discovery_name = bytes((0x04, 0x01))
+    discovery_names = [ bytes((0x04, 0x01)) ]
     size = 1
 
 class FSR14_2x(FSR14):
-    discovery_name = bytes((0x04, 0x02))
+    discovery_names = [ bytes((0x04, 0x02)) ]
     size = 2
 
 class FSR14_4x(FSR14):
-    discovery_name = bytes((0x04, 0x01))
+    discovery_names = [ bytes((0x04, 0x01)) ]
     size = 4
 
 class F4SR14_LED(FSR14):
-    discovery_name = bytes((0x04, 0x09))
+    discovery_names = [ bytes((0x04, 0x09)) ]
     size = 4
 
 class FSB14(BusObject, HasProgrammableRPS):
     size = 2
-    discovery_name = bytes((0x04, 0x06))
+    discovery_names = [ bytes((0x04, 0x06)) ]
     sensor_address_range = range(17, 127)
     range_func_group_1 = range(16,17)
     range_func_group_2 = range(17,127)
 
     def __init__(self, *args, **kwargs):
         super().__init__(*args, **kwargs)
         self.programmable_rps = (17, self.memory_size)
@@ -801,53 +801,53 @@
     async def get_all_sensors(self) -> list[SensorInfo]:
         result = []
         result.extend( await self.get_registered_sensors(self.range_func_group_1, 1) )
         result.extend( await self.get_registered_sensors(self.range_func_group_2, 2) )
         return result
 
 class F3Z14D(BusObject):
-    discovery_name = bytes((0x04, 0x67))
+    discovery_names = [ bytes((0x04, 0x67)) ]
     size = 3
 
 class FMZ14(BusObject, HasProgrammableRPS):
-    discovery_name = bytes((0x04, 0x0e))
+    discovery_names = [ bytes((0x04, 0x0e)) ]
     size = 1
     sensor_address_range = range(8, 8+47)
 
     def __init__(self, *args, **kwargs):
         super().__init__(*args, **kwargs)
         self.programmable_rps = (8, self.memory_size)
         self.gfvs_code = KeyFunction.SWITCHING_STATE_FROM_CONTROLLER
 
     async def get_all_sensors(self) -> list[SensorInfo]:
         return await self.get_registered_sensors(self.sensor_address_range, 1)
 
 class FWG14MS(BusObject):
-    discovery_name = bytes((0x04, 0x1a))
+    discovery_names = [ bytes((0x04, 0x1a)) ]
     size = 1
 
 class FSU14(BusObject):
-    discovery_name = bytes((0x07, 0x14))
+    discovery_names = [ bytes((0x07, 0x14)) ]
     size = 8
     async def show_off(self):
         await super().show_off()
 
         hour = random.randint(0, 23)
         minutes = random.randint(0, 59)
         print("Setting clock to %02d:%02d"%(hour, minutes))
         await self.write_mem_line(0x5d, b"\x16\x01\x01\x08" + bytes((((hour // 10) << 4) + (hour % 10), ((minutes // 10) << 4) + (minutes % 10))) + b"\x00\x01")
 
         await asyncio.sleep(3)
 
 class FMSR14(BusObject):
-    discovery_name = bytes((0x05, 0x15))
+    discovery_names = [ bytes((0x05, 0x15)) ]
     size = 5
 
 class FWZ14_65A(BusObject):
-    discovery_name = bytes((0x04, 0x66))
+    discovery_names = [ bytes((0x04, 0x66)) ]
     size = 1
 
     @classmethod
     def annotate_memory(cls, mem):
         return {
                 1: MemoryFileNibbleExplanationComment(".. .. .. .. ..  SUM kWh", "accumulated counter value as sent in DT=0 DIV=0 telegram"),
                 5: MemoryFileNibbleExplanationComment("S0 S1 S2 S3 .. .. .. ..", "Serial number as sent in DT=1 DIV=3 TI=8 messages (once as with DB3..1 = S1 S0 00, once as S3 S2 01)")
@@ -870,29 +870,29 @@
             # Device is sending its serial number, which is better obtained
             # from memory
             return {}
 
         return A5_12_01.decode(msg.data)
 
 class FSG14_1_10V(DimmerStyle):
-    discovery_name = bytes((0x04, 0x07))
+    discovery_names = [ bytes((0x04, 0x07)) ]
     size = 1
     has_subchannels = False
 
     def __init__(self, *args, **kwargs):
         super().__init__(*args, **kwargs)
         self.programmable_rps = (12, self.memory_size)
         self.gfvs_code = 32
 
 class FGW14_USB(BusObject):
-    discovery_name = bytes((0x04, 0xfe))
+    discovery_names = [ bytes((0x04, 0xfe)) ]
     size = 1
 
 class FDG14(DimmerStyle):
-    discovery_name = bytes((0x04, 0x34))
+    discovery_names = [ bytes((0x04, 0x34)) ]
     size = 16
     has_subchannels = True
 
     def __init__(self, *args, **kwargs):
         super().__init__(*args, **kwargs)
         self.programmable_dimmer = (14, self.memory_size)
         self.gfvs_code = 32
@@ -921,18 +921,17 @@
                     MemoryFileStartOfSectionComment("function group 1"),
                     MemoryFileNibbleExplanationComment(
                          "AD DR ES S, KY FN CH V ",
                          "key (5 = left, 6 = right), function (eg. 32 = A5-38-08), ch = channel (0x10 = broadcast), v = value (e.g. dimming in percentage, brightness)"),
                     ],
                 }
     
-
 class FAE14SSR(BusObject, HasProgrammableRPS):
     size = 2
-    discovery_name = bytes((0x04, 0x16))
+    discovery_names = [ bytes((0x04, 0x16)) ]
     thermostat_address_range = range(8,10)
     temp_sensor_range = range(10,12)
     smart_home_controller_address_range = range(12,14)
     sensor_address_range = range(14, 127)
 
     def __init__(self, *args, **kwargs):
         super().__init__(*args, **kwargs)
@@ -947,41 +946,57 @@
                 4: MemoryFileNibbleExplanationComment(
                     "-- RV -- -- -- -- -- --",
                     "RV = return value, 1. bit channel 1 & 2. bit channel 2 "),
                 5: MemoryFileNibbleExplanationComment(
                     "-- -- -- -- dt dt -- --", "temp offset channel 1 & 2"),
                 7: MemoryFileNibbleExplanationComment(
                     "a  a  hc tp hc tp  tt tt", ""),
-                8: MemoryFileStartOfSectionComment("function group 1 / Temp Controller"),
-                10: MemoryFileStartOfSectionComment("function group 2 / Temp Sensor"),
-                12: MemoryFileStartOfSectionComment("function group 3 / Smart Home SW"),
-                14: MemoryFileStartOfSectionComment("function group 3 / switches, contacts, ..."),
+                cls.thermostat_address_range[0]: MemoryFileStartOfSectionComment("function group 1 / Temp Controller"),
+                cls.temp_sensor_range[0]: MemoryFileStartOfSectionComment("function group 2 / Temp Sensor"),
+                cls.smart_home_controller_address_range[0]: MemoryFileStartOfSectionComment("function group 3 / Smart Home SW"),
+                cls.sensor_address_range[0]: MemoryFileStartOfSectionComment("function group 3 / switches, contacts, ..."),
                 }
     
     async def get_all_sensors(self) -> list[SensorInfo]:
         result = []
         result.extend( await self.get_registered_sensors(self.thermostat_address_range, 1 ))
         result.extend( await self.get_registered_sensors(self.temp_sensor_range, 2 ))
         result.extend( await self.get_registered_sensors(self.smart_home_controller_address_range, 3 ))
         result.extend( await self.get_registered_sensors(self.sensor_address_range, 4 ))
         return result
 
+class FHK14(FAE14SSR):
+    size=2
+    discovery_names = [ bytes((0x04, 0x18)) ]
+
+    def __init__(self, *args, **kwargs):
+        super().__init__(*args, **kwargs)
 
+class F4HK14(FHK14, HasProgrammableRPS):
+    size = 4
+    discovery_names = [ bytes((0x04, 0x18)) ]
+    thermostat_address_range = range(8,12)
+    temp_sensor_range = range(12,16)
+    smart_home_controller_address_range = range(16,20)
+    sensor_address_range = range(20, 127)
+
+    def __init__(self, *args, **kwargs):
+        super().__init__(*args, **kwargs)
 
-known_objects = [FAM14, FUD14, FUD14_800W, FSB14, FSR14_1x, FSR14_2x, FSR14_4x, F4SR14_LED, F3Z14D, FMZ14, FWG14MS, FSU14, FMSR14, FWZ14_65A, FSG14_1_10V, FGW14_USB, FDG14, FAE14SSR]
+known_objects = [FAM14, FUD14, FUD14_800W, FSB14, FSR14_1x, FSR14_2x, FSR14_4x, F4SR14_LED, F3Z14D, FMZ14, FWG14MS, FSU14, FMSR14, FWZ14_65A, FSG14_1_10V, FGW14_USB, FDG14, FHK14, F4HK14, FAE14SSR]
 # sorted so the first match of (discovery name is a prefix, size matches) can be used
-sorted_known_objects = sorted(known_objects, key=lambda o: len(o.discovery_name) + 0.5 * (o.size is not None), reverse=True)
+sorted_known_objects = sorted(known_objects, key=lambda o: len(o.discovery_names[0]) + 0.5 * (o.size is not None), reverse=True)
 
 async def create_busobject(bus, id):
     response = await bus.exchange(EltakoDiscoveryRequest(address=id), EltakoDiscoveryReply)
 
     assert id == response.reported_address, "Queried for ID %s, received %s" % (id, prettify(response))
 
     for o in sorted_known_objects:
-        if response.model.startswith(o.discovery_name) and (o.size is None or o.size == response.reported_size):
+        if response.model[0:2] in o.discovery_names and (o.size is None or o.size == response.reported_size):
             return o(response, bus=bus)
     else:
         return BusObject(response, bus=bus)
 
     
 
 class MemoryFile(defaultdict):
```

### Comparing `eltako14bus-0.0.53/eltakobus/eep.py` & `eltako14bus-0.0.54/eltakobus/eep.py`

 * *Files identical despite different names*

### Comparing `eltako14bus-0.0.53/eltakobus/error.py` & `eltako14bus-0.0.54/eltakobus/error.py`

 * *Files identical despite different names*

### Comparing `eltako14bus-0.0.53/eltakobus/locking.py` & `eltako14bus-0.0.54/eltakobus/locking.py`

 * *Files identical despite different names*

### Comparing `eltako14bus-0.0.53/eltakobus/message.py` & `eltako14bus-0.0.54/eltakobus/message.py`

 * *Files identical despite different names*

### Comparing `eltako14bus-0.0.53/eltakobus/serial.py` & `eltako14bus-0.0.54/eltakobus/serial.py`

 * *Files identical despite different names*

### Comparing `eltako14bus-0.0.53/eltakobus/util.py` & `eltako14bus-0.0.54/eltakobus/util.py`

 * *Files identical despite different names*

### Comparing `eltako14bus-0.0.53/setup.py` & `eltako14bus-0.0.54/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -9,15 +9,15 @@
 }
 
 with open("README.md", "r") as fh:
     long_description = fh.read()
 
 setuptools.setup(
     name="eltako14bus",
-    version="0.0.53",
+    version="0.0.54",
     author="chrysn, grimmpp",
     author_email="chrysn@fsfe.org, grimmpp14@gmail.com",
     description="Library for participating in the Eltako Series 14 RS485 bus",
     url="https://github.com/grimmpp/eltako14bus",
     packages=setuptools.find_packages(),
     extras_require=extras_require,
     # Not that there'd be tests, but at least it fetches the right dependencies and syntax checks everything
```

### Comparing `eltako14bus-0.0.53/tests/generic_eep_test.py` & `eltako14bus-0.0.54/tests/generic_eep_test.py`

 * *Files identical despite different names*

