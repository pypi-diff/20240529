# Comparing `tmp/chat_rag-0.1.69.tar.gz` & `tmp/chat_rag-0.1.70.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "chat_rag-0.1.69.tar", max compression
+gzip compressed data, was "chat_rag-0.1.70.tar", max compression
```

## Comparing `chat_rag-0.1.69.tar` & `chat_rag-0.1.70.tar`

### file list

```diff
@@ -1,36 +1,36 @@
--rw-r--r--   0        0        0     1083 2024-02-07 11:08:45.534329 chat_rag-0.1.69/LICENSE
--rw-r--r--   0        0        0     1666 2024-02-07 11:08:45.534329 chat_rag-0.1.69/README.md
--rw-r--r--   0        0        0       68 2024-04-25 12:19:16.531849 chat_rag-0.1.69/chat_rag/__init__.py
--rw-r--r--   0        0        0     3448 2024-04-27 16:28:16.074506 chat_rag-0.1.69/chat_rag/async_rag.py
--rw-r--r--   0        0        0        0 2024-02-07 11:08:45.534329 chat_rag-0.1.69/chat_rag/data/__init__.py
--rw-r--r--   0        0        0      788 2024-02-07 11:08:45.534329 chat_rag-0.1.69/chat_rag/data/models.py
--rw-r--r--   0        0        0    10492 2024-04-25 12:19:16.531849 chat_rag-0.1.69/chat_rag/data/parsers.py
--rw-r--r--   0        0        0    13027 2024-03-06 16:38:44.353919 chat_rag-0.1.69/chat_rag/data/splitters.py
--rw-r--r--   0        0        0      897 2024-02-26 10:37:33.379027 chat_rag-0.1.69/chat_rag/exceptions.py
--rw-r--r--   0        0        0        0 2024-02-07 11:08:45.534329 chat_rag-0.1.69/chat_rag/inf_retrieval/__init__.py
--rw-r--r--   0        0        0     3924 2024-02-07 11:08:45.534329 chat_rag-0.1.69/chat_rag/inf_retrieval/check_answ_questions.py
--rw-r--r--   0        0        0     2450 2024-02-07 11:08:45.534329 chat_rag-0.1.69/chat_rag/inf_retrieval/cross_encoder.py
--rw-r--r--   0        0        0      141 2024-02-07 11:08:45.534329 chat_rag-0.1.69/chat_rag/inf_retrieval/embedding_models/__init__.py
--rw-r--r--   0        0        0     4617 2024-02-07 11:08:45.534329 chat_rag-0.1.69/chat_rag/inf_retrieval/embedding_models/base_model.py
--rw-r--r--   0        0        0     1494 2024-04-18 10:45:56.532544 chat_rag-0.1.69/chat_rag/inf_retrieval/embedding_models/e5_model.py
--rw-r--r--   0        0        0     4693 2024-02-07 11:08:45.534329 chat_rag-0.1.69/chat_rag/inf_retrieval/query_generator.py
--rw-r--r--   0        0        0     3918 2024-05-29 15:03:20.869731 chat_rag-0.1.69/chat_rag/inf_retrieval/reference_checker.py
--rw-r--r--   0        0        0      240 2024-04-25 12:19:16.531849 chat_rag-0.1.69/chat_rag/inf_retrieval/retrievers/__init__.py
--rw-r--r--   0        0        0     6913 2024-05-29 15:41:37.734475 chat_rag-0.1.69/chat_rag/inf_retrieval/retrievers/colbert_retriever.py
--rw-r--r--   0        0        0      856 2024-04-25 12:19:16.531849 chat_rag-0.1.69/chat_rag/inf_retrieval/retrievers/rerank_retriever.py
--rw-r--r--   0        0        0      503 2024-04-25 12:19:16.535849 chat_rag-0.1.69/chat_rag/inf_retrieval/retrievers/retriever_client.py
--rw-r--r--   0        0        0     7447 2024-02-07 11:08:45.534329 chat_rag-0.1.69/chat_rag/inf_retrieval/retrievers/semantic_retriever.py
--rw-r--r--   0        0        0      135 2024-02-07 11:08:45.534329 chat_rag-0.1.69/chat_rag/intent_detection/__init__.py
--rw-r--r--   0        0        0     1527 2024-02-07 11:08:45.534329 chat_rag-0.1.69/chat_rag/intent_detection/clusterize_text.py
--rw-r--r--   0        0        0     1419 2024-02-07 11:08:45.534329 chat_rag-0.1.69/chat_rag/intent_detection/gen_intent.py
--rw-r--r--   0        0        0      445 2024-04-25 12:19:16.535849 chat_rag-0.1.69/chat_rag/llms/__init__.py
--rw-r--r--   0        0        0     6995 2024-02-26 10:37:33.379027 chat_rag-0.1.69/chat_rag/llms/base_llm.py
--rw-r--r--   0        0        0     9040 2024-04-25 12:19:16.535849 chat_rag-0.1.69/chat_rag/llms/claude_client.py
--rw-r--r--   0        0        0     5219 2024-02-07 11:08:45.534329 chat_rag-0.1.69/chat_rag/llms/ggml_llm.py
--rw-r--r--   0        0        0     9255 2024-02-07 11:08:45.534329 chat_rag-0.1.69/chat_rag/llms/hf_llm.py
--rw-r--r--   0        0        0    10715 2024-04-25 12:19:16.535849 chat_rag-0.1.69/chat_rag/llms/mistral_client.py
--rw-r--r--   0        0        0    11021 2024-04-27 16:28:16.074506 chat_rag-0.1.69/chat_rag/llms/openai_client.py
--rw-r--r--   0        0        0    25992 2024-04-25 12:19:16.535849 chat_rag-0.1.69/chat_rag/llms/vllm_client.py
--rw-r--r--   0        0        0     3578 2024-04-25 12:19:16.535849 chat_rag-0.1.69/chat_rag/rag.py
--rw-r--r--   0        0        0      930 2024-05-29 15:44:09.914414 chat_rag-0.1.69/pyproject.toml
--rw-r--r--   0        0        0     3159 1970-01-01 00:00:00.000000 chat_rag-0.1.69/PKG-INFO
+-rw-r--r--   0        0        0     1083 2024-02-07 11:08:45.534329 chat_rag-0.1.70/LICENSE
+-rw-r--r--   0        0        0     1666 2024-02-07 11:08:45.534329 chat_rag-0.1.70/README.md
+-rw-r--r--   0        0        0       68 2024-04-25 12:19:16.531849 chat_rag-0.1.70/chat_rag/__init__.py
+-rw-r--r--   0        0        0     3448 2024-04-27 16:28:16.074506 chat_rag-0.1.70/chat_rag/async_rag.py
+-rw-r--r--   0        0        0        0 2024-02-07 11:08:45.534329 chat_rag-0.1.70/chat_rag/data/__init__.py
+-rw-r--r--   0        0        0      788 2024-02-07 11:08:45.534329 chat_rag-0.1.70/chat_rag/data/models.py
+-rw-r--r--   0        0        0    10492 2024-04-25 12:19:16.531849 chat_rag-0.1.70/chat_rag/data/parsers.py
+-rw-r--r--   0        0        0    13027 2024-03-06 16:38:44.353919 chat_rag-0.1.70/chat_rag/data/splitters.py
+-rw-r--r--   0        0        0      897 2024-02-26 10:37:33.379027 chat_rag-0.1.70/chat_rag/exceptions.py
+-rw-r--r--   0        0        0        0 2024-02-07 11:08:45.534329 chat_rag-0.1.70/chat_rag/inf_retrieval/__init__.py
+-rw-r--r--   0        0        0     3924 2024-02-07 11:08:45.534329 chat_rag-0.1.70/chat_rag/inf_retrieval/check_answ_questions.py
+-rw-r--r--   0        0        0     2450 2024-02-07 11:08:45.534329 chat_rag-0.1.70/chat_rag/inf_retrieval/cross_encoder.py
+-rw-r--r--   0        0        0      141 2024-02-07 11:08:45.534329 chat_rag-0.1.70/chat_rag/inf_retrieval/embedding_models/__init__.py
+-rw-r--r--   0        0        0     4617 2024-02-07 11:08:45.534329 chat_rag-0.1.70/chat_rag/inf_retrieval/embedding_models/base_model.py
+-rw-r--r--   0        0        0     1494 2024-04-18 10:45:56.532544 chat_rag-0.1.70/chat_rag/inf_retrieval/embedding_models/e5_model.py
+-rw-r--r--   0        0        0     4693 2024-02-07 11:08:45.534329 chat_rag-0.1.70/chat_rag/inf_retrieval/query_generator.py
+-rw-r--r--   0        0        0     3918 2024-05-29 15:03:20.869731 chat_rag-0.1.70/chat_rag/inf_retrieval/reference_checker.py
+-rw-r--r--   0        0        0      240 2024-04-25 12:19:16.531849 chat_rag-0.1.70/chat_rag/inf_retrieval/retrievers/__init__.py
+-rw-r--r--   0        0        0     6913 2024-05-29 15:41:37.734475 chat_rag-0.1.70/chat_rag/inf_retrieval/retrievers/colbert_retriever.py
+-rw-r--r--   0        0        0      856 2024-04-25 12:19:16.531849 chat_rag-0.1.70/chat_rag/inf_retrieval/retrievers/rerank_retriever.py
+-rw-r--r--   0        0        0      503 2024-04-25 12:19:16.535849 chat_rag-0.1.70/chat_rag/inf_retrieval/retrievers/retriever_client.py
+-rw-r--r--   0        0        0     7447 2024-02-07 11:08:45.534329 chat_rag-0.1.70/chat_rag/inf_retrieval/retrievers/semantic_retriever.py
+-rw-r--r--   0        0        0      135 2024-02-07 11:08:45.534329 chat_rag-0.1.70/chat_rag/intent_detection/__init__.py
+-rw-r--r--   0        0        0     1527 2024-02-07 11:08:45.534329 chat_rag-0.1.70/chat_rag/intent_detection/clusterize_text.py
+-rw-r--r--   0        0        0     1419 2024-02-07 11:08:45.534329 chat_rag-0.1.70/chat_rag/intent_detection/gen_intent.py
+-rw-r--r--   0        0        0      445 2024-04-25 12:19:16.535849 chat_rag-0.1.70/chat_rag/llms/__init__.py
+-rw-r--r--   0        0        0     6995 2024-02-26 10:37:33.379027 chat_rag-0.1.70/chat_rag/llms/base_llm.py
+-rw-r--r--   0        0        0     9040 2024-04-25 12:19:16.535849 chat_rag-0.1.70/chat_rag/llms/claude_client.py
+-rw-r--r--   0        0        0     5219 2024-02-07 11:08:45.534329 chat_rag-0.1.70/chat_rag/llms/ggml_llm.py
+-rw-r--r--   0        0        0     9255 2024-02-07 11:08:45.534329 chat_rag-0.1.70/chat_rag/llms/hf_llm.py
+-rw-r--r--   0        0        0    10715 2024-04-25 12:19:16.535849 chat_rag-0.1.70/chat_rag/llms/mistral_client.py
+-rw-r--r--   0        0        0    11021 2024-04-27 16:28:16.074506 chat_rag-0.1.70/chat_rag/llms/openai_client.py
+-rw-r--r--   0        0        0    25992 2024-04-25 12:19:16.535849 chat_rag-0.1.70/chat_rag/llms/vllm_client.py
+-rw-r--r--   0        0        0     3578 2024-04-25 12:19:16.535849 chat_rag-0.1.70/chat_rag/rag.py
+-rw-r--r--   0        0        0      930 2024-05-29 15:52:23.887052 chat_rag-0.1.70/pyproject.toml
+-rw-r--r--   0        0        0     3159 1970-01-01 00:00:00.000000 chat_rag-0.1.70/PKG-INFO
```

### Comparing `chat_rag-0.1.69/LICENSE` & `chat_rag-0.1.70/LICENSE`

 * *Files identical despite different names*

### Comparing `chat_rag-0.1.69/README.md` & `chat_rag-0.1.70/README.md`

 * *Files identical despite different names*

### Comparing `chat_rag-0.1.69/chat_rag/async_rag.py` & `chat_rag-0.1.70/chat_rag/async_rag.py`

 * *Files identical despite different names*

### Comparing `chat_rag-0.1.69/chat_rag/data/models.py` & `chat_rag-0.1.70/chat_rag/data/models.py`

 * *Files identical despite different names*

### Comparing `chat_rag-0.1.69/chat_rag/data/parsers.py` & `chat_rag-0.1.70/chat_rag/data/parsers.py`

 * *Files identical despite different names*

### Comparing `chat_rag-0.1.69/chat_rag/data/splitters.py` & `chat_rag-0.1.70/chat_rag/data/splitters.py`

 * *Files identical despite different names*

### Comparing `chat_rag-0.1.69/chat_rag/exceptions.py` & `chat_rag-0.1.70/chat_rag/exceptions.py`

 * *Files identical despite different names*

### Comparing `chat_rag-0.1.69/chat_rag/inf_retrieval/check_answ_questions.py` & `chat_rag-0.1.70/chat_rag/inf_retrieval/check_answ_questions.py`

 * *Files identical despite different names*

### Comparing `chat_rag-0.1.69/chat_rag/inf_retrieval/cross_encoder.py` & `chat_rag-0.1.70/chat_rag/inf_retrieval/cross_encoder.py`

 * *Files identical despite different names*

### Comparing `chat_rag-0.1.69/chat_rag/inf_retrieval/embedding_models/base_model.py` & `chat_rag-0.1.70/chat_rag/inf_retrieval/embedding_models/base_model.py`

 * *Files identical despite different names*

### Comparing `chat_rag-0.1.69/chat_rag/inf_retrieval/embedding_models/e5_model.py` & `chat_rag-0.1.70/chat_rag/inf_retrieval/embedding_models/e5_model.py`

 * *Files identical despite different names*

### Comparing `chat_rag-0.1.69/chat_rag/inf_retrieval/query_generator.py` & `chat_rag-0.1.70/chat_rag/inf_retrieval/query_generator.py`

 * *Files identical despite different names*

### Comparing `chat_rag-0.1.69/chat_rag/inf_retrieval/reference_checker.py` & `chat_rag-0.1.70/chat_rag/inf_retrieval/reference_checker.py`

 * *Files identical despite different names*

### Comparing `chat_rag-0.1.69/chat_rag/inf_retrieval/retrievers/colbert_retriever.py` & `chat_rag-0.1.70/chat_rag/inf_retrieval/retrievers/colbert_retriever.py`

 * *Files identical despite different names*

### Comparing `chat_rag-0.1.69/chat_rag/inf_retrieval/retrievers/rerank_retriever.py` & `chat_rag-0.1.70/chat_rag/inf_retrieval/retrievers/rerank_retriever.py`

 * *Files identical despite different names*

### Comparing `chat_rag-0.1.69/chat_rag/inf_retrieval/retrievers/semantic_retriever.py` & `chat_rag-0.1.70/chat_rag/inf_retrieval/retrievers/semantic_retriever.py`

 * *Files identical despite different names*

### Comparing `chat_rag-0.1.69/chat_rag/intent_detection/clusterize_text.py` & `chat_rag-0.1.70/chat_rag/intent_detection/clusterize_text.py`

 * *Files identical despite different names*

### Comparing `chat_rag-0.1.69/chat_rag/intent_detection/gen_intent.py` & `chat_rag-0.1.70/chat_rag/intent_detection/gen_intent.py`

 * *Files identical despite different names*

### Comparing `chat_rag-0.1.69/chat_rag/llms/base_llm.py` & `chat_rag-0.1.70/chat_rag/llms/base_llm.py`

 * *Files identical despite different names*

### Comparing `chat_rag-0.1.69/chat_rag/llms/claude_client.py` & `chat_rag-0.1.70/chat_rag/llms/claude_client.py`

 * *Files identical despite different names*

### Comparing `chat_rag-0.1.69/chat_rag/llms/ggml_llm.py` & `chat_rag-0.1.70/chat_rag/llms/ggml_llm.py`

 * *Files identical despite different names*

### Comparing `chat_rag-0.1.69/chat_rag/llms/hf_llm.py` & `chat_rag-0.1.70/chat_rag/llms/hf_llm.py`

 * *Files identical despite different names*

### Comparing `chat_rag-0.1.69/chat_rag/llms/mistral_client.py` & `chat_rag-0.1.70/chat_rag/llms/mistral_client.py`

 * *Files identical despite different names*

### Comparing `chat_rag-0.1.69/chat_rag/llms/openai_client.py` & `chat_rag-0.1.70/chat_rag/llms/openai_client.py`

 * *Files identical despite different names*

### Comparing `chat_rag-0.1.69/chat_rag/llms/vllm_client.py` & `chat_rag-0.1.70/chat_rag/llms/vllm_client.py`

 * *Files identical despite different names*

### Comparing `chat_rag-0.1.69/chat_rag/rag.py` & `chat_rag-0.1.70/chat_rag/rag.py`

 * *Files identical despite different names*

### Comparing `chat_rag-0.1.69/pyproject.toml` & `chat_rag-0.1.70/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "chat-rag"
-version = "0.1.69"
+version = "0.1.70"
 description = ""
 authors = ["Diego Peláez Paquico <diego.pelaez@with-madrid.com>"]
 readme = "README.md"
 packages = [{ include = "chat_rag" }]
 
 [tool.poetry.dependencies]
 python = "^3.10"
