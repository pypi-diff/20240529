# Comparing `tmp/zrcl-0.3.0.tar.gz` & `tmp/zrcl-0.3.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "zrcl-0.3.0.tar", max compression
+gzip compressed data, was "zrcl-0.3.1.tar", max compression
```

## Comparing `zrcl-0.3.0.tar` & `zrcl-0.3.1.tar`

### file list

```diff
@@ -1,32 +1,33 @@
--rw-r--r--   0        0        0     1085 2024-05-09 17:36:26.540318 zrcl-0.3.0/LICENSE
--rw-r--r--   0        0        0     1524 2024-05-12 17:05:46.256632 zrcl-0.3.0/pyproject.toml
--rw-r--r--   0        0        0     1093 2024-05-11 15:06:11.869950 zrcl-0.3.0/README.md
--rw-r--r--   0        0        0        0 2024-05-09 17:37:17.169306 zrcl-0.3.0/src/zrcl3_uses/__init__.py
--rw-r--r--   0        0        0    10579 2024-05-12 17:03:07.540952 zrcl-0.3.0/src/zrcl3_uses/automation.py
--rw-r--r--   0        0        0      245 2024-05-09 18:05:40.455832 zrcl-0.3.0/src/zrcl3_uses/bit.py
--rw-r--r--   0        0        0     2240 2024-05-09 18:05:40.471062 zrcl-0.3.0/src/zrcl3_uses/cli_selection.py
--rw-r--r--   0        0        0      276 2024-05-09 18:05:40.453821 zrcl-0.3.0/src/zrcl3_uses/do_nothing.py
--rw-r--r--   0        0        0     5163 2024-05-12 15:33:36.125350 zrcl-0.3.0/src/zrcl3_uses/file.py
--rw-r--r--   0        0        0     4764 2024-05-10 19:06:51.955640 zrcl-0.3.0/src/zrcl3_uses/github.py
--rw-r--r--   0        0        0     1478 2024-05-09 18:05:40.475062 zrcl-0.3.0/src/zrcl3_uses/markdown.py
--rw-r--r--   0        0        0     6922 2024-05-10 17:45:30.801464 zrcl-0.3.0/src/zrcl3_uses/png_meta.py
--rw-r--r--   0        0        0      455 2024-05-09 18:05:40.469121 zrcl-0.3.0/src/zrcl3_uses/singleton.py
--rw-r--r--   0        0        0     1228 2024-05-09 18:05:40.415956 zrcl-0.3.0/src/zrcl3_uses/zip_crack.py
--rw-r--r--   0        0        0       49 2024-05-10 18:43:59.832504 zrcl-0.3.0/src/zrcl4/__init__.py
--rw-r--r--   0        0        0     2594 2024-05-10 18:43:59.862096 zrcl-0.3.0/src/zrcl4/__primitive__.py
--rw-r--r--   0        0        0     5144 2024-05-10 18:43:59.867653 zrcl-0.3.0/src/zrcl4/cryptography.py
--rw-r--r--   0        0        0     1371 2024-05-09 18:05:40.432405 zrcl-0.3.0/src/zrcl4/easyocr.py
--rw-r--r--   0        0        0      837 2024-05-09 18:05:40.415956 zrcl-0.3.0/src/zrcl4/hashlib.py
--rw-r--r--   0        0        0      348 2024-05-12 15:03:33.410713 zrcl-0.3.0/src/zrcl4/json.py
--rw-r--r--   0        0        0      427 2024-05-09 18:05:40.415956 zrcl-0.3.0/src/zrcl4/keyring.py
--rw-r--r--   0        0        0      128 2024-05-09 18:05:40.415450 zrcl-0.3.0/src/zrcl4/logging.py
--rw-r--r--   0        0        0      149 2024-05-09 18:05:40.415956 zrcl-0.3.0/src/zrcl4/os.py
--rw-r--r--   0        0        0      234 2024-05-09 18:05:40.415956 zrcl-0.3.0/src/zrcl4/pillow.py
--rw-r--r--   0        0        0     2995 2024-05-12 16:42:08.316590 zrcl-0.3.0/src/zrcl4/pygetwindow.py
--rw-r--r--   0        0        0     2374 2024-05-09 18:05:40.448673 zrcl-0.3.0/src/zrcl4/pyscreeze.py
--rw-r--r--   0        0        0      441 2024-05-09 18:05:40.439260 zrcl-0.3.0/src/zrcl4/pywin32.py
--rw-r--r--   0        0        0     1842 2024-05-12 15:54:49.777054 zrcl-0.3.0/src/zrcl4/screeninfo.py
--rw-r--r--   0        0        0     4434 2024-05-09 18:05:40.464698 zrcl-0.3.0/src/zrcl4/subprocess.py
--rw-r--r--   0        0        0     1511 2024-05-09 18:05:40.456834 zrcl-0.3.0/src/zrcl4/time.py
--rw-r--r--   0        0        0     2055 2024-05-09 18:05:40.465138 zrcl-0.3.0/src/zrcl4/typing.py
--rw-r--r--   0        0        0     1449 1970-01-01 00:00:00.000000 zrcl-0.3.0/PKG-INFO
+-rw-r--r--   0        0        0     1085 2024-05-09 17:36:26.540318 zrcl-0.3.1/LICENSE
+-rw-r--r--   0        0        0     1565 2024-05-29 03:27:20.405189 zrcl-0.3.1/pyproject.toml
+-rw-r--r--   0        0        0     1093 2024-05-11 15:06:11.869950 zrcl-0.3.1/README.md
+-rw-r--r--   0        0        0        0 2024-05-09 17:37:17.169306 zrcl-0.3.1/src/zrcl3_uses/__init__.py
+-rw-r--r--   0        0        0    10545 2024-05-29 01:22:55.881735 zrcl-0.3.1/src/zrcl3_uses/automation.py
+-rw-r--r--   0        0        0      245 2024-05-09 18:05:40.455832 zrcl-0.3.1/src/zrcl3_uses/bit.py
+-rw-r--r--   0        0        0     2240 2024-05-09 18:05:40.471062 zrcl-0.3.1/src/zrcl3_uses/cli_selection.py
+-rw-r--r--   0        0        0      276 2024-05-09 18:05:40.453821 zrcl-0.3.1/src/zrcl3_uses/do_nothing.py
+-rw-r--r--   0        0        0     5163 2024-05-29 01:22:55.847612 zrcl-0.3.1/src/zrcl3_uses/file.py
+-rw-r--r--   0        0        0     4761 2024-05-29 01:22:55.841612 zrcl-0.3.1/src/zrcl3_uses/github.py
+-rw-r--r--   0        0        0     1478 2024-05-09 18:05:40.475062 zrcl-0.3.1/src/zrcl3_uses/markdown.py
+-rw-r--r--   0        0        0     6922 2024-05-10 17:45:30.801464 zrcl-0.3.1/src/zrcl3_uses/png_meta.py
+-rw-r--r--   0        0        0      455 2024-05-09 18:05:40.469121 zrcl-0.3.1/src/zrcl3_uses/singleton.py
+-rw-r--r--   0        0        0     1228 2024-05-09 18:05:40.415956 zrcl-0.3.1/src/zrcl3_uses/zip_crack.py
+-rw-r--r--   0        0        0       49 2024-05-10 18:43:59.832504 zrcl-0.3.1/src/zrcl4/__init__.py
+-rw-r--r--   0        0        0     2594 2024-05-10 18:43:59.862096 zrcl-0.3.1/src/zrcl4/__primitive__.py
+-rw-r--r--   0        0        0     5144 2024-05-10 18:43:59.867653 zrcl-0.3.1/src/zrcl4/cryptography.py
+-rw-r--r--   0        0        0     1371 2024-05-09 18:05:40.432405 zrcl-0.3.1/src/zrcl4/easyocr.py
+-rw-r--r--   0        0        0     1687 2024-05-29 01:22:55.830051 zrcl-0.3.1/src/zrcl4/hashlib.py
+-rw-r--r--   0        0        0     2107 2024-05-29 03:23:52.968146 zrcl-0.3.1/src/zrcl4/json.py
+-rw-r--r--   0        0        0      427 2024-05-09 18:05:40.415956 zrcl-0.3.1/src/zrcl4/keyring.py
+-rw-r--r--   0        0        0      128 2024-05-09 18:05:40.415450 zrcl-0.3.1/src/zrcl4/logging.py
+-rw-r--r--   0        0        0     2432 2024-05-29 03:37:22.299721 zrcl-0.3.1/src/zrcl4/moviepy.py
+-rw-r--r--   0        0        0      149 2024-05-09 18:05:40.415956 zrcl-0.3.1/src/zrcl4/os.py
+-rw-r--r--   0        0        0      234 2024-05-29 01:22:55.827545 zrcl-0.3.1/src/zrcl4/pillow.py
+-rw-r--r--   0        0        0     3045 2024-05-29 03:26:18.977629 zrcl-0.3.1/src/zrcl4/pygetwindow.py
+-rw-r--r--   0        0        0     2374 2024-05-09 18:05:40.448673 zrcl-0.3.1/src/zrcl4/pyscreeze.py
+-rw-r--r--   0        0        0      441 2024-05-09 18:05:40.439260 zrcl-0.3.1/src/zrcl4/pywin32.py
+-rw-r--r--   0        0        0     1844 2024-05-29 01:22:55.846612 zrcl-0.3.1/src/zrcl4/screeninfo.py
+-rw-r--r--   0        0        0     4434 2024-05-09 18:05:40.464698 zrcl-0.3.1/src/zrcl4/subprocess.py
+-rw-r--r--   0        0        0     1511 2024-05-09 18:05:40.456834 zrcl-0.3.1/src/zrcl4/time.py
+-rw-r--r--   0        0        0     2055 2024-05-09 18:05:40.465138 zrcl-0.3.1/src/zrcl4/typing.py
+-rw-r--r--   0        0        0     1449 1970-01-01 00:00:00.000000 zrcl-0.3.1/PKG-INFO
```

### Comparing `zrcl-0.3.0/LICENSE` & `zrcl-0.3.1/LICENSE`

 * *Files identical despite different names*

### Comparing `zrcl-0.3.0/pyproject.toml` & `zrcl-0.3.1/pyproject.toml`

 * *Files 6% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "zrcl"
-version = "0.3.0"
+version = "0.3.1"
 description = ""
 authors = ["ZackaryW <36378555+ZackaryW@users.noreply.github.com>"]
 license = "MIT"
 readme = "README.md"
 packages = [
     { include = "zrcl4", from = "src" },
     { include = "zrcl3_uses", from = "src" },
@@ -16,14 +16,16 @@
 [build-system]
 requires = ["poetry-core"]
 build-backend = "poetry.core.masonry.api"
 
 [tool.poetry.group.dev.dependencies]
 black = ">=23.1,<25.0"
 
+keyring = "^25.2.1"
+moviepy = "^1.0.3"
 [tool.poetry.group.extra-dev.dependencies]
 pygetwindow = ">=0.0.9"
 readchar=">=4.0.6"
 pytest="8.2.0"
 click=">=8.1.7"
 toml = ">=0.10.2"
 easyocr = ">=1.7.1"
```

