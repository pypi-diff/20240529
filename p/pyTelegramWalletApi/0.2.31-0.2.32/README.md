# Comparing `tmp/pyTelegramWalletApi-0.2.31.tar.gz` & `tmp/pyTelegramWalletApi-0.2.32.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pyTelegramWalletApi-0.2.31.tar", last modified: Thu May 23 16:31:08 2024, max compression
+gzip compressed data, was "pyTelegramWalletApi-0.2.32.tar", last modified: Wed May 29 14:22:39 2024, max compression
```

## Comparing `pyTelegramWalletApi-0.2.31.tar` & `pyTelegramWalletApi-0.2.32.tar`

### file list

```diff
@@ -1,26 +1,26 @@
-drwxrwxrwx   0        0        0        0 2024-05-23 16:31:08.462126 pyTelegramWalletApi-0.2.31/
--rw-rw-rw-   0        0        0     4829 2024-05-23 16:31:08.462126 pyTelegramWalletApi-0.2.31/PKG-INFO
--rw-rw-rw-   0        0        0     4620 2024-05-20 02:37:51.000000 pyTelegramWalletApi-0.2.31/README.md
-drwxrwxrwx   0        0        0        0 2024-05-23 16:31:08.422129 pyTelegramWalletApi-0.2.31/pyTelegramWalletApi.egg-info/
--rw-rw-rw-   0        0        0     4829 2024-05-23 16:31:08.000000 pyTelegramWalletApi-0.2.31/pyTelegramWalletApi.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      481 2024-05-23 16:31:08.000000 pyTelegramWalletApi-0.2.31/pyTelegramWalletApi.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-05-23 16:31:08.000000 pyTelegramWalletApi-0.2.31/pyTelegramWalletApi.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       30 2024-05-23 16:31:08.000000 pyTelegramWalletApi-0.2.31/pyTelegramWalletApi.egg-info/requires.txt
--rw-rw-rw-   0        0        0       13 2024-05-23 16:31:08.000000 pyTelegramWalletApi-0.2.31/pyTelegramWalletApi.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2024-05-23 16:31:08.465128 pyTelegramWalletApi-0.2.31/setup.cfg
--rw-rw-rw-   0        0        0      572 2024-05-23 16:29:37.000000 pyTelegramWalletApi-0.2.31/setup.py
-drwxrwxrwx   0        0        0        0 2024-05-23 16:31:08.434130 pyTelegramWalletApi-0.2.31/tests/
--rw-rw-rw-   0        0        0        0 2023-10-02 22:55:55.000000 pyTelegramWalletApi-0.2.31/tests/__init__.py
--rw-rw-rw-   0        0        0      902 2024-05-20 02:37:51.000000 pyTelegramWalletApi-0.2.31/tests/test_account.py
--rw-rw-rw-   0        0        0     2680 2024-05-20 02:37:51.000000 pyTelegramWalletApi-0.2.31/tests/test_p2p.py
--rw-rw-rw-   0        0        0      733 2024-05-20 02:37:51.000000 pyTelegramWalletApi-0.2.31/tests/utils.py
-drwxrwxrwx   0        0        0        0 2024-05-23 16:31:08.439128 pyTelegramWalletApi-0.2.31/wallet/
--rw-rw-rw-   0        0        0       70 2023-10-02 23:59:27.000000 pyTelegramWalletApi-0.2.31/wallet/__init__.py
-drwxrwxrwx   0        0        0        0 2024-05-23 16:31:08.442127 pyTelegramWalletApi-0.2.31/wallet/rest/
--rw-rw-rw-   0        0        0    18205 2024-05-20 02:37:51.000000 pyTelegramWalletApi-0.2.31/wallet/rest/__init__.py
-drwxrwxrwx   0        0        0        0 2024-05-23 16:31:08.458127 pyTelegramWalletApi-0.2.31/wallet/types/
--rw-rw-rw-   0        0        0      184 2024-05-20 02:37:51.000000 pyTelegramWalletApi-0.2.31/wallet/types/__init__.py
--rw-rw-rw-   0        0        0      975 2024-05-20 02:37:51.000000 pyTelegramWalletApi-0.2.31/wallet/types/balances.py
--rw-rw-rw-   0        0        0     4987 2024-05-20 02:37:51.000000 pyTelegramWalletApi-0.2.31/wallet/types/offers.py
--rw-rw-rw-   0        0        0     3128 2024-05-20 02:37:51.000000 pyTelegramWalletApi-0.2.31/wallet/types/transactions.py
--rw-rw-rw-   0        0        0     4530 2024-05-23 16:26:30.000000 pyTelegramWalletApi-0.2.31/wallet/web_client.py
+drwxrwxrwx   0        0        0        0 2024-05-29 14:22:39.471553 pyTelegramWalletApi-0.2.32/
+-rw-rw-rw-   0        0        0     4829 2024-05-29 14:22:39.471553 pyTelegramWalletApi-0.2.32/PKG-INFO
+-rw-rw-rw-   0        0        0     4620 2024-05-20 02:37:51.000000 pyTelegramWalletApi-0.2.32/README.md
+drwxrwxrwx   0        0        0        0 2024-05-29 14:22:39.434878 pyTelegramWalletApi-0.2.32/pyTelegramWalletApi.egg-info/
+-rw-rw-rw-   0        0        0     4829 2024-05-29 14:22:39.000000 pyTelegramWalletApi-0.2.32/pyTelegramWalletApi.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      481 2024-05-29 14:22:39.000000 pyTelegramWalletApi-0.2.32/pyTelegramWalletApi.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-05-29 14:22:39.000000 pyTelegramWalletApi-0.2.32/pyTelegramWalletApi.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       30 2024-05-29 14:22:39.000000 pyTelegramWalletApi-0.2.32/pyTelegramWalletApi.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       13 2024-05-29 14:22:39.000000 pyTelegramWalletApi-0.2.32/pyTelegramWalletApi.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2024-05-29 14:22:39.474027 pyTelegramWalletApi-0.2.32/setup.cfg
+-rw-rw-rw-   0        0        0      572 2024-05-29 14:22:24.000000 pyTelegramWalletApi-0.2.32/setup.py
+drwxrwxrwx   0        0        0        0 2024-05-29 14:22:39.449391 pyTelegramWalletApi-0.2.32/tests/
+-rw-rw-rw-   0        0        0        0 2023-10-02 22:55:55.000000 pyTelegramWalletApi-0.2.32/tests/__init__.py
+-rw-rw-rw-   0        0        0      889 2024-05-29 13:58:29.000000 pyTelegramWalletApi-0.2.32/tests/test_account.py
+-rw-rw-rw-   0        0        0     2680 2024-05-20 02:37:51.000000 pyTelegramWalletApi-0.2.32/tests/test_p2p.py
+-rw-rw-rw-   0        0        0      733 2024-05-20 02:37:51.000000 pyTelegramWalletApi-0.2.32/tests/utils.py
+drwxrwxrwx   0        0        0        0 2024-05-29 14:22:39.455171 pyTelegramWalletApi-0.2.32/wallet/
+-rw-rw-rw-   0        0        0       70 2023-10-02 23:59:27.000000 pyTelegramWalletApi-0.2.32/wallet/__init__.py
+drwxrwxrwx   0        0        0        0 2024-05-29 14:22:39.457525 pyTelegramWalletApi-0.2.32/wallet/rest/
+-rw-rw-rw-   0        0        0    18233 2024-05-29 14:14:05.000000 pyTelegramWalletApi-0.2.32/wallet/rest/__init__.py
+drwxrwxrwx   0        0        0        0 2024-05-29 14:22:39.469043 pyTelegramWalletApi-0.2.32/wallet/types/
+-rw-rw-rw-   0        0        0      180 2024-05-29 13:46:15.000000 pyTelegramWalletApi-0.2.32/wallet/types/__init__.py
+-rw-rw-rw-   0        0        0      975 2024-05-20 02:37:51.000000 pyTelegramWalletApi-0.2.32/wallet/types/balances.py
+-rw-rw-rw-   0        0        0     4987 2024-05-20 02:37:51.000000 pyTelegramWalletApi-0.2.32/wallet/types/offers.py
+-rw-rw-rw-   0        0        0     2740 2024-05-29 14:19:14.000000 pyTelegramWalletApi-0.2.32/wallet/types/transactions.py
+-rw-rw-rw-   0        0        0     4524 2024-05-23 22:04:37.000000 pyTelegramWalletApi-0.2.32/wallet/web_client.py
```

### Comparing `pyTelegramWalletApi-0.2.31/PKG-INFO` & `pyTelegramWalletApi-0.2.32/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pyTelegramWalletApi
-Version: 0.2.31
+Version: 0.2.32
 Summary: Telegram Wallet API
 Author: no-name-user-name
 Author-email: dimazver61@gmail.com
 Description-Content-Type: text/markdown
 
 <br/>
 <p align="center">
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: pyTelegramWalletApi Version: 0.2.31 Summary:
+Metadata-Version: 2.1 Name: pyTelegramWalletApi Version: 0.2.32 Summary:
 Telegram Wallet API Author: no-name-user-name Author-email:
 dimazver61@gmail.com Description-Content-Type: text/markdown
                                     _[_L_o_g_o_]
                          ******** TTeelleeggrraamm WWaalllleett AAPPII ********
          Unofficial library for managing your personal Wallet account
 
 ## Table Of Contents * [About the Project](#about-the-project) * [Built With]
