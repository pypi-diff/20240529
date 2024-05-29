# Comparing `tmp/apyanki-0.15.4.tar.gz` & `tmp/apyanki-0.15.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "apyanki-0.15.4.tar", max compression
+gzip compressed data, was "apyanki-0.15.5.tar", max compression
```

## Comparing `apyanki-0.15.4.tar` & `apyanki-0.15.5.tar`

### file list

```diff
@@ -1,13 +1,13 @@
--rw-r--r--   0        0        0     1075 2023-06-03 19:56:02.857177 apyanki-0.15.4/LICENSE.md
--rw-r--r--   0        0        0    11250 2024-04-19 20:43:04.288990 apyanki-0.15.4/README.md
--rw-r--r--   0        0        0     1561 2024-05-21 20:23:03.331872 apyanki-0.15.4/pyproject.toml
--rw-r--r--   0        0        0      362 2024-04-11 17:02:39.255040 apyanki-0.15.4/src/apyanki/__init__.py
--rw-r--r--   0        0        0    16917 2024-04-19 20:21:19.756773 apyanki-0.15.4/src/apyanki/anki.py
--rw-r--r--   0        0        0     1964 2024-04-11 17:02:57.515160 apyanki-0.15.4/src/apyanki/cards.py
--rw-r--r--   0        0        0    14640 2024-04-11 17:03:04.491873 apyanki-0.15.4/src/apyanki/cli.py
--rw-r--r--   0        0        0     2064 2024-04-19 20:39:20.334116 apyanki-0.15.4/src/apyanki/config.py
--rw-r--r--   0        0        0     1259 2024-03-22 19:17:12.627164 apyanki-0.15.4/src/apyanki/console.py
--rw-r--r--   0        0        0     9169 2024-04-19 20:40:01.254397 apyanki-0.15.4/src/apyanki/fields.py
--rw-r--r--   0        0        0    23307 2024-04-11 17:08:37.727403 apyanki-0.15.4/src/apyanki/note.py
--rw-r--r--   0        0        0     2987 2024-04-11 17:11:39.668604 apyanki-0.15.4/src/apyanki/utilities.py
--rw-r--r--   0        0        0    12312 1970-01-01 00:00:00.000000 apyanki-0.15.4/PKG-INFO
+-rw-r--r--   0        0        0     1075 2023-06-03 19:56:02.857177 apyanki-0.15.5/LICENSE.md
+-rw-r--r--   0        0        0    11250 2024-04-19 20:43:04.288990 apyanki-0.15.5/README.md
+-rw-r--r--   0        0        0     1561 2024-05-28 21:29:51.750790 apyanki-0.15.5/pyproject.toml
+-rw-r--r--   0        0        0      362 2024-04-11 17:02:39.255040 apyanki-0.15.5/src/apyanki/__init__.py
+-rw-r--r--   0        0        0    16926 2024-05-28 21:27:16.653454 apyanki-0.15.5/src/apyanki/anki.py
+-rw-r--r--   0        0        0     1964 2024-04-11 17:02:57.515160 apyanki-0.15.5/src/apyanki/cards.py
+-rw-r--r--   0        0        0    14640 2024-04-11 17:03:04.491873 apyanki-0.15.5/src/apyanki/cli.py
+-rw-r--r--   0        0        0     2064 2024-04-19 20:39:20.334116 apyanki-0.15.5/src/apyanki/config.py
+-rw-r--r--   0        0        0     1259 2024-03-22 19:17:12.627164 apyanki-0.15.5/src/apyanki/console.py
+-rw-r--r--   0        0        0     9169 2024-04-19 20:40:01.254397 apyanki-0.15.5/src/apyanki/fields.py
+-rw-r--r--   0        0        0    23313 2024-05-28 21:27:17.533459 apyanki-0.15.5/src/apyanki/note.py
+-rw-r--r--   0        0        0     3051 2024-05-28 21:27:15.306780 apyanki-0.15.5/src/apyanki/utilities.py
+-rw-r--r--   0        0        0    12312 1970-01-01 00:00:00.000000 apyanki-0.15.5/PKG-INFO
```

### Comparing `apyanki-0.15.4/LICENSE.md` & `apyanki-0.15.5/LICENSE.md`

 * *Files identical despite different names*

### Comparing `apyanki-0.15.4/README.md` & `apyanki-0.15.5/README.md`

 * *Files identical despite different names*

### Comparing `apyanki-0.15.4/pyproject.toml` & `apyanki-0.15.5/pyproject.toml`

 * *Files 7% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "apyanki"
-version = "0.15.4"
+version = "0.15.5"
 description = "CLI script for interacting with local Anki collection"
 authors = ["Karl Yngve Lervåg <karl.yngve@lervag.net>"]
 readme = "README.md"
 classifiers = [
     "Programming Language :: Python :: 3",
     "License :: OSI Approved :: MIT License",
     "Operating System :: OS Independent",
```

### Comparing `apyanki-0.15.4/src/apyanki/anki.py` & `apyanki-0.15.5/src/apyanki/anki.py`

 * *Files 0% similar despite different names*

