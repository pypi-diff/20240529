# Comparing `tmp/TineAutomationToolkit-1.1.1.tar.gz` & `tmp/TineAutomationToolkit-1.1.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist\TineAutomationToolkit-1.1.1.tar", last modified: Thu May  9 06:27:09 2024, max compression
+gzip compressed data, was "dist\TineAutomationToolkit-1.1.2.tar", last modified: Wed May 29 04:24:11 2024, max compression
```

## Comparing `TineAutomationToolkit-1.1.1.tar` & `TineAutomationToolkit-1.1.2.tar`

### file list

```diff
@@ -1,27 +1,28 @@
-drwxrwxrwx   0        0        0        0 2024-05-09 06:27:09.000000 TineAutomationToolkit-1.1.1/
--rw-rw-rw-   0        0        0     2280 2024-05-09 06:27:09.000000 TineAutomationToolkit-1.1.1/PKG-INFO
--rw-rw-rw-   0        0        0     1623 2024-03-15 00:45:23.000000 TineAutomationToolkit-1.1.1/README.md
-drwxrwxrwx   0        0        0        0 2024-05-09 06:27:09.000000 TineAutomationToolkit-1.1.1/TineAutomationToolkit/
--rw-rw-rw-   0        0        0      403 2024-04-25 03:30:22.000000 TineAutomationToolkit-1.1.1/TineAutomationToolkit/__init__.py
-drwxrwxrwx   0        0        0        0 2024-05-09 06:27:09.000000 TineAutomationToolkit-1.1.1/TineAutomationToolkit/detect/
--rw-rw-rw-   0        0        0       99 2024-04-10 08:38:20.000000 TineAutomationToolkit-1.1.1/TineAutomationToolkit/detect/__init__.py
--rw-rw-rw-   0        0        0     4950 2024-04-10 09:28:36.000000 TineAutomationToolkit-1.1.1/TineAutomationToolkit/detect/detectelement.py
-drwxrwxrwx   0        0        0        0 2024-05-09 06:27:09.000000 TineAutomationToolkit-1.1.1/TineAutomationToolkit/keywords/
--rw-rw-rw-   0        0        0      812 2024-04-25 03:30:23.000000 TineAutomationToolkit-1.1.1/TineAutomationToolkit/keywords/__init__.py
--rw-rw-rw-   0        0        0     3371 2024-03-19 02:54:39.000000 TineAutomationToolkit-1.1.1/TineAutomationToolkit/keywords/capturescreenshot.py
--rw-rw-rw-   0        0        0     5502 2024-05-09 06:26:49.000000 TineAutomationToolkit-1.1.1/TineAutomationToolkit/keywords/connectionmanagement.py
--rw-rw-rw-   0        0        0    18183 2024-04-19 08:45:03.000000 TineAutomationToolkit-1.1.1/TineAutomationToolkit/keywords/controlelement.py
--rw-rw-rw-   0        0        0     4388 2024-05-08 03:58:42.000000 TineAutomationToolkit-1.1.1/TineAutomationToolkit/keywords/convertobject.py
--rw-rw-rw-   0        0        0     2495 2024-04-17 15:53:57.000000 TineAutomationToolkit-1.1.1/TineAutomationToolkit/keywords/keyevent.py
--rw-rw-rw-   0        0        0     3474 2024-03-19 03:06:11.000000 TineAutomationToolkit-1.1.1/TineAutomationToolkit/keywords/scroll.py
--rw-rw-rw-   0        0        0      237 2024-03-14 00:55:44.000000 TineAutomationToolkit-1.1.1/TineAutomationToolkit/keywords/toolkitstest.py
--rw-rw-rw-   0        0        0     2444 2024-04-17 15:25:52.000000 TineAutomationToolkit-1.1.1/TineAutomationToolkit/keywords/touch.py
--rw-rw-rw-   0        0        0    10151 2024-05-08 03:55:50.000000 TineAutomationToolkit-1.1.1/TineAutomationToolkit/keywords/waitingelement.py
-drwxrwxrwx   0        0        0        0 2024-05-09 06:27:09.000000 TineAutomationToolkit-1.1.1/TineAutomationToolkit.egg-info/
--rw-rw-rw-   0        0        0     2280 2024-05-09 06:27:08.000000 TineAutomationToolkit-1.1.1/TineAutomationToolkit.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      830 2024-05-09 06:27:09.000000 TineAutomationToolkit-1.1.1/TineAutomationToolkit.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-05-09 06:27:08.000000 TineAutomationToolkit-1.1.1/TineAutomationToolkit.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       25 2024-05-09 06:27:08.000000 TineAutomationToolkit-1.1.1/TineAutomationToolkit.egg-info/requires.txt
--rw-rw-rw-   0        0        0       22 2024-05-09 06:27:08.000000 TineAutomationToolkit-1.1.1/TineAutomationToolkit.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2024-05-09 06:27:09.000000 TineAutomationToolkit-1.1.1/setup.cfg
--rw-rw-rw-   0        0        0      755 2024-05-09 06:16:48.000000 TineAutomationToolkit-1.1.1/setup.py
+drwxrwxrwx   0        0        0        0 2024-05-29 04:24:11.000000 TineAutomationToolkit-1.1.2/
+-rw-rw-rw-   0        0        0     2280 2024-05-29 04:24:11.000000 TineAutomationToolkit-1.1.2/PKG-INFO
+-rw-rw-rw-   0        0        0     1623 2024-03-15 00:45:23.000000 TineAutomationToolkit-1.1.2/README.md
+drwxrwxrwx   0        0        0        0 2024-05-29 04:24:11.000000 TineAutomationToolkit-1.1.2/TineAutomationToolkit/
+-rw-rw-rw-   0        0        0      403 2024-04-25 03:30:22.000000 TineAutomationToolkit-1.1.2/TineAutomationToolkit/__init__.py
+drwxrwxrwx   0        0        0        0 2024-05-29 04:24:11.000000 TineAutomationToolkit-1.1.2/TineAutomationToolkit/detect/
+-rw-rw-rw-   0        0        0       99 2024-04-10 08:38:20.000000 TineAutomationToolkit-1.1.2/TineAutomationToolkit/detect/__init__.py
+-rw-rw-rw-   0        0        0     5072 2024-05-16 10:19:22.000000 TineAutomationToolkit-1.1.2/TineAutomationToolkit/detect/detectelement.py
+-rw-rw-rw-   0        0        0     3202 2024-05-29 04:19:10.000000 TineAutomationToolkit-1.1.2/TineAutomationToolkit/detect/flutterfinderelement.py
+drwxrwxrwx   0        0        0        0 2024-05-29 04:24:11.000000 TineAutomationToolkit-1.1.2/TineAutomationToolkit/keywords/
+-rw-rw-rw-   0        0        0      812 2024-04-25 03:30:23.000000 TineAutomationToolkit-1.1.2/TineAutomationToolkit/keywords/__init__.py
+-rw-rw-rw-   0        0        0     3371 2024-03-19 02:54:39.000000 TineAutomationToolkit-1.1.2/TineAutomationToolkit/keywords/capturescreenshot.py
+-rw-rw-rw-   0        0        0     5502 2024-05-09 06:28:44.000000 TineAutomationToolkit-1.1.2/TineAutomationToolkit/keywords/connectionmanagement.py
+-rw-rw-rw-   0        0        0    18691 2024-05-29 04:20:29.000000 TineAutomationToolkit-1.1.2/TineAutomationToolkit/keywords/controlelement.py
+-rw-rw-rw-   0        0        0     5259 2024-05-29 04:22:39.000000 TineAutomationToolkit-1.1.2/TineAutomationToolkit/keywords/convertobject.py
+-rw-rw-rw-   0        0        0     2495 2024-04-17 15:53:57.000000 TineAutomationToolkit-1.1.2/TineAutomationToolkit/keywords/keyevent.py
+-rw-rw-rw-   0        0        0     3474 2024-03-19 03:06:11.000000 TineAutomationToolkit-1.1.2/TineAutomationToolkit/keywords/scroll.py
+-rw-rw-rw-   0        0        0      237 2024-03-14 00:55:44.000000 TineAutomationToolkit-1.1.2/TineAutomationToolkit/keywords/toolkitstest.py
+-rw-rw-rw-   0        0        0     2444 2024-04-17 15:25:52.000000 TineAutomationToolkit-1.1.2/TineAutomationToolkit/keywords/touch.py
+-rw-rw-rw-   0        0        0    10151 2024-05-08 03:55:50.000000 TineAutomationToolkit-1.1.2/TineAutomationToolkit/keywords/waitingelement.py
+drwxrwxrwx   0        0        0        0 2024-05-29 04:24:11.000000 TineAutomationToolkit-1.1.2/TineAutomationToolkit.egg-info/
+-rw-rw-rw-   0        0        0     2280 2024-05-29 04:24:11.000000 TineAutomationToolkit-1.1.2/TineAutomationToolkit.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      883 2024-05-29 04:24:11.000000 TineAutomationToolkit-1.1.2/TineAutomationToolkit.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-05-29 04:24:11.000000 TineAutomationToolkit-1.1.2/TineAutomationToolkit.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       25 2024-05-29 04:24:11.000000 TineAutomationToolkit-1.1.2/TineAutomationToolkit.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       22 2024-05-29 04:24:11.000000 TineAutomationToolkit-1.1.2/TineAutomationToolkit.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2024-05-29 04:24:11.000000 TineAutomationToolkit-1.1.2/setup.cfg
+-rw-rw-rw-   0        0        0      755 2024-05-29 04:20:36.000000 TineAutomationToolkit-1.1.2/setup.py
```

### Comparing `TineAutomationToolkit-1.1.1/PKG-INFO` & `TineAutomationToolkit-1.1.2/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: TineAutomationToolkit
-Version: 1.1.1
+Version: 1.1.2
 Summary: Test Library for TineAutomationToolkit
 Home-page: https://github.com/pornpawit08/TineAutomationToolkit.git
 Author: Pornpawit Suttha
 Author-email: pornpawit14suttha@gmail.com
 License: UNKNOWN
 Description: # TineAutomationToolkit
         TineAutomationToolkit is a comprehensive automation toolkit designed to streamline and enhance the testing and development process for mobile applications. With a focus on integrating seamlessly with Appium and Flutter, this toolkit provides a robust set of tools and utilities to simplify the automation of mobile app testing.
