# Comparing `tmp/openagents_grpc_proto-0.9.tar.gz` & `tmp/openagents_grpc_proto-0.9.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "openagents_grpc_proto-0.9.tar", last modified: Thu May 23 09:00:19 2024, max compression
+gzip compressed data, was "openagents_grpc_proto-0.9.1.tar", last modified: Tue May 28 17:10:47 2024, max compression
```

## Comparing `openagents_grpc_proto-0.9.tar` & `openagents_grpc_proto-0.9.1.tar`

### file list

```diff
@@ -1,34 +1,36 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-23 09:00:19.296179 openagents_grpc_proto-0.9/
--rw-r--r--   0 runner    (1001) docker     (127)       15 2024-05-23 09:00:18.000000 openagents_grpc_proto-0.9/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (127)      196 2024-05-23 09:00:19.296179 openagents_grpc_proto-0.9/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)        4 2024-05-23 09:00:18.000000 openagents_grpc_proto-0.9/VERSION
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-23 09:00:19.296179 openagents_grpc_proto-0.9/openagents_grpc_proto/
--rw-r--r--   0 runner    (1001) docker     (127)     1464 2024-05-23 09:00:18.000000 openagents_grpc_proto-0.9/openagents_grpc_proto/JobInput_pb2.py
--rw-r--r--   0 runner    (1001) docker     (127)     1125 2024-05-23 09:00:18.000000 openagents_grpc_proto-0.9/openagents_grpc_proto/JobInput_pb2_grpc.py
--rw-r--r--   0 runner    (1001) docker     (127)     1249 2024-05-23 09:00:18.000000 openagents_grpc_proto-0.9/openagents_grpc_proto/JobParam_pb2.py
--rw-r--r--   0 runner    (1001) docker     (127)     1125 2024-05-23 09:00:18.000000 openagents_grpc_proto-0.9/openagents_grpc_proto/JobParam_pb2_grpc.py
--rw-r--r--   0 runner    (1001) docker     (127)     1296 2024-05-23 09:00:18.000000 openagents_grpc_proto-0.9/openagents_grpc_proto/JobResult_pb2.py
--rw-r--r--   0 runner    (1001) docker     (127)     1126 2024-05-23 09:00:18.000000 openagents_grpc_proto-0.9/openagents_grpc_proto/JobResult_pb2_grpc.py
--rw-r--r--   0 runner    (1001) docker     (127)     1684 2024-05-23 09:00:18.000000 openagents_grpc_proto-0.9/openagents_grpc_proto/JobState_pb2.py
--rw-r--r--   0 runner    (1001) docker     (127)     1125 2024-05-23 09:00:18.000000 openagents_grpc_proto-0.9/openagents_grpc_proto/JobState_pb2_grpc.py
--rw-r--r--   0 runner    (1001) docker     (127)     1402 2024-05-23 09:00:18.000000 openagents_grpc_proto-0.9/openagents_grpc_proto/JobStatus_pb2.py
--rw-r--r--   0 runner    (1001) docker     (127)     1126 2024-05-23 09:00:18.000000 openagents_grpc_proto-0.9/openagents_grpc_proto/JobStatus_pb2_grpc.py
--rw-r--r--   0 runner    (1001) docker     (127)     2207 2024-05-23 09:00:18.000000 openagents_grpc_proto-0.9/openagents_grpc_proto/Job_pb2.py
--rw-r--r--   0 runner    (1001) docker     (127)     1120 2024-05-23 09:00:18.000000 openagents_grpc_proto-0.9/openagents_grpc_proto/Job_pb2_grpc.py
--rw-r--r--   0 runner    (1001) docker     (127)     1359 2024-05-23 09:00:18.000000 openagents_grpc_proto-0.9/openagents_grpc_proto/Log_pb2.py
--rw-r--r--   0 runner    (1001) docker     (127)     1120 2024-05-23 09:00:18.000000 openagents_grpc_proto-0.9/openagents_grpc_proto/Log_pb2_grpc.py
--rw-r--r--   0 runner    (1001) docker     (127)     1448 2024-05-23 09:00:18.000000 openagents_grpc_proto-0.9/openagents_grpc_proto/PaymentStatus_pb2.py
--rw-r--r--   0 runner    (1001) docker     (127)     1130 2024-05-23 09:00:18.000000 openagents_grpc_proto-0.9/openagents_grpc_proto/PaymentStatus_pb2_grpc.py
--rw-r--r--   0 runner    (1001) docker     (127)     1438 2024-05-23 09:00:18.000000 openagents_grpc_proto-0.9/openagents_grpc_proto/Payment_pb2.py
--rw-r--r--   0 runner    (1001) docker     (127)     1124 2024-05-23 09:00:18.000000 openagents_grpc_proto-0.9/openagents_grpc_proto/Payment_pb2_grpc.py
--rw-r--r--   0 runner    (1001) docker     (127)       83 2024-05-23 09:00:18.000000 openagents_grpc_proto-0.9/openagents_grpc_proto/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    17599 2024-05-23 09:00:18.000000 openagents_grpc_proto-0.9/openagents_grpc_proto/rpc_pb2.py
--rw-r--r--   0 runner    (1001) docker     (127)    55640 2024-05-23 09:00:18.000000 openagents_grpc_proto-0.9/openagents_grpc_proto/rpc_pb2_grpc.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-23 09:00:19.296179 openagents_grpc_proto-0.9/openagents_grpc_proto.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)      196 2024-05-23 09:00:18.000000 openagents_grpc_proto-0.9/openagents_grpc_proto.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     1078 2024-05-23 09:00:19.000000 openagents_grpc_proto-0.9/openagents_grpc_proto.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-23 09:00:18.000000 openagents_grpc_proto-0.9/openagents_grpc_proto.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       32 2024-05-23 09:00:18.000000 openagents_grpc_proto-0.9/openagents_grpc_proto.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       22 2024-05-23 09:00:18.000000 openagents_grpc_proto-0.9/openagents_grpc_proto.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-23 09:00:19.296179 openagents_grpc_proto-0.9/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)      504 2024-05-23 09:00:18.000000 openagents_grpc_proto-0.9/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-28 17:10:47.913634 openagents_grpc_proto-0.9.1/
+-rw-r--r--   0 runner    (1001) docker     (127)       15 2024-05-28 17:10:47.000000 openagents_grpc_proto-0.9.1/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (127)      198 2024-05-28 17:10:47.913634 openagents_grpc_proto-0.9.1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)        6 2024-05-28 17:10:47.000000 openagents_grpc_proto-0.9.1/VERSION
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-28 17:10:47.913634 openagents_grpc_proto-0.9.1/openagents_grpc_proto/
+-rw-r--r--   0 runner    (1001) docker     (127)     1274 2024-05-28 17:10:47.000000 openagents_grpc_proto-0.9.1/openagents_grpc_proto/Bid_pb2.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1120 2024-05-28 17:10:47.000000 openagents_grpc_proto-0.9.1/openagents_grpc_proto/Bid_pb2_grpc.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1464 2024-05-28 17:10:47.000000 openagents_grpc_proto-0.9.1/openagents_grpc_proto/JobInput_pb2.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1125 2024-05-28 17:10:47.000000 openagents_grpc_proto-0.9.1/openagents_grpc_proto/JobInput_pb2_grpc.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1249 2024-05-28 17:10:47.000000 openagents_grpc_proto-0.9.1/openagents_grpc_proto/JobParam_pb2.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1125 2024-05-28 17:10:47.000000 openagents_grpc_proto-0.9.1/openagents_grpc_proto/JobParam_pb2_grpc.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1296 2024-05-28 17:10:47.000000 openagents_grpc_proto-0.9.1/openagents_grpc_proto/JobResult_pb2.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1126 2024-05-28 17:10:47.000000 openagents_grpc_proto-0.9.1/openagents_grpc_proto/JobResult_pb2_grpc.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1798 2024-05-28 17:10:47.000000 openagents_grpc_proto-0.9.1/openagents_grpc_proto/JobState_pb2.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1125 2024-05-28 17:10:47.000000 openagents_grpc_proto-0.9.1/openagents_grpc_proto/JobState_pb2_grpc.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1402 2024-05-28 17:10:47.000000 openagents_grpc_proto-0.9.1/openagents_grpc_proto/JobStatus_pb2.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1126 2024-05-28 17:10:47.000000 openagents_grpc_proto-0.9.1/openagents_grpc_proto/JobStatus_pb2_grpc.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2386 2024-05-28 17:10:47.000000 openagents_grpc_proto-0.9.1/openagents_grpc_proto/Job_pb2.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1120 2024-05-28 17:10:47.000000 openagents_grpc_proto-0.9.1/openagents_grpc_proto/Job_pb2_grpc.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1359 2024-05-28 17:10:47.000000 openagents_grpc_proto-0.9.1/openagents_grpc_proto/Log_pb2.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1120 2024-05-28 17:10:47.000000 openagents_grpc_proto-0.9.1/openagents_grpc_proto/Log_pb2_grpc.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1448 2024-05-28 17:10:47.000000 openagents_grpc_proto-0.9.1/openagents_grpc_proto/PaymentStatus_pb2.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1130 2024-05-28 17:10:47.000000 openagents_grpc_proto-0.9.1/openagents_grpc_proto/PaymentStatus_pb2_grpc.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1543 2024-05-28 17:10:47.000000 openagents_grpc_proto-0.9.1/openagents_grpc_proto/Payment_pb2.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1124 2024-05-28 17:10:47.000000 openagents_grpc_proto-0.9.1/openagents_grpc_proto/Payment_pb2_grpc.py
+-rw-r--r--   0 runner    (1001) docker     (127)       83 2024-05-28 17:10:47.000000 openagents_grpc_proto-0.9.1/openagents_grpc_proto/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    17599 2024-05-28 17:10:47.000000 openagents_grpc_proto-0.9.1/openagents_grpc_proto/rpc_pb2.py
+-rw-r--r--   0 runner    (1001) docker     (127)    55640 2024-05-28 17:10:47.000000 openagents_grpc_proto-0.9.1/openagents_grpc_proto/rpc_pb2_grpc.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-28 17:10:47.913634 openagents_grpc_proto-0.9.1/openagents_grpc_proto.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)      198 2024-05-28 17:10:47.000000 openagents_grpc_proto-0.9.1/openagents_grpc_proto.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     1149 2024-05-28 17:10:47.000000 openagents_grpc_proto-0.9.1/openagents_grpc_proto.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-28 17:10:47.000000 openagents_grpc_proto-0.9.1/openagents_grpc_proto.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       32 2024-05-28 17:10:47.000000 openagents_grpc_proto-0.9.1/openagents_grpc_proto.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       22 2024-05-28 17:10:47.000000 openagents_grpc_proto-0.9.1/openagents_grpc_proto.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-28 17:10:47.913634 openagents_grpc_proto-0.9.1/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)      504 2024-05-28 17:10:47.000000 openagents_grpc_proto-0.9.1/setup.py
```

### Comparing `openagents_grpc_proto-0.9/openagents_grpc_proto/JobInput_pb2.py` & `openagents_grpc_proto-0.9.1/openagents_grpc_proto/JobInput_pb2.py`

 * *Files identical despite different names*

### Comparing `openagents_grpc_proto-0.9/openagents_grpc_proto/JobInput_pb2_grpc.py` & `openagents_grpc_proto-0.9.1/openagents_grpc_proto/JobInput_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `openagents_grpc_proto-0.9/openagents_grpc_proto/JobParam_pb2.py` & `openagents_grpc_proto-0.9.1/openagents_grpc_proto/JobParam_pb2.py`

 * *Files identical despite different names*

