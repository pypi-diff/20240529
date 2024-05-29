# Comparing `tmp/nhs_aws_helpers-0.7.3.tar.gz` & `tmp/nhs_aws_helpers-0.7.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "nhs_aws_helpers-0.7.3.tar", max compression
+gzip compressed data, was "nhs_aws_helpers-0.7.4.tar", max compression
```

## Comparing `nhs_aws_helpers-0.7.3.tar` & `nhs_aws_helpers-0.7.4.tar`

### file list

```diff
@@ -1,25 +1,25 @@
--rw-r--r--   0        0        0     1078 2024-02-14 13:41:42.449296 nhs_aws_helpers-0.7.3/LICENSE.md
--rw-r--r--   0        0        0      783 2024-02-14 13:41:42.449296 nhs_aws_helpers-0.7.3/README.md
--rw-r--r--   0        0        0    38664 2024-02-14 13:41:42.449296 nhs_aws_helpers-0.7.3/nhs_aws_helpers/__init__.py
--rw-r--r--   0        0        0     7970 2024-02-14 13:41:42.449296 nhs_aws_helpers-0.7.3/nhs_aws_helpers/async_s3_object_reader.py
--rw-r--r--   0        0        0     6709 2024-02-14 13:41:42.449296 nhs_aws_helpers-0.7.3/nhs_aws_helpers/async_s3_object_writer.py
--rw-r--r--   0        0        0     1388 2024-02-14 13:41:42.449296 nhs_aws_helpers-0.7.3/nhs_aws_helpers/common.py
--rw-r--r--   0        0        0        0 2024-02-14 13:41:42.449296 nhs_aws_helpers-0.7.3/nhs_aws_helpers/dynamodb_model_store/__init__.py
--rw-r--r--   0        0        0     1978 2024-02-14 13:41:42.449296 nhs_aws_helpers-0.7.3/nhs_aws_helpers/dynamodb_model_store/base_model.py
--rw-r--r--   0        0        0    27724 2024-02-14 13:41:42.449296 nhs_aws_helpers-0.7.3/nhs_aws_helpers/dynamodb_model_store/base_model_store.py
--rw-r--r--   0        0        0     5463 2024-02-14 13:41:42.449296 nhs_aws_helpers-0.7.3/nhs_aws_helpers/fixtures.py
--rw-r--r--   0        0        0        0 2024-02-14 13:41:42.449296 nhs_aws_helpers-0.7.3/nhs_aws_helpers/py.typed
--rw-r--r--   0        0        0     7903 2024-02-14 13:41:42.449296 nhs_aws_helpers-0.7.3/nhs_aws_helpers/s3_object_reader.py
--rw-r--r--   0        0        0     6712 2024-02-14 13:41:42.449296 nhs_aws_helpers-0.7.3/nhs_aws_helpers/s3_object_writer.py
--rw-r--r--   0        0        0     3671 2024-02-14 13:41:55.673393 nhs_aws_helpers-0.7.3/pyproject.toml
--rw-r--r--   0        0        0        0 2024-02-14 13:41:42.453296 nhs_aws_helpers-0.7.3/tests/__init__.py
--rw-r--r--   0        0        0    11155 2024-02-14 13:41:42.453296 nhs_aws_helpers-0.7.3/tests/async_s3_object_buffer_tests.py
--rw-r--r--   0        0        0     7756 2024-02-14 13:41:42.453296 nhs_aws_helpers-0.7.3/tests/aws_tests.py
--rw-r--r--   0        0        0    25240 2024-02-14 13:41:42.453296 nhs_aws_helpers-0.7.3/tests/base_model_store_tests.py
--rw-r--r--   0        0        0      312 2024-02-14 13:41:42.453296 nhs_aws_helpers-0.7.3/tests/conftest.py
--rw-r--r--   0        0        0     2231 2024-02-14 13:41:42.453296 nhs_aws_helpers-0.7.3/tests/ddb_tests.py
--rw-r--r--   0        0        0     2590 2024-02-14 13:41:42.453296 nhs_aws_helpers-0.7.3/tests/fixtures_tests.py
--rw-r--r--   0        0        0    10156 2024-02-14 13:41:42.453296 nhs_aws_helpers-0.7.3/tests/s3_object_buffer_tests.py
--rw-r--r--   0        0        0      665 2024-02-14 13:41:42.453296 nhs_aws_helpers-0.7.3/tests/test_helpers.py
--rw-r--r--   0        0        0      518 2024-02-14 13:41:42.453296 nhs_aws_helpers-0.7.3/tests/utils.py
--rw-r--r--   0        0        0     1635 1970-01-01 00:00:00.000000 nhs_aws_helpers-0.7.3/PKG-INFO
+-rw-r--r--   0        0        0     1078 2024-05-23 08:14:03.187562 nhs_aws_helpers-0.7.4/LICENSE.md
+-rw-r--r--   0        0        0      783 2024-05-23 08:14:03.187562 nhs_aws_helpers-0.7.4/README.md
+-rw-r--r--   0        0        0    38881 2024-05-23 08:14:03.187562 nhs_aws_helpers-0.7.4/nhs_aws_helpers/__init__.py
+-rw-r--r--   0        0        0     7970 2024-05-23 08:14:03.187562 nhs_aws_helpers-0.7.4/nhs_aws_helpers/async_s3_object_reader.py
+-rw-r--r--   0        0        0     6709 2024-05-23 08:14:03.187562 nhs_aws_helpers-0.7.4/nhs_aws_helpers/async_s3_object_writer.py
+-rw-r--r--   0        0        0     1388 2024-05-23 08:14:03.187562 nhs_aws_helpers-0.7.4/nhs_aws_helpers/common.py
+-rw-r--r--   0        0        0        0 2024-05-23 08:14:03.187562 nhs_aws_helpers-0.7.4/nhs_aws_helpers/dynamodb_model_store/__init__.py
+-rw-r--r--   0        0        0     1978 2024-05-23 08:14:03.187562 nhs_aws_helpers-0.7.4/nhs_aws_helpers/dynamodb_model_store/base_model.py
+-rw-r--r--   0        0        0    27736 2024-05-23 08:14:03.187562 nhs_aws_helpers-0.7.4/nhs_aws_helpers/dynamodb_model_store/base_model_store.py
+-rw-r--r--   0        0        0     5463 2024-05-23 08:14:03.187562 nhs_aws_helpers-0.7.4/nhs_aws_helpers/fixtures.py
+-rw-r--r--   0        0        0        0 2024-05-23 08:14:03.187562 nhs_aws_helpers-0.7.4/nhs_aws_helpers/py.typed
+-rw-r--r--   0        0        0     7903 2024-05-23 08:14:03.187562 nhs_aws_helpers-0.7.4/nhs_aws_helpers/s3_object_reader.py
+-rw-r--r--   0        0        0     6712 2024-05-23 08:14:03.187562 nhs_aws_helpers-0.7.4/nhs_aws_helpers/s3_object_writer.py
+-rw-r--r--   0        0        0     3674 2024-05-23 08:14:19.011414 nhs_aws_helpers-0.7.4/pyproject.toml
+-rw-r--r--   0        0        0        0 2024-05-23 08:14:03.191562 nhs_aws_helpers-0.7.4/tests/__init__.py
+-rw-r--r--   0        0        0    11155 2024-05-23 08:14:03.191562 nhs_aws_helpers-0.7.4/tests/async_s3_object_buffer_tests.py
+-rw-r--r--   0        0        0     7756 2024-05-23 08:14:03.191562 nhs_aws_helpers-0.7.4/tests/aws_tests.py
+-rw-r--r--   0        0        0    25240 2024-05-23 08:14:03.191562 nhs_aws_helpers-0.7.4/tests/base_model_store_tests.py
+-rw-r--r--   0        0        0      312 2024-05-23 08:14:03.191562 nhs_aws_helpers-0.7.4/tests/conftest.py
+-rw-r--r--   0        0        0     2231 2024-05-23 08:14:03.191562 nhs_aws_helpers-0.7.4/tests/ddb_tests.py
+-rw-r--r--   0        0        0     2590 2024-05-23 08:14:03.191562 nhs_aws_helpers-0.7.4/tests/fixtures_tests.py
+-rw-r--r--   0        0        0    10156 2024-05-23 08:14:03.191562 nhs_aws_helpers-0.7.4/tests/s3_object_buffer_tests.py
+-rw-r--r--   0        0        0      665 2024-05-23 08:14:03.191562 nhs_aws_helpers-0.7.4/tests/test_helpers.py
+-rw-r--r--   0        0        0      518 2024-05-23 08:14:03.191562 nhs_aws_helpers-0.7.4/tests/utils.py
+-rw-r--r--   0        0        0     1639 1970-01-01 00:00:00.000000 nhs_aws_helpers-0.7.4/PKG-INFO
```

### Comparing `nhs_aws_helpers-0.7.3/LICENSE.md` & `nhs_aws_helpers-0.7.4/LICENSE.md`

 * *Files identical despite different names*

### Comparing `nhs_aws_helpers-0.7.3/README.md` & `nhs_aws_helpers-0.7.4/README.md`

 * *Files identical despite different names*

### Comparing `nhs_aws_helpers-0.7.3/nhs_aws_helpers/__init__.py` & `nhs_aws_helpers-0.7.4/nhs_aws_helpers/__init__.py`

 * *Files 0% similar despite different names*

```diff
@@ -65,14 +65,15 @@
     CompletedPartTypeDef,
     DeleteMarkerEntryTypeDef,
     DeleteTypeDef,
     GetObjectOutputTypeDef,
     ObjectVersionTypeDef,
 )
 from mypy_boto3_secretsmanager.client import SecretsManagerClient
