# Comparing `tmp/curve_dao-0.0.5.tar.gz` & `tmp/curve_dao-0.0.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "curve_dao-0.0.5.tar", last modified: Tue Apr 23 19:03:05 2024, max compression
+gzip compressed data, was "curve_dao-0.0.6.tar", last modified: Wed May 29 13:21:44 2024, max compression
```

## Comparing `curve_dao-0.0.5.tar` & `curve_dao-0.0.6.tar`

### file list

```diff
@@ -1,19 +1,19 @@
-drwxr-xr-x   0 swadhinnanda   (501) staff       (20)        0 2024-04-23 19:03:05.405404 curve_dao-0.0.5/
--rw-r--r--   0 swadhinnanda   (501) staff       (20)     1933 2024-04-23 19:03:05.405117 curve_dao-0.0.5/PKG-INFO
--rw-r--r--   0 swadhinnanda   (501) staff       (20)     1060 2024-04-23 15:39:50.000000 curve_dao-0.0.5/README.md
-drwxr-xr-x   0 swadhinnanda   (501) staff       (20)        0 2024-04-23 19:03:05.401924 curve_dao-0.0.5/curve_dao/
--rw-r--r--   0 swadhinnanda   (501) staff       (20)     1228 2024-04-23 19:01:23.000000 curve_dao-0.0.5/curve_dao/__init__.py
--rw-r--r--   0 swadhinnanda   (501) staff       (20)     1415 2024-04-23 16:43:33.000000 curve_dao-0.0.5/curve_dao/addresses.py
--rw-r--r--   0 swadhinnanda   (501) staff       (20)     1247 2024-04-23 19:01:23.000000 curve_dao-0.0.5/curve_dao/ipfs.py
--rw-r--r--   0 swadhinnanda   (501) staff       (20)     1544 2024-04-23 19:01:23.000000 curve_dao-0.0.5/curve_dao/simulate.py
--rw-r--r--   0 swadhinnanda   (501) staff       (20)     1763 2024-04-23 19:01:23.000000 curve_dao-0.0.5/curve_dao/vote_utils.py
-drwxr-xr-x   0 swadhinnanda   (501) staff       (20)        0 2024-04-23 19:03:05.404776 curve_dao-0.0.5/curve_dao.egg-info/
--rw-r--r--   0 swadhinnanda   (501) staff       (20)     1933 2024-04-23 19:03:05.000000 curve_dao-0.0.5/curve_dao.egg-info/PKG-INFO
--rw-r--r--   0 swadhinnanda   (501) staff       (20)      322 2024-04-23 19:03:05.000000 curve_dao-0.0.5/curve_dao.egg-info/SOURCES.txt
--rw-r--r--   0 swadhinnanda   (501) staff       (20)        1 2024-04-23 19:03:05.000000 curve_dao-0.0.5/curve_dao.egg-info/dependency_links.txt
--rw-r--r--   0 swadhinnanda   (501) staff       (20)       34 2024-04-23 19:03:05.000000 curve_dao-0.0.5/curve_dao.egg-info/requires.txt
--rw-r--r--   0 swadhinnanda   (501) staff       (20)       10 2024-04-23 19:03:05.000000 curve_dao-0.0.5/curve_dao.egg-info/top_level.txt
--rw-r--r--   0 swadhinnanda   (501) staff       (20)     1173 2024-04-23 19:01:22.000000 curve_dao-0.0.5/pyproject.toml
--rw-r--r--   0 swadhinnanda   (501) staff       (20)       38 2024-04-23 19:03:05.405464 curve_dao-0.0.5/setup.cfg
-drwxr-xr-x   0 swadhinnanda   (501) staff       (20)        0 2024-04-23 19:03:05.404385 curve_dao-0.0.5/tests/
--rw-r--r--   0 swadhinnanda   (501) staff       (20)     1908 2024-04-23 18:46:45.000000 curve_dao-0.0.5/tests/test_kill_gauge.py
+drwxr-xr-x   0 swadhinnanda   (501) staff       (20)        0 2024-05-29 13:21:44.724580 curve_dao-0.0.6/
+-rw-r--r--   0 swadhinnanda   (501) staff       (20)     1853 2024-05-29 13:21:44.724254 curve_dao-0.0.6/PKG-INFO
+-rw-r--r--   0 swadhinnanda   (501) staff       (20)      980 2024-05-29 13:20:42.000000 curve_dao-0.0.6/README.md
+drwxr-xr-x   0 swadhinnanda   (501) staff       (20)        0 2024-05-29 13:21:44.722720 curve_dao-0.0.6/curve_dao/
+-rw-r--r--   0 swadhinnanda   (501) staff       (20)     1228 2024-04-23 19:01:23.000000 curve_dao-0.0.6/curve_dao/__init__.py
+-rw-r--r--   0 swadhinnanda   (501) staff       (20)     1196 2024-05-29 13:15:59.000000 curve_dao-0.0.6/curve_dao/addresses.py
+-rw-r--r--   0 swadhinnanda   (501) staff       (20)     1247 2024-04-23 19:01:23.000000 curve_dao-0.0.6/curve_dao/ipfs.py
+-rw-r--r--   0 swadhinnanda   (501) staff       (20)     1544 2024-04-23 19:01:23.000000 curve_dao-0.0.6/curve_dao/simulate.py
+-rw-r--r--   0 swadhinnanda   (501) staff       (20)     1763 2024-04-23 19:01:23.000000 curve_dao-0.0.6/curve_dao/vote_utils.py
+drwxr-xr-x   0 swadhinnanda   (501) staff       (20)        0 2024-05-29 13:21:44.723902 curve_dao-0.0.6/curve_dao.egg-info/
+-rw-r--r--   0 swadhinnanda   (501) staff       (20)     1853 2024-05-29 13:21:44.000000 curve_dao-0.0.6/curve_dao.egg-info/PKG-INFO
+-rw-r--r--   0 swadhinnanda   (501) staff       (20)      322 2024-05-29 13:21:44.000000 curve_dao-0.0.6/curve_dao.egg-info/SOURCES.txt
+-rw-r--r--   0 swadhinnanda   (501) staff       (20)        1 2024-05-29 13:21:44.000000 curve_dao-0.0.6/curve_dao.egg-info/dependency_links.txt
+-rw-r--r--   0 swadhinnanda   (501) staff       (20)       34 2024-05-29 13:21:44.000000 curve_dao-0.0.6/curve_dao.egg-info/requires.txt
+-rw-r--r--   0 swadhinnanda   (501) staff       (20)       10 2024-05-29 13:21:44.000000 curve_dao-0.0.6/curve_dao.egg-info/top_level.txt
+-rw-r--r--   0 swadhinnanda   (501) staff       (20)     1173 2024-05-29 13:20:25.000000 curve_dao-0.0.6/pyproject.toml
+-rw-r--r--   0 swadhinnanda   (501) staff       (20)       38 2024-05-29 13:21:44.724630 curve_dao-0.0.6/setup.cfg
+drwxr-xr-x   0 swadhinnanda   (501) staff       (20)        0 2024-05-29 13:21:44.723695 curve_dao-0.0.6/tests/
+-rw-r--r--   0 swadhinnanda   (501) staff       (20)     1858 2024-05-29 13:21:16.000000 curve_dao-0.0.6/tests/test_kill_gauge.py
```

### Comparing `curve_dao-0.0.5/PKG-INFO` & `curve_dao-0.0.6/PKG-INFO`

 * *Files 24% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: curve-dao
-Version: 0.0.5
+Version: 0.0.6
 Summary: DAO governance tools for CurveDAO.
 Author-email: FiddyResearch <fiddyresearch@gmail.com>
 Maintainer-email: FiddyResearch <fiddyresearch@gmail.com>
 License: AGPL-3.0-only License
 Project-URL: Homepage, https://pypi.org/project/curve-dao/
 Project-URL: GitHub, https://github.com/bout3fiddy/curve-dao
 Project-URL: Changelog, https://github.com/bout3fiddy/curve-dao/blob/main/CHANGELOG.md
@@ -15,28 +15,38 @@
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.10
 Description-Content-Type: text/markdown
 Requires-Dist: titanoboa>=0.1.10b1
 Requires-Dist: requests
 Requires-Dist: rich
 
-# Curve DAO Operations
+# What is this?
 
-This repository contains tools, written in python, for Curve DAO operations. The goal is to provide a simple command-line interface that allows veCRV holders to create and decode on-chain executable proposals, and simple scripts to produce analytics on governance in the Curve DAO.
-
-Such a CLI tool allows independence from a web-ui: after all, decentralisation goes beyond just network decentralisation: it more or less means democratic access to technology.
+Simple python package to simulate on-chain CurveDAO proposals and publish proposals for DAO voting on-chain.
 
 # Who needs this?
 
 veCRV holders looking to create on-chain proposals such as
 
 - Creating or killing Curve DAO gauges that reward CRV inflation to addresses (liquidity pools or otherwise).
 - Creating a smartwallet whitelist to lock veCRV (veCRV restricts smart contracts to lock CRV, subject to a DAO whitelist vote)
 - Changing liquidity pool parameters
 - Adding gauge types ...
 - ... etc.
 
 Curve DAO stakeholders have the ability to change the protocol in many ways. This repository is an attempt to consolidate all on-chain DAO operations into a single tool.
 
-# Setup
+# How does one install it?
+
+`pip install curve-dao`
+
+# How does one contribute?
+
+1. Pull Requests.
+2. Create issues.
+3. ...
+
+# How does one build and publish?
 
-...
+1. Update codebase
+2. Up version in pyproject.toml
+3. `python -m build; python -m twine upload --repository pypi dist/* --verbose`
```

### Comparing `curve_dao-0.0.5/curve_dao/__init__.py` & `curve_dao-0.0.6/curve_dao/__init__.py`

 * *Files identical despite different names*

### Comparing `curve_dao-0.0.5/curve_dao/addresses.py` & `curve_dao-0.0.6/curve_dao/addresses.py`

 * *Files 9% similar despite different names*

```diff
@@ -8,22 +8,15 @@
 CURVE_DAO_PARAM = {
     "agent": "0x4eeb3ba4f221ca16ed4a0cc7254e2e32df948c5f",
     "voting": "0xbcff8b0b9419b9a88c44546519b1e909cf330399",
     "token": "0x5f3b5DfEb7B28CDbD7FAba78963EE202a494e2A2",
     "quorum": 15,
 }
 
-EMERGENCY_DAO = {
-    "forwarder": "0xf409Ce40B5bb1e4Ef8e97b1979629859c6d5481f",
-    "agent": "0x00669DF67E4827FCc0E48A1838a8d5AB79281909",
-    "voting": "0x1115c9b3168563354137cdc60efb66552dd50678",
-    "token": "0x4c0947B16FB1f755A2D32EC21A0c4181f711C500",
-    "quorum": 51,
-}
-
+EMERGENCY_DAO = "0x467947EE34aF926cF1DCac093870f613C96B1E0c"
 GAUGE_CONTROLLER = "0x2F50D538606Fa9EDD2B11E2446BEb18C9D5846bB"
 VOTING_ESCROW = "0x5f3b5DfEb7B28CDbD7FAba78963EE202a494e2A2"
 veCRV = VOTING_ESCROW
 CRV = "0xD533a949740bb3306d119CC777fa900bA034cd52"
 CONVEX_VOTERPROXY = "0x989AEB4D175E16225E39E87D0D97A3360524AD80"
 ADDRESSPROVIDER = "0x5ffe7FB82894076ECB99A30D6A32e969e6e35E98"  # On all chains
```

### Comparing `curve_dao-0.0.5/curve_dao/ipfs.py` & `curve_dao-0.0.6/curve_dao/ipfs.py`

 * *Files identical despite different names*

### Comparing `curve_dao-0.0.5/curve_dao/simulate.py` & `curve_dao-0.0.6/curve_dao/simulate.py`

 * *Files identical despite different names*

### Comparing `curve_dao-0.0.5/curve_dao/vote_utils.py` & `curve_dao-0.0.6/curve_dao/vote_utils.py`

 * *Files identical despite different names*

### Comparing `curve_dao-0.0.5/curve_dao.egg-info/PKG-INFO` & `curve_dao-0.0.6/curve_dao.egg-info/PKG-INFO`

 * *Files 24% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: curve-dao
-Version: 0.0.5
+Version: 0.0.6
 Summary: DAO governance tools for CurveDAO.
 Author-email: FiddyResearch <fiddyresearch@gmail.com>
 Maintainer-email: FiddyResearch <fiddyresearch@gmail.com>
 License: AGPL-3.0-only License
 Project-URL: Homepage, https://pypi.org/project/curve-dao/
 Project-URL: GitHub, https://github.com/bout3fiddy/curve-dao
 Project-URL: Changelog, https://github.com/bout3fiddy/curve-dao/blob/main/CHANGELOG.md
@@ -15,28 +15,38 @@
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.10
 Description-Content-Type: text/markdown
 Requires-Dist: titanoboa>=0.1.10b1
 Requires-Dist: requests
 Requires-Dist: rich
 
-# Curve DAO Operations
+# What is this?
 
-This repository contains tools, written in python, for Curve DAO operations. The goal is to provide a simple command-line interface that allows veCRV holders to create and decode on-chain executable proposals, and simple scripts to produce analytics on governance in the Curve DAO.
-
-Such a CLI tool allows independence from a web-ui: after all, decentralisation goes beyond just network decentralisation: it more or less means democratic access to technology.
+Simple python package to simulate on-chain CurveDAO proposals and publish proposals for DAO voting on-chain.
 
 # Who needs this?
 
 veCRV holders looking to create on-chain proposals such as
 
 - Creating or killing Curve DAO gauges that reward CRV inflation to addresses (liquidity pools or otherwise).
 - Creating a smartwallet whitelist to lock veCRV (veCRV restricts smart contracts to lock CRV, subject to a DAO whitelist vote)
 - Changing liquidity pool parameters
 - Adding gauge types ...
 - ... etc.
 
 Curve DAO stakeholders have the ability to change the protocol in many ways. This repository is an attempt to consolidate all on-chain DAO operations into a single tool.
 
-# Setup
+# How does one install it?
+
+`pip install curve-dao`
+
+# How does one contribute?
+
+1. Pull Requests.
+2. Create issues.
+3. ...
+
+# How does one build and publish?
 
-...
+1. Update codebase
+2. Up version in pyproject.toml
+3. `python -m build; python -m twine upload --repository pypi dist/* --verbose`
```

### Comparing `curve_dao-0.0.5/pyproject.toml` & `curve_dao-0.0.6/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [project]
 name = "curve-dao"
-version = "0.0.5"
+version = "0.0.6"
 description = "DAO governance tools for CurveDAO."
 readme = {file = "README.md", content-type = "text/markdown"}
 requires-python = ">=3.10"
 license = {text = "AGPL-3.0-only License"}
 keywords = ["ethereum", "smart-contracts", "evm", "vyper", "curve-finance", "dao", "defi"]
 authors = [
     {name = "FiddyResearch", email = "fiddyresearch@gmail.com"},
```

### Comparing `curve_dao-0.0.5/tests/test_kill_gauge.py` & `curve_dao-0.0.6/tests/test_kill_gauge.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,63 +1,63 @@
 import boa
-import curve_dao
 import pytest
 
+import curve_dao
+
+
 @pytest.fixture
 def gauge_to_kill(etherscan_api_key):
     return boa.from_etherscan(
-        '0x04e80db3f84873e4132b221831af1045d27f140f',
+        "0x04e80db3f84873e4132b221831af1045d27f140f",
         name="LiquidityGaugeV6",
-        api_key=etherscan_api_key
+        api_key=etherscan_api_key,
     )
 
 
 @pytest.fixture
 def actions(gauge_to_kill):
-    return [(gauge_to_kill.address, 'set_killed', True)]
+    return [(gauge_to_kill.address, "set_killed", True)]
 
 
 @pytest.fixture
 def description():
     return "test"
-    
-    
+
+
 @pytest.fixture
 def target():
     return curve_dao.addresses.CURVE_DAO_OWNERSHIP
 
 
 @pytest.fixture
 def evm_script(target, actions, etherscan_api_key):
     return curve_dao.prepare_evm_script(target, actions, etherscan_api_key)
 
 
 def test_evm_script(evm_script):
-    assert evm_script.hex() == "0000000140907540d8a6c65c637785e8f8b742ae6b0b9968000000c4b61d27f600000000000000000000000004e80db3f84873e4132b221831af1045d27f140f00000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000060000000000000000000000000000000000000000000000000000000000000002490b22997000000000000000000000000000000000000000000000000000000000000000100000000000000000000000000000000000000000000000000000000"
-    
-    
+    assert (
+        evm_script.hex()
+        == "0000000140907540d8a6c65c637785e8f8b742ae6b0b9968000000c4b61d27f600000000000000000000000004e80db3f84873e4132b221831af1045d27f140f00000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000000060000000000000000000000000000000000000000000000000000000000000002490b22997000000000000000000000000000000000000000000000000000000000000000100000000000000000000000000000000000000000000000000000000"
+    )
+
+
 @pytest.mark.ignore_isolation
 @pytest.fixture
 def test_create_vote(
     target, actions, description, etherscan_api_key, pinata_token, vote_creator
 ):
     with boa.env.prank(vote_creator):
         vote_id = curve_dao.create_vote(
-            target, 
-            actions, 
-            description, 
-            etherscan_api_key, 
-            pinata_token
+            target, actions, description, etherscan_api_key, pinata_token
         )
     return vote_id
 
 
 @pytest.mark.ignore_isolation
 @pytest.fixture
 def test_simulate(test_create_vote, target, etherscan_api_key):
-    
     vote_id = test_create_vote
-    assert curve_dao.simulate(vote_id, target['voting'], etherscan_api_key)
-    
+    assert curve_dao.simulate(vote_id, target["voting"], etherscan_api_key)
+
 
 def test_gauge_killed(test_create_vote, test_simulate, gauge_to_kill):
-    assert gauge_to_kill.is_killed() == True
+    assert gauge_to_kill.is_killed() is True
```

