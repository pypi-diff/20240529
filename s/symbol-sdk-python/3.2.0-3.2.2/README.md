# Comparing `tmp/symbol_sdk_python-3.2.0.tar.gz` & `tmp/symbol_sdk_python-3.2.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "symbol_sdk_python-3.2.0.tar", max compression
+gzip compressed data, was "symbol_sdk_python-3.2.2.tar", max compression
```

## Comparing `symbol_sdk_python-3.2.0.tar` & `symbol_sdk_python-3.2.2.tar`

### file list

```diff
@@ -1,54 +1,54 @@
--rw-r--r--   0        0        0     4585 2024-04-10 01:40:59.424770 symbol_sdk_python-3.2.0/README.md
--rw-r--r--   0        0        0      842 2024-04-10 01:44:54.079071 symbol_sdk_python-3.2.0/pyproject.toml
--rw-r--r--   0        0        0     2508 2024-04-10 01:40:59.428770 symbol_sdk_python-3.2.0/symbolchain/AccountDescriptorRepository.py
--rw-r--r--   0        0        0     3728 2024-04-10 01:40:59.428770 symbol_sdk_python-3.2.0/symbolchain/ArrayHelpers.py
--rw-r--r--   0        0        0     1482 2024-04-10 01:40:59.428770 symbol_sdk_python-3.2.0/symbolchain/BaseValue.py
--rw-r--r--   0        0        0     1787 2024-04-10 01:40:59.428770 symbol_sdk_python-3.2.0/symbolchain/Bip32.py
--rw-r--r--   0        0        0      723 2024-04-10 01:40:59.428770 symbol_sdk_python-3.2.0/symbolchain/BlockchainSettings.py
--rw-r--r--   0        0        0      883 2024-04-10 01:40:59.428770 symbol_sdk_python-3.2.0/symbolchain/BufferReader.py
--rw-r--r--   0        0        0      639 2024-04-10 01:40:59.428770 symbol_sdk_python-3.2.0/symbolchain/BufferWriter.py
--rw-r--r--   0        0        0     1059 2024-04-10 01:40:59.428770 symbol_sdk_python-3.2.0/symbolchain/ByteArray.py
--rw-r--r--   0        0        0     2158 2024-04-10 01:40:59.428770 symbol_sdk_python-3.2.0/symbolchain/Cipher.py
--rw-r--r--   0        0        0     1233 2024-04-10 01:40:59.428770 symbol_sdk_python-3.2.0/symbolchain/CodeWordsEncoder.py
--rw-r--r--   0        0        0     1844 2024-04-10 01:40:59.428770 symbol_sdk_python-3.2.0/symbolchain/CryptoTypes.py
--rw-r--r--   0        0        0     1848 2024-04-10 01:40:59.428770 symbol_sdk_python-3.2.0/symbolchain/DiceMnemonicGenerator.py
--rw-r--r--   0        0        0     3368 2024-04-10 01:40:59.428770 symbol_sdk_python-3.2.0/symbolchain/Network.py
--rw-r--r--   0        0        0     1595 2024-04-10 01:40:59.428770 symbol_sdk_python-3.2.0/symbolchain/NetworkTimestamp.py
--rw-r--r--   0        0        0     1019 2024-04-10 01:40:59.428770 symbol_sdk_python-3.2.0/symbolchain/NodeDescriptorRepository.py
--rw-r--r--   0        0        0      397 2024-04-10 01:40:59.428770 symbol_sdk_python-3.2.0/symbolchain/Ordered.py
--rw-r--r--   0        0        0     1606 2024-04-10 01:40:59.428770 symbol_sdk_python-3.2.0/symbolchain/PrivateKeyStorage.py
--rw-r--r--   0        0        0     1348 2024-04-10 01:40:59.432770 symbol_sdk_python-3.2.0/symbolchain/QrSignatureStorage.py
--rw-r--r--   0        0        0     1494 2024-04-10 01:40:59.432770 symbol_sdk_python-3.2.0/symbolchain/QrStorage.py
--rw-r--r--   0        0        0     5101 2024-04-10 01:40:59.432770 symbol_sdk_python-3.2.0/symbolchain/RuleBasedTransactionFactory.py
--rw-r--r--   0        0        0      593 2024-04-10 01:40:59.432770 symbol_sdk_python-3.2.0/symbolchain/SharedKey.py
--rw-r--r--   0        0        0     1806 2024-04-10 01:40:59.432770 symbol_sdk_python-3.2.0/symbolchain/TransactionDescriptorProcessor.py
--rw-r--r--   0        0        0      226 2024-04-10 01:40:59.432770 symbol_sdk_python-3.2.0/symbolchain/Transforms.py
--rw-r--r--   0        0        0        0 2024-04-10 01:40:59.432770 symbol_sdk_python-3.2.0/symbolchain/__init__.py
--rw-r--r--   0        0        0        0 2024-04-10 01:40:59.432770 symbol_sdk_python-3.2.0/symbolchain/external/__init__.py
--rw-r--r--   0        0        0     7833 2024-04-10 01:40:59.432770 symbol_sdk_python-3.2.0/symbolchain/external/ed25519.py
--rw-r--r--   0        0        0     2983 2024-04-10 01:40:59.432770 symbol_sdk_python-3.2.0/symbolchain/facade/BatchOperations.py
--rw-r--r--   0        0        0     2990 2024-04-10 01:40:59.432770 symbol_sdk_python-3.2.0/symbolchain/facade/NemFacade.py
--rw-r--r--   0        0        0     5128 2024-04-10 01:40:59.432770 symbol_sdk_python-3.2.0/symbolchain/facade/SymbolFacade.py
--rw-r--r--   0        0        0        0 2024-04-10 01:40:59.432770 symbol_sdk_python-3.2.0/symbolchain/facade/__init__.py
--rw-r--r--   0        0        0     2152 2024-04-10 01:40:59.432770 symbol_sdk_python-3.2.0/symbolchain/impl/CipherHelpers.py
--rw-r--r--   0        0        0        0 2024-04-10 01:40:59.432770 symbol_sdk_python-3.2.0/symbolchain/impl/__init__.py
--rw-r--r--   0        0        0   106403 2024-04-10 01:40:59.432770 symbol_sdk_python-3.2.0/symbolchain/nc/__init__.py
--rw-r--r--   0        0        0     3712 2024-04-10 01:40:59.432770 symbol_sdk_python-3.2.0/symbolchain/nem/KeyPair.py
--rw-r--r--   0        0        0     2583 2024-04-10 01:40:59.432770 symbol_sdk_python-3.2.0/symbolchain/nem/MessageEncoder.py
--rw-r--r--   0        0        0     1746 2024-04-10 01:40:59.432770 symbol_sdk_python-3.2.0/symbolchain/nem/Network.py
--rw-r--r--   0        0        0     1094 2024-04-10 01:40:59.432770 symbol_sdk_python-3.2.0/symbolchain/nem/SharedKey.py
--rw-r--r--   0        0        0     4017 2024-04-10 01:40:59.432770 symbol_sdk_python-3.2.0/symbolchain/nem/TransactionFactory.py
--rw-r--r--   0        0        0        0 2024-04-10 01:40:59.432770 symbol_sdk_python-3.2.0/symbolchain/nem/__init__.py
--rw-r--r--   0        0        0      378 2024-04-10 01:40:59.432770 symbol_sdk_python-3.2.0/symbolchain/ripemd160.py
--rw-r--r--   0        0        0   286967 2024-04-10 01:40:59.436770 symbol_sdk_python-3.2.0/symbolchain/sc/__init__.py
--rw-r--r--   0        0        0     1696 2024-04-10 01:40:59.436770 symbol_sdk_python-3.2.0/symbolchain/symbol/IdGenerator.py
--rw-r--r--   0        0        0     1506 2024-04-10 01:40:59.436770 symbol_sdk_python-3.2.0/symbolchain/symbol/KeyPair.py
--rw-r--r--   0        0        0     7243 2024-04-10 01:40:59.436770 symbol_sdk_python-3.2.0/symbolchain/symbol/Merkle.py
--rw-r--r--   0        0        0     3766 2024-04-10 01:40:59.436770 symbol_sdk_python-3.2.0/symbolchain/symbol/MessageEncoder.py
--rw-r--r--   0        0        0      567 2024-04-10 01:40:59.436770 symbol_sdk_python-3.2.0/symbolchain/symbol/Metadata.py
--rw-r--r--   0        0        0     2229 2024-04-10 01:40:59.436770 symbol_sdk_python-3.2.0/symbolchain/symbol/Network.py
--rw-r--r--   0        0        0      334 2024-04-10 01:40:59.436770 symbol_sdk_python-3.2.0/symbolchain/symbol/SharedKey.py
--rw-r--r--   0        0        0     3624 2024-04-10 01:40:59.436770 symbol_sdk_python-3.2.0/symbolchain/symbol/TransactionFactory.py
--rw-r--r--   0        0        0     1686 2024-04-10 01:40:59.436770 symbol_sdk_python-3.2.0/symbolchain/symbol/VotingKeysGenerator.py
--rw-r--r--   0        0        0        0 2024-04-10 01:40:59.436770 symbol_sdk_python-3.2.0/symbolchain/symbol/__init__.py
--rw-r--r--   0        0        0     5584 1970-01-01 00:00:00.000000 symbol_sdk_python-3.2.0/PKG-INFO
+-rw-r--r--   0        0        0     4585 2024-05-28 22:26:27.973061 symbol_sdk_python-3.2.2/README.md
+-rw-r--r--   0        0        0      842 2024-05-28 22:32:32.272505 symbol_sdk_python-3.2.2/pyproject.toml
+-rw-r--r--   0        0        0     2508 2024-05-28 22:26:27.973061 symbol_sdk_python-3.2.2/symbolchain/AccountDescriptorRepository.py
+-rw-r--r--   0        0        0     3728 2024-05-28 22:26:27.973061 symbol_sdk_python-3.2.2/symbolchain/ArrayHelpers.py
+-rw-r--r--   0        0        0     1482 2024-05-28 22:26:27.973061 symbol_sdk_python-3.2.2/symbolchain/BaseValue.py
+-rw-r--r--   0        0        0     1787 2024-05-28 22:26:27.973061 symbol_sdk_python-3.2.2/symbolchain/Bip32.py
+-rw-r--r--   0        0        0      723 2024-05-28 22:26:27.973061 symbol_sdk_python-3.2.2/symbolchain/BlockchainSettings.py
+-rw-r--r--   0        0        0      883 2024-05-28 22:26:27.973061 symbol_sdk_python-3.2.2/symbolchain/BufferReader.py
+-rw-r--r--   0        0        0      639 2024-05-28 22:26:27.973061 symbol_sdk_python-3.2.2/symbolchain/BufferWriter.py
+-rw-r--r--   0        0        0     1059 2024-05-28 22:26:27.973061 symbol_sdk_python-3.2.2/symbolchain/ByteArray.py
+-rw-r--r--   0        0        0     2158 2024-05-28 22:26:27.973061 symbol_sdk_python-3.2.2/symbolchain/Cipher.py
+-rw-r--r--   0        0        0     1233 2024-05-28 22:26:27.973061 symbol_sdk_python-3.2.2/symbolchain/CodeWordsEncoder.py
+-rw-r--r--   0        0        0     1844 2024-05-28 22:26:27.973061 symbol_sdk_python-3.2.2/symbolchain/CryptoTypes.py
+-rw-r--r--   0        0        0     1848 2024-05-28 22:26:27.973061 symbol_sdk_python-3.2.2/symbolchain/DiceMnemonicGenerator.py
+-rw-r--r--   0        0        0     3368 2024-05-28 22:26:27.973061 symbol_sdk_python-3.2.2/symbolchain/Network.py
+-rw-r--r--   0        0        0     1595 2024-05-28 22:26:27.973061 symbol_sdk_python-3.2.2/symbolchain/NetworkTimestamp.py
+-rw-r--r--   0        0        0     1019 2024-05-28 22:26:27.973061 symbol_sdk_python-3.2.2/symbolchain/NodeDescriptorRepository.py
+-rw-r--r--   0        0        0      397 2024-05-28 22:26:27.973061 symbol_sdk_python-3.2.2/symbolchain/Ordered.py
+-rw-r--r--   0        0        0     1606 2024-05-28 22:26:27.973061 symbol_sdk_python-3.2.2/symbolchain/PrivateKeyStorage.py
+-rw-r--r--   0        0        0     1348 2024-05-28 22:26:27.973061 symbol_sdk_python-3.2.2/symbolchain/QrSignatureStorage.py
+-rw-r--r--   0        0        0     1494 2024-05-28 22:26:27.973061 symbol_sdk_python-3.2.2/symbolchain/QrStorage.py
+-rw-r--r--   0        0        0     5101 2024-05-28 22:26:27.973061 symbol_sdk_python-3.2.2/symbolchain/RuleBasedTransactionFactory.py
+-rw-r--r--   0        0        0      593 2024-05-28 22:26:27.973061 symbol_sdk_python-3.2.2/symbolchain/SharedKey.py
+-rw-r--r--   0        0        0     1806 2024-05-28 22:26:27.973061 symbol_sdk_python-3.2.2/symbolchain/TransactionDescriptorProcessor.py
+-rw-r--r--   0        0        0      226 2024-05-28 22:26:27.973061 symbol_sdk_python-3.2.2/symbolchain/Transforms.py
+-rw-r--r--   0        0        0        0 2024-05-28 22:26:27.973061 symbol_sdk_python-3.2.2/symbolchain/__init__.py
+-rw-r--r--   0        0        0        0 2024-05-28 22:26:27.973061 symbol_sdk_python-3.2.2/symbolchain/external/__init__.py
+-rw-r--r--   0        0        0     7833 2024-05-28 22:26:27.973061 symbol_sdk_python-3.2.2/symbolchain/external/ed25519.py
+-rw-r--r--   0        0        0     2983 2024-05-28 22:26:27.977061 symbol_sdk_python-3.2.2/symbolchain/facade/BatchOperations.py
+-rw-r--r--   0        0        0     4166 2024-05-28 22:26:27.977061 symbol_sdk_python-3.2.2/symbolchain/facade/NemFacade.py
+-rw-r--r--   0        0        0     6527 2024-05-28 22:26:27.977061 symbol_sdk_python-3.2.2/symbolchain/facade/SymbolFacade.py
+-rw-r--r--   0        0        0        0 2024-05-28 22:26:27.977061 symbol_sdk_python-3.2.2/symbolchain/facade/__init__.py
+-rw-r--r--   0        0        0     2152 2024-05-28 22:26:27.977061 symbol_sdk_python-3.2.2/symbolchain/impl/CipherHelpers.py
+-rw-r--r--   0        0        0        0 2024-05-28 22:26:27.977061 symbol_sdk_python-3.2.2/symbolchain/impl/__init__.py
+-rw-r--r--   0        0        0   106403 2024-05-28 22:26:27.977061 symbol_sdk_python-3.2.2/symbolchain/nc/__init__.py
+-rw-r--r--   0        0        0     3712 2024-05-28 22:26:27.977061 symbol_sdk_python-3.2.2/symbolchain/nem/KeyPair.py
+-rw-r--r--   0        0        0     2699 2024-05-28 22:26:27.977061 symbol_sdk_python-3.2.2/symbolchain/nem/MessageEncoder.py
+-rw-r--r--   0        0        0     1746 2024-05-28 22:26:27.977061 symbol_sdk_python-3.2.2/symbolchain/nem/Network.py
+-rw-r--r--   0        0        0     1094 2024-05-28 22:26:27.977061 symbol_sdk_python-3.2.2/symbolchain/nem/SharedKey.py
+-rw-r--r--   0        0        0     4170 2024-05-28 22:26:27.977061 symbol_sdk_python-3.2.2/symbolchain/nem/TransactionFactory.py
+-rw-r--r--   0        0        0        0 2024-05-28 22:26:27.977061 symbol_sdk_python-3.2.2/symbolchain/nem/__init__.py
+-rw-r--r--   0        0        0      429 2024-05-28 22:26:27.977061 symbol_sdk_python-3.2.2/symbolchain/ripemd160.py
+-rw-r--r--   0        0        0   286967 2024-05-28 22:26:27.977061 symbol_sdk_python-3.2.2/symbolchain/sc/__init__.py
+-rw-r--r--   0        0        0     1696 2024-05-28 22:26:27.977061 symbol_sdk_python-3.2.2/symbolchain/symbol/IdGenerator.py
+-rw-r--r--   0        0        0     1506 2024-05-28 22:26:27.977061 symbol_sdk_python-3.2.2/symbolchain/symbol/KeyPair.py
+-rw-r--r--   0        0        0     7243 2024-05-28 22:26:27.977061 symbol_sdk_python-3.2.2/symbolchain/symbol/Merkle.py
+-rw-r--r--   0        0        0     3882 2024-05-28 22:26:27.977061 symbol_sdk_python-3.2.2/symbolchain/symbol/MessageEncoder.py
+-rw-r--r--   0        0        0      884 2024-05-28 22:26:27.977061 symbol_sdk_python-3.2.2/symbolchain/symbol/Metadata.py
+-rw-r--r--   0        0        0     2933 2024-05-28 22:26:27.977061 symbol_sdk_python-3.2.2/symbolchain/symbol/Network.py
+-rw-r--r--   0        0        0      334 2024-05-28 22:26:27.977061 symbol_sdk_python-3.2.2/symbolchain/symbol/SharedKey.py
+-rw-r--r--   0        0        0     3957 2024-05-28 22:26:27.977061 symbol_sdk_python-3.2.2/symbolchain/symbol/TransactionFactory.py
+-rw-r--r--   0        0        0     1686 2024-05-28 22:26:27.977061 symbol_sdk_python-3.2.2/symbolchain/symbol/VotingKeysGenerator.py
+-rw-r--r--   0        0        0        0 2024-05-28 22:26:27.977061 symbol_sdk_python-3.2.2/symbolchain/symbol/__init__.py
+-rw-r--r--   0        0        0     5584 1970-01-01 00:00:00.000000 symbol_sdk_python-3.2.2/PKG-INFO
```

### Comparing `symbol_sdk_python-3.2.0/README.md` & `symbol_sdk_python-3.2.2/README.md`

 * *Files identical despite different names*

### Comparing `symbol_sdk_python-3.2.0/pyproject.toml` & `symbol_sdk_python-3.2.2/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = 'symbol-sdk-python'
-version = '3.2.0'
+version = '3.2.2'
 description = 'Symbol SDK'
 authors = ['Symbol Contributors <contributors@symbol.dev>']
 maintainers = ['Symbol Contributors <contributors@symbol.dev>']
 license = 'MIT'
 
 readme = 'README.md'
