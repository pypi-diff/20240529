# Comparing `tmp/pysqream-blue-1.0.46.tar.gz` & `tmp/pysqream-blue-1.0.47.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pysqream-blue-1.0.46.tar", last modified: Sun Apr 14 14:46:33 2024, max compression
+gzip compressed data, was "pysqream-blue-1.0.47.tar", last modified: Wed May 29 08:01:20 2024, max compression
```

## Comparing `pysqream-blue-1.0.46.tar` & `pysqream-blue-1.0.47.tar`

### file list

```diff
@@ -1,33 +1,33 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-14 14:46:33.751053 pysqream-blue-1.0.46/
--rw-r--r--   0 runner    (1001) docker     (127)     1519 2024-04-14 14:46:17.000000 pysqream-blue-1.0.46/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)     6518 2024-04-14 14:46:33.751053 pysqream-blue-1.0.46/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     6060 2024-04-14 14:46:17.000000 pysqream-blue-1.0.46/README.rst
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-14 14:46:33.751053 pysqream-blue-1.0.46/protos/
--rw-r--r--   0 runner    (1001) docker     (127)     5619 2024-04-14 14:46:17.000000 pysqream-blue-1.0.46/protos/authentication_pb2.py
--rw-r--r--   0 runner    (1001) docker     (127)     6018 2024-04-14 14:46:17.000000 pysqream-blue-1.0.46/protos/authentication_pb2_grpc.py
--rw-r--r--   0 runner    (1001) docker     (127)     1420 2024-04-14 14:46:17.000000 pysqream-blue-1.0.46/protos/authentication_type_pb2.py
--rw-r--r--   0 runner    (1001) docker     (127)      159 2024-04-14 14:46:17.000000 pysqream-blue-1.0.46/protos/authentication_type_pb2_grpc.py
--rw-r--r--   0 runner    (1001) docker     (127)     1980 2024-04-14 14:46:17.000000 pysqream-blue-1.0.46/protos/client_info_pb2.py
--rw-r--r--   0 runner    (1001) docker     (127)      159 2024-04-14 14:46:17.000000 pysqream-blue-1.0.46/protos/client_info_pb2_grpc.py
--rw-r--r--   0 runner    (1001) docker     (127)     1284 2024-04-14 14:46:17.000000 pysqream-blue-1.0.46/protos/error_pb2.py
--rw-r--r--   0 runner    (1001) docker     (127)      159 2024-04-14 14:46:17.000000 pysqream-blue-1.0.46/protos/error_pb2_grpc.py
--rw-r--r--   0 runner    (1001) docker     (127)    15292 2024-04-14 14:46:17.000000 pysqream-blue-1.0.46/protos/queryhandler_pb2.py
--rw-r--r--   0 runner    (1001) docker     (127)    12578 2024-04-14 14:46:17.000000 pysqream-blue-1.0.46/protos/queryhandler_pb2_grpc.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-14 14:46:33.751053 pysqream-blue-1.0.46/pysqream_blue/
--rw-r--r--   0 runner    (1001) docker     (127)      157 2024-04-14 14:46:17.000000 pysqream-blue-1.0.46/pysqream_blue/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     7116 2024-04-14 14:46:17.000000 pysqream-blue-1.0.46/pysqream_blue/array_parser.py
--rw-r--r--   0 runner    (1001) docker     (127)     2174 2024-04-14 14:46:17.000000 pysqream-blue-1.0.46/pysqream_blue/casting.py
--rw-r--r--   0 runner    (1001) docker     (127)    12200 2024-04-14 14:46:17.000000 pysqream-blue-1.0.46/pysqream_blue/connection.py
--rw-r--r--   0 runner    (1001) docker     (127)    18099 2024-04-14 14:46:17.000000 pysqream-blue-1.0.46/pysqream_blue/cursor.py
--rw-r--r--   0 runner    (1001) docker     (127)     3102 2024-04-14 14:46:17.000000 pysqream-blue-1.0.46/pysqream_blue/globals.py
--rw-r--r--   0 runner    (1001) docker     (127)     2886 2024-04-14 14:46:17.000000 pysqream-blue-1.0.46/pysqream_blue/logger.py
--rwxr-xr-x   0 runner    (1001) docker     (127)     3237 2024-04-14 14:46:17.000000 pysqream-blue-1.0.46/pysqream_blue/pysqream_blue.py
--rw-r--r--   0 runner    (1001) docker     (127)      523 2024-04-14 14:46:17.000000 pysqream-blue-1.0.46/pysqream_blue/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-14 14:46:33.751053 pysqream-blue-1.0.46/pysqream_blue.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     6518 2024-04-14 14:46:33.000000 pysqream-blue-1.0.46/pysqream_blue.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      744 2024-04-14 14:46:33.000000 pysqream-blue-1.0.46/pysqream_blue.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-14 14:46:33.000000 pysqream-blue-1.0.46/pysqream_blue.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)      135 2024-04-14 14:46:33.000000 pysqream-blue-1.0.46/pysqream_blue.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       21 2024-04-14 14:46:33.000000 pysqream-blue-1.0.46/pysqream_blue.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-14 14:46:33.751053 pysqream-blue-1.0.46/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)      983 2024-04-14 14:46:17.000000 pysqream-blue-1.0.46/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-29 08:01:20.411144 pysqream-blue-1.0.47/
+-rw-r--r--   0 runner    (1001) docker     (127)     1519 2024-05-29 08:01:00.000000 pysqream-blue-1.0.47/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)     6518 2024-05-29 08:01:20.411144 pysqream-blue-1.0.47/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     6060 2024-05-29 08:01:00.000000 pysqream-blue-1.0.47/README.rst
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-29 08:01:20.411144 pysqream-blue-1.0.47/protos/
+-rw-r--r--   0 runner    (1001) docker     (127)     5619 2024-05-29 08:01:00.000000 pysqream-blue-1.0.47/protos/authentication_pb2.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6018 2024-05-29 08:01:00.000000 pysqream-blue-1.0.47/protos/authentication_pb2_grpc.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1420 2024-05-29 08:01:00.000000 pysqream-blue-1.0.47/protos/authentication_type_pb2.py
+-rw-r--r--   0 runner    (1001) docker     (127)      159 2024-05-29 08:01:00.000000 pysqream-blue-1.0.47/protos/authentication_type_pb2_grpc.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1980 2024-05-29 08:01:00.000000 pysqream-blue-1.0.47/protos/client_info_pb2.py
+-rw-r--r--   0 runner    (1001) docker     (127)      159 2024-05-29 08:01:00.000000 pysqream-blue-1.0.47/protos/client_info_pb2_grpc.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1284 2024-05-29 08:01:00.000000 pysqream-blue-1.0.47/protos/error_pb2.py
+-rw-r--r--   0 runner    (1001) docker     (127)      159 2024-05-29 08:01:00.000000 pysqream-blue-1.0.47/protos/error_pb2_grpc.py
+-rw-r--r--   0 runner    (1001) docker     (127)    15497 2024-05-29 08:01:00.000000 pysqream-blue-1.0.47/protos/queryhandler_pb2.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12578 2024-05-29 08:01:00.000000 pysqream-blue-1.0.47/protos/queryhandler_pb2_grpc.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-29 08:01:20.411144 pysqream-blue-1.0.47/pysqream_blue/
+-rw-r--r--   0 runner    (1001) docker     (127)      157 2024-05-29 08:01:00.000000 pysqream-blue-1.0.47/pysqream_blue/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7116 2024-05-29 08:01:00.000000 pysqream-blue-1.0.47/pysqream_blue/array_parser.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2174 2024-05-29 08:01:00.000000 pysqream-blue-1.0.47/pysqream_blue/casting.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12200 2024-05-29 08:01:00.000000 pysqream-blue-1.0.47/pysqream_blue/connection.py
+-rw-r--r--   0 runner    (1001) docker     (127)    18549 2024-05-29 08:01:00.000000 pysqream-blue-1.0.47/pysqream_blue/cursor.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3102 2024-05-29 08:01:00.000000 pysqream-blue-1.0.47/pysqream_blue/globals.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2886 2024-05-29 08:01:00.000000 pysqream-blue-1.0.47/pysqream_blue/logger.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)     3237 2024-05-29 08:01:00.000000 pysqream-blue-1.0.47/pysqream_blue/pysqream_blue.py
+-rw-r--r--   0 runner    (1001) docker     (127)      523 2024-05-29 08:01:00.000000 pysqream-blue-1.0.47/pysqream_blue/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-29 08:01:20.411144 pysqream-blue-1.0.47/pysqream_blue.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     6518 2024-05-29 08:01:20.000000 pysqream-blue-1.0.47/pysqream_blue.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      744 2024-05-29 08:01:20.000000 pysqream-blue-1.0.47/pysqream_blue.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-29 08:01:20.000000 pysqream-blue-1.0.47/pysqream_blue.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      135 2024-05-29 08:01:20.000000 pysqream-blue-1.0.47/pysqream_blue.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       21 2024-05-29 08:01:20.000000 pysqream-blue-1.0.47/pysqream_blue.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-29 08:01:20.411144 pysqream-blue-1.0.47/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)      983 2024-05-29 08:01:00.000000 pysqream-blue-1.0.47/setup.py
```

### Comparing `pysqream-blue-1.0.46/LICENSE` & `pysqream-blue-1.0.47/LICENSE`

 * *Files identical despite different names*

### Comparing `pysqream-blue-1.0.46/PKG-INFO` & `pysqream-blue-1.0.47/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pysqream-blue
-Version: 1.0.46
+Version: 1.0.47
 Summary: DB-API connector for SQream DB
 Home-page: https://github.com/SQream/pysqream-blue
 Author: SQream
 Author-email: info@sqream.com
 Keywords: database db-api sqream sqreamdbV2
 Classifier: Programming Language :: Python :: 3.9
 Classifier: License :: OSI Approved :: BSD License
