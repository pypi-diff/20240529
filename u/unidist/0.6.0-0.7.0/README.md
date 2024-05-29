# Comparing `tmp/unidist-0.6.0.tar.gz` & `tmp/unidist-0.7.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "unidist-0.6.0.tar", last modified: Mon Jan  8 21:02:42 2024, max compression
+gzip compressed data, was "unidist-0.7.0.tar", last modified: Wed May 29 14:08:39 2024, max compression
```

## Comparing `unidist-0.6.0.tar` & `unidist-0.7.0.tar`

### file list

```diff
@@ -1,127 +1,127 @@
-drwxrwxr-x   0 yigoshev  (1003) yigoshev  (1003)        0 2024-01-08 21:02:42.430157 unidist-0.6.0/
--rw-rw-r--   0 yigoshev  (1003) yigoshev  (1003)      687 2024-01-08 20:53:10.000000 unidist-0.6.0/AUTHORS
--rw-rw-r--   0 yigoshev  (1003) yigoshev  (1003)    11357 2024-01-08 20:53:10.000000 unidist-0.6.0/LICENSE
--rw-rw-r--   0 yigoshev  (1003) yigoshev  (1003)       50 2024-01-08 20:53:10.000000 unidist-0.6.0/MANIFEST.in
--rw-r--r--   0 yigoshev  (1003) yigoshev  (1003)     7818 2024-01-08 21:02:42.430157 unidist-0.6.0/PKG-INFO
--rw-rw-r--   0 yigoshev  (1003) yigoshev  (1003)     6755 2024-01-08 20:53:10.000000 unidist-0.6.0/README.md
--rw-rw-r--   0 yigoshev  (1003) yigoshev  (1003)      354 2024-01-08 21:02:42.430157 unidist-0.6.0/setup.cfg
--rw-rw-r--   0 yigoshev  (1003) yigoshev  (1003)     2199 2024-01-08 20:53:10.000000 unidist-0.6.0/setup.py
-drwxrwxr-x   0 yigoshev  (1003) yigoshev  (1003)        0 2024-01-08 21:02:42.430157 unidist-0.6.0/unidist/
--rw-rw-r--   0 yigoshev  (1003) yigoshev  (1003)      559 2024-01-08 20:53:10.000000 unidist-0.6.0/unidist/__init__.py
--rw-rw-r--   0 yigoshev  (1003) yigoshev  (1003)      497 2024-01-08 21:02:42.430157 unidist-0.6.0/unidist/_version.py
--rw-rw-r--   0 yigoshev  (1003) yigoshev  (1003)     6912 2024-01-08 20:53:10.000000 unidist-0.6.0/unidist/api.py
-drwxrwxr-x   0 yigoshev  (1003) yigoshev  (1003)        0 2024-01-08 21:02:42.422157 unidist-0.6.0/unidist/config/
--rw-rw-r--   0 yigoshev  (1003) yigoshev  (1003)     1188 2024-01-08 20:53:10.000000 unidist-0.6.0/unidist/config/__init__.py
-drwxrwxr-x   0 yigoshev  (1003) yigoshev  (1003)        0 2024-01-08 21:02:42.422157 unidist-0.6.0/unidist/config/backends/
--rw-rw-r--   0 yigoshev  (1003) yigoshev  (1003)      172 2024-01-08 20:53:10.000000 unidist-0.6.0/unidist/config/backends/__init__.py
-drwxrwxr-x   0 yigoshev  (1003) yigoshev  (1003)        0 2024-01-08 21:02:42.422157 unidist-0.6.0/unidist/config/backends/common/
--rw-rw-r--   0 yigoshev  (1003) yigoshev  (1003)      232 2024-01-08 20:53:10.000000 unidist-0.6.0/unidist/config/backends/common/__init__.py
--rw-rw-r--   0 yigoshev  (1003) yigoshev  (1003)     2337 2024-01-08 20:53:10.000000 unidist-0.6.0/unidist/config/backends/common/envvars.py
-drwxrwxr-x   0 yigoshev  (1003) yigoshev  (1003)        0 2024-01-08 21:02:42.422157 unidist-0.6.0/unidist/config/backends/dask/
--rw-rw-r--   0 yigoshev  (1003) yigoshev  (1003)      323 2024-01-08 20:53:10.000000 unidist-0.6.0/unidist/config/backends/dask/__init__.py
--rw-rw-r--   0 yigoshev  (1003) yigoshev  (1003)      758 2024-01-08 20:53:10.000000 unidist-0.6.0/unidist/config/backends/dask/envvars.py
-drwxrwxr-x   0 yigoshev  (1003) yigoshev  (1003)        0 2024-01-08 21:02:42.422157 unidist-0.6.0/unidist/config/backends/mpi/
--rw-rw-r--   0 yigoshev  (1003) yigoshev  (1003)      676 2024-01-08 20:53:10.000000 unidist-0.6.0/unidist/config/backends/mpi/__init__.py
--rw-rw-r--   0 yigoshev  (1003) yigoshev  (1003)     4383 2024-01-08 20:53:10.000000 unidist-0.6.0/unidist/config/backends/mpi/envvars.py
-drwxrwxr-x   0 yigoshev  (1003) yigoshev  (1003)        0 2024-01-08 21:02:42.422157 unidist-0.6.0/unidist/config/backends/ray/
--rw-rw-r--   0 yigoshev  (1003) yigoshev  (1003)      434 2024-01-08 20:53:10.000000 unidist-0.6.0/unidist/config/backends/ray/__init__.py
--rw-rw-r--   0 yigoshev  (1003) yigoshev  (1003)     1131 2024-01-08 20:53:10.000000 unidist-0.6.0/unidist/config/backends/ray/envvars.py
--rw-rw-r--   0 yigoshev  (1003) yigoshev  (1003)     6866 2024-01-08 20:53:10.000000 unidist-0.6.0/unidist/config/parameter.py
-drwxrwxr-x   0 yigoshev  (1003) yigoshev  (1003)        0 2024-01-08 21:02:42.422157 unidist-0.6.0/unidist/core/
--rw-rw-r--   0 yigoshev  (1003) yigoshev  (1003)      107 2024-01-08 20:53:10.000000 unidist-0.6.0/unidist/core/__init__.py
-drwxrwxr-x   0 yigoshev  (1003) yigoshev  (1003)        0 2024-01-08 21:02:42.422157 unidist-0.6.0/unidist/core/backends/
--rw-rw-r--   0 yigoshev  (1003) yigoshev  (1003)       80 2024-01-08 20:53:10.000000 unidist-0.6.0/unidist/core/backends/__init__.py
-drwxrwxr-x   0 yigoshev  (1003) yigoshev  (1003)        0 2024-01-08 21:02:42.422157 unidist-0.6.0/unidist/core/backends/common/
--rw-rw-r--   0 yigoshev  (1003) yigoshev  (1003)      122 2024-01-08 20:53:10.000000 unidist-0.6.0/unidist/core/backends/common/__init__.py
--rw-rw-r--   0 yigoshev  (1003) yigoshev  (1003)      909 2024-01-08 20:53:10.000000 unidist-0.6.0/unidist/core/backends/common/data_id.py
--rw-rw-r--   0 yigoshev  (1003) yigoshev  (1003)     1121 2024-01-08 20:53:10.000000 unidist-0.6.0/unidist/core/backends/common/utils.py
-drwxrwxr-x   0 yigoshev  (1003) yigoshev  (1003)        0 2024-01-08 21:02:42.422157 unidist-0.6.0/unidist/core/backends/dask/
--rw-rw-r--   0 yigoshev  (1003) yigoshev  (1003)      115 2024-01-08 20:53:10.000000 unidist-0.6.0/unidist/core/backends/dask/__init__.py
--rw-rw-r--   0 yigoshev  (1003) yigoshev  (1003)     6692 2024-01-08 20:53:10.000000 unidist-0.6.0/unidist/core/backends/dask/actor.py
--rw-rw-r--   0 yigoshev  (1003) yigoshev  (1003)     5526 2024-01-08 20:53:10.000000 unidist-0.6.0/unidist/core/backends/dask/backend.py
--rw-rw-r--   0 yigoshev  (1003) yigoshev  (1003)     3460 2024-01-08 20:53:10.000000 unidist-0.6.0/unidist/core/backends/dask/remote_function.py
--rw-rw-r--   0 yigoshev  (1003) yigoshev  (1003)     1078 2024-01-08 20:53:10.000000 unidist-0.6.0/unidist/core/backends/dask/utils.py
-drwxrwxr-x   0 yigoshev  (1003) yigoshev  (1003)        0 2024-01-08 21:02:42.422157 unidist-0.6.0/unidist/core/backends/mpi/
--rw-rw-r--   0 yigoshev  (1003) yigoshev  (1003)      114 2024-01-08 20:53:10.000000 unidist-0.6.0/unidist/core/backends/mpi/__init__.py
--rw-rw-r--   0 yigoshev  (1003) yigoshev  (1003)     5692 2024-01-08 20:53:10.000000 unidist-0.6.0/unidist/core/backends/mpi/actor.py
--rw-rw-r--   0 yigoshev  (1003) yigoshev  (1003)     4668 2024-01-08 20:53:10.000000 unidist-0.6.0/unidist/core/backends/mpi/backend.py
-drwxrwxr-x   0 yigoshev  (1003) yigoshev  (1003)        0 2024-01-08 21:02:42.426157 unidist-0.6.0/unidist/core/backends/mpi/core/
--rwxrwxr-x   0 yigoshev  (1003) yigoshev  (1003)      408 2024-01-08 20:53:10.000000 unidist-0.6.0/unidist/core/backends/mpi/core/__init__.py
--rw-rw-r--   0 yigoshev  (1003) yigoshev  (1003)     1965 2024-01-08 20:53:10.000000 unidist-0.6.0/unidist/core/backends/mpi/core/async_operations.py
--rwxrwxr-x   0 yigoshev  (1003) yigoshev  (1003)    15186 2024-01-08 20:53:10.000000 unidist-0.6.0/unidist/core/backends/mpi/core/common.py
--rwxrwxr-x   0 yigoshev  (1003) yigoshev  (1003)    34133 2024-01-08 20:53:10.000000 unidist-0.6.0/unidist/core/backends/mpi/core/communication.py
-drwxrwxr-x   0 yigoshev  (1003) yigoshev  (1003)        0 2024-01-08 21:02:42.426157 unidist-0.6.0/unidist/core/backends/mpi/core/controller/
--rw-rw-r--   0 yigoshev  (1003) yigoshev  (1003)      533 2024-01-08 20:53:10.000000 unidist-0.6.0/unidist/core/backends/mpi/core/controller/__init__.py
--rw-rw-r--   0 yigoshev  (1003) yigoshev  (1003)     6575 2024-01-08 20:53:10.000000 unidist-0.6.0/unidist/core/backends/mpi/core/controller/actor.py
--rw-rw-r--   0 yigoshev  (1003) yigoshev  (1003)    19455 2024-01-08 20:53:10.000000 unidist-0.6.0/unidist/core/backends/mpi/core/controller/api.py
--rw-rw-r--   0 yigoshev  (1003) yigoshev  (1003)    14065 2024-01-08 20:53:10.000000 unidist-0.6.0/unidist/core/backends/mpi/core/controller/common.py
--rw-rw-r--   0 yigoshev  (1003) yigoshev  (1003)     5457 2024-01-08 20:53:10.000000 unidist-0.6.0/unidist/core/backends/mpi/core/controller/garbage_collector.py
--rw-rw-r--   0 yigoshev  (1003) yigoshev  (1003)     9355 2024-01-08 20:53:10.000000 unidist-0.6.0/unidist/core/backends/mpi/core/local_object_store.py
-drwxrwxr-x   0 yigoshev  (1003) yigoshev  (1003)        0 2024-01-08 21:02:42.426157 unidist-0.6.0/unidist/core/backends/mpi/core/memory/
--rw-rw-r--   0 yigoshev  (1003) yigoshev  (1003)  1033993 2024-01-08 21:02:20.000000 unidist-0.6.0/unidist/core/backends/mpi/core/memory/_memory.cpp
--rw-rw-r--   0 yigoshev  (1003) yigoshev  (1003)     2023 2024-01-08 20:53:10.000000 unidist-0.6.0/unidist/core/backends/mpi/core/memory/memory.cpp
--rw-rw-r--   0 yigoshev  (1003) yigoshev  (1003)      627 2024-01-08 20:53:10.000000 unidist-0.6.0/unidist/core/backends/mpi/core/memory/memory.h
-drwxrwxr-x   0 yigoshev  (1003) yigoshev  (1003)        0 2024-01-08 21:02:42.426157 unidist-0.6.0/unidist/core/backends/mpi/core/monitor/
--rw-rw-r--   0 yigoshev  (1003) yigoshev  (1003)      143 2024-01-08 20:53:10.000000 unidist-0.6.0/unidist/core/backends/mpi/core/monitor/__init__.py
--rwxrwxr-x   0 yigoshev  (1003) yigoshev  (1003)    10227 2024-01-08 20:53:10.000000 unidist-0.6.0/unidist/core/backends/mpi/core/monitor/loop.py
--rw-rw-r--   0 yigoshev  (1003) yigoshev  (1003)     7919 2024-01-08 20:53:10.000000 unidist-0.6.0/unidist/core/backends/mpi/core/monitor/shared_memory_manager.py
--rw-rw-r--   0 yigoshev  (1003) yigoshev  (1003)     2676 2024-01-08 20:53:10.000000 unidist-0.6.0/unidist/core/backends/mpi/core/object_store.py
--rwxrwxr-x   0 yigoshev  (1003) yigoshev  (1003)    10559 2024-01-08 20:53:10.000000 unidist-0.6.0/unidist/core/backends/mpi/core/serialization.py
--rw-rw-r--   0 yigoshev  (1003) yigoshev  (1003)    31634 2024-01-08 20:53:10.000000 unidist-0.6.0/unidist/core/backends/mpi/core/shared_object_store.py
-drwxrwxr-x   0 yigoshev  (1003) yigoshev  (1003)        0 2024-01-08 21:02:42.426157 unidist-0.6.0/unidist/core/backends/mpi/core/worker/
--rw-rw-r--   0 yigoshev  (1003) yigoshev  (1003)      142 2024-01-08 20:53:10.000000 unidist-0.6.0/unidist/core/backends/mpi/core/worker/__init__.py
--rw-rw-r--   0 yigoshev  (1003) yigoshev  (1003)     9495 2024-01-08 20:53:10.000000 unidist-0.6.0/unidist/core/backends/mpi/core/worker/loop.py
--rw-rw-r--   0 yigoshev  (1003) yigoshev  (1003)     9827 2024-01-08 20:53:10.000000 unidist-0.6.0/unidist/core/backends/mpi/core/worker/request_store.py
--rw-rw-r--   0 yigoshev  (1003) yigoshev  (1003)    18303 2024-01-08 20:53:10.000000 unidist-0.6.0/unidist/core/backends/mpi/core/worker/task_store.py
--rw-rw-r--   0 yigoshev  (1003) yigoshev  (1003)     3331 2024-01-08 20:53:10.000000 unidist-0.6.0/unidist/core/backends/mpi/remote_function.py
--rw-rw-r--   0 yigoshev  (1003) yigoshev  (1003)     1008 2024-01-08 20:53:10.000000 unidist-0.6.0/unidist/core/backends/mpi/utils.py
-drwxrwxr-x   0 yigoshev  (1003) yigoshev  (1003)        0 2024-01-08 21:02:42.426157 unidist-0.6.0/unidist/core/backends/pymp/
--rw-rw-r--   0 yigoshev  (1003) yigoshev  (1003)      133 2024-01-08 20:53:10.000000 unidist-0.6.0/unidist/core/backends/pymp/__init__.py
--rw-rw-r--   0 yigoshev  (1003) yigoshev  (1003)     4336 2024-01-08 20:53:10.000000 unidist-0.6.0/unidist/core/backends/pymp/actor.py
--rw-rw-r--   0 yigoshev  (1003) yigoshev  (1003)     4815 2024-01-08 20:53:10.000000 unidist-0.6.0/unidist/core/backends/pymp/backend.py
-drwxrwxr-x   0 yigoshev  (1003) yigoshev  (1003)        0 2024-01-08 21:02:42.426157 unidist-0.6.0/unidist/core/backends/pymp/core/
--rw-rw-r--   0 yigoshev  (1003) yigoshev  (1003)      305 2024-01-08 20:53:10.000000 unidist-0.6.0/unidist/core/backends/pymp/core/__init__.py
--rw-rw-r--   0 yigoshev  (1003) yigoshev  (1003)     4701 2024-01-08 20:53:10.000000 unidist-0.6.0/unidist/core/backends/pymp/core/actor.py
--rw-rw-r--   0 yigoshev  (1003) yigoshev  (1003)     4067 2024-01-08 20:53:10.000000 unidist-0.6.0/unidist/core/backends/pymp/core/api.py
--rw-rw-r--   0 yigoshev  (1003) yigoshev  (1003)     4268 2024-01-08 20:53:10.000000 unidist-0.6.0/unidist/core/backends/pymp/core/object_store.py
--rw-rw-r--   0 yigoshev  (1003) yigoshev  (1003)     6900 2024-01-08 20:53:10.000000 unidist-0.6.0/unidist/core/backends/pymp/core/process_manager.py
--rw-rw-r--   0 yigoshev  (1003) yigoshev  (1003)     3004 2024-01-08 20:53:10.000000 unidist-0.6.0/unidist/core/backends/pymp/remote_function.py
--rw-rw-r--   0 yigoshev  (1003) yigoshev  (1003)      506 2024-01-08 20:53:10.000000 unidist-0.6.0/unidist/core/backends/pymp/utils.py
-drwxrwxr-x   0 yigoshev  (1003) yigoshev  (1003)        0 2024-01-08 21:02:42.426157 unidist-0.6.0/unidist/core/backends/pyseq/
--rw-rw-r--   0 yigoshev  (1003) yigoshev  (1003)      128 2024-01-08 20:53:10.000000 unidist-0.6.0/unidist/core/backends/pyseq/__init__.py
--rw-rw-r--   0 yigoshev  (1003) yigoshev  (1003)     4225 2024-01-08 20:53:10.000000 unidist-0.6.0/unidist/core/backends/pyseq/actor.py
--rw-rw-r--   0 yigoshev  (1003) yigoshev  (1003)     4609 2024-01-08 20:53:10.000000 unidist-0.6.0/unidist/core/backends/pyseq/backend.py
-drwxrwxr-x   0 yigoshev  (1003) yigoshev  (1003)        0 2024-01-08 21:02:42.426157 unidist-0.6.0/unidist/core/backends/pyseq/core/
--rw-rw-r--   0 yigoshev  (1003) yigoshev  (1003)      252 2024-01-08 20:53:10.000000 unidist-0.6.0/unidist/core/backends/pyseq/core/__init__.py
--rw-rw-r--   0 yigoshev  (1003) yigoshev  (1003)     3060 2024-01-08 20:53:10.000000 unidist-0.6.0/unidist/core/backends/pyseq/core/api.py
--rw-rw-r--   0 yigoshev  (1003) yigoshev  (1003)     2313 2024-01-08 20:53:10.000000 unidist-0.6.0/unidist/core/backends/pyseq/core/object_store.py
--rw-rw-r--   0 yigoshev  (1003) yigoshev  (1003)     2905 2024-01-08 20:53:10.000000 unidist-0.6.0/unidist/core/backends/pyseq/remote_function.py
--rw-rw-r--   0 yigoshev  (1003) yigoshev  (1003)      382 2024-01-08 20:53:10.000000 unidist-0.6.0/unidist/core/backends/pyseq/utils.py
-drwxrwxr-x   0 yigoshev  (1003) yigoshev  (1003)        0 2024-01-08 21:02:42.426157 unidist-0.6.0/unidist/core/backends/ray/
--rw-rw-r--   0 yigoshev  (1003) yigoshev  (1003)      114 2024-01-08 20:53:10.000000 unidist-0.6.0/unidist/core/backends/ray/__init__.py
--rw-rw-r--   0 yigoshev  (1003) yigoshev  (1003)     5544 2024-01-08 20:53:10.000000 unidist-0.6.0/unidist/core/backends/ray/actor.py
--rw-rw-r--   0 yigoshev  (1003) yigoshev  (1003)     4616 2024-01-08 20:53:10.000000 unidist-0.6.0/unidist/core/backends/ray/backend.py
--rw-rw-r--   0 yigoshev  (1003) yigoshev  (1003)     2742 2024-01-08 20:53:10.000000 unidist-0.6.0/unidist/core/backends/ray/remote_function.py
--rw-rw-r--   0 yigoshev  (1003) yigoshev  (1003)     4778 2024-01-08 20:53:10.000000 unidist-0.6.0/unidist/core/backends/ray/utils.py
-drwxrwxr-x   0 yigoshev  (1003) yigoshev  (1003)        0 2024-01-08 21:02:42.430157 unidist-0.6.0/unidist/core/base/
--rw-rw-r--   0 yigoshev  (1003) yigoshev  (1003)      112 2024-01-08 20:53:10.000000 unidist-0.6.0/unidist/core/base/__init__.py
--rw-rw-r--   0 yigoshev  (1003) yigoshev  (1003)     6620 2024-01-08 20:53:10.000000 unidist-0.6.0/unidist/core/base/actor.py
--rw-rw-r--   0 yigoshev  (1003) yigoshev  (1003)    10573 2024-01-08 20:53:10.000000 unidist-0.6.0/unidist/core/base/backend.py
--rw-rw-r--   0 yigoshev  (1003) yigoshev  (1003)     1255 2024-01-08 20:53:10.000000 unidist-0.6.0/unidist/core/base/common.py
--rw-rw-r--   0 yigoshev  (1003) yigoshev  (1003)      384 2024-01-08 20:53:10.000000 unidist-0.6.0/unidist/core/base/object_ref.py
--rw-rw-r--   0 yigoshev  (1003) yigoshev  (1003)     3105 2024-01-08 20:53:10.000000 unidist-0.6.0/unidist/core/base/remote_function.py
--rw-rw-r--   0 yigoshev  (1003) yigoshev  (1003)     3330 2024-01-08 20:53:10.000000 unidist-0.6.0/unidist/core/base/utils.py
-drwxrwxr-x   0 yigoshev  (1003) yigoshev  (1003)        0 2024-01-08 21:02:42.430157 unidist-0.6.0/unidist/test/
--rw-rw-r--   0 yigoshev  (1003) yigoshev  (1003)       80 2024-01-08 20:53:10.000000 unidist-0.6.0/unidist/test/__init__.py
--rw-rw-r--   0 yigoshev  (1003) yigoshev  (1003)     4174 2024-01-08 20:53:10.000000 unidist-0.6.0/unidist/test/test_actor.py
--rw-rw-r--   0 yigoshev  (1003) yigoshev  (1003)     6039 2024-01-08 20:53:10.000000 unidist-0.6.0/unidist/test/test_async_actor.py
--rw-rw-r--   0 yigoshev  (1003) yigoshev  (1003)     2555 2024-01-08 20:53:10.000000 unidist-0.6.0/unidist/test/test_general.py
--rw-rw-r--   0 yigoshev  (1003) yigoshev  (1003)     2939 2024-01-08 20:53:10.000000 unidist-0.6.0/unidist/test/test_task.py
--rw-rw-r--   0 yigoshev  (1003) yigoshev  (1003)     2276 2024-01-08 20:53:10.000000 unidist-0.6.0/unidist/test/utils.py
-drwxrwxr-x   0 yigoshev  (1003) yigoshev  (1003)        0 2024-01-08 21:02:42.422157 unidist-0.6.0/unidist.egg-info/
--rw-r--r--   0 yigoshev  (1003) yigoshev  (1003)     7818 2024-01-08 21:02:42.000000 unidist-0.6.0/unidist.egg-info/PKG-INFO
--rw-rw-r--   0 yigoshev  (1003) yigoshev  (1003)     3736 2024-01-08 21:02:42.000000 unidist-0.6.0/unidist.egg-info/SOURCES.txt
--rw-rw-r--   0 yigoshev  (1003) yigoshev  (1003)        1 2024-01-08 21:02:42.000000 unidist-0.6.0/unidist.egg-info/dependency_links.txt
--rw-rw-r--   0 yigoshev  (1003) yigoshev  (1003)      273 2024-01-08 21:02:42.000000 unidist-0.6.0/unidist.egg-info/requires.txt
--rw-rw-r--   0 yigoshev  (1003) yigoshev  (1003)        8 2024-01-08 21:02:42.000000 unidist-0.6.0/unidist.egg-info/top_level.txt
--rw-rw-r--   0 yigoshev  (1003) yigoshev  (1003)    80049 2024-01-08 20:53:10.000000 unidist-0.6.0/versioneer.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-29 14:08:39.265344 unidist-0.7.0/
+-rw-r--r--   0 runner    (1001) docker     (127)      687 2024-05-29 14:08:34.000000 unidist-0.7.0/AUTHORS
+-rw-r--r--   0 runner    (1001) docker     (127)    11357 2024-05-29 14:08:34.000000 unidist-0.7.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)      165 2024-05-29 14:08:34.000000 unidist-0.7.0/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (127)     7106 2024-05-29 14:08:39.265344 unidist-0.7.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     6755 2024-05-29 14:08:34.000000 unidist-0.7.0/README.md
+-rw-r--r--   0 runner    (1001) docker     (127)      354 2024-05-29 14:08:39.265344 unidist-0.7.0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)     1503 2024-05-29 14:08:34.000000 unidist-0.7.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-29 14:08:39.253344 unidist-0.7.0/unidist/
+-rw-r--r--   0 runner    (1001) docker     (127)      539 2024-05-29 14:08:34.000000 unidist-0.7.0/unidist/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      497 2024-05-29 14:08:39.269344 unidist-0.7.0/unidist/_version.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6912 2024-05-29 14:08:34.000000 unidist-0.7.0/unidist/api.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-29 14:08:39.253344 unidist-0.7.0/unidist/config/
+-rw-r--r--   0 runner    (1001) docker     (127)     1188 2024-05-29 14:08:34.000000 unidist-0.7.0/unidist/config/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-29 14:08:39.253344 unidist-0.7.0/unidist/config/backends/
+-rw-r--r--   0 runner    (1001) docker     (127)      172 2024-05-29 14:08:34.000000 unidist-0.7.0/unidist/config/backends/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-29 14:08:39.253344 unidist-0.7.0/unidist/config/backends/common/
+-rw-r--r--   0 runner    (1001) docker     (127)      232 2024-05-29 14:08:34.000000 unidist-0.7.0/unidist/config/backends/common/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2337 2024-05-29 14:08:34.000000 unidist-0.7.0/unidist/config/backends/common/envvars.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-29 14:08:39.253344 unidist-0.7.0/unidist/config/backends/dask/
+-rw-r--r--   0 runner    (1001) docker     (127)      323 2024-05-29 14:08:34.000000 unidist-0.7.0/unidist/config/backends/dask/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      758 2024-05-29 14:08:34.000000 unidist-0.7.0/unidist/config/backends/dask/envvars.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-29 14:08:39.253344 unidist-0.7.0/unidist/config/backends/mpi/
+-rw-r--r--   0 runner    (1001) docker     (127)      676 2024-05-29 14:08:34.000000 unidist-0.7.0/unidist/config/backends/mpi/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4383 2024-05-29 14:08:34.000000 unidist-0.7.0/unidist/config/backends/mpi/envvars.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-29 14:08:39.253344 unidist-0.7.0/unidist/config/backends/ray/
+-rw-r--r--   0 runner    (1001) docker     (127)      434 2024-05-29 14:08:34.000000 unidist-0.7.0/unidist/config/backends/ray/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1131 2024-05-29 14:08:34.000000 unidist-0.7.0/unidist/config/backends/ray/envvars.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6866 2024-05-29 14:08:34.000000 unidist-0.7.0/unidist/config/parameter.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-29 14:08:39.253344 unidist-0.7.0/unidist/core/
+-rw-r--r--   0 runner    (1001) docker     (127)      107 2024-05-29 14:08:34.000000 unidist-0.7.0/unidist/core/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-29 14:08:39.253344 unidist-0.7.0/unidist/core/backends/
+-rw-r--r--   0 runner    (1001) docker     (127)       80 2024-05-29 14:08:34.000000 unidist-0.7.0/unidist/core/backends/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-29 14:08:39.253344 unidist-0.7.0/unidist/core/backends/common/
+-rw-r--r--   0 runner    (1001) docker     (127)      122 2024-05-29 14:08:34.000000 unidist-0.7.0/unidist/core/backends/common/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      909 2024-05-29 14:08:34.000000 unidist-0.7.0/unidist/core/backends/common/data_id.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1121 2024-05-29 14:08:34.000000 unidist-0.7.0/unidist/core/backends/common/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-29 14:08:39.257344 unidist-0.7.0/unidist/core/backends/dask/
+-rw-r--r--   0 runner    (1001) docker     (127)      115 2024-05-29 14:08:34.000000 unidist-0.7.0/unidist/core/backends/dask/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6692 2024-05-29 14:08:34.000000 unidist-0.7.0/unidist/core/backends/dask/actor.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5526 2024-05-29 14:08:34.000000 unidist-0.7.0/unidist/core/backends/dask/backend.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3460 2024-05-29 14:08:34.000000 unidist-0.7.0/unidist/core/backends/dask/remote_function.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1078 2024-05-29 14:08:34.000000 unidist-0.7.0/unidist/core/backends/dask/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-29 14:08:39.257344 unidist-0.7.0/unidist/core/backends/mpi/
+-rw-r--r--   0 runner    (1001) docker     (127)      114 2024-05-29 14:08:34.000000 unidist-0.7.0/unidist/core/backends/mpi/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5692 2024-05-29 14:08:34.000000 unidist-0.7.0/unidist/core/backends/mpi/actor.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4668 2024-05-29 14:08:34.000000 unidist-0.7.0/unidist/core/backends/mpi/backend.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-29 14:08:39.257344 unidist-0.7.0/unidist/core/backends/mpi/core/
+-rwxr-xr-x   0 runner    (1001) docker     (127)      408 2024-05-29 14:08:34.000000 unidist-0.7.0/unidist/core/backends/mpi/core/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1965 2024-05-29 14:08:34.000000 unidist-0.7.0/unidist/core/backends/mpi/core/async_operations.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)    15186 2024-05-29 14:08:34.000000 unidist-0.7.0/unidist/core/backends/mpi/core/common.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)    34133 2024-05-29 14:08:34.000000 unidist-0.7.0/unidist/core/backends/mpi/core/communication.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-29 14:08:39.257344 unidist-0.7.0/unidist/core/backends/mpi/core/controller/
+-rw-r--r--   0 runner    (1001) docker     (127)      533 2024-05-29 14:08:34.000000 unidist-0.7.0/unidist/core/backends/mpi/core/controller/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6575 2024-05-29 14:08:34.000000 unidist-0.7.0/unidist/core/backends/mpi/core/controller/actor.py
+-rw-r--r--   0 runner    (1001) docker     (127)    19455 2024-05-29 14:08:34.000000 unidist-0.7.0/unidist/core/backends/mpi/core/controller/api.py
+-rw-r--r--   0 runner    (1001) docker     (127)    14065 2024-05-29 14:08:34.000000 unidist-0.7.0/unidist/core/backends/mpi/core/controller/common.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5457 2024-05-29 14:08:34.000000 unidist-0.7.0/unidist/core/backends/mpi/core/controller/garbage_collector.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9355 2024-05-29 14:08:34.000000 unidist-0.7.0/unidist/core/backends/mpi/core/local_object_store.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-29 14:08:39.261344 unidist-0.7.0/unidist/core/backends/mpi/core/memory/
+-rw-r--r--   0 runner    (1001) docker     (127)  1034260 2024-05-29 14:08:39.000000 unidist-0.7.0/unidist/core/backends/mpi/core/memory/_memory.cpp
+-rw-r--r--   0 runner    (1001) docker     (127)      980 2024-05-29 14:08:34.000000 unidist-0.7.0/unidist/core/backends/mpi/core/memory/_memory.pyx
+-rw-r--r--   0 runner    (1001) docker     (127)      558 2024-05-29 14:08:34.000000 unidist-0.7.0/unidist/core/backends/mpi/core/memory/memory.pxd
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-29 14:08:39.261344 unidist-0.7.0/unidist/core/backends/mpi/core/monitor/
+-rw-r--r--   0 runner    (1001) docker     (127)      143 2024-05-29 14:08:34.000000 unidist-0.7.0/unidist/core/backends/mpi/core/monitor/__init__.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)    10227 2024-05-29 14:08:34.000000 unidist-0.7.0/unidist/core/backends/mpi/core/monitor/loop.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7983 2024-05-29 14:08:34.000000 unidist-0.7.0/unidist/core/backends/mpi/core/monitor/shared_memory_manager.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2676 2024-05-29 14:08:34.000000 unidist-0.7.0/unidist/core/backends/mpi/core/object_store.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)    10559 2024-05-29 14:08:34.000000 unidist-0.7.0/unidist/core/backends/mpi/core/serialization.py
+-rw-r--r--   0 runner    (1001) docker     (127)    31718 2024-05-29 14:08:34.000000 unidist-0.7.0/unidist/core/backends/mpi/core/shared_object_store.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-29 14:08:39.261344 unidist-0.7.0/unidist/core/backends/mpi/core/worker/
+-rw-r--r--   0 runner    (1001) docker     (127)      142 2024-05-29 14:08:34.000000 unidist-0.7.0/unidist/core/backends/mpi/core/worker/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9495 2024-05-29 14:08:34.000000 unidist-0.7.0/unidist/core/backends/mpi/core/worker/loop.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9827 2024-05-29 14:08:34.000000 unidist-0.7.0/unidist/core/backends/mpi/core/worker/request_store.py
+-rw-r--r--   0 runner    (1001) docker     (127)    18303 2024-05-29 14:08:34.000000 unidist-0.7.0/unidist/core/backends/mpi/core/worker/task_store.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3331 2024-05-29 14:08:34.000000 unidist-0.7.0/unidist/core/backends/mpi/remote_function.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1008 2024-05-29 14:08:34.000000 unidist-0.7.0/unidist/core/backends/mpi/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-29 14:08:39.261344 unidist-0.7.0/unidist/core/backends/pymp/
+-rw-r--r--   0 runner    (1001) docker     (127)      133 2024-05-29 14:08:34.000000 unidist-0.7.0/unidist/core/backends/pymp/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4336 2024-05-29 14:08:34.000000 unidist-0.7.0/unidist/core/backends/pymp/actor.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4815 2024-05-29 14:08:34.000000 unidist-0.7.0/unidist/core/backends/pymp/backend.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-29 14:08:39.261344 unidist-0.7.0/unidist/core/backends/pymp/core/
+-rw-r--r--   0 runner    (1001) docker     (127)      305 2024-05-29 14:08:34.000000 unidist-0.7.0/unidist/core/backends/pymp/core/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4701 2024-05-29 14:08:34.000000 unidist-0.7.0/unidist/core/backends/pymp/core/actor.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4067 2024-05-29 14:08:34.000000 unidist-0.7.0/unidist/core/backends/pymp/core/api.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4268 2024-05-29 14:08:34.000000 unidist-0.7.0/unidist/core/backends/pymp/core/object_store.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6900 2024-05-29 14:08:34.000000 unidist-0.7.0/unidist/core/backends/pymp/core/process_manager.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3004 2024-05-29 14:08:34.000000 unidist-0.7.0/unidist/core/backends/pymp/remote_function.py
+-rw-r--r--   0 runner    (1001) docker     (127)      506 2024-05-29 14:08:34.000000 unidist-0.7.0/unidist/core/backends/pymp/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-29 14:08:39.265344 unidist-0.7.0/unidist/core/backends/pyseq/
+-rw-r--r--   0 runner    (1001) docker     (127)      128 2024-05-29 14:08:34.000000 unidist-0.7.0/unidist/core/backends/pyseq/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4225 2024-05-29 14:08:34.000000 unidist-0.7.0/unidist/core/backends/pyseq/actor.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4609 2024-05-29 14:08:34.000000 unidist-0.7.0/unidist/core/backends/pyseq/backend.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-29 14:08:39.265344 unidist-0.7.0/unidist/core/backends/pyseq/core/
+-rw-r--r--   0 runner    (1001) docker     (127)      252 2024-05-29 14:08:34.000000 unidist-0.7.0/unidist/core/backends/pyseq/core/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3060 2024-05-29 14:08:34.000000 unidist-0.7.0/unidist/core/backends/pyseq/core/api.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2313 2024-05-29 14:08:34.000000 unidist-0.7.0/unidist/core/backends/pyseq/core/object_store.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2905 2024-05-29 14:08:34.000000 unidist-0.7.0/unidist/core/backends/pyseq/remote_function.py
+-rw-r--r--   0 runner    (1001) docker     (127)      382 2024-05-29 14:08:34.000000 unidist-0.7.0/unidist/core/backends/pyseq/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-29 14:08:39.265344 unidist-0.7.0/unidist/core/backends/ray/
+-rw-r--r--   0 runner    (1001) docker     (127)      114 2024-05-29 14:08:34.000000 unidist-0.7.0/unidist/core/backends/ray/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5544 2024-05-29 14:08:34.000000 unidist-0.7.0/unidist/core/backends/ray/actor.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4616 2024-05-29 14:08:34.000000 unidist-0.7.0/unidist/core/backends/ray/backend.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2742 2024-05-29 14:08:34.000000 unidist-0.7.0/unidist/core/backends/ray/remote_function.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4778 2024-05-29 14:08:34.000000 unidist-0.7.0/unidist/core/backends/ray/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-29 14:08:39.265344 unidist-0.7.0/unidist/core/base/
+-rw-r--r--   0 runner    (1001) docker     (127)      112 2024-05-29 14:08:34.000000 unidist-0.7.0/unidist/core/base/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6620 2024-05-29 14:08:34.000000 unidist-0.7.0/unidist/core/base/actor.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10573 2024-05-29 14:08:34.000000 unidist-0.7.0/unidist/core/base/backend.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1255 2024-05-29 14:08:34.000000 unidist-0.7.0/unidist/core/base/common.py
+-rw-r--r--   0 runner    (1001) docker     (127)      384 2024-05-29 14:08:34.000000 unidist-0.7.0/unidist/core/base/object_ref.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3105 2024-05-29 14:08:34.000000 unidist-0.7.0/unidist/core/base/remote_function.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3330 2024-05-29 14:08:34.000000 unidist-0.7.0/unidist/core/base/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-29 14:08:39.265344 unidist-0.7.0/unidist/test/
+-rw-r--r--   0 runner    (1001) docker     (127)       80 2024-05-29 14:08:34.000000 unidist-0.7.0/unidist/test/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4174 2024-05-29 14:08:34.000000 unidist-0.7.0/unidist/test/test_actor.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6039 2024-05-29 14:08:34.000000 unidist-0.7.0/unidist/test/test_async_actor.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2555 2024-05-29 14:08:34.000000 unidist-0.7.0/unidist/test/test_general.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2939 2024-05-29 14:08:34.000000 unidist-0.7.0/unidist/test/test_task.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2276 2024-05-29 14:08:34.000000 unidist-0.7.0/unidist/test/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-29 14:08:39.253344 unidist-0.7.0/unidist.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     7106 2024-05-29 14:08:39.000000 unidist-0.7.0/unidist.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     3739 2024-05-29 14:08:39.000000 unidist-0.7.0/unidist.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-29 14:08:39.000000 unidist-0.7.0/unidist.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      273 2024-05-29 14:08:39.000000 unidist-0.7.0/unidist.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        8 2024-05-29 14:08:39.000000 unidist-0.7.0/unidist.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)    86854 2024-05-29 14:08:34.000000 unidist-0.7.0/versioneer.py
```

### Comparing `unidist-0.6.0/AUTHORS` & `unidist-0.7.0/AUTHORS`

 * *Files identical despite different names*

### Comparing `unidist-0.6.0/LICENSE` & `unidist-0.7.0/LICENSE`

 * *Files identical despite different names*

### Comparing `unidist-0.6.0/PKG-INFO` & `unidist-0.7.0/PKG-INFO`

 * *Files 14% similar despite different names*

```diff
@@ -1,37 +1,21 @@
 Metadata-Version: 2.1
 Name: unidist
