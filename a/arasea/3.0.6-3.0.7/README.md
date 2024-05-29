# Comparing `tmp/arasea-3.0.6.tar.gz` & `tmp/arasea-3.0.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "arasea-3.0.6.tar", last modified: Tue Apr 30 15:26:15 2024, max compression
+gzip compressed data, was "arasea-3.0.7.tar", last modified: Wed May 29 05:48:23 2024, max compression
```

## Comparing `arasea-3.0.6.tar` & `arasea-3.0.7.tar`

### file list

```diff
@@ -1,453 +1,452 @@
-drwxrwxr-x   0 arkanepetra  (1000) arkanepetra  (1000)        0 2024-04-30 15:26:15.767294 arasea-3.0.6/
--rw-r--r--   0 arkanepetra  (1000) arkanepetra  (1000)     2515 2024-04-25 08:29:07.000000 arasea-3.0.6/LICENSE.txt
--rw-r--r--   0 arkanepetra  (1000) arkanepetra  (1000)     1660 2024-04-30 15:26:15.767294 arasea-3.0.6/PKG-INFO
--rw-r--r--   0 arkanepetra  (1000) arkanepetra  (1000)     5503 2024-04-25 08:29:07.000000 arasea-3.0.6/README.md
-drwxrwxr-x   0 arkanepetra  (1000) arkanepetra  (1000)        0 2024-04-30 15:26:15.637281 arasea-3.0.6/arasea/
--rw-r--r--   0 arkanepetra  (1000) arkanepetra  (1000)     5760 2024-04-25 08:29:07.000000 arasea-3.0.6/arasea/__init__.py
--rw-r--r--   0 arkanepetra  (1000) arkanepetra  (1000)      411 2024-04-30 15:25:57.000000 arasea-3.0.6/arasea/_version.py
--rw-r--r--   0 arkanepetra  (1000) arkanepetra  (1000)      252 2024-04-25 08:29:07.000000 arasea-3.0.6/arasea/assert_op.py
--rw-r--r--   0 arkanepetra  (1000) arkanepetra  (1000)     3561 2024-04-25 08:29:07.000000 arasea-3.0.6/arasea/benchmark.log
-drwxrwxr-x   0 arkanepetra  (1000) arkanepetra  (1000)        0 2024-04-30 15:26:15.639281 arasea-3.0.6/arasea/bin/
--rw-r--r--   0 arkanepetra  (1000) arkanepetra  (1000)        0 2024-04-25 08:29:07.000000 arasea-3.0.6/arasea/bin/__init__.py
--rw-r--r--   0 arkanepetra  (1000) arkanepetra  (1000)     4080 2024-04-25 08:29:07.000000 arasea-3.0.6/arasea/bin/arasea_cache.py
--rw-r--r--   0 arkanepetra  (1000) arkanepetra  (1000)     6055 2024-04-25 08:29:07.000000 arasea-3.0.6/arasea/breakpoint.py
-drwxrwxr-x   0 arkanepetra  (1000) arkanepetra  (1000)        0 2024-04-30 15:26:15.644281 arasea-3.0.6/arasea/compile/
--rw-r--r--   0 arkanepetra  (1000) arkanepetra  (1000)     1410 2024-04-25 08:29:07.000000 arasea-3.0.6/arasea/compile/__init__.py
--rw-r--r--   0 arkanepetra  (1000) arkanepetra  (1000)    41442 2024-04-25 08:29:07.000000 arasea-3.0.6/arasea/compile/builders.py
--rw-r--r--   0 arkanepetra  (1000) arkanepetra  (1000)     9954 2024-04-25 08:29:07.000000 arasea-3.0.6/arasea/compile/compiledir.py
--rw-r--r--   0 arkanepetra  (1000) arkanepetra  (1000)     2041 2024-04-25 08:29:07.000000 arasea-3.0.6/arasea/compile/compilelock.py
--rw-r--r--   0 arkanepetra  (1000) arkanepetra  (1000)    85654 2024-04-25 08:29:07.000000 arasea-3.0.6/arasea/compile/debugmode.py
-drwxrwxr-x   0 arkanepetra  (1000) arkanepetra  (1000)        0 2024-04-30 15:26:15.645282 arasea-3.0.6/arasea/compile/function/
--rw-r--r--   0 arkanepetra  (1000) arkanepetra  (1000)    13377 2024-04-25 08:29:07.000000 arasea-3.0.6/arasea/compile/function/__init__.py
--rw-r--r--   0 arkanepetra  (1000) arkanepetra  (1000)    22096 2024-04-25 08:29:07.000000 arasea-3.0.6/arasea/compile/function/pfunc.py
--rw-r--r--   0 arkanepetra  (1000) arkanepetra  (1000)    73889 2024-04-25 08:29:07.000000 arasea-3.0.6/arasea/compile/function/types.py
--rw-r--r--   0 arkanepetra  (1000) arkanepetra  (1000)     9102 2024-04-25 08:29:07.000000 arasea-3.0.6/arasea/compile/io.py
--rw-r--r--   0 arkanepetra  (1000) arkanepetra  (1000)    17793 2024-04-25 08:29:07.000000 arasea-3.0.6/arasea/compile/mode.py
--rw-r--r--   0 arkanepetra  (1000) arkanepetra  (1000)     3706 2024-04-25 08:29:07.000000 arasea-3.0.6/arasea/compile/monitormode.py
--rw-r--r--   0 arkanepetra  (1000) arkanepetra  (1000)     8326 2024-04-25 08:29:07.000000 arasea-3.0.6/arasea/compile/nanguardmode.py
--rw-r--r--   0 arkanepetra  (1000) arkanepetra  (1000)    11245 2024-04-25 08:29:07.000000 arasea-3.0.6/arasea/compile/ops.py
--rw-r--r--   0 arkanepetra  (1000) arkanepetra  (1000)    59770 2024-04-25 08:29:07.000000 arasea-3.0.6/arasea/compile/profiling.py
--rw-r--r--   0 arkanepetra  (1000) arkanepetra  (1000)     7179 2024-04-25 08:29:07.000000 arasea-3.0.6/arasea/compile/sharedvalue.py
--rw-r--r--   0 arkanepetra  (1000) arkanepetra  (1000)    46225 2024-04-25 08:29:07.000000 arasea-3.0.6/arasea/configdefaults.py
--rw-r--r--   0 arkanepetra  (1000) arkanepetra  (1000)    22462 2024-04-25 08:29:07.000000 arasea-3.0.6/arasea/configparser.py
-drwxrwxr-x   0 arkanepetra  (1000) arkanepetra  (1000)        0 2024-04-30 15:26:15.646282 arasea-3.0.6/arasea/d3viz/
--rw-r--r--   0 arkanepetra  (1000) arkanepetra  (1000)       46 2024-04-25 08:29:07.000000 arasea-3.0.6/arasea/d3viz/__init__.py
--rw-r--r--   0 arkanepetra  (1000) arkanepetra  (1000)     3830 2024-04-25 08:29:07.000000 arasea-3.0.6/arasea/d3viz/d3viz.py
--rw-r--r--   0 arkanepetra  (1000) arkanepetra  (1000)    11843 2024-04-25 08:29:07.000000 arasea-3.0.6/arasea/d3viz/formatting.py
--rw-r--r--   0 arkanepetra  (1000) arkanepetra  (1000)        0 2024-04-25 08:29:07.000000 arasea-3.0.6/arasea/debug.log
--rw-r--r--   0 arkanepetra  (1000) arkanepetra  (1000)    86751 2024-04-25 08:29:07.000000 arasea-3.0.6/arasea/gradient.py
-drwxrwxr-x   0 arkanepetra  (1000) arkanepetra  (1000)        0 2024-04-30 15:26:15.652282 arasea-3.0.6/arasea/graph/
--rw-r--r--   0 arkanepetra  (1000) arkanepetra  (1000)      505 2024-04-25 08:29:07.000000 arasea-3.0.6/arasea/graph/__init__.py
--rw-r--r--   0 arkanepetra  (1000) arkanepetra  (1000)    59773 2024-04-25 08:29:07.000000 arasea-3.0.6/arasea/graph/basic.py
--rw-r--r--   0 arkanepetra  (1000) arkanepetra  (1000)    33216 2024-04-25 08:29:07.000000 arasea-3.0.6/arasea/graph/destroyhandler.py
--rw-r--r--   0 arkanepetra  (1000) arkanepetra  (1000)    24835 2024-04-25 08:29:07.000000 arasea-3.0.6/arasea/graph/features.py
--rw-r--r--   0 arkanepetra  (1000) arkanepetra  (1000)    36232 2024-04-25 08:29:07.000000 arasea-3.0.6/arasea/graph/fg.py
--rw-r--r--   0 arkanepetra  (1000) arkanepetra  (1000)      246 2024-04-25 08:29:07.000000 arasea-3.0.6/arasea/graph/kanren.py
--rw-r--r--   0 arkanepetra  (1000) arkanepetra  (1000)     1150 2024-04-25 08:29:07.000000 arasea-3.0.6/arasea/graph/null_type.py
--rw-r--r--   0 arkanepetra  (1000) arkanepetra  (1000)    25036 2024-04-25 08:29:07.000000 arasea-3.0.6/arasea/graph/op.py
--rw-r--r--   0 arkanepetra  (1000) arkanepetra  (1000)      793 2024-04-25 08:29:07.000000 arasea-3.0.6/arasea/graph/opt.py
--rw-r--r--   0 arkanepetra  (1000) arkanepetra  (1000)      799 2024-04-25 08:29:07.000000 arasea-3.0.6/arasea/graph/opt_utils.py
--rw-r--r--   0 arkanepetra  (1000) arkanepetra  (1000)      786 2024-04-25 08:29:07.000000 arasea-3.0.6/arasea/graph/optdb.py
-drwxrwxr-x   0 arkanepetra  (1000) arkanepetra  (1000)        0 2024-04-30 15:26:15.654282 arasea-3.0.6/arasea/graph/rewriting/
--rw-r--r--   0 arkanepetra  (1000) arkanepetra  (1000)        0 2024-04-25 08:29:07.000000 arasea-3.0.6/arasea/graph/rewriting/__init__.py
--rw-r--r--   0 arkanepetra  (1000) arkanepetra  (1000)   114199 2024-04-25 08:29:07.000000 arasea-3.0.6/arasea/graph/rewriting/basic.py
--rw-r--r--   0 arkanepetra  (1000) arkanepetra  (1000)    19934 2024-04-25 08:29:07.000000 arasea-3.0.6/arasea/graph/rewriting/db.py
--rw-r--r--   0 arkanepetra  (1000) arkanepetra  (1000)     3035 2024-04-25 08:29:07.000000 arasea-3.0.6/arasea/graph/rewriting/kanren.py
--rw-r--r--   0 arkanepetra  (1000) arkanepetra  (1000)     7239 2024-04-25 08:29:07.000000 arasea-3.0.6/arasea/graph/rewriting/unify.py
--rw-r--r--   0 arkanepetra  (1000) arkanepetra  (1000)     9148 2024-04-25 08:29:07.000000 arasea-3.0.6/arasea/graph/rewriting/utils.py
--rw-r--r--   0 arkanepetra  (1000) arkanepetra  (1000)     7865 2024-04-25 08:29:07.000000 arasea-3.0.6/arasea/graph/sched.py
--rw-r--r--   0 arkanepetra  (1000) arkanepetra  (1000)      223 2024-04-25 08:29:07.000000 arasea-3.0.6/arasea/graph/toolbox.py
--rw-r--r--   0 arkanepetra  (1000) arkanepetra  (1000)     9527 2024-04-25 08:29:07.000000 arasea-3.0.6/arasea/graph/type.py
--rw-r--r--   0 arkanepetra  (1000) arkanepetra  (1000)      243 2024-04-25 08:29:07.000000 arasea-3.0.6/arasea/graph/unify.py
--rw-r--r--   0 arkanepetra  (1000) arkanepetra  (1000)    12091 2024-04-25 08:29:07.000000 arasea-3.0.6/arasea/graph/utils.py
--rw-r--r--   0 arkanepetra  (1000) arkanepetra  (1000)    29067 2024-04-25 08:29:07.000000 arasea-3.0.6/arasea/ifelse.py
-drwxrwxr-x   0 arkanepetra  (1000) arkanepetra  (1000)        0 2024-04-30 15:26:15.655283 arasea-3.0.6/arasea/link/
--rw-r--r--   0 arkanepetra  (1000) arkanepetra  (1000)        3 2024-04-25 08:29:07.000000 arasea-3.0.6/arasea/link/__init__.py
--rw-r--r--   0 arkanepetra  (1000) arkanepetra  (1000)    23890 2024-04-25 08:29:07.000000 arasea-3.0.6/arasea/link/basic.py
-drwxrwxr-x   0 arkanepetra  (1000) arkanepetra  (1000)        0 2024-04-30 15:26:15.659283 arasea-3.0.6/arasea/link/c/
--rw-r--r--   0 arkanepetra  (1000) arkanepetra  (1000)        0 2024-04-25 08:29:07.000000 arasea-3.0.6/arasea/link/c/__init__.py
--rw-r--r--   0 arkanepetra  (1000) arkanepetra  (1000)    72572 2024-04-25 08:29:07.000000 arasea-3.0.6/arasea/link/c/basic.py
--rw-r--r--   0 arkanepetra  (1000) arkanepetra  (1000)   113013 2024-04-25 08:29:07.000000 arasea-3.0.6/arasea/link/c/cmodule.py
--rw-r--r--   0 arkanepetra  (1000) arkanepetra  (1000)     4182 2024-04-25 08:29:07.000000 arasea-3.0.6/arasea/link/c/cutils.py
--rw-r--r--   0 arkanepetra  (1000) arkanepetra  (1000)     1054 2024-04-25 08:29:07.000000 arasea-3.0.6/arasea/link/c/cvm.py
--rw-r--r--   0 arkanepetra  (1000) arkanepetra  (1000)      402 2024-04-25 08:29:07.000000 arasea-3.0.6/arasea/link/c/exceptions.py
--rw-r--r--   0 arkanepetra  (1000) arkanepetra  (1000)    19955 2024-04-25 08:29:07.000000 arasea-3.0.6/arasea/link/c/interface.py
--rw-r--r--   0 arkanepetra  (1000) arkanepetra  (1000)     6641 2024-04-25 08:29:07.000000 arasea-3.0.6/arasea/link/c/lazylinker_c.py
--rw-r--r--   0 arkanepetra  (1000) arkanepetra  (1000)    24724 2024-04-25 08:29:07.000000 arasea-3.0.6/arasea/link/c/op.py
--rw-r--r--   0 arkanepetra  (1000) arkanepetra  (1000)    31544 2024-04-25 08:29:07.000000 arasea-3.0.6/arasea/link/c/params_type.py
--rw-r--r--   0 arkanepetra  (1000) arkanepetra  (1000)    26540 2024-04-25 08:29:07.000000 arasea-3.0.6/arasea/link/c/type.py
-drwxrwxr-x   0 arkanepetra  (1000) arkanepetra  (1000)        0 2024-04-30 15:26:15.660283 arasea-3.0.6/arasea/link/jax/
--rw-r--r--   0 arkanepetra  (1000) arkanepetra  (1000)       48 2024-04-25 08:29:07.000000 arasea-3.0.6/arasea/link/jax/__init__.py
-drwxrwxr-x   0 arkanepetra  (1000) arkanepetra  (1000)        0 2024-04-30 15:26:15.664284 arasea-3.0.6/arasea/link/jax/dispatch/
--rw-r--r--   0 arkanepetra  (1000) arkanepetra  (1000)      529 2024-04-25 08:29:07.000000 arasea-3.0.6/arasea/link/jax/dispatch/__init__.py
--rw-r--r--   0 arkanepetra  (1000) arkanepetra  (1000)     2370 2024-04-25 08:29:07.000000 arasea-3.0.6/arasea/link/jax/dispatch/basic.py
--rw-r--r--   0 arkanepetra  (1000) arkanepetra  (1000)     2944 2024-04-25 08:29:07.000000 arasea-3.0.6/arasea/link/jax/dispatch/elemwise.py
--rw-r--r--   0 arkanepetra  (1000) arkanepetra  (1000)     3380 2024-04-25 08:29:07.000000 arasea-3.0.6/arasea/link/jax/dispatch/extra_ops.py
--rw-r--r--   0 arkanepetra  (1000) arkanepetra  (1000)     3072 2024-04-25 08:29:07.000000 arasea-3.0.6/arasea/link/jax/dispatch/nlinalg.py
--rw-r--r--   0 arkanepetra  (1000) arkanepetra  (1000)    14480 2024-04-25 08:29:07.000000 arasea-3.0.6/arasea/link/jax/dispatch/random.py
--rw-r--r--   0 arkanepetra  (1000) arkanepetra  (1000)     5622 2024-04-25 08:29:07.000000 arasea-3.0.6/arasea/link/jax/dispatch/scalar.py
--rw-r--r--   0 arkanepetra  (1000) arkanepetra  (1000)     5382 2024-04-25 08:29:07.000000 arasea-3.0.6/arasea/link/jax/dispatch/scan.py
--rw-r--r--   0 arkanepetra  (1000) arkanepetra  (1000)     2745 2024-04-25 08:29:07.000000 arasea-3.0.6/arasea/link/jax/dispatch/shape.py
--rw-r--r--   0 arkanepetra  (1000) arkanepetra  (1000)     1115 2024-04-25 08:29:07.000000 arasea-3.0.6/arasea/link/jax/dispatch/slinalg.py
--rw-r--r--   0 arkanepetra  (1000) arkanepetra  (1000)     3188 2024-04-25 08:29:07.000000 arasea-3.0.6/arasea/link/jax/dispatch/subtensor.py
--rw-r--r--   0 arkanepetra  (1000) arkanepetra  (1000)     3380 2024-04-25 08:29:07.000000 arasea-3.0.6/arasea/link/jax/dispatch/tensor_basic.py
--rw-r--r--   0 arkanepetra  (1000) arkanepetra  (1000)      238 2024-04-25 08:29:07.000000 arasea-3.0.6/arasea/link/jax/jax_dispatch.py
--rw-r--r--   0 arkanepetra  (1000) arkanepetra  (1000)      232 2024-04-25 08:29:07.000000 arasea-3.0.6/arasea/link/jax/jax_linker.py
--rw-r--r--   0 arkanepetra  (1000) arkanepetra  (1000)     2991 2024-04-25 08:29:07.000000 arasea-3.0.6/arasea/link/jax/linker.py
-drwxrwxr-x   0 arkanepetra  (1000) arkanepetra  (1000)        0 2024-04-30 15:26:15.664284 arasea-3.0.6/arasea/link/numba/
--rw-r--r--   0 arkanepetra  (1000) arkanepetra  (1000)       49 2024-04-25 08:29:07.000000 arasea-3.0.6/arasea/link/numba/__init__.py
-drwxrwxr-x   0 arkanepetra  (1000) arkanepetra  (1000)        0 2024-04-30 15:26:15.667284 arasea-3.0.6/arasea/link/numba/dispatch/
--rw-r--r--   0 arkanepetra  (1000) arkanepetra  (1000)      506 2024-04-25 08:29:07.000000 arasea-3.0.6/arasea/link/numba/dispatch/__init__.py
--rw-r--r--   0 arkanepetra  (1000) arkanepetra  (1000)    25903 2024-04-25 08:29:07.000000 arasea-3.0.6/arasea/link/numba/dispatch/basic.py
--rw-r--r--   0 arkanepetra  (1000) arkanepetra  (1000)    22260 2024-04-25 08:29:07.000000 arasea-3.0.6/arasea/link/numba/dispatch/elemwise.py
--rw-r--r--   0 arkanepetra  (1000) arkanepetra  (1000)     9262 2024-04-25 08:29:07.000000 arasea-3.0.6/arasea/link/numba/dispatch/extra_ops.py
--rw-r--r--   0 arkanepetra  (1000) arkanepetra  (1000)     5076 2024-04-25 08:29:07.000000 arasea-3.0.6/arasea/link/numba/dispatch/nlinalg.py
--rw-r--r--   0 arkanepetra  (1000) arkanepetra  (1000)    12812 2024-04-25 08:29:07.000000 arasea-3.0.6/arasea/link/numba/dispatch/random.py
--rw-r--r--   0 arkanepetra  (1000) arkanepetra  (1000)     8893 2024-04-25 08:29:07.000000 arasea-3.0.6/arasea/link/numba/dispatch/scalar.py
--rw-r--r--   0 arkanepetra  (1000) arkanepetra  (1000)    14203 2024-04-25 08:29:07.000000 arasea-3.0.6/arasea/link/numba/dispatch/scan.py
--rw-r--r--   0 arkanepetra  (1000) arkanepetra  (1000)     6109 2024-04-25 08:29:07.000000 arasea-3.0.6/arasea/link/numba/dispatch/sparse.py
--rw-r--r--   0 arkanepetra  (1000) arkanepetra  (1000)     6403 2024-04-25 08:29:07.000000 arasea-3.0.6/arasea/link/numba/dispatch/tensor_basic.py
--rw-r--r--   0 arkanepetra  (1000) arkanepetra  (1000)     1044 2024-04-25 08:29:07.000000 arasea-3.0.6/arasea/link/numba/linker.py
--rw-r--r--   0 arkanepetra  (1000) arkanepetra  (1000)    28716 2024-04-25 08:29:07.000000 arasea-3.0.6/arasea/link/utils.py
--rw-r--r--   0 arkanepetra  (1000) arkanepetra  (1000)    50565 2024-04-25 08:29:07.000000 arasea-3.0.6/arasea/link/vm.py
-drwxrwxr-x   0 arkanepetra  (1000) arkanepetra  (1000)        0 2024-04-30 15:26:15.671284 arasea-3.0.6/arasea/misc/
--rw-r--r--   0 arkanepetra  (1000) arkanepetra  (1000)        0 2024-04-25 08:29:07.000000 arasea-3.0.6/arasea/misc/__init__.py
--rw-r--r--   0 arkanepetra  (1000) arkanepetra  (1000)    10017 2024-04-25 08:29:07.000000 arasea-3.0.6/arasea/misc/check_blas.py
--rwxr-xr-x   0 arkanepetra  (1000) arkanepetra  (1000)      280 2024-04-25 08:29:07.000000 arasea-3.0.6/arasea/misc/check_blas_many.sh
--rw-r--r--   0 arkanepetra  (1000) arkanepetra  (1000)     2409 2024-04-25 08:29:07.000000 arasea-3.0.6/arasea/misc/check_duplicate_key.py
--rw-r--r--   0 arkanepetra  (1000) arkanepetra  (1000)     2166 2024-04-25 08:29:07.000000 arasea-3.0.6/arasea/misc/elemwise_openmp_speedup.py
--rw-r--r--   0 arkanepetra  (1000) arkanepetra  (1000)     1887 2024-04-25 08:29:07.000000 arasea-3.0.6/arasea/misc/elemwise_time_test.py
--rw-r--r--   0 arkanepetra  (1000) arkanepetra  (1000)     1347 2024-04-25 08:29:07.000000 arasea-3.0.6/arasea/misc/frozendict.py
--rw-r--r--   0 arkanepetra  (1000) arkanepetra  (1000)      607 2024-04-25 08:29:07.000000 arasea-3.0.6/arasea/misc/latence_gpu_transfert.py
--rw-r--r--   0 arkanepetra  (1000) arkanepetra  (1000)      921 2024-04-25 08:29:07.000000 arasea-3.0.6/arasea/misc/may_share_memory.py
--rw-r--r--   0 arkanepetra  (1000) arkanepetra  (1000)     7191 2024-04-25 08:29:07.000000 arasea-3.0.6/arasea/misc/ordered_set.py
--rw-r--r--   0 arkanepetra  (1000) arkanepetra  (1000)    10166 2024-04-25 08:29:07.000000 arasea-3.0.6/arasea/misc/pkl_utils.py
--rw-r--r--   0 arkanepetra  (1000) arkanepetra  (1000)     2293 2024-04-25 08:29:07.000000 arasea-3.0.6/arasea/misc/safe_asarray.py
--rw-r--r--   0 arkanepetra  (1000) arkanepetra  (1000)    67046 2024-04-25 08:29:07.000000 arasea-3.0.6/arasea/printing.py
--rw-r--r--   0 arkanepetra  (1000) arkanepetra  (1000)        0 2024-04-25 08:29:07.000000 arasea-3.0.6/arasea/py.typed
--rw-r--r--   0 arkanepetra  (1000) arkanepetra  (1000)     5837 2024-04-25 08:29:07.000000 arasea-3.0.6/arasea/raise_op.py
-drwxrwxr-x   0 arkanepetra  (1000) arkanepetra  (1000)        0 2024-04-30 15:26:15.673284 arasea-3.0.6/arasea/sandbox/
--rw-r--r--   0 arkanepetra  (1000) arkanepetra  (1000)        0 2024-04-25 08:29:07.000000 arasea-3.0.6/arasea/sandbox/__init__.py
--rw-r--r--   0 arkanepetra  (1000) arkanepetra  (1000)     3873 2024-04-25 08:29:07.000000 arasea-3.0.6/arasea/sandbox/fourier.py
-drwxrwxr-x   0 arkanepetra  (1000) arkanepetra  (1000)        0 2024-04-30 15:26:15.674285 arasea-3.0.6/arasea/sandbox/linalg/
--rw-r--r--   0 arkanepetra  (1000) arkanepetra  (1000)       60 2024-04-25 08:29:07.000000 arasea-3.0.6/arasea/sandbox/linalg/__init__.py
--rw-r--r--   0 arkanepetra  (1000) arkanepetra  (1000)     6060 2024-04-25 08:29:07.000000 arasea-3.0.6/arasea/sandbox/linalg/ops.py
--rw-r--r--   0 arkanepetra  (1000) arkanepetra  (1000)     1455 2024-04-25 08:29:07.000000 arasea-3.0.6/arasea/sandbox/minimal.py
--rw-r--r--   0 arkanepetra  (1000) arkanepetra  (1000)    14812 2024-04-25 08:29:07.000000 arasea-3.0.6/arasea/sandbox/multinomial.py
--rw-r--r--   0 arkanepetra  (1000) arkanepetra  (1000)    48271 2024-04-25 08:29:07.000000 arasea-3.0.6/arasea/sandbox/rng_mrg.py
--rw-r--r--   0 arkanepetra  (1000) arkanepetra  (1000)      217 2024-04-25 08:29:07.000000 arasea-3.0.6/arasea/sandbox/solve.py
-drwxrwxr-x   0 arkanepetra  (1000) arkanepetra  (1000)        0 2024-04-30 15:26:15.676285 arasea-3.0.6/arasea/scalar/
--rw-r--r--   0 arkanepetra  (1000) arkanepetra  (1000)      709 2024-04-25 08:29:07.000000 arasea-3.0.6/arasea/scalar/__init__.py
--rw-r--r--   0 arkanepetra  (1000) arkanepetra  (1000)   143429 2024-04-25 08:29:07.000000 arasea-3.0.6/arasea/scalar/basic.py
--rw-r--r--   0 arkanepetra  (1000) arkanepetra  (1000)      223 2024-04-25 08:29:07.000000 arasea-3.0.6/arasea/scalar/basic_scipy.py
--rw-r--r--   0 arkanepetra  (1000) arkanepetra  (1000)     3275 2024-04-25 08:29:07.000000 arasea-3.0.6/arasea/scalar/basic_sympy.py
--rw-r--r--   0 arkanepetra  (1000) arkanepetra  (1000)    46142 2024-04-25 08:29:07.000000 arasea-3.0.6/arasea/scalar/math.py
--rw-r--r--   0 arkanepetra  (1000) arkanepetra  (1000)     1851 2024-04-25 08:29:07.000000 arasea-3.0.6/arasea/scalar/sharedvar.py
-drwxrwxr-x   0 arkanepetra  (1000) arkanepetra  (1000)        0 2024-04-30 15:26:15.679285 arasea-3.0.6/arasea/scan/
--rw-r--r--   0 arkanepetra  (1000) arkanepetra  (1000)     1931 2024-04-25 08:29:07.000000 arasea-3.0.6/arasea/scan/__init__.py
--rw-r--r--   0 arkanepetra  (1000) arkanepetra  (1000)    50095 2024-04-25 08:29:07.000000 arasea-3.0.6/arasea/scan/basic.py
--rw-r--r--   0 arkanepetra  (1000) arkanepetra  (1000)     6743 2024-04-25 08:29:07.000000 arasea-3.0.6/arasea/scan/checkpoints.py
--rw-r--r--   0 arkanepetra  (1000) arkanepetra  (1000)   140522 2024-04-25 08:29:07.000000 arasea-3.0.6/arasea/scan/op.py
--rw-r--r--   0 arkanepetra  (1000) arkanepetra  (1000)      226 2024-04-25 08:29:07.000000 arasea-3.0.6/arasea/scan/opt.py
--rw-r--r--   0 arkanepetra  (1000) arkanepetra  (1000)    95587 2024-04-25 08:29:07.000000 arasea-3.0.6/arasea/scan/rewriting.py
--rw-r--r--   0 arkanepetra  (1000) arkanepetra  (1000)     3511 2024-04-25 08:29:07.000000 arasea-3.0.6/arasea/scan/scan_perform_ext.py
--rw-r--r--   0 arkanepetra  (1000) arkanepetra  (1000)    38052 2024-04-25 08:29:07.000000 arasea-3.0.6/arasea/scan/utils.py
--rw-r--r--   0 arkanepetra  (1000) arkanepetra  (1000)     4599 2024-04-25 08:29:07.000000 arasea-3.0.6/arasea/scan/views.py
-drwxrwxr-x   0 arkanepetra  (1000) arkanepetra  (1000)        0 2024-04-30 15:26:15.682285 arasea-3.0.6/arasea/sparse/
--rw-r--r--   0 arkanepetra  (1000) arkanepetra  (1000)     1097 2024-04-25 08:29:07.000000 arasea-3.0.6/arasea/sparse/__init__.py
--rw-r--r--   0 arkanepetra  (1000) arkanepetra  (1000)   118008 2024-04-25 08:29:07.000000 arasea-3.0.6/arasea/sparse/basic.py
--rw-r--r--   0 arkanepetra  (1000) arkanepetra  (1000)      232 2024-04-25 08:29:07.000000 arasea-3.0.6/arasea/sparse/opt.py
--rw-r--r--   0 arkanepetra  (1000) arkanepetra  (1000)    76905 2024-04-25 08:29:07.000000 arasea-3.0.6/arasea/sparse/rewriting.py
-drwxrwxr-x   0 arkanepetra  (1000) arkanepetra  (1000)        0 2024-04-30 15:26:15.683286 arasea-3.0.6/arasea/sparse/sandbox/
--rw-r--r--   0 arkanepetra  (1000) arkanepetra  (1000)        0 2024-04-25 08:29:07.000000 arasea-3.0.6/arasea/sparse/sandbox/__init__.py
--rw-r--r--   0 arkanepetra  (1000) arkanepetra  (1000)    17303 2024-04-25 08:29:07.000000 arasea-3.0.6/arasea/sparse/sandbox/sp.py
--rw-r--r--   0 arkanepetra  (1000) arkanepetra  (1000)     7194 2024-04-25 08:29:07.000000 arasea-3.0.6/arasea/sparse/sandbox/sp2.py
--rw-r--r--   0 arkanepetra  (1000) arkanepetra  (1000)      827 2024-04-25 08:29:07.000000 arasea-3.0.6/arasea/sparse/sharedvar.py
--rw-r--r--   0 arkanepetra  (1000) arkanepetra  (1000)     8044 2024-04-25 08:29:07.000000 arasea-3.0.6/arasea/sparse/type.py
--rw-r--r--   0 arkanepetra  (1000) arkanepetra  (1000)      767 2024-04-25 08:29:07.000000 arasea-3.0.6/arasea/sparse/utils.py
-drwxrwxr-x   0 arkanepetra  (1000) arkanepetra  (1000)        0 2024-04-30 15:26:15.697287 arasea-3.0.6/arasea/tensor/
--rw-r--r--   0 arkanepetra  (1000) arkanepetra  (1000)     4883 2024-04-25 08:29:07.000000 arasea-3.0.6/arasea/tensor/__init__.py
--rw-r--r--   0 arkanepetra  (1000) arkanepetra  (1000)   135651 2024-04-25 08:29:07.000000 arasea-3.0.6/arasea/tensor/basic.py
--rw-r--r--   0 arkanepetra  (1000) arkanepetra  (1000)      461 2024-04-25 08:29:07.000000 arasea-3.0.6/arasea/tensor/basic_opt.py
--rw-r--r--   0 arkanepetra  (1000) arkanepetra  (1000)    98819 2024-04-25 08:29:07.000000 arasea-3.0.6/arasea/tensor/blas.py
--rw-r--r--   0 arkanepetra  (1000) arkanepetra  (1000)    26486 2024-04-25 08:29:07.000000 arasea-3.0.6/arasea/tensor/blas_c.py
--rw-r--r--   0 arkanepetra  (1000) arkanepetra  (1000)    68050 2024-04-25 08:29:07.000000 arasea-3.0.6/arasea/tensor/blas_headers.py
--rw-r--r--   0 arkanepetra  (1000) arkanepetra  (1000)     2783 2024-04-25 08:29:07.000000 arasea-3.0.6/arasea/tensor/blas_scipy.py
--rw-r--r--   0 arkanepetra  (1000) arkanepetra  (1000)    66675 2024-04-25 08:29:07.000000 arasea-3.0.6/arasea/tensor/elemwise.py
--rw-r--r--   0 arkanepetra  (1000) arkanepetra  (1000)    20860 2024-04-25 08:29:07.000000 arasea-3.0.6/arasea/tensor/elemwise_cgen.py
--rw-r--r--   0 arkanepetra  (1000) arkanepetra  (1000)      362 2024-04-25 08:29:07.000000 arasea-3.0.6/arasea/tensor/exceptions.py
--rw-r--r--   0 arkanepetra  (1000) arkanepetra  (1000)    57997 2024-04-25 08:29:07.000000 arasea-3.0.6/arasea/tensor/extra_ops.py
--rw-r--r--   0 arkanepetra  (1000) arkanepetra  (1000)     7589 2024-04-25 08:29:07.000000 arasea-3.0.6/arasea/tensor/fft.py
--rw-r--r--   0 arkanepetra  (1000) arkanepetra  (1000)     6565 2024-04-25 08:29:07.000000 arasea-3.0.6/arasea/tensor/fourier.py
--rw-r--r--   0 arkanepetra  (1000) arkanepetra  (1000)     7848 2024-04-25 08:29:07.000000 arasea-3.0.6/arasea/tensor/inplace.py
--rw-r--r--   0 arkanepetra  (1000) arkanepetra  (1000)     7239 2024-04-25 08:29:07.000000 arasea-3.0.6/arasea/tensor/io.py
--rw-r--r--   0 arkanepetra  (1000) arkanepetra  (1000)       72 2024-04-25 08:29:07.000000 arasea-3.0.6/arasea/tensor/linalg.py
--rw-r--r--   0 arkanepetra  (1000) arkanepetra  (1000)    96168 2024-04-25 08:29:07.000000 arasea-3.0.6/arasea/tensor/math.py
--rw-r--r--   0 arkanepetra  (1000) arkanepetra  (1000)      247 2024-04-25 08:29:07.000000 arasea-3.0.6/arasea/tensor/math_opt.py
--rw-r--r--   0 arkanepetra  (1000) arkanepetra  (1000)    22498 2024-04-25 08:29:07.000000 arasea-3.0.6/arasea/tensor/nlinalg.py
-drwxrwxr-x   0 arkanepetra  (1000) arkanepetra  (1000)        0 2024-04-30 15:26:15.702288 arasea-3.0.6/arasea/tensor/nnet/
--rw-r--r--   0 arkanepetra  (1000) arkanepetra  (1000)     1431 2024-04-25 08:29:07.000000 arasea-3.0.6/arasea/tensor/nnet/__init__.py
--rw-r--r--   0 arkanepetra  (1000) arkanepetra  (1000)   138965 2024-04-25 08:29:07.000000 arasea-3.0.6/arasea/tensor/nnet/abstract_conv.py
--rw-r--r--   0 arkanepetra  (1000) arkanepetra  (1000)    75765 2024-04-25 08:29:07.000000 arasea-3.0.6/arasea/tensor/nnet/basic.py
--rw-r--r--   0 arkanepetra  (1000) arkanepetra  (1000)    35376 2024-04-25 08:29:07.000000 arasea-3.0.6/arasea/tensor/nnet/batchnorm.py
--rw-r--r--   0 arkanepetra  (1000) arkanepetra  (1000)     8902 2024-04-25 08:29:07.000000 arasea-3.0.6/arasea/tensor/nnet/blocksparse.py
--rw-r--r--   0 arkanepetra  (1000) arkanepetra  (1000)    94523 2024-04-25 08:29:07.000000 arasea-3.0.6/arasea/tensor/nnet/conv.py
--rw-r--r--   0 arkanepetra  (1000) arkanepetra  (1000)     9910 2024-04-25 08:29:07.000000 arasea-3.0.6/arasea/tensor/nnet/conv3d2d.py
--rw-r--r--   0 arkanepetra  (1000) arkanepetra  (1000)    40356 2024-04-25 08:29:07.000000 arasea-3.0.6/arasea/tensor/nnet/corr.py
--rw-r--r--   0 arkanepetra  (1000) arkanepetra  (1000)    36145 2024-04-25 08:29:07.000000 arasea-3.0.6/arasea/tensor/nnet/corr3d.py
--rw-r--r--   0 arkanepetra  (1000) arkanepetra  (1000)     8522 2024-04-25 08:29:07.000000 arasea-3.0.6/arasea/tensor/nnet/ctc.py
--rw-r--r--   0 arkanepetra  (1000) arkanepetra  (1000)    35353 2024-04-25 08:29:07.000000 arasea-3.0.6/arasea/tensor/nnet/neighbours.py
--rw-r--r--   0 arkanepetra  (1000) arkanepetra  (1000)      247 2024-04-25 08:29:07.000000 arasea-3.0.6/arasea/tensor/nnet/opt.py
--rw-r--r--   0 arkanepetra  (1000) arkanepetra  (1000)    17297 2024-04-25 08:29:07.000000 arasea-3.0.6/arasea/tensor/nnet/rewriting.py
--rw-r--r--   0 arkanepetra  (1000) arkanepetra  (1000)     5212 2024-04-25 08:29:07.000000 arasea-3.0.6/arasea/tensor/nnet/sigm.py
--rw-r--r--   0 arkanepetra  (1000) arkanepetra  (1000)      277 2024-04-25 08:29:07.000000 arasea-3.0.6/arasea/tensor/opt_uncanonicalize.py
-drwxrwxr-x   0 arkanepetra  (1000) arkanepetra  (1000)        0 2024-04-30 15:26:15.704288 arasea-3.0.6/arasea/tensor/random/
--rw-r--r--   0 arkanepetra  (1000) arkanepetra  (1000)      265 2024-04-25 08:29:07.000000 arasea-3.0.6/arasea/tensor/random/__init__.py
--rw-r--r--   0 arkanepetra  (1000) arkanepetra  (1000)    65558 2024-04-25 08:29:07.000000 arasea-3.0.6/arasea/tensor/random/basic.py
--rw-r--r--   0 arkanepetra  (1000) arkanepetra  (1000)    14324 2024-04-25 08:29:07.000000 arasea-3.0.6/arasea/tensor/random/op.py
--rw-r--r--   0 arkanepetra  (1000) arkanepetra  (1000)      253 2024-04-25 08:29:07.000000 arasea-3.0.6/arasea/tensor/random/opt.py
-drwxrwxr-x   0 arkanepetra  (1000) arkanepetra  (1000)        0 2024-04-30 15:26:15.705288 arasea-3.0.6/arasea/tensor/random/rewriting/
--rw-r--r--   0 arkanepetra  (1000) arkanepetra  (1000)      221 2024-04-25 08:29:07.000000 arasea-3.0.6/arasea/tensor/random/rewriting/__init__.py
--rw-r--r--   0 arkanepetra  (1000) arkanepetra  (1000)    15290 2024-04-25 08:29:07.000000 arasea-3.0.6/arasea/tensor/random/rewriting/basic.py
--rw-r--r--   0 arkanepetra  (1000) arkanepetra  (1000)     1887 2024-04-25 08:29:07.000000 arasea-3.0.6/arasea/tensor/random/rewriting/jax.py
--rw-r--r--   0 arkanepetra  (1000) arkanepetra  (1000)     6730 2024-04-25 08:29:07.000000 arasea-3.0.6/arasea/tensor/random/type.py
--rw-r--r--   0 arkanepetra  (1000) arkanepetra  (1000)     9024 2024-04-25 08:29:07.000000 arasea-3.0.6/arasea/tensor/random/utils.py
--rw-r--r--   0 arkanepetra  (1000) arkanepetra  (1000)     1534 2024-04-25 08:29:07.000000 arasea-3.0.6/arasea/tensor/random/var.py
-drwxrwxr-x   0 arkanepetra  (1000) arkanepetra  (1000)        0 2024-04-30 15:26:15.709288 arasea-3.0.6/arasea/tensor/rewriting/
--rw-r--r--   0 arkanepetra  (1000) arkanepetra  (1000)      384 2024-04-25 08:29:07.000000 arasea-3.0.6/arasea/tensor/rewriting/__init__.py
--rw-r--r--   0 arkanepetra  (1000) arkanepetra  (1000)    42723 2024-04-25 08:29:07.000000 arasea-3.0.6/arasea/tensor/rewriting/basic.py
--rw-r--r--   0 arkanepetra  (1000) arkanepetra  (1000)    39439 2024-04-25 08:29:07.000000 arasea-3.0.6/arasea/tensor/rewriting/elemwise.py
--rw-r--r--   0 arkanepetra  (1000) arkanepetra  (1000)     4845 2024-04-25 08:29:07.000000 arasea-3.0.6/arasea/tensor/rewriting/extra_ops.py
--rw-r--r--   0 arkanepetra  (1000) arkanepetra  (1000)     3954 2024-04-25 08:29:07.000000 arasea-3.0.6/arasea/tensor/rewriting/jax.py
--rw-r--r--   0 arkanepetra  (1000) arkanepetra  (1000)   124250 2024-04-25 08:29:07.000000 arasea-3.0.6/arasea/tensor/rewriting/math.py
--rw-r--r--   0 arkanepetra  (1000) arkanepetra  (1000)    43264 2024-04-25 08:29:07.000000 arasea-3.0.6/arasea/tensor/rewriting/shape.py
--rw-r--r--   0 arkanepetra  (1000) arkanepetra  (1000)     6111 2024-04-25 08:29:07.000000 arasea-3.0.6/arasea/tensor/rewriting/special.py
--rw-r--r--   0 arkanepetra  (1000) arkanepetra  (1000)    63199 2024-04-25 08:29:07.000000 arasea-3.0.6/arasea/tensor/rewriting/subtensor.py
--rw-r--r--   0 arkanepetra  (1000) arkanepetra  (1000)     9500 2024-04-25 08:29:07.000000 arasea-3.0.6/arasea/tensor/rewriting/uncanonicalize.py
--rw-r--r--   0 arkanepetra  (1000) arkanepetra  (1000)    33298 2024-04-25 08:29:07.000000 arasea-3.0.6/arasea/tensor/shape.py
--rw-r--r--   0 arkanepetra  (1000) arkanepetra  (1000)     3858 2024-04-25 08:29:07.000000 arasea-3.0.6/arasea/tensor/sharedvar.py
-drwxrwxr-x   0 arkanepetra  (1000) arkanepetra  (1000)        0 2024-04-30 15:26:15.710288 arasea-3.0.6/arasea/tensor/signal/
--rw-r--r--   0 arkanepetra  (1000) arkanepetra  (1000)        0 2024-04-25 08:29:07.000000 arasea-3.0.6/arasea/tensor/signal/__init__.py
--rw-r--r--   0 arkanepetra  (1000) arkanepetra  (1000)     3509 2024-04-25 08:29:07.000000 arasea-3.0.6/arasea/tensor/signal/conv.py
--rwxr-xr-x   0 arkanepetra  (1000) arkanepetra  (1000)    97524 2024-04-25 08:29:07.000000 arasea-3.0.6/arasea/tensor/signal/pool.py
--rw-r--r--   0 arkanepetra  (1000) arkanepetra  (1000)    24997 2024-04-25 08:29:07.000000 arasea-3.0.6/arasea/tensor/slinalg.py
--rw-r--r--   0 arkanepetra  (1000) arkanepetra  (1000)    17849 2024-04-25 08:29:07.000000 arasea-3.0.6/arasea/tensor/sort.py
--rw-r--r--   0 arkanepetra  (1000) arkanepetra  (1000)    27385 2024-04-25 08:29:07.000000 arasea-3.0.6/arasea/tensor/special.py
--rw-r--r--   0 arkanepetra  (1000) arkanepetra  (1000)    91231 2024-04-25 08:29:07.000000 arasea-3.0.6/arasea/tensor/subtensor.py
--rw-r--r--   0 arkanepetra  (1000) arkanepetra  (1000)      262 2024-04-25 08:29:07.000000 arasea-3.0.6/arasea/tensor/subtensor_opt.py
--rw-r--r--   0 arkanepetra  (1000) arkanepetra  (1000)    41188 2024-04-25 08:29:07.000000 arasea-3.0.6/arasea/tensor/type.py
--rw-r--r--   0 arkanepetra  (1000) arkanepetra  (1000)     4088 2024-04-25 08:29:07.000000 arasea-3.0.6/arasea/tensor/type_other.py
--rw-r--r--   0 arkanepetra  (1000) arkanepetra  (1000)     3211 2024-04-25 08:29:07.000000 arasea-3.0.6/arasea/tensor/utils.py
--rw-r--r--   0 arkanepetra  (1000) arkanepetra  (1000)    37592 2024-04-25 08:29:07.000000 arasea-3.0.6/arasea/tensor/var.py
--rw-r--r--   0 arkanepetra  (1000) arkanepetra  (1000)     1831 2024-04-25 08:29:07.000000 arasea-3.0.6/arasea/tensor/xlogx.py
-drwxrwxr-x   0 arkanepetra  (1000) arkanepetra  (1000)        0 2024-04-30 15:26:15.712288 arasea-3.0.6/arasea/typed_list/
--rw-r--r--   0 arkanepetra  (1000) arkanepetra  (1000)      127 2024-04-25 08:29:07.000000 arasea-3.0.6/arasea/typed_list/__init__.py
--rw-r--r--   0 arkanepetra  (1000) arkanepetra  (1000)    18222 2024-04-25 08:29:07.000000 arasea-3.0.6/arasea/typed_list/basic.py
--rw-r--r--   0 arkanepetra  (1000) arkanepetra  (1000)      779 2024-04-25 08:29:07.000000 arasea-3.0.6/arasea/typed_list/rewriting.py
--rw-r--r--   0 arkanepetra  (1000) arkanepetra  (1000)     3933 2024-04-25 08:29:07.000000 arasea-3.0.6/arasea/typed_list/type.py
--rw-r--r--   0 arkanepetra  (1000) arkanepetra  (1000)     2924 2024-04-25 08:29:07.000000 arasea-3.0.6/arasea/updates.py
--rw-r--r--   0 arkanepetra  (1000) arkanepetra  (1000)    13640 2024-04-25 08:29:07.000000 arasea-3.0.6/arasea/utils.py
--rw-r--r--   0 arkanepetra  (1000) arkanepetra  (1000)      962 2024-04-30 15:25:53.000000 arasea-3.0.6/arasea/version.py
-drwxrwxr-x   0 arkanepetra  (1000) arkanepetra  (1000)        0 2024-04-30 15:26:15.766294 arasea-3.0.6/arasea.egg-info/
--rw-r--r--   0 arkanepetra  (1000) arkanepetra  (1000)     1660 2024-04-30 15:26:15.000000 arasea-3.0.6/arasea.egg-info/PKG-INFO
--rw-rw-r--   0 arkanepetra  (1000) arkanepetra  (1000)    11411 2024-04-30 15:26:15.000000 arasea-3.0.6/arasea.egg-info/SOURCES.txt
--rw-rw-r--   0 arkanepetra  (1000) arkanepetra  (1000)        1 2024-04-30 15:26:15.000000 arasea-3.0.6/arasea.egg-info/dependency_links.txt
--rw-rw-r--   0 arkanepetra  (1000) arkanepetra  (1000)       86 2024-04-30 15:26:15.000000 arasea-3.0.6/arasea.egg-info/requires.txt
--rw-rw-r--   0 arkanepetra  (1000) arkanepetra  (1000)       17 2024-04-30 15:26:15.000000 arasea-3.0.6/arasea.egg-info/top_level.txt
-drwxrwxr-x   0 arkanepetra  (1000) arkanepetra  (1000)        0 2024-04-30 15:26:15.713289 arasea-3.0.6/bin/
--rw-r--r--   0 arkanepetra  (1000) arkanepetra  (1000)      239 2024-04-25 08:29:07.000000 arasea-3.0.6/bin/__init__.py
--rw-r--r--   0 arkanepetra  (1000) arkanepetra  (1000)      332 2024-04-25 08:29:07.000000 arasea-3.0.6/bin/arasea_cache.py
--rw-rw-r--   0 arkanepetra  (1000) arkanepetra  (1000)       38 2024-04-30 15:26:15.767294 arasea-3.0.6/setup.cfg
--rw-r--r--   0 arkanepetra  (1000) arkanepetra  (1000)     2384 2024-04-30 15:26:02.000000 arasea-3.0.6/setup.py
-drwxrwxr-x   0 arkanepetra  (1000) arkanepetra  (1000)        0 2024-04-30 15:26:15.716289 arasea-3.0.6/tests/
--rw-r--r--   0 arkanepetra  (1000) arkanepetra  (1000)        0 2024-04-25 08:29:08.000000 arasea-3.0.6/tests/__init__.py
-drwxrwxr-x   0 arkanepetra  (1000) arkanepetra  (1000)        0 2024-04-30 15:26:15.719289 arasea-3.0.6/tests/compile/
--rw-r--r--   0 arkanepetra  (1000) arkanepetra  (1000)        0 2024-04-25 08:29:08.000000 arasea-3.0.6/tests/compile/__init__.py
-drwxrwxr-x   0 arkanepetra  (1000) arkanepetra  (1000)        0 2024-04-30 15:26:15.720289 arasea-3.0.6/tests/compile/function/
--rw-r--r--   0 arkanepetra  (1000) arkanepetra  (1000)        0 2024-04-25 08:29:08.000000 arasea-3.0.6/tests/compile/function/__init__.py
--rw-r--r--   0 arkanepetra  (1000) arkanepetra  (1000)     7284 2024-04-25 08:29:08.000000 arasea-3.0.6/tests/compile/function/test_function.py
--rw-r--r--   0 arkanepetra  (1000) arkanepetra  (1000)    36404 2024-04-25 08:29:08.000000 arasea-3.0.6/tests/compile/function/test_pfunc.py
--rw-r--r--   0 arkanepetra  (1000) arkanepetra  (1000)    42215 2024-04-25 08:29:08.000000 arasea-3.0.6/tests/compile/function/test_types.py
--rw-r--r--   0 arkanepetra  (1000) arkanepetra  (1000)    24285 2024-04-25 08:29:08.000000 arasea-3.0.6/tests/compile/test_builders.py
--rw-r--r--   0 arkanepetra  (1000) arkanepetra  (1000)     3917 2024-04-25 08:29:08.000000 arasea-3.0.6/tests/compile/test_compilelock.py
--rw-r--r--   0 arkanepetra  (1000) arkanepetra  (1000)    25864 2024-04-25 08:29:08.000000 arasea-3.0.6/tests/compile/test_debugmode.py
--rw-r--r--   0 arkanepetra  (1000) arkanepetra  (1000)     2927 2024-04-25 08:29:08.000000 arasea-3.0.6/tests/compile/test_misc.py
--rw-r--r--   0 arkanepetra  (1000) arkanepetra  (1000)     4687 2024-04-25 08:29:08.000000 arasea-3.0.6/tests/compile/test_mode.py
--rw-r--r--   0 arkanepetra  (1000) arkanepetra  (1000)     3259 2024-04-25 08:29:08.000000 arasea-3.0.6/tests/compile/test_monitormode.py
--rw-r--r--   0 arkanepetra  (1000) arkanepetra  (1000)     2479 2024-04-25 08:29:08.000000 arasea-3.0.6/tests/compile/test_nanguardmode.py
--rw-r--r--   0 arkanepetra  (1000) arkanepetra  (1000)     2026 2024-04-25 08:29:08.000000 arasea-3.0.6/tests/compile/test_ops.py
--rw-r--r--   0 arkanepetra  (1000) arkanepetra  (1000)     3557 2024-04-25 08:29:08.000000 arasea-3.0.6/tests/compile/test_profiling.py
--rw-r--r--   0 arkanepetra  (1000) arkanepetra  (1000)    10290 2024-04-25 08:29:08.000000 arasea-3.0.6/tests/compile/test_shared.py
-drwxrwxr-x   0 arkanepetra  (1000) arkanepetra  (1000)        0 2024-04-30 15:26:15.722290 arasea-3.0.6/tests/d3viz/
--rw-r--r--   0 arkanepetra  (1000) arkanepetra  (1000)        0 2024-04-25 08:29:08.000000 arasea-3.0.6/tests/d3viz/__init__.py
--rw-r--r--   0 arkanepetra  (1000) arkanepetra  (1000)     1746 2024-04-25 08:29:08.000000 arasea-3.0.6/tests/d3viz/models.py
--rw-r--r--   0 arkanepetra  (1000) arkanepetra  (1000)     1790 2024-04-25 08:29:08.000000 arasea-3.0.6/tests/d3viz/test_d3viz.py
--rw-r--r--   0 arkanepetra  (1000) arkanepetra  (1000)     2102 2024-04-25 08:29:08.000000 arasea-3.0.6/tests/d3viz/test_formatting.py
-drwxrwxr-x   0 arkanepetra  (1000) arkanepetra  (1000)        0 2024-04-30 15:26:15.725290 arasea-3.0.6/tests/graph/
--rw-r--r--   0 arkanepetra  (1000) arkanepetra  (1000)        0 2024-04-25 08:29:08.000000 arasea-3.0.6/tests/graph/__init__.py
-drwxrwxr-x   0 arkanepetra  (1000) arkanepetra  (1000)        0 2024-04-30 15:26:15.727290 arasea-3.0.6/tests/graph/rewriting/
--rw-r--r--   0 arkanepetra  (1000) arkanepetra  (1000)        0 2024-04-25 08:29:08.000000 arasea-3.0.6/tests/graph/rewriting/__init__.py
--rw-r--r--   0 arkanepetra  (1000) arkanepetra  (1000)    28891 2024-04-25 08:29:08.000000 arasea-3.0.6/tests/graph/rewriting/test_basic.py
--rw-r--r--   0 arkanepetra  (1000) arkanepetra  (1000)     2890 2024-04-25 08:29:08.000000 arasea-3.0.6/tests/graph/rewriting/test_db.py
--rw-r--r--   0 arkanepetra  (1000) arkanepetra  (1000)     5385 2024-04-25 08:29:08.000000 arasea-3.0.6/tests/graph/rewriting/test_kanren.py
--rw-r--r--   0 arkanepetra  (1000) arkanepetra  (1000)     8469 2024-04-25 08:29:08.000000 arasea-3.0.6/tests/graph/rewriting/test_unify.py
--rw-r--r--   0 arkanepetra  (1000) arkanepetra  (1000)     5006 2024-04-25 08:29:08.000000 arasea-3.0.6/tests/graph/rewriting/test_utils.py
--rw-r--r--   0 arkanepetra  (1000) arkanepetra  (1000)    23703 2024-04-25 08:29:08.000000 arasea-3.0.6/tests/graph/test_basic.py
--rw-r--r--   0 arkanepetra  (1000) arkanepetra  (1000)    10663 2024-04-25 08:29:08.000000 arasea-3.0.6/tests/graph/test_compute_test_value.py
--rw-r--r--   0 arkanepetra  (1000) arkanepetra  (1000)    14846 2024-04-25 08:29:08.000000 arasea-3.0.6/tests/graph/test_destroyhandler.py
--rw-r--r--   0 arkanepetra  (1000) arkanepetra  (1000)     6933 2024-04-25 08:29:08.000000 arasea-3.0.6/tests/graph/test_features.py
--rw-r--r--   0 arkanepetra  (1000) arkanepetra  (1000)    22433 2024-04-25 08:29:08.000000 arasea-3.0.6/tests/graph/test_fg.py
--rw-r--r--   0 arkanepetra  (1000) arkanepetra  (1000)     6511 2024-04-25 08:29:08.000000 arasea-3.0.6/tests/graph/test_op.py
--rw-r--r--   0 arkanepetra  (1000) arkanepetra  (1000)     2089 2024-04-25 08:29:08.000000 arasea-3.0.6/tests/graph/test_sched.py
--rw-r--r--   0 arkanepetra  (1000) arkanepetra  (1000)     1326 2024-04-25 08:29:08.000000 arasea-3.0.6/tests/graph/test_types.py
--rw-r--r--   0 arkanepetra  (1000) arkanepetra  (1000)      389 2024-04-25 08:29:08.000000 arasea-3.0.6/tests/graph/test_utils.py
--rw-r--r--   0 arkanepetra  (1000) arkanepetra  (1000)     4119 2024-04-25 08:29:08.000000 arasea-3.0.6/tests/graph/utils.py
-drwxrwxr-x   0 arkanepetra  (1000) arkanepetra  (1000)        0 2024-04-30 15:26:15.728290 arasea-3.0.6/tests/link/
--rw-r--r--   0 arkanepetra  (1000) arkanepetra  (1000)        0 2024-04-25 08:29:08.000000 arasea-3.0.6/tests/link/__init__.py
-drwxrwxr-x   0 arkanepetra  (1000) arkanepetra  (1000)        0 2024-04-30 15:26:15.729290 arasea-3.0.6/tests/link/c/
--rw-r--r--   0 arkanepetra  (1000) arkanepetra  (1000)        0 2024-04-25 08:29:08.000000 arasea-3.0.6/tests/link/c/__init__.py
--rw-r--r--   0 arkanepetra  (1000) arkanepetra  (1000)    13074 2024-04-25 08:29:08.000000 arasea-3.0.6/tests/link/c/test_basic.py
--rw-r--r--   0 arkanepetra  (1000) arkanepetra  (1000)     9069 2024-04-25 08:29:08.000000 arasea-3.0.6/tests/link/c/test_cmodule.py
--rw-r--r--   0 arkanepetra  (1000) arkanepetra  (1000)     6848 2024-04-25 08:29:08.000000 arasea-3.0.6/tests/link/c/test_op.py
--rw-r--r--   0 arkanepetra  (1000) arkanepetra  (1000)    12881 2024-04-25 08:29:08.000000 arasea-3.0.6/tests/link/c/test_params_type.py
--rw-r--r--   0 arkanepetra  (1000) arkanepetra  (1000)     8730 2024-04-25 08:29:08.000000 arasea-3.0.6/tests/link/c/test_type.py
-drwxrwxr-x   0 arkanepetra  (1000) arkanepetra  (1000)        0 2024-04-30 15:26:15.733291 arasea-3.0.6/tests/link/numba/
--rw-r--r--   0 arkanepetra  (1000) arkanepetra  (1000)        0 2024-04-25 08:29:08.000000 arasea-3.0.6/tests/link/numba/__init__.py
--rw-r--r--   0 arkanepetra  (1000) arkanepetra  (1000)    30411 2024-04-25 08:29:08.000000 arasea-3.0.6/tests/link/numba/test_basic.py
--rw-r--r--   0 arkanepetra  (1000) arkanepetra  (1000)    15952 2024-04-25 08:29:08.000000 arasea-3.0.6/tests/link/numba/test_elemwise.py
--rw-r--r--   0 arkanepetra  (1000) arkanepetra  (1000)    13197 2024-04-25 08:29:08.000000 arasea-3.0.6/tests/link/numba/test_extra_ops.py
--rw-r--r--   0 arkanepetra  (1000) arkanepetra  (1000)    12589 2024-04-25 08:29:08.000000 arasea-3.0.6/tests/link/numba/test_nlinalg.py
--rw-r--r--   0 arkanepetra  (1000) arkanepetra  (1000)     2038 2024-04-25 08:29:08.000000 arasea-3.0.6/tests/link/numba/test_performance.py
--rw-r--r--   0 arkanepetra  (1000) arkanepetra  (1000)    16845 2024-04-25 08:29:08.000000 arasea-3.0.6/tests/link/numba/test_random.py
--rw-r--r--   0 arkanepetra  (1000) arkanepetra  (1000)     4012 2024-04-25 08:29:08.000000 arasea-3.0.6/tests/link/numba/test_scalar.py
--rw-r--r--   0 arkanepetra  (1000) arkanepetra  (1000)    10723 2024-04-25 08:29:08.000000 arasea-3.0.6/tests/link/numba/test_scan.py
--rw-r--r--   0 arkanepetra  (1000) arkanepetra  (1000)     2353 2024-04-25 08:29:08.000000 arasea-3.0.6/tests/link/numba/test_sparse.py
--rw-r--r--   0 arkanepetra  (1000) arkanepetra  (1000)    10235 2024-04-25 08:29:08.000000 arasea-3.0.6/tests/link/numba/test_tensor_basic.py
--rw-r--r--   0 arkanepetra  (1000) arkanepetra  (1000)     7491 2024-04-25 08:29:08.000000 arasea-3.0.6/tests/link/test_link.py
--rw-r--r--   0 arkanepetra  (1000) arkanepetra  (1000)     5653 2024-04-25 08:29:08.000000 arasea-3.0.6/tests/link/test_utils.py
--rw-r--r--   0 arkanepetra  (1000) arkanepetra  (1000)    14430 2024-04-25 08:29:08.000000 arasea-3.0.6/tests/link/test_vm.py
-drwxrwxr-x   0 arkanepetra  (1000) arkanepetra  (1000)        0 2024-04-30 15:26:15.734291 arasea-3.0.6/tests/misc/
--rw-r--r--   0 arkanepetra  (1000) arkanepetra  (1000)        0 2024-04-25 08:29:08.000000 arasea-3.0.6/tests/misc/__init__.py
--rw-r--r--   0 arkanepetra  (1000) arkanepetra  (1000)     3533 2024-04-25 08:29:08.000000 arasea-3.0.6/tests/misc/test_may_share_memory.py
--rw-r--r--   0 arkanepetra  (1000) arkanepetra  (1000)     2212 2024-04-25 08:29:08.000000 arasea-3.0.6/tests/misc/test_pkl_utils.py
-drwxrwxr-x   0 arkanepetra  (1000) arkanepetra  (1000)        0 2024-04-30 15:26:15.735291 arasea-3.0.6/tests/sandbox/
--rw-r--r--   0 arkanepetra  (1000) arkanepetra  (1000)        0 2024-04-25 08:29:08.000000 arasea-3.0.6/tests/sandbox/__init__.py
-drwxrwxr-x   0 arkanepetra  (1000) arkanepetra  (1000)        0 2024-04-30 15:26:15.736291 arasea-3.0.6/tests/sandbox/linalg/
--rw-r--r--   0 arkanepetra  (1000) arkanepetra  (1000)        0 2024-04-25 08:29:08.000000 arasea-3.0.6/tests/sandbox/linalg/__init__.py
--rw-r--r--   0 arkanepetra  (1000) arkanepetra  (1000)     4367 2024-04-25 08:29:08.000000 arasea-3.0.6/tests/sandbox/linalg/test_linalg.py
--rw-r--r--   0 arkanepetra  (1000) arkanepetra  (1000)      836 2024-04-25 08:29:08.000000 arasea-3.0.6/tests/sandbox/test_minimal.py
--rw-r--r--   0 arkanepetra  (1000) arkanepetra  (1000)     3777 2024-04-25 08:29:08.000000 arasea-3.0.6/tests/sandbox/test_multinomial.py
--rw-r--r--   0 arkanepetra  (1000) arkanepetra  (1000)     7233 2024-04-25 08:29:08.000000 arasea-3.0.6/tests/sandbox/test_multinomial_wo_replacement.py
--rw-r--r--   0 arkanepetra  (1000) arkanepetra  (1000)    34649 2024-04-25 08:29:08.000000 arasea-3.0.6/tests/sandbox/test_rng_mrg.py
-drwxrwxr-x   0 arkanepetra  (1000) arkanepetra  (1000)        0 2024-04-30 15:26:15.737291 arasea-3.0.6/tests/scalar/
--rw-r--r--   0 arkanepetra  (1000) arkanepetra  (1000)        0 2024-04-25 08:29:08.000000 arasea-3.0.6/tests/scalar/__init__.py
--rw-r--r--   0 arkanepetra  (1000) arkanepetra  (1000)    16995 2024-04-25 08:29:08.000000 arasea-3.0.6/tests/scalar/test_basic.py
--rw-r--r--   0 arkanepetra  (1000) arkanepetra  (1000)      991 2024-04-25 08:29:08.000000 arasea-3.0.6/tests/scalar/test_basic_sympy.py
--rw-r--r--   0 arkanepetra  (1000) arkanepetra  (1000)     2539 2024-04-25 08:29:08.000000 arasea-3.0.6/tests/scalar/test_math.py
--rw-r--r--   0 arkanepetra  (1000) arkanepetra  (1000)     1897 2024-04-25 08:29:08.000000 arasea-3.0.6/tests/scalar/test_type.py
-drwxrwxr-x   0 arkanepetra  (1000) arkanepetra  (1000)        0 2024-04-30 15:26:15.739291 arasea-3.0.6/tests/scan/
--rw-r--r--   0 arkanepetra  (1000) arkanepetra  (1000)        0 2024-04-25 08:29:08.000000 arasea-3.0.6/tests/scan/__init__.py
--rw-r--r--   0 arkanepetra  (1000) arkanepetra  (1000)   133995 2024-04-25 08:29:08.000000 arasea-3.0.6/tests/scan/test_basic.py
--rw-r--r--   0 arkanepetra  (1000) arkanepetra  (1000)     1777 2024-04-25 08:29:08.000000 arasea-3.0.6/tests/scan/test_checkpoints.py
--rw-r--r--   0 arkanepetra  (1000) arkanepetra  (1000)    25319 2024-04-25 08:29:08.000000 arasea-3.0.6/tests/scan/test_printing.py
--rw-r--r--   0 arkanepetra  (1000) arkanepetra  (1000)    56551 2024-04-25 08:29:08.000000 arasea-3.0.6/tests/scan/test_rewriting.py
--rw-r--r--   0 arkanepetra  (1000) arkanepetra  (1000)    17205 2024-04-25 08:29:08.000000 arasea-3.0.6/tests/scan/test_utils.py
--rw-r--r--   0 arkanepetra  (1000) arkanepetra  (1000)     4534 2024-04-25 08:29:08.000000 arasea-3.0.6/tests/scan/test_views.py
-drwxrwxr-x   0 arkanepetra  (1000) arkanepetra  (1000)        0 2024-04-30 15:26:15.742292 arasea-3.0.6/tests/sparse/
--rw-r--r--   0 arkanepetra  (1000) arkanepetra  (1000)        0 2024-04-25 08:29:08.000000 arasea-3.0.6/tests/sparse/__init__.py
-drwxrwxr-x   0 arkanepetra  (1000) arkanepetra  (1000)        0 2024-04-30 15:26:15.743292 arasea-3.0.6/tests/sparse/sandbox/
--rw-r--r--   0 arkanepetra  (1000) arkanepetra  (1000)        0 2024-04-25 08:29:08.000000 arasea-3.0.6/tests/sparse/sandbox/__init__.py
--rw-r--r--   0 arkanepetra  (1000) arkanepetra  (1000)     9198 2024-04-25 08:29:08.000000 arasea-3.0.6/tests/sparse/sandbox/test_sp.py
--rw-r--r--   0 arkanepetra  (1000) arkanepetra  (1000)   116949 2024-04-25 08:29:08.000000 arasea-3.0.6/tests/sparse/test_basic.py
--rw-r--r--   0 arkanepetra  (1000) arkanepetra  (1000)     5942 2024-04-25 08:29:08.000000 arasea-3.0.6/tests/sparse/test_rewriting.py
--rw-r--r--   0 arkanepetra  (1000) arkanepetra  (1000)      373 2024-04-25 08:29:08.000000 arasea-3.0.6/tests/sparse/test_sharedvar.py
--rw-r--r--   0 arkanepetra  (1000) arkanepetra  (1000)     4094 2024-04-25 08:29:08.000000 arasea-3.0.6/tests/sparse/test_sp2.py
--rw-r--r--   0 arkanepetra  (1000) arkanepetra  (1000)     2485 2024-04-25 08:29:08.000000 arasea-3.0.6/tests/sparse/test_type.py
--rw-r--r--   0 arkanepetra  (1000) arkanepetra  (1000)     1608 2024-04-25 08:29:08.000000 arasea-3.0.6/tests/sparse/test_utils.py
--rw-r--r--   0 arkanepetra  (1000) arkanepetra  (1000)     8061 2024-04-25 08:29:08.000000 arasea-3.0.6/tests/sparse/test_var.py
-drwxrwxr-x   0 arkanepetra  (1000) arkanepetra  (1000)        0 2024-04-30 15:26:15.754293 arasea-3.0.6/tests/tensor/
--rw-r--r--   0 arkanepetra  (1000) arkanepetra  (1000)        0 2024-04-25 08:29:08.000000 arasea-3.0.6/tests/tensor/__init__.py
--rw-r--r--   0 arkanepetra  (1000) arkanepetra  (1000)     1475 2024-04-25 08:29:08.000000 arasea-3.0.6/tests/tensor/_test_mpi_roundtrip.py
-drwxrwxr-x   0 arkanepetra  (1000) arkanepetra  (1000)        0 2024-04-30 15:26:15.758293 arasea-3.0.6/tests/tensor/nnet/
--rw-r--r--   0 arkanepetra  (1000) arkanepetra  (1000)        0 2024-04-25 08:29:08.000000 arasea-3.0.6/tests/tensor/nnet/__init__.py
--rw-r--r--   0 arkanepetra  (1000) arkanepetra  (1000)    15242 2024-04-25 08:29:08.000000 arasea-3.0.6/tests/tensor/nnet/speed_test_conv.py
--rw-r--r--   0 arkanepetra  (1000) arkanepetra  (1000)   103862 2024-04-25 08:29:08.000000 arasea-3.0.6/tests/tensor/nnet/test_abstract_conv.py
--rw-r--r--   0 arkanepetra  (1000) arkanepetra  (1000)    42020 2024-04-25 08:29:08.000000 arasea-3.0.6/tests/tensor/nnet/test_basic.py
--rw-r--r--   0 arkanepetra  (1000) arkanepetra  (1000)    25674 2024-04-25 08:29:08.000000 arasea-3.0.6/tests/tensor/nnet/test_batchnorm.py
--rw-r--r--   0 arkanepetra  (1000) arkanepetra  (1000)    10203 2024-04-25 08:29:08.000000 arasea-3.0.6/tests/tensor/nnet/test_blocksparse.py
--rw-r--r--   0 arkanepetra  (1000) arkanepetra  (1000)    28956 2024-04-25 08:29:08.000000 arasea-3.0.6/tests/tensor/nnet/test_conv.py
--rw-r--r--   0 arkanepetra  (1000) arkanepetra  (1000)     6947 2024-04-25 08:29:08.000000 arasea-3.0.6/tests/tensor/nnet/test_conv3d2d.py
--rw-r--r--   0 arkanepetra  (1000) arkanepetra  (1000)    21906 2024-04-25 08:29:08.000000 arasea-3.0.6/tests/tensor/nnet/test_corr.py
--rw-r--r--   0 arkanepetra  (1000) arkanepetra  (1000)    21818 2024-04-25 08:29:08.000000 arasea-3.0.6/tests/tensor/nnet/test_corr3d.py
--rw-r--r--   0 arkanepetra  (1000) arkanepetra  (1000)     6197 2024-04-25 08:29:08.000000 arasea-3.0.6/tests/tensor/nnet/test_ctc.py
--rw-r--r--   0 arkanepetra  (1000) arkanepetra  (1000)    25410 2024-04-25 08:29:08.000000 arasea-3.0.6/tests/tensor/nnet/test_neighbours.py
--rw-r--r--   0 arkanepetra  (1000) arkanepetra  (1000)     1694 2024-04-25 08:29:08.000000 arasea-3.0.6/tests/tensor/nnet/test_rewriting.py
--rw-r--r--   0 arkanepetra  (1000) arkanepetra  (1000)     4825 2024-04-25 08:29:08.000000 arasea-3.0.6/tests/tensor/nnet/test_sigm.py
-drwxrwxr-x   0 arkanepetra  (1000) arkanepetra  (1000)        0 2024-04-30 15:26:15.761294 arasea-3.0.6/tests/tensor/random/
--rw-r--r--   0 arkanepetra  (1000) arkanepetra  (1000)        0 2024-04-25 08:29:08.000000 arasea-3.0.6/tests/tensor/random/__init__.py
--rw-r--r--   0 arkanepetra  (1000) arkanepetra  (1000)    41757 2024-04-25 08:29:08.000000 arasea-3.0.6/tests/tensor/random/test_basic.py
--rw-r--r--   0 arkanepetra  (1000) arkanepetra  (1000)     5974 2024-04-25 08:29:08.000000 arasea-3.0.6/tests/tensor/random/test_op.py
--rw-r--r--   0 arkanepetra  (1000) arkanepetra  (1000)    17712 2024-04-25 08:29:08.000000 arasea-3.0.6/tests/tensor/random/test_rewriting.py
--rw-r--r--   0 arkanepetra  (1000) arkanepetra  (1000)     6674 2024-04-25 08:29:08.000000 arasea-3.0.6/tests/tensor/random/test_type.py
--rw-r--r--   0 arkanepetra  (1000) arkanepetra  (1000)    10653 2024-04-25 08:29:08.000000 arasea-3.0.6/tests/tensor/random/test_utils.py
--rw-r--r--   0 arkanepetra  (1000) arkanepetra  (1000)     3642 2024-04-25 08:29:08.000000 arasea-3.0.6/tests/tensor/random/test_var.py
-drwxrwxr-x   0 arkanepetra  (1000) arkanepetra  (1000)        0 2024-04-30 15:26:15.764294 arasea-3.0.6/tests/tensor/rewriting/
--rw-r--r--   0 arkanepetra  (1000) arkanepetra  (1000)        0 2024-04-25 08:29:08.000000 arasea-3.0.6/tests/tensor/rewriting/__init__.py
--rw-r--r--   0 arkanepetra  (1000) arkanepetra  (1000)    63207 2024-04-25 08:29:08.000000 arasea-3.0.6/tests/tensor/rewriting/test_basic.py
--rw-r--r--   0 arkanepetra  (1000) arkanepetra  (1000)    41140 2024-04-25 08:29:08.000000 arasea-3.0.6/tests/tensor/rewriting/test_elemwise.py
--rw-r--r--   0 arkanepetra  (1000) arkanepetra  (1000)    10481 2024-04-25 08:29:08.000000 arasea-3.0.6/tests/tensor/rewriting/test_extra_ops.py
--rw-r--r--   0 arkanepetra  (1000) arkanepetra  (1000)   166414 2024-04-25 08:29:08.000000 arasea-3.0.6/tests/tensor/rewriting/test_math.py
--rw-r--r--   0 arkanepetra  (1000) arkanepetra  (1000)    18170 2024-04-25 08:29:08.000000 arasea-3.0.6/tests/tensor/rewriting/test_shape.py
--rw-r--r--   0 arkanepetra  (1000) arkanepetra  (1000)     4483 2024-04-25 08:29:08.000000 arasea-3.0.6/tests/tensor/rewriting/test_special.py
--rw-r--r--   0 arkanepetra  (1000) arkanepetra  (1000)    80378 2024-04-25 08:29:08.000000 arasea-3.0.6/tests/tensor/rewriting/test_subtensor.py
--rw-r--r--   0 arkanepetra  (1000) arkanepetra  (1000)     7105 2024-04-25 08:29:08.000000 arasea-3.0.6/tests/tensor/rewriting/test_uncanonicalize.py
-drwxrwxr-x   0 arkanepetra  (1000) arkanepetra  (1000)        0 2024-04-30 15:26:15.765294 arasea-3.0.6/tests/tensor/signal/
--rw-r--r--   0 arkanepetra  (1000) arkanepetra  (1000)        0 2024-04-25 08:29:08.000000 arasea-3.0.6/tests/tensor/signal/__init__.py
--rw-r--r--   0 arkanepetra  (1000) arkanepetra  (1000)     4145 2024-04-25 08:29:08.000000 arasea-3.0.6/tests/tensor/signal/test_conv.py
--rw-r--r--   0 arkanepetra  (1000) arkanepetra  (1000)    51694 2024-04-25 08:29:08.000000 arasea-3.0.6/tests/tensor/signal/test_pool.py
--rw-r--r--   0 arkanepetra  (1000) arkanepetra  (1000)   148595 2024-04-25 08:29:08.000000 arasea-3.0.6/tests/tensor/test_basic.py
--rw-r--r--   0 arkanepetra  (1000) arkanepetra  (1000)    99618 2024-04-25 08:29:08.000000 arasea-3.0.6/tests/tensor/test_blas.py
--rw-r--r--   0 arkanepetra  (1000) arkanepetra  (1000)    14554 2024-04-25 08:29:08.000000 arasea-3.0.6/tests/tensor/test_blas_c.py
--rw-r--r--   0 arkanepetra  (1000) arkanepetra  (1000)     2550 2024-04-25 08:29:08.000000 arasea-3.0.6/tests/tensor/test_blas_scipy.py
--rw-r--r--   0 arkanepetra  (1000) arkanepetra  (1000)     4161 2024-04-25 08:29:08.000000 arasea-3.0.6/tests/tensor/test_casting.py
--rw-r--r--   0 arkanepetra  (1000) arkanepetra  (1000)     4344 2024-04-25 08:29:08.000000 arasea-3.0.6/tests/tensor/test_complex.py
--rw-r--r--   0 arkanepetra  (1000) arkanepetra  (1000)    34431 2024-04-25 08:29:08.000000 arasea-3.0.6/tests/tensor/test_elemwise.py
--rw-r--r--   0 arkanepetra  (1000) arkanepetra  (1000)    47330 2024-04-25 08:29:08.000000 arasea-3.0.6/tests/tensor/test_extra_ops.py
--rw-r--r--   0 arkanepetra  (1000) arkanepetra  (1000)     6580 2024-04-25 08:29:08.000000 arasea-3.0.6/tests/tensor/test_fft.py
--rw-r--r--   0 arkanepetra  (1000) arkanepetra  (1000)     2218 2024-04-25 08:29:08.000000 arasea-3.0.6/tests/tensor/test_fourier.py
--rw-r--r--   0 arkanepetra  (1000) arkanepetra  (1000)     4059 2024-04-25 08:29:08.000000 arasea-3.0.6/tests/tensor/test_gc.py
--rw-r--r--   0 arkanepetra  (1000) arkanepetra  (1000)    11957 2024-04-25 08:29:08.000000 arasea-3.0.6/tests/tensor/test_inplace.py
--rw-r--r--   0 arkanepetra  (1000) arkanepetra  (1000)     2080 2024-04-25 08:29:08.000000 arasea-3.0.6/tests/tensor/test_io.py
--rw-r--r--   0 arkanepetra  (1000) arkanepetra  (1000)     6667 2024-04-25 08:29:08.000000 arasea-3.0.6/tests/tensor/test_keepdims.py
--rw-r--r--   0 arkanepetra  (1000) arkanepetra  (1000)   123957 2024-04-25 08:29:08.000000 arasea-3.0.6/tests/tensor/test_math.py
--rw-r--r--   0 arkanepetra  (1000) arkanepetra  (1000)    29972 2024-04-25 08:29:08.000000 arasea-3.0.6/tests/tensor/test_math_scipy.py
--rw-r--r--   0 arkanepetra  (1000) arkanepetra  (1000)     2345 2024-04-25 08:29:08.000000 arasea-3.0.6/tests/tensor/test_merge.py
--rw-r--r--   0 arkanepetra  (1000) arkanepetra  (1000)     2467 2024-04-25 08:29:08.000000 arasea-3.0.6/tests/tensor/test_misc.py
--rw-r--r--   0 arkanepetra  (1000) arkanepetra  (1000)     2946 2024-04-25 08:29:08.000000 arasea-3.0.6/tests/tensor/test_mpi.py
--rw-r--r--   0 arkanepetra  (1000) arkanepetra  (1000)    14603 2024-04-25 08:29:08.000000 arasea-3.0.6/tests/tensor/test_nlinalg.py
--rw-r--r--   0 arkanepetra  (1000) arkanepetra  (1000)    22601 2024-04-25 08:29:08.000000 arasea-3.0.6/tests/tensor/test_shape.py
--rw-r--r--   0 arkanepetra  (1000) arkanepetra  (1000)    27332 2024-04-25 08:29:08.000000 arasea-3.0.6/tests/tensor/test_sharedvar.py
--rw-r--r--   0 arkanepetra  (1000) arkanepetra  (1000)    18787 2024-04-25 08:29:08.000000 arasea-3.0.6/tests/tensor/test_slinalg.py
--rw-r--r--   0 arkanepetra  (1000) arkanepetra  (1000)    18538 2024-04-25 08:29:08.000000 arasea-3.0.6/tests/tensor/test_sort.py
--rw-r--r--   0 arkanepetra  (1000) arkanepetra  (1000)     5148 2024-04-25 08:29:08.000000 arasea-3.0.6/tests/tensor/test_special.py
--rw-r--r--   0 arkanepetra  (1000) arkanepetra  (1000)    91185 2024-04-25 08:29:08.000000 arasea-3.0.6/tests/tensor/test_subtensor.py
--rw-r--r--   0 arkanepetra  (1000) arkanepetra  (1000)     9802 2024-04-25 08:29:08.000000 arasea-3.0.6/tests/tensor/test_type.py
--rw-r--r--   0 arkanepetra  (1000) arkanepetra  (1000)     1766 2024-04-25 08:29:08.000000 arasea-3.0.6/tests/tensor/test_type_other.py
--rw-r--r--   0 arkanepetra  (1000) arkanepetra  (1000)     2417 2024-04-25 08:29:08.000000 arasea-3.0.6/tests/tensor/test_utils.py
--rw-r--r--   0 arkanepetra  (1000) arkanepetra  (1000)    12727 2024-04-25 08:29:08.000000 arasea-3.0.6/tests/tensor/test_var.py
--rw-r--r--   0 arkanepetra  (1000) arkanepetra  (1000)      716 2024-04-25 08:29:08.000000 arasea-3.0.6/tests/tensor/test_xlogx.py
--rw-r--r--   0 arkanepetra  (1000) arkanepetra  (1000)    38712 2024-04-25 08:29:08.000000 arasea-3.0.6/tests/tensor/utils.py
--rw-r--r--   0 arkanepetra  (1000) arkanepetra  (1000)     2922 2024-04-25 08:29:08.000000 arasea-3.0.6/tests/test_breakpoint.py
--rw-r--r--   0 arkanepetra  (1000) arkanepetra  (1000)    10470 2024-04-25 08:29:08.000000 arasea-3.0.6/tests/test_config.py
--rw-r--r--   0 arkanepetra  (1000) arkanepetra  (1000)    34472 2024-04-25 08:29:08.000000 arasea-3.0.6/tests/test_gradient.py
--rw-r--r--   0 arkanepetra  (1000) arkanepetra  (1000)    25050 2024-04-25 08:29:08.000000 arasea-3.0.6/tests/test_ifelse.py
--rw-r--r--   0 arkanepetra  (1000) arkanepetra  (1000)    13025 2024-04-25 08:29:08.000000 arasea-3.0.6/tests/test_printing.py
--rw-r--r--   0 arkanepetra  (1000) arkanepetra  (1000)     5383 2024-04-25 08:29:08.000000 arasea-3.0.6/tests/test_raise_op.py
--rw-r--r--   0 arkanepetra  (1000) arkanepetra  (1000)    13207 2024-04-25 08:29:08.000000 arasea-3.0.6/tests/test_rop.py
--rw-r--r--   0 arkanepetra  (1000) arkanepetra  (1000)     1679 2024-04-25 08:29:08.000000 arasea-3.0.6/tests/test_updates.py
-drwxrwxr-x   0 arkanepetra  (1000) arkanepetra  (1000)        0 2024-04-30 15:26:15.766294 arasea-3.0.6/tests/typed_list/
--rw-r--r--   0 arkanepetra  (1000) arkanepetra  (1000)        0 2024-04-25 08:29:08.000000 arasea-3.0.6/tests/typed_list/__init__.py
--rw-r--r--   0 arkanepetra  (1000) arkanepetra  (1000)    17535 2024-04-25 08:29:08.000000 arasea-3.0.6/tests/typed_list/test_basic.py
--rw-r--r--   0 arkanepetra  (1000) arkanepetra  (1000)     4926 2024-04-25 08:29:08.000000 arasea-3.0.6/tests/typed_list/test_rewriting.py
--rw-r--r--   0 arkanepetra  (1000) arkanepetra  (1000)     4903 2024-04-25 08:29:08.000000 arasea-3.0.6/tests/typed_list/test_type.py
--rw-r--r--   0 arkanepetra  (1000) arkanepetra  (1000)    14042 2024-04-25 08:29:08.000000 arasea-3.0.6/tests/unittest_tools.py
+drwxrwxr-x   0 arkanepetra  (1000) arkanepetra  (1000)        0 2024-05-29 05:48:23.788437 arasea-3.0.7/
+-rw-r--r--   0 arkanepetra  (1000) arkanepetra  (1000)     2515 2024-05-29 05:18:48.000000 arasea-3.0.7/LICENSE.txt
+-rw-r--r--   0 arkanepetra  (1000) arkanepetra  (1000)     1660 2024-05-29 05:48:23.788437 arasea-3.0.7/PKG-INFO
+-rw-r--r--   0 arkanepetra  (1000) arkanepetra  (1000)     5503 2024-05-29 05:18:48.000000 arasea-3.0.7/README.md
+drwxrwxr-x   0 arkanepetra  (1000) arkanepetra  (1000)        0 2024-05-29 05:48:23.673429 arasea-3.0.7/arasea/
+-rw-r--r--   0 arkanepetra  (1000) arkanepetra  (1000)     5760 2024-05-29 05:18:48.000000 arasea-3.0.7/arasea/__init__.py
+-rw-r--r--   0 arkanepetra  (1000) arkanepetra  (1000)      411 2024-05-29 05:30:29.000000 arasea-3.0.7/arasea/_version.py
+-rw-r--r--   0 arkanepetra  (1000) arkanepetra  (1000)      252 2024-05-29 05:18:48.000000 arasea-3.0.7/arasea/assert_op.py
+-rw-r--r--   0 arkanepetra  (1000) arkanepetra  (1000)     3561 2024-05-29 05:18:48.000000 arasea-3.0.7/arasea/benchmark.log
+drwxrwxr-x   0 arkanepetra  (1000) arkanepetra  (1000)        0 2024-05-29 05:48:23.676429 arasea-3.0.7/arasea/bin/
+-rw-r--r--   0 arkanepetra  (1000) arkanepetra  (1000)        0 2024-05-29 05:18:48.000000 arasea-3.0.7/arasea/bin/__init__.py
+-rw-r--r--   0 arkanepetra  (1000) arkanepetra  (1000)     4080 2024-05-29 05:18:48.000000 arasea-3.0.7/arasea/bin/arasea_cache.py
+-rw-r--r--   0 arkanepetra  (1000) arkanepetra  (1000)     6055 2024-05-29 05:18:48.000000 arasea-3.0.7/arasea/breakpoint.py
+drwxrwxr-x   0 arkanepetra  (1000) arkanepetra  (1000)        0 2024-05-29 05:48:23.680429 arasea-3.0.7/arasea/compile/
+-rw-r--r--   0 arkanepetra  (1000) arkanepetra  (1000)     1410 2024-05-29 05:18:48.000000 arasea-3.0.7/arasea/compile/__init__.py
+-rw-r--r--   0 arkanepetra  (1000) arkanepetra  (1000)    41442 2024-05-29 05:18:48.000000 arasea-3.0.7/arasea/compile/builders.py
+-rw-r--r--   0 arkanepetra  (1000) arkanepetra  (1000)     9954 2024-05-29 05:18:48.000000 arasea-3.0.7/arasea/compile/compiledir.py
+-rw-r--r--   0 arkanepetra  (1000) arkanepetra  (1000)     2041 2024-05-29 05:18:48.000000 arasea-3.0.7/arasea/compile/compilelock.py
+-rw-r--r--   0 arkanepetra  (1000) arkanepetra  (1000)    85654 2024-05-29 05:18:48.000000 arasea-3.0.7/arasea/compile/debugmode.py
+drwxrwxr-x   0 arkanepetra  (1000) arkanepetra  (1000)        0 2024-05-29 05:48:23.681429 arasea-3.0.7/arasea/compile/function/
+-rw-r--r--   0 arkanepetra  (1000) arkanepetra  (1000)    13377 2024-05-29 05:18:48.000000 arasea-3.0.7/arasea/compile/function/__init__.py
+-rw-r--r--   0 arkanepetra  (1000) arkanepetra  (1000)    22096 2024-05-29 05:18:48.000000 arasea-3.0.7/arasea/compile/function/pfunc.py
+-rw-r--r--   0 arkanepetra  (1000) arkanepetra  (1000)    73889 2024-05-29 05:18:48.000000 arasea-3.0.7/arasea/compile/function/types.py
+-rw-r--r--   0 arkanepetra  (1000) arkanepetra  (1000)     9102 2024-05-29 05:18:48.000000 arasea-3.0.7/arasea/compile/io.py
+-rw-r--r--   0 arkanepetra  (1000) arkanepetra  (1000)    17793 2024-05-29 05:18:48.000000 arasea-3.0.7/arasea/compile/mode.py
+-rw-r--r--   0 arkanepetra  (1000) arkanepetra  (1000)     3706 2024-05-29 05:18:48.000000 arasea-3.0.7/arasea/compile/monitormode.py
+-rw-r--r--   0 arkanepetra  (1000) arkanepetra  (1000)     8326 2024-05-29 05:18:48.000000 arasea-3.0.7/arasea/compile/nanguardmode.py
+-rw-r--r--   0 arkanepetra  (1000) arkanepetra  (1000)    11245 2024-05-29 05:18:48.000000 arasea-3.0.7/arasea/compile/ops.py
+-rw-r--r--   0 arkanepetra  (1000) arkanepetra  (1000)    59770 2024-05-29 05:18:48.000000 arasea-3.0.7/arasea/compile/profiling.py
+-rw-r--r--   0 arkanepetra  (1000) arkanepetra  (1000)     7179 2024-05-29 05:18:48.000000 arasea-3.0.7/arasea/compile/sharedvalue.py
+-rw-r--r--   0 arkanepetra  (1000) arkanepetra  (1000)    46225 2024-05-29 05:18:48.000000 arasea-3.0.7/arasea/configdefaults.py
+-rw-r--r--   0 arkanepetra  (1000) arkanepetra  (1000)    22462 2024-05-29 05:18:48.000000 arasea-3.0.7/arasea/configparser.py
+drwxrwxr-x   0 arkanepetra  (1000) arkanepetra  (1000)        0 2024-05-29 05:48:23.682429 arasea-3.0.7/arasea/d3viz/
+-rw-r--r--   0 arkanepetra  (1000) arkanepetra  (1000)       46 2024-05-29 05:18:48.000000 arasea-3.0.7/arasea/d3viz/__init__.py
+-rw-r--r--   0 arkanepetra  (1000) arkanepetra  (1000)     3830 2024-05-29 05:18:48.000000 arasea-3.0.7/arasea/d3viz/d3viz.py
+-rw-r--r--   0 arkanepetra  (1000) arkanepetra  (1000)    11843 2024-05-29 05:18:48.000000 arasea-3.0.7/arasea/d3viz/formatting.py
+-rw-r--r--   0 arkanepetra  (1000) arkanepetra  (1000)        0 2024-05-29 05:18:48.000000 arasea-3.0.7/arasea/debug.log
+-rw-r--r--   0 arkanepetra  (1000) arkanepetra  (1000)    86751 2024-05-29 05:18:48.000000 arasea-3.0.7/arasea/gradient.py
+drwxrwxr-x   0 arkanepetra  (1000) arkanepetra  (1000)        0 2024-05-29 05:48:23.687430 arasea-3.0.7/arasea/graph/
+-rw-r--r--   0 arkanepetra  (1000) arkanepetra  (1000)      505 2024-05-29 05:18:48.000000 arasea-3.0.7/arasea/graph/__init__.py
+-rw-r--r--   0 arkanepetra  (1000) arkanepetra  (1000)    59773 2024-05-29 05:18:48.000000 arasea-3.0.7/arasea/graph/basic.py
+-rw-r--r--   0 arkanepetra  (1000) arkanepetra  (1000)    33216 2024-05-29 05:18:48.000000 arasea-3.0.7/arasea/graph/destroyhandler.py
+-rw-r--r--   0 arkanepetra  (1000) arkanepetra  (1000)    24835 2024-05-29 05:18:48.000000 arasea-3.0.7/arasea/graph/features.py
+-rw-r--r--   0 arkanepetra  (1000) arkanepetra  (1000)    36232 2024-05-29 05:18:48.000000 arasea-3.0.7/arasea/graph/fg.py
+-rw-r--r--   0 arkanepetra  (1000) arkanepetra  (1000)      246 2024-05-29 05:18:48.000000 arasea-3.0.7/arasea/graph/kanren.py
+-rw-r--r--   0 arkanepetra  (1000) arkanepetra  (1000)     1150 2024-05-29 05:18:48.000000 arasea-3.0.7/arasea/graph/null_type.py
+-rw-r--r--   0 arkanepetra  (1000) arkanepetra  (1000)    25036 2024-05-29 05:18:48.000000 arasea-3.0.7/arasea/graph/op.py
+-rw-r--r--   0 arkanepetra  (1000) arkanepetra  (1000)      793 2024-05-29 05:18:48.000000 arasea-3.0.7/arasea/graph/opt.py
+-rw-r--r--   0 arkanepetra  (1000) arkanepetra  (1000)      799 2024-05-29 05:18:48.000000 arasea-3.0.7/arasea/graph/opt_utils.py
+-rw-r--r--   0 arkanepetra  (1000) arkanepetra  (1000)      786 2024-05-29 05:18:48.000000 arasea-3.0.7/arasea/graph/optdb.py
+drwxrwxr-x   0 arkanepetra  (1000) arkanepetra  (1000)        0 2024-05-29 05:48:23.688430 arasea-3.0.7/arasea/graph/rewriting/
+-rw-r--r--   0 arkanepetra  (1000) arkanepetra  (1000)        0 2024-05-29 05:18:48.000000 arasea-3.0.7/arasea/graph/rewriting/__init__.py
+-rw-r--r--   0 arkanepetra  (1000) arkanepetra  (1000)   114199 2024-05-29 05:18:48.000000 arasea-3.0.7/arasea/graph/rewriting/basic.py
+-rw-r--r--   0 arkanepetra  (1000) arkanepetra  (1000)    19934 2024-05-29 05:18:48.000000 arasea-3.0.7/arasea/graph/rewriting/db.py
+-rw-r--r--   0 arkanepetra  (1000) arkanepetra  (1000)     3035 2024-05-29 05:18:48.000000 arasea-3.0.7/arasea/graph/rewriting/kanren.py
+-rw-r--r--   0 arkanepetra  (1000) arkanepetra  (1000)     7239 2024-05-29 05:18:48.000000 arasea-3.0.7/arasea/graph/rewriting/unify.py
+-rw-r--r--   0 arkanepetra  (1000) arkanepetra  (1000)     9148 2024-05-29 05:18:48.000000 arasea-3.0.7/arasea/graph/rewriting/utils.py
+-rw-r--r--   0 arkanepetra  (1000) arkanepetra  (1000)     7865 2024-05-29 05:18:48.000000 arasea-3.0.7/arasea/graph/sched.py
+-rw-r--r--   0 arkanepetra  (1000) arkanepetra  (1000)      223 2024-05-29 05:18:48.000000 arasea-3.0.7/arasea/graph/toolbox.py
+-rw-r--r--   0 arkanepetra  (1000) arkanepetra  (1000)     9527 2024-05-29 05:18:48.000000 arasea-3.0.7/arasea/graph/type.py
+-rw-r--r--   0 arkanepetra  (1000) arkanepetra  (1000)      243 2024-05-29 05:18:48.000000 arasea-3.0.7/arasea/graph/unify.py
+-rw-r--r--   0 arkanepetra  (1000) arkanepetra  (1000)    12091 2024-05-29 05:18:48.000000 arasea-3.0.7/arasea/graph/utils.py
+-rw-r--r--   0 arkanepetra  (1000) arkanepetra  (1000)    29067 2024-05-29 05:18:48.000000 arasea-3.0.7/arasea/ifelse.py
+drwxrwxr-x   0 arkanepetra  (1000) arkanepetra  (1000)        0 2024-05-29 05:48:23.689430 arasea-3.0.7/arasea/link/
+-rw-r--r--   0 arkanepetra  (1000) arkanepetra  (1000)        3 2024-05-29 05:18:48.000000 arasea-3.0.7/arasea/link/__init__.py
+-rw-r--r--   0 arkanepetra  (1000) arkanepetra  (1000)    23890 2024-05-29 05:18:48.000000 arasea-3.0.7/arasea/link/basic.py
+drwxrwxr-x   0 arkanepetra  (1000) arkanepetra  (1000)        0 2024-05-29 05:48:23.693430 arasea-3.0.7/arasea/link/c/
+-rw-r--r--   0 arkanepetra  (1000) arkanepetra  (1000)        0 2024-05-29 05:18:48.000000 arasea-3.0.7/arasea/link/c/__init__.py
+-rw-r--r--   0 arkanepetra  (1000) arkanepetra  (1000)    72572 2024-05-29 05:18:48.000000 arasea-3.0.7/arasea/link/c/basic.py
+-rw-r--r--   0 arkanepetra  (1000) arkanepetra  (1000)   113013 2024-05-29 05:18:48.000000 arasea-3.0.7/arasea/link/c/cmodule.py
+-rw-r--r--   0 arkanepetra  (1000) arkanepetra  (1000)     4182 2024-05-29 05:18:48.000000 arasea-3.0.7/arasea/link/c/cutils.py
+-rw-r--r--   0 arkanepetra  (1000) arkanepetra  (1000)     1054 2024-05-29 05:18:48.000000 arasea-3.0.7/arasea/link/c/cvm.py
+-rw-r--r--   0 arkanepetra  (1000) arkanepetra  (1000)      402 2024-05-29 05:18:48.000000 arasea-3.0.7/arasea/link/c/exceptions.py
+-rw-r--r--   0 arkanepetra  (1000) arkanepetra  (1000)    19955 2024-05-29 05:18:48.000000 arasea-3.0.7/arasea/link/c/interface.py
+-rw-r--r--   0 arkanepetra  (1000) arkanepetra  (1000)     6641 2024-05-29 05:18:48.000000 arasea-3.0.7/arasea/link/c/lazylinker_c.py
+-rw-r--r--   0 arkanepetra  (1000) arkanepetra  (1000)    24724 2024-05-29 05:18:48.000000 arasea-3.0.7/arasea/link/c/op.py
+-rw-r--r--   0 arkanepetra  (1000) arkanepetra  (1000)    31544 2024-05-29 05:18:48.000000 arasea-3.0.7/arasea/link/c/params_type.py
+-rw-r--r--   0 arkanepetra  (1000) arkanepetra  (1000)    26540 2024-05-29 05:18:48.000000 arasea-3.0.7/arasea/link/c/type.py
+drwxrwxr-x   0 arkanepetra  (1000) arkanepetra  (1000)        0 2024-05-29 05:48:23.694430 arasea-3.0.7/arasea/link/jax/
+-rw-r--r--   0 arkanepetra  (1000) arkanepetra  (1000)       48 2024-05-29 05:18:48.000000 arasea-3.0.7/arasea/link/jax/__init__.py
+drwxrwxr-x   0 arkanepetra  (1000) arkanepetra  (1000)        0 2024-05-29 05:48:23.697430 arasea-3.0.7/arasea/link/jax/dispatch/
+-rw-r--r--   0 arkanepetra  (1000) arkanepetra  (1000)      529 2024-05-29 05:18:48.000000 arasea-3.0.7/arasea/link/jax/dispatch/__init__.py
+-rw-r--r--   0 arkanepetra  (1000) arkanepetra  (1000)     2370 2024-05-29 05:18:48.000000 arasea-3.0.7/arasea/link/jax/dispatch/basic.py
+-rw-r--r--   0 arkanepetra  (1000) arkanepetra  (1000)     2944 2024-05-29 05:18:48.000000 arasea-3.0.7/arasea/link/jax/dispatch/elemwise.py
+-rw-r--r--   0 arkanepetra  (1000) arkanepetra  (1000)     3380 2024-05-29 05:18:48.000000 arasea-3.0.7/arasea/link/jax/dispatch/extra_ops.py
+-rw-r--r--   0 arkanepetra  (1000) arkanepetra  (1000)     3072 2024-05-29 05:18:48.000000 arasea-3.0.7/arasea/link/jax/dispatch/nlinalg.py
+-rw-r--r--   0 arkanepetra  (1000) arkanepetra  (1000)    14480 2024-05-29 05:18:48.000000 arasea-3.0.7/arasea/link/jax/dispatch/random.py
+-rw-r--r--   0 arkanepetra  (1000) arkanepetra  (1000)     5622 2024-05-29 05:18:48.000000 arasea-3.0.7/arasea/link/jax/dispatch/scalar.py
+-rw-r--r--   0 arkanepetra  (1000) arkanepetra  (1000)     5382 2024-05-29 05:18:48.000000 arasea-3.0.7/arasea/link/jax/dispatch/scan.py
+-rw-r--r--   0 arkanepetra  (1000) arkanepetra  (1000)     2745 2024-05-29 05:18:48.000000 arasea-3.0.7/arasea/link/jax/dispatch/shape.py
+-rw-r--r--   0 arkanepetra  (1000) arkanepetra  (1000)     1115 2024-05-29 05:18:48.000000 arasea-3.0.7/arasea/link/jax/dispatch/slinalg.py
+-rw-r--r--   0 arkanepetra  (1000) arkanepetra  (1000)     3188 2024-05-29 05:18:48.000000 arasea-3.0.7/arasea/link/jax/dispatch/subtensor.py
+-rw-r--r--   0 arkanepetra  (1000) arkanepetra  (1000)     3380 2024-05-29 05:18:48.000000 arasea-3.0.7/arasea/link/jax/dispatch/tensor_basic.py
+-rw-r--r--   0 arkanepetra  (1000) arkanepetra  (1000)      238 2024-05-29 05:18:48.000000 arasea-3.0.7/arasea/link/jax/jax_dispatch.py
+-rw-r--r--   0 arkanepetra  (1000) arkanepetra  (1000)      232 2024-05-29 05:18:48.000000 arasea-3.0.7/arasea/link/jax/jax_linker.py
+-rw-r--r--   0 arkanepetra  (1000) arkanepetra  (1000)     2991 2024-05-29 05:18:48.000000 arasea-3.0.7/arasea/link/jax/linker.py
+drwxrwxr-x   0 arkanepetra  (1000) arkanepetra  (1000)        0 2024-05-29 05:48:23.698430 arasea-3.0.7/arasea/link/numba/
+-rw-r--r--   0 arkanepetra  (1000) arkanepetra  (1000)       49 2024-05-29 05:18:48.000000 arasea-3.0.7/arasea/link/numba/__init__.py
+drwxrwxr-x   0 arkanepetra  (1000) arkanepetra  (1000)        0 2024-05-29 05:48:23.701431 arasea-3.0.7/arasea/link/numba/dispatch/
+-rw-r--r--   0 arkanepetra  (1000) arkanepetra  (1000)      506 2024-05-29 05:18:48.000000 arasea-3.0.7/arasea/link/numba/dispatch/__init__.py
+-rw-r--r--   0 arkanepetra  (1000) arkanepetra  (1000)    25903 2024-05-29 05:18:48.000000 arasea-3.0.7/arasea/link/numba/dispatch/basic.py
+-rw-r--r--   0 arkanepetra  (1000) arkanepetra  (1000)    22260 2024-05-29 05:18:48.000000 arasea-3.0.7/arasea/link/numba/dispatch/elemwise.py
+-rw-r--r--   0 arkanepetra  (1000) arkanepetra  (1000)     9262 2024-05-29 05:18:48.000000 arasea-3.0.7/arasea/link/numba/dispatch/extra_ops.py
+-rw-r--r--   0 arkanepetra  (1000) arkanepetra  (1000)     5076 2024-05-29 05:18:48.000000 arasea-3.0.7/arasea/link/numba/dispatch/nlinalg.py
+-rw-r--r--   0 arkanepetra  (1000) arkanepetra  (1000)    12812 2024-05-29 05:18:48.000000 arasea-3.0.7/arasea/link/numba/dispatch/random.py
+-rw-r--r--   0 arkanepetra  (1000) arkanepetra  (1000)     8893 2024-05-29 05:18:48.000000 arasea-3.0.7/arasea/link/numba/dispatch/scalar.py
+-rw-r--r--   0 arkanepetra  (1000) arkanepetra  (1000)    14203 2024-05-29 05:18:48.000000 arasea-3.0.7/arasea/link/numba/dispatch/scan.py
+-rw-r--r--   0 arkanepetra  (1000) arkanepetra  (1000)     6109 2024-05-29 05:18:48.000000 arasea-3.0.7/arasea/link/numba/dispatch/sparse.py
+-rw-r--r--   0 arkanepetra  (1000) arkanepetra  (1000)     6403 2024-05-29 05:18:48.000000 arasea-3.0.7/arasea/link/numba/dispatch/tensor_basic.py
+-rw-r--r--   0 arkanepetra  (1000) arkanepetra  (1000)     1044 2024-05-29 05:18:48.000000 arasea-3.0.7/arasea/link/numba/linker.py
+-rw-r--r--   0 arkanepetra  (1000) arkanepetra  (1000)    28716 2024-05-29 05:18:48.000000 arasea-3.0.7/arasea/link/utils.py
+-rw-r--r--   0 arkanepetra  (1000) arkanepetra  (1000)    50565 2024-05-29 05:18:48.000000 arasea-3.0.7/arasea/link/vm.py
+drwxrwxr-x   0 arkanepetra  (1000) arkanepetra  (1000)        0 2024-05-29 05:48:23.703431 arasea-3.0.7/arasea/misc/
+-rw-r--r--   0 arkanepetra  (1000) arkanepetra  (1000)        0 2024-05-29 05:18:48.000000 arasea-3.0.7/arasea/misc/__init__.py
+-rw-r--r--   0 arkanepetra  (1000) arkanepetra  (1000)    10017 2024-05-29 05:18:48.000000 arasea-3.0.7/arasea/misc/check_blas.py
+-rw-r--r--   0 arkanepetra  (1000) arkanepetra  (1000)     2409 2024-05-29 05:18:48.000000 arasea-3.0.7/arasea/misc/check_duplicate_key.py
+-rw-r--r--   0 arkanepetra  (1000) arkanepetra  (1000)     2166 2024-05-29 05:18:48.000000 arasea-3.0.7/arasea/misc/elemwise_openmp_speedup.py
+-rw-r--r--   0 arkanepetra  (1000) arkanepetra  (1000)     1887 2024-05-29 05:18:48.000000 arasea-3.0.7/arasea/misc/elemwise_time_test.py
+-rw-r--r--   0 arkanepetra  (1000) arkanepetra  (1000)     1347 2024-05-29 05:18:48.000000 arasea-3.0.7/arasea/misc/frozendict.py
+-rw-r--r--   0 arkanepetra  (1000) arkanepetra  (1000)      607 2024-05-29 05:18:48.000000 arasea-3.0.7/arasea/misc/latence_gpu_transfert.py
+-rw-r--r--   0 arkanepetra  (1000) arkanepetra  (1000)      921 2024-05-29 05:18:48.000000 arasea-3.0.7/arasea/misc/may_share_memory.py
+-rw-r--r--   0 arkanepetra  (1000) arkanepetra  (1000)     7191 2024-05-29 05:18:48.000000 arasea-3.0.7/arasea/misc/ordered_set.py
+-rw-r--r--   0 arkanepetra  (1000) arkanepetra  (1000)    10166 2024-05-29 05:18:48.000000 arasea-3.0.7/arasea/misc/pkl_utils.py
+-rw-r--r--   0 arkanepetra  (1000) arkanepetra  (1000)     2293 2024-05-29 05:18:48.000000 arasea-3.0.7/arasea/misc/safe_asarray.py
+-rw-r--r--   0 arkanepetra  (1000) arkanepetra  (1000)    67046 2024-05-29 05:18:48.000000 arasea-3.0.7/arasea/printing.py
+-rw-r--r--   0 arkanepetra  (1000) arkanepetra  (1000)        0 2024-05-29 05:18:48.000000 arasea-3.0.7/arasea/py.typed
+-rw-r--r--   0 arkanepetra  (1000) arkanepetra  (1000)     5837 2024-05-29 05:18:48.000000 arasea-3.0.7/arasea/raise_op.py
+drwxrwxr-x   0 arkanepetra  (1000) arkanepetra  (1000)        0 2024-05-29 05:48:23.705431 arasea-3.0.7/arasea/sandbox/
+-rw-r--r--   0 arkanepetra  (1000) arkanepetra  (1000)        0 2024-05-29 05:18:48.000000 arasea-3.0.7/arasea/sandbox/__init__.py
+-rw-r--r--   0 arkanepetra  (1000) arkanepetra  (1000)     3873 2024-05-29 05:18:48.000000 arasea-3.0.7/arasea/sandbox/fourier.py
+drwxrwxr-x   0 arkanepetra  (1000) arkanepetra  (1000)        0 2024-05-29 05:48:23.705431 arasea-3.0.7/arasea/sandbox/linalg/
+-rw-r--r--   0 arkanepetra  (1000) arkanepetra  (1000)       60 2024-05-29 05:18:48.000000 arasea-3.0.7/arasea/sandbox/linalg/__init__.py
+-rw-r--r--   0 arkanepetra  (1000) arkanepetra  (1000)     6060 2024-05-29 05:18:48.000000 arasea-3.0.7/arasea/sandbox/linalg/ops.py
+-rw-r--r--   0 arkanepetra  (1000) arkanepetra  (1000)     1455 2024-05-29 05:18:48.000000 arasea-3.0.7/arasea/sandbox/minimal.py
+-rw-r--r--   0 arkanepetra  (1000) arkanepetra  (1000)    14812 2024-05-29 05:18:48.000000 arasea-3.0.7/arasea/sandbox/multinomial.py
+-rw-r--r--   0 arkanepetra  (1000) arkanepetra  (1000)    48271 2024-05-29 05:18:48.000000 arasea-3.0.7/arasea/sandbox/rng_mrg.py
+-rw-r--r--   0 arkanepetra  (1000) arkanepetra  (1000)      217 2024-05-29 05:18:48.000000 arasea-3.0.7/arasea/sandbox/solve.py
+drwxrwxr-x   0 arkanepetra  (1000) arkanepetra  (1000)        0 2024-05-29 05:48:23.707431 arasea-3.0.7/arasea/scalar/
+-rw-r--r--   0 arkanepetra  (1000) arkanepetra  (1000)      709 2024-05-29 05:18:48.000000 arasea-3.0.7/arasea/scalar/__init__.py
+-rw-r--r--   0 arkanepetra  (1000) arkanepetra  (1000)   143429 2024-05-29 05:18:48.000000 arasea-3.0.7/arasea/scalar/basic.py
+-rw-r--r--   0 arkanepetra  (1000) arkanepetra  (1000)      223 2024-05-29 05:18:48.000000 arasea-3.0.7/arasea/scalar/basic_scipy.py
+-rw-r--r--   0 arkanepetra  (1000) arkanepetra  (1000)     3275 2024-05-29 05:18:48.000000 arasea-3.0.7/arasea/scalar/basic_sympy.py
+-rw-r--r--   0 arkanepetra  (1000) arkanepetra  (1000)    46142 2024-05-29 05:18:48.000000 arasea-3.0.7/arasea/scalar/math.py
+-rw-r--r--   0 arkanepetra  (1000) arkanepetra  (1000)     1851 2024-05-29 05:18:48.000000 arasea-3.0.7/arasea/scalar/sharedvar.py
+drwxrwxr-x   0 arkanepetra  (1000) arkanepetra  (1000)        0 2024-05-29 05:48:23.710431 arasea-3.0.7/arasea/scan/
+-rw-r--r--   0 arkanepetra  (1000) arkanepetra  (1000)     1931 2024-05-29 05:18:48.000000 arasea-3.0.7/arasea/scan/__init__.py
+-rw-r--r--   0 arkanepetra  (1000) arkanepetra  (1000)    50095 2024-05-29 05:18:48.000000 arasea-3.0.7/arasea/scan/basic.py
+-rw-r--r--   0 arkanepetra  (1000) arkanepetra  (1000)     6743 2024-05-29 05:18:48.000000 arasea-3.0.7/arasea/scan/checkpoints.py
+-rw-r--r--   0 arkanepetra  (1000) arkanepetra  (1000)   140522 2024-05-29 05:18:48.000000 arasea-3.0.7/arasea/scan/op.py
+-rw-r--r--   0 arkanepetra  (1000) arkanepetra  (1000)      226 2024-05-29 05:18:48.000000 arasea-3.0.7/arasea/scan/opt.py
+-rw-r--r--   0 arkanepetra  (1000) arkanepetra  (1000)    95587 2024-05-29 05:18:48.000000 arasea-3.0.7/arasea/scan/rewriting.py
+-rw-r--r--   0 arkanepetra  (1000) arkanepetra  (1000)     3511 2024-05-29 05:18:48.000000 arasea-3.0.7/arasea/scan/scan_perform_ext.py
+-rw-r--r--   0 arkanepetra  (1000) arkanepetra  (1000)    38052 2024-05-29 05:18:48.000000 arasea-3.0.7/arasea/scan/utils.py
+-rw-r--r--   0 arkanepetra  (1000) arkanepetra  (1000)     4599 2024-05-29 05:18:48.000000 arasea-3.0.7/arasea/scan/views.py
+drwxrwxr-x   0 arkanepetra  (1000) arkanepetra  (1000)        0 2024-05-29 05:48:23.712431 arasea-3.0.7/arasea/sparse/
+-rw-r--r--   0 arkanepetra  (1000) arkanepetra  (1000)     1097 2024-05-29 05:18:48.000000 arasea-3.0.7/arasea/sparse/__init__.py
+-rw-r--r--   0 arkanepetra  (1000) arkanepetra  (1000)   118008 2024-05-29 05:18:48.000000 arasea-3.0.7/arasea/sparse/basic.py
+-rw-r--r--   0 arkanepetra  (1000) arkanepetra  (1000)      232 2024-05-29 05:18:48.000000 arasea-3.0.7/arasea/sparse/opt.py
+-rw-r--r--   0 arkanepetra  (1000) arkanepetra  (1000)    76905 2024-05-29 05:18:48.000000 arasea-3.0.7/arasea/sparse/rewriting.py
+drwxrwxr-x   0 arkanepetra  (1000) arkanepetra  (1000)        0 2024-05-29 05:48:23.713431 arasea-3.0.7/arasea/sparse/sandbox/
+-rw-r--r--   0 arkanepetra  (1000) arkanepetra  (1000)        0 2024-05-29 05:18:48.000000 arasea-3.0.7/arasea/sparse/sandbox/__init__.py
+-rw-r--r--   0 arkanepetra  (1000) arkanepetra  (1000)    17303 2024-05-29 05:18:48.000000 arasea-3.0.7/arasea/sparse/sandbox/sp.py
+-rw-r--r--   0 arkanepetra  (1000) arkanepetra  (1000)     7194 2024-05-29 05:18:48.000000 arasea-3.0.7/arasea/sparse/sandbox/sp2.py
+-rw-r--r--   0 arkanepetra  (1000) arkanepetra  (1000)      827 2024-05-29 05:18:48.000000 arasea-3.0.7/arasea/sparse/sharedvar.py
+-rw-r--r--   0 arkanepetra  (1000) arkanepetra  (1000)     8044 2024-05-29 05:18:48.000000 arasea-3.0.7/arasea/sparse/type.py
+-rw-r--r--   0 arkanepetra  (1000) arkanepetra  (1000)      767 2024-05-29 05:18:48.000000 arasea-3.0.7/arasea/sparse/utils.py
+drwxrwxr-x   0 arkanepetra  (1000) arkanepetra  (1000)        0 2024-05-29 05:48:23.723432 arasea-3.0.7/arasea/tensor/
+-rw-r--r--   0 arkanepetra  (1000) arkanepetra  (1000)     4883 2024-05-29 05:18:48.000000 arasea-3.0.7/arasea/tensor/__init__.py
+-rw-r--r--   0 arkanepetra  (1000) arkanepetra  (1000)   135651 2024-05-29 05:18:48.000000 arasea-3.0.7/arasea/tensor/basic.py
+-rw-r--r--   0 arkanepetra  (1000) arkanepetra  (1000)      461 2024-05-29 05:18:48.000000 arasea-3.0.7/arasea/tensor/basic_opt.py
+-rw-r--r--   0 arkanepetra  (1000) arkanepetra  (1000)    98819 2024-05-29 05:18:48.000000 arasea-3.0.7/arasea/tensor/blas.py
+-rw-r--r--   0 arkanepetra  (1000) arkanepetra  (1000)    26486 2024-05-29 05:18:48.000000 arasea-3.0.7/arasea/tensor/blas_c.py
+-rw-r--r--   0 arkanepetra  (1000) arkanepetra  (1000)    68050 2024-05-29 05:18:48.000000 arasea-3.0.7/arasea/tensor/blas_headers.py
+-rw-r--r--   0 arkanepetra  (1000) arkanepetra  (1000)     2783 2024-05-29 05:18:48.000000 arasea-3.0.7/arasea/tensor/blas_scipy.py
+-rw-r--r--   0 arkanepetra  (1000) arkanepetra  (1000)    66675 2024-05-29 05:18:48.000000 arasea-3.0.7/arasea/tensor/elemwise.py
+-rw-r--r--   0 arkanepetra  (1000) arkanepetra  (1000)    20860 2024-05-29 05:18:48.000000 arasea-3.0.7/arasea/tensor/elemwise_cgen.py
+-rw-r--r--   0 arkanepetra  (1000) arkanepetra  (1000)      362 2024-05-29 05:18:48.000000 arasea-3.0.7/arasea/tensor/exceptions.py
+-rw-r--r--   0 arkanepetra  (1000) arkanepetra  (1000)    57997 2024-05-29 05:18:48.000000 arasea-3.0.7/arasea/tensor/extra_ops.py
+-rw-r--r--   0 arkanepetra  (1000) arkanepetra  (1000)     7589 2024-05-29 05:18:48.000000 arasea-3.0.7/arasea/tensor/fft.py
+-rw-r--r--   0 arkanepetra  (1000) arkanepetra  (1000)     6565 2024-05-29 05:18:48.000000 arasea-3.0.7/arasea/tensor/fourier.py
+-rw-r--r--   0 arkanepetra  (1000) arkanepetra  (1000)     7848 2024-05-29 05:18:48.000000 arasea-3.0.7/arasea/tensor/inplace.py
+-rw-r--r--   0 arkanepetra  (1000) arkanepetra  (1000)     7239 2024-05-29 05:18:48.000000 arasea-3.0.7/arasea/tensor/io.py
+-rw-r--r--   0 arkanepetra  (1000) arkanepetra  (1000)       72 2024-05-29 05:18:48.000000 arasea-3.0.7/arasea/tensor/linalg.py
+-rw-r--r--   0 arkanepetra  (1000) arkanepetra  (1000)    96168 2024-05-29 05:18:48.000000 arasea-3.0.7/arasea/tensor/math.py
+-rw-r--r--   0 arkanepetra  (1000) arkanepetra  (1000)      247 2024-05-29 05:18:48.000000 arasea-3.0.7/arasea/tensor/math_opt.py
+-rw-r--r--   0 arkanepetra  (1000) arkanepetra  (1000)    22498 2024-05-29 05:18:48.000000 arasea-3.0.7/arasea/tensor/nlinalg.py
+drwxrwxr-x   0 arkanepetra  (1000) arkanepetra  (1000)        0 2024-05-29 05:48:23.728433 arasea-3.0.7/arasea/tensor/nnet/
+-rw-r--r--   0 arkanepetra  (1000) arkanepetra  (1000)     1431 2024-05-29 05:18:48.000000 arasea-3.0.7/arasea/tensor/nnet/__init__.py
+-rw-r--r--   0 arkanepetra  (1000) arkanepetra  (1000)   138965 2024-05-29 05:18:48.000000 arasea-3.0.7/arasea/tensor/nnet/abstract_conv.py
+-rw-r--r--   0 arkanepetra  (1000) arkanepetra  (1000)    75765 2024-05-29 05:18:48.000000 arasea-3.0.7/arasea/tensor/nnet/basic.py
+-rw-r--r--   0 arkanepetra  (1000) arkanepetra  (1000)    35376 2024-05-29 05:18:48.000000 arasea-3.0.7/arasea/tensor/nnet/batchnorm.py
+-rw-r--r--   0 arkanepetra  (1000) arkanepetra  (1000)     8902 2024-05-29 05:18:48.000000 arasea-3.0.7/arasea/tensor/nnet/blocksparse.py
+-rw-r--r--   0 arkanepetra  (1000) arkanepetra  (1000)    94523 2024-05-29 05:18:48.000000 arasea-3.0.7/arasea/tensor/nnet/conv.py
+-rw-r--r--   0 arkanepetra  (1000) arkanepetra  (1000)     9910 2024-05-29 05:18:48.000000 arasea-3.0.7/arasea/tensor/nnet/conv3d2d.py
+-rw-r--r--   0 arkanepetra  (1000) arkanepetra  (1000)    40356 2024-05-29 05:18:48.000000 arasea-3.0.7/arasea/tensor/nnet/corr.py
+-rw-r--r--   0 arkanepetra  (1000) arkanepetra  (1000)    36145 2024-05-29 05:18:48.000000 arasea-3.0.7/arasea/tensor/nnet/corr3d.py
+-rw-r--r--   0 arkanepetra  (1000) arkanepetra  (1000)     8522 2024-05-29 05:18:48.000000 arasea-3.0.7/arasea/tensor/nnet/ctc.py
+-rw-r--r--   0 arkanepetra  (1000) arkanepetra  (1000)    35353 2024-05-29 05:18:48.000000 arasea-3.0.7/arasea/tensor/nnet/neighbours.py
+-rw-r--r--   0 arkanepetra  (1000) arkanepetra  (1000)      247 2024-05-29 05:18:48.000000 arasea-3.0.7/arasea/tensor/nnet/opt.py
+-rw-r--r--   0 arkanepetra  (1000) arkanepetra  (1000)    17297 2024-05-29 05:18:48.000000 arasea-3.0.7/arasea/tensor/nnet/rewriting.py
+-rw-r--r--   0 arkanepetra  (1000) arkanepetra  (1000)     5212 2024-05-29 05:18:48.000000 arasea-3.0.7/arasea/tensor/nnet/sigm.py
+-rw-r--r--   0 arkanepetra  (1000) arkanepetra  (1000)      277 2024-05-29 05:18:48.000000 arasea-3.0.7/arasea/tensor/opt_uncanonicalize.py
+drwxrwxr-x   0 arkanepetra  (1000) arkanepetra  (1000)        0 2024-05-29 05:48:23.730433 arasea-3.0.7/arasea/tensor/random/
+-rw-r--r--   0 arkanepetra  (1000) arkanepetra  (1000)      265 2024-05-29 05:18:48.000000 arasea-3.0.7/arasea/tensor/random/__init__.py
+-rw-r--r--   0 arkanepetra  (1000) arkanepetra  (1000)    65558 2024-05-29 05:18:48.000000 arasea-3.0.7/arasea/tensor/random/basic.py
+-rw-r--r--   0 arkanepetra  (1000) arkanepetra  (1000)    14324 2024-05-29 05:18:48.000000 arasea-3.0.7/arasea/tensor/random/op.py
+-rw-r--r--   0 arkanepetra  (1000) arkanepetra  (1000)      253 2024-05-29 05:18:48.000000 arasea-3.0.7/arasea/tensor/random/opt.py
+drwxrwxr-x   0 arkanepetra  (1000) arkanepetra  (1000)        0 2024-05-29 05:48:23.731433 arasea-3.0.7/arasea/tensor/random/rewriting/
+-rw-r--r--   0 arkanepetra  (1000) arkanepetra  (1000)      221 2024-05-29 05:18:48.000000 arasea-3.0.7/arasea/tensor/random/rewriting/__init__.py
+-rw-r--r--   0 arkanepetra  (1000) arkanepetra  (1000)    15290 2024-05-29 05:18:48.000000 arasea-3.0.7/arasea/tensor/random/rewriting/basic.py
+-rw-r--r--   0 arkanepetra  (1000) arkanepetra  (1000)     1887 2024-05-29 05:18:48.000000 arasea-3.0.7/arasea/tensor/random/rewriting/jax.py
+-rw-r--r--   0 arkanepetra  (1000) arkanepetra  (1000)     6730 2024-05-29 05:18:48.000000 arasea-3.0.7/arasea/tensor/random/type.py
+-rw-r--r--   0 arkanepetra  (1000) arkanepetra  (1000)     9024 2024-05-29 05:18:48.000000 arasea-3.0.7/arasea/tensor/random/utils.py
+-rw-r--r--   0 arkanepetra  (1000) arkanepetra  (1000)     1534 2024-05-29 05:18:48.000000 arasea-3.0.7/arasea/tensor/random/var.py
+drwxrwxr-x   0 arkanepetra  (1000) arkanepetra  (1000)        0 2024-05-29 05:48:23.734433 arasea-3.0.7/arasea/tensor/rewriting/
+-rw-r--r--   0 arkanepetra  (1000) arkanepetra  (1000)      384 2024-05-29 05:18:48.000000 arasea-3.0.7/arasea/tensor/rewriting/__init__.py
+-rw-r--r--   0 arkanepetra  (1000) arkanepetra  (1000)    42723 2024-05-29 05:18:48.000000 arasea-3.0.7/arasea/tensor/rewriting/basic.py
+-rw-r--r--   0 arkanepetra  (1000) arkanepetra  (1000)    39439 2024-05-29 05:18:48.000000 arasea-3.0.7/arasea/tensor/rewriting/elemwise.py
+-rw-r--r--   0 arkanepetra  (1000) arkanepetra  (1000)     4845 2024-05-29 05:18:48.000000 arasea-3.0.7/arasea/tensor/rewriting/extra_ops.py
+-rw-r--r--   0 arkanepetra  (1000) arkanepetra  (1000)     3954 2024-05-29 05:18:48.000000 arasea-3.0.7/arasea/tensor/rewriting/jax.py
+-rw-r--r--   0 arkanepetra  (1000) arkanepetra  (1000)   124250 2024-05-29 05:18:48.000000 arasea-3.0.7/arasea/tensor/rewriting/math.py
+-rw-r--r--   0 arkanepetra  (1000) arkanepetra  (1000)    43264 2024-05-29 05:18:48.000000 arasea-3.0.7/arasea/tensor/rewriting/shape.py
+-rw-r--r--   0 arkanepetra  (1000) arkanepetra  (1000)     6111 2024-05-29 05:18:48.000000 arasea-3.0.7/arasea/tensor/rewriting/special.py
+-rw-r--r--   0 arkanepetra  (1000) arkanepetra  (1000)    63199 2024-05-29 05:18:48.000000 arasea-3.0.7/arasea/tensor/rewriting/subtensor.py
+-rw-r--r--   0 arkanepetra  (1000) arkanepetra  (1000)     9500 2024-05-29 05:18:48.000000 arasea-3.0.7/arasea/tensor/rewriting/uncanonicalize.py
+-rw-r--r--   0 arkanepetra  (1000) arkanepetra  (1000)    33298 2024-05-29 05:18:48.000000 arasea-3.0.7/arasea/tensor/shape.py
+-rw-r--r--   0 arkanepetra  (1000) arkanepetra  (1000)     3858 2024-05-29 05:18:48.000000 arasea-3.0.7/arasea/tensor/sharedvar.py
+drwxrwxr-x   0 arkanepetra  (1000) arkanepetra  (1000)        0 2024-05-29 05:48:23.734433 arasea-3.0.7/arasea/tensor/signal/
+-rw-r--r--   0 arkanepetra  (1000) arkanepetra  (1000)        0 2024-05-29 05:18:48.000000 arasea-3.0.7/arasea/tensor/signal/__init__.py
+-rw-r--r--   0 arkanepetra  (1000) arkanepetra  (1000)     3509 2024-05-29 05:18:48.000000 arasea-3.0.7/arasea/tensor/signal/conv.py
+-rwxr-xr-x   0 arkanepetra  (1000) arkanepetra  (1000)    97524 2024-05-29 05:18:48.000000 arasea-3.0.7/arasea/tensor/signal/pool.py
+-rw-r--r--   0 arkanepetra  (1000) arkanepetra  (1000)    24997 2024-05-29 05:18:48.000000 arasea-3.0.7/arasea/tensor/slinalg.py
+-rw-r--r--   0 arkanepetra  (1000) arkanepetra  (1000)    17849 2024-05-29 05:18:48.000000 arasea-3.0.7/arasea/tensor/sort.py
+-rw-r--r--   0 arkanepetra  (1000) arkanepetra  (1000)    27385 2024-05-29 05:18:48.000000 arasea-3.0.7/arasea/tensor/special.py
+-rw-r--r--   0 arkanepetra  (1000) arkanepetra  (1000)    91231 2024-05-29 05:18:48.000000 arasea-3.0.7/arasea/tensor/subtensor.py
+-rw-r--r--   0 arkanepetra  (1000) arkanepetra  (1000)      262 2024-05-29 05:18:48.000000 arasea-3.0.7/arasea/tensor/subtensor_opt.py
+-rw-r--r--   0 arkanepetra  (1000) arkanepetra  (1000)    41188 2024-05-29 05:18:48.000000 arasea-3.0.7/arasea/tensor/type.py
+-rw-r--r--   0 arkanepetra  (1000) arkanepetra  (1000)     4088 2024-05-29 05:18:48.000000 arasea-3.0.7/arasea/tensor/type_other.py
+-rw-r--r--   0 arkanepetra  (1000) arkanepetra  (1000)     3211 2024-05-29 05:18:48.000000 arasea-3.0.7/arasea/tensor/utils.py
+-rw-r--r--   0 arkanepetra  (1000) arkanepetra  (1000)    37592 2024-05-29 05:18:48.000000 arasea-3.0.7/arasea/tensor/var.py
+-rw-r--r--   0 arkanepetra  (1000) arkanepetra  (1000)     1831 2024-05-29 05:18:48.000000 arasea-3.0.7/arasea/tensor/xlogx.py
+drwxrwxr-x   0 arkanepetra  (1000) arkanepetra  (1000)        0 2024-05-29 05:48:23.736433 arasea-3.0.7/arasea/typed_list/
+-rw-r--r--   0 arkanepetra  (1000) arkanepetra  (1000)      127 2024-05-29 05:18:48.000000 arasea-3.0.7/arasea/typed_list/__init__.py
+-rw-r--r--   0 arkanepetra  (1000) arkanepetra  (1000)    18222 2024-05-29 05:18:48.000000 arasea-3.0.7/arasea/typed_list/basic.py
+-rw-r--r--   0 arkanepetra  (1000) arkanepetra  (1000)      779 2024-05-29 05:18:48.000000 arasea-3.0.7/arasea/typed_list/rewriting.py
+-rw-r--r--   0 arkanepetra  (1000) arkanepetra  (1000)     3933 2024-05-29 05:18:48.000000 arasea-3.0.7/arasea/typed_list/type.py
+-rw-r--r--   0 arkanepetra  (1000) arkanepetra  (1000)     2924 2024-05-29 05:18:48.000000 arasea-3.0.7/arasea/updates.py
+-rw-r--r--   0 arkanepetra  (1000) arkanepetra  (1000)    13640 2024-05-29 05:18:48.000000 arasea-3.0.7/arasea/utils.py
+-rw-r--r--   0 arkanepetra  (1000) arkanepetra  (1000)      962 2024-05-29 05:30:07.000000 arasea-3.0.7/arasea/version.py
+drwxrwxr-x   0 arkanepetra  (1000) arkanepetra  (1000)        0 2024-05-29 05:48:23.787437 arasea-3.0.7/arasea.egg-info/
+-rw-r--r--   0 arkanepetra  (1000) arkanepetra  (1000)     1660 2024-05-29 05:48:23.000000 arasea-3.0.7/arasea.egg-info/PKG-INFO
+-rw-rw-r--   0 arkanepetra  (1000) arkanepetra  (1000)    11380 2024-05-29 05:48:23.000000 arasea-3.0.7/arasea.egg-info/SOURCES.txt
+-rw-rw-r--   0 arkanepetra  (1000) arkanepetra  (1000)        1 2024-05-29 05:48:23.000000 arasea-3.0.7/arasea.egg-info/dependency_links.txt
+-rw-rw-r--   0 arkanepetra  (1000) arkanepetra  (1000)       86 2024-05-29 05:48:23.000000 arasea-3.0.7/arasea.egg-info/requires.txt
+-rw-rw-r--   0 arkanepetra  (1000) arkanepetra  (1000)       17 2024-05-29 05:48:23.000000 arasea-3.0.7/arasea.egg-info/top_level.txt
+drwxrwxr-x   0 arkanepetra  (1000) arkanepetra  (1000)        0 2024-05-29 05:48:23.736433 arasea-3.0.7/bin/
+-rw-r--r--   0 arkanepetra  (1000) arkanepetra  (1000)      239 2024-05-29 05:18:48.000000 arasea-3.0.7/bin/__init__.py
+-rw-r--r--   0 arkanepetra  (1000) arkanepetra  (1000)      332 2024-05-29 05:18:48.000000 arasea-3.0.7/bin/arasea_cache.py
+-rw-rw-r--   0 arkanepetra  (1000) arkanepetra  (1000)       38 2024-05-29 05:48:23.788437 arasea-3.0.7/setup.cfg
+-rw-r--r--   0 arkanepetra  (1000) arkanepetra  (1000)     3529 2024-05-29 05:29:48.000000 arasea-3.0.7/setup.py
+drwxrwxr-x   0 arkanepetra  (1000) arkanepetra  (1000)        0 2024-05-29 05:48:23.739433 arasea-3.0.7/tests/
+-rw-r--r--   0 arkanepetra  (1000) arkanepetra  (1000)        0 2024-05-29 05:18:49.000000 arasea-3.0.7/tests/__init__.py
+drwxrwxr-x   0 arkanepetra  (1000) arkanepetra  (1000)        0 2024-05-29 05:48:23.742433 arasea-3.0.7/tests/compile/
+-rw-r--r--   0 arkanepetra  (1000) arkanepetra  (1000)        0 2024-05-29 05:18:49.000000 arasea-3.0.7/tests/compile/__init__.py
+drwxrwxr-x   0 arkanepetra  (1000) arkanepetra  (1000)        0 2024-05-29 05:48:23.743434 arasea-3.0.7/tests/compile/function/
+-rw-r--r--   0 arkanepetra  (1000) arkanepetra  (1000)        0 2024-05-29 05:18:49.000000 arasea-3.0.7/tests/compile/function/__init__.py
+-rw-r--r--   0 arkanepetra  (1000) arkanepetra  (1000)     7284 2024-05-29 05:18:49.000000 arasea-3.0.7/tests/compile/function/test_function.py
+-rw-r--r--   0 arkanepetra  (1000) arkanepetra  (1000)    36404 2024-05-29 05:18:49.000000 arasea-3.0.7/tests/compile/function/test_pfunc.py
+-rw-r--r--   0 arkanepetra  (1000) arkanepetra  (1000)    42215 2024-05-29 05:18:49.000000 arasea-3.0.7/tests/compile/function/test_types.py
+-rw-r--r--   0 arkanepetra  (1000) arkanepetra  (1000)    24285 2024-05-29 05:18:49.000000 arasea-3.0.7/tests/compile/test_builders.py
+-rw-r--r--   0 arkanepetra  (1000) arkanepetra  (1000)     3917 2024-05-29 05:18:49.000000 arasea-3.0.7/tests/compile/test_compilelock.py
+-rw-r--r--   0 arkanepetra  (1000) arkanepetra  (1000)    25864 2024-05-29 05:18:49.000000 arasea-3.0.7/tests/compile/test_debugmode.py
+-rw-r--r--   0 arkanepetra  (1000) arkanepetra  (1000)     2927 2024-05-29 05:18:49.000000 arasea-3.0.7/tests/compile/test_misc.py
+-rw-r--r--   0 arkanepetra  (1000) arkanepetra  (1000)     4687 2024-05-29 05:18:49.000000 arasea-3.0.7/tests/compile/test_mode.py
+-rw-r--r--   0 arkanepetra  (1000) arkanepetra  (1000)     3259 2024-05-29 05:18:49.000000 arasea-3.0.7/tests/compile/test_monitormode.py
+-rw-r--r--   0 arkanepetra  (1000) arkanepetra  (1000)     2479 2024-05-29 05:18:49.000000 arasea-3.0.7/tests/compile/test_nanguardmode.py
+-rw-r--r--   0 arkanepetra  (1000) arkanepetra  (1000)     2026 2024-05-29 05:18:49.000000 arasea-3.0.7/tests/compile/test_ops.py
+-rw-r--r--   0 arkanepetra  (1000) arkanepetra  (1000)     3557 2024-05-29 05:18:49.000000 arasea-3.0.7/tests/compile/test_profiling.py
+-rw-r--r--   0 arkanepetra  (1000) arkanepetra  (1000)    10290 2024-05-29 05:18:49.000000 arasea-3.0.7/tests/compile/test_shared.py
+drwxrwxr-x   0 arkanepetra  (1000) arkanepetra  (1000)        0 2024-05-29 05:48:23.745434 arasea-3.0.7/tests/d3viz/
+-rw-r--r--   0 arkanepetra  (1000) arkanepetra  (1000)        0 2024-05-29 05:18:49.000000 arasea-3.0.7/tests/d3viz/__init__.py
+-rw-r--r--   0 arkanepetra  (1000) arkanepetra  (1000)     1746 2024-05-29 05:18:49.000000 arasea-3.0.7/tests/d3viz/models.py
+-rw-r--r--   0 arkanepetra  (1000) arkanepetra  (1000)     1790 2024-05-29 05:18:49.000000 arasea-3.0.7/tests/d3viz/test_d3viz.py
+-rw-r--r--   0 arkanepetra  (1000) arkanepetra  (1000)     2102 2024-05-29 05:18:49.000000 arasea-3.0.7/tests/d3viz/test_formatting.py
+drwxrwxr-x   0 arkanepetra  (1000) arkanepetra  (1000)        0 2024-05-29 05:48:23.748434 arasea-3.0.7/tests/graph/
+-rw-r--r--   0 arkanepetra  (1000) arkanepetra  (1000)        0 2024-05-29 05:18:49.000000 arasea-3.0.7/tests/graph/__init__.py
+drwxrwxr-x   0 arkanepetra  (1000) arkanepetra  (1000)        0 2024-05-29 05:48:23.750434 arasea-3.0.7/tests/graph/rewriting/
+-rw-r--r--   0 arkanepetra  (1000) arkanepetra  (1000)        0 2024-05-29 05:18:49.000000 arasea-3.0.7/tests/graph/rewriting/__init__.py
+-rw-r--r--   0 arkanepetra  (1000) arkanepetra  (1000)    28891 2024-05-29 05:18:49.000000 arasea-3.0.7/tests/graph/rewriting/test_basic.py
+-rw-r--r--   0 arkanepetra  (1000) arkanepetra  (1000)     2890 2024-05-29 05:18:49.000000 arasea-3.0.7/tests/graph/rewriting/test_db.py
+-rw-r--r--   0 arkanepetra  (1000) arkanepetra  (1000)     5385 2024-05-29 05:18:49.000000 arasea-3.0.7/tests/graph/rewriting/test_kanren.py
+-rw-r--r--   0 arkanepetra  (1000) arkanepetra  (1000)     8469 2024-05-29 05:18:49.000000 arasea-3.0.7/tests/graph/rewriting/test_unify.py
+-rw-r--r--   0 arkanepetra  (1000) arkanepetra  (1000)     5006 2024-05-29 05:18:49.000000 arasea-3.0.7/tests/graph/rewriting/test_utils.py
+-rw-r--r--   0 arkanepetra  (1000) arkanepetra  (1000)    23703 2024-05-29 05:18:49.000000 arasea-3.0.7/tests/graph/test_basic.py
+-rw-r--r--   0 arkanepetra  (1000) arkanepetra  (1000)    10663 2024-05-29 05:18:49.000000 arasea-3.0.7/tests/graph/test_compute_test_value.py
+-rw-r--r--   0 arkanepetra  (1000) arkanepetra  (1000)    14846 2024-05-29 05:18:49.000000 arasea-3.0.7/tests/graph/test_destroyhandler.py
+-rw-r--r--   0 arkanepetra  (1000) arkanepetra  (1000)     6933 2024-05-29 05:18:49.000000 arasea-3.0.7/tests/graph/test_features.py
+-rw-r--r--   0 arkanepetra  (1000) arkanepetra  (1000)    22433 2024-05-29 05:18:49.000000 arasea-3.0.7/tests/graph/test_fg.py
+-rw-r--r--   0 arkanepetra  (1000) arkanepetra  (1000)     6511 2024-05-29 05:18:49.000000 arasea-3.0.7/tests/graph/test_op.py
+-rw-r--r--   0 arkanepetra  (1000) arkanepetra  (1000)     2089 2024-05-29 05:18:49.000000 arasea-3.0.7/tests/graph/test_sched.py
+-rw-r--r--   0 arkanepetra  (1000) arkanepetra  (1000)     1326 2024-05-29 05:18:49.000000 arasea-3.0.7/tests/graph/test_types.py
+-rw-r--r--   0 arkanepetra  (1000) arkanepetra  (1000)      389 2024-05-29 05:18:49.000000 arasea-3.0.7/tests/graph/test_utils.py
+-rw-r--r--   0 arkanepetra  (1000) arkanepetra  (1000)     4119 2024-05-29 05:18:49.000000 arasea-3.0.7/tests/graph/utils.py
+drwxrwxr-x   0 arkanepetra  (1000) arkanepetra  (1000)        0 2024-05-29 05:48:23.751434 arasea-3.0.7/tests/link/
+-rw-r--r--   0 arkanepetra  (1000) arkanepetra  (1000)        0 2024-05-29 05:18:49.000000 arasea-3.0.7/tests/link/__init__.py
+drwxrwxr-x   0 arkanepetra  (1000) arkanepetra  (1000)        0 2024-05-29 05:48:23.752434 arasea-3.0.7/tests/link/c/
+-rw-r--r--   0 arkanepetra  (1000) arkanepetra  (1000)        0 2024-05-29 05:18:49.000000 arasea-3.0.7/tests/link/c/__init__.py
+-rw-r--r--   0 arkanepetra  (1000) arkanepetra  (1000)    13074 2024-05-29 05:18:49.000000 arasea-3.0.7/tests/link/c/test_basic.py
+-rw-r--r--   0 arkanepetra  (1000) arkanepetra  (1000)     9069 2024-05-29 05:18:49.000000 arasea-3.0.7/tests/link/c/test_cmodule.py
+-rw-r--r--   0 arkanepetra  (1000) arkanepetra  (1000)     6848 2024-05-29 05:18:49.000000 arasea-3.0.7/tests/link/c/test_op.py
+-rw-r--r--   0 arkanepetra  (1000) arkanepetra  (1000)    12881 2024-05-29 05:18:49.000000 arasea-3.0.7/tests/link/c/test_params_type.py
+-rw-r--r--   0 arkanepetra  (1000) arkanepetra  (1000)     8730 2024-05-29 05:18:49.000000 arasea-3.0.7/tests/link/c/test_type.py
+drwxrwxr-x   0 arkanepetra  (1000) arkanepetra  (1000)        0 2024-05-29 05:48:23.756434 arasea-3.0.7/tests/link/numba/
+-rw-r--r--   0 arkanepetra  (1000) arkanepetra  (1000)        0 2024-05-29 05:18:49.000000 arasea-3.0.7/tests/link/numba/__init__.py
+-rw-r--r--   0 arkanepetra  (1000) arkanepetra  (1000)    30411 2024-05-29 05:18:49.000000 arasea-3.0.7/tests/link/numba/test_basic.py
+-rw-r--r--   0 arkanepetra  (1000) arkanepetra  (1000)    15952 2024-05-29 05:18:49.000000 arasea-3.0.7/tests/link/numba/test_elemwise.py
+-rw-r--r--   0 arkanepetra  (1000) arkanepetra  (1000)    13197 2024-05-29 05:18:49.000000 arasea-3.0.7/tests/link/numba/test_extra_ops.py
+-rw-r--r--   0 arkanepetra  (1000) arkanepetra  (1000)    12589 2024-05-29 05:18:49.000000 arasea-3.0.7/tests/link/numba/test_nlinalg.py
+-rw-r--r--   0 arkanepetra  (1000) arkanepetra  (1000)     2038 2024-05-29 05:18:49.000000 arasea-3.0.7/tests/link/numba/test_performance.py
+-rw-r--r--   0 arkanepetra  (1000) arkanepetra  (1000)    16845 2024-05-29 05:18:49.000000 arasea-3.0.7/tests/link/numba/test_random.py
+-rw-r--r--   0 arkanepetra  (1000) arkanepetra  (1000)     4012 2024-05-29 05:18:49.000000 arasea-3.0.7/tests/link/numba/test_scalar.py
+-rw-r--r--   0 arkanepetra  (1000) arkanepetra  (1000)    10723 2024-05-29 05:18:49.000000 arasea-3.0.7/tests/link/numba/test_scan.py
+-rw-r--r--   0 arkanepetra  (1000) arkanepetra  (1000)     2353 2024-05-29 05:18:49.000000 arasea-3.0.7/tests/link/numba/test_sparse.py
+-rw-r--r--   0 arkanepetra  (1000) arkanepetra  (1000)    10235 2024-05-29 05:18:49.000000 arasea-3.0.7/tests/link/numba/test_tensor_basic.py
+-rw-r--r--   0 arkanepetra  (1000) arkanepetra  (1000)     7491 2024-05-29 05:18:49.000000 arasea-3.0.7/tests/link/test_link.py
+-rw-r--r--   0 arkanepetra  (1000) arkanepetra  (1000)     5653 2024-05-29 05:18:49.000000 arasea-3.0.7/tests/link/test_utils.py
+-rw-r--r--   0 arkanepetra  (1000) arkanepetra  (1000)    14430 2024-05-29 05:18:49.000000 arasea-3.0.7/tests/link/test_vm.py
+drwxrwxr-x   0 arkanepetra  (1000) arkanepetra  (1000)        0 2024-05-29 05:48:23.756434 arasea-3.0.7/tests/misc/
+-rw-r--r--   0 arkanepetra  (1000) arkanepetra  (1000)        0 2024-05-29 05:18:49.000000 arasea-3.0.7/tests/misc/__init__.py
+-rw-r--r--   0 arkanepetra  (1000) arkanepetra  (1000)     3533 2024-05-29 05:18:49.000000 arasea-3.0.7/tests/misc/test_may_share_memory.py
+-rw-r--r--   0 arkanepetra  (1000) arkanepetra  (1000)     2212 2024-05-29 05:18:49.000000 arasea-3.0.7/tests/misc/test_pkl_utils.py
+drwxrwxr-x   0 arkanepetra  (1000) arkanepetra  (1000)        0 2024-05-29 05:48:23.758434 arasea-3.0.7/tests/sandbox/
+-rw-r--r--   0 arkanepetra  (1000) arkanepetra  (1000)        0 2024-05-29 05:18:49.000000 arasea-3.0.7/tests/sandbox/__init__.py
+drwxrwxr-x   0 arkanepetra  (1000) arkanepetra  (1000)        0 2024-05-29 05:48:23.758434 arasea-3.0.7/tests/sandbox/linalg/
+-rw-r--r--   0 arkanepetra  (1000) arkanepetra  (1000)        0 2024-05-29 05:18:49.000000 arasea-3.0.7/tests/sandbox/linalg/__init__.py
+-rw-r--r--   0 arkanepetra  (1000) arkanepetra  (1000)     4367 2024-05-29 05:18:49.000000 arasea-3.0.7/tests/sandbox/linalg/test_linalg.py
+-rw-r--r--   0 arkanepetra  (1000) arkanepetra  (1000)      836 2024-05-29 05:18:49.000000 arasea-3.0.7/tests/sandbox/test_minimal.py
+-rw-r--r--   0 arkanepetra  (1000) arkanepetra  (1000)     3777 2024-05-29 05:18:49.000000 arasea-3.0.7/tests/sandbox/test_multinomial.py
+-rw-r--r--   0 arkanepetra  (1000) arkanepetra  (1000)     7233 2024-05-29 05:18:49.000000 arasea-3.0.7/tests/sandbox/test_multinomial_wo_replacement.py
+-rw-r--r--   0 arkanepetra  (1000) arkanepetra  (1000)    34649 2024-05-29 05:18:49.000000 arasea-3.0.7/tests/sandbox/test_rng_mrg.py
+drwxrwxr-x   0 arkanepetra  (1000) arkanepetra  (1000)        0 2024-05-29 05:48:23.760435 arasea-3.0.7/tests/scalar/
+-rw-r--r--   0 arkanepetra  (1000) arkanepetra  (1000)        0 2024-05-29 05:18:49.000000 arasea-3.0.7/tests/scalar/__init__.py
+-rw-r--r--   0 arkanepetra  (1000) arkanepetra  (1000)    16995 2024-05-29 05:18:49.000000 arasea-3.0.7/tests/scalar/test_basic.py
+-rw-r--r--   0 arkanepetra  (1000) arkanepetra  (1000)      991 2024-05-29 05:18:49.000000 arasea-3.0.7/tests/scalar/test_basic_sympy.py
+-rw-r--r--   0 arkanepetra  (1000) arkanepetra  (1000)     2539 2024-05-29 05:18:49.000000 arasea-3.0.7/tests/scalar/test_math.py
+-rw-r--r--   0 arkanepetra  (1000) arkanepetra  (1000)     1897 2024-05-29 05:18:49.000000 arasea-3.0.7/tests/scalar/test_type.py
+drwxrwxr-x   0 arkanepetra  (1000) arkanepetra  (1000)        0 2024-05-29 05:48:23.762435 arasea-3.0.7/tests/scan/
+-rw-r--r--   0 arkanepetra  (1000) arkanepetra  (1000)        0 2024-05-29 05:18:49.000000 arasea-3.0.7/tests/scan/__init__.py
+-rw-r--r--   0 arkanepetra  (1000) arkanepetra  (1000)   133995 2024-05-29 05:18:49.000000 arasea-3.0.7/tests/scan/test_basic.py
+-rw-r--r--   0 arkanepetra  (1000) arkanepetra  (1000)     1777 2024-05-29 05:18:49.000000 arasea-3.0.7/tests/scan/test_checkpoints.py
+-rw-r--r--   0 arkanepetra  (1000) arkanepetra  (1000)    25319 2024-05-29 05:18:49.000000 arasea-3.0.7/tests/scan/test_printing.py
+-rw-r--r--   0 arkanepetra  (1000) arkanepetra  (1000)    56551 2024-05-29 05:18:49.000000 arasea-3.0.7/tests/scan/test_rewriting.py
+-rw-r--r--   0 arkanepetra  (1000) arkanepetra  (1000)    17205 2024-05-29 05:18:49.000000 arasea-3.0.7/tests/scan/test_utils.py
+-rw-r--r--   0 arkanepetra  (1000) arkanepetra  (1000)     4534 2024-05-29 05:18:49.000000 arasea-3.0.7/tests/scan/test_views.py
+drwxrwxr-x   0 arkanepetra  (1000) arkanepetra  (1000)        0 2024-05-29 05:48:23.765435 arasea-3.0.7/tests/sparse/
+-rw-r--r--   0 arkanepetra  (1000) arkanepetra  (1000)        0 2024-05-29 05:18:49.000000 arasea-3.0.7/tests/sparse/__init__.py
+drwxrwxr-x   0 arkanepetra  (1000) arkanepetra  (1000)        0 2024-05-29 05:48:23.765435 arasea-3.0.7/tests/sparse/sandbox/
+-rw-r--r--   0 arkanepetra  (1000) arkanepetra  (1000)        0 2024-05-29 05:18:49.000000 arasea-3.0.7/tests/sparse/sandbox/__init__.py
+-rw-r--r--   0 arkanepetra  (1000) arkanepetra  (1000)     9198 2024-05-29 05:18:49.000000 arasea-3.0.7/tests/sparse/sandbox/test_sp.py
+-rw-r--r--   0 arkanepetra  (1000) arkanepetra  (1000)   116949 2024-05-29 05:18:49.000000 arasea-3.0.7/tests/sparse/test_basic.py
+-rw-r--r--   0 arkanepetra  (1000) arkanepetra  (1000)     5942 2024-05-29 05:18:49.000000 arasea-3.0.7/tests/sparse/test_rewriting.py
+-rw-r--r--   0 arkanepetra  (1000) arkanepetra  (1000)      373 2024-05-29 05:18:49.000000 arasea-3.0.7/tests/sparse/test_sharedvar.py
+-rw-r--r--   0 arkanepetra  (1000) arkanepetra  (1000)     4094 2024-05-29 05:18:49.000000 arasea-3.0.7/tests/sparse/test_sp2.py
+-rw-r--r--   0 arkanepetra  (1000) arkanepetra  (1000)     2485 2024-05-29 05:18:49.000000 arasea-3.0.7/tests/sparse/test_type.py
+-rw-r--r--   0 arkanepetra  (1000) arkanepetra  (1000)     1608 2024-05-29 05:18:49.000000 arasea-3.0.7/tests/sparse/test_utils.py
+-rw-r--r--   0 arkanepetra  (1000) arkanepetra  (1000)     8061 2024-05-29 05:18:49.000000 arasea-3.0.7/tests/sparse/test_var.py
+drwxrwxr-x   0 arkanepetra  (1000) arkanepetra  (1000)        0 2024-05-29 05:48:23.776436 arasea-3.0.7/tests/tensor/
+-rw-r--r--   0 arkanepetra  (1000) arkanepetra  (1000)        0 2024-05-29 05:18:49.000000 arasea-3.0.7/tests/tensor/__init__.py
+-rw-r--r--   0 arkanepetra  (1000) arkanepetra  (1000)     1475 2024-05-29 05:18:49.000000 arasea-3.0.7/tests/tensor/_test_mpi_roundtrip.py
+drwxrwxr-x   0 arkanepetra  (1000) arkanepetra  (1000)        0 2024-05-29 05:48:23.780436 arasea-3.0.7/tests/tensor/nnet/
+-rw-r--r--   0 arkanepetra  (1000) arkanepetra  (1000)        0 2024-05-29 05:18:49.000000 arasea-3.0.7/tests/tensor/nnet/__init__.py
+-rw-r--r--   0 arkanepetra  (1000) arkanepetra  (1000)    15242 2024-05-29 05:18:49.000000 arasea-3.0.7/tests/tensor/nnet/speed_test_conv.py
+-rw-r--r--   0 arkanepetra  (1000) arkanepetra  (1000)   103862 2024-05-29 05:18:49.000000 arasea-3.0.7/tests/tensor/nnet/test_abstract_conv.py
+-rw-r--r--   0 arkanepetra  (1000) arkanepetra  (1000)    42020 2024-05-29 05:18:49.000000 arasea-3.0.7/tests/tensor/nnet/test_basic.py
+-rw-r--r--   0 arkanepetra  (1000) arkanepetra  (1000)    25674 2024-05-29 05:18:49.000000 arasea-3.0.7/tests/tensor/nnet/test_batchnorm.py
+-rw-r--r--   0 arkanepetra  (1000) arkanepetra  (1000)    10203 2024-05-29 05:18:49.000000 arasea-3.0.7/tests/tensor/nnet/test_blocksparse.py
+-rw-r--r--   0 arkanepetra  (1000) arkanepetra  (1000)    28956 2024-05-29 05:18:49.000000 arasea-3.0.7/tests/tensor/nnet/test_conv.py
+-rw-r--r--   0 arkanepetra  (1000) arkanepetra  (1000)     6947 2024-05-29 05:18:49.000000 arasea-3.0.7/tests/tensor/nnet/test_conv3d2d.py
+-rw-r--r--   0 arkanepetra  (1000) arkanepetra  (1000)    21906 2024-05-29 05:18:49.000000 arasea-3.0.7/tests/tensor/nnet/test_corr.py
+-rw-r--r--   0 arkanepetra  (1000) arkanepetra  (1000)    21818 2024-05-29 05:18:49.000000 arasea-3.0.7/tests/tensor/nnet/test_corr3d.py
+-rw-r--r--   0 arkanepetra  (1000) arkanepetra  (1000)     6197 2024-05-29 05:18:49.000000 arasea-3.0.7/tests/tensor/nnet/test_ctc.py
+-rw-r--r--   0 arkanepetra  (1000) arkanepetra  (1000)    25410 2024-05-29 05:18:49.000000 arasea-3.0.7/tests/tensor/nnet/test_neighbours.py
+-rw-r--r--   0 arkanepetra  (1000) arkanepetra  (1000)     1694 2024-05-29 05:18:49.000000 arasea-3.0.7/tests/tensor/nnet/test_rewriting.py
+-rw-r--r--   0 arkanepetra  (1000) arkanepetra  (1000)     4825 2024-05-29 05:18:49.000000 arasea-3.0.7/tests/tensor/nnet/test_sigm.py
+drwxrwxr-x   0 arkanepetra  (1000) arkanepetra  (1000)        0 2024-05-29 05:48:23.782436 arasea-3.0.7/tests/tensor/random/
+-rw-r--r--   0 arkanepetra  (1000) arkanepetra  (1000)        0 2024-05-29 05:18:49.000000 arasea-3.0.7/tests/tensor/random/__init__.py
+-rw-r--r--   0 arkanepetra  (1000) arkanepetra  (1000)    41757 2024-05-29 05:18:49.000000 arasea-3.0.7/tests/tensor/random/test_basic.py
+-rw-r--r--   0 arkanepetra  (1000) arkanepetra  (1000)     5974 2024-05-29 05:18:49.000000 arasea-3.0.7/tests/tensor/random/test_op.py
+-rw-r--r--   0 arkanepetra  (1000) arkanepetra  (1000)    17712 2024-05-29 05:18:49.000000 arasea-3.0.7/tests/tensor/random/test_rewriting.py
+-rw-r--r--   0 arkanepetra  (1000) arkanepetra  (1000)     6674 2024-05-29 05:18:49.000000 arasea-3.0.7/tests/tensor/random/test_type.py
+-rw-r--r--   0 arkanepetra  (1000) arkanepetra  (1000)    10653 2024-05-29 05:18:49.000000 arasea-3.0.7/tests/tensor/random/test_utils.py
+-rw-r--r--   0 arkanepetra  (1000) arkanepetra  (1000)     3642 2024-05-29 05:18:49.000000 arasea-3.0.7/tests/tensor/random/test_var.py
+drwxrwxr-x   0 arkanepetra  (1000) arkanepetra  (1000)        0 2024-05-29 05:48:23.785436 arasea-3.0.7/tests/tensor/rewriting/
+-rw-r--r--   0 arkanepetra  (1000) arkanepetra  (1000)        0 2024-05-29 05:18:49.000000 arasea-3.0.7/tests/tensor/rewriting/__init__.py
+-rw-r--r--   0 arkanepetra  (1000) arkanepetra  (1000)    63207 2024-05-29 05:18:49.000000 arasea-3.0.7/tests/tensor/rewriting/test_basic.py
+-rw-r--r--   0 arkanepetra  (1000) arkanepetra  (1000)    41140 2024-05-29 05:18:49.000000 arasea-3.0.7/tests/tensor/rewriting/test_elemwise.py
+-rw-r--r--   0 arkanepetra  (1000) arkanepetra  (1000)    10481 2024-05-29 05:18:49.000000 arasea-3.0.7/tests/tensor/rewriting/test_extra_ops.py
+-rw-r--r--   0 arkanepetra  (1000) arkanepetra  (1000)   166414 2024-05-29 05:18:49.000000 arasea-3.0.7/tests/tensor/rewriting/test_math.py
+-rw-r--r--   0 arkanepetra  (1000) arkanepetra  (1000)    18170 2024-05-29 05:18:49.000000 arasea-3.0.7/tests/tensor/rewriting/test_shape.py
+-rw-r--r--   0 arkanepetra  (1000) arkanepetra  (1000)     4483 2024-05-29 05:18:49.000000 arasea-3.0.7/tests/tensor/rewriting/test_special.py
+-rw-r--r--   0 arkanepetra  (1000) arkanepetra  (1000)    80378 2024-05-29 05:18:49.000000 arasea-3.0.7/tests/tensor/rewriting/test_subtensor.py
+-rw-r--r--   0 arkanepetra  (1000) arkanepetra  (1000)     7105 2024-05-29 05:18:49.000000 arasea-3.0.7/tests/tensor/rewriting/test_uncanonicalize.py
+drwxrwxr-x   0 arkanepetra  (1000) arkanepetra  (1000)        0 2024-05-29 05:48:23.786436 arasea-3.0.7/tests/tensor/signal/
+-rw-r--r--   0 arkanepetra  (1000) arkanepetra  (1000)        0 2024-05-29 05:18:49.000000 arasea-3.0.7/tests/tensor/signal/__init__.py
+-rw-r--r--   0 arkanepetra  (1000) arkanepetra  (1000)     4145 2024-05-29 05:18:49.000000 arasea-3.0.7/tests/tensor/signal/test_conv.py
+-rw-r--r--   0 arkanepetra  (1000) arkanepetra  (1000)    51694 2024-05-29 05:18:49.000000 arasea-3.0.7/tests/tensor/signal/test_pool.py
+-rw-r--r--   0 arkanepetra  (1000) arkanepetra  (1000)   148595 2024-05-29 05:18:49.000000 arasea-3.0.7/tests/tensor/test_basic.py
+-rw-r--r--   0 arkanepetra  (1000) arkanepetra  (1000)    99618 2024-05-29 05:18:49.000000 arasea-3.0.7/tests/tensor/test_blas.py
+-rw-r--r--   0 arkanepetra  (1000) arkanepetra  (1000)    14554 2024-05-29 05:18:49.000000 arasea-3.0.7/tests/tensor/test_blas_c.py
+-rw-r--r--   0 arkanepetra  (1000) arkanepetra  (1000)     2550 2024-05-29 05:18:49.000000 arasea-3.0.7/tests/tensor/test_blas_scipy.py
+-rw-r--r--   0 arkanepetra  (1000) arkanepetra  (1000)     4161 2024-05-29 05:18:49.000000 arasea-3.0.7/tests/tensor/test_casting.py
+-rw-r--r--   0 arkanepetra  (1000) arkanepetra  (1000)     4344 2024-05-29 05:18:49.000000 arasea-3.0.7/tests/tensor/test_complex.py
+-rw-r--r--   0 arkanepetra  (1000) arkanepetra  (1000)    34431 2024-05-29 05:18:49.000000 arasea-3.0.7/tests/tensor/test_elemwise.py
+-rw-r--r--   0 arkanepetra  (1000) arkanepetra  (1000)    47330 2024-05-29 05:18:49.000000 arasea-3.0.7/tests/tensor/test_extra_ops.py
+-rw-r--r--   0 arkanepetra  (1000) arkanepetra  (1000)     6580 2024-05-29 05:18:49.000000 arasea-3.0.7/tests/tensor/test_fft.py
+-rw-r--r--   0 arkanepetra  (1000) arkanepetra  (1000)     2218 2024-05-29 05:18:49.000000 arasea-3.0.7/tests/tensor/test_fourier.py
+-rw-r--r--   0 arkanepetra  (1000) arkanepetra  (1000)     4059 2024-05-29 05:18:49.000000 arasea-3.0.7/tests/tensor/test_gc.py
+-rw-r--r--   0 arkanepetra  (1000) arkanepetra  (1000)    11957 2024-05-29 05:18:49.000000 arasea-3.0.7/tests/tensor/test_inplace.py
+-rw-r--r--   0 arkanepetra  (1000) arkanepetra  (1000)     2080 2024-05-29 05:18:49.000000 arasea-3.0.7/tests/tensor/test_io.py
+-rw-r--r--   0 arkanepetra  (1000) arkanepetra  (1000)     6667 2024-05-29 05:18:49.000000 arasea-3.0.7/tests/tensor/test_keepdims.py
+-rw-r--r--   0 arkanepetra  (1000) arkanepetra  (1000)   123957 2024-05-29 05:18:49.000000 arasea-3.0.7/tests/tensor/test_math.py
+-rw-r--r--   0 arkanepetra  (1000) arkanepetra  (1000)    29972 2024-05-29 05:18:49.000000 arasea-3.0.7/tests/tensor/test_math_scipy.py
+-rw-r--r--   0 arkanepetra  (1000) arkanepetra  (1000)     2345 2024-05-29 05:18:49.000000 arasea-3.0.7/tests/tensor/test_merge.py
+-rw-r--r--   0 arkanepetra  (1000) arkanepetra  (1000)     2467 2024-05-29 05:18:49.000000 arasea-3.0.7/tests/tensor/test_misc.py
+-rw-r--r--   0 arkanepetra  (1000) arkanepetra  (1000)     2946 2024-05-29 05:18:49.000000 arasea-3.0.7/tests/tensor/test_mpi.py
+-rw-r--r--   0 arkanepetra  (1000) arkanepetra  (1000)    14603 2024-05-29 05:18:49.000000 arasea-3.0.7/tests/tensor/test_nlinalg.py
+-rw-r--r--   0 arkanepetra  (1000) arkanepetra  (1000)    22601 2024-05-29 05:18:49.000000 arasea-3.0.7/tests/tensor/test_shape.py
+-rw-r--r--   0 arkanepetra  (1000) arkanepetra  (1000)    27332 2024-05-29 05:18:49.000000 arasea-3.0.7/tests/tensor/test_sharedvar.py
+-rw-r--r--   0 arkanepetra  (1000) arkanepetra  (1000)    18787 2024-05-29 05:18:49.000000 arasea-3.0.7/tests/tensor/test_slinalg.py
+-rw-r--r--   0 arkanepetra  (1000) arkanepetra  (1000)    18538 2024-05-29 05:18:49.000000 arasea-3.0.7/tests/tensor/test_sort.py
+-rw-r--r--   0 arkanepetra  (1000) arkanepetra  (1000)     5148 2024-05-29 05:18:49.000000 arasea-3.0.7/tests/tensor/test_special.py
+-rw-r--r--   0 arkanepetra  (1000) arkanepetra  (1000)    91185 2024-05-29 05:18:49.000000 arasea-3.0.7/tests/tensor/test_subtensor.py
+-rw-r--r--   0 arkanepetra  (1000) arkanepetra  (1000)     9802 2024-05-29 05:18:49.000000 arasea-3.0.7/tests/tensor/test_type.py
+-rw-r--r--   0 arkanepetra  (1000) arkanepetra  (1000)     1766 2024-05-29 05:18:49.000000 arasea-3.0.7/tests/tensor/test_type_other.py
+-rw-r--r--   0 arkanepetra  (1000) arkanepetra  (1000)     2417 2024-05-29 05:18:49.000000 arasea-3.0.7/tests/tensor/test_utils.py
+-rw-r--r--   0 arkanepetra  (1000) arkanepetra  (1000)    12727 2024-05-29 05:18:49.000000 arasea-3.0.7/tests/tensor/test_var.py
+-rw-r--r--   0 arkanepetra  (1000) arkanepetra  (1000)      716 2024-05-29 05:18:49.000000 arasea-3.0.7/tests/tensor/test_xlogx.py
+-rw-r--r--   0 arkanepetra  (1000) arkanepetra  (1000)    38712 2024-05-29 05:18:49.000000 arasea-3.0.7/tests/tensor/utils.py
+-rw-r--r--   0 arkanepetra  (1000) arkanepetra  (1000)     2922 2024-05-29 05:18:49.000000 arasea-3.0.7/tests/test_breakpoint.py
+-rw-r--r--   0 arkanepetra  (1000) arkanepetra  (1000)    10470 2024-05-29 05:18:49.000000 arasea-3.0.7/tests/test_config.py
+-rw-r--r--   0 arkanepetra  (1000) arkanepetra  (1000)    34472 2024-05-29 05:18:49.000000 arasea-3.0.7/tests/test_gradient.py
+-rw-r--r--   0 arkanepetra  (1000) arkanepetra  (1000)    25050 2024-05-29 05:18:49.000000 arasea-3.0.7/tests/test_ifelse.py
+-rw-r--r--   0 arkanepetra  (1000) arkanepetra  (1000)    13025 2024-05-29 05:18:49.000000 arasea-3.0.7/tests/test_printing.py
+-rw-r--r--   0 arkanepetra  (1000) arkanepetra  (1000)     5383 2024-05-29 05:18:49.000000 arasea-3.0.7/tests/test_raise_op.py
+-rw-r--r--   0 arkanepetra  (1000) arkanepetra  (1000)    13207 2024-05-29 05:18:49.000000 arasea-3.0.7/tests/test_rop.py
+-rw-r--r--   0 arkanepetra  (1000) arkanepetra  (1000)     1679 2024-05-29 05:18:49.000000 arasea-3.0.7/tests/test_updates.py
+drwxrwxr-x   0 arkanepetra  (1000) arkanepetra  (1000)        0 2024-05-29 05:48:23.787437 arasea-3.0.7/tests/typed_list/
+-rw-r--r--   0 arkanepetra  (1000) arkanepetra  (1000)        0 2024-05-29 05:18:49.000000 arasea-3.0.7/tests/typed_list/__init__.py
+-rw-r--r--   0 arkanepetra  (1000) arkanepetra  (1000)    17535 2024-05-29 05:18:49.000000 arasea-3.0.7/tests/typed_list/test_basic.py
+-rw-r--r--   0 arkanepetra  (1000) arkanepetra  (1000)     4926 2024-05-29 05:18:49.000000 arasea-3.0.7/tests/typed_list/test_rewriting.py
+-rw-r--r--   0 arkanepetra  (1000) arkanepetra  (1000)     4903 2024-05-29 05:18:49.000000 arasea-3.0.7/tests/typed_list/test_type.py
+-rw-r--r--   0 arkanepetra  (1000) arkanepetra  (1000)    14042 2024-05-29 05:18:49.000000 arasea-3.0.7/tests/unittest_tools.py
```

### Comparing `arasea-3.0.6/LICENSE.txt` & `arasea-3.0.7/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `arasea-3.0.6/PKG-INFO` & `arasea-3.0.7/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: arasea
-Version: 3.0.6
+Version: 3.0.7
 Summary: A library for defining, optimizing, and efficiently evaluating mathematical expressions involving multi-dimensional arrays.
 Home-page: https://github.com/arasea-devs/arasea
 Author: arasea-devs
 Author-email: arasea.devs@gmail.com
 License: BSD-3-Clause
 Keywords: arasea,math,numerical,symbolic,blas,numpy,autodiff,differentiation
 Classifier: Development Status :: 6 - Mature
```

