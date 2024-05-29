# Comparing `tmp/ralium-2.1.0.tar.gz` & `tmp/ralium-2.1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ralium-2.1.0.tar", last modified: Wed May 29 00:46:53 2024, max compression
+gzip compressed data, was "ralium-2.1.1.tar", last modified: Wed May 29 00:59:03 2024, max compression
```

## Comparing `ralium-2.1.0.tar` & `ralium-2.1.1.tar`

### file list

```diff
@@ -1,41 +1,41 @@
-drwxrwxrwx   0        0        0        0 2024-05-29 00:46:53.117566 ralium-2.1.0/
--rw-rw-rw-   0        0        0    35823 2024-05-21 00:22:26.000000 ralium-2.1.0/LICENSE
--rw-rw-rw-   0        0        0    41897 2024-05-29 00:46:53.116276 ralium-2.1.0/PKG-INFO
--rw-rw-rw-   0        0        0       52 2024-05-21 00:22:26.000000 ralium-2.1.0/README.md
--rw-rw-rw-   0        0        0      970 2024-05-29 00:45:51.000000 ralium-2.1.0/pyproject.toml
-drwxrwxrwx   0        0        0        0 2024-05-29 00:46:53.091605 ralium-2.1.0/ralium/
--rw-rw-rw-   0        0        0      357 2024-05-21 05:00:06.000000 ralium-2.1.0/ralium/__init__.py
--rw-rw-rw-   0        0        0     2247 2024-05-29 00:45:57.000000 ralium-2.1.0/ralium/_util.py
--rw-rw-rw-   0        0        0     1192 2024-05-29 00:14:14.000000 ralium-2.1.0/ralium/_util.pyi
--rw-rw-rw-   0        0        0     7555 2024-05-29 00:26:49.000000 ralium-2.1.0/ralium/api.py
--rw-rw-rw-   0        0        0     1066 2024-05-21 00:25:27.000000 ralium-2.1.0/ralium/api.pyi
--rw-rw-rw-   0        0        0      680 2024-05-21 00:25:27.000000 ralium-2.1.0/ralium/builtins.py
--rw-rw-rw-   0        0        0      541 2024-05-21 00:25:27.000000 ralium-2.1.0/ralium/builtins.pyi
--rw-rw-rw-   0        0        0     9527 2024-05-29 00:38:25.000000 ralium-2.1.0/ralium/bundle.py
--rw-rw-rw-   0        0        0     1958 2024-05-29 00:37:29.000000 ralium-2.1.0/ralium/bundle.pyi
--rw-rw-rw-   0        0        0     3332 2024-05-21 00:25:27.000000 ralium-2.1.0/ralium/config.py
--rw-rw-rw-   0        0        0      467 2024-05-21 00:25:27.000000 ralium-2.1.0/ralium/config.pyi
--rw-rw-rw-   0        0        0     6425 2024-05-21 00:25:27.000000 ralium-2.1.0/ralium/element.py
--rw-rw-rw-   0        0        0     1376 2024-05-21 00:26:03.000000 ralium-2.1.0/ralium/element.pyi
--rw-rw-rw-   0        0        0     4402 2024-05-21 00:26:03.000000 ralium-2.1.0/ralium/engine.py
--rw-rw-rw-   0        0        0     1389 2024-05-21 00:25:27.000000 ralium-2.1.0/ralium/engine.pyi
--rw-rw-rw-   0        0        0     1147 2024-05-27 18:22:26.000000 ralium-2.1.0/ralium/errors.py
--rw-rw-rw-   0        0        0     2387 2024-05-21 00:25:27.000000 ralium-2.1.0/ralium/listener.py
--rw-rw-rw-   0        0        0      890 2024-05-21 00:25:27.000000 ralium-2.1.0/ralium/listener.pyi
--rw-rw-rw-   0        0        0      804 2024-05-21 00:25:27.000000 ralium-2.1.0/ralium/navigation.py
--rw-rw-rw-   0        0        0      376 2024-05-21 00:25:27.000000 ralium-2.1.0/ralium/navigation.pyi
--rw-rw-rw-   0        0        0     4847 2024-05-28 23:54:13.000000 ralium-2.1.0/ralium/pyhtml.py
--rw-rw-rw-   0        0        0      531 2024-05-21 07:20:26.000000 ralium-2.1.0/ralium/pyhtml.pyi
--rw-rw-rw-   0        0        0     7678 2024-05-28 23:49:25.000000 ralium-2.1.0/ralium/setuptools.py
--rw-rw-rw-   0        0        0      959 2024-05-28 23:49:19.000000 ralium-2.1.0/ralium/setuptools.pyi
--rw-rw-rw-   0        0        0     6471 2024-05-29 00:21:58.000000 ralium-2.1.0/ralium/webpage.py
--rw-rw-rw-   0        0        0     1870 2024-05-21 00:26:03.000000 ralium-2.1.0/ralium/webpage.pyi
--rw-rw-rw-   0        0        0     6078 2024-05-29 00:22:41.000000 ralium-2.1.0/ralium/window.py
--rw-rw-rw-   0        0        0      693 2024-05-21 00:25:27.000000 ralium-2.1.0/ralium/window.pyi
-drwxrwxrwx   0        0        0        0 2024-05-29 00:46:53.114766 ralium-2.1.0/ralium.egg-info/
--rw-rw-rw-   0        0        0    41897 2024-05-29 00:46:53.000000 ralium-2.1.0/ralium.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      692 2024-05-29 00:46:53.000000 ralium-2.1.0/ralium.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-05-29 00:46:53.000000 ralium-2.1.0/ralium.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       42 2024-05-29 00:46:53.000000 ralium-2.1.0/ralium.egg-info/requires.txt
--rw-rw-rw-   0        0        0        7 2024-05-29 00:46:53.000000 ralium-2.1.0/ralium.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2024-05-29 00:46:53.117566 ralium-2.1.0/setup.cfg
+drwxrwxrwx   0        0        0        0 2024-05-29 00:59:03.795092 ralium-2.1.1/
+-rw-rw-rw-   0        0        0    35823 2024-05-21 00:22:26.000000 ralium-2.1.1/LICENSE
+-rw-rw-rw-   0        0        0    41897 2024-05-29 00:59:03.793644 ralium-2.1.1/PKG-INFO
+-rw-rw-rw-   0        0        0       52 2024-05-21 00:22:26.000000 ralium-2.1.1/README.md
+-rw-rw-rw-   0        0        0      970 2024-05-29 00:58:37.000000 ralium-2.1.1/pyproject.toml
+drwxrwxrwx   0        0        0        0 2024-05-29 00:59:03.773062 ralium-2.1.1/ralium/
+-rw-rw-rw-   0        0        0      357 2024-05-21 05:00:06.000000 ralium-2.1.1/ralium/__init__.py
+-rw-rw-rw-   0        0        0     2317 2024-05-29 00:58:34.000000 ralium-2.1.1/ralium/_util.py
+-rw-rw-rw-   0        0        0     1192 2024-05-29 00:14:14.000000 ralium-2.1.1/ralium/_util.pyi
+-rw-rw-rw-   0        0        0     7555 2024-05-29 00:26:49.000000 ralium-2.1.1/ralium/api.py
+-rw-rw-rw-   0        0        0     1066 2024-05-21 00:25:27.000000 ralium-2.1.1/ralium/api.pyi
+-rw-rw-rw-   0        0        0      680 2024-05-21 00:25:27.000000 ralium-2.1.1/ralium/builtins.py
+-rw-rw-rw-   0        0        0      541 2024-05-21 00:25:27.000000 ralium-2.1.1/ralium/builtins.pyi
+-rw-rw-rw-   0        0        0     9527 2024-05-29 00:38:25.000000 ralium-2.1.1/ralium/bundle.py
+-rw-rw-rw-   0        0        0     1958 2024-05-29 00:37:29.000000 ralium-2.1.1/ralium/bundle.pyi
+-rw-rw-rw-   0        0        0     3332 2024-05-21 00:25:27.000000 ralium-2.1.1/ralium/config.py
+-rw-rw-rw-   0        0        0      467 2024-05-21 00:25:27.000000 ralium-2.1.1/ralium/config.pyi
+-rw-rw-rw-   0        0        0     6425 2024-05-21 00:25:27.000000 ralium-2.1.1/ralium/element.py
+-rw-rw-rw-   0        0        0     1376 2024-05-21 00:26:03.000000 ralium-2.1.1/ralium/element.pyi
+-rw-rw-rw-   0        0        0     4402 2024-05-21 00:26:03.000000 ralium-2.1.1/ralium/engine.py
+-rw-rw-rw-   0        0        0     1389 2024-05-21 00:25:27.000000 ralium-2.1.1/ralium/engine.pyi
+-rw-rw-rw-   0        0        0     1147 2024-05-27 18:22:26.000000 ralium-2.1.1/ralium/errors.py
+-rw-rw-rw-   0        0        0     2387 2024-05-21 00:25:27.000000 ralium-2.1.1/ralium/listener.py
+-rw-rw-rw-   0        0        0      890 2024-05-21 00:25:27.000000 ralium-2.1.1/ralium/listener.pyi
+-rw-rw-rw-   0        0        0      804 2024-05-21 00:25:27.000000 ralium-2.1.1/ralium/navigation.py
+-rw-rw-rw-   0        0        0      376 2024-05-21 00:25:27.000000 ralium-2.1.1/ralium/navigation.pyi
+-rw-rw-rw-   0        0        0     4847 2024-05-28 23:54:13.000000 ralium-2.1.1/ralium/pyhtml.py
+-rw-rw-rw-   0        0        0      531 2024-05-21 07:20:26.000000 ralium-2.1.1/ralium/pyhtml.pyi
+-rw-rw-rw-   0        0        0     7678 2024-05-28 23:49:25.000000 ralium-2.1.1/ralium/setuptools.py
+-rw-rw-rw-   0        0        0      959 2024-05-28 23:49:19.000000 ralium-2.1.1/ralium/setuptools.pyi
+-rw-rw-rw-   0        0        0     6471 2024-05-29 00:21:58.000000 ralium-2.1.1/ralium/webpage.py
+-rw-rw-rw-   0        0        0     1870 2024-05-21 00:26:03.000000 ralium-2.1.1/ralium/webpage.pyi
+-rw-rw-rw-   0        0        0     6078 2024-05-29 00:22:41.000000 ralium-2.1.1/ralium/window.py
+-rw-rw-rw-   0        0        0      693 2024-05-21 00:25:27.000000 ralium-2.1.1/ralium/window.pyi
+drwxrwxrwx   0        0        0        0 2024-05-29 00:59:03.792112 ralium-2.1.1/ralium.egg-info/
+-rw-rw-rw-   0        0        0    41897 2024-05-29 00:59:03.000000 ralium-2.1.1/ralium.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      692 2024-05-29 00:59:03.000000 ralium-2.1.1/ralium.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-05-29 00:59:03.000000 ralium-2.1.1/ralium.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       42 2024-05-29 00:59:03.000000 ralium-2.1.1/ralium.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        7 2024-05-29 00:59:03.000000 ralium-2.1.1/ralium.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2024-05-29 00:59:03.795596 ralium-2.1.1/setup.cfg
```

### Comparing `ralium-2.1.0/LICENSE` & `ralium-2.1.1/LICENSE`

 * *Files identical despite different names*

### Comparing `ralium-2.1.0/PKG-INFO` & `ralium-2.1.1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ralium
-Version: 2.1.0
+Version: 2.1.1
 Summary: An easy to use wrapper for pywebview.
 Author-email: Isaiah Coroama <coroamaisaiah@gmail.com>
 License:                     GNU GENERAL PUBLIC LICENSE
                                Version 3, 29 June 2007
         
          Copyright (C) 2007 Free Software Foundation, Inc. <https://fsf.org/>
          Everyone is permitted to copy and distribute verbatim copies
