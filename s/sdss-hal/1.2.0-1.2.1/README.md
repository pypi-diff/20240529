# Comparing `tmp/sdss_hal-1.2.0.tar.gz` & `tmp/sdss_hal-1.2.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "sdss_hal-1.2.0.tar", max compression
+gzip compressed data, was "sdss_hal-1.2.1.tar", max compression
```

## Comparing `sdss_hal-1.2.0.tar` & `sdss_hal-1.2.1.tar`

### file list

```diff
@@ -1,46 +1,46 @@
--rw-r--r--   0        0        0     1504 2024-05-26 20:09:52.901536 sdss_hal-1.2.0/LICENSE.md
--rw-r--r--   0        0        0      816 2024-05-26 20:09:52.901536 sdss_hal-1.2.0/README.md
--rw-r--r--   0        0        0     2708 2024-05-26 20:09:52.905536 sdss_hal-1.2.0/pyproject.toml
--rw-r--r--   0        0        0      483 2024-05-26 20:09:52.905536 sdss_hal-1.2.0/src/hal/__init__.py
--rw-r--r--   0        0        0     1761 2024-05-26 20:09:52.905536 sdss_hal-1.2.0/src/hal/__main__.py
--rw-r--r--   0        0        0      356 2024-05-26 20:09:52.905536 sdss_hal-1.2.0/src/hal/actor/__init__.py
--rw-r--r--   0        0        0     3024 2024-05-26 20:09:52.905536 sdss_hal-1.2.0/src/hal/actor/actor.py
--rw-r--r--   0        0        0     3326 2024-05-26 20:09:52.905536 sdss_hal-1.2.0/src/hal/actor/commands/__init__.py
--rw-r--r--   0        0        0     3940 2024-05-26 20:09:52.905536 sdss_hal-1.2.0/src/hal/actor/commands/auto_pilot.py
--rw-r--r--   0        0        0     1593 2024-05-26 20:09:52.905536 sdss_hal-1.2.0/src/hal/actor/commands/bypass.py
--rw-r--r--   0        0        0      844 2024-05-26 20:09:52.905536 sdss_hal-1.2.0/src/hal/actor/commands/calibrations.py
--rw-r--r--   0        0        0     8082 2024-05-26 20:09:52.905536 sdss_hal-1.2.0/src/hal/actor/commands/expose.py
--rw-r--r--   0        0        0     1669 2024-05-26 20:09:52.905536 sdss_hal-1.2.0/src/hal/actor/commands/goto.py
--rw-r--r--   0        0        0     3498 2024-05-26 20:09:52.905536 sdss_hal-1.2.0/src/hal/actor/commands/goto_field.py
--rw-r--r--   0        0        0     2537 2024-05-26 20:09:52.905536 sdss_hal-1.2.0/src/hal/actor/commands/script.py
--rw-r--r--   0        0        0     1419 2024-05-26 20:09:52.905536 sdss_hal-1.2.0/src/hal/actor/commands/status.py
--rw-r--r--   0        0        0      687 2024-05-26 20:09:52.905536 sdss_hal-1.2.0/src/hal/actor/commands/test.py
--rw-r--r--   0        0        0     3362 2024-05-26 20:09:52.905536 sdss_hal-1.2.0/src/hal/etc/hal.yml
--rw-r--r--   0        0        0     2190 2024-05-26 20:09:52.905536 sdss_hal-1.2.0/src/hal/etc/schema.json
--rw-r--r--   0        0        0      346 2024-05-26 20:09:52.905536 sdss_hal-1.2.0/src/hal/etc/scripts/apo/cartchange.inp
--rw-r--r--   0        0        0     1161 2024-05-26 20:09:52.905536 sdss_hal-1.2.0/src/hal/etc/scripts/apo/eveningcals.inp
--rw-r--r--   0        0        0      161 2024-05-26 20:09:52.905536 sdss_hal-1.2.0/src/hal/etc/scripts/apo/example.inp
--rw-r--r--   0        0        0     1616 2024-05-26 20:09:52.905536 sdss_hal-1.2.0/src/hal/etc/scripts/apo/morningcals.inp
--rw-r--r--   0        0        0       35 2024-05-26 20:09:52.905536 sdss_hal-1.2.0/src/hal/etc/scripts/apo/test.inp
--rw-r--r--   0        0        0      346 2024-05-26 20:09:52.905536 sdss_hal-1.2.0/src/hal/etc/scripts/lco/cartchange.inp
--rw-r--r--   0        0        0     1056 2024-05-26 20:09:52.905536 sdss_hal-1.2.0/src/hal/etc/scripts/lco/eveningcals.inp
--rw-r--r--   0        0        0     1450 2024-05-26 20:09:52.905536 sdss_hal-1.2.0/src/hal/etc/scripts/lco/morningcals.inp
--rw-r--r--   0        0        0     1180 2024-05-26 20:09:52.905536 sdss_hal-1.2.0/src/hal/exceptions.py
--rw-r--r--   0        0        0     3502 2024-05-26 20:09:52.905536 sdss_hal-1.2.0/src/hal/helpers/__init__.py
--rw-r--r--   0        0        0    10610 2024-05-26 20:09:52.905536 sdss_hal-1.2.0/src/hal/helpers/apogee.py
--rw-r--r--   0        0        0     7101 2024-05-26 20:09:52.905536 sdss_hal-1.2.0/src/hal/helpers/boss.py
--rw-r--r--   0        0        0     6514 2024-05-26 20:09:52.905536 sdss_hal-1.2.0/src/hal/helpers/cherno.py
--rw-r--r--   0        0        0     1769 2024-05-26 20:09:52.905536 sdss_hal-1.2.0/src/hal/helpers/ffs.py
--rw-r--r--   0        0        0     8270 2024-05-26 20:09:52.905536 sdss_hal-1.2.0/src/hal/helpers/jaeger.py
--rw-r--r--   0        0        0    10429 2024-05-26 20:09:52.905536 sdss_hal-1.2.0/src/hal/helpers/lamps.py
--rw-r--r--   0        0        0     4732 2024-05-26 20:09:52.905536 sdss_hal-1.2.0/src/hal/helpers/overhead.py
--rw-r--r--   0        0        0     4671 2024-05-26 20:09:52.905536 sdss_hal-1.2.0/src/hal/helpers/scripts.py
--rw-r--r--   0        0        0    13441 2024-05-26 20:09:52.905536 sdss_hal-1.2.0/src/hal/helpers/tcc.py
--rw-r--r--   0        0        0     1399 2024-05-26 20:09:52.905536 sdss_hal-1.2.0/src/hal/macros/__init__.py
--rw-r--r--   0        0        0     3844 2024-05-26 20:09:52.905536 sdss_hal-1.2.0/src/hal/macros/apogee_dome_flat.py
--rw-r--r--   0        0        0    12278 2024-05-26 20:09:52.905536 sdss_hal-1.2.0/src/hal/macros/auto_pilot.py
--rw-r--r--   0        0        0    21544 2024-05-26 20:09:52.905536 sdss_hal-1.2.0/src/hal/macros/expose.py
--rw-r--r--   0        0        0    23929 2024-05-26 20:09:52.905536 sdss_hal-1.2.0/src/hal/macros/goto_field.py
--rw-r--r--   0        0        0    18881 2024-05-26 20:09:52.905536 sdss_hal-1.2.0/src/hal/macros/macro.py
--rw-r--r--   0        0        0     1263 2024-05-26 20:09:52.905536 sdss_hal-1.2.0/src/hal/macros/test_macro.py
--rw-r--r--   0        0        0     2219 1970-01-01 00:00:00.000000 sdss_hal-1.2.0/PKG-INFO
+-rw-r--r--   0        0        0     1504 2024-05-28 23:23:59.051606 sdss_hal-1.2.1/LICENSE.md
+-rw-r--r--   0        0        0      816 2024-05-28 23:23:59.051606 sdss_hal-1.2.1/README.md
+-rw-r--r--   0        0        0     2708 2024-05-28 23:23:59.059606 sdss_hal-1.2.1/pyproject.toml
+-rw-r--r--   0        0        0      483 2024-05-28 23:23:59.059606 sdss_hal-1.2.1/src/hal/__init__.py
+-rw-r--r--   0        0        0     1761 2024-05-28 23:23:59.059606 sdss_hal-1.2.1/src/hal/__main__.py
+-rw-r--r--   0        0        0      356 2024-05-28 23:23:59.059606 sdss_hal-1.2.1/src/hal/actor/__init__.py
+-rw-r--r--   0        0        0     3024 2024-05-28 23:23:59.059606 sdss_hal-1.2.1/src/hal/actor/actor.py
+-rw-r--r--   0        0        0     3326 2024-05-28 23:23:59.059606 sdss_hal-1.2.1/src/hal/actor/commands/__init__.py
+-rw-r--r--   0        0        0     3953 2024-05-28 23:23:59.059606 sdss_hal-1.2.1/src/hal/actor/commands/auto_pilot.py
+-rw-r--r--   0        0        0     1593 2024-05-28 23:23:59.059606 sdss_hal-1.2.1/src/hal/actor/commands/bypass.py
+-rw-r--r--   0        0        0      844 2024-05-28 23:23:59.059606 sdss_hal-1.2.1/src/hal/actor/commands/calibrations.py
+-rw-r--r--   0        0        0     8082 2024-05-28 23:23:59.059606 sdss_hal-1.2.1/src/hal/actor/commands/expose.py
+-rw-r--r--   0        0        0     1669 2024-05-28 23:23:59.059606 sdss_hal-1.2.1/src/hal/actor/commands/goto.py
+-rw-r--r--   0        0        0     3498 2024-05-28 23:23:59.059606 sdss_hal-1.2.1/src/hal/actor/commands/goto_field.py
+-rw-r--r--   0        0        0     2537 2024-05-28 23:23:59.059606 sdss_hal-1.2.1/src/hal/actor/commands/script.py
+-rw-r--r--   0        0        0     1419 2024-05-28 23:23:59.059606 sdss_hal-1.2.1/src/hal/actor/commands/status.py
+-rw-r--r--   0        0        0      687 2024-05-28 23:23:59.059606 sdss_hal-1.2.1/src/hal/actor/commands/test.py
+-rw-r--r--   0        0        0     3362 2024-05-28 23:23:59.059606 sdss_hal-1.2.1/src/hal/etc/hal.yml
+-rw-r--r--   0        0        0     2190 2024-05-28 23:23:59.059606 sdss_hal-1.2.1/src/hal/etc/schema.json
+-rw-r--r--   0        0        0      346 2024-05-28 23:23:59.059606 sdss_hal-1.2.1/src/hal/etc/scripts/apo/cartchange.inp
+-rw-r--r--   0        0        0     1161 2024-05-28 23:23:59.059606 sdss_hal-1.2.1/src/hal/etc/scripts/apo/eveningcals.inp
+-rw-r--r--   0        0        0      161 2024-05-28 23:23:59.059606 sdss_hal-1.2.1/src/hal/etc/scripts/apo/example.inp
+-rw-r--r--   0        0        0     1616 2024-05-28 23:23:59.059606 sdss_hal-1.2.1/src/hal/etc/scripts/apo/morningcals.inp
+-rw-r--r--   0        0        0       35 2024-05-28 23:23:59.059606 sdss_hal-1.2.1/src/hal/etc/scripts/apo/test.inp
+-rw-r--r--   0        0        0      346 2024-05-28 23:23:59.059606 sdss_hal-1.2.1/src/hal/etc/scripts/lco/cartchange.inp
+-rw-r--r--   0        0        0     1056 2024-05-28 23:23:59.059606 sdss_hal-1.2.1/src/hal/etc/scripts/lco/eveningcals.inp
+-rw-r--r--   0        0        0     1450 2024-05-28 23:23:59.059606 sdss_hal-1.2.1/src/hal/etc/scripts/lco/morningcals.inp
+-rw-r--r--   0        0        0     1180 2024-05-28 23:23:59.059606 sdss_hal-1.2.1/src/hal/exceptions.py
+-rw-r--r--   0        0        0     3502 2024-05-28 23:23:59.059606 sdss_hal-1.2.1/src/hal/helpers/__init__.py
+-rw-r--r--   0        0        0    10610 2024-05-28 23:23:59.059606 sdss_hal-1.2.1/src/hal/helpers/apogee.py
+-rw-r--r--   0        0        0     7101 2024-05-28 23:23:59.059606 sdss_hal-1.2.1/src/hal/helpers/boss.py
+-rw-r--r--   0        0        0     6514 2024-05-28 23:23:59.059606 sdss_hal-1.2.1/src/hal/helpers/cherno.py
+-rw-r--r--   0        0        0     1769 2024-05-28 23:23:59.059606 sdss_hal-1.2.1/src/hal/helpers/ffs.py
+-rw-r--r--   0        0        0     8270 2024-05-28 23:23:59.059606 sdss_hal-1.2.1/src/hal/helpers/jaeger.py
+-rw-r--r--   0        0        0    10429 2024-05-28 23:23:59.059606 sdss_hal-1.2.1/src/hal/helpers/lamps.py
+-rw-r--r--   0        0        0     4732 2024-05-28 23:23:59.059606 sdss_hal-1.2.1/src/hal/helpers/overhead.py
+-rw-r--r--   0        0        0     4671 2024-05-28 23:23:59.059606 sdss_hal-1.2.1/src/hal/helpers/scripts.py
+-rw-r--r--   0        0        0    13441 2024-05-28 23:23:59.059606 sdss_hal-1.2.1/src/hal/helpers/tcc.py
+-rw-r--r--   0        0        0     1399 2024-05-28 23:23:59.059606 sdss_hal-1.2.1/src/hal/macros/__init__.py
+-rw-r--r--   0        0        0     3844 2024-05-28 23:23:59.059606 sdss_hal-1.2.1/src/hal/macros/apogee_dome_flat.py
+-rw-r--r--   0        0        0    12441 2024-05-28 23:23:59.059606 sdss_hal-1.2.1/src/hal/macros/auto_pilot.py
+-rw-r--r--   0        0        0    21726 2024-05-28 23:23:59.059606 sdss_hal-1.2.1/src/hal/macros/expose.py
+-rw-r--r--   0        0        0    23929 2024-05-28 23:23:59.059606 sdss_hal-1.2.1/src/hal/macros/goto_field.py
+-rw-r--r--   0        0        0    18881 2024-05-28 23:23:59.059606 sdss_hal-1.2.1/src/hal/macros/macro.py
+-rw-r--r--   0        0        0     1263 2024-05-28 23:23:59.059606 sdss_hal-1.2.1/src/hal/macros/test_macro.py
+-rw-r--r--   0        0        0     2219 1970-01-01 00:00:00.000000 sdss_hal-1.2.1/PKG-INFO
```

### Comparing `sdss_hal-1.2.0/LICENSE.md` & `sdss_hal-1.2.1/LICENSE.md`

 * *Files identical despite different names*

### Comparing `sdss_hal-1.2.0/README.md` & `sdss_hal-1.2.1/README.md`

 * *Files identical despite different names*

### Comparing `sdss_hal-1.2.0/pyproject.toml` & `sdss_hal-1.2.1/pyproject.toml`

 * *Files 5% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "sdss-hal"
-version = "1.2.0"
+version = "1.2.1"
 description = "High-level observing tool for SDSS-V (replaces SOP)"
 authors = ["José Sánchez-Gallego <gallegoj@uw.edu>"]
 license = "BSD-3-Clause"
 readme = "README.md"
 homepage = "https://github.com/sdss/hal"
 repository = "https://github.com/sdss/hal"
 documentation = "https://sdss-hal.readthedocs.org"
```

