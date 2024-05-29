# Comparing `tmp/lazy_mongo-0.2.4.tar.gz` & `tmp/lazy_mongo-0.3.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "lazy_mongo-0.2.4.tar", max compression
+gzip compressed data, was "lazy_mongo-0.3.0.tar", max compression
```

## Comparing `lazy_mongo-0.2.4.tar` & `lazy_mongo-0.3.0.tar`

### file list

```diff
@@ -1,9 +1,9 @@
--rw-r--r--   0        0        0       40 2024-03-08 03:29:01.600206 lazy_mongo-0.2.4/README.md
--rw-r--r--   0        0        0      207 2024-03-22 03:18:21.246648 lazy_mongo-0.2.4/lazy_mongo/__init__.py
--rw-r--r--   0        0        0      265 2024-04-16 01:49:02.827730 lazy_mongo-0.2.4/lazy_mongo/insert_response.py
--rw-r--r--   0        0        0     2180 2024-04-16 01:50:16.611945 lazy_mongo-0.2.4/lazy_mongo/lazy_collection.py
--rw-r--r--   0        0        0     1818 2024-03-27 05:13:57.761621 lazy_mongo-0.2.4/lazy_mongo/lazy_database.py
--rw-r--r--   0        0        0     2456 2024-04-19 04:05:17.074776 lazy_mongo-0.2.4/lazy_mongo/lazy_mongo.py
--rw-r--r--   0        0        0      211 2024-04-16 01:49:06.275740 lazy_mongo-0.2.4/lazy_mongo/update_response.py
--rw-r--r--   0        0        0      296 2024-04-19 04:05:26.666226 lazy_mongo-0.2.4/pyproject.toml
--rw-r--r--   0        0        0      578 1970-01-01 00:00:00.000000 lazy_mongo-0.2.4/PKG-INFO
+-rw-r--r--   0        0        0       40 2024-03-08 03:29:01.600206 lazy_mongo-0.3.0/README.md
+-rw-r--r--   0        0        0      207 2024-03-22 03:18:21.246648 lazy_mongo-0.3.0/lazy_mongo/__init__.py
+-rw-r--r--   0        0        0      217 2024-05-28 06:19:06.611731 lazy_mongo-0.3.0/lazy_mongo/insert_response.py
+-rw-r--r--   0        0        0     3085 2024-05-29 03:01:18.125400 lazy_mongo-0.3.0/lazy_mongo/lazy_collection.py
+-rw-r--r--   0        0        0     2291 2024-05-28 06:17:14.155397 lazy_mongo-0.3.0/lazy_mongo/lazy_database.py
+-rw-r--r--   0        0        0     2812 2024-05-28 06:19:18.974919 lazy_mongo-0.3.0/lazy_mongo/lazy_mongo.py
+-rw-r--r--   0        0        0      211 2024-04-16 01:49:06.275740 lazy_mongo-0.3.0/lazy_mongo/update_response.py
+-rw-r--r--   0        0        0      296 2024-05-29 03:01:30.453840 lazy_mongo-0.3.0/pyproject.toml
+-rw-r--r--   0        0        0      578 1970-01-01 00:00:00.000000 lazy_mongo-0.3.0/PKG-INFO
```

### Comparing `lazy_mongo-0.2.4/lazy_mongo/lazy_collection.py` & `lazy_mongo-0.3.0/lazy_mongo/lazy_collection.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,15 +1,22 @@
-from typing import Dict, NamedTuple
+from typing import Dict, NamedTuple, TYPE_CHECKING
 from pymongo.collection import Collection
+from pymongo.typings import _Pipeline
 from pymongo.errors import DuplicateKeyError
 from .update_response import UpdateResponse
 from .insert_response import InsertResponse
 
+if TYPE_CHECKING:
+    from .lazy_database import LazyDatabase
+    from .lazy_mongo import LazyMongo
+
 
 class LazyCollection(NamedTuple):
+    mongo: LazyMongo
+    database: LazyDatabase
     collection: Collection
 
     def find_one(
         self,
         query: Dict = None,
         project: Dict = None,
     ):
@@ -25,27 +32,36 @@
     def insert_one(
         self,
         document: Dict = None,  # type: ignore
     ):
         try:
             result = self.collection.insert_one(document)
 
+            if self.mongo.log:
+                print("[Mongo.Insert]", result.inserted_id)
+
             return InsertResponse(
                 ok=True,
                 result=result,
             )
 
         except DuplicateKeyError as e:
+            if self.mongo.log:
+                print("[Mongo.Duplicate]", e)
+
             return InsertResponse(
                 ok=False,
                 is_duplicate=True,
                 error=e,
             )
 
         except Exception as e:
+            if self.mongo.log:
+                print("[Mongo.Error]", e)
+
             return InsertResponse(
                 ok=False,
                 error=e,
             )
 
     def update_set_one(
         self,
@@ -57,33 +73,51 @@
                 filter=filter,
                 update={
                     "$set": document,
                 },
                 upsert=False,
             )
 
+            if self.mongo.log:
+                print(
+                    "[Mongo.Update]",
+                    result.modified_count,
+                )
+
             return UpdateResponse(
                 ok=True,
                 result=result,
             )
 
         except DuplicateKeyError as e:
+            if self.mongo.log:
+                print("[Mongo.Duplicate]", e)
+
             return UpdateResponse(
                 ok=False,
                 is_duplicate=True,
                 error=e,
             )
 
         except Exception as e:
+            if self.mongo.log:
+                print("[Mongo.Error]", e)
+
             return UpdateResponse(
                 ok=False,
                 error=e,
             )
 
     def count(
         self,
         query: Dict = None,  # type: ignore
     ):
         return self.collection.count_documents(query)
 
     def distinct(self, key: str):  # type: ignore
         return self.collection.distinct(key)
+
+    def aggregate(self, pipeline: _Pipeline, **kwargs):
+        return self.collection.aggregate(
+            pipeline,
+            **kwargs,
+        )
```

### Comparing `lazy_mongo-0.2.4/lazy_mongo/lazy_database.py` & `lazy_mongo-0.3.0/lazy_mongo/lazy_database.py`

 * *Files 17% similar despite different names*

```diff
@@ -1,18 +1,27 @@
-from typing import Dict, NamedTuple
+from typing import Dict, NamedTuple, TYPE_CHECKING
 from pymongo.database import Database
 from .lazy_collection import LazyCollection
+from pymongo.typings import _Pipeline
+
+if TYPE_CHECKING:
+    from .lazy_mongo import LazyMongo
 
 
 class LazyDatabase(NamedTuple):
+    mongo: LazyMongo
     database: Database
     default_collection_name: str = None  # type: ignore
 
     def __getitem__(self, key: str):
-        return LazyCollection(self.database[key])
+        return LazyCollection(
+            mongo=self.mongo,
+            database=self,
+            collection=self.database[key],
+        )
 
     def find_one(
         self,
         collection: str = None,
         query: Dict = None,
         project: Dict = None,
     ):
@@ -62,7 +71,17 @@
         self,
         key: str,
         collection: str = None,  # type: ignore
     ):
         coll = self[collection or self.default_collection_name]
 
         return coll.distinct(key)
+
+    def aggregate(
+        self,
+        pipeline: _Pipeline,
+        collection: str = None,  # type: ignore
+        **kwargs,
+    ):
+        coll = self[collection or self.default_collection_name]
+
+        return coll.aggregate(pipeline, **kwargs)
```

### Comparing `lazy_mongo-0.2.4/lazy_mongo/lazy_mongo.py` & `lazy_mongo-0.3.0/lazy_mongo/lazy_mongo.py`

 * *Files 25% similar despite different names*

```diff
@@ -1,28 +1,31 @@
 from typing import Dict
 from pymongo import MongoClient
 from .lazy_database import LazyDatabase
+from pymongo.typings import _Pipeline
 
 
 class LazyMongo:
     def __init__(self):
         self.mongo: MongoClient = None  # type: ignore
         self.default_database: str = None  # type: ignore
         self.default_collection: str = None  # type: ignore
+        self.log: bool = True
 
     def connect(self, uri: str):
         try:
             self.mongo = MongoClient(uri)
         except:
             pass
 
         return self
 
     def __getitem__(self, key: str):
         return LazyDatabase(
+            mongo=self,
             database=self.mongo[key or self.default_database],
             default_collection_name=self.default_collection,
         )
 
     def find_one(
         self,
         database: str = None,
@@ -85,7 +88,18 @@
         key: str,
         database: str = None,  # type: ignore
         collection: str = None,  # type: ignore
     ):
         db = self[database or self.default_database]
 
         return db.distinct(key, collection)
+
+    def aggregate(
+        self,
+        pipeline: _Pipeline,
+        database: str = None,
+        collection: str = None,
+        **kwargs,
+    ):
+        db = self[database or self.default_database]
+
+        return db.aggregate(pipeline, collection, **kwargs)
```

### Comparing `lazy_mongo-0.2.4/PKG-INFO` & `lazy_mongo-0.3.0/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: lazy-mongo
-Version: 0.2.4
+Version: 0.3.0
 Summary: 
 Author: MisterNyan
 Author-email: michael.edmund.wong@gmail.com
 Requires-Python: >=3.8,<4.0
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
```