### Comparing `zrcl-0.3.0/README.md` & `zrcl-0.3.1/README.md`

 * *Files identical despite different names*

### Comparing `zrcl-0.3.0/src/zrcl3_uses/automation.py` & `zrcl-0.3.1/src/zrcl3_uses/automation.py`

 * *Files 4% similar despite different names*

```diff
@@ -10,27 +10,28 @@
 import screeninfo
 from zrcl4.pillow import load_base64_img
 from zrcl4.pygetwindow import activate_wnd, get_window_pos, refetch_wnd
 from zrcl4.pyscreeze import boxcenter
 from zrcl4.screeninfo import get_primary_monitor, wnd_on_monitor
 from pyscreeze import Box
 
+
 def img_reg(token: "AutoToken"):
     from zrcl4.pyscreeze import locate
 
     res = locate(
         token.sourceImg,
         token.targetImg,
         _algo=token.cfg_imgAlgo,
         confidence=token.confidence,
     )
 
     if isinstance(res, Box) or (isinstance(res, tuple) and len(res) == 4):
         return tuple(boxcenter(res))
-    
+
     return res
 
 
 def ocr(token: "AutoToken"):
     from zrcl4.easyocr import get_text_coordinates, EasyOCRMeta
 
     imagearr = numpy.array(token.targetImg)
@@ -72,14 +73,15 @@
         return None
 
     top_left = rect["top_left"]
     bottom_rght = rect["bottom_right"]
     # return as center point
     return (top_left[0] + bottom_rght[0]) / 2, (top_left[1] + bottom_rght[1]) / 2
 
+
 @dataclass
 class AutoToken:
     text: str = None
     image: typing.Union[Image.Image, str, numpy.ndarray] = None
 
     wnd: typing.Union[str, gw.Window] = None
     monitor: typing.Union[screeninfo.Monitor, int] = None
@@ -201,15 +203,15 @@
         match (self.wnd, self.monitor, self.region):
             case (None, None, None):
                 primary = get_primary_monitor()
                 return (primary.x, primary.y, primary.width, primary.height)
             case (wnd, _, None):
                 return get_window_pos(wnd)
             case (wnd, _, region) if self.regionIsRect:
-                base = get_window_pos(wnd) 
+                base = get_window_pos(wnd)
                 return (base[0] + region[0], base[1] + region[1], region[2], region[3])
             case (wnd, _, region) if not self.regionIsRect:
                 # treat as width and height in center
                 base = get_window_pos(wnd)
                 return (
                     base[0] + base[2] / 2 - region[0] / 2,
                     base[1] + base[3] / 2 - region[1] / 2,
@@ -252,62 +254,62 @@
         if self.wnd:
             activate_wnd(self.wnd)
 
         if self.text:
             res = self.ocrMethod(self)
         else:
             res = self.imgMethod(self)
-        
+
         if not res:
             return None
 
         # relative to interested region
         iregion = self.interestedRegion
         self.result = res
         curr_normalized = (res[0] + iregion[0], res[1] + iregion[1])
         if self.postProcessCallback:
             self.postProcessCallback(self, curr_normalized)
-        
+
         return curr_normalized
 
     def __call__(self, **kwds):
         return self._execute()
-    
+
     @property
     def normalizedResult(self):
         iregion = self.interestedRegion
         return (
             self.result[0] + iregion[0],
             self.result[1] + iregion[1],
         )
 
+
 @dataclass(init=False)
 class FrozenToken(AutoToken):
     def __init__(self, autoToken: AutoToken):
         if not autoToken.result:
             raise ValueError("result must be set")
-        d= asdict(autoToken)
+        d = asdict(autoToken)
         super().__init__(
             **d,
         )
         self.__inited__ = True
 
     def __setattr__(self, name: str, value) -> None:
         if not hasattr(self, "__inited__"):
             return super().__setattr__(name, value)
 
         if not hasattr(self, name):
             return super().__setattr__(name, value)
-        
+
         raise AttributeError(f"{self.__class__.__name__} is frozen")
 
     def __hash__(self):
         return hash(self.result)
-    
-    
+
 
 def waitFor(token: AutoToken, timeout: float = 10.0, interval: float = 1.1):
     currentTime = time.time()
     while time.time() - currentTime < timeout:
         try:
             if token():
                 break
@@ -316,12 +318,13 @@
 
         time.sleep(interval)
 
     if not token.result:
         raise TimeoutError("Timed out")
     return token.normalizedResult
 
+
 @contextmanager
 def repeatWith(token: AutoToken, times: int = 1):
     for _ in range(times):
         yield token()
     return token.normalizedResult
```