-Version: 0.6.0
+Version: 0.7.0
 Summary: Unified Distributed Execution
 Home-page: https://github.com/modin-project/unidist
 License: Apache-2.0
-Requires-Python: >=3.7.1
+Requires-Python: >=3.9
 Description-Content-Type: text/markdown
-License-File: LICENSE
-License-File: AUTHORS
-Requires-Dist: packaging
-Requires-Dist: cloudpickle
 Provides-Extra: ray
-Requires-Dist: ray[default]>=1.13.0; extra == "ray"
-Requires-Dist: pydantic<2; extra == "ray"
 Provides-Extra: dask
-Requires-Dist: dask[complete]>=2.22.0; extra == "dask"
-Requires-Dist: distributed>=2.22.0; extra == "dask"
 Provides-Extra: mpi
-Requires-Dist: mpi4py>=3.0.3; extra == "mpi"
-Requires-Dist: msgpack>=1.0.0; extra == "mpi"
-Requires-Dist: psutil; extra == "mpi"
 Provides-Extra: all
-Requires-Dist: ray[default]>=1.13.0; extra == "all"
-Requires-Dist: pydantic<2; extra == "all"
-Requires-Dist: dask[complete]>=2.22.0; extra == "all"
-Requires-Dist: distributed>=2.22.0; extra == "all"
-Requires-Dist: mpi4py>=3.0.3; extra == "all"
-Requires-Dist: msgpack>=1.0.0; extra == "all"
-Requires-Dist: psutil; extra == "all"
+License-File: LICENSE
+License-File: AUTHORS
 
 <p align="center">
     <a href="https://unidist.readthedocs.io"><img alt="" src="https://github.com/modin-project/unidist/blob/d17f0da551846277c9d56a7f5e7d8f244c09d660/docs/img/unidist-logo-simple-628x128.png?raw=true"></a>
 </p>
 <h2 align="center">Unified Distributed Execution</h2>
 
 <p align="center">