+from mypy_boto3_ses import SESClient
 from mypy_boto3_sns.client import SNSClient
 from mypy_boto3_sqs import SQSServiceResource
 from mypy_boto3_sqs.client import SQSClient
 from mypy_boto3_ssm.client import SSMClient
 from mypy_boto3_stepfunctions import SFNClient
 
 from nhs_aws_helpers.common import run_in_executor
@@ -279,14 +280,18 @@
     return _aws("dynamodb", "client", session, config)  # type: ignore[no-any-return]
 
 
 def ddb_table(table_name: str, session: Optional[Session] = None, config: Optional[Config] = None) -> Table:
     return dynamodb(session=session, config=config).Table(table_name)
 
 
+def ses_client(session: Optional[Session] = None, config: Optional[Config] = None) -> SESClient:
+    return _aws("ses", "client", session, config)  # type: ignore[no-any-return]
+
+
 def sqs_client(session: Optional[Session] = None, config: Optional[Config] = None) -> SQSClient:
     return _aws("sqs", "client", session, config)  # type: ignore[no-any-return]
 
 
 def sqs_resource(session: Optional[Session] = None, config: Optional[Config] = None) -> SQSServiceResource:
     return _aws("sqs", "resource", session, config)  # type: ignore[no-any-return]
```

### Comparing `nhs_aws_helpers-0.7.3/nhs_aws_helpers/async_s3_object_reader.py` & `nhs_aws_helpers-0.7.4/nhs_aws_helpers/async_s3_object_reader.py`

 * *Files identical despite different names*

### Comparing `nhs_aws_helpers-0.7.3/nhs_aws_helpers/async_s3_object_writer.py` & `nhs_aws_helpers-0.7.4/nhs_aws_helpers/async_s3_object_writer.py`

 * *Files identical despite different names*

### Comparing `nhs_aws_helpers-0.7.3/nhs_aws_helpers/common.py` & `nhs_aws_helpers-0.7.4/nhs_aws_helpers/common.py`

 * *Files identical despite different names*

### Comparing `nhs_aws_helpers-0.7.3/nhs_aws_helpers/dynamodb_model_store/base_model.py` & `nhs_aws_helpers-0.7.4/nhs_aws_helpers/dynamodb_model_store/base_model.py`

 * *Files identical despite different names*

### Comparing `nhs_aws_helpers-0.7.3/nhs_aws_helpers/dynamodb_model_store/base_model_store.py` & `nhs_aws_helpers-0.7.4/nhs_aws_helpers/dynamodb_model_store/base_model_store.py`

 * *Files 0% similar despite different names*

```diff
@@ -27,15 +27,15 @@
 from mypy_boto3_dynamodb import DynamoDBClient
 from mypy_boto3_dynamodb.service_resource import DynamoDBServiceResource, Table
 from mypy_boto3_dynamodb.type_defs import (
     BatchGetItemOutputServiceResourceTypeDef,
     QueryOutputTableTypeDef,
     TransactGetItemTypeDef,
     UpdateItemOutputTableTypeDef,
-    WriteRequestTypeDef,
+    WriteRequestOutputTypeDef,
 )
 
 from nhs_aws_helpers import dynamodb, dynamodb_retry_backoff
 from nhs_aws_helpers.common import (
     is_dataclass_instance,
     optional_origin_type,
     run_in_executor,
@@ -680,15 +680,15 @@
     converted from boto3.dynamodb.BatchWriter to be async
     """
 
     def __init__(self, store: BaseModelStore, flush_amount=25):
         self._store = store
         self._table_name = store.table.table_name
         self._client = store.client
-        self._items_buffer: List[WriteRequestTypeDef] = []
+        self._items_buffer: List[WriteRequestOutputTypeDef] = []
         self._flush_amount = flush_amount
         self._overwrite_by_keys = store.table_key_fields
 
     async def put_item(self, item, **kwargs):
         await self._add_request_and_process({"PutRequest": {"Item": self._store.serialise_value(item, **kwargs)}})
 
     async def delete_item(self, key, **kwargs):
```

### Comparing `nhs_aws_helpers-0.7.3/nhs_aws_helpers/fixtures.py` & `nhs_aws_helpers-0.7.4/nhs_aws_helpers/fixtures.py`

 * *Files identical despite different names*

### Comparing `nhs_aws_helpers-0.7.3/nhs_aws_helpers/s3_object_reader.py` & `nhs_aws_helpers-0.7.4/nhs_aws_helpers/s3_object_reader.py`

 * *Files identical despite different names*

### Comparing `nhs_aws_helpers-0.7.3/nhs_aws_helpers/s3_object_writer.py` & `nhs_aws_helpers-0.7.4/nhs_aws_helpers/s3_object_writer.py`

 * *Files identical despite different names*

### Comparing `nhs_aws_helpers-0.7.3/pyproject.toml` & `nhs_aws_helpers-0.7.4/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,25 +1,25 @@
 [tool.poetry]
 name = "nhs_aws_helpers"
-version = "0.7.3"
+version = "0.7.4"
 description = ""
 authors = ["spinecore"]
 license = "MIT"
 packages = [
     { include = "nhs_aws_helpers" },
     { include = "tests", format = "sdist" },
 ]
 readme = "README.md"
 repository = "https://github.com/NHSDigital/nhs-aws-helpers"
 
 [tool.poetry.dependencies]
 # core dependencies
 python = ">=3.8,<4.0"
 boto3 = "^1.26.159"
-boto3-stubs = {extras = ["s3", "ssm", "secretsmanager", "dynamodb", "stepfunctions", "sqs", "lambda", "logs", "sns", "events", "kms", "firehose", "athena"], version = ">=1.28.0,^1.28.36"}
+boto3-stubs = {extras = ["s3", "ssm", "secretsmanager", "dynamodb", "stepfunctions", "sqs", "lambda", "logs", "ses", "sns", "events", "kms", "firehose", "athena"], version = ">=1.28.0,^1.28.36"}
 botocore-stubs = "^1.29.159"
 
 
 [tool.setuptools.package-data]
 "nhs_aws_helpers" = ["py.typed"]
 
 [tool.poetry.group.dev.dependencies]
@@ -28,15 +28,15 @@
 black = "^24.1.1"
 mypy = "^1.4.0"
 coverage = "^7.2.7"
 pytest = "^7.3.1"
 pytest-asyncio = "^0.23.4"
 tox = "^4.6.3"
 pytest-httpserver = "^1.0.8"
-ruff = "^0.2.0"
+ruff = "^0"
 
 
 [tool.poetry.group.local.dependencies]
 ipython = "^8.12.2"
 
 [tool.poetry.extras]
 pytest = ["pytest", "petname"]
```

### Comparing `nhs_aws_helpers-0.7.3/tests/async_s3_object_buffer_tests.py` & `nhs_aws_helpers-0.7.4/tests/async_s3_object_buffer_tests.py`

 * *Files identical despite different names*

### Comparing `nhs_aws_helpers-0.7.3/tests/aws_tests.py` & `nhs_aws_helpers-0.7.4/tests/aws_tests.py`

 * *Files identical despite different names*

### Comparing `nhs_aws_helpers-0.7.3/tests/base_model_store_tests.py` & `nhs_aws_helpers-0.7.4/tests/base_model_store_tests.py`

 * *Files identical despite different names*

### Comparing `nhs_aws_helpers-0.7.3/tests/ddb_tests.py` & `nhs_aws_helpers-0.7.4/tests/ddb_tests.py`

 * *Files identical despite different names*

### Comparing `nhs_aws_helpers-0.7.3/tests/fixtures_tests.py` & `nhs_aws_helpers-0.7.4/tests/fixtures_tests.py`

 * *Files identical despite different names*

### Comparing `nhs_aws_helpers-0.7.3/tests/s3_object_buffer_tests.py` & `nhs_aws_helpers-0.7.4/tests/s3_object_buffer_tests.py`

 * *Files identical despite different names*

### Comparing `nhs_aws_helpers-0.7.3/tests/test_helpers.py` & `nhs_aws_helpers-0.7.4/tests/test_helpers.py`

 * *Files identical despite different names*

### Comparing `nhs_aws_helpers-0.7.3/tests/utils.py` & `nhs_aws_helpers-0.7.4/tests/utils.py`

 * *Files identical despite different names*

### Comparing `nhs_aws_helpers-0.7.3/PKG-INFO` & `nhs_aws_helpers-0.7.4/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,24 +1,24 @@
 Metadata-Version: 2.1
 Name: nhs-aws-helpers
-Version: 0.7.3
+Version: 0.7.4
 Summary: 
 Home-page: https://github.com/NHSDigital/nhs-aws-helpers
 License: MIT
 Author: spinecore
 Requires-Python: >=3.8,<4.0
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Provides-Extra: pytest
 Requires-Dist: boto3 (>=1.26.159,<2.0.0)
-Requires-Dist: boto3-stubs[athena,dynamodb,events,firehose,kms,lambda,logs,s3,secretsmanager,sns,sqs,ssm,stepfunctions] (>=1.28.36,<2.0.0)
+Requires-Dist: boto3-stubs[athena,dynamodb,events,firehose,kms,lambda,logs,s3,secretsmanager,ses,sns,sqs,ssm,stepfunctions] (>=1.28.36,<2.0.0)
 Requires-Dist: botocore-stubs (>=1.29.159,<2.0.0)
 Project-URL: Repository, https://github.com/NHSDigital/nhs-aws-helpers
 Description-Content-Type: text/markdown
 
 # NHS AWS Helpers
 
 some useful boto3 utilities
```