### Comparing `arasea-3.0.6/README.md` & `arasea-3.0.7/README.md`

 * *Files identical despite different names*

### Comparing `arasea-3.0.6/arasea/__init__.py` & `arasea-3.0.7/arasea/__init__.py`

 * *Files identical despite different names*

### Comparing `arasea-3.0.6/arasea/benchmark.log` & `arasea-3.0.7/arasea/benchmark.log`

 * *Files identical despite different names*

### Comparing `arasea-3.0.6/arasea/bin/arasea_cache.py` & `arasea-3.0.7/arasea/bin/arasea_cache.py`

 * *Files identical despite different names*

### Comparing `arasea-3.0.6/arasea/breakpoint.py` & `arasea-3.0.7/arasea/breakpoint.py`

 * *Files identical despite different names*

### Comparing `arasea-3.0.6/arasea/compile/__init__.py` & `arasea-3.0.7/arasea/compile/__init__.py`

 * *Files identical despite different names*

### Comparing `arasea-3.0.6/arasea/compile/builders.py` & `arasea-3.0.7/arasea/compile/builders.py`

 * *Files identical despite different names*

### Comparing `arasea-3.0.6/arasea/compile/compiledir.py` & `arasea-3.0.7/arasea/compile/compiledir.py`

 * *Files identical despite different names*

