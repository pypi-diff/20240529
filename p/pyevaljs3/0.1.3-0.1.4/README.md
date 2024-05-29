# Comparing `tmp/pyevaljs3-0.1.3.tar.gz` & `tmp/pyevaljs3-0.1.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pyevaljs3-0.1.3.tar", last modified: Sun May 26 10:22:45 2024, max compression
+gzip compressed data, was "pyevaljs3-0.1.4.tar", last modified: Wed May 29 15:09:26 2024, max compression
```

## Comparing `pyevaljs3-0.1.3.tar` & `pyevaljs3-0.1.4.tar`

### file list

```diff
@@ -1,22 +1,23 @@
-drwxrwxrwx   0        0        0        0 2024-05-26 10:22:45.515473 pyevaljs3-0.1.3/
--rw-rw-rw-   0        0        0     1093 2023-12-13 10:50:19.000000 pyevaljs3-0.1.3/LICENSE
--rw-rw-rw-   0        0        0     3332 2024-05-26 10:22:45.514473 pyevaljs3-0.1.3/PKG-INFO
--rw-rw-rw-   0        0        0     2542 2024-03-04 18:42:48.000000 pyevaljs3-0.1.3/README.md
-drwxrwxrwx   0        0        0        0 2024-05-26 10:22:45.498469 pyevaljs3-0.1.3/pyevaljs3/
--rw-rw-rw-   0        0        0     2565 2024-03-04 18:41:30.000000 pyevaljs3-0.1.3/pyevaljs3/__init__.py
--rw-rw-rw-   0        0        0       55 2024-05-26 10:20:50.000000 pyevaljs3-0.1.3/pyevaljs3/__version__.py
--rw-rw-rw-   0        0        0      329 2024-05-26 10:11:11.000000 pyevaljs3-0.1.3/pyevaljs3/_node_program.py
--rw-rw-rw-   0        0        0     1860 2024-05-18 11:31:35.000000 pyevaljs3-0.1.3/pyevaljs3/evaljs.py
--rw-rw-rw-   0        0        0       96 2023-12-13 08:02:55.000000 pyevaljs3-0.1.3/pyevaljs3/exception.py
--rw-rw-rw-   0        0        0      462 2024-05-26 10:17:44.000000 pyevaljs3-0.1.3/pyevaljs3/runner.py
--rw-rw-rw-   0        0        0     4095 2024-05-26 10:17:59.000000 pyevaljs3-0.1.3/pyevaljs3/runtime.py
--rw-rw-rw-   0        0        0       97 2024-05-26 10:20:03.000000 pyevaljs3-0.1.3/pyevaljs3/setting.py
-drwxrwxrwx   0        0        0        0 2024-05-26 10:22:45.513473 pyevaljs3-0.1.3/pyevaljs3.egg-info/
--rw-rw-rw-   0        0        0     3332 2024-05-26 10:22:45.000000 pyevaljs3-0.1.3/pyevaljs3.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      351 2024-05-26 10:22:45.000000 pyevaljs3-0.1.3/pyevaljs3.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-05-26 10:22:45.000000 pyevaljs3-0.1.3/pyevaljs3.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       10 2024-05-26 10:22:45.000000 pyevaljs3-0.1.3/pyevaljs3.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2024-05-26 10:22:45.516474 pyevaljs3-0.1.3/setup.cfg
--rw-rw-rw-   0        0        0     1193 2024-03-04 17:52:32.000000 pyevaljs3-0.1.3/setup.py
-drwxrwxrwx   0        0        0        0 2024-05-26 10:22:45.511472 pyevaljs3-0.1.3/tests/
--rw-rw-rw-   0        0        0      790 2024-05-26 08:12:35.000000 pyevaljs3-0.1.3/tests/test.py
+drwxrwxrwx   0        0        0        0 2024-05-29 15:09:26.153014 pyevaljs3-0.1.4/
+-rw-rw-rw-   0        0        0     1093 2023-12-13 10:50:19.000000 pyevaljs3-0.1.4/LICENSE
+-rw-rw-rw-   0        0        0     3332 2024-05-29 15:09:26.152014 pyevaljs3-0.1.4/PKG-INFO
+-rw-rw-rw-   0        0        0     2542 2024-03-04 18:42:48.000000 pyevaljs3-0.1.4/README.md
+drwxrwxrwx   0        0        0        0 2024-05-29 15:09:26.137010 pyevaljs3-0.1.4/pyevaljs3/
+-rw-rw-rw-   0        0        0     2565 2024-03-04 18:41:30.000000 pyevaljs3-0.1.4/pyevaljs3/__init__.py
+-rw-rw-rw-   0        0        0       55 2024-05-29 15:06:58.000000 pyevaljs3-0.1.4/pyevaljs3/__version__.py
+-rw-rw-rw-   0        0        0      329 2024-05-26 10:11:11.000000 pyevaljs3-0.1.4/pyevaljs3/_node_program.py
+-rw-rw-rw-   0        0        0     1860 2024-05-18 11:31:35.000000 pyevaljs3-0.1.4/pyevaljs3/evaljs.py
+-rw-rw-rw-   0        0        0      176 2024-05-29 15:02:01.000000 pyevaljs3-0.1.4/pyevaljs3/exception.py
+-rw-rw-rw-   0        0        0      462 2024-05-26 10:17:44.000000 pyevaljs3-0.1.4/pyevaljs3/runner.py
+-rw-rw-rw-   0        0        0     4269 2024-05-29 15:06:58.000000 pyevaljs3-0.1.4/pyevaljs3/runtime.py
+-rw-rw-rw-   0        0        0       97 2024-05-26 10:20:03.000000 pyevaljs3-0.1.4/pyevaljs3/setting.py
+-rw-rw-rw-   0        0        0      195 2024-05-29 15:06:58.000000 pyevaljs3-0.1.4/pyevaljs3/utils.py
+drwxrwxrwx   0        0        0        0 2024-05-29 15:09:26.151013 pyevaljs3-0.1.4/pyevaljs3.egg-info/
+-rw-rw-rw-   0        0        0     3332 2024-05-29 15:09:26.000000 pyevaljs3-0.1.4/pyevaljs3.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      370 2024-05-29 15:09:26.000000 pyevaljs3-0.1.4/pyevaljs3.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-05-29 15:09:26.000000 pyevaljs3-0.1.4/pyevaljs3.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       10 2024-05-29 15:09:26.000000 pyevaljs3-0.1.4/pyevaljs3.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2024-05-29 15:09:26.153014 pyevaljs3-0.1.4/setup.cfg
+-rw-rw-rw-   0        0        0     1193 2024-03-04 17:52:32.000000 pyevaljs3-0.1.4/setup.py
+drwxrwxrwx   0        0        0        0 2024-05-29 15:09:26.149012 pyevaljs3-0.1.4/tests/
+-rw-rw-rw-   0        0        0     1010 2024-05-29 07:02:55.000000 pyevaljs3-0.1.4/tests/test.py
```

### Comparing `pyevaljs3-0.1.3/LICENSE` & `pyevaljs3-0.1.4/LICENSE`

 * *Files identical despite different names*

### Comparing `pyevaljs3-0.1.3/PKG-INFO` & `pyevaljs3-0.1.4/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pyevaljs3
-Version: 0.1.3
+Version: 0.1.4
 Summary: 一个依赖node.js来执行js代码的python库
 Home-page: https://github.com/Smawexi/PyevalJS3
 Author: Samwe
 Author-email: 1281722462@qq.com
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
```

### Comparing `pyevaljs3-0.1.3/README.md` & `pyevaljs3-0.1.4/README.md`

 * *Files identical despite different names*

### Comparing `pyevaljs3-0.1.3/pyevaljs3/__init__.py` & `pyevaljs3-0.1.4/pyevaljs3/__init__.py`

 * *Files identical despite different names*

### Comparing `pyevaljs3-0.1.3/pyevaljs3/evaljs.py` & `pyevaljs3-0.1.4/pyevaljs3/evaljs.py`

 * *Files identical despite different names*

### Comparing `pyevaljs3-0.1.3/pyevaljs3/runtime.py` & `pyevaljs3-0.1.4/pyevaljs3/runtime.py`

 * *Files 8% similar despite different names*

```diff
@@ -10,43 +10,42 @@
 import json
 import abc
 import tempfile
 
 from . import exception
 from .setting import IS_WINDOWS, NO_WARNINGS
 from .runner import Runner
