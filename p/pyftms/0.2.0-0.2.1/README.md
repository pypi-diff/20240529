# Comparing `tmp/pyftms-0.2.0.tar.gz` & `tmp/pyftms-0.2.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pyftms-0.2.0.tar", max compression
+gzip compressed data, was "pyftms-0.2.1.tar", max compression
```

## Comparing `pyftms-0.2.0.tar` & `pyftms-0.2.1.tar`

### file list

```diff
@@ -1,40 +1,40 @@
--rw-r--r--   0        0        0    11374 2024-05-29 11:20:47.502093 pyftms-0.2.0/LICENSE
--rw-r--r--   0        0        0      793 2024-05-29 11:20:47.502093 pyftms-0.2.0/README.md
--rw-r--r--   0        0        0     1604 2024-05-29 11:20:47.502093 pyftms-0.2.0/pyftms/__init__.py
--rw-r--r--   0        0        0      939 2024-05-29 11:20:47.502093 pyftms-0.2.0/pyftms/__main__.py
--rw-r--r--   0        0        0     3573 2024-05-29 11:20:47.502093 pyftms-0.2.0/pyftms/client/__init__.py
--rw-r--r--   0        0        0      695 2024-05-29 11:20:47.502093 pyftms-0.2.0/pyftms/client/backends/__init__.py
--rw-r--r--   0        0        0     8214 2024-05-29 11:20:47.502093 pyftms-0.2.0/pyftms/client/backends/controller.py
--rw-r--r--   0        0        0     6245 2024-05-29 11:20:47.502093 pyftms-0.2.0/pyftms/client/backends/event.py
--rw-r--r--   0        0        0     2039 2024-05-29 11:20:47.502093 pyftms-0.2.0/pyftms/client/backends/updater.py
--rw-r--r--   0        0        0    11045 2024-05-29 11:20:47.502093 pyftms-0.2.0/pyftms/client/client.py
--rw-r--r--   0        0        0     4841 2024-05-29 11:20:47.502093 pyftms-0.2.0/pyftms/client/const.py
--rw-r--r--   0        0        0      867 2024-05-29 11:20:47.502093 pyftms-0.2.0/pyftms/client/machines/__init__.py
--rw-r--r--   0        0        0      599 2024-05-29 11:20:47.502093 pyftms-0.2.0/pyftms/client/machines/cross_trainer.py
--rw-r--r--   0        0        0      576 2024-05-29 11:20:47.502093 pyftms-0.2.0/pyftms/client/machines/indoor_bike.py
--rw-r--r--   0        0        0      542 2024-05-29 11:20:47.502093 pyftms-0.2.0/pyftms/client/machines/rower.py
--rw-r--r--   0        0        0      553 2024-05-29 11:20:47.502093 pyftms-0.2.0/pyftms/client/machines/treadmill.py
--rw-r--r--   0        0        0    10069 2024-05-29 11:20:47.502093 pyftms-0.2.0/pyftms/client/manager.py
--rw-r--r--   0        0        0      685 2024-05-29 11:20:47.502093 pyftms-0.2.0/pyftms/client/properties/__init__.py
--rw-r--r--   0        0        0     1216 2024-05-29 11:20:47.502093 pyftms-0.2.0/pyftms/client/properties/device_info.py
--rw-r--r--   0        0        0     5838 2024-05-29 11:20:47.502093 pyftms-0.2.0/pyftms/client/properties/features.py
--rw-r--r--   0        0        0     2448 2024-05-29 11:20:47.502093 pyftms-0.2.0/pyftms/client/properties/machine_type.py
--rw-r--r--   0        0        0     1117 2024-05-29 11:20:47.506093 pyftms-0.2.0/pyftms/models/__init__.py
--rw-r--r--   0        0        0     2530 2024-05-29 11:20:47.506093 pyftms-0.2.0/pyftms/models/common.py
--rw-r--r--   0        0        0     8956 2024-05-29 11:20:47.506093 pyftms-0.2.0/pyftms/models/control_point.py
--rw-r--r--   0        0        0     6446 2024-05-29 11:20:47.506093 pyftms-0.2.0/pyftms/models/machine_status.py
--rw-r--r--   0        0        0      374 2024-05-29 11:20:47.506093 pyftms-0.2.0/pyftms/models/realtime_data/__init__.py
--rw-r--r--   0        0        0     2823 2024-05-29 11:20:47.506093 pyftms-0.2.0/pyftms/models/realtime_data/common.py
--rw-r--r--   0        0        0     3075 2024-05-29 11:20:47.506093 pyftms-0.2.0/pyftms/models/realtime_data/cross_trainer.py
--rw-r--r--   0        0        0     2324 2024-05-29 11:20:47.506093 pyftms-0.2.0/pyftms/models/realtime_data/indoor_bike.py
--rw-r--r--   0        0        0     2973 2024-05-29 11:20:47.506093 pyftms-0.2.0/pyftms/models/realtime_data/rower.py
--rw-r--r--   0        0        0     2701 2024-05-29 11:20:47.506093 pyftms-0.2.0/pyftms/models/realtime_data/treadmill.py
--rw-r--r--   0        0        0     1350 2024-05-29 11:20:47.506093 pyftms-0.2.0/pyftms/models/spin_down.py
--rw-r--r--   0        0        0     2194 2024-05-29 11:20:47.506093 pyftms-0.2.0/pyftms/models/training_status.py
--rw-r--r--   0        0        0      471 2024-05-29 11:20:47.506093 pyftms-0.2.0/pyftms/serializer/__init__.py
--rw-r--r--   0        0        0      783 2024-05-29 11:20:47.506093 pyftms-0.2.0/pyftms/serializer/list.py
--rw-r--r--   0        0        0     7662 2024-05-29 11:20:47.506093 pyftms-0.2.0/pyftms/serializer/model.py
--rw-r--r--   0        0        0     2080 2024-05-29 11:20:47.506093 pyftms-0.2.0/pyftms/serializer/num.py
--rw-r--r--   0        0        0      594 2024-05-29 11:20:47.506093 pyftms-0.2.0/pyftms/serializer/serializer.py
--rw-r--r--   0        0        0      480 2024-05-29 11:20:47.506093 pyftms-0.2.0/pyproject.toml
--rw-r--r--   0        0        0     1289 1970-01-01 00:00:00.000000 pyftms-0.2.0/PKG-INFO
+-rw-r--r--   0        0        0    11374 2024-05-29 18:54:51.042888 pyftms-0.2.1/LICENSE
+-rw-r--r--   0        0        0      792 2024-05-29 18:54:51.042888 pyftms-0.2.1/README.md
+-rw-r--r--   0        0        0     1604 2024-05-29 18:54:51.042888 pyftms-0.2.1/pyftms/__init__.py
+-rw-r--r--   0        0        0      939 2024-05-29 18:54:51.042888 pyftms-0.2.1/pyftms/__main__.py
+-rw-r--r--   0        0        0     3573 2024-05-29 18:54:51.042888 pyftms-0.2.1/pyftms/client/__init__.py
+-rw-r--r--   0        0        0      695 2024-05-29 18:54:51.042888 pyftms-0.2.1/pyftms/client/backends/__init__.py
+-rw-r--r--   0        0        0     8214 2024-05-29 18:54:51.042888 pyftms-0.2.1/pyftms/client/backends/controller.py
+-rw-r--r--   0        0        0     6245 2024-05-29 18:54:51.042888 pyftms-0.2.1/pyftms/client/backends/event.py
+-rw-r--r--   0        0        0     2039 2024-05-29 18:54:51.042888 pyftms-0.2.1/pyftms/client/backends/updater.py
+-rw-r--r--   0        0        0    11045 2024-05-29 18:54:51.042888 pyftms-0.2.1/pyftms/client/client.py
+-rw-r--r--   0        0        0     4841 2024-05-29 18:54:51.042888 pyftms-0.2.1/pyftms/client/const.py
+-rw-r--r--   0        0        0      867 2024-05-29 18:54:51.042888 pyftms-0.2.1/pyftms/client/machines/__init__.py
+-rw-r--r--   0        0        0      599 2024-05-29 18:54:51.042888 pyftms-0.2.1/pyftms/client/machines/cross_trainer.py
+-rw-r--r--   0        0        0      576 2024-05-29 18:54:51.042888 pyftms-0.2.1/pyftms/client/machines/indoor_bike.py
+-rw-r--r--   0        0        0      542 2024-05-29 18:54:51.042888 pyftms-0.2.1/pyftms/client/machines/rower.py
+-rw-r--r--   0        0        0      553 2024-05-29 18:54:51.042888 pyftms-0.2.1/pyftms/client/machines/treadmill.py
+-rw-r--r--   0        0        0    10069 2024-05-29 18:54:51.042888 pyftms-0.2.1/pyftms/client/manager.py
+-rw-r--r--   0        0        0      685 2024-05-29 18:54:51.042888 pyftms-0.2.1/pyftms/client/properties/__init__.py
+-rw-r--r--   0        0        0     1216 2024-05-29 18:54:51.042888 pyftms-0.2.1/pyftms/client/properties/device_info.py
+-rw-r--r--   0        0        0     5838 2024-05-29 18:54:51.042888 pyftms-0.2.1/pyftms/client/properties/features.py
+-rw-r--r--   0        0        0     2448 2024-05-29 18:54:51.042888 pyftms-0.2.1/pyftms/client/properties/machine_type.py
+-rw-r--r--   0        0        0     1117 2024-05-29 18:54:51.042888 pyftms-0.2.1/pyftms/models/__init__.py
+-rw-r--r--   0        0        0     2530 2024-05-29 18:54:51.042888 pyftms-0.2.1/pyftms/models/common.py
+-rw-r--r--   0        0        0     8956 2024-05-29 18:54:51.046888 pyftms-0.2.1/pyftms/models/control_point.py
+-rw-r--r--   0        0        0     6446 2024-05-29 18:54:51.046888 pyftms-0.2.1/pyftms/models/machine_status.py
+-rw-r--r--   0        0        0      374 2024-05-29 18:54:51.046888 pyftms-0.2.1/pyftms/models/realtime_data/__init__.py
+-rw-r--r--   0        0        0     2823 2024-05-29 18:54:51.046888 pyftms-0.2.1/pyftms/models/realtime_data/common.py
+-rw-r--r--   0        0        0     3075 2024-05-29 18:54:51.046888 pyftms-0.2.1/pyftms/models/realtime_data/cross_trainer.py
+-rw-r--r--   0        0        0     2324 2024-05-29 18:54:51.046888 pyftms-0.2.1/pyftms/models/realtime_data/indoor_bike.py
+-rw-r--r--   0        0        0     2973 2024-05-29 18:54:51.046888 pyftms-0.2.1/pyftms/models/realtime_data/rower.py
+-rw-r--r--   0        0        0     2701 2024-05-29 18:54:51.046888 pyftms-0.2.1/pyftms/models/realtime_data/treadmill.py
+-rw-r--r--   0        0        0     1350 2024-05-29 18:54:51.046888 pyftms-0.2.1/pyftms/models/spin_down.py
+-rw-r--r--   0        0        0     2194 2024-05-29 18:54:51.046888 pyftms-0.2.1/pyftms/models/training_status.py
+-rw-r--r--   0        0        0      471 2024-05-29 18:54:51.046888 pyftms-0.2.1/pyftms/serializer/__init__.py
+-rw-r--r--   0        0        0      783 2024-05-29 18:54:51.046888 pyftms-0.2.1/pyftms/serializer/list.py
+-rw-r--r--   0        0        0     7662 2024-05-29 18:54:51.046888 pyftms-0.2.1/pyftms/serializer/model.py
+-rw-r--r--   0        0        0     2080 2024-05-29 18:54:51.046888 pyftms-0.2.1/pyftms/serializer/num.py
+-rw-r--r--   0        0        0      594 2024-05-29 18:54:51.046888 pyftms-0.2.1/pyftms/serializer/serializer.py
+-rw-r--r--   0        0        0      478 2024-05-29 18:54:51.046888 pyftms-0.2.1/pyproject.toml
+-rw-r--r--   0        0        0     1273 1970-01-01 00:00:00.000000 pyftms-0.2.1/PKG-INFO
```

### Comparing `pyftms-0.2.0/LICENSE` & `pyftms-0.2.1/LICENSE`

 * *Files identical despite different names*

### Comparing `pyftms-0.2.0/README.md` & `pyftms-0.2.1/README.md`

 * *Files 18% similar despite different names*

```diff
@@ -6,17 +6,17 @@
  3. **Rower** (Rowing Machine)
  4. **Indoor Bike** (Spin Bike)
 
 **Step Climber** and **Stair Climber** machines are **not supported** due to incomplete protocol information and low popularity.
 
 ## Requirments
 
