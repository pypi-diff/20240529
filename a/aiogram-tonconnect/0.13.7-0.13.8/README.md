# Comparing `tmp/aiogram-tonconnect-0.13.7.tar.gz` & `tmp/aiogram-tonconnect-0.13.8.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "aiogram-tonconnect-0.13.7.tar", last modified: Mon May 27 04:28:08 2024, max compression
+gzip compressed data, was "aiogram-tonconnect-0.13.8.tar", last modified: Wed May 29 16:37:36 2024, max compression
```

## Comparing `aiogram-tonconnect-0.13.7.tar` & `aiogram-tonconnect-0.13.8.tar`

### file list

```diff
@@ -1,43 +1,43 @@
-drwxrwxr-x   0 ness      (1000) ness      (1000)        0 2024-05-27 04:28:08.939554 aiogram-tonconnect-0.13.7/
--rw-rw-r--   0 ness      (1000) ness      (1000)     1064 2024-03-27 17:06:19.000000 aiogram-tonconnect-0.13.7/LICENSE
--rw-r--r--   0 ness      (1000) ness      (1000)     5438 2024-05-27 04:28:08.939554 aiogram-tonconnect-0.13.7/PKG-INFO
--rw-rw-r--   0 ness      (1000) ness      (1000)     4458 2024-03-27 17:06:19.000000 aiogram-tonconnect-0.13.7/README.md
-drwxrwxr-x   0 ness      (1000) ness      (1000)        0 2024-05-27 04:28:08.935554 aiogram-tonconnect-0.13.7/aiogram_tonconnect/
--rw-rw-r--   0 ness      (1000) ness      (1000)       65 2024-03-27 17:06:19.000000 aiogram-tonconnect-0.13.7/aiogram_tonconnect/__init__.py
--rw-rw-r--   0 ness      (1000) ness      (1000)     6377 2024-03-27 17:06:19.000000 aiogram-tonconnect-0.13.7/aiogram_tonconnect/handlers.py
--rw-rw-r--   0 ness      (1000) ness      (1000)    20809 2024-05-27 04:26:10.000000 aiogram-tonconnect-0.13.7/aiogram_tonconnect/manager.py
--rw-rw-r--   0 ness      (1000) ness      (1000)     5253 2024-05-19 12:46:38.000000 aiogram-tonconnect-0.13.7/aiogram_tonconnect/middleware.py
-drwxrwxr-x   0 ness      (1000) ness      (1000)        0 2024-05-27 04:28:08.935554 aiogram-tonconnect-0.13.7/aiogram_tonconnect/tonconnect/
--rw-rw-r--   0 ness      (1000) ness      (1000)      140 2024-03-27 17:06:19.000000 aiogram-tonconnect-0.13.7/aiogram_tonconnect/tonconnect/__init__.py
--rw-rw-r--   0 ness      (1000) ness      (1000)     7608 2024-03-27 17:06:19.000000 aiogram-tonconnect-0.13.7/aiogram_tonconnect/tonconnect/models.py
--rw-rw-r--   0 ness      (1000) ness      (1000)     7469 2024-03-30 13:07:39.000000 aiogram-tonconnect-0.13.7/aiogram_tonconnect/tonconnect/provider.py
-drwxrwxr-x   0 ness      (1000) ness      (1000)        0 2024-05-27 04:28:08.935554 aiogram-tonconnect-0.13.7/aiogram_tonconnect/tonconnect/storage/
--rw-rw-r--   0 ness      (1000) ness      (1000)      300 2024-03-27 17:06:19.000000 aiogram-tonconnect-0.13.7/aiogram_tonconnect/tonconnect/storage/__init__.py
--rw-rw-r--   0 ness      (1000) ness      (1000)     2047 2024-03-27 17:06:19.000000 aiogram-tonconnect-0.13.7/aiogram_tonconnect/tonconnect/storage/base.py
--rw-rw-r--   0 ness      (1000) ness      (1000)     2247 2024-03-27 17:06:19.000000 aiogram-tonconnect-0.13.7/aiogram_tonconnect/tonconnect/storage/callback.py
--rw-rw-r--   0 ness      (1000) ness      (1000)     1214 2024-03-27 17:06:19.000000 aiogram-tonconnect-0.13.7/aiogram_tonconnect/tonconnect/storage/session.py
--rw-rw-r--   0 ness      (1000) ness      (1000)     1078 2024-03-27 17:06:19.000000 aiogram-tonconnect-0.13.7/aiogram_tonconnect/tonconnect/storage/task.py
--rw-rw-r--   0 ness      (1000) ness      (1000)     2197 2024-03-30 13:09:49.000000 aiogram-tonconnect-0.13.7/aiogram_tonconnect/tonconnect/tonconnect.py
--rw-rw-r--   0 ness      (1000) ness      (1000)     6268 2024-03-27 17:06:19.000000 aiogram-tonconnect-0.13.7/aiogram_tonconnect/tonconnect/transactions.py
-drwxrwxr-x   0 ness      (1000) ness      (1000)        0 2024-05-27 04:28:08.939554 aiogram-tonconnect-0.13.7/aiogram_tonconnect/tonconnect/wallet/
--rw-rw-r--   0 ness      (1000) ness      (1000)        0 2024-03-27 17:06:19.000000 aiogram-tonconnect-0.13.7/aiogram_tonconnect/tonconnect/wallet/__init__.py
--rw-rw-r--   0 ness      (1000) ness      (1000)     6641 2024-03-27 17:06:19.000000 aiogram-tonconnect-0.13.7/aiogram_tonconnect/tonconnect/wallet/manager.py
-drwxrwxr-x   0 ness      (1000) ness      (1000)        0 2024-05-27 04:28:08.939554 aiogram-tonconnect-0.13.7/aiogram_tonconnect/utils/
--rw-rw-r--   0 ness      (1000) ness      (1000)        0 2024-03-27 17:06:19.000000 aiogram-tonconnect-0.13.7/aiogram_tonconnect/utils/__init__.py
--rw-rw-r--   0 ness      (1000) ness      (1000)     2416 2024-03-27 17:06:19.000000 aiogram-tonconnect-0.13.7/aiogram_tonconnect/utils/address.py
--rw-rw-r--   0 ness      (1000) ness      (1000)      945 2024-03-27 17:06:19.000000 aiogram-tonconnect-0.13.7/aiogram_tonconnect/utils/exceptions.py
--rw-rw-r--   0 ness      (1000) ness      (1000)     6024 2024-03-27 17:06:19.000000 aiogram-tonconnect-0.13.7/aiogram_tonconnect/utils/keyboards.py
--rw-rw-r--   0 ness      (1000) ness      (1000)     1914 2024-03-27 17:06:19.000000 aiogram-tonconnect-0.13.7/aiogram_tonconnect/utils/proof.py
-drwxrwxr-x   0 ness      (1000) ness      (1000)        0 2024-05-27 04:28:08.939554 aiogram-tonconnect-0.13.7/aiogram_tonconnect/utils/qrcode/
--rw-rw-r--   0 ness      (1000) ness      (1000)     2348 2024-03-27 17:06:19.000000 aiogram-tonconnect-0.13.7/aiogram_tonconnect/utils/qrcode/__init__.py
--rw-rw-r--   0 ness      (1000) ness      (1000)    31987 2024-03-27 17:06:19.000000 aiogram-tonconnect-0.13.7/aiogram_tonconnect/utils/qrcode/generator.py
--rw-rw-r--   0 ness      (1000) ness      (1000)      947 2024-03-27 17:06:19.000000 aiogram-tonconnect-0.13.7/aiogram_tonconnect/utils/states.py
--rw-rw-r--   0 ness      (1000) ness      (1000)     6120 2024-03-27 17:06:19.000000 aiogram-tonconnect-0.13.7/aiogram_tonconnect/utils/texts.py
-drwxrwxr-x   0 ness      (1000) ness      (1000)        0 2024-05-27 04:28:08.935554 aiogram-tonconnect-0.13.7/aiogram_tonconnect.egg-info/
--rw-r--r--   0 ness      (1000) ness      (1000)     5438 2024-05-27 04:28:08.000000 aiogram-tonconnect-0.13.7/aiogram_tonconnect.egg-info/PKG-INFO
--rw-rw-r--   0 ness      (1000) ness      (1000)     1254 2024-05-27 04:28:08.000000 aiogram-tonconnect-0.13.7/aiogram_tonconnect.egg-info/SOURCES.txt
--rw-rw-r--   0 ness      (1000) ness      (1000)        1 2024-05-27 04:28:08.000000 aiogram-tonconnect-0.13.7/aiogram_tonconnect.egg-info/dependency_links.txt
--rw-rw-r--   0 ness      (1000) ness      (1000)       98 2024-05-27 04:28:08.000000 aiogram-tonconnect-0.13.7/aiogram_tonconnect.egg-info/requires.txt
--rw-rw-r--   0 ness      (1000) ness      (1000)       19 2024-05-27 04:28:08.000000 aiogram-tonconnect-0.13.7/aiogram_tonconnect.egg-info/top_level.txt
--rw-rw-r--   0 ness      (1000) ness      (1000)       38 2024-05-27 04:28:08.939554 aiogram-tonconnect-0.13.7/setup.cfg
--rw-rw-r--   0 ness      (1000) ness      (1000)     1222 2024-05-27 04:27:53.000000 aiogram-tonconnect-0.13.7/setup.py
+drwxrwxr-x   0 ness      (1000) ness      (1000)        0 2024-05-29 16:37:36.904754 aiogram-tonconnect-0.13.8/
+-rw-rw-r--   0 ness      (1000) ness      (1000)     1064 2024-03-27 17:06:19.000000 aiogram-tonconnect-0.13.8/LICENSE
+-rw-r--r--   0 ness      (1000) ness      (1000)     5438 2024-05-29 16:37:36.900754 aiogram-tonconnect-0.13.8/PKG-INFO
+-rw-rw-r--   0 ness      (1000) ness      (1000)     4458 2024-03-27 17:06:19.000000 aiogram-tonconnect-0.13.8/README.md
+drwxrwxr-x   0 ness      (1000) ness      (1000)        0 2024-05-29 16:37:36.896754 aiogram-tonconnect-0.13.8/aiogram_tonconnect/
+-rw-rw-r--   0 ness      (1000) ness      (1000)       65 2024-03-27 17:06:19.000000 aiogram-tonconnect-0.13.8/aiogram_tonconnect/__init__.py
+-rw-rw-r--   0 ness      (1000) ness      (1000)     6377 2024-03-27 17:06:19.000000 aiogram-tonconnect-0.13.8/aiogram_tonconnect/handlers.py
+-rw-rw-r--   0 ness      (1000) ness      (1000)    20809 2024-05-27 04:26:10.000000 aiogram-tonconnect-0.13.8/aiogram_tonconnect/manager.py
+-rw-rw-r--   0 ness      (1000) ness      (1000)     5253 2024-05-19 12:46:38.000000 aiogram-tonconnect-0.13.8/aiogram_tonconnect/middleware.py
+drwxrwxr-x   0 ness      (1000) ness      (1000)        0 2024-05-29 16:37:36.900754 aiogram-tonconnect-0.13.8/aiogram_tonconnect/tonconnect/
+-rw-rw-r--   0 ness      (1000) ness      (1000)      140 2024-03-27 17:06:19.000000 aiogram-tonconnect-0.13.8/aiogram_tonconnect/tonconnect/__init__.py
+-rw-rw-r--   0 ness      (1000) ness      (1000)     7607 2024-05-29 16:34:38.000000 aiogram-tonconnect-0.13.8/aiogram_tonconnect/tonconnect/models.py
+-rw-rw-r--   0 ness      (1000) ness      (1000)     7469 2024-03-30 13:07:39.000000 aiogram-tonconnect-0.13.8/aiogram_tonconnect/tonconnect/provider.py
+drwxrwxr-x   0 ness      (1000) ness      (1000)        0 2024-05-29 16:37:36.900754 aiogram-tonconnect-0.13.8/aiogram_tonconnect/tonconnect/storage/
+-rw-rw-r--   0 ness      (1000) ness      (1000)      300 2024-03-27 17:06:19.000000 aiogram-tonconnect-0.13.8/aiogram_tonconnect/tonconnect/storage/__init__.py
+-rw-rw-r--   0 ness      (1000) ness      (1000)     2047 2024-03-27 17:06:19.000000 aiogram-tonconnect-0.13.8/aiogram_tonconnect/tonconnect/storage/base.py
+-rw-rw-r--   0 ness      (1000) ness      (1000)     2247 2024-03-27 17:06:19.000000 aiogram-tonconnect-0.13.8/aiogram_tonconnect/tonconnect/storage/callback.py
+-rw-rw-r--   0 ness      (1000) ness      (1000)     1214 2024-03-27 17:06:19.000000 aiogram-tonconnect-0.13.8/aiogram_tonconnect/tonconnect/storage/session.py
+-rw-rw-r--   0 ness      (1000) ness      (1000)     1078 2024-03-27 17:06:19.000000 aiogram-tonconnect-0.13.8/aiogram_tonconnect/tonconnect/storage/task.py
+-rw-rw-r--   0 ness      (1000) ness      (1000)     2197 2024-03-30 13:09:49.000000 aiogram-tonconnect-0.13.8/aiogram_tonconnect/tonconnect/tonconnect.py
+-rw-rw-r--   0 ness      (1000) ness      (1000)     6268 2024-03-27 17:06:19.000000 aiogram-tonconnect-0.13.8/aiogram_tonconnect/tonconnect/transactions.py
+drwxrwxr-x   0 ness      (1000) ness      (1000)        0 2024-05-29 16:37:36.900754 aiogram-tonconnect-0.13.8/aiogram_tonconnect/tonconnect/wallet/
+-rw-rw-r--   0 ness      (1000) ness      (1000)        0 2024-03-27 17:06:19.000000 aiogram-tonconnect-0.13.8/aiogram_tonconnect/tonconnect/wallet/__init__.py
+-rw-rw-r--   0 ness      (1000) ness      (1000)     6641 2024-03-27 17:06:19.000000 aiogram-tonconnect-0.13.8/aiogram_tonconnect/tonconnect/wallet/manager.py
+drwxrwxr-x   0 ness      (1000) ness      (1000)        0 2024-05-29 16:37:36.900754 aiogram-tonconnect-0.13.8/aiogram_tonconnect/utils/
+-rw-rw-r--   0 ness      (1000) ness      (1000)        0 2024-03-27 17:06:19.000000 aiogram-tonconnect-0.13.8/aiogram_tonconnect/utils/__init__.py
+-rw-rw-r--   0 ness      (1000) ness      (1000)     2416 2024-03-27 17:06:19.000000 aiogram-tonconnect-0.13.8/aiogram_tonconnect/utils/address.py
+-rw-rw-r--   0 ness      (1000) ness      (1000)      945 2024-03-27 17:06:19.000000 aiogram-tonconnect-0.13.8/aiogram_tonconnect/utils/exceptions.py
+-rw-rw-r--   0 ness      (1000) ness      (1000)     6024 2024-03-27 17:06:19.000000 aiogram-tonconnect-0.13.8/aiogram_tonconnect/utils/keyboards.py
+-rw-rw-r--   0 ness      (1000) ness      (1000)     1914 2024-03-27 17:06:19.000000 aiogram-tonconnect-0.13.8/aiogram_tonconnect/utils/proof.py
+drwxrwxr-x   0 ness      (1000) ness      (1000)        0 2024-05-29 16:37:36.900754 aiogram-tonconnect-0.13.8/aiogram_tonconnect/utils/qrcode/
+-rw-rw-r--   0 ness      (1000) ness      (1000)     2348 2024-03-27 17:06:19.000000 aiogram-tonconnect-0.13.8/aiogram_tonconnect/utils/qrcode/__init__.py
+-rw-rw-r--   0 ness      (1000) ness      (1000)    31987 2024-03-27 17:06:19.000000 aiogram-tonconnect-0.13.8/aiogram_tonconnect/utils/qrcode/generator.py
+-rw-rw-r--   0 ness      (1000) ness      (1000)      947 2024-03-27 17:06:19.000000 aiogram-tonconnect-0.13.8/aiogram_tonconnect/utils/states.py
+-rw-rw-r--   0 ness      (1000) ness      (1000)     6120 2024-03-27 17:06:19.000000 aiogram-tonconnect-0.13.8/aiogram_tonconnect/utils/texts.py
+drwxrwxr-x   0 ness      (1000) ness      (1000)        0 2024-05-29 16:37:36.896754 aiogram-tonconnect-0.13.8/aiogram_tonconnect.egg-info/
+-rw-r--r--   0 ness      (1000) ness      (1000)     5438 2024-05-29 16:37:36.000000 aiogram-tonconnect-0.13.8/aiogram_tonconnect.egg-info/PKG-INFO
+-rw-rw-r--   0 ness      (1000) ness      (1000)     1254 2024-05-29 16:37:36.000000 aiogram-tonconnect-0.13.8/aiogram_tonconnect.egg-info/SOURCES.txt
+-rw-rw-r--   0 ness      (1000) ness      (1000)        1 2024-05-29 16:37:36.000000 aiogram-tonconnect-0.13.8/aiogram_tonconnect.egg-info/dependency_links.txt
+-rw-rw-r--   0 ness      (1000) ness      (1000)       98 2024-05-29 16:37:36.000000 aiogram-tonconnect-0.13.8/aiogram_tonconnect.egg-info/requires.txt
+-rw-rw-r--   0 ness      (1000) ness      (1000)       19 2024-05-29 16:37:36.000000 aiogram-tonconnect-0.13.8/aiogram_tonconnect.egg-info/top_level.txt
+-rw-rw-r--   0 ness      (1000) ness      (1000)       38 2024-05-29 16:37:36.904754 aiogram-tonconnect-0.13.8/setup.cfg
+-rw-rw-r--   0 ness      (1000) ness      (1000)     1222 2024-05-29 16:36:37.000000 aiogram-tonconnect-0.13.8/setup.py
```

### Comparing `aiogram-tonconnect-0.13.7/LICENSE` & `aiogram-tonconnect-0.13.8/LICENSE`

 * *Files identical despite different names*

### Comparing `aiogram-tonconnect-0.13.7/PKG-INFO` & `aiogram-tonconnect-0.13.8/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: aiogram-tonconnect
-Version: 0.13.7
+Version: 0.13.8
 Summary: TON Connect UI for aiogram bots.
 Home-page: https://github.com/nessshon/aiogram-tonconnect/
 Author: nessshon
 Project-URL: Documentation, https://nessshon.github.io/aiogram-tonconnect/
 Project-URL: Bot example, https://t.me/aiogramTONConnectBot/
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
```

### Comparing `aiogram-tonconnect-0.13.7/README.md` & `aiogram-tonconnect-0.13.8/README.md`

 * *Files identical despite different names*

### Comparing `aiogram-tonconnect-0.13.7/aiogram_tonconnect/handlers.py` & `aiogram-tonconnect-0.13.8/aiogram_tonconnect/handlers.py`

 * *Files identical despite different names*

### Comparing `aiogram-tonconnect-0.13.7/aiogram_tonconnect/manager.py` & `aiogram-tonconnect-0.13.8/aiogram_tonconnect/manager.py`

 * *Files identical despite different names*

### Comparing `aiogram-tonconnect-0.13.7/aiogram_tonconnect/middleware.py` & `aiogram-tonconnect-0.13.8/aiogram_tonconnect/middleware.py`

 * *Files identical despite different names*

### Comparing `aiogram-tonconnect-0.13.7/aiogram_tonconnect/tonconnect/models.py` & `aiogram-tonconnect-0.13.8/aiogram_tonconnect/tonconnect/models.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-from enum import IntEnum
+from enum import Enum
 from typing import Awaitable, Callable, Dict, List, Optional, Any, Union
 
 from pydantic import BaseModel, Field
 from pytonconnect.parsers import WalletInfo
 
 from aiogram_tonconnect.utils.address import Address
 
