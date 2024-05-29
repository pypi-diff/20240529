# Comparing `tmp/asyncfix-0.9.0.tar.gz` & `tmp/asyncfix-1.0.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "asyncfix-0.9.0.tar", last modified: Sat Oct 14 14:54:43 2023, max compression
+gzip compressed data, was "asyncfix-1.0.1.tar", last modified: Wed May 29 08:08:51 2024, max compression
```

## Comparing `asyncfix-0.9.0.tar` & `asyncfix-1.0.1.tar`

### file list

```diff
@@ -1,44 +1,44 @@
-drwxr-xr-x   0 ubertrader  (1000) ubertrader  (1000)        0 2023-10-14 14:54:43.481438 asyncfix-0.9.0/
--rw-r--r--   0 ubertrader  (1000) ubertrader  (1000)     1075 2023-09-19 19:17:18.000000 asyncfix-0.9.0/LICENSE
--rw-r--r--   0 ubertrader  (1000) ubertrader  (1000)     2447 2023-10-14 14:54:43.481438 asyncfix-0.9.0/PKG-INFO
--rw-r--r--   0 ubertrader  (1000) ubertrader  (1000)     1373 2023-10-14 14:50:07.000000 asyncfix-0.9.0/README.md
-drwxr-xr-x   0 ubertrader  (1000) ubertrader  (1000)        0 2023-10-14 14:54:43.477438 asyncfix-0.9.0/asyncfix/
--rwxr-xr-x   0 ubertrader  (1000) ubertrader  (1000)      353 2023-10-14 12:54:19.000000 asyncfix-0.9.0/asyncfix/__init__.py
--rwxr-xr-x   0 ubertrader  (1000) ubertrader  (1000)    10649 2023-10-14 06:51:02.000000 asyncfix-0.9.0/asyncfix/codec.py
--rw-r--r--   0 ubertrader  (1000) ubertrader  (1000)    31438 2023-10-14 06:56:47.000000 asyncfix-0.9.0/asyncfix/connection.py
--rw-r--r--   0 ubertrader  (1000) ubertrader  (1000)     2273 2023-10-14 13:01:28.000000 asyncfix-0.9.0/asyncfix/connection_client.py
--rw-r--r--   0 ubertrader  (1000) ubertrader  (1000)     2674 2023-10-14 07:02:25.000000 asyncfix-0.9.0/asyncfix/connection_server.py
--rw-r--r--   0 ubertrader  (1000) ubertrader  (1000)      837 2023-10-14 07:09:51.000000 asyncfix-0.9.0/asyncfix/errors.py
--rw-r--r--   0 ubertrader  (1000) ubertrader  (1000)    16562 2023-10-14 07:35:52.000000 asyncfix-0.9.0/asyncfix/fix_tester.py
--rwxr-xr-x   0 ubertrader  (1000) ubertrader  (1000)    26451 2023-10-14 07:38:02.000000 asyncfix-0.9.0/asyncfix/fixtags.py
--rwxr-xr-x   0 ubertrader  (1000) ubertrader  (1000)     9190 2023-10-14 07:49:35.000000 asyncfix-0.9.0/asyncfix/journaler.py
--rwxr-xr-x   0 ubertrader  (1000) ubertrader  (1000)    12276 2023-10-14 12:55:47.000000 asyncfix-0.9.0/asyncfix/message.py
--rwxr-xr-x   0 ubertrader  (1000) ubertrader  (1000)     3333 2023-10-14 13:01:28.000000 asyncfix-0.9.0/asyncfix/msgtype.py
-drwxr-xr-x   0 ubertrader  (1000) ubertrader  (1000)        0 2023-10-14 14:54:43.477438 asyncfix-0.9.0/asyncfix/protocol/
--rwxr-xr-x   0 ubertrader  (1000) ubertrader  (1000)      254 2023-10-14 12:54:19.000000 asyncfix-0.9.0/asyncfix/protocol/__init__.py
--rw-r--r--   0 ubertrader  (1000) ubertrader  (1000)     1954 2023-10-14 13:01:28.000000 asyncfix-0.9.0/asyncfix/protocol/common.py
--rw-r--r--   0 ubertrader  (1000) ubertrader  (1000)    17434 2023-10-14 13:01:29.000000 asyncfix-0.9.0/asyncfix/protocol/order_single.py
--rwxr-xr-x   0 ubertrader  (1000) ubertrader  (1000)      301 2023-10-14 13:01:28.000000 asyncfix-0.9.0/asyncfix/protocol/protocol_base.py
--rwxr-xr-x   0 ubertrader  (1000) ubertrader  (1000)     8433 2023-10-14 13:01:28.000000 asyncfix-0.9.0/asyncfix/protocol/protocol_fix44.py
--rw-r--r--   0 ubertrader  (1000) ubertrader  (1000)    23371 2023-10-14 13:01:29.000000 asyncfix-0.9.0/asyncfix/protocol/schema.py
--rwxr-xr-x   0 ubertrader  (1000) ubertrader  (1000)     3240 2023-10-14 13:01:28.000000 asyncfix-0.9.0/asyncfix/session.py
-drwxr-xr-x   0 ubertrader  (1000) ubertrader  (1000)        0 2023-10-14 14:54:43.477438 asyncfix-0.9.0/asyncfix.egg-info/
--rw-r--r--   0 ubertrader  (1000) ubertrader  (1000)     2447 2023-10-14 14:54:43.000000 asyncfix-0.9.0/asyncfix.egg-info/PKG-INFO
--rw-r--r--   0 ubertrader  (1000) ubertrader  (1000)      945 2023-10-14 14:54:43.000000 asyncfix-0.9.0/asyncfix.egg-info/SOURCES.txt
--rw-r--r--   0 ubertrader  (1000) ubertrader  (1000)        1 2023-10-14 14:54:43.000000 asyncfix-0.9.0/asyncfix.egg-info/dependency_links.txt
--rw-r--r--   0 ubertrader  (1000) ubertrader  (1000)      135 2023-10-14 14:54:43.000000 asyncfix-0.9.0/asyncfix.egg-info/requires.txt
--rw-r--r--   0 ubertrader  (1000) ubertrader  (1000)        1 2023-10-14 14:54:43.000000 asyncfix-0.9.0/asyncfix.egg-info/top_level.txt
--rw-r--r--   0 ubertrader  (1000) ubertrader  (1000)     1169 2023-10-14 14:54:37.000000 asyncfix-0.9.0/pyproject.toml
--rw-r--r--   0 ubertrader  (1000) ubertrader  (1000)       38 2023-10-14 14:54:43.481438 asyncfix-0.9.0/setup.cfg
-drwxr-xr-x   0 ubertrader  (1000) ubertrader  (1000)        0 2023-10-14 14:54:43.481438 asyncfix-0.9.0/tests/
--rw-r--r--   0 ubertrader  (1000) ubertrader  (1000)    18036 2023-10-04 11:37:22.000000 asyncfix-0.9.0/tests/test_codec.py
--rw-r--r--   0 ubertrader  (1000) ubertrader  (1000)    54592 2023-10-14 12:48:02.000000 asyncfix-0.9.0/tests/test_connection.py
--rw-r--r--   0 ubertrader  (1000) ubertrader  (1000)     3178 2023-10-12 11:07:02.000000 asyncfix-0.9.0/tests/test_connection_client.py
--rw-r--r--   0 ubertrader  (1000) ubertrader  (1000)     2804 2023-10-12 11:08:09.000000 asyncfix-0.9.0/tests/test_connection_server.py
--rw-r--r--   0 ubertrader  (1000) ubertrader  (1000)     9360 2023-10-09 10:38:58.000000 asyncfix-0.9.0/tests/test_journaler.py
--rw-r--r--   0 ubertrader  (1000) ubertrader  (1000)     7093 2023-10-14 13:11:20.000000 asyncfix-0.9.0/tests/test_message.py
--rw-r--r--   0 ubertrader  (1000) ubertrader  (1000)      569 2023-09-23 11:52:58.000000 asyncfix-0.9.0/tests/test_protocol_common.py
--rw-r--r--   0 ubertrader  (1000) ubertrader  (1000)    78508 2023-10-14 13:11:44.000000 asyncfix-0.9.0/tests/test_protocol_order_single.py
--rw-r--r--   0 ubertrader  (1000) ubertrader  (1000)    29033 2023-10-14 12:44:02.000000 asyncfix-0.9.0/tests/test_protocol_schema.py
--rw-r--r--   0 ubertrader  (1000) ubertrader  (1000)     2265 2023-10-06 06:40:08.000000 asyncfix-0.9.0/tests/test_session.py
--rw-r--r--   0 ubertrader  (1000) ubertrader  (1000)      824 2023-09-20 09:09:14.000000 asyncfix-0.9.0/tests/test_tags_msgs.py
+drwxrws---   0 ubertrader  (1000) quant     (1002)        0 2024-05-29 08:08:51.258170 asyncfix-1.0.1/
+-rw-r-S---   0 ubertrader  (1000) quant     (1002)     1075 2023-09-19 19:17:18.000000 asyncfix-1.0.1/LICENSE
+-rw-r--r--   0 ubertrader  (1000) quant     (1002)     2460 2024-05-29 08:08:51.258170 asyncfix-1.0.1/PKG-INFO
+-rw-r-S---   0 ubertrader  (1000) quant     (1002)     1373 2023-10-14 14:50:07.000000 asyncfix-1.0.1/README.md
+drwxrws---   0 ubertrader  (1000) quant     (1002)        0 2024-05-29 08:08:51.250170 asyncfix-1.0.1/asyncfix/
+-rw-r-S---   0 ubertrader  (1000) quant     (1002)      353 2023-10-14 12:54:19.000000 asyncfix-1.0.1/asyncfix/__init__.py
+-rw-r-S---   0 ubertrader  (1000) quant     (1002)    10649 2023-10-14 06:51:02.000000 asyncfix-1.0.1/asyncfix/codec.py
+-rw-r-S---   0 ubertrader  (1000) quant     (1002)    31438 2023-10-14 06:56:47.000000 asyncfix-1.0.1/asyncfix/connection.py
+-rw-r-S---   0 ubertrader  (1000) quant     (1002)     2273 2023-10-14 13:01:28.000000 asyncfix-1.0.1/asyncfix/connection_client.py
+-rw-r-S---   0 ubertrader  (1000) quant     (1002)     2674 2023-10-14 07:02:25.000000 asyncfix-1.0.1/asyncfix/connection_server.py
+-rw-r-S---   0 ubertrader  (1000) quant     (1002)      837 2023-10-14 07:09:51.000000 asyncfix-1.0.1/asyncfix/errors.py
+-rw-r-S---   0 ubertrader  (1000) quant     (1002)    16562 2023-10-14 07:35:52.000000 asyncfix-1.0.1/asyncfix/fix_tester.py
+-rw-r-S---   0 ubertrader  (1000) quant     (1002)    26451 2023-10-14 07:38:02.000000 asyncfix-1.0.1/asyncfix/fixtags.py
+-rw-r-S---   0 ubertrader  (1000) quant     (1002)     9190 2023-10-14 07:49:35.000000 asyncfix-1.0.1/asyncfix/journaler.py
+-rw-r-S---   0 ubertrader  (1000) quant     (1002)    12276 2023-10-14 12:55:47.000000 asyncfix-1.0.1/asyncfix/message.py
+-rw-r-S---   0 ubertrader  (1000) quant     (1002)     3333 2023-10-14 13:01:28.000000 asyncfix-1.0.1/asyncfix/msgtype.py
+drwxrws---   0 ubertrader  (1000) quant     (1002)        0 2024-05-29 08:08:51.254170 asyncfix-1.0.1/asyncfix/protocol/
+-rw-r-S---   0 ubertrader  (1000) quant     (1002)      254 2023-10-14 12:54:19.000000 asyncfix-1.0.1/asyncfix/protocol/__init__.py
+-rw-r-S---   0 ubertrader  (1000) quant     (1002)     1954 2023-10-14 13:01:28.000000 asyncfix-1.0.1/asyncfix/protocol/common.py
+-rw-r-S---   0 ubertrader  (1000) quant     (1002)    17434 2023-10-14 13:01:29.000000 asyncfix-1.0.1/asyncfix/protocol/order_single.py
+-rw-r-S---   0 ubertrader  (1000) quant     (1002)      301 2023-10-14 13:01:28.000000 asyncfix-1.0.1/asyncfix/protocol/protocol_base.py
+-rw-r-S---   0 ubertrader  (1000) quant     (1002)     8433 2023-10-14 13:01:28.000000 asyncfix-1.0.1/asyncfix/protocol/protocol_fix44.py
+-rw-r-S---   0 ubertrader  (1000) quant     (1002)    23371 2023-10-14 13:01:29.000000 asyncfix-1.0.1/asyncfix/protocol/schema.py
+-rw-r-S---   0 ubertrader  (1000) quant     (1002)     3240 2023-10-14 13:01:28.000000 asyncfix-1.0.1/asyncfix/session.py
+drwxrws---   0 ubertrader  (1000) quant     (1002)        0 2024-05-29 08:08:51.254170 asyncfix-1.0.1/asyncfix.egg-info/
+-rw-r--r--   0 ubertrader  (1000) quant     (1002)     2460 2024-05-29 08:08:51.000000 asyncfix-1.0.1/asyncfix.egg-info/PKG-INFO
+-rw-r-S---   0 ubertrader  (1000) quant     (1002)      945 2024-05-29 08:08:51.000000 asyncfix-1.0.1/asyncfix.egg-info/SOURCES.txt
+-rw-r-S---   0 ubertrader  (1000) quant     (1002)        1 2024-05-29 08:08:51.000000 asyncfix-1.0.1/asyncfix.egg-info/dependency_links.txt
+-rw-r-S---   0 ubertrader  (1000) quant     (1002)      135 2024-05-29 08:08:51.000000 asyncfix-1.0.1/asyncfix.egg-info/requires.txt
+-rw-r-S---   0 ubertrader  (1000) quant     (1002)        9 2024-05-29 08:08:51.000000 asyncfix-1.0.1/asyncfix.egg-info/top_level.txt
+-rw-r-S---   0 ubertrader  (1000) quant     (1002)     1258 2024-05-29 08:07:26.000000 asyncfix-1.0.1/pyproject.toml
+-rw-rw----   0 ubertrader  (1000) quant     (1002)       38 2024-05-29 08:08:51.258170 asyncfix-1.0.1/setup.cfg
+drwxrws---   0 ubertrader  (1000) quant     (1002)        0 2024-05-29 08:08:51.254170 asyncfix-1.0.1/tests/
+-rw-r-S---   0 ubertrader  (1000) quant     (1002)    18036 2023-10-04 11:37:22.000000 asyncfix-1.0.1/tests/test_codec.py
+-rw-r-S---   0 ubertrader  (1000) quant     (1002)    54592 2023-10-14 12:48:02.000000 asyncfix-1.0.1/tests/test_connection.py
+-rw-r-S---   0 ubertrader  (1000) quant     (1002)     3178 2023-10-12 11:07:02.000000 asyncfix-1.0.1/tests/test_connection_client.py
+-rw-r-S---   0 ubertrader  (1000) quant     (1002)     2804 2023-10-12 11:08:09.000000 asyncfix-1.0.1/tests/test_connection_server.py
+-rw-r-S---   0 ubertrader  (1000) quant     (1002)     9360 2023-10-09 10:38:58.000000 asyncfix-1.0.1/tests/test_journaler.py
+-rw-r-S---   0 ubertrader  (1000) quant     (1002)     7093 2023-10-14 13:11:20.000000 asyncfix-1.0.1/tests/test_message.py
+-rw-r-S---   0 ubertrader  (1000) quant     (1002)      569 2023-09-23 11:52:58.000000 asyncfix-1.0.1/tests/test_protocol_common.py
+-rw-r-S---   0 ubertrader  (1000) quant     (1002)    78508 2023-10-14 13:11:44.000000 asyncfix-1.0.1/tests/test_protocol_order_single.py
+-rw-r-S---   0 ubertrader  (1000) quant     (1002)    29033 2023-10-14 12:44:02.000000 asyncfix-1.0.1/tests/test_protocol_schema.py
+-rw-r-S---   0 ubertrader  (1000) quant     (1002)     2265 2023-10-06 06:40:08.000000 asyncfix-1.0.1/tests/test_session.py
+-rw-r-S---   0 ubertrader  (1000) quant     (1002)      824 2023-09-20 09:09:14.000000 asyncfix-1.0.1/tests/test_tags_msgs.py
```

### Comparing `asyncfix-0.9.0/LICENSE` & `asyncfix-1.0.1/LICENSE`

 * *Files identical despite different names*

### Comparing `asyncfix-0.9.0/PKG-INFO` & `asyncfix-1.0.1/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,19 +1,19 @@
 Metadata-Version: 2.1
 Name: asyncfix
