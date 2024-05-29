# Comparing `tmp/seqslab-cli-3.3.3.tar.gz` & `tmp/seqslab-cli-3.3.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "seqslab-cli-3.3.3.tar", last modified: Mon May 20 10:11:24 2024, max compression
+gzip compressed data, was "seqslab-cli-3.3.4.tar", last modified: Wed May 29 06:58:29 2024, max compression
```

## Comparing `seqslab-cli-3.3.3.tar` & `seqslab-cli-3.3.4.tar`

### file list

```diff
@@ -1,143 +1,143 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-20 10:11:24.463486 seqslab-cli-3.3.3/
--rw-r--r--   0 runner    (1001) docker     (127)      689 2024-05-20 10:11:10.000000 seqslab-cli-3.3.3/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)       44 2024-05-20 10:11:10.000000 seqslab-cli-3.3.3/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (127)     6565 2024-05-20 10:11:24.463486 seqslab-cli-3.3.3/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     4631 2024-05-20 10:11:10.000000 seqslab-cli-3.3.3/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-20 10:11:24.447486 seqslab-cli-3.3.3/python/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-20 10:11:24.447486 seqslab-cli-3.3.3/python/seqslab/
--rw-r--r--   0 runner    (1001) docker     (127)      779 2024-05-20 10:11:10.000000 seqslab-cli-3.3.3/python/seqslab/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-20 10:11:24.451486 seqslab-cli-3.3.3/python/seqslab/auth/
--rw-r--r--   0 runner    (1001) docker     (127)       79 2024-05-20 10:11:10.000000 seqslab-cli-3.3.3/python/seqslab/auth/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     4545 2024-05-20 10:11:10.000000 seqslab-cli-3.3.3/python/seqslab/auth/azuread.py
--rw-r--r--   0 runner    (1001) docker     (127)    14598 2024-05-20 10:11:10.000000 seqslab-cli-3.3.3/python/seqslab/auth/commands.py
--rw-r--r--   0 runner    (1001) docker     (127)     1678 2024-05-20 10:11:10.000000 seqslab-cli-3.3.3/python/seqslab/cli.py
--rw-r--r--   0 runner    (1001) docker     (127)      694 2024-05-20 10:11:10.000000 seqslab-cli-3.3.3/python/seqslab/context.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-20 10:11:24.451486 seqslab-cli-3.3.3/python/seqslab/drs/
--rw-r--r--   0 runner    (1001) docker     (127)      226 2024-05-20 10:11:10.000000 seqslab-cli-3.3.3/python/seqslab/drs/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-20 10:11:24.451486 seqslab-cli-3.3.3/python/seqslab/drs/api/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-20 10:11:10.000000 seqslab-cli-3.3.3/python/seqslab/drs/api/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    16095 2024-05-20 10:11:10.000000 seqslab-cli-3.3.3/python/seqslab/drs/api/azure.py
--rw-r--r--   0 runner    (1001) docker     (127)    17051 2024-05-20 10:11:10.000000 seqslab-cli-3.3.3/python/seqslab/drs/api/base.py
--rw-r--r--   0 runner    (1001) docker     (127)     1354 2024-05-20 10:11:10.000000 seqslab-cli-3.3.3/python/seqslab/drs/api/common.py
--rw-r--r--   0 runner    (1001) docker     (127)     5415 2024-05-20 10:11:10.000000 seqslab-cli-3.3.3/python/seqslab/drs/api/template.py
--rw-r--r--   0 runner    (1001) docker     (127)    49945 2024-05-20 10:11:10.000000 seqslab-cli-3.3.3/python/seqslab/drs/commands.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-20 10:11:24.451486 seqslab-cli-3.3.3/python/seqslab/drs/internal/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-20 10:11:10.000000 seqslab-cli-3.3.3/python/seqslab/drs/internal/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    21876 2024-05-20 10:11:10.000000 seqslab-cli-3.3.3/python/seqslab/drs/internal/aiocopy.py
--rw-r--r--   0 runner    (1001) docker     (127)     1343 2024-05-20 10:11:10.000000 seqslab-cli-3.3.3/python/seqslab/drs/internal/common.py
--rw-r--r--   0 runner    (1001) docker     (127)     4487 2024-05-20 10:11:10.000000 seqslab-cli-3.3.3/python/seqslab/drs/internal/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-20 10:11:24.451486 seqslab-cli-3.3.3/python/seqslab/drs/storage/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-20 10:11:10.000000 seqslab-cli-3.3.3/python/seqslab/drs/storage/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    28712 2024-05-20 10:11:10.000000 seqslab-cli-3.3.3/python/seqslab/drs/storage/azure.py
--rw-r--r--   0 runner    (1001) docker     (127)    12704 2024-05-20 10:11:10.000000 seqslab-cli-3.3.3/python/seqslab/drs/storage/base.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-20 10:11:24.451486 seqslab-cli-3.3.3/python/seqslab/drs/utils/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-20 10:11:10.000000 seqslab-cli-3.3.3/python/seqslab/drs/utils/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     5815 2024-05-20 10:11:10.000000 seqslab-cli-3.3.3/python/seqslab/drs/utils/atgxmetadata.py
--rw-r--r--   0 runner    (1001) docker     (127)     2093 2024-05-20 10:11:10.000000 seqslab-cli-3.3.3/python/seqslab/drs/utils/biomimetype.py
--rw-r--r--   0 runner    (1001) docker     (127)     3175 2024-05-20 10:11:10.000000 seqslab-cli-3.3.3/python/seqslab/drs/utils/progressbar.py
--rw-r--r--   0 runner    (1001) docker     (127)     2305 2024-05-20 10:11:10.000000 seqslab-cli-3.3.3/python/seqslab/exceptions.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-20 10:11:24.451486 seqslab-cli-3.3.3/python/seqslab/organization/
--rw-r--r--   0 runner    (1001) docker     (127)      261 2024-05-20 10:11:10.000000 seqslab-cli-3.3.3/python/seqslab/organization/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2354 2024-05-20 10:11:10.000000 seqslab-cli-3.3.3/python/seqslab/organization/commands.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-20 10:11:24.451486 seqslab-cli-3.3.3/python/seqslab/organization/resource/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-20 10:11:10.000000 seqslab-cli-3.3.3/python/seqslab/organization/resource/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1221 2024-05-20 10:11:10.000000 seqslab-cli-3.3.3/python/seqslab/organization/resource/base.py
--rw-r--r--   0 runner    (1001) docker     (127)     5144 2024-05-20 10:11:10.000000 seqslab-cli-3.3.3/python/seqslab/plugin.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-20 10:11:24.451486 seqslab-cli-3.3.3/python/seqslab/role/
--rw-r--r--   0 runner    (1001) docker     (127)      228 2024-05-20 10:11:10.000000 seqslab-cli-3.3.3/python/seqslab/role/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1274 2024-05-20 10:11:10.000000 seqslab-cli-3.3.3/python/seqslab/role/commands.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-20 10:11:24.455486 seqslab-cli-3.3.3/python/seqslab/role/internal/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-20 10:11:10.000000 seqslab-cli-3.3.3/python/seqslab/role/internal/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1342 2024-05-20 10:11:10.000000 seqslab-cli-3.3.3/python/seqslab/role/internal/common.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-20 10:11:24.455486 seqslab-cli-3.3.3/python/seqslab/role/resource/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-20 10:11:10.000000 seqslab-cli-3.3.3/python/seqslab/role/resource/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      865 2024-05-20 10:11:10.000000 seqslab-cli-3.3.3/python/seqslab/role/resource/azure.py
--rw-r--r--   0 runner    (1001) docker     (127)     1354 2024-05-20 10:11:10.000000 seqslab-cli-3.3.3/python/seqslab/role/resource/base.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-20 10:11:24.455486 seqslab-cli-3.3.3/python/seqslab/runsheet/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-20 10:11:10.000000 seqslab-cli-3.3.3/python/seqslab/runsheet/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     6374 2024-05-20 10:11:10.000000 seqslab-cli-3.3.3/python/seqslab/runsheet/runsheet.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-20 10:11:24.455486 seqslab-cli-3.3.3/python/seqslab/sample_sheet/
--rw-r--r--   0 runner    (1001) docker     (127)    56711 2024-05-20 10:11:11.000000 seqslab-cli-3.3.3/python/seqslab/sample_sheet/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)       22 2024-05-20 10:11:11.000000 seqslab-cli-3.3.3/python/seqslab/sample_sheet/_version.py
--rw-r--r--   0 runner    (1001) docker     (127)      630 2024-05-20 10:11:11.000000 seqslab-cli-3.3.3/python/seqslab/sample_sheet/util.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-20 10:11:24.455486 seqslab-cli-3.3.3/python/seqslab/scr/
--rw-r--r--   0 runner    (1001) docker     (127)      226 2024-05-20 10:11:10.000000 seqslab-cli-3.3.3/python/seqslab/scr/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     6253 2024-05-20 10:11:10.000000 seqslab-cli-3.3.3/python/seqslab/scr/commands.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-20 10:11:24.455486 seqslab-cli-3.3.3/python/seqslab/scr/internal/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-20 10:11:10.000000 seqslab-cli-3.3.3/python/seqslab/scr/internal/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1342 2024-05-20 10:11:10.000000 seqslab-cli-3.3.3/python/seqslab/scr/internal/common.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-20 10:11:24.455486 seqslab-cli-3.3.3/python/seqslab/scr/resource/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-20 10:11:10.000000 seqslab-cli-3.3.3/python/seqslab/scr/resource/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      865 2024-05-20 10:11:10.000000 seqslab-cli-3.3.3/python/seqslab/scr/resource/azure.py
--rw-r--r--   0 runner    (1001) docker     (127)     4698 2024-05-20 10:11:10.000000 seqslab-cli-3.3.3/python/seqslab/scr/resource/base.py
--rw-r--r--   0 runner    (1001) docker     (127)      452 2024-05-20 10:11:10.000000 seqslab-cli-3.3.3/python/seqslab/session_logger.py
--rw-r--r--   0 runner    (1001) docker     (127)      895 2024-05-20 10:11:10.000000 seqslab-cli-3.3.3/python/seqslab/settings.py
--rw-r--r--   0 runner    (1001) docker     (127)     1370 2024-05-20 10:11:10.000000 seqslab-cli-3.3.3/python/seqslab/statusbar.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-20 10:11:24.455486 seqslab-cli-3.3.3/python/seqslab/trs/
--rw-r--r--   0 runner    (1001) docker     (127)      226 2024-05-20 10:11:10.000000 seqslab-cli-3.3.3/python/seqslab/trs/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    23164 2024-05-20 10:11:10.000000 seqslab-cli-3.3.3/python/seqslab/trs/commands.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-20 10:11:24.455486 seqslab-cli-3.3.3/python/seqslab/trs/internal/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-20 10:11:10.000000 seqslab-cli-3.3.3/python/seqslab/trs/internal/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1685 2024-05-20 10:11:10.000000 seqslab-cli-3.3.3/python/seqslab/trs/internal/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-20 10:11:24.455486 seqslab-cli-3.3.3/python/seqslab/trs/register/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-20 10:11:10.000000 seqslab-cli-3.3.3/python/seqslab/trs/register/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      999 2024-05-20 10:11:10.000000 seqslab-cli-3.3.3/python/seqslab/trs/register/azure.py
--rw-r--r--   0 runner    (1001) docker     (127)    10958 2024-05-20 10:11:10.000000 seqslab-cli-3.3.3/python/seqslab/trs/register/base.py
--rw-r--r--   0 runner    (1001) docker     (127)     1338 2024-05-20 10:11:10.000000 seqslab-cli-3.3.3/python/seqslab/trs/register/common.py
--rw-r--r--   0 runner    (1001) docker     (127)     7662 2024-05-20 10:11:10.000000 seqslab-cli-3.3.3/python/seqslab/trs/register/template.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-20 10:11:24.459486 seqslab-cli-3.3.3/python/seqslab/trs/resource/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-20 10:11:10.000000 seqslab-cli-3.3.3/python/seqslab/trs/resource/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      865 2024-05-20 10:11:10.000000 seqslab-cli-3.3.3/python/seqslab/trs/resource/azure.py
--rw-r--r--   0 runner    (1001) docker     (127)     6203 2024-05-20 10:11:10.000000 seqslab-cli-3.3.3/python/seqslab/trs/resource/base.py
--rw-r--r--   0 runner    (1001) docker     (127)     1340 2024-05-20 10:11:10.000000 seqslab-cli-3.3.3/python/seqslab/trs/resource/common.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-20 10:11:24.459486 seqslab-cli-3.3.3/python/seqslab/trs/template/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-20 10:11:10.000000 seqslab-cli-3.3.3/python/seqslab/trs/template/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     8959 2024-05-20 10:11:10.000000 seqslab-cli-3.3.3/python/seqslab/trs/template/base.py
--rw-r--r--   0 runner    (1001) docker     (127)     2724 2024-05-20 10:11:10.000000 seqslab-cli-3.3.3/python/seqslab/trs/template/template.py
--rw-r--r--   0 runner    (1001) docker     (127)      951 2024-05-20 10:11:10.000000 seqslab-cli-3.3.3/python/seqslab/usage_logger.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-20 10:11:24.459486 seqslab-cli-3.3.3/python/seqslab/user/
--rw-r--r--   0 runner    (1001) docker     (127)      228 2024-05-20 10:11:10.000000 seqslab-cli-3.3.3/python/seqslab/user/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     7721 2024-05-20 10:11:10.000000 seqslab-cli-3.3.3/python/seqslab/user/commands.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-20 10:11:24.459486 seqslab-cli-3.3.3/python/seqslab/user/internal/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-20 10:11:10.000000 seqslab-cli-3.3.3/python/seqslab/user/internal/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1345 2024-05-20 10:11:10.000000 seqslab-cli-3.3.3/python/seqslab/user/internal/common.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-20 10:11:24.459486 seqslab-cli-3.3.3/python/seqslab/user/resource/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-20 10:11:10.000000 seqslab-cli-3.3.3/python/seqslab/user/resource/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1724 2024-05-20 10:11:10.000000 seqslab-cli-3.3.3/python/seqslab/user/resource/azure.py
--rw-r--r--   0 runner    (1001) docker     (127)     4165 2024-05-20 10:11:10.000000 seqslab-cli-3.3.3/python/seqslab/user/resource/base.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-20 10:11:24.459486 seqslab-cli-3.3.3/python/seqslab/wes/
--rw-r--r--   0 runner    (1001) docker     (127)      226 2024-05-20 10:11:10.000000 seqslab-cli-3.3.3/python/seqslab/wes/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    27990 2024-05-20 10:11:10.000000 seqslab-cli-3.3.3/python/seqslab/wes/commands.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-20 10:11:24.459486 seqslab-cli-3.3.3/python/seqslab/wes/internal/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-20 10:11:10.000000 seqslab-cli-3.3.3/python/seqslab/wes/internal/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1362 2024-05-20 10:11:10.000000 seqslab-cli-3.3.3/python/seqslab/wes/internal/common.py
--rw-r--r--   0 runner    (1001) docker     (127)     8654 2024-05-20 10:11:10.000000 seqslab-cli-3.3.3/python/seqslab/wes/internal/parameters.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-20 10:11:24.459486 seqslab-cli-3.3.3/python/seqslab/wes/resource/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-20 10:11:10.000000 seqslab-cli-3.3.3/python/seqslab/wes/resource/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      885 2024-05-20 10:11:10.000000 seqslab-cli-3.3.3/python/seqslab/wes/resource/azure.py
--rw-r--r--   0 runner    (1001) docker     (127)    13553 2024-05-20 10:11:10.000000 seqslab-cli-3.3.3/python/seqslab/wes/resource/base.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-20 10:11:24.459486 seqslab-cli-3.3.3/python/seqslab/wes/template/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-20 10:11:10.000000 seqslab-cli-3.3.3/python/seqslab/wes/template/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     4294 2024-05-20 10:11:10.000000 seqslab-cli-3.3.3/python/seqslab/wes/template/base.py
--rw-r--r--   0 runner    (1001) docker     (127)     3036 2024-05-20 10:11:10.000000 seqslab-cli-3.3.3/python/seqslab/wes/template/template.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-20 10:11:24.463486 seqslab-cli-3.3.3/python/seqslab/workspace/
--rw-r--r--   0 runner    (1001) docker     (127)      233 2024-05-20 10:11:10.000000 seqslab-cli-3.3.3/python/seqslab/workspace/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     5983 2024-05-20 10:11:10.000000 seqslab-cli-3.3.3/python/seqslab/workspace/commands.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-20 10:11:24.463486 seqslab-cli-3.3.3/python/seqslab/workspace/internal/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-20 10:11:10.000000 seqslab-cli-3.3.3/python/seqslab/workspace/internal/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1354 2024-05-20 10:11:10.000000 seqslab-cli-3.3.3/python/seqslab/workspace/internal/common.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-20 10:11:24.463486 seqslab-cli-3.3.3/python/seqslab/workspace/resource/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-20 10:11:10.000000 seqslab-cli-3.3.3/python/seqslab/workspace/resource/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      865 2024-05-20 10:11:10.000000 seqslab-cli-3.3.3/python/seqslab/workspace/resource/azure.py
--rw-r--r--   0 runner    (1001) docker     (127)     3236 2024-05-20 10:11:10.000000 seqslab-cli-3.3.3/python/seqslab/workspace/resource/base.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-20 10:11:24.463486 seqslab-cli-3.3.3/python/seqslab_cli.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     6565 2024-05-20 10:11:23.000000 seqslab-cli-3.3.3/python/seqslab_cli.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     3787 2024-05-20 10:11:24.000000 seqslab-cli-3.3.3/python/seqslab_cli.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-20 10:11:23.000000 seqslab-cli-3.3.3/python/seqslab_cli.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       46 2024-05-20 10:11:23.000000 seqslab-cli-3.3.3/python/seqslab_cli.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (127)      518 2024-05-20 10:11:23.000000 seqslab-cli-3.3.3/python/seqslab_cli.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)        8 2024-05-20 10:11:23.000000 seqslab-cli-3.3.3/python/seqslab_cli.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-20 10:11:23.000000 seqslab-cli-3.3.3/python/seqslab_cli.egg-info/zip-safe
--rw-r--r--   0 runner    (1001) docker     (127)      454 2024-05-20 10:11:10.000000 seqslab-cli-3.3.3/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (127)      368 2024-05-20 10:11:24.463486 seqslab-cli-3.3.3/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)     2432 2024-05-20 10:11:10.000000 seqslab-cli-3.3.3/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-29 06:58:29.087246 seqslab-cli-3.3.4/
+-rw-r--r--   0 runner    (1001) docker     (127)      689 2024-05-29 06:58:16.000000 seqslab-cli-3.3.4/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)       44 2024-05-29 06:58:16.000000 seqslab-cli-3.3.4/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (127)     6565 2024-05-29 06:58:29.087246 seqslab-cli-3.3.4/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     4631 2024-05-29 06:58:16.000000 seqslab-cli-3.3.4/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-29 06:58:29.071246 seqslab-cli-3.3.4/python/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-29 06:58:29.071246 seqslab-cli-3.3.4/python/seqslab/
+-rw-r--r--   0 runner    (1001) docker     (127)      779 2024-05-29 06:58:16.000000 seqslab-cli-3.3.4/python/seqslab/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-29 06:58:29.071246 seqslab-cli-3.3.4/python/seqslab/auth/
+-rw-r--r--   0 runner    (1001) docker     (127)       79 2024-05-29 06:58:16.000000 seqslab-cli-3.3.4/python/seqslab/auth/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4544 2024-05-29 06:58:16.000000 seqslab-cli-3.3.4/python/seqslab/auth/azuread.py
+-rw-r--r--   0 runner    (1001) docker     (127)    14701 2024-05-29 06:58:16.000000 seqslab-cli-3.3.4/python/seqslab/auth/commands.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1678 2024-05-29 06:58:16.000000 seqslab-cli-3.3.4/python/seqslab/cli.py
+-rw-r--r--   0 runner    (1001) docker     (127)      694 2024-05-29 06:58:16.000000 seqslab-cli-3.3.4/python/seqslab/context.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-29 06:58:29.071246 seqslab-cli-3.3.4/python/seqslab/drs/
+-rw-r--r--   0 runner    (1001) docker     (127)      226 2024-05-29 06:58:16.000000 seqslab-cli-3.3.4/python/seqslab/drs/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-29 06:58:29.075245 seqslab-cli-3.3.4/python/seqslab/drs/api/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-29 06:58:16.000000 seqslab-cli-3.3.4/python/seqslab/drs/api/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    16095 2024-05-29 06:58:16.000000 seqslab-cli-3.3.4/python/seqslab/drs/api/azure.py
+-rw-r--r--   0 runner    (1001) docker     (127)    17051 2024-05-29 06:58:16.000000 seqslab-cli-3.3.4/python/seqslab/drs/api/base.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1354 2024-05-29 06:58:16.000000 seqslab-cli-3.3.4/python/seqslab/drs/api/common.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5415 2024-05-29 06:58:16.000000 seqslab-cli-3.3.4/python/seqslab/drs/api/template.py
+-rw-r--r--   0 runner    (1001) docker     (127)    49945 2024-05-29 06:58:16.000000 seqslab-cli-3.3.4/python/seqslab/drs/commands.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-29 06:58:29.075245 seqslab-cli-3.3.4/python/seqslab/drs/internal/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-29 06:58:16.000000 seqslab-cli-3.3.4/python/seqslab/drs/internal/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    21876 2024-05-29 06:58:16.000000 seqslab-cli-3.3.4/python/seqslab/drs/internal/aiocopy.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1343 2024-05-29 06:58:16.000000 seqslab-cli-3.3.4/python/seqslab/drs/internal/common.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4487 2024-05-29 06:58:16.000000 seqslab-cli-3.3.4/python/seqslab/drs/internal/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-29 06:58:29.075245 seqslab-cli-3.3.4/python/seqslab/drs/storage/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-29 06:58:16.000000 seqslab-cli-3.3.4/python/seqslab/drs/storage/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    28712 2024-05-29 06:58:16.000000 seqslab-cli-3.3.4/python/seqslab/drs/storage/azure.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12704 2024-05-29 06:58:16.000000 seqslab-cli-3.3.4/python/seqslab/drs/storage/base.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-29 06:58:29.075245 seqslab-cli-3.3.4/python/seqslab/drs/utils/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-29 06:58:16.000000 seqslab-cli-3.3.4/python/seqslab/drs/utils/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5815 2024-05-29 06:58:16.000000 seqslab-cli-3.3.4/python/seqslab/drs/utils/atgxmetadata.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2093 2024-05-29 06:58:16.000000 seqslab-cli-3.3.4/python/seqslab/drs/utils/biomimetype.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3175 2024-05-29 06:58:16.000000 seqslab-cli-3.3.4/python/seqslab/drs/utils/progressbar.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2305 2024-05-29 06:58:16.000000 seqslab-cli-3.3.4/python/seqslab/exceptions.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-29 06:58:29.075245 seqslab-cli-3.3.4/python/seqslab/organization/
+-rw-r--r--   0 runner    (1001) docker     (127)      261 2024-05-29 06:58:16.000000 seqslab-cli-3.3.4/python/seqslab/organization/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2354 2024-05-29 06:58:16.000000 seqslab-cli-3.3.4/python/seqslab/organization/commands.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-29 06:58:29.075245 seqslab-cli-3.3.4/python/seqslab/organization/resource/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-29 06:58:16.000000 seqslab-cli-3.3.4/python/seqslab/organization/resource/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1221 2024-05-29 06:58:16.000000 seqslab-cli-3.3.4/python/seqslab/organization/resource/base.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5144 2024-05-29 06:58:16.000000 seqslab-cli-3.3.4/python/seqslab/plugin.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-29 06:58:29.075245 seqslab-cli-3.3.4/python/seqslab/role/
+-rw-r--r--   0 runner    (1001) docker     (127)      228 2024-05-29 06:58:16.000000 seqslab-cli-3.3.4/python/seqslab/role/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1274 2024-05-29 06:58:16.000000 seqslab-cli-3.3.4/python/seqslab/role/commands.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-29 06:58:29.075245 seqslab-cli-3.3.4/python/seqslab/role/internal/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-29 06:58:16.000000 seqslab-cli-3.3.4/python/seqslab/role/internal/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1342 2024-05-29 06:58:16.000000 seqslab-cli-3.3.4/python/seqslab/role/internal/common.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-29 06:58:29.075245 seqslab-cli-3.3.4/python/seqslab/role/resource/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-29 06:58:16.000000 seqslab-cli-3.3.4/python/seqslab/role/resource/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      865 2024-05-29 06:58:16.000000 seqslab-cli-3.3.4/python/seqslab/role/resource/azure.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1354 2024-05-29 06:58:16.000000 seqslab-cli-3.3.4/python/seqslab/role/resource/base.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-29 06:58:29.075245 seqslab-cli-3.3.4/python/seqslab/runsheet/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-29 06:58:16.000000 seqslab-cli-3.3.4/python/seqslab/runsheet/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6374 2024-05-29 06:58:16.000000 seqslab-cli-3.3.4/python/seqslab/runsheet/runsheet.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-29 06:58:29.079245 seqslab-cli-3.3.4/python/seqslab/sample_sheet/
+-rw-r--r--   0 runner    (1001) docker     (127)    56711 2024-05-29 06:58:16.000000 seqslab-cli-3.3.4/python/seqslab/sample_sheet/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)       22 2024-05-29 06:58:16.000000 seqslab-cli-3.3.4/python/seqslab/sample_sheet/_version.py
+-rw-r--r--   0 runner    (1001) docker     (127)      630 2024-05-29 06:58:16.000000 seqslab-cli-3.3.4/python/seqslab/sample_sheet/util.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-29 06:58:29.079245 seqslab-cli-3.3.4/python/seqslab/scr/
+-rw-r--r--   0 runner    (1001) docker     (127)      226 2024-05-29 06:58:16.000000 seqslab-cli-3.3.4/python/seqslab/scr/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6253 2024-05-29 06:58:16.000000 seqslab-cli-3.3.4/python/seqslab/scr/commands.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-29 06:58:29.079245 seqslab-cli-3.3.4/python/seqslab/scr/internal/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-29 06:58:16.000000 seqslab-cli-3.3.4/python/seqslab/scr/internal/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1342 2024-05-29 06:58:16.000000 seqslab-cli-3.3.4/python/seqslab/scr/internal/common.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-29 06:58:29.079245 seqslab-cli-3.3.4/python/seqslab/scr/resource/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-29 06:58:16.000000 seqslab-cli-3.3.4/python/seqslab/scr/resource/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      865 2024-05-29 06:58:16.000000 seqslab-cli-3.3.4/python/seqslab/scr/resource/azure.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4698 2024-05-29 06:58:16.000000 seqslab-cli-3.3.4/python/seqslab/scr/resource/base.py
+-rw-r--r--   0 runner    (1001) docker     (127)      452 2024-05-29 06:58:16.000000 seqslab-cli-3.3.4/python/seqslab/session_logger.py
+-rw-r--r--   0 runner    (1001) docker     (127)      895 2024-05-29 06:58:16.000000 seqslab-cli-3.3.4/python/seqslab/settings.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1370 2024-05-29 06:58:16.000000 seqslab-cli-3.3.4/python/seqslab/statusbar.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-29 06:58:29.079245 seqslab-cli-3.3.4/python/seqslab/trs/
+-rw-r--r--   0 runner    (1001) docker     (127)      226 2024-05-29 06:58:16.000000 seqslab-cli-3.3.4/python/seqslab/trs/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    23164 2024-05-29 06:58:16.000000 seqslab-cli-3.3.4/python/seqslab/trs/commands.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-29 06:58:29.079245 seqslab-cli-3.3.4/python/seqslab/trs/internal/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-29 06:58:16.000000 seqslab-cli-3.3.4/python/seqslab/trs/internal/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1685 2024-05-29 06:58:16.000000 seqslab-cli-3.3.4/python/seqslab/trs/internal/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-29 06:58:29.079245 seqslab-cli-3.3.4/python/seqslab/trs/register/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-29 06:58:16.000000 seqslab-cli-3.3.4/python/seqslab/trs/register/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      999 2024-05-29 06:58:16.000000 seqslab-cli-3.3.4/python/seqslab/trs/register/azure.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10958 2024-05-29 06:58:16.000000 seqslab-cli-3.3.4/python/seqslab/trs/register/base.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1338 2024-05-29 06:58:16.000000 seqslab-cli-3.3.4/python/seqslab/trs/register/common.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7662 2024-05-29 06:58:16.000000 seqslab-cli-3.3.4/python/seqslab/trs/register/template.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-29 06:58:29.079245 seqslab-cli-3.3.4/python/seqslab/trs/resource/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-29 06:58:16.000000 seqslab-cli-3.3.4/python/seqslab/trs/resource/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      865 2024-05-29 06:58:16.000000 seqslab-cli-3.3.4/python/seqslab/trs/resource/azure.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6203 2024-05-29 06:58:16.000000 seqslab-cli-3.3.4/python/seqslab/trs/resource/base.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1340 2024-05-29 06:58:16.000000 seqslab-cli-3.3.4/python/seqslab/trs/resource/common.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-29 06:58:29.083245 seqslab-cli-3.3.4/python/seqslab/trs/template/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-29 06:58:16.000000 seqslab-cli-3.3.4/python/seqslab/trs/template/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7844 2024-05-29 06:58:16.000000 seqslab-cli-3.3.4/python/seqslab/trs/template/base.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2724 2024-05-29 06:58:16.000000 seqslab-cli-3.3.4/python/seqslab/trs/template/template.py
+-rw-r--r--   0 runner    (1001) docker     (127)      951 2024-05-29 06:58:16.000000 seqslab-cli-3.3.4/python/seqslab/usage_logger.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-29 06:58:29.083245 seqslab-cli-3.3.4/python/seqslab/user/
+-rw-r--r--   0 runner    (1001) docker     (127)      228 2024-05-29 06:58:16.000000 seqslab-cli-3.3.4/python/seqslab/user/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7721 2024-05-29 06:58:16.000000 seqslab-cli-3.3.4/python/seqslab/user/commands.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-29 06:58:29.083245 seqslab-cli-3.3.4/python/seqslab/user/internal/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-29 06:58:16.000000 seqslab-cli-3.3.4/python/seqslab/user/internal/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1345 2024-05-29 06:58:16.000000 seqslab-cli-3.3.4/python/seqslab/user/internal/common.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-29 06:58:29.083245 seqslab-cli-3.3.4/python/seqslab/user/resource/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-29 06:58:16.000000 seqslab-cli-3.3.4/python/seqslab/user/resource/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1724 2024-05-29 06:58:16.000000 seqslab-cli-3.3.4/python/seqslab/user/resource/azure.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4165 2024-05-29 06:58:16.000000 seqslab-cli-3.3.4/python/seqslab/user/resource/base.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-29 06:58:29.083245 seqslab-cli-3.3.4/python/seqslab/wes/
+-rw-r--r--   0 runner    (1001) docker     (127)      226 2024-05-29 06:58:16.000000 seqslab-cli-3.3.4/python/seqslab/wes/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    31396 2024-05-29 06:58:16.000000 seqslab-cli-3.3.4/python/seqslab/wes/commands.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-29 06:58:29.083245 seqslab-cli-3.3.4/python/seqslab/wes/internal/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-29 06:58:16.000000 seqslab-cli-3.3.4/python/seqslab/wes/internal/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7936 2024-05-29 06:58:16.000000 seqslab-cli-3.3.4/python/seqslab/wes/internal/parameters.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-29 06:58:29.083245 seqslab-cli-3.3.4/python/seqslab/wes/resource/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-29 06:58:16.000000 seqslab-cli-3.3.4/python/seqslab/wes/resource/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      885 2024-05-29 06:58:16.000000 seqslab-cli-3.3.4/python/seqslab/wes/resource/azure.py
+-rw-r--r--   0 runner    (1001) docker     (127)    14752 2024-05-29 06:58:16.000000 seqslab-cli-3.3.4/python/seqslab/wes/resource/base.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1362 2024-05-29 06:58:16.000000 seqslab-cli-3.3.4/python/seqslab/wes/resource/common.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-29 06:58:29.083245 seqslab-cli-3.3.4/python/seqslab/wes/template/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-29 06:58:16.000000 seqslab-cli-3.3.4/python/seqslab/wes/template/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4437 2024-05-29 06:58:16.000000 seqslab-cli-3.3.4/python/seqslab/wes/template/base.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3036 2024-05-29 06:58:16.000000 seqslab-cli-3.3.4/python/seqslab/wes/template/template.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-29 06:58:29.083245 seqslab-cli-3.3.4/python/seqslab/workspace/
+-rw-r--r--   0 runner    (1001) docker     (127)      233 2024-05-29 06:58:16.000000 seqslab-cli-3.3.4/python/seqslab/workspace/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5983 2024-05-29 06:58:16.000000 seqslab-cli-3.3.4/python/seqslab/workspace/commands.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-29 06:58:29.083245 seqslab-cli-3.3.4/python/seqslab/workspace/internal/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-29 06:58:16.000000 seqslab-cli-3.3.4/python/seqslab/workspace/internal/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1354 2024-05-29 06:58:16.000000 seqslab-cli-3.3.4/python/seqslab/workspace/internal/common.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-29 06:58:29.087246 seqslab-cli-3.3.4/python/seqslab/workspace/resource/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-29 06:58:16.000000 seqslab-cli-3.3.4/python/seqslab/workspace/resource/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      865 2024-05-29 06:58:16.000000 seqslab-cli-3.3.4/python/seqslab/workspace/resource/azure.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3236 2024-05-29 06:58:16.000000 seqslab-cli-3.3.4/python/seqslab/workspace/resource/base.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-29 06:58:29.087246 seqslab-cli-3.3.4/python/seqslab_cli.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     6565 2024-05-29 06:58:28.000000 seqslab-cli-3.3.4/python/seqslab_cli.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     3787 2024-05-29 06:58:29.000000 seqslab-cli-3.3.4/python/seqslab_cli.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-29 06:58:28.000000 seqslab-cli-3.3.4/python/seqslab_cli.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       46 2024-05-29 06:58:28.000000 seqslab-cli-3.3.4/python/seqslab_cli.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      544 2024-05-29 06:58:28.000000 seqslab-cli-3.3.4/python/seqslab_cli.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        8 2024-05-29 06:58:28.000000 seqslab-cli-3.3.4/python/seqslab_cli.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-29 06:58:28.000000 seqslab-cli-3.3.4/python/seqslab_cli.egg-info/zip-safe
+-rw-r--r--   0 runner    (1001) docker     (127)      480 2024-05-29 06:58:16.000000 seqslab-cli-3.3.4/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      368 2024-05-29 06:58:29.087246 seqslab-cli-3.3.4/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)     2432 2024-05-29 06:58:16.000000 seqslab-cli-3.3.4/setup.py
```

### Comparing `seqslab-cli-3.3.3/LICENSE` & `seqslab-cli-3.3.4/LICENSE`

 * *Files identical despite different names*

### Comparing `seqslab-cli-3.3.3/PKG-INFO` & `seqslab-cli-3.3.4/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: seqslab-cli
-Version: 3.3.3
+Version: 3.3.4
 Summary: Atgenomix SeqsLab Command Line Tool
 Home-page: https://github.com/AnomeGAP/seqslab-cli
 Author: Allen Chang
 Author-email: allen.chang@atgenomix.com
 License: Apache License, Version 2.0
 Project-URL: Documentation, https://docs.atgenomix.com/
 Project-URL: Repository, https://github.com/atgenomix/seqslab-cli
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: seqslab-cli Version: 3.3.3 Summary: Atgenomix
+Metadata-Version: 2.1 Name: seqslab-cli Version: 3.3.4 Summary: Atgenomix
 SeqsLab Command Line Tool Home-page: https://github.com/AnomeGAP/seqslab-cli
 Author: Allen Chang Author-email: allen.chang@atgenomix.com License: Apache
 License, Version 2.0 Project-URL: Documentation, https://docs.atgenomix.com/
 Project-URL: Repository, https://github.com/atgenomix/seqslab-cli Description:
 This package provides a unified command line interface to Atgenomix SeqsLab, a
 cloud-native biomedical informatics (BioMed IT) platform. Table of Contents
    1. _G_e_t_t_i_n_g_ _S_t_a_r_t_e_d
