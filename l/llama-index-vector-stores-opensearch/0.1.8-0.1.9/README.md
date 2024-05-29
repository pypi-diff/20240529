# Comparing `tmp/llama_index_vector_stores_opensearch-0.1.8.tar.gz` & `tmp/llama_index_vector_stores_opensearch-0.1.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "llama_index_vector_stores_opensearch-0.1.8.tar", max compression
+gzip compressed data, was "llama_index_vector_stores_opensearch-0.1.9.tar", max compression
```

## Comparing `llama_index_vector_stores_opensearch-0.1.8.tar` & `llama_index_vector_stores_opensearch-0.1.9.tar`

### file list

```diff
@@ -1,5 +1,5 @@
--rw-r--r--   0        0        0       51 2024-03-15 17:45:47.334033 llama_index_vector_stores_opensearch-0.1.8/README.md
--rw-r--r--   0        0        0      176 2024-03-15 17:45:47.334033 llama_index_vector_stores_opensearch-0.1.8/llama_index/vector_stores/opensearch/__init__.py
--rw-r--r--   0        0        0    16958 2024-03-15 17:45:47.334033 llama_index_vector_stores_opensearch-0.1.8/llama_index/vector_stores/opensearch/base.py
--rw-r--r--   0        0        0     1555 2024-03-15 17:45:47.334033 llama_index_vector_stores_opensearch-0.1.8/pyproject.toml
--rw-r--r--   0        0        0      677 1970-01-01 00:00:00.000000 llama_index_vector_stores_opensearch-0.1.8/PKG-INFO
+-rw-r--r--   0        0        0       51 2024-05-29 00:51:31.566124 llama_index_vector_stores_opensearch-0.1.9/README.md
+-rw-r--r--   0        0        0      176 2024-05-29 00:51:31.566124 llama_index_vector_stores_opensearch-0.1.9/llama_index/vector_stores/opensearch/__init__.py
+-rw-r--r--   0        0        0    19141 2024-05-29 00:51:31.566124 llama_index_vector_stores_opensearch-0.1.9/llama_index/vector_stores/opensearch/base.py
+-rw-r--r--   0        0        0     1555 2024-05-29 00:51:31.566124 llama_index_vector_stores_opensearch-0.1.9/pyproject.toml
+-rw-r--r--   0        0        0      677 1970-01-01 00:00:00.000000 llama_index_vector_stores_opensearch-0.1.9/PKG-INFO
```

### Comparing `llama_index_vector_stores_opensearch-0.1.8/llama_index/vector_stores/opensearch/base.py` & `llama_index_vector_stores_opensearch-0.1.9/llama_index/vector_stores/opensearch/base.py`

 * *Files 19% similar despite different names*

```diff
@@ -28,228 +28,14 @@
 )
 INVALID_HYBRID_QUERY_ERROR = (
     "Please specify the lexical_query and search_pipeline for hybrid search."
 )
 MATCH_ALL_QUERY = {"match_all": {}}  # type: Dict
 
 
