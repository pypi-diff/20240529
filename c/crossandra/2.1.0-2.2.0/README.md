# Comparing `tmp/crossandra-2.1.0.tar.gz` & `tmp/crossandra-2.2.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "crossandra-2.1.0.tar", last modified: Wed May  1 17:26:29 2024, max compression
+gzip compressed data, was "crossandra-2.2.0.tar", last modified: Wed May 29 12:07:09 2024, max compression
```

## Comparing `crossandra-2.1.0.tar` & `crossandra-2.2.0.tar`

### file list

```diff
@@ -1,23 +1,23 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-01 17:26:29.027715 crossandra-2.1.0/
--rw-r--r--   0 runner    (1001) docker     (127)     1056 2024-05-01 17:26:21.000000 crossandra-2.1.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)     2408 2024-05-01 17:26:29.027715 crossandra-2.1.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     2039 2024-05-01 17:26:21.000000 crossandra-2.1.0/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-01 17:26:29.027715 crossandra-2.1.0/crossandra/
--rw-r--r--   0 runner    (1001) docker     (127)      463 2024-05-01 17:26:21.000000 crossandra-2.1.0/crossandra/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2362 2024-05-01 17:26:21.000000 crossandra-2.1.0/crossandra/common.py
--rw-r--r--   0 runner    (1001) docker     (127)      285 2024-05-01 17:26:21.000000 crossandra-2.1.0/crossandra/exceptions.py
--rw-r--r--   0 runner    (1001) docker     (127)     6202 2024-05-01 17:26:21.000000 crossandra-2.1.0/crossandra/lib.py
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-01 17:26:21.000000 crossandra-2.1.0/crossandra/py.typed
--rw-r--r--   0 runner    (1001) docker     (127)     3858 2024-05-01 17:26:21.000000 crossandra-2.1.0/crossandra/rule.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-01 17:26:29.027715 crossandra-2.1.0/crossandra.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     2408 2024-05-01 17:26:29.000000 crossandra-2.1.0/crossandra.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      375 2024-05-01 17:26:29.000000 crossandra-2.1.0/crossandra.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-01 17:26:29.000000 crossandra-2.1.0/crossandra.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       14 2024-05-01 17:26:29.000000 crossandra-2.1.0/crossandra.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       39 2024-05-01 17:26:29.000000 crossandra-2.1.0/crossandra.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)      915 2024-05-01 17:26:21.000000 crossandra-2.1.0/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-01 17:26:29.027715 crossandra-2.1.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)      275 2024-05-01 17:26:21.000000 crossandra-2.1.0/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-01 17:26:29.027715 crossandra-2.1.0/tests/
--rw-r--r--   0 runner    (1001) docker     (127)     4806 2024-05-01 17:26:21.000000 crossandra-2.1.0/tests/test_api.py
--rw-r--r--   0 runner    (1001) docker     (127)     7785 2024-05-01 17:26:21.000000 crossandra-2.1.0/tests/test_common.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-29 12:07:09.589681 crossandra-2.2.0/
+-rw-r--r--   0 runner    (1001) docker     (127)     1056 2024-05-29 12:07:01.000000 crossandra-2.2.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)     3001 2024-05-29 12:07:09.589681 crossandra-2.2.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     2632 2024-05-29 12:07:01.000000 crossandra-2.2.0/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-29 12:07:09.589681 crossandra-2.2.0/crossandra/
+-rw-r--r--   0 runner    (1001) docker     (127)      463 2024-05-29 12:07:01.000000 crossandra-2.2.0/crossandra/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2615 2024-05-29 12:07:01.000000 crossandra-2.2.0/crossandra/common.py
+-rw-r--r--   0 runner    (1001) docker     (127)      285 2024-05-29 12:07:01.000000 crossandra-2.2.0/crossandra/exceptions.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6202 2024-05-29 12:07:01.000000 crossandra-2.2.0/crossandra/lib.py
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-29 12:07:01.000000 crossandra-2.2.0/crossandra/py.typed
+-rw-r--r--   0 runner    (1001) docker     (127)     4268 2024-05-29 12:07:01.000000 crossandra-2.2.0/crossandra/rule.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-29 12:07:09.589681 crossandra-2.2.0/crossandra.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     3001 2024-05-29 12:07:09.000000 crossandra-2.2.0/crossandra.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      375 2024-05-29 12:07:09.000000 crossandra-2.2.0/crossandra.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-29 12:07:09.000000 crossandra-2.2.0/crossandra.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       14 2024-05-29 12:07:09.000000 crossandra-2.2.0/crossandra.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       39 2024-05-29 12:07:09.000000 crossandra-2.2.0/crossandra.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)     1049 2024-05-29 12:07:01.000000 crossandra-2.2.0/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-29 12:07:09.589681 crossandra-2.2.0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)      275 2024-05-29 12:07:01.000000 crossandra-2.2.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-29 12:07:09.589681 crossandra-2.2.0/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)     6239 2024-05-29 12:07:01.000000 crossandra-2.2.0/tests/test_api.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8439 2024-05-29 12:07:01.000000 crossandra-2.2.0/tests/test_common.py
```

### Comparing `crossandra-2.1.0/LICENSE` & `crossandra-2.2.0/LICENSE`

 * *Files 11% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-Copyright (c) 2022–2023 trag1c
+Copyright (c) 2022–2024 trag1c
 
 Permission is hereby granted, free of charge, to any person obtaining a copy
 of this software and associated documentation files (the "Software"), to deal
 in the Software without restriction, including without limitation the rights
 to use, copy, modify, merge, publish, distribute, sublicense, and/or sell
 copies of the Software, and to permit persons to whom the Software is
 furnished to do so, subject to the following conditions:
```

