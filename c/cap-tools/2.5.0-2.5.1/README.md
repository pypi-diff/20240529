# Comparing `tmp/cap_tools-2.5.0.tar.gz` & `tmp/cap_tools-2.5.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "cap_tools-2.5.0.tar", max compression
+gzip compressed data, was "cap_tools-2.5.1.tar", max compression
```

## Comparing `cap_tools-2.5.0.tar` & `cap_tools-2.5.1.tar`

### file list

```diff
@@ -1,7 +1,8 @@
--rw-r--r--   0        0        0     1069 2024-05-27 19:41:22.721122 cap_tools-2.5.0/LICENSE
--rw-r--r--   0        0        0     5301 2024-05-27 19:41:22.721122 cap_tools-2.5.0/README.md
--rw-r--r--   0        0        0     1978 2024-05-27 19:41:22.721122 cap_tools-2.5.0/pyproject.toml
--rw-r--r--   0        0        0      530 2024-05-27 19:41:22.721122 cap_tools-2.5.0/src/cap_tools/__init__.py
--rw-r--r--   0        0        0    15865 2024-05-27 19:41:22.721122 cap_tools-2.5.0/src/cap_tools/models.py
--rw-r--r--   0        0        0      321 2024-05-27 19:41:22.725122 cap_tools-2.5.0/src/cap_tools/utils.py
--rw-r--r--   0        0        0     5832 1970-01-01 00:00:00.000000 cap_tools-2.5.0/PKG-INFO
+-rw-r--r--   0        0        0     1069 2024-05-29 17:06:27.212595 cap_tools-2.5.1/LICENSE
+-rw-r--r--   0        0        0     5301 2024-05-29 17:06:27.212595 cap_tools-2.5.1/README.md
+-rw-r--r--   0        0        0     1989 2024-05-29 17:06:27.212595 cap_tools-2.5.1/pyproject.toml
+-rw-r--r--   0        0        0      530 2024-05-29 17:06:27.216595 cap_tools-2.5.1/src/cap_tools/__init__.py
+-rw-r--r--   0        0        0    15850 2024-05-29 17:06:27.216595 cap_tools-2.5.1/src/cap_tools/models.py
+-rw-r--r--   0        0        0        0 2024-05-29 17:06:27.216595 cap_tools-2.5.1/src/cap_tools/py.typed
+-rw-r--r--   0        0        0      321 2024-05-29 17:06:27.216595 cap_tools-2.5.1/src/cap_tools/utils.py
+-rw-r--r--   0        0        0     5832 1970-01-01 00:00:00.000000 cap_tools-2.5.1/PKG-INFO
```

### Comparing `cap_tools-2.5.0/LICENSE` & `cap_tools-2.5.1/LICENSE`

 * *Files identical despite different names*

### Comparing `cap_tools-2.5.0/README.md` & `cap_tools-2.5.1/README.md`

 * *Files identical despite different names*

### Comparing `cap_tools-2.5.0/pyproject.toml` & `cap_tools-2.5.1/pyproject.toml`

 * *Files 4% similar despite different names*

```diff
@@ -14,19 +14,19 @@
 update_changelog_on_bump = true
 
 [tool.coverage.run]
 source = ["src", "tests"]
 
 [tool.mypy]
 strict = true
-files = "src"
+files = ["src", "tests"]
 
 [tool.poetry]
 name = "cap-tools"
-version = "2.5.0"
+version = "2.5.1"
 description = "Python data bindings for the Common Alerting Protocol Version."
 authors = ["Björn Reetz <git@bjoern-reetz.de>"]
 readme = "README.md"
 packages = [{include = "cap_tools", from = "src"}]
 
 [tool.poetry.dependencies]
 python = "^3.10"
```

### Comparing `cap_tools-2.5.0/src/cap_tools/__init__.py` & `cap_tools-2.5.1/src/cap_tools/__init__.py`

 * *Files identical despite different names*

### Comparing `cap_tools-2.5.0/src/cap_tools/models.py` & `cap_tools-2.5.1/src/cap_tools/models.py`

 * *Files 0% similar despite different names*

```diff
@@ -277,15 +277,15 @@
         default=None,
         metadata={
             "type": "Element",
             "namespace": "urn:oasis:names:tc:emergency:cap:1.2",
         },
     )
 
-    def geocodes_to_dict(self) -> MultiDict[str, str]:
+    def geocodes_to_dict(self) -> MultiDict[str]:
         """Return the Area.geocodes as a MultiDict."""
         return MultiDict(
             (geocode.value_name.value, geocode.value.value) for geocode in self.geocodes
         )
 
     def geocodes_from_dict(self, geocodes: Mapping[str, str]) -> None:
         """Overwrite Area.geocodes with values derived from the given mapping (e.g. dict or MultiDict)."""
@@ -470,27 +470,27 @@
         will set `Info.language` to `None`. Retrieving the language then via `Info.get_language`
         will correctly return "en-US".
 
         If you want to set the language to 'en-US' explicitly, use `Info.language = "en-US"` instead.
         """
         self.language = None if language == DEFAULT_LANGUAGE else language
 
-    def event_codes_to_dict(self) -> MultiDict[str, str]:
+    def event_codes_to_dict(self) -> MultiDict[str]:
         return MultiDict(
             (event_code.value_name.value, event_code.value.value)
             for event_code in self.event_codes
         )
 
     def event_codes_from_dict(self, event_codes: Mapping[str, str]) -> None:
         self.event_codes = [
             EventCode(ValueName(name), Value(value))
             for name, value in event_codes.items()
         ]
 
-    def parameters_to_dict(self) -> MultiDict[str, str]:
+    def parameters_to_dict(self) -> MultiDict[str]:
         return MultiDict(
             (parameter.value_name.value, parameter.value.value)
             for parameter in self.parameters
         )
 
     def parameters_from_dict(self, parameters: Mapping[str, str]) -> None:
         self.parameters = [
```

### Comparing `cap_tools-2.5.0/PKG-INFO` & `cap_tools-2.5.1/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: cap-tools
-Version: 2.5.0
+Version: 2.5.1
 Summary: Python data bindings for the Common Alerting Protocol Version.
 Author: Björn Reetz
 Author-email: git@bjoern-reetz.de
 Requires-Python: >=3.10,<4.0
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
```

