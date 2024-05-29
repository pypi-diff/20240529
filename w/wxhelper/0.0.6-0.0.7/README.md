# Comparing `tmp/wxhelper-0.0.6.tar.gz` & `tmp/wxhelper-0.0.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "wxhelper-0.0.6.tar", last modified: Tue May 28 09:46:39 2024, max compression
+gzip compressed data, was "wxhelper-0.0.7.tar", last modified: Wed May 29 09:58:13 2024, max compression
```

## Comparing `wxhelper-0.0.6.tar` & `wxhelper-0.0.7.tar`

### file list

```diff
@@ -1,24 +1,26 @@
-drwxrwxrwx   0        0        0        0 2024-05-28 09:46:39.409824 wxhelper-0.0.6/
--rw-rw-rw-   0        0        0     1077 2024-05-14 05:57:33.000000 wxhelper-0.0.6/LICENSE
--rw-rw-rw-   0        0        0       53 2024-05-14 05:57:33.000000 wxhelper-0.0.6/MANIFEST.in
--rw-rw-rw-   0        0        0     3652 2024-05-28 09:46:39.408831 wxhelper-0.0.6/PKG-INFO
--rw-rw-rw-   0        0        0     2904 2024-05-14 05:57:33.000000 wxhelper-0.0.6/README.md
--rw-rw-rw-   0        0        0       42 2024-05-28 09:46:39.409824 wxhelper-0.0.6/setup.cfg
--rw-rw-rw-   0        0        0     3932 2024-05-28 09:46:31.000000 wxhelper-0.0.6/setup.py
-drwxrwxrwx   0        0        0        0 2024-05-28 09:46:39.400821 wxhelper-0.0.6/wxhelper/
--rw-rw-rw-   0        0        0       44 2024-05-28 09:46:31.000000 wxhelper-0.0.6/wxhelper/__init__.py
--rw-rw-rw-   0        0        0    21463 2024-05-28 09:46:31.000000 wxhelper-0.0.6/wxhelper/core.py
--rw-rw-rw-   0        0        0      630 2024-05-14 05:57:33.000000 wxhelper-0.0.6/wxhelper/events.py
--rw-rw-rw-   0        0        0      314 2024-05-14 05:57:33.000000 wxhelper-0.0.6/wxhelper/logger.py
--rw-rw-rw-   0        0        0     2693 2024-05-14 09:19:20.000000 wxhelper-0.0.6/wxhelper/model.py
-drwxrwxrwx   0        0        0        0 2024-05-28 09:46:39.407822 wxhelper-0.0.6/wxhelper/tools/
--rwxrwxrwx   0        0        0   270336 2024-05-14 05:57:33.000000 wxhelper-0.0.6/wxhelper/tools/faker.exe
--rwxrwxrwx   0        0        0   888832 2024-05-14 05:57:33.000000 wxhelper-0.0.6/wxhelper/tools/start-wechat.exe
--rw-rw-rw-   0        0        0   489984 2024-05-14 05:57:33.000000 wxhelper-0.0.6/wxhelper/tools/wxhelper.dll
--rw-rw-rw-   0        0        0     3789 2024-05-14 05:57:33.000000 wxhelper-0.0.6/wxhelper/utils.py
-drwxrwxrwx   0        0        0        0 2024-05-28 09:46:39.404821 wxhelper-0.0.6/wxhelper.egg-info/
--rw-rw-rw-   0        0        0     3652 2024-05-28 09:46:39.000000 wxhelper-0.0.6/wxhelper.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      394 2024-05-28 09:46:39.000000 wxhelper-0.0.6/wxhelper.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-05-28 09:46:39.000000 wxhelper-0.0.6/wxhelper.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       38 2024-05-28 09:46:39.000000 wxhelper-0.0.6/wxhelper.egg-info/requires.txt
--rw-rw-rw-   0        0        0        9 2024-05-28 09:46:39.000000 wxhelper-0.0.6/wxhelper.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2024-05-29 09:58:13.870849 wxhelper-0.0.7/
+-rw-rw-rw-   0        0        0     1077 2024-05-14 05:57:33.000000 wxhelper-0.0.7/LICENSE
+-rw-rw-rw-   0        0        0       53 2024-05-14 05:57:33.000000 wxhelper-0.0.7/MANIFEST.in
+-rw-rw-rw-   0        0        0     3652 2024-05-29 09:58:13.869850 wxhelper-0.0.7/PKG-INFO
+-rw-rw-rw-   0        0        0     2904 2024-05-14 05:57:33.000000 wxhelper-0.0.7/README.md
+-rw-rw-rw-   0        0        0       42 2024-05-29 09:58:13.870849 wxhelper-0.0.7/setup.cfg
+-rw-rw-rw-   0        0        0     3932 2024-05-29 09:55:13.000000 wxhelper-0.0.7/setup.py
+drwxrwxrwx   0        0        0        0 2024-05-29 09:58:13.856801 wxhelper-0.0.7/wxhelper/
+-rw-rw-rw-   0        0        0       44 2024-05-29 09:55:13.000000 wxhelper-0.0.7/wxhelper/__init__.py
+-rw-rw-rw-   0        0        0    21463 2024-05-28 09:46:31.000000 wxhelper-0.0.7/wxhelper/core.py
+-rw-rw-rw-   0        0        0      630 2024-05-14 05:57:33.000000 wxhelper-0.0.7/wxhelper/events.py
+-rw-rw-rw-   0        0        0      314 2024-05-14 05:57:33.000000 wxhelper-0.0.7/wxhelper/logger.py
+-rw-rw-rw-   0        0        0     2733 2024-05-29 09:48:16.000000 wxhelper-0.0.7/wxhelper/model.py
+drwxrwxrwx   0        0        0        0 2024-05-29 09:58:13.868852 wxhelper-0.0.7/wxhelper/tools/
+-rw-rw-rw-   0        0        0       22 2024-05-29 09:51:35.000000 wxhelper-0.0.7/wxhelper/tools/config.ini
+-rwxrwxrwx   0        0        0   270336 2024-05-14 05:57:33.000000 wxhelper-0.0.7/wxhelper/tools/faker.exe
+-rwxrwxrwx   0        0        0   888832 2024-05-14 05:57:33.000000 wxhelper-0.0.7/wxhelper/tools/start-wechat.exe
+-rw-rw-rw-   0        0        0   489984 2024-05-14 05:57:33.000000 wxhelper-0.0.7/wxhelper/tools/wxhelper.dll
+-rw-rw-rw-   0        0        0      103 2024-05-29 09:51:35.000000 wxhelper-0.0.7/wxhelper/tools/wxhelper.json
+-rw-rw-rw-   0        0        0     3789 2024-05-14 05:57:33.000000 wxhelper-0.0.7/wxhelper/utils.py
+drwxrwxrwx   0        0        0        0 2024-05-29 09:58:13.861828 wxhelper-0.0.7/wxhelper.egg-info/
+-rw-rw-rw-   0        0        0     3652 2024-05-29 09:58:13.000000 wxhelper-0.0.7/wxhelper.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      449 2024-05-29 09:58:13.000000 wxhelper-0.0.7/wxhelper.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-05-29 09:58:13.000000 wxhelper-0.0.7/wxhelper.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       38 2024-05-29 09:58:13.000000 wxhelper-0.0.7/wxhelper.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        9 2024-05-29 09:58:13.000000 wxhelper-0.0.7/wxhelper.egg-info/top_level.txt
```

### Comparing `wxhelper-0.0.6/LICENSE` & `wxhelper-0.0.7/LICENSE`

 * *Files identical despite different names*

### Comparing `wxhelper-0.0.6/PKG-INFO` & `wxhelper-0.0.7/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: wxhelper
-Version: 0.0.6
+Version: 0.0.7
 Summary: wechat robot framework.
 Home-page: https://github.com/miloira/wxhelper
 Author: Msky
 Author-email: 690126048@qq.com
 License: MIT
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python
```

### Comparing `wxhelper-0.0.6/README.md` & `wxhelper-0.0.7/README.md`

 * *Files identical despite different names*

### Comparing `wxhelper-0.0.6/setup.py` & `wxhelper-0.0.7/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -14,15 +14,15 @@
 # Package meta-data.
 NAME = 'wxhelper'
 DESCRIPTION = 'wechat robot framework.'
 URL = 'https://github.com/miloira/wxhelper'
 EMAIL = '690126048@qq.com'
 AUTHOR = 'Msky'
 REQUIRES_PYTHON = '>=3.8.0'
