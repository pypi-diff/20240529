# Comparing `tmp/confidence_openfeature_provider-0.1.4.tar.gz` & `tmp/confidence_openfeature_provider-0.2.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "confidence_openfeature_provider-0.1.4.tar", last modified: Tue Feb 13 12:57:31 2024, max compression
+gzip compressed data, was "confidence_openfeature_provider-0.2.0.tar", last modified: Wed May 29 09:12:11 2024, max compression
```

## Comparing `confidence_openfeature_provider-0.1.4.tar` & `confidence_openfeature_provider-0.2.0.tar`

### file list

```diff
@@ -1,21 +1,25 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-02-13 12:57:31.904139 confidence_openfeature_provider-0.1.4/
--rw-r--r--   0 root         (0) root         (0)    11357 2024-02-13 12:57:18.000000 confidence_openfeature_provider-0.1.4/LICENSE
--rw-r--r--   0 root         (0) root         (0)    15799 2024-02-13 12:57:31.904139 confidence_openfeature_provider-0.1.4/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)     2118 2024-02-13 12:57:18.000000 confidence_openfeature_provider-0.1.4/README.md
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-02-13 12:57:31.900139 confidence_openfeature_provider-0.1.4/confidence/
--rw-r--r--   0 root         (0) root         (0)      199 2024-02-13 12:57:18.000000 confidence_openfeature_provider-0.1.4/confidence/__init__.py
--rw-r--r--   0 root         (0) root         (0)      411 2024-02-13 12:57:31.000000 confidence_openfeature_provider-0.1.4/confidence/_version.py
--rw-r--r--   0 root         (0) root         (0)      748 2024-02-13 12:57:18.000000 confidence_openfeature_provider-0.1.4/confidence/names.py
--rw-r--r--   0 root         (0) root         (0)     7505 2024-02-13 12:57:18.000000 confidence_openfeature_provider-0.1.4/confidence/provider.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-02-13 12:57:31.904139 confidence_openfeature_provider-0.1.4/confidence_openfeature_provider.egg-info/
--rw-r--r--   0 root         (0) root         (0)    15799 2024-02-13 12:57:31.000000 confidence_openfeature_provider-0.1.4/confidence_openfeature_provider.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)      474 2024-02-13 12:57:31.000000 confidence_openfeature_provider-0.1.4/confidence_openfeature_provider.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2024-02-13 12:57:31.000000 confidence_openfeature_provider-0.1.4/confidence_openfeature_provider.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)      106 2024-02-13 12:57:31.000000 confidence_openfeature_provider-0.1.4/confidence_openfeature_provider.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)       11 2024-02-13 12:57:31.000000 confidence_openfeature_provider-0.1.4/confidence_openfeature_provider.egg-info/top_level.txt
--rw-r--r--   0 root         (0) root         (0)      888 2024-02-13 12:57:18.000000 confidence_openfeature_provider-0.1.4/pyproject.toml
--rw-r--r--   0 root         (0) root         (0)       38 2024-02-13 12:57:31.904139 confidence_openfeature_provider-0.1.4/setup.cfg
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-02-13 12:57:31.904139 confidence_openfeature_provider-0.1.4/tests/
--rw-r--r--   0 root         (0) root         (0)     1054 2024-02-13 12:57:18.000000 confidence_openfeature_provider-0.1.4/tests/test_names.py
--rw-r--r--   0 root         (0) root         (0)    10394 2024-02-13 12:57:18.000000 confidence_openfeature_provider-0.1.4/tests/test_provider.py
--rw-r--r--   0 root         (0) root         (0)      971 2024-02-13 12:57:18.000000 confidence_openfeature_provider-0.1.4/tests/test_provider_parametrized.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-29 09:12:11.754631 confidence_openfeature_provider-0.2.0/
+-rw-r--r--   0 root         (0) root         (0)    11357 2024-05-29 09:12:00.000000 confidence_openfeature_provider-0.2.0/LICENSE
+-rw-r--r--   0 root         (0) root         (0)    15801 2024-05-29 09:12:11.754631 confidence_openfeature_provider-0.2.0/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)     2120 2024-05-29 09:12:00.000000 confidence_openfeature_provider-0.2.0/README.md
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-29 09:12:11.750631 confidence_openfeature_provider-0.2.0/confidence/
+-rw-r--r--   0 root         (0) root         (0)      199 2024-05-29 09:12:00.000000 confidence_openfeature_provider-0.2.0/confidence/__init__.py
+-rw-r--r--   0 root         (0) root         (0)      411 2024-05-29 09:12:11.000000 confidence_openfeature_provider-0.2.0/confidence/_version.py
+-rw-r--r--   0 root         (0) root         (0)     9407 2024-05-29 09:12:00.000000 confidence_openfeature_provider-0.2.0/confidence/confidence.py
+-rw-r--r--   0 root         (0) root         (0)     4358 2024-05-29 09:12:00.000000 confidence_openfeature_provider-0.2.0/confidence/errors.py
+-rw-r--r--   0 root         (0) root         (0)     1625 2024-05-29 09:12:00.000000 confidence_openfeature_provider-0.2.0/confidence/flag_types.py
+-rw-r--r--   0 root         (0) root         (0)      748 2024-05-29 09:12:00.000000 confidence_openfeature_provider-0.2.0/confidence/names.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-29 09:12:11.750631 confidence_openfeature_provider-0.2.0/confidence/provider/
+-rw-r--r--   0 root         (0) root         (0)     7139 2024-05-29 09:12:00.000000 confidence_openfeature_provider-0.2.0/confidence/provider/provider.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-29 09:12:11.750631 confidence_openfeature_provider-0.2.0/confidence_openfeature_provider.egg-info/
+-rw-r--r--   0 root         (0) root         (0)    15801 2024-05-29 09:12:11.000000 confidence_openfeature_provider-0.2.0/confidence_openfeature_provider.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)      554 2024-05-29 09:12:11.000000 confidence_openfeature_provider-0.2.0/confidence_openfeature_provider.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2024-05-29 09:12:11.000000 confidence_openfeature_provider-0.2.0/confidence_openfeature_provider.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)      106 2024-05-29 09:12:11.000000 confidence_openfeature_provider-0.2.0/confidence_openfeature_provider.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)       11 2024-05-29 09:12:11.000000 confidence_openfeature_provider-0.2.0/confidence_openfeature_provider.egg-info/top_level.txt
+-rw-r--r--   0 root         (0) root         (0)      888 2024-05-29 09:12:00.000000 confidence_openfeature_provider-0.2.0/pyproject.toml
+-rw-r--r--   0 root         (0) root         (0)       38 2024-05-29 09:12:11.754631 confidence_openfeature_provider-0.2.0/setup.cfg
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-29 09:12:11.750631 confidence_openfeature_provider-0.2.0/tests/
+-rw-r--r--   0 root         (0) root         (0)     1054 2024-05-29 09:12:00.000000 confidence_openfeature_provider-0.2.0/tests/test_names.py
+-rw-r--r--   0 root         (0) root         (0)    10500 2024-05-29 09:12:00.000000 confidence_openfeature_provider-0.2.0/tests/test_provider.py
+-rw-r--r--   0 root         (0) root         (0)     1037 2024-05-29 09:12:00.000000 confidence_openfeature_provider-0.2.0/tests/test_provider_parametrized.py
```

### Comparing `confidence_openfeature_provider-0.1.4/LICENSE` & `confidence_openfeature_provider-0.2.0/LICENSE`

 * *Files identical despite different names*

### Comparing `confidence_openfeature_provider-0.1.4/PKG-INFO` & `confidence_openfeature_provider-0.2.0/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: confidence_openfeature_provider
-Version: 0.1.4
+Version: 0.2.0
 Summary: Confidence provider for the OpenFeature SDK
 Author: Confidence team
 License: 
                                          Apache License
                                    Version 2.0, January 2004
                                 http://www.apache.org/licenses/
         
