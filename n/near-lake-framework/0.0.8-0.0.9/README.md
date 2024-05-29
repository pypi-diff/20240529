# Comparing `tmp/near-lake-framework-0.0.8.tar.gz` & `tmp/near_lake_framework-0.0.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "near-lake-framework-0.0.8.tar", last modified: Thu Apr 25 16:56:08 2024, max compression
+gzip compressed data, was "near_lake_framework-0.0.9.tar", last modified: Wed May 29 14:38:19 2024, max compression
```

## Comparing `near-lake-framework-0.0.8.tar` & `near_lake_framework-0.0.9.tar`

### file list

```diff
@@ -1,18 +1,19 @@
-drwxr-xr-x   0 frolik     (501) staff       (20)        0 2024-04-25 16:56:08.446586 near-lake-framework-0.0.8/
--rw-r--r--   0 frolik     (501) staff       (20)     9722 2023-10-15 22:01:13.000000 near-lake-framework-0.0.8/LICENSE-APACHE
--rw-r--r--   0 frolik     (501) staff       (20)     4617 2024-04-25 16:56:08.446505 near-lake-framework-0.0.8/PKG-INFO
--rw-r--r--   0 frolik     (501) staff       (20)     3840 2024-04-25 16:42:44.000000 near-lake-framework-0.0.8/README.md
--rw-r--r--   0 frolik     (501) staff       (20)      110 2024-04-25 16:56:08.446958 near-lake-framework-0.0.8/setup.cfg
--rw-r--r--   0 frolik     (501) staff       (20)     1139 2024-04-25 16:39:59.000000 near-lake-framework-0.0.8/setup.py
-drwxr-xr-x   0 frolik     (501) staff       (20)        0 2024-04-25 16:56:08.442794 near-lake-framework-0.0.8/src/
-drwxr-xr-x   0 frolik     (501) staff       (20)        0 2024-04-25 16:56:08.444902 near-lake-framework-0.0.8/src/near_lake_framework/
--rw-r--r--   0 frolik     (501) staff       (20)     4884 2024-04-25 16:39:35.000000 near-lake-framework-0.0.8/src/near_lake_framework/__init__.py
--rw-r--r--   0 frolik     (501) staff       (20)     4879 2023-10-15 22:01:13.000000 near-lake-framework-0.0.8/src/near_lake_framework/near_primitives.py
--rw-r--r--   0 frolik     (501) staff       (20)        0 2024-04-25 16:39:35.000000 near-lake-framework-0.0.8/src/near_lake_framework/py.typed
--rw-r--r--   0 frolik     (501) staff       (20)     2431 2024-04-25 16:53:20.000000 near-lake-framework-0.0.8/src/near_lake_framework/s3_fetchers.py
-drwxr-xr-x   0 frolik     (501) staff       (20)        0 2024-04-25 16:56:08.446211 near-lake-framework-0.0.8/src/near_lake_framework.egg-info/
--rw-r--r--   0 frolik     (501) staff       (20)     4617 2024-04-25 16:56:08.000000 near-lake-framework-0.0.8/src/near_lake_framework.egg-info/PKG-INFO
--rw-r--r--   0 frolik     (501) staff       (20)      428 2024-04-25 16:56:08.000000 near-lake-framework-0.0.8/src/near_lake_framework.egg-info/SOURCES.txt
--rw-r--r--   0 frolik     (501) staff       (20)        1 2024-04-25 16:56:08.000000 near-lake-framework-0.0.8/src/near_lake_framework.egg-info/dependency_links.txt
--rw-r--r--   0 frolik     (501) staff       (20)       75 2024-04-25 16:56:08.000000 near-lake-framework-0.0.8/src/near_lake_framework.egg-info/requires.txt
--rw-r--r--   0 frolik     (501) staff       (20)       20 2024-04-25 16:56:08.000000 near-lake-framework-0.0.8/src/near_lake_framework.egg-info/top_level.txt
+drwxr-xr-x   0 frolik     (501) staff       (20)        0 2024-05-29 14:38:19.578352 near_lake_framework-0.0.9/
+-rw-r--r--   0 frolik     (501) staff       (20)     9722 2023-10-15 22:01:13.000000 near_lake_framework-0.0.9/LICENSE-APACHE
+-rw-r--r--   0 frolik     (501) staff       (20)     5251 2024-05-29 14:38:19.578277 near_lake_framework-0.0.9/PKG-INFO
+-rw-r--r--   0 frolik     (501) staff       (20)     4283 2024-05-29 14:09:55.000000 near_lake_framework-0.0.9/README.md
+-rw-r--r--   0 frolik     (501) staff       (20)      110 2024-05-29 14:38:19.578603 near_lake_framework-0.0.9/setup.cfg
+-rw-r--r--   0 frolik     (501) staff       (20)     1310 2024-05-29 14:31:54.000000 near_lake_framework-0.0.9/setup.py
+drwxr-xr-x   0 frolik     (501) staff       (20)        0 2024-05-29 14:38:19.574223 near_lake_framework-0.0.9/src/
+drwxr-xr-x   0 frolik     (501) staff       (20)        0 2024-05-29 14:38:19.576452 near_lake_framework-0.0.9/src/near_lake_framework/
+-rw-r--r--   0 frolik     (501) staff       (20)     5134 2024-05-29 14:26:30.000000 near_lake_framework-0.0.9/src/near_lake_framework/__init__.py
+-rw-r--r--   0 frolik     (501) staff       (20)     4967 2024-05-29 14:10:02.000000 near_lake_framework-0.0.9/src/near_lake_framework/near_primitives.py
+-rw-r--r--   0 frolik     (501) staff       (20)        0 2024-04-25 16:39:35.000000 near_lake_framework-0.0.9/src/near_lake_framework/py.typed
+-rw-r--r--   0 frolik     (501) staff       (20)     2865 2024-05-29 14:21:47.000000 near_lake_framework-0.0.9/src/near_lake_framework/s3_fetchers.py
+-rw-r--r--   0 frolik     (501) staff       (20)      992 2024-05-29 14:09:55.000000 near_lake_framework-0.0.9/src/near_lake_framework/utils.py
+drwxr-xr-x   0 frolik     (501) staff       (20)        0 2024-05-29 14:38:19.578006 near_lake_framework-0.0.9/src/near_lake_framework.egg-info/
+-rw-r--r--   0 frolik     (501) staff       (20)     5251 2024-05-29 14:38:19.000000 near_lake_framework-0.0.9/src/near_lake_framework.egg-info/PKG-INFO
+-rw-r--r--   0 frolik     (501) staff       (20)      461 2024-05-29 14:38:19.000000 near_lake_framework-0.0.9/src/near_lake_framework.egg-info/SOURCES.txt
+-rw-r--r--   0 frolik     (501) staff       (20)        1 2024-05-29 14:38:19.000000 near_lake_framework-0.0.9/src/near_lake_framework.egg-info/dependency_links.txt
+-rw-r--r--   0 frolik     (501) staff       (20)      191 2024-05-29 14:38:19.000000 near_lake_framework-0.0.9/src/near_lake_framework.egg-info/requires.txt
+-rw-r--r--   0 frolik     (501) staff       (20)       20 2024-05-29 14:38:19.000000 near_lake_framework-0.0.9/src/near_lake_framework.egg-info/top_level.txt
```

### Comparing `near-lake-framework-0.0.8/LICENSE-APACHE` & `near_lake_framework-0.0.9/LICENSE-APACHE`

 * *Files identical despite different names*

### Comparing `near-lake-framework-0.0.8/PKG-INFO` & `near_lake_framework-0.0.9/README.md`

 * *Files 11% similar despite different names*

```diff
@@ -1,27 +1,7 @@
-Metadata-Version: 2.1
-Name: near-lake-framework
-Version: 0.0.8
-Summary: Python Library to connect to the NEAR Lake S3 and stream the data
-Home-page: https://github.com/frolvanya/near-lake-framework-py
-Author: Ivan Frolov
-Author-email: frolvanya@gmail.com
-Project-URL: Bug Tracker, https://github.com/frolvanya/near-lake-framework-py/issues
-Classifier: Programming Language :: Python :: 3
-Classifier: License :: OSI Approved :: MIT License
-Classifier: License :: OSI Approved :: Apache Software License
-Classifier: Operating System :: OS Independent
-Requires-Python: >=3.9
-Description-Content-Type: text/markdown
-License-File: LICENSE-APACHE
-Requires-Dist: asyncio>=3.4.3
-Requires-Dist: dataclasses>=0.6
-Requires-Dist: dataclasses-json>=0.5.7
-Requires-Dist: aiobotocore>=2.3.0
-
 # NEAR Lake Framework for Python
 
 Available in programming languages: [Rust](https://github.com/near/near-lake-framework-rs) | [Javascript](https://github.com/near/near-lake-framework-js) | **Python3**
 
 NEAR Lake Framework is a small library companion to [NEAR Lake](https://github.com/near/near-lake). It allows you to build
 your own indexer that subscribes to the stream of blocks from the NEAR Lake data source and create your own logic to process
 the NEAR Protocol data.
@@ -36,37 +16,52 @@
 
 ---
 
 ## Example
 
 ```python3
 import asyncio
+import logging
 import os
 
 from near_lake_framework import LakeConfig, streamer, Network
+from near_lake_framework.utils import fetch_latest_block
+
+# Suppress warning logs from specific dependencies
+logging.getLogger("near_lake_framework").setLevel(logging.INFO)
 
 
 async def main():
+    network = Network.TESTNET
+    latest_final_block = fetch_latest_block(network=network)
     config = LakeConfig(
-        network=Network.MAINNET,
-        aws_access_key_id=os.getenv("AWS_ACCESS_KEY_ID"),
-        aws_secret_key=os.getenv("AWS_SECRET_ACCESS_KEY"),
-        start_block_height=69130938,
+        network,
+        start_block_height=latest_final_block,
+        # These fields must be set!
+        aws_access_key_id=os.environ["AWS_ACCESS_KEY_ID"],
+        aws_secret_key=os.environ["AWS_SECRET_ACCESS_KEY"],
     )
 
     stream_handle, streamer_messages_queue = streamer(config)
     while True:
         streamer_message = await streamer_messages_queue.get()
         print(
             f"Received Block #{streamer_message.block.header.height} from Lake Framework"
         )
 
 
-loop = asyncio.get_event_loop()
-loop.run_until_complete(main())
+if __name__ == "__main__":
+    loop = asyncio.new_event_loop()
+    loop.run_until_complete(main())
+```
+
+Try it yourself as follows
+```shell
+pip3 install -r requirements.txt
+python3 example/run.py
 ```
 
 ## How to use
 
 ### Dependencies
 
 Install `near-lake-framework`
```

### Comparing `near-lake-framework-0.0.8/setup.py` & `near_lake_framework-0.0.9/setup.py`

 * *Files 22% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 import setuptools
 
 with open("README.md", "r", encoding="utf-8") as fh:
     long_description = fh.read()
 
 setuptools.setup(
     name="near-lake-framework",
-    version="0.0.8",
+    version="0.0.9",
     author="Ivan Frolov",
     author_email="frolvanya@gmail.com",
     description="Python Library to connect to the NEAR Lake S3 and stream the data",
     long_description=long_description,
     long_description_content_type="text/markdown",
     url="https://github.com/frolvanya/near-lake-framework-py",
     project_urls={
@@ -23,12 +23,17 @@
     ],
     package_dir={"": "src"},
     packages=setuptools.find_packages(where="src"),
     python_requires=">=3.9",
     install_requires=[
         "asyncio>=3.4.3",
         "dataclasses>=0.6",
-        "dataclasses-json>=0.5.7",
-        "aiobotocore>=2.3.0",
+        "dataclasses-json>=0.6.6",
+        "botocore>=1.34.70",
+        "aiobotocore>=2.13.0",
+        "requests>=2.32.2",
+        "types-botocore>=1.0.2",
+        "types-aiobotocore>=2.13.0",
+        "types-requests>=2.32.0.20240523",
     ],
     package_data={"near_lake_framework": ["py.typed"]},
 )
```

### Comparing `near-lake-framework-0.0.8/src/near_lake_framework/__init__.py` & `near_lake_framework-0.0.9/src/near_lake_framework/__init__.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,20 +1,27 @@
 from __future__ import annotations
 import asyncio
 import itertools
 from enum import Enum
+
+import logging
 from typing import Optional
+from dataclasses import dataclass
 
-from aiobotocore.session import get_session  # type: ignore
+from aiobotocore.session import get_session
 
 from near_lake_framework import near_primitives
 from near_lake_framework import s3_fetchers
 
 
-from dataclasses import dataclass
+# Configure logging
+logging.basicConfig(
+    level=logging.INFO, format="%(asctime)s %(levelname)s %(name)s %(message)s"
+)
+logger = logging.getLogger(__name__)
 
 
 class Network(Enum):
     MAINNET = "mainnet"
     TESTNET = "testnet"
 
     @staticmethod
@@ -39,15 +46,15 @@
     s3_bucket_name: str
     s3_region_name: str
     aws_access_key_id: str
     aws_secret_key: str
     start_block_height: near_primitives.BlockHeight
     blocks_preload_pool_size: int = 200
 
-    def __init__(
+    def __init__(  # pylint: disable=too-many-arguments
         self,
         network: Network,
         aws_access_key_id: str,
         aws_secret_key: str,
         start_block_height: near_primitives.BlockHeight,
         preload_pool_size: int = 200,
     ):
@@ -77,20 +84,20 @@
                 s3_client,
                 config.s3_bucket_name,
                 start_from_block_height,
                 config.blocks_preload_pool_size * 2,
             )
 
             if not block_heights_prefixes:
-                print("No new blocks on S3, retry in 2s...")
+                logger.info("No new blocks on S3, retry in 2s...")
 
                 await asyncio.sleep(2)
                 continue
 
-            print("Received {} blocks from S3".format(len(block_heights_prefixes)))
+            logger.info("Received %d blocks from S3", len(block_heights_prefixes))
 
             pending_block_heights = iter(block_heights_prefixes)
             streamer_messages_futures = []
             for block_height in itertools.islice(
                 pending_block_heights, streamer_messages_queue.maxsize
             ):
                 streamer_messages_futures.append(
@@ -105,16 +112,17 @@
                 streamer_message = await streamer_messages_futures.pop(0)
 
                 if (
                     last_processed_block_hash
                     and last_processed_block_hash
                     != streamer_message.block.header.prev_hash
                 ):
-                    print(
-                        "`prev_hash` does not match, refetching the data from S3 in 200ms",
+                    logger.warning(
+                        "`prev_hash` does not match, re-fetching the data from S3 in 200ms: "
+                        "%s != %s",
                         last_processed_block_hash,
                         streamer_message.block.header.prev_hash,
                     )
 
                     await asyncio.sleep(0.2)
                     break
```

### Comparing `near-lake-framework-0.0.8/src/near_lake_framework/near_primitives.py` & `near_lake_framework-0.0.9/src/near_lake_framework/near_primitives.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,29 +1,30 @@
-from typing import Any, List, Optional
+from typing import Any, Optional
 
 from dataclasses import dataclass, field
 from dataclasses_json import DataClassJsonMixin, config, mm
 
 
 AccountId = str
 CryptoHash = str
 BlockHeight = int
 
 
 class BlockHeightField(mm.fields.Integer):
-    """Block Height is unsigned 64-bit integer, so it needs to be serialized as a string and get deserialized
-    to an integer type in Python.
+    """
+    Block Height is unsigned 64-bit integer, so it needs to be serialized
+    as a string and get deserialized to an integer type in Python.
     """
 
     def __init__(self, *args, **kwargs):
-        return super().__init__(*args, **kwargs, as_string=True)
+        super().__init__(*args, **kwargs, as_string=True)
 
 
 @dataclass
-class BlockHeader(DataClassJsonMixin):
+class BlockHeader(DataClassJsonMixin):  # pylint: disable=too-many-instance-attributes
     epoch_id: CryptoHash
     next_epoch_id: CryptoHash
     hash: CryptoHash
     prev_hash: CryptoHash
     prev_state_root: CryptoHash
     chunk_receipts_root: CryptoHash
     chunk_headers_root: CryptoHash
@@ -32,42 +33,42 @@
     chunks_included: int
     challenges_root: CryptoHash
     timestamp: int
     timestamp_nanosec: int = field(
         metadata=config(mm_field=mm.fields.Integer(as_string=True))
     )
     random_value: CryptoHash
-    validator_proposals: List[Any]
-    chunk_mask: List[bool]
+    validator_proposals: list[Any]
+    chunk_mask: list[bool]
     gas_price: int = field(metadata=config(mm_field=mm.fields.Integer(as_string=True)))
     block_ordinal: Optional[int]
     rent_paid: int = field(metadata=config(mm_field=mm.fields.Integer(as_string=True)))
     validator_reward: int = field(
         metadata=config(mm_field=mm.fields.Integer(as_string=True))
     )
     total_supply: int = field(
         metadata=config(mm_field=mm.fields.Integer(as_string=True))
     )
-    challenges_result: List[Any]
+    challenges_result: list[Any]
     last_final_block: CryptoHash
     last_ds_final_block: CryptoHash
     next_bp_hash: CryptoHash
     block_merkle_root: CryptoHash
     epoch_sync_data_hash: Optional[CryptoHash]
-    approvals: List[Optional[str]]
+    approvals: list[Optional[str]]
     signature: str
     latest_protocol_version: int
     height: BlockHeight = field(metadata=config(mm_field=BlockHeightField()))
     prev_height: Optional[BlockHeight] = field(
         default=None, metadata=config(mm_field=BlockHeightField())
     )
 
 
 @dataclass
-class ChunkHeader(DataClassJsonMixin):
+class ChunkHeader(DataClassJsonMixin):  # pylint: disable=too-many-instance-attributes
     chunk_hash: CryptoHash
     prev_block_hash: CryptoHash
     outcome_root: CryptoHash
     prev_state_root: CryptoHash
     encoded_merkle_root: CryptoHash
     encoded_length: int
     height_created: int
@@ -80,23 +81,23 @@
         metadata=config(mm_field=mm.fields.Integer(as_string=True))
     )
     balance_burnt: int = field(
         metadata=config(mm_field=mm.fields.Integer(as_string=True))
     )
     outgoing_receipts_root: CryptoHash
     tx_root: CryptoHash
-    validator_proposals: List[Any]
+    validator_proposals: list[Any]
     signature: str
 
 
 @dataclass
 class Block(DataClassJsonMixin):
     author: AccountId
     header: BlockHeader
-    chunks: List[ChunkHeader]
+    chunks: list[ChunkHeader]
 
 
 @dataclass
 class Receipt(DataClassJsonMixin):
     predecessor_id: AccountId
     receiver_id: AccountId
     receipt_id: CryptoHash
@@ -109,33 +110,33 @@
     cost: str
     gas_used: int
 
 
 @dataclass
 class ExecutionMetadata(DataClassJsonMixin):
     version: int
-    gas_profile: Optional[List[CostGasUsed]]
+    gas_profile: Optional[list[CostGasUsed]]
 
 
 @dataclass
 class ExecutionOutcome(DataClassJsonMixin):
-    logs: List[str]
-    receipt_ids: List[CryptoHash]
+    logs: list[str]
+    receipt_ids: list[CryptoHash]
     gas_burnt: int
     tokens_burnt: int = field(
         metadata=config(mm_field=mm.fields.Integer(as_string=True))
     )
     executor_id: AccountId
     status: Any
     metadata: ExecutionMetadata
 
 
 @dataclass
 class ExecutionOutcomeWithId(DataClassJsonMixin):
-    proof: List[Any]
+    proof: list[Any]
     block_hash: CryptoHash
     id: CryptoHash
     outcome: ExecutionOutcome
 
 
 @dataclass
 class IndexerExecutionOutcomeWithReceipt(DataClassJsonMixin):
@@ -145,15 +146,15 @@
 
 @dataclass
 class SignedTransaction(DataClassJsonMixin):
     signer_id: AccountId
     public_key: str
     nonce: int
     receiver_id: AccountId
-    actions: List[Any]
+    actions: list[Any]
     signature: str
     hash: CryptoHash
 
 
 @dataclass
 class IndexerExecutionOutcomeWithOptionalReceipt:
     execution_outcome: ExecutionOutcomeWithId
@@ -166,23 +167,23 @@
     outcome: IndexerExecutionOutcomeWithOptionalReceipt
 
 
 @dataclass
 class IndexerChunk(DataClassJsonMixin):
     author: AccountId
     header: ChunkHeader
-    transactions: List[IndexerTransactionWithOutcome]
-    receipts: List[Receipt]
+    transactions: list[IndexerTransactionWithOutcome]
+    receipts: list[Receipt]
 
 
 @dataclass
 class IndexerShard(DataClassJsonMixin):
     shard_id: int
     chunk: Optional[IndexerChunk]
-    receipt_execution_outcomes: List[IndexerExecutionOutcomeWithReceipt]
-    state_changes: List[Any]
+    receipt_execution_outcomes: list[IndexerExecutionOutcomeWithReceipt]
+    state_changes: list[Any]
 
 
 @dataclass
 class StreamerMessage(DataClassJsonMixin):
     block: Block
-    shards: List[IndexerShard]
+    shards: list[IndexerShard]
```

### Comparing `near-lake-framework-0.0.8/src/near_lake_framework/s3_fetchers.py` & `near_lake_framework-0.0.9/src/near_lake_framework/s3_fetchers.py`

 * *Files 26% similar despite different names*

```diff
@@ -1,80 +1,86 @@
 import asyncio
 import logging
-from typing import List
 import traceback
-from botocore.exceptions import ClientError
+from botocore.exceptions import ClientError, EndpointConnectionError
 
 from near_lake_framework import near_primitives
 
 
 async def list_blocks(
     s3_client,
     s3_bucket_name: str,
     start_from_block_height: near_primitives.BlockHeight,
     number_of_blocks_requested: int,
-) -> List[near_primitives.BlockHeight]:
+) -> list[near_primitives.BlockHeight]:
     response = await s3_client.list_objects_v2(
         Bucket=s3_bucket_name,
         Delimiter="/",
         MaxKeys=number_of_blocks_requested,
-        StartAfter="{:012d}".format(start_from_block_height),
+        StartAfter=f"{start_from_block_height:012d}",
         RequestPayer="requester",
     )
 
     return [
         near_primitives.BlockHeight(prefix.get("Prefix")[:-1])
         for prefix in response.get("CommonPrefixes", [])
     ]
 
 
 async def fetch_streamer_message(
     s3_client, s3_bucket_name: str, block_height: near_primitives.BlockHeight
 ) -> near_primitives.StreamerMessage:
     response = await s3_client.get_object(
         Bucket=s3_bucket_name,
-        Key="{:012d}/block.json".format(block_height),
+        Key=f"{block_height:012d}/block.json",
         RequestPayer="requester",
     )
 
     async with response["Body"] as stream:
         body = await stream.read()
 
     block = near_primitives.Block.from_json(body)
 
     shards_fetching = [
         fetch_shard_or_retry(s3_client, s3_bucket_name, block_height, shard_id)
         for shard_id in range(len(block.chunks))
     ]
     shards = await asyncio.gather(*shards_fetching)
 
-    return near_primitives.StreamerMessage(block, shards)
+    return near_primitives.StreamerMessage(block, list(shards))
 
 
 async def fetch_shard_or_retry(
     s3_client,
     s3_bucket_name: str,
     block_height: near_primitives.BlockHeight,
     shard_id: int,
 ) -> near_primitives.IndexerShard:
     while True:
-        shard_key = "{:012d}/shard_{}.json".format(block_height, shard_id)
+        shard_key = f"{block_height:012d}/shard_{shard_id}.json"
         try:
             response = await s3_client.get_object(
                 Bucket=s3_bucket_name,
                 Key=shard_key,
                 RequestPayer="requester",
             )
 
             async with response["Body"] as stream:
                 body = await stream.read()
 
             return near_primitives.IndexerShard.from_json(body)
         except ClientError as e:
             if e.response["Error"]["Code"] == "NoSuchKey":
-                logging.warning(
-                    "Failed to fetch shard {} - does not exist".format(shard_key)
-                )
+                logging.warning("Failed to fetch shard %s - doesn't exist", shard_key)
             else:
                 traceback.print_exc()
-        except Exception:
+        except EndpointConnectionError as e:
+            logging.error(
+                "EndpointConnectionError while fetching shard %s: %s", shard_key, e
+            )
+            traceback.print_exc()
+        except asyncio.TimeoutError as e:
+            logging.error("TimeoutError while fetching shard %s: %s", shard_key, e)
+            traceback.print_exc()
+        except Exception as e:  # pylint: disable=broad-exception-caught
+            logging.error("Unexpected error while fetching shard %s: %s", shard_key, e)
             traceback.print_exc()
```

### Comparing `near-lake-framework-0.0.8/src/near_lake_framework.egg-info/PKG-INFO` & `near_lake_framework-0.0.9/PKG-INFO`

 * *Files 16% similar despite different names*

```diff
@@ -1,26 +1,31 @@
 Metadata-Version: 2.1
 Name: near-lake-framework
-Version: 0.0.8
+Version: 0.0.9
 Summary: Python Library to connect to the NEAR Lake S3 and stream the data
 Home-page: https://github.com/frolvanya/near-lake-framework-py
 Author: Ivan Frolov
 Author-email: frolvanya@gmail.com
 Project-URL: Bug Tracker, https://github.com/frolvanya/near-lake-framework-py/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.9
 Description-Content-Type: text/markdown
 License-File: LICENSE-APACHE
 Requires-Dist: asyncio>=3.4.3
 Requires-Dist: dataclasses>=0.6
-Requires-Dist: dataclasses-json>=0.5.7
-Requires-Dist: aiobotocore>=2.3.0
+Requires-Dist: dataclasses-json>=0.6.6
+Requires-Dist: botocore>=1.34.70
+Requires-Dist: aiobotocore>=2.13.0
+Requires-Dist: requests>=2.32.2
+Requires-Dist: types-botocore>=1.0.2
+Requires-Dist: types-aiobotocore>=2.13.0
+Requires-Dist: types-requests>=2.32.0.20240523
 
 # NEAR Lake Framework for Python
 
 Available in programming languages: [Rust](https://github.com/near/near-lake-framework-rs) | [Javascript](https://github.com/near/near-lake-framework-js) | **Python3**
 
 NEAR Lake Framework is a small library companion to [NEAR Lake](https://github.com/near/near-lake). It allows you to build
 your own indexer that subscribes to the stream of blocks from the NEAR Lake data source and create your own logic to process
@@ -36,37 +41,52 @@
 
 ---
 
 ## Example
 
 ```python3
 import asyncio
+import logging
 import os
 
 from near_lake_framework import LakeConfig, streamer, Network
+from near_lake_framework.utils import fetch_latest_block
+
+# Suppress warning logs from specific dependencies
+logging.getLogger("near_lake_framework").setLevel(logging.INFO)
 
 
 async def main():
+    network = Network.TESTNET
+    latest_final_block = fetch_latest_block(network=network)
     config = LakeConfig(
-        network=Network.MAINNET,
-        aws_access_key_id=os.getenv("AWS_ACCESS_KEY_ID"),
-        aws_secret_key=os.getenv("AWS_SECRET_ACCESS_KEY"),
-        start_block_height=69130938,
+        network,
+        start_block_height=latest_final_block,
+        # These fields must be set!
+        aws_access_key_id=os.environ["AWS_ACCESS_KEY_ID"],
+        aws_secret_key=os.environ["AWS_SECRET_ACCESS_KEY"],
     )
 
     stream_handle, streamer_messages_queue = streamer(config)
     while True:
         streamer_message = await streamer_messages_queue.get()
         print(
             f"Received Block #{streamer_message.block.header.height} from Lake Framework"
         )
 
 
-loop = asyncio.get_event_loop()
-loop.run_until_complete(main())
+if __name__ == "__main__":
+    loop = asyncio.new_event_loop()
+    loop.run_until_complete(main())
+```
+
+Try it yourself as follows
+```shell
+pip3 install -r requirements.txt
+python3 example/run.py
 ```
 
 ## How to use
 
 ### Dependencies
 
 Install `near-lake-framework`
```

