# Comparing `tmp/spark_congruity-0.0.1rc3.tar.gz` & `tmp/spark_congruity-0.0.1rc4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "spark_congruity-0.0.1rc3.tar", max compression
+gzip compressed data, was "spark_congruity-0.0.1rc4.tar", max compression
```

## Comparing `spark_congruity-0.0.1rc3.tar` & `spark_congruity-0.0.1rc4.tar`

### file list

```diff
@@ -1,9 +1,13 @@
--rw-r--r--   0        0        0    11357 2024-05-28 21:15:49.236696 spark_congruity-0.0.1rc3/LICENSE
--rw-r--r--   0        0        0     1150 2024-05-28 21:15:49.236696 spark_congruity-0.0.1rc3/NOTICE
--rw-r--r--   0        0        0    15808 2024-05-28 21:15:49.236696 spark_congruity-0.0.1rc3/README.md
--rw-r--r--   0        0        0     2151 2024-05-28 21:15:49.236696 spark_congruity-0.0.1rc3/congruity/__init__.py
--rw-r--r--   0        0        0     1594 2024-05-28 21:15:49.236696 spark_congruity-0.0.1rc3/congruity/json_conversion.py
--rw-r--r--   0        0        0    18998 2024-05-28 21:15:49.236696 spark_congruity-0.0.1rc3/congruity/rdd_adapter.py
--rw-r--r--   0        0        0     1768 2024-05-28 21:15:49.236696 spark_congruity-0.0.1rc3/congruity/spark_context_adapter.py
--rw-r--r--   0        0        0     2206 2024-05-28 21:15:49.236696 spark_congruity-0.0.1rc3/pyproject.toml
--rw-r--r--   0        0        0    16742 1970-01-01 00:00:00.000000 spark_congruity-0.0.1rc3/PKG-INFO
+-rw-r--r--   0        0        0    11357 2024-05-29 09:28:20.634394 spark_congruity-0.0.1rc4/LICENSE
+-rw-r--r--   0        0        0     1150 2024-05-29 09:28:20.634394 spark_congruity-0.0.1rc4/NOTICE
+-rw-r--r--   0        0        0    15808 2024-05-29 09:28:20.634394 spark_congruity-0.0.1rc4/README.md
+-rw-r--r--   0        0        0      775 2024-05-29 09:28:20.634394 spark_congruity-0.0.1rc4/congruity/__init__.py
+-rw-r--r--   0        0        0     2670 2024-05-29 09:28:20.634394 spark_congruity-0.0.1rc4/congruity/helper/__init__.py
+-rw-r--r--   0        0        0     2099 2024-05-29 09:28:20.634394 spark_congruity-0.0.1rc4/congruity/helper/patch.py
+-rw-r--r--   0        0        0     1885 2024-05-29 09:28:20.634394 spark_congruity-0.0.1rc4/congruity/helper/rdd.py
+-rw-r--r--   0        0        0     1594 2024-05-29 09:28:20.634394 spark_congruity-0.0.1rc4/congruity/json_conversion.py
+-rw-r--r--   0        0        0      898 2024-05-29 09:28:20.634394 spark_congruity-0.0.1rc4/congruity/patch.py
+-rw-r--r--   0        0        0    16647 2024-05-29 09:28:20.634394 spark_congruity-0.0.1rc4/congruity/rdd_adapter.py
+-rw-r--r--   0        0        0     1768 2024-05-29 09:28:20.634394 spark_congruity-0.0.1rc4/congruity/spark_context_adapter.py
+-rw-r--r--   0        0        0     2206 2024-05-29 09:28:20.634394 spark_congruity-0.0.1rc4/pyproject.toml
+-rw-r--r--   0        0        0    16742 1970-01-01 00:00:00.000000 spark_congruity-0.0.1rc4/PKG-INFO
```

### Comparing `spark_congruity-0.0.1rc3/LICENSE` & `spark_congruity-0.0.1rc4/LICENSE`

 * *Files identical despite different names*

### Comparing `spark_congruity-0.0.1rc3/NOTICE` & `spark_congruity-0.0.1rc4/NOTICE`

 * *Files identical despite different names*

### Comparing `spark_congruity-0.0.1rc3/README.md` & `spark_congruity-0.0.1rc4/README.md`

 * *Files identical despite different names*

### Comparing `spark_congruity-0.0.1rc3/congruity/__init__.py` & `spark_congruity-0.0.1rc4/congruity/helper/patch.py`

 * *Files 7% similar despite different names*

```diff
@@ -8,51 +8,47 @@
 # http://www.apache.org/licenses/LICENSE-2.0
 #
 # Unless required by applicable law or agreed to in writing, software
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
+
 from pyspark.errors import PySparkAttributeError, PySparkNotImplementedError
 
 from congruity.json_conversion import to_json_conversion
 from congruity.rdd_adapter import adapt_to_rdd
 from congruity.spark_context_adapter import adapt_to_spark_context
 