```

### Comparing `symbol_sdk_python-3.2.0/symbolchain/AccountDescriptorRepository.py` & `symbol_sdk_python-3.2.2/symbolchain/AccountDescriptorRepository.py`

 * *Files identical despite different names*

### Comparing `symbol_sdk_python-3.2.0/symbolchain/ArrayHelpers.py` & `symbol_sdk_python-3.2.2/symbolchain/ArrayHelpers.py`

 * *Files identical despite different names*

### Comparing `symbol_sdk_python-3.2.0/symbolchain/BaseValue.py` & `symbol_sdk_python-3.2.2/symbolchain/BaseValue.py`

 * *Files identical despite different names*

### Comparing `symbol_sdk_python-3.2.0/symbolchain/Bip32.py` & `symbol_sdk_python-3.2.2/symbolchain/Bip32.py`

 * *Files identical despite different names*

### Comparing `symbol_sdk_python-3.2.0/symbolchain/BlockchainSettings.py` & `symbol_sdk_python-3.2.2/symbolchain/BlockchainSettings.py`

 * *Files identical despite different names*

### Comparing `symbol_sdk_python-3.2.0/symbolchain/BufferReader.py` & `symbol_sdk_python-3.2.2/symbolchain/BufferReader.py`

 * *Files identical despite different names*

### Comparing `symbol_sdk_python-3.2.0/symbolchain/BufferWriter.py` & `symbol_sdk_python-3.2.2/symbolchain/BufferWriter.py`

 * *Files identical despite different names*

### Comparing `symbol_sdk_python-3.2.0/symbolchain/ByteArray.py` & `symbol_sdk_python-3.2.2/symbolchain/ByteArray.py`

 * *Files identical despite different names*

### Comparing `symbol_sdk_python-3.2.0/symbolchain/Cipher.py` & `symbol_sdk_python-3.2.2/symbolchain/Cipher.py`

 * *Files identical despite different names*

### Comparing `symbol_sdk_python-3.2.0/symbolchain/CodeWordsEncoder.py` & `symbol_sdk_python-3.2.2/symbolchain/CodeWordsEncoder.py`

 * *Files identical despite different names*

### Comparing `symbol_sdk_python-3.2.0/symbolchain/CryptoTypes.py` & `symbol_sdk_python-3.2.2/symbolchain/CryptoTypes.py`

 * *Files identical despite different names*

### Comparing `symbol_sdk_python-3.2.0/symbolchain/DiceMnemonicGenerator.py` & `symbol_sdk_python-3.2.2/symbolchain/DiceMnemonicGenerator.py`

 * *Files identical despite different names*

### Comparing `symbol_sdk_python-3.2.0/symbolchain/Network.py` & `symbol_sdk_python-3.2.2/symbolchain/Network.py`

 * *Files identical despite different names*

### Comparing `symbol_sdk_python-3.2.0/symbolchain/NetworkTimestamp.py` & `symbol_sdk_python-3.2.2/symbolchain/NetworkTimestamp.py`

 * *Files identical despite different names*

### Comparing `symbol_sdk_python-3.2.0/symbolchain/NodeDescriptorRepository.py` & `symbol_sdk_python-3.2.2/symbolchain/NodeDescriptorRepository.py`

 * *Files identical despite different names*

### Comparing `symbol_sdk_python-3.2.0/symbolchain/PrivateKeyStorage.py` & `symbol_sdk_python-3.2.2/symbolchain/PrivateKeyStorage.py`

 * *Files identical despite different names*

### Comparing `symbol_sdk_python-3.2.0/symbolchain/QrSignatureStorage.py` & `symbol_sdk_python-3.2.2/symbolchain/QrSignatureStorage.py`

 * *Files identical despite different names*

### Comparing `symbol_sdk_python-3.2.0/symbolchain/QrStorage.py` & `symbol_sdk_python-3.2.2/symbolchain/QrStorage.py`

 * *Files identical despite different names*

### Comparing `symbol_sdk_python-3.2.0/symbolchain/RuleBasedTransactionFactory.py` & `symbol_sdk_python-3.2.2/symbolchain/RuleBasedTransactionFactory.py`

 * *Files identical despite different names*

### Comparing `symbol_sdk_python-3.2.0/symbolchain/SharedKey.py` & `symbol_sdk_python-3.2.2/symbolchain/SharedKey.py`

 * *Files identical despite different names*

### Comparing `symbol_sdk_python-3.2.0/symbolchain/TransactionDescriptorProcessor.py` & `symbol_sdk_python-3.2.2/symbolchain/TransactionDescriptorProcessor.py`

 * *Files identical despite different names*

### Comparing `symbol_sdk_python-3.2.0/symbolchain/external/ed25519.py` & `symbol_sdk_python-3.2.2/symbolchain/external/ed25519.py`

 * *Files identical despite different names*

### Comparing `symbol_sdk_python-3.2.0/symbolchain/facade/BatchOperations.py` & `symbol_sdk_python-3.2.2/symbolchain/facade/BatchOperations.py`

 * *Files identical despite different names*

### Comparing `symbol_sdk_python-3.2.0/symbolchain/facade/NemFacade.py` & `symbol_sdk_python-3.2.2/symbolchain/facade/NemFacade.py`

 * *Files 27% similar despite different names*

```diff
@@ -1,18 +1,50 @@
 from datetime import datetime, timezone
 
 import sha3
 
 from ..CryptoTypes import Hash256, PrivateKey, PublicKey
 from ..nem.KeyPair import KeyPair, Verifier
