# Comparing `tmp/qctrl_workflow_client-3.1.0.tar.gz` & `tmp/qctrl_workflow_client-3.1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "qctrl_workflow_client-3.1.0.tar", max compression
+gzip compressed data, was "qctrl_workflow_client-3.1.1.tar", max compression
```

## Comparing `qctrl_workflow_client-3.1.0.tar` & `qctrl_workflow_client-3.1.1.tar`

### file list

```diff
@@ -1,15 +1,15 @@
--rw-r--r--   0        0        0    36587 2024-05-22 02:04:53.984077 qctrl_workflow_client-3.1.0/LICENSE
--rw-r--r--   0        0        0      223 2024-05-22 02:04:53.984077 qctrl_workflow_client-3.1.0/README.md
--rw-r--r--   0        0        0     2785 2024-05-22 02:05:17.628090 qctrl_workflow_client-3.1.0/pyproject.toml
--rw-r--r--   0        0        0      954 2024-05-22 02:05:17.632090 qctrl_workflow_client-3.1.0/qctrlworkflowclient/__init__.py
--rw-r--r--   0        0        0     3311 2024-05-22 02:04:53.988077 qctrl_workflow_client-3.1.0/qctrlworkflowclient/defaults.py
--rw-r--r--   0        0        0     4840 2024-05-22 02:04:53.988077 qctrl_workflow_client-3.1.0/qctrlworkflowclient/functions.py
--rw-r--r--   0        0        0     1583 2024-05-22 02:04:53.988077 qctrl_workflow_client-3.1.0/qctrlworkflowclient/globals.py
--rw-r--r--   0        0        0      969 2024-05-22 02:04:53.988077 qctrl_workflow_client-3.1.0/qctrlworkflowclient/products.py
--rw-r--r--   0        0        0      638 2024-05-22 02:05:17.636090 qctrl_workflow_client-3.1.0/qctrlworkflowclient/router/__init__.py
--rw-r--r--   0        0        0    24063 2024-05-22 02:04:53.988077 qctrl_workflow_client-3.1.0/qctrlworkflowclient/router/api.py
--rw-r--r--   0        0        0     1206 2024-05-22 02:04:53.988077 qctrl_workflow_client-3.1.0/qctrlworkflowclient/router/base.py
--rw-r--r--   0        0        0     1201 2024-05-22 02:04:53.988077 qctrl_workflow_client-3.1.0/qctrlworkflowclient/router/local.py
--rw-r--r--   0        0        0     3332 2024-05-22 02:04:53.988077 qctrl_workflow_client-3.1.0/qctrlworkflowclient/settings.py
--rw-r--r--   0        0        0     5361 2024-05-22 02:04:53.988077 qctrl_workflow_client-3.1.0/qctrlworkflowclient/utils.py
--rw-r--r--   0        0        0     2489 1970-01-01 00:00:00.000000 qctrl_workflow_client-3.1.0/PKG-INFO
+-rw-r--r--   0        0        0    36587 2024-05-29 06:32:39.870887 qctrl_workflow_client-3.1.1/LICENSE
+-rw-r--r--   0        0        0      223 2024-05-29 06:32:39.870887 qctrl_workflow_client-3.1.1/README.md
+-rw-r--r--   0        0        0     2784 2024-05-29 06:33:03.782964 qctrl_workflow_client-3.1.1/pyproject.toml
+-rw-r--r--   0        0        0      954 2024-05-29 06:33:03.786964 qctrl_workflow_client-3.1.1/qctrlworkflowclient/__init__.py
+-rw-r--r--   0        0        0     3311 2024-05-29 06:32:39.874887 qctrl_workflow_client-3.1.1/qctrlworkflowclient/defaults.py
+-rw-r--r--   0        0        0     4944 2024-05-29 06:32:39.874887 qctrl_workflow_client-3.1.1/qctrlworkflowclient/functions.py
+-rw-r--r--   0        0        0     1583 2024-05-29 06:32:39.874887 qctrl_workflow_client-3.1.1/qctrlworkflowclient/globals.py
+-rw-r--r--   0        0        0      969 2024-05-29 06:32:39.874887 qctrl_workflow_client-3.1.1/qctrlworkflowclient/products.py
+-rw-r--r--   0        0        0      638 2024-05-29 06:33:03.790964 qctrl_workflow_client-3.1.1/qctrlworkflowclient/router/__init__.py
+-rw-r--r--   0        0        0    24063 2024-05-29 06:32:39.874887 qctrl_workflow_client-3.1.1/qctrlworkflowclient/router/api.py
+-rw-r--r--   0        0        0     1206 2024-05-29 06:32:39.874887 qctrl_workflow_client-3.1.1/qctrlworkflowclient/router/base.py
+-rw-r--r--   0        0        0     1201 2024-05-29 06:32:39.874887 qctrl_workflow_client-3.1.1/qctrlworkflowclient/router/local.py
+-rw-r--r--   0        0        0     3332 2024-05-29 06:32:39.874887 qctrl_workflow_client-3.1.1/qctrlworkflowclient/settings.py
+-rw-r--r--   0        0        0     5361 2024-05-29 06:32:39.874887 qctrl_workflow_client-3.1.1/qctrlworkflowclient/utils.py
+-rw-r--r--   0        0        0     2489 1970-01-01 00:00:00.000000 qctrl_workflow_client-3.1.1/PKG-INFO
```

### Comparing `qctrl_workflow_client-3.1.0/LICENSE` & `qctrl_workflow_client-3.1.1/LICENSE`

 * *Files identical despite different names*

### Comparing `qctrl_workflow_client-3.1.0/pyproject.toml` & `qctrl_workflow_client-3.1.1/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "qctrl-workflow-client"
-version = "3.1.0"
+version = "3.1.1"
 description = "Q-CTRL Client"
 license = "https://q-ctrl.com/terms"
 authors = ["Q-CTRL <support@q-ctrl.com>"]
 maintainers = ["Q-CTRL <support@q-ctrl.com>"]
 readme = "README.md"
 homepage = "https://q-ctrl.com"
 documentation = "https://docs.q-ctrl.com"
