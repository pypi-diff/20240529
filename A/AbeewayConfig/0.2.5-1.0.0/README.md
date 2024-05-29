# Comparing `tmp/abeewayconfig-0.2.5.tar.gz` & `tmp/abeewayconfig-1.0.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "abeewayconfig-0.2.5.tar", last modified: Mon May 27 18:49:18 2024, max compression
+gzip compressed data, was "abeewayconfig-1.0.0.tar", last modified: Wed May 29 14:05:43 2024, max compression
```

## Comparing `abeewayconfig-0.2.5.tar` & `abeewayconfig-1.0.0.tar`

### file list

```diff
@@ -1,22 +1,23 @@
-drwxr-xr-x   0 lucas     (1001) lucas     (1001)        0 2024-05-27 18:49:18.071294 abeewayconfig-0.2.5/
--rw-r--r--   0 lucas     (1001) lucas     (1001)    35149 2024-05-15 17:30:13.000000 abeewayconfig-0.2.5/LICENSE
--rw-r--r--   0 lucas     (1001) lucas     (1001)     1731 2024-05-27 18:49:18.071294 abeewayconfig-0.2.5/PKG-INFO
--rw-r--r--   0 lucas     (1001) lucas     (1001)     1321 2024-05-27 17:40:44.000000 abeewayconfig-0.2.5/README.md
--rw-r--r--   0 lucas     (1001) lucas     (1001)       38 2024-05-27 18:49:18.071294 abeewayconfig-0.2.5/setup.cfg
--rw-r--r--   0 lucas     (1001) lucas     (1001)      801 2024-05-27 18:48:55.000000 abeewayconfig-0.2.5/setup.py
-drwxr-xr-x   0 lucas     (1001) lucas     (1001)        0 2024-05-27 18:49:18.067961 abeewayconfig-0.2.5/src/
-drwxr-xr-x   0 lucas     (1001) lucas     (1001)        0 2024-05-27 18:49:18.067961 abeewayconfig-0.2.5/src/AbeewayConfig/
--rw-r--r--   0 lucas     (1001) lucas     (1001)     8088 2024-05-27 18:43:27.000000 abeewayconfig-0.2.5/src/AbeewayConfig/CSVFile.py
--rw-r--r--   0 lucas     (1001) lucas     (1001)     3479 2024-05-27 18:47:25.000000 abeewayconfig-0.2.5/src/AbeewayConfig/Config.py
--rw-r--r--   0 lucas     (1001) lucas     (1001)     3034 2024-05-24 18:45:21.000000 abeewayconfig-0.2.5/src/AbeewayConfig/Device.py
--rw-r--r--   0 lucas     (1001) lucas     (1001)       74 2024-05-27 18:38:48.000000 abeewayconfig-0.2.5/src/AbeewayConfig/GUI_setup.py
--rw-r--r--   0 lucas     (1001) lucas     (1001)       32 2024-05-16 13:41:49.000000 abeewayconfig-0.2.5/src/AbeewayConfig/__init__.py
--rw-r--r--   0 lucas     (1001) lucas     (1001)     6100 2024-05-27 18:47:25.000000 abeewayconfig-0.2.5/src/AbeewayConfig/abeewayconfig.py
--rw-r--r--   0 lucas     (1001) lucas     (1001)     4026 2024-05-14 13:11:26.000000 abeewayconfig-0.2.5/src/AbeewayConfig/smartbadgecfgdict.py
-drwxr-xr-x   0 lucas     (1001) lucas     (1001)        0 2024-05-27 18:49:18.071294 abeewayconfig-0.2.5/src/AbeewayConfig.egg-info/
--rw-r--r--   0 lucas     (1001) lucas     (1001)     1731 2024-05-27 18:49:18.000000 abeewayconfig-0.2.5/src/AbeewayConfig.egg-info/PKG-INFO
--rw-r--r--   0 lucas     (1001) lucas     (1001)      494 2024-05-27 18:49:18.000000 abeewayconfig-0.2.5/src/AbeewayConfig.egg-info/SOURCES.txt
--rw-r--r--   0 lucas     (1001) lucas     (1001)        1 2024-05-27 18:49:18.000000 abeewayconfig-0.2.5/src/AbeewayConfig.egg-info/dependency_links.txt
--rw-r--r--   0 lucas     (1001) lucas     (1001)       67 2024-05-27 18:49:18.000000 abeewayconfig-0.2.5/src/AbeewayConfig.egg-info/entry_points.txt
--rw-r--r--   0 lucas     (1001) lucas     (1001)       21 2024-05-27 18:49:18.000000 abeewayconfig-0.2.5/src/AbeewayConfig.egg-info/requires.txt
--rw-r--r--   0 lucas     (1001) lucas     (1001)       14 2024-05-27 18:49:18.000000 abeewayconfig-0.2.5/src/AbeewayConfig.egg-info/top_level.txt
+drwxr-xr-x   0 lucas     (1001) lucas     (1001)        0 2024-05-29 14:05:43.724491 abeewayconfig-1.0.0/
+-rw-r--r--   0 lucas     (1001) lucas     (1001)    35149 2024-05-15 17:30:13.000000 abeewayconfig-1.0.0/LICENSE
+-rw-r--r--   0 lucas     (1001) lucas     (1001)     1731 2024-05-29 14:05:43.724491 abeewayconfig-1.0.0/PKG-INFO
+-rw-r--r--   0 lucas     (1001) lucas     (1001)     1321 2024-05-27 17:40:44.000000 abeewayconfig-1.0.0/README.md
+-rw-r--r--   0 lucas     (1001) lucas     (1001)       38 2024-05-29 14:05:43.724491 abeewayconfig-1.0.0/setup.cfg
+-rw-r--r--   0 lucas     (1001) lucas     (1001)      801 2024-05-29 14:04:34.000000 abeewayconfig-1.0.0/setup.py
+drwxr-xr-x   0 lucas     (1001) lucas     (1001)        0 2024-05-29 14:05:43.724491 abeewayconfig-1.0.0/src/
+drwxr-xr-x   0 lucas     (1001) lucas     (1001)        0 2024-05-29 14:05:43.724491 abeewayconfig-1.0.0/src/AbeewayConfig/
+-rw-r--r--   0 lucas     (1001) lucas     (1001)    10531 2024-05-29 13:59:27.000000 abeewayconfig-1.0.0/src/AbeewayConfig/CSVFile.py
+-rw-r--r--   0 lucas     (1001) lucas     (1001)     3746 2024-05-29 12:31:52.000000 abeewayconfig-1.0.0/src/AbeewayConfig/Config.py
+-rw-r--r--   0 lucas     (1001) lucas     (1001)     1374 2024-05-29 13:52:04.000000 abeewayconfig-1.0.0/src/AbeewayConfig/CustomGUI.py
+-rw-r--r--   0 lucas     (1001) lucas     (1001)     3034 2024-05-24 18:45:21.000000 abeewayconfig-1.0.0/src/AbeewayConfig/Device.py
+-rw-r--r--   0 lucas     (1001) lucas     (1001)       74 2024-05-27 18:38:48.000000 abeewayconfig-1.0.0/src/AbeewayConfig/GUI_setup.py
+-rw-r--r--   0 lucas     (1001) lucas     (1001)       32 2024-05-16 13:41:49.000000 abeewayconfig-1.0.0/src/AbeewayConfig/__init__.py
+-rw-r--r--   0 lucas     (1001) lucas     (1001)     5902 2024-05-29 12:48:13.000000 abeewayconfig-1.0.0/src/AbeewayConfig/abeewayconfig.py
+-rw-r--r--   0 lucas     (1001) lucas     (1001)     4026 2024-05-14 13:11:26.000000 abeewayconfig-1.0.0/src/AbeewayConfig/smartbadgecfgdict.py
+drwxr-xr-x   0 lucas     (1001) lucas     (1001)        0 2024-05-29 14:05:43.724491 abeewayconfig-1.0.0/src/AbeewayConfig.egg-info/
+-rw-r--r--   0 lucas     (1001) lucas     (1001)     1731 2024-05-29 14:05:43.000000 abeewayconfig-1.0.0/src/AbeewayConfig.egg-info/PKG-INFO
+-rw-r--r--   0 lucas     (1001) lucas     (1001)      525 2024-05-29 14:05:43.000000 abeewayconfig-1.0.0/src/AbeewayConfig.egg-info/SOURCES.txt
+-rw-r--r--   0 lucas     (1001) lucas     (1001)        1 2024-05-29 14:05:43.000000 abeewayconfig-1.0.0/src/AbeewayConfig.egg-info/dependency_links.txt
+-rw-r--r--   0 lucas     (1001) lucas     (1001)       67 2024-05-29 14:05:43.000000 abeewayconfig-1.0.0/src/AbeewayConfig.egg-info/entry_points.txt
+-rw-r--r--   0 lucas     (1001) lucas     (1001)       21 2024-05-29 14:05:43.000000 abeewayconfig-1.0.0/src/AbeewayConfig.egg-info/requires.txt
+-rw-r--r--   0 lucas     (1001) lucas     (1001)       14 2024-05-29 14:05:43.000000 abeewayconfig-1.0.0/src/AbeewayConfig.egg-info/top_level.txt
```

### Comparing `abeewayconfig-0.2.5/LICENSE` & `abeewayconfig-1.0.0/LICENSE`

 * *Files identical despite different names*

### Comparing `abeewayconfig-0.2.5/PKG-INFO` & `abeewayconfig-1.0.0/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: AbeewayConfig
-Version: 0.2.5
+Version: 1.0.0
 Summary: Abeeway configuration tool
 Home-page: https://github.com/jlabbude/AbeewayConfig
 Author: João Lucas
 Classifier: Development Status :: 3 - Alpha
 Classifier: Programming Language :: Python :: 3
 Requires-Python: >=3.0
 Description-Content-Type: text/markdown