-_monkey_patch_complete = False
-
 
 def adapt_session_getattr(self, name):
     if name in ["_jsc", "_jconf", "_jvm", "_jsparkSession"]:
         raise PySparkAttributeError(
             error_class="JVM_ATTRIBUTE_NOT_SUPPORTED", message_parameters={"attr_name": name}
         )
     elif name in ["newSession"]:
         raise PySparkNotImplementedError(
             error_class="NOT_IMPLEMENTED", message_parameters={"feature": f"{name}()"}
         )
 
 
 def monkey_patch_spark():
+    import congruity.patch as p
     from pyspark.sql.connect.session import SparkSession
 
-    global _monkey_patch_complete
-    if _monkey_patch_complete:
+    if p._monkey_patch_complete:
         return
     from pyspark.sql.connect.dataframe import DataFrame
 
     # Register all the monkey patches here.
     DataFrame.toJSON = to_json_conversion
 
     # Patch properties.
     setattr(DataFrame, "rdd", property(adapt_to_rdd))
     setattr(DataFrame, "sparkContext", property(adapt_to_spark_context))
 
     # Spark Session
     setattr(SparkSession, "sparkContext", property(adapt_to_spark_context))
     SparkSession.__getattr__ = adapt_session_getattr
 
-    _monkey_patch_complete = True
+    p._monkey_patch_complete = True
     return
-
-
-monkey_patch_spark()
```

### Comparing `spark_congruity-0.0.1rc3/congruity/json_conversion.py` & `spark_congruity-0.0.1rc4/congruity/json_conversion.py`

 * *Files identical despite different names*

### Comparing `spark_congruity-0.0.1rc3/congruity/rdd_adapter.py` & `spark_congruity-0.0.1rc4/congruity/rdd_adapter.py`

 * *Files 9% similar despite different names*

```diff
@@ -31,14 +31,17 @@
     Generic,
 )
 
 import pandas
 from pyspark.serializers import CloudPickleSerializer, CPickleSerializer, AutoBatchedSerializer
 from pyspark.statcounter import StatCounter
 
+import congruity.helper
+from congruity.helper.rdd import WrappedIterator
+
 T = TypeVar("T")
 T_co = TypeVar("T_co", covariant=True)
 U = TypeVar("U")
 K = TypeVar("K", bound=Hashable)
 V = TypeVar("V")
 V1 = TypeVar("V1")
 V2 = TypeVar("V2")
@@ -393,41 +396,14 @@
         return RDDAdapter(df, first_field=True)
 
     groupByKey.__doc__ = RDD.groupByKey.__doc__
 
     mapValues = RDD.mapValues
     mapValues.__doc__ = RDD.mapValues.__doc__
 
-    class WrappedIterator(Iterable):
-        """This is a helper class that wraps the iterator of RecordBatches as returned by
-        mapInArrow and converts it into an iterator of the underlaying values."""
-
-        def __init__(self, i: Iterable[RecordBatch], first_field=False):
-            self._first_field = first_field
-            self._iter = i
-            self._current_batch = None
-            self._current_idx = 0
-            self._done = False
-
-        def __next__(self):
-            if self._current_batch is None or self._current_idx >= len(self._current_batch):
-                self._current_idx = 0
-                v: RecordBatch = next(self._iter)
-                if self._first_field:
-                    self._current_batch = [loads(x["__bin_field__"]) for x in v.to_pylist()]
-                else:
-                    self._current_batch = [Row(**x) for x in v.to_pylist()]
-
-            result = self._current_batch[self._current_idx]
-            self._current_idx += 1
-            return result
-
-        def __iter__(self):
-            return self
-
     def mapPartitions(
         self, f: Callable[[Iterable[T]], Iterable[U]], preservesPartitioning=False
     ) -> "RDDAdapter[U]":
         # Every pipeline becomes mapPartitions in the end. So we pass the current RDD as the
         # previous reference and the next transformation function.
         return Pipeline(self, f)
 