```

### Comparing `TineAutomationToolkit-1.1.1/README.md` & `TineAutomationToolkit-1.1.2/README.md`

 * *Files identical despite different names*

### Comparing `TineAutomationToolkit-1.1.1/TineAutomationToolkit/detect/detectelement.py` & `TineAutomationToolkit-1.1.2/TineAutomationToolkit/detect/detectelement.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,14 +1,15 @@
 # -*- coding: utf-8 -*-
-from appium_flutter_finder import FlutterElement , FlutterFinder
+# from appium_flutter_finder import FlutterElement , FlutterFinder
 from AppiumLibrary import utils
 from appium.webdriver.common.appiumby import AppiumBy
 from robot.api import logger
+from TineAutomationToolkit.detect.flutterfinderelement import FlutterDetectElement , FlutterFinderElement
 
-detect_element = FlutterFinder()
+detect_element = FlutterFinderElement()
 # strategies = {
 #     'default': _find_by_default,
 #     'id': _find_by_id,
 #     'key': _find_by_key,
 #  }
 
 
@@ -53,15 +54,15 @@
         # different and inside appium python client. Need to expose these and improve in order to make
         # _find_by_key_attrs useful.
         # return self._find_by_id(application, criteria, tag, constraints)
         return self._find_by_key(application, criteria, tag, constraints)
     
     def _find_by_key(self, application, element_key, tag, constraints):
         finder_key = detect_element.by_value_key(element_key)
