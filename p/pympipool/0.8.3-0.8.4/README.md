# Comparing `tmp/pympipool-0.8.3.tar.gz` & `tmp/pympipool-0.8.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pympipool-0.8.3.tar", last modified: Thu May 16 15:19:52 2024, max compression
+gzip compressed data, was "pympipool-0.8.4.tar", last modified: Wed May 29 09:59:25 2024, max compression
```

## Comparing `pympipool-0.8.3.tar` & `pympipool-0.8.4.tar`

### file list

```diff
@@ -1,56 +1,56 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-16 15:19:52.341984 pympipool-0.8.3/
--rw-r--r--   0 runner    (1001) docker     (127)     1511 2024-05-16 15:19:10.000000 pympipool-0.8.3/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)       15 2024-05-16 15:19:10.000000 pympipool-0.8.3/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (127)    10992 2024-05-16 15:19:52.341984 pympipool-0.8.3/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     8087 2024-05-16 15:19:10.000000 pympipool-0.8.3/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-16 15:19:52.333984 pympipool-0.8.3/pympipool/
--rw-r--r--   0 runner    (1001) docker     (127)    10248 2024-05-16 15:19:10.000000 pympipool-0.8.3/pympipool/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      496 2024-05-16 15:19:52.341984 pympipool-0.8.3/pympipool/_version.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-16 15:19:52.333984 pympipool-0.8.3/pympipool/backend/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-16 15:19:10.000000 pympipool-0.8.3/pympipool/backend/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2762 2024-05-16 15:19:10.000000 pympipool-0.8.3/pympipool/backend/mpiexec.py
--rw-r--r--   0 runner    (1001) docker     (127)     2094 2024-05-16 15:19:10.000000 pympipool-0.8.3/pympipool/backend/serial.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-16 15:19:52.333984 pympipool-0.8.3/pympipool/scheduler/
--rw-r--r--   0 runner    (1001) docker     (127)     7530 2024-05-16 15:19:10.000000 pympipool-0.8.3/pympipool/scheduler/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     9200 2024-05-16 15:19:10.000000 pympipool-0.8.3/pympipool/scheduler/flux.py
--rw-r--r--   0 runner    (1001) docker     (127)     6828 2024-05-16 15:19:10.000000 pympipool-0.8.3/pympipool/scheduler/mpi.py
--rw-r--r--   0 runner    (1001) docker     (127)     7757 2024-05-16 15:19:10.000000 pympipool-0.8.3/pympipool/scheduler/slurm.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-16 15:19:52.337984 pympipool-0.8.3/pympipool/shared/
--rw-r--r--   0 runner    (1001) docker     (127)      601 2024-05-16 15:19:10.000000 pympipool-0.8.3/pympipool/shared/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2179 2024-05-16 15:19:10.000000 pympipool-0.8.3/pympipool/shared/backend.py
--rw-r--r--   0 runner    (1001) docker     (127)     6140 2024-05-16 15:19:10.000000 pympipool-0.8.3/pympipool/shared/communication.py
--rw-r--r--   0 runner    (1001) docker     (127)      813 2024-05-16 15:19:10.000000 pympipool-0.8.3/pympipool/shared/dependencies.py
--rw-r--r--   0 runner    (1001) docker     (127)    23991 2024-05-16 15:19:10.000000 pympipool-0.8.3/pympipool/shared/executorbase.py
--rw-r--r--   0 runner    (1001) docker     (127)     2828 2024-05-16 15:19:10.000000 pympipool-0.8.3/pympipool/shared/inputcheck.py
--rw-r--r--   0 runner    (1001) docker     (127)     3996 2024-05-16 15:19:10.000000 pympipool-0.8.3/pympipool/shared/interface.py
--rw-r--r--   0 runner    (1001) docker     (127)      769 2024-05-16 15:19:10.000000 pympipool-0.8.3/pympipool/shared/thread.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-16 15:19:52.337984 pympipool-0.8.3/pympipool/shell/
--rw-r--r--   0 runner    (1001) docker     (127)      169 2024-05-16 15:19:10.000000 pympipool-0.8.3/pympipool/shell/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2987 2024-05-16 15:19:10.000000 pympipool-0.8.3/pympipool/shell/executor.py
--rw-r--r--   0 runner    (1001) docker     (127)     7397 2024-05-16 15:19:10.000000 pympipool-0.8.3/pympipool/shell/interactive.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-16 15:19:52.337984 pympipool-0.8.3/pympipool.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)    10992 2024-05-16 15:19:52.000000 pympipool-0.8.3/pympipool.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     1326 2024-05-16 15:19:52.000000 pympipool-0.8.3/pympipool.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-16 15:19:52.000000 pympipool-0.8.3/pympipool.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       94 2024-05-16 15:19:52.000000 pympipool-0.8.3/pympipool.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       10 2024-05-16 15:19:52.000000 pympipool-0.8.3/pympipool.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)     1560 2024-05-16 15:19:50.000000 pympipool-0.8.3/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-16 15:19:52.341984 pympipool-0.8.3/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)      136 2024-05-16 15:19:10.000000 pympipool-0.8.3/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-16 15:19:52.337984 pympipool-0.8.3/tests/
--rw-r--r--   0 runner    (1001) docker     (127)     2874 2024-05-16 15:19:10.000000 pympipool-0.8.3/tests/test_backend_serial.py
--rw-r--r--   0 runner    (1001) docker     (127)      631 2024-05-16 15:19:10.000000 pympipool-0.8.3/tests/test_dependencies_executor.py
--rw-r--r--   0 runner    (1001) docker     (127)     3008 2024-05-16 15:19:10.000000 pympipool-0.8.3/tests/test_executor_backend_flux.py
--rw-r--r--   0 runner    (1001) docker     (127)     2228 2024-05-16 15:19:10.000000 pympipool-0.8.3/tests/test_executor_backend_mpi.py
--rw-r--r--   0 runner    (1001) docker     (127)     2442 2024-05-16 15:19:10.000000 pympipool-0.8.3/tests/test_executor_backend_mpi_noblock.py
--rw-r--r--   0 runner    (1001) docker     (127)     3704 2024-05-16 15:19:10.000000 pympipool-0.8.3/tests/test_flux_executor.py
--rw-r--r--   0 runner    (1001) docker     (127)     7586 2024-05-16 15:19:10.000000 pympipool-0.8.3/tests/test_integration_pyiron_workflow.py
--rw-r--r--   0 runner    (1001) docker     (127)    14133 2024-05-16 15:19:10.000000 pympipool-0.8.3/tests/test_mpi_executor.py
--rw-r--r--   0 runner    (1001) docker     (127)     3933 2024-05-16 15:19:10.000000 pympipool-0.8.3/tests/test_mpi_executor_future.py
--rw-r--r--   0 runner    (1001) docker     (127)     3237 2024-05-16 15:19:10.000000 pympipool-0.8.3/tests/test_shared_backend.py
--rw-r--r--   0 runner    (1001) docker     (127)     1898 2024-05-16 15:19:10.000000 pympipool-0.8.3/tests/test_shared_communication.py
--rw-r--r--   0 runner    (1001) docker     (127)      712 2024-05-16 15:19:10.000000 pympipool-0.8.3/tests/test_shared_executorbase.py
--rw-r--r--   0 runner    (1001) docker     (127)     1868 2024-05-16 15:19:10.000000 pympipool-0.8.3/tests/test_shared_input_check.py
--rw-r--r--   0 runner    (1001) docker     (127)      345 2024-05-16 15:19:10.000000 pympipool-0.8.3/tests/test_shared_thread.py
--rw-r--r--   0 runner    (1001) docker     (127)     3408 2024-05-16 15:19:10.000000 pympipool-0.8.3/tests/test_shell_executor.py
--rw-r--r--   0 runner    (1001) docker     (127)     2450 2024-05-16 15:19:10.000000 pympipool-0.8.3/tests/test_shell_interactive.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-29 09:59:25.202346 pympipool-0.8.4/
+-rw-r--r--   0 runner    (1001) docker     (127)     1511 2024-05-29 09:58:42.000000 pympipool-0.8.4/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)       15 2024-05-29 09:58:42.000000 pympipool-0.8.4/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (127)    10992 2024-05-29 09:59:25.202346 pympipool-0.8.4/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     8087 2024-05-29 09:58:42.000000 pympipool-0.8.4/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-29 09:59:25.194346 pympipool-0.8.4/pympipool/
+-rw-r--r--   0 runner    (1001) docker     (127)    10754 2024-05-29 09:58:42.000000 pympipool-0.8.4/pympipool/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      496 2024-05-29 09:59:25.202346 pympipool-0.8.4/pympipool/_version.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-29 09:59:25.198346 pympipool-0.8.4/pympipool/backend/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-29 09:58:42.000000 pympipool-0.8.4/pympipool/backend/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2762 2024-05-29 09:58:42.000000 pympipool-0.8.4/pympipool/backend/mpiexec.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2094 2024-05-29 09:58:42.000000 pympipool-0.8.4/pympipool/backend/serial.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-29 09:59:25.198346 pympipool-0.8.4/pympipool/scheduler/
+-rw-r--r--   0 runner    (1001) docker     (127)     7770 2024-05-29 09:58:42.000000 pympipool-0.8.4/pympipool/scheduler/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9568 2024-05-29 09:58:42.000000 pympipool-0.8.4/pympipool/scheduler/flux.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6848 2024-05-29 09:58:42.000000 pympipool-0.8.4/pympipool/scheduler/mpi.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7777 2024-05-29 09:58:42.000000 pympipool-0.8.4/pympipool/scheduler/slurm.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-29 09:59:25.198346 pympipool-0.8.4/pympipool/shared/
+-rw-r--r--   0 runner    (1001) docker     (127)      601 2024-05-29 09:58:42.000000 pympipool-0.8.4/pympipool/shared/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2179 2024-05-29 09:58:42.000000 pympipool-0.8.4/pympipool/shared/backend.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6140 2024-05-29 09:58:42.000000 pympipool-0.8.4/pympipool/shared/communication.py
+-rw-r--r--   0 runner    (1001) docker     (127)      813 2024-05-29 09:58:42.000000 pympipool-0.8.4/pympipool/shared/dependencies.py
+-rw-r--r--   0 runner    (1001) docker     (127)    23991 2024-05-29 09:58:42.000000 pympipool-0.8.4/pympipool/shared/executorbase.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3665 2024-05-29 09:58:42.000000 pympipool-0.8.4/pympipool/shared/inputcheck.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3996 2024-05-29 09:58:42.000000 pympipool-0.8.4/pympipool/shared/interface.py
+-rw-r--r--   0 runner    (1001) docker     (127)      769 2024-05-29 09:58:42.000000 pympipool-0.8.4/pympipool/shared/thread.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-29 09:59:25.198346 pympipool-0.8.4/pympipool/shell/
+-rw-r--r--   0 runner    (1001) docker     (127)      169 2024-05-29 09:58:42.000000 pympipool-0.8.4/pympipool/shell/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2987 2024-05-29 09:58:42.000000 pympipool-0.8.4/pympipool/shell/executor.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7397 2024-05-29 09:58:42.000000 pympipool-0.8.4/pympipool/shell/interactive.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-29 09:59:25.202346 pympipool-0.8.4/pympipool.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)    10992 2024-05-29 09:59:25.000000 pympipool-0.8.4/pympipool.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     1326 2024-05-29 09:59:25.000000 pympipool-0.8.4/pympipool.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-29 09:59:25.000000 pympipool-0.8.4/pympipool.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       94 2024-05-29 09:59:25.000000 pympipool-0.8.4/pympipool.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       10 2024-05-29 09:59:25.000000 pympipool-0.8.4/pympipool.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)     1560 2024-05-29 09:59:23.000000 pympipool-0.8.4/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-29 09:59:25.202346 pympipool-0.8.4/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)      136 2024-05-29 09:58:42.000000 pympipool-0.8.4/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-29 09:59:25.202346 pympipool-0.8.4/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)     2874 2024-05-29 09:58:42.000000 pympipool-0.8.4/tests/test_backend_serial.py
+-rw-r--r--   0 runner    (1001) docker     (127)      631 2024-05-29 09:58:42.000000 pympipool-0.8.4/tests/test_dependencies_executor.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3099 2024-05-29 09:58:42.000000 pympipool-0.8.4/tests/test_executor_backend_flux.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2228 2024-05-29 09:58:42.000000 pympipool-0.8.4/tests/test_executor_backend_mpi.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2442 2024-05-29 09:58:42.000000 pympipool-0.8.4/tests/test_executor_backend_mpi_noblock.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3771 2024-05-29 09:58:42.000000 pympipool-0.8.4/tests/test_flux_executor.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7586 2024-05-29 09:58:42.000000 pympipool-0.8.4/tests/test_integration_pyiron_workflow.py
+-rw-r--r--   0 runner    (1001) docker     (127)    14133 2024-05-29 09:58:42.000000 pympipool-0.8.4/tests/test_mpi_executor.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3933 2024-05-29 09:58:42.000000 pympipool-0.8.4/tests/test_mpi_executor_future.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3237 2024-05-29 09:58:42.000000 pympipool-0.8.4/tests/test_shared_backend.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1898 2024-05-29 09:58:42.000000 pympipool-0.8.4/tests/test_shared_communication.py
+-rw-r--r--   0 runner    (1001) docker     (127)      712 2024-05-29 09:58:42.000000 pympipool-0.8.4/tests/test_shared_executorbase.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1949 2024-05-29 09:58:42.000000 pympipool-0.8.4/tests/test_shared_input_check.py
+-rw-r--r--   0 runner    (1001) docker     (127)      345 2024-05-29 09:58:42.000000 pympipool-0.8.4/tests/test_shared_thread.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3408 2024-05-29 09:58:42.000000 pympipool-0.8.4/tests/test_shell_executor.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2450 2024-05-29 09:58:42.000000 pympipool-0.8.4/tests/test_shell_interactive.py
```

### Comparing `pympipool-0.8.3/LICENSE` & `pympipool-0.8.4/LICENSE`

 * *Files identical despite different names*

### Comparing `pympipool-0.8.3/PKG-INFO` & `pympipool-0.8.4/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pympipool
-Version: 0.8.3
+Version: 0.8.4
 Summary: Scale serial and MPI-parallel python functions over hundreds of compute nodes all from within a jupyter notebook or serial python process.
 Author-email: Jan Janssen <janssen@lanl.gov>
 License: BSD 3-Clause License
         
         Copyright (c) 2022, Jan Janssen
         All rights reserved.
