# Comparing `tmp/pyiskra-1.0.0.tar.gz` & `tmp/pyiskra-1.0.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pyiskra-1.0.0.tar", last modified: Mon May 27 12:12:24 2024, max compression
+gzip compressed data, was "pyiskra-1.0.1.tar", last modified: Wed May 29 06:04:08 2024, max compression
```

## Comparing `pyiskra-1.0.0.tar` & `pyiskra-1.0.1.tar`

### file list

```diff
@@ -1,17 +1,17 @@
-drwxrwxrwx   0        0        0        0 2024-05-27 12:12:24.347282 pyiskra-1.0.0/
--rw-rw-rw-   0        0        0     3117 2024-05-27 12:12:24.335858 pyiskra-1.0.0/PKG-INFO
--rw-rw-rw-   0        0        0     2380 2024-02-20 10:46:59.000000 pyiskra-1.0.0/README.md
-drwxrwxrwx   0        0        0        0 2024-05-27 12:12:24.298632 pyiskra-1.0.0/pyiskra/
--rw-rw-rw-   0        0        0        0 2024-02-16 07:27:58.000000 pyiskra-1.0.0/pyiskra/__init__.py
--rw-rw-rw-   0        0        0     5356 2024-05-27 09:59:36.000000 pyiskra-1.0.0/pyiskra/discovery.py
--rw-rw-rw-   0        0        0      253 2024-02-21 10:19:06.000000 pyiskra-1.0.0/pyiskra/exceptions.py
--rw-rw-rw-   0        0        0     3659 2024-02-21 11:40:58.000000 pyiskra-1.0.0/pyiskra/helper.py
-drwxrwxrwx   0        0        0        0 2024-05-27 12:12:24.335858 pyiskra-1.0.0/pyiskra.egg-info/
--rw-rw-rw-   0        0        0     3117 2024-05-27 12:12:24.000000 pyiskra-1.0.0/pyiskra.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      268 2024-05-27 12:12:24.000000 pyiskra-1.0.0/pyiskra.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-05-27 12:12:24.000000 pyiskra-1.0.0/pyiskra.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       27 2024-05-27 12:12:24.000000 pyiskra-1.0.0/pyiskra.egg-info/requires.txt
--rw-rw-rw-   0        0        0        8 2024-05-27 12:12:24.000000 pyiskra-1.0.0/pyiskra.egg-info/top_level.txt
--rw-rw-rw-   0        0        0      873 2024-05-27 12:00:27.000000 pyiskra-1.0.0/pyproject.toml
--rw-rw-rw-   0        0        0       42 2024-05-27 12:12:24.347282 pyiskra-1.0.0/setup.cfg
--rw-rw-rw-   0        0        0     1018 2024-05-27 12:00:38.000000 pyiskra-1.0.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-29 06:04:08.886002 pyiskra-1.0.1/
+-rw-r--r--   0 runner    (1001) docker     (127)     3016 2024-05-29 06:04:08.886002 pyiskra-1.0.1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     2300 2024-05-29 06:03:55.000000 pyiskra-1.0.1/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-29 06:04:08.882002 pyiskra-1.0.1/pyiskra/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-29 06:03:55.000000 pyiskra-1.0.1/pyiskra/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5424 2024-05-29 06:03:55.000000 pyiskra-1.0.1/pyiskra/discovery.py
+-rw-r--r--   0 runner    (1001) docker     (127)      236 2024-05-29 06:03:55.000000 pyiskra-1.0.1/pyiskra/exceptions.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3511 2024-05-29 06:03:55.000000 pyiskra-1.0.1/pyiskra/helper.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-29 06:04:08.886002 pyiskra-1.0.1/pyiskra.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     3016 2024-05-29 06:04:08.000000 pyiskra-1.0.1/pyiskra.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      268 2024-05-29 06:04:08.000000 pyiskra-1.0.1/pyiskra.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-29 06:04:08.000000 pyiskra-1.0.1/pyiskra.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       27 2024-05-29 06:04:08.000000 pyiskra-1.0.1/pyiskra.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        8 2024-05-29 06:04:08.000000 pyiskra-1.0.1/pyiskra.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      845 2024-05-29 06:03:55.000000 pyiskra-1.0.1/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-29 06:04:08.886002 pyiskra-1.0.1/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)      988 2024-05-29 06:03:55.000000 pyiskra-1.0.1/setup.py
```

### Comparing `pyiskra-1.0.0/PKG-INFO` & `pyiskra-1.0.1/PKG-INFO`

 * *Files 16% similar despite different names*

```diff
@@ -1,101 +1,101 @@
-Metadata-Version: 2.1
-Name: pyiskra
-Version: 1.0.0
-Summary: Python Iskra devices interface
-Home-page: https://github.com/Iskramis/pyiskra
-Author: Iskra d.o.o.
-Author-email: razvoj.mis@iskra.eu
-Maintainer: Iskra <razvoj.mis@iskra.eu>
-License: GPL
-Keywords: homeautomation,iskra,energy meter
-Classifier: Programming Language :: Python :: 3
-Classifier: License :: OSI Approved :: GNU General Public License v3 (GPLv3)
-Classifier: Operating System :: OS Independent
-Classifier: Topic :: Software Development :: Libraries :: Application Frameworks
-Classifier: Topic :: Home Automation
-Requires-Python: >=3.8
-Description-Content-Type: text/markdown
-Requires-Dist: netifaces
-Requires-Dist: aiohttp
-Requires-Dist: pymodbus
-
-# PyIskra
-
-PyIskra is a Python package designed to provide interface for Iskra devices using SG and it's RestAPI or ModbusTCP/RTU.
-
-## Installation
-
-You can install PyIskra using pip:
-
-```bash
-pip install pyiskra
-```
-
-## Features
-
-- Object-oriented mapping for energy meters
-- Access to measurements
-- Access to Energy counters
-
-## Supported devices
-
-- Smart Gateway
-- IE38
-- IE14
-- MCXXX
-- iMCXXX
-- MTXXX
-- iMTXXX
-
-
-## Usage
-
-Here's a basic example of how to use PyIskra:
-
-```
-import asyncio
-from pyiskra.devices import Device
-from pyiskra.adapters import RestAPI
-
-
-device_ip = "192.168.1.1"
-device_auth = {"username": "admin", "password": "iskra"}
-
-async def main():
-    # Set device IP address
-
-    # Create adapter
-    adapter = RestAPI(ip_address=device_ip, authentication=device_auth)
-
-    # Create device
-    device = await Device.create_device(adapter)
-
-    # Initalize device
-    await device.init()
-
-    devices = [device]
-
-
-    if device.is_gateway:
-        devices += device.get_child_devices()
-
-
-    for device in devices:
-        # Update device status
-        print(f"Updating status for {device.model} {device.serial}")
-        await device.update_status()
-
-        if device.supports_measurements:
-            for index, phase in enumerate(device.measurements.phases):
-                print(f"Phase {index+1} - U: {phase.voltage.value} {phase.voltage.units}, I: {phase.current.value} {phase.current.units} P: {phase.active_power.value} {phase.active_power.units} Q: {phase.reactive_power.value} {phase.reactive_power.units} S: {phase.apparent_power.value} {phase.apparent_power.units} PF: {phase.power_factor.value} {phase.power_factor.units} PA: {phase.power_angle.value} {phase.power_angle.units} THD U: {phase.thd_voltage.value} {phase.thd_voltage.units} THD I: {phase.thd_current.value} {phase.thd_current.units}")
-
-        if device.supports_counters:
-            for counter in device.counters.non_resettable :
-                print(f"Non-resettable counter - Name: {counter.name}, Value: {counter.value} {counter.units}, Direction: {counter.direction}")
-
-
-            for counter in device.counters.resettable:
-                print(f"Resettable counter - Name: {counter.name}, Value: {counter.value} {counter.units}, Direction: {counter.direction}")
-
-asyncio.run(main())
-```
+Metadata-Version: 2.1
+Name: pyiskra
+Version: 1.0.1
+Summary: Python Iskra devices interface
+Home-page: https://github.com/Iskramis/pyiskra
+Author: Iskra d.o.o.
+Author-email: razvoj.mis@iskra.eu
+Maintainer: Iskra <razvoj.mis@iskra.eu>
+License: GPL
+Keywords: homeautomation,iskra,energy meter
+Classifier: Programming Language :: Python :: 3
+Classifier: License :: OSI Approved :: GNU General Public License v3 (GPLv3)
+Classifier: Operating System :: OS Independent
+Classifier: Topic :: Software Development :: Libraries :: Application Frameworks
+Classifier: Topic :: Home Automation
+Requires-Python: >=3.8
+Description-Content-Type: text/markdown
+Requires-Dist: netifaces
+Requires-Dist: aiohttp
+Requires-Dist: pymodbus
+
+# PyIskra
+
+PyIskra is a Python package designed to provide interface for Iskra devices using SG and it's RestAPI or ModbusTCP/RTU.
+
+## Installation
+
+You can install PyIskra using pip:
+
+```bash
+pip install pyiskra
+```
+
+## Features
+
+- Object-oriented mapping for energy meters
+- Access to measurements
+- Access to Energy counters
+
+## Supported devices
+
+- Smart Gateway
+- IE38
+- IE14
+- MCXXX
+- iMCXXX
+- MTXXX
+- iMTXXX
+
+
+## Usage
+
+Here's a basic example of how to use PyIskra:
+
+```
+import asyncio
+from pyiskra.devices import Device
+from pyiskra.adapters import RestAPI
+
+
+device_ip = "192.168.1.1"
+device_auth = {"username": "admin", "password": "iskra"}
+
+async def main():
+    # Set device IP address
+
+    # Create adapter
+    adapter = RestAPI(ip_address=device_ip, authentication=device_auth)
+
+    # Create device
+    device = await Device.create_device(adapter)
+
+    # Initalize device
+    await device.init()
+
+    devices = [device]
+
+
+    if device.is_gateway:
+        devices += device.get_child_devices()
+
+
+    for device in devices:
+        # Update device status
+        print(f"Updating status for {device.model} {device.serial}")
+        await device.update_status()
+
+        if device.supports_measurements:
+            for index, phase in enumerate(device.measurements.phases):
+                print(f"Phase {index+1} - U: {phase.voltage.value} {phase.voltage.units}, I: {phase.current.value} {phase.current.units} P: {phase.active_power.value} {phase.active_power.units} Q: {phase.reactive_power.value} {phase.reactive_power.units} S: {phase.apparent_power.value} {phase.apparent_power.units} PF: {phase.power_factor.value} {phase.power_factor.units} PA: {phase.power_angle.value} {phase.power_angle.units} THD U: {phase.thd_voltage.value} {phase.thd_voltage.units} THD I: {phase.thd_current.value} {phase.thd_current.units}")
+
+        if device.supports_counters:
+            for counter in device.counters.non_resettable :
+                print(f"Non-resettable counter - Name: {counter.name}, Value: {counter.value} {counter.units}, Direction: {counter.direction}")
+
+
+            for counter in device.counters.resettable:
+                print(f"Resettable counter - Name: {counter.name}, Value: {counter.value} {counter.units}, Direction: {counter.direction}")
+
+asyncio.run(main())
+```
```

### Comparing `pyiskra-1.0.0/README.md` & `pyiskra-1.0.1/README.md`

 * *Ordering differences only*

 * *Files 14% similar despite different names*

```diff
@@ -1,80 +1,80 @@
-# PyIskra
-
-PyIskra is a Python package designed to provide interface for Iskra devices using SG and it's RestAPI or ModbusTCP/RTU.
-
-## Installation
-
-You can install PyIskra using pip:
-
-```bash
-pip install pyiskra
-```
-
-## Features
-
-- Object-oriented mapping for energy meters
-- Access to measurements
-- Access to Energy counters
-
-## Supported devices
-
-- Smart Gateway
-- IE38
-- IE14
-- MCXXX
-- iMCXXX
-- MTXXX
-- iMTXXX
-
-
-## Usage
-
-Here's a basic example of how to use PyIskra:
-
-```
-import asyncio
-from pyiskra.devices import Device
-from pyiskra.adapters import RestAPI
-
-
-device_ip = "192.168.1.1"
-device_auth = {"username": "admin", "password": "iskra"}
-
-async def main():
-    # Set device IP address
-
-    # Create adapter
-    adapter = RestAPI(ip_address=device_ip, authentication=device_auth)
-
-    # Create device
-    device = await Device.create_device(adapter)
-
-    # Initalize device
-    await device.init()
-
-    devices = [device]
-
-
-    if device.is_gateway:
-        devices += device.get_child_devices()
-
-
-    for device in devices:
-        # Update device status
-        print(f"Updating status for {device.model} {device.serial}")
-        await device.update_status()
-
-        if device.supports_measurements:
-            for index, phase in enumerate(device.measurements.phases):
-                print(f"Phase {index+1} - U: {phase.voltage.value} {phase.voltage.units}, I: {phase.current.value} {phase.current.units} P: {phase.active_power.value} {phase.active_power.units} Q: {phase.reactive_power.value} {phase.reactive_power.units} S: {phase.apparent_power.value} {phase.apparent_power.units} PF: {phase.power_factor.value} {phase.power_factor.units} PA: {phase.power_angle.value} {phase.power_angle.units} THD U: {phase.thd_voltage.value} {phase.thd_voltage.units} THD I: {phase.thd_current.value} {phase.thd_current.units}")
-
-        if device.supports_counters:
-            for counter in device.counters.non_resettable :
-                print(f"Non-resettable counter - Name: {counter.name}, Value: {counter.value} {counter.units}, Direction: {counter.direction}")
-
-
-            for counter in device.counters.resettable:
-                print(f"Resettable counter - Name: {counter.name}, Value: {counter.value} {counter.units}, Direction: {counter.direction}")
-
-asyncio.run(main())
-```
+# PyIskra
+
+PyIskra is a Python package designed to provide interface for Iskra devices using SG and it's RestAPI or ModbusTCP/RTU.
+
+## Installation
+
+You can install PyIskra using pip:
+
+```bash
+pip install pyiskra
+```
+
+## Features
+
+- Object-oriented mapping for energy meters
+- Access to measurements
+- Access to Energy counters
+
+## Supported devices
+
+- Smart Gateway
+- IE38
+- IE14
+- MCXXX
+- iMCXXX
+- MTXXX
+- iMTXXX
+
+
+## Usage
+
+Here's a basic example of how to use PyIskra:
+
+```
+import asyncio
+from pyiskra.devices import Device
+from pyiskra.adapters import RestAPI
+
+
+device_ip = "192.168.1.1"
+device_auth = {"username": "admin", "password": "iskra"}
+
+async def main():
+    # Set device IP address
+
+    # Create adapter
+    adapter = RestAPI(ip_address=device_ip, authentication=device_auth)
+
+    # Create device
+    device = await Device.create_device(adapter)
+
+    # Initalize device
+    await device.init()
+
+    devices = [device]
+
+
+    if device.is_gateway:
+        devices += device.get_child_devices()
+
+
+    for device in devices:
+        # Update device status
+        print(f"Updating status for {device.model} {device.serial}")
+        await device.update_status()
+
+        if device.supports_measurements:
+            for index, phase in enumerate(device.measurements.phases):
+                print(f"Phase {index+1} - U: {phase.voltage.value} {phase.voltage.units}, I: {phase.current.value} {phase.current.units} P: {phase.active_power.value} {phase.active_power.units} Q: {phase.reactive_power.value} {phase.reactive_power.units} S: {phase.apparent_power.value} {phase.apparent_power.units} PF: {phase.power_factor.value} {phase.power_factor.units} PA: {phase.power_angle.value} {phase.power_angle.units} THD U: {phase.thd_voltage.value} {phase.thd_voltage.units} THD I: {phase.thd_current.value} {phase.thd_current.units}")
+
+        if device.supports_counters:
+            for counter in device.counters.non_resettable :
+                print(f"Non-resettable counter - Name: {counter.name}, Value: {counter.value} {counter.units}, Direction: {counter.direction}")
+
+
+            for counter in device.counters.resettable:
+                print(f"Resettable counter - Name: {counter.name}, Value: {counter.value} {counter.units}, Direction: {counter.direction}")
+
+asyncio.run(main())
+```
```

### Comparing `pyiskra-1.0.0/pyiskra.egg-info/PKG-INFO` & `pyiskra-1.0.1/pyiskra.egg-info/PKG-INFO`

 * *Files 16% similar despite different names*

```diff
@@ -1,101 +1,101 @@
-Metadata-Version: 2.1
-Name: pyiskra
-Version: 1.0.0
-Summary: Python Iskra devices interface
-Home-page: https://github.com/Iskramis/pyiskra
-Author: Iskra d.o.o.
-Author-email: razvoj.mis@iskra.eu
-Maintainer: Iskra <razvoj.mis@iskra.eu>
-License: GPL
-Keywords: homeautomation,iskra,energy meter
-Classifier: Programming Language :: Python :: 3
-Classifier: License :: OSI Approved :: GNU General Public License v3 (GPLv3)
-Classifier: Operating System :: OS Independent
-Classifier: Topic :: Software Development :: Libraries :: Application Frameworks
-Classifier: Topic :: Home Automation
-Requires-Python: >=3.8
-Description-Content-Type: text/markdown
-Requires-Dist: netifaces
-Requires-Dist: aiohttp
-Requires-Dist: pymodbus
-
-# PyIskra
-
-PyIskra is a Python package designed to provide interface for Iskra devices using SG and it's RestAPI or ModbusTCP/RTU.
-
-## Installation
-
-You can install PyIskra using pip:
-
-```bash
-pip install pyiskra
-```
-
-## Features
-
-- Object-oriented mapping for energy meters
-- Access to measurements
-- Access to Energy counters
-
-## Supported devices
-
-- Smart Gateway
-- IE38
-- IE14
-- MCXXX
-- iMCXXX
-- MTXXX
-- iMTXXX
-
-
-## Usage
-
-Here's a basic example of how to use PyIskra:
-
-```
-import asyncio
-from pyiskra.devices import Device
-from pyiskra.adapters import RestAPI
-
-
-device_ip = "192.168.1.1"
-device_auth = {"username": "admin", "password": "iskra"}
-
-async def main():
-    # Set device IP address
-
-    # Create adapter
-    adapter = RestAPI(ip_address=device_ip, authentication=device_auth)
-
-    # Create device
-    device = await Device.create_device(adapter)
-
-    # Initalize device
-    await device.init()
-
-    devices = [device]
-
-
-    if device.is_gateway:
-        devices += device.get_child_devices()
-
-
-    for device in devices:
-        # Update device status
-        print(f"Updating status for {device.model} {device.serial}")
-        await device.update_status()
-
-        if device.supports_measurements:
-            for index, phase in enumerate(device.measurements.phases):
-                print(f"Phase {index+1} - U: {phase.voltage.value} {phase.voltage.units}, I: {phase.current.value} {phase.current.units} P: {phase.active_power.value} {phase.active_power.units} Q: {phase.reactive_power.value} {phase.reactive_power.units} S: {phase.apparent_power.value} {phase.apparent_power.units} PF: {phase.power_factor.value} {phase.power_factor.units} PA: {phase.power_angle.value} {phase.power_angle.units} THD U: {phase.thd_voltage.value} {phase.thd_voltage.units} THD I: {phase.thd_current.value} {phase.thd_current.units}")
-
-        if device.supports_counters:
-            for counter in device.counters.non_resettable :
-                print(f"Non-resettable counter - Name: {counter.name}, Value: {counter.value} {counter.units}, Direction: {counter.direction}")
-
-
-            for counter in device.counters.resettable:
-                print(f"Resettable counter - Name: {counter.name}, Value: {counter.value} {counter.units}, Direction: {counter.direction}")
-
-asyncio.run(main())
-```
+Metadata-Version: 2.1
+Name: pyiskra
+Version: 1.0.1
+Summary: Python Iskra devices interface
+Home-page: https://github.com/Iskramis/pyiskra
+Author: Iskra d.o.o.
+Author-email: razvoj.mis@iskra.eu
+Maintainer: Iskra <razvoj.mis@iskra.eu>
+License: GPL
+Keywords: homeautomation,iskra,energy meter
+Classifier: Programming Language :: Python :: 3
+Classifier: License :: OSI Approved :: GNU General Public License v3 (GPLv3)
+Classifier: Operating System :: OS Independent
+Classifier: Topic :: Software Development :: Libraries :: Application Frameworks
+Classifier: Topic :: Home Automation
+Requires-Python: >=3.8
+Description-Content-Type: text/markdown
+Requires-Dist: netifaces
+Requires-Dist: aiohttp
+Requires-Dist: pymodbus
+
+# PyIskra
+
+PyIskra is a Python package designed to provide interface for Iskra devices using SG and it's RestAPI or ModbusTCP/RTU.
+
+## Installation
+
+You can install PyIskra using pip:
+
+```bash
+pip install pyiskra
+```
+
+## Features
+
+- Object-oriented mapping for energy meters
+- Access to measurements
+- Access to Energy counters
+
+## Supported devices
+
+- Smart Gateway
+- IE38
+- IE14
+- MCXXX
+- iMCXXX
+- MTXXX
+- iMTXXX
+
+
+## Usage
+
+Here's a basic example of how to use PyIskra:
+
+```
+import asyncio
+from pyiskra.devices import Device
+from pyiskra.adapters import RestAPI
+
+
+device_ip = "192.168.1.1"
+device_auth = {"username": "admin", "password": "iskra"}
+
+async def main():
+    # Set device IP address
+
+    # Create adapter
+    adapter = RestAPI(ip_address=device_ip, authentication=device_auth)
+
+    # Create device
+    device = await Device.create_device(adapter)
+
+    # Initalize device
+    await device.init()
+
+    devices = [device]
+
+
+    if device.is_gateway:
+        devices += device.get_child_devices()
+
+
+    for device in devices:
+        # Update device status
+        print(f"Updating status for {device.model} {device.serial}")
+        await device.update_status()
+
+        if device.supports_measurements:
+            for index, phase in enumerate(device.measurements.phases):
+                print(f"Phase {index+1} - U: {phase.voltage.value} {phase.voltage.units}, I: {phase.current.value} {phase.current.units} P: {phase.active_power.value} {phase.active_power.units} Q: {phase.reactive_power.value} {phase.reactive_power.units} S: {phase.apparent_power.value} {phase.apparent_power.units} PF: {phase.power_factor.value} {phase.power_factor.units} PA: {phase.power_angle.value} {phase.power_angle.units} THD U: {phase.thd_voltage.value} {phase.thd_voltage.units} THD I: {phase.thd_current.value} {phase.thd_current.units}")
+
+        if device.supports_counters:
+            for counter in device.counters.non_resettable :
+                print(f"Non-resettable counter - Name: {counter.name}, Value: {counter.value} {counter.units}, Direction: {counter.direction}")
+
+
+            for counter in device.counters.resettable:
+                print(f"Resettable counter - Name: {counter.name}, Value: {counter.value} {counter.units}, Direction: {counter.direction}")
+
+asyncio.run(main())
+```
```

### Comparing `pyiskra-1.0.0/pyproject.toml` & `pyiskra-1.0.1/pyproject.toml`

 * *Files 20% similar despite different names*

```diff
@@ -1,29 +1,29 @@
-[build-system]
-requires = ["setuptools", "wheel"]
-
-[tool.poetry]
-name = "pyiskra"
-version = "1.0.0"
-description = "Python Iskra devices interface"
-authors = ["Iskra d.o.o. <razvoj.mis@iskra.eu>"]
-license = "GPL"
-readme = "README.md"
-homepage = "https://github.com/Iskramis/pyiskra"
-repository = "https://github.com/Iskramis/pyiskra"
-documentation = "https://github.com/Iskramis/pyiskra"
-keywords = ["homeautomation", "iskra", "energy meter"]
-classifiers = [
-    "Programming Language :: Python :: 3",
-    "License :: OSI Approved :: GNU General Public License v3 (GPLv3)",
-    "Operating System :: OS Independent",
-    "Topic :: Software Development :: Libraries :: Application Frameworks",
-    "Topic :: Home Automation",
-]
-
-[tool.poetry.dependencies]
-python = "^3.8"
-netifaces = "*"
-aiohttp = "*"
-pymodbus = "*"
-
+[build-system]
+requires = ["setuptools", "wheel"]
+
+[tool.poetry]
+name = "pyiskra"
+version = "1.0.1"
+description = "Python Iskra devices interface"
+authors = ["Iskra d.o.o. <razvoj.mis@iskra.eu>"]
+license = "GPL"
+readme = "README.md"
+homepage = "https://github.com/Iskramis/pyiskra"
+repository = "https://github.com/Iskramis/pyiskra"
+documentation = "https://github.com/Iskramis/pyiskra"
+keywords = ["homeautomation", "iskra", "energy meter"]
+classifiers = [
+    "Programming Language :: Python :: 3",
+    "License :: OSI Approved :: GNU General Public License v3 (GPLv3)",
+    "Operating System :: OS Independent",
+    "Topic :: Software Development :: Libraries :: Application Frameworks",
+    "Topic :: Home Automation",
+]
+
+[tool.poetry.dependencies]
+python = "^3.8"
+netifaces = "*"
+aiohttp = "*"
+pymodbus = "*"
+
 [tool.poetry.dev-dependencies]
