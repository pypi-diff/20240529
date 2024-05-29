# Comparing `tmp/pons-0.7.0.tar.gz` & `tmp/pons-0.8.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pons-0.7.0.tar", last modified: Sun Jul  9 20:57:11 2023, max compression
+gzip compressed data, was "pons-0.8.0.tar", last modified: Wed May 29 03:47:32 2024, max compression
```

## Comparing `pons-0.7.0.tar` & `pons-0.8.0.tar`

### file list

```diff
@@ -1,43 +1,44 @@
--rw-r--r--   0        0        0      177 2022-04-23 23:56:47.860000 pons-0.7.0/.coveragerc
--rw-r--r--   0        0        0     1055 2022-02-27 04:36:26.110000 pons-0.7.0/LICENSE.md
--rw-r--r--   0        0        0     1051 2022-06-06 01:00:07.570000 pons-0.7.0/README.md
--rw-r--r--   0        0        0      638 2022-02-28 05:30:25.300000 pons-0.7.0/docs/Makefile
--rw-r--r--   0        0        0     4665 2023-06-01 23:14:39.716552 pons-0.7.0/docs/api.rst
--rw-r--r--   0        0        0     5097 2023-07-09 20:51:06.297956 pons-0.7.0/docs/changelog.rst
--rw-r--r--   0        0        0     2565 2023-02-05 09:02:39.350000 pons-0.7.0/docs/conf.py
--rw-r--r--   0        0        0     3177 2022-09-14 20:33:08.940000 pons-0.7.0/docs/index.rst
--rw-r--r--   0        0        0     7116 2023-06-01 23:14:39.717149 pons-0.7.0/docs/tutorial.rst
--rw-r--r--   0        0        0      164 2023-06-02 00:42:13.657633 pons-0.7.0/mypy.ini
--rw-r--r--   0        0        0      768 2023-06-01 23:14:39.717416 pons-0.7.0/pons/__init__.py
--rw-r--r--   0        0        0    18498 2023-05-31 23:30:41.956540 pons-0.7.0/pons/_abi_types.py
--rw-r--r--   0        0        0    29885 2023-06-01 23:14:39.717747 pons-0.7.0/pons/_client.py
--rw-r--r--   0        0        0     6174 2023-06-01 23:14:39.717918 pons-0.7.0/pons/_contract.py
--rw-r--r--   0        0        0    26702 2023-06-01 23:14:39.718290 pons-0.7.0/pons/_contract_abi.py
--rw-r--r--   0        0        0    19703 2023-05-31 23:30:41.957089 pons-0.7.0/pons/_entities.py
--rw-r--r--   0        0        0     6384 2023-05-31 23:30:41.957231 pons-0.7.0/pons/_fallback_provider.py
--rw-r--r--   0        0        0     6329 2023-05-31 23:30:41.957394 pons-0.7.0/pons/_provider.py
--rw-r--r--   0        0        0     1227 2022-08-17 18:47:24.899999 pons-0.7.0/pons/_signer.py
--rw-r--r--   0        0        0      757 2022-04-24 22:22:36.230000 pons-0.7.0/pons/abi.py
--rw-r--r--   0        0        0        0 2022-04-23 23:56:47.860000 pons-0.7.0/pons/py.typed
--rw-r--r--   0        0        0     1215 2023-07-09 20:51:35.471942 pons-0.7.0/pyproject.toml
--rw-r--r--   0        0        0       26 2022-04-25 23:59:46.280000 pons-0.7.0/pytest.ini
--rw-r--r--   0        0        0      887 2023-06-01 05:58:07.212219 pons-0.7.0/tests/MockMulticall.sol
--rw-r--r--   0        0        0     2399 2022-06-05 01:05:34.940000 pons-0.7.0/tests/TestClient.sol
--rw-r--r--   0        0        0      939 2022-05-25 05:17:34.620000 pons-0.7.0/tests/TestContract.sol
--rw-r--r--   0        0        0     2165 2023-06-01 23:14:39.718768 pons-0.7.0/tests/TestContractFunctionality.sol
--rw-r--r--   0        0        0      343 2022-03-06 23:50:17.740000 pons-0.7.0/tests/__init__.py
--rw-r--r--   0        0        0      640 2022-05-24 03:06:04.490000 pons-0.7.0/tests/compile.py
--rw-r--r--   0        0        0      585 2022-06-05 01:05:34.940000 pons-0.7.0/tests/conftest.py
--rw-r--r--   0        0        0    10957 2023-06-01 23:14:39.718925 pons-0.7.0/tests/provider.py
--rw-r--r--   0        0        0     2648 2022-09-14 20:33:08.940000 pons-0.7.0/tests/provider_server.py
--rw-r--r--   0        0        0    11849 2023-05-31 23:30:41.957552 pons-0.7.0/tests/test_abi_types.py
--rw-r--r--   0        0        0    35138 2023-06-01 23:14:39.719144 pons-0.7.0/tests/test_client.py
--rw-r--r--   0        0        0     4513 2023-06-01 23:14:39.719300 pons-0.7.0/tests/test_contract.py
--rw-r--r--   0        0        0    22359 2023-06-01 23:14:39.719514 pons-0.7.0/tests/test_contract_abi.py
--rw-r--r--   0        0        0     6520 2023-06-01 23:14:39.719775 pons-0.7.0/tests/test_contract_functionality.py
--rw-r--r--   0        0        0    12207 2023-05-26 17:16:32.160667 pons-0.7.0/tests/test_entities.py
--rw-r--r--   0        0        0     7854 2023-05-31 23:30:41.957944 pons-0.7.0/tests/test_fallback_provider.py
--rw-r--r--   0        0        0     1982 2023-06-01 22:02:43.711692 pons-0.7.0/tests/test_multicall.py
--rw-r--r--   0        0        0     7389 2023-05-31 23:30:41.958172 pons-0.7.0/tests/test_provider.py
--rw-r--r--   0        0        0     1209 2022-06-05 01:05:34.950000 pons-0.7.0/tests/test_signer.py
--rw-r--r--   0        0        0     1386 1970-01-01 00:00:00.000000 pons-0.7.0/PKG-INFO
+-rw-r--r--   0        0        0      177 2022-04-23 23:56:47.860000 pons-0.8.0/.coveragerc
+-rw-r--r--   0        0        0     1055 2022-02-27 04:36:26.110000 pons-0.8.0/LICENSE.md
+-rw-r--r--   0        0        0     1059 2024-05-29 03:34:49.131921 pons-0.8.0/README.md
+-rw-r--r--   0        0        0      638 2022-02-28 05:30:25.300000 pons-0.8.0/docs/Makefile
+-rw-r--r--   0        0        0     4609 2024-05-29 03:34:49.132372 pons-0.8.0/docs/api.rst
+-rw-r--r--   0        0        0     9188 2024-05-29 03:46:57.112617 pons-0.8.0/docs/changelog.rst
+-rw-r--r--   0        0        0     2682 2024-05-29 03:34:49.133335 pons-0.8.0/docs/conf.py
+-rw-r--r--   0        0        0     3248 2024-05-29 03:34:49.133809 pons-0.8.0/docs/index.rst
+-rw-r--r--   0        0        0     7106 2024-05-29 03:34:49.134190 pons-0.8.0/docs/tutorial.rst
+-rw-r--r--   0        0        0     2094 2024-05-29 03:34:49.135920 pons-0.8.0/pons/__init__.py
+-rw-r--r--   0        0        0    18307 2024-05-29 03:34:49.136337 pons-0.8.0/pons/_abi_types.py
+-rw-r--r--   0        0        0    32634 2024-05-29 03:34:49.136962 pons-0.8.0/pons/_client.py
+-rw-r--r--   0        0        0     2402 2024-05-29 03:34:49.137260 pons-0.8.0/pons/_compiler.py
+-rw-r--r--   0        0        0     6059 2024-05-29 03:34:49.137683 pons-0.8.0/pons/_contract.py
+-rw-r--r--   0        0        0    30275 2024-05-29 03:34:49.138078 pons-0.8.0/pons/_contract_abi.py
+-rw-r--r--   0        0        0     7065 2024-05-29 03:34:49.138500 pons-0.8.0/pons/_fallback_provider.py
+-rw-r--r--   0        0        0     4057 2024-05-29 03:34:49.138828 pons-0.8.0/pons/_http_provider_server.py
+-rw-r--r--   0        0        0     2719 2024-05-29 03:45:25.649699 pons-0.8.0/pons/_local_provider.py
+-rw-r--r--   0        0        0     5434 2024-05-29 03:34:49.139541 pons-0.8.0/pons/_provider.py
+-rw-r--r--   0        0        0     1770 2024-05-29 03:34:49.139773 pons-0.8.0/pons/_signer.py
+-rw-r--r--   0        0        0      829 2024-03-05 23:03:39.115235 pons-0.8.0/pons/abi.py
+-rw-r--r--   0        0        0        0 2022-04-23 23:56:47.860000 pons-0.8.0/pons/py.typed
+-rw-r--r--   0        0        0     2168 2024-05-29 03:46:42.676370 pons-0.8.0/pyproject.toml
+-rw-r--r--   0        0        0      887 2023-06-01 05:58:07.212219 pons-0.8.0/tests/MockMulticall.sol
+-rw-r--r--   0        0        0     3218 2024-02-20 04:04:30.142988 pons-0.8.0/tests/TestClient.sol
+-rw-r--r--   0        0        0       80 2023-12-31 01:32:18.502539 pons-0.8.0/tests/TestCompiler.sol
+-rw-r--r--   0        0        0      101 2023-12-31 01:32:18.502611 pons-0.8.0/tests/TestCompilerWithImport.sol
+-rw-r--r--   0        0        0      939 2022-05-25 05:17:34.620000 pons-0.8.0/tests/TestContract.sol
+-rw-r--r--   0        0        0     2411 2024-05-29 03:45:25.650148 pons-0.8.0/tests/TestContractFunctionality.sol
+-rw-r--r--   0        0        0      235 2023-12-31 06:33:44.994485 pons-0.8.0/tests/TestLocalProvider.sol
+-rw-r--r--   0        0        0     1983 2024-02-03 19:11:19.200520 pons-0.8.0/tests/_test_multicall.py
+-rw-r--r--   0        0        0      579 2024-05-29 03:45:25.650492 pons-0.8.0/tests/conftest.py
+-rw-r--r--   0        0        0    12530 2024-05-29 03:34:49.141107 pons-0.8.0/tests/test_abi_types.py
+-rw-r--r--   0        0        0    45842 2024-05-29 03:34:49.141620 pons-0.8.0/tests/test_client.py
+-rw-r--r--   0        0        0      656 2024-05-29 01:50:30.168655 pons-0.8.0/tests/test_compiler.py
+-rw-r--r--   0        0        0     4516 2024-05-29 03:34:49.142059 pons-0.8.0/tests/test_contract.py
+-rw-r--r--   0        0        0    26194 2024-05-29 03:34:49.142455 pons-0.8.0/tests/test_contract_abi.py
+-rw-r--r--   0        0        0     7133 2024-05-29 03:45:25.650967 pons-0.8.0/tests/test_contract_functionality.py
+-rw-r--r--   0        0        0     7740 2024-05-29 03:34:49.143064 pons-0.8.0/tests/test_fallback_provider.py
+-rw-r--r--   0        0        0     1305 2024-05-29 03:34:49.143399 pons-0.8.0/tests/test_http_provider_server.py
+-rw-r--r--   0        0        0     2927 2024-05-29 03:34:49.143615 pons-0.8.0/tests/test_local_provider.py
+-rw-r--r--   0        0        0     7482 2024-05-29 03:34:49.143993 pons-0.8.0/tests/test_provider.py
+-rw-r--r--   0        0        0     1465 2024-05-29 03:34:49.144235 pons-0.8.0/tests/test_signer.py
+-rw-r--r--   0        0        0     1455 1970-01-01 00:00:00.000000 pons-0.8.0/PKG-INFO
```

### Comparing `pons-0.7.0/LICENSE.md` & `pons-0.8.0/LICENSE.md`

 * *Files identical despite different names*

### Comparing `pons-0.7.0/README.md` & `pons-0.8.0/README.md`

 * *Files 11% similar despite different names*

```diff
@@ -9,11 +9,11 @@
 
 
 [pypi-image]: https://img.shields.io/pypi/v/pons
 [pypi-link]: https://pypi.org/project/pons/
 [pypi-license-image]: https://img.shields.io/pypi/l/pons
 [rtd-image]: https://readthedocs.org/projects/pons/badge/?version=latest
 [rtd-link]: https://pons.readthedocs.io/en/latest/
-[cov-image]: https://codecov.io/gh/fjarri/pons/branch/master/graph/badge.svg?token=RZP1LK1HB2
-[cov-link]: https://codecov.io/gh/fjarri/pons
+[cov-image]: https://codecov.io/gh/fjarri-eth/pons/branch/master/graph/badge.svg?token=RZP1LK1HB2
+[cov-link]: https://codecov.io/gh/fjarri-eth/pons
 [black-image]: https://img.shields.io/badge/code%20style-black-000000.svg
 [black-link]: https://github.com/psf/black
```

### Comparing `pons-0.7.0/docs/Makefile` & `pons-0.8.0/docs/Makefile`

 * *Files identical despite different names*

### Comparing `pons-0.7.0/docs/api.rst` & `pons-0.8.0/docs/api.rst`

 * *Files 15% similar despite different names*

```diff
@@ -6,22 +6,22 @@
 
 Clients
 -------
 
 .. autoclass:: Client
    :members:
 
-.. autoclass:: pons._client.ClientSession()
+.. autoclass:: ClientSession()
    :members:
 
 
 Providers
 ---------
 
-.. autoclass:: pons._provider.Provider
+.. autoclass:: Provider
 
 .. autoclass:: HTTPProvider
    :show-inheritance:
 
 
 Fallback providers
 ------------------
@@ -47,18 +47,17 @@
 
 .. autoclass:: pons.ABIDecodingError
 
 .. autoclass:: pons.RemoteError
 
 .. autoclass:: pons.Unreachable
 
-.. autoclass:: pons.TransactionFailed
+.. autoclass:: pons.ProtocolError
 
-.. autoclass:: pons._client.ProviderErrorCode
-   :members:
+.. autoclass:: pons.TransactionFailed
 
 .. autoclass:: pons.ProviderError()
    :show-inheritance:
    :members:
 
 .. autoclass:: pons._client.ContractPanicReason
    :members:
@@ -79,14 +78,15 @@
 Signers
 -------
 
 .. autoclass:: Signer
    :members:
 
 .. autoclass:: AccountSigner
+   :members:
    :show-inheritance:
 
 
 Contract ABI
 ------------
 
 .. autoclass:: ContractABI
@@ -99,58 +99,96 @@
    :members:
    :special-members: __call__
 
 .. autoclass:: Method
    :members:
    :special-members: __call__
 
+.. autoclass:: MultiMethod
+   :members:
+   :special-members: __call__
+
 .. autoclass:: Event
    :members:
 
 .. autoclass:: Error
    :members:
 
 .. autoclass:: Fallback
    :members:
 
 .. autoclass:: Receive
    :members:
 
 
+Testing utilities
+-----------------
+
+``pons`` exposes several types useful for testing applications that connect to Ethereum RPC servers. Not intended for the production environment.
+
+Install with the feature ``local-provider`` for it to be available.
+
+
+.. autoclass:: LocalProvider
+   :show-inheritance:
+   :members: disable_auto_mine_transactions, enable_auto_mine_transactions, take_snapshot, revert_to_snapshot
+
+.. autoclass:: SnapshotID
+
+.. autoclass:: HTTPProviderServer
+   :members:
+   :special-members: __call__
+
+
+Compiler
+--------
+
+Install with the feature ``compiler`` for it to be available.
+
+
+.. autofunction:: compile_contract_file
+
+.. autoclass:: EVMVersion
+   :members:
+
+
 Secondary classes
 -----------------
 
-.. autoclass:: pons._contract_abi.ConstructorCall()
+The instances of these classes are not created by the user directly, but rather found as return values, or attributes of other objects.
+
+
+.. autoclass:: ConstructorCall()
    :members:
 
-.. autoclass:: pons._contract_abi.MethodCall()
+.. autoclass:: MethodCall()
    :members:
 
-.. autoclass:: pons._contract_abi.EventFilter()
+.. autoclass:: EventFilter()
    :members:
 
-.. autoclass:: pons._contract.BoundConstructor()
+.. autoclass:: BoundConstructor()
    :members:
    :special-members: __call__
 
-.. autoclass:: pons._contract.BoundConstructorCall()
+.. autoclass:: BoundConstructorCall()
    :members:
 
-.. autoclass:: pons._contract.BoundMethod()
+.. autoclass:: BoundMethod()
    :members:
    :special-members: __call__
 
-.. autoclass:: pons._contract.BoundMethodCall()
+.. autoclass:: BoundMethodCall()
    :members:
 
-.. autoclass:: pons._contract.BoundEvent()
+.. autoclass:: BoundEvent()
    :members:
    :special-members: __call__
 
-.. autoclass:: pons._contract.BoundEventFilter()
+.. autoclass:: BoundEventFilter()
    :members:
 
 
 Utility classes
 ---------------
 
 .. autoclass:: pons._contract_abi.Methods()
@@ -174,64 +212,22 @@
 .. autoclass:: CompiledContract
    :members:
 
 .. autoclass:: DeployedContract
    :members:
 
 
-Entities
---------
-
-.. autoclass:: Amount
-   :members:
-
-.. class:: pons._entities.CustomAmount
-
-   A type derived from :py:class:`Amount`.
-
-.. autoclass:: Address
-   :members:
-
-.. class:: pons._entities.CustomAddress
-
-   A type derived from :py:class:`Address`.
-
-.. autoclass:: Block()
-   :members:
-
-.. autoclass:: TxHash
-   :members:
-
-.. autoclass:: BlockHash
-   :members:
-
-.. autoclass:: pons._entities.TxReceipt()
-   :members:
-
-.. autoclass:: pons._entities.BlockInfo()
-   :members:
-
-.. autoclass:: pons._entities.TxInfo()
-   :members:
-
-.. autoclass:: pons._entities.BlockFilter()
-
-.. autoclass:: pons._entities.PendingTransactionFilter()
-
-.. autoclass:: pons._entities.LogFilter()
-
-.. autoclass:: pons._entities.LogTopic()
+Filter objects
+--------------
 
-.. autoclass:: pons._entities.LogEntry()
-   :members:
+.. autoclass:: pons._client.BlockFilter()
 
