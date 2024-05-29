# Comparing `tmp/frinx_conductor_workers-2.0.0.tar.gz` & `tmp/frinx_conductor_workers-2.1.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "frinx_conductor_workers-2.0.0.tar", last modified: Thu Feb 29 08:17:39 2024, max compression
+gzip compressed data, was "frinx_conductor_workers-2.1.0.tar", last modified: Wed May 29 06:37:04 2024, max compression
```

## Comparing `frinx_conductor_workers-2.0.0.tar` & `frinx_conductor_workers-2.1.0.tar`

### file list

```diff
@@ -1,48 +1,47 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-29 08:17:39.476505 frinx_conductor_workers-2.0.0/
--rw-r--r--   0 runner    (1001) docker     (127)       51 2024-02-29 08:17:30.000000 frinx_conductor_workers-2.0.0/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (127)      725 2024-02-29 08:17:39.476505 frinx_conductor_workers-2.0.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      440 2024-02-29 08:17:30.000000 frinx_conductor_workers-2.0.0/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-29 08:17:39.472505 frinx_conductor_workers-2.0.0/frinx_conductor_workers/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-02-29 08:17:30.000000 frinx_conductor_workers-2.0.0/frinx_conductor_workers/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    14022 2024-02-29 08:17:30.000000 frinx_conductor_workers-2.0.0/frinx_conductor_workers/cli_worker.py
--rw-r--r--   0 runner    (1001) docker     (127)    10474 2024-02-29 08:17:30.000000 frinx_conductor_workers-2.0.0/frinx_conductor_workers/cli_worker_test.py
--rw-r--r--   0 runner    (1001) docker     (127)     3736 2024-02-29 08:17:30.000000 frinx_conductor_workers-2.0.0/frinx_conductor_workers/common_worker.py
--rw-r--r--   0 runner    (1001) docker     (127)     4659 2024-02-29 08:17:30.000000 frinx_conductor_workers-2.0.0/frinx_conductor_workers/connection_manager_worker.py
--rw-r--r--   0 runner    (1001) docker     (127)     2997 2024-02-29 08:17:30.000000 frinx_conductor_workers-2.0.0/frinx_conductor_workers/frinx_rest.py
--rw-r--r--   0 runner    (1001) docker     (127)     5916 2024-02-29 08:17:30.000000 frinx_conductor_workers-2.0.0/frinx_conductor_workers/http_worker.py
--rw-r--r--   0 runner    (1001) docker     (127)     2259 2024-02-29 08:17:30.000000 frinx_conductor_workers-2.0.0/frinx_conductor_workers/import_workflows.py
--rw-r--r--   0 runner    (1001) docker     (127)     1116 2024-02-29 08:17:30.000000 frinx_conductor_workers-2.0.0/frinx_conductor_workers/logging_helpers.py
--rw-r--r--   0 runner    (1001) docker     (127)    12602 2024-02-29 08:17:30.000000 frinx_conductor_workers-2.0.0/frinx_conductor_workers/netconf_worker.py
--rw-r--r--   0 runner    (1001) docker     (127)    10910 2024-02-29 08:17:30.000000 frinx_conductor_workers-2.0.0/frinx_conductor_workers/netconf_worker_test.py
--rw-r--r--   0 runner    (1001) docker     (127)    60931 2024-02-29 08:17:30.000000 frinx_conductor_workers-2.0.0/frinx_conductor_workers/resource_manager_worker.py
--rw-r--r--   0 runner    (1001) docker     (127)    32553 2024-02-29 08:17:30.000000 frinx_conductor_workers-2.0.0/frinx_conductor_workers/uniconfig_worker.py
--rw-r--r--   0 runner    (1001) docker     (127)    21836 2024-02-29 08:17:30.000000 frinx_conductor_workers-2.0.0/frinx_conductor_workers/uniconfig_worker_test.py
--rw-r--r--   0 runner    (1001) docker     (127)     2288 2024-02-29 08:17:30.000000 frinx_conductor_workers-2.0.0/frinx_conductor_workers/util.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-29 08:17:39.472505 frinx_conductor_workers-2.0.0/frinx_conductor_workers.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)      725 2024-02-29 08:17:39.000000 frinx_conductor_workers-2.0.0/frinx_conductor_workers.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     2132 2024-02-29 08:17:39.000000 frinx_conductor_workers-2.0.0/frinx_conductor_workers.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-02-29 08:17:39.000000 frinx_conductor_workers-2.0.0/frinx_conductor_workers.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       50 2024-02-29 08:17:39.000000 frinx_conductor_workers-2.0.0/frinx_conductor_workers.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-29 08:17:39.472505 frinx_conductor_workers-2.0.0/frinx_conductor_workflows/
--rw-r--r--   0 runner    (1001) docker     (127)     2948 2024-02-29 08:17:30.000000 frinx_conductor_workers-2.0.0/frinx_conductor_workflows/Dynamic_fork.json
--rw-r--r--   0 runner    (1001) docker     (127)     1873 2024-02-29 08:17:30.000000 frinx_conductor_workers-2.0.0/frinx_conductor_workflows/Mount_apply_template_unmount_cli.json
--rw-r--r--   0 runner    (1001) docker     (127)     2277 2024-02-29 08:17:30.000000 frinx_conductor_workers-2.0.0/frinx_conductor_workflows/UC_TX_close.json
--rw-r--r--   0 runner    (1001) docker     (127)     2345 2024-02-29 08:17:30.000000 frinx_conductor_workers-2.0.0/frinx_conductor_workflows/UC_TX_commit.json
--rw-r--r--   0 runner    (1001) docker     (127)      944 2024-02-29 08:17:30.000000 frinx_conductor_workers-2.0.0/frinx_conductor_workflows/UC_TX_rollback.json
--rw-r--r--   0 runner    (1001) docker     (127)     2422 2024-02-29 08:17:30.000000 frinx_conductor_workers-2.0.0/frinx_conductor_workflows/UC_TX_start.json
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-02-29 08:17:30.000000 frinx_conductor_workers-2.0.0/frinx_conductor_workflows/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-29 08:17:39.472505 frinx_conductor_workers-2.0.0/frinx_conductor_workflows/resource_manager_workflows/
--rw-r--r--   0 runner    (1001) docker     (127)     5851 2024-02-29 08:17:30.000000 frinx_conductor_workers-2.0.0/frinx_conductor_workflows/resource_manager_workflows/Allocate_IPv4_Prefix_Resource.json
--rw-r--r--   0 runner    (1001) docker     (127)     4818 2024-02-29 08:17:30.000000 frinx_conductor_workers-2.0.0/frinx_conductor_workflows/resource_manager_workflows/Allocate_IPv4_Resource.json
--rw-r--r--   0 runner    (1001) docker     (127)     5568 2024-02-29 08:17:30.000000 frinx_conductor_workers-2.0.0/frinx_conductor_workflows/resource_manager_workflows/Allocate_IPv6_Prefix_Resource.json
--rw-r--r--   0 runner    (1001) docker     (127)     5073 2024-02-29 08:17:30.000000 frinx_conductor_workers-2.0.0/frinx_conductor_workflows/resource_manager_workflows/Allocate_IPv6_Resource.json
--rw-r--r--   0 runner    (1001) docker     (127)     2272 2024-02-29 08:17:30.000000 frinx_conductor_workers-2.0.0/frinx_conductor_workflows/resource_manager_workflows/Create_IPv4_Pool.json
--rw-r--r--   0 runner    (1001) docker     (127)     2428 2024-02-29 08:17:30.000000 frinx_conductor_workers-2.0.0/frinx_conductor_workflows/resource_manager_workflows/Create_IPv4_Prefix_Pool.json
--rw-r--r--   0 runner    (1001) docker     (127)     2403 2024-02-29 08:17:30.000000 frinx_conductor_workers-2.0.0/frinx_conductor_workflows/resource_manager_workflows/Create_IPv6_Pool.json
--rw-r--r--   0 runner    (1001) docker     (127)     2426 2024-02-29 08:17:30.000000 frinx_conductor_workers-2.0.0/frinx_conductor_workflows/resource_manager_workflows/Create_IPv6_Prefix_Pool.json
--rw-r--r--   0 runner    (1001) docker     (127)    17433 2024-02-29 08:17:30.000000 frinx_conductor_workers-2.0.0/frinx_conductor_workflows/resource_manager_workflows/Create_Subnet.json
--rw-r--r--   0 runner    (1001) docker     (127)     1117 2024-02-29 08:17:30.000000 frinx_conductor_workers-2.0.0/frinx_conductor_workflows/resource_manager_workflows/Deallocate_Resource.json
--rw-r--r--   0 runner    (1001) docker     (127)      907 2024-02-29 08:17:30.000000 frinx_conductor_workers-2.0.0/frinx_conductor_workflows/resource_manager_workflows/Delete_Pool_IPv4.json
--rw-r--r--   0 runner    (1001) docker     (127)      907 2024-02-29 08:17:30.000000 frinx_conductor_workers-2.0.0/frinx_conductor_workflows/resource_manager_workflows/Delete_Pool_IPv6.json
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-02-29 08:17:39.476505 frinx_conductor_workers-2.0.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)      645 2024-02-29 08:17:30.000000 frinx_conductor_workers-2.0.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-29 06:37:04.101613 frinx_conductor_workers-2.1.0/
+-rw-r--r--   0 runner    (1001) docker     (127)       51 2024-05-29 06:36:52.000000 frinx_conductor_workers-2.1.0/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (127)      725 2024-05-29 06:37:04.101613 frinx_conductor_workers-2.1.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      440 2024-05-29 06:36:52.000000 frinx_conductor_workers-2.1.0/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-29 06:37:04.101613 frinx_conductor_workers-2.1.0/frinx_conductor_workers/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-29 06:36:52.000000 frinx_conductor_workers-2.1.0/frinx_conductor_workers/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    14022 2024-05-29 06:36:52.000000 frinx_conductor_workers-2.1.0/frinx_conductor_workers/cli_worker.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10474 2024-05-29 06:36:52.000000 frinx_conductor_workers-2.1.0/frinx_conductor_workers/cli_worker_test.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3736 2024-05-29 06:36:52.000000 frinx_conductor_workers-2.1.0/frinx_conductor_workers/common_worker.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4659 2024-05-29 06:36:52.000000 frinx_conductor_workers-2.1.0/frinx_conductor_workers/connection_manager_worker.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2997 2024-05-29 06:36:52.000000 frinx_conductor_workers-2.1.0/frinx_conductor_workers/frinx_rest.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5916 2024-05-29 06:36:52.000000 frinx_conductor_workers-2.1.0/frinx_conductor_workers/http_worker.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2383 2024-05-29 06:36:52.000000 frinx_conductor_workers-2.1.0/frinx_conductor_workers/import_workflows.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1116 2024-05-29 06:36:52.000000 frinx_conductor_workers-2.1.0/frinx_conductor_workers/logging_helpers.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12578 2024-05-29 06:36:52.000000 frinx_conductor_workers-2.1.0/frinx_conductor_workers/netconf_worker.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10910 2024-05-29 06:36:52.000000 frinx_conductor_workers-2.1.0/frinx_conductor_workers/netconf_worker_test.py
+-rw-r--r--   0 runner    (1001) docker     (127)    61429 2024-05-29 06:36:52.000000 frinx_conductor_workers-2.1.0/frinx_conductor_workers/resource_manager_worker.py
+-rw-r--r--   0 runner    (1001) docker     (127)    32525 2024-05-29 06:36:52.000000 frinx_conductor_workers-2.1.0/frinx_conductor_workers/uniconfig_worker.py
+-rw-r--r--   0 runner    (1001) docker     (127)    21836 2024-05-29 06:36:52.000000 frinx_conductor_workers-2.1.0/frinx_conductor_workers/uniconfig_worker_test.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2288 2024-05-29 06:36:52.000000 frinx_conductor_workers-2.1.0/frinx_conductor_workers/util.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-29 06:37:04.101613 frinx_conductor_workers-2.1.0/frinx_conductor_workers.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)      725 2024-05-29 06:37:04.000000 frinx_conductor_workers-2.1.0/frinx_conductor_workers.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     2094 2024-05-29 06:37:04.000000 frinx_conductor_workers-2.1.0/frinx_conductor_workers.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-29 06:37:04.000000 frinx_conductor_workers-2.1.0/frinx_conductor_workers.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       50 2024-05-29 06:37:04.000000 frinx_conductor_workers-2.1.0/frinx_conductor_workers.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-29 06:37:04.101613 frinx_conductor_workers-2.1.0/frinx_conductor_workflows/
+-rw-r--r--   0 runner    (1001) docker     (127)     2948 2024-05-29 06:36:52.000000 frinx_conductor_workers-2.1.0/frinx_conductor_workflows/Dynamic_fork.json
+-rw-r--r--   0 runner    (1001) docker     (127)     1873 2024-05-29 06:36:52.000000 frinx_conductor_workers-2.1.0/frinx_conductor_workflows/Mount_apply_template_unmount_cli.json
+-rw-r--r--   0 runner    (1001) docker     (127)     2277 2024-05-29 06:36:52.000000 frinx_conductor_workers-2.1.0/frinx_conductor_workflows/UC_TX_close.json
+-rw-r--r--   0 runner    (1001) docker     (127)     2345 2024-05-29 06:36:52.000000 frinx_conductor_workers-2.1.0/frinx_conductor_workflows/UC_TX_commit.json
+-rw-r--r--   0 runner    (1001) docker     (127)      944 2024-05-29 06:36:52.000000 frinx_conductor_workers-2.1.0/frinx_conductor_workflows/UC_TX_rollback.json
+-rw-r--r--   0 runner    (1001) docker     (127)     2422 2024-05-29 06:36:52.000000 frinx_conductor_workers-2.1.0/frinx_conductor_workflows/UC_TX_start.json
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-29 06:37:04.101613 frinx_conductor_workers-2.1.0/frinx_conductor_workflows/resource_manager_workflows/
+-rw-r--r--   0 runner    (1001) docker     (127)     5912 2024-05-29 06:36:52.000000 frinx_conductor_workers-2.1.0/frinx_conductor_workflows/resource_manager_workflows/Allocate_IPv4_Prefix_Resource.json
+-rw-r--r--   0 runner    (1001) docker     (127)     4868 2024-05-29 06:36:52.000000 frinx_conductor_workers-2.1.0/frinx_conductor_workflows/resource_manager_workflows/Allocate_IPv4_Resource.json
+-rw-r--r--   0 runner    (1001) docker     (127)     5629 2024-05-29 06:36:52.000000 frinx_conductor_workers-2.1.0/frinx_conductor_workflows/resource_manager_workflows/Allocate_IPv6_Prefix_Resource.json
+-rw-r--r--   0 runner    (1001) docker     (127)     5123 2024-05-29 06:36:52.000000 frinx_conductor_workers-2.1.0/frinx_conductor_workflows/resource_manager_workflows/Allocate_IPv6_Resource.json
+-rw-r--r--   0 runner    (1001) docker     (127)     2278 2024-05-29 06:36:52.000000 frinx_conductor_workers-2.1.0/frinx_conductor_workflows/resource_manager_workflows/Create_IPv4_Pool.json
+-rw-r--r--   0 runner    (1001) docker     (127)     2434 2024-05-29 06:36:52.000000 frinx_conductor_workers-2.1.0/frinx_conductor_workflows/resource_manager_workflows/Create_IPv4_Prefix_Pool.json
+-rw-r--r--   0 runner    (1001) docker     (127)     2409 2024-05-29 06:36:52.000000 frinx_conductor_workers-2.1.0/frinx_conductor_workflows/resource_manager_workflows/Create_IPv6_Pool.json
+-rw-r--r--   0 runner    (1001) docker     (127)     2432 2024-05-29 06:36:52.000000 frinx_conductor_workers-2.1.0/frinx_conductor_workflows/resource_manager_workflows/Create_IPv6_Prefix_Pool.json
+-rw-r--r--   0 runner    (1001) docker     (127)    17642 2024-05-29 06:36:52.000000 frinx_conductor_workers-2.1.0/frinx_conductor_workflows/resource_manager_workflows/Create_Subnet.json
+-rw-r--r--   0 runner    (1001) docker     (127)     1128 2024-05-29 06:36:52.000000 frinx_conductor_workers-2.1.0/frinx_conductor_workflows/resource_manager_workflows/Deallocate_Resource.json
+-rw-r--r--   0 runner    (1001) docker     (127)      918 2024-05-29 06:36:52.000000 frinx_conductor_workers-2.1.0/frinx_conductor_workflows/resource_manager_workflows/Delete_Pool_IPv4.json
+-rw-r--r--   0 runner    (1001) docker     (127)      918 2024-05-29 06:36:52.000000 frinx_conductor_workers-2.1.0/frinx_conductor_workflows/resource_manager_workflows/Delete_Pool_IPv6.json
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-29 06:37:04.101613 frinx_conductor_workers-2.1.0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)      645 2024-05-29 06:36:52.000000 frinx_conductor_workers-2.1.0/setup.py
```

### Comparing `frinx_conductor_workers-2.0.0/PKG-INFO` & `frinx_conductor_workers-2.1.0/PKG-INFO`

 * *Files 14% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: frinx_conductor_workers
-Version: 2.0.0
+Version: 2.1.0
 Summary: Conductor python client workers
 Home-page: https://github.com/FRINXio/fm-base-workers
 Author: Frinx
 Author-email: info@frinx.io
 License: Apache 2.0
 Keywords: conductor
 Description-Content-Type: text/markdown
```

