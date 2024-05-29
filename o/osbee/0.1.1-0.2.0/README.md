# Comparing `tmp/osbee-0.1.1.tar.gz` & `tmp/osbee-0.2.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "osbee-0.1.1.tar", last modified: Mon May 27 06:15:39 2024, max compression
+gzip compressed data, was "osbee-0.2.0.tar", last modified: Wed May 29 08:01:24 2024, max compression
```

## Comparing `osbee-0.1.1.tar` & `osbee-0.2.0.tar`

### file list

```diff
@@ -1,16 +1,16 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-27 06:15:39.698674 osbee-0.1.1/
--rw-r--r--   0 runner    (1001) docker     (127)     1068 2024-05-27 06:15:27.000000 osbee-0.1.1/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)     1992 2024-05-27 06:15:39.698674 osbee-0.1.1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      227 2024-05-27 06:15:27.000000 osbee-0.1.1/README.md
--rw-r--r--   0 runner    (1001) docker     (127)      713 2024-05-27 06:15:27.000000 osbee-0.1.1/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-27 06:15:39.698674 osbee-0.1.1/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-27 06:15:39.694674 osbee-0.1.1/src/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-27 06:15:39.698674 osbee-0.1.1/src/osbee/
--rw-r--r--   0 runner    (1001) docker     (127)       65 2024-05-27 06:15:27.000000 osbee-0.1.1/src/osbee/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     7348 2024-05-27 06:15:27.000000 osbee-0.1.1/src/osbee/osbee.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-27 06:15:39.698674 osbee-0.1.1/src/osbee.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     1992 2024-05-27 06:15:39.000000 osbee-0.1.1/src/osbee.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      237 2024-05-27 06:15:39.000000 osbee-0.1.1/src/osbee.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-27 06:15:39.000000 osbee-0.1.1/src/osbee.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       13 2024-05-27 06:15:39.000000 osbee-0.1.1/src/osbee.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)        6 2024-05-27 06:15:39.000000 osbee-0.1.1/src/osbee.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-29 08:01:24.116773 osbee-0.2.0/
+-rw-r--r--   0 runner    (1001) docker     (127)     1068 2024-05-29 08:01:20.000000 osbee-0.2.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)     3182 2024-05-29 08:01:24.116773 osbee-0.2.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     1372 2024-05-29 08:01:20.000000 osbee-0.2.0/README.md
+-rw-r--r--   0 runner    (1001) docker     (127)      734 2024-05-29 08:01:20.000000 osbee-0.2.0/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-29 08:01:24.116773 osbee-0.2.0/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-29 08:01:24.112774 osbee-0.2.0/src/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-29 08:01:24.112774 osbee-0.2.0/src/osbee/
+-rw-r--r--   0 runner    (1001) docker     (127)       94 2024-05-29 08:01:20.000000 osbee-0.2.0/src/osbee/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7846 2024-05-29 08:01:20.000000 osbee-0.2.0/src/osbee/osbee.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-29 08:01:24.116773 osbee-0.2.0/src/osbee.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     3182 2024-05-29 08:01:24.000000 osbee-0.2.0/src/osbee.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      237 2024-05-29 08:01:24.000000 osbee-0.2.0/src/osbee.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-29 08:01:24.000000 osbee-0.2.0/src/osbee.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       28 2024-05-29 08:01:24.000000 osbee-0.2.0/src/osbee.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        6 2024-05-29 08:01:24.000000 osbee-0.2.0/src/osbee.egg-info/top_level.txt
```

### Comparing `osbee-0.1.1/LICENSE` & `osbee-0.2.0/LICENSE`

 * *Files identical despite different names*

### Comparing `osbee-0.1.1/pyproject.toml` & `osbee-0.2.0/pyproject.toml`

 * *Files 25% similar despite different names*

```diff
@@ -1,26 +1,26 @@
 [build-system]
 requires      = ["setuptools", "wheel"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "osbee"
-version = "0.1.1"
+version = "0.2.0"
 description = "Connect to your OSBee 3-valve controller's REST API"
 readme = "README.md"
 authors = [{ name = "Allan Clark", email = "allanc@chickenandpork.com" }]
 license = { file = "LICENSE" }
 classifiers = [
     "License :: OSI Approved :: MIT License",
     "Programming Language :: Python",
     "Programming Language :: Python :: 3",
 ]
 keywords = ["osbee", "opensprinkler"]
 # yup, pure bog-standard python
-dependencies = []
+dependencies = [ "aiohttp", "typing" ]
 #requires-python = ">=3.9"
 
 [project.optional-dependencies]
 dev = [ "black" ]
 
 [project.urls]
 Homepage = "https://github.com/chickenandpork/osbee"
```

### Comparing `osbee-0.1.1/src/osbee/osbee.py` & `osbee-0.2.0/src/osbee/osbee.py`

 * *Files 12% similar despite different names*

```diff
@@ -5,21 +5,28 @@
 
 https://github.com/OpenSprinkler/OSBeeWiFi-Firmware/blob/master/docs/firmware1.0.0/OSBeeAPI1.0.0.pdf
 """
 
 import aiohttp
 import logging
 from threading import Lock
+from typing import Awaitable, Callable, Optional, Dict, Any
 
 _LOGGER = logging.getLogger(__name__)
 
 
 class OSBeeAPI:
     """aiohttp facade for API requests to OSB Hub device."""
 
+    _host: str
+    _jc_cache: Optional[Dict[str, Any]]
+    _max_runtime: int
+    _session: aiohttp.ClientSession
+    _token: str
+
     def __init__(
         self, host: str, max_runtime: int, token: str, session: aiohttp.ClientSession
     ) -> None:
         """Create an OSBeeAPI by offering a host, and an async session to get there."""
         self._host = host
         self._jc_cache = None
         _LOGGER.warning("type of timeout/max_runtime is %s", type(max_runtime))
@@ -30,15 +37,15 @@
         _LOGGER.warning(
             "created OSBeeAPI at %s max_runtime %s (%s)",
             self._host,
             self._max_runtime,
             type(self._max_runtime),
         )
 
-    async def fetch_data(self, index):
+    async def fetch_data(self, index) -> str:
         """Get raw device state from the OSBee Hub via API.  No authentication yet considered.
 
         Essentially,the unprotected result of hitting your OSBee with GET http://{IP}/jc with a
         text/json content-type (OSBee-1.0.0; firmware-1.0.2 seems to offer application.json) and
         contains the status of the device.
         """
 
@@ -60,24 +67,24 @@
                 )
 
             if jc_request.status != 200:
                 raise Exception(  # pylint: disable=broad-exception-raised
                     f"Error connecting to OSBee Hub (HTTP/{jc_request.status or 'None'})"
                 )
 
-            jc_body = await jc_request.json(content_type="text/html")
+            jc_body = await jc_request.json(content_type=None)
             if len(jc_body) == 0:
                 raise Exception(  # pylint: disable=broad-exception-raised
                     "The server returned a zero-length body, not a valid response"
                 )
 
             self._jc_cache = jc_body
             return jc_body  # the resulting structure has no conventional "data" element, just raw JSON
 
-    async def async_turn_off(self, zone_id):
+    async def async_turn_off(self, zone_id) -> str:
         """Async entry point to deactivate the valve/relay for the zone.
 
         Based on the current status of the device, this method creates a new determination of
         active valves as bit-fields, and pushes the new list of active valves as a new manual
         program running those valves, replacing the current manual program.  This has the effect of
         turning off the given valve.
         """
@@ -92,15 +99,15 @@
                 _LOGGER.debug("In turn_off: current state is %s", current)
                 mask = 1 << zone_id
                 self._jc_cache["zbits"] = current & ~mask
             _LOGGER.debug("In turn_off: new state is %s", self._jc_cache["zbits"])
 
         return await self.async_apply_state()
 
-    async def async_turn_on(self, zone_id):
+    async def async_turn_on(self, zone_id) -> str:
         """Async entry point to activate the valve/relay for the zone.
 
         Based on the current status of the device, this method creates a new determination of
         active valves as bit-fields, and pushes the new list of active valves as a new manual
         program running those valves, replacing the current manual program.  This has the effect of
         turning off the given valve.
         """
@@ -115,33 +122,40 @@
                 _LOGGER.debug("In turn_on: current state is %s", current)
                 mask = 1 << zone_id
                 self._jc_cache["zbits"] = current | mask
             _LOGGER.debug("In turn_on: new state is %s", self._jc_cache["zbits"])
 
         return await self.async_apply_state()
 
-    async def async_apply_state(self):
+    async def async_apply_state(self) -> str:
         """Async entry point to set active zones.
 
         Mostly used internally by async_turn_off(...), async_turn_on(...), this method applies the
         desired state by generating the GET http://{IP}/cc to shut off all valves, or
         http://{IP}/rp to run a manual program of the given valves.
         """
 
+        # type-shuffle: assign a non-optional dict to satisfy type-hint
+        if self._jc_cache:
+            new_bitz: int = self._jc_cache["zbits"]  # bits: which valves are open
+        else:
+            raise Exception(  # pylint: disable=broad-exception-raised
+                "INTERNAL: async_apply_state is supposed to be gated from _jc_cache==None"
+            )
+
         # firmware-1.0.0, part 11: Run Program (rp): http://devip/rp?dkey=xxx&pid=x&...
         # ...
         # When pid=77 (ASCII value of 'M'), this command starts a manual program.  You will need to supply two additional parameters:
         #  - zbits=x: zone enable bits (e.g. zbits=4 means zone 3 will turn on)
         #  - dur=x: duration (in seconds)
         #  - Example: pid=77&zbits=3&dur=300 turns on zones 1 and 2 manually for 5 minutes
 
-        if self._jc_cache["zbits"] == 0:  # on zbits==0, we need to actually reset
+        if new_bitz == 0:  # on zbits==0, we need to actually reset
             url = f"http://{self._host}/cc?dkey={self._token}&reset=1"
         else:
-            new_bitz = self._jc_cache["zbits"]  # avoid triple-quoting
             url = f"http://{self._host}/rp?dkey={self._token}&pid=77&zbits={new_bitz}&dur={self._max_runtime}"
 
         async with self._session.get(url) as rp_request:
             if rp_request.status == 401:
                 raise AuthenticationError(
                     "Unable to authenticate with the OSBee API (HTTP/401)"
                 )
```