+from ..nem.MessageEncoder import MessageEncoder
 from ..nem.Network import Address, Network
 from ..nem.SharedKey import SharedKey
 from ..nem.TransactionFactory import TransactionFactory
 from ..Network import NetworkLocator
 
+# region NemPublicAccount / NemAccount
+
+
+class NemPublicAccount:
+	"""NEM public account."""
+
+	def __init__(self, facade, public_key):
+		"""Creates a NEM public account."""
+		self._facade = facade
+		self.public_key = public_key
+		self.address = self._facade.network.public_key_to_address(self.public_key)
+
+
+class NemAccount(NemPublicAccount):
+	"""NEM account."""
+
+	def __init__(self, facade, key_pair):
+		"""Creates a NEM account."""
+		super().__init__(facade, key_pair.public_key)
+		self.key_pair = key_pair
+
+	def message_encoder(self):
+		"""Creates a message encoder that can be used for encrypting and encoding messages between two parties."""
+		return MessageEncoder(self.key_pair)
+
+	def sign_transaction(self, transaction):
+		"""Signs a NEM transaction."""
+		return self._facade.sign_transaction(self.key_pair, transaction)
+
+# endregion
+
 
 class NemFacade:
 	"""Facade used to interact with NEM blockchain."""
 
 	BIP32_CURVE_NAME = 'ed25519-keccak'
 
 	Address = Address  # pylint: disable=duplicate-code