### Comparing `arasea-3.0.6/arasea/compile/compilelock.py` & `arasea-3.0.7/arasea/compile/compilelock.py`

 * *Files identical despite different names*

### Comparing `arasea-3.0.6/arasea/compile/debugmode.py` & `arasea-3.0.7/arasea/compile/debugmode.py`

 * *Files identical despite different names*

### Comparing `arasea-3.0.6/arasea/compile/function/__init__.py` & `arasea-3.0.7/arasea/compile/function/__init__.py`

 * *Files identical despite different names*

### Comparing `arasea-3.0.6/arasea/compile/function/pfunc.py` & `arasea-3.0.7/arasea/compile/function/pfunc.py`

 * *Files identical despite different names*

### Comparing `arasea-3.0.6/arasea/compile/function/types.py` & `arasea-3.0.7/arasea/compile/function/types.py`

 * *Files identical despite different names*

### Comparing `arasea-3.0.6/arasea/compile/io.py` & `arasea-3.0.7/arasea/compile/io.py`

 * *Files identical despite different names*

### Comparing `arasea-3.0.6/arasea/compile/mode.py` & `arasea-3.0.7/arasea/compile/mode.py`

 * *Files identical despite different names*

### Comparing `arasea-3.0.6/arasea/compile/monitormode.py` & `arasea-3.0.7/arasea/compile/monitormode.py`

 * *Files identical despite different names*

