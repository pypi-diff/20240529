# Comparing `tmp/firex_flame-2.6.85.tar.gz` & `tmp/firex_flame-2.6.86.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "firex_flame-2.6.85.tar", last modified: Wed May 22 14:54:05 2024, max compression
+gzip compressed data, was "firex_flame-2.6.86.tar", last modified: Wed May 29 11:11:32 2024, max compression
```

## Comparing `firex_flame-2.6.85.tar` & `firex_flame-2.6.86.tar`

### file list

```diff
@@ -1,33 +1,33 @@
-drwxr-xr-x   0 firex      (101) nogroup  (65533)        0 2024-05-22 14:54:05.717453 firex_flame-2.6.85/
--rw-rw-rw-   0 firex      (101) nogroup  (65533)     1505 2024-05-22 14:53:50.000000 firex_flame-2.6.85/LICENSE
--rw-rw-rw-   0 firex      (101) nogroup  (65533)      103 2024-05-22 14:53:50.000000 firex_flame-2.6.85/MANIFEST.in
--rw-r--r--   0 firex      (101) nogroup  (65533)      785 2024-05-22 14:54:05.717453 firex_flame-2.6.85/PKG-INFO
--rw-rw-rw-   0 firex      (101) nogroup  (65533)     1642 2024-05-22 14:53:50.000000 firex_flame-2.6.85/README.md
--rw-rw-rw-   0 firex      (101) nogroup  (65533)     4042 2024-05-22 14:53:50.000000 firex_flame-2.6.85/fastentrypoints.py
-drwxr-xr-x   0 firex      (101) nogroup  (65533)        0 2024-05-22 14:54:05.718453 firex_flame-2.6.85/firex_flame/
--rw-rw-rw-   0 firex      (101) nogroup  (65533)       92 2024-05-22 14:53:50.000000 firex_flame-2.6.85/firex_flame/__init__.py
--rw-rw-rw-   0 firex      (101) nogroup  (65533)     8928 2024-05-22 14:53:50.000000 firex_flame-2.6.85/firex_flame/__main__.py
--rw-r--r--   0 firex      (101) nogroup  (65533)      498 2024-05-22 14:54:05.718453 firex_flame-2.6.85/firex_flame/_version.py
--rw-rw-rw-   0 firex      (101) nogroup  (65533)    15544 2024-05-22 14:53:50.000000 firex_flame-2.6.85/firex_flame/api.py
--rw-rw-rw-   0 firex      (101) nogroup  (65533)    18364 2024-05-22 14:53:50.000000 firex_flame-2.6.85/firex_flame/controller.py
--rw-rw-rw-   0 firex      (101) nogroup  (65533)     7418 2024-05-22 14:53:50.000000 firex_flame-2.6.85/firex_flame/event_broker_processor.py
--rw-rw-rw-   0 firex      (101) nogroup  (65533)     3440 2024-05-22 14:53:50.000000 firex_flame-2.6.85/firex_flame/event_file_processor.py
--rw-rw-rw-   0 firex      (101) nogroup  (65533)     6365 2024-05-22 14:53:50.000000 firex_flame-2.6.85/firex_flame/flame_helper.py
--rw-rw-rw-   0 firex      (101) nogroup  (65533)    43510 2024-05-22 14:53:50.000000 firex_flame-2.6.85/firex_flame/flame_task_graph.py
--rw-rw-rw-   0 firex      (101) nogroup  (65533)     9330 2024-05-22 14:53:50.000000 firex_flame-2.6.85/firex_flame/launcher.py
--rw-rw-rw-   0 firex      (101) nogroup  (65533)     2866 2024-05-22 14:53:50.000000 firex_flame-2.6.85/firex_flame/main_app.py
--rw-rw-rw-   0 firex      (101) nogroup  (65533)     6008 2024-05-22 14:53:50.000000 firex_flame-2.6.85/firex_flame/model_dumper.py
-drwxr-xr-x   0 firex      (101) nogroup  (65533)        0 2024-05-22 14:54:05.717453 firex_flame-2.6.85/firex_flame/templates/
--rw-rw-rw-   0 firex      (101) nogroup  (65533)     2530 2024-05-22 14:53:50.000000 firex_flame-2.6.85/firex_flame/templates/index.html
--rw-rw-rw-   0 firex      (101) nogroup  (65533)     8171 2024-05-22 14:53:50.000000 firex_flame-2.6.85/firex_flame/web_app.py
-drwxr-xr-x   0 firex      (101) nogroup  (65533)        0 2024-05-22 14:54:05.717453 firex_flame-2.6.85/firex_flame.egg-info/
--rw-r--r--   0 firex      (101) nogroup  (65533)      785 2024-05-22 14:54:05.000000 firex_flame-2.6.85/firex_flame.egg-info/PKG-INFO
--rw-r--r--   0 firex      (101) nogroup  (65533)      706 2024-05-22 14:54:05.000000 firex_flame-2.6.85/firex_flame.egg-info/SOURCES.txt
--rw-r--r--   0 firex      (101) nogroup  (65533)        1 2024-05-22 14:54:05.000000 firex_flame-2.6.85/firex_flame.egg-info/dependency_links.txt
--rw-r--r--   0 firex      (101) nogroup  (65533)      136 2024-05-22 14:54:05.000000 firex_flame-2.6.85/firex_flame.egg-info/entry_points.txt
--rw-r--r--   0 firex      (101) nogroup  (65533)      257 2024-05-22 14:54:05.000000 firex_flame-2.6.85/firex_flame.egg-info/requires.txt
--rw-r--r--   0 firex      (101) nogroup  (65533)       12 2024-05-22 14:54:05.000000 firex_flame-2.6.85/firex_flame.egg-info/top_level.txt
--rw-r--r--   0 firex      (101) nogroup  (65533)        1 2024-05-22 14:54:05.000000 firex_flame-2.6.85/firex_flame.egg-info/zip-safe
--rw-rw-rw-   0 firex      (101) nogroup  (65533)      277 2024-05-22 14:54:05.718453 firex_flame-2.6.85/setup.cfg
--rw-rw-rw-   0 firex      (101) nogroup  (65533)     1928 2024-05-22 14:53:50.000000 firex_flame-2.6.85/setup.py
--rw-rw-rw-   0 firex      (101) nogroup  (65533)    70144 2024-05-22 14:53:50.000000 firex_flame-2.6.85/versioneer.py
+drwxr-xr-x   0 firex      (101) nogroup  (65533)        0 2024-05-29 11:11:32.330772 firex_flame-2.6.86/
+-rw-rw-rw-   0 firex      (101) nogroup  (65533)     1505 2024-05-29 11:11:16.000000 firex_flame-2.6.86/LICENSE
+-rw-rw-rw-   0 firex      (101) nogroup  (65533)      103 2024-05-29 11:11:16.000000 firex_flame-2.6.86/MANIFEST.in
+-rw-r--r--   0 firex      (101) nogroup  (65533)      625 2024-05-29 11:11:32.330772 firex_flame-2.6.86/PKG-INFO
+-rw-rw-rw-   0 firex      (101) nogroup  (65533)     1642 2024-05-29 11:11:16.000000 firex_flame-2.6.86/README.md
+-rw-rw-rw-   0 firex      (101) nogroup  (65533)     4042 2024-05-29 11:11:16.000000 firex_flame-2.6.86/fastentrypoints.py
+drwxr-xr-x   0 firex      (101) nogroup  (65533)        0 2024-05-29 11:11:32.331772 firex_flame-2.6.86/firex_flame/
+-rw-rw-rw-   0 firex      (101) nogroup  (65533)       92 2024-05-29 11:11:16.000000 firex_flame-2.6.86/firex_flame/__init__.py
+-rw-rw-rw-   0 firex      (101) nogroup  (65533)     8928 2024-05-29 11:11:16.000000 firex_flame-2.6.86/firex_flame/__main__.py
+-rw-r--r--   0 firex      (101) nogroup  (65533)      498 2024-05-29 11:11:32.331772 firex_flame-2.6.86/firex_flame/_version.py
+-rw-rw-rw-   0 firex      (101) nogroup  (65533)    15568 2024-05-29 11:11:16.000000 firex_flame-2.6.86/firex_flame/api.py
+-rw-rw-rw-   0 firex      (101) nogroup  (65533)    18364 2024-05-29 11:11:16.000000 firex_flame-2.6.86/firex_flame/controller.py
+-rw-rw-rw-   0 firex      (101) nogroup  (65533)     7418 2024-05-29 11:11:16.000000 firex_flame-2.6.86/firex_flame/event_broker_processor.py
+-rw-rw-rw-   0 firex      (101) nogroup  (65533)     3440 2024-05-29 11:11:16.000000 firex_flame-2.6.86/firex_flame/event_file_processor.py
+-rw-rw-rw-   0 firex      (101) nogroup  (65533)     6365 2024-05-29 11:11:16.000000 firex_flame-2.6.86/firex_flame/flame_helper.py
+-rw-rw-rw-   0 firex      (101) nogroup  (65533)    43510 2024-05-29 11:11:16.000000 firex_flame-2.6.86/firex_flame/flame_task_graph.py
+-rw-rw-rw-   0 firex      (101) nogroup  (65533)     9330 2024-05-29 11:11:16.000000 firex_flame-2.6.86/firex_flame/launcher.py
+-rw-rw-rw-   0 firex      (101) nogroup  (65533)     2866 2024-05-29 11:11:16.000000 firex_flame-2.6.86/firex_flame/main_app.py
+-rw-rw-rw-   0 firex      (101) nogroup  (65533)     6008 2024-05-29 11:11:16.000000 firex_flame-2.6.86/firex_flame/model_dumper.py
+drwxr-xr-x   0 firex      (101) nogroup  (65533)        0 2024-05-29 11:11:32.330772 firex_flame-2.6.86/firex_flame/templates/
+-rw-rw-rw-   0 firex      (101) nogroup  (65533)     2530 2024-05-29 11:11:16.000000 firex_flame-2.6.86/firex_flame/templates/index.html
+-rw-rw-rw-   0 firex      (101) nogroup  (65533)     8171 2024-05-29 11:11:16.000000 firex_flame-2.6.86/firex_flame/web_app.py
+drwxr-xr-x   0 firex      (101) nogroup  (65533)        0 2024-05-29 11:11:32.330772 firex_flame-2.6.86/firex_flame.egg-info/
+-rw-r--r--   0 firex      (101) nogroup  (65533)      625 2024-05-29 11:11:32.000000 firex_flame-2.6.86/firex_flame.egg-info/PKG-INFO
+-rw-r--r--   0 firex      (101) nogroup  (65533)      706 2024-05-29 11:11:32.000000 firex_flame-2.6.86/firex_flame.egg-info/SOURCES.txt
+-rw-r--r--   0 firex      (101) nogroup  (65533)        1 2024-05-29 11:11:32.000000 firex_flame-2.6.86/firex_flame.egg-info/dependency_links.txt
+-rw-r--r--   0 firex      (101) nogroup  (65533)      136 2024-05-29 11:11:32.000000 firex_flame-2.6.86/firex_flame.egg-info/entry_points.txt
+-rw-r--r--   0 firex      (101) nogroup  (65533)      172 2024-05-29 11:11:32.000000 firex_flame-2.6.86/firex_flame.egg-info/requires.txt
+-rw-r--r--   0 firex      (101) nogroup  (65533)       12 2024-05-29 11:11:32.000000 firex_flame-2.6.86/firex_flame.egg-info/top_level.txt
+-rw-r--r--   0 firex      (101) nogroup  (65533)        1 2024-05-29 11:11:32.000000 firex_flame-2.6.86/firex_flame.egg-info/zip-safe
+-rw-rw-rw-   0 firex      (101) nogroup  (65533)      277 2024-05-29 11:11:32.331772 firex_flame-2.6.86/setup.cfg
+-rw-rw-rw-   0 firex      (101) nogroup  (65533)     1675 2024-05-29 11:11:16.000000 firex_flame-2.6.86/setup.py
+-rw-rw-rw-   0 firex      (101) nogroup  (65533)    70144 2024-05-29 11:11:16.000000 firex_flame-2.6.86/versioneer.py
```

### Comparing `firex_flame-2.6.85/LICENSE` & `firex_flame-2.6.86/LICENSE`

 * *Files identical despite different names*

### Comparing `firex_flame-2.6.85/PKG-INFO` & `firex_flame-2.6.86/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: firex_flame
-Version: 2.6.85
+Version: 2.6.86
 Summary: FireX event processor and web server.
 Home-page: https://github.com/FireXStuff/firex-flame
 Author: Core FireX Team
 Author-email: firex-dev@gmail.com
 License: BSD-3-Clause
 License-File: LICENSE
 Requires-Dist: Flask