-        element = FlutterElement(application, finder_key)
+        element = FlutterDetectElement(application, finder_key)
 
         return element
     
     def _find_by_xpath(self, application, criteria, tag, constraints):
         print(f"xpath criteria: {criteria}")
         return self._filter_elements(
             application.find_elements(by=AppiumBy.XPATH, value=criteria),
```

### Comparing `TineAutomationToolkit-1.1.1/TineAutomationToolkit/keywords/__init__.py` & `TineAutomationToolkit-1.1.2/TineAutomationToolkit/keywords/__init__.py`

 * *Files identical despite different names*

### Comparing `TineAutomationToolkit-1.1.1/TineAutomationToolkit/keywords/capturescreenshot.py` & `TineAutomationToolkit-1.1.2/TineAutomationToolkit/keywords/capturescreenshot.py`

 * *Files identical despite different names*

### Comparing `TineAutomationToolkit-1.1.1/TineAutomationToolkit/keywords/connectionmanagement.py` & `TineAutomationToolkit-1.1.2/TineAutomationToolkit/keywords/connectionmanagement.py`

 * *Files identical despite different names*

### Comparing `TineAutomationToolkit-1.1.1/TineAutomationToolkit/keywords/controlelement.py` & `TineAutomationToolkit-1.1.2/TineAutomationToolkit/keywords/controlelement.py`

 * *Files 1% similar despite different names*

```diff
@@ -304,16 +304,16 @@
         - ชื่อถูกเปลี่ยนจาก `Get Elements` เป็นชื่อปัจจุบัน
         - อาร์กิวเมนต์ที่ไม่แนะนำอีกต่อไป ``fail_on_error``, ใช้ `Run Keyword and Ignore Error` ถ้าจำเป็น
 
         ใหม่ใน AppiumLibrary 1.4
         """
         return self._element_find_t(locator, False, True)
 
-    #Flutter
-
+    #Flutter (Not available , อยู่ในช่วงทดสอบ ยังไม่สามารถใช้งานได้)
+    
     def flutter_get_element_attribute(self, locator, attribute):
         """ *******Not available wait for update flutter*******
 
         Because FinderType is Limited
 
         Get element attribute using given attribute: name, value,...
 
@@ -332,14 +332,25 @@
 
         try:
             attr_val = elements[0].get_attribute(attribute)
             log._info("Element '%s' attribute '%s' value '%s' " % (locator, attribute, attr_val))
             return attr_val
         except:
             raise AssertionError("Attribute '%s' is not valid for element '%s'" % (attribute, locator))
+        
+    def flutter_check_element_enable(self,locator):
+        """ *******Not available wait for update flutter*******
+
+        Get element enable 
+
+        Examples:
+
+        | Check Element Enable | locator |
+        """
+        print("ยังอยู่ในช่วงทดสอบ ยังไม่สามารถใช้งานได้")
     
     #PRIVATE_FUNCTION
 
     def _element_find_flutter(self, locator, first_only, required, tag=None):
         application = cache_app._current_application()
         elements = None
         if isstr(locator):
```

### Comparing `TineAutomationToolkit-1.1.1/TineAutomationToolkit/keywords/convertobject.py` & `TineAutomationToolkit-1.1.2/TineAutomationToolkit/keywords/convertobject.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,12 +1,14 @@
 # -*- coding: utf-8 -*-
 import bson
 import logging
 import pytz
 import re
+import base64
+import json
 
 from datetime import datetime
 
 class ConvertObject:
 
     def __init__(self):
         #เนื่องจากปัญหาเรื่องโครงสร้าง structure เลยยังไม่สามารถใช้ได้
@@ -66,14 +68,32 @@
                 raise ValueError("Invalid date format. Please provide the date in the format 'YYYY-MM-DDTHH:MM:SS.sss+HH:MM'")
         
             # แปลง string เป็น datetime object
             date_time = datetime.fromisoformat(date)
             local_date_time = date_time.astimezone(local_timezone)
         
         return local_date_time
+    
+    #(ยังใช้ไม่ได้อยู่ในช่วงทดสอบ)
+    def convert_get_render_tree_to_json(self,tree):
+        """ Owner : pornpawit.s@chareontut.co.th
+        ***|    Description     |***
+        |   มีไว้สำหรับนำข้อมูล get render tree แปลง
+        |   เป็น json (ยังใช้ไม่ได้อยู่ในช่วงทดสอบ)
+        """
+        # แปลงข้อมูล Render Tree เป็น JSON
+        render_tree_json = json.dumps(tree, indent=4)
+        with open('render_tree.json', 'w') as json_file:
+            json_file.write(render_tree_json)
+        
+        with open('render_tree.json', 'r') as json_file:
+            data = json.load(json_file)
+            print(data)
+        
+
 
     #Private Function
 
     def _tree_structure(self, data, level=0, prefix=''):
         indent = "│   " * level
         branch = "├── " if level > 0 else ""
         if isinstance(data, dict):
```

### Comparing `TineAutomationToolkit-1.1.1/TineAutomationToolkit/keywords/keyevent.py` & `TineAutomationToolkit-1.1.2/TineAutomationToolkit/keywords/keyevent.py`

 * *Files identical despite different names*

### Comparing `TineAutomationToolkit-1.1.1/TineAutomationToolkit/keywords/scroll.py` & `TineAutomationToolkit-1.1.2/TineAutomationToolkit/keywords/scroll.py`

 * *Files identical despite different names*

### Comparing `TineAutomationToolkit-1.1.1/TineAutomationToolkit/keywords/touch.py` & `TineAutomationToolkit-1.1.2/TineAutomationToolkit/keywords/touch.py`

 * *Files identical despite different names*

### Comparing `TineAutomationToolkit-1.1.1/TineAutomationToolkit/keywords/waitingelement.py` & `TineAutomationToolkit-1.1.2/TineAutomationToolkit/keywords/waitingelement.py`

 * *Files identical despite different names*

### Comparing `TineAutomationToolkit-1.1.1/TineAutomationToolkit.egg-info/PKG-INFO` & `TineAutomationToolkit-1.1.2/TineAutomationToolkit.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: TineAutomationToolkit
-Version: 1.1.1
+Version: 1.1.2
 Summary: Test Library for TineAutomationToolkit
 Home-page: https://github.com/pornpawit08/TineAutomationToolkit.git
 Author: Pornpawit Suttha
 Author-email: pornpawit14suttha@gmail.com
 License: UNKNOWN
 Description: # TineAutomationToolkit
         TineAutomationToolkit is a comprehensive automation toolkit designed to streamline and enhance the testing and development process for mobile applications. With a focus on integrating seamlessly with Appium and Flutter, this toolkit provides a robust set of tools and utilities to simplify the automation of mobile app testing.
```

### Comparing `TineAutomationToolkit-1.1.1/TineAutomationToolkit.egg-info/SOURCES.txt` & `TineAutomationToolkit-1.1.2/TineAutomationToolkit.egg-info/SOURCES.txt`

 * *Files 17% similar despite different names*

```diff
@@ -4,14 +4,15 @@
 TineAutomationToolkit.egg-info/PKG-INFO
 TineAutomationToolkit.egg-info/SOURCES.txt
 TineAutomationToolkit.egg-info/dependency_links.txt
 TineAutomationToolkit.egg-info/requires.txt
 TineAutomationToolkit.egg-info/top_level.txt
 TineAutomationToolkit/detect/__init__.py
 TineAutomationToolkit/detect/detectelement.py
+TineAutomationToolkit/detect/flutterfinderelement.py
 TineAutomationToolkit/keywords/__init__.py
 TineAutomationToolkit/keywords/capturescreenshot.py
 TineAutomationToolkit/keywords/connectionmanagement.py
 TineAutomationToolkit/keywords/controlelement.py
 TineAutomationToolkit/keywords/convertobject.py
 TineAutomationToolkit/keywords/keyevent.py
 TineAutomationToolkit/keywords/scroll.py
```

### Comparing `TineAutomationToolkit-1.1.1/setup.py` & `TineAutomationToolkit-1.1.2/setup.py`

 * *Files 15% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from setuptools import setup, find_packages
 
 setup(
     name="TineAutomationToolkit",
-    version="1.1.1",
+    version="1.1.2",
     author="Pornpawit Suttha",
     author_email="pornpawit14suttha@gmail.com",
     description="Test Library for TineAutomationToolkit",
     long_description=open('README.md', encoding='utf-8').read(),
     long_description_content_type="text/markdown",
     url="https://github.com/pornpawit08/TineAutomationToolkit.git",
     packages=find_packages(),
```