@@ -84,15 +84,15 @@
 qctrl-commons = { version = "^22.0.0", source = "PyPI" }
 qctrl-client = { version = "^9.1.0", source = "PyPI" }
 
 [tool.poetry.group.dev.dependencies]
 black = "^24.3.0"
 isort = "^5.12.0"
 pre-commit = "^3.3.3"
-pylint = "^2.14.4"
+pylint = "^3.2.2"
 pytest = "^7.2.2"
 pytest-cov = "^4.0.0"
 pytest-mock = "^3.10.0"
 pytest-xdist = "^3.2.1"
 qctrl-core-workflow-manager = "^3.2.0"
 
 [tool.isort]
```

### Comparing `qctrl_workflow_client-3.1.0/qctrlworkflowclient/__init__.py` & `qctrl_workflow_client-3.1.1/qctrlworkflowclient/__init__.py`

 * *Files 2% similar despite different names*

```diff
@@ -7,15 +7,15 @@
 #
 #    https://q-ctrl.com/terms
 #
 # Unless required by applicable law or agreed to in writing, software
 # distributed under the License is distributed on an "AS IS" BASIS. See the
 # License for the specific language.
 
-__version__ = "3.1.0"
+__version__ = "3.1.1"
 
 from .defaults import (
     get_authenticated_client_for_product,
     get_default_api_url,
     get_default_cli_auth,
     get_default_oidc_url,
 )
