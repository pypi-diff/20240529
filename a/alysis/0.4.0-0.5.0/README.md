# Comparing `tmp/alysis-0.4.0.tar.gz` & `tmp/alysis-0.5.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "alysis-0.4.0.tar", last modified: Fri Mar 15 23:44:23 2024, max compression
+gzip compressed data, was "alysis-0.5.0.tar", last modified: Wed May 29 03:10:51 2024, max compression
```

## Comparing `alysis-0.4.0.tar` & `alysis-0.5.0.tar`

### file list

```diff
@@ -1,18 +1,18 @@
--rw-r--r--   0        0        0     1059 2024-02-29 22:34:28.443213 alysis-0.4.0/LICENSE.md
--rw-r--r--   0        0        0      941 2024-02-29 22:34:28.443431 alysis-0.4.0/README.md
--rw-r--r--   0        0        0      474 2024-03-09 23:43:56.815632 alysis-0.4.0/alysis/__init__.py
--rw-r--r--   0        0        0    21974 2024-03-09 23:43:56.815920 alysis-0.4.0/alysis/_backend.py
--rw-r--r--   0        0        0      523 2024-03-09 18:48:26.579843 alysis-0.4.0/alysis/_exceptions.py
--rw-r--r--   0        0        0    16694 2024-03-15 23:17:51.724628 alysis-0.4.0/alysis/_node.py
--rw-r--r--   0        0        0    10425 2024-03-15 23:43:22.770566 alysis-0.4.0/alysis/_rpc.py
--rw-r--r--   0        0        0        0 2024-02-29 22:34:28.443481 alysis-0.4.0/alysis/py.typed
--rw-r--r--   0        0        0     7117 2024-03-15 23:43:22.770937 alysis-0.4.0/alysis/schema.py
--rw-r--r--   0        0        0      638 2024-02-29 22:34:28.443729 alysis-0.4.0/docs/Makefile
--rw-r--r--   0        0        0      873 2024-03-09 23:43:56.817426 alysis-0.4.0/docs/api.rst
--rw-r--r--   0        0        0     1566 2024-03-15 23:43:56.897895 alysis-0.4.0/docs/changelog.rst
--rw-r--r--   0        0        0     2531 2024-03-09 23:43:56.817935 alysis-0.4.0/docs/conf.py
--rw-r--r--   0        0        0      233 2024-03-01 04:40:00.207434 alysis-0.4.0/docs/index.rst
--rw-r--r--   0        0        0     2001 2024-03-15 23:44:03.415352 alysis-0.4.0/pyproject.toml
--rw-r--r--   0        0        0      375 2024-03-01 05:46:43.553586 alysis-0.4.0/tests/conftest.py
--rw-r--r--   0        0        0      607 2024-03-09 20:23:05.241284 alysis-0.4.0/tests/test_rpc.py
--rw-r--r--   0        0        0     1448 1970-01-01 00:00:00.000000 alysis-0.4.0/PKG-INFO
+-rw-r--r--   0        0        0     1059 2024-02-29 22:34:28.443213 alysis-0.5.0/LICENSE.md
+-rw-r--r--   0        0        0      949 2024-05-29 03:08:32.107855 alysis-0.5.0/README.md
+-rw-r--r--   0        0        0      501 2024-05-29 03:08:32.108358 alysis-0.5.0/alysis/__init__.py
+-rw-r--r--   0        0        0    22931 2024-05-29 03:08:32.108831 alysis-0.5.0/alysis/_backend.py
+-rw-r--r--   0        0        0      924 2024-05-29 03:08:32.109037 alysis-0.5.0/alysis/_constants.py
+-rw-r--r--   0        0        0      523 2024-03-09 18:48:26.579843 alysis-0.5.0/alysis/_exceptions.py
+-rw-r--r--   0        0        0    16885 2024-05-29 03:08:32.109449 alysis-0.5.0/alysis/_node.py
+-rw-r--r--   0        0        0     9501 2024-05-29 03:08:32.109957 alysis-0.5.0/alysis/_rpc.py
+-rw-r--r--   0        0        0        0 2024-02-29 22:34:28.443481 alysis-0.5.0/alysis/py.typed
+-rw-r--r--   0        0        0      638 2024-02-29 22:34:28.443729 alysis-0.5.0/docs/Makefile
+-rw-r--r--   0        0        0      412 2024-05-29 03:08:32.110300 alysis-0.5.0/docs/api.rst
+-rw-r--r--   0        0        0     1832 2024-05-29 03:09:49.370925 alysis-0.5.0/docs/changelog.rst
+-rw-r--r--   0        0        0     2541 2024-05-29 03:08:32.110973 alysis-0.5.0/docs/conf.py
+-rw-r--r--   0        0        0      233 2024-03-01 04:40:00.207434 alysis-0.5.0/docs/index.rst
+-rw-r--r--   0        0        0     2068 2024-05-29 03:09:15.202765 alysis-0.5.0/pyproject.toml
+-rw-r--r--   0        0        0      376 2024-05-29 03:08:32.112668 alysis-0.5.0/tests/conftest.py
+-rw-r--r--   0        0        0      615 2024-05-29 02:49:57.277727 alysis-0.5.0/tests/test_rpc.py
+-rw-r--r--   0        0        0     1460 1970-01-01 00:00:00.000000 alysis-0.5.0/PKG-INFO
```

### Comparing `alysis-0.4.0/LICENSE.md` & `alysis-0.5.0/LICENSE.md`

 * *Files identical despite different names*

### Comparing `alysis-0.4.0/README.md` & `alysis-0.5.0/README.md`

 * *Files 13% similar despite different names*

```diff
@@ -9,9 +9,9 @@
 
 
 [pypi-image]: https://img.shields.io/pypi/v/alysis
 [pypi-link]: https://pypi.org/project/alysis/
 [pypi-license-image]: https://img.shields.io/pypi/l/alysis
 [rtd-image]: https://readthedocs.org/projects/alysis/badge/?version=latest
 [rtd-link]: https://alysis.readthedocs.io/en/latest/
-[cov-image]: https://codecov.io/gh/fjarri/alysis/branch/master/graph/badge.svg?token=RZP1LK1HB2
-[cov-link]: https://codecov.io/gh/fjarri/alysis
+[cov-image]: https://codecov.io/gh/fjarri-eth/alysis/branch/master/graph/badge.svg?token=RZP1LK1HB2
+[cov-link]: https://codecov.io/gh/fjarri-eth/alysis
```

### Comparing `alysis-0.4.0/alysis/_backend.py` & `alysis-0.5.0/alysis/_backend.py`

 * *Files 11% similar despite different names*

```diff
@@ -13,93 +13,123 @@
     ReceiptAPI,
     SignedTransactionAPI,
     TransactionFieldsAPI,
     VirtualMachineAPI,
 )
 from eth.chains.base import MiningChain
 from eth.constants import (
+    BLANK_ROOT_HASH,
     POST_MERGE_DIFFICULTY,
     POST_MERGE_MIX_HASH,
     POST_MERGE_NONCE,
 )
 from eth.db import get_db_backend
 from eth.exceptions import HeaderNotFound, Revert, VMError
 from eth.tools.builder.chain import copy as copy_chain
 from eth.typing import AccountDetails