```

### Comparing `pyTelegramWalletApi-0.2.31/README.md` & `pyTelegramWalletApi-0.2.32/README.md`

 * *Files identical despite different names*

### Comparing `pyTelegramWalletApi-0.2.31/pyTelegramWalletApi.egg-info/PKG-INFO` & `pyTelegramWalletApi-0.2.32/pyTelegramWalletApi.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pyTelegramWalletApi
-Version: 0.2.31
+Version: 0.2.32
 Summary: Telegram Wallet API
 Author: no-name-user-name
 Author-email: dimazver61@gmail.com
 Description-Content-Type: text/markdown
 
 <br/>
 <p align="center">
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: pyTelegramWalletApi Version: 0.2.31 Summary:
+Metadata-Version: 2.1 Name: pyTelegramWalletApi Version: 0.2.32 Summary:
 Telegram Wallet API Author: no-name-user-name Author-email:
 dimazver61@gmail.com Description-Content-Type: text/markdown
                                     _[_L_o_g_o_]
                          ******** TTeelleeggrraamm WWaalllleett AAPPII ********
          Unofficial library for managing your personal Wallet account
 
 ## Table Of Contents * [About the Project](#about-the-project) * [Built With]
```

### Comparing `pyTelegramWalletApi-0.2.31/tests/test_account.py` & `pyTelegramWalletApi-0.2.32/tests/test_account.py`

 * *Files 3% similar despite different names*

```diff
@@ -12,15 +12,15 @@
     check_api_update(
         w.get_user_balances(currency='TON')
     )
 
 
 def test_get_transactions():
     txs = w.get_transactions()