```

### Comparing `pympipool-0.8.3/README.md` & `pympipool-0.8.4/README.md`

 * *Files identical despite different names*

### Comparing `pympipool-0.8.3/pympipool/__init__.py` & `pympipool-0.8.4/pympipool/__init__.py`

 * *Files 3% similar despite different names*

```diff
@@ -28,14 +28,15 @@
                            recommended, as computers have a limited number of compute cores.
         max_cores (int): defines the number cores which can be used in parallel
         cores_per_worker (int): number of MPI cores to be used for each function call
         threads_per_core (int): number of OpenMP threads to be used for each function call
         gpus_per_worker (int): number of GPUs per worker - defaults to 0
         oversubscribe (bool): adds the `--oversubscribe` command line flag (OpenMPI and SLURM only) - default False
         cwd (str/None): current working directory where the parallel python task is executed
+        executor (flux.job.FluxExecutor): Flux Python interface to submit the workers to flux
         hostname_localhost (boolean): use localhost instead of the hostname to establish the zmq connection. In the
                                       context of an HPC cluster this essential to be able to communicate to an
                                       Executor running on a different compute node within the same allocation. And
                                       in principle any computer should be able to resolve that their own hostname
                                       points to the same address as localhost. Still MacOS >= 12 seems to disable
                                       this look up for security reasons. So on MacOS it is required to set this
                                       option to true