```

### Comparing `seqslab-cli-3.3.3/README.md` & `seqslab-cli-3.3.4/README.md`

 * *Files identical despite different names*

### Comparing `seqslab-cli-3.3.3/python/seqslab/__init__.py` & `seqslab-cli-3.3.4/python/seqslab/__init__.py`

 * *Files 0% similar despite different names*

```diff
@@ -17,10 +17,10 @@
 """
 
 name = "seqslab"
 
 __all__ = []
 
 
-__version__ = "3.3.3"
+__version__ = "3.3.4"
 
 LOGGING = {"DIR_PATH": "/var/log/seqslab"}
```

### Comparing `seqslab-cli-3.3.3/python/seqslab/auth/azuread.py` & `seqslab-cli-3.3.4/python/seqslab/auth/azuread.py`

 * *Files 1% similar despite different names*

```diff
@@ -68,22 +68,22 @@
         arbitrary_types_allowed = True
 
 
 class ClientApp(AuthBaseModel):
     public_app: msal.ClientApplication = None
     confidential_app: msal.ClientApplication = None
 
-    def load_client(self, credential: str = None) -> Client:
+    def load_client(self, credential: str = None, tenant: str = None) -> Client:
         proxies = context.get_context().args.proxy
         if credential:
             if not self.confidential_app:
                 self.confidential_app = msal.ConfidentialClientApplication(
                     SOCIAL_AUTH_AZURE_KEY,
                     client_credential=credential,
-                    authority=f"https://login.microsoftonline.com/{SOCIAL_AUTH_AZURE_TENANT_ID}",
+                    authority=f"https://login.microsoftonline.com/{tenant}",
                     app_name=seqslab.name,
                     app_version=seqslab.__version__,
                     proxies=proxies,
                     http_cache=persisted_http_cache,
                 )
             return self.confidential_app
         else:
```

### Comparing `seqslab-cli-3.3.3/python/seqslab/auth/commands.py` & `seqslab-cli-3.3.4/python/seqslab/auth/commands.py`

 * *Files 1% similar despite different names*

```diff
@@ -56,15 +56,17 @@
         credential: str,
         assertion: str,
         scope: str,
         backend: str,
         proxy: str = None,
     ) -> dict:
         scopes = azuread.SOCIAL_AUTH_AZURE_SCOPE_APP.get(scope)
-        client = aad_app.load_client(credential=credential)
+        client = aad_app.load_client(
+            credential=credential, tenant=self._decode(assertion)["tid"]
+        )
         result = client.acquire_token_silent(scopes, account=None)
         if not result:
             logging.info(
                 "No suitable token exists in cache. Let's get a new one from AAD."
             )
             result = client.acquire_token_for_client(scopes=scopes)
 
@@ -88,15 +90,15 @@
 
     def _signin_azure(
         self, device_code: bool, daemon: bool, backend: str, proxy: str = None
     ) -> dict:
         result = None
         token_uri = self.ACCESS_TOKEN_URL.format(backend=backend)
         scopes = azuread.SOCIAL_AUTH_AZURE_SCOPE
-        client = aad_app.load_client()
+        client = aad_app.load_client(tenant=azuread.SOCIAL_AUTH_AZURE_TENANT_ID)
         accounts = client.get_accounts()
         if accounts:
             logging.info(
                 "Azure AD account(s) exists in cache and proceed with token cache."
             )
 
             if 1 == len(accounts):
```

### Comparing `seqslab-cli-3.3.3/python/seqslab/cli.py` & `seqslab-cli-3.3.4/python/seqslab/cli.py`

 * *Files identical despite different names*

### Comparing `seqslab-cli-3.3.3/python/seqslab/context.py` & `seqslab-cli-3.3.4/python/seqslab/context.py`

 * *Files identical despite different names*

### Comparing `seqslab-cli-3.3.3/python/seqslab/drs/api/azure.py` & `seqslab-cli-3.3.4/python/seqslab/drs/api/azure.py`

 * *Files identical despite different names*

### Comparing `seqslab-cli-3.3.3/python/seqslab/drs/api/base.py` & `seqslab-cli-3.3.4/python/seqslab/drs/api/base.py`

 * *Files identical despite different names*

### Comparing `seqslab-cli-3.3.3/python/seqslab/drs/api/common.py` & `seqslab-cli-3.3.4/python/seqslab/drs/api/common.py`

 * *Files identical despite different names*

### Comparing `seqslab-cli-3.3.3/python/seqslab/drs/api/template.py` & `seqslab-cli-3.3.4/python/seqslab/drs/api/template.py`

 * *Files identical despite different names*

### Comparing `seqslab-cli-3.3.3/python/seqslab/drs/commands.py` & `seqslab-cli-3.3.4/python/seqslab/drs/commands.py`

 * *Files identical despite different names*

### Comparing `seqslab-cli-3.3.3/python/seqslab/drs/internal/aiocopy.py` & `seqslab-cli-3.3.4/python/seqslab/drs/internal/aiocopy.py`

 * *Files identical despite different names*

### Comparing `seqslab-cli-3.3.3/python/seqslab/drs/internal/common.py` & `seqslab-cli-3.3.4/python/seqslab/drs/internal/common.py`

 * *Files identical despite different names*

### Comparing `seqslab-cli-3.3.3/python/seqslab/drs/internal/utils.py` & `seqslab-cli-3.3.4/python/seqslab/drs/internal/utils.py`

 * *Files identical despite different names*

### Comparing `seqslab-cli-3.3.3/python/seqslab/drs/storage/azure.py` & `seqslab-cli-3.3.4/python/seqslab/drs/storage/azure.py`

 * *Files identical despite different names*

### Comparing `seqslab-cli-3.3.3/python/seqslab/drs/storage/base.py` & `seqslab-cli-3.3.4/python/seqslab/drs/storage/base.py`

 * *Files identical despite different names*

### Comparing `seqslab-cli-3.3.3/python/seqslab/drs/utils/atgxmetadata.py` & `seqslab-cli-3.3.4/python/seqslab/drs/utils/atgxmetadata.py`

 * *Files identical despite different names*

### Comparing `seqslab-cli-3.3.3/python/seqslab/drs/utils/biomimetype.py` & `seqslab-cli-3.3.4/python/seqslab/drs/utils/biomimetype.py`

 * *Files identical despite different names*

### Comparing `seqslab-cli-3.3.3/python/seqslab/drs/utils/progressbar.py` & `seqslab-cli-3.3.4/python/seqslab/drs/utils/progressbar.py`

 * *Files identical despite different names*

### Comparing `seqslab-cli-3.3.3/python/seqslab/exceptions.py` & `seqslab-cli-3.3.4/python/seqslab/exceptions.py`

 * *Files identical despite different names*

### Comparing `seqslab-cli-3.3.3/python/seqslab/organization/commands.py` & `seqslab-cli-3.3.4/python/seqslab/organization/commands.py`

 * *Files identical despite different names*

### Comparing `seqslab-cli-3.3.3/python/seqslab/organization/resource/base.py` & `seqslab-cli-3.3.4/python/seqslab/organization/resource/base.py`

 * *Files identical despite different names*

### Comparing `seqslab-cli-3.3.3/python/seqslab/plugin.py` & `seqslab-cli-3.3.4/python/seqslab/plugin.py`

 * *Files identical despite different names*

### Comparing `seqslab-cli-3.3.3/python/seqslab/role/commands.py` & `seqslab-cli-3.3.4/python/seqslab/role/commands.py`

 * *Files identical despite different names*

### Comparing `seqslab-cli-3.3.3/python/seqslab/role/internal/common.py` & `seqslab-cli-3.3.4/python/seqslab/role/internal/common.py`

 * *Files identical despite different names*

### Comparing `seqslab-cli-3.3.3/python/seqslab/role/resource/azure.py` & `seqslab-cli-3.3.4/python/seqslab/role/resource/azure.py`

 * *Files identical despite different names*

### Comparing `seqslab-cli-3.3.3/python/seqslab/role/resource/base.py` & `seqslab-cli-3.3.4/python/seqslab/role/resource/base.py`

 * *Files identical despite different names*

### Comparing `seqslab-cli-3.3.3/python/seqslab/runsheet/runsheet.py` & `seqslab-cli-3.3.4/python/seqslab/runsheet/runsheet.py`

 * *Files identical despite different names*

### Comparing `seqslab-cli-3.3.3/python/seqslab/sample_sheet/__init__.py` & `seqslab-cli-3.3.4/python/seqslab/sample_sheet/__init__.py`

 * *Files identical despite different names*

### Comparing `seqslab-cli-3.3.3/python/seqslab/sample_sheet/util.py` & `seqslab-cli-3.3.4/python/seqslab/sample_sheet/util.py`

 * *Files identical despite different names*

### Comparing `seqslab-cli-3.3.3/python/seqslab/scr/commands.py` & `seqslab-cli-3.3.4/python/seqslab/scr/commands.py`

 * *Files identical despite different names*

### Comparing `seqslab-cli-3.3.3/python/seqslab/scr/internal/common.py` & `seqslab-cli-3.3.4/python/seqslab/scr/internal/common.py`

 * *Files identical despite different names*

### Comparing `seqslab-cli-3.3.3/python/seqslab/scr/resource/azure.py` & `seqslab-cli-3.3.4/python/seqslab/scr/resource/azure.py`

 * *Files identical despite different names*

### Comparing `seqslab-cli-3.3.3/python/seqslab/scr/resource/base.py` & `seqslab-cli-3.3.4/python/seqslab/scr/resource/base.py`

 * *Files identical despite different names*

### Comparing `seqslab-cli-3.3.3/python/seqslab/settings.py` & `seqslab-cli-3.3.4/python/seqslab/settings.py`

 * *Files identical despite different names*

### Comparing `seqslab-cli-3.3.3/python/seqslab/statusbar.py` & `seqslab-cli-3.3.4/python/seqslab/statusbar.py`

 * *Files identical despite different names*

### Comparing `seqslab-cli-3.3.3/python/seqslab/trs/commands.py` & `seqslab-cli-3.3.4/python/seqslab/trs/commands.py`

 * *Files identical despite different names*

### Comparing `seqslab-cli-3.3.3/python/seqslab/trs/internal/utils.py` & `seqslab-cli-3.3.4/python/seqslab/trs/internal/utils.py`

 * *Files identical despite different names*

### Comparing `seqslab-cli-3.3.3/python/seqslab/trs/register/azure.py` & `seqslab-cli-3.3.4/python/seqslab/trs/register/azure.py`

 * *Files identical despite different names*

### Comparing `seqslab-cli-3.3.3/python/seqslab/trs/register/base.py` & `seqslab-cli-3.3.4/python/seqslab/trs/register/base.py`

 * *Files identical despite different names*

### Comparing `seqslab-cli-3.3.3/python/seqslab/trs/register/common.py` & `seqslab-cli-3.3.4/python/seqslab/trs/register/common.py`

 * *Files identical despite different names*

### Comparing `seqslab-cli-3.3.3/python/seqslab/trs/register/template.py` & `seqslab-cli-3.3.4/python/seqslab/trs/register/template.py`

 * *Files identical despite different names*

### Comparing `seqslab-cli-3.3.3/python/seqslab/trs/resource/azure.py` & `seqslab-cli-3.3.4/python/seqslab/trs/resource/azure.py`

 * *Files identical despite different names*

### Comparing `seqslab-cli-3.3.3/python/seqslab/trs/resource/base.py` & `seqslab-cli-3.3.4/python/seqslab/trs/resource/base.py`

 * *Files identical despite different names*

### Comparing `seqslab-cli-3.3.3/python/seqslab/trs/resource/common.py` & `seqslab-cli-3.3.4/python/seqslab/trs/resource/common.py`

 * *Files identical despite different names*

### Comparing `seqslab-cli-3.3.3/python/seqslab/trs/template/base.py` & `seqslab-cli-3.3.4/python/seqslab/trs/template/base.py`

 * *Files 4% similar despite different names*

```diff
@@ -18,15 +18,15 @@
         oconfig: List,
         **kwargs,
     ) -> dict:
         parameter = BaseJobs.parameter(
             primary_descriptor=primary_descriptor, zip_file=zip_file
         )
         workflow = self.desc_template(parameter)
-        calls = self.workflow_call_template(parameter)
+        calls = self.call_template(parameter)
         inputs_connections = self.inputs_connections(
             parameter=parameter, inputs_json=inputs_json
         )
         iconfig = self.import_conf(parameter.get("i_configs"), iconfig)
         oconfig = self.import_conf(parameter.get("o_configs"), oconfig)
         return get_template().create(
             parameters=parameter,
@@ -37,15 +37,14 @@
             iconfig=iconfig,
             oconfig=oconfig,
         )
 
     @staticmethod
     def dot_cleaning(gs: str) -> str:
         # Standard Library
-        import re
 
         rx = r';[\w;="]+'
         return re.sub(rx, "", gs)
 
     @staticmethod
     def add_nodes(graph: pydot.Dot) -> set:
         calls = set()
@@ -55,40 +54,14 @@
 
         for subgraph in graph.get_subgraphs():
             for node in subgraph.get_nodes():
                 if node.get_name().startswith("CALL_"):
                     calls.add(node.get_name().replace("CALL_", ""))
         return calls
 
-    def workflow_call_template(self, parameter: dict) -> list:
-        # adding main workflow
-        runtime_cell_select = [
-            pydot.graph_from_dot_data(
-                TrsCreateTemplate.dot_cleaning(parameter["graph"])
-            )[0].get_name()
-        ]
-
-        # parsing workflow>call information from graph string
-        graphRex = re.compile(r'graph\s\w+|}|label="call\s\w+', re.IGNORECASE)
-        wnames = []
-        matches = graphRex.findall(parameter.get("graph"))
-        if matches:
-            for e in matches:
-                if e.startswith("graph "):
-                    wnames.append(e.split(" ")[1].replace("cluster_", ""))
-                elif e.startswith("}"):
-                    wnames.pop()
-                elif e.startswith("label="):
-                    call = e.replace('label="', "").strip('"')
-                    if call.lower().startswith("call"):
-                        runtime_cell_select.append(
-                            "" + wnames[-1] + ">" + call.replace("call ", "")
-                        )
-        return runtime_cell_select
-
     def call_template(self, parameter: dict) -> list:
         calls = [
             pydot.graph_from_dot_data(
                 TrsCreateTemplate.dot_cleaning(parameter["graph"])
             )[0].get_name()
         ]
         for workflow in [
```

### Comparing `seqslab-cli-3.3.3/python/seqslab/trs/template/template.py` & `seqslab-cli-3.3.4/python/seqslab/trs/template/template.py`

 * *Files identical despite different names*

### Comparing `seqslab-cli-3.3.3/python/seqslab/usage_logger.py` & `seqslab-cli-3.3.4/python/seqslab/usage_logger.py`

 * *Files identical despite different names*

### Comparing `seqslab-cli-3.3.3/python/seqslab/user/commands.py` & `seqslab-cli-3.3.4/python/seqslab/user/commands.py`

 * *Files identical despite different names*

### Comparing `seqslab-cli-3.3.3/python/seqslab/user/internal/common.py` & `seqslab-cli-3.3.4/python/seqslab/user/internal/common.py`

 * *Files identical despite different names*

### Comparing `seqslab-cli-3.3.3/python/seqslab/user/resource/azure.py` & `seqslab-cli-3.3.4/python/seqslab/user/resource/azure.py`

 * *Files identical despite different names*

### Comparing `seqslab-cli-3.3.3/python/seqslab/user/resource/base.py` & `seqslab-cli-3.3.4/python/seqslab/user/resource/base.py`

 * *Files identical despite different names*

### Comparing `seqslab-cli-3.3.3/python/seqslab/wes/commands.py` & `seqslab-cli-3.3.4/python/seqslab/wes/commands.py`

 * *Files 9% similar despite different names*

```diff
@@ -7,27 +7,29 @@
 import random
 import re
 import time
 from datetime import datetime
 from functools import lru_cache
 from typing import List
 
+import pytz
 import requests
 from nubia import argument, command, context
 from requests_toolbelt.multipart.encoder import MultipartEncoder
 from seqslab.auth.commands import BaseAuth
 from seqslab.exceptions import exception_handler
 from seqslab.runsheet.runsheet import Run, RunSheet
 from seqslab.trs.register.common import trs_register
 from seqslab.wes import API_HOSTNAME, __version__
 from seqslab.wes.internal import parameters
 from tenacity import retry, stop_after_attempt, wait_fixed
 from termcolor import cprint
+from tzlocal import get_localzone
 
-from .internal.common import get_factory
+from .resource.common import get_factory
 
 """
 Copyright (C) 2022, Atgenomix Incorporated.
 
 All Rights Reserved.
 
 This program is an unpublished copyrighted work which is proprietary to