### Comparing `sdss_hal-1.2.0/src/hal/__main__.py` & `sdss_hal-1.2.1/src/hal/__main__.py`

 * *Files identical despite different names*

### Comparing `sdss_hal-1.2.0/src/hal/actor/actor.py` & `sdss_hal-1.2.1/src/hal/actor/actor.py`

 * *Files identical despite different names*

### Comparing `sdss_hal-1.2.0/src/hal/actor/commands/__init__.py` & `sdss_hal-1.2.1/src/hal/actor/commands/__init__.py`

 * *Files identical despite different names*

### Comparing `sdss_hal-1.2.0/src/hal/actor/commands/auto_pilot.py` & `sdss_hal-1.2.1/src/hal/actor/commands/auto_pilot.py`

 * *Files 1% similar despite different names*

```diff
@@ -139,15 +139,15 @@
 
         # Run the auto loop until the command is cancelled.
         if not await macro.run():
             result = False
             break
 
         await asyncio.sleep(0.1)
-
+        break
         if macro.cancelled:
             # Cancelled macros return result=True
             break
 
     if result is False:
         return command.fail()
```

### Comparing `sdss_hal-1.2.0/src/hal/actor/commands/bypass.py` & `sdss_hal-1.2.1/src/hal/actor/commands/bypass.py`

 * *Files identical despite different names*

