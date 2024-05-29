# Comparing `tmp/torchsnapshot_nightly-2024.5.27.tar.gz` & `tmp/torchsnapshot_nightly-2024.5.28.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "torchsnapshot_nightly-2024.5.27.tar", last modified: Mon May 27 11:31:38 2024, max compression
+gzip compressed data, was "torchsnapshot_nightly-2024.5.28.tar", last modified: Tue May 28 11:30:48 2024, max compression
```

## Comparing `torchsnapshot_nightly-2024.5.27.tar` & `torchsnapshot_nightly-2024.5.28.tar`

### file list

```diff
@@ -1,88 +1,88 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-27 11:31:38.825688 torchsnapshot_nightly-2024.5.27/
--rw-r--r--   0 runner    (1001) docker     (127)     1538 2024-05-27 11:30:35.000000 torchsnapshot_nightly-2024.5.27/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)     5018 2024-05-27 11:31:38.825688 torchsnapshot_nightly-2024.5.27/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     3451 2024-05-27 11:30:35.000000 torchsnapshot_nightly-2024.5.27/README.md
--rw-r--r--   0 runner    (1001) docker     (127)       44 2024-05-27 11:30:35.000000 torchsnapshot_nightly-2024.5.27/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-27 11:31:38.825688 torchsnapshot_nightly-2024.5.27/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)     3175 2024-05-27 11:30:35.000000 torchsnapshot_nightly-2024.5.27/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-27 11:31:38.813688 torchsnapshot_nightly-2024.5.27/tests/
--rw-r--r--   0 runner    (1001) docker     (127)     4411 2024-05-27 11:30:35.000000 torchsnapshot_nightly-2024.5.27/tests/test_async_take.py
--rw-r--r--   0 runner    (1001) docker     (127)    13778 2024-05-27 11:30:35.000000 torchsnapshot_nightly-2024.5.27/tests/test_batcher.py
--rw-r--r--   0 runner    (1001) docker     (127)    11630 2024-05-27 11:30:35.000000 torchsnapshot_nightly-2024.5.27/tests/test_chunked_tensor_io_preparer.py
--rw-r--r--   0 runner    (1001) docker     (127)     6789 2024-05-27 11:30:35.000000 torchsnapshot_nightly-2024.5.27/tests/test_ddp.py
--rw-r--r--   0 runner    (1001) docker     (127)     4133 2024-05-27 11:30:35.000000 torchsnapshot_nightly-2024.5.27/tests/test_ddp_infer_replication.py
--rw-r--r--   0 runner    (1001) docker     (127)     1734 2024-05-27 11:30:35.000000 torchsnapshot_nightly-2024.5.27/tests/test_ddp_replication_glob.py
--rw-r--r--   0 runner    (1001) docker     (127)     6849 2024-05-27 11:30:35.000000 torchsnapshot_nightly-2024.5.27/tests/test_dist_store.py
--rw-r--r--   0 runner    (1001) docker     (127)     7005 2024-05-27 11:30:35.000000 torchsnapshot_nightly-2024.5.27/tests/test_flatten.py
--rw-r--r--   0 runner    (1001) docker     (127)     2130 2024-05-27 11:30:35.000000 torchsnapshot_nightly-2024.5.27/tests/test_fs_storage_plugin.py
--rw-r--r--   0 runner    (1001) docker     (127)     4162 2024-05-27 11:30:35.000000 torchsnapshot_nightly-2024.5.27/tests/test_gcs_storage_plugin.py
--rw-r--r--   0 runner    (1001) docker     (127)    27126 2024-05-27 11:30:35.000000 torchsnapshot_nightly-2024.5.27/tests/test_manifest.py
--rw-r--r--   0 runner    (1001) docker     (127)     1812 2024-05-27 11:30:35.000000 torchsnapshot_nightly-2024.5.27/tests/test_memoryview_stream.py
--rw-r--r--   0 runner    (1001) docker     (127)     8806 2024-05-27 11:30:35.000000 torchsnapshot_nightly-2024.5.27/tests/test_partitioner.py
--rw-r--r--   0 runner    (1001) docker     (127)     1838 2024-05-27 11:30:35.000000 torchsnapshot_nightly-2024.5.27/tests/test_pg_wrapper.py
--rw-r--r--   0 runner    (1001) docker     (127)     5779 2024-05-27 11:30:35.000000 torchsnapshot_nightly-2024.5.27/tests/test_read_object.py
--rw-r--r--   0 runner    (1001) docker     (127)     3355 2024-05-27 11:30:35.000000 torchsnapshot_nightly-2024.5.27/tests/test_replication_glob.py
--rw-r--r--   0 runner    (1001) docker     (127)     1101 2024-05-27 11:30:35.000000 torchsnapshot_nightly-2024.5.27/tests/test_rng_state.py
--rw-r--r--   0 runner    (1001) docker     (127)      574 2024-05-27 11:30:35.000000 torchsnapshot_nightly-2024.5.27/tests/test_rss_profiler.py
--rw-r--r--   0 runner    (1001) docker     (127)     3356 2024-05-27 11:30:35.000000 torchsnapshot_nightly-2024.5.27/tests/test_s3_storage_plugin.py
--rw-r--r--   0 runner    (1001) docker     (127)     4036 2024-05-27 11:30:35.000000 torchsnapshot_nightly-2024.5.27/tests/test_serialization.py
--rw-r--r--   0 runner    (1001) docker     (127)    10067 2024-05-27 11:30:35.000000 torchsnapshot_nightly-2024.5.27/tests/test_sharded_tensor_io_preparer.py
--rw-r--r--   0 runner    (1001) docker     (127)     3470 2024-05-27 11:30:35.000000 torchsnapshot_nightly-2024.5.27/tests/test_sharded_tensor_resharding.py
--rw-r--r--   0 runner    (1001) docker     (127)     7905 2024-05-27 11:30:35.000000 torchsnapshot_nightly-2024.5.27/tests/test_snapshot.py
--rw-r--r--   0 runner    (1001) docker     (127)     2391 2024-05-27 11:30:35.000000 torchsnapshot_nightly-2024.5.27/tests/test_state_dict.py
--rw-r--r--   0 runner    (1001) docker     (127)    13669 2024-05-27 11:30:35.000000 torchsnapshot_nightly-2024.5.27/tests/test_tensor_io_preparer.py
--rw-r--r--   0 runner    (1001) docker     (127)     5075 2024-05-27 11:30:35.000000 torchsnapshot_nightly-2024.5.27/tests/test_test_utils.py
--rw-r--r--   0 runner    (1001) docker     (127)      978 2024-05-27 11:30:35.000000 torchsnapshot_nightly-2024.5.27/tests/test_uvm_tensor.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-27 11:31:38.821688 torchsnapshot_nightly-2024.5.27/torchsnapshot/
--rw-r--r--   0 runner    (1001) docker     (127)     1153 2024-05-27 11:30:35.000000 torchsnapshot_nightly-2024.5.27/torchsnapshot/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    17905 2024-05-27 11:30:35.000000 torchsnapshot_nightly-2024.5.27/torchsnapshot/batcher.py
--rw-r--r--   0 runner    (1001) docker     (127)     6158 2024-05-27 11:30:35.000000 torchsnapshot_nightly-2024.5.27/torchsnapshot/dist_store.py
--rw-r--r--   0 runner    (1001) docker     (127)     2322 2024-05-27 11:30:35.000000 torchsnapshot_nightly-2024.5.27/torchsnapshot/dtensor_utils.py
--rw-r--r--   0 runner    (1001) docker     (127)      729 2024-05-27 11:30:35.000000 torchsnapshot_nightly-2024.5.27/torchsnapshot/event.py
--rw-r--r--   0 runner    (1001) docker     (127)     1520 2024-05-27 11:30:35.000000 torchsnapshot_nightly-2024.5.27/torchsnapshot/event_handlers.py
--rw-r--r--   0 runner    (1001) docker     (127)     7696 2024-05-27 11:30:35.000000 torchsnapshot_nightly-2024.5.27/torchsnapshot/flatten.py
--rw-r--r--   0 runner    (1001) docker     (127)     6346 2024-05-27 11:30:35.000000 torchsnapshot_nightly-2024.5.27/torchsnapshot/io_preparer.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-27 11:31:38.821688 torchsnapshot_nightly-2024.5.27/torchsnapshot/io_preparers/
--rw-r--r--   0 runner    (1001) docker     (127)      223 2024-05-27 11:30:35.000000 torchsnapshot_nightly-2024.5.27/torchsnapshot/io_preparers/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     4354 2024-05-27 11:30:35.000000 torchsnapshot_nightly-2024.5.27/torchsnapshot/io_preparers/chunked_tensor.py
--rw-r--r--   0 runner    (1001) docker     (127)    10746 2024-05-27 11:30:35.000000 torchsnapshot_nightly-2024.5.27/torchsnapshot/io_preparers/dtensor.py
--rw-r--r--   0 runner    (1001) docker     (127)     2677 2024-05-27 11:30:35.000000 torchsnapshot_nightly-2024.5.27/torchsnapshot/io_preparers/object.py
--rw-r--r--   0 runner    (1001) docker     (127)    12707 2024-05-27 11:30:35.000000 torchsnapshot_nightly-2024.5.27/torchsnapshot/io_preparers/sharded_tensor.py
--rw-r--r--   0 runner    (1001) docker     (127)    15281 2024-05-27 11:30:35.000000 torchsnapshot_nightly-2024.5.27/torchsnapshot/io_preparers/tensor.py
--rw-r--r--   0 runner    (1001) docker     (127)     2679 2024-05-27 11:30:35.000000 torchsnapshot_nightly-2024.5.27/torchsnapshot/io_types.py
--rw-r--r--   0 runner    (1001) docker     (127)     4210 2024-05-27 11:30:35.000000 torchsnapshot_nightly-2024.5.27/torchsnapshot/knobs.py
--rw-r--r--   0 runner    (1001) docker     (127)    15513 2024-05-27 11:30:35.000000 torchsnapshot_nightly-2024.5.27/torchsnapshot/manifest.py
--rw-r--r--   0 runner    (1001) docker     (127)    10432 2024-05-27 11:30:35.000000 torchsnapshot_nightly-2024.5.27/torchsnapshot/manifest_ops.py
--rw-r--r--   0 runner    (1001) docker     (127)     3247 2024-05-27 11:30:35.000000 torchsnapshot_nightly-2024.5.27/torchsnapshot/manifest_utils.py
--rw-r--r--   0 runner    (1001) docker     (127)     2554 2024-05-27 11:30:35.000000 torchsnapshot_nightly-2024.5.27/torchsnapshot/memoryview_stream.py
--rw-r--r--   0 runner    (1001) docker     (127)    13859 2024-05-27 11:30:35.000000 torchsnapshot_nightly-2024.5.27/torchsnapshot/partitioner.py
--rw-r--r--   0 runner    (1001) docker     (127)     2917 2024-05-27 11:30:35.000000 torchsnapshot_nightly-2024.5.27/torchsnapshot/pg_wrapper.py
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-27 11:30:35.000000 torchsnapshot_nightly-2024.5.27/torchsnapshot/py.typed
--rw-r--r--   0 runner    (1001) docker     (127)     1344 2024-05-27 11:30:35.000000 torchsnapshot_nightly-2024.5.27/torchsnapshot/rng_state.py
--rw-r--r--   0 runner    (1001) docker     (127)     1581 2024-05-27 11:30:35.000000 torchsnapshot_nightly-2024.5.27/torchsnapshot/rss_profiler.py
--rw-r--r--   0 runner    (1001) docker     (127)    16831 2024-05-27 11:30:35.000000 torchsnapshot_nightly-2024.5.27/torchsnapshot/scheduler.py
--rw-r--r--   0 runner    (1001) docker     (127)    15262 2024-05-27 11:30:35.000000 torchsnapshot_nightly-2024.5.27/torchsnapshot/serialization.py
--rw-r--r--   0 runner    (1001) docker     (127)    40127 2024-05-27 11:30:35.000000 torchsnapshot_nightly-2024.5.27/torchsnapshot/snapshot.py
--rw-r--r--   0 runner    (1001) docker     (127)      874 2024-05-27 11:30:35.000000 torchsnapshot_nightly-2024.5.27/torchsnapshot/state_dict.py
--rw-r--r--   0 runner    (1001) docker     (127)      570 2024-05-27 11:30:35.000000 torchsnapshot_nightly-2024.5.27/torchsnapshot/stateful.py
--rw-r--r--   0 runner    (1001) docker     (127)     2675 2024-05-27 11:30:35.000000 torchsnapshot_nightly-2024.5.27/torchsnapshot/storage_plugin.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-27 11:31:38.821688 torchsnapshot_nightly-2024.5.27/torchsnapshot/storage_plugins/
--rw-r--r--   0 runner    (1001) docker     (127)      223 2024-05-27 11:30:35.000000 torchsnapshot_nightly-2024.5.27/torchsnapshot/storage_plugins/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1915 2024-05-27 11:30:35.000000 torchsnapshot_nightly-2024.5.27/torchsnapshot/storage_plugins/fs.py
--rw-r--r--   0 runner    (1001) docker     (127)     9807 2024-05-27 11:30:35.000000 torchsnapshot_nightly-2024.5.27/torchsnapshot/storage_plugins/gcs.py
--rw-r--r--   0 runner    (1001) docker     (127)     3001 2024-05-27 11:30:35.000000 torchsnapshot_nightly-2024.5.27/torchsnapshot/storage_plugins/s3.py
--rw-r--r--   0 runner    (1001) docker     (127)     9949 2024-05-27 11:30:35.000000 torchsnapshot_nightly-2024.5.27/torchsnapshot/test_utils.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-27 11:31:38.821688 torchsnapshot_nightly-2024.5.27/torchsnapshot/tricks/
--rw-r--r--   0 runner    (1001) docker     (127)      208 2024-05-27 11:30:35.000000 torchsnapshot_nightly-2024.5.27/torchsnapshot/tricks/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1419 2024-05-27 11:30:35.000000 torchsnapshot_nightly-2024.5.27/torchsnapshot/tricks/ddp.py
--rw-r--r--   0 runner    (1001) docker     (127)     3405 2024-05-27 11:30:35.000000 torchsnapshot_nightly-2024.5.27/torchsnapshot/tricks/deepspeed.py
--rw-r--r--   0 runner    (1001) docker     (127)     1821 2024-05-27 11:30:35.000000 torchsnapshot_nightly-2024.5.27/torchsnapshot/tricks/fsdp.py
--rw-r--r--   0 runner    (1001) docker     (127)     1019 2024-05-27 11:30:35.000000 torchsnapshot_nightly-2024.5.27/torchsnapshot/uvm_tensor.py
--rw-r--r--   0 runner    (1001) docker     (127)      539 2024-05-27 11:30:35.000000 torchsnapshot_nightly-2024.5.27/torchsnapshot/version.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-27 11:31:38.821688 torchsnapshot_nightly-2024.5.27/torchsnapshot_nightly.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     5018 2024-05-27 11:31:38.000000 torchsnapshot_nightly-2024.5.27/torchsnapshot_nightly.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     2375 2024-05-27 11:31:38.000000 torchsnapshot_nightly-2024.5.27/torchsnapshot_nightly.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-27 11:31:38.000000 torchsnapshot_nightly-2024.5.27/torchsnapshot_nightly.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)      255 2024-05-27 11:31:38.000000 torchsnapshot_nightly-2024.5.27/torchsnapshot_nightly.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       14 2024-05-27 11:31:38.000000 torchsnapshot_nightly-2024.5.27/torchsnapshot_nightly.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-27 11:31:38.000000 torchsnapshot_nightly-2024.5.27/torchsnapshot_nightly.egg-info/zip-safe
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-28 11:30:48.495142 torchsnapshot_nightly-2024.5.28/
+-rw-r--r--   0 runner    (1001) docker     (127)     1538 2024-05-28 11:29:46.000000 torchsnapshot_nightly-2024.5.28/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)     5018 2024-05-28 11:30:48.495142 torchsnapshot_nightly-2024.5.28/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     3451 2024-05-28 11:29:46.000000 torchsnapshot_nightly-2024.5.28/README.md
+-rw-r--r--   0 runner    (1001) docker     (127)       44 2024-05-28 11:29:46.000000 torchsnapshot_nightly-2024.5.28/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-28 11:30:48.495142 torchsnapshot_nightly-2024.5.28/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)     3175 2024-05-28 11:29:46.000000 torchsnapshot_nightly-2024.5.28/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-28 11:30:48.483142 torchsnapshot_nightly-2024.5.28/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)     4411 2024-05-28 11:29:46.000000 torchsnapshot_nightly-2024.5.28/tests/test_async_take.py
+-rw-r--r--   0 runner    (1001) docker     (127)    13778 2024-05-28 11:29:46.000000 torchsnapshot_nightly-2024.5.28/tests/test_batcher.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11630 2024-05-28 11:29:46.000000 torchsnapshot_nightly-2024.5.28/tests/test_chunked_tensor_io_preparer.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6789 2024-05-28 11:29:46.000000 torchsnapshot_nightly-2024.5.28/tests/test_ddp.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4133 2024-05-28 11:29:46.000000 torchsnapshot_nightly-2024.5.28/tests/test_ddp_infer_replication.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1734 2024-05-28 11:29:46.000000 torchsnapshot_nightly-2024.5.28/tests/test_ddp_replication_glob.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6849 2024-05-28 11:29:46.000000 torchsnapshot_nightly-2024.5.28/tests/test_dist_store.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7005 2024-05-28 11:29:46.000000 torchsnapshot_nightly-2024.5.28/tests/test_flatten.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2130 2024-05-28 11:29:46.000000 torchsnapshot_nightly-2024.5.28/tests/test_fs_storage_plugin.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4162 2024-05-28 11:29:46.000000 torchsnapshot_nightly-2024.5.28/tests/test_gcs_storage_plugin.py
+-rw-r--r--   0 runner    (1001) docker     (127)    27126 2024-05-28 11:29:46.000000 torchsnapshot_nightly-2024.5.28/tests/test_manifest.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1812 2024-05-28 11:29:46.000000 torchsnapshot_nightly-2024.5.28/tests/test_memoryview_stream.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8806 2024-05-28 11:29:46.000000 torchsnapshot_nightly-2024.5.28/tests/test_partitioner.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1838 2024-05-28 11:29:46.000000 torchsnapshot_nightly-2024.5.28/tests/test_pg_wrapper.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5779 2024-05-28 11:29:46.000000 torchsnapshot_nightly-2024.5.28/tests/test_read_object.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3355 2024-05-28 11:29:46.000000 torchsnapshot_nightly-2024.5.28/tests/test_replication_glob.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1101 2024-05-28 11:29:46.000000 torchsnapshot_nightly-2024.5.28/tests/test_rng_state.py
+-rw-r--r--   0 runner    (1001) docker     (127)      574 2024-05-28 11:29:46.000000 torchsnapshot_nightly-2024.5.28/tests/test_rss_profiler.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3356 2024-05-28 11:29:46.000000 torchsnapshot_nightly-2024.5.28/tests/test_s3_storage_plugin.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4036 2024-05-28 11:29:46.000000 torchsnapshot_nightly-2024.5.28/tests/test_serialization.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10067 2024-05-28 11:29:46.000000 torchsnapshot_nightly-2024.5.28/tests/test_sharded_tensor_io_preparer.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3470 2024-05-28 11:29:46.000000 torchsnapshot_nightly-2024.5.28/tests/test_sharded_tensor_resharding.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7905 2024-05-28 11:29:46.000000 torchsnapshot_nightly-2024.5.28/tests/test_snapshot.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2391 2024-05-28 11:29:46.000000 torchsnapshot_nightly-2024.5.28/tests/test_state_dict.py
+-rw-r--r--   0 runner    (1001) docker     (127)    13669 2024-05-28 11:29:46.000000 torchsnapshot_nightly-2024.5.28/tests/test_tensor_io_preparer.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5075 2024-05-28 11:29:46.000000 torchsnapshot_nightly-2024.5.28/tests/test_test_utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)      978 2024-05-28 11:29:46.000000 torchsnapshot_nightly-2024.5.28/tests/test_uvm_tensor.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-28 11:30:48.491142 torchsnapshot_nightly-2024.5.28/torchsnapshot/
+-rw-r--r--   0 runner    (1001) docker     (127)     1153 2024-05-28 11:29:46.000000 torchsnapshot_nightly-2024.5.28/torchsnapshot/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    17905 2024-05-28 11:29:46.000000 torchsnapshot_nightly-2024.5.28/torchsnapshot/batcher.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6158 2024-05-28 11:29:46.000000 torchsnapshot_nightly-2024.5.28/torchsnapshot/dist_store.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2322 2024-05-28 11:29:46.000000 torchsnapshot_nightly-2024.5.28/torchsnapshot/dtensor_utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)      729 2024-05-28 11:29:46.000000 torchsnapshot_nightly-2024.5.28/torchsnapshot/event.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1520 2024-05-28 11:29:46.000000 torchsnapshot_nightly-2024.5.28/torchsnapshot/event_handlers.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7696 2024-05-28 11:29:46.000000 torchsnapshot_nightly-2024.5.28/torchsnapshot/flatten.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6346 2024-05-28 11:29:46.000000 torchsnapshot_nightly-2024.5.28/torchsnapshot/io_preparer.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-28 11:30:48.491142 torchsnapshot_nightly-2024.5.28/torchsnapshot/io_preparers/
+-rw-r--r--   0 runner    (1001) docker     (127)      223 2024-05-28 11:29:46.000000 torchsnapshot_nightly-2024.5.28/torchsnapshot/io_preparers/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4354 2024-05-28 11:29:46.000000 torchsnapshot_nightly-2024.5.28/torchsnapshot/io_preparers/chunked_tensor.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10746 2024-05-28 11:29:46.000000 torchsnapshot_nightly-2024.5.28/torchsnapshot/io_preparers/dtensor.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2677 2024-05-28 11:29:46.000000 torchsnapshot_nightly-2024.5.28/torchsnapshot/io_preparers/object.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12707 2024-05-28 11:29:46.000000 torchsnapshot_nightly-2024.5.28/torchsnapshot/io_preparers/sharded_tensor.py
+-rw-r--r--   0 runner    (1001) docker     (127)    15281 2024-05-28 11:29:46.000000 torchsnapshot_nightly-2024.5.28/torchsnapshot/io_preparers/tensor.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2679 2024-05-28 11:29:46.000000 torchsnapshot_nightly-2024.5.28/torchsnapshot/io_types.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4210 2024-05-28 11:29:46.000000 torchsnapshot_nightly-2024.5.28/torchsnapshot/knobs.py
+-rw-r--r--   0 runner    (1001) docker     (127)    15513 2024-05-28 11:29:46.000000 torchsnapshot_nightly-2024.5.28/torchsnapshot/manifest.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10432 2024-05-28 11:29:46.000000 torchsnapshot_nightly-2024.5.28/torchsnapshot/manifest_ops.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3247 2024-05-28 11:29:46.000000 torchsnapshot_nightly-2024.5.28/torchsnapshot/manifest_utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2554 2024-05-28 11:29:46.000000 torchsnapshot_nightly-2024.5.28/torchsnapshot/memoryview_stream.py
+-rw-r--r--   0 runner    (1001) docker     (127)    13859 2024-05-28 11:29:46.000000 torchsnapshot_nightly-2024.5.28/torchsnapshot/partitioner.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2917 2024-05-28 11:29:46.000000 torchsnapshot_nightly-2024.5.28/torchsnapshot/pg_wrapper.py
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-28 11:29:46.000000 torchsnapshot_nightly-2024.5.28/torchsnapshot/py.typed
+-rw-r--r--   0 runner    (1001) docker     (127)     1344 2024-05-28 11:29:46.000000 torchsnapshot_nightly-2024.5.28/torchsnapshot/rng_state.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1581 2024-05-28 11:29:46.000000 torchsnapshot_nightly-2024.5.28/torchsnapshot/rss_profiler.py
+-rw-r--r--   0 runner    (1001) docker     (127)    16831 2024-05-28 11:29:46.000000 torchsnapshot_nightly-2024.5.28/torchsnapshot/scheduler.py
+-rw-r--r--   0 runner    (1001) docker     (127)    15262 2024-05-28 11:29:46.000000 torchsnapshot_nightly-2024.5.28/torchsnapshot/serialization.py
+-rw-r--r--   0 runner    (1001) docker     (127)    40127 2024-05-28 11:29:46.000000 torchsnapshot_nightly-2024.5.28/torchsnapshot/snapshot.py
+-rw-r--r--   0 runner    (1001) docker     (127)      874 2024-05-28 11:29:46.000000 torchsnapshot_nightly-2024.5.28/torchsnapshot/state_dict.py
+-rw-r--r--   0 runner    (1001) docker     (127)      570 2024-05-28 11:29:46.000000 torchsnapshot_nightly-2024.5.28/torchsnapshot/stateful.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2675 2024-05-28 11:29:46.000000 torchsnapshot_nightly-2024.5.28/torchsnapshot/storage_plugin.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-28 11:30:48.491142 torchsnapshot_nightly-2024.5.28/torchsnapshot/storage_plugins/
+-rw-r--r--   0 runner    (1001) docker     (127)      223 2024-05-28 11:29:46.000000 torchsnapshot_nightly-2024.5.28/torchsnapshot/storage_plugins/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1915 2024-05-28 11:29:46.000000 torchsnapshot_nightly-2024.5.28/torchsnapshot/storage_plugins/fs.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9807 2024-05-28 11:29:46.000000 torchsnapshot_nightly-2024.5.28/torchsnapshot/storage_plugins/gcs.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3001 2024-05-28 11:29:46.000000 torchsnapshot_nightly-2024.5.28/torchsnapshot/storage_plugins/s3.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9949 2024-05-28 11:29:46.000000 torchsnapshot_nightly-2024.5.28/torchsnapshot/test_utils.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-28 11:30:48.491142 torchsnapshot_nightly-2024.5.28/torchsnapshot/tricks/
+-rw-r--r--   0 runner    (1001) docker     (127)      208 2024-05-28 11:29:46.000000 torchsnapshot_nightly-2024.5.28/torchsnapshot/tricks/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1419 2024-05-28 11:29:46.000000 torchsnapshot_nightly-2024.5.28/torchsnapshot/tricks/ddp.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3405 2024-05-28 11:29:46.000000 torchsnapshot_nightly-2024.5.28/torchsnapshot/tricks/deepspeed.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1821 2024-05-28 11:29:46.000000 torchsnapshot_nightly-2024.5.28/torchsnapshot/tricks/fsdp.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1019 2024-05-28 11:29:46.000000 torchsnapshot_nightly-2024.5.28/torchsnapshot/uvm_tensor.py
+-rw-r--r--   0 runner    (1001) docker     (127)      539 2024-05-28 11:29:46.000000 torchsnapshot_nightly-2024.5.28/torchsnapshot/version.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-28 11:30:48.491142 torchsnapshot_nightly-2024.5.28/torchsnapshot_nightly.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     5018 2024-05-28 11:30:48.000000 torchsnapshot_nightly-2024.5.28/torchsnapshot_nightly.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     2375 2024-05-28 11:30:48.000000 torchsnapshot_nightly-2024.5.28/torchsnapshot_nightly.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-28 11:30:48.000000 torchsnapshot_nightly-2024.5.28/torchsnapshot_nightly.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      255 2024-05-28 11:30:48.000000 torchsnapshot_nightly-2024.5.28/torchsnapshot_nightly.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       14 2024-05-28 11:30:48.000000 torchsnapshot_nightly-2024.5.28/torchsnapshot_nightly.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-28 11:30:48.000000 torchsnapshot_nightly-2024.5.28/torchsnapshot_nightly.egg-info/zip-safe
```

### Comparing `torchsnapshot_nightly-2024.5.27/LICENSE` & `torchsnapshot_nightly-2024.5.28/LICENSE`

 * *Files identical despite different names*

### Comparing `torchsnapshot_nightly-2024.5.27/PKG-INFO` & `torchsnapshot_nightly-2024.5.28/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: torchsnapshot-nightly
-Version: 2024.5.27
+Version: 2024.5.28
 Summary: A performant, memory-efficient checkpointing library for PyTorch applications, designed with large, complex distributed workloads in mind.
 Home-page: https://github.com/pytorch/torchsnapshot
 Author: torchsnapshot team
 Author-email: yifu@fb.com
 License: BSD-3
 Keywords: pytorch,snapshot,checkpoint
 Classifier: Development Status :: 2 - Pre-Alpha
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: torchsnapshot-nightly Version: 2024.5.27 Summary: A
+Metadata-Version: 2.1 Name: torchsnapshot-nightly Version: 2024.5.28 Summary: A
 performant, memory-efficient checkpointing library for PyTorch applications,
 designed with large, complex distributed workloads in mind. Home-page: https://
 github.com/pytorch/torchsnapshot Author: torchsnapshot team Author-email:
 yifu@fb.com License: BSD-3 Keywords: pytorch,snapshot,checkpoint Classifier:
 Development Status :: 2 - Pre-Alpha Classifier: Intended Audience :: Developers
 Classifier: Intended Audience :: Science/Research Classifier: License :: OSI
 Approved :: BSD License Classifier: Programming Language :: Python :: 3
