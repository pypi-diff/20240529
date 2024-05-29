# Comparing `tmp/titandevice-0.4.1.1.tar.gz` & `tmp/titandevice-0.5.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "titandevice-0.4.1.1.tar", last modified: Wed May 15 03:24:14 2024, max compression
+gzip compressed data, was "titandevice-0.5.0.tar", last modified: Wed May 29 07:54:36 2024, max compression
```

## Comparing `titandevice-0.4.1.1.tar` & `titandevice-0.5.0.tar`

### file list

```diff
@@ -1,24 +1,43 @@
-drwxrwxr-x   0 mark      (1000) mark      (1000)        0 2024-05-15 03:24:14.236597 titandevice-0.4.1.1/
--rw-r--r--   0 mark      (1000) mark      (1000)      575 2024-05-15 03:24:14.236597 titandevice-0.4.1.1/PKG-INFO
--rw-rw-r--   0 mark      (1000) mark      (1000)      161 2024-05-11 08:04:43.000000 titandevice-0.4.1.1/README.md
--rw-rw-r--   0 mark      (1000) mark      (1000)       38 2024-05-15 03:24:14.236597 titandevice-0.4.1.1/setup.cfg
--rw-rw-r--   0 mark      (1000) mark      (1000)      798 2024-05-15 03:24:14.000000 titandevice-0.4.1.1/setup.py
-drwxrwxr-x   0 mark      (1000) mark      (1000)        0 2024-05-15 03:24:14.236597 titandevice-0.4.1.1/tests/
--rw-rw-r--   0 mark      (1000) mark      (1000)     2689 2024-05-15 02:46:20.000000 titandevice-0.4.1.1/tests/tests.py
-drwxrwxr-x   0 mark      (1000) mark      (1000)        0 2024-05-15 03:24:14.236597 titandevice-0.4.1.1/titandevice/
--rw-rw-r--   0 mark      (1000) mark      (1000)       75 2024-05-15 03:24:14.000000 titandevice-0.4.1.1/titandevice/__init__.py
--rw-rw-r--   0 mark      (1000) mark      (1000)     1162 2024-05-14 11:10:29.000000 titandevice-0.4.1.1/titandevice/_titian_exception.py
-drwxrwxr-x   0 mark      (1000) mark      (1000)        0 2024-05-15 03:24:14.236597 titandevice-0.4.1.1/titandevice/android/
--rw-rw-r--   0 mark      (1000) mark      (1000)        0 2024-05-14 09:15:12.000000 titandevice-0.4.1.1/titandevice/android/__init__.py
--rw-rw-r--   0 mark      (1000) mark      (1000)     3280 2024-05-15 03:09:28.000000 titandevice-0.4.1.1/titandevice/android/device.py
--rw-rw-r--   0 mark      (1000) mark      (1000)     1234 2024-05-15 03:09:28.000000 titandevice-0.4.1.1/titandevice/android/device_manager.py
--rw-rw-r--   0 mark      (1000) mark      (1000)     3006 2024-05-15 03:09:28.000000 titandevice-0.4.1.1/titandevice/android/frida.py
--rw-rw-r--   0 mark      (1000) mark      (1000)     2026 2024-05-15 03:09:55.000000 titandevice-0.4.1.1/titandevice/android/frida_manager.py
--rw-rw-r--   0 mark      (1000) mark      (1000)     1638 2024-05-15 03:09:28.000000 titandevice-0.4.1.1/titandevice/android/package_manager.py
--rw-rw-r--   0 mark      (1000) mark      (1000)       88 2024-05-14 07:18:06.000000 titandevice-0.4.1.1/titandevice/utils.py
-drwxrwxr-x   0 mark      (1000) mark      (1000)        0 2024-05-15 03:24:14.236597 titandevice-0.4.1.1/titandevice.egg-info/
--rw-r--r--   0 mark      (1000) mark      (1000)      575 2024-05-15 03:24:14.000000 titandevice-0.4.1.1/titandevice.egg-info/PKG-INFO
--rw-rw-r--   0 mark      (1000) mark      (1000)      490 2024-05-15 03:24:14.000000 titandevice-0.4.1.1/titandevice.egg-info/SOURCES.txt
--rw-rw-r--   0 mark      (1000) mark      (1000)        1 2024-05-15 03:24:14.000000 titandevice-0.4.1.1/titandevice.egg-info/dependency_links.txt
--rw-rw-r--   0 mark      (1000) mark      (1000)       18 2024-05-15 03:24:14.000000 titandevice-0.4.1.1/titandevice.egg-info/requires.txt
--rw-rw-r--   0 mark      (1000) mark      (1000)       12 2024-05-15 03:24:14.000000 titandevice-0.4.1.1/titandevice.egg-info/top_level.txt
+drwxrwxr-x   0 mark      (1000) mark      (1000)        0 2024-05-29 07:54:36.424466 titandevice-0.5.0/
+-rw-r--r--   0 mark      (1000) mark      (1000)      573 2024-05-29 07:54:36.424466 titandevice-0.5.0/PKG-INFO
+-rw-rw-r--   0 mark      (1000) mark      (1000)      161 2024-05-11 08:04:43.000000 titandevice-0.5.0/README.md
+-rw-rw-r--   0 mark      (1000) mark      (1000)       38 2024-05-29 07:54:36.424466 titandevice-0.5.0/setup.cfg
+-rw-rw-r--   0 mark      (1000) mark      (1000)      796 2024-05-29 07:54:26.000000 titandevice-0.5.0/setup.py
+drwxrwxr-x   0 mark      (1000) mark      (1000)        0 2024-05-29 07:54:36.424466 titandevice-0.5.0/tests/
+-rw-rw-r--   0 mark      (1000) mark      (1000)     4456 2024-05-29 07:54:26.000000 titandevice-0.5.0/tests/tests.py
+drwxrwxr-x   0 mark      (1000) mark      (1000)        0 2024-05-29 07:54:36.424466 titandevice-0.5.0/titandevice/
+-rw-rw-r--   0 mark      (1000) mark      (1000)        0 2024-05-28 02:04:52.000000 titandevice-0.5.0/titandevice/__init__.py
+drwxrwxr-x   0 mark      (1000) mark      (1000)        0 2024-05-29 07:54:36.424466 titandevice-0.5.0/titandevice/android/
+-rw-rw-r--   0 mark      (1000) mark      (1000)      202 2024-05-28 03:02:02.000000 titandevice-0.5.0/titandevice/android/__init__.py
+drwxrwxr-x   0 mark      (1000) mark      (1000)        0 2024-05-29 07:54:36.424466 titandevice-0.5.0/titandevice/android/application/
+-rw-rw-r--   0 mark      (1000) mark      (1000)        0 2024-05-27 07:04:46.000000 titandevice-0.5.0/titandevice/android/application/__init__.py
+-rw-rw-r--   0 mark      (1000) mark      (1000)      897 2024-05-29 03:23:15.000000 titandevice-0.5.0/titandevice/android/application/application.py
+-rw-rw-r--   0 mark      (1000) mark      (1000)     3380 2024-05-29 03:07:03.000000 titandevice-0.5.0/titandevice/android/application/package.py
+-rw-rw-r--   0 mark      (1000) mark      (1000)     4984 2024-05-29 06:33:14.000000 titandevice-0.5.0/titandevice/android/application/package_manager.py
+-rw-rw-r--   0 mark      (1000) mark      (1000)     2265 2024-05-28 10:21:31.000000 titandevice-0.5.0/titandevice/android/application/test.py
+drwxrwxr-x   0 mark      (1000) mark      (1000)        0 2024-05-29 07:54:36.424466 titandevice-0.5.0/titandevice/android/capture/
+-rw-rw-r--   0 mark      (1000) mark      (1000)        0 2024-05-16 02:43:04.000000 titandevice-0.5.0/titandevice/android/capture/__init__.py
+-rw-rw-r--   0 mark      (1000) mark      (1000)     3668 2024-05-29 06:32:04.000000 titandevice-0.5.0/titandevice/android/capture/capture_manager.py
+drwxrwxr-x   0 mark      (1000) mark      (1000)        0 2024-05-29 07:54:36.424466 titandevice-0.5.0/titandevice/android/config/
+-rw-rw-r--   0 mark      (1000) mark      (1000)     2336 2024-05-29 02:07:26.000000 titandevice-0.5.0/titandevice/android/config/__init__.py
+drwxrwxr-x   0 mark      (1000) mark      (1000)        0 2024-05-29 07:54:36.424466 titandevice-0.5.0/titandevice/android/device/
+-rw-rw-r--   0 mark      (1000) mark      (1000)        0 2024-05-27 07:03:29.000000 titandevice-0.5.0/titandevice/android/device/__init__.py
+-rw-rw-r--   0 mark      (1000) mark      (1000)     2791 2024-05-29 06:17:58.000000 titandevice-0.5.0/titandevice/android/device/device_manager.py
+drwxrwxr-x   0 mark      (1000) mark      (1000)        0 2024-05-29 07:54:36.424466 titandevice-0.5.0/titandevice/android/frida/
+-rw-rw-r--   0 mark      (1000) mark      (1000)        0 2024-05-27 07:04:51.000000 titandevice-0.5.0/titandevice/android/frida/__init__.py
+-rw-rw-r--   0 mark      (1000) mark      (1000)     1614 2024-05-22 07:10:55.000000 titandevice-0.5.0/titandevice/android/frida/frida_app.py
+-rw-rw-r--   0 mark      (1000) mark      (1000)      736 2024-05-28 02:44:59.000000 titandevice-0.5.0/titandevice/android/frida/frida_app_manager.py
+-rw-rw-r--   0 mark      (1000) mark      (1000)     3568 2024-05-28 02:44:59.000000 titandevice-0.5.0/titandevice/android/frida/frida_device.py
+-rw-rw-r--   0 mark      (1000) mark      (1000)     2364 2024-05-27 13:11:12.000000 titandevice-0.5.0/titandevice/android/frida/frida_device_manager.py
+drwxrwxr-x   0 mark      (1000) mark      (1000)        0 2024-05-29 07:54:36.424466 titandevice-0.5.0/titandevice/exception/
+-rw-rw-r--   0 mark      (1000) mark      (1000)     1993 2024-05-29 03:01:48.000000 titandevice-0.5.0/titandevice/exception/__init__.py
+drwxrwxr-x   0 mark      (1000) mark      (1000)        0 2024-05-29 07:54:36.424466 titandevice-0.5.0/titandevice/utils/
+-rw-rw-r--   0 mark      (1000) mark      (1000)      566 2024-05-29 06:17:58.000000 titandevice-0.5.0/titandevice/utils/__init__.py
+-rw-rw-r--   0 mark      (1000) mark      (1000)     4098 2024-05-29 03:23:15.000000 titandevice-0.5.0/titandevice/utils/adb_utils.py
+-rw-rw-r--   0 mark      (1000) mark      (1000)      976 2024-05-28 02:56:11.000000 titandevice-0.5.0/titandevice/utils/logger_utils.py
+drwxrwxr-x   0 mark      (1000) mark      (1000)        0 2024-05-29 07:54:36.424466 titandevice-0.5.0/titandevice.egg-info/
+-rw-r--r--   0 mark      (1000) mark      (1000)      573 2024-05-29 07:54:36.000000 titandevice-0.5.0/titandevice.egg-info/PKG-INFO
+-rw-rw-r--   0 mark      (1000) mark      (1000)     1043 2024-05-29 07:54:36.000000 titandevice-0.5.0/titandevice.egg-info/SOURCES.txt
+-rw-rw-r--   0 mark      (1000) mark      (1000)        1 2024-05-29 07:54:36.000000 titandevice-0.5.0/titandevice.egg-info/dependency_links.txt
+-rw-rw-r--   0 mark      (1000) mark      (1000)       18 2024-05-29 07:54:36.000000 titandevice-0.5.0/titandevice.egg-info/requires.txt
+-rw-rw-r--   0 mark      (1000) mark      (1000)       12 2024-05-29 07:54:36.000000 titandevice-0.5.0/titandevice.egg-info/top_level.txt
```

### Comparing `titandevice-0.4.1.1/PKG-INFO` & `titandevice-0.5.0/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: titandevice
-Version: 0.4.1.1
+Version: 0.5.0
 Summary: A Python library used for managing device
 Author: 369
 Author-email: luck.yangbo@gmai.com
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.6
```

### Comparing `titandevice-0.4.1.1/setup.py` & `titandevice-0.5.0/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -7,15 +7,15 @@
 def read_readme():
     with open(os.path.join(os.getcwd(), 'README.md'), 'r', encoding='utf-8') as file:
         return file.read()
 
 
 setup(
     name="titandevice",
-    version="0.4.1.1",
+    version="0.5.0",
     author="369",
     author_email="luck.yangbo@gmai.com",
     description="A Python library used for managing device",
     long_description=read_readme(),
     long_description_content_type="text/markdown",
     packages=setuptools.find_packages(),
     classifiers=[
```

### Comparing `titandevice-0.4.1.1/titandevice/_titian_exception.py` & `titandevice-0.5.0/titandevice/exception/__init__.py`

 * *Files 20% similar despite different names*

```diff
@@ -14,14 +14,29 @@
 
 
 class PackageNoFoundException(TitanException):
     def __init__(self, device_serial: str, package_name: str):
         super().__init__(f"Package {package_name} not found on device {device_serial}.")
 
 
+class GooglePlayAccountNotSetException(TitanException):
+    def __init__(self, device_serial: str):
+        super().__init__(f"Google Play account not set on device {device_serial}.")
+
+
+class GooglePlayIsNotInstalledException(TitanException):
+    def __init__(self, device_serial: str):
+        super().__init__(f"Google Play is not installed on device {device_serial}.")
+
+
+class PackageNotInstalledException(TitanException):
+    def __init__(self, device_serial: str, package_name: str):
+        super().__init__(f"Package {package_name} is not installed on device {device_serial}.")
+
+
 class DeviceMustBeRootedException(TitanException):
     def __init__(self, device_serial: str):
         super().__init__(f"Device with serial {device_serial} must be rooted.")
 
 
 class AnyFridaNotInstalledException(TitanException):
     def __init__(self):
@@ -29,7 +44,14 @@
 
 
 class FridaNotInstalledException(TitanException):
     def __init__(self, device_serial: str, frida_server_path: str):
         super().__init__(
             f"Frida not installed on device {device_serial} with path {frida_server_path}."
         )
+
+
+class FridaNotRunningException(TitanException):
+    def __init__(self, device_serial: str, frida_server_name: str):
+        super().__init__(
+            f"Frida not running on device {device_serial} with name {frida_server_name}."
+        )
```

### Comparing `titandevice-0.4.1.1/titandevice/android/frida.py` & `titandevice-0.5.0/titandevice/android/frida/frida_device.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,33 +1,46 @@
 import os.path
 import subprocess
 
 from adbutils import adb_path
 
-from titandevice import FridaNotInstalledException
+from titandevice import FridaNotInstalledException, FridaNotRunningException
+from titandevice.android.device.device import Device
+from titandevice.android.frida.frida_app_manager import FridaAppManager
 from titandevice.utils import get_file_name_from_path
 
 
-class AndroidFrida:
+class FridaDevice:
 
     @staticmethod
     def __check_is_installed(func):
 
         def wrapper(self, *args, **kwargs):
             if not self.__android_device.file_exists(self.__frida_server_full_path):
                 raise FridaNotInstalledException(
-                    self.__android_device.device_serial, self.__frida_server_full_path
+                    self.__android_device.__device_serial, self.__frida_server_full_path
+                )
+            return func(self, *args, **kwargs)
+
+        return wrapper
+
+    @staticmethod
+    def __check_is_running(func):
+
+        def wrapper(self, *args, **kwargs):
+            if not self.__is_running:
+                raise FridaNotRunningException(
+                    self.__android_device.__device_serial, self.__frida_server_name
                 )
             return func(self, *args, **kwargs)
 
         return wrapper
 
     def __init__(self, android_device, frida_server_executable_file_path):
-        from titandevice.android.device import AndroidDevice
-        self.__android_device: AndroidDevice = android_device
+        self.__android_device: Device = android_device
         self.__frida_server_full_path = frida_server_executable_file_path
         self.__frida_server_path = os.path.abspath(frida_server_executable_file_path)
         self.__frida_server_name = get_file_name_from_path(
             frida_server_executable_file_path
         )
         self.__version = self.__get_version()
         self.__is_running = self.__check_if_running()
@@ -69,15 +82,15 @@
             'version': self.__version
         }
 
     @__check_is_installed
     def start(self):
         if not self.__is_running:
             subprocess.Popen(
-                [adb_path(), '-s', self.__android_device.device_serial, 'shell',
+                [adb_path(), '-s', self.__android_device.__device_serial, 'shell',
                  'nohup',
                  'su -c', self.__frida_server_full_path, '&']
             )
         self.__is_running = self.__check_if_running()
         return self.__is_running
 
     @__check_is_installed
@@ -88,7 +101,12 @@
             )
         self.__is_running = self.__check_if_running()
         return not self.__is_running
 
     def uninstall(self):
         self.__android_device.remove_file(self.__frida_server_full_path)
         return not self.__android_device.file_exists(self.__frida_server_full_path)
+
+    @__check_is_running
+    def get_application_manager(self):
+        return FridaAppManager(self.__android_device)
+
```

### Comparing `titandevice-0.4.1.1/titandevice/android/frida_manager.py` & `titandevice-0.5.0/titandevice/android/frida/frida_device_manager.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,36 +1,36 @@
-from titandevice.android.device import AndroidDevice
+from titandevice.android.device.device import Device
+from titandevice.android.frida.frida_device import FridaDevice
 
 
-class AndroidFridaManager:
+class FridaDeviceManager:
     def __init__(
-            self, android_device: AndroidDevice, frida_server_file_name_prefix: str,
+            self, android_device: Device, frida_server_file_name_prefix: str,
             frida_server_install_path: str
     ):
         self.__android_device = android_device
         self.__frida_server_file_name_prefix = frida_server_file_name_prefix
         if not frida_server_install_path.endswith('/'):
             frida_server_install_path += '/'
         self.__frida_server_install_path = frida_server_install_path
 
-    def get_all_frida(self):
-        from titandevice.android.frida import AndroidFrida
+    def get_all_frida_list(self):
         return [
-            AndroidFrida(self.__android_device, frida_server_path) for
+            FridaDevice(self.__android_device, frida_server_path) for
             frida_server_path in
             self.get_all_frida_executable_file_path()
         ]
 
     def get_all_frida_executable_file_path(self) -> list[str]:
         files = self.__android_device.get_all_files(self.__frida_server_install_path)
         return [self.__get_frida_server_path(file) for file in files if
                 file.startswith(self.__frida_server_file_name_prefix)]
 
     def uninstall_all(self):
-        for frida in self.get_all_frida():
+        for frida in self.get_all_frida_list():
             frida.stop()
             frida.uninstall()
 
     def install_frida(self, input_frida_server_path: str):
         from titandevice.utils import get_file_name_from_path
         file_name = get_file_name_from_path(input_frida_server_path)
         self.__android_device.push(
@@ -42,9 +42,18 @@
         )
         return self.__android_device.file_exists(frida_server_file_path)
 
     def __get_frida_server_path(self, frida_server_name: str) -> str:
         return f'{self.__frida_server_install_path}{frida_server_name}'
 
     def stop_all_frida(self):
-        for frida in self.get_all_frida():
+        for frida in self.get_all_frida_list():
             frida.stop()
+
+    def get_frida_by_path(self, frida_server_full_path):
+        return FridaDevice(self.__android_device, frida_server_full_path)
+
+    def get_frida_by_version(self, frida_version):
+        for frida in self.get_all_frida_list():
+            if frida.version == frida_version:
+                return frida
+        return None
```

### Comparing `titandevice-0.4.1.1/titandevice.egg-info/PKG-INFO` & `titandevice-0.5.0/titandevice.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: titandevice
-Version: 0.4.1.1
+Version: 0.5.0
 Summary: A Python library used for managing device
 Author: 369
 Author-email: luck.yangbo@gmai.com
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.6
```

