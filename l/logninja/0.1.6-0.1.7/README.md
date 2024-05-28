# Comparing `tmp/logninja-0.1.6.tar.gz` & `tmp/logninja-0.1.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "logninja-0.1.6.tar", last modified: Fri May 24 20:39:30 2024, max compression
+gzip compressed data, was "logninja-0.1.7.tar", last modified: Tue May 28 18:35:19 2024, max compression
```

## Comparing `logninja-0.1.6.tar` & `logninja-0.1.7.tar`

### file list

```diff
@@ -1,24 +1,25 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-24 20:39:30.300490 logninja-0.1.6/
--rw-r--r--   0 runner    (1001) docker     (127)     1071 2024-05-24 20:39:26.000000 logninja-0.1.6/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)     7603 2024-05-24 20:39:30.300490 logninja-0.1.6/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     6734 2024-05-24 20:39:26.000000 logninja-0.1.6/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-24 20:39:30.300490 logninja-0.1.6/logninja/
--rw-r--r--   0 runner    (1001) docker     (127)      690 2024-05-24 20:39:26.000000 logninja-0.1.6/logninja/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-24 20:39:30.300490 logninja-0.1.6/logninja/asgi/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-24 20:39:26.000000 logninja-0.1.6/logninja/asgi/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     4034 2024-05-24 20:39:26.000000 logninja-0.1.6/logninja/asgi/middleware.py
--rw-r--r--   0 runner    (1001) docker     (127)      134 2024-05-24 20:39:26.000000 logninja-0.1.6/logninja/console_formatter.py
--rw-r--r--   0 runner    (1001) docker     (127)      456 2024-05-24 20:39:26.000000 logninja-0.1.6/logninja/contextvars_filter.py
--rw-r--r--   0 runner    (1001) docker     (127)     1427 2024-05-24 20:39:26.000000 logninja-0.1.6/logninja/decorators.py
--rw-r--r--   0 runner    (1001) docker     (127)     1749 2024-05-24 20:39:26.000000 logninja-0.1.6/logninja/json_formatter.py
--rw-r--r--   0 runner    (1001) docker     (127)     5705 2024-05-24 20:39:26.000000 logninja-0.1.6/logninja/traceback.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-24 20:39:30.300490 logninja-0.1.6/logninja.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     7603 2024-05-24 20:39:30.000000 logninja-0.1.6/logninja.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      428 2024-05-24 20:39:30.000000 logninja-0.1.6/logninja.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-24 20:39:30.000000 logninja-0.1.6/logninja.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       39 2024-05-24 20:39:30.000000 logninja-0.1.6/logninja.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)        9 2024-05-24 20:39:30.000000 logninja-0.1.6/logninja.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)      858 2024-05-24 20:39:26.000000 logninja-0.1.6/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-24 20:39:30.300490 logninja-0.1.6/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-24 20:39:30.300490 logninja-0.1.6/tests/
--rw-r--r--   0 runner    (1001) docker     (127)     1217 2024-05-24 20:39:26.000000 logninja-0.1.6/tests/test_json_formatter.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-28 18:35:19.219811 logninja-0.1.7/
+-rw-r--r--   0 runner    (1001) docker     (127)     1071 2024-05-28 18:35:15.000000 logninja-0.1.7/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)     7676 2024-05-28 18:35:19.219811 logninja-0.1.7/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     6807 2024-05-28 18:35:15.000000 logninja-0.1.7/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-28 18:35:19.219811 logninja-0.1.7/logninja/
+-rw-r--r--   0 runner    (1001) docker     (127)     1254 2024-05-28 18:35:15.000000 logninja-0.1.7/logninja/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-28 18:35:19.219811 logninja-0.1.7/logninja/asgi/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-28 18:35:15.000000 logninja-0.1.7/logninja/asgi/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4034 2024-05-28 18:35:15.000000 logninja-0.1.7/logninja/asgi/middleware.py
+-rw-r--r--   0 runner    (1001) docker     (127)      280 2024-05-28 18:35:15.000000 logninja-0.1.7/logninja/configs.py
+-rw-r--r--   0 runner    (1001) docker     (127)      134 2024-05-28 18:35:15.000000 logninja-0.1.7/logninja/console_formatter.py
+-rw-r--r--   0 runner    (1001) docker     (127)      456 2024-05-28 18:35:15.000000 logninja-0.1.7/logninja/contextvars_filter.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1427 2024-05-28 18:35:15.000000 logninja-0.1.7/logninja/decorators.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1749 2024-05-28 18:35:15.000000 logninja-0.1.7/logninja/json_formatter.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5705 2024-05-28 18:35:15.000000 logninja-0.1.7/logninja/traceback.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-28 18:35:19.219811 logninja-0.1.7/logninja.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     7676 2024-05-28 18:35:19.000000 logninja-0.1.7/logninja.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      448 2024-05-28 18:35:19.000000 logninja-0.1.7/logninja.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-28 18:35:19.000000 logninja-0.1.7/logninja.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       39 2024-05-28 18:35:19.000000 logninja-0.1.7/logninja.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        9 2024-05-28 18:35:19.000000 logninja-0.1.7/logninja.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      858 2024-05-28 18:35:15.000000 logninja-0.1.7/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-28 18:35:19.219811 logninja-0.1.7/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-28 18:35:19.219811 logninja-0.1.7/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)     1217 2024-05-28 18:35:15.000000 logninja-0.1.7/tests/test_json_formatter.py
```

### Comparing `logninja-0.1.6/LICENSE` & `logninja-0.1.7/LICENSE`

 * *Files identical despite different names*

### Comparing `logninja-0.1.6/PKG-INFO` & `logninja-0.1.7/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: logninja
-Version: 0.1.6
+Version: 0.1.7
 Summary: A log configuration library for Python projects.
 Author-email: Pedro Cantidio <ppcantidio@gmail.com>
 Project-URL: homepage, https://github.com/ppcantidio/logninja.py
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
@@ -231,7 +231,10 @@
         }
       ]
     }
   ]
 }
 ```
 **Important Notice**: This functionality contains code derived from the `structlog` project, available at https://github.com/hynek/structlog. Changes were made starting from May 24th, 2024. The original code is licensed under the MIT License or Apache-2.0. Please ensure to comply with these licenses when using LogNinja.
+
+## License
+This project is licensed under the terms of the MIT license.
```