-1. `python` >= 3.11;
-2. `bleak` >= 0.22;
-3. `bleak-retry-connector` >= 3.5.0.
+1. `python` >=3.11;
+2. `bleak` ==0.22.1;
+3. `bleak-retry-connector` ==3.5.0.
 
 ## Install it from PyPI
 
 ```bash
 pip install pyftms
 ```
```

### Comparing `pyftms-0.2.0/pyftms/__init__.py` & `pyftms-0.2.1/pyftms/__init__.py`

 * *Files identical despite different names*

### Comparing `pyftms-0.2.0/pyftms/__main__.py` & `pyftms-0.2.1/pyftms/__main__.py`

 * *Files identical despite different names*

### Comparing `pyftms-0.2.0/pyftms/client/__init__.py` & `pyftms-0.2.1/pyftms/client/__init__.py`

 * *Files identical despite different names*

### Comparing `pyftms-0.2.0/pyftms/client/backends/__init__.py` & `pyftms-0.2.1/pyftms/client/backends/__init__.py`

 * *Files identical despite different names*

### Comparing `pyftms-0.2.0/pyftms/client/backends/controller.py` & `pyftms-0.2.1/pyftms/client/backends/controller.py`

 * *Files identical despite different names*

### Comparing `pyftms-0.2.0/pyftms/client/backends/event.py` & `pyftms-0.2.1/pyftms/client/backends/event.py`

 * *Files identical despite different names*

### Comparing `pyftms-0.2.0/pyftms/client/backends/updater.py` & `pyftms-0.2.1/pyftms/client/backends/updater.py`

 * *Files identical despite different names*

### Comparing `pyftms-0.2.0/pyftms/client/client.py` & `pyftms-0.2.1/pyftms/client/client.py`

 * *Files identical despite different names*

### Comparing `pyftms-0.2.0/pyftms/client/const.py` & `pyftms-0.2.1/pyftms/client/const.py`

 * *Files identical despite different names*

### Comparing `pyftms-0.2.0/pyftms/client/machines/__init__.py` & `pyftms-0.2.1/pyftms/client/machines/__init__.py`

 * *Files identical despite different names*

### Comparing `pyftms-0.2.0/pyftms/client/machines/cross_trainer.py` & `pyftms-0.2.1/pyftms/client/machines/cross_trainer.py`

 * *Files identical despite different names*

### Comparing `pyftms-0.2.0/pyftms/client/machines/indoor_bike.py` & `pyftms-0.2.1/pyftms/client/machines/indoor_bike.py`

 * *Files identical despite different names*

### Comparing `pyftms-0.2.0/pyftms/client/machines/rower.py` & `pyftms-0.2.1/pyftms/client/machines/rower.py`

 * *Files identical despite different names*

### Comparing `pyftms-0.2.0/pyftms/client/machines/treadmill.py` & `pyftms-0.2.1/pyftms/client/machines/treadmill.py`

 * *Files identical despite different names*

### Comparing `pyftms-0.2.0/pyftms/client/manager.py` & `pyftms-0.2.1/pyftms/client/manager.py`

 * *Files identical despite different names*

### Comparing `pyftms-0.2.0/pyftms/client/properties/__init__.py` & `pyftms-0.2.1/pyftms/client/properties/__init__.py`

 * *Files identical despite different names*

### Comparing `pyftms-0.2.0/pyftms/client/properties/device_info.py` & `pyftms-0.2.1/pyftms/client/properties/device_info.py`

 * *Files identical despite different names*

### Comparing `pyftms-0.2.0/pyftms/client/properties/features.py` & `pyftms-0.2.1/pyftms/client/properties/features.py`

 * *Files identical despite different names*

### Comparing `pyftms-0.2.0/pyftms/client/properties/machine_type.py` & `pyftms-0.2.1/pyftms/client/properties/machine_type.py`

 * *Files identical despite different names*

### Comparing `pyftms-0.2.0/pyftms/models/__init__.py` & `pyftms-0.2.1/pyftms/models/__init__.py`

 * *Files identical despite different names*

### Comparing `pyftms-0.2.0/pyftms/models/common.py` & `pyftms-0.2.1/pyftms/models/common.py`

 * *Files identical despite different names*

### Comparing `pyftms-0.2.0/pyftms/models/control_point.py` & `pyftms-0.2.1/pyftms/models/control_point.py`

 * *Files identical despite different names*

### Comparing `pyftms-0.2.0/pyftms/models/machine_status.py` & `pyftms-0.2.1/pyftms/models/machine_status.py`

 * *Files identical despite different names*

### Comparing `pyftms-0.2.0/pyftms/models/realtime_data/common.py` & `pyftms-0.2.1/pyftms/models/realtime_data/common.py`

 * *Files identical despite different names*

### Comparing `pyftms-0.2.0/pyftms/models/realtime_data/cross_trainer.py` & `pyftms-0.2.1/pyftms/models/realtime_data/cross_trainer.py`

 * *Files identical despite different names*

### Comparing `pyftms-0.2.0/pyftms/models/realtime_data/indoor_bike.py` & `pyftms-0.2.1/pyftms/models/realtime_data/indoor_bike.py`

 * *Files identical despite different names*

### Comparing `pyftms-0.2.0/pyftms/models/realtime_data/rower.py` & `pyftms-0.2.1/pyftms/models/realtime_data/rower.py`

 * *Files identical despite different names*

### Comparing `pyftms-0.2.0/pyftms/models/realtime_data/treadmill.py` & `pyftms-0.2.1/pyftms/models/realtime_data/treadmill.py`

 * *Files identical despite different names*

### Comparing `pyftms-0.2.0/pyftms/models/spin_down.py` & `pyftms-0.2.1/pyftms/models/spin_down.py`

 * *Files identical despite different names*

### Comparing `pyftms-0.2.0/pyftms/models/training_status.py` & `pyftms-0.2.1/pyftms/models/training_status.py`

 * *Files identical despite different names*

### Comparing `pyftms-0.2.0/pyftms/serializer/list.py` & `pyftms-0.2.1/pyftms/serializer/list.py`

 * *Files identical despite different names*

### Comparing `pyftms-0.2.0/pyftms/serializer/model.py` & `pyftms-0.2.1/pyftms/serializer/model.py`

 * *Files identical despite different names*

### Comparing `pyftms-0.2.0/pyftms/serializer/num.py` & `pyftms-0.2.1/pyftms/serializer/num.py`

 * *Files identical despite different names*

### Comparing `pyftms-0.2.0/pyftms/serializer/serializer.py` & `pyftms-0.2.1/pyftms/serializer/serializer.py`

 * *Files identical despite different names*

### Comparing `pyftms-0.2.0/PKG-INFO` & `pyftms-0.2.1/PKG-INFO`

 * *Files 10% similar despite different names*

```diff
@@ -1,36 +1,36 @@
 Metadata-Version: 2.1
 Name: pyftms
