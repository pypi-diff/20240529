# Comparing `tmp/baserun-1.0.0b2.tar.gz` & `tmp/baserun-1.0.0b4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "baserun-1.0.0b2.tar", last modified: Wed May 22 21:35:53 2024, max compression
+gzip compressed data, was "baserun-1.0.0b4.tar", last modified: Tue May 28 20:50:46 2024, max compression
```

## Comparing `baserun-1.0.0b2.tar` & `baserun-1.0.0b4.tar`

### file list

```diff
@@ -1,28 +1,28 @@
-drwxr-xr-x   0 epeterson   (501) staff       (20)        0 2024-05-22 21:35:53.521123 baserun-1.0.0b2/
--rw-r--r--   0 epeterson   (501) staff       (20)     1073 2023-08-04 18:23:26.000000 baserun-1.0.0b2/LICENSE
--rw-r--r--   0 epeterson   (501) staff       (20)     6223 2024-05-22 21:35:53.520942 baserun-1.0.0b2/PKG-INFO
--rw-r--r--   0 epeterson   (501) staff       (20)     4569 2024-03-20 17:26:14.000000 baserun-1.0.0b2/README.md
-drwxr-xr-x   0 epeterson   (501) staff       (20)        0 2024-05-22 21:35:53.478915 baserun-1.0.0b2/baserun/
--rw-r--r--   0 epeterson   (501) staff       (20)     1381 2024-05-22 21:27:26.000000 baserun-1.0.0b2/baserun/__init__.py
--rw-r--r--   0 epeterson   (501) staff       (20)     8252 2024-05-22 21:26:13.000000 baserun-1.0.0b2/baserun/api.py
--rw-r--r--   0 epeterson   (501) staff       (20)     6754 2024-05-22 21:15:55.000000 baserun-1.0.0b2/baserun/mixins.py
-drwxr-xr-x   0 epeterson   (501) staff       (20)        0 2024-05-22 21:35:53.484968 baserun-1.0.0b2/baserun/models/
--rw-r--r--   0 epeterson   (501) staff       (20)        0 2024-05-22 21:03:15.000000 baserun-1.0.0b2/baserun/models/__init__.py
--rw-r--r--   0 epeterson   (501) staff       (20)     3292 2024-05-22 21:17:36.000000 baserun-1.0.0b2/baserun/models/evals.py
--rw-r--r--   0 epeterson   (501) staff       (20)     2390 2024-05-22 21:17:36.000000 baserun-1.0.0b2/baserun/models/tags.py
--rw-r--r--   0 epeterson   (501) staff       (20)        0 2024-05-22 21:30:51.000000 baserun-1.0.0b2/baserun/py.typed
--rw-r--r--   0 epeterson   (501) staff       (20)     2086 2024-05-22 21:03:15.000000 baserun-1.0.0b2/baserun/utils.py
-drwxr-xr-x   0 epeterson   (501) staff       (20)        0 2024-05-22 21:35:53.518004 baserun-1.0.0b2/baserun/wrappers/
--rw-r--r--   0 epeterson   (501) staff       (20)        0 2024-05-22 21:03:15.000000 baserun-1.0.0b2/baserun/wrappers/__init__.py
--rw-r--r--   0 epeterson   (501) staff       (20)    16173 2024-05-22 21:16:07.000000 baserun-1.0.0b2/baserun/wrappers/openai.py
-drwxr-xr-x   0 epeterson   (501) staff       (20)        0 2024-05-22 21:35:53.520167 baserun-1.0.0b2/baserun.egg-info/
--rw-r--r--   0 epeterson   (501) staff       (20)     6223 2024-05-22 21:35:53.000000 baserun-1.0.0b2/baserun.egg-info/PKG-INFO
--rw-r--r--   0 epeterson   (501) staff       (20)      474 2024-05-22 21:35:53.000000 baserun-1.0.0b2/baserun.egg-info/SOURCES.txt
--rw-r--r--   0 epeterson   (501) staff       (20)        1 2024-05-22 21:35:53.000000 baserun-1.0.0b2/baserun.egg-info/dependency_links.txt
--rw-r--r--   0 epeterson   (501) staff       (20)       44 2024-05-22 21:35:53.000000 baserun-1.0.0b2/baserun.egg-info/entry_points.txt
--rw-r--r--   0 epeterson   (501) staff       (20)       21 2024-05-22 21:35:53.000000 baserun-1.0.0b2/baserun.egg-info/requires.txt
--rw-r--r--   0 epeterson   (501) staff       (20)        8 2024-05-22 21:35:53.000000 baserun-1.0.0b2/baserun.egg-info/top_level.txt
--rw-r--r--   0 epeterson   (501) staff       (20)     1091 2024-05-22 21:35:16.000000 baserun-1.0.0b2/pyproject.toml
--rw-r--r--   0 epeterson   (501) staff       (20)       81 2024-05-22 21:35:53.521732 baserun-1.0.0b2/setup.cfg
-drwxr-xr-x   0 epeterson   (501) staff       (20)        0 2024-05-22 21:35:53.519064 baserun-1.0.0b2/tests/
--rw-r--r--   0 epeterson   (501) staff       (20)    13540 2024-05-22 21:17:36.000000 baserun-1.0.0b2/tests/testing_functions.py
+drwxr-xr-x   0 epeterson   (501) staff       (20)        0 2024-05-28 20:50:46.632039 baserun-1.0.0b4/
+-rw-r--r--   0 epeterson   (501) staff       (20)     1073 2023-08-04 18:23:26.000000 baserun-1.0.0b4/LICENSE
+-rw-r--r--   0 epeterson   (501) staff       (20)     6223 2024-05-28 20:50:46.631748 baserun-1.0.0b4/PKG-INFO
+-rw-r--r--   0 epeterson   (501) staff       (20)     4569 2024-03-20 17:26:14.000000 baserun-1.0.0b4/README.md
+drwxr-xr-x   0 epeterson   (501) staff       (20)        0 2024-05-28 20:50:46.606783 baserun-1.0.0b4/baserun/
+-rw-r--r--   0 epeterson   (501) staff       (20)     1381 2024-05-28 20:37:48.000000 baserun-1.0.0b4/baserun/__init__.py
+-rw-r--r--   0 epeterson   (501) staff       (20)     8668 2024-05-28 20:48:32.000000 baserun-1.0.0b4/baserun/api.py
+-rw-r--r--   0 epeterson   (501) staff       (20)     6754 2024-05-28 20:37:48.000000 baserun-1.0.0b4/baserun/mixins.py
+drwxr-xr-x   0 epeterson   (501) staff       (20)        0 2024-05-28 20:50:46.626951 baserun-1.0.0b4/baserun/models/
+-rw-r--r--   0 epeterson   (501) staff       (20)        0 2024-05-28 20:37:48.000000 baserun-1.0.0b4/baserun/models/__init__.py
+-rw-r--r--   0 epeterson   (501) staff       (20)     3292 2024-05-28 20:37:48.000000 baserun-1.0.0b4/baserun/models/evals.py
+-rw-r--r--   0 epeterson   (501) staff       (20)     2390 2024-05-28 20:37:48.000000 baserun-1.0.0b4/baserun/models/tags.py
+-rw-r--r--   0 epeterson   (501) staff       (20)        0 2024-05-22 21:30:51.000000 baserun-1.0.0b4/baserun/py.typed
+-rw-r--r--   0 epeterson   (501) staff       (20)     2086 2024-05-28 20:37:48.000000 baserun-1.0.0b4/baserun/utils.py
+drwxr-xr-x   0 epeterson   (501) staff       (20)        0 2024-05-28 20:50:46.628678 baserun-1.0.0b4/baserun/wrappers/
+-rw-r--r--   0 epeterson   (501) staff       (20)        0 2024-05-28 20:37:48.000000 baserun-1.0.0b4/baserun/wrappers/__init__.py
+-rw-r--r--   0 epeterson   (501) staff       (20)    16173 2024-05-28 20:37:48.000000 baserun-1.0.0b4/baserun/wrappers/openai.py
+drwxr-xr-x   0 epeterson   (501) staff       (20)        0 2024-05-28 20:50:46.630652 baserun-1.0.0b4/baserun.egg-info/
+-rw-r--r--   0 epeterson   (501) staff       (20)     6223 2024-05-28 20:50:46.000000 baserun-1.0.0b4/baserun.egg-info/PKG-INFO
+-rw-r--r--   0 epeterson   (501) staff       (20)      474 2024-05-28 20:50:46.000000 baserun-1.0.0b4/baserun.egg-info/SOURCES.txt
+-rw-r--r--   0 epeterson   (501) staff       (20)        1 2024-05-28 20:50:46.000000 baserun-1.0.0b4/baserun.egg-info/dependency_links.txt
+-rw-r--r--   0 epeterson   (501) staff       (20)       44 2024-05-28 20:50:46.000000 baserun-1.0.0b4/baserun.egg-info/entry_points.txt
+-rw-r--r--   0 epeterson   (501) staff       (20)       21 2024-05-28 20:50:46.000000 baserun-1.0.0b4/baserun.egg-info/requires.txt
+-rw-r--r--   0 epeterson   (501) staff       (20)        8 2024-05-28 20:50:46.000000 baserun-1.0.0b4/baserun.egg-info/top_level.txt
+-rw-r--r--   0 epeterson   (501) staff       (20)     1091 2024-05-28 20:50:26.000000 baserun-1.0.0b4/pyproject.toml
+-rw-r--r--   0 epeterson   (501) staff       (20)       81 2024-05-28 20:50:46.632986 baserun-1.0.0b4/setup.cfg
+drwxr-xr-x   0 epeterson   (501) staff       (20)        0 2024-05-28 20:50:46.629567 baserun-1.0.0b4/tests/
+-rw-r--r--   0 epeterson   (501) staff       (20)    13539 2024-05-28 20:39:02.000000 baserun-1.0.0b4/tests/testing_functions.py
```

### Comparing `baserun-1.0.0b2/LICENSE` & `baserun-1.0.0b4/LICENSE`

 * *Files identical despite different names*

### Comparing `baserun-1.0.0b2/PKG-INFO` & `baserun-1.0.0b4/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: baserun
-Version: 1.0.0b2
+Version: 1.0.0b4
 Summary: tools for testing, debugging, and evaluating llm features.
 Author-email: Erik Peterson <erik@baserun.ai>
 License: MIT License
         
         Copyright (c) 2023 Mochi Labs, Inc.
         
         Permission is hereby granted, free of charge, to any person obtaining a copy