### Comparing `arasea-3.0.6/arasea/compile/nanguardmode.py` & `arasea-3.0.7/arasea/compile/nanguardmode.py`

 * *Files identical despite different names*

### Comparing `arasea-3.0.6/arasea/compile/ops.py` & `arasea-3.0.7/arasea/compile/ops.py`

 * *Files identical despite different names*

### Comparing `arasea-3.0.6/arasea/compile/profiling.py` & `arasea-3.0.7/arasea/compile/profiling.py`

 * *Files identical despite different names*

### Comparing `arasea-3.0.6/arasea/compile/sharedvalue.py` & `arasea-3.0.7/arasea/compile/sharedvalue.py`

 * *Files identical despite different names*

### Comparing `arasea-3.0.6/arasea/configdefaults.py` & `arasea-3.0.7/arasea/configdefaults.py`

 * *Files identical despite different names*

### Comparing `arasea-3.0.6/arasea/configparser.py` & `arasea-3.0.7/arasea/configparser.py`

 * *Files identical despite different names*

### Comparing `arasea-3.0.6/arasea/d3viz/d3viz.py` & `arasea-3.0.7/arasea/d3viz/d3viz.py`

 * *Files identical despite different names*

### Comparing `arasea-3.0.6/arasea/d3viz/formatting.py` & `arasea-3.0.7/arasea/d3viz/formatting.py`

 * *Files identical despite different names*