```

### Comparing `pysqream-blue-1.0.46/README.rst` & `pysqream-blue-1.0.47/README.rst`

 * *Files identical despite different names*

### Comparing `pysqream-blue-1.0.46/protos/authentication_pb2.py` & `pysqream-blue-1.0.47/protos/authentication_pb2.py`

 * *Files identical despite different names*

### Comparing `pysqream-blue-1.0.46/protos/authentication_pb2_grpc.py` & `pysqream-blue-1.0.47/protos/authentication_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `pysqream-blue-1.0.46/protos/authentication_type_pb2.py` & `pysqream-blue-1.0.47/protos/authentication_type_pb2.py`

 * *Files identical despite different names*

### Comparing `pysqream-blue-1.0.46/protos/client_info_pb2.py` & `pysqream-blue-1.0.47/protos/client_info_pb2.py`

 * *Files identical despite different names*

### Comparing `pysqream-blue-1.0.46/protos/error_pb2.py` & `pysqream-blue-1.0.47/protos/error_pb2.py`

 * *Files identical despite different names*

### Comparing `pysqream-blue-1.0.46/protos/queryhandler_pb2.py` & `pysqream-blue-1.0.47/protos/queryhandler_pb2.py`

 * *Files 2% similar despite different names*

```diff
@@ -12,15 +12,15 @@
 
 _sym_db = _symbol_database.Default()
 
 
 from protos import error_pb2 as protos_dot_error__pb2
 
 
-DESCRIPTOR = _descriptor_pool.Default().AddSerializedFile(b'\n\x19protos/queryhandler.proto\x12\x1d\x63om.sqream.cloud.generated.v1\x1a\x12protos/error.proto\"Z\n\x0e\x43ompileRequest\x12\x12\n\ncontext_id\x18\x01 \x01(\t\x12\x0b\n\x03sql\x18\x02 \x01(\x0c\x12\x10\n\x08\x65ncoding\x18\x03 \x01(\t\x12\x15\n\rquery_timeout\x18\x04 \x01(\x03\"\xd8\x01\n\x0f\x43ompileResponse\x12\x12\n\ncontext_id\x18\x01 \x01(\t\x12>\n\x07\x63olumns\x18\x02 \x03(\x0b\x32-.com.sqream.cloud.generated.v1.ColumnMetadata\x12<\n\nquery_type\x18\x03 \x01(\x0e\x32(.com.sqream.cloud.generated.v1.QueryType\x12\x33\n\x05\x65rror\x18\x04 \x01(\x0b\x32$.com.sqream.cloud.generated.v1.Error\"#\n\rStatusRequest\x12\x12\n\ncontext_id\x18\x01 \x01(\t\"\x8a\x01\n\x0eStatusResponse\x12\x43\n\x06status\x18\x01 \x01(\x0e\x32\x33.com.sqream.cloud.generated.v1.QueryExecutionStatus\x12\x33\n\x05\x65rror\x18\x02 \x01(\x0b\x32$.com.sqream.cloud.generated.v1.Error\"$\n\x0e\x45xecuteRequest\x12\x12\n\ncontext_id\x18\x01 \x01(\t\"Z\n\x0f\x45xecuteResponse\x12\x12\n\ncontext_id\x18\x01 \x01(\t\x12\x33\n\x05\x65rror\x18\x02 \x01(\x0b\x32$.com.sqream.cloud.generated.v1.Error\"\xf1\x01\n\x0e\x43olumnMetadata\x12\x37\n\x04type\x18\x01 \x01(\x0e\x32).com.sqream.cloud.generated.v1.ColumnType\x12\x10\n\x08nullable\x18\x02 \x01(\x08\x12\x13\n\x0btru_varchar\x18\x03 \x01(\x08\x12\x0c\n\x04name\x18\x04 \x01(\t\x12\x12\n\nvalue_size\x18\x05 \x01(\x03\x12\r\n\x05scale\x18\x06 \x01(\x05\x12\x11\n\tprecision\x18\x07 \x01(\x05\x12;\n\x08sub_type\x18\x08 \x01(\x0e\x32).com.sqream.cloud.generated.v1.ColumnType\"\"\n\x0c\x46\x65tchRequest\x12\x12\n\ncontext_id\x18\x01 \x01(\t\"o\n\rFetchResponse\x12\x14\n\x0cquery_result\x18\x01 \x01(\x0c\x12\x33\n\x05\x65rror\x18\x02 \x01(\x0b\x32$.com.sqream.cloud.generated.v1.Error\x12\x13\n\x0bretry_fetch\x18\x03 \x01(\x08\"[\n\x15\x43loseStatementRequest\x12\x42\n\rclose_request\x18\x01 \x01(\x0b\x32+.com.sqream.cloud.generated.v1.CloseRequest\"^\n\x16\x43loseStatementResponse\x12\x44\n\x0e\x63lose_response\x18\x01 \x01(\x0b\x32,.com.sqream.cloud.generated.v1.CloseResponse\"Y\n\x13\x43loseSessionRequest\x12\x42\n\rclose_request\x18\x01 \x01(\x0b\x32+.com.sqream.cloud.generated.v1.CloseRequest\"\\\n\x14\x43loseSessionResponse\x12\x44\n\x0e\x63lose_response\x18\x01 \x01(\x0b\x32,.com.sqream.cloud.generated.v1.CloseResponse\"\"\n\x0c\x43loseRequest\x12\x12\n\ncontext_id\x18\x01 \x01(\t\"T\n\rCloseResponse\x12\x0e\n\x06\x63losed\x18\x01 \x01(\x08\x12\x33\n\x05\x65rror\x18\x02 \x01(\x0b\x32$.com.sqream.cloud.generated.v1.Error\"#\n\rCancelRequest\x12\x12\n\ncontext_id\x18\x01 \x01(\t\"W\n\x0e\x43\x61ncelResponse\x12\x10\n\x08\x63\x61nceled\x18\x01 \x01(\x08\x12\x33\n\x05\x65rror\x18\x02 \x01(\x0b\x32$.com.sqream.cloud.generated.v1.Error*\xb9\x03\n\nColumnType\x12\x1b\n\x17\x43OLUMN_TYPE_UNSPECIFIED\x10\x00\x12\x18\n\x14\x43OLUMN_TYPE_LONG_INT\x10\x01\x12\x19\n\x15\x43OLUMN_TYPE_ULONG_INT\x10\x02\x12\x13\n\x0f\x43OLUMN_TYPE_INT\x10\x04\x12\x14\n\x10\x43OLUMN_TYPE_UINT\x10\x05\x12\x17\n\x13\x43OLUMN_TYPE_VARCHAR\x10\x06\x12\x16\n\x12\x43OLUMN_TYPE_DOUBLE\x10\x07\x12\x14\n\x10\x43OLUMN_TYPE_BYTE\x10\x08\x12\x15\n\x11\x43OLUMN_TYPE_UBYTE\x10\t\x12\x15\n\x11\x43OLUMN_TYPE_SHORT\x10\n\x12\x16\n\x12\x43OLUMN_TYPE_USHORT\x10\x0b\x12\x15\n\x11\x43OLUMN_TYPE_FLOAT\x10\x0c\x12\x14\n\x10\x43OLUMN_TYPE_DATE\x10\r\x12\x18\n\x14\x43OLUMN_TYPE_DATETIME\x10\x0e\x12\x14\n\x10\x43OLUMN_TYPE_BOOL\x10\x0f\x12\x14\n\x10\x43OLUMN_TYPE_BLOB\x10\x10\x12\x17\n\x13\x43OLUMN_TYPE_NUMERIC\x10\x11\x12\x15\n\x11\x43OLUMN_TYPE_ARRAY\x10\x12*W\n\tQueryType\x12\x1a\n\x16QUERY_TYPE_UNSPECIFIED\x10\x00\x12\x14\n\x10QUERY_TYPE_QUERY\x10\x01\x12\x18\n\x14QUERY_TYPE_NON_QUERY\x10\x02*\x98\x02\n\x14QueryExecutionStatus\x12&\n\"QUERY_EXECUTION_STATUS_UNSPECIFIED\x10\x00\x12\"\n\x1eQUERY_EXECUTION_STATUS_RUNNING\x10\x01\x12$\n QUERY_EXECUTION_STATUS_SUCCEEDED\x10\x02\x12!\n\x1dQUERY_EXECUTION_STATUS_FAILED\x10\x03\x12$\n QUERY_EXECUTION_STATUS_CANCELLED\x10\x04\x12\"\n\x1eQUERY_EXECUTION_STATUS_ABORTED\x10\x05\x12!\n\x1dQUERY_EXECUTION_STATUS_QUEUED\x10\x06\x32\x93\x06\n\x13QueryHandlerService\x12h\n\x07\x43ompile\x12-.com.sqream.cloud.generated.v1.CompileRequest\x1a..com.sqream.cloud.generated.v1.CompileResponse\x12h\n\x07\x45xecute\x12-.com.sqream.cloud.generated.v1.ExecuteRequest\x1a..com.sqream.cloud.generated.v1.ExecuteResponse\x12\x65\n\x06Status\x12,.com.sqream.cloud.generated.v1.StatusRequest\x1a-.com.sqream.cloud.generated.v1.StatusResponse\x12\x62\n\x05\x46\x65tch\x12+.com.sqream.cloud.generated.v1.FetchRequest\x1a,.com.sqream.cloud.generated.v1.FetchResponse\x12}\n\x0e\x43loseStatement\x12\x34.com.sqream.cloud.generated.v1.CloseStatementRequest\x1a\x35.com.sqream.cloud.generated.v1.CloseStatementResponse\x12\x65\n\x06\x43\x61ncel\x12,.com.sqream.cloud.generated.v1.CancelRequest\x1a-.com.sqream.cloud.generated.v1.CancelResponse\x12w\n\x0c\x43loseSession\x12\x32.com.sqream.cloud.generated.v1.CloseSessionRequest\x1a\x33.com.sqream.cloud.generated.v1.CloseSessionResponseB\x02P\x01\x62\x06proto3')
+DESCRIPTOR = _descriptor_pool.Default().AddSerializedFile(b'\n\x19protos/queryhandler.proto\x12\x1d\x63om.sqream.cloud.generated.v1\x1a\x12protos/error.proto\"Z\n\x0e\x43ompileRequest\x12\x12\n\ncontext_id\x18\x01 \x01(\t\x12\x0b\n\x03sql\x18\x02 \x01(\x0c\x12\x10\n\x08\x65ncoding\x18\x03 \x01(\t\x12\x15\n\rquery_timeout\x18\x04 \x01(\x03\"\xd8\x01\n\x0f\x43ompileResponse\x12\x12\n\ncontext_id\x18\x01 \x01(\t\x12>\n\x07\x63olumns\x18\x02 \x03(\x0b\x32-.com.sqream.cloud.generated.v1.ColumnMetadata\x12<\n\nquery_type\x18\x03 \x01(\x0e\x32(.com.sqream.cloud.generated.v1.QueryType\x12\x33\n\x05\x65rror\x18\x04 \x01(\x0b\x32$.com.sqream.cloud.generated.v1.Error\"#\n\rStatusRequest\x12\x12\n\ncontext_id\x18\x01 \x01(\t\"\x8a\x01\n\x0eStatusResponse\x12\x43\n\x06status\x18\x01 \x01(\x0e\x32\x33.com.sqream.cloud.generated.v1.QueryExecutionStatus\x12\x33\n\x05\x65rror\x18\x02 \x01(\x0b\x32$.com.sqream.cloud.generated.v1.Error\"$\n\x0e\x45xecuteRequest\x12\x12\n\ncontext_id\x18\x01 \x01(\t\"Z\n\x0f\x45xecuteResponse\x12\x12\n\ncontext_id\x18\x01 \x01(\t\x12\x33\n\x05\x65rror\x18\x02 \x01(\x0b\x32$.com.sqream.cloud.generated.v1.Error\"\xf1\x01\n\x0e\x43olumnMetadata\x12\x37\n\x04type\x18\x01 \x01(\x0e\x32).com.sqream.cloud.generated.v1.ColumnType\x12\x10\n\x08nullable\x18\x02 \x01(\x08\x12\x13\n\x0btru_varchar\x18\x03 \x01(\x08\x12\x0c\n\x04name\x18\x04 \x01(\t\x12\x12\n\nvalue_size\x18\x05 \x01(\x03\x12\r\n\x05scale\x18\x06 \x01(\x05\x12\x11\n\tprecision\x18\x07 \x01(\x05\x12;\n\x08sub_type\x18\x08 \x01(\x0e\x32).com.sqream.cloud.generated.v1.ColumnType\"\"\n\x0c\x46\x65tchRequest\x12\x12\n\ncontext_id\x18\x01 \x01(\t\"o\n\rFetchResponse\x12\x14\n\x0cquery_result\x18\x01 \x01(\x0c\x12\x33\n\x05\x65rror\x18\x02 \x01(\x0b\x32$.com.sqream.cloud.generated.v1.Error\x12\x13\n\x0bretry_fetch\x18\x03 \x01(\x08\"[\n\x15\x43loseStatementRequest\x12\x42\n\rclose_request\x18\x01 \x01(\x0b\x32+.com.sqream.cloud.generated.v1.CloseRequest\"^\n\x16\x43loseStatementResponse\x12\x44\n\x0e\x63lose_response\x18\x01 \x01(\x0b\x32,.com.sqream.cloud.generated.v1.CloseResponse\"Y\n\x13\x43loseSessionRequest\x12\x42\n\rclose_request\x18\x01 \x01(\x0b\x32+.com.sqream.cloud.generated.v1.CloseRequest\"\\\n\x14\x43loseSessionResponse\x12\x44\n\x0e\x63lose_response\x18\x01 \x01(\x0b\x32,.com.sqream.cloud.generated.v1.CloseResponse\"\"\n\x0c\x43loseRequest\x12\x12\n\ncontext_id\x18\x01 \x01(\t\"T\n\rCloseResponse\x12\x0e\n\x06\x63losed\x18\x01 \x01(\x08\x12\x33\n\x05\x65rror\x18\x02 \x01(\x0b\x32$.com.sqream.cloud.generated.v1.Error\"#\n\rCancelRequest\x12\x12\n\ncontext_id\x18\x01 \x01(\t\"W\n\x0e\x43\x61ncelResponse\x12\x10\n\x08\x63\x61nceled\x18\x01 \x01(\x08\x12\x33\n\x05\x65rror\x18\x02 \x01(\x0b\x32$.com.sqream.cloud.generated.v1.Error*\xb9\x03\n\nColumnType\x12\x1b\n\x17\x43OLUMN_TYPE_UNSPECIFIED\x10\x00\x12\x18\n\x14\x43OLUMN_TYPE_LONG_INT\x10\x01\x12\x19\n\x15\x43OLUMN_TYPE_ULONG_INT\x10\x02\x12\x13\n\x0f\x43OLUMN_TYPE_INT\x10\x04\x12\x14\n\x10\x43OLUMN_TYPE_UINT\x10\x05\x12\x17\n\x13\x43OLUMN_TYPE_VARCHAR\x10\x06\x12\x16\n\x12\x43OLUMN_TYPE_DOUBLE\x10\x07\x12\x14\n\x10\x43OLUMN_TYPE_BYTE\x10\x08\x12\x15\n\x11\x43OLUMN_TYPE_UBYTE\x10\t\x12\x15\n\x11\x43OLUMN_TYPE_SHORT\x10\n\x12\x16\n\x12\x43OLUMN_TYPE_USHORT\x10\x0b\x12\x15\n\x11\x43OLUMN_TYPE_FLOAT\x10\x0c\x12\x14\n\x10\x43OLUMN_TYPE_DATE\x10\r\x12\x18\n\x14\x43OLUMN_TYPE_DATETIME\x10\x0e\x12\x14\n\x10\x43OLUMN_TYPE_BOOL\x10\x0f\x12\x14\n\x10\x43OLUMN_TYPE_BLOB\x10\x10\x12\x17\n\x13\x43OLUMN_TYPE_NUMERIC\x10\x11\x12\x15\n\x11\x43OLUMN_TYPE_ARRAY\x10\x12*W\n\tQueryType\x12\x1a\n\x16QUERY_TYPE_UNSPECIFIED\x10\x00\x12\x14\n\x10QUERY_TYPE_QUERY\x10\x01\x12\x18\n\x14QUERY_TYPE_NON_QUERY\x10\x02*\xf4\x02\n\x14QueryExecutionStatus\x12&\n\"QUERY_EXECUTION_STATUS_UNSPECIFIED\x10\x00\x12\"\n\x1eQUERY_EXECUTION_STATUS_RUNNING\x10\x01\x12$\n QUERY_EXECUTION_STATUS_SUCCEEDED\x10\x02\x12!\n\x1dQUERY_EXECUTION_STATUS_FAILED\x10\x03\x12$\n QUERY_EXECUTION_STATUS_CANCELLED\x10\x04\x12\"\n\x1eQUERY_EXECUTION_STATUS_ABORTED\x10\x05\x12!\n\x1dQUERY_EXECUTION_STATUS_QUEUED\x10\x06\x12(\n$QUERY_EXECUTION_STATUS_QUEUE_TIMEOUT\x10\x07\x12\x30\n,QUERY_EXECUTION_STATUS_QUERY_RUNTIME_TIMEOUT\x10\x08\x32\x93\x06\n\x13QueryHandlerService\x12h\n\x07\x43ompile\x12-.com.sqream.cloud.generated.v1.CompileRequest\x1a..com.sqream.cloud.generated.v1.CompileResponse\x12h\n\x07\x45xecute\x12-.com.sqream.cloud.generated.v1.ExecuteRequest\x1a..com.sqream.cloud.generated.v1.ExecuteResponse\x12\x65\n\x06Status\x12,.com.sqream.cloud.generated.v1.StatusRequest\x1a-.com.sqream.cloud.generated.v1.StatusResponse\x12\x62\n\x05\x46\x65tch\x12+.com.sqream.cloud.generated.v1.FetchRequest\x1a,.com.sqream.cloud.generated.v1.FetchResponse\x12}\n\x0e\x43loseStatement\x12\x34.com.sqream.cloud.generated.v1.CloseStatementRequest\x1a\x35.com.sqream.cloud.generated.v1.CloseStatementResponse\x12\x65\n\x06\x43\x61ncel\x12,.com.sqream.cloud.generated.v1.CancelRequest\x1a-.com.sqream.cloud.generated.v1.CancelResponse\x12w\n\x0c\x43loseSession\x12\x32.com.sqream.cloud.generated.v1.CloseSessionRequest\x1a\x33.com.sqream.cloud.generated.v1.CloseSessionResponseB\x02P\x01\x62\x06proto3')
 
 _COLUMNTYPE = DESCRIPTOR.enum_types_by_name['ColumnType']
 ColumnType = enum_type_wrapper.EnumTypeWrapper(_COLUMNTYPE)
 _QUERYTYPE = DESCRIPTOR.enum_types_by_name['QueryType']
 QueryType = enum_type_wrapper.EnumTypeWrapper(_QUERYTYPE)
 _QUERYEXECUTIONSTATUS = DESCRIPTOR.enum_types_by_name['QueryExecutionStatus']
 QueryExecutionStatus = enum_type_wrapper.EnumTypeWrapper(_QUERYEXECUTIONSTATUS)
@@ -48,14 +48,16 @@
 QUERY_EXECUTION_STATUS_UNSPECIFIED = 0
 QUERY_EXECUTION_STATUS_RUNNING = 1
 QUERY_EXECUTION_STATUS_SUCCEEDED = 2
 QUERY_EXECUTION_STATUS_FAILED = 3
 QUERY_EXECUTION_STATUS_CANCELLED = 4
 QUERY_EXECUTION_STATUS_ABORTED = 5
 QUERY_EXECUTION_STATUS_QUEUED = 6
+QUERY_EXECUTION_STATUS_QUEUE_TIMEOUT = 7
+QUERY_EXECUTION_STATUS_QUERY_RUNTIME_TIMEOUT = 8
 
 
 _COMPILEREQUEST = DESCRIPTOR.message_types_by_name['CompileRequest']
 _COMPILERESPONSE = DESCRIPTOR.message_types_by_name['CompileResponse']
 _STATUSREQUEST = DESCRIPTOR.message_types_by_name['StatusRequest']
 _STATUSRESPONSE = DESCRIPTOR.message_types_by_name['StatusResponse']
 _EXECUTEREQUEST = DESCRIPTOR.message_types_by_name['ExecuteRequest']
@@ -196,15 +198,15 @@
   DESCRIPTOR._options = None
   DESCRIPTOR._serialized_options = b'P\001'
   _COLUMNTYPE._serialized_start=1715
   _COLUMNTYPE._serialized_end=2156
   _QUERYTYPE._serialized_start=2158
   _QUERYTYPE._serialized_end=2245
   _QUERYEXECUTIONSTATUS._serialized_start=2248
-  _QUERYEXECUTIONSTATUS._serialized_end=2528
+  _QUERYEXECUTIONSTATUS._serialized_end=2620
   _COMPILEREQUEST._serialized_start=80
   _COMPILEREQUEST._serialized_end=170
   _COMPILERESPONSE._serialized_start=173
   _COMPILERESPONSE._serialized_end=389
   _STATUSREQUEST._serialized_start=391
   _STATUSREQUEST._serialized_end=426
   _STATUSRESPONSE._serialized_start=429
@@ -231,10 +233,10 @@
   _CLOSEREQUEST._serialized_end=1500
   _CLOSERESPONSE._serialized_start=1502
   _CLOSERESPONSE._serialized_end=1586
   _CANCELREQUEST._serialized_start=1588
   _CANCELREQUEST._serialized_end=1623
   _CANCELRESPONSE._serialized_start=1625
   _CANCELRESPONSE._serialized_end=1712
-  _QUERYHANDLERSERVICE._serialized_start=2531
-  _QUERYHANDLERSERVICE._serialized_end=3318
+  _QUERYHANDLERSERVICE._serialized_start=2623
+  _QUERYHANDLERSERVICE._serialized_end=3410
 # @@protoc_insertion_point(module_scope)
```

