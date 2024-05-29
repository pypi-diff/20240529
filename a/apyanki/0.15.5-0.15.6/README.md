# Comparing `tmp/apyanki-0.15.5.tar.gz` & `tmp/apyanki-0.15.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "apyanki-0.15.5.tar", max compression
+gzip compressed data, was "apyanki-0.15.6.tar", max compression
```

## Comparing `apyanki-0.15.5.tar` & `apyanki-0.15.6.tar`

### file list

```diff
@@ -1,13 +1,13 @@
--rw-r--r--   0        0        0     1075 2023-06-03 19:56:02.857177 apyanki-0.15.5/LICENSE.md
--rw-r--r--   0        0        0    11250 2024-04-19 20:43:04.288990 apyanki-0.15.5/README.md
--rw-r--r--   0        0        0     1561 2024-05-28 21:29:51.750790 apyanki-0.15.5/pyproject.toml
--rw-r--r--   0        0        0      362 2024-04-11 17:02:39.255040 apyanki-0.15.5/src/apyanki/__init__.py
--rw-r--r--   0        0        0    16926 2024-05-28 21:27:16.653454 apyanki-0.15.5/src/apyanki/anki.py
--rw-r--r--   0        0        0     1964 2024-04-11 17:02:57.515160 apyanki-0.15.5/src/apyanki/cards.py
--rw-r--r--   0        0        0    14640 2024-04-11 17:03:04.491873 apyanki-0.15.5/src/apyanki/cli.py
--rw-r--r--   0        0        0     2064 2024-04-19 20:39:20.334116 apyanki-0.15.5/src/apyanki/config.py
--rw-r--r--   0        0        0     1259 2024-03-22 19:17:12.627164 apyanki-0.15.5/src/apyanki/console.py
--rw-r--r--   0        0        0     9169 2024-04-19 20:40:01.254397 apyanki-0.15.5/src/apyanki/fields.py
--rw-r--r--   0        0        0    23313 2024-05-28 21:27:17.533459 apyanki-0.15.5/src/apyanki/note.py
--rw-r--r--   0        0        0     3051 2024-05-28 21:27:15.306780 apyanki-0.15.5/src/apyanki/utilities.py
--rw-r--r--   0        0        0    12312 1970-01-01 00:00:00.000000 apyanki-0.15.5/PKG-INFO
+-rw-r--r--   0        0        0     1075 2023-06-03 19:56:02.857177 apyanki-0.15.6/LICENSE.md
+-rw-r--r--   0        0        0    11250 2024-04-19 20:43:04.288990 apyanki-0.15.6/README.md
+-rw-r--r--   0        0        0     1561 2024-05-29 19:50:25.723303 apyanki-0.15.6/pyproject.toml
+-rw-r--r--   0        0        0      362 2024-04-11 17:02:39.255040 apyanki-0.15.6/src/apyanki/__init__.py
+-rw-r--r--   0        0        0    16926 2024-05-28 21:27:16.653454 apyanki-0.15.6/src/apyanki/anki.py
+-rw-r--r--   0        0        0     1964 2024-04-11 17:02:57.515160 apyanki-0.15.6/src/apyanki/cards.py
+-rw-r--r--   0        0        0    14650 2024-05-29 19:46:44.352978 apyanki-0.15.6/src/apyanki/cli.py
+-rw-r--r--   0        0        0     2064 2024-04-19 20:39:20.334116 apyanki-0.15.6/src/apyanki/config.py
+-rw-r--r--   0        0        0     1259 2024-03-22 19:17:12.627164 apyanki-0.15.6/src/apyanki/console.py
+-rw-r--r--   0        0        0     9169 2024-04-19 20:40:01.254397 apyanki-0.15.6/src/apyanki/fields.py
+-rw-r--r--   0        0        0    23306 2024-05-29 19:48:20.600896 apyanki-0.15.6/src/apyanki/note.py
+-rw-r--r--   0        0        0     3051 2024-05-28 21:27:15.306780 apyanki-0.15.6/src/apyanki/utilities.py
+-rw-r--r--   0        0        0    12312 1970-01-01 00:00:00.000000 apyanki-0.15.6/PKG-INFO
```

### Comparing `apyanki-0.15.5/LICENSE.md` & `apyanki-0.15.6/LICENSE.md`

 * *Files identical despite different names*

### Comparing `apyanki-0.15.5/README.md` & `apyanki-0.15.6/README.md`

 * *Files identical despite different names*

### Comparing `apyanki-0.15.5/pyproject.toml` & `apyanki-0.15.6/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "apyanki"
-version = "0.15.5"
+version = "0.15.6"
 description = "CLI script for interacting with local Anki collection"
 authors = ["Karl Yngve Lervåg <karl.yngve@lervag.net>"]
 readme = "README.md"
 classifiers = [
     "Programming Language :: Python :: 3",
     "License :: OSI Approved :: MIT License",
     "Operating System :: OS Independent",
```

### Comparing `apyanki-0.15.5/src/apyanki/anki.py` & `apyanki-0.15.6/src/apyanki/anki.py`

 * *Files identical despite different names*

### Comparing `apyanki-0.15.5/src/apyanki/cards.py` & `apyanki-0.15.6/src/apyanki/cards.py`

 * *Files identical despite different names*

### Comparing `apyanki-0.15.5/src/apyanki/cli.py` & `apyanki-0.15.6/src/apyanki/cli.py`

 * *Files 1% similar despite different names*

```diff
@@ -32,19 +32,19 @@
     (https://docs.ankiweb.net/files.html#file-locations).
 
     A few sub commands will open an editor for input. Vim is used by default.
     The input is parsed when one saves and quits. To abort, one should exit the
     editor with a non-zero exit code. In Vim, one can do this with the `:cquit`
     command.
 
-    One may specify a different editor with the EDITOR environment variable.
+    One may specify a different editor with the VISUAL or EDITOR environment variable.
     For example, to use emacs one can add this to one's `~/.bashrc` (or similar)
     file:
 
-        export EDITOR=emacs
+        export VISUAL=emacs
 
     Note: Use `apy subcmd --help` to get detailed help for a given subcommand.
     """
     if version:
         console.print(f"apy {__version__}")
         sys.exit()
```

### Comparing `apyanki-0.15.5/src/apyanki/config.py` & `apyanki-0.15.6/src/apyanki/config.py`

 * *Files identical despite different names*

### Comparing `apyanki-0.15.5/src/apyanki/console.py` & `apyanki-0.15.6/src/apyanki/console.py`

 * *Files identical despite different names*

### Comparing `apyanki-0.15.5/src/apyanki/fields.py` & `apyanki-0.15.6/src/apyanki/fields.py`

 * *Files identical despite different names*

### Comparing `apyanki-0.15.5/src/apyanki/note.py` & `apyanki-0.15.6/src/apyanki/note.py`

 * *Files 0% similar despite different names*

```diff
@@ -250,15 +250,15 @@
 
         models = sorted(self.a.model_names)  # type: ignore[has-type]
         while True:
             console.clear()
             console.print("Please choose new model:")
             for n, m in enumerate(models):
                 console.print(f"  {n+1}: {m}")
-            index: int = console.prompt_int(">>> ", prompt_suffix="") - 1
+            index: int = console.prompt_int(">>> ", suffix="") - 1
             try:
                 new_model = models[index]
                 self.a.set_model(new_model)
                 model = self.a.get_model(new_model)
                 if not model:
                     continue
             except IndexError:
```

### Comparing `apyanki-0.15.5/src/apyanki/utilities.py` & `apyanki-0.15.6/src/apyanki/utilities.py`

 * *Files identical despite different names*

### Comparing `apyanki-0.15.5/PKG-INFO` & `apyanki-0.15.6/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: apyanki
-Version: 0.15.5
+Version: 0.15.6
 Summary: CLI script for interacting with local Anki collection
 Home-page: https://github.com/lervag/apy
 Author: Karl Yngve Lervåg
 Author-email: karl.yngve@lervag.net
 Requires-Python: >=3.9,<4.0
 Classifier: Environment :: Console
 Classifier: License :: OSI Approved :: MIT License
```