### Comparing `arasea-3.0.6/arasea/gradient.py` & `arasea-3.0.7/arasea/gradient.py`

 * *Files identical despite different names*

### Comparing `arasea-3.0.6/arasea/graph/basic.py` & `arasea-3.0.7/arasea/graph/basic.py`

 * *Files identical despite different names*

### Comparing `arasea-3.0.6/arasea/graph/destroyhandler.py` & `arasea-3.0.7/arasea/graph/destroyhandler.py`

 * *Files identical despite different names*

### Comparing `arasea-3.0.6/arasea/graph/features.py` & `arasea-3.0.7/arasea/graph/features.py`

 * *Files identical despite different names*

### Comparing `arasea-3.0.6/arasea/graph/fg.py` & `arasea-3.0.7/arasea/graph/fg.py`

 * *Files identical despite different names*

### Comparing `arasea-3.0.6/arasea/graph/null_type.py` & `arasea-3.0.7/arasea/graph/null_type.py`

 * *Files identical despite different names*

### Comparing `arasea-3.0.6/arasea/graph/op.py` & `arasea-3.0.7/arasea/graph/op.py`

 * *Files identical despite different names*

### Comparing `arasea-3.0.6/arasea/graph/opt.py` & `arasea-3.0.7/arasea/graph/opt.py`

 * *Files identical despite different names*

