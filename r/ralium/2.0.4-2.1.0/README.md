# Comparing `tmp/ralium-2.0.4.tar.gz` & `tmp/ralium-2.1.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ralium-2.0.4.tar", last modified: Tue May 28 05:38:10 2024, max compression
+gzip compressed data, was "ralium-2.1.0.tar", last modified: Wed May 29 00:46:53 2024, max compression
```

## Comparing `ralium-2.0.4.tar` & `ralium-2.1.0.tar`

### file list

```diff
@@ -1,41 +1,41 @@
-drwxrwxrwx   0        0        0        0 2024-05-28 05:38:10.041849 ralium-2.0.4/
--rw-rw-rw-   0        0        0    35823 2024-05-21 00:22:26.000000 ralium-2.0.4/LICENSE
--rw-rw-rw-   0        0        0    41897 2024-05-28 05:38:10.041849 ralium-2.0.4/PKG-INFO
--rw-rw-rw-   0        0        0       52 2024-05-21 00:22:26.000000 ralium-2.0.4/README.md
--rw-rw-rw-   0        0        0      970 2024-05-28 05:37:44.000000 ralium-2.0.4/pyproject.toml
-drwxrwxrwx   0        0        0        0 2024-05-28 05:38:10.020226 ralium-2.0.4/ralium/
--rw-rw-rw-   0        0        0      357 2024-05-21 05:00:06.000000 ralium-2.0.4/ralium/__init__.py
--rw-rw-rw-   0        0        0     1895 2024-05-28 05:37:50.000000 ralium-2.0.4/ralium/_util.py
--rw-rw-rw-   0        0        0     1098 2024-05-27 18:21:08.000000 ralium-2.0.4/ralium/_util.pyi
--rw-rw-rw-   0        0        0     7555 2024-05-21 04:21:31.000000 ralium-2.0.4/ralium/api.py
--rw-rw-rw-   0        0        0     1066 2024-05-21 00:25:27.000000 ralium-2.0.4/ralium/api.pyi
--rw-rw-rw-   0        0        0      680 2024-05-21 00:25:27.000000 ralium-2.0.4/ralium/builtins.py
--rw-rw-rw-   0        0        0      541 2024-05-21 00:25:27.000000 ralium-2.0.4/ralium/builtins.pyi
--rw-rw-rw-   0        0        0     8231 2024-05-21 06:11:47.000000 ralium-2.0.4/ralium/bundle.py
--rw-rw-rw-   0        0        0     1581 2024-05-21 00:26:03.000000 ralium-2.0.4/ralium/bundle.pyi
--rw-rw-rw-   0        0        0     3332 2024-05-21 00:25:27.000000 ralium-2.0.4/ralium/config.py
--rw-rw-rw-   0        0        0      467 2024-05-21 00:25:27.000000 ralium-2.0.4/ralium/config.pyi
--rw-rw-rw-   0        0        0     6425 2024-05-21 00:25:27.000000 ralium-2.0.4/ralium/element.py
--rw-rw-rw-   0        0        0     1376 2024-05-21 00:26:03.000000 ralium-2.0.4/ralium/element.pyi
--rw-rw-rw-   0        0        0     4402 2024-05-21 00:26:03.000000 ralium-2.0.4/ralium/engine.py
--rw-rw-rw-   0        0        0     1389 2024-05-21 00:25:27.000000 ralium-2.0.4/ralium/engine.pyi
--rw-rw-rw-   0        0        0     1147 2024-05-27 18:22:26.000000 ralium-2.0.4/ralium/errors.py
--rw-rw-rw-   0        0        0     2387 2024-05-21 00:25:27.000000 ralium-2.0.4/ralium/listener.py
--rw-rw-rw-   0        0        0      890 2024-05-21 00:25:27.000000 ralium-2.0.4/ralium/listener.pyi
--rw-rw-rw-   0        0        0      804 2024-05-21 00:25:27.000000 ralium-2.0.4/ralium/navigation.py
--rw-rw-rw-   0        0        0      376 2024-05-21 00:25:27.000000 ralium-2.0.4/ralium/navigation.pyi
--rw-rw-rw-   0        0        0     4805 2024-05-21 15:38:14.000000 ralium-2.0.4/ralium/pyhtml.py
--rw-rw-rw-   0        0        0      531 2024-05-21 07:20:26.000000 ralium-2.0.4/ralium/pyhtml.pyi
--rw-rw-rw-   0        0        0     7851 2024-05-21 05:23:35.000000 ralium-2.0.4/ralium/setuptools.py
--rw-rw-rw-   0        0        0      965 2024-05-21 05:19:13.000000 ralium-2.0.4/ralium/setuptools.pyi
--rw-rw-rw-   0        0        0     6452 2024-05-27 18:22:15.000000 ralium-2.0.4/ralium/webpage.py
--rw-rw-rw-   0        0        0     1870 2024-05-21 00:26:03.000000 ralium-2.0.4/ralium/webpage.pyi
--rw-rw-rw-   0        0        0     6078 2024-05-27 18:21:30.000000 ralium-2.0.4/ralium/window.py
--rw-rw-rw-   0        0        0      693 2024-05-21 00:25:27.000000 ralium-2.0.4/ralium/window.pyi
-drwxrwxrwx   0        0        0        0 2024-05-28 05:38:10.040516 ralium-2.0.4/ralium.egg-info/
--rw-rw-rw-   0        0        0    41897 2024-05-28 05:38:09.000000 ralium-2.0.4/ralium.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      692 2024-05-28 05:38:09.000000 ralium-2.0.4/ralium.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-05-28 05:38:09.000000 ralium-2.0.4/ralium.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       42 2024-05-28 05:38:09.000000 ralium-2.0.4/ralium.egg-info/requires.txt
--rw-rw-rw-   0        0        0        7 2024-05-28 05:38:09.000000 ralium-2.0.4/ralium.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2024-05-28 05:38:10.043162 ralium-2.0.4/setup.cfg
+drwxrwxrwx   0        0        0        0 2024-05-29 00:46:53.117566 ralium-2.1.0/
+-rw-rw-rw-   0        0        0    35823 2024-05-21 00:22:26.000000 ralium-2.1.0/LICENSE
+-rw-rw-rw-   0        0        0    41897 2024-05-29 00:46:53.116276 ralium-2.1.0/PKG-INFO
+-rw-rw-rw-   0        0        0       52 2024-05-21 00:22:26.000000 ralium-2.1.0/README.md
+-rw-rw-rw-   0        0        0      970 2024-05-29 00:45:51.000000 ralium-2.1.0/pyproject.toml
+drwxrwxrwx   0        0        0        0 2024-05-29 00:46:53.091605 ralium-2.1.0/ralium/
+-rw-rw-rw-   0        0        0      357 2024-05-21 05:00:06.000000 ralium-2.1.0/ralium/__init__.py
+-rw-rw-rw-   0        0        0     2247 2024-05-29 00:45:57.000000 ralium-2.1.0/ralium/_util.py
+-rw-rw-rw-   0        0        0     1192 2024-05-29 00:14:14.000000 ralium-2.1.0/ralium/_util.pyi
+-rw-rw-rw-   0        0        0     7555 2024-05-29 00:26:49.000000 ralium-2.1.0/ralium/api.py
+-rw-rw-rw-   0        0        0     1066 2024-05-21 00:25:27.000000 ralium-2.1.0/ralium/api.pyi
+-rw-rw-rw-   0        0        0      680 2024-05-21 00:25:27.000000 ralium-2.1.0/ralium/builtins.py
+-rw-rw-rw-   0        0        0      541 2024-05-21 00:25:27.000000 ralium-2.1.0/ralium/builtins.pyi
+-rw-rw-rw-   0        0        0     9527 2024-05-29 00:38:25.000000 ralium-2.1.0/ralium/bundle.py
+-rw-rw-rw-   0        0        0     1958 2024-05-29 00:37:29.000000 ralium-2.1.0/ralium/bundle.pyi
+-rw-rw-rw-   0        0        0     3332 2024-05-21 00:25:27.000000 ralium-2.1.0/ralium/config.py
+-rw-rw-rw-   0        0        0      467 2024-05-21 00:25:27.000000 ralium-2.1.0/ralium/config.pyi
+-rw-rw-rw-   0        0        0     6425 2024-05-21 00:25:27.000000 ralium-2.1.0/ralium/element.py
+-rw-rw-rw-   0        0        0     1376 2024-05-21 00:26:03.000000 ralium-2.1.0/ralium/element.pyi
+-rw-rw-rw-   0        0        0     4402 2024-05-21 00:26:03.000000 ralium-2.1.0/ralium/engine.py
+-rw-rw-rw-   0        0        0     1389 2024-05-21 00:25:27.000000 ralium-2.1.0/ralium/engine.pyi
+-rw-rw-rw-   0        0        0     1147 2024-05-27 18:22:26.000000 ralium-2.1.0/ralium/errors.py
+-rw-rw-rw-   0        0        0     2387 2024-05-21 00:25:27.000000 ralium-2.1.0/ralium/listener.py
+-rw-rw-rw-   0        0        0      890 2024-05-21 00:25:27.000000 ralium-2.1.0/ralium/listener.pyi
+-rw-rw-rw-   0        0        0      804 2024-05-21 00:25:27.000000 ralium-2.1.0/ralium/navigation.py
+-rw-rw-rw-   0        0        0      376 2024-05-21 00:25:27.000000 ralium-2.1.0/ralium/navigation.pyi
+-rw-rw-rw-   0        0        0     4847 2024-05-28 23:54:13.000000 ralium-2.1.0/ralium/pyhtml.py
+-rw-rw-rw-   0        0        0      531 2024-05-21 07:20:26.000000 ralium-2.1.0/ralium/pyhtml.pyi
+-rw-rw-rw-   0        0        0     7678 2024-05-28 23:49:25.000000 ralium-2.1.0/ralium/setuptools.py
+-rw-rw-rw-   0        0        0      959 2024-05-28 23:49:19.000000 ralium-2.1.0/ralium/setuptools.pyi
+-rw-rw-rw-   0        0        0     6471 2024-05-29 00:21:58.000000 ralium-2.1.0/ralium/webpage.py
+-rw-rw-rw-   0        0        0     1870 2024-05-21 00:26:03.000000 ralium-2.1.0/ralium/webpage.pyi
+-rw-rw-rw-   0        0        0     6078 2024-05-29 00:22:41.000000 ralium-2.1.0/ralium/window.py
+-rw-rw-rw-   0        0        0      693 2024-05-21 00:25:27.000000 ralium-2.1.0/ralium/window.pyi
+drwxrwxrwx   0        0        0        0 2024-05-29 00:46:53.114766 ralium-2.1.0/ralium.egg-info/
+-rw-rw-rw-   0        0        0    41897 2024-05-29 00:46:53.000000 ralium-2.1.0/ralium.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      692 2024-05-29 00:46:53.000000 ralium-2.1.0/ralium.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-05-29 00:46:53.000000 ralium-2.1.0/ralium.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       42 2024-05-29 00:46:53.000000 ralium-2.1.0/ralium.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        7 2024-05-29 00:46:53.000000 ralium-2.1.0/ralium.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2024-05-29 00:46:53.117566 ralium-2.1.0/setup.cfg
```

### Comparing `ralium-2.0.4/LICENSE` & `ralium-2.1.0/LICENSE`

 * *Files identical despite different names*

### Comparing `ralium-2.0.4/PKG-INFO` & `ralium-2.1.0/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ralium
-Version: 2.0.4
+Version: 2.1.0
 Summary: An easy to use wrapper for pywebview.
 Author-email: Isaiah Coroama <coroamaisaiah@gmail.com>
 License:                     GNU GENERAL PUBLIC LICENSE
                                Version 3, 29 June 2007
         
          Copyright (C) 2007 Free Software Foundation, Inc. <https://fsf.org/>
          Everyone is permitted to copy and distribute verbatim copies