```

### Comparing `ralium-2.1.0/pyproject.toml` & `ralium-2.1.1/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires      = ["setuptools >= 69.5.0", "wheel >= 0.43.0"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "ralium"
-version = "2.1.0"
+version = "2.1.1"
 description = "An easy to use wrapper for pywebview."
 readme = "README.md"
 authors = [{ name = "Isaiah Coroama", email = "coroamaisaiah@gmail.com" }]
 license = { file = "LICENSE" }
 classifiers = [
     'Development Status :: 3 - Alpha',
     'Intended Audience :: Developers',
```

### Comparing `ralium-2.1.0/ralium/_util.py` & `ralium-2.1.1/ralium/_util.py`

 * *Files 3% similar despite different names*

```diff
@@ -4,15 +4,17 @@
 import os
 
 __all__ = [
     "__version__", "BasicHTTPServer", "NamedDict", "_get_http_server_handler", "_get_bundle", 
     "_norm_url", "_norm_path", "_check_exists",  "_check_is_dir", "_read_file", "_get_path"
 ]
 
-__version__ = "2.1.0"
+__version__ = "2.1.1"
+
+relpathsep = "\\" if sys.platform.startswith("win") else "/"
 
 SYS_BUNDLE_ATTRIBUTE = "bundled"
 
 class BasicHTTPServer(http.server.SimpleHTTPRequestHandler):
     pass
 
 class NamedDict(dict):
@@ -62,15 +64,15 @@
 
 def _norm_url(path):
     return os.path.normpath(f"\\{path.lstrip('/\\')}").replace("\\", "/")
 
 def _norm_path(path):
     if _is_abs_win(path):
         return path
-    return os.path.normpath(f"\\{path.lstrip('/\\')}").replace("/", "\\")
+    return os.path.normpath(f"\\{path.lstrip('/\\')}").replace("/", relpathsep)
 
 def _read_file(path, encoding = "UTF-8"):
     bundle = _get_bundle()
 
     if bundle is not None:
         return bundle.open(path).decode(encoding)
```

### Comparing `ralium-2.1.0/ralium/_util.pyi` & `ralium-2.1.1/ralium/_util.pyi`

 * *Files identical despite different names*

### Comparing `ralium-2.1.0/ralium/api.py` & `ralium-2.1.1/ralium/api.py`

 * *Files identical despite different names*

### Comparing `ralium-2.1.0/ralium/api.pyi` & `ralium-2.1.1/ralium/api.pyi`

 * *Files identical despite different names*

### Comparing `ralium-2.1.0/ralium/builtins.py` & `ralium-2.1.1/ralium/builtins.py`

 * *Files identical despite different names*

### Comparing `ralium-2.1.0/ralium/builtins.pyi` & `ralium-2.1.1/ralium/builtins.pyi`

 * *Files identical despite different names*

### Comparing `ralium-2.1.0/ralium/bundle.py` & `ralium-2.1.1/ralium/bundle.py`

 * *Files identical despite different names*

### Comparing `ralium-2.1.0/ralium/bundle.pyi` & `ralium-2.1.1/ralium/bundle.pyi`

 * *Files identical despite different names*

### Comparing `ralium-2.1.0/ralium/config.py` & `ralium-2.1.1/ralium/config.py`

 * *Files identical despite different names*

### Comparing `ralium-2.1.0/ralium/element.py` & `ralium-2.1.1/ralium/element.py`

 * *Files identical despite different names*

### Comparing `ralium-2.1.0/ralium/element.pyi` & `ralium-2.1.1/ralium/element.pyi`

 * *Files identical despite different names*

### Comparing `ralium-2.1.0/ralium/engine.py` & `ralium-2.1.1/ralium/engine.py`

 * *Files identical despite different names*

### Comparing `ralium-2.1.0/ralium/engine.pyi` & `ralium-2.1.1/ralium/engine.pyi`

 * *Files identical despite different names*

### Comparing `ralium-2.1.0/ralium/errors.py` & `ralium-2.1.1/ralium/errors.py`

 * *Files identical despite different names*

### Comparing `ralium-2.1.0/ralium/listener.py` & `ralium-2.1.1/ralium/listener.py`

 * *Files identical despite different names*

### Comparing `ralium-2.1.0/ralium/listener.pyi` & `ralium-2.1.1/ralium/listener.pyi`

 * *Files identical despite different names*

### Comparing `ralium-2.1.0/ralium/navigation.py` & `ralium-2.1.1/ralium/navigation.py`

 * *Files identical despite different names*

### Comparing `ralium-2.1.0/ralium/pyhtml.py` & `ralium-2.1.1/ralium/pyhtml.py`

 * *Files identical despite different names*

### Comparing `ralium-2.1.0/ralium/pyhtml.pyi` & `ralium-2.1.1/ralium/pyhtml.pyi`

 * *Files identical despite different names*

### Comparing `ralium-2.1.0/ralium/setuptools.py` & `ralium-2.1.1/ralium/setuptools.py`

 * *Files identical despite different names*

### Comparing `ralium-2.1.0/ralium/setuptools.pyi` & `ralium-2.1.1/ralium/setuptools.pyi`

 * *Files identical despite different names*

### Comparing `ralium-2.1.0/ralium/webpage.py` & `ralium-2.1.1/ralium/webpage.py`

 * *Files identical despite different names*

### Comparing `ralium-2.1.0/ralium/webpage.pyi` & `ralium-2.1.1/ralium/webpage.pyi`

 * *Files identical despite different names*

### Comparing `ralium-2.1.0/ralium/window.py` & `ralium-2.1.1/ralium/window.py`

 * *Files identical despite different names*

### Comparing `ralium-2.1.0/ralium/window.pyi` & `ralium-2.1.1/ralium/window.pyi`

 * *Files identical despite different names*

### Comparing `ralium-2.1.0/ralium.egg-info/PKG-INFO` & `ralium-2.1.1/ralium.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ralium
-Version: 2.1.0
+Version: 2.1.1
 Summary: An easy to use wrapper for pywebview.
 Author-email: Isaiah Coroama <coroamaisaiah@gmail.com>
 License:                     GNU GENERAL PUBLIC LICENSE
                                Version 3, 29 June 2007
         
          Copyright (C) 2007 Free Software Foundation, Inc. <https://fsf.org/>
          Everyone is permitted to copy and distribute verbatim copies
```

### Comparing `ralium-2.1.0/ralium.egg-info/SOURCES.txt` & `ralium-2.1.1/ralium.egg-info/SOURCES.txt`

 * *Files identical despite different names*