-def _import_async_opensearch() -> Any:
-    """Import OpenSearch if available, otherwise raise error."""
-    return AsyncOpenSearch
-
-
-def _import_async_bulk() -> Any:
-    """Import bulk if available, otherwise raise error."""
-    return async_bulk
-
-
-def _import_not_found_error() -> Any:
-    """Import not found error if available, otherwise raise error."""
-    return NotFoundError
-
-
-def _get_async_opensearch_client(opensearch_url: str, **kwargs: Any) -> Any:
-    """Get AsyncOpenSearch client from the opensearch_url, otherwise raise error."""
-    try:
-        opensearch = _import_async_opensearch()
-        client = opensearch(opensearch_url, **kwargs)
-
-    except ValueError as e:
-        raise ValueError(
-            f"AsyncOpenSearch client string provided is not in proper format. "
-            f"Got error: {e} "
-        )
-    return client
-
-
-async def _bulk_ingest_embeddings(
-    client: Any,
-    index_name: str,
-    embeddings: List[List[float]],
-    texts: Iterable[str],
-    metadatas: Optional[List[dict]] = None,
-    ids: Optional[List[str]] = None,
-    vector_field: str = "embedding",
-    text_field: str = "content",
-    mapping: Optional[Dict] = None,
-    max_chunk_bytes: Optional[int] = 1 * 1024 * 1024,
-    is_aoss: bool = False,
-) -> List[str]:
-    """Async Bulk Ingest Embeddings into given index."""
-    if not mapping:
-        mapping = {}
-
-    async_bulk = _import_async_bulk()
-    not_found_error = _import_not_found_error()
-    requests = []
-    return_ids = []
-    mapping = mapping
-
-    try:
-        await client.indices.get(index=index_name)
-    except not_found_error:
-        await client.indices.create(index=index_name, body=mapping)
-
-    for i, text in enumerate(texts):
-        metadata = metadatas[i] if metadatas else {}
-        _id = ids[i] if ids else str(uuid.uuid4())
-        request = {
-            "_op_type": "index",
-            "_index": index_name,
-            vector_field: embeddings[i],
-            text_field: text,
-            "metadata": metadata,
-        }
-        if is_aoss:
-            request["id"] = _id
-        else:
-            request["_id"] = _id
-        requests.append(request)
-        return_ids.append(_id)
-    await async_bulk(client, requests, max_chunk_bytes=max_chunk_bytes)
-    if not is_aoss:
-        await client.indices.refresh(index=index_name)
-    return return_ids
-
-
-def _default_approximate_search_query(
-    query_vector: List[float],
-    k: int = 4,
-    vector_field: str = "embedding",
-) -> Dict:
-    """For Approximate k-NN Search, this is the default query."""
-    return {
-        "size": k,
-        "query": {"knn": {vector_field: {"vector": query_vector, "k": k}}},
-    }
-
-
-def _parse_filters(filters: Optional[MetadataFilters]) -> Any:
-    pre_filter = []
-    if filters is not None:
-        for f in filters.legacy_filters():
-            pre_filter.append({f.key: json.loads(str(f.value))})
-
-    return pre_filter
-
-
-def _knn_search_query(
-    embedding_field: str,
-    query_embedding: List[float],
-    k: int,
-    filters: Optional[MetadataFilters] = None,
-) -> Dict:
-    """
-    Do knn search.
-
-    If there are no filters do approx-knn search.
-    If there are (pre)-filters, do an exhaustive exact knn search using 'painless
-        scripting'.
-
-    Note that approximate knn search does not support pre-filtering.
-
-    Args:
-        query_embedding: Vector embedding to query.
-        k: Maximum number of results.
-        filters: Optional filters to apply before the search.
-            Supports filter-context queries documented at
-            https://opensearch.org/docs/latest/query-dsl/query-filter-context/
-
-    Returns:
-        Up to k docs closest to query_embedding
-    """
-    if filters is None:
-        search_query = _default_approximate_search_query(
-            query_embedding, k, vector_field=embedding_field
-        )
-    else:
-        pre_filter = _parse_filters(filters)
-        # https://opensearch.org/docs/latest/search-plugins/knn/painless-functions/
-        search_query = _default_painless_scripting_query(
-            query_embedding,
-            k,
-            space_type="l2Squared",
-            pre_filter={"bool": {"filter": pre_filter}},
-            vector_field=embedding_field,
-        )
-
-    return search_query
-
-
-def _hybrid_search_query(
-    text_field: str,
-    query_str: str,
-    embedding_field: str,
-    query_embedding: List[float],
-    k: int,
-    filters: Optional[MetadataFilters] = None,
-) -> Dict:
-    knn_query = _knn_search_query(embedding_field, query_embedding, k, filters)["query"]
-    lexical_query = {"must": {"match": {text_field: {"query": query_str}}}}
-
-    parsed_filters = _parse_filters(filters)
-    if len(parsed_filters) > 0:
-        lexical_query["filter"] = parsed_filters
-    return {
-        "size": k,
-        "query": {"hybrid": {"queries": [{"bool": lexical_query}, knn_query]}},
-    }
-
-
-def __get_painless_scripting_source(
-    space_type: str, vector_field: str = "embedding"
-) -> str:
-    """For Painless Scripting, it returns the script source based on space type."""
-    source_value = f"(1.0 + {space_type}(params.query_value, doc['{vector_field}']))"
-    if space_type == "cosineSimilarity":
-        return source_value
-    else:
-        return f"1/{source_value}"
-
-
-def _default_painless_scripting_query(
-    query_vector: List[float],
-    k: int = 4,
-    space_type: str = "l2Squared",
-    pre_filter: Optional[Union[Dict, List]] = None,
-    vector_field: str = "embedding",
-) -> Dict:
-    """For Painless Scripting Search, this is the default query."""
-    if not pre_filter:
-        pre_filter = MATCH_ALL_QUERY
-
-    source = __get_painless_scripting_source(space_type, vector_field)
-    return {
-        "size": k,
-        "query": {
-            "script_score": {
-                "query": pre_filter,
-                "script": {
-                    "source": source,
-                    "params": {
-                        "field": vector_field,
-                        "query_value": query_vector,
-                    },
-                },
-            }
-        },
-    }
-
-
-def _is_aoss_enabled(http_auth: Any) -> bool:
-    """Check if the service is http_auth is set as `aoss`."""
-    if (
-        http_auth is not None
-        and hasattr(http_auth, "service")
-        and http_auth.service == "aoss"
-    ):
-        return True
-    return False
-
-
 class OpensearchVectorClient:
     """
     Object encapsulating an Opensearch index that has vector search enabled.
 
     If the index does not yet exist, it is created during init.
     Therefore, the underlying index is assumed to either:
     1) not exist yet or 2) be created due to previous usage of this class.
@@ -298,76 +84,287 @@
         self._dim = dim
         self._index = index
         self._text_field = text_field
         self._max_chunk_bytes = max_chunk_bytes
 
         self._search_pipeline = search_pipeline
         http_auth = kwargs.get("http_auth")
-        self.is_aoss = _is_aoss_enabled(http_auth=http_auth)
+        self.is_aoss = self._is_aoss_enabled(http_auth=http_auth)
         # initialize mapping
         idx_conf = {
             "settings": {"index": {"knn": True, "knn.algo_param.ef_search": 100}},
             "mappings": {
                 "properties": {
                     embedding_field: {
                         "type": "knn_vector",
                         "dimension": dim,
                         "method": method,
                     },
                 }
             },
         }
-        self._os_client = _get_async_opensearch_client(self._endpoint, **kwargs)
-        not_found_error = _import_not_found_error()
+        self._os_client = self._get_async_opensearch_client(self._endpoint, **kwargs)
+        not_found_error = self._import_not_found_error()
 
         event_loop = asyncio.get_event_loop()
         try:
             event_loop.run_until_complete(
                 self._os_client.indices.get(index=self._index)
             )
         except not_found_error:
             event_loop.run_until_complete(
                 self._os_client.indices.create(index=self._index, body=idx_conf)
             )
             event_loop.run_until_complete(
                 self._os_client.indices.refresh(index=self._index)
             )
 
+    def _import_async_opensearch(self) -> Any:
+        """Import OpenSearch if available, otherwise raise error."""
+        return AsyncOpenSearch
+
+    def _import_async_bulk(self) -> Any:
+        """Import bulk if available, otherwise raise error."""
+        return async_bulk
+
+    def _import_not_found_error(self) -> Any:
+        """Import not found error if available, otherwise raise error."""
+        return NotFoundError
+
+    def _get_async_opensearch_client(self, opensearch_url: str, **kwargs: Any) -> Any:
+        """Get AsyncOpenSearch client from the opensearch_url, otherwise raise error."""
+        try:
+            opensearch = self._import_async_opensearch()
+            client = opensearch(opensearch_url, **kwargs)
+
+        except ValueError as e:
+            raise ValueError(
+                f"AsyncOpenSearch client string provided is not in proper format. "
+                f"Got error: {e} "
+            )
+        return client
+
+    async def _bulk_ingest_embeddings(
+        self,
+        client: Any,
+        index_name: str,
+        embeddings: List[List[float]],
+        texts: Iterable[str],
+        metadatas: Optional[List[dict]] = None,
+        ids: Optional[List[str]] = None,
+        vector_field: str = "embedding",
+        text_field: str = "content",
+        mapping: Optional[Dict] = None,
+        max_chunk_bytes: Optional[int] = 1 * 1024 * 1024,
+        is_aoss: bool = False,
+    ) -> List[str]:
+        """Async Bulk Ingest Embeddings into given index."""
+        if not mapping:
+            mapping = {}
+
+        async_bulk = self._import_async_bulk()
+        not_found_error = self._import_not_found_error()
+        requests = []
+        return_ids = []
+        mapping = mapping
+
+        try:
+            await client.indices.get(index=index_name)
+        except not_found_error:
+            await client.indices.create(index=index_name, body=mapping)
+
+        for i, text in enumerate(texts):
+            metadata = metadatas[i] if metadatas else {}
+            _id = ids[i] if ids else str(uuid.uuid4())
+            request = {
+                "_op_type": "index",
+                "_index": index_name,
+                vector_field: embeddings[i],
+                text_field: text,
+                "metadata": metadata,
+            }
+            if is_aoss:
+                request["id"] = _id
+            else:
+                request["_id"] = _id
+            requests.append(request)
+            return_ids.append(_id)
+        await async_bulk(client, requests, max_chunk_bytes=max_chunk_bytes)
+        if not is_aoss:
+            await client.indices.refresh(index=index_name)
+        return return_ids
+
+    def _default_approximate_search_query(
+        self,
+        query_vector: List[float],
+        k: int = 4,
+        vector_field: str = "embedding",
+    ) -> Dict:
+        """For Approximate k-NN Search, this is the default query."""
+        return {
+            "size": k,
+            "query": {"knn": {vector_field: {"vector": query_vector, "k": k}}},
+        }
+
+    def _parse_filters(self, filters: Optional[MetadataFilters]) -> Any:
+        pre_filter = []
+        if filters is not None:
+            for f in filters.legacy_filters():
+                pre_filter.append({f.key: json.loads(str(f.value))})
+
+        return pre_filter
+
+    def _knn_search_query(
+        self,
+        embedding_field: str,
+        query_embedding: List[float],
+        k: int,
+        filters: Optional[MetadataFilters] = None,
+    ) -> Dict:
+        """
+        Do knn search.
+
+        If there are no filters do approx-knn search.
+        If there are (pre)-filters, do an exhaustive exact knn search using 'painless
+            scripting'.
+
+        Note that approximate knn search does not support pre-filtering.
+
+        Args:
+            query_embedding: Vector embedding to query.
+            k: Maximum number of results.
+            filters: Optional filters to apply before the search.
+                Supports filter-context queries documented at
+                https://opensearch.org/docs/latest/query-dsl/query-filter-context/
+
+        Returns:
+            Up to k docs closest to query_embedding
+        """
+        if filters is None:
+            search_query = self._default_approximate_search_query(
+                query_embedding, k, vector_field=embedding_field
+            )
+        else:
+            pre_filter = self._parse_filters(filters)
+            # https://opensearch.org/docs/latest/search-plugins/knn/painless-functions/
+            search_query = self._default_painless_scripting_query(
+                query_embedding,
+                k,
+                space_type="l2Squared",
+                pre_filter={"bool": {"filter": pre_filter}},
+                vector_field=embedding_field,
+            )
+
+        return search_query
+
+    def _hybrid_search_query(
+        self,
+        text_field: str,
+        query_str: str,
+        embedding_field: str,
+        query_embedding: List[float],
+        k: int,
+        filters: Optional[MetadataFilters] = None,
+    ) -> Dict:
+        knn_query = self._knn_search_query(
+            embedding_field, query_embedding, k, filters
+        )["query"]
+        lexical_query = {"must": {"match": {text_field: {"query": query_str}}}}
+
+        parsed_filters = self._parse_filters(filters)
+        if len(parsed_filters) > 0:
+            lexical_query["filter"] = parsed_filters
+        return {
+            "size": k,
+            "query": {"hybrid": {"queries": [{"bool": lexical_query}, knn_query]}},
+        }
+
+    def __get_painless_scripting_source(
+        self, space_type: str, vector_field: str = "embedding"
+    ) -> str:
+        """For Painless Scripting, it returns the script source based on space type."""
+        source_value = (
+            f"(1.0 + {space_type}(params.query_value, doc['{vector_field}']))"
+        )
+        if space_type == "cosineSimilarity":
+            return source_value
+        else:
+            return f"1/{source_value}"
+
+    def _default_painless_scripting_query(
+        self,
+        query_vector: List[float],
+        k: int = 4,
+        space_type: str = "l2Squared",
+        pre_filter: Optional[Union[Dict, List]] = None,
+        vector_field: str = "embedding",
+    ) -> Dict:
+        """For Painless Scripting Search, this is the default query."""
+        if not pre_filter:
+            pre_filter = MATCH_ALL_QUERY
+
+        source = self.__get_painless_scripting_source(space_type, vector_field)
+        return {
+            "size": k,
+            "query": {
+                "script_score": {
+                    "query": pre_filter,
+                    "script": {
+                        "source": source,
+                        "params": {
+                            "field": vector_field,
+                            "query_value": query_vector,
+                        },
+                    },
+                }
+            },
+        }
+
+    def _is_aoss_enabled(self, http_auth: Any) -> bool:
+        """Check if the service is http_auth is set as `aoss`."""
+        if (
+            http_auth is not None
+            and hasattr(http_auth, "service")
+            and http_auth.service == "aoss"
+        ):
+            return True
+        return False
+
     async def index_results(self, nodes: List[BaseNode], **kwargs: Any) -> List[str]:
         """Store results in the index."""
         embeddings: List[List[float]] = []
         texts: List[str] = []
         metadatas: List[dict] = []
         ids: List[str] = []
         for node in nodes:
             ids.append(node.node_id)
             embeddings.append(node.get_embedding())
             texts.append(node.get_content(metadata_mode=MetadataMode.NONE))
             metadatas.append(node_to_metadata_dict(node, remove_text=True))
 
-        return await _bulk_ingest_embeddings(
+        return await self._bulk_ingest_embeddings(
             self._os_client,
             self._index,
             embeddings,
             texts,
             metadatas=metadatas,
             ids=ids,
             vector_field=self._embedding_field,
             text_field=self._text_field,
             mapping=None,
             max_chunk_bytes=self._max_chunk_bytes,
             is_aoss=self.is_aoss,
         )
 
-    async def delete_doc_id(self, doc_id: str) -> None:
+    async def delete_by_doc_id(self, doc_id: str) -> None:
         """
