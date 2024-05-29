# Comparing `tmp/cobrafuzz-2.2.0.tar.gz` & `tmp/cobrafuzz-2.3.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "cobrafuzz-2.2.0.tar", last modified: Tue Mar 19 21:06:06 2024, max compression
+gzip compressed data, was "cobrafuzz-2.3.0.tar", last modified: Wed May 29 21:32:07 2024, max compression
```

## Comparing `cobrafuzz-2.2.0.tar` & `cobrafuzz-2.3.0.tar`

### file list

```diff
@@ -1,31 +1,33 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-19 21:06:06.878954 cobrafuzz-2.2.0/
--rw-r--r--   0 runner    (1001) docker     (127)    11356 2024-03-19 21:05:55.000000 cobrafuzz-2.2.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)     6218 2024-03-19 21:06:06.878954 cobrafuzz-2.2.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     4597 2024-03-19 21:05:55.000000 cobrafuzz-2.2.0/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-19 21:06:06.874954 cobrafuzz-2.2.0/cobrafuzz/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-03-19 21:05:55.000000 cobrafuzz-2.2.0/cobrafuzz/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)       88 2024-03-19 21:05:55.000000 cobrafuzz-2.2.0/cobrafuzz/common.py
--rw-r--r--   0 runner    (1001) docker     (127)    16679 2024-03-19 21:05:55.000000 cobrafuzz-2.2.0/cobrafuzz/fuzzer.py
--rw-r--r--   0 runner    (1001) docker     (127)     3220 2024-03-19 21:05:55.000000 cobrafuzz-2.2.0/cobrafuzz/main.py
--rw-r--r--   0 runner    (1001) docker     (127)    18062 2024-03-19 21:05:55.000000 cobrafuzz-2.2.0/cobrafuzz/mutator.py
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-03-19 21:05:55.000000 cobrafuzz-2.2.0/cobrafuzz/py.typed
--rw-r--r--   0 runner    (1001) docker     (127)     3554 2024-03-19 21:05:55.000000 cobrafuzz-2.2.0/cobrafuzz/state.py
--rw-r--r--   0 runner    (1001) docker     (127)     1615 2024-03-19 21:05:55.000000 cobrafuzz-2.2.0/cobrafuzz/tracer.py
--rw-r--r--   0 runner    (1001) docker     (127)     6191 2024-03-19 21:05:55.000000 cobrafuzz-2.2.0/cobrafuzz/util.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-19 21:06:06.874954 cobrafuzz-2.2.0/cobrafuzz.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     6218 2024-03-19 21:06:06.000000 cobrafuzz-2.2.0/cobrafuzz.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      493 2024-03-19 21:06:06.000000 cobrafuzz-2.2.0/cobrafuzz.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-03-19 21:06:06.000000 cobrafuzz-2.2.0/cobrafuzz.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)      441 2024-03-19 21:06:06.000000 cobrafuzz-2.2.0/cobrafuzz.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       36 2024-03-19 21:06:06.000000 cobrafuzz-2.2.0/cobrafuzz.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)     5617 2024-03-19 21:05:55.000000 cobrafuzz-2.2.0/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-03-19 21:06:06.878954 cobrafuzz-2.2.0/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-19 21:06:06.874954 cobrafuzz-2.2.0/stubs/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-03-19 21:05:55.000000 cobrafuzz-2.2.0/stubs/__init__.pyi
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-19 21:06:06.874954 cobrafuzz-2.2.0/stubs/scipy/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-03-19 21:05:55.000000 cobrafuzz-2.2.0/stubs/scipy/__init__.pyi
--rw-r--r--   0 runner    (1001) docker     (127)      221 2024-03-19 21:05:55.000000 cobrafuzz-2.2.0/stubs/scipy/stats.pyi
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-19 21:06:06.874954 cobrafuzz-2.2.0/tests/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-03-19 21:05:55.000000 cobrafuzz-2.2.0/tests/__init__.py
--rwxr-xr-x   0 runner    (1001) docker     (127)      242 2024-03-19 21:05:55.000000 cobrafuzz-2.2.0/tests/fuzz_fuzzer.py
--rw-r--r--   0 runner    (1001) docker     (127)      383 2024-03-19 21:05:55.000000 cobrafuzz-2.2.0/tests/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-29 21:32:07.886129 cobrafuzz-2.3.0/
+-rw-r--r--   0 runner    (1001) docker     (127)    11356 2024-05-29 21:32:03.000000 cobrafuzz-2.3.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)     6313 2024-05-29 21:32:07.882128 cobrafuzz-2.3.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     4636 2024-05-29 21:32:03.000000 cobrafuzz-2.3.0/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-29 21:32:07.878128 cobrafuzz-2.3.0/cobrafuzz/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-29 21:32:03.000000 cobrafuzz-2.3.0/cobrafuzz/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      136 2024-05-29 21:32:03.000000 cobrafuzz-2.3.0/cobrafuzz/common.py
+-rw-r--r--   0 runner    (1001) docker     (127)    16750 2024-05-29 21:32:03.000000 cobrafuzz-2.3.0/cobrafuzz/fuzzer.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5289 2024-05-29 21:32:03.000000 cobrafuzz-2.3.0/cobrafuzz/main.py
+-rw-r--r--   0 runner    (1001) docker     (127)    17766 2024-05-29 21:32:03.000000 cobrafuzz-2.3.0/cobrafuzz/mutator.py
+-rw-r--r--   0 runner    (1001) docker     (127)      555 2024-05-29 21:32:03.000000 cobrafuzz-2.3.0/cobrafuzz/prune.py
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-29 21:32:03.000000 cobrafuzz-2.3.0/cobrafuzz/py.typed
+-rw-r--r--   0 runner    (1001) docker     (127)     8568 2024-05-29 21:32:03.000000 cobrafuzz-2.3.0/cobrafuzz/simplifier.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3554 2024-05-29 21:32:03.000000 cobrafuzz-2.3.0/cobrafuzz/state.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1615 2024-05-29 21:32:03.000000 cobrafuzz-2.3.0/cobrafuzz/tracer.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8135 2024-05-29 21:32:03.000000 cobrafuzz-2.3.0/cobrafuzz/util.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-29 21:32:07.882128 cobrafuzz-2.3.0/cobrafuzz.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     6313 2024-05-29 21:32:07.000000 cobrafuzz-2.3.0/cobrafuzz.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      533 2024-05-29 21:32:07.000000 cobrafuzz-2.3.0/cobrafuzz.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-29 21:32:07.000000 cobrafuzz-2.3.0/cobrafuzz.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      464 2024-05-29 21:32:07.000000 cobrafuzz-2.3.0/cobrafuzz.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       36 2024-05-29 21:32:07.000000 cobrafuzz-2.3.0/cobrafuzz.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)     5648 2024-05-29 21:32:03.000000 cobrafuzz-2.3.0/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-29 21:32:07.886129 cobrafuzz-2.3.0/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-29 21:32:07.882128 cobrafuzz-2.3.0/stubs/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-29 21:32:03.000000 cobrafuzz-2.3.0/stubs/__init__.pyi
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-29 21:32:07.882128 cobrafuzz-2.3.0/stubs/scipy/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-29 21:32:03.000000 cobrafuzz-2.3.0/stubs/scipy/__init__.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)      221 2024-05-29 21:32:03.000000 cobrafuzz-2.3.0/stubs/scipy/stats.pyi
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-29 21:32:07.882128 cobrafuzz-2.3.0/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-29 21:32:03.000000 cobrafuzz-2.3.0/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1171 2024-05-29 21:32:03.000000 cobrafuzz-2.3.0/tests/test_doc.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2616 2024-05-29 21:32:03.000000 cobrafuzz-2.3.0/tests/utils.py
```

### Comparing `cobrafuzz-2.2.0/LICENSE` & `cobrafuzz-2.3.0/LICENSE`

 * *Files identical despite different names*

### Comparing `cobrafuzz-2.2.0/PKG-INFO` & `cobrafuzz-2.3.0/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: cobrafuzz
-Version: 2.2.0
+Version: 2.3.0
 Summary: Coverage-guided fuzz testing for Python
 Author-email: Alexander Senier <mail@senier.net>
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Operating System :: OS Independent
 Classifier: Topic :: Software Development :: Testing
 Requires-Python: >=3.8.0
