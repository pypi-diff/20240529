# Comparing `tmp/chat_rag-0.1.68.tar.gz` & `tmp/chat_rag-0.1.69.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "chat_rag-0.1.68.tar", max compression
+gzip compressed data, was "chat_rag-0.1.69.tar", max compression
```

## Comparing `chat_rag-0.1.68.tar` & `chat_rag-0.1.69.tar`

### file list

```diff
@@ -1,35 +1,36 @@
--rw-r--r--   0        0        0     1083 2024-02-07 11:08:45.534329 chat_rag-0.1.68/LICENSE
--rw-r--r--   0        0        0     1666 2024-02-07 11:08:45.534329 chat_rag-0.1.68/README.md
--rw-r--r--   0        0        0       68 2024-04-16 07:55:27.403398 chat_rag-0.1.68/chat_rag/__init__.py
--rw-r--r--   0        0        0     3295 2024-04-16 07:55:27.407398 chat_rag-0.1.68/chat_rag/async_rag.py
--rw-r--r--   0        0        0        0 2024-02-07 11:08:45.534329 chat_rag-0.1.68/chat_rag/data/__init__.py
--rw-r--r--   0        0        0      788 2024-02-07 11:08:45.534329 chat_rag-0.1.68/chat_rag/data/models.py
--rw-r--r--   0        0        0    10492 2024-04-16 07:55:27.407398 chat_rag-0.1.68/chat_rag/data/parsers.py
--rw-r--r--   0        0        0    13027 2024-03-06 16:38:44.353919 chat_rag-0.1.68/chat_rag/data/splitters.py
--rw-r--r--   0        0        0      897 2024-02-26 10:37:33.379027 chat_rag-0.1.68/chat_rag/exceptions.py
--rw-r--r--   0        0        0        0 2024-02-07 11:08:45.534329 chat_rag-0.1.68/chat_rag/inf_retrieval/__init__.py
--rw-r--r--   0        0        0     3924 2024-02-07 11:08:45.534329 chat_rag-0.1.68/chat_rag/inf_retrieval/check_answ_questions.py
--rw-r--r--   0        0        0     2450 2024-02-07 11:08:45.534329 chat_rag-0.1.68/chat_rag/inf_retrieval/cross_encoder.py
--rw-r--r--   0        0        0      141 2024-02-07 11:08:45.534329 chat_rag-0.1.68/chat_rag/inf_retrieval/embedding_models/__init__.py
--rw-r--r--   0        0        0     4617 2024-02-07 11:08:45.534329 chat_rag-0.1.68/chat_rag/inf_retrieval/embedding_models/base_model.py
--rw-r--r--   0        0        0     1494 2024-04-18 10:45:56.532544 chat_rag-0.1.68/chat_rag/inf_retrieval/embedding_models/e5_model.py
--rw-r--r--   0        0        0     4693 2024-02-07 11:08:45.534329 chat_rag-0.1.68/chat_rag/inf_retrieval/query_generator.py
--rw-r--r--   0        0        0     3886 2024-02-07 11:08:45.534329 chat_rag-0.1.68/chat_rag/inf_retrieval/reference_checker.py
--rw-r--r--   0        0        0      240 2024-04-16 07:55:27.407398 chat_rag-0.1.68/chat_rag/inf_retrieval/retrievers/__init__.py
--rw-r--r--   0        0        0      856 2024-04-16 07:55:27.407398 chat_rag-0.1.68/chat_rag/inf_retrieval/retrievers/rerank_retriever.py
--rw-r--r--   0        0        0      503 2024-04-16 07:55:27.407398 chat_rag-0.1.68/chat_rag/inf_retrieval/retrievers/retriever_client.py
--rw-r--r--   0        0        0     7447 2024-02-07 11:08:45.534329 chat_rag-0.1.68/chat_rag/inf_retrieval/retrievers/semantic_retriever.py
--rw-r--r--   0        0        0      135 2024-02-07 11:08:45.534329 chat_rag-0.1.68/chat_rag/intent_detection/__init__.py
--rw-r--r--   0        0        0     1527 2024-02-07 11:08:45.534329 chat_rag-0.1.68/chat_rag/intent_detection/clusterize_text.py
--rw-r--r--   0        0        0     1419 2024-02-07 11:08:45.534329 chat_rag-0.1.68/chat_rag/intent_detection/gen_intent.py
--rw-r--r--   0        0        0      445 2024-04-16 07:55:27.407398 chat_rag-0.1.68/chat_rag/llms/__init__.py
--rw-r--r--   0        0        0     6995 2024-02-26 10:37:33.379027 chat_rag-0.1.68/chat_rag/llms/base_llm.py
--rw-r--r--   0        0        0     9040 2024-04-16 07:55:27.407398 chat_rag-0.1.68/chat_rag/llms/claude_client.py
--rw-r--r--   0        0        0     5219 2024-02-07 11:08:45.534329 chat_rag-0.1.68/chat_rag/llms/ggml_llm.py
--rw-r--r--   0        0        0     9255 2024-02-07 11:08:45.534329 chat_rag-0.1.68/chat_rag/llms/hf_llm.py
--rw-r--r--   0        0        0    10715 2024-04-16 07:55:27.407398 chat_rag-0.1.68/chat_rag/llms/mistral_client.py
--rw-r--r--   0        0        0    11021 2024-04-23 09:13:44.604113 chat_rag-0.1.68/chat_rag/llms/openai_client.py
--rw-r--r--   0        0        0    25992 2024-04-16 07:55:27.407398 chat_rag-0.1.68/chat_rag/llms/vllm_client.py
--rw-r--r--   0        0        0     3578 2024-04-16 07:55:27.407398 chat_rag-0.1.68/chat_rag/rag.py
--rw-r--r--   0        0        0      930 2024-04-23 09:54:54.694245 chat_rag-0.1.68/pyproject.toml
--rw-r--r--   0        0        0     3159 1970-01-01 00:00:00.000000 chat_rag-0.1.68/PKG-INFO
+-rw-r--r--   0        0        0     1083 2024-02-07 11:08:45.534329 chat_rag-0.1.69/LICENSE
+-rw-r--r--   0        0        0     1666 2024-02-07 11:08:45.534329 chat_rag-0.1.69/README.md
+-rw-r--r--   0        0        0       68 2024-04-25 12:19:16.531849 chat_rag-0.1.69/chat_rag/__init__.py
+-rw-r--r--   0        0        0     3448 2024-04-27 16:28:16.074506 chat_rag-0.1.69/chat_rag/async_rag.py
+-rw-r--r--   0        0        0        0 2024-02-07 11:08:45.534329 chat_rag-0.1.69/chat_rag/data/__init__.py
+-rw-r--r--   0        0        0      788 2024-02-07 11:08:45.534329 chat_rag-0.1.69/chat_rag/data/models.py
+-rw-r--r--   0        0        0    10492 2024-04-25 12:19:16.531849 chat_rag-0.1.69/chat_rag/data/parsers.py
+-rw-r--r--   0        0        0    13027 2024-03-06 16:38:44.353919 chat_rag-0.1.69/chat_rag/data/splitters.py
+-rw-r--r--   0        0        0      897 2024-02-26 10:37:33.379027 chat_rag-0.1.69/chat_rag/exceptions.py
+-rw-r--r--   0        0        0        0 2024-02-07 11:08:45.534329 chat_rag-0.1.69/chat_rag/inf_retrieval/__init__.py
+-rw-r--r--   0        0        0     3924 2024-02-07 11:08:45.534329 chat_rag-0.1.69/chat_rag/inf_retrieval/check_answ_questions.py
+-rw-r--r--   0        0        0     2450 2024-02-07 11:08:45.534329 chat_rag-0.1.69/chat_rag/inf_retrieval/cross_encoder.py
+-rw-r--r--   0        0        0      141 2024-02-07 11:08:45.534329 chat_rag-0.1.69/chat_rag/inf_retrieval/embedding_models/__init__.py
+-rw-r--r--   0        0        0     4617 2024-02-07 11:08:45.534329 chat_rag-0.1.69/chat_rag/inf_retrieval/embedding_models/base_model.py
+-rw-r--r--   0        0        0     1494 2024-04-18 10:45:56.532544 chat_rag-0.1.69/chat_rag/inf_retrieval/embedding_models/e5_model.py
+-rw-r--r--   0        0        0     4693 2024-02-07 11:08:45.534329 chat_rag-0.1.69/chat_rag/inf_retrieval/query_generator.py
+-rw-r--r--   0        0        0     3918 2024-05-29 15:03:20.869731 chat_rag-0.1.69/chat_rag/inf_retrieval/reference_checker.py
+-rw-r--r--   0        0        0      240 2024-04-25 12:19:16.531849 chat_rag-0.1.69/chat_rag/inf_retrieval/retrievers/__init__.py
+-rw-r--r--   0        0        0     6913 2024-05-29 15:41:37.734475 chat_rag-0.1.69/chat_rag/inf_retrieval/retrievers/colbert_retriever.py
+-rw-r--r--   0        0        0      856 2024-04-25 12:19:16.531849 chat_rag-0.1.69/chat_rag/inf_retrieval/retrievers/rerank_retriever.py
+-rw-r--r--   0        0        0      503 2024-04-25 12:19:16.535849 chat_rag-0.1.69/chat_rag/inf_retrieval/retrievers/retriever_client.py
+-rw-r--r--   0        0        0     7447 2024-02-07 11:08:45.534329 chat_rag-0.1.69/chat_rag/inf_retrieval/retrievers/semantic_retriever.py
+-rw-r--r--   0        0        0      135 2024-02-07 11:08:45.534329 chat_rag-0.1.69/chat_rag/intent_detection/__init__.py
+-rw-r--r--   0        0        0     1527 2024-02-07 11:08:45.534329 chat_rag-0.1.69/chat_rag/intent_detection/clusterize_text.py
+-rw-r--r--   0        0        0     1419 2024-02-07 11:08:45.534329 chat_rag-0.1.69/chat_rag/intent_detection/gen_intent.py
+-rw-r--r--   0        0        0      445 2024-04-25 12:19:16.535849 chat_rag-0.1.69/chat_rag/llms/__init__.py
+-rw-r--r--   0        0        0     6995 2024-02-26 10:37:33.379027 chat_rag-0.1.69/chat_rag/llms/base_llm.py
+-rw-r--r--   0        0        0     9040 2024-04-25 12:19:16.535849 chat_rag-0.1.69/chat_rag/llms/claude_client.py
+-rw-r--r--   0        0        0     5219 2024-02-07 11:08:45.534329 chat_rag-0.1.69/chat_rag/llms/ggml_llm.py
+-rw-r--r--   0        0        0     9255 2024-02-07 11:08:45.534329 chat_rag-0.1.69/chat_rag/llms/hf_llm.py
+-rw-r--r--   0        0        0    10715 2024-04-25 12:19:16.535849 chat_rag-0.1.69/chat_rag/llms/mistral_client.py
+-rw-r--r--   0        0        0    11021 2024-04-27 16:28:16.074506 chat_rag-0.1.69/chat_rag/llms/openai_client.py
+-rw-r--r--   0        0        0    25992 2024-04-25 12:19:16.535849 chat_rag-0.1.69/chat_rag/llms/vllm_client.py
+-rw-r--r--   0        0        0     3578 2024-04-25 12:19:16.535849 chat_rag-0.1.69/chat_rag/rag.py
+-rw-r--r--   0        0        0      930 2024-05-29 15:44:09.914414 chat_rag-0.1.69/pyproject.toml
+-rw-r--r--   0        0        0     3159 1970-01-01 00:00:00.000000 chat_rag-0.1.69/PKG-INFO
```

### Comparing `chat_rag-0.1.68/LICENSE` & `chat_rag-0.1.69/LICENSE`

 * *Files identical despite different names*

### Comparing `chat_rag-0.1.68/README.md` & `chat_rag-0.1.69/README.md`

 * *Files identical despite different names*

### Comparing `chat_rag-0.1.68/chat_rag/async_rag.py` & `chat_rag-0.1.69/chat_rag/async_rag.py`

 * *Files 11% similar despite different names*

```diff
@@ -41,15 +41,15 @@
             Dictionary containing the structure of the prompt.
 
         Returns
         -------
         Tuple[List[str], List[Dict[str, str]]]
             List of all conversation contexts and list of the retrieved contexts for the current user message.
         """
-        logger.info("Retrieving new contexts")
+        logger.info(f"Retrieving contexts for message: {message}")
         contexts = await self.retriever.retrieve(
             message,
             top_k=prompt_structure_dict["n_contexts_to_use"]
         )
 
         if not contexts:
             return [], []
@@ -58,17 +58,20 @@
         returned_contexts = [contexts[:prompt_structure_dict["n_contexts_to_use"]]]  # structure for references
 
         # Use a list comprehension to preserve order and not adding duplicates
         seen = set()
         contents = [x for x in prev_contents + contents if not (x in seen or seen.add(x))]
         return contents, returned_contexts
 
-    async def stream(self, messages: List[Dict[str, str]], prev_contents: List[str], prompt_structure_dict: dict, generation_config_dict: dict, stop_words: List[str] = None):
+    async def stream(self, messages: List[Dict[str, str]], prev_contents: List[str], prompt_structure_dict: dict, generation_config_dict: dict, stop_words: List[str] = None, only_context: bool = False):
         # Retrieve
         contents, returned_contexts = await self.retrieve(messages[-1]['content'], prev_contents, prompt_structure_dict)
+        if only_context:
+            yield {"res": "", "context": returned_contexts}
+            return
 
         # Generate
         async for new_text in self.model.stream(
             messages, contents, prompt_structure_dict=prompt_structure_dict,
             generation_config_dict=generation_config_dict, lang=self.lang, stop_words=stop_words
         ):
             yield {"res": new_text, "context": returned_contexts}
@@ -77,8 +80,8 @@
         # Retrieve
         contents, returned_contexts = await self.retrieve(messages[-1]['content'], prev_contents, prompt_structure_dict)
 
         output_text = await self.model.generate(
             messages, contents, prompt_structure_dict=prompt_structure_dict,
             generation_config_dict=generation_config_dict, lang=self.lang, stop_words=stop_words
         )
-        return {"res": output_text, "context": returned_contexts}
+        return {"res": output_text, "context": returned_contexts}
```

### Comparing `chat_rag-0.1.68/chat_rag/data/models.py` & `chat_rag-0.1.69/chat_rag/data/models.py`

 * *Files identical despite different names*

### Comparing `chat_rag-0.1.68/chat_rag/data/parsers.py` & `chat_rag-0.1.69/chat_rag/data/parsers.py`

 * *Files identical despite different names*

### Comparing `chat_rag-0.1.68/chat_rag/data/splitters.py` & `chat_rag-0.1.69/chat_rag/data/splitters.py`

 * *Files identical despite different names*

### Comparing `chat_rag-0.1.68/chat_rag/exceptions.py` & `chat_rag-0.1.69/chat_rag/exceptions.py`

 * *Files identical despite different names*

### Comparing `chat_rag-0.1.68/chat_rag/inf_retrieval/check_answ_questions.py` & `chat_rag-0.1.69/chat_rag/inf_retrieval/check_answ_questions.py`

 * *Files identical despite different names*

### Comparing `chat_rag-0.1.68/chat_rag/inf_retrieval/cross_encoder.py` & `chat_rag-0.1.69/chat_rag/inf_retrieval/cross_encoder.py`

 * *Files identical despite different names*

### Comparing `chat_rag-0.1.68/chat_rag/inf_retrieval/embedding_models/base_model.py` & `chat_rag-0.1.69/chat_rag/inf_retrieval/embedding_models/base_model.py`

 * *Files identical despite different names*

### Comparing `chat_rag-0.1.68/chat_rag/inf_retrieval/embedding_models/e5_model.py` & `chat_rag-0.1.69/chat_rag/inf_retrieval/embedding_models/e5_model.py`

 * *Files identical despite different names*

### Comparing `chat_rag-0.1.68/chat_rag/inf_retrieval/query_generator.py` & `chat_rag-0.1.69/chat_rag/inf_retrieval/query_generator.py`

 * *Files identical despite different names*

### Comparing `chat_rag-0.1.68/chat_rag/inf_retrieval/reference_checker.py` & `chat_rag-0.1.69/chat_rag/inf_retrieval/reference_checker.py`

 * *Files 4% similar despite different names*

```diff
@@ -42,15 +42,15 @@
         for true_label in self.true_labels:
             if (highest_score - output['scores'][output['labels'].index(true_label)]) < 0.1:
                 return True
 
         return False # if not question or instruction, then don't retrieve
     
 
-def clean_relevant_references(sources: List[Dict[str, Any]], min_difference=0.09, min_score=0.3) -> List[Dict[str, Any]]:
+def clean_relevant_references(sources: List[Dict[str, Any]], min_difference=0.09, min_score=0.3, score_key: str = 'score') -> List[Dict[str, Any]]:
     """
     Find the relevant sources from a list of sources. We use the similarity scores to find the relevant sources. We calculate the standard deviation of the gaps between consecutive sources and return all sources up to the first significant gap.
     Parameters
     ----------
     sources: List[Dict[str, Any]]
         List of sources to find the relevant sources from.
     min_difference: float