@@ -230,20 +230,20 @@
 and get familiar with the concepts. 
 
 ## Adding the dependency
 
 #### pip install
 <!---x-release-please-start-version-->
 ```python
-pip install confidence-openfeature-provider==0.1.4
+pip install confidence-openfeature-provider==0.2.0
 ```
 
 #### requirements.txt
 ```python
-confidence-openfeature-provider==0.1.4
+confidence-openfeature-provider==0.2.0
 
 pip install requirements.txt
 ```
 <!---x-release-please-end-->
 
 ### Creating and using the flag provider
 
@@ -258,15 +258,15 @@
 
 You can also use only the flag name `test-flag` and retrieve all values as a map with `resolve_object_details()`. 
 
 The flag's schema is validated against the requested data type, and if it doesn't match it will fall back to the default value.
 
 ```python
 
-from confidence.provider import Region
+from confidence.confidence import Region
 from confidence.provider import ConfidenceOpenFeatureProvider
 from openfeature.api import EvaluationContext
 from openfeature import api
 
 provider = ConfidenceOpenFeatureProvider("client_secret", Region.EU)
 
 api.set_provider(provider)
```

### Comparing `confidence_openfeature_provider-0.1.4/README.md` & `confidence_openfeature_provider-0.2.0/README.md`

 * *Files 2% similar despite different names*

