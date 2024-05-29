# Comparing `tmp/ralium-2.0.3.tar.gz` & `tmp/ralium-2.0.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ralium-2.0.3.tar", last modified: Tue May 28 05:33:51 2024, max compression
+gzip compressed data, was "ralium-2.0.4.tar", last modified: Tue May 28 05:38:10 2024, max compression
```

## Comparing `ralium-2.0.3.tar` & `ralium-2.0.4.tar`

### file list

```diff
@@ -1,41 +1,41 @@
-drwxrwxrwx   0        0        0        0 2024-05-28 05:33:51.976877 ralium-2.0.3/
--rw-rw-rw-   0        0        0    35823 2024-05-21 00:22:26.000000 ralium-2.0.3/LICENSE
--rw-rw-rw-   0        0        0    41897 2024-05-28 05:33:51.975516 ralium-2.0.3/PKG-INFO
--rw-rw-rw-   0        0        0       52 2024-05-21 00:22:26.000000 ralium-2.0.3/README.md
--rw-rw-rw-   0        0        0      970 2024-05-28 05:33:22.000000 ralium-2.0.3/pyproject.toml
-drwxrwxrwx   0        0        0        0 2024-05-28 05:33:51.955440 ralium-2.0.3/ralium/
--rw-rw-rw-   0        0        0      357 2024-05-21 05:00:06.000000 ralium-2.0.3/ralium/__init__.py
--rw-rw-rw-   0        0        0     1902 2024-05-28 05:33:27.000000 ralium-2.0.3/ralium/_util.py
--rw-rw-rw-   0        0        0     1098 2024-05-27 18:21:08.000000 ralium-2.0.3/ralium/_util.pyi
--rw-rw-rw-   0        0        0     7555 2024-05-21 04:21:31.000000 ralium-2.0.3/ralium/api.py
--rw-rw-rw-   0        0        0     1066 2024-05-21 00:25:27.000000 ralium-2.0.3/ralium/api.pyi
--rw-rw-rw-   0        0        0      680 2024-05-21 00:25:27.000000 ralium-2.0.3/ralium/builtins.py
--rw-rw-rw-   0        0        0      541 2024-05-21 00:25:27.000000 ralium-2.0.3/ralium/builtins.pyi
--rw-rw-rw-   0        0        0     8231 2024-05-21 06:11:47.000000 ralium-2.0.3/ralium/bundle.py
--rw-rw-rw-   0        0        0     1581 2024-05-21 00:26:03.000000 ralium-2.0.3/ralium/bundle.pyi
--rw-rw-rw-   0        0        0     3332 2024-05-21 00:25:27.000000 ralium-2.0.3/ralium/config.py
--rw-rw-rw-   0        0        0      467 2024-05-21 00:25:27.000000 ralium-2.0.3/ralium/config.pyi
--rw-rw-rw-   0        0        0     6425 2024-05-21 00:25:27.000000 ralium-2.0.3/ralium/element.py
--rw-rw-rw-   0        0        0     1376 2024-05-21 00:26:03.000000 ralium-2.0.3/ralium/element.pyi
--rw-rw-rw-   0        0        0     4402 2024-05-21 00:26:03.000000 ralium-2.0.3/ralium/engine.py
--rw-rw-rw-   0        0        0     1389 2024-05-21 00:25:27.000000 ralium-2.0.3/ralium/engine.pyi
--rw-rw-rw-   0        0        0     1147 2024-05-27 18:22:26.000000 ralium-2.0.3/ralium/errors.py
--rw-rw-rw-   0        0        0     2387 2024-05-21 00:25:27.000000 ralium-2.0.3/ralium/listener.py
--rw-rw-rw-   0        0        0      890 2024-05-21 00:25:27.000000 ralium-2.0.3/ralium/listener.pyi
--rw-rw-rw-   0        0        0      804 2024-05-21 00:25:27.000000 ralium-2.0.3/ralium/navigation.py
--rw-rw-rw-   0        0        0      376 2024-05-21 00:25:27.000000 ralium-2.0.3/ralium/navigation.pyi
--rw-rw-rw-   0        0        0     4805 2024-05-21 15:38:14.000000 ralium-2.0.3/ralium/pyhtml.py
--rw-rw-rw-   0        0        0      531 2024-05-21 07:20:26.000000 ralium-2.0.3/ralium/pyhtml.pyi
--rw-rw-rw-   0        0        0     7851 2024-05-21 05:23:35.000000 ralium-2.0.3/ralium/setuptools.py
--rw-rw-rw-   0        0        0      965 2024-05-21 05:19:13.000000 ralium-2.0.3/ralium/setuptools.pyi
--rw-rw-rw-   0        0        0     6452 2024-05-27 18:22:15.000000 ralium-2.0.3/ralium/webpage.py
--rw-rw-rw-   0        0        0     1870 2024-05-21 00:26:03.000000 ralium-2.0.3/ralium/webpage.pyi
--rw-rw-rw-   0        0        0     6078 2024-05-27 18:21:30.000000 ralium-2.0.3/ralium/window.py
--rw-rw-rw-   0        0        0      693 2024-05-21 00:25:27.000000 ralium-2.0.3/ralium/window.pyi
-drwxrwxrwx   0        0        0        0 2024-05-28 05:33:51.974508 ralium-2.0.3/ralium.egg-info/
--rw-rw-rw-   0        0        0    41897 2024-05-28 05:33:51.000000 ralium-2.0.3/ralium.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      692 2024-05-28 05:33:51.000000 ralium-2.0.3/ralium.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-05-28 05:33:51.000000 ralium-2.0.3/ralium.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       42 2024-05-28 05:33:51.000000 ralium-2.0.3/ralium.egg-info/requires.txt
--rw-rw-rw-   0        0        0        7 2024-05-28 05:33:51.000000 ralium-2.0.3/ralium.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2024-05-28 05:33:51.976877 ralium-2.0.3/setup.cfg
+drwxrwxrwx   0        0        0        0 2024-05-28 05:38:10.041849 ralium-2.0.4/
+-rw-rw-rw-   0        0        0    35823 2024-05-21 00:22:26.000000 ralium-2.0.4/LICENSE
+-rw-rw-rw-   0        0        0    41897 2024-05-28 05:38:10.041849 ralium-2.0.4/PKG-INFO
+-rw-rw-rw-   0        0        0       52 2024-05-21 00:22:26.000000 ralium-2.0.4/README.md
+-rw-rw-rw-   0        0        0      970 2024-05-28 05:37:44.000000 ralium-2.0.4/pyproject.toml
+drwxrwxrwx   0        0        0        0 2024-05-28 05:38:10.020226 ralium-2.0.4/ralium/
+-rw-rw-rw-   0        0        0      357 2024-05-21 05:00:06.000000 ralium-2.0.4/ralium/__init__.py
+-rw-rw-rw-   0        0        0     1895 2024-05-28 05:37:50.000000 ralium-2.0.4/ralium/_util.py
+-rw-rw-rw-   0        0        0     1098 2024-05-27 18:21:08.000000 ralium-2.0.4/ralium/_util.pyi
+-rw-rw-rw-   0        0        0     7555 2024-05-21 04:21:31.000000 ralium-2.0.4/ralium/api.py
+-rw-rw-rw-   0        0        0     1066 2024-05-21 00:25:27.000000 ralium-2.0.4/ralium/api.pyi
+-rw-rw-rw-   0        0        0      680 2024-05-21 00:25:27.000000 ralium-2.0.4/ralium/builtins.py
+-rw-rw-rw-   0        0        0      541 2024-05-21 00:25:27.000000 ralium-2.0.4/ralium/builtins.pyi
+-rw-rw-rw-   0        0        0     8231 2024-05-21 06:11:47.000000 ralium-2.0.4/ralium/bundle.py
+-rw-rw-rw-   0        0        0     1581 2024-05-21 00:26:03.000000 ralium-2.0.4/ralium/bundle.pyi
+-rw-rw-rw-   0        0        0     3332 2024-05-21 00:25:27.000000 ralium-2.0.4/ralium/config.py
+-rw-rw-rw-   0        0        0      467 2024-05-21 00:25:27.000000 ralium-2.0.4/ralium/config.pyi
+-rw-rw-rw-   0        0        0     6425 2024-05-21 00:25:27.000000 ralium-2.0.4/ralium/element.py
+-rw-rw-rw-   0        0        0     1376 2024-05-21 00:26:03.000000 ralium-2.0.4/ralium/element.pyi
+-rw-rw-rw-   0        0        0     4402 2024-05-21 00:26:03.000000 ralium-2.0.4/ralium/engine.py
+-rw-rw-rw-   0        0        0     1389 2024-05-21 00:25:27.000000 ralium-2.0.4/ralium/engine.pyi
+-rw-rw-rw-   0        0        0     1147 2024-05-27 18:22:26.000000 ralium-2.0.4/ralium/errors.py
+-rw-rw-rw-   0        0        0     2387 2024-05-21 00:25:27.000000 ralium-2.0.4/ralium/listener.py
+-rw-rw-rw-   0        0        0      890 2024-05-21 00:25:27.000000 ralium-2.0.4/ralium/listener.pyi
+-rw-rw-rw-   0        0        0      804 2024-05-21 00:25:27.000000 ralium-2.0.4/ralium/navigation.py
+-rw-rw-rw-   0        0        0      376 2024-05-21 00:25:27.000000 ralium-2.0.4/ralium/navigation.pyi
+-rw-rw-rw-   0        0        0     4805 2024-05-21 15:38:14.000000 ralium-2.0.4/ralium/pyhtml.py
+-rw-rw-rw-   0        0        0      531 2024-05-21 07:20:26.000000 ralium-2.0.4/ralium/pyhtml.pyi
+-rw-rw-rw-   0        0        0     7851 2024-05-21 05:23:35.000000 ralium-2.0.4/ralium/setuptools.py
+-rw-rw-rw-   0        0        0      965 2024-05-21 05:19:13.000000 ralium-2.0.4/ralium/setuptools.pyi
+-rw-rw-rw-   0        0        0     6452 2024-05-27 18:22:15.000000 ralium-2.0.4/ralium/webpage.py
+-rw-rw-rw-   0        0        0     1870 2024-05-21 00:26:03.000000 ralium-2.0.4/ralium/webpage.pyi
+-rw-rw-rw-   0        0        0     6078 2024-05-27 18:21:30.000000 ralium-2.0.4/ralium/window.py
+-rw-rw-rw-   0        0        0      693 2024-05-21 00:25:27.000000 ralium-2.0.4/ralium/window.pyi
+drwxrwxrwx   0        0        0        0 2024-05-28 05:38:10.040516 ralium-2.0.4/ralium.egg-info/
+-rw-rw-rw-   0        0        0    41897 2024-05-28 05:38:09.000000 ralium-2.0.4/ralium.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      692 2024-05-28 05:38:09.000000 ralium-2.0.4/ralium.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-05-28 05:38:09.000000 ralium-2.0.4/ralium.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       42 2024-05-28 05:38:09.000000 ralium-2.0.4/ralium.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        7 2024-05-28 05:38:09.000000 ralium-2.0.4/ralium.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2024-05-28 05:38:10.043162 ralium-2.0.4/setup.cfg
```

### Comparing `ralium-2.0.3/LICENSE` & `ralium-2.0.4/LICENSE`

 * *Files identical despite different names*

### Comparing `ralium-2.0.3/PKG-INFO` & `ralium-2.0.4/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ralium
-Version: 2.0.3
+Version: 2.0.4
 Summary: An easy to use wrapper for pywebview.
 Author-email: Isaiah Coroama <coroamaisaiah@gmail.com>
 License:                     GNU GENERAL PUBLIC LICENSE
                                Version 3, 29 June 2007
         
          Copyright (C) 2007 Free Software Foundation, Inc. <https://fsf.org/>
          Everyone is permitted to copy and distribute verbatim copies