@@ -182,48 +184,130 @@
         with open(os.path.join(working_dir, response_path), "w") as f:
             json.dump(run_list, f, indent=4)
 
         return 0
 
     @command
     @argument(
-        "run_request_id",
+        "request_path",
         type=str,
         positional=False,
-        description="Specify a previously scheduled run request ID (required). ",
+        description="Specify the request.json file to run (required).",
     )
     @argument(
-        "schedule_tag",
+        "workspace",
+        type=str,
+        description="Specify the workspace based on the signed in account (required).",
+    )
+    @argument(
+        "date",
         type=str,
         positional=False,
-        description="Specify a tag marked on previously uploaded samples for a scheduled WES run (required).",
+        aliases=["d"],
+        description="Specify the schedule date, in the format of YYYY-MM-DD (required).",
     )
     @argument(
-        "workspace",
+        "time",
         type=str,
-        description="Specify the workspace based on the signed in account (required).",
+        positional=False,
+        aliases=["t"],
+        description="Specify the schedule time, in the format of HH-MM (required).",
+    )
+    @argument(
+        "time_zone",
+        type=str,
+        choices=["UTC", "LOCAL"],
+        positional=False,
+        aliases=["z"],
+        description="Specify the time zone for the provided date and time. If 'LOCAL' is selected, the date and time "
+        "will be interpreted according to the operating system's time zone. (optional, default = UTC).",
+    )
+    @argument(
+        "recurrence",
+        type=str,
+        positional=False,
+        aliases=["r"],
+        choices=["Once", "Hourly", "Daily", "Weekly", "Monthly"],
+        description="Specify the schedule recurrence (optional, default = Once).",
     )