-from eth.vm.forks import ShanghaiVM
+from eth.vm.forks import (
+    BerlinVM,
+    ByzantiumVM,
+    CancunVM,
+    ConstantinopleVM,
+    HomesteadVM,
+    IstanbulVM,
+    LondonVM,
+    ParisVM,
+    ShanghaiVM,
+    SpuriousDragonVM,
+    TangerineWhistleVM,
+)
 from eth.vm.forks.berlin.transactions import TypedTransaction
 from eth.vm.spoof import SpoofTransaction
 from eth_keys import KeyAPI
 from eth_typing import Address as EthAddress
 from eth_typing import BlockNumber as EthBlockNumber
 from eth_typing import Hash32 as EthHash32
-from eth_utils import encode_hex, keccak
 from eth_utils.exceptions import ValidationError as EthValidationError
-
-from ._exceptions import (
-    BlockNotFound,
-    TransactionFailed,
-    TransactionNotFound,
-    TransactionReverted,
-    ValidationError,
-)
-from .schema import (
+from ethereum_rpc import (
     Address,
+    Amount,
     Block,
+    BlockHash,
     BlockInfo,
     BlockLabel,
     BlockNonce,
     EstimateGasParams,
     EthCallParams,
-    Hash32,
     LogEntry,
     LogsBloom,
     LogTopic,
-    TransactionInfo,
-    TransactionReceipt,
+    TrieHash,
+    TxHash,
+    TxInfo,
+    TxReceipt,
+    UnclesHash,
+    keccak,
+)
+
+from ._constants import EVMVersion
+from ._exceptions import (
+    BlockNotFound,
+    TransactionFailed,
+    TransactionNotFound,
+    TransactionReverted,
+    ValidationError,
 )
 
 ZERO_ADDRESS = EthAddress(20 * b"\x00")
 
+EVM_MAPPING = {
+    EVMVersion.HOMESTEAD: HomesteadVM,
+    EVMVersion.TANGERINE_WHISTLE: TangerineWhistleVM,
+    EVMVersion.SPURIOUS_DRAGON: SpuriousDragonVM,
+    EVMVersion.BYZANTIUM: ByzantiumVM,
+    EVMVersion.CONSTANTINOPLE: ConstantinopleVM,
+    EVMVersion.ISTANBUL: IstanbulVM,
+    EVMVersion.BERLIN: BerlinVM,
+    EVMVersion.LONDON: LondonVM,
+    EVMVersion.PARIS: ParisVM,
+    EVMVersion.SHANGHAI: ShanghaiVM,
+    EVMVersion.CANCUN: CancunVM,
+}
+
 
 def _rlp_encode(obj: Any) -> bytes:
     # Force typing here, since `rlp` is not typed
     return cast(bytes, rlp.encode(obj))
 
 
 class PyEVMBackend:
-    def __init__(self, root_balance_wei: int, chain_id: int):
+    def __init__(self, root_balance_wei: int, chain_id: int, evm_version: EVMVersion):
         chain_id_ = chain_id
 
         class MainnetTesterPosChain(MiningChain):
             chain_id = chain_id_
-            vm_configuration = ((EthBlockNumber(0), ShanghaiVM),)
+            vm_configuration = ((EthBlockNumber(0), EVM_MAPPING[evm_version]),)
 
             def create_header_from_parent(
                 self, parent_header: BlockHeaderAPI, **header_params: Any
             ) -> BlockHeaderAPI:
                 """
                 Call the parent class method maintaining the same gas_limit as the
                 previous block.
                 """
                 header_params["gas_limit"] = parent_header.gas_limit
                 return super().create_header_from_parent(parent_header, **header_params)
 
-        blank_root_hash = keccak(_rlp_encode(b""))
-
         genesis_params: dict[str, None | int | EthBlockNumber | bytes | EthAddress | EthHash32] = {
             "coinbase": ZERO_ADDRESS,
             "difficulty": POST_MERGE_DIFFICULTY,
             "extra_data": b"",
             "gas_limit": 30029122,  # gas limit at London fork block 12965000 on mainnet
             "mix_hash": POST_MERGE_MIX_HASH,
             "nonce": POST_MERGE_NONCE,
-            "receipt_root": blank_root_hash,
+            "receipt_root": BLANK_ROOT_HASH,
             "timestamp": int(time.time()),
-            "transaction_root": blank_root_hash,
+            "transaction_root": BLANK_ROOT_HASH,
         }
 
         account_state: AccountDetails = {
             "balance": root_balance_wei,
             "storage": {},
             "code": b"",
             "nonce": 0,
@@ -136,30 +166,30 @@
         self._total_difficulty = total_difficulty
 
     def __deepcopy__(self, _memo: None | dict[Any, Any]) -> "PyEVMBackend":
         obj = object.__new__(self.__class__)
         obj._initialize(copy_chain(self.chain), self.root_private_key, self._total_difficulty)  # noqa: SLF001
         return obj
 
-    def mine_block(self, timestamp: None | int = None) -> Hash32:
+    def mine_block(self, timestamp: None | int = None) -> BlockHash:
         if timestamp is not None:
             current_timestamp = self.chain.header.timestamp
             if timestamp < current_timestamp:
                 raise ValidationError(
                     f"The new timestamp ({timestamp}) must be greater than "
                     f"the current one ({current_timestamp})"
                 )
 
             # timestamp adjusted by 1 b/c a second is added in mine_blocks
             self.chain.header = self.chain.header.copy(timestamp=timestamp - 1)
 
         # ParisVM and forward, generate a random `mix_hash` to simulate the `prevrandao` value.
         mix_hash = os.urandom(32)
 
-        block_hash = Hash32(self.chain.mine_block(coinbase=ZERO_ADDRESS, mix_hash=mix_hash).hash)
+        block_hash = BlockHash(self.chain.mine_block(coinbase=ZERO_ADDRESS, mix_hash=mix_hash).hash)
         self._total_difficulty += self._get_block_by_number(BlockLabel.LATEST).header.difficulty
         return block_hash
 
     def _get_block_by_number(self, block: Block) -> BlockAPI:
         if isinstance(block, int):
             # Note: The head block is the pending block. If a block number is passed
             # explicitly here, return the block only if it is already part of the chain
@@ -190,22 +220,22 @@
             receipt = receipts[transaction_index]
             for log_index, log in enumerate(receipt.logs):
                 entries.append(
                     make_log_entry(block, transaction, transaction_index, log, log_index)
                 )
         return entries
 
-    def get_log_entries_by_block_hash(self, block_hash: Hash32) -> list[LogEntry]:
+    def get_log_entries_by_block_hash(self, block_hash: BlockHash) -> list[LogEntry]:
         return self._get_log_entries(self._get_block_by_hash(block_hash))
 
     def get_log_entries_by_block_number(self, block: Block) -> list[LogEntry]:
         return self._get_log_entries(self._get_block_by_number(block))
 
-    def get_latest_block_hash(self) -> Hash32:
-        return Hash32(self._get_block_by_number(BlockLabel.LATEST).hash)
+    def get_latest_block_hash(self) -> BlockHash:
+        return BlockHash(self._get_block_by_number(BlockLabel.LATEST).hash)
 
     def get_latest_block_number(self) -> int:
         return self._get_block_by_number(BlockLabel.LATEST).number
 
     def get_block_by_number(self, block: Block, *, with_transactions: bool) -> BlockInfo:
         block_api = self._get_block_by_number(block)
         is_pending = block_api.number == self.chain.get_block().number
@@ -213,105 +243,105 @@
             self.chain_id,
             block_api,
             total_difficulty=self._total_difficulty,
             with_transactions=with_transactions,
             is_pending=is_pending,
         )
 
-    def _get_block_by_hash(self, block_hash: Hash32) -> BlockAPI:
+    def _get_block_by_hash(self, block_hash: BlockHash) -> BlockAPI:
         try:
-            block = self.chain.get_block_by_hash(EthHash32(block_hash))
+            block = self.chain.get_block_by_hash(EthHash32(bytes(block_hash)))
         except HeaderNotFound as exc:
             raise BlockNotFound(f"No block found for block hash: {block_hash.hex()}") from exc
 
         if block.number >= self.chain.get_block().number:
             raise BlockNotFound(f"No block found for block hash: {block_hash.hex()}")
 
         return block
 
-    def get_block_number_by_hash(self, block_hash: Hash32) -> int:
+    def get_block_number_by_hash(self, block_hash: BlockHash) -> int:
         return self._get_block_by_hash(block_hash).number
 
-    def get_block_by_hash(self, block_hash: Hash32, *, with_transactions: bool) -> BlockInfo:
+    def get_block_by_hash(self, block_hash: BlockHash, *, with_transactions: bool) -> BlockInfo:
         block = self._get_block_by_hash(block_hash)
         is_pending = block.number == self.chain.get_block().number
         return make_block_info(
             self.chain_id,
             block,
             total_difficulty=self._total_difficulty,
             with_transactions=with_transactions,
             is_pending=is_pending,
         )
 
     def _get_transaction_by_hash(
-        self, transaction_hash: Hash32
+        self, transaction_hash: TxHash
     ) -> tuple[BlockAPI, SignedTransactionAPI, int]:
         head_block = self.chain.get_block()
         for index, transaction in enumerate(head_block.transactions):
-            if Hash32(transaction.hash) == transaction_hash:
+            if TxHash(transaction.hash) == transaction_hash:
                 return head_block, transaction, index
         # Since there is no method in PyEvm to get a transaction by hash directly,
         # we have to go through all the blocks, starting from the most recent ones.
         for block_number in range(head_block.number - 1, -1, -1):
             block = self._get_block_by_number(block_number)
             for index, transaction in enumerate(block.transactions):
-                if Hash32(transaction.hash) == transaction_hash:
+                if TxHash(transaction.hash) == transaction_hash:
                     return block, transaction, index
 
         raise TransactionNotFound(
-            f"No transaction found for transaction hash: {encode_hex(transaction_hash)}"
+            f"No transaction found for transaction hash: {transaction_hash.hex()}"
         )
 
-    def get_transaction_by_hash(self, transaction_hash: Hash32) -> TransactionInfo:
+    def get_transaction_by_hash(self, transaction_hash: TxHash) -> TxInfo:
         block, transaction, transaction_index = self._get_transaction_by_hash(
             transaction_hash,
         )
         is_pending = block.number == self.chain.get_block().number
         return make_transaction_info(
             self.chain_id, block, transaction, transaction_index, is_pending=is_pending
         )
 
     def _get_vm_for_block_number(self, block: Block) -> VirtualMachineAPI:
         block_api = self._get_block_by_number(block)
         return self.chain.get_vm(at_header=block_api.header)
 
-    def get_transaction_receipt(self, transaction_hash: Hash32) -> TransactionReceipt:
+    def get_transaction_receipt(self, transaction_hash: TxHash) -> TxReceipt:
         block, transaction, transaction_index = self._get_transaction_by_hash(
             transaction_hash,
         )
         is_pending = block.number == self.chain.get_block().number
         if is_pending:
             raise TransactionNotFound(
-                f"Transaction {encode_hex(transaction_hash)} is not yet included in a block"
+                f"Transaction {transaction_hash.hex()} is not yet included in a block"
             )
 
         block_receipts = block.get_receipts(self.chain.chaindb)
 
         return make_transaction_receipt(
             block,
             transaction,
             block_receipts,
             transaction_index,
         )
 
     def get_transaction_count(self, address: Address, block: Block) -> int:
         vm = self._get_vm_for_block_number(block)
-        return vm.state.get_nonce(EthAddress(address))
+        return vm.state.get_nonce(EthAddress(bytes(address)))
 
     def get_balance(self, address: Address, block: Block) -> int:
         vm = self._get_vm_for_block_number(block)
-        return vm.state.get_balance(EthAddress(address))
+        return vm.state.get_balance(EthAddress(bytes(address)))
 
     def get_code(self, address: Address, block: Block) -> bytes:
         vm = self._get_vm_for_block_number(block)
-        return vm.state.get_code(EthAddress(address))
+        return vm.state.get_code(EthAddress(bytes(address)))
 
     def get_storage(self, address: Address, slot: int, block: Block) -> bytes:
         vm = self._get_vm_for_block_number(block)
-        return vm.state.get_storage(EthAddress(address), slot).to_bytes(32, byteorder="big")
+        return vm.state.get_storage(EthAddress(bytes(address)), slot).to_bytes(32, byteorder="big")
 
     def get_base_fee(self, block: Block) -> int:
         vm = self._get_vm_for_block_number(block)
         return vm.state.base_fee
 
     def decode_transaction(self, raw_transaction: bytes) -> SignedTransactionAPI:
         vm = self._get_vm_for_block_number(BlockLabel.LATEST)
@@ -327,26 +357,26 @@
             raise ValidationError(f"Invalid transaction: {exc}") from exc
         return evm_transaction.hash
 
     def estimate_gas(self, params: EstimateGasParams, block: Block) -> int:
         from_ = params.from_
         header = self._get_block_by_number(block).header
         nonce = self.get_transaction_count(from_, block) if params.nonce is None else params.nonce
-        to = EthAddress(b"" if params.to is None else params.to)
+        to = EthAddress(b"" if params.to is None else bytes(params.to))
 
         evm_transaction = self.chain.create_unsigned_transaction(
-            gas_price=params.gas_price,
-            gas=params.gas if params.gas is not None else header.gas_limit,
+            gas_price=params.gas_price.as_wei() if params.gas_price else 0,
+            gas=params.gas if params.gas else header.gas_limit,
             nonce=nonce,
-            value=params.value,
-            data=params.data if params.data is not None else b"",
+            value=params.value.as_wei() if params.value else 0,
+            data=params.data if params.data else b"",
             to=to,
         )
 
-        spoofed_transaction = SpoofTransaction(evm_transaction, from_=EthAddress(from_))
+        spoofed_transaction = SpoofTransaction(evm_transaction, from_=EthAddress(bytes(from_)))
 
         try:
             # For whatever reason `SpoofTransaction` does not implement `SignedTransactionAPI`,
             # but has the same duck type.
             return self.chain.estimate_gas(cast(SignedTransactionAPI, spoofed_transaction), header)
 
         except EthValidationError as exc:
@@ -356,23 +386,23 @@
             raise TransactionReverted(exc.args[0]) from exc
 
         except VMError as exc:
             raise TransactionFailed(exc.args[0]) from exc
 
     def call(self, params: EthCallParams, block: Block) -> bytes:
         nonce = self.get_transaction_count(params.from_, block) if params.from_ else 0
-        from_ = EthAddress(params.from_) if params.from_ is not None else ZERO_ADDRESS
+        from_ = EthAddress(bytes(params.from_)) if params.from_ is not None else ZERO_ADDRESS
         header = self._get_block_by_number(block).header
         evm_transaction = self.chain.create_unsigned_transaction(
-            gas_price=params.gas_price,
+            gas_price=params.gas_price.as_wei() if params.gas_price else 0,
             gas=params.gas if params.gas is not None else header.gas_limit,
             nonce=nonce,
-            value=params.value,
+            value=params.value.as_wei() if params.value else 0,
             data=params.data if params.data is not None else b"",
-            to=EthAddress(params.to),
+            to=EthAddress(bytes(params.to)),
         )
         spoofed_transaction = SpoofTransaction(evm_transaction, from_=from_)
 
         try:
             # For whatever reason `SpoofTransaction` does not implement `SignedTransactionAPI`,
             # but has the same duck type.
             return self.chain.get_transaction_result(
@@ -393,100 +423,100 @@
     chain_id: int,
     block: BlockAPI,
     *,
     total_difficulty: int,
     with_transactions: bool,
     is_pending: bool,
 ) -> BlockInfo:
-    transactions: list[Hash32] | list[TransactionInfo]
+    transactions: tuple[TxHash, ...] | tuple[TxInfo, ...]
     if with_transactions:
-        transactions = [
+        transactions = tuple(
             make_transaction_info(chain_id, block, transaction, index, is_pending=is_pending)
             for index, transaction in enumerate(block.transactions)
-        ]
+        )
     else:
-        transactions = [Hash32(transaction.hash) for transaction in block.transactions]
+        transactions = tuple(TxHash(transaction.hash) for transaction in block.transactions)
 
     return BlockInfo(
         # While the docs for major provider say that `number` is `null` for pending blocks,
         # it actually isn't in their return values.
         number=block.header.block_number,
-        hash=Hash32(block.header.hash) if not is_pending else None,
-        parent_hash=Hash32(block.header.parent_hash),
+        hash_=BlockHash(block.header.hash) if not is_pending else None,
+        parent_hash=BlockHash(block.header.parent_hash),
         nonce=BlockNonce(block.header.nonce) if not is_pending else None,
-        sha3_uncles=Hash32(block.header.uncles_hash),
+        sha3_uncles=UnclesHash(block.header.uncles_hash),
         logs_bloom=LogsBloom(block.header.bloom.to_bytes(256, byteorder="big"))
         if not is_pending
         else None,
-        transactions_root=Hash32(block.header.transaction_root),
-        state_root=Hash32(block.header.state_root),
-        receipts_root=Hash32(block.header.receipt_root),
+        transactions_root=TrieHash(block.header.transaction_root),
+        state_root=TrieHash(block.header.state_root),
+        receipts_root=TrieHash(block.header.receipt_root),
         miner=Address(block.header.coinbase) if not is_pending else None,
         difficulty=block.header.difficulty if not is_pending else 0,
         total_difficulty=total_difficulty if not is_pending else None,
         extra_data=block.header.extra_data.rjust(32, b"\x00"),
         # Note: not sure if this is right, but Ethereum is extremely vague
         # about what this field represents. Reopen #16 if there is new information.
         size=len(_rlp_encode(block)),
         gas_limit=block.header.gas_limit,
         gas_used=block.header.gas_used,
         # Note: this appears after EIP-1559 upgrade. Ethereum.org does not list this field,
         # but it's returned by providers.
         # Since we create the VM with Shanghai fork, we can safely cast to int here.
-        base_fee_per_gas=cast(int, block.header.base_fee_per_gas),
+        base_fee_per_gas=Amount(cast(int, block.header.base_fee_per_gas)),
         timestamp=block.header.timestamp,
         transactions=transactions,
-        uncles=[Hash32(uncle.hash) for uncle in block.uncles],
+        uncles=tuple(BlockHash(uncle.hash) for uncle in block.uncles),
     )
 
 
 def make_transaction_info(
     chain_id: int,
     block: BlockAPI,
     transaction: SignedTransactionAPI,
     transaction_index: int,
     *,
     is_pending: bool,
-) -> TransactionInfo:
+) -> TxInfo:
     txn_type = _extract_transaction_type(transaction)