### Comparing `zrcl-0.3.0/src/zrcl3_uses/cli_selection.py` & `zrcl-0.3.1/src/zrcl3_uses/cli_selection.py`

 * *Files identical despite different names*

### Comparing `zrcl-0.3.0/src/zrcl3_uses/file.py` & `zrcl-0.3.1/src/zrcl3_uses/file.py`

 * *Files 0% similar despite different names*

```diff
@@ -152,12 +152,13 @@
                 callback = FilePropertyMeta.callBackHooks[callback]
             callback(
                 self.path, self._cachedContent[self.path], self._properties[self.path]
             )
 
         return self._cachedContent[self.path]
 
+
 # ANCHOR
 def startApp(path: str):
     import zrcl4.subprocess as subprocess
+
     subprocess.exec_command(path)
-
```

### Comparing `zrcl-0.3.0/src/zrcl3_uses/github.py` & `zrcl-0.3.1/src/zrcl3_uses/github.py`

 * *Files 2% similar despite different names*

```diff
@@ -81,16 +81,18 @@
     response = requests.get(url, headers=GITHUB_HEADERS)
     return response.json()
 
 
 def github_release_meta(
     repo: str,
     name: str = None,
-    match: typing.Literal["exact", "startswith", "contains", "endswith", "glob"] = "exact",
-    match_release_tag = False,
+    match: typing.Literal[
+        "exact", "startswith", "contains", "endswith", "glob"
+    ] = "exact",
+    match_release_tag=False,
 ):
     # Base URL for GitHub API
     base_url = f"https://api.github.com/repos/{repo}/releases"
 
     # Determine the URL to use based on whether a specific release tag is provided
     if name and match == "exact":
         url = f"{base_url}/tags/{name}"
@@ -117,15 +119,17 @@
     response.raise_for_status()  # Raises an HTTPError for bad responses
     return response.json()
 
 
 def download_release(
     releasejson: dict,
     filename: str = None,
-    match: typing.Literal["exact", "startswith", "contains", "endswith", "glob"] = "exact",
+    match: typing.Literal[
+        "exact", "startswith", "contains", "endswith", "glob"
+    ] = "exact",
     save: str = None,
 ):
     for asset in releasejson.get("assets", []):
         if match == "exact" and asset["name"] != filename:
             continue
         elif match == "startswith" and not asset["name"].startswith(filename):
             continue
@@ -135,22 +139,20 @@
             continue
         elif match == "glob" and re.match(filename, asset["name"]) is None:
             continue
 
         download_url = asset["browser_download_url"]
         # download using stream
         response = requests.get(download_url, stream=True)
-        response.raise_for_status() 
-        
+        response.raise_for_status()
+
         content = io.BytesIO()
 
         for block in response.iter_content(1024):
             content.write(block)
 
         if save:
             with open(save, "wb") as f:
                 f.write(content.getvalue())
             return
-        
+
         return content
-    
-
```