### Comparing `openagents_grpc_proto-0.9/openagents_grpc_proto/JobParam_pb2_grpc.py` & `openagents_grpc_proto-0.9.1/openagents_grpc_proto/JobParam_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `openagents_grpc_proto-0.9/openagents_grpc_proto/JobResult_pb2.py` & `openagents_grpc_proto-0.9.1/openagents_grpc_proto/JobResult_pb2.py`

 * *Files identical despite different names*

### Comparing `openagents_grpc_proto-0.9/openagents_grpc_proto/JobResult_pb2_grpc.py` & `openagents_grpc_proto-0.9.1/openagents_grpc_proto/JobResult_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `openagents_grpc_proto-0.9/openagents_grpc_proto/JobState_pb2.py` & `openagents_grpc_proto-0.9.1/openagents_grpc_proto/JobState_pb2.py`

 * *Files 4% similar despite different names*

```diff
@@ -11,20 +11,21 @@
 
 _sym_db = _symbol_database.Default()
 
 
 import Log_pb2 as Log__pb2
 import JobStatus_pb2 as JobStatus__pb2
 import JobResult_pb2 as JobResult__pb2
+import Payment_pb2 as Payment__pb2
 
 
-DESCRIPTOR = _descriptor_pool.Default().AddSerializedFile(b'\n\x0eJobState.proto\x1a\tLog.proto\x1a\x0fJobStatus.proto\x1a\x0fJobResult.proto\"\xa9\x01\n\x08JobState\x12\x12\n\nacceptedAt\x18\r \x01(\x04\x12\x12\n\nacceptedBy\x18\x0e \x01(\t\x12\x1a\n\x06status\x18\x0f \x01(\x0e\x32\n.JobStatus\x12\x12\n\x04logs\x18\x11 \x03(\x0b\x32\x04.Log\x12\x11\n\ttimestamp\x18\x12 \x01(\x04\x12\x1a\n\x06result\x18\x13 \x01(\x0b\x32\n.JobResult\x12\x16\n\x0e\x61\x63\x63\x65ptedByNode\x18\x14 \x01(\tB.\xca\x02\x0e\x41pp\\Grpc\\nostr\xe2\x02\x1a\x41pp\\Grpc\\nostr\\GPBMetadatab\x06proto3')
+DESCRIPTOR = _descriptor_pool.Default().AddSerializedFile(b'\n\x0eJobState.proto\x1a\tLog.proto\x1a\x0fJobStatus.proto\x1a\x0fJobResult.proto\x1a\rPayment.proto\"\xcc\x01\n\x08JobState\x12\x12\n\nacceptedAt\x18\r \x01(\x04\x12\x12\n\nacceptedBy\x18\x0e \x01(\t\x12\x1a\n\x06status\x18\x0f \x01(\x0e\x32\n.JobStatus\x12\x12\n\x04logs\x18\x11 \x03(\x0b\x32\x04.Log\x12\x11\n\ttimestamp\x18\x12 \x01(\x04\x12\x1a\n\x06result\x18\x13 \x01(\x0b\x32\n.JobResult\x12\x16\n\x0e\x61\x63\x63\x65ptedByNode\x18\x14 \x01(\t\x12!\n\x0fpaymentRequests\x18\x15 \x03(\x0b\x32\x08.PaymentB.\xca\x02\x0e\x41pp\\Grpc\\nostr\xe2\x02\x1a\x41pp\\Grpc\\nostr\\GPBMetadatab\x06proto3')
 
 _globals = globals()
 _builder.BuildMessageAndEnumDescriptors(DESCRIPTOR, _globals)
 _builder.BuildTopDescriptorsAndMessages(DESCRIPTOR, 'JobState_pb2', _globals)
 if not _descriptor._USE_C_DESCRIPTORS:
   _globals['DESCRIPTOR']._loaded_options = None
   _globals['DESCRIPTOR']._serialized_options = b'\312\002\016App\\Grpc\\nostr\342\002\032App\\Grpc\\nostr\\GPBMetadata'
-  _globals['_JOBSTATE']._serialized_start=64
-  _globals['_JOBSTATE']._serialized_end=233
+  _globals['_JOBSTATE']._serialized_start=79
+  _globals['_JOBSTATE']._serialized_end=283
 # @@protoc_insertion_point(module_scope)
```