@@ -21,14 +21,15 @@
 Requires-Dist: isort==5.13.2; extra == "devel"
 Requires-Dist: mypy<1.8.0; extra == "devel"
 Requires-Dist: plotly==5.19.0; extra == "devel"
 Requires-Dist: purl==1.6; extra == "devel"
 Requires-Dist: pytest==7.4.4; extra == "devel"
 Requires-Dist: pytest-cov==4.1.0; extra == "devel"
 Requires-Dist: pytest-xdist==3.5.0; extra == "devel"
+Requires-Dist: python-dateutil==2.9.0; extra == "devel"
 Requires-Dist: python-kacl==0.4.6; extra == "devel"
 Requires-Dist: requests==2.31.0; extra == "devel"
 Requires-Dist: ruff==0.1.13; extra == "devel"
 Requires-Dist: scipy<1.11; python_version < "3.9" and extra == "devel"
 Requires-Dist: scipy==1.11.4; python_version >= "3.9" and extra == "devel"
 Requires-Dist: types-requests==2.31.0.20240125; extra == "devel"
 Requires-Dist: vulture==2.11; extra == "devel"
@@ -49,30 +50,30 @@
 ## Usage
 
 ### Fuzz Target
 
 The first step is to implement a function to be fuzz-tested, also called a fuzz target.
 Here is an example of a simple fuzz target for the built-in `html` module
 
-```python
-from html.parser import HTMLParser
+```python,examples/fuzz_htmlparser/fuzz.py
 from cobrafuzz.main import CobraFuzz
 
 
 @CobraFuzz
-def fuzz(buf):
+def fuzz(buf: bytes) -> None:
+    from html.parser import HTMLParser
+
     try:
-        string = buf.decode("ascii")
         parser = HTMLParser()
-        parser.feed(string)
+        parser.feed(buf.decode("ascii"))
     except UnicodeDecodeError:
         pass
 
 
-if __name__ == '__main__':
+if __name__ == "__main__":
     fuzz()
 ```
 
 Features of a fuzz target:
 
 * `fuzz()` will call the fuzz target in an infinite loop with random data generated by the coverage-guided algorithm. The data is passed to the target in a separate process through the `buf` parameter.
 * The function must catch and ignore any expected exceptions that arise when passing invalid input to the tested program.
@@ -84,15 +85,15 @@
 
 The next step is to download CobraFuzz and then run the fuzzer:
 
 ```console
 $ pip install cobrafuzz
 [...]
 
-$ python examples/htmlparser/fuzz.py --crash-dir results --max-crashes 1
+$ python examples/fuzz_htmlparser/fuzz.py --crash-dir results fuzz --max-crashes 1
 #0 READ units: 1 workers: 7 seeds: 1
 #1 NEW     cov: 279 corp: 1 exec/s: 89 crashes: 0
 #5 NEW     cov: 366 corp: 2 exec/s: 299 crashes: 0
 #7 NEW     cov: 401 corp: 3 exec/s: 3124 crashes: 0
 [...]
 #154382 NEW     cov: 1086 corp: 50 exec/s: 22835 crashes: 0
 #156521 NEW     cov: 1092 corp: 51 exec/s: 2797 crashes: 0
```

### Comparing `cobrafuzz-2.2.0/README.md` & `cobrafuzz-2.3.0/README.md`

 * *Files 3% similar despite different names*

```diff
@@ -12,30 +12,30 @@
 ## Usage
 
 ### Fuzz Target
 
 The first step is to implement a function to be fuzz-tested, also called a fuzz target.
 Here is an example of a simple fuzz target for the built-in `html` module
 
-```python
-from html.parser import HTMLParser
+```python,examples/fuzz_htmlparser/fuzz.py
 from cobrafuzz.main import CobraFuzz
 
 
 @CobraFuzz
-def fuzz(buf):
+def fuzz(buf: bytes) -> None:
+    from html.parser import HTMLParser
+
     try:
-        string = buf.decode("ascii")
         parser = HTMLParser()
