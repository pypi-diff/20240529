# Comparing `tmp/eventum_core-1.0.1.tar.gz` & `tmp/eventum_core-1.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "eventum_core-1.0.1.tar", max compression
+gzip compressed data, was "eventum_core-1.0.2.tar", max compression
```

## Comparing `eventum_core-1.0.1.tar` & `eventum_core-1.0.2.tar`

### file list

```diff
@@ -1,13 +1,13 @@
--rw-r--r--   0        0        0    11345 2024-05-18 21:13:58.350025 eventum_core-1.0.1/LICENSE
--rw-r--r--   0        0        0     4969 2024-05-18 21:13:58.350025 eventum_core-1.0.1/README.md
--rw-r--r--   0        0        0        0 2024-05-18 21:13:58.350025 eventum_core-1.0.1/eventum_core/__init__.py
--rw-r--r--   0        0        0     6155 2024-05-27 18:25:30.864070 eventum_core-1.0.1/eventum_core/app.py
--rw-r--r--   0        0        0     2697 2024-05-18 21:13:58.350025 eventum_core-1.0.1/eventum_core/batcher.py
--rw-r--r--   0        0        0     3717 2024-05-27 18:43:56.363810 eventum_core-1.0.1/eventum_core/plugins_connector.py
--rw-r--r--   0        0        0        0 2024-05-26 15:45:08.775672 eventum_core-1.0.1/eventum_core/py.typed
--rw-r--r--   0        0        0     1311 2024-05-27 17:12:30.335092 eventum_core-1.0.1/eventum_core/settings.py
--rw-r--r--   0        0        0     8660 2024-05-27 18:52:49.493682 eventum_core-1.0.1/eventum_core/subprocesses.py
--rw-r--r--   0        0        0      940 2024-05-26 15:46:55.835646 eventum_core-1.0.1/eventum_core/tests/test_batcher.py
--rw-r--r--   0        0        0     3425 2024-05-27 18:59:13.803591 eventum_core-1.0.1/eventum_core/tests/test_subprocesses.py
--rw-r--r--   0        0        0     1234 2024-05-27 19:08:53.573460 eventum_core-1.0.1/pyproject.toml
--rw-r--r--   0        0        0     6227 1970-01-01 00:00:00.000000 eventum_core-1.0.1/PKG-INFO
+-rw-r--r--   0        0        0    11345 2024-05-18 21:13:58.350025 eventum_core-1.0.2/LICENSE
+-rw-r--r--   0        0        0     4969 2024-05-18 21:13:58.350025 eventum_core-1.0.2/README.md
+-rw-r--r--   0        0        0        0 2024-05-18 21:13:58.350025 eventum_core-1.0.2/eventum_core/__init__.py
+-rw-r--r--   0        0        0     6155 2024-05-28 20:10:31.868089 eventum_core-1.0.2/eventum_core/app.py
+-rw-r--r--   0        0        0     2697 2024-05-18 21:13:58.350025 eventum_core-1.0.2/eventum_core/batcher.py
+-rw-r--r--   0        0        0     3717 2024-05-27 18:43:56.363810 eventum_core-1.0.2/eventum_core/plugins_connector.py
+-rw-r--r--   0        0        0        0 2024-05-26 15:45:08.775672 eventum_core-1.0.2/eventum_core/py.typed
+-rw-r--r--   0        0        0     1311 2024-05-27 17:12:30.335092 eventum_core-1.0.2/eventum_core/settings.py
+-rw-r--r--   0        0        0     8660 2024-05-27 18:52:49.493682 eventum_core-1.0.2/eventum_core/subprocesses.py
+-rw-r--r--   0        0        0      940 2024-05-26 15:46:55.835646 eventum_core-1.0.2/eventum_core/tests/test_batcher.py
+-rw-r--r--   0        0        0     3425 2024-05-27 18:59:13.803591 eventum_core-1.0.2/eventum_core/tests/test_subprocesses.py
+-rw-r--r--   0        0        0     1234 2024-05-28 20:10:58.548086 eventum_core-1.0.2/pyproject.toml
+-rw-r--r--   0        0        0     6227 1970-01-01 00:00:00.000000 eventum_core-1.0.2/PKG-INFO
```

### Comparing `eventum_core-1.0.1/LICENSE` & `eventum_core-1.0.2/LICENSE`

 * *Files identical despite different names*

### Comparing `eventum_core-1.0.1/README.md` & `eventum_core-1.0.2/README.md`

 * *Files identical despite different names*

### Comparing `eventum_core-1.0.1/eventum_core/app.py` & `eventum_core-1.0.2/eventum_core/app.py`

 * *Ordering differences only*

 * *Files 0% similar despite different names*

```diff
@@ -57,16 +57,16 @@
 
         self._processed_events: SynchronizedBase = Value('Q', 0)
 
         self._proc_input = Process(
             target=start_input_subprocess,
             args=(
                 self._config.input,
-                self._time_mode,
                 self._settings,
+                self._time_mode,
                 self._input_queue,
                 self._is_input_done
             )
         )
         self._proc_event = Process(
             target=start_event_subprocess,
             args=(
```

### Comparing `eventum_core-1.0.1/eventum_core/batcher.py` & `eventum_core-1.0.2/eventum_core/batcher.py`

 * *Files identical despite different names*

### Comparing `eventum_core-1.0.1/eventum_core/plugins_connector.py` & `eventum_core-1.0.2/eventum_core/plugins_connector.py`

 * *Files identical despite different names*

### Comparing `eventum_core-1.0.1/eventum_core/settings.py` & `eventum_core-1.0.2/eventum_core/settings.py`

 * *Files identical despite different names*

### Comparing `eventum_core-1.0.1/eventum_core/subprocesses.py` & `eventum_core-1.0.2/eventum_core/subprocesses.py`

 * *Files identical despite different names*

### Comparing `eventum_core-1.0.1/eventum_core/tests/test_batcher.py` & `eventum_core-1.0.2/eventum_core/tests/test_batcher.py`

 * *Files identical despite different names*

### Comparing `eventum_core-1.0.1/eventum_core/tests/test_subprocesses.py` & `eventum_core-1.0.2/eventum_core/tests/test_subprocesses.py`

 * *Files identical despite different names*

### Comparing `eventum_core-1.0.1/pyproject.toml` & `eventum_core-1.0.2/pyproject.toml`

 * *Files 9% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "eventum-core"
-version = "1.0.1"
+version = "1.0.2"
 description = "Flexible event generator"
 license = "Apache-2.0"
 authors = ["Nikita Reznikov <nikita.reznikov.public@mail.ru>"]
 readme = "README.md"
 repository = "https://github.com/Eventum-Generatives/EventumCore"
 documentation = "https://eventum-generatives.github.io/Website/"
 keywords = ["generator", "testing", "data", "event"]
```

### Comparing `eventum_core-1.0.1/PKG-INFO` & `eventum_core-1.0.2/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: eventum-core
-Version: 1.0.1
+Version: 1.0.2
 Summary: Flexible event generator
 Home-page: https://github.com/Eventum-Generatives/EventumCore
 License: Apache-2.0
 Keywords: generator,testing,data,event
 Author: Nikita Reznikov
 Author-email: nikita.reznikov.public@mail.ru
 Requires-Python: >=3.11,<4.0
```