-Version: 0.9.0
+Version: 1.0.1
 Summary: AsyncIO FIX Protocol client for Python
 Author-email: Alex Veden <i@alexveden.com>
 License: MIT License
 Project-URL: Homepage, https://github.com/alexveden/asyncfix
 Keywords: asyncio,FIX,protocol,client,server,parser,unit tests,simplefix,tester,orders
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3.8
-Classifier: Development Status :: 4 - Beta
+Classifier: Development Status :: 5 - Production/Stable
 Requires-Python: >=3.8
 Description-Content-Type: text/markdown
 License-File: LICENSE
 Provides-Extra: dev
 Requires-Dist: pytest; extra == "dev"
 Requires-Dist: isort==5.12.0; extra == "dev"
 Requires-Dist: flake8==6.1.0; extra == "dev"
```

### Comparing `asyncfix-0.9.0/README.md` & `asyncfix-1.0.1/README.md`

 * *Files identical despite different names*

### Comparing `asyncfix-0.9.0/asyncfix/codec.py` & `asyncfix-1.0.1/asyncfix/codec.py`

 * *Files identical despite different names*

### Comparing `asyncfix-0.9.0/asyncfix/connection.py` & `asyncfix-1.0.1/asyncfix/connection.py`

 * *Files identical despite different names*

### Comparing `asyncfix-0.9.0/asyncfix/connection_client.py` & `asyncfix-1.0.1/asyncfix/connection_client.py`

 * *Files identical despite different names*

### Comparing `asyncfix-0.9.0/asyncfix/connection_server.py` & `asyncfix-1.0.1/asyncfix/connection_server.py`

 * *Files identical despite different names*

### Comparing `asyncfix-0.9.0/asyncfix/errors.py` & `asyncfix-1.0.1/asyncfix/errors.py`

 * *Files identical despite different names*

### Comparing `asyncfix-0.9.0/asyncfix/fix_tester.py` & `asyncfix-1.0.1/asyncfix/fix_tester.py`

 * *Files identical despite different names*

### Comparing `asyncfix-0.9.0/asyncfix/fixtags.py` & `asyncfix-1.0.1/asyncfix/fixtags.py`

 * *Files identical despite different names*

### Comparing `asyncfix-0.9.0/asyncfix/journaler.py` & `asyncfix-1.0.1/asyncfix/journaler.py`

 * *Files identical despite different names*

### Comparing `asyncfix-0.9.0/asyncfix/message.py` & `asyncfix-1.0.1/asyncfix/message.py`

 * *Files identical despite different names*

### Comparing `asyncfix-0.9.0/asyncfix/msgtype.py` & `asyncfix-1.0.1/asyncfix/msgtype.py`

 * *Files identical despite different names*

### Comparing `asyncfix-0.9.0/asyncfix/protocol/common.py` & `asyncfix-1.0.1/asyncfix/protocol/common.py`

 * *Files identical despite different names*

### Comparing `asyncfix-0.9.0/asyncfix/protocol/order_single.py` & `asyncfix-1.0.1/asyncfix/protocol/order_single.py`

 * *Files identical despite different names*

### Comparing `asyncfix-0.9.0/asyncfix/protocol/protocol_fix44.py` & `asyncfix-1.0.1/asyncfix/protocol/protocol_fix44.py`

 * *Files identical despite different names*

### Comparing `asyncfix-0.9.0/asyncfix/protocol/schema.py` & `asyncfix-1.0.1/asyncfix/protocol/schema.py`

 * *Files identical despite different names*

### Comparing `asyncfix-0.9.0/asyncfix/session.py` & `asyncfix-1.0.1/asyncfix/session.py`

 * *Files identical despite different names*

### Comparing `asyncfix-0.9.0/asyncfix.egg-info/PKG-INFO` & `asyncfix-1.0.1/asyncfix.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,19 +1,19 @@
 Metadata-Version: 2.1
 Name: asyncfix
