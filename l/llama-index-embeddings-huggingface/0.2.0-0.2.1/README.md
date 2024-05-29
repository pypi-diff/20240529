# Comparing `tmp/llama_index_embeddings_huggingface-0.2.0.tar.gz` & `tmp/llama_index_embeddings_huggingface-0.2.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "llama_index_embeddings_huggingface-0.2.0.tar", max compression
+gzip compressed data, was "llama_index_embeddings_huggingface-0.2.1.tar", max compression
```

## Comparing `llama_index_embeddings_huggingface-0.2.0.tar` & `llama_index_embeddings_huggingface-0.2.1.tar`

### file list

```diff
@@ -1,7 +1,7 @@
--rw-r--r--   0        0        0       49 2024-03-26 16:43:17.182311 llama_index_embeddings_huggingface-0.2.0/README.md
--rw-r--r--   0        0        0      283 2024-03-26 16:43:17.182311 llama_index_embeddings_huggingface-0.2.0/llama_index/embeddings/huggingface/__init__.py
--rw-r--r--   0        0        0    12710 2024-03-26 16:43:17.182311 llama_index_embeddings_huggingface-0.2.0/llama_index/embeddings/huggingface/base.py
--rw-r--r--   0        0        0     2260 2024-03-26 16:43:17.182311 llama_index_embeddings_huggingface-0.2.0/llama_index/embeddings/huggingface/pooling.py
--rw-r--r--   0        0        0     3198 2024-03-26 16:43:17.182311 llama_index_embeddings_huggingface-0.2.0/llama_index/embeddings/huggingface/utils.py
--rw-r--r--   0        0        0     1638 2024-03-26 16:43:17.182311 llama_index_embeddings_huggingface-0.2.0/pyproject.toml
--rw-r--r--   0        0        0      725 1970-01-01 00:00:00.000000 llama_index_embeddings_huggingface-0.2.0/PKG-INFO
+-rw-r--r--   0        0        0       49 2024-05-29 03:18:45.104596 llama_index_embeddings_huggingface-0.2.1/README.md
+-rw-r--r--   0        0        0      283 2024-05-29 03:18:45.104596 llama_index_embeddings_huggingface-0.2.1/llama_index/embeddings/huggingface/__init__.py
+-rw-r--r--   0        0        0    12710 2024-05-29 03:18:45.104596 llama_index_embeddings_huggingface-0.2.1/llama_index/embeddings/huggingface/base.py
+-rw-r--r--   0        0        0     2260 2024-05-29 03:18:45.104596 llama_index_embeddings_huggingface-0.2.1/llama_index/embeddings/huggingface/pooling.py
+-rw-r--r--   0        0        0     3198 2024-05-29 03:18:45.104596 llama_index_embeddings_huggingface-0.2.1/llama_index/embeddings/huggingface/utils.py
+-rw-r--r--   0        0        0     1638 2024-05-29 03:18:45.104596 llama_index_embeddings_huggingface-0.2.1/pyproject.toml
+-rw-r--r--   0        0        0      725 1970-01-01 00:00:00.000000 llama_index_embeddings_huggingface-0.2.1/PKG-INFO
```

### Comparing `llama_index_embeddings_huggingface-0.2.0/llama_index/embeddings/huggingface/base.py` & `llama_index_embeddings_huggingface-0.2.1/llama_index/embeddings/huggingface/base.py`

 * *Files identical despite different names*

### Comparing `llama_index_embeddings_huggingface-0.2.0/llama_index/embeddings/huggingface/pooling.py` & `llama_index_embeddings_huggingface-0.2.1/llama_index/embeddings/huggingface/pooling.py`

 * *Files identical despite different names*

### Comparing `llama_index_embeddings_huggingface-0.2.0/llama_index/embeddings/huggingface/utils.py` & `llama_index_embeddings_huggingface-0.2.1/llama_index/embeddings/huggingface/utils.py`

 * *Files identical despite different names*

### Comparing `llama_index_embeddings_huggingface-0.2.0/pyproject.toml` & `llama_index_embeddings_huggingface-0.2.1/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -24,15 +24,15 @@
 [tool.poetry]
 authors = ["Your Name <you@example.com>"]
 description = "llama-index embeddings huggingface integration"
 exclude = ["**/BUILD"]
 license = "MIT"
 name = "llama-index-embeddings-huggingface"
 readme = "README.md"
-version = "0.2.0"
+version = "0.2.1"
 
 [tool.poetry.dependencies]
 python = ">=3.8.1,<4.0"
 llama-index-core = "^0.10.1"
 sentence-transformers = "^2.6.1"
 
 [tool.poetry.dependencies.huggingface-hub]
```

### Comparing `llama_index_embeddings_huggingface-0.2.0/PKG-INFO` & `llama_index_embeddings_huggingface-0.2.1/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: llama-index-embeddings-huggingface
-Version: 0.2.0
+Version: 0.2.1
 Summary: llama-index embeddings huggingface integration
 License: MIT
 Author: Your Name
 Author-email: you@example.com
 Requires-Python: >=3.8.1,<4.0
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
```

