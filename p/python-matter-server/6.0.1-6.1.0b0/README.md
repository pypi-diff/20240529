# Comparing `tmp/python_matter_server-6.0.1.tar.gz` & `tmp/python_matter_server-6.1.0b0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "python_matter_server-6.0.1.tar", last modified: Mon May 20 14:54:23 2024, max compression
+gzip compressed data, was "python_matter_server-6.1.0b0.tar", last modified: Wed May 29 08:45:44 2024, max compression
```

## Comparing `python_matter_server-6.0.1.tar` & `python_matter_server-6.1.0b0.tar`

### file list

```diff
@@ -1,58 +1,58 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-20 14:54:23.308885 python_matter_server-6.0.1/
--rw-r--r--   0 runner    (1001) docker     (127)    11342 2024-05-20 14:54:07.000000 python_matter_server-6.0.1/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)    14204 2024-05-20 14:54:23.308885 python_matter_server-6.0.1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)    12409 2024-05-20 14:54:07.000000 python_matter_server-6.0.1/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-20 14:54:23.300886 python_matter_server-6.0.1/matter_server/
--rw-r--r--   0 runner    (1001) docker     (127)       68 2024-05-20 14:54:07.000000 python_matter_server-6.0.1/matter_server/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-20 14:54:23.300886 python_matter_server-6.0.1/matter_server/client/
--rw-r--r--   0 runner    (1001) docker     (127)       97 2024-05-20 14:54:07.000000 python_matter_server-6.0.1/matter_server/client/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    29900 2024-05-20 14:54:07.000000 python_matter_server-6.0.1/matter_server/client/client.py
--rw-r--r--   0 runner    (1001) docker     (127)     5757 2024-05-20 14:54:07.000000 python_matter_server-6.0.1/matter_server/client/connection.py
--rw-r--r--   0 runner    (1001) docker     (127)     1622 2024-05-20 14:54:07.000000 python_matter_server-6.0.1/matter_server/client/exceptions.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-20 14:54:23.300886 python_matter_server-6.0.1/matter_server/client/models/
--rw-r--r--   0 runner    (1001) docker     (127)       63 2024-05-20 14:54:07.000000 python_matter_server-6.0.1/matter_server/client/models/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     5318 2024-05-20 14:54:07.000000 python_matter_server-6.0.1/matter_server/client/models/clusters.py
--rw-r--r--   0 runner    (1001) docker     (127)    21263 2024-05-20 14:54:07.000000 python_matter_server-6.0.1/matter_server/client/models/device_types.py
--rw-r--r--   0 runner    (1001) docker     (127)    15226 2024-05-20 14:54:07.000000 python_matter_server-6.0.1/matter_server/client/models/node.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-20 14:54:23.300886 python_matter_server-6.0.1/matter_server/common/
--rw-r--r--   0 runner    (1001) docker     (127)       50 2024-05-20 14:54:07.000000 python_matter_server-6.0.1/matter_server/common/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      255 2024-05-20 14:54:07.000000 python_matter_server-6.0.1/matter_server/common/const.py
--rw-r--r--   0 runner    (1001) docker     (127)     1878 2024-05-20 14:54:07.000000 python_matter_server-6.0.1/matter_server/common/errors.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-20 14:54:23.300886 python_matter_server-6.0.1/matter_server/common/helpers/
--rw-r--r--   0 runner    (1001) docker     (127)     2039 2024-05-20 14:54:07.000000 python_matter_server-6.0.1/matter_server/common/helpers/api.py
--rw-r--r--   0 runner    (1001) docker     (127)     1306 2024-05-20 14:54:07.000000 python_matter_server-6.0.1/matter_server/common/helpers/json.py
--rw-r--r--   0 runner    (1001) docker     (127)    12201 2024-05-20 14:54:07.000000 python_matter_server-6.0.1/matter_server/common/helpers/util.py
--rw-r--r--   0 runner    (1001) docker     (127)     5384 2024-05-20 14:54:07.000000 python_matter_server-6.0.1/matter_server/common/models.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-20 14:54:23.300886 python_matter_server-6.0.1/matter_server/dashboard/
--rw-r--r--   0 runner    (1001) docker     (127)     1102 2024-05-20 14:54:21.000000 python_matter_server-6.0.1/matter_server/dashboard/index.html
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-20 14:54:23.300886 python_matter_server-6.0.1/matter_server/dashboard/js/
--rw-r--r--   0 runner    (1001) docker     (127)    13016 2024-05-20 14:54:21.000000 python_matter_server-6.0.1/matter_server/dashboard/js/dialog-box-ztARVrB9.js
--rw-r--r--   0 runner    (1001) docker     (127)     5611 2024-05-20 14:54:21.000000 python_matter_server-6.0.1/matter_server/dashboard/js/main.js
--rw-r--r--   0 runner    (1001) docker     (127)   230455 2024-05-20 14:54:21.000000 python_matter_server-6.0.1/matter_server/dashboard/js/matter-dashboard-app-DQAdChQl.js
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-20 14:54:07.000000 python_matter_server-6.0.1/matter_server/py.typed
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-20 14:54:23.304885 python_matter_server-6.0.1/matter_server/server/
--rw-r--r--   0 runner    (1001) docker     (127)      135 2024-05-20 14:54:07.000000 python_matter_server-6.0.1/matter_server/server/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     6123 2024-05-20 14:54:07.000000 python_matter_server-6.0.1/matter_server/server/__main__.py
--rw-r--r--   0 runner    (1001) docker     (127)     9307 2024-05-20 14:54:07.000000 python_matter_server-6.0.1/matter_server/server/client_handler.py
--rw-r--r--   0 runner    (1001) docker     (127)      641 2024-05-20 14:54:07.000000 python_matter_server-6.0.1/matter_server/server/const.py
--rw-r--r--   0 runner    (1001) docker     (127)    62667 2024-05-20 14:54:07.000000 python_matter_server-6.0.1/matter_server/server/device_controller.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-20 14:54:23.304885 python_matter_server-6.0.1/matter_server/server/helpers/
--rw-r--r--   0 runner    (1001) docker     (127)       43 2024-05-20 14:54:07.000000 python_matter_server-6.0.1/matter_server/server/helpers/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1062 2024-05-20 14:54:07.000000 python_matter_server-6.0.1/matter_server/server/helpers/attributes.py
--rw-r--r--   0 runner    (1001) docker     (127)     2084 2024-05-20 14:54:07.000000 python_matter_server-6.0.1/matter_server/server/helpers/custom_web_runner.py
--rw-r--r--   0 runner    (1001) docker     (127)     9147 2024-05-20 14:54:07.000000 python_matter_server-6.0.1/matter_server/server/helpers/paa_certificates.py
--rw-r--r--   0 runner    (1001) docker     (127)     1672 2024-05-20 14:54:07.000000 python_matter_server-6.0.1/matter_server/server/helpers/utils.py
--rw-r--r--   0 runner    (1001) docker     (127)    11456 2024-05-20 14:54:07.000000 python_matter_server-6.0.1/matter_server/server/server.py
--rw-r--r--   0 runner    (1001) docker     (127)     5154 2024-05-20 14:54:07.000000 python_matter_server-6.0.1/matter_server/server/stack.py
--rw-r--r--   0 runner    (1001) docker     (127)     5406 2024-05-20 14:54:07.000000 python_matter_server-6.0.1/matter_server/server/storage.py
--rw-r--r--   0 runner    (1001) docker     (127)     4851 2024-05-20 14:54:07.000000 python_matter_server-6.0.1/matter_server/server/vendor_info.py
--rw-r--r--   0 runner    (1001) docker     (127)     4779 2024-05-20 14:54:09.000000 python_matter_server-6.0.1/pyproject.toml
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-20 14:54:23.304885 python_matter_server-6.0.1/python_matter_server.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)    14204 2024-05-20 14:54:23.000000 python_matter_server-6.0.1/python_matter_server.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     1626 2024-05-20 14:54:23.000000 python_matter_server-6.0.1/python_matter_server.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-20 14:54:23.000000 python_matter_server-6.0.1/python_matter_server.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       69 2024-05-20 14:54:23.000000 python_matter_server-6.0.1/python_matter_server.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-20 14:54:23.000000 python_matter_server-6.0.1/python_matter_server.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (127)      469 2024-05-20 14:54:23.000000 python_matter_server-6.0.1/python_matter_server.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       14 2024-05-20 14:54:23.000000 python_matter_server-6.0.1/python_matter_server.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-20 14:54:23.308885 python_matter_server-6.0.1/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-29 08:45:44.001897 python_matter_server-6.1.0b0/
+-rw-r--r--   0 runner    (1001) docker     (127)    11342 2024-05-29 08:45:20.000000 python_matter_server-6.1.0b0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)    14206 2024-05-29 08:45:44.001897 python_matter_server-6.1.0b0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)    12409 2024-05-29 08:45:20.000000 python_matter_server-6.1.0b0/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-29 08:45:43.993897 python_matter_server-6.1.0b0/matter_server/
+-rw-r--r--   0 runner    (1001) docker     (127)       68 2024-05-29 08:45:20.000000 python_matter_server-6.1.0b0/matter_server/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-29 08:45:43.993897 python_matter_server-6.1.0b0/matter_server/client/
+-rw-r--r--   0 runner    (1001) docker     (127)       97 2024-05-29 08:45:20.000000 python_matter_server-6.1.0b0/matter_server/client/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    29159 2024-05-29 08:45:20.000000 python_matter_server-6.1.0b0/matter_server/client/client.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5757 2024-05-29 08:45:20.000000 python_matter_server-6.1.0b0/matter_server/client/connection.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1622 2024-05-29 08:45:20.000000 python_matter_server-6.1.0b0/matter_server/client/exceptions.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-29 08:45:43.993897 python_matter_server-6.1.0b0/matter_server/client/models/
+-rw-r--r--   0 runner    (1001) docker     (127)       63 2024-05-29 08:45:20.000000 python_matter_server-6.1.0b0/matter_server/client/models/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    21263 2024-05-29 08:45:20.000000 python_matter_server-6.1.0b0/matter_server/client/models/device_types.py
+-rw-r--r--   0 runner    (1001) docker     (127)    15226 2024-05-29 08:45:20.000000 python_matter_server-6.1.0b0/matter_server/client/models/node.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-29 08:45:43.993897 python_matter_server-6.1.0b0/matter_server/common/
+-rw-r--r--   0 runner    (1001) docker     (127)       50 2024-05-29 08:45:20.000000 python_matter_server-6.1.0b0/matter_server/common/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      255 2024-05-29 08:45:20.000000 python_matter_server-6.1.0b0/matter_server/common/const.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7641 2024-05-29 08:45:20.000000 python_matter_server-6.1.0b0/matter_server/common/custom_clusters.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1890 2024-05-29 08:45:20.000000 python_matter_server-6.1.0b0/matter_server/common/errors.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-29 08:45:43.993897 python_matter_server-6.1.0b0/matter_server/common/helpers/
+-rw-r--r--   0 runner    (1001) docker     (127)     2039 2024-05-29 08:45:20.000000 python_matter_server-6.1.0b0/matter_server/common/helpers/api.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1306 2024-05-29 08:45:20.000000 python_matter_server-6.1.0b0/matter_server/common/helpers/json.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12201 2024-05-29 08:45:20.000000 python_matter_server-6.1.0b0/matter_server/common/helpers/util.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5336 2024-05-29 08:45:20.000000 python_matter_server-6.1.0b0/matter_server/common/models.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-29 08:45:43.993897 python_matter_server-6.1.0b0/matter_server/dashboard/
+-rw-r--r--   0 runner    (1001) docker     (127)     1102 2024-05-29 08:45:41.000000 python_matter_server-6.1.0b0/matter_server/dashboard/index.html
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-29 08:45:43.993897 python_matter_server-6.1.0b0/matter_server/dashboard/js/
+-rw-r--r--   0 runner    (1001) docker     (127)    13016 2024-05-29 08:45:41.000000 python_matter_server-6.1.0b0/matter_server/dashboard/js/dialog-box-ztARVrB9.js
+-rw-r--r--   0 runner    (1001) docker     (127)     5611 2024-05-29 08:45:41.000000 python_matter_server-6.1.0b0/matter_server/dashboard/js/main.js
+-rw-r--r--   0 runner    (1001) docker     (127)   230455 2024-05-29 08:45:41.000000 python_matter_server-6.1.0b0/matter_server/dashboard/js/matter-dashboard-app-DQAdChQl.js
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-29 08:45:20.000000 python_matter_server-6.1.0b0/matter_server/py.typed
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-29 08:45:43.997897 python_matter_server-6.1.0b0/matter_server/server/
+-rw-r--r--   0 runner    (1001) docker     (127)      135 2024-05-29 08:45:20.000000 python_matter_server-6.1.0b0/matter_server/server/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5698 2024-05-29 08:45:20.000000 python_matter_server-6.1.0b0/matter_server/server/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9307 2024-05-29 08:45:20.000000 python_matter_server-6.1.0b0/matter_server/server/client_handler.py
+-rw-r--r--   0 runner    (1001) docker     (127)      641 2024-05-29 08:45:20.000000 python_matter_server-6.1.0b0/matter_server/server/const.py
+-rw-r--r--   0 runner    (1001) docker     (127)    66771 2024-05-29 08:45:20.000000 python_matter_server-6.1.0b0/matter_server/server/device_controller.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-29 08:45:43.997897 python_matter_server-6.1.0b0/matter_server/server/helpers/
+-rw-r--r--   0 runner    (1001) docker     (127)       43 2024-05-29 08:45:20.000000 python_matter_server-6.1.0b0/matter_server/server/helpers/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1062 2024-05-29 08:45:20.000000 python_matter_server-6.1.0b0/matter_server/server/helpers/attributes.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2084 2024-05-29 08:45:20.000000 python_matter_server-6.1.0b0/matter_server/server/helpers/custom_web_runner.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9147 2024-05-29 08:45:20.000000 python_matter_server-6.1.0b0/matter_server/server/helpers/paa_certificates.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1672 2024-05-29 08:45:20.000000 python_matter_server-6.1.0b0/matter_server/server/helpers/utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11456 2024-05-29 08:45:20.000000 python_matter_server-6.1.0b0/matter_server/server/server.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5154 2024-05-29 08:45:20.000000 python_matter_server-6.1.0b0/matter_server/server/stack.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5406 2024-05-29 08:45:20.000000 python_matter_server-6.1.0b0/matter_server/server/storage.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4851 2024-05-29 08:45:20.000000 python_matter_server-6.1.0b0/matter_server/server/vendor_info.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4781 2024-05-29 08:45:29.000000 python_matter_server-6.1.0b0/pyproject.toml
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-29 08:45:43.997897 python_matter_server-6.1.0b0/python_matter_server.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)    14206 2024-05-29 08:45:43.000000 python_matter_server-6.1.0b0/python_matter_server.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     1626 2024-05-29 08:45:43.000000 python_matter_server-6.1.0b0/python_matter_server.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-29 08:45:43.000000 python_matter_server-6.1.0b0/python_matter_server.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       69 2024-05-29 08:45:43.000000 python_matter_server-6.1.0b0/python_matter_server.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-29 08:45:43.000000 python_matter_server-6.1.0b0/python_matter_server.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (127)      469 2024-05-29 08:45:43.000000 python_matter_server-6.1.0b0/python_matter_server.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       14 2024-05-29 08:45:43.000000 python_matter_server-6.1.0b0/python_matter_server.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-29 08:45:44.001897 python_matter_server-6.1.0b0/setup.cfg
```

### Comparing `python_matter_server-6.0.1/LICENSE` & `python_matter_server-6.1.0b0/LICENSE`

 * *Files identical despite different names*

### Comparing `python_matter_server-6.0.1/PKG-INFO` & `python_matter_server-6.1.0b0/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: python-matter-server
-Version: 6.0.1
+Version: 6.1.0b0
 Summary: Python Matter WebSocket Server
 Author-email: The Home Assistant Authors <hello@home-assistant.io>
 License: Apache-2.0
 Platform: any
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Developers
 Classifier: Environment :: Console
