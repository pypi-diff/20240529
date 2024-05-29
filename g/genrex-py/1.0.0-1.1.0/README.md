# Comparing `tmp/genrex_py-1.0.0.tar.gz` & `tmp/genrex_py-1.1.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "genrex_py-1.0.0.tar", max compression
+gzip compressed data, was "genrex_py-1.1.0.tar", max compression
```

## Comparing `genrex_py-1.0.0.tar` & `genrex_py-1.1.0.tar`

### file list

```diff
@@ -1,14 +1,14 @@
--rw-r--r--   0        0        0     1102 2024-02-06 14:31:39.058423 genrex_py-1.0.0/LICENSE.md
--rw-r--r--   0        0        0     4283 2024-02-14 10:26:50.894616 genrex_py-1.0.0/README.md
--rw-r--r--   0        0        0      117 2024-02-14 10:28:02.810793 genrex_py-1.0.0/genrex/__init__.py
--rw-r--r--   0        0        0    28915 2024-02-06 14:31:39.058423 genrex_py-1.0.0/genrex/classes.py
--rw-r--r--   0        0        0    14342 2024-02-13 20:08:09.639017 genrex_py-1.0.0/genrex/clustering.py
--rw-r--r--   0        0        0     4116 2024-02-06 14:31:39.058423 genrex_py-1.0.0/genrex/enums.py
--rw-r--r--   0        0        0     3849 2024-02-06 14:31:39.058423 genrex_py-1.0.0/genrex/genrex.py
--rw-r--r--   0        0        0      291 2024-02-06 14:31:39.058423 genrex_py-1.0.0/genrex/logging.py
--rw-r--r--   0        0        0     1749 2024-02-06 14:31:39.058423 genrex_py-1.0.0/genrex/misc.py
--rw-r--r--   0        0        0        0 2024-02-06 14:31:39.058423 genrex_py-1.0.0/genrex/py.typed
--rw-r--r--   0        0        0    27846 2024-02-06 14:31:39.058423 genrex_py-1.0.0/genrex/regex.py
--rw-r--r--   0        0        0     2743 2024-02-06 14:31:39.058423 genrex_py-1.0.0/genrex/types.py
--rw-r--r--   0        0        0     1960 2024-02-14 10:28:13.956975 genrex_py-1.0.0/pyproject.toml
--rw-r--r--   0        0        0     4960 1970-01-01 00:00:00.000000 genrex_py-1.0.0/PKG-INFO
+-rw-r--r--   0        0        0     1102 2024-05-29 14:04:50.043861 genrex_py-1.1.0/LICENSE.md
+-rw-r--r--   0        0        0     4283 2024-05-29 14:04:50.043861 genrex_py-1.1.0/README.md
+-rw-r--r--   0        0        0      160 2024-05-29 18:13:52.395900 genrex_py-1.1.0/genrex/__init__.py
+-rw-r--r--   0        0        0    28951 2024-05-29 17:53:51.000000 genrex_py-1.1.0/genrex/classes.py
+-rw-r--r--   0        0        0    14219 2024-05-29 17:58:13.000000 genrex_py-1.1.0/genrex/clustering.py
+-rw-r--r--   0        0        0     4116 2024-05-29 14:04:50.045861 genrex_py-1.1.0/genrex/enums.py
+-rw-r--r--   0        0        0     4520 2024-05-29 18:05:38.481702 genrex_py-1.1.0/genrex/genrex.py
+-rw-r--r--   0        0        0      291 2024-05-29 14:04:50.045861 genrex_py-1.1.0/genrex/logging.py
+-rw-r--r--   0        0        0     2000 2024-05-29 17:58:51.000000 genrex_py-1.1.0/genrex/misc.py
+-rw-r--r--   0        0        0        0 2024-05-29 14:04:50.045861 genrex_py-1.1.0/genrex/py.typed
+-rw-r--r--   0        0        0    27931 2024-05-29 14:34:28.000000 genrex_py-1.1.0/genrex/regex.py
+-rw-r--r--   0        0        0     2743 2024-05-29 14:04:50.046861 genrex_py-1.1.0/genrex/types.py
+-rw-r--r--   0        0        0     1915 2024-05-29 18:14:06.112128 genrex_py-1.1.0/pyproject.toml
+-rw-r--r--   0        0        0     4960 1970-01-01 00:00:00.000000 genrex_py-1.1.0/PKG-INFO
```

### Comparing `genrex_py-1.0.0/LICENSE.md` & `genrex_py-1.1.0/LICENSE.md`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 The MIT License (MIT)
 
-Copyright (c) 2023 Avast Software
+Copyright (c) 2024 Avast Software
 
 Permission is hereby granted, free of charge, to any person obtaining a copy of
 this software and associated documentation files (the "Software"), to deal
 in the Software without restriction, including without limitation the rights to
 use, copy, modify, merge, publish, distribute, sublicense, and/or sell copies
 of the Software, and to permit persons to whom the Software is furnished to do
 so, subject to the following conditions:
```

