# Comparing `tmp/voyageai-0.2.2.tar.gz` & `tmp/voyageai-0.2.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "voyageai-0.2.2.tar", max compression
+gzip compressed data, was "voyageai-0.2.3.tar", max compression
```

## Comparing `voyageai-0.2.2.tar` & `voyageai-0.2.3.tar`

### file list

```diff
@@ -1,20 +1,20 @@
--rw-r--r--   0        0        0     1140 2023-10-20 18:34:31.000000 voyageai-0.2.2/LICENSE
--rw-r--r--   0        0        0     1960 2024-04-08 00:09:37.066315 voyageai-0.2.2/README.md
--rw-r--r--   0        0        0      446 2024-03-28 19:25:44.652139 voyageai-0.2.2/pyproject.toml
--rw-r--r--   0        0        0     1635 2024-04-05 01:01:51.506241 voyageai-0.2.2/voyageai/__init__.py
--rw-r--r--   0        0        0      298 2024-03-02 01:20:18.478801 voyageai-0.2.2/voyageai/api_resources/__init__.py
--rw-r--r--   0        0        0    17505 2024-04-05 01:03:25.382598 voyageai-0.2.2/voyageai/api_resources/api_requestor.py
--rw-r--r--   0        0        0     2203 2024-04-05 01:01:51.516327 voyageai-0.2.2/voyageai/api_resources/api_resource.py
--rw-r--r--   0        0        0     2157 2024-03-27 23:59:57.198284 voyageai-0.2.2/voyageai/api_resources/embedding.py
--rw-r--r--   0        0        0      573 2024-04-05 01:01:51.503202 voyageai-0.2.2/voyageai/api_resources/reranking.py
--rw-r--r--   0        0        0     5561 2024-04-05 01:03:39.591029 voyageai-0.2.2/voyageai/api_resources/response.py
--rw-r--r--   0        0        0     3785 2024-04-05 01:01:51.518833 voyageai-0.2.2/voyageai/client.py
--rw-r--r--   0        0        0     3117 2024-04-05 01:01:51.515009 voyageai-0.2.2/voyageai/client_async.py
--rw-r--r--   0        0        0     6529 2024-04-05 01:02:44.889774 voyageai-0.2.2/voyageai/embeddings_utils.py
--rw-r--r--   0        0        0     2490 2024-04-05 01:01:51.517715 voyageai-0.2.2/voyageai/error.py
--rw-r--r--   0        0        0      110 2024-04-05 01:01:51.505333 voyageai-0.2.2/voyageai/object/__init__.py
--rw-r--r--   0        0        0      502 2024-04-05 01:01:51.509038 voyageai-0.2.2/voyageai/object/embeddings.py
--rw-r--r--   0        0        0      639 2024-04-05 01:01:51.511331 voyageai-0.2.2/voyageai/object/reranking.py
--rw-r--r--   0        0        0     2585 2024-04-05 01:01:51.520920 voyageai-0.2.2/voyageai/util.py
--rw-r--r--   0        0        0       18 2024-03-28 19:25:35.659378 voyageai-0.2.2/voyageai/version.py
--rw-r--r--   0        0        0     2631 1970-01-01 00:00:00.000000 voyageai-0.2.2/PKG-INFO
+-rw-r--r--   0        0        0     1140 2023-10-20 18:34:31.000000 voyageai-0.2.3/LICENSE
+-rw-r--r--   0        0        0     1974 2024-05-29 00:30:43.074967 voyageai-0.2.3/README.md
+-rw-r--r--   0        0        0      446 2024-05-22 01:04:38.546821 voyageai-0.2.3/pyproject.toml
+-rw-r--r--   0        0        0     1635 2024-04-05 01:01:51.506241 voyageai-0.2.3/voyageai/__init__.py
+-rw-r--r--   0        0        0      298 2024-03-02 01:20:18.478801 voyageai-0.2.3/voyageai/api_resources/__init__.py
+-rw-r--r--   0        0        0    17505 2024-04-05 01:03:25.382598 voyageai-0.2.3/voyageai/api_resources/api_requestor.py
+-rw-r--r--   0        0        0     2203 2024-04-05 01:01:51.516327 voyageai-0.2.3/voyageai/api_resources/api_resource.py
+-rw-r--r--   0        0        0     2157 2024-03-27 23:59:57.198284 voyageai-0.2.3/voyageai/api_resources/embedding.py
+-rw-r--r--   0        0        0      573 2024-04-05 01:01:51.503202 voyageai-0.2.3/voyageai/api_resources/reranking.py
+-rw-r--r--   0        0        0     5561 2024-04-05 01:03:39.591029 voyageai-0.2.3/voyageai/api_resources/response.py
+-rw-r--r--   0        0        0     4586 2024-05-22 00:26:26.400907 voyageai-0.2.3/voyageai/client.py
+-rw-r--r--   0        0        0     3117 2024-04-05 01:01:51.515009 voyageai-0.2.3/voyageai/client_async.py
+-rw-r--r--   0        0        0     6529 2024-04-05 01:02:44.889774 voyageai-0.2.3/voyageai/embeddings_utils.py
+-rw-r--r--   0        0        0     2490 2024-04-05 01:01:51.517715 voyageai-0.2.3/voyageai/error.py
+-rw-r--r--   0        0        0      110 2024-04-05 01:01:51.505333 voyageai-0.2.3/voyageai/object/__init__.py
+-rw-r--r--   0        0        0      502 2024-04-05 01:01:51.509038 voyageai-0.2.3/voyageai/object/embeddings.py
+-rw-r--r--   0        0        0      639 2024-04-05 01:01:51.511331 voyageai-0.2.3/voyageai/object/reranking.py
+-rw-r--r--   0        0        0     2585 2024-04-05 01:01:51.520920 voyageai-0.2.3/voyageai/util.py
+-rw-r--r--   0        0        0       18 2024-05-22 01:04:30.384617 voyageai-0.2.3/voyageai/version.py
+-rw-r--r--   0        0        0     2645 1970-01-01 00:00:00.000000 voyageai-0.2.3/PKG-INFO
```

### Comparing `voyageai-0.2.2/LICENSE` & `voyageai-0.2.3/LICENSE`

 * *Files identical despite different names*

### Comparing `voyageai-0.2.2/README.md` & `voyageai-0.2.3/README.md`

 * *Files 3% similar despite different names*

```diff
@@ -4,10 +4,10 @@
 
 Embedding models are neural net models (e.g., transformers) that convert unstructured and complex data, such as documents, images, audios, videos, or tabular data, into dense numerical vectors (i.e. embeddings) that capture their semantic meanings. These vectors serve as representations/indices for datapoints and are essential building blocks for semantic search and retrieval-augmented generation (RAG), which is the predominant approach for domain-specific or company-specific chatbots and other AI applications.
 
 Rerankers are neural nets that output relevance scores between a query and multiple documents. It is common practice to use the relevance scores to rerank the documents initially retrieved with embedding-based methods (or with lexical search algorithms such as BM25 and TF-IDF). Selecting the highest-scored documents refines the retrieval results into a more relevant subset.
 
 Voyage AI provides API endpoints for embedding and reranking models that take in your data (e.g., documents, queries, or query-document pairs) and return their embeddings or relevance scores. Embedding models and rerankers, as modular components, seamlessly integrate with other parts of a RAG stack, including vector stores and generative Large Language Models (LLMs).
 