@@ -15,36 +15,36 @@
 Description-Content-Type: text/markdown
 License-File: LICENSE
 Requires-Dist: aiohttp
 Requires-Dist: aiorun
 Requires-Dist: async-timeout
 Requires-Dist: coloredlogs
 Requires-Dist: orjson
-Requires-Dist: home-assistant-chip-clusters==2024.5.0
+Requires-Dist: home-assistant-chip-clusters==2024.5.1
 Provides-Extra: server
 Requires-Dist: aiohttp==3.9.5; extra == "server"
 Requires-Dist: aiorun==2024.5.1; extra == "server"
 Requires-Dist: async-timeout==4.0.3; extra == "server"
 Requires-Dist: coloredlogs==15.0.1; extra == "server"
 Requires-Dist: cryptography==42.0.7; extra == "server"
 Requires-Dist: orjson==3.10.3; extra == "server"
 Requires-Dist: zeroconf==0.132.2; extra == "server"
-Requires-Dist: home-assistant-chip-core==2024.5.0; extra == "server"
+Requires-Dist: home-assistant-chip-core==2024.5.1; extra == "server"
 Provides-Extra: test
-Requires-Dist: codespell==2.2.6; extra == "test"
+Requires-Dist: codespell==2.3.0; extra == "test"
 Requires-Dist: isort==5.13.2; extra == "test"
 Requires-Dist: mypy==1.10.0; extra == "test"
 Requires-Dist: pre-commit==3.7.1; extra == "test"
 Requires-Dist: pre-commit-hooks==4.6.0; extra == "test"
 Requires-Dist: pylint==3.2.2; extra == "test"
 Requires-Dist: pytest==8.2.1; extra == "test"
 Requires-Dist: pytest-asyncio==0.23.7; extra == "test"
 Requires-Dist: pytest-aiohttp==1.0.5; extra == "test"
 Requires-Dist: pytest-cov==5.0.0; extra == "test"