### Comparing `sdss_hal-1.2.0/src/hal/actor/commands/calibrations.py` & `sdss_hal-1.2.1/src/hal/actor/commands/calibrations.py`

 * *Files identical despite different names*

### Comparing `sdss_hal-1.2.0/src/hal/actor/commands/expose.py` & `sdss_hal-1.2.1/src/hal/actor/commands/expose.py`

 * *Files identical despite different names*

### Comparing `sdss_hal-1.2.0/src/hal/actor/commands/goto.py` & `sdss_hal-1.2.1/src/hal/actor/commands/goto.py`

 * *Files identical despite different names*

### Comparing `sdss_hal-1.2.0/src/hal/actor/commands/goto_field.py` & `sdss_hal-1.2.1/src/hal/actor/commands/goto_field.py`

 * *Files identical despite different names*

### Comparing `sdss_hal-1.2.0/src/hal/actor/commands/script.py` & `sdss_hal-1.2.1/src/hal/actor/commands/script.py`

 * *Files identical despite different names*

### Comparing `sdss_hal-1.2.0/src/hal/actor/commands/status.py` & `sdss_hal-1.2.1/src/hal/actor/commands/status.py`

 * *Files identical despite different names*

### Comparing `sdss_hal-1.2.0/src/hal/actor/commands/test.py` & `sdss_hal-1.2.1/src/hal/actor/commands/test.py`

 * *Files identical despite different names*

