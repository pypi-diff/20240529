# Comparing `tmp/nftpy-1.1.1.tar.gz` & `tmp/nftpy-1.1.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "nftpy-1.1.1.tar", max compression
+gzip compressed data, was "nftpy-1.1.2.tar", max compression
```

## Comparing `nftpy-1.1.1.tar` & `nftpy-1.1.2.tar`

### file list

```diff
@@ -1,12 +1,12 @@
--rw-r--r--   0        0        0     1091 2024-05-27 01:41:06.348086 nftpy-1.1.1/LICENSE
--rw-r--r--   0        0        0      269 2024-05-28 08:15:32.289802 nftpy-1.1.1/nftpy/__init__.py
--rw-r--r--   0        0        0     2669 2024-05-28 05:51:30.861326 nftpy-1.1.1/nftpy/errors.py
--rw-r--r--   0        0        0      152 2024-05-27 20:44:18.057168 nftpy-1.1.1/nftpy/EVM/__init__.py
--rw-r--r--   0        0        0    14009 2024-05-28 06:40:00.392465 nftpy-1.1.1/nftpy/EVM/abi.py
--rw-r--r--   0        0        0     3142 2024-05-28 06:06:15.680338 nftpy-1.1.1/nftpy/EVM/chains.py
--rw-r--r--   0        0        0     6286 2024-05-28 05:48:12.511059 nftpy-1.1.1/nftpy/EVM/nft.py
--rw-r--r--   0        0        0     7534 2024-05-28 08:10:02.369569 nftpy-1.1.1/nftpy/EVM/wallet.py
--rw-r--r--   0        0        0     8626 2024-05-28 05:47:40.676820 nftpy-1.1.1/nftpy/opensea.py
--rw-r--r--   0        0        0      570 2024-05-28 08:12:47.554479 nftpy-1.1.1/pyproject.toml
--rw-r--r--   0        0        0    12704 2024-05-28 08:20:29.669317 nftpy-1.1.1/README.md
--rw-r--r--   0        0        0    13069 1970-01-01 00:00:00.000000 nftpy-1.1.1/PKG-INFO
+-rw-r--r--   0        0        0     1091 2024-05-28 18:17:49.643296 nftpy-1.1.2/LICENSE
+-rw-r--r--   0        0        0      269 2024-05-28 18:17:49.646297 nftpy-1.1.2/nftpy/__init__.py
+-rw-r--r--   0        0        0     2669 2024-05-28 18:17:49.646297 nftpy-1.1.2/nftpy/errors.py
+-rw-r--r--   0        0        0      152 2024-05-28 18:17:49.644297 nftpy-1.1.2/nftpy/EVM/__init__.py
+-rw-r--r--   0        0        0    14009 2024-05-28 18:17:49.644297 nftpy-1.1.2/nftpy/EVM/abi.py
+-rw-r--r--   0        0        0     3142 2024-05-28 18:17:49.644297 nftpy-1.1.2/nftpy/EVM/chains.py
+-rw-r--r--   0        0        0     6286 2024-05-28 18:17:49.645297 nftpy-1.1.2/nftpy/EVM/nft.py
+-rw-r--r--   0        0        0    14109 2024-05-28 18:17:49.645297 nftpy-1.1.2/nftpy/EVM/wallet.py
+-rw-r--r--   0        0        0    15051 2024-05-28 18:17:49.647298 nftpy-1.1.2/nftpy/opensea.py
+-rw-r--r--   0        0        0      570 2024-05-28 18:17:49.647298 nftpy-1.1.2/pyproject.toml
+-rw-r--r--   0        0        0    12971 2024-05-28 18:18:11.585707 nftpy-1.1.2/README.md
+-rw-r--r--   0        0        0    13332 1970-01-01 00:00:00.000000 nftpy-1.1.2/PKG-INFO
```

### Comparing `nftpy-1.1.1/LICENSE` & `nftpy-1.1.2/LICENSE`

 * *Files identical despite different names*

### Comparing `nftpy-1.1.1/nftpy/errors.py` & `nftpy-1.1.2/nftpy/errors.py`

 * *Files identical despite different names*

### Comparing `nftpy-1.1.1/nftpy/EVM/abi.py` & `nftpy-1.1.2/nftpy/EVM/abi.py`

 * *Files identical despite different names*

### Comparing `nftpy-1.1.1/nftpy/EVM/chains.py` & `nftpy-1.1.2/nftpy/EVM/chains.py`

 * *Files identical despite different names*

### Comparing `nftpy-1.1.1/nftpy/EVM/nft.py` & `nftpy-1.1.2/nftpy/EVM/nft.py`

 * *Files identical despite different names*

### Comparing `nftpy-1.1.1/pyproject.toml` & `nftpy-1.1.2/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "nftpy"
-version = "1.1.1"
+version = "1.1.2"
 description = "A NFT specific Python library for easy NFT integration in Python"
 authors = ["CoulterStutz <coultercash@gmail.com>"]
 readme = "README.md"
 license = "MIT"
 homepage = "https://github.com/coulterstutz/nftpy"
 repository = "https://github.com/coulterstutz/nftpy"
