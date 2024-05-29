# Comparing `tmp/ragstack_ai_knowledge_store-0.0.1.tar.gz` & `tmp/ragstack_ai_knowledge_store-0.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ragstack_ai_knowledge_store-0.0.1.tar", max compression
+gzip compressed data, was "ragstack_ai_knowledge_store-0.0.2.tar", max compression
```

## Comparing `ragstack_ai_knowledge_store-0.0.1.tar` & `ragstack_ai_knowledge_store-0.0.2.tar`

### file list

```diff
@@ -1,8 +1,8 @@
--rw-r--r--   0        0        0      362 2024-05-22 19:47:21.341025 ragstack_ai_knowledge_store-0.0.1/README.md
--rw-r--r--   0        0        0     1412 2024-05-22 19:47:21.357025 ragstack_ai_knowledge_store-0.0.1/pyproject.toml
--rw-r--r--   0        0        0       74 2024-05-22 19:47:21.357025 ragstack_ai_knowledge_store-0.0.1/ragstack_knowledge_store/__init__.py
--rw-r--r--   0        0        0      613 2024-05-22 19:47:21.357025 ragstack_ai_knowledge_store-0.0.1/ragstack_knowledge_store/_utils.py
--rw-r--r--   0        0        0     1841 2024-05-22 19:47:21.357025 ragstack_ai_knowledge_store-0.0.1/ragstack_knowledge_store/concurrency.py
--rw-r--r--   0        0        0     1036 2024-05-22 19:47:21.357025 ragstack_ai_knowledge_store-0.0.1/ragstack_knowledge_store/content.py
--rw-r--r--   0        0        0    14301 2024-05-22 19:47:21.357025 ragstack_ai_knowledge_store-0.0.1/ragstack_knowledge_store/knowledge_store.py
--rw-r--r--   0        0        0     1095 1970-01-01 00:00:00.000000 ragstack_ai_knowledge_store-0.0.1/PKG-INFO
+-rw-r--r--   0        0        0     3857 2024-05-29 15:03:14.721553 ragstack_ai_knowledge_store-0.0.2/README.md
+-rw-r--r--   0        0        0     1414 2024-05-29 15:03:14.741554 ragstack_ai_knowledge_store-0.0.2/pyproject.toml
+-rw-r--r--   0        0        0       74 2024-05-29 15:03:14.741554 ragstack_ai_knowledge_store-0.0.2/ragstack_knowledge_store/__init__.py
+-rw-r--r--   0        0        0      613 2024-05-29 15:03:14.741554 ragstack_ai_knowledge_store-0.0.2/ragstack_knowledge_store/_utils.py
+-rw-r--r--   0        0        0     2638 2024-05-29 15:03:14.741554 ragstack_ai_knowledge_store-0.0.2/ragstack_knowledge_store/concurrency.py
+-rw-r--r--   0        0        0      640 2024-05-29 15:03:14.741554 ragstack_ai_knowledge_store-0.0.2/ragstack_knowledge_store/content.py
+-rw-r--r--   0        0        0    18050 2024-05-29 15:03:14.741554 ragstack_ai_knowledge_store-0.0.2/ragstack_knowledge_store/knowledge_store.py
+-rw-r--r--   0        0        0     4592 1970-01-01 00:00:00.000000 ragstack_ai_knowledge_store-0.0.2/PKG-INFO
```

### Comparing `ragstack_ai_knowledge_store-0.0.1/pyproject.toml` & `ragstack_ai_knowledge_store-0.0.2/pyproject.toml`

 * *Files 20% similar despite different names*

```diff
@@ -1,34 +1,35 @@
 [tool.poetry]
 name = "ragstack-ai-knowledge-store"
-version = "0.0.1"
+version = "0.0.2"
 description = "DataStax RAGStack Knowledge Store"
 license = "BUSL-1.1"
 authors = ["DataStax"]
 readme = "README.md"
 repository = "https://github.com/datastax/ragstack-ai"
 documentation = "https://docs.datastax.com/en/ragstack"
 packages = [{ include = "ragstack_knowledge_store" }]
 
 [tool.poetry.dependencies]
-python = ">=3.9,<3.12"
+python = ">=3.10,<3.13"
 langchain-core = "^0.2"
 cassio = "^0.1.7"
 
 [tool.poetry.group.dev.dependencies]
 ruff = "*"
 pytest = "*"
 mypy = "^1.10.0"
 pytest-asyncio = "^0.23.6"
 langchain-community = "^0.2"
 ipykernel = "^6.29.4"
 langchain-openai = "^0.1.7"
 testcontainers = "~3.7.1"
-# https://github.com/psf/requests/issues/6707
-requests = "<=2.31.0"
+precisely = "^0.1.9"
+setuptools = "^70.0.0"
+python-dotenv = "^1.0.1"
 
 [build-system]
 requires = ["poetry-core"]
 build-backend = "poetry.core.masonry.api"
 
 
 [tool.ruff]
