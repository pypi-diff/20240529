# Comparing `tmp/g3tester-0.1.0.tar.gz` & `tmp/g3tester-0.1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "g3tester-0.1.0.tar", last modified: Mon Apr 29 21:27:52 2024, max compression
+gzip compressed data, was "g3tester-0.1.1.tar", last modified: Wed May 29 18:51:21 2024, max compression
```

## Comparing `g3tester-0.1.0.tar` & `g3tester-0.1.1.tar`

### file list

```diff
@@ -1,48 +1,48 @@
-drwxrwxrwx   0        0        0        0 2024-04-29 21:27:52.785411 g3tester-0.1.0/
--rw-rw-rw-   0        0        0     1091 2023-06-02 14:34:32.000000 g3tester-0.1.0/LICENCE
--rw-rw-rw-   0        0        0     1195 2024-04-29 21:27:52.783358 g3tester-0.1.0/PKG-INFO
--rw-rw-rw-   0        0        0      245 2024-04-29 21:23:39.000000 g3tester-0.1.0/README.md
--rw-rw-rw-   0        0        0     1082 2024-04-29 20:36:08.000000 g3tester-0.1.0/pyproject.toml
--rw-rw-rw-   0        0        0       42 2024-04-29 21:27:52.785411 g3tester-0.1.0/setup.cfg
-drwxrwxrwx   0        0        0        0 2024-04-29 21:27:52.440872 g3tester-0.1.0/src/
-drwxrwxrwx   0        0        0        0 2024-04-29 21:27:52.524195 g3tester-0.1.0/src/g3tester/
--rw-rw-rw-   0        0        0      603 2024-04-15 12:13:55.000000 g3tester-0.1.0/src/g3tester/__init__.py
--rw-rw-rw-   0        0        0    10799 2024-04-15 13:38:53.000000 g3tester-0.1.0/src/g3tester/_memory.py
--rw-rw-rw-   0        0        0    60409 2024-04-15 13:43:25.000000 g3tester-0.1.0/src/g3tester/_test.py
--rw-rw-rw-   0        0        0      994 2024-04-15 13:41:13.000000 g3tester-0.1.0/src/g3tester/enums.py
--rw-rw-rw-   0        0        0      211 2024-04-15 07:51:48.000000 g3tester-0.1.0/src/g3tester/exceptions.py
--rw-rw-rw-   0        0        0        0 2024-03-21 00:48:36.000000 g3tester-0.1.0/src/g3tester/py.typed
-drwxrwxrwx   0        0        0        0 2024-04-29 21:27:52.559093 g3tester-0.1.0/src/g3tester/tags/
--rw-rw-rw-   0        0        0      403 2024-04-15 07:48:52.000000 g3tester-0.1.0/src/g3tester/tags/__init__.py
--rw-rw-rw-   0        0        0    51181 2024-04-16 17:33:23.000000 g3tester-0.1.0/src/g3tester/tags/_tags.py
-drwxrwxrwx   0        0        0        0 2024-04-29 21:27:52.565794 g3tester-0.1.0/src/g3tester/testinfo/
--rw-rw-rw-   0        0        0      140 2024-04-15 12:14:09.000000 g3tester-0.1.0/src/g3tester/testinfo/__init__.py
--rw-rw-rw-   0        0        0     2224 2024-04-15 12:14:29.000000 g3tester-0.1.0/src/g3tester/testinfo/_testinfo.py
-drwxrwxrwx   0        0        0        0 2024-04-29 21:27:52.571808 g3tester-0.1.0/src/g3tester/testlib/
--rw-rw-rw-   0        0        0      212 2024-04-15 09:38:00.000000 g3tester-0.1.0/src/g3tester/testlib/__init__.py
-drwxrwxrwx   0        0        0        0 2024-04-29 21:27:52.584623 g3tester-0.1.0/src/g3tester/testlib/all/
--rw-rw-rw-   0        0        0      260 2024-04-15 09:39:15.000000 g3tester-0.1.0/src/g3tester/testlib/all/__init__.py
-drwxrwxrwx   0        0        0        0 2024-04-29 21:27:52.653165 g3tester-0.1.0/src/g3tester/testlib/detector/
--rw-rw-rw-   0        0        0      213 2024-04-15 09:39:42.000000 g3tester-0.1.0/src/g3tester/testlib/detector/__init__.py
--rw-rw-rw-   0        0        0     3348 2024-04-14 14:22:59.000000 g3tester-0.1.0/src/g3tester/testlib/detector/_detector.py
-drwxrwxrwx   0        0        0        0 2024-04-29 21:27:52.671988 g3tester-0.1.0/src/g3tester/testlib/element/
--rw-rw-rw-   0        0        0      116 2024-03-27 13:46:11.000000 g3tester-0.1.0/src/g3tester/testlib/element/__init__.py
--rw-rw-rw-   0        0        0     4355 2024-04-15 09:42:46.000000 g3tester-0.1.0/src/g3tester/testlib/element/_element.py
-drwxrwxrwx   0        0        0        0 2024-04-29 21:27:52.706765 g3tester-0.1.0/src/g3tester/testlib/pointmachine/
--rw-rw-rw-   0        0        0      124 2024-03-25 15:27:38.000000 g3tester-0.1.0/src/g3tester/testlib/pointmachine/__init__.py
--rw-rw-rw-   0        0        0     7039 2024-04-15 09:43:43.000000 g3tester-0.1.0/src/g3tester/testlib/pointmachine/_pointmachine.py
-drwxrwxrwx   0        0        0        0 2024-04-29 21:27:52.754747 g3tester-0.1.0/src/g3tester/testlib/route/
--rw-rw-rw-   0        0        0      216 2024-04-03 19:29:18.000000 g3tester-0.1.0/src/g3tester/testlib/route/__init__.py
--rw-rw-rw-   0        0        0    45473 2024-04-29 20:21:27.000000 g3tester-0.1.0/src/g3tester/testlib/route/_passage_generator.py
--rw-rw-rw-   0        0        0    10141 2024-04-15 09:44:53.000000 g3tester-0.1.0/src/g3tester/testlib/route/_route.py
-drwxrwxrwx   0        0        0        0 2024-04-29 21:27:52.764850 g3tester-0.1.0/src/g3tester/testlib/zone/
--rw-rw-rw-   0        0        0      154 2024-03-24 20:48:19.000000 g3tester-0.1.0/src/g3tester/testlib/zone/__init__.py
--rw-rw-rw-   0        0        0     6360 2024-04-15 09:46:04.000000 g3tester-0.1.0/src/g3tester/testlib/zone/_zone.py
-drwxrwxrwx   0        0        0        0 2024-04-29 21:27:52.775306 g3tester-0.1.0/src/g3tester.egg-info/
--rw-rw-rw-   0        0        0     1195 2024-04-29 21:27:52.000000 g3tester-0.1.0/src/g3tester.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0     1032 2024-04-29 21:27:52.000000 g3tester-0.1.0/src/g3tester.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-04-29 21:27:52.000000 g3tester-0.1.0/src/g3tester.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       13 2024-04-29 21:27:52.000000 g3tester-0.1.0/src/g3tester.egg-info/requires.txt
--rw-rw-rw-   0        0        0        9 2024-04-29 21:27:52.000000 g3tester-0.1.0/src/g3tester.egg-info/top_level.txt
-drwxrwxrwx   0        0        0        0 2024-04-29 21:27:52.764850 g3tester-0.1.0/tests/
--rw-rw-rw-   0        0        0     1803 2024-04-15 07:47:34.000000 g3tester-0.1.0/tests/test_memory.py
+drwxrwxrwx   0        0        0        0 2024-05-29 18:51:21.643308 g3tester-0.1.1/
+-rw-rw-rw-   0        0        0     1091 2024-05-14 06:56:57.000000 g3tester-0.1.1/LICENCE
+-rw-rw-rw-   0        0        0     1195 2024-05-29 18:51:21.643308 g3tester-0.1.1/PKG-INFO
+-rw-rw-rw-   0        0        0      245 2024-05-14 06:56:57.000000 g3tester-0.1.1/README.md
+-rw-rw-rw-   0        0        0     1082 2024-05-29 18:42:14.000000 g3tester-0.1.1/pyproject.toml
+-rw-rw-rw-   0        0        0       42 2024-05-29 18:51:21.643308 g3tester-0.1.1/setup.cfg
+drwxrwxrwx   0        0        0        0 2024-05-29 18:51:21.574274 g3tester-0.1.1/src/
+drwxrwxrwx   0        0        0        0 2024-05-29 18:51:21.596408 g3tester-0.1.1/src/g3tester/
+-rw-rw-rw-   0        0        0      603 2024-05-14 06:56:57.000000 g3tester-0.1.1/src/g3tester/__init__.py
+-rw-rw-rw-   0        0        0    10799 2024-05-14 06:56:57.000000 g3tester-0.1.1/src/g3tester/_memory.py
+-rw-rw-rw-   0        0        0    60409 2024-05-21 15:04:00.000000 g3tester-0.1.1/src/g3tester/_test.py
+-rw-rw-rw-   0        0        0      994 2024-05-14 06:56:57.000000 g3tester-0.1.1/src/g3tester/enums.py
+-rw-rw-rw-   0        0        0      211 2024-05-14 06:56:57.000000 g3tester-0.1.1/src/g3tester/exceptions.py
+-rw-rw-rw-   0        0        0        0 2024-05-14 06:56:57.000000 g3tester-0.1.1/src/g3tester/py.typed
+drwxrwxrwx   0        0        0        0 2024-05-29 18:51:21.612049 g3tester-0.1.1/src/g3tester/tags/
+-rw-rw-rw-   0        0        0      403 2024-05-14 06:56:57.000000 g3tester-0.1.1/src/g3tester/tags/__init__.py
+-rw-rw-rw-   0        0        0    51181 2024-05-14 06:56:57.000000 g3tester-0.1.1/src/g3tester/tags/_tags.py
+drwxrwxrwx   0        0        0        0 2024-05-29 18:51:21.627674 g3tester-0.1.1/src/g3tester/testinfo/
+-rw-rw-rw-   0        0        0      140 2024-05-14 06:56:57.000000 g3tester-0.1.1/src/g3tester/testinfo/__init__.py
+-rw-rw-rw-   0        0        0     2224 2024-05-14 06:56:57.000000 g3tester-0.1.1/src/g3tester/testinfo/_testinfo.py
+drwxrwxrwx   0        0        0        0 2024-05-29 18:51:21.627674 g3tester-0.1.1/src/g3tester/testlib/
+-rw-rw-rw-   0        0        0      212 2024-05-14 06:56:57.000000 g3tester-0.1.1/src/g3tester/testlib/__init__.py
+drwxrwxrwx   0        0        0        0 2024-05-29 18:51:21.627674 g3tester-0.1.1/src/g3tester/testlib/all/
+-rw-rw-rw-   0        0        0      260 2024-05-14 06:56:57.000000 g3tester-0.1.1/src/g3tester/testlib/all/__init__.py
+drwxrwxrwx   0        0        0        0 2024-05-29 18:51:21.627674 g3tester-0.1.1/src/g3tester/testlib/detector/
+-rw-rw-rw-   0        0        0      213 2024-05-14 06:56:57.000000 g3tester-0.1.1/src/g3tester/testlib/detector/__init__.py
+-rw-rw-rw-   0        0        0     3348 2024-05-21 16:56:55.000000 g3tester-0.1.1/src/g3tester/testlib/detector/_detector.py
+drwxrwxrwx   0        0        0        0 2024-05-29 18:51:21.627674 g3tester-0.1.1/src/g3tester/testlib/element/
+-rw-rw-rw-   0        0        0      116 2024-05-14 06:56:57.000000 g3tester-0.1.1/src/g3tester/testlib/element/__init__.py
+-rw-rw-rw-   0        0        0     4355 2024-05-14 06:56:57.000000 g3tester-0.1.1/src/g3tester/testlib/element/_element.py
+drwxrwxrwx   0        0        0        0 2024-05-29 18:51:21.643308 g3tester-0.1.1/src/g3tester/testlib/pointmachine/
+-rw-rw-rw-   0        0        0      124 2024-05-14 06:56:57.000000 g3tester-0.1.1/src/g3tester/testlib/pointmachine/__init__.py
+-rw-rw-rw-   0        0        0     7039 2024-05-14 06:56:57.000000 g3tester-0.1.1/src/g3tester/testlib/pointmachine/_pointmachine.py
+drwxrwxrwx   0        0        0        0 2024-05-29 18:51:21.643308 g3tester-0.1.1/src/g3tester/testlib/route/
+-rw-rw-rw-   0        0        0      216 2024-05-14 06:56:57.000000 g3tester-0.1.1/src/g3tester/testlib/route/__init__.py
+-rw-rw-rw-   0        0        0    45477 2024-05-21 16:56:31.000000 g3tester-0.1.1/src/g3tester/testlib/route/_passage_generator.py
+-rw-rw-rw-   0        0        0    10224 2024-05-29 18:42:05.000000 g3tester-0.1.1/src/g3tester/testlib/route/_route.py
+drwxrwxrwx   0        0        0        0 2024-05-29 18:51:21.643308 g3tester-0.1.1/src/g3tester/testlib/zone/
+-rw-rw-rw-   0        0        0      154 2024-05-14 06:56:57.000000 g3tester-0.1.1/src/g3tester/testlib/zone/__init__.py
+-rw-rw-rw-   0        0        0     6360 2024-05-14 06:56:57.000000 g3tester-0.1.1/src/g3tester/testlib/zone/_zone.py
+drwxrwxrwx   0        0        0        0 2024-05-29 18:51:21.643308 g3tester-0.1.1/src/g3tester.egg-info/
+-rw-rw-rw-   0        0        0     1195 2024-05-29 18:51:21.000000 g3tester-0.1.1/src/g3tester.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0     1032 2024-05-29 18:51:21.000000 g3tester-0.1.1/src/g3tester.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-05-29 18:51:21.000000 g3tester-0.1.1/src/g3tester.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       13 2024-05-29 18:51:21.000000 g3tester-0.1.1/src/g3tester.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        9 2024-05-29 18:51:21.000000 g3tester-0.1.1/src/g3tester.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2024-05-29 18:51:21.643308 g3tester-0.1.1/tests/
+-rw-rw-rw-   0        0        0     1803 2024-05-14 06:56:57.000000 g3tester-0.1.1/tests/test_memory.py
```

### Comparing `g3tester-0.1.0/LICENCE` & `g3tester-0.1.1/LICENCE`

 * *Files identical despite different names*

### Comparing `g3tester-0.1.0/PKG-INFO` & `g3tester-0.1.1/PKG-INFO`

 * *Files 7% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: g3tester
-Version: 0.1.0
+Version: 0.1.1
 Summary: PLC System G3 testing suite
 Author: Elektroline a.s.
 Project-URL: Homepage, https://gitlab.elektroline.cz/plc/systemg3-py/SystemG3Tester
 Keywords: Elektroline,System G3
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Developers
 Classifier: Intended Audience :: Other Audience
```

