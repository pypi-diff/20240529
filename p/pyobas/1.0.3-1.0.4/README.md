# Comparing `tmp/pyobas-1.0.3.tar.gz` & `tmp/pyobas-1.0.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pyobas-1.0.3.tar", last modified: Thu May 23 14:27:25 2024, max compression
+gzip compressed data, was "pyobas-1.0.4.tar", last modified: Tue May 28 22:00:56 2024, max compression
```

## Comparing `pyobas-1.0.3.tar` & `pyobas-1.0.4.tar`

### file list

```diff
@@ -1,43 +1,45 @@
-drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2024-05-23 14:27:25.912378 pyobas-1.0.3/
--rw-r--r--   0 circleci  (1001) circleci  (1002)    11357 2024-05-23 14:27:16.000000 pyobas-1.0.3/LICENSE
--rw-r--r--   0 circleci  (1001) circleci  (1002)     4865 2024-05-23 14:27:25.912378 pyobas-1.0.3/PKG-INFO
--rw-r--r--   0 circleci  (1001) circleci  (1002)     3159 2024-05-23 14:27:16.000000 pyobas-1.0.3/README.md
-drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2024-05-23 14:27:25.904378 pyobas-1.0.3/pyobas/
--rw-r--r--   0 circleci  (1001) circleci  (1002)      524 2024-05-23 14:27:16.000000 pyobas-1.0.3/pyobas/__init__.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)      183 2024-05-23 14:27:16.000000 pyobas-1.0.3/pyobas/_version.py
-drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2024-05-23 14:27:25.908378 pyobas-1.0.3/pyobas/apis/
--rw-r--r--   0 circleci  (1001) circleci  (1002)      497 2024-05-23 14:27:16.000000 pyobas-1.0.3/pyobas/apis/__init__.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)      643 2024-05-23 14:27:16.000000 pyobas-1.0.3/pyobas/apis/attack_pattern.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)      532 2024-05-23 14:27:16.000000 pyobas-1.0.3/pyobas/apis/collector.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)      516 2024-05-23 14:27:16.000000 pyobas-1.0.3/pyobas/apis/document.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)      890 2024-05-23 14:27:16.000000 pyobas-1.0.3/pyobas/apis/inject.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)      722 2024-05-23 14:27:16.000000 pyobas-1.0.3/pyobas/apis/injector.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)      635 2024-05-23 14:27:16.000000 pyobas-1.0.3/pyobas/apis/kill_chain_phase.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)      397 2024-05-23 14:27:16.000000 pyobas-1.0.3/pyobas/apis/me.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)      263 2024-05-23 14:27:16.000000 pyobas-1.0.3/pyobas/apis/organization.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)      788 2024-05-23 14:27:16.000000 pyobas-1.0.3/pyobas/apis/team.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)      893 2024-05-23 14:27:16.000000 pyobas-1.0.3/pyobas/apis/user.py
-drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2024-05-23 14:27:25.908378 pyobas-1.0.3/pyobas/backends/
--rw-r--r--   0 circleci  (1001) circleci  (1002)      272 2024-05-23 14:27:16.000000 pyobas-1.0.3/pyobas/backends/__init__.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)     4328 2024-05-23 14:27:16.000000 pyobas-1.0.3/pyobas/backends/backend.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)      842 2024-05-23 14:27:16.000000 pyobas-1.0.3/pyobas/backends/protocol.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)    10756 2024-05-23 14:27:16.000000 pyobas-1.0.3/pyobas/base.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)    16141 2024-05-23 14:27:16.000000 pyobas-1.0.3/pyobas/client.py
-drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2024-05-23 14:27:25.908378 pyobas-1.0.3/pyobas/contracts/
--rw-r--r--   0 circleci  (1001) circleci  (1002)      103 2024-05-23 14:27:16.000000 pyobas-1.0.3/pyobas/contracts/__init__.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)      987 2024-05-23 14:27:16.000000 pyobas-1.0.3/pyobas/contracts/contract_builder.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)     5609 2024-05-23 14:27:16.000000 pyobas-1.0.3/pyobas/contracts/contract_config.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)      451 2024-05-23 14:27:16.000000 pyobas-1.0.3/pyobas/contracts/contract_utils.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)     4208 2024-05-23 14:27:16.000000 pyobas-1.0.3/pyobas/contracts/variable_helper.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)     2525 2024-05-23 14:27:16.000000 pyobas-1.0.3/pyobas/exceptions.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)    14284 2024-05-23 14:27:16.000000 pyobas-1.0.3/pyobas/helpers.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)     6777 2024-05-23 14:27:16.000000 pyobas-1.0.3/pyobas/mixins.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)     3865 2024-05-23 14:27:16.000000 pyobas-1.0.3/pyobas/utils.py
-drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2024-05-23 14:27:25.908378 pyobas-1.0.3/pyobas.egg-info/
--rw-r--r--   0 circleci  (1001) circleci  (1002)     4865 2024-05-23 14:27:25.000000 pyobas-1.0.3/pyobas.egg-info/PKG-INFO
--rw-r--r--   0 circleci  (1001) circleci  (1002)      856 2024-05-23 14:27:25.000000 pyobas-1.0.3/pyobas.egg-info/SOURCES.txt
--rw-r--r--   0 circleci  (1001) circleci  (1002)        1 2024-05-23 14:27:25.000000 pyobas-1.0.3/pyobas.egg-info/dependency_links.txt
--rw-r--r--   0 circleci  (1001) circleci  (1002)      378 2024-05-23 14:27:25.000000 pyobas-1.0.3/pyobas.egg-info/requires.txt
--rw-r--r--   0 circleci  (1001) circleci  (1002)        7 2024-05-23 14:27:25.000000 pyobas-1.0.3/pyobas.egg-info/top_level.txt
--rw-r--r--   0 circleci  (1001) circleci  (1002)      598 2024-05-23 14:27:16.000000 pyobas-1.0.3/pyproject.toml
--rw-r--r--   0 circleci  (1001) circleci  (1002)     1386 2024-05-23 14:27:25.912378 pyobas-1.0.3/setup.cfg
+drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2024-05-28 22:00:56.120499 pyobas-1.0.4/
+-rw-r--r--   0 circleci  (1001) circleci  (1002)    11357 2024-05-28 22:00:43.000000 pyobas-1.0.4/LICENSE
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     5167 2024-05-28 22:00:56.120499 pyobas-1.0.4/PKG-INFO
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     3159 2024-05-28 22:00:43.000000 pyobas-1.0.4/README.md
+drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2024-05-28 22:00:56.112499 pyobas-1.0.4/pyobas/
+-rw-r--r--   0 circleci  (1001) circleci  (1002)      524 2024-05-28 22:00:43.000000 pyobas-1.0.4/pyobas/__init__.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)      183 2024-05-28 22:00:43.000000 pyobas-1.0.4/pyobas/_version.py
+drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2024-05-28 22:00:56.116499 pyobas-1.0.4/pyobas/apis/
+-rw-r--r--   0 circleci  (1001) circleci  (1002)      593 2024-05-28 22:00:43.000000 pyobas-1.0.4/pyobas/apis/__init__.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)      643 2024-05-28 22:00:43.000000 pyobas-1.0.4/pyobas/apis/attack_pattern.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)      532 2024-05-28 22:00:43.000000 pyobas-1.0.4/pyobas/apis/collector.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)      516 2024-05-28 22:00:43.000000 pyobas-1.0.4/pyobas/apis/document.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)      492 2024-05-28 22:00:43.000000 pyobas-1.0.4/pyobas/apis/endpoint.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)      890 2024-05-28 22:00:43.000000 pyobas-1.0.4/pyobas/apis/inject.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     1716 2024-05-28 22:00:43.000000 pyobas-1.0.4/pyobas/apis/inject_expectation.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)      722 2024-05-28 22:00:43.000000 pyobas-1.0.4/pyobas/apis/injector.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)      635 2024-05-28 22:00:43.000000 pyobas-1.0.4/pyobas/apis/kill_chain_phase.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)      397 2024-05-28 22:00:43.000000 pyobas-1.0.4/pyobas/apis/me.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)      263 2024-05-28 22:00:43.000000 pyobas-1.0.4/pyobas/apis/organization.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)      788 2024-05-28 22:00:43.000000 pyobas-1.0.4/pyobas/apis/team.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)      893 2024-05-28 22:00:43.000000 pyobas-1.0.4/pyobas/apis/user.py
+drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2024-05-28 22:00:56.116499 pyobas-1.0.4/pyobas/backends/
+-rw-r--r--   0 circleci  (1001) circleci  (1002)      272 2024-05-28 22:00:43.000000 pyobas-1.0.4/pyobas/backends/__init__.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     4328 2024-05-28 22:00:43.000000 pyobas-1.0.4/pyobas/backends/backend.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)      842 2024-05-28 22:00:43.000000 pyobas-1.0.4/pyobas/backends/protocol.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)    10756 2024-05-28 22:00:43.000000 pyobas-1.0.4/pyobas/base.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)    16261 2024-05-28 22:00:43.000000 pyobas-1.0.4/pyobas/client.py
+drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2024-05-28 22:00:56.116499 pyobas-1.0.4/pyobas/contracts/
+-rw-r--r--   0 circleci  (1001) circleci  (1002)      103 2024-05-28 22:00:43.000000 pyobas-1.0.4/pyobas/contracts/__init__.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)      987 2024-05-28 22:00:43.000000 pyobas-1.0.4/pyobas/contracts/contract_builder.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     5609 2024-05-28 22:00:43.000000 pyobas-1.0.4/pyobas/contracts/contract_config.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)      451 2024-05-28 22:00:43.000000 pyobas-1.0.4/pyobas/contracts/contract_utils.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     4208 2024-05-28 22:00:43.000000 pyobas-1.0.4/pyobas/contracts/variable_helper.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     2525 2024-05-28 22:00:43.000000 pyobas-1.0.4/pyobas/exceptions.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)    15283 2024-05-28 22:00:43.000000 pyobas-1.0.4/pyobas/helpers.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     6777 2024-05-28 22:00:43.000000 pyobas-1.0.4/pyobas/mixins.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     5297 2024-05-28 22:00:43.000000 pyobas-1.0.4/pyobas/utils.py
+drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2024-05-28 22:00:56.116499 pyobas-1.0.4/pyobas.egg-info/
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     5167 2024-05-28 22:00:56.000000 pyobas-1.0.4/pyobas.egg-info/PKG-INFO
+-rw-r--r--   0 circleci  (1001) circleci  (1002)      914 2024-05-28 22:00:56.000000 pyobas-1.0.4/pyobas.egg-info/SOURCES.txt
+-rw-r--r--   0 circleci  (1001) circleci  (1002)        1 2024-05-28 22:00:56.000000 pyobas-1.0.4/pyobas.egg-info/dependency_links.txt
+-rw-r--r--   0 circleci  (1001) circleci  (1002)      596 2024-05-28 22:00:56.000000 pyobas-1.0.4/pyobas.egg-info/requires.txt
+-rw-r--r--   0 circleci  (1001) circleci  (1002)        7 2024-05-28 22:00:56.000000 pyobas-1.0.4/pyobas.egg-info/top_level.txt
+-rw-r--r--   0 circleci  (1001) circleci  (1002)      598 2024-05-28 22:00:43.000000 pyobas-1.0.4/pyproject.toml
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     1604 2024-05-28 22:00:56.120499 pyobas-1.0.4/setup.cfg
```

### Comparing `pyobas-1.0.3/LICENSE` & `pyobas-1.0.4/LICENSE`

 * *Files identical despite different names*

### Comparing `pyobas-1.0.3/PKG-INFO` & `pyobas-1.0.4/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pyobas
-Version: 1.0.3
+Version: 1.0.4
 Summary: Python API client for OpenBAS.
 Home-page: https://github.com/OpenBAS-Platform/client-python
 Author: Filigran
 Author-email: contact@filigran.io
 Maintainer: Filigran
 License: Apache
 Classifier: Development Status :: 5 - Production/Stable