### Comparing `crossandra-2.1.0/PKG-INFO` & `crossandra-2.2.0/PKG-INFO`

 * *Files 10% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: crossandra
-Version: 2.1.0
+Version: 2.2.0
 Summary: A fast and simple enum/regex-based tokenizer with decent configurability
 Author-email: trag1c <trag1cdev@yahoo.com>
 License: MIT
 Project-URL: repository, https://github.com/trag1c/crossandra
 Requires-Python: >=3.8
 Description-Content-Type: text/markdown
 License-File: LICENSE
@@ -19,18 +19,15 @@
 Python package manager:
 ```sh
 $ pip install crossandra
 ```
 (Some systems may require you to use `pip3`, `python -m pip`, or `py -m pip`
 instead)
 
-## License
-Crossandra is licensed under the MIT License.
-
-## [Documentation](https://github.com/trag1c/crossandra/wiki/The-Crossandra-class)
+## [Documentation]
 
 ## Examples
 ```py
 from enum import Enum
 from crossandra import Crossandra
 
 class Brainfuck(Enum):
@@ -57,15 +54,15 @@
 def hex2rgb(hex_color: str) -> tuple[int, int, int]:
     r, g, b = (int(hex_color[i:i+2], 16) for i in range(1, 6, 2))
     return r, g, b
 
 t = Crossandra(
     ignore_whitespace=True,
     rules=[
-        Rule(r"#[0-9a-fA-F]+", hex2rgb),
+        Rule(r"#[0-9a-fA-F]{6}", hex2rgb),
         common.WORD
     ]
 )
 
 text = "My favorite color is #facade"
 print(t.tokenize(text))
 # ['My', 'favorite', 'color', 'is', (250, 202, 222)]
@@ -85,16 +82,41 @@
     DIV = "--"
     POW = "+++"
     MOD = "---"
 
 sm = Crossandra(
     Op,
     ignore_whitespace=True,
-    rules=[Rule(r"(?:\\|/)+", sm_int)]
+    rules=[Rule(r"[\\/]+", sm_int)]
 )
 
 print(*sm.tokenize(r"//\ ++ /\\/ --- /\/\/ - ///"))
 # 6 Op.MUL 9 Op.MOD 21 Op.SUB 7
 ```
 
