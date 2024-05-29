# Comparing `tmp/pynamodb-6.0.1.tar.gz` & `tmp/pynamodb-6.0a0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pynamodb-6.0.1.tar", last modified: Wed May 29 18:50:23 2024, max compression
+gzip compressed data, was "pynamodb-6.0a0.tar", last modified: Sun Jan 14 03:01:44 2024, max compression
```

## Comparing `pynamodb-6.0.1.tar` & `pynamodb-6.0a0.tar`

### file list

```diff
@@ -1,56 +1,56 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-29 18:50:23.910476 pynamodb-6.0.1/
--rw-r--r--   0 runner    (1001) docker     (127)     1080 2024-05-29 18:50:09.000000 pynamodb-6.0.1/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)       60 2024-05-29 18:50:09.000000 pynamodb-6.0.1/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (127)     6714 2024-05-29 18:50:23.910476 pynamodb-6.0.1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     5722 2024-05-29 18:50:09.000000 pynamodb-6.0.1/README.rst
--rw-r--r--   0 runner    (1001) docker     (127)      441 2024-05-29 18:50:09.000000 pynamodb-6.0.1/mypy.ini
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-29 18:50:23.902476 pynamodb-6.0.1/pynamodb/
--rw-r--r--   0 runner    (1001) docker     (127)      150 2024-05-29 18:50:09.000000 pynamodb-6.0.1/pynamodb/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1162 2024-05-29 18:50:09.000000 pynamodb-6.0.1/pynamodb/_schema.py
--rw-r--r--   0 runner    (1001) docker     (127)     3350 2024-05-29 18:50:09.000000 pynamodb-6.0.1/pynamodb/_util.py
--rw-r--r--   0 runner    (1001) docker     (127)    58586 2024-05-29 18:50:09.000000 pynamodb-6.0.1/pynamodb/attributes.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-29 18:50:23.902476 pynamodb-6.0.1/pynamodb/connection/
--rw-r--r--   0 runner    (1001) docker     (127)      201 2024-05-29 18:50:09.000000 pynamodb-6.0.1/pynamodb/connection/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      789 2024-05-29 18:50:09.000000 pynamodb-6.0.1/pynamodb/connection/_botocore_private.py
--rw-r--r--   0 runner    (1001) docker     (127)    50937 2024-05-29 18:50:09.000000 pynamodb-6.0.1/pynamodb/connection/base.py
--rw-r--r--   0 runner    (1001) docker     (127)    11889 2024-05-29 18:50:09.000000 pynamodb-6.0.1/pynamodb/connection/table.py
--rw-r--r--   0 runner    (1001) docker     (127)     6797 2024-05-29 18:50:09.000000 pynamodb-6.0.1/pynamodb/constants.py
--rw-r--r--   0 runner    (1001) docker     (127)     7919 2024-05-29 18:50:09.000000 pynamodb-6.0.1/pynamodb/exceptions.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-29 18:50:23.906476 pynamodb-6.0.1/pynamodb/expressions/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-29 18:50:09.000000 pynamodb-6.0.1/pynamodb/expressions/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     4393 2024-05-29 18:50:09.000000 pynamodb-6.0.1/pynamodb/expressions/condition.py
--rw-r--r--   0 runner    (1001) docker     (127)    14293 2024-05-29 18:50:09.000000 pynamodb-6.0.1/pynamodb/expressions/operand.py
--rw-r--r--   0 runner    (1001) docker     (127)      811 2024-05-29 18:50:09.000000 pynamodb-6.0.1/pynamodb/expressions/projection.py
--rw-r--r--   0 runner    (1001) docker     (127)     4661 2024-05-29 18:50:09.000000 pynamodb-6.0.1/pynamodb/expressions/update.py
--rw-r--r--   0 runner    (1001) docker     (127)     2476 2024-05-29 18:50:09.000000 pynamodb-6.0.1/pynamodb/expressions/util.py
--rw-r--r--   0 runner    (1001) docker     (127)     8217 2024-05-29 18:50:09.000000 pynamodb-6.0.1/pynamodb/indexes.py
--rw-r--r--   0 runner    (1001) docker     (127)    49590 2024-05-29 18:50:09.000000 pynamodb-6.0.1/pynamodb/models.py
--rw-r--r--   0 runner    (1001) docker     (127)     7356 2024-05-29 18:50:09.000000 pynamodb-6.0.1/pynamodb/pagination.py
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-29 18:50:09.000000 pynamodb-6.0.1/pynamodb/py.typed
--rw-r--r--   0 runner    (1001) docker     (127)     1741 2024-05-29 18:50:09.000000 pynamodb-6.0.1/pynamodb/settings.py
--rw-r--r--   0 runner    (1001) docker     (127)     1533 2024-05-29 18:50:09.000000 pynamodb-6.0.1/pynamodb/signals.py
--rw-r--r--   0 runner    (1001) docker     (127)     5595 2024-05-29 18:50:09.000000 pynamodb-6.0.1/pynamodb/transactions.py
--rw-r--r--   0 runner    (1001) docker     (127)      101 2024-05-29 18:50:09.000000 pynamodb-6.0.1/pynamodb/types.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-29 18:50:23.910476 pynamodb-6.0.1/pynamodb.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     6714 2024-05-29 18:50:23.000000 pynamodb-6.0.1/pynamodb.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     1202 2024-05-29 18:50:23.000000 pynamodb-6.0.1/pynamodb.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-29 18:50:23.000000 pynamodb-6.0.1/pynamodb.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-29 18:50:23.000000 pynamodb-6.0.1/pynamodb.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (127)       96 2024-05-29 18:50:23.000000 pynamodb-6.0.1/pynamodb.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)        9 2024-05-29 18:50:23.000000 pynamodb-6.0.1/pynamodb.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)      176 2024-05-29 18:50:09.000000 pynamodb-6.0.1/requirements-dev.txt
--rw-r--r--   0 runner    (1001) docker     (127)      101 2024-05-29 18:50:23.910476 pynamodb-6.0.1/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)     1382 2024-05-29 18:50:09.000000 pynamodb-6.0.1/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-29 18:50:23.906476 pynamodb-6.0.1/tests/
--rw-r--r--   0 runner    (1001) docker     (127)    50686 2024-05-29 18:50:09.000000 pynamodb-6.0.1/tests/test_attributes.py
--rw-r--r--   0 runner    (1001) docker     (127)    54894 2024-05-29 18:50:09.000000 pynamodb-6.0.1/tests/test_base_connection.py
--rw-r--r--   0 runner    (1001) docker     (127)      466 2024-05-29 18:50:09.000000 pynamodb-6.0.1/tests/test_binary_legacy_encoding.py
--rw-r--r--   0 runner    (1001) docker     (127)     6828 2024-05-29 18:50:09.000000 pynamodb-6.0.1/tests/test_discriminator.py
--rw-r--r--   0 runner    (1001) docker     (127)     1155 2024-05-29 18:50:09.000000 pynamodb-6.0.1/tests/test_exceptions.py
--rw-r--r--   0 runner    (1001) docker     (127)    30876 2024-05-29 18:50:09.000000 pynamodb-6.0.1/tests/test_expressions.py
--rw-r--r--   0 runner    (1001) docker     (127)   127499 2024-05-29 18:50:09.000000 pynamodb-6.0.1/tests/test_model.py
--rw-r--r--   0 runner    (1001) docker     (127)     2078 2024-05-29 18:50:09.000000 pynamodb-6.0.1/tests/test_pagination.py
--rw-r--r--   0 runner    (1001) docker     (127)      643 2024-05-29 18:50:09.000000 pynamodb-6.0.1/tests/test_settings.py
--rw-r--r--   0 runner    (1001) docker     (127)     3788 2024-05-29 18:50:09.000000 pynamodb-6.0.1/tests/test_signals.py
--rw-r--r--   0 runner    (1001) docker     (127)    20252 2024-05-29 18:50:09.000000 pynamodb-6.0.1/tests/test_table_connection.py
--rw-r--r--   0 runner    (1001) docker     (127)     4551 2024-05-29 18:50:09.000000 pynamodb-6.0.1/tests/test_transaction.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-14 03:01:44.116251 pynamodb-6.0a0/
+-rw-r--r--   0 runner    (1001) docker     (127)     1080 2024-01-14 03:01:23.000000 pynamodb-6.0a0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)       60 2024-01-14 03:01:23.000000 pynamodb-6.0a0/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (127)     6714 2024-01-14 03:01:44.116251 pynamodb-6.0a0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     5722 2024-01-14 03:01:23.000000 pynamodb-6.0a0/README.rst
+-rw-r--r--   0 runner    (1001) docker     (127)      441 2024-01-14 03:01:23.000000 pynamodb-6.0a0/mypy.ini
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-14 03:01:44.108251 pynamodb-6.0a0/pynamodb/
+-rw-r--r--   0 runner    (1001) docker     (127)      150 2024-01-14 03:01:23.000000 pynamodb-6.0a0/pynamodb/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1162 2024-01-14 03:01:23.000000 pynamodb-6.0a0/pynamodb/_schema.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3350 2024-01-14 03:01:23.000000 pynamodb-6.0a0/pynamodb/_util.py
+-rw-r--r--   0 runner    (1001) docker     (127)    58584 2024-01-14 03:01:23.000000 pynamodb-6.0a0/pynamodb/attributes.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-14 03:01:44.108251 pynamodb-6.0a0/pynamodb/connection/
+-rw-r--r--   0 runner    (1001) docker     (127)      201 2024-01-14 03:01:23.000000 pynamodb-6.0a0/pynamodb/connection/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      789 2024-01-14 03:01:23.000000 pynamodb-6.0a0/pynamodb/connection/_botocore_private.py
+-rw-r--r--   0 runner    (1001) docker     (127)    50888 2024-01-14 03:01:23.000000 pynamodb-6.0a0/pynamodb/connection/base.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11889 2024-01-14 03:01:23.000000 pynamodb-6.0a0/pynamodb/connection/table.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6797 2024-01-14 03:01:23.000000 pynamodb-6.0a0/pynamodb/constants.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7862 2024-01-14 03:01:23.000000 pynamodb-6.0a0/pynamodb/exceptions.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-14 03:01:44.108251 pynamodb-6.0a0/pynamodb/expressions/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-01-14 03:01:23.000000 pynamodb-6.0a0/pynamodb/expressions/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4393 2024-01-14 03:01:23.000000 pynamodb-6.0a0/pynamodb/expressions/condition.py
+-rw-r--r--   0 runner    (1001) docker     (127)    14293 2024-01-14 03:01:23.000000 pynamodb-6.0a0/pynamodb/expressions/operand.py
+-rw-r--r--   0 runner    (1001) docker     (127)      811 2024-01-14 03:01:23.000000 pynamodb-6.0a0/pynamodb/expressions/projection.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4661 2024-01-14 03:01:23.000000 pynamodb-6.0a0/pynamodb/expressions/update.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2476 2024-01-14 03:01:23.000000 pynamodb-6.0a0/pynamodb/expressions/util.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8217 2024-01-14 03:01:23.000000 pynamodb-6.0a0/pynamodb/indexes.py
+-rw-r--r--   0 runner    (1001) docker     (127)    49590 2024-01-14 03:01:23.000000 pynamodb-6.0a0/pynamodb/models.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7356 2024-01-14 03:01:23.000000 pynamodb-6.0a0/pynamodb/pagination.py
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-01-14 03:01:23.000000 pynamodb-6.0a0/pynamodb/py.typed
+-rw-r--r--   0 runner    (1001) docker     (127)     1741 2024-01-14 03:01:23.000000 pynamodb-6.0a0/pynamodb/settings.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1533 2024-01-14 03:01:23.000000 pynamodb-6.0a0/pynamodb/signals.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5595 2024-01-14 03:01:23.000000 pynamodb-6.0a0/pynamodb/transactions.py
+-rw-r--r--   0 runner    (1001) docker     (127)      101 2024-01-14 03:01:23.000000 pynamodb-6.0a0/pynamodb/types.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-14 03:01:44.112251 pynamodb-6.0a0/pynamodb.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     6714 2024-01-14 03:01:44.000000 pynamodb-6.0a0/pynamodb.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     1202 2024-01-14 03:01:44.000000 pynamodb-6.0a0/pynamodb.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-01-14 03:01:44.000000 pynamodb-6.0a0/pynamodb.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-01-14 03:01:43.000000 pynamodb-6.0a0/pynamodb.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (127)       96 2024-01-14 03:01:44.000000 pynamodb-6.0a0/pynamodb.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        9 2024-01-14 03:01:44.000000 pynamodb-6.0a0/pynamodb.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      166 2024-01-14 03:01:23.000000 pynamodb-6.0a0/requirements-dev.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      101 2024-01-14 03:01:44.116251 pynamodb-6.0a0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)     1382 2024-01-14 03:01:23.000000 pynamodb-6.0a0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-14 03:01:44.112251 pynamodb-6.0a0/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)    50686 2024-01-14 03:01:23.000000 pynamodb-6.0a0/tests/test_attributes.py
+-rw-r--r--   0 runner    (1001) docker     (127)    54302 2024-01-14 03:01:23.000000 pynamodb-6.0a0/tests/test_base_connection.py
+-rw-r--r--   0 runner    (1001) docker     (127)      466 2024-01-14 03:01:23.000000 pynamodb-6.0a0/tests/test_binary_legacy_encoding.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6828 2024-01-14 03:01:23.000000 pynamodb-6.0a0/tests/test_discriminator.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1155 2024-01-14 03:01:23.000000 pynamodb-6.0a0/tests/test_exceptions.py
+-rw-r--r--   0 runner    (1001) docker     (127)    30876 2024-01-14 03:01:23.000000 pynamodb-6.0a0/tests/test_expressions.py
+-rw-r--r--   0 runner    (1001) docker     (127)   127499 2024-01-14 03:01:23.000000 pynamodb-6.0a0/tests/test_model.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2078 2024-01-14 03:01:23.000000 pynamodb-6.0a0/tests/test_pagination.py
+-rw-r--r--   0 runner    (1001) docker     (127)      643 2024-01-14 03:01:23.000000 pynamodb-6.0a0/tests/test_settings.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3788 2024-01-14 03:01:23.000000 pynamodb-6.0a0/tests/test_signals.py
+-rw-r--r--   0 runner    (1001) docker     (127)    20252 2024-01-14 03:01:23.000000 pynamodb-6.0a0/tests/test_table_connection.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4551 2024-01-14 03:01:23.000000 pynamodb-6.0a0/tests/test_transaction.py
```

### Comparing `pynamodb-6.0.1/LICENSE` & `pynamodb-6.0a0/LICENSE`

 * *Files identical despite different names*

### Comparing `pynamodb-6.0.1/PKG-INFO` & `pynamodb-6.0a0/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pynamodb
-Version: 6.0.1
+Version: 6.0a0
 Summary: A Pythonic Interface to DynamoDB
 Home-page: http://jlafon.io/pynamodb.html
 Author: Jharrod LaFon
 Author-email: jlafon@eyesopen.com
 License: MIT
 Project-URL: Source, https://github.com/pynamodb/PynamoDB
 Keywords: python dynamodb amazon
