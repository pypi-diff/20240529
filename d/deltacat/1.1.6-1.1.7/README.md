# Comparing `tmp/deltacat-1.1.6.tar.gz` & `tmp/deltacat-1.1.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/deltacat-1.1.6.tar", last modified: Thu May 16 01:13:08 2024, max compression
+gzip compressed data, was "dist/deltacat-1.1.7.tar", last modified: Wed May 29 02:00:56 2024, max compression
```

## Comparing `deltacat-1.1.6.tar` & `deltacat-1.1.7.tar`

### file list

```diff
@@ -1,271 +1,275 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-16 01:13:08.000000 deltacat-1.1.6/
--rw-r--r--   0 runner    (1001) docker     (127)       25 2024-05-16 01:00:15.000000 deltacat-1.1.6/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (127)     1569 2024-05-16 01:13:08.000000 deltacat-1.1.6/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      686 2024-05-16 01:00:15.000000 deltacat-1.1.6/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-16 01:13:08.000000 deltacat-1.1.6/deltacat/
--rw-r--r--   0 runner    (1001) docker     (127)     1777 2024-05-16 01:00:15.000000 deltacat-1.1.6/deltacat/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-16 01:13:08.000000 deltacat-1.1.6/deltacat/aws/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-16 01:00:15.000000 deltacat-1.1.6/deltacat/aws/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     6948 2024-05-16 01:00:15.000000 deltacat-1.1.6/deltacat/aws/clients.py
--rw-r--r--   0 runner    (1001) docker     (127)      501 2024-05-16 01:00:15.000000 deltacat-1.1.6/deltacat/aws/constants.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-16 01:13:08.000000 deltacat-1.1.6/deltacat/aws/redshift/
--rw-r--r--   0 runner    (1001) docker     (127)      342 2024-05-16 01:00:15.000000 deltacat-1.1.6/deltacat/aws/redshift/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-16 01:13:08.000000 deltacat-1.1.6/deltacat/aws/redshift/model/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-16 01:00:15.000000 deltacat-1.1.6/deltacat/aws/redshift/model/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    12987 2024-05-16 01:00:15.000000 deltacat-1.1.6/deltacat/aws/redshift/model/manifest.py
--rw-r--r--   0 runner    (1001) docker     (127)    26525 2024-05-16 01:00:15.000000 deltacat-1.1.6/deltacat/aws/s3u.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-16 01:13:08.000000 deltacat-1.1.6/deltacat/benchmarking/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-16 01:00:15.000000 deltacat-1.1.6/deltacat/benchmarking/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1709 2024-05-16 01:00:15.000000 deltacat-1.1.6/deltacat/benchmarking/benchmark_parquet_reads.py
--rw-r--r--   0 runner    (1001) docker     (127)     1604 2024-05-16 01:00:15.000000 deltacat-1.1.6/deltacat/benchmarking/conftest.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-16 01:13:08.000000 deltacat-1.1.6/deltacat/catalog/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-16 01:00:15.000000 deltacat-1.1.6/deltacat/catalog/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-16 01:13:08.000000 deltacat-1.1.6/deltacat/catalog/default_catalog_impl/
--rw-r--r--   0 runner    (1001) docker     (127)    12677 2024-05-16 01:00:15.000000 deltacat-1.1.6/deltacat/catalog/default_catalog_impl/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     8745 2024-05-16 01:00:15.000000 deltacat-1.1.6/deltacat/catalog/delegate.py
--rw-r--r--   0 runner    (1001) docker     (127)     6556 2024-05-16 01:00:15.000000 deltacat-1.1.6/deltacat/catalog/interface.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-16 01:13:08.000000 deltacat-1.1.6/deltacat/catalog/model/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-16 01:00:15.000000 deltacat-1.1.6/deltacat/catalog/model/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2212 2024-05-16 01:00:15.000000 deltacat-1.1.6/deltacat/catalog/model/catalog.py
--rw-r--r--   0 runner    (1001) docker     (127)      727 2024-05-16 01:00:15.000000 deltacat-1.1.6/deltacat/catalog/model/table_definition.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-16 01:13:08.000000 deltacat-1.1.6/deltacat/compute/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-16 01:00:15.000000 deltacat-1.1.6/deltacat/compute/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-16 01:13:08.000000 deltacat-1.1.6/deltacat/compute/compactor/
--rw-r--r--   0 runner    (1001) docker     (127)     1022 2024-05-16 01:00:15.000000 deltacat-1.1.6/deltacat/compute/compactor/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    27612 2024-05-16 01:00:15.000000 deltacat-1.1.6/deltacat/compute/compactor/compaction_session.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-16 01:13:08.000000 deltacat-1.1.6/deltacat/compute/compactor/model/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-16 01:00:15.000000 deltacat-1.1.6/deltacat/compute/compactor/model/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    15195 2024-05-16 01:00:15.000000 deltacat-1.1.6/deltacat/compute/compactor/model/compact_partition_params.py
--rw-r--r--   0 runner    (1001) docker     (127)    30547 2024-05-16 01:00:15.000000 deltacat-1.1.6/deltacat/compute/compactor/model/compaction_session_audit_info.py
--rw-r--r--   0 runner    (1001) docker     (127)       87 2024-05-16 01:00:15.000000 deltacat-1.1.6/deltacat/compute/compactor/model/compactor_version.py
--rw-r--r--   0 runner    (1001) docker     (127)      292 2024-05-16 01:00:15.000000 deltacat-1.1.6/deltacat/compute/compactor/model/dedupe_result.py
--rw-r--r--   0 runner    (1001) docker     (127)    12258 2024-05-16 01:00:15.000000 deltacat-1.1.6/deltacat/compute/compactor/model/delta_annotated.py
--rw-r--r--   0 runner    (1001) docker     (127)     3676 2024-05-16 01:00:15.000000 deltacat-1.1.6/deltacat/compute/compactor/model/delta_file_envelope.py
--rw-r--r--   0 runner    (1001) docker     (127)     1905 2024-05-16 01:00:15.000000 deltacat-1.1.6/deltacat/compute/compactor/model/delta_file_locator.py
--rw-r--r--   0 runner    (1001) docker     (127)      275 2024-05-16 01:00:15.000000 deltacat-1.1.6/deltacat/compute/compactor/model/hash_bucket_result.py
--rw-r--r--   0 runner    (1001) docker     (127)     2656 2024-05-16 01:00:15.000000 deltacat-1.1.6/deltacat/compute/compactor/model/materialize_result.py
--rw-r--r--   0 runner    (1001) docker     (127)    10449 2024-05-16 01:00:15.000000 deltacat-1.1.6/deltacat/compute/compactor/model/primary_key_index.py
--rw-r--r--   0 runner    (1001) docker     (127)     1324 2024-05-16 01:00:15.000000 deltacat-1.1.6/deltacat/compute/compactor/model/pyarrow_write_result.py
--rw-r--r--   0 runner    (1001) docker     (127)      140 2024-05-16 01:00:15.000000 deltacat-1.1.6/deltacat/compute/compactor/model/repartition_result.py
--rw-r--r--   0 runner    (1001) docker     (127)     4940 2024-05-16 01:00:15.000000 deltacat-1.1.6/deltacat/compute/compactor/model/round_completion_info.py
--rw-r--r--   0 runner    (1001) docker     (127)     1487 2024-05-16 01:00:15.000000 deltacat-1.1.6/deltacat/compute/compactor/model/table_object_store.py
--rw-r--r--   0 runner    (1001) docker     (127)     7240 2024-05-16 01:00:15.000000 deltacat-1.1.6/deltacat/compute/compactor/repartition_session.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-16 01:13:08.000000 deltacat-1.1.6/deltacat/compute/compactor/steps/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-16 01:00:15.000000 deltacat-1.1.6/deltacat/compute/compactor/steps/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    10190 2024-05-16 01:00:15.000000 deltacat-1.1.6/deltacat/compute/compactor/steps/dedupe.py
--rw-r--r--   0 runner    (1001) docker     (127)    10655 2024-05-16 01:00:15.000000 deltacat-1.1.6/deltacat/compute/compactor/steps/hash_bucket.py
--rw-r--r--   0 runner    (1001) docker     (127)    14246 2024-05-16 01:00:15.000000 deltacat-1.1.6/deltacat/compute/compactor/steps/materialize.py
--rw-r--r--   0 runner    (1001) docker     (127)    10960 2024-05-16 01:00:15.000000 deltacat-1.1.6/deltacat/compute/compactor/steps/repartition.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-16 01:13:08.000000 deltacat-1.1.6/deltacat/compute/compactor/utils/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-16 01:00:15.000000 deltacat-1.1.6/deltacat/compute/compactor/utils/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    17303 2024-05-16 01:00:15.000000 deltacat-1.1.6/deltacat/compute/compactor/utils/io.py
--rw-r--r--   0 runner    (1001) docker     (127)     2435 2024-05-16 01:00:15.000000 deltacat-1.1.6/deltacat/compute/compactor/utils/primary_key_index.py
--rw-r--r--   0 runner    (1001) docker     (127)     2345 2024-05-16 01:00:15.000000 deltacat-1.1.6/deltacat/compute/compactor/utils/round_completion_file.py
--rw-r--r--   0 runner    (1001) docker     (127)     2397 2024-05-16 01:00:15.000000 deltacat-1.1.6/deltacat/compute/compactor/utils/sort_key.py
--rw-r--r--   0 runner    (1001) docker     (127)     9399 2024-05-16 01:00:15.000000 deltacat-1.1.6/deltacat/compute/compactor/utils/system_columns.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-16 01:13:08.000000 deltacat-1.1.6/deltacat/compute/compactor_v2/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-16 01:00:15.000000 deltacat-1.1.6/deltacat/compute/compactor_v2/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    26087 2024-05-16 01:00:15.000000 deltacat-1.1.6/deltacat/compute/compactor_v2/compaction_session.py
--rw-r--r--   0 runner    (1001) docker     (127)     2118 2024-05-16 01:00:15.000000 deltacat-1.1.6/deltacat/compute/compactor_v2/constants.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-16 01:13:08.000000 deltacat-1.1.6/deltacat/compute/compactor_v2/deletes/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-16 01:00:15.000000 deltacat-1.1.6/deltacat/compute/compactor_v2/deletes/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     3111 2024-05-16 01:00:15.000000 deltacat-1.1.6/deltacat/compute/compactor_v2/deletes/delete_file_envelope.py
--rw-r--r--   0 runner    (1001) docker     (127)     2833 2024-05-16 01:00:15.000000 deltacat-1.1.6/deltacat/compute/compactor_v2/deletes/delete_strategy.py
--rw-r--r--   0 runner    (1001) docker     (127)     6503 2024-05-16 01:00:15.000000 deltacat-1.1.6/deltacat/compute/compactor_v2/deletes/delete_strategy_equality_delete.py
--rw-r--r--   0 runner    (1001) docker     (127)      558 2024-05-16 01:00:15.000000 deltacat-1.1.6/deltacat/compute/compactor_v2/deletes/model.py
--rw-r--r--   0 runner    (1001) docker     (127)     6640 2024-05-16 01:00:15.000000 deltacat-1.1.6/deltacat/compute/compactor_v2/deletes/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-16 01:13:08.000000 deltacat-1.1.6/deltacat/compute/compactor_v2/model/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-16 01:00:15.000000 deltacat-1.1.6/deltacat/compute/compactor_v2/model/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     3042 2024-05-16 01:00:15.000000 deltacat-1.1.6/deltacat/compute/compactor_v2/model/hash_bucket_input.py
--rw-r--r--   0 runner    (1001) docker     (127)      309 2024-05-16 01:00:15.000000 deltacat-1.1.6/deltacat/compute/compactor_v2/model/hash_bucket_result.py
--rw-r--r--   0 runner    (1001) docker     (127)     7410 2024-05-16 01:00:15.000000 deltacat-1.1.6/deltacat/compute/compactor_v2/model/merge_file_group.py
--rw-r--r--   0 runner    (1001) docker     (127)     5416 2024-05-16 01:00:15.000000 deltacat-1.1.6/deltacat/compute/compactor_v2/model/merge_input.py
--rw-r--r--   0 runner    (1001) docker     (127)      436 2024-05-16 01:00:15.000000 deltacat-1.1.6/deltacat/compute/compactor_v2/model/merge_result.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-16 01:13:08.000000 deltacat-1.1.6/deltacat/compute/compactor_v2/steps/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-16 01:00:15.000000 deltacat-1.1.6/deltacat/compute/compactor_v2/steps/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     6617 2024-05-16 01:00:15.000000 deltacat-1.1.6/deltacat/compute/compactor_v2/steps/hash_bucket.py
--rw-r--r--   0 runner    (1001) docker     (127)    21657 2024-05-16 01:00:15.000000 deltacat-1.1.6/deltacat/compute/compactor_v2/steps/merge.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-16 01:13:08.000000 deltacat-1.1.6/deltacat/compute/compactor_v2/utils/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-16 01:00:15.000000 deltacat-1.1.6/deltacat/compute/compactor_v2/utils/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2156 2024-05-16 01:00:15.000000 deltacat-1.1.6/deltacat/compute/compactor_v2/utils/content_type_params.py
--rw-r--r--   0 runner    (1001) docker     (127)     1932 2024-05-16 01:00:15.000000 deltacat-1.1.6/deltacat/compute/compactor_v2/utils/dedupe.py
--rw-r--r--   0 runner    (1001) docker     (127)     3635 2024-05-16 01:00:15.000000 deltacat-1.1.6/deltacat/compute/compactor_v2/utils/delta.py
--rw-r--r--   0 runner    (1001) docker     (127)     5264 2024-05-16 01:00:15.000000 deltacat-1.1.6/deltacat/compute/compactor_v2/utils/io.py
--rw-r--r--   0 runner    (1001) docker     (127)     5244 2024-05-16 01:00:15.000000 deltacat-1.1.6/deltacat/compute/compactor_v2/utils/merge.py
--rw-r--r--   0 runner    (1001) docker     (127)    11393 2024-05-16 01:00:15.000000 deltacat-1.1.6/deltacat/compute/compactor_v2/utils/primary_key_index.py
--rw-r--r--   0 runner    (1001) docker     (127)    14160 2024-05-16 01:00:15.000000 deltacat-1.1.6/deltacat/compute/compactor_v2/utils/task_options.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-16 01:13:08.000000 deltacat-1.1.6/deltacat/compute/merge_on_read/
--rw-r--r--   0 runner    (1001) docker     (127)      214 2024-05-16 01:00:15.000000 deltacat-1.1.6/deltacat/compute/merge_on_read/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1400 2024-05-16 01:00:15.000000 deltacat-1.1.6/deltacat/compute/merge_on_read/daft.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-16 01:13:08.000000 deltacat-1.1.6/deltacat/compute/merge_on_read/model/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-16 01:00:15.000000 deltacat-1.1.6/deltacat/compute/merge_on_read/model/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2035 2024-05-16 01:00:15.000000 deltacat-1.1.6/deltacat/compute/merge_on_read/model/merge_on_read_params.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-16 01:13:08.000000 deltacat-1.1.6/deltacat/compute/merge_on_read/utils/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-16 01:00:15.000000 deltacat-1.1.6/deltacat/compute/merge_on_read/utils/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1367 2024-05-16 01:00:15.000000 deltacat-1.1.6/deltacat/compute/merge_on_read/utils/delta.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-16 01:13:08.000000 deltacat-1.1.6/deltacat/compute/metastats/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-16 01:00:15.000000 deltacat-1.1.6/deltacat/compute/metastats/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-16 01:13:08.000000 deltacat-1.1.6/deltacat/compute/metastats/config/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-16 01:00:15.000000 deltacat-1.1.6/deltacat/compute/metastats/config/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    18731 2024-05-16 01:00:15.000000 deltacat-1.1.6/deltacat/compute/metastats/meta_stats.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-16 01:13:08.000000 deltacat-1.1.6/deltacat/compute/metastats/model/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-16 01:00:15.000000 deltacat-1.1.6/deltacat/compute/metastats/model/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1123 2024-05-16 01:00:15.000000 deltacat-1.1.6/deltacat/compute/metastats/model/partition_stats_dict.py
--rw-r--r--   0 runner    (1001) docker     (127)     2849 2024-05-16 01:00:15.000000 deltacat-1.1.6/deltacat/compute/metastats/model/stats_cluster_size_estimator.py
--rw-r--r--   0 runner    (1001) docker     (127)     7363 2024-05-16 01:00:15.000000 deltacat-1.1.6/deltacat/compute/metastats/stats.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-16 01:13:08.000000 deltacat-1.1.6/deltacat/compute/metastats/utils/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-16 01:00:15.000000 deltacat-1.1.6/deltacat/compute/metastats/utils/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      869 2024-05-16 01:00:15.000000 deltacat-1.1.6/deltacat/compute/metastats/utils/constants.py
--rw-r--r--   0 runner    (1001) docker     (127)     9007 2024-05-16 01:00:15.000000 deltacat-1.1.6/deltacat/compute/metastats/utils/io.py
--rw-r--r--   0 runner    (1001) docker     (127)     1143 2024-05-16 01:00:15.000000 deltacat-1.1.6/deltacat/compute/metastats/utils/pyarrow_memory_estimation_function.py
--rw-r--r--   0 runner    (1001) docker     (127)     4516 2024-05-16 01:00:15.000000 deltacat-1.1.6/deltacat/compute/metastats/utils/ray_utils.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-16 01:13:08.000000 deltacat-1.1.6/deltacat/compute/stats/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-16 01:00:15.000000 deltacat-1.1.6/deltacat/compute/stats/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     8837 2024-05-16 01:00:15.000000 deltacat-1.1.6/deltacat/compute/stats/basic.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-16 01:13:08.000000 deltacat-1.1.6/deltacat/compute/stats/models/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-16 01:00:15.000000 deltacat-1.1.6/deltacat/compute/stats/models/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     3300 2024-05-16 01:00:15.000000 deltacat-1.1.6/deltacat/compute/stats/models/delta_column_stats.py
--rw-r--r--   0 runner    (1001) docker     (127)     8556 2024-05-16 01:00:15.000000 deltacat-1.1.6/deltacat/compute/stats/models/delta_stats.py
--rw-r--r--   0 runner    (1001) docker     (127)     1624 2024-05-16 01:00:15.000000 deltacat-1.1.6/deltacat/compute/stats/models/delta_stats_cache_result.py
--rw-r--r--   0 runner    (1001) docker     (127)     2419 2024-05-16 01:00:15.000000 deltacat-1.1.6/deltacat/compute/stats/models/manifest_entry_stats.py
--rw-r--r--   0 runner    (1001) docker     (127)     3820 2024-05-16 01:00:15.000000 deltacat-1.1.6/deltacat/compute/stats/models/stats_result.py
--rw-r--r--   0 runner    (1001) docker     (127)      215 2024-05-16 01:00:15.000000 deltacat-1.1.6/deltacat/compute/stats/types.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-16 01:13:08.000000 deltacat-1.1.6/deltacat/compute/stats/utils/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-16 01:00:15.000000 deltacat-1.1.6/deltacat/compute/stats/utils/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     3094 2024-05-16 01:00:15.000000 deltacat-1.1.6/deltacat/compute/stats/utils/intervals.py
--rw-r--r--   0 runner    (1001) docker     (127)     9059 2024-05-16 01:00:15.000000 deltacat-1.1.6/deltacat/compute/stats/utils/io.py
--rw-r--r--   0 runner    (1001) docker     (127)     3693 2024-05-16 01:00:15.000000 deltacat-1.1.6/deltacat/compute/stats/utils/manifest_stats_file.py
--rw-r--r--   0 runner    (1001) docker     (127)     1939 2024-05-16 01:00:15.000000 deltacat-1.1.6/deltacat/constants.py
--rw-r--r--   0 runner    (1001) docker     (127)      199 2024-05-16 01:00:15.000000 deltacat-1.1.6/deltacat/exceptions.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-16 01:13:08.000000 deltacat-1.1.6/deltacat/io/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-16 01:00:15.000000 deltacat-1.1.6/deltacat/io/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-16 01:13:08.000000 deltacat-1.1.6/deltacat/io/aws/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-16 01:00:15.000000 deltacat-1.1.6/deltacat/io/aws/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-16 01:13:08.000000 deltacat-1.1.6/deltacat/io/aws/redshift/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-16 01:00:15.000000 deltacat-1.1.6/deltacat/io/aws/redshift/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    22599 2024-05-16 01:00:15.000000 deltacat-1.1.6/deltacat/io/aws/redshift/redshift_datasource.py
--rw-r--r--   0 runner    (1001) docker     (127)     3755 2024-05-16 01:00:15.000000 deltacat-1.1.6/deltacat/io/dataset.py
--rw-r--r--   0 runner    (1001) docker     (127)     1346 2024-05-16 01:00:15.000000 deltacat-1.1.6/deltacat/io/file_object_store.py
--rw-r--r--   0 runner    (1001) docker     (127)     9185 2024-05-16 01:00:15.000000 deltacat-1.1.6/deltacat/io/memcached_object_store.py
--rw-r--r--   0 runner    (1001) docker     (127)     1576 2024-05-16 01:00:15.000000 deltacat-1.1.6/deltacat/io/object_store.py
--rw-r--r--   0 runner    (1001) docker     (127)      905 2024-05-16 01:00:15.000000 deltacat-1.1.6/deltacat/io/ray_plasma_object_store.py
--rw-r--r--   0 runner    (1001) docker     (127)     7023 2024-05-16 01:00:15.000000 deltacat-1.1.6/deltacat/io/read_api.py
--rw-r--r--   0 runner    (1001) docker     (127)     3507 2024-05-16 01:00:15.000000 deltacat-1.1.6/deltacat/io/redis_object_store.py
--rw-r--r--   0 runner    (1001) docker     (127)     1317 2024-05-16 01:00:15.000000 deltacat-1.1.6/deltacat/io/s3_object_store.py
--rw-r--r--   0 runner    (1001) docker     (127)     8438 2024-05-16 01:00:15.000000 deltacat-1.1.6/deltacat/logs.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-16 01:13:08.000000 deltacat-1.1.6/deltacat/storage/
--rw-r--r--   0 runner    (1001) docker     (127)     1561 2024-05-16 01:00:15.000000 deltacat-1.1.6/deltacat/storage/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    21649 2024-05-16 01:00:15.000000 deltacat-1.1.6/deltacat/storage/interface.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-16 01:13:08.000000 deltacat-1.1.6/deltacat/storage/model/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-16 01:00:15.000000 deltacat-1.1.6/deltacat/storage/model/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1563 2024-05-16 01:00:15.000000 deltacat-1.1.6/deltacat/storage/model/delete_parameters.py
--rw-r--r--   0 runner    (1001) docker     (127)    14857 2024-05-16 01:00:15.000000 deltacat-1.1.6/deltacat/storage/model/delta.py
--rw-r--r--   0 runner    (1001) docker     (127)     2466 2024-05-16 01:00:15.000000 deltacat-1.1.6/deltacat/storage/model/list_result.py
--rw-r--r--   0 runner    (1001) docker     (127)     1296 2024-05-16 01:00:15.000000 deltacat-1.1.6/deltacat/storage/model/locator.py
--rw-r--r--   0 runner    (1001) docker     (127)     2086 2024-05-16 01:00:15.000000 deltacat-1.1.6/deltacat/storage/model/namespace.py
--rw-r--r--   0 runner    (1001) docker     (127)    11068 2024-05-16 01:00:15.000000 deltacat-1.1.6/deltacat/storage/model/partition.py
--rw-r--r--   0 runner    (1001) docker     (127)     1156 2024-05-16 01:00:15.000000 deltacat-1.1.6/deltacat/storage/model/sort_key.py
--rw-r--r--   0 runner    (1001) docker     (127)     7738 2024-05-16 01:00:15.000000 deltacat-1.1.6/deltacat/storage/model/stream.py
--rw-r--r--   0 runner    (1001) docker     (127)     4225 2024-05-16 01:00:15.000000 deltacat-1.1.6/deltacat/storage/model/table.py
--rw-r--r--   0 runner    (1001) docker     (127)     7413 2024-05-16 01:00:15.000000 deltacat-1.1.6/deltacat/storage/model/table_version.py
--rw-r--r--   0 runner    (1001) docker     (127)     1608 2024-05-16 01:00:15.000000 deltacat-1.1.6/deltacat/storage/model/types.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-16 01:13:08.000000 deltacat-1.1.6/deltacat/tests/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-16 01:00:15.000000 deltacat-1.1.6/deltacat/tests/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-16 01:13:08.000000 deltacat-1.1.6/deltacat/tests/aws/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-16 01:00:15.000000 deltacat-1.1.6/deltacat/tests/aws/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     3790 2024-05-16 01:00:15.000000 deltacat-1.1.6/deltacat/tests/aws/test_clients.py
--rw-r--r--   0 runner    (1001) docker     (127)     4654 2024-05-16 01:00:15.000000 deltacat-1.1.6/deltacat/tests/aws/test_s3u.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-16 01:13:08.000000 deltacat-1.1.6/deltacat/tests/catalog/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-16 01:00:15.000000 deltacat-1.1.6/deltacat/tests/catalog/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     3125 2024-05-16 01:00:15.000000 deltacat-1.1.6/deltacat/tests/catalog/test_default_catalog_impl.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-16 01:13:08.000000 deltacat-1.1.6/deltacat/tests/compute/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-16 01:00:15.000000 deltacat-1.1.6/deltacat/tests/compute/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    73645 2024-05-16 01:00:15.000000 deltacat-1.1.6/deltacat/tests/compute/compact_partition_rebase_then_incremental_test_cases.py
--rw-r--r--   0 runner    (1001) docker     (127)    22651 2024-05-16 01:00:15.000000 deltacat-1.1.6/deltacat/tests/compute/compact_partition_test_cases.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-16 01:13:08.000000 deltacat-1.1.6/deltacat/tests/compute/compactor/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-16 01:00:15.000000 deltacat-1.1.6/deltacat/tests/compute/compactor/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-16 01:13:08.000000 deltacat-1.1.6/deltacat/tests/compute/compactor/steps/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-16 01:00:15.000000 deltacat-1.1.6/deltacat/tests/compute/compactor/steps/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     9305 2024-05-16 01:00:15.000000 deltacat-1.1.6/deltacat/tests/compute/compactor/steps/test_repartition.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-16 01:13:08.000000 deltacat-1.1.6/deltacat/tests/compute/compactor/utils/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-16 01:00:15.000000 deltacat-1.1.6/deltacat/tests/compute/compactor/utils/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     4326 2024-05-16 01:00:15.000000 deltacat-1.1.6/deltacat/tests/compute/compactor/utils/test_io.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-16 01:13:08.000000 deltacat-1.1.6/deltacat/tests/compute/compactor_v2/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-16 01:00:15.000000 deltacat-1.1.6/deltacat/tests/compute/compactor_v2/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     3320 2024-05-16 01:00:15.000000 deltacat-1.1.6/deltacat/tests/compute/compactor_v2/test_compaction_session.py
--rw-r--r--   0 runner    (1001) docker     (127)      328 2024-05-16 01:00:15.000000 deltacat-1.1.6/deltacat/tests/compute/compactor_v2/test_hashlib.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-16 01:13:08.000000 deltacat-1.1.6/deltacat/tests/compute/compactor_v2/utils/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-16 01:00:15.000000 deltacat-1.1.6/deltacat/tests/compute/compactor_v2/utils/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      862 2024-05-16 01:00:15.000000 deltacat-1.1.6/deltacat/tests/compute/compactor_v2/utils/test_task_options.py
--rw-r--r--   0 runner    (1001) docker     (127)    11301 2024-05-16 01:00:15.000000 deltacat-1.1.6/deltacat/tests/compute/test_compact_partition_incremental.py
--rw-r--r--   0 runner    (1001) docker     (127)     8497 2024-05-16 01:00:15.000000 deltacat-1.1.6/deltacat/tests/compute/test_compact_partition_params.py
--rw-r--r--   0 runner    (1001) docker     (127)    14364 2024-05-16 01:00:15.000000 deltacat-1.1.6/deltacat/tests/compute/test_compact_partition_rebase_then_incremental.py
--rw-r--r--   0 runner    (1001) docker     (127)     6066 2024-05-16 01:00:15.000000 deltacat-1.1.6/deltacat/tests/compute/test_util_common.py
--rw-r--r--   0 runner    (1001) docker     (127)      929 2024-05-16 01:00:15.000000 deltacat-1.1.6/deltacat/tests/compute/test_util_constant.py
--rw-r--r--   0 runner    (1001) docker     (127)     7613 2024-05-16 01:00:15.000000 deltacat-1.1.6/deltacat/tests/compute/test_util_create_table_deltas_repo.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-16 01:13:08.000000 deltacat-1.1.6/deltacat/tests/io/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-16 01:00:15.000000 deltacat-1.1.6/deltacat/tests/io/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1376 2024-05-16 01:00:15.000000 deltacat-1.1.6/deltacat/tests/io/test_cloudpickle_bug_fix.py
--rw-r--r--   0 runner    (1001) docker     (127)     2559 2024-05-16 01:00:15.000000 deltacat-1.1.6/deltacat/tests/io/test_file_object_store.py
--rw-r--r--   0 runner    (1001) docker     (127)     8070 2024-05-16 01:00:15.000000 deltacat-1.1.6/deltacat/tests/io/test_memcached_object_store.py
--rw-r--r--   0 runner    (1001) docker     (127)     1911 2024-05-16 01:00:15.000000 deltacat-1.1.6/deltacat/tests/io/test_ray_plasma_object_store.py
--rw-r--r--   0 runner    (1001) docker     (127)     3838 2024-05-16 01:00:15.000000 deltacat-1.1.6/deltacat/tests/io/test_redis_object_store.py
--rw-r--r--   0 runner    (1001) docker     (127)     1900 2024-05-16 01:00:15.000000 deltacat-1.1.6/deltacat/tests/io/test_s3_object_store.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-16 01:13:08.000000 deltacat-1.1.6/deltacat/tests/local_deltacat_storage/
--rw-r--r--   0 runner    (1001) docker     (127)    35466 2024-05-16 01:00:15.000000 deltacat-1.1.6/deltacat/tests/local_deltacat_storage/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-16 01:13:08.000000 deltacat-1.1.6/deltacat/tests/stats/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-16 01:00:15.000000 deltacat-1.1.6/deltacat/tests/stats/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1955 2024-05-16 01:00:15.000000 deltacat-1.1.6/deltacat/tests/stats/test_intervals.py
--rw-r--r--   0 runner    (1001) docker     (127)     3828 2024-05-16 01:00:15.000000 deltacat-1.1.6/deltacat/tests/test_logs.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-16 01:13:08.000000 deltacat-1.1.6/deltacat/tests/test_utils/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-16 01:00:15.000000 deltacat-1.1.6/deltacat/tests/test_utils/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      214 2024-05-16 01:00:15.000000 deltacat-1.1.6/deltacat/tests/test_utils/constants.py
--rw-r--r--   0 runner    (1001) docker     (127)     2491 2024-05-16 01:00:15.000000 deltacat-1.1.6/deltacat/tests/test_utils/pyarrow.py
--rw-r--r--   0 runner    (1001) docker     (127)      972 2024-05-16 01:00:15.000000 deltacat-1.1.6/deltacat/tests/test_utils/storage.py
--rw-r--r--   0 runner    (1001) docker     (127)      455 2024-05-16 01:00:15.000000 deltacat-1.1.6/deltacat/tests/test_utils/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-16 01:13:08.000000 deltacat-1.1.6/deltacat/tests/utils/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-16 01:00:15.000000 deltacat-1.1.6/deltacat/tests/utils/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-16 01:13:08.000000 deltacat-1.1.6/deltacat/tests/utils/data/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-16 01:00:15.000000 deltacat-1.1.6/deltacat/tests/utils/data/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1506 2024-05-16 01:00:15.000000 deltacat-1.1.6/deltacat/tests/utils/test_cloudpickle.py
--rw-r--r--   0 runner    (1001) docker     (127)     6488 2024-05-16 01:00:15.000000 deltacat-1.1.6/deltacat/tests/utils/test_daft.py
--rw-r--r--   0 runner    (1001) docker     (127)    16339 2024-05-16 01:00:15.000000 deltacat-1.1.6/deltacat/tests/utils/test_metrics.py
--rw-r--r--   0 runner    (1001) docker     (127)      597 2024-05-16 01:00:15.000000 deltacat-1.1.6/deltacat/tests/utils/test_placement.py
--rw-r--r--   0 runner    (1001) docker     (127)    17307 2024-05-16 01:00:15.000000 deltacat-1.1.6/deltacat/tests/utils/test_pyarrow.py
--rw-r--r--   0 runner    (1001) docker     (127)    11321 2024-05-16 01:00:15.000000 deltacat-1.1.6/deltacat/tests/utils/test_record_batch_tables.py
--rw-r--r--   0 runner    (1001) docker     (127)     2560 2024-05-16 01:00:15.000000 deltacat-1.1.6/deltacat/tests/utils/test_resources.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-16 01:13:08.000000 deltacat-1.1.6/deltacat/types/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-16 01:00:15.000000 deltacat-1.1.6/deltacat/types/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2320 2024-05-16 01:00:15.000000 deltacat-1.1.6/deltacat/types/media.py
--rw-r--r--   0 runner    (1001) docker     (127)     2516 2024-05-16 01:00:15.000000 deltacat-1.1.6/deltacat/types/partial_download.py
--rw-r--r--   0 runner    (1001) docker     (127)     4409 2024-05-16 01:00:15.000000 deltacat-1.1.6/deltacat/types/tables.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-16 01:13:08.000000 deltacat-1.1.6/deltacat/utils/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-16 01:00:15.000000 deltacat-1.1.6/deltacat/utils/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1191 2024-05-16 01:00:15.000000 deltacat-1.1.6/deltacat/utils/arguments.py
--rw-r--r--   0 runner    (1001) docker     (127)     1187 2024-05-16 01:00:15.000000 deltacat-1.1.6/deltacat/utils/cloudpickle.py
--rw-r--r--   0 runner    (1001) docker     (127)     1375 2024-05-16 01:00:15.000000 deltacat-1.1.6/deltacat/utils/common.py
--rw-r--r--   0 runner    (1001) docker     (127)     5650 2024-05-16 01:00:15.000000 deltacat-1.1.6/deltacat/utils/daft.py
--rw-r--r--   0 runner    (1001) docker     (127)    10778 2024-05-16 01:00:15.000000 deltacat-1.1.6/deltacat/utils/metrics.py
--rw-r--r--   0 runner    (1001) docker     (127)     2027 2024-05-16 01:00:15.000000 deltacat-1.1.6/deltacat/utils/numpy.py
--rw-r--r--   0 runner    (1001) docker     (127)     9562 2024-05-16 01:00:15.000000 deltacat-1.1.6/deltacat/utils/pandas.py
--rw-r--r--   0 runner    (1001) docker     (127)      645 2024-05-16 01:00:15.000000 deltacat-1.1.6/deltacat/utils/performance.py
--rw-r--r--   0 runner    (1001) docker     (127)    12060 2024-05-16 01:00:15.000000 deltacat-1.1.6/deltacat/utils/placement.py
--rw-r--r--   0 runner    (1001) docker     (127)    28979 2024-05-16 01:00:15.000000 deltacat-1.1.6/deltacat/utils/pyarrow.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-16 01:13:08.000000 deltacat-1.1.6/deltacat/utils/ray_utils/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-16 01:00:15.000000 deltacat-1.1.6/deltacat/utils/ray_utils/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1951 2024-05-16 01:00:15.000000 deltacat-1.1.6/deltacat/utils/ray_utils/collections.py
--rw-r--r--   0 runner    (1001) docker     (127)     5457 2024-05-16 01:00:15.000000 deltacat-1.1.6/deltacat/utils/ray_utils/concurrency.py
--rw-r--r--   0 runner    (1001) docker     (127)     3244 2024-05-16 01:00:15.000000 deltacat-1.1.6/deltacat/utils/ray_utils/dataset.py
--rw-r--r--   0 runner    (1001) docker     (127)      464 2024-05-16 01:00:15.000000 deltacat-1.1.6/deltacat/utils/ray_utils/performance.py
--rw-r--r--   0 runner    (1001) docker     (127)     5009 2024-05-16 01:00:15.000000 deltacat-1.1.6/deltacat/utils/ray_utils/runtime.py
--rw-r--r--   0 runner    (1001) docker     (127)     8253 2024-05-16 01:00:15.000000 deltacat-1.1.6/deltacat/utils/resources.py
--rw-r--r--   0 runner    (1001) docker     (127)      662 2024-05-16 01:00:15.000000 deltacat-1.1.6/deltacat/utils/s3fs.py
--rw-r--r--   0 runner    (1001) docker     (127)     1564 2024-05-16 01:00:15.000000 deltacat-1.1.6/deltacat/utils/schema.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-16 01:13:08.000000 deltacat-1.1.6/deltacat.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     1569 2024-05-16 01:13:07.000000 deltacat-1.1.6/deltacat.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     8954 2024-05-16 01:13:08.000000 deltacat-1.1.6/deltacat.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-16 01:13:07.000000 deltacat-1.1.6/deltacat.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)      238 2024-05-16 01:13:07.000000 deltacat-1.1.6/deltacat.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)        9 2024-05-16 01:13:07.000000 deltacat-1.1.6/deltacat.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-16 01:13:08.000000 deltacat-1.1.6/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)     2059 2024-05-16 01:00:15.000000 deltacat-1.1.6/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-29 02:00:56.000000 deltacat-1.1.7/
+-rw-r--r--   0 runner    (1001) docker     (127)       25 2024-05-29 01:51:15.000000 deltacat-1.1.7/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (127)     1569 2024-05-29 02:00:56.000000 deltacat-1.1.7/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      686 2024-05-29 01:51:15.000000 deltacat-1.1.7/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-29 02:00:56.000000 deltacat-1.1.7/deltacat/
+-rw-r--r--   0 runner    (1001) docker     (127)     1777 2024-05-29 01:51:15.000000 deltacat-1.1.7/deltacat/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-29 02:00:56.000000 deltacat-1.1.7/deltacat/aws/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-29 01:51:15.000000 deltacat-1.1.7/deltacat/aws/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6948 2024-05-29 01:51:15.000000 deltacat-1.1.7/deltacat/aws/clients.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1051 2024-05-29 01:51:15.000000 deltacat-1.1.7/deltacat/aws/constants.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-29 02:00:56.000000 deltacat-1.1.7/deltacat/aws/redshift/
+-rw-r--r--   0 runner    (1001) docker     (127)      342 2024-05-29 01:51:15.000000 deltacat-1.1.7/deltacat/aws/redshift/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-29 02:00:56.000000 deltacat-1.1.7/deltacat/aws/redshift/model/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-29 01:51:15.000000 deltacat-1.1.7/deltacat/aws/redshift/model/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12987 2024-05-29 01:51:15.000000 deltacat-1.1.7/deltacat/aws/redshift/model/manifest.py
+-rw-r--r--   0 runner    (1001) docker     (127)    27738 2024-05-29 01:51:15.000000 deltacat-1.1.7/deltacat/aws/s3u.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-29 02:00:56.000000 deltacat-1.1.7/deltacat/benchmarking/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-29 01:51:15.000000 deltacat-1.1.7/deltacat/benchmarking/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1709 2024-05-29 01:51:15.000000 deltacat-1.1.7/deltacat/benchmarking/benchmark_parquet_reads.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1604 2024-05-29 01:51:15.000000 deltacat-1.1.7/deltacat/benchmarking/conftest.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-29 02:00:56.000000 deltacat-1.1.7/deltacat/catalog/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-29 01:51:15.000000 deltacat-1.1.7/deltacat/catalog/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-29 02:00:56.000000 deltacat-1.1.7/deltacat/catalog/default_catalog_impl/
+-rw-r--r--   0 runner    (1001) docker     (127)    12677 2024-05-29 01:51:15.000000 deltacat-1.1.7/deltacat/catalog/default_catalog_impl/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8745 2024-05-29 01:51:15.000000 deltacat-1.1.7/deltacat/catalog/delegate.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6556 2024-05-29 01:51:15.000000 deltacat-1.1.7/deltacat/catalog/interface.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-29 02:00:56.000000 deltacat-1.1.7/deltacat/catalog/model/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-29 01:51:15.000000 deltacat-1.1.7/deltacat/catalog/model/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2212 2024-05-29 01:51:15.000000 deltacat-1.1.7/deltacat/catalog/model/catalog.py
+-rw-r--r--   0 runner    (1001) docker     (127)      727 2024-05-29 01:51:15.000000 deltacat-1.1.7/deltacat/catalog/model/table_definition.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-29 02:00:56.000000 deltacat-1.1.7/deltacat/compute/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-29 01:51:15.000000 deltacat-1.1.7/deltacat/compute/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-29 02:00:56.000000 deltacat-1.1.7/deltacat/compute/compactor/
+-rw-r--r--   0 runner    (1001) docker     (127)     1022 2024-05-29 01:51:15.000000 deltacat-1.1.7/deltacat/compute/compactor/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    27612 2024-05-29 01:51:15.000000 deltacat-1.1.7/deltacat/compute/compactor/compaction_session.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-29 02:00:56.000000 deltacat-1.1.7/deltacat/compute/compactor/model/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-29 01:51:15.000000 deltacat-1.1.7/deltacat/compute/compactor/model/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    15195 2024-05-29 01:51:15.000000 deltacat-1.1.7/deltacat/compute/compactor/model/compact_partition_params.py
+-rw-r--r--   0 runner    (1001) docker     (127)    30547 2024-05-29 01:51:15.000000 deltacat-1.1.7/deltacat/compute/compactor/model/compaction_session_audit_info.py
+-rw-r--r--   0 runner    (1001) docker     (127)       87 2024-05-29 01:51:15.000000 deltacat-1.1.7/deltacat/compute/compactor/model/compactor_version.py
+-rw-r--r--   0 runner    (1001) docker     (127)      292 2024-05-29 01:51:15.000000 deltacat-1.1.7/deltacat/compute/compactor/model/dedupe_result.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12258 2024-05-29 01:51:15.000000 deltacat-1.1.7/deltacat/compute/compactor/model/delta_annotated.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3676 2024-05-29 01:51:15.000000 deltacat-1.1.7/deltacat/compute/compactor/model/delta_file_envelope.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1905 2024-05-29 01:51:15.000000 deltacat-1.1.7/deltacat/compute/compactor/model/delta_file_locator.py
+-rw-r--r--   0 runner    (1001) docker     (127)      275 2024-05-29 01:51:15.000000 deltacat-1.1.7/deltacat/compute/compactor/model/hash_bucket_result.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2656 2024-05-29 01:51:15.000000 deltacat-1.1.7/deltacat/compute/compactor/model/materialize_result.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10449 2024-05-29 01:51:15.000000 deltacat-1.1.7/deltacat/compute/compactor/model/primary_key_index.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1324 2024-05-29 01:51:15.000000 deltacat-1.1.7/deltacat/compute/compactor/model/pyarrow_write_result.py
+-rw-r--r--   0 runner    (1001) docker     (127)      140 2024-05-29 01:51:15.000000 deltacat-1.1.7/deltacat/compute/compactor/model/repartition_result.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5115 2024-05-29 01:51:15.000000 deltacat-1.1.7/deltacat/compute/compactor/model/round_completion_info.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1487 2024-05-29 01:51:15.000000 deltacat-1.1.7/deltacat/compute/compactor/model/table_object_store.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7240 2024-05-29 01:51:15.000000 deltacat-1.1.7/deltacat/compute/compactor/repartition_session.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-29 02:00:56.000000 deltacat-1.1.7/deltacat/compute/compactor/steps/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-29 01:51:15.000000 deltacat-1.1.7/deltacat/compute/compactor/steps/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10190 2024-05-29 01:51:15.000000 deltacat-1.1.7/deltacat/compute/compactor/steps/dedupe.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10655 2024-05-29 01:51:15.000000 deltacat-1.1.7/deltacat/compute/compactor/steps/hash_bucket.py
+-rw-r--r--   0 runner    (1001) docker     (127)    14246 2024-05-29 01:51:15.000000 deltacat-1.1.7/deltacat/compute/compactor/steps/materialize.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10960 2024-05-29 01:51:15.000000 deltacat-1.1.7/deltacat/compute/compactor/steps/repartition.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-29 02:00:56.000000 deltacat-1.1.7/deltacat/compute/compactor/utils/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-29 01:51:15.000000 deltacat-1.1.7/deltacat/compute/compactor/utils/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    17303 2024-05-29 01:51:15.000000 deltacat-1.1.7/deltacat/compute/compactor/utils/io.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2435 2024-05-29 01:51:15.000000 deltacat-1.1.7/deltacat/compute/compactor/utils/primary_key_index.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2345 2024-05-29 01:51:15.000000 deltacat-1.1.7/deltacat/compute/compactor/utils/round_completion_file.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2397 2024-05-29 01:51:15.000000 deltacat-1.1.7/deltacat/compute/compactor/utils/sort_key.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9399 2024-05-29 01:51:15.000000 deltacat-1.1.7/deltacat/compute/compactor/utils/system_columns.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-29 02:00:56.000000 deltacat-1.1.7/deltacat/compute/compactor_v2/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-29 01:51:15.000000 deltacat-1.1.7/deltacat/compute/compactor_v2/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    27574 2024-05-29 01:51:15.000000 deltacat-1.1.7/deltacat/compute/compactor_v2/compaction_session.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2564 2024-05-29 01:51:15.000000 deltacat-1.1.7/deltacat/compute/compactor_v2/constants.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-29 02:00:56.000000 deltacat-1.1.7/deltacat/compute/compactor_v2/deletes/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-29 01:51:15.000000 deltacat-1.1.7/deltacat/compute/compactor_v2/deletes/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3111 2024-05-29 01:51:15.000000 deltacat-1.1.7/deltacat/compute/compactor_v2/deletes/delete_file_envelope.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2833 2024-05-29 01:51:15.000000 deltacat-1.1.7/deltacat/compute/compactor_v2/deletes/delete_strategy.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6503 2024-05-29 01:51:15.000000 deltacat-1.1.7/deltacat/compute/compactor_v2/deletes/delete_strategy_equality_delete.py
+-rw-r--r--   0 runner    (1001) docker     (127)      558 2024-05-29 01:51:15.000000 deltacat-1.1.7/deltacat/compute/compactor_v2/deletes/model.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6640 2024-05-29 01:51:15.000000 deltacat-1.1.7/deltacat/compute/compactor_v2/deletes/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-29 02:00:56.000000 deltacat-1.1.7/deltacat/compute/compactor_v2/model/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-29 01:51:15.000000 deltacat-1.1.7/deltacat/compute/compactor_v2/model/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      579 2024-05-29 01:51:15.000000 deltacat-1.1.7/deltacat/compute/compactor_v2/model/compaction_session.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3042 2024-05-29 01:51:15.000000 deltacat-1.1.7/deltacat/compute/compactor_v2/model/hash_bucket_input.py
+-rw-r--r--   0 runner    (1001) docker     (127)      309 2024-05-29 01:51:15.000000 deltacat-1.1.7/deltacat/compute/compactor_v2/model/hash_bucket_result.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7410 2024-05-29 01:51:15.000000 deltacat-1.1.7/deltacat/compute/compactor_v2/model/merge_file_group.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5416 2024-05-29 01:51:15.000000 deltacat-1.1.7/deltacat/compute/compactor_v2/model/merge_input.py
+-rw-r--r--   0 runner    (1001) docker     (127)      436 2024-05-29 01:51:15.000000 deltacat-1.1.7/deltacat/compute/compactor_v2/model/merge_result.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-29 02:00:56.000000 deltacat-1.1.7/deltacat/compute/compactor_v2/steps/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-29 01:51:15.000000 deltacat-1.1.7/deltacat/compute/compactor_v2/steps/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6852 2024-05-29 01:51:15.000000 deltacat-1.1.7/deltacat/compute/compactor_v2/steps/hash_bucket.py
+-rw-r--r--   0 runner    (1001) docker     (127)    21880 2024-05-29 01:51:15.000000 deltacat-1.1.7/deltacat/compute/compactor_v2/steps/merge.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-29 02:00:56.000000 deltacat-1.1.7/deltacat/compute/compactor_v2/utils/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-29 01:51:15.000000 deltacat-1.1.7/deltacat/compute/compactor_v2/utils/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2156 2024-05-29 01:51:15.000000 deltacat-1.1.7/deltacat/compute/compactor_v2/utils/content_type_params.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1932 2024-05-29 01:51:15.000000 deltacat-1.1.7/deltacat/compute/compactor_v2/utils/dedupe.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3635 2024-05-29 01:51:15.000000 deltacat-1.1.7/deltacat/compute/compactor_v2/utils/delta.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5264 2024-05-29 01:51:15.000000 deltacat-1.1.7/deltacat/compute/compactor_v2/utils/io.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5244 2024-05-29 01:51:15.000000 deltacat-1.1.7/deltacat/compute/compactor_v2/utils/merge.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11393 2024-05-29 01:51:15.000000 deltacat-1.1.7/deltacat/compute/compactor_v2/utils/primary_key_index.py
+-rw-r--r--   0 runner    (1001) docker     (127)    14285 2024-05-29 01:51:15.000000 deltacat-1.1.7/deltacat/compute/compactor_v2/utils/task_options.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-29 02:00:56.000000 deltacat-1.1.7/deltacat/compute/merge_on_read/
+-rw-r--r--   0 runner    (1001) docker     (127)      214 2024-05-29 01:51:15.000000 deltacat-1.1.7/deltacat/compute/merge_on_read/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1400 2024-05-29 01:51:15.000000 deltacat-1.1.7/deltacat/compute/merge_on_read/daft.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-29 02:00:56.000000 deltacat-1.1.7/deltacat/compute/merge_on_read/model/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-29 01:51:15.000000 deltacat-1.1.7/deltacat/compute/merge_on_read/model/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2035 2024-05-29 01:51:15.000000 deltacat-1.1.7/deltacat/compute/merge_on_read/model/merge_on_read_params.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-29 02:00:56.000000 deltacat-1.1.7/deltacat/compute/merge_on_read/utils/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-29 01:51:15.000000 deltacat-1.1.7/deltacat/compute/merge_on_read/utils/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1367 2024-05-29 01:51:15.000000 deltacat-1.1.7/deltacat/compute/merge_on_read/utils/delta.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-29 02:00:56.000000 deltacat-1.1.7/deltacat/compute/metastats/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-29 01:51:15.000000 deltacat-1.1.7/deltacat/compute/metastats/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-29 02:00:56.000000 deltacat-1.1.7/deltacat/compute/metastats/config/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-29 01:51:15.000000 deltacat-1.1.7/deltacat/compute/metastats/config/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    18731 2024-05-29 01:51:15.000000 deltacat-1.1.7/deltacat/compute/metastats/meta_stats.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-29 02:00:56.000000 deltacat-1.1.7/deltacat/compute/metastats/model/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-29 01:51:15.000000 deltacat-1.1.7/deltacat/compute/metastats/model/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1123 2024-05-29 01:51:15.000000 deltacat-1.1.7/deltacat/compute/metastats/model/partition_stats_dict.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2849 2024-05-29 01:51:15.000000 deltacat-1.1.7/deltacat/compute/metastats/model/stats_cluster_size_estimator.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7363 2024-05-29 01:51:15.000000 deltacat-1.1.7/deltacat/compute/metastats/stats.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-29 02:00:56.000000 deltacat-1.1.7/deltacat/compute/metastats/utils/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-29 01:51:15.000000 deltacat-1.1.7/deltacat/compute/metastats/utils/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      869 2024-05-29 01:51:15.000000 deltacat-1.1.7/deltacat/compute/metastats/utils/constants.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9007 2024-05-29 01:51:15.000000 deltacat-1.1.7/deltacat/compute/metastats/utils/io.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1143 2024-05-29 01:51:15.000000 deltacat-1.1.7/deltacat/compute/metastats/utils/pyarrow_memory_estimation_function.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4516 2024-05-29 01:51:15.000000 deltacat-1.1.7/deltacat/compute/metastats/utils/ray_utils.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-29 02:00:56.000000 deltacat-1.1.7/deltacat/compute/stats/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-29 01:51:15.000000 deltacat-1.1.7/deltacat/compute/stats/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8837 2024-05-29 01:51:15.000000 deltacat-1.1.7/deltacat/compute/stats/basic.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-29 02:00:56.000000 deltacat-1.1.7/deltacat/compute/stats/models/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-29 01:51:15.000000 deltacat-1.1.7/deltacat/compute/stats/models/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3300 2024-05-29 01:51:15.000000 deltacat-1.1.7/deltacat/compute/stats/models/delta_column_stats.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8556 2024-05-29 01:51:15.000000 deltacat-1.1.7/deltacat/compute/stats/models/delta_stats.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1624 2024-05-29 01:51:15.000000 deltacat-1.1.7/deltacat/compute/stats/models/delta_stats_cache_result.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2419 2024-05-29 01:51:15.000000 deltacat-1.1.7/deltacat/compute/stats/models/manifest_entry_stats.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3820 2024-05-29 01:51:15.000000 deltacat-1.1.7/deltacat/compute/stats/models/stats_result.py
+-rw-r--r--   0 runner    (1001) docker     (127)      215 2024-05-29 01:51:15.000000 deltacat-1.1.7/deltacat/compute/stats/types.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-29 02:00:56.000000 deltacat-1.1.7/deltacat/compute/stats/utils/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-29 01:51:15.000000 deltacat-1.1.7/deltacat/compute/stats/utils/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3094 2024-05-29 01:51:15.000000 deltacat-1.1.7/deltacat/compute/stats/utils/intervals.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9059 2024-05-29 01:51:15.000000 deltacat-1.1.7/deltacat/compute/stats/utils/io.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3693 2024-05-29 01:51:15.000000 deltacat-1.1.7/deltacat/compute/stats/utils/manifest_stats_file.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1939 2024-05-29 01:51:15.000000 deltacat-1.1.7/deltacat/constants.py
+-rw-r--r--   0 runner    (1001) docker     (127)      199 2024-05-29 01:51:15.000000 deltacat-1.1.7/deltacat/exceptions.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-29 02:00:56.000000 deltacat-1.1.7/deltacat/io/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-29 01:51:15.000000 deltacat-1.1.7/deltacat/io/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-29 02:00:56.000000 deltacat-1.1.7/deltacat/io/aws/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-29 01:51:15.000000 deltacat-1.1.7/deltacat/io/aws/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-29 02:00:56.000000 deltacat-1.1.7/deltacat/io/aws/redshift/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-29 01:51:15.000000 deltacat-1.1.7/deltacat/io/aws/redshift/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    22599 2024-05-29 01:51:15.000000 deltacat-1.1.7/deltacat/io/aws/redshift/redshift_datasource.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3755 2024-05-29 01:51:15.000000 deltacat-1.1.7/deltacat/io/dataset.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1346 2024-05-29 01:51:15.000000 deltacat-1.1.7/deltacat/io/file_object_store.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9185 2024-05-29 01:51:15.000000 deltacat-1.1.7/deltacat/io/memcached_object_store.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1576 2024-05-29 01:51:15.000000 deltacat-1.1.7/deltacat/io/object_store.py
+-rw-r--r--   0 runner    (1001) docker     (127)      905 2024-05-29 01:51:15.000000 deltacat-1.1.7/deltacat/io/ray_plasma_object_store.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7023 2024-05-29 01:51:15.000000 deltacat-1.1.7/deltacat/io/read_api.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3507 2024-05-29 01:51:15.000000 deltacat-1.1.7/deltacat/io/redis_object_store.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1317 2024-05-29 01:51:15.000000 deltacat-1.1.7/deltacat/io/s3_object_store.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8438 2024-05-29 01:51:15.000000 deltacat-1.1.7/deltacat/logs.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-29 02:00:56.000000 deltacat-1.1.7/deltacat/storage/
+-rw-r--r--   0 runner    (1001) docker     (127)     1561 2024-05-29 01:51:15.000000 deltacat-1.1.7/deltacat/storage/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    21913 2024-05-29 01:51:15.000000 deltacat-1.1.7/deltacat/storage/interface.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-29 02:00:56.000000 deltacat-1.1.7/deltacat/storage/model/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-29 01:51:15.000000 deltacat-1.1.7/deltacat/storage/model/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1563 2024-05-29 01:51:15.000000 deltacat-1.1.7/deltacat/storage/model/delete_parameters.py
+-rw-r--r--   0 runner    (1001) docker     (127)    14857 2024-05-29 01:51:15.000000 deltacat-1.1.7/deltacat/storage/model/delta.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2466 2024-05-29 01:51:15.000000 deltacat-1.1.7/deltacat/storage/model/list_result.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1296 2024-05-29 01:51:15.000000 deltacat-1.1.7/deltacat/storage/model/locator.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2086 2024-05-29 01:51:15.000000 deltacat-1.1.7/deltacat/storage/model/namespace.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11068 2024-05-29 01:51:15.000000 deltacat-1.1.7/deltacat/storage/model/partition.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1156 2024-05-29 01:51:15.000000 deltacat-1.1.7/deltacat/storage/model/sort_key.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7738 2024-05-29 01:51:15.000000 deltacat-1.1.7/deltacat/storage/model/stream.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4225 2024-05-29 01:51:15.000000 deltacat-1.1.7/deltacat/storage/model/table.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7413 2024-05-29 01:51:15.000000 deltacat-1.1.7/deltacat/storage/model/table_version.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1608 2024-05-29 01:51:15.000000 deltacat-1.1.7/deltacat/storage/model/types.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-29 02:00:56.000000 deltacat-1.1.7/deltacat/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-29 01:51:15.000000 deltacat-1.1.7/deltacat/tests/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-29 02:00:56.000000 deltacat-1.1.7/deltacat/tests/aws/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-29 01:51:15.000000 deltacat-1.1.7/deltacat/tests/aws/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3790 2024-05-29 01:51:15.000000 deltacat-1.1.7/deltacat/tests/aws/test_clients.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7805 2024-05-29 01:51:15.000000 deltacat-1.1.7/deltacat/tests/aws/test_s3u.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-29 02:00:56.000000 deltacat-1.1.7/deltacat/tests/catalog/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-29 01:51:15.000000 deltacat-1.1.7/deltacat/tests/catalog/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3180 2024-05-29 01:51:15.000000 deltacat-1.1.7/deltacat/tests/catalog/test_default_catalog_impl.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-29 02:00:56.000000 deltacat-1.1.7/deltacat/tests/compute/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-29 01:51:15.000000 deltacat-1.1.7/deltacat/tests/compute/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    73645 2024-05-29 01:51:15.000000 deltacat-1.1.7/deltacat/tests/compute/compact_partition_rebase_then_incremental_test_cases.py
+-rw-r--r--   0 runner    (1001) docker     (127)    25061 2024-05-29 01:51:15.000000 deltacat-1.1.7/deltacat/tests/compute/compact_partition_test_cases.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-29 02:00:56.000000 deltacat-1.1.7/deltacat/tests/compute/compactor/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-29 01:51:15.000000 deltacat-1.1.7/deltacat/tests/compute/compactor/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-29 02:00:56.000000 deltacat-1.1.7/deltacat/tests/compute/compactor/steps/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-29 01:51:15.000000 deltacat-1.1.7/deltacat/tests/compute/compactor/steps/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9305 2024-05-29 01:51:15.000000 deltacat-1.1.7/deltacat/tests/compute/compactor/steps/test_repartition.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-29 02:00:56.000000 deltacat-1.1.7/deltacat/tests/compute/compactor/utils/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-29 01:51:15.000000 deltacat-1.1.7/deltacat/tests/compute/compactor/utils/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4326 2024-05-29 01:51:15.000000 deltacat-1.1.7/deltacat/tests/compute/compactor/utils/test_io.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-29 02:00:56.000000 deltacat-1.1.7/deltacat/tests/compute/compactor_v2/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-29 01:51:15.000000 deltacat-1.1.7/deltacat/tests/compute/compactor_v2/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3375 2024-05-29 01:51:15.000000 deltacat-1.1.7/deltacat/tests/compute/compactor_v2/test_compaction_session.py
+-rw-r--r--   0 runner    (1001) docker     (127)      328 2024-05-29 01:51:15.000000 deltacat-1.1.7/deltacat/tests/compute/compactor_v2/test_hashlib.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-29 02:00:56.000000 deltacat-1.1.7/deltacat/tests/compute/compactor_v2/utils/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-29 01:51:15.000000 deltacat-1.1.7/deltacat/tests/compute/compactor_v2/utils/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      862 2024-05-29 01:51:15.000000 deltacat-1.1.7/deltacat/tests/compute/compactor_v2/utils/test_task_options.py
+-rw-r--r--   0 runner    (1001) docker     (127)    13995 2024-05-29 01:51:15.000000 deltacat-1.1.7/deltacat/tests/compute/test_compact_partition_incremental.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8497 2024-05-29 01:51:15.000000 deltacat-1.1.7/deltacat/tests/compute/test_compact_partition_params.py
+-rw-r--r--   0 runner    (1001) docker     (127)    14159 2024-05-29 01:51:15.000000 deltacat-1.1.7/deltacat/tests/compute/test_compact_partition_rebase_then_incremental.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6066 2024-05-29 01:51:15.000000 deltacat-1.1.7/deltacat/tests/compute/test_util_common.py
+-rw-r--r--   0 runner    (1001) docker     (127)      929 2024-05-29 01:51:15.000000 deltacat-1.1.7/deltacat/tests/compute/test_util_constant.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8992 2024-05-29 01:51:15.000000 deltacat-1.1.7/deltacat/tests/compute/test_util_create_table_deltas_repo.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-29 02:00:56.000000 deltacat-1.1.7/deltacat/tests/io/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-29 01:51:15.000000 deltacat-1.1.7/deltacat/tests/io/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1376 2024-05-29 01:51:15.000000 deltacat-1.1.7/deltacat/tests/io/test_cloudpickle_bug_fix.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2559 2024-05-29 01:51:15.000000 deltacat-1.1.7/deltacat/tests/io/test_file_object_store.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8070 2024-05-29 01:51:15.000000 deltacat-1.1.7/deltacat/tests/io/test_memcached_object_store.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1911 2024-05-29 01:51:15.000000 deltacat-1.1.7/deltacat/tests/io/test_ray_plasma_object_store.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3838 2024-05-29 01:51:15.000000 deltacat-1.1.7/deltacat/tests/io/test_redis_object_store.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1900 2024-05-29 01:51:15.000000 deltacat-1.1.7/deltacat/tests/io/test_s3_object_store.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-29 02:00:56.000000 deltacat-1.1.7/deltacat/tests/local_deltacat_storage/
+-rw-r--r--   0 runner    (1001) docker     (127)    36316 2024-05-29 01:51:15.000000 deltacat-1.1.7/deltacat/tests/local_deltacat_storage/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-29 02:00:56.000000 deltacat-1.1.7/deltacat/tests/stats/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-29 01:51:15.000000 deltacat-1.1.7/deltacat/tests/stats/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1955 2024-05-29 01:51:15.000000 deltacat-1.1.7/deltacat/tests/stats/test_intervals.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3828 2024-05-29 01:51:15.000000 deltacat-1.1.7/deltacat/tests/test_logs.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-29 02:00:56.000000 deltacat-1.1.7/deltacat/tests/test_utils/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-29 01:51:15.000000 deltacat-1.1.7/deltacat/tests/test_utils/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      214 2024-05-29 01:51:15.000000 deltacat-1.1.7/deltacat/tests/test_utils/constants.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2491 2024-05-29 01:51:15.000000 deltacat-1.1.7/deltacat/tests/test_utils/pyarrow.py
+-rw-r--r--   0 runner    (1001) docker     (127)      972 2024-05-29 01:51:15.000000 deltacat-1.1.7/deltacat/tests/test_utils/storage.py
+-rw-r--r--   0 runner    (1001) docker     (127)      455 2024-05-29 01:51:15.000000 deltacat-1.1.7/deltacat/tests/test_utils/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-29 02:00:56.000000 deltacat-1.1.7/deltacat/tests/utils/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-29 01:51:15.000000 deltacat-1.1.7/deltacat/tests/utils/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-29 02:00:56.000000 deltacat-1.1.7/deltacat/tests/utils/data/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-29 01:51:15.000000 deltacat-1.1.7/deltacat/tests/utils/data/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-29 02:00:56.000000 deltacat-1.1.7/deltacat/tests/utils/ray_utils/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-29 01:51:15.000000 deltacat-1.1.7/deltacat/tests/utils/ray_utils/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1211 2024-05-29 01:51:15.000000 deltacat-1.1.7/deltacat/tests/utils/ray_utils/test_concurrency.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1506 2024-05-29 01:51:15.000000 deltacat-1.1.7/deltacat/tests/utils/test_cloudpickle.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6488 2024-05-29 01:51:15.000000 deltacat-1.1.7/deltacat/tests/utils/test_daft.py
+-rw-r--r--   0 runner    (1001) docker     (127)    16339 2024-05-29 01:51:15.000000 deltacat-1.1.7/deltacat/tests/utils/test_metrics.py
+-rw-r--r--   0 runner    (1001) docker     (127)      597 2024-05-29 01:51:15.000000 deltacat-1.1.7/deltacat/tests/utils/test_placement.py
+-rw-r--r--   0 runner    (1001) docker     (127)    17307 2024-05-29 01:51:15.000000 deltacat-1.1.7/deltacat/tests/utils/test_pyarrow.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11321 2024-05-29 01:51:15.000000 deltacat-1.1.7/deltacat/tests/utils/test_record_batch_tables.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3443 2024-05-29 01:51:15.000000 deltacat-1.1.7/deltacat/tests/utils/test_resources.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-29 02:00:56.000000 deltacat-1.1.7/deltacat/types/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-29 01:51:15.000000 deltacat-1.1.7/deltacat/types/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2320 2024-05-29 01:51:15.000000 deltacat-1.1.7/deltacat/types/media.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2516 2024-05-29 01:51:15.000000 deltacat-1.1.7/deltacat/types/partial_download.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4409 2024-05-29 01:51:15.000000 deltacat-1.1.7/deltacat/types/tables.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-29 02:00:56.000000 deltacat-1.1.7/deltacat/utils/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-29 01:51:15.000000 deltacat-1.1.7/deltacat/utils/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1191 2024-05-29 01:51:15.000000 deltacat-1.1.7/deltacat/utils/arguments.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1187 2024-05-29 01:51:15.000000 deltacat-1.1.7/deltacat/utils/cloudpickle.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1375 2024-05-29 01:51:15.000000 deltacat-1.1.7/deltacat/utils/common.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5650 2024-05-29 01:51:15.000000 deltacat-1.1.7/deltacat/utils/daft.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10778 2024-05-29 01:51:15.000000 deltacat-1.1.7/deltacat/utils/metrics.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2027 2024-05-29 01:51:15.000000 deltacat-1.1.7/deltacat/utils/numpy.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9562 2024-05-29 01:51:15.000000 deltacat-1.1.7/deltacat/utils/pandas.py
+-rw-r--r--   0 runner    (1001) docker     (127)      645 2024-05-29 01:51:15.000000 deltacat-1.1.7/deltacat/utils/performance.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12060 2024-05-29 01:51:15.000000 deltacat-1.1.7/deltacat/utils/placement.py
+-rw-r--r--   0 runner    (1001) docker     (127)    28979 2024-05-29 01:51:15.000000 deltacat-1.1.7/deltacat/utils/pyarrow.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-29 02:00:56.000000 deltacat-1.1.7/deltacat/utils/ray_utils/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-29 01:51:15.000000 deltacat-1.1.7/deltacat/utils/ray_utils/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1951 2024-05-29 01:51:15.000000 deltacat-1.1.7/deltacat/utils/ray_utils/collections.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5457 2024-05-29 01:51:15.000000 deltacat-1.1.7/deltacat/utils/ray_utils/concurrency.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3244 2024-05-29 01:51:15.000000 deltacat-1.1.7/deltacat/utils/ray_utils/dataset.py
+-rw-r--r--   0 runner    (1001) docker     (127)      464 2024-05-29 01:51:15.000000 deltacat-1.1.7/deltacat/utils/ray_utils/performance.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5009 2024-05-29 01:51:15.000000 deltacat-1.1.7/deltacat/utils/ray_utils/runtime.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9757 2024-05-29 01:51:15.000000 deltacat-1.1.7/deltacat/utils/resources.py
+-rw-r--r--   0 runner    (1001) docker     (127)      662 2024-05-29 01:51:15.000000 deltacat-1.1.7/deltacat/utils/s3fs.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1564 2024-05-29 01:51:15.000000 deltacat-1.1.7/deltacat/utils/schema.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-29 02:00:56.000000 deltacat-1.1.7/deltacat.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     1569 2024-05-29 02:00:56.000000 deltacat-1.1.7/deltacat.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     9106 2024-05-29 02:00:56.000000 deltacat-1.1.7/deltacat.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-29 02:00:56.000000 deltacat-1.1.7/deltacat.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      238 2024-05-29 02:00:56.000000 deltacat-1.1.7/deltacat.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        9 2024-05-29 02:00:56.000000 deltacat-1.1.7/deltacat.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-29 02:00:56.000000 deltacat-1.1.7/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)     2059 2024-05-29 01:51:15.000000 deltacat-1.1.7/setup.py
```

### Comparing `deltacat-1.1.6/PKG-INFO` & `deltacat-1.1.7/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: deltacat
-Version: 1.1.6
+Version: 1.1.7
 Summary: A scalable, fast, ACID-compliant Data Catalog powered by Ray.
 Home-page: https://github.com/ray-project/deltacat
 Author: Ray Team
 License: UNKNOWN
 Description: # DeltaCAT
         
         DeltaCAT is a Pythonic Data Catalog powered by Ray.