### Comparing `frinx_conductor_workers-2.0.0/frinx_conductor_workers/cli_worker.py` & `frinx_conductor_workers-2.1.0/frinx_conductor_workers/cli_worker.py`

 * *Files identical despite different names*

### Comparing `frinx_conductor_workers-2.0.0/frinx_conductor_workers/cli_worker_test.py` & `frinx_conductor_workers-2.1.0/frinx_conductor_workers/cli_worker_test.py`

 * *Files identical despite different names*

### Comparing `frinx_conductor_workers-2.0.0/frinx_conductor_workers/common_worker.py` & `frinx_conductor_workers-2.1.0/frinx_conductor_workers/common_worker.py`

 * *Files identical despite different names*

### Comparing `frinx_conductor_workers-2.0.0/frinx_conductor_workers/connection_manager_worker.py` & `frinx_conductor_workers-2.1.0/frinx_conductor_workers/connection_manager_worker.py`

 * *Files identical despite different names*

### Comparing `frinx_conductor_workers-2.0.0/frinx_conductor_workers/frinx_rest.py` & `frinx_conductor_workers-2.1.0/frinx_conductor_workers/frinx_rest.py`

 * *Files identical despite different names*

### Comparing `frinx_conductor_workers-2.0.0/frinx_conductor_workers/http_worker.py` & `frinx_conductor_workers-2.1.0/frinx_conductor_workers/http_worker.py`

 * *Files identical despite different names*