```

### Comparing `pynamodb-6.0.1/README.rst` & `pynamodb-6.0a0/README.rst`

 * *Files identical despite different names*

### Comparing `pynamodb-6.0.1/pynamodb/_schema.py` & `pynamodb-6.0a0/pynamodb/_schema.py`

 * *Files identical despite different names*

### Comparing `pynamodb-6.0.1/pynamodb/_util.py` & `pynamodb-6.0a0/pynamodb/_util.py`

 * *Files identical despite different names*

### Comparing `pynamodb-6.0.1/pynamodb/attributes.py` & `pynamodb-6.0a0/pynamodb/attributes.py`

 * *Files 0% similar despite different names*

```diff
@@ -925,15 +925,15 @@
     MapAttribute behave differently based both on where they are instantiated and on their type.
     Because of this complicated behavior, a bit of an introduction is warranted.
 
     Models that contain a MapAttribute define its properties using a class attribute on the model.
     For example, below we define "MyModel" which contains a MapAttribute "my_map":
 
     class MyModel(Model):
-       my_map = MapAttribute(attr_name="dynamo_name", default=dict)
+       my_map = MapAttribute(attr_name="dynamo_name", default={})
 
     When instantiated in this manner (as a class attribute of an AttributeContainer class), the MapAttribute
     class acts as an instance of the Attribute class. The instance stores data about the attribute (in this
     example the dynamo name and default value), and acts as a data descriptor, storing any value bound to it
     on the `attribute_values` dictionary of the containing instance (in this case an instance of MyModel).
 
     Unlike other Attribute types, the value that gets bound to the containing instance is a new instance of