```

### Comparing `ralium-2.0.3/pyproject.toml` & `ralium-2.0.4/pyproject.toml`

 * *Files 8% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires      = ["setuptools >= 69.5.0", "wheel >= 0.43.0"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "ralium"
-version = "2.0.3"
+version = "2.0.4"
 description = "An easy to use wrapper for pywebview."
 readme = "README.md"
 authors = [{ name = "Isaiah Coroama", email = "coroamaisaiah@gmail.com" }]
 license = { file = "LICENSE" }
 classifiers = [
     'Development Status :: 3 - Alpha',
     'Intended Audience :: Developers',
```

### Comparing `ralium-2.0.3/ralium/_util.py` & `ralium-2.0.4/ralium/_util.py`

 * *Files 1% similar despite different names*

```diff
@@ -3,15 +3,15 @@
 import os
 
 __all__ = [
     "__version__", "BasicHTTPServer", "NamedDict", "_get_http_server_handler", "_get_bundle", 
     "_norm_url", "_check_exists",  "_check_is_dir", "_read_file", "_get_path"
 ]
 
-__version__ = "2.0.3"
+__version__ = "2.0.4"
 
 SYS_BUNDLE_ATTRIBUTE = "bundled"
 
 class BasicHTTPServer(http.server.SimpleHTTPRequestHandler):
     pass
 
 class NamedDict(dict):
@@ -63,13 +63,13 @@
     with open(path, "r", encoding=encoding) as f:
         return f.read()
 
 def _get_path(path):
     bundle = _get_bundle()
 
     if bundle is not None:
-        return os.path.normpath(path)
+        return _norm_url(path)
 
     if getattr(sys, "frozen", False):
         return os.path.abspath(os.path.join(sys._MEIPASS, path))
 
     return os.path.abspath(path)
```