@@ -17,22 +17,28 @@
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python :: 3
 Classifier: Topic :: Security
 Classifier: Topic :: Software Development :: Libraries :: Python Modules
 Requires-Python: >=3.7
 Description-Content-Type: text/markdown
 License-File: LICENSE
-Requires-Dist: dataclasses-json~=0.6.4
-Requires-Dist: pika~=1.3.1
-Requires-Dist: prometheus-client~=0.20.0
+Requires-Dist: datefinder~=0.7.3
+Requires-Dist: pika~=1.3.0
+Requires-Dist: python-magic~=0.4.27; sys_platform == "linux" or sys_platform == "darwin"
+Requires-Dist: python-magic-bin~=0.4.14; sys_platform == "win32"
 Requires-Dist: python_json_logger~=2.0.4
-Requires-Dist: pyyaml~=6.0
-Requires-Dist: requests~=2.32.2
-Requires-Dist: requests-toolbelt~=1.0.0
+Requires-Dist: PyYAML~=6.0
+Requires-Dist: requests~=2.31.0
 Requires-Dist: setuptools~=70.0.0
+Requires-Dist: cachetools~=5.3.0
+Requires-Dist: prometheus-client~=0.20.0
+Requires-Dist: opentelemetry-api~=1.22.0
+Requires-Dist: opentelemetry-sdk~=1.22.0
+Requires-Dist: requests-toolbelt~=1.0.0
+Requires-Dist: dataclasses-json~=0.6.4
 Provides-Extra: dev
 Requires-Dist: black~=24.4.0; extra == "dev"
 Requires-Dist: build~=1.2.1; extra == "dev"
 Requires-Dist: isort~=5.13.0; extra == "dev"
 Requires-Dist: types-pytz~=2024.1.0.20240203; extra == "dev"
 Requires-Dist: pre-commit~=3.7.1; extra == "dev"
 Requires-Dist: types-python-dateutil~=2.9.0; extra == "dev"