@@ -16,12 +16,7 @@
 Requires-Dist: requests
 Requires-Dist: beautifulsoup4
 Requires-Dist: paramiko
 Requires-Dist: gevent-websocket
 Requires-Dist: gevent
 Requires-Dist: importlib-resources
 Requires-Dist: jsonpath-ng
-Requires-Dist: zope.interface==6.3
-Requires-Dist: zipp==3.18.1
-Requires-Dist: bcrypt==4.1.2
-Requires-Dist: cryptography==42.0.5
-Requires-Dist: rapidfuzz==3.8.1
```

### Comparing `firex_flame-2.6.85/README.md` & `firex_flame-2.6.86/README.md`

 * *Files identical despite different names*

### Comparing `firex_flame-2.6.85/fastentrypoints.py` & `firex_flame-2.6.86/fastentrypoints.py`

 * *Files identical despite different names*

### Comparing `firex_flame-2.6.85/firex_flame/__main__.py` & `firex_flame-2.6.86/firex_flame/__main__.py`

 * *Files identical despite different names*

### Comparing `firex_flame-2.6.85/firex_flame/api.py` & `firex_flame-2.6.86/firex_flame/api.py`

 * *Files 1% similar despite different names*

```diff
@@ -364,15 +364,15 @@
     @web_app.route('/api/revoke', methods=['GET', 'POST'])
     def rest_revoke_root_task():
         # a revoke run quickly after submission
         # might be received before the root task is known,
         # so wait a brief amount of time.
         root_uuid = wait_until(
             lambda: controller.graph.root_uuid,
-            timeout=5,
+            timeout=20, # startup can be slow.
             sleep_for=0.1,
         )
         logger.debug(f'Revoking entire run via root task UUID: {root_uuid}')
         if not root_uuid:
             return '', 500
         return _rest_revoke_task(root_uuid)