```diff
@@ -8,20 +8,20 @@
 and get familiar with the concepts. 
 
 ## Adding the dependency
 
 #### pip install
 <!---x-release-please-start-version-->
 ```python
-pip install confidence-openfeature-provider==0.1.4
+pip install confidence-openfeature-provider==0.2.0
 ```
 
 #### requirements.txt
 ```python
-confidence-openfeature-provider==0.1.4
+confidence-openfeature-provider==0.2.0
 
 pip install requirements.txt
 ```
 <!---x-release-please-end-->
 
 ### Creating and using the flag provider
 
@@ -36,15 +36,15 @@
 
 You can also use only the flag name `test-flag` and retrieve all values as a map with `resolve_object_details()`. 
 
 The flag's schema is validated against the requested data type, and if it doesn't match it will fall back to the default value.
 
 ```python
 
-from confidence.provider import Region
+from confidence.confidence import Region
 from confidence.provider import ConfidenceOpenFeatureProvider
 from openfeature.api import EvaluationContext
 from openfeature import api
 
 provider = ConfidenceOpenFeatureProvider("client_secret", Region.EU)
 
 api.set_provider(provider)
```

### Comparing `confidence_openfeature_provider-0.1.4/confidence/names.py` & `confidence_openfeature_provider-0.2.0/confidence/names.py`

 * *Files identical despite different names*

### Comparing `confidence_openfeature_provider-0.1.4/confidence_openfeature_provider.egg-info/PKG-INFO` & `confidence_openfeature_provider-0.2.0/confidence_openfeature_provider.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: confidence_openfeature_provider
-Version: 0.1.4
+Version: 0.2.0
 Summary: Confidence provider for the OpenFeature SDK
 Author: Confidence team
 License: 
                                          Apache License
                                    Version 2.0, January 2004
                                 http://www.apache.org/licenses/
         
@@ -230,20 +230,20 @@
 and get familiar with the concepts. 
 
 ## Adding the dependency
 
 #### pip install
 <!---x-release-please-start-version-->
 ```python
-pip install confidence-openfeature-provider==0.1.4
+pip install confidence-openfeature-provider==0.2.0
 ```
 
 #### requirements.txt
 ```python
-confidence-openfeature-provider==0.1.4
+confidence-openfeature-provider==0.2.0
 
 pip install requirements.txt
 ```
 <!---x-release-please-end-->
 
 ### Creating and using the flag provider
 
@@ -258,15 +258,15 @@
 
 You can also use only the flag name `test-flag` and retrieve all values as a map with `resolve_object_details()`. 
 
 The flag's schema is validated against the requested data type, and if it doesn't match it will fall back to the default value.
 
 ```python
 
-from confidence.provider import Region
+from confidence.confidence import Region
 from confidence.provider import ConfidenceOpenFeatureProvider
 from openfeature.api import EvaluationContext
 from openfeature import api
 
 provider = ConfidenceOpenFeatureProvider("client_secret", Region.EU)
 
 api.set_provider(provider)
```

