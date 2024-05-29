# Comparing `tmp/chromadb_data_pipes-0.0.8.tar.gz` & `tmp/chromadb_data_pipes-0.0.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "chromadb_data_pipes-0.0.8.tar", max compression
+gzip compressed data, was "chromadb_data_pipes-0.0.9.tar", max compression
```

## Comparing `chromadb_data_pipes-0.0.8.tar` & `chromadb_data_pipes-0.0.9.tar`

### file list

```diff
@@ -1,31 +1,31 @@
--rw-r--r--   0        0        0     1077 2024-04-06 16:10:19.455087 chromadb_data_pipes-0.0.8/LICENSE.md
--rw-r--r--   0        0        0     4852 2024-04-06 16:10:19.455087 chromadb_data_pipes-0.0.8/README.md
--rw-r--r--   0        0        0     1989 2024-04-06 16:10:19.455087 chromadb_data_pipes-0.0.8/chroma_dp/__init__.py
--rw-r--r--   0        0        0        0 2024-04-06 16:10:19.455087 chromadb_data_pipes-0.0.8/chroma_dp/chroma/__init__.py
--rw-r--r--   0        0        0     5792 2024-04-06 16:10:19.455087 chromadb_data_pipes-0.0.8/chroma_dp/chroma/chroma_export.py
--rw-r--r--   0        0        0     5478 2024-04-06 16:10:19.455087 chromadb_data_pipes-0.0.8/chroma_dp/chroma/chroma_import.py
--rw-r--r--   0        0        0    15486 2024-04-06 16:10:19.455087 chromadb_data_pipes-0.0.8/chroma_dp/huggingface/__init__.py
--rw-r--r--   0        0        0     1798 2024-04-06 16:10:19.455087 chromadb_data_pipes-0.0.8/chroma_dp/huggingface/utils.py
--rw-r--r--   0        0        0     2866 2024-04-06 16:10:19.455087 chromadb_data_pipes-0.0.8/chroma_dp/main.py
--rw-r--r--   0        0        0        0 2024-04-06 16:10:19.455087 chromadb_data_pipes-0.0.8/chroma_dp/processor/__init__.py
--rw-r--r--   0        0        0     3071 2024-04-06 16:10:19.455087 chromadb_data_pipes-0.0.8/chroma_dp/processor/chunk.py
--rw-r--r--   0        0        0     3066 2024-04-06 16:10:19.455087 chromadb_data_pipes-0.0.8/chroma_dp/processor/embed.py
--rw-r--r--   0        0        0     4921 2024-04-06 16:10:19.455087 chromadb_data_pipes-0.0.8/chroma_dp/processor/id.py
--rw-r--r--   0        0        0     1343 2024-04-06 16:10:19.455087 chromadb_data_pipes-0.0.8/chroma_dp/processor/langchain_utils.py
--rw-r--r--   0        0        0     4473 2024-04-06 16:10:19.455087 chromadb_data_pipes-0.0.8/chroma_dp/processor/metadata.py
--rw-r--r--   0        0        0        0 2024-04-06 16:10:19.455087 chromadb_data_pipes-0.0.8/chroma_dp/processor/misc/__init__.py
--rw-r--r--   0        0        0     2028 2024-04-06 16:10:19.455087 chromadb_data_pipes-0.0.8/chroma_dp/processor/misc/emoji_clean.py
--rw-r--r--   0        0        0        0 2024-04-06 16:10:19.455087 chromadb_data_pipes-0.0.8/chroma_dp/producer/__init__.py
--rw-r--r--   0        0        0        0 2024-04-06 16:10:19.455087 chromadb_data_pipes-0.0.8/chroma_dp/producer/file/__init__.py
--rw-r--r--   0        0        0     4188 2024-04-06 16:10:19.455087 chromadb_data_pipes-0.0.8/chroma_dp/producer/file/csv.py
--rw-r--r--   0        0        0     2302 2024-04-06 16:10:19.455087 chromadb_data_pipes-0.0.8/chroma_dp/producer/file/pdf.py
--rw-r--r--   0        0        0     2363 2024-04-06 16:10:19.455087 chromadb_data_pipes-0.0.8/chroma_dp/producer/file/text.py
--rw-r--r--   0        0        0       97 2024-04-06 16:10:19.455087 chromadb_data_pipes-0.0.8/chroma_dp/producer/langchain/__init__.py
--rw-r--r--   0        0        0        0 2024-04-06 16:10:19.455087 chromadb_data_pipes-0.0.8/chroma_dp/producer/url/__init__.py
--rw-r--r--   0        0        0     2900 2024-04-06 16:10:19.455087 chromadb_data_pipes-0.0.8/chroma_dp/producer/url/url_loader.py
--rw-r--r--   0        0        0      482 2024-04-06 16:10:19.455087 chromadb_data_pipes-0.0.8/chroma_dp/utils/__init__.py
--rw-r--r--   0        0        0     6598 2024-04-06 16:10:19.455087 chromadb_data_pipes-0.0.8/chroma_dp/utils/chroma.py
--rw-r--r--   0        0        0     2918 2024-04-06 16:10:19.455087 chromadb_data_pipes-0.0.8/chroma_dp/utils/embedding.py
--rw-r--r--   0        0        0      608 2024-04-06 16:10:19.455087 chromadb_data_pipes-0.0.8/chroma_dp/utils/templating.py
--rw-r--r--   0        0        0     1604 2024-04-06 16:10:19.459087 chromadb_data_pipes-0.0.8/pyproject.toml
--rw-r--r--   0        0        0     6147 1970-01-01 00:00:00.000000 chromadb_data_pipes-0.0.8/PKG-INFO
+-rw-r--r--   0        0        0     1077 2024-05-08 10:08:59.960432 chromadb_data_pipes-0.0.9/LICENSE.md
+-rw-r--r--   0        0        0     4852 2024-05-08 10:08:59.960432 chromadb_data_pipes-0.0.9/README.md
+-rw-r--r--   0        0        0     1989 2024-05-08 10:08:59.960432 chromadb_data_pipes-0.0.9/chroma_dp/__init__.py
+-rw-r--r--   0        0        0        0 2024-05-08 10:08:59.960432 chromadb_data_pipes-0.0.9/chroma_dp/chroma/__init__.py
+-rw-r--r--   0        0        0     6643 2024-05-08 10:08:59.960432 chromadb_data_pipes-0.0.9/chroma_dp/chroma/chroma_export.py
+-rw-r--r--   0        0        0     5478 2024-05-08 10:08:59.960432 chromadb_data_pipes-0.0.9/chroma_dp/chroma/chroma_import.py
+-rw-r--r--   0        0        0    15486 2024-05-08 10:08:59.960432 chromadb_data_pipes-0.0.9/chroma_dp/huggingface/__init__.py
+-rw-r--r--   0        0        0     1798 2024-05-08 10:08:59.960432 chromadb_data_pipes-0.0.9/chroma_dp/huggingface/utils.py
+-rw-r--r--   0        0        0     2871 2024-05-08 10:08:59.960432 chromadb_data_pipes-0.0.9/chroma_dp/main.py
+-rw-r--r--   0        0        0        0 2024-05-08 10:08:59.960432 chromadb_data_pipes-0.0.9/chroma_dp/processor/__init__.py
+-rw-r--r--   0        0        0     3071 2024-05-08 10:08:59.960432 chromadb_data_pipes-0.0.9/chroma_dp/processor/chunk.py
+-rw-r--r--   0        0        0     3066 2024-05-08 10:08:59.964432 chromadb_data_pipes-0.0.9/chroma_dp/processor/embed.py
+-rw-r--r--   0        0        0     4921 2024-05-08 10:08:59.964432 chromadb_data_pipes-0.0.9/chroma_dp/processor/id.py
+-rw-r--r--   0        0        0     1343 2024-05-08 10:08:59.964432 chromadb_data_pipes-0.0.9/chroma_dp/processor/langchain_utils.py
+-rw-r--r--   0        0        0     4473 2024-05-08 10:08:59.964432 chromadb_data_pipes-0.0.9/chroma_dp/processor/metadata.py
+-rw-r--r--   0        0        0        0 2024-05-08 10:08:59.964432 chromadb_data_pipes-0.0.9/chroma_dp/processor/misc/__init__.py
+-rw-r--r--   0        0        0     2028 2024-05-08 10:08:59.964432 chromadb_data_pipes-0.0.9/chroma_dp/processor/misc/emoji_clean.py
+-rw-r--r--   0        0        0        0 2024-05-08 10:08:59.964432 chromadb_data_pipes-0.0.9/chroma_dp/producer/__init__.py
+-rw-r--r--   0        0        0        0 2024-05-08 10:08:59.964432 chromadb_data_pipes-0.0.9/chroma_dp/producer/file/__init__.py
+-rw-r--r--   0        0        0     4188 2024-05-08 10:08:59.964432 chromadb_data_pipes-0.0.9/chroma_dp/producer/file/csv.py
+-rw-r--r--   0        0        0     2302 2024-05-08 10:08:59.964432 chromadb_data_pipes-0.0.9/chroma_dp/producer/file/pdf.py
+-rw-r--r--   0        0        0     2363 2024-05-08 10:08:59.964432 chromadb_data_pipes-0.0.9/chroma_dp/producer/file/text.py
+-rw-r--r--   0        0        0       97 2024-05-08 10:08:59.964432 chromadb_data_pipes-0.0.9/chroma_dp/producer/langchain/__init__.py
+-rw-r--r--   0        0        0        0 2024-05-08 10:08:59.964432 chromadb_data_pipes-0.0.9/chroma_dp/producer/url/__init__.py
+-rw-r--r--   0        0        0     2900 2024-05-08 10:08:59.964432 chromadb_data_pipes-0.0.9/chroma_dp/producer/url/url_loader.py
+-rw-r--r--   0        0        0      482 2024-05-08 10:08:59.964432 chromadb_data_pipes-0.0.9/chroma_dp/utils/__init__.py
+-rw-r--r--   0        0        0     6598 2024-05-08 10:08:59.964432 chromadb_data_pipes-0.0.9/chroma_dp/utils/chroma.py
+-rw-r--r--   0        0        0     2918 2024-05-08 10:08:59.964432 chromadb_data_pipes-0.0.9/chroma_dp/utils/embedding.py
+-rw-r--r--   0        0        0      608 2024-05-08 10:08:59.964432 chromadb_data_pipes-0.0.9/chroma_dp/utils/templating.py
+-rw-r--r--   0        0        0     1610 2024-05-08 10:08:59.968432 chromadb_data_pipes-0.0.9/pyproject.toml
+-rw-r--r--   0        0        0     6143 1970-01-01 00:00:00.000000 chromadb_data_pipes-0.0.9/PKG-INFO
```

### Comparing `chromadb_data_pipes-0.0.8/LICENSE.md` & `chromadb_data_pipes-0.0.9/LICENSE.md`

 * *Files identical despite different names*

### Comparing `chromadb_data_pipes-0.0.8/README.md` & `chromadb_data_pipes-0.0.9/README.md`

 * *Files identical despite different names*

### Comparing `chromadb_data_pipes-0.0.8/chroma_dp/__init__.py` & `chromadb_data_pipes-0.0.9/chroma_dp/__init__.py`

 * *Files identical despite different names*

### Comparing `chromadb_data_pipes-0.0.8/chroma_dp/chroma/chroma_export.py` & `chromadb_data_pipes-0.0.9/chroma_dp/chroma/chroma_export.py`

 * *Files 20% similar despite different names*

```diff
@@ -65,52 +65,27 @@
         offset=offset,
         include=["embeddings", "documents", "metadatas"],
     )
     return result
 
 
 def chroma_export(
-    uri: Annotated[str, typer.Argument(help="The Chroma endpoint.")],
-    collection: Annotated[
-        Optional[str], typer.Option(help="The Chroma collection.")
-    ] = None,
-    export_file: Optional[str] = typer.Option(
-        None, "--out", help="Export .jsonl file."
-    ),
-    append: Annotated[bool, typer.Option(help="Append to export file.")] = False,
-    limit: Annotated[int, typer.Option(help="The limit.")] = -1,
-    offset: Annotated[int, typer.Option(help="The offset.")] = 0,
-    batch_size: Annotated[int, typer.Option(help="The batch size.")] = 100,
-    embed_feature: Annotated[
-        str, typer.Option(help="The embedding feature.")
-    ] = "embedding",
-    meta_features: Optional[List[str]] = typer.Option(None,help="The metadata features."),
-    id_feature: Annotated[str, typer.Option(help="The id feature.")] = "id",
-    doc_feature: Annotated[
-        str, typer.Option(help="The document feature.")
-    ] = "text_chunk",
-    where: Optional[str] = typer.Option(
-        None,
-        "--where",
-        "-m",
-        help='Metadata filter. JSON with Chroma syntax is expected - \'{"metadata_key": "metadata_value"}\'',
-    ),
-    where_document: Optional[str] = typer.Option(
-        None,
-        "--where-document",
-        "-d",
-        help='Document filter string - JSON with Chroma syntax is expected - \'{"$contains": "search for this"}\'',
-    ),
-    format_output: Optional[str] = typer.Option(
-        "record", "--format",
-        help="Export format. Default is `record`. Supported formats: `record` and `jsonl`. "
-    ),
-) -> None:
-    if uri is None:
-        raise ValueError("Please provide a ChromaDP URI.")
+    uri: str,
+    collection: Optional[str] = None,
+    limit: Optional[int] = -1,
+    offset: Optional[int] = 0,
+    batch_size: Optional[int] = 100,
+    embed_feature: Optional[str] = "embedding",
+    meta_features: Optional[List[str]] = None,
+    id_feature: Optional[str] = "id",
+    doc_feature: Optional[str] = "text_chunk",
+    where: Optional[str] = None,
+    where_document: Optional[str] = None,
+    format_output: Optional[str] = "record",
+) -> List[Dict[str, Any]]:
     parsed_uri = CDPUri.from_uri(uri)
     client = get_client_for_uri(parsed_uri)
     _collection = parsed_uri.collection or collection
     _batch_size = parsed_uri.batch_size or batch_size
     _offset = parsed_uri.offset or offset
     _limit = parsed_uri.limit or limit
     _start = _offset if _offset > 0 else 0