@@ -445,33 +421,17 @@
         self._df = input._df.mapInArrow(mapper, RDDAdapter.BIN_TUPLE_SCHEMA)
         self._first_field = True
 
     def _build_mapper(self, f, needs_conversion):
         # Fixed constants for the mapPartitions implementation.
         schema = RDDAdapter.PA_TUPLE_SCHEMA
         max_rows_per_batch = 1000
-
-        def mapper(iter: Iterable[RecordBatch]):
-            # the function that is passed to mapPartitions works the same way as the mapper. But
-            # when next(iter) is called we have to send the converted batch instead of the raw
-            # data.
-            wrapped = RDDAdapter.WrappedIterator(iter, needs_conversion)
-            result = []
-            for kv in f(wrapped):
-                # kv is a tuple with a key value pair.
-                assert len(kv) == 2
-                result.append({"__bin_field_k__": dumps(kv[0]), "__bin_field_v__": dumps(kv[1])})
-                if len(result) > max_rows_per_batch:
-                    yield RecordBatch.from_pylist(result, schema=schema)
-                    result = []
-
-            if len(result) > 0:
-                yield RecordBatch.from_pylist(result, schema=schema)
-
-        return mapper
+        return congruity.helper.generate_tuple_mapper(
+            f, needs_conversion, schema, max_rows_per_batch
+        )
 
 
 class Pipeline(RDDAdapter):
     """The pipeline is an extension of the RDDAdapter that allows to pipeline multiple
     mapPartitions operations. This is useful to avoid the overhead of creating multiple
     plan execution nodes. Instead, we can create a single plan node that executes all the
     operations in a single pass."""
@@ -505,24 +465,10 @@
         self._df = source.mapInArrow(mapper, RDDAdapter.BIN_SCHEMA)
         self._first_field = True
 
     def _build_mapper(self, f, needs_conversion):
         # Fixed constants for the mapPartitions implementation.
         schema = RDDAdapter.PA_SCHEMA
         max_rows_per_batch = 1000
-
-        def mapper(iter: Iterable[RecordBatch]):
-            # the function that is passed to mapPartitions works the same way as the mapper. But
-            # when next(iter) is called we have to send the converted batch instead of the raw
-            # data.
-            wrapped = RDDAdapter.WrappedIterator(iter, needs_conversion)
-            result = []
-            for batch in f(wrapped):
-                result.append({"__bin_field__": dumps(batch)})
-                if len(result) > max_rows_per_batch:
-                    yield RecordBatch.from_pylist(result, schema=schema)
-                    result = []
-
-            if len(result) > 0:
-                yield RecordBatch.from_pylist(result, schema=schema)
-
-        return mapper
+        return congruity.helper.generate_partitions_mapper(
+            f, needs_conversion, schema, max_rows_per_batch
+        )
```

### Comparing `spark_congruity-0.0.1rc3/congruity/spark_context_adapter.py` & `spark_congruity-0.0.1rc4/congruity/spark_context_adapter.py`

 * *Files identical despite different names*

### Comparing `spark_congruity-0.0.1rc3/pyproject.toml` & `spark_congruity-0.0.1rc4/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -11,15 +11,15 @@
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 
 [tool.poetry]
 name = "spark-congruity"
-version = "0.0.1rc3"
+version = "0.0.1rc4"
 description = ""
 authors = ["Matthew Powers <matthewkevinpowers@gmail.com>", "Martin Grund <martin@databricks.com>"]
 readme = "README.md"
 license = "Apache-2.0"
 homepage = "https://github.com/databricks/congruity"
 repository = "https://github.com/databricks/congruity"
 classifiers = [
```

### Comparing `spark_congruity-0.0.1rc3/PKG-INFO` & `spark_congruity-0.0.1rc4/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: spark-congruity
-Version: 0.0.1rc3
+Version: 0.0.1rc4
 Summary: 
 Home-page: https://github.com/databricks/congruity
 License: Apache-2.0
 Author: Matthew Powers
 Author-email: matthewkevinpowers@gmail.com
 Requires-Python: >=3.8,<4.0
 Classifier: Development Status :: 4 - Beta
```