```

### Comparing `torchsnapshot_nightly-2024.5.27/README.md` & `torchsnapshot_nightly-2024.5.28/README.md`

 * *Files identical despite different names*

### Comparing `torchsnapshot_nightly-2024.5.27/setup.py` & `torchsnapshot_nightly-2024.5.28/setup.py`

 * *Files identical despite different names*

### Comparing `torchsnapshot_nightly-2024.5.27/tests/test_async_take.py` & `torchsnapshot_nightly-2024.5.28/tests/test_async_take.py`

 * *Files identical despite different names*

### Comparing `torchsnapshot_nightly-2024.5.27/tests/test_batcher.py` & `torchsnapshot_nightly-2024.5.28/tests/test_batcher.py`

 * *Files identical despite different names*

### Comparing `torchsnapshot_nightly-2024.5.27/tests/test_chunked_tensor_io_preparer.py` & `torchsnapshot_nightly-2024.5.28/tests/test_chunked_tensor_io_preparer.py`

 * *Files identical despite different names*

### Comparing `torchsnapshot_nightly-2024.5.27/tests/test_ddp.py` & `torchsnapshot_nightly-2024.5.28/tests/test_ddp.py`

 * *Files identical despite different names*

### Comparing `torchsnapshot_nightly-2024.5.27/tests/test_ddp_infer_replication.py` & `torchsnapshot_nightly-2024.5.28/tests/test_ddp_infer_replication.py`

 * *Files identical despite different names*

### Comparing `torchsnapshot_nightly-2024.5.27/tests/test_ddp_replication_glob.py` & `torchsnapshot_nightly-2024.5.28/tests/test_ddp_replication_glob.py`

 * *Files identical despite different names*

### Comparing `torchsnapshot_nightly-2024.5.27/tests/test_dist_store.py` & `torchsnapshot_nightly-2024.5.28/tests/test_dist_store.py`

 * *Files identical despite different names*

### Comparing `torchsnapshot_nightly-2024.5.27/tests/test_flatten.py` & `torchsnapshot_nightly-2024.5.28/tests/test_flatten.py`

 * *Files identical despite different names*

### Comparing `torchsnapshot_nightly-2024.5.27/tests/test_fs_storage_plugin.py` & `torchsnapshot_nightly-2024.5.28/tests/test_fs_storage_plugin.py`

 * *Files identical despite different names*

### Comparing `torchsnapshot_nightly-2024.5.27/tests/test_gcs_storage_plugin.py` & `torchsnapshot_nightly-2024.5.28/tests/test_gcs_storage_plugin.py`

 * *Files identical despite different names*

### Comparing `torchsnapshot_nightly-2024.5.27/tests/test_manifest.py` & `torchsnapshot_nightly-2024.5.28/tests/test_manifest.py`

 * *Files identical despite different names*

### Comparing `torchsnapshot_nightly-2024.5.27/tests/test_memoryview_stream.py` & `torchsnapshot_nightly-2024.5.28/tests/test_memoryview_stream.py`

 * *Files identical despite different names*

### Comparing `torchsnapshot_nightly-2024.5.27/tests/test_partitioner.py` & `torchsnapshot_nightly-2024.5.28/tests/test_partitioner.py`

 * *Files identical despite different names*

### Comparing `torchsnapshot_nightly-2024.5.27/tests/test_pg_wrapper.py` & `torchsnapshot_nightly-2024.5.28/tests/test_pg_wrapper.py`

 * *Files identical despite different names*

### Comparing `torchsnapshot_nightly-2024.5.27/tests/test_read_object.py` & `torchsnapshot_nightly-2024.5.28/tests/test_read_object.py`

 * *Files identical despite different names*

### Comparing `torchsnapshot_nightly-2024.5.27/tests/test_replication_glob.py` & `torchsnapshot_nightly-2024.5.28/tests/test_replication_glob.py`

 * *Files identical despite different names*

### Comparing `torchsnapshot_nightly-2024.5.27/tests/test_rng_state.py` & `torchsnapshot_nightly-2024.5.28/tests/test_rng_state.py`

 * *Files identical despite different names*

### Comparing `torchsnapshot_nightly-2024.5.27/tests/test_rss_profiler.py` & `torchsnapshot_nightly-2024.5.28/tests/test_rss_profiler.py`

 * *Files identical despite different names*

### Comparing `torchsnapshot_nightly-2024.5.27/tests/test_s3_storage_plugin.py` & `torchsnapshot_nightly-2024.5.28/tests/test_s3_storage_plugin.py`

 * *Files identical despite different names*

### Comparing `torchsnapshot_nightly-2024.5.27/tests/test_serialization.py` & `torchsnapshot_nightly-2024.5.28/tests/test_serialization.py`

 * *Files identical despite different names*

### Comparing `torchsnapshot_nightly-2024.5.27/tests/test_sharded_tensor_io_preparer.py` & `torchsnapshot_nightly-2024.5.28/tests/test_sharded_tensor_io_preparer.py`

 * *Files identical despite different names*

### Comparing `torchsnapshot_nightly-2024.5.27/tests/test_sharded_tensor_resharding.py` & `torchsnapshot_nightly-2024.5.28/tests/test_sharded_tensor_resharding.py`

 * *Files identical despite different names*

### Comparing `torchsnapshot_nightly-2024.5.27/tests/test_snapshot.py` & `torchsnapshot_nightly-2024.5.28/tests/test_snapshot.py`

 * *Files identical despite different names*

### Comparing `torchsnapshot_nightly-2024.5.27/tests/test_state_dict.py` & `torchsnapshot_nightly-2024.5.28/tests/test_state_dict.py`

 * *Files identical despite different names*

### Comparing `torchsnapshot_nightly-2024.5.27/tests/test_tensor_io_preparer.py` & `torchsnapshot_nightly-2024.5.28/tests/test_tensor_io_preparer.py`

 * *Files identical despite different names*

### Comparing `torchsnapshot_nightly-2024.5.27/tests/test_test_utils.py` & `torchsnapshot_nightly-2024.5.28/tests/test_test_utils.py`

 * *Files identical despite different names*

### Comparing `torchsnapshot_nightly-2024.5.27/tests/test_uvm_tensor.py` & `torchsnapshot_nightly-2024.5.28/tests/test_uvm_tensor.py`

 * *Files identical despite different names*

### Comparing `torchsnapshot_nightly-2024.5.27/torchsnapshot/__init__.py` & `torchsnapshot_nightly-2024.5.28/torchsnapshot/__init__.py`

 * *Files identical despite different names*

### Comparing `torchsnapshot_nightly-2024.5.27/torchsnapshot/batcher.py` & `torchsnapshot_nightly-2024.5.28/torchsnapshot/batcher.py`

 * *Files identical despite different names*

### Comparing `torchsnapshot_nightly-2024.5.27/torchsnapshot/dist_store.py` & `torchsnapshot_nightly-2024.5.28/torchsnapshot/dist_store.py`

 * *Files identical despite different names*

### Comparing `torchsnapshot_nightly-2024.5.27/torchsnapshot/dtensor_utils.py` & `torchsnapshot_nightly-2024.5.28/torchsnapshot/dtensor_utils.py`

 * *Files identical despite different names*

### Comparing `torchsnapshot_nightly-2024.5.27/torchsnapshot/event.py` & `torchsnapshot_nightly-2024.5.28/torchsnapshot/event.py`

 * *Files identical despite different names*

### Comparing `torchsnapshot_nightly-2024.5.27/torchsnapshot/event_handlers.py` & `torchsnapshot_nightly-2024.5.28/torchsnapshot/event_handlers.py`

 * *Files identical despite different names*

### Comparing `torchsnapshot_nightly-2024.5.27/torchsnapshot/flatten.py` & `torchsnapshot_nightly-2024.5.28/torchsnapshot/flatten.py`

 * *Files identical despite different names*

### Comparing `torchsnapshot_nightly-2024.5.27/torchsnapshot/io_preparer.py` & `torchsnapshot_nightly-2024.5.28/torchsnapshot/io_preparer.py`

 * *Files identical despite different names*

### Comparing `torchsnapshot_nightly-2024.5.27/torchsnapshot/io_preparers/chunked_tensor.py` & `torchsnapshot_nightly-2024.5.28/torchsnapshot/io_preparers/chunked_tensor.py`

 * *Files identical despite different names*

### Comparing `torchsnapshot_nightly-2024.5.27/torchsnapshot/io_preparers/dtensor.py` & `torchsnapshot_nightly-2024.5.28/torchsnapshot/io_preparers/dtensor.py`

 * *Files identical despite different names*

### Comparing `torchsnapshot_nightly-2024.5.27/torchsnapshot/io_preparers/object.py` & `torchsnapshot_nightly-2024.5.28/torchsnapshot/io_preparers/object.py`

 * *Files identical despite different names*

### Comparing `torchsnapshot_nightly-2024.5.27/torchsnapshot/io_preparers/sharded_tensor.py` & `torchsnapshot_nightly-2024.5.28/torchsnapshot/io_preparers/sharded_tensor.py`

 * *Files identical despite different names*

### Comparing `torchsnapshot_nightly-2024.5.27/torchsnapshot/io_preparers/tensor.py` & `torchsnapshot_nightly-2024.5.28/torchsnapshot/io_preparers/tensor.py`

 * *Files identical despite different names*

### Comparing `torchsnapshot_nightly-2024.5.27/torchsnapshot/io_types.py` & `torchsnapshot_nightly-2024.5.28/torchsnapshot/io_types.py`

 * *Files identical despite different names*

### Comparing `torchsnapshot_nightly-2024.5.27/torchsnapshot/knobs.py` & `torchsnapshot_nightly-2024.5.28/torchsnapshot/knobs.py`

 * *Files identical despite different names*

### Comparing `torchsnapshot_nightly-2024.5.27/torchsnapshot/manifest.py` & `torchsnapshot_nightly-2024.5.28/torchsnapshot/manifest.py`

 * *Files identical despite different names*

### Comparing `torchsnapshot_nightly-2024.5.27/torchsnapshot/manifest_ops.py` & `torchsnapshot_nightly-2024.5.28/torchsnapshot/manifest_ops.py`

 * *Files identical despite different names*

### Comparing `torchsnapshot_nightly-2024.5.27/torchsnapshot/manifest_utils.py` & `torchsnapshot_nightly-2024.5.28/torchsnapshot/manifest_utils.py`

 * *Files identical despite different names*

### Comparing `torchsnapshot_nightly-2024.5.27/torchsnapshot/memoryview_stream.py` & `torchsnapshot_nightly-2024.5.28/torchsnapshot/memoryview_stream.py`

 * *Files identical despite different names*

### Comparing `torchsnapshot_nightly-2024.5.27/torchsnapshot/partitioner.py` & `torchsnapshot_nightly-2024.5.28/torchsnapshot/partitioner.py`

 * *Files identical despite different names*

### Comparing `torchsnapshot_nightly-2024.5.27/torchsnapshot/pg_wrapper.py` & `torchsnapshot_nightly-2024.5.28/torchsnapshot/pg_wrapper.py`

 * *Files identical despite different names*

### Comparing `torchsnapshot_nightly-2024.5.27/torchsnapshot/rng_state.py` & `torchsnapshot_nightly-2024.5.28/torchsnapshot/rng_state.py`

 * *Files identical despite different names*

### Comparing `torchsnapshot_nightly-2024.5.27/torchsnapshot/rss_profiler.py` & `torchsnapshot_nightly-2024.5.28/torchsnapshot/rss_profiler.py`

 * *Files identical despite different names*

### Comparing `torchsnapshot_nightly-2024.5.27/torchsnapshot/scheduler.py` & `torchsnapshot_nightly-2024.5.28/torchsnapshot/scheduler.py`

 * *Files identical despite different names*

### Comparing `torchsnapshot_nightly-2024.5.27/torchsnapshot/serialization.py` & `torchsnapshot_nightly-2024.5.28/torchsnapshot/serialization.py`

 * *Files identical despite different names*

### Comparing `torchsnapshot_nightly-2024.5.27/torchsnapshot/snapshot.py` & `torchsnapshot_nightly-2024.5.28/torchsnapshot/snapshot.py`

 * *Files identical despite different names*

### Comparing `torchsnapshot_nightly-2024.5.27/torchsnapshot/state_dict.py` & `torchsnapshot_nightly-2024.5.28/torchsnapshot/state_dict.py`

 * *Files identical despite different names*

### Comparing `torchsnapshot_nightly-2024.5.27/torchsnapshot/stateful.py` & `torchsnapshot_nightly-2024.5.28/torchsnapshot/stateful.py`

 * *Files identical despite different names*

### Comparing `torchsnapshot_nightly-2024.5.27/torchsnapshot/storage_plugin.py` & `torchsnapshot_nightly-2024.5.28/torchsnapshot/storage_plugin.py`

 * *Files identical despite different names*

### Comparing `torchsnapshot_nightly-2024.5.27/torchsnapshot/storage_plugins/fs.py` & `torchsnapshot_nightly-2024.5.28/torchsnapshot/storage_plugins/fs.py`

 * *Files identical despite different names*

### Comparing `torchsnapshot_nightly-2024.5.27/torchsnapshot/storage_plugins/gcs.py` & `torchsnapshot_nightly-2024.5.28/torchsnapshot/storage_plugins/gcs.py`

 * *Files identical despite different names*

### Comparing `torchsnapshot_nightly-2024.5.27/torchsnapshot/storage_plugins/s3.py` & `torchsnapshot_nightly-2024.5.28/torchsnapshot/storage_plugins/s3.py`

 * *Files identical despite different names*

### Comparing `torchsnapshot_nightly-2024.5.27/torchsnapshot/test_utils.py` & `torchsnapshot_nightly-2024.5.28/torchsnapshot/test_utils.py`

 * *Files identical despite different names*

### Comparing `torchsnapshot_nightly-2024.5.27/torchsnapshot/tricks/ddp.py` & `torchsnapshot_nightly-2024.5.28/torchsnapshot/tricks/ddp.py`

 * *Files identical despite different names*

### Comparing `torchsnapshot_nightly-2024.5.27/torchsnapshot/tricks/deepspeed.py` & `torchsnapshot_nightly-2024.5.28/torchsnapshot/tricks/deepspeed.py`

 * *Files identical despite different names*

### Comparing `torchsnapshot_nightly-2024.5.27/torchsnapshot/tricks/fsdp.py` & `torchsnapshot_nightly-2024.5.28/torchsnapshot/tricks/fsdp.py`

 * *Files identical despite different names*

### Comparing `torchsnapshot_nightly-2024.5.27/torchsnapshot/uvm_tensor.py` & `torchsnapshot_nightly-2024.5.28/torchsnapshot/uvm_tensor.py`

 * *Files identical despite different names*

### Comparing `torchsnapshot_nightly-2024.5.27/torchsnapshot/version.py` & `torchsnapshot_nightly-2024.5.28/torchsnapshot/version.py`

 * *Files identical despite different names*

### Comparing `torchsnapshot_nightly-2024.5.27/torchsnapshot_nightly.egg-info/PKG-INFO` & `torchsnapshot_nightly-2024.5.28/torchsnapshot_nightly.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: torchsnapshot-nightly
-Version: 2024.5.27
+Version: 2024.5.28
 Summary: A performant, memory-efficient checkpointing library for PyTorch applications, designed with large, complex distributed workloads in mind.
 Home-page: https://github.com/pytorch/torchsnapshot
 Author: torchsnapshot team
 Author-email: yifu@fb.com
 License: BSD-3
 Keywords: pytorch,snapshot,checkpoint
 Classifier: Development Status :: 2 - Pre-Alpha
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: torchsnapshot-nightly Version: 2024.5.27 Summary: A
+Metadata-Version: 2.1 Name: torchsnapshot-nightly Version: 2024.5.28 Summary: A
 performant, memory-efficient checkpointing library for PyTorch applications,
 designed with large, complex distributed workloads in mind. Home-page: https://
 github.com/pytorch/torchsnapshot Author: torchsnapshot team Author-email:
 yifu@fb.com License: BSD-3 Keywords: pytorch,snapshot,checkpoint Classifier:
 Development Status :: 2 - Pre-Alpha Classifier: Intended Audience :: Developers
 Classifier: Intended Audience :: Science/Research Classifier: License :: OSI
 Approved :: BSD License Classifier: Programming Language :: Python :: 3
```

### Comparing `torchsnapshot_nightly-2024.5.27/torchsnapshot_nightly.egg-info/SOURCES.txt` & `torchsnapshot_nightly-2024.5.28/torchsnapshot_nightly.egg-info/SOURCES.txt`

 * *Files identical despite different names*