```

### Comparing `pynamodb-6.0.1/pynamodb/connection/_botocore_private.py` & `pynamodb-6.0a0/pynamodb/connection/_botocore_private.py`

 * *Files identical despite different names*

### Comparing `pynamodb-6.0.1/pynamodb/connection/base.py` & `pynamodb-6.0a0/pynamodb/connection/base.py`

 * *Files 1% similar despite different names*

```diff
@@ -327,17 +327,18 @@
 
     def send_pre_boto_callback(self, operation_name, req_uuid, table_name):
         try:
             pre_dynamodb_send.send(self, operation_name=operation_name, table_name=table_name, req_uuid=req_uuid)
         except Exception:
             log.exception("pre_boto callback threw an exception.")
 
-    def _before_send(self, request, **_) -> None:
+    def _before_sign(self, request, **_) -> None:
         if self._extra_headers is not None:
-            request.headers.update(self._extra_headers)
+            for k, v in self._extra_headers.items():
+                request.headers.add_header(k, v)
 
     def _make_api_call(self, operation_name: str, operation_kwargs: Dict) -> Dict:
         try:
             return self.client._make_api_call(operation_name, operation_kwargs)
         except ClientError as e:
             resp_metadata = e.response.get('ResponseMetadata', {}).get('HTTPHeaders', {})
             cancellation_reasons = e.response.get('CancellationReasons', [])
