# Comparing `tmp/nameguard-0.1.3.tar.gz` & `tmp/nameguard-0.1.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "nameguard-0.1.3.tar", max compression
+gzip compressed data, was "nameguard-0.1.4.tar", max compression
```

## Comparing `nameguard-0.1.3.tar` & `nameguard-0.1.4.tar`

### file list

```diff
@@ -1,39 +1,39 @@
--rw-r--r--   0        0        0     1065 2024-02-28 11:46:06.971502 nameguard-0.1.3/LICENSE
--rw-r--r--   0        0        0     3528 2024-02-28 11:46:06.971502 nameguard-0.1.3/README.md
--rw-r--r--   0        0        0       42 2024-02-28 11:46:06.971502 nameguard-0.1.3/nameguard/__init__.py
--rw-r--r--   0        0        0       62 2024-02-28 11:46:06.971502 nameguard-0.1.3/nameguard/checks/__init__.py
--rw-r--r--   0        0        0      180 2024-02-28 11:46:06.971502 nameguard-0.1.3/nameguard/checks/dna/__init__.py
--rw-r--r--   0        0        0     2491 2024-02-28 11:46:06.971502 nameguard-0.1.3/nameguard/checks/dna/normalized.py
--rw-r--r--   0        0        0     2204 2024-02-28 11:46:06.971502 nameguard-0.1.3/nameguard/checks/dna/punycode.py
--rw-r--r--   0        0        0       91 2024-02-28 11:46:06.975502 nameguard-0.1.3/nameguard/checks/grapheme/__init__.py
--rw-r--r--   0        0        0     1510 2024-02-28 11:46:06.975502 nameguard-0.1.3/nameguard/checks/grapheme/confusables.py
--rw-r--r--   0        0        0     1249 2024-02-28 11:46:06.975502 nameguard-0.1.3/nameguard/checks/grapheme/font_support.py
--rw-r--r--   0        0        0     1047 2024-02-28 11:46:06.975502 nameguard-0.1.3/nameguard/checks/grapheme/invisible.py
--rw-r--r--   0        0        0     1006 2024-02-28 11:46:06.975502 nameguard-0.1.3/nameguard/checks/grapheme/typing_difficulty.py
--rw-r--r--   0        0        0       67 2024-02-28 11:46:06.975502 nameguard-0.1.3/nameguard/checks/label/__init__.py
--rw-r--r--   0        0        0     1388 2024-02-28 11:46:06.975502 nameguard-0.1.3/nameguard/checks/label/mixed_scripts.py
--rw-r--r--   0        0        0     1536 2024-02-28 11:46:06.975502 nameguard-0.1.3/nameguard/checks/label/namewrapper.py
--rw-r--r--   0        0        0      881 2024-02-28 11:46:06.975502 nameguard-0.1.3/nameguard/checks/label/unknown.py
--rw-r--r--   0        0        0       89 2024-02-28 11:46:06.975502 nameguard-0.1.3/nameguard/checks/name/__init__.py
--rw-r--r--   0        0        0     3418 2024-02-28 11:46:06.975502 nameguard-0.1.3/nameguard/checks/name/decentralized_name.py
--rw-r--r--   0        0        0     2418 2024-02-28 11:46:06.975502 nameguard-0.1.3/nameguard/checks/name/impersonation_risk.py
--rw-r--r--   0        0        0      536 2024-02-28 11:46:06.975502 nameguard-0.1.3/nameguard/checks/name/namewrapper_fuses.py
--rw-r--r--   0        0        0      150 2024-02-28 11:46:06.975502 nameguard-0.1.3/nameguard/context.py
--rw-r--r--   0        0        0      356 2024-02-28 11:46:06.975502 nameguard-0.1.3/nameguard/endpoints.py
--rw-r--r--   0        0        0     1899 2024-02-28 11:46:06.975502 nameguard-0.1.3/nameguard/exceptions.py
--rw-r--r--   0        0        0      101 2024-02-28 11:46:06.975502 nameguard-0.1.3/nameguard/generic_utils.py
--rw-r--r--   0        0        0      262 2024-02-28 11:46:06.975502 nameguard-0.1.3/nameguard/grapheme_normalization.py
--rw-r--r--   0        0        0      100 2024-02-28 11:46:06.975502 nameguard-0.1.3/nameguard/lambda.py
--rw-r--r--   0        0        0      294 2024-02-28 11:46:06.975502 nameguard-0.1.3/nameguard/logging.py
--rw-r--r--   0        0        0      627 2024-02-28 11:46:06.975502 nameguard-0.1.3/nameguard/models/__init__.py
--rw-r--r--   0        0        0     8426 2024-02-28 11:46:06.975502 nameguard-0.1.3/nameguard/models/checks.py
--rw-r--r--   0        0        0      124 2024-02-28 11:46:06.975502 nameguard-0.1.3/nameguard/models/request.py
--rw-r--r--   0        0        0    14925 2024-02-28 11:46:06.975502 nameguard-0.1.3/nameguard/models/result.py
--rw-r--r--   0        0        0    22986 2024-02-28 11:46:06.975502 nameguard-0.1.3/nameguard/nameguard.py
--rw-r--r--   0        0        0     7799 2024-02-28 11:46:06.975502 nameguard-0.1.3/nameguard/our_ens.py
--rw-r--r--   0        0        0     1449 2024-02-28 11:46:06.975502 nameguard-0.1.3/nameguard/provider.py
--rw-r--r--   0        0        0     8864 2024-02-28 11:46:06.975502 nameguard-0.1.3/nameguard/subgraph.py
--rw-r--r--   0        0        0     6897 2024-02-28 11:46:06.975502 nameguard-0.1.3/nameguard/utils.py
--rw-r--r--   0        0        0    20055 2024-02-28 11:46:06.975502 nameguard-0.1.3/nameguard/web_api.py
--rw-r--r--   0        0        0     1399 2024-02-28 11:46:06.975502 nameguard-0.1.3/pyproject.toml
--rw-r--r--   0        0        0     4577 1970-01-01 00:00:00.000000 nameguard-0.1.3/PKG-INFO
+-rw-r--r--   0        0        0     1065 2024-05-29 11:47:47.352058 nameguard-0.1.4/LICENSE
+-rw-r--r--   0        0        0     4091 2024-05-29 11:47:47.352058 nameguard-0.1.4/README.md
+-rw-r--r--   0        0        0       42 2024-05-29 11:47:47.352058 nameguard-0.1.4/nameguard/__init__.py
+-rw-r--r--   0        0        0       62 2024-05-29 11:47:47.352058 nameguard-0.1.4/nameguard/checks/__init__.py
+-rw-r--r--   0        0        0      180 2024-05-29 11:47:47.352058 nameguard-0.1.4/nameguard/checks/dna/__init__.py
+-rw-r--r--   0        0        0     2491 2024-05-29 11:47:47.352058 nameguard-0.1.4/nameguard/checks/dna/normalized.py
+-rw-r--r--   0        0        0     2204 2024-05-29 11:47:47.352058 nameguard-0.1.4/nameguard/checks/dna/punycode.py
+-rw-r--r--   0        0        0       91 2024-05-29 11:47:47.352058 nameguard-0.1.4/nameguard/checks/grapheme/__init__.py
+-rw-r--r--   0        0        0     1510 2024-05-29 11:47:47.352058 nameguard-0.1.4/nameguard/checks/grapheme/confusables.py
+-rw-r--r--   0        0        0     1249 2024-05-29 11:47:47.352058 nameguard-0.1.4/nameguard/checks/grapheme/font_support.py
+-rw-r--r--   0        0        0     1047 2024-05-29 11:47:47.352058 nameguard-0.1.4/nameguard/checks/grapheme/invisible.py
+-rw-r--r--   0        0        0     1006 2024-05-29 11:47:47.352058 nameguard-0.1.4/nameguard/checks/grapheme/typing_difficulty.py
+-rw-r--r--   0        0        0       67 2024-05-29 11:47:47.352058 nameguard-0.1.4/nameguard/checks/label/__init__.py
+-rw-r--r--   0        0        0     1388 2024-05-29 11:47:47.352058 nameguard-0.1.4/nameguard/checks/label/mixed_scripts.py
+-rw-r--r--   0        0        0     1536 2024-05-29 11:47:47.352058 nameguard-0.1.4/nameguard/checks/label/namewrapper.py
+-rw-r--r--   0        0        0      881 2024-05-29 11:47:47.352058 nameguard-0.1.4/nameguard/checks/label/unknown.py
+-rw-r--r--   0        0        0       89 2024-05-29 11:47:47.352058 nameguard-0.1.4/nameguard/checks/name/__init__.py
+-rw-r--r--   0        0        0     3418 2024-05-29 11:47:47.352058 nameguard-0.1.4/nameguard/checks/name/decentralized_name.py
+-rw-r--r--   0        0        0     2418 2024-05-29 11:47:47.352058 nameguard-0.1.4/nameguard/checks/name/impersonation_risk.py
+-rw-r--r--   0        0        0      536 2024-05-29 11:47:47.352058 nameguard-0.1.4/nameguard/checks/name/namewrapper_fuses.py
+-rw-r--r--   0        0        0      150 2024-05-29 11:47:47.352058 nameguard-0.1.4/nameguard/context.py
+-rw-r--r--   0        0        0      356 2024-05-29 11:47:47.352058 nameguard-0.1.4/nameguard/endpoints.py
+-rw-r--r--   0        0        0     1899 2024-05-29 11:47:47.352058 nameguard-0.1.4/nameguard/exceptions.py
+-rw-r--r--   0        0        0      101 2024-05-29 11:47:47.352058 nameguard-0.1.4/nameguard/generic_utils.py
+-rw-r--r--   0        0        0      262 2024-05-29 11:47:47.352058 nameguard-0.1.4/nameguard/grapheme_normalization.py
+-rw-r--r--   0        0        0      100 2024-05-29 11:47:47.352058 nameguard-0.1.4/nameguard/lambda.py
+-rw-r--r--   0        0        0      294 2024-05-29 11:47:47.352058 nameguard-0.1.4/nameguard/logging.py
+-rw-r--r--   0        0        0      627 2024-05-29 11:47:47.352058 nameguard-0.1.4/nameguard/models/__init__.py
+-rw-r--r--   0        0        0     8426 2024-05-29 11:47:47.352058 nameguard-0.1.4/nameguard/models/checks.py
+-rw-r--r--   0        0        0      102 2024-05-29 11:47:47.352058 nameguard-0.1.4/nameguard/models/request.py
+-rw-r--r--   0        0        0    14925 2024-05-29 11:47:47.352058 nameguard-0.1.4/nameguard/models/result.py
+-rw-r--r--   0        0        0    23371 2024-05-29 11:47:47.352058 nameguard-0.1.4/nameguard/nameguard.py
+-rw-r--r--   0        0        0     7799 2024-05-29 11:47:47.352058 nameguard-0.1.4/nameguard/our_ens.py
+-rw-r--r--   0        0        0     1449 2024-05-29 11:47:47.352058 nameguard-0.1.4/nameguard/provider.py
+-rw-r--r--   0        0        0     8776 2024-05-29 11:47:47.352058 nameguard-0.1.4/nameguard/subgraph.py
+-rw-r--r--   0        0        0     6897 2024-05-29 11:47:47.352058 nameguard-0.1.4/nameguard/utils.py
+-rw-r--r--   0        0        0    20055 2024-05-29 11:47:47.352058 nameguard-0.1.4/nameguard/web_api.py
+-rw-r--r--   0        0        0     1399 2024-05-29 11:47:47.356058 nameguard-0.1.4/pyproject.toml
+-rw-r--r--   0        0        0     5140 1970-01-01 00:00:00.000000 nameguard-0.1.4/PKG-INFO
```

### Comparing `nameguard-0.1.3/LICENSE` & `nameguard-0.1.4/LICENSE`

 * *Files identical despite different names*

### Comparing `nameguard-0.1.3/README.md` & `nameguard-0.1.4/README.md`

 * *Files 8% similar despite different names*

```diff
@@ -1,39 +1,55 @@
 # NameGuard Python
 