@@ -43,14 +44,15 @@
                        is selected (the default) the available backend is determined automatically.
         block_allocation (boolean): To accelerate the submission of a series of python functions with the same resource
                                     requirements, pympipool supports block allocation. In this case all resources have
                                     to be defined on the executor, rather than during the submission of the individual
                                     function.
         init_function (None): optional function to preset arguments for functions which are submitted later
         command_line_argument_lst (list): Additional command line arguments for the srun call (SLURM only)
+        pmi (str): PMI interface to use (OpenMPI v5 requires pmix) default is None (Flux only)
 
     Examples:
         ```
         >>> import numpy as np
         >>> from pympipool import Executor
         >>>
         >>> def calc(i, j, k):
@@ -80,14 +82,15 @@
         cwd: Optional[str] = None,
         executor=None,
         hostname_localhost: bool = False,
         backend="auto",
         block_allocation: bool = True,
         init_function: Optional[callable] = None,
         command_line_argument_lst: list[str] = [],
+        pmi: Optional[str] = None,
         disable_dependencies: bool = False,
         refresh_rate: float = 0.01,
     ):
         # Use __new__() instead of __init__(). This function is only implemented to enable auto-completion.
         pass
 
     def __new__(
@@ -101,14 +104,15 @@
         cwd: Optional[str] = None,
         executor=None,
         hostname_localhost: bool = False,
         backend: str = "auto",
         block_allocation: bool = False,
         init_function: Optional[callable] = None,
         command_line_argument_lst: list[str] = [],
+        pmi: Optional[str] = None,
         disable_dependencies: bool = False,
         refresh_rate: float = 0.01,
     ):
         """
         Instead of returning a pympipool.Executor object this function returns either a pympipool.mpi.PyMPIExecutor,
         pympipool.slurm.PySlurmExecutor or pympipool.flux.PyFluxExecutor depending on which backend is available. The
         pympipool.flux.PyFluxExecutor is the preferred choice while the pympipool.mpi.PyMPIExecutor is primarily used
@@ -122,14 +126,15 @@
                                max_cores is recommended, as computers have a limited number of compute cores.
             max_cores (int): defines the number cores which can be used in parallel
             cores_per_worker (int): number of MPI cores to be used for each function call
             threads_per_core (int): number of OpenMP threads to be used for each function call
             gpus_per_worker (int): number of GPUs per worker - defaults to 0
             oversubscribe (bool): adds the `--oversubscribe` command line flag (OpenMPI and SLURM only) - default False
             cwd (str/None): current working directory where the parallel python task is executed
+            executor (flux.job.FluxExecutor): Flux Python interface to submit the workers to flux
             hostname_localhost (boolean): use localhost instead of the hostname to establish the zmq connection. In the
                                       context of an HPC cluster this essential to be able to communicate to an
                                       Executor running on a different compute node within the same allocation. And
                                       in principle any computer should be able to resolve that their own hostname
                                       points to the same address as localhost. Still MacOS >= 12 seems to disable
                                       this look up for security reasons. So on MacOS it is required to set this
                                       option to true
@@ -137,14 +142,15 @@
                            is selected (the default) the available backend is determined automatically.
             block_allocation (boolean): To accelerate the submission of a series of python functions with the same
                                         resource requirements, pympipool supports block allocation. In this case all
                                         resources have to be defined on the executor, rather than during the submission
                                         of the individual function.
             init_function (None): optional function to preset arguments for functions which are submitted later
             command_line_argument_lst (list): Additional command line arguments for the srun call (SLURM only)
+            pmi (str): PMI interface to use (OpenMPI v5 requires pmix) default is None (Flux only)
             disable_dependencies (boolean): Disable resolving future objects during the submission.
             refresh_rate (float): Set the refresh rate in seconds, how frequently the input queue is checked.
 
         """
         if not disable_dependencies:
             return ExecutorWithDependencies(
                 max_workers=max_workers,
@@ -156,14 +162,15 @@
                 cwd=cwd,
                 executor=executor,
                 hostname_localhost=hostname_localhost,
                 backend=backend,
                 block_allocation=block_allocation,
                 init_function=init_function,
                 command_line_argument_lst=command_line_argument_lst,
+                pmi=pmi,
                 refresh_rate=refresh_rate,
             )
         else:
             _check_refresh_rate(refresh_rate=refresh_rate)
             return create_executor(
                 max_workers=max_workers,
                 max_cores=max_cores,
@@ -174,8 +181,9 @@
                 cwd=cwd,
                 executor=executor,
                 hostname_localhost=hostname_localhost,
                 backend=backend,
                 block_allocation=block_allocation,
                 init_function=init_function,
                 command_line_argument_lst=command_line_argument_lst,
+                pmi=pmi,
             )
```

