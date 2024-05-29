# Comparing `tmp/mypy_boto3_athena-1.34.115.tar.gz` & `tmp/mypy-boto3-athena-1.34.23.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "mypy_boto3_athena-1.34.115.tar", last modified: Wed May 29 19:19:45 2024, max compression
+gzip compressed data, was "mypy-boto3-athena-1.34.23.tar", last modified: Fri Jan 19 20:47:10 2024, max compression
```

## Comparing `mypy_boto3_athena-1.34.115.tar` & `mypy-boto3-athena-1.34.23.tar`

### file list

```diff
@@ -1,27 +1,27 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-29 19:19:45.928560 mypy_boto3_athena-1.34.115/
--rw-r--r--   0 runner    (1001) docker     (127)     1070 2024-05-29 19:18:45.000000 mypy_boto3_athena-1.34.115/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)    13464 2024-05-29 19:19:45.928560 mypy_boto3_athena-1.34.115/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)    11911 2024-05-29 19:18:45.000000 mypy_boto3_athena-1.34.115/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-29 19:19:45.928560 mypy_boto3_athena-1.34.115/mypy_boto3_athena/
--rw-r--r--   0 runner    (1001) docker     (127)     1850 2024-05-29 19:18:45.000000 mypy_boto3_athena-1.34.115/mypy_boto3_athena/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1850 2024-05-29 19:18:45.000000 mypy_boto3_athena-1.34.115/mypy_boto3_athena/__init__.pyi
--rw-r--r--   0 runner    (1001) docker     (127)      918 2024-05-29 19:18:45.000000 mypy_boto3_athena-1.34.115/mypy_boto3_athena/__main__.py
--rw-r--r--   0 runner    (1001) docker     (127)    46472 2024-05-29 19:18:46.000000 mypy_boto3_athena-1.34.115/mypy_boto3_athena/client.py
--rw-r--r--   0 runner    (1001) docker     (127)    46469 2024-05-29 19:18:46.000000 mypy_boto3_athena-1.34.115/mypy_boto3_athena/client.pyi
--rw-r--r--   0 runner    (1001) docker     (127)    11384 2024-05-29 19:18:46.000000 mypy_boto3_athena-1.34.115/mypy_boto3_athena/literals.py
--rw-r--r--   0 runner    (1001) docker     (127)    11384 2024-05-29 19:18:46.000000 mypy_boto3_athena-1.34.115/mypy_boto3_athena/literals.pyi
--rw-r--r--   0 runner    (1001) docker     (127)     8363 2024-05-29 19:18:46.000000 mypy_boto3_athena-1.34.115/mypy_boto3_athena/paginator.py
--rw-r--r--   0 runner    (1001) docker     (127)     8355 2024-05-29 19:18:46.000000 mypy_boto3_athena-1.34.115/mypy_boto3_athena/paginator.pyi
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-29 19:18:45.000000 mypy_boto3_athena-1.34.115/mypy_boto3_athena/py.typed
--rw-r--r--   0 runner    (1001) docker     (127)    54982 2024-05-29 19:18:47.000000 mypy_boto3_athena-1.34.115/mypy_boto3_athena/type_defs.py
--rw-r--r--   0 runner    (1001) docker     (127)    54982 2024-05-29 19:18:47.000000 mypy_boto3_athena-1.34.115/mypy_boto3_athena/type_defs.pyi
--rw-r--r--   0 runner    (1001) docker     (127)       63 2024-05-29 19:18:45.000000 mypy_boto3_athena-1.34.115/mypy_boto3_athena/version.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-29 19:19:45.928560 mypy_boto3_athena-1.34.115/mypy_boto3_athena.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)    13464 2024-05-29 19:19:45.000000 mypy_boto3_athena-1.34.115/mypy_boto3_athena.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      661 2024-05-29 19:19:45.000000 mypy_boto3_athena-1.34.115/mypy_boto3_athena.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-29 19:19:45.000000 mypy_boto3_athena-1.34.115/mypy_boto3_athena.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-29 19:19:45.000000 mypy_boto3_athena-1.34.115/mypy_boto3_athena.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (127)       53 2024-05-29 19:19:45.000000 mypy_boto3_athena-1.34.115/mypy_boto3_athena.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       18 2024-05-29 19:19:45.000000 mypy_boto3_athena-1.34.115/mypy_boto3_athena.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-29 19:19:45.928560 mypy_boto3_athena-1.34.115/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)     1969 2024-05-29 19:18:45.000000 mypy_boto3_athena-1.34.115/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-19 20:47:10.595482 mypy-boto3-athena-1.34.23/
+-rw-r--r--   0 runner    (1001) docker     (127)     1070 2024-01-19 20:46:46.000000 mypy-boto3-athena-1.34.23/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)    13461 2024-01-19 20:47:10.595482 mypy-boto3-athena-1.34.23/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)    11910 2024-01-19 20:46:46.000000 mypy-boto3-athena-1.34.23/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-19 20:47:10.595482 mypy-boto3-athena-1.34.23/mypy_boto3_athena/
+-rw-r--r--   0 runner    (1001) docker     (127)     1850 2024-01-19 20:46:46.000000 mypy-boto3-athena-1.34.23/mypy_boto3_athena/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1850 2024-01-19 20:46:46.000000 mypy-boto3-athena-1.34.23/mypy_boto3_athena/__init__.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)      904 2024-01-19 20:46:46.000000 mypy-boto3-athena-1.34.23/mypy_boto3_athena/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    46452 2024-01-19 20:46:47.000000 mypy-boto3-athena-1.34.23/mypy_boto3_athena/client.py
+-rw-r--r--   0 runner    (1001) docker     (127)    46449 2024-01-19 20:46:46.000000 mypy-boto3-athena-1.34.23/mypy_boto3_athena/client.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)    11228 2024-01-19 20:46:47.000000 mypy-boto3-athena-1.34.23/mypy_boto3_athena/literals.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11228 2024-01-19 20:46:47.000000 mypy-boto3-athena-1.34.23/mypy_boto3_athena/literals.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)     8363 2024-01-19 20:46:47.000000 mypy-boto3-athena-1.34.23/mypy_boto3_athena/paginator.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8355 2024-01-19 20:46:47.000000 mypy-boto3-athena-1.34.23/mypy_boto3_athena/paginator.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-01-19 20:46:46.000000 mypy-boto3-athena-1.34.23/mypy_boto3_athena/py.typed
+-rw-r--r--   0 runner    (1001) docker     (127)    53853 2024-01-19 20:46:48.000000 mypy-boto3-athena-1.34.23/mypy_boto3_athena/type_defs.py
+-rw-r--r--   0 runner    (1001) docker     (127)    53853 2024-01-19 20:46:47.000000 mypy-boto3-athena-1.34.23/mypy_boto3_athena/type_defs.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)       62 2024-01-19 20:46:46.000000 mypy-boto3-athena-1.34.23/mypy_boto3_athena/version.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-19 20:47:10.595482 mypy-boto3-athena-1.34.23/mypy_boto3_athena.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)    13461 2024-01-19 20:47:10.000000 mypy-boto3-athena-1.34.23/mypy_boto3_athena.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      661 2024-01-19 20:47:10.000000 mypy-boto3-athena-1.34.23/mypy_boto3_athena.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-01-19 20:47:10.000000 mypy-boto3-athena-1.34.23/mypy_boto3_athena.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-01-19 20:47:10.000000 mypy-boto3-athena-1.34.23/mypy_boto3_athena.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (127)       53 2024-01-19 20:47:10.000000 mypy-boto3-athena-1.34.23/mypy_boto3_athena.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       18 2024-01-19 20:47:10.000000 mypy-boto3-athena-1.34.23/mypy_boto3_athena.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-01-19 20:47:10.595482 mypy-boto3-athena-1.34.23/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)     1983 2024-01-19 20:46:46.000000 mypy-boto3-athena-1.34.23/setup.py
```

### Comparing `mypy_boto3_athena-1.34.115/LICENSE` & `mypy-boto3-athena-1.34.23/LICENSE`

 * *Files identical despite different names*

### Comparing `mypy_boto3_athena-1.34.115/PKG-INFO` & `mypy-boto3-athena-1.34.23/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 Metadata-Version: 2.1
 Name: mypy-boto3-athena
-Version: 1.34.115
-Summary: Type annotations for boto3.Athena 1.34.115 service generated with mypy-boto3-builder 7.24.0
+Version: 1.34.23
+Summary: Type annotations for boto3.Athena 1.34.23 service generated with mypy-boto3-builder 7.23.1
 Home-page: https://github.com/youtype/mypy_boto3_builder
 Author: Vlad Emelianov
 Author-email: vlad.emelianov.nz@gmail.com
 License: MIT License
 Project-URL: Documentation, https://youtype.github.io/boto3_stubs_docs/mypy_boto3_athena/
 Project-URL: Source, https://github.com/youtype/mypy_boto3_builder
 Project-URL: Tracker, https://github.com/youtype/mypy_boto3_builder/issues