### Comparing `confidence_openfeature_provider-0.1.4/pyproject.toml` & `confidence_openfeature_provider-0.2.0/pyproject.toml`

 * *Files identical despite different names*

### Comparing `confidence_openfeature_provider-0.1.4/tests/test_names.py` & `confidence_openfeature_provider-0.2.0/tests/test_names.py`

 * *Files identical despite different names*

### Comparing `confidence_openfeature_provider-0.1.4/tests/test_provider.py` & `confidence_openfeature_provider-0.2.0/tests/test_provider.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,20 +1,23 @@
 import requests_mock
 import unittest
 import json
-from confidence.provider import ConfidenceOpenFeatureProvider
-from confidence.provider import EvaluationContext
-from confidence.provider import Region
-from confidence.provider import Reason
-from confidence import provider
+
+from openfeature.flag_evaluation import Reason
+
+import confidence.confidence
+from confidence.confidence import Confidence
+from confidence.provider.provider import ConfidenceOpenFeatureProvider
+from confidence.provider.provider import EvaluationContext
+from confidence.provider.provider import Region
 
 
 class TestMyProvider(unittest.TestCase):
     def setUp(self):
-        self.provider = ConfidenceOpenFeatureProvider(client_secret="test")
+        self.provider = ConfidenceOpenFeatureProvider(Confidence(client_secret="test"))
 
     def test_region_has_endpoint(self):
         assert Region.GLOBAL.endpoint()
 
     def test_resolve_string_with_dot_notation(self):
         ctx = EvaluationContext(targeting_key="boop")
         with requests_mock.Mocker() as mock:
@@ -57,15 +60,15 @@
 
     def test_resolve_string_with_dot_notation_request_payload(self):
         ctx = EvaluationContext(
             targeting_key="boop",
             attributes={"user": {"country": "US"}, "connection": "wifi"},
         )
         with requests_mock.Mocker() as mock:
-            provider.__version__ = "v0.0.0"
+            confidence.confidence.__version__ = "v0.0.0"
             mock.post(
                 "https://resolver.confidence.dev/v1/flags:resolve",
                 json=SUCCESSFUL_FLAG_RESOLVE,
             )
             self.provider.resolve_string_details(
                 flag_key="python-flag-1.string-key",
                 default_value="yellow",
@@ -257,15 +260,15 @@
     "targeting_key": "boop",
     "user": { "country": "US" },
     "connection": "wifi"
   },
   "apply": true,
   "flags": ["flags/python-flag-1"],
   "sdk": {
-    "id": "SDK_ID_PYTHON_PROVIDER",
+    "id": "SDK_ID_PYTHON_CONFIDENCE",
     "version": "v0.0.0"
    }
 }"""
 )
 
 SUCCESSFUL_FLAG_RESOLVE = json.loads(
     """{
```

### Comparing `confidence_openfeature_provider-0.1.4/tests/test_provider_parametrized.py` & `confidence_openfeature_provider-0.2.0/tests/test_provider_parametrized.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,20 +1,21 @@
 import pytest
 import requests_mock
 from openfeature.evaluation_context import EvaluationContext
 
-from confidence.provider import ConfidenceOpenFeatureProvider
+from confidence.confidence import Confidence
+from confidence.provider.provider import ConfidenceOpenFeatureProvider
 from tests.test_provider import SUCCESSFUL_FLAG_RESOLVE
 
 
 @pytest.mark.parametrize("apply_on_resolve", ((True, False)))
 def test_apply_configurable(apply_on_resolve):
     ctx = EvaluationContext(targeting_key="meh")
     apply_provider = ConfidenceOpenFeatureProvider(
-        client_secret="test", apply_on_resolve=apply_on_resolve
+        Confidence(client_secret="test", apply_on_resolve=apply_on_resolve)
     )
     with requests_mock.Mocker() as mock:
         mock.post(
             "https://resolver.confidence.dev/v1/flags:resolve",
             json=SUCCESSFUL_FLAG_RESOLVE,
         )
```