-Requires-Dist: ruff==0.4.4; extra == "test"
+Requires-Dist: ruff==0.4.5; extra == "test"
 Requires-Dist: tomli==2.0.1; extra == "test"
 
 # Python Matter Server
 
 This project implements a Matter Controller Server over WebSockets using the
 [official Matter (formerly CHIP) SDK](https://github.com/project-chip/connectedhomeip)
 as a base and provides both a server and client implementation.
```

### Comparing `python_matter_server-6.0.1/README.md` & `python_matter_server-6.1.0b0/README.md`

 * *Files identical despite different names*

### Comparing `python_matter_server-6.0.1/matter_server/client/client.py` & `python_matter_server-6.1.0b0/matter_server/client/client.py`

 * *Files 2% similar despite different names*

```diff
@@ -459,26 +459,23 @@
             timed_request_timeout_ms=timed_request_timeout_ms,
             interaction_timeout_ms=interaction_timeout_ms,
         )
 
     async def read_attribute(
         self,
         node_id: int,
-        attribute_path: str,
+        attribute_path: str | list[str],
     ) -> dict[str, Any]:
         """Read one or more attribute(s) on a node by specifying an attributepath."""
         updated_values = await self.send_command(
             APICommand.READ_ATTRIBUTE,
-            require_schema=4,
+            require_schema=9,
             node_id=node_id,
             attribute_path=attribute_path,
         )
-        if not isinstance(updated_values, dict):
-            # can happen is the server is running schema < 8
-            return {attribute_path: updated_values}
         return cast(dict[str, Any], updated_values)
 
     async def refresh_attribute(
         self,
         node_id: int,
         attribute_path: str,
     ) -> None:
@@ -506,31 +503,14 @@
         """Remove a Matter node/device from the fabric."""
         await self.send_command(APICommand.REMOVE_NODE, node_id=node_id)
 
     async def interview_node(self, node_id: int) -> None:
         """Interview a node."""
         await self.send_command(APICommand.INTERVIEW_NODE, node_id=node_id)
 
-    async def subscribe_attribute(
-        self, node_id: int, attribute_path: str | list[str]
-    ) -> None:
-        """
-        Subscribe to given AttributePath(s).
-
-        Either supply a single attribute path or a list of paths.
-        The given attribute path(s) will be added to the list of attributes that
-        are watched for the given node. This is persistent over restarts.
-        """
-        await self.send_command(
-            APICommand.SUBSCRIBE_ATTRIBUTE,
-            require_schema=4,
-            node_id=node_id,
-            attribute_path=attribute_path,
-        )
-
     async def send_command(
         self,
         command: str,
         require_schema: int | None = None,
         **kwargs: Any,
     ) -> Any:
         """Send a command and get a response."""