```

### Comparing `firex_flame-2.6.85/firex_flame/controller.py` & `firex_flame-2.6.86/firex_flame/controller.py`

 * *Files identical despite different names*

### Comparing `firex_flame-2.6.85/firex_flame/event_broker_processor.py` & `firex_flame-2.6.86/firex_flame/event_broker_processor.py`

 * *Files identical despite different names*

### Comparing `firex_flame-2.6.85/firex_flame/event_file_processor.py` & `firex_flame-2.6.86/firex_flame/event_file_processor.py`

 * *Files identical despite different names*

### Comparing `firex_flame-2.6.85/firex_flame/flame_helper.py` & `firex_flame-2.6.86/firex_flame/flame_helper.py`

 * *Files identical despite different names*

### Comparing `firex_flame-2.6.85/firex_flame/flame_task_graph.py` & `firex_flame-2.6.86/firex_flame/flame_task_graph.py`

 * *Files identical despite different names*

### Comparing `firex_flame-2.6.85/firex_flame/launcher.py` & `firex_flame-2.6.86/firex_flame/launcher.py`

 * *Files identical despite different names*

### Comparing `firex_flame-2.6.85/firex_flame/main_app.py` & `firex_flame-2.6.86/firex_flame/main_app.py`

 * *Files identical despite different names*

### Comparing `firex_flame-2.6.85/firex_flame/model_dumper.py` & `firex_flame-2.6.86/firex_flame/model_dumper.py`

 * *Files identical despite different names*

### Comparing `firex_flame-2.6.85/firex_flame/templates/index.html` & `firex_flame-2.6.86/firex_flame/templates/index.html`

 * *Files identical despite different names*

### Comparing `firex_flame-2.6.85/firex_flame/web_app.py` & `firex_flame-2.6.86/firex_flame/web_app.py`

 * *Files identical despite different names*

### Comparing `firex_flame-2.6.85/firex_flame.egg-info/PKG-INFO` & `firex_flame-2.6.86/firex_flame.egg-info/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: firex_flame
-Version: 2.6.85
+Version: 2.6.86
 Summary: FireX event processor and web server.
 Home-page: https://github.com/FireXStuff/firex-flame
 Author: Core FireX Team
 Author-email: firex-dev@gmail.com
 License: BSD-3-Clause
 License-File: LICENSE
 Requires-Dist: Flask
