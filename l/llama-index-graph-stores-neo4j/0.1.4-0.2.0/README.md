# Comparing `tmp/llama_index_graph_stores_neo4j-0.1.4.tar.gz` & `tmp/llama_index_graph_stores_neo4j-0.2.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "llama_index_graph_stores_neo4j-0.1.4.tar", max compression
+gzip compressed data, was "llama_index_graph_stores_neo4j-0.2.0.tar", max compression
```

## Comparing `llama_index_graph_stores_neo4j-0.1.4.tar` & `llama_index_graph_stores_neo4j-0.2.0.tar`

### file list

```diff
@@ -1,5 +1,6 @@
--rw-r--r--   0        0        0       45 2024-03-28 17:15:29.685162 llama_index_graph_stores_neo4j-0.1.4/README.md
--rw-r--r--   0        0        0       95 2024-03-28 17:15:29.685162 llama_index_graph_stores_neo4j-0.1.4/llama_index/graph_stores/neo4j/__init__.py
--rw-r--r--   0        0        0     9432 2024-03-28 17:15:29.685162 llama_index_graph_stores_neo4j-0.1.4/llama_index/graph_stores/neo4j/base.py
--rw-r--r--   0        0        0     1469 2024-03-28 17:15:29.685162 llama_index_graph_stores_neo4j-0.1.4/pyproject.toml
--rw-r--r--   0        0        0      645 1970-01-01 00:00:00.000000 llama_index_graph_stores_neo4j-0.1.4/PKG-INFO
+-rw-r--r--   0        0        0       45 2024-05-29 03:18:45.120596 llama_index_graph_stores_neo4j-0.2.0/README.md
+-rw-r--r--   0        0        0      188 2024-05-29 03:18:45.120596 llama_index_graph_stores_neo4j-0.2.0/llama_index/graph_stores/neo4j/__init__.py
+-rw-r--r--   0        0        0     9432 2024-05-29 03:18:45.120596 llama_index_graph_stores_neo4j-0.2.0/llama_index/graph_stores/neo4j/base.py
+-rw-r--r--   0        0        0    33442 2024-05-29 03:18:45.120596 llama_index_graph_stores_neo4j-0.2.0/llama_index/graph_stores/neo4j/neo4j_property_graph.py
+-rw-r--r--   0        0        0     1499 2024-05-29 03:18:45.120596 llama_index_graph_stores_neo4j-0.2.0/pyproject.toml
+-rw-r--r--   0        0        0      646 1970-01-01 00:00:00.000000 llama_index_graph_stores_neo4j-0.2.0/PKG-INFO
```

### Comparing `llama_index_graph_stores_neo4j-0.1.4/llama_index/graph_stores/neo4j/base.py` & `llama_index_graph_stores_neo4j-0.2.0/llama_index/graph_stores/neo4j/base.py`

 * *Files identical despite different names*

### Comparing `llama_index_graph_stores_neo4j-0.1.4/pyproject.toml` & `llama_index_graph_stores_neo4j-0.2.0/pyproject.toml`

 * *Files 12% similar despite different names*

```diff
@@ -9,33 +9,34 @@
 
 [tool.llamahub]
 contains_example = false
 import_path = "llama_index.graph_stores.neo4j"
 
 [tool.llamahub.class_authors]
 Neo4jGraphStore = "llama-index"
+Neo4jPGStore = "llama-index"
 
 [tool.mypy]
 disallow_untyped_defs = true
 exclude = ["_static", "build", "examples", "notebooks", "venv"]
 ignore_missing_imports = true
 python_version = "3.8"
 
 [tool.poetry]
 authors = ["Your Name <you@example.com>"]
 description = "llama-index graph stores neo4j integration"
 exclude = ["**/BUILD"]
 license = "MIT"
 name = "llama-index-graph-stores-neo4j"
 readme = "README.md"
-version = "0.1.4"
+version = "0.2.0"
 
 [tool.poetry.dependencies]
 python = ">=3.8.1,<4.0"
-llama-index-core = "^0.10.1"
+llama-index-core = "^0.10.40"
 neo4j = "^5.16.0"
 
 [tool.poetry.group.dev.dependencies]
 ipython = "8.10.0"
 jupyter = "^1.0.0"
 mypy = "0.991"
 pre-commit = "3.2.0"
```

### Comparing `llama_index_graph_stores_neo4j-0.1.4/PKG-INFO` & `llama_index_graph_stores_neo4j-0.2.0/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,19 +1,19 @@
 Metadata-Version: 2.1
 Name: llama-index-graph-stores-neo4j
-Version: 0.1.4
+Version: 0.2.0
 Summary: llama-index graph stores neo4j integration
 License: MIT
 Author: Your Name
 Author-email: you@example.com
 Requires-Python: >=3.8.1,<4.0
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
-Requires-Dist: llama-index-core (>=0.10.1,<0.11.0)
+Requires-Dist: llama-index-core (>=0.10.40,<0.11.0)
 Requires-Dist: neo4j (>=5.16.0,<6.0.0)
 Description-Content-Type: text/markdown
 
 # LlamaIndex Graph Stores Integration: Neo4J
```