@@ -61,15 +61,15 @@
     -------
     List[Dict[str, Any]]
         List of relevant sources.
     """
 
     # Calculate gaps between consecutive sources
     # print the similarity scores
-    gaps = [sources[i]['score'] - sources[i + 1]['score'] for i in range(len(sources) - 1)]
+    gaps = [sources[i][score_key] - sources[i + 1][score_key] for i in range(len(sources) - 1)]
 
     # Compute standard deviation of the gaps if there are enough gaps
     if len(gaps) > 1:
         std_dev = np.std(gaps)
     else:
         # If there's only one gap or none, return all sources as relevant
         return sources
@@ -77,12 +77,12 @@
     # Identify the first significant gap
     for i, gap in enumerate(gaps):
         if gap > std_dev and gap > min_difference:  # A significant gap
             return sources[:i + 1]
         
     final_sources = []
     for source in sources:
-        if source['score'] > min_score:
+        if source[score_key] > min_score:
             final_sources.append(source)
 
     # If no significant gap found, return all sources
     return final_sources
```

### Comparing `chat_rag-0.1.68/chat_rag/inf_retrieval/retrievers/rerank_retriever.py` & `chat_rag-0.1.69/chat_rag/inf_retrieval/retrievers/rerank_retriever.py`

 * *Files identical despite different names*

### Comparing `chat_rag-0.1.68/chat_rag/inf_retrieval/retrievers/semantic_retriever.py` & `chat_rag-0.1.69/chat_rag/inf_retrieval/retrievers/semantic_retriever.py`

 * *Files identical despite different names*

### Comparing `chat_rag-0.1.68/chat_rag/intent_detection/clusterize_text.py` & `chat_rag-0.1.69/chat_rag/intent_detection/clusterize_text.py`

 * *Files identical despite different names*

### Comparing `chat_rag-0.1.68/chat_rag/intent_detection/gen_intent.py` & `chat_rag-0.1.69/chat_rag/intent_detection/gen_intent.py`

 * *Files identical despite different names*

### Comparing `chat_rag-0.1.68/chat_rag/llms/base_llm.py` & `chat_rag-0.1.69/chat_rag/llms/base_llm.py`

 * *Files identical despite different names*

### Comparing `chat_rag-0.1.68/chat_rag/llms/claude_client.py` & `chat_rag-0.1.69/chat_rag/llms/claude_client.py`

 * *Files identical despite different names*

### Comparing `chat_rag-0.1.68/chat_rag/llms/ggml_llm.py` & `chat_rag-0.1.69/chat_rag/llms/ggml_llm.py`

 * *Files identical despite different names*

### Comparing `chat_rag-0.1.68/chat_rag/llms/hf_llm.py` & `chat_rag-0.1.69/chat_rag/llms/hf_llm.py`

 * *Files identical despite different names*

### Comparing `chat_rag-0.1.68/chat_rag/llms/mistral_client.py` & `chat_rag-0.1.69/chat_rag/llms/mistral_client.py`

 * *Files identical despite different names*

### Comparing `chat_rag-0.1.68/chat_rag/llms/openai_client.py` & `chat_rag-0.1.69/chat_rag/llms/openai_client.py`

 * *Files identical despite different names*

### Comparing `chat_rag-0.1.68/chat_rag/llms/vllm_client.py` & `chat_rag-0.1.69/chat_rag/llms/vllm_client.py`

 * *Files identical despite different names*

### Comparing `chat_rag-0.1.68/chat_rag/rag.py` & `chat_rag-0.1.69/chat_rag/rag.py`

 * *Files identical despite different names*

### Comparing `chat_rag-0.1.68/pyproject.toml` & `chat_rag-0.1.69/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "chat-rag"
-version = "0.1.68"
+version = "0.1.69"
 description = ""
 authors = ["Diego Peláez Paquico <diego.pelaez@with-madrid.com>"]
 readme = "README.md"
 packages = [{ include = "chat_rag" }]
 
 [tool.poetry.dependencies]
 python = "^3.10"
```

### Comparing `chat_rag-0.1.68/PKG-INFO` & `chat_rag-0.1.69/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: chat-rag
-Version: 0.1.68
+Version: 0.1.69
 Summary: 
 Author: Diego Peláez Paquico
 Author-email: diego.pelaez@with-madrid.com
 Requires-Python: >=3.10,<4.0
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
```