```

### Comparing `pyiskra-1.0.0/setup.py` & `pyiskra-1.0.1/setup.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,30 +1,30 @@
-#!/usr/bin/env python3
-
-from setuptools import setup
-
-with open("README.md", "r") as fh:
-    long_description = fh.read()
-
-setup(
-    name="pyiskra",
-    version="1.0.0",
-    description="Python Iskra devices interface",
-    long_description=long_description,
-    long_description_content_type="text/markdown",
-    author="Iskra d.o.o.",
-    author_email="razvoj.mis@iskra.eu",
-    maintainer=", ".join(("Iskra <razvoj.mis@iskra.eu>",)),
-    license="GPL",
-    url="https://github.com/Iskramis/pyiskra",
-    python_requires=">=3.8",
-    packages=["pyiskra"],
-    keywords=["homeautomation", "iskra", "energy meter"],
-    classifiers=[
-        "Programming Language :: Python :: 3",
-        "License :: OSI Approved :: GNU General Public License v3 (GPLv3)",
-        "Operating System :: OS Independent",
-        "Topic :: Software Development :: Libraries :: Application Frameworks",
-        "Topic :: Home Automation",
-    ],
-    install_requires=["netifaces", "aiohttp", "pymodbus"],
-)
+#!/usr/bin/env python3
+
+from setuptools import setup
+
+with open("README.md", "r") as fh:
+    long_description = fh.read()
+
+setup(
+    name="pyiskra",
+    version="1.0.1",
+    description="Python Iskra devices interface",
+    long_description=long_description,
+    long_description_content_type="text/markdown",
+    author="Iskra d.o.o.",
+    author_email="razvoj.mis@iskra.eu",
+    maintainer=", ".join(("Iskra <razvoj.mis@iskra.eu>",)),
+    license="GPL",
+    url="https://github.com/Iskramis/pyiskra",
+    python_requires=">=3.8",
+    packages=["pyiskra"],
+    keywords=["homeautomation", "iskra", "energy meter"],
+    classifiers=[
+        "Programming Language :: Python :: 3",
+        "License :: OSI Approved :: GNU General Public License v3 (GPLv3)",
+        "Operating System :: OS Independent",
+        "Topic :: Software Development :: Libraries :: Application Frameworks",
+        "Topic :: Home Automation",
+    ],
+    install_requires=["netifaces", "aiohttp", "pymodbus"],
+)
```

