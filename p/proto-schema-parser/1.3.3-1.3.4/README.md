# Comparing `tmp/proto_schema_parser-1.3.3.tar.gz` & `tmp/proto_schema_parser-1.3.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "proto_schema_parser-1.3.3.tar", last modified: Thu Apr 18 16:35:23 2024, max compression
+gzip compressed data, was "proto_schema_parser-1.3.4.tar", last modified: Tue May 28 22:56:38 2024, max compression
```

## Comparing `proto_schema_parser-1.3.3.tar` & `proto_schema_parser-1.3.4.tar`

### file list

```diff
@@ -1,19 +1,20 @@
--rw-r--r--   0        0        0     1072 2024-04-18 16:35:11.435788 proto_schema_parser-1.3.3/LICENSE
--rw-r--r--   0        0        0     2968 2024-04-18 16:35:11.435788 proto_schema_parser-1.3.3/README.md
--rw-r--r--   0        0        0      157 2024-04-18 16:35:11.447788 proto_schema_parser-1.3.3/proto_schema_parser/__init__.py
--rw-r--r--   0        0        0    23013 2024-04-18 16:35:11.447788 proto_schema_parser-1.3.3/proto_schema_parser/antlr/ProtobufLexer.interp
--rw-r--r--   0        0        0    22508 2024-04-18 16:35:11.447788 proto_schema_parser-1.3.3/proto_schema_parser/antlr/ProtobufLexer.py
--rw-r--r--   0        0        0     1307 2024-04-18 16:35:11.447788 proto_schema_parser-1.3.3/proto_schema_parser/antlr/ProtobufLexer.tokens
--rw-r--r--   0        0        0    30561 2024-04-18 16:35:11.447788 proto_schema_parser-1.3.3/proto_schema_parser/antlr/ProtobufParser.interp
--rw-r--r--   0        0        0   274553 2024-04-18 16:35:11.447788 proto_schema_parser-1.3.3/proto_schema_parser/antlr/ProtobufParser.py
--rw-r--r--   0        0        0     1307 2024-04-18 16:35:11.447788 proto_schema_parser-1.3.3/proto_schema_parser/antlr/ProtobufParser.tokens
--rw-r--r--   0        0        0    30970 2024-04-18 16:35:11.447788 proto_schema_parser-1.3.3/proto_schema_parser/antlr/ProtobufParserListener.py
--rw-r--r--   0        0        0    18335 2024-04-18 16:35:11.447788 proto_schema_parser-1.3.3/proto_schema_parser/antlr/ProtobufParserVisitor.py
--rw-r--r--   0        0        0        0 2024-04-18 16:35:11.447788 proto_schema_parser-1.3.3/proto_schema_parser/antlr/__init__.py
--rw-r--r--   0        0        0     5720 2024-04-18 16:35:11.447788 proto_schema_parser-1.3.3/proto_schema_parser/ast.py
--rw-r--r--   0        0        0     9879 2024-04-18 16:35:11.447788 proto_schema_parser-1.3.3/proto_schema_parser/generator.py
--rw-r--r--   0        0        0    11078 2024-04-18 16:35:11.447788 proto_schema_parser-1.3.3/proto_schema_parser/parser.py
--rw-r--r--   0        0        0     1407 2024-04-18 16:35:23.647794 proto_schema_parser-1.3.3/pyproject.toml
--rw-r--r--   0        0        0    15798 2024-04-18 16:35:11.447788 proto_schema_parser-1.3.3/tests/test_generator.py
--rw-r--r--   0        0        0    31399 2024-04-18 16:35:11.451788 proto_schema_parser-1.3.3/tests/test_parser.py
--rw-r--r--   0        0        0     3254 1970-01-01 00:00:00.000000 proto_schema_parser-1.3.3/PKG-INFO
+-rw-r--r--   0        0        0     1072 2024-05-28 22:56:22.202997 proto_schema_parser-1.3.4/LICENSE
+-rw-r--r--   0        0        0     2538 2024-05-28 22:56:22.202997 proto_schema_parser-1.3.4/README.md
+-rw-r--r--   0        0        0      157 2024-05-28 22:56:22.214997 proto_schema_parser-1.3.4/proto_schema_parser/__init__.py
+-rw-r--r--   0        0        0    23013 2024-05-28 22:56:22.214997 proto_schema_parser-1.3.4/proto_schema_parser/antlr/ProtobufLexer.interp
+-rw-r--r--   0        0        0    22508 2024-05-28 22:56:22.214997 proto_schema_parser-1.3.4/proto_schema_parser/antlr/ProtobufLexer.py
+-rw-r--r--   0        0        0     1307 2024-05-28 22:56:22.214997 proto_schema_parser-1.3.4/proto_schema_parser/antlr/ProtobufLexer.tokens
+-rw-r--r--   0        0        0    30561 2024-05-28 22:56:22.214997 proto_schema_parser-1.3.4/proto_schema_parser/antlr/ProtobufParser.interp
+-rw-r--r--   0        0        0   274553 2024-05-28 22:56:22.214997 proto_schema_parser-1.3.4/proto_schema_parser/antlr/ProtobufParser.py
+-rw-r--r--   0        0        0     1307 2024-05-28 22:56:22.214997 proto_schema_parser-1.3.4/proto_schema_parser/antlr/ProtobufParser.tokens
+-rw-r--r--   0        0        0    30970 2024-05-28 22:56:22.214997 proto_schema_parser-1.3.4/proto_schema_parser/antlr/ProtobufParserListener.py
+-rw-r--r--   0        0        0    18335 2024-05-28 22:56:22.214997 proto_schema_parser-1.3.4/proto_schema_parser/antlr/ProtobufParserVisitor.py
+-rw-r--r--   0        0        0        0 2024-05-28 22:56:22.214997 proto_schema_parser-1.3.4/proto_schema_parser/antlr/__init__.py
+-rw-r--r--   0        0        0     5720 2024-05-28 22:56:22.214997 proto_schema_parser-1.3.4/proto_schema_parser/ast.py
+-rw-r--r--   0        0        0     9879 2024-05-28 22:56:22.214997 proto_schema_parser-1.3.4/proto_schema_parser/generator.py
+-rw-r--r--   0        0        0    11078 2024-05-28 22:56:22.214997 proto_schema_parser-1.3.4/proto_schema_parser/parser.py
+-rw-r--r--   0        0        0        0 2024-05-28 22:56:22.214997 proto_schema_parser-1.3.4/proto_schema_parser/py.typed
+-rw-r--r--   0        0        0     1407 2024-05-28 22:56:38.567114 proto_schema_parser-1.3.4/pyproject.toml
+-rw-r--r--   0        0        0    15798 2024-05-28 22:56:22.214997 proto_schema_parser-1.3.4/tests/test_generator.py
+-rw-r--r--   0        0        0    31399 2024-05-28 22:56:22.214997 proto_schema_parser-1.3.4/tests/test_parser.py
+-rw-r--r--   0        0        0     2824 1970-01-01 00:00:00.000000 proto_schema_parser-1.3.4/PKG-INFO
```

### Comparing `proto_schema_parser-1.3.3/LICENSE` & `proto_schema_parser-1.3.4/LICENSE`

 * *Files identical despite different names*

### Comparing `proto_schema_parser-1.3.3/README.md` & `proto_schema_parser-1.3.4/README.md`

 * *Files 8% similar despite different names*

```diff
@@ -41,32 +41,39 @@
 """
 
 result = Parser().parse(text)
 ```
 
 This will return an AST object (`ast.File`) representing the parsed protobuf schema.
 
-```
-File(syntax='proto3',
-     file_elements=[Message(name='SearchRequest',
-                            elements=[Field(name='query',
-                                            number=1,
-                                            type='string',
-                                            cardinality=None,
-                                            options=[]),
-                                      Field(name='page_number',
-                                            number=2,
-                                            type='int32',
-                                            cardinality=None,
-                                            options=[]),
-                                      Field(name='result_per_page',
-                                            number=3,
-                                            type='int32',
-                                            cardinality=None,
-                                            options=[])])])
+```python
+File(
+  syntax='proto3',
+  file_elements=[
+    Message(
+      name='SearchRequest',
+      elements=[
+        Field(
+          name='query',
+          number=1,
+          type='string',
+          cardinality=None,
+          options=[]),
+        Field(
+          name='page_number',
+          number=2,
+          type='int32',
+          cardinality=None,
+          options=[]),
+        Field(
+          name='result_per_page',
+          number=3,
+          type='int32',
+          cardinality=None,
+          options=[])])])
 ```
 
 To write the AST back to a protobuf schema, create a `Generator` object and call the `generate` method:
 
 ```python
 from proto_schema_parser.generator import Generator
```

### Comparing `proto_schema_parser-1.3.3/proto_schema_parser/antlr/ProtobufLexer.interp` & `proto_schema_parser-1.3.4/proto_schema_parser/antlr/ProtobufLexer.interp`

 * *Files identical despite different names*

### Comparing `proto_schema_parser-1.3.3/proto_schema_parser/antlr/ProtobufLexer.py` & `proto_schema_parser-1.3.4/proto_schema_parser/antlr/ProtobufLexer.py`

 * *Files identical despite different names*

### Comparing `proto_schema_parser-1.3.3/proto_schema_parser/antlr/ProtobufLexer.tokens` & `proto_schema_parser-1.3.4/proto_schema_parser/antlr/ProtobufLexer.tokens`

 * *Files identical despite different names*

### Comparing `proto_schema_parser-1.3.3/proto_schema_parser/antlr/ProtobufParser.interp` & `proto_schema_parser-1.3.4/proto_schema_parser/antlr/ProtobufParser.interp`

 * *Files identical despite different names*

### Comparing `proto_schema_parser-1.3.3/proto_schema_parser/antlr/ProtobufParser.py` & `proto_schema_parser-1.3.4/proto_schema_parser/antlr/ProtobufParser.py`

 * *Files identical despite different names*

### Comparing `proto_schema_parser-1.3.3/proto_schema_parser/antlr/ProtobufParser.tokens` & `proto_schema_parser-1.3.4/proto_schema_parser/antlr/ProtobufParser.tokens`

 * *Files identical despite different names*

### Comparing `proto_schema_parser-1.3.3/proto_schema_parser/antlr/ProtobufParserListener.py` & `proto_schema_parser-1.3.4/proto_schema_parser/antlr/ProtobufParserListener.py`

 * *Files identical despite different names*

### Comparing `proto_schema_parser-1.3.3/proto_schema_parser/antlr/ProtobufParserVisitor.py` & `proto_schema_parser-1.3.4/proto_schema_parser/antlr/ProtobufParserVisitor.py`

 * *Files identical despite different names*

### Comparing `proto_schema_parser-1.3.3/proto_schema_parser/ast.py` & `proto_schema_parser-1.3.4/proto_schema_parser/ast.py`

 * *Files identical despite different names*

### Comparing `proto_schema_parser-1.3.3/proto_schema_parser/generator.py` & `proto_schema_parser-1.3.4/proto_schema_parser/generator.py`

 * *Files identical despite different names*

### Comparing `proto_schema_parser-1.3.3/proto_schema_parser/parser.py` & `proto_schema_parser-1.3.4/proto_schema_parser/parser.py`

 * *Files identical despite different names*

### Comparing `proto_schema_parser-1.3.3/pyproject.toml` & `proto_schema_parser-1.3.4/pyproject.toml`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [project]
 name = "proto-schema-parser"
-version = "1.3.3"
+version = "1.3.4"
 description = "A Pure Python Protobuf .proto Parser"
 authors = [
     { name = "Chris Riccomini", email = "criccomini@apache.org" },
 ]
 dependencies = [
     "antlr4-python3-runtime>=4.13.0",
 ]
```

### Comparing `proto_schema_parser-1.3.3/tests/test_generator.py` & `proto_schema_parser-1.3.4/tests/test_generator.py`

 * *Files identical despite different names*

### Comparing `proto_schema_parser-1.3.3/tests/test_parser.py` & `proto_schema_parser-1.3.4/tests/test_parser.py`

 * *Files identical despite different names*

### Comparing `proto_schema_parser-1.3.3/PKG-INFO` & `proto_schema_parser-1.3.4/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: proto-schema-parser
-Version: 1.3.3
+Version: 1.3.4
 Summary: A Pure Python Protobuf .proto Parser
 Author-Email: Chris Riccomini <criccomini@apache.org>
 License: MIT
 Requires-Python: >=3.8
 Requires-Dist: antlr4-python3-runtime>=4.13.0
 Description-Content-Type: text/markdown
 
@@ -51,32 +51,39 @@
 """
 
 result = Parser().parse(text)
 ```
 
 This will return an AST object (`ast.File`) representing the parsed protobuf schema.
 
-```
-File(syntax='proto3',
-     file_elements=[Message(name='SearchRequest',
-                            elements=[Field(name='query',
-                                            number=1,
-                                            type='string',
-                                            cardinality=None,
-                                            options=[]),
-                                      Field(name='page_number',
-                                            number=2,
-                                            type='int32',
-                                            cardinality=None,
-                                            options=[]),
-                                      Field(name='result_per_page',
-                                            number=3,
-                                            type='int32',
-                                            cardinality=None,
-                                            options=[])])])
+```python
+File(
+  syntax='proto3',
+  file_elements=[
+    Message(
+      name='SearchRequest',
+      elements=[
+        Field(
+          name='query',
+          number=1,
+          type='string',
+          cardinality=None,
+          options=[]),
+        Field(
+          name='page_number',
+          number=2,
+          type='int32',
+          cardinality=None,
+          options=[]),
+        Field(
+          name='result_per_page',
+          number=3,
+          type='int32',
+          cardinality=None,
+          options=[])])])
 ```
 
 To write the AST back to a protobuf schema, create a `Generator` object and call the `generate` method:
 
 ```python
 from proto_schema_parser.generator import Generator
```

