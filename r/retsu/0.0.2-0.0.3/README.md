# Comparing `tmp/retsu-0.0.2.tar.gz` & `tmp/retsu-0.0.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "retsu-0.0.2.tar", max compression
+gzip compressed data, was "retsu-0.0.3.tar", max compression
```

## Comparing `retsu-0.0.2.tar` & `retsu-0.0.3.tar`

### file list

```diff
@@ -1,10 +1,10 @@
--rw-r--r--   0        0        0     1514 2024-05-28 03:22:21.814493 retsu-0.0.2/LICENSE
--rw-r--r--   0        0        0      319 2024-05-28 03:22:21.814493 retsu-0.0.2/README.md
--rw-r--r--   0        0        0     2213 2024-05-28 03:23:25.762966 retsu-0.0.2/pyproject.toml
--rw-r--r--   0        0        0      666 2024-05-28 03:23:25.762966 retsu-0.0.2/src/retsu/__init__.py
--rw-r--r--   0        0        0     1755 2024-05-28 03:22:21.818493 retsu-0.0.2/src/retsu/celery.py
--rw-r--r--   0        0        0     5494 2024-05-28 03:22:21.818493 retsu-0.0.2/src/retsu/core.py
--rw-r--r--   0        0        0       31 2024-05-28 03:22:21.818493 retsu-0.0.2/src/retsu/plugins/__init__.py
--rw-r--r--   0        0        0      827 2024-05-28 03:22:21.818493 retsu-0.0.2/src/retsu/plugins/django.py
--rw-r--r--   0        0        0        0 2024-05-28 03:22:21.818493 retsu-0.0.2/src/retsu/py.typed
--rw-r--r--   0        0        0     1075 1970-01-01 00:00:00.000000 retsu-0.0.2/PKG-INFO
+-rw-r--r--   0        0        0     1514 2024-05-29 04:16:24.816518 retsu-0.0.3/LICENSE
+-rw-r--r--   0        0        0      319 2024-05-29 04:16:24.820518 retsu-0.0.3/README.md
+-rw-r--r--   0        0        0     2224 2024-05-29 04:17:28.440662 retsu-0.0.3/pyproject.toml
+-rw-r--r--   0        0        0      666 2024-05-29 04:17:28.436662 retsu-0.0.3/src/retsu/__init__.py
+-rw-r--r--   0        0        0     1956 2024-05-29 04:16:24.820518 retsu-0.0.3/src/retsu/celery.py
+-rw-r--r--   0        0        0     5513 2024-05-29 04:16:24.820518 retsu-0.0.3/src/retsu/core.py
+-rw-r--r--   0        0        0       31 2024-05-29 04:16:24.820518 retsu-0.0.3/src/retsu/plugins/__init__.py
+-rw-r--r--   0        0        0      827 2024-05-29 04:16:24.824518 retsu-0.0.3/src/retsu/plugins/django.py
+-rw-r--r--   0        0        0        0 2024-05-29 04:16:24.824518 retsu-0.0.3/src/retsu/py.typed
+-rw-r--r--   0        0        0     1075 1970-01-01 00:00:00.000000 retsu-0.0.3/PKG-INFO
```

### Comparing `retsu-0.0.2/LICENSE` & `retsu-0.0.3/LICENSE`

 * *Files identical despite different names*

### Comparing `retsu-0.0.2/pyproject.toml` & `retsu-0.0.3/pyproject.toml`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "retsu"
-version = "0.0.2"  # semantic-release
+version = "0.0.3"  # semantic-release
 description = "Retsu aims to wrap-up Celery in way to facilitate to create parallel and serial tasks"
 readme = "README.md"
 authors = ["Ivan Ogasawara <ivan.ogasawara@gmail.com>"]
 packages = [
   {include = "retsu", from="src"},
 ]
 license = "BSD 3 Clause"
@@ -81,14 +81,15 @@
 [tool.ruff]
 line-length = 79
 force-exclude = true
 src = ["./"]
 exclude = [
   'docs',
 ]
+fix = true
 
 [tool.ruff.lint]
 select = [
   "E",   # pycodestyle
   "F",   # pyflakes
   "D",   # pydocstyle
   "YTT", # flake8-2020
```

### Comparing `retsu-0.0.2/src/retsu/__init__.py` & `retsu-0.0.3/src/retsu/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -11,15 +11,15 @@
 
 
 def get_version() -> str:
     """Return the program version."""
     try:
         return importlib_metadata.version(__name__)
     except importlib_metadata.PackageNotFoundError:  # pragma: no cover
-        return "0.0.2"  # semantic-release
+        return "0.0.3"  # semantic-release
 
 
 version = get_version()
 
 __version__ = version
 __author__ = "Ivan Ogasawara"
 __email__ = "ivan.ogasawara@gmail.com"