### Comparing `pympipool-0.8.3/pympipool/backend/mpiexec.py` & `pympipool-0.8.4/pympipool/backend/mpiexec.py`

 * *Files identical despite different names*

### Comparing `pympipool-0.8.3/pympipool/backend/serial.py` & `pympipool-0.8.4/pympipool/backend/serial.py`

 * *Files identical despite different names*

### Comparing `pympipool-0.8.3/pympipool/scheduler/__init__.py` & `pympipool-0.8.4/pympipool/scheduler/__init__.py`

 * *Files 2% similar despite different names*

```diff
@@ -8,16 +8,17 @@
 from pympipool.shared.interface import SLURM_COMMAND
 from pympipool.shared.inputcheck import (
     check_command_line_argument_lst,
     check_gpus_per_worker,
     check_threads_per_core,
     check_oversubscribe,
     check_executor,
-    check_backend,
     check_init_function,
+    check_pmi,
+    validate_backend,
     validate_number_of_cores,
 )
 from pympipool.scheduler.slurm import (
     PySlurmExecutor,
     PySlurmStepExecutor,
 )
 
@@ -46,14 +47,15 @@
     cwd: Optional[str] = None,
     executor=None,
     hostname_localhost: bool = False,
     backend: str = "auto",
     block_allocation: bool = False,
     init_function: Optional[callable] = None,
     command_line_argument_lst: list[str] = [],
+    pmi: Optional[str] = None,
 ):
     """
     Instead of returning a pympipool.Executor object this function returns either a pympipool.mpi.PyMPIExecutor,
     pympipool.slurm.PySlurmExecutor or pympipool.flux.PyFluxExecutor depending on which backend is available. The
     pympipool.flux.PyFluxExecutor is the preferred choice while the pympipool.mpi.PyMPIExecutor is primarily used
     for development and testing. The pympipool.flux.PyFluxExecutor requires flux-core from the flux-framework to be
     installed and in addition flux-sched to enable GPU scheduling. Finally, the pympipool.slurm.PySlurmExecutor
@@ -79,46 +81,52 @@
                        is selected (the default) the available backend is determined automatically.
         block_allocation (boolean): To accelerate the submission of a series of python functions with the same
                                     resource requirements, pympipool supports block allocation. In this case all
                                     resources have to be defined on the executor, rather than during the submission
                                     of the individual function.
         init_function (None): optional function to preset arguments for functions which are submitted later
         command_line_argument_lst (list): Additional command line arguments for the srun call (SLURM only)
+        pmi (str): PMI interface to use (OpenMPI v5 requires pmix) default is None (Flux only)
 
     """
     max_cores = validate_number_of_cores(max_cores=max_cores, max_workers=max_workers)
     check_init_function(block_allocation=block_allocation, init_function=init_function)
-    check_backend(backend=backend)
-    if backend == "flux" or (backend == "auto" and flux_installed):
+    backend = validate_backend(
+        backend=backend, flux_installed=flux_installed, slurm_installed=slurm_installed
+    )
+    check_pmi(backend=backend, pmi=pmi)
+    if backend == "flux":
         check_oversubscribe(oversubscribe=oversubscribe)
         check_command_line_argument_lst(
             command_line_argument_lst=command_line_argument_lst
         )
         if block_allocation:
             return PyFluxExecutor(
                 max_workers=int(max_cores / cores_per_worker),
                 cores_per_worker=cores_per_worker,
                 threads_per_core=threads_per_core,
                 gpus_per_worker=gpus_per_worker,
                 init_function=init_function,
                 cwd=cwd,
                 executor=executor,
                 hostname_localhost=hostname_localhost,
+                pmi=pmi,
             )
         else:
             return PyFluxStepExecutor(
                 max_cores=max_cores,
                 cores_per_worker=cores_per_worker,
                 threads_per_core=threads_per_core,
                 gpus_per_worker=gpus_per_worker,
                 cwd=cwd,
                 executor=executor,
                 hostname_localhost=hostname_localhost,
+                pmi=pmi,
             )
-    elif backend == "slurm" or (backend == "auto" and slurm_installed):
+    elif backend == "slurm":
         check_executor(executor=executor)
         if block_allocation:
             return PySlurmExecutor(
                 max_workers=int(max_cores / cores_per_worker),
                 cores_per_worker=cores_per_worker,
                 threads_per_core=threads_per_core,
                 gpus_per_worker=gpus_per_worker,
```