```

### Comparing `pyobas-1.0.3/README.md` & `pyobas-1.0.4/README.md`

 * *Files identical despite different names*

### Comparing `pyobas-1.0.3/pyobas/__init__.py` & `pyobas-1.0.4/pyobas/__init__.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 # -*- coding: utf-8 -*-
-__version__ = "1.0.3"
+__version__ = "1.0.4"
 
 from pyobas._version import (  # noqa: F401
     __author__,
     __copyright__,
     __email__,
     __license__,
     __title__,
```

### Comparing `pyobas-1.0.3/pyobas/apis/attack_pattern.py` & `pyobas-1.0.4/pyobas/apis/attack_pattern.py`

 * *Files identical despite different names*

### Comparing `pyobas-1.0.3/pyobas/apis/collector.py` & `pyobas-1.0.4/pyobas/apis/collector.py`

 * *Files identical despite different names*

### Comparing `pyobas-1.0.3/pyobas/apis/document.py` & `pyobas-1.0.4/pyobas/apis/document.py`

 * *Files identical despite different names*

### Comparing `pyobas-1.0.3/pyobas/apis/inject.py` & `pyobas-1.0.4/pyobas/apis/inject.py`

 * *Files identical despite different names*

### Comparing `pyobas-1.0.3/pyobas/apis/injector.py` & `pyobas-1.0.4/pyobas/apis/injector.py`

 * *Files identical despite different names*

### Comparing `pyobas-1.0.3/pyobas/apis/kill_chain_phase.py` & `pyobas-1.0.4/pyobas/apis/kill_chain_phase.py`

 * *Files identical despite different names*

### Comparing `pyobas-1.0.3/pyobas/apis/team.py` & `pyobas-1.0.4/pyobas/apis/team.py`

 * *Files identical despite different names*

### Comparing `pyobas-1.0.3/pyobas/apis/user.py` & `pyobas-1.0.4/pyobas/apis/user.py`

 * *Files identical despite different names*

### Comparing `pyobas-1.0.3/pyobas/backends/backend.py` & `pyobas-1.0.4/pyobas/backends/backend.py`

 * *Files identical despite different names*

### Comparing `pyobas-1.0.3/pyobas/backends/protocol.py` & `pyobas-1.0.4/pyobas/backends/protocol.py`

 * *Files identical despite different names*

### Comparing `pyobas-1.0.3/pyobas/base.py` & `pyobas-1.0.4/pyobas/base.py`

 * *Files identical despite different names*

### Comparing `pyobas-1.0.3/pyobas/client.py` & `pyobas-1.0.4/pyobas/client.py`

 * *Files 0% similar despite different names*

```diff
@@ -60,15 +60,17 @@
         self.injector = apis.InjectorManager(self)
         self.collector = apis.CollectorManager(self)
         self.inject = apis.InjectManager(self)
         self.document = apis.DocumentManager(self)
         self.kill_chain_phase = apis.KillChainPhaseManager(self)
         self.attack_pattern = apis.AttackPatternManager(self)
         self.team = apis.TeamManager(self)
+        self.endpoint = apis.EndpointManager(self)
         self.user = apis.UserManager(self)
+        self.inject_expectation = apis.InjectExpectationManager(self)
 
     @staticmethod
     def _check_redirects(result: requests.Response) -> None:
         # Check the requests history to detect 301/302 redirections.
         # If the initial verb is POST or PUT, the redirected request will use a
         # GET request, leading to unwanted behaviour.
         # If we detect a redirection with a POST or a PUT request, we
@@ -289,15 +291,14 @@
         post_data: Optional[Union[Dict[str, Any], bytes, BinaryIO]] = None,
         raw: bool = False,
         files: Optional[Dict[str, Any]] = None,
         **kwargs: Any,
     ) -> Union[Dict[str, Any], requests.Response]:
         query_data = query_data or {}
         post_data = post_data or {}