### Comparing `ralium-2.0.3/ralium/_util.pyi` & `ralium-2.0.4/ralium/_util.pyi`

 * *Files identical despite different names*

### Comparing `ralium-2.0.3/ralium/api.py` & `ralium-2.0.4/ralium/api.py`

 * *Files identical despite different names*

### Comparing `ralium-2.0.3/ralium/api.pyi` & `ralium-2.0.4/ralium/api.pyi`

 * *Files identical despite different names*

### Comparing `ralium-2.0.3/ralium/builtins.py` & `ralium-2.0.4/ralium/builtins.py`

 * *Files identical despite different names*

### Comparing `ralium-2.0.3/ralium/builtins.pyi` & `ralium-2.0.4/ralium/builtins.pyi`

 * *Files identical despite different names*

### Comparing `ralium-2.0.3/ralium/bundle.py` & `ralium-2.0.4/ralium/bundle.py`

 * *Files identical despite different names*

### Comparing `ralium-2.0.3/ralium/bundle.pyi` & `ralium-2.0.4/ralium/bundle.pyi`

 * *Files identical despite different names*

### Comparing `ralium-2.0.3/ralium/config.py` & `ralium-2.0.4/ralium/config.py`

 * *Files identical despite different names*

### Comparing `ralium-2.0.3/ralium/element.py` & `ralium-2.0.4/ralium/element.py`

 * *Files identical despite different names*