```

### Comparing `ralium-2.0.4/pyproject.toml` & `ralium-2.1.0/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires      = ["setuptools >= 69.5.0", "wheel >= 0.43.0"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "ralium"
-version = "2.0.4"
+version = "2.1.0"
 description = "An easy to use wrapper for pywebview."
 readme = "README.md"
 authors = [{ name = "Isaiah Coroama", email = "coroamaisaiah@gmail.com" }]
 license = { file = "LICENSE" }
 classifiers = [
     'Development Status :: 3 - Alpha',
     'Intended Audience :: Developers',
```

### Comparing `ralium-2.0.4/ralium/_util.py` & `ralium-2.1.0/ralium/_util.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,17 +1,18 @@
 import http.server
+import string
 import sys
 import os
 
 __all__ = [
     "__version__", "BasicHTTPServer", "NamedDict", "_get_http_server_handler", "_get_bundle", 
-    "_norm_url", "_check_exists",  "_check_is_dir", "_read_file", "_get_path"
+    "_norm_url", "_norm_path", "_check_exists",  "_check_is_dir", "_read_file", "_get_path"
 ]
 
-__version__ = "2.0.4"
+__version__ = "2.1.0"
 
 SYS_BUNDLE_ATTRIBUTE = "bundled"
 
 class BasicHTTPServer(http.server.SimpleHTTPRequestHandler):
     pass
 
 class NamedDict(dict):
@@ -19,57 +20,71 @@
         for key, value in iterable.items():
             if isinstance(value, dict):
                 self[key] = NamedDict(value)
                 continue
 
             self[key] = value
 
+def _is_abs_win(path):
+    if not sys.platform.startswith("win"):
+        return False
+
+    for letter in string.ascii_uppercase:
+        if path.startswith(f"{letter}:"):
+            return True
+
+    return False
+
 def _get_bundle():
     return getattr(sys, SYS_BUNDLE_ATTRIBUTE, None)
 
 def _get_http_server_handler():
     if _get_bundle() is not None:
         import ralium.bundle
         return ralium.bundle.BundledHTTPServer
     return BasicHTTPServer
 
 def _check_exists(path):
-    path = _norm_url(path)
+    path = _norm_path(path)
     bundle = _get_bundle()
 
     if bundle is not None:
-        if path in ["\\template", "\\template\\routes"]: return True
-        return bundle.get(path, False)
+        return bundle.exists(path)
     
     return os.path.exists(path)
 
 def _check_is_dir(path):
-    path = _norm_url(path)
     bundle = _get_bundle()
 
     if bundle is not None:
-        return True
+        return path in bundle.dirs
     
     return os.path.isdir(path)
 
 def _norm_url(path):
     return os.path.normpath(f"\\{path.lstrip('/\\')}").replace("\\", "/")
 
+def _norm_path(path):
+    if _is_abs_win(path):
+        return path
+    return os.path.normpath(f"\\{path.lstrip('/\\')}").replace("/", "\\")
+
 def _read_file(path, encoding = "UTF-8"):
     bundle = _get_bundle()
 
     if bundle is not None:
-        return bundle[path].decode(encoding)
+        return bundle.open(path).decode(encoding)
     
     with open(path, "r", encoding=encoding) as f:
         return f.read()
 
 def _get_path(path):
+    path = _norm_path(path)
     bundle = _get_bundle()
 
     if bundle is not None:
-        return _norm_url(path)
+        return path
 
     if getattr(sys, "frozen", False):
         return os.path.abspath(os.path.join(sys._MEIPASS, path))
 
-    return os.path.abspath(path)
+    return os.path.abspath(path.lstrip("\\"))
```

### Comparing `ralium-2.0.4/ralium/_util.pyi` & `ralium-2.1.0/ralium/_util.pyi`

 * *Files 8% similar despite different names*

```diff
@@ -14,29 +14,31 @@
     ModuleType
 )
 
 import http.server
 
 __all__ = [
     "__version__", "BasicHTTPServer", "NamedDict", "_get_http_server_handler", "_get_bundle", 
-    "_norm_url", "_check_exists",  "_check_is_dir", "_read_file", "_get_path"
+    "_norm_url", "_norm_path", "_check_exists",  "_check_is_dir", "_read_file", "_get_path"
 ]
 
 __version__: str
 
 _RT = TypeVar("_RT") # Return Type
 ClassType: TypeAlias = object
 DirPathStr: TypeAlias = str
 FilePathStr: TypeAlias = str
 
 class BasicHTTPServer(http.server.SimpleHTTPRequestHandler): ...
 
 class NamedDict(dict):
     def __init__(self, iterable: dict[str, Any]) -> None: ...
 
+def _is_abs_win(path: str) -> bool: ...
 def _get_bundle() -> FileSystem | None: ...
 def _get_http_server_handler() -> BasicHTTPServer | BundledHTTPServer: ...
 def _check_exists(path: str) -> bool: ...
 def _check_is_dir(path: str) -> bool: ...
 def _norm_url(path: str) -> str: ...
+def _norm_path(path: str) -> str: ...
 def _read_file(path: str, encoding: str = "UTF-8") -> str: ...
 def _get_path(path: str) -> str: ...
```

### Comparing `ralium-2.0.4/ralium/api.py` & `ralium-2.1.0/ralium/api.py`

 * *Files identical despite different names*

### Comparing `ralium-2.0.4/ralium/api.pyi` & `ralium-2.1.0/ralium/api.pyi`

 * *Files identical despite different names*

### Comparing `ralium-2.0.4/ralium/builtins.py` & `ralium-2.1.0/ralium/builtins.py`

 * *Files identical despite different names*

### Comparing `ralium-2.0.4/ralium/builtins.pyi` & `ralium-2.1.0/ralium/builtins.pyi`

 * *Files identical despite different names*

### Comparing `ralium-2.0.4/ralium/bundle.py` & `ralium-2.1.0/ralium/bundle.py`

 * *Files 8% similar despite different names*

```diff
@@ -12,23 +12,24 @@
 
 from shutil import COPY_BUFSIZE
 from http import HTTPStatus
 
 import urllib.parse
 import http.server
 import posixpath
-import sys
 import os
 
 IMAGE_FILE_EXTENSIONS = [
     ".apng", ".gif", ".ico", ".cur", ".jpg", ".jpeg", 
     ".jfif", ".pjpeg", ".pjp", ".png", ".svg", ".ico",
     ".webp"
 ]
 
+# A modified version of http.server.SimpleHTTPRequstHandler
+# made compatible with the custom 'FileSystem' class.
 class BundledHTTPServer(http.server.SimpleHTTPRequestHandler):
     def do_GET(self):
         """Serve a GET request."""
         f = self.send_head()
         if f is not None:
             try:
                 self.copyfile(f, self.wfile)
@@ -58,15 +59,15 @@
         # However, some OS platforms accept a trailingSlash as a filename
         # See discussion on python-dev and Issue34711 regarding
         # parsing and rejection of filenames with a trailing slash
         if path.endswith("/"):
             self.send_error(HTTPStatus.NOT_FOUND, "File not found")
             return None
         try:
-            f = _get_bundle()[path]
+            f = _get_bundle().open(path)
         except FileNotFoundError:
             self.send_error(HTTPStatus.NOT_FOUND, "File not found")
             return None
 
         try:
             self.send_response(HTTPStatus.OK)
             self.send_header("Content-type", ctype)
@@ -108,68 +109,107 @@
 
     def copyfile(self, fsrc, fdst):
         fdst_write = fdst.write
         while buf := fsrc[:COPY_BUFSIZE]:
             fdst_write(buf)
 
 class File:
+    __slots__ = ("relpath", "content",)
+
     def __init__(self, relpath, content):
         self.relpath = relpath
         self.content = content
     
     def __str__(self):
         return self.content.decode()
 
     def __repr__(self):
         return f"ralium.bundle.File(relpath='{self.relpath.replace('\\', '\\\\')}', content={repr(self.content)})"
     
 class Bundle:
+    __slots__ = ("url", "page", "server", "styles",)
+
     def __init__(self, *, url, page, server, styles):
         self.url = url
         self.page = page
         self.server = server
         self.styles = styles
     
     def __repr__(self):
         return f"ralium.bundle.Bundle(url='{self.url}', page={repr(self.page)}, server={repr(self.server)}, styles=[{''.join([repr(v) for v in self.styles])}])"
 
-class FileSystem(dict):
+class FileSystem:
+    __slots__ = ("images", "styles", "bundles", "dirs", "files",)
+
     def __init__(self, *, images, styles, bundles):
         self.images = images
         self.styles = styles
         self.bundles = bundles
 
+        self.dirs = ["\\"]
+        self.files = {}
+
         for image in images:
-            self[image.relpath] = image.content
-        
+            self.__add_file(image)
+
         for style in styles:
-            self[style.relpath] = style.content
+            self.__add_file(style)
         
         for bundle in bundles:
-            self[bundle.page.relpath] = bundle.page.content
+            self.__add_file(bundle.page)
 
             if bundle.server is not None:
-                self[bundle.server.relpath] = bundle.server.content
+                self.__add_file(bundle.server)
             
             for style in bundle.styles:
-                self[style.relpath] = style.content
+                self.__add_file(style)
     
-    def __getitem__(self, __path):
+    def __add_file(self, file):
+        segments = file.relpath.split("\\")[1:]
+        segments = [f"\\{'\\'.join([*segments[:i], v])}" for i, v in enumerate(segments)]
+
+        self.mkdirs(*segments[:-1])
+        self.mkfiles(**{segments[-1]: file.content})
+
+    def open(self, filename):
         try:
-            return super().__getitem__(__path)
+            return self.files[filename]
         except KeyError:
-            raise FileNotFoundError(f"Failed to find '{__path}'")
+            raise FileNotFoundError(f"'{filename}' does not exist.")
+    
+    def exists(self, path):
+        if self.files.get(path) is not None:
+            return False
+        return path in self.dirs
+
+    def mkdirs(self, *dirs):
+        self.dirs.extend(dirs)
+    
+    def mkfile(self, filename, data):
+        if not isinstance(filename, str):
+            raise TypeError(f"File name must be of type str, intead got '{type(filename)}'")
+        
+        if not isinstance(data, bytes):
+            raise TypeError(f"File content must be of type bytes, instead got '{type(data)}'.")
+
+        self.files[filename] = data
+    
+    def mkfiles(self, **files):
+        for filename, data in files.items():
+            self.mkfile(filename, data)
 
 class PyBundler:
+    __slots__ = ("pyfile", "webfolder", "webroutes", "cssfolder", "imgfolder",)
+
     def __init__(self, pyfile, webfolder):
         self.pyfile = pyfile
         self.webfolder = _get_path(webfolder)
-        self.webroutes = os.path.normpath(os.path.join(webfolder, "routes"))
-        self.cssfolder = os.path.normpath(os.path.join(webfolder, "styles"))
-        self.imgfolder = os.path.normpath(os.path.join(webfolder, "images"))
+        self.webroutes = os.path.normpath(os.path.join(self.webfolder, "routes"))
+        self.cssfolder = os.path.normpath(os.path.join(self.webfolder, "styles"))
+        self.imgfolder = os.path.normpath(os.path.join(self.webfolder, "images"))
 
         _check_web_folder(self.webfolder)
         _check_web_routes(self.webroutes)
 
     def view(self):
         images = self.collect(self.imgfolder, PyBundler.isimage)
         styles = self.collect(self.cssfolder, PyBundler.iscss)
```

### Comparing `ralium-2.0.4/ralium/bundle.pyi` & `ralium-2.1.0/ralium/bundle.pyi`

 * *Files 4% similar despite different names*

```diff
@@ -13,38 +13,50 @@
     def do_GET(self) -> None: ...
     def do_HEAD(self) -> None: ...
     def send_head(self) -> bytes | None: ...
     def translate_path(self, path) -> str: ...
     def copyfile(self, fsrc: bytes, fdst: BinaryIO) -> None: ...
 
 class File:
+    __slots__: tuple[str]
+    
     def __init__(self, relpath: str, content: bytes) -> None: ...
     def __str__(self) -> str: ...
     def __repr__(self) -> str: ...
 
 class Bundle:
+    __slots__: tuple[str]
+
     def __init__(self, *,
         url: str,
         page: bytes,
         server: bytes | None,
         styles: list[File]
     ) -> None: ...
 
     def __repr__(self) -> str: ...
 
 class FileSystem(dict):
+    __slots__: tuple[str]
+
     def __init__(self, *,
         images: list[File],
         styles: list[File],
         bundles: list[Bundle]
     ) -> None: ...
 
-    def __getitem__(self, __path: FilePathStr) -> bytes: ...
+    def open(self, filename: FilePathStr) -> bytes: ...
+    def exists(self, path: FilePathStr | DirPathStr) -> bool: ...
+    def mkdirs(self, *dirs: tuple[DirPathStr]) -> None: ...
+    def mkfile(self, filename: FilePathStr, data: bytes) -> None: ...
+    def mkfiles(self, **files: dict[str, bytes]) -> None: ...
 
 class PyBundler:
+    __slots__: tuple[str]
+
     def __init__(self, pyfile: FilePathStr, webfolder: DirPathStr) -> None: ...
 
     def view(self) -> list[bytes]: ...
     def relpath(self, filename: FilePathStr) -> FilePathStr: ...
     def collect(self, dir: DirPathStr, callback: Callable[[FilePathStr], bool]) -> list[File]: ...
 
     @staticmethod
```

### Comparing `ralium-2.0.4/ralium/config.py` & `ralium-2.1.0/ralium/config.py`

 * *Files identical despite different names*

### Comparing `ralium-2.0.4/ralium/element.py` & `ralium-2.1.0/ralium/element.py`

 * *Files identical despite different names*

### Comparing `ralium-2.0.4/ralium/element.pyi` & `ralium-2.1.0/ralium/element.pyi`

 * *Files identical despite different names*

### Comparing `ralium-2.0.4/ralium/engine.py` & `ralium-2.1.0/ralium/engine.py`

 * *Files identical despite different names*

### Comparing `ralium-2.0.4/ralium/engine.pyi` & `ralium-2.1.0/ralium/engine.pyi`

 * *Files identical despite different names*

### Comparing `ralium-2.0.4/ralium/errors.py` & `ralium-2.1.0/ralium/errors.py`

 * *Files identical despite different names*

### Comparing `ralium-2.0.4/ralium/listener.py` & `ralium-2.1.0/ralium/listener.py`

 * *Files identical despite different names*

### Comparing `ralium-2.0.4/ralium/listener.pyi` & `ralium-2.1.0/ralium/listener.pyi`

 * *Files identical despite different names*

### Comparing `ralium-2.0.4/ralium/navigation.py` & `ralium-2.1.0/ralium/navigation.py`

 * *Files identical despite different names*

### Comparing `ralium-2.0.4/ralium/pyhtml.py` & `ralium-2.1.0/ralium/pyhtml.py`

 * *Files 3% similar despite different names*

```diff
@@ -2,14 +2,16 @@
 from ralium._util import NamedDict
 import copy
 import re
 
 RE_HTML_PATTERN = r"((<.*>.*</.*>)|(<.*/>))"
 
 class PyHTML:
+    __slots__ = ("_html", "_webhook",)
+
     def __init__(self, webhook):
         self._html = webhook.html
         self._webhook = webhook
     
     def compile(self):
         """
         Compiles the HTML content of the webhook by processing embedded Ralium tags.
```

### Comparing `ralium-2.0.4/ralium/pyhtml.pyi` & `ralium-2.1.0/ralium/pyhtml.pyi`

 * *Files identical despite different names*

### Comparing `ralium-2.0.4/ralium/setuptools.py` & `ralium-2.1.0/ralium/setuptools.py`

 * *Files 2% similar despite different names*

```diff
@@ -115,53 +115,50 @@
     icon = None,
     bundle = False,
     webfolder = None,
     warnings = False,
     onefile = True,
     noconsole = True,
     bundle_dist = None,
+    optimize = None,
     pyi_args = None,
     use_subprocess = False,
-    optimize_level = None
 ):
     """
     Compiles a Ralium project to an executable using PyInstaller.
 
     :param pyfile: The python file to compile.
     :param name: Display name for the executable.
     :param icon: Display icon for the executable.
     :param bundle: Bundles all of the html, css, python and image files into one executable. (Requires a `webfolder`)
     :param webfolder: Directory of the project.
     :param warnings: Calls the `DisableWarnings` to prevent warnings.
     :param onefile: Creates the executable as a standalone file.
     :param noconsole: Prevents a console from being displayed.
     :param bundle_dist: The directory name Ralium will use for bundling projects. (Default: `dist`)
+    :param optimize: Set the `PYTHONOPTIMIZE` level or the PyInstaller `--optimize` flag. (Default: `0`)
     :param pyi_args: Extra parameters for PyInstaller to use.
     :param use_subprocess: Use `PyInstaller` through a subprocess.
-    :param optimize_level: Set the `PYTHONOPTIMIZE` level. (Requires use_subprocess to be `True`)
 
     :raises TypeError: If the name or icon is not a `str` or `None`.
-    :raises SetupError: If `bundle` is `True` while the `webfolder` is `None` or if `optimize_level` is set without `use_subprocess` being `True`.
+    :raises SetupError: If `bundle` is `True` while the `webfolder` is `None`.
     :raises RuntimeError: If this function is called within an already compiled executable file.
     :raises FileNotFoundError: If a certain file path doesn't exist.
     """
 
     logger.info("Ralium: %s", __version__)
 
     if getattr(sys, "frozen", False):
         raise RuntimeError("Ralium 'setup' cannot be ran from an executable file.")
 
     if not os.path.exists(pyfile):
         raise FileNotFoundError(f"Failed to find python file '{pyfile}'")
     
-    if optimize_level is not None and not use_subprocess:
-        raise SetupError("Optimization level can only be set if 'use_subprocess' is 'True'.")
-    
-    if optimize_level not in [None, *range(0, 3)]:
-        raise ValueError("The optimization level must be in the range of 0 - 2.")
+    if optimize not in [None, *range(0, 3)]:
+        raise ValueError("The optimization level must be the value of 0, 1, or 2.")
 
     args = [pyfile, *(pyi_args or [])]
 
     if name is not None:
         if not isinstance(name, str):
             raise _exe_str_error("name", name)
         
@@ -196,24 +193,26 @@
     elif webfolder:
         for src, dst in collect_webfolder(webfolder).items():
             args.append(_add_data_arg(src, dst))
 
     if use_subprocess:
         optimize_flag = ""
 
-        match optimize_level:
+        match optimize:
             case 1: optimize_flag = "-O"
             case 2: optimize_flag = "-OO"
         
         args = [
             sys.executable,
             "-m",
             "PyInstaller",
             *args
         ]
 
         if optimize_flag:
             args.insert(1, optimize_flag)
         
         return subprocess.run(args) and None
+    else:
+        args.append(f"--optimize={optimize or 0}")
     
     pack(args)
```

### Comparing `ralium-2.0.4/ralium/setuptools.pyi` & `ralium-2.1.0/ralium/setuptools.pyi`

 * *Files 2% similar despite different names*

```diff
@@ -26,11 +26,11 @@
     icon: FilePathStr | None = None,
     bundle: bool = False,
     webfolder: DirPathStr | None = None,
     warnings: bool = False,
     onefile: bool = True,
     noconsole: bool = True,
     bundle_dist: DirPathStr | None = None,
+    optimize: int | None = None,
     pyi_args: list[str] | None = None,
-    use_subprocess: bool = False,
-    optimize_level: int | None = None
+    use_subprocess: bool = False
 ) -> None: ...
```

### Comparing `ralium-2.0.4/ralium/webpage.py` & `ralium-2.1.0/ralium/webpage.py`

 * *Files 2% similar despite different names*

```diff
@@ -128,15 +128,15 @@
     def _get_css(self):
         if isinstance(self.css, (list, tuple, set,)):
             files = [item for item in self.css if _check_exists(item)]
             values = [item for item in self.css if not _check_exists(item)]
             self.css = "\n".join([CSSReader(*files, encoding=self.encoding).content, *values])
             return
         
-        if isinstance(self.css, (str, bytes,)) and _check_exists(self.css):
+        if isinstance(self.css, (str, bytes,)) and _check_exists(self.css) and self.css != "":
             self.css = CSSReader(self.css, encoding=self.encoding).content
     
     def _wrap_functions(self):
         if self.window is None:
             return
 
         self.functions = [WebHookFunction(function, self.window) for function in self.functions]
```

### Comparing `ralium-2.0.4/ralium/webpage.pyi` & `ralium-2.1.0/ralium/webpage.pyi`

 * *Files identical despite different names*

### Comparing `ralium-2.0.4/ralium/window.py` & `ralium-2.1.0/ralium/window.py`

 * *Files identical despite different names*

### Comparing `ralium-2.0.4/ralium/window.pyi` & `ralium-2.1.0/ralium/window.pyi`

 * *Files identical despite different names*

### Comparing `ralium-2.0.4/ralium.egg-info/PKG-INFO` & `ralium-2.1.0/ralium.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ralium
-Version: 2.0.4
+Version: 2.1.0
 Summary: An easy to use wrapper for pywebview.
 Author-email: Isaiah Coroama <coroamaisaiah@gmail.com>
 License:                     GNU GENERAL PUBLIC LICENSE
                                Version 3, 29 June 2007
         
          Copyright (C) 2007 Free Software Foundation, Inc. <https://fsf.org/>
          Everyone is permitted to copy and distribute verbatim copies
```

### Comparing `ralium-2.0.4/ralium.egg-info/SOURCES.txt` & `ralium-2.1.0/ralium.egg-info/SOURCES.txt`

 * *Files identical despite different names*