### Comparing `pysqream-blue-1.0.46/protos/queryhandler_pb2_grpc.py` & `pysqream-blue-1.0.47/protos/queryhandler_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `pysqream-blue-1.0.46/pysqream_blue/array_parser.py` & `pysqream-blue-1.0.47/pysqream_blue/array_parser.py`

 * *Files identical despite different names*

### Comparing `pysqream-blue-1.0.46/pysqream_blue/casting.py` & `pysqream-blue-1.0.47/pysqream_blue/casting.py`

 * *Files identical despite different names*

### Comparing `pysqream-blue-1.0.46/pysqream_blue/connection.py` & `pysqream-blue-1.0.47/pysqream_blue/connection.py`

 * *Files identical despite different names*

### Comparing `pysqream-blue-1.0.46/pysqream_blue/cursor.py` & `pysqream-blue-1.0.47/pysqream_blue/cursor.py`

 * *Files 2% similar despite different names*

```diff
@@ -189,14 +189,22 @@
                     self.logs.log_and_raise(OperationalError,
                                   f'Query id: {self.stmt_id}. Error while attempting to get query status.\n{status_response.error}')
 
                 if status_response.status == qh_messages.QUERY_EXECUTION_STATUS_ABORTED:
                     self.logs.message(f"Query id {self.stmt_id} is aborted", self.logs.info)
                     return
 
+                if status_response.status == qh_messages.QUERY_EXECUTION_STATUS_QUEUE_TIMEOUT:
+                    self.logs.message("Connection query queue timeout expired.", self.logs.info)
+                    return
+
+                if status_response.status == qh_messages.QUERY_EXECUTION_STATUS_QUERY_RUNTIME_TIMEOUT:
+                    self.logs.message("Connection query runtime timeout expired.", self.logs.info)
+                    return
+
                 elif status_response.status != qh_messages.QUERY_EXECUTION_STATUS_RUNNING and \
                         status_response.status != qh_messages.QUERY_EXECUTION_STATUS_QUEUED:
                     self.stmt_status = status_response.status
                     self.logs.message(
                         f'Query id: {self.stmt_id}. status: '
                         f'{qh_messages.QueryExecutionStatus.Name(self.stmt_status)}.', self.logs.info)
                     if self.stmt_status != qh_messages.QUERY_EXECUTION_STATUS_SUCCEEDED:
```