-        parser.feed(string)
+        parser.feed(buf.decode("ascii"))
     except UnicodeDecodeError:
         pass
 
 
-if __name__ == '__main__':
+if __name__ == "__main__":
     fuzz()
 ```
 
 Features of a fuzz target:
 
 * `fuzz()` will call the fuzz target in an infinite loop with random data generated by the coverage-guided algorithm. The data is passed to the target in a separate process through the `buf` parameter.
 * The function must catch and ignore any expected exceptions that arise when passing invalid input to the tested program.
@@ -47,15 +47,15 @@
 
 The next step is to download CobraFuzz and then run the fuzzer:
 
 ```console
 $ pip install cobrafuzz
 [...]
 
-$ python examples/htmlparser/fuzz.py --crash-dir results --max-crashes 1
+$ python examples/fuzz_htmlparser/fuzz.py --crash-dir results fuzz --max-crashes 1
 #0 READ units: 1 workers: 7 seeds: 1
 #1 NEW     cov: 279 corp: 1 exec/s: 89 crashes: 0
 #5 NEW     cov: 366 corp: 2 exec/s: 299 crashes: 0
 #7 NEW     cov: 401 corp: 3 exec/s: 3124 crashes: 0
 [...]
 #154382 NEW     cov: 1086 corp: 50 exec/s: 22835 crashes: 0
 #156521 NEW     cov: 1092 corp: 51 exec/s: 2797 crashes: 0
```

### Comparing `cobrafuzz-2.2.0/cobrafuzz/fuzzer.py` & `cobrafuzz-2.3.0/cobrafuzz/fuzzer.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,24 +1,24 @@
 from __future__ import annotations
 
+import atexit
 import hashlib
 import io
 import logging
 import multiprocessing as mp
 import sys
 import time
 import traceback
 from dataclasses import dataclass
 from pathlib import Path
-from types import TracebackType
 from typing import Callable, Optional, Union, cast
 
 import dill as pickle  # type: ignore[import-untyped]
 
-from cobrafuzz import state as st, tracer
+from cobrafuzz import simplifier, state as st, tracer, util
 
 logging.getLogger().setLevel(logging.DEBUG)
 
 MPContext = Union[mp.context.ForkContext, mp.context.ForkServerContext, mp.context.SpawnContext]
 MPProcess = Union[mp.context.ForkProcess, mp.context.ForkServerProcess, mp.context.SpawnProcess]
 
 
@@ -54,29 +54,14 @@
 
 
 @dataclass
 class Error(Report):
     message: str
 
 
-def covered(t: Optional[TracebackType]) -> set[tuple[Optional[str], Optional[int], str, int]]:
-    """Construct coverage information from exception traceback."""
-
-    prev_line: Optional[int] = None
-    prev_file: Optional[str] = None
-    result = set()
-    tb: Optional[TracebackType] = t
-    while tb:
-        result.add((prev_file, prev_line, tb.tb_frame.f_code.co_filename, tb.tb_lineno))
-        prev_line = tb.tb_lineno
-        prev_file = tb.tb_frame.f_code.co_filename
-        tb = tb.tb_next
-    return result
-
-
 def worker(  # noqa: PLR0913
     wid: int,
     target_bytes: bytes,
     update_queue: mp.Queue[Update],
     result_queue: mp.Queue[StatusBase],
     close_stdout: bool,
     close_stderr: bool,
@@ -172,29 +157,29 @@
     def unraisablehook(unraisable: sys.UnraisableHookArgs) -> None:
         message = (
             "\n".join(map(str, unraisable.exc_value.args))
             if unraisable.exc_value
             else "Unraisable exception"
         )
         nonlocal unraisable_covered, unraisable_message
-        unraisable_covered = covered(unraisable.exc_traceback)
+        unraisable_covered = util.covered(unraisable.exc_traceback)
         unraisable_message = message
         del unraisable
 
     _old_unraisablehook = sys.unraisablehook
     sys.unraisablehook = unraisablehook
 
     try:
         target(bytes(data))
     except Exception as e:  # noqa: BLE001
         return Error(
             wid=wid,
             runs=runs,
             data=data,
-            covered=covered(e.__traceback__),
+            covered=util.covered(e.__traceback__),
             message=f"{traceback.format_exc()}",
         )
     finally:
         sys.unraisablehook = _old_unraisablehook
 
     if unraisable_message:
         return Error(
@@ -232,14 +217,15 @@
         max_time: Optional[int] = None,
         num_workers: Optional[int] = 1,
         regression: bool = False,
         seeds: Optional[list[Path]] = None,
         start_method: Optional[str] = None,
         state_file: Optional[Path] = None,
         load_crashes: bool = True,
+        simplify: Optional[Path] = None,
     ):
         """
         Fuzz-test target and store crash artifacts into crash_dir.
 
         Arguments:
         ---------
         crash_dir:          Directory to store crash artifacts in. Will be created if missing.
@@ -252,19 +238,21 @@
         stat_frequency:     Frequency in which to produce a statistics if no other events are
                             logged.
         max_crashes:        Number of crashes after which to exit the fuzzer.
         max_input_size:     Maximum length of input to create.
         max_insert_length:  Maximum number of bytes to insert during mutation.
         max_modifications:  Maximum number of consecutive modifications during mutation.
         max_runs:           Number of target executions after which to exit the fuzzer.
-        max_time:           Number of seconds after which to exit the fuzzer.
+        max_time:           Number of seconds after which to exit.
         num_workers:        Number of parallel workers.
                             Use None to spawn one fewer than CPUs available.
         regression:         Execute target on all samples found in crash_dir, print errors and exit.
         seeds:              List of files and directories to seed the fuzzer with.
+        simplify:           When set, run simplifier and store simplified crash results in
+                            directory.
         start_method:       Multiprocessing start method to use (spawn, forkserver or fork).
                             Defaults to "spawn". Do not use "fork" as it is unreliable and may lead
                             to deadlocks.
         state_file:         File to load state from. Will be updated periodically. If no file is
                             specified, the state will be held in memory and discarded on exit.
         load_crashes:       Load crashes from crash directory on startup.
         """
@@ -283,14 +271,15 @@
             else mp.get_context("spawn")
         )
 
         self._result_queue: mp.Queue[Result] = self._mp_ctx.Queue()
         self._workers: list[tuple[MPProcess, mp.Queue[Update]]] = []
 
         self._crash_dir = crash_dir