### Comparing `logninja-0.1.6/README.md` & `logninja-0.1.7/README.md`

 * *Files 1% similar despite different names*

```diff
@@ -209,8 +209,11 @@
           ]
         }
       ]
     }
   ]
 }
 ```
-**Important Notice**: This functionality contains code derived from the `structlog` project, available at https://github.com/hynek/structlog. Changes were made starting from May 24th, 2024. The original code is licensed under the MIT License or Apache-2.0. Please ensure to comply with these licenses when using LogNinja.
+**Important Notice**: This functionality contains code derived from the `structlog` project, available at https://github.com/hynek/structlog. Changes were made starting from May 24th, 2024. The original code is licensed under the MIT License or Apache-2.0. Please ensure to comply with these licenses when using LogNinja.
+
+## License
+This project is licensed under the terms of the MIT license.
```

### Comparing `logninja-0.1.6/logninja/asgi/middleware.py` & `logninja-0.1.7/logninja/asgi/middleware.py`

 * *Files identical despite different names*

### Comparing `logninja-0.1.6/logninja/decorators.py` & `logninja-0.1.7/logninja/decorators.py`

 * *Files identical despite different names*

### Comparing `logninja-0.1.6/logninja/json_formatter.py` & `logninja-0.1.7/logninja/json_formatter.py`

 * *Files identical despite different names*

### Comparing `logninja-0.1.6/logninja/traceback.py` & `logninja-0.1.7/logninja/traceback.py`

 * *Files identical despite different names*

### Comparing `logninja-0.1.6/logninja.egg-info/PKG-INFO` & `logninja-0.1.7/logninja.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: logninja
-Version: 0.1.6
+Version: 0.1.7
 Summary: A log configuration library for Python projects.
 Author-email: Pedro Cantidio <ppcantidio@gmail.com>
 Project-URL: homepage, https://github.com/ppcantidio/logninja.py
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
@@ -231,7 +231,10 @@
         }
       ]
     }
   ]
 }
 ```
 **Important Notice**: This functionality contains code derived from the `structlog` project, available at https://github.com/hynek/structlog. Changes were made starting from May 24th, 2024. The original code is licensed under the MIT License or Apache-2.0. Please ensure to comply with these licenses when using LogNinja.
+
+## License
+This project is licensed under the terms of the MIT license.
```

### Comparing `logninja-0.1.6/pyproject.toml` & `logninja-0.1.7/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 [build-system]
 requires = ["setuptools", "wheel"]
 
 [project]
 name = "logninja"
-version = "0.1.6"
+version = "0.1.7"
 authors = [{ name = "Pedro Cantidio", email = "ppcantidio@gmail.com" }]
 description = "A log configuration library for Python projects."
 readme = "README.md"
 classifiers = [
     "Development Status :: 3 - Alpha",
     "Intended Audience :: Developers",
     "License :: OSI Approved :: MIT License",
```

### Comparing `logninja-0.1.6/tests/test_json_formatter.py` & `logninja-0.1.7/tests/test_json_formatter.py`

 * *Files identical despite different names*