-.. class:: JSON
+.. autoclass:: pons._client.PendingTransactionFilter()
 
-   A JSON-ifiable object (``bool``, ``int``, ``float``, ``str``, ``None``,
-   iterable of ``JSON``, or mapping of ``str`` to ``JSON``).
+.. autoclass:: pons._client.LogFilter()
 
 
 Solidity types
 --------------
 
 Type aliases are exported from the ``abi`` submodule.
 Arrays can be obtained from ``Type`` objects by indexing them (either with an integer for a fixed-size array, or with ``...`` for a variable-sized array).
```

### Comparing `pons-0.7.0/docs/conf.py` & `pons-0.8.0/docs/conf.py`

 * *Files 7% similar despite different names*

```diff
@@ -10,20 +10,19 @@
 # add these directories to sys.path here. If the directory is relative to the
 # documentation root, use os.path.abspath to make it absolute, like shown here.
 #
 # import os
 # import sys
 # sys.path.insert(0, os.path.abspath('.'))
 
-import os
 import importlib.metadata
+import os
 
 import setuptools_scm
 
-
 # -- Project information -----------------------------------------------------
 
 project = "pons"
 copyright = "2022-now, Bogdan Opanchuk"
 author = "Bogdan Opanchuk"
 
 # The full version, including alpha/beta/rc tags
@@ -44,14 +43,15 @@
     "sphinx.ext.intersphinx",
     "sphinx.ext.doctest",
     "sphinx.ext.viewcode",
 ]
 
 autoclass_content = "both"
 autodoc_member_order = "groupwise"
+autodoc_type_aliases = {"JSON": "JSON"}
 
 # Add any paths that contain templates here, relative to this directory.
 templates_path = []
 
 # List of patterns, relative to source directory, that match files and
 # directories to ignore when looking for source files.
 # This pattern also affects html_static_path and html_extra_path.
@@ -71,9 +71,10 @@
 html_static_path = []
 
 # Do not prepend module to type names when it can be resolved.
 python_use_unqualified_type_names = True
 
 intersphinx_mapping = {
     "python": ("https://docs.python.org/3", None),
-    "eth_account": ("https://eth-account.readthedocs.io/en/stable/", None),
+    "eth_account": ("https://eth-account.readthedocs.io/en/v0.13.0/", None),
+    "ethereum_rpc": ("https://ethereum-rpc.readthedocs.io/en/v0.1.0", None),
 }
```

### Comparing `pons-0.7.0/docs/index.rst` & `pons-0.8.0/docs/index.rst`

 * *Files 14% similar despite different names*

```diff
@@ -7,17 +7,18 @@
 
 .. testsetup::
 
     import os
     import trio
     import pons
     import eth_account
+    import ethereum_rpc
 
-    from tests.provider import EthereumTesterProvider
-    from tests.provider_server import ServerHandle
+    from ethereum_rpc import Amount
+    from pons import LocalProvider, HTTPProviderServer
 
     # Run examples with our test server in the background
 
     orig_trio_run = trio.run
 
     def mock_trio_run(func):
         async def wrapper():
@@ -28,61 +29,62 @@
     trio.run = mock_trio_run
 
     # This variable will be set when the server is started
 
     http_provider = None
     pons.HTTPProvider = lambda uri: http_provider
 
-    # This variable will be set when the EthereumTesterProvider is created
+    # This variable will be set when the LocalProvider is created
 
-    root_account = None
+    root_signer = None
     orig_Account_from_key = eth_account.Account.from_key
 
     def mock_Account_from_key(private_key_hex):
         if private_key_hex == "0x<your secret key>":
-            return root_account
+            return root_signer.account
         else:
             return orig_Account_from_key(private_key_hex)
 
     eth_account.Account.from_key = mock_Account_from_key
 
     # So that we don't have to use real addresses
 
-    orig_Address_from_hex = pons.Address.from_hex
+    orig_Address_from_hex = ethereum_rpc.Address.from_hex
 
     def mock_Address_from_hex(address_hex):
         if address_hex == "0x<another_address>":
             return Address(os.urandom(20))
         else:
             return orig_Address_from_hex(address_hex)
 
-    pons.Address.from_hex = mock_Address_from_hex
+    ethereum_rpc.Address.from_hex = mock_Address_from_hex
 
     # This function will start a test server and fill in some global variables
 
     async def run_with_server(func):
-        global root_account
+        global root_signer
         global http_provider
 
-        test_provider = EthereumTesterProvider()
-        root_account = test_provider.root_account
+        local_provider = LocalProvider(root_balance=Amount.ether(100))
+        root_signer = local_provider.root
 
         async with trio.open_nursery() as nursery:
-            handle = ServerHandle(test_provider)
+            handle = HTTPProviderServer(local_provider)
             http_provider = handle.http_provider
             await nursery.start(handle)
             await func()
             await handle.shutdown()
 
 .. testcode::
 
     import trio
 
     from eth_account import Account
-    from pons import Client, HTTPProvider, AccountSigner, Address, Amount
+    from ethereum_rpc import Address, Amount
+    from pons import Client, HTTPProvider, AccountSigner
 
     async def main():
 
         provider = HTTPProvider("<your provider's https endpoint>")
         client = Client(provider)
 
         acc = Account.from_key("0x<your secret key>")
```

### Comparing `pons-0.7.0/docs/tutorial.rst` & `pons-0.8.0/docs/tutorial.rst`

 * *Files 1% similar despite different names*

```diff
@@ -13,29 +13,29 @@
 Sessions
 --------
 
 All calls to the provider in ``pons`` happen within a session.
 It translates to the usage of a single session in the backend HTTP request library, so the details are implementation-dependent, but in general it means that multiple requests will happen faster.
 For example, in a session an SSL handshake only happens once, and it is a somewhat slow process.
 
-Correspondingly, all the main functionality of the library is concentrated in the :py:class:`~pons._client.ClientSession` class.
+Correspondingly, all the main functionality of the library is concentrated in the :py:class:`~pons.ClientSession` class.
 
 
 Signers
 -------
 
 Any operation that entails writing information into the blockchain takes a :py:class:`~pons.Signer` object.
 For now, only signers created from ``eth_account.Account`` are supported, but one can define their own class backed by, say, a hardware signer, using the abstract :py:class:`~pons.Signer` class.
 
 
 Amounts and addresses
 ---------------------
 
 Native currency amounts and network addresses are typed in ``pons``.
-All methods expect and return only :py:class:`~pons.Amount` and :py:class:`~pons.Address` objects --- no integers or strings allowed.
+All methods expect and return only :py:class:`ethereum_rpc.Amount` and :py:class:`ethereum_rpc.Address` objects --- no integers or strings allowed.
 
 In an application using ``pons`` one can superclass these classes to distinguish between different types of currencies, or addresses from different networks.
 Note though that all the arithmetic and comparison functions require **strict** type equality and raise an exception if it is not the case, to protect from accidental usage of addresses/amounts from wrong domains.
 
 
 Contract ABI
 ------------
@@ -152,15 +152,15 @@
 
 
 Deploying contracts
 -------------------
 
 In order to deploy a contract one needs its ABI and bytecode.
 At the moment ``pons`` does not expose the compiler interface, so it has to come from a third party library, for example `py-solcx <https://solcx.readthedocs.io/en/latest/>`_.
-With that, create a :py:class:`~pons.CompiledContract` object and use :py:meth:`~pons._client.ClientSession.deploy`:
+With that, create a :py:class:`~pons.CompiledContract` object and use :py:meth:`~pons.ClientSession.deploy`:
 
 ::
 
     compiled_contract = CompiledContract(cabi, bytecode)
     deployed_contract = await session.deploy(signer, compiled_contract.constructor(arg1, arg2))
 
 This will result in a :py:class:`~pons.DeployedContract` object encapsulating the contract address and its ABI and allowing one to interact with the contract.
@@ -174,15 +174,15 @@
 
 Interacting with deployed contracts
 -----------------------------------
 
 A :py:class:`~pons.DeployedContract` object wraps all ABI method objects into "bound" state, similarly to how Python methods are bound to class instances.
 It means that all the method calls created from this object have the contract address inside them, so that it does not need to be provided every time.
 
-For example, to call a non-mutating contract method via :py:meth:`~pons._client.ClientSession.eth_call`:
+For example, to call a non-mutating contract method via :py:meth:`~pons.ClientSession.eth_call`:
 
 ::
 
     call = deployed_contract.method.getState(1)
     result = await session.eth_call(call)
 
 Note that when the :py:class:`~pons.ContractABI` object is created from the JSON ABI, even if the method returns a single value, it is still represented as a list of one element in the JSON, so the ``result`` will be a list too.
```

### Comparing `pons-0.7.0/pons/_abi_types.py` & `pons-0.8.0/pons/_abi_types.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,146 +1,122 @@
+# We need to have some module-private members in `Type`.
+# ruff: noqa: SLF001
+
+import re
 from abc import ABC, abstractmethod
+from collections.abc import Iterable, Mapping, Sequence
 from functools import cached_property
-import re
-from typing import Optional, Any, Union, Iterable, Mapping, Dict, Tuple, Sequence, List, cast
+from types import EllipsisType
+from typing import Any
 
-from eth_abi.exceptions import DecodingError
 import eth_abi
-from eth_utils import keccak
+from eth_abi.exceptions import DecodingError
+from ethereum_rpc import Address, keccak
+
+# Maximum bits in an `int` or `uint` type in Solidity.
+MAX_INTEGER_BITS = 256
 
-from ._entities import Address
+# Maximum size of a `bytes` type in Solidity.
+MAX_BYTES_SIZE = 32
 
 
 class ABIDecodingError(Exception):
-    """
-    Raised on an error when decoding a value in an Eth ABI encoded bytestring.
-    """
+    """Raised on an error when decoding a value in an Eth ABI encoded bytestring."""
 
 
-ABIType = Union[int, str, bytes, bool, List["ABIType"]]
+ABIType = int | str | bytes | bool | list["ABIType"]
 """
 Represents the argument type that can be received from ``eth_abi.decode()``,
 or passed to ``eth_abi.encode()``.
 """
 
 
-def encode_typed(types: Iterable[str], args: Iterable[ABIType]) -> bytes:
-    # ``eth_abi.encode()`` does not have type annotations.
-    # This is a typed wrapper (easier than making custom stubs).
-    # Remove when typing is added in ``eth_abi``.
-    encoded = eth_abi.encode(types, args)
-    return encoded
-
-
-def decode_typed(types: Iterable[str], data: bytes) -> Tuple[ABIType, ...]:
-    # ``eth_abi.decode()`` does not have type annotations.
-    # This is a typed wrapper (easier than making custom stubs).
-    # Remove when typing is added in ``eth_abi``.
-    decoded = eth_abi.decode(types, data)
-    return cast(Tuple[ABIType, ...], decoded)
-
-
 class Type(ABC):
     """The base type for Solidity types."""
 
     @property
     @abstractmethod
     def canonical_form(self) -> str:
-        """
-        Returns the type as a string in the canonical form (for ``eth_abi`` consumption).
-        """
+        """Returns the type as a string in the canonical form (for ``eth_abi`` consumption)."""
         ...
 
     @abstractmethod
     def _normalize(self, val: Any) -> ABIType:
         """
         Checks and possibly normalizes the value making it ready to be passed
         to ``encode()`` for encoding.
         """
         ...
 
     @abstractmethod
     def _denormalize(self, val: ABIType) -> Any:
-        """
-        Checks the result of ``decode()``
-        and wraps it in a specific type, if applicable.
-        """
+        """Checks the result of ``decode()`` and wraps it in a specific type, if applicable."""
         ...
 
     def encode(self, val: Any) -> bytes:
-        """
-        Encodes the given value in the contract ABI format.
-        """
-        return encode_typed([self.canonical_form], [val])
+        """Encodes the given value in the contract ABI format."""
+        return eth_abi.encode([self.canonical_form], [val])
 
     def encode_to_topic(self, val: Any) -> bytes:
-        """
-        Encodes the given value as an event topic.
-        """
+        """Encodes the given value as an event topic."""
         # EVM uses a simpler encoding scheme for encoding values into event topics
         # because objects of reference types are just hashed,
         # and there is no need to unpack them later
         # (basically, all values are just concatenated without any lentgh labels).
         # Therefore we have to provide these methods
         # and cannot just use the functions from ``eth_abi``.
 
         # Before doing anything, normalize the value,
         # this will ensure the constituent values are actually valid.
         return self._encode_to_topic_outer(self._normalize(val))
 
     def _encode_to_topic_outer(self, val: Any) -> bytes:
-        """
-        Encodes a value of the outer indexed type.
-        """
+        """Encodes a value of the outer indexed type."""
         # By default it's just the encoding of the value type.
         # May be overridden.
         return self.encode(val)
 
     def _encode_to_topic_inner(self, val: Any) -> bytes:
-        """
-        Encodes a value contained within an indexed array or struct.
-        """
+        """Encodes a value contained within an indexed array or struct."""
         # By default it's just the encoding of the value type.
         # May be overridden.
         return self.encode(val)
 
-    def decode_from_topic(self, val: bytes) -> Optional[Any]:
+    def decode_from_topic(self, val: bytes) -> Any | None:
         """
         Decodes an encoded topic.
         Returns ``None`` if the decoding is impossible
         (that is, the original value was hashed).
         """
         # This method does not have inner/outer division, since all reference types are hashed,
         # and there's no need to go recursively into structs/arrays - we won't be able to recover
         # the values anyway.
 
         # By default it's just the decoding of the value type.
         # May be overridden.
-        return self._denormalize(decode_typed([self.canonical_form], val)[0])
+        return self._denormalize(eth_abi.decode([self.canonical_form], val)[0])
 
     def __str__(self) -> str:
         return self.canonical_form
 
-    def __getitem__(self, array_size: Union[int, Any]) -> "Array":
+    def __getitem__(self, array_size: int | EllipsisType) -> "Array":
         # In Py3.10 they added EllipsisType which would work better here.
         # For now, relying on the documentation.
         if isinstance(array_size, int):
             return Array(self, array_size)
         if array_size == ...:
             return Array(self, None)
         raise TypeError(f"Invalid array size specifier type: {type(array_size).__name__}")
 
 
 class UInt(Type):
-    """
-    Corresponds to the Solidity ``uint<bits>`` type.
-    """
+    """Corresponds to the Solidity ``uint<bits>`` type."""
 
     def __init__(self, bits: int):
-        if bits <= 0 or bits > 256 or bits % 8 != 0:
+        if bits <= 0 or bits > MAX_INTEGER_BITS or bits % 8 != 0:
             raise ValueError(f"Incorrect `uint` bit size: {bits}")
         self._bits = bits
 
     @property
     def canonical_form(self) -> str:
         return f"uint{self._bits}"
 
@@ -164,25 +140,23 @@
 
     def _normalize(self, val: Any) -> int:
         return self._check_val(val)
 
     def _denormalize(self, val: ABIType) -> int:
         return self._check_val(val)
 
-    def __eq__(self, other: Any) -> bool:
+    def __eq__(self, other: object) -> bool:
         return isinstance(other, UInt) and self._bits == other._bits
 
 
 class Int(Type):
-    """
-    Corresponds to the Solidity ``int<bits>`` type.
-    """
+    """Corresponds to the Solidity ``int<bits>`` type."""
 
     def __init__(self, bits: int):
-        if bits <= 0 or bits > 256 or bits % 8 != 0:
+        if bits <= 0 or bits > MAX_INTEGER_BITS or bits % 8 != 0:
             raise ValueError(f"Incorrect `int` bit size: {bits}")
         self._bits = bits
 
     @property
     def canonical_form(self) -> str:
         return f"int{self._bits}"
 
@@ -202,25 +176,23 @@
 
     def _normalize(self, val: Any) -> int:
         return self._check_val(val)
 
     def _denormalize(self, val: ABIType) -> int:
         return self._check_val(val)
 
-    def __eq__(self, other: Any) -> bool:
+    def __eq__(self, other: object) -> bool:
         return isinstance(other, Int) and self._bits == other._bits
 
 
 class Bytes(Type):
-    """
-    Corresponds to the Solidity ``bytes<size>`` type.
-    """
+    """Corresponds to the Solidity ``bytes<size>`` type."""
 
-    def __init__(self, size: Optional[int] = None):
-        if size is not None and (size <= 0 or size > 32):
+    def __init__(self, size: None | int = None):
+        if size is not None and (size <= 0 or size > MAX_BYTES_SIZE):
             raise ValueError(f"Incorrect `bytes` size: {size}")
         self._size = size
 
     @property
     def canonical_form(self) -> str:
         return f"bytes{self._size if self._size else ''}"
 
@@ -251,28 +223,28 @@
         if self._size is None:
             # Dynamic `bytes` is padded to a multiple of 32 bytes.
             padding_len = (32 - len(val)) % 32
             return val + b"\x00" * padding_len
         # Sized `bytes` is a value type, falls back to the base implementation.
         return super()._encode_to_topic_inner(val)
 
-    def decode_from_topic(self, val: bytes) -> Optional[bytes]:
+    def decode_from_topic(self, val: bytes) -> None | bytes:
         if self._size is None:
             # Cannot recover a hashed value.
             return None
         return super().decode_from_topic(val)
 
-    def __eq__(self, other: Any) -> bool:
+    def __eq__(self, other: object) -> bool:
         return isinstance(other, Bytes) and self._size == other._size
 
 
 class AddressType(Type):
     """
     Corresponds to the Solidity ``address`` type.
-    Not to be confused with :py:class:`~pons.Address` which represents an address value.
+    Not to be confused with :py:class:`ethereum_rpc.Address` which represents an address value.
     """
 
     @property
     def canonical_form(self) -> str:
         return "address"
 
     def _normalize(self, val: Any) -> str:
@@ -284,22 +256,20 @@
         return val.checksum
 
     def _denormalize(self, val: ABIType) -> Address:
         if not isinstance(val, str):
             raise TypeError(f"Expected a string to convert to `Address`, got {type(val).__name__}")
         return Address.from_hex(val)
 
-    def __eq__(self, other: Any) -> bool:
+    def __eq__(self, other: object) -> bool:
         return isinstance(other, AddressType)
 
 
 class String(Type):
-    """
-    Corresponds to the Solidity ``string`` type.
-    """
+    """Corresponds to the Solidity ``string`` type."""
 
     @property
     def canonical_form(self) -> str:
         return "string"
 
     def _check_val(self, val: Any) -> str:
         if not isinstance(val, str):
