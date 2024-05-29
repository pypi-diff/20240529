# Comparing `tmp/web3mc-0.1.6.tar.gz` & `tmp/web3mc-0.1.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "web3mc-0.1.6.tar", max compression
+gzip compressed data, was "web3mc-0.1.7.tar", max compression
```

## Comparing `web3mc-0.1.6.tar` & `web3mc-0.1.7.tar`

### file list

```diff
@@ -1,11 +1,11 @@
--rw-r--r--   0        0        0     1056 2023-12-31 14:19:21.425876 web3mc-0.1.6/LICENSE
--rw-r--r--   0        0        0     2649 2023-12-31 14:19:21.425876 web3mc-0.1.6/README.md
--rw-r--r--   0        0        0      889 2023-12-31 14:19:21.425876 web3mc-0.1.6/pyproject.toml
--rw-r--r--   0        0        0       58 2023-12-31 14:19:21.429875 web3mc-0.1.6/web3mc/__init__.py
--rw-r--r--   0        0        0    14532 2023-12-31 14:19:21.429875 web3mc-0.1.6/web3mc/abi.py
--rw-r--r--   0        0        0       58 2023-12-31 14:19:21.429875 web3mc-0.1.6/web3mc/auto.py
--rw-r--r--   0        0        0     1545 2023-12-31 14:19:21.429875 web3mc-0.1.6/web3mc/call.py
--rw-r--r--   0        0        0    20838 2023-12-31 14:19:21.429875 web3mc-0.1.6/web3mc/constants.py
--rw-r--r--   0        0        0       46 2023-12-31 14:19:21.429875 web3mc-0.1.6/web3mc/exceptions.py
--rw-r--r--   0        0        0     7739 2023-12-31 14:19:21.429875 web3mc-0.1.6/web3mc/multicall.py
--rw-r--r--   0        0        0     3224 1970-01-01 00:00:00.000000 web3mc-0.1.6/PKG-INFO
+-rw-r--r--   0        0        0     1056 2024-05-29 20:45:12.040066 web3mc-0.1.7/LICENSE
+-rw-r--r--   0        0        0     2649 2024-05-29 20:45:12.040066 web3mc-0.1.7/README.md
+-rw-r--r--   0        0        0      889 2024-05-29 20:45:12.040066 web3mc-0.1.7/pyproject.toml
+-rw-r--r--   0        0        0       58 2024-05-29 20:45:12.040066 web3mc-0.1.7/web3mc/__init__.py
+-rw-r--r--   0        0        0    14532 2024-05-29 20:45:12.040066 web3mc-0.1.7/web3mc/abi.py
+-rw-r--r--   0        0        0       58 2024-05-29 20:45:12.040066 web3mc-0.1.7/web3mc/auto.py
+-rw-r--r--   0        0        0     1545 2024-05-29 20:45:12.040066 web3mc-0.1.7/web3mc/call.py
+-rw-r--r--   0        0        0    21006 2024-05-29 20:45:12.040066 web3mc-0.1.7/web3mc/constants.py
+-rw-r--r--   0        0        0       46 2024-05-29 20:45:12.040066 web3mc-0.1.7/web3mc/exceptions.py
+-rw-r--r--   0        0        0     7739 2024-05-29 20:45:12.040066 web3mc-0.1.7/web3mc/multicall.py
+-rw-r--r--   0        0        0     3224 1970-01-01 00:00:00.000000 web3mc-0.1.7/PKG-INFO
```

### Comparing `web3mc-0.1.6/LICENSE` & `web3mc-0.1.7/LICENSE`

 * *Files identical despite different names*

### Comparing `web3mc-0.1.6/README.md` & `web3mc-0.1.7/README.md`

 * *Files identical despite different names*

### Comparing `web3mc-0.1.6/pyproject.toml` & `web3mc-0.1.7/pyproject.toml`

 * *Files 17% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "web3mc"
-version = "0.1.6"
+version = "0.1.7"
 description = "Multicall library for aggregating web3py contract calls"
 authors = ["amfet42"]
 license = "MIT"
 readme = "README.md"
 repository = "https://github.com/amfet42/web3mc"
 keywords = ["web3", "multicall"]
```

### Comparing `web3mc-0.1.6/web3mc/abi.py` & `web3mc-0.1.7/web3mc/abi.py`

 * *Files identical despite different names*

### Comparing `web3mc-0.1.6/web3mc/call.py` & `web3mc-0.1.7/web3mc/call.py`

 * *Files identical despite different names*

### Comparing `web3mc-0.1.6/web3mc/constants.py` & `web3mc-0.1.7/web3mc/constants.py`

 * *Files 0% similar despite different names*

```diff
@@ -144,15 +144,17 @@
     Gnosis = 100
     Velas = 106
     Thundercore = 108
     Coston2Testnet = 114
     Fuse = 122
     Heco = 128
     Polygon = 137
+    Xlayer = 196
     Fantom = 250
+    Fraxtal = 252
     Boba = 288
     KCC = 321
     OptimismGorli = 420
     Astar = 592
     Metis = 1088
     Moonbeam = 1284
     Moonriver = 1285
@@ -238,15 +240,17 @@
     Network.Gnosis: "0xcA11bde05977b3631167028862bE2a173976CA11",
     Network.Velas: "0xcA11bde05977b3631167028862bE2a173976CA11",
     Network.Thundercore: "0xcA11bde05977b3631167028862bE2a173976CA11",
     Network.Coston2Testnet: "0xcA11bde05977b3631167028862bE2a173976CA11",
     Network.Fuse: "0xcA11bde05977b3631167028862bE2a173976CA11",
     Network.Heco: "0xcA11bde05977b3631167028862bE2a173976CA11",
     Network.Polygon: "0xcA11bde05977b3631167028862bE2a173976CA11",
+    Network.Xlayer: "0xcA11bde05977b3631167028862bE2a173976CA11",
     Network.Fantom: "0xcA11bde05977b3631167028862bE2a173976CA11",
+    Network.Fraxtal: "0xcA11bde05977b3631167028862bE2a173976CA11",
     Network.Boba: "0xcA11bde05977b3631167028862bE2a173976CA11",
     Network.KCC: "0xcA11bde05977b3631167028862bE2a173976CA11",
     Network.OptimismGorli: "0xcA11bde05977b3631167028862bE2a173976CA11",
     Network.Astar: "0xcA11bde05977b3631167028862bE2a173976CA11",
     Network.Metis: "0xcA11bde05977b3631167028862bE2a173976CA11",
     Network.Moonbeam: "0xcA11bde05977b3631167028862bE2a173976CA11",
     Network.Moonriver: "0xcA11bde05977b3631167028862bE2a173976CA11",
```

### Comparing `web3mc-0.1.6/web3mc/multicall.py` & `web3mc-0.1.7/web3mc/multicall.py`

 * *Files identical despite different names*

### Comparing `web3mc-0.1.6/PKG-INFO` & `web3mc-0.1.7/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: web3mc
-Version: 0.1.6
+Version: 0.1.7
 Summary: Multicall library for aggregating web3py contract calls
 Home-page: https://github.com/amfet42/web3mc
 License: MIT
 Keywords: web3,multicall
 Author: amfet42
 Requires-Python: >=3.10,<4.0
 Classifier: License :: OSI Approved :: MIT License
```

