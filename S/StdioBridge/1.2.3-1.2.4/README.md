# Comparing `tmp/StdioBridge-1.2.3.tar.gz` & `tmp/StdioBridge-1.2.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "StdioBridge-1.2.3.tar", last modified: Thu May 23 18:21:22 2024, max compression
+gzip compressed data, was "StdioBridge-1.2.4.tar", last modified: Wed May 29 09:33:11 2024, max compression
```

## Comparing `StdioBridge-1.2.3.tar` & `StdioBridge-1.2.4.tar`

### file list

```diff
@@ -1,24 +1,24 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-23 18:21:22.245226 StdioBridge-1.2.3/
--rw-r--r--   0 runner    (1001) docker     (127)     1069 2024-05-23 18:21:07.000000 StdioBridge-1.2.3/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)     3536 2024-05-23 18:21:22.245226 StdioBridge-1.2.3/PKG-INFO
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-23 18:21:22.241226 StdioBridge-1.2.3/StdioBridge/
--rw-r--r--   0 runner    (1001) docker     (127)       59 2024-05-23 18:21:07.000000 StdioBridge-1.2.3/StdioBridge/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)       18 2024-05-23 18:21:07.000000 StdioBridge-1.2.3/StdioBridge/_config.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-23 18:21:22.245226 StdioBridge-1.2.3/StdioBridge/api/
--rw-r--r--   0 runner    (1001) docker     (127)      185 2024-05-23 18:21:07.000000 StdioBridge-1.2.3/StdioBridge/api/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     3594 2024-05-23 18:21:07.000000 StdioBridge-1.2.3/StdioBridge/api/_api.py
--rw-r--r--   0 runner    (1001) docker     (127)      822 2024-05-23 18:21:07.000000 StdioBridge-1.2.3/StdioBridge/api/_response.py
--rw-r--r--   0 runner    (1001) docker     (127)     7208 2024-05-23 18:21:07.000000 StdioBridge-1.2.3/StdioBridge/api/_router.py
--rw-r--r--   0 runner    (1001) docker     (127)     1424 2024-05-23 18:21:07.000000 StdioBridge-1.2.3/StdioBridge/api/errors.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-23 18:21:22.245226 StdioBridge-1.2.3/StdioBridge/client/
--rw-r--r--   0 runner    (1001) docker     (127)      112 2024-05-23 18:21:07.000000 StdioBridge-1.2.3/StdioBridge/client/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     4379 2024-05-23 18:21:07.000000 StdioBridge-1.2.3/StdioBridge/client/_client.py
--rw-r--r--   0 runner    (1001) docker     (127)     1334 2024-05-23 18:21:07.000000 StdioBridge-1.2.3/StdioBridge/client/_response.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-23 18:21:22.241226 StdioBridge-1.2.3/StdioBridge.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     3536 2024-05-23 18:21:22.000000 StdioBridge-1.2.3/StdioBridge.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      464 2024-05-23 18:21:22.000000 StdioBridge-1.2.3/StdioBridge.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-23 18:21:22.000000 StdioBridge-1.2.3/StdioBridge.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       18 2024-05-23 18:21:22.000000 StdioBridge-1.2.3/StdioBridge.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       12 2024-05-23 18:21:22.000000 StdioBridge-1.2.3/StdioBridge.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-23 18:21:22.245226 StdioBridge-1.2.3/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)     1170 2024-05-23 18:21:07.000000 StdioBridge-1.2.3/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-29 09:33:11.400504 StdioBridge-1.2.4/
+-rw-r--r--   0 runner    (1001) docker     (127)     1069 2024-05-29 09:33:02.000000 StdioBridge-1.2.4/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)     3536 2024-05-29 09:33:11.400504 StdioBridge-1.2.4/PKG-INFO
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-29 09:33:11.396504 StdioBridge-1.2.4/StdioBridge/
+-rw-r--r--   0 runner    (1001) docker     (127)       59 2024-05-29 09:33:02.000000 StdioBridge-1.2.4/StdioBridge/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)       18 2024-05-29 09:33:02.000000 StdioBridge-1.2.4/StdioBridge/_config.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-29 09:33:11.400504 StdioBridge-1.2.4/StdioBridge/api/
+-rw-r--r--   0 runner    (1001) docker     (127)      185 2024-05-29 09:33:02.000000 StdioBridge-1.2.4/StdioBridge/api/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3770 2024-05-29 09:33:02.000000 StdioBridge-1.2.4/StdioBridge/api/_api.py
+-rw-r--r--   0 runner    (1001) docker     (127)      822 2024-05-29 09:33:02.000000 StdioBridge-1.2.4/StdioBridge/api/_response.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7208 2024-05-29 09:33:02.000000 StdioBridge-1.2.4/StdioBridge/api/_router.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1424 2024-05-29 09:33:02.000000 StdioBridge-1.2.4/StdioBridge/api/errors.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-29 09:33:11.400504 StdioBridge-1.2.4/StdioBridge/client/
+-rw-r--r--   0 runner    (1001) docker     (127)      112 2024-05-29 09:33:02.000000 StdioBridge-1.2.4/StdioBridge/client/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4379 2024-05-29 09:33:02.000000 StdioBridge-1.2.4/StdioBridge/client/_client.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1334 2024-05-29 09:33:02.000000 StdioBridge-1.2.4/StdioBridge/client/_response.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-29 09:33:11.396504 StdioBridge-1.2.4/StdioBridge.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     3536 2024-05-29 09:33:11.000000 StdioBridge-1.2.4/StdioBridge.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      464 2024-05-29 09:33:11.000000 StdioBridge-1.2.4/StdioBridge.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-29 09:33:11.000000 StdioBridge-1.2.4/StdioBridge.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       18 2024-05-29 09:33:11.000000 StdioBridge-1.2.4/StdioBridge.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       12 2024-05-29 09:33:11.000000 StdioBridge-1.2.4/StdioBridge.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-29 09:33:11.400504 StdioBridge-1.2.4/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)     1170 2024-05-29 09:33:02.000000 StdioBridge-1.2.4/setup.py
```

### Comparing `StdioBridge-1.2.3/LICENSE` & `StdioBridge-1.2.4/LICENSE`

 * *Files identical despite different names*

### Comparing `StdioBridge-1.2.3/PKG-INFO` & `StdioBridge-1.2.4/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: StdioBridge
-Version: 1.2.3
+Version: 1.2.4
 Summary: A StdioBridge package.
 Home-page: https://github.com/SergeiKrivko
 Author: SergeiKrivko
 License: MIT License
         
         Copyright (c) 2024 SergeiKrivko