### Comparing `openagents_grpc_proto-0.9/openagents_grpc_proto/JobState_pb2_grpc.py` & `openagents_grpc_proto-0.9.1/openagents_grpc_proto/JobState_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `openagents_grpc_proto-0.9/openagents_grpc_proto/JobStatus_pb2.py` & `openagents_grpc_proto-0.9.1/openagents_grpc_proto/JobStatus_pb2.py`

 * *Files identical despite different names*

### Comparing `openagents_grpc_proto-0.9/openagents_grpc_proto/JobStatus_pb2_grpc.py` & `openagents_grpc_proto-0.9.1/openagents_grpc_proto/JobStatus_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `openagents_grpc_proto-0.9/openagents_grpc_proto/Job_pb2.py` & `openagents_grpc_proto-0.9.1/openagents_grpc_proto/Job_pb2.py`

 * *Files 9% similar despite different names*

```diff
@@ -12,20 +12,22 @@
 _sym_db = _symbol_database.Default()
 
 
 import JobParam_pb2 as JobParam__pb2
 import JobInput_pb2 as JobInput__pb2
 import JobState_pb2 as JobState__pb2
 import JobResult_pb2 as JobResult__pb2
+import Payment_pb2 as Payment__pb2
+import Bid_pb2 as Bid__pb2
 
 
-DESCRIPTOR = _descriptor_pool.Default().AddSerializedFile(b'\n\tJob.proto\x1a\x0eJobParam.proto\x1a\x0eJobInput.proto\x1a\x0eJobState.proto\x1a\x0fJobResult.proto\"\x93\x03\n\x03Job\x12\n\n\x02id\x18\x01 \x01(\t\x12\x0c\n\x04kind\x18\x0e \x01(\r\x12\r\n\x05runOn\x18\x02 \x01(\t\x12\x12\n\nexpiration\x18\x03 \x01(\x04\x12\x11\n\ttimestamp\x18\x04 \x01(\x04\x12\x18\n\x05input\x18\x05 \x03(\x0b\x32\t.JobInput\x12\x18\n\x05param\x18\x06 \x03(\x0b\x32\t.JobParam\x12\x19\n\x11\x63ustomerPublicKey\x18\x07 \x01(\t\x12\x13\n\x0b\x64\x65scription\x18\x08 \x01(\t\x12\x10\n\x08provider\x18\t \x01(\t\x12\x0e\n\x06relays\x18\n \x03(\t\x12\x1a\n\x06result\x18\x0c \x01(\x0b\x32\n.JobResult\x12\x18\n\x05state\x18\x0b \x01(\x0b\x32\t.JobState\x12\x1a\n\x07results\x18\x12 \x03(\x0b\x32\t.JobState\x12\x18\n\x10maxExecutionTime\x18\r \x01(\x04\x12\x0e\n\x06nodeId\x18\x0f \x01(\t\x12\x14\n\x0coutputFormat\x18\x10 \x01(\t\x12\x16\n\tencrypted\x18\x11 \x01(\x08H\x00\x88\x01\x01\x42\x0c\n\n_encryptedB.\xca\x02\x0e\x41pp\\Grpc\\nostr\xe2\x02\x1a\x41pp\\Grpc\\nostr\\GPBMetadatab\x06proto3')
+DESCRIPTOR = _descriptor_pool.Default().AddSerializedFile(b'\n\tJob.proto\x1a\x0eJobParam.proto\x1a\x0eJobInput.proto\x1a\x0eJobState.proto\x1a\x0fJobResult.proto\x1a\rPayment.proto\x1a\tBid.proto\"\xb3\x03\n\x03Job\x12\n\n\x02id\x18\x01 \x01(\t\x12\x0c\n\x04kind\x18\x0e \x01(\r\x12\r\n\x05runOn\x18\x02 \x01(\t\x12\x12\n\nexpiration\x18\x03 \x01(\x04\x12\x11\n\ttimestamp\x18\x04 \x01(\x04\x12\x18\n\x05input\x18\x05 \x03(\x0b\x32\t.JobInput\x12\x18\n\x05param\x18\x06 \x03(\x0b\x32\t.JobParam\x12\x19\n\x11\x63ustomerPublicKey\x18\x07 \x01(\t\x12\x13\n\x0b\x64\x65scription\x18\x08 \x01(\t\x12\x10\n\x08provider\x18\t \x01(\t\x12\x0e\n\x06relays\x18\n \x03(\t\x12\x1a\n\x06result\x18\x0c \x01(\x0b\x32\n.JobResult\x12\x18\n\x05state\x18\x0b \x01(\x0b\x32\t.JobState\x12\x1a\n\x07results\x18\x12 \x03(\x0b\x32\t.JobState\x12\x18\n\x10maxExecutionTime\x18\r \x01(\x04\x12\x0e\n\x06nodeId\x18\x0f \x01(\t\x12\x14\n\x0coutputFormat\x18\x10 \x01(\t\x12\x16\n\tencrypted\x18\x11 \x01(\x08H\x00\x88\x01\x01\x12\x16\n\x03\x62id\x18\x13 \x01(\x0b\x32\x04.BidH\x01\x88\x01\x01\x42\x0c\n\n_encryptedB\x06\n\x04_bidB.\xca\x02\x0e\x41pp\\Grpc\\nostr\xe2\x02\x1a\x41pp\\Grpc\\nostr\\GPBMetadatab\x06proto3')
 
 _globals = globals()
 _builder.BuildMessageAndEnumDescriptors(DESCRIPTOR, _globals)
 _builder.BuildTopDescriptorsAndMessages(DESCRIPTOR, 'Job_pb2', _globals)
 if not _descriptor._USE_C_DESCRIPTORS:
   _globals['DESCRIPTOR']._loaded_options = None
   _globals['DESCRIPTOR']._serialized_options = b'\312\002\016App\\Grpc\\nostr\342\002\032App\\Grpc\\nostr\\GPBMetadata'
-  _globals['_JOB']._serialized_start=79
-  _globals['_JOB']._serialized_end=482
+  _globals['_JOB']._serialized_start=105
+  _globals['_JOB']._serialized_end=540
 # @@protoc_insertion_point(module_scope)
```