```

### Comparing `ragstack_ai_knowledge_store-0.0.1/ragstack_knowledge_store/_utils.py` & `ragstack_ai_knowledge_store-0.0.2/ragstack_knowledge_store/_utils.py`

 * *Files identical despite different names*

### Comparing `ragstack_ai_knowledge_store-0.0.1/ragstack_knowledge_store/knowledge_store.py` & `ragstack_ai_knowledge_store-0.0.2/ragstack_knowledge_store/knowledge_store.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,22 +1,25 @@
 import secrets
-from typing import Any, Dict, Iterable, List, Optional, Set, Union
+from typing import Any, Dict, Iterable, List, NamedTuple, Optional, Sequence, Union
 
 from cassandra.cluster import ResponseFuture, Session
 from cassio.config import check_resolve_keyspace, check_resolve_session
 from langchain_core.documents import Document
 from langchain_core.embeddings import Embeddings
 from langchain_core.runnables import Runnable, RunnableLambda
 from langchain_core.vectorstores import VectorStore
 
 from .concurrency import ConcurrentQueries
+from .content import Kind
 
 CONTENT_ID = "content_id"
 PARENT_CONTENT_ID = "parent_content_id"
 KEYWORDS = "keywords"
+HREFS = "hrefs"
+URLS = "urls"
 
 
 def _row_to_document(row) -> Document:
     return Document(
         page_content=row.text_content,
         metadata={
             CONTENT_ID: row.content_id,
@@ -50,16 +53,16 @@
         *,
         node_table: str = "knowledge_nodes",
         edge_table: str = "knowledge_edges",
         session: Optional[Session] = None,
         keyspace: Optional[str] = None,
         apply_schema: bool = True,
         concurrency: int = 20,
-        infer_links: Union[bool, Set[str]] = True,
-        infer_keywords: Union[bool, Set[str]] = True,
+        infer_links: bool = True,
+        infer_keywords: bool = True,
     ):
         """
         Create the hybrid knowledge store.
 
         Parameters configure the ways that edges should be added between
         documents. Many take `Union[bool, Set[str]]`, with `False` disabling
         inference, `True` enabling it globally between all documents, and a set
@@ -68,23 +71,18 @@
         with the same `source` metadata value.
 
         Args:
             embedding: The embeddings to use for the document content.
             concurrency: Maximum number of queries to have concurrently executing.
             apply_schema: If true, the schema will be created if necessary. If false,
                 the schema must have already been applied.
-            infer_links: Whether to enable (and optionally scope for) inference
-                based on the `hrefs` and `urls` in the metadata. These metadata
-                fields should be populated with a collection of URLs referenced
-                by the document (hrefs) and a collection of URLs representing
-                the document (urls), respectively.
-            infer_keywords: Whether to enable (and optionally scope for)
-                inference based on the `keywords` in the metadata. This metadata
-                should be populated with a collection of keywords present in the
-                document.
+            infer_links: Whether to enable inference based on the `hrefs` and `urls`
+                in the metadata.
+            infer_keywords: Whether to enable nference based on the `keywords` in
+                the metadata.
         """
         session = check_resolve_session(session)
         keyspace = check_resolve_keyspace(keyspace)
 
         self._concurrency = concurrency
         self._embedding = embedding
         self._node_table = node_table
@@ -99,16 +97,16 @@
         self._infer_keywords = infer_keywords
 
         # TODO: Metadata
         # TODO: Parent ID / source ID / etc.
         self._insert_passage = session.prepare(
             f"""
             INSERT INTO {keyspace}.{node_table} (
-                content_id, kind, text_content, text_embedding, keywords
-            ) VALUES (?, 'passage', ?, ?, ?)
+                content_id, kind, text_content, text_embedding, keywords, urls, hrefs
+            ) VALUES (?, '{Kind.passage}', ?, ?, ?, ?, ?)
             """
         )
 
         self._insert_edge = session.prepare(
             f"""
             INSERT INTO {keyspace}.{edge_table} (
                 source_content_id, target_content_id
@@ -154,25 +152,43 @@
             f"""
             SELECT content_id
             FROM {keyspace}.{node_table}
             WHERE keywords CONTAINS ?
             """
         )
 
+        self._query_ids_by_href = session.prepare(
+            f"""
+            SELECT content_id
+            FROM {keyspace}.{node_table}
+            WHERE hrefs CONTAINS ?
+            """
+        )
+
+        self._query_ids_by_url = session.prepare(
+            f"""
+            SELECT content_id
+            FROM {keyspace}.{node_table}
+            WHERE urls CONTAINS ?
+            """
+        )
+
     def _apply_schema(self):
         """Apply the schema to the database."""
         embedding_dim = len(self._embedding.embed_query("Test Query"))
         self._session.execute(
             f"""CREATE TABLE IF NOT EXISTS {self._keyspace}.{self._node_table} (
                 content_id TEXT,
                 kind TEXT,
                 text_content TEXT,
                 text_embedding VECTOR<FLOAT, {embedding_dim}>,
 
                 keywords SET<TEXT>,
+                hrefs SET<TEXT>,
+                urls SET<TEXT>,
 
                 PRIMARY KEY (content_id)
             )
             """
         )
 
         self._session.execute(
@@ -201,19 +217,38 @@
             f"""
             CREATE CUSTOM INDEX IF NOT EXISTS {self._node_table}_keywords_index
             ON {self._keyspace}.{self._node_table} (keywords)
             USING 'StorageAttachedIndex';
             """
         )
 
+        self._session.execute(
+            f"""
+            CREATE CUSTOM INDEX IF NOT EXISTS {self._node_table}_hrefs_index
+            ON {self._keyspace}.{self._node_table} (hrefs)
+            USING 'StorageAttachedIndex';
+            """
+        )
+
+        self._session.execute(
+            f"""
+            CREATE CUSTOM INDEX IF NOT EXISTS {self._node_table}_urls_index
+            ON {self._keyspace}.{self._node_table} (urls)
+            USING 'StorageAttachedIndex';
+            """
+        )
+
     @property
     def embeddings(self) -> Optional[Embeddings]:
         """Access the query embedding object if available."""
         return self._embedding
 
+    def _concurrent_queries(self) -> ConcurrentQueries:
+        return ConcurrentQueries(self._session, concurrency=self._concurrency)
+
     # TODO: async
     def add_texts(
         self,
         texts: Iterable[str],
         metadatas: Optional[Iterable[Dict[str, Any]]] = None,
         **kwargs: Any,
     ) -> List[str]:
@@ -230,42 +265,107 @@
         texts = list(texts)
 
         metadatas: Iterable[Dict[str, str]] = (
             [{} for _ in texts] if metadatas is None else metadatas
         )
         text_embeddings = self._embedding.embed_documents(texts)
 
-        # TODO: Retrieve keywords concurrently?
         keywords_in_texts = {k for md in metadatas for k in md.get(KEYWORDS, {})}
-        keywords_to_ids = {
-            k: set(_results_to_ids(self._session.execute(self._query_ids_by_keyword, (k,))))
-            for k in keywords_in_texts
-        }
+        keywords_to_ids = {}
+        if self._infer_keywords:
+            with self._concurrent_queries() as cq:
+
+                def handle_keywords(rows, k):
+                    related = set(_results_to_ids(rows))
+                    keywords_to_ids[k] = related
+
+                for k in keywords_in_texts:
+                    cq.execute(
+                        self._query_ids_by_keyword,
+                        parameters=(k,),
+                        callback=lambda rows, k1=k: handle_keywords(rows, k1),
+                    )
+
+        new_hrefs_to_ids = {}
+        new_urls_to_ids = {}
 
-        with ConcurrentQueries(self._session, concurrency=self._concurrency) as cq:
+        ids = []
+        with self._concurrent_queries() as cq:
             tuples = zip(texts, text_embeddings, metadatas, strict=True)
             for text, text_embedding, metadata in tuples:
                 id = metadata.get(CONTENT_ID) or secrets.token_hex(8)
+                ids.append(id)
                 keywords = metadata.get(KEYWORDS, set())
+                urls = metadata.get(URLS, set())
+                hrefs = metadata.get(HREFS, set())
 
-                cq.execute(self._insert_passage, (id, text, text_embedding, keywords))
+                for url in urls:
+                    new_urls_to_ids.setdefault(url, set()).add(id)
+                for href in hrefs:
+                    new_hrefs_to_ids.setdefault(href, set()).add(id)
+
+                cq.execute(
+                    self._insert_passage, (id, text, text_embedding, keywords, urls, hrefs)
+                )
 
                 if (parent_content_id := metadata.get(PARENT_CONTENT_ID)) is not None:
                     cq.execute(self._insert_edge, (id, str(parent_content_id)))
+
                 if self._infer_keywords and keywords:
                     related_ids = set()
                     for k in keywords:
                         k_ids = keywords_to_ids.setdefault(k, set())
                         related_ids.update(k_ids)
                         k_ids.add(id)
 
                     for r in related_ids:
                         cq.execute(self._insert_edge, (id, r))
                         cq.execute(self._insert_edge, (r, id))
 
+        if self._infer_links:
+            # Assumption: we only need to add edges for href->url links that involve
+            # one of the new IDs as either the href or the url.
+
+            href_url_pairs = set()
+
+            with self._concurrent_queries() as cq:
+
+                def add_href_url_pairs(href_ids, url_ids):
+                    for href_id in href_ids:
+                        if not isinstance(href_id, str):
+                            href_id = href_id.content_id
+
+                        for url_id in url_ids:
+                            if not isinstance(url_id, str):
+                                url_id = url_id.content_id
+                            href_url_pairs.add((href_id, url_id))
+
+                for href, href_ids in new_hrefs_to_ids.items():
+                    cq.execute(
+                        self._query_ids_by_url,
+                        parameters=(href,),
+                        # Weird syntax to capture each `href_ids` instead of the last iteration.
+                        callback=lambda urls, hrefs=href_ids: add_href_url_pairs(hrefs, urls),
+                    )
+
+                for url, url_ids in new_urls_to_ids.items():
+                    cq.execute(
+                        self._query_ids_by_href,
+                        parameters=(url,),
+                        # Weird syntax to capture each `url_ids` instead of the last iteration.
+                        callback=lambda hrefs, urls=url_ids: add_href_url_pairs(hrefs, urls),
+                    )
+
+            with self._concurrent_queries() as cq:
+                for href, url in href_url_pairs:
+                    cq.execute(self._insert_edge, (href, url))
+            print(f"Added {len(href_url_pairs)} edges based on HREFs/URLs")
+
+        return ids
+
     # TODO: Async
     @classmethod
     def from_texts(
         cls,
         texts: List[str],
         embedding: Embeddings,
         metadatas: Optional[List[dict]] = None,
@@ -318,35 +418,31 @@
             filter: Filter on the metadata to apply.
         Returns:
             List of Document, the most simliar to the query vector.
         """
         results = self._session.execute(self._query_by_embedding, (query_vector, k))
         return _results_to_documents(results)
 
-    def _similarity_search_ids(
-        self,
-        query: str,
-        *,
-        k: int = 4,
-    ) -> Iterable[str]:
-        "Return content IDs of documents by similarity to `query`."
-        query_vector = self._embedding.embed_query(query)
-        results = self._session.execute(self._query_ids_by_embedding, (query_vector, k))
-        return _results_to_ids(results)
-
     def _query_by_ids(
         self,
         ids: Iterable[str],
     ) -> Iterable[Document]:
-        # TODO: Concurrency.
-        return [
-            _row_to_document(row)
-            for id in ids
-            for row in self._session.execute(self._query_by_id, (id,))
-        ]
+        results = []
+        with self._concurrent_queries() as cq:
+            for id in ids:
+
+                def add_documents(rows):
+                    results.extend(_results_to_documents(rows))
+
+                cq.execute(
+                    self._query_by_id,
+                    parameters=(id,),
+                    callback=lambda rows: add_documents(rows),
+                )
+        return results
 
     def _linked_ids(
         self,
         source_id: str,
     ) -> Iterable[str]:
         results = self._session.execute(self._query_linked_ids, (source_id,))
         return _results_to_ids(results)
@@ -365,33 +461,44 @@
             k: The number of Documents to return from the initial vector search.
                 Defaults to 4. Applies to each of the query strings.
             depth: The maximum depth of edges to traverse. Defaults to 1.
         Returns:
             Collection of retrieved documents.
         """
         if isinstance(query, str):
-            query = [query]
-
-        start_ids = {
-            content_id for q in query for content_id in self._similarity_search_ids(q, k=k)
-        }
-
-        result_ids = start_ids
-        source_ids = start_ids
-        for _ in range(0, depth):
-            # TODO: Concurrency
-            level_ids = {
-                content_id
-                for source_id in source_ids
-                for content_id in self._linked_ids(source_id)
-            }
-            result_ids.update(level_ids)
-            source_ids = level_ids
+            query = {query}
+        else:
+            query = set(query)
+
+        with self._concurrent_queries() as cq:
+            visited = {}
+
+            def visit(d: int, nodes: Sequence[NamedTuple]):
+                nonlocal visited
+                for node in nodes:
+                    content_id = node.content_id
+                    if d <= visited.get(content_id, depth):
+                        visited[content_id] = d
+                        # We discovered this for the first time, or at a shorter depth.
+                        if d + 1 <= depth:
+                            cq.execute(
+                                self._query_linked_ids,
+                                parameters=(content_id,),
+                                callback=lambda nodes, d=d: visit(d + 1, nodes),
+                            )
+
+            for q in query:
+                query_embedding = self._embedding.embed_query(q)
+                cq.execute(
+                    self._query_ids_by_embedding,
+                    parameters=(query_embedding, k),
+                    callback=lambda nodes: visit(0, nodes),
+                )
 
-        return self._query_by_ids(result_ids)
+        return self._query_by_ids(visited.keys())
 
     def as_retriever(
         self,
         *,
         k: int = 4,
         depth: int = 1,
     ) -> Runnable[Union[str | Iterable[str]], Iterable[Document]]:
```