```

### Comparing `StdioBridge-1.2.3/StdioBridge/api/_api.py` & `StdioBridge-1.2.4/StdioBridge/api/_api.py`

 * *Files 7% similar despite different names*

```diff
@@ -50,43 +50,45 @@
             res = await func(data, path_params, query)
 
             if isinstance(res, StreamResponse):
                 if not stream:
                     lst = []
                     async for chunk in res:
                         lst.append(chunk)
-                    print('!response!', json.dumps({'id': resp_id, 'code': res.code, 'data': lst}), sep='')
+                    print('!response!', json.dumps({'id': resp_id, 'code': res.code, 'data': lst}), sep='', flush=True)
                 else:
                     started = False
                     async for el in res:
                         if not started:
-                            print('!stream_start!', json.dumps({'id': resp_id, 'code': res.code}), sep='')
+                            print('!stream_start!', json.dumps({'id': resp_id, 'code': res.code}), sep='', flush=True)
                             started = True
-                        print('!stream_chunk!', json.dumps({'id': resp_id, 'chunk': el}), sep='')
-                    print('!stream_end!', json.dumps({'id': resp_id, 'code': res.code}), sep='')
+                        print('!stream_chunk!', json.dumps({'id': resp_id, 'chunk': el}), sep='', flush=True)
+                    print('!stream_end!', json.dumps({'id': resp_id, 'code': res.code}), sep='', flush=True)
             elif isinstance(res, Response):
                 if stream:
-                    print('!stream_start!', json.dumps({'id': resp_id, 'code': res.code}), sep='')
-                    print('!stream_chunk!', json.dumps({'id': resp_id, 'chunk': res.data}), sep='')
-                    print('!stream_end!', json.dumps({'id': resp_id, 'code': res.code}), sep='')
+                    print('!stream_start!', json.dumps({'id': resp_id, 'code': res.code}), sep='', flush=True)
+                    print('!stream_chunk!', json.dumps({'id': resp_id, 'chunk': res.data}), sep='', flush=True)
+                    print('!stream_end!', json.dumps({'id': resp_id, 'code': res.code}), sep='', flush=True)
                 else:
-                    print('!response!', json.dumps({'id': resp_id, 'code': res.code, 'data': res.data}), sep='')
+                    print('!response!', json.dumps({'id': resp_id, 'code': res.code, 'data': res.data}), sep='',
+                          flush=True)
             else:
                 raise InternalServerError(f"Error in StdioBridge: Invalid response type {type(res)}")
         except ApiError as err:
-            print('!response!', json.dumps({'id': resp_id, 'code': err.code, 'data': {'message': err.message}}), sep='')
+            print('!response!', json.dumps({'id': resp_id, 'code': err.code, 'data': {'message': err.message}}), sep='',
+                  flush=True)
         except Exception:
             print('!response!', json.dumps({'id': resp_id, 'code': 500,
-                                            'data': {'message': "Internal Server Error"}}), sep='')
+                                            'data': {'message': "Internal Server Error"}}), sep='', flush=True)
 
     def run(self):
         asyncio.run(self._run())
 
     async def _run(self):
         while True:
             try:
                 inp = await ainput()
                 data = json.loads(inp)
             except json.JSONDecodeError:
-                print("Invalid JSON")
+                print("Invalid JSON", flush=True)
             else:
                 asyncio.create_task(self._process_request(data)).done()
```

### Comparing `StdioBridge-1.2.3/StdioBridge/api/_response.py` & `StdioBridge-1.2.4/StdioBridge/api/_response.py`

 * *Files identical despite different names*

### Comparing `StdioBridge-1.2.3/StdioBridge/api/_router.py` & `StdioBridge-1.2.4/StdioBridge/api/_router.py`

 * *Files identical despite different names*

### Comparing `StdioBridge-1.2.3/StdioBridge/api/errors.py` & `StdioBridge-1.2.4/StdioBridge/api/errors.py`

 * *Files identical despite different names*

### Comparing `StdioBridge-1.2.3/StdioBridge/client/_client.py` & `StdioBridge-1.2.4/StdioBridge/client/_client.py`

 * *Files identical despite different names*

### Comparing `StdioBridge-1.2.3/StdioBridge/client/_response.py` & `StdioBridge-1.2.4/StdioBridge/client/_response.py`

 * *Files identical despite different names*

### Comparing `StdioBridge-1.2.3/StdioBridge.egg-info/PKG-INFO` & `StdioBridge-1.2.4/StdioBridge.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: StdioBridge
-Version: 1.2.3
+Version: 1.2.4
 Summary: A StdioBridge package.
 Home-page: https://github.com/SergeiKrivko
 Author: SergeiKrivko
 License: MIT License
         
         Copyright (c) 2024 SergeiKrivko
```

### Comparing `StdioBridge-1.2.3/setup.py` & `StdioBridge-1.2.4/setup.py`

 * *Files identical despite different names*