+from .utils import get_node_env
 JSException = exception.JSException
+RunTimeNotFoundError = exception.RunTimeNotFoundError
 _logger = logging.getLogger("JSEval")
 if not IS_WINDOWS:
     subprocess.DETACHED_PROCESS = 0
 
 
-def get_node_env():
-    node = os.environ.get('NODE_PATH') if os.environ.get('NODE_PATH') else os.environ.get('NODE')
-    if not node:
-        return "node"
-    return node
-
-
 class AbstractRuntime:
 
     @abc.abstractmethod
     def eval(self, code: str = None):
         raise NotImplementedError()
 
     @abc.abstractmethod
     def compile(self, source: str = None, suffix: str = None):
         raise NotImplementedError()
 
     def _eval(self, code: str = None, ignore_output=False):
         node = get_node_env()
         _cmd = [node, NO_WARNINGS]
         _input = Runner.program('eval', code)
-        popen = subprocess.Popen(_cmd, stdin=subprocess.PIPE, stdout=subprocess.PIPE, stderr=subprocess.STDOUT,
-                                 universal_newlines=True, creationflags=subprocess.DETACHED_PROCESS)
+        try:
+            popen = subprocess.Popen(_cmd, stdin=subprocess.PIPE, stdout=subprocess.PIPE, stderr=subprocess.STDOUT,
+                                     universal_newlines=True, creationflags=subprocess.DETACHED_PROCESS)
+        except Exception:
+            raise RunTimeNotFoundError("Missing node environment")
+
         try:
             outs, errs = popen.communicate(input=_input)
         except Exception as e:
             _logger.error(e)
             popen.kill()
             outs, errs = popen.communicate()
 