### Comparing `openagents_grpc_proto-0.9/openagents_grpc_proto/Job_pb2_grpc.py` & `openagents_grpc_proto-0.9.1/openagents_grpc_proto/Job_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `openagents_grpc_proto-0.9/openagents_grpc_proto/Log_pb2.py` & `openagents_grpc_proto-0.9.1/openagents_grpc_proto/Log_pb2.py`

 * *Files identical despite different names*

### Comparing `openagents_grpc_proto-0.9/openagents_grpc_proto/Log_pb2_grpc.py` & `openagents_grpc_proto-0.9.1/openagents_grpc_proto/Log_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `openagents_grpc_proto-0.9/openagents_grpc_proto/PaymentStatus_pb2.py` & `openagents_grpc_proto-0.9.1/openagents_grpc_proto/PaymentStatus_pb2.py`

 * *Files identical despite different names*

### Comparing `openagents_grpc_proto-0.9/openagents_grpc_proto/PaymentStatus_pb2_grpc.py` & `openagents_grpc_proto-0.9.1/openagents_grpc_proto/PaymentStatus_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `openagents_grpc_proto-0.9/openagents_grpc_proto/Payment_pb2.py` & `openagents_grpc_proto-0.9.1/openagents_grpc_proto/Bid_pb2.py`

 * *Files 15% similar despite different names*