### Comparing `pympipool-0.8.3/pympipool/scheduler/flux.py` & `pympipool-0.8.4/pympipool/scheduler/flux.py`

 * *Files 3% similar despite different names*

```diff
@@ -24,26 +24,27 @@
         max_workers (int): defines the number workers which can execute functions in parallel
         cores_per_worker (int): number of MPI cores to be used for each function call
         threads_per_core (int): number of OpenMP threads to be used for each function call
         gpus_per_worker (int): number of GPUs per worker - defaults to 0
         init_function (None): optional function to preset arguments for functions which are submitted later
         cwd (str/None): current working directory where the parallel python task is executed
         executor (flux.job.FluxExecutor): Flux Python interface to submit the workers to flux
+        pmi (str): PMI interface to use (OpenMPI v5 requires pmix) default is None
         hostname_localhost (boolean): use localhost instead of the hostname to establish the zmq connection. In the
                                       context of an HPC cluster this essential to be able to communicate to an
                                       Executor running on a different compute node within the same allocation. And
                                       in principle any computer should be able to resolve that their own hostname
                                       points to the same address as localhost. Still MacOS >= 12 seems to disable
                                       this look up for security reasons. So on MacOS it is required to set this
                                       option to true
 
     Examples:
 
         >>> import numpy as np
-        >>> from pympipool.flux import PyFluxExecutor
+        >>> from pympipool.scheduler.flux import PyFluxExecutor
         >>>
         >>> def calc(i, j, k):
         >>>     from mpi4py import MPI
         >>>     size = MPI.COMM_WORLD.Get_size()
         >>>     rank = MPI.COMM_WORLD.Get_rank()
         >>>     return np.array([i, j, k]), size, rank
         >>>
@@ -62,14 +63,15 @@
         max_workers: int = 1,
         cores_per_worker: int = 1,
         threads_per_core: int = 1,
         gpus_per_worker: int = 0,
         init_function: Optional[callable] = None,
         cwd: Optional[str] = None,
         executor: Optional[flux.job.FluxExecutor] = None,
+        pmi: Optional[str] = None,
         hostname_localhost: Optional[bool] = False,
     ):
         super().__init__()
         self._set_process(
             process=[
                 RaisingThread(
                     target=execute_parallel_tasks,
@@ -81,14 +83,15 @@
                         "hostname_localhost": hostname_localhost,
                         "init_function": init_function,
                         # Interface Arguments
                         "threads_per_core": threads_per_core,
                         "gpus_per_core": int(gpus_per_worker / cores_per_worker),
                         "cwd": cwd,
                         "executor": executor,
+                        "pmi": pmi,
                     },
                 )
                 for _ in range(max_workers)
             ],
         )
 
 
@@ -100,29 +103,29 @@
     worker.
 
     Args:
         max_cores (int): defines the number workers which can execute functions in parallel
         cores_per_worker (int): number of MPI cores to be used for each function call
         threads_per_core (int): number of OpenMP threads to be used for each function call
         gpus_per_worker (int): number of GPUs per worker - defaults to 0
-        init_function (None): optional function to preset arguments for functions which are submitted later
         cwd (str/None): current working directory where the parallel python task is executed
         executor (flux.job.FluxExecutor): Flux Python interface to submit the workers to flux
+        pmi (str): PMI interface to use (OpenMPI v5 requires pmix) default is None
         hostname_localhost (boolean): use localhost instead of the hostname to establish the zmq connection. In the
                                       context of an HPC cluster this essential to be able to communicate to an
                                       Executor running on a different compute node within the same allocation. And
                                       in principle any computer should be able to resolve that their own hostname
                                       points to the same address as localhost. Still MacOS >= 12 seems to disable
                                       this look up for security reasons. So on MacOS it is required to set this
                                       option to true
 
     Examples:
 
         >>> import numpy as np
-        >>> from pympipool.flux import PyFluxStepExecutor
+        >>> from pympipool.scheduler.flux import PyFluxStepExecutor
         >>>
         >>> def calc(i, j, k):
         >>>     from mpi4py import MPI
         >>>     size = MPI.COMM_WORLD.Get_size()
         >>>     rank = MPI.COMM_WORLD.Get_rank()
         >>>     return np.array([i, j, k]), size, rank
         >>>
@@ -138,14 +141,15 @@
         self,
         max_cores: int = 1,
         cores_per_worker: int = 1,
         threads_per_core: int = 1,
         gpus_per_worker: int = 0,
         cwd: Optional[str] = None,
         executor: Optional[flux.job.FluxExecutor] = None,
+        pmi: Optional[str] = None,
         hostname_localhost: Optional[bool] = False,
     ):
         super().__init__()
         self._set_process(
             RaisingThread(
                 target=execute_separate_tasks,
                 kwargs={
@@ -156,37 +160,40 @@
                     "max_cores": max_cores,
                     "hostname_localhost": hostname_localhost,
                     # Interface Arguments
                     "threads_per_core": threads_per_core,
                     "gpus_per_core": int(gpus_per_worker / cores_per_worker),
                     "cwd": cwd,
                     "executor": executor,
+                    "pmi": pmi,
                 },
             )
         )
 
 
 class FluxPythonInterface(BaseInterface):
     def __init__(
         self,
         cwd: Optional[str] = None,
         cores: int = 1,
         threads_per_core: int = 1,
         gpus_per_core: int = 0,
         oversubscribe: bool = False,
         executor: Optional[flux.job.FluxExecutor] = None,
+        pmi: Optional[str] = None,
     ):
         super().__init__(
             cwd=cwd,
             cores=cores,
             oversubscribe=oversubscribe,
         )
         self._threads_per_core = threads_per_core
         self._gpus_per_core = gpus_per_core
         self._executor = executor
+        self._pmi = pmi
         self._future = None
 
     def bootup(self, command_lst: list[str]):
         if self._oversubscribe:
             raise ValueError(
                 "Oversubscribing is currently not supported for the Flux adapter."
             )
@@ -197,14 +204,16 @@
             num_tasks=self._cores,
             cores_per_task=self._threads_per_core,
             gpus_per_task=self._gpus_per_core,
             num_nodes=None,
             exclusive=False,
         )
         jobspec.environment = dict(os.environ)
+        if self._pmi is not None:
+            jobspec.setattr_shell_option("pmi", self._pmi)
         if self._cwd is not None:
             jobspec.cwd = self._cwd
         self._future = self._executor.submit(jobspec)
 
     def shutdown(self, wait: bool = True):
         if self.poll():
             self._future.cancel()
```

