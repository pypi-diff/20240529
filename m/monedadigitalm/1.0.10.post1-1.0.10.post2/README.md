# Comparing `tmp/monedadigitalm-1.0.10.post1.tar.gz` & `tmp/monedadigitalm-1.0.10.post2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "D:\DEV\xampp\htdocs\pymexc\dist\tmpt0vyxdl8\monedadigitalm-1.0.10.post1.tar", last modified: Fri Dec 15 17:46:02 2023, max compression
+gzip compressed data, was "monedadigitalm-1.0.10.post2.tar", last modified: Wed May 29 13:23:31 2024, max compression
```

## Comparing `monedadigitalm-1.0.10.post1.tar` & `monedadigitalm-1.0.10.post2.tar`

### file list

```diff
@@ -1,19 +1,19 @@
-drwxrwxrwx   0        0        0        0 2023-12-15 17:46:02.000000 monedadigitalm-1.0.10.post1/
--rw-rw-rw-   0        0        0     1067 2023-11-19 19:09:48.000000 monedadigitalm-1.0.10.post1/LICENSE
-drwxrwxrwx   0        0        0        0 2023-12-15 17:46:02.000000 monedadigitalm-1.0.10.post1/monedadigitalm.egg-info/
--rw-rw-rw-   0        0        0        1 2023-12-15 17:46:02.000000 monedadigitalm-1.0.10.post1/monedadigitalm.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0        2 2023-12-15 17:46:02.000000 monedadigitalm-1.0.10.post1/monedadigitalm.egg-info/not-zip-safe
--rw-rw-rw-   0        0        0     3935 2023-12-15 17:46:02.000000 monedadigitalm-1.0.10.post1/monedadigitalm.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0       26 2023-12-15 17:46:02.000000 monedadigitalm-1.0.10.post1/monedadigitalm.egg-info/requires.txt
--rw-rw-rw-   0        0        0      354 2023-12-15 17:46:02.000000 monedadigitalm-1.0.10.post1/monedadigitalm.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        7 2023-12-15 17:46:02.000000 monedadigitalm-1.0.10.post1/monedadigitalm.egg-info/top_level.txt
--rw-rw-rw-   0        0        0     3935 2023-12-15 17:46:02.000000 monedadigitalm-1.0.10.post1/PKG-INFO
-drwxrwxrwx   0        0        0        0 2023-12-15 17:46:02.000000 monedadigitalm-1.0.10.post1/pymexc/
--rw-rw-rw-   0        0        0     6182 2023-12-15 17:28:15.000000 monedadigitalm-1.0.10.post1/pymexc/base.py
--rw-rw-rw-   0        0        0    17147 2023-11-19 19:09:48.000000 monedadigitalm-1.0.10.post1/pymexc/base_websocket.py
--rw-rw-rw-   0        0        0    66134 2023-12-15 17:29:34.000000 monedadigitalm-1.0.10.post1/pymexc/futures.py
--rw-rw-rw-   0        0        0    70632 2023-12-15 17:30:00.000000 monedadigitalm-1.0.10.post1/pymexc/spot.py
--rw-rw-rw-   0        0        0     1372 2023-11-19 19:09:48.000000 monedadigitalm-1.0.10.post1/pymexc/__init__.py
--rw-rw-rw-   0        0        0     2699 2023-11-19 19:09:48.000000 monedadigitalm-1.0.10.post1/README.md
--rw-rw-rw-   0        0        0       42 2023-12-15 17:46:02.000000 monedadigitalm-1.0.10.post1/setup.cfg
--rw-rw-rw-   0        0        0     1698 2023-12-15 17:44:17.000000 monedadigitalm-1.0.10.post1/setup.py
+drwxrwxrwx   0        0        0        0 2024-05-29 13:23:31.747682 monedadigitalm-1.0.10.post2/
+-rw-rw-rw-   0        0        0     1067 2023-11-19 19:09:48.000000 monedadigitalm-1.0.10.post2/LICENSE
+-rw-rw-rw-   0        0        0     3970 2024-05-29 13:23:31.744598 monedadigitalm-1.0.10.post2/PKG-INFO
+-rw-rw-rw-   0        0        0     2699 2023-11-19 19:09:48.000000 monedadigitalm-1.0.10.post2/README.md
+drwxrwxrwx   0        0        0        0 2024-05-29 13:23:31.743602 monedadigitalm-1.0.10.post2/monedadigitalm.egg-info/
+-rw-rw-rw-   0        0        0     3970 2024-05-29 13:23:31.000000 monedadigitalm-1.0.10.post2/monedadigitalm.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      354 2024-05-29 13:23:31.000000 monedadigitalm-1.0.10.post2/monedadigitalm.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-05-29 13:23:31.000000 monedadigitalm-1.0.10.post2/monedadigitalm.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0        2 2023-12-15 17:46:02.000000 monedadigitalm-1.0.10.post2/monedadigitalm.egg-info/not-zip-safe
+-rw-rw-rw-   0        0        0       26 2024-05-29 13:23:31.000000 monedadigitalm-1.0.10.post2/monedadigitalm.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        7 2024-05-29 13:23:31.000000 monedadigitalm-1.0.10.post2/monedadigitalm.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2024-05-29 13:23:31.739974 monedadigitalm-1.0.10.post2/pymexc/
+-rw-rw-rw-   0        0        0     1372 2023-11-19 19:09:48.000000 monedadigitalm-1.0.10.post2/pymexc/__init__.py
+-rw-rw-rw-   0        0        0     6455 2024-05-29 13:17:32.000000 monedadigitalm-1.0.10.post2/pymexc/base.py
+-rw-rw-rw-   0        0        0    17147 2023-11-19 19:09:48.000000 monedadigitalm-1.0.10.post2/pymexc/base_websocket.py
+-rw-rw-rw-   0        0        0    66134 2023-12-15 17:29:34.000000 monedadigitalm-1.0.10.post2/pymexc/futures.py
+-rw-rw-rw-   0        0        0    70632 2023-12-15 17:30:00.000000 monedadigitalm-1.0.10.post2/pymexc/spot.py
+-rw-rw-rw-   0        0        0       42 2024-05-29 13:23:31.747682 monedadigitalm-1.0.10.post2/setup.cfg
+-rw-rw-rw-   0        0        0     1698 2024-05-29 13:17:38.000000 monedadigitalm-1.0.10.post2/setup.py
```

### filetype from file(1)

```diff
@@ -1 +1 @@
-POSIX tar archive (GNU)
+POSIX tar archive
```

### Comparing `monedadigitalm-1.0.10.post1/LICENSE` & `monedadigitalm-1.0.10.post2/LICENSE`

 * *Files identical despite different names*

### Comparing `monedadigitalm-1.0.10.post1/monedadigitalm.egg-info/PKG-INFO` & `monedadigitalm-1.0.10.post2/PKG-INFO`

 * *Files 10% similar despite different names*

```diff
@@ -1,17 +1,16 @@
 Metadata-Version: 2.1
 Name: monedadigitalm