### Comparing `ralium-2.0.3/ralium/element.pyi` & `ralium-2.0.4/ralium/element.pyi`

 * *Files identical despite different names*

### Comparing `ralium-2.0.3/ralium/engine.py` & `ralium-2.0.4/ralium/engine.py`

 * *Files identical despite different names*

### Comparing `ralium-2.0.3/ralium/engine.pyi` & `ralium-2.0.4/ralium/engine.pyi`

 * *Files identical despite different names*

### Comparing `ralium-2.0.3/ralium/errors.py` & `ralium-2.0.4/ralium/errors.py`

 * *Files identical despite different names*

### Comparing `ralium-2.0.3/ralium/listener.py` & `ralium-2.0.4/ralium/listener.py`

 * *Files identical despite different names*

### Comparing `ralium-2.0.3/ralium/listener.pyi` & `ralium-2.0.4/ralium/listener.pyi`

 * *Files identical despite different names*

### Comparing `ralium-2.0.3/ralium/navigation.py` & `ralium-2.0.4/ralium/navigation.py`

 * *Files identical despite different names*

### Comparing `ralium-2.0.3/ralium/pyhtml.py` & `ralium-2.0.4/ralium/pyhtml.py`

 * *Files identical despite different names*

### Comparing `ralium-2.0.3/ralium/pyhtml.pyi` & `ralium-2.0.4/ralium/pyhtml.pyi`

 * *Files identical despite different names*

### Comparing `ralium-2.0.3/ralium/setuptools.py` & `ralium-2.0.4/ralium/setuptools.py`

 * *Files identical despite different names*

### Comparing `ralium-2.0.3/ralium/setuptools.pyi` & `ralium-2.0.4/ralium/setuptools.pyi`

 * *Files identical despite different names*

### Comparing `ralium-2.0.3/ralium/webpage.py` & `ralium-2.0.4/ralium/webpage.py`

 * *Files identical despite different names*

### Comparing `ralium-2.0.3/ralium/webpage.pyi` & `ralium-2.0.4/ralium/webpage.pyi`

 * *Files identical despite different names*

### Comparing `ralium-2.0.3/ralium/window.py` & `ralium-2.0.4/ralium/window.py`

 * *Files identical despite different names*

### Comparing `ralium-2.0.3/ralium/window.pyi` & `ralium-2.0.4/ralium/window.pyi`

 * *Files identical despite different names*

### Comparing `ralium-2.0.3/ralium.egg-info/PKG-INFO` & `ralium-2.0.4/ralium.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ralium
-Version: 2.0.3
+Version: 2.0.4
 Summary: An easy to use wrapper for pywebview.
 Author-email: Isaiah Coroama <coroamaisaiah@gmail.com>
 License:                     GNU GENERAL PUBLIC LICENSE
                                Version 3, 29 June 2007
         
          Copyright (C) 2007 Free Software Foundation, Inc. <https://fsf.org/>
          Everyone is permitted to copy and distribute verbatim copies
```

### Comparing `ralium-2.0.3/ralium.egg-info/SOURCES.txt` & `ralium-2.0.4/ralium.egg-info/SOURCES.txt`

 * *Files identical despite different names*