```

### Comparing `unidist-0.6.0/README.md` & `unidist-0.7.0/README.md`

 * *Files identical despite different names*

### Comparing `unidist-0.6.0/unidist/__init__.py` & `unidist-0.7.0/unidist/__init__.py`

 * *Files 23% similar despite different names*

```diff
@@ -13,15 +13,15 @@
     get,
     wait,
     is_object_ref,
     get_ip,
     num_cpus,
     cluster_resources,
 )
-from ._version import get_versions
+from . import _version
 
 __all__ = [
     "init",
     "is_initialized",
     "shutdown",
     "remote",
     "put",
@@ -29,9 +29,8 @@
     "wait",
     "is_object_ref",
     "get_ip",
     "num_cpus",
     "cluster_resources",
 ]
 
-__version__ = get_versions()["version"]
-del get_versions
+__version__ = _version.get_versions()["version"]
```

### Comparing `unidist-0.6.0/unidist/api.py` & `unidist-0.7.0/unidist/api.py`

 * *Files identical despite different names*

### Comparing `unidist-0.6.0/unidist/config/__init__.py` & `unidist-0.7.0/unidist/config/__init__.py`

 * *Files identical despite different names*

### Comparing `unidist-0.6.0/unidist/config/backends/common/envvars.py` & `unidist-0.7.0/unidist/config/backends/common/envvars.py`

 * *Files identical despite different names*

### Comparing `unidist-0.6.0/unidist/config/backends/dask/envvars.py` & `unidist-0.7.0/unidist/config/backends/dask/envvars.py`

 * *Files identical despite different names*

### Comparing `unidist-0.6.0/unidist/config/backends/mpi/__init__.py` & `unidist-0.7.0/unidist/config/backends/mpi/__init__.py`

 * *Files identical despite different names*

### Comparing `unidist-0.6.0/unidist/config/backends/mpi/envvars.py` & `unidist-0.7.0/unidist/config/backends/mpi/envvars.py`

 * *Files identical despite different names*

### Comparing `unidist-0.6.0/unidist/config/backends/ray/envvars.py` & `unidist-0.7.0/unidist/config/backends/ray/envvars.py`

 * *Files identical despite different names*

### Comparing `unidist-0.6.0/unidist/config/parameter.py` & `unidist-0.7.0/unidist/config/parameter.py`

 * *Files identical despite different names*

### Comparing `unidist-0.6.0/unidist/core/backends/common/data_id.py` & `unidist-0.7.0/unidist/core/backends/common/data_id.py`

 * *Files identical despite different names*

### Comparing `unidist-0.6.0/unidist/core/backends/common/utils.py` & `unidist-0.7.0/unidist/core/backends/common/utils.py`

 * *Files identical despite different names*

### Comparing `unidist-0.6.0/unidist/core/backends/dask/actor.py` & `unidist-0.7.0/unidist/core/backends/dask/actor.py`

 * *Files identical despite different names*

### Comparing `unidist-0.6.0/unidist/core/backends/dask/backend.py` & `unidist-0.7.0/unidist/core/backends/dask/backend.py`

 * *Files identical despite different names*

### Comparing `unidist-0.6.0/unidist/core/backends/dask/remote_function.py` & `unidist-0.7.0/unidist/core/backends/dask/remote_function.py`

 * *Files identical despite different names*

### Comparing `unidist-0.6.0/unidist/core/backends/dask/utils.py` & `unidist-0.7.0/unidist/core/backends/dask/utils.py`

 * *Files identical despite different names*

### Comparing `unidist-0.6.0/unidist/core/backends/mpi/actor.py` & `unidist-0.7.0/unidist/core/backends/mpi/actor.py`

 * *Files identical despite different names*

### Comparing `unidist-0.6.0/unidist/core/backends/mpi/backend.py` & `unidist-0.7.0/unidist/core/backends/mpi/backend.py`

 * *Files identical despite different names*

### Comparing `unidist-0.6.0/unidist/core/backends/mpi/core/async_operations.py` & `unidist-0.7.0/unidist/core/backends/mpi/core/async_operations.py`

 * *Files identical despite different names*

### Comparing `unidist-0.6.0/unidist/core/backends/mpi/core/common.py` & `unidist-0.7.0/unidist/core/backends/mpi/core/common.py`

 * *Files identical despite different names*

### Comparing `unidist-0.6.0/unidist/core/backends/mpi/core/communication.py` & `unidist-0.7.0/unidist/core/backends/mpi/core/communication.py`

 * *Files identical despite different names*

### Comparing `unidist-0.6.0/unidist/core/backends/mpi/core/controller/__init__.py` & `unidist-0.7.0/unidist/core/backends/mpi/core/controller/__init__.py`

 * *Files identical despite different names*

### Comparing `unidist-0.6.0/unidist/core/backends/mpi/core/controller/actor.py` & `unidist-0.7.0/unidist/core/backends/mpi/core/controller/actor.py`

 * *Files identical despite different names*

### Comparing `unidist-0.6.0/unidist/core/backends/mpi/core/controller/api.py` & `unidist-0.7.0/unidist/core/backends/mpi/core/controller/api.py`

 * *Files identical despite different names*

### Comparing `unidist-0.6.0/unidist/core/backends/mpi/core/controller/common.py` & `unidist-0.7.0/unidist/core/backends/mpi/core/controller/common.py`

 * *Files identical despite different names*

### Comparing `unidist-0.6.0/unidist/core/backends/mpi/core/controller/garbage_collector.py` & `unidist-0.7.0/unidist/core/backends/mpi/core/controller/garbage_collector.py`

 * *Files identical despite different names*

### Comparing `unidist-0.6.0/unidist/core/backends/mpi/core/local_object_store.py` & `unidist-0.7.0/unidist/core/backends/mpi/core/local_object_store.py`

 * *Files identical despite different names*

### Comparing `unidist-0.6.0/unidist/core/backends/mpi/core/memory/_memory.cpp` & `unidist-0.7.0/unidist/core/backends/mpi/core/memory/_memory.cpp`

 * *Files 0% similar despite different names*

```diff
@@ -1,16 +1,22 @@
-/* Generated by Cython 3.0.5 */
+/* Generated by Cython 3.0.10 */
 
 /* BEGIN: Cython Metadata
 {
     "distutils": {
         "depends": [
             "unidist/core/backends/mpi/core/memory/memory.cpp",
             "unidist/core/backends/mpi/core/memory/memory.h"
         ],
+        "extra_compile_args": [
+            "-std=c++11"
+        ],
+        "extra_link_args": [
+            "-std=c++11"
+        ],
         "include_dirs": [
             "unidist/core/backends/mpi/core/memory"
         ],
         "language": "c++",
         "name": "unidist.core.backends.mpi.core._memory",
         "sources": [
             "unidist/core/backends/mpi/core/memory/_memory.pyx"
@@ -40,18 +46,18 @@
     #error Cython requires Python 2.7+ or Python 3.3+.
 #else
 #if defined(CYTHON_LIMITED_API) && CYTHON_LIMITED_API
 #define __PYX_EXTRA_ABI_MODULE_NAME "limited"
 #else
 #define __PYX_EXTRA_ABI_MODULE_NAME ""
 #endif
-#define CYTHON_ABI "3_0_5" __PYX_EXTRA_ABI_MODULE_NAME
+#define CYTHON_ABI "3_0_10" __PYX_EXTRA_ABI_MODULE_NAME
 #define __PYX_ABI_MODULE_NAME "_cython_" CYTHON_ABI
 #define __PYX_TYPE_MODULE_PREFIX __PYX_ABI_MODULE_NAME "."
-#define CYTHON_HEX_VERSION 0x030005F0
+#define CYTHON_HEX_VERSION 0x03000AF0
 #define CYTHON_FUTURE_DIVISION 1
 #include <stddef.h>
 #ifndef offsetof
   #define offsetof(type, member) ( (size_t) & ((type*)0) -> member )
 #endif
 #if !defined(_WIN32) && !defined(WIN32) && !defined(MS_WINDOWS)
   #ifndef __stdcall
@@ -135,14 +141,16 @@
   #undef CYTHON_USE_DICT_VERSIONS
   #define CYTHON_USE_DICT_VERSIONS 0
   #undef CYTHON_USE_EXC_INFO_STACK
   #define CYTHON_USE_EXC_INFO_STACK 0
   #ifndef CYTHON_UPDATE_DESCRIPTOR_DOC
     #define CYTHON_UPDATE_DESCRIPTOR_DOC 0
   #endif
+  #undef CYTHON_USE_FREELISTS
+  #define CYTHON_USE_FREELISTS 0
 #elif defined(PYPY_VERSION)
   #define CYTHON_COMPILING_IN_PYPY 1
   #define CYTHON_COMPILING_IN_CPYTHON 0
   #define CYTHON_COMPILING_IN_LIMITED_API 0
   #define CYTHON_COMPILING_IN_GRAAL 0
   #define CYTHON_COMPILING_IN_NOGIL 0
   #undef CYTHON_USE_TYPE_SLOTS
@@ -196,14 +204,16 @@
   #undef CYTHON_USE_DICT_VERSIONS
   #define CYTHON_USE_DICT_VERSIONS 0
   #undef CYTHON_USE_EXC_INFO_STACK
   #define CYTHON_USE_EXC_INFO_STACK 0
   #ifndef CYTHON_UPDATE_DESCRIPTOR_DOC
     #define CYTHON_UPDATE_DESCRIPTOR_DOC 0
   #endif
+  #undef CYTHON_USE_FREELISTS
+  #define CYTHON_USE_FREELISTS 0
 #elif defined(CYTHON_LIMITED_API)
   #ifdef Py_LIMITED_API
     #undef __PYX_LIMITED_VERSION_HEX
     #define __PYX_LIMITED_VERSION_HEX Py_LIMITED_API
   #endif
   #define CYTHON_COMPILING_IN_PYPY 0
   #define CYTHON_COMPILING_IN_CPYTHON 0
@@ -257,60 +267,83 @@
   #undef CYTHON_USE_DICT_VERSIONS
   #define CYTHON_USE_DICT_VERSIONS 0
   #undef CYTHON_USE_EXC_INFO_STACK
   #define CYTHON_USE_EXC_INFO_STACK 0
   #ifndef CYTHON_UPDATE_DESCRIPTOR_DOC
     #define CYTHON_UPDATE_DESCRIPTOR_DOC 0
   #endif
-#elif defined(PY_NOGIL)
+  #undef CYTHON_USE_FREELISTS
+  #define CYTHON_USE_FREELISTS 0
+#elif defined(Py_GIL_DISABLED) || defined(Py_NOGIL)
   #define CYTHON_COMPILING_IN_PYPY 0
   #define CYTHON_COMPILING_IN_CPYTHON 0
   #define CYTHON_COMPILING_IN_LIMITED_API 0
   #define CYTHON_COMPILING_IN_GRAAL 0
   #define CYTHON_COMPILING_IN_NOGIL 1
   #ifndef CYTHON_USE_TYPE_SLOTS
     #define CYTHON_USE_TYPE_SLOTS 1
   #endif
+  #ifndef CYTHON_USE_TYPE_SPECS
+    #define CYTHON_USE_TYPE_SPECS 0
+  #endif
   #undef CYTHON_USE_PYTYPE_LOOKUP
   #define CYTHON_USE_PYTYPE_LOOKUP 0
   #ifndef CYTHON_USE_ASYNC_SLOTS
     #define CYTHON_USE_ASYNC_SLOTS 1
   #endif
+  #ifndef CYTHON_USE_PYLONG_INTERNALS
+    #define CYTHON_USE_PYLONG_INTERNALS 0
+  #endif
   #undef CYTHON_USE_PYLIST_INTERNALS
   #define CYTHON_USE_PYLIST_INTERNALS 0
   #ifndef CYTHON_USE_UNICODE_INTERNALS
     #define CYTHON_USE_UNICODE_INTERNALS 1
   #endif
   #undef CYTHON_USE_UNICODE_WRITER
   #define CYTHON_USE_UNICODE_WRITER 0
-  #undef CYTHON_USE_PYLONG_INTERNALS
-  #define CYTHON_USE_PYLONG_INTERNALS 0
   #ifndef CYTHON_AVOID_BORROWED_REFS
     #define CYTHON_AVOID_BORROWED_REFS 0
   #endif
   #ifndef CYTHON_ASSUME_SAFE_MACROS
     #define CYTHON_ASSUME_SAFE_MACROS 1
   #endif
   #ifndef CYTHON_UNPACK_METHODS
     #define CYTHON_UNPACK_METHODS 1
   #endif
   #undef CYTHON_FAST_THREAD_STATE
   #define CYTHON_FAST_THREAD_STATE 0
+  #undef CYTHON_FAST_GIL
+  #define CYTHON_FAST_GIL 0
+  #ifndef CYTHON_METH_FASTCALL
+    #define CYTHON_METH_FASTCALL 1
+  #endif
   #undef CYTHON_FAST_PYCALL
   #define CYTHON_FAST_PYCALL 0
+  #ifndef CYTHON_PEP487_INIT_SUBCLASS
+    #define CYTHON_PEP487_INIT_SUBCLASS 1
+  #endif
   #ifndef CYTHON_PEP489_MULTI_PHASE_INIT
     #define CYTHON_PEP489_MULTI_PHASE_INIT 1
   #endif
+  #ifndef CYTHON_USE_MODULE_STATE
+    #define CYTHON_USE_MODULE_STATE 0
+  #endif
   #ifndef CYTHON_USE_TP_FINALIZE
     #define CYTHON_USE_TP_FINALIZE 1
   #endif
   #undef CYTHON_USE_DICT_VERSIONS
   #define CYTHON_USE_DICT_VERSIONS 0
   #undef CYTHON_USE_EXC_INFO_STACK
   #define CYTHON_USE_EXC_INFO_STACK 0
+  #ifndef CYTHON_UPDATE_DESCRIPTOR_DOC
+    #define CYTHON_UPDATE_DESCRIPTOR_DOC 1
+  #endif
+  #ifndef CYTHON_USE_FREELISTS
+    #define CYTHON_USE_FREELISTS 0
+  #endif
 #else
   #define CYTHON_COMPILING_IN_PYPY 0
   #define CYTHON_COMPILING_IN_CPYTHON 1
   #define CYTHON_COMPILING_IN_LIMITED_API 0
   #define CYTHON_COMPILING_IN_GRAAL 0
   #define CYTHON_COMPILING_IN_NOGIL 0
   #ifndef CYTHON_USE_TYPE_SLOTS
@@ -393,14 +426,17 @@
     #define CYTHON_USE_EXC_INFO_STACK 0
   #elif !defined(CYTHON_USE_EXC_INFO_STACK)
     #define CYTHON_USE_EXC_INFO_STACK 1
   #endif
   #ifndef CYTHON_UPDATE_DESCRIPTOR_DOC
     #define CYTHON_UPDATE_DESCRIPTOR_DOC 1
   #endif
+  #ifndef CYTHON_USE_FREELISTS
+    #define CYTHON_USE_FREELISTS 1
+  #endif
 #endif
 #if !defined(CYTHON_FAST_PYCCALL)
 #define CYTHON_FAST_PYCCALL  (CYTHON_FAST_PYCALL && PY_VERSION_HEX >= 0x030600B1)
 #endif
 #if !defined(CYTHON_VECTORCALL)
 #define CYTHON_VECTORCALL  (CYTHON_FAST_PYCCALL && PY_VERSION_HEX >= 0x030800B1)
 #endif
@@ -601,26 +637,27 @@
     static CYTHON_INLINE PyObject* __Pyx_PyCode_New(int a, int p, int k, int l, int s, int f,
                                                     PyObject *code, PyObject *c, PyObject* n, PyObject *v,
                                                     PyObject *fv, PyObject *cell, PyObject* fn,
                                                     PyObject *name, int fline, PyObject *lnos) {
         PyObject *exception_table = NULL;
         PyObject *types_module=NULL, *code_type=NULL, *result=NULL;
         #if __PYX_LIMITED_VERSION_HEX < 0x030B0000
-        PyObject *version_info; // borrowed
-        #endif
+        PyObject *version_info;
         PyObject *py_minor_version = NULL;
+        #endif
         long minor_version = 0;
         PyObject *type, *value, *traceback;
         PyErr_Fetch(&type, &value, &traceback);
         #if __PYX_LIMITED_VERSION_HEX >= 0x030B0000
-        minor_version = 11; // we don't yet need to distinguish between versions > 11
+        minor_version = 11;
         #else
         if (!(version_info = PySys_GetObject("version_info"))) goto end;
         if (!(py_minor_version = PySequence_GetItem(version_info, 1))) goto end;
         minor_version = PyLong_AsLong(py_minor_version);
+        Py_DECREF(py_minor_version);
         if (minor_version == -1 && PyErr_Occurred()) goto end;
         #endif
         if (!(types_module = PyImport_ImportModule("types"))) goto end;
         if (!(code_type = PyObject_GetAttrString(types_module, "CodeType"))) goto end;
         if (minor_version <= 7) {
             (void)p;
             result = PyObject_CallFunction(code_type, "iiiiiOOOOOOiOO", a, k, l, s, f, code,
@@ -633,15 +670,14 @@
             result = PyObject_CallFunction(code_type, "iiiiiiOOOOOOOiOO", a,p, k, l, s, f, code,
                           c, n, v, fn, name, name, fline, lnos, exception_table, fv, cell);
         }
     end:
         Py_XDECREF(code_type);
         Py_XDECREF(exception_table);
         Py_XDECREF(types_module);
-        Py_XDECREF(py_minor_version);
         if (type) {
             PyErr_Restore(type, value, traceback);
         }
         return result;
     }
     #ifndef CO_OPTIMIZED
     #define CO_OPTIMIZED 0x0001
@@ -666,15 +702,15 @@
     #endif
 #elif PY_VERSION_HEX >= 0x030B0000
   static CYTHON_INLINE PyCodeObject* __Pyx_PyCode_New(int a, int p, int k, int l, int s, int f,
                                                     PyObject *code, PyObject *c, PyObject* n, PyObject *v,
                                                     PyObject *fv, PyObject *cell, PyObject* fn,
                                                     PyObject *name, int fline, PyObject *lnos) {
     PyCodeObject *result;
-    PyObject *empty_bytes = PyBytes_FromStringAndSize("", 0);  // we don't have access to __pyx_empty_bytes here
+    PyObject *empty_bytes = PyBytes_FromStringAndSize("", 0);
     if (!empty_bytes) return NULL;
     result =
       #if PY_VERSION_HEX >= 0x030C0000
         PyUnstable_Code_NewWithPosOnlyArgs
       #else
         PyCode_NewWithPosOnlyArgs
       #endif
@@ -752,16 +788,21 @@
   #ifndef METH_FASTCALL
      #define METH_FASTCALL 0x80
   #endif
   typedef PyObject *(*__Pyx_PyCFunctionFast) (PyObject *self, PyObject *const *args, Py_ssize_t nargs);
   typedef PyObject *(*__Pyx_PyCFunctionFastWithKeywords) (PyObject *self, PyObject *const *args,
                                                           Py_ssize_t nargs, PyObject *kwnames);
 #else
-  #define __Pyx_PyCFunctionFast _PyCFunctionFast
-  #define __Pyx_PyCFunctionFastWithKeywords _PyCFunctionFastWithKeywords
+  #if PY_VERSION_HEX >= 0x030d00A4
+  #  define __Pyx_PyCFunctionFast PyCFunctionFast
+  #  define __Pyx_PyCFunctionFastWithKeywords PyCFunctionFastWithKeywords
+  #else
+  #  define __Pyx_PyCFunctionFast _PyCFunctionFast
+  #  define __Pyx_PyCFunctionFastWithKeywords _PyCFunctionFastWithKeywords
+  #endif
 #endif
 #if CYTHON_METH_FASTCALL
   #define __Pyx_METH_FASTCALL METH_FASTCALL
   #define __Pyx_PyCFunction_FastCall __Pyx_PyCFunctionFast
   #define __Pyx_PyCFunction_FastCallWithKeywords __Pyx_PyCFunctionFastWithKeywords
 #else
   #define __Pyx_METH_FASTCALL METH_VARARGS
@@ -961,15 +1002,15 @@
 #if CYTHON_COMPILING_IN_LIMITED_API
   #define __Pyx_SetItemOnTypeDict(tp, k, v) PyObject_GenericSetAttr((PyObject*)tp, k, v)
 #else
   #define __Pyx_SetItemOnTypeDict(tp, k, v) PyDict_SetItem(tp->tp_dict, k, v)
 #endif
 #if CYTHON_USE_TYPE_SPECS && PY_VERSION_HEX >= 0x03080000
 #define __Pyx_PyHeapTypeObject_GC_Del(obj)  {\
-    PyTypeObject *type = Py_TYPE(obj);\
+    PyTypeObject *type = Py_TYPE((PyObject*)obj);\
     assert(__Pyx_PyType_HasFeature(type, Py_TPFLAGS_HEAPTYPE));\
     PyObject_GC_Del(obj);\
     Py_DECREF(type);\
 }
 #else
 #define __Pyx_PyHeapTypeObject_GC_Del(obj)  PyObject_GC_Del(obj)
 #endif
@@ -1105,15 +1146,15 @@
   #define __Pyx_PyList_SET_ITEM(o, i, v) PyList_SetItem(o, i, v)
   #define __Pyx_PyTuple_GET_SIZE(o) PyTuple_Size(o)
   #define __Pyx_PyList_GET_SIZE(o) PyList_Size(o)
   #define __Pyx_PySet_GET_SIZE(o) PySet_Size(o)
   #define __Pyx_PyBytes_GET_SIZE(o) PyBytes_Size(o)
   #define __Pyx_PyByteArray_GET_SIZE(o) PyByteArray_Size(o)
 #endif
-#if PY_VERSION_HEX >= 0x030d00A1
+#if __PYX_LIMITED_VERSION_HEX >= 0x030d00A1
   #define __Pyx_PyImport_AddModuleRef(name) PyImport_AddModuleRef(name)
 #else
   static CYTHON_INLINE PyObject *__Pyx_PyImport_AddModuleRef(const char *name) {
       PyObject *module = PyImport_AddModule(name);
       Py_XINCREF(module);
       return module;
   }
@@ -1192,15 +1233,15 @@
 #if defined(__CYGWIN__) && defined(_LDBL_EQ_DBL)
 #define __Pyx_truncl trunc
 #else
 #define __Pyx_truncl truncl
 #endif
 
 #define __PYX_MARK_ERR_POS(f_index, lineno) \
-    { __pyx_filename = __pyx_f[f_index]; (void)__pyx_filename; __pyx_lineno = lineno; (void)__pyx_lineno; __pyx_clineno = __LINE__; (void)__pyx_clineno; }
+    { __pyx_filename = __pyx_f[f_index]; (void)__pyx_filename; __pyx_lineno = lineno; (void)__pyx_lineno; __pyx_clineno = __LINE__;  (void)__pyx_clineno; }
 #define __PYX_ERR(f_index, lineno, Ln_error) \
     { __PYX_MARK_ERR_POS(f_index, lineno) goto Ln_error; }
 
 #ifdef CYTHON_EXTERN_C
     #undef __PYX_EXTERN_C
     #define __PYX_EXTERN_C CYTHON_EXTERN_C
 #elif defined(__PYX_EXTERN_C)
@@ -1297,32 +1338,15 @@
 #define __Pyx_PyObject_AsSString(s)    ((const signed char*) __Pyx_PyObject_AsString(s))
 #define __Pyx_PyObject_AsUString(s)    ((const unsigned char*) __Pyx_PyObject_AsString(s))
 #define __Pyx_PyObject_FromCString(s)  __Pyx_PyObject_FromString((const char*)s)
 #define __Pyx_PyBytes_FromCString(s)   __Pyx_PyBytes_FromString((const char*)s)
 #define __Pyx_PyByteArray_FromCString(s)   __Pyx_PyByteArray_FromString((const char*)s)
 #define __Pyx_PyStr_FromCString(s)     __Pyx_PyStr_FromString((const char*)s)
 #define __Pyx_PyUnicode_FromCString(s) __Pyx_PyUnicode_FromString((const char*)s)
-#if CYTHON_COMPILING_IN_LIMITED_API
-static CYTHON_INLINE size_t __Pyx_Py_UNICODE_strlen(const wchar_t *u)
-{
-    const wchar_t *u_end = u;
-    while (*u_end++) ;
-    return (size_t)(u_end - u - 1);
-}
-#else
-static CYTHON_INLINE size_t __Pyx_Py_UNICODE_strlen(const Py_UNICODE *u)
-{
-    const Py_UNICODE *u_end = u;
-    while (*u_end++) ;
-    return (size_t)(u_end - u - 1);
-}
-#endif
 #define __Pyx_PyUnicode_FromOrdinal(o)       PyUnicode_FromOrdinal((int)o)
-#define __Pyx_PyUnicode_FromUnicode(u)       PyUnicode_FromUnicode(u, __Pyx_Py_UNICODE_strlen(u))
-#define __Pyx_PyUnicode_FromUnicodeAndLength PyUnicode_FromUnicode
 #define __Pyx_PyUnicode_AsUnicode            PyUnicode_AsUnicode
 #define __Pyx_NewRef(obj) (Py_INCREF(obj), obj)
 #define __Pyx_Owned_Py_None(b) __Pyx_NewRef(Py_None)
 static CYTHON_INLINE PyObject * __Pyx_PyBool_FromLong(long b);
 static CYTHON_INLINE int __Pyx_PyObject_IsTrue(PyObject*);
 static CYTHON_INLINE int __Pyx_PyObject_IsTrueAndDecref(PyObject*);
 static CYTHON_INLINE PyObject* __Pyx_PyNumber_IntOrLong(PyObject* x);
@@ -1364,15 +1388,15 @@
     #define __Pyx_PyLong_CompactValue(x)  PyUnstable_Long_CompactValue((PyLongObject*) x)
   #else
     #define __Pyx_PyLong_IsCompact(x)     (((PyLongObject*)x)->long_value.lv_tag < (2 << _PyLong_NON_SIZE_BITS))
     #define __Pyx_PyLong_CompactValue(x)  ((1 - (Py_ssize_t) __Pyx_PyLong_Sign(x)) * (Py_ssize_t) __Pyx_PyLong_Digits(x)[0])
   #endif
   typedef Py_ssize_t  __Pyx_compact_pylong;
   typedef size_t  __Pyx_compact_upylong;
-  #else  // Py < 3.12
+  #else
   #define __Pyx_PyLong_IsNeg(x)  (Py_SIZE(x) < 0)
   #define __Pyx_PyLong_IsNonNeg(x)  (Py_SIZE(x) >= 0)
   #define __Pyx_PyLong_IsZero(x)  (Py_SIZE(x) == 0)
   #define __Pyx_PyLong_IsPos(x)  (Py_SIZE(x) > 0)
   #define __Pyx_PyLong_CompactValueUnsigned(x)  ((Py_SIZE(x) == 0) ? 0 : __Pyx_PyLong_Digits(x)[0])
   #define __Pyx_PyLong_DigitCount(x)  __Pyx_sst_abs(Py_SIZE(x))
   #define __Pyx_PyLong_SignedDigitCount(x)  Py_SIZE(x)
@@ -1871,33 +1895,34 @@
 #else
     #define __Pyx_Arg_VARARGS(args, i) PyTuple_GetItem(args, i)
 #endif
 #if CYTHON_AVOID_BORROWED_REFS
     #define __Pyx_Arg_NewRef_VARARGS(arg) __Pyx_NewRef(arg)
     #define __Pyx_Arg_XDECREF_VARARGS(arg) Py_XDECREF(arg)
 #else
-    #define __Pyx_Arg_NewRef_VARARGS(arg) arg // no-op
-    #define __Pyx_Arg_XDECREF_VARARGS(arg) // no-op - arg is borrowed
+    #define __Pyx_Arg_NewRef_VARARGS(arg) arg
+    #define __Pyx_Arg_XDECREF_VARARGS(arg)
 #endif
 #define __Pyx_NumKwargs_VARARGS(kwds) PyDict_Size(kwds)
 #define __Pyx_KwValues_VARARGS(args, nargs) NULL
 #define __Pyx_GetKwValue_VARARGS(kw, kwvalues, s) __Pyx_PyDict_GetItemStrWithError(kw, s)
 #define __Pyx_KwargsAsDict_VARARGS(kw, kwvalues) PyDict_Copy(kw)
 #if CYTHON_METH_FASTCALL
     #define __Pyx_Arg_FASTCALL(args, i) args[i]
     #define __Pyx_NumKwargs_FASTCALL(kwds) PyTuple_GET_SIZE(kwds)
     #define __Pyx_KwValues_FASTCALL(args, nargs) ((args) + (nargs))
     static CYTHON_INLINE PyObject * __Pyx_GetKwValue_FASTCALL(PyObject *kwnames, PyObject *const *kwvalues, PyObject *s);
 #if CYTHON_COMPILING_IN_CPYTHON && PY_VERSION_HEX >= 0x030d0000
-    static CYTHON_UNUSED PyObject *__Pyx_KwargsAsDict_FASTCALL(PyObject *kwnames, PyObject *const *kwvalues);
+    CYTHON_UNUSED static PyObject *__Pyx_KwargsAsDict_FASTCALL(PyObject *kwnames, PyObject *const *kwvalues);
   #else
     #define __Pyx_KwargsAsDict_FASTCALL(kw, kwvalues) _PyStack_AsDict(kwvalues, kw)
   #endif
-    #define __Pyx_Arg_NewRef_FASTCALL(arg) arg // no-op, __Pyx_Arg_FASTCALL is direct and this needs
-    #define __Pyx_Arg_XDECREF_FASTCALL(arg)  // no-op - arg was returned from array
+    #define __Pyx_Arg_NewRef_FASTCALL(arg) arg  /* no-op, __Pyx_Arg_FASTCALL is direct and this needs
+                                                   to have the same reference counting */
+    #define __Pyx_Arg_XDECREF_FASTCALL(arg)
 #else
     #define __Pyx_Arg_FASTCALL __Pyx_Arg_VARARGS
     #define __Pyx_NumKwargs_FASTCALL __Pyx_NumKwargs_VARARGS
     #define __Pyx_KwValues_FASTCALL __Pyx_KwValues_VARARGS
     #define __Pyx_GetKwValue_FASTCALL __Pyx_GetKwValue_VARARGS
     #define __Pyx_KwargsAsDict_FASTCALL __Pyx_KwargsAsDict_VARARGS
     #define __Pyx_Arg_NewRef_FASTCALL(arg) __Pyx_Arg_NewRef_VARARGS(arg)