```diff
@@ -1,27 +1,27 @@
 # -*- coding: utf-8 -*-
 # Generated by the protocol buffer compiler.  DO NOT EDIT!
-# source: Payment.proto
+# source: Bid.proto
 # Protobuf Python Version: 5.26.1
 """Generated protocol buffer code."""
 from google.protobuf import descriptor as _descriptor
 from google.protobuf import descriptor_pool as _descriptor_pool
 from google.protobuf import symbol_database as _symbol_database
 from google.protobuf.internal import builder as _builder
 # @@protoc_insertion_point(imports)
 
 _sym_db = _symbol_database.Default()
 
 
 
 
-DESCRIPTOR = _descriptor_pool.Default().AddSerializedFile(b'\n\rPayment.proto\"u\n\x07Payment\x12\n\n\x02id\x18\x01 \x01(\t\x12\x0e\n\x06\x61mount\x18\x02 \x01(\x04\x12\x10\n\x08\x63urrency\x18\x03 \x01(\t\x12\x10\n\x08protocol\x18\x04 \x01(\t\x12\x0e\n\x06status\x18\x05 \x01(\t\x12\x11\n\x04\x64\x61ta\x18\x06 \x01(\tH\x00\x88\x01\x01\x42\x07\n\x05_dataB.\xca\x02\x0e\x41pp\\Grpc\\nostr\xe2\x02\x1a\x41pp\\Grpc\\nostr\\GPBMetadatab\x06proto3')
+DESCRIPTOR = _descriptor_pool.Default().AddSerializedFile(b'\n\tBid.proto\"9\n\x03\x42id\x12\x0e\n\x06\x61mount\x18\x01 \x01(\x04\x12\x10\n\x08\x63urrency\x18\x02 \x01(\t\x12\x10\n\x08protocol\x18\x03 \x01(\tB.\xca\x02\x0e\x41pp\\Grpc\\nostr\xe2\x02\x1a\x41pp\\Grpc\\nostr\\GPBMetadatab\x06proto3')
 
 _globals = globals()
 _builder.BuildMessageAndEnumDescriptors(DESCRIPTOR, _globals)
-_builder.BuildTopDescriptorsAndMessages(DESCRIPTOR, 'Payment_pb2', _globals)
+_builder.BuildTopDescriptorsAndMessages(DESCRIPTOR, 'Bid_pb2', _globals)
 if not _descriptor._USE_C_DESCRIPTORS:
   _globals['DESCRIPTOR']._loaded_options = None
   _globals['DESCRIPTOR']._serialized_options = b'\312\002\016App\\Grpc\\nostr\342\002\032App\\Grpc\\nostr\\GPBMetadata'
-  _globals['_PAYMENT']._serialized_start=17
-  _globals['_PAYMENT']._serialized_end=134
+  _globals['_BID']._serialized_start=13
+  _globals['_BID']._serialized_end=70
 # @@protoc_insertion_point(module_scope)
```