### Comparing `genrex_py-1.0.0/README.md` & `genrex_py-1.1.0/README.md`

 * *Files 0% similar despite different names*

```diff
@@ -127,10 +127,10 @@
 
 ```bash
 make tests
 ```
 
 ## License
 
-Copyright (c) 2023 Avast Software, licensed under the MIT license. See the
+Copyright (c) 2024 Avast Software, licensed under the MIT license. See the
 [`LICENSE`](https://github.com/avast/genrex/blob/master/LICENSE) file for more
 details.
```

### Comparing `genrex_py-1.0.0/genrex/classes.py` & `genrex_py-1.1.0/genrex/classes.py`

 * *Files 0% similar despite different names*

```diff
@@ -30,29 +30,31 @@
     "frame",
     "google",
     "java",
     "manager",
     "mutex",
     "processor",
     "program",
+    "run",
     "script",
     "server",
     "spoolsv",
     "svchost",
     "synaptics",
     "task",
     "toolbar",
     "txt",
+    "update",
     "ver",
     "window",
     "windows",
     "genrexdot",
-    "genrexbracket",
-    "genrexguid",
-    "genrexhex",
+    "genrexguidbracket",
+    "genrexsimpleguid",
+    "genrexthex",
     "genrexhex8",
     "genrexexem",
 ]
 
 
 class Expression(abc.ABC):
     suffix: bool = False
```

### Comparing `genrex_py-1.0.0/genrex/clustering.py` & `genrex_py-1.1.0/genrex/clustering.py`

 * *Files 4% similar despite different names*

