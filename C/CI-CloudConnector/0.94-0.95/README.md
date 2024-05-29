# Comparing `tmp/ci_cloudconnector-0.94.tar.gz` & `tmp/ci_cloudconnector-0.95.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ci_cloudconnector-0.94.tar", last modified: Wed May 29 18:21:08 2024, max compression
+gzip compressed data, was "ci_cloudconnector-0.95.tar", last modified: Wed May 29 18:48:21 2024, max compression
```

## Comparing `ci_cloudconnector-0.94.tar` & `ci_cloudconnector-0.95.tar`

### file list

```diff
@@ -1,13 +1,13 @@
-drwxrwxrwx   0        0        0        0 2024-05-29 18:21:08.394905 ci_cloudconnector-0.94/
-drwxrwxrwx   0        0        0        0 2024-05-29 18:21:08.387708 ci_cloudconnector-0.94/CI_CloudConnector.egg-info/
--rw-rw-rw-   0        0        0      358 2024-05-29 18:21:08.000000 ci_cloudconnector-0.94/CI_CloudConnector.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      213 2024-05-29 18:21:08.000000 ci_cloudconnector-0.94/CI_CloudConnector.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-05-29 18:21:08.000000 ci_cloudconnector-0.94/CI_CloudConnector.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       27 2024-05-29 18:21:08.000000 ci_cloudconnector-0.94/CI_CloudConnector.egg-info/top_level.txt
--rw-rw-rw-   0        0        0      358 2024-05-29 18:21:08.391921 ci_cloudconnector-0.94/PKG-INFO
--rw-rw-rw-   0        0        0       86 2024-05-23 13:47:51.000000 ci_cloudconnector-0.94/README.txt
--rw-rw-rw-   0        0        0    38752 2024-05-29 18:20:51.000000 ci_cloudconnector-0.94/logic.py
--rw-rw-rw-   0        0        0     8241 2024-05-29 17:52:57.000000 ci_cloudconnector-0.94/main.py
--rw-rw-rw-   0        0        0     2666 2024-05-29 17:20:02.000000 ci_cloudconnector-0.94/myservice.py
--rw-rw-rw-   0        0        0       42 2024-05-29 18:21:08.395313 ci_cloudconnector-0.94/setup.cfg
--rw-rw-rw-   0        0        0      791 2024-05-29 18:20:42.000000 ci_cloudconnector-0.94/setup.py
+drwxrwxrwx   0        0        0        0 2024-05-29 18:48:21.926079 ci_cloudconnector-0.95/
+drwxrwxrwx   0        0        0        0 2024-05-29 18:48:21.920328 ci_cloudconnector-0.95/CI_CloudConnector.egg-info/
+-rw-rw-rw-   0        0        0      358 2024-05-29 18:48:21.000000 ci_cloudconnector-0.95/CI_CloudConnector.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      213 2024-05-29 18:48:21.000000 ci_cloudconnector-0.95/CI_CloudConnector.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-05-29 18:48:21.000000 ci_cloudconnector-0.95/CI_CloudConnector.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       27 2024-05-29 18:48:21.000000 ci_cloudconnector-0.95/CI_CloudConnector.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0      358 2024-05-29 18:48:21.922662 ci_cloudconnector-0.95/PKG-INFO
+-rw-rw-rw-   0        0        0       86 2024-05-23 13:47:51.000000 ci_cloudconnector-0.95/README.txt
+-rw-rw-rw-   0        0        0    38752 2024-05-29 18:47:31.000000 ci_cloudconnector-0.95/logic.py
+-rw-rw-rw-   0        0        0     7755 2024-05-29 18:47:17.000000 ci_cloudconnector-0.95/main.py
+-rw-rw-rw-   0        0        0     2827 2024-05-29 18:43:18.000000 ci_cloudconnector-0.95/myservice.py
+-rw-rw-rw-   0        0        0       42 2024-05-29 18:48:21.926079 ci_cloudconnector-0.95/setup.cfg
+-rw-rw-rw-   0        0        0      791 2024-05-29 18:47:40.000000 ci_cloudconnector-0.95/setup.py
```

### Comparing `ci_cloudconnector-0.94/logic.py` & `ci_cloudconnector-0.95/logic.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 
 import logging, time, datetime, sys, os, socket, configparser, random, tzlocal, glob, fnmatch
 import platform
 from datetime import datetime
 
 from cpppo.server.enip import address, client  # for EtherNet/IP communication
 
-VER = "0.94"
+VER = "0.95"
 
 TagsDefenitionFileName = "TagsDefenition.txt"
 TagsValuesFileName = "[NEW]TagsValues"
 TagsValueDir = "TagValues"
 HomeDir = "CI_LC"
 GetTagsFromServerMinRateSeconds = 10
 GetCloudVersionFromServerMinRateSeconds = 10
```

### Comparing `ci_cloudconnector-0.94/main.py` & `ci_cloudconnector-0.95/main.py`

 * *Files 8% similar despite different names*

```diff
@@ -42,27 +42,21 @@
             self.is_running = True
 
     def stop(self):
         self._timer.cancel()
         self.is_running = False
 
 