@@ -85,16 +84,21 @@
         raise NotImplementedError()
 
     def _call(self, func, args):
         node = get_node_env()
         _source = Runner.program('call', self._source, func, args)
         _path = self._make_temp_file(_source)
         _cmd = [node, NO_WARNINGS, _path]
-        popen = subprocess.Popen(_cmd, stdin=subprocess.PIPE, stdout=subprocess.PIPE, stderr=subprocess.STDOUT,
-                                 universal_newlines=True, creationflags=subprocess.DETACHED_PROCESS)
+        try:
+            popen = subprocess.Popen(_cmd, stdin=subprocess.PIPE, stdout=subprocess.PIPE, stderr=subprocess.STDOUT,
+                                     universal_newlines=True, creationflags=subprocess.DETACHED_PROCESS)
+        except Exception:
+            os.remove(_path)
+            raise RunTimeNotFoundError("Missing node environment")
+
         try:
             outs, errs = popen.communicate()
         except Exception as e:
             _logger.error(e)
             popen.kill()
             outs, errs = popen.communicate()
         finally:
```

### Comparing `pyevaljs3-0.1.3/pyevaljs3.egg-info/PKG-INFO` & `pyevaljs3-0.1.4/pyevaljs3.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pyevaljs3
-Version: 0.1.3
+Version: 0.1.4
 Summary: 一个依赖node.js来执行js代码的python库
 Home-page: https://github.com/Smawexi/PyevalJS3
 Author: Samwe
 Author-email: 1281722462@qq.com
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
```

### Comparing `pyevaljs3-0.1.3/setup.py` & `pyevaljs3-0.1.4/setup.py`

 * *Files identical despite different names*

### Comparing `pyevaljs3-0.1.3/tests/test.py` & `pyevaljs3-0.1.4/tests/test.py`

 * *Files 15% similar despite different names*

```diff
@@ -1,19 +1,28 @@
 import json
+import time
+
 import pyevaljs3
 
 payload = {
         "cursor_score": "", "num": 31, "refresh_type": 1, "note_index": 35, "unread_begin_note_id": "",
         "unread_end_note_id": "", "unread_note_count": 0, "category": "homefeed_recommend", "search_key": "",
         "need_num": 6, "image_formats": ["jpg", "webp", "avif"]
     }
 
 cookie = 'a1=18c0436e5549rvr1aukayp8l2qjpdrh8f3wz3nlc650000328069;web_session=030037a25201ca6f3b3ef31319224af8cd067a;'
 
 code = open("xhs2.js", encoding="utf-8").read()
 code += ';return getXS("/api/sns/web/v1/homefeed", %s, "%s");' % (json.dumps(payload), cookie)
 xsxt = pyevaljs3.eval_(code, True)
 print(xsxt, type(xsxt))
-
+s = time.time()
+for _ in range(100):
+    xsxt = pyevaljs3.eval_(code, True)
+    # print(xsxt, type(xsxt))
+print(time.time() - s)
 ctx = pyevaljs3.compile_('xhs2.js')
-r = ctx.call('getXS', "/api/sns/web/v1/homefeed", payload, cookie)
-print(r, type(r))
+s = time.time()
+for _ in range(100):
+    r = ctx.call('getXS', "/api/sns/web/v1/homefeed", payload, cookie)
+    # print(r, type(r))
+print(time.time() - s)
```