@@ -119,17 +94,14 @@
     total_results_to_fetch = min(col_count, _limit) if _limit > 0 else col_count
     _where = None
     if where:
         _where = validate_where(json.loads(where))
     _where_document = None
     if where_document:
         _where_document = validate_where_document(json.loads(where_document))
-    if export_file and not append:
-        with open(export_file, "w") as f:
-            f.write("")
     for offset in range(_start, total_results_to_fetch, _batch_size):
         _results = _get_result_to_chroma_doc_list(
             read_large_data_in_chunks(
                 chroma_collection,
                 offset=offset,
                 limit=min(total_results_to_fetch - offset, _batch_size),
                 where=_where,
@@ -147,14 +119,75 @@
                     id_feature=id_feature,
                     meta_features=meta_features,
                 )
                 for doc in _results
             ]
         else:
             raise ValueError(f"Unsupported format: {format}")
-        if export_file:
-            with open(export_file, "a") as f:
-                for _doc in _final_results:
-                    f.write(str(json.dumps(_doc)) + "\n")
-        else:
+        return _final_results
+
+
+def chroma_export_cli(
+    uri: Annotated[str, typer.Argument(help="The Chroma endpoint.")],
+    collection: Annotated[
+        Optional[str], typer.Option(help="The Chroma collection.")
+    ] = None,
+    export_file: Optional[str] = typer.Option(
+        None, "--out", help="Export .jsonl file."
+    ),
+    append: Annotated[bool, typer.Option(help="Append to export file.")] = False,
+    limit: Annotated[int, typer.Option(help="The limit.")] = -1,
+    offset: Annotated[int, typer.Option(help="The offset.")] = 0,
+    batch_size: Annotated[int, typer.Option(help="The batch size.")] = 100,
+    embed_feature: Annotated[
+        str, typer.Option(help="The embedding feature.")
+    ] = "embedding",
+    meta_features: Optional[List[str]] = typer.Option(
+        None, help="The metadata features."
+    ),
+    id_feature: Annotated[str, typer.Option(help="The id feature.")] = "id",
+    doc_feature: Annotated[
+        str, typer.Option(help="The document feature.")
+    ] = "text_chunk",
+    where: Optional[str] = typer.Option(
+        None,
+        "--where",
+        "-m",
+        help='Metadata filter. JSON with Chroma syntax is expected - \'{"metadata_key": "metadata_value"}\'',
+    ),
+    where_document: Optional[str] = typer.Option(
+        None,
+        "--where-document",
+        "-d",
+        help='Document filter string - JSON with Chroma syntax is expected - \'{"$contains": "search for this"}\'',
+    ),
+    format_output: Optional[str] = typer.Option(
+        "record",
+        "--format",
+        help="Export format. Default is `record`. Supported formats: `record` and `jsonl`. ",
+    ),
+) -> None:
+    if export_file and not append:
+        with open(export_file, "w") as f:
+            f.write("")
+    _final_results = chroma_export(
+        uri=uri,
+        collection=collection,
+        limit=limit,
+        offset=offset,
+        batch_size=batch_size,
+        embed_feature=embed_feature,
+        meta_features=meta_features,
+        id_feature=id_feature,
+        doc_feature=doc_feature,
+        where=where,
+        where_document=where_document,
+        format_output=format_output,
+    )
+
+    if export_file:
+        with open(export_file, "a") as f:
             for _doc in _final_results:
-                typer.echo(json.dumps(_doc))
+                f.write(str(json.dumps(_doc)) + "\n")
+    else:
+        for _doc in _final_results:
+            typer.echo(json.dumps(_doc))
```

### Comparing `chromadb_data_pipes-0.0.8/chroma_dp/chroma/chroma_import.py` & `chromadb_data_pipes-0.0.9/chroma_dp/chroma/chroma_import.py`

 * *Files identical despite different names*

### Comparing `chromadb_data_pipes-0.0.8/chroma_dp/huggingface/__init__.py` & `chromadb_data_pipes-0.0.9/chroma_dp/huggingface/__init__.py`

 * *Files identical despite different names*

### Comparing `chromadb_data_pipes-0.0.8/chroma_dp/huggingface/utils.py` & `chromadb_data_pipes-0.0.9/chroma_dp/huggingface/utils.py`

 * *Files identical despite different names*

### Comparing `chromadb_data_pipes-0.0.8/chroma_dp/main.py` & `chromadb_data_pipes-0.0.9/chroma_dp/main.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 import typer
 from dotenv import load_dotenv
-from chroma_dp.chroma.chroma_export import chroma_export
+from chroma_dp.chroma.chroma_export import chroma_export_cli
 from chroma_dp.chroma.chroma_import import chroma_import
 from chroma_dp.processor.chunk import chunk_process
 from chroma_dp.processor.embed import filter_embed
 from chroma_dp.huggingface import hf_import, hf_export
 from chroma_dp.processor.id import id_process
 from chroma_dp.processor.metadata import meta_process
 from chroma_dp.processor.misc.emoji_clean import emoji_clean