@@ -318,26 +288,24 @@
         # `string` is encoded and treated as dynamic `bytes`
         return Bytes()._encode_to_topic_outer(val.encode())
 
     def _encode_to_topic_inner(self, val: str) -> bytes:
         # `string` is encoded and treated as dynamic `bytes`
         return Bytes()._encode_to_topic_inner(val.encode())
 
-    def decode_from_topic(self, val: bytes) -> None:
+    def decode_from_topic(self, _val: bytes) -> None:
         # Dynamic `string` is hashed, so the value cannot be recovered.
         return None
 
-    def __eq__(self, other: Any) -> bool:
+    def __eq__(self, other: object) -> bool:
         return isinstance(other, String)
 
 
 class Bool(Type):
-    """
-    Corresponds to the Solidity ``bool`` type.
-    """
+    """Corresponds to the Solidity ``bool`` type."""
 
     @property
     def canonical_form(self) -> str:
         return "bool"
 
     def _check_val(self, val: Any) -> bool:
         if not isinstance(val, bool):
@@ -348,24 +316,22 @@
 
     def _normalize(self, val: Any) -> bool:
         return self._check_val(val)
 
     def _denormalize(self, val: ABIType) -> bool:
         return self._check_val(val)
 
-    def __eq__(self, other: Any) -> bool:
+    def __eq__(self, other: object) -> bool:
         return isinstance(other, Bool)
 
 
 class Array(Type):
-    """
-    Corresponds to the Solidity array (``[<size>]``) type.
-    """
+    """Corresponds to the Solidity array (``[<size>]``) type."""
 