-    return TransactionInfo(
+    return TxInfo(
         chain_id=chain_id,
-        block_hash=Hash32(block.hash) if not is_pending else None,
-        hash=Hash32(transaction.hash),
+        block_hash=BlockHash(block.hash) if not is_pending else None,
+        hash_=TxHash(transaction.hash),
         nonce=transaction.nonce,
         # While the docs for major provider say that `number` is `null`
         # for pending transactions, it actually isn't in their return values.
         block_number=block.number,
         transaction_index=None if is_pending else transaction_index,
         from_=Address(transaction.sender),
         to=Address(transaction.to),
-        value=transaction.value,
+        value=Amount(transaction.value),
         gas=transaction.gas,
-        max_fee_per_gas=transaction.max_fee_per_gas,
-        max_priority_fee_per_gas=transaction.max_priority_fee_per_gas,
+        max_fee_per_gas=Amount(transaction.max_fee_per_gas),
+        max_priority_fee_per_gas=Amount(transaction.max_priority_fee_per_gas),
         # It is still being returned by providers
         gas_price=(
-            transaction.max_fee_per_gas
+            Amount(transaction.max_fee_per_gas)
             if is_pending
             else _calculate_effective_gas_price(transaction, block, txn_type)
         ),
-        input=transaction.data,
-        type=txn_type,
+        input_=transaction.data,
+        type_=txn_type,
         r=transaction.r,
         s=transaction.s,
         v=transaction.y_parity,
     )
 
 
 def make_transaction_receipt(
     block: BlockAPI,
     transaction: SignedTransactionAPI,
     receipts: Sequence[ReceiptAPI],
     transaction_index: int,
-) -> TransactionReceipt:
+) -> TxReceipt:
     txn_type = _extract_transaction_type(transaction)
     receipt = receipts[transaction_index]
 
     if transaction.to == b"":
         contract_addr = Address(
             _generate_contract_address(
                 transaction.sender,
@@ -497,52 +527,52 @@
         contract_addr = None
 
     if transaction_index == 0:
         origin_gas = 0
     else:
         origin_gas = receipts[transaction_index - 1].gas_used
 
-    return TransactionReceipt(
-        block_hash=Hash32(block.hash),
+    return TxReceipt(
+        block_hash=BlockHash(block.hash),
         block_number=block.number,
         contract_address=contract_addr,
         cumulative_gas_used=receipt.gas_used,
         effective_gas_price=_calculate_effective_gas_price(transaction, block, txn_type),
         from_=Address(transaction.sender),
         gas_used=receipt.gas_used - origin_gas,
-        logs=[
+        logs=tuple(
             make_log_entry(block, transaction, transaction_index, log, log_index)
             for log_index, log in enumerate(receipt.logs)
-        ],
+        ),
         logs_bloom=LogsBloom(receipt.bloom.to_bytes(256, byteorder="big")),
         status=1 if receipt.state_root == b"\x01" else 0,
-        to=Address(transaction.to) or None,
-        transaction_hash=Hash32(transaction.hash),
+        to=Address(transaction.to) if transaction.to else None,
+        transaction_hash=TxHash(transaction.hash),
         transaction_index=transaction_index,
-        type=txn_type,
+        type_=txn_type,
     )
 
 
 def make_log_entry(
     block: BlockAPI,
     transaction: TransactionFieldsAPI,
     transaction_index: int,
     log: LogAPI,
     log_index: int,
 ) -> LogEntry:
     return LogEntry(
         address=Address(log.address),
-        block_hash=Hash32(block.hash),
+        block_hash=BlockHash(block.hash),
         block_number=block.number,
         data=log.data,
         log_index=log_index,
         removed=False,
-        topics=[LogTopic(topic.to_bytes(32, byteorder="big")) for topic in log.topics],
+        topics=tuple(LogTopic(topic.to_bytes(32, byteorder="big")) for topic in log.topics),
         transaction_index=transaction_index,
-        transaction_hash=Hash32(transaction.hash),
+        transaction_hash=TxHash(transaction.hash),
     )
 
 
 def _generate_contract_address(address: EthAddress, nonce: int) -> EthAddress:
     next_account_hash = keccak(_rlp_encode([address, nonce]))
     return EthAddress(next_account_hash[-20:])
 
@@ -556,19 +586,19 @@
         return 1
     # legacy transactions being '0x0' taken from current geth version v1.10.10
     return 0
 
 
 def _calculate_effective_gas_price(
     transaction: TransactionFieldsAPI, block: BlockAPI, transaction_type: int
-) -> int:
+) -> Amount:
     base_fee_per_gas = block.header.base_fee_per_gas
     # It is not None after the London fork.
     assert base_fee_per_gas is not None  # noqa: S101
-    return (
+    return Amount(
         min(
             transaction.max_fee_per_gas,
             transaction.max_priority_fee_per_gas + base_fee_per_gas,
         )
         if transaction_type == 2
         else transaction.gas_price
     )
```

### Comparing `alysis-0.4.0/alysis/_exceptions.py` & `alysis-0.5.0/alysis/_exceptions.py`

 * *Files identical despite different names*

### Comparing `alysis-0.4.0/alysis/_node.py` & `alysis-0.5.0/alysis/_node.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,32 +1,33 @@
 import itertools
 from collections.abc import Iterator
 from copy import deepcopy
 from typing import Any
 
-from ._backend import PyEVMBackend
-from ._exceptions import (
-    FilterNotFound,
-    ValidationError,
-)
-from .schema import (
+from ethereum_rpc import (
     Address,
+    Amount,
     Block,
+    BlockHash,
     BlockInfo,
     BlockLabel,
     EstimateGasParams,
     EthCallParams,
     FilterParams,
     FilterParamsEIP234,
-    Hash32,
     LogEntry,
-    TransactionInfo,
-    TransactionReceipt,
+    TxHash,
+    TxInfo,
+    TxReceipt,
 )
 
+from ._backend import PyEVMBackend
+from ._constants import EVMVersion
+from ._exceptions import FilterNotFound, ValidationError
+
 
 class LogFilter:
     def __init__(self, params: FilterParams, current_block_number: int):
         if isinstance(params.from_block, int):
             from_block = params.from_block
         elif params.from_block in (BlockLabel.LATEST, BlockLabel.SAFE, BlockLabel.FINALIZED):
             from_block = current_block_number
@@ -40,20 +41,20 @@
         elif params.to_block in (BlockLabel.LATEST, BlockLabel.SAFE, BlockLabel.FINALIZED):
             to_block = None  # indicates an open-ended filter
         elif params.from_block == BlockLabel.EARLIEST:
             to_block = 0
         else:
             raise ValidationError(f"`to_block` value of {params.to_block} is not supported")
 
-        if isinstance(params.address, list):
+        if isinstance(params.address, tuple):
             addresses = params.address
         elif params.address is None:
             addresses = None
         else:
-            addresses = [params.address]
+            addresses = (params.address,)
 
         self._from_block = from_block
         self._to_block = to_block
         self._addresses = addresses
         self._topics = params.topics
 
     def block_number_range(self, current_block_number: int) -> range:
@@ -81,15 +82,15 @@
         # But note that if `self._topics` is shorter than `entry.topics`
         # it is equivalent to the missing values being `None`,
         # that is, matching anything.
         for topics, logged_topic in zip(self._topics, entry.topics, strict=False):
             if topics is None:
                 continue
 
-            filter_topics = topics if isinstance(topics, list) else [topics]
+            filter_topics = topics if isinstance(topics, tuple) else (topics,)
 
             for filter_topic in filter_topics:
                 if filter_topic == logged_topic:
                     break
             else:
                 return False
 
@@ -109,19 +110,22 @@
     root_private_key: bytes
     """The private key of the funded address created with the chain."""
 
     def __init__(
         self,
         *,
         root_balance_wei: int,
+        evm_version: EVMVersion = EVMVersion.CANCUN,
         chain_id: int = DEFAULT_ID,
         net_version: int = 1,
         auto_mine_transactions: bool = True,
     ):
-        backend = PyEVMBackend(root_balance_wei=root_balance_wei, chain_id=chain_id)
+        backend = PyEVMBackend(
+            root_balance_wei=root_balance_wei, chain_id=chain_id, evm_version=evm_version
+        )
         self._initialize(
             backend=backend,
             net_version=net_version,
             auto_mine_transactions=auto_mine_transactions,
             filter_counter=itertools.count(),
             log_filters={},
             log_filter_entries={},
@@ -133,16 +137,16 @@
         self,
         backend: PyEVMBackend,
         net_version: int,
         auto_mine_transactions: bool,  # noqa: FBT001
         filter_counter: Iterator[int],
         log_filters: dict[int, LogFilter],
         log_filter_entries: dict[int, list[LogEntry]],
-        block_filters: dict[int, list[Hash32]],
-        pending_transaction_filters: dict[int, list[Hash32]],
+        block_filters: dict[int, list[BlockHash]],
+        pending_transaction_filters: dict[int, list[TxHash]],
     ) -> None:
         self.root_private_key = backend.root_private_key
         self._backend = backend
         self._auto_mine_transactions = auto_mine_transactions
         self._net_version = net_version
 
         # filter tracking
@@ -205,22 +209,22 @@
         """Returns the current network id."""
         return self._net_version
 
     def eth_chain_id(self) -> int:
         """Returns the chain ID used for signing replay-protected transactions."""
         return self._backend.chain_id
 
-    def eth_gas_price(self) -> int:
+    def eth_gas_price(self) -> Amount:
         """Returns an estimate of the current price per gas in wei."""
         # The specific algorithm is not enforced in the standard,
         # but this is the logic Infura uses. Seems to work for them.
         block_info = self.eth_get_block_by_number(BlockLabel.LATEST, with_transactions=False)
 
         # Base fee plus 1 GWei
-        return block_info.base_fee_per_gas + 10**9
+        return block_info.base_fee_per_gas + Amount.gwei(1)
 
     def eth_block_number(self) -> int:
         """Returns the number of most recent block."""
         return self._backend.get_latest_block_number()
 
     def eth_get_balance(self, address: Address, block: Block) -> int:
         """Returns the balance (in wei) of the account of given address."""
@@ -239,15 +243,15 @@
         """Returns the value from a storage position at a given address."""
         return self._backend.get_storage(address, slot, block)
 
     def eth_get_transaction_count(self, address: Address, block: Block) -> int:
         """Returns the number of transactions sent from an address."""
         return self._backend.get_transaction_count(address, block)
 
-    def eth_get_transaction_by_hash(self, transaction_hash: Hash32) -> TransactionInfo:
+    def eth_get_transaction_by_hash(self, transaction_hash: TxHash) -> TxInfo:
         """
         Returns the information about a transaction requested by transaction hash.
 
         Raises :py:class:`TransactionNotFound` if the transaction with this hash
         has not been included in a block yet.
         """
         return self._backend.get_transaction_by_hash(transaction_hash)
@@ -256,43 +260,43 @@
         """
         Returns information about a block by block number.
 
         Raises :py:class:`BlockNotFound` if the requested block does not exist.
         """
         return self._backend.get_block_by_number(block, with_transactions=with_transactions)
 
-    def eth_get_block_by_hash(self, block_hash: Hash32, *, with_transactions: bool) -> BlockInfo:
+    def eth_get_block_by_hash(self, block_hash: BlockHash, *, with_transactions: bool) -> BlockInfo:
         """
         Returns information about a block by hash.
 
         Raises :py:class:`BlockNotFound` if the requested block does not exist.
         """
         return self._backend.get_block_by_hash(block_hash, with_transactions=with_transactions)
 
-    def eth_get_transaction_receipt(self, transaction_hash: Hash32) -> TransactionReceipt:
+    def eth_get_transaction_receipt(self, transaction_hash: TxHash) -> TxReceipt:
         """
         Returns the receipt of a transaction by transaction hash.
 
         Raises :py:class:`TransactionNotFound` if the transaction with this hash
         has not been included in a block yet.
         """
         return self._backend.get_transaction_receipt(transaction_hash)
 
-    def eth_send_raw_transaction(self, raw_transaction: bytes) -> Hash32:
+    def eth_send_raw_transaction(self, raw_transaction: bytes) -> TxHash:
         """
         Attempts to add a signed RLP-encoded transaction to the current block.
         Returns the transaction hash on success.
 
         If the transaction is invalid, raises :py:class:`ValidationError`.
         If the transaction is sent to the EVM but is reverted during execution,
         raises :py:class:`TransactionReverted`.
         If there were other problems with the transaction, raises :py:class:`TransactionFailed`.
         """
         transaction = self._backend.decode_transaction(raw_transaction)
-        transaction_hash = Hash32(transaction.hash)
+        transaction_hash = TxHash(transaction.hash)
 
         for tx_filter in self._pending_transaction_filters.values():
             tx_filter.append(transaction_hash)
 
         self._backend.send_decoded_transaction(transaction)
 
         if self._auto_mine_transactions:
@@ -363,33 +367,35 @@
         elif filter_id in self._pending_transaction_filters:
             del self._pending_transaction_filters[filter_id]
         elif filter_id in self._log_filters:
             del self._log_filters[filter_id]
         else:
             raise FilterNotFound("Unknown filter id")
 
-    def eth_get_filter_changes(self, filter_id: int) -> list[LogEntry] | list[Hash32]:
+    def eth_get_filter_changes(
+        self, filter_id: int
+    ) -> list[LogEntry] | list[TxHash] | list[BlockHash]:
         """
         Polling method for a filter, which returns an array of logs which occurred since last poll.
 
         .. note::
 
             This method will not return the events that happened before the filter creation,
             even if they satisfy the filter predicate.
             Call :py:meth:`eth_get_filter_logs` to get those.
         """
         if filter_id in self._block_filters:
-            entries = self._block_filters[filter_id]
+            block_entries = self._block_filters[filter_id]
             self._block_filters[filter_id] = []
-            return entries
+            return block_entries
 
         if filter_id in self._pending_transaction_filters:
-            entries = self._pending_transaction_filters[filter_id]
+            tx_entries = self._pending_transaction_filters[filter_id]
             self._pending_transaction_filters[filter_id] = []
-            return entries
+            return tx_entries
 
         if filter_id in self._log_filters:
             log_entries = self._log_filter_entries[filter_id]
             self._log_filter_entries[filter_id] = []
             return log_entries
 
         raise FilterNotFound("Unknown filter id")
```

### Comparing `alysis-0.4.0/alysis/_rpc.py` & `alysis-0.5.0/alysis/_rpc.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,73 +1,37 @@
 """RPC-like API, mimicking the behavior of major Ethereum providers."""
 
-from enum import Enum
 from typing import cast
 
 from compages import StructuringError, UnstructuringError
-
-from ._exceptions import (
-    BlockNotFound,
-    TransactionFailed,
-    TransactionNotFound,
-    TransactionReverted,
-    ValidationError,
-)
-from ._node import Node
-from .schema import (
+from ethereum_rpc import (
     JSON,
     Address,
     Block,
+    BlockHash,
     EstimateGasParams,
     EthCallParams,
     FilterParams,
     FilterParamsEIP234,
-    Hash32,
     LogEntry,
+    RPCError,
+    RPCErrorCode,
+    TxHash,
     structure,
     unstructure,
 )
 
-
-class RPCErrorCode(Enum):
-    """Known RPC error codes returned by providers."""
-
-    SERVER_ERROR = -32000
-    """Reserved for implementation-defined server-errors. See the message for details."""
-
-    METHOD_NOT_FOUND = -32601
-    """The method does not exist / is not available."""
-
-    INVALID_PARAMETER = -32602
-    """Invalid method parameter(s)."""
-
-    EXECUTION_ERROR = 3
-    """Contract transaction failed during execution. See the data for details."""
-
-
-class RPCError(Exception):
-    """
-    An exception raised in case of a known error, that is something that would be returned as
-    ``"error": {"code": ..., "message": ..., "data": ...}`` sub-dictionary in an RPC response.
-    """
-
-    code: int
-    """The error type."""
-
-    message: str
-    """The associated message."""
-
-    data: None | bytes
-    """The associated hex-encoded data (if any)."""
-
-    def __init__(self, code: RPCErrorCode, message: str, data: None | bytes = None):
-        super().__init__(f"Error {code}: {message}")
-        self.code = code.value
-        self.message = message
-        self.data = data
+from ._exceptions import (
+    BlockNotFound,
+    TransactionFailed,
+    TransactionNotFound,
+    TransactionReverted,
+    ValidationError,
+)
+from ._node import Node
 
 
 class RPCNode:
     """
     A wrapper for :py:class:`Node` exposing an RPC-like interface,
     taking and returning JSON-compatible data structures.
     """
@@ -97,31 +61,33 @@
             eth_getLogs=self._eth_get_logs,
             eth_getFilterLogs=self._eth_get_filter_logs,
         )
 
     def rpc(self, method_name: str, *params: JSON) -> JSON:
         """
         Makes an RPC request to the chain and returns the result on success,
-        or raises :py:class:`RPCError` on failure.
+        or raises :py:class:`ethereum_rpc.RPCError` on failure.
         """
         if method_name not in self._methods:
-            raise RPCError(RPCErrorCode.METHOD_NOT_FOUND, f"Unknown method: {method_name}")
+            raise RPCError.with_code(
+                RPCErrorCode.METHOD_NOT_FOUND, f"Unknown method: {method_name}"
+            )
 
         try:
             return self._methods[method_name](params)
 
         except (BlockNotFound, TransactionNotFound) as exc:
             # If we didn't process it earlier, it's a SERVER_ERROR
-            raise RPCError(RPCErrorCode.SERVER_ERROR, str(exc)) from exc
+            raise RPCError.with_code(RPCErrorCode.SERVER_ERROR, str(exc)) from exc
 
         except (StructuringError, ValidationError) as exc:
-            raise RPCError(RPCErrorCode.INVALID_PARAMETER, str(exc)) from exc
+            raise RPCError.with_code(RPCErrorCode.INVALID_PARAMETER, str(exc)) from exc
 
         except UnstructuringError as exc:
-            raise RPCError(RPCErrorCode.SERVER_ERROR, str(exc)) from exc
+            raise RPCError.with_code(RPCErrorCode.SERVER_ERROR, str(exc)) from exc
 
         except TransactionReverted as exc:
             reason_data = exc.args[0]
 
             if reason_data == b"":
                 # Empty `revert()`, or `require()` without a message.
 
@@ -133,18 +99,18 @@
                 data = None
 
             else:
                 error = RPCErrorCode.EXECUTION_ERROR
                 message = "execution reverted"
                 data = reason_data
 
-            raise RPCError(error, message, data) from exc
+            raise RPCError.with_code(error, message, data) from exc
 
         except TransactionFailed as exc:
-            raise RPCError(RPCErrorCode.SERVER_ERROR, exc.args[0]) from exc
+            raise RPCError.with_code(RPCErrorCode.SERVER_ERROR, exc.args[0]) from exc
 
     def _net_version(self, params: tuple[JSON, ...]) -> JSON:
         _ = structure(tuple[()], params)
         # Note: it's not hex encoded, but just stringified!
         return str(self.node.net_version())
 
     def _eth_chain_id(self, params: tuple[JSON, ...]) -> JSON:
@@ -174,15 +140,15 @@
         return unstructure(self.node.eth_get_storage_at(address, slot, block))
 
     def _eth_get_transaction_count(self, params: tuple[JSON, ...]) -> JSON:
         address, block = cast(tuple[Address, Block], structure(tuple[Address, Block], params))
         return unstructure(self.node.eth_get_transaction_count(address, block))
 
     def _eth_get_transaction_by_hash(self, params: tuple[JSON, ...]) -> JSON:
-        (transaction_hash,) = cast(tuple[Hash32], structure(tuple[Hash32], params))
+        (transaction_hash,) = cast(tuple[TxHash], structure(tuple[TxHash], params))
         try:
             transaction = self.node.eth_get_transaction_by_hash(transaction_hash)
         except TransactionNotFound:
             return None
         return unstructure(transaction)
 
     def _eth_get_block_by_number(self, params: tuple[JSON, ...]) -> JSON:
@@ -193,27 +159,27 @@
             )
         except BlockNotFound:
             return None
         return unstructure(block_info)
 
     def _eth_get_block_by_hash(self, params: tuple[JSON, ...]) -> JSON:
         block_hash, with_transactions = cast(
-            tuple[Hash32, bool],
-            structure(tuple[Hash32, bool], params),
+            tuple[BlockHash, bool],
+            structure(tuple[BlockHash, bool], params),
         )
         try:
             block_info = self.node.eth_get_block_by_hash(
                 block_hash, with_transactions=with_transactions
             )
         except BlockNotFound:
             return None
         return unstructure(block_info)
 
     def _eth_get_transaction_receipt(self, params: tuple[JSON, ...]) -> JSON:
-        (transaction_hash,) = cast(tuple[Hash32], structure(tuple[Hash32], params))
+        (transaction_hash,) = cast(tuple[TxHash], structure(tuple[TxHash], params))
         try:
             receipt = self.node.eth_get_transaction_receipt(transaction_hash)
         except TransactionNotFound:
             return None
         return unstructure(receipt)
 
     def _eth_send_raw_transaction(self, params: tuple[JSON, ...]) -> JSON:
@@ -249,15 +215,16 @@
     def _eth_new_filter(self, params: tuple[JSON, ...]) -> JSON:
         (typed_params,) = cast(tuple[FilterParams], structure(tuple[FilterParams], params))
         return unstructure(self.node.eth_new_filter(typed_params))
 
     def _eth_get_filter_changes(self, params: tuple[JSON, ...]) -> JSON:
         (filter_id,) = cast(tuple[int], structure(tuple[int], params))
         return unstructure(
-            self.node.eth_get_filter_changes(filter_id), list[LogEntry] | list[Hash32]
+            self.node.eth_get_filter_changes(filter_id),
+            list[LogEntry] | list[TxHash] | list[BlockHash],
         )
 
     def _eth_get_filter_logs(self, params: tuple[JSON, ...]) -> JSON:
         (filter_id,) = cast(tuple[int], structure(tuple[int], params))
         return unstructure(self.node.eth_get_filter_logs(filter_id), list[LogEntry])
 
     def _eth_get_logs(self, params: tuple[JSON, ...]) -> JSON:
```

### Comparing `alysis-0.4.0/docs/Makefile` & `alysis-0.5.0/docs/Makefile`

 * *Files identical despite different names*

### Comparing `alysis-0.4.0/docs/changelog.rst` & `alysis-0.5.0/docs/changelog.rst`

 * *Files 22% similar despite different names*

```diff
@@ -1,21 +1,36 @@
 Changelog
 =========
 
+
+0.5.0 (2024-05-28)
+------------------
+
+Changed
+^^^^^^^
+
+- Bump ``py-evm`` to 0.10.1b1. (PR_24_)
+- Using ``ethereum-rpc`` types. (PR_25_)
+
+
+.. _PR_24: https://github.com/fjarri-eth/alsyis/pull/24
+.. _PR_25: https://github.com/fjarri-eth/alsyis/pull/25
+
+
 0.4.0 (2024-03-15)
 ------------------
 
 Changed
 ^^^^^^^
 
 - ``RPCError.data`` is now ``None | bytes`` instead of ``None | str``. (PR_23_)
 - ``compages`` dependency bumped to 0.3. (PR_23_)
 
 
-.. _PR_23: https://github.com/fjarri/compages/pull/23
+.. _PR_23: https://github.com/fjarri-eth/alsyis/pull/23
 
 
 0.3.0 (2024-03-09)
 ------------------
 
 Changed
 ^^^^^^^
@@ -38,23 +53,23 @@
 ^^^^^
 
 - Process transaction validation errors and missing method errors correctly on RPC level. (PR_20_)
 - Correctly mismatch if there are more topics in the filter than there is in the log entry. (PR_22_)
 - Calculate ``BlockInfo.total_difficulty`` correctly. (PR_22_)
 
 
-.. _PR_18: https://github.com/fjarri/compages/pull/18
-.. _PR_20: https://github.com/fjarri/compages/pull/20
-.. _PR_21: https://github.com/fjarri/compages/pull/21
-.. _PR_22: https://github.com/fjarri/compages/pull/22
+.. _PR_18: https://github.com/fjarri-eth/alsyis/pull/18
+.. _PR_20: https://github.com/fjarri-eth/alsyis/pull/20
+.. _PR_21: https://github.com/fjarri-eth/alsyis/pull/21
+.. _PR_22: https://github.com/fjarri-eth/alsyis/pull/22
 
 
 0.2.0 (2024-03-05)
 ------------------
 
 Changed
 ^^^^^^^
 
 - Minimum Python version bumped to 3.10. (PR_4_)
 
 
-.. _PR_4: https://github.com/fjarri/compages/pull/4
+.. _PR_4: https://github.com/fjarri-eth/alsyis/pull/4
```

### Comparing `alysis-0.4.0/docs/conf.py` & `alysis-0.5.0/docs/conf.py`

 * *Files 23% similar despite different names*

```diff
@@ -38,20 +38,18 @@
 # extensions coming with Sphinx (named 'sphinx.ext.*') or your custom
 # ones.
 extensions = [
     "sphinx.ext.autodoc",
     "sphinx.ext.intersphinx",
     "sphinx.ext.doctest",
     "sphinx.ext.viewcode",
-    "enum_tools.autoenum",
 ]
 
 autoclass_content = "both"
 autodoc_member_order = "groupwise"
-autodoc_type_aliases = {"JSON": "JSON"}
 
 # Add any paths that contain templates here, relative to this directory.
 templates_path = []
 
 # List of patterns, relative to source directory, that match files and
 # directories to ignore when looking for source files.
 # This pattern also affects html_static_path and html_extra_path.
@@ -71,8 +69,9 @@
 html_static_path = []
 
 # Do not prepend module to type names when it can be resolved.
 python_use_unqualified_type_names = True
 
 intersphinx_mapping = {
     "python": ("https://docs.python.org/3", None),
+    "ethereum_rpc": ("https://ethereum-rpc.readthedocs.io/en/v0.1.0", None),
 }
```

### Comparing `alysis-0.4.0/pyproject.toml` & `alysis-0.5.0/pyproject.toml`

 * *Files 3% similar despite different names*

```diff
@@ -1,49 +1,49 @@
 [project]
 name = "alysis"
-version = "0.4.0"
+version = "0.5.0"
 description = "Ethereum testerchain"
 authors = [
     { name = "Bogdan Opanchuk", email = "bogdan@opanchuk.net" },
 ]
 dependencies = [
     "eth-utils>=3",
     "setuptools",
-    "py-evm==0.9.0b1",
+    "py-evm==0.10.1b1",
     "eth-typing>=4",
     "eth-keys>=0.5",
     "rlp>=4",
     "compages>=0.3.0",
+    "ethereum-rpc>=0.1",
 ]
 requires-python = ">=3.10"
 classifiers = [
     "Development Status :: 4 - Beta",
     "Programming Language :: Python :: 3",
     "License :: OSI Approved :: MIT License",
     "Operating System :: OS Independent",
 ]
 readme = "README.md"
 
 [project.license]
 file = "LICENSE.md"
 
 [project.urls]
-homepage = "https://github.com/fjarri/alysis"
+homepage = "https://github.com/fjarri-eth/alysis"
 
 [project.optional-dependencies]
 tests = [
     "pytest>=6",
     "pytest-cov",
-    "eth-account>=0.6",
+    "eth-account>=0.13",
 ]
 docs = [
     "sphinx>=4",
     "furo",
     "setuptools-scm",
-    "enum-tools[sphinx]",
 ]
 lint = [
     "mypy>=1.4",
     "ruff>=0.2",
 ]
 
 [tool.pdm.version]
@@ -114,14 +114,19 @@
     "dist",
 ]
 dummy-variable-rgx = "^(_+|(_+[a-zA-Z0-9_]*[a-zA-Z0-9]+?))$"
 
 [tool.ruff.lint.pyupgrade]
 keep-runtime-typing = true
 
+[tool.ruff.lint.isort]
+known-first-party = [
+    "alysis",
+]
+
 [tool.ruff.lint.per-file-ignores]
 
 [build-system]
 requires = [
     "pdm-pep517",
 ]
 build-backend = "pdm.pep517.api"
```

### Comparing `alysis-0.4.0/tests/test_rpc.py` & `alysis-0.5.0/tests/test_rpc.py`

 * *Files 17% similar despite different names*

```diff
@@ -5,13 +5,13 @@
         "to": another_account.address,
         "value": hex(10**9),
         "gas": hex(21000),
         "maxFeePerGas": rpc_node.rpc("eth_gasPrice"),
         "maxPriorityFeePerGas": hex(10**9),
         "nonce": hex(0),
     }
-    signed_tx = root_account.sign_transaction(tx).rawTransaction
+    signed_tx = root_account.sign_transaction(tx).raw_transaction
 
-    rpc_node.rpc("eth_sendRawTransaction", signed_tx.hex())
+    rpc_node.rpc("eth_sendRawTransaction", "0x" + signed_tx.hex())
 
     result = rpc_node.rpc("eth_getBalance", another_account.address, "latest")
     assert result == hex(10**9)
```

### Comparing `alysis-0.4.0/PKG-INFO` & `alysis-0.5.0/PKG-INFO`

 * *Files 10% similar despite different names*

```diff
@@ -1,21 +1,21 @@
 Metadata-Version: 2.1
 Name: alysis
-Version: 0.4.0
+Version: 0.5.0
 Summary: Ethereum testerchain
 Author-email: Bogdan Opanchuk <bogdan@opanchuk.net>
 Requires-Python: >=3.10
 Classifier: Development Status :: 4 - Beta
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python :: 3
 Provides-Extra: docs
 Provides-Extra: lint
 Provides-Extra: tests
-Project-URL: homepage, https://github.com/fjarri/alysis
+Project-URL: homepage, https://github.com/fjarri-eth/alysis
 Description-Content-Type: text/markdown
 
 Alysis, an Ethereum testerchain
 ===============================
 
 [![pypi package][pypi-image]][pypi-link] ![License][pypi-license-image] [![Docs][rtd-image]][rtd-link] [![Coverage][cov-image]][cov-link]
 
@@ -25,10 +25,10 @@
 
 
 [pypi-image]: https://img.shields.io/pypi/v/alysis
 [pypi-link]: https://pypi.org/project/alysis/
 [pypi-license-image]: https://img.shields.io/pypi/l/alysis
 [rtd-image]: https://readthedocs.org/projects/alysis/badge/?version=latest
 [rtd-link]: https://alysis.readthedocs.io/en/latest/
-[cov-image]: https://codecov.io/gh/fjarri/alysis/branch/master/graph/badge.svg?token=RZP1LK1HB2
-[cov-link]: https://codecov.io/gh/fjarri/alysis
+[cov-image]: https://codecov.io/gh/fjarri-eth/alysis/branch/master/graph/badge.svg?token=RZP1LK1HB2
+[cov-link]: https://codecov.io/gh/fjarri-eth/alysis
```