@@ -14,24 +14,24 @@
 tqdm = "^4.65.0"
 pyarrow = "^12.0.0"
 pillow = "^10.1.0"
 certifi = "^2023.7.22"
 urllib3 = "^1.26.18"
 aiohttp = "^3.8.5"
 cryptography = "^41.0.4"
-torch = "2.2.2"
+torch = "2.3.0"
 transformers = "^4.38.2"
 sentence-transformers = "^2.3.0"
 ctransformers = "^0.2.10"
 einops = "^0.6.1"
 accelerate = "^0.21.0"
 autoawq = "0.1.7"
 unstructured = {extras = ["pdf"], version = "0.12.0", python = ">=3.10,<3.12"}
 unstructured-inference = "0.7.21"
-torchvision = "0.17.2"
+torchvision = "0.18.0"
 openai = "^1.3.4"
 anthropic = "0.18.1"
 mistralai = "0.0.9"
 protobuf = "3.20.2"
 ragatouille = "^0.0.8.post2"
 
 [build-system]
```

### Comparing `chat_rag-0.1.69/PKG-INFO` & `chat_rag-0.1.70/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: chat-rag
-Version: 0.1.69
+Version: 0.1.70
 Summary: 
 Author: Diego Peláez Paquico
 Author-email: diego.pelaez@with-madrid.com
 Requires-Python: >=3.10,<4.0
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
@@ -23,16 +23,16 @@
 Requires-Dist: pandas (==1.4.4)
 Requires-Dist: pillow (>=10.1.0,<11.0.0)
 Requires-Dist: protobuf (==3.20.2)
 Requires-Dist: pyarrow (>=12.0.0,<13.0.0)
 Requires-Dist: python-dotenv (>=0.21.0,<0.22.0)
 Requires-Dist: ragatouille (>=0.0.8.post2,<0.0.9)
 Requires-Dist: sentence-transformers (>=2.3.0,<3.0.0)
-Requires-Dist: torch (==2.2.2)
-Requires-Dist: torchvision (==0.17.2)
+Requires-Dist: torch (==2.3.0)
+Requires-Dist: torchvision (==0.18.0)
 Requires-Dist: tqdm (>=4.65.0,<5.0.0)
 Requires-Dist: transformers (>=4.38.2,<5.0.0)
 Requires-Dist: unstructured-inference (==0.7.21)
 Requires-Dist: unstructured[pdf] (==0.12.0) ; python_version >= "3.10" and python_version < "3.12"
 Requires-Dist: urllib3 (>=1.26.18,<2.0.0)
 Description-Content-Type: text/markdown
```