-    def schedule(self, run_request_id: str, schedule_tag: str, workspace: str) -> int:
+    def schedule(
+        self,
+        request_path: str,
+        workspace: str,
+        date: str,
+        time: str,
+        time_zone: str = "UTC",
+        recurrence: str = "Once",
+    ) -> int:
         """
-        Run a WES run based on a previously registered run request. Typically, the run request
-        is designed for a scheduled WES run, where the FQN-DRS connection of sequencing samples
-        are left blank for future runtime sample-resolving. Thus, by specifying a sample-resolving rule,
-        the run request can be used to serve a scheduled WES run use case.
+        Schedule a WES run with given date, time, and recurrence.
         """
-        mp = MultipartEncoder(fields={})
+        if not os.path.isfile(request_path):
+            cprint("request_path is not a file", "red")
+            return errno.EINVAL
+        else:
+            try:
+                with open(request_path, "r") as f:
+                    req = json.load(f)
+            except json.decoder.JSONDecodeError as e:
+                cprint(f"given request not in json format - {e}", "red")
+                return errno.EINVAL
+
+        if not self._is_valid_time(date, "%Y-%m-%d"):
+            cprint(f"date {date} not in YYYY-MM-DD format", "red")
+            return errno.EINVAL
+
+        if not self._is_valid_time(time, "%H:%M"):
+            cprint(f"time {time} not in HH-MM format", "red")
+            return errno.EINVAL
+
+        time_f = f"{date} {time}"
+
+        if time_zone == "LOCAL":
+            time_f, msg = self._to_utc(time_f)
+            if not time_f:
+                cprint(f"timezone transform failed {msg}", "red")
+                return errno.EINVAL
+
+        payloads = {
+            "schedule": {"schedule_type": recurrence[0], "next_run": time_f},
+            "request": req,
+        }
+
         resource = get_factory().load_resource(workspace)