### Comparing `pympipool-0.8.3/pympipool/scheduler/mpi.py` & `pympipool-0.8.4/pympipool/scheduler/mpi.py`

 * *Files 1% similar despite different names*

```diff
@@ -31,15 +31,15 @@
                                       points to the same address as localhost. Still MacOS >= 12 seems to disable
                                       this look up for security reasons. So on MacOS it is required to set this
                                       option to true
 
     Examples:
 
         >>> import numpy as np
-        >>> from pympipool.mpi import PyMPIExecutor
+        >>> from pympipool.scheduler.mpi import PyMPIExecutor
         >>>
         >>> def calc(i, j, k):
         >>>     from mpi4py import MPI
         >>>     size = MPI.COMM_WORLD.Get_size()
         >>>     rank = MPI.COMM_WORLD.Get_rank()
         >>>     return np.array([i, j, k]), size, rank
         >>>
@@ -104,15 +104,15 @@
                                       points to the same address as localhost. Still MacOS >= 12 seems to disable
                                       this look up for security reasons. So on MacOS it is required to set this
                                       option to true
 
     Examples:
 
         >>> import numpy as np
-        >>> from pympipool.mpi import PyMPIStepExecutor
+        >>> from pympipool.scheduler.mpi import PyMPIStepExecutor
         >>>
         >>> def calc(i, j, k):
         >>>     from mpi4py import MPI
         >>>     size = MPI.COMM_WORLD.Get_size()
         >>>     rank = MPI.COMM_WORLD.Get_rank()
         >>>     return np.array([i, j, k]), size, rank
         >>>
```

### Comparing `pympipool-0.8.3/pympipool/scheduler/slurm.py` & `pympipool-0.8.4/pympipool/scheduler/slurm.py`

 * *Files 1% similar despite different names*

```diff
@@ -32,15 +32,15 @@
                                       this look up for security reasons. So on MacOS it is required to set this
                                       option to true
         command_line_argument_lst (list): Additional command line arguments for the srun call
 
     Examples:
 
         >>> import numpy as np
-        >>> from pympipool.slurm import PySlurmExecutor
+        >>> from pympipool.scheduler.slurm import PySlurmExecutor
         >>>
         >>> def calc(i, j, k):
         >>>     from mpi4py import MPI
         >>>     size = MPI.COMM_WORLD.Get_size()
         >>>     rank = MPI.COMM_WORLD.Get_rank()
         >>>     return np.array([i, j, k]), size, rank
         >>>
@@ -113,15 +113,15 @@
                                       this look up for security reasons. So on MacOS it is required to set this
                                       option to true
         command_line_argument_lst (list): Additional command line arguments for the srun call
 
     Examples:
 
         >>> import numpy as np
-        >>> from pympipool.slurm import PySlurmStepExecutor
+        >>> from pympipool.scheduler.slurm import PySlurmStepExecutor
         >>>
         >>> def calc(i, j, k):
         >>>     from mpi4py import MPI
         >>>     size = MPI.COMM_WORLD.Get_size()
         >>>     rank = MPI.COMM_WORLD.Get_rank()
         >>>     return np.array([i, j, k]), size, rank
         >>>
```

### Comparing `pympipool-0.8.3/pympipool/shared/__init__.py` & `pympipool-0.8.4/pympipool/shared/__init__.py`

 * *Files identical despite different names*

### Comparing `pympipool-0.8.3/pympipool/shared/backend.py` & `pympipool-0.8.4/pympipool/shared/backend.py`

 * *Files identical despite different names*

### Comparing `pympipool-0.8.3/pympipool/shared/communication.py` & `pympipool-0.8.4/pympipool/shared/communication.py`

 * *Files identical despite different names*

### Comparing `pympipool-0.8.3/pympipool/shared/dependencies.py` & `pympipool-0.8.4/pympipool/shared/dependencies.py`

 * *Files identical despite different names*

### Comparing `pympipool-0.8.3/pympipool/shared/executorbase.py` & `pympipool-0.8.4/pympipool/shared/executorbase.py`

 * *Files identical despite different names*

### Comparing `pympipool-0.8.3/pympipool/shared/inputcheck.py` & `pympipool-0.8.4/pympipool/shared/inputcheck.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,87 +1,106 @@
 import inspect
+from typing import List, Optional
+from concurrent.futures import Executor
 
 
-def check_oversubscribe(oversubscribe):
+def check_oversubscribe(oversubscribe: bool):
     if oversubscribe:
         raise ValueError(
             "Oversubscribing is not supported for the pympipool.flux.PyFLuxExecutor backend."
             "Please use oversubscribe=False instead of oversubscribe=True."
         )
 
 