@@ -68,46 +68,46 @@
 )(filter_embed)
 
 # Chroma commands
 app.command(
     name="export",
     help="Export data from ChromaDB.",
     no_args_is_help=True,
-)(chroma_export)
+)(chroma_export_cli)
 
 app.command(
     name="import",
     help="Import data into ChromaDB.",
     no_args_is_help=True,
 )(chroma_import)
 
-## Dataset commands
+# Dataset commands
 
 
 app.command(
     name="ds-get",
     help="Gets a dataset from HF.",
     no_args_is_help=True,
 )(hf_import)
 
 app.command(
     name="ds-put",
     help="Upload a dataset to HF.",
     no_args_is_help=True,
 )(hf_export)
 
-## Metadata processor
+# Metadata processor
 
 app.command(
     name="meta",
     help="Add or remove metadata.",
     no_args_is_help=True,
 )(meta_process)
 
-## ID processor
+# ID processor
 
 
 app.command(
     name="id",
     help="Generate IDs for resources given a strategy.",
     no_args_is_help=True,
 )(id_process)
```

### Comparing `chromadb_data_pipes-0.0.8/chroma_dp/processor/chunk.py` & `chromadb_data_pipes-0.0.9/chroma_dp/processor/chunk.py`

 * *Files identical despite different names*

### Comparing `chromadb_data_pipes-0.0.8/chroma_dp/processor/embed.py` & `chromadb_data_pipes-0.0.9/chroma_dp/processor/embed.py`

 * *Files identical despite different names*

### Comparing `chromadb_data_pipes-0.0.8/chroma_dp/processor/id.py` & `chromadb_data_pipes-0.0.9/chroma_dp/processor/id.py`

 * *Files identical despite different names*

### Comparing `chromadb_data_pipes-0.0.8/chroma_dp/processor/langchain_utils.py` & `chromadb_data_pipes-0.0.9/chroma_dp/processor/langchain_utils.py`

 * *Files identical despite different names*

### Comparing `chromadb_data_pipes-0.0.8/chroma_dp/processor/metadata.py` & `chromadb_data_pipes-0.0.9/chroma_dp/processor/metadata.py`

 * *Files identical despite different names*

### Comparing `chromadb_data_pipes-0.0.8/chroma_dp/processor/misc/emoji_clean.py` & `chromadb_data_pipes-0.0.9/chroma_dp/processor/misc/emoji_clean.py`

 * *Files identical despite different names*

### Comparing `chromadb_data_pipes-0.0.8/chroma_dp/producer/file/csv.py` & `chromadb_data_pipes-0.0.9/chroma_dp/producer/file/csv.py`

 * *Files identical despite different names*

### Comparing `chromadb_data_pipes-0.0.8/chroma_dp/producer/file/pdf.py` & `chromadb_data_pipes-0.0.9/chroma_dp/producer/file/pdf.py`

 * *Files identical despite different names*

### Comparing `chromadb_data_pipes-0.0.8/chroma_dp/producer/file/text.py` & `chromadb_data_pipes-0.0.9/chroma_dp/producer/file/text.py`

 * *Files identical despite different names*

### Comparing `chromadb_data_pipes-0.0.8/chroma_dp/producer/url/url_loader.py` & `chromadb_data_pipes-0.0.9/chroma_dp/producer/url/url_loader.py`

 * *Files identical despite different names*

### Comparing `chromadb_data_pipes-0.0.8/chroma_dp/utils/chroma.py` & `chromadb_data_pipes-0.0.9/chroma_dp/utils/chroma.py`

 * *Files identical despite different names*

### Comparing `chromadb_data_pipes-0.0.8/chroma_dp/utils/embedding.py` & `chromadb_data_pipes-0.0.9/chroma_dp/utils/embedding.py`

 * *Files identical despite different names*

### Comparing `chromadb_data_pipes-0.0.8/chroma_dp/utils/templating.py` & `chromadb_data_pipes-0.0.9/chroma_dp/utils/templating.py`

 * *Files identical despite different names*

### Comparing `chromadb_data_pipes-0.0.8/pyproject.toml` & `chromadb_data_pipes-0.0.9/pyproject.toml`

 * *Files 6% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "chromadb-data-pipes"
-version = "0.0.8"
+version = "0.0.9"
 description = "ChromaDB Data Pipes 🖇️ - The easiest way to get data into and out of ChromaDB"
 authors = ["Trayan Azarov <trayan.azarov@amikos.tech>"]
 license = "MIT"
 readme = "README.md"
 packages = [{ include = "chroma_dp" }]
 [tool.poetry.urls]
 "Bug Tracker" = "https://github.com/amikos-tech/chromadb-data-pipes/issues"
@@ -19,25 +19,25 @@
 chromadb = "0.4.24"
 datasets = "^2.15.0"
 tqdm = "^4.66.1"
 rich = "^13.7.0"
 typer = { extras = ["all"], version = "^0.9.0" }
 pydantic = "^2.5.3"
 tenacity = "^8.2.3"
-fastapi = "^0.108.0"
+fastapi = ">=0.108,<0.110"
 langchain = "^0.1.0"
 pypdf = "^3.17.4"
 py-ulid = "^1.0.3"
 python-dotenv = "^1.0.1"
 orjson = "^3.9.12"
 
 
 [tool.poetry.group.dev.dependencies]
 pytest = "^7.4.3"
-black = "23.3.0"
+black = "24.3.0"
 pre-commit = "^3.6.0"
 hypothesis = "^6.92.0"
 
 [tool.poetry.group.docs.dependencies]
 pypdf = "^3.17.4"
 unstructured = "^0.12.0"
```