```diff
@@ -14,15 +14,15 @@
 from rich.progress import Progress, SpinnerColumn, TextColumn
 from rich.table import Table
 
 from apyanki import cards
 from apyanki.config import cfg
 from apyanki.console import console
 from apyanki.note import Note, NoteData, markdown_file_to_notes
-from apyanki.utilities import cd, choose, editor, suppress_stdout
+from apyanki.utilities import cd, choose, edit_file, suppress_stdout
 
 if TYPE_CHECKING:
     from anki.notes import NoteId
     from anki.models import NotetypeDict
     from anki.cards import CardId
 
 
@@ -364,15 +364,15 @@
 
         with tempfile.NamedTemporaryFile(
             mode="w+", prefix="_apy_edit_", suffix=".css", delete=False
         ) as tf:
             tf.write(model["css"])
             tf.flush()
 
-            retcode = editor(tf.name)
+            retcode = edit_file(tf.name)
             if retcode != 0:
                 console.print(f"Editor return with exit code {retcode}!")
                 return
 
             with open(tf.name, "r", encoding="utf8") as f:
                 new_content = f.read()
 
@@ -437,15 +437,15 @@
             input_string = "\n".join(input_strings) + "\n"
 
         with tempfile.NamedTemporaryFile(
             mode="w+", prefix="apy_note_", suffix=".md", delete=False
         ) as tf:
             tf.write(input_string)
             tf.flush()
-            retcode = editor(tf.name)
+            retcode = edit_file(tf.name)
 
             if retcode != 0:
                 console.print(f"Editor return with exit code {retcode}!")
                 return []
 
             return self.add_notes_from_file(tf.name)
```

### Comparing `apyanki-0.15.4/src/apyanki/cards.py` & `apyanki-0.15.5/src/apyanki/cards.py`

 * *Files identical despite different names*

### Comparing `apyanki-0.15.4/src/apyanki/cli.py` & `apyanki-0.15.5/src/apyanki/cli.py`

 * *Files identical despite different names*

### Comparing `apyanki-0.15.4/src/apyanki/config.py` & `apyanki-0.15.5/src/apyanki/config.py`

 * *Files identical despite different names*

### Comparing `apyanki-0.15.4/src/apyanki/console.py` & `apyanki-0.15.5/src/apyanki/console.py`

 * *Files identical despite different names*

### Comparing `apyanki-0.15.4/src/apyanki/fields.py` & `apyanki-0.15.5/src/apyanki/fields.py`

 * *Files identical despite different names*

### Comparing `apyanki-0.15.4/src/apyanki/note.py` & `apyanki-0.15.5/src/apyanki/note.py`

 * *Files 0% similar despite different names*

```diff
@@ -27,15 +27,15 @@
     convert_text_to_field,
     img_paths_from_field,
     img_paths_from_field_latex,
     prepare_field_for_cli,
     prepare_field_for_cli_raw,
     toggle_field_to_markdown,
 )
-from apyanki.utilities import cd, choose, editor
+from apyanki.utilities import cd, choose, edit_file
 
 if TYPE_CHECKING:
     from apyanki.anki import Anki
     from anki.notes import Note as ANote
 
 
 class Note:
@@ -188,15 +188,15 @@
         """Edit tags and fields of current note"""
         with tempfile.NamedTemporaryFile(
             mode="w+", dir=os.getcwd(), prefix="edit_note_", suffix=".md"
         ) as tf:
             tf.write(str(self))
             tf.flush()
 
-            retcode = editor(tf.name)
+            retcode = edit_file(tf.name)
             if retcode != 0:
                 console.print(f"[red]Editor return with exit code {retcode}![/red]")
                 return
 
             notes = markdown_file_to_notes(tf.name)
 
         if not notes:
```

### Comparing `apyanki-0.15.4/src/apyanki/utilities.py` & `apyanki-0.15.5/src/apyanki/utilities.py`

 * *Files 6% similar despite different names*

```diff
@@ -29,28 +29,29 @@
         exc_type: Optional[type[BaseException]],
         exc_val: Optional[BaseException],
         exc_tb: Optional[TracebackType],
     ) -> None:
         os.chdir(self.savedPath)
 
 
-def editor(filepath: str) -> int:
-    """Use EDITOR to edit file at given path"""
-    return call([os.environ.get("EDITOR", "vim"), filepath])
+def edit_file(filepath: str) -> int:
+    """Use $VISUAL or $EDITOR to edit file at given path"""
+    editor = os.environ.get("VISUAL", os.environ.get("EDITOR", "vim"))
+    return call([editor, filepath])
 
 
 def edit_text(input_text: str, prefix: str = "") -> str:
     """Use EDITOR to edit text (from a temporary file)"""
     if prefix:
         prefix = prefix + "_"
 
     with NamedTemporaryFile(mode="w+", prefix=prefix, suffix=".md") as tf:
         tf.write(input_text)
         tf.flush()
-        editor(tf.name)
+        edit_file(tf.name)
         tf.seek(0)
         edited_message = tf.read().strip()
 
     return edited_message
 
 
 chooseType = TypeVar("chooseType")
```

### Comparing `apyanki-0.15.4/PKG-INFO` & `apyanki-0.15.5/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: apyanki
-Version: 0.15.4
+Version: 0.15.5
 Summary: CLI script for interacting with local Anki collection
 Home-page: https://github.com/lervag/apy
 Author: Karl Yngve Lervåg
 Author-email: karl.yngve@lervag.net
 Requires-Python: >=3.9,<4.0
 Classifier: Environment :: Console
 Classifier: License :: OSI Approved :: MIT License
```