-    assert isinstance(txs.size, int)
+    assert len(txs) > 0
 
 
 def test_get_transaction_details():
     check_api_update(
         w.get_transaction_details(tx_id=49159406)
     )
```

### Comparing `pyTelegramWalletApi-0.2.31/tests/test_p2p.py` & `pyTelegramWalletApi-0.2.32/tests/test_p2p.py`

 * *Files identical despite different names*

### Comparing `pyTelegramWalletApi-0.2.31/tests/utils.py` & `pyTelegramWalletApi-0.2.32/tests/utils.py`

 * *Files identical despite different names*

### Comparing `pyTelegramWalletApi-0.2.31/wallet/rest/__init__.py` & `pyTelegramWalletApi-0.2.32/wallet/rest/__init__.py`

 * *Files 3% similar despite different names*

```diff
@@ -99,32 +99,32 @@
             for a in balances.accounts:
                 if a.currency == currency:
                     return a
         else:
             return balances
 
     def get_transactions(self, limit: int = 20, last_id: int = None, crypto_currency: str = None,
-                         transaction_type: str = None, transaction_gateway: str = None) -> TxResponse:
+                         transaction_type: str = None, transaction_gateway: str = None) -> list[TxDetails]:
         """ Account in withdraw | deposit txs
 
         :param transaction_gateway: withdraw_onchain | tg_transfer | top_up | p2p_order | earn | internal
         :param transaction_type: withdraw | deposit
         :param crypto_currency: BTC USDT TON NOT
         :param limit:
         :param last_id:
         :return:
         """
         params = {
-            limit: limit,
-            last_id: last_id,
-            crypto_currency: crypto_currency,
-            transaction_type: transaction_type,
-            transaction_gateway: transaction_gateway
+            'limit': limit,
+            'last_id': last_id,
+            'crypto_currency': crypto_currency,
+            'transaction_type': transaction_type,
+            'transaction_gateway': transaction_gateway
         }
-        return TxResponse.from_dict(self.request(f'transactions/', params=params))
+        return TxResponse.from_dict(self.request(f'transactions/', params=params)).transactions
 
     def get_transaction_details(self, tx_id: int) -> TxDetails:
         """ One tx info
 
         :param tx_id:
         :return:
         """
```

### Comparing `pyTelegramWalletApi-0.2.31/wallet/types/balances.py` & `pyTelegramWalletApi-0.2.32/wallet/types/balances.py`

 * *Files identical despite different names*

### Comparing `pyTelegramWalletApi-0.2.31/wallet/types/offers.py` & `pyTelegramWalletApi-0.2.32/wallet/types/offers.py`

 * *Files identical despite different names*

### Comparing `pyTelegramWalletApi-0.2.31/wallet/types/transactions.py` & `pyTelegramWalletApi-0.2.32/wallet/types/transactions.py`

 * *Files 17% similar despite different names*

```diff
@@ -22,38 +22,57 @@
     has_transactions: bool
     addresses: list[AccountAddress]
     unknown_things: CatchAll = None
 
 
 @dataclass_json(undefined=Undefined.INCLUDE)
 @dataclass