@@ -352,15 +353,14 @@
                 operation_name,
                 verbose_props,
                 cancellation_reasons=(
                     (
                         CancellationReason(
                             code=d['Code'],
                             message=d.get('Message'),
-                            raw_item=cast(Optional[Dict[str, Dict[str, Any]]], d.get('Item')),
                         ) if d['Code'] != 'None' else None
                     )
                     for d in cancellation_reasons
                 ),
             ) from e
 
     def _get_table_name_for_error_context(self, operation_kwargs) -> str:
@@ -407,15 +407,15 @@
                 retries={
                     'total_max_attempts': 1 + self._max_retry_attempts_exception,
                     'mode': 'standard',
                 }
             )
             self._client = cast(BotocoreBaseClientPrivate, self.session.create_client(SERVICE_NAME, self.region, endpoint_url=self.host, config=config))
 
-            self._client.meta.events.register_first('before-send.*.*', self._before_send)
+            self._client.meta.events.register_first('before-sign.*.*', self._before_sign)
         return self._client
 
     def add_meta_table(self, meta_table: MetaTable) -> None:
         """
         Adds information about the table's schema.
         """
         if meta_table.table_name in self._tables:
```

### Comparing `pynamodb-6.0.1/pynamodb/connection/table.py` & `pynamodb-6.0a0/pynamodb/connection/table.py`

 * *Files identical despite different names*

### Comparing `pynamodb-6.0.1/pynamodb/constants.py` & `pynamodb-6.0a0/pynamodb/constants.py`

 * *Files identical despite different names*

### Comparing `pynamodb-6.0.1/pynamodb/exceptions.py` & `pynamodb-6.0a0/pynamodb/exceptions.py`

 * *Files 2% similar despite different names*

```diff
@@ -130,15 +130,14 @@
     see `TransactGetItems`_ and `TransactWriteItems`_ in the AWS documentation.
 
     .. _TransactGetItems: https://docs.aws.amazon.com/amazondynamodb/latest/APIReference/API_TransactGetItems.html
     .. _TransactWriteItems: https://docs.aws.amazon.com/amazondynamodb/latest/APIReference/API_TransactWriteItems.html
     """
     code: str
     message: Optional[str] = None
-    raw_item: Optional[Dict[str, Dict[str, Any]]] = None
 
 
 class TransactWriteError(PynamoDBException):
     """
     Raised when a :class:`~pynamodb.transactions.TransactWrite` operation fails.
     """
```

### Comparing `pynamodb-6.0.1/pynamodb/expressions/condition.py` & `pynamodb-6.0a0/pynamodb/expressions/condition.py`

 * *Files identical despite different names*

### Comparing `pynamodb-6.0.1/pynamodb/expressions/operand.py` & `pynamodb-6.0a0/pynamodb/expressions/operand.py`

 * *Files identical despite different names*

### Comparing `pynamodb-6.0.1/pynamodb/expressions/projection.py` & `pynamodb-6.0a0/pynamodb/expressions/projection.py`

 * *Files identical despite different names*

### Comparing `pynamodb-6.0.1/pynamodb/expressions/update.py` & `pynamodb-6.0a0/pynamodb/expressions/update.py`

 * *Files identical despite different names*

### Comparing `pynamodb-6.0.1/pynamodb/expressions/util.py` & `pynamodb-6.0a0/pynamodb/expressions/util.py`

 * *Files identical despite different names*

### Comparing `pynamodb-6.0.1/pynamodb/indexes.py` & `pynamodb-6.0a0/pynamodb/indexes.py`

 * *Files identical despite different names*

### Comparing `pynamodb-6.0.1/pynamodb/models.py` & `pynamodb-6.0a0/pynamodb/models.py`

 * *Files identical despite different names*

### Comparing `pynamodb-6.0.1/pynamodb/pagination.py` & `pynamodb-6.0a0/pynamodb/pagination.py`

 * *Files identical despite different names*

### Comparing `pynamodb-6.0.1/pynamodb/settings.py` & `pynamodb-6.0a0/pynamodb/settings.py`

 * *Files identical despite different names*

### Comparing `pynamodb-6.0.1/pynamodb/signals.py` & `pynamodb-6.0a0/pynamodb/signals.py`

 * *Files identical despite different names*

### Comparing `pynamodb-6.0.1/pynamodb/transactions.py` & `pynamodb-6.0a0/pynamodb/transactions.py`

 * *Files identical despite different names*

### Comparing `pynamodb-6.0.1/pynamodb.egg-info/PKG-INFO` & `pynamodb-6.0a0/pynamodb.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pynamodb
-Version: 6.0.1
+Version: 6.0a0
 Summary: A Pythonic Interface to DynamoDB
 Home-page: http://jlafon.io/pynamodb.html
 Author: Jharrod LaFon
 Author-email: jlafon@eyesopen.com
 License: MIT
 Project-URL: Source, https://github.com/pynamodb/PynamoDB
 Keywords: python dynamodb amazon
```

### Comparing `pynamodb-6.0.1/pynamodb.egg-info/SOURCES.txt` & `pynamodb-6.0a0/pynamodb.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `pynamodb-6.0.1/setup.py` & `pynamodb-6.0a0/setup.py`

 * *Files identical despite different names*

### Comparing `pynamodb-6.0.1/tests/test_attributes.py` & `pynamodb-6.0a0/tests/test_attributes.py`

 * *Files identical despite different names*

### Comparing `pynamodb-6.0.1/tests/test_base_connection.py` & `pynamodb-6.0a0/tests/test_base_connection.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,26 +1,22 @@
 """
 Tests for the base connection class
 """
 import base64
 import json
-from datetime import datetime
-from uuid import UUID
-
 import urllib3
 from unittest import mock
 from unittest.mock import patch
 
 import botocore.exceptions
 from botocore.awsrequest import AWSResponse
 from botocore.client import ClientError
 from botocore.exceptions import BotoCoreError
 
 import pytest
-from freezegun import freeze_time
 
 from pynamodb.connection import Connection
 from pynamodb.connection.base import MetaTable
 from pynamodb.exceptions import (
     TableError, DeleteError, PutError, ScanError, GetError, UpdateError, TableDoesNotExist, VerboseClientError)
 from pynamodb.constants import (
     UNPROCESSED_ITEMS, STRING, BINARY, DEFAULT_ENCODING, TABLE_KEY,
@@ -1515,42 +1511,29 @@
 def test_connection__botocore_config():
     c = Connection(connect_timeout_seconds=5, read_timeout_seconds=10, max_pool_connections=20)
     assert c.client._client_config.connect_timeout == 5
     assert c.client._client_config.read_timeout == 10
     assert c.client._client_config.max_pool_connections == 20
 
 
-@freeze_time()
-def test_connection_make_api_call___extra_headers(mocker):
+@mock.patch('botocore.httpsession.URLLib3Session.send')
+def test_connection_make_api_call___extra_headers(send_mock):
     good_response = mock.Mock(spec=AWSResponse, status_code=200, headers={}, text='{}', content=b'{}')
-    send_mock = mocker.patch('botocore.httpsession.URLLib3Session.send', return_value=good_response)
 
-    # return constant UUID
-    mocker.patch('uuid.uuid4', return_value=UUID('01FC4BDB-B223-4B86-88F4-DEE79B77F275'))
+    send_mock.return_value = good_response
 
     c = Connection(extra_headers={'foo': 'bar'}, max_retry_attempts=0)
     c._make_api_call(
         'DescribeTable',
         {'TableName': 'MyTable'},
     )
 
     assert send_mock.call_count == 1
     request = send_mock.call_args[0][0]
-    assert request.headers['foo'] == 'bar'
-
-    c = Connection(extra_headers={'foo': 'baz'}, max_retry_attempts=0)
-    c._make_api_call(
-        'DescribeTable',
-        {'TableName': 'MyTable'},
-    )
-
-    assert send_mock.call_count == 2
-    request2 = send_mock.call_args[0][0]
-    # all headers, including signatures, and except 'foo', should match
-    assert {**request.headers, 'foo': ''} == {**request2.headers, 'foo': ''}
+    assert request.headers.get('foo').decode() == 'bar'
 
 
 @mock.patch('botocore.httpsession.URLLib3Session.send')
 def test_connection_make_api_call__throws_when_retries_exhausted(send_mock):
     send_mock.side_effect = [
         botocore.exceptions.ConnectionError(error="problems"),
         botocore.exceptions.ConnectionError(error="problems"),
```

### Comparing `pynamodb-6.0.1/tests/test_discriminator.py` & `pynamodb-6.0a0/tests/test_discriminator.py`

 * *Files identical despite different names*

### Comparing `pynamodb-6.0.1/tests/test_exceptions.py` & `pynamodb-6.0a0/tests/test_exceptions.py`

 * *Files identical despite different names*

### Comparing `pynamodb-6.0.1/tests/test_expressions.py` & `pynamodb-6.0a0/tests/test_expressions.py`

 * *Files identical despite different names*

### Comparing `pynamodb-6.0.1/tests/test_model.py` & `pynamodb-6.0a0/tests/test_model.py`

 * *Files identical despite different names*

### Comparing `pynamodb-6.0.1/tests/test_pagination.py` & `pynamodb-6.0a0/tests/test_pagination.py`

 * *Files identical despite different names*

### Comparing `pynamodb-6.0.1/tests/test_settings.py` & `pynamodb-6.0a0/tests/test_settings.py`

 * *Files identical despite different names*

### Comparing `pynamodb-6.0.1/tests/test_signals.py` & `pynamodb-6.0a0/tests/test_signals.py`

 * *Files identical despite different names*

### Comparing `pynamodb-6.0.1/tests/test_table_connection.py` & `pynamodb-6.0a0/tests/test_table_connection.py`

 * *Files identical despite different names*

### Comparing `pynamodb-6.0.1/tests/test_transaction.py` & `pynamodb-6.0a0/tests/test_transaction.py`

 * *Files identical despite different names*