-Voyage AI’s embedding models and rerankers are **state-of-the-art** in retrieval accuracy. Please read our announcing [blog post](https://blog.voyageai.com/2023/10/29/voyage-embeddings/) for details.  Please also check out a high-level [introduction](https://www.pinecone.io/learn/retrieval-augmented-generation/) of embedding models, semantic search, and RAG, and our step-by-step [quickstart tutorial](https://docs.voyageai.com/tutorials/) on implementing a minimalist RAG chatbot using Voyage model endpoints.
+Voyage AI’s embedding models and rerankers are **state-of-the-art** in retrieval accuracy. Please read our announcing [blog post](https://blog.voyageai.com/2023/10/29/voyage-embeddings/) for details.  Please also check out a high-level [introduction](https://www.pinecone.io/learn/retrieval-augmented-generation/) of embedding models, semantic search, and RAG, and our step-by-step [quickstart tutorial](https://docs.voyageai.com/docs/quickstart-tutorial) on implementing a minimalist RAG chatbot using Voyage model endpoints.
 
 ### [Voyage AI Official Documentation](https://docs.voyageai.com)
```

### Comparing `voyageai-0.2.2/voyageai/__init__.py` & `voyageai-0.2.3/voyageai/__init__.py`

 * *Files identical despite different names*

### Comparing `voyageai-0.2.2/voyageai/api_resources/api_requestor.py` & `voyageai-0.2.3/voyageai/api_resources/api_requestor.py`

 * *Files identical despite different names*

### Comparing `voyageai-0.2.2/voyageai/api_resources/api_resource.py` & `voyageai-0.2.3/voyageai/api_resources/api_resource.py`

 * *Files identical despite different names*

### Comparing `voyageai-0.2.2/voyageai/api_resources/embedding.py` & `voyageai-0.2.3/voyageai/api_resources/embedding.py`

 * *Files identical despite different names*

### Comparing `voyageai-0.2.2/voyageai/api_resources/reranking.py` & `voyageai-0.2.3/voyageai/api_resources/reranking.py`

 * *Files identical despite different names*

### Comparing `voyageai-0.2.2/voyageai/api_resources/response.py` & `voyageai-0.2.3/voyageai/api_resources/response.py`

 * *Files identical despite different names*

### Comparing `voyageai-0.2.2/voyageai/client.py` & `voyageai-0.2.3/voyageai/client.py`

 * *Files 14% similar despite different names*

```diff
@@ -97,34 +97,52 @@
                     truncation=truncation,
                     **self._params,
                 )
 
         result = RerankingObject(documents, response)
         return result
 
-    @property
     @functools.lru_cache()
-    def tokenizer(self):
+    def tokenizer(self, model: str):
         try:
             from tokenizers import Tokenizer
         except ImportError:
             raise ImportError(
-                "tokenizers package not found. Please run `pip install tokenizers` "
+                "The package `tokenizers` is not found. Please run `pip install tokenizers` "
                 "to install the dependency."
             )
 
-        tokenizer = Tokenizer.from_pretrained("voyageai/voyage")
-        tokenizer.no_truncation()
+        try:
+            tokenizer = Tokenizer.from_pretrained(f"voyageai/{model}")
+            tokenizer.no_truncation()
+        except:
+            warnings.warn(
+                f"Failed to load the tokenizer for `{model}`. Please ensure that it is a valid model name."
+            )
+            raise
+        
         return tokenizer
 
     def tokenize(
         self,
         texts: List[str],
+        model: Optional[str] = None,
     ) -> List[Any]:
-        return self.tokenizer.encode_batch(texts)
+
+        if model is None:
+            warnings.warn(
+                "Please specify the `model` when using the tokenizer. Voyage's older models use the same "
+                "tokenizer, but new models may use different tokenizers. If `model` is not specified, "
+                "the old tokenizer will be used and the results might be different. `model` will be a "
+                "required argument in the future."
+            )
+            model = voyageai.VOYAGE_EMBED_DEFAULT_MODEL
+
+        return self.tokenizer(model).encode_batch(texts)
 
     def count_tokens(
         self,
         texts: List[str],
+        model: Optional[str] = None,
     ) -> int:
-        tokenized = self.tokenize(texts)
+        tokenized = self.tokenize(texts, model)
         return sum([len(t) for t in tokenized])
```

### Comparing `voyageai-0.2.2/voyageai/client_async.py` & `voyageai-0.2.3/voyageai/client_async.py`

 * *Files identical despite different names*

### Comparing `voyageai-0.2.2/voyageai/embeddings_utils.py` & `voyageai-0.2.3/voyageai/embeddings_utils.py`

 * *Files identical despite different names*

### Comparing `voyageai-0.2.2/voyageai/error.py` & `voyageai-0.2.3/voyageai/error.py`

 * *Files identical despite different names*

### Comparing `voyageai-0.2.2/voyageai/object/reranking.py` & `voyageai-0.2.3/voyageai/object/reranking.py`

 * *Files identical despite different names*

### Comparing `voyageai-0.2.2/voyageai/util.py` & `voyageai-0.2.3/voyageai/util.py`

 * *Files identical despite different names*

### Comparing `voyageai-0.2.2/PKG-INFO` & `voyageai-0.2.3/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: voyageai
-Version: 0.2.2
+Version: 0.2.3
 Summary: 
 Author: Yujie Qian
 Author-email: yujieq@voyageai.com
 Requires-Python: >=3.7.1,<4.0.0
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
@@ -24,11 +24,11 @@
 
 Embedding models are neural net models (e.g., transformers) that convert unstructured and complex data, such as documents, images, audios, videos, or tabular data, into dense numerical vectors (i.e. embeddings) that capture their semantic meanings. These vectors serve as representations/indices for datapoints and are essential building blocks for semantic search and retrieval-augmented generation (RAG), which is the predominant approach for domain-specific or company-specific chatbots and other AI applications.
 
 Rerankers are neural nets that output relevance scores between a query and multiple documents. It is common practice to use the relevance scores to rerank the documents initially retrieved with embedding-based methods (or with lexical search algorithms such as BM25 and TF-IDF). Selecting the highest-scored documents refines the retrieval results into a more relevant subset.
 
 Voyage AI provides API endpoints for embedding and reranking models that take in your data (e.g., documents, queries, or query-document pairs) and return their embeddings or relevance scores. Embedding models and rerankers, as modular components, seamlessly integrate with other parts of a RAG stack, including vector stores and generative Large Language Models (LLMs).
 
-Voyage AI’s embedding models and rerankers are **state-of-the-art** in retrieval accuracy. Please read our announcing [blog post](https://blog.voyageai.com/2023/10/29/voyage-embeddings/) for details.  Please also check out a high-level [introduction](https://www.pinecone.io/learn/retrieval-augmented-generation/) of embedding models, semantic search, and RAG, and our step-by-step [quickstart tutorial](https://docs.voyageai.com/tutorials/) on implementing a minimalist RAG chatbot using Voyage model endpoints.
+Voyage AI’s embedding models and rerankers are **state-of-the-art** in retrieval accuracy. Please read our announcing [blog post](https://blog.voyageai.com/2023/10/29/voyage-embeddings/) for details.  Please also check out a high-level [introduction](https://www.pinecone.io/learn/retrieval-augmented-generation/) of embedding models, semantic search, and RAG, and our step-by-step [quickstart tutorial](https://docs.voyageai.com/docs/quickstart-tutorial) on implementing a minimalist RAG chatbot using Voyage model endpoints.
 
 ### [Voyage AI Official Documentation](https://docs.voyageai.com)
```