### Comparing `arasea-3.0.6/arasea/graph/opt_utils.py` & `arasea-3.0.7/arasea/graph/opt_utils.py`

 * *Files identical despite different names*

### Comparing `arasea-3.0.6/arasea/graph/optdb.py` & `arasea-3.0.7/arasea/graph/optdb.py`

 * *Files identical despite different names*

### Comparing `arasea-3.0.6/arasea/graph/rewriting/basic.py` & `arasea-3.0.7/arasea/graph/rewriting/basic.py`

 * *Files identical despite different names*

### Comparing `arasea-3.0.6/arasea/graph/rewriting/db.py` & `arasea-3.0.7/arasea/graph/rewriting/db.py`

 * *Files identical despite different names*

### Comparing `arasea-3.0.6/arasea/graph/rewriting/kanren.py` & `arasea-3.0.7/arasea/graph/rewriting/kanren.py`

 * *Files identical despite different names*

### Comparing `arasea-3.0.6/arasea/graph/rewriting/unify.py` & `arasea-3.0.7/arasea/graph/rewriting/unify.py`

 * *Files identical despite different names*

### Comparing `arasea-3.0.6/arasea/graph/rewriting/utils.py` & `arasea-3.0.7/arasea/graph/rewriting/utils.py`

 * *Files identical despite different names*