### Comparing `sdss_hal-1.2.0/src/hal/etc/hal.yml` & `sdss_hal-1.2.1/src/hal/etc/hal.yml`

 * *Files identical despite different names*

### Comparing `sdss_hal-1.2.0/src/hal/etc/schema.json` & `sdss_hal-1.2.1/src/hal/etc/schema.json`

 * *Files identical despite different names*

### Comparing `sdss_hal-1.2.0/src/hal/etc/scripts/apo/eveningcals.inp` & `sdss_hal-1.2.1/src/hal/etc/scripts/apo/eveningcals.inp`

 * *Files identical despite different names*

### Comparing `sdss_hal-1.2.0/src/hal/etc/scripts/apo/morningcals.inp` & `sdss_hal-1.2.1/src/hal/etc/scripts/apo/morningcals.inp`

 * *Files identical despite different names*

### Comparing `sdss_hal-1.2.0/src/hal/etc/scripts/lco/eveningcals.inp` & `sdss_hal-1.2.1/src/hal/etc/scripts/lco/eveningcals.inp`

 * *Files identical despite different names*

### Comparing `sdss_hal-1.2.0/src/hal/etc/scripts/lco/morningcals.inp` & `sdss_hal-1.2.1/src/hal/etc/scripts/lco/morningcals.inp`

 * *Files identical despite different names*