+        self._target = target
         self._target_bytes = pickle.dumps(target)
 
         self._close_stderr = close_stderr or False
         self._close_stdout = close_stdout or False
         self._stat_frequency = stat_frequency
         self._max_crashes = max_crashes
         self._max_runs = max_runs
@@ -300,14 +289,15 @@
             seeds=seeds,
             adaptive=adaptive,
             max_input_size=max_input_size,
             max_modifications=max_modifications,
             max_insert_length=max_insert_length,
             file=state_file,
         )
+        self._simplify = simplify
 
         if load_crashes:
             self._load_crashes(regression=regression)
 
     def _load_crashes(self, regression: bool) -> None:
         """
         Load crash coverage from crash directory.
@@ -324,24 +314,24 @@
             if not error_file.is_file():
                 continue
             with error_file.open("br") as f:
                 try:
                     target(f.read())
                 except Exception as e:  # noqa: BLE001
                     if regression:
-                        changed = local_state.store_coverage(covered(e.__traceback__))
+                        changed = local_state.store_coverage(util.covered(e.__traceback__))
                         if changed:
                             logging.info(
                                 "\n========================================================================\n"
                                 "Testing %s:\n%s",
                                 error_file,
                                 traceback.format_exc(),
                             )
                     else:
-                        self._state.store_coverage(covered(e.__traceback__))
+                        self._state.store_coverage(util.covered(e.__traceback__))
                 else:
                     if regression:
                         logging.info("No error when testing %s", error_file)
 
         if regression:
             sys.exit(0)
 
@@ -372,20 +362,16 @@
         m.update(buf)
 
         if not self._crash_dir.exists():
             self._crash_dir.mkdir(parents=True)
             logging.info("Crash dir created (%s)", self._crash_dir)
 
         crash_path = self._crash_dir / (prefix + m.hexdigest())
-
-        with crash_path.open("wb") as f:
-            f.write(buf)
-        logging.info("sample was written to %s", crash_path)
-        if len(buf) < 200:
-            logging.info("sample = %s", buf.hex())
+        crash_path.write_bytes(buf)
+        logging.info(util.hexdump(title=f"Sample written to {crash_path.name}:", data=buf))
 
     def _initialize_process(self, wid: int) -> tuple[MPProcess, mp.Queue[Update]]:
         queue: mp.Queue[Update] = self._mp_ctx.Queue()
         result = self._mp_ctx.Process(
             target=worker,
             args=(
                 wid,
@@ -398,24 +384,31 @@
                 self._state,
             ),
         )
         result.start()
         return result, queue
 
     def _terminate_workers(self) -> None:
+        if not self._workers:
+            return
+
         self._result_queue.cancel_join_thread()
+
         for p, q in self._workers:
             q.cancel_join_thread()
             p.terminate()
             p.join(timeout=1)
 
+        del self._workers[:]
+
     def start(self) -> None:  # noqa: PLR0912
         start_time = time.time()
 
         self._workers = [self._initialize_process(wid=wid) for wid in range(self._num_workers)]
+        atexit.register(self._terminate_workers)
 
         logging.info(
             "START units: %d, workers: %d, seeds: %d",
             self._state.size,
             self._num_workers,
             self._state.num_seeds,
         )
@@ -485,8 +478,19 @@
 
             if (time.time() - self._last_stats_time) > self._stat_frequency:
                 self._log_stats("PULSE", self._state.total_coverage, self._state.size)
 
         self._state.save()
 
         self._terminate_workers()
-        sys.exit(0 if self._current_crashes == 0 else 1)
+
+        if self._current_crashes:
+            if self._simplify:
+                simplifier.Simp(
+                    crash_dir=self._crash_dir,
+                    target=self._target,
+                    output_dir=self._simplify,
+                    max_time=self._max_time,
+                ).simplify()
+            sys.exit(1)
+
+        sys.exit(0)
```

### Comparing `cobrafuzz-2.2.0/cobrafuzz/mutator.py` & `cobrafuzz-2.3.0/cobrafuzz/mutator.py`

 * *Files 8% similar despite different names*

```diff
@@ -3,57 +3,43 @@
 import ast
 import struct
 from typing import Callable, Optional
 
 from . import common, util
 
 
-class Params:
-    def __init__(self, **kwargs: util.ParamBase[int]):
-        self._data: dict[str, util.ParamBase[int]] = kwargs
-
-    def __getattr__(self, attr: str) -> util.ParamBase[int]:
-        if attr.startswith("_") or attr not in self._data:
-            raise AttributeError(f"'{self.__class__.__name__}' object has no attribute '{attr}'")
-        return self._data[attr]
-
-    def update(self, success: bool = False) -> None:
-        for rand in self._data.values():
-            rand.update(success=success)
-
-
 def _mutate_remove_range_of_bytes(
     res: bytearray,
-    rand: Params,
+    rand: util.Params,
     _inputs: Optional[util.AdaptiveChoiceBase[bytearray]] = None,
 ) -> None:
     if len(res) < 2:
         raise common.OutOfDataError
     assert isinstance(rand.length, util.AdaptiveRange)
     assert isinstance(rand.start, util.AdaptiveRange)
     length = rand.length.sample(1, len(res))
     util.remove(data=res, start=rand.start.sample(0, len(res) - length), length=length)
 
 
 def _mutate_insert_range_of_bytes(
     res: bytearray,
-    rand: Params,
+    rand: util.Params,
     _inputs: Optional[util.AdaptiveChoiceBase[bytearray]] = None,
 ) -> None:
     assert isinstance(rand.length, util.AdaptiveRange)
     assert isinstance(rand.start, util.AdaptiveRange)
     assert isinstance(rand.data, util.AdaptiveRange)
     assert isinstance(rand.max_length, util.Param)
     data = bytes(rand.data.sample(0, 255) for _ in range(rand.length.sample(1, rand.max_length())))
     util.insert(data=res, start=rand.start.sample(0, len(res)), data_to_insert=data)
 
 
 def _mutate_duplicate_range_of_bytes(
     res: bytearray,
-    rand: Params,
+    rand: util.Params,
     _inputs: Optional[util.AdaptiveChoiceBase[bytearray]] = None,
 ) -> None:
     if len(res) < 2:
         raise common.OutOfDataError
     assert isinstance(rand.src_pos, util.AdaptiveRange)
     assert isinstance(rand.dst_pos, util.AdaptiveRange)
     assert isinstance(rand.length, util.AdaptiveRange)
@@ -61,15 +47,15 @@
     src_pos = rand.src_pos.sample(0, dst_pos)
     length = rand.length.sample(1, len(res) - src_pos)
     util.insert(res, dst_pos, res[src_pos : src_pos + length])
 
 
 def _mutate_copy_range_of_bytes(
     res: bytearray,
-    rand: Params,
+    rand: util.Params,
     _inputs: Optional[util.AdaptiveChoiceBase[bytearray]] = None,
 ) -> None:
     if len(res) < 2:
         raise common.OutOfDataError
     assert isinstance(rand.src_pos, util.AdaptiveRange)
     assert isinstance(rand.dst_pos, util.AdaptiveRange)
     assert isinstance(rand.length, util.AdaptiveRange)
@@ -77,70 +63,70 @@
     src_pos = rand.src_pos.sample(0, dst_pos)
     length = rand.length.sample(1, min(len(res) - src_pos, len(res) - dst_pos))
     util.copy(res, src_pos, dst_pos, length)
 
 
 def _mutate_bit_flip(
     res: bytearray,
-    rand: Params,
+    rand: util.Params,
     _inputs: Optional[util.AdaptiveChoiceBase[bytearray]] = None,
 ) -> None:
     if len(res) < 1:
         raise common.OutOfDataError
     assert isinstance(rand.byte_pos, util.AdaptiveRange)
     assert isinstance(rand.bit_pos, util.AdaptiveRange)
     byte_pos = rand.byte_pos.sample(0, len(res) - 1)
     bit_pos = rand.bit_pos.sample(0, 7)
     res[byte_pos] ^= 1 << bit_pos
 
 
 def _mutate_flip_random_bits_of_random_byte(
     res: bytearray,
-    rand: Params,
+    rand: util.Params,
     _inputs: Optional[util.AdaptiveChoiceBase[bytearray]] = None,
 ) -> None:
     if len(res) < 1:
         raise common.OutOfDataError
     assert isinstance(rand.pos, util.AdaptiveRange)
     assert isinstance(rand.value, util.AdaptiveRange)
     pos = rand.pos.sample(0, len(res) - 1)
     res[pos] ^= rand.value.sample(0, 255)
 
 
 def _mutate_swap_two_bytes(
     res: bytearray,
-    rand: Params,
+    rand: util.Params,
     _inputs: Optional[util.AdaptiveChoiceBase[bytearray]] = None,
 ) -> None:
     if len(res) < 2:
         raise common.OutOfDataError
     assert isinstance(rand.first_pos, util.AdaptiveRange)
     assert isinstance(rand.second_pos, util.AdaptiveRange)
     first_pos = rand.first_pos.sample(0, len(res) - 1)
     second_pos = rand.second_pos.sample(0, len(res) - 1)
     res[first_pos], res[second_pos] = res[second_pos], res[first_pos]
 
 
 def _mutate_add_subtract_from_a_byte(
     res: bytearray,
-    rand: Params,
+    rand: util.Params,
     _inputs: Optional[util.AdaptiveChoiceBase[bytearray]] = None,
 ) -> None:
     if len(res) < 1:
         raise common.OutOfDataError
     assert isinstance(rand.pos, util.AdaptiveRange)
     assert isinstance(rand.value, util.AdaptiveRange)
     pos = rand.pos.sample(0, len(res) - 1)
     v_int = rand.value.sample(0, 255)
     res[pos] = (res[pos] + v_int) % 256
 
 
 def _mutate_add_subtract_from_a_uint16(
     res: bytearray,
-    rand: Params,
+    rand: util.Params,
     _inputs: Optional[util.AdaptiveChoiceBase[bytearray]] = None,
 ) -> None:
     if len(res) < 2:
         raise common.OutOfDataError
     assert isinstance(rand.pos, util.AdaptiveRange)
     assert isinstance(rand.value, util.AdaptiveRange)
     assert isinstance(rand.big_endian, util.AdaptiveRange)
@@ -150,15 +136,15 @@
     # TODO(#18): Implement version performing 16-bit addition
     res[pos] = (res[pos] + v[0]) % 256
     res[pos + 1] = (res[pos + 1] + v[1]) % 256
 
 
 def _mutate_add_subtract_from_a_uint32(
     res: bytearray,
-    rand: Params,
+    rand: util.Params,
     _inputs: Optional[util.AdaptiveChoiceBase[bytearray]] = None,
 ) -> None:
     if len(res) < 4:
         raise common.OutOfDataError
     assert isinstance(rand.pos, util.AdaptiveRange)
     assert isinstance(rand.value, util.AdaptiveRange)
     assert isinstance(rand.big_endian, util.AdaptiveRange)
@@ -169,15 +155,15 @@
     res[pos + 1] = (res[pos + 1] + v[1]) % 256
     res[pos + 2] = (res[pos + 2] + v[2]) % 256
     res[pos + 3] = (res[pos + 3] + v[3]) % 256
 
 
 def _mutate_add_subtract_from_a_uint64(
     res: bytearray,
-    rand: Params,
+    rand: util.Params,
     _inputs: Optional[util.AdaptiveChoiceBase[bytearray]] = None,
 ) -> None:
     if len(res) < 8:
         raise common.OutOfDataError
     assert isinstance(rand.pos, util.AdaptiveRange)
     assert isinstance(rand.value, util.AdaptiveRange)
     assert isinstance(rand.big_endian, util.AdaptiveRange)
@@ -192,28 +178,28 @@
     res[pos + 5] = (res[pos + 5] + v[5]) % 256
     res[pos + 6] = (res[pos + 6] + v[6]) % 256
     res[pos + 7] = (res[pos + 7] + v[7]) % 256
 
 
 def _mutate_replace_a_byte_with_an_interesting_value(
     res: bytearray,
-    rand: Params,
+    rand: util.Params,
     _inputs: Optional[util.AdaptiveChoiceBase[bytearray]] = None,
 ) -> None:
     if len(res) < 1:
         raise common.OutOfDataError
     assert isinstance(rand.pos, util.AdaptiveRange)
     assert isinstance(rand.interesting_8, util.AdaptiveChoiceBase)
     pos = rand.pos.sample(0, len(res) - 1)
     res[pos] = rand.interesting_8.sample()
 
 
 def _mutate_replace_an_uint16_with_an_interesting_value(
     res: bytearray,
-    rand: Params,
+    rand: util.Params,
     _inputs: Optional[util.AdaptiveChoiceBase[bytearray]] = None,
 ) -> None:
     if len(res) < 2:
         raise common.OutOfDataError
     assert isinstance(rand.pos, util.AdaptiveRange)
     assert isinstance(rand.big_endian, util.AdaptiveRange)
     assert isinstance(rand.interesting_16, util.AdaptiveChoiceBase)
@@ -222,15 +208,15 @@
     v = struct.pack(">H", v_int) if rand.big_endian.sample(0, 1) else struct.pack("<H", v_int)
     res[pos] = v[0] % 256
     res[pos + 1] = v[1] % 256
 
 
 def _mutate_replace_an_uint32_with_an_interesting_value(
     res: bytearray,
-    rand: Params,
+    rand: util.Params,
     _inputs: Optional[util.AdaptiveChoiceBase[bytearray]] = None,
 ) -> None:
     if len(res) < 4:
         raise common.OutOfDataError
     assert isinstance(rand.pos, util.AdaptiveRange)
     assert isinstance(rand.big_endian, util.AdaptiveRange)
     assert isinstance(rand.interesting_32, util.AdaptiveChoiceBase)
@@ -241,29 +227,29 @@
     res[pos + 1] = v[1] % 256
     res[pos + 2] = v[2] % 256
     res[pos + 3] = v[3] % 256
 
 
 def _mutate_replace_an_ascii_digit_with_another_digit(
     res: bytearray,
-    rand: Params,
+    rand: util.Params,
     _inputs: Optional[util.AdaptiveChoiceBase[bytearray]] = None,
 ) -> None:
     digits_present = [i for i in range(len(res)) if ord("0") <= res[i] <= ord("9")]
     if len(digits_present) < 1:
         raise common.OutOfDataError
     assert isinstance(rand.pos, util.AdaptiveRange)
     assert isinstance(rand.digits, util.AdaptiveChoiceBase)
     pos = rand.pos.sample(0, len(res) - 1)
     res[pos] = rand.digits.sample()
 
 
 def _mutate_splice(
     res: bytearray,
-    rand: Params,
+    rand: util.Params,
     inputs: Optional[util.AdaptiveChoiceBase[bytearray]] = None,
 ) -> None:
     if len(res) < 1:
         raise common.OutOfDataError
     assert inputs is not None
     right = inputs.sample()
     if len(right) < 1:
@@ -284,125 +270,128 @@
         adaptive: bool = True,
     ):
         self._inputs: util.AdaptiveChoiceBase[bytearray] = util.AdaptiveChoiceBase(population=None)
         self._max_input_size = max_input_size
         self._max_modifications = max_modifications
         self._modifications = util.AdaptiveRange(adaptive=adaptive)
         self._mutators: util.AdaptiveChoiceBase[
-            tuple[Callable[[bytearray, Params, util.AdaptiveChoiceBase[bytearray]], None], Params]
+            tuple[
+                Callable[[bytearray, util.Params, util.AdaptiveChoiceBase[bytearray]], None],
+                util.Params,
+            ]
         ] = util.AdaptiveChoiceBase(
             population=[
                 (
                     _mutate_remove_range_of_bytes,
-                    Params(
+                    util.Params(
                         length=util.AdaptiveRange(adaptive=adaptive),
                         start=util.AdaptiveRange(adaptive=adaptive),
                     ),
                 ),
                 (
                     _mutate_insert_range_of_bytes,
-                    Params(
+                    util.Params(
                         length=util.AdaptiveRange(adaptive=adaptive),
                         start=util.AdaptiveRange(adaptive=adaptive),
                         data=util.AdaptiveRange(adaptive=adaptive),
                         max_length=util.Param(max_insert_length),
                     ),
                 ),
                 (
                     _mutate_duplicate_range_of_bytes,
-                    Params(
+                    util.Params(
                         src_pos=util.AdaptiveRange(adaptive=adaptive),
                         dst_pos=util.AdaptiveRange(adaptive=adaptive),
                         length=util.AdaptiveRange(adaptive=adaptive),
                     ),
                 ),
                 (
                     _mutate_copy_range_of_bytes,
-                    Params(
+                    util.Params(
                         src_pos=util.AdaptiveRange(adaptive=adaptive),
                         dst_pos=util.AdaptiveRange(adaptive=adaptive),
                         length=util.AdaptiveRange(adaptive=adaptive),
                     ),
                 ),
                 (
                     _mutate_bit_flip,
-                    Params(
+                    util.Params(
                         byte_pos=util.AdaptiveRange(adaptive=adaptive),
                         bit_pos=util.AdaptiveRange(adaptive=adaptive),
                     ),
                 ),
                 (
                     _mutate_flip_random_bits_of_random_byte,
-                    Params(
+                    util.Params(
                         pos=util.AdaptiveRange(adaptive=adaptive),
                         value=util.AdaptiveRange(adaptive=adaptive),
                     ),
                 ),
                 (
                     _mutate_swap_two_bytes,
-                    Params(
+                    util.Params(
                         first_pos=util.AdaptiveRange(adaptive=adaptive),
                         second_pos=util.AdaptiveRange(adaptive=adaptive),
                     ),
                 ),
                 (
                     _mutate_add_subtract_from_a_byte,
-                    Params(
+                    util.Params(
                         pos=util.AdaptiveRange(adaptive=adaptive),
                         value=util.AdaptiveRange(adaptive=adaptive),
                     ),
                 ),
                 (
                     _mutate_add_subtract_from_a_uint16,
-                    Params(
+                    util.Params(
                         pos=util.AdaptiveRange(adaptive=adaptive),
                         value=util.AdaptiveRange(adaptive=adaptive),
                         big_endian=util.AdaptiveRange(adaptive=adaptive),
                     ),
                 ),
                 (
                     _mutate_add_subtract_from_a_uint32,
-                    Params(
+                    util.Params(
                         pos=util.AdaptiveRange(adaptive=adaptive),
                         value=util.AdaptiveRange(adaptive=adaptive),
                         big_endian=util.AdaptiveRange(adaptive=adaptive),
                     ),
                 ),
                 (
                     _mutate_add_subtract_from_a_uint64,
-                    Params(
+                    util.Params(
                         pos=util.AdaptiveRange(adaptive=adaptive),
                         value=util.AdaptiveRange(adaptive=adaptive),
                         big_endian=util.AdaptiveRange(adaptive=adaptive),
                     ),
                 ),
                 (
                     _mutate_replace_a_byte_with_an_interesting_value,
-                    Params(
+                    util.Params(
                         pos=util.AdaptiveRange(adaptive=adaptive),
                         interesting_8=util.AdaptiveChoiceBase(
                             population=[1, 1, 16, 32, 64, 100, 127, 128, 129, 255],
                             adaptive=adaptive,
                         ),
                     ),
                 ),
                 (
                     _mutate_replace_an_uint16_with_an_interesting_value,
-                    Params(
+                    util.Params(
                         pos=util.AdaptiveRange(adaptive=adaptive),
                         interesting_16=util.AdaptiveChoiceBase(
                             population=[0, 128, 255, 256, 512, 1000, 1024, 4096, 32767, 65535],
                             adaptive=adaptive,
                         ),
                         big_endian=util.AdaptiveRange(adaptive=adaptive),
                     ),
                 ),
                 (
                     _mutate_replace_an_uint32_with_an_interesting_value,
-                    Params(
+                    util.Params(
                         pos=util.AdaptiveRange(adaptive=adaptive),
                         interesting_32=util.AdaptiveChoiceBase(
                             population=[
                                 0,
                                 1,
                                 32768,
                                 65535,
@@ -414,34 +403,34 @@
                             adaptive=adaptive,
                         ),
                         big_endian=util.AdaptiveRange(adaptive=adaptive),
                     ),
                 ),
                 (
                     _mutate_replace_an_ascii_digit_with_another_digit,
-                    Params(
+                    util.Params(
                         pos=util.AdaptiveRange(adaptive=adaptive),
                         digits=util.AdaptiveChoiceBase(
                             population=[
                                 ord(i) for i in ("0", "1", "2", "3", "4", "5", "6", "7", "8", "9")
                             ],
                             adaptive=adaptive,
                         ),
                     ),
                 ),
                 (
                     _mutate_splice,
-                    Params(
+                    util.Params(
                         left_pos=util.AdaptiveRange(adaptive=adaptive),
                         right_pos=util.AdaptiveRange(adaptive=adaptive),
                     ),
                 ),
             ],
         )
-        self._last_rands: Optional[Params] = None
+        self._last_rands: Optional[util.Params] = None
 
     def _mutate(self, buf: bytearray) -> bytearray:
         res = buf[:]
         nm = self._modifications.sample(1, self._max_modifications)
         while nm:
             modify, self._last_rands = self._mutators.sample()
             try:
```

### Comparing `cobrafuzz-2.2.0/cobrafuzz/state.py` & `cobrafuzz-2.3.0/cobrafuzz/state.py`

 * *Files identical despite different names*

### Comparing `cobrafuzz-2.2.0/cobrafuzz/tracer.py` & `cobrafuzz-2.3.0/cobrafuzz/tracer.py`

 * *Files identical despite different names*

### Comparing `cobrafuzz-2.2.0/cobrafuzz/util.py` & `cobrafuzz-2.3.0/cobrafuzz/util.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,12 +1,15 @@
 from __future__ import annotations
 
+import logging
 import random
 from abc import abstractmethod
-from typing import Generator, Generic, Optional, TypeVar
+from contextlib import contextmanager
+from types import TracebackType
+from typing import Generator, Generic, Iterator, Optional, TypeVar
 
 from . import common
 
 PopulationType = TypeVar("PopulationType")
 
 
 class ParamBase(Generic[PopulationType]):
@@ -22,14 +25,28 @@
     def __call__(self) -> int:
         return self._value
 
     def update(self, success: bool = False) -> None:
         pass
 
 
+class Params:
+    def __init__(self, **kwargs: ParamBase[int]):
+        self._data: dict[str, ParamBase[int]] = kwargs
+
+    def __getattr__(self, attr: str) -> ParamBase[int]:
+        if attr.startswith("_") or attr not in self._data:
+            raise AttributeError(f"'{self.__class__.__name__}' object has no attribute '{attr}'")
+        return self._data[attr]
+
+    def update(self, success: bool = False) -> None:
+        for rand in self._data.values():
+            rand.update(success=success)
+
+
 class AdaptiveRandBase(ParamBase[PopulationType]):
     def _succeed(self) -> None:
         raise NotImplementedError
 
     def _fail(self) -> None:
         raise NotImplementedError
 
@@ -113,14 +130,16 @@
 
     def append(self, element: PopulationType) -> None:
         self._population.append(element)
         if self._distribution is not None:
             self._distribution.append(1)
 
     def sample(self) -> PopulationType:
+        if len(self._population) < 1:
+            raise common.OutOfBoundsError("No samples")
         if self._distribution is None:
             return random.choice(self._population)  # noqa: S311
         self._last = random.choices(self._population, self._distribution, k=1)[0]  # noqa: S311
         return self._last
 
 
 def copy(
@@ -184,7 +203,47 @@
     data: bytearray to modify.
     start: Position where to insert new data.
     data_to_insert: bytearray to insert.
     """
     if start > len(data):
         raise common.OutOfBoundsError("Start out of range")
     data[:] = data[:start] + data_to_insert + data[start:]
