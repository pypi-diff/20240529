# Comparing `tmp/pyblu-0.3.6.tar.gz` & `tmp/pyblu-0.3.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pyblu-0.3.6.tar", max compression
+gzip compressed data, was "pyblu-0.3.7.tar", max compression
```

## Comparing `pyblu-0.3.6.tar` & `pyblu-0.3.7.tar`

### file list

```diff
@@ -1,8 +1,8 @@
--rw-r--r--   0        0        0     1069 2024-03-09 09:45:55.409568 pyblu-0.3.6/LICENSE
--rw-r--r--   0        0        0      873 2024-04-12 16:28:03.088001 pyblu-0.3.6/README.md
--rw-r--r--   0        0        0      921 2024-04-27 10:38:11.092700 pyblu-0.3.6/pyproject.toml
--rw-r--r--   0        0        0      277 2024-04-14 21:03:17.059292 pyblu-0.3.6/src/pyblu/__init__.py
--rw-r--r--   0        0        0     4605 2024-04-27 10:36:10.024239 pyblu-0.3.6/src/pyblu/_entities.py
--rw-r--r--   0        0        0     6109 2024-04-27 10:36:10.043239 pyblu-0.3.6/src/pyblu/_parse.py
--rw-r--r--   0        0        0    14367 2024-04-20 09:50:30.350831 pyblu-0.3.6/src/pyblu/_player.py
--rw-r--r--   0        0        0     1466 1970-01-01 00:00:00.000000 pyblu-0.3.6/PKG-INFO
+-rw-r--r--   0        0        0     1069 2024-03-09 09:45:55.409568 pyblu-0.3.7/LICENSE
+-rw-r--r--   0        0        0      873 2024-04-12 16:28:03.088001 pyblu-0.3.7/README.md
+-rw-r--r--   0        0        0      921 2024-04-27 10:57:36.359367 pyblu-0.3.7/pyproject.toml
+-rw-r--r--   0        0        0      277 2024-04-14 21:03:17.059292 pyblu-0.3.7/src/pyblu/__init__.py
+-rw-r--r--   0        0        0     4625 2024-04-27 10:40:06.923209 pyblu-0.3.7/src/pyblu/_entities.py
+-rw-r--r--   0        0        0     6109 2024-04-27 10:36:10.043239 pyblu-0.3.7/src/pyblu/_parse.py
+-rw-r--r--   0        0        0    14451 2024-04-27 10:57:08.006403 pyblu-0.3.7/src/pyblu/_player.py
+-rw-r--r--   0        0        0     1466 1970-01-01 00:00:00.000000 pyblu-0.3.7/PKG-INFO
```

### Comparing `pyblu-0.3.6/LICENSE` & `pyblu-0.3.7/LICENSE`

 * *Files identical despite different names*

### Comparing `pyblu-0.3.6/README.md` & `pyblu-0.3.7/README.md`

 * *Files identical despite different names*

### Comparing `pyblu-0.3.6/pyproject.toml` & `pyblu-0.3.7/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "pyblu"
-version = "0.3.6"
+version = "0.3.7"
 description = ""
 authors = ["Louis Christ <mail@louischrist.de>"]
 repository = "https://github.com/LouisChrist/pyblu"
 license = "MIT"
 readme = "README.md"
 packages = [
     { include = "pyblu", from = "src" },
```

### Comparing `pyblu-0.3.6/src/pyblu/_entities.py` & `pyblu-0.3.7/src/pyblu/_entities.py`

 * *Files 0% similar despite different names*

```diff
@@ -53,15 +53,15 @@
     """Volume level of the group. Only present on master. Range is 0-100."""
 
     indexing: bool
     """True if the player is currently indexing."""
 
     stream_url: str | None
     """The presence of this element should be treated as a flag and its contents as an opaque value. 
-    Seems to be present for radio stations and to be the same as the url from the matching preset."""
+    Seems to be present for radio stations and to be the same as the url from the matching preset(for Radio Stations)."""
 
 
 @dataclass
 class PairedPlayer:
     ip: str
     """IP address of the player"""
     port: int
```

### Comparing `pyblu-0.3.6/src/pyblu/_parse.py` & `pyblu-0.3.7/src/pyblu/_parse.py`

 * *Files identical despite different names*

### Comparing `pyblu-0.3.6/src/pyblu/_player.py` & `pyblu-0.3.7/src/pyblu/_player.py`

 * *Files 1% similar despite different names*

```diff
@@ -48,15 +48,15 @@
 
         :param etag: The last etag received from the server. Triggers long polling if set.
         :param timeout: The timeout in seconds for long polling.
 
         :return: The current status of the player. Only selected fields are returned.
         """
         params = {}
-        if etag:
+        if etag is not None:
             params["etag"] = etag
             params["timeout"] = timeout
         async with self._session.get(f"{self.base_url}/Status", params=params) as response:
             response.raise_for_status()
             response_data = await response.text()
             response_dict = xmltodict.parse(response_data)
 
@@ -72,15 +72,15 @@
 
         :param etag: The last etag received from the server. Triggers long polling if set.
         :param timeout: The timeout in seconds for long polling.
 
         :return: The SyncStatus of the player.
         """
         params = {}
-        if etag:
+        if etag is not None:
             params["etag"] = etag
             params["timeout"] = timeout
         async with self._session.get(f"{self.base_url}/SyncStatus", params=params) as response:
             response.raise_for_status()
             response_data = await response.text()
             response_dict = xmltodict.parse(response_data)
 
@@ -95,19 +95,19 @@
         :param level: The volume level to set. Range is 0-100.
         :param mute: Whether to mute the player.
         :param tell_slaves: Whether to tell grouped speakers to change their volume as well.
 
         :return: The current volume of the player.
         """
         params = {}
-        if level:
+        if level is not None:
             params["level"] = level
-        if mute:
+        if mute is not None:
             params["mute"] = "1" if mute else "0"
-        if tell_slaves:
+        if tell_slaves is not None:
             params["tell_slaves"] = "1" if tell_slaves else "0"
 
         async with self._session.get(f"{self.base_url}/Volume", params=params) as response:
             response.raise_for_status()
             response_data = await response.text()
             response_dict = xmltodict.parse(response_data)
 
@@ -120,15 +120,15 @@
         Works only when paused, not when stopped.
 
         :param seek: The position in seconds to seek to.
 
         :return: The playback state after command execution.
         """
         params = {}
-        if seek:
+        if seek is not None:
             params["seek"] = seek
 
         async with self._session.get(f"{self.base_url}/Play", params=params) as response:
             response.raise_for_status()
             response_data = await response.text()
             response_dict = xmltodict.parse(response_data)
 
@@ -155,15 +155,15 @@
         """Pause the current track. **toggle** can be used to toggle between playing and pause.
 
         :param toggle: Toggle between playing and pause.
 
         :return: The playback state after command execution.
         """
         params = {}
-        if toggle:
+        if toggle is not None:
             params["toggle"] = "1"
 
         async with self._session.get(f"{self.base_url}/Pause", params=params) as response:
             response.raise_for_status()
             response_data = await response.text()
             response_dict = xmltodict.parse(response_data)
```

### Comparing `pyblu-0.3.6/PKG-INFO` & `pyblu-0.3.7/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pyblu
-Version: 0.3.6
+Version: 0.3.7
 Summary: 
 Home-page: https://github.com/LouisChrist/pyblu
 License: MIT
 Author: Louis Christ
 Author-email: mail@louischrist.de
 Requires-Python: >=3.11,<4.0
 Classifier: License :: OSI Approved :: MIT License
```