+![Tests](https://github.com/namehash/nameguard/actions/workflows/ci_api.yml/badge.svg?branch=main)
+![Coverage](coverage_badge.svg)
+
 This repository contains the core logic for NameGuard, a python library, web API server, and AWS Lambda handler.
 
 ## Getting Started
 
-### Env variables
+### Using the public API
+
+NameGuard is hosted at <https://api.nameguard.io>
+
+You can make a basic request to the API like this:
+
+```bash
+curl https://api.nameguard.io/inspect-name/mainnet/nick.eth
+```
+
+The API documentation is available at <https://api.nameguard.io/redoc> or <https://api.nameguard.io/docs>.
+
+### Running your own NameGuard instance
+
+#### Env variables
 
 ```bash
 AWS_ROLE - AWS Role used by GitHub actions to create the CloudFormation infrastructure for deploying NameGuard as an AWS Lambda and pushing the latest build image to AWS ECR.
 SLACK_WEBHOOK_URL - Slack webhook url used by GitHub actions to send notifications of deployment success or failure to the dev team's slack channel.
 ```
 
-### Installing the library
+#### Installing the library
 
 NameGuard is available as a Python library on [PyPI](https://pypi.org/project/nameguard/). You can install it with `pip`:
 
 ```bash
 pip install nameguard
 ```
 
-### Setting Provider URIs
+#### Setting Provider URIs
 
 NameGuard uses the specified Provider endpoint (e.g. Alchemy, Infura, your own Ethereum node, etc...) for `secure-primary-name/`. Provider endpoints have to be set by environment variables, e.g.:
 
 ```bash
 export PROVIDER_URI_MAINNET=https://eth-mainnet.g.alchemy.com/v2/[YOUR_ALCHEMY_API_KEY]
-export PROVIDER_URI_GOERLI=https://eth-goerli.g.alchemy.com/v2/[YOUR_ALCHEMY_API_KEY]
 export PROVIDER_URI_SEPOLIA=https://eth-sepolia.g.alchemy.com/v2/[YOUR_ALCHEMY_API_KEY]
 ```
 
-### Starting the web server
+#### Starting the web server
 
 A FastAPI application is included in the `nameguard.web_api` module. The default installation from PyPI does not include an ASGI server, so you will need to install one separately. For example, to install [uvicorn](https://www.uvicorn.org):
 
 ```bash
 pip install 'uvicorn[standard]'
 ```
 
@@ -101,7 +117,13 @@
 ### Disable monkeypatch tests
 
 By default, the tests are using mock responses from external APIs. If you want to run tests using real requests to external APIs then set `MONKEYPATCH=0`.
 
 ```bash
 MONKEYPATCH=0 poetry run pytest
 ```
+
+## License
+
+Licensed under the MIT License, Copyright © 2023-present [NameHash Labs](https://namehashlabs.org).
+
+See [LICENSE](./LICENSE) for more information.
```

#### encoding

```diff
@@ -1 +1 @@
-us-ascii
+utf-8
```

### Comparing `nameguard-0.1.3/nameguard/checks/dna/normalized.py` & `nameguard-0.1.4/nameguard/checks/dna/normalized.py`

 * *Files identical despite different names*

### Comparing `nameguard-0.1.3/nameguard/checks/dna/punycode.py` & `nameguard-0.1.4/nameguard/checks/dna/punycode.py`

 * *Files identical despite different names*

### Comparing `nameguard-0.1.3/nameguard/checks/grapheme/confusables.py` & `nameguard-0.1.4/nameguard/checks/grapheme/confusables.py`

 * *Files identical despite different names*

### Comparing `nameguard-0.1.3/nameguard/checks/grapheme/font_support.py` & `nameguard-0.1.4/nameguard/checks/grapheme/font_support.py`

 * *Files identical despite different names*

### Comparing `nameguard-0.1.3/nameguard/checks/grapheme/invisible.py` & `nameguard-0.1.4/nameguard/checks/grapheme/invisible.py`

 * *Files identical despite different names*

### Comparing `nameguard-0.1.3/nameguard/checks/grapheme/typing_difficulty.py` & `nameguard-0.1.4/nameguard/checks/grapheme/typing_difficulty.py`

 * *Files identical despite different names*

### Comparing `nameguard-0.1.3/nameguard/checks/label/mixed_scripts.py` & `nameguard-0.1.4/nameguard/checks/label/mixed_scripts.py`

 * *Files identical despite different names*

### Comparing `nameguard-0.1.3/nameguard/checks/label/namewrapper.py` & `nameguard-0.1.4/nameguard/checks/label/namewrapper.py`

 * *Files identical despite different names*

### Comparing `nameguard-0.1.3/nameguard/checks/label/unknown.py` & `nameguard-0.1.4/nameguard/checks/label/unknown.py`

 * *Files identical despite different names*

### Comparing `nameguard-0.1.3/nameguard/checks/name/decentralized_name.py` & `nameguard-0.1.4/nameguard/checks/name/decentralized_name.py`

 * *Files identical despite different names*

### Comparing `nameguard-0.1.3/nameguard/checks/name/impersonation_risk.py` & `nameguard-0.1.4/nameguard/checks/name/impersonation_risk.py`

 * *Files identical despite different names*

### Comparing `nameguard-0.1.3/nameguard/checks/name/namewrapper_fuses.py` & `nameguard-0.1.4/nameguard/checks/name/namewrapper_fuses.py`

 * *Files identical despite different names*

### Comparing `nameguard-0.1.3/nameguard/exceptions.py` & `nameguard-0.1.4/nameguard/exceptions.py`

 * *Files identical despite different names*

### Comparing `nameguard-0.1.3/nameguard/models/__init__.py` & `nameguard-0.1.4/nameguard/models/__init__.py`

 * *Files identical despite different names*

### Comparing `nameguard-0.1.3/nameguard/models/checks.py` & `nameguard-0.1.4/nameguard/models/checks.py`

 * *Files identical despite different names*

### Comparing `nameguard-0.1.3/nameguard/models/result.py` & `nameguard-0.1.4/nameguard/models/result.py`

 * *Files identical despite different names*

### Comparing `nameguard-0.1.3/nameguard/nameguard.py` & `nameguard-0.1.4/nameguard/nameguard.py`

 * *Files 2% similar despite different names*

```diff
@@ -122,15 +122,14 @@
     def __init__(self):
         self._inspector = init_inspector()
         load_dotenv()
         # TODO use web sockets and async
         self.ns = {}
         for network_name, env_var in (
             (NetworkName.MAINNET, 'PROVIDER_URI_MAINNET'),
-            (NetworkName.GOERLI, 'PROVIDER_URI_GOERLI'),
             (NetworkName.SEPOLIA, 'PROVIDER_URI_SEPOLIA'),
         ):
             if os.environ.get(env_var) is None:
                 logger.warning(f'Environment variable {env_var} is not set')
             self.ns[network_name] = OurENS(HTTPProvider(os.environ.get(env_var)))
 
         # optimization
@@ -143,22 +142,31 @@
 
     async def inspect_name(
         self, network_name: NetworkName, name: str, resolve_labelhashes: bool = True, bulk_mode: bool = False
     ) -> Union[NameGuardReport, ConsolidatedNameGuardReport]:
         """
         Inspect a name. A name is a sequence of labels separated by dots.
         A label can be a labelhash or a string.
+        If a labelhash is encountered and `resolve_labelhashes` is `True`, a lookup will be performed.
+        """
+        if resolve_labelhashes:
+            name = await resolve_all_labelhashes_in_name_querying_labelhashes(network_name, name)
+        return self.inspect_name_sync(name, bulk_mode)
+
+    def inspect_name_sync(
+        self, name: str, bulk_mode: bool = False
+    ) -> Union[NameGuardReport, ConsolidatedNameGuardReport]:
+        """
+        Inspect a name. A name is a sequence of labels separated by dots.
+        A label can be a labelhash or a string.
         If a labelhash is encountered, it will be treated as an unknown label.
         """
 
         logger.debug(f"[inspect_name] name: '{name}'")
 
-        if resolve_labelhashes:
-            name = await resolve_all_labelhashes_in_name_querying_labelhashes(network_name, name)
-
         if bulk_mode and simple_name(name):
             return consolidated_report_from_simple_name(name)
 
         labels = [] if len(name) == 0 else name.split('.')
         logger.debug(f'[inspect_name] labels: {labels}')
 
         # labelhashes have `None` as their analysis
```

### Comparing `nameguard-0.1.3/nameguard/our_ens.py` & `nameguard-0.1.4/nameguard/our_ens.py`

 * *Files identical despite different names*

### Comparing `nameguard-0.1.3/nameguard/provider.py` & `nameguard-0.1.4/nameguard/provider.py`

 * *Files identical despite different names*

### Comparing `nameguard-0.1.3/nameguard/subgraph.py` & `nameguard-0.1.4/nameguard/subgraph.py`

 * *Files 1% similar despite different names*

```diff
@@ -11,15 +11,14 @@
 
 # The label limit for using the multi-label lookup query.
 # Longer names will be resolved by querying the namehash of the full name.
 MAX_MULTI_LABEL_LOOKUP = 256
 
 ENS_SUBGRAPH_URL = {
     NetworkName.MAINNET: 'https://api.thegraph.com/subgraphs/name/ensdomains/ens',
-    NetworkName.GOERLI: 'https://api.thegraph.com/subgraphs/name/ensdomains/ensgoerli',
     NetworkName.SEPOLIA: 'https://api.studio.thegraph.com/proxy/49574/enssepolia/version/latest',
 }
 
 
 RESOLVE_NAMEHASH_QUERY = """
 query resolveNamehash($nameHash: String) {
   domain(id: $nameHash) {
```

### Comparing `nameguard-0.1.3/nameguard/utils.py` & `nameguard-0.1.4/nameguard/utils.py`

 * *Files identical despite different names*

### Comparing `nameguard-0.1.3/nameguard/web_api.py` & `nameguard-0.1.4/nameguard/web_api.py`

 * *Files identical despite different names*

### Comparing `nameguard-0.1.3/pyproject.toml` & `nameguard-0.1.4/pyproject.toml`

 * *Files 7% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "nameguard"
-version = "0.1.3"
+version = "0.1.4"
 description = "Security \"x-ray\" for ENS names"
 authors = ["NameHash Team <devops@namehash.io>"]
 maintainers = ["NameHash Team <devops@namehash.io>"]
 homepage = "https://github.com/namehash/nameguard"
 repository = "https://github.com/namehash/nameguard"
 readme = "README.md"
 license = "LICENSE"
```

### Comparing `nameguard-0.1.3/PKG-INFO` & `nameguard-0.1.4/PKG-INFO`

 * *Files 18% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: nameguard
-Version: 0.1.3
+Version: 0.1.4
 Summary: Security "x-ray" for ENS names
 Home-page: https://github.com/namehash/nameguard
 License: LICENSE
 Author: NameHash Team
 Author-email: devops@namehash.io
 Maintainer: NameHash Team
 Maintainer-email: devops@namehash.io
@@ -24,44 +24,60 @@
 Requires-Dist: python-dotenv (>=1.0.0,<2.0.0)
 Requires-Dist: web3 (==6.11.1)
 Project-URL: Repository, https://github.com/namehash/nameguard
 Description-Content-Type: text/markdown
 
 # NameGuard Python
 
+![Tests](https://github.com/namehash/nameguard/actions/workflows/ci_api.yml/badge.svg?branch=main)
+![Coverage](coverage_badge.svg)
+
 This repository contains the core logic for NameGuard, a python library, web API server, and AWS Lambda handler.
 
 ## Getting Started
 
-### Env variables
+### Using the public API
+
+NameGuard is hosted at <https://api.nameguard.io>
+
+You can make a basic request to the API like this:
+
+```bash
+curl https://api.nameguard.io/inspect-name/mainnet/nick.eth
+```
+
+The API documentation is available at <https://api.nameguard.io/redoc> or <https://api.nameguard.io/docs>.
+
+### Running your own NameGuard instance
+
+#### Env variables
 
 ```bash
 AWS_ROLE - AWS Role used by GitHub actions to create the CloudFormation infrastructure for deploying NameGuard as an AWS Lambda and pushing the latest build image to AWS ECR.
 SLACK_WEBHOOK_URL - Slack webhook url used by GitHub actions to send notifications of deployment success or failure to the dev team's slack channel.
 ```
 
-### Installing the library
+#### Installing the library
 
 NameGuard is available as a Python library on [PyPI](https://pypi.org/project/nameguard/). You can install it with `pip`:
 
 ```bash
 pip install nameguard
 ```
 
-### Setting Provider URIs
+#### Setting Provider URIs
 
 NameGuard uses the specified Provider endpoint (e.g. Alchemy, Infura, your own Ethereum node, etc...) for `secure-primary-name/`. Provider endpoints have to be set by environment variables, e.g.:
 
 ```bash
 export PROVIDER_URI_MAINNET=https://eth-mainnet.g.alchemy.com/v2/[YOUR_ALCHEMY_API_KEY]
-export PROVIDER_URI_GOERLI=https://eth-goerli.g.alchemy.com/v2/[YOUR_ALCHEMY_API_KEY]
 export PROVIDER_URI_SEPOLIA=https://eth-sepolia.g.alchemy.com/v2/[YOUR_ALCHEMY_API_KEY]
 ```
 
-### Starting the web server
+#### Starting the web server
 
 A FastAPI application is included in the `nameguard.web_api` module. The default installation from PyPI does not include an ASGI server, so you will need to install one separately. For example, to install [uvicorn](https://www.uvicorn.org):
 
 ```bash
 pip install 'uvicorn[standard]'
 ```
 
@@ -130,7 +146,13 @@
 
 By default, the tests are using mock responses from external APIs. If you want to run tests using real requests to external APIs then set `MONKEYPATCH=0`.
 
 ```bash
 MONKEYPATCH=0 poetry run pytest
 ```
 
+## License
+
+Licensed under the MIT License, Copyright © 2023-present [NameHash Labs](https://namehashlabs.org).
+
+See [LICENSE](./LICENSE) for more information.
+
```

#### encoding

```diff
@@ -1 +1 @@
-us-ascii
+utf-8
```