-        Delete a document.
+        Deletes all OpenSearch documents corresponding to the given LlamaIndex `Document` ID.
 
         Args:
-            doc_id (str): document id
+            doc_id (str): a LlamaIndex `Document` id
         """
         search_query = {
             "query": {"term": {"metadata.doc_id.keyword": {"value": doc_id}}}
         }
         await self._os_client.delete_by_query(index=self._index, body=search_query)
 
     async def aquery(
@@ -377,28 +374,31 @@
         query_embedding: List[float],
         k: int,
         filters: Optional[MetadataFilters] = None,
     ) -> VectorStoreQueryResult:
         if query_mode == VectorStoreQueryMode.HYBRID:
             if query_str is None or self._search_pipeline is None:
                 raise ValueError(INVALID_HYBRID_QUERY_ERROR)
-            search_query = _hybrid_search_query(
+            search_query = self._hybrid_search_query(
                 self._text_field,
                 query_str,
                 self._embedding_field,
                 query_embedding,
                 k,
                 filters=filters,
             )
-            params = {"search_pipeline": self._search_pipeline}
+            params = {
+                "search_pipeline": self._search_pipeline,
+                "_source_excludes": ["embedding"],
+            }
         else:
-            search_query = _knn_search_query(
+            search_query = self._knn_search_query(
                 self._embedding_field, query_embedding, k, filters=filters
             )
-            params = None
+            params = {"_source_excludes": ["embedding"]}
 
         res = await self._os_client.search(
             index=self._index, body=search_query, params=params
         )
         nodes = []
         ids = []
         scores = []
@@ -439,14 +439,43 @@
 class OpensearchVectorStore(BasePydanticVectorStore):
     """
     Elasticsearch/Opensearch vector store.
 
     Args:
         client (OpensearchVectorClient): Vector index client to use
             for data insertion/querying.