### Comparing `pysqream-blue-1.0.46/pysqream_blue/globals.py` & `pysqream-blue-1.0.47/pysqream_blue/globals.py`

 * *Files 0% similar despite different names*

```diff
@@ -6,15 +6,15 @@
 import protos.queryhandler_pb2_grpc as qh_services
 import protos.authentication_pb2 as auth_messages
 import protos.authentication_pb2_grpc as auth_services
 import protos.client_info_pb2 as cl_messages
 import protos.client_info_pb2_grpc as cl_services
 import protos.authentication_type_pb2 as auth_type_messages
 
-__version__ = '1.0.46'
+__version__ = '1.0.47'
 
 dbapi_typecodes = {
     qh_messages.COLUMN_TYPE_LONG_INT:  'NUMBER',
     qh_messages.COLUMN_TYPE_ULONG_INT: 'NUMBER',
     qh_messages.COLUMN_TYPE_INT:       'NUMBER',
     qh_messages.COLUMN_TYPE_UINT:      'NUMBER',
     qh_messages.COLUMN_TYPE_VARCHAR:   'STRING',
```

### Comparing `pysqream-blue-1.0.46/pysqream_blue/logger.py` & `pysqream-blue-1.0.47/pysqream_blue/logger.py`

 * *Files identical despite different names*