-Version: 1.0.10.post1
+Version: 1.0.10.post2
 Summary: Unofficial python library for interacting with the MEXC crypto exchange :REVISION:AmadoRamos
 Home-page: https://github.com/AmadoRamos/pymexc.git
+Download-URL: https://github.com/AmadoRamos/pymexc/archive/refs/tags/v1.0.10r2.zip
 Author: abuztrade
 Author-email: abuztrade.work@gmail.com
 License: MIT License
-Download-URL: https://github.com/AmadoRamos/pymexc/archive/refs/tags/v1.0.10r1.zip
-Platform: UNKNOWN
 Classifier: Development Status :: 4 - Beta
 Classifier: Topic :: Communications :: Email
 Classifier: Operating System :: OS Independent
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.6
 Classifier: Programming Language :: Python :: 3.7
@@ -20,14 +19,16 @@
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Intended Audience :: Developers
 Classifier: Intended Audience :: Customer Service
 Classifier: Intended Audience :: Financial and Insurance Industry
 Requires-Python: >=3.6.0
 Description-Content-Type: text/markdown
 License-File: LICENSE
+Requires-Dist: requests
+Requires-Dist: websocket-client
 
 [![PyPI version](https://badge.fury.io/py/pymexc.svg)](https://badge.fury.io/py/pymexc)
 [![License](https://img.shields.io/github/license/makarworld/pymexc.svg?label=License&logo=apache&cacheSeconds=2592000)](https://github.com/makarworld/pymexc/blob/main/LICENSE)
 [![image](https://img.shields.io/pypi/pyversions/pymexc.svg)](https://pypi.org/project/pymexc/)
 [![Github last commit date](https://img.shields.io/github/last-commit/makarworld/pymexc.svg?label=Updated&logo=github&cacheSeconds=600)](https://github.com/makarworld/pymexc/commits)
 
 # pymexc
@@ -95,9 +96,7 @@
 
 
 # Documentation
 You can find the official documentation for the MEXC API [here](https://mexcdevelop.github.io/apidocs/spot_v3_en/#introduction).
 
 # License
 This library is licensed under the MIT License.
-
-
```

### Comparing `monedadigitalm-1.0.10.post1/PKG-INFO` & `monedadigitalm-1.0.10.post2/monedadigitalm.egg-info/PKG-INFO`

 * *Files 10% similar despite different names*

```diff
@@ -1,17 +1,16 @@
 Metadata-Version: 2.1
 Name: monedadigitalm
-Version: 1.0.10.post1
+Version: 1.0.10.post2
 Summary: Unofficial python library for interacting with the MEXC crypto exchange :REVISION:AmadoRamos
 Home-page: https://github.com/AmadoRamos/pymexc.git
+Download-URL: https://github.com/AmadoRamos/pymexc/archive/refs/tags/v1.0.10r2.zip
 Author: abuztrade
 Author-email: abuztrade.work@gmail.com
 License: MIT License
-Download-URL: https://github.com/AmadoRamos/pymexc/archive/refs/tags/v1.0.10r1.zip
-Platform: UNKNOWN
 Classifier: Development Status :: 4 - Beta
 Classifier: Topic :: Communications :: Email
 Classifier: Operating System :: OS Independent
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.6
 Classifier: Programming Language :: Python :: 3.7
@@ -20,14 +19,16 @@
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Intended Audience :: Developers
 Classifier: Intended Audience :: Customer Service
 Classifier: Intended Audience :: Financial and Insurance Industry
 Requires-Python: >=3.6.0
 Description-Content-Type: text/markdown
 License-File: LICENSE
+Requires-Dist: requests
+Requires-Dist: websocket-client
 
 [![PyPI version](https://badge.fury.io/py/pymexc.svg)](https://badge.fury.io/py/pymexc)
 [![License](https://img.shields.io/github/license/makarworld/pymexc.svg?label=License&logo=apache&cacheSeconds=2592000)](https://github.com/makarworld/pymexc/blob/main/LICENSE)
 [![image](https://img.shields.io/pypi/pyversions/pymexc.svg)](https://pypi.org/project/pymexc/)
 [![Github last commit date](https://img.shields.io/github/last-commit/makarworld/pymexc.svg?label=Updated&logo=github&cacheSeconds=600)](https://github.com/makarworld/pymexc/commits)
 
 # pymexc
@@ -95,9 +96,7 @@
 
 
 # Documentation
 You can find the official documentation for the MEXC API [here](https://mexcdevelop.github.io/apidocs/spot_v3_en/#introduction).
 
 # License
 This library is licensed under the MIT License.
-
-
```

### Comparing `monedadigitalm-1.0.10.post1/pymexc/base.py` & `monedadigitalm-1.0.10.post2/pymexc/base.py`

 * *Files 4% similar despite different names*

```diff
@@ -155,17 +155,24 @@
 
         for variant in ('params', 'json'):
             if kwargs.get(variant):
                 kwargs[variant] = {k: v for k, v in kwargs[variant].items() if v is not None}
             
                 if self.api_key and self.api_secret:
                     # add signature
-                    timestamp = str(int(time.time() * 1000))
+                    timestamp = str(self.get_server_time())
 
                     kwargs['headers'] = {
                         "Request-Time": timestamp,
                         "Signature": self.sign(timestamp, **kwargs[variant])
                     }
 
         response = self.session.request(method, f"{self.base_url}{router}", *args, **kwargs)
 
-        return response.json()
+        return response.json()
+    
+    def get_server_time(self):
+        response = self.session.request("GET",'https://www.mexc.com/open/api/v2/common/timestamp')
+        if response.status_code == 200:
+            return response.json()['data']
+        else:
+            raise int(time.time() * 1000)
```

### Comparing `monedadigitalm-1.0.10.post1/pymexc/base_websocket.py` & `monedadigitalm-1.0.10.post2/pymexc/base_websocket.py`

 * *Files identical despite different names*

### Comparing `monedadigitalm-1.0.10.post1/pymexc/futures.py` & `monedadigitalm-1.0.10.post2/pymexc/futures.py`

 * *Files identical despite different names*

### Comparing `monedadigitalm-1.0.10.post1/pymexc/spot.py` & `monedadigitalm-1.0.10.post2/pymexc/spot.py`

 * *Files identical despite different names*

### Comparing `monedadigitalm-1.0.10.post1/pymexc/__init__.py` & `monedadigitalm-1.0.10.post2/pymexc/__init__.py`

 * *Files identical despite different names*

### Comparing `monedadigitalm-1.0.10.post1/README.md` & `monedadigitalm-1.0.10.post2/README.md`

 * *Files identical despite different names*

### Comparing `monedadigitalm-1.0.10.post1/setup.py` & `monedadigitalm-1.0.10.post2/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -4,15 +4,15 @@
 :author: abuztrade
 :license: MIT License, see LICENSE file.
 :copyright: (c) 2022 by abuztrade.
 :revision: Amado Ramos
 """
 
 
-version = '1.0.10r1'
+version = '1.0.10r2'
 
 with open("README.md", "r") as f:
     long_description = f.read()
 
 setup(
     name="monedadigitalm",
     version=version,
```