-Version: 0.9.0
+Version: 1.0.1
 Summary: AsyncIO FIX Protocol client for Python
 Author-email: Alex Veden <i@alexveden.com>
 License: MIT License
 Project-URL: Homepage, https://github.com/alexveden/asyncfix
 Keywords: asyncio,FIX,protocol,client,server,parser,unit tests,simplefix,tester,orders
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3.8
-Classifier: Development Status :: 4 - Beta
+Classifier: Development Status :: 5 - Production/Stable
 Requires-Python: >=3.8
 Description-Content-Type: text/markdown
 License-File: LICENSE
 Provides-Extra: dev
 Requires-Dist: pytest; extra == "dev"
 Requires-Dist: isort==5.12.0; extra == "dev"
 Requires-Dist: flake8==6.1.0; extra == "dev"
```

### Comparing `asyncfix-0.9.0/asyncfix.egg-info/SOURCES.txt` & `asyncfix-1.0.1/asyncfix.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `asyncfix-0.9.0/pyproject.toml` & `asyncfix-1.0.1/pyproject.toml`

 * *Files 12% similar despite different names*

```diff
@@ -1,19 +1,19 @@
 [project]
 name = "asyncfix"
-version = "0.9.0"
+version = "1.0.1"
 description = "AsyncIO FIX Protocol client for Python"
 readme = "README.md"
 authors = [{ name = "Alex Veden", email = "i@alexveden.com" }]
 license = {text = "MIT License"}
 classifiers = [
     "License :: OSI Approved :: MIT License",
     "Programming Language :: Python",
     "Programming Language :: Python :: 3.8",
-    "Development Status :: 4 - Beta",
+    "Development Status :: 5 - Production/Stable",
 ]
 keywords = ["asyncio", "FIX", "protocol", "client", "server", "parser", "unit tests", "simplefix", "tester", "orders"]
 requires-python = ">=3.8"
 
 dependencies = []
 
 [project.optional-dependencies]
@@ -31,20 +31,23 @@
   "mkdocs",
 ]
 
 [project.urls]
 Homepage = "https://github.com/alexveden/asyncfix"
 
 [tool.setuptools]
-py-modules = []
+packages = ["asyncfix", "asyncfix.protocol"]
 
 [tool.isort]
 profile = "black"
 extend_skip = ["__init__.py"]
 
+[tool.distutils.bdist_wheel]
+universal = true
+
 [tool.pydocstringformatter]
 write = true
 strip-whitespaces = true
 summary-quotes-same-line = true
 max-line-length = 88
 split-summary-body = false
 linewrap-full-docstring = true
```