### Comparing `zrcl-0.3.0/src/zrcl3_uses/markdown.py` & `zrcl-0.3.1/src/zrcl3_uses/markdown.py`

 * *Files identical despite different names*

### Comparing `zrcl-0.3.0/src/zrcl3_uses/png_meta.py` & `zrcl-0.3.1/src/zrcl3_uses/png_meta.py`

 * *Files identical despite different names*

### Comparing `zrcl-0.3.0/src/zrcl3_uses/zip_crack.py` & `zrcl-0.3.1/src/zrcl3_uses/zip_crack.py`

 * *Files identical despite different names*

### Comparing `zrcl-0.3.0/src/zrcl4/__primitive__.py` & `zrcl-0.3.1/src/zrcl4/__primitive__.py`

 * *Files identical despite different names*

### Comparing `zrcl-0.3.0/src/zrcl4/cryptography.py` & `zrcl-0.3.1/src/zrcl4/cryptography.py`

 * *Files identical despite different names*

### Comparing `zrcl-0.3.0/src/zrcl4/easyocr.py` & `zrcl-0.3.1/src/zrcl4/easyocr.py`

 * *Files identical despite different names*

### Comparing `zrcl-0.3.0/src/zrcl4/hashlib.py` & `zrcl-0.3.1/src/zrcl4/hashlib.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,10 +1,12 @@
 import hashlib
 import io
 from typing import overload