```

### Comparing `python_matter_server-6.0.1/matter_server/client/connection.py` & `python_matter_server-6.1.0b0/matter_server/client/connection.py`

 * *Files identical despite different names*

### Comparing `python_matter_server-6.0.1/matter_server/client/exceptions.py` & `python_matter_server-6.1.0b0/matter_server/client/exceptions.py`

 * *Files identical despite different names*

### Comparing `python_matter_server-6.0.1/matter_server/client/models/device_types.py` & `python_matter_server-6.1.0b0/matter_server/client/models/device_types.py`

 * *Files identical despite different names*

### Comparing `python_matter_server-6.0.1/matter_server/client/models/node.py` & `python_matter_server-6.1.0b0/matter_server/client/models/node.py`

 * *Files identical despite different names*

### Comparing `python_matter_server-6.0.1/matter_server/common/errors.py` & `python_matter_server-6.1.0b0/matter_server/common/errors.py`

 * *Files 5% similar despite different names*

```diff
@@ -38,15 +38,15 @@
 class NodeNotReady(MatterError):
     """Error raised when performing action on node that has not been fully added."""
 
     error_code = 3
 
 
 class NodeNotResolving(MatterError):
-    """Error raised when resolving the node fails."""
+    """Error raised when no CASE session could be established."""
 
     error_code = 4
 
 
 class NodeNotExists(MatterError):
     """Error raised when performing action on node that does not exist."""
```

### Comparing `python_matter_server-6.0.1/matter_server/common/helpers/api.py` & `python_matter_server-6.1.0b0/matter_server/common/helpers/api.py`

 * *Files identical despite different names*

### Comparing `python_matter_server-6.0.1/matter_server/common/helpers/json.py` & `python_matter_server-6.1.0b0/matter_server/common/helpers/json.py`

 * *Files identical despite different names*

### Comparing `python_matter_server-6.0.1/matter_server/common/helpers/util.py` & `python_matter_server-6.1.0b0/matter_server/common/helpers/util.py`

 * *Files identical despite different names*

### Comparing `python_matter_server-6.0.1/matter_server/common/models.py` & `python_matter_server-6.1.0b0/matter_server/common/models.py`

 * *Files 4% similar despite different names*

```diff
@@ -38,15 +38,14 @@
     SET_THREAD_DATASET = "set_thread_dataset"
     OPEN_COMMISSIONING_WINDOW = "open_commissioning_window"
     DISCOVER = "discover"
     INTERVIEW_NODE = "interview_node"
     DEVICE_COMMAND = "device_command"
     REMOVE_NODE = "remove_node"
     GET_VENDOR_NAMES = "get_vendor_names"
-    SUBSCRIBE_ATTRIBUTE = "subscribe_attribute"
     READ_ATTRIBUTE = "read_attribute"
     WRITE_ATTRIBUTE = "write_attribute"
     PING_NODE = "ping_node"
     GET_NODE_IP_ADRESSES = "get_node_ip_addresses"
     IMPORT_TEST_NODE = "import_test_node"
```

### Comparing `python_matter_server-6.0.1/matter_server/dashboard/index.html` & `python_matter_server-6.1.0b0/matter_server/dashboard/index.html`

 * *Files identical despite different names*

### Comparing `python_matter_server-6.0.1/matter_server/dashboard/js/dialog-box-ztARVrB9.js` & `python_matter_server-6.1.0b0/matter_server/dashboard/js/dialog-box-ztARVrB9.js`

 * *Files identical despite different names*

### Comparing `python_matter_server-6.0.1/matter_server/dashboard/js/main.js` & `python_matter_server-6.1.0b0/matter_server/dashboard/js/main.js`

 * *Files identical despite different names*

### Comparing `python_matter_server-6.0.1/matter_server/dashboard/js/matter-dashboard-app-DQAdChQl.js` & `python_matter_server-6.1.0b0/matter_server/dashboard/js/matter-dashboard-app-DQAdChQl.js`

 * *Files identical despite different names*

### Comparing `python_matter_server-6.0.1/matter_server/server/__main__.py` & `python_matter_server-6.1.0b0/matter_server/server/__main__.py`

 * *Files 3% similar despite different names*

```diff
@@ -140,19 +140,14 @@
         logger.addHandler(file_handler)
 
     stack.init_logging(args.log_level_sdk.upper())
     logger.setLevel(args.log_level.upper())
 
     if not logger.isEnabledFor(VERBOSE_LOG_LEVEL):
         logging.getLogger("PersistentStorage").setLevel(logging.WARNING)