+
+
+def covered(
+    t: Optional[TracebackType],
+    skip_first_n: int = 0,
+) -> set[tuple[Optional[str], Optional[int], str, int]]:
+    """Construct coverage information from exception traceback."""
+
+    prev_line: Optional[int] = None
+    prev_file: Optional[str] = None
+    result: list[tuple[Optional[str], Optional[int], str, int]] = []
+    tb: Optional[TracebackType] = t
+    while tb:
+        result.append((prev_file, prev_line, tb.tb_frame.f_code.co_filename, tb.tb_lineno))
+        prev_line = tb.tb_lineno
+        prev_file = tb.tb_frame.f_code.co_filename
+        tb = tb.tb_next
+    return set(result[skip_first_n:])
+
+
+@contextmanager
+def disable_logging() -> Iterator[None]:
+    previous_level = logging.root.manager.disable
+    logging.disable(logging.CRITICAL)
+
+    try:
+        yield
+    finally:
+        logging.disable(previous_level)
+
+
+def hexdump(title: str, data: bytes) -> str:
+    length = 16
+    result = [title]
+    for i in range(0, len(data), length):
+        chunk = data[i : i + length]
+        hex_chunk = " ".join(f"{b:02x}" for b in chunk)
+        ascii_chunk = "".join(chr(b) if 32 <= b < 127 else "." for b in chunk)
+        result.append(f"{i:08x}: {hex_chunk:<{length*3}} {ascii_chunk}")
+    return "\n".join(result)
```

### Comparing `cobrafuzz-2.2.0/cobrafuzz.egg-info/PKG-INFO` & `cobrafuzz-2.3.0/cobrafuzz.egg-info/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: cobrafuzz
-Version: 2.2.0
+Version: 2.3.0
 Summary: Coverage-guided fuzz testing for Python
 Author-email: Alexander Senier <mail@senier.net>
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Operating System :: OS Independent
 Classifier: Topic :: Software Development :: Testing
 Requires-Python: >=3.8.0