@@ -42,14 +74,22 @@
 			PublicKey: 'public_key'
 		}
 
 	def now(self):
 		"""Creates a network timestamp representing the current time."""
 		return self.network.from_datetime(datetime.now(timezone.utc))
 
+	def create_public_account(self, public_key):
+		"""Creates a NEM public account from a public key."""
+		return NemPublicAccount(self, public_key)
+
+	def create_account(self, private_key):
+		"""Creates a NEM account from a private key."""
+		return NemAccount(self, KeyPair(private_key))
+
 	@staticmethod
 	def hash_transaction(transaction):
 		"""Hashes a NEM transaction."""
 		non_verifiable_transaction = TransactionFactory.to_non_verifiable_transaction(transaction)
 		return Hash256(sha3.keccak_256(non_verifiable_transaction.serialize()).digest())
 
 	@staticmethod
```

### Comparing `symbol_sdk_python-3.2.0/symbolchain/facade/SymbolFacade.py` & `symbol_sdk_python-3.2.2/symbolchain/facade/SymbolFacade.py`

 * *Files 14% similar despite different names*

```diff
@@ -2,14 +2,15 @@
 from datetime import datetime, timezone
 
 from .. import sc
 from ..CryptoTypes import Hash256, PublicKey, Signature
 from ..Network import NetworkLocator
 from ..symbol.KeyPair import KeyPair, Verifier
 from ..symbol.Merkle import MerkleHashBuilder