```

### Comparing `qctrl_workflow_client-3.1.0/qctrlworkflowclient/defaults.py` & `qctrl_workflow_client-3.1.1/qctrlworkflowclient/defaults.py`

 * *Files identical despite different names*

### Comparing `qctrl_workflow_client-3.1.0/qctrlworkflowclient/functions.py` & `qctrl_workflow_client-3.1.1/qctrlworkflowclient/functions.py`

 * *Files 5% similar despite different names*

```diff
@@ -18,14 +18,16 @@
     Dict,
     Optional,
 )
 from warnings import warn
 
 from qctrlcommons.exceptions import QctrlArgumentsValueError
 
+from qctrlworkflowclient.router.api import ApiRouter
+
 
 def core_workflow(
     get_config: Callable, workflow: str, formatter: Optional[Callable] = None
 ):
     """
     Decorator for a function which will execute a workflow.
     The decorated function should return the data to be used
@@ -60,15 +62,16 @@
         def customized_decorator(*args, **kwargs):
             # router is instantiated before function is called
             # so any alteration to settings is visible within
             # the function
             config = get_config()
             router = config.get_router()
 
-            router.set_async_state(kwargs.pop("is_async", False))
+            if isinstance(router, ApiRouter):
+                router.set_async_state(kwargs.pop("is_async", False))
 
             data = func(*args, **kwargs)
             result = router(workflow, data)
 
             if formatter:
                 result = formatter(result)
```

### Comparing `qctrl_workflow_client-3.1.0/qctrlworkflowclient/globals.py` & `qctrl_workflow_client-3.1.1/qctrlworkflowclient/globals.py`

 * *Files identical despite different names*

### Comparing `qctrl_workflow_client-3.1.0/qctrlworkflowclient/products.py` & `qctrl_workflow_client-3.1.1/qctrlworkflowclient/products.py`

 * *Files identical despite different names*

### Comparing `qctrl_workflow_client-3.1.0/qctrlworkflowclient/router/__init__.py` & `qctrl_workflow_client-3.1.1/qctrlworkflowclient/router/__init__.py`

 * *Files identical despite different names*

### Comparing `qctrl_workflow_client-3.1.0/qctrlworkflowclient/router/api.py` & `qctrl_workflow_client-3.1.1/qctrlworkflowclient/router/api.py`

 * *Files identical despite different names*

### Comparing `qctrl_workflow_client-3.1.0/qctrlworkflowclient/router/base.py` & `qctrl_workflow_client-3.1.1/qctrlworkflowclient/router/base.py`

 * *Files identical despite different names*

### Comparing `qctrl_workflow_client-3.1.0/qctrlworkflowclient/router/local.py` & `qctrl_workflow_client-3.1.1/qctrlworkflowclient/router/local.py`

 * *Files identical despite different names*

### Comparing `qctrl_workflow_client-3.1.0/qctrlworkflowclient/settings.py` & `qctrl_workflow_client-3.1.1/qctrlworkflowclient/settings.py`

 * *Files identical despite different names*

### Comparing `qctrl_workflow_client-3.1.0/qctrlworkflowclient/utils.py` & `qctrl_workflow_client-3.1.1/qctrlworkflowclient/utils.py`

 * *Files identical despite different names*

### Comparing `qctrl_workflow_client-3.1.0/PKG-INFO` & `qctrl_workflow_client-3.1.1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: qctrl-workflow-client
-Version: 3.1.0
+Version: 3.1.1
 Summary: Q-CTRL Client
 Home-page: https://q-ctrl.com
 License: https://q-ctrl.com/terms
 Keywords: black opal,boulder opal,fire opal,nisq,open controls,q control,q ctrl,q-control,q-ctrl,qcontrol,qctrl,quantum,quantum algorithms,quantum circuits,quantum coding,quantum coding software,quantum computing,quantum control,quantum control software,quantum control theory,quantum engineering,quantum error correction,quantum firmware,quantum fundamentals,quantum sensing,qubit,qudit
 Author: Q-CTRL
 Author-email: support@q-ctrl.com
 Maintainer: Q-CTRL
```