### Comparing `frinx_conductor_workers-2.0.0/frinx_conductor_workers/import_workflows.py` & `frinx_conductor_workers-2.1.0/frinx_conductor_workers/import_workflows.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,24 +1,26 @@
 import json
 import logging
 import os
+from pathlib import Path
 
 import requests
 from frinx_conductor_workers.frinx_rest import conductor_headers
 from frinx_conductor_workers.frinx_rest import conductor_url_base
 
 local_logs = logging.getLogger(__name__)
 
 workflow_import_url = conductor_url_base + "/metadata/workflow"
 
+DIR_PATH = Path(os.path.dirname(os.path.realpath(__file__))).parent
+FRINX_CONDUCTOR_WORKFLOWS: Path = Path(f"{DIR_PATH}/frinx_conductor_workflows")
 
-def import_base_workflows():
-    import frinx_conductor_workflows
 
-    import_workflows(os.path.dirname(frinx_conductor_workflows.__file__))
+def import_base_workflows():
+    import_workflows(FRINX_CONDUCTOR_WORKFLOWS)
 
 
 def import_workflows(path):
     if os.path.isdir(path):
         local_logs.info("Importing workflows from folder %s", path)
         with os.scandir(path) as entries:
             for entry in entries:
@@ -32,15 +34,15 @@
                             payload.append(payload_json)
                             r = requests.put(
                                 workflow_import_url,
                                 data=json.dumps(payload),
                                 headers=conductor_headers,
                             )
                             local_logs.info("Response status code - %s", r.status_code)
-                            if r.status_code != 204:
+                            if r.status_code != requests.codes.ok:
                                 local_logs.warning(
                                     "Import of workflow %s failed. "
                                     "Ignoring the workflow. Response content: %s",
                                     entry.name,
                                     r.content,
                                 )
                     except Exception as err:
```

### Comparing `frinx_conductor_workers-2.0.0/frinx_conductor_workers/logging_helpers.py` & `frinx_conductor_workers-2.1.0/frinx_conductor_workers/logging_helpers.py`

 * *Files identical despite different names*

### Comparing `frinx_conductor_workers-2.0.0/frinx_conductor_workers/netconf_worker.py` & `frinx_conductor_workers-2.1.0/frinx_conductor_workers/netconf_worker.py`

 * *Files 2% similar despite different names*

```diff
@@ -71,58 +71,58 @@
     mount_body["input"]["netconf"]["netconf-node-topology:tcp-only"] = task["inputData"]["tcp-only"]
     mount_body["input"]["netconf"]["netconf-node-topology:username"] = task["inputData"]["username"]
     mount_body["input"]["netconf"]["netconf-node-topology:password"] = task["inputData"]["password"]
 
     if (
         "reconcile" in task["inputData"]
         and task["inputData"]["reconcile"] is not None
-        and task["inputData"]["reconcile"] is not ""
+        and task["inputData"]["reconcile"] != ""
     ):
         mount_body["input"]["netconf"]["node-extension:reconcile"] = task["inputData"]["reconcile"]
 
     if (
         "schema-cache-directory" in task["inputData"]
         and task["inputData"]["schema-cache-directory"] is not None
-        and task["inputData"]["schema-cache-directory"] is not ""
+        and task["inputData"]["schema-cache-directory"] != ""
     ):
         mount_body["input"]["netconf"]["netconf-node-topology:schema-cache-directory"] = task[
             "inputData"
         ]["schema-cache-directory"]
 
     if (
         "sleep-factor" in task["inputData"]
         and task["inputData"]["sleep-factor"] is not None
-        and task["inputData"]["sleep-factor"] is not ""
+        and task["inputData"]["sleep-factor"] != ""
     ):
         mount_body["input"]["netconf"]["netconf-node-topology:sleep-factor"] = task["inputData"][
             "sleep-factor"
         ]
 
     if (
         "between-attempts-timeout-millis" in task["inputData"]
         and task["inputData"]["between-attempts-timeout-millis"] is not None
-        and task["inputData"]["between-attempts-timeout-millis"] is not ""
+        and task["inputData"]["between-attempts-timeout-millis"] != ""
     ):
         mount_body["input"]["netconf"]["netconf-node-topology:between-attempts-timeout-millis"] = (
             task["inputData"]["between-attempts-timeout-millis"]
         )
 
     if (
         "connection-timeout-millis" in task["inputData"]
         and task["inputData"]["connection-timeout-millis"] is not None
-        and task["inputData"]["connection-timeout-millis"] is not ""
+        and task["inputData"]["connection-timeout-millis"] != ""
     ):
         mount_body["input"]["netconf"]["netconf-node-topology:connection-timeout-millis"] = task[
             "inputData"
         ]["connection-timeout-millis"]
 
     if (
         "uniconfig-native" in task["inputData"]
         and task["inputData"]["uniconfig-native"] is not None
-        and task["inputData"]["uniconfig-native"] is not ""
+        and task["inputData"]["uniconfig-native"] != ""
     ):
         mount_body["input"]["netconf"]["uniconfig-config:uniconfig-native-enabled"] = task[
             "inputData"
         ]["uniconfig-native"]
 
     if "blacklist" in task["inputData"] and task["inputData"]["blacklist"] is not None:
         mount_body["input"]["netconf"]["uniconfig-config:blacklist"] = {"uniconfig-config:path": []}