+import os
+import typing
 
 
 @overload
 def hash_file(file: str, algorithm="sha256", chunk_size=4096): ...
 @overload
 def hash_file(file: io.IOBase, algorithm="sha256", chunk_size=4096): ...
 
@@ -21,7 +23,29 @@
         fileIo.close()
     return hash_algo.hexdigest()
 
 
 def hash_bytes(data, algorithm="sha256"):
     """Hash bytes with the specified algorithm."""
     return hashlib.new(algorithm, data).hexdigest()
+
+
+def hash_folder(
+    path: str,
+    allowed_extensions: typing.List[str] = None,
+    algorithm="sha256",
+    chunk_size=4096,
+):
+    """Hash all files in a folder with the specified algorithm and return a dictionary of file hashes."""
+    folder_hashes = {}
+    collective_hash = hashlib.new(algorithm)
+    for root, _, files in os.walk(path):
+        for file in files:
+            if allowed_extensions and not file.lower().endswith(
+                tuple(allowed_extensions)
+            ):
+                continue
+            file_path = os.path.join(root, file)
+            file_hash = hash_file(file_path, algorithm, chunk_size)
+            collective_hash.update(file_hash.encode("utf-8"))
+            folder_hashes[file_path] = file_hash
+    return folder_hashes, collective_hash.hexdigest()
```

### Comparing `zrcl-0.3.0/src/zrcl4/pygetwindow.py` & `zrcl-0.3.1/src/zrcl4/pygetwindow.py`

 * *Files 20% similar despite different names*

```diff
@@ -4,14 +4,16 @@
 import pygetwindow as gw
 import typing
 from .screeninfo import get_screen_dimensions
 
 
 def activate_wnd(wnd: gw.Window):
     try:
