# Comparing `tmp/xfapi-0.0.1.tar.gz` & `tmp/xfapi-0.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "xfapi-0.0.1.tar", last modified: Wed May 29 06:54:16 2024, max compression
+gzip compressed data, was "xfapi-0.0.2.tar", last modified: Wed May 29 07:24:09 2024, max compression
```

## Comparing `xfapi-0.0.1.tar` & `xfapi-0.0.2.tar`

### file list

```diff
@@ -1,11 +1,11 @@
-drwxr-xr-x   0 asia       (501) staff       (20)        0 2024-05-29 06:54:16.995467 xfapi-0.0.1/
--rw-r--r--   0 asia       (501) staff       (20)     1307 2024-05-29 06:54:16.995251 xfapi-0.0.1/PKG-INFO
--rw-r--r--   0 asia       (501) staff       (20)       14 2024-05-29 05:50:03.000000 xfapi-0.0.1/requirements.txt
--rw-r--r--   0 asia       (501) staff       (20)       38 2024-05-29 06:54:16.995530 xfapi-0.0.1/setup.cfg
--rw-r--r--   0 asia       (501) staff       (20)     1715 2024-05-29 06:25:56.000000 xfapi-0.0.1/setup.py
-drwxr-xr-x   0 asia       (501) staff       (20)        0 2024-05-29 06:54:16.994981 xfapi-0.0.1/xfapi.egg-info/
--rw-r--r--   0 asia       (501) staff       (20)     1307 2024-05-29 06:54:16.000000 xfapi-0.0.1/xfapi.egg-info/PKG-INFO
--rw-r--r--   0 asia       (501) staff       (20)      169 2024-05-29 06:54:16.000000 xfapi-0.0.1/xfapi.egg-info/SOURCES.txt
--rw-r--r--   0 asia       (501) staff       (20)        1 2024-05-29 06:54:16.000000 xfapi-0.0.1/xfapi.egg-info/dependency_links.txt
--rw-r--r--   0 asia       (501) staff       (20)       15 2024-05-29 06:54:16.000000 xfapi-0.0.1/xfapi.egg-info/requires.txt
--rw-r--r--   0 asia       (501) staff       (20)        1 2024-05-29 06:54:16.000000 xfapi-0.0.1/xfapi.egg-info/top_level.txt
+drwxr-xr-x   0 asia       (501) staff       (20)        0 2024-05-29 07:24:09.556513 xfapi-0.0.2/
+-rw-r--r--   0 asia       (501) staff       (20)     1307 2024-05-29 07:24:09.556305 xfapi-0.0.2/PKG-INFO
+-rw-r--r--   0 asia       (501) staff       (20)       14 2024-05-29 05:50:03.000000 xfapi-0.0.2/requirements.txt
+-rw-r--r--   0 asia       (501) staff       (20)       38 2024-05-29 07:24:09.556557 xfapi-0.0.2/setup.cfg
+-rw-r--r--   0 asia       (501) staff       (20)     1393 2024-05-29 07:23:01.000000 xfapi-0.0.2/setup.py
+drwxr-xr-x   0 asia       (501) staff       (20)        0 2024-05-29 07:24:09.556089 xfapi-0.0.2/xfapi.egg-info/
+-rw-r--r--   0 asia       (501) staff       (20)     1307 2024-05-29 07:24:09.000000 xfapi-0.0.2/xfapi.egg-info/PKG-INFO
+-rw-r--r--   0 asia       (501) staff       (20)      169 2024-05-29 07:24:09.000000 xfapi-0.0.2/xfapi.egg-info/SOURCES.txt
+-rw-r--r--   0 asia       (501) staff       (20)        1 2024-05-29 07:24:09.000000 xfapi-0.0.2/xfapi.egg-info/dependency_links.txt
+-rw-r--r--   0 asia       (501) staff       (20)       15 2024-05-29 07:24:09.000000 xfapi-0.0.2/xfapi.egg-info/requires.txt
+-rw-r--r--   0 asia       (501) staff       (20)        1 2024-05-29 07:24:09.000000 xfapi-0.0.2/xfapi.egg-info/top_level.txt
```

### Comparing `xfapi-0.0.1/PKG-INFO` & `xfapi-0.0.2/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: xfapi
-Version: 0.0.1
+Version: 0.0.2
 Summary: Apis tool base fastapi
 Home-page: https://pypi.org/project/xfapi/
 Author: Alex_M
 Author-email: asiaier@163.com
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

### Comparing `xfapi-0.0.1/setup.py` & `xfapi-0.0.2/setup.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,25 +1,14 @@
 import setuptools
-import re
-import requests
-from bs4 import BeautifulSoup
  
 package_name = "xfapi"
  
- 
-def curr_version():
-    url = f"https://pypi.org/project/{package_name}/"
-    response = requests.get(url)
-    soup = BeautifulSoup(response.content, "html.parser")
-    latest_version = soup.select_one(".release__version").text.strip()
-    return str(latest_version)
- 
- 
+
 def get_version():
-   return "0.0.1"
+   return "0.0.2"
  
  
 def upload():
     with open("README.md", "r") as fh:
         long_description = fh.read()
     with open('requirements.txt') as f:
         required = f.read().splitlines()
@@ -50,14 +39,14 @@
     with open("VERSION", "w") as version_f:
         version_f.write(get_version())
  
  
 def main():
     try:
         upload()
-        print("Upload success , Current VERSION:", "0.0.1")
+        print("Upload success , Current VERSION:", get_version())
     except Exception as e:
         raise Exception("Upload package error", e)
  
  
 if __name__ == '__main__':
     main()
```

### Comparing `xfapi-0.0.1/xfapi.egg-info/PKG-INFO` & `xfapi-0.0.2/xfapi.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: xfapi
-Version: 0.0.1
+Version: 0.0.2
 Summary: Apis tool base fastapi
 Home-page: https://pypi.org/project/xfapi/
 Author: Alex_M
 Author-email: asiaier@163.com
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