```

### Comparing `abeewayconfig-0.2.5/README.md` & `abeewayconfig-1.0.0/README.md`

 * *Files identical despite different names*

### Comparing `abeewayconfig-0.2.5/setup.py` & `abeewayconfig-1.0.0/setup.py`

 * *Files 15% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 from setuptools import setup, find_packages
 
 with open("README.md", "r") as f:
     description = f.read()
 
 setup(
     name="AbeewayConfig",
-    version="0.2.5",
+    version="1.0.0",
     description="Abeeway configuration tool",
     author="João Lucas",
     url="https://github.com/jlabbude/AbeewayConfig",
     packages=find_packages(where="src"),
     package_dir={"": "src"},
     install_requires=[
         "pyserial",
```

### Comparing `abeewayconfig-0.2.5/src/AbeewayConfig/Config.py` & `abeewayconfig-1.0.0/src/AbeewayConfig/Config.py`

 * *Files 4% similar despite different names*

```diff
@@ -6,14 +6,22 @@
 
 from .Device import Device
 from .GUI_setup import console
 from .smartbadgecfgdict import config_dict
 
 
 class Config:
+
+    @staticmethod
+    def clear_dev_log():
+        with open(os.path.join(os.path.dirname(os.path.abspath(__file__)), "utils", "deveui.txt"), 'w') as file:
+            file.truncate()
+            file.close()
+        console.insert(tk.END, 'DevEUI log cleared.\n')
+
     def get_config_value_from_cfg(parameter: int, line: str) -> int:
         if parameter is not None:
             pattern = r"config set %d (.*)" % parameter
             p = re.compile(pattern)
             match = p.search(line)
             if match:
                 return int(match.group(1))
```