+
 def update_and_run(script_path, package_name, package_version):
     try:
         logic.ci_print(f'package_version: {package_version}')
 
-        # Get the directory of the Python executable
-        python_executable_path = sys.executable
-        python_executable_dir = os.path.dirname(python_executable_path)
-
         current_script_dir = os.path.dirname(os.path.abspath(__file__))
 
-        # Path to the pip executable
-        pip_executable = r"C:\\Users\\yochaim\\AppData\\Local\\Programs\\Python\\Python312\\Scripts\\pip.exe"
-
         if package_version == '':
             # Upgrade the package
             command = ["pip", "install", "--upgrade", package_name]
         else:
             # Install or upgrade the package with specific version
             command = ["pip", "install", "--force-reinstall", f"{package_name}=={package_version}"]
 
@@ -104,44 +98,35 @@
 
         if package_location is None:
             logic.ci_print("Could not determine the package location.")
             return
 
         # Construct the path to the installed package
         installed_package_path = package_location
-        destination_path = os.getcwd()
 
         logic.ci_print('package_info: ' + package_info)
         logic.ci_print('installed_package_path: ' + installed_package_path)
-        logic.ci_print('destination_path: ' + destination_path)
 
         logic_source = os.path.join(installed_package_path, "logic.py")
         main_source = os.path.join(installed_package_path, "main.py")
         myservice_source = os.path.join(installed_package_path, "myservice.py")
         setup_source = os.path.join(installed_package_path, "setup.py")
 
         if not os.path.isfile(logic_source) or not os.path.isfile(main_source):
             print(f"logic.py or main.py not found in {installed_package_path}.")
             return
 
         # Copy files to the destination
-        shutil.copy(logic_source, destination_path)
-        shutil.copy(main_source, destination_path)
-        shutil.copy(myservice_source, destination_path)
-        shutil.copy(setup_source, destination_path)
-
         shutil.copy(logic_source, current_script_dir)
         shutil.copy(main_source, current_script_dir)
         shutil.copy(myservice_source, current_script_dir)
         shutil.copy(setup_source, current_script_dir)
 
 
-
-
-        print(f"Copied logic.py and main.py to {destination_path}")
+        print(f"Copied logic.py and main.py to {current_script_dir}")
 
 
     except subprocess.CalledProcessError as e:
         logic.ci_print(f"An error occurred: {e}")
 
 
 def upgrade_version(new_version="", current_version=""):
@@ -230,38 +215,37 @@
 
             # Stop the service
             self.myService.ServiceUpdated()
             logic.ci_print("Service stopped. You may restart it if necessary.")
 
 
 
-
-
-
 def monitor_main_file(main_file, service):
     observer = Observer()
-    event_handler = MainFileChangeHandler(main_file, service)
-    observer.schedule(event_handler, path='.', recursive=False)
+
+    event_handler = MainFileChangeHandler(os.path.basename(main_file), service)
+    observer.schedule(event_handler, path=os.path.dirname(main_file), recursive=False)
+
     observer.start()
     return observer
 
 
 def init():
     logic.create_directories_if_missing()
     logic.initialize_config()
 
 
 
-
-
 def serviceStop():
     global service_stop
     service_stop = 1
     logic.ci_print("Service stop requested.")
 
 
 
 if __name__ == '__main__':
     init()
     args(sys.argv)
     #args([0, 'Start'])
-    monitor_main_file("logic.py")
+    current_script_dir = os.path.dirname(os.path.abspath(__file__))
+    main_file = os.path.join(current_script_dir, "logic.py")
+    monitor_main_file(main_file)
```

### Comparing `ci_cloudconnector-0.94/myservice.py` & `ci_cloudconnector-0.95/myservice.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,7 +1,8 @@
+import os
 import sys
 import time
 
 import psutil
 import win32api
 import win32con
 import win32serviceutil
@@ -21,15 +22,18 @@
         win32serviceutil.ServiceFramework.__init__(self, args)
         self.stop_event = win32event.CreateEvent(None, 0, 0, None)
 
     def SvcDoRun(self):
         try:
             main.init()
             main.args([0, 'Start'])
-            observer = main.monitor_main_file("logic.py", self)
+
+            current_script_dir = os.path.dirname(os.path.abspath(__file__))
+            logic_file = os.path.join(current_script_dir, "logic.py")
+            observer = main.monitor_main_file(logic_file, self)
 
             try:
                 while main.service_stop == 0:
                     time.sleep(1)
             except KeyboardInterrupt:
                 pass
             finally:
```

### Comparing `ci_cloudconnector-0.94/setup.py` & `ci_cloudconnector-0.95/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -11,15 +11,15 @@
 
     return ans
 
 
 
 setup(
     name="CI_CloudConnector",
-    version="0.94",
+    version="0.95",
     packages=find_packages(),
     py_modules=["logic", "main", "setup", "myservice"],
     description="IOT application that collects data from PLC (ModBus or AnB Ethernet/IP) and sends it to the cloud using HTTPS",
     author="Yochai",
     author_email="yochaim@contel.co.il",
     install_requires=[],
     url="https://trunovate.com/",
```