+from ..symbol.MessageEncoder import MessageEncoder
 from ..symbol.Network import Address, Network
 from ..symbol.SharedKey import SharedKey
 from ..symbol.TransactionFactory import TransactionFactory
 
 TRANSACTION_HEADER_SIZE = sum(field[1] for field in [
 	('size', 4),
 	('reserved1', 4),
@@ -22,14 +23,49 @@
 	('version_network_type', 4),
 	('max_fee', 8),
 	('deadline', 8),
 	('transactions_hash', Hash256.SIZE)
 ])
 
 
+# region SymbolPublicAccount / SymbolAccount
+
+class SymbolPublicAccount:
+	"""Symbol public account."""
+
+	def __init__(self, facade, public_key):
+		"""Creates a Symbol public account."""
+		self._facade = facade
+		self.public_key = public_key
+		self.address = self._facade.network.public_key_to_address(self.public_key)
+
+
+class SymbolAccount(SymbolPublicAccount):
+	"""Symbol account."""
+
+	def __init__(self, facade, key_pair):
+		"""Creates a Symbol account."""
+		super().__init__(facade, key_pair.public_key)
+		self.key_pair = key_pair
+
+	def message_encoder(self):
+		"""Creates a message encoder that can be used for encrypting and encoding messages between two parties."""
+		return MessageEncoder(self.key_pair)
+
+	def sign_transaction(self, transaction):
+		"""Signs a Symbol transaction."""
+		return self._facade.sign_transaction(self.key_pair, transaction)
+
+	def cosign_transaction(self, transaction, detached=False):
+		"""Cosigns a Symbol transaction."""
+		return self._facade.cosign_transaction(self.key_pair, transaction, detached)
+
+# endregion
+
+
 class SymbolFacade:
 	"""Facade used to interact with Symbol blockchain."""
 
 	BIP32_CURVE_NAME = 'ed25519'
 
 	Address = Address  # pylint: disable=duplicate-code
 	KeyPair = KeyPair  # pylint: disable=duplicate-code