```diff
@@ -9,15 +9,15 @@
 Results are in class Cluster.
 """
 
 import ntpath
 import re
 from collections import defaultdict
 from dataclasses import dataclass, field
-from statistics import mean
+from statistics import mean, median
 
 from genrex.enums import InputType
 from genrex.logging import logger
 from genrex.misc import filter_ngrams, ready_to_print, string2ngrams
 
 
 @dataclass(slots=True)
@@ -135,23 +135,14 @@
                     logger.warning(f"String {string} is GUID")
                     continue
 
                 self.add(string, prep_string, source)
 
         self.extract_ngrams(self.input_type)
 
-    def estimate_len_of_ngram(self):
-        if len(self.samples) == 0:
-            logger.info("No input data after filtering. Exiting.")
-            return
-        self.ngrams = sum(map(len, self.samples)) // (2 * len(self.samples))
-        if len(self.samples) < 10:
-            self.ngrams = self.ngrams // 2
-        self.ngrams = max(self.ngrams, self.min_ngram)
-
     def filter_short_strings(self):
         self.samples = dict(
             filter(lambda x: (len(x[0]) >= self.ngrams), self.samples.items())
         )
 
     def extract_ngrams(self, input_type):
         splited_list = {}
@@ -161,31 +152,31 @@
             for remove_string in filter_ngrams["url"] + filter_ngrams["others"]:
                 pattern = re.compile(remove_string, re.IGNORECASE)
                 ngram_string = pattern.sub("^", ngram_string)
 
             if len(ngram_string) < self.min_ngram:
                 continue
 
-            splited_list[prep_string] = re.split(
-                r"/|\^|\\|\?|!|\+|&|=|\.", ngram_string
+            splited_list[prep_string] = list(
+                filter(None, re.split(r"/|\^|\\|\?|!| |,|\+|&|=", ngram_string))
             )
 
         splited = [len(substr) for k in splited_list.values() for substr in k]
         if len(splited) == 0:
             logger.info("No input data after filtering. Exiting.")
             return
 
-        self.ngrams = sum(splited) // (len(splited))
-        self.ngrams = self.ngrams // 2
-        self.ngrams = max(self.ngrams, self.min_ngram)
-        if input_type in [
+        self.ngrams = int((median(splited) + mean(splited)) // 2)
+        if input_type not in [
             InputType.FILE_ACCESS,
             InputType.KEY_ACCESS,
         ]:
-            self.ngrams = self.ngrams * 4
+            self.ngrams = self.ngrams // 2
+
+        self.ngrams = max(self.ngrams, self.min_ngram)
 
         for key, value in splited_list.items():
             for part in value:
                 if len(part) < self.ngrams:
                     continue
                 self.unique_ngrams[key].extend(string2ngrams(part, self.ngrams))
 
@@ -354,19 +345,26 @@
                     if sample in scores:
                         scores[sample].append(match)
                     else:
                         scores[sample] = [match]
                         ngrams[sample] = sequence
                     seen.add(match)
 
-        self.test_results(scores, ngrams)
+        self.split_general_clusters(scores, ngrams)
         clusters = self.save_results(scores, ngrams)
         return clusters
 
-    def test_results(self, scores: dict[str, list[str]], ngrams: dict[str, str]):
+    def split_general_clusters(
+        self, scores: dict[str, list[str]], ngrams: dict[str, str]
+    ):
+        """
+        Split clusters if the lenght of the strings are too different,
+        creating too general regular expressions.
+        This leads to more clusters with the same n-gram.
+        """
         welp_scores = {}
         welp_ngrams = {}
         for key, cluster in scores.items():
             cluster_checked = [
                 x for x in cluster if ngrams[key] in x and isinstance(x, str)
             ]
             lentghs = [len(x) for x in cluster_checked]
```

### Comparing `genrex_py-1.0.0/genrex/enums.py` & `genrex_py-1.1.0/genrex/enums.py`

 * *Files identical despite different names*

### Comparing `genrex_py-1.0.0/genrex/genrex.py` & `genrex_py-1.1.0/genrex/genrex.py`

 * *Files 27% similar despite different names*

```diff
@@ -2,14 +2,33 @@
 import re
 
 from genrex.clustering import Cluster, Corpus
 from genrex.logging import logger
 from genrex.regex import Regex
 
 
+def log_large_dict(data_dict):
+    """Logs a dictionary with limited keys and values."""
+    max_keys = 3
+    max_values = 3
+    # Limit the number of keys to log
+    limited_keys = list(data_dict.keys())[:max_keys]
+
+    # Create a message string to log
+    message = "{"
+    for i, key in enumerate(limited_keys):
+        # Limit the number of values to log per key
+        limited_values = list(data_dict[key])[:max_values]
+        message += f"{key}: {', '.join(map(str, limited_values))}"
+        if i < len(limited_keys) - 1:
+            message += ", "
+    message += "}"
+    return message
+
+
 def generate(
     cuckoo_format: bool = False,
     store_original_strings: bool = False,
     *,
     input_type: str = "",
     **kwargs,
 ) -> list[Cluster]:
@@ -24,15 +43,15 @@
             directory - a path to directory
     Output:
         a list of Clusters
     """
     data_set: dict = {}
     if "source" in kwargs:
         data_set = kwargs["source"]
-        logger.info(f"Adding source data: {data_set}")
+        logger.info(f"Adding source data (shortened): {log_large_dict(data_set)}")
     elif "directory" in kwargs:
         data_set = load_data_dir(kwargs["directory"])
     else:
         logger.error("No source of data was added!")
         raise IOError("No source of data was added!")
 
     clusters: list[Cluster] = clustering(
@@ -44,15 +63,15 @@
 def load_data_dir(filepath: str) -> dict:
     data_set: dict = {}
     is_valid_directory(filepath)
     datafiles: list[str] = os.listdir(filepath)
     for datafile in datafiles:
         with open(os.path.join(filepath, datafile), "r", encoding="utf-8") as file:
             data_set[datafile] = [line.strip() for line in file if line.strip()]
-    logger.info(f"Adding directory data: {data_set}")
+    logger.info(f"Adding directory data (shortened): {log_large_dict(data_set)}")
     return data_set
 
 
 def is_valid_directory(filepath: str):
     if not os.path.exists(filepath):
         logger.error(f"The directory {filepath} does not exist!")
         raise IOError(f"The directory {filepath} does not exist!")
@@ -71,15 +90,15 @@
     return clusters
 
 
 def generate_regex(clusters: list[Cluster]) -> list[Cluster]:
     results: list[Cluster] = []
     for cluster in clusters:
         logger.info(
-            f"Generating regular expression for cluster {list(cluster.similars.values())}"
+            f"Generating regular expression for cluster {list(cluster.similars.values())[:5]} (shortened)"
         )
         regex: Regex = Regex()
         regex.make_regex(cluster)
         cluster.regex = regex.get_results(reduce=False)
         logger.info(f"Regular expression '{cluster.regex}' generated")
         results.append(cluster)
     return optimized(results)
```