@@ -2502,15 +2527,15 @@
     PyObject *func_code;
     PyObject *func_closure;
 #if PY_VERSION_HEX < 0x030900B1 || CYTHON_COMPILING_IN_LIMITED_API
     PyObject *func_classobj;
 #endif
     void *defaults;
     int defaults_pyobjects;
-    size_t defaults_size;  // used by FusedFunction for copying defaults
+    size_t defaults_size;
     int flags;
     PyObject *defaults_tuple;
     PyObject *defaults_kwdict;
     PyObject *(*defaults_getter)(PyObject *);
     PyObject *func_annotations;
     PyObject *func_is_coroutine;
 } __pyx_CyFunctionObject;
@@ -19580,15 +19605,15 @@
   #if PY_MAJOR_VERSION < 3
   __pyx_m = Py_InitModule4("_memory", __pyx_methods, 0, 0, PYTHON_API_VERSION); Py_XINCREF(__pyx_m);
   if (unlikely(!__pyx_m)) __PYX_ERR(1, 1, __pyx_L1_error)
   #elif CYTHON_USE_MODULE_STATE
   __pyx_t_1 = PyModule_Create(&__pyx_moduledef); if (unlikely(!__pyx_t_1)) __PYX_ERR(1, 1, __pyx_L1_error)
   {
     int add_module_result = PyState_AddModule(__pyx_t_1, &__pyx_moduledef);
-    __pyx_t_1 = 0; /* transfer ownership from __pyx_t_1 to _memory pseudovariable */
+    __pyx_t_1 = 0; /* transfer ownership from __pyx_t_1 to "_memory" pseudovariable */
     if (unlikely((add_module_result < 0))) __PYX_ERR(1, 1, __pyx_L1_error)
     pystate_addmodule_run = 1;
   }
   #else
   __pyx_m = PyModule_Create(&__pyx_moduledef);
   if (unlikely(!__pyx_m)) __PYX_ERR(1, 1, __pyx_L1_error)
   #endif
@@ -20486,22 +20511,22 @@
     {
         if (s == PyTuple_GET_ITEM(kwnames, i)) return kwvalues[i];
     }
     for (i = 0; i < n; i++)
     {
         int eq = __Pyx_PyUnicode_Equals(s, PyTuple_GET_ITEM(kwnames, i), Py_EQ);
         if (unlikely(eq != 0)) {
-            if (unlikely(eq < 0)) return NULL;  // error
+            if (unlikely(eq < 0)) return NULL;
             return kwvalues[i];
         }
     }
-    return NULL;  // not found (no exception set)
+    return NULL;
 }
 #if CYTHON_COMPILING_IN_CPYTHON && PY_VERSION_HEX >= 0x030d0000
-static CYTHON_UNUSED PyObject *__Pyx_KwargsAsDict_FASTCALL(PyObject *kwnames, PyObject *const *kwvalues) {
+CYTHON_UNUSED static PyObject *__Pyx_KwargsAsDict_FASTCALL(PyObject *kwnames, PyObject *const *kwvalues) {
     Py_ssize_t i, nkwargs = PyTuple_GET_SIZE(kwnames);
     PyObject *dict;
     dict = PyDict_New();
     if (unlikely(!dict))
         return NULL;
     for (i=0; i<nkwargs; i++) {
         PyObject *key = PyTuple_GET_ITEM(kwnames, i);
@@ -20603,15 +20628,15 @@
 #endif
         }
         name = first_kw_arg;
         while (*name && (**name != key)) name++;
         if (*name) {
             values[name-argnames] = value;
 #if CYTHON_AVOID_BORROWED_REFS
-            Py_INCREF(value); // transfer ownership of value to values
+            Py_INCREF(value);
             Py_DECREF(key);
 #endif
             key = NULL;
             value = NULL;
             continue;
         }
 #if !CYTHON_AVOID_BORROWED_REFS
@@ -20622,15 +20647,15 @@
         #if PY_MAJOR_VERSION < 3
         if (likely(PyString_Check(key))) {
             while (*name) {
                 if ((CYTHON_COMPILING_IN_PYPY || PyString_GET_SIZE(**name) == PyString_GET_SIZE(key))
                         && _PyString_Eq(**name, key)) {
                     values[name-argnames] = value;
 #if CYTHON_AVOID_BORROWED_REFS
-                    value = NULL;  // ownership transferred to values
+                    value = NULL;
 #endif
                     break;
                 }
                 name++;
             }
             if (*name) continue;
             else {
@@ -20654,15 +20679,15 @@
                 #endif
                     PyUnicode_Compare(**name, key)
                 );
                 if (cmp < 0 && unlikely(PyErr_Occurred())) goto bad;
                 if (cmp == 0) {
                     values[name-argnames] = value;
 #if CYTHON_AVOID_BORROWED_REFS
-                    value = NULL; // ownership transferred to values
+                    value = NULL;
 #endif
                     break;
                 }
                 name++;
             }
             if (*name) continue;
             else {
@@ -21735,15 +21760,15 @@
                     PyErr_Clear();
                 }
             }
             return sm->sq_item(o, i);
         }
     }
 #else
-    if (is_list || PySequence_Check(o)) {
+    if (is_list || !PyMapping_Check(o)) {
         return PySequence_GetItem(o, i);
     }
 #endif
     return __Pyx_GetItemInt_Generic(o, PyInt_FromSsize_t(i));
 }
 
 /* PyObjectCallOneArg */
@@ -22619,19 +22644,15 @@
                     PyErr_Clear();
                 }
             }
             return sm->sq_ass_item(o, i, v);
         }
     }
 #else