@@ -59,14 +95,22 @@
 			PublicKey: 'public_key',
 		}
 
 	def now(self):
 		"""Creates a network timestamp representing the current time."""
 		return self.network.from_datetime(datetime.now(timezone.utc))
 
+	def create_public_account(self, public_key):
+		"""Creates a Symbol public account from a public key."""
+		return SymbolPublicAccount(self, public_key)
+
+	def create_account(self, private_key):
+		"""Creates a Symbol account from a private key."""
+		return SymbolAccount(self, KeyPair(private_key))
+
 	def hash_transaction(self, transaction):
 		"""Hashes a Symbol transaction."""
 		hasher = hashlib.sha3_256()
 		hasher.update(transaction.signature.bytes)
 		hasher.update(transaction.signer_public_key.bytes)
 		hasher.update(self.network.generation_hash_seed.bytes)
 		hasher.update(self._transaction_data_buffer(transaction.serialize()))
```

### Comparing `symbol_sdk_python-3.2.0/symbolchain/impl/CipherHelpers.py` & `symbol_sdk_python-3.2.2/symbolchain/impl/CipherHelpers.py`

 * *Files identical despite different names*

### Comparing `symbol_sdk_python-3.2.0/symbolchain/nc/__init__.py` & `symbol_sdk_python-3.2.2/symbolchain/nc/__init__.py`

 * *Files identical despite different names*

### Comparing `symbol_sdk_python-3.2.0/symbolchain/nem/KeyPair.py` & `symbol_sdk_python-3.2.2/symbolchain/nem/KeyPair.py`

 * *Files identical despite different names*

### Comparing `symbol_sdk_python-3.2.0/symbolchain/nem/MessageEncoder.py` & `symbol_sdk_python-3.2.2/symbolchain/nem/MessageEncoder.py`

 * *Files 4% similar despite different names*

```diff
@@ -13,14 +13,20 @@
 	"""Encrypts and encodes messages between two parties."""
 
 	def __init__(self, key_pair: KeyPair):
 		"""Creates message encoder around key pair."""
 
 		self.key_pair = key_pair
 