-        # Temporary disable the logger of chip.clusters.Attribute because it now logs
-        # an error on every custom attribute that couldn't be parsed which confuses people.
-        # We can restore the default log level again when we've patched the device controller
-        # to handle the raw attribute data to deal with custom clusters.
-        logging.getLogger("chip.clusters.Attribute").setLevel(logging.CRITICAL)
         # (temporary) raise the log level of zeroconf as its a logs an annoying
         # warning at startup while trying to bind to a loopback IPv6 interface
         logging.getLogger("zeroconf").setLevel(logging.ERROR)
 
     # register global uncaught exception loggers
     sys.excepthook = lambda *args: logger.exception(
         "Uncaught exception",
```

### Comparing `python_matter_server-6.0.1/matter_server/server/client_handler.py` & `python_matter_server-6.1.0b0/matter_server/server/client_handler.py`

 * *Files identical despite different names*

### Comparing `python_matter_server-6.0.1/matter_server/server/const.py` & `python_matter_server-6.1.0b0/matter_server/server/const.py`

 * *Files identical despite different names*

### Comparing `python_matter_server-6.0.1/matter_server/server/device_controller.py` & `python_matter_server-6.1.0b0/matter_server/server/device_controller.py`

 * *Files 4% similar despite different names*

```diff
@@ -18,14 +18,15 @@
 from chip.clusters.ClusterObjects import ALL_ATTRIBUTES, ALL_CLUSTERS, Cluster
 from chip.discovery import DiscoveryType
 from chip.exceptions import ChipStackError
 from zeroconf import BadTypeInNameException, IPVersion, ServiceStateChange, Zeroconf
 from zeroconf.asyncio import AsyncServiceBrowser, AsyncServiceInfo, AsyncZeroconf
 
 from matter_server.common.const import VERBOSE_LOG_LEVEL
+from matter_server.common.custom_clusters import check_polled_attributes
 from matter_server.common.models import CommissionableNodeData, CommissioningParameters
 from matter_server.server.helpers.attributes import parse_attributes_from_read_result
 from matter_server.server.helpers.utils import ping_ip
 
 from ..common.errors import (
     InvalidArguments,
     NodeCommissionFailed,
@@ -73,23 +74,32 @@
 MAX_COMMISSION_RETRIES = 3
 NODE_RESUBSCRIBE_ATTEMPTS_UNAVAILABLE = 3
 NODE_RESUBSCRIBE_TIMEOUT_OFFLINE = 30 * 60 * 1000
 NODE_PING_TIMEOUT = 10
 NODE_PING_TIMEOUT_BATTERY_POWERED = 60
 NODE_MDNS_BACKOFF = 610  # must be higher than (highest) sub ceiling
 FALLBACK_NODE_SCANNER_INTERVAL = 1800
+CUSTOM_ATTRIBUTES_POLLER_INTERVAL = 30
 
 MDNS_TYPE_OPERATIONAL_NODE = "_matter._tcp.local."
 MDNS_TYPE_COMMISSIONABLE_NODE = "_matterc._udp.local."
 
 TEST_NODE_START = 900000
 
 ROUTING_ROLE_ATTRIBUTE_PATH = create_attribute_path_from_attribute(
     0, Clusters.ThreadNetworkDiagnostics.Attributes.RoutingRole
 )
+DESCRIPTOR_PARTS_LIST_ATTRIBUTE_PATH = create_attribute_path_from_attribute(
+    0, Clusters.Descriptor.Attributes.PartsList
+)
+BASIC_INFORMATION_SOFTWARE_VERSION_ATTRIBUTE_PATH = (
+    create_attribute_path_from_attribute(
+        0, Clusters.BasicInformation.Attributes.SoftwareVersion
+    )
+)
 
 
 # pylint: disable=too-many-lines,too-many-locals,too-many-statements,too-many-branches,too-many-instance-attributes
 
 
 class MatterDeviceController:
     """Class that manages the Matter devices."""
@@ -118,14 +128,17 @@
         self._aiobrowser: AsyncServiceBrowser | None = None
         self._aiozc: AsyncZeroconf | None = None
         self._fallback_node_scanner_timer: asyncio.TimerHandle | None = None
         self._fallback_node_scanner_task: asyncio.Task | None = None
         self._node_setup_throttle = asyncio.Semaphore(5)
         self._mdns_event_timer: dict[str, asyncio.TimerHandle] = {}
         self._node_lock: dict[int, asyncio.Lock] = {}
+        self._polled_attributes: dict[int, set[str]] = {}
+        self._custom_attribute_poller_timer: asyncio.TimerHandle | None = None
+        self._custom_attribute_poller_task: asyncio.Task | None = None
 
     async def initialize(self, paa_root_cert_dir: Path) -> None:
         """Async initialize of controller."""
         # (re)fetch all PAA certificates once at startup
         # NOTE: this must be done before initializing the controller
         await fetch_certificates(paa_root_cert_dir)
 
@@ -601,63 +614,94 @@
                 responseType=response_type,
                 timedRequestTimeoutMs=timed_request_timeout_ms,
                 interactionTimeoutMs=interaction_timeout_ms,
             )
 
     @api_command(APICommand.READ_ATTRIBUTE)
     async def read_attribute(
-        self, node_id: int, attribute_path: str, fabric_filtered: bool = False
+        self,
+        node_id: int,
+        attribute_path: str | list[str],
+        fabric_filtered: bool = False,
     ) -> dict[str, Any]:
-        """Read one or more attribute(s) on a node by specifying an attributepath."""
+        """
+        Read one or more attribute(s) on a node by specifying an attributepath.
+
+        The attribute path can be a single string or a list of strings.
+        The attribute path may contain wildcards (*) for cluster and/or attribute id.
+
+        The return type is a dictionary with the attribute path as key and the value as value.
+        """
         if self.chip_controller is None:
             raise RuntimeError("Device Controller not initialized.")
         if (node := self._nodes.get(node_id)) is None or not node.available:
             raise NodeNotReady(f"Node {node_id} is not (yet) available.")
-        endpoint_id, cluster_id, attribute_id = parse_attribute_path(attribute_path)
-        # Read a list of attributes and/or events from a target node.
-        # This is basically a re-implementation of the chip controller's Read function
-        # but one that allows us to send/request custom attributes.
+        attribute_paths = (
+            attribute_path if isinstance(attribute_path, list) else [attribute_path]
+        )
 
         if TYPE_CHECKING:
             assert self.server.loop
             assert self.chip_controller
 
+        # handle test node
         if node_id >= TEST_NODE_START:
             LOGGER.debug(
-                "read_attribute called for test node %s on path: %s - fabric_filtered: %s",
+                "read_attribute called for test node %s on path(s): %s - fabric_filtered: %s",
                 node_id,
-                attribute_path,
+                str(attribute_paths),
                 fabric_filtered,
             )
-            if attribute_path in self._nodes[node_id].attributes:
-                return {attribute_path: self._nodes[node_id].attributes[attribute_path]}
-            return {}
+            return {
+                attr_path: self._nodes[node_id].attributes.get(attr_path)
+                for attr_path in attribute_paths
+            }
 
+        # parse text based attribute paths into the SDK Attribute Path objects
+        attributes: list[Attribute.AttributePath] = []
+        for attr_path in attribute_paths:
+            endpoint_id, cluster_id, attribute_id = parse_attribute_path(attr_path)
+            attributes.append(
+                Attribute.AttributePath(
+                    EndpointId=endpoint_id,
+                    ClusterId=cluster_id,
+                    AttributeId=attribute_id,
+                )
+            )
+        # Read a list of attributes and/or events from a target node.
+        # This is basically a re-implementation of the chip controller's Read function
+        # but one that allows us to send/request custom attributes.
         future = self.server.loop.create_future()
-        device = await self._resolve_node(node_id)
+        device = await self._find_or_establish_case_session(node_id)
         async with self._get_node_lock(node_id):
             Attribute.Read(
                 future=future,
                 eventLoop=self.server.loop,
                 device=device.deviceProxy,
                 devCtrl=self.chip_controller,
-                attributes=[
-                    Attribute.AttributePath(
-                        EndpointId=endpoint_id,
-                        ClusterId=cluster_id,
-                        AttributeId=attribute_id,
-                    )
-                ],
+                attributes=attributes,
                 fabricFiltered=fabric_filtered,
             ).raise_on_error()
             result: Attribute.AsyncReadTransaction.ReadResponse = await future
         read_atributes = parse_attributes_from_read_result(result.tlvAttributes)
-        # update cached info in node attributes
-        self._nodes[node_id].attributes.update(read_atributes)
-        self._write_node_state(node_id)
+        # update cached info in node attributes and signal events for updated attributes
+        values_changed = False
+        for attr_path, value in read_atributes.items():
+            if node.attributes.get(attr_path) != value:
+                node.attributes[attr_path] = value
+                self.server.signal_event(
+                    EventType.ATTRIBUTE_UPDATED,
+                    # send data as tuple[node_id, attribute_path, new_value]
+                    (node_id, attr_path, value),
+                )
+
+                values_changed = True
+        # schedule writing of the node state if any values changed
+        if values_changed:
+            self._write_node_state(node_id)
         return read_atributes
 
     @api_command(APICommand.WRITE_ATTRIBUTE)
     async def write_attribute(
         self,
         node_id: int,
         attribute_path: str,
@@ -756,30 +800,14 @@
             LOGGER.info("Successfully removed Home Assistant fabric from device.")
         else:
             LOGGER.warning(
                 "Removing current fabric from device failed with status code %d.",
                 result.statusCode,
             )
 
-    @api_command(APICommand.SUBSCRIBE_ATTRIBUTE)
-    async def subscribe_attribute(
-        self, node_id: int, attribute_path: str | list[str]
-    ) -> None:
-        """
-        Subscribe to given AttributePath(s).
-
-        Either supply a single attribute path or a list of paths.
-        The given attribute path(s) will be added to the list of attributes that
-        are watched for the given node. This is persistent over restarts.
-        """
-        LOGGER.debug(
-            "The subscribe_attribute command has been deprecated and will be removed from"
-            " a future version. You no longer need to call this to subscribe to attribute changes."
-        )
-
     @api_command(APICommand.PING_NODE)
     async def ping_node(self, node_id: int, attempts: int = 1) -> NodePingResult:
         """Ping node on the currently known IP-adress(es)."""
         result: NodePingResult = {}
         if node_id >= TEST_NODE_START:
             return {"0.0.0.0": True, "0000:1111:2222:3333:4444": True}
         node = self._nodes.get(node_id)
@@ -917,77 +945,71 @@
             node_logger.info("Unsubscribing from existing subscription.")
             await self._call_sdk(prev_sub.Shutdown)
             del self._subscriptions[node_id]
 
         loop = cast(asyncio.AbstractEventLoop, self.server.loop)
 
         def attribute_updated(
-            path: Attribute.TypedAttributePath,
+            path: Attribute.AttributePath,
             old_value: Any,
             new_value: Any,
         ) -> None:
             node_logger.log(
                 VERBOSE_LOG_LEVEL,
                 "Attribute updated: %s - old value: %s - new value: %s",
                 path,
                 old_value,
                 new_value,
             )
 
             # work out added/removed endpoints on bridges
-            if (
-                node.is_bridge
-                and path.Path.EndpointId == 0
-                and path.AttributeType == Clusters.Descriptor.Attributes.PartsList
-            ):
+            if node.is_bridge and str(path) == DESCRIPTOR_PARTS_LIST_ATTRIBUTE_PATH:
                 endpoints_removed = set(old_value or []) - set(new_value)
                 endpoints_added = set(new_value) - set(old_value or [])
                 if endpoints_removed:
                     self._handle_endpoints_removed(node_id, endpoints_removed)
                 if endpoints_added:
                     loop.create_task(
                         self._handle_endpoints_added(node_id, endpoints_added)
                     )
                 return
 
             # work out if software version changed
             if (
-                path.AttributeType == Clusters.BasicInformation.softwareVersion
+                str(path) == BASIC_INFORMATION_SOFTWARE_VERSION_ATTRIBUTE_PATH
                 and new_value != old_value
             ):
                 # schedule a full interview of the node if the software version changed
                 loop.create_task(self.interview_node(node_id))
 
             # store updated value in node attributes
-            attr_path = str(path.Path)
-            node.attributes[attr_path] = new_value
+            node.attributes[str(path)] = new_value
 
             # schedule save to persistent storage
             self._write_node_state(node_id)
 
             # This callback is running in the CHIP stack thread
             self.server.signal_event(
                 EventType.ATTRIBUTE_UPDATED,
                 # send data as tuple[node_id, attribute_path, new_value]
-                (node_id, attr_path, new_value),
+                (node_id, str(path), new_value),
             )
 
         def attribute_updated_callback(
-            path: Attribute.TypedAttributePath,
+            path: Attribute.AttributePath,
             transaction: Attribute.SubscriptionTransaction,
         ) -> None:
             self._node_last_seen[node_id] = time.time()
-            new_value = transaction.GetAttribute(path)
+            new_value = transaction.GetTLVAttribute(path)
             # failsafe: ignore ValueDecodeErrors
             # these are set by the SDK if parsing the value failed miserably
             if isinstance(new_value, ValueDecodeFailure):
                 return
 
-            attr_path = str(path.Path)
-            old_value = node.attributes.get(attr_path)
+            old_value = node.attributes.get(str(path))
 
             # return early if the value did not actually change at all
             if old_value == new_value:
                 return
 
             loop.call_soon_threadsafe(attribute_updated, path, old_value, new_value)
 
@@ -1092,28 +1114,34 @@
                 attributes="*",
                 events=[("*", 1)],
                 returnClusterObject=False,
                 reportInterval=(interval_floor, interval_ceiling),
                 autoResubscribe=True,
             )
 
-        sub.SetAttributeUpdateCallback(attribute_updated_callback)
+        if not isinstance(sub, Attribute.SubscriptionTransaction):
+            # Aborted setups result in ReadResult instead of SubscriptionTransaction
+            # Probably a bug: https://github.com/project-chip/connectedhomeip/issues/33570
+            node_logger.warning("Subscription setup failed.")
+            return
+
+        # Make sure to clear default handler which prints to stdout
+        sub.SetAttributeUpdateCallback(None)
+        sub.SetRawAttributeUpdateCallback(attribute_updated_callback)
         sub.SetEventUpdateCallback(event_callback)
         sub.SetErrorCallback(error_callback)
         sub.SetResubscriptionAttemptedCallback(resubscription_attempted)
         sub.SetResubscriptionSucceededCallback(resubscription_succeeded)
 
         # if we reach this point, it means the node could be resolved
         # and the initial subscription succeeded, mark the node available.
         self._subscriptions[node_id] = sub
         node.available = True
         # update attributes with current state from read request
-        # NOTE: Make public method upstream for retrieving the attributeTLVCache
-        # pylint: disable=protected-access
-        tlv_attributes = sub._readTransaction._cache.attributeTLVCache
+        tlv_attributes = sub.GetTLVAttributes()
         node.attributes.update(parse_attributes_from_read_result(tlv_attributes))
 
         report_interval_floor, report_interval_ceiling = (
             sub.GetReportingIntervalsSeconds()
         )
         node_logger.info(
             "Subscription succeeded with report interval [%d, %d]",
@@ -1201,30 +1229,29 @@
                 15 * 60, log_node_long_setup, time_start
             )
             try:
                 node_logger.info("Setting-up node...")
 
                 # try to resolve the node using the sdk first before do anything else
                 try:
-                    await self._resolve_node(node_id=node_id)
+                    await self._find_or_establish_case_session(node_id=node_id)
                 except NodeNotResolving as err:
                     node_logger.warning(
                         "Setup for node failed: %s",
                         str(err) or err.__class__.__name__,
                         # log full stack trace if verbose logging is enabled
                         exc_info=err
                         if LOGGER.isEnabledFor(VERBOSE_LOG_LEVEL)
                         else None,
                     )
                     # NOTE: the node will be picked up by mdns discovery automatically
                     # when it comes available again.
                     return
 
                 # (re)interview node (only) if needed
-
                 if (
                     # re-interview if we dont have any node attributes (empty node)
                     not node_data.attributes
                     # re-interview if the data model schema has changed
                     or node_data.interview_version != DATA_MODEL_SCHEMA_VERSION
                 ):
                     try:
@@ -1252,54 +1279,64 @@
                         # log full stack trace if verbose logging is enabled
                         exc_info=err
                         if LOGGER.isEnabledFor(VERBOSE_LOG_LEVEL)
                         else None,
                     )
                     # NOTE: the node will be picked up by mdns discovery automatically
                     # when it becomes available again.