-def check_command_line_argument_lst(command_line_argument_lst):
+def check_command_line_argument_lst(command_line_argument_lst: List[str]):
     if len(command_line_argument_lst) > 0:
         raise ValueError(
             "The command_line_argument_lst parameter is not supported for the SLURM backend."
         )
 
 
-def check_gpus_per_worker(gpus_per_worker):
+def check_gpus_per_worker(gpus_per_worker: int):
     if gpus_per_worker != 0:
         raise TypeError(
             "GPU assignment is not supported for the pympipool.mpi.PyMPIExecutor backend."
             "Please use gpus_per_worker=0 instead of gpus_per_worker="
             + str(gpus_per_worker)
             + "."
         )
 
 
-def check_threads_per_core(threads_per_core):
+def check_threads_per_core(threads_per_core: int):
     if threads_per_core != 1:
         raise TypeError(
             "Thread based parallelism is not supported for the pympipool.mpi.PyMPIExecutor backend."
             "Please use threads_per_core=1 instead of threads_per_core="
             + str(threads_per_core)
             + "."
         )
 
 
-def check_executor(executor):
+def check_executor(executor: Executor):
     if executor is not None:
         raise ValueError(
             "The executor parameter is only supported for the flux framework backend."
         )
 
 
-def check_resource_dict(function):
+def check_resource_dict(function: callable):
     if "resource_dict" in inspect.signature(function).parameters.keys():
         raise ValueError(
             "The parameter resource_dict is used internally in pympipool, "
             "so it cannot be used as parameter in the submitted functions."
         )
 
 
-def check_resource_dict_is_empty(resource_dict):
+def check_resource_dict_is_empty(resource_dict: dict):
     if len(resource_dict) > 0:
         raise ValueError(
             "When block_allocation is enabled, the resource requirements have to be defined on the executor level."
         )
 
 
-def check_refresh_rate(refresh_rate):
+def check_refresh_rate(refresh_rate: float):
     if refresh_rate != 0.01:
         raise ValueError(
             "The sleep_interval parameter is only used when disable_dependencies=False."
         )
 
 
-def check_backend(backend):
+def validate_backend(
+    backend: str, flux_installed: bool = False, slurm_installed: bool = False
+) -> str:
     if backend not in ["auto", "mpi", "slurm", "flux"]:
         raise ValueError(
             'The currently implemented backends are ["flux", "mpi", "slurm"]. '
             'Alternatively, you can select "auto", the default option, to automatically determine the backend. But '
             + backend
             + " is not a valid choice."
         )
+    elif backend == "flux" or (backend == "auto" and flux_installed):
+        return "flux"
+    elif backend == "slurm" or (backend == "auto" and slurm_installed):
+        return "slurm"
+    else:
+        return "mpi"
 
 
-def check_init_function(block_allocation, init_function):
+def check_pmi(backend: str, pmi: Optional[str]):
+    if backend != "flux" and pmi is not None:
+        raise ValueError("The pmi parameter is currently only implemented for flux.")
+    elif backend == "flux" and pmi not in ["pmix", "pmi1", "pmi2", None]:
+        raise ValueError(
+            "The pmi parameter supports [pmix, pmi1, pmi2], but not: " + pmi
+        )
+
+
+def check_init_function(block_allocation: bool, init_function: callable):
     if not block_allocation and init_function is not None:
         raise ValueError("")
 
 
-def validate_number_of_cores(max_cores, max_workers):
+def validate_number_of_cores(max_cores: int, max_workers: int) -> int:
     # only overwrite max_cores when it is set to 1
     if max_workers != 1 and max_cores == 1:
         return max_workers
     return max_cores
```

### Comparing `pympipool-0.8.3/pympipool/shared/interface.py` & `pympipool-0.8.4/pympipool/shared/interface.py`

 * *Files identical despite different names*

### Comparing `pympipool-0.8.3/pympipool/shared/thread.py` & `pympipool-0.8.4/pympipool/shared/thread.py`

 * *Files identical despite different names*

### Comparing `pympipool-0.8.3/pympipool/shell/executor.py` & `pympipool-0.8.4/pympipool/shell/executor.py`

 * *Files identical despite different names*

### Comparing `pympipool-0.8.3/pympipool/shell/interactive.py` & `pympipool-0.8.4/pympipool/shell/interactive.py`

 * *Files identical despite different names*

### Comparing `pympipool-0.8.3/pympipool.egg-info/PKG-INFO` & `pympipool-0.8.4/pympipool.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pympipool
-Version: 0.8.3
+Version: 0.8.4
 Summary: Scale serial and MPI-parallel python functions over hundreds of compute nodes all from within a jupyter notebook or serial python process.
 Author-email: Jan Janssen <janssen@lanl.gov>
 License: BSD 3-Clause License
         
         Copyright (c) 2022, Jan Janssen
         All rights reserved.
```

### Comparing `pympipool-0.8.3/pympipool.egg-info/SOURCES.txt` & `pympipool-0.8.4/pympipool.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `pympipool-0.8.3/pyproject.toml` & `pympipool-0.8.4/pyproject.toml`

 * *Files identical despite different names*

### Comparing `pympipool-0.8.3/tests/test_backend_serial.py` & `pympipool-0.8.4/tests/test_backend_serial.py`

 * *Files identical despite different names*

### Comparing `pympipool-0.8.3/tests/test_dependencies_executor.py` & `pympipool-0.8.4/tests/test_dependencies_executor.py`

 * *Files identical despite different names*

### Comparing `pympipool-0.8.3/tests/test_executor_backend_flux.py` & `pympipool-0.8.4/tests/test_executor_backend_flux.py`

 * *Files 4% similar despite different names*