### Comparing `arasea-3.0.6/arasea/graph/sched.py` & `arasea-3.0.7/arasea/graph/sched.py`

 * *Files identical despite different names*

### Comparing `arasea-3.0.6/arasea/graph/type.py` & `arasea-3.0.7/arasea/graph/type.py`

 * *Files identical despite different names*

### Comparing `arasea-3.0.6/arasea/graph/utils.py` & `arasea-3.0.7/arasea/graph/utils.py`

 * *Files identical despite different names*

### Comparing `arasea-3.0.6/arasea/ifelse.py` & `arasea-3.0.7/arasea/ifelse.py`

 * *Files identical despite different names*

### Comparing `arasea-3.0.6/arasea/link/basic.py` & `arasea-3.0.7/arasea/link/basic.py`

 * *Files identical despite different names*

### Comparing `arasea-3.0.6/arasea/link/c/basic.py` & `arasea-3.0.7/arasea/link/c/basic.py`

 * *Files identical despite different names*

### Comparing `arasea-3.0.6/arasea/link/c/cmodule.py` & `arasea-3.0.7/arasea/link/c/cmodule.py`

 * *Files identical despite different names*

### Comparing `arasea-3.0.6/arasea/link/c/cutils.py` & `arasea-3.0.7/arasea/link/c/cutils.py`

 * *Files identical despite different names*

### Comparing `arasea-3.0.6/arasea/link/c/cvm.py` & `arasea-3.0.7/arasea/link/c/cvm.py`

 * *Files identical despite different names*

### Comparing `arasea-3.0.6/arasea/link/c/interface.py` & `arasea-3.0.7/arasea/link/c/interface.py`

 * *Files identical despite different names*

### Comparing `arasea-3.0.6/arasea/link/c/lazylinker_c.py` & `arasea-3.0.7/arasea/link/c/lazylinker_c.py`

 * *Files identical despite different names*

### Comparing `arasea-3.0.6/arasea/link/c/op.py` & `arasea-3.0.7/arasea/link/c/op.py`

 * *Files identical despite different names*

### Comparing `arasea-3.0.6/arasea/link/c/params_type.py` & `arasea-3.0.7/arasea/link/c/params_type.py`

 * *Files identical despite different names*

### Comparing `arasea-3.0.6/arasea/link/c/type.py` & `arasea-3.0.7/arasea/link/c/type.py`

 * *Files identical despite different names*

### Comparing `arasea-3.0.6/arasea/link/jax/dispatch/__init__.py` & `arasea-3.0.7/arasea/link/jax/dispatch/__init__.py`

 * *Files identical despite different names*

### Comparing `arasea-3.0.6/arasea/link/jax/dispatch/basic.py` & `arasea-3.0.7/arasea/link/jax/dispatch/basic.py`

 * *Files identical despite different names*

### Comparing `arasea-3.0.6/arasea/link/jax/dispatch/elemwise.py` & `arasea-3.0.7/arasea/link/jax/dispatch/elemwise.py`

 * *Files identical despite different names*

### Comparing `arasea-3.0.6/arasea/link/jax/dispatch/extra_ops.py` & `arasea-3.0.7/arasea/link/jax/dispatch/extra_ops.py`

 * *Files identical despite different names*

### Comparing `arasea-3.0.6/arasea/link/jax/dispatch/nlinalg.py` & `arasea-3.0.7/arasea/link/jax/dispatch/nlinalg.py`

 * *Files identical despite different names*

### Comparing `arasea-3.0.6/arasea/link/jax/dispatch/random.py` & `arasea-3.0.7/arasea/link/jax/dispatch/random.py`

 * *Files identical despite different names*

### Comparing `arasea-3.0.6/arasea/link/jax/dispatch/scalar.py` & `arasea-3.0.7/arasea/link/jax/dispatch/scalar.py`

 * *Files identical despite different names*

### Comparing `arasea-3.0.6/arasea/link/jax/dispatch/scan.py` & `arasea-3.0.7/arasea/link/jax/dispatch/scan.py`

 * *Files identical despite different names*

### Comparing `arasea-3.0.6/arasea/link/jax/dispatch/shape.py` & `arasea-3.0.7/arasea/link/jax/dispatch/shape.py`

 * *Files identical despite different names*

### Comparing `arasea-3.0.6/arasea/link/jax/dispatch/slinalg.py` & `arasea-3.0.7/arasea/link/jax/dispatch/slinalg.py`

 * *Files identical despite different names*

### Comparing `arasea-3.0.6/arasea/link/jax/dispatch/subtensor.py` & `arasea-3.0.7/arasea/link/jax/dispatch/subtensor.py`

 * *Files identical despite different names*

### Comparing `arasea-3.0.6/arasea/link/jax/dispatch/tensor_basic.py` & `arasea-3.0.7/arasea/link/jax/dispatch/tensor_basic.py`

 * *Files identical despite different names*

### Comparing `arasea-3.0.6/arasea/link/jax/linker.py` & `arasea-3.0.7/arasea/link/jax/linker.py`

 * *Files identical despite different names*

### Comparing `arasea-3.0.6/arasea/link/numba/dispatch/basic.py` & `arasea-3.0.7/arasea/link/numba/dispatch/basic.py`

 * *Files identical despite different names*

### Comparing `arasea-3.0.6/arasea/link/numba/dispatch/elemwise.py` & `arasea-3.0.7/arasea/link/numba/dispatch/elemwise.py`

 * *Files identical despite different names*

### Comparing `arasea-3.0.6/arasea/link/numba/dispatch/extra_ops.py` & `arasea-3.0.7/arasea/link/numba/dispatch/extra_ops.py`

 * *Files identical despite different names*

### Comparing `arasea-3.0.6/arasea/link/numba/dispatch/nlinalg.py` & `arasea-3.0.7/arasea/link/numba/dispatch/nlinalg.py`

 * *Files identical despite different names*

### Comparing `arasea-3.0.6/arasea/link/numba/dispatch/random.py` & `arasea-3.0.7/arasea/link/numba/dispatch/random.py`

 * *Files identical despite different names*

### Comparing `arasea-3.0.6/arasea/link/numba/dispatch/scalar.py` & `arasea-3.0.7/arasea/link/numba/dispatch/scalar.py`

 * *Files identical despite different names*

### Comparing `arasea-3.0.6/arasea/link/numba/dispatch/scan.py` & `arasea-3.0.7/arasea/link/numba/dispatch/scan.py`

 * *Files identical despite different names*

### Comparing `arasea-3.0.6/arasea/link/numba/dispatch/sparse.py` & `arasea-3.0.7/arasea/link/numba/dispatch/sparse.py`

 * *Files identical despite different names*

### Comparing `arasea-3.0.6/arasea/link/numba/dispatch/tensor_basic.py` & `arasea-3.0.7/arasea/link/numba/dispatch/tensor_basic.py`

 * *Files identical despite different names*

### Comparing `arasea-3.0.6/arasea/link/numba/linker.py` & `arasea-3.0.7/arasea/link/numba/linker.py`

 * *Files identical despite different names*

### Comparing `arasea-3.0.6/arasea/link/utils.py` & `arasea-3.0.7/arasea/link/utils.py`

 * *Files identical despite different names*

### Comparing `arasea-3.0.6/arasea/link/vm.py` & `arasea-3.0.7/arasea/link/vm.py`

 * *Files identical despite different names*

### Comparing `arasea-3.0.6/arasea/misc/check_blas.py` & `arasea-3.0.7/arasea/misc/check_blas.py`

 * *Files identical despite different names*

### Comparing `arasea-3.0.6/arasea/misc/check_duplicate_key.py` & `arasea-3.0.7/arasea/misc/check_duplicate_key.py`

 * *Files identical despite different names*

### Comparing `arasea-3.0.6/arasea/misc/elemwise_openmp_speedup.py` & `arasea-3.0.7/arasea/misc/elemwise_openmp_speedup.py`

 * *Files identical despite different names*

### Comparing `arasea-3.0.6/arasea/misc/elemwise_time_test.py` & `arasea-3.0.7/arasea/misc/elemwise_time_test.py`

 * *Files identical despite different names*

### Comparing `arasea-3.0.6/arasea/misc/frozendict.py` & `arasea-3.0.7/arasea/misc/frozendict.py`

 * *Files identical despite different names*

### Comparing `arasea-3.0.6/arasea/misc/latence_gpu_transfert.py` & `arasea-3.0.7/arasea/misc/latence_gpu_transfert.py`

 * *Files identical despite different names*

### Comparing `arasea-3.0.6/arasea/misc/may_share_memory.py` & `arasea-3.0.7/arasea/misc/may_share_memory.py`

 * *Files identical despite different names*

### Comparing `arasea-3.0.6/arasea/misc/ordered_set.py` & `arasea-3.0.7/arasea/misc/ordered_set.py`

 * *Files identical despite different names*

### Comparing `arasea-3.0.6/arasea/misc/pkl_utils.py` & `arasea-3.0.7/arasea/misc/pkl_utils.py`

 * *Files identical despite different names*

### Comparing `arasea-3.0.6/arasea/misc/safe_asarray.py` & `arasea-3.0.7/arasea/misc/safe_asarray.py`

 * *Files identical despite different names*

### Comparing `arasea-3.0.6/arasea/printing.py` & `arasea-3.0.7/arasea/printing.py`

 * *Files identical despite different names*

### Comparing `arasea-3.0.6/arasea/raise_op.py` & `arasea-3.0.7/arasea/raise_op.py`

 * *Files identical despite different names*

### Comparing `arasea-3.0.6/arasea/sandbox/fourier.py` & `arasea-3.0.7/arasea/sandbox/fourier.py`

 * *Files identical despite different names*

### Comparing `arasea-3.0.6/arasea/sandbox/linalg/ops.py` & `arasea-3.0.7/arasea/sandbox/linalg/ops.py`

 * *Files identical despite different names*

### Comparing `arasea-3.0.6/arasea/sandbox/minimal.py` & `arasea-3.0.7/arasea/sandbox/minimal.py`

 * *Files identical despite different names*

### Comparing `arasea-3.0.6/arasea/sandbox/multinomial.py` & `arasea-3.0.7/arasea/sandbox/multinomial.py`

 * *Files identical despite different names*

### Comparing `arasea-3.0.6/arasea/sandbox/rng_mrg.py` & `arasea-3.0.7/arasea/sandbox/rng_mrg.py`

 * *Files identical despite different names*

### Comparing `arasea-3.0.6/arasea/scalar/__init__.py` & `arasea-3.0.7/arasea/scalar/__init__.py`

 * *Files identical despite different names*

### Comparing `arasea-3.0.6/arasea/scalar/basic.py` & `arasea-3.0.7/arasea/scalar/basic.py`

 * *Files identical despite different names*

### Comparing `arasea-3.0.6/arasea/scalar/basic_sympy.py` & `arasea-3.0.7/arasea/scalar/basic_sympy.py`

 * *Files identical despite different names*

### Comparing `arasea-3.0.6/arasea/scalar/math.py` & `arasea-3.0.7/arasea/scalar/math.py`

 * *Files identical despite different names*

### Comparing `arasea-3.0.6/arasea/scalar/sharedvar.py` & `arasea-3.0.7/arasea/scalar/sharedvar.py`

 * *Files identical despite different names*

### Comparing `arasea-3.0.6/arasea/scan/__init__.py` & `arasea-3.0.7/arasea/scan/__init__.py`

 * *Files identical despite different names*

### Comparing `arasea-3.0.6/arasea/scan/basic.py` & `arasea-3.0.7/arasea/scan/basic.py`

 * *Files identical despite different names*

### Comparing `arasea-3.0.6/arasea/scan/checkpoints.py` & `arasea-3.0.7/arasea/scan/checkpoints.py`

 * *Files identical despite different names*

### Comparing `arasea-3.0.6/arasea/scan/op.py` & `arasea-3.0.7/arasea/scan/op.py`

 * *Files identical despite different names*

### Comparing `arasea-3.0.6/arasea/scan/rewriting.py` & `arasea-3.0.7/arasea/scan/rewriting.py`

 * *Files identical despite different names*

### Comparing `arasea-3.0.6/arasea/scan/scan_perform_ext.py` & `arasea-3.0.7/arasea/scan/scan_perform_ext.py`

 * *Files identical despite different names*

### Comparing `arasea-3.0.6/arasea/scan/utils.py` & `arasea-3.0.7/arasea/scan/utils.py`

 * *Files identical despite different names*

### Comparing `arasea-3.0.6/arasea/scan/views.py` & `arasea-3.0.7/arasea/scan/views.py`

 * *Files identical despite different names*

### Comparing `arasea-3.0.6/arasea/sparse/__init__.py` & `arasea-3.0.7/arasea/sparse/__init__.py`

 * *Files identical despite different names*

### Comparing `arasea-3.0.6/arasea/sparse/basic.py` & `arasea-3.0.7/arasea/sparse/basic.py`

 * *Files identical despite different names*

### Comparing `arasea-3.0.6/arasea/sparse/rewriting.py` & `arasea-3.0.7/arasea/sparse/rewriting.py`

 * *Files identical despite different names*

### Comparing `arasea-3.0.6/arasea/sparse/sandbox/sp.py` & `arasea-3.0.7/arasea/sparse/sandbox/sp.py`

 * *Files identical despite different names*

### Comparing `arasea-3.0.6/arasea/sparse/sandbox/sp2.py` & `arasea-3.0.7/arasea/sparse/sandbox/sp2.py`

 * *Files identical despite different names*

### Comparing `arasea-3.0.6/arasea/sparse/sharedvar.py` & `arasea-3.0.7/arasea/sparse/sharedvar.py`

 * *Files identical despite different names*

### Comparing `arasea-3.0.6/arasea/sparse/type.py` & `arasea-3.0.7/arasea/sparse/type.py`

 * *Files identical despite different names*

### Comparing `arasea-3.0.6/arasea/sparse/utils.py` & `arasea-3.0.7/arasea/sparse/utils.py`

 * *Files identical despite different names*

### Comparing `arasea-3.0.6/arasea/tensor/__init__.py` & `arasea-3.0.7/arasea/tensor/__init__.py`

 * *Files identical despite different names*

### Comparing `arasea-3.0.6/arasea/tensor/basic.py` & `arasea-3.0.7/arasea/tensor/basic.py`

 * *Files identical despite different names*

### Comparing `arasea-3.0.6/arasea/tensor/blas.py` & `arasea-3.0.7/arasea/tensor/blas.py`

 * *Files identical despite different names*

### Comparing `arasea-3.0.6/arasea/tensor/blas_c.py` & `arasea-3.0.7/arasea/tensor/blas_c.py`

 * *Files identical despite different names*

### Comparing `arasea-3.0.6/arasea/tensor/blas_headers.py` & `arasea-3.0.7/arasea/tensor/blas_headers.py`

 * *Files identical despite different names*

### Comparing `arasea-3.0.6/arasea/tensor/blas_scipy.py` & `arasea-3.0.7/arasea/tensor/blas_scipy.py`

 * *Files identical despite different names*

### Comparing `arasea-3.0.6/arasea/tensor/elemwise.py` & `arasea-3.0.7/arasea/tensor/elemwise.py`

 * *Files identical despite different names*

### Comparing `arasea-3.0.6/arasea/tensor/elemwise_cgen.py` & `arasea-3.0.7/arasea/tensor/elemwise_cgen.py`

 * *Files identical despite different names*

### Comparing `arasea-3.0.6/arasea/tensor/extra_ops.py` & `arasea-3.0.7/arasea/tensor/extra_ops.py`

 * *Files identical despite different names*

### Comparing `arasea-3.0.6/arasea/tensor/fft.py` & `arasea-3.0.7/arasea/tensor/fft.py`

 * *Files identical despite different names*

### Comparing `arasea-3.0.6/arasea/tensor/fourier.py` & `arasea-3.0.7/arasea/tensor/fourier.py`

 * *Files identical despite different names*

### Comparing `arasea-3.0.6/arasea/tensor/inplace.py` & `arasea-3.0.7/arasea/tensor/inplace.py`

 * *Files identical despite different names*

### Comparing `arasea-3.0.6/arasea/tensor/io.py` & `arasea-3.0.7/arasea/tensor/io.py`

 * *Files identical despite different names*

### Comparing `arasea-3.0.6/arasea/tensor/math.py` & `arasea-3.0.7/arasea/tensor/math.py`

 * *Files identical despite different names*

### Comparing `arasea-3.0.6/arasea/tensor/nlinalg.py` & `arasea-3.0.7/arasea/tensor/nlinalg.py`

 * *Files identical despite different names*

### Comparing `arasea-3.0.6/arasea/tensor/nnet/__init__.py` & `arasea-3.0.7/arasea/tensor/nnet/__init__.py`

 * *Files identical despite different names*

### Comparing `arasea-3.0.6/arasea/tensor/nnet/abstract_conv.py` & `arasea-3.0.7/arasea/tensor/nnet/abstract_conv.py`

 * *Files identical despite different names*

### Comparing `arasea-3.0.6/arasea/tensor/nnet/basic.py` & `arasea-3.0.7/arasea/tensor/nnet/basic.py`

 * *Files identical despite different names*

### Comparing `arasea-3.0.6/arasea/tensor/nnet/batchnorm.py` & `arasea-3.0.7/arasea/tensor/nnet/batchnorm.py`

 * *Files identical despite different names*

### Comparing `arasea-3.0.6/arasea/tensor/nnet/blocksparse.py` & `arasea-3.0.7/arasea/tensor/nnet/blocksparse.py`

 * *Files identical despite different names*

### Comparing `arasea-3.0.6/arasea/tensor/nnet/conv.py` & `arasea-3.0.7/arasea/tensor/nnet/conv.py`

 * *Files identical despite different names*

### Comparing `arasea-3.0.6/arasea/tensor/nnet/conv3d2d.py` & `arasea-3.0.7/arasea/tensor/nnet/conv3d2d.py`

 * *Files identical despite different names*

### Comparing `arasea-3.0.6/arasea/tensor/nnet/corr.py` & `arasea-3.0.7/arasea/tensor/nnet/corr.py`

 * *Files identical despite different names*

### Comparing `arasea-3.0.6/arasea/tensor/nnet/corr3d.py` & `arasea-3.0.7/arasea/tensor/nnet/corr3d.py`

 * *Files identical despite different names*

### Comparing `arasea-3.0.6/arasea/tensor/nnet/ctc.py` & `arasea-3.0.7/arasea/tensor/nnet/ctc.py`

 * *Files identical despite different names*

### Comparing `arasea-3.0.6/arasea/tensor/nnet/neighbours.py` & `arasea-3.0.7/arasea/tensor/nnet/neighbours.py`

 * *Files identical despite different names*

### Comparing `arasea-3.0.6/arasea/tensor/nnet/rewriting.py` & `arasea-3.0.7/arasea/tensor/nnet/rewriting.py`

 * *Files identical despite different names*

### Comparing `arasea-3.0.6/arasea/tensor/nnet/sigm.py` & `arasea-3.0.7/arasea/tensor/nnet/sigm.py`

 * *Files identical despite different names*

### Comparing `arasea-3.0.6/arasea/tensor/random/basic.py` & `arasea-3.0.7/arasea/tensor/random/basic.py`

 * *Files identical despite different names*

### Comparing `arasea-3.0.6/arasea/tensor/random/op.py` & `arasea-3.0.7/arasea/tensor/random/op.py`

 * *Files identical despite different names*

### Comparing `arasea-3.0.6/arasea/tensor/random/rewriting/basic.py` & `arasea-3.0.7/arasea/tensor/random/rewriting/basic.py`

 * *Files identical despite different names*

### Comparing `arasea-3.0.6/arasea/tensor/random/rewriting/jax.py` & `arasea-3.0.7/arasea/tensor/random/rewriting/jax.py`

 * *Files identical despite different names*

### Comparing `arasea-3.0.6/arasea/tensor/random/type.py` & `arasea-3.0.7/arasea/tensor/random/type.py`

 * *Files identical despite different names*

### Comparing `arasea-3.0.6/arasea/tensor/random/utils.py` & `arasea-3.0.7/arasea/tensor/random/utils.py`

 * *Files identical despite different names*

### Comparing `arasea-3.0.6/arasea/tensor/random/var.py` & `arasea-3.0.7/arasea/tensor/random/var.py`

 * *Files identical despite different names*

### Comparing `arasea-3.0.6/arasea/tensor/rewriting/basic.py` & `arasea-3.0.7/arasea/tensor/rewriting/basic.py`

 * *Files identical despite different names*

### Comparing `arasea-3.0.6/arasea/tensor/rewriting/elemwise.py` & `arasea-3.0.7/arasea/tensor/rewriting/elemwise.py`

 * *Files identical despite different names*

### Comparing `arasea-3.0.6/arasea/tensor/rewriting/extra_ops.py` & `arasea-3.0.7/arasea/tensor/rewriting/extra_ops.py`

 * *Files identical despite different names*

### Comparing `arasea-3.0.6/arasea/tensor/rewriting/jax.py` & `arasea-3.0.7/arasea/tensor/rewriting/jax.py`

 * *Files identical despite different names*

### Comparing `arasea-3.0.6/arasea/tensor/rewriting/math.py` & `arasea-3.0.7/arasea/tensor/rewriting/math.py`

 * *Files identical despite different names*

### Comparing `arasea-3.0.6/arasea/tensor/rewriting/shape.py` & `arasea-3.0.7/arasea/tensor/rewriting/shape.py`

 * *Files identical despite different names*

### Comparing `arasea-3.0.6/arasea/tensor/rewriting/special.py` & `arasea-3.0.7/arasea/tensor/rewriting/special.py`

 * *Files identical despite different names*

### Comparing `arasea-3.0.6/arasea/tensor/rewriting/subtensor.py` & `arasea-3.0.7/arasea/tensor/rewriting/subtensor.py`

 * *Files identical despite different names*

### Comparing `arasea-3.0.6/arasea/tensor/rewriting/uncanonicalize.py` & `arasea-3.0.7/arasea/tensor/rewriting/uncanonicalize.py`

 * *Files identical despite different names*

### Comparing `arasea-3.0.6/arasea/tensor/shape.py` & `arasea-3.0.7/arasea/tensor/shape.py`

 * *Files identical despite different names*

### Comparing `arasea-3.0.6/arasea/tensor/sharedvar.py` & `arasea-3.0.7/arasea/tensor/sharedvar.py`

 * *Files identical despite different names*

### Comparing `arasea-3.0.6/arasea/tensor/signal/conv.py` & `arasea-3.0.7/arasea/tensor/signal/conv.py`

 * *Files identical despite different names*

### Comparing `arasea-3.0.6/arasea/tensor/signal/pool.py` & `arasea-3.0.7/arasea/tensor/signal/pool.py`

 * *Files identical despite different names*

### Comparing `arasea-3.0.6/arasea/tensor/slinalg.py` & `arasea-3.0.7/arasea/tensor/slinalg.py`

 * *Files identical despite different names*

### Comparing `arasea-3.0.6/arasea/tensor/sort.py` & `arasea-3.0.7/arasea/tensor/sort.py`

 * *Files identical despite different names*

### Comparing `arasea-3.0.6/arasea/tensor/special.py` & `arasea-3.0.7/arasea/tensor/special.py`

 * *Files identical despite different names*

### Comparing `arasea-3.0.6/arasea/tensor/subtensor.py` & `arasea-3.0.7/arasea/tensor/subtensor.py`

 * *Files identical despite different names*

### Comparing `arasea-3.0.6/arasea/tensor/type.py` & `arasea-3.0.7/arasea/tensor/type.py`

 * *Files identical despite different names*

### Comparing `arasea-3.0.6/arasea/tensor/type_other.py` & `arasea-3.0.7/arasea/tensor/type_other.py`

 * *Files identical despite different names*

### Comparing `arasea-3.0.6/arasea/tensor/utils.py` & `arasea-3.0.7/arasea/tensor/utils.py`

 * *Files identical despite different names*