```

### Comparing `deltacat-1.1.6/README.md` & `deltacat-1.1.7/README.md`

 * *Files identical despite different names*

### Comparing `deltacat-1.1.6/deltacat/__init__.py` & `deltacat-1.1.7/deltacat/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -40,15 +40,15 @@
     SortOrder,
 )
 from deltacat.types.media import ContentEncoding, ContentType, TableType
 from deltacat.types.tables import TableWriteMode
 
 deltacat.logs.configure_deltacat_logger(logging.getLogger(__name__))
 
-__version__ = "1.1.6"
+__version__ = "1.1.7"
 
 
 __all__ = [
     "__version__",
     "all_catalogs",
     "alter_table",
     "create_table",
```

### Comparing `deltacat-1.1.6/deltacat/aws/clients.py` & `deltacat-1.1.7/deltacat/aws/clients.py`

 * *Files identical despite different names*

### Comparing `deltacat-1.1.6/deltacat/aws/redshift/model/manifest.py` & `deltacat-1.1.7/deltacat/aws/redshift/model/manifest.py`

 * *Files identical despite different names*

### Comparing `deltacat-1.1.6/deltacat/aws/s3u.py` & `deltacat-1.1.7/deltacat/aws/s3u.py`

 * *Files 4% similar despite different names*

```diff
@@ -2,40 +2,41 @@
 import multiprocessing
 from functools import partial
 from typing import Any, Callable, Dict, Generator, List, Optional, Union
 from uuid import uuid4
 from botocore.config import Config
 from deltacat.aws.constants import (
     BOTO_MAX_RETRIES,
-    RETRY_STOP_AFTER_DELAY,
-    RETRYABLE_PUT_OBJECT_ERROR_CODES,
+    UPLOAD_DOWNLOAD_RETRY_STOP_AFTER_DELAY,
+    BOTO_THROTTLING_ERROR_CODES,
+    RETRYABLE_TRANSIENT_ERRORS,
+    BOTO_TIMEOUT_ERROR_CODES,
+    UPLOAD_SLICED_TABLE_RETRY_STOP_AFTER_DELAY,
+    DOWNLOAD_MANIFEST_ENTRY_RETRY_STOP_AFTER_DELAY,
 )
 
 import pyarrow as pa
 import ray
 import s3fs
 from boto3.resources.base import ServiceResource
 from botocore.client import BaseClient
-from botocore.exceptions import ClientError, NoCredentialsError
+from botocore.exceptions import ClientError
 from ray.data.block import Block, BlockAccessor, BlockMetadata
 from ray.data.datasource import BlockWritePathProvider
 from ray.types import ObjectRef
 from tenacity import (
     Retrying,
     retry_if_exception_type,
     retry_if_not_exception_type,
     stop_after_delay,
     wait_random_exponential,
 )
 from deltacat.utils.ray_utils.concurrency import invoke_parallel
 import deltacat.aws.clients as aws_utils
 from deltacat import logs
-from deltacat.aws.constants import (
-    TIMEOUT_ERROR_CODES,
-)
 from deltacat.exceptions import NonRetryableError, RetryableError
 from deltacat.storage import (
     DistributedDataset,
     LocalDataset,
     LocalTable,
     Manifest,
     ManifestEntry,
@@ -253,18 +254,29 @@
             include_columns,
             file_reader_kwargs_provider,
             partial_file_download_params,
             **s3_client_kwargs,
         )
         return table
     except ClientError as e:
-        if e.response["Error"]["Code"] in TIMEOUT_ERROR_CODES:
+        if (
+            e.response["Error"]["Code"]
+            in BOTO_TIMEOUT_ERROR_CODES | BOTO_THROTTLING_ERROR_CODES
+        ):
             # Timeout error not caught by botocore
-            raise RetryableError(f"Retry table download from: {s3_url}") from e
-        raise NonRetryableError(f"Failed table download from: {s3_url}") from e
+            raise RetryableError(
+                f"Retry table download from: {s3_url} after receiving {type(e).__name__}"
+            ) from e
+        raise NonRetryableError(
+            f"Failed table download from: {s3_url} after receiving {type(e).__name__}"
+        ) from e
+    except RETRYABLE_TRANSIENT_ERRORS as e:
+        raise RetryableError(
+            f"Retry upload for: {s3_url} after receiving {type(e).__name__}"
+        ) from e
     except BaseException as e:
         logger.warn(
             f"Read has failed for {s3_url} and content_type={content_type} "
             f"and encoding={content_encoding}. Error: {e}",
             exc_info=True,
         )
         raise e
@@ -281,15 +293,15 @@
     content_type: ContentType = ContentType.PARQUET,
     **s3_client_kwargs,
 ) -> ManifestEntryList:
 
     # @retry decorator can't be pickled by Ray, so wrap upload in Retrying
     retrying = Retrying(
         wait=wait_random_exponential(multiplier=1, max=60),
-        stop=stop_after_delay(30 * 60),
+        stop=stop_after_delay(UPLOAD_SLICED_TABLE_RETRY_STOP_AFTER_DELAY),
         retry=retry_if_exception_type(RetryableError),
     )
 
     manifest_entries = ManifestEntryList()
     table_record_count = get_table_length(table)
 
     if max_records_per_entry is None or not table_record_count:
@@ -362,16 +374,31 @@
                 metadata[block_idx].size_bytes,
                 **s3_client_kwargs,
             )
             manifest_entries.append(manifest_entry)
         except ClientError as e:
             if e.response["Error"]["Code"] == "NoSuchKey":
                 # s3fs may swallow S3 errors - we were probably throttled
-                raise RetryableError(f"Retry table upload to: {s3_url}") from e
-            raise NonRetryableError(f"Failed table upload to: {s3_url}") from e
+                raise RetryableError(
+                    f"Retry table download from: {s3_url} after receiving {type(e).__name__}"
+                ) from e
+            if (
+                e.response["Error"]["Code"]
+                in BOTO_TIMEOUT_ERROR_CODES | BOTO_THROTTLING_ERROR_CODES
+            ):
+                raise RetryableError(
+                    f"Retry table download from: {s3_url} after receiving {type(e).__name__}"
+                ) from e
+            raise NonRetryableError(
+                f"Failed table upload to: {s3_url} after receiving {type(e).__name__}"
+            ) from e
+        except RETRYABLE_TRANSIENT_ERRORS as e:
+            raise RetryableError(
+                f"Retry upload for: {s3_url} after receiving {type(e).__name__}"
+            ) from e
         except BaseException as e:
             logger.warn(
                 f"Upload has failed for {s3_url} and content_type={content_type}. Error: {e}",
                 exc_info=True,
             )
             raise e
     return manifest_entries