-
         result = self.http_request(
             "put",
             path,
             query_data=query_data,
             post_data=post_data,
             files=files,
             raw=raw,
```

### Comparing `pyobas-1.0.3/pyobas/contracts/contract_builder.py` & `pyobas-1.0.4/pyobas/contracts/contract_builder.py`

 * *Files identical despite different names*

### Comparing `pyobas-1.0.3/pyobas/contracts/contract_config.py` & `pyobas-1.0.4/pyobas/contracts/contract_config.py`

 * *Files identical despite different names*

### Comparing `pyobas-1.0.3/pyobas/contracts/variable_helper.py` & `pyobas-1.0.4/pyobas/contracts/variable_helper.py`

 * *Files identical despite different names*

### Comparing `pyobas-1.0.3/pyobas/exceptions.py` & `pyobas-1.0.4/pyobas/exceptions.py`

 * *Files identical despite different names*

### Comparing `pyobas-1.0.3/pyobas/helpers.py` & `pyobas-1.0.4/pyobas/helpers.py`

 * *Files 10% similar despite different names*

```diff
@@ -8,15 +8,15 @@
 import traceback
 from datetime import datetime, timezone
 from typing import Callable, Dict, List, Optional, Union
 
 import pika
 import yaml
 
-from pyobas import OpenBAS
+from pyobas import OpenBAS, utils
 
 TRUTHY: List[str] = ["yes", "true", "True"]
 FALSY: List[str] = ["no", "false", "False"]
 
 
 # As cert must be written in files to be loaded in ssl context
 # Creates a temporary file in the most secure manner possible
@@ -148,24 +148,26 @@
 
 
 class ListenQueue(threading.Thread):
     def __init__(
         self,
         config: Dict,
         injector_config: Dict,
+        logger,
         callback,
     ) -> None:
         threading.Thread.__init__(self)
         self.pika_credentials = None
         self.pika_parameters = None
         self.pika_connection = None
         self.channel = None
 
         self.callback = callback
         self.config = config
+        self.logger = logger
         self.host = injector_config.connection["host"]
         self.vhost = injector_config.connection["vhost"]
         self.use_ssl = injector_config.connection["use_ssl"]
         self.port = injector_config.connection["port"]
         self.user = injector_config.connection["user"]
         self.password = injector_config.connection["pass"]
         self.queue_name = injector_config.listen
@@ -193,18 +195,18 @@
         self.thread = threading.Thread(target=self._data_handler, args=[json_data])
         self.thread.start()
 
     def _data_handler(self, json_data) -> None:
         self.callback(json_data)
 
     def run(self) -> None:
-        print("Starting ListenQueue thread")
+        self.logger.info("Starting ListenQueue thread")
         while not self.exit_event.is_set():
             try:
-                print("ListenQueue connecting to rabbitMq.")
+                self.logger.info("ListenQueue connecting to RabbitMQ.")
                 # Connect the broker
                 self.pika_credentials = pika.PlainCredentials(self.user, self.password)
                 self.pika_parameters = pika.ConnectionParameters(
                     host=self.host,
                     port=self.port,
                     virtual_host=self.vhost,
                     credentials=self.pika_credentials,
@@ -217,64 +219,65 @@
                 self.pika_connection = pika.BlockingConnection(self.pika_parameters)
                 self.channel = self.pika_connection.channel()
                 try:
                     # confirm_delivery is only for cluster mode rabbitMQ
                     # when not in cluster mode this line raise an exception
                     self.channel.confirm_delivery()
                 except Exception as err:  # pylint: disable=broad-except
-                    print(str(err))
+                    self.logger.error(str(err))
                 self.channel.basic_qos(prefetch_count=1)
                 assert self.channel is not None
                 self.channel.basic_consume(
                     queue=self.queue_name, on_message_callback=self._process_message
                 )
                 self.channel.start_consuming()
             except Exception:  # pylint: disable=broad-except
                 try:
                     self.pika_connection.close()
                 except Exception as errInException:
-                    print(str(errInException))
+                    self.logger.error(str(errInException))
                 traceback.print_exc()
                 # Wait some time and then retry ListenQueue again.
                 time.sleep(10)
 
     def stop(self):
-        print("Preparing ListenQueue for clean shutdown")
+        self.logger.info("Preparing ListenQueue for clean shutdown")
         self.exit_event.set()
         self.pika_connection.close()
         if self.thread:
             self.thread.join()
 
 
 class PingAlive(threading.Thread):
-    def __init__(self, api, config, ping_type) -> None:
+    def __init__(self, api, config, logger, ping_type) -> None:
         threading.Thread.__init__(self)
         self.ping_type = ping_type
         self.api = api
         self.config = config
+        self.logger = logger
         self.in_error = False
         self.exit_event = threading.Event()
 
     def ping(self) -> None:
         while not self.exit_event.is_set():
             try:
                 if self.ping_type == "injector":
                     self.api.injector.create(self.config, False)
                 else:
                     self.api.collector.create(self.config, False)
             except Exception as e:  # pylint: disable=broad-except
-                print(str(e))
+                self.logger.error(str(e))
             self.exit_event.wait(40)
 
     def run(self) -> None:
-        print("Starting PingAlive thread")
+        self.logger.info("Starting PingAlive thread")
         self.ping()
 
     def stop(self) -> None:
-        print("Preparing PingAlive for clean shutdown")
+        self.logger.info("Preparing PingAlive for clean shutdown")
         self.exit_event.set()
 
 
 class OpenBASConfigHelper:
     def __init__(self, base_path, variables: Dict):
         config_file_path = os.path.dirname(os.path.abspath(base_path)) + "/config.yml"
         self.file_config = (
@@ -305,46 +308,59 @@
 class OpenBASCollectorHelper:
     def __init__(self, config: OpenBASConfigHelper, icon) -> None:
         self.config_helper = config
         self.api = OpenBAS(
             url=config.get_conf("openbas_url"),
             token=config.get_conf("openbas_token"),
         )
+
         self.config = {
             "collector_id": config.get_conf("collector_id"),
             "collector_name": config.get_conf("collector_name"),
             "collector_type": config.get_conf("collector_type"),
             "collector_period": config.get_conf("collector_period"),
         }
+
+        self.logger_class = utils.logger(
+            config.get_conf("collector_log_level", default="info").upper(),
+            config.get_conf("collector_json_logging", default=True),
+        )
+        self.collector_logger = self.logger_class(config.get_conf("collector_name"))
+
         icon_name = config.get_conf("collector_id") + ".png"
         collector_icon = (icon_name, icon, "image/png")
         self.api.collector.create(self.config, collector_icon)
         self.connect_run_and_terminate = False
         # self.api.injector.create(self.config)
         self.scheduler = sched.scheduler(time.time, time.sleep)
         # Start ping thread
         if not self.connect_run_and_terminate:
-            self.ping = PingAlive(self.api, self.config, "collector")
+            self.ping = PingAlive(
+                self.api, self.config, self.collector_logger, "collector"
+            )
             self.ping.start()
         self.listen_queue = None
 
     def _schedule(self, scheduler, message_callback, delay):
         # Execute
         message_callback()
         # Then schedule the next execution
         scheduler.enter(delay, 1, self._schedule, (scheduler, message_callback, delay))
 
     def schedule(self, message_callback, delay):
         # Start execution directly
-        message_callback()
-        now = datetime.now(timezone.utc).isoformat()
-        self.api.collector.update(
-            self.config_helper.get_conf("collector_id"),
-            {"collector_last_execution": now},
-        )
+        try:
+            message_callback()
+            now = datetime.now(timezone.utc).isoformat()
+            self.api.collector.update(
+                self.config_helper.get_conf("collector_id"),
+                {"collector_last_execution": now},
+            )
+        except Exception as err:  # pylint: disable=broad-except
+            self.collector_logger.error(str(err))
         # Then schedule the next execution
         self.scheduler.enter(
             delay, 1, self._schedule, (self.scheduler, message_callback, delay)
         )
         self.scheduler.run()
 
 
@@ -367,25 +383,32 @@
             "injector_executor_commands": config.get_conf(
                 "injector_executor_commands", default=None
             ),
             "injector_executor_clear_commands": config.get_conf(
                 "injector_executor_clear_commands", default=None
             ),
         }
+
+        self.logger_class = utils.logger(
+            config.get_conf("injector_log_level", default="info").upper(),
+            config.get_conf("injector_json_logging", default=True),
+        )
+        self.injector_logger = self.logger_class(config.get_conf("injector_name"))
+
         icon_name = config.get_conf("injector_type") + ".png"
         injector_icon = (icon_name, icon, "image/png")
         self.injector_config = self.api.injector.create(self.config, injector_icon)
         self.connect_run_and_terminate = False
         self.scheduler = sched.scheduler(time.time, time.sleep)
         # Start ping thread
         if not self.connect_run_and_terminate:
-            self.ping = PingAlive(self.api, self.config, "injector")
+            self.ping = PingAlive(
+                self.api, self.config, self.injector_logger, "injector"
+            )
             self.ping.start()
         self.listen_queue = None
 
     def listen(self, message_callback: Callable[[Dict], None]) -> None:
         self.listen_queue = ListenQueue(
-            self.config,
-            self.injector_config,
-            message_callback,
+            self.config, self.injector_config, self.injector_logger, message_callback
         )
         self.listen_queue.start()
```

### Comparing `pyobas-1.0.3/pyobas/mixins.py` & `pyobas-1.0.4/pyobas/mixins.py`

 * *Files identical despite different names*

### Comparing `pyobas-1.0.3/pyobas.egg-info/PKG-INFO` & `pyobas-1.0.4/pyobas.egg-info/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pyobas
-Version: 1.0.3
+Version: 1.0.4
 Summary: Python API client for OpenBAS.
 Home-page: https://github.com/OpenBAS-Platform/client-python
 Author: Filigran
 Author-email: contact@filigran.io
 Maintainer: Filigran
 License: Apache
 Classifier: Development Status :: 5 - Production/Stable
@@ -17,22 +17,28 @@
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python :: 3
 Classifier: Topic :: Security
 Classifier: Topic :: Software Development :: Libraries :: Python Modules
 Requires-Python: >=3.7
 Description-Content-Type: text/markdown
 License-File: LICENSE
-Requires-Dist: dataclasses-json~=0.6.4
-Requires-Dist: pika~=1.3.1
-Requires-Dist: prometheus-client~=0.20.0
+Requires-Dist: datefinder~=0.7.3
+Requires-Dist: pika~=1.3.0
+Requires-Dist: python-magic~=0.4.27; sys_platform == "linux" or sys_platform == "darwin"
+Requires-Dist: python-magic-bin~=0.4.14; sys_platform == "win32"
 Requires-Dist: python_json_logger~=2.0.4
-Requires-Dist: pyyaml~=6.0
-Requires-Dist: requests~=2.32.2
-Requires-Dist: requests-toolbelt~=1.0.0
+Requires-Dist: PyYAML~=6.0
+Requires-Dist: requests~=2.31.0
 Requires-Dist: setuptools~=70.0.0
+Requires-Dist: cachetools~=5.3.0
+Requires-Dist: prometheus-client~=0.20.0
+Requires-Dist: opentelemetry-api~=1.22.0
+Requires-Dist: opentelemetry-sdk~=1.22.0
+Requires-Dist: requests-toolbelt~=1.0.0
+Requires-Dist: dataclasses-json~=0.6.4
 Provides-Extra: dev
 Requires-Dist: black~=24.4.0; extra == "dev"
 Requires-Dist: build~=1.2.1; extra == "dev"
 Requires-Dist: isort~=5.13.0; extra == "dev"
 Requires-Dist: types-pytz~=2024.1.0.20240203; extra == "dev"
 Requires-Dist: pre-commit~=3.7.1; extra == "dev"
 Requires-Dist: types-python-dateutil~=2.9.0; extra == "dev"
```

### Comparing `pyobas-1.0.3/pyobas.egg-info/SOURCES.txt` & `pyobas-1.0.4/pyobas.egg-info/SOURCES.txt`

 * *Files 9% similar despite different names*

```diff
@@ -15,15 +15,17 @@
 pyobas.egg-info/dependency_links.txt
 pyobas.egg-info/requires.txt
 pyobas.egg-info/top_level.txt
 pyobas/apis/__init__.py
 pyobas/apis/attack_pattern.py
 pyobas/apis/collector.py
 pyobas/apis/document.py
+pyobas/apis/endpoint.py
 pyobas/apis/inject.py
+pyobas/apis/inject_expectation.py
 pyobas/apis/injector.py
 pyobas/apis/kill_chain_phase.py
 pyobas/apis/me.py
 pyobas/apis/organization.py
 pyobas/apis/team.py
 pyobas/apis/user.py
 pyobas/backends/__init__.py
```

### Comparing `pyobas-1.0.3/pyproject.toml` & `pyobas-1.0.4/pyproject.toml`

 * *Files identical despite different names*

### Comparing `pyobas-1.0.3/setup.cfg` & `pyobas-1.0.4/setup.cfg`

 * *Files 20% similar despite different names*

```diff
@@ -27,22 +27,28 @@
 packages = 
 	pyobas
 	pyobas.apis
 	pyobas.backends
 	pyobas.contracts
 include_package_data = True
 install_requires = 
-	dataclasses-json~=0.6.4
-	pika~=1.3.1
-	prometheus-client~=0.20.0
+	datefinder~=0.7.3
+	pika~=1.3.0
+	python-magic~=0.4.27; sys_platform == 'linux' or sys_platform == 'darwin'
+	python-magic-bin~=0.4.14; sys_platform == 'win32'
 	python_json_logger~=2.0.4
-	pyyaml~=6.0
-	requests~=2.32.2
-	requests-toolbelt~=1.0.0
+	PyYAML~=6.0
+	requests~=2.31.0
 	setuptools~=70.0.0
+	cachetools~=5.3.0
+	prometheus-client~=0.20.0
+	opentelemetry-api~=1.22.0
+	opentelemetry-sdk~=1.22.0
+	requests-toolbelt~=1.0.0
+	dataclasses-json~=0.6.4
 
 [options.extras_require]
 dev = 
 	black~=24.4.0
 	build~=1.2.1
 	isort~=5.13.0
 	types-pytz~=2024.1.0.20240203
```