@@ -39,24 +39,24 @@
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/mypy-boto3-athena.svg?color=blue)](https://pypi.org/project/mypy-boto3-athena)
 [![Docs](https://img.shields.io/readthedocs/boto3-stubs.svg?color=blue)](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_athena/)
 [![PyPI - Downloads](https://static.pepy.tech/badge/mypy-boto3-athena)](https://pepy.tech/project/mypy-boto3-athena)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
-[boto3.Athena 1.34.115](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/athena.html#Athena)
+[boto3.Athena 1.34.23](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/athena.html#Athena)
 service compatible with [VSCode](https://code.visualstudio.com/),
 [PyCharm](https://www.jetbrains.com/pycharm/),
 [Emacs](https://www.gnu.org/software/emacs/),
 [Sublime Text](https://www.sublimetext.com/),
 [mypy](https://github.com/python/mypy),
 [pyright](https://github.com/microsoft/pyright) and other tools.
 
 Generated by
-[mypy-boto3-builder 7.24.0](https://github.com/youtype/mypy_boto3_builder).
+[mypy-boto3-builder 7.23.1](https://github.com/youtype/mypy_boto3_builder).
 
 More information can be found on
 [boto3-stubs](https://pypi.org/project/boto3-stubs/) page and in
 [mypy-boto3-athena docs](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_athena/).
 
 See how it helps to find and fix potential bugs:
```

### Comparing `mypy_boto3_athena-1.34.115/README.md` & `mypy-boto3-athena-1.34.23/README.md`

 * *Files 0% similar despite different names*

```diff
@@ -6,24 +6,24 @@
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/mypy-boto3-athena.svg?color=blue)](https://pypi.org/project/mypy-boto3-athena)
 [![Docs](https://img.shields.io/readthedocs/boto3-stubs.svg?color=blue)](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_athena/)
 [![PyPI - Downloads](https://static.pepy.tech/badge/mypy-boto3-athena)](https://pepy.tech/project/mypy-boto3-athena)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
-[boto3.Athena 1.34.115](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/athena.html#Athena)
+[boto3.Athena 1.34.23](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/athena.html#Athena)
 service compatible with [VSCode](https://code.visualstudio.com/),
 [PyCharm](https://www.jetbrains.com/pycharm/),
 [Emacs](https://www.gnu.org/software/emacs/),
 [Sublime Text](https://www.sublimetext.com/),
 [mypy](https://github.com/python/mypy),
 [pyright](https://github.com/microsoft/pyright) and other tools.
 
 Generated by
-[mypy-boto3-builder 7.24.0](https://github.com/youtype/mypy_boto3_builder).
+[mypy-boto3-builder 7.23.1](https://github.com/youtype/mypy_boto3_builder).
 
 More information can be found on
 [boto3-stubs](https://pypi.org/project/boto3-stubs/) page and in
 [mypy-boto3-athena docs](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_athena/).
 
 See how it helps to find and fix potential bugs:
```

### Comparing `mypy_boto3_athena-1.34.115/mypy_boto3_athena/__init__.py` & `mypy-boto3-athena-1.34.23/mypy_boto3_athena/__init__.py`

 * *Files identical despite different names*

### Comparing `mypy_boto3_athena-1.34.115/mypy_boto3_athena/__init__.pyi` & `mypy-boto3-athena-1.34.23/mypy_boto3_athena/__init__.pyi`

 * *Files identical despite different names*

### Comparing `mypy_boto3_athena-1.34.115/mypy_boto3_athena/__main__.py` & `mypy-boto3-athena-1.34.23/mypy_boto3_athena/__main__.py`

 * *Files 15% similar despite different names*

```diff
@@ -6,29 +6,28 @@
 
 
 def print_info() -> None:
     """
     Print package info to stdout.
     """
     print(
-        "Type annotations for boto3.Athena 1.34.115\n"
-        "Version:         1.34.115\n"
-        "Builder version: 7.24.0\n"
-        "Docs:            https://youtype.github.io/boto3_stubs_docs/mypy_boto3_athena//\n"
-        "Boto3 docs:      https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/athena.html#Athena\n"
-        "Other services:  https://pypi.org/project/boto3-stubs/\n"
-        "Changelog:       https://github.com/youtype/mypy_boto3_builder/releases"
+        "Type annotations for boto3.Athena 1.34.23\nVersion:         1.34.23\nBuilder version:"
+        " 7.23.1\nDocs:           "
+        " https://youtype.github.io/boto3_stubs_docs/mypy_boto3_athena//\nBoto3 docs:     "
+        " https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/athena.html#Athena\nOther"
+        " services:  https://pypi.org/project/boto3-stubs/\nChangelog:      "
+        " https://github.com/youtype/mypy_boto3_builder/releases"
     )
 
 
 def print_version() -> None:
     """
     Print package version to stdout.
     """
-    print("1.34.115")
+    print("1.34.23")
 
 
 def main() -> None:
     """
     Main CLI entrypoint.
     """
     if "--version" in sys.argv:
```

### Comparing `mypy_boto3_athena-1.34.115/mypy_boto3_athena/client.py` & `mypy-boto3-athena-1.34.23/mypy_boto3_athena/client.py`

 * *Files 0% similar despite different names*

```diff
@@ -36,19 +36,19 @@
     ListTagsForResourcePaginator,
 )
 from .type_defs import (
     BatchGetNamedQueryOutputTypeDef,
     BatchGetPreparedStatementOutputTypeDef,
     BatchGetQueryExecutionOutputTypeDef,
     CalculationConfigurationTypeDef,
-    CapacityAssignmentUnionTypeDef,
+    CapacityAssignmentTypeDef,
     CreateNamedQueryOutputTypeDef,
     CreateNotebookOutputTypeDef,
     CreatePresignedNotebookUrlResponseTypeDef,
-    EngineConfigurationUnionTypeDef,
+    EngineConfigurationTypeDef,
     ExportNotebookOutputTypeDef,
     FilterDefinitionTypeDef,
     GetCalculationExecutionCodeResponseTypeDef,
     GetCalculationExecutionResponseTypeDef,
     GetCalculationExecutionStatusResponseTypeDef,
     GetCapacityAssignmentConfigurationOutputTypeDef,
     GetCapacityReservationOutputTypeDef,
@@ -742,15 +742,15 @@
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_athena/client/#list_work_groups)
         """
 
     def put_capacity_assignment_configuration(
         self,
         *,
         CapacityReservationName: str,
-        CapacityAssignments: Sequence[CapacityAssignmentUnionTypeDef],
+        CapacityAssignments: Sequence[CapacityAssignmentTypeDef],
     ) -> Dict[str, Any]:
         """
         Puts a new capacity assignment configuration for a specified capacity
         reservation.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/athena.html#Athena.Client.put_capacity_assignment_configuration)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_athena/client/#put_capacity_assignment_configuration)
@@ -790,15 +790,15 @@
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_athena/client/#start_query_execution)
         """
 
     def start_session(
         self,
         *,
         WorkGroup: str,
-        EngineConfiguration: EngineConfigurationUnionTypeDef,
+        EngineConfiguration: EngineConfigurationTypeDef,
         Description: str = ...,
         NotebookVersion: str = ...,
         SessionIdleTimeoutInMinutes: int = ...,
         ClientRequestToken: str = ...,
     ) -> StartSessionResponseTypeDef:
         """
         Creates a session for running calculations within a workgroup.
```

### Comparing `mypy_boto3_athena-1.34.115/mypy_boto3_athena/client.pyi` & `mypy-boto3-athena-1.34.23/mypy_boto3_athena/client.pyi`

 * *Files 0% similar despite different names*

```diff
@@ -36,19 +36,19 @@
     ListTagsForResourcePaginator,
 )
 from .type_defs import (
     BatchGetNamedQueryOutputTypeDef,
     BatchGetPreparedStatementOutputTypeDef,
     BatchGetQueryExecutionOutputTypeDef,
     CalculationConfigurationTypeDef,
-    CapacityAssignmentUnionTypeDef,
+    CapacityAssignmentTypeDef,
     CreateNamedQueryOutputTypeDef,
     CreateNotebookOutputTypeDef,
     CreatePresignedNotebookUrlResponseTypeDef,
-    EngineConfigurationUnionTypeDef,
+    EngineConfigurationTypeDef,
     ExportNotebookOutputTypeDef,
     FilterDefinitionTypeDef,
     GetCalculationExecutionCodeResponseTypeDef,
     GetCalculationExecutionResponseTypeDef,
     GetCalculationExecutionStatusResponseTypeDef,
     GetCapacityAssignmentConfigurationOutputTypeDef,
     GetCapacityReservationOutputTypeDef,
@@ -739,15 +739,15 @@
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_athena/client/#list_work_groups)
         """
 
     def put_capacity_assignment_configuration(
         self,
         *,
         CapacityReservationName: str,
-        CapacityAssignments: Sequence[CapacityAssignmentUnionTypeDef],
+        CapacityAssignments: Sequence[CapacityAssignmentTypeDef],
     ) -> Dict[str, Any]:
         """
         Puts a new capacity assignment configuration for a specified capacity
         reservation.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/athena.html#Athena.Client.put_capacity_assignment_configuration)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_athena/client/#put_capacity_assignment_configuration)
@@ -787,15 +787,15 @@
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_athena/client/#start_query_execution)
         """
 
     def start_session(
         self,
         *,
         WorkGroup: str,
-        EngineConfiguration: EngineConfigurationUnionTypeDef,
+        EngineConfiguration: EngineConfigurationTypeDef,
         Description: str = ...,
         NotebookVersion: str = ...,
         SessionIdleTimeoutInMinutes: int = ...,
         ClientRequestToken: str = ...,
     ) -> StartSessionResponseTypeDef:
         """
         Creates a session for running calculations within a workgroup.
```

### Comparing `mypy_boto3_athena-1.34.115/mypy_boto3_athena/literals.py` & `mypy-boto3-athena-1.34.23/mypy_boto3_athena/literals.py`

 * *Files 10% similar despite different names*

```diff
@@ -102,15 +102,14 @@
     "application-insights",
     "applicationcostprofiler",
     "appmesh",
     "apprunner",
     "appstream",
     "appsync",
     "arc-zonal-shift",
-    "artifact",
     "athena",
     "auditmanager",
     "autoscaling",
     "autoscaling-plans",
     "b2bi",
     "backup",
     "backup-gateway",
@@ -121,15 +120,14 @@
     "bedrock-agent",
     "bedrock-agent-runtime",
     "bedrock-runtime",
     "billingconductor",
     "braket",
     "budgets",
     "ce",
-    "chatbot",
     "chime",
     "chime-sdk-identity",
     "chime-sdk-media-pipelines",
     "chime-sdk-meetings",
     "chime-sdk-messaging",
     "chime-sdk-voice",
     "cleanrooms",
@@ -147,15 +145,14 @@
     "cloudtrail",
     "cloudtrail-data",
     "cloudwatch",
     "codeartifact",
     "codebuild",
     "codecatalyst",
     "codecommit",
-    "codeconnections",
     "codedeploy",
     "codeguru-reviewer",
     "codeguru-security",
     "codeguruprofiler",
     "codepipeline",
     "codestar",
     "codestar-connections",
@@ -168,26 +165,24 @@
     "compute-optimizer",
     "config",
     "connect",
     "connect-contact-lens",
     "connectcampaigns",
     "connectcases",
     "connectparticipant",
-    "controlcatalog",
     "controltower",
     "cost-optimization-hub",
     "cur",
     "customer-profiles",
     "databrew",
     "dataexchange",
     "datapipeline",
     "datasync",
     "datazone",
     "dax",
-    "deadline",
     "detective",
     "devicefarm",
     "devops-guru",
     "directconnect",
     "discovery",
     "dlm",
     "dms",
@@ -248,14 +243,15 @@
     "inspector",
     "inspector-scan",
     "inspector2",
     "internetmonitor",
     "iot",
     "iot-data",
     "iot-jobs-data",
+    "iot-roborunner",
     "iot1click-devices",
     "iot1click-projects",
     "iotanalytics",
     "iotdeviceadvisor",
     "iotevents",
     "iotevents-data",
     "iotfleethub",
@@ -297,15 +293,14 @@
     "logs",
     "lookoutequipment",
     "lookoutmetrics",
     "lookoutvision",
     "m2",
     "machinelearning",
     "macie2",
-    "mailmanager",
     "managedblockchain",
     "managedblockchain-query",
     "marketplace-agreement",
     "marketplace-catalog",
     "marketplace-deployment",
     "marketplace-entitlement",
     "marketplacecommerceanalytics",
@@ -385,15 +380,14 @@
     "robomaker",
     "rolesanywhere",
     "route53",
     "route53-recovery-cluster",
     "route53-recovery-control-config",
     "route53-recovery-readiness",
     "route53domains",
-    "route53profiles",
     "route53resolver",
     "rum",
     "s3",
     "s3control",
     "s3outposts",
     "sagemaker",
     "sagemaker-a2i-runtime",
@@ -437,15 +431,14 @@
     "sts",
     "supplychain",
     "support",
     "support-app",
     "swf",
     "synthetics",
     "textract",
-    "timestream-influxdb",
     "timestream-query",
     "timestream-write",
     "tnb",
     "transcribe",
     "transfer",
     "translate",
     "trustedadvisor",
@@ -496,15 +489,14 @@
     "ap-south-1",
     "ap-south-2",
     "ap-southeast-1",
     "ap-southeast-2",
     "ap-southeast-3",
     "ap-southeast-4",
     "ca-central-1",
-    "ca-west-1",
     "eu-central-1",
     "eu-central-2",
     "eu-north-1",
     "eu-south-1",
     "eu-south-2",
     "eu-west-1",
     "eu-west-2",
```

### Comparing `mypy_boto3_athena-1.34.115/mypy_boto3_athena/literals.pyi` & `mypy-boto3-athena-1.34.23/mypy_boto3_athena/literals.pyi`

 * *Files 10% similar despite different names*

```diff
@@ -102,15 +102,14 @@
     "application-insights",
     "applicationcostprofiler",
     "appmesh",
     "apprunner",
     "appstream",
     "appsync",
     "arc-zonal-shift",
-    "artifact",
     "athena",
     "auditmanager",
     "autoscaling",
     "autoscaling-plans",
     "b2bi",
     "backup",
     "backup-gateway",
@@ -121,15 +120,14 @@
     "bedrock-agent",
     "bedrock-agent-runtime",
     "bedrock-runtime",
     "billingconductor",
     "braket",
     "budgets",
     "ce",
-    "chatbot",
     "chime",
     "chime-sdk-identity",
     "chime-sdk-media-pipelines",
     "chime-sdk-meetings",
     "chime-sdk-messaging",
     "chime-sdk-voice",
     "cleanrooms",
@@ -147,15 +145,14 @@
     "cloudtrail",
     "cloudtrail-data",
     "cloudwatch",
     "codeartifact",
     "codebuild",
     "codecatalyst",
     "codecommit",
-    "codeconnections",
     "codedeploy",
     "codeguru-reviewer",
     "codeguru-security",
     "codeguruprofiler",
     "codepipeline",
     "codestar",
     "codestar-connections",
@@ -168,26 +165,24 @@
     "compute-optimizer",
     "config",
     "connect",
     "connect-contact-lens",
     "connectcampaigns",
     "connectcases",
     "connectparticipant",
-    "controlcatalog",
     "controltower",
     "cost-optimization-hub",
     "cur",
     "customer-profiles",
     "databrew",
     "dataexchange",
     "datapipeline",
     "datasync",
     "datazone",
     "dax",
-    "deadline",
     "detective",
     "devicefarm",
     "devops-guru",
     "directconnect",
     "discovery",
     "dlm",
     "dms",
@@ -248,14 +243,15 @@
     "inspector",
     "inspector-scan",
     "inspector2",
     "internetmonitor",
     "iot",
     "iot-data",
     "iot-jobs-data",
+    "iot-roborunner",
     "iot1click-devices",
     "iot1click-projects",
     "iotanalytics",
     "iotdeviceadvisor",
     "iotevents",
     "iotevents-data",
     "iotfleethub",
@@ -297,15 +293,14 @@
     "logs",
     "lookoutequipment",
     "lookoutmetrics",
     "lookoutvision",
     "m2",
     "machinelearning",
     "macie2",
-    "mailmanager",
     "managedblockchain",
     "managedblockchain-query",
     "marketplace-agreement",
     "marketplace-catalog",
     "marketplace-deployment",
     "marketplace-entitlement",
     "marketplacecommerceanalytics",
@@ -385,15 +380,14 @@
     "robomaker",
     "rolesanywhere",
     "route53",
     "route53-recovery-cluster",
     "route53-recovery-control-config",
     "route53-recovery-readiness",
     "route53domains",
-    "route53profiles",
     "route53resolver",
     "rum",
     "s3",
     "s3control",
     "s3outposts",
     "sagemaker",
     "sagemaker-a2i-runtime",
@@ -437,15 +431,14 @@
     "sts",
     "supplychain",
     "support",
     "support-app",
     "swf",
     "synthetics",
     "textract",
-    "timestream-influxdb",
     "timestream-query",
     "timestream-write",
     "tnb",
     "transcribe",
     "transfer",
     "translate",
     "trustedadvisor",
@@ -496,15 +489,14 @@
     "ap-south-1",
     "ap-south-2",
     "ap-southeast-1",
     "ap-southeast-2",
     "ap-southeast-3",
     "ap-southeast-4",
     "ca-central-1",
-    "ca-west-1",
     "eu-central-1",
     "eu-central-2",
     "eu-north-1",
     "eu-south-1",
     "eu-south-2",
     "eu-west-1",
     "eu-west-2",
```

### Comparing `mypy_boto3_athena-1.34.115/mypy_boto3_athena/paginator.py` & `mypy-boto3-athena-1.34.23/mypy_boto3_athena/paginator.py`

 * *Files identical despite different names*

### Comparing `mypy_boto3_athena-1.34.115/mypy_boto3_athena/paginator.pyi` & `mypy-boto3-athena-1.34.23/mypy_boto3_athena/paginator.pyi`

 * *Files identical despite different names*

### Comparing `mypy_boto3_athena-1.34.115/mypy_boto3_athena/type_defs.py` & `mypy-boto3-athena-1.34.23/mypy_boto3_athena/type_defs.py`

 * *Files 1% similar despite different names*

```diff
@@ -10,15 +10,15 @@
 
     data: AclConfigurationTypeDef = ...
     ```
 """
 
 import sys
 from datetime import datetime
-from typing import Any, Dict, List, Mapping, Sequence, Union
+from typing import Any, Dict, List, Mapping, Sequence
 
 from .literals import (
     CalculationExecutionStateType,
     CapacityAllocationStatusType,
     CapacityReservationStatusType,
     ColumnNullableType,
     DataCatalogTypeType,
@@ -59,15 +59,14 @@
     "UnprocessedQueryExecutionIdTypeDef",
     "CalculationConfigurationTypeDef",
     "CalculationResultTypeDef",
     "CalculationStatisticsTypeDef",
     "CalculationStatusTypeDef",
     "CancelCapacityReservationInputRequestTypeDef",
     "CapacityAllocationTypeDef",
-    "CapacityAssignmentOutputTypeDef",
     "CapacityAssignmentTypeDef",
     "ColumnInfoTypeDef",
     "ColumnTypeDef",
     "TagTypeDef",
     "CreateNamedQueryInputRequestTypeDef",
     "CreateNotebookInputRequestTypeDef",
     "CreatePreparedStatementInputRequestTypeDef",
@@ -80,15 +79,14 @@
     "DeleteCapacityReservationInputRequestTypeDef",
     "DeleteDataCatalogInputRequestTypeDef",
     "DeleteNamedQueryInputRequestTypeDef",
     "DeleteNotebookInputRequestTypeDef",
     "DeletePreparedStatementInputRequestTypeDef",
     "DeleteWorkGroupInputRequestTypeDef",
     "EncryptionConfigurationTypeDef",
-    "EngineConfigurationOutputTypeDef",
     "EngineConfigurationTypeDef",
     "EngineVersionTypeDef",
     "ExecutorsSummaryTypeDef",
     "ExportNotebookInputRequestTypeDef",
     "NotebookMetadataTypeDef",
     "FilterDefinitionTypeDef",
     "GetCalculationExecutionCodeRequestRequestTypeDef",
@@ -168,30 +166,29 @@
     "BatchGetPreparedStatementOutputTypeDef",
     "StartCalculationExecutionRequestRequestTypeDef",
     "CalculationSummaryTypeDef",
     "GetCalculationExecutionResponseTypeDef",
     "GetCalculationExecutionStatusResponseTypeDef",
     "CapacityReservationTypeDef",
     "CapacityAssignmentConfigurationTypeDef",
-    "CapacityAssignmentUnionTypeDef",
+    "PutCapacityAssignmentConfigurationInputRequestTypeDef",
     "ResultSetMetadataTypeDef",
     "TableMetadataTypeDef",
     "CreateCapacityReservationInputRequestTypeDef",
     "CreateDataCatalogInputRequestTypeDef",
     "ListTagsForResourceOutputTypeDef",
     "TagResourceInputRequestTypeDef",
     "ListDataCatalogsOutputTypeDef",
     "GetDataCatalogOutputTypeDef",
     "GetDatabaseOutputTypeDef",
     "ListDatabasesOutputTypeDef",
     "RowTypeDef",
     "ResultConfigurationTypeDef",
     "ResultConfigurationUpdatesTypeDef",
     "SessionConfigurationTypeDef",
-    "EngineConfigurationUnionTypeDef",
     "StartSessionRequestRequestTypeDef",
     "ListEngineVersionsOutputTypeDef",
     "WorkGroupSummaryTypeDef",
     "ListExecutorsResponseTypeDef",
     "ExportNotebookOutputTypeDef",
     "GetNotebookMetadataOutputTypeDef",
     "ListNotebookMetadataOutputTypeDef",
@@ -210,15 +207,14 @@
     "QueryExecutionStatisticsTypeDef",
     "QueryRuntimeStatisticsTypeDef",
     "ResultReuseConfigurationTypeDef",
     "ListCalculationExecutionsResponseTypeDef",
     "GetCapacityReservationOutputTypeDef",
     "ListCapacityReservationsOutputTypeDef",
     "GetCapacityAssignmentConfigurationOutputTypeDef",
-    "PutCapacityAssignmentConfigurationInputRequestTypeDef",
     "GetTableMetadataOutputTypeDef",
     "ListTableMetadataOutputTypeDef",
     "ResultSetTypeDef",
     "WorkGroupConfigurationTypeDef",
     "WorkGroupConfigurationUpdatesTypeDef",
     "GetSessionResponseTypeDef",
     "ListWorkGroupsOutputTypeDef",
@@ -274,18 +270,18 @@
         "WorkGroup": NotRequired[str],
     },
 )
 ResponseMetadataTypeDef = TypedDict(
     "ResponseMetadataTypeDef",
     {
         "RequestId": str,
+        "HostId": str,
         "HTTPStatusCode": int,
         "HTTPHeaders": Dict[str, str],
         "RetryAttempts": int,
-        "HostId": NotRequired[str],
     },
 )
 UnprocessedNamedQueryIdTypeDef = TypedDict(
     "UnprocessedNamedQueryIdTypeDef",
     {
         "NamedQueryId": NotRequired[str],
         "ErrorCode": NotRequired[str],
@@ -373,24 +369,18 @@
     {
         "Status": CapacityAllocationStatusType,
         "RequestTime": datetime,
         "StatusMessage": NotRequired[str],
         "RequestCompletionTime": NotRequired[datetime],
     },
 )
-CapacityAssignmentOutputTypeDef = TypedDict(
-    "CapacityAssignmentOutputTypeDef",
-    {
-        "WorkGroupNames": NotRequired[List[str]],
-    },
-)
 CapacityAssignmentTypeDef = TypedDict(
     "CapacityAssignmentTypeDef",
     {
-        "WorkGroupNames": NotRequired[Sequence[str]],
+        "WorkGroupNames": NotRequired[List[str]],
     },
 )
 ColumnInfoTypeDef = TypedDict(
     "ColumnInfoTypeDef",
     {
         "Name": str,
         "Type": str,
@@ -530,32 +520,22 @@
 EncryptionConfigurationTypeDef = TypedDict(
     "EncryptionConfigurationTypeDef",
     {
         "EncryptionOption": EncryptionOptionType,
         "KmsKey": NotRequired[str],
     },
 )
-EngineConfigurationOutputTypeDef = TypedDict(
-    "EngineConfigurationOutputTypeDef",
-    {
-        "MaxConcurrentDpus": int,
-        "CoordinatorDpuSize": NotRequired[int],
-        "DefaultExecutorDpuSize": NotRequired[int],
-        "AdditionalConfigs": NotRequired[Dict[str, str]],
-        "SparkProperties": NotRequired[Dict[str, str]],
-    },
-)
 EngineConfigurationTypeDef = TypedDict(
     "EngineConfigurationTypeDef",
     {
         "MaxConcurrentDpus": int,
         "CoordinatorDpuSize": NotRequired[int],
         "DefaultExecutorDpuSize": NotRequired[int],
-        "AdditionalConfigs": NotRequired[Mapping[str, str]],
-        "SparkProperties": NotRequired[Mapping[str, str]],
+        "AdditionalConfigs": NotRequired[Dict[str, str]],
+        "SparkProperties": NotRequired[Dict[str, str]],
     },
 )
 EngineVersionTypeDef = TypedDict(
     "EngineVersionTypeDef",
     {
         "SelectedEngineVersion": NotRequired[str],
         "EffectiveEngineVersion": NotRequired[str],
@@ -1088,32 +1068,32 @@
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 ListApplicationDPUSizesOutputTypeDef = TypedDict(
     "ListApplicationDPUSizesOutputTypeDef",
     {
         "ApplicationDPUSizes": List[ApplicationDPUSizesTypeDef],
+        "NextToken": str,
         "ResponseMetadata": ResponseMetadataTypeDef,
-        "NextToken": NotRequired[str],
     },
 )
 ListNamedQueriesOutputTypeDef = TypedDict(
     "ListNamedQueriesOutputTypeDef",
     {
         "NamedQueryIds": List[str],
+        "NextToken": str,
         "ResponseMetadata": ResponseMetadataTypeDef,
-        "NextToken": NotRequired[str],
     },
 )
 ListQueryExecutionsOutputTypeDef = TypedDict(
     "ListQueryExecutionsOutputTypeDef",
     {
         "QueryExecutionIds": List[str],
+        "NextToken": str,
         "ResponseMetadata": ResponseMetadataTypeDef,
-        "NextToken": NotRequired[str],
     },
 )
 StartCalculationExecutionResponseTypeDef = TypedDict(
     "StartCalculationExecutionResponseTypeDef",
     {
         "CalculationExecutionId": str,
         "State": CalculationExecutionStateType,
@@ -1223,18 +1203,24 @@
         "LastSuccessfulAllocationTime": NotRequired[datetime],
     },
 )
 CapacityAssignmentConfigurationTypeDef = TypedDict(
     "CapacityAssignmentConfigurationTypeDef",
     {
         "CapacityReservationName": NotRequired[str],
-        "CapacityAssignments": NotRequired[List[CapacityAssignmentOutputTypeDef]],
+        "CapacityAssignments": NotRequired[List[CapacityAssignmentTypeDef]],
+    },
+)
+PutCapacityAssignmentConfigurationInputRequestTypeDef = TypedDict(
+    "PutCapacityAssignmentConfigurationInputRequestTypeDef",
+    {
+        "CapacityReservationName": str,
+        "CapacityAssignments": Sequence[CapacityAssignmentTypeDef],
     },
 )
-CapacityAssignmentUnionTypeDef = Union[CapacityAssignmentTypeDef, CapacityAssignmentOutputTypeDef]
 ResultSetMetadataTypeDef = TypedDict(
     "ResultSetMetadataTypeDef",
     {
         "ColumnInfo": NotRequired[List[ColumnInfoTypeDef]],
     },
 )
 TableMetadataTypeDef = TypedDict(
@@ -1267,31 +1253,31 @@
         "Tags": NotRequired[Sequence[TagTypeDef]],
     },
 )
 ListTagsForResourceOutputTypeDef = TypedDict(
     "ListTagsForResourceOutputTypeDef",
     {
         "Tags": List[TagTypeDef],
+        "NextToken": str,
         "ResponseMetadata": ResponseMetadataTypeDef,
-        "NextToken": NotRequired[str],
     },
 )
 TagResourceInputRequestTypeDef = TypedDict(
     "TagResourceInputRequestTypeDef",
     {
         "ResourceARN": str,
         "Tags": Sequence[TagTypeDef],
     },
 )
 ListDataCatalogsOutputTypeDef = TypedDict(
     "ListDataCatalogsOutputTypeDef",
     {
         "DataCatalogsSummary": List[DataCatalogSummaryTypeDef],
+        "NextToken": str,
         "ResponseMetadata": ResponseMetadataTypeDef,
-        "NextToken": NotRequired[str],
     },
 )
 GetDataCatalogOutputTypeDef = TypedDict(
     "GetDataCatalogOutputTypeDef",
     {
         "DataCatalog": DataCatalogTypeDef,
         "ResponseMetadata": ResponseMetadataTypeDef,
@@ -1304,16 +1290,16 @@
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 ListDatabasesOutputTypeDef = TypedDict(
     "ListDatabasesOutputTypeDef",
     {
         "DatabaseList": List[DatabaseTypeDef],
+        "NextToken": str,
         "ResponseMetadata": ResponseMetadataTypeDef,
-        "NextToken": NotRequired[str],
     },
 )
 RowTypeDef = TypedDict(
     "RowTypeDef",
     {
         "Data": NotRequired[List[DatumTypeDef]],
     },
@@ -1345,17 +1331,14 @@
     {
         "ExecutionRole": NotRequired[str],
         "WorkingDirectory": NotRequired[str],
         "IdleTimeoutSeconds": NotRequired[int],
         "EncryptionConfiguration": NotRequired[EncryptionConfigurationTypeDef],
     },
 )
-EngineConfigurationUnionTypeDef = Union[
-    EngineConfigurationTypeDef, EngineConfigurationOutputTypeDef
-]
 StartSessionRequestRequestTypeDef = TypedDict(
     "StartSessionRequestRequestTypeDef",
     {
         "WorkGroup": str,
         "EngineConfiguration": EngineConfigurationTypeDef,
         "Description": NotRequired[str],
         "NotebookVersion": NotRequired[str],
@@ -1363,16 +1346,16 @@
         "ClientRequestToken": NotRequired[str],
     },
 )
 ListEngineVersionsOutputTypeDef = TypedDict(
     "ListEngineVersionsOutputTypeDef",
     {
         "EngineVersions": List[EngineVersionTypeDef],
+        "NextToken": str,
         "ResponseMetadata": ResponseMetadataTypeDef,
-        "NextToken": NotRequired[str],
     },
 )
 WorkGroupSummaryTypeDef = TypedDict(
     "WorkGroupSummaryTypeDef",
     {
         "Name": NotRequired[str],
         "State": NotRequired[WorkGroupStateType],
@@ -1382,17 +1365,17 @@
         "IdentityCenterApplicationArn": NotRequired[str],
     },
 )
 ListExecutorsResponseTypeDef = TypedDict(
     "ListExecutorsResponseTypeDef",
     {
         "SessionId": str,
+        "NextToken": str,
         "ExecutorsSummary": List[ExecutorsSummaryTypeDef],
         "ResponseMetadata": ResponseMetadataTypeDef,
-        "NextToken": NotRequired[str],
     },
 )
 ExportNotebookOutputTypeDef = TypedDict(
     "ExportNotebookOutputTypeDef",
     {
         "NotebookMetadata": NotebookMetadataTypeDef,
         "Payload": str,
@@ -1405,17 +1388,17 @@
         "NotebookMetadata": NotebookMetadataTypeDef,
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 ListNotebookMetadataOutputTypeDef = TypedDict(
     "ListNotebookMetadataOutputTypeDef",
     {
+        "NextToken": str,
         "NotebookMetadataList": List[NotebookMetadataTypeDef],
         "ResponseMetadata": ResponseMetadataTypeDef,
-        "NextToken": NotRequired[str],
     },
 )
 ListNotebookMetadataInputRequestTypeDef = TypedDict(
     "ListNotebookMetadataInputRequestTypeDef",
     {
         "WorkGroup": str,
         "Filters": NotRequired[FilterDefinitionTypeDef],
@@ -1494,24 +1477,24 @@
         "Status": NotRequired[SessionStatusTypeDef],
     },
 )
 ListNotebookSessionsResponseTypeDef = TypedDict(
     "ListNotebookSessionsResponseTypeDef",
     {
         "NotebookSessionsList": List[NotebookSessionSummaryTypeDef],
+        "NextToken": str,
         "ResponseMetadata": ResponseMetadataTypeDef,
-        "NextToken": NotRequired[str],
     },
 )
 ListPreparedStatementsOutputTypeDef = TypedDict(
     "ListPreparedStatementsOutputTypeDef",
     {
         "PreparedStatements": List[PreparedStatementSummaryTypeDef],
+        "NextToken": str,
         "ResponseMetadata": ResponseMetadataTypeDef,
-        "NextToken": NotRequired[str],
     },
 )
 QueryExecutionStatisticsTypeDef = TypedDict(
     "QueryExecutionStatisticsTypeDef",
     {
         "EngineExecutionTimeInMillis": NotRequired[int],
         "DataScannedInBytes": NotRequired[int],
@@ -1537,61 +1520,54 @@
     {
         "ResultReuseByAgeConfiguration": NotRequired[ResultReuseByAgeConfigurationTypeDef],
     },
 )
 ListCalculationExecutionsResponseTypeDef = TypedDict(
     "ListCalculationExecutionsResponseTypeDef",
     {
+        "NextToken": str,
         "Calculations": List[CalculationSummaryTypeDef],
         "ResponseMetadata": ResponseMetadataTypeDef,
-        "NextToken": NotRequired[str],
     },
 )
 GetCapacityReservationOutputTypeDef = TypedDict(
     "GetCapacityReservationOutputTypeDef",
     {
         "CapacityReservation": CapacityReservationTypeDef,
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 ListCapacityReservationsOutputTypeDef = TypedDict(
     "ListCapacityReservationsOutputTypeDef",
     {
+        "NextToken": str,
         "CapacityReservations": List[CapacityReservationTypeDef],
         "ResponseMetadata": ResponseMetadataTypeDef,
-        "NextToken": NotRequired[str],
     },
 )
 GetCapacityAssignmentConfigurationOutputTypeDef = TypedDict(
     "GetCapacityAssignmentConfigurationOutputTypeDef",
     {
         "CapacityAssignmentConfiguration": CapacityAssignmentConfigurationTypeDef,
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
-PutCapacityAssignmentConfigurationInputRequestTypeDef = TypedDict(
-    "PutCapacityAssignmentConfigurationInputRequestTypeDef",
-    {
-        "CapacityReservationName": str,
-        "CapacityAssignments": Sequence[CapacityAssignmentUnionTypeDef],
-    },
-)
 GetTableMetadataOutputTypeDef = TypedDict(
     "GetTableMetadataOutputTypeDef",
     {
         "TableMetadata": TableMetadataTypeDef,
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 ListTableMetadataOutputTypeDef = TypedDict(
     "ListTableMetadataOutputTypeDef",
     {
         "TableMetadataList": List[TableMetadataTypeDef],
+        "NextToken": str,
         "ResponseMetadata": ResponseMetadataTypeDef,
-        "NextToken": NotRequired[str],
     },
 )
 ResultSetTypeDef = TypedDict(
     "ResultSetTypeDef",
     {
         "Rows": NotRequired[List[RowTypeDef]],
         "ResultSetMetadata": NotRequired[ResultSetMetadataTypeDef],
@@ -1643,36 +1619,36 @@
 GetSessionResponseTypeDef = TypedDict(
     "GetSessionResponseTypeDef",
     {
         "SessionId": str,
         "Description": str,
         "WorkGroup": str,
         "EngineVersion": str,
-        "EngineConfiguration": EngineConfigurationOutputTypeDef,
+        "EngineConfiguration": EngineConfigurationTypeDef,
         "NotebookVersion": str,
         "SessionConfiguration": SessionConfigurationTypeDef,
         "Status": SessionStatusTypeDef,
         "Statistics": SessionStatisticsTypeDef,
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 ListWorkGroupsOutputTypeDef = TypedDict(
     "ListWorkGroupsOutputTypeDef",
     {
         "WorkGroups": List[WorkGroupSummaryTypeDef],
+        "NextToken": str,
         "ResponseMetadata": ResponseMetadataTypeDef,
-        "NextToken": NotRequired[str],
     },
 )
 ListSessionsResponseTypeDef = TypedDict(
     "ListSessionsResponseTypeDef",
     {
+        "NextToken": str,
         "Sessions": List[SessionSummaryTypeDef],
         "ResponseMetadata": ResponseMetadataTypeDef,
-        "NextToken": NotRequired[str],
     },
 )
 GetQueryRuntimeStatisticsOutputTypeDef = TypedDict(
     "GetQueryRuntimeStatisticsOutputTypeDef",
     {
         "QueryRuntimeStatistics": QueryRuntimeStatisticsTypeDef,
         "ResponseMetadata": ResponseMetadataTypeDef,
@@ -1711,16 +1687,16 @@
     },
 )
 GetQueryResultsOutputTypeDef = TypedDict(
     "GetQueryResultsOutputTypeDef",
     {
         "UpdateCount": int,
         "ResultSet": ResultSetTypeDef,
+        "NextToken": str,
         "ResponseMetadata": ResponseMetadataTypeDef,
-        "NextToken": NotRequired[str],
     },
 )
 CreateWorkGroupInputRequestTypeDef = TypedDict(
     "CreateWorkGroupInputRequestTypeDef",
     {
         "Name": str,
         "Configuration": NotRequired[WorkGroupConfigurationTypeDef],
```

### Comparing `mypy_boto3_athena-1.34.115/mypy_boto3_athena/type_defs.pyi` & `mypy-boto3-athena-1.34.23/mypy_boto3_athena/type_defs.pyi`

 * *Files 1% similar despite different names*

```diff
@@ -10,15 +10,15 @@
 
     data: AclConfigurationTypeDef = ...
     ```
 """
 
 import sys
 from datetime import datetime
-from typing import Any, Dict, List, Mapping, Sequence, Union
+from typing import Any, Dict, List, Mapping, Sequence
 
 from .literals import (
     CalculationExecutionStateType,
     CapacityAllocationStatusType,
     CapacityReservationStatusType,
     ColumnNullableType,
     DataCatalogTypeType,
@@ -59,15 +59,14 @@
     "UnprocessedQueryExecutionIdTypeDef",
     "CalculationConfigurationTypeDef",
     "CalculationResultTypeDef",
     "CalculationStatisticsTypeDef",
     "CalculationStatusTypeDef",
     "CancelCapacityReservationInputRequestTypeDef",
     "CapacityAllocationTypeDef",
-    "CapacityAssignmentOutputTypeDef",
     "CapacityAssignmentTypeDef",
     "ColumnInfoTypeDef",
     "ColumnTypeDef",
     "TagTypeDef",
     "CreateNamedQueryInputRequestTypeDef",
     "CreateNotebookInputRequestTypeDef",
     "CreatePreparedStatementInputRequestTypeDef",
@@ -80,15 +79,14 @@
     "DeleteCapacityReservationInputRequestTypeDef",
     "DeleteDataCatalogInputRequestTypeDef",
     "DeleteNamedQueryInputRequestTypeDef",
     "DeleteNotebookInputRequestTypeDef",
     "DeletePreparedStatementInputRequestTypeDef",
     "DeleteWorkGroupInputRequestTypeDef",
     "EncryptionConfigurationTypeDef",
-    "EngineConfigurationOutputTypeDef",
     "EngineConfigurationTypeDef",
     "EngineVersionTypeDef",
     "ExecutorsSummaryTypeDef",
     "ExportNotebookInputRequestTypeDef",
     "NotebookMetadataTypeDef",
     "FilterDefinitionTypeDef",
     "GetCalculationExecutionCodeRequestRequestTypeDef",
@@ -168,30 +166,29 @@
     "BatchGetPreparedStatementOutputTypeDef",
     "StartCalculationExecutionRequestRequestTypeDef",
     "CalculationSummaryTypeDef",
     "GetCalculationExecutionResponseTypeDef",
     "GetCalculationExecutionStatusResponseTypeDef",
     "CapacityReservationTypeDef",
     "CapacityAssignmentConfigurationTypeDef",
-    "CapacityAssignmentUnionTypeDef",
+    "PutCapacityAssignmentConfigurationInputRequestTypeDef",
     "ResultSetMetadataTypeDef",
     "TableMetadataTypeDef",
     "CreateCapacityReservationInputRequestTypeDef",
     "CreateDataCatalogInputRequestTypeDef",
     "ListTagsForResourceOutputTypeDef",
     "TagResourceInputRequestTypeDef",
     "ListDataCatalogsOutputTypeDef",
     "GetDataCatalogOutputTypeDef",
     "GetDatabaseOutputTypeDef",
     "ListDatabasesOutputTypeDef",
     "RowTypeDef",
     "ResultConfigurationTypeDef",
     "ResultConfigurationUpdatesTypeDef",
     "SessionConfigurationTypeDef",
-    "EngineConfigurationUnionTypeDef",
     "StartSessionRequestRequestTypeDef",
     "ListEngineVersionsOutputTypeDef",
     "WorkGroupSummaryTypeDef",
     "ListExecutorsResponseTypeDef",
     "ExportNotebookOutputTypeDef",
     "GetNotebookMetadataOutputTypeDef",
     "ListNotebookMetadataOutputTypeDef",
@@ -210,15 +207,14 @@
     "QueryExecutionStatisticsTypeDef",
     "QueryRuntimeStatisticsTypeDef",
     "ResultReuseConfigurationTypeDef",
     "ListCalculationExecutionsResponseTypeDef",
     "GetCapacityReservationOutputTypeDef",
     "ListCapacityReservationsOutputTypeDef",
     "GetCapacityAssignmentConfigurationOutputTypeDef",
-    "PutCapacityAssignmentConfigurationInputRequestTypeDef",
     "GetTableMetadataOutputTypeDef",
     "ListTableMetadataOutputTypeDef",
     "ResultSetTypeDef",
     "WorkGroupConfigurationTypeDef",
     "WorkGroupConfigurationUpdatesTypeDef",
     "GetSessionResponseTypeDef",
     "ListWorkGroupsOutputTypeDef",
@@ -274,18 +270,18 @@
         "WorkGroup": NotRequired[str],
     },
 )
 ResponseMetadataTypeDef = TypedDict(
     "ResponseMetadataTypeDef",
     {
         "RequestId": str,
+        "HostId": str,
         "HTTPStatusCode": int,
         "HTTPHeaders": Dict[str, str],
         "RetryAttempts": int,
-        "HostId": NotRequired[str],
     },
 )
 UnprocessedNamedQueryIdTypeDef = TypedDict(
     "UnprocessedNamedQueryIdTypeDef",
     {
         "NamedQueryId": NotRequired[str],
         "ErrorCode": NotRequired[str],
@@ -373,24 +369,18 @@
     {
         "Status": CapacityAllocationStatusType,
         "RequestTime": datetime,
         "StatusMessage": NotRequired[str],
         "RequestCompletionTime": NotRequired[datetime],
     },
 )
-CapacityAssignmentOutputTypeDef = TypedDict(
-    "CapacityAssignmentOutputTypeDef",
-    {
-        "WorkGroupNames": NotRequired[List[str]],
-    },
-)
 CapacityAssignmentTypeDef = TypedDict(
     "CapacityAssignmentTypeDef",
     {
-        "WorkGroupNames": NotRequired[Sequence[str]],
+        "WorkGroupNames": NotRequired[List[str]],
     },
 )
 ColumnInfoTypeDef = TypedDict(
     "ColumnInfoTypeDef",
     {
         "Name": str,
         "Type": str,
@@ -530,32 +520,22 @@
 EncryptionConfigurationTypeDef = TypedDict(
     "EncryptionConfigurationTypeDef",
     {
         "EncryptionOption": EncryptionOptionType,
         "KmsKey": NotRequired[str],
     },
 )
-EngineConfigurationOutputTypeDef = TypedDict(
-    "EngineConfigurationOutputTypeDef",
-    {
-        "MaxConcurrentDpus": int,
-        "CoordinatorDpuSize": NotRequired[int],
-        "DefaultExecutorDpuSize": NotRequired[int],
-        "AdditionalConfigs": NotRequired[Dict[str, str]],
-        "SparkProperties": NotRequired[Dict[str, str]],
-    },
-)
 EngineConfigurationTypeDef = TypedDict(
     "EngineConfigurationTypeDef",
     {
         "MaxConcurrentDpus": int,
         "CoordinatorDpuSize": NotRequired[int],
         "DefaultExecutorDpuSize": NotRequired[int],
-        "AdditionalConfigs": NotRequired[Mapping[str, str]],
-        "SparkProperties": NotRequired[Mapping[str, str]],
+        "AdditionalConfigs": NotRequired[Dict[str, str]],
+        "SparkProperties": NotRequired[Dict[str, str]],
     },
 )
 EngineVersionTypeDef = TypedDict(
     "EngineVersionTypeDef",
     {
         "SelectedEngineVersion": NotRequired[str],
         "EffectiveEngineVersion": NotRequired[str],
@@ -1088,32 +1068,32 @@
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 ListApplicationDPUSizesOutputTypeDef = TypedDict(
     "ListApplicationDPUSizesOutputTypeDef",
     {
         "ApplicationDPUSizes": List[ApplicationDPUSizesTypeDef],
+        "NextToken": str,
         "ResponseMetadata": ResponseMetadataTypeDef,
-        "NextToken": NotRequired[str],
     },
 )
 ListNamedQueriesOutputTypeDef = TypedDict(
     "ListNamedQueriesOutputTypeDef",
     {
         "NamedQueryIds": List[str],
+        "NextToken": str,
         "ResponseMetadata": ResponseMetadataTypeDef,
-        "NextToken": NotRequired[str],
     },
 )
 ListQueryExecutionsOutputTypeDef = TypedDict(
     "ListQueryExecutionsOutputTypeDef",
     {
         "QueryExecutionIds": List[str],
+        "NextToken": str,
         "ResponseMetadata": ResponseMetadataTypeDef,
-        "NextToken": NotRequired[str],
     },
 )
 StartCalculationExecutionResponseTypeDef = TypedDict(
     "StartCalculationExecutionResponseTypeDef",
     {
         "CalculationExecutionId": str,
         "State": CalculationExecutionStateType,
@@ -1223,18 +1203,24 @@
         "LastSuccessfulAllocationTime": NotRequired[datetime],
     },
 )
 CapacityAssignmentConfigurationTypeDef = TypedDict(
     "CapacityAssignmentConfigurationTypeDef",
     {
         "CapacityReservationName": NotRequired[str],
-        "CapacityAssignments": NotRequired[List[CapacityAssignmentOutputTypeDef]],
+        "CapacityAssignments": NotRequired[List[CapacityAssignmentTypeDef]],
+    },
+)
+PutCapacityAssignmentConfigurationInputRequestTypeDef = TypedDict(
+    "PutCapacityAssignmentConfigurationInputRequestTypeDef",
+    {
+        "CapacityReservationName": str,
+        "CapacityAssignments": Sequence[CapacityAssignmentTypeDef],
     },
 )
-CapacityAssignmentUnionTypeDef = Union[CapacityAssignmentTypeDef, CapacityAssignmentOutputTypeDef]
 ResultSetMetadataTypeDef = TypedDict(
     "ResultSetMetadataTypeDef",
     {
         "ColumnInfo": NotRequired[List[ColumnInfoTypeDef]],
     },
 )
 TableMetadataTypeDef = TypedDict(
@@ -1267,31 +1253,31 @@
         "Tags": NotRequired[Sequence[TagTypeDef]],
     },
 )
 ListTagsForResourceOutputTypeDef = TypedDict(
     "ListTagsForResourceOutputTypeDef",
     {
         "Tags": List[TagTypeDef],
+        "NextToken": str,
         "ResponseMetadata": ResponseMetadataTypeDef,
-        "NextToken": NotRequired[str],
     },
 )
 TagResourceInputRequestTypeDef = TypedDict(
     "TagResourceInputRequestTypeDef",
     {
         "ResourceARN": str,
         "Tags": Sequence[TagTypeDef],
     },
 )
 ListDataCatalogsOutputTypeDef = TypedDict(
     "ListDataCatalogsOutputTypeDef",
     {
         "DataCatalogsSummary": List[DataCatalogSummaryTypeDef],
+        "NextToken": str,
         "ResponseMetadata": ResponseMetadataTypeDef,
-        "NextToken": NotRequired[str],
     },
 )
 GetDataCatalogOutputTypeDef = TypedDict(
     "GetDataCatalogOutputTypeDef",
     {
         "DataCatalog": DataCatalogTypeDef,
         "ResponseMetadata": ResponseMetadataTypeDef,
@@ -1304,16 +1290,16 @@
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 ListDatabasesOutputTypeDef = TypedDict(
     "ListDatabasesOutputTypeDef",
     {
         "DatabaseList": List[DatabaseTypeDef],
+        "NextToken": str,
         "ResponseMetadata": ResponseMetadataTypeDef,
-        "NextToken": NotRequired[str],
     },
 )
 RowTypeDef = TypedDict(
     "RowTypeDef",
     {
         "Data": NotRequired[List[DatumTypeDef]],
     },
@@ -1345,17 +1331,14 @@
     {
         "ExecutionRole": NotRequired[str],
         "WorkingDirectory": NotRequired[str],
         "IdleTimeoutSeconds": NotRequired[int],
         "EncryptionConfiguration": NotRequired[EncryptionConfigurationTypeDef],
     },
 )
-EngineConfigurationUnionTypeDef = Union[
-    EngineConfigurationTypeDef, EngineConfigurationOutputTypeDef
-]
 StartSessionRequestRequestTypeDef = TypedDict(
     "StartSessionRequestRequestTypeDef",
     {
         "WorkGroup": str,
         "EngineConfiguration": EngineConfigurationTypeDef,
         "Description": NotRequired[str],
         "NotebookVersion": NotRequired[str],
@@ -1363,16 +1346,16 @@
         "ClientRequestToken": NotRequired[str],
     },
 )
 ListEngineVersionsOutputTypeDef = TypedDict(
     "ListEngineVersionsOutputTypeDef",
     {
         "EngineVersions": List[EngineVersionTypeDef],
+        "NextToken": str,
         "ResponseMetadata": ResponseMetadataTypeDef,
-        "NextToken": NotRequired[str],
     },
 )
 WorkGroupSummaryTypeDef = TypedDict(
     "WorkGroupSummaryTypeDef",
     {
         "Name": NotRequired[str],
         "State": NotRequired[WorkGroupStateType],
@@ -1382,17 +1365,17 @@
         "IdentityCenterApplicationArn": NotRequired[str],
     },
 )
 ListExecutorsResponseTypeDef = TypedDict(
     "ListExecutorsResponseTypeDef",
     {
         "SessionId": str,
+        "NextToken": str,
         "ExecutorsSummary": List[ExecutorsSummaryTypeDef],
         "ResponseMetadata": ResponseMetadataTypeDef,
-        "NextToken": NotRequired[str],
     },
 )
 ExportNotebookOutputTypeDef = TypedDict(
     "ExportNotebookOutputTypeDef",
     {
         "NotebookMetadata": NotebookMetadataTypeDef,
         "Payload": str,
@@ -1405,17 +1388,17 @@
         "NotebookMetadata": NotebookMetadataTypeDef,
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 ListNotebookMetadataOutputTypeDef = TypedDict(
     "ListNotebookMetadataOutputTypeDef",
     {
+        "NextToken": str,
         "NotebookMetadataList": List[NotebookMetadataTypeDef],
         "ResponseMetadata": ResponseMetadataTypeDef,
-        "NextToken": NotRequired[str],
     },
 )
 ListNotebookMetadataInputRequestTypeDef = TypedDict(
     "ListNotebookMetadataInputRequestTypeDef",
     {
         "WorkGroup": str,
         "Filters": NotRequired[FilterDefinitionTypeDef],
@@ -1494,24 +1477,24 @@
         "Status": NotRequired[SessionStatusTypeDef],
     },
 )
 ListNotebookSessionsResponseTypeDef = TypedDict(
     "ListNotebookSessionsResponseTypeDef",
     {
         "NotebookSessionsList": List[NotebookSessionSummaryTypeDef],
+        "NextToken": str,
         "ResponseMetadata": ResponseMetadataTypeDef,
-        "NextToken": NotRequired[str],
     },
 )
 ListPreparedStatementsOutputTypeDef = TypedDict(
     "ListPreparedStatementsOutputTypeDef",
     {
         "PreparedStatements": List[PreparedStatementSummaryTypeDef],
+        "NextToken": str,
         "ResponseMetadata": ResponseMetadataTypeDef,
-        "NextToken": NotRequired[str],
     },
 )
 QueryExecutionStatisticsTypeDef = TypedDict(
     "QueryExecutionStatisticsTypeDef",
     {
         "EngineExecutionTimeInMillis": NotRequired[int],
         "DataScannedInBytes": NotRequired[int],
@@ -1537,61 +1520,54 @@
     {
         "ResultReuseByAgeConfiguration": NotRequired[ResultReuseByAgeConfigurationTypeDef],
     },
 )
 ListCalculationExecutionsResponseTypeDef = TypedDict(
     "ListCalculationExecutionsResponseTypeDef",
     {
+        "NextToken": str,
         "Calculations": List[CalculationSummaryTypeDef],
         "ResponseMetadata": ResponseMetadataTypeDef,
-        "NextToken": NotRequired[str],
     },
 )
 GetCapacityReservationOutputTypeDef = TypedDict(
     "GetCapacityReservationOutputTypeDef",
     {
         "CapacityReservation": CapacityReservationTypeDef,
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 ListCapacityReservationsOutputTypeDef = TypedDict(
     "ListCapacityReservationsOutputTypeDef",
     {
+        "NextToken": str,
         "CapacityReservations": List[CapacityReservationTypeDef],
         "ResponseMetadata": ResponseMetadataTypeDef,
-        "NextToken": NotRequired[str],
     },
 )
 GetCapacityAssignmentConfigurationOutputTypeDef = TypedDict(
     "GetCapacityAssignmentConfigurationOutputTypeDef",
     {
         "CapacityAssignmentConfiguration": CapacityAssignmentConfigurationTypeDef,
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
-PutCapacityAssignmentConfigurationInputRequestTypeDef = TypedDict(
-    "PutCapacityAssignmentConfigurationInputRequestTypeDef",
-    {
-        "CapacityReservationName": str,
-        "CapacityAssignments": Sequence[CapacityAssignmentUnionTypeDef],
-    },
-)
 GetTableMetadataOutputTypeDef = TypedDict(
     "GetTableMetadataOutputTypeDef",
     {
         "TableMetadata": TableMetadataTypeDef,
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 ListTableMetadataOutputTypeDef = TypedDict(
     "ListTableMetadataOutputTypeDef",
     {
         "TableMetadataList": List[TableMetadataTypeDef],
+        "NextToken": str,
         "ResponseMetadata": ResponseMetadataTypeDef,
-        "NextToken": NotRequired[str],
     },
 )
 ResultSetTypeDef = TypedDict(
     "ResultSetTypeDef",
     {
         "Rows": NotRequired[List[RowTypeDef]],
         "ResultSetMetadata": NotRequired[ResultSetMetadataTypeDef],
@@ -1643,36 +1619,36 @@
 GetSessionResponseTypeDef = TypedDict(
     "GetSessionResponseTypeDef",
     {
         "SessionId": str,
         "Description": str,
         "WorkGroup": str,
         "EngineVersion": str,
-        "EngineConfiguration": EngineConfigurationOutputTypeDef,
+        "EngineConfiguration": EngineConfigurationTypeDef,
         "NotebookVersion": str,
         "SessionConfiguration": SessionConfigurationTypeDef,
         "Status": SessionStatusTypeDef,
         "Statistics": SessionStatisticsTypeDef,
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 ListWorkGroupsOutputTypeDef = TypedDict(
     "ListWorkGroupsOutputTypeDef",
     {
         "WorkGroups": List[WorkGroupSummaryTypeDef],
+        "NextToken": str,
         "ResponseMetadata": ResponseMetadataTypeDef,
-        "NextToken": NotRequired[str],
     },
 )
 ListSessionsResponseTypeDef = TypedDict(
     "ListSessionsResponseTypeDef",
     {
+        "NextToken": str,
         "Sessions": List[SessionSummaryTypeDef],
         "ResponseMetadata": ResponseMetadataTypeDef,
-        "NextToken": NotRequired[str],
     },
 )
 GetQueryRuntimeStatisticsOutputTypeDef = TypedDict(
     "GetQueryRuntimeStatisticsOutputTypeDef",
     {
         "QueryRuntimeStatistics": QueryRuntimeStatisticsTypeDef,
         "ResponseMetadata": ResponseMetadataTypeDef,
@@ -1711,16 +1687,16 @@
     },
 )
 GetQueryResultsOutputTypeDef = TypedDict(
     "GetQueryResultsOutputTypeDef",
     {
         "UpdateCount": int,
         "ResultSet": ResultSetTypeDef,
+        "NextToken": str,
         "ResponseMetadata": ResponseMetadataTypeDef,
-        "NextToken": NotRequired[str],
     },
 )
 CreateWorkGroupInputRequestTypeDef = TypedDict(
     "CreateWorkGroupInputRequestTypeDef",
     {
         "Name": str,
         "Configuration": NotRequired[WorkGroupConfigurationTypeDef],
```

### Comparing `mypy_boto3_athena-1.34.115/mypy_boto3_athena.egg-info/PKG-INFO` & `mypy-boto3-athena-1.34.23/mypy_boto3_athena.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 Metadata-Version: 2.1
 Name: mypy-boto3-athena
-Version: 1.34.115
-Summary: Type annotations for boto3.Athena 1.34.115 service generated with mypy-boto3-builder 7.24.0
+Version: 1.34.23
+Summary: Type annotations for boto3.Athena 1.34.23 service generated with mypy-boto3-builder 7.23.1
 Home-page: https://github.com/youtype/mypy_boto3_builder
 Author: Vlad Emelianov
 Author-email: vlad.emelianov.nz@gmail.com
 License: MIT License
 Project-URL: Documentation, https://youtype.github.io/boto3_stubs_docs/mypy_boto3_athena/
 Project-URL: Source, https://github.com/youtype/mypy_boto3_builder
 Project-URL: Tracker, https://github.com/youtype/mypy_boto3_builder/issues
@@ -39,24 +39,24 @@
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/mypy-boto3-athena.svg?color=blue)](https://pypi.org/project/mypy-boto3-athena)
 [![Docs](https://img.shields.io/readthedocs/boto3-stubs.svg?color=blue)](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_athena/)
 [![PyPI - Downloads](https://static.pepy.tech/badge/mypy-boto3-athena)](https://pepy.tech/project/mypy-boto3-athena)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
-[boto3.Athena 1.34.115](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/athena.html#Athena)
+[boto3.Athena 1.34.23](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/athena.html#Athena)
 service compatible with [VSCode](https://code.visualstudio.com/),
 [PyCharm](https://www.jetbrains.com/pycharm/),
 [Emacs](https://www.gnu.org/software/emacs/),
 [Sublime Text](https://www.sublimetext.com/),
 [mypy](https://github.com/python/mypy),
 [pyright](https://github.com/microsoft/pyright) and other tools.
 
 Generated by
-[mypy-boto3-builder 7.24.0](https://github.com/youtype/mypy_boto3_builder).
+[mypy-boto3-builder 7.23.1](https://github.com/youtype/mypy_boto3_builder).
 
 More information can be found on
 [boto3-stubs](https://pypi.org/project/boto3-stubs/) page and in
 [mypy-boto3-athena docs](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_athena/).
 
 See how it helps to find and fix potential bugs:
```

### Comparing `mypy_boto3_athena-1.34.115/mypy_boto3_athena.egg-info/SOURCES.txt` & `mypy-boto3-athena-1.34.23/mypy_boto3_athena.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `mypy_boto3_athena-1.34.115/setup.py` & `mypy-boto3-athena-1.34.23/setup.py`

 * *Files 11% similar despite different names*

```diff
@@ -7,21 +7,23 @@
 from setuptools import setup
 
 LONG_DESCRIPTION = (Path(__file__).parent / "README.md").read_text()
 
 
 setup(
     name="mypy-boto3-athena",
-    version="1.34.115",
+    version="1.34.23",
     packages=["mypy_boto3_athena"],
     url="https://github.com/youtype/mypy_boto3_builder",
     license="MIT License",
     author="Vlad Emelianov",
     author_email="vlad.emelianov.nz@gmail.com",
-    description="Type annotations for boto3.Athena 1.34.115 service generated with mypy-boto3-builder 7.24.0",
+    description=(
+        "Type annotations for boto3.Athena 1.34.23 service generated with mypy-boto3-builder 7.23.1"
+    ),
     classifiers=[
         "Development Status :: 5 - Production/Stable",
         "Intended Audience :: Developers",
         "Environment :: Console",
         "License :: OSI Approved :: MIT License",
         "Natural Language :: English",
         "Operating System :: OS Independent",
```