-#if CYTHON_COMPILING_IN_PYPY
-    if (is_list || (PySequence_Check(o) && !PyDict_Check(o)))
-#else
-    if (is_list || PySequence_Check(o))
-#endif
+    if (is_list || !PyMapping_Check(o))
     {
         return PySequence_SetItem(o, i, v);
     }
 #endif
     return __Pyx_SetItemInt_Generic(o, PyInt_FromSsize_t(i), v);
 }
 
@@ -23017,46 +23038,46 @@
                 "base class '" __Pyx_FMT_TYPENAME "' is not a heap type", b_name);
             __Pyx_DECREF_TypeName(b_name);
 #if CYTHON_AVOID_BORROWED_REFS
             Py_DECREF(b0);
 #endif
             return -1;
         }
-#if !CYTHON_USE_TYPE_SLOTS
-        if (dictoffset == 0) {
-            PyErr_Format(PyExc_TypeError,
-                "extension type '%s.200s': "
-                "unable to validate whether bases have a __dict__ "
-                "when CYTHON_USE_TYPE_SLOTS is off "
-                "(likely because you are building in the limited API). "
-                "Therefore, all extension types with multiple bases "
-                "must add 'cdef dict __dict__' in this compilation mode",
-                type_name);
-#if CYTHON_AVOID_BORROWED_REFS
-            Py_DECREF(b0);
-#endif
-            return -1;
-        }
-#else
-        if (dictoffset == 0 && b->tp_dictoffset)
+        if (dictoffset == 0)
         {
-            __Pyx_TypeName b_name = __Pyx_PyType_GetName(b);
-            PyErr_Format(PyExc_TypeError,
-                "extension type '%.200s' has no __dict__ slot, "
-                "but base type '" __Pyx_FMT_TYPENAME "' has: "
-                "either add 'cdef dict __dict__' to the extension type "
-                "or add '__slots__ = [...]' to the base type",
-                type_name, b_name);
-            __Pyx_DECREF_TypeName(b_name);
+            Py_ssize_t b_dictoffset = 0;
+#if CYTHON_USE_TYPE_SLOTS || CYTHON_COMPILING_IN_PYPY
+            b_dictoffset = b->tp_dictoffset;
+#else
+            PyObject *py_b_dictoffset = PyObject_GetAttrString((PyObject*)b, "__dictoffset__");
+            if (!py_b_dictoffset) goto dictoffset_return;
+            b_dictoffset = PyLong_AsSsize_t(py_b_dictoffset);
+            Py_DECREF(py_b_dictoffset);
+            if (b_dictoffset == -1 && PyErr_Occurred()) goto dictoffset_return;
+#endif
+            if (b_dictoffset) {
+                {
+                    __Pyx_TypeName b_name = __Pyx_PyType_GetName(b);
+                    PyErr_Format(PyExc_TypeError,
+                        "extension type '%.200s' has no __dict__ slot, "
+                        "but base type '" __Pyx_FMT_TYPENAME "' has: "
+                        "either add 'cdef dict __dict__' to the extension type "
+                        "or add '__slots__ = [...]' to the base type",
+                        type_name, b_name);
+                    __Pyx_DECREF_TypeName(b_name);
+                }
+#if !(CYTHON_USE_TYPE_SLOTS || CYTHON_COMPILING_IN_PYPY)
+              dictoffset_return:
+#endif
 #if CYTHON_AVOID_BORROWED_REFS
-            Py_DECREF(b0);
+                Py_DECREF(b0);
 #endif
-            return -1;
+                return -1;
+            }
         }
-#endif
 #if CYTHON_AVOID_BORROWED_REFS
         Py_DECREF(b0);
 #endif
     }
     return 0;
 }
 #endif
@@ -24327,15 +24348,15 @@
         break;
     case 0:
         self = ((PyCFunctionObject*)cyfunc)->m_self;
         break;
     default:
         return NULL;
     }
-    return ((_PyCFunctionFastWithKeywords)(void(*)(void))def->ml_meth)(self, args, nargs, kwnames);
+    return ((__Pyx_PyCFunctionFastWithKeywords)(void(*)(void))def->ml_meth)(self, args, nargs, kwnames);
 }
 static PyObject * __Pyx_CyFunction_Vectorcall_FASTCALL_KEYWORDS_METHOD(PyObject *func, PyObject *const *args, size_t nargsf, PyObject *kwnames)
 {
     __pyx_CyFunctionObject *cyfunc = (__pyx_CyFunctionObject *)func;
     PyMethodDef* def = ((PyCFunctionObject*)cyfunc)->m_ml;
     PyTypeObject *cls = (PyTypeObject *) __Pyx_CyFunction_GetClassObj(cyfunc);
 #if CYTHON_BACKPORT_VECTORCALL
@@ -24786,15 +24807,15 @@
         py_line,
         __pyx_empty_bytes  /*PyObject *lnotab*/
     );
     Py_DECREF(py_srcfile);
     #else
     py_code = PyCode_NewEmpty(filename, funcname, py_line);
     #endif
-    Py_XDECREF(py_funcname);  // XDECREF since it's only set on Py3 if cline
+    Py_XDECREF(py_funcname);
     return py_code;
 bad:
     Py_XDECREF(py_funcname);
     #if PY_MAJOR_VERSION < 3
     Py_XDECREF(py_srcfile);
     #endif
     return NULL;
```

### Comparing `unidist-0.6.0/unidist/core/backends/mpi/core/monitor/loop.py` & `unidist-0.7.0/unidist/core/backends/mpi/core/monitor/loop.py`

 * *Files identical despite different names*

### Comparing `unidist-0.6.0/unidist/core/backends/mpi/core/monitor/shared_memory_manager.py` & `unidist-0.7.0/unidist/core/backends/mpi/core/monitor/shared_memory_manager.py`

 * *Files 0% similar despite different names*

```diff
@@ -204,21 +204,23 @@
             return
         cleanup_list = self.pending_cleanup + data_id_list
         self.pending_cleanup = []
 
         has_refs = array(
             "B",
             [
-                1
-                if data_id in self._reservation_info
-                and self.shared_store.get_ref_number(
-                    data_id, self._reservation_info[data_id]["service_index"]
+                (
+                    1
+                    if data_id in self._reservation_info
+                    and self.shared_store.get_ref_number(
+                        data_id, self._reservation_info[data_id]["service_index"]
+                    )
+                    > 0
+                    else 0
                 )
-                > 0
-                else 0
                 for data_id in cleanup_list
             ],
         )
 
         if self.monitor_comm is not None:
             all_refs = array("B", [0] * len(has_refs))
             self.monitor_comm.Allreduce(has_refs, all_refs, MPI.MAX)
```

### Comparing `unidist-0.6.0/unidist/core/backends/mpi/core/object_store.py` & `unidist-0.7.0/unidist/core/backends/mpi/core/object_store.py`

 * *Files identical despite different names*

### Comparing `unidist-0.6.0/unidist/core/backends/mpi/core/serialization.py` & `unidist-0.7.0/unidist/core/backends/mpi/core/serialization.py`

 * *Files identical despite different names*

### Comparing `unidist-0.6.0/unidist/core/backends/mpi/core/shared_object_store.py` & `unidist-0.7.0/unidist/core/backends/mpi/core/shared_object_store.py`

 * *Files 2% similar despite different names*

```diff
@@ -226,32 +226,36 @@
                 + "than the available amount of memory."
             )
 
         # Shared memory is allocated only once by the monitor process.
         info = MPI.Info.Create()
         info.Set("alloc_shared_noncontig", "true")
         self.win = MPI.Win.Allocate_shared(
-            self.shared_memory_size * MPI.BYTE.size
-            if mpi_state.is_monitor_process()
-            else 0,
+            (
+                self.shared_memory_size * MPI.BYTE.size
+                if mpi_state.is_monitor_process()
+                else 0
+            ),
             MPI.BYTE.size,
             comm=mpi_state.host_comm,
             info=info,
         )
         self.shared_buffer, _ = self.win.Shared_query(communication.MPIRank.MONITOR)
 
         self.service_info_max_count = (
             self.service_memory_size
             // (self.INFO_SIZE * MPI.LONG.size)
             * self.INFO_SIZE
         )
         self.service_win = MPI.Win.Allocate_shared(
-            self.service_info_max_count * MPI.LONG.size
-            if mpi_state.is_monitor_process()
-            else 0,
+            (
+                self.service_info_max_count * MPI.LONG.size
+                if mpi_state.is_monitor_process()
+                else 0
+            ),
             MPI.LONG.size,
             comm=mpi_state.host_comm,
             info=info,
         )
         service_buffer, _ = self.service_win.Shared_query(communication.MPIRank.MONITOR)
         self.service_shared_buffer = memoryview(service_buffer).cast("l")
         # Set -1 to the service buffer because 0 is a valid value and may be recognized by mistake.
@@ -359,21 +363,21 @@
         Notes
         -----
         This information must be set after writing data to shared memory.
         """
         worker_id, data_number = self._parse_data_id(data_id)
 
         with WinLock(self.service_win):
-            self.service_shared_buffer[
-                service_index + self.FIRST_DATA_INDEX
-            ] = first_index
+            self.service_shared_buffer[service_index + self.FIRST_DATA_INDEX] = (
+                first_index
+            )
             self.service_shared_buffer[service_index + self.REFERENCES_NUMBER] = 1
-            self.service_shared_buffer[
-                service_index + self.DATA_NUMBER_INDEX
-            ] = data_number
+            self.service_shared_buffer[service_index + self.DATA_NUMBER_INDEX] = (
+                data_number
+            )
             self.service_shared_buffer[service_index + self.WORKER_ID_INDEX] = worker_id
 
         self.finalizers.append(
             weakref.finalize(
                 data_id, self._decrement_ref_number, str(data_id), service_index
             )
         )
```

### Comparing `unidist-0.6.0/unidist/core/backends/mpi/core/worker/loop.py` & `unidist-0.7.0/unidist/core/backends/mpi/core/worker/loop.py`

 * *Files identical despite different names*

### Comparing `unidist-0.6.0/unidist/core/backends/mpi/core/worker/request_store.py` & `unidist-0.7.0/unidist/core/backends/mpi/core/worker/request_store.py`

 * *Files identical despite different names*

### Comparing `unidist-0.6.0/unidist/core/backends/mpi/core/worker/task_store.py` & `unidist-0.7.0/unidist/core/backends/mpi/core/worker/task_store.py`

 * *Files identical despite different names*

### Comparing `unidist-0.6.0/unidist/core/backends/mpi/remote_function.py` & `unidist-0.7.0/unidist/core/backends/mpi/remote_function.py`

 * *Files identical despite different names*

### Comparing `unidist-0.6.0/unidist/core/backends/mpi/utils.py` & `unidist-0.7.0/unidist/core/backends/mpi/utils.py`

 * *Files identical despite different names*

### Comparing `unidist-0.6.0/unidist/core/backends/pymp/actor.py` & `unidist-0.7.0/unidist/core/backends/pymp/actor.py`

 * *Files identical despite different names*

### Comparing `unidist-0.6.0/unidist/core/backends/pymp/backend.py` & `unidist-0.7.0/unidist/core/backends/pymp/backend.py`

 * *Files identical despite different names*

### Comparing `unidist-0.6.0/unidist/core/backends/pymp/core/actor.py` & `unidist-0.7.0/unidist/core/backends/pymp/core/actor.py`

 * *Files identical despite different names*

### Comparing `unidist-0.6.0/unidist/core/backends/pymp/core/api.py` & `unidist-0.7.0/unidist/core/backends/pymp/core/api.py`

 * *Files identical despite different names*

### Comparing `unidist-0.6.0/unidist/core/backends/pymp/core/object_store.py` & `unidist-0.7.0/unidist/core/backends/pymp/core/object_store.py`

 * *Files identical despite different names*

### Comparing `unidist-0.6.0/unidist/core/backends/pymp/core/process_manager.py` & `unidist-0.7.0/unidist/core/backends/pymp/core/process_manager.py`

 * *Files identical despite different names*

### Comparing `unidist-0.6.0/unidist/core/backends/pymp/remote_function.py` & `unidist-0.7.0/unidist/core/backends/pymp/remote_function.py`

 * *Files identical despite different names*

### Comparing `unidist-0.6.0/unidist/core/backends/pyseq/actor.py` & `unidist-0.7.0/unidist/core/backends/pyseq/actor.py`

 * *Files identical despite different names*

### Comparing `unidist-0.6.0/unidist/core/backends/pyseq/backend.py` & `unidist-0.7.0/unidist/core/backends/pyseq/backend.py`

 * *Files identical despite different names*

### Comparing `unidist-0.6.0/unidist/core/backends/pyseq/core/api.py` & `unidist-0.7.0/unidist/core/backends/pyseq/core/api.py`

 * *Files identical despite different names*

### Comparing `unidist-0.6.0/unidist/core/backends/pyseq/core/object_store.py` & `unidist-0.7.0/unidist/core/backends/pyseq/core/object_store.py`

 * *Files identical despite different names*

### Comparing `unidist-0.6.0/unidist/core/backends/pyseq/remote_function.py` & `unidist-0.7.0/unidist/core/backends/pyseq/remote_function.py`

 * *Files identical despite different names*

### Comparing `unidist-0.6.0/unidist/core/backends/ray/actor.py` & `unidist-0.7.0/unidist/core/backends/ray/actor.py`

 * *Files identical despite different names*

### Comparing `unidist-0.6.0/unidist/core/backends/ray/backend.py` & `unidist-0.7.0/unidist/core/backends/ray/backend.py`

 * *Files identical despite different names*

### Comparing `unidist-0.6.0/unidist/core/backends/ray/remote_function.py` & `unidist-0.7.0/unidist/core/backends/ray/remote_function.py`

 * *Files identical despite different names*

### Comparing `unidist-0.6.0/unidist/core/backends/ray/utils.py` & `unidist-0.7.0/unidist/core/backends/ray/utils.py`

 * *Files identical despite different names*

### Comparing `unidist-0.6.0/unidist/core/base/actor.py` & `unidist-0.7.0/unidist/core/base/actor.py`

 * *Files identical despite different names*

### Comparing `unidist-0.6.0/unidist/core/base/backend.py` & `unidist-0.7.0/unidist/core/base/backend.py`

 * *Files identical despite different names*

### Comparing `unidist-0.6.0/unidist/core/base/common.py` & `unidist-0.7.0/unidist/core/base/common.py`

 * *Files identical despite different names*

### Comparing `unidist-0.6.0/unidist/core/base/remote_function.py` & `unidist-0.7.0/unidist/core/base/remote_function.py`

 * *Files identical despite different names*

### Comparing `unidist-0.6.0/unidist/core/base/utils.py` & `unidist-0.7.0/unidist/core/base/utils.py`

 * *Files identical despite different names*

### Comparing `unidist-0.6.0/unidist/test/test_actor.py` & `unidist-0.7.0/unidist/test/test_actor.py`

 * *Files identical despite different names*

### Comparing `unidist-0.6.0/unidist/test/test_async_actor.py` & `unidist-0.7.0/unidist/test/test_async_actor.py`

 * *Files identical despite different names*

### Comparing `unidist-0.6.0/unidist/test/test_general.py` & `unidist-0.7.0/unidist/test/test_general.py`

 * *Files identical despite different names*

### Comparing `unidist-0.6.0/unidist/test/test_task.py` & `unidist-0.7.0/unidist/test/test_task.py`

 * *Files identical despite different names*

### Comparing `unidist-0.6.0/unidist/test/utils.py` & `unidist-0.7.0/unidist/test/utils.py`

 * *Files identical despite different names*

### Comparing `unidist-0.6.0/unidist.egg-info/PKG-INFO` & `unidist-0.7.0/unidist.egg-info/PKG-INFO`

 * *Files 14% similar despite different names*

```diff
@@ -1,37 +1,21 @@
 Metadata-Version: 2.1
 Name: unidist
-Version: 0.6.0
+Version: 0.7.0
 Summary: Unified Distributed Execution
 Home-page: https://github.com/modin-project/unidist
 License: Apache-2.0
-Requires-Python: >=3.7.1
+Requires-Python: >=3.9
 Description-Content-Type: text/markdown
-License-File: LICENSE
-License-File: AUTHORS
-Requires-Dist: packaging
-Requires-Dist: cloudpickle
 Provides-Extra: ray
-Requires-Dist: ray[default]>=1.13.0; extra == "ray"
-Requires-Dist: pydantic<2; extra == "ray"
 Provides-Extra: dask
-Requires-Dist: dask[complete]>=2.22.0; extra == "dask"
-Requires-Dist: distributed>=2.22.0; extra == "dask"
 Provides-Extra: mpi
-Requires-Dist: mpi4py>=3.0.3; extra == "mpi"
-Requires-Dist: msgpack>=1.0.0; extra == "mpi"
-Requires-Dist: psutil; extra == "mpi"
 Provides-Extra: all
-Requires-Dist: ray[default]>=1.13.0; extra == "all"
-Requires-Dist: pydantic<2; extra == "all"
-Requires-Dist: dask[complete]>=2.22.0; extra == "all"
-Requires-Dist: distributed>=2.22.0; extra == "all"
-Requires-Dist: mpi4py>=3.0.3; extra == "all"
-Requires-Dist: msgpack>=1.0.0; extra == "all"
-Requires-Dist: psutil; extra == "all"
+License-File: LICENSE
+License-File: AUTHORS
 
 <p align="center">
     <a href="https://unidist.readthedocs.io"><img alt="" src="https://github.com/modin-project/unidist/blob/d17f0da551846277c9d56a7f5e7d8f244c09d660/docs/img/unidist-logo-simple-628x128.png?raw=true"></a>
 </p>
 <h2 align="center">Unified Distributed Execution</h2>
 
 <p align="center">
```

### Comparing `unidist-0.6.0/unidist.egg-info/SOURCES.txt` & `unidist-0.7.0/unidist.egg-info/SOURCES.txt`

 * *Files 0% similar despite different names*

```diff
@@ -49,16 +49,16 @@
 unidist/core/backends/mpi/core/shared_object_store.py
 unidist/core/backends/mpi/core/controller/__init__.py
 unidist/core/backends/mpi/core/controller/actor.py
 unidist/core/backends/mpi/core/controller/api.py
 unidist/core/backends/mpi/core/controller/common.py
 unidist/core/backends/mpi/core/controller/garbage_collector.py
 unidist/core/backends/mpi/core/memory/_memory.cpp
-unidist/core/backends/mpi/core/memory/memory.cpp
-unidist/core/backends/mpi/core/memory/memory.h
+unidist/core/backends/mpi/core/memory/_memory.pyx
+unidist/core/backends/mpi/core/memory/memory.pxd
 unidist/core/backends/mpi/core/monitor/__init__.py
 unidist/core/backends/mpi/core/monitor/loop.py
 unidist/core/backends/mpi/core/monitor/shared_memory_manager.py
 unidist/core/backends/mpi/core/worker/__init__.py
 unidist/core/backends/mpi/core/worker/loop.py
 unidist/core/backends/mpi/core/worker/request_store.py
 unidist/core/backends/mpi/core/worker/task_store.py
```

### Comparing `unidist-0.6.0/versioneer.py` & `unidist-0.7.0/versioneer.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,35 +1,63 @@
-# Version: 0.21
+# Version: 0.29
 
 """The Versioneer - like a rocketeer, but for versions.
 
 The Versioneer
 ==============
 
 * like a rocketeer, but for versions!
 * https://github.com/python-versioneer/python-versioneer
 * Brian Warner
-* License: Public Domain
-* Compatible with: Python 3.6, 3.7, 3.8, 3.9 and pypy3
+* License: Public Domain (Unlicense)
+* Compatible with: Python 3.7, 3.8, 3.9, 3.10, 3.11 and pypy3
 * [![Latest Version][pypi-image]][pypi-url]
 * [![Build Status][travis-image]][travis-url]
 