### Comparing `pysqream-blue-1.0.46/pysqream_blue/pysqream_blue.py` & `pysqream-blue-1.0.47/pysqream_blue/pysqream_blue.py`

 * *Files identical despite different names*

### Comparing `pysqream-blue-1.0.46/pysqream_blue/utils.py` & `pysqream-blue-1.0.47/pysqream_blue/utils.py`

 * *Files identical despite different names*

### Comparing `pysqream-blue-1.0.46/pysqream_blue.egg-info/PKG-INFO` & `pysqream-blue-1.0.47/pysqream_blue.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pysqream-blue
-Version: 1.0.46
+Version: 1.0.47
 Summary: DB-API connector for SQream DB
 Home-page: https://github.com/SQream/pysqream-blue
 Author: SQream
 Author-email: info@sqream.com
 Keywords: database db-api sqream sqreamdbV2
 Classifier: Programming Language :: Python :: 3.9
 Classifier: License :: OSI Approved :: BSD License
```

### Comparing `pysqream-blue-1.0.46/pysqream_blue.egg-info/SOURCES.txt` & `pysqream-blue-1.0.47/pysqream_blue.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `pysqream-blue-1.0.46/setup.py` & `pysqream-blue-1.0.47/setup.py`

 * *Files identical despite different names*