+
+    Examples:
+        `pip install llama-index-vector-stores-opensearch`
+
+        ```python
+        from llama_index.vector_stores.opensearch import (
+            OpensearchVectorStore,
+            OpensearchVectorClient,
+        )
+
+        # http endpoint for your cluster (opensearch required for vector index usage)
+        endpoint = "http://localhost:9200"
+        # index to demonstrate the VectorStore impl
+        idx = "gpt-index-demo"
+
+        # OpensearchVectorClient stores text in this field by default
+        text_field = "content"
+        # OpensearchVectorClient stores embeddings in this field by default
+        embedding_field = "embedding"
+
+        # OpensearchVectorClient encapsulates logic for a
+        # single opensearch index with vector search enabled
+        client = OpensearchVectorClient(
+            endpoint, idx, 1536, embedding_field=embedding_field, text_field=text_field
+        )
+
+        # initialize vector store
+        vector_store = OpensearchVectorStore(client)
+        ```
     """
 
     stores_text: bool = True
     _client: OpensearchVectorClient = PrivateAttr(default=None)
 
     def __init__(
         self,
@@ -490,33 +519,33 @@
 
         """
         await self._client.index_results(nodes)
         return [result.node_id for result in nodes]
 
     def delete(self, ref_doc_id: str, **delete_kwargs: Any) -> None:
         """
-        Delete nodes using with ref_doc_id.
+        Delete nodes using a ref_doc_id.
 
         Args:
-            ref_doc_id (str): The doc_id of the document to delete.
+            ref_doc_id (str): The doc_id of the document whose nodes should be deleted.
 
         """
         asyncio.get_event_loop().run_until_complete(
             self.adelete(ref_doc_id, **delete_kwargs)
         )
 
     async def adelete(self, ref_doc_id: str, **delete_kwargs: Any) -> None:
         """
-        Async delete nodes using with ref_doc_id.
+        Async delete nodes using a ref_doc_id.
 
         Args:
-            ref_doc_id (str): The doc_id of the document to delete.
+            ref_doc_id (str): The doc_id of the document whose nodes should be deleted.
 
         """