+        if wnd.isActive:
+            return
         wnd.activate()
     except gw.PyGetWindowException:
         pass
 
 
 def get_window_pos(wnd: gw.Window) -> typing.Tuple[float, float, float, float]:
     return (wnd.left, wnd.top, wnd.width, wnd.height)
@@ -59,44 +61,50 @@
         window_instance.moveTo(new_x, new_y)
 
         if index == row * col - 1:
             break
 
         sleep(sleepTime)
 
-def get_process_wnds(processname : str) -> typing.List[gw.Window]:
+
+def get_process_wnds(processname: str) -> typing.List[gw.Window]:
     if not platform.system() == "Windows":
         raise NotImplementedError
-    
+
     procs = []
     import psutil
+
     for proc in psutil.process_iter():
         if proc.name().startswith(processname):
             procs.append(proc)
 
     procIds = [proc.pid for proc in procs]
     import win32process
+
     wnds = []
     for wnd in gw.getAllWindows():
-        wnd : gw.Win32Window
+        wnd: gw.Win32Window
 
         _, winpid = win32process.GetWindowThreadProcessId(wnd._hWnd)
 
         if winpid in procIds:
             wnds.append(wnd)
     return wnds
 
-def get_visible_process_wnds(processname : str):
-    return [wnd for wnd in get_process_wnds(processname) if wnd.height > 0 and wnd.width > 0]
 
-def refetch_wnd(wnd : gw.Window) -> gw.Window:
+def get_visible_process_wnds(processname: str):
+    return [
+        wnd for wnd in get_process_wnds(processname) if wnd.height > 0 and wnd.width > 0
+    ]
+
+
+def refetch_wnd(wnd: gw.Window) -> gw.Window:
     candidates = gw.getWindowsWithTitle(wnd.title)
     if len(candidates) == 1:
         return candidates[0]
 
     for candidate in candidates:
         if platform.system() == "Windows":
             if candidate._hWnd == wnd._hWnd:
                 return candidate
         else:
-            return candidate        
-    
+            return candidate
```

### Comparing `zrcl-0.3.0/src/zrcl4/pyscreeze.py` & `zrcl-0.3.1/src/zrcl4/pyscreeze.py`

 * *Files identical despite different names*

### Comparing `zrcl-0.3.0/src/zrcl4/screeninfo.py` & `zrcl-0.3.1/src/zrcl4/screeninfo.py`

 * *Ordering differences only*

 * *Files 0% similar despite different names*

```diff
@@ -56,8 +56,8 @@
 
     wnd.move(coord[0], coord[1])
 
 
 def wnd_to_primary(wnd: gw.Window = None):
     if wnd is None:
         wnd = gw.getActiveWindow()
-    wnd_to_monitor(wnd, get_primary_monitor())
+    wnd_to_monitor(wnd, get_primary_monitor())
```

### Comparing `zrcl-0.3.0/src/zrcl4/subprocess.py` & `zrcl-0.3.1/src/zrcl4/subprocess.py`

 * *Files identical despite different names*

### Comparing `zrcl-0.3.0/src/zrcl4/time.py` & `zrcl-0.3.1/src/zrcl4/time.py`

 * *Files identical despite different names*

### Comparing `zrcl-0.3.0/src/zrcl4/typing.py` & `zrcl-0.3.1/src/zrcl4/typing.py`

 * *Files identical despite different names*

### Comparing `zrcl-0.3.0/PKG-INFO` & `zrcl-0.3.1/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: zrcl
-Version: 0.3.0
+Version: 0.3.1
 Summary: 
 License: MIT
 Author: ZackaryW
 Author-email: 36378555+ZackaryW@users.noreply.github.com
 Requires-Python: >=3.12,<4.0.0
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
```