-This is a tool for managing a recorded version number in distutils-based
+This is a tool for managing a recorded version number in setuptools-based
 python projects. The goal is to remove the tedious and error-prone "update
 the embedded version string" step from your release process. Making a new
 release should be as easy as recording a new tag in your version-control
 system, and maybe making new tarballs.
 
 
 ## Quick Install
 
+Versioneer provides two installation modes. The "classic" vendored mode installs
+a copy of versioneer into your repository. The experimental build-time dependency mode
+is intended to allow you to skip this step and simplify the process of upgrading.
+
+### Vendored mode
+
 * `pip install versioneer` to somewhere in your $PATH
-* add a `[versioneer]` section to your setup.cfg (see [Install](INSTALL.md))
-* run `versioneer install` in your source tree, commit the results
-* Verify version information with `python setup.py version`
+   * A [conda-forge recipe](https://github.com/conda-forge/versioneer-feedstock) is
+     available, so you can also use `conda install -c conda-forge versioneer`
+* add a `[tool.versioneer]` section to your `pyproject.toml` or a
+  `[versioneer]` section to your `setup.cfg` (see [Install](INSTALL.md))
+   * Note that you will need to add `tomli; python_version < "3.11"` to your
+     build-time dependencies if you use `pyproject.toml`
+* run `versioneer install --vendor` in your source tree, commit the results
+* verify version information with `python setup.py version`
+
+### Build-time dependency mode
+
+* `pip install versioneer` to somewhere in your $PATH
+   * A [conda-forge recipe](https://github.com/conda-forge/versioneer-feedstock) is
+     available, so you can also use `conda install -c conda-forge versioneer`
+* add a `[tool.versioneer]` section to your `pyproject.toml` or a
+  `[versioneer]` section to your `setup.cfg` (see [Install](INSTALL.md))
+* add `versioneer` (with `[toml]` extra, if configuring in `pyproject.toml`)
+  to the `requires` key of the `build-system` table in `pyproject.toml`:
+  ```toml
+  [build-system]
+  requires = ["setuptools", "versioneer[toml]"]
+  build-backend = "setuptools.build_meta"
+  ```
+* run `versioneer install --no-vendor` in your source tree, commit the results
+* verify version information with `python setup.py version`
 
 ## Version Identifiers
 
 Source trees come from a variety of places:
 
 * a version-control system checkout (mostly used by developers)
 * a nightly tarball, produced by build automation
@@ -226,17 +254,18 @@
 
 
 ## Updating Versioneer
 
 To upgrade your project to a new release of Versioneer, do the following:
 
 * install the new Versioneer (`pip install -U versioneer` or equivalent)
-* edit `setup.cfg`, if necessary, to include any new configuration settings
-  indicated by the release notes. See [UPGRADING](./UPGRADING.md) for details.
-* re-run `versioneer install` in your source tree, to replace
+* edit `setup.cfg` and `pyproject.toml`, if necessary,
+  to include any new configuration settings indicated by the release notes.
+  See [UPGRADING](./UPGRADING.md) for details.
+* re-run `versioneer install --[no-]vendor` in your source tree, to replace
   `SRC/_version.py`
 * commit any changed files
 
 ## Future Directions
 
 This tool is designed to make it easily extended to other version-control
 systems: all VCS-specific components are in separate directories like
@@ -258,17 +287,16 @@
 * [versioningit](https://github.com/jwodder/versioningit) - a PEP 518-based setuptools
   plugin
 
 ## License
 
 To make Versioneer easier to embed, all its code is dedicated to the public
 domain. The `_version.py` that it creates is also in the public domain.
-Specifically, both are released under the Creative Commons "Public Domain
-Dedication" license (CC0-1.0), as described in
-https://creativecommons.org/publicdomain/zero/1.0/ .
+Specifically, both are released under the "Unlicense", as described in
+https://unlicense.org/.
 
 [pypi-image]: https://img.shields.io/pypi/v/versioneer.svg
 [pypi-url]: https://pypi.python.org/pypi/versioneer/
 [travis-image]:
 https://img.shields.io/travis/com/python-versioneer/python-versioneer.svg
 [travis-url]: https://travis-ci.com/github/python-versioneer/python-versioneer
 
@@ -282,36 +310,66 @@
 import configparser
 import errno
 import json
 import os
 import re
 import subprocess
 import sys
-from typing import Callable, Dict
+from pathlib import Path
+from typing import Any, Callable, cast, Dict, List, Optional, Tuple, Union
+from typing import NoReturn
+import functools
+
+have_tomllib = True
+if sys.version_info >= (3, 11):
+    import tomllib
+else:
+    try:
+        import tomli as tomllib
+    except ImportError:
+        have_tomllib = False
 
 
 class VersioneerConfig:
     """Container for Versioneer configuration parameters."""
 
+    VCS: str
+    style: str
+    tag_prefix: str
+    versionfile_source: str
+    versionfile_build: Optional[str]
+    parentdir_prefix: Optional[str]
+    verbose: Optional[bool]
+
 
-def get_root():
+def get_root() -> str:
     """Get the project root directory.
 
     We require that all commands are run from the project root, i.e. the
     directory that contains setup.py, setup.cfg, and versioneer.py .
     """
     root = os.path.realpath(os.path.abspath(os.getcwd()))
     setup_py = os.path.join(root, "setup.py")
+    pyproject_toml = os.path.join(root, "pyproject.toml")
     versioneer_py = os.path.join(root, "versioneer.py")
-    if not (os.path.exists(setup_py) or os.path.exists(versioneer_py)):
+    if not (
+        os.path.exists(setup_py)
+        or os.path.exists(pyproject_toml)
+        or os.path.exists(versioneer_py)
+    ):
         # allow 'python path/to/setup.py COMMAND'
         root = os.path.dirname(os.path.realpath(os.path.abspath(sys.argv[0])))
         setup_py = os.path.join(root, "setup.py")
+        pyproject_toml = os.path.join(root, "pyproject.toml")
         versioneer_py = os.path.join(root, "versioneer.py")
-    if not (os.path.exists(setup_py) or os.path.exists(versioneer_py)):
+    if not (
+        os.path.exists(setup_py)
+        or os.path.exists(pyproject_toml)
+        or os.path.exists(versioneer_py)
+    ):
         err = (
             "Versioneer was unable to run the project root directory. "
             "Versioneer requires setup.py to be executed from "
             "its immediate directory (like 'python setup.py COMMAND'), "
             "or in a way that lets it use sys.argv[0] to find the root "
             "(like 'python path/to/setup.py COMMAND')."
         )
@@ -322,90 +380,125 @@
         # "versioneer" may be imported multiple times, and python's shared
         # module-import table will cache the first one. So we can't use
         # os.path.dirname(__file__), as that will find whichever
         # versioneer.py was first imported, even in later projects.
         my_path = os.path.realpath(os.path.abspath(__file__))
         me_dir = os.path.normcase(os.path.splitext(my_path)[0])
         vsr_dir = os.path.normcase(os.path.splitext(versioneer_py)[0])
-        if me_dir != vsr_dir:
+        if me_dir != vsr_dir and "VERSIONEER_PEP518" not in globals():
             print(
                 "Warning: build in %s is using versioneer.py from %s"
                 % (os.path.dirname(my_path), versioneer_py)
             )
     except NameError:
         pass
     return root
 
 
-def get_config_from_root(root):
+def get_config_from_root(root: str) -> VersioneerConfig:
     """Read the project setup.cfg file to determine Versioneer config."""
     # This might raise OSError (if setup.cfg is missing), or
     # configparser.NoSectionError (if it lacks a [versioneer] section), or
     # configparser.NoOptionError (if it lacks "VCS="). See the docstring at
     # the top of versioneer.py for instructions on writing your setup.cfg .
-    setup_cfg = os.path.join(root, "setup.cfg")
-    parser = configparser.ConfigParser()
-    with open(setup_cfg, "r") as cfg_file:
-        parser.read_file(cfg_file)
-    VCS = parser.get("versioneer", "VCS")  # mandatory
-
-    # Dict-like interface for non-mandatory entries
-    section = parser["versioneer"]
+    root_pth = Path(root)
+    pyproject_toml = root_pth / "pyproject.toml"
+    setup_cfg = root_pth / "setup.cfg"
+    section: Union[Dict[str, Any], configparser.SectionProxy, None] = None
+    if pyproject_toml.exists() and have_tomllib:
+        try:
+            with open(pyproject_toml, "rb") as fobj:
+                pp = tomllib.load(fobj)
+            section = pp["tool"]["versioneer"]
+        except (tomllib.TOMLDecodeError, KeyError) as e:
+            print(f"Failed to load config from {pyproject_toml}: {e}")
+            print("Try to load it from setup.cfg")
+    if not section:
+        parser = configparser.ConfigParser()
+        with open(setup_cfg) as cfg_file:
+            parser.read_file(cfg_file)
+        parser.get("versioneer", "VCS")  # raise error if missing
+
+        section = parser["versioneer"]
+
+    # `cast`` really shouldn't be used, but its simplest for the
+    # common VersioneerConfig users at the moment. We verify against
+    # `None` values elsewhere where it matters
 
     cfg = VersioneerConfig()
-    cfg.VCS = VCS
+    cfg.VCS = section["VCS"]
     cfg.style = section.get("style", "")
-    cfg.versionfile_source = section.get("versionfile_source")
+    cfg.versionfile_source = cast(str, section.get("versionfile_source"))
     cfg.versionfile_build = section.get("versionfile_build")
-    cfg.tag_prefix = section.get("tag_prefix")
-    if cfg.tag_prefix in ("''", '""'):
+    cfg.tag_prefix = cast(str, section.get("tag_prefix"))
+    if cfg.tag_prefix in ("''", '""', None):
         cfg.tag_prefix = ""
     cfg.parentdir_prefix = section.get("parentdir_prefix")
-    cfg.verbose = section.get("verbose")
+    if isinstance(section, configparser.SectionProxy):
+        # Make sure configparser translates to bool
+        cfg.verbose = section.getboolean("verbose")
+    else:
+        cfg.verbose = section.get("verbose")
+
     return cfg
 
 
 class NotThisMethod(Exception):
     """Exception raised if a method is not valid for the current scenario."""
 
 
 # these dictionaries contain VCS-specific tools
 LONG_VERSION_PY: Dict[str, str] = {}
 HANDLERS: Dict[str, Dict[str, Callable]] = {}
 
 
-def register_vcs_handler(vcs, method):  # decorator
+def register_vcs_handler(vcs: str, method: str) -> Callable:  # decorator
     """Create decorator to mark a method as the handler of a VCS."""
 
-    def decorate(f):
+    def decorate(f: Callable) -> Callable:
         """Store f in HANDLERS[vcs][method]."""
         HANDLERS.setdefault(vcs, {})[method] = f
         return f
 
     return decorate
 
 
-def run_command(commands, args, cwd=None, verbose=False, hide_stderr=False, env=None):
+def run_command(
+    commands: List[str],
+    args: List[str],
+    cwd: Optional[str] = None,
+    verbose: bool = False,
+    hide_stderr: bool = False,
+    env: Optional[Dict[str, str]] = None,
+) -> Tuple[Optional[str], Optional[int]]:
     """Call the given command(s)."""
     assert isinstance(commands, list)
     process = None
+
+    popen_kwargs: Dict[str, Any] = {}
+    if sys.platform == "win32":
+        # This hides the console window if pythonw.exe is used
+        startupinfo = subprocess.STARTUPINFO()
+        startupinfo.dwFlags |= subprocess.STARTF_USESHOWWINDOW
+        popen_kwargs["startupinfo"] = startupinfo
+
     for command in commands:
         try:
             dispcmd = str([command] + args)
             # remember shell=False, so use git.cmd on windows, not just git
             process = subprocess.Popen(
                 [command] + args,
                 cwd=cwd,
                 env=env,
                 stdout=subprocess.PIPE,
                 stderr=(subprocess.PIPE if hide_stderr else None),
+                **popen_kwargs,
             )
             break
-        except OSError:
-            e = sys.exc_info()[1]
+        except OSError as e:
             if e.errno == errno.ENOENT:
                 continue
             if verbose:
                 print("unable to run %s" % dispcmd)
                 print(e)
             return None, None
     else:
@@ -426,28 +519,30 @@
 ] = r'''
 # This file helps to compute a version number in source trees obtained from
 # git-archive tarball (such as those provided by githubs download-from-tag
 # feature). Distribution tarballs (built by setup.py sdist) and build
 # directories (produced by setup.py build) will contain a much shorter file
 # that just contains the computed version number.
 
-# This file is released into the public domain. Generated by
-# versioneer-0.21 (https://github.com/python-versioneer/python-versioneer)
+# This file is released into the public domain.
+# Generated by versioneer-0.29
+# https://github.com/python-versioneer/python-versioneer
 
 """Git implementation of _version.py."""
 
 import errno
 import os
 import re
 import subprocess
 import sys
-from typing import Callable, Dict
+from typing import Any, Callable, Dict, List, Optional, Tuple
+import functools
 
 
-def get_keywords():
+def get_keywords() -> Dict[str, str]:
     """Get the keywords needed to look up the version information."""
     # these strings will be replaced by git during git-archive.
     # setup.py/versioneer.py will grep for the variable names, so they must
     # each be defined on a line of their own. _version.py will just call
     # get_keywords().
     git_refnames = "%(DOLLAR)sFormat:%%d%(DOLLAR)s"
     git_full = "%(DOLLAR)sFormat:%%H%(DOLLAR)s"
@@ -455,16 +550,23 @@
     keywords = {"refnames": git_refnames, "full": git_full, "date": git_date}
     return keywords
 
 
 class VersioneerConfig:
     """Container for Versioneer configuration parameters."""
 
+    VCS: str
+    style: str
+    tag_prefix: str
+    parentdir_prefix: str
+    versionfile_source: str
+    verbose: bool
 
-def get_config():
+
+def get_config() -> VersioneerConfig:
     """Create, populate and return the VersioneerConfig() object."""
     # these strings are filled in when 'setup.py versioneer' creates
     # _version.py
     cfg = VersioneerConfig()
     cfg.VCS = "git"
     cfg.style = "%(STYLE)s"
     cfg.tag_prefix = "%(TAG_PREFIX)s"
@@ -478,41 +580,54 @@
     """Exception raised if a method is not valid for the current scenario."""
 
 
 LONG_VERSION_PY: Dict[str, str] = {}
 HANDLERS: Dict[str, Dict[str, Callable]] = {}
 
 
-def register_vcs_handler(vcs, method):  # decorator
+def register_vcs_handler(vcs: str, method: str) -> Callable:  # decorator
     """Create decorator to mark a method as the handler of a VCS."""
-    def decorate(f):
+    def decorate(f: Callable) -> Callable:
         """Store f in HANDLERS[vcs][method]."""
         if vcs not in HANDLERS:
             HANDLERS[vcs] = {}
         HANDLERS[vcs][method] = f
         return f
     return decorate
 
 
-def run_command(commands, args, cwd=None, verbose=False, hide_stderr=False,
-                env=None):
+def run_command(
+    commands: List[str],
+    args: List[str],
+    cwd: Optional[str] = None,
+    verbose: bool = False,
+    hide_stderr: bool = False,
+    env: Optional[Dict[str, str]] = None,
+) -> Tuple[Optional[str], Optional[int]]:
     """Call the given command(s)."""
     assert isinstance(commands, list)
     process = None
+
+    popen_kwargs: Dict[str, Any] = {}
+    if sys.platform == "win32":
+        # This hides the console window if pythonw.exe is used
+        startupinfo = subprocess.STARTUPINFO()
+        startupinfo.dwFlags |= subprocess.STARTF_USESHOWWINDOW
+        popen_kwargs["startupinfo"] = startupinfo
+
     for command in commands:
         try:
             dispcmd = str([command] + args)
             # remember shell=False, so use git.cmd on windows, not just git
             process = subprocess.Popen([command] + args, cwd=cwd, env=env,
                                        stdout=subprocess.PIPE,
                                        stderr=(subprocess.PIPE if hide_stderr
-                                               else None))
+                                               else None), **popen_kwargs)
             break
-        except OSError:
-            e = sys.exc_info()[1]
+        except OSError as e:
             if e.errno == errno.ENOENT:
                 continue
             if verbose:
                 print("unable to run %%s" %% dispcmd)
                 print(e)
             return None, None
     else:
@@ -524,15 +639,19 @@
         if verbose:
             print("unable to run %%s (error)" %% dispcmd)
             print("stdout was %%s" %% stdout)
         return None, process.returncode
     return stdout, process.returncode
 
 
-def versions_from_parentdir(parentdir_prefix, root, verbose):
+def versions_from_parentdir(
+    parentdir_prefix: str,
+    root: str,
+    verbose: bool,
+) -> Dict[str, Any]:
     """Try to determine the version from the parent directory name.
 
     Source tarballs conventionally unpack into a directory that includes both
     the project name and a version string. We will also support searching up
     two directory levels for an appropriately named parent directory
     """
     rootdirs = []
@@ -549,21 +668,21 @@
     if verbose:
         print("Tried directories %%s but none started with prefix %%s" %%
               (str(rootdirs), parentdir_prefix))
     raise NotThisMethod("rootdir doesn't start with parentdir_prefix")
 
 
 @register_vcs_handler("git", "get_keywords")
-def git_get_keywords(versionfile_abs):
+def git_get_keywords(versionfile_abs: str) -> Dict[str, str]:
     """Extract version information from the given file."""
     # the code embedded in _version.py can just fetch the value of these
     # keywords. When used from setup.py, we don't want to import _version.py,
     # so we do it with a regexp instead. This function is not used from
     # _version.py.
-    keywords = {}
+    keywords: Dict[str, str] = {}
     try:
         with open(versionfile_abs, "r") as fobj:
             for line in fobj:
                 if line.strip().startswith("git_refnames ="):
                     mo = re.search(r'=\s*"(.*)"', line)
                     if mo:
                         keywords["refnames"] = mo.group(1)
@@ -577,15 +696,19 @@
                         keywords["date"] = mo.group(1)
     except OSError:
         pass
     return keywords
 
 
 @register_vcs_handler("git", "keywords")
-def git_versions_from_keywords(keywords, tag_prefix, verbose):
+def git_versions_from_keywords(
+    keywords: Dict[str, str],
+    tag_prefix: str,
+    verbose: bool,
+) -> Dict[str, Any]:
     """Get version information from git keywords."""
     if "refnames" not in keywords:
         raise NotThisMethod("Short version file found")
     date = keywords.get("date")
     if date is not None:
         # Use only the last line.  Previous lines may contain GPG signature
         # information.
@@ -641,51 +764,60 @@
         print("no suitable tags, using unknown + full revision id")
     return {"version": "0+unknown",
             "full-revisionid": keywords["full"].strip(),
             "dirty": False, "error": "no suitable tags", "date": None}
 
 
 @register_vcs_handler("git", "pieces_from_vcs")
-def git_pieces_from_vcs(tag_prefix, root, verbose, runner=run_command):
+def git_pieces_from_vcs(
+    tag_prefix: str,
+    root: str,
+    verbose: bool,
+    runner: Callable = run_command
+) -> Dict[str, Any]:
     """Get version from 'git describe' in the root of the source tree.
 
     This only gets called if the git-archive 'subst' keywords were *not*
     expanded, and _version.py hasn't already been rewritten with a short
     version string, meaning we're inside a checked out source tree.
     """
     GITS = ["git"]
-    TAG_PREFIX_REGEX = "*"
     if sys.platform == "win32":
         GITS = ["git.cmd", "git.exe"]
-        TAG_PREFIX_REGEX = r"\*"
+
+    # GIT_DIR can interfere with correct operation of Versioneer.
+    # It may be intended to be passed to the Versioneer-versioned project,
+    # but that should not change where we get our version from.
+    env = os.environ.copy()
+    env.pop("GIT_DIR", None)
+    runner = functools.partial(runner, env=env)
 
     _, rc = runner(GITS, ["rev-parse", "--git-dir"], cwd=root,
-                   hide_stderr=True)
+                   hide_stderr=not verbose)
     if rc != 0:
         if verbose:
             print("Directory %%s not under git control" %% root)
         raise NotThisMethod("'git rev-parse --git-dir' returned error")
 
     # if there is a tag matching tag_prefix, this yields TAG-NUM-gHEX[-dirty]
     # if there isn't one, this yields HEX[-dirty] (no NUM)
-    describe_out, rc = runner(GITS, ["describe", "--tags", "--dirty",
-                                     "--always", "--long",
-                                     "--match",
-                                     "%%s%%s" %% (tag_prefix, TAG_PREFIX_REGEX)],
-                              cwd=root)
+    describe_out, rc = runner(GITS, [
+        "describe", "--tags", "--dirty", "--always", "--long",
+        "--match", f"{tag_prefix}[[:digit:]]*"
+    ], cwd=root)
     # --long was added in git-1.5.5
     if describe_out is None:
         raise NotThisMethod("'git describe' failed")
     describe_out = describe_out.strip()
     full_out, rc = runner(GITS, ["rev-parse", "HEAD"], cwd=root)
     if full_out is None:
         raise NotThisMethod("'git rev-parse' failed")
     full_out = full_out.strip()
 
-    pieces = {}
+    pieces: Dict[str, Any] = {}
     pieces["long"] = full_out
     pieces["short"] = full_out[:7]  # maybe improved later
     pieces["error"] = None
 
     branch_name, rc = runner(GITS, ["rev-parse", "--abbrev-ref", "HEAD"],
                              cwd=root)
     # --abbrev-ref was added in git-1.6.3
@@ -756,35 +888,35 @@
 
         # commit: short hex revision ID
         pieces["short"] = mo.group(3)
 
     else:
         # HEX: no tags
         pieces["closest-tag"] = None
-        count_out, rc = runner(GITS, ["rev-list", "HEAD", "--count"], cwd=root)
-        pieces["distance"] = int(count_out)  # total number of commits
+        out, rc = runner(GITS, ["rev-list", "HEAD", "--left-right"], cwd=root)
+        pieces["distance"] = len(out.split())  # total number of commits
 
     # commit date: see ISO-8601 comment in git_versions_from_keywords()
     date = runner(GITS, ["show", "-s", "--format=%%ci", "HEAD"], cwd=root)[0].strip()
     # Use only the last line.  Previous lines may contain GPG signature
     # information.
     date = date.splitlines()[-1]
     pieces["date"] = date.strip().replace(" ", "T", 1).replace(" ", "", 1)
 
     return pieces
 
 
-def plus_or_dot(pieces):
+def plus_or_dot(pieces: Dict[str, Any]) -> str:
     """Return a + if we don't already have one, else return a ."""
     if "+" in pieces.get("closest-tag", ""):
         return "."
     return "+"
 
 
-def render_pep440(pieces):
+def render_pep440(pieces: Dict[str, Any]) -> str:
     """Build up version string, with post-release "local version identifier".
 
     Our goal: TAG[+DISTANCE.gHEX[.dirty]] . Note that if you
     get a tagged build and then dirty it, you'll get TAG+0.gHEX.dirty
 
     Exceptions:
     1: no tags. git_describe was just HEX. 0+untagged.DISTANCE.gHEX[.dirty]
@@ -801,15 +933,15 @@
         rendered = "0+untagged.%%d.g%%s" %% (pieces["distance"],
                                           pieces["short"])
         if pieces["dirty"]:
             rendered += ".dirty"
     return rendered
 
 
-def render_pep440_branch(pieces):
+def render_pep440_branch(pieces: Dict[str, Any]) -> str:
     """TAG[[.dev0]+DISTANCE.gHEX[.dirty]] .
 
     The ".dev0" means not master branch. Note that .dev0 sorts backwards
     (a feature branch will appear "older" than the master branch).
 
     Exceptions:
     1: no tags. 0[.dev0]+untagged.DISTANCE.gHEX[.dirty]
@@ -831,49 +963,49 @@
         rendered += "+untagged.%%d.g%%s" %% (pieces["distance"],
                                           pieces["short"])
         if pieces["dirty"]:
             rendered += ".dirty"
     return rendered
 
 
-def pep440_split_post(ver):
+def pep440_split_post(ver: str) -> Tuple[str, Optional[int]]:
     """Split pep440 version string at the post-release segment.
 
     Returns the release segments before the post-release and the
     post-release version number (or -1 if no post-release segment is present).
     """
     vc = str.split(ver, ".post")
     return vc[0], int(vc[1] or 0) if len(vc) == 2 else None
 
 
-def render_pep440_pre(pieces):
+def render_pep440_pre(pieces: Dict[str, Any]) -> str:
     """TAG[.postN.devDISTANCE] -- No -dirty.
 
     Exceptions:
     1: no tags. 0.post0.devDISTANCE
     """
     if pieces["closest-tag"]:
         if pieces["distance"]:
             # update the post release segment
             tag_version, post_version = pep440_split_post(pieces["closest-tag"])
             rendered = tag_version
             if post_version is not None:
-                rendered += ".post%%d.dev%%d" %% (post_version+1, pieces["distance"])
+                rendered += ".post%%d.dev%%d" %% (post_version + 1, pieces["distance"])
             else:
                 rendered += ".post0.dev%%d" %% (pieces["distance"])
         else:
             # no commits, use the tag as the version
             rendered = pieces["closest-tag"]
     else:
         # exception #1
         rendered = "0.post0.dev%%d" %% pieces["distance"]
     return rendered
 
 
-def render_pep440_post(pieces):
+def render_pep440_post(pieces: Dict[str, Any]) -> str:
     """TAG[.postDISTANCE[.dev0]+gHEX] .
 
     The ".dev0" means dirty. Note that .dev0 sorts backwards
     (a dirty tree will appear "older" than the corresponding clean one),
     but you shouldn't be releasing software with -dirty anyways.
 
     Exceptions:
@@ -892,15 +1024,15 @@
         rendered = "0.post%%d" %% pieces["distance"]
         if pieces["dirty"]:
             rendered += ".dev0"
         rendered += "+g%%s" %% pieces["short"]
     return rendered
 
 
-def render_pep440_post_branch(pieces):
+def render_pep440_post_branch(pieces: Dict[str, Any]) -> str:
     """TAG[.postDISTANCE[.dev0]+gHEX[.dirty]] .
 
     The ".dev0" means not master branch.
 
     Exceptions:
     1: no tags. 0.postDISTANCE[.dev0]+gHEX[.dirty]
     """
@@ -921,15 +1053,15 @@
             rendered += ".dev0"
         rendered += "+g%%s" %% pieces["short"]
         if pieces["dirty"]:
             rendered += ".dirty"
     return rendered
 
 
-def render_pep440_old(pieces):
+def render_pep440_old(pieces: Dict[str, Any]) -> str:
     """TAG[.postDISTANCE[.dev0]] .
 
     The ".dev0" means dirty.
 
     Exceptions:
     1: no tags. 0.postDISTANCE[.dev0]
     """
@@ -943,15 +1075,15 @@
         # exception #1
         rendered = "0.post%%d" %% pieces["distance"]
         if pieces["dirty"]:
             rendered += ".dev0"
     return rendered
 
 
-def render_git_describe(pieces):
+def render_git_describe(pieces: Dict[str, Any]) -> str:
     """TAG[-DISTANCE-gHEX][-dirty].
 
     Like 'git describe --tags --dirty --always'.
 
     Exceptions:
     1: no tags. HEX[-dirty]  (note: no 'g' prefix)
     """
@@ -963,15 +1095,15 @@
         # exception #1
         rendered = pieces["short"]
     if pieces["dirty"]:
         rendered += "-dirty"
     return rendered
 
 
-def render_git_describe_long(pieces):
+def render_git_describe_long(pieces: Dict[str, Any]) -> str:
     """TAG-DISTANCE-gHEX[-dirty].
 
     Like 'git describe --tags --dirty --always -long'.
     The distance/hash is unconditional.
 
     Exceptions:
     1: no tags. HEX[-dirty]  (note: no 'g' prefix)
@@ -983,15 +1115,15 @@
         # exception #1
         rendered = pieces["short"]
     if pieces["dirty"]:
         rendered += "-dirty"
     return rendered
 
 
-def render(pieces, style):
+def render(pieces: Dict[str, Any], style: str) -> Dict[str, Any]:
     """Render the given version pieces into the requested style."""
     if pieces["error"]:
         return {"version": "unknown",
                 "full-revisionid": pieces.get("long"),
                 "dirty": None,
                 "error": pieces["error"],
                 "date": None}
@@ -1019,15 +1151,15 @@
         raise ValueError("unknown style '%%s'" %% style)
 
     return {"version": rendered, "full-revisionid": pieces["long"],
             "dirty": pieces["dirty"], "error": None,
             "date": pieces.get("date")}
 
 
-def get_versions():
+def get_versions() -> Dict[str, Any]:
     """Get version information or return default if unable to do so."""
     # I am in _version.py, which lives at ROOT/VERSIONFILE_SOURCE. If we have
     # __file__, we can work backwards from there to the root. Some
     # py2exe/bbfreeze/non-CPython implementations don't do __file__, in which
     # case we can only use expanded keywords.
 
     cfg = get_config()
@@ -1067,21 +1199,21 @@
     return {"version": "0+unknown", "full-revisionid": None,
             "dirty": None,
             "error": "unable to compute version", "date": None}
 '''
 
 
 @register_vcs_handler("git", "get_keywords")
-def git_get_keywords(versionfile_abs):
+def git_get_keywords(versionfile_abs: str) -> Dict[str, str]:
     """Extract version information from the given file."""
     # the code embedded in _version.py can just fetch the value of these
     # keywords. When used from setup.py, we don't want to import _version.py,
     # so we do it with a regexp instead. This function is not used from
     # _version.py.
-    keywords = {}
+    keywords: Dict[str, str] = {}
     try:
         with open(versionfile_abs, "r") as fobj:
             for line in fobj:
                 if line.strip().startswith("git_refnames ="):
                     mo = re.search(r'=\s*"(.*)"', line)
                     if mo:
                         keywords["refnames"] = mo.group(1)
@@ -1095,15 +1227,19 @@
                         keywords["date"] = mo.group(1)
     except OSError:
         pass
     return keywords
 
 
 @register_vcs_handler("git", "keywords")
-def git_versions_from_keywords(keywords, tag_prefix, verbose):
+def git_versions_from_keywords(
+    keywords: Dict[str, str],
+    tag_prefix: str,
+    verbose: bool,
+) -> Dict[str, Any]:
     """Get version information from git keywords."""
     if "refnames" not in keywords:
         raise NotThisMethod("Short version file found")
     date = keywords.get("date")
     if date is not None:
         # Use only the last line.  Previous lines may contain GPG signature
         # information.
@@ -1166,28 +1302,35 @@
         "dirty": False,
         "error": "no suitable tags",
         "date": None,
     }
 
 
 @register_vcs_handler("git", "pieces_from_vcs")
-def git_pieces_from_vcs(tag_prefix, root, verbose, runner=run_command):
+def git_pieces_from_vcs(
+    tag_prefix: str, root: str, verbose: bool, runner: Callable = run_command
+) -> Dict[str, Any]:
     """Get version from 'git describe' in the root of the source tree.
 
     This only gets called if the git-archive 'subst' keywords were *not*
     expanded, and _version.py hasn't already been rewritten with a short
     version string, meaning we're inside a checked out source tree.
     """
     GITS = ["git"]
-    TAG_PREFIX_REGEX = "*"
     if sys.platform == "win32":
         GITS = ["git.cmd", "git.exe"]
-        TAG_PREFIX_REGEX = r"\*"
 
-    _, rc = runner(GITS, ["rev-parse", "--git-dir"], cwd=root, hide_stderr=True)
+    # GIT_DIR can interfere with correct operation of Versioneer.
+    # It may be intended to be passed to the Versioneer-versioned project,
+    # but that should not change where we get our version from.
+    env = os.environ.copy()
+    env.pop("GIT_DIR", None)
+    runner = functools.partial(runner, env=env)
+
+    _, rc = runner(GITS, ["rev-parse", "--git-dir"], cwd=root, hide_stderr=not verbose)
     if rc != 0:
         if verbose:
             print("Directory %s not under git control" % root)
         raise NotThisMethod("'git rev-parse --git-dir' returned error")
 
     # if there is a tag matching tag_prefix, this yields TAG-NUM-gHEX[-dirty]
     # if there isn't one, this yields HEX[-dirty] (no NUM)
@@ -1196,28 +1339,28 @@
         [
             "describe",
             "--tags",
             "--dirty",
             "--always",
             "--long",
             "--match",
-            "%s%s" % (tag_prefix, TAG_PREFIX_REGEX),
+            f"{tag_prefix}[[:digit:]]*",
         ],
         cwd=root,
     )
     # --long was added in git-1.5.5
     if describe_out is None:
         raise NotThisMethod("'git describe' failed")
     describe_out = describe_out.strip()
     full_out, rc = runner(GITS, ["rev-parse", "HEAD"], cwd=root)
     if full_out is None:
         raise NotThisMethod("'git rev-parse' failed")
     full_out = full_out.strip()
 
