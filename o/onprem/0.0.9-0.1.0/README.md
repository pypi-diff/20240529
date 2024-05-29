# Comparing `tmp/onprem-0.0.9.tar.gz` & `tmp/onprem-0.1.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "onprem-0.0.9.tar", last modified: Wed Sep  6 18:11:45 2023, max compression
+gzip compressed data, was "onprem-0.1.0.tar", last modified: Wed May 29 16:25:41 2024, max compression
```

## Comparing `onprem-0.0.9.tar` & `onprem-0.1.0.tar`

### file list

```diff
@@ -1,22 +1,31 @@
-drwxrwxr-x   0 amaiya    (1001) amaiya    (1001)        0 2023-09-06 18:11:45.093912 onprem-0.0.9/
--rw-rw-r--   0 amaiya    (1001) amaiya    (1001)    11344 2023-09-01 22:09:40.000000 onprem-0.0.9/LICENSE
--rw-rw-r--   0 amaiya    (1001) amaiya    (1001)      111 2023-08-31 21:00:21.000000 onprem-0.0.9/MANIFEST.in
--rw-rw-r--   0 amaiya    (1001) amaiya    (1001)     9737 2023-09-06 18:11:45.093912 onprem-0.0.9/PKG-INFO
--rw-rw-r--   0 amaiya    (1001) amaiya    (1001)     8937 2023-09-06 16:43:21.000000 onprem-0.0.9/README.md
-drwxrwxr-x   0 amaiya    (1001) amaiya    (1001)        0 2023-09-06 18:11:45.093912 onprem-0.0.9/onprem/
--rw-rw-r--   0 amaiya    (1001) amaiya    (1001)       45 2023-09-06 16:42:31.000000 onprem-0.0.9/onprem/__init__.py
--rw-rw-r--   0 amaiya    (1001) amaiya    (1001)     2573 2023-09-06 16:42:31.000000 onprem-0.0.9/onprem/_modidx.py
--rw-rw-r--   0 amaiya    (1001) amaiya    (1001)     7554 2023-09-06 16:42:31.000000 onprem-0.0.9/onprem/core.py
--rw-rw-r--   0 amaiya    (1001) amaiya    (1001)     8120 2023-09-06 16:42:31.000000 onprem-0.0.9/onprem/ingest.py
--rw-rw-r--   0 amaiya    (1001) amaiya    (1001)     1104 2023-09-06 16:42:31.000000 onprem-0.0.9/onprem/utils.py
-drwxrwxr-x   0 amaiya    (1001) amaiya    (1001)        0 2023-09-06 18:11:45.093912 onprem-0.0.9/onprem.egg-info/
--rw-rw-r--   0 amaiya    (1001) amaiya    (1001)     9737 2023-09-06 18:11:45.000000 onprem-0.0.9/onprem.egg-info/PKG-INFO
--rw-rw-r--   0 amaiya    (1001) amaiya    (1001)      347 2023-09-06 18:11:45.000000 onprem-0.0.9/onprem.egg-info/SOURCES.txt
--rw-rw-r--   0 amaiya    (1001) amaiya    (1001)        1 2023-09-06 18:11:45.000000 onprem-0.0.9/onprem.egg-info/dependency_links.txt
--rw-rw-r--   0 amaiya    (1001) amaiya    (1001)       34 2023-09-06 18:11:45.000000 onprem-0.0.9/onprem.egg-info/entry_points.txt
--rw-rw-r--   0 amaiya    (1001) amaiya    (1001)        1 2023-08-31 21:02:33.000000 onprem-0.0.9/onprem.egg-info/not-zip-safe
--rw-rw-r--   0 amaiya    (1001) amaiya    (1001)      218 2023-09-06 18:11:45.000000 onprem-0.0.9/onprem.egg-info/requires.txt
--rw-rw-r--   0 amaiya    (1001) amaiya    (1001)        7 2023-09-06 18:11:45.000000 onprem-0.0.9/onprem.egg-info/top_level.txt
--rw-rw-r--   0 amaiya    (1001) amaiya    (1001)     1177 2023-09-05 19:18:53.000000 onprem-0.0.9/settings.ini
--rw-rw-r--   0 amaiya    (1001) amaiya    (1001)       38 2023-09-06 18:11:45.093912 onprem-0.0.9/setup.cfg
--rw-rw-r--   0 amaiya    (1001) amaiya    (1001)     2596 2023-08-31 21:00:21.000000 onprem-0.0.9/setup.py
+drwxrwxr-x   0 amaiya    (1001) amaiya    (1001)        0 2024-05-29 16:25:41.790322 onprem-0.1.0/
+-rw-rw-r--   0 amaiya    (1001) amaiya    (1001)     1457 2024-04-04 02:53:11.000000 onprem-0.1.0/CONTRIBUTING.md
+-rw-rw-r--   0 amaiya    (1001) amaiya    (1001)    11344 2023-09-01 22:09:40.000000 onprem-0.1.0/LICENSE
+-rw-rw-r--   0 amaiya    (1001) amaiya    (1001)      111 2023-08-31 21:00:21.000000 onprem-0.1.0/MANIFEST.in
+-rw-r--r--   0 amaiya    (1001) amaiya    (1001)    32423 2024-05-29 16:25:41.790322 onprem-0.1.0/PKG-INFO
+-rw-rw-r--   0 amaiya    (1001) amaiya    (1001)    31081 2024-05-29 15:35:32.000000 onprem-0.1.0/README.md
+drwxrwxr-x   0 amaiya    (1001) amaiya    (1001)        0 2024-05-29 16:25:41.774322 onprem-0.1.0/onprem/
+-rw-rw-r--   0 amaiya    (1001) amaiya    (1001)      837 2024-05-29 16:17:57.000000 onprem-0.1.0/onprem/__init__.py
+-rw-rw-r--   0 amaiya    (1001) amaiya    (1001)    11387 2024-05-29 16:17:57.000000 onprem-0.1.0/onprem/_modidx.py
+-rw-rw-r--   0 amaiya    (1001) amaiya    (1001)     1370 2024-04-04 02:53:12.000000 onprem-0.1.0/onprem/console.py
+-rw-rw-r--   0 amaiya    (1001) amaiya    (1001)    20212 2024-05-29 16:17:57.000000 onprem-0.1.0/onprem/core.py
+-rw-rw-r--   0 amaiya    (1001) amaiya    (1001)     1582 2024-05-29 16:17:57.000000 onprem-0.1.0/onprem/guider.py
+-rw-rw-r--   0 amaiya    (1001) amaiya    (1001)    12574 2024-05-29 16:17:57.000000 onprem-0.1.0/onprem/ingest.py
+drwxrwxr-x   0 amaiya    (1001) amaiya    (1001)        0 2024-05-29 16:25:41.790322 onprem-0.1.0/onprem/pipelines/
+-rw-rw-r--   0 amaiya    (1001) amaiya    (1001)      158 2024-05-29 16:17:57.000000 onprem-0.1.0/onprem/pipelines/__init__.py
+-rw-rw-r--   0 amaiya    (1001) amaiya    (1001)     8613 2024-05-29 16:17:57.000000 onprem-0.1.0/onprem/pipelines/classifier.py
+-rw-rw-r--   0 amaiya    (1001) amaiya    (1001)     4261 2024-05-29 16:17:57.000000 onprem-0.1.0/onprem/pipelines/extractor.py
+-rw-rw-r--   0 amaiya    (1001) amaiya    (1001)    10323 2024-05-29 16:17:57.000000 onprem-0.1.0/onprem/pipelines/summarizer.py
+-rw-rw-r--   0 amaiya    (1001) amaiya    (1001)     2139 2024-05-29 16:17:57.000000 onprem-0.1.0/onprem/utils.py
+-rw-rw-r--   0 amaiya    (1001) amaiya    (1001)    10946 2024-04-04 02:53:12.000000 onprem-0.1.0/onprem/webapp.py
+drwxrwxr-x   0 amaiya    (1001) amaiya    (1001)        0 2024-05-29 16:25:41.786322 onprem-0.1.0/onprem.egg-info/
+-rw-r--r--   0 amaiya    (1001) amaiya    (1001)    32423 2024-05-29 16:25:41.000000 onprem-0.1.0/onprem.egg-info/PKG-INFO
+-rw-rw-r--   0 amaiya    (1001) amaiya    (1001)      536 2024-05-29 16:25:41.000000 onprem-0.1.0/onprem.egg-info/SOURCES.txt
+-rw-rw-r--   0 amaiya    (1001) amaiya    (1001)        1 2024-05-29 16:25:41.000000 onprem-0.1.0/onprem.egg-info/dependency_links.txt
+-rw-rw-r--   0 amaiya    (1001) amaiya    (1001)       81 2024-05-29 16:25:41.000000 onprem-0.1.0/onprem.egg-info/entry_points.txt
+-rw-rw-r--   0 amaiya    (1001) amaiya    (1001)        1 2023-08-31 21:02:33.000000 onprem-0.1.0/onprem.egg-info/not-zip-safe
+-rw-rw-r--   0 amaiya    (1001) amaiya    (1001)      269 2024-05-29 16:25:41.000000 onprem-0.1.0/onprem.egg-info/requires.txt
+-rw-rw-r--   0 amaiya    (1001) amaiya    (1001)        7 2024-05-29 16:25:41.000000 onprem-0.1.0/onprem.egg-info/top_level.txt
+-rw-rw-r--   0 amaiya    (1001) amaiya    (1001)     1478 2024-05-29 16:00:40.000000 onprem-0.1.0/settings.ini
+-rw-rw-r--   0 amaiya    (1001) amaiya    (1001)       38 2024-05-29 16:25:41.790322 onprem-0.1.0/setup.cfg
+-rw-rw-r--   0 amaiya    (1001) amaiya    (1001)     2596 2023-08-31 21:00:21.000000 onprem-0.1.0/setup.py
```

### Comparing `onprem-0.0.9/LICENSE` & `onprem-0.1.0/LICENSE`

 * *Files identical despite different names*

### Comparing `onprem-0.0.9/onprem/ingest.py` & `onprem-0.1.0/onprem/ingest.py`

 * *Files 27% similar despite different names*

```diff
@@ -1,72 +1,81 @@
 # AUTOGENERATED! DO NOT EDIT! File to edit: ../nbs/01_ingest.ipynb.
 
 # %% auto 0