### Comparing `openagents_grpc_proto-0.9/openagents_grpc_proto/Payment_pb2_grpc.py` & `openagents_grpc_proto-0.9.1/openagents_grpc_proto/Payment_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `openagents_grpc_proto-0.9/openagents_grpc_proto/rpc_pb2.py` & `openagents_grpc_proto-0.9.1/openagents_grpc_proto/rpc_pb2.py`

 * *Files identical despite different names*

### Comparing `openagents_grpc_proto-0.9/openagents_grpc_proto/rpc_pb2_grpc.py` & `openagents_grpc_proto-0.9.1/openagents_grpc_proto/rpc_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `openagents_grpc_proto-0.9/openagents_grpc_proto.egg-info/SOURCES.txt` & `openagents_grpc_proto-0.9.1/openagents_grpc_proto.egg-info/SOURCES.txt`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,12 @@
 MANIFEST.in
 VERSION
 setup.py
+openagents_grpc_proto/Bid_pb2.py
+openagents_grpc_proto/Bid_pb2_grpc.py
 openagents_grpc_proto/JobInput_pb2.py
 openagents_grpc_proto/JobInput_pb2_grpc.py
 openagents_grpc_proto/JobParam_pb2.py
 openagents_grpc_proto/JobParam_pb2_grpc.py
 openagents_grpc_proto/JobResult_pb2.py
 openagents_grpc_proto/JobResult_pb2_grpc.py
 openagents_grpc_proto/JobState_pb2.py
```