### Comparing `sdss_hal-1.2.0/src/hal/exceptions.py` & `sdss_hal-1.2.1/src/hal/exceptions.py`

 * *Files identical despite different names*

### Comparing `sdss_hal-1.2.0/src/hal/helpers/__init__.py` & `sdss_hal-1.2.1/src/hal/helpers/__init__.py`

 * *Files identical despite different names*

### Comparing `sdss_hal-1.2.0/src/hal/helpers/apogee.py` & `sdss_hal-1.2.1/src/hal/helpers/apogee.py`

 * *Files identical despite different names*

### Comparing `sdss_hal-1.2.0/src/hal/helpers/boss.py` & `sdss_hal-1.2.1/src/hal/helpers/boss.py`

 * *Files identical despite different names*

### Comparing `sdss_hal-1.2.0/src/hal/helpers/cherno.py` & `sdss_hal-1.2.1/src/hal/helpers/cherno.py`

 * *Files identical despite different names*

### Comparing `sdss_hal-1.2.0/src/hal/helpers/ffs.py` & `sdss_hal-1.2.1/src/hal/helpers/ffs.py`

 * *Files identical despite different names*

### Comparing `sdss_hal-1.2.0/src/hal/helpers/jaeger.py` & `sdss_hal-1.2.1/src/hal/helpers/jaeger.py`

 * *Files identical despite different names*

### Comparing `sdss_hal-1.2.0/src/hal/helpers/lamps.py` & `sdss_hal-1.2.1/src/hal/helpers/lamps.py`

 * *Files identical despite different names*

### Comparing `sdss_hal-1.2.0/src/hal/helpers/overhead.py` & `sdss_hal-1.2.1/src/hal/helpers/overhead.py`

 * *Files identical despite different names*

### Comparing `sdss_hal-1.2.0/src/hal/helpers/scripts.py` & `sdss_hal-1.2.1/src/hal/helpers/scripts.py`

 * *Files identical despite different names*

### Comparing `sdss_hal-1.2.0/src/hal/helpers/tcc.py` & `sdss_hal-1.2.1/src/hal/helpers/tcc.py`

 * *Files identical despite different names*

### Comparing `sdss_hal-1.2.0/src/hal/macros/__init__.py` & `sdss_hal-1.2.1/src/hal/macros/__init__.py`

 * *Files identical despite different names*

