# Comparing `tmp/hellologger-0.2.2.post1.tar.gz` & `tmp/hellologger-0.2.2.post2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "hellologger-0.2.2.post1.tar", max compression
+gzip compressed data, was "hellologger-0.2.2.post2.tar", max compression
```

## Comparing `hellologger-0.2.2.post1.tar` & `hellologger-0.2.2.post2.tar`

### file list

```diff
@@ -1,6 +1,6 @@
--rw-r--r--   0        0        0     1086 2024-03-22 13:18:42.471202 hellologger-0.2.2.post1/LICENSE
--rw-r--r--   0        0        0      601 2024-05-02 17:35:00.702011 hellologger-0.2.2.post1/pyproject.toml
--rw-r--r--   0        0        0     4354 2024-03-31 15:04:10.183295 hellologger-0.2.2.post1/README.md
--rw-r--r--   0        0        0     6078 2024-05-02 17:33:31.290933 hellologger-0.2.2.post1/src/hellologger/__init__.py
--rw-r--r--   0        0        0      345 2024-05-02 17:32:48.532251 hellologger-0.2.2.post1/src/hellologger/const.py
--rw-r--r--   0        0        0     4842 1970-01-01 00:00:00.000000 hellologger-0.2.2.post1/PKG-INFO
+-rw-r--r--   0        0        0     1086 2024-05-14 15:32:06.571022 hellologger-0.2.2.post2/LICENSE
+-rw-r--r--   0        0        0      601 2024-05-29 09:18:10.299615 hellologger-0.2.2.post2/pyproject.toml
+-rw-r--r--   0        0        0     4354 2024-05-14 15:32:06.572173 hellologger-0.2.2.post2/README.md
+-rw-r--r--   0        0        0     6610 2024-05-29 09:17:32.156483 hellologger-0.2.2.post2/src/hellologger/__init__.py
+-rw-r--r--   0        0        0      345 2024-05-29 09:17:51.228007 hellologger-0.2.2.post2/src/hellologger/const.py
+-rw-r--r--   0        0        0     4842 1970-01-01 00:00:00.000000 hellologger-0.2.2.post2/PKG-INFO
```

### Comparing `hellologger-0.2.2.post1/LICENSE` & `hellologger-0.2.2.post2/LICENSE`

 * *Files identical despite different names*

### Comparing `hellologger-0.2.2.post1/pyproject.toml` & `hellologger-0.2.2.post2/pyproject.toml`

 * *Files 18% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "hellologger"
-version = "0.2.2.post1"
+version = "0.2.2.post2"
 description = ""
 authors = ["快乐的老鼠宝宝 <laoshubaby@protonmail.com>"]
 license = "MIT"
 readme = "README.md"
 repository = "https://github.com/OSMChina/Yuheng"
 classifiers = [
     "Programming Language :: Python :: 3",
```

### Comparing `hellologger-0.2.2.post1/README.md` & `hellologger-0.2.2.post2/README.md`

 * *Files identical despite different names*

### Comparing `hellologger-0.2.2.post1/src/hellologger/__init__.py` & `hellologger-0.2.2.post2/src/hellologger/__init__.py`

 * *Files 3% similar despite different names*