+                    return
+
+                # check if this node has any custom clusters that need to be polled
+                if polled_attributes := check_polled_attributes(node_data):
+                    self._polled_attributes[node_id] = polled_attributes
+                    self._schedule_custom_attributes_poller()
+
             finally:
                 log_timers[node_id].cancel()
                 self._nodes_in_setup.discard(node_id)
 
-    async def _resolve_node(
-        self, node_id: int, retries: int = 2, attempt: int = 1
+    async def _find_or_establish_case_session(
+        self, node_id: int, retries: int = 2
     ) -> DeviceProxyWrapper:
-        """Resolve a Node on the network."""
-        log_level = logging.DEBUG if attempt == 1 else logging.INFO
+        """Attempt to establish a CASE session with target Node."""
         if self.chip_controller is None:
             raise RuntimeError("Device Controller not initialized.")
-        try:
-            LOGGER.log(
-                log_level,
-                "Attempting to resolve node %s... (attempt %s of %s)",
-                node_id,
-                attempt,
-                retries,
-            )
-            time_start = time.time()
-            async with self._get_node_lock(node_id):
-                return await self.chip_controller.GetConnectedDevice(
-                    nodeid=node_id,
-                    allowPASE=False,
-                    timeoutMs=None,
+
+        node_logger = LOGGER.getChild(f"node_{node_id}")
+        attempt = 1
+
+        while attempt <= retries:
+            try:
+                node_logger.log(
+                    logging.DEBUG if attempt == 1 else logging.INFO,
+                    "Attempting to establish CASE session... (attempt %s of %s)",
+                    attempt,
+                    retries,
                 )
-        except ChipStackError as err:
-            if attempt >= retries:
-                # when we're out of retries, raise NodeNotResolving
-                raise NodeNotResolving(f"Unable to resolve Node {node_id}") from err
-            await asyncio.sleep(2 + attempt)
-            # retry the resolve
-            return await self._resolve_node(
-                node_id=node_id, retries=retries, attempt=attempt + 1
-            )
-        finally:
-            resolve_time_seconds = int(time.time() - time_start)
-            LOGGER.debug(
-                "Resolving node %s took %s seconds", node_id, resolve_time_seconds
-            )
+                time_start = time.time()
+                async with self._get_node_lock(node_id):
+                    return await self.chip_controller.GetConnectedDevice(
+                        nodeid=node_id,
+                        allowPASE=False,
+                        timeoutMs=None,
+                    )
+            except ChipStackError as err:
+                if attempt >= retries:
+                    # when we're out of retries, raise NodeNotResolving
+                    raise NodeNotResolving(
+                        f"Unable to establish CASE session with Node {node_id}"
+                    ) from err
+                await asyncio.sleep(2 + attempt)
+            finally:
+                node_logger.debug(
+                    "Establishing CASE session took %.1f seconds",
+                    time.time() - time_start,
+                )
+            attempt += 1
+        return None
 
     def _handle_endpoints_removed(self, node_id: int, endpoints: Iterable[int]) -> None:
         """Handle callback for when bridge endpoint(s) get deleted."""
         node = self._nodes[node_id]
         for endpoint_id in endpoints:
             node.attributes = {
                 key: value
@@ -1496,7 +1533,59 @@
         )
 
     def _get_node_lock(self, node_id: int) -> asyncio.Lock:
         """Return lock for given node."""
         if node_id not in self._node_lock:
             self._node_lock[node_id] = asyncio.Lock()
         return self._node_lock[node_id]
+
+    async def _custom_attributes_poller(self) -> None:
+        """Poll custom clusters/attributes for changes."""
+        for node_id, polled_attributes in self._polled_attributes.items():
+            node = self._nodes[node_id]
+            if not node.available:
+                continue
+            for attribute_path in polled_attributes:
+                try:
+                    # try to read the attribute(s) - this will fire an event if the value changed
+                    async with self._get_node_lock(node_id):
+                        await self.read_attribute(
+                            node_id, attribute_path, fabric_filtered=False
+                        )
+                except (ChipStackError, NodeNotReady) as err:
+                    LOGGER.warning(
+                        "Polling custom attribute %s for node %s failed: %s",
+                        attribute_path,
+                        node_id,
+                        str(err) or err.__class__.__name__,
+                        # log full stack trace if verbose logging is enabled
+                        exc_info=err
+                        if LOGGER.isEnabledFor(VERBOSE_LOG_LEVEL)
+                        else None,
+                    )
+                # polling attributes is heavy on network traffic, so we throttle it a bit
+                await asyncio.sleep(2)
+        # reschedule self to run at next interval
+        self._schedule_custom_attributes_poller()
+
+    def _schedule_custom_attributes_poller(self) -> None:
+        """Schedule running the custom clusters/attributes poller at X interval."""
+        if existing := self._custom_attribute_poller_timer:
+            existing.cancel()
+
+        def run_custom_attributes_poller() -> None:
+            self._custom_attribute_poller_timer = None
+            if (existing := self._custom_attribute_poller_task) and not existing.done():
+                existing.cancel()
+            self._custom_attribute_poller_task = asyncio.create_task(
+                self._custom_attributes_poller()
+            )
+
+        # no need to schedule the poll if we have no (more) custom attributes to poll
+        if not self._polled_attributes:
+            return
+
+        if TYPE_CHECKING:
+            assert self.server.loop
+        self._custom_attribute_poller_timer = self.server.loop.call_later(
+            CUSTOM_ATTRIBUTES_POLLER_INTERVAL, run_custom_attributes_poller
+        )
```

### Comparing `python_matter_server-6.0.1/matter_server/server/helpers/attributes.py` & `python_matter_server-6.1.0b0/matter_server/server/helpers/attributes.py`

 * *Files identical despite different names*

### Comparing `python_matter_server-6.0.1/matter_server/server/helpers/custom_web_runner.py` & `python_matter_server-6.1.0b0/matter_server/server/helpers/custom_web_runner.py`

 * *Files identical despite different names*

### Comparing `python_matter_server-6.0.1/matter_server/server/helpers/paa_certificates.py` & `python_matter_server-6.1.0b0/matter_server/server/helpers/paa_certificates.py`

 * *Files identical despite different names*

### Comparing `python_matter_server-6.0.1/matter_server/server/helpers/utils.py` & `python_matter_server-6.1.0b0/matter_server/server/helpers/utils.py`

 * *Files identical despite different names*

### Comparing `python_matter_server-6.0.1/matter_server/server/server.py` & `python_matter_server-6.1.0b0/matter_server/server/server.py`

 * *Files identical despite different names*

### Comparing `python_matter_server-6.0.1/matter_server/server/stack.py` & `python_matter_server-6.1.0b0/matter_server/server/stack.py`

 * *Files identical despite different names*

### Comparing `python_matter_server-6.0.1/matter_server/server/storage.py` & `python_matter_server-6.1.0b0/matter_server/server/storage.py`

 * *Files identical despite different names*

### Comparing `python_matter_server-6.0.1/matter_server/server/vendor_info.py` & `python_matter_server-6.1.0b0/matter_server/server/vendor_info.py`

 * *Files identical despite different names*

### Comparing `python_matter_server-6.0.1/pyproject.toml` & `python_matter_server-6.1.0b0/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -18,48 +18,48 @@
 ]
 dependencies = [
     "aiohttp",
     "aiorun",
     "async-timeout",
     "coloredlogs",
     "orjson",
-    "home-assistant-chip-clusters==2024.5.0",
+    "home-assistant-chip-clusters==2024.5.1",
 ]
 description = "Python Matter WebSocket Server"
 name = "python-matter-server"
 readme = "README.md"
 requires-python = ">=3.11"
-version = "6.0.1"
+version = "6.1.0b0"
 
 [project.license]
 text = "Apache-2.0"
 
 [project.optional-dependencies]
 server = [
     "aiohttp==3.9.5",
     "aiorun==2024.5.1",
     "async-timeout==4.0.3",
     "coloredlogs==15.0.1",
     "cryptography==42.0.7",
     "orjson==3.10.3",
     "zeroconf==0.132.2",
-    "home-assistant-chip-core==2024.5.0",
+    "home-assistant-chip-core==2024.5.1",
 ]
 test = [
-    "codespell==2.2.6",
+    "codespell==2.3.0",
     "isort==5.13.2",
     "mypy==1.10.0",
     "pre-commit==3.7.1",
     "pre-commit-hooks==4.6.0",
     "pylint==3.2.2",
     "pytest==8.2.1",
     "pytest-asyncio==0.23.7",
     "pytest-aiohttp==1.0.5",
     "pytest-cov==5.0.0",
-    "ruff==0.4.4",
+    "ruff==0.4.5",
     "tomli==2.0.1",
 ]
 
 [project.scripts]
 matter-server = "matter_server.server.__main__:main"
 
 [tool.codespell]
```

### Comparing `python_matter_server-6.0.1/python_matter_server.egg-info/PKG-INFO` & `python_matter_server-6.1.0b0/python_matter_server.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: python-matter-server
-Version: 6.0.1
+Version: 6.1.0b0
 Summary: Python Matter WebSocket Server
 Author-email: The Home Assistant Authors <hello@home-assistant.io>
 License: Apache-2.0
 Platform: any
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Developers
 Classifier: Environment :: Console
@@ -15,36 +15,36 @@
 Description-Content-Type: text/markdown
 License-File: LICENSE
 Requires-Dist: aiohttp
 Requires-Dist: aiorun
 Requires-Dist: async-timeout
 Requires-Dist: coloredlogs
 Requires-Dist: orjson
-Requires-Dist: home-assistant-chip-clusters==2024.5.0
+Requires-Dist: home-assistant-chip-clusters==2024.5.1
 Provides-Extra: server
 Requires-Dist: aiohttp==3.9.5; extra == "server"
 Requires-Dist: aiorun==2024.5.1; extra == "server"
 Requires-Dist: async-timeout==4.0.3; extra == "server"
 Requires-Dist: coloredlogs==15.0.1; extra == "server"
 Requires-Dist: cryptography==42.0.7; extra == "server"
 Requires-Dist: orjson==3.10.3; extra == "server"
 Requires-Dist: zeroconf==0.132.2; extra == "server"
-Requires-Dist: home-assistant-chip-core==2024.5.0; extra == "server"
+Requires-Dist: home-assistant-chip-core==2024.5.1; extra == "server"
 Provides-Extra: test
-Requires-Dist: codespell==2.2.6; extra == "test"
+Requires-Dist: codespell==2.3.0; extra == "test"
 Requires-Dist: isort==5.13.2; extra == "test"
 Requires-Dist: mypy==1.10.0; extra == "test"
 Requires-Dist: pre-commit==3.7.1; extra == "test"
 Requires-Dist: pre-commit-hooks==4.6.0; extra == "test"
 Requires-Dist: pylint==3.2.2; extra == "test"
 Requires-Dist: pytest==8.2.1; extra == "test"
 Requires-Dist: pytest-asyncio==0.23.7; extra == "test"
 Requires-Dist: pytest-aiohttp==1.0.5; extra == "test"
 Requires-Dist: pytest-cov==5.0.0; extra == "test"
-Requires-Dist: ruff==0.4.4; extra == "test"
+Requires-Dist: ruff==0.4.5; extra == "test"
 Requires-Dist: tomli==2.0.1; extra == "test"
 
 # Python Matter Server
 
 This project implements a Matter Controller Server over WebSockets using the
 [official Matter (formerly CHIP) SDK](https://github.com/project-chip/connectedhomeip)
 as a base and provides both a server and client implementation.
```

### Comparing `python_matter_server-6.0.1/python_matter_server.egg-info/SOURCES.txt` & `python_matter_server-6.1.0b0/python_matter_server.egg-info/SOURCES.txt`

 * *Files 4% similar despite different names*

```diff
@@ -4,19 +4,19 @@
 matter_server/__init__.py
 matter_server/py.typed
 matter_server/client/__init__.py
 matter_server/client/client.py
 matter_server/client/connection.py
 matter_server/client/exceptions.py
 matter_server/client/models/__init__.py
-matter_server/client/models/clusters.py
 matter_server/client/models/device_types.py
 matter_server/client/models/node.py
 matter_server/common/__init__.py
 matter_server/common/const.py
+matter_server/common/custom_clusters.py
 matter_server/common/errors.py
 matter_server/common/models.py
 matter_server/common/helpers/api.py
 matter_server/common/helpers/json.py
 matter_server/common/helpers/util.py
 matter_server/dashboard/index.html
 matter_server/dashboard/js/dialog-box-ztARVrB9.js
```