-class Tx:
+class TxDetails:
     id: int
-    type: str
-    created_at: str
-    amount: int
-    currency: str
-    status: str
-    gateway: str
-    username: str
-    tg_id: int
-    mention: str
-    input_addresses: str | None
-    recipient_wallet_address: str | None
-    # activated_amount: float
-    # remaining_amount: float
-    # purchase_external_id: int
-    photo_url: str
-    # details_for_user: None
-    pair_transaction_amount: int
-    pair_transaction_currency: str
-    is_blocked: bool
-    # block: str
-    is_cancellable: bool
-    network: str | None
+    type: str | None = None
+    created_at: str | None = None
+    crypto_amount: float | None = None
+    fiat_amount: float | None = None
+    crypto_currency: str | None = None
+    fiat_currency: str | None = None
+    value_at_time: float | None = None
+    username: str | None = None
+    tg_id: int | None = None
+    mention: str | None = None
+    status: str | None = None
+    gateway: str | None = None
+    input_addresses: str | None = None
+    recipient_wallet_address: str | None = None
+    transaction_link: str | None = None
+    full_number_of_activations: int | None = None
+    number_of_activations: int | None = None
+    amount_of_activations: float | None = None
+    remaining_amount: float | None = None
+    fee_currency: str | None = None
+    fee_amount: float | None = None
+    activation_channel_title: str | None = None
+    activation_channel_name: str | None = None
+    check_url: str | None = None
+    seller: str | None = None
+    buyer: str | None = None
+    avatar_code: str | None = None
+    entity_id: int | None = None
+    photo_url: str | None = None
+    details_for_user: str | None = None
+    pair_transaction_amount: float | None = None
+    pair_transaction_currency: str | None = None
+    is_blocked: str | None = None
+    block: str | None = None
+    is_cancellable: bool | None = None
+    comment: str | None = None
+    giveaway_gift: str | None = None
+    network: str | None = None
+    amount: int | None = None
+    activated_amount: int | None = None
+    currency: str | None = None
     unknown_things: CatchAll = None
 
     @staticmethod
     def to_dict():
         pass
 
     @staticmethod
@@ -61,70 +80,17 @@
         pass
 
 
 @dataclass_json(undefined=Undefined.INCLUDE)
 @dataclass
 class TxResponse:
     limit: int
-    offset: int
     size: int
-    transactions: list[Tx]
-    unknown_things: CatchAll = None
-
-    @staticmethod
-    def to_dict():
-        pass
-
-    @staticmethod
-    def from_dict(data):
-        pass
-
-
-@dataclass_json(undefined=Undefined.INCLUDE)
-@dataclass
-class TxDetails:
-    id: int
-    type: str | None
-    created_at: str | None
-    crypto_amount: float | None
-    fiat_amount: float | None
-    crypto_currency: str | None
-    fiat_currency: str | None
-    value_at_time: float | None
-    username: str | None
-    tg_id: int | None
-    mention: str | None
-    status: str | None
-    gateway: str | None
-    input_addresses: str | None
-    recipient_wallet_address: str | None
-    transaction_link: str | None
-    full_number_of_activations: int | None
-    number_of_activations: int | None
-    amount_of_activations: float | None
-    remaining_amount: float | None
-    fee_currency: str | None
-    fee_amount: float | None
-    activation_channel_title: str | None
-    activation_channel_name: str | None
-    check_url: str | None
-    seller: str | None
-    buyer: str | None
-    avatar_code: str | None
-    entity_id: int | None
-    photo_url: str | None
-    details_for_user: str | None
-    pair_transaction_amount: float | None
-    pair_transaction_currency: str | None
-    is_blocked: str | None
-    block: str | None
-    is_cancellable: bool
-    comment: str | None
-    giveaway_gift: str | None
-    network: str | None
+    transactions: list[TxDetails]
+    offset: int = None
     unknown_things: CatchAll = None
 
     @staticmethod
     def to_dict():
         pass
 
     @staticmethod
```

### Comparing `pyTelegramWalletApi-0.2.31/wallet/web_client.py` & `pyTelegramWalletApi-0.2.32/wallet/web_client.py`

 * *Files 0% similar despite different names*

```diff
@@ -59,17 +59,14 @@
                     return c
                 else:
                     time.sleep(1)
 
         except Exception as e:
             pass
 
-
-
-
     def _parse_token(self, wallet_endpoint):
         try:
             iframe = WebDriverWait(self.driver, 10).until(
                 EC.presence_of_element_located((By.TAG_NAME, 'iframe'))
             )
         except Exception as e:
             raise Exception('Iframe not find! Try start client with attr "headless"=True to recognize problem')
```

