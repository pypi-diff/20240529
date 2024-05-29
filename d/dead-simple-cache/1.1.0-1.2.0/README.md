# Comparing `tmp/dead_simple_cache-1.1.0-py3-none-any.whl.zip` & `tmp/dead_simple_cache-1.2.0-py3-none-any.whl.zip`

## zipinfo {}

```diff
@@ -1,10 +1,10 @@
-Zip file size: 7347 bytes, number of entries: 8
--rw-rw-r--  2.0 unx     2988 b- defN 24-May-28 16:31 dead_simple_cache/__init__.py
--rw-rw-r--  2.0 unx      177 b- defN 24-May-28 16:28 dead_simple_cache/version.py
--rw-rw-r--  2.0 unx    11359 b- defN 24-May-28 16:38 dead_simple_cache-1.1.0.dist-info/LICENSE
--rw-rw-r--  2.0 unx     1059 b- defN 24-May-28 16:38 dead_simple_cache-1.1.0.dist-info/METADATA
--rw-rw-r--  2.0 unx       92 b- defN 24-May-28 16:38 dead_simple_cache-1.1.0.dist-info/WHEEL
--rw-rw-r--  2.0 unx       18 b- defN 24-May-28 16:38 dead_simple_cache-1.1.0.dist-info/top_level.txt
--rw-rw-r--  2.0 unx        1 b- defN 24-May-28 16:38 dead_simple_cache-1.1.0.dist-info/zip-safe
--rw-rw-r--  2.0 unx      703 b- defN 24-May-28 16:38 dead_simple_cache-1.1.0.dist-info/RECORD
-8 files, 16397 bytes uncompressed, 6101 bytes compressed:  62.8%
+Zip file size: 7399 bytes, number of entries: 8
+-rw-rw-r--  2.0 unx     3154 b- defN 24-May-28 20:06 dead_simple_cache/__init__.py
+-rw-rw-r--  2.0 unx      177 b- defN 24-May-28 19:34 dead_simple_cache/version.py
+-rw-rw-r--  2.0 unx    11359 b- defN 24-May-28 20:17 dead_simple_cache-1.2.0.dist-info/LICENSE
+-rw-rw-r--  2.0 unx     1072 b- defN 24-May-28 20:17 dead_simple_cache-1.2.0.dist-info/METADATA
+-rw-rw-r--  2.0 unx       92 b- defN 24-May-28 20:17 dead_simple_cache-1.2.0.dist-info/WHEEL
+-rw-rw-r--  2.0 unx       18 b- defN 24-May-28 20:17 dead_simple_cache-1.2.0.dist-info/top_level.txt
+-rw-rw-r--  2.0 unx        1 b- defN 24-May-28 20:17 dead_simple_cache-1.2.0.dist-info/zip-safe
+-rw-rw-r--  2.0 unx      703 b- defN 24-May-28 20:17 dead_simple_cache-1.2.0.dist-info/RECORD
+8 files, 16576 bytes uncompressed, 6153 bytes compressed:  62.9%
```

## zipnote {}

```diff
@@ -1,25 +1,25 @@
 Filename: dead_simple_cache/__init__.py
 Comment: 
 
 Filename: dead_simple_cache/version.py
 Comment: 
 
-Filename: dead_simple_cache-1.1.0.dist-info/LICENSE
+Filename: dead_simple_cache-1.2.0.dist-info/LICENSE
 Comment: 
 
-Filename: dead_simple_cache-1.1.0.dist-info/METADATA
+Filename: dead_simple_cache-1.2.0.dist-info/METADATA
 Comment: 
 
-Filename: dead_simple_cache-1.1.0.dist-info/WHEEL
+Filename: dead_simple_cache-1.2.0.dist-info/WHEEL
 Comment: 
 
-Filename: dead_simple_cache-1.1.0.dist-info/top_level.txt
+Filename: dead_simple_cache-1.2.0.dist-info/top_level.txt
 Comment: 
 
-Filename: dead_simple_cache-1.1.0.dist-info/zip-safe
+Filename: dead_simple_cache-1.2.0.dist-info/zip-safe
 Comment: 
 
-Filename: dead_simple_cache-1.1.0.dist-info/RECORD
+Filename: dead_simple_cache-1.2.0.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## dead_simple_cache/__init__.py

```diff
@@ -17,20 +17,20 @@
     """Simple cache."""
 
     def __init__(self, file_path: str, fuzzy_threshold: float = 0.75):
         if not file_path:
             logger.error("error setting cache: 'path' must be set")
             raise ValueError("'path' must be set")
         try:
-            base_dir = os.path.dirname(file_path)
+            full_path = os.path.abspath(os.path.expanduser(file_path))
+            base_dir = os.path.dirname(full_path)
             os.makedirs(base_dir, exist_ok=True)
         except Exception as e:
             logger.error(f"error setting cache: {e}")
             raise ValueError(e)
-        full_path = os.path.abspath(os.path.expanduser(file_path))
         if full_path not in FILE_LOCKS:
             FILE_LOCKS[full_path] = Lock()
         self._lock = FILE_LOCKS[full_path]
         # Open database for reading and writing
         self._db = shelve.open(file_path, flag='c', protocol=None, writeback=False)
         self._threshold = fuzzy_threshold
         with self._lock:
@@ -41,37 +41,37 @@
             self._db.sync()
             self._db.close()
 
     def _match(self, key: str, query: str) -> float:
         """Fuzzy matching helper method."""
         return DamerauLevenshtein.normalized_similarity(key, query) >= self._threshold
 
-    def _get(self, key: str) -> list:
+    def _get(self, key: str) -> dict:
         """Get data."""
         with self._lock:
             data = self._db.get(key, default=[])
-        return data
+        return {key: data} if data else {}
 
-    def _fuzzy_get(self, query: str) -> list:
+    def _fuzzy_get(self, query: str) -> dict:
         """Get data with fuzzy matching."""
         with self._lock:
-            filtered_keys = list(
+            keys = list(
                     filter(
                         lambda key: self._match(key, query),
                         self.keys
                     )
                 )
-            data = sum([self._db[key] for key in filtered_keys], [])
-        return data
+            data = [self._db[key] for key in keys]
+        return dict(zip(keys, data)) if keys else {}
 
     def replace(self, key: Any, data: Any) -> None:
         """Replace data."""
         key_ = str(key).lower()
         with self._lock:
-            self._db[key_] = [data]
+            self._db[key_] = data if isinstance(data, list) else [data]
 
     def delete(self, key: Any) -> None:
         key_ = str(key).lower()
         with self._lock:
             if key_ in self.keys:
                 del self._db[key_]
                 self.keys.remove(key_)
@@ -81,16 +81,19 @@
         data_ = []
         key_ = str(key).lower()
         with self._lock:
             if key_ in self.keys:
                 data_ = self._db[key_]
             else:
                 insort(self.keys, key_)
-            data_.append(data)
+            if isinstance(data, list):
+                data_.extend(data)
+            else:
+                data_.append(data)
             self._db[key_] = data_
 
-    def get(self, query: Any, fuzzy: bool = False) -> Optional[Any]:
+    def get(self, query: Any, fuzzy: bool = False) -> Optional[dict]:
         """Get data."""
         if fuzzy:
             return self._fuzzy_get(str(query))
         else:
             return self._get(str(query))
```

## dead_simple_cache/version.py

```diff
@@ -1,7 +1,7 @@
 # The following lines are replaced during the release process.
 # START_VERSION_BLOCK
 VERSION_MAJOR = 1
-VERSION_MINOR = 1
+VERSION_MINOR = 2
 VERSION_BUILD = 0
 VERSION_ALPHA = 0
 # END_VERSION_BLOCK
```

## Comparing `dead_simple_cache-1.1.0.dist-info/LICENSE` & `dead_simple_cache-1.2.0.dist-info/LICENSE`

 * *Files identical despite different names*

## Comparing `dead_simple_cache-1.1.0.dist-info/METADATA` & `dead_simple_cache-1.2.0.dist-info/METADATA`

 * *Files 26% similar despite different names*

```diff
@@ -1,34 +1,34 @@
 Metadata-Version: 2.1
 Name: dead-simple-cache
-Version: 1.1.0
-Summary: A dead simple Python caching lib
+Version: 1.2.0
+Summary: A dead simple caching lib
 Home-page: https://github.com/femelo/dead-simple-cache
 Author: Flávio De Melo
 Author-email: flavio.eler@gmail.com
 License: Apache 2.0
 Keywords: caching
 Description-Content-Type: text/markdown
 License-File: LICENSE
 Requires-Dist: rapidfuzz
 
-# Metadata cache
+# Dead Simple Cache
 
 A dead simple thread-safe caching lib powered by [shelve](https://docs.python.org/3/library/shelve.html).
 
 ## Usage
 
 Include the plugin as dependency and use it as:
 
 ```python
 >>> from dead_simple_cache import SimpleCache
->>> cache = SimpleCache(file_path="~/.cache/cache.db")
+>>> cache = SimpleCache(file_path="~/.cache/cache")
 >>> cache.add(key="tsf jazz", data={"name": "tsf jazz", "url": "http://tsfjazz.ice.infomaniak.ch/tsfjazz-high.mp3"})
 >>> cache.get(query="tsf jazz")
-    [{'name': 'tsf jazz',
-      'url': 'http://tsfjazz.ice.infomaniak.ch/tsfjazz-high.mp3'}]
+  {'tsf jazz': [{'name': 'tsf jazz',
+    'url': 'http://tsfjazz.ice.infomaniak.ch/tsfjazz-high.mp3'}]}
 >>> cache.get(query="tsf jas")
-    []
+    {}
 >>> cache.get(query="tsf jas", fuzzy=True)
-    [{'name': 'tsf jazz',
-      'url': 'http://tsfjazz.ice.infomaniak.ch/tsfjazz-high.mp3'}]
+  {'tsf jazz': [{'name': 'tsf jazz',
+    'url': 'http://tsfjazz.ice.infomaniak.ch/tsfjazz-high.mp3'}]}
 ```
```

## Comparing `dead_simple_cache-1.1.0.dist-info/RECORD` & `dead_simple_cache-1.2.0.dist-info/RECORD`

 * *Files 25% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-dead_simple_cache/__init__.py,sha256=qLeCTgcb3ljlqyoI9XTmxCnAyJap8WmmDoCw-qIU0eo,2988
-dead_simple_cache/version.py,sha256=QhCEpRnWjcAahK9d4tQka767FA6R2Dsf1wOhR-9b2JU,177
-dead_simple_cache-1.1.0.dist-info/LICENSE,sha256=jG2zQEdRNt88EgHUWPpXVWmOrOduUQRx7MnYV9YIPaw,11359
-dead_simple_cache-1.1.0.dist-info/METADATA,sha256=C7o1zQdSCLy66UV9_ld1JznUgX-8x79H3jA-SuctuhA,1059
-dead_simple_cache-1.1.0.dist-info/WHEEL,sha256=GJ7t_kWBFywbagK5eo9IoUwLW6oyOeTKmQ-9iHFVNxQ,92
-dead_simple_cache-1.1.0.dist-info/top_level.txt,sha256=rTXFTTGmSN_J-s3wSqL0KtbHyyZ2oA_-kyWEt6-e0Ss,18
-dead_simple_cache-1.1.0.dist-info/zip-safe,sha256=AbpHGcgLb-kRsJGnwFEktk7uzpZOCcBY74-YBdrKVGs,1
-dead_simple_cache-1.1.0.dist-info/RECORD,,
+dead_simple_cache/__init__.py,sha256=xTr9dRhtU32HBu1jQbVtZG8AgP0VVs8M1wOPFwE2uqA,3154
+dead_simple_cache/version.py,sha256=xkoU9LVlDlOSIZ00Z6I4UlYCHlCNGapNzUksvH9hl3I,177
+dead_simple_cache-1.2.0.dist-info/LICENSE,sha256=jG2zQEdRNt88EgHUWPpXVWmOrOduUQRx7MnYV9YIPaw,11359
+dead_simple_cache-1.2.0.dist-info/METADATA,sha256=9t2Xy4CDf7K1NMGjiJVXYHtdlFpF9JeVaoNchAfLVx4,1072
+dead_simple_cache-1.2.0.dist-info/WHEEL,sha256=GJ7t_kWBFywbagK5eo9IoUwLW6oyOeTKmQ-9iHFVNxQ,92
+dead_simple_cache-1.2.0.dist-info/top_level.txt,sha256=rTXFTTGmSN_J-s3wSqL0KtbHyyZ2oA_-kyWEt6-e0Ss,18
+dead_simple_cache-1.2.0.dist-info/zip-safe,sha256=AbpHGcgLb-kRsJGnwFEktk7uzpZOCcBY74-YBdrKVGs,1
+dead_simple_cache-1.2.0.dist-info/RECORD,,
```