### Comparing `asyncfix-0.9.0/tests/test_codec.py` & `asyncfix-1.0.1/tests/test_codec.py`

 * *Files identical despite different names*

### Comparing `asyncfix-0.9.0/tests/test_connection.py` & `asyncfix-1.0.1/tests/test_connection.py`

 * *Files identical despite different names*

### Comparing `asyncfix-0.9.0/tests/test_connection_client.py` & `asyncfix-1.0.1/tests/test_connection_client.py`

 * *Files identical despite different names*

### Comparing `asyncfix-0.9.0/tests/test_connection_server.py` & `asyncfix-1.0.1/tests/test_connection_server.py`

 * *Files identical despite different names*

### Comparing `asyncfix-0.9.0/tests/test_journaler.py` & `asyncfix-1.0.1/tests/test_journaler.py`

 * *Files identical despite different names*

### Comparing `asyncfix-0.9.0/tests/test_message.py` & `asyncfix-1.0.1/tests/test_message.py`

 * *Files identical despite different names*

### Comparing `asyncfix-0.9.0/tests/test_protocol_common.py` & `asyncfix-1.0.1/tests/test_protocol_common.py`

 * *Files identical despite different names*

### Comparing `asyncfix-0.9.0/tests/test_protocol_order_single.py` & `asyncfix-1.0.1/tests/test_protocol_order_single.py`

 * *Files identical despite different names*

### Comparing `asyncfix-0.9.0/tests/test_protocol_schema.py` & `asyncfix-1.0.1/tests/test_protocol_schema.py`

 * *Files identical despite different names*

### Comparing `asyncfix-0.9.0/tests/test_session.py` & `asyncfix-1.0.1/tests/test_session.py`

 * *Files identical despite different names*

### Comparing `asyncfix-0.9.0/tests/test_tags_msgs.py` & `asyncfix-1.0.1/tests/test_tags_msgs.py`

 * *Files identical despite different names*