```

### Comparing `retsu-0.0.2/src/retsu/celery.py` & `retsu-0.0.3/src/retsu/celery.py`

 * *Files 11% similar despite different names*

```diff
@@ -17,24 +17,32 @@
     def task(self, *args, task_id: str, **kwargs) -> None:  # type: ignore
         """Define the task to be executed."""
         chord_tasks, chord_callback = self.get_chord_tasks(
             *args, task_id=task_id, **kwargs
         )
         chain_tasks = self.get_chain_tasks(*args, task_id=task_id, **kwargs)
 
+        # start the tasks
         if chord_tasks:
             if chord_callback:
                 workflow_chord = chord(chord_tasks, chord_callback)
             else:
                 workflow_chord = chord(chord_tasks)
-            workflow_chord.apply_async()
+            promise_chord = workflow_chord.apply_async()
 
         if chain_tasks:
             workflow_chain = chain(chord_tasks)
-            workflow_chain.apply_async()
+            promise_chain = workflow_chain.apply_async()
+
+        # wait for the tasks
+        if chord_tasks:
+            promise_chord.get()
+
+        if chain_tasks:
+            promise_chain.get()
 
     def get_chord_tasks(  # type: ignore
         self, *args, **kwargs
     ) -> tuple[list[celery.Signature], Optional[celery.Signature]]:
         """
         Run tasks with chord.
```

### Comparing `retsu-0.0.2/src/retsu/core.py` & `retsu-0.0.3/src/retsu/core.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,29 +1,33 @@
 """Retsu core classes."""
 
 from __future__ import annotations
 
 import json
 import multiprocessing as mp
+import os
 import warnings
 
 from abc import abstractmethod
 from pathlib import Path
 from typing import Any, Optional, cast
 from uuid import uuid4
 
 from public import public
 
 
 class ResultTask:
     """Result from a task."""
 
-    def __init__(self, result_path: Path) -> None:
+    def __init__(self) -> None:
         """Initialize ResultTask."""
-        self.result_path = result_path
+        self.result_path = Path(
+            os.getenv("RETSU_RESULT_PATH", "/tmp/retsu/results")
+        )
+        os.makedirs(self.result_path, exist_ok=True)
 
     @public
     def save(self, task_id: str, result: Any) -> None:
         """Save the result in a file."""
         with open(self.result_path / f"{task_id}.json", "w") as f:
             json.dump(
                 {"task_id": task_id, "result": result},
@@ -55,19 +59,19 @@
         return self.load(task_id)
 
 
 @public
 class Task:
     """Main class for handling a task."""
 
-    def __init__(self, result_path: Path, workers: int = 1) -> None:
+    def __init__(self, workers: int = 1) -> None:
         """Initialize a task object."""
         self.active = True
         self.workers = workers
-        self.result = ResultTask(result_path)
+        self.result = ResultTask()
         self.queue_in: mp.Queue[Any] = mp.Queue()
         self.processes: list[mp.Process] = []
 
     @public
     def get_result(self, task_id: str) -> Any:
         """Get the result for given task id."""
         return self.result.get(task_id)
@@ -143,34 +147,34 @@
                 return
             self.prepare_task(data)
 
 
 class SerialTask(Task):
     """Serial Task class."""
 
-    def __init__(self, result_path: Path, workers: int = 1) -> None:
+    def __init__(self, workers: int = 1) -> None:
         """Initialize a serial task object."""
         if workers != 1:
             warnings.warn(
                 "SerialTask should have just 1 worker. "
                 "Switching automatically to 1 ..."
             )
             workers = 1
-        super().__init__(result_path, workers=workers)
+        super().__init__(workers=workers)
 
 
 class ParallelTask(Task):
     """Initialize a parallel task object."""
 
-    def __init__(self, result_path: Path, workers: int = 1) -> None:
+    def __init__(self, workers: int = 1) -> None:
         """Initialize ParallelTask."""
         if workers <= 1:
             raise Exception("ParallelTask should have more than 1 worker.")
 
-        super().__init__(result_path, workers=workers)
+        super().__init__(workers=workers)
 
 
 class TaskManager:
     """Manage tasks."""
 
     tasks: dict[str, Task]
```

### Comparing `retsu-0.0.2/src/retsu/plugins/django.py` & `retsu-0.0.3/src/retsu/plugins/django.py`

 * *Files identical despite different names*

### Comparing `retsu-0.0.2/PKG-INFO` & `retsu-0.0.3/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: retsu
-Version: 0.0.2
+Version: 0.0.3
 Summary: Retsu aims to wrap-up Celery in way to facilitate to create parallel and serial tasks
 License: BSD 3 Clause
 Author: Ivan Ogasawara
 Author-email: ivan.ogasawara@gmail.com
 Requires-Python: >=3.8.1,<4
 Classifier: License :: Other/Proprietary License
 Classifier: Programming Language :: Python :: 3
```

