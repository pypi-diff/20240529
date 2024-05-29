# Comparing `tmp/intersphinx_registry-0.2405.27.tar.gz` & `tmp/intersphinx_registry-0.2405.29.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "intersphinx_registry-0.2405.27.tar", last modified: Fri Jan  1 00:00:00 2016, max compression
+gzip compressed data, was "intersphinx_registry-0.2405.29.tar", last modified: Fri Jan  1 00:00:00 2016, max compression
```

## Comparing `intersphinx_registry-0.2405.27.tar` & `intersphinx_registry-0.2405.29.tar`

### file list

```diff
@@ -1,7 +1,10 @@
--rw-r--r--   0        0        0     1086 2024-05-03 07:52:01.783580 intersphinx_registry-0.2405.27/LICENSE
--rw-r--r--   0        0        0     1017 2024-05-27 08:45:56.933382 intersphinx_registry-0.2405.27/README.md
--rw-r--r--   0        0        0     1705 2024-05-27 08:49:29.949581 intersphinx_registry-0.2405.27/intersphinx_registry/__init__.py
--rw-r--r--   0        0        0        0 2024-05-03 07:55:04.206909 intersphinx_registry-0.2405.27/intersphinx_registry/py.typed
--rw-r--r--   0        0        0     9785 2024-05-27 08:45:56.933718 intersphinx_registry-0.2405.27/intersphinx_registry/registry.json
--rw-r--r--   0        0        0      637 2024-05-03 13:38:36.749859 intersphinx_registry-0.2405.27/pyproject.toml
--rw-r--r--   0        0        0     1560 1970-01-01 00:00:00.000000 intersphinx_registry-0.2405.27/PKG-INFO
+-rw-r--r--   0        0        0      698 2024-05-03 15:35:42.574589 intersphinx_registry-0.2405.29/.github/workflows/tests.yml
+-rw-r--r--   0        0        0       18 2024-05-27 08:45:56.933164 intersphinx_registry-0.2405.29/.gitignore
+-rw-r--r--   0        0        0     1086 2024-05-03 07:52:01.783580 intersphinx_registry-0.2405.29/LICENSE
+-rw-r--r--   0        0        0     1021 2024-05-27 08:51:53.838781 intersphinx_registry-0.2405.29/README.md
+-rw-r--r--   0        0        0     1705 2024-05-29 09:00:28.875611 intersphinx_registry-0.2405.29/intersphinx_registry/__init__.py
+-rw-r--r--   0        0        0        0 2024-05-03 07:55:04.206909 intersphinx_registry-0.2405.29/intersphinx_registry/py.typed
+-rw-r--r--   0        0        0     9911 2024-05-29 08:55:10.358748 intersphinx_registry-0.2405.29/intersphinx_registry/registry.json
+-rw-r--r--   0        0        0      637 2024-05-03 13:38:36.749859 intersphinx_registry-0.2405.29/pyproject.toml
+-rw-r--r--   0        0        0     1125 2024-05-27 08:45:56.934125 intersphinx_registry-0.2405.29/tests/test_basic.py
+-rw-r--r--   0        0        0     1564 1970-01-01 00:00:00.000000 intersphinx_registry-0.2405.29/PKG-INFO
```

### Comparing `intersphinx_registry-0.2405.27/LICENSE` & `intersphinx_registry-0.2405.29/LICENSE`

 * *Files identical despite different names*

### Comparing `intersphinx_registry-0.2405.27/README.md` & `intersphinx_registry-0.2405.29/README.md`

 * *Files 2% similar despite different names*

```diff
@@ -5,15 +5,15 @@
 Usage in `conf.py`
 
 ```python
 from intersphinx_registry import get_intersphinx_mapping
 
 # ...
 intersphinx_mapping = get_intersphinx_mapping(
-    only={"ipython", "matplotlib", "pandas", "python"}
+    packages={"ipython", "matplotlib", "pandas", "python"}
 )
 intersphinx_mapping.update({
     'overwrite': ('<url>', None),
     'my-package' : ('<url>', None),
 })
 ```
```

### Comparing `intersphinx_registry-0.2405.27/intersphinx_registry/__init__.py` & `intersphinx_registry-0.2405.29/intersphinx_registry/__init__.py`

 * *Files 6% similar despite different names*

```diff
@@ -6,15 +6,15 @@
 
 from pathlib import Path
 import json
 from typing import Dict, Tuple, Set, Optional, cast
 
 # See issue 4, we this the best format is Major.YYMM.day,
 # in case of multiple releases a day we can borrow the next day's date.
-__version__ = "0.2405.27"
+__version__ = "0.2405.29"
 
 registry_file = Path(__file__).parent / "registry.json"
 
 def _get_all_mappings() ->  Dict[str, Tuple[str, Optional[str]]]:
     return cast(
         Dict[str, Tuple[str, Optional[str]]],
         {k: tuple(v) for (k, v) in json.loads(registry_file.read_bytes()).items()},
```

### Comparing `intersphinx_registry-0.2405.27/intersphinx_registry/registry.json` & `intersphinx_registry-0.2405.29/intersphinx_registry/registry.json`

 * *Files 1% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.987012987012987%*

 * *Differences: {"'mne_icalabel'": "['https://mne.tools/mne-icalabel/stable/', None]",*

 * * "'mne_lsl'": "['https://mne.tools/mne-lsl/stable/', None]"}*

```diff
@@ -235,14 +235,22 @@
         "https://meson-python.readthedocs.io/en/stable/",
         null
     ],
     "mne": [
         "https://mne.tools/stable/",
         null
     ],
+    "mne_icalabel": [
+        "https://mne.tools/mne-icalabel/stable/",
+        null
+    ],
+    "mne_lsl": [
+        "https://mne.tools/mne-lsl/stable/",
+        null
+    ],
     "monkeytype": [
         "https://monkeytype.readthedocs.io/en/latest/",
         null
     ],
     "mpmath": [
         "https://mpmath.org/doc/current/",
         null
```

### Comparing `intersphinx_registry-0.2405.27/pyproject.toml` & `intersphinx_registry-0.2405.29/pyproject.toml`

 * *Files identical despite different names*

### Comparing `intersphinx_registry-0.2405.27/PKG-INFO` & `intersphinx_registry-0.2405.29/PKG-INFO`

 * *Files 12% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: intersphinx_registry
-Version: 0.2405.27
+Version: 0.2405.29
 Summary: This package provides convenient utilities and data to write a sphinx config file.
 Author-email: Matthias Bussonnier <bussonniermatthias@gmail.com>
 Description-Content-Type: text/markdown
 Classifier: License :: OSI Approved :: MIT License
 Requires-Dist: pytest>=7.0 ; extra == "tests"
 Requires-Dist: pytest-xdist ; extra == "tests"
 Requires-Dist: requests ; extra == "tests"
@@ -18,15 +18,15 @@
 Usage in `conf.py`
 
 ```python
 from intersphinx_registry import get_intersphinx_mapping
 
 # ...
 intersphinx_mapping = get_intersphinx_mapping(
-    only={"ipython", "matplotlib", "pandas", "python"}
+    packages={"ipython", "matplotlib", "pandas", "python"}
 )
 intersphinx_mapping.update({
     'overwrite': ('<url>', None),
     'my-package' : ('<url>', None),
 })
 ```
```