### Comparing `abeewayconfig-0.2.5/src/AbeewayConfig/Device.py` & `abeewayconfig-1.0.0/src/AbeewayConfig/Device.py`

 * *Files identical despite different names*

### Comparing `abeewayconfig-0.2.5/src/AbeewayConfig/abeewayconfig.py` & `abeewayconfig-1.0.0/src/AbeewayConfig/abeewayconfig.py`

 * *Files 13% similar despite different names*

```diff
@@ -1,21 +1,19 @@
-import tkinter as tk
-import serial.tools.list_ports
-import importlib
-
 from argparse import ArgumentParser
 from glob import glob
 from platform import system
 from threading import Thread
 from time import sleep
-from tkinter import Button, Text
+from tkinter import Button
+
+import serial.tools.list_ports
 
+from .CSVFile import CSVFile
 from .Config import Config
 from .Device import Device
-from .CSVFile import CSVFile
 from .GUI_setup import root, console
 
 baud_rate = 9600
 operating_system = system()
 
 
 def define_os_specific_serial_ports() -> None:
@@ -47,34 +45,34 @@
         thread = Thread(target=target, args=(serial_port, baud_rate))
         threads.append(thread)
         thread.start()
     for thread in threads:
         thread.join()
 
 
-def with_console_parallel_process(target, console_output):
+def no_join_parallel_process(target):
     threads = []
     for serial_port in serial_port_array:
-        thread = Thread(target=target, args=(serial_port, baud_rate, console_output))
+        thread = Thread(target=target, args=(serial_port, baud_rate))
         threads.append(thread)
         thread.start()
     return threads
 
 
-def config_process(console_output) -> None:
+def config_process() -> None:
     define_os_specific_serial_ports()
 
     # TODO: investigate instability here
     serial_parallel_process(target=Device.start_dev)
     sleep(5)
 
     serial_parallel_process(target=Device.set_config_on_device)
     sleep(5)
 
-    with_console_parallel_process(target=Config.check_config_discrepancy, console_output=console_output)
+    no_join_parallel_process(target=Config.check_config_discrepancy)
     sleep(5)
 
     serial_parallel_process(target=Device.reset_dev)
 
 
 def main() -> None:
     parser = ArgumentParser()
@@ -91,15 +89,15 @@
             button1 = Button(root,
                              text="Configure device",
                              bg="lightblue",
                              fg="black",
                              width=15,
                              height=2,
                              font=("Arial", 12),
-                             command=lambda: config_process(console_output=console))
+                             command=lambda: config_process())
             button4 = Button(root,
                              text="Reset device",
                              bg="lightcoral",
                              fg="black",
                              width=15,
                              height=2,
                              font=("Arial", 12),
@@ -125,42 +123,41 @@
             button1 = Button(root,
                              text="Make CSV",
                              bg="lightblue",
                              fg="black",
                              width=15,
                              height=2,
                              font=("Arial", 12),
-                             command=lambda: CSVFile.csv_builder())
+                             command=lambda: CSVFile.csv_builder_and_writer())
             button2 = Button(root,
-                             text="Import device info",
+                             text="Import",
                              bg="lightblue",
                              fg="black",
                              width=15,
                              height=2,
                              font=("Arial", 12),
-                             command=lambda: CSVFile.import_values())
+                             command=lambda: CSVFile.importer())
             button3 = Button(root,
                              text="Clear device log",
                              bg="lightcoral",
                              fg="black",
                              width=15,
                              height=2,
                              font=("Arial", 12),
-                             command=lambda: CSVFile.retrieve_token())
+                             command=lambda: Config.clear_dev_log())
             button4 = Button(root,
                              text="Export devices",
                              bg="lightgreen",
                              fg="black",
                              width=15,
                              height=2,
                              font=("Arial", 12),
                              command=lambda: CSVFile.export_devices_from_csv())
 
         case _:
-            print("Incorrect args.")
             exit()
 
     root.grid_rowconfigure(0, weight=1)
     root.grid_rowconfigure(1, weight=1)
     root.grid_rowconfigure(2, weight=1)
     root.grid_rowconfigure(3, weight=1)
     root.grid_rowconfigure(4, weight=4)
```

### Comparing `abeewayconfig-0.2.5/src/AbeewayConfig/smartbadgecfgdict.py` & `abeewayconfig-1.0.0/src/AbeewayConfig/smartbadgecfgdict.py`

 * *Files identical despite different names*

### Comparing `abeewayconfig-0.2.5/src/AbeewayConfig.egg-info/PKG-INFO` & `abeewayconfig-1.0.0/src/AbeewayConfig.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: AbeewayConfig
-Version: 0.2.5
+Version: 1.0.0
 Summary: Abeeway configuration tool
 Home-page: https://github.com/jlabbude/AbeewayConfig
 Author: João Lucas
 Classifier: Development Status :: 3 - Alpha
 Classifier: Programming Language :: Python :: 3
 Requires-Python: >=3.0
 Description-Content-Type: text/markdown
```