### Comparing `arasea-3.0.6/arasea/tensor/var.py` & `arasea-3.0.7/arasea/tensor/var.py`

 * *Files identical despite different names*

### Comparing `arasea-3.0.6/arasea/tensor/xlogx.py` & `arasea-3.0.7/arasea/tensor/xlogx.py`

 * *Files identical despite different names*

### Comparing `arasea-3.0.6/arasea/typed_list/basic.py` & `arasea-3.0.7/arasea/typed_list/basic.py`

 * *Files identical despite different names*

### Comparing `arasea-3.0.6/arasea/typed_list/rewriting.py` & `arasea-3.0.7/arasea/typed_list/rewriting.py`

 * *Files identical despite different names*

### Comparing `arasea-3.0.6/arasea/typed_list/type.py` & `arasea-3.0.7/arasea/typed_list/type.py`

 * *Files identical despite different names*

### Comparing `arasea-3.0.6/arasea/updates.py` & `arasea-3.0.7/arasea/updates.py`

 * *Files identical despite different names*

### Comparing `arasea-3.0.6/arasea/utils.py` & `arasea-3.0.7/arasea/utils.py`

 * *Files identical despite different names*

### Comparing `arasea-3.0.6/arasea/version.py` & `arasea-3.0.7/arasea/version.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 try:
     #from arasea._version import __version__ as version
-    version = "3.0.6"
+    version = "3.0.7"
 except ImportError:
     raise RuntimeError(
         "Unable to find the version number that is generated when either building or "
         "installing from source. Please make sure that this Arasea has been properly "
         "installed, e.g. with\n\n  pip install -e .\n"
     )
```

### Comparing `arasea-3.0.6/arasea.egg-info/PKG-INFO` & `arasea-3.0.7/arasea.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: arasea
-Version: 3.0.6
+Version: 3.0.7
 Summary: A library for defining, optimizing, and efficiently evaluating mathematical expressions involving multi-dimensional arrays.
 Home-page: https://github.com/arasea-devs/arasea
 Author: arasea-devs
 Author-email: arasea.devs@gmail.com
 License: BSD-3-Clause
 Keywords: arasea,math,numerical,symbolic,blas,numpy,autodiff,differentiation
 Classifier: Development Status :: 6 - Mature
```

### Comparing `arasea-3.0.6/arasea.egg-info/SOURCES.txt` & `arasea-3.0.7/arasea.egg-info/SOURCES.txt`

 * *Files 1% similar despite different names*

```diff
@@ -105,15 +105,14 @@
 arasea/link/numba/dispatch/random.py
 arasea/link/numba/dispatch/scalar.py
 arasea/link/numba/dispatch/scan.py
 arasea/link/numba/dispatch/sparse.py
 arasea/link/numba/dispatch/tensor_basic.py
 arasea/misc/__init__.py
 arasea/misc/check_blas.py
-arasea/misc/check_blas_many.sh
 arasea/misc/check_duplicate_key.py
 arasea/misc/elemwise_openmp_speedup.py
 arasea/misc/elemwise_time_test.py
 arasea/misc/frozendict.py
 arasea/misc/latence_gpu_transfert.py
 arasea/misc/may_share_memory.py
 arasea/misc/ordered_set.py
```

### Comparing `arasea-3.0.6/tests/compile/function/test_function.py` & `arasea-3.0.7/tests/compile/function/test_function.py`

 * *Files identical despite different names*

### Comparing `arasea-3.0.6/tests/compile/function/test_pfunc.py` & `arasea-3.0.7/tests/compile/function/test_pfunc.py`

 * *Files identical despite different names*

### Comparing `arasea-3.0.6/tests/compile/function/test_types.py` & `arasea-3.0.7/tests/compile/function/test_types.py`

 * *Files identical despite different names*

### Comparing `arasea-3.0.6/tests/compile/test_builders.py` & `arasea-3.0.7/tests/compile/test_builders.py`

 * *Files identical despite different names*

### Comparing `arasea-3.0.6/tests/compile/test_compilelock.py` & `arasea-3.0.7/tests/compile/test_compilelock.py`

 * *Files identical despite different names*

### Comparing `arasea-3.0.6/tests/compile/test_debugmode.py` & `arasea-3.0.7/tests/compile/test_debugmode.py`

 * *Files identical despite different names*

### Comparing `arasea-3.0.6/tests/compile/test_misc.py` & `arasea-3.0.7/tests/compile/test_misc.py`

 * *Files identical despite different names*

### Comparing `arasea-3.0.6/tests/compile/test_mode.py` & `arasea-3.0.7/tests/compile/test_mode.py`

 * *Files identical despite different names*

### Comparing `arasea-3.0.6/tests/compile/test_monitormode.py` & `arasea-3.0.7/tests/compile/test_monitormode.py`

 * *Files identical despite different names*

### Comparing `arasea-3.0.6/tests/compile/test_nanguardmode.py` & `arasea-3.0.7/tests/compile/test_nanguardmode.py`

 * *Files identical despite different names*

### Comparing `arasea-3.0.6/tests/compile/test_ops.py` & `arasea-3.0.7/tests/compile/test_ops.py`

 * *Files identical despite different names*

### Comparing `arasea-3.0.6/tests/compile/test_profiling.py` & `arasea-3.0.7/tests/compile/test_profiling.py`

 * *Files identical despite different names*

### Comparing `arasea-3.0.6/tests/compile/test_shared.py` & `arasea-3.0.7/tests/compile/test_shared.py`

 * *Files identical despite different names*

### Comparing `arasea-3.0.6/tests/d3viz/models.py` & `arasea-3.0.7/tests/d3viz/models.py`

 * *Files identical despite different names*

### Comparing `arasea-3.0.6/tests/d3viz/test_d3viz.py` & `arasea-3.0.7/tests/d3viz/test_d3viz.py`

 * *Files identical despite different names*

### Comparing `arasea-3.0.6/tests/d3viz/test_formatting.py` & `arasea-3.0.7/tests/d3viz/test_formatting.py`

 * *Files identical despite different names*

### Comparing `arasea-3.0.6/tests/graph/rewriting/test_basic.py` & `arasea-3.0.7/tests/graph/rewriting/test_basic.py`

 * *Files identical despite different names*

### Comparing `arasea-3.0.6/tests/graph/rewriting/test_db.py` & `arasea-3.0.7/tests/graph/rewriting/test_db.py`

 * *Files identical despite different names*

### Comparing `arasea-3.0.6/tests/graph/rewriting/test_kanren.py` & `arasea-3.0.7/tests/graph/rewriting/test_kanren.py`

 * *Files identical despite different names*

### Comparing `arasea-3.0.6/tests/graph/rewriting/test_unify.py` & `arasea-3.0.7/tests/graph/rewriting/test_unify.py`

 * *Files identical despite different names*

### Comparing `arasea-3.0.6/tests/graph/rewriting/test_utils.py` & `arasea-3.0.7/tests/graph/rewriting/test_utils.py`

 * *Files identical despite different names*

### Comparing `arasea-3.0.6/tests/graph/test_basic.py` & `arasea-3.0.7/tests/graph/test_basic.py`

 * *Files identical despite different names*

### Comparing `arasea-3.0.6/tests/graph/test_compute_test_value.py` & `arasea-3.0.7/tests/graph/test_compute_test_value.py`

 * *Files identical despite different names*

### Comparing `arasea-3.0.6/tests/graph/test_destroyhandler.py` & `arasea-3.0.7/tests/graph/test_destroyhandler.py`

 * *Files identical despite different names*

### Comparing `arasea-3.0.6/tests/graph/test_features.py` & `arasea-3.0.7/tests/graph/test_features.py`

 * *Files identical despite different names*

### Comparing `arasea-3.0.6/tests/graph/test_fg.py` & `arasea-3.0.7/tests/graph/test_fg.py`

 * *Files identical despite different names*

### Comparing `arasea-3.0.6/tests/graph/test_op.py` & `arasea-3.0.7/tests/graph/test_op.py`

 * *Files identical despite different names*

### Comparing `arasea-3.0.6/tests/graph/test_sched.py` & `arasea-3.0.7/tests/graph/test_sched.py`

 * *Files identical despite different names*

### Comparing `arasea-3.0.6/tests/graph/test_types.py` & `arasea-3.0.7/tests/graph/test_types.py`

 * *Files identical despite different names*

### Comparing `arasea-3.0.6/tests/graph/utils.py` & `arasea-3.0.7/tests/graph/utils.py`

 * *Files identical despite different names*

### Comparing `arasea-3.0.6/tests/link/c/test_basic.py` & `arasea-3.0.7/tests/link/c/test_basic.py`

 * *Files identical despite different names*

### Comparing `arasea-3.0.6/tests/link/c/test_cmodule.py` & `arasea-3.0.7/tests/link/c/test_cmodule.py`

 * *Files identical despite different names*

### Comparing `arasea-3.0.6/tests/link/c/test_op.py` & `arasea-3.0.7/tests/link/c/test_op.py`

 * *Files identical despite different names*

### Comparing `arasea-3.0.6/tests/link/c/test_params_type.py` & `arasea-3.0.7/tests/link/c/test_params_type.py`

 * *Files identical despite different names*

### Comparing `arasea-3.0.6/tests/link/c/test_type.py` & `arasea-3.0.7/tests/link/c/test_type.py`

 * *Files identical despite different names*

### Comparing `arasea-3.0.6/tests/link/numba/test_basic.py` & `arasea-3.0.7/tests/link/numba/test_basic.py`

 * *Files identical despite different names*

### Comparing `arasea-3.0.6/tests/link/numba/test_elemwise.py` & `arasea-3.0.7/tests/link/numba/test_elemwise.py`

 * *Files identical despite different names*

### Comparing `arasea-3.0.6/tests/link/numba/test_extra_ops.py` & `arasea-3.0.7/tests/link/numba/test_extra_ops.py`

 * *Files identical despite different names*

### Comparing `arasea-3.0.6/tests/link/numba/test_nlinalg.py` & `arasea-3.0.7/tests/link/numba/test_nlinalg.py`

 * *Files identical despite different names*

### Comparing `arasea-3.0.6/tests/link/numba/test_performance.py` & `arasea-3.0.7/tests/link/numba/test_performance.py`

 * *Files identical despite different names*

### Comparing `arasea-3.0.6/tests/link/numba/test_random.py` & `arasea-3.0.7/tests/link/numba/test_random.py`

 * *Files identical despite different names*

### Comparing `arasea-3.0.6/tests/link/numba/test_scalar.py` & `arasea-3.0.7/tests/link/numba/test_scalar.py`

 * *Files identical despite different names*

### Comparing `arasea-3.0.6/tests/link/numba/test_scan.py` & `arasea-3.0.7/tests/link/numba/test_scan.py`

 * *Files identical despite different names*

### Comparing `arasea-3.0.6/tests/link/numba/test_sparse.py` & `arasea-3.0.7/tests/link/numba/test_sparse.py`

 * *Files identical despite different names*

### Comparing `arasea-3.0.6/tests/link/numba/test_tensor_basic.py` & `arasea-3.0.7/tests/link/numba/test_tensor_basic.py`

 * *Files identical despite different names*

### Comparing `arasea-3.0.6/tests/link/test_link.py` & `arasea-3.0.7/tests/link/test_link.py`

 * *Files identical despite different names*

### Comparing `arasea-3.0.6/tests/link/test_utils.py` & `arasea-3.0.7/tests/link/test_utils.py`

 * *Files identical despite different names*

### Comparing `arasea-3.0.6/tests/link/test_vm.py` & `arasea-3.0.7/tests/link/test_vm.py`

 * *Files identical despite different names*

### Comparing `arasea-3.0.6/tests/misc/test_may_share_memory.py` & `arasea-3.0.7/tests/misc/test_may_share_memory.py`

 * *Files identical despite different names*

### Comparing `arasea-3.0.6/tests/misc/test_pkl_utils.py` & `arasea-3.0.7/tests/misc/test_pkl_utils.py`

 * *Files identical despite different names*

### Comparing `arasea-3.0.6/tests/sandbox/linalg/test_linalg.py` & `arasea-3.0.7/tests/sandbox/linalg/test_linalg.py`

 * *Files identical despite different names*

### Comparing `arasea-3.0.6/tests/sandbox/test_minimal.py` & `arasea-3.0.7/tests/sandbox/test_minimal.py`

 * *Files identical despite different names*

### Comparing `arasea-3.0.6/tests/sandbox/test_multinomial.py` & `arasea-3.0.7/tests/sandbox/test_multinomial.py`

 * *Files identical despite different names*

### Comparing `arasea-3.0.6/tests/sandbox/test_multinomial_wo_replacement.py` & `arasea-3.0.7/tests/sandbox/test_multinomial_wo_replacement.py`

 * *Files identical despite different names*

### Comparing `arasea-3.0.6/tests/sandbox/test_rng_mrg.py` & `arasea-3.0.7/tests/sandbox/test_rng_mrg.py`

 * *Files identical despite different names*

### Comparing `arasea-3.0.6/tests/scalar/test_basic.py` & `arasea-3.0.7/tests/scalar/test_basic.py`

 * *Files identical despite different names*

### Comparing `arasea-3.0.6/tests/scalar/test_basic_sympy.py` & `arasea-3.0.7/tests/scalar/test_basic_sympy.py`

 * *Files identical despite different names*

### Comparing `arasea-3.0.6/tests/scalar/test_math.py` & `arasea-3.0.7/tests/scalar/test_math.py`

 * *Files identical despite different names*

### Comparing `arasea-3.0.6/tests/scalar/test_type.py` & `arasea-3.0.7/tests/scalar/test_type.py`

 * *Files identical despite different names*

### Comparing `arasea-3.0.6/tests/scan/test_basic.py` & `arasea-3.0.7/tests/scan/test_basic.py`

 * *Files identical despite different names*

### Comparing `arasea-3.0.6/tests/scan/test_checkpoints.py` & `arasea-3.0.7/tests/scan/test_checkpoints.py`

 * *Files identical despite different names*

### Comparing `arasea-3.0.6/tests/scan/test_printing.py` & `arasea-3.0.7/tests/scan/test_printing.py`

 * *Files identical despite different names*

### Comparing `arasea-3.0.6/tests/scan/test_rewriting.py` & `arasea-3.0.7/tests/scan/test_rewriting.py`

 * *Files identical despite different names*

### Comparing `arasea-3.0.6/tests/scan/test_utils.py` & `arasea-3.0.7/tests/scan/test_utils.py`

 * *Files identical despite different names*

### Comparing `arasea-3.0.6/tests/scan/test_views.py` & `arasea-3.0.7/tests/scan/test_views.py`

 * *Files identical despite different names*

### Comparing `arasea-3.0.6/tests/sparse/sandbox/test_sp.py` & `arasea-3.0.7/tests/sparse/sandbox/test_sp.py`

 * *Files identical despite different names*

### Comparing `arasea-3.0.6/tests/sparse/test_basic.py` & `arasea-3.0.7/tests/sparse/test_basic.py`

 * *Files identical despite different names*

### Comparing `arasea-3.0.6/tests/sparse/test_rewriting.py` & `arasea-3.0.7/tests/sparse/test_rewriting.py`

 * *Files identical despite different names*

### Comparing `arasea-3.0.6/tests/sparse/test_sp2.py` & `arasea-3.0.7/tests/sparse/test_sp2.py`

 * *Files identical despite different names*

### Comparing `arasea-3.0.6/tests/sparse/test_type.py` & `arasea-3.0.7/tests/sparse/test_type.py`

 * *Files identical despite different names*

### Comparing `arasea-3.0.6/tests/sparse/test_utils.py` & `arasea-3.0.7/tests/sparse/test_utils.py`

 * *Files identical despite different names*

### Comparing `arasea-3.0.6/tests/sparse/test_var.py` & `arasea-3.0.7/tests/sparse/test_var.py`

 * *Files identical despite different names*

### Comparing `arasea-3.0.6/tests/tensor/_test_mpi_roundtrip.py` & `arasea-3.0.7/tests/tensor/_test_mpi_roundtrip.py`

 * *Files identical despite different names*

### Comparing `arasea-3.0.6/tests/tensor/nnet/speed_test_conv.py` & `arasea-3.0.7/tests/tensor/nnet/speed_test_conv.py`

 * *Files identical despite different names*

### Comparing `arasea-3.0.6/tests/tensor/nnet/test_abstract_conv.py` & `arasea-3.0.7/tests/tensor/nnet/test_abstract_conv.py`

 * *Files identical despite different names*

### Comparing `arasea-3.0.6/tests/tensor/nnet/test_basic.py` & `arasea-3.0.7/tests/tensor/nnet/test_basic.py`

 * *Files identical despite different names*

### Comparing `arasea-3.0.6/tests/tensor/nnet/test_batchnorm.py` & `arasea-3.0.7/tests/tensor/nnet/test_batchnorm.py`

 * *Files identical despite different names*

### Comparing `arasea-3.0.6/tests/tensor/nnet/test_blocksparse.py` & `arasea-3.0.7/tests/tensor/nnet/test_blocksparse.py`

 * *Files identical despite different names*

### Comparing `arasea-3.0.6/tests/tensor/nnet/test_conv.py` & `arasea-3.0.7/tests/tensor/nnet/test_conv.py`

 * *Files identical despite different names*

### Comparing `arasea-3.0.6/tests/tensor/nnet/test_conv3d2d.py` & `arasea-3.0.7/tests/tensor/nnet/test_conv3d2d.py`

 * *Files identical despite different names*

### Comparing `arasea-3.0.6/tests/tensor/nnet/test_corr.py` & `arasea-3.0.7/tests/tensor/nnet/test_corr.py`

 * *Files identical despite different names*

### Comparing `arasea-3.0.6/tests/tensor/nnet/test_corr3d.py` & `arasea-3.0.7/tests/tensor/nnet/test_corr3d.py`

 * *Files identical despite different names*

### Comparing `arasea-3.0.6/tests/tensor/nnet/test_ctc.py` & `arasea-3.0.7/tests/tensor/nnet/test_ctc.py`

 * *Files identical despite different names*

### Comparing `arasea-3.0.6/tests/tensor/nnet/test_neighbours.py` & `arasea-3.0.7/tests/tensor/nnet/test_neighbours.py`

 * *Files identical despite different names*

### Comparing `arasea-3.0.6/tests/tensor/nnet/test_rewriting.py` & `arasea-3.0.7/tests/tensor/nnet/test_rewriting.py`

 * *Files identical despite different names*

### Comparing `arasea-3.0.6/tests/tensor/nnet/test_sigm.py` & `arasea-3.0.7/tests/tensor/nnet/test_sigm.py`

 * *Files identical despite different names*

### Comparing `arasea-3.0.6/tests/tensor/random/test_basic.py` & `arasea-3.0.7/tests/tensor/random/test_basic.py`

 * *Files identical despite different names*

### Comparing `arasea-3.0.6/tests/tensor/random/test_op.py` & `arasea-3.0.7/tests/tensor/random/test_op.py`

 * *Files identical despite different names*

### Comparing `arasea-3.0.6/tests/tensor/random/test_rewriting.py` & `arasea-3.0.7/tests/tensor/random/test_rewriting.py`

 * *Files identical despite different names*

### Comparing `arasea-3.0.6/tests/tensor/random/test_type.py` & `arasea-3.0.7/tests/tensor/random/test_type.py`

 * *Files identical despite different names*

### Comparing `arasea-3.0.6/tests/tensor/random/test_utils.py` & `arasea-3.0.7/tests/tensor/random/test_utils.py`

 * *Files identical despite different names*

### Comparing `arasea-3.0.6/tests/tensor/random/test_var.py` & `arasea-3.0.7/tests/tensor/random/test_var.py`

 * *Files identical despite different names*

### Comparing `arasea-3.0.6/tests/tensor/rewriting/test_basic.py` & `arasea-3.0.7/tests/tensor/rewriting/test_basic.py`

 * *Files identical despite different names*

### Comparing `arasea-3.0.6/tests/tensor/rewriting/test_elemwise.py` & `arasea-3.0.7/tests/tensor/rewriting/test_elemwise.py`

 * *Files identical despite different names*

### Comparing `arasea-3.0.6/tests/tensor/rewriting/test_extra_ops.py` & `arasea-3.0.7/tests/tensor/rewriting/test_extra_ops.py`

 * *Files identical despite different names*

### Comparing `arasea-3.0.6/tests/tensor/rewriting/test_math.py` & `arasea-3.0.7/tests/tensor/rewriting/test_math.py`

 * *Files identical despite different names*

### Comparing `arasea-3.0.6/tests/tensor/rewriting/test_shape.py` & `arasea-3.0.7/tests/tensor/rewriting/test_shape.py`

 * *Files identical despite different names*

### Comparing `arasea-3.0.6/tests/tensor/rewriting/test_special.py` & `arasea-3.0.7/tests/tensor/rewriting/test_special.py`

 * *Files identical despite different names*

### Comparing `arasea-3.0.6/tests/tensor/rewriting/test_subtensor.py` & `arasea-3.0.7/tests/tensor/rewriting/test_subtensor.py`

 * *Files identical despite different names*

### Comparing `arasea-3.0.6/tests/tensor/rewriting/test_uncanonicalize.py` & `arasea-3.0.7/tests/tensor/rewriting/test_uncanonicalize.py`

 * *Files identical despite different names*

### Comparing `arasea-3.0.6/tests/tensor/signal/test_conv.py` & `arasea-3.0.7/tests/tensor/signal/test_conv.py`

 * *Files identical despite different names*

### Comparing `arasea-3.0.6/tests/tensor/signal/test_pool.py` & `arasea-3.0.7/tests/tensor/signal/test_pool.py`

 * *Files identical despite different names*

### Comparing `arasea-3.0.6/tests/tensor/test_basic.py` & `arasea-3.0.7/tests/tensor/test_basic.py`

 * *Files identical despite different names*

### Comparing `arasea-3.0.6/tests/tensor/test_blas.py` & `arasea-3.0.7/tests/tensor/test_blas.py`

 * *Files identical despite different names*

### Comparing `arasea-3.0.6/tests/tensor/test_blas_c.py` & `arasea-3.0.7/tests/tensor/test_blas_c.py`

 * *Files identical despite different names*

### Comparing `arasea-3.0.6/tests/tensor/test_blas_scipy.py` & `arasea-3.0.7/tests/tensor/test_blas_scipy.py`

 * *Files identical despite different names*

### Comparing `arasea-3.0.6/tests/tensor/test_casting.py` & `arasea-3.0.7/tests/tensor/test_casting.py`

 * *Files identical despite different names*

### Comparing `arasea-3.0.6/tests/tensor/test_complex.py` & `arasea-3.0.7/tests/tensor/test_complex.py`

 * *Files identical despite different names*

### Comparing `arasea-3.0.6/tests/tensor/test_elemwise.py` & `arasea-3.0.7/tests/tensor/test_elemwise.py`

 * *Files identical despite different names*

### Comparing `arasea-3.0.6/tests/tensor/test_extra_ops.py` & `arasea-3.0.7/tests/tensor/test_extra_ops.py`

 * *Files identical despite different names*

### Comparing `arasea-3.0.6/tests/tensor/test_fft.py` & `arasea-3.0.7/tests/tensor/test_fft.py`

 * *Files identical despite different names*

### Comparing `arasea-3.0.6/tests/tensor/test_fourier.py` & `arasea-3.0.7/tests/tensor/test_fourier.py`

 * *Files identical despite different names*

### Comparing `arasea-3.0.6/tests/tensor/test_gc.py` & `arasea-3.0.7/tests/tensor/test_gc.py`

 * *Files identical despite different names*

### Comparing `arasea-3.0.6/tests/tensor/test_inplace.py` & `arasea-3.0.7/tests/tensor/test_inplace.py`

 * *Files identical despite different names*

### Comparing `arasea-3.0.6/tests/tensor/test_io.py` & `arasea-3.0.7/tests/tensor/test_io.py`

 * *Files identical despite different names*

### Comparing `arasea-3.0.6/tests/tensor/test_keepdims.py` & `arasea-3.0.7/tests/tensor/test_keepdims.py`

 * *Files identical despite different names*

### Comparing `arasea-3.0.6/tests/tensor/test_math.py` & `arasea-3.0.7/tests/tensor/test_math.py`

 * *Files identical despite different names*

### Comparing `arasea-3.0.6/tests/tensor/test_math_scipy.py` & `arasea-3.0.7/tests/tensor/test_math_scipy.py`

 * *Files identical despite different names*

### Comparing `arasea-3.0.6/tests/tensor/test_merge.py` & `arasea-3.0.7/tests/tensor/test_merge.py`

 * *Files identical despite different names*

### Comparing `arasea-3.0.6/tests/tensor/test_misc.py` & `arasea-3.0.7/tests/tensor/test_misc.py`

 * *Files identical despite different names*

### Comparing `arasea-3.0.6/tests/tensor/test_mpi.py` & `arasea-3.0.7/tests/tensor/test_mpi.py`

 * *Files identical despite different names*

### Comparing `arasea-3.0.6/tests/tensor/test_nlinalg.py` & `arasea-3.0.7/tests/tensor/test_nlinalg.py`

 * *Files identical despite different names*

### Comparing `arasea-3.0.6/tests/tensor/test_shape.py` & `arasea-3.0.7/tests/tensor/test_shape.py`

 * *Files identical despite different names*

### Comparing `arasea-3.0.6/tests/tensor/test_sharedvar.py` & `arasea-3.0.7/tests/tensor/test_sharedvar.py`

 * *Files identical despite different names*

### Comparing `arasea-3.0.6/tests/tensor/test_slinalg.py` & `arasea-3.0.7/tests/tensor/test_slinalg.py`

 * *Files identical despite different names*

### Comparing `arasea-3.0.6/tests/tensor/test_sort.py` & `arasea-3.0.7/tests/tensor/test_sort.py`

 * *Files identical despite different names*

### Comparing `arasea-3.0.6/tests/tensor/test_special.py` & `arasea-3.0.7/tests/tensor/test_special.py`

 * *Files identical despite different names*

### Comparing `arasea-3.0.6/tests/tensor/test_subtensor.py` & `arasea-3.0.7/tests/tensor/test_subtensor.py`

 * *Files identical despite different names*

### Comparing `arasea-3.0.6/tests/tensor/test_type.py` & `arasea-3.0.7/tests/tensor/test_type.py`

 * *Files identical despite different names*

### Comparing `arasea-3.0.6/tests/tensor/test_type_other.py` & `arasea-3.0.7/tests/tensor/test_type_other.py`

 * *Files identical despite different names*

### Comparing `arasea-3.0.6/tests/tensor/test_utils.py` & `arasea-3.0.7/tests/tensor/test_utils.py`

 * *Files identical despite different names*

### Comparing `arasea-3.0.6/tests/tensor/test_var.py` & `arasea-3.0.7/tests/tensor/test_var.py`

 * *Files identical despite different names*

### Comparing `arasea-3.0.6/tests/tensor/test_xlogx.py` & `arasea-3.0.7/tests/tensor/test_xlogx.py`

 * *Files identical despite different names*

### Comparing `arasea-3.0.6/tests/tensor/utils.py` & `arasea-3.0.7/tests/tensor/utils.py`

 * *Files identical despite different names*

### Comparing `arasea-3.0.6/tests/test_breakpoint.py` & `arasea-3.0.7/tests/test_breakpoint.py`

 * *Files identical despite different names*

### Comparing `arasea-3.0.6/tests/test_config.py` & `arasea-3.0.7/tests/test_config.py`

 * *Files identical despite different names*

### Comparing `arasea-3.0.6/tests/test_gradient.py` & `arasea-3.0.7/tests/test_gradient.py`

 * *Files identical despite different names*

### Comparing `arasea-3.0.6/tests/test_ifelse.py` & `arasea-3.0.7/tests/test_ifelse.py`

 * *Files identical despite different names*

### Comparing `arasea-3.0.6/tests/test_printing.py` & `arasea-3.0.7/tests/test_printing.py`

 * *Files identical despite different names*

### Comparing `arasea-3.0.6/tests/test_raise_op.py` & `arasea-3.0.7/tests/test_raise_op.py`

 * *Files identical despite different names*

### Comparing `arasea-3.0.6/tests/test_rop.py` & `arasea-3.0.7/tests/test_rop.py`

 * *Files identical despite different names*

### Comparing `arasea-3.0.6/tests/test_updates.py` & `arasea-3.0.7/tests/test_updates.py`

 * *Files identical despite different names*

### Comparing `arasea-3.0.6/tests/typed_list/test_basic.py` & `arasea-3.0.7/tests/typed_list/test_basic.py`

 * *Files identical despite different names*

### Comparing `arasea-3.0.6/tests/typed_list/test_rewriting.py` & `arasea-3.0.7/tests/typed_list/test_rewriting.py`

 * *Files identical despite different names*

### Comparing `arasea-3.0.6/tests/typed_list/test_type.py` & `arasea-3.0.7/tests/typed_list/test_type.py`

 * *Files identical despite different names*

### Comparing `arasea-3.0.6/tests/unittest_tools.py` & `arasea-3.0.7/tests/unittest_tools.py`

 * *Files identical despite different names*