@@ -411,15 +438,15 @@
             if isinstance(type_params, PartialFileDownloadParams):
                 partial_file_download_params = type_params
                 break
 
     # @retry decorator can't be pickled by Ray, so wrap download in Retrying
     retrying = Retrying(
         wait=wait_random_exponential(multiplier=1, max=60),
-        stop=stop_after_delay(30 * 60),
+        stop=stop_after_delay(DOWNLOAD_MANIFEST_ENTRY_RETRY_STOP_AFTER_DELAY),
         retry=retry_if_not_exception_type(NonRetryableError),
     )
     table = retrying(
         read_file,
         s3_url,
         content_type,
         content_encoding,
@@ -507,15 +534,15 @@
 
 def upload(s3_url: str, body, **s3_client_kwargs) -> Dict[str, Any]:
 
     parsed_s3_url = parse_s3_url(s3_url)
     s3 = s3_client_cache(None, **s3_client_kwargs)
     retrying = Retrying(
         wait=wait_random_exponential(multiplier=1, max=15),
-        stop=stop_after_delay(RETRY_STOP_AFTER_DELAY),
+        stop=stop_after_delay(UPLOAD_DOWNLOAD_RETRY_STOP_AFTER_DELAY),
         retry=retry_if_exception_type(RetryableError),
     )
     return retrying(
         _put_object,
         s3,
         body,
         parsed_s3_url.bucket,
@@ -527,40 +554,40 @@
     s3_client, body: Any, bucket: str, key: str, **s3_put_object_kwargs
 ) -> Dict[str, Any]:
     try:
         return s3_client.put_object(
             Body=body, Bucket=bucket, Key=key, **s3_put_object_kwargs
         )
     except ClientError as e:
-        if e.response["Error"]["Code"] in RETRYABLE_PUT_OBJECT_ERROR_CODES:
+        if e.response["Error"]["Code"] in BOTO_THROTTLING_ERROR_CODES:
             raise RetryableError(
                 f"Retry upload for: {bucket}/{key} after receiving {e.response['Error']['Code']}"
             ) from e
         raise NonRetryableError(f"Failed table upload to: {bucket}/{key}") from e
-    except NoCredentialsError as e:
+    except RETRYABLE_TRANSIENT_ERRORS as e:
         raise RetryableError(
-            f"Failed to fetch credentials when putting object into: {bucket}/{key}"
+            f"Retry upload for: {bucket}/{key} after receiving {type(e).__name__}"
         ) from e
     except BaseException as e:
         logger.error(
-            f"Upload has failed for {bucket}/{key}. Error: {e}",
+            f"Upload has failed for {bucket}/{key}. Error: {type(e).__name__}",
             exc_info=True,
         )
         raise NonRetryableError(f"Failed table upload to: {bucket}/{key}") from e
 
 
 def download(
     s3_url: str, fail_if_not_found: bool = True, **s3_client_kwargs
 ) -> Optional[Dict[str, Any]]:
 
     parsed_s3_url = parse_s3_url(s3_url)
     s3 = s3_client_cache(None, **s3_client_kwargs)
     retrying = Retrying(
         wait=wait_random_exponential(multiplier=1, max=15),
-        stop=stop_after_delay(RETRY_STOP_AFTER_DELAY),
+        stop=stop_after_delay(UPLOAD_DOWNLOAD_RETRY_STOP_AFTER_DELAY),
         retry=retry_if_exception_type(RetryableError),
     )
     return retrying(
         _get_object,
         s3,
         parsed_s3_url.bucket,
         parsed_s3_url.key,
@@ -577,17 +604,17 @@
     except ClientError as e:
         if e.response["Error"]["Code"] == "NoSuchKey":
             if fail_if_not_found:
                 raise NonRetryableError(
                     f"Failed get object from: {bucket}/{key}"
                 ) from e
             logger.info(f"file not found: {bucket}/{key}")
-    except NoCredentialsError as e:
+    except RETRYABLE_TRANSIENT_ERRORS as e:
         raise RetryableError(
-            f"Failed to fetch credentials when getting object from: {bucket}/{key}"
+            f"Retry get object: {bucket}/{key} after receiving {type(e).__name__}"
         ) from e
 
     return None
 
 
 def _download_manifest_entries_parallel(
     manifest: Manifest,
```

### Comparing `deltacat-1.1.6/deltacat/benchmarking/benchmark_parquet_reads.py` & `deltacat-1.1.7/deltacat/benchmarking/benchmark_parquet_reads.py`

 * *Files identical despite different names*

### Comparing `deltacat-1.1.6/deltacat/benchmarking/conftest.py` & `deltacat-1.1.7/deltacat/benchmarking/conftest.py`

 * *Files identical despite different names*

### Comparing `deltacat-1.1.6/deltacat/catalog/default_catalog_impl/__init__.py` & `deltacat-1.1.7/deltacat/catalog/default_catalog_impl/__init__.py`

 * *Files identical despite different names*

### Comparing `deltacat-1.1.6/deltacat/catalog/delegate.py` & `deltacat-1.1.7/deltacat/catalog/delegate.py`

 * *Files identical despite different names*

### Comparing `deltacat-1.1.6/deltacat/catalog/interface.py` & `deltacat-1.1.7/deltacat/catalog/interface.py`

 * *Files identical despite different names*

### Comparing `deltacat-1.1.6/deltacat/catalog/model/catalog.py` & `deltacat-1.1.7/deltacat/catalog/model/catalog.py`

 * *Files identical despite different names*

### Comparing `deltacat-1.1.6/deltacat/catalog/model/table_definition.py` & `deltacat-1.1.7/deltacat/catalog/model/table_definition.py`

 * *Files identical despite different names*

### Comparing `deltacat-1.1.6/deltacat/compute/compactor/__init__.py` & `deltacat-1.1.7/deltacat/compute/compactor/__init__.py`

 * *Files identical despite different names*

### Comparing `deltacat-1.1.6/deltacat/compute/compactor/compaction_session.py` & `deltacat-1.1.7/deltacat/compute/compactor/compaction_session.py`

 * *Files identical despite different names*

### Comparing `deltacat-1.1.6/deltacat/compute/compactor/model/compact_partition_params.py` & `deltacat-1.1.7/deltacat/compute/compactor/model/compact_partition_params.py`

 * *Files identical despite different names*

### Comparing `deltacat-1.1.6/deltacat/compute/compactor/model/compaction_session_audit_info.py` & `deltacat-1.1.7/deltacat/compute/compactor/model/compaction_session_audit_info.py`

 * *Files identical despite different names*

### Comparing `deltacat-1.1.6/deltacat/compute/compactor/model/delta_annotated.py` & `deltacat-1.1.7/deltacat/compute/compactor/model/delta_annotated.py`

 * *Files identical despite different names*

### Comparing `deltacat-1.1.6/deltacat/compute/compactor/model/delta_file_envelope.py` & `deltacat-1.1.7/deltacat/compute/compactor/model/delta_file_envelope.py`

 * *Files identical despite different names*

### Comparing `deltacat-1.1.6/deltacat/compute/compactor/model/delta_file_locator.py` & `deltacat-1.1.7/deltacat/compute/compactor/model/delta_file_locator.py`

 * *Files identical despite different names*

### Comparing `deltacat-1.1.6/deltacat/compute/compactor/model/materialize_result.py` & `deltacat-1.1.7/deltacat/compute/compactor/model/materialize_result.py`

 * *Files identical despite different names*

### Comparing `deltacat-1.1.6/deltacat/compute/compactor/model/primary_key_index.py` & `deltacat-1.1.7/deltacat/compute/compactor/model/primary_key_index.py`

 * *Files identical despite different names*

### Comparing `deltacat-1.1.6/deltacat/compute/compactor/model/pyarrow_write_result.py` & `deltacat-1.1.7/deltacat/compute/compactor/model/pyarrow_write_result.py`

 * *Files identical despite different names*

### Comparing `deltacat-1.1.6/deltacat/compute/compactor/model/round_completion_info.py` & `deltacat-1.1.7/deltacat/compute/compactor/model/round_completion_info.py`

 * *Files 3% similar despite different names*

```diff
@@ -124,7 +124,11 @@
     @property
     def input_inflation(self) -> Optional[float]:
         return self.get("inputInflation")
 
     @property
     def input_average_record_size_bytes(self) -> Optional[float]:
         return self.get("inputAverageRecordSizeBytes")
+
+    @staticmethod
+    def get_audit_bucket_name_and_key(compaction_audit_url: str) -> Tuple[str, str]:
+        return compaction_audit_url.replace("s3://", "").split("/", 1)
```

### Comparing `deltacat-1.1.6/deltacat/compute/compactor/model/table_object_store.py` & `deltacat-1.1.7/deltacat/compute/compactor/model/table_object_store.py`

 * *Files identical despite different names*

### Comparing `deltacat-1.1.6/deltacat/compute/compactor/repartition_session.py` & `deltacat-1.1.7/deltacat/compute/compactor/repartition_session.py`

 * *Files identical despite different names*

### Comparing `deltacat-1.1.6/deltacat/compute/compactor/steps/dedupe.py` & `deltacat-1.1.7/deltacat/compute/compactor/steps/dedupe.py`

 * *Files identical despite different names*

### Comparing `deltacat-1.1.6/deltacat/compute/compactor/steps/hash_bucket.py` & `deltacat-1.1.7/deltacat/compute/compactor/steps/hash_bucket.py`

 * *Files identical despite different names*

### Comparing `deltacat-1.1.6/deltacat/compute/compactor/steps/materialize.py` & `deltacat-1.1.7/deltacat/compute/compactor/steps/materialize.py`

 * *Files identical despite different names*

### Comparing `deltacat-1.1.6/deltacat/compute/compactor/steps/repartition.py` & `deltacat-1.1.7/deltacat/compute/compactor/steps/repartition.py`

 * *Files identical despite different names*

### Comparing `deltacat-1.1.6/deltacat/compute/compactor/utils/io.py` & `deltacat-1.1.7/deltacat/compute/compactor/utils/io.py`

 * *Files identical despite different names*

### Comparing `deltacat-1.1.6/deltacat/compute/compactor/utils/primary_key_index.py` & `deltacat-1.1.7/deltacat/compute/compactor/utils/primary_key_index.py`

 * *Files identical despite different names*

### Comparing `deltacat-1.1.6/deltacat/compute/compactor/utils/round_completion_file.py` & `deltacat-1.1.7/deltacat/compute/compactor/utils/round_completion_file.py`

 * *Files identical despite different names*

### Comparing `deltacat-1.1.6/deltacat/compute/compactor/utils/sort_key.py` & `deltacat-1.1.7/deltacat/compute/compactor/utils/sort_key.py`

 * *Files identical despite different names*

### Comparing `deltacat-1.1.6/deltacat/compute/compactor/utils/system_columns.py` & `deltacat-1.1.7/deltacat/compute/compactor/utils/system_columns.py`

 * *Files identical despite different names*

### Comparing `deltacat-1.1.6/deltacat/compute/compactor_v2/compaction_session.py` & `deltacat-1.1.7/deltacat/compute/compactor_v2/compaction_session.py`

 * *Files 2% similar despite different names*

```diff
@@ -20,14 +20,17 @@
 from deltacat.compute.compactor import (
     HighWatermark,
     PyArrowWriteResult,
     RoundCompletionInfo,
 )
 from deltacat.compute.compactor_v2.model.merge_result import MergeResult
 from deltacat.compute.compactor_v2.model.hash_bucket_result import HashBucketResult
+from deltacat.compute.compactor_v2.model.compaction_session import (
+    ExecutionCompactionResult,
+)
 from deltacat.compute.compactor.model.materialize_result import MaterializeResult
 from deltacat.compute.compactor_v2.utils.merge import (
     generate_local_merge_input,
 )
 from deltacat.compute.compactor import DeltaAnnotated
 from deltacat.compute.compactor_v2.utils.delta import contains_delete_deltas
 from deltacat.compute.compactor_v2.deletes.delete_strategy import (
@@ -37,31 +40,34 @@
     DeleteFileEnvelope,
 )
 from deltacat.compute.compactor_v2.deletes.utils import prepare_deletes
 
 from deltacat.storage import (
     Delta,
     DeltaLocator,
+    DeltaType,
     Manifest,
     Partition,
+    Stream,
+    StreamLocator,
 )
 from deltacat.compute.compactor.model.compact_partition_params import (
     CompactPartitionParams,
 )
 from deltacat.utils.ray_utils.concurrency import (
     invoke_parallel,
     task_resource_options_provider,
 )
 from deltacat.compute.compactor_v2.steps import merge as mg
 from deltacat.compute.compactor_v2.steps import hash_bucket as hb
 from deltacat.compute.compactor_v2.utils import io
 from deltacat.compute.compactor.utils import round_completion_file as rcf
 from deltacat.utils.metrics import metrics
 
-from typing import List, Optional, Tuple
+from typing import List, Optional
 from collections import defaultdict
 from deltacat.compute.compactor.model.compaction_session_audit_info import (
     CompactionSessionAuditInfo,
 )
 from deltacat.utils.resources import (
     get_current_process_peak_memory_usage_in_bytes,
 )
@@ -77,57 +83,74 @@
 
 
 logger = logs.configure_deltacat_logger(logging.getLogger(__name__))
 
 
 @metrics
 def compact_partition(params: CompactPartitionParams, **kwargs) -> Optional[str]:
-
     assert (
         params.hash_bucket_count is not None and params.hash_bucket_count >= 1
     ), "hash_bucket_count is a required arg for compactor v2"
 
     with memray.Tracker(
-        f"compaction_partition.bin"
+        "compaction_partition.bin"
     ) if params.enable_profiler else nullcontext():
-        (new_partition, new_rci, new_rcf_partition_locator,) = _execute_compaction(
+        execute_compaction_result: ExecutionCompactionResult = _execute_compaction(
             params,
             **kwargs,
         )
-
+        compaction_session_type: str = (
+            "INPLACE"
+            if execute_compaction_result.is_inplace_compacted
+            else "NON-INPLACE"
+        )
         logger.info(
             f"Partition-{params.source_partition_locator} -> "
-            f"Compaction session data processing completed"
+            f"{compaction_session_type} Compaction session data processing completed"
         )
-        round_completion_file_s3_url = None
-        if new_partition:
-            logger.info(f"Committing compacted partition to: {new_partition.locator}")
-            partition: Partition = params.deltacat_storage.commit_partition(
-                new_partition, **params.deltacat_storage_kwargs
+        round_completion_file_s3_url: Optional[str] = None
+        if execute_compaction_result.new_compacted_partition:
+            previous_partition: Optional[Partition] = None
+            if execute_compaction_result.is_inplace_compacted:
+                previous_partition: Optional[
+                    Partition
+                ] = params.deltacat_storage.get_partition(
+                    params.source_partition_locator.stream_locator,
+                    params.source_partition_locator.partition_values,
+                    **params.deltacat_storage_kwargs,
+                )
+                # NOTE: Retrieving the previous partition again as the partition_id may have changed by the time commit_partition is called.
+            logger.info(
+                f"Committing compacted partition to: {execute_compaction_result.new_compacted_partition.locator} "
+                f"using previous partition: {previous_partition.locator if previous_partition else None}"
             )
-            logger.info(f"Committed compacted partition: {partition}")
-
+            commited_partition: Partition = params.deltacat_storage.commit_partition(
+                execute_compaction_result.new_compacted_partition,
+                previous_partition,
+                **params.deltacat_storage_kwargs,
+            )
+            logger.info(f"Committed compacted partition: {commited_partition}")
             round_completion_file_s3_url = rcf.write_round_completion_file(
                 params.compaction_artifact_s3_bucket,
-                new_rcf_partition_locator,
-                new_rci,
+                execute_compaction_result.new_round_completion_file_partition_locator,
+                execute_compaction_result.new_round_completion_info,
                 **params.s3_client_kwargs,
             )
         else:
             logger.warning("No new partition was committed during compaction.")
 
         logger.info(
             f"Completed compaction session for: {params.source_partition_locator}"
         )
         return round_completion_file_s3_url
 
 
 def _execute_compaction(
     params: CompactPartitionParams, **kwargs
-) -> Tuple[Optional[Partition], Optional[RoundCompletionInfo], Optional[str]]:
+) -> ExecutionCompactionResult:
 
     rcf_source_partition_locator = (
         params.rebase_source_partition_locator or params.source_partition_locator
     )
 
     base_audit_url = rcf_source_partition_locator.path(
         f"s3://{params.compaction_artifact_s3_bucket}/compaction-audit"
@@ -138,15 +161,15 @@
         CompactionSessionAuditInfo(deltacat.__version__, ray.__version__, audit_url)
         .set_hash_bucket_count(params.hash_bucket_count)
         .set_compactor_version(CompactorVersion.V2.value)
     )
 
     compaction_start = time.monotonic()
 
-    task_max_parallelism = params.task_max_parallelism
+    task_max_parallelism: int = params.task_max_parallelism
 
     if params.pg_config:
         logger.info(
             "pg_config specified. Tasks will be scheduled in a placement group."
         )
         cluster_resources = params.pg_config.resource
         cluster_cpus = cluster_resources["CPU"]
@@ -201,27 +224,27 @@
         high_watermark,
         params.deltacat_storage,
         params.deltacat_storage_kwargs,
         params.list_deltas_kwargs,
     )
     if not input_deltas:
         logger.info("No input deltas found to compact.")
-        return None, None, None
+        return ExecutionCompactionResult(None, None, None, False)
 
     delete_strategy: Optional[DeleteStrategy] = None
     delete_file_envelopes: Optional[List[DeleteFileEnvelope]] = None
     delete_file_size_bytes: int = 0
     if contains_delete_deltas(input_deltas):
         input_deltas, delete_file_envelopes, delete_strategy = prepare_deletes(
             params, input_deltas
         )
         for delete_file_envelope in delete_file_envelopes:
             delete_file_size_bytes += delete_file_envelope.table_size_bytes
         logger.info(
-            f" Input deltas contain DELETE-type deltas. Total delete file size={delete_file_size_bytes}."
+            f" Input deltas contain {DeltaType.DELETE}-type deltas. Total delete file size={delete_file_size_bytes}."
             f" Total length of delete file envelopes={len(delete_file_envelopes)}"
         )
     uniform_deltas: List[DeltaAnnotated] = io.create_uniform_input_deltas(
         input_deltas=input_deltas,
         hash_bucket_count=params.hash_bucket_count,
         compaction_audit=compaction_audit,
         deltacat_storage=params.deltacat_storage,
@@ -243,22 +266,24 @@
     s3_utils.upload(
         compaction_audit.audit_url,
         str(json.dumps(compaction_audit)),
         **params.s3_client_kwargs,
     )
 
     # create a new stream for this round
-    compacted_stream_locator = params.destination_partition_locator.stream_locator
-    compacted_stream = params.deltacat_storage.get_stream(
+    compacted_stream_locator: Optional[
+        StreamLocator
+    ] = params.destination_partition_locator.stream_locator
+    compacted_stream: Stream = params.deltacat_storage.get_stream(
         compacted_stream_locator.namespace,
         compacted_stream_locator.table_name,
         compacted_stream_locator.table_version,
         **params.deltacat_storage_kwargs,
     )
-    compacted_partition = params.deltacat_storage.stage_partition(
+    compacted_partition: Partition = params.deltacat_storage.stage_partition(
         compacted_stream,
         params.destination_partition_locator.partition_values,
         **params.deltacat_storage_kwargs,
     )
 
     hb_options_provider = functools.partial(
         task_resource_options_provider,
@@ -528,28 +553,28 @@
         **params.s3_client_kwargs,
     )
 
     deltas = [m.delta for m in mat_results]
 
     # Note: An appropriate last stream position must be set
     # to avoid correctness issue.
-    merged_delta = Delta.merge_deltas(
+    merged_delta: Delta = Delta.merge_deltas(
         deltas,
         stream_position=params.last_stream_position_to_compact,
     )
 
     record_info_msg = (
         f"Hash bucket records: {total_hb_record_count},"
         f" Deduped records: {total_dd_record_count}, "
         f" Deleted records: {total_deleted_record_count}, "
         f" Materialized records: {merged_delta.meta.record_count}"
     )
     logger.info(record_info_msg)
 
-    compacted_delta = params.deltacat_storage.commit_delta(
+    compacted_delta: Delta = params.deltacat_storage.commit_delta(
         merged_delta,
         properties=kwargs.get("properties", {}),
         **params.deltacat_storage_kwargs,
     )
 
     logger.info(f"Committed compacted delta: {compacted_delta}")
 
@@ -649,12 +674,13 @@
     if is_inplace_compacted:
         logger.info(
             "Overriding round completion file source partition locator as in-place compacted. "
             + f"Got compacted partition partition_id of {compacted_partition.locator.partition_id} "
             f"and rcf source partition_id of {rcf_source_partition_locator.partition_id}."
         )
         rcf_source_partition_locator = compacted_partition.locator
-    return (
+    return ExecutionCompactionResult(
         compacted_partition,
         new_round_completion_info,
         rcf_source_partition_locator,
+        is_inplace_compacted,
     )
```

### Comparing `deltacat-1.1.6/deltacat/compute/compactor_v2/constants.py` & `deltacat-1.1.7/deltacat/compute/compactor_v2/constants.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,7 +1,9 @@
+from deltacat.utils.common import env_integer
+
 TOTAL_BYTES_IN_SHA1_HASH = 20
 
 PK_DELIMITER = "L6kl7u5f"
 
 MAX_RECORDS_PER_COMPACTED_FILE = 4_000_000
 
 # The maximum amount of delta bytes allowed in a batch.
@@ -37,14 +39,24 @@
 DROP_DUPLICATES = True
 
 # PARQUET to PYARROW inflation multiplier
 # This is the observed upper bound inflation for parquet
 # size in metadata to pyarrow table size.
 PARQUET_TO_PYARROW_INFLATION = 4
 
+# A merge task will fail after this timeout
+# The default is currently double the observed maximum.
+# This timeout depends on total data processed per task.
+MERGE_TASK_TIMEOUT_IN_SECONDS = env_integer("MERGE_TASK_TIMEOUT_IN_SECONDS", 25 * 60)
+
+# A hash bucket task will fail after this timeout
+HASH_BUCKET_TASK_TIMEOUT_IN_SECONDS = env_integer(
+    "HASH_BUCKET_TASK_TIMEOUT_IN_SECONDS", 25 * 60
+)
+
 # Metric Names
 # Time taken for a hash bucket task
 HASH_BUCKET_TIME_IN_SECONDS = "hash_bucket_time"
 
 # Hash bucket success count
 HASH_BUCKET_SUCCESS_COUNT = "hash_bucket_success_count"
```

### Comparing `deltacat-1.1.6/deltacat/compute/compactor_v2/deletes/delete_file_envelope.py` & `deltacat-1.1.7/deltacat/compute/compactor_v2/deletes/delete_file_envelope.py`

 * *Files identical despite different names*

### Comparing `deltacat-1.1.6/deltacat/compute/compactor_v2/deletes/delete_strategy.py` & `deltacat-1.1.7/deltacat/compute/compactor_v2/deletes/delete_strategy.py`

 * *Files identical despite different names*

### Comparing `deltacat-1.1.6/deltacat/compute/compactor_v2/deletes/delete_strategy_equality_delete.py` & `deltacat-1.1.7/deltacat/compute/compactor_v2/deletes/delete_strategy_equality_delete.py`

 * *Files identical despite different names*

### Comparing `deltacat-1.1.6/deltacat/compute/compactor_v2/deletes/model.py` & `deltacat-1.1.7/deltacat/compute/compactor_v2/deletes/model.py`

 * *Files identical despite different names*

### Comparing `deltacat-1.1.6/deltacat/compute/compactor_v2/deletes/utils.py` & `deltacat-1.1.7/deltacat/compute/compactor_v2/deletes/utils.py`

 * *Files identical despite different names*

### Comparing `deltacat-1.1.6/deltacat/compute/compactor_v2/model/hash_bucket_input.py` & `deltacat-1.1.7/deltacat/compute/compactor_v2/model/hash_bucket_input.py`

 * *Files identical despite different names*

### Comparing `deltacat-1.1.6/deltacat/compute/compactor_v2/model/merge_file_group.py` & `deltacat-1.1.7/deltacat/compute/compactor_v2/model/merge_file_group.py`

 * *Files identical despite different names*

### Comparing `deltacat-1.1.6/deltacat/compute/compactor_v2/model/merge_input.py` & `deltacat-1.1.7/deltacat/compute/compactor_v2/model/merge_input.py`

 * *Files identical despite different names*

### Comparing `deltacat-1.1.6/deltacat/compute/compactor_v2/steps/hash_bucket.py` & `deltacat-1.1.7/deltacat/compute/compactor_v2/steps/hash_bucket.py`

 * *Files 3% similar despite different names*

```diff
@@ -25,20 +25,22 @@
 )
 from deltacat.utils.common import ReadKwargsProvider
 from deltacat.utils.performance import timed_invocation
 from deltacat.utils.metrics import emit_timer_metrics, failure_metric, success_metric
 from deltacat.utils.resources import (
     get_current_process_peak_memory_usage_in_bytes,
     ProcessUtilizationOverTimeRange,
+    timeout,
 )
 from deltacat.constants import BYTES_PER_GIBIBYTE
 from deltacat.compute.compactor_v2.constants import (
     HASH_BUCKET_TIME_IN_SECONDS,
     HASH_BUCKET_FAILURE_COUNT,
     HASH_BUCKET_SUCCESS_COUNT,
+    HASH_BUCKET_TASK_TIMEOUT_IN_SECONDS,
 )
 
 if importlib.util.find_spec("memray"):
     import memray
 
 logger = logs.configure_deltacat_logger(logging.getLogger(__name__))
 
@@ -92,16 +94,20 @@
                         delta_type=dfe.delta_type,
                         table=table,
                     )
                 )
     return hb_to_delta_file_envelopes, total_record_count, total_size_bytes
 
 
+# TODO: use timeout parameter in ray.remote
+# https://github.com/ray-project/ray/issues/18916
+# Note: order of decorators is important
 @success_metric(name=HASH_BUCKET_SUCCESS_COUNT)
 @failure_metric(name=HASH_BUCKET_FAILURE_COUNT)
+@timeout(HASH_BUCKET_TASK_TIMEOUT_IN_SECONDS)
 def _timed_hash_bucket(input: HashBucketInput):
     task_id = get_current_ray_task_id()
     worker_id = get_current_ray_worker_id()
     with memray.Tracker(
         f"hash_bucket_{worker_id}_{task_id}.bin"
     ) if input.enable_profiler else nullcontext():
         (
```

### Comparing `deltacat-1.1.6/deltacat/compute/compactor_v2/steps/merge.py` & `deltacat-1.1.7/deltacat/compute/compactor_v2/steps/merge.py`

 * *Files 2% similar despite different names*

```diff
@@ -24,14 +24,15 @@
 )
 from deltacat.compute.compactor.utils import system_columns as sc
 from deltacat.utils.performance import timed_invocation
 from deltacat.utils.metrics import emit_timer_metrics, failure_metric, success_metric
 from deltacat.utils.resources import (
     get_current_process_peak_memory_usage_in_bytes,
     ProcessUtilizationOverTimeRange,
+    timeout,
 )
 from deltacat.compute.compactor_v2.utils.primary_key_index import (
     generate_pk_hash_column,
 )
 from deltacat.storage import (
     Delta,
     DeltaLocator,
@@ -42,14 +43,15 @@
 )
 from deltacat.compute.compactor_v2.utils.dedupe import drop_duplicates
 from deltacat.constants import BYTES_PER_GIBIBYTE
 from deltacat.compute.compactor_v2.constants import (
     MERGE_TIME_IN_SECONDS,
     MERGE_SUCCESS_COUNT,
     MERGE_FAILURE_COUNT,
+    MERGE_TASK_TIMEOUT_IN_SECONDS,
 )
 
 
 if importlib.util.find_spec("memray"):
     import memray
 
 logger = logs.configure_deltacat_logger(logging.getLogger(__name__))
@@ -480,16 +482,20 @@
             f"Copying {len(referenced_materialized_results)} manifest files by reference..."
         )
         materialized_results.extend(referenced_materialized_results)
 
     return materialized_results
 
 
+# TODO: use timeout parameter in ray.remote
+# https://github.com/ray-project/ray/issues/18916
+# Note: order of decorators is important
 @success_metric(name=MERGE_SUCCESS_COUNT)
 @failure_metric(name=MERGE_FAILURE_COUNT)
+@timeout(MERGE_TASK_TIMEOUT_IN_SECONDS)
 def _timed_merge(input: MergeInput) -> MergeResult:
     task_id = get_current_ray_task_id()
     worker_id = get_current_ray_worker_id()
     with memray.Tracker(
         f"merge_{worker_id}_{task_id}.bin"
     ) if input.enable_profiler else nullcontext():
         total_input_records, total_deduped_records = 0, 0
```

### Comparing `deltacat-1.1.6/deltacat/compute/compactor_v2/utils/content_type_params.py` & `deltacat-1.1.7/deltacat/compute/compactor_v2/utils/content_type_params.py`

 * *Files identical despite different names*

### Comparing `deltacat-1.1.6/deltacat/compute/compactor_v2/utils/dedupe.py` & `deltacat-1.1.7/deltacat/compute/compactor_v2/utils/dedupe.py`

 * *Files identical despite different names*

### Comparing `deltacat-1.1.6/deltacat/compute/compactor_v2/utils/delta.py` & `deltacat-1.1.7/deltacat/compute/compactor_v2/utils/delta.py`

 * *Files identical despite different names*

### Comparing `deltacat-1.1.6/deltacat/compute/compactor_v2/utils/io.py` & `deltacat-1.1.7/deltacat/compute/compactor_v2/utils/io.py`

 * *Files identical despite different names*

### Comparing `deltacat-1.1.6/deltacat/compute/compactor_v2/utils/merge.py` & `deltacat-1.1.7/deltacat/compute/compactor_v2/utils/merge.py`

 * *Files identical despite different names*

### Comparing `deltacat-1.1.6/deltacat/compute/compactor_v2/utils/primary_key_index.py` & `deltacat-1.1.7/deltacat/compute/compactor_v2/utils/primary_key_index.py`

 * *Files identical despite different names*

### Comparing `deltacat-1.1.6/deltacat/compute/compactor_v2/utils/task_options.py` & `deltacat-1.1.7/deltacat/compute/compactor_v2/utils/task_options.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,9 +1,10 @@
 import botocore
 import logging
+import tenacity
 from typing import Dict, Optional, List, Tuple, Any
 from deltacat import logs
 from deltacat.compute.compactor_v2.model.merge_file_group import (
     LocalMergeFileGroupsProvider,
 )
 from deltacat.types.media import ContentEncoding, ContentType
 from deltacat.types.partial_download import PartialParquetParameters
@@ -62,15 +63,16 @@
 
 def get_task_options(
     cpu: float, memory: float, ray_custom_resources: Optional[Dict] = None
 ) -> Dict:
 
     # NOTE: With DEFAULT scheduling strategy in Ray 2.20.0, autoscaler does
     # not spin up enough nodes fast and hence we see only approximately
-    # 20 tasks get scheduled out of 100 tasks in queue.
+    # 20 tasks get scheduled out of 100 tasks in queue. Hence, we use SPREAD
+    # which is also ideal for merge and hash bucket tasks.
     # https://docs.ray.io/en/latest/ray-core/scheduling/index.html
     task_opts = {"num_cpus": cpu, "memory": memory, "scheduling_strategy": "SPREAD"}
 
     if ray_custom_resources:
         task_opts["resources"] = ray_custom_resources
 
     task_opts["max_retries"] = 3
@@ -79,14 +81,15 @@
     # https://github.com/boto/botocore/blob/develop/botocore/exceptions.py
     task_opts["retry_exceptions"] = [
         botocore.exceptions.ConnectionError,
         botocore.exceptions.HTTPClientError,
         ConnectionError,
         TimeoutError,
         DaftTransientError,
+        tenacity.RetryError,
     ]
 
     return task_opts
 
 
 def estimate_manifest_entry_size_bytes(
     entry: ManifestEntry, previous_inflation: float, **kwargs
```

### Comparing `deltacat-1.1.6/deltacat/compute/merge_on_read/daft.py` & `deltacat-1.1.7/deltacat/compute/merge_on_read/daft.py`

 * *Files identical despite different names*

### Comparing `deltacat-1.1.6/deltacat/compute/merge_on_read/model/merge_on_read_params.py` & `deltacat-1.1.7/deltacat/compute/merge_on_read/model/merge_on_read_params.py`

 * *Files identical despite different names*

### Comparing `deltacat-1.1.6/deltacat/compute/merge_on_read/utils/delta.py` & `deltacat-1.1.7/deltacat/compute/merge_on_read/utils/delta.py`

 * *Files identical despite different names*

### Comparing `deltacat-1.1.6/deltacat/compute/metastats/meta_stats.py` & `deltacat-1.1.7/deltacat/compute/metastats/meta_stats.py`

 * *Files identical despite different names*

### Comparing `deltacat-1.1.6/deltacat/compute/metastats/model/partition_stats_dict.py` & `deltacat-1.1.7/deltacat/compute/metastats/model/partition_stats_dict.py`

 * *Files identical despite different names*

### Comparing `deltacat-1.1.6/deltacat/compute/metastats/model/stats_cluster_size_estimator.py` & `deltacat-1.1.7/deltacat/compute/metastats/model/stats_cluster_size_estimator.py`

 * *Files identical despite different names*

### Comparing `deltacat-1.1.6/deltacat/compute/metastats/stats.py` & `deltacat-1.1.7/deltacat/compute/metastats/stats.py`

 * *Files identical despite different names*

### Comparing `deltacat-1.1.6/deltacat/compute/metastats/utils/constants.py` & `deltacat-1.1.7/deltacat/compute/metastats/utils/constants.py`

 * *Files identical despite different names*

### Comparing `deltacat-1.1.6/deltacat/compute/metastats/utils/io.py` & `deltacat-1.1.7/deltacat/compute/metastats/utils/io.py`

 * *Files identical despite different names*

### Comparing `deltacat-1.1.6/deltacat/compute/metastats/utils/pyarrow_memory_estimation_function.py` & `deltacat-1.1.7/deltacat/compute/metastats/utils/pyarrow_memory_estimation_function.py`

 * *Files identical despite different names*

### Comparing `deltacat-1.1.6/deltacat/compute/metastats/utils/ray_utils.py` & `deltacat-1.1.7/deltacat/compute/metastats/utils/ray_utils.py`

 * *Files identical despite different names*

### Comparing `deltacat-1.1.6/deltacat/compute/stats/basic.py` & `deltacat-1.1.7/deltacat/compute/stats/basic.py`

 * *Files identical despite different names*

### Comparing `deltacat-1.1.6/deltacat/compute/stats/models/delta_column_stats.py` & `deltacat-1.1.7/deltacat/compute/stats/models/delta_column_stats.py`

 * *Files identical despite different names*

### Comparing `deltacat-1.1.6/deltacat/compute/stats/models/delta_stats.py` & `deltacat-1.1.7/deltacat/compute/stats/models/delta_stats.py`

 * *Files identical despite different names*

### Comparing `deltacat-1.1.6/deltacat/compute/stats/models/delta_stats_cache_result.py` & `deltacat-1.1.7/deltacat/compute/stats/models/delta_stats_cache_result.py`

 * *Files identical despite different names*

### Comparing `deltacat-1.1.6/deltacat/compute/stats/models/manifest_entry_stats.py` & `deltacat-1.1.7/deltacat/compute/stats/models/manifest_entry_stats.py`

 * *Files identical despite different names*

### Comparing `deltacat-1.1.6/deltacat/compute/stats/models/stats_result.py` & `deltacat-1.1.7/deltacat/compute/stats/models/stats_result.py`

 * *Files identical despite different names*

### Comparing `deltacat-1.1.6/deltacat/compute/stats/utils/intervals.py` & `deltacat-1.1.7/deltacat/compute/stats/utils/intervals.py`

 * *Files identical despite different names*

### Comparing `deltacat-1.1.6/deltacat/compute/stats/utils/io.py` & `deltacat-1.1.7/deltacat/compute/stats/utils/io.py`

 * *Files identical despite different names*

### Comparing `deltacat-1.1.6/deltacat/compute/stats/utils/manifest_stats_file.py` & `deltacat-1.1.7/deltacat/compute/stats/utils/manifest_stats_file.py`

 * *Files identical despite different names*

### Comparing `deltacat-1.1.6/deltacat/constants.py` & `deltacat-1.1.7/deltacat/constants.py`

 * *Files identical despite different names*

### Comparing `deltacat-1.1.6/deltacat/io/aws/redshift/redshift_datasource.py` & `deltacat-1.1.7/deltacat/io/aws/redshift/redshift_datasource.py`

 * *Files identical despite different names*

### Comparing `deltacat-1.1.6/deltacat/io/dataset.py` & `deltacat-1.1.7/deltacat/io/dataset.py`

 * *Files identical despite different names*

### Comparing `deltacat-1.1.6/deltacat/io/file_object_store.py` & `deltacat-1.1.7/deltacat/io/file_object_store.py`

 * *Files identical despite different names*

### Comparing `deltacat-1.1.6/deltacat/io/memcached_object_store.py` & `deltacat-1.1.7/deltacat/io/memcached_object_store.py`

 * *Files identical despite different names*

### Comparing `deltacat-1.1.6/deltacat/io/object_store.py` & `deltacat-1.1.7/deltacat/io/object_store.py`

 * *Files identical despite different names*

### Comparing `deltacat-1.1.6/deltacat/io/ray_plasma_object_store.py` & `deltacat-1.1.7/deltacat/io/ray_plasma_object_store.py`

 * *Files identical despite different names*

### Comparing `deltacat-1.1.6/deltacat/io/read_api.py` & `deltacat-1.1.7/deltacat/io/read_api.py`

 * *Files identical despite different names*

### Comparing `deltacat-1.1.6/deltacat/io/redis_object_store.py` & `deltacat-1.1.7/deltacat/io/redis_object_store.py`

 * *Files identical despite different names*

### Comparing `deltacat-1.1.6/deltacat/io/s3_object_store.py` & `deltacat-1.1.7/deltacat/io/s3_object_store.py`

 * *Files identical despite different names*

### Comparing `deltacat-1.1.6/deltacat/logs.py` & `deltacat-1.1.7/deltacat/logs.py`

 * *Files identical despite different names*

### Comparing `deltacat-1.1.6/deltacat/storage/__init__.py` & `deltacat-1.1.7/deltacat/storage/__init__.py`

 * *Files identical despite different names*

### Comparing `deltacat-1.1.6/deltacat/storage/interface.py` & `deltacat-1.1.7/deltacat/storage/interface.py`

 * *Files 1% similar despite different names*

```diff
@@ -410,19 +410,26 @@
     with the same partition values, then it will have its previous partition ID
     set to the ID of the partition being replaced. Partition keys should not be
     specified for unpartitioned tables.
     """
     raise NotImplementedError("stage_partition not implemented")
 
 
-def commit_partition(partition: Partition, *args, **kwargs) -> Partition:
+def commit_partition(
+    partition: Partition,
+    previous_partition: Optional[Partition] = None,
+    *args,
+    **kwargs
+) -> Partition:
     """
     Commits the given partition to its associated table version stream,
-    replacing any previous partition registered for the same stream and
-    partition values. Returns the registered partition. If the partition's
+    replacing any previous partition (i.e., "partition being replaced") registered for the same stream and
+    partition values.
+    If the previous_partition is passed as an argument, the specified previous_partition will be the partition being replaced, otherwise it will be retrieved.
+    Returns the registered partition. If the partition's
     previous delta stream position is specified, then the commit will
     be rejected if it does not match the actual previous stream position of
     the partition being replaced. If the partition's previous partition ID is
     specified, then the commit will be rejected if it does not match the actual
     ID of the partition being replaced.
     """
     raise NotImplementedError("commit_partition not implemented")
```

### Comparing `deltacat-1.1.6/deltacat/storage/model/delete_parameters.py` & `deltacat-1.1.7/deltacat/storage/model/delete_parameters.py`

 * *Files identical despite different names*

### Comparing `deltacat-1.1.6/deltacat/storage/model/delta.py` & `deltacat-1.1.7/deltacat/storage/model/delta.py`

 * *Files identical despite different names*

### Comparing `deltacat-1.1.6/deltacat/storage/model/list_result.py` & `deltacat-1.1.7/deltacat/storage/model/list_result.py`

 * *Files identical despite different names*

### Comparing `deltacat-1.1.6/deltacat/storage/model/locator.py` & `deltacat-1.1.7/deltacat/storage/model/locator.py`

 * *Files identical despite different names*

### Comparing `deltacat-1.1.6/deltacat/storage/model/namespace.py` & `deltacat-1.1.7/deltacat/storage/model/namespace.py`

 * *Files identical despite different names*

### Comparing `deltacat-1.1.6/deltacat/storage/model/partition.py` & `deltacat-1.1.7/deltacat/storage/model/partition.py`

 * *Files identical despite different names*

### Comparing `deltacat-1.1.6/deltacat/storage/model/sort_key.py` & `deltacat-1.1.7/deltacat/storage/model/sort_key.py`

 * *Files identical despite different names*

### Comparing `deltacat-1.1.6/deltacat/storage/model/stream.py` & `deltacat-1.1.7/deltacat/storage/model/stream.py`

 * *Files identical despite different names*

### Comparing `deltacat-1.1.6/deltacat/storage/model/table.py` & `deltacat-1.1.7/deltacat/storage/model/table.py`

 * *Files identical despite different names*

### Comparing `deltacat-1.1.6/deltacat/storage/model/table_version.py` & `deltacat-1.1.7/deltacat/storage/model/table_version.py`

 * *Files identical despite different names*

### Comparing `deltacat-1.1.6/deltacat/storage/model/types.py` & `deltacat-1.1.7/deltacat/storage/model/types.py`

 * *Files identical despite different names*

### Comparing `deltacat-1.1.6/deltacat/tests/aws/test_clients.py` & `deltacat-1.1.7/deltacat/tests/aws/test_clients.py`

 * *Files identical despite different names*

### Comparing `deltacat-1.1.6/deltacat/tests/aws/test_s3u.py` & `deltacat-1.1.7/deltacat/tests/aws/test_s3u.py`

 * *Files 26% similar despite different names*

```diff
@@ -1,19 +1,29 @@
 import unittest
+
+import botocore
+
+from deltacat.aws.constants import RETRYABLE_TRANSIENT_ERRORS
 from deltacat.aws.s3u import UuidBlockWritePathProvider, CapturedBlockWritePaths
 
 
 import os
 from unittest import mock
 from unittest.mock import patch
 
 import boto3
 import pytest
 from boto3.resources.base import ServiceResource
-from botocore.exceptions import ClientError, NoCredentialsError
+from botocore.exceptions import (
+    ClientError,
+    NoCredentialsError,
+    ReadTimeoutError,
+    ConnectTimeoutError,
+    HTTPClientError,
+)
 from deltacat.exceptions import NonRetryableError
 from moto import mock_s3
 from tenacity import RetryError
 
 from deltacat.aws import s3u
 
 
@@ -60,15 +70,15 @@
         assert uploaded_file is not None
         assert uploaded_file["ResponseMetadata"]["HTTPStatusCode"] == 200
         downloaded_file = s3u.download(uri)
         downloaded_body = downloaded_file["Body"].read().decode("utf-8")
         assert downloaded_file["ResponseMetadata"]["HTTPStatusCode"] == 200
         assert downloaded_body == body
 
-    @patch("deltacat.aws.s3u.RETRY_STOP_AFTER_DELAY", 1)
+    @patch("deltacat.aws.s3u.UPLOAD_DOWNLOAD_RETRY_STOP_AFTER_DELAY", 1)
     @patch("deltacat.aws.s3u.s3_client_cache")
     def test_upload_throttled(self, mock_s3_client_cache):
         uri = f"s3://{self.TEST_S3_BUCKET_NAME}/{self.TEST_S3_KEY}"
         body = "test-body"
         throttling_err = ClientError({"Error": {"Code": "Throttling"}}, "put_object")
         mock_s3_client_cache.return_value = mock_s3 = mock.MagicMock()
         mock_s3.put_object.side_effect = throttling_err
@@ -83,28 +93,73 @@
         no_credentials_err = NoCredentialsError()
         mock_s3.put_object.side_effect = no_credentials_err
         with pytest.raises(RetryError):
             s3u.upload(uri, body)
 
         assert mock_s3.put_object.call_count > 3
 
+    @patch("deltacat.aws.s3u.UPLOAD_SLICED_TABLE_RETRY_STOP_AFTER_DELAY", 1)
+    @patch("deltacat.aws.s3u.ManifestEntry")
+    @patch("deltacat.aws.s3u._get_metadata")
+    @patch("deltacat.aws.s3u.CapturedBlockWritePaths")
+    def test_upload_sliced_table_retry(
+        self,
+        mock_captured_block_write_paths,
+        mock_get_metadata,
+        mock_manifest_entry,
+    ):
+        mock_manifest_entry.from_s3_obj_url.side_effect = OSError(
+            "Please reduce your request rate.."
+        )
+        mock_get_metadata.return_value = [mock.MagicMock()]
+        cbwp = CapturedBlockWritePaths()
+        cbwp._write_paths = ["s3_write_path"]
+        cbwp._block_refs = [mock.MagicMock()]
+        mock_captured_block_write_paths.return_value = cbwp
+        with pytest.raises(RetryError):
+            s3u.upload_sliced_table(
+                mock.MagicMock(),
+                "s3-prefix",
+                mock.MagicMock(),
+                mock.MagicMock(),
+                mock.MagicMock(),
+                mock.MagicMock(),
+            )
+
+    @patch("deltacat.aws.s3u.UPLOAD_DOWNLOAD_RETRY_STOP_AFTER_DELAY", 1)
+    @patch("deltacat.aws.s3u.s3_client_cache")
+    def test_upload_transient_error_retry(self, mock_s3_client_cache):
+        uri = f"s3://{self.TEST_S3_BUCKET_NAME}/{self.TEST_S3_KEY}"
+        body = "test-body"
+        transient_errors = [*RETRYABLE_TRANSIENT_ERRORS]
+        mock_s3_client_cache.return_value = mock_s3 = mock.MagicMock()
+
+        while transient_errors:
+            err_cls = transient_errors.pop()
+            err_obj = self._populate_error_by_type(err_cls)
+            mock_s3.put_object.side_effect = err_obj
+            with pytest.raises(RetryError):
+                s3u.upload(uri, body)
+
+        assert mock_s3.put_object.call_count > len(RETRYABLE_TRANSIENT_ERRORS)
+
     @patch("deltacat.aws.s3u.s3_client_cache")
     def test_upload_unexpected_error_code(self, mock_s3_client_cache):
         uri = f"s3://{self.TEST_S3_BUCKET_NAME}/{self.TEST_S3_KEY}"
         body = "test-body"
         err = ClientError({"Error": {"Code": "UnexpectedError"}}, "put_object")
         mock_s3_client_cache.return_value = mock_s3 = mock.MagicMock()
         mock_s3.put_object.side_effect = err
         file = None
         with pytest.raises(NonRetryableError):
             s3u.upload(uri, body)
         assert file is None
         assert mock_s3.put_object.call_count == 1
 
-    @patch("deltacat.aws.s3u.RETRY_STOP_AFTER_DELAY", 1)
+    @patch("deltacat.aws.s3u.UPLOAD_DOWNLOAD_RETRY_STOP_AFTER_DELAY", 1)
     @patch("deltacat.aws.s3u.s3_client_cache")
     def test_download_throttled(self, mock_s3_client_cache):
         uri = f"s3://{self.TEST_S3_BUCKET_NAME}/{self.TEST_S3_KEY}"
         no_credentials_err = NoCredentialsError()
         mock_s3_client_cache.return_value = mock_s3 = mock.MagicMock()
         mock_s3.get_object.side_effect = no_credentials_err
         file = None
@@ -118,7 +173,33 @@
         file = None
         with pytest.raises(NonRetryableError):
             file = s3u.download(uri)
         assert file is None
 
         file = s3u.download(uri, fail_if_not_found=False)
         assert file is None
+
+    @patch("deltacat.aws.s3u.UPLOAD_DOWNLOAD_RETRY_STOP_AFTER_DELAY", 1)
+    @patch("deltacat.aws.s3u.s3_client_cache")
+    def test_download_transient_error_retry(self, mock_s3_client_cache):
+        uri = f"s3://{self.TEST_S3_BUCKET_NAME}/{self.TEST_S3_KEY}"
+        transient_errors = [*RETRYABLE_TRANSIENT_ERRORS]
+        mock_s3_client_cache.return_value = mock_s3 = mock.MagicMock()
+
+        while transient_errors:
+            err_cls = transient_errors.pop()
+            err_obj = self._populate_error_by_type(err_cls)
+            mock_s3.get_object.side_effect = err_obj
+            with pytest.raises(RetryError):
+                s3u.download(uri)
+
+        assert mock_s3.get_object.call_count > len(RETRYABLE_TRANSIENT_ERRORS)
+
+    @staticmethod
+    def _populate_error_by_type(err_cls):
+        if err_cls in (ReadTimeoutError, ConnectTimeoutError):
+            err_obj = err_cls(endpoint_url="127.0.0.1")
+        elif err_cls in (HTTPClientError, botocore.exceptions.ConnectionError):
+            err_obj = err_cls(endpoint_url="127.0.0.1", error=Exception)
+        else:
+            err_obj = err_cls()
+        return err_obj
```

### Comparing `deltacat-1.1.6/deltacat/tests/catalog/test_default_catalog_impl.py` & `deltacat-1.1.7/deltacat/tests/catalog/test_default_catalog_impl.py`

 * *Files 2% similar despite different names*

```diff
@@ -32,14 +32,16 @@
         cls.deltacat_storage_kwargs = {ds.DB_FILE_PATH_ARG: cls.DB_FILE_PATH}
 
         super().setUpClass()
 
     @classmethod
     def doClassCleanups(cls) -> None:
         os.remove(cls.DB_FILE_PATH)
+        ray.shutdown()
+        super().tearDownClass()
 
     def test_daft_distributed_read_sanity(self):
         # setup
         READ_TABLE_TABLE_NAME = "test_read_table"
         create_delta_from_csv_file(
             self.READ_TABLE_NAMESPACE,
             [self.SAMPLE_FILE_PATH],
```

### Comparing `deltacat-1.1.6/deltacat/tests/compute/compact_partition_rebase_then_incremental_test_cases.py` & `deltacat-1.1.7/deltacat/tests/compute/compact_partition_rebase_then_incremental_test_cases.py`

 * *Files identical despite different names*

### Comparing `deltacat-1.1.6/deltacat/tests/compute/compact_partition_test_cases.py` & `deltacat-1.1.7/deltacat/tests/compute/compact_partition_test_cases.py`

 * *Files 2% similar despite different names*

```diff
@@ -18,14 +18,15 @@
 
 from deltacat.storage import (
     DeltaType,
 )
 from deltacat.compute.compactor_v2.compaction_session import (
     compact_partition as compact_partition_v2,
 )
+from deltacat.storage import DeleteParameters
 
 from deltacat.compute.compactor.model.compactor_version import CompactorVersion
 
 from deltacat.storage.model.sort_key import SortKey
 
 ZERO_VALUED_SORT_KEY, ZERO_VALUED_PARTITION_VALUES_PARAM = [], []
 ZERO_VALUED_PARTITION_KEYS_PARAM = None
@@ -85,17 +86,21 @@
 
 
 @dataclass(frozen=True)
 class IncrementalCompactionTestCaseParams(BaseCompactorTestCase):
     """
     Args:
         is_inplace: bool - argument to indicate whether to try compacting an in-place compacted table (the source table is the destination table). Also needed to control whether the destination table is created
+        add_late_deltas: List[Tuple[pa.Table, DeltaType]] - argument to indicate whether to add deltas to the source_partition after we've triggered compaction
     """
 
     is_inplace: bool
+    add_late_deltas: Optional[
+        List[Tuple[pa.Table, DeltaType, Optional[DeleteParameters]]]
+    ]
 
 
 @dataclass(frozen=True)
 class NoRCFOutputCompactionTestCaseParams(BaseCompactorTestCase):
     pass
 
 
@@ -144,14 +149,15 @@
         expected_terminal_exception_message=None,
         do_create_placement_group=False,
         records_per_compacted_file=DEFAULT_MAX_RECORDS_PER_FILE,
         hash_bucket_count=DEFAULT_HASH_BUCKET_COUNT,
         read_kwargs_provider=None,
         drop_duplicates=True,
         is_inplace=False,
+        add_late_deltas=None,
         skip_enabled_compact_partition_drivers=None,
     ),
     "2-incremental-pkstr-skstr-norcf": IncrementalCompactionTestCaseParams(
         primary_keys={"pk_col_1"},
         sort_keys=ZERO_VALUED_SORT_KEY,
         partition_keys=[PartitionKey.of("region_id", PartitionKeyType.INT)],
         partition_values=["1"],
@@ -171,14 +177,15 @@
         expected_terminal_exception_message=None,
         do_create_placement_group=False,
         records_per_compacted_file=DEFAULT_MAX_RECORDS_PER_FILE,
         hash_bucket_count=DEFAULT_HASH_BUCKET_COUNT,
         read_kwargs_provider=None,
         drop_duplicates=True,
         is_inplace=False,
+        add_late_deltas=None,
         skip_enabled_compact_partition_drivers=None,
     ),
     "3-incremental-pkstr-multiskstr-norcf": IncrementalCompactionTestCaseParams(
         primary_keys={"pk_col_1"},
         sort_keys=[
             SortKey.of(key_name="sk_col_1"),
             SortKey.of(key_name="sk_col_2"),
@@ -207,14 +214,15 @@
         expected_terminal_exception_message=None,
         do_create_placement_group=False,
         records_per_compacted_file=DEFAULT_MAX_RECORDS_PER_FILE,
         hash_bucket_count=DEFAULT_HASH_BUCKET_COUNT,
         read_kwargs_provider=None,
         drop_duplicates=True,
         is_inplace=False,
+        add_late_deltas=None,
         skip_enabled_compact_partition_drivers=None,
     ),
     "4-incremental-duplicate-pk": IncrementalCompactionTestCaseParams(
         primary_keys={"pk_col_1"},
         sort_keys=[
             SortKey.of(key_name="sk_col_1"),
             SortKey.of(key_name="sk_col_2"),
@@ -242,14 +250,15 @@
         expected_terminal_exception_message=None,
         do_create_placement_group=False,
         records_per_compacted_file=DEFAULT_MAX_RECORDS_PER_FILE,
         hash_bucket_count=DEFAULT_HASH_BUCKET_COUNT,
         read_kwargs_provider=None,
         drop_duplicates=True,
         is_inplace=False,
+        add_late_deltas=None,
         skip_enabled_compact_partition_drivers=None,
     ),
     "5-incremental-decimal-pk-simple": IncrementalCompactionTestCaseParams(
         primary_keys={"pk_col_1"},
         sort_keys=[SortKey.of(key_name="sk_col_1")],
         partition_keys=[PartitionKey.of("region_id", PartitionKeyType.INT)],
         partition_values=["1"],
@@ -272,14 +281,15 @@
         expected_terminal_exception_message=None,
         do_create_placement_group=False,
         records_per_compacted_file=DEFAULT_MAX_RECORDS_PER_FILE,
         hash_bucket_count=DEFAULT_HASH_BUCKET_COUNT,
         read_kwargs_provider=None,
         drop_duplicates=True,
         is_inplace=False,
+        add_late_deltas=None,
         skip_enabled_compact_partition_drivers=None,
     ),
     "6-incremental-integer-pk-simple": IncrementalCompactionTestCaseParams(
         primary_keys={"pk_col_1"},
         sort_keys=[SortKey.of(key_name="sk_col_1")],
         partition_keys=[PartitionKey.of("region_id", PartitionKeyType.INT)],
         partition_values=["1"],
@@ -302,14 +312,15 @@
         expected_terminal_exception_message=None,
         do_create_placement_group=False,
         records_per_compacted_file=DEFAULT_MAX_RECORDS_PER_FILE,
         hash_bucket_count=DEFAULT_HASH_BUCKET_COUNT,
         read_kwargs_provider=None,
         drop_duplicates=True,
         is_inplace=False,
+        add_late_deltas=None,
         skip_enabled_compact_partition_drivers=None,
     ),
     "7-incremental-timestamp-pk-simple": IncrementalCompactionTestCaseParams(
         primary_keys={"pk_col_1"},
         sort_keys=[SortKey.of(key_name="sk_col_1")],
         partition_keys=[PartitionKey.of("region_id", PartitionKeyType.INT)],
         partition_values=["1"],
@@ -332,14 +343,15 @@
         expected_terminal_exception_message=None,
         do_create_placement_group=False,
         records_per_compacted_file=DEFAULT_MAX_RECORDS_PER_FILE,
         hash_bucket_count=DEFAULT_HASH_BUCKET_COUNT,
         read_kwargs_provider=None,
         drop_duplicates=True,
         is_inplace=False,
+        add_late_deltas=None,
         skip_enabled_compact_partition_drivers=None,
     ),
     "8-incremental-decimal-timestamp-pk-multi": IncrementalCompactionTestCaseParams(
         primary_keys={"pk_col_1", "pk_col_2"},
         sort_keys=[SortKey.of(key_name="sk_col_1")],
         partition_keys=[PartitionKey.of("region_id", PartitionKeyType.INT)],
         partition_values=["1"],
@@ -364,14 +376,15 @@
         expected_terminal_exception_message=None,
         do_create_placement_group=False,
         records_per_compacted_file=DEFAULT_MAX_RECORDS_PER_FILE,
         hash_bucket_count=DEFAULT_HASH_BUCKET_COUNT,
         read_kwargs_provider=None,
         drop_duplicates=True,
         is_inplace=False,
+        add_late_deltas=None,
         skip_enabled_compact_partition_drivers=None,
     ),
     "9-incremental-decimal-pk-multi-dup": IncrementalCompactionTestCaseParams(
         primary_keys={"pk_col_1"},
         sort_keys=[SortKey.of(key_name="sk_col_1")],
         partition_keys=[PartitionKey.of("region_id", PartitionKeyType.INT)],
         partition_values=["1"],
@@ -394,14 +407,15 @@
         expected_terminal_exception_message=None,
         do_create_placement_group=False,
         records_per_compacted_file=DEFAULT_MAX_RECORDS_PER_FILE,
         hash_bucket_count=DEFAULT_HASH_BUCKET_COUNT,
         read_kwargs_provider=None,
         drop_duplicates=True,
         is_inplace=False,
+        add_late_deltas=None,
         skip_enabled_compact_partition_drivers=None,
     ),
     "10-incremental-decimal-pk-partitionless": IncrementalCompactionTestCaseParams(
         primary_keys={"pk_col_1"},
         sort_keys=[SortKey.of(key_name="sk_col_1")],
         partition_keys=ZERO_VALUED_PARTITION_KEYS_PARAM,
         partition_values=ZERO_VALUED_PARTITION_VALUES_PARAM,
@@ -424,14 +438,15 @@
         expected_terminal_exception_message=None,
         do_create_placement_group=False,
         records_per_compacted_file=DEFAULT_MAX_RECORDS_PER_FILE,
         hash_bucket_count=DEFAULT_HASH_BUCKET_COUNT,
         read_kwargs_provider=None,
         drop_duplicates=True,
         is_inplace=False,
+        add_late_deltas=None,
         skip_enabled_compact_partition_drivers=None,
     ),
     "11-incremental-decimal-hash-bucket-single": IncrementalCompactionTestCaseParams(
         primary_keys={"pk_col_1"},
         sort_keys=[SortKey.of(key_name="sk_col_1")],
         partition_keys=ZERO_VALUED_PARTITION_KEYS_PARAM,
         partition_values=ZERO_VALUED_PARTITION_VALUES_PARAM,
@@ -454,14 +469,15 @@
         expected_terminal_exception_message=None,
         do_create_placement_group=False,
         records_per_compacted_file=DEFAULT_MAX_RECORDS_PER_FILE,
         hash_bucket_count=DEFAULT_HASH_BUCKET_COUNT,
         read_kwargs_provider=None,
         drop_duplicates=True,
         is_inplace=False,
+        add_late_deltas=None,
         skip_enabled_compact_partition_drivers=None,
     ),
     "12-incremental-decimal-single-hash-bucket": IncrementalCompactionTestCaseParams(
         primary_keys={"pk_col_1"},
         sort_keys=[SortKey.of(key_name="sk_col_1")],
         partition_keys=ZERO_VALUED_PARTITION_KEYS_PARAM,
         partition_values=ZERO_VALUED_PARTITION_VALUES_PARAM,
@@ -484,14 +500,15 @@
         expected_terminal_exception_message=None,
         do_create_placement_group=False,
         records_per_compacted_file=DEFAULT_MAX_RECORDS_PER_FILE,
         hash_bucket_count=1,
         read_kwargs_provider=None,
         drop_duplicates=True,
         is_inplace=False,
+        add_late_deltas=None,
         skip_enabled_compact_partition_drivers=None,
     ),
     "13-incremental-pkstr-skexists-isinplacecompacted": IncrementalCompactionTestCaseParams(
         primary_keys={"pk_col_1"},
         sort_keys=[SortKey.of(key_name="sk_col_1")],
         partition_keys=[PartitionKey.of("region_id", PartitionKeyType.INT)],
         partition_values=["1"],
@@ -514,12 +531,56 @@
         expected_terminal_exception_message=None,
         do_create_placement_group=False,
         records_per_compacted_file=DEFAULT_MAX_RECORDS_PER_FILE,
         hash_bucket_count=DEFAULT_HASH_BUCKET_COUNT,
         read_kwargs_provider=None,
         drop_duplicates=True,
         is_inplace=True,
+        add_late_deltas=[
+            (
+                pa.Table.from_arrays(
+                    [
+                        pa.array([str(i) for i in range(20)]),
+                        pa.array([i for i in range(20)]),
+                    ],
+                    names=["pk_col_1", "sk_col_1"],
+                ),
+                DeltaType.UPSERT,
+                None,
+            )
+        ],
+        skip_enabled_compact_partition_drivers=[CompactorVersion.V1],
+    ),
+    "14-incremental-pkstr-skexists-unhappy-hash-bucket-count-not-present": IncrementalCompactionTestCaseParams(
+        primary_keys={"pk_col_1"},
+        sort_keys=[SortKey.of(key_name="sk_col_1")],
+        partition_keys=[PartitionKey.of("region_id", PartitionKeyType.INT)],
+        partition_values=["1"],
+        input_deltas=pa.Table.from_arrays(
+            [
+                pa.array([str(i) for i in range(10)]),
+                pa.array([i for i in range(10)]),
+            ],
+            names=["pk_col_1", "sk_col_1"],
+        ),
+        input_deltas_delta_type=DeltaType.UPSERT,
+        expected_terminal_compact_partition_result=pa.Table.from_arrays(
+            [
+                pa.array([str(i) for i in range(10)]),
+                pa.array([i for i in range(10)]),
+            ],
+            names=["pk_col_1", "sk_col_1"],
+        ),
+        expected_terminal_exception=AssertionError,
+        expected_terminal_exception_message="hash_bucket_count is a required arg for compactor v2",
+        do_create_placement_group=False,
+        records_per_compacted_file=DEFAULT_MAX_RECORDS_PER_FILE,
+        hash_bucket_count=None,
+        read_kwargs_provider=None,
+        drop_duplicates=True,
+        is_inplace=False,
+        add_late_deltas=False,
         skip_enabled_compact_partition_drivers=[CompactorVersion.V1],
     ),
 }
 
 INCREMENTAL_TEST_CASES = with_compactor_version_func_test_param(INCREMENTAL_TEST_CASES)
```

### Comparing `deltacat-1.1.6/deltacat/tests/compute/compactor/steps/test_repartition.py` & `deltacat-1.1.7/deltacat/tests/compute/compactor/steps/test_repartition.py`

 * *Files identical despite different names*

### Comparing `deltacat-1.1.6/deltacat/tests/compute/compactor/utils/test_io.py` & `deltacat-1.1.7/deltacat/tests/compute/compactor/utils/test_io.py`

 * *Files identical despite different names*

### Comparing `deltacat-1.1.6/deltacat/tests/compute/compactor_v2/test_compaction_session.py` & `deltacat-1.1.7/deltacat/tests/compute/compactor_v2/test_compaction_session.py`

 * *Files 2% similar despite different names*

```diff
@@ -31,14 +31,16 @@
         cls.deltacat_storage_kwargs = {ds.DB_FILE_PATH_ARG: cls.DB_FILE_PATH}
 
         super().setUpClass()
 
     @classmethod
     def doClassCleanups(cls) -> None:
         os.remove(cls.DB_FILE_PATH)
+        ray.shutdown()
+        super().tearDownClass()
 
     @patch("deltacat.compute.compactor_v2.compaction_session.rcf")
     @patch("deltacat.compute.compactor_v2.compaction_session.s3_utils")
     def test_compact_partition_when_no_input_deltas_to_compact(self, s3_utils, rcf_url):
         # setup
         rcf_url.read_round_completion_file.return_value = None
         staged_source = stage_partition_from_file_paths(
```

### Comparing `deltacat-1.1.6/deltacat/tests/compute/compactor_v2/utils/test_task_options.py` & `deltacat-1.1.7/deltacat/tests/compute/compactor_v2/utils/test_task_options.py`

 * *Files identical despite different names*

### Comparing `deltacat-1.1.6/deltacat/tests/compute/test_compact_partition_incremental.py` & `deltacat-1.1.7/deltacat/tests/compute/test_compact_partition_incremental.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,52 +1,76 @@
 import ray
 from moto import mock_s3
 import pytest
 import os
+import logging
 import boto3
-from typing import Any, Callable, Dict, List, Optional, Set
+from typing import Any, Callable, Dict, List, Optional, Set, Tuple
 from boto3.resources.base import ServiceResource
 import pyarrow as pa
 from pytest_benchmark.fixture import BenchmarkFixture
 from deltacat.types.media import StorageType
 
 from deltacat.tests.compute.test_util_common import (
     get_rcf,
 )
 from deltacat.tests.test_utils.utils import read_s3_contents
 from deltacat.tests.compute.test_util_create_table_deltas_repo import (
     create_src_w_deltas_destination_plus_destination,
+    add_late_deltas_to_partition,
 )
 from deltacat.tests.compute.compact_partition_test_cases import (
     INCREMENTAL_TEST_CASES,
 )
 from deltacat.tests.compute.test_util_constant import (
     TEST_S3_RCF_BUCKET_NAME,
     DEFAULT_NUM_WORKERS,
     DEFAULT_WORKER_INSTANCE_CPUS,
 )
 from deltacat.compute.compactor import (
     RoundCompletionInfo,
 )
+from deltacat.storage import (
+    CommitState,
+    DeltaType,
+    Delta,
+    DeltaLocator,
+    Partition,
+    PartitionLocator,
+)
+from deltacat.types.media import ContentType
+from deltacat.compute.compactor.model.compaction_session_audit_info import (
+    CompactionSessionAuditInfo,
+)
+from deltacat.compute.compactor.model.compact_partition_params import (
+    CompactPartitionParams,
+)
+from deltacat.utils.placement import (
+    PlacementGroupManager,
+)
+from deltacat import logs
 
 DATABASE_FILE_PATH_KEY, DATABASE_FILE_PATH_VALUE = (
     "db_file_path",
     "deltacat/tests/local_deltacat_storage/db_test.sqlite",
 )
 
+logger = logs.configure_deltacat_logger(logging.getLogger(__name__))
+
 
 """
 MODULE scoped fixtures
 """
 
 
 @pytest.fixture(autouse=True, scope="module")
 def setup_ray_cluster():
     ray.init(local_mode=True, ignore_reinit_error=True)
     yield
+    ray.shutdown()
 
 
 @pytest.fixture(autouse=True, scope="module")
 def mock_aws_credential():
     os.environ["AWS_ACCESS_KEY_ID"] = "testing"
     os.environ["AWS_SECRET_ACCESS_ID"] = "testing"
     os.environ["AWS_SECURITY_TOKEN"] = "testing"
@@ -54,27 +78,28 @@
     os.environ["AWS_DEFAULT_REGION"] = "us-east-1"
     yield
 
 
 @pytest.fixture(autouse=True, scope="module")
 def cleanup_the_database_file_after_all_compaction_session_package_tests_complete():
     # make sure the database file is deleted after all the compactor package tests are completed
+    yield
     if os.path.exists(DATABASE_FILE_PATH_VALUE):
         os.remove(DATABASE_FILE_PATH_VALUE)
 
 
 @pytest.fixture(scope="module")
-def setup_s3_resource(mock_aws_credential):
+def s3_resource():
     with mock_s3():
         yield boto3.resource("s3")
 
 
 @pytest.fixture(autouse=True, scope="module")
-def setup_compaction_artifacts_s3_bucket(setup_s3_resource: ServiceResource):
-    setup_s3_resource.create_bucket(
+def setup_compaction_artifacts_s3_bucket(s3_resource: ServiceResource):
+    s3_resource.create_bucket(
         ACL="authenticated-read",
         Bucket=TEST_S3_RCF_BUCKET_NAME,
     )
     yield
 
 
 """
@@ -108,14 +133,15 @@
         "create_placement_group_param",
         "records_per_compacted_file_param",
         "hash_bucket_count_param",
         "read_kwargs_provider_param",
         "drop_duplicates_param",
         "skip_enabled_compact_partition_drivers",
         "is_inplace",
+        "add_late_deltas",
         "compact_partition_func",
     ],
     [
         (
             test_name,
             primary_keys,
             sort_keys,
@@ -129,14 +155,15 @@
             create_placement_group_param,
             records_per_compacted_file_param,
             hash_bucket_count_param,
             drop_duplicates_param,
             read_kwargs_provider,
             skip_enabled_compact_partition_drivers,
             is_inplace,
+            add_late_deltas,
             compact_partition_func,
         )
         for test_name, (
             primary_keys,
             sort_keys,
             partition_keys_param,
             partition_values_param,
@@ -148,21 +175,22 @@
             create_placement_group_param,
             records_per_compacted_file_param,
             hash_bucket_count_param,
             drop_duplicates_param,
             read_kwargs_provider,
             skip_enabled_compact_partition_drivers,
             is_inplace,
+            add_late_deltas,
             compact_partition_func,
         ) in INCREMENTAL_TEST_CASES.items()
     ],
     ids=[test_name for test_name in INCREMENTAL_TEST_CASES],
 )
 def test_compact_partition_incremental(
-    setup_s3_resource: ServiceResource,
+    s3_resource: ServiceResource,
     offer_local_deltacat_storage_kwargs: Dict[str, Any],
     test_name: str,
     primary_keys: Set[str],
     sort_keys: Dict[str, str],
     partition_keys_param: Optional[Dict[str, str]],
     partition_values_param: str,
     input_deltas: pa.Table,
@@ -173,42 +201,31 @@
     create_placement_group_param: bool,
     records_per_compacted_file_param: int,
     hash_bucket_count_param: int,
     drop_duplicates_param: bool,
     read_kwargs_provider_param: Any,
     skip_enabled_compact_partition_drivers,
     is_inplace: bool,
+    add_late_deltas: Optional[List[Tuple[pa.Table, DeltaType]]],
     compact_partition_func: Callable,
     benchmark: BenchmarkFixture,
 ):
     import deltacat.tests.local_deltacat_storage as ds
-    from deltacat.types.media import ContentType
-    from deltacat.storage import (
-        DeltaLocator,
-        Partition,
-        PartitionLocator,
-    )
-    from deltacat.compute.compactor.model.compaction_session_audit_info import (
-        CompactionSessionAuditInfo,
-    )
-    from deltacat.compute.compactor.model.compact_partition_params import (
-        CompactPartitionParams,
-    )
-    from deltacat.utils.placement import (
-        PlacementGroupManager,
-    )
 
     ds_mock_kwargs: Dict[str, Any] = offer_local_deltacat_storage_kwargs
 
     # setup
     partition_keys = partition_keys_param
     (
         source_table_stream,
         destination_table_stream,
         _,
+        source_table_namespace,
+        source_table_name,
+        source_table_version,
     ) = create_src_w_deltas_destination_plus_destination(
         primary_keys,
         sort_keys,
         partition_keys,
         input_deltas,
         input_deltas_delta_type,
         partition_values_param,
@@ -223,19 +240,21 @@
     destination_partition_locator: PartitionLocator = PartitionLocator.of(
         destination_table_stream.locator,
         partition_values_param,
         None,
     )
     num_workers, worker_instance_cpu = DEFAULT_NUM_WORKERS, DEFAULT_WORKER_INSTANCE_CPUS
     total_cpus: int = num_workers * worker_instance_cpu
-    pgm: Optional[PlacementGroupManager] = None
-    if create_placement_group_param:
-        pgm = PlacementGroupManager(
+    pgm: Optional[PlacementGroupManager] = (
+        PlacementGroupManager(
             1, total_cpus, worker_instance_cpu, memory_per_bundle=4000000
         ).pgs[0]
+        if create_placement_group_param
+        else None
+    )
     compact_partition_params = CompactPartitionParams.of(
         {
             "compaction_artifact_s3_bucket": TEST_S3_RCF_BUCKET_NAME,
             "compacted_file_content_type": ContentType.PARQUET,
             "dd_max_parallelism_ratio": 1.0,
             "deltacat_storage": ds,
             "deltacat_storage_kwargs": ds_mock_kwargs,
@@ -261,32 +280,44 @@
         """
         This callable runs right before invoking the benchmark target function (compaction).
         This is needed as the benchmark module will invoke the target function multiple times
         in a single test run, which can lead to non-idempotent behavior if RCFs are generated.
 
         Returns: args, kwargs
         """
-        setup_s3_resource.Bucket(TEST_S3_RCF_BUCKET_NAME).objects.all().delete()
+        s3_resource.Bucket(TEST_S3_RCF_BUCKET_NAME).objects.all().delete()
         return (compact_partition_params,), {}
 
+    if add_late_deltas:
+        # NOTE: In the case of in-place compaction it is plausible that new deltas may be added to the source partition during compaction
+        # (so that the source_partitition.stream_position > last_stream_position_to_compact).
+        # This parameter helps simulate the case to check that no late deltas are dropped even when the compacted partition is created.
+        latest_delta, _ = add_late_deltas_to_partition(
+            add_late_deltas, source_partition, ds_mock_kwargs
+        )
+    if expected_terminal_exception:
+        with pytest.raises(expected_terminal_exception) as exc_info:
+            compact_partition_func(compact_partition_params)
+        assert expected_terminal_exception_message in str(exc_info.value)
+        return
     rcf_file_s3_uri = benchmark.pedantic(
         compact_partition_func, setup=_incremental_compaction_setup
     )
+
     # validate
-    round_completion_info: RoundCompletionInfo = get_rcf(
-        setup_s3_resource, rcf_file_s3_uri
-    )
+    round_completion_info: RoundCompletionInfo = get_rcf(s3_resource, rcf_file_s3_uri)
     compacted_delta_locator: DeltaLocator = (
         round_completion_info.compacted_delta_locator
     )
-    audit_bucket, audit_key = round_completion_info.compaction_audit_url.replace(
-        "s3://", ""
-    ).split("/", 1)
+    audit_bucket, audit_key = RoundCompletionInfo.get_audit_bucket_name_and_key(
+        round_completion_info.compaction_audit_url
+    )
+
     compaction_audit_obj: Dict[str, Any] = read_s3_contents(
-        setup_s3_resource, audit_bucket, audit_key
+        s3_resource, audit_bucket, audit_key
     )
     compaction_audit: CompactionSessionAuditInfo = CompactionSessionAuditInfo(
         **compaction_audit_obj
     )
 
     tables = ds.download_delta(
         compacted_delta_locator, storage_type=StorageType.LOCAL, **ds_mock_kwargs
@@ -314,12 +345,38 @@
 
     if is_inplace:
         assert (
             source_partition.locator.partition_values
             == destination_partition_locator.partition_values
             and source_partition.locator.stream_id
             == destination_partition_locator.stream_id
-        ), "The source partition should match the destination partition"
+        ), f"The source partition: {source_partition.locator.canonical_string} should match the destination partition: {destination_partition_locator.canonical_string}"
         assert (
             compacted_delta_locator.stream_id == source_partition.locator.stream_id
         ), "The compacted delta should be in the same stream as the source"
+        source_partition: Partition = ds.get_partition(
+            source_table_stream.locator,
+            partition_values_param,
+            **ds_mock_kwargs,
+        )
+        compacted_partition: Optional[Partition] = ds.get_partition(
+            compacted_delta_locator.stream_locator,
+            partition_values_param,
+            **ds_mock_kwargs,
+        )
+        assert (
+            compacted_partition.state == source_partition.state == CommitState.COMMITTED
+        ), f"The compacted/source table partition should be in {CommitState.COMMITTED} state and not {CommitState.DEPRECATED}"
+        if add_late_deltas:
+            compacted_partition_deltas: List[Delta] = ds.list_partition_deltas(
+                partition_like=compacted_partition,
+                ascending_order=False,
+                **ds_mock_kwargs,
+            ).all_items()
+            assert (
+                len(compacted_partition_deltas) == len(add_late_deltas) + 1
+            ), f"Expected the number of deltas within the newly promoted partition to equal 1 (the compacted delta) + the # of late deltas: {len(add_late_deltas)}"
+            assert (
+                compacted_partition_deltas[0].stream_position
+                == latest_delta.stream_position
+            ), f"Expected the latest delta in the compacted partition: {compacted_partition_deltas[0].stream_position} to have the same stream position as the latest delta: {latest_delta.stream_position}"
     return
```

### Comparing `deltacat-1.1.6/deltacat/tests/compute/test_compact_partition_params.py` & `deltacat-1.1.7/deltacat/tests/compute/test_compact_partition_params.py`

 * *Files identical despite different names*

### Comparing `deltacat-1.1.6/deltacat/tests/compute/test_compact_partition_rebase_then_incremental.py` & `deltacat-1.1.7/deltacat/tests/compute/test_compact_partition_rebase_then_incremental.py`

 * *Files 6% similar despite different names*

```diff
@@ -33,14 +33,27 @@
 from deltacat.tests.compute.compact_partition_rebase_then_incremental_test_cases import (
     REBASE_THEN_INCREMENTAL_TEST_CASES,
 )
 from typing import Any, Callable, Dict, List, Optional, Set, Tuple
 from deltacat.types.media import StorageType
 from deltacat.storage import (
     DeltaType,
+    DeltaLocator,
+    Partition,
+    PartitionLocator,
+)
+from deltacat.types.media import ContentType
+from deltacat.compute.compactor.model.compact_partition_params import (
+    CompactPartitionParams,
+)
+from deltacat.utils.placement import (
+    PlacementGroupManager,
+)
+from deltacat.compute.compactor.model.compaction_session_audit_info import (
+    CompactionSessionAuditInfo,
 )
 
 DATABASE_FILE_PATH_KEY, DATABASE_FILE_PATH_VALUE = (
     "db_file_path",
     "deltacat/tests/local_deltacat_storage/db_test.sqlite",
 )
 
@@ -50,14 +63,15 @@
 """
 
 
 @pytest.fixture(autouse=True, scope="module")
 def setup_ray_cluster():
     ray.init(local_mode=True, ignore_reinit_error=True)
     yield
+    ray.shutdown()
 
 
 @pytest.fixture(autouse=True, scope="module")
 def mock_aws_credential():
     os.environ["AWS_ACCESS_KEY_ID"] = "testing"
     os.environ["AWS_SECRET_ACCESS_ID"] = "testing"
     os.environ["AWS_SECURITY_TOKEN"] = "testing"
@@ -70,22 +84,22 @@
 def cleanup_the_database_file_after_all_compaction_session_package_tests_complete():
     # make sure the database file is deleted after all the compactor package tests are completed
     if os.path.exists(DATABASE_FILE_PATH_VALUE):
         os.remove(DATABASE_FILE_PATH_VALUE)
 
 
 @pytest.fixture(scope="module")
-def setup_s3_resource(mock_aws_credential):
+def s3_resource(mock_aws_credential):
     with mock_s3():
         yield boto3.resource("s3")
 
 
 @pytest.fixture(autouse=True, scope="module")
-def setup_compaction_artifacts_s3_bucket(setup_s3_resource: ServiceResource):
-    setup_s3_resource.create_bucket(
+def setup_compaction_artifacts_s3_bucket(s3_resource: ServiceResource):
+    s3_resource.create_bucket(
         ACL="authenticated-read",
         Bucket=TEST_S3_RCF_BUCKET_NAME,
     )
     yield
 
 
 """
@@ -168,15 +182,15 @@
             rebase_expected_compact_partition_result,
             compact_partition_func,
         ) in REBASE_THEN_INCREMENTAL_TEST_CASES.items()
     ],
     ids=[test_name for test_name in REBASE_THEN_INCREMENTAL_TEST_CASES],
 )
 def test_compact_partition_rebase_then_incremental(
-    setup_s3_resource: ServiceResource,
+    s3_resource: ServiceResource,
     local_deltacat_storage_kwargs: Dict[str, Any],
     test_name: str,
     primary_keys: Set[str],
     sort_keys: List[Optional[Any]],
     partition_keys_param: Optional[List[Any]],
     partition_values_param: List[Optional[str]],
     input_deltas_param: List[pa.Array],
@@ -192,33 +206,16 @@
     incremental_deltas: List[Tuple[pa.Table, DeltaType, Optional[Dict[str, str]]]],
     rebase_expected_compact_partition_result: pa.Table,
     skip_enabled_compact_partition_drivers: List[CompactorVersion],
     compact_partition_func: Callable,
     benchmark: BenchmarkFixture,
 ):
     import deltacat.tests.local_deltacat_storage as ds
-    from deltacat.types.media import ContentType
-    from deltacat.storage import (
-        DeltaLocator,
-        Partition,
-        PartitionLocator,
-    )
-    from deltacat.compute.compactor.model.compact_partition_params import (
-        CompactPartitionParams,
-    )
-    from deltacat.utils.placement import (
-        PlacementGroupManager,
-    )
-    from deltacat.compute.compactor.model.compaction_session_audit_info import (
-        CompactionSessionAuditInfo,
-    )
 
     ds_mock_kwargs = local_deltacat_storage_kwargs
-    ray.shutdown()
-    ray.init(local_mode=True, ignore_reinit_error=True)
     """
     REBASE
     """
     partition_keys = partition_keys_param
     (
         source_table_stream,
         destination_table_stream,
@@ -276,15 +273,15 @@
             "source_partition_locator": rebased_partition.locator,
             "sort_keys": sort_keys if sort_keys else None,
         }
     )
     # execute
     rcf_file_s3_uri = benchmark(compact_partition_func, compact_partition_params)
     compacted_delta_locator: DeltaLocator = get_compacted_delta_locator_from_rcf(
-        setup_s3_resource, rcf_file_s3_uri
+        s3_resource, rcf_file_s3_uri
     )
     tables = ds.download_delta(
         compacted_delta_locator, storage_type=StorageType.LOCAL, **ds_mock_kwargs
     )
     actual_rebase_compacted_table = pa.concat_tables(tables)
     # if no primary key is specified then sort by sort_key for consistent assertion
     sorting_cols: List[Any] = (
@@ -342,24 +339,22 @@
     )
     if expected_terminal_exception:
         with pytest.raises(expected_terminal_exception) as exc_info:
             compact_partition_func(compact_partition_params)
         assert expected_terminal_exception_message in str(exc_info.value)
         return
     rcf_file_s3_uri = compact_partition_func(compact_partition_params)
-    round_completion_info = get_rcf(setup_s3_resource, rcf_file_s3_uri)
+    round_completion_info = get_rcf(s3_resource, rcf_file_s3_uri)
     compacted_delta_locator_incremental: DeltaLocator = (
         round_completion_info.compacted_delta_locator
     )
     audit_bucket, audit_key = round_completion_info.compaction_audit_url.replace(
         "s3://", ""
     ).split("/", 1)
-    compaction_audit_obj: dict = read_s3_contents(
-        setup_s3_resource, audit_bucket, audit_key
-    )
+    compaction_audit_obj: dict = read_s3_contents(s3_resource, audit_bucket, audit_key)
     compaction_audit: CompactionSessionAuditInfo = CompactionSessionAuditInfo(
         **compaction_audit_obj
     )
 
     tables = ds.download_delta(
         compacted_delta_locator_incremental,
         storage_type=StorageType.LOCAL,
```

### Comparing `deltacat-1.1.6/deltacat/tests/compute/test_util_common.py` & `deltacat-1.1.7/deltacat/tests/compute/test_util_common.py`

 * *Files identical despite different names*

### Comparing `deltacat-1.1.6/deltacat/tests/compute/test_util_constant.py` & `deltacat-1.1.7/deltacat/tests/compute/test_util_constant.py`

 * *Files identical despite different names*

### Comparing `deltacat-1.1.6/deltacat/tests/compute/test_util_create_table_deltas_repo.py` & `deltacat-1.1.7/deltacat/tests/compute/test_util_create_table_deltas_repo.py`

 * *Files 4% similar despite different names*

```diff
@@ -15,14 +15,50 @@
     Stream,
 )
 from deltacat.tests.compute.test_util_common import (
     create_src_table,
     create_destination_table,
     create_rebase_table,
 )
+import logging
+from deltacat import logs
+
+logger = logs.configure_deltacat_logger(logging.getLogger(__name__))
+
+
+def _add_deltas_to_partition(
+    deltas_ingredients: List[Tuple[pa.Table, DeltaType, Optional[Dict[str, str]]]],
+    partition: Optional[Partition],
+    ds_mock_kwargs: Optional[Dict[str, Any]],
+) -> List[Optional[Delta], int]:
+    import deltacat.tests.local_deltacat_storage as ds
+
+    all_deltas_length = 0
+    for (delta_data, delta_type, delete_parameters) in deltas_ingredients:
+        staged_delta: Delta = ds.stage_delta(
+            delta_data,
+            partition,
+            delta_type,
+            delete_parameters=delete_parameters,
+            **ds_mock_kwargs,
+        )
+        incremental_delta = ds.commit_delta(
+            staged_delta,
+            **ds_mock_kwargs,
+        )
+        all_deltas_length += len(delta_data) if delta_data else 0
+    return incremental_delta, all_deltas_length
+
+
+def add_late_deltas_to_partition(
+    late_deltas: List[Tuple[pa.Table, DeltaType, Optional[Dict[str, str]]]],
+    source_partition: Optional[Partition],
+    ds_mock_kwargs: Optional[Dict[str, Any]],
+) -> List[Optional[Delta], int]:
+    return _add_deltas_to_partition(late_deltas, source_partition, ds_mock_kwargs)
 
 
 def create_incremental_deltas_on_source_table(
     source_namespace: str,
     source_table_name: str,
     source_table_version: str,
     source_table_stream: Stream,
@@ -81,15 +117,15 @@
     sort_keys: Optional[List[Any]],
     partition_keys: Optional[List[PartitionKey]],
     input_deltas: pa.Table,
     input_delta_type: DeltaType,
     partition_values: Optional[List[Any]],
     ds_mock_kwargs: Optional[Dict[str, Any]],
     simulate_is_inplace: bool = False,
-) -> Tuple[Stream, Stream, Optional[Stream]]:
+) -> Tuple[Stream, Stream, Optional[Stream], str, str, str]:
     import deltacat.tests.local_deltacat_storage as ds
 
     source_namespace, source_table_name, source_table_version = create_src_table(
         primary_keys, sort_keys, partition_keys, ds_mock_kwargs
     )
 
     source_table_stream: Stream = ds.get_stream(
@@ -133,15 +169,22 @@
 
     destination_table_stream: Stream = ds.get_stream(
         namespace=destination_table_namespace,
         table_name=destination_table_name,
         table_version=destination_table_version,
         **ds_mock_kwargs,
     )
-    return source_table_stream_after_committed, destination_table_stream, None
+    return (
+        source_table_stream_after_committed,
+        destination_table_stream,
+        None,
+        source_namespace,
+        source_table_name,
+        source_table_version,
+    )
 
 
 def create_src_w_deltas_destination_rebase_w_deltas_strategy(
     primary_keys: Set[str],
     sort_keys: Optional[List[Any]],
     partition_keys: Optional[List[PartitionKey]],
     input_deltas: pa.Table,
```

### Comparing `deltacat-1.1.6/deltacat/tests/io/test_cloudpickle_bug_fix.py` & `deltacat-1.1.7/deltacat/tests/io/test_cloudpickle_bug_fix.py`

 * *Files identical despite different names*

### Comparing `deltacat-1.1.6/deltacat/tests/io/test_file_object_store.py` & `deltacat-1.1.7/deltacat/tests/io/test_file_object_store.py`

 * *Files identical despite different names*

### Comparing `deltacat-1.1.6/deltacat/tests/io/test_memcached_object_store.py` & `deltacat-1.1.7/deltacat/tests/io/test_memcached_object_store.py`

 * *Files identical despite different names*

### Comparing `deltacat-1.1.6/deltacat/tests/io/test_ray_plasma_object_store.py` & `deltacat-1.1.7/deltacat/tests/io/test_ray_plasma_object_store.py`

 * *Files identical despite different names*

### Comparing `deltacat-1.1.6/deltacat/tests/io/test_redis_object_store.py` & `deltacat-1.1.7/deltacat/tests/io/test_redis_object_store.py`

 * *Files identical despite different names*

### Comparing `deltacat-1.1.6/deltacat/tests/io/test_s3_object_store.py` & `deltacat-1.1.7/deltacat/tests/io/test_s3_object_store.py`

 * *Files identical despite different names*

### Comparing `deltacat-1.1.6/deltacat/tests/local_deltacat_storage/__init__.py` & `deltacat-1.1.7/deltacat/tests/local_deltacat_storage/__init__.py`

 * *Files 2% similar despite different names*

```diff
@@ -267,17 +267,15 @@
             <= last_stream_position
         ):
             result.append(current_delta)
 
         if not include_manifest:
             current_delta.manifest = None
 
-    result.sort(
-        reverse=True if not ascending_order else False, key=lambda d: d.stream_position
-    )
+    result.sort(reverse=(not ascending_order), key=lambda d: d.stream_position)
     return ListResult.of(result, None, None)
 
 
 def get_delta(
     namespace: str,
     table_name: str,
     stream_position: int,
@@ -794,41 +792,65 @@
     )
     cur.execute("INSERT INTO partitions VALUES (?, ?, ?)", params)
     con.commit()
 
     return partition
 
 
-def commit_partition(partition: Partition, *args, **kwargs) -> Partition:
+def commit_partition(
+    partition: Partition,
+    previous_partition: Optional[Partition] = None,
+    *args,
+    **kwargs,
+) -> Partition:
     cur, con = _get_sqlite3_cursor_con(kwargs)
-    pv_partition = get_partition(
+    pv_partition: Optional[Partition] = previous_partition or get_partition(
         partition.stream_locator,
         partition_values=partition.partition_values,
         *args,
         **kwargs,
     )
-
-    # deprecate old and commit new one
+    # deprecate old partition and commit new one
     if pv_partition:
         pv_partition.state = CommitState.DEPRECATED
         params = (json.dumps(pv_partition), pv_partition.locator.canonical_string())
         cur.execute("UPDATE partitions SET value = ? WHERE locator = ?", params)
-
-    deltas = list_partition_deltas(partition, *args, **kwargs).all_items()
-    deltas.sort(reverse=True, key=lambda x: x.stream_position)
-
-    stream_position = partition.stream_position
-    if deltas:
-        stream_position = deltas[0].stream_position
+    previous_partition_deltas = (
+        list_partition_deltas(
+            pv_partition, ascending_order=False, *args, **kwargs
+        ).all_items()
+        or []
+    )
+    partition_deltas: Optional[List[Delta]] = (
+        list_partition_deltas(
+            partition, ascending_order=False, *args, **kwargs
+        ).all_items()
+        or []
+    )
+    previous_partition_deltas_spos_gt: List[Delta] = [
+        delta
+        for delta in previous_partition_deltas
+        if delta.stream_position > partition_deltas[0].stream_position
+    ]
+    # handle the case if the previous partition deltas have a greater stream position than the partition_delta
+    partition_deltas = previous_partition_deltas_spos_gt + partition_deltas
+
+    stream_position = (
+        partition_deltas[0].stream_position
+        if partition_deltas
+        else partition.stream_position
+    )
 
     partition.state = CommitState.COMMITTED
     partition.stream_position = stream_position
     partition.previous_stream_position = (
         pv_partition.stream_position if pv_partition else None
     )
+    if partition_deltas:
+        partition.locator = partition_deltas[0].partition_locator
     params = (json.dumps(partition), partition.locator.canonical_string())
     cur.execute("UPDATE partitions SET value = ? WHERE locator = ?", params)
     con.commit()
 
     return partition
 
 
@@ -971,17 +993,16 @@
 
     con.commit()
     return delta
 
 
 def commit_delta(delta: Delta, *args, **kwargs) -> Delta:
     cur, con = _get_sqlite3_cursor_con(kwargs)
-
-    if not delta.stream_position:
-        delta.locator.stream_position = current_time_ms()
+    delta_stream_position: Optional[int] = delta.stream_position
+    delta.locator.stream_position = delta_stream_position or current_time_ms()
 
     params = (
         delta.locator.canonical_string(),
         delta.partition_locator.canonical_string(),
         json.dumps(delta),
     )
 
@@ -991,17 +1012,15 @@
         delta.partition_locator.canonical_string(),
         json.dumps(delta),
         delta.locator.canonical_string(),
     )
     cur.execute(
         "UPDATE deltas SET partition_locator = ?, value = ? WHERE locator = ?", params
     )
-
     con.commit()
-
     return delta
 
 
 def get_namespace(namespace: str, *args, **kwargs) -> Optional[Namespace]:
     cur, con = _get_sqlite3_cursor_con(kwargs)
     locator = NamespaceLocator.of(namespace)
```

### Comparing `deltacat-1.1.6/deltacat/tests/stats/test_intervals.py` & `deltacat-1.1.7/deltacat/tests/stats/test_intervals.py`

 * *Files identical despite different names*

### Comparing `deltacat-1.1.6/deltacat/tests/test_logs.py` & `deltacat-1.1.7/deltacat/tests/test_logs.py`

 * *Files identical despite different names*

### Comparing `deltacat-1.1.6/deltacat/tests/test_utils/pyarrow.py` & `deltacat-1.1.7/deltacat/tests/test_utils/pyarrow.py`

 * *Files identical despite different names*

### Comparing `deltacat-1.1.6/deltacat/tests/test_utils/storage.py` & `deltacat-1.1.7/deltacat/tests/test_utils/storage.py`

 * *Files identical despite different names*

### Comparing `deltacat-1.1.6/deltacat/tests/utils/test_cloudpickle.py` & `deltacat-1.1.7/deltacat/tests/utils/test_cloudpickle.py`

 * *Files identical despite different names*

### Comparing `deltacat-1.1.6/deltacat/tests/utils/test_daft.py` & `deltacat-1.1.7/deltacat/tests/utils/test_daft.py`

 * *Files identical despite different names*

### Comparing `deltacat-1.1.6/deltacat/tests/utils/test_metrics.py` & `deltacat-1.1.7/deltacat/tests/utils/test_metrics.py`

 * *Files identical despite different names*

### Comparing `deltacat-1.1.6/deltacat/tests/utils/test_placement.py` & `deltacat-1.1.7/deltacat/tests/utils/test_placement.py`

 * *Files identical despite different names*

### Comparing `deltacat-1.1.6/deltacat/tests/utils/test_pyarrow.py` & `deltacat-1.1.7/deltacat/tests/utils/test_pyarrow.py`

 * *Files identical despite different names*

### Comparing `deltacat-1.1.6/deltacat/tests/utils/test_record_batch_tables.py` & `deltacat-1.1.7/deltacat/tests/utils/test_record_batch_tables.py`

 * *Files identical despite different names*

### Comparing `deltacat-1.1.6/deltacat/types/media.py` & `deltacat-1.1.7/deltacat/types/media.py`

 * *Files identical despite different names*

### Comparing `deltacat-1.1.6/deltacat/types/partial_download.py` & `deltacat-1.1.7/deltacat/types/partial_download.py`

 * *Files identical despite different names*

### Comparing `deltacat-1.1.6/deltacat/types/tables.py` & `deltacat-1.1.7/deltacat/types/tables.py`

 * *Files identical despite different names*

### Comparing `deltacat-1.1.6/deltacat/utils/arguments.py` & `deltacat-1.1.7/deltacat/utils/arguments.py`

 * *Files identical despite different names*

### Comparing `deltacat-1.1.6/deltacat/utils/cloudpickle.py` & `deltacat-1.1.7/deltacat/utils/cloudpickle.py`

 * *Files identical despite different names*

### Comparing `deltacat-1.1.6/deltacat/utils/common.py` & `deltacat-1.1.7/deltacat/utils/common.py`

 * *Files identical despite different names*

### Comparing `deltacat-1.1.6/deltacat/utils/daft.py` & `deltacat-1.1.7/deltacat/utils/daft.py`

 * *Files identical despite different names*

### Comparing `deltacat-1.1.6/deltacat/utils/metrics.py` & `deltacat-1.1.7/deltacat/utils/metrics.py`

 * *Files identical despite different names*

### Comparing `deltacat-1.1.6/deltacat/utils/numpy.py` & `deltacat-1.1.7/deltacat/utils/numpy.py`

 * *Files identical despite different names*

### Comparing `deltacat-1.1.6/deltacat/utils/pandas.py` & `deltacat-1.1.7/deltacat/utils/pandas.py`

 * *Files identical despite different names*

### Comparing `deltacat-1.1.6/deltacat/utils/performance.py` & `deltacat-1.1.7/deltacat/utils/performance.py`

 * *Files identical despite different names*

### Comparing `deltacat-1.1.6/deltacat/utils/placement.py` & `deltacat-1.1.7/deltacat/utils/placement.py`

 * *Files identical despite different names*

### Comparing `deltacat-1.1.6/deltacat/utils/pyarrow.py` & `deltacat-1.1.7/deltacat/utils/pyarrow.py`

 * *Files identical despite different names*

### Comparing `deltacat-1.1.6/deltacat/utils/ray_utils/collections.py` & `deltacat-1.1.7/deltacat/utils/ray_utils/collections.py`

 * *Files identical despite different names*

### Comparing `deltacat-1.1.6/deltacat/utils/ray_utils/concurrency.py` & `deltacat-1.1.7/deltacat/utils/ray_utils/concurrency.py`

 * *Files identical despite different names*

### Comparing `deltacat-1.1.6/deltacat/utils/ray_utils/dataset.py` & `deltacat-1.1.7/deltacat/utils/ray_utils/dataset.py`

 * *Files identical despite different names*

### Comparing `deltacat-1.1.6/deltacat/utils/ray_utils/runtime.py` & `deltacat-1.1.7/deltacat/utils/ray_utils/runtime.py`

 * *Files identical despite different names*

### Comparing `deltacat-1.1.6/deltacat/utils/resources.py` & `deltacat-1.1.7/deltacat/utils/resources.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,10 +1,12 @@
 # Allow classes to use self-referencing Type hints in Python 3.7.
 from __future__ import annotations
 
+import functools
+import signal
 from contextlib import AbstractContextManager
 from types import TracebackType
 import ray
 import sys
 import threading
 import time
 from typing import Dict, Any, Optional
@@ -226,7 +228,50 @@
                 while not cease_continuous_run.is_set():
                     schedule.run_pending()
                     time.sleep(float(str(interval)))
 
         continuous_thread = ScheduleThread()
         continuous_thread.start()
         return cease_continuous_run
+
+
+def timeout(value_in_seconds: int):
+    """
+    A decorator that will raise a TimeoutError if the decorated function takes longer
+    than the specified timeout.
+
+    Note: The decorator does not work in a multithreading env or on Windows platform.
+    Hence, the default behavior is same as executing a method without timeout set.
+
+    Also note: it is still the responsibility of the caller to clean up any resource leaks
+    during the execution of the underlying function.
+    """
+
+    def _decorate(func):
+        @functools.wraps(func)
+        def wrapper(*args, **kwargs):
+            current_platform = platform.system()
+
+            def handler(signum, frame):
+                raise TimeoutError(
+                    f"Timeout occurred on method: {func.__name__},"
+                    f" args={args}, kwargs={kwargs}"
+                )
+
+            if current_platform == "Windows":
+                return func(*args, **kwargs)
+
+            old_handler = signal.signal(signal.SIGALRM, handler)
+            # An alarm works per process.
+            # https://pubs.opengroup.org/onlinepubs/9699919799/functions/alarm.html
+            signal.alarm(value_in_seconds)
+            try:
+                return func(*args, **kwargs)
+            finally:
+                # reset the SIGALRM handler
+                signal.signal(signal.SIGALRM, old_handler)
+                # cancel the alarm
+                signal.alarm(0)
+
+        return wrapper
+
+    return _decorate
```

### Comparing `deltacat-1.1.6/deltacat/utils/s3fs.py` & `deltacat-1.1.7/deltacat/utils/s3fs.py`

 * *Files identical despite different names*

### Comparing `deltacat-1.1.6/deltacat/utils/schema.py` & `deltacat-1.1.7/deltacat/utils/schema.py`

 * *Files identical despite different names*

### Comparing `deltacat-1.1.6/deltacat.egg-info/PKG-INFO` & `deltacat-1.1.7/deltacat.egg-info/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: deltacat
-Version: 1.1.6
+Version: 1.1.7
 Summary: A scalable, fast, ACID-compliant Data Catalog powered by Ray.
 Home-page: https://github.com/ray-project/deltacat
 Author: Ray Team
 License: UNKNOWN
 Description: # DeltaCAT
         
         DeltaCAT is a Pythonic Data Catalog powered by Ray.
```

### Comparing `deltacat-1.1.6/deltacat.egg-info/SOURCES.txt` & `deltacat-1.1.7/deltacat.egg-info/SOURCES.txt`

 * *Files 1% similar despite different names*

```diff
@@ -63,14 +63,15 @@
 deltacat/compute/compactor_v2/deletes/__init__.py
 deltacat/compute/compactor_v2/deletes/delete_file_envelope.py
 deltacat/compute/compactor_v2/deletes/delete_strategy.py
 deltacat/compute/compactor_v2/deletes/delete_strategy_equality_delete.py
 deltacat/compute/compactor_v2/deletes/model.py
 deltacat/compute/compactor_v2/deletes/utils.py
 deltacat/compute/compactor_v2/model/__init__.py
+deltacat/compute/compactor_v2/model/compaction_session.py
 deltacat/compute/compactor_v2/model/hash_bucket_input.py
 deltacat/compute/compactor_v2/model/hash_bucket_result.py
 deltacat/compute/compactor_v2/model/merge_file_group.py
 deltacat/compute/compactor_v2/model/merge_input.py
 deltacat/compute/compactor_v2/model/merge_result.py
 deltacat/compute/compactor_v2/steps/__init__.py
 deltacat/compute/compactor_v2/steps/hash_bucket.py
@@ -186,14 +187,16 @@
 deltacat/tests/utils/test_daft.py
 deltacat/tests/utils/test_metrics.py
 deltacat/tests/utils/test_placement.py
 deltacat/tests/utils/test_pyarrow.py
 deltacat/tests/utils/test_record_batch_tables.py
 deltacat/tests/utils/test_resources.py
 deltacat/tests/utils/data/__init__.py
+deltacat/tests/utils/ray_utils/__init__.py
+deltacat/tests/utils/ray_utils/test_concurrency.py
 deltacat/types/__init__.py
 deltacat/types/media.py
 deltacat/types/partial_download.py
 deltacat/types/tables.py
 deltacat/utils/__init__.py
 deltacat/utils/arguments.py
 deltacat/utils/cloudpickle.py
```

### Comparing `deltacat-1.1.6/setup.py` & `deltacat-1.1.7/setup.py`

 * *Files identical despite different names*