@@ -21,14 +21,15 @@
 Requires-Dist: isort==5.13.2; extra == "devel"
 Requires-Dist: mypy<1.8.0; extra == "devel"
 Requires-Dist: plotly==5.19.0; extra == "devel"
 Requires-Dist: purl==1.6; extra == "devel"
 Requires-Dist: pytest==7.4.4; extra == "devel"
 Requires-Dist: pytest-cov==4.1.0; extra == "devel"
 Requires-Dist: pytest-xdist==3.5.0; extra == "devel"
+Requires-Dist: python-dateutil==2.9.0; extra == "devel"
 Requires-Dist: python-kacl==0.4.6; extra == "devel"
 Requires-Dist: requests==2.31.0; extra == "devel"
 Requires-Dist: ruff==0.1.13; extra == "devel"
 Requires-Dist: scipy<1.11; python_version < "3.9" and extra == "devel"
 Requires-Dist: scipy==1.11.4; python_version >= "3.9" and extra == "devel"
 Requires-Dist: types-requests==2.31.0.20240125; extra == "devel"
 Requires-Dist: vulture==2.11; extra == "devel"
@@ -49,30 +50,30 @@
 ## Usage
 
 ### Fuzz Target
 
 The first step is to implement a function to be fuzz-tested, also called a fuzz target.
 Here is an example of a simple fuzz target for the built-in `html` module
 