-Version: 0.2.0
+Version: 0.2.1
 Summary: PyFTMS - Python Fitness Machine Service client library.
 Author: Sergey V. DUDANOV
 Author-email: sergey.dudanov@gmail.com
 Requires-Python: >=3.11,<3.13
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: Python :: 3.12
-Requires-Dist: bleak (>=0.22.1,<0.23.0)
-Requires-Dist: bleak-retry-connector (>=3.5.0,<4.0.0)
+Requires-Dist: bleak (==0.22.1)
+Requires-Dist: bleak-retry-connector (==3.5.0)
 Description-Content-Type: text/markdown
 
 # PyFTMS - Python Fitness Machine Service client library
 
 **PyFTMS** is a Python client library for the **FTMS service**, which is a standard for fitness equipment with a Bluetooth interface. **Bleak** is used as the Bluetooth library. Currently four main types of fitness machines are supported:
  1. **Treadmill**
  2. **Cross Trainer** (Elliptical Trainer)
  3. **Rower** (Rowing Machine)
  4. **Indoor Bike** (Spin Bike)
 
 **Step Climber** and **Stair Climber** machines are **not supported** due to incomplete protocol information and low popularity.
 
 ## Requirments
 
-1. `python` >= 3.11;
-2. `bleak` >= 0.22;
-3. `bleak-retry-connector` >= 3.5.0.
+1. `python` >=3.11;
+2. `bleak` ==0.22.1;
+3. `bleak-retry-connector` ==3.5.0.
 
 ## Install it from PyPI
 
 ```bash
 pip install pyftms
 ```
```