-VERSION = '0.0.6'
+VERSION = '0.0.7'
 
 # What packages are required for this module to be executed?
 REQUIRED = [
     'loguru',
     'psutil',
     'pyee',
     'requests',
```

### Comparing `wxhelper-0.0.6/wxhelper/core.py` & `wxhelper-0.0.7/wxhelper/core.py`

 * *Files identical despite different names*

### Comparing `wxhelper-0.0.6/wxhelper/events.py` & `wxhelper-0.0.7/wxhelper/events.py`

 * *Files identical despite different names*

### Comparing `wxhelper-0.0.6/wxhelper/model.py` & `wxhelper-0.0.7/wxhelper/model.py`

 * *Files 2% similar despite different names*

```diff
@@ -16,14 +16,15 @@
     thumbPath: typing.Optional[str] = None
     pid: typing.Optional[int] = None
     sign: typing.Optional[str] = None
     signature: typing.Optional[str] = None
     time: typing.Optional[str] = None
     timestamp: typing.Optional[int] = None
     type: typing.Optional[int] = None
+    data: typing.Optional[list] = None
 
 
 @dataclass
 class Account:
     """用户"""
     account: str
     city: str
```

### Comparing `wxhelper-0.0.6/wxhelper/tools/faker.exe` & `wxhelper-0.0.7/wxhelper/tools/faker.exe`

 * *Files identical despite different names*

### Comparing `wxhelper-0.0.6/wxhelper/tools/start-wechat.exe` & `wxhelper-0.0.7/wxhelper/tools/start-wechat.exe`

 * *Files identical despite different names*

### Comparing `wxhelper-0.0.6/wxhelper/tools/wxhelper.dll` & `wxhelper-0.0.7/wxhelper/tools/wxhelper.dll`

 * *Files identical despite different names*

### Comparing `wxhelper-0.0.6/wxhelper/utils.py` & `wxhelper-0.0.7/wxhelper/utils.py`

 * *Files identical despite different names*

### Comparing `wxhelper-0.0.6/wxhelper.egg-info/PKG-INFO` & `wxhelper-0.0.7/wxhelper.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: wxhelper
-Version: 0.0.6
+Version: 0.0.7
 Summary: wechat robot framework.
 Home-page: https://github.com/miloira/wxhelper
 Author: Msky
 Author-email: 690126048@qq.com
 License: MIT
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python
```