```diff
@@ -32,61 +32,72 @@
     * aws
     """
     if (
         log_target.get("aliyun", True)
         or log_target.get("aws", True)
         or log_target.get("webhook", True)
     ):
-        logging_config = {
-            "version": 1,
-            "formatters": {
-                "rawformatter": {
-                    "class": "logging.Formatter",
-                    "format": "%(message)s",
-                }
-            },
-            "handlers": {
-                "aliyun_sls_python_sdk": {
-                    "()": "aliyun.log.QueuedLogHandler",
-                    "level": log_level.get("aliyun", "INFO"),
-                    "formatter": "rawformatter",
-                    "end_point": get_variable(
-                        key=log_config.get("LOG_CONFIG_ALIYUN_ENDPOINT", None),
-                        default=LOG_CONFIG_ALIYUN_ENDPOINT,
-                    ),
-                    "access_key_id": get_variable(
-                        key="ALIYUN_ACCESSKEY_ID",
-                        default=LOG_CONFIG_ALIYUN_ACCESSKEY_ID,
-                    ),
-                    "access_key": get_variable(
-                        key="ALIYUN_ACCESSKEY_SECRET",
-                        default=LOG_CONFIG_ALIYUN_ACCESSKEY_SECRET,
-                    ),
-                    "project": get_variable(
-                        key=log_config.get("LOG_CONFIG_ALIYUN_PROJECT", None),
-                        default=LOG_CONFIG_ALIYUN_PROJECT,
-                    ),
-                    "log_store": get_variable(
-                        key=log_config.get("LOG_CONFIG_ALIYUN_LOGSTORE", None),
-                        default=LOG_CONFIG_ALIYUN_LOGSTORE,
-                    ),
-                }
-            },
-            "loggers": {
-                "aliyun_sls": {
-                    "handlers": [
-                        "aliyun_sls_python_sdk",
-                    ],
-                    "level": log_level.get("aliyun", "INFO"),
-                    "propagate": False,
-                }
-            },
-        }
-        logging.config.dictConfig(logging_config)
-        logging_handler_aliyun = logging.getLogger("aliyun_sls").handlers[0]
+        try:
+            logging_config = {
+                "version": 1,
+                "formatters": {
+                    "rawformatter": {
+                        "class": "logging.Formatter",
+                        "format": "%(message)s",
+                    }
+                },
+                "handlers": {
+                    "aliyun_sls_python_sdk": {
+                        "()": "aliyun.log.QueuedLogHandler",
+                        "level": log_level.get("aliyun", "INFO"),
+                        "formatter": "rawformatter",
+                        "end_point": get_variable(
+                            key=log_config.get(
+                                "LOG_CONFIG_ALIYUN_ENDPOINT", None
+                            ),
+                            default=LOG_CONFIG_ALIYUN_ENDPOINT,
+                        ),
+                        "access_key_id": get_variable(
+                            key="ALIYUN_ACCESSKEY_ID",
+                            default=LOG_CONFIG_ALIYUN_ACCESSKEY_ID,
+                        ),
+                        "access_key": get_variable(
+                            key="ALIYUN_ACCESSKEY_SECRET",
+                            default=LOG_CONFIG_ALIYUN_ACCESSKEY_SECRET,
+                        ),
+                        "project": get_variable(
+                            key=log_config.get(
+                                "LOG_CONFIG_ALIYUN_PROJECT", None
+                            ),
+                            default=LOG_CONFIG_ALIYUN_PROJECT,
+                        ),
+                        "log_store": get_variable(
+                            key=log_config.get(
+                                "LOG_CONFIG_ALIYUN_LOGSTORE", None
+                            ),
+                            default=LOG_CONFIG_ALIYUN_LOGSTORE,
+                        ),
+                    }
+                },
+                "loggers": {
+                    "aliyun_sls": {
+                        "handlers": [
+                            "aliyun_sls_python_sdk",
+                        ],
+                        "level": log_level.get("aliyun", "INFO"),
+                        "propagate": False,
+                    }
+                },
+            }
+            logging.config.dictConfig(logging_config)
+            logging_handler_aliyun = logging.getLogger("aliyun_sls").handlers[
+                0
+            ]
+        except Exception as e:
+            print("Can't load user specific logger due to some reason.")
 
     loguru_config = {}
     loguru_format = "{time:YYYY-MM-DD HH:mm:ss.SSS} | {level: <8} | {name}:{function}:{line} - {message}"
     logger = loguru.logger
 
     # for pytest project may need to record logs write by framework
     # pytest-loguru
```

### Comparing `hellologger-0.2.2.post1/PKG-INFO` & `hellologger-0.2.2.post2/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: hellologger
-Version: 0.2.2.post1
+Version: 0.2.2.post2
 Summary: 
 Home-page: https://github.com/OSMChina/Yuheng
 License: MIT
 Author: 快乐的老鼠宝宝
 Author-email: laoshubaby@protonmail.com
 Requires-Python: >=3.11,<4.0
 Classifier: License :: OSI Approved :: MIT License
```