-    pieces = {}
+    pieces: Dict[str, Any] = {}
     pieces["long"] = full_out
     pieces["short"] = full_out[:7]  # maybe improved later
     pieces["error"] = None
 
     branch_name, rc = runner(GITS, ["rev-parse", "--abbrev-ref", "HEAD"], cwd=root)
     # --abbrev-ref was added in git-1.6.3
     if rc != 0 or branch_name is None:
@@ -1288,47 +1431,48 @@
 
         # commit: short hex revision ID
         pieces["short"] = mo.group(3)
 
     else:
         # HEX: no tags
         pieces["closest-tag"] = None
-        count_out, rc = runner(GITS, ["rev-list", "HEAD", "--count"], cwd=root)
-        pieces["distance"] = int(count_out)  # total number of commits
+        out, rc = runner(GITS, ["rev-list", "HEAD", "--left-right"], cwd=root)
+        pieces["distance"] = len(out.split())  # total number of commits
 
     # commit date: see ISO-8601 comment in git_versions_from_keywords()
     date = runner(GITS, ["show", "-s", "--format=%ci", "HEAD"], cwd=root)[0].strip()
     # Use only the last line.  Previous lines may contain GPG signature
     # information.
     date = date.splitlines()[-1]
     pieces["date"] = date.strip().replace(" ", "T", 1).replace(" ", "", 1)
 
     return pieces
 
 
-def do_vcs_install(manifest_in, versionfile_source, ipy):
+def do_vcs_install(versionfile_source: str, ipy: Optional[str]) -> None:
     """Git-specific installation logic for Versioneer.
 
     For Git, this means creating/changing .gitattributes to mark _version.py
     for export-subst keyword substitution.
     """
     GITS = ["git"]
     if sys.platform == "win32":
         GITS = ["git.cmd", "git.exe"]
-    files = [manifest_in, versionfile_source]
+    files = [versionfile_source]
     if ipy:
         files.append(ipy)
-    try:
-        my_path = __file__
-        if my_path.endswith(".pyc") or my_path.endswith(".pyo"):
-            my_path = os.path.splitext(my_path)[0] + ".py"
-        versioneer_file = os.path.relpath(my_path)
-    except NameError:
-        versioneer_file = "versioneer.py"
-    files.append(versioneer_file)
+    if "VERSIONEER_PEP518" not in globals():
+        try:
+            my_path = __file__
+            if my_path.endswith((".pyc", ".pyo")):
+                my_path = os.path.splitext(my_path)[0] + ".py"
+            versioneer_file = os.path.relpath(my_path)
+        except NameError:
+            versioneer_file = "versioneer.py"
+        files.append(versioneer_file)
     present = False
     try:
         with open(".gitattributes", "r") as fobj:
             for line in fobj:
                 if line.strip().startswith(versionfile_source):
                     if "export-subst" in line.strip().split()[1:]:
                         present = True
@@ -1338,15 +1482,19 @@
     if not present:
         with open(".gitattributes", "a+") as fobj:
             fobj.write(f"{versionfile_source} export-subst\n")
         files.append(".gitattributes")
     run_command(GITS, ["add", "--"] + files)
 
 
-def versions_from_parentdir(parentdir_prefix, root, verbose):
+def versions_from_parentdir(
+    parentdir_prefix: str,
+    root: str,
+    verbose: bool,
+) -> Dict[str, Any]:
     """Try to determine the version from the parent directory name.
 
     Source tarballs conventionally unpack into a directory that includes both
     the project name and a version string. We will also support searching up
     two directory levels for an appropriately named parent directory
     """
     rootdirs = []
@@ -1369,15 +1517,15 @@
             "Tried directories %s but none started with prefix %s"
             % (str(rootdirs), parentdir_prefix)
         )
     raise NotThisMethod("rootdir doesn't start with parentdir_prefix")
 
 
 SHORT_VERSION_PY = """
-# This file was generated by 'versioneer.py' (0.21) from
+# This file was generated by 'versioneer.py' (0.29) from
 # revision-control system data, or from the parent directory name of an
 # unpacked source archive. Distribution tarballs contain a pre-generated copy
 # of this file.
 
 import json
 
 version_json = '''
@@ -1386,15 +1534,15 @@
 
 
 def get_versions():
     return json.loads(version_json)
 """
 
 
-def versions_from_file(filename):
+def versions_from_file(filename: str) -> Dict[str, Any]:
     """Try to determine the version from _version.py if present."""
     try:
         with open(filename) as f:
             contents = f.read()
     except OSError:
         raise NotThisMethod("unable to read _version.py")
     mo = re.search(
@@ -1405,32 +1553,31 @@
             r"version_json = '''\r\n(.*)'''  # END VERSION_JSON", contents, re.M | re.S
         )
     if not mo:
         raise NotThisMethod("no version_json in _version.py")
     return json.loads(mo.group(1))
 
 
-def write_to_version_file(filename, versions):
+def write_to_version_file(filename: str, versions: Dict[str, Any]) -> None:
     """Write the given version number to the given _version.py file."""
-    os.unlink(filename)
     contents = json.dumps(versions, sort_keys=True, indent=1, separators=(",", ": "))
     with open(filename, "w") as f:
         f.write(SHORT_VERSION_PY % contents)
 
     print("set %s to '%s'" % (filename, versions["version"]))
 
 
-def plus_or_dot(pieces):
+def plus_or_dot(pieces: Dict[str, Any]) -> str:
     """Return a + if we don't already have one, else return a ."""
     if "+" in pieces.get("closest-tag", ""):
         return "."
     return "+"
 
 
-def render_pep440(pieces):
+def render_pep440(pieces: Dict[str, Any]) -> str:
     """Build up version string, with post-release "local version identifier".
 
     Our goal: TAG[+DISTANCE.gHEX[.dirty]] . Note that if you
     get a tagged build and then dirty it, you'll get TAG+0.gHEX.dirty
 
     Exceptions:
     1: no tags. git_describe was just HEX. 0+untagged.DISTANCE.gHEX[.dirty]
@@ -1446,15 +1593,15 @@
         # exception #1
         rendered = "0+untagged.%d.g%s" % (pieces["distance"], pieces["short"])
         if pieces["dirty"]:
             rendered += ".dirty"
     return rendered
 
 
-def render_pep440_branch(pieces):
+def render_pep440_branch(pieces: Dict[str, Any]) -> str:
     """TAG[[.dev0]+DISTANCE.gHEX[.dirty]] .
 
     The ".dev0" means not master branch. Note that .dev0 sorts backwards
     (a feature branch will appear "older" than the master branch).
 
     Exceptions:
     1: no tags. 0[.dev0]+untagged.DISTANCE.gHEX[.dirty]