-        await self._client.delete_doc_id(ref_doc_id)
+        await self._client.delete_by_doc_id(ref_doc_id)
 
     def query(self, query: VectorStoreQuery, **kwargs: Any) -> VectorStoreQueryResult:
         """
         Query index for top k most similar nodes.
 
         Args:
             query (VectorStoreQuery): Store query object.
```

### Comparing `llama_index_vector_stores_opensearch-0.1.8/pyproject.toml` & `llama_index_vector_stores_opensearch-0.1.9/pyproject.toml`

 * *Files 4% similar despite different names*

```diff
@@ -23,15 +23,15 @@
 [tool.poetry]
 authors = ["Your Name <you@example.com>"]
 description = "llama-index vector_stores opensearch integration"
 exclude = ["**/BUILD"]
 license = "MIT"
 name = "llama-index-vector-stores-opensearch"
 readme = "README.md"
-version = "0.1.8"
+version = "0.1.9"
 
 [tool.poetry.dependencies]
 python = ">=3.8.1,<4.0"
 llama-index-core = "^0.10.1"
 
 [tool.poetry.dependencies.opensearch-py]
 extras = ["async"]
```

### Comparing `llama_index_vector_stores_opensearch-0.1.8/PKG-INFO` & `llama_index_vector_stores_opensearch-0.1.9/PKG-INFO`

 * *Files 14% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: llama-index-vector-stores-opensearch
-Version: 0.1.8
+Version: 0.1.9
 Summary: llama-index vector_stores opensearch integration
 License: MIT
 Author: Your Name
 Author-email: you@example.com
 Requires-Python: >=3.8.1,<4.0
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
```