+	@property
+	def public_key(self):
+		"""Public key used for message encoding."""
+
+		return self.key_pair.public_key
+
 	def try_decode(self, recipient_public_key, encoded_message: Message):
 		"""Tries to decode encoded message, returns tuple:
 		* True, message - if message has been decoded and decrypted
 		* False, encoded_message - otherwise
 		"""
 
 		if MessageType.ENCRYPTED != encoded_message.message_type:
```

### Comparing `symbol_sdk_python-3.2.0/symbolchain/nem/Network.py` & `symbol_sdk_python-3.2.2/symbolchain/nem/Network.py`

 * *Files identical despite different names*

### Comparing `symbol_sdk_python-3.2.0/symbolchain/nem/SharedKey.py` & `symbol_sdk_python-3.2.2/symbolchain/nem/SharedKey.py`

 * *Files identical despite different names*

### Comparing `symbol_sdk_python-3.2.0/symbolchain/nem/TransactionFactory.py` & `symbol_sdk_python-3.2.2/symbolchain/nem/TransactionFactory.py`

 * *Files 3% similar despite different names*

```diff
@@ -36,14 +36,19 @@
 		# hack: explicitly translate transfer message
 		if nc.TransactionType.TRANSFER == transaction.type_ and transaction.message and isinstance(transaction.message.message, str):
 			transaction.message.message = transaction.message.message.encode('utf8')
 
 		return transaction
 
 	@staticmethod