### Comparing `sdss_hal-1.2.0/src/hal/macros/apogee_dome_flat.py` & `sdss_hal-1.2.1/src/hal/macros/apogee_dome_flat.py`

 * *Files identical despite different names*

### Comparing `sdss_hal-1.2.0/src/hal/macros/auto_pilot.py` & `sdss_hal-1.2.1/src/hal/macros/auto_pilot.py`

 * *Files 2% similar despite different names*

```diff
@@ -103,18 +103,21 @@
 
         # If we don't know about the spec states, fail.
         if self.system_state.apogee_exposure_state is None:
             raise MacroError("Cannot determine APOGEE exposure state.")
         if self.system_state.boss_exposure_state is None:
             raise MacroError("Cannot determine BOSS exposure state.")
 
-        time_remaining = self.system_state.exposure_time_remaining
-        if time_remaining > 0:
+        # Is there a configuration loaded and has it been observed?
+        configuration = self.helpers.jaeger.configuration
+        observed = configuration and configuration.observed
+
+        if self.system_state.exposure_time_remaining > 0:
             # We are exposing.
-            if self.helpers.jaeger.preloaded:
+            if self.helpers.jaeger.preloaded or not observed:
                 # There is already a preloaded configuration. Just wait
                 # until the exposure is done.
                 self._auto_pilot_message("Waiting for exposure before loading design")
 
             else:
                 # We need to preload a design.
                 await self._preload_design()
```

### Comparing `sdss_hal-1.2.0/src/hal/macros/expose.py` & `sdss_hal-1.2.1/src/hal/macros/expose.py`

 * *Files 1% similar despite different names*

```diff
@@ -11,21 +11,27 @@
 
 import asyncio
 import os
 from contextlib import suppress
 from dataclasses import dataclass
 from time import time
 
+from typing import TYPE_CHECKING
+
 import numpy
 
 from hal import config
 from hal.exceptions import MacroError
 from hal.macros import Macro
 
 
+if TYPE_CHECKING:
+    from hal.helpers.jaeger import Configuration
+
+
 __all__ = ["ExposeMacro"]
 
 
 @dataclass
 class ExposeParameters:
     """Expose macro parameters."""
 
@@ -426,14 +432,19 @@
     __PRECONDITIONS__ = ["prepare"]
     __STAGES__ = [("expose_boss", "expose_apogee")]
     __CLEANUP__ = ["cleanup"]
 
     expose_helper: ExposeHelper
     _pause_event = asyncio.Event()
 
+    def __init__(self):
+        super().__init__()
+
+        self.configuration: Configuration | None = None
+
     def _reset_internal(self, **opts):
         """Reset the exposure status."""
 
         self.expose_helper = ExposeHelper(self, **opts)
 
         # An event blocker for when we wait to pause the execution of the macro.
         if not self._pause_event.is_set():
@@ -597,16 +608,16 @@
 
         if self.helpers.boss.is_exposing():
             if self.helpers.boss.is_reading():
                 self.command.info("BOSS is reading.")
             else:
                 self.command.warning("BOSS exposure is running. Not cancelling it.")
 
-        if not self.failed and not self.cancelled and self.helpers.jaeger.configuration:
-            self.helpers.jaeger.configuration.observed = True
+        if not self.failed and not self.cancelled and self.configuration:
+            self.configuration.observed = True
 
     async def _pause(self):
         """Pauses the execution of the macro."""
 
         if self._pause_event.is_set():
             self._pause_event.clear()
             self.command.warning("Pausing execution of the expose macro.")
```

### Comparing `sdss_hal-1.2.0/src/hal/macros/goto_field.py` & `sdss_hal-1.2.1/src/hal/macros/goto_field.py`

 * *Files identical despite different names*

### Comparing `sdss_hal-1.2.0/src/hal/macros/macro.py` & `sdss_hal-1.2.1/src/hal/macros/macro.py`

 * *Files identical despite different names*

### Comparing `sdss_hal-1.2.0/src/hal/macros/test_macro.py` & `sdss_hal-1.2.1/src/hal/macros/test_macro.py`

 * *Files identical despite different names*

### Comparing `sdss_hal-1.2.0/PKG-INFO` & `sdss_hal-1.2.1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: sdss-hal
-Version: 1.2.0
+Version: 1.2.1
 Summary: High-level observing tool for SDSS-V (replaces SOP)
 Home-page: https://github.com/sdss/hal
 License: BSD-3-Clause
 Keywords: astronomy,software
 Author: José Sánchez-Gallego
 Author-email: gallegoj@uw.edu
 Requires-Python: >=3.10,<4.0
```