```diff
@@ -10,14 +10,15 @@
     import flux.job
     from pympipool.scheduler.flux import (
         PyFluxExecutor,
         FluxPythonInterface,
     )
 
     skip_flux_test = "FLUX_URI" not in os.environ
+    pmi = os.environ.get("PYMPIPOOL_PMIX", None)
 except ImportError:
     skip_flux_test = True
 
 
 def calc(i):
     return i
 
@@ -77,26 +78,28 @@
     def test_flux_executor_parallel(self):
         with Executor(
             max_cores=2,
             cores_per_worker=2,
             executor=self.executor,
             backend="flux",
             block_allocation=True,
+            pmi=pmi,
         ) as exe:
             fs_1 = exe.submit(mpi_funct, 1)
             self.assertEqual(fs_1.result(), [(1, 2, 0), (1, 2, 1)])
             self.assertTrue(fs_1.done())
 
     def test_single_task(self):
         with Executor(
             max_cores=2,
             cores_per_worker=2,
             executor=self.executor,
             backend="flux",
             block_allocation=True,
+            pmi=pmi,
         ) as p:
             output = p.map(mpi_funct, [1, 2, 3])
         self.assertEqual(
             list(output),
             [[(1, 2, 0), (1, 2, 1)], [(2, 2, 0), (2, 2, 1)], [(3, 2, 0), (3, 2, 1)]],
         )
```

### Comparing `pympipool-0.8.3/tests/test_executor_backend_mpi.py` & `pympipool-0.8.4/tests/test_executor_backend_mpi.py`

 * *Files identical despite different names*

### Comparing `pympipool-0.8.3/tests/test_executor_backend_mpi_noblock.py` & `pympipool-0.8.4/tests/test_executor_backend_mpi_noblock.py`

 * *Files identical despite different names*

### Comparing `pympipool-0.8.3/tests/test_flux_executor.py` & `pympipool-0.8.4/tests/test_flux_executor.py`

 * *Files 3% similar despite different names*

```diff
@@ -12,14 +12,15 @@
     import flux.job
     from pympipool.scheduler.flux import (
         PyFluxExecutor,
         FluxPythonInterface,
     )
 
     skip_flux_test = "FLUX_URI" not in os.environ
+    pmi = os.environ.get("PYMPIPOOL_PMIX", None)
 except ImportError:
     skip_flux_test = True
 
 
 def calc(i):
     return i
 
@@ -65,23 +66,23 @@
             self.assertEqual(fs_1.result(), 1)
             self.assertEqual(fs_2.result(), 2)
             self.assertTrue(fs_1.done())
             self.assertTrue(fs_2.done())
 
     def test_flux_executor_parallel(self):
         with PyFluxExecutor(
-            max_workers=1, cores_per_worker=2, executor=self.executor
+            max_workers=1, cores_per_worker=2, executor=self.executor, pmi=pmi
         ) as exe:
             fs_1 = exe.submit(mpi_funct, 1)
             self.assertEqual(fs_1.result(), [(1, 2, 0), (1, 2, 1)])
             self.assertTrue(fs_1.done())
 
     def test_single_task(self):
         with PyFluxExecutor(
-            max_workers=1, cores_per_worker=2, executor=self.executor
+            max_workers=1, cores_per_worker=2, executor=self.executor, pmi=pmi
         ) as p:
             output = p.map(mpi_funct, [1, 2, 3])
         self.assertEqual(
             list(output),
             [[(1, 2, 0), (1, 2, 1)], [(2, 2, 0), (2, 2, 1)], [(3, 2, 0), (3, 2, 1)]],
         )
```

### Comparing `pympipool-0.8.3/tests/test_integration_pyiron_workflow.py` & `pympipool-0.8.4/tests/test_integration_pyiron_workflow.py`

 * *Files identical despite different names*

### Comparing `pympipool-0.8.3/tests/test_mpi_executor.py` & `pympipool-0.8.4/tests/test_mpi_executor.py`

 * *Files identical despite different names*

### Comparing `pympipool-0.8.3/tests/test_mpi_executor_future.py` & `pympipool-0.8.4/tests/test_mpi_executor_future.py`

 * *Files identical despite different names*

### Comparing `pympipool-0.8.3/tests/test_shared_backend.py` & `pympipool-0.8.4/tests/test_shared_backend.py`

 * *Files identical despite different names*

### Comparing `pympipool-0.8.3/tests/test_shared_communication.py` & `pympipool-0.8.4/tests/test_shared_communication.py`

 * *Files identical despite different names*

### Comparing `pympipool-0.8.3/tests/test_shared_executorbase.py` & `pympipool-0.8.4/tests/test_shared_executorbase.py`

 * *Files identical despite different names*

### Comparing `pympipool-0.8.3/tests/test_shared_input_check.py` & `pympipool-0.8.4/tests/test_shared_input_check.py`

 * *Files 6% similar despite different names*

```diff
@@ -2,19 +2,19 @@
 
 from pympipool.shared.inputcheck import (
     check_command_line_argument_lst,
     check_gpus_per_worker,
     check_threads_per_core,
     check_oversubscribe,
     check_executor,
-    check_backend,
     check_init_function,
     check_refresh_rate,
     check_resource_dict,
     check_resource_dict_is_empty,
+    validate_backend,
 )
 
 
 class TestInputCheck(unittest.TestCase):
     def test_check_command_line_argument_lst(self):
         with self.assertRaises(ValueError):
             check_command_line_argument_lst(command_line_argument_lst=["a"])
@@ -33,15 +33,17 @@
 
     def test_check_executor(self):
         with self.assertRaises(ValueError):
             check_executor(executor=1)
 
     def test_check_backend(self):
         with self.assertRaises(ValueError):
-            check_backend(backend="test")
+            validate_backend(
+                backend="test", flux_installed=False, slurm_installed=False
+            )
 
     def test_check_init_function(self):
         with self.assertRaises(ValueError):
             check_init_function(init_function=1, block_allocation=False)
 
     def test_check_refresh_rate(self):
         with self.assertRaises(ValueError):
```

### Comparing `pympipool-0.8.3/tests/test_shell_executor.py` & `pympipool-0.8.4/tests/test_shell_executor.py`

 * *Files identical despite different names*

### Comparing `pympipool-0.8.3/tests/test_shell_interactive.py` & `pympipool-0.8.4/tests/test_shell_interactive.py`

 * *Files identical despite different names*