+	def deserialize(payload):
+		"""Deserializes a transaction from a binary payload."""
+		return nc.TransactionFactory.deserialize(payload)
+
+	@staticmethod
 	def to_non_verifiable_transaction(transaction):
 		"""Converts a transaction to a non-verifiable transaction."""
 		non_verifiable_class_name = type(transaction).__name__
 		if not non_verifiable_class_name.startswith('NonVerifiable'):
 			non_verifiable_class_name = f'NonVerifiable{non_verifiable_class_name}'
 
 		non_verifiable_class = getattr(nc, non_verifiable_class_name)
```

### Comparing `symbol_sdk_python-3.2.0/symbolchain/sc/__init__.py` & `symbol_sdk_python-3.2.2/symbolchain/sc/__init__.py`

 * *Files identical despite different names*

### Comparing `symbol_sdk_python-3.2.0/symbolchain/symbol/IdGenerator.py` & `symbol_sdk_python-3.2.2/symbolchain/symbol/IdGenerator.py`

 * *Files identical despite different names*

### Comparing `symbol_sdk_python-3.2.0/symbolchain/symbol/KeyPair.py` & `symbol_sdk_python-3.2.2/symbolchain/symbol/KeyPair.py`

 * *Files identical despite different names*

### Comparing `symbol_sdk_python-3.2.0/symbolchain/symbol/Merkle.py` & `symbol_sdk_python-3.2.2/symbolchain/symbol/Merkle.py`

 * *Files identical despite different names*

### Comparing `symbol_sdk_python-3.2.0/symbolchain/symbol/MessageEncoder.py` & `symbol_sdk_python-3.2.2/symbolchain/symbol/MessageEncoder.py`

 * *Files 5% similar despite different names*

```diff
@@ -16,14 +16,20 @@
 	"""Encrypts and encodes messages between two parties."""
 
 	def __init__(self, key_pair: KeyPair):
 		"""Creates message encoder around key pair."""
 
 		self.key_pair = key_pair
 
+	@property
+	def public_key(self):
+		"""Public key used for message encoding."""
+
+		return self.key_pair.public_key
+
 	def try_decode(self, recipient_public_key, encoded_message):
 		"""Tries to decode encoded message, returns tuple:
 		* True, message - if message has been decoded and decrypted
 		* False, encoded_message - otherwise
 		"""
 
 		if 1 == encoded_message[0]:
```

### Comparing `symbol_sdk_python-3.2.0/symbolchain/symbol/TransactionFactory.py` & `symbol_sdk_python-3.2.2/symbolchain/symbol/TransactionFactory.py`

 * *Files 6% similar despite different names*

```diff
@@ -52,14 +52,24 @@
 		Creates an embedded transaction from a transaction descriptor.
 		When autosort is set (default), descriptor arrays requiring ordering will be automatically sorted.
 		When unset, descriptor arrays will be presumed to be already sorted.
 		"""
 		return self._create_and_extend(transaction_descriptor, autosort, sc.EmbeddedTransactionFactory)
 
 	@staticmethod
+	def deserialize(payload):
+		"""Deserializes a transaction from a binary payload."""
+		return sc.TransactionFactory.deserialize(payload)
+
+	@staticmethod
+	def deserialize_embedded(payload):
+		"""Deserializes an embedded transaction from a binary payload."""
+		return sc.EmbeddedTransactionFactory.deserialize(payload)
+
+	@staticmethod
 	def attach_signature(transaction, signature):
 		"""Attaches a signature to a transaction."""
 		transaction.signature = sc.Signature(signature.bytes)
 
 		transaction_buffer = transaction.serialize()
 		hex_payload = hexlify(transaction_buffer).decode('utf8').upper()
 		json_payload = f'{{"payload": "{hex_payload}"}}'
```

### Comparing `symbol_sdk_python-3.2.0/symbolchain/symbol/VotingKeysGenerator.py` & `symbol_sdk_python-3.2.2/symbolchain/symbol/VotingKeysGenerator.py`

 * *Files identical despite different names*

### Comparing `symbol_sdk_python-3.2.0/PKG-INFO` & `symbol_sdk_python-3.2.2/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: symbol-sdk-python
-Version: 3.2.0
+Version: 3.2.2
 Summary: Symbol SDK
 Home-page: https://github.com/symbol/symbol/tree/main/sdk/python
 License: MIT
 Keywords: symbol,sdk,Symbol SDK
 Author: Symbol Contributors
 Author-email: contributors@symbol.dev
 Maintainer: Symbol Contributors
```