@@ -26,15 +26,15 @@
         SOFTWARE.
         
 Project-URL: Homepage, https://baserun.ai
 Project-URL: Repository, https://github.com/baserun-ai/baserun-py
 Requires-Python: <3.12,>=3.8
 Description-Content-Type: text/markdown
 License-File: LICENSE
-Requires-Dist: httpx[http2]>=0.20.0
+Requires-Dist: httpx[http2]>=0.24.0
 
 # Baserun
 
 
 [![](https://img.shields.io/badge/Visit%20Us-baserun.ai-brightgreen)](https://baserun.ai)
 [![](https://img.shields.io/badge/View%20Documentation-Docs-yellow)](https://docs.baserun.ai)
 [![](https://img.shields.io/badge/Join%20our%20community-Discord-blue)](https://discord.gg/xEPFsvSmkb)
```

### Comparing `baserun-1.0.0b2/README.md` & `baserun-1.0.0b4/README.md`

 * *Files identical despite different names*

### Comparing `baserun-1.0.0b2/baserun/__init__.py` & `baserun-1.0.0b4/baserun/__init__.py`

 * *Files identical despite different names*

### Comparing `baserun-1.0.0b2/baserun/api.py` & `baserun-1.0.0b4/baserun/api.py`

 * *Files 13% similar despite different names*

```diff
@@ -1,18 +1,16 @@
 import asyncio
 import atexit
 import json
 import logging
 import os
-import signal
-import sys
-from queue import Empty, Queue
-from threading import Lock, Thread
+from multiprocessing import Process, Queue
+from queue import Empty
 from time import sleep
-from typing import TYPE_CHECKING, Any, Dict, Optional, Union
+from typing import TYPE_CHECKING, Any, Dict, List, Optional, Union
 
 import httpx
 import tiktoken
 from openai.types.chat import ChatCompletionMessageParam
 
 from baserun.utils import deep_merge
 
@@ -21,19 +19,18 @@
         WrappedAsyncStream,
         WrappedChatCompletion,
         WrappedOpenAIBaseClient,
         WrappedSyncStream,
     )
 
 logger = logging.getLogger(__name__)
-logging.basicConfig(level=logging.DEBUG)
 
 exporter_queue: Queue = Queue()
-exporter_thread: Union[Thread, None] = None
-thread_lock = Lock()
+tasks: List[asyncio.Task] = []  # Make tasks a global variable
+exporter_process: Union[Process, None] = None
 
 
 def count_prompt_tokens(
     messages: list[ChatCompletionMessageParam],
     encoder="cl100k_base",
 ):
     """FYI this doesn't count "name" keys correctly"""
@@ -44,88 +41,102 @@
 
 def count_message_tokens(text: str, encoder="cl100k_base"):
     return len(tiktoken.get_encoding(encoder).encode(text))
 
 
 async def worker(queue: Queue, base_url: str, api_key: str):
     logger.debug(f"Starting worker with base_url: {base_url}")
+    tasks: List[asyncio.Task] = []  # Create tasks locally
     async with httpx.AsyncClient(http2=True) as client:
         while True:
             try:
-                item: Dict = queue.get(timeout=1)
+                item: Dict = queue.get_nowait()
             except Empty:
+                sleep(1)
                 continue
 
             if item is None:
                 break
 
             try:
                 endpoint = item.pop("endpoint")
                 data = item.pop("data")
                 logger.debug(f"Submitting {data} to Baserun at {base_url}/api/public/{endpoint}")
-                result = await client.post(
-                    f"{base_url}/api/public/{endpoint}",
-                    headers={"Authorization": f"Bearer {api_key}"},
-                    json=data,
+                tasks.append(
+                    asyncio.create_task(
+                        client.post(
+                            f"{base_url}/api/public/{endpoint}",
+                            headers={"Authorization": f"Bearer {api_key}"},
+                            json=data,
+                        )
+                    )
                 )
-                logger.debug(f"Got response from Baserun: {result} {result.headers}")
             except Exception as e:
                 logger.warning(f"Failed to submit {endpoint} to Baserun: {e}")
-            finally:
-                queue.task_done()
+
+    logger.debug(f"Waiting for {len(tasks)} tasks to finish")
+    await asyncio.gather(*tasks)
+    logger.debug("Exiting worker")
+    loop = asyncio.get_running_loop()
+    loop.stop()
+
+
+def run_worker(queue, base_url, api_key):
+    loop = asyncio.new_event_loop()
+    asyncio.set_event_loop(loop)
+    loop.create_task(worker(queue, base_url, api_key))
+    try:
+        loop.run_forever()
+    except KeyboardInterrupt:
+        pass
+    finally:
+        loop.close()
 
 
 def start_worker(base_url: str, api_key: str):
-    global exporter_thread
-    with thread_lock:
-        if exporter_thread is None:
-            loop = asyncio.new_event_loop()
-            asyncio.set_event_loop(loop)
-            exporter_thread = Thread(
-                target=loop.run_until_complete,
-                args=(worker(exporter_queue, base_url, api_key),),
-            )
-            exporter_thread.daemon = True
-            exporter_thread.start()
+    global exporter_process
+    if exporter_process is None:
+        exporter_process = Process(
+            target=run_worker,
+            args=(exporter_queue, base_url, api_key),
+        )
+        exporter_process.daemon = False
+        exporter_process.start()
 
 
 class ApiClient:
     def __init__(
         self,
         client: Union["WrappedOpenAIBaseClient"],
         api_key: Optional[str] = None,
         base_url: Optional[str] = None,
     ):
         self.environment = os.getenv("BASERUN_ENVIRONMENT", os.getenv("ENVIRONMENT", "production"))
         self.client = client
 
-        def signal_function(sig, frame):
-            self.exit_handler(sig, frame)
-
-        signal.signal(signal.SIGINT, signal_function)
-        signal.signal(signal.SIGTERM, signal_function)
         atexit.register(self.exit_handler)
 
         start_worker(
             base_url or os.getenv("BASERUN_API_URL") or "https://app.baserun.ai",
             api_key or os.getenv("BASERUN_API_KEY") or "",
         )
 
     def exit_handler(self, *args) -> None:
-        logger.debug("Baserun exiting")
-        exporter_queue.put(None)
-
-        try_count = 0
-        while not exporter_queue.empty() and try_count < 5:
-            logger.debug("Baserun finishing export of spans")
-            sleep(0.25)
-            try_count += 1
-
-        if len(args) > 1:
-            sys.exit(0)
+        global exporter_process, exporter_queue, tasks  # Add tasks to global variables
+        if exporter_process is not None:
+            # Put None into the queue to signal the worker to stop
+            exporter_queue.put(None)
+            while len(tasks):
+                logger.debug(f"Waiting for {len(tasks)} tasks to finish")
+                sleep(0.25)
+            exporter_process.terminate()
+            exporter_process.join()
+        # Close and join the queue
+        if exporter_queue is not None:
+            exporter_queue.close()
 
     def submit_completion(self, completion: "WrappedChatCompletion"):
         dict_items = completion.model_dump()
         dict_items.pop("client", None)
         start_timestamp = dict_items.pop("start_timestamp", None)
         end_timestamp = dict_items.pop("end_timestamp", None)
         first_token_timestamp = dict_items.pop("first_token_timestamp", None)
```

### Comparing `baserun-1.0.0b2/baserun/mixins.py` & `baserun-1.0.0b4/baserun/mixins.py`

 * *Files identical despite different names*

### Comparing `baserun-1.0.0b2/baserun/models/evals.py` & `baserun-1.0.0b4/baserun/models/evals.py`

 * *Files identical despite different names*

### Comparing `baserun-1.0.0b2/baserun/models/tags.py` & `baserun-1.0.0b4/baserun/models/tags.py`

 * *Files identical despite different names*

### Comparing `baserun-1.0.0b2/baserun/utils.py` & `baserun-1.0.0b4/baserun/utils.py`

 * *Files identical despite different names*

### Comparing `baserun-1.0.0b2/baserun/wrappers/openai.py` & `baserun-1.0.0b4/baserun/wrappers/openai.py`

 * *Files identical despite different names*

### Comparing `baserun-1.0.0b2/baserun.egg-info/PKG-INFO` & `baserun-1.0.0b4/baserun.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: baserun
-Version: 1.0.0b2
+Version: 1.0.0b4
 Summary: tools for testing, debugging, and evaluating llm features.
 Author-email: Erik Peterson <erik@baserun.ai>
 License: MIT License
         
         Copyright (c) 2023 Mochi Labs, Inc.
         
         Permission is hereby granted, free of charge, to any person obtaining a copy
@@ -26,15 +26,15 @@
         SOFTWARE.
         
 Project-URL: Homepage, https://baserun.ai
 Project-URL: Repository, https://github.com/baserun-ai/baserun-py
 Requires-Python: <3.12,>=3.8
 Description-Content-Type: text/markdown
 License-File: LICENSE
-Requires-Dist: httpx[http2]>=0.20.0
+Requires-Dist: httpx[http2]>=0.24.0
 
 # Baserun
 
 
 [![](https://img.shields.io/badge/Visit%20Us-baserun.ai-brightgreen)](https://baserun.ai)
 [![](https://img.shields.io/badge/View%20Documentation-Docs-yellow)](https://docs.baserun.ai)
 [![](https://img.shields.io/badge/Join%20our%20community-Discord-blue)](https://discord.gg/xEPFsvSmkb)
```

### Comparing `baserun-1.0.0b2/pyproject.toml` & `baserun-1.0.0b4/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,23 +1,23 @@
 [build-system]
 requires = ["setuptools", "wheel"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "baserun"
-version = "1.0.0b2"
+version = "1.0.0b4"
 description = "tools for testing, debugging, and evaluating llm features."
 readme = "README.md"
 license = { file = "LICENSE" }
 authors = [
     { name = "Erik Peterson", email = "erik@baserun.ai" }
 ]
 requires-python = ">=3.8, <3.12"
 dependencies = [
-    "httpx[http2]>=0.20.0",
+    "httpx[http2]>=0.24.0",
 ]
 
 [project.urls]
 Homepage = "https://baserun.ai"
 Repository = "https://github.com/baserun-ai/baserun-py"
 
 [project.entry-points.pytest11]
```

### Comparing `baserun-1.0.0b2/tests/testing_functions.py` & `baserun-1.0.0b4/tests/testing_functions.py`

 * *Files 1% similar despite different names*

```diff
@@ -356,15 +356,14 @@
     return result
 
 
 # Allows you to call any of these functions, e.g. python tests/testing_functions.py openai_chat_functions_streaming
 if __name__ == "__main__":
     from dotenv import load_dotenv
 
-
     load_dotenv()
     openai.api_key = os.environ.get("OPENAI_API_KEY")
 
     parser = argparse.ArgumentParser(description="Execute a function with a prompt.")
     parser.add_argument("function_to_call", type=str, help="Name of the function to call")
     parser.add_argument("--prompt", type=str, help="Prompt to pass to the function", default=None)
 
@@ -382,8 +381,8 @@
                 print(f"----- {name} result:\n{result}\n-----")
             except Exception:
                 exc_type, exc_value, exc_traceback = sys.exc_info()
                 traceback.print_exception(exc_type, exc_value, exc_traceback)
     else:
         call_function(traced_functions, function_name, parsed_args)
 
-    sleep(2)
+    sleep(4)
```