### Comparing `g3tester-0.1.0/pyproject.toml` & `g3tester-0.1.1/pyproject.toml`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [project]
 name = "g3tester"
-version = "0.1.0"
+version = "0.1.1"
 description = "PLC System G3 testing suite"
 readme = "README.md"
 license = {file = "LICENSE"}
 authors = [
   { name = "Elektroline a.s." },
 ]
 classifiers = [
```

### Comparing `g3tester-0.1.0/src/g3tester/__init__.py` & `g3tester-0.1.1/src/g3tester/__init__.py`

 * *Files identical despite different names*

### Comparing `g3tester-0.1.0/src/g3tester/_memory.py` & `g3tester-0.1.1/src/g3tester/_memory.py`

 * *Files identical despite different names*

### Comparing `g3tester-0.1.0/src/g3tester/_test.py` & `g3tester-0.1.1/src/g3tester/_test.py`

 * *Files identical despite different names*

### Comparing `g3tester-0.1.0/src/g3tester/enums.py` & `g3tester-0.1.1/src/g3tester/enums.py`

 * *Files identical despite different names*

### Comparing `g3tester-0.1.0/src/g3tester/tags/_tags.py` & `g3tester-0.1.1/src/g3tester/tags/_tags.py`

 * *Files identical despite different names*

### Comparing `g3tester-0.1.0/src/g3tester/testinfo/_testinfo.py` & `g3tester-0.1.1/src/g3tester/testinfo/_testinfo.py`

 * *Files identical despite different names*

### Comparing `g3tester-0.1.0/src/g3tester/testlib/detector/_detector.py` & `g3tester-0.1.1/src/g3tester/testlib/detector/_detector.py`

 * *Files identical despite different names*

### Comparing `g3tester-0.1.0/src/g3tester/testlib/element/_element.py` & `g3tester-0.1.1/src/g3tester/testlib/element/_element.py`

 * *Files identical despite different names*

### Comparing `g3tester-0.1.0/src/g3tester/testlib/pointmachine/_pointmachine.py` & `g3tester-0.1.1/src/g3tester/testlib/pointmachine/_pointmachine.py`

 * *Files identical despite different names*

### Comparing `g3tester-0.1.0/src/g3tester/testlib/route/_passage_generator.py` & `g3tester-0.1.1/src/g3tester/testlib/route/_passage_generator.py`

 * *Files 0% similar despite different names*

```diff
@@ -73,21 +73,22 @@
         self.control_client = control_client
         self.test_client = test_client
         self.control_paths = control_paths or {}
         self.test_paths = test_paths or {}
 
     def get_default_path_control(self, element: ElementABC) -> str:
         return self.control_paths.setdefault(
-            element.shv_path_full, f'shv/{element.shv_path_full}'
+            element.shv_path_full, f'{element.shv_path_full}'
             )
 
     def get_default_path_test(self, element: ElementABC) -> str:
-        return self.test_paths.setdefault(
-            element.shv_path_full, f'shv/{element.shv_path_full}/_test'
+        path = self.test_paths.setdefault(
+            element.name, f'{element.shv_path_full}/_test'
             )
+        return path
 
     @typing.overload
     def __call__(
         self, element: Detector
     ) -> ElementSHVNodes[SHVDetectorControlNode, SHVDetectorTestNode]: ...
 
     @typing.overload
```

### Comparing `g3tester-0.1.0/src/g3tester/testlib/route/_route.py` & `g3tester-0.1.1/src/g3tester/testlib/route/_route.py`

 * *Files 2% similar despite different names*

```diff
@@ -42,15 +42,16 @@
 
     @command
     async def request(self) -> shv.SHVType:
         return await self.route_node.request()
 
     @value_getter
     async def get_route_memory(self) -> list[str]:
-        memory = await self.route_entry_gate_node.requestMemory.get()
+        
+        memory = await self.route_entry_gate_node.request_memory.get()
         if not isinstance(memory, str):
             raise TestFailFatal(f'Expected str, got {type(memory).__name__}')
         return memory.splitlines()
 
     @before_command(command=request)
     async def get_route_memory_before_request(self) -> None:
         memory = await self.get_route_memory()
@@ -222,20 +223,22 @@
                     f'OCCUPIED={self.trigger_detector_occupied}'
                     )
         self._logger.debug(
             'Waiting until the route "%s" switches to READY',
             self.route_name
             )
         bit_alias = self.route_control_node.status.BitAlias
-        await self.route_control_node.status.status_change_wait(
-            any_true=[bit_alias.READY, bit_alias.BUILD],
-            any_false=[bit_alias.FREE],
-            timeout=self.max_duration,
-            get_period=self._exec_sleep
-            )
+
+        if(route_status != bit_alias.READY):
+            await self.route_control_node.status.status_change_wait(
+                any_true=[bit_alias.READY, bit_alias.BUILD],
+                any_false=[bit_alias.FREE],
+                timeout=self.max_duration,
+                get_period=self._exec_sleep
+                )
         if self.trigger_detector_control_node is not None:
             # prevent race condition, when the trigger detector release after
             # its occupation is registered with a delay. This can happen if
             # the detector datachange event is not registered or
             # is registered with a delay. This is slightly unsafe, because
             # theoretically (although very unlikely) the detector release can
             # physically happen and be registered AFTER the route is ready,
```

### Comparing `g3tester-0.1.0/src/g3tester/testlib/zone/_zone.py` & `g3tester-0.1.1/src/g3tester/testlib/zone/_zone.py`

 * *Files identical despite different names*

### Comparing `g3tester-0.1.0/src/g3tester.egg-info/PKG-INFO` & `g3tester-0.1.1/src/g3tester.egg-info/PKG-INFO`

 * *Files 7% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: g3tester
-Version: 0.1.0
+Version: 0.1.1
 Summary: PLC System G3 testing suite
 Author: Elektroline a.s.
 Project-URL: Homepage, https://gitlab.elektroline.cz/plc/systemg3-py/SystemG3Tester
 Keywords: Elektroline,System G3
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Developers
 Classifier: Intended Audience :: Other Audience
```

### Comparing `g3tester-0.1.0/src/g3tester.egg-info/SOURCES.txt` & `g3tester-0.1.1/src/g3tester.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `g3tester-0.1.0/tests/test_memory.py` & `g3tester-0.1.1/tests/test_memory.py`

 * *Files identical despite different names*