@@ -165,15 +165,15 @@
 
     address: str
     amount: str
     stateInit: Optional[str] = Field(default="")
     payload: Optional[str] = Field(default="")
 
 
-class CHAIN(IntEnum):
+class CHAIN(str, Enum):
     MAINNET = "-239"
     TESTNET = "-3"
 
 
 class Transaction(BaseModel):
     """
     Data class representing a AiogramTonConnect transaction.
```

### Comparing `aiogram-tonconnect-0.13.7/aiogram_tonconnect/tonconnect/provider.py` & `aiogram-tonconnect-0.13.8/aiogram_tonconnect/tonconnect/provider.py`

 * *Files identical despite different names*

### Comparing `aiogram-tonconnect-0.13.7/aiogram_tonconnect/tonconnect/storage/base.py` & `aiogram-tonconnect-0.13.8/aiogram_tonconnect/tonconnect/storage/base.py`

 * *Files identical despite different names*

### Comparing `aiogram-tonconnect-0.13.7/aiogram_tonconnect/tonconnect/storage/callback.py` & `aiogram-tonconnect-0.13.8/aiogram_tonconnect/tonconnect/storage/callback.py`

 * *Files identical despite different names*

### Comparing `aiogram-tonconnect-0.13.7/aiogram_tonconnect/tonconnect/storage/session.py` & `aiogram-tonconnect-0.13.8/aiogram_tonconnect/tonconnect/storage/session.py`

 * *Files identical despite different names*

### Comparing `aiogram-tonconnect-0.13.7/aiogram_tonconnect/tonconnect/storage/task.py` & `aiogram-tonconnect-0.13.8/aiogram_tonconnect/tonconnect/storage/task.py`

 * *Files identical despite different names*

### Comparing `aiogram-tonconnect-0.13.7/aiogram_tonconnect/tonconnect/tonconnect.py` & `aiogram-tonconnect-0.13.8/aiogram_tonconnect/tonconnect/tonconnect.py`

 * *Files identical despite different names*

### Comparing `aiogram-tonconnect-0.13.7/aiogram_tonconnect/tonconnect/transactions.py` & `aiogram-tonconnect-0.13.8/aiogram_tonconnect/tonconnect/transactions.py`

 * *Files identical despite different names*

### Comparing `aiogram-tonconnect-0.13.7/aiogram_tonconnect/tonconnect/wallet/manager.py` & `aiogram-tonconnect-0.13.8/aiogram_tonconnect/tonconnect/wallet/manager.py`

 * *Files identical despite different names*

### Comparing `aiogram-tonconnect-0.13.7/aiogram_tonconnect/utils/address.py` & `aiogram-tonconnect-0.13.8/aiogram_tonconnect/utils/address.py`

 * *Files identical despite different names*

### Comparing `aiogram-tonconnect-0.13.7/aiogram_tonconnect/utils/exceptions.py` & `aiogram-tonconnect-0.13.8/aiogram_tonconnect/utils/exceptions.py`

 * *Files identical despite different names*

### Comparing `aiogram-tonconnect-0.13.7/aiogram_tonconnect/utils/keyboards.py` & `aiogram-tonconnect-0.13.8/aiogram_tonconnect/utils/keyboards.py`

 * *Files identical despite different names*

### Comparing `aiogram-tonconnect-0.13.7/aiogram_tonconnect/utils/proof.py` & `aiogram-tonconnect-0.13.8/aiogram_tonconnect/utils/proof.py`

 * *Files identical despite different names*

### Comparing `aiogram-tonconnect-0.13.7/aiogram_tonconnect/utils/qrcode/__init__.py` & `aiogram-tonconnect-0.13.8/aiogram_tonconnect/utils/qrcode/__init__.py`

 * *Files identical despite different names*

### Comparing `aiogram-tonconnect-0.13.7/aiogram_tonconnect/utils/qrcode/generator.py` & `aiogram-tonconnect-0.13.8/aiogram_tonconnect/utils/qrcode/generator.py`

 * *Files identical despite different names*

### Comparing `aiogram-tonconnect-0.13.7/aiogram_tonconnect/utils/states.py` & `aiogram-tonconnect-0.13.8/aiogram_tonconnect/utils/states.py`

 * *Files identical despite different names*

### Comparing `aiogram-tonconnect-0.13.7/aiogram_tonconnect/utils/texts.py` & `aiogram-tonconnect-0.13.8/aiogram_tonconnect/utils/texts.py`

 * *Files identical despite different names*

### Comparing `aiogram-tonconnect-0.13.7/aiogram_tonconnect.egg-info/PKG-INFO` & `aiogram-tonconnect-0.13.8/aiogram_tonconnect.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: aiogram-tonconnect
-Version: 0.13.7
+Version: 0.13.8
 Summary: TON Connect UI for aiogram bots.
 Home-page: https://github.com/nessshon/aiogram-tonconnect/
 Author: nessshon
 Project-URL: Documentation, https://nessshon.github.io/aiogram-tonconnect/
 Project-URL: Bot example, https://t.me/aiogramTONConnectBot/
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
```

### Comparing `aiogram-tonconnect-0.13.7/aiogram_tonconnect.egg-info/SOURCES.txt` & `aiogram-tonconnect-0.13.8/aiogram_tonconnect.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `aiogram-tonconnect-0.13.7/setup.py` & `aiogram-tonconnect-0.13.8/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 import setuptools
 
 with open("README.md", "r") as fh:
     long_description = fh.read()
 
 setuptools.setup(
     name="aiogram-tonconnect",
-    version="0.13.7",
+    version="0.13.8",
     author="nessshon",
     description="TON Connect UI for aiogram bots.",
     long_description=long_description,
     long_description_content_type="text/markdown",
     packages=setuptools.find_packages(exclude=["example", "docs"]),
     install_requires=[
         "aiofiles",
```