+## Contributing
+
+Contributions are welcome!
+
+Please open an issue before submitting a pull request (unless it's a minor
+change like fixing a typo).
+
+To get started:
+1. Clone your fork of the project.
+2. Set up the project with `just install` (uses [uv]).
+3. After you're done, run `just check` to check your changes.
+
+> [!note]
+> If you don't want to use [`just`][just], simply look up the recipes
+> in the project's [`justfile`][justfile].
+
+## License
+Crossandra is licensed under the MIT License.
+
 If you have any questions, or would like to get in touch, join my
-[Discord server](https://discord.gg/C8QE5tVQEq)!
+[Discord server]!
+
+[Documentation]: https://trag1c.github.io/crossandra/
+[Discord server]: https://discord.gg/C8QE5tVQEq
+[just]: https://github.com/casey/just
+[justfile]: https://github.com/trag1c/crossandra/blob/main/justfile
+[uv]: https://github.com/astral-sh/uv
```

### Comparing `crossandra-2.1.0/README.md` & `crossandra-2.2.0/crossandra.egg-info/PKG-INFO`

 * *Files 18% similar despite different names*

```diff
@@ -1,24 +1,33 @@
+Metadata-Version: 2.1
+Name: crossandra
+Version: 2.2.0
+Summary: A fast and simple enum/regex-based tokenizer with decent configurability
+Author-email: trag1c <trag1cdev@yahoo.com>
+License: MIT
+Project-URL: repository, https://github.com/trag1c/crossandra
+Requires-Python: >=3.8
+Description-Content-Type: text/markdown
+License-File: LICENSE
+Requires-Dist: result~=0.9.0
+
 # Crossandra
 Crossandra is a fast and simple tokenization library for Python operating on
 enums and regular expressions, with a decent amount of configuration.
 
 ## Installation
 Crossandra is available on PyPI and can be installed with pip, or any other
 Python package manager:
 ```sh
 $ pip install crossandra
 ```
 (Some systems may require you to use `pip3`, `python -m pip`, or `py -m pip`
 instead)
 
-## License
-Crossandra is licensed under the MIT License.
-
-## [Documentation](https://github.com/trag1c/crossandra/wiki/The-Crossandra-class)
+## [Documentation]
 
 ## Examples
 ```py
 from enum import Enum
 from crossandra import Crossandra
 
 class Brainfuck(Enum):
@@ -45,15 +54,15 @@
 def hex2rgb(hex_color: str) -> tuple[int, int, int]:
     r, g, b = (int(hex_color[i:i+2], 16) for i in range(1, 6, 2))
     return r, g, b
 
 t = Crossandra(
     ignore_whitespace=True,
     rules=[
-        Rule(r"#[0-9a-fA-F]+", hex2rgb),
+        Rule(r"#[0-9a-fA-F]{6}", hex2rgb),
         common.WORD
     ]
 )
 
 text = "My favorite color is #facade"
 print(t.tokenize(text))
 # ['My', 'favorite', 'color', 'is', (250, 202, 222)]
@@ -73,16 +82,41 @@
     DIV = "--"
     POW = "+++"
     MOD = "---"
 
 sm = Crossandra(
     Op,
     ignore_whitespace=True,
-    rules=[Rule(r"(?:\\|/)+", sm_int)]
+    rules=[Rule(r"[\\/]+", sm_int)]
 )
 
 print(*sm.tokenize(r"//\ ++ /\\/ --- /\/\/ - ///"))
 # 6 Op.MUL 9 Op.MOD 21 Op.SUB 7
 ```
 
+## Contributing
+
+Contributions are welcome!
+
+Please open an issue before submitting a pull request (unless it's a minor
+change like fixing a typo).
+
+To get started:
+1. Clone your fork of the project.
+2. Set up the project with `just install` (uses [uv]).
+3. After you're done, run `just check` to check your changes.
+
+> [!note]
+> If you don't want to use [`just`][just], simply look up the recipes
+> in the project's [`justfile`][justfile].
+
+## License
+Crossandra is licensed under the MIT License.
+
 If you have any questions, or would like to get in touch, join my
-[Discord server](https://discord.gg/C8QE5tVQEq)!
+[Discord server]!
+
+[Documentation]: https://trag1c.github.io/crossandra/
+[Discord server]: https://discord.gg/C8QE5tVQEq
+[just]: https://github.com/casey/just
+[justfile]: https://github.com/trag1c/crossandra/blob/main/justfile
+[uv]: https://github.com/astral-sh/uv
```

### Comparing `crossandra-2.1.0/crossandra/common.py` & `crossandra-2.2.0/crossandra/common.py`

 * *Files 10% similar despite different names*

```diff
@@ -58,7 +58,14 @@
 
 STRING: RuleGroup = SINGLE_QUOTED_STRING | DOUBLE_QUOTED_STRING
 """A string enclosed in either single or double quotes."""
 NUMBER: RuleGroup = FLOAT | INT
 """A number (either an integer or a floating point value)."""
 SIGNED_NUMBER: RuleGroup = SIGNED_FLOAT | SIGNED_INT
 """A signed number (either an integer or a floating point value)."""
+
+ANY_INT: RuleGroup = INT | SIGNED_INT
+"""Any integer value (optional sign)."""
+ANY_FLOAT: RuleGroup = FLOAT | SIGNED_FLOAT
+"""Any floating point value (optional sign)."""
+ANY_NUMBER: RuleGroup = NUMBER | SIGNED_NUMBER
+"""Any number (optional sign)."""
```

### Comparing `crossandra-2.1.0/crossandra/lib.py` & `crossandra-2.2.0/crossandra/lib.py`

 * *Files identical despite different names*

### Comparing `crossandra-2.1.0/crossandra/rule.py` & `crossandra-2.2.0/crossandra/rule.py`

 * *Files 2% similar despite different names*

```diff
@@ -118,14 +118,24 @@
     """
     Used for storing multiple Rules in one object. Can be constructed
     by passing in a tuple of rules or by ORing (`|`) two or more rules.
     """
 
     rules: tuple[Rule[Any], ...]
 
+    def apply(self, target: str) -> tuple[Any | str | Ignored, int] | NotApplied:
+        """
+        Applies the rules in the group to the target string. Returns the
+        result of the first rule that matches, or `NotApplied` if none do.
+        """
+        for rule in self.rules:
+            if (result := rule.apply(target)) is not NOT_APPLIED:
+                return result
+        return NOT_APPLIED
+
     def __iter__(self) -> Iterator[Rule[Any]]:
         yield from self.rules
 
     def __or__(self, other: object) -> RuleGroup:
         if isinstance(other, RuleGroup):
             return RuleGroup((*self.rules, *other.rules))
         if isinstance(other, Rule):
```

### Comparing `crossandra-2.1.0/crossandra.egg-info/PKG-INFO` & `crossandra-2.2.0/README.md`

 * *Files 15% similar despite different names*

```diff
@@ -1,36 +1,21 @@
-Metadata-Version: 2.1
-Name: crossandra
-Version: 2.1.0
-Summary: A fast and simple enum/regex-based tokenizer with decent configurability
-Author-email: trag1c <trag1cdev@yahoo.com>
-License: MIT
-Project-URL: repository, https://github.com/trag1c/crossandra
-Requires-Python: >=3.8
-Description-Content-Type: text/markdown
-License-File: LICENSE
-Requires-Dist: result~=0.9.0
-
 # Crossandra
 Crossandra is a fast and simple tokenization library for Python operating on
 enums and regular expressions, with a decent amount of configuration.
 
 ## Installation
 Crossandra is available on PyPI and can be installed with pip, or any other
 Python package manager:
 ```sh
 $ pip install crossandra
 ```
 (Some systems may require you to use `pip3`, `python -m pip`, or `py -m pip`
 instead)
 
-## License
-Crossandra is licensed under the MIT License.
-
-## [Documentation](https://github.com/trag1c/crossandra/wiki/The-Crossandra-class)
+## [Documentation]
 
 ## Examples
 ```py
 from enum import Enum
 from crossandra import Crossandra
 
 class Brainfuck(Enum):
@@ -57,15 +42,15 @@
 def hex2rgb(hex_color: str) -> tuple[int, int, int]:
     r, g, b = (int(hex_color[i:i+2], 16) for i in range(1, 6, 2))
     return r, g, b
 
 t = Crossandra(
     ignore_whitespace=True,
     rules=[
-        Rule(r"#[0-9a-fA-F]+", hex2rgb),
+        Rule(r"#[0-9a-fA-F]{6}", hex2rgb),
         common.WORD
     ]
 )
 
 text = "My favorite color is #facade"
 print(t.tokenize(text))
 # ['My', 'favorite', 'color', 'is', (250, 202, 222)]
@@ -85,16 +70,41 @@
     DIV = "--"
     POW = "+++"
     MOD = "---"
 
 sm = Crossandra(
     Op,
     ignore_whitespace=True,
-    rules=[Rule(r"(?:\\|/)+", sm_int)]
+    rules=[Rule(r"[\\/]+", sm_int)]
 )
 
 print(*sm.tokenize(r"//\ ++ /\\/ --- /\/\/ - ///"))
 # 6 Op.MUL 9 Op.MOD 21 Op.SUB 7
 ```
 
+## Contributing
+
+Contributions are welcome!
+
+Please open an issue before submitting a pull request (unless it's a minor
+change like fixing a typo).
+
+To get started:
+1. Clone your fork of the project.
+2. Set up the project with `just install` (uses [uv]).
+3. After you're done, run `just check` to check your changes.
+
+> [!note]
+> If you don't want to use [`just`][just], simply look up the recipes
+> in the project's [`justfile`][justfile].
+
+## License
+Crossandra is licensed under the MIT License.
+
 If you have any questions, or would like to get in touch, join my
-[Discord server](https://discord.gg/C8QE5tVQEq)!
+[Discord server]!
+
+[Documentation]: https://trag1c.github.io/crossandra/
+[Discord server]: https://discord.gg/C8QE5tVQEq
+[just]: https://github.com/casey/just
+[justfile]: https://github.com/trag1c/crossandra/blob/main/justfile
+[uv]: https://github.com/astral-sh/uv
```

### Comparing `crossandra-2.1.0/pyproject.toml` & `crossandra-2.2.0/pyproject.toml`

 * *Files 27% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [project]
 name = "crossandra"
-version = "2.1.0"
+version = "2.2.0"
 description = "A fast and simple enum/regex-based tokenizer with decent configurability"
 authors = [{ email = "trag1c <trag1cdev@yahoo.com>" }]
 license = { text = "MIT" }
 urls = { repository = "https://github.com/trag1c/crossandra" }
 readme = "README.md"
 requires-python = ">=3.8"
 dependencies = ["result ~= 0.9.0"]
@@ -14,14 +14,21 @@
 
 [tool.cibuildwheel.linux]
 archs = ["auto", "aarch64"]
 
 [tool.cibuildwheel.macos]
 archs = ["x86_64", "universal2"]
 
+[tool.coverage.report]
+exclude_also = [
+    "if TYPE_CHECKING:",
+    "if sys.version_info.*:",
+    "if __name__ == \"__main__\":",
+]
+
 [tool.ruff]
 target-version = "py38"
 
 [tool.ruff.lint]
 select = ["ALL"]
 ignore = ["COM", "D", "FIX", "ANN1", "ANN401", "ISC001", "ERA", "C9", "PLR0913"]
```

### Comparing `crossandra-2.1.0/tests/test_common.py` & `crossandra-2.2.0/tests/test_common.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,32 +1,14 @@
 from __future__ import annotations
 
 from typing import Tuple, Union
 
 import pytest
 
-from crossandra.common import (
-    C_NAME,
-    CHAR,
-    DECIMAL,
-    DIGIT,
-    DOUBLE_QUOTED_STRING,
-    FLOAT,
-    HEXDIGIT,
-    INT,
-    LETTER,
-    NEWLINE,
-    NUMBER,
-    SIGNED_FLOAT,
-    SIGNED_INT,
-    SIGNED_NUMBER,
-    SINGLE_QUOTED_STRING,
-    STRING,
-    WORD,
-)
+from crossandra import common
 from crossandra.lib import Crossandra
 from crossandra.rule import NOT_APPLIED, Ignored, NotApplied
 
 # ESC = ESCAPED
 # UC = UPPERCASE
 # LC = LOWERCASE
 # POS = POSITIVE
@@ -46,15 +28,15 @@
         ("'test", NOT_APPLIED),  # NO ENDING QUOTE
         ("\\'test'", NOT_APPLIED),  # ESC STARTING QUOTE
         ("'test\\'", NOT_APPLIED),  # ESC ENDING QUOTE
         ("''", ("''", 2)),  # EMPTY
     ],
 )
 def test_single_quoted_string(string: str, result: RuleResult) -> None:
-    assert SINGLE_QUOTED_STRING.apply(string) == result
+    assert common.SINGLE_QUOTED_STRING.apply(string) == result
 
 
 @pytest.mark.parametrize(
     ("string", "result"),
     [
         ('"test"', ('"test"', 6)),  # CLASSIC
         ('"""', ('""', 2)),  # STRING CONTAINING QUOTE
@@ -63,19 +45,22 @@
         ('"test', NOT_APPLIED),  # NO ENDING QUOTE
         ('\\"test"', NOT_APPLIED),  # ESC STARTING QUOTE
         ('"test\\"', NOT_APPLIED),  # ESC ENDING QUOTE
         ('""', ('""', 2)),  # EMPTY
     ],
 )
 def test_double_quoted_string(string: str, result: RuleResult) -> None:
-    assert DOUBLE_QUOTED_STRING.apply(string) == result
+    assert common.DOUBLE_QUOTED_STRING.apply(string) == result
 
 
 def test_string() -> None:
-    assert Crossandra(rules=[STRING]).tokenize("'test'\"test\"") == ["'test'", '"test"']
+    assert Crossandra(rules=[common.STRING]).tokenize("'test'\"test\"") == [
+        "'test'",
+        '"test"',
+    ]
 
 
 @pytest.mark.parametrize(
     ("string", "result"),
     [
         ("'t'", ("'t'", 3)),  # CLASSIC
         ("'''", NOT_APPLIED),  # SINGLE QUOTE CHAR
@@ -84,81 +69,81 @@
         ("'t", NOT_APPLIED),  # NO ENDING QUOTE
         ("\\'t'", NOT_APPLIED),  # ESC STARTING QUOTE
         ("'t\\'", NOT_APPLIED),  # ESC ENDING QUOTE
         ("''", NOT_APPLIED),  # EMPTY
     ],
 )
 def test_char(string: str, result: RuleResult) -> None:
-    assert CHAR.apply(string) == result
+    assert common.CHAR.apply(string) == result
 
 
 @pytest.mark.parametrize(
     ("string", "result"),
     [
         ("A", ("A", 1)),  # UC LETTER
         ("a", ("a", 1)),  # LC LETTER
         ("!", NOT_APPLIED),  # ASCII CHAR BETWEEN UC AND LC
         ("@", NOT_APPLIED),  # ASCII CHAR BEFORE UC
         ("|", NOT_APPLIED),  # ASCII CHAR AFTER LC
         ("", NOT_APPLIED),  # EMPTY
     ],
 )
 def test_letter(string: str, result: RuleResult) -> None:
-    assert LETTER.apply(string) == result
+    assert common.LETTER.apply(string) == result
 
 
 @pytest.mark.parametrize(
     ("string", "result"),
     [
         ("word", ("word", 4)),  # CLASSIC
         ("", NOT_APPLIED),  # EMPTY
     ],
 )
 def test_word(string: str, result: RuleResult) -> None:
-    assert WORD.apply(string) == result
+    assert common.WORD.apply(string) == result
 
 
 @pytest.mark.parametrize(
     ("string", "result"),
     [
         ("0", (0, 1)),  # CLASSIC
         ("/", NOT_APPLIED),  # CHAR BEFORE DIGITS IN ASCII TABLE
         (":", NOT_APPLIED),  # CHAR AFTER DIGITS IN ASCII TABLE
         ("", NOT_APPLIED),  # EMPTY
     ],
 )
 def test_digit(string: str, result: RuleResult) -> None:
-    assert DIGIT.apply(string) == result
+    assert common.DIGIT.apply(string) == result
 
 
 @pytest.mark.parametrize(
     ("string", "result"),
     [
         ("69", (69, 2)),  # CLASSIC
         ("069", (69, 3)),  # LEADING ZERO
         ("1_000_000", (1000000, 9)),  # USCORE SEP
         ("1__0", (10, 4)),  # TWO USCORES AS SEP
         ("", NOT_APPLIED),  # EMPTY
     ],
 )
 def test_int(string: str, result: RuleResult) -> None:
-    assert INT.apply(string) == result
+    assert common.INT.apply(string) == result
 
 
 @pytest.mark.parametrize(
     ("string", "result"),
     [
         ("+69", (69, 3)),  # POS INT
         ("-69", (-69, 3)),  # NEG INT
         ("69", NOT_APPLIED),  # NOT SIGNED
         ("", NOT_APPLIED),  # EMPTY
     ],
 )
 def test_signed_int(string: str, result: RuleResult) -> None:
-    assert SIGNED_INT.apply(string) == result
+    assert common.SIGNED_INT.apply(string) == result
 
 
 @pytest.mark.parametrize(
     ("string", "result"),
     [
         ("3.14", (3.14, 4)),  # CLASSIC
         ("3.0", (3.0, 3)),  # POST-COMMA TRAILING ZERO
@@ -166,29 +151,29 @@
         ("0.92", (0.92, 4)),  # ZERO-DIGIT
         (".92", (0.92, 3)),  # IMPLICIT ZERO-DIGIT
         ("3.", (3.0, 2)),  # IMPLICIT POST-COMMA ZERO
         ("", NOT_APPLIED),  # EMPTY
     ],
 )
 def test_decimal(string: str, result: RuleResult) -> None:
-    assert DECIMAL.apply(string) == result
+    assert common.DECIMAL.apply(string) == result
 
 
 @pytest.mark.parametrize(
     ("string", "result"),
     [
         ("3", (3, 1)),  # CLASSIC: DIGIT
         ("D", (13, 1)),  # CLASSIC: UC LETTER
         ("a", (10, 1)),  # CLASSIC: LC LETTER
         ("g", NOT_APPLIED),  # INVALID HEX VALUE
         ("", NOT_APPLIED),  # EMPTY
     ],
 )
 def test_hexdigit(string: str, result: RuleResult) -> None:
-    assert HEXDIGIT.apply(string) == result
+    assert common.HEXDIGIT.apply(string) == result
 
 
 @pytest.mark.parametrize(
     ("string", "result"),
     [
         ("W", ("W", 1)),  # ONE LETTER
         ("_", ("_", 1)),  # ONE USCORE
@@ -202,29 +187,29 @@
         ("_word0", ("_word0", 6)),  # 'PRIVATE' TRAILING DIGIT
         ("0", NOT_APPLIED),  # SINGLE DIGIT
         ("69420", NOT_APPLIED),  # N-DIGITS
         ("", NOT_APPLIED),  # EMPTY
     ],
 )
 def test_c_name(string: str, result: RuleResult) -> None:
-    assert C_NAME.apply(string) == result
+    assert common.C_NAME.apply(string) == result
 
 
 @pytest.mark.parametrize(
     ("string", "result"),
     [
         ("\n", ("\n", 1)),  # LF NEWLINE
         ("\r\n", ("\r\n", 2)),  # CRLF NEWLINE
         ("\r", NOT_APPLIED),  # CR NEWLINE
         ("\\n", NOT_APPLIED),  # ESC LF NEWLINE
         ("", NOT_APPLIED),  # EMPTY
     ],
 )
 def test_newline(string: str, result: RuleResult) -> None:
-    assert NEWLINE.apply(string) == result
+    assert common.NEWLINE.apply(string) == result
 
 
 @pytest.mark.parametrize(
     ("string", "result"),
     [
         ("1e3", (1_000.0, 3)),  # INT, LC E, INT
         ("1e+3", (1_000.0, 4)),  # INT, E, POS INT
@@ -233,15 +218,15 @@
         ("1.0e3", (1_000.0, 5)),  # DECIMAL, E, INT
         ("1.0e+3", (1_000.0, 6)),  # DECIMAL, E, POS INT
         ("1.0e-3", (0.001, 6)),  # DECIMAL, E, NEG INT
         ("", NOT_APPLIED),  # EMPTY
     ],
 )
 def test_float(string: str, result: RuleResult) -> None:
-    assert FLOAT.apply(string) == result
+    assert common.FLOAT.apply(string) == result
 
 
 @pytest.mark.parametrize(
     ("string", "result"),
     [
         ("+1e3", (1_000.0, 4)),  # POS INT, E, INT
         ("-1e3", (-1_000.0, 4)),  # NEG INT, E, INT
@@ -251,16 +236,47 @@
         ("-1.0e3", (-1_000.0, 6)),  # NEG DECIMAL, E, INT
         ("+1.0e+3", (1_000.0, 7)),  # POS DECIMAL, E, POS INT
         ("+1.0e-3", (0.001, 7)),  # POS DECIMAL, E, NEG INT
         ("", NOT_APPLIED),  # EMPTY
     ],
 )
 def test_signed_float(string: str, result: RuleResult) -> None:
-    assert SIGNED_FLOAT.apply(string) == result
+    assert common.SIGNED_FLOAT.apply(string) == result
 
 
 def test_number() -> None:
-    assert Crossandra(rules=[NUMBER]).tokenize("1.0") == [1.0]
+    assert common.NUMBER.apply("1.0") == (1.0, 3)
 
 
 def test_signed_number() -> None:
-    assert Crossandra(rules=[SIGNED_NUMBER]).tokenize("-1.0") == [-1.0]
+    assert common.SIGNED_NUMBER.apply("-1.0") == (-1.0, 4)
+
+
+@pytest.mark.parametrize(
+    ("string", "result"),
+    [("1", (1, 1)), ("-1", (-1, 2)), ("+1", (1, 2))],
+)
+def test_any_int(string: str, result: RuleResult) -> None:
+    assert common.ANY_INT.apply(string) == result
+
+
+@pytest.mark.parametrize(
+    ("string", "result"),
+    [("1.0", (1.0, 3)), ("-1.0", (-1.0, 4)), ("+1.0", (1.0, 4))],
+)
+def test_any_float(string: str, result: RuleResult) -> None:
+    assert common.ANY_FLOAT.apply(string) == result
+
+
+@pytest.mark.parametrize(
+    ("string", "result"),
+    [
+        ("1", (1, 1)),
+        ("-1", (-1, 2)),
+        ("+1", (1, 2)),
+        ("1.05", (1.05, 4)),
+        ("-1.05", (-1.05, 5)),
+        ("+1.05", (1.05, 5)),
+    ],
+)
+def test_any_number(string: str, result: RuleResult) -> None:
+    assert common.ANY_NUMBER.apply(string) == result
```