-        ret = resource.sync_run_jobs(
-            data=mp,
-            headers={"Content-Type": mp.content_type},
-            run_request_id=run_request_id,
-            run_name=schedule_tag,
+        ret = resource.schedule_run(
+            data=payloads,
+        ).json()
+        cprint(
+            f"wes_schedule_id: {ret['id']}; schedule_details: {str(ret['schedule'])}",
+            "yellow",
         )
-        cprint(f"{ret.content.decode('utf-8')}", "yellow")
         return 0
 
+    @staticmethod
+    def _is_valid_time(time_str: str, time_format: str):
+        try:
+            datetime.strptime(time_str, time_format)
+            return True
+        except ValueError:
+            return False
+
+    @staticmethod
+    def _to_utc(local_t: str):
+        try:
+            local_timezone = pytz.timezone(get_localzone().key)
+            utc_t = (
+                local_timezone.localize(datetime.strptime(local_t, "%Y-%m-%d %H:%M"))
+                .astimezone(pytz.utc)
+                .strftime("%Y-%m-%d %H:%M")
+            )
+            return utc_t, None
+        except Exception as e:
+            return None, str(e)
+
     @command(aliases=["state"])
     @argument(
         "run_id",
         type=str,
         positional=False,
         description="Specify a previously executed WES run ID (required).",
     )
@@ -396,16 +480,29 @@
         if not execs:
             trs_register().load_resource().get_execs_json(
                 workflow_url=run.workflow_url, download_path=execs_path
             )
         else:
             execs_path = f"{working_dir}/{execs}"
 
+        resource = get_factory().load_resource(workspace)
+        ops = resource.list_operator_pipelines(page=1, page_size=1000)["results"]
+        opp_w_args = [
+            op["id"]
+            for op in ops
+            for operator in op["operators"]
+            if isinstance(operator, dict) and operator.get("arguments")
+        ]
         params = parameters.workflow_params(
-            execs_path, run, is_runsheet_template, is_single_end, fq_signature
+            execs_path,
+            run,
+            is_runsheet_template,
+            is_single_end,
+            fq_signature,
+            opp_w_args,
         )
         if not isinstance(params, dict):
             raise Exception(
                 f"Unable to generate workflow_params based on given exec_path, with error code {params}"
             )
 
         request = {
@@ -616,18 +713,17 @@
     def cancel(self, run_id: str, workspace: str) -> int:
         """
         Cancel WES run based on run ID.
         """
         try:
             result = get_factory().load_resource(workspace).cancel_run(run_id)
             cprint(json.dumps(result, indent=4), "yellow")
-        except requests.HTTPError:
-            cprint(f"given run_id {run_id} is not valid.", "red")
+        except requests.HTTPError as e:
+            cprint(f"Fail to cancel Job {run_id} - '{str(e)}'.", "red")
             return -1
-
         return 0
 
     @command
     @argument(
         "run_id",
         type=str,
         positional=False,
@@ -721,27 +817,25 @@
     def operator_pipelines(
         self, workspace: str, page: int = 1, page_size: int = 10, output="json"
     ) -> int:
         """
         List registered operator pipelines.
         """
         resource = get_factory().load_resource(workspace)
-        r = resource.list_runtime_options(page=page, page_size=page_size)
+        r = resource.list_operator_pipelines(page=page, page_size=page_size)
 
         if isinstance(r, int):
             return r
 
         self._stdout(r["results"], output)
         return 0
 
     @staticmethod
     def _stdout(results, output: str) -> int:
         # Standard Library
-        import csv
-        from io import StringIO
 
         from tabulate import tabulate
 
         """
             stdout:: TODO: support different format ex: json, tsv, table
         """
         if output == "json":
@@ -752,14 +846,38 @@
             cprint(
                 tabulate(
                     tabular_data=table_datas, headers=table_header, tablefmt="pipe"
                 )
             )
         return 0
 
+    @command
+    @argument(
+        "run_id",
+        type=str,
+        positional=False,
+        description="Specify the run_id that is going to be delete (required).",
+    )
+    @argument(
+        "workspace",
+        type=str,
+        description="Specify the workspace based on the signed in account (required).",
+    )
+    def delete(self, run_id: str, workspace: str) -> int:
+        """
+        Delete WES run as well as all the generated output files based on run ID.
+        """
+        try:
+            get_factory().load_resource(workspace).delete_run(run_id)
+        except requests.HTTPError as e:
+            cprint(f"Fail to delete Job {run_id} - '{str(e)}'.", "red")
+            return -1
+
+        return 0
+
 
 @command
 class Jobs(BaseJobs):
     """Workflow execution commands"""
 
     @command
     @argument(
```

### Comparing `seqslab-cli-3.3.3/python/seqslab/wes/internal/common.py` & `seqslab-cli-3.3.4/python/seqslab/wes/resource/common.py`

 * *Files identical despite different names*

### Comparing `seqslab-cli-3.3.3/python/seqslab/wes/internal/parameters.py` & `seqslab-cli-3.3.4/python/seqslab/wes/internal/parameters.py`

 * *Files 3% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 import errno
 import json
 import os
 import re
 import zipfile
 
 from seqslab.runsheet.runsheet import Run
-from seqslab.wes.internal.common import get_factory
+from seqslab.wes.resource.common import get_factory
 from seqslab.wes.template.base import (
     WorkflowBackendParamsClusterTemplate,
     WorkflowBackendParamsTemplate,
     WorkflowParamsTemplate,
 )
 from termcolor import cprint
 
@@ -115,28 +115,31 @@
 
 def workflow_params(
     execs_json: str,
     run: Run,
     is_runsheet_template: bool,
     is_single_end: bool,
     fq_sig: str,
+    opp_w_args: dict,
 ) -> dict:
     """
     Create workflow_params.json.
     """
     # TODO: write DRS id to workflow_params based run_sheet content
     if not os.path.isfile(execs_json):
         cprint(f"{execs_json} does not exist", "red")
         return errno.ENOENT
 
     try:
         with open(execs_json, "r") as f:
             t_content = json.loads(f.read())
 
-        params = WorkflowParamsTemplate().create(ex_template=t_content)
+        params = WorkflowParamsTemplate().create(
+            ex_template=t_content, opp_w_args=opp_w_args
+        )
 
         if is_runsheet_template:
             r1fqn, r2fqn = validate_label_column(run)
             lb1 = [sa.Read1_Label for sa in run.samples]
             lb2 = [sa.Read2_Label for sa in run.samples]
             na1 = [
                 f'{_fastq_expr(fq_sig, {k.replace(" ", "_"): v for k, v in sa.to_json().items()})}_r1'
@@ -226,41 +229,21 @@
     resource = get_factory().load_resource(workspace)
     clusters = []
     for k, v in rt_dict.items():
         if k not in calls:
             raise RuntimeError(
                 f"given call name {k} not in TRS registered call name list {calls}!"
             )
-
-        # general workflow>call handling
-        ids = k.split(">")
-        if len(ids) == 2:
-            clusters.append(
-                WorkflowBackendParamsClusterTemplate(
-                    run_time=resource.get_runtime_setting(v),
-                    call_name=ids[1],
-                    workflow_name=ids[0],
-                    kernel_version=kernel_version,
-                )
+        clusters.append(
+            WorkflowBackendParamsClusterTemplate(
+                run_time=resource.get_runtime_setting(v),
+                workflow_name=k,
+                kernel_version=kernel_version,
             )
-        else:
-            # main workflow name
-            if k == primary_workflow_name:
-                clusters.append(
-                    WorkflowBackendParamsClusterTemplate(
-                        run_time=resource.get_runtime_setting(v),
-                        call_name=k,
-                        kernel_version=kernel_version,
-                    )
-                )
-            else:
-                # raise exception for incorrect format of k
-                raise RuntimeError(
-                    f"given identifier {k} does not in format of in TRS registered call name list {calls}!"
-                )
+        )
 
     bk_template = WorkflowBackendParamsTemplate(
         graph=execs.get("graph"),
         clusters=clusters,
         workspace=workspace,
         integrity=integrity,
         trust=trust,
```

### Comparing `seqslab-cli-3.3.3/python/seqslab/wes/resource/azure.py` & `seqslab-cli-3.3.4/python/seqslab/wes/resource/azure.py`

 * *Files identical despite different names*

### Comparing `seqslab-cli-3.3.3/python/seqslab/wes/resource/base.py` & `seqslab-cli-3.3.4/python/seqslab/wes/resource/base.py`

 * *Files 3% similar despite different names*

```diff
@@ -51,14 +51,15 @@
     WES_RUNS_FILE_URL = f"{WES_BASE_URL}runs/{{id}}/files/?backend={{backend}}"
     WES_RUNS_STATUS_URL = f"{WES_BASE_URL}runs/{{id}}/status/?backend={{backend}}"
     WES_RUNTIME_OPTIONS_BASE_URL = f"{WES_BASE_URL}runtime-options/"
     WES_OPERATOR_PIPELINES_BASE_URL = f"{WES_BASE_URL}operator-pipelines/"
     WES_RUNTIME_OPTIONS_URL = (
         f"{WES_BASE_URL}runtime-options/{{name}}?backend={{backend}}"
     )
+    WES_SCHEDULES_URL = f"{WES_BASE_URL}schedules/?backend={{backend}}"
 
     class Response(NamedTuple):
         status: int
         headers: CIMultiDictProxy[str]
         body: Any = None
         attrs: OrderedDict = {}
 
@@ -309,14 +310,24 @@
             url=f"{self.WES_BASE_URL}runs/{run_id}/cancel",
             headers={"Authorization": f"Bearer {token}"},
         ) as response:
             if response.status_code not in [requests.codes.ok]:
                 raise requests.HTTPError(response.text)
             return json.loads(response.content)
 
+    def delete_run(self, run_id) -> int:
+        token = BaseAuth.get_token().get("tokens").get("access")
+        with requests.delete(
+            url=f"{self.WES_BASE_URL}runs/{run_id}",
+            headers={"Authorization": f"Bearer {token}"},
+        ) as response:
+            if response.status_code not in [204]:
+                raise requests.HTTPError(response.text)
+            return 0
+
     def list_runtime_options(self, page=1, page_size=10):
         try:
             token = BaseAuth.get_token().get("tokens").get("access")
             with requests.get(
                 url=f"{self.WES_RUNTIME_OPTIONS_BASE_URL}?page={page}&page_size={page_size}",
                 headers={"Authorization": f"Bearer {token}"},
             ) as response:
@@ -340,7 +351,29 @@
                     raise requests.HTTPError(
                         f"{response.status_code}: {repr(response.text)}"
                     )
         except Exception as err:
             print(err)
             raise err
         return response.json()
+
+    def schedule_run(self, data) -> requests.Response:
+        try:
+            ctx = context.get_context()
+            backend = ctx.args.backend
+            token = BaseAuth.get_token().get("tokens").get("access")
+
+            response = requests.post(
+                url=self.WES_SCHEDULES_URL.format(backend=backend),
+                headers={"Authorization": f"Bearer {token}"},
+                json=data,
+            )
+
+            if response.status_code not in [requests.codes.created]:
+                raise requests.HTTPError(
+                    f"{response.status_code}: {repr(response.text)}"
+                )
+        except Exception as err:
+            print(err)
+            raise err
+
+        return response
```

### Comparing `seqslab-cli-3.3.3/python/seqslab/wes/template/base.py` & `seqslab-cli-3.3.4/python/seqslab/wes/template/base.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 class WorkflowParamsTemplate:
-    def create(self, ex_template: dict) -> dict:
-        operator_pipelines = self.operator_pipelines(ex_template)
+    def create(self, ex_template: dict, opp_w_args: dict) -> dict:
+        operator_pipelines = self.operator_pipelines(ex_template, opp_w_args)
         return {
             "inputs": ex_template.get("inputs"),
             "datasets": ex_template.get("connections", None),
             "tasks": operator_pipelines,
         }
 
     def _flat_list(self, v: list, r: list = [], layer: int = 1) -> dict:
@@ -15,16 +15,15 @@
             else:
                 r.append(element)
         if sub_v:
             layer += 1
             return self._flat_list(sub_v, r, layer)
         return {"list": r, "layer": layer}
 
-    @staticmethod
-    def operator_pipelines(ex_template: dict) -> dict:
+    def operator_pipelines(self, ex_template: dict, opp_w_args: dict) -> dict:
         """
         :param: parameter: parameter API response
         :return:
             {
                 "e2e.alignmentRun.Bwa.in_file_fastq_r1": {
                     "operators": [""],
                     "description": "demo operator"
@@ -38,22 +37,29 @@
                 continue
             assert (
                 v in pl_keys
             ), f"given operator pipeline ID {v} for FQN {k} not in operator pipeline list from execs: {pl_keys}"
             for pipeline in ex_template["operator_pipelines"]:
                 if pipeline["id"] == v:
                     tasks[k] = {
-                        "id": v,
+                        "id": self.norm_pl_key(v, opp_w_args),
                         "operators": pipeline["operators"],
                         "description": pipeline["description"],
                     }
                     continue
         return tasks
 
     @staticmethod
+    def norm_pl_key(pl_key: str, opp_w_args: dict) -> str:
+        for opp in opp_w_args:
+            if pl_key.startswith(opp):
+                return opp
+        return pl_key
+
+    @staticmethod
     def inputs_connections(inputs_connection: list = None) -> dict:
         """
         :param:
             parameter = parameter API response
             inputs_json = {
                 "e2e.ref_sa": "local_path1",
                 "e2e.primer_bedpe": "local_path2",
@@ -111,18 +117,15 @@
     }
     if graph:
         ret.update({"graph": graph})
     return ret
 
 
 def WorkflowBackendParamsClusterTemplate(
-    run_time: dict, call_name: str, kernel_version: str, workflow_name: str = ""
+    run_time: dict, kernel_version: str, workflow_name: str = ""
 ) -> dict:
     if kernel_version:
         opts = run_time["options"]
         opts.append(f"seqslab.kernel.version {kernel_version}")
         run_time.update({"options": opts})
-    if workflow_name:
-        run_time.update({"call": call_name, "workflow": workflow_name})
-    else:
-        run_time.update({"call": call_name})
+    run_time.update({"call": workflow_name})
     return run_time
```

### Comparing `seqslab-cli-3.3.3/python/seqslab/wes/template/template.py` & `seqslab-cli-3.3.4/python/seqslab/wes/template/template.py`

 * *Files identical despite different names*

### Comparing `seqslab-cli-3.3.3/python/seqslab/workspace/commands.py` & `seqslab-cli-3.3.4/python/seqslab/workspace/commands.py`

 * *Files identical despite different names*

### Comparing `seqslab-cli-3.3.3/python/seqslab/workspace/internal/common.py` & `seqslab-cli-3.3.4/python/seqslab/workspace/internal/common.py`

 * *Files identical despite different names*

### Comparing `seqslab-cli-3.3.3/python/seqslab/workspace/resource/azure.py` & `seqslab-cli-3.3.4/python/seqslab/workspace/resource/azure.py`

 * *Files identical despite different names*

### Comparing `seqslab-cli-3.3.3/python/seqslab/workspace/resource/base.py` & `seqslab-cli-3.3.4/python/seqslab/workspace/resource/base.py`

 * *Files identical despite different names*

### Comparing `seqslab-cli-3.3.3/python/seqslab_cli.egg-info/PKG-INFO` & `seqslab-cli-3.3.4/python/seqslab_cli.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: seqslab-cli
-Version: 3.3.3
+Version: 3.3.4
 Summary: Atgenomix SeqsLab Command Line Tool
 Home-page: https://github.com/AnomeGAP/seqslab-cli
 Author: Allen Chang
 Author-email: allen.chang@atgenomix.com
 License: Apache License, Version 2.0
 Project-URL: Documentation, https://docs.atgenomix.com/
 Project-URL: Repository, https://github.com/atgenomix/seqslab-cli
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: seqslab-cli Version: 3.3.3 Summary: Atgenomix
+Metadata-Version: 2.1 Name: seqslab-cli Version: 3.3.4 Summary: Atgenomix
 SeqsLab Command Line Tool Home-page: https://github.com/AnomeGAP/seqslab-cli
 Author: Allen Chang Author-email: allen.chang@atgenomix.com License: Apache
 License, Version 2.0 Project-URL: Documentation, https://docs.atgenomix.com/
 Project-URL: Repository, https://github.com/atgenomix/seqslab-cli Description:
 This package provides a unified command line interface to Atgenomix SeqsLab, a
 cloud-native biomedical informatics (BioMed IT) platform. Table of Contents
    1. _G_e_t_t_i_n_g_ _S_t_a_r_t_e_d
```

### Comparing `seqslab-cli-3.3.3/python/seqslab_cli.egg-info/SOURCES.txt` & `seqslab-cli-3.3.4/python/seqslab_cli.egg-info/SOURCES.txt`

 * *Files 0% similar despite different names*

```diff
@@ -79,19 +79,19 @@
 python/seqslab/user/internal/common.py
 python/seqslab/user/resource/__init__.py
 python/seqslab/user/resource/azure.py
 python/seqslab/user/resource/base.py
 python/seqslab/wes/__init__.py
 python/seqslab/wes/commands.py
 python/seqslab/wes/internal/__init__.py
-python/seqslab/wes/internal/common.py
 python/seqslab/wes/internal/parameters.py
 python/seqslab/wes/resource/__init__.py
 python/seqslab/wes/resource/azure.py
 python/seqslab/wes/resource/base.py
+python/seqslab/wes/resource/common.py
 python/seqslab/wes/template/__init__.py
 python/seqslab/wes/template/base.py
 python/seqslab/wes/template/template.py
 python/seqslab/workspace/__init__.py
 python/seqslab/workspace/commands.py
 python/seqslab/workspace/internal/__init__.py
 python/seqslab/workspace/internal/common.py
```

### Comparing `seqslab-cli-3.3.3/python/seqslab_cli.egg-info/requires.txt` & `seqslab-cli-3.3.4/python/seqslab_cli.egg-info/requires.txt`

 * *Files 19% similar despite different names*

```diff
@@ -24,7 +24,9 @@
 pydot==2.0.0
 orjson==3.10.3
 pydantic~=2.7.1
 aiohttp_retry==2.8.3
 requests~=2.31.0
 setuptools~=69.5.1
 jsonpath-ng==1.6.0
+tzlocal==5.2
+pytz==2021.3
```

### Comparing `seqslab-cli-3.3.3/setup.py` & `seqslab-cli-3.3.4/setup.py`

 * *Files identical despite different names*