@@ -16,12 +16,7 @@
 Requires-Dist: requests
 Requires-Dist: beautifulsoup4
 Requires-Dist: paramiko
 Requires-Dist: gevent-websocket
 Requires-Dist: gevent
 Requires-Dist: importlib-resources
 Requires-Dist: jsonpath-ng
-Requires-Dist: zope.interface==6.3
-Requires-Dist: zipp==3.18.1
-Requires-Dist: bcrypt==4.1.2
-Requires-Dist: cryptography==42.0.5
-Requires-Dist: rapidfuzz==3.8.1
```

### Comparing `firex_flame-2.6.85/firex_flame.egg-info/SOURCES.txt` & `firex_flame-2.6.86/firex_flame.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `firex_flame-2.6.85/setup.py` & `firex_flame-2.6.86/setup.py`

 * *Files 10% similar despite different names*

```diff
@@ -30,23 +30,14 @@
             "requests",
             "beautifulsoup4",
             "paramiko",
             "gevent-websocket",
             "gevent",
             "importlib-resources",
             "jsonpath-ng",
-
-            # pin to debug seg fail in Open Source CI.
-            # "setuptools==69.5.1",
-
-            "zope.interface==6.3",
-            "zipp==3.18.1",
-            "bcrypt==4.1.2",
-            "cryptography==42.0.5",
-            "rapidfuzz==3.8.1",
       ],
       package_data={
         'firex_flame': ['templates/*.html'],
       },
       entry_points={
           'console_scripts': ['firex_flame = firex_flame.__main__:main'],
           'firex_tracking_service': ['flame_launcher = firex_flame.launcher:FlameLauncher', ],
```

### Comparing `firex_flame-2.6.85/versioneer.py` & `firex_flame-2.6.86/versioneer.py`

 * *Files identical despite different names*