### Comparing `genrex_py-1.0.0/genrex/regex.py` & `genrex_py-1.1.0/genrex/regex.py`

 * *Files 1% similar despite different names*

```diff
@@ -195,21 +195,21 @@
         if ranged is not None:
             return Concatenation(ranged, expr_b.expr_b)
 
     return None
 
 
 class State:
-    def __init__(self):
-        self.accept = False
-        self.transitions = {}
+    def __init__(self) -> None:
+        self.accept: bool = False
+        self.transitions: dict = {}
 
 
 class Trie:
-    def __init__(self):
+    def __init__(self) -> None:
         self.root: State = State()
         self.nodes: list[State] = []
         self.ngram_start: int | None = None
         self.ngram: Literal | None = None
 
     def add(self, word: str, start: int = -1, ngram_trie_root=None):
         node = self.root
@@ -695,30 +695,30 @@
                 expr_a[i] = {}
 
 
 patterns: dict = {
     "GENREXGUIDBRACKET": (
         r"\{[A-Za-z0-9]{8}-[A-Za-z0-9]{4}-[A-Za-z0-9]{4}-[A-Za-z0-9]{4}-[A-Za-z0-9]{12}\}"
     ),
-    "GENREXGUID": r"[A-Za-z0-9]{8}-[A-Za-z0-9]{4}-[A-Za-z0-9]{4}-[A-Za-z0-9]{4}-[A-Za-z0-9]{12}",
+    "GENREXSIMPLEGUID": r"[A-Za-z0-9]{8}-[A-Za-z0-9]{4}-[A-Za-z0-9]{4}-[A-Za-z0-9]{4}-[A-Za-z0-9]{12}",
     "GENREXHEX8": r"[0-9A-Fa-f]{8}:[0-9A-Fa-f]:[0-9A-Fa-f]{8}:[0-9A-Fa-f]{8}:[0-9A-Fa-f]{8}",
     "GENREXURL": r"[0-9]{1,3}\.[0-9]{1,3}\.[0-9]{1,3}\.[0-9]{1,3}",
     "GENREXTHEX": r"[0-9a-f]{3}\.[0-9a-f]{3}\.[0-9a-f]{3}",
     "GENREXDOT": r"\.[A-Za-z]{2,4}$",
     "GENREXPHONE": r"\+?[0-9]-[0-9]{3}-[0-9]{3}-[0-9]{4}",
 }
 
 
 class Regex:
-    def __init__(self):
-        self.regexps = ""
-        self.found_patterns = set()
-        self.dot_array = set()
-        self.prefix = False
-        self.suffix = False
+    def __init__(self) -> None:
+        self.regexps: Expression = Literal("")
+        self.found_patterns: set = set()
+        self.dot_array: set = set()
+        self.prefix: bool = False
+        self.suffix: bool = False
 
     def get_regexps(self):
         return self.regexps
 
     def make_regex(self, cluster: Cluster):
         if NamedObjectStrictType.contains(str(cluster.input_type)):
             self.prefix = True
```