### Comparing `chromadb_data_pipes-0.0.8/PKG-INFO` & `chromadb_data_pipes-0.0.9/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,23 +1,23 @@
 Metadata-Version: 2.1
 Name: chromadb-data-pipes
-Version: 0.0.8
+Version: 0.0.9
 Summary: ChromaDB Data Pipes 🖇️ - The easiest way to get data into and out of ChromaDB
 License: MIT
 Author: Trayan Azarov
 Author-email: trayan.azarov@amikos.tech
 Requires-Python: >=3.9,<3.12
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Requires-Dist: chromadb (==0.4.24)
 Requires-Dist: datasets (>=2.15.0,<3.0.0)
-Requires-Dist: fastapi (>=0.108.0,<0.109.0)
+Requires-Dist: fastapi (>=0.108,<0.110)
 Requires-Dist: langchain (>=0.1.0,<0.2.0)
 Requires-Dist: orjson (>=3.9.12,<4.0.0)
 Requires-Dist: py-ulid (>=1.0.3,<2.0.0)
 Requires-Dist: pydantic (>=2.5.3,<3.0.0)
 Requires-Dist: pypdf (>=3.17.4,<4.0.0)
 Requires-Dist: python-dotenv (>=1.0.1,<2.0.0)
 Requires-Dist: rich (>=13.7.0,<14.0.0)
```