```

### Comparing `nftpy-1.1.1/README.md` & `nftpy-1.1.2/README.md`

 * *Files 2% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 # NFTPy
-[![PyPi](https://img.shields.io/badge/PyPi-1.1.1-green?labelColor=026ab5&style=flat-square&logo=pypi&logoColor=ffffff&link=https://pypi.org/project/NFTPy/)](https://pypi.org/project/NFTPy/)
+[![PyPi](https://img.shields.io/badge/PyPi-1.1.2-green?labelColor=026ab5&style=flat-square&logo=pypi&logoColor=ffffff&link=https://pypi.org/project/NFTPy/)](https://pypi.org/project/NFTPy/)
 [![Python](https://img.shields.io/badge/Python-3.7,%203.8,%203.9,%203.10,%203.11,%203.12-green?labelColor=026ab5&style=flat-square&logo=pypi&logoColor=ffffff&link=https://pypi.org/project/NFTPy/)](https://pypi.org/project/NFTPy/)
 
 A Python package designed to facilitate the integration and adoption of NFT (ERC721, ERC1155) tokens in software applications.
 
 ## Features
 
 #### EVM Interaction with NFT Tokens
@@ -27,14 +27,18 @@
 **Wallet Features:**
 - **get_balance**: Retrieve the balance of NFTs for a given address in Ether.
 - **get_balance_wei**: Retrieve the balance of NFTs for a given address in Wei.
 - **get_gas_price_wei**: Fetch the current gas price in Wei.
 - **get_gas_price_gwei**: Fetch the current gas price in Gwei.
 - **transfer_nft**: Transfer an NFT from the wallet to another address.
 - **wait_until_transaction_processes**: Delays the program until the transaction has fully processed in the blockchain
+- **get_transaction_count**: Get the number of transactions sent from the wallet.
+- **estimate_gas**: Estimate the gas required for a transaction.
+- **is_synced**: Check if the blockchain is synced.
+- **get_latest_block**: Get the latest block on the blockchain.
 
 #### Built-in OpenSea Interface
 ![OpenSea Support](https://img.shields.io/badge/OpenSea-%232081E2.svg?style=for-the-badge&logo=opensea&logoColor=white)
 
 NFTPy includes a built-in interface for interacting with OpenSea via an API key. This allows for in-package queries to OpenSea, enabling access to pricing information and other OpenSea-specific data. The OpenSea interface can be configured to focus on a single collection or query multiple collections. The available methods include:
 
 - **get_collection_stats**: Obtain statistics for a collection.
```

### Comparing `nftpy-1.1.1/PKG-INFO` & `nftpy-1.1.2/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: nftpy
-Version: 1.1.1
+Version: 1.1.2
 Summary: A NFT specific Python library for easy NFT integration in Python
 Home-page: https://github.com/coulterstutz/nftpy
 License: MIT
 Author: CoulterStutz
 Author-email: coultercash@gmail.com
 Requires-Python: >=3.12,<4.0
 Classifier: License :: OSI Approved :: MIT License
@@ -12,15 +12,15 @@
 Classifier: Programming Language :: Python :: 3.12
 Requires-Dist: requests (>=2.28.1,<3.0.0)
 Requires-Dist: web3 (>=6.2.0,<7.0.0)
 Project-URL: Repository, https://github.com/coulterstutz/nftpy
 Description-Content-Type: text/markdown
 
 # NFTPy
-[![PyPi](https://img.shields.io/badge/PyPi-1.1.1-green?labelColor=026ab5&style=flat-square&logo=pypi&logoColor=ffffff&link=https://pypi.org/project/NFTPy/)](https://pypi.org/project/NFTPy/)
+[![PyPi](https://img.shields.io/badge/PyPi-1.1.2-green?labelColor=026ab5&style=flat-square&logo=pypi&logoColor=ffffff&link=https://pypi.org/project/NFTPy/)](https://pypi.org/project/NFTPy/)
 [![Python](https://img.shields.io/badge/Python-3.7,%203.8,%203.9,%203.10,%203.11,%203.12-green?labelColor=026ab5&style=flat-square&logo=pypi&logoColor=ffffff&link=https://pypi.org/project/NFTPy/)](https://pypi.org/project/NFTPy/)
 
 A Python package designed to facilitate the integration and adoption of NFT (ERC721, ERC1155) tokens in software applications.
 
 ## Features
 
 #### EVM Interaction with NFT Tokens
@@ -44,14 +44,18 @@
 **Wallet Features:**
 - **get_balance**: Retrieve the balance of NFTs for a given address in Ether.
 - **get_balance_wei**: Retrieve the balance of NFTs for a given address in Wei.
 - **get_gas_price_wei**: Fetch the current gas price in Wei.
 - **get_gas_price_gwei**: Fetch the current gas price in Gwei.
 - **transfer_nft**: Transfer an NFT from the wallet to another address.
 - **wait_until_transaction_processes**: Delays the program until the transaction has fully processed in the blockchain
+- **get_transaction_count**: Get the number of transactions sent from the wallet.
+- **estimate_gas**: Estimate the gas required for a transaction.
+- **is_synced**: Check if the blockchain is synced.
+- **get_latest_block**: Get the latest block on the blockchain.
 
 #### Built-in OpenSea Interface
 ![OpenSea Support](https://img.shields.io/badge/OpenSea-%232081E2.svg?style=for-the-badge&logo=opensea&logoColor=white)
 
 NFTPy includes a built-in interface for interacting with OpenSea via an API key. This allows for in-package queries to OpenSea, enabling access to pricing information and other OpenSea-specific data. The OpenSea interface can be configured to focus on a single collection or query multiple collections. The available methods include:
 
 - **get_collection_stats**: Obtain statistics for a collection.
```