```

### Comparing `frinx_conductor_workers-2.0.0/frinx_conductor_workers/netconf_worker_test.py` & `frinx_conductor_workers-2.1.0/frinx_conductor_workers/netconf_worker_test.py`

 * *Files identical despite different names*

### Comparing `frinx_conductor_workers-2.0.0/frinx_conductor_workers/resource_manager_worker.py` & `frinx_conductor_workers-2.1.0/frinx_conductor_workers/resource_manager_worker.py`

 * *Files 0% similar despite different names*

```diff
@@ -56,15 +56,19 @@
     QueryResourcePools(
         tags: { matchesAny: [
             { matchesAll: [{{ pool_names }}] }
             ]
         },
         resourceTypeId: $resource_type_id)
     {
-        id
+        edges {
+            node {
+                id
+            }
+        }
     }
     }"""
 )
 
 query_resource_template = Template(
     """
     query QueryId($resource: String) {
@@ -77,33 +81,35 @@
     }"""
 )
 
 query_pool_by_tag_template = Template(
     """
     query SearchPools($poolTag: String!) {
     SearchPoolsByTags(tags: { matchesAny: [{matchesAll: [$poolTag]}]}) {
-        id
-        AllocationStrategy {Name}
-        Name
-        PoolProperties
+        edges {
+            node {
+                id
+                AllocationStrategy {Name}
+                Name
+                PoolProperties
+            }
+        }
     }
     } """
 )
 
 query_claimed_resource_template = Template(
     """
     query QueryClaimedResource($pool_id: ID!,{{ input_variable }}) {
     {{ query_resource }}(
         poolId: $pool_id,
         {{ input }})
     {
         edges {
-            cursor {
-                ID
-            }
+            cursor
             node {
                 id
                 Properties
                 ParentPool {
                     id
                     Name
                 }
@@ -158,20 +164,18 @@
         utilizedCapacity
     }
     }"""
 )
 
 query_resource_by_alt_id_template = Template(
     """
-    query QueryResourcesByAltId($poolId: ID, $input: Map!, $first: Int, $last: Int, $after: String, $before: String) {
+    query QueryResourcesByAltId($poolId: ID, $input: Map!, $first: Int, $last: Int, $after: Cursor, $before: Cursor) {
     QueryResourcesByAltId(input: $input, poolId: $poolId, first: $first, last: $last, after: $after, before: $before) {
         edges {
-            cursor {
-                ID
-            }
+            cursor
             node {
                 id
                 Properties
                 ParentPool {
                     id
                     Name
                 }
@@ -212,22 +216,26 @@
     }"""
 )
 
 query_search_empty_pools_template = Template(
     """
     query getEmptyPools($resourceTypeId: ID) {
     QueryEmptyResourcePools(resourceTypeId: $resourceTypeId) {
-        id
-        Name
-        Tags {
-            Tag
+        edges {
+            node {
+                id
+                Name
+                Tags {
+                    Tag
+                }
+                AllocationStrategy {
+                    Name
+                }
+            }
         }
-        AllocationStrategy {
-            Name        
-        }    
     }
     }"""
 )
 
 query_recently_active_resources_template = Template(
     """
     query QueryRecentlyActiveResources($fromDatetime: String!, $toDatetime: String, $first: Int, $last: Int, $before: String, $after: String) {
@@ -242,17 +250,15 @@
                     Name
                 } 
                 NestedPool {
                 id                    
                 Name
                 } 
             }
-            cursor{
-                ID
-            }
+            cursor
         }
     }
     }
     """
 )
 
 
@@ -340,17 +346,15 @@
 
         Returns:
             Response from uniresource. Worker output format::
             "result": {
               "data": {
                 "<query_type>": {
                     edges [
-                        cursor {
-                            <ID>
-                        }
+                        cursor: "<ID>"
                         node {
                           "id": "<id>",
                           "Properties": {
                             <properties>
                           }
                           ParentPool {
                             <id>
@@ -711,22 +715,26 @@
 
              task (dict): dictionary with input data ["poolNames", "resource"]
 
              logs: stream of log messages
 
         Returns:
             Response from uniresource. Worker output format::
-            "result":{
-              "data": {
-                "QueryResourcePools": [
-                  {
-                    "id": "<id>"
-                  }
-                ]
-              }
+            "result": {
+                "data": {
+                    "QueryResourcePools": {
+                        "edges": [
+                          {
+                            "node": {
+                                "id": "<id>"
+                            }
+                          }
+                        ]
+                    }
+                }
             }
 
     """
     pool_names = task["inputData"]["poolNames"]
     if type(pool_names) == str:
         pool_names = [name.strip() for name in pool_names.split(",")]
     resource = task["inputData"]["resource"]
@@ -796,22 +804,26 @@
              task (dict): dictionary with input data ["poolTag"]
 
 
          Returns:
             Response from uniresource. Worker output format::
             "result": {
                 "data": {
-                    "SearchPoolsByTags": [
-                        {
+                    "SearchPoolsByTags": {
+                        "edges": [
+                          {
+                            "node": {
                             "id": "<id>",
                             "AllocationStrategy": <Name>
                             "Name": "<name>"
                             "PoolProperties": <PoolProperties>
-                        }
-                    ]
+                            }
+                          }
+                        ]
+                    }
                 }
             }
 
     """
     pool_tag = task["inputData"]["poolTag"]
     body = query_pool_by_tag_template.render()
     variables = {"poolTag": pool_tag}
@@ -1391,22 +1403,26 @@
              task (dict): dictionary with input data ["resourceTypeId"]
 
 
          Returns:
             Response from uniresource. Worker output format::
             "result": {
                 "data": {
-                    "QueryEmptyResourcePools": [
-                        {
-                            "id": "<id>",
-                            "AllocationStrategy": <Name>
-                            "Name": "<name>"
-                            "Tags": <tag>
-                        }
-                    ]
+                    "QueryEmptyResourcePools": {
+                        "edges": [
+                          {
+                            "node": {
+                              "id": "<id>",
+                              "AllocationStrategy": <Name>
+                              "Name": "<name>"
+                              "Tags": <tag>
+                            }
+                          }
+                        ]
+                    }
                 }
             }
 
     """
     resource_type_id = task["inputData"]["resourceTypeId"]
     body = query_search_empty_pools_template.render()
     variables = {"resourceTypeId": resource_type_id}
@@ -1440,17 +1456,15 @@
                                     Name
                                 }
                                 NestedPool {
                                 id
                                 Name
                                 }
                             }
-                            cursor{
-                                ID
-                            }
+                            cursor: "<ID>"
                         }
                     }
                 }
             }
 
     """
     from_datetime = task["inputData"]["fromDatetime"]
```

### Comparing `frinx_conductor_workers-2.0.0/frinx_conductor_workers/uniconfig_worker.py` & `frinx_conductor_workers-2.1.0/frinx_conductor_workers/uniconfig_worker.py`

 * *Files 0% similar despite different names*

```diff
@@ -286,19 +286,17 @@
         for dev in devices:
             if isinstance(dev, str):
                 extracted_devices.append(dev)
             else:
                 if "name" in dev:
                     extracted_devices.append(dev.get("name"))
     else:
-        extracted_devices = (
-            [x.strip() for x in devices.split(",") if x is not ""] if devices else []
-        )
+        extracted_devices = [x.strip() for x in devices.split(",") if x != ""] if devices else []
 
-    if fail_on_empty and len(extracted_devices) is 0:
+    if fail_on_empty and len(extracted_devices) == 0:
         raise Exception(
             "For Uniconfig RPCs, a list of devices needs to be specified. "
             "Global RPCs (involving all devices in topology) are not allowed for your own safety."
         )
     return extracted_devices
```

### Comparing `frinx_conductor_workers-2.0.0/frinx_conductor_workers/uniconfig_worker_test.py` & `frinx_conductor_workers-2.1.0/frinx_conductor_workers/uniconfig_worker_test.py`

 * *Files identical despite different names*

### Comparing `frinx_conductor_workers-2.0.0/frinx_conductor_workers/util.py` & `frinx_conductor_workers-2.1.0/frinx_conductor_workers/util.py`

 * *Files identical despite different names*

### Comparing `frinx_conductor_workers-2.0.0/frinx_conductor_workers.egg-info/PKG-INFO` & `frinx_conductor_workers-2.1.0/frinx_conductor_workers.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: frinx-conductor-workers
-Version: 2.0.0
+Version: 2.1.0
 Summary: Conductor python client workers
 Home-page: https://github.com/FRINXio/fm-base-workers
 Author: Frinx
 Author-email: info@frinx.io
 License: Apache 2.0
 Keywords: conductor
 Description-Content-Type: text/markdown
```

### Comparing `frinx_conductor_workers-2.0.0/frinx_conductor_workers.egg-info/SOURCES.txt` & `frinx_conductor_workers-2.1.0/frinx_conductor_workers.egg-info/SOURCES.txt`

 * *Files 1% similar despite different names*

```diff
@@ -22,15 +22,14 @@
 frinx_conductor_workers.egg-info/top_level.txt
 frinx_conductor_workflows/Dynamic_fork.json
 frinx_conductor_workflows/Mount_apply_template_unmount_cli.json
 frinx_conductor_workflows/UC_TX_close.json
 frinx_conductor_workflows/UC_TX_commit.json
 frinx_conductor_workflows/UC_TX_rollback.json
 frinx_conductor_workflows/UC_TX_start.json
-frinx_conductor_workflows/__init__.py
 frinx_conductor_workflows/resource_manager_workflows/Allocate_IPv4_Prefix_Resource.json
 frinx_conductor_workflows/resource_manager_workflows/Allocate_IPv4_Resource.json
 frinx_conductor_workflows/resource_manager_workflows/Allocate_IPv6_Prefix_Resource.json
 frinx_conductor_workflows/resource_manager_workflows/Allocate_IPv6_Resource.json
 frinx_conductor_workflows/resource_manager_workflows/Create_IPv4_Pool.json
 frinx_conductor_workflows/resource_manager_workflows/Create_IPv4_Prefix_Pool.json
 frinx_conductor_workflows/resource_manager_workflows/Create_IPv6_Pool.json
```

### Comparing `frinx_conductor_workers-2.0.0/frinx_conductor_workflows/Dynamic_fork.json` & `frinx_conductor_workers-2.1.0/frinx_conductor_workflows/Dynamic_fork.json`

 * *Files identical despite different names*

### Comparing `frinx_conductor_workers-2.0.0/frinx_conductor_workflows/Mount_apply_template_unmount_cli.json` & `frinx_conductor_workers-2.1.0/frinx_conductor_workflows/Mount_apply_template_unmount_cli.json`

 * *Files identical despite different names*

### Comparing `frinx_conductor_workers-2.0.0/frinx_conductor_workflows/UC_TX_close.json` & `frinx_conductor_workers-2.1.0/frinx_conductor_workflows/UC_TX_close.json`

 * *Files identical despite different names*

### Comparing `frinx_conductor_workers-2.0.0/frinx_conductor_workflows/UC_TX_commit.json` & `frinx_conductor_workers-2.1.0/frinx_conductor_workflows/UC_TX_commit.json`

 * *Files identical despite different names*

### Comparing `frinx_conductor_workers-2.0.0/frinx_conductor_workflows/UC_TX_rollback.json` & `frinx_conductor_workers-2.1.0/frinx_conductor_workflows/UC_TX_rollback.json`

 * *Files identical despite different names*

### Comparing `frinx_conductor_workers-2.0.0/frinx_conductor_workflows/UC_TX_start.json` & `frinx_conductor_workers-2.1.0/frinx_conductor_workflows/UC_TX_start.json`

 * *Files identical despite different names*

### Comparing `frinx_conductor_workers-2.0.0/frinx_conductor_workflows/resource_manager_workflows/Allocate_IPv4_Prefix_Resource.json` & `frinx_conductor_workers-2.1.0/frinx_conductor_workflows/resource_manager_workflows/Allocate_IPv4_Prefix_Resource.json`

 * *Files 2% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.9994762155162545%*

 * *Differences: {"'tasks'": "{1: {'inputParameters': {'pool_exists': "*

 * *            "'${query_pool_by_tag.output.result.data.SearchPoolsByTags.edges}'}}, 2: "*

 * *            "{'inputParameters': {'address': "*

 * *            "'${query_pool_by_tag.output.result.data.SearchPoolsByTags.edges[0].node.PoolProperties.address}', "*

 * *            "'prefix': "*

 * *            "'${query_pool_by_tag.output.result.data.SearchPoolsByTags.edges[0].node.PoolProperties.prefix}'}}, "*

 * *            "3: {'inputParameters': {'subnet': "*

 * *            "'${query_ […]*

```diff
@@ -38,15 +38,15 @@
                         "taskReferenceName": "terminate_cleanup_pool",
                         "type": "TERMINATE"
                     }
                 ]
             },
             "defaultCase": [],
             "inputParameters": {
-                "pool_exists": "${query_pool_by_tag.output.result.data.SearchPoolsByTags}"
+                "pool_exists": "${query_pool_by_tag.output.result.data.SearchPoolsByTags.edges}"
             },
             "label": "decision",
             "name": "decisionTask",
             "optional": false,
             "startDelay": 0,
             "taskReferenceName": "pool_exists",
             "type": "DECISION"
@@ -54,16 +54,16 @@
         {
             "asyncComplete": false,
             "decisionCases": {},
             "defaultCase": [],
             "defaultExclusiveJoinTask": [],
             "forkTasks": [],
             "inputParameters": {
-                "address": "${query_pool_by_tag.output.result.data.SearchPoolsByTags[0].PoolProperties.address}",
-                "prefix": "${query_pool_by_tag.output.result.data.SearchPoolsByTags[0].PoolProperties.prefix}",
+                "address": "${query_pool_by_tag.output.result.data.SearchPoolsByTags.edges[0].node.PoolProperties.address}",
+                "prefix": "${query_pool_by_tag.output.result.data.SearchPoolsByTags.edges[0].node.PoolProperties.prefix}",
                 "scriptExpression": "return {'subnetAddress': $.address, 'subnetPrefix': $.prefix}"
             },
             "joinOn": [],
             "loopOver": [],
             "name": "LAMBDA_TASK",
             "optional": false,
             "startDelay": 0,
@@ -71,15 +71,15 @@
             "type": "LAMBDA"
         },
         {
             "asyncComplete": false,
             "inputParameters": {
                 "prefix": "${workflow.input.prefix}",
                 "resourceType": "ipv4_prefix",
-                "subnet": "${query_pool_by_tag.output.result.data.SearchPoolsByTags[0].PoolProperties.subnet}"
+                "subnet": "${query_pool_by_tag.output.result.data.SearchPoolsByTags.edges[0].node.PoolProperties.subnet}"
             },
             "name": "RESOURCE_MANAGER_calculate_desired_size_from_prefix",
             "optional": false,
             "startDelay": 0,
             "taskReferenceName": "calculate_desired_size_from_prefix",
             "type": "SIMPLE"
         },
@@ -87,30 +87,30 @@
             "caseExpression": "$.desiredValue.length > 0 ? 'True' : 'False'",
             "decisionCases": {
                 "False": [
                     {
                         "inputParameters": {
                             "alternativeId": "${lambda_print_alt_id.output.result}",
                             "description": "${workflow.input.description}",
-                            "poolId": "${query_pool_by_tag.output.result.data.SearchPoolsByTags[0].id}",
+                            "poolId": "${query_pool_by_tag.output.result.data.SearchPoolsByTags.edges[0].node.id}",
                             "userInput": {
                                 "desiredSize": "${calculate_desired_size_from_prefix.output.result.data}"
                             }
                         },
                         "name": "RESOURCE_MANAGER_claim_resource",
                         "taskReferenceName": "claim_resource_without_desired_value",
                         "type": "SIMPLE"
                     }
                 ],
                 "True": [
                     {
                         "inputParameters": {
                             "alternativeId": "${lambda_print_alt_id.output.result}",
                             "description": "${workflow.input.description}",
-                            "poolId": "${query_pool_by_tag.output.result.data.SearchPoolsByTags[0].id}",
+                            "poolId": "${query_pool_by_tag.output.result.data.SearchPoolsByTags.edges[0].node.id}",
                             "userInput": {
                                 "desiredSize": "${calculate_desired_size_from_prefix.output.result.data}",
                                 "desiredValue": "${workflow.input.desired_value}"
                             }
                         },
                         "name": "RESOURCE_MANAGER_claim_resource",
                         "taskReferenceName": "claim_resource_with_desired_value",
```

### Comparing `frinx_conductor_workers-2.0.0/frinx_conductor_workflows/resource_manager_workflows/Allocate_IPv4_Resource.json` & `frinx_conductor_workers-2.1.0/frinx_conductor_workflows/resource_manager_workflows/Allocate_IPv4_Resource.json`

 * *Files 2% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.9995191055689102%*

 * *Differences: {"'tasks'": "{1: {'inputParameters': {'pool_exists': "*

 * *            "'${query_pool_by_tag.output.result.data.SearchPoolsByTags.edges}'}}, 2: "*

 * *            "{'inputParameters': {'address': "*

 * *            "'${query_pool_by_tag.output.result.data.SearchPoolsByTags.edges[0].node.PoolProperties.address}', "*

 * *            "'prefix': "*

 * *            "'${query_pool_by_tag.output.result.data.SearchPoolsByTags.edges[0].node.PoolProperties.prefix}'}}, "*

 * *            "3: {'decisionCases': {'True': {0: {'inputParameters': {'po […]*

```diff
@@ -38,15 +38,15 @@
                         "taskReferenceName": "terminate_cleanup_pool",
                         "type": "TERMINATE"
                     }
                 ]
             },
             "defaultCase": [],
             "inputParameters": {
-                "pool_exists": "${query_pool_by_tag.output.result.data.SearchPoolsByTags}"
+                "pool_exists": "${query_pool_by_tag.output.result.data.SearchPoolsByTags.edges}"
             },
             "label": "decision",
             "name": "decisionTask",
             "optional": false,
             "startDelay": 0,
             "taskReferenceName": "pool_exists",
             "type": "DECISION"
@@ -54,16 +54,16 @@
         {
             "asyncComplete": false,
             "decisionCases": {},
             "defaultCase": [],
             "defaultExclusiveJoinTask": [],
             "forkTasks": [],
             "inputParameters": {
-                "address": "${query_pool_by_tag.output.result.data.SearchPoolsByTags[0].PoolProperties.address}",
-                "prefix": "${query_pool_by_tag.output.result.data.SearchPoolsByTags[0].PoolProperties.prefix}",
+                "address": "${query_pool_by_tag.output.result.data.SearchPoolsByTags.edges[0].node.PoolProperties.address}",
+                "prefix": "${query_pool_by_tag.output.result.data.SearchPoolsByTags.edges[0].node.PoolProperties.prefix}",
                 "scriptExpression": "return {'subnetAddress': $.address, 'subnetPrefix': $.prefix}"
             },
             "joinOn": [],
             "loopOver": [],
             "name": "LAMBDA_TASK",
             "optional": false,
             "startDelay": 0,
@@ -74,27 +74,27 @@
             "caseExpression": "$.desiredValue.length > 0 ? 'True' : 'False'",
             "decisionCases": {
                 "False": [
                     {
                         "inputParameters": {
                             "alternativeId": "${lambda_print_alt_id.output.result}",
                             "description": "${workflow.input.description}",
-                            "poolId": "${query_pool_by_tag.output.result.data.SearchPoolsByTags[0].id}"
+                            "poolId": "${query_pool_by_tag.output.result.data.SearchPoolsByTags.edges[0].node.id}"
                         },
                         "name": "RESOURCE_MANAGER_claim_resource",
                         "taskReferenceName": "claim_resource_without_desired_value",
                         "type": "SIMPLE"
                     }
                 ],
                 "True": [
                     {
                         "inputParameters": {
                             "alternativeId": "${lambda_print_alt_id.output.result}",
                             "description": "${workflow.input.description}",
-                            "poolId": "${query_pool_by_tag.output.result.data.SearchPoolsByTags[0].id}",
+                            "poolId": "${query_pool_by_tag.output.result.data.SearchPoolsByTags.edges[0].node.id}",
                             "userInput": {
                                 "desiredValue": "${workflow.input.desired_value}"
                             }
                         },
                         "name": "RESOURCE_MANAGER_claim_resource",
                         "taskReferenceName": "claim_resource_with_desired_value",
                         "type": "SIMPLE"
```

### Comparing `frinx_conductor_workers-2.0.0/frinx_conductor_workflows/resource_manager_workflows/Allocate_IPv6_Prefix_Resource.json` & `frinx_conductor_workers-2.1.0/frinx_conductor_workflows/resource_manager_workflows/Allocate_IPv6_Prefix_Resource.json`

 * *Files 3% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.9994762155162545%*

 * *Differences: {"'tasks'": "{1: {'inputParameters': {'pool_exists': "*

 * *            "'${query_pool_by_tag.output.result.data.SearchPoolsByTags.edges}'}}, 2: "*

 * *            "{'inputParameters': {'address': "*

 * *            "'${query_pool_by_tag.output.result.data.SearchPoolsByTags.edges[0].node.PoolProperties.address}', "*

 * *            "'prefix': "*

 * *            "'${query_pool_by_tag.output.result.data.SearchPoolsByTags.edges[0].node.PoolProperties.prefix}'}}, "*

 * *            "3: {'inputParameters': {'subnet': "*

 * *            "'${query_ […]*

```diff
@@ -38,15 +38,15 @@
                         "taskReferenceName": "terminate_cleanup_pool",
                         "type": "TERMINATE"
                     }
                 ]
             },
             "defaultCase": [],
             "inputParameters": {
-                "pool_exists": "${query_pool_by_tag.output.result.data.SearchPoolsByTags}"
+                "pool_exists": "${query_pool_by_tag.output.result.data.SearchPoolsByTags.edges}"
             },
             "label": "decision",
             "name": "decisionTask",
             "optional": false,
             "startDelay": 0,
             "taskReferenceName": "pool_exists",
             "type": "DECISION"
@@ -54,16 +54,16 @@
         {
             "asyncComplete": false,
             "decisionCases": {},
             "defaultCase": [],
             "defaultExclusiveJoinTask": [],
             "forkTasks": [],
             "inputParameters": {
-                "address": "${query_pool_by_tag.output.result.data.SearchPoolsByTags[0].PoolProperties.address}",
-                "prefix": "${query_pool_by_tag.output.result.data.SearchPoolsByTags[0].PoolProperties.prefix}",
+                "address": "${query_pool_by_tag.output.result.data.SearchPoolsByTags.edges[0].node.PoolProperties.address}",
+                "prefix": "${query_pool_by_tag.output.result.data.SearchPoolsByTags.edges[0].node.PoolProperties.prefix}",
                 "scriptExpression": "return {'subnetAddress': $.address, 'subnetPrefix': $.prefix}"
             },
             "joinOn": [],
             "loopOver": [],
             "name": "LAMBDA_TASK",
             "optional": false,
             "startDelay": 0,
@@ -71,15 +71,15 @@
             "type": "LAMBDA"
         },
         {
             "asyncComplete": false,
             "inputParameters": {
                 "prefix": "${workflow.input.prefix}",
                 "resourceType": "ipv6_prefix",
-                "subnet": "${query_pool_by_tag.output.result.data.SearchPoolsByTags[0].PoolProperties.subnet}"
+                "subnet": "${query_pool_by_tag.output.result.data.SearchPoolsByTags.edges[0].node.PoolProperties.subnet}"
             },
             "name": "RESOURCE_MANAGER_calculate_desired_size_from_prefix",
             "optional": false,
             "startDelay": 0,
             "taskReferenceName": "calculate_desired_size_from_prefix",
             "type": "SIMPLE"
         },
@@ -87,30 +87,30 @@
             "caseExpression": "$.desiredValue.length > 0 ? 'True' : 'False'",
             "decisionCases": {
                 "False": [
                     {
                         "inputParameters": {
                             "alternativeId": "${lambda_print_alt_id.output.result}",
                             "description": "${workflow.input.description}",
-                            "poolId": "${query_pool_by_tag.output.result.data.SearchPoolsByTags[0].id}",
+                            "poolId": "${query_pool_by_tag.output.result.data.SearchPoolsByTags.edges[0].node.id}",
                             "userInput": {
                                 "desiredSize": "${calculate_desired_size_from_prefix.output.result.data}"
                             }
                         },
                         "name": "RESOURCE_MANAGER_claim_resource",
                         "taskReferenceName": "claim_resource_without_desired_value",
                         "type": "SIMPLE"
                     }
                 ],
                 "True": [
                     {
                         "inputParameters": {
                             "alternativeId": "${lambda_print_alt_id.output.result}",
                             "description": "${workflow.input.description}",
-                            "poolId": "${query_pool_by_tag.output.result.data.SearchPoolsByTags[0].id}",
+                            "poolId": "${query_pool_by_tag.output.result.data.SearchPoolsByTags.edges[0].node.id}",
                             "userInput": {
                                 "desiredSize": "${calculate_desired_size_from_prefix.output.result.data}",
                                 "desiredValue": "${workflow.input.desired_value}"
                             }
                         },
                         "name": "RESOURCE_MANAGER_claim_resource",
                         "taskReferenceName": "claim_resource_with_desired_value",
```

### Comparing `frinx_conductor_workers-2.0.0/frinx_conductor_workflows/resource_manager_workflows/Allocate_IPv6_Resource.json` & `frinx_conductor_workers-2.1.0/frinx_conductor_workflows/resource_manager_workflows/Allocate_IPv6_Resource.json`

 * *Files 2% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.9995191055689102%*

 * *Differences: {"'tasks'": "{1: {'inputParameters': {'pool_exists': "*

 * *            "'${query_pool_by_tag.output.result.data.SearchPoolsByTags.edges}'}}, 2: "*

 * *            "{'inputParameters': {'address': "*

 * *            "'${query_pool_by_tag.output.result.data.SearchPoolsByTags.edges[0].node.PoolProperties.address}', "*

 * *            "'prefix': "*

 * *            "'${query_pool_by_tag.output.result.data.SearchPoolsByTags.edges[0].node.PoolProperties.prefix}'}}, "*

 * *            "3: {'decisionCases': {'True': {0: {'inputParameters': {'po […]*

```diff
@@ -38,15 +38,15 @@
                         "taskReferenceName": "terminate_cleanup_pool",
                         "type": "TERMINATE"
                     }
                 ]
             },
             "defaultCase": [],
             "inputParameters": {
-                "pool_exists": "${query_pool_by_tag.output.result.data.SearchPoolsByTags}"
+                "pool_exists": "${query_pool_by_tag.output.result.data.SearchPoolsByTags.edges}"
             },
             "label": "decision",
             "name": "decisionTask",
             "optional": false,
             "startDelay": 0,
             "taskReferenceName": "pool_exists",
             "type": "DECISION"
@@ -54,16 +54,16 @@
         {
             "asyncComplete": false,
             "decisionCases": {},
             "defaultCase": [],
             "defaultExclusiveJoinTask": [],
             "forkTasks": [],
             "inputParameters": {
-                "address": "${query_pool_by_tag.output.result.data.SearchPoolsByTags[0].PoolProperties.address}",
-                "prefix": "${query_pool_by_tag.output.result.data.SearchPoolsByTags[0].PoolProperties.prefix}",
+                "address": "${query_pool_by_tag.output.result.data.SearchPoolsByTags.edges[0].node.PoolProperties.address}",
+                "prefix": "${query_pool_by_tag.output.result.data.SearchPoolsByTags.edges[0].node.PoolProperties.prefix}",
                 "scriptExpression": "return {'subnetAddress': $.address, 'subnetPrefix': $.prefix}"
             },
             "joinOn": [],
             "loopOver": [],
             "name": "LAMBDA_TASK",
             "optional": false,
             "startDelay": 0,
@@ -74,27 +74,27 @@
             "caseExpression": "$.desiredValue.length > 0 ? 'True' : 'False'",
             "decisionCases": {
                 "False": [
                     {
                         "inputParameters": {
                             "alternativeId": "${lambda_print_alt_id.output.result}",
                             "description": "${workflow.input.description}",
-                            "poolId": "${query_pool_by_tag.output.result.data.SearchPoolsByTags[0].id}"
+                            "poolId": "${query_pool_by_tag.output.result.data.SearchPoolsByTags.edges[0].node.id}"
                         },
                         "name": "RESOURCE_MANAGER_claim_resource",
                         "taskReferenceName": "claim_resource_without_desired_value",
                         "type": "SIMPLE"
                     }
                 ],
                 "True": [
                     {
                         "inputParameters": {
                             "alternativeId": "${lambda_print_alt_id.output.result}",
                             "description": "${workflow.input.description}",
-                            "poolId": "${query_pool_by_tag.output.result.data.SearchPoolsByTags[0].id}",
+                            "poolId": "${query_pool_by_tag.output.result.data.SearchPoolsByTags.edges[0].node.id}",
                             "userInput": {
                                 "desiredValue": "${workflow.input.desired_value}"
                             }
                         },
                         "name": "RESOURCE_MANAGER_claim_resource",
                         "taskReferenceName": "claim_resource_with_desired_value",
                         "type": "SIMPLE"
```

### Comparing `frinx_conductor_workers-2.0.0/frinx_conductor_workflows/resource_manager_workflows/Create_IPv4_Pool.json` & `frinx_conductor_workers-2.1.0/frinx_conductor_workflows/resource_manager_workflows/Create_IPv4_Pool.json`

 * *Files 1% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.9994791666666667%*

 * *Differences: {"'tasks'": "{1: {'inputParameters': {'pool_exists': "*

 * *            "'${query_pool_by_tag.output.result.data.SearchPoolsByTags.edges}'}}}"}*

```diff
@@ -34,15 +34,15 @@
                         "taskReferenceName": "terminate_cleanup_pool",
                         "type": "TERMINATE"
                     }
                 ]
             },
             "defaultCase": [],
             "inputParameters": {
-                "pool_exists": "${query_pool_by_tag.output.result.data.SearchPoolsByTags}"
+                "pool_exists": "${query_pool_by_tag.output.result.data.SearchPoolsByTags.edges}"
             },
             "label": "decision",
             "name": "decisionTask",
             "optional": false,
             "startDelay": 0,
             "taskReferenceName": "pool_exists",
             "type": "DECISION"
```

### Comparing `frinx_conductor_workers-2.0.0/frinx_conductor_workflows/resource_manager_workflows/Create_IPv4_Prefix_Pool.json` & `frinx_conductor_workers-2.1.0/frinx_conductor_workflows/resource_manager_workflows/Create_IPv4_Prefix_Pool.json`

 * *Files 0% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.9994791666666667%*

 * *Differences: {"'tasks'": "{1: {'inputParameters': {'pool_exists': "*

 * *            "'${query_pool_by_tag.output.result.data.SearchPoolsByTags.edges}'}}}"}*

```diff
@@ -34,15 +34,15 @@
                         "taskReferenceName": "terminate_cleanup_pool",
                         "type": "TERMINATE"
                     }
                 ]
             },
             "defaultCase": [],
             "inputParameters": {
-                "pool_exists": "${query_pool_by_tag.output.result.data.SearchPoolsByTags}"
+                "pool_exists": "${query_pool_by_tag.output.result.data.SearchPoolsByTags.edges}"
             },
             "label": "decision",
             "name": "decisionTask",
             "optional": false,
             "startDelay": 0,
             "taskReferenceName": "pool_exists",
             "type": "DECISION"
```

### Comparing `frinx_conductor_workers-2.0.0/frinx_conductor_workflows/resource_manager_workflows/Create_IPv6_Pool.json` & `frinx_conductor_workers-2.1.0/frinx_conductor_workflows/resource_manager_workflows/Create_IPv6_Pool.json`

 * *Files 1% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.9994791666666667%*

 * *Differences: {"'tasks'": "{1: {'inputParameters': {'pool_exists': "*

 * *            "'${query_pool_by_tag.output.result.data.SearchPoolsByTags.edges}'}}}"}*

```diff
@@ -34,15 +34,15 @@
                         "taskReferenceName": "terminate_cleanup_pool",
                         "type": "TERMINATE"
                     }
                 ]
             },
             "defaultCase": [],
             "inputParameters": {
-                "pool_exists": "${query_pool_by_tag.output.result.data.SearchPoolsByTags}"
+                "pool_exists": "${query_pool_by_tag.output.result.data.SearchPoolsByTags.edges}"
             },
             "label": "decision",
             "name": "decisionTask",
             "optional": false,
             "startDelay": 0,
             "taskReferenceName": "pool_exists",
             "type": "DECISION"
```

### Comparing `frinx_conductor_workers-2.0.0/frinx_conductor_workflows/resource_manager_workflows/Create_IPv6_Prefix_Pool.json` & `frinx_conductor_workers-2.1.0/frinx_conductor_workflows/resource_manager_workflows/Create_IPv6_Prefix_Pool.json`

 * *Files 4% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.9994791666666667%*

 * *Differences: {"'tasks'": "{1: {'inputParameters': {'pool_exists': "*

 * *            "'${query_pool_by_tag.output.result.data.SearchPoolsByTags.edges}'}}}"}*

```diff
@@ -34,15 +34,15 @@
                         "taskReferenceName": "terminate_cleanup_pool",
                         "type": "TERMINATE"
                     }
                 ]
             },
             "defaultCase": [],
             "inputParameters": {
-                "pool_exists": "${query_pool_by_tag.output.result.data.SearchPoolsByTags}"
+                "pool_exists": "${query_pool_by_tag.output.result.data.SearchPoolsByTags.edges}"
             },
             "label": "decision",
             "name": "decisionTask",
             "optional": false,
             "startDelay": 0,
             "taskReferenceName": "pool_exists",
             "type": "DECISION"
```

### Comparing `frinx_conductor_workers-2.0.0/frinx_conductor_workflows/resource_manager_workflows/Create_Subnet.json` & `frinx_conductor_workers-2.1.0/frinx_conductor_workflows/resource_manager_workflows/Create_Subnet.json`

 * *Files 7% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.9995923281365872%*

 * *Differences: {"'tasks'": "{1: {'inputParameters': {'address': "*

 * *            "'${query_pool_by_tag.output.result.data.SearchPoolsByTags.edges[0].node.PoolProperties.address}', "*

 * *            "'prefix': "*

 * *            "'${query_pool_by_tag.output.result.data.SearchPoolsByTags.edges[0].node.PoolProperties.prefix}'}}, "*

 * *            "2: {'inputParameters': {'resourceType': "*

 * *            "'${query_pool_by_tag.output.result.data.SearchPoolsByTags.edges[0].node.AllocationStrategy.Name}', "*

 * *            "'subnet': "*

 * *            "'$ […]*

```diff
@@ -22,31 +22,32 @@
         {
             "asyncComplete": false,
             "decisionCases": {},
             "defaultCase": [],
             "defaultExclusiveJoinTask": [],
             "forkTasks": [],
             "inputParameters": {
-                "address": "${query_pool_by_tag.output.result.data.SearchPoolsByTags[0].PoolProperties.address}",
-                "prefix": "${query_pool_by_tag.output.result.data.SearchPoolsByTags[0].PoolProperties.prefix}",
+                "address": "${query_pool_by_tag.output.result.data.SearchPoolsByTags.edges[0].node.PoolProperties.address}",
+                "prefix": "${query_pool_by_tag.output.result.data.SearchPoolsByTags.edges[0].node.PoolProperties.prefix}",
                 "scriptExpression": "return {'subnetAddress': $.address, 'subnetPrefix': $.prefix}"
             },
             "joinOn": [],
             "loopOver": [],
             "name": "LAMBDA_TASK",
             "optional": false,
             "startDelay": 0,
             "taskReferenceName": "lambda_print_alt_id",
             "type": "LAMBDA"
         },
         {
             "asyncComplete": false,
             "inputParameters": {
                 "prefix": "${workflow.input.prefix}",
-                "resourceType": "${query_pool_by_tag.output.result.data.SearchPoolsByTags[0].AllocationStrategy.Name}"
+                "resourceType": "${query_pool_by_tag.output.result.data.SearchPoolsByTags.edges[0].node.AllocationStrategy.Name}",
+                "subnet": "${query_pool_by_tag.output.result.data.SearchPoolsByTags.edges[0].node.PoolProperties.subnet}"
             },
             "name": "RESOURCE_MANAGER_calculate_desired_size_from_prefix",
             "optional": false,
             "startDelay": 0,
             "taskReferenceName": "calculate_desired_size_from_prefix",
             "type": "SIMPLE"
         },
@@ -96,15 +97,15 @@
                                     "caseExpression": "$.param.length > 0 ? 'True' : 'False'",
                                     "decisionCases": {
                                         "False": [
                                             {
                                                 "inputParameters": {
                                                     "alternativeId": "${lambda_print_alt_id.output.result}",
                                                     "description": "parent resource for nested pool",
-                                                    "poolId": "${query_pool_by_tag.output.result.data.SearchPoolsByTags[0].id}",
+                                                    "poolId": "${query_pool_by_tag.output.result.data.SearchPoolsByTags.edges[0].node.id}",
                                                     "userInput": {
                                                         "desiredSize": "${calculate_desired_size_from_prefix.output.result.data}"
                                                     }
                                                 },
                                                 "name": "RESOURCE_MANAGER_claim_resource",
                                                 "taskReferenceName": "claim_resource_ipv4",
                                                 "type": "SIMPLE"
@@ -112,15 +113,15 @@
                                         ],
                                         "True": [
                                             {
                                                 "inputParameters": {
                                                     "alternativeId": "${lambda_print_alt_id.output.result}",
                                                     "description": "parent resource for nested pool",
                                                     "hostAddress": "${workflow.input.subnet_ip_address}",
-                                                    "poolId": "${query_pool_by_tag.output.result.data.SearchPoolsByTags[0].id}",
+                                                    "poolId": "${query_pool_by_tag.output.result.data.SearchPoolsByTags.edges[0].node.id}",
                                                     "userInput": {
                                                         "desiredSize": "${calculate_desired_size_from_prefix.output.result.data}",
                                                         "desiredValue": "${workflow.input.subnet_ip_address}"
                                                     }
                                                 },
                                                 "name": "RESOURCE_MANAGER_claim_resource",
                                                 "taskReferenceName": "claim_resource_ipv4_desiredValue",
@@ -194,15 +195,15 @@
                                     "caseExpression": "$.param.length > 0 ? 'True' : 'False'",
                                     "decisionCases": {
                                         "False": [
                                             {
                                                 "inputParameters": {
                                                     "alternativeId": "${lambda_print_alt_id.output.result}",
                                                     "description": "parent resource for nested pool",
-                                                    "poolId": "${query_pool_by_tag.output.result.data.SearchPoolsByTags[0].id}",
+                                                    "poolId": "${query_pool_by_tag.output.result.data.SearchPoolsByTags.edges[0].node.id}",
                                                     "userInput": {
                                                         "desiredSize": "${calculate_desired_size_from_prefix.output.result.data}"
                                                     }
                                                 },
                                                 "name": "RESOURCE_MANAGER_claim_resource",
                                                 "taskReferenceName": "claim_resource_ipv6",
                                                 "type": "SIMPLE"
@@ -210,15 +211,15 @@
                                         ],
                                         "True": [
                                             {
                                                 "inputParameters": {
                                                     "alternativeId": "${lambda_print_alt_id.output.result}",
                                                     "description": "parent resource for nested pool",
                                                     "hostAddress": "${workflow.input.subnet_ip_address}",
-                                                    "poolId": "${query_pool_by_tag.output.result.data.SearchPoolsByTags[0].id}",
+                                                    "poolId": "${query_pool_by_tag.output.result.data.SearchPoolsByTags.edges[0].node.id}",
                                                     "userInput": {
                                                         "desiredSize": "${calculate_desired_size_from_prefix.output.result.data}",
                                                         "desiredValue": "${workflow.input.subnet_ip_address}"
                                                     }
                                                 },
                                                 "name": "RESOURCE_MANAGER_claim_resource",
                                                 "taskReferenceName": "claim_resource_ipv6_desiredValue",
@@ -285,15 +286,15 @@
                                     "startDelay": 0,
                                     "taskReferenceName": "lambda_print_result_ipv6",
                                     "type": "LAMBDA"
                                 }
                             ]
                         },
                         "inputParameters": {
-                            "poolType": "${query_pool_by_tag.output.result.data.SearchPoolsByTags[0].AllocationStrategy.Name}"
+                            "poolType": "${query_pool_by_tag.output.result.data.SearchPoolsByTags.edges[0].node.AllocationStrategy.Name}"
                         },
                         "label": "decision",
                         "name": "decisionTask",
                         "optional": false,
                         "startDelay": 0,
                         "taskReferenceName": "decision_pool_type",
                         "type": "DECISION"
```

### Comparing `frinx_conductor_workers-2.0.0/frinx_conductor_workflows/resource_manager_workflows/Deallocate_Resource.json` & `frinx_conductor_workers-2.1.0/frinx_conductor_workflows/resource_manager_workflows/Deallocate_Resource.json`

 * *Files 2% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.9990234375%*

 * *Differences: {"'tasks'": "{1: {'inputParameters': {'poolId': "*

 * *            "'${query_pool_by_tag.output.result.data.SearchPoolsByTags.edges[0].node.id}'}}}"}*

```diff
@@ -13,15 +13,15 @@
             },
             "name": "RESOURCE_MANAGER_query_pool_by_tag",
             "taskReferenceName": "query_pool_by_tag",
             "type": "SIMPLE"
         },
         {
             "inputParameters": {
-                "poolId": "${query_pool_by_tag.output.result.data.SearchPoolsByTags[0].id}",
+                "poolId": "${query_pool_by_tag.output.result.data.SearchPoolsByTags.edges[0].node.id}",
                 "userInput": {
                     "address": "${workflow.input.ip_address}"
                 }
             },
             "name": "RESOURCE_MANAGER_deallocate_resource",
             "taskReferenceName": "deallocate_resource",
             "type": "SIMPLE"
```

### Comparing `frinx_conductor_workers-2.0.0/frinx_conductor_workflows/resource_manager_workflows/Delete_Pool_IPv4.json` & `frinx_conductor_workers-2.1.0/frinx_conductor_workflows/resource_manager_workflows/Delete_Pool_IPv4.json`

 * *Files 2% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.998046875%*

 * *Differences: {"'tasks'": "{1: {'inputParameters': {'poolId': "*

 * *            "'${query_pool_by_tag.output.result.data.SearchPoolsByTags.edges[0].node.id}'}}}"}*

```diff
@@ -13,15 +13,15 @@
             },
             "name": "RESOURCE_MANAGER_query_pool_by_tag",
             "taskReferenceName": "query_pool_by_tag",
             "type": "SIMPLE"
         },
         {
             "inputParameters": {
-                "poolId": "${query_pool_by_tag.output.result.data.SearchPoolsByTags[0].id}"
+                "poolId": "${query_pool_by_tag.output.result.data.SearchPoolsByTags.edges[0].node.id}"
             },
             "name": "RESOURCE_MANAGER_delete_pool",
             "taskReferenceName": "delete_pool",
             "type": "SIMPLE"
         }
     ],
     "version": 1,
```

### Comparing `frinx_conductor_workers-2.0.0/frinx_conductor_workflows/resource_manager_workflows/Delete_Pool_IPv6.json` & `frinx_conductor_workers-2.1.0/frinx_conductor_workflows/resource_manager_workflows/Delete_Pool_IPv6.json`

 * *Files 25% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.998046875%*

 * *Differences: {"'tasks'": "{1: {'inputParameters': {'poolId': "*

 * *            "'${query_pool_by_tag.output.result.data.SearchPoolsByTags.edges[0].node.id}'}}}"}*

```diff
@@ -13,15 +13,15 @@
             },
             "name": "RESOURCE_MANAGER_query_pool_by_tag",
             "taskReferenceName": "query_pool_by_tag",
             "type": "SIMPLE"
         },
         {
             "inputParameters": {
-                "poolId": "${query_pool_by_tag.output.result.data.SearchPoolsByTags[0].id}"
+                "poolId": "${query_pool_by_tag.output.result.data.SearchPoolsByTags.edges[0].node.id}"
             },
             "name": "RESOURCE_MANAGER_delete_pool",
             "taskReferenceName": "delete_pool",
             "type": "SIMPLE"
         }
     ],
     "version": 1,
```

### Comparing `frinx_conductor_workers-2.0.0/setup.py` & `frinx_conductor_workers-2.1.0/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -6,15 +6,15 @@
 def __read__(file_name):
     return open(os.path.join(os.path.dirname(__file__), file_name)).read()
 
 
 setup(
     name="frinx_conductor_workers",
     packages=["frinx_conductor_workers", "frinx_conductor_workflows"],
-    version="2.0.0",
+    version="2.1.0",
     description="Conductor python client workers",
     author="Frinx",
     author_email="info@frinx.io",
     url="https://github.com/FRINXio/fm-base-workers",
     keywords=["conductor"],
     license="Apache 2.0",
     include_package_data=True,
```