### Comparing `genrex_py-1.0.0/genrex/types.py` & `genrex_py-1.1.0/genrex/types.py`

 * *Files identical despite different names*

### Comparing `genrex_py-1.0.0/pyproject.toml` & `genrex_py-1.1.0/pyproject.toml`

 * *Files 16% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "genrex-py"
-version = "1.0.0"
+version = "1.1.0"
 description = "GenRex is a tool that generates regular expressions from strings such as artifacts dynamically generated by samples."
 authors = ["Dominika Regéciová <Dominika.Regeciova@gendigital.com>"]
 maintainers = ["Dominika Regéciová <Dominika.Regeciova@gendigital.com>"]
 readme = "README.md"
 license = "MIT"
 include = ["py.typed", "LICENSE"]
 
@@ -12,39 +12,37 @@
 	{ include = "genrex" }
 ]
 
 [tool.poetry.dependencies]
 python = "^3.10"
 
 [tool.poetry.dev-dependencies]
-black = "^24.2.0"
 isort = "^5.10.1"
-mypy = "^1.3.0"
-poethepoet = "^0.24.0"
-pytest = "^8.0.0"
-pytest-black = "^0.3.12"
-pytest-isort = "^3.1.0"
-pytest-cov = "^4.0.0"
-pytest-mock = "^3.10.0"
+mypy = "^1.10.0"
+poethepoet = "^0.26.1"
+pytest = "^8.2.1"
+pytest-isort = "^4.0.0"
+pytest-cov = "^5.0.0"
+pytest-mock = "^3.14.0"
 pytest-mypy = "^0.10.3"
-requests-mock = "^1.10.0"
+requests-mock = "^1.12.1"
 pytest-pylint = "^0.21.0"
-pylint = "^3.0.3"
+pylint = "^3.2.2"
 types-requests = ">=0.1.8,<3.0.0"
 types-tabulate = ">=0.1.0,<0.9.1"
-ruff = "^0.2.1"
-pytest-ruff = "^0.2.1"
+ruff = "^0.4.5"
+pytest-ruff = "^0.3"
 
 [tool.poe.tasks]
-_black = "black genrex/ tests/"
+_ruff = "ruff format genrex/ tests/"
 _isort = "isort genrex/ tests/"
-_black_check = "black --check genrex/ tests/"
+_ruff_check = "ruff check genrex/ tests/"
 _isort_check = "isort --check genrex/ tests/"
-format = ["_isort", "_black"]
-format-check = ["_isort_check", "_black_check"]
+format = ["_isort", "_ruff"]
+format-check = ["_isort_check", "_ruff_check"]
 test = "pytest -vvv --mypy --ruff --pylint --pylint-rcfile=pyproject.toml --cov=genrex --cov-report=term-missing -l genrex/ tests/"
 
 
 [tool.isort]
 profile = "black"
 
 [tool.pylint.master]
```

### Comparing `genrex_py-1.0.0/PKG-INFO` & `genrex_py-1.1.0/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: genrex-py
-Version: 1.0.0
+Version: 1.1.0
 Summary: GenRex is a tool that generates regular expressions from strings such as artifacts dynamically generated by samples.
 License: MIT
 Author: Dominika Regéciová
 Author-email: Dominika.Regeciova@gendigital.com
 Maintainer: Dominika Regéciová
 Maintainer-email: Dominika.Regeciova@gendigital.com
 Requires-Python: >=3.10,<4.0
@@ -144,11 +144,11 @@
 
 ```bash
 make tests
 ```
 
 ## License
 
-Copyright (c) 2023 Avast Software, licensed under the MIT license. See the
+Copyright (c) 2024 Avast Software, licensed under the MIT license. See the
 [`LICENSE`](https://github.com/avast/genrex/blob/master/LICENSE) file for more
 details.
```