-```python
-from html.parser import HTMLParser
+```python,examples/fuzz_htmlparser/fuzz.py
 from cobrafuzz.main import CobraFuzz
 
 
 @CobraFuzz
-def fuzz(buf):
+def fuzz(buf: bytes) -> None:
+    from html.parser import HTMLParser
+
     try:
-        string = buf.decode("ascii")
         parser = HTMLParser()
-        parser.feed(string)
+        parser.feed(buf.decode("ascii"))
     except UnicodeDecodeError:
         pass
 
 
-if __name__ == '__main__':
+if __name__ == "__main__":
     fuzz()
 ```
 
 Features of a fuzz target:
 
 * `fuzz()` will call the fuzz target in an infinite loop with random data generated by the coverage-guided algorithm. The data is passed to the target in a separate process through the `buf` parameter.
 * The function must catch and ignore any expected exceptions that arise when passing invalid input to the tested program.
@@ -84,15 +85,15 @@
 
 The next step is to download CobraFuzz and then run the fuzzer:
 
 ```console
 $ pip install cobrafuzz
 [...]
 
-$ python examples/htmlparser/fuzz.py --crash-dir results --max-crashes 1
+$ python examples/fuzz_htmlparser/fuzz.py --crash-dir results fuzz --max-crashes 1
 #0 READ units: 1 workers: 7 seeds: 1
 #1 NEW     cov: 279 corp: 1 exec/s: 89 crashes: 0
 #5 NEW     cov: 366 corp: 2 exec/s: 299 crashes: 0
 #7 NEW     cov: 401 corp: 3 exec/s: 3124 crashes: 0
 [...]
 #154382 NEW     cov: 1086 corp: 50 exec/s: 22835 crashes: 0
 #156521 NEW     cov: 1092 corp: 51 exec/s: 2797 crashes: 0
```

### Comparing `cobrafuzz-2.2.0/pyproject.toml` & `cobrafuzz-2.3.0/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ['setuptools>=64', 'wheel']
 build-backend = 'setuptools.build_meta'
 
 [project]
 name = "cobrafuzz"
-version = "2.2.0"
+version = "2.3.0"
 authors = [
     {name = "Alexander Senier", email = "mail@senier.net"}
 ]
 description = "Coverage-guided fuzz testing for Python"
 readme = "README.md"
 classifiers = [
     "Programming Language :: Python :: 3",
@@ -32,14 +32,15 @@
     "isort ==5.13.2",
     "mypy <1.8.0",
     "plotly ==5.19.0",
     "purl ==1.6",
     "pytest ==7.4.4",
     "pytest-cov ==4.1.0",
     "pytest-xdist ==3.5.0",
+    "python-dateutil ==2.9.0",
     "python-kacl ==0.4.6",
     "requests ==2.31.0",
     "ruff ==0.1.13",
     "scipy <1.11; python_version<'3.9'",
     "scipy ==1.11.4; python_version>='3.9'",
     "types-requests ==2.31.0.20240125",
     "vulture ==2.11",
```