-    def __init__(self, element_type: Type, size: Optional[int] = None):
+    def __init__(self, element_type: Type, size: None | int = None):
         self._element_type = element_type
         self._size = size
 
     @cached_property
     def canonical_form(self) -> str:
         return (
             self._element_type.canonical_form + "[" + (str(self._size) if self._size else "") + "]"
@@ -374,41 +340,39 @@
     def _check_val(self, val: Any) -> Sequence[Any]:
         if not isinstance(val, Sequence):
             raise TypeError(f"Expected an iterable, got {type(val).__name__}")
         if self._size is not None and len(val) != self._size:
             raise ValueError(f"Expected {self._size} elements, got {len(val)}")
         return val
 
-    def _normalize(self, val: Any) -> List[ABIType]:
+    def _normalize(self, val: Any) -> list[ABIType]:
         return [self._element_type._normalize(item) for item in self._check_val(val)]
 
-    def _denormalize(self, val: ABIType) -> List[ABIType]:
+    def _denormalize(self, val: ABIType) -> list[ABIType]:
         return [self._element_type._denormalize(item) for item in self._check_val(val)]
 
     def _encode_to_topic_outer(self, val: Any) -> bytes:
         return keccak(self._encode_to_topic_inner(val))
 
     def _encode_to_topic_inner(self, val: Any) -> bytes:
         return b"".join(self._element_type._encode_to_topic_inner(elem) for elem in val)
 
-    def decode_from_topic(self, val: Any) -> None:
+    def decode_from_topic(self, _val: Any) -> None:
         return None
 
-    def __eq__(self, other: Any) -> bool:
+    def __eq__(self, other: object) -> bool:
         return (
             isinstance(other, Array)
             and self._element_type == other._element_type
             and self._size == other._size
         )
 
 
 class Struct(Type):
-    """
-    Corresponds to the Solidity struct type.
-    """
+    """Corresponds to the Solidity struct type."""
 
     def __init__(self, fields: Mapping[str, Type]):
         self._fields = fields
 
     @cached_property
     def canonical_form(self) -> str:
         return "(" + ",".join(field.canonical_form for field in self._fields.values()) + ")"
@@ -416,47 +380,49 @@
     def _check_val(self, val: Any) -> Sequence[Any]:
         if not isinstance(val, Sequence):
             raise TypeError(f"Expected an iterable, got {type(val).__name__}")
         if len(val) != len(self._fields):
             raise ValueError(f"Expected {len(self._fields)} elements, got {len(val)}")
         return val
 
-    def _normalize(self, val: Any) -> List[ABIType]:
+    def _normalize(self, val: Any) -> list[ABIType]:
         if isinstance(val, Mapping):
             if val.keys() != self._fields.keys():
                 raise ValueError(
                     f"Expected fields {list(self._fields.keys())}, got {list(val.keys())}"
                 )
             return [tp._normalize(val[name]) for name, tp in self._fields.items()]
         return [
-            tp._normalize(item) for item, tp in zip(self._check_val(val), self._fields.values())
+            tp._normalize(item)
+            for item, tp in zip(self._check_val(val), self._fields.values(), strict=True)
         ]
 
-    def _denormalize(self, val: ABIType) -> Dict[str, ABIType]:
+    def _denormalize(self, val: ABIType) -> dict[str, ABIType]:
         return {
             name: tp._denormalize(item)
-            for item, (name, tp) in zip(self._check_val(val), self._fields.items())
+            for item, (name, tp) in zip(self._check_val(val), self._fields.items(), strict=True)
         }
 
     def _encode_to_topic_outer(self, val: Any) -> bytes:
         return keccak(self._encode_to_topic_inner(val))
 
     def _encode_to_topic_inner(self, val: Any) -> bytes:
         return b"".join(
-            tp._encode_to_topic_inner(elem) for elem, tp in zip(val, self._fields.values())
+            tp._encode_to_topic_inner(elem)
+            for elem, tp in zip(val, self._fields.values(), strict=True)
         )
 
-    def decode_from_topic(self, val: Any) -> None:
+    def decode_from_topic(self, _val: Any) -> None:
         return None
 
     def __str__(self) -> str:
         # Overriding  the `Type`'s implementation because we want to show the field names too
         return "(" + ", ".join(str(tp) + " " + str(name) for name, tp in self._fields.items()) + ")"
 
-    def __eq__(self, other: Any) -> bool:
+    def __eq__(self, other: object) -> bool:
         return (
             isinstance(other, Struct)
             and self._fields == other._fields
             # structs with the same fields but in different order are not equal
             and list(self._fields) == list(other._fields)
         )
 
@@ -498,49 +464,57 @@
         array_size = int(array_size)
 
     if is_array:
         element_entry = dict(abi_entry)
         element_entry["type"] = element_type_name
         element_type = dispatch_type(element_entry)
         return Array(element_type, array_size)
-    elif element_type_name == "tuple":
+
+    if element_type_name == "tuple":
         fields = {}
         for component in abi_entry["components"]:
             fields[component["name"]] = dispatch_type(component)
         return Struct(fields)
-    else:
-        return type_from_abi_string(element_type_name)
 
+    return type_from_abi_string(element_type_name)
 
-def dispatch_types(abi_entry: Iterable[Dict[str, Any]]) -> Dict[str, Type]:
-    # Since we are returning a dictionary, need to be sure we don't silently merge entries
+
+def dispatch_types(abi_entry: Iterable[dict[str, Any]]) -> list[Type] | dict[str, Type]:
     names = [entry["name"] for entry in abi_entry]
+
+    # Unnamed arguments; treat as positional arguments
+    if names and all(not name for name in names):
+        return [dispatch_type(entry) for entry in abi_entry]
+
+    if any(not name for name in names):
+        raise ValueError("Arguments must be either all named or all unnamed")
+
+    # Since we are returning a dictionary, need to be sure we don't silently merge entries
     if len(names) != len(set(names)):
         raise ValueError("All ABI entries must have distinct names")
     return {entry["name"]: dispatch_type(entry) for entry in abi_entry}
 
 
-def encode_args(*types_and_args: Tuple[Type, Any]) -> bytes:
+def encode_args(*types_and_args: tuple[Type, Any]) -> bytes:
     if types_and_args:
-        types, args = zip(*types_and_args)
+        types, args = zip(*types_and_args, strict=True)
     else:
         types, args = (), ()
-    return encode_typed(
+    return eth_abi.encode(
         [tp.canonical_form for tp in types],
-        tuple(tp._normalize(arg) for tp, arg in zip(types, args)),
+        tuple(tp._normalize(arg) for tp, arg in zip(types, args, strict=True)),
     )
 
 
-def decode_args(types: Iterable[Type], data: bytes) -> Tuple[ABIType, ...]:
+def decode_args(types: Iterable[Type], data: bytes) -> tuple[ABIType, ...]:
     canonical_types = [tp.canonical_form for tp in types]
     try:
-        values = decode_typed(canonical_types, data)
+        values = eth_abi.decode(canonical_types, data)
     except DecodingError as exc:
         # wrap possible `eth_abi` errors
         signature = "(" + ",".join(canonical_types) + ")"
         message = (
-            f"Could not decode the return value "
-            f"with the expected signature {signature}: {str(exc)}"
+            f"Could not decode the return value with the expected signature {signature}: {exc}"
         )
         raise ABIDecodingError(message) from exc
 
-    return tuple(tp._denormalize(value) for tp, value in zip(types, values))
+    return tuple(tp._denormalize(value) for tp, value in zip(types, values, strict=True))
```

### Comparing `pons-0.7.0/pons/_contract.py` & `pons-0.8.0/pons/_contract.py`

 * *Files 19% similar despite different names*

```diff
@@ -1,84 +1,81 @@
-from typing import Any, Dict, Tuple, Optional, List
+from typing import Any
+
+from ethereum_rpc import Address, LogEntry, LogTopic
 
 from ._contract_abi import (
     ContractABI,
-    Methods,
-    Method,
+    Error,
     Event,
     EventFilter,
-    Error,
+    Method,
+    Methods,
+    MultiMethod,
 )
-from ._entities import Address, LogEntry, LogTopic
 from ._provider import JSON
 
 
 class BoundConstructor:
-    """
-    A constructor bound to a specific contract's bytecode.
-    """
+    """A constructor bound to a specific contract's bytecode."""
 
     def __init__(self, compiled_contract: "CompiledContract"):
         self._bytecode = compiled_contract.bytecode
         self._contract_abi = compiled_contract.abi
         self._constructor = compiled_contract.abi.constructor
 
     def __call__(self, *args: Any, **kwargs: Any) -> "BoundConstructorCall":
-        """
-        Returns a constructor call with encoded arguments and bytecode.
-        """
+        """Returns a constructor call with encoded arguments and bytecode."""
         call = self._constructor(*args, **kwargs)
         data_bytes = self._bytecode + call.input_bytes
-        return BoundConstructorCall(self._contract_abi, data_bytes, self._constructor.payable)
+        return BoundConstructorCall(
+            self._contract_abi, data_bytes, payable=self._constructor.payable
+        )
 
 
 class BoundConstructorCall:
-    """
-    A constructor call with encoded arguments and bytecode.
-    """
+    """A constructor call with encoded arguments and bytecode."""
 
     contract_abi: ContractABI
     """The corresponding contract's ABI"""
 
     payable: bool
     """Whether this call is payable."""
 
     data_bytes: bytes
     """Encoded arguments and the contract's bytecode."""
 
-    def __init__(self, contract_abi: ContractABI, data_bytes: bytes, payable: bool):
+    def __init__(self, contract_abi: ContractABI, data_bytes: bytes, *, payable: bool):
         self.contract_abi = contract_abi
         self.payable = payable
         self.data_bytes = data_bytes
 
 
 class BoundMethod:
-    """
-    A regular method bound to a specific contract's address.
-    """
+    """A regular method bound to a specific contract's address."""
 
-    def __init__(self, contract_abi: ContractABI, contract_address: Address, method: Method):
+    def __init__(
+        self,
+        contract_abi: ContractABI,
+        contract_address: Address,
+        method: Method | MultiMethod,
+    ):
         self._contract_abi = contract_abi
         self._contract_address = contract_address
         self._method = method
 
     def __call__(self, *args: Any, **kwargs: Any) -> "BoundMethodCall":
-        """
-        Returns a contract call with encoded arguments bound to a specific address.
-        """
+        """Returns a contract call with encoded arguments bound to a specific address."""
         call = self._method(*args, **kwargs)
         return BoundMethodCall(
-            self._contract_abi, self._method, self._contract_address, call.data_bytes
+            self._contract_abi, call.method, self._contract_address, call.data_bytes
         )
 
 
 class BoundMethodCall:
-    """
-    A regular method call with encoded arguments bound to a specific contract address.
-    """
+    """A regular method call with encoded arguments bound to a specific contract address."""
 
     contract_abi: ContractABI
     """The corresponding contract's ABI"""
 
     contract_address: Address
     """The contract address."""
 
@@ -102,95 +99,79 @@
         self.contract_abi = contract_abi
         self.contract_address = contract_address
         self.data_bytes = data_bytes
         self.payable = self._method.payable
         self.mutating = self._method.mutating
 
     def decode_output(self, output_bytes: bytes) -> Any:
-        """
-        Decodes contract output packed into the bytestring.
-        """
+        """Decodes contract output packed into the bytestring."""
         return self._method.decode_output(output_bytes)
 
 
 class BoundEvent:
-    """
-    An event creation call with encoded topics bound to a specific contract address.
-    """
+    """An event creation call with encoded topics bound to a specific contract address."""
 
     def __init__(self, contract_address: Address, event: Event):
         self.contract_address = contract_address
         self.event = event
 
     def __call__(self, *args: Any, **kwargs: Any) -> "BoundEventFilter":
-        """
-        Returns an event filter with encoded arguments bound to a specific address.
-        """
+        """Returns an event filter with encoded arguments bound to a specific address."""
         return BoundEventFilter(self.contract_address, self.event, self.event(*args, **kwargs))
 
 
 class BoundEventFilter:
-    """
-    An event filter bound to a specific contract address.
-    """
+    """An event filter bound to a specific contract address."""
 
     contract_address: Address
     """The contract address."""
 
-    topics: Tuple[Optional[Tuple[LogTopic, ...]], ...]
+    topics: tuple[None | tuple[LogTopic, ...], ...]
     """Encoded topics for filtering."""
 
     def __init__(self, contract_address: Address, event: Event, event_filter: EventFilter):
         self.contract_address = contract_address
         self.topics = event_filter.topics
         self._event = event
 
-    def decode_log_entry(self, log_entry: LogEntry) -> Dict[str, Any]:
+    def decode_log_entry(self, log_entry: LogEntry) -> dict[str, Any]:
         if log_entry.address != self.contract_address:
             raise ValueError("Log entry originates from a different contract")
         return self._event.decode_log_entry(log_entry)
 
 
 class CompiledContract:
-    """
-    A compiled contract (ABI and bytecode).
-    """
+    """A compiled contract (ABI and bytecode)."""
 
     abi: ContractABI
     """Contract's ABI."""
 
     bytecode: bytes
     """Contract's bytecode."""
 
     @classmethod
     def from_compiler_output(
-        cls, json_abi: List[Dict[str, JSON]], bytecode: bytes
+        cls, json_abi: list[dict[str, JSON]], bytecode: bytes
     ) -> "CompiledContract":
-        """
-        Creates a compiled contract object from the output of a Solidity compiler.
-        """
+        """Creates a compiled contract object from the output of a Solidity compiler."""
         abi = ContractABI.from_json(json_abi)
         return cls(abi, bytecode)
 
     def __init__(self, abi: ContractABI, bytecode: bytes):
         self.abi = abi
         self.bytecode = bytecode
 
     @property
     def constructor(self) -> BoundConstructor:
-        """
-        Returns the constructor bound to this contract's bytecode.
-        """
+        """Returns the constructor bound to this contract's bytecode."""
         return BoundConstructor(self)
 
 
 class DeployedContract:
-    """
-    A deployed contract (ABI and address).
-    """
+    """A deployed contract (ABI and address)."""
 
     abi: ContractABI
     """Contract's ABI."""
 
     address: Address
     """Contract's address."""
```

### Comparing `pons-0.7.0/pons/_contract_abi.py` & `pons-0.8.0/pons/_contract_abi.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,52 +1,47 @@
-from abc import ABC, abstractmethod
+import inspect
+from collections.abc import Iterable, Iterator, Mapping, Sequence
+from collections.abc import Set as AbstractSet
 from enum import Enum
 from functools import cached_property
-import inspect
+from inspect import BoundArguments
 from itertools import chain
 from keyword import iskeyword
-from typing import (
-    Any,
-    AbstractSet,
-    Iterable,
-    List,
-    Dict,
-    Optional,
-    Union,
-    Mapping,
-    TypeVar,
-    Generic,
-    Iterator,
-    Sequence,
-    Tuple,
-)
+from typing import Any, Generic, TypeVar
+
+from ethereum_rpc import LogEntry, LogTopic, keccak
 
 from . import abi
-from ._abi_types import Type, dispatch_types, dispatch_type, encode_args, decode_args, keccak
-from ._entities import LogTopic, LogEntry
+from ._abi_types import Type, decode_args, dispatch_type, dispatch_types, encode_args
 from ._provider import JSON
 
+# Anonymous events can have at most 4 indexed fields
+ANONYMOUS_EVENT_INDEXED_FIELDS = 4
+
+# Anonymous events can have at most 4 indexed fields
+EVENT_INDEXED_FIELDS = 3
+
+# The number of bytes in a function selector.
+SELECTOR_LENGTH = 4
+
 
 # We are using the `inspect` machinery to bind arguments to parameters.
 # From Py3.11 on it does not allow parameter names to coincide with keywords,
 # so we have to escape them.
 # This can be avoided if we write our own `inspect.Signature` implementation.
 def make_name_safe(name: str) -> str:
     if iskeyword(name):
         return name + "_"
-    else:
-        return name
+    return name
 
 
 class Signature:
-    """
-    Generalized signature of either inputs or outputs of a method.
-    """
+    """Generalized signature of either inputs or outputs of a method."""
 
-    def __init__(self, parameters: Union[Mapping[str, Type], Sequence[Type]]):
+    def __init__(self, parameters: Mapping[str, Type] | Sequence[Type]):
         if isinstance(parameters, Mapping):
             self._signature = inspect.Signature(
                 parameters=[
                     inspect.Parameter(make_name_safe(name), inspect.Parameter.POSITIONAL_OR_KEYWORD)
                     for name, tp in parameters.items()
                 ]
             )
@@ -64,64 +59,60 @@
 
     @property
     def empty(self) -> bool:
         return not bool(self._types)
 
     @cached_property
     def canonical_form(self) -> str:
-        """
-        Returns the signature serialized in the canonical form as a string.
-        """
+        """Returns the signature serialized in the canonical form as a string."""
         return "(" + ",".join(tp.canonical_form for tp in self._types) + ")"
 
+    def bind(self, *args: Any, **kwargs: Any) -> BoundArguments:
+        return self._signature.bind(*args, **kwargs)
+
+    def encode_bound(self, bound_args: BoundArguments) -> bytes:
+        return encode_args(*zip(self._types, bound_args.args, strict=True))
+
     def encode(self, *args: Any, **kwargs: Any) -> bytes:
         """
         Encodes assorted positional/keyword arguments into the bytestring
         according to the ABI format.
         """
-        bound_args = self._signature.bind(*args, **kwargs)
-        return encode_args(*zip(self._types, bound_args.args))
+        bound_args = self.bind(*args, **kwargs)
+        return self.encode_bound(bound_args)
 
-    def decode_into_tuple(self, value_bytes: bytes) -> Tuple[Any, ...]:
-        """
-        Decodes the packed bytestring into a list of values.
-        """
+    def decode_into_tuple(self, value_bytes: bytes) -> tuple[Any, ...]:
+        """Decodes the packed bytestring into a list of values."""
         return decode_args(self._types, value_bytes)
 
-    def decode_into_dict(self, value_bytes: bytes) -> Dict[str, Any]:
-        """
-        Decodes the packed bytestring into a dict of values.
-        """
+    def decode_into_dict(self, value_bytes: bytes) -> dict[str, Any]:
+        """Decodes the packed bytestring into a dict of values."""
         decoded = self.decode_into_tuple(value_bytes)
-        return dict(zip(self._signature.parameters, decoded))
+        return dict(zip(self._signature.parameters, decoded, strict=True))
 
     def __str__(self) -> str:
         if self._named_parameters:
             params = ", ".join(
                 f"{tp.canonical_form} {name}"
-                for name, tp in zip(self._signature.parameters, self._types)
+                for name, tp in zip(self._signature.parameters, self._types, strict=True)
             )
         else:
             params = ", ".join(f"{tp.canonical_form}" for tp in self._types)
         return f"({params})"
 
 
 class Either:
-    """
-    Denotes an `OR` operation when filtering events.
-    """
+    """Denotes an `OR` operation when filtering events."""
 
     def __init__(self, *items: Any):
         self.items = items
 
 
 class EventSignature:
-    """
-    A signature representing the constructor of an event (that is, its fields).
-    """
+    """A signature representing the constructor of an event (that is, its fields)."""
 
     def __init__(self, parameters: Mapping[str, Type], indexed: AbstractSet[str]):
         parameters = {make_name_safe(name): val for name, val in parameters.items()}
         indexed = {make_name_safe(name) for name in indexed}
         self._signature = inspect.Signature(
             parameters=[
                 inspect.Parameter(name, inspect.Parameter.POSITIONAL_OR_KEYWORD)
@@ -131,25 +122,22 @@
         )
         self._types = parameters
         self._types_nonindexed = {
             name: self._types[name] for name in parameters if name not in indexed
         }
         self._indexed = indexed
 
-    def encode_to_topics(
-        self, *args: Any, **kwargs: Any
-    ) -> Tuple[Optional[Tuple[bytes, ...]], ...]:
+    def encode_to_topics(self, *args: Any, **kwargs: Any) -> tuple[None | tuple[bytes, ...], ...]:
         """
         Binds given arguments to event's indexed parameters
         and encodes them as log topics.
         """
-
         bound_args = self._signature.bind_partial(*args, **kwargs)
 
-        encoded_topics: List[Optional[Tuple[bytes, ...]]] = []
+        encoded_topics: list[None | tuple[bytes, ...]] = []
         for param_name in self._signature.parameters:
             if param_name not in bound_args.arguments:
                 encoded_topics.append(None)
                 continue
 
             bound_val = bound_args.arguments[param_name]
             tp = self._types[param_name]
@@ -164,53 +152,47 @@
 
         # remove trailing `None`s - they are redundant
         while encoded_topics and encoded_topics[-1] is None:
             encoded_topics.pop()
 
         return tuple(encoded_topics)
 
-    def decode_log_entry(self, topics: Sequence[bytes], data: bytes) -> Dict[str, Any]:
-        """
-        Decodes the event fields from the given log entry data.
-        """
+    def decode_log_entry(self, topics: Sequence[bytes], data: bytes) -> dict[str, Any]:
+        """Decodes the event fields from the given log entry data."""
         if len(topics) != len(self._indexed):
             raise ValueError(
                 f"The number of topics in the log entry ({len(topics)}) does not match "
                 f"the number of indexed fields in the event ({len(self._indexed)})"
             )
 
         decoded_topics = {
             name: self._types[name].decode_from_topic(topic)
-            for name, topic in zip(self._signature.parameters, topics)
+            for name, topic in zip(self._signature.parameters, topics, strict=True)
         }
 
         decoded_data_tuple = decode_args(self._types_nonindexed.values(), data)
-        decoded_data = dict(zip(self._types_nonindexed, decoded_data_tuple))
+        decoded_data = dict(zip(self._types_nonindexed, decoded_data_tuple, strict=True))
 
         result = {}
         for name in self._types:
             if name in decoded_topics:
                 result[name] = decoded_topics[name]
             else:
                 result[name] = decoded_data[name]
 
         return result
 
     @cached_property
     def canonical_form(self) -> str:
-        """
-        Returns the signature serialized in the canonical form as a string.
-        """
+        """Returns the signature serialized in the canonical form as a string."""
         return "(" + ",".join(tp.canonical_form for tp in self._types.values()) + ")"
 
     @cached_property
     def canonical_form_nonindexed(self) -> str:
-        """
-        Returns the signature serialized in the canonical form as a string.
-        """
+        """Returns the signature serialized in the canonical form as a string."""
         return "(" + ",".join(tp.canonical_form for tp in self._types_nonindexed.values()) + ")"
 
     def __str__(self) -> str:
         params = []
         for name, tp in self._types.items():
             indexed = "indexed " if name in self._indexed else ""
             params.append(f"{tp.canonical_form} {indexed}{name}")
@@ -230,53 +212,47 @@
     inputs: Signature
     """Input signature."""
 
     payable: bool
     """Whether this method is marked as payable"""
 
     @classmethod
-    def from_json(cls, method_entry: Dict[str, Any]) -> "Constructor":
-        """
-        Creates this object from a JSON ABI method entry.
-        """
+    def from_json(cls, method_entry: dict[str, Any]) -> "Constructor":
+        """Creates this object from a JSON ABI method entry."""
         if method_entry["type"] != "constructor":
             raise ValueError(
                 "Constructor object must be created from a JSON entry with type='constructor'"
             )
         if "name" in method_entry:
             raise ValueError("Constructor's JSON entry cannot have a `name`")
-        if "outputs" in method_entry and method_entry["outputs"]:
+        if method_entry.get("outputs"):
             raise ValueError("Constructor's JSON entry cannot have non-empty `outputs`")
         if method_entry["stateMutability"] not in ("nonpayable", "payable"):
             raise ValueError(
                 "Constructor's JSON entry state mutability must be `nonpayable` or `payable`"
             )
         inputs = dispatch_types(method_entry.get("inputs", []))
         payable = method_entry["stateMutability"] == "payable"
         return cls(inputs, payable=payable)
 
-    def __init__(self, inputs: Union[Mapping[str, Type], Sequence[Type]], payable: bool = False):
+    def __init__(self, inputs: Mapping[str, Type] | Sequence[Type], *, payable: bool = False):
         self.inputs = Signature(inputs)
         self.payable = payable
 
     def __call__(self, *args: Any, **kwargs: Any) -> "ConstructorCall":
-        """
-        Returns an encoded call with given arguments.
-        """
+        """Returns an encoded call with given arguments."""
         input_bytes = self.inputs.encode(*args, **kwargs)
         return ConstructorCall(input_bytes)
 
     def __str__(self) -> str:
         return f"constructor{self.inputs} " + ("payable" if self.payable else "nonpayable")
 
 
 class Mutability(Enum):
-    """
-    Possible states of a contract's method mutability.
-    """
+    """Possible states of a contract's method mutability."""
 
     PURE = "pure"
     """Solidity's ``pure`` (does not read or write the contract state)."""
     VIEW = "view"
     """Solidity's ``view`` (may read the contract state)."""
     NONPAYABLE = "nonpayable"
     """Solidity's ``nonpayable`` (may write the contract state)."""
@@ -300,20 +276,20 @@
 
     @property
     def payable(self) -> bool:
         return self == Mutability.PAYABLE
 
     @property
     def mutating(self) -> bool:
-        return self == Mutability.PAYABLE or self == Mutability.NONPAYABLE
+        return self in {Mutability.PAYABLE, Mutability.NONPAYABLE}
 
 
 class Method:
     """
-    A non-mutating contract method.
+    A contract method.
 
     .. note::
 
        If the name of a parameter (input or output) given to the constructor
        matches a Python keyword, ``_`` will be appended to it.
     """
 
@@ -323,43 +299,41 @@
     payable: bool
     """Whether this method is marked as payable."""
 
     mutating: bool
     """Whether this method may mutate the contract state."""
 
     @classmethod
-    def from_json(cls, method_entry: Dict[str, Any]) -> "Method":
-        """
-        Creates this object from a JSON ABI method entry.
-        """
+    def from_json(cls, method_entry: dict[str, Any]) -> "Method":
+        """Creates this object from a JSON ABI method entry."""
         if method_entry["type"] != "function":
             raise ValueError("Method object must be created from a JSON entry with type='function'")
 
         name = method_entry["name"]
         inputs = dispatch_types(method_entry["inputs"])
 
         mutability = Mutability.from_json(method_entry["stateMutability"])
 
         # Outputs can be anonymous
-        outputs: Union[Dict[str, Type], List[Type]]
+        outputs: dict[str, Type] | list[Type]
         if "outputs" not in method_entry:
             outputs = []
         elif all(entry["name"] == "" for entry in method_entry["outputs"]):
             outputs = [dispatch_type(entry) for entry in method_entry["outputs"]]
         else:
             outputs = dispatch_types(method_entry["outputs"])
 
         return cls(name=name, inputs=inputs, outputs=outputs, mutability=mutability)
 
     def __init__(
         self,
         name: str,
         mutability: Mutability,
-        inputs: Union[Mapping[str, Type], Sequence[Type]],
-        outputs: Union[Mapping[str, Type], Sequence[Type], Type, None] = None,
+        inputs: Mapping[str, Type] | Sequence[Type],
+        outputs: None | Mapping[str, Type] | Sequence[Type] | Type = None,
     ):
         self._name = name
         self._inputs = Signature(inputs)
         self._mutability = mutability
         self.payable = mutability.payable
         self.mutating = mutability.mutating
 
@@ -372,125 +346,198 @@
         else:
             self._single_output = False
 
         self.outputs = Signature(outputs)
 
     @property
     def name(self) -> str:
+        """The name of this method."""
         return self._name
 
     @property
     def inputs(self) -> Signature:
+        """The input signature of this method."""
         return self._inputs
 
+    def bind(self, *args: Any, **kwargs: Any) -> BoundArguments:
+        return self._inputs.bind(*args, **kwargs)
+
     def __call__(self, *args: Any, **kwargs: Any) -> "MethodCall":
-        """
-        Returns an encoded call with given arguments.
-        """
-        return MethodCall(self._encode_call(*args, **kwargs))
+        """Returns an encoded call with given arguments."""
+        bound_args = self.bind(*args, **kwargs)
+        return self.call_bound(bound_args)
+
+    def call_bound(self, bound_args: BoundArguments) -> "MethodCall":
+        input_bytes = self.inputs.encode_bound(bound_args)
+        encoded = self.selector + input_bytes
+        return MethodCall(self, encoded)
 
     @cached_property
     def selector(self) -> bytes:
-        """
-        Method's selector.
-        """
-        return keccak(self.name.encode() + self.inputs.canonical_form.encode())[:4]
-
-    def _encode_call(self, *args: Any, **kwargs: Any) -> bytes:
-        input_bytes = self.inputs.encode(*args, **kwargs)
-        return self.selector + input_bytes
+        """Method's selector."""
+        return keccak(self.name.encode() + self.inputs.canonical_form.encode())[:SELECTOR_LENGTH]
 
     def decode_output(self, output_bytes: bytes) -> Any:
-        """
-        Decodes the output from ABI-packed bytes.
-        """
+        """Decodes the output from ABI-packed bytes."""
         results = self.outputs.decode_into_tuple(output_bytes)
         if self._single_output:
             results = results[0]
         return results
 
+    def with_method(self, method: "Method") -> "MultiMethod":
+        return MultiMethod(self, method)
+
     def __str__(self) -> str:
-        if self.outputs.empty:
-            returns = ""
-        else:
-            returns = f" returns {self.outputs}"
+        returns = "" if self.outputs.empty else f" returns {self.outputs}"
         return f"function {self.name}{self.inputs} {self._mutability.value}{returns}"
 
 
+class MultiMethod:
+    """
+    An overloaded contract method, containing several :py:class:`Method` objects with the same name
+    but different input signatures.
+    """
+
+    def __init__(self, *methods: Method):
+        if len(methods) == 0:
+            raise ValueError("`methods` cannot be empty")
+        first_method = methods[0]
+        self._methods = {first_method.inputs.canonical_form: first_method}
+        self._name = first_method.name
+
+        for method in methods[1:]:
+            self._add_method(method)
+
+    def __getitem__(self, args: str) -> Method:
+        """
+        Returns the :py:class:`Method` with the given canonical form of an input signature
+        (corresponding to :py:attr:`Signature.canonical_form`).
+        """
+        return self._methods[args]
+
+    @property
+    def name(self) -> str:
+        """The name of this method."""
+        return self._name
+
+    @property
+    def methods(self) -> dict[str, Method]:
+        """All the overloaded methods, indexed by the canonical form of their input signatures."""
+        return self._methods
+
+    def _add_method(self, method: Method) -> None:
+        if method.name != self.name:
+            raise ValueError("All overloaded methods must have the same name")
+        if method.inputs.canonical_form in self._methods:
+            raise ValueError(
+                f"A method {self.name}{method.inputs.canonical_form} "
+                "is already registered in this MultiMethod"
+            )
+        self._methods[method.inputs.canonical_form] = method
+
+    def with_method(self, method: Method) -> "MultiMethod":
+        """Returns a new ``MultiMethod`` with the given method included."""
+        new_mm = MultiMethod(*self._methods.values())
+        new_mm._add_method(method)  # noqa: SLF001
+        return new_mm
+
+    def __call__(self, *args: Any, **kwds: Any) -> "MethodCall":
+        """Returns an encoded call with given arguments."""
+        for method in self._methods.values():
+            try:
+                bound_args = method.bind(*args, **kwds)
+            except TypeError:
+                # If it's a non-overloaded method, we do not want to complicate things
+                if len(self._methods) == 1:
+                    raise
+
+                continue
+
+            return method.call_bound(bound_args)
+
+        raise TypeError("Could not find a suitable overloaded method for the given arguments")
+
+    def __str__(self) -> str:
+        return "; ".join(str(method) for method in self._methods.values())
+
+
 class Event:
     """
     A contract event.
 
     .. note::
 
        If the name of a field given to the constructor matches a Python keyword,
        ``_`` will be appended to it.
     """
 
     @classmethod
-    def from_json(cls, event_entry: Dict[str, Any]) -> "Event":
-        """
-        Creates this object from a JSON ABI method entry.
-        """
+    def from_json(cls, event_entry: dict[str, Any]) -> "Event":
+        """Creates this object from a JSON ABI method entry."""
         if event_entry["type"] != "event":
             raise ValueError("Event object must be created from a JSON entry with type='event'")
 
         name = event_entry["name"]
         fields = dispatch_types(event_entry["inputs"])
+        if isinstance(fields, list):
+            raise TypeError("Event fields must be named")
+
         indexed = {input_["name"] for input_ in event_entry["inputs"] if input_["indexed"]}
 
         return cls(name=name, fields=fields, indexed=indexed, anonymous=event_entry["anonymous"])
 
     def __init__(
         self,
         name: str,
         fields: Mapping[str, Type],
         indexed: AbstractSet[str],
+        *,
         anonymous: bool = False,
     ):
-        if anonymous and len(indexed) > 4:
-            raise ValueError("Anonymous events can have at most 4 indexed fields")
-        if not anonymous and len(indexed) > 3:
-            raise ValueError("Non-anonymous events can have at most 3 indexed fields")
+        if anonymous and len(indexed) > ANONYMOUS_EVENT_INDEXED_FIELDS:
+            raise ValueError(
+                f"Anonymous events can have at most {ANONYMOUS_EVENT_INDEXED_FIELDS} indexed fields"
+            )
+        if not anonymous and len(indexed) > EVENT_INDEXED_FIELDS:
+            raise ValueError(
+                f"Non-anonymous events can have at most {EVENT_INDEXED_FIELDS} indexed fields"
+            )
 
         self.name = name
         self.indexed = indexed
         self.fields = EventSignature(fields, indexed)
         self.anonymous = anonymous
 
     @cached_property
     def _topic(self) -> LogTopic:
-        """
-        The topic representing this event's signature.
-        """
+        """The topic representing this event's signature."""
         return LogTopic(keccak(self.name.encode() + self.fields.canonical_form.encode()))
 
     def __call__(self, *args: Any, **kwargs: Any) -> "EventFilter":
         """
         Creates an event filter from provided values for indexed parameters.
         Some arguments can be omitted, which will mean that the filter
         will match events with any value of that parameter.
         :py:class:`Either` can be used to denote an OR operation and match
         either of several values of a parameter.
         """
-
         encoded_topics = self.fields.encode_to_topics(*args, **kwargs)
 
-        log_topics: List[Optional[Tuple[LogTopic, ...]]] = []
+        log_topics: list[None | tuple[LogTopic, ...]] = []
         if not self.anonymous:
             log_topics.append((self._topic,))
         for topic in encoded_topics:
             if topic is None:
                 log_topics.append(None)
             else:
                 log_topics.append(tuple(LogTopic(elem) for elem in topic))
 
         return EventFilter(tuple(log_topics))
 
-    def decode_log_entry(self, log_entry: LogEntry) -> Dict[str, Any]:
+    def decode_log_entry(self, log_entry: LogEntry) -> dict[str, Any]:
         """
         Decodes the event fields from the given log entry.
         Fields that cannot be decoded (indexed reference types,
         which are hashed before saving them to the log) are set to ``None``.
         """
         topics = log_entry.topics
         if not self.anonymous:
@@ -501,184 +548,164 @@
         return self.fields.decode_log_entry([bytes(topic) for topic in topics], log_entry.data)
 
     def __str__(self) -> str:
         return f"event {self.name}{self.fields}" + (" anonymous" if self.anonymous else "")
 
 
 class EventFilter:
-    """
-    A filter for events coming from any contract address.
-    """
+    """A filter for events coming from any contract address."""
 
-    topics: Tuple[Optional[Tuple[LogTopic, ...]], ...]
+    topics: tuple[None | tuple[LogTopic, ...], ...]
 
-    def __init__(self, topics: Tuple[Optional[Tuple[LogTopic, ...]], ...]):
+    def __init__(self, topics: tuple[None | tuple[LogTopic, ...], ...]):
         self.topics = topics
 
 
 class Error:
-    """
-    A custom contract error.
-    """
+    """A custom contract error."""
 
     @classmethod
-    def from_json(cls, error_entry: Dict[str, Any]) -> "Error":
-        """
-        Creates this object from a JSON ABI method entry.
-        """
+    def from_json(cls, error_entry: dict[str, Any]) -> "Error":
+        """Creates this object from a JSON ABI method entry."""
         if error_entry["type"] != "error":
             raise ValueError("Error object must be created from a JSON entry with type='error'")
 
         name = error_entry["name"]
         fields = dispatch_types(error_entry["inputs"])
+        if isinstance(fields, list):
+            raise TypeError("Error fields must be named")
 
         return cls(name=name, fields=fields)
 
     def __init__(
         self,
         name: str,
         fields: Mapping[str, Type],
     ):
         self.name = name
         self.fields = Signature(fields)
 
     @cached_property
     def selector(self) -> bytes:
-        """
-        Error's selector.
-        """
-        return keccak(self.name.encode() + self.fields.canonical_form.encode())[:4]
+        """Error's selector."""
+        return keccak(self.name.encode() + self.fields.canonical_form.encode())[:SELECTOR_LENGTH]
 
-    def decode_fields(self, data_bytes: bytes) -> Dict[str, Any]:
-        """
-        Decodes the error fields from the given packed data.
-        """
+    def decode_fields(self, data_bytes: bytes) -> dict[str, Any]:
+        """Decodes the error fields from the given packed data."""
         return self.fields.decode_into_dict(data_bytes)
 
     def __str__(self) -> str:
         return f"error {self.name}{self.fields}"
 
 
 class Fallback:
-    """
-    A fallback method.
-    """
+    """A fallback method."""
 
     payable: bool
     """Whether this method is marked as payable"""
 
     @classmethod
-    def from_json(cls, method_entry: Dict[str, Any]) -> "Fallback":
-        """
-        Creates this object from a JSON ABI method entry.
-        """
+    def from_json(cls, method_entry: dict[str, Any]) -> "Fallback":
+        """Creates this object from a JSON ABI method entry."""
         if method_entry["type"] != "fallback":
             raise ValueError(
                 "Fallback object must be created from a JSON entry with type='fallback'"
             )
         if method_entry["stateMutability"] not in ("nonpayable", "payable"):
             raise ValueError(
                 "Fallback method's JSON entry state mutability must be `nonpayable` or `payable`"
             )
         payable = method_entry["stateMutability"] == "payable"
-        return cls(payable)
+        return cls(payable=payable)
 
-    def __init__(self, payable: bool = False):
+    def __init__(self, *, payable: bool = False):
         self.payable = payable
 
     def __str__(self) -> str:
         return "fallback() " + ("payable" if self.payable else "nonpayable")
 
 
 class Receive:
-    """
-    A receive method.
-    """
+    """A receive method."""
 
     payable: bool
     """Whether this method is marked as payable"""
 
     @classmethod
-    def from_json(cls, method_entry: Dict[str, Any]) -> "Receive":
-        """
-        Creates this object from a JSON ABI method entry.
-        """
+    def from_json(cls, method_entry: dict[str, Any]) -> "Receive":
+        """Creates this object from a JSON ABI method entry."""
         if method_entry["type"] != "receive":
             raise ValueError(
                 "Receive object must be created from a JSON entry with type='fallback'"
             )
         if method_entry["stateMutability"] not in ("nonpayable", "payable"):
             raise ValueError(
                 "Receive method's JSON entry state mutability must be `nonpayable` or `payable`"
             )
         payable = method_entry["stateMutability"] == "payable"
-        return cls(payable)
+        return cls(payable=payable)
 
-    def __init__(self, payable: bool = False):
+    def __init__(self, *, payable: bool = False):
         self.payable = payable
 
     def __str__(self) -> str:
         return "receive() " + ("payable" if self.payable else "nonpayable")
 
 
 class ConstructorCall:
-    """
-    A call to the contract's constructor.
-    """
+    """A call to the contract's constructor."""
 
     input_bytes: bytes
     """Encoded call arguments."""
 
     def __init__(self, input_bytes: bytes):
         self.input_bytes = input_bytes
 
 
 class MethodCall:
-    """
-    A call to a contract's regular method.
-    """
+    """A call to a contract's regular method."""
 
     data_bytes: bytes
     """Encoded call arguments with the selector."""
 
-    def __init__(self, data_bytes: bytes):
+    method: Method
+    """The method object that encoded this call."""
+
+    def __init__(self, method: Method, data_bytes: bytes):
+        self.method = method
         self.data_bytes = data_bytes
 
 
 # This is force-documented as :py:class in ``api.rst``
 # because Sphinx cannot resolve typevars correctly.
 # See https://github.com/sphinx-doc/sphinx/issues/9705
 MethodType = TypeVar("MethodType")
 
 
 class Methods(Generic[MethodType]):
     """
-    Bases: ``Generic`` [``MethodType``]
+    Bases: ``Generic`` [``MethodType``].
 
     A holder for named methods which can be accessed as attributes,
     or iterated over.
     """
 
     # :show-inheritance: is turned off in ``api.rst``, and we are documenting the base manually
     # (although without hyperlinking which I cannot get to work).
     # See https://github.com/sphinx-doc/sphinx/issues/9705
 
     def __init__(self, methods_dict: Mapping[str, MethodType]):
         self._methods_dict = methods_dict
 
     def __getattr__(self, method_name: str) -> MethodType:
-        """
-        Returns the method by name.
-        """
+        """Returns the method by name."""
         return self._methods_dict[method_name]
 
     def __iter__(self) -> Iterator[MethodType]:
-        """
-        Returns the iterator over all methods.
-        """
+        """Returns the iterator over all methods."""
         return iter(self._methods_dict.values())
 
 
 PANIC_ERROR = Error("Panic", dict(code=abi.uint(256)))
 
 
 LEGACY_ERROR = Error("Error", dict(message=abi.string))
@@ -694,54 +721,51 @@
 
     Contract methods are grouped by type and are accessible via the attributes below.
     """
 
     constructor: Constructor
     """Contract's constructor."""
 
-    fallback: Optional[Fallback]
+    fallback: None | Fallback
     """Contract's fallback method."""
 
-    receive: Optional[Receive]
+    receive: None | Receive
     """Contract's receive method."""
 
-    method: Methods[Method]
+    method: Methods[Method | MultiMethod]
     """Contract's regular methods."""
 
     event: Methods[Event]
     """Contract's events."""
 
     error: Methods[Error]
     """Contract's errors."""
 
     @classmethod
-    def from_json(cls, json_abi: List[Dict[str, JSON]]) -> "ContractABI":
-        """
-        Creates this object from a JSON ABI (e.g. generated by a Solidity compiler).
-        """
+    def from_json(cls, json_abi: list[dict[str, JSON]]) -> "ContractABI":  # noqa: C901, PLR0912
+        """Creates this object from a JSON ABI (e.g. generated by a Solidity compiler)."""
         constructor = None
         fallback = None
         receive = None
-        methods = {}
+        methods: dict[Any, Method | MultiMethod] = {}
         events = {}
         errors = {}
 
         for entry in json_abi:
             if entry["type"] == "constructor":
                 if constructor:
                     raise ValueError("JSON ABI contains more than one constructor declarations")
                 constructor = Constructor.from_json(entry)
 
             elif entry["type"] == "function":
+                method = Method.from_json(entry)
                 if entry["name"] in methods:
-                    # TODO: add support for overloaded methods
-                    raise ValueError(
-                        f"JSON ABI contains more than one declarations of `{entry['name']}`"
-                    )
-                methods[entry["name"]] = Method.from_json(entry)
+                    methods[entry["name"]] = methods[entry["name"]].with_method(method)
+                else:
+                    methods[entry["name"]] = method
 
             elif entry["type"] == "fallback":
                 if fallback:
                     raise ValueError("JSON ABI contains more than one fallback declarations")
                 fallback = Fallback.from_json(entry)
 
             elif entry["type"] == "receive":
@@ -773,20 +797,20 @@
             methods=methods.values(),
             events=events.values(),
             errors=errors.values(),
         )
 
     def __init__(
         self,
-        constructor: Optional[Constructor] = None,
-        fallback: Optional[Fallback] = None,
-        receive: Optional[Receive] = None,
-        methods: Optional[Iterable[Method]] = None,
-        events: Optional[Iterable[Event]] = None,
-        errors: Optional[Iterable[Error]] = None,
+        constructor: None | Constructor = None,
+        fallback: None | Fallback = None,
+        receive: None | Receive = None,
+        methods: None | Iterable[Method | MultiMethod] = None,
+        events: None | Iterable[Event] = None,
+        errors: None | Iterable[Error] = None,
     ):
         if constructor is None:
             constructor = Constructor(inputs=[])
 
         self.fallback = fallback
         self.receive = receive
         self.constructor = constructor
@@ -794,35 +818,45 @@
         self.event = Methods({event.name: event for event in (events or [])})
         self.error = Methods({error.name: error for error in (errors or [])})
 
         self._error_by_selector = {
             error.selector: error for error in chain([PANIC_ERROR, LEGACY_ERROR], self.error)
         }
 
-    def resolve_error(self, error_data: bytes) -> Tuple[Error, Dict[str, Any]]:
+    def resolve_error(self, error_data: bytes) -> tuple[Error, dict[str, Any]]:
         """
         Given the packed error data, attempts to find the error in the ABI
         and decode the data into its fields.
         """
-        if len(error_data) < 4:
+        if len(error_data) < SELECTOR_LENGTH:
             raise ValueError("Error data too short to contain a selector")
 
-        selector, data = error_data[:4], error_data[4:]
+        selector, data = error_data[:SELECTOR_LENGTH], error_data[SELECTOR_LENGTH:]
 
         if selector in self._error_by_selector:
             error = self._error_by_selector[selector]
             decoded = error.decode_fields(data)
             return error, decoded
 
         raise UnknownError(f"Could not find an error with selector {selector.hex()} in the ABI")
 
     def __str__(self) -> str:
-        all_methods: Iterable[Union[Constructor, Fallback, Receive, Method, Event, Error]] = chain(
+        all_methods: Iterable[
+            Constructor | Fallback | Receive | Method | MultiMethod | Event | Error
+        ] = chain(
             [self.constructor] if self.constructor else [],
             [self.fallback] if self.fallback else [],
             [self.receive] if self.receive else [],
             self.method,
             self.event,
             self.error,
         )
-        method_list = ["    " + str(method) for method in all_methods]
+
+        indent = "    "
+
+        def to_str(item: Any) -> str:
+            if isinstance(item, MultiMethod):
+                return ("\n" + indent).join(str(method) for method in item.methods.values())
+            return str(item)
+
+        method_list = [indent + to_str(method) for method in all_methods]
         return "{\n" + "\n".join(method_list) + "\n}"
```

### Comparing `pons-0.7.0/pons/_fallback_provider.py` & `pons-0.8.0/pons/_fallback_provider.py`

 * *Files 17% similar despite different names*

```diff
@@ -1,21 +1,21 @@
 from abc import ABC, abstractmethod
-from contextlib import asynccontextmanager, AsyncExitStack
-from typing import Any, AsyncIterator, Optional, Iterable, List, Tuple, Union
+from collections.abc import AsyncIterator, Iterable
+from contextlib import AsyncExitStack, asynccontextmanager
 
-from ._provider import Provider, ProviderSession, JSON, RPCError, UnexpectedResponse
+from ethereum_rpc import RPCError
+
+from ._provider import JSON, InvalidResponse, Provider, ProviderSession
 
 
 class FallbackStrategy(ABC):
-    """
-    An abstract class defining a fallback strategy for multiple providers.
-    """
+    """An abstract class defining a fallback strategy for multiple providers."""
 
     @abstractmethod
-    def get_provider_order(self) -> List[int]:
+    def get_provider_order(self) -> list[int]:
         """
         Returns the suggested order of providers to query, based on the accumulated data.
         This method is called once on every high-level request to the provider.
         """
 
 
 class FallbackStrategyFactory(ABC):
@@ -23,26 +23,24 @@
     An abstract class defining a fallback strategy factory for multiple providers.
     This will be called in ``FallbackProvider`` to create an actual strategy object
     (which may be mutated).
     """
 
     @abstractmethod
     def make_strategy(self, num_providers: int) -> FallbackStrategy:
-        """
-        Returns a strategy object.
-        """
+        """Returns a strategy object."""
 
 
 class CycleFallbackStrategy(FallbackStrategy):
-    def __init__(self, weights: List[int]):
+    def __init__(self, weights: list[int]):
         self._providers = list(range(len(weights)))
         self._weights = weights
         self._counter = 0
 
-    def get_provider_order(self) -> List[int]:
+    def get_provider_order(self) -> list[int]:
         if self._counter == self._weights[0]:
             self._counter = 0
             self._providers = self._providers[1:] + [self._providers[0]]
             self._weights = self._weights[1:] + [self._weights[0]]
 
         self._counter += 1
         return list(self._providers)
@@ -53,26 +51,23 @@
     Creates a strategy where the providers are cycled such that the number of times
     a given provider is first in the priority list is equal
     to the corresponding entry in ``weights``
     (the length of which should match the number of providers).
     If ``weights`` is not given, a list of ``1`` will be used.
     """
 
-    def __init__(self, weights: Optional[Iterable[int]] = None):
-        self._weights: Optional[List[int]]
+    def __init__(self, weights: None | Iterable[int] = None):
+        self._weights: None | list[int]
         if weights:
             self._weights = list(weights)
         else:
             self._weights = None
 
     def make_strategy(self, num_providers: int) -> CycleFallbackStrategy:
-        if not self._weights:
-            weights = [1] * num_providers
-        else:
-            weights = self._weights
+        weights = self._weights or [1] * num_providers
 
         if len(weights) != num_providers:
             raise ValueError(
                 f"Length of the weights ({len(weights)}) "
                 f"inconsistent with the number of providers ({num_providers})"
             )
 
@@ -84,15 +79,15 @@
     Creates a strategy where the providers are queried in the order
     they were given to ``FallbackProvider``, until a successful response is received.
     """
 
     def __init__(self, num_providers: int):
         self._providers = list(range(num_providers))
 
-    def get_provider_order(self) -> List[int]:
+    def get_provider_order(self) -> list[int]:
         return self._providers
 
 
 class PriorityFallback(FallbackStrategyFactory):
     def make_strategy(self, num_providers: int) -> PriorityFallbackStrategy:
         return PriorityFallbackStrategy(num_providers)
 
@@ -110,63 +105,77 @@
     If all requests finished with an error, the most informative error is raised.
     """
 
     def __init__(
         self,
         providers: Iterable[Provider],
         strategy: FallbackStrategyFactory = PriorityFallback(),
+        *,
         same_provider: bool = False,
     ):
         self._providers = list(providers)
         self._strategy = strategy.make_strategy(len(self._providers))
         self._same_provider = same_provider
 
     @asynccontextmanager
     async def session(self) -> AsyncIterator["ProviderSession"]:
         async with AsyncExitStack() as stack:
-            sessions = []
-            for provider in self._providers:
-                sessions.append(await stack.enter_async_context(provider.session()))
-            yield FallbackProviderSession(sessions, self._strategy, self._same_provider)
+            sessions = [
+                await stack.enter_async_context(provider.session()) for provider in self._providers
+            ]
+            yield FallbackProviderSession(
+                sessions, self._strategy, same_provider=self._same_provider
+            )
 
 
 class FallbackProviderSession(ProviderSession):
     def __init__(
-        self, sessions: List[ProviderSession], strategy: FallbackStrategy, same_provider: bool
+        self, sessions: list[ProviderSession], strategy: FallbackStrategy, *, same_provider: bool
     ):
         self._sessions = sessions
         self._strategy = strategy
         self._same_provider = same_provider
 
-    async def rpc_and_pin(self, method: str, *args: JSON) -> Tuple[JSON, Tuple[int, ...]]:
-        exceptions: List[Exception] = []
+    async def rpc_and_pin(self, method: str, *args: JSON) -> tuple[JSON, tuple[int, ...]]:
+        exceptions: list[Exception] = []
         provider_idxs = self._strategy.get_provider_order()
         for provider_idx in provider_idxs:
             try:
                 result, sub_idx = await self._sessions[provider_idx].rpc_and_pin(method, *args)
-            except Exception as exc:
+            # PERF203: There won't be a lot of providers, and we need to collect errors from each.
+            # BLE001: it's just a middleware, collecting all errors.
+            except Exception as exc:  # noqa: PERF203, BLE001
                 exceptions.append(exc)
             else:
-                return result, (provider_idx,) + sub_idx
+                return result, (provider_idx, *sub_idx)
 
         # Here we may have a list with each element being
-        # `RPCError`, `UnexpectedResponse`, or `Unreachable`.
+        # `RPCError`, `ProtocolError`, `InvalidResponse`, or `Unreachable`.
         # Since the users of `Provider` rely on the error being one of these types,
         # we can only raise one. So we raise the one with the most information.
+        #
+        # RPC errors give the most information, since they usually signify our request was invalid,
+        # so all the providers would respond to it in the same manner.
+        #
+        # `InvalidResponse` means that the library is unable to parse the response for some reason,
+        # probably because of a bug. So it will be the same for all providers.
+        #
+        # The other two, `ProtocolError` and `Unreachable` is exactly why we have the fallback.
+        # It is pretty much expected to happen.
         rpc_errors = [exc for exc in exceptions if isinstance(exc, RPCError)]
         if len(rpc_errors) > 0:
             raise rpc_errors[0]
-        unexpecteds = [exc for exc in exceptions if isinstance(exc, UnexpectedResponse)]
-        if len(unexpecteds) > 0:
-            raise unexpecteds[0]
+        invalid_responses = [exc for exc in exceptions if isinstance(exc, InvalidResponse)]
+        if len(invalid_responses) > 0:
+            raise invalid_responses[0]
         raise exceptions[0]
 
     async def rpc(self, method: str, *args: JSON) -> JSON:
         result, _provider = await self.rpc_and_pin(method, *args)
         return result
 
-    async def rpc_at_pin(self, path: Tuple[int, ...], method: str, *args: JSON) -> JSON:
+    async def rpc_at_pin(self, path: tuple[int, ...], method: str, *args: JSON) -> JSON:
         if self._same_provider:
             return await self.rpc(method, *args)
         if not path or path[0] < 0 or path[0] >= len(self._sessions):
             raise ValueError(f"Invalid provider path: {path}")
         return await self._sessions[path[0]].rpc_at_pin(path[1:], method, *args)
```

### Comparing `pons-0.7.0/pons/_provider.py` & `pons-0.8.0/pons/_provider.py`

 * *Files 22% similar despite different names*

```diff
@@ -1,188 +1,151 @@
 from abc import ABC, abstractmethod
+from collections.abc import AsyncIterator, Mapping
 from contextlib import asynccontextmanager
 from http import HTTPStatus
-from typing import Any, AsyncIterator, Dict, Optional, Union, cast, Iterable, Mapping, Tuple
+from json import JSONDecodeError
+from typing import cast
 
 import httpx
+from compages import StructuringError
+from ethereum_rpc import JSON, RPCError, structure
 
 
-# TODO: the doc entry had to be written manually for this type because of Sphinx limitations.
-JSON = Union[bool, int, float, str, None, Iterable["JSON"], Mapping[str, "JSON"]]
+class InvalidResponse(Exception):
+    """Raised when the remote server's response is not of an expected format."""
+
+
+class Unreachable(Exception):
+    """Raised when there is a problem connecting to the provider."""
+
+
+class ProtocolError(Exception):
+    """A protocol-specific error."""
+
+
+class HTTPError(ProtocolError):
+    def __init__(self, status_code: int, message: str):
+        try:
+            status = HTTPStatus(status_code)
+        except ValueError:  # pragma: no cover
+            # How to handle it better? Ideally, `httpx` should have returned a parsed status
+            # in the first place, but, alas, it just gives us an integer.
+            status = HTTPStatus.INTERNAL_SERVER_ERROR
+
+        self.status = status
+        self.message = message
+
+    def __str__(self) -> str:
+        return f"HTTP status {self.status}: {self.message}"
 
 
 class Provider(ABC):
-    """
-    The base class for JSON RPC providers.
-    """
+    """The base class for JSON RPC providers."""
 
     @abstractmethod
     @asynccontextmanager
     async def session(self) -> AsyncIterator["ProviderSession"]:
         """
         Opens a session to the provider
         (allowing the backend to perform multiple operations faster).
         """
-        yield  # type: ignore
-
-
-class UnexpectedResponse(Exception):
-    """
-    Raised when the remote server's response is not of an expected format.
-    """
-
-
-class ResponseDict:
-    """
-    A wrapper for dictionaries allowing as to narrow down KeyErrors
-    resulting from an incorrectly formatted response.
-    """
-
-    def __init__(self, response: Any):
-        if not isinstance(response, dict):
-            raise UnexpectedResponse(
-                f"Expected a dictionary as a response, got {type(response).__name__}"
-            )
-        if not all(isinstance(key, str) for key in response):
-            raise UnexpectedResponse(f"Some keys in the response are not strings: {response}")
-        self._response = cast(Dict[str, JSON], response)
-
-    def __contains__(self, field: str) -> bool:
-        return field in self._response
-
-    def __getitem__(self, field: str) -> JSON:
-        try:
-            contents = self._response[field]
-        except KeyError as exc:
-            raise UnexpectedResponse(
-                f"Expected field `{field}` is missing from the result"
-            ) from exc
-        return contents
+        # mypy does not work with abstract generators correctly.
+        # See https://github.com/python/mypy/issues/5070
+        yield  # type: ignore[misc]
 
 
 class ProviderSession(ABC):
     """
     The base class for provider sessions.
+
+    The methods of this class may raise the following exceptions:
+    - :py:class:`RPCError` signifies an error coming from the backend provider;
+    - :py:class:`Unreachable` if the provider is unreachable;
+    - :py:class:`InvalidResponse` if the response was received but could not be parsed;
+    - :py:class:`ProtocolError` if there was an unrecognized error on the protocol level
+      (e.g. an HTTP status code that is not 200 or 400).
+
+    All other exceptions can be considered implementation bugs.
     """
 
     @abstractmethod
     async def rpc(self, method: str, *args: JSON) -> JSON:
-        """
-        Calls the given RPC method with the already json-ified arguments.
-        """
+        """Calls the given RPC method with the already json-ified arguments."""
         ...
 
-    async def rpc_and_pin(self, method: str, *args: JSON) -> Tuple[JSON, Tuple[int, ...]]:
+    async def rpc_and_pin(self, method: str, *args: JSON) -> tuple[JSON, tuple[int, ...]]:
         """
         Calls the given RPC method and returns the path to the provider it succeded on.
         This method will be typically overriden by multi-provider implementations.
         """
         return await self.rpc(method, *args), ()
 
-    async def rpc_at_pin(self, path: Tuple[int, ...], method: str, *args: JSON) -> JSON:
+    async def rpc_at_pin(self, path: tuple[int, ...], method: str, *args: JSON) -> JSON:
         """
         Calls the given RPC method at the provider by the given path
         (obtained previously from ``rpc_and_pin()``).
         This method will be typically overriden by multi-provider implementations.
         """
         if path != ():
             raise ValueError(f"Unexpected provider path: {path}")
         return await self.rpc(method, *args)
 
-    async def rpc_dict(self, method: str, *args: JSON) -> Optional[ResponseDict]:
-        """
-        Calls the given RPC method expecting to get a dictionary (or ``null``) in response.
-        """
-        result = await self.rpc(method, *args)
-        if result is None:
-            return None
-        return ResponseDict(result)
-
 
 class HTTPProvider(Provider):
-    """
-    A provider for RPC via HTTP(S).
-    """
+    """A provider for RPC via HTTP(S)."""
 
     def __init__(self, url: str):
         self._url = url
 
     @asynccontextmanager
     async def session(self) -> AsyncIterator["HTTPSession"]:
         async with httpx.AsyncClient() as client:
             yield HTTPSession(self._url, client)
 
 
-class RPCError(Exception):
-    """
-    A wrapper for a server error returned either as a proper RPC response,
-    or as an HTTP error code response.
-    """
-
-    @classmethod
-    def from_json(cls, response: JSON) -> "RPCError":
-        error = ResponseDict(response)
-        if "data" in error:
-            data = error["data"]
-            if data is not None and not isinstance(data, str):
-                raise UnexpectedResponse(
-                    f"Error data must be a string or None, got {type(data)} ({data})"
-                )
-        else:
-            data = None
-
-        error_code = error["code"]
-        if isinstance(error_code, str):
-            code = int(error_code)
-        elif isinstance(error_code, int):
-            code = error_code
-        else:
-            raise UnexpectedResponse(
-                "Error code must be an integer (possibly string-encoded), "
-                f"got {type(error_code)} ({error_code})"
-            )
-
-        message = error["message"]
-        if not isinstance(message, str):
-            raise UnexpectedResponse(
-                f"Error message must be a string, got {type(message)} ({message})"
-            )
-
-        return cls(code, message, data)
-
-    def __init__(self, code: int, message: str, data: Optional[str] = None):
-        super().__init__(code, message, data)
-        self.code = code
-        self.message = message
-        self.data = data
-
-
-class Unreachable(Exception):
-    """
-    Raised when there is a problem connecting to the provider.
-    """
-
-
 class HTTPSession(ProviderSession):
     def __init__(self, url: str, http_client: httpx.AsyncClient):
         self._url = url
         self._client = http_client
 
+    def _prepare_request(self, method: str, *args: JSON) -> JSON:
+        return {"jsonrpc": "2.0", "method": method, "params": args, "id": 0}
+
     async def rpc(self, method: str, *args: JSON) -> JSON:
-        json = {"jsonrpc": "2.0", "method": method, "params": args, "id": 0}
+        json = self._prepare_request(method, *args)
         try:
             response = await self._client.post(self._url, json=json)
-        except Exception as exc:
+        except httpx.ConnectError as exc:
             raise Unreachable(str(exc)) from exc
-        if response.status_code != HTTPStatus.OK:
-            raise RPCError(response.status_code, response.content.decode())
 
-        response_json = response.json()
+        status = response.status_code
+
+        try:
+            response_json = response.json()
+        except JSONDecodeError as exc:
+            content = response.content.decode()
+            raise InvalidResponse(
+                f"Expected a JSON response, got HTTP status {status}: {content}"
+            ) from exc
+
         if not isinstance(response_json, Mapping):
-            raise UnexpectedResponse(f"RPC response must be a dictionary, got: {response_json}")
-        # Assuming that the HTTP client knows what it's doing, and gives us a valid JSON dict
+            raise InvalidResponse(f"RPC response must be a dictionary, got: {response_json}")
         response_json = cast(Mapping[str, JSON], response_json)
+
+        # Note that the Eth-side errors (e.g. transaction having been reverted)
+        # will have the HTTP status 200, so we are checking for the "error" field first.
         if "error" in response_json:
-            raise RPCError.from_json(response_json["error"])
-        if "result" not in response_json:
-            raise UnexpectedResponse(f"`result` is not present in the response: {response_json}")
-        return response_json["result"]
+            try:
+                error = structure(RPCError, response_json["error"])
+            except StructuringError as exc:
+                raise InvalidResponse(
+                    f"Failed to parse an error response: {response_json}"
+                ) from exc
+
+            raise error
+
+        if status == HTTPStatus.OK:
+            if "result" in response_json:
+                return response_json["result"]
+            raise InvalidResponse(f"`result` is not present in the response: {response_json}")
+
+        raise HTTPError(status, response.content.decode())
```

### Comparing `pons-0.7.0/pons/abi.py` & `pons-0.8.0/pons/abi.py`

 * *Files 23% similar despite different names*

```diff
@@ -1,26 +1,28 @@
-from typing import Optional
+# This is the whole point of this module.
+# ruff: noqa: A001
 
-from ._abi_types import UInt, Int, Bytes, AddressType, String, Bool, Type, Struct
+"""Aliases for various Solidity types."""
 
+from ._abi_types import AddressType, Bool, Bytes, Int, String, Struct, Type, UInt
 
 _PyInt = int
 
 
 def uint(bits: _PyInt) -> UInt:
     """Returns the ``uint<bits>`` type."""
     return UInt(bits)
 
 
 def int(bits: _PyInt) -> Int:
     """Returns the ``int<bits>`` type."""
     return Int(bits)
 
 
-def bytes(size: Optional[_PyInt] = None) -> Bytes:
+def bytes(size: None | _PyInt = None) -> Bytes:
     """Returns the ``bytes<size>`` type, or ``bytes`` if ``size`` is ``None``."""
     return Bytes(size)
 
 
 def struct(**kwargs: Type) -> Struct:
     """Returns the structure type with given fields."""
     return Struct(kwargs)
```

### Comparing `pons-0.7.0/tests/MockMulticall.sol` & `pons-0.8.0/tests/MockMulticall.sol`

 * *Files identical despite different names*

### Comparing `pons-0.7.0/tests/TestClient.sol` & `pons-0.8.0/tests/TestClient.sol`

 * *Files 11% similar despite different names*

```diff
@@ -1,21 +1,45 @@
 pragma solidity >=0.8.0 <0.9.0;
 
 
+contract EmptyContract {
+    uint256 public state;
+
+    constructor(uint256 _state) {
+        state = _state;
+    }
+}
+
+contract Storage {
+    uint x;
+    mapping(address => uint) y;
+    constructor(uint256 _x, address _y_key, uint256 _y_val) {
+        x = _x;
+        y[_y_key] = _y_val;
+    }
+}
+
 contract BasicContract {
     uint256 public state;
 
     constructor(uint256 _state) {
         state = _state;
     }
 
     function setState(uint256 _x) public {
         state = _x;
     }
 
+    function doubleStateAndCheck(uint256 _x) public {
+        state = state * 2;
+        if (state == _x) {
+            revert("Check succeeded");
+        }
+    }
+
     function payableSetState(uint256 _x) public payable {
         state = _x;
     }
 
     function faultySetState(uint256 _x) public {
         if (_x == 0) {
             revert("Wrong value");
@@ -23,14 +47,18 @@
         state = _x;
     }
 
     function getState(uint256 _x) public view returns (uint256) {
         return state + _x;
     }
 
+    function getSender() public view returns (address) {
+        return msg.sender;
+    }
+
     event Deposit(
         address indexed from,
         bytes4 indexed id,
         uint value
     );
 
     event Deposit2(
@@ -43,16 +71,30 @@
     function deposit(bytes4 id) public payable {
         emit Deposit(msg.sender, id, msg.value);
     }
 
     function deposit2(bytes4 id) public payable {
         emit Deposit2(msg.sender, id, msg.value, msg.value + 1);
     }
-}
 
+    event Event1(
+        uint32 indexed value
+    );
+
+    event Event2(
+        uint32 value
+    );
+
+    function emitMultipleEvents(uint32 x) public {
+        emit Event1(x);
+        emit Event1(x + 1);
+        emit Event2(x + 2);
+        emit Event2(x + 3);
+    }
+}
 
 contract PayableConstructor {
     uint256 public state;
 
     constructor(uint256 _state) payable {
         state = _state;
     }
```

### Comparing `pons-0.7.0/tests/TestContract.sol` & `pons-0.8.0/tests/TestContract.sol`

 * *Files identical despite different names*

### Comparing `pons-0.7.0/tests/TestContractFunctionality.sol` & `pons-0.8.0/tests/TestContractFunctionality.sol`

 * *Files 6% similar despite different names*

```diff
@@ -38,14 +38,22 @@
         v1 = _v1;
     }
 
     function getState(uint256 _x) public view returns (uint256) {
         return v1 + _x;
     }
 
+    function overloaded(uint256 _x, uint256 _y) public pure returns (uint256) {
+        return _y + _x;
+    }
+
+    function overloaded(uint256 _x) public view returns (uint256) {
+        return v1 + _x;
+    }
+
     struct Inner {
         uint256 inner1;
         uint256 inner2;
     }
 
     struct Outer {
         Inner inner;
@@ -86,8 +94,10 @@
         bytes2 x = "aa";
         bytes2 y = "bb";
         bytes2[2] memory foo2 = [x, y];
         Foo memory foo = Foo("4567", foo2, bytestring33len1, "\u1234\u1212", inner1);
         ByteInner[2] memory inner_arr = [inner1, inner2];
         emit Complicated("aaaa", bytestring33len2, foo, inner_arr);
     }
+
+    error MyError(address sender);
 }
```

### Comparing `pons-0.7.0/tests/test_abi_types.py` & `pons-0.8.0/tests/test_abi_types.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,20 +1,20 @@
 import os
 
 import pytest
+from ethereum_rpc import Address, keccak
 
-from pons import abi, Address
+from pons import abi
 from pons._abi_types import (
-    type_from_abi_string,
+    ABIDecodingError,
+    decode_args,
     dispatch_type,
     dispatch_types,
-    ABIDecodingError,
     encode_args,
-    decode_args,
-    keccak,
+    type_from_abi_string,
 )
 
 
 def test_uint():
     for val in [0, 255, 10]:
         assert abi.uint(8)._normalize(val) == val
         assert abi.uint(8)._denormalize(val) == val
@@ -33,16 +33,15 @@
         abi.uint(128)._normalize("abc")
     with pytest.raises(
         ValueError, match="`uint128` must correspond to a non-negative integer, got -1"
     ):
         abi.uint(128)._normalize(-1)
     with pytest.raises(
         ValueError,
-        match="`uint128` must correspond to an unsigned integer under 128 bits, got "
-        + str(2**128),
+        match="`uint128` must correspond to an unsigned integer under 128 bits, got " + str(2**128),
     ):
         abi.uint(128)._normalize(2**128)
 
 
 def test_int():
     for val in [0, 127, -128, 10]:
         assert abi.int(8)._normalize(val) == val
@@ -208,22 +207,37 @@
 
 
 def test_dispatch_types():
     entries = [
         dict(name="param2", type="uint8"),
         dict(name="param1", type="uint16[2]"),
     ]
+
+    assert dispatch_types(entries) == dict(param2=abi.uint(8), param1=abi.uint(16)[2])
+
     # Check that the order is preserved, too
     assert list(dispatch_types(entries).items()) == [
         ("param2", abi.uint(8)),
         ("param1", abi.uint(16)[2]),
     ]
 
+    # Note that if all the names are empty, it is treated as a list of positional arguments
+    assert dispatch_types([dict(name="", type="uint8"), dict(name="", type="uint16[2]")]) == [
+        abi.uint(8),
+        abi.uint(16)[2],
+    ]
+
+    # For an empty argument list we choose to resolve it as an empty dictionary, for certainty.
+    assert dispatch_types([]) == {}
+
+    with pytest.raises(ValueError, match="Arguments must be either all named or all unnamed"):
+        dispatch_types([dict(name="foo", type="uint8"), dict(name="", type="uint16[2]")])
+
     with pytest.raises(ValueError, match="All ABI entries must have distinct names"):
-        dispatch_types([dict(name="", type="uint8"), dict(name="", type="uint16[2]")])
+        dispatch_types([dict(name="foo", type="uint8"), dict(name="foo", type="uint16[2]")])
 
 
 def test_making_arrays():
     assert abi.uint(8)[2].canonical_form == "uint8[2]"
     assert abi.uint(8)[...][3][...].canonical_form == "uint8[][3][]"
 
     with pytest.raises(TypeError, match="Invalid array size specifier type: float"):
@@ -247,15 +261,15 @@
     # normalize() loses info on struct field names
     assert struct._normalize(value) == expected_normalized
 
     # denormalize() should recover struct field names
     assert struct._denormalize(expected_normalized) == value
 
 
-def check_topic_encode_decode(tp, val, encoded_val, can_be_decoded=True):
+def check_topic_encode_decode(tp, val, encoded_val, *, can_be_decoded=True):
     assert tp.encode_to_topic(val) == encoded_val
     if can_be_decoded:
         assert tp.decode_from_topic(encoded_val) == val
     else:
         assert tp.decode_from_topic(encoded_val) is None
 
 
@@ -320,25 +334,25 @@
     )
     check_topic_encode_decode(tp, val, encoded_val, can_be_decoded=False)
 
 
 def test_encode_decode_args():
     args = ("some string", b"bytestring", 1234)
     types = [abi.string, abi.bytes(), abi.uint(256)]
-    encoded = encode_args(*zip(types, args))
+    encoded = encode_args(*zip(types, args, strict=True))
     assert decode_args(types, encoded) == args
 
     # empty types/args list
     assert encode_args() == b""
 
 
 def test_decoding_error():
     types = [abi.uint(256), abi.uint(256)]
     encoded_bytes = b"\x00" * 31 + b"\x01"  # Only one uint256
 
     expected_message = (
         r"Could not decode the return value with the expected signature \(uint256,uint256\): "
-        r"Tried to read 32 bytes.  Only got 0 bytes"
+        r"Tried to read 32 bytes, only got 0 bytes"
     )
 
     with pytest.raises(ABIDecodingError, match=expected_message):
         decode_args(types, encoded_bytes)
```

### Comparing `pons-0.7.0/tests/test_contract.py` & `pons-0.8.0/tests/test_contract.py`

 * *Files 11% similar despite different names*

```diff
@@ -1,39 +1,34 @@
-from collections import namedtuple
 from pathlib import Path
+from typing import NamedTuple
 
 import pytest
+from ethereum_rpc import Address, LogTopic, keccak
 
 from pons import (
-    abi,
-    Address,
     Constructor,
-    Method,
+    Event,
     Fallback,
+    Method,
     Receive,
-    Event,
+    abi,
+    compile_contract_file,
 )
-from pons._abi_types import keccak, encode_args
-from pons._contract import DeployedContract, BoundMethod
-from pons._entities import LogTopic
-
-from .compile import compile_file
+from pons._abi_types import encode_args
+from pons._contract import BoundMethod, DeployedContract
 
 
 @pytest.fixture
 def compiled_contracts():
     path = Path(__file__).resolve().parent / "TestContract.sol"
-    yield compile_file(path)
+    return compile_contract_file(path)
 
 
 def test_abi_declaration(compiled_contracts):
-    """
-    Checks that the compiler output is parsed correctly.
-    """
-
+    """Checks that the compiler output is parsed correctly."""
     compiled_contract = compiled_contracts["JsonAbiTest"]
 
     cabi = compiled_contract.abi
 
     assert isinstance(cabi.constructor, Constructor)
     assert str(cabi.constructor.inputs) == "(uint256 _v1, uint256 _v2)"
     assert cabi.constructor.payable
@@ -68,18 +63,15 @@
     assert isinstance(cabi.event.Foo, Event)
     assert str(cabi.event.Foo.fields) == "(uint256 indexed x, bytes indexed y, bytes4 u, bytes v)"
     assert cabi.event.Foo.anonymous
     assert cabi.event.Foo.indexed == {"x", "y"}
 
 
 def test_api_binding(compiled_contracts):
-    """
-    Checks that the methods are bound correctly on deploy.
-    """
-
+    """Checks that the methods are bound correctly on deploy."""
     compiled_contract = compiled_contracts["JsonAbiTest"]
 
     address = Address(b"\xab" * 20)
     deployed_contract = DeployedContract(compiled_contract.abi, address)
 
     assert deployed_contract.address == address
     assert deployed_contract.abi == compiled_contract.abi
@@ -113,21 +105,25 @@
     assert event_filter.contract_address == address
     assert event_filter.topics == (
         (LogTopic(abi.uint(256).encode(1)),),
         (LogTopic(keccak(b"1234")),),
     )
 
     # We only need a couple of fields
-    fake_log_entry = namedtuple("fake_log_entry", ["topics", "data", "address"])
+    class FakeLogEntry(NamedTuple):
+        data: bytes
+        address: Address
+        topics: tuple[LogTopic, ...]
+
     decoded = event_filter.decode_log_entry(
-        fake_log_entry(
+        FakeLogEntry(
             address=address,
             topics=[LogTopic(abi.uint(256).encode(1)), LogTopic(keccak(b"1234"))],
             data=encode_args((abi.bytes(4), b"4567"), (abi.bytes(), b"bytestring")),
         )
     )
     assert decoded == dict(x=1, y=None, u=b"4567", v=b"bytestring")
 
     with pytest.raises(ValueError, match="Log entry originates from a different contract"):
         decoded = event_filter.decode_log_entry(
-            fake_log_entry(address=Address(b"\xba" * 20), topics=[], data=b"")
+            FakeLogEntry(address=Address(b"\xba" * 20), topics=[], data=b"")
         )
```

### Comparing `pons-0.7.0/tests/test_contract_abi.py` & `pons-0.8.0/tests/test_contract_abi.py`

 * *Files 9% similar despite different names*

```diff
@@ -1,34 +1,34 @@
-from collections import namedtuple
 import re
+from typing import NamedTuple
 
 import pytest
+from ethereum_rpc import LogTopic, keccak
 
 from pons import (
-    abi,
     Constructor,
-    Method,
-    Fallback,
-    Receive,
     ContractABI,
-    Event,
-    Error,
     Either,
-    ABIDecodingError,
+    Error,
+    Event,
+    Fallback,
+    Method,
+    MultiMethod,
     Mutability,
+    Receive,
+    abi,
 )
-from pons._abi_types import keccak, encode_args
+from pons._abi_types import encode_args
 from pons._contract_abi import (
-    Signature,
-    EventSignature,
-    PANIC_ERROR,
     LEGACY_ERROR,
+    PANIC_ERROR,
+    EventSignature,
+    Signature,
     UnknownError,
 )
-from pons._entities import LogTopic
 
 
 def test_signature_from_dict():
     sig = Signature(dict(a=abi.uint(8), b=abi.bool))
     assert sig.canonical_form == "(uint8,bool)"
     assert str(sig) == "(uint8 a, bool b)"
     assert sig.decode_into_tuple(sig.encode(1, True)) == (1, True)
@@ -252,14 +252,87 @@
         ],
     )
 
     with pytest.raises(ValueError, match="Unknown mutability identifier: invalid"):
         Method.from_json(json)
 
 
+def test_multi_method():
+    method1 = Method(
+        name="someMethod",
+        mutability=Mutability.VIEW,
+        inputs=dict(a=abi.uint(8), b=abi.bool),
+        outputs=abi.uint(8),
+    )
+    method2 = Method(
+        name="someMethod",
+        mutability=Mutability.VIEW,
+        inputs=dict(a=abi.uint(8)),
+        outputs=abi.uint(8),
+    )
+
+    multi_method = MultiMethod(method1, method2)
+    assert multi_method["(uint8,bool)"] == method1
+    assert multi_method["(uint8)"] == method2
+
+    assert str(multi_method) == (
+        "function someMethod(uint8 a, bool b) view returns (uint8); "
+        "function someMethod(uint8 a) view returns (uint8)"
+    )
+
+    # Create sequentially
+    multi_method = MultiMethod(method1).with_method(method2)
+    assert multi_method["(uint8,bool)"] == method1
+    assert multi_method["(uint8)"] == method2
+
+    # Call the first method
+    call = multi_method(1, b=True)
+    assert call.method == method1
+
+    # Call the second method
+    call = multi_method(a=1)
+    assert call.method == method2
+
+    # Call with arguments not matching any of the methods
+    with pytest.raises(
+        TypeError, match="Could not find a suitable overloaded method for the given arguments"
+    ):
+        multi_method(1, True, 2)
+
+    # If the multi-method only contains one method, raise the binding error right away
+    multi_method = MultiMethod(method1)
+    with pytest.raises(TypeError, match="missing a required argument: 'b'"):
+        multi_method(1)
+
+
+def test_multi_method_errors():
+    with pytest.raises(ValueError, match="`methods` cannot be empty"):
+        MultiMethod()
+
+    method = Method(
+        name="someMethod",
+        mutability=Mutability.VIEW,
+        inputs=dict(a=abi.uint(8), b=abi.bool),
+        outputs=abi.uint(8),
+    )
+    method_with_different_name = Method(
+        name="someMethod2",
+        mutability=Mutability.VIEW,
+        inputs=dict(a=abi.uint(8)),
+        outputs=abi.uint(8),
+    )
+
+    with pytest.raises(ValueError, match="All overloaded methods must have the same name"):
+        MultiMethod(method, method_with_different_name)
+
+    msg = re.escape("A method someMethod(uint8,bool) is already registered in this MultiMethod")
+    with pytest.raises(ValueError, match=msg):
+        MultiMethod(method, method)
+
+
 def test_fallback():
     fallback = Fallback.from_json(dict(type="fallback", stateMutability="payable"))
     assert fallback.payable
 
 
 def test_fallback_errors():
     with pytest.raises(
@@ -421,53 +494,86 @@
     assert isinstance(cabi.constructor, Constructor)
     assert isinstance(cabi.fallback, Fallback)
     assert isinstance(cabi.receive, Receive)
     assert isinstance(cabi.method.readMethod, Method)
     assert isinstance(cabi.method.writeMethod, Method)
 
 
+def test_overloaded_methods():
+    json_abi = [
+        dict(
+            type="function",
+            name="readMethod",
+            stateMutability="view",
+            inputs=[
+                dict(type="uint8", name="a"),
+                dict(type="bool", name="b"),
+            ],
+            outputs=[
+                dict(type="uint8", name=""),
+            ],
+        ),
+        dict(
+            type="function",
+            name="readMethod",
+            stateMutability="view",
+            inputs=[
+                dict(type="uint8", name="a"),
+            ],
+            outputs=[
+                dict(type="uint8", name=""),
+            ],
+        ),
+    ]
+
+    cabi = ContractABI.from_json(json_abi)
+    assert str(cabi) == (
+        "{\n"
+        "    constructor() nonpayable\n"
+        "    function readMethod(uint8 a, bool b) view returns (uint8)\n"
+        "    function readMethod(uint8 a) view returns (uint8)\n"
+        "}"
+    )
+
+    assert isinstance(cabi.method.readMethod, MultiMethod)
+
+
 def test_no_constructor():
     cabi = ContractABI()
     assert isinstance(cabi.constructor, Constructor)
     assert cabi.constructor.inputs.canonical_form == "()"
 
 
 def test_contract_abi_errors():
     constructor_abi = dict(type="constructor", stateMutability="payable", inputs=[])
     with pytest.raises(
         ValueError, match="JSON ABI contains more than one constructor declarations"
     ):
-        abi = ContractABI.from_json([constructor_abi, constructor_abi])
-
-    write_abi = dict(type="function", name="someMethod", stateMutability="payable", inputs=[])
-    with pytest.raises(
-        ValueError, match="JSON ABI contains more than one declarations of `someMethod`"
-    ):
-        abi = ContractABI.from_json([write_abi, write_abi])
+        ContractABI.from_json([constructor_abi, constructor_abi])
 
     fallback_abi = dict(type="fallback", stateMutability="payable")
     with pytest.raises(ValueError, match="JSON ABI contains more than one fallback declarations"):
-        abi = ContractABI.from_json([fallback_abi, fallback_abi])
+        ContractABI.from_json([fallback_abi, fallback_abi])
 
     receive_abi = dict(type="receive", stateMutability="payable")
     with pytest.raises(
         ValueError, match="JSON ABI contains more than one receive method declarations"
     ):
-        abi = ContractABI.from_json([receive_abi, receive_abi])
+        ContractABI.from_json([receive_abi, receive_abi])
 
     event_abi = dict(type="event", name="Foo", inputs=[], anonymous=False)
     with pytest.raises(ValueError, match="JSON ABI contains more than one declarations of `Foo`"):
-        abi = ContractABI.from_json([event_abi, event_abi])
+        ContractABI.from_json([event_abi, event_abi])
 
     error_abi = dict(type="error", name="Foo", inputs=[])
     with pytest.raises(ValueError, match="JSON ABI contains more than one declarations of `Foo`"):
-        abi = ContractABI.from_json([error_abi, error_abi])
+        ContractABI.from_json([error_abi, error_abi])
 
     with pytest.raises(ValueError, match="Unknown ABI entry type: foobar"):
-        abi = ContractABI.from_json([dict(type="foobar")])
+        ContractABI.from_json([dict(type="foobar")])
 
 
 def test_event_from_json():
     event = Event.from_json(
         dict(
             anonymous=True,
             inputs=[
@@ -516,34 +622,36 @@
         None,
         (LogTopic(abi.uint(8).encode(1)), LogTopic(abi.uint(8).encode(2))),
     )
 
 
 def test_event_decode():
     # We only need a couple of fields
-    fake_log_entry = namedtuple("fake_log_entry", ["topics", "data"])
+    class FakeLogEntry(NamedTuple):
+        topics: tuple[LogTopic, ...]
+        data: bytes
 
     event = Event("Foo", dict(a=abi.bool, b=abi.uint(8), c=abi.bytes(4), d=abi.bytes()), {"a", "b"})
 
     decoded = event.decode_log_entry(
-        fake_log_entry(
+        FakeLogEntry(
             [
                 LogTopic(keccak(event.name.encode() + event.fields.canonical_form.encode())),
                 LogTopic(abi.bool.encode(True)),
                 LogTopic(abi.uint(8).encode(2)),
             ],
             encode_args((abi.bytes(4), b"1234"), (abi.bytes(), b"bytestring")),
         )
     )
     assert decoded == dict(a=True, b=2, c=b"1234", d=b"bytestring")
 
     # Wrong selector
     with pytest.raises(ValueError, match="This log entry belongs to a different event"):
         decoded = event.decode_log_entry(
-            fake_log_entry(
+            FakeLogEntry(
                 [
                     LogTopic(keccak(b"NotFoo" + event.fields.canonical_form.encode())),
                     LogTopic(abi.bool.encode(True)),
                     LogTopic(abi.uint(8).encode(2)),
                 ],
                 encode_args((abi.bytes(4), b"1234"), (abi.bytes(), b"bytestring")),
             )
@@ -555,15 +663,15 @@
         "Foo",
         dict(a=abi.bool, b=abi.uint(8), c=abi.bytes(4), d=abi.bytes()),
         {"a", "b"},
         anonymous=True,
     )
 
     decoded = event.decode_log_entry(
-        fake_log_entry(
+        FakeLogEntry(
             [LogTopic(abi.bool.encode(True)), LogTopic(abi.uint(8).encode(2))],
             encode_args((abi.bytes(4), b"1234"), (abi.bytes(), b"bytestring")),
         )
     )
     assert decoded == dict(a=True, b=2, c=b"1234", d=b"bytestring")
 
 
@@ -596,14 +704,27 @@
         Event(
             "Foo", dict(a=uint8, b=uint8, c=uint8, d=uint8, e=uint8), indexed={"a", "b", "c", "d"}
         )
 
     # This works
     Event("Foo", dict(a=uint8, b=uint8, c=uint8, d=uint8, e=uint8), indexed={"a", "b", "c"})
 
+    with pytest.raises(TypeError, match="Event fields must be named"):
+        Event.from_json(
+            dict(
+                anonymous=True,
+                inputs=[
+                    dict(indexed=True, internalType="address", name="", type="address"),
+                    dict(indexed=False, internalType="uint8", name="", type="uint8"),
+                ],
+                name="Foo",
+                type="event",
+            )
+        )
+
 
 def test_error_from_json():
     error = Error.from_json(
         dict(
             inputs=[
                 dict(internalType="address", name="from", type="address"),
                 dict(internalType="bytes", name="foo", type="bytes"),
@@ -618,14 +739,26 @@
 
     with pytest.raises(
         ValueError,
         match="Error object must be created from a JSON entry with type='error'",
     ):
         Error.from_json(dict(type="constructor"))
 
+    with pytest.raises(TypeError, match="Error fields must be named"):
+        Error.from_json(
+            dict(
+                inputs=[
+                    dict(internalType="address", name="", type="address"),
+                    dict(internalType="bytes", name="", type="bytes"),
+                ],
+                name="Foo",
+                type="error",
+            )
+        )
+
 
 def test_error_init():
     error = Error(
         "Foo",
         dict(from_=abi.address, foo=abi.bytes(), bar=abi.uint(8)),
     )
     assert error.name == "Foo"
```

### Comparing `pons-0.7.0/tests/test_contract_functionality.py` & `pons-0.8.0/tests/test_contract_functionality.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,28 +1,35 @@
 from pathlib import Path
 
 import pytest
+from ethereum_rpc import Amount
 
-from pons import Amount, ContractABI, abi, Constructor, Method, DeployedContract, Mutability
-
-from .compile import compile_file
+from pons import (
+    Constructor,
+    ContractABI,
+    DeployedContract,
+    EVMVersion,
+    Method,
+    Mutability,
+    abi,
+    compile_contract_file,
+)
 
 
 @pytest.fixture
 def compiled_contracts():
     path = Path(__file__).resolve().parent / "TestContractFunctionality.sol"
-    yield compile_file(path)
+    return compile_contract_file(path, evm_version=EVMVersion.CANCUN)
 
 
 async def test_empty_constructor(session, root_signer, compiled_contracts):
     """
     Checks that an empty constructor is created automatically if none is provided,
     and it can be used to deploy the contract.
     """
-
     compiled_contract = compiled_contracts["NoConstructor"]
 
     deployed_contract = await session.deploy(root_signer, compiled_contract.constructor())
     call = deployed_contract.method.getState(123)
     result = await session.eth_call(call)
     assert result == (1 + 123,)
 
@@ -50,14 +57,28 @@
 
     inner = dict(inner1=1, inner2=2)
     outer = dict(inner=inner, outer1=3)
     result = await session.eth_call(deployed_contract.method.testStructs(inner, outer))
     assert result == (inner, outer)
 
 
+async def test_overloaded_method(session, root_signer, compiled_contracts):
+    compiled_contract = compiled_contracts["Test"]
+
+    # Deploy the contract
+    call = compiled_contract.constructor(12345, 56789)
+    deployed_contract = await session.deploy(root_signer, call)
+
+    result = await session.eth_call(deployed_contract.method.overloaded(123))
+    assert result == (12345 + 123,)
+
+    result = await session.eth_call(deployed_contract.method.overloaded(123, 456))
+    assert result == (456 + 123,)
+
+
 async def test_read_only_mode(session, root_signer, compiled_contracts):
     # Test that a "nonpayable" (that is, mutating) method can still be invoked
     # via `eth_call`, and it will use the current state of the contract
     # in a "copy-on-write" mode, where it will be able to make changes,
     # but they will not be saved.
 
     compiled_contract = compiled_contracts["Test"]
@@ -146,15 +167,15 @@
     inner1 = [b"0123", bytestring33len1]
     inner2 = [b"-123", bytestring33len2]
     foo = [b"4567", [b"aa", b"bb"], bytestring33len1, "\u1234\u1212", inner1]
     event_filter = basic_contract.abi.event.Complicated(
         b"aaaa", bytestring33len2, foo, [inner1, inner2]
     )
 
-    contract = await session.deploy(root_signer, basic_contract.constructor(123, 456))
+    contract = await session.deploy(root_signer, basic_contract.constructor(12345, 56789))
 
     log_filter1 = await session.eth_new_filter(event_filter=event_filter)  # filter by topics
     log_filter2 = await session.eth_new_filter()  # collect everything
     await session.transact(root_signer, contract.method.emitComplicated())
     entries_filtered = await session.eth_get_filter_changes(log_filter1)
     entries_all = await session.eth_get_filter_changes(log_filter2)
```

### Comparing `pons-0.7.0/tests/test_fallback_provider.py` & `pons-0.8.0/tests/test_fallback_provider.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,17 +1,18 @@
-from enum import Enum
-from contextlib import asynccontextmanager
-from typing import Optional, List, AsyncIterator
 import os
+from collections.abc import AsyncIterator
+from contextlib import asynccontextmanager
+from enum import Enum
 
 import pytest
+from ethereum_rpc import JSON, RPCError
 
-from pons import FallbackProvider, FallbackStrategy, CycleFallback, PriorityFallback, Unreachable
-from pons._provider import Provider, ProviderSession, JSON, UnexpectedResponse, RPCError
+from pons import CycleFallback, FallbackProvider, PriorityFallback, Unreachable
 from pons._fallback_provider import PriorityFallbackStrategy
+from pons._provider import InvalidResponse, Provider, ProviderSession
 
 
 def random_request():
     return os.urandom(2).hex()
 
 
 class ProviderState(Enum):
@@ -34,24 +35,23 @@
         yield MockSession(self)
 
 
 class MockSession(ProviderSession):
     def __init__(self, provider: Provider):
         self.provider = provider
 
-    async def rpc(self, method: str, *args: JSON) -> JSON:
+    async def rpc(self, method: str, *_args: JSON) -> JSON:
         self.provider.requests.append(method)
-        if self.provider.state == ProviderState.NORMAL:
-            return "success"
-        elif self.provider.state == ProviderState.UNREACHABLE:
+        if self.provider.state == ProviderState.UNREACHABLE:
             raise Unreachable("")
-        elif self.provider.state == ProviderState.BAD_RESPONSE:
-            raise UnexpectedResponse("")
-        elif self.provider.state == ProviderState.RPC_ERROR:
+        if self.provider.state == ProviderState.BAD_RESPONSE:
+            raise InvalidResponse("")
+        if self.provider.state == ProviderState.RPC_ERROR:
             raise RPCError(-1, "")
+        return "success"
 
 
 async def test_default_fallback():
     providers = [MockProvider() for i in range(3)]
     provider = FallbackProvider(providers)
     assert isinstance(provider._strategy, PriorityFallbackStrategy)
 
@@ -128,29 +128,29 @@
 
     async with provider.session() as session:
         # All are unreachable, an Unreachable is raised
         providers[0].set_state(ProviderState.UNREACHABLE)
         providers[1].set_state(ProviderState.UNREACHABLE)
         providers[2].set_state(ProviderState.UNREACHABLE)
         with pytest.raises(Unreachable):
-            result = await session.rpc(random_request())
+            await session.rpc(random_request())
 
-        # UnexpectedResponse is raised if present
+        # InvalidResponse is raised if present
         providers[0].set_state(ProviderState.UNREACHABLE)
         providers[1].set_state(ProviderState.BAD_RESPONSE)
         providers[2].set_state(ProviderState.UNREACHABLE)
-        with pytest.raises(UnexpectedResponse):
-            result = await session.rpc(random_request())
+        with pytest.raises(InvalidResponse):
+            await session.rpc(random_request())
 
         # RPCError is raised if present
         providers[0].set_state(ProviderState.UNREACHABLE)
         providers[1].set_state(ProviderState.BAD_RESPONSE)
         providers[2].set_state(ProviderState.RPC_ERROR)
         with pytest.raises(RPCError):
-            result = await session.rpc(random_request())
+            await session.rpc(random_request())
 
 
 async def test_nested_providers():
     providers = [MockProvider() for i in range(4)]
     subprovider1 = FallbackProvider([providers[0], providers[1]], PriorityFallback())
     subprovider2 = FallbackProvider(
         [providers[2], providers[3]], PriorityFallback(), same_provider=True
@@ -189,15 +189,15 @@
         assert providers[2].requests[-1] == request
 
         # Since provider 2 and 3 are marked as "same provider",
         # provider 3 can be used instead of the pinned provider 2
         request = random_request()
         providers[3].set_state(ProviderState.NORMAL)
         providers[2].set_state(ProviderState.UNREACHABLE)
-        result = await session.rpc_at_pin(path, request)
+        await session.rpc_at_pin(path, request)
         assert providers[3].requests[-1] == request
 
 
 async def test_invalid_path():
     providers = [MockProvider() for i in range(4)]
     subprovider1 = FallbackProvider([providers[0], providers[1]], PriorityFallback())
     subprovider2 = FallbackProvider(
```

### Comparing `pons-0.7.0/tests/test_multicall.py` & `pons-0.8.0/tests/_test_multicall.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,28 +1,27 @@
 from pathlib import Path
 
 import pytest
 
 from pons import (
-    abi,
     Address,
     Constructor,
-    Method,
     ContractABI,
+    Method,
     Mutability,
+    abi,
+    compile_contract_file,
 )
 from pons._contract import DeployedContract
 
-from .compile import compile_file
-
 
 @pytest.fixture
 def compiled_contracts():
     path = Path(__file__).resolve().parent / "MockMulticall.sol"
-    yield compile_file(path)
+    yield compile_contract_file(path)
 
 
 async def test_multicall(session, root_signer, compiled_contracts):
     mock = compiled_contracts["MockMulticall"]
 
     dmock = await session.deploy(root_signer, mock.constructor())
```

### Comparing `pons-0.7.0/tests/test_provider.py` & `pons-0.8.0/tests/test_provider.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,77 +1,48 @@
 from contextlib import asynccontextmanager
+from http import HTTPStatus
 
-import trio
 import pytest
+import trio
+from ethereum_rpc import Amount
 
-from pons import Client, Amount, HTTPProvider, Unreachable
-from pons._client import ProviderError, BadResponseFormat
-from pons._provider import ResponseDict, UnexpectedResponse, RPCError, Provider, ProviderSession
-
-from .provider_server import ServerHandle
-from . import provider_server  # For monkeypatching purposes
+from pons import (
+    Client,
+    HTTPProvider,
+    HTTPProviderServer,
+    Unreachable,
+    _http_provider_server,  # For monkeypatching purposes
+)
+from pons._client import BadResponseFormat, ProviderError
+from pons._provider import HTTPError, Provider, ProviderSession
 
 
 @pytest.fixture
-async def test_server(nursery, test_provider):
-    handle = ServerHandle(test_provider)
+async def test_server(nursery, local_provider):
+    handle = HTTPProviderServer(local_provider)
     await nursery.start(handle)
     yield handle
     await handle.shutdown()
 
 
 @pytest.fixture
 async def session(test_server):
     client = Client(test_server.http_provider)
     async with client.session() as session:
         yield session
 
 
 async def test_single_value_request(session):
-    assert await session.net_version() == "0"
+    assert await session.net_version() == "1"
 
 
 async def test_dict_request(session, root_signer, another_signer):
     await session.transfer(root_signer, another_signer.address, Amount.ether(10))
 
 
-def test_response_dict():
-    with pytest.raises(
-        UnexpectedResponse, match="Some keys in the response are not strings: {1: 2}"
-    ):
-        ResponseDict({1: 2})
-
-
-def test_rpc_error():
-    with pytest.raises(
-        UnexpectedResponse, match=r"Error data must be a string or None, got <class 'int'> \(1\)"
-    ):
-        RPCError.from_json({"data": 1, "code": 2, "message": "error"})
-
-    error = RPCError.from_json({"code": 2, "message": "error"})
-    assert error.data is None
-
-    error = RPCError.from_json({"code": "2", "message": "error"})
-    assert error.code == 2
-
-    with pytest.raises(
-        UnexpectedResponse,
-        match=(
-            r"Error code must be an integer \(possibly string-encoded\), "
-            r"got <class 'float'> \(1\.0\)"
-        ),
-    ):
-        RPCError.from_json({"code": 1.0, "message": "error"})
-
-    with pytest.raises(
-        UnexpectedResponse, match=r"Error message must be a string, got <class 'int'> \(1\)"
-    ):
-        RPCError.from_json({"code": 2, "message": 1})
-
-
 async def test_dict_request_introspection(session, root_signer, another_signer):
     # This test covers the __contains__ method of ResponseDict.
     # It is invoked when the error response is checked for the "data" field,
     # so we trigger an intentionally bad transaction.
     # A little roundabout, is there a better way?
     with pytest.raises(
         ProviderError,
@@ -79,101 +50,131 @@
     ):
         await session.estimate_transfer(
             root_signer.address, another_signer.address, Amount.ether(1000)
         )
 
 
 async def test_unexpected_response_type(
-    test_provider, session, monkeypatch, root_signer, another_signer
+    local_provider, session, monkeypatch, root_signer, another_signer
 ):
-    monkeypatch.setattr(test_provider, "eth_get_transaction_receipt", lambda tx_hash: "something")
-
     tx_hash = await session.broadcast_transfer(
         root_signer, another_signer.address, Amount.ether(10)
     )
 
-    with pytest.raises(BadResponseFormat, match="Expected a dictionary as a response, got str"):
-        receipt = await session.eth_get_transaction_receipt(tx_hash)
+    monkeypatch.setattr(local_provider, "rpc", lambda _method, *_args: "something")
 
+    with pytest.raises(BadResponseFormat, match="Cannot structure into"):
+        await session.eth_get_transaction_receipt(tx_hash)
 
-async def test_missing_field(test_provider, session, monkeypatch, root_signer, another_signer):
-    orig_eth_get_transaction_receipt = test_provider.eth_get_transaction_receipt
 
-    def faulty_eth_get_transaction_receipt(tx_hash):
-        receipt = orig_eth_get_transaction_receipt(tx_hash)
-        del receipt["status"]
-        return receipt
+async def test_missing_field(local_provider, session, monkeypatch, root_signer, another_signer):
+    orig_rpc = local_provider.rpc
 
-    monkeypatch.setattr(
-        test_provider, "eth_get_transaction_receipt", faulty_eth_get_transaction_receipt
-    )
+    def mock_rpc(method, *args):
+        result = orig_rpc(method, *args)
+        if method == "eth_getTransactionReceipt":
+            del result["status"]
+        return result
 
     tx_hash = await session.broadcast_transfer(
         root_signer, another_signer.address, Amount.ether(10)
     )
 
-    with pytest.raises(
-        BadResponseFormat, match="Expected field `status` is missing from the result"
-    ):
-        receipt = await session.eth_get_transaction_receipt(tx_hash)
+    monkeypatch.setattr(local_provider, "rpc", mock_rpc)
+
+    with pytest.raises(BadResponseFormat, match="status: Missing field"):
+        await session.eth_get_transaction_receipt(tx_hash)
 
 
 async def test_none_instead_of_dict(
-    test_provider, session, monkeypatch, root_signer, another_signer
+    local_provider, session, monkeypatch, root_signer, another_signer
 ):
+    tx_hash = await session.broadcast_transfer(
+        root_signer, another_signer.address, Amount.ether(10)
+    )
+
     # Check that a None can be returned in a call that expects a `dict`
     # (the interpretation of such an event is up to the client).
     # `eth_getTransactionReceipt` can return a None normally (if there's no receipt yet),
     # but we force it here, just in case.
-    monkeypatch.setattr(test_provider, "eth_get_transaction_receipt", lambda tx_hash: None)
-    tx_hash = await session.broadcast_transfer(
-        root_signer, another_signer.address, Amount.ether(10)
-    )
+    monkeypatch.setattr(local_provider, "rpc", lambda _method, *_args: None)
+
     assert await session.eth_get_transaction_receipt(tx_hash) is None
 
 
-async def test_non_ok_http_status(test_provider, session, monkeypatch):
-    def faulty_net_version():
+async def test_non_json_response(local_provider, session, monkeypatch):
+    def faulty_net_version(_method, *_args):
         # A generic exception will generate a 500 status code
-        raise Exception("Something unexpected happened")
+        raise Exception("Something unexpected happened")  # noqa: TRY002
 
-    monkeypatch.setattr(test_provider, "net_version", faulty_net_version)
+    monkeypatch.setattr(local_provider, "rpc", faulty_net_version)
 
-    with pytest.raises(
-        ProviderError, match=r"Provider error \(500\): Something unexpected happened"
-    ):
+    message = "Expected a JSON response, got HTTP status 500: Something unexpected happened"
+    with pytest.raises(BadResponseFormat, match=message):
         await session.net_version()
 
 
-async def test_neither_result_nor_error_field(test_provider, session, monkeypatch):
-    # Tests the handling of a badly formed provider response
-    # without either "error" or "result" fields.
-    # Unfortunately we can't achieve that by just patching the provider, have to patch the server
+async def test_no_result_field(session, monkeypatch):
+    # Tests the handling of a badly formed success response without the "result" field.
 
-    orig_process_request = provider_server.process_request
+    orig_process_request = _http_provider_server.process_request
 
     async def faulty_process_request(*args, **kwargs):
-        result = await orig_process_request(*args, **kwargs)
-        del result["result"]
-        return result
+        status, response = await orig_process_request(*args, **kwargs)
+        del response["result"]
+        return (status, response)
 
-    monkeypatch.setattr(provider_server, "process_request", faulty_process_request)
+    monkeypatch.setattr(_http_provider_server, "process_request", faulty_process_request)
 
     with pytest.raises(BadResponseFormat, match="`result` is not present in the response"):
         await session.net_version()
 
 
-async def test_result_is_not_a_dict(test_provider, session, monkeypatch):
+async def test_no_error_field(session, monkeypatch):
+    # Tests the handling of a badly formed error response without the "error" field.
+
+    orig_process_request = _http_provider_server.process_request
+
+    async def faulty_process_request(*args, **kwargs):
+        status, response = await orig_process_request(*args, **kwargs)
+        del response["result"]
+        return (HTTPStatus.BAD_REQUEST, response)
+
+    monkeypatch.setattr(_http_provider_server, "process_request", faulty_process_request)
+
+    with pytest.raises(HTTPError, match=r"HTTP status 400: {\"jsonrpc\":\"2.0\",\"id\":0}"):
+        await session.net_version()
+
+
+async def test_malformed_error_field(session, monkeypatch):
+    # Tests the handling of a badly formed error response
+    # where the "error" field cannot be parsed as an RPCError.
+
+    orig_process_request = _http_provider_server.process_request
+
+    async def faulty_process_request(*args, **kwargs):
+        status, response = await orig_process_request(*args, **kwargs)
+        del response["result"]
+        response["error"] = {"something_weird": 1}
+        return (HTTPStatus.BAD_REQUEST, response)
+
+    monkeypatch.setattr(_http_provider_server, "process_request", faulty_process_request)
+
+    with pytest.raises(BadResponseFormat, match=r"Failed to parse an error response"):
+        await session.net_version()
+
+
+async def test_result_is_not_a_dict(session, monkeypatch):
     # Tests the handling of a badly formed provider response that is not a dictionary.
     # Unfortunately we can't achieve that by just patching the provider, have to patch the server
 
-    async def faulty_process_request(*args, **kwargs):
-        return 1
+    async def faulty_process_request(*_args, **_kwargs):
+        return (HTTPStatus.OK, 1)
 
-    monkeypatch.setattr(provider_server, "process_request", faulty_process_request)
+    monkeypatch.setattr(_http_provider_server, "process_request", faulty_process_request)
 
     with pytest.raises(BadResponseFormat, match="RPC response must be a dictionary, got: 1"):
         await session.net_version()
 
 
 async def test_unreachable_provider():
     bad_provider = HTTPProvider("https://127.0.0.1:8889")
@@ -189,15 +190,15 @@
 async def test_default_implementations():
     class MockProvider(Provider):
         @asynccontextmanager
         async def session(self):
             yield MockSession()
 
     class MockSession(ProviderSession):
-        async def rpc(self, method, *args):
+        async def rpc(self, method, *_args):
             return method
 
     provider = MockProvider()
     async with provider.session() as session:
         result = await session.rpc_and_pin("1")
         assert result == ("1", ())
```

### Comparing `pons-0.7.0/PKG-INFO` & `pons-0.8.0/PKG-INFO`

 * *Files 12% similar despite different names*

```diff
@@ -1,18 +1,20 @@
 Metadata-Version: 2.1
 Name: pons
-Version: 0.7.0
+Version: 0.8.0
 Summary: Async RPC client for Ethereum
 License: MIT
 Author-email: Bogdan Opanchuk <bogdan@opanchuk.net>
-Requires-Python: >=3.8
+Requires-Python: >=3.10
+Provides-Extra: compiler
 Provides-Extra: docs
 Provides-Extra: lint
+Provides-Extra: local-provider
 Provides-Extra: tests
-Project-URL: homepage, https://github.com/fjarri/pons
+Project-URL: homepage, https://github.com/fjarri-eth/pons
 Description-Content-Type: text/markdown
 
 Async RPC client for Ethereum
 -----------------------------
 
 [![pypi package][pypi-image]][pypi-link] ![License][pypi-license-image] [![Docs][rtd-image]][rtd-link] [![Coverage][cov-image]][cov-link] [![Code style: black][black-image]][black-link]
 
@@ -22,12 +24,12 @@
 
 
 [pypi-image]: https://img.shields.io/pypi/v/pons
 [pypi-link]: https://pypi.org/project/pons/
 [pypi-license-image]: https://img.shields.io/pypi/l/pons
 [rtd-image]: https://readthedocs.org/projects/pons/badge/?version=latest
 [rtd-link]: https://pons.readthedocs.io/en/latest/
-[cov-image]: https://codecov.io/gh/fjarri/pons/branch/master/graph/badge.svg?token=RZP1LK1HB2
-[cov-link]: https://codecov.io/gh/fjarri/pons
+[cov-image]: https://codecov.io/gh/fjarri-eth/pons/branch/master/graph/badge.svg?token=RZP1LK1HB2
+[cov-link]: https://codecov.io/gh/fjarri-eth/pons
 [black-image]: https://img.shields.io/badge/code%20style-black-000000.svg
 [black-link]: https://github.com/psf/black
```