-__all__ = ['chunk_size', 'chunk_overlap', 'LOADER_MAPPING', 'DEFAULT_DB', 'MyElmLoader', 'load_single_document', 'load_documents',
-           'process_documents', 'does_vectorstore_exist', 'Ingester']
+__all__ = ['logger', 'DEFAULT_CHUNK_SIZE', 'DEFAULT_CHUNK_OVERLAP', 'COLLECTION_NAME', 'CHROMA_MAX', 'LOADER_MAPPING',
+           'DEFAULT_DB', 'MyElmLoader', 'load_single_document', 'load_documents', 'process_documents',
+           'does_vectorstore_exist', 'batchify_chunks', 'Ingester']
 
 # %% ../nbs/01_ingest.ipynb 3
 import os
 import os.path
 import glob
-from typing import List
+from typing import Any, Dict, Generator, List, Optional, Tuple, Union, Callable
 from dotenv import load_dotenv
 from multiprocessing import Pool
 from tqdm import tqdm
 
-from langchain.document_loaders import (
+from langchain.text_splitter import RecursiveCharacterTextSplitter
+from langchain.docstore.document import Document
+from langchain_community.document_loaders import (
     CSVLoader,
     EverNoteLoader,
     PyMuPDFLoader,
     TextLoader,
     UnstructuredEmailLoader,
     UnstructuredEPubLoader,
     UnstructuredHTMLLoader,
     UnstructuredMarkdownLoader,
     UnstructuredODTLoader,
     UnstructuredPowerPointLoader,
     UnstructuredWordDocumentLoader,
 )
-
-from langchain.text_splitter import RecursiveCharacterTextSplitter
-from langchain.vectorstores import Chroma
-from langchain.embeddings import HuggingFaceEmbeddings
-from langchain.docstore.document import Document
+from langchain_community.vectorstores import Chroma
+from langchain_community.embeddings import HuggingFaceEmbeddings
 import chromadb
 from chromadb.config import Settings
-chunk_size = 500
-chunk_overlap = 50
+from . import utils as U
+
+import logging
+import sys
+
+logging.basicConfig(stream=sys.stdout, level=logging.WARNING)
+logger = logging.getLogger('OnPrem.LLM-ingest')
+
+DEFAULT_CHUNK_SIZE = 500
+DEFAULT_CHUNK_OVERLAP = 50
+COLLECTION_NAME = "onprem_chroma"
+CHROMA_MAX = 41000
 
 # %% ../nbs/01_ingest.ipynb 4
 class MyElmLoader(UnstructuredEmailLoader):
     """Wrapper to fallback to text/plain when default does not work"""
 
     def load(self) -> List[Document]:
         """Wrapper adding fallback for elm without html"""
         try:
             try:
                 doc = UnstructuredEmailLoader.load(self)
             except ValueError as e:
-                if 'text/html content not found in email' in str(e):
+                if "text/html content not found in email" in str(e):
                     # Try plain text
-                    self.unstructured_kwargs["content_source"]="text/plain"
+                    self.unstructured_kwargs["content_source"] = "text/plain"
                     doc = UnstructuredEmailLoader.load(self)
                 else:
                     raise
         except Exception as e:
             # Add file_path to exception message
             raise type(e)(f"{self.file_path}: {e}") from e
 
         return doc
 
 # %% ../nbs/01_ingest.ipynb 5
 # Map file extensions to document loaders and their arguments
 LOADER_MAPPING = {
     ".csv": (CSVLoader, {}),
-    # ".docx": (Docx2txtLoader, {}),
     ".doc": (UnstructuredWordDocumentLoader, {}),
     ".docx": (UnstructuredWordDocumentLoader, {}),
     ".enex": (EverNoteLoader, {}),
     ".eml": (MyElmLoader, {}),
     ".epub": (UnstructuredEPubLoader, {}),
     ".html": (UnstructuredHTMLLoader, {}),
     ".md": (UnstructuredMarkdownLoader, {}),
@@ -76,139 +85,260 @@
     ".pptx": (UnstructuredPowerPointLoader, {}),
     ".txt": (TextLoader, {"encoding": "utf8"}),
     # Add more mappings for other file extensions and loaders as needed
 }
 
 
 def load_single_document(file_path: str) -> List[Document]:
+    """
+    Load a single document (invoked by `load_documents`).
+    """
     ext = "." + file_path.rsplit(".", 1)[-1].lower()
     if ext in LOADER_MAPPING:
-        loader_class, loader_args = LOADER_MAPPING[ext]
-        loader = loader_class(file_path, **loader_args)
-        return loader.load()
+        try:
+            loader_class, loader_args = LOADER_MAPPING[ext]
+            loader = loader_class(file_path, **loader_args)
+            return loader.load()
+        except Exception as e:
+            logger.warning(f'Skipping {file_path} due to error: {str(e)}')
+    else:
+        logger.warning(f"Skipping {file_path} due to unsupported file extension: '{ext}'")
 
-    raise ValueError(f"Unsupported file extension '{ext}'")
 
-def load_documents(source_dir: str, ignored_files: List[str] = []) -> List[Document]:
+def load_documents(source_dir: str, ignored_files: List[str] = [], ignore_fn:Optional[Callable] = None
+) -> List[Document]:
     """
     Loads all documents from the source documents directory, ignoring specified files
     """
+    source_dir = os.path.abspath(source_dir)
     all_files = []
     for ext in LOADER_MAPPING:
         all_files.extend(
             glob.glob(os.path.join(source_dir, f"**/*{ext.lower()}"), recursive=True)
         )
         all_files.extend(
             glob.glob(os.path.join(source_dir, f"**/*{ext.upper()}"), recursive=True)
         )
-    filtered_files = [file_path for file_path in all_files if file_path not in ignored_files]
+
+    filtered_files = [
+        file_path for file_path in all_files if file_path not in ignored_files and not os.path.basename(file_path).startswith('~$')
+         and (ignore_fn is None or not ignore_fn(file_path))
+    ]
 
     with Pool(processes=os.cpu_count()) as pool:
         results = []
-        with tqdm(total=len(filtered_files), desc='Loading new documents', ncols=80) as pbar:
-            for i, docs in enumerate(pool.imap_unordered(load_single_document, filtered_files)):
-                results.extend(docs)
+        with tqdm(
+            total=len(filtered_files), desc="Loading new documents", ncols=80
+        ) as pbar:
+            for i, docs in enumerate(
+                pool.imap_unordered(load_single_document, filtered_files)
+            ):
+                if docs is not None: results.extend(docs)
                 pbar.update()
 
     return results
 
-def process_documents(source_directory:str, ignored_files: List[str] = [], ) -> List[Document]:
+
+def process_documents(
+    source_directory: str,
+    ignored_files: List[str] = [],
+    chunk_size: int = DEFAULT_CHUNK_SIZE,
+    chunk_overlap: int = DEFAULT_CHUNK_OVERLAP,
+    ignore_fn:Optional[Callable] = None
+
+
+) -> List[Document]:
     """
     Load documents and split in chunks
+
+    **Args**:
+
+      - *source_directory*: path to folder containing document store
+      - *chunk_size*: text is split to this many characters by `langchain.text_splitter.RecursiveCharacterTextSplitter`
+      - *chunk_overlap*: character overlap between chunks in `langchain.text_splitter.RecursiveCharacterTextSplitter`
+      - *ignore_fn*: Optional function that accepts the file path (including file name) as input and returns True
+                     if file path should not be ingested.
+
+    **Returns:** list of `langchain.docstore.document.Document` objects
+
     """
     print(f"Loading documents from {source_directory}")
-    documents = load_documents(source_directory, ignored_files)
+    documents = load_documents(source_directory, ignored_files, ignore_fn=ignore_fn)
     if not documents:
         print("No new documents to load")
         return
     print(f"Loaded {len(documents)} new documents from {source_directory}")
-    text_splitter = RecursiveCharacterTextSplitter(chunk_size=chunk_size, chunk_overlap=chunk_overlap)
+    text_splitter = RecursiveCharacterTextSplitter(
+        chunk_size=chunk_size, chunk_overlap=chunk_overlap
+    )
     texts = text_splitter.split_documents(documents)
-    print(f"Split into {len(texts)} chunks of text (max. {chunk_size} tokens each)")
+    print(f"Split into {len(texts)} chunks of text (max. {chunk_size} chars each)")
     return texts
 
-def does_vectorstore_exist(persist_directory: str, embeddings: HuggingFaceEmbeddings) -> bool:
+
+def does_vectorstore_exist(db) -> bool:
     """
     Checks if vectorstore exists
     """
-    db = Chroma(persist_directory=persist_directory, embedding_function=embeddings)
-    if not db.get()['documents']:
+    if not db.get()["documents"]:
         return False
     return True
 
+
+def batchify_chunks(texts):
+    split_docs_chunked = U.split_list(texts, CHROMA_MAX)
+    total_chunks = sum(1 for _ in U.split_list(texts, CHROMA_MAX))
+    return split_docs_chunked, total_chunks
+
+
 # %% ../nbs/01_ingest.ipynb 6
-from typing import Any, Dict, Generator, List, Optional, Tuple, Union
 from .utils import get_datadir
-os.environ['TOKENIZERS_PARALLELISM'] = '0'
-DEFAULT_DB = 'vectordb'
+
+os.environ["TOKENIZERS_PARALLELISM"] = "0"
+DEFAULT_DB = "vectordb"
+
 
 class Ingester:
-    def __init__(self,
-                 embedding_model_name:str ='sentence-transformers/all-MiniLM-L6-v2',
-                 embedding_model_kwargs:dict ={'device': 'cpu'}
-                ):
+    def __init__(
+        self,
+        embedding_model_name: str = "sentence-transformers/all-MiniLM-L6-v2",
+        embedding_model_kwargs: dict = {"device": "cpu"},
+        embedding_encode_kwargs: dict = {"normalize_embeddings": False},
+        persist_directory: Optional[str] = None,
+    ):
         """
         Ingests all documents in `source_folder` (previously-ingested documents are ignored)
 
         **Args**:
-        
+
           - *embedding_model*: name of sentence-transformers model
           - *embedding_model_kwargs*: arguments to embedding model (e.g., `{device':'cpu'}`)
+          - *embedding_encode_kwargs*: arguments to encode method of
+                                       embedding model (e.g., `{'normalize_embeddings': False}`).
+          - *persist_directory*: Path to vector database (created if it doesn't exist).
+                                 Default is `onprem_data/vectordb` in user's home directory.
+
 
         **Returns**: `None`
         """
-        self.persist_directory = os.path.join(get_datadir(), DEFAULT_DB)
-        self.embeddings = HuggingFaceEmbeddings(model_name=embedding_model_name)
-        self.chroma_settings = Settings(persist_directory=self.persist_directory,anonymized_telemetry=False)
-        self.chroma_client = chromadb.PersistentClient(settings=self.chroma_settings , path=self.persist_directory)
+        self.persist_directory = persist_directory or os.path.join(
+            get_datadir(), DEFAULT_DB
+        )
+        self.embeddings = HuggingFaceEmbeddings(
+            model_name=embedding_model_name,
+            model_kwargs=embedding_model_kwargs,
+            encode_kwargs=embedding_encode_kwargs,
+        )
+        self.chroma_settings = Settings(
+            persist_directory=self.persist_directory, anonymized_telemetry=False
+        )
+        self.chroma_client = chromadb.PersistentClient(
+            settings=self.chroma_settings, path=self.persist_directory
+        )
         return
-     
-    
+
     def get_db(self):
-        db = None
-        if does_vectorstore_exist(self.persist_directory, self.embeddings):
-            db = Chroma(persist_directory=self.persist_directory, 
-                        embedding_function=self.embeddings, 
-                        client_settings=self.chroma_settings, client=self.chroma_client)
-        return db
-            
-    
-    def ingest(self,
-               source_directory:str, 
-              ):
         """
-        Ingests all documents in `source_folder` (previously-ingested documents are ignored)
+        Returns an instance to the `langchain.vectorstores.Chroma` instance
+        """
+        db = Chroma(
+            persist_directory=self.persist_directory,
+            embedding_function=self.embeddings,
+            client_settings=self.chroma_settings,
+            client=self.chroma_client,
+            collection_metadata={"hnsw:space": "cosine"},
+            collection_name=COLLECTION_NAME,
+        )
+        return db if does_vectorstore_exist(db) else None
+
+    def get_embedding_model(self):
+        """
+        Returns an instance to the `langchain.embeddings.huggingface.HuggingFaceEmbeddings` instance
+        """
+        return self.embeddings
+
+
+    def get_ingested_files(self):
+        """
+        Returns a list of files previously added to vector database (typically via `LLM.ingest`)
+        """
+        return set([d['source'] for d in self.get_db().get()['metadatas']])
+
+
+    def ingest(
+        self,
+        source_directory: str,
+        chunk_size: int = DEFAULT_CHUNK_SIZE,
+        chunk_overlap: int = DEFAULT_CHUNK_OVERLAP,
+        ignore_fn:Optional[Callable] = None
+    ):
+        """
+        Ingests all documents in `source_directory` (previously-ingested documents are ignored).
 
         **Args**:
 
           - *source_directory*: path to folder containing document store
+          - *chunk_size*: text is split to this many characters by `langchain.text_splitter.RecursiveCharacterTextSplitter`
+          - *chunk_overlap*: character overlap between chunks in `langchain.text_splitter.RecursiveCharacterTextSplitter`
+          - *ignore_fn*: Optional function that accepts the file path (including file name) as input and returns True
+                         if file path should not be ingested.
+
 
         **Returns**: `None`
         """
 
         if not os.path.exists(source_directory):
-            raise ValueError('The source_directory does not exist.')
+            raise ValueError("The source_directory does not exist.")
+        elif os.path.isfile(source_directory):
+            raise ValueError(
+                "The source_directory argument must be a folder, not a file."
+            )
         texts = None
         db = self.get_db()
         if db:
             # Update and store locally vectorstore
             print(f"Appending to existing vectorstore at {self.persist_directory}")
             collection = db.get()
-            texts = process_documents(source_directory, 
-                                      ignored_files=[metadata['source'] for metadata in collection['metadatas']])
+            texts = process_documents(
+                source_directory,
+                ignored_files=[
+                    metadata["source"] for metadata in collection["metadatas"]],
+                ignore_fn=ignore_fn
+
+            )
             if texts:
                 print(f"Creating embeddings. May take some minutes...")
-                db.add_documents(texts)
+                chunk_batches, total_chunks = batchify_chunks(texts)
+                for lst in tqdm(chunk_batches, total=total_chunks):
+                    db.add_documents(lst)
         else:
             # Create and store locally vectorstore
-            print("Creating new vectorstore")
-            texts = process_documents(source_directory)
+            print(f"Creating new vectorstore at {self.persist_directory}")
+            texts = process_documents(
+                source_directory, chunk_size=chunk_size, chunk_overlap=chunk_overlap, ignore_fn=ignore_fn
+            )
+
             if texts:
+                chunk_batches, total_chunks = batchify_chunks(texts)
                 print(f"Creating embeddings. May take some minutes...")
-                db = Chroma.from_documents(texts, 
-                                           self.embeddings, persist_directory=self.persist_directory, 
-                                           client_settings=self.chroma_settings, client=self.chroma_client)
+                db = None
+
+                for lst in tqdm(chunk_batches, total=total_chunks):
+                    if not db:
+                        db = Chroma.from_documents(
+                            lst,
+                            self.embeddings,
+                            persist_directory=self.persist_directory,
+                            client_settings=self.chroma_settings,
+                            client=self.chroma_client,
+                            collection_metadata={"hnsw:space": "cosine"},
+                            collection_name=COLLECTION_NAME,
+                        )
+                    else:
+                        db.add_documents(lst)
         if texts:
             db.persist()
-            print(f"Ingestion complete! You can now query your documents using the LLM.ask method")
+            print(
+                f"Ingestion complete! You can now query your documents using the LLM.ask or LLM.chat methods"
+            )
         db = None
         return
```

### Comparing `onprem-0.0.9/settings.ini` & `onprem-0.1.0/settings.ini`

 * *Files 27% similar despite different names*

```diff
@@ -1,30 +1,30 @@
 [DEFAULT]
 # All sections below are required unless otherwise specified.
 # See https://github.com/fastai/nbdev/blob/master/settings.ini for examples.
 
 ### Python library ###
 repo = onprem
 lib_name = %(repo)s
-version = 0.0.9
-min_python = 3.7
+version = 0.1.0
+min_python = 3.8
 license = apache2
 black_formatting = False
 
 ### nbdev ###
 doc_path = _docs
 lib_path = onprem
 nbs_path = nbs
 recursive = True
 tst_flags = notest
 put_version_in_init = True
 
 ### Docs ###
 branch = master
-custom_sidebar = False
+custom_sidebar = True
 doc_host = https://%(user)s.github.io
 doc_baseurl = /%(repo)s
 git_url = https://github.com/%(user)s/%(repo)s
 title = %(lib_name)s
 
 ### PyPI ###
 audience = Developers
@@ -34,10 +34,13 @@
 description = A tool for running on-premises large language models on non-public data
 keywords = nbdev jupyter notebook python
 language = English
 status = 3
 user = amaiya
 
 ### Optional ###
-requirements = requests langchain==0.0.240 chromadb==0.4.7 PyMuPDF==1.23.1 unstructured==0.10.8 extract-msg==0.45.0 tabulate==0.9.0 pandoc==2.3 pypandoc==1.11 tqdm==4.66.1 sentence_transformers==2.2.2 llama-cpp-python==0.1.69
+# Notes:
+# pinning to transformers due to bug in SetFit (https://github.com/huggingface/setfit/issues/528) - transformers dependency can be removed after SetFix upgrade
+# pinning to ChromaDB due to backwards compatibility issue
+requirements = transformers<=4.40.2 requests unstructured PyMuPDF markdown python-docx python-pptx extract-msg tabulate pandoc pypandoc tqdm syntok pandas sentence_transformers cmake setfit guidance>=0.1.5 langchain>=0.1.0 langchain-community langchain-openai chromadb==0.4.15 
 # dev_requirements = 
-# console_scripts =
+console_scripts=onprem=onprem.console:cli
```

### Comparing `onprem-0.0.9/setup.py` & `onprem-0.1.0/setup.py`

 * *Files identical despite different names*