@@ -1475,25 +1622,25 @@
             rendered += ".dev0"
         rendered += "+untagged.%d.g%s" % (pieces["distance"], pieces["short"])
         if pieces["dirty"]:
             rendered += ".dirty"
     return rendered
 
 
-def pep440_split_post(ver):
+def pep440_split_post(ver: str) -> Tuple[str, Optional[int]]:
     """Split pep440 version string at the post-release segment.
 
     Returns the release segments before the post-release and the
     post-release version number (or -1 if no post-release segment is present).
     """
     vc = str.split(ver, ".post")
     return vc[0], int(vc[1] or 0) if len(vc) == 2 else None
 
 
-def render_pep440_pre(pieces):
+def render_pep440_pre(pieces: Dict[str, Any]) -> str:
     """TAG[.postN.devDISTANCE] -- No -dirty.
 
     Exceptions:
     1: no tags. 0.post0.devDISTANCE
     """
     if pieces["closest-tag"]:
         if pieces["distance"]:
@@ -1509,15 +1656,15 @@
             rendered = pieces["closest-tag"]
     else:
         # exception #1
         rendered = "0.post0.dev%d" % pieces["distance"]
     return rendered
 
 
-def render_pep440_post(pieces):
+def render_pep440_post(pieces: Dict[str, Any]) -> str:
     """TAG[.postDISTANCE[.dev0]+gHEX] .
 
     The ".dev0" means dirty. Note that .dev0 sorts backwards
     (a dirty tree will appear "older" than the corresponding clean one),
     but you shouldn't be releasing software with -dirty anyways.
 
     Exceptions:
@@ -1536,15 +1683,15 @@
         rendered = "0.post%d" % pieces["distance"]
         if pieces["dirty"]:
             rendered += ".dev0"
         rendered += "+g%s" % pieces["short"]
     return rendered
 
 
-def render_pep440_post_branch(pieces):
+def render_pep440_post_branch(pieces: Dict[str, Any]) -> str:
     """TAG[.postDISTANCE[.dev0]+gHEX[.dirty]] .
 
     The ".dev0" means not master branch.
 
     Exceptions:
     1: no tags. 0.postDISTANCE[.dev0]+gHEX[.dirty]
     """
@@ -1565,15 +1712,15 @@
             rendered += ".dev0"
         rendered += "+g%s" % pieces["short"]
         if pieces["dirty"]:
             rendered += ".dirty"
     return rendered
 
 
-def render_pep440_old(pieces):
+def render_pep440_old(pieces: Dict[str, Any]) -> str:
     """TAG[.postDISTANCE[.dev0]] .
 
     The ".dev0" means dirty.
 
     Exceptions:
     1: no tags. 0.postDISTANCE[.dev0]
     """
@@ -1587,15 +1734,15 @@
         # exception #1
         rendered = "0.post%d" % pieces["distance"]
         if pieces["dirty"]:
             rendered += ".dev0"
     return rendered
 
 
-def render_git_describe(pieces):
+def render_git_describe(pieces: Dict[str, Any]) -> str:
     """TAG[-DISTANCE-gHEX][-dirty].
 
     Like 'git describe --tags --dirty --always'.
 
     Exceptions:
     1: no tags. HEX[-dirty]  (note: no 'g' prefix)
     """
@@ -1607,15 +1754,15 @@
         # exception #1
         rendered = pieces["short"]
     if pieces["dirty"]:
         rendered += "-dirty"
     return rendered
 
 
-def render_git_describe_long(pieces):
+def render_git_describe_long(pieces: Dict[str, Any]) -> str:
     """TAG-DISTANCE-gHEX[-dirty].
 
     Like 'git describe --tags --dirty --always -long'.
     The distance/hash is unconditional.
 
     Exceptions:
     1: no tags. HEX[-dirty]  (note: no 'g' prefix)
@@ -1627,15 +1774,15 @@
         # exception #1
         rendered = pieces["short"]
     if pieces["dirty"]:
         rendered += "-dirty"
     return rendered
 
 
-def render(pieces, style):
+def render(pieces: Dict[str, Any], style: str) -> Dict[str, Any]:
     """Render the given version pieces into the requested style."""
     if pieces["error"]:
         return {
             "version": "unknown",
             "full-revisionid": pieces.get("long"),
             "dirty": None,
             "error": pieces["error"],
@@ -1673,30 +1820,30 @@
     }
 
 
 class VersioneerBadRootError(Exception):
     """The project root directory is unknown or missing key files."""
 
 
-def get_versions(verbose=False):
+def get_versions(verbose: bool = False) -> Dict[str, Any]:
     """Get the project version from whatever source is available.
 
     Returns dict with two keys: 'version' and 'full'.
     """
     if "versioneer" in sys.modules:
         # see the discussion in cmdclass.py:get_cmdclass()
         del sys.modules["versioneer"]
 
     root = get_root()
     cfg = get_config_from_root(root)
 
     assert cfg.VCS is not None, "please set [versioneer]VCS= in setup.cfg"
     handlers = HANDLERS.get(cfg.VCS)
     assert handlers, "unrecognized VCS '%s'" % cfg.VCS
-    verbose = verbose or cfg.verbose
+    verbose = verbose or bool(cfg.verbose)  # `bool()` used to avoid `None`
     assert (
         cfg.versionfile_source is not None
     ), "please set versioneer.versionfile_source"
     assert cfg.tag_prefix is not None, "please set versioneer.tag_prefix"
 
     versionfile_abs = os.path.join(root, cfg.versionfile_source)
 
@@ -1754,21 +1901,21 @@
         "full-revisionid": None,
         "dirty": None,
         "error": "unable to compute version",
         "date": None,
     }
 
 
-def get_version():
+def get_version() -> str:
     """Get the short version string for this project."""
     return get_versions()["version"]
 
 
-def get_cmdclass(cmdclass=None):
-    """Get the custom setuptools/distutils subclasses used by Versioneer.
+def get_cmdclass(cmdclass: Optional[Dict[str, Any]] = None):
+    """Get the custom setuptools subclasses used by Versioneer.
 
     If the package uses a different cmdclass (e.g. one from numpy), it
     should be provide as an argument.
     """
     if "versioneer" in sys.modules:
         del sys.modules["versioneer"]
         # this fixes the "python setup.py develop" case (also 'install' and
@@ -1782,116 +1929,128 @@
         # parent is protected against the child's "import versioneer". By
         # removing ourselves from sys.modules here, before the child build
         # happens, we protect the child from the parent's versioneer too.
         # Also see https://github.com/python-versioneer/python-versioneer/issues/52
 
     cmds = {} if cmdclass is None else cmdclass.copy()
 
-    # we add "version" to both distutils and setuptools
-    from distutils.core import Command
+    # we add "version" to setuptools
+    from setuptools import Command
 
     class cmd_version(Command):
         description = "report generated version string"
-        user_options = []
-        boolean_options = []
+        user_options: List[Tuple[str, str, str]] = []
+        boolean_options: List[str] = []
 
-        def initialize_options(self):
+        def initialize_options(self) -> None:
             pass
 
-        def finalize_options(self):
+        def finalize_options(self) -> None:
             pass
 
-        def run(self):
+        def run(self) -> None:
             vers = get_versions(verbose=True)
             print("Version: %s" % vers["version"])
             print(" full-revisionid: %s" % vers.get("full-revisionid"))
             print(" dirty: %s" % vers.get("dirty"))
             print(" date: %s" % vers.get("date"))
             if vers["error"]:
                 print(" error: %s" % vers["error"])
 
     cmds["version"] = cmd_version
 
-    # we override "build_py" in both distutils and setuptools
+    # we override "build_py" in setuptools
     #
     # most invocation pathways end up running build_py:
     #  distutils/build -> build_py
     #  distutils/install -> distutils/build ->..
     #  setuptools/bdist_wheel -> distutils/install ->..
     #  setuptools/bdist_egg -> distutils/install_lib -> build_py
     #  setuptools/install -> bdist_egg ->..
     #  setuptools/develop -> ?
     #  pip install:
     #   copies source tree to a tempdir before running egg_info/etc
     #   if .git isn't copied too, 'git describe' will fail
     #   then does setup.py bdist_wheel, or sometimes setup.py install
     #  setup.py egg_info -> ?
 
+    # pip install -e . and setuptool/editable_wheel will invoke build_py
+    # but the build_py command is not expected to copy any files.
+
     # we override different "build_py" commands for both environments
     if "build_py" in cmds:
-        _build_py = cmds["build_py"]
-    elif "setuptools" in sys.modules:
-        from setuptools.command.build_py import build_py as _build_py
+        _build_py: Any = cmds["build_py"]
     else:
-        from distutils.command.build_py import build_py as _build_py
+        from setuptools.command.build_py import build_py as _build_py
 
     class cmd_build_py(_build_py):
-        def run(self):
+        def run(self) -> None:
             root = get_root()
             cfg = get_config_from_root(root)
             versions = get_versions()
             _build_py.run(self)
+            if getattr(self, "editable_mode", False):
+                # During editable installs `.py` and data files are
+                # not copied to build_lib
+                return
             # now locate _version.py in the new build/ directory and replace
             # it with an updated value
             if cfg.versionfile_build:
                 target_versionfile = os.path.join(self.build_lib, cfg.versionfile_build)
                 print("UPDATING %s" % target_versionfile)
                 write_to_version_file(target_versionfile, versions)
 
     cmds["build_py"] = cmd_build_py
 
     if "build_ext" in cmds:
-        _build_ext = cmds["build_ext"]
-    elif "setuptools" in sys.modules:
-        from setuptools.command.build_ext import build_ext as _build_ext
+        _build_ext: Any = cmds["build_ext"]
     else:
-        from distutils.command.build_ext import build_ext as _build_ext
+        from setuptools.command.build_ext import build_ext as _build_ext
 
     class cmd_build_ext(_build_ext):
-        def run(self):
+        def run(self) -> None:
             root = get_root()
             cfg = get_config_from_root(root)
             versions = get_versions()
             _build_ext.run(self)
             if self.inplace:
                 # build_ext --inplace will only build extensions in
                 # build/lib<..> dir with no _version.py to write to.
                 # As in place builds will already have a _version.py
                 # in the module dir, we do not need to write one.
                 return
             # now locate _version.py in the new build/ directory and replace
             # it with an updated value
+            if not cfg.versionfile_build:
+                return
             target_versionfile = os.path.join(self.build_lib, cfg.versionfile_build)
+            if not os.path.exists(target_versionfile):
+                print(
+                    f"Warning: {target_versionfile} does not exist, skipping "
+                    "version update. This can happen if you are running build_ext "
+                    "without first running build_py."
+                )
+                return
             print("UPDATING %s" % target_versionfile)
             write_to_version_file(target_versionfile, versions)
 
     cmds["build_ext"] = cmd_build_ext
 
     if "cx_Freeze" in sys.modules:  # cx_freeze enabled?
-        from cx_Freeze.dist import build_exe as _build_exe
+        from cx_Freeze.dist import build_exe as _build_exe  # type: ignore
 
         # nczeczulin reports that py2exe won't like the pep440-style string
         # as FILEVERSION, but it can be used for PRODUCTVERSION, e.g.
         # setup(console=[{
         #   "version": versioneer.get_version().split("+", 1)[0], # FILEVERSION
         #   "product_version": versioneer.get_version(),
         #   ...
 
         class cmd_build_exe(_build_exe):
-            def run(self):
+            def run(self) -> None:
                 root = get_root()
                 cfg = get_config_from_root(root)
                 versions = get_versions()
                 target_versionfile = cfg.versionfile_source
                 print("UPDATING %s" % target_versionfile)
                 write_to_version_file(target_versionfile, versions)
 
@@ -1910,18 +2069,21 @@
                         }
                     )
 
         cmds["build_exe"] = cmd_build_exe
         del cmds["build_py"]
 
     if "py2exe" in sys.modules:  # py2exe enabled?
-        from py2exe.distutils_buildexe import py2exe as _py2exe
+        try:
+            from py2exe.setuptools_buildexe import py2exe as _py2exe  # type: ignore
+        except ImportError:
+            from py2exe.distutils_buildexe import py2exe as _py2exe  # type: ignore
 
         class cmd_py2exe(_py2exe):
-            def run(self):
+            def run(self) -> None:
                 root = get_root()
                 cfg = get_config_from_root(root)
                 versions = get_versions()
                 target_versionfile = cfg.versionfile_source
                 print("UPDATING %s" % target_versionfile)
                 write_to_version_file(target_versionfile, versions)
 
@@ -1938,32 +2100,70 @@
                             "PARENTDIR_PREFIX": cfg.parentdir_prefix,
                             "VERSIONFILE_SOURCE": cfg.versionfile_source,
                         }
                     )
 
         cmds["py2exe"] = cmd_py2exe
 
+    # sdist farms its file list building out to egg_info
+    if "egg_info" in cmds:
+        _egg_info: Any = cmds["egg_info"]
+    else:
+        from setuptools.command.egg_info import egg_info as _egg_info
+
+    class cmd_egg_info(_egg_info):
+        def find_sources(self) -> None:
+            # egg_info.find_sources builds the manifest list and writes it
+            # in one shot
+            super().find_sources()
+
+            # Modify the filelist and normalize it
+            root = get_root()
+            cfg = get_config_from_root(root)
+            self.filelist.append("versioneer.py")
+            if cfg.versionfile_source:
+                # There are rare cases where versionfile_source might not be
+                # included by default, so we must be explicit
+                self.filelist.append(cfg.versionfile_source)
+            self.filelist.sort()
+            self.filelist.remove_duplicates()
+
+            # The write method is hidden in the manifest_maker instance that
+            # generated the filelist and was thrown away
+            # We will instead replicate their final normalization (to unicode,
+            # and POSIX-style paths)
+            from setuptools import unicode_utils
+
+            normalized = [
+                unicode_utils.filesys_decode(f).replace(os.sep, "/")
+                for f in self.filelist.files
+            ]
+
+            manifest_filename = os.path.join(self.egg_info, "SOURCES.txt")
+            with open(manifest_filename, "w") as fobj:
+                fobj.write("\n".join(normalized))
+
+    cmds["egg_info"] = cmd_egg_info
+
     # we override different "sdist" commands for both environments
     if "sdist" in cmds:
-        _sdist = cmds["sdist"]
-    elif "setuptools" in sys.modules:
-        from setuptools.command.sdist import sdist as _sdist
+        _sdist: Any = cmds["sdist"]
     else:
-        from distutils.command.sdist import sdist as _sdist
+        from setuptools.command.sdist import sdist as _sdist
 
     class cmd_sdist(_sdist):
-        def run(self):
+        def run(self) -> None:
             versions = get_versions()
             self._versioneer_generated_versions = versions
             # unless we update this, the command will keep using the old
             # version
             self.distribution.metadata.version = versions["version"]
             return _sdist.run(self)
 
-        def make_release_tree(self, base_dir, files):
+        def make_release_tree(self, base_dir: str, files: List[str]) -> None:
             root = get_root()
             cfg = get_config_from_root(root)
             _sdist.make_release_tree(self, base_dir, files)
             # now locate _version.py in the new base_dir directory
             # (remembering that it may be a hardlink) and replace it with an
             # updated value
             target_versionfile = os.path.join(base_dir, cfg.versionfile_source)
@@ -2022,15 +2222,15 @@
 
 INIT_PY_SNIPPET = """
 from . import {0}
 __version__ = {0}.get_versions()['version']
 """
 
 
-def do_setup():
+def do_setup() -> int:
     """Do main VCS-independent setup function for installing Versioneer."""
     root = get_root()
     try:
         cfg = get_config_from_root(root)
     except (OSError, configparser.NoSectionError, configparser.NoOptionError) as e:
         if isinstance(e, (OSError, configparser.NoSectionError)):
             print("Adding sample versioneer config to setup.cfg", file=sys.stderr)
@@ -2050,14 +2250,15 @@
                 "TAG_PREFIX": cfg.tag_prefix,
                 "PARENTDIR_PREFIX": cfg.parentdir_prefix,
                 "VERSIONFILE_SOURCE": cfg.versionfile_source,
             }
         )
 
     ipy = os.path.join(os.path.dirname(cfg.versionfile_source), "__init__.py")
+    maybe_ipy: Optional[str] = ipy
     if os.path.exists(ipy):
         try:
             with open(ipy, "r") as f:
                 old = f.read()
         except OSError:
             old = ""
         module = os.path.splitext(os.path.basename(cfg.versionfile_source))[0]
@@ -2070,58 +2271,24 @@
             print(" appending to %s" % ipy)
             with open(ipy, "a") as f:
                 f.write(snippet)
         else:
             print(" %s unmodified" % ipy)
     else:
         print(" %s doesn't exist, ok" % ipy)
-        ipy = None
-
-    # Make sure both the top-level "versioneer.py" and versionfile_source
-    # (PKG/_version.py, used by runtime code) are in MANIFEST.in, so
-    # they'll be copied into source distributions. Pip won't be able to
-    # install the package without this.
-    manifest_in = os.path.join(root, "MANIFEST.in")
-    simple_includes = set()
-    try:
-        with open(manifest_in, "r") as f:
-            for line in f:
-                if line.startswith("include "):
-                    for include in line.split()[1:]:
-                        simple_includes.add(include)
-    except OSError:
-        pass
-    # That doesn't cover everything MANIFEST.in can do
-    # (http://docs.python.org/2/distutils/sourcedist.html#commands), so
-    # it might give some false negatives. Appending redundant 'include'
-    # lines is safe, though.
-    if "versioneer.py" not in simple_includes:
-        print(" appending 'versioneer.py' to MANIFEST.in")
-        with open(manifest_in, "a") as f:
-            f.write("include versioneer.py\n")
-    else:
-        print(" 'versioneer.py' already in MANIFEST.in")
-    if cfg.versionfile_source not in simple_includes:
-        print(
-            " appending versionfile_source ('%s') to MANIFEST.in"
-            % cfg.versionfile_source
-        )
-        with open(manifest_in, "a") as f:
-            f.write("include %s\n" % cfg.versionfile_source)
-    else:
-        print(" versionfile_source already in MANIFEST.in")
+        maybe_ipy = None
 
     # Make VCS-specific changes. For git, this means creating/changing
     # .gitattributes to mark _version.py for export-subst keyword
     # substitution.
-    do_vcs_install(manifest_in, cfg.versionfile_source, ipy)
+    do_vcs_install(cfg.versionfile_source, maybe_ipy)
     return 0
 
 
-def scan_setup_py():
+def scan_setup_py() -> int:
     """Validate the contents of setup.py against Versioneer's expectations."""
     found = set()
     setters = False
     errors = 0
     with open("setup.py", "r") as f:
         for line in f.readlines():
             if "import versioneer" in line:
@@ -2150,14 +2317,18 @@
         print("'versioneer.versionfile_source = ' . This configuration")
         print("now lives in setup.cfg, and should be removed from setup.py")
         print("")
         errors += 1
     return errors
 
 
+def setup_command() -> NoReturn:
+    """Set up Versioneer and exit with appropriate error code."""
+    errors = do_setup()
+    errors += scan_setup_py()
+    sys.exit(1 if errors else 0)
+
+
 if __name__ == "__main__":
     cmd = sys.argv[1]
     if cmd == "setup":
-        errors = do_setup()
-        errors += scan_setup_py()
-        if errors:
-            sys.exit(1)
+        setup_command()
```

