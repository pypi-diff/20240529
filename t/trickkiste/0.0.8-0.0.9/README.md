# Comparing `tmp/trickkiste-0.0.8.tar.gz` & `tmp/trickkiste-0.0.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "trickkiste-0.0.8.tar", max compression
+gzip compressed data, was "trickkiste-0.0.9.tar", max compression
```

## Comparing `trickkiste-0.0.8.tar` & `trickkiste-0.0.9.tar`

### file list

```diff
@@ -1,12 +1,12 @@
--rw-r--r--   0        0        0      676 2023-12-10 05:33:15.492574 trickkiste-0.0.8/Readme.md
--rw-r--r--   0        0        0     1563 2024-03-20 15:20:10.709973 trickkiste-0.0.8/pyproject.toml
--rw-r--r--   0        0        0        0 2024-01-11 10:54:02.708905 trickkiste-0.0.8/trickkiste/__init__.py
--rw-r--r--   0        0        0       42 2024-01-11 10:54:02.712905 trickkiste-0.0.8/trickkiste/base_tui_app.css
--rw-r--r--   0        0        0     2982 2024-01-11 10:54:02.712905 trickkiste-0.0.8/trickkiste/base_tui_app.py
--rwxr-xr-x   0        0        0      978 2024-02-08 08:51:43.258359 trickkiste-0.0.8/trickkiste/examples/fancylogging.py
--rwxr-xr-x   0        0        0     1785 2024-01-11 10:54:02.716905 trickkiste-0.0.8/trickkiste/examples/fancytui.py
--rw-r--r--   0        0        0     3588 2024-02-08 08:49:35.260768 trickkiste-0.0.8/trickkiste/logging_helper.py
--rw-r--r--   0        0        0     5678 2024-03-20 15:13:42.588026 trickkiste-0.0.8/trickkiste/misc.py
--rw-r--r--   0        0        0        0 2024-01-11 10:54:02.716905 trickkiste-0.0.8/trickkiste/py.typed
--rwxr-xr-x   0        0        0     2293 2024-01-11 10:54:02.716905 trickkiste-0.0.8/trickkiste/std_suppress.py
--rw-r--r--   0        0        0     1188 1970-01-01 00:00:00.000000 trickkiste-0.0.8/PKG-INFO
+-rw-r--r--   0        0        0      676 2023-12-10 05:33:15.492574 trickkiste-0.0.9/Readme.md
+-rw-r--r--   0        0        0     1563 2024-04-17 06:54:02.806553 trickkiste-0.0.9/pyproject.toml
+-rw-r--r--   0        0        0        0 2024-01-11 10:54:02.708905 trickkiste-0.0.9/trickkiste/__init__.py
+-rw-r--r--   0        0        0       42 2024-01-11 10:54:02.712905 trickkiste-0.0.9/trickkiste/base_tui_app.css
+-rw-r--r--   0        0        0     3638 2024-04-17 06:52:34.021628 trickkiste-0.0.9/trickkiste/base_tui_app.py
+-rwxr-xr-x   0        0        0      978 2024-02-08 08:51:43.258359 trickkiste-0.0.9/trickkiste/examples/fancylogging.py
+-rwxr-xr-x   0        0        0     1785 2024-01-11 10:54:02.716905 trickkiste-0.0.9/trickkiste/examples/fancytui.py
+-rw-r--r--   0        0        0     3588 2024-02-08 08:49:35.260768 trickkiste-0.0.9/trickkiste/logging_helper.py
+-rw-r--r--   0        0        0     5678 2024-03-20 15:13:42.588026 trickkiste-0.0.9/trickkiste/misc.py
+-rw-r--r--   0        0        0        0 2024-01-11 10:54:02.716905 trickkiste-0.0.9/trickkiste/py.typed
+-rwxr-xr-x   0        0        0     2293 2024-01-11 10:54:02.716905 trickkiste-0.0.9/trickkiste/std_suppress.py
+-rw-r--r--   0        0        0     1188 1970-01-01 00:00:00.000000 trickkiste-0.0.9/PKG-INFO
```

### Comparing `trickkiste-0.0.8/Readme.md` & `trickkiste-0.0.9/Readme.md`

 * *Files identical despite different names*

### Comparing `trickkiste-0.0.8/pyproject.toml` & `trickkiste-0.0.9/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "trickkiste"
-version = "0.0.8"
+version = "0.0.9"
 description = "Random useful stuff"
 authors = ["Frans Fürst <frans.fuerst+gitlab@protonmail.com>"]
 repository = "https://projects.om-office.de/frans/trickkiste.git"
 readme = "Readme.md"
 packages = [
   {include = "trickkiste"},
   # {include = "trickkiste/py.typed"},
```

### Comparing `trickkiste-0.0.8/trickkiste/base_tui_app.py` & `trickkiste-0.0.9/trickkiste/base_tui_app.py`

 * *Files 20% similar despite different names*

```diff
@@ -22,16 +22,16 @@
     """Returns the logger instance to use here"""
     return logging.getLogger("trickkiste.base_app")
 
 
 class RichLogHandler(RichHandler):
     """Redirects rich.RichHanlder capabilities to a textual.RichLog"""
 
-    def __init__(self, widget: RichLog):
-        super().__init__(show_path=False, markup=True, show_time=False)
+    def __init__(self, widget: RichLog, level: int = logging.INFO):
+        super().__init__(show_path=False, markup=True, show_time=False, level=level)
         self.widget: RichLog = widget
 
     def emit(self, record: logging.LogRecord) -> None:
         record.args = record.args and tuple(
             markup_escape(arg) if isinstance(arg, str) else arg for arg in record.args
         )
         record.msg = markup_escape(record.msg)
@@ -58,14 +58,15 @@
 
     CSS_PATH = Path(__file__).parent / "base_tui_app.css"
 
     def __init__(self, logger_funcname: bool = True) -> None:
         super().__init__()
         self._richlog = LockingRichLog()
         self._logger_funcname = logger_funcname
+        self._log_level: int | str = logging.INFO
 
     def add_default_arguments(self, parser: ArgumentParser) -> None:
         """Adds arguments to @parser we need in every app"""
         parser.add_argument(
             "--log-level",
             "-l",
             type=str.upper,
@@ -83,13 +84,28 @@
         optional_funcname = "│ [grey53]%(funcName)-32s[/] " if self._logger_funcname else ""
         handler.setFormatter(
             logging.Formatter(
                 f"│ %(asctime)s {optional_funcname}│ [bold white]%(message)s[/]",
                 datefmt="%Y-%m-%d %H:%M:%S",
             )
         )
+        self.set_log_level(self._log_level)
 
     def execute(self) -> None:
         """Wrapper for async run and optional cleanup if provided"""
         asyncio.run(self.run_async())
         if hasattr(self, "cleanup"):
             self.cleanup()
+
+    def set_log_level(self, level: int | str) -> None:
+        """Sets the overall log level for internal log console"""
+
+        # log level for everything
+        logging.getLogger().setLevel(logging.DEBUG if level == "ALL_DEBUG" else logging.WARNING)
+
+        # log level for provided @logger
+        used_level = getattr(logging, level.split("_")[-1]) if isinstance(level, str) else level
+
+        for handler in logging.getLogger().handlers:
+            handler.setLevel(used_level)
+
+        self._log_level = level
```

### Comparing `trickkiste-0.0.8/trickkiste/examples/fancylogging.py` & `trickkiste-0.0.9/trickkiste/examples/fancylogging.py`

 * *Files identical despite different names*

### Comparing `trickkiste-0.0.8/trickkiste/examples/fancytui.py` & `trickkiste-0.0.9/trickkiste/examples/fancytui.py`

 * *Files identical despite different names*

### Comparing `trickkiste-0.0.8/trickkiste/logging_helper.py` & `trickkiste-0.0.9/trickkiste/logging_helper.py`

 * *Files identical despite different names*

### Comparing `trickkiste-0.0.8/trickkiste/misc.py` & `trickkiste-0.0.9/trickkiste/misc.py`

 * *Files identical despite different names*

### Comparing `trickkiste-0.0.8/trickkiste/std_suppress.py` & `trickkiste-0.0.9/trickkiste/std_suppress.py`

 * *Files identical despite different names*

### Comparing `trickkiste-0.0.8/PKG-INFO` & `trickkiste-0.0.9/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: trickkiste
-Version: 0.0.8
+Version: 0.0.9
 Summary: Random useful stuff
 Home-page: https://projects.om-office.de/frans/trickkiste.git
 Author: Frans Fürst
 Author-email: frans.fuerst+gitlab@protonmail.com
 Requires-Python: >=3.10.4,<4
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.11
```

