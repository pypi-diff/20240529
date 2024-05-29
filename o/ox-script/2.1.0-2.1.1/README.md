# Comparing `tmp/ox_script-2.1.0.tar.gz` & `tmp/ox_script-2.1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ox_script-2.1.0.tar", last modified: Tue May 28 20:12:42 2024, max compression
+gzip compressed data, was "ox_script-2.1.1.tar", last modified: Wed May 29 08:54:15 2024, max compression
```

## Comparing `ox_script-2.1.0.tar` & `ox_script-2.1.1.tar`

### file list

```diff
@@ -1,15 +1,15 @@
-drwxr-xr-x   0 jarvislu   (501) staff       (20)        0 2024-05-28 20:12:42.068400 ox_script-2.1.0/
--rw-r--r--   0 jarvislu   (501) staff       (20)       13 2023-04-22 17:32:02.000000 ox_script-2.1.0/MANIFEST.in
--rw-r--r--   0 jarvislu   (501) staff       (20)      939 2024-05-28 20:12:42.068094 ox_script-2.1.0/PKG-INFO
-drwxr-xr-x   0 jarvislu   (501) staff       (20)        0 2024-05-28 20:12:42.066436 ox_script-2.1.0/ox_script/
--rw-r--r--   0 jarvislu   (501) staff       (20)       72 2023-04-22 22:41:41.000000 ox_script-2.1.0/ox_script/__init__.py
--rw-------   0 jarvislu   (501) staff       (20)    12256 2023-04-26 16:53:14.000000 ox_script-2.1.0/ox_script/general_purpose_apis.py
--rw-------   0 jarvislu   (501) staff       (20)    36820 2023-04-26 18:04:03.000000 ox_script-2.1.0/ox_script/printer_specific_apis.py
-drwxr-xr-x   0 jarvislu   (501) staff       (20)        0 2024-05-28 20:12:42.067748 ox_script-2.1.0/ox_script.egg-info/
--rw-r--r--   0 jarvislu   (501) staff       (20)      939 2024-05-28 20:12:42.000000 ox_script-2.1.0/ox_script.egg-info/PKG-INFO
--rw-r--r--   0 jarvislu   (501) staff       (20)      275 2024-05-28 20:12:42.000000 ox_script-2.1.0/ox_script.egg-info/SOURCES.txt
--rw-r--r--   0 jarvislu   (501) staff       (20)        1 2024-05-28 20:12:42.000000 ox_script-2.1.0/ox_script.egg-info/dependency_links.txt
--rw-r--r--   0 jarvislu   (501) staff       (20)       16 2024-05-28 20:12:42.000000 ox_script-2.1.0/ox_script.egg-info/requires.txt
--rw-r--r--   0 jarvislu   (501) staff       (20)       10 2024-05-28 20:12:42.000000 ox_script-2.1.0/ox_script.egg-info/top_level.txt
--rw-r--r--   0 jarvislu   (501) staff       (20)       38 2024-05-28 20:12:42.068456 ox_script-2.1.0/setup.cfg
--rw-r--r--   0 jarvislu   (501) staff       (20)     1497 2024-05-28 20:12:37.000000 ox_script-2.1.0/setup.py
+drwxrwxrwx   0        0        0        0 2024-05-29 08:54:15.164136 ox_script-2.1.1/
+-rw-rw-rw-   0        0        0       14 2024-05-29 07:34:20.000000 ox_script-2.1.1/MANIFEST.in
+-rw-rw-rw-   0        0        0      905 2024-05-29 08:54:15.164136 ox_script-2.1.1/PKG-INFO
+drwxrwxrwx   0        0        0        0 2024-05-29 08:54:15.157843 ox_script-2.1.1/ox_script/
+-rw-rw-rw-   0        0        0       73 2024-05-29 07:34:20.000000 ox_script-2.1.1/ox_script/__init__.py
+-rw-rw-rw-   0        0        0     8147 2024-05-29 08:19:08.000000 ox_script-2.1.1/ox_script/general_purpose_apis.py
+-rw-rw-rw-   0        0        0    63272 2024-05-29 08:54:03.000000 ox_script-2.1.1/ox_script/printer_specific_apis.py
+drwxrwxrwx   0        0        0        0 2024-05-29 08:54:15.163137 ox_script-2.1.1/ox_script.egg-info/
+-rw-rw-rw-   0        0        0      905 2024-05-29 08:54:15.000000 ox_script-2.1.1/ox_script.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      275 2024-05-29 08:54:15.000000 ox_script-2.1.1/ox_script.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-05-29 08:54:15.000000 ox_script-2.1.1/ox_script.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       16 2024-05-29 08:54:15.000000 ox_script-2.1.1/ox_script.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       10 2024-05-29 08:54:15.000000 ox_script-2.1.1/ox_script.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2024-05-29 08:54:15.164136 ox_script-2.1.1/setup.cfg
+-rw-rw-rw-   0        0        0     1517 2024-05-29 08:54:11.000000 ox_script-2.1.1/setup.py
```

### Comparing `ox_script-2.1.0/PKG-INFO` & `ox_script-2.1.1/PKG-INFO`

 * *Files 10% similar despite different names*

```diff
@@ -1,14 +1,12 @@
-Metadata-Version: 2.1
-Name: ox_script
-Version: 2.1.0
-Summary: The pskfunc.py file details offically supported APIs. The printer have a version of pskfunc.py on the printer with all functions fully implemented.
-Home-page: https://github.com/POSTEK-OX-Script
-Author: Postek Electronics Co., Ltd.
-Author-email: support@postek.com.cn
-License: MIT
-Description-Content-Type: text/markdown
-Requires-Dist: pandas
-Requires-Dist: openpyxl
-
-The pskfunc.py file details offically supported APIs. The printer have a version of pskfunc.py on the printer with all functions fully implemented.
-Most printer specific functions are left blank intentionally as they are meant to be executed on the printer and will throw an error if called on your devices. This file is provided more so for the beneift of keeping your IDE of choice happy while programming, providing extensive comments on the different functions and allowing for easy install through pip. 
+Metadata-Version: 2.1
+Name: ox_script
+Version: 2.1.1
+Summary: The pskfunc.py file details offically supported APIs. The printer have a version of pskfunc.py on the printer with all functions fully implemented.
+Home-page: https://github.com/POSTEK-OX-Script
+Author: Postek Electronics Co., Ltd.
+Author-email: support@postek.com.cn
+License: MIT
+Description-Content-Type: text/markdown
+
+The pskfunc.py file details offically supported APIs. The printer have a version of pskfunc.py on the printer with all functions fully implemented.
+Most printer specific functions are left blank intentionally as they are meant to be executed on the printer and will throw an error if called on your devices. This file is provided more so for the beneift of keeping your IDE of choice happy while programming, providing extensive comments on the different functions and allowing for easy install through pip.
```

### Comparing `ox_script-2.1.0/ox_script.egg-info/PKG-INFO` & `ox_script-2.1.1/ox_script.egg-info/PKG-INFO`

 * *Files 9% similar despite different names*

```diff
@@ -1,14 +1,12 @@
-Metadata-Version: 2.1
-Name: ox-script
-Version: 2.1.0
-Summary: The pskfunc.py file details offically supported APIs. The printer have a version of pskfunc.py on the printer with all functions fully implemented.
-Home-page: https://github.com/POSTEK-OX-Script
-Author: Postek Electronics Co., Ltd.
-Author-email: support@postek.com.cn
-License: MIT
-Description-Content-Type: text/markdown
-Requires-Dist: pandas
-Requires-Dist: openpyxl
-
-The pskfunc.py file details offically supported APIs. The printer have a version of pskfunc.py on the printer with all functions fully implemented.
-Most printer specific functions are left blank intentionally as they are meant to be executed on the printer and will throw an error if called on your devices. This file is provided more so for the beneift of keeping your IDE of choice happy while programming, providing extensive comments on the different functions and allowing for easy install through pip. 
+Metadata-Version: 2.1
+Name: ox-script
+Version: 2.1.1
+Summary: The pskfunc.py file details offically supported APIs. The printer have a version of pskfunc.py on the printer with all functions fully implemented.
+Home-page: https://github.com/POSTEK-OX-Script
+Author: Postek Electronics Co., Ltd.
+Author-email: support@postek.com.cn
+License: MIT
+Description-Content-Type: text/markdown
+
+The pskfunc.py file details offically supported APIs. The printer have a version of pskfunc.py on the printer with all functions fully implemented.
+Most printer specific functions are left blank intentionally as they are meant to be executed on the printer and will throw an error if called on your devices. This file is provided more so for the beneift of keeping your IDE of choice happy while programming, providing extensive comments on the different functions and allowing for easy install through pip.
```

### Comparing `ox_script-2.1.0/setup.py` & `ox_script-2.1.1/setup.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,20 +1,20 @@
-from setuptools import setup, find_packages
-
-long_description = "The pskfunc.py file details offically supported APIs. The printer have a version of pskfunc.py on the printer with all functions fully implemented.\nMost printer specific functions are left blank intentionally as they are meant to be executed on the printer and will throw an error if called on your devices. This file is provided more so for the beneift of keeping your IDE of choice happy while programming, providing extensive comments on the different functions and allowing for easy install through pip. "
-
-setup(
-    name='ox_script',
-    version='2.1.0',
-    author='Postek Electronics Co., Ltd.',
-    author_email='support@postek.com.cn',
-    packages=find_packages(),
-    license="MIT",
-    description="The pskfunc.py file details offically supported APIs. The printer have a version of pskfunc.py on the printer with all functions fully implemented.\nMost printer specific functions are left blank intentionally as they are meant to be executed on the printer and will throw an error if called on your devices. This file is provided more so for the beneift of keeping your IDE of choice happy while programming, providing extensive comments on the different functions and allowing for easy install through pip. ",
-    long_description=long_description,
-    long_description_content_type="text/markdown",
-    url="https://github.com/POSTEK-OX-Script",
-    install_requires=[
-        "pandas",
-        "openpyxl",
-    ],
-)
+from setuptools import setup, find_packages
+
+long_description = "The pskfunc.py file details offically supported APIs. The printer have a version of pskfunc.py on the printer with all functions fully implemented.\nMost printer specific functions are left blank intentionally as they are meant to be executed on the printer and will throw an error if called on your devices. This file is provided more so for the beneift of keeping your IDE of choice happy while programming, providing extensive comments on the different functions and allowing for easy install through pip. "
+
+setup(
+    name='ox_script',
+    version='2.1.1',
+    author='Postek Electronics Co., Ltd.',
+    author_email='support@postek.com.cn',
+    packages=find_packages(),
+    license="MIT",
+    description="The pskfunc.py file details offically supported APIs. The printer have a version of pskfunc.py on the printer with all functions fully implemented.\nMost printer specific functions are left blank intentionally as they are meant to be executed on the printer and will throw an error if called on your devices. This file is provided more so for the beneift of keeping your IDE of choice happy while programming, providing extensive comments on the different functions and allowing for easy install through pip. ",
+    long_description=long_description,
+    long_description_content_type="text/markdown",
+    url="https://github.com/POSTEK-OX-Script",
+    install_requires=[
+        "pandas",
+        "openpyxl",
+    ],
+)
```

