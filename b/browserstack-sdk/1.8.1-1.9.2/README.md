# Comparing `tmp/browserstack_sdk-1.8.1.tar.gz` & `tmp/browserstack_sdk-1.9.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "browserstack_sdk-1.8.1.tar", last modified: Wed May 24 06:15:03 2023, max compression
+gzip compressed data, was "browserstack_sdk-1.9.2.tar", last modified: Fri Jun  2 10:42:30 2023, max compression
```

## Comparing `browserstack_sdk-1.8.1.tar` & `browserstack_sdk-1.9.2.tar`

### file list

```diff
@@ -1,20 +1,20 @@
-drwxr-xr-x   0 francis    (503) staff       (20)        0 2023-05-24 06:15:03.443093 browserstack_sdk-1.8.1/
--rw-r--r--   0 francis    (503) staff       (20)     4335 2023-05-24 06:14:23.000000 browserstack_sdk-1.8.1/LICENSE.txt
--rw-r--r--   0 francis    (503) staff       (20)     5046 2023-05-24 06:15:03.442963 browserstack_sdk-1.8.1/PKG-INFO
--rw-r--r--   0 francis    (503) staff       (20)      815 2023-05-24 06:14:23.000000 browserstack_sdk-1.8.1/README.md
-drwxr-xr-x   0 francis    (503) staff       (20)        0 2023-05-24 06:15:03.441928 browserstack_sdk-1.8.1/browserstack_sdk/
--rw-r--r--   0 francis    (503) staff       (20)   183595 2023-05-24 06:14:23.000000 browserstack_sdk-1.8.1/browserstack_sdk/__init__.py
--rw-r--r--   0 francis    (503) staff       (20)       22 2023-05-24 06:14:23.000000 browserstack_sdk-1.8.1/browserstack_sdk/_version.py
--rw-r--r--   0 francis    (503) staff       (20)     3891 2023-05-24 06:14:23.000000 browserstack_sdk-1.8.1/browserstack_sdk/browserstack.framework.yml.sample
--rw-r--r--   0 francis    (503) staff       (20)     3125 2023-05-24 06:14:23.000000 browserstack_sdk-1.8.1/browserstack_sdk/browserstack.generic.yml.sample
-drwxr-xr-x   0 francis    (503) staff       (20)        0 2023-05-24 06:15:03.442568 browserstack_sdk-1.8.1/browserstack_sdk.egg-info/
--rw-r--r--   0 francis    (503) staff       (20)     5046 2023-05-24 06:15:03.000000 browserstack_sdk-1.8.1/browserstack_sdk.egg-info/PKG-INFO
--rw-r--r--   0 francis    (503) staff       (20)      466 2023-05-24 06:15:03.000000 browserstack_sdk-1.8.1/browserstack_sdk.egg-info/SOURCES.txt
--rw-r--r--   0 francis    (503) staff       (20)        1 2023-05-24 06:15:03.000000 browserstack_sdk-1.8.1/browserstack_sdk.egg-info/dependency_links.txt
--rw-r--r--   0 francis    (503) staff       (20)      139 2023-05-24 06:15:03.000000 browserstack_sdk-1.8.1/browserstack_sdk.egg-info/entry_points.txt
--rw-r--r--   0 francis    (503) staff       (20)       70 2023-05-24 06:15:03.000000 browserstack_sdk-1.8.1/browserstack_sdk.egg-info/requires.txt
--rw-r--r--   0 francis    (503) staff       (20)       43 2023-05-24 06:15:03.000000 browserstack_sdk-1.8.1/browserstack_sdk.egg-info/top_level.txt
-drwxr-xr-x   0 francis    (503) staff       (20)        0 2023-05-24 06:15:03.442752 browserstack_sdk-1.8.1/pytest_browserstackplugin/
--rw-r--r--   0 francis    (503) staff       (20)    11015 2023-05-24 06:14:23.000000 browserstack_sdk-1.8.1/pytest_browserstackplugin/plugin.py
--rw-r--r--   0 francis    (503) staff       (20)       38 2023-05-24 06:15:03.443129 browserstack_sdk-1.8.1/setup.cfg
--rw-r--r--   0 francis    (503) staff       (20)     1343 2023-05-24 06:14:23.000000 browserstack_sdk-1.8.1/setup.py
+drwxr-xr-x   0 francis    (503) wheel        (0)        0 2023-06-02 10:42:30.185954 browserstack_sdk-1.9.2/
+-rw-r--r--   0 francis    (503) wheel        (0)     4335 2023-06-02 10:42:14.000000 browserstack_sdk-1.9.2/LICENSE.txt
+-rw-r--r--   0 francis    (503) wheel        (0)     5046 2023-06-02 10:42:30.185838 browserstack_sdk-1.9.2/PKG-INFO
+-rw-r--r--   0 francis    (503) wheel        (0)      815 2023-06-02 10:42:14.000000 browserstack_sdk-1.9.2/README.md
+drwxr-xr-x   0 francis    (503) wheel        (0)        0 2023-06-02 10:42:30.184930 browserstack_sdk-1.9.2/browserstack_sdk/
+-rw-r--r--   0 francis    (503) wheel        (0)   186900 2023-06-02 10:42:14.000000 browserstack_sdk-1.9.2/browserstack_sdk/__init__.py
+-rw-r--r--   0 francis    (503) wheel        (0)       22 2023-06-02 10:42:14.000000 browserstack_sdk-1.9.2/browserstack_sdk/_version.py
+-rw-r--r--   0 francis    (503) wheel        (0)     3891 2023-06-02 10:42:14.000000 browserstack_sdk-1.9.2/browserstack_sdk/browserstack.framework.yml.sample
+-rw-r--r--   0 francis    (503) wheel        (0)     3125 2023-06-02 10:42:14.000000 browserstack_sdk-1.9.2/browserstack_sdk/browserstack.generic.yml.sample
+drwxr-xr-x   0 francis    (503) wheel        (0)        0 2023-06-02 10:42:30.185572 browserstack_sdk-1.9.2/browserstack_sdk.egg-info/
+-rw-r--r--   0 francis    (503) wheel        (0)     5046 2023-06-02 10:42:30.000000 browserstack_sdk-1.9.2/browserstack_sdk.egg-info/PKG-INFO
+-rw-r--r--   0 francis    (503) wheel        (0)      466 2023-06-02 10:42:30.000000 browserstack_sdk-1.9.2/browserstack_sdk.egg-info/SOURCES.txt
+-rw-r--r--   0 francis    (503) wheel        (0)        1 2023-06-02 10:42:30.000000 browserstack_sdk-1.9.2/browserstack_sdk.egg-info/dependency_links.txt
+-rw-r--r--   0 francis    (503) wheel        (0)      139 2023-06-02 10:42:30.000000 browserstack_sdk-1.9.2/browserstack_sdk.egg-info/entry_points.txt
+-rw-r--r--   0 francis    (503) wheel        (0)       70 2023-06-02 10:42:30.000000 browserstack_sdk-1.9.2/browserstack_sdk.egg-info/requires.txt
+-rw-r--r--   0 francis    (503) wheel        (0)       43 2023-06-02 10:42:30.000000 browserstack_sdk-1.9.2/browserstack_sdk.egg-info/top_level.txt
+drwxr-xr-x   0 francis    (503) wheel        (0)        0 2023-06-02 10:42:30.185678 browserstack_sdk-1.9.2/pytest_browserstackplugin/
+-rw-r--r--   0 francis    (503) wheel        (0)    11065 2023-06-02 10:42:14.000000 browserstack_sdk-1.9.2/pytest_browserstackplugin/plugin.py
+-rw-r--r--   0 francis    (503) wheel        (0)       38 2023-06-02 10:42:30.185984 browserstack_sdk-1.9.2/setup.cfg
+-rw-r--r--   0 francis    (503) wheel        (0)     1343 2023-06-02 10:42:14.000000 browserstack_sdk-1.9.2/setup.py
```

### Comparing `browserstack_sdk-1.8.1/LICENSE.txt` & `browserstack_sdk-1.9.2/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `browserstack_sdk-1.8.1/PKG-INFO` & `browserstack_sdk-1.9.2/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: browserstack_sdk
-Version: 1.8.1
+Version: 1.9.2
 Summary: Python SDK for browserstack selenium-webdriver tests
 Author: BrowserStack
 Author-email: support@browserstack.com
 License: BrowserStack Software License Agreement
         The “Licensed Software” under this BrowserStack Software License Agreement (“Agreement”) shall be used by
         you only if You agree to the following terms and conditions. Downloading the Licensed Software and indicating
         your consent to the terms of this license constitutes a binding Agreement between BrowserStack and You. If
```

### Comparing `browserstack_sdk-1.8.1/README.md` & `browserstack_sdk-1.9.2/README.md`

 * *Files identical despite different names*

### Comparing `browserstack_sdk-1.8.1/browserstack_sdk/__init__.py` & `browserstack_sdk-1.9.2/browserstack_sdk/__init__.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,1468 +1,1558 @@
 # coding: UTF-8
 import sys
-bstack1ll_opy_ = sys.version_info [0] == 2
-bstack1l_opy_ = 2048
-bstack1l1l_opy_ = 7
-def bstack1ll1_opy_ (bstack1_opy_):
+bstack11l_opy_ = sys.version_info [0] == 2
+bstack1ll_opy_ = 2048
+bstackl_opy_ = 7
+def bstack11_opy_ (bstack1_opy_):
     global bstack111_opy_
     stringNr = ord (bstack1_opy_ [-1])
-    bstack1l1_opy_ = bstack1_opy_ [:-1]
-    bstack1lll_opy_ = stringNr % len (bstack1l1_opy_)
-    bstack11l_opy_ = bstack1l1_opy_ [:bstack1lll_opy_] + bstack1l1_opy_ [bstack1lll_opy_:]
-    if bstack1ll_opy_:
-        bstack11_opy_ = unicode () .join ([unichr (ord (char) - bstack1l_opy_ - (bstackl_opy_ + stringNr) % bstack1l1l_opy_) for bstackl_opy_, char in enumerate (bstack11l_opy_)])
+    bstack1ll1_opy_ = bstack1_opy_ [:-1]
+    bstack1l_opy_ = stringNr % len (bstack1ll1_opy_)
+    bstack1l1_opy_ = bstack1ll1_opy_ [:bstack1l_opy_] + bstack1ll1_opy_ [bstack1l_opy_:]
+    if bstack11l_opy_:
+        bstack1lll_opy_ = unicode () .join ([unichr (ord (char) - bstack1ll_opy_ - (bstack1l1l_opy_ + stringNr) % bstackl_opy_) for bstack1l1l_opy_, char in enumerate (bstack1l1_opy_)])
     else:
-        bstack11_opy_ = str () .join ([chr (ord (char) - bstack1l_opy_ - (bstackl_opy_ + stringNr) % bstack1l1l_opy_) for bstackl_opy_, char in enumerate (bstack11l_opy_)])
-    return eval (bstack11_opy_)
+        bstack1lll_opy_ = str () .join ([chr (ord (char) - bstack1ll_opy_ - (bstack1l1l_opy_ + stringNr) % bstackl_opy_) for bstack1l1l_opy_, char in enumerate (bstack1l1_opy_)])
+    return eval (bstack1lll_opy_)
 import atexit
 import os
 import signal
 import sys
+import time
 import yaml
 import requests
 import logging
 import threading
 import socket
 import datetime
 import string
 import random
 import json
 import collections.abc
 import re
+from multiprocessing import Pool
 from packaging import version
 from browserstack.local import Local
 from urllib.parse import urlparse
-bstack111l11l_opy_ = {
-	bstack1ll1_opy_ (u"ࠬࡻࡳࡦࡴࡑࡥࡲ࡫ࠧࠁ"): bstack1ll1_opy_ (u"࠭ࡢࡳࡱࡺࡷࡪࡸࡳࡵࡣࡦ࡯࠳ࡻࡳࡦࡴࠪࠂ"),
-  bstack1ll1_opy_ (u"ࠧࡢࡥࡦࡩࡸࡹࡋࡦࡻࠪࠃ"): bstack1ll1_opy_ (u"ࠨࡤࡵࡳࡼࡹࡥࡳࡵࡷࡥࡨࡱ࠮࡬ࡧࡼࠫࠄ"),
-  bstack1ll1_opy_ (u"ࠩࡲࡷ࡛࡫ࡲࡴ࡫ࡲࡲࠬࠅ"): bstack1ll1_opy_ (u"ࠪࡳࡸࡥࡶࡦࡴࡶ࡭ࡴࡴࠧࠆ"),
-  bstack1ll1_opy_ (u"ࠫࡺࡹࡥࡘ࠵ࡆࠫࠇ"): bstack1ll1_opy_ (u"ࠬࡨࡲࡰࡹࡶࡩࡷࡹࡴࡢࡥ࡮࠲ࡺࡹࡥࡠࡹ࠶ࡧࠬࠈ"),
-  bstack1ll1_opy_ (u"࠭ࡰࡳࡱ࡭ࡩࡨࡺࡎࡢ࡯ࡨࠫࠉ"): bstack1ll1_opy_ (u"ࠧࡱࡴࡲ࡮ࡪࡩࡴࠨࠊ"),
-  bstack1ll1_opy_ (u"ࠨࡤࡸ࡭ࡱࡪࡎࡢ࡯ࡨࠫࠋ"): bstack1ll1_opy_ (u"ࠩࡥࡹ࡮ࡲࡤࠨࠌ"),
-  bstack1ll1_opy_ (u"ࠪࡷࡪࡹࡳࡪࡱࡱࡒࡦࡳࡥࠨࠍ"): bstack1ll1_opy_ (u"ࠫࡳࡧ࡭ࡦࠩࠎ"),
-  bstack1ll1_opy_ (u"ࠬࡪࡥࡣࡷࡪࠫࠏ"): bstack1ll1_opy_ (u"࠭ࡢࡳࡱࡺࡷࡪࡸࡳࡵࡣࡦ࡯࠳ࡪࡥࡣࡷࡪࠫࠐ"),
-  bstack1ll1_opy_ (u"ࠧࡤࡱࡱࡷࡴࡲࡥࡍࡱࡪࡷࠬࠑ"): bstack1ll1_opy_ (u"ࠨࡤࡵࡳࡼࡹࡥࡳࡵࡷࡥࡨࡱ࠮ࡤࡱࡱࡷࡴࡲࡥࠨࠒ"),
-  bstack1ll1_opy_ (u"ࠩࡱࡩࡹࡽ࡯ࡳ࡭ࡏࡳ࡬ࡹࠧࠓ"): bstack1ll1_opy_ (u"ࠪࡦࡷࡵࡷࡴࡧࡵࡷࡹࡧࡣ࡬࠰ࡱࡩࡹࡽ࡯ࡳ࡭ࡏࡳ࡬ࡹࠧࠔ"),
-  bstack1ll1_opy_ (u"ࠫࡦࡶࡰࡪࡷࡰࡐࡴ࡭ࡳࠨࠕ"): bstack1ll1_opy_ (u"ࠬࡨࡲࡰࡹࡶࡩࡷࡹࡴࡢࡥ࡮࠲ࡦࡶࡰࡪࡷࡰࡐࡴ࡭ࡳࠨࠖ"),
-  bstack1ll1_opy_ (u"࠭ࡶࡪࡦࡨࡳࠬࠗ"): bstack1ll1_opy_ (u"ࠧࡣࡴࡲࡻࡸ࡫ࡲࡴࡶࡤࡧࡰ࠴ࡶࡪࡦࡨࡳࠬ࠘"),
-  bstack1ll1_opy_ (u"ࠨࡵࡨࡰࡪࡴࡩࡶ࡯ࡏࡳ࡬ࡹࠧ࠙"): bstack1ll1_opy_ (u"ࠩࡥࡶࡴࡽࡳࡦࡴࡶࡸࡦࡩ࡫࠯ࡵࡨࡰࡪࡴࡩࡶ࡯ࡏࡳ࡬ࡹࠧࠚ"),
-  bstack1ll1_opy_ (u"ࠪࡸࡪࡲࡥ࡮ࡧࡷࡶࡾࡒ࡯ࡨࡵࠪࠛ"): bstack1ll1_opy_ (u"ࠫࡧࡸ࡯ࡸࡵࡨࡶࡸࡺࡡࡤ࡭࠱ࡸࡪࡲࡥ࡮ࡧࡷࡶࡾࡒ࡯ࡨࡵࠪࠜ"),
-  bstack1ll1_opy_ (u"ࠬ࡭ࡥࡰࡎࡲࡧࡦࡺࡩࡰࡰࠪࠝ"): bstack1ll1_opy_ (u"࠭ࡢࡳࡱࡺࡷࡪࡸࡳࡵࡣࡦ࡯࠳࡭ࡥࡰࡎࡲࡧࡦࡺࡩࡰࡰࠪࠞ"),
-  bstack1ll1_opy_ (u"ࠧࡵ࡫ࡰࡩࡿࡵ࡮ࡦࠩࠟ"): bstack1ll1_opy_ (u"ࠨࡤࡵࡳࡼࡹࡥࡳࡵࡷࡥࡨࡱ࠮ࡵ࡫ࡰࡩࡿࡵ࡮ࡦࠩࠠ"),
-  bstack1ll1_opy_ (u"ࠩࡶࡩࡱ࡫࡮ࡪࡷࡰ࡚ࡪࡸࡳࡪࡱࡱࠫࠡ"): bstack1ll1_opy_ (u"ࠪࡦࡷࡵࡷࡴࡧࡵࡷࡹࡧࡣ࡬࠰ࡶࡩࡱ࡫࡮ࡪࡷࡰࡣࡻ࡫ࡲࡴ࡫ࡲࡲࠬࠢ"),
-  bstack1ll1_opy_ (u"ࠫࡲࡧࡳ࡬ࡅࡲࡱࡲࡧ࡮ࡥࡵࠪࠣ"): bstack1ll1_opy_ (u"ࠬࡨࡲࡰࡹࡶࡩࡷࡹࡴࡢࡥ࡮࠲ࡲࡧࡳ࡬ࡅࡲࡱࡲࡧ࡮ࡥࡵࠪࠤ"),
-  bstack1ll1_opy_ (u"࠭ࡩࡥ࡮ࡨࡘ࡮ࡳࡥࡰࡷࡷࠫࠥ"): bstack1ll1_opy_ (u"ࠧࡣࡴࡲࡻࡸ࡫ࡲࡴࡶࡤࡧࡰ࠴ࡩࡥ࡮ࡨࡘ࡮ࡳࡥࡰࡷࡷࠫࠦ"),
-  bstack1ll1_opy_ (u"ࠨ࡯ࡤࡷࡰࡈࡡࡴ࡫ࡦࡅࡺࡺࡨࠨࠧ"): bstack1ll1_opy_ (u"ࠩࡥࡶࡴࡽࡳࡦࡴࡶࡸࡦࡩ࡫࠯࡯ࡤࡷࡰࡈࡡࡴ࡫ࡦࡅࡺࡺࡨࠨࠨ"),
-  bstack1ll1_opy_ (u"ࠪࡷࡪࡴࡤࡌࡧࡼࡷࠬࠩ"): bstack1ll1_opy_ (u"ࠫࡧࡸ࡯ࡸࡵࡨࡶࡸࡺࡡࡤ࡭࠱ࡷࡪࡴࡤࡌࡧࡼࡷࠬࠪ"),
-  bstack1ll1_opy_ (u"ࠬࡧࡵࡵࡱ࡚ࡥ࡮ࡺࠧࠫ"): bstack1ll1_opy_ (u"࠭ࡢࡳࡱࡺࡷࡪࡸࡳࡵࡣࡦ࡯࠳ࡧࡵࡵࡱ࡚ࡥ࡮ࡺࠧࠬ"),
-  bstack1ll1_opy_ (u"ࠧࡩࡱࡶࡸࡸ࠭࠭"): bstack1ll1_opy_ (u"ࠨࡤࡵࡳࡼࡹࡥࡳࡵࡷࡥࡨࡱ࠮ࡩࡱࡶࡸࡸ࠭࠮"),
-  bstack1ll1_opy_ (u"ࠩࡥࡪࡨࡧࡣࡩࡧࠪ࠯"): bstack1ll1_opy_ (u"ࠪࡦࡷࡵࡷࡴࡧࡵࡷࡹࡧࡣ࡬࠰ࡥࡪࡨࡧࡣࡩࡧࠪ࠰"),
-  bstack1ll1_opy_ (u"ࠫࡼࡹࡌࡰࡥࡤࡰࡘࡻࡰࡱࡱࡵࡸࠬ࠱"): bstack1ll1_opy_ (u"ࠬࡨࡲࡰࡹࡶࡩࡷࡹࡴࡢࡥ࡮࠲ࡼࡹࡌࡰࡥࡤࡰࡘࡻࡰࡱࡱࡵࡸࠬ࠲"),
-  bstack1ll1_opy_ (u"࠭ࡤࡪࡵࡤࡦࡱ࡫ࡃࡰࡴࡶࡖࡪࡹࡴࡳ࡫ࡦࡸ࡮ࡵ࡮ࡴࠩ࠳"): bstack1ll1_opy_ (u"ࠧࡣࡴࡲࡻࡸ࡫ࡲࡴࡶࡤࡧࡰ࠴ࡤࡪࡵࡤࡦࡱ࡫ࡃࡰࡴࡶࡖࡪࡹࡴࡳ࡫ࡦࡸ࡮ࡵ࡮ࡴࠩ࠴"),
-  bstack1ll1_opy_ (u"ࠨࡦࡨࡺ࡮ࡩࡥࡏࡣࡰࡩࠬ࠵"): bstack1ll1_opy_ (u"ࠩࡧࡩࡻ࡯ࡣࡦࠩ࠶"),
-  bstack1ll1_opy_ (u"ࠪࡶࡪࡧ࡬ࡎࡱࡥ࡭ࡱ࡫ࠧ࠷"): bstack1ll1_opy_ (u"ࠫࡷ࡫ࡡ࡭ࡡࡰࡳࡧ࡯࡬ࡦࠩ࠸"),
-  bstack1ll1_opy_ (u"ࠬࡧࡰࡱ࡫ࡸࡱ࡛࡫ࡲࡴ࡫ࡲࡲࠬ࠹"): bstack1ll1_opy_ (u"࠭ࡢࡳࡱࡺࡷࡪࡸࡳࡵࡣࡦ࡯࠳ࡧࡰࡱ࡫ࡸࡱࡤࡼࡥࡳࡵ࡬ࡳࡳ࠭࠺"),
-  bstack1ll1_opy_ (u"ࠧࡤࡷࡶࡸࡴࡳࡎࡦࡶࡺࡳࡷࡱࠧ࠻"): bstack1ll1_opy_ (u"ࠨࡤࡵࡳࡼࡹࡥࡳࡵࡷࡥࡨࡱ࠮ࡤࡷࡶࡸࡴࡳࡎࡦࡶࡺࡳࡷࡱࠧ࠼"),
-  bstack1ll1_opy_ (u"ࠩࡱࡩࡹࡽ࡯ࡳ࡭ࡓࡶࡴ࡬ࡩ࡭ࡧࠪ࠽"): bstack1ll1_opy_ (u"ࠪࡦࡷࡵࡷࡴࡧࡵࡷࡹࡧࡣ࡬࠰ࡱࡩࡹࡽ࡯ࡳ࡭ࡓࡶࡴ࡬ࡩ࡭ࡧࠪ࠾"),
-  bstack1ll1_opy_ (u"ࠫࡦࡩࡣࡦࡲࡷࡍࡳࡹࡥࡤࡷࡵࡩࡈ࡫ࡲࡵࡵࠪ࠿"): bstack1ll1_opy_ (u"ࠬࡧࡣࡤࡧࡳࡸࡘࡹ࡬ࡄࡧࡵࡸࡸ࠭ࡀ"),
-  bstack1ll1_opy_ (u"࠭ࡢࡳࡱࡺࡷࡪࡸࡳࡵࡣࡦ࡯ࡘࡊࡋࠨࡁ"): bstack1ll1_opy_ (u"ࠧࡣࡴࡲࡻࡸ࡫ࡲࡴࡶࡤࡧࡰ࠴ࡢࡳࡱࡺࡷࡪࡸࡳࡵࡣࡦ࡯ࡘࡊࡋࠨࡂ"),
-  bstack1ll1_opy_ (u"ࠨࡵࡲࡹࡷࡩࡥࠨࡃ"): bstack1ll1_opy_ (u"ࠩࡥࡶࡴࡽࡳࡦࡴࡶࡸࡦࡩ࡫࠯ࡵࡲࡹࡷࡩࡥࠨࡄ"),
-  bstack1ll1_opy_ (u"ࠪࡦࡺ࡯࡬ࡥࡋࡧࡩࡳࡺࡩࡧ࡫ࡨࡶࠬࡅ"): bstack1ll1_opy_ (u"ࠫࡧࡸ࡯ࡸࡵࡨࡶࡸࡺࡡࡤ࡭࠱ࡦࡺ࡯࡬ࡥࡋࡧࡩࡳࡺࡩࡧ࡫ࡨࡶࠬࡆ"),
-  bstack1ll1_opy_ (u"ࠬ࡮࡯ࡴࡶࡑࡥࡲ࡫ࠧࡇ"): bstack1ll1_opy_ (u"࠭ࡢࡳࡱࡺࡷࡪࡸࡳࡵࡣࡦ࡯࠳࡮࡯ࡴࡶࡑࡥࡲ࡫ࠧࡈ"),
+bstack1l1ll11l1_opy_ = {
+	bstack11_opy_ (u"ࠬࡻࡳࡦࡴࡑࡥࡲ࡫ࠧࠁ"): bstack11_opy_ (u"࠭ࡢࡳࡱࡺࡷࡪࡸࡳࡵࡣࡦ࡯࠳ࡻࡳࡦࡴࠪࠂ"),
+  bstack11_opy_ (u"ࠧࡢࡥࡦࡩࡸࡹࡋࡦࡻࠪࠃ"): bstack11_opy_ (u"ࠨࡤࡵࡳࡼࡹࡥࡳࡵࡷࡥࡨࡱ࠮࡬ࡧࡼࠫࠄ"),
+  bstack11_opy_ (u"ࠩࡲࡷ࡛࡫ࡲࡴ࡫ࡲࡲࠬࠅ"): bstack11_opy_ (u"ࠪࡳࡸࡥࡶࡦࡴࡶ࡭ࡴࡴࠧࠆ"),
+  bstack11_opy_ (u"ࠫࡺࡹࡥࡘ࠵ࡆࠫࠇ"): bstack11_opy_ (u"ࠬࡨࡲࡰࡹࡶࡩࡷࡹࡴࡢࡥ࡮࠲ࡺࡹࡥࡠࡹ࠶ࡧࠬࠈ"),
+  bstack11_opy_ (u"࠭ࡰࡳࡱ࡭ࡩࡨࡺࡎࡢ࡯ࡨࠫࠉ"): bstack11_opy_ (u"ࠧࡱࡴࡲ࡮ࡪࡩࡴࠨࠊ"),
+  bstack11_opy_ (u"ࠨࡤࡸ࡭ࡱࡪࡎࡢ࡯ࡨࠫࠋ"): bstack11_opy_ (u"ࠩࡥࡹ࡮ࡲࡤࠨࠌ"),
+  bstack11_opy_ (u"ࠪࡷࡪࡹࡳࡪࡱࡱࡒࡦࡳࡥࠨࠍ"): bstack11_opy_ (u"ࠫࡳࡧ࡭ࡦࠩࠎ"),
+  bstack11_opy_ (u"ࠬࡪࡥࡣࡷࡪࠫࠏ"): bstack11_opy_ (u"࠭ࡢࡳࡱࡺࡷࡪࡸࡳࡵࡣࡦ࡯࠳ࡪࡥࡣࡷࡪࠫࠐ"),
+  bstack11_opy_ (u"ࠧࡤࡱࡱࡷࡴࡲࡥࡍࡱࡪࡷࠬࠑ"): bstack11_opy_ (u"ࠨࡤࡵࡳࡼࡹࡥࡳࡵࡷࡥࡨࡱ࠮ࡤࡱࡱࡷࡴࡲࡥࠨࠒ"),
+  bstack11_opy_ (u"ࠩࡱࡩࡹࡽ࡯ࡳ࡭ࡏࡳ࡬ࡹࠧࠓ"): bstack11_opy_ (u"ࠪࡦࡷࡵࡷࡴࡧࡵࡷࡹࡧࡣ࡬࠰ࡱࡩࡹࡽ࡯ࡳ࡭ࡏࡳ࡬ࡹࠧࠔ"),
+  bstack11_opy_ (u"ࠫࡦࡶࡰࡪࡷࡰࡐࡴ࡭ࡳࠨࠕ"): bstack11_opy_ (u"ࠬࡨࡲࡰࡹࡶࡩࡷࡹࡴࡢࡥ࡮࠲ࡦࡶࡰࡪࡷࡰࡐࡴ࡭ࡳࠨࠖ"),
+  bstack11_opy_ (u"࠭ࡶࡪࡦࡨࡳࠬࠗ"): bstack11_opy_ (u"ࠧࡣࡴࡲࡻࡸ࡫ࡲࡴࡶࡤࡧࡰ࠴ࡶࡪࡦࡨࡳࠬ࠘"),
+  bstack11_opy_ (u"ࠨࡵࡨࡰࡪࡴࡩࡶ࡯ࡏࡳ࡬ࡹࠧ࠙"): bstack11_opy_ (u"ࠩࡥࡶࡴࡽࡳࡦࡴࡶࡸࡦࡩ࡫࠯ࡵࡨࡰࡪࡴࡩࡶ࡯ࡏࡳ࡬ࡹࠧࠚ"),
+  bstack11_opy_ (u"ࠪࡸࡪࡲࡥ࡮ࡧࡷࡶࡾࡒ࡯ࡨࡵࠪࠛ"): bstack11_opy_ (u"ࠫࡧࡸ࡯ࡸࡵࡨࡶࡸࡺࡡࡤ࡭࠱ࡸࡪࡲࡥ࡮ࡧࡷࡶࡾࡒ࡯ࡨࡵࠪࠜ"),
+  bstack11_opy_ (u"ࠬ࡭ࡥࡰࡎࡲࡧࡦࡺࡩࡰࡰࠪࠝ"): bstack11_opy_ (u"࠭ࡢࡳࡱࡺࡷࡪࡸࡳࡵࡣࡦ࡯࠳࡭ࡥࡰࡎࡲࡧࡦࡺࡩࡰࡰࠪࠞ"),
+  bstack11_opy_ (u"ࠧࡵ࡫ࡰࡩࡿࡵ࡮ࡦࠩࠟ"): bstack11_opy_ (u"ࠨࡤࡵࡳࡼࡹࡥࡳࡵࡷࡥࡨࡱ࠮ࡵ࡫ࡰࡩࡿࡵ࡮ࡦࠩࠠ"),
+  bstack11_opy_ (u"ࠩࡶࡩࡱ࡫࡮ࡪࡷࡰ࡚ࡪࡸࡳࡪࡱࡱࠫࠡ"): bstack11_opy_ (u"ࠪࡦࡷࡵࡷࡴࡧࡵࡷࡹࡧࡣ࡬࠰ࡶࡩࡱ࡫࡮ࡪࡷࡰࡣࡻ࡫ࡲࡴ࡫ࡲࡲࠬࠢ"),
+  bstack11_opy_ (u"ࠫࡲࡧࡳ࡬ࡅࡲࡱࡲࡧ࡮ࡥࡵࠪࠣ"): bstack11_opy_ (u"ࠬࡨࡲࡰࡹࡶࡩࡷࡹࡴࡢࡥ࡮࠲ࡲࡧࡳ࡬ࡅࡲࡱࡲࡧ࡮ࡥࡵࠪࠤ"),
+  bstack11_opy_ (u"࠭ࡩࡥ࡮ࡨࡘ࡮ࡳࡥࡰࡷࡷࠫࠥ"): bstack11_opy_ (u"ࠧࡣࡴࡲࡻࡸ࡫ࡲࡴࡶࡤࡧࡰ࠴ࡩࡥ࡮ࡨࡘ࡮ࡳࡥࡰࡷࡷࠫࠦ"),
+  bstack11_opy_ (u"ࠨ࡯ࡤࡷࡰࡈࡡࡴ࡫ࡦࡅࡺࡺࡨࠨࠧ"): bstack11_opy_ (u"ࠩࡥࡶࡴࡽࡳࡦࡴࡶࡸࡦࡩ࡫࠯࡯ࡤࡷࡰࡈࡡࡴ࡫ࡦࡅࡺࡺࡨࠨࠨ"),
+  bstack11_opy_ (u"ࠪࡷࡪࡴࡤࡌࡧࡼࡷࠬࠩ"): bstack11_opy_ (u"ࠫࡧࡸ࡯ࡸࡵࡨࡶࡸࡺࡡࡤ࡭࠱ࡷࡪࡴࡤࡌࡧࡼࡷࠬࠪ"),
+  bstack11_opy_ (u"ࠬࡧࡵࡵࡱ࡚ࡥ࡮ࡺࠧࠫ"): bstack11_opy_ (u"࠭ࡢࡳࡱࡺࡷࡪࡸࡳࡵࡣࡦ࡯࠳ࡧࡵࡵࡱ࡚ࡥ࡮ࡺࠧࠬ"),
+  bstack11_opy_ (u"ࠧࡩࡱࡶࡸࡸ࠭࠭"): bstack11_opy_ (u"ࠨࡤࡵࡳࡼࡹࡥࡳࡵࡷࡥࡨࡱ࠮ࡩࡱࡶࡸࡸ࠭࠮"),
+  bstack11_opy_ (u"ࠩࡥࡪࡨࡧࡣࡩࡧࠪ࠯"): bstack11_opy_ (u"ࠪࡦࡷࡵࡷࡴࡧࡵࡷࡹࡧࡣ࡬࠰ࡥࡪࡨࡧࡣࡩࡧࠪ࠰"),
+  bstack11_opy_ (u"ࠫࡼࡹࡌࡰࡥࡤࡰࡘࡻࡰࡱࡱࡵࡸࠬ࠱"): bstack11_opy_ (u"ࠬࡨࡲࡰࡹࡶࡩࡷࡹࡴࡢࡥ࡮࠲ࡼࡹࡌࡰࡥࡤࡰࡘࡻࡰࡱࡱࡵࡸࠬ࠲"),
+  bstack11_opy_ (u"࠭ࡤࡪࡵࡤࡦࡱ࡫ࡃࡰࡴࡶࡖࡪࡹࡴࡳ࡫ࡦࡸ࡮ࡵ࡮ࡴࠩ࠳"): bstack11_opy_ (u"ࠧࡣࡴࡲࡻࡸ࡫ࡲࡴࡶࡤࡧࡰ࠴ࡤࡪࡵࡤࡦࡱ࡫ࡃࡰࡴࡶࡖࡪࡹࡴࡳ࡫ࡦࡸ࡮ࡵ࡮ࡴࠩ࠴"),
+  bstack11_opy_ (u"ࠨࡦࡨࡺ࡮ࡩࡥࡏࡣࡰࡩࠬ࠵"): bstack11_opy_ (u"ࠩࡧࡩࡻ࡯ࡣࡦࠩ࠶"),
+  bstack11_opy_ (u"ࠪࡶࡪࡧ࡬ࡎࡱࡥ࡭ࡱ࡫ࠧ࠷"): bstack11_opy_ (u"ࠫࡷ࡫ࡡ࡭ࡡࡰࡳࡧ࡯࡬ࡦࠩ࠸"),
+  bstack11_opy_ (u"ࠬࡧࡰࡱ࡫ࡸࡱ࡛࡫ࡲࡴ࡫ࡲࡲࠬ࠹"): bstack11_opy_ (u"࠭ࡢࡳࡱࡺࡷࡪࡸࡳࡵࡣࡦ࡯࠳ࡧࡰࡱ࡫ࡸࡱࡤࡼࡥࡳࡵ࡬ࡳࡳ࠭࠺"),
+  bstack11_opy_ (u"ࠧࡤࡷࡶࡸࡴࡳࡎࡦࡶࡺࡳࡷࡱࠧ࠻"): bstack11_opy_ (u"ࠨࡤࡵࡳࡼࡹࡥࡳࡵࡷࡥࡨࡱ࠮ࡤࡷࡶࡸࡴࡳࡎࡦࡶࡺࡳࡷࡱࠧ࠼"),
+  bstack11_opy_ (u"ࠩࡱࡩࡹࡽ࡯ࡳ࡭ࡓࡶࡴ࡬ࡩ࡭ࡧࠪ࠽"): bstack11_opy_ (u"ࠪࡦࡷࡵࡷࡴࡧࡵࡷࡹࡧࡣ࡬࠰ࡱࡩࡹࡽ࡯ࡳ࡭ࡓࡶࡴ࡬ࡩ࡭ࡧࠪ࠾"),
+  bstack11_opy_ (u"ࠫࡦࡩࡣࡦࡲࡷࡍࡳࡹࡥࡤࡷࡵࡩࡈ࡫ࡲࡵࡵࠪ࠿"): bstack11_opy_ (u"ࠬࡧࡣࡤࡧࡳࡸࡘࡹ࡬ࡄࡧࡵࡸࡸ࠭ࡀ"),
+  bstack11_opy_ (u"࠭ࡢࡳࡱࡺࡷࡪࡸࡳࡵࡣࡦ࡯ࡘࡊࡋࠨࡁ"): bstack11_opy_ (u"ࠧࡣࡴࡲࡻࡸ࡫ࡲࡴࡶࡤࡧࡰ࠴ࡢࡳࡱࡺࡷࡪࡸࡳࡵࡣࡦ࡯ࡘࡊࡋࠨࡂ"),
+  bstack11_opy_ (u"ࠨࡵࡲࡹࡷࡩࡥࠨࡃ"): bstack11_opy_ (u"ࠩࡥࡶࡴࡽࡳࡦࡴࡶࡸࡦࡩ࡫࠯ࡵࡲࡹࡷࡩࡥࠨࡄ"),
+  bstack11_opy_ (u"ࠪࡦࡺ࡯࡬ࡥࡋࡧࡩࡳࡺࡩࡧ࡫ࡨࡶࠬࡅ"): bstack11_opy_ (u"ࠫࡧࡸ࡯ࡸࡵࡨࡶࡸࡺࡡࡤ࡭࠱ࡦࡺ࡯࡬ࡥࡋࡧࡩࡳࡺࡩࡧ࡫ࡨࡶࠬࡆ"),
+  bstack11_opy_ (u"ࠬ࡮࡯ࡴࡶࡑࡥࡲ࡫ࠧࡇ"): bstack11_opy_ (u"࠭ࡢࡳࡱࡺࡷࡪࡸࡳࡵࡣࡦ࡯࠳࡮࡯ࡴࡶࡑࡥࡲ࡫ࠧࡈ"),
 }
-bstack11l11l_opy_ = [
-  bstack1ll1_opy_ (u"ࠧࡰࡵࠪࡉ"),
-  bstack1ll1_opy_ (u"ࠨࡱࡶ࡚ࡪࡸࡳࡪࡱࡱࠫࡊ"),
-  bstack1ll1_opy_ (u"ࠩࡶࡩࡱ࡫࡮ࡪࡷࡰ࡚ࡪࡸࡳࡪࡱࡱࠫࡋ"),
-  bstack1ll1_opy_ (u"ࠪࡷࡪࡹࡳࡪࡱࡱࡒࡦࡳࡥࠨࡌ"),
-  bstack1ll1_opy_ (u"ࠫࡩ࡫ࡶࡪࡥࡨࡒࡦࡳࡥࠨࡍ"),
-  bstack1ll1_opy_ (u"ࠬࡸࡥࡢ࡮ࡐࡳࡧ࡯࡬ࡦࠩࡎ"),
-  bstack1ll1_opy_ (u"࠭ࡡࡱࡲ࡬ࡹࡲ࡜ࡥࡳࡵ࡬ࡳࡳ࠭ࡏ"),
+bstack1l1lllll1_opy_ = [
+  bstack11_opy_ (u"ࠧࡰࡵࠪࡉ"),
+  bstack11_opy_ (u"ࠨࡱࡶ࡚ࡪࡸࡳࡪࡱࡱࠫࡊ"),
+  bstack11_opy_ (u"ࠩࡶࡩࡱ࡫࡮ࡪࡷࡰ࡚ࡪࡸࡳࡪࡱࡱࠫࡋ"),
+  bstack11_opy_ (u"ࠪࡷࡪࡹࡳࡪࡱࡱࡒࡦࡳࡥࠨࡌ"),
+  bstack11_opy_ (u"ࠫࡩ࡫ࡶࡪࡥࡨࡒࡦࡳࡥࠨࡍ"),
+  bstack11_opy_ (u"ࠬࡸࡥࡢ࡮ࡐࡳࡧ࡯࡬ࡦࠩࡎ"),
+  bstack11_opy_ (u"࠭ࡡࡱࡲ࡬ࡹࡲ࡜ࡥࡳࡵ࡬ࡳࡳ࠭ࡏ"),
 ]
-bstack1l111l_opy_ = {
-  bstack1ll1_opy_ (u"ࠧࡶࡵࡨࡶࡓࡧ࡭ࡦࠩࡐ"): [bstack1ll1_opy_ (u"ࠨࡄࡕࡓ࡜࡙ࡅࡓࡕࡗࡅࡈࡑ࡟ࡖࡕࡈࡖࡓࡇࡍࡆࠩࡑ"), bstack1ll1_opy_ (u"ࠩࡅࡖࡔ࡝ࡓࡆࡔࡖࡘࡆࡉࡋࡠࡗࡖࡉࡗࡥࡎࡂࡏࡈࠫࡒ")],
-  bstack1ll1_opy_ (u"ࠪࡥࡨࡩࡥࡴࡵࡎࡩࡾ࠭ࡓ"): bstack1ll1_opy_ (u"ࠫࡇࡘࡏࡘࡕࡈࡖࡘ࡚ࡁࡄࡍࡢࡅࡈࡉࡅࡔࡕࡢࡏࡊ࡟ࠧࡔ"),
-  bstack1ll1_opy_ (u"ࠬࡨࡵࡪ࡮ࡧࡒࡦࡳࡥࠨࡕ"): bstack1ll1_opy_ (u"࠭ࡂࡓࡑ࡚ࡗࡊࡘࡓࡕࡃࡆࡏࡤࡈࡕࡊࡎࡇࡣࡓࡇࡍࡆࠩࡖ"),
-  bstack1ll1_opy_ (u"ࠧࡱࡴࡲ࡮ࡪࡩࡴࡏࡣࡰࡩࠬࡗ"): bstack1ll1_opy_ (u"ࠨࡄࡕࡓ࡜࡙ࡅࡓࡕࡗࡅࡈࡑ࡟ࡑࡔࡒࡎࡊࡉࡔࡠࡐࡄࡑࡊ࠭ࡘ"),
-  bstack1ll1_opy_ (u"ࠩࡥࡹ࡮ࡲࡤࡊࡦࡨࡲࡹ࡯ࡦࡪࡧࡵ࡙ࠫ"): bstack1ll1_opy_ (u"ࠪࡆࡗࡕࡗࡔࡇࡕࡗ࡙ࡇࡃࡌࡡࡅ࡙ࡎࡒࡄࡠࡋࡇࡉࡓ࡚ࡉࡇࡋࡈࡖ࡚ࠬ"),
-  bstack1ll1_opy_ (u"ࠫࡵࡧࡲࡢ࡮࡯ࡩࡱࡹࡐࡦࡴࡓࡰࡦࡺࡦࡰࡴࡰ࡛ࠫ"): bstack1ll1_opy_ (u"ࠬࡈࡒࡐ࡙ࡖࡉࡗ࡙ࡔࡂࡅࡎࡣࡕࡇࡒࡂࡎࡏࡉࡑ࡙࡟ࡑࡇࡕࡣࡕࡒࡁࡕࡈࡒࡖࡒ࠭࡜"),
-  bstack1ll1_opy_ (u"࠭ࡢࡳࡱࡺࡷࡪࡸࡳࡵࡣࡦ࡯ࡑࡵࡣࡢ࡮ࠪ࡝"): bstack1ll1_opy_ (u"ࠧࡃࡔࡒ࡛ࡘࡋࡒࡔࡖࡄࡇࡐࡥࡌࡐࡅࡄࡐࠬ࡞"),
-  bstack1ll1_opy_ (u"ࠨࡴࡨࡶࡺࡴࡔࡦࡵࡷࡷࠬ࡟"): bstack1ll1_opy_ (u"ࠩࡅࡖࡔ࡝ࡓࡆࡔࡖࡘࡆࡉࡋࡠࡔࡈࡖ࡚ࡔ࡟ࡕࡇࡖࡘࡘ࠭ࡠ"),
-  bstack1ll1_opy_ (u"ࠪࡥࡵࡶࠧࡡ"): bstack1ll1_opy_ (u"ࠫࡇࡘࡏࡘࡕࡈࡖࡘ࡚ࡁࡄࡍࡢࡅࡕࡖࠧࡢ"),
-  bstack1ll1_opy_ (u"ࠬࡲ࡯ࡨࡎࡨࡺࡪࡲࠧࡣ"): bstack1ll1_opy_ (u"࠭ࡂࡓࡑ࡚ࡗࡊࡘࡓࡕࡃࡆࡏࡤࡕࡂࡔࡇࡕ࡚ࡆࡈࡉࡍࡋࡗ࡝ࡤࡊࡅࡃࡗࡊࠫࡤ"),
-  bstack1ll1_opy_ (u"ࠧࡢࡷࡷࡳࡲࡧࡴࡪࡱࡱࠫࡥ"): bstack1ll1_opy_ (u"ࠨࡄࡕࡓ࡜࡙ࡅࡓࡕࡗࡅࡈࡑ࡟ࡂࡗࡗࡓࡒࡇࡔࡊࡑࡑࠫࡦ")
+bstack1ll111ll_opy_ = {
+  bstack11_opy_ (u"ࠧࡶࡵࡨࡶࡓࡧ࡭ࡦࠩࡐ"): [bstack11_opy_ (u"ࠨࡄࡕࡓ࡜࡙ࡅࡓࡕࡗࡅࡈࡑ࡟ࡖࡕࡈࡖࡓࡇࡍࡆࠩࡑ"), bstack11_opy_ (u"ࠩࡅࡖࡔ࡝ࡓࡆࡔࡖࡘࡆࡉࡋࡠࡗࡖࡉࡗࡥࡎࡂࡏࡈࠫࡒ")],
+  bstack11_opy_ (u"ࠪࡥࡨࡩࡥࡴࡵࡎࡩࡾ࠭ࡓ"): bstack11_opy_ (u"ࠫࡇࡘࡏࡘࡕࡈࡖࡘ࡚ࡁࡄࡍࡢࡅࡈࡉࡅࡔࡕࡢࡏࡊ࡟ࠧࡔ"),
+  bstack11_opy_ (u"ࠬࡨࡵࡪ࡮ࡧࡒࡦࡳࡥࠨࡕ"): bstack11_opy_ (u"࠭ࡂࡓࡑ࡚ࡗࡊࡘࡓࡕࡃࡆࡏࡤࡈࡕࡊࡎࡇࡣࡓࡇࡍࡆࠩࡖ"),
+  bstack11_opy_ (u"ࠧࡱࡴࡲ࡮ࡪࡩࡴࡏࡣࡰࡩࠬࡗ"): bstack11_opy_ (u"ࠨࡄࡕࡓ࡜࡙ࡅࡓࡕࡗࡅࡈࡑ࡟ࡑࡔࡒࡎࡊࡉࡔࡠࡐࡄࡑࡊ࠭ࡘ"),
+  bstack11_opy_ (u"ࠩࡥࡹ࡮ࡲࡤࡊࡦࡨࡲࡹ࡯ࡦࡪࡧࡵ࡙ࠫ"): bstack11_opy_ (u"ࠪࡆࡗࡕࡗࡔࡇࡕࡗ࡙ࡇࡃࡌࡡࡅ࡙ࡎࡒࡄࡠࡋࡇࡉࡓ࡚ࡉࡇࡋࡈࡖ࡚ࠬ"),
+  bstack11_opy_ (u"ࠫࡵࡧࡲࡢ࡮࡯ࡩࡱࡹࡐࡦࡴࡓࡰࡦࡺࡦࡰࡴࡰ࡛ࠫ"): bstack11_opy_ (u"ࠬࡈࡒࡐ࡙ࡖࡉࡗ࡙ࡔࡂࡅࡎࡣࡕࡇࡒࡂࡎࡏࡉࡑ࡙࡟ࡑࡇࡕࡣࡕࡒࡁࡕࡈࡒࡖࡒ࠭࡜"),
+  bstack11_opy_ (u"࠭ࡢࡳࡱࡺࡷࡪࡸࡳࡵࡣࡦ࡯ࡑࡵࡣࡢ࡮ࠪ࡝"): bstack11_opy_ (u"ࠧࡃࡔࡒ࡛ࡘࡋࡒࡔࡖࡄࡇࡐࡥࡌࡐࡅࡄࡐࠬ࡞"),
+  bstack11_opy_ (u"ࠨࡴࡨࡶࡺࡴࡔࡦࡵࡷࡷࠬ࡟"): bstack11_opy_ (u"ࠩࡅࡖࡔ࡝ࡓࡆࡔࡖࡘࡆࡉࡋࡠࡔࡈࡖ࡚ࡔ࡟ࡕࡇࡖࡘࡘ࠭ࡠ"),
+  bstack11_opy_ (u"ࠪࡥࡵࡶࠧࡡ"): bstack11_opy_ (u"ࠫࡇࡘࡏࡘࡕࡈࡖࡘ࡚ࡁࡄࡍࡢࡅࡕࡖࠧࡢ"),
+  bstack11_opy_ (u"ࠬࡲ࡯ࡨࡎࡨࡺࡪࡲࠧࡣ"): bstack11_opy_ (u"࠭ࡂࡓࡑ࡚ࡗࡊࡘࡓࡕࡃࡆࡏࡤࡕࡂࡔࡇࡕ࡚ࡆࡈࡉࡍࡋࡗ࡝ࡤࡊࡅࡃࡗࡊࠫࡤ"),
+  bstack11_opy_ (u"ࠧࡢࡷࡷࡳࡲࡧࡴࡪࡱࡱࠫࡥ"): bstack11_opy_ (u"ࠨࡄࡕࡓ࡜࡙ࡅࡓࡕࡗࡅࡈࡑ࡟ࡂࡗࡗࡓࡒࡇࡔࡊࡑࡑࠫࡦ")
 }
-bstack11l11lll_opy_ = {
-  bstack1ll1_opy_ (u"ࠩࡸࡷࡪࡸࡎࡢ࡯ࡨࠫࡧ"): [bstack1ll1_opy_ (u"ࠪࡦࡷࡵࡷࡴࡧࡵࡷࡹࡧࡣ࡬࠰ࡸࡷࡪࡸ࡟࡯ࡣࡰࡩࠬࡨ"), bstack1ll1_opy_ (u"ࠫࡧࡸ࡯ࡸࡵࡨࡶࡸࡺࡡࡤ࡭࠱ࡹࡸ࡫ࡲࡏࡣࡰࡩࠬࡩ")],
-  bstack1ll1_opy_ (u"ࠬࡧࡣࡤࡧࡶࡷࡐ࡫ࡹࠨࡪ"): [bstack1ll1_opy_ (u"࠭ࡢࡳࡱࡺࡷࡪࡸࡳࡵࡣࡦ࡯࠳ࡧࡣࡤࡧࡶࡷࡤࡱࡥࡺࠩ࡫"), bstack1ll1_opy_ (u"ࠧࡣࡴࡲࡻࡸ࡫ࡲࡴࡶࡤࡧࡰ࠴ࡡࡤࡥࡨࡷࡸࡑࡥࡺࠩ࡬")],
-  bstack1ll1_opy_ (u"ࠨࡤࡸ࡭ࡱࡪࡎࡢ࡯ࡨࠫ࡭"): bstack1ll1_opy_ (u"ࠩࡥࡶࡴࡽࡳࡦࡴࡶࡸࡦࡩ࡫࠯ࡤࡸ࡭ࡱࡪࡎࡢ࡯ࡨࠫ࡮"),
-  bstack1ll1_opy_ (u"ࠪࡴࡷࡵࡪࡦࡥࡷࡒࡦࡳࡥࠨ࡯"): bstack1ll1_opy_ (u"ࠫࡧࡸ࡯ࡸࡵࡨࡶࡸࡺࡡࡤ࡭࠱ࡴࡷࡵࡪࡦࡥࡷࡒࡦࡳࡥࠨࡰ"),
-  bstack1ll1_opy_ (u"ࠬࡨࡵࡪ࡮ࡧࡍࡩ࡫࡮ࡵ࡫ࡩ࡭ࡪࡸࠧࡱ"): bstack1ll1_opy_ (u"࠭ࡢࡳࡱࡺࡷࡪࡸࡳࡵࡣࡦ࡯࠳ࡨࡵࡪ࡮ࡧࡍࡩ࡫࡮ࡵ࡫ࡩ࡭ࡪࡸࠧࡲ"),
-  bstack1ll1_opy_ (u"ࠧࡱࡣࡵࡥࡱࡲࡥ࡭ࡵࡓࡩࡷࡖ࡬ࡢࡶࡩࡳࡷࡳࠧࡳ"): [bstack1ll1_opy_ (u"ࠨࡤࡵࡳࡼࡹࡥࡳࡵࡷࡥࡨࡱ࠮ࡱࡲࡳࠫࡴ"), bstack1ll1_opy_ (u"ࠩࡥࡶࡴࡽࡳࡦࡴࡶࡸࡦࡩ࡫࠯ࡲࡤࡶࡦࡲ࡬ࡦ࡮ࡶࡔࡪࡸࡐ࡭ࡣࡷࡪࡴࡸ࡭ࠨࡵ")],
-  bstack1ll1_opy_ (u"ࠪࡦࡷࡵࡷࡴࡧࡵࡷࡹࡧࡣ࡬ࡎࡲࡧࡦࡲࠧࡶ"): bstack1ll1_opy_ (u"ࠫࡧࡸ࡯ࡸࡵࡨࡶࡸࡺࡡࡤ࡭࠱ࡰࡴࡩࡡ࡭ࠩࡷ"),
-  bstack1ll1_opy_ (u"ࠬࡸࡥࡳࡷࡱࡘࡪࡹࡴࡴࠩࡸ"): bstack1ll1_opy_ (u"࠭ࡢࡳࡱࡺࡷࡪࡸࡳࡵࡣࡦ࡯࠳ࡸࡥࡳࡷࡱࡘࡪࡹࡴࡴࠩࡹ"),
-  bstack1ll1_opy_ (u"ࠧࡢࡲࡳࠫࡺ"): bstack1ll1_opy_ (u"ࠨࡤࡵࡳࡼࡹࡥࡳࡵࡷࡥࡨࡱ࠮ࡢࡲࡳࠫࡻ"),
-  bstack1ll1_opy_ (u"ࠩ࡯ࡳ࡬ࡒࡥࡷࡧ࡯ࠫࡼ"): bstack1ll1_opy_ (u"ࠪࡦࡷࡵࡷࡴࡧࡵࡷࡹࡧࡣ࡬࠰࡯ࡳ࡬ࡒࡥࡷࡧ࡯ࠫࡽ"),
-  bstack1ll1_opy_ (u"ࠫࡦࡻࡴࡰ࡯ࡤࡸ࡮ࡵ࡮ࠨࡾ"): bstack1ll1_opy_ (u"ࠬࡨࡲࡰࡹࡶࡩࡷࡹࡴࡢࡥ࡮࠲ࡦࡻࡴࡰ࡯ࡤࡸ࡮ࡵ࡮ࠨࡿ")
+bstack1ll111111_opy_ = {
+  bstack11_opy_ (u"ࠩࡸࡷࡪࡸࡎࡢ࡯ࡨࠫࡧ"): [bstack11_opy_ (u"ࠪࡦࡷࡵࡷࡴࡧࡵࡷࡹࡧࡣ࡬࠰ࡸࡷࡪࡸ࡟࡯ࡣࡰࡩࠬࡨ"), bstack11_opy_ (u"ࠫࡧࡸ࡯ࡸࡵࡨࡶࡸࡺࡡࡤ࡭࠱ࡹࡸ࡫ࡲࡏࡣࡰࡩࠬࡩ")],
+  bstack11_opy_ (u"ࠬࡧࡣࡤࡧࡶࡷࡐ࡫ࡹࠨࡪ"): [bstack11_opy_ (u"࠭ࡢࡳࡱࡺࡷࡪࡸࡳࡵࡣࡦ࡯࠳ࡧࡣࡤࡧࡶࡷࡤࡱࡥࡺࠩ࡫"), bstack11_opy_ (u"ࠧࡣࡴࡲࡻࡸ࡫ࡲࡴࡶࡤࡧࡰ࠴ࡡࡤࡥࡨࡷࡸࡑࡥࡺࠩ࡬")],
+  bstack11_opy_ (u"ࠨࡤࡸ࡭ࡱࡪࡎࡢ࡯ࡨࠫ࡭"): bstack11_opy_ (u"ࠩࡥࡶࡴࡽࡳࡦࡴࡶࡸࡦࡩ࡫࠯ࡤࡸ࡭ࡱࡪࡎࡢ࡯ࡨࠫ࡮"),
+  bstack11_opy_ (u"ࠪࡴࡷࡵࡪࡦࡥࡷࡒࡦࡳࡥࠨ࡯"): bstack11_opy_ (u"ࠫࡧࡸ࡯ࡸࡵࡨࡶࡸࡺࡡࡤ࡭࠱ࡴࡷࡵࡪࡦࡥࡷࡒࡦࡳࡥࠨࡰ"),
+  bstack11_opy_ (u"ࠬࡨࡵࡪ࡮ࡧࡍࡩ࡫࡮ࡵ࡫ࡩ࡭ࡪࡸࠧࡱ"): bstack11_opy_ (u"࠭ࡢࡳࡱࡺࡷࡪࡸࡳࡵࡣࡦ࡯࠳ࡨࡵࡪ࡮ࡧࡍࡩ࡫࡮ࡵ࡫ࡩ࡭ࡪࡸࠧࡲ"),
+  bstack11_opy_ (u"ࠧࡱࡣࡵࡥࡱࡲࡥ࡭ࡵࡓࡩࡷࡖ࡬ࡢࡶࡩࡳࡷࡳࠧࡳ"): [bstack11_opy_ (u"ࠨࡤࡵࡳࡼࡹࡥࡳࡵࡷࡥࡨࡱ࠮ࡱࡲࡳࠫࡴ"), bstack11_opy_ (u"ࠩࡥࡶࡴࡽࡳࡦࡴࡶࡸࡦࡩ࡫࠯ࡲࡤࡶࡦࡲ࡬ࡦ࡮ࡶࡔࡪࡸࡐ࡭ࡣࡷࡪࡴࡸ࡭ࠨࡵ")],
+  bstack11_opy_ (u"ࠪࡦࡷࡵࡷࡴࡧࡵࡷࡹࡧࡣ࡬ࡎࡲࡧࡦࡲࠧࡶ"): bstack11_opy_ (u"ࠫࡧࡸ࡯ࡸࡵࡨࡶࡸࡺࡡࡤ࡭࠱ࡰࡴࡩࡡ࡭ࠩࡷ"),
+  bstack11_opy_ (u"ࠬࡸࡥࡳࡷࡱࡘࡪࡹࡴࡴࠩࡸ"): bstack11_opy_ (u"࠭ࡢࡳࡱࡺࡷࡪࡸࡳࡵࡣࡦ࡯࠳ࡸࡥࡳࡷࡱࡘࡪࡹࡴࡴࠩࡹ"),
+  bstack11_opy_ (u"ࠧࡢࡲࡳࠫࡺ"): bstack11_opy_ (u"ࠨࡤࡵࡳࡼࡹࡥࡳࡵࡷࡥࡨࡱ࠮ࡢࡲࡳࠫࡻ"),
+  bstack11_opy_ (u"ࠩ࡯ࡳ࡬ࡒࡥࡷࡧ࡯ࠫࡼ"): bstack11_opy_ (u"ࠪࡦࡷࡵࡷࡴࡧࡵࡷࡹࡧࡣ࡬࠰࡯ࡳ࡬ࡒࡥࡷࡧ࡯ࠫࡽ"),
+  bstack11_opy_ (u"ࠫࡦࡻࡴࡰ࡯ࡤࡸ࡮ࡵ࡮ࠨࡾ"): bstack11_opy_ (u"ࠬࡨࡲࡰࡹࡶࡩࡷࡹࡴࡢࡥ࡮࠲ࡦࡻࡴࡰ࡯ࡤࡸ࡮ࡵ࡮ࠨࡿ")
 }
-bstack1l1ll1111_opy_ = {
-  bstack1ll1_opy_ (u"࠭࡯ࡴࡘࡨࡶࡸ࡯࡯࡯ࠩࢀ"): bstack1ll1_opy_ (u"ࠧࡰࡵࡢࡺࡪࡸࡳࡪࡱࡱࠫࢁ"),
-  bstack1ll1_opy_ (u"ࠨࡵࡨࡰࡪࡴࡩࡶ࡯࡙ࡩࡷࡹࡩࡰࡰࠪࢂ"): [bstack1ll1_opy_ (u"ࠩࡥࡶࡴࡽࡳࡦࡴࡶࡸࡦࡩ࡫࠯ࡵࡨࡰࡪࡴࡩࡶ࡯ࡢࡺࡪࡸࡳࡪࡱࡱࠫࢃ"), bstack1ll1_opy_ (u"ࠪࡷࡪࡲࡥ࡯࡫ࡸࡱࡤࡼࡥࡳࡵ࡬ࡳࡳ࠭ࢄ")],
-  bstack1ll1_opy_ (u"ࠫࡸ࡫ࡳࡴ࡫ࡲࡲࡓࡧ࡭ࡦࠩࢅ"): bstack1ll1_opy_ (u"ࠬࡴࡡ࡮ࡧࠪࢆ"),
-  bstack1ll1_opy_ (u"࠭ࡤࡦࡸ࡬ࡧࡪࡔࡡ࡮ࡧࠪࢇ"): bstack1ll1_opy_ (u"ࠧࡥࡧࡹ࡭ࡨ࡫ࠧ࢈"),
-  bstack1ll1_opy_ (u"ࠨࡤࡵࡳࡼࡹࡥࡳࡐࡤࡱࡪ࠭ࢉ"): [bstack1ll1_opy_ (u"ࠩࡥࡶࡴࡽࡳࡦࡴࠪࢊ"), bstack1ll1_opy_ (u"ࠪࡦࡷࡵࡷࡴࡧࡵࡣࡳࡧ࡭ࡦࠩࢋ")],
-  bstack1ll1_opy_ (u"ࠫࡧࡸ࡯ࡸࡵࡨࡶ࡛࡫ࡲࡴ࡫ࡲࡲࠬࢌ"): bstack1ll1_opy_ (u"ࠬࡨࡲࡰࡹࡶࡩࡷࡥࡶࡦࡴࡶ࡭ࡴࡴࠧࢍ"),
-  bstack1ll1_opy_ (u"࠭ࡲࡦࡣ࡯ࡑࡴࡨࡩ࡭ࡧࠪࢎ"): bstack1ll1_opy_ (u"ࠧࡳࡧࡤࡰࡤࡳ࡯ࡣ࡫࡯ࡩࠬ࢏"),
-  bstack1ll1_opy_ (u"ࠨࡣࡳࡴ࡮ࡻ࡭ࡗࡧࡵࡷ࡮ࡵ࡮ࠨ࢐"): [bstack1ll1_opy_ (u"ࠩࡥࡶࡴࡽࡳࡦࡴࡶࡸࡦࡩ࡫࠯ࡣࡳࡴ࡮ࡻ࡭ࡠࡸࡨࡶࡸ࡯࡯࡯ࠩ࢑"), bstack1ll1_opy_ (u"ࠪࡥࡵࡶࡩࡶ࡯ࡢࡺࡪࡸࡳࡪࡱࡱࠫ࢒")],
-  bstack1ll1_opy_ (u"ࠫࡦࡩࡣࡦࡲࡷࡍࡳࡹࡥࡤࡷࡵࡩࡈ࡫ࡲࡵࡵࠪ࢓"): [bstack1ll1_opy_ (u"ࠬࡧࡣࡤࡧࡳࡸࡘࡹ࡬ࡄࡧࡵࡸࡸ࠭࢔"), bstack1ll1_opy_ (u"࠭ࡡࡤࡥࡨࡴࡹ࡙ࡳ࡭ࡅࡨࡶࡹ࠭࢕")]
+bstack1ll111l1l_opy_ = {
+  bstack11_opy_ (u"࠭࡯ࡴࡘࡨࡶࡸ࡯࡯࡯ࠩࢀ"): bstack11_opy_ (u"ࠧࡰࡵࡢࡺࡪࡸࡳࡪࡱࡱࠫࢁ"),
+  bstack11_opy_ (u"ࠨࡵࡨࡰࡪࡴࡩࡶ࡯࡙ࡩࡷࡹࡩࡰࡰࠪࢂ"): [bstack11_opy_ (u"ࠩࡥࡶࡴࡽࡳࡦࡴࡶࡸࡦࡩ࡫࠯ࡵࡨࡰࡪࡴࡩࡶ࡯ࡢࡺࡪࡸࡳࡪࡱࡱࠫࢃ"), bstack11_opy_ (u"ࠪࡷࡪࡲࡥ࡯࡫ࡸࡱࡤࡼࡥࡳࡵ࡬ࡳࡳ࠭ࢄ")],
+  bstack11_opy_ (u"ࠫࡸ࡫ࡳࡴ࡫ࡲࡲࡓࡧ࡭ࡦࠩࢅ"): bstack11_opy_ (u"ࠬࡴࡡ࡮ࡧࠪࢆ"),
+  bstack11_opy_ (u"࠭ࡤࡦࡸ࡬ࡧࡪࡔࡡ࡮ࡧࠪࢇ"): bstack11_opy_ (u"ࠧࡥࡧࡹ࡭ࡨ࡫ࠧ࢈"),
+  bstack11_opy_ (u"ࠨࡤࡵࡳࡼࡹࡥࡳࡐࡤࡱࡪ࠭ࢉ"): [bstack11_opy_ (u"ࠩࡥࡶࡴࡽࡳࡦࡴࠪࢊ"), bstack11_opy_ (u"ࠪࡦࡷࡵࡷࡴࡧࡵࡣࡳࡧ࡭ࡦࠩࢋ")],
+  bstack11_opy_ (u"ࠫࡧࡸ࡯ࡸࡵࡨࡶ࡛࡫ࡲࡴ࡫ࡲࡲࠬࢌ"): bstack11_opy_ (u"ࠬࡨࡲࡰࡹࡶࡩࡷࡥࡶࡦࡴࡶ࡭ࡴࡴࠧࢍ"),
+  bstack11_opy_ (u"࠭ࡲࡦࡣ࡯ࡑࡴࡨࡩ࡭ࡧࠪࢎ"): bstack11_opy_ (u"ࠧࡳࡧࡤࡰࡤࡳ࡯ࡣ࡫࡯ࡩࠬ࢏"),
+  bstack11_opy_ (u"ࠨࡣࡳࡴ࡮ࡻ࡭ࡗࡧࡵࡷ࡮ࡵ࡮ࠨ࢐"): [bstack11_opy_ (u"ࠩࡥࡶࡴࡽࡳࡦࡴࡶࡸࡦࡩ࡫࠯ࡣࡳࡴ࡮ࡻ࡭ࡠࡸࡨࡶࡸ࡯࡯࡯ࠩ࢑"), bstack11_opy_ (u"ࠪࡥࡵࡶࡩࡶ࡯ࡢࡺࡪࡸࡳࡪࡱࡱࠫ࢒")],
+  bstack11_opy_ (u"ࠫࡦࡩࡣࡦࡲࡷࡍࡳࡹࡥࡤࡷࡵࡩࡈ࡫ࡲࡵࡵࠪ࢓"): [bstack11_opy_ (u"ࠬࡧࡣࡤࡧࡳࡸࡘࡹ࡬ࡄࡧࡵࡸࡸ࠭࢔"), bstack11_opy_ (u"࠭ࡡࡤࡥࡨࡴࡹ࡙ࡳ࡭ࡅࡨࡶࡹ࠭࢕")]
 }
-bstack111ll_opy_ = [
-  bstack1ll1_opy_ (u"ࠧࡢࡥࡦࡩࡵࡺࡉ࡯ࡵࡨࡧࡺࡸࡥࡄࡧࡵࡸࡸ࠭࢖"),
-  bstack1ll1_opy_ (u"ࠨࡲࡤ࡫ࡪࡒ࡯ࡢࡦࡖࡸࡷࡧࡴࡦࡩࡼࠫࢗ"),
-  bstack1ll1_opy_ (u"ࠩࡳࡶࡴࡾࡹࠨ࢘"),
-  bstack1ll1_opy_ (u"ࠪࡷࡪࡺࡗࡪࡰࡧࡳࡼࡘࡥࡤࡶ࢙ࠪ"),
-  bstack1ll1_opy_ (u"ࠫࡹ࡯࡭ࡦࡱࡸࡸࡸ࢚࠭"),
-  bstack1ll1_opy_ (u"ࠬࡹࡴࡳ࡫ࡦࡸࡋ࡯࡬ࡦࡋࡱࡸࡪࡸࡡࡤࡶࡤࡦ࡮ࡲࡩࡵࡻ࢛ࠪ"),
-  bstack1ll1_opy_ (u"࠭ࡵ࡯ࡪࡤࡲࡩࡲࡥࡥࡒࡵࡳࡲࡶࡴࡃࡧ࡫ࡥࡻ࡯࡯ࡳࠩ࢜"),
-  bstack1ll1_opy_ (u"ࠧࡨࡱࡲ࡫࠿ࡩࡨࡳࡱࡰࡩࡔࡶࡴࡪࡱࡱࡷࠬ࢝"),
-  bstack1ll1_opy_ (u"ࠨ࡯ࡲࡾ࠿࡬ࡩࡳࡧࡩࡳࡽࡕࡰࡵ࡫ࡲࡲࡸ࠭࢞"),
-  bstack1ll1_opy_ (u"ࠩࡰࡷ࠿࡫ࡤࡨࡧࡒࡴࡹ࡯࡯࡯ࡵࠪ࢟"),
-  bstack1ll1_opy_ (u"ࠪࡷࡪࡀࡩࡦࡑࡳࡸ࡮ࡵ࡮ࡴࠩࢠ"),
-  bstack1ll1_opy_ (u"ࠫࡸࡧࡦࡢࡴ࡬࠲ࡴࡶࡴࡪࡱࡱࡷࠬࢡ"),
+bstack1l11ll11l_opy_ = [
+  bstack11_opy_ (u"ࠧࡢࡥࡦࡩࡵࡺࡉ࡯ࡵࡨࡧࡺࡸࡥࡄࡧࡵࡸࡸ࠭࢖"),
+  bstack11_opy_ (u"ࠨࡲࡤ࡫ࡪࡒ࡯ࡢࡦࡖࡸࡷࡧࡴࡦࡩࡼࠫࢗ"),
+  bstack11_opy_ (u"ࠩࡳࡶࡴࡾࡹࠨ࢘"),
+  bstack11_opy_ (u"ࠪࡷࡪࡺࡗࡪࡰࡧࡳࡼࡘࡥࡤࡶ࢙ࠪ"),
+  bstack11_opy_ (u"ࠫࡹ࡯࡭ࡦࡱࡸࡸࡸ࢚࠭"),
+  bstack11_opy_ (u"ࠬࡹࡴࡳ࡫ࡦࡸࡋ࡯࡬ࡦࡋࡱࡸࡪࡸࡡࡤࡶࡤࡦ࡮ࡲࡩࡵࡻ࢛ࠪ"),
+  bstack11_opy_ (u"࠭ࡵ࡯ࡪࡤࡲࡩࡲࡥࡥࡒࡵࡳࡲࡶࡴࡃࡧ࡫ࡥࡻ࡯࡯ࡳࠩ࢜"),
+  bstack11_opy_ (u"ࠧࡨࡱࡲ࡫࠿ࡩࡨࡳࡱࡰࡩࡔࡶࡴࡪࡱࡱࡷࠬ࢝"),
+  bstack11_opy_ (u"ࠨ࡯ࡲࡾ࠿࡬ࡩࡳࡧࡩࡳࡽࡕࡰࡵ࡫ࡲࡲࡸ࠭࢞"),
+  bstack11_opy_ (u"ࠩࡰࡷ࠿࡫ࡤࡨࡧࡒࡴࡹ࡯࡯࡯ࡵࠪ࢟"),
+  bstack11_opy_ (u"ࠪࡷࡪࡀࡩࡦࡑࡳࡸ࡮ࡵ࡮ࡴࠩࢠ"),
+  bstack11_opy_ (u"ࠫࡸࡧࡦࡢࡴ࡬࠲ࡴࡶࡴࡪࡱࡱࡷࠬࢡ"),
 ]
-bstack1llll_opy_ = [
-  bstack1ll1_opy_ (u"ࠬࡨࡲࡰࡹࡶࡩࡷࡹࡴࡢࡥ࡮ࡐࡴࡩࡡ࡭ࠩࢢ"),
-  bstack1ll1_opy_ (u"࠭ࡢࡳࡱࡺࡷࡪࡸࡓࡵࡣࡦ࡯ࡑࡵࡣࡢ࡮ࡒࡴࡹ࡯࡯࡯ࡵࠪࢣ"),
-  bstack1ll1_opy_ (u"ࠧ࡭ࡱࡦࡥࡱࡕࡰࡵ࡫ࡲࡲࡸ࠭ࢤ"),
-  bstack1ll1_opy_ (u"ࠨࡲࡤࡶࡦࡲ࡬ࡦ࡮ࡶࡔࡪࡸࡐ࡭ࡣࡷࡪࡴࡸ࡭ࠨࢥ"),
-  bstack1ll1_opy_ (u"ࠩࡳࡰࡦࡺࡦࡰࡴࡰࡷࠬࢦ"),
-  bstack1ll1_opy_ (u"ࠪࡰࡴ࡭ࡌࡦࡸࡨࡰࠬࢧ"),
-  bstack1ll1_opy_ (u"ࠫ࡭ࡺࡴࡱࡒࡵࡳࡽࡿࠧࢨ"),
-  bstack1ll1_opy_ (u"ࠬ࡮ࡴࡵࡲࡶࡔࡷࡵࡸࡺࠩࢩ"),
-  bstack1ll1_opy_ (u"࠭ࡦࡳࡣࡰࡩࡼࡵࡲ࡬ࠩࢪ"),
+bstack1l111l1_opy_ = [
+  bstack11_opy_ (u"ࠬࡨࡲࡰࡹࡶࡩࡷࡹࡴࡢࡥ࡮ࡐࡴࡩࡡ࡭ࠩࢢ"),
+  bstack11_opy_ (u"࠭ࡢࡳࡱࡺࡷࡪࡸࡓࡵࡣࡦ࡯ࡑࡵࡣࡢ࡮ࡒࡴࡹ࡯࡯࡯ࡵࠪࢣ"),
+  bstack11_opy_ (u"ࠧ࡭ࡱࡦࡥࡱࡕࡰࡵ࡫ࡲࡲࡸ࠭ࢤ"),
+  bstack11_opy_ (u"ࠨࡲࡤࡶࡦࡲ࡬ࡦ࡮ࡶࡔࡪࡸࡐ࡭ࡣࡷࡪࡴࡸ࡭ࠨࢥ"),
+  bstack11_opy_ (u"ࠩࡳࡰࡦࡺࡦࡰࡴࡰࡷࠬࢦ"),
+  bstack11_opy_ (u"ࠪࡰࡴ࡭ࡌࡦࡸࡨࡰࠬࢧ"),
+  bstack11_opy_ (u"ࠫ࡭ࡺࡴࡱࡒࡵࡳࡽࡿࠧࢨ"),
+  bstack11_opy_ (u"ࠬ࡮ࡴࡵࡲࡶࡔࡷࡵࡸࡺࠩࢩ"),
+  bstack11_opy_ (u"࠭ࡦࡳࡣࡰࡩࡼࡵࡲ࡬ࠩࢪ"),
 ]
-bstack1lll1l1l_opy_ = [
-  bstack1ll1_opy_ (u"ࠧࡶࡲ࡯ࡳࡦࡪࡍࡦࡦ࡬ࡥࠬࢫ"),
-  bstack1ll1_opy_ (u"ࠨࡷࡶࡩࡷࡔࡡ࡮ࡧࠪࢬ"),
-  bstack1ll1_opy_ (u"ࠩࡤࡧࡨ࡫ࡳࡴࡍࡨࡽࠬࢭ"),
-  bstack1ll1_opy_ (u"ࠪࡷࡪࡹࡳࡪࡱࡱࡒࡦࡳࡥࠨࢮ"),
-  bstack1ll1_opy_ (u"ࠫࡹ࡫ࡳࡵࡒࡵ࡭ࡴࡸࡩࡵࡻࠪࢯ"),
-  bstack1ll1_opy_ (u"ࠬࡨࡵࡪ࡮ࡧࡒࡦࡳࡥࠨࢰ"),
-  bstack1ll1_opy_ (u"࠭ࡢࡶ࡫࡯ࡨ࡙ࡧࡧࠨࢱ"),
-  bstack1ll1_opy_ (u"ࠧࡱࡴࡲ࡮ࡪࡩࡴࡏࡣࡰࡩࠬࢲ"),
-  bstack1ll1_opy_ (u"ࠨࡵࡨࡰࡪࡴࡩࡶ࡯࡙ࡩࡷࡹࡩࡰࡰࠪࢳ"),
-  bstack1ll1_opy_ (u"ࠩࡥࡶࡴࡽࡳࡦࡴࡑࡥࡲ࡫ࠧࢴ"),
-  bstack1ll1_opy_ (u"ࠪࡦࡷࡵࡷࡴࡧࡵ࡚ࡪࡸࡳࡪࡱࡱࠫࢵ"),
-  bstack1ll1_opy_ (u"ࠫࡱࡵࡣࡢ࡮ࠪࢶ"),
-  bstack1ll1_opy_ (u"ࠬࡵࡳࠨࢷ"),
-  bstack1ll1_opy_ (u"࠭࡯ࡴࡘࡨࡶࡸ࡯࡯࡯ࠩࢸ"),
-  bstack1ll1_opy_ (u"ࠧࡩࡱࡶࡸࡸ࠭ࢹ"),
-  bstack1ll1_opy_ (u"ࠨࡣࡸࡸࡴ࡝ࡡࡪࡶࠪࢺ"),
-  bstack1ll1_opy_ (u"ࠩࡵࡩ࡬࡯࡯࡯ࠩࢻ"),
-  bstack1ll1_opy_ (u"ࠪࡸ࡮ࡳࡥࡻࡱࡱࡩࠬࢼ"),
-  bstack1ll1_opy_ (u"ࠫࡲࡧࡣࡩ࡫ࡱࡩࠬࢽ"),
-  bstack1ll1_opy_ (u"ࠬࡸࡥࡴࡱ࡯ࡹࡹ࡯࡯࡯ࠩࢾ"),
-  bstack1ll1_opy_ (u"࠭ࡩࡥ࡮ࡨࡘ࡮ࡳࡥࡰࡷࡷࠫࢿ"),
-  bstack1ll1_opy_ (u"ࠧࡥࡧࡹ࡭ࡨ࡫ࡏࡳ࡫ࡨࡲࡹࡧࡴࡪࡱࡱࠫࣀ"),
-  bstack1ll1_opy_ (u"ࠨࡸ࡬ࡨࡪࡵࠧࣁ"),
-  bstack1ll1_opy_ (u"ࠩࡱࡳࡕࡧࡧࡦࡎࡲࡥࡩ࡚ࡩ࡮ࡧࡲࡹࡹ࠭ࣂ"),
-  bstack1ll1_opy_ (u"ࠪࡦ࡫ࡩࡡࡤࡪࡨࠫࣃ"),
-  bstack1ll1_opy_ (u"ࠫࡩ࡫ࡢࡶࡩࠪࣄ"),
-  bstack1ll1_opy_ (u"ࠬࡩࡵࡴࡶࡲࡱࡘࡩࡲࡦࡧࡱࡷ࡭ࡵࡴࡴࠩࣅ"),
-  bstack1ll1_opy_ (u"࠭ࡣࡶࡵࡷࡳࡲ࡙ࡥ࡯ࡦࡎࡩࡾࡹࠧࣆ"),
-  bstack1ll1_opy_ (u"ࠧࡳࡧࡤࡰࡒࡵࡢࡪ࡮ࡨࠫࣇ"),
-  bstack1ll1_opy_ (u"ࠨࡰࡲࡔ࡮ࡶࡥ࡭࡫ࡱࡩࠬࣈ"),
-  bstack1ll1_opy_ (u"ࠩࡦ࡬ࡪࡩ࡫ࡖࡔࡏࠫࣉ"),
-  bstack1ll1_opy_ (u"ࠪࡰࡴࡩࡡ࡭ࡋࡧࡩࡳࡺࡩࡧ࡫ࡨࡶࠬ࣊"),
-  bstack1ll1_opy_ (u"ࠫࡦࡩࡣࡦࡲࡷࡇࡴࡵ࡫ࡪࡧࡶࠫ࣋"),
-  bstack1ll1_opy_ (u"ࠬࡩࡡࡱࡶࡸࡶࡪࡉࡲࡢࡵ࡫ࠫ࣌"),
-  bstack1ll1_opy_ (u"࠭ࡤࡦࡸ࡬ࡧࡪࡔࡡ࡮ࡧࠪ࣍"),
-  bstack1ll1_opy_ (u"ࠧࡢࡲࡳ࡭ࡺࡳࡖࡦࡴࡶ࡭ࡴࡴࠧ࣎"),
-  bstack1ll1_opy_ (u"ࠨࡣࡸࡸࡴࡳࡡࡵ࡫ࡲࡲ࡛࡫ࡲࡴ࡫ࡲࡲ࣏ࠬ"),
-  bstack1ll1_opy_ (u"ࠩࡱࡳࡇࡲࡡ࡯࡭ࡓࡳࡱࡲࡩ࡯ࡩ࣐ࠪ"),
-  bstack1ll1_opy_ (u"ࠪࡱࡦࡹ࡫ࡔࡧࡱࡨࡐ࡫ࡹࡴ࣑ࠩ"),
-  bstack1ll1_opy_ (u"ࠫࡩ࡫ࡶࡪࡥࡨࡐࡴ࡭ࡳࠨ࣒"),
-  bstack1ll1_opy_ (u"ࠬࡪࡥࡷ࡫ࡦࡩࡎࡪ࣓ࠧ"),
-  bstack1ll1_opy_ (u"࠭ࡤࡦࡦ࡬ࡧࡦࡺࡥࡥࡆࡨࡺ࡮ࡩࡥࠨࣔ"),
-  bstack1ll1_opy_ (u"ࠧࡩࡧࡤࡨࡪࡸࡐࡢࡴࡤࡱࡸ࠭ࣕ"),
-  bstack1ll1_opy_ (u"ࠨࡲ࡫ࡳࡳ࡫ࡎࡶ࡯ࡥࡩࡷ࠭ࣖ"),
-  bstack1ll1_opy_ (u"ࠩࡱࡩࡹࡽ࡯ࡳ࡭ࡏࡳ࡬ࡹࠧࣗ"),
-  bstack1ll1_opy_ (u"ࠪࡲࡪࡺࡷࡰࡴ࡮ࡐࡴ࡭ࡳࡐࡲࡷ࡭ࡴࡴࡳࠨࣘ"),
-  bstack1ll1_opy_ (u"ࠫࡨࡵ࡮ࡴࡱ࡯ࡩࡑࡵࡧࡴࠩࣙ"),
-  bstack1ll1_opy_ (u"ࠬࡻࡳࡦ࡙࠶ࡇࠬࣚ"),
-  bstack1ll1_opy_ (u"࠭ࡡࡱࡲ࡬ࡹࡲࡒ࡯ࡨࡵࠪࣛ"),
-  bstack1ll1_opy_ (u"ࠧࡦࡰࡤࡦࡱ࡫ࡂࡪࡱࡰࡩࡹࡸࡩࡤࠩࣜ"),
-  bstack1ll1_opy_ (u"ࠨࡸ࡬ࡨࡪࡵࡖ࠳ࠩࣝ"),
-  bstack1ll1_opy_ (u"ࠩࡰ࡭ࡩ࡙ࡥࡴࡵ࡬ࡳࡳࡏ࡮ࡴࡶࡤࡰࡱࡇࡰࡱࡵࠪࣞ"),
-  bstack1ll1_opy_ (u"ࠪࡩࡸࡶࡲࡦࡵࡶࡳࡘ࡫ࡲࡷࡧࡵࠫࣟ"),
-  bstack1ll1_opy_ (u"ࠫࡸ࡫࡬ࡦࡰ࡬ࡹࡲࡒ࡯ࡨࡵࠪ࣠"),
-  bstack1ll1_opy_ (u"ࠬࡹࡥ࡭ࡧࡱ࡭ࡺࡳࡃࡥࡲࠪ࣡"),
-  bstack1ll1_opy_ (u"࠭ࡴࡦ࡮ࡨࡱࡪࡺࡲࡺࡎࡲ࡫ࡸ࠭࣢"),
-  bstack1ll1_opy_ (u"ࠧࡴࡻࡱࡧ࡙࡯࡭ࡦ࡙࡬ࡸ࡭ࡔࡔࡑࣣࠩ"),
-  bstack1ll1_opy_ (u"ࠨࡩࡨࡳࡑࡵࡣࡢࡶ࡬ࡳࡳ࠭ࣤ"),
-  bstack1ll1_opy_ (u"ࠩࡪࡴࡸࡒ࡯ࡤࡣࡷ࡭ࡴࡴࠧࣥ"),
-  bstack1ll1_opy_ (u"ࠪࡲࡪࡺࡷࡰࡴ࡮ࡔࡷࡵࡦࡪ࡮ࡨࣦࠫ"),
-  bstack1ll1_opy_ (u"ࠫࡨࡻࡳࡵࡱࡰࡒࡪࡺࡷࡰࡴ࡮ࠫࣧ"),
-  bstack1ll1_opy_ (u"ࠬ࡬࡯ࡳࡥࡨࡇ࡭ࡧ࡮ࡨࡧࡍࡥࡷ࠭ࣨ"),
-  bstack1ll1_opy_ (u"࠭ࡸ࡮ࡵࡍࡥࡷࣩ࠭"),
-  bstack1ll1_opy_ (u"ࠧࡹ࡯ࡻࡎࡦࡸࠧ࣪"),
-  bstack1ll1_opy_ (u"ࠨ࡯ࡤࡷࡰࡉ࡯࡮࡯ࡤࡲࡩࡹࠧ࣫"),
-  bstack1ll1_opy_ (u"ࠩࡰࡥࡸࡱࡂࡢࡵ࡬ࡧࡆࡻࡴࡩࠩ࣬"),
-  bstack1ll1_opy_ (u"ࠪࡻࡸࡒ࡯ࡤࡣ࡯ࡗࡺࡶࡰࡰࡴࡷ࣭ࠫ"),
-  bstack1ll1_opy_ (u"ࠫࡩ࡯ࡳࡢࡤ࡯ࡩࡈࡵࡲࡴࡔࡨࡷࡹࡸࡩࡤࡶ࡬ࡳࡳࡹ࣮ࠧ"),
-  bstack1ll1_opy_ (u"ࠬࡧࡰࡱࡘࡨࡶࡸ࡯࡯࡯࣯ࠩ"),
-  bstack1ll1_opy_ (u"࠭ࡡࡤࡥࡨࡴࡹࡏ࡮ࡴࡧࡦࡹࡷ࡫ࡃࡦࡴࡷࡷࣰࠬ"),
-  bstack1ll1_opy_ (u"ࠧࡳࡧࡶ࡭࡬ࡴࡁࡱࡲࣱࠪ"),
-  bstack1ll1_opy_ (u"ࠨࡦ࡬ࡷࡦࡨ࡬ࡦࡃࡱ࡭ࡲࡧࡴࡪࡱࡱࡷࣲࠬ"),
-  bstack1ll1_opy_ (u"ࠩࡦࡥࡳࡧࡲࡺࠩࣳ"),
-  bstack1ll1_opy_ (u"ࠪࡪ࡮ࡸࡥࡧࡱࡻࠫࣴ"),
-  bstack1ll1_opy_ (u"ࠫࡨ࡮ࡲࡰ࡯ࡨࠫࣵ"),
-  bstack1ll1_opy_ (u"ࠬ࡯ࡥࠨࣶ"),
-  bstack1ll1_opy_ (u"࠭ࡥࡥࡩࡨࠫࣷ"),
-  bstack1ll1_opy_ (u"ࠧࡴࡣࡩࡥࡷ࡯ࠧࣸ"),
-  bstack1ll1_opy_ (u"ࠨࡳࡸࡩࡺ࡫ࣹࠧ"),
-  bstack1ll1_opy_ (u"ࠩ࡬ࡲࡹ࡫ࡲ࡯ࡣ࡯ࣺࠫ"),
-  bstack1ll1_opy_ (u"ࠪࡥࡵࡶࡓࡵࡱࡵࡩࡈࡵ࡮ࡧ࡫ࡪࡹࡷࡧࡴࡪࡱࡱࠫࣻ"),
-  bstack1ll1_opy_ (u"ࠫࡪࡴࡡࡣ࡮ࡨࡇࡦࡳࡥࡳࡣࡌࡱࡦ࡭ࡥࡊࡰ࡭ࡩࡨࡺࡩࡰࡰࠪࣼ"),
-  bstack1ll1_opy_ (u"ࠬࡴࡥࡵࡹࡲࡶࡰࡒ࡯ࡨࡵࡈࡼࡨࡲࡵࡥࡧࡋࡳࡸࡺࡳࠨࣽ"),
-  bstack1ll1_opy_ (u"࠭࡮ࡦࡶࡺࡳࡷࡱࡌࡰࡩࡶࡍࡳࡩ࡬ࡶࡦࡨࡌࡴࡹࡴࡴࠩࣾ"),
-  bstack1ll1_opy_ (u"ࠧࡶࡲࡧࡥࡹ࡫ࡁࡱࡲࡖࡩࡹࡺࡩ࡯ࡩࡶࠫࣿ"),
-  bstack1ll1_opy_ (u"ࠨࡴࡨࡷࡪࡸࡶࡦࡆࡨࡺ࡮ࡩࡥࠨऀ"),
-  bstack1ll1_opy_ (u"ࠩࡶࡳࡺࡸࡣࡦࠩँ"),
-  bstack1ll1_opy_ (u"ࠪࡷࡪࡴࡤࡌࡧࡼࡷࠬं"),
-  bstack1ll1_opy_ (u"ࠫࡪࡴࡡࡣ࡮ࡨࡔࡦࡹࡳࡤࡱࡧࡩࠬः"),
-  bstack1ll1_opy_ (u"ࠬࡻࡰࡥࡣࡷࡩࡎࡵࡳࡅࡧࡹ࡭ࡨ࡫ࡓࡦࡶࡷ࡭ࡳ࡭ࡳࠨऄ"),
-  bstack1ll1_opy_ (u"࠭ࡥ࡯ࡣࡥࡰࡪࡇࡵࡥ࡫ࡲࡍࡳࡰࡥࡤࡶ࡬ࡳࡳ࠭अ"),
-  bstack1ll1_opy_ (u"ࠧࡦࡰࡤࡦࡱ࡫ࡁࡱࡲ࡯ࡩࡕࡧࡹࠨआ"),
-  bstack1ll1_opy_ (u"ࠨࡤࡵࡳࡼࡹࡥࡳࠩइ"),
-  bstack1ll1_opy_ (u"ࠩࡺࡨ࡮ࡵࡓࡦࡴࡹ࡭ࡨ࡫ࠧई"),
-  bstack1ll1_opy_ (u"ࠪࡦࡷࡵࡷࡴࡧࡵࡷࡹࡧࡣ࡬ࡕࡇࡏࠬउ"),
-  bstack1ll1_opy_ (u"ࠫࡵࡸࡥࡷࡧࡱࡸࡈࡸ࡯ࡴࡵࡖ࡭ࡹ࡫ࡔࡳࡣࡦ࡯࡮ࡴࡧࠨऊ"),
-  bstack1ll1_opy_ (u"ࠬ࡮ࡩࡨࡪࡆࡳࡳࡺࡲࡢࡵࡷࠫऋ"),
-  bstack1ll1_opy_ (u"࠭ࡤࡦࡸ࡬ࡧࡪࡖࡲࡦࡨࡨࡶࡪࡴࡣࡦࡵࠪऌ"),
-  bstack1ll1_opy_ (u"ࠧࡦࡰࡤࡦࡱ࡫ࡓࡪ࡯ࠪऍ"),
-  bstack1ll1_opy_ (u"ࠨࡵ࡬ࡱࡔࡶࡴࡪࡱࡱࡷࠬऎ"),
-  bstack1ll1_opy_ (u"ࠩࡵࡩࡲࡵࡶࡦࡋࡒࡗࡆࡶࡰࡔࡧࡷࡸ࡮ࡴࡧࡴࡎࡲࡧࡦࡲࡩࡻࡣࡷ࡭ࡴࡴࠧए"),
-  bstack1ll1_opy_ (u"ࠪ࡬ࡴࡹࡴࡏࡣࡰࡩࠬऐ"),
-  bstack1ll1_opy_ (u"ࠫࡧࡻࡩ࡭ࡦࡌࡨࡪࡴࡴࡪࡨ࡬ࡩࡷ࠭ऑ"),
-  bstack1ll1_opy_ (u"ࠬࡶ࡬ࡢࡶࡩࡳࡷࡳࠧऒ"),
-  bstack1ll1_opy_ (u"࠭ࡰ࡭ࡣࡷࡪࡴࡸ࡭ࡏࡣࡰࡩࠬओ"),
-  bstack1ll1_opy_ (u"ࠧࡱ࡮ࡤࡸ࡫ࡵࡲ࡮ࡘࡨࡶࡸ࡯࡯࡯ࠩऔ"),
-  bstack1ll1_opy_ (u"ࠨࡲࡤ࡫ࡪࡒ࡯ࡢࡦࡖࡸࡷࡧࡴࡦࡩࡼࠫक"),
-  bstack1ll1_opy_ (u"ࠩࡳࡶࡴࡾࡹࠨख"),
-  bstack1ll1_opy_ (u"ࠪࡸ࡮ࡳࡥࡰࡷࡷࡷࠬग"),
-  bstack1ll1_opy_ (u"ࠫࡺࡴࡨࡢࡰࡧࡰࡪࡪࡐࡳࡱࡰࡴࡹࡈࡥࡩࡣࡹ࡭ࡴࡸࠧघ")
+bstack111l1l11_opy_ = [
+  bstack11_opy_ (u"ࠧࡶࡲ࡯ࡳࡦࡪࡍࡦࡦ࡬ࡥࠬࢫ"),
+  bstack11_opy_ (u"ࠨࡷࡶࡩࡷࡔࡡ࡮ࡧࠪࢬ"),
+  bstack11_opy_ (u"ࠩࡤࡧࡨ࡫ࡳࡴࡍࡨࡽࠬࢭ"),
+  bstack11_opy_ (u"ࠪࡷࡪࡹࡳࡪࡱࡱࡒࡦࡳࡥࠨࢮ"),
+  bstack11_opy_ (u"ࠫࡹ࡫ࡳࡵࡒࡵ࡭ࡴࡸࡩࡵࡻࠪࢯ"),
+  bstack11_opy_ (u"ࠬࡨࡵࡪ࡮ࡧࡒࡦࡳࡥࠨࢰ"),
+  bstack11_opy_ (u"࠭ࡢࡶ࡫࡯ࡨ࡙ࡧࡧࠨࢱ"),
+  bstack11_opy_ (u"ࠧࡱࡴࡲ࡮ࡪࡩࡴࡏࡣࡰࡩࠬࢲ"),
+  bstack11_opy_ (u"ࠨࡵࡨࡰࡪࡴࡩࡶ࡯࡙ࡩࡷࡹࡩࡰࡰࠪࢳ"),
+  bstack11_opy_ (u"ࠩࡥࡶࡴࡽࡳࡦࡴࡑࡥࡲ࡫ࠧࢴ"),
+  bstack11_opy_ (u"ࠪࡦࡷࡵࡷࡴࡧࡵ࡚ࡪࡸࡳࡪࡱࡱࠫࢵ"),
+  bstack11_opy_ (u"ࠫࡱࡵࡣࡢ࡮ࠪࢶ"),
+  bstack11_opy_ (u"ࠬࡵࡳࠨࢷ"),
+  bstack11_opy_ (u"࠭࡯ࡴࡘࡨࡶࡸ࡯࡯࡯ࠩࢸ"),
+  bstack11_opy_ (u"ࠧࡩࡱࡶࡸࡸ࠭ࢹ"),
+  bstack11_opy_ (u"ࠨࡣࡸࡸࡴ࡝ࡡࡪࡶࠪࢺ"),
+  bstack11_opy_ (u"ࠩࡵࡩ࡬࡯࡯࡯ࠩࢻ"),
+  bstack11_opy_ (u"ࠪࡸ࡮ࡳࡥࡻࡱࡱࡩࠬࢼ"),
+  bstack11_opy_ (u"ࠫࡲࡧࡣࡩ࡫ࡱࡩࠬࢽ"),
+  bstack11_opy_ (u"ࠬࡸࡥࡴࡱ࡯ࡹࡹ࡯࡯࡯ࠩࢾ"),
+  bstack11_opy_ (u"࠭ࡩࡥ࡮ࡨࡘ࡮ࡳࡥࡰࡷࡷࠫࢿ"),
+  bstack11_opy_ (u"ࠧࡥࡧࡹ࡭ࡨ࡫ࡏࡳ࡫ࡨࡲࡹࡧࡴࡪࡱࡱࠫࣀ"),
+  bstack11_opy_ (u"ࠨࡸ࡬ࡨࡪࡵࠧࣁ"),
+  bstack11_opy_ (u"ࠩࡱࡳࡕࡧࡧࡦࡎࡲࡥࡩ࡚ࡩ࡮ࡧࡲࡹࡹ࠭ࣂ"),
+  bstack11_opy_ (u"ࠪࡦ࡫ࡩࡡࡤࡪࡨࠫࣃ"),
+  bstack11_opy_ (u"ࠫࡩ࡫ࡢࡶࡩࠪࣄ"),
+  bstack11_opy_ (u"ࠬࡩࡵࡴࡶࡲࡱࡘࡩࡲࡦࡧࡱࡷ࡭ࡵࡴࡴࠩࣅ"),
+  bstack11_opy_ (u"࠭ࡣࡶࡵࡷࡳࡲ࡙ࡥ࡯ࡦࡎࡩࡾࡹࠧࣆ"),
+  bstack11_opy_ (u"ࠧࡳࡧࡤࡰࡒࡵࡢࡪ࡮ࡨࠫࣇ"),
+  bstack11_opy_ (u"ࠨࡰࡲࡔ࡮ࡶࡥ࡭࡫ࡱࡩࠬࣈ"),
+  bstack11_opy_ (u"ࠩࡦ࡬ࡪࡩ࡫ࡖࡔࡏࠫࣉ"),
+  bstack11_opy_ (u"ࠪࡰࡴࡩࡡ࡭ࡋࡧࡩࡳࡺࡩࡧ࡫ࡨࡶࠬ࣊"),
+  bstack11_opy_ (u"ࠫࡦࡩࡣࡦࡲࡷࡇࡴࡵ࡫ࡪࡧࡶࠫ࣋"),
+  bstack11_opy_ (u"ࠬࡩࡡࡱࡶࡸࡶࡪࡉࡲࡢࡵ࡫ࠫ࣌"),
+  bstack11_opy_ (u"࠭ࡤࡦࡸ࡬ࡧࡪࡔࡡ࡮ࡧࠪ࣍"),
+  bstack11_opy_ (u"ࠧࡢࡲࡳ࡭ࡺࡳࡖࡦࡴࡶ࡭ࡴࡴࠧ࣎"),
+  bstack11_opy_ (u"ࠨࡣࡸࡸࡴࡳࡡࡵ࡫ࡲࡲ࡛࡫ࡲࡴ࡫ࡲࡲ࣏ࠬ"),
+  bstack11_opy_ (u"ࠩࡱࡳࡇࡲࡡ࡯࡭ࡓࡳࡱࡲࡩ࡯ࡩ࣐ࠪ"),
+  bstack11_opy_ (u"ࠪࡱࡦࡹ࡫ࡔࡧࡱࡨࡐ࡫ࡹࡴ࣑ࠩ"),
+  bstack11_opy_ (u"ࠫࡩ࡫ࡶࡪࡥࡨࡐࡴ࡭ࡳࠨ࣒"),
+  bstack11_opy_ (u"ࠬࡪࡥࡷ࡫ࡦࡩࡎࡪ࣓ࠧ"),
+  bstack11_opy_ (u"࠭ࡤࡦࡦ࡬ࡧࡦࡺࡥࡥࡆࡨࡺ࡮ࡩࡥࠨࣔ"),
+  bstack11_opy_ (u"ࠧࡩࡧࡤࡨࡪࡸࡐࡢࡴࡤࡱࡸ࠭ࣕ"),
+  bstack11_opy_ (u"ࠨࡲ࡫ࡳࡳ࡫ࡎࡶ࡯ࡥࡩࡷ࠭ࣖ"),
+  bstack11_opy_ (u"ࠩࡱࡩࡹࡽ࡯ࡳ࡭ࡏࡳ࡬ࡹࠧࣗ"),
+  bstack11_opy_ (u"ࠪࡲࡪࡺࡷࡰࡴ࡮ࡐࡴ࡭ࡳࡐࡲࡷ࡭ࡴࡴࡳࠨࣘ"),
+  bstack11_opy_ (u"ࠫࡨࡵ࡮ࡴࡱ࡯ࡩࡑࡵࡧࡴࠩࣙ"),
+  bstack11_opy_ (u"ࠬࡻࡳࡦ࡙࠶ࡇࠬࣚ"),
+  bstack11_opy_ (u"࠭ࡡࡱࡲ࡬ࡹࡲࡒ࡯ࡨࡵࠪࣛ"),
+  bstack11_opy_ (u"ࠧࡦࡰࡤࡦࡱ࡫ࡂࡪࡱࡰࡩࡹࡸࡩࡤࠩࣜ"),
+  bstack11_opy_ (u"ࠨࡸ࡬ࡨࡪࡵࡖ࠳ࠩࣝ"),
+  bstack11_opy_ (u"ࠩࡰ࡭ࡩ࡙ࡥࡴࡵ࡬ࡳࡳࡏ࡮ࡴࡶࡤࡰࡱࡇࡰࡱࡵࠪࣞ"),
+  bstack11_opy_ (u"ࠪࡩࡸࡶࡲࡦࡵࡶࡳࡘ࡫ࡲࡷࡧࡵࠫࣟ"),
+  bstack11_opy_ (u"ࠫࡸ࡫࡬ࡦࡰ࡬ࡹࡲࡒ࡯ࡨࡵࠪ࣠"),
+  bstack11_opy_ (u"ࠬࡹࡥ࡭ࡧࡱ࡭ࡺࡳࡃࡥࡲࠪ࣡"),
+  bstack11_opy_ (u"࠭ࡴࡦ࡮ࡨࡱࡪࡺࡲࡺࡎࡲ࡫ࡸ࠭࣢"),
+  bstack11_opy_ (u"ࠧࡴࡻࡱࡧ࡙࡯࡭ࡦ࡙࡬ࡸ࡭ࡔࡔࡑࣣࠩ"),
+  bstack11_opy_ (u"ࠨࡩࡨࡳࡑࡵࡣࡢࡶ࡬ࡳࡳ࠭ࣤ"),
+  bstack11_opy_ (u"ࠩࡪࡴࡸࡒ࡯ࡤࡣࡷ࡭ࡴࡴࠧࣥ"),
+  bstack11_opy_ (u"ࠪࡲࡪࡺࡷࡰࡴ࡮ࡔࡷࡵࡦࡪ࡮ࡨࣦࠫ"),
+  bstack11_opy_ (u"ࠫࡨࡻࡳࡵࡱࡰࡒࡪࡺࡷࡰࡴ࡮ࠫࣧ"),
+  bstack11_opy_ (u"ࠬ࡬࡯ࡳࡥࡨࡇ࡭ࡧ࡮ࡨࡧࡍࡥࡷ࠭ࣨ"),
+  bstack11_opy_ (u"࠭ࡸ࡮ࡵࡍࡥࡷࣩ࠭"),
+  bstack11_opy_ (u"ࠧࡹ࡯ࡻࡎࡦࡸࠧ࣪"),
+  bstack11_opy_ (u"ࠨ࡯ࡤࡷࡰࡉ࡯࡮࡯ࡤࡲࡩࡹࠧ࣫"),
+  bstack11_opy_ (u"ࠩࡰࡥࡸࡱࡂࡢࡵ࡬ࡧࡆࡻࡴࡩࠩ࣬"),
+  bstack11_opy_ (u"ࠪࡻࡸࡒ࡯ࡤࡣ࡯ࡗࡺࡶࡰࡰࡴࡷ࣭ࠫ"),
+  bstack11_opy_ (u"ࠫࡩ࡯ࡳࡢࡤ࡯ࡩࡈࡵࡲࡴࡔࡨࡷࡹࡸࡩࡤࡶ࡬ࡳࡳࡹ࣮ࠧ"),
+  bstack11_opy_ (u"ࠬࡧࡰࡱࡘࡨࡶࡸ࡯࡯࡯࣯ࠩ"),
+  bstack11_opy_ (u"࠭ࡡࡤࡥࡨࡴࡹࡏ࡮ࡴࡧࡦࡹࡷ࡫ࡃࡦࡴࡷࡷࣰࠬ"),
+  bstack11_opy_ (u"ࠧࡳࡧࡶ࡭࡬ࡴࡁࡱࡲࣱࠪ"),
+  bstack11_opy_ (u"ࠨࡦ࡬ࡷࡦࡨ࡬ࡦࡃࡱ࡭ࡲࡧࡴࡪࡱࡱࡷࣲࠬ"),
+  bstack11_opy_ (u"ࠩࡦࡥࡳࡧࡲࡺࠩࣳ"),
+  bstack11_opy_ (u"ࠪࡪ࡮ࡸࡥࡧࡱࡻࠫࣴ"),
+  bstack11_opy_ (u"ࠫࡨ࡮ࡲࡰ࡯ࡨࠫࣵ"),
+  bstack11_opy_ (u"ࠬ࡯ࡥࠨࣶ"),
+  bstack11_opy_ (u"࠭ࡥࡥࡩࡨࠫࣷ"),
+  bstack11_opy_ (u"ࠧࡴࡣࡩࡥࡷ࡯ࠧࣸ"),
+  bstack11_opy_ (u"ࠨࡳࡸࡩࡺ࡫ࣹࠧ"),
+  bstack11_opy_ (u"ࠩ࡬ࡲࡹ࡫ࡲ࡯ࡣ࡯ࣺࠫ"),
+  bstack11_opy_ (u"ࠪࡥࡵࡶࡓࡵࡱࡵࡩࡈࡵ࡮ࡧ࡫ࡪࡹࡷࡧࡴࡪࡱࡱࠫࣻ"),
+  bstack11_opy_ (u"ࠫࡪࡴࡡࡣ࡮ࡨࡇࡦࡳࡥࡳࡣࡌࡱࡦ࡭ࡥࡊࡰ࡭ࡩࡨࡺࡩࡰࡰࠪࣼ"),
+  bstack11_opy_ (u"ࠬࡴࡥࡵࡹࡲࡶࡰࡒ࡯ࡨࡵࡈࡼࡨࡲࡵࡥࡧࡋࡳࡸࡺࡳࠨࣽ"),
+  bstack11_opy_ (u"࠭࡮ࡦࡶࡺࡳࡷࡱࡌࡰࡩࡶࡍࡳࡩ࡬ࡶࡦࡨࡌࡴࡹࡴࡴࠩࣾ"),
+  bstack11_opy_ (u"ࠧࡶࡲࡧࡥࡹ࡫ࡁࡱࡲࡖࡩࡹࡺࡩ࡯ࡩࡶࠫࣿ"),
+  bstack11_opy_ (u"ࠨࡴࡨࡷࡪࡸࡶࡦࡆࡨࡺ࡮ࡩࡥࠨऀ"),
+  bstack11_opy_ (u"ࠩࡶࡳࡺࡸࡣࡦࠩँ"),
+  bstack11_opy_ (u"ࠪࡷࡪࡴࡤࡌࡧࡼࡷࠬं"),
+  bstack11_opy_ (u"ࠫࡪࡴࡡࡣ࡮ࡨࡔࡦࡹࡳࡤࡱࡧࡩࠬः"),
+  bstack11_opy_ (u"ࠬࡻࡰࡥࡣࡷࡩࡎࡵࡳࡅࡧࡹ࡭ࡨ࡫ࡓࡦࡶࡷ࡭ࡳ࡭ࡳࠨऄ"),
+  bstack11_opy_ (u"࠭ࡥ࡯ࡣࡥࡰࡪࡇࡵࡥ࡫ࡲࡍࡳࡰࡥࡤࡶ࡬ࡳࡳ࠭अ"),
+  bstack11_opy_ (u"ࠧࡦࡰࡤࡦࡱ࡫ࡁࡱࡲ࡯ࡩࡕࡧࡹࠨआ"),
+  bstack11_opy_ (u"ࠨࡤࡵࡳࡼࡹࡥࡳࠩइ"),
+  bstack11_opy_ (u"ࠩࡺࡨ࡮ࡵࡓࡦࡴࡹ࡭ࡨ࡫ࠧई"),
+  bstack11_opy_ (u"ࠪࡦࡷࡵࡷࡴࡧࡵࡷࡹࡧࡣ࡬ࡕࡇࡏࠬउ"),
+  bstack11_opy_ (u"ࠫࡵࡸࡥࡷࡧࡱࡸࡈࡸ࡯ࡴࡵࡖ࡭ࡹ࡫ࡔࡳࡣࡦ࡯࡮ࡴࡧࠨऊ"),
+  bstack11_opy_ (u"ࠬ࡮ࡩࡨࡪࡆࡳࡳࡺࡲࡢࡵࡷࠫऋ"),
+  bstack11_opy_ (u"࠭ࡤࡦࡸ࡬ࡧࡪࡖࡲࡦࡨࡨࡶࡪࡴࡣࡦࡵࠪऌ"),
+  bstack11_opy_ (u"ࠧࡦࡰࡤࡦࡱ࡫ࡓࡪ࡯ࠪऍ"),
+  bstack11_opy_ (u"ࠨࡵ࡬ࡱࡔࡶࡴࡪࡱࡱࡷࠬऎ"),
+  bstack11_opy_ (u"ࠩࡵࡩࡲࡵࡶࡦࡋࡒࡗࡆࡶࡰࡔࡧࡷࡸ࡮ࡴࡧࡴࡎࡲࡧࡦࡲࡩࡻࡣࡷ࡭ࡴࡴࠧए"),
+  bstack11_opy_ (u"ࠪ࡬ࡴࡹࡴࡏࡣࡰࡩࠬऐ"),
+  bstack11_opy_ (u"ࠫࡧࡻࡩ࡭ࡦࡌࡨࡪࡴࡴࡪࡨ࡬ࡩࡷ࠭ऑ"),
+  bstack11_opy_ (u"ࠬࡶ࡬ࡢࡶࡩࡳࡷࡳࠧऒ"),
+  bstack11_opy_ (u"࠭ࡰ࡭ࡣࡷࡪࡴࡸ࡭ࡏࡣࡰࡩࠬओ"),
+  bstack11_opy_ (u"ࠧࡱ࡮ࡤࡸ࡫ࡵࡲ࡮ࡘࡨࡶࡸ࡯࡯࡯ࠩऔ"),
+  bstack11_opy_ (u"ࠨࡲࡤ࡫ࡪࡒ࡯ࡢࡦࡖࡸࡷࡧࡴࡦࡩࡼࠫक"),
+  bstack11_opy_ (u"ࠩࡳࡶࡴࡾࡹࠨख"),
+  bstack11_opy_ (u"ࠪࡸ࡮ࡳࡥࡰࡷࡷࡷࠬग"),
+  bstack11_opy_ (u"ࠫࡺࡴࡨࡢࡰࡧࡰࡪࡪࡐࡳࡱࡰࡴࡹࡈࡥࡩࡣࡹ࡭ࡴࡸࠧघ")
 ]
-bstack1ll111l1l_opy_ = {
-  bstack1ll1_opy_ (u"ࠬࡼࠧङ"): bstack1ll1_opy_ (u"࠭ࡶࠨच"),
-  bstack1ll1_opy_ (u"ࠧࡧࠩछ"): bstack1ll1_opy_ (u"ࠨࡨࠪज"),
-  bstack1ll1_opy_ (u"ࠩࡩࡳࡷࡩࡥࠨझ"): bstack1ll1_opy_ (u"ࠪࡪࡴࡸࡣࡦࠩञ"),
-  bstack1ll1_opy_ (u"ࠫࡴࡴ࡬ࡺࡣࡸࡸࡴࡳࡡࡵࡧࠪट"): bstack1ll1_opy_ (u"ࠬࡵ࡮࡭ࡻࡄࡹࡹࡵ࡭ࡢࡶࡨࠫठ"),
-  bstack1ll1_opy_ (u"࠭ࡦࡰࡴࡦࡩࡱࡵࡣࡢ࡮ࠪड"): bstack1ll1_opy_ (u"ࠧࡧࡱࡵࡧࡪࡲ࡯ࡤࡣ࡯ࠫढ"),
-  bstack1ll1_opy_ (u"ࠨࡲࡵࡳࡽࡿࡨࡰࡵࡷࠫण"): bstack1ll1_opy_ (u"ࠩࡳࡶࡴࡾࡹࡉࡱࡶࡸࠬत"),
-  bstack1ll1_opy_ (u"ࠪࡴࡷࡵࡸࡺࡲࡲࡶࡹ࠭थ"): bstack1ll1_opy_ (u"ࠫࡵࡸ࡯ࡹࡻࡓࡳࡷࡺࠧद"),
-  bstack1ll1_opy_ (u"ࠬࡶࡲࡰࡺࡼࡹࡸ࡫ࡲࠨध"): bstack1ll1_opy_ (u"࠭ࡰࡳࡱࡻࡽ࡚ࡹࡥࡳࠩन"),
-  bstack1ll1_opy_ (u"ࠧࡱࡴࡲࡼࡾࡶࡡࡴࡵࠪऩ"): bstack1ll1_opy_ (u"ࠨࡲࡵࡳࡽࡿࡐࡢࡵࡶࠫप"),
-  bstack1ll1_opy_ (u"ࠩ࡯ࡳࡨࡧ࡬ࡱࡴࡲࡼࡾ࡮࡯ࡴࡶࠪफ"): bstack1ll1_opy_ (u"ࠪࡰࡴࡩࡡ࡭ࡒࡵࡳࡽࡿࡈࡰࡵࡷࠫब"),
-  bstack1ll1_opy_ (u"ࠫࡱࡵࡣࡢ࡮ࡳࡶࡴࡾࡹࡱࡱࡵࡸࠬभ"): bstack1ll1_opy_ (u"ࠬࡲ࡯ࡤࡣ࡯ࡔࡷࡵࡸࡺࡒࡲࡶࡹ࠭म"),
-  bstack1ll1_opy_ (u"࠭࡬ࡰࡥࡤࡰࡵࡸ࡯ࡹࡻࡸࡷࡪࡸࠧय"): bstack1ll1_opy_ (u"ࠧ࠮࡮ࡲࡧࡦࡲࡐࡳࡱࡻࡽ࡚ࡹࡥࡳࠩर"),
-  bstack1ll1_opy_ (u"ࠨ࠯࡯ࡳࡨࡧ࡬ࡱࡴࡲࡼࡾࡻࡳࡦࡴࠪऱ"): bstack1ll1_opy_ (u"ࠩ࠰ࡰࡴࡩࡡ࡭ࡒࡵࡳࡽࡿࡕࡴࡧࡵࠫल"),
-  bstack1ll1_opy_ (u"ࠪࡰࡴࡩࡡ࡭ࡲࡵࡳࡽࡿࡰࡢࡵࡶࠫळ"): bstack1ll1_opy_ (u"ࠫ࠲ࡲ࡯ࡤࡣ࡯ࡔࡷࡵࡸࡺࡒࡤࡷࡸ࠭ऴ"),
-  bstack1ll1_opy_ (u"ࠬ࠳࡬ࡰࡥࡤࡰࡵࡸ࡯ࡹࡻࡳࡥࡸࡹࠧव"): bstack1ll1_opy_ (u"࠭࠭࡭ࡱࡦࡥࡱࡖࡲࡰࡺࡼࡔࡦࡹࡳࠨश"),
-  bstack1ll1_opy_ (u"ࠧࡣ࡫ࡱࡥࡷࡿࡰࡢࡶ࡫ࠫष"): bstack1ll1_opy_ (u"ࠨࡤ࡬ࡲࡦࡸࡹࡱࡣࡷ࡬ࠬस"),
-  bstack1ll1_opy_ (u"ࠩࡳࡥࡨ࡬ࡩ࡭ࡧࠪह"): bstack1ll1_opy_ (u"ࠪ࠱ࡵࡧࡣ࠮ࡨ࡬ࡰࡪ࠭ऺ"),
-  bstack1ll1_opy_ (u"ࠫࡵࡧࡣ࠮ࡨ࡬ࡰࡪ࠭ऻ"): bstack1ll1_opy_ (u"ࠬ࠳ࡰࡢࡥ࠰ࡪ࡮ࡲࡥࠨ़"),
-  bstack1ll1_opy_ (u"࠭࠭ࡱࡣࡦ࠱࡫࡯࡬ࡦࠩऽ"): bstack1ll1_opy_ (u"ࠧ࠮ࡲࡤࡧ࠲࡬ࡩ࡭ࡧࠪा"),
-  bstack1ll1_opy_ (u"ࠨ࡮ࡲ࡫࡫࡯࡬ࡦࠩि"): bstack1ll1_opy_ (u"ࠩ࡯ࡳ࡬࡬ࡩ࡭ࡧࠪी"),
-  bstack1ll1_opy_ (u"ࠪࡰࡴࡩࡡ࡭࡫ࡧࡩࡳࡺࡩࡧ࡫ࡨࡶࠬु"): bstack1ll1_opy_ (u"ࠫࡱࡵࡣࡢ࡮ࡌࡨࡪࡴࡴࡪࡨ࡬ࡩࡷ࠭ू"),
+bstack1l111l1l1_opy_ = {
+  bstack11_opy_ (u"ࠬࡼࠧङ"): bstack11_opy_ (u"࠭ࡶࠨच"),
+  bstack11_opy_ (u"ࠧࡧࠩछ"): bstack11_opy_ (u"ࠨࡨࠪज"),
+  bstack11_opy_ (u"ࠩࡩࡳࡷࡩࡥࠨझ"): bstack11_opy_ (u"ࠪࡪࡴࡸࡣࡦࠩञ"),
+  bstack11_opy_ (u"ࠫࡴࡴ࡬ࡺࡣࡸࡸࡴࡳࡡࡵࡧࠪट"): bstack11_opy_ (u"ࠬࡵ࡮࡭ࡻࡄࡹࡹࡵ࡭ࡢࡶࡨࠫठ"),
+  bstack11_opy_ (u"࠭ࡦࡰࡴࡦࡩࡱࡵࡣࡢ࡮ࠪड"): bstack11_opy_ (u"ࠧࡧࡱࡵࡧࡪࡲ࡯ࡤࡣ࡯ࠫढ"),
+  bstack11_opy_ (u"ࠨࡲࡵࡳࡽࡿࡨࡰࡵࡷࠫण"): bstack11_opy_ (u"ࠩࡳࡶࡴࡾࡹࡉࡱࡶࡸࠬत"),
+  bstack11_opy_ (u"ࠪࡴࡷࡵࡸࡺࡲࡲࡶࡹ࠭थ"): bstack11_opy_ (u"ࠫࡵࡸ࡯ࡹࡻࡓࡳࡷࡺࠧद"),
+  bstack11_opy_ (u"ࠬࡶࡲࡰࡺࡼࡹࡸ࡫ࡲࠨध"): bstack11_opy_ (u"࠭ࡰࡳࡱࡻࡽ࡚ࡹࡥࡳࠩन"),
+  bstack11_opy_ (u"ࠧࡱࡴࡲࡼࡾࡶࡡࡴࡵࠪऩ"): bstack11_opy_ (u"ࠨࡲࡵࡳࡽࡿࡐࡢࡵࡶࠫप"),
+  bstack11_opy_ (u"ࠩ࡯ࡳࡨࡧ࡬ࡱࡴࡲࡼࡾ࡮࡯ࡴࡶࠪफ"): bstack11_opy_ (u"ࠪࡰࡴࡩࡡ࡭ࡒࡵࡳࡽࡿࡈࡰࡵࡷࠫब"),
+  bstack11_opy_ (u"ࠫࡱࡵࡣࡢ࡮ࡳࡶࡴࡾࡹࡱࡱࡵࡸࠬभ"): bstack11_opy_ (u"ࠬࡲ࡯ࡤࡣ࡯ࡔࡷࡵࡸࡺࡒࡲࡶࡹ࠭म"),
+  bstack11_opy_ (u"࠭࡬ࡰࡥࡤࡰࡵࡸ࡯ࡹࡻࡸࡷࡪࡸࠧय"): bstack11_opy_ (u"ࠧ࠮࡮ࡲࡧࡦࡲࡐࡳࡱࡻࡽ࡚ࡹࡥࡳࠩर"),
+  bstack11_opy_ (u"ࠨ࠯࡯ࡳࡨࡧ࡬ࡱࡴࡲࡼࡾࡻࡳࡦࡴࠪऱ"): bstack11_opy_ (u"ࠩ࠰ࡰࡴࡩࡡ࡭ࡒࡵࡳࡽࡿࡕࡴࡧࡵࠫल"),
+  bstack11_opy_ (u"ࠪࡰࡴࡩࡡ࡭ࡲࡵࡳࡽࡿࡰࡢࡵࡶࠫळ"): bstack11_opy_ (u"ࠫ࠲ࡲ࡯ࡤࡣ࡯ࡔࡷࡵࡸࡺࡒࡤࡷࡸ࠭ऴ"),
+  bstack11_opy_ (u"ࠬ࠳࡬ࡰࡥࡤࡰࡵࡸ࡯ࡹࡻࡳࡥࡸࡹࠧव"): bstack11_opy_ (u"࠭࠭࡭ࡱࡦࡥࡱࡖࡲࡰࡺࡼࡔࡦࡹࡳࠨश"),
+  bstack11_opy_ (u"ࠧࡣ࡫ࡱࡥࡷࡿࡰࡢࡶ࡫ࠫष"): bstack11_opy_ (u"ࠨࡤ࡬ࡲࡦࡸࡹࡱࡣࡷ࡬ࠬस"),
+  bstack11_opy_ (u"ࠩࡳࡥࡨ࡬ࡩ࡭ࡧࠪह"): bstack11_opy_ (u"ࠪ࠱ࡵࡧࡣ࠮ࡨ࡬ࡰࡪ࠭ऺ"),
+  bstack11_opy_ (u"ࠫࡵࡧࡣ࠮ࡨ࡬ࡰࡪ࠭ऻ"): bstack11_opy_ (u"ࠬ࠳ࡰࡢࡥ࠰ࡪ࡮ࡲࡥࠨ़"),
+  bstack11_opy_ (u"࠭࠭ࡱࡣࡦ࠱࡫࡯࡬ࡦࠩऽ"): bstack11_opy_ (u"ࠧ࠮ࡲࡤࡧ࠲࡬ࡩ࡭ࡧࠪा"),
+  bstack11_opy_ (u"ࠨ࡮ࡲ࡫࡫࡯࡬ࡦࠩि"): bstack11_opy_ (u"ࠩ࡯ࡳ࡬࡬ࡩ࡭ࡧࠪी"),
+  bstack11_opy_ (u"ࠪࡰࡴࡩࡡ࡭࡫ࡧࡩࡳࡺࡩࡧ࡫ࡨࡶࠬु"): bstack11_opy_ (u"ࠫࡱࡵࡣࡢ࡮ࡌࡨࡪࡴࡴࡪࡨ࡬ࡩࡷ࠭ू"),
 }
-bstack11lll1_opy_ = bstack1ll1_opy_ (u"ࠬ࡮ࡴࡵࡲࡶ࠾࠴࠵ࡨࡶࡤ࠱ࡦࡷࡵࡷࡴࡧࡵࡷࡹࡧࡣ࡬࠰ࡦࡳࡲ࠵ࡷࡥ࠱࡫ࡹࡧ࠭ृ")
-bstack1l1ll111l_opy_ = bstack1ll1_opy_ (u"࠭ࡨࡵࡶࡳ࠾࠴࠵ࡨࡶࡤ࠱ࡦࡷࡵࡷࡴࡧࡵࡷࡹࡧࡣ࡬࠰ࡦࡳࡲࡀ࠸࠱࠱ࡺࡨ࠴࡮ࡵࡣࠩॄ")
-bstack1ll1l1_opy_ = {
-  bstack1ll1_opy_ (u"ࠧࡤࡴ࡬ࡸ࡮ࡩࡡ࡭ࠩॅ"): 50,
-  bstack1ll1_opy_ (u"ࠨࡧࡵࡶࡴࡸࠧॆ"): 40,
-  bstack1ll1_opy_ (u"ࠩࡺࡥࡷࡴࡩ࡯ࡩࠪे"): 30,
-  bstack1ll1_opy_ (u"ࠪ࡭ࡳ࡬࡯ࠨै"): 20,
-  bstack1ll1_opy_ (u"ࠫࡩ࡫ࡢࡶࡩࠪॉ"): 10
+bstack1lll11111_opy_ = bstack11_opy_ (u"ࠬ࡮ࡴࡵࡲࡶ࠾࠴࠵ࡨࡶࡤ࠱ࡦࡷࡵࡷࡴࡧࡵࡷࡹࡧࡣ࡬࠰ࡦࡳࡲ࠵ࡷࡥ࠱࡫ࡹࡧ࠭ृ")
+bstack111l111_opy_ = bstack11_opy_ (u"࠭ࡨࡵࡶࡳ࠾࠴࠵ࡨࡶࡤ࠱ࡦࡷࡵࡷࡴࡧࡵࡷࡹࡧࡣ࡬࠰ࡦࡳࡲࡀ࠸࠱࠱ࡺࡨ࠴࡮ࡵࡣࠩॄ")
+bstack1ll11lll1_opy_ = bstack11_opy_ (u"ࠧࡩࡶࡷࡴࡸࡀ࠯࠰ࡪࡸࡦ࠳ࡨࡲࡰࡹࡶࡩࡷࡹࡴࡢࡥ࡮࠲ࡨࡵ࡭࠰ࡰࡨࡼࡹࡥࡨࡶࡤࡶࠫॅ")
+bstack1l1ll_opy_ = {
+  bstack11_opy_ (u"ࠨࡥࡵ࡭ࡹ࡯ࡣࡢ࡮ࠪॆ"): 50,
+  bstack11_opy_ (u"ࠩࡨࡶࡷࡵࡲࠨे"): 40,
+  bstack11_opy_ (u"ࠪࡻࡦࡸ࡮ࡪࡰࡪࠫै"): 30,
+  bstack11_opy_ (u"ࠫ࡮ࡴࡦࡰࠩॉ"): 20,
+  bstack11_opy_ (u"ࠬࡪࡥࡣࡷࡪࠫॊ"): 10
 }
-DEFAULT_LOG_LEVEL = bstack1ll1l1_opy_[bstack1ll1_opy_ (u"ࠬ࡯࡮ࡧࡱࠪॊ")]
-bstack1lllll111_opy_ = bstack1ll1_opy_ (u"࠭ࡰࡺࡶ࡫ࡳࡳ࠳ࡰࡺࡶ࡫ࡳࡳࡧࡧࡦࡰࡷ࠳ࠬो")
-bstack1l1l1l_opy_ = bstack1ll1_opy_ (u"ࠧࡳࡱࡥࡳࡹ࠳ࡰࡺࡶ࡫ࡳࡳࡧࡧࡦࡰࡷ࠳ࠬौ")
-bstack1lllll11_opy_ = bstack1ll1_opy_ (u"ࠨࡤࡨ࡬ࡦࡼࡥ࠮ࡲࡼࡸ࡭ࡵ࡮ࡢࡩࡨࡲࡹ࠵्ࠧ")
-bstack1l11l1ll1_opy_ = bstack1ll1_opy_ (u"ࠩࡳࡽࡹ࡫ࡳࡵ࠯ࡳࡽࡹ࡮࡯࡯ࡣࡪࡩࡳࡺ࠯ࠨॎ")
-bstack1ll1ll1ll_opy_ = [bstack1ll1_opy_ (u"ࠪࡆࡗࡕࡗࡔࡇࡕࡗ࡙ࡇࡃࡌࡡࡘࡗࡊࡘࡎࡂࡏࡈࠫॏ"), bstack1ll1_opy_ (u"ࠫ࡞ࡕࡕࡓࡡࡘࡗࡊࡘࡎࡂࡏࡈࠫॐ")]
-bstack111111ll_opy_ = [bstack1ll1_opy_ (u"ࠬࡈࡒࡐ࡙ࡖࡉࡗ࡙ࡔࡂࡅࡎࡣࡆࡉࡃࡆࡕࡖࡣࡐࡋ࡙ࠨ॑"), bstack1ll1_opy_ (u"࡙࠭ࡐࡗࡕࡣࡆࡉࡃࡆࡕࡖࡣࡐࡋ࡙ࠨ॒")]
-bstack1l11l1lll_opy_ = [
-  bstack1ll1_opy_ (u"ࠧࡢࡷࡷࡳࡲࡧࡴࡪࡱࡱࡒࡦࡳࡥࠨ॓"),
-  bstack1ll1_opy_ (u"ࠨࡲ࡯ࡥࡹ࡬࡯ࡳ࡯࡙ࡩࡷࡹࡩࡰࡰࠪ॔"),
-  bstack1ll1_opy_ (u"ࠩࡧࡩࡻ࡯ࡣࡦࡐࡤࡱࡪ࠭ॕ"),
-  bstack1ll1_opy_ (u"ࠪࡲࡪࡽࡃࡰ࡯ࡰࡥࡳࡪࡔࡪ࡯ࡨࡳࡺࡺࠧॖ"),
-  bstack1ll1_opy_ (u"ࠫࡦࡶࡰࠨॗ"),
-  bstack1ll1_opy_ (u"ࠬࡻࡤࡪࡦࠪक़"),
-  bstack1ll1_opy_ (u"࠭࡬ࡢࡰࡪࡹࡦ࡭ࡥࠨख़"),
-  bstack1ll1_opy_ (u"ࠧ࡭ࡱࡦࡥࡱ࡫ࠧग़"),
-  bstack1ll1_opy_ (u"ࠨࡱࡵ࡭ࡪࡴࡴࡢࡶ࡬ࡳࡳ࠭ज़"),
-  bstack1ll1_opy_ (u"ࠩࡤࡹࡹࡵࡗࡦࡤࡹ࡭ࡪࡽࠧड़"),
-  bstack1ll1_opy_ (u"ࠪࡲࡴࡘࡥࡴࡧࡷࠫढ़"), bstack1ll1_opy_ (u"ࠫ࡫ࡻ࡬࡭ࡔࡨࡷࡪࡺࠧफ़"),
-  bstack1ll1_opy_ (u"ࠬࡩ࡬ࡦࡣࡵࡗࡾࡹࡴࡦ࡯ࡉ࡭ࡱ࡫ࡳࠨय़"),
-  bstack1ll1_opy_ (u"࠭ࡥࡷࡧࡱࡸ࡙࡯࡭ࡪࡰࡪࡷࠬॠ"),
-  bstack1ll1_opy_ (u"ࠧࡦࡰࡤࡦࡱ࡫ࡐࡦࡴࡩࡳࡷࡳࡡ࡯ࡥࡨࡐࡴ࡭ࡧࡪࡰࡪࠫॡ"),
-  bstack1ll1_opy_ (u"ࠨࡱࡷ࡬ࡪࡸࡁࡱࡲࡶࠫॢ"),
-  bstack1ll1_opy_ (u"ࠩࡳࡶ࡮ࡴࡴࡑࡣࡪࡩࡘࡵࡵࡳࡥࡨࡓࡳࡌࡩ࡯ࡦࡉࡥ࡮ࡲࡵࡳࡧࠪॣ"),
-  bstack1ll1_opy_ (u"ࠪࡥࡵࡶࡁࡤࡶ࡬ࡺ࡮ࡺࡹࠨ।"), bstack1ll1_opy_ (u"ࠫࡦࡶࡰࡑࡣࡦ࡯ࡦ࡭ࡥࠨ॥"), bstack1ll1_opy_ (u"ࠬࡧࡰࡱ࡙ࡤ࡭ࡹࡇࡣࡵ࡫ࡹ࡭ࡹࡿࠧ०"), bstack1ll1_opy_ (u"࠭ࡡࡱࡲ࡚ࡥ࡮ࡺࡐࡢࡥ࡮ࡥ࡬࡫ࠧ१"), bstack1ll1_opy_ (u"ࠧࡢࡲࡳ࡛ࡦ࡯ࡴࡅࡷࡵࡥࡹ࡯࡯࡯ࠩ२"),
-  bstack1ll1_opy_ (u"ࠨࡦࡨࡺ࡮ࡩࡥࡓࡧࡤࡨࡾ࡚ࡩ࡮ࡧࡲࡹࡹ࠭३"),
-  bstack1ll1_opy_ (u"ࠩࡤࡰࡱࡵࡷࡕࡧࡶࡸࡕࡧࡣ࡬ࡣࡪࡩࡸ࠭४"),
-  bstack1ll1_opy_ (u"ࠪࡥࡳࡪࡲࡰ࡫ࡧࡇࡴࡼࡥࡳࡣࡪࡩࠬ५"), bstack1ll1_opy_ (u"ࠫࡦࡴࡤࡳࡱ࡬ࡨࡈࡵࡶࡦࡴࡤ࡫ࡪࡋ࡮ࡥࡋࡱࡸࡪࡴࡴࠨ६"),
-  bstack1ll1_opy_ (u"ࠬࡧ࡮ࡥࡴࡲ࡭ࡩࡊࡥࡷ࡫ࡦࡩࡗ࡫ࡡࡥࡻࡗ࡭ࡲ࡫࡯ࡶࡶࠪ७"),
-  bstack1ll1_opy_ (u"࠭ࡡࡥࡤࡓࡳࡷࡺࠧ८"),
-  bstack1ll1_opy_ (u"ࠧࡢࡰࡧࡶࡴ࡯ࡤࡅࡧࡹ࡭ࡨ࡫ࡓࡰࡥ࡮ࡩࡹ࠭९"),
-  bstack1ll1_opy_ (u"ࠨࡣࡱࡨࡷࡵࡩࡥࡋࡱࡷࡹࡧ࡬࡭ࡖ࡬ࡱࡪࡵࡵࡵࠩ॰"),
-  bstack1ll1_opy_ (u"ࠩࡤࡲࡩࡸ࡯ࡪࡦࡌࡲࡸࡺࡡ࡭࡮ࡓࡥࡹ࡮ࠧॱ"),
-  bstack1ll1_opy_ (u"ࠪࡥࡻࡪࠧॲ"), bstack1ll1_opy_ (u"ࠫࡦࡼࡤࡍࡣࡸࡲࡨ࡮ࡔࡪ࡯ࡨࡳࡺࡺࠧॳ"), bstack1ll1_opy_ (u"ࠬࡧࡶࡥࡔࡨࡥࡩࡿࡔࡪ࡯ࡨࡳࡺࡺࠧॴ"), bstack1ll1_opy_ (u"࠭ࡡࡷࡦࡄࡶ࡬ࡹࠧॵ"),
-  bstack1ll1_opy_ (u"ࠧࡶࡵࡨࡏࡪࡿࡳࡵࡱࡵࡩࠬॶ"), bstack1ll1_opy_ (u"ࠨ࡭ࡨࡽࡸࡺ࡯ࡳࡧࡓࡥࡹ࡮ࠧॷ"), bstack1ll1_opy_ (u"ࠩ࡮ࡩࡾࡹࡴࡰࡴࡨࡔࡦࡹࡳࡸࡱࡵࡨࠬॸ"),
-  bstack1ll1_opy_ (u"ࠪ࡯ࡪࡿࡁ࡭࡫ࡤࡷࠬॹ"), bstack1ll1_opy_ (u"ࠫࡰ࡫ࡹࡑࡣࡶࡷࡼࡵࡲࡥࠩॺ"),
-  bstack1ll1_opy_ (u"ࠬࡩࡨࡳࡱࡰࡩࡩࡸࡩࡷࡧࡵࡉࡽ࡫ࡣࡶࡶࡤࡦࡱ࡫ࠧॻ"), bstack1ll1_opy_ (u"࠭ࡣࡩࡴࡲࡱࡪࡪࡲࡪࡸࡨࡶࡆࡸࡧࡴࠩॼ"), bstack1ll1_opy_ (u"ࠧࡤࡪࡵࡳࡲ࡫ࡤࡳ࡫ࡹࡩࡷࡋࡸࡦࡥࡸࡸࡦࡨ࡬ࡦࡆ࡬ࡶࠬॽ"), bstack1ll1_opy_ (u"ࠨࡥ࡫ࡶࡴࡳࡥࡥࡴ࡬ࡺࡪࡸࡃࡩࡴࡲࡱࡪࡓࡡࡱࡲ࡬ࡲ࡬ࡌࡩ࡭ࡧࠪॾ"), bstack1ll1_opy_ (u"ࠩࡦ࡬ࡷࡵ࡭ࡦࡦࡵ࡭ࡻ࡫ࡲࡖࡵࡨࡗࡾࡹࡴࡦ࡯ࡈࡼࡪࡩࡵࡵࡣࡥࡰࡪ࠭ॿ"),
-  bstack1ll1_opy_ (u"ࠪࡧ࡭ࡸ࡯࡮ࡧࡧࡶ࡮ࡼࡥࡳࡒࡲࡶࡹ࠭ঀ"), bstack1ll1_opy_ (u"ࠫࡨ࡮ࡲࡰ࡯ࡨࡨࡷ࡯ࡶࡦࡴࡓࡳࡷࡺࡳࠨঁ"),
-  bstack1ll1_opy_ (u"ࠬࡩࡨࡳࡱࡰࡩࡩࡸࡩࡷࡧࡵࡈ࡮ࡹࡡࡣ࡮ࡨࡆࡺ࡯࡬ࡥࡅ࡫ࡩࡨࡱࠧং"),
-  bstack1ll1_opy_ (u"࠭ࡡࡶࡶࡲ࡛ࡪࡨࡶࡪࡧࡺࡘ࡮ࡳࡥࡰࡷࡷࠫঃ"),
-  bstack1ll1_opy_ (u"ࠧࡪࡰࡷࡩࡳࡺࡁࡤࡶ࡬ࡳࡳ࠭঄"), bstack1ll1_opy_ (u"ࠨ࡫ࡱࡸࡪࡴࡴࡄࡣࡷࡩ࡬ࡵࡲࡺࠩঅ"), bstack1ll1_opy_ (u"ࠩ࡬ࡲࡹ࡫࡮ࡵࡈ࡯ࡥ࡬ࡹࠧআ"), bstack1ll1_opy_ (u"ࠪࡳࡵࡺࡩࡰࡰࡤࡰࡎࡴࡴࡦࡰࡷࡅࡷ࡭ࡵ࡮ࡧࡱࡸࡸ࠭ই"),
-  bstack1ll1_opy_ (u"ࠫࡩࡵ࡮ࡵࡕࡷࡳࡵࡇࡰࡱࡑࡱࡖࡪࡹࡥࡵࠩঈ"),
-  bstack1ll1_opy_ (u"ࠬࡻ࡮ࡪࡥࡲࡨࡪࡑࡥࡺࡤࡲࡥࡷࡪࠧউ"), bstack1ll1_opy_ (u"࠭ࡲࡦࡵࡨࡸࡐ࡫ࡹࡣࡱࡤࡶࡩ࠭ঊ"),
-  bstack1ll1_opy_ (u"ࠧ࡯ࡱࡖ࡭࡬ࡴࠧঋ"),
-  bstack1ll1_opy_ (u"ࠨ࡫ࡪࡲࡴࡸࡥࡖࡰ࡬ࡱࡵࡵࡲࡵࡣࡱࡸ࡛࡯ࡥࡸࡵࠪঌ"),
-  bstack1ll1_opy_ (u"ࠩࡧ࡭ࡸࡧࡢ࡭ࡧࡄࡲࡩࡸ࡯ࡪࡦ࡚ࡥࡹࡩࡨࡦࡴࡶࠫ঍"),
-  bstack1ll1_opy_ (u"ࠪࡧ࡭ࡸ࡯࡮ࡧࡒࡴࡹ࡯࡯࡯ࡵࠪ঎"),
-  bstack1ll1_opy_ (u"ࠫࡷ࡫ࡣࡳࡧࡤࡸࡪࡉࡨࡳࡱࡰࡩࡉࡸࡩࡷࡧࡵࡗࡪࡹࡳࡪࡱࡱࡷࠬএ"),
-  bstack1ll1_opy_ (u"ࠬࡴࡡࡵ࡫ࡹࡩ࡜࡫ࡢࡔࡥࡵࡩࡪࡴࡳࡩࡱࡷࠫঐ"),
-  bstack1ll1_opy_ (u"࠭ࡡ࡯ࡦࡵࡳ࡮ࡪࡓࡤࡴࡨࡩࡳࡹࡨࡰࡶࡓࡥࡹ࡮ࠧ঑"),
-  bstack1ll1_opy_ (u"ࠧ࡯ࡧࡷࡻࡴࡸ࡫ࡔࡲࡨࡩࡩ࠭঒"),
-  bstack1ll1_opy_ (u"ࠨࡩࡳࡷࡊࡴࡡࡣ࡮ࡨࡨࠬও"),
-  bstack1ll1_opy_ (u"ࠩ࡬ࡷࡍ࡫ࡡࡥ࡮ࡨࡷࡸ࠭ঔ"),
-  bstack1ll1_opy_ (u"ࠪࡥࡩࡨࡅࡹࡧࡦࡘ࡮ࡳࡥࡰࡷࡷࠫক"),
-  bstack1ll1_opy_ (u"ࠫࡱࡵࡣࡢ࡮ࡨࡗࡨࡸࡩࡱࡶࠪখ"),
-  bstack1ll1_opy_ (u"ࠬࡹ࡫ࡪࡲࡇࡩࡻ࡯ࡣࡦࡋࡱ࡭ࡹ࡯ࡡ࡭࡫ࡽࡥࡹ࡯࡯࡯ࠩগ"),
-  bstack1ll1_opy_ (u"࠭ࡡࡶࡶࡲࡋࡷࡧ࡮ࡵࡒࡨࡶࡲ࡯ࡳࡴ࡫ࡲࡲࡸ࠭ঘ"),
-  bstack1ll1_opy_ (u"ࠧࡢࡰࡧࡶࡴ࡯ࡤࡏࡣࡷࡹࡷࡧ࡬ࡐࡴ࡬ࡩࡳࡺࡡࡵ࡫ࡲࡲࠬঙ"),
-  bstack1ll1_opy_ (u"ࠨࡵࡼࡷࡹ࡫࡭ࡑࡱࡵࡸࠬচ"),
-  bstack1ll1_opy_ (u"ࠩࡵࡩࡲࡵࡴࡦࡃࡧࡦࡍࡵࡳࡵࠩছ"),
-  bstack1ll1_opy_ (u"ࠪࡷࡰ࡯ࡰࡖࡰ࡯ࡳࡨࡱࠧজ"), bstack1ll1_opy_ (u"ࠫࡺࡴ࡬ࡰࡥ࡮ࡘࡾࡶࡥࠨঝ"), bstack1ll1_opy_ (u"ࠬࡻ࡮࡭ࡱࡦ࡯ࡐ࡫ࡹࠨঞ"),
-  bstack1ll1_opy_ (u"࠭ࡡࡶࡶࡲࡐࡦࡻ࡮ࡤࡪࠪট"),
-  bstack1ll1_opy_ (u"ࠧࡴ࡭࡬ࡴࡑࡵࡧࡤࡣࡷࡇࡦࡶࡴࡶࡴࡨࠫঠ"),
-  bstack1ll1_opy_ (u"ࠨࡷࡱ࡭ࡳࡹࡴࡢ࡮࡯ࡓࡹ࡮ࡥࡳࡒࡤࡧࡰࡧࡧࡦࡵࠪড"),
-  bstack1ll1_opy_ (u"ࠩࡧ࡭ࡸࡧࡢ࡭ࡧ࡚࡭ࡳࡪ࡯ࡸࡃࡱ࡭ࡲࡧࡴࡪࡱࡱࠫঢ"),
-  bstack1ll1_opy_ (u"ࠪࡦࡺ࡯࡬ࡥࡖࡲࡳࡱࡹࡖࡦࡴࡶ࡭ࡴࡴࠧণ"),
-  bstack1ll1_opy_ (u"ࠫࡪࡴࡦࡰࡴࡦࡩࡆࡶࡰࡊࡰࡶࡸࡦࡲ࡬ࠨত"),
-  bstack1ll1_opy_ (u"ࠬ࡫࡮ࡴࡷࡵࡩ࡜࡫ࡢࡷ࡫ࡨࡻࡸࡎࡡࡷࡧࡓࡥ࡬࡫ࡳࠨথ"), bstack1ll1_opy_ (u"࠭ࡷࡦࡤࡹ࡭ࡪࡽࡄࡦࡸࡷࡳࡴࡲࡳࡑࡱࡵࡸࠬদ"), bstack1ll1_opy_ (u"ࠧࡦࡰࡤࡦࡱ࡫ࡗࡦࡤࡹ࡭ࡪࡽࡄࡦࡶࡤ࡭ࡱࡹࡃࡰ࡮࡯ࡩࡨࡺࡩࡰࡰࠪধ"),
-  bstack1ll1_opy_ (u"ࠨࡴࡨࡱࡴࡺࡥࡂࡲࡳࡷࡈࡧࡣࡩࡧࡏ࡭ࡲ࡯ࡴࠨন"),
-  bstack1ll1_opy_ (u"ࠩࡦࡥࡱ࡫࡮ࡥࡣࡵࡊࡴࡸ࡭ࡢࡶࠪ঩"),
-  bstack1ll1_opy_ (u"ࠪࡦࡺࡴࡤ࡭ࡧࡌࡨࠬপ"),
-  bstack1ll1_opy_ (u"ࠫࡱࡧࡵ࡯ࡥ࡫ࡘ࡮ࡳࡥࡰࡷࡷࠫফ"),
-  bstack1ll1_opy_ (u"ࠬࡲ࡯ࡤࡣࡷ࡭ࡴࡴࡓࡦࡴࡹ࡭ࡨ࡫ࡳࡆࡰࡤࡦࡱ࡫ࡤࠨব"), bstack1ll1_opy_ (u"࠭࡬ࡰࡥࡤࡸ࡮ࡵ࡮ࡔࡧࡵࡺ࡮ࡩࡥࡴࡃࡸࡸ࡭ࡵࡲࡪࡼࡨࡨࠬভ"),
-  bstack1ll1_opy_ (u"ࠧࡢࡷࡷࡳࡆࡩࡣࡦࡲࡷࡅࡱ࡫ࡲࡵࡵࠪম"), bstack1ll1_opy_ (u"ࠨࡣࡸࡸࡴࡊࡩࡴ࡯࡬ࡷࡸࡇ࡬ࡦࡴࡷࡷࠬয"),
-  bstack1ll1_opy_ (u"ࠩࡱࡥࡹ࡯ࡶࡦࡋࡱࡷࡹࡸࡵ࡮ࡧࡱࡸࡸࡒࡩࡣࠩর"),
-  bstack1ll1_opy_ (u"ࠪࡲࡦࡺࡩࡷࡧ࡚ࡩࡧ࡚ࡡࡱࠩ঱"),
-  bstack1ll1_opy_ (u"ࠫࡸࡧࡦࡢࡴ࡬ࡍࡳ࡯ࡴࡪࡣ࡯࡙ࡷࡲࠧল"), bstack1ll1_opy_ (u"ࠬࡹࡡࡧࡣࡵ࡭ࡆࡲ࡬ࡰࡹࡓࡳࡵࡻࡰࡴࠩ঳"), bstack1ll1_opy_ (u"࠭ࡳࡢࡨࡤࡶ࡮ࡏࡧ࡯ࡱࡵࡩࡋࡸࡡࡶࡦ࡚ࡥࡷࡴࡩ࡯ࡩࠪ঴"), bstack1ll1_opy_ (u"ࠧࡴࡣࡩࡥࡷ࡯ࡏࡱࡧࡱࡐ࡮ࡴ࡫ࡴࡋࡱࡆࡦࡩ࡫ࡨࡴࡲࡹࡳࡪࠧ঵"),
-  bstack1ll1_opy_ (u"ࠨ࡭ࡨࡩࡵࡑࡥࡺࡅ࡫ࡥ࡮ࡴࡳࠨশ"),
-  bstack1ll1_opy_ (u"ࠩ࡯ࡳࡨࡧ࡬ࡪࡼࡤࡦࡱ࡫ࡓࡵࡴ࡬ࡲ࡬ࡹࡄࡪࡴࠪষ"),
-  bstack1ll1_opy_ (u"ࠪࡴࡷࡵࡣࡦࡵࡶࡅࡷ࡭ࡵ࡮ࡧࡱࡸࡸ࠭স"),
-  bstack1ll1_opy_ (u"ࠫ࡮ࡴࡴࡦࡴࡎࡩࡾࡊࡥ࡭ࡣࡼࠫহ"),
-  bstack1ll1_opy_ (u"ࠬࡹࡨࡰࡹࡌࡓࡘࡒ࡯ࡨࠩ঺"),
-  bstack1ll1_opy_ (u"࠭ࡳࡦࡰࡧࡏࡪࡿࡓࡵࡴࡤࡸࡪ࡭ࡹࠨ঻"),
-  bstack1ll1_opy_ (u"ࠧࡸࡧࡥ࡯࡮ࡺࡒࡦࡵࡳࡳࡳࡹࡥࡕ࡫ࡰࡩࡴࡻࡴࠨ়"), bstack1ll1_opy_ (u"ࠨࡵࡦࡶࡪ࡫࡮ࡴࡪࡲࡸ࡜ࡧࡩࡵࡖ࡬ࡱࡪࡵࡵࡵࠩঽ"),
-  bstack1ll1_opy_ (u"ࠩࡵࡩࡲࡵࡴࡦࡆࡨࡦࡺ࡭ࡐࡳࡱࡻࡽࠬা"),
-  bstack1ll1_opy_ (u"ࠪࡩࡳࡧࡢ࡭ࡧࡄࡷࡾࡴࡣࡆࡺࡨࡧࡺࡺࡥࡇࡴࡲࡱࡍࡺࡴࡱࡵࠪি"),
-  bstack1ll1_opy_ (u"ࠫࡸࡱࡩࡱࡎࡲ࡫ࡈࡧࡰࡵࡷࡵࡩࠬী"),
-  bstack1ll1_opy_ (u"ࠬࡽࡥࡣ࡭࡬ࡸࡉ࡫ࡢࡶࡩࡓࡶࡴࡾࡹࡑࡱࡵࡸࠬু"),
-  bstack1ll1_opy_ (u"࠭ࡦࡶ࡮࡯ࡇࡴࡴࡴࡦࡺࡷࡐ࡮ࡹࡴࠨূ"),
-  bstack1ll1_opy_ (u"ࠧࡸࡣ࡬ࡸࡋࡵࡲࡂࡲࡳࡗࡨࡸࡩࡱࡶࠪৃ"),
-  bstack1ll1_opy_ (u"ࠨࡹࡨࡦࡻ࡯ࡥࡸࡅࡲࡲࡳ࡫ࡣࡵࡔࡨࡸࡷ࡯ࡥࡴࠩৄ"),
-  bstack1ll1_opy_ (u"ࠩࡤࡴࡵࡔࡡ࡮ࡧࠪ৅"),
-  bstack1ll1_opy_ (u"ࠪࡧࡺࡹࡴࡰ࡯ࡖࡗࡑࡉࡥࡳࡶࠪ৆"),
-  bstack1ll1_opy_ (u"ࠫࡹࡧࡰࡘ࡫ࡷ࡬ࡘ࡮࡯ࡳࡶࡓࡶࡪࡹࡳࡅࡷࡵࡥࡹ࡯࡯࡯ࠩে"),
-  bstack1ll1_opy_ (u"ࠬࡹࡣࡢ࡮ࡨࡊࡦࡩࡴࡰࡴࠪৈ"),
-  bstack1ll1_opy_ (u"࠭ࡷࡥࡣࡏࡳࡨࡧ࡬ࡑࡱࡵࡸࠬ৉"),
-  bstack1ll1_opy_ (u"ࠧࡴࡪࡲࡻ࡝ࡩ࡯ࡥࡧࡏࡳ࡬࠭৊"),
-  bstack1ll1_opy_ (u"ࠨ࡫ࡲࡷࡎࡴࡳࡵࡣ࡯ࡰࡕࡧࡵࡴࡧࠪো"),
-  bstack1ll1_opy_ (u"ࠩࡻࡧࡴࡪࡥࡄࡱࡱࡪ࡮࡭ࡆࡪ࡮ࡨࠫৌ"),
-  bstack1ll1_opy_ (u"ࠪ࡯ࡪࡿࡣࡩࡣ࡬ࡲࡕࡧࡳࡴࡹࡲࡶࡩ্࠭"),
-  bstack1ll1_opy_ (u"ࠫࡺࡹࡥࡑࡴࡨࡦࡺ࡯࡬ࡵ࡙ࡇࡅࠬৎ"),
-  bstack1ll1_opy_ (u"ࠬࡶࡲࡦࡸࡨࡲࡹ࡝ࡄࡂࡃࡷࡸࡦࡩࡨ࡮ࡧࡱࡸࡸ࠭৏"),
-  bstack1ll1_opy_ (u"࠭ࡷࡦࡤࡇࡶ࡮ࡼࡥࡳࡃࡪࡩࡳࡺࡕࡳ࡮ࠪ৐"),
-  bstack1ll1_opy_ (u"ࠧ࡬ࡧࡼࡧ࡭ࡧࡩ࡯ࡒࡤࡸ࡭࠭৑"),
-  bstack1ll1_opy_ (u"ࠨࡷࡶࡩࡓ࡫ࡷࡘࡆࡄࠫ৒"),
-  bstack1ll1_opy_ (u"ࠩࡺࡨࡦࡒࡡࡶࡰࡦ࡬࡙࡯࡭ࡦࡱࡸࡸࠬ৓"), bstack1ll1_opy_ (u"ࠪࡻࡩࡧࡃࡰࡰࡱࡩࡨࡺࡩࡰࡰࡗ࡭ࡲ࡫࡯ࡶࡶࠪ৔"),
-  bstack1ll1_opy_ (u"ࠫࡽࡩ࡯ࡥࡧࡒࡶ࡬ࡏࡤࠨ৕"), bstack1ll1_opy_ (u"ࠬࡾࡣࡰࡦࡨࡗ࡮࡭࡮ࡪࡰࡪࡍࡩ࠭৖"),
-  bstack1ll1_opy_ (u"࠭ࡵࡱࡦࡤࡸࡪࡪࡗࡅࡃࡅࡹࡳࡪ࡬ࡦࡋࡧࠫৗ"),
-  bstack1ll1_opy_ (u"ࠧࡳࡧࡶࡩࡹࡕ࡮ࡔࡧࡶࡷ࡮ࡵ࡮ࡔࡶࡤࡶࡹࡕ࡮࡭ࡻࠪ৘"),
-  bstack1ll1_opy_ (u"ࠨࡥࡲࡱࡲࡧ࡮ࡥࡖ࡬ࡱࡪࡵࡵࡵࡵࠪ৙"),
-  bstack1ll1_opy_ (u"ࠩࡺࡨࡦ࡙ࡴࡢࡴࡷࡹࡵࡘࡥࡵࡴ࡬ࡩࡸ࠭৚"), bstack1ll1_opy_ (u"ࠪࡻࡩࡧࡓࡵࡣࡵࡸࡺࡶࡒࡦࡶࡵࡽࡎࡴࡴࡦࡴࡹࡥࡱ࠭৛"),
-  bstack1ll1_opy_ (u"ࠫࡨࡵ࡮࡯ࡧࡦࡸࡍࡧࡲࡥࡹࡤࡶࡪࡑࡥࡺࡤࡲࡥࡷࡪࠧড়"),
-  bstack1ll1_opy_ (u"ࠬࡳࡡࡹࡖࡼࡴ࡮ࡴࡧࡇࡴࡨࡵࡺ࡫࡮ࡤࡻࠪঢ়"),
-  bstack1ll1_opy_ (u"࠭ࡳࡪ࡯ࡳࡰࡪࡏࡳࡗ࡫ࡶ࡭ࡧࡲࡥࡄࡪࡨࡧࡰ࠭৞"),
-  bstack1ll1_opy_ (u"ࠧࡶࡵࡨࡇࡦࡸࡴࡩࡣࡪࡩࡘࡹ࡬ࠨয়"),
-  bstack1ll1_opy_ (u"ࠨࡵ࡫ࡳࡺࡲࡤࡖࡵࡨࡗ࡮ࡴࡧ࡭ࡧࡷࡳࡳ࡚ࡥࡴࡶࡐࡥࡳࡧࡧࡦࡴࠪৠ"),
-  bstack1ll1_opy_ (u"ࠩࡶࡸࡦࡸࡴࡊ࡙ࡇࡔࠬৡ"),
-  bstack1ll1_opy_ (u"ࠪࡥࡱࡲ࡯ࡸࡖࡲࡹࡨ࡮ࡉࡥࡇࡱࡶࡴࡲ࡬ࠨৢ"),
-  bstack1ll1_opy_ (u"ࠫ࡮࡭࡮ࡰࡴࡨࡌ࡮ࡪࡤࡦࡰࡄࡴ࡮ࡖ࡯࡭࡫ࡦࡽࡊࡸࡲࡰࡴࠪৣ"),
-  bstack1ll1_opy_ (u"ࠬࡳ࡯ࡤ࡭ࡏࡳࡨࡧࡴࡪࡱࡱࡅࡵࡶࠧ৤"),
-  bstack1ll1_opy_ (u"࠭࡬ࡰࡩࡦࡥࡹࡌ࡯ࡳ࡯ࡤࡸࠬ৥"), bstack1ll1_opy_ (u"ࠧ࡭ࡱࡪࡧࡦࡺࡆࡪ࡮ࡷࡩࡷ࡙ࡰࡦࡥࡶࠫ০"),
-  bstack1ll1_opy_ (u"ࠨࡣ࡯ࡰࡴࡽࡄࡦ࡮ࡤࡽࡆࡪࡢࠨ১")
+DEFAULT_LOG_LEVEL = bstack1l1ll_opy_[bstack11_opy_ (u"࠭ࡩ࡯ࡨࡲࠫो")]
+bstack111l1_opy_ = bstack11_opy_ (u"ࠧࡱࡻࡷ࡬ࡴࡴ࠭ࡱࡻࡷ࡬ࡴࡴࡡࡨࡧࡱࡸ࠴࠭ौ")
+bstack1l111l111_opy_ = bstack11_opy_ (u"ࠨࡴࡲࡦࡴࡺ࠭ࡱࡻࡷ࡬ࡴࡴࡡࡨࡧࡱࡸ࠴्࠭")
+bstack1llll11_opy_ = bstack11_opy_ (u"ࠩࡥࡩ࡭ࡧࡶࡦ࠯ࡳࡽࡹ࡮࡯࡯ࡣࡪࡩࡳࡺ࠯ࠨॎ")
+bstack1l1l11l_opy_ = bstack11_opy_ (u"ࠪࡴࡾࡺࡥࡴࡶ࠰ࡴࡾࡺࡨࡰࡰࡤ࡫ࡪࡴࡴ࠰ࠩॏ")
+bstack11lll_opy_ = [bstack11_opy_ (u"ࠫࡇࡘࡏࡘࡕࡈࡖࡘ࡚ࡁࡄࡍࡢ࡙ࡘࡋࡒࡏࡃࡐࡉࠬॐ"), bstack11_opy_ (u"ࠬ࡟ࡏࡖࡔࡢ࡙ࡘࡋࡒࡏࡃࡐࡉࠬ॑")]
+bstack1111l111_opy_ = [bstack11_opy_ (u"࠭ࡂࡓࡑ࡚ࡗࡊࡘࡓࡕࡃࡆࡏࡤࡇࡃࡄࡇࡖࡗࡤࡑࡅ࡚॒ࠩ"), bstack11_opy_ (u"࡚ࠧࡑࡘࡖࡤࡇࡃࡄࡇࡖࡗࡤࡑࡅ࡚ࠩ॓")]
+bstack1l1l1l_opy_ = [
+  bstack11_opy_ (u"ࠨࡣࡸࡸࡴࡳࡡࡵ࡫ࡲࡲࡓࡧ࡭ࡦࠩ॔"),
+  bstack11_opy_ (u"ࠩࡳࡰࡦࡺࡦࡰࡴࡰ࡚ࡪࡸࡳࡪࡱࡱࠫॕ"),
+  bstack11_opy_ (u"ࠪࡨࡪࡼࡩࡤࡧࡑࡥࡲ࡫ࠧॖ"),
+  bstack11_opy_ (u"ࠫࡳ࡫ࡷࡄࡱࡰࡱࡦࡴࡤࡕ࡫ࡰࡩࡴࡻࡴࠨॗ"),
+  bstack11_opy_ (u"ࠬࡧࡰࡱࠩक़"),
+  bstack11_opy_ (u"࠭ࡵࡥ࡫ࡧࠫख़"),
+  bstack11_opy_ (u"ࠧ࡭ࡣࡱ࡫ࡺࡧࡧࡦࠩग़"),
+  bstack11_opy_ (u"ࠨ࡮ࡲࡧࡦࡲࡥࠨज़"),
+  bstack11_opy_ (u"ࠩࡲࡶ࡮࡫࡮ࡵࡣࡷ࡭ࡴࡴࠧड़"),
+  bstack11_opy_ (u"ࠪࡥࡺࡺ࡯ࡘࡧࡥࡺ࡮࡫ࡷࠨढ़"),
+  bstack11_opy_ (u"ࠫࡳࡵࡒࡦࡵࡨࡸࠬफ़"), bstack11_opy_ (u"ࠬ࡬ࡵ࡭࡮ࡕࡩࡸ࡫ࡴࠨय़"),
+  bstack11_opy_ (u"࠭ࡣ࡭ࡧࡤࡶࡘࡿࡳࡵࡧࡰࡊ࡮ࡲࡥࡴࠩॠ"),
+  bstack11_opy_ (u"ࠧࡦࡸࡨࡲࡹ࡚ࡩ࡮࡫ࡱ࡫ࡸ࠭ॡ"),
+  bstack11_opy_ (u"ࠨࡧࡱࡥࡧࡲࡥࡑࡧࡵࡪࡴࡸ࡭ࡢࡰࡦࡩࡑࡵࡧࡨ࡫ࡱ࡫ࠬॢ"),
+  bstack11_opy_ (u"ࠩࡲࡸ࡭࡫ࡲࡂࡲࡳࡷࠬॣ"),
+  bstack11_opy_ (u"ࠪࡴࡷ࡯࡮ࡵࡒࡤ࡫ࡪ࡙࡯ࡶࡴࡦࡩࡔࡴࡆࡪࡰࡧࡊࡦ࡯࡬ࡶࡴࡨࠫ।"),
+  bstack11_opy_ (u"ࠫࡦࡶࡰࡂࡥࡷ࡭ࡻ࡯ࡴࡺࠩ॥"), bstack11_opy_ (u"ࠬࡧࡰࡱࡒࡤࡧࡰࡧࡧࡦࠩ०"), bstack11_opy_ (u"࠭ࡡࡱࡲ࡚ࡥ࡮ࡺࡁࡤࡶ࡬ࡺ࡮ࡺࡹࠨ१"), bstack11_opy_ (u"ࠧࡢࡲࡳ࡛ࡦ࡯ࡴࡑࡣࡦ࡯ࡦ࡭ࡥࠨ२"), bstack11_opy_ (u"ࠨࡣࡳࡴ࡜ࡧࡩࡵࡆࡸࡶࡦࡺࡩࡰࡰࠪ३"),
+  bstack11_opy_ (u"ࠩࡧࡩࡻ࡯ࡣࡦࡔࡨࡥࡩࡿࡔࡪ࡯ࡨࡳࡺࡺࠧ४"),
+  bstack11_opy_ (u"ࠪࡥࡱࡲ࡯ࡸࡖࡨࡷࡹࡖࡡࡤ࡭ࡤ࡫ࡪࡹࠧ५"),
+  bstack11_opy_ (u"ࠫࡦࡴࡤࡳࡱ࡬ࡨࡈࡵࡶࡦࡴࡤ࡫ࡪ࠭६"), bstack11_opy_ (u"ࠬࡧ࡮ࡥࡴࡲ࡭ࡩࡉ࡯ࡷࡧࡵࡥ࡬࡫ࡅ࡯ࡦࡌࡲࡹ࡫࡮ࡵࠩ७"),
+  bstack11_opy_ (u"࠭ࡡ࡯ࡦࡵࡳ࡮ࡪࡄࡦࡸ࡬ࡧࡪࡘࡥࡢࡦࡼࡘ࡮ࡳࡥࡰࡷࡷࠫ८"),
+  bstack11_opy_ (u"ࠧࡢࡦࡥࡔࡴࡸࡴࠨ९"),
+  bstack11_opy_ (u"ࠨࡣࡱࡨࡷࡵࡩࡥࡆࡨࡺ࡮ࡩࡥࡔࡱࡦ࡯ࡪࡺࠧ॰"),
+  bstack11_opy_ (u"ࠩࡤࡲࡩࡸ࡯ࡪࡦࡌࡲࡸࡺࡡ࡭࡮ࡗ࡭ࡲ࡫࡯ࡶࡶࠪॱ"),
+  bstack11_opy_ (u"ࠪࡥࡳࡪࡲࡰ࡫ࡧࡍࡳࡹࡴࡢ࡮࡯ࡔࡦࡺࡨࠨॲ"),
+  bstack11_opy_ (u"ࠫࡦࡼࡤࠨॳ"), bstack11_opy_ (u"ࠬࡧࡶࡥࡎࡤࡹࡳࡩࡨࡕ࡫ࡰࡩࡴࡻࡴࠨॴ"), bstack11_opy_ (u"࠭ࡡࡷࡦࡕࡩࡦࡪࡹࡕ࡫ࡰࡩࡴࡻࡴࠨॵ"), bstack11_opy_ (u"ࠧࡢࡸࡧࡅࡷ࡭ࡳࠨॶ"),
+  bstack11_opy_ (u"ࠨࡷࡶࡩࡐ࡫ࡹࡴࡶࡲࡶࡪ࠭ॷ"), bstack11_opy_ (u"ࠩ࡮ࡩࡾࡹࡴࡰࡴࡨࡔࡦࡺࡨࠨॸ"), bstack11_opy_ (u"ࠪ࡯ࡪࡿࡳࡵࡱࡵࡩࡕࡧࡳࡴࡹࡲࡶࡩ࠭ॹ"),
+  bstack11_opy_ (u"ࠫࡰ࡫ࡹࡂ࡮࡬ࡥࡸ࠭ॺ"), bstack11_opy_ (u"ࠬࡱࡥࡺࡒࡤࡷࡸࡽ࡯ࡳࡦࠪॻ"),
+  bstack11_opy_ (u"࠭ࡣࡩࡴࡲࡱࡪࡪࡲࡪࡸࡨࡶࡊࡾࡥࡤࡷࡷࡥࡧࡲࡥࠨॼ"), bstack11_opy_ (u"ࠧࡤࡪࡵࡳࡲ࡫ࡤࡳ࡫ࡹࡩࡷࡇࡲࡨࡵࠪॽ"), bstack11_opy_ (u"ࠨࡥ࡫ࡶࡴࡳࡥࡥࡴ࡬ࡺࡪࡸࡅࡹࡧࡦࡹࡹࡧࡢ࡭ࡧࡇ࡭ࡷ࠭ॾ"), bstack11_opy_ (u"ࠩࡦ࡬ࡷࡵ࡭ࡦࡦࡵ࡭ࡻ࡫ࡲࡄࡪࡵࡳࡲ࡫ࡍࡢࡲࡳ࡭ࡳ࡭ࡆࡪ࡮ࡨࠫॿ"), bstack11_opy_ (u"ࠪࡧ࡭ࡸ࡯࡮ࡧࡧࡶ࡮ࡼࡥࡳࡗࡶࡩࡘࡿࡳࡵࡧࡰࡉࡽ࡫ࡣࡶࡶࡤࡦࡱ࡫ࠧঀ"),
+  bstack11_opy_ (u"ࠫࡨ࡮ࡲࡰ࡯ࡨࡨࡷ࡯ࡶࡦࡴࡓࡳࡷࡺࠧঁ"), bstack11_opy_ (u"ࠬࡩࡨࡳࡱࡰࡩࡩࡸࡩࡷࡧࡵࡔࡴࡸࡴࡴࠩং"),
+  bstack11_opy_ (u"࠭ࡣࡩࡴࡲࡱࡪࡪࡲࡪࡸࡨࡶࡉ࡯ࡳࡢࡤ࡯ࡩࡇࡻࡩ࡭ࡦࡆ࡬ࡪࡩ࡫ࠨঃ"),
+  bstack11_opy_ (u"ࠧࡢࡷࡷࡳ࡜࡫ࡢࡷ࡫ࡨࡻ࡙࡯࡭ࡦࡱࡸࡸࠬ঄"),
+  bstack11_opy_ (u"ࠨ࡫ࡱࡸࡪࡴࡴࡂࡥࡷ࡭ࡴࡴࠧঅ"), bstack11_opy_ (u"ࠩ࡬ࡲࡹ࡫࡮ࡵࡅࡤࡸࡪ࡭࡯ࡳࡻࠪআ"), bstack11_opy_ (u"ࠪ࡭ࡳࡺࡥ࡯ࡶࡉࡰࡦ࡭ࡳࠨই"), bstack11_opy_ (u"ࠫࡴࡶࡴࡪࡱࡱࡥࡱࡏ࡮ࡵࡧࡱࡸࡆࡸࡧࡶ࡯ࡨࡲࡹࡹࠧঈ"),
+  bstack11_opy_ (u"ࠬࡪ࡯࡯ࡶࡖࡸࡴࡶࡁࡱࡲࡒࡲࡗ࡫ࡳࡦࡶࠪউ"),
+  bstack11_opy_ (u"࠭ࡵ࡯࡫ࡦࡳࡩ࡫ࡋࡦࡻࡥࡳࡦࡸࡤࠨঊ"), bstack11_opy_ (u"ࠧࡳࡧࡶࡩࡹࡑࡥࡺࡤࡲࡥࡷࡪࠧঋ"),
+  bstack11_opy_ (u"ࠨࡰࡲࡗ࡮࡭࡮ࠨঌ"),
+  bstack11_opy_ (u"ࠩ࡬࡫ࡳࡵࡲࡦࡗࡱ࡭ࡲࡶ࡯ࡳࡶࡤࡲࡹ࡜ࡩࡦࡹࡶࠫ঍"),
+  bstack11_opy_ (u"ࠪࡨ࡮ࡹࡡࡣ࡮ࡨࡅࡳࡪࡲࡰ࡫ࡧ࡛ࡦࡺࡣࡩࡧࡵࡷࠬ঎"),
+  bstack11_opy_ (u"ࠫࡨ࡮ࡲࡰ࡯ࡨࡓࡵࡺࡩࡰࡰࡶࠫএ"),
+  bstack11_opy_ (u"ࠬࡸࡥࡤࡴࡨࡥࡹ࡫ࡃࡩࡴࡲࡱࡪࡊࡲࡪࡸࡨࡶࡘ࡫ࡳࡴ࡫ࡲࡲࡸ࠭ঐ"),
+  bstack11_opy_ (u"࠭࡮ࡢࡶ࡬ࡺࡪ࡝ࡥࡣࡕࡦࡶࡪ࡫࡮ࡴࡪࡲࡸࠬ঑"),
+  bstack11_opy_ (u"ࠧࡢࡰࡧࡶࡴ࡯ࡤࡔࡥࡵࡩࡪࡴࡳࡩࡱࡷࡔࡦࡺࡨࠨ঒"),
+  bstack11_opy_ (u"ࠨࡰࡨࡸࡼࡵࡲ࡬ࡕࡳࡩࡪࡪࠧও"),
+  bstack11_opy_ (u"ࠩࡪࡴࡸࡋ࡮ࡢࡤ࡯ࡩࡩ࠭ঔ"),
+  bstack11_opy_ (u"ࠪ࡭ࡸࡎࡥࡢࡦ࡯ࡩࡸࡹࠧক"),
+  bstack11_opy_ (u"ࠫࡦࡪࡢࡆࡺࡨࡧ࡙࡯࡭ࡦࡱࡸࡸࠬখ"),
+  bstack11_opy_ (u"ࠬࡲ࡯ࡤࡣ࡯ࡩࡘࡩࡲࡪࡲࡷࠫগ"),
+  bstack11_opy_ (u"࠭ࡳ࡬࡫ࡳࡈࡪࡼࡩࡤࡧࡌࡲ࡮ࡺࡩࡢ࡮࡬ࡾࡦࡺࡩࡰࡰࠪঘ"),
+  bstack11_opy_ (u"ࠧࡢࡷࡷࡳࡌࡸࡡ࡯ࡶࡓࡩࡷࡳࡩࡴࡵ࡬ࡳࡳࡹࠧঙ"),
+  bstack11_opy_ (u"ࠨࡣࡱࡨࡷࡵࡩࡥࡐࡤࡸࡺࡸࡡ࡭ࡑࡵ࡭ࡪࡴࡴࡢࡶ࡬ࡳࡳ࠭চ"),
+  bstack11_opy_ (u"ࠩࡶࡽࡸࡺࡥ࡮ࡒࡲࡶࡹ࠭ছ"),
+  bstack11_opy_ (u"ࠪࡶࡪࡳ࡯ࡵࡧࡄࡨࡧࡎ࡯ࡴࡶࠪজ"),
+  bstack11_opy_ (u"ࠫࡸࡱࡩࡱࡗࡱࡰࡴࡩ࡫ࠨঝ"), bstack11_opy_ (u"ࠬࡻ࡮࡭ࡱࡦ࡯࡙ࡿࡰࡦࠩঞ"), bstack11_opy_ (u"࠭ࡵ࡯࡮ࡲࡧࡰࡑࡥࡺࠩট"),
+  bstack11_opy_ (u"ࠧࡢࡷࡷࡳࡑࡧࡵ࡯ࡥ࡫ࠫঠ"),
+  bstack11_opy_ (u"ࠨࡵ࡮࡭ࡵࡒ࡯ࡨࡥࡤࡸࡈࡧࡰࡵࡷࡵࡩࠬড"),
+  bstack11_opy_ (u"ࠩࡸࡲ࡮ࡴࡳࡵࡣ࡯ࡰࡔࡺࡨࡦࡴࡓࡥࡨࡱࡡࡨࡧࡶࠫঢ"),
+  bstack11_opy_ (u"ࠪࡨ࡮ࡹࡡࡣ࡮ࡨ࡛࡮ࡴࡤࡰࡹࡄࡲ࡮ࡳࡡࡵ࡫ࡲࡲࠬণ"),
+  bstack11_opy_ (u"ࠫࡧࡻࡩ࡭ࡦࡗࡳࡴࡲࡳࡗࡧࡵࡷ࡮ࡵ࡮ࠨত"),
+  bstack11_opy_ (u"ࠬ࡫࡮ࡧࡱࡵࡧࡪࡇࡰࡱࡋࡱࡷࡹࡧ࡬࡭ࠩথ"),
+  bstack11_opy_ (u"࠭ࡥ࡯ࡵࡸࡶࡪ࡝ࡥࡣࡸ࡬ࡩࡼࡹࡈࡢࡸࡨࡔࡦ࡭ࡥࡴࠩদ"), bstack11_opy_ (u"ࠧࡸࡧࡥࡺ࡮࡫ࡷࡅࡧࡹࡸࡴࡵ࡬ࡴࡒࡲࡶࡹ࠭ধ"), bstack11_opy_ (u"ࠨࡧࡱࡥࡧࡲࡥࡘࡧࡥࡺ࡮࡫ࡷࡅࡧࡷࡥ࡮ࡲࡳࡄࡱ࡯ࡰࡪࡩࡴࡪࡱࡱࠫন"),
+  bstack11_opy_ (u"ࠩࡵࡩࡲࡵࡴࡦࡃࡳࡴࡸࡉࡡࡤࡪࡨࡐ࡮ࡳࡩࡵࠩ঩"),
+  bstack11_opy_ (u"ࠪࡧࡦࡲࡥ࡯ࡦࡤࡶࡋࡵࡲ࡮ࡣࡷࠫপ"),
+  bstack11_opy_ (u"ࠫࡧࡻ࡮ࡥ࡮ࡨࡍࡩ࠭ফ"),
+  bstack11_opy_ (u"ࠬࡲࡡࡶࡰࡦ࡬࡙࡯࡭ࡦࡱࡸࡸࠬব"),
+  bstack11_opy_ (u"࠭࡬ࡰࡥࡤࡸ࡮ࡵ࡮ࡔࡧࡵࡺ࡮ࡩࡥࡴࡇࡱࡥࡧࡲࡥࡥࠩভ"), bstack11_opy_ (u"ࠧ࡭ࡱࡦࡥࡹ࡯࡯࡯ࡕࡨࡶࡻ࡯ࡣࡦࡵࡄࡹࡹ࡮࡯ࡳ࡫ࡽࡩࡩ࠭ম"),
+  bstack11_opy_ (u"ࠨࡣࡸࡸࡴࡇࡣࡤࡧࡳࡸࡆࡲࡥࡳࡶࡶࠫয"), bstack11_opy_ (u"ࠩࡤࡹࡹࡵࡄࡪࡵࡰ࡭ࡸࡹࡁ࡭ࡧࡵࡸࡸ࠭র"),
+  bstack11_opy_ (u"ࠪࡲࡦࡺࡩࡷࡧࡌࡲࡸࡺࡲࡶ࡯ࡨࡲࡹࡹࡌࡪࡤࠪ঱"),
+  bstack11_opy_ (u"ࠫࡳࡧࡴࡪࡸࡨ࡛ࡪࡨࡔࡢࡲࠪল"),
+  bstack11_opy_ (u"ࠬࡹࡡࡧࡣࡵ࡭ࡎࡴࡩࡵ࡫ࡤࡰ࡚ࡸ࡬ࠨ঳"), bstack11_opy_ (u"࠭ࡳࡢࡨࡤࡶ࡮ࡇ࡬࡭ࡱࡺࡔࡴࡶࡵࡱࡵࠪ঴"), bstack11_opy_ (u"ࠧࡴࡣࡩࡥࡷ࡯ࡉࡨࡰࡲࡶࡪࡌࡲࡢࡷࡧ࡛ࡦࡸ࡮ࡪࡰࡪࠫ঵"), bstack11_opy_ (u"ࠨࡵࡤࡪࡦࡸࡩࡐࡲࡨࡲࡑ࡯࡮࡬ࡵࡌࡲࡇࡧࡣ࡬ࡩࡵࡳࡺࡴࡤࠨশ"),
+  bstack11_opy_ (u"ࠩ࡮ࡩࡪࡶࡋࡦࡻࡆ࡬ࡦ࡯࡮ࡴࠩষ"),
+  bstack11_opy_ (u"ࠪࡰࡴࡩࡡ࡭࡫ࡽࡥࡧࡲࡥࡔࡶࡵ࡭ࡳ࡭ࡳࡅ࡫ࡵࠫস"),
+  bstack11_opy_ (u"ࠫࡵࡸ࡯ࡤࡧࡶࡷࡆࡸࡧࡶ࡯ࡨࡲࡹࡹࠧহ"),
+  bstack11_opy_ (u"ࠬ࡯࡮ࡵࡧࡵࡏࡪࡿࡄࡦ࡮ࡤࡽࠬ঺"),
+  bstack11_opy_ (u"࠭ࡳࡩࡱࡺࡍࡔ࡙ࡌࡰࡩࠪ঻"),
+  bstack11_opy_ (u"ࠧࡴࡧࡱࡨࡐ࡫ࡹࡔࡶࡵࡥࡹ࡫ࡧࡺ়ࠩ"),
+  bstack11_opy_ (u"ࠨࡹࡨࡦࡰ࡯ࡴࡓࡧࡶࡴࡴࡴࡳࡦࡖ࡬ࡱࡪࡵࡵࡵࠩঽ"), bstack11_opy_ (u"ࠩࡶࡧࡷ࡫ࡥ࡯ࡵ࡫ࡳࡹ࡝ࡡࡪࡶࡗ࡭ࡲ࡫࡯ࡶࡶࠪা"),
+  bstack11_opy_ (u"ࠪࡶࡪࡳ࡯ࡵࡧࡇࡩࡧࡻࡧࡑࡴࡲࡼࡾ࠭ি"),
+  bstack11_opy_ (u"ࠫࡪࡴࡡࡣ࡮ࡨࡅࡸࡿ࡮ࡤࡇࡻࡩࡨࡻࡴࡦࡈࡵࡳࡲࡎࡴࡵࡲࡶࠫী"),
+  bstack11_opy_ (u"ࠬࡹ࡫ࡪࡲࡏࡳ࡬ࡉࡡࡱࡶࡸࡶࡪ࠭ু"),
+  bstack11_opy_ (u"࠭ࡷࡦࡤ࡮࡭ࡹࡊࡥࡣࡷࡪࡔࡷࡵࡸࡺࡒࡲࡶࡹ࠭ূ"),
+  bstack11_opy_ (u"ࠧࡧࡷ࡯ࡰࡈࡵ࡮ࡵࡧࡻࡸࡑ࡯ࡳࡵࠩৃ"),
+  bstack11_opy_ (u"ࠨࡹࡤ࡭ࡹࡌ࡯ࡳࡃࡳࡴࡘࡩࡲࡪࡲࡷࠫৄ"),
+  bstack11_opy_ (u"ࠩࡺࡩࡧࡼࡩࡦࡹࡆࡳࡳࡴࡥࡤࡶࡕࡩࡹࡸࡩࡦࡵࠪ৅"),
+  bstack11_opy_ (u"ࠪࡥࡵࡶࡎࡢ࡯ࡨࠫ৆"),
+  bstack11_opy_ (u"ࠫࡨࡻࡳࡵࡱࡰࡗࡘࡒࡃࡦࡴࡷࠫে"),
+  bstack11_opy_ (u"ࠬࡺࡡࡱ࡙࡬ࡸ࡭࡙ࡨࡰࡴࡷࡔࡷ࡫ࡳࡴࡆࡸࡶࡦࡺࡩࡰࡰࠪৈ"),
+  bstack11_opy_ (u"࠭ࡳࡤࡣ࡯ࡩࡋࡧࡣࡵࡱࡵࠫ৉"),
+  bstack11_opy_ (u"ࠧࡸࡦࡤࡐࡴࡩࡡ࡭ࡒࡲࡶࡹ࠭৊"),
+  bstack11_opy_ (u"ࠨࡵ࡫ࡳࡼ࡞ࡣࡰࡦࡨࡐࡴ࡭ࠧো"),
+  bstack11_opy_ (u"ࠩ࡬ࡳࡸࡏ࡮ࡴࡶࡤࡰࡱࡖࡡࡶࡵࡨࠫৌ"),
+  bstack11_opy_ (u"ࠪࡼࡨࡵࡤࡦࡅࡲࡲ࡫࡯ࡧࡇ࡫࡯ࡩ্ࠬ"),
+  bstack11_opy_ (u"ࠫࡰ࡫ࡹࡤࡪࡤ࡭ࡳࡖࡡࡴࡵࡺࡳࡷࡪࠧৎ"),
+  bstack11_opy_ (u"ࠬࡻࡳࡦࡒࡵࡩࡧࡻࡩ࡭ࡶ࡚ࡈࡆ࠭৏"),
+  bstack11_opy_ (u"࠭ࡰࡳࡧࡹࡩࡳࡺࡗࡅࡃࡄࡸࡹࡧࡣࡩ࡯ࡨࡲࡹࡹࠧ৐"),
+  bstack11_opy_ (u"ࠧࡸࡧࡥࡈࡷ࡯ࡶࡦࡴࡄ࡫ࡪࡴࡴࡖࡴ࡯ࠫ৑"),
+  bstack11_opy_ (u"ࠨ࡭ࡨࡽࡨ࡮ࡡࡪࡰࡓࡥࡹ࡮ࠧ৒"),
+  bstack11_opy_ (u"ࠩࡸࡷࡪࡔࡥࡸ࡙ࡇࡅࠬ৓"),
+  bstack11_opy_ (u"ࠪࡻࡩࡧࡌࡢࡷࡱࡧ࡭࡚ࡩ࡮ࡧࡲࡹࡹ࠭৔"), bstack11_opy_ (u"ࠫࡼࡪࡡࡄࡱࡱࡲࡪࡩࡴࡪࡱࡱࡘ࡮ࡳࡥࡰࡷࡷࠫ৕"),
+  bstack11_opy_ (u"ࠬࡾࡣࡰࡦࡨࡓࡷ࡭ࡉࡥࠩ৖"), bstack11_opy_ (u"࠭ࡸࡤࡱࡧࡩࡘ࡯ࡧ࡯࡫ࡱ࡫ࡎࡪࠧৗ"),
+  bstack11_opy_ (u"ࠧࡶࡲࡧࡥࡹ࡫ࡤࡘࡆࡄࡆࡺࡴࡤ࡭ࡧࡌࡨࠬ৘"),
+  bstack11_opy_ (u"ࠨࡴࡨࡷࡪࡺࡏ࡯ࡕࡨࡷࡸ࡯࡯࡯ࡕࡷࡥࡷࡺࡏ࡯࡮ࡼࠫ৙"),
+  bstack11_opy_ (u"ࠩࡦࡳࡲࡳࡡ࡯ࡦࡗ࡭ࡲ࡫࡯ࡶࡶࡶࠫ৚"),
+  bstack11_opy_ (u"ࠪࡻࡩࡧࡓࡵࡣࡵࡸࡺࡶࡒࡦࡶࡵ࡭ࡪࡹࠧ৛"), bstack11_opy_ (u"ࠫࡼࡪࡡࡔࡶࡤࡶࡹࡻࡰࡓࡧࡷࡶࡾࡏ࡮ࡵࡧࡵࡺࡦࡲࠧড়"),
+  bstack11_opy_ (u"ࠬࡩ࡯࡯ࡰࡨࡧࡹࡎࡡࡳࡦࡺࡥࡷ࡫ࡋࡦࡻࡥࡳࡦࡸࡤࠨঢ়"),
+  bstack11_opy_ (u"࠭࡭ࡢࡺࡗࡽࡵ࡯࡮ࡨࡈࡵࡩࡶࡻࡥ࡯ࡥࡼࠫ৞"),
+  bstack11_opy_ (u"ࠧࡴ࡫ࡰࡴࡱ࡫ࡉࡴࡘ࡬ࡷ࡮ࡨ࡬ࡦࡅ࡫ࡩࡨࡱࠧয়"),
+  bstack11_opy_ (u"ࠨࡷࡶࡩࡈࡧࡲࡵࡪࡤ࡫ࡪ࡙ࡳ࡭ࠩৠ"),
+  bstack11_opy_ (u"ࠩࡶ࡬ࡴࡻ࡬ࡥࡗࡶࡩࡘ࡯࡮ࡨ࡮ࡨࡸࡴࡴࡔࡦࡵࡷࡑࡦࡴࡡࡨࡧࡵࠫৡ"),
+  bstack11_opy_ (u"ࠪࡷࡹࡧࡲࡵࡋ࡚ࡈࡕ࠭ৢ"),
+  bstack11_opy_ (u"ࠫࡦࡲ࡬ࡰࡹࡗࡳࡺࡩࡨࡊࡦࡈࡲࡷࡵ࡬࡭ࠩৣ"),
+  bstack11_opy_ (u"ࠬ࡯ࡧ࡯ࡱࡵࡩࡍ࡯ࡤࡥࡧࡱࡅࡵ࡯ࡐࡰ࡮࡬ࡧࡾࡋࡲࡳࡱࡵࠫ৤"),
+  bstack11_opy_ (u"࠭࡭ࡰࡥ࡮ࡐࡴࡩࡡࡵ࡫ࡲࡲࡆࡶࡰࠨ৥"),
+  bstack11_opy_ (u"ࠧ࡭ࡱࡪࡧࡦࡺࡆࡰࡴࡰࡥࡹ࠭০"), bstack11_opy_ (u"ࠨ࡮ࡲ࡫ࡨࡧࡴࡇ࡫࡯ࡸࡪࡸࡓࡱࡧࡦࡷࠬ১"),
+  bstack11_opy_ (u"ࠩࡤࡰࡱࡵࡷࡅࡧ࡯ࡥࡾࡇࡤࡣࠩ২")
 ]
-bstack1l1llll1_opy_ = bstack1ll1_opy_ (u"ࠩ࡫ࡸࡹࡶࡳ࠻࠱࠲ࡥࡵ࡯࠭ࡤ࡮ࡲࡹࡩ࠴ࡢࡳࡱࡺࡷࡪࡸࡳࡵࡣࡦ࡯࠳ࡩ࡯࡮࠱ࡤࡴࡵ࠳ࡡࡶࡶࡲࡱࡦࡺࡥ࠰ࡷࡳࡰࡴࡧࡤࠨ২")
-bstack1l1l1l1_opy_ = [bstack1ll1_opy_ (u"ࠪ࠲ࡦࡶ࡫ࠨ৩"), bstack1ll1_opy_ (u"ࠫ࠳ࡧࡡࡣࠩ৪"), bstack1ll1_opy_ (u"ࠬ࠴ࡩࡱࡣࠪ৫")]
-bstack1l11l1l1l_opy_ = [bstack1ll1_opy_ (u"࠭ࡩࡥࠩ৬"), bstack1ll1_opy_ (u"ࠧࡱࡣࡷ࡬ࠬ৭"), bstack1ll1_opy_ (u"ࠨࡥࡸࡷࡹࡵ࡭ࡠ࡫ࡧࠫ৮"), bstack1ll1_opy_ (u"ࠩࡶ࡬ࡦࡸࡥࡢࡤ࡯ࡩࡤ࡯ࡤࠨ৯")]
-bstack11l1ll11_opy_ = {
-  bstack1ll1_opy_ (u"ࠪࡧ࡭ࡸ࡯࡮ࡧࡒࡴࡹ࡯࡯࡯ࡵࠪৰ"): bstack1ll1_opy_ (u"ࠫ࡬ࡵ࡯ࡨ࠼ࡦ࡬ࡷࡵ࡭ࡦࡑࡳࡸ࡮ࡵ࡮ࡴࠩৱ"),
-  bstack1ll1_opy_ (u"ࠬ࡬ࡩࡳࡧࡩࡳࡽࡕࡰࡵ࡫ࡲࡲࡸ࠭৲"): bstack1ll1_opy_ (u"࠭࡭ࡰࡼ࠽ࡪ࡮ࡸࡥࡧࡱࡻࡓࡵࡺࡩࡰࡰࡶࠫ৳"),
-  bstack1ll1_opy_ (u"ࠧࡦࡦࡪࡩࡔࡶࡴࡪࡱࡱࡷࠬ৴"): bstack1ll1_opy_ (u"ࠨ࡯ࡶ࠾ࡪࡪࡧࡦࡑࡳࡸ࡮ࡵ࡮ࡴࠩ৵"),
-  bstack1ll1_opy_ (u"ࠩ࡬ࡩࡔࡶࡴࡪࡱࡱࡷࠬ৶"): bstack1ll1_opy_ (u"ࠪࡷࡪࡀࡩࡦࡑࡳࡸ࡮ࡵ࡮ࡴࠩ৷"),
-  bstack1ll1_opy_ (u"ࠫࡸࡧࡦࡢࡴ࡬ࡓࡵࡺࡩࡰࡰࡶࠫ৸"): bstack1ll1_opy_ (u"ࠬࡹࡡࡧࡣࡵ࡭࠳ࡵࡰࡵ࡫ࡲࡲࡸ࠭৹")
+bstack1l111lll_opy_ = bstack11_opy_ (u"ࠪ࡬ࡹࡺࡰࡴ࠼࠲࠳ࡦࡶࡩ࠮ࡥ࡯ࡳࡺࡪ࠮ࡣࡴࡲࡻࡸ࡫ࡲࡴࡶࡤࡧࡰ࠴ࡣࡰ࡯࠲ࡥࡵࡶ࠭ࡢࡷࡷࡳࡲࡧࡴࡦ࠱ࡸࡴࡱࡵࡡࡥࠩ৩")
+bstack1lll1l_opy_ = [bstack11_opy_ (u"ࠫ࠳ࡧࡰ࡬ࠩ৪"), bstack11_opy_ (u"ࠬ࠴ࡡࡢࡤࠪ৫"), bstack11_opy_ (u"࠭࠮ࡪࡲࡤࠫ৬")]
+bstack1l1l1l1l_opy_ = [bstack11_opy_ (u"ࠧࡪࡦࠪ৭"), bstack11_opy_ (u"ࠨࡲࡤࡸ࡭࠭৮"), bstack11_opy_ (u"ࠩࡦࡹࡸࡺ࡯࡮ࡡ࡬ࡨࠬ৯"), bstack11_opy_ (u"ࠪࡷ࡭ࡧࡲࡦࡣࡥࡰࡪࡥࡩࡥࠩৰ")]
+bstack1ll111l1_opy_ = {
+  bstack11_opy_ (u"ࠫࡨ࡮ࡲࡰ࡯ࡨࡓࡵࡺࡩࡰࡰࡶࠫৱ"): bstack11_opy_ (u"ࠬ࡭࡯ࡰࡩ࠽ࡧ࡭ࡸ࡯࡮ࡧࡒࡴࡹ࡯࡯࡯ࡵࠪ৲"),
+  bstack11_opy_ (u"࠭ࡦࡪࡴࡨࡪࡴࡾࡏࡱࡶ࡬ࡳࡳࡹࠧ৳"): bstack11_opy_ (u"ࠧ࡮ࡱࡽ࠾࡫࡯ࡲࡦࡨࡲࡼࡔࡶࡴࡪࡱࡱࡷࠬ৴"),
+  bstack11_opy_ (u"ࠨࡧࡧ࡫ࡪࡕࡰࡵ࡫ࡲࡲࡸ࠭৵"): bstack11_opy_ (u"ࠩࡰࡷ࠿࡫ࡤࡨࡧࡒࡴࡹ࡯࡯࡯ࡵࠪ৶"),
+  bstack11_opy_ (u"ࠪ࡭ࡪࡕࡰࡵ࡫ࡲࡲࡸ࠭৷"): bstack11_opy_ (u"ࠫࡸ࡫࠺ࡪࡧࡒࡴࡹ࡯࡯࡯ࡵࠪ৸"),
+  bstack11_opy_ (u"ࠬࡹࡡࡧࡣࡵ࡭ࡔࡶࡴࡪࡱࡱࡷࠬ৹"): bstack11_opy_ (u"࠭ࡳࡢࡨࡤࡶ࡮࠴࡯ࡱࡶ࡬ࡳࡳࡹࠧ৺")
 }
-bstack11111l11_opy_ = [
-  bstack1ll1_opy_ (u"࠭ࡧࡰࡱࡪ࠾ࡨ࡮ࡲࡰ࡯ࡨࡓࡵࡺࡩࡰࡰࡶࠫ৺"),
-  bstack1ll1_opy_ (u"ࠧ࡮ࡱࡽ࠾࡫࡯ࡲࡦࡨࡲࡼࡔࡶࡴࡪࡱࡱࡷࠬ৻"),
-  bstack1ll1_opy_ (u"ࠨ࡯ࡶ࠾ࡪࡪࡧࡦࡑࡳࡸ࡮ࡵ࡮ࡴࠩৼ"),
-  bstack1ll1_opy_ (u"ࠩࡶࡩ࠿࡯ࡥࡐࡲࡷ࡭ࡴࡴࡳࠨ৽"),
-  bstack1ll1_opy_ (u"ࠪࡷࡦ࡬ࡡࡳ࡫࠱ࡳࡵࡺࡩࡰࡰࡶࠫ৾"),
+bstack1l111l11_opy_ = [
+  bstack11_opy_ (u"ࠧࡨࡱࡲ࡫࠿ࡩࡨࡳࡱࡰࡩࡔࡶࡴࡪࡱࡱࡷࠬ৻"),
+  bstack11_opy_ (u"ࠨ࡯ࡲࡾ࠿࡬ࡩࡳࡧࡩࡳࡽࡕࡰࡵ࡫ࡲࡲࡸ࠭ৼ"),
+  bstack11_opy_ (u"ࠩࡰࡷ࠿࡫ࡤࡨࡧࡒࡴࡹ࡯࡯࡯ࡵࠪ৽"),
+  bstack11_opy_ (u"ࠪࡷࡪࡀࡩࡦࡑࡳࡸ࡮ࡵ࡮ࡴࠩ৾"),
+  bstack11_opy_ (u"ࠫࡸࡧࡦࡢࡴ࡬࠲ࡴࡶࡴࡪࡱࡱࡷࠬ৿"),
 ]
-bstack11111l1l_opy_ = bstack1llll_opy_ + bstack1lll1l1l_opy_ + bstack1l11l1lll_opy_
-bstack1lll111ll_opy_ = [
-  bstack1ll1_opy_ (u"ࠫࡣࡲ࡯ࡤࡣ࡯࡬ࡴࡹࡴࠥࠩ৿"),
-  bstack1ll1_opy_ (u"ࠬࡤࡢࡴ࠯࡯ࡳࡨࡧ࡬࠯ࡥࡲࡱࠩ࠭਀"),
-  bstack1ll1_opy_ (u"࠭࡞࠲࠴࠺࠲ࠬਁ"),
-  bstack1ll1_opy_ (u"ࠧ࡟࠳࠳࠲ࠬਂ"),
-  bstack1ll1_opy_ (u"ࠨࡠ࠴࠻࠷࠴࠱࡜࠸࠰࠽ࡢ࠴ࠧਃ"),
-  bstack1ll1_opy_ (u"ࠩࡡ࠵࠼࠸࠮࠳࡝࠳࠱࠾ࡣ࠮ࠨ਄"),
-  bstack1ll1_opy_ (u"ࠪࡢ࠶࠽࠲࠯࠵࡞࠴࠲࠷࡝࠯ࠩਅ"),
-  bstack1ll1_opy_ (u"ࠫࡣ࠷࠹࠳࠰࠴࠺࠽࠴ࠧਆ")
+bstack11l11lll_opy_ = bstack1l111l1_opy_ + bstack111l1l11_opy_ + bstack1l1l1l_opy_
+bstack1l1l11ll_opy_ = [
+  bstack11_opy_ (u"ࠬࡤ࡬ࡰࡥࡤࡰ࡭ࡵࡳࡵࠦࠪ਀"),
+  bstack11_opy_ (u"࠭࡞ࡣࡵ࠰ࡰࡴࡩࡡ࡭࠰ࡦࡳࡲࠪࠧਁ"),
+  bstack11_opy_ (u"ࠧ࡟࠳࠵࠻࠳࠭ਂ"),
+  bstack11_opy_ (u"ࠨࡠ࠴࠴࠳࠭ਃ"),
+  bstack11_opy_ (u"ࠩࡡ࠵࠼࠸࠮࠲࡝࠹࠱࠾ࡣ࠮ࠨ਄"),
+  bstack11_opy_ (u"ࠪࡢ࠶࠽࠲࠯࠴࡞࠴࠲࠿࡝࠯ࠩਅ"),
+  bstack11_opy_ (u"ࠫࡣ࠷࠷࠳࠰࠶࡟࠵࠳࠱࡞࠰ࠪਆ"),
+  bstack11_opy_ (u"ࠬࡤ࠱࠺࠴࠱࠵࠻࠾࠮ࠨਇ")
 ]
-bstack1l1l11_opy_ = bstack1ll1_opy_ (u"ࠬ࡮ࡴࡵࡲࡶ࠾࠴࠵ࡡࡱ࡫࠱ࡦࡷࡵࡷࡴࡧࡵࡷࡹࡧࡣ࡬࠰ࡦࡳࡲ࠵ࡻࡾࠩਇ")
-bstack1llll11l_opy_ = bstack1ll1_opy_ (u"࠭ࡳࡥ࡭࠲ࡺ࠶࠵ࡥࡷࡧࡱࡸࠬਈ")
-bstack1lllllll_opy_ = [ bstack1ll1_opy_ (u"ࠧࡢࡷࡷࡳࡲࡧࡴࡦࠩਉ") ]
-bstack1l1l1l111_opy_ = [ bstack1ll1_opy_ (u"ࠨࡣࡳࡴ࠲ࡧࡵࡵࡱࡰࡥࡹ࡫ࠧਊ") ]
-bstack11ll111l_opy_ = [ bstack1ll1_opy_ (u"ࠩࡲࡦࡸ࡫ࡲࡷࡣࡥ࡭ࡱ࡯ࡴࡺࠩ਋") ]
-bstack1l11l1l1_opy_ = bstack1ll1_opy_ (u"ࠪࡗࡉࡑࡓࡦࡶࡸࡴࠬ਌")
-bstack1l1llll1l_opy_ = bstack1ll1_opy_ (u"ࠫࡘࡊࡋࡕࡧࡶࡸࡆࡺࡴࡦ࡯ࡳࡸࡪࡪࠧ਍")
-bstack1lll1l111_opy_ = bstack1ll1_opy_ (u"࡙ࠬࡄࡌࡖࡨࡷࡹ࡙ࡵࡤࡥࡨࡷࡸ࡬ࡵ࡭ࠩ਎")
-bstack1lllll1l_opy_ = bstack1ll1_opy_ (u"࠭࠴࠯࠲࠱࠴ࠬਏ")
-bstack1l1l1llll_opy_ = [
-  bstack1ll1_opy_ (u"ࠧࡆࡔࡕࡣࡋࡇࡉࡍࡇࡇࠫਐ"),
-  bstack1ll1_opy_ (u"ࠨࡇࡕࡖࡤ࡚ࡉࡎࡇࡇࡣࡔ࡛ࡔࠨ਑"),
-  bstack1ll1_opy_ (u"ࠩࡈࡖࡗࡥࡂࡍࡑࡆࡏࡊࡊ࡟ࡃ࡛ࡢࡇࡑࡏࡅࡏࡖࠪ਒"),
-  bstack1ll1_opy_ (u"ࠪࡉࡗࡘ࡟ࡏࡇࡗ࡛ࡔࡘࡋࡠࡅࡋࡅࡓࡍࡅࡅࠩਓ"),
-  bstack1ll1_opy_ (u"ࠫࡊࡘࡒࡠࡕࡒࡇࡐࡋࡔࡠࡐࡒࡘࡤࡉࡏࡏࡐࡈࡇ࡙ࡋࡄࠨਔ"),
-  bstack1ll1_opy_ (u"ࠬࡋࡒࡓࡡࡆࡓࡓࡔࡅࡄࡖࡌࡓࡓࡥࡃࡍࡑࡖࡉࡉ࠭ਕ"),
-  bstack1ll1_opy_ (u"࠭ࡅࡓࡔࡢࡇࡔࡔࡎࡆࡅࡗࡍࡔࡔ࡟ࡓࡇࡖࡉ࡙࠭ਖ"),
-  bstack1ll1_opy_ (u"ࠧࡆࡔࡕࡣࡈࡕࡎࡏࡇࡆࡘࡎࡕࡎࡠࡔࡈࡊ࡚࡙ࡅࡅࠩਗ"),
-  bstack1ll1_opy_ (u"ࠨࡇࡕࡖࡤࡉࡏࡏࡐࡈࡇ࡙ࡏࡏࡏࡡࡄࡆࡔࡘࡔࡆࡆࠪਘ"),
-  bstack1ll1_opy_ (u"ࠩࡈࡖࡗࡥࡃࡐࡐࡑࡉࡈ࡚ࡉࡐࡐࡢࡊࡆࡏࡌࡆࡆࠪਙ"),
-  bstack1ll1_opy_ (u"ࠪࡉࡗࡘ࡟ࡏࡃࡐࡉࡤࡔࡏࡕࡡࡕࡉࡘࡕࡌࡗࡇࡇࠫਚ"),
-  bstack1ll1_opy_ (u"ࠫࡊࡘࡒࡠࡃࡇࡈࡗࡋࡓࡔࡡࡌࡒ࡛ࡇࡌࡊࡆࠪਛ"),
-  bstack1ll1_opy_ (u"ࠬࡋࡒࡓࡡࡄࡈࡉࡘࡅࡔࡕࡢ࡙ࡓࡘࡅࡂࡅࡋࡅࡇࡒࡅࠨਜ"),
-  bstack1ll1_opy_ (u"࠭ࡅࡓࡔࡢࡘ࡚ࡔࡎࡆࡎࡢࡇࡔࡔࡎࡆࡅࡗࡍࡔࡔ࡟ࡇࡃࡌࡐࡊࡊࠧਝ"),
-  bstack1ll1_opy_ (u"ࠧࡆࡔࡕࡣࡈࡕࡎࡏࡇࡆࡘࡎࡕࡎࡠࡖࡌࡑࡊࡊ࡟ࡐࡗࡗࠫਞ"),
-  bstack1ll1_opy_ (u"ࠨࡇࡕࡖࡤ࡙ࡏࡄࡍࡖࡣࡈࡕࡎࡏࡇࡆࡘࡎࡕࡎࡠࡈࡄࡍࡑࡋࡄࠨਟ"),
-  bstack1ll1_opy_ (u"ࠩࡈࡖࡗࡥࡓࡐࡅࡎࡗࡤࡉࡏࡏࡐࡈࡇ࡙ࡏࡏࡏࡡࡋࡓࡘ࡚࡟ࡖࡐࡕࡉࡆࡉࡈࡂࡄࡏࡉࠬਠ"),
-  bstack1ll1_opy_ (u"ࠪࡉࡗࡘ࡟ࡑࡔࡒ࡜࡞ࡥࡃࡐࡐࡑࡉࡈ࡚ࡉࡐࡐࡢࡊࡆࡏࡌࡆࡆࠪਡ"),
-  bstack1ll1_opy_ (u"ࠫࡊࡘࡒࡠࡐࡄࡑࡊࡥࡎࡐࡖࡢࡖࡊ࡙ࡏࡍࡘࡈࡈࠬਢ"),
-  bstack1ll1_opy_ (u"ࠬࡋࡒࡓࡡࡑࡅࡒࡋ࡟ࡓࡇࡖࡓࡑ࡛ࡔࡊࡑࡑࡣࡋࡇࡉࡍࡇࡇࠫਣ"),
-  bstack1ll1_opy_ (u"࠭ࡅࡓࡔࡢࡑࡆࡔࡄࡂࡖࡒࡖ࡞ࡥࡐࡓࡑ࡛࡝ࡤࡉࡏࡏࡈࡌࡋ࡚ࡘࡁࡕࡋࡒࡒࡤࡌࡁࡊࡎࡈࡈࠬਤ"),
+bstack1l1l111_opy_ = bstack11_opy_ (u"࠭ࡨࡵࡶࡳࡷ࠿࠵࠯ࡢࡲ࡬࠲ࡧࡸ࡯ࡸࡵࡨࡶࡸࡺࡡࡤ࡭࠱ࡧࡴࡳ࠯ࡼࡿࠪਈ")
+bstack1l11ll111_opy_ = bstack11_opy_ (u"ࠧࡴࡦ࡮࠳ࡻ࠷࠯ࡦࡸࡨࡲࡹ࠭ਉ")
+bstack1l111111_opy_ = [ bstack11_opy_ (u"ࠨࡣࡸࡸࡴࡳࡡࡵࡧࠪਊ") ]
+bstack1llll1lll_opy_ = [ bstack11_opy_ (u"ࠩࡤࡴࡵ࠳ࡡࡶࡶࡲࡱࡦࡺࡥࠨ਋") ]
+bstack11ll11l_opy_ = [ bstack11_opy_ (u"ࠪࡳࡧࡹࡥࡳࡸࡤࡦ࡮ࡲࡩࡵࡻࠪ਌") ]
+bstack1llll_opy_ = bstack11_opy_ (u"ࠫࡘࡊࡋࡔࡧࡷࡹࡵ࠭਍")
+bstack1l1ll1ll1_opy_ = bstack11_opy_ (u"࡙ࠬࡄࡌࡖࡨࡷࡹࡇࡴࡵࡧࡰࡴࡹ࡫ࡤࠨ਎")
+bstack1llll111_opy_ = bstack11_opy_ (u"࠭ࡓࡅࡍࡗࡩࡸࡺࡓࡶࡥࡦࡩࡸࡹࡦࡶ࡮ࠪਏ")
+bstack1l1ll111_opy_ = bstack11_opy_ (u"ࠧ࠵࠰࠳࠲࠵࠭ਐ")
+bstack1l1lll11l_opy_ = [
+  bstack11_opy_ (u"ࠨࡇࡕࡖࡤࡌࡁࡊࡎࡈࡈࠬ਑"),
+  bstack11_opy_ (u"ࠩࡈࡖࡗࡥࡔࡊࡏࡈࡈࡤࡕࡕࡕࠩ਒"),
+  bstack11_opy_ (u"ࠪࡉࡗࡘ࡟ࡃࡎࡒࡇࡐࡋࡄࡠࡄ࡜ࡣࡈࡒࡉࡆࡐࡗࠫਓ"),
+  bstack11_opy_ (u"ࠫࡊࡘࡒࡠࡐࡈࡘ࡜ࡕࡒࡌࡡࡆࡌࡆࡔࡇࡆࡆࠪਔ"),
+  bstack11_opy_ (u"ࠬࡋࡒࡓࡡࡖࡓࡈࡑࡅࡕࡡࡑࡓ࡙ࡥࡃࡐࡐࡑࡉࡈ࡚ࡅࡅࠩਕ"),
+  bstack11_opy_ (u"࠭ࡅࡓࡔࡢࡇࡔࡔࡎࡆࡅࡗࡍࡔࡔ࡟ࡄࡎࡒࡗࡊࡊࠧਖ"),
+  bstack11_opy_ (u"ࠧࡆࡔࡕࡣࡈࡕࡎࡏࡇࡆࡘࡎࡕࡎࡠࡔࡈࡗࡊ࡚ࠧਗ"),
+  bstack11_opy_ (u"ࠨࡇࡕࡖࡤࡉࡏࡏࡐࡈࡇ࡙ࡏࡏࡏࡡࡕࡉࡋ࡛ࡓࡆࡆࠪਘ"),
+  bstack11_opy_ (u"ࠩࡈࡖࡗࡥࡃࡐࡐࡑࡉࡈ࡚ࡉࡐࡐࡢࡅࡇࡕࡒࡕࡇࡇࠫਙ"),
+  bstack11_opy_ (u"ࠪࡉࡗࡘ࡟ࡄࡑࡑࡒࡊࡉࡔࡊࡑࡑࡣࡋࡇࡉࡍࡇࡇࠫਚ"),
+  bstack11_opy_ (u"ࠫࡊࡘࡒࡠࡐࡄࡑࡊࡥࡎࡐࡖࡢࡖࡊ࡙ࡏࡍࡘࡈࡈࠬਛ"),
+  bstack11_opy_ (u"ࠬࡋࡒࡓࡡࡄࡈࡉࡘࡅࡔࡕࡢࡍࡓ࡜ࡁࡍࡋࡇࠫਜ"),
+  bstack11_opy_ (u"࠭ࡅࡓࡔࡢࡅࡉࡊࡒࡆࡕࡖࡣ࡚ࡔࡒࡆࡃࡆࡌࡆࡈࡌࡆࠩਝ"),
+  bstack11_opy_ (u"ࠧࡆࡔࡕࡣ࡙࡛ࡎࡏࡇࡏࡣࡈࡕࡎࡏࡇࡆࡘࡎࡕࡎࡠࡈࡄࡍࡑࡋࡄࠨਞ"),
+  bstack11_opy_ (u"ࠨࡇࡕࡖࡤࡉࡏࡏࡐࡈࡇ࡙ࡏࡏࡏࡡࡗࡍࡒࡋࡄࡠࡑࡘࡘࠬਟ"),
+  bstack11_opy_ (u"ࠩࡈࡖࡗࡥࡓࡐࡅࡎࡗࡤࡉࡏࡏࡐࡈࡇ࡙ࡏࡏࡏࡡࡉࡅࡎࡒࡅࡅࠩਠ"),
+  bstack11_opy_ (u"ࠪࡉࡗࡘ࡟ࡔࡑࡆࡏࡘࡥࡃࡐࡐࡑࡉࡈ࡚ࡉࡐࡐࡢࡌࡔ࡙ࡔࡠࡗࡑࡖࡊࡇࡃࡉࡃࡅࡐࡊ࠭ਡ"),
+  bstack11_opy_ (u"ࠫࡊࡘࡒࡠࡒࡕࡓ࡝࡟࡟ࡄࡑࡑࡒࡊࡉࡔࡊࡑࡑࡣࡋࡇࡉࡍࡇࡇࠫਢ"),
+  bstack11_opy_ (u"ࠬࡋࡒࡓࡡࡑࡅࡒࡋ࡟ࡏࡑࡗࡣࡗࡋࡓࡐࡎ࡙ࡉࡉ࠭ਣ"),
+  bstack11_opy_ (u"࠭ࡅࡓࡔࡢࡒࡆࡓࡅࡠࡔࡈࡗࡔࡒࡕࡕࡋࡒࡒࡤࡌࡁࡊࡎࡈࡈࠬਤ"),
+  bstack11_opy_ (u"ࠧࡆࡔࡕࡣࡒࡇࡎࡅࡃࡗࡓࡗ࡟࡟ࡑࡔࡒ࡜࡞ࡥࡃࡐࡐࡉࡍࡌ࡛ࡒࡂࡖࡌࡓࡓࡥࡆࡂࡋࡏࡉࡉ࠭ਥ"),
 ]
-bstack1l1l1l1ll_opy_ = bstack1ll1_opy_ (u"ࠧࡔࡧࡷࡸ࡮ࡴࡧࠡࡷࡳࠤ࡫ࡵࡲࠡࡄࡵࡳࡼࡹࡥࡳࡵࡷࡥࡨࡱࠬࠡࡷࡶ࡭ࡳ࡭ࠠࡧࡴࡤࡱࡪࡽ࡯ࡳ࡭࠽ࠤࢀࢃࠧਥ")
-bstack1l1llll_opy_ = bstack1ll1_opy_ (u"ࠨࡅࡲࡱࡵࡲࡥࡵࡧࡧࠤࡸ࡫ࡴࡶࡲࠤࠫਦ")
-bstack11lll11_opy_ = bstack1ll1_opy_ (u"ࠩࡓࡥࡷࡹࡥࡥࠢࡦࡳࡳ࡬ࡩࡨࠢࡩ࡭ࡱ࡫࠺ࠡࡽࢀࠫਧ")
-bstack1l1ll1_opy_ = bstack1ll1_opy_ (u"ࠪࡗࡦࡴࡩࡵ࡫ࡽࡩࡩࠦࡣࡰࡰࡩ࡭࡬ࠦࡦࡪ࡮ࡨ࠾ࠥࢁࡽࠨਨ")
-bstack1lll1ll_opy_ = bstack1ll1_opy_ (u"࡚ࠫࡹࡩ࡯ࡩࠣ࡬ࡺࡨࠠࡶࡴ࡯࠾ࠥࢁࡽࠨ਩")
-bstack11lll11l_opy_ = bstack1ll1_opy_ (u"࡙ࠬࡥࡴࡵ࡬ࡳࡳࠦࡳࡵࡣࡵࡸࡪࡪࠠࡸ࡫ࡷ࡬ࠥ࡯ࡤ࠻ࠢࡾࢁࠬਪ")
-bstack1l1l11l1_opy_ = bstack1ll1_opy_ (u"࠭ࡒࡦࡥࡨ࡭ࡻ࡫ࡤࠡ࡫ࡱࡸࡪࡸࡲࡶࡲࡷ࠰ࠥ࡫ࡸࡪࡶ࡬ࡲ࡬࠭ਫ")
-bstack11l11_opy_ = bstack1ll1_opy_ (u"ࠧࡑ࡮ࡨࡥࡸ࡫ࠠࡪࡰࡶࡸࡦࡲ࡬ࠡࡵࡨࡰࡪࡴࡩࡶ࡯ࠣࡸࡴࠦࡲࡶࡰࠣࡸࡪࡹࡴࡴ࠰ࠣࡤࡵ࡯ࡰࠡ࡫ࡱࡷࡹࡧ࡬࡭ࠢࡶࡩࡱ࡫࡮ࡪࡷࡰࡤࠬਬ")
-bstack1lll11ll1_opy_ = bstack1ll1_opy_ (u"ࠨࡒ࡯ࡩࡦࡹࡥࠡ࡫ࡱࡷࡹࡧ࡬࡭ࠢࡳࡽࡹ࡫ࡳࡵࠢࡤࡲࡩࠦࡰࡺࡶࡨࡷࡹ࠳ࡳࡦ࡮ࡨࡲ࡮ࡻ࡭ࠡࡲࡤࡧࡰࡧࡧࡦࡵ࠱ࠤࡥࡶࡩࡱࠢ࡬ࡲࡸࡺࡡ࡭࡮ࠣࡴࡾࡺࡥࡴࡶࠣࡴࡾࡺࡥࡴࡶ࠰ࡷࡪࡲࡥ࡯࡫ࡸࡱࡥ࠭ਭ")
-bstack1llll1ll1_opy_ = bstack1ll1_opy_ (u"ࠩࡓࡰࡪࡧࡳࡦࠢ࡬ࡲࡸࡺࡡ࡭࡮ࠣࡶࡴࡨ࡯ࡵ࠮ࠣࡴࡦࡨ࡯ࡵࠢࡤࡲࡩࠦࡳࡦ࡮ࡨࡲ࡮ࡻ࡭࡭࡫ࡥࡶࡦࡸࡹࠡࡲࡤࡧࡰࡧࡧࡦࡵࠣࡸࡴࠦࡲࡶࡰࠣࡶࡴࡨ࡯ࡵࠢࡷࡩࡸࡺࡳࠡ࡫ࡱࠤࡵࡧࡲࡢ࡮࡯ࡩࡱ࠴ࠠࡡࡲ࡬ࡴࠥ࡯࡮ࡴࡶࡤࡰࡱࠦࡲࡰࡤࡲࡸ࡫ࡸࡡ࡮ࡧࡺࡳࡷࡱࠠࡳࡱࡥࡳࡹ࡬ࡲࡢ࡯ࡨࡻࡴࡸ࡫࠮ࡲࡤࡦࡴࡺࠠࡳࡱࡥࡳࡹ࡬ࡲࡢ࡯ࡨࡻࡴࡸ࡫࠮ࡵࡨࡰࡪࡴࡩࡶ࡯࡯࡭ࡧࡸࡡࡳࡻࡣࠫਮ")
-bstack1l111ll_opy_ = bstack1ll1_opy_ (u"ࠪࡔࡱ࡫ࡡࡴࡧࠣ࡭ࡳࡹࡴࡢ࡮࡯ࠤࡧ࡫ࡨࡢࡸࡨࠤࡹࡵࠠࡳࡷࡱࠤࡹ࡫ࡳࡵࡵ࠱ࠤࡥࡶࡩࡱࠢ࡬ࡲࡸࡺࡡ࡭࡮ࠣࡦࡪ࡮ࡡࡷࡧࡣࠫਯ")
-bstack1l11lll1l_opy_ = bstack1ll1_opy_ (u"ࠫࡕࡲࡥࡢࡵࡨࠤ࡮ࡴࡳࡵࡣ࡯ࡰࠥࡧࡰࡱ࡫ࡸࡱ࠲ࡩ࡬ࡪࡧࡱࡸࠥࡺ࡯ࠡࡴࡸࡲࠥࡺࡥࡴࡶࡶ࠲ࠥࡦࡰࡪࡲࠣ࡭ࡳࡹࡴࡢ࡮࡯ࠤࡆࡶࡰࡪࡷࡰ࠱ࡕࡿࡴࡩࡱࡱ࠱ࡈࡲࡩࡦࡰࡷࡤࠬਰ")
-bstack1llll111l_opy_ = bstack1ll1_opy_ (u"ࠬࡖ࡬ࡦࡣࡶࡩࠥ࡯࡮ࡴࡶࡤࡰࡱࠦࡰ࡭ࡣࡼࡻࡷ࡯ࡧࡩࡶࠣࡸࡴࠦࡲࡶࡰࠣࡸࡪࡹࡴࡴ࠰ࠣࡤࡵ࡯ࡰࠡ࡫ࡱࡷࡹࡧ࡬࡭ࠢࡳࡰࡦࡿࡷࡳ࡫ࡪ࡬ࡹࡦࠧ਱")
-bstack1l11l11l_opy_ = bstack1ll1_opy_ (u"࠭ࡈࡢࡰࡧࡰ࡮ࡴࡧࠡࡵࡨࡷࡸ࡯࡯࡯ࠢࡦࡰࡴࡹࡥࠨਲ")
-bstack1l11lllll_opy_ = bstack1ll1_opy_ (u"ࠧࡂ࡮࡯ࠤࡩࡵ࡮ࡦࠣࠪਲ਼")
-bstack1lllll_opy_ = bstack1ll1_opy_ (u"ࠨࡅࡲࡲ࡫࡯ࡧࠡࡨ࡬ࡰࡪࠦࡤࡰࡧࡶࠤࡳࡵࡴࠡࡧࡻ࡭ࡸࡺࠠࡢࡶࠣࡥࡳࡿࠠࡱࡣࡵࡩࡳࡺࠠࡥ࡫ࡵࡩࡨࡺ࡯ࡳࡻࠣࡳ࡫ࠦࠢࡼࡿࠥ࠲ࠥࡖ࡬ࡦࡣࡶࡩࠥ࡯࡮ࡤ࡮ࡸࡨࡪࠦࡡࠡࡤࡵࡳࡼࡹࡥࡳࡵࡷࡥࡨࡱ࠮ࡺ࡯࡯࠳ࡧࡸ࡯ࡸࡵࡨࡶࡸࡺࡡࡤ࡭࠱ࡽࡦࡳ࡬ࠡࡨ࡬ࡰࡪࠦࡣࡰࡰࡷࡥ࡮ࡴࡩ࡯ࡩࠣࡧࡴࡴࡦࡪࡩࡸࡶࡦࡺࡩࡰࡰࠣࡪࡴࡸࠠࡵࡧࡶࡸࡸ࠴ࠧ਴")
-bstack11l1llll_opy_ = bstack1ll1_opy_ (u"ࠩࡅࡶࡴࡽࡳࡦࡴࡶࡸࡦࡩ࡫ࠡࡥࡵࡩࡩ࡫࡮ࡵ࡫ࡤࡰࡸࠦ࡮ࡰࡶࠣࡴࡷࡵࡶࡪࡦࡨࡨ࠳ࠦࡐ࡭ࡧࡤࡷࡪࠦࡡࡥࡦࠣࡸ࡭࡫࡭ࠡ࡫ࡱࠤࡧࡸ࡯ࡸࡵࡨࡶࡸࡺࡡࡤ࡭࠱ࡽࡲࡲࠠࡤࡱࡱࡪ࡮࡭ࠠࡧ࡫࡯ࡩࠥࡧࡳࠡࠤࡸࡷࡪࡸࡎࡢ࡯ࡨࠦࠥࡧ࡮ࡥࠢࠥࡥࡨࡩࡥࡴࡵࡎࡩࡾࠨࠠࡰࡴࠣࡷࡪࡺࠠࡵࡪࡨࡱࠥࡧࡳࠡࡧࡱࡺ࡮ࡸ࡯࡯࡯ࡨࡲࡹࠦࡶࡢࡴ࡬ࡥࡧࡲࡥࡴ࠼ࠣࠦࡇࡘࡏࡘࡕࡈࡖࡘ࡚ࡁࡄࡍࡢ࡙ࡘࡋࡒࡏࡃࡐࡉࠧࠦࡡ࡯ࡦࠣࠦࡇࡘࡏࡘࡕࡈࡖࡘ࡚ࡁࡄࡍࡢࡅࡈࡉࡅࡔࡕࡢࡏࡊ࡟ࠢࠨਵ")
-bstack1ll11ll11_opy_ = bstack1ll1_opy_ (u"ࠪࡑࡦࡲࡦࡰࡴࡰࡩࡩࠦࡣࡰࡰࡩ࡭࡬ࠦࡦࡪ࡮ࡨ࠾ࠧࢁࡽࠣࠩਸ਼")
-bstack111ll11_opy_ = bstack1ll1_opy_ (u"ࠫࡊࡴࡣࡰࡷࡱࡸࡪࡸࡥࡥࠢࡨࡶࡷࡵࡲࠡࡹ࡫࡭ࡱ࡫ࠠࡴࡧࡷࡸ࡮ࡴࡧࠡࡷࡳࠤ࠲ࠦࡻࡾࠩ਷")
-bstack1l111l1_opy_ = bstack1ll1_opy_ (u"࡙ࠬࡴࡢࡴࡷ࡭ࡳ࡭ࠠࡃࡴࡲࡻࡸ࡫ࡲࡴࡶࡤࡧࡰࠦࡌࡰࡥࡤࡰࠬਸ")
-bstack1l11l111_opy_ = bstack1ll1_opy_ (u"࠭ࡓࡵࡱࡳࡴ࡮ࡴࡧࠡࡄࡵࡳࡼࡹࡥࡳࡵࡷࡥࡨࡱࠠࡍࡱࡦࡥࡱ࠭ਹ")
-bstack1ll11ll1_opy_ = bstack1ll1_opy_ (u"ࠧࡃࡴࡲࡻࡸ࡫ࡲࡴࡶࡤࡧࡰࠦࡌࡰࡥࡤࡰࠥ࡯ࡳࠡࡰࡲࡻࠥࡸࡵ࡯ࡰ࡬ࡲ࡬ࠧࠧ਺")
-bstack1llll1ll_opy_ = bstack1ll1_opy_ (u"ࠨࡅࡲࡹࡱࡪࠠ࡯ࡱࡷࠤࡸࡺࡡࡳࡶࠣࡆࡷࡵࡷࡴࡧࡵࡷࡹࡧࡣ࡬ࠢࡏࡳࡨࡧ࡬࠻ࠢࡾࢁࠬ਻")
-bstack11l1ll1l_opy_ = bstack1ll1_opy_ (u"ࠩࡖࡸࡦࡸࡴࡪࡰࡪࠤࡱࡵࡣࡢ࡮ࠣࡦ࡮ࡴࡡࡳࡻࠣࡻ࡮ࡺࡨࠡࡱࡳࡸ࡮ࡵ࡮ࡴ࠼ࠣࡿࢂ਼࠭")
-bstack1ll1lll11_opy_ = bstack1ll1_opy_ (u"࡙ࠪࡵࡪࡡࡵ࡫ࡱ࡫ࠥࡹࡥࡴࡵ࡬ࡳࡳࠦࡤࡦࡶࡤ࡭ࡱࡹ࠺ࠡࡽࢀࠫ਽")
-bstack1l1l1ll_opy_ = bstack1ll1_opy_ (u"ࠫࡊࡸࡲࡰࡴࠣ࡭ࡳࠦࡳࡦࡶࡷ࡭ࡳ࡭ࠠࡶࡲࡧࡥࡹ࡯࡮ࡨࠢࡷࡩࡸࡺࠠࡴࡶࡤࡸࡺࡹࠠࡼࡿࠪਾ")
-bstack1111l1l1_opy_ = bstack1ll1_opy_ (u"ࠬࡖ࡬ࡦࡣࡶࡩࠥࡶࡲࡰࡸ࡬ࡨࡪࠦࡡ࡯ࠢࡤࡴࡵࡸ࡯ࡱࡴ࡬ࡥࡹ࡫ࠠࡇ࡙ࠣࠬࡷࡵࡢࡰࡶ࠲ࡴࡦࡨ࡯ࡵࠫࠣ࡭ࡳࠦࡣࡰࡰࡩ࡭࡬ࠦࡦࡪ࡮ࡨ࠰ࠥࡹ࡫ࡪࡲࠣࡸ࡭࡫ࠠࡧࡴࡤࡱࡪࡽ࡯ࡳ࡭ࠣ࡯ࡪࡿࠠࡪࡰࠣࡧࡴࡴࡦࡪࡩࠣ࡭࡫ࠦࡲࡶࡰࡱ࡭ࡳ࡭ࠠࡴ࡫ࡰࡴࡱ࡫ࠠࡱࡻࡷ࡬ࡴࡴࠠࡴࡥࡵ࡭ࡵࡺࠠࡸ࡫ࡷ࡬ࡴࡻࡴࠡࡣࡱࡽࠥࡌࡗ࠯ࠩਿ")
-bstack11lllll_opy_ = bstack1ll1_opy_ (u"࠭ࡓࡦࡶࡷ࡭ࡳ࡭ࠠࡩࡶࡷࡴࡕࡸ࡯ࡹࡻ࠲࡬ࡹࡺࡰࡴࡒࡵࡳࡽࡿࠠࡪࡵࠣࡲࡴࡺࠠࡴࡷࡳࡴࡴࡸࡴࡦࡦࠣࡳࡳࠦࡣࡶࡴࡵࡩࡳࡺ࡬ࡺࠢ࡬ࡲࡸࡺࡡ࡭࡮ࡨࡨࠥࡼࡥࡳࡵ࡬ࡳࡳࠦ࡯ࡧࠢࡶࡩࡱ࡫࡮ࡪࡷࡰࠤ࠭ࢁࡽࠪ࠮ࠣࡴࡱ࡫ࡡࡴࡧࠣࡹࡵ࡭ࡲࡢࡦࡨࠤࡹࡵࠠࡔࡧ࡯ࡩࡳ࡯ࡵ࡮ࡀࡀ࠸࠳࠶࠮࠱ࠢࡲࡶࠥࡸࡥࡧࡧࡵࠤࡹࡵࠠࡩࡶࡷࡴࡸࡀ࠯࠰ࡹࡺࡻ࠳ࡨࡲࡰࡹࡶࡩࡷࡹࡴࡢࡥ࡮࠲ࡨࡵ࡭࠰ࡦࡲࡧࡸ࠵ࡡࡶࡶࡲࡱࡦࡺࡥ࠰ࡵࡨࡰࡪࡴࡩࡶ࡯࠲ࡶࡺࡴ࠭ࡵࡧࡶࡸࡸ࠳ࡢࡦࡪ࡬ࡲࡩ࠳ࡰࡳࡱࡻࡽࠨࡶࡹࡵࡪࡲࡲࠥ࡬࡯ࡳࠢࡤࠤࡼࡵࡲ࡬ࡣࡵࡳࡺࡴࡤ࠯ࠩੀ")
-bstack1111llll_opy_ = bstack1ll1_opy_ (u"ࠧࡈࡧࡱࡩࡷࡧࡴࡪࡰࡪࠤࡧࡸ࡯ࡸࡵࡨࡶࡸࡺࡡࡤ࡭ࠣࡧࡴࡴࡦࡪࡩࡸࡶࡦࡺࡩࡰࡰࠣࡽࡲࡲࠠࡧ࡫࡯ࡩ࠳࠴ࠧੁ")
-bstack11111ll_opy_ = bstack1ll1_opy_ (u"ࠨࡕࡸࡧࡨ࡫ࡳࡴࡨࡸࡰࡱࡿࠠࡨࡧࡱࡩࡷࡧࡴࡦࡦࠣࡸ࡭࡫ࠠࡤࡱࡱࡪ࡮࡭ࡵࡳࡣࡷ࡭ࡴࡴࠠࡧ࡫࡯ࡩࠦ࠭ੂ")
-bstack1l111111_opy_ = bstack1ll1_opy_ (u"ࠩࡉࡥ࡮ࡲࡥࡥࠢࡷࡳࠥ࡭ࡥ࡯ࡧࡵࡥࡹ࡫ࠠࡵࡪࡨࠤࡧࡸ࡯ࡸࡵࡨࡶࡸࡺࡡࡤ࡭ࠣࡧࡴࡴࡦࡪࡩࡸࡶࡦࡺࡩࡰࡰࠣࡪ࡮ࡲࡥ࠯ࠢࡾࢁࠬ੃")
-bstack1lll1lll_opy_ = bstack1ll1_opy_ (u"ࠪࡉࡽࡶࡥࡤࡶࡨࡨࠥࡧࡴࠡ࡮ࡨࡥࡸࡺࠠ࠲ࠢ࡬ࡲࡵࡻࡴ࠭ࠢࡵࡩࡨ࡫ࡩࡷࡧࡧࠤ࠵࠭੄")
-bstack111llll1_opy_ = bstack1ll1_opy_ (u"ࠫࡊࡸࡲࡰࡴࠣࡨࡺࡸࡩ࡯ࡩࠣࡅࡵࡶࠠࡶࡲ࡯ࡳࡦࡪ࠮ࠡࡽࢀࠫ੅")
-bstack111ll11l_opy_ = bstack1ll1_opy_ (u"ࠬࡌࡡࡪ࡮ࡨࡨࠥࡺ࡯ࠡࡷࡳࡰࡴࡧࡤࠡࡃࡳࡴ࠳ࠦࡉ࡯ࡸࡤࡰ࡮ࡪࠠࡧ࡫࡯ࡩࠥࡶࡡࡵࡪࠣࡴࡷࡵࡶࡪࡦࡨࡨࠥࢁࡽ࠯ࠩ੆")
-bstack1ll11ll_opy_ = bstack1ll1_opy_ (u"࠭ࡋࡦࡻࡶࠤࡨࡧ࡮࡯ࡱࡷࠤࡨࡵ࠭ࡦࡺ࡬ࡷࡹࠦࡡࡴࠢࡤࡴࡵࠦࡶࡢ࡮ࡸࡩࡸ࠲ࠠࡶࡵࡨࠤࡦࡴࡹࠡࡱࡱࡩࠥࡶࡲࡰࡲࡨࡶࡹࡿࠠࡧࡴࡲࡱࠥࢁࡩࡥ࠾ࡶࡸࡷ࡯࡮ࡨࡀ࠯ࠤࡵࡧࡴࡩ࠾ࡶࡸࡷ࡯࡮ࡨࡀ࠯ࠤࡨࡻࡳࡵࡱࡰࡣ࡮ࡪ࠼ࡴࡶࡵ࡭ࡳ࡭࠾࠭ࠢࡶ࡬ࡦࡸࡥࡢࡤ࡯ࡩࡤ࡯ࡤ࠽ࡵࡷࡶ࡮ࡴࡧ࠿ࡿ࠯ࠤࡴࡴ࡬ࡺࠢࠥࡴࡦࡺࡨࠣࠢࡤࡲࡩࠦࠢࡤࡷࡶࡸࡴࡳ࡟ࡪࡦࠥࠤࡨࡧ࡮ࠡࡥࡲ࠱ࡪࡾࡩࡴࡶࠣࡸࡴ࡭ࡥࡵࡪࡨࡶ࠳࠭ੇ")
-bstack1l1ll1l1l_opy_ = bstack1ll1_opy_ (u"ࠧ࡜ࡋࡱࡺࡦࡲࡩࡥࠢࡤࡴࡵࠦࡰࡳࡱࡳࡩࡷࡺࡹ࡞ࠢࡶࡹࡵࡶ࡯ࡳࡶࡨࡨࠥࡶࡲࡰࡲࡨࡶࡹ࡯ࡥࡴࠢࡤࡶࡪࠦࡻࡪࡦ࠿ࡷࡹࡸࡩ࡯ࡩࡁ࠰ࠥࡶࡡࡵࡪ࠿ࡷࡹࡸࡩ࡯ࡩࡁ࠰ࠥࡩࡵࡴࡶࡲࡱࡤ࡯ࡤ࠽ࡵࡷࡶ࡮ࡴࡧ࠿࠮ࠣࡷ࡭ࡧࡲࡦࡣࡥࡰࡪࡥࡩࡥ࠾ࡶࡸࡷ࡯࡮ࡨࡀࢀ࠲ࠥࡌ࡯ࡳࠢࡰࡳࡷ࡫ࠠࡥࡧࡷࡥ࡮ࡲࡳࠡࡲ࡯ࡩࡦࡹࡥࠡࡸ࡬ࡷ࡮ࡺࠠࡩࡶࡷࡴࡸࡀ࠯࠰ࡹࡺࡻ࠳ࡨࡲࡰࡹࡶࡩࡷࡹࡴࡢࡥ࡮࠲ࡨࡵ࡭࠰ࡦࡲࡧࡸ࠵ࡡࡱࡲ࠰ࡥࡺࡺ࡯࡮ࡣࡷࡩ࠴ࡧࡰࡱ࡫ࡸࡱ࠴ࡹࡥࡵ࠯ࡸࡴ࠲ࡺࡥࡴࡶࡶ࠳ࡸࡶࡥࡤ࡫ࡩࡽ࠲ࡧࡰࡱࠩੈ")
-bstack111ll1l1_opy_ = bstack1ll1_opy_ (u"ࠨ࡝ࡌࡲࡻࡧ࡬ࡪࡦࠣࡥࡵࡶࠠࡱࡴࡲࡴࡪࡸࡴࡺ࡟ࠣࡗࡺࡶࡰࡰࡴࡷࡩࡩࠦࡶࡢ࡮ࡸࡩࡸࠦ࡯ࡧࠢࡤࡴࡵࠦࡡࡳࡧࠣࡳ࡫ࠦࡻࡪࡦ࠿ࡷࡹࡸࡩ࡯ࡩࡁ࠰ࠥࡶࡡࡵࡪ࠿ࡷࡹࡸࡩ࡯ࡩࡁ࠰ࠥࡩࡵࡴࡶࡲࡱࡤ࡯ࡤ࠽ࡵࡷࡶ࡮ࡴࡧ࠿࠮ࠣࡷ࡭ࡧࡲࡦࡣࡥࡰࡪࡥࡩࡥ࠾ࡶࡸࡷ࡯࡮ࡨࡀࢀ࠲ࠥࡌ࡯ࡳࠢࡰࡳࡷ࡫ࠠࡥࡧࡷࡥ࡮ࡲࡳࠡࡲ࡯ࡩࡦࡹࡥࠡࡸ࡬ࡷ࡮ࡺࠠࡩࡶࡷࡴࡸࡀ࠯࠰ࡹࡺࡻ࠳ࡨࡲࡰࡹࡶࡩࡷࡹࡴࡢࡥ࡮࠲ࡨࡵ࡭࠰ࡦࡲࡧࡸ࠵ࡡࡱࡲ࠰ࡥࡺࡺ࡯࡮ࡣࡷࡩ࠴ࡧࡰࡱ࡫ࡸࡱ࠴ࡹࡥࡵ࠯ࡸࡴ࠲ࡺࡥࡴࡶࡶ࠳ࡸࡶࡥࡤ࡫ࡩࡽ࠲ࡧࡰࡱࠩ੉")
-bstack1llllll1l_opy_ = bstack1ll1_opy_ (u"ࠩࡘࡷ࡮ࡴࡧࠡࡧࡻ࡭ࡸࡺࡩ࡯ࡩࠣࡥࡵࡶࠠࡪࡦࠣࡿࢂࠦࡦࡰࡴࠣ࡬ࡦࡹࡨࠡ࠼ࠣࡿࢂ࠴ࠧ੊")
-bstack11lllll1_opy_ = bstack1ll1_opy_ (u"ࠪࡅࡵࡶࠠࡖࡲ࡯ࡳࡦࡪࡥࡥࠢࡖࡹࡨࡩࡥࡴࡵࡩࡹࡱࡲࡹ࠯ࠢࡌࡈࠥࡀࠠࡼࡿࠪੋ")
-bstack1l11l11_opy_ = bstack1ll1_opy_ (u"࡚ࠫࡹࡩ࡯ࡩࠣࡅࡵࡶࠠ࠻ࠢࡾࢁ࠳࠭ੌ")
-bstack11ll1l_opy_ = bstack1ll1_opy_ (u"ࠬࡶࡡࡳࡣ࡯ࡰࡪࡲࡳࡑࡧࡵࡔࡱࡧࡴࡧࡱࡵࡱࠥ࡯ࡳࠡࡰࡲࡸࠥࡹࡵࡱࡲࡲࡶࡹ࡫ࡤࠡࡨࡲࡶࠥࡼࡡ࡯࡫࡯ࡰࡦࠦࡰࡺࡶ࡫ࡳࡳࠦࡴࡦࡵࡷࡷ࠱ࠦࡲࡶࡰࡱ࡭ࡳ࡭ࠠࡸ࡫ࡷ࡬ࠥࡶࡡࡳࡣ࡯ࡰࡪࡲࡐࡦࡴࡓࡰࡦࡺࡦࡰࡴࡰࠤࡂࠦ࠱ࠨ੍")
-bstack11111l_opy_ = bstack1ll1_opy_ (u"࠭ࡅࡳࡴࡲࡶࠥ࡯࡮ࠡࡥࡵࡩࡦࡺࡩ࡯ࡩࠣࡦࡺ࡯࡬ࡥࡋࡧࡩࡳࡺࡩࡧ࡫ࡨࡶ࠿ࠦࡻࡾࠩ੎")
-bstack1l11llll1_opy_ = bstack1ll1_opy_ (u"ࠧࡄࡱࡸࡰࡩࠦ࡮ࡰࡶࠣࡧࡱࡵࡳࡦࠢࡥࡶࡴࡽࡳࡦࡴ࠽ࠤࢀࢃࠧ੏")
-bstack1l1l1ll1l_opy_ = bstack1ll1_opy_ (u"ࠨࡅࡲࡹࡱࡪࠠ࡯ࡱࡷࠤ࡬࡫ࡴࠡࡴࡨࡥࡸࡵ࡮ࠡࡨࡲࡶࠥࡨࡥࡩࡣࡹࡩࠥ࡬ࡥࡢࡶࡸࡶࡪࠦࡦࡢ࡫࡯ࡹࡷ࡫࠮ࠡࡽࢀࠫ੐")
-bstack11ll1l1_opy_ = bstack1ll1_opy_ (u"ࠩࡈࡶࡷࡵࡲࠡࡹ࡫࡭ࡱ࡫ࠠࡨࡧࡷࡸ࡮ࡴࡧࠡࡴࡨࡷࡵࡵ࡮ࡴࡧࠣࡪࡷࡵ࡭ࠡࡣࡳ࡭ࠥࡩࡡ࡭࡮࠱ࠤࡊࡸࡲࡰࡴ࠽ࠤࢀࢃࠧੑ")
-bstack11ll1ll_opy_ = bstack1ll1_opy_ (u"࡙ࠪࡳࡧࡢ࡭ࡧࠣࡸࡴࠦࡳࡩࡱࡺࠤࡧࡻࡩ࡭ࡦ࡙ࠣࡗࡒࠬࠡࡣࡶࠤࡧࡻࡩ࡭ࡦࠣࡧࡦࡶࡡࡣ࡫࡯࡭ࡹࡿࠠࡪࡵࠣࡲࡴࡺࠠࡶࡵࡨࡨ࠳࠭੒")
-bstack1111_opy_ = bstack1ll1_opy_ (u"ࠫࡘ࡫ࡲࡷࡧࡵࠤࡸ࡯ࡤࡦࠢࡥࡹ࡮ࡲࡤࡏࡣࡰࡩ࠭ࢁࡽࠪࠢ࡬ࡷࠥࡴ࡯ࡵࠢࡶࡥࡲ࡫ࠠࡢࡵࠣࡧࡱ࡯ࡥ࡯ࡶࠣࡷ࡮ࡪࡥࠡࡤࡸ࡭ࡱࡪࡎࡢ࡯ࡨࠬࢀࢃࠩࠨ੓")
-bstack1lll11_opy_ = bstack1ll1_opy_ (u"ࠬ࡜ࡩࡦࡹࠣࡦࡺ࡯࡬ࡥࠢࡲࡲࠥࡈࡲࡰࡹࡶࡩࡷ࡙ࡴࡢࡥ࡮ࠤࡩࡧࡳࡩࡤࡲࡥࡷࡪ࠺ࠡࡽࢀࠫ੔")
-bstack1111111l_opy_ = bstack1ll1_opy_ (u"࠭ࡕ࡯ࡣࡥࡰࡪࠦࡴࡰࠢࡤࡧࡨ࡫ࡳࡴࠢࡤࠤࡵࡸࡩࡷࡣࡷࡩࠥࡪ࡯࡮ࡣ࡬ࡲ࠿ࠦࡻࡾࠢ࠱ࠤࡘ࡫ࡴࠡࡶ࡫ࡩࠥ࡬࡯࡭࡮ࡲࡻ࡮ࡴࡧࠡࡥࡲࡲ࡫࡯ࡧࠡ࡫ࡱࠤࡾࡵࡵࡳࠢࡥࡶࡴࡽࡳࡦࡴࡶࡸࡦࡩ࡫࠯ࡻࡰࡰࠥ࡬ࡩ࡭ࡧ࠽ࠤࡡࡴ࠭࠮࠯࠰࠱࠲࠳࠭࠮࠯࠰ࠤࡡࡴࠠࡣࡴࡲࡻࡸ࡫ࡲࡴࡶࡤࡧࡰࡒ࡯ࡤࡣ࡯࠾ࠥࡺࡲࡶࡧࠣࡠࡳ࠳࠭࠮࠯࠰࠱࠲࠳࠭࠮࠯ࠪ੕")
-bstack1l1l1ll1_opy_ = bstack1ll1_opy_ (u"ࠧࡔࡱࡰࡩࡹ࡮ࡩ࡯ࡩࠣࡻࡪࡴࡴࠡࡹࡵࡳࡳ࡭ࠠࡸࡪ࡬ࡰࡪࠦࡥࡹࡧࡦࡹࡹ࡯࡮ࡨࠢࡪࡩࡹࡥ࡮ࡶࡦࡪࡩࡤࡲ࡯ࡤࡣ࡯ࡣࡪࡸࡲࡰࡴࠣ࠾ࠥࢁࡽࠨ੖")
-bstack11ll11l_opy_ = bstack1ll1_opy_ (u"ࠣࡇࡵࡶࡴࡸࠠࡪࡰࠣࡷࡪࡴࡤࡠࡣࡰࡴࡱ࡯ࡴࡶࡦࡨࡣࡪࡼࡥ࡯ࡶࠣࡪࡴࡸࠠࡔࡆࡎࡗࡪࡺࡵࡱࠢࡾࢁࠧ੗")
-bstack1l1l1lll_opy_ = bstack1ll1_opy_ (u"ࠤࡈࡶࡷࡵࡲࠡ࡫ࡱࠤࡸ࡫࡮ࡥࡡࡤࡱࡵࡲࡩࡵࡷࡧࡩࡤ࡫ࡶࡦࡰࡷࠤ࡫ࡵࡲࠡࡕࡇࡏ࡙࡫ࡳࡵࡃࡷࡸࡪࡳࡰࡵࡧࡧࠤࢀࢃࠢ੘")
-bstack1l1lll11l_opy_ = bstack1ll1_opy_ (u"ࠥࡉࡷࡸ࡯ࡳࠢ࡬ࡲࠥࡹࡥ࡯ࡦࡢࡥࡲࡶ࡬ࡪࡶࡸࡨࡪࡥࡥࡷࡧࡱࡸࠥ࡬࡯ࡳࠢࡖࡈࡐ࡚ࡥࡴࡶࡖࡹࡨࡩࡥࡴࡵࡩࡹࡱࠦࡻࡾࠤਖ਼")
-bstack1l1l11111_opy_ = bstack1ll1_opy_ (u"ࠦࡊࡸࡲࡰࡴࠣ࡭ࡳࠦࡦࡪࡴࡨࡣࡷ࡫ࡱࡶࡧࡶࡸࠥࢁࡽࠣਗ਼")
-bstack11ll11_opy_ = bstack1ll1_opy_ (u"ࠧࡖࡏࡔࡖࠣࡉࡻ࡫࡮ࡵࠢࡾࢁࠥࡸࡥࡴࡲࡲࡲࡸ࡫ࠠ࠻ࠢࡾࢁࠧਜ਼")
-bstack1l11ll1ll_opy_ = bstack1ll1_opy_ (u"࠭ࡆࡢ࡫࡯ࡩࡩࠦࡴࡰࠢࡦࡳࡳ࡬ࡩࡨࡷࡵࡩࠥࡶࡲࡰࡺࡼࠤࡸ࡫ࡴࡵ࡫ࡱ࡫ࡸ࠲ࠠࡦࡴࡵࡳࡷࡀࠠࡼࡿࠪੜ")
-bstack11l111l1_opy_ = bstack1ll1_opy_ (u"ࠧࠡࠢ࠲࠮ࠥࡃ࠽࠾࠿ࡀࡁࡂࡃ࠽࠾࠿ࡀࡁࡂࡃ࠽࠾࠿ࡀࡁࡂࡃ࠽࠾࠿ࡀࡁࡂࡃ࠽࠾࠿ࡀࡁࡂࡃ࠽࠾࠿ࡀࡁࡂࡃ࠽࠾࠿ࡀࡁࡂࡃ࠽࠾࠿ࡀࡁࡂࡃ࠽࠾࠿ࡀࡁࡂࡃ࠽࠾࠿ࡀࡁࡂࡃ࠽࠾࠿ࡀࡁࡂࡃ࠽࠾࠿ࡀࡁࡂࡃ࠽࠾࠿ࡀࡁࡂࡃ࠽࠾࠿ࡀࡁࡂࡃ࠽࠾࠿ࡀࡁࡂࡃ࠽࠾࠿ࡀࡁࡂࡃ࠽࠾࠿ࡀࡁࡂࡃ࠽࠾ࠢ࠭࠳ࡡࡴࠠࠡ࡫ࡩࠬࡵࡧࡧࡦࠢࡀࡁࡂࠦࡶࡰ࡫ࡧࠤ࠵࠯ࠠࡼ࡞ࡱࠤࠥࠦࡴࡳࡻࡾࡠࡳࠦࡣࡰࡰࡶࡸࠥ࡬ࡳࠡ࠿ࠣࡶࡪࡷࡵࡪࡴࡨࠬࡡ࠭ࡦࡴ࡞ࠪ࠭ࡀࡢ࡮ࠡࠢࠣࠤࠥ࡬ࡳ࠯ࡣࡳࡴࡪࡴࡤࡇ࡫࡯ࡩࡘࡿ࡮ࡤࠪࡥࡷࡹࡧࡣ࡬ࡡࡳࡥࡹ࡮ࠬࠡࡌࡖࡓࡓ࠴ࡳࡵࡴ࡬ࡲ࡬࡯ࡦࡺࠪࡳࡣ࡮ࡴࡤࡦࡺࠬࠤ࠰ࠦࠢ࠻ࠤࠣ࠯ࠥࡐࡓࡐࡐ࠱ࡷࡹࡸࡩ࡯ࡩ࡬ࡪࡾ࠮ࡊࡔࡑࡑ࠲ࡵࡧࡲࡴࡧࠫࠬࡦࡽࡡࡪࡶࠣࡲࡪࡽࡐࡢࡩࡨ࠶࠳࡫ࡶࡢ࡮ࡸࡥࡹ࡫ࠨࠣࠪࠬࠤࡂࡄࠠࡼࡿࠥ࠰ࠥࡢࠧࡣࡴࡲࡻࡸ࡫ࡲࡴࡶࡤࡧࡰࡥࡥࡹࡧࡦࡹࡹࡵࡲ࠻ࠢࡾࠦࡦࡩࡴࡪࡱࡱࠦ࠿ࠦࠢࡨࡧࡷࡗࡪࡹࡳࡪࡱࡱࡈࡪࡺࡡࡪ࡮ࡶࠦࢂࡢࠧࠪࠫࠬ࡟ࠧ࡮ࡡࡴࡪࡨࡨࡤ࡯ࡤࠣ࡟ࠬࠤ࠰ࠦࠢ࠭࡞࡟ࡲࠧ࠯࡜࡯ࠢࠣࠤࠥࢃࡣࡢࡶࡦ࡬࠭࡫ࡸࠪࡽ࡟ࡲࠥࠦࠠࠡࡿ࡟ࡲࠥࠦࡽ࡝ࡰࠣࠤ࠴࠰ࠠ࠾࠿ࡀࡁࡂࡃ࠽࠾࠿ࡀࡁࡂࡃ࠽࠾࠿ࡀࡁࡂࡃ࠽࠾࠿ࡀࡁࡂࡃ࠽࠾࠿ࡀࡁࡂࡃ࠽࠾࠿ࡀࡁࡂࡃ࠽࠾࠿ࡀࡁࡂࡃ࠽࠾࠿ࡀࡁࡂࡃ࠽࠾࠿ࡀࡁࡂࡃ࠽࠾࠿ࡀࡁࡂࡃ࠽࠾࠿ࡀࡁࡂࡃ࠽࠾࠿ࡀࡁࡂࡃ࠽࠾࠿ࡀࡁࡂࡃ࠽࠾࠿ࡀࡁࡂࡃ࠽࠾࠿ࡀࡁࡂࡃ࠽࠾࠿ࡀࡁࡂࡃ࠽࠾࠿ࡀࡁࡂࡃ࠽࠾࠿ࡀࠤ࠯࠵ࠧ੝")
-bstack1ll1llll1_opy_ = bstack1ll1_opy_ (u"ࠨ࡞ࡱ࠳࠯ࠦ࠽࠾࠿ࡀࡁࡂࡃ࠽࠾࠿ࡀࡁࡂࡃ࠽࠾࠿ࡀࡁࡂࡃ࠽࠾࠿ࡀࡁࡂࡃ࠽࠾࠿ࡀࡁࡂࡃ࠽࠾࠿ࡀࡁࡂࡃ࠽࠾࠿ࡀࡁࡂࡃ࠽࠾࠿ࡀࡁࡂࡃ࠽࠾࠿ࡀࡁࡂࡃ࠽࠾࠿ࡀࡁࡂࡃ࠽࠾࠿ࡀࡁࡂࡃ࠽࠾࠿ࡀࡁࡂࡃ࠽࠾࠿ࡀࡁࡂࡃ࠽࠾࠿ࡀࡁࡂࡃ࠽࠾࠿ࡀࡁࡂࡃ࠽࠾࠿ࡀࡁࡂࡃ࠽࠾࠿ࡀࡁࡂࡃ࠽࠾࠿ࠣ࠮࠴ࡢ࡮ࡤࡱࡱࡷࡹࠦࡢࡴࡶࡤࡧࡰࡥࡰࡢࡶ࡫ࠤࡂࠦࡰࡳࡱࡦࡩࡸࡹ࠮ࡢࡴࡪࡺࡠࡶࡲࡰࡥࡨࡷࡸ࠴ࡡࡳࡩࡹ࠲ࡱ࡫࡮ࡨࡶ࡫ࠤ࠲ࠦ࠳࡞࡞ࡱࡧࡴࡴࡳࡵࠢࡥࡷࡹࡧࡣ࡬ࡡࡦࡥࡵࡹࠠ࠾ࠢࡳࡶࡴࡩࡥࡴࡵ࠱ࡥࡷ࡭ࡶ࡜ࡲࡵࡳࡨ࡫ࡳࡴ࠰ࡤࡶ࡬ࡼ࠮࡭ࡧࡱ࡫ࡹ࡮ࠠ࠮ࠢ࠴ࡡࡡࡴࡣࡰࡰࡶࡸࠥࡶ࡟ࡪࡰࡧࡩࡽࠦ࠽ࠡࡲࡵࡳࡨ࡫ࡳࡴ࠰ࡤࡶ࡬ࡼ࡛ࡱࡴࡲࡧࡪࡹࡳ࠯ࡣࡵ࡫ࡻ࠴࡬ࡦࡰࡪࡸ࡭ࠦ࠭ࠡ࠴ࡠࡠࡳࡶࡲࡰࡥࡨࡷࡸ࠴ࡡࡳࡩࡹࠤࡂࠦࡰࡳࡱࡦࡩࡸࡹ࠮ࡢࡴࡪࡺ࠳ࡹ࡬ࡪࡥࡨࠬ࠵࠲ࠠࡱࡴࡲࡧࡪࡹࡳ࠯ࡣࡵ࡫ࡻ࠴࡬ࡦࡰࡪࡸ࡭ࠦ࠭ࠡ࠵ࠬࡠࡳࡩ࡯࡯ࡵࡷࠤ࡮ࡳࡰࡰࡴࡷࡣࡵࡲࡡࡺࡹࡵ࡭࡬࡮ࡴ࠵ࡡࡥࡷࡹࡧࡣ࡬ࠢࡀࠤࡷ࡫ࡱࡶ࡫ࡵࡩ࠭ࠨࡰ࡭ࡣࡼࡻࡷ࡯ࡧࡩࡶࠥ࠭ࡀࡢ࡮ࡪ࡯ࡳࡳࡷࡺ࡟ࡱ࡮ࡤࡽࡼࡸࡩࡨࡪࡷ࠸ࡤࡨࡳࡵࡣࡦ࡯࠳ࡩࡨࡳࡱࡰ࡭ࡺࡳ࠮࡭ࡣࡸࡲࡨ࡮ࠠ࠾ࠢࡤࡷࡾࡴࡣࠡࠪ࡯ࡥࡺࡴࡣࡩࡑࡳࡸ࡮ࡵ࡮ࡴࠫࠣࡁࡃࠦࡻ࡝ࡰ࡯ࡩࡹࠦࡣࡢࡲࡶ࠿ࡡࡴࡴࡳࡻࠣࡿࡡࡴࡣࡢࡲࡶࠤࡂࠦࡊࡔࡑࡑ࠲ࡵࡧࡲࡴࡧࠫࡦࡸࡺࡡࡤ࡭ࡢࡧࡦࡶࡳࠪ࡞ࡱࠤࠥࢃࠠࡤࡣࡷࡧ࡭࠮ࡥࡹࠫࠣࡿࡡࡴࠠࠡࠢࠣࢁࡡࡴࠠࠡࡴࡨࡸࡺࡸ࡮ࠡࡣࡺࡥ࡮ࡺࠠࡪ࡯ࡳࡳࡷࡺ࡟ࡱ࡮ࡤࡽࡼࡸࡩࡨࡪࡷ࠸ࡤࡨࡳࡵࡣࡦ࡯࠳ࡩࡨࡳࡱࡰ࡭ࡺࡳ࠮ࡤࡱࡱࡲࡪࡩࡴࠩࡽ࡟ࡲࠥࠦࠠࠡࡹࡶࡉࡳࡪࡰࡰ࡫ࡱࡸ࠿ࠦࡠࡸࡵࡶ࠾࠴࠵ࡣࡥࡲ࠱ࡦࡷࡵࡷࡴࡧࡵࡷࡹࡧࡣ࡬࠰ࡦࡳࡲ࠵ࡰ࡭ࡣࡼࡻࡷ࡯ࡧࡩࡶࡂࡧࡦࡶࡳ࠾ࠦࡾࡩࡳࡩ࡯ࡥࡧࡘࡖࡎࡉ࡯࡮ࡲࡲࡲࡪࡴࡴࠩࡌࡖࡓࡓ࠴ࡳࡵࡴ࡬ࡲ࡬࡯ࡦࡺࠪࡦࡥࡵࡹࠩࠪࡿࡣ࠰ࡡࡴࠠࠡࠢࠣ࠲࠳࠴࡬ࡢࡷࡱࡧ࡭ࡕࡰࡵ࡫ࡲࡲࡸࡢ࡮ࠡࠢࢀ࠭ࡡࡴࡽ࡝ࡰ࠲࠮ࠥࡃ࠽࠾࠿ࡀࡁࡂࡃ࠽࠾࠿ࡀࡁࡂࡃ࠽࠾࠿ࡀࡁࡂࡃ࠽࠾࠿ࡀࡁࡂࡃ࠽࠾࠿ࡀࡁࡂࡃ࠽࠾࠿ࡀࡁࡂࡃ࠽࠾࠿ࡀࡁࡂࡃ࠽࠾࠿ࡀࡁࡂࡃ࠽࠾࠿ࡀࡁࡂࡃ࠽࠾࠿ࡀࡁࡂࡃ࠽࠾࠿ࡀࡁࡂࡃ࠽࠾࠿ࡀࡁࡂࡃ࠽࠾࠿ࡀࡁࡂࡃ࠽࠾࠿ࡀࡁࡂࡃ࠽࠾࠿ࡀࡁࡂࡃ࠽࠾࠿ࡀࡁࡂࡃ࠽࠾࠿ࡀࡁࡂࡃ࠽࠾ࠢ࠭࠳ࡡࡴࠧਫ਼")
+def bstack1l1lllll_opy_():
+  global CONFIG
+  headers = {
+        bstack11_opy_ (u"ࠨࡅࡲࡲࡹ࡫࡮ࡵ࠯ࡷࡽࡵ࡫ࠧਦ"): bstack11_opy_ (u"ࠩࡤࡴࡵࡲࡩࡤࡣࡷ࡭ࡴࡴ࠯࡫ࡵࡲࡲࠬਧ"),
+      }
+  proxy = bstack1ll11ll1l_opy_(CONFIG)
+  proxies = {}
+  if CONFIG.get(bstack11_opy_ (u"ࠪ࡬ࡹࡺࡰࡑࡴࡲࡼࡾ࠭ਨ")) or CONFIG.get(bstack11_opy_ (u"ࠫ࡭ࡺࡴࡱࡵࡓࡶࡴࡾࡹࠨ਩")):
+    proxies = {
+      bstack11_opy_ (u"ࠬ࡮ࡴࡵࡲࡶࠫਪ"): proxy
+    }
+  try:
+    response = requests.get(bstack1ll11lll1_opy_, headers=headers, proxies=proxies, timeout=5)
+    if response.json():
+      bstack11l1ll1l_opy_ = response.json()[bstack11_opy_ (u"࠭ࡨࡶࡤࡶࠫਫ")]
+      logger.debug(bstack1l11lll_opy_.format(response.json()))
+      return bstack11l1ll1l_opy_
+    else:
+      logger.debug(bstack1ll11l11l_opy_.format(e))
+  except Exception as e:
+    logger.debug(bstack1ll11l11l_opy_.format(e))
+def bstack1ll1ll11_opy_(hub_url):
+  global CONFIG
+  url = bstack11_opy_ (u"ࠢࡩࡶࡷࡴࡸࡀ࠯࠰ࠤਬ")+  hub_url + bstack11_opy_ (u"ࠣ࠱ࡦ࡬ࡪࡩ࡫ࠣਭ")
+  headers = {
+        bstack11_opy_ (u"ࠩࡆࡳࡳࡺࡥ࡯ࡶ࠰ࡸࡾࡶࡥࠨਮ"): bstack11_opy_ (u"ࠪࡥࡵࡶ࡬ࡪࡥࡤࡸ࡮ࡵ࡮࠰࡬ࡶࡳࡳ࠭ਯ"),
+      }
+  proxy = bstack1ll11ll1l_opy_(CONFIG)
+  proxies = {}
+  if CONFIG.get(bstack11_opy_ (u"ࠫ࡭ࡺࡴࡱࡒࡵࡳࡽࡿࠧਰ")) or CONFIG.get(bstack11_opy_ (u"ࠬ࡮ࡴࡵࡲࡶࡔࡷࡵࡸࡺࠩ਱")):
+    proxies = {
+      bstack11_opy_ (u"࠭ࡨࡵࡶࡳࡷࠬਲ"): proxy
+    }
+  try:
+    start_time = time.perf_counter()
+    requests.get(url, headers=headers, proxies=proxies, timeout=5)
+    latency = time.perf_counter() - start_time
+    logger.debug(bstack1lllll1l_opy_.format(hub_url, latency))
+    return dict(hub_url=hub_url, latency=latency)
+  except Exception as e:
+    logger.debug(bstack11lll1l1_opy_.format(hub_url, e))
+def bstack11l11l1l_opy_():
+  try:
+    global bstack1l1ll11_opy_
+    bstack11l1ll1l_opy_ = bstack1l1lllll_opy_()
+    with Pool() as pool:
+      results = pool.map(bstack1ll1ll11_opy_, bstack11l1ll1l_opy_)
+    bstack1lll11lll_opy_ = {}
+    for item in results:
+      hub_url = item[bstack11_opy_ (u"ࠧࡩࡷࡥࡣࡺࡸ࡬ࠨਲ਼")]
+      latency = item[bstack11_opy_ (u"ࠨ࡮ࡤࡸࡪࡴࡣࡺࠩ਴")]
+      bstack1lll11lll_opy_[hub_url] = latency
+    bstack11lll1l_opy_ = min(bstack1lll11lll_opy_, key= lambda x: bstack1lll11lll_opy_[x])
+    bstack1l1ll11_opy_ = bstack11lll1l_opy_
+    logger.debug(bstack111l_opy_.format(bstack11lll1l_opy_))
+  except Exception as e:
+    logger.debug(bstack1111l1_opy_.format(e))
+bstack1111ll_opy_ = bstack11_opy_ (u"ࠩࡖࡩࡹࡺࡩ࡯ࡩࠣࡹࡵࠦࡦࡰࡴࠣࡆࡷࡵࡷࡴࡧࡵࡷࡹࡧࡣ࡬࠮ࠣࡹࡸ࡯࡮ࡨࠢࡩࡶࡦࡳࡥࡸࡱࡵ࡯࠿ࠦࡻࡾࠩਵ")
+bstack111111_opy_ = bstack11_opy_ (u"ࠪࡇࡴࡳࡰ࡭ࡧࡷࡩࡩࠦࡳࡦࡶࡸࡴࠦ࠭ਸ਼")
+bstack1ll11l111_opy_ = bstack11_opy_ (u"ࠫࡕࡧࡲࡴࡧࡧࠤࡨࡵ࡮ࡧ࡫ࡪࠤ࡫࡯࡬ࡦ࠼ࠣࡿࢂ࠭਷")
+bstack1l1l1ll11_opy_ = bstack11_opy_ (u"࡙ࠬࡡ࡯࡫ࡷ࡭ࡿ࡫ࡤࠡࡥࡲࡲ࡫࡯ࡧࠡࡨ࡬ࡰࡪࡀࠠࡼࡿࠪਸ")
+bstack1lll1111_opy_ = bstack11_opy_ (u"࠭ࡕࡴ࡫ࡱ࡫ࠥ࡮ࡵࡣࠢࡸࡶࡱࡀࠠࡼࡿࠪਹ")
+bstack111111l1_opy_ = bstack11_opy_ (u"ࠧࡔࡧࡶࡷ࡮ࡵ࡮ࠡࡵࡷࡥࡷࡺࡥࡥࠢࡺ࡭ࡹ࡮ࠠࡪࡦ࠽ࠤࢀࢃࠧ਺")
+bstack1ll1l1l1l_opy_ = bstack11_opy_ (u"ࠨࡔࡨࡧࡪ࡯ࡶࡦࡦࠣ࡭ࡳࡺࡥࡳࡴࡸࡴࡹ࠲ࠠࡦࡺ࡬ࡸ࡮ࡴࡧࠨ਻")
+bstack11l1l1l1_opy_ = bstack11_opy_ (u"ࠩࡓࡰࡪࡧࡳࡦࠢ࡬ࡲࡸࡺࡡ࡭࡮ࠣࡷࡪࡲࡥ࡯࡫ࡸࡱࠥࡺ࡯ࠡࡴࡸࡲࠥࡺࡥࡴࡶࡶ࠲ࠥࡦࡰࡪࡲࠣ࡭ࡳࡹࡴࡢ࡮࡯ࠤࡸ࡫࡬ࡦࡰ࡬ࡹࡲࡦ਼ࠧ")
+bstack111lll_opy_ = bstack11_opy_ (u"ࠪࡔࡱ࡫ࡡࡴࡧࠣ࡭ࡳࡹࡴࡢ࡮࡯ࠤࡵࡿࡴࡦࡵࡷࠤࡦࡴࡤࠡࡲࡼࡸࡪࡹࡴ࠮ࡵࡨࡰࡪࡴࡩࡶ࡯ࠣࡴࡦࡩ࡫ࡢࡩࡨࡷ࠳ࠦࡠࡱ࡫ࡳࠤ࡮ࡴࡳࡵࡣ࡯ࡰࠥࡶࡹࡵࡧࡶࡸࠥࡶࡹࡵࡧࡶࡸ࠲ࡹࡥ࡭ࡧࡱ࡭ࡺࡳࡠࠨ਽")
+bstack11l111ll_opy_ = bstack11_opy_ (u"ࠫࡕࡲࡥࡢࡵࡨࠤ࡮ࡴࡳࡵࡣ࡯ࡰࠥࡸ࡯ࡣࡱࡷ࠰ࠥࡶࡡࡣࡱࡷࠤࡦࡴࡤࠡࡵࡨࡰࡪࡴࡩࡶ࡯࡯࡭ࡧࡸࡡࡳࡻࠣࡴࡦࡩ࡫ࡢࡩࡨࡷࠥࡺ࡯ࠡࡴࡸࡲࠥࡸ࡯ࡣࡱࡷࠤࡹ࡫ࡳࡵࡵࠣ࡭ࡳࠦࡰࡢࡴࡤࡰࡱ࡫࡬࠯ࠢࡣࡴ࡮ࡶࠠࡪࡰࡶࡸࡦࡲ࡬ࠡࡴࡲࡦࡴࡺࡦࡳࡣࡰࡩࡼࡵࡲ࡬ࠢࡵࡳࡧࡵࡴࡧࡴࡤࡱࡪࡽ࡯ࡳ࡭࠰ࡴࡦࡨ࡯ࡵࠢࡵࡳࡧࡵࡴࡧࡴࡤࡱࡪࡽ࡯ࡳ࡭࠰ࡷࡪࡲࡥ࡯࡫ࡸࡱࡱ࡯ࡢࡳࡣࡵࡽࡥ࠭ਾ")
+bstack111111ll_opy_ = bstack11_opy_ (u"ࠬࡖ࡬ࡦࡣࡶࡩࠥ࡯࡮ࡴࡶࡤࡰࡱࠦࡢࡦࡪࡤࡺࡪࠦࡴࡰࠢࡵࡹࡳࠦࡴࡦࡵࡷࡷ࠳ࠦࡠࡱ࡫ࡳࠤ࡮ࡴࡳࡵࡣ࡯ࡰࠥࡨࡥࡩࡣࡹࡩࡥ࠭ਿ")
+bstack11ll1l11_opy_ = bstack11_opy_ (u"࠭ࡐ࡭ࡧࡤࡷࡪࠦࡩ࡯ࡵࡷࡥࡱࡲࠠࡢࡲࡳ࡭ࡺࡳ࠭ࡤ࡮࡬ࡩࡳࡺࠠࡵࡱࠣࡶࡺࡴࠠࡵࡧࡶࡸࡸ࠴ࠠࡡࡲ࡬ࡴࠥ࡯࡮ࡴࡶࡤࡰࡱࠦࡁࡱࡲ࡬ࡹࡲ࠳ࡐࡺࡶ࡫ࡳࡳ࠳ࡃ࡭࡫ࡨࡲࡹࡦࠧੀ")
+bstack1ll1lll11_opy_ = bstack11_opy_ (u"ࠧࡑ࡮ࡨࡥࡸ࡫ࠠࡪࡰࡶࡸࡦࡲ࡬ࠡࡲ࡯ࡥࡾࡽࡲࡪࡩ࡫ࡸࠥࡺ࡯ࠡࡴࡸࡲࠥࡺࡥࡴࡶࡶ࠲ࠥࡦࡰࡪࡲࠣ࡭ࡳࡹࡴࡢ࡮࡯ࠤࡵࡲࡡࡺࡹࡵ࡭࡬࡮ࡴࡡࠩੁ")
+bstack1l1l11ll1_opy_ = bstack11_opy_ (u"ࠨࡊࡤࡲࡩࡲࡩ࡯ࡩࠣࡷࡪࡹࡳࡪࡱࡱࠤࡨࡲ࡯ࡴࡧࠪੂ")
+bstack1l1111lll_opy_ = bstack11_opy_ (u"ࠩࡄࡰࡱࠦࡤࡰࡰࡨࠥࠬ੃")
+bstack11l11_opy_ = bstack11_opy_ (u"ࠪࡇࡴࡴࡦࡪࡩࠣࡪ࡮ࡲࡥࠡࡦࡲࡩࡸࠦ࡮ࡰࡶࠣࡩࡽ࡯ࡳࡵࠢࡤࡸࠥࡧ࡮ࡺࠢࡳࡥࡷ࡫࡮ࡵࠢࡧ࡭ࡷ࡫ࡣࡵࡱࡵࡽࠥࡵࡦࠡࠤࡾࢁࠧ࠴ࠠࡑ࡮ࡨࡥࡸ࡫ࠠࡪࡰࡦࡰࡺࡪࡥࠡࡣࠣࡦࡷࡵࡷࡴࡧࡵࡷࡹࡧࡣ࡬࠰ࡼࡱࡱ࠵ࡢࡳࡱࡺࡷࡪࡸࡳࡵࡣࡦ࡯࠳ࡿࡡ࡮࡮ࠣࡪ࡮ࡲࡥࠡࡥࡲࡲࡹࡧࡩ࡯࡫ࡱ࡫ࠥࡩ࡯࡯ࡨ࡬࡫ࡺࡸࡡࡵ࡫ࡲࡲࠥ࡬࡯ࡳࠢࡷࡩࡸࡺࡳ࠯ࠩ੄")
+bstack1l1l11_opy_ = bstack11_opy_ (u"ࠫࡇࡸ࡯ࡸࡵࡨࡶࡸࡺࡡࡤ࡭ࠣࡧࡷ࡫ࡤࡦࡰࡷ࡭ࡦࡲࡳࠡࡰࡲࡸࠥࡶࡲࡰࡸ࡬ࡨࡪࡪ࠮ࠡࡒ࡯ࡩࡦࡹࡥࠡࡣࡧࡨࠥࡺࡨࡦ࡯ࠣ࡭ࡳࠦࡢࡳࡱࡺࡷࡪࡸࡳࡵࡣࡦ࡯࠳ࡿ࡭࡭ࠢࡦࡳࡳ࡬ࡩࡨࠢࡩ࡭ࡱ࡫ࠠࡢࡵࠣࠦࡺࡹࡥࡳࡐࡤࡱࡪࠨࠠࡢࡰࡧࠤࠧࡧࡣࡤࡧࡶࡷࡐ࡫ࡹࠣࠢࡲࡶࠥࡹࡥࡵࠢࡷ࡬ࡪࡳࠠࡢࡵࠣࡩࡳࡼࡩࡳࡱࡱࡱࡪࡴࡴࠡࡸࡤࡶ࡮ࡧࡢ࡭ࡧࡶ࠾ࠥࠨࡂࡓࡑ࡚ࡗࡊࡘࡓࡕࡃࡆࡏࡤ࡛ࡓࡆࡔࡑࡅࡒࡋࠢࠡࡣࡱࡨࠥࠨࡂࡓࡑ࡚ࡗࡊࡘࡓࡕࡃࡆࡏࡤࡇࡃࡄࡇࡖࡗࡤࡑࡅ࡚ࠤࠪ੅")
+bstack11l1l11_opy_ = bstack11_opy_ (u"ࠬࡓࡡ࡭ࡨࡲࡶࡲ࡫ࡤࠡࡥࡲࡲ࡫࡯ࡧࠡࡨ࡬ࡰࡪࡀࠢࡼࡿࠥࠫ੆")
+bstack11ll1lll_opy_ = bstack11_opy_ (u"࠭ࡅ࡯ࡥࡲࡹࡳࡺࡥࡳࡧࡧࠤࡪࡸࡲࡰࡴࠣࡻ࡭࡯࡬ࡦࠢࡶࡩࡹࡺࡩ࡯ࡩࠣࡹࡵࠦ࠭ࠡࡽࢀࠫੇ")
+bstack1llllll_opy_ = bstack11_opy_ (u"ࠧࡔࡶࡤࡶࡹ࡯࡮ࡨࠢࡅࡶࡴࡽࡳࡦࡴࡶࡸࡦࡩ࡫ࠡࡎࡲࡧࡦࡲࠧੈ")
+bstack1llllll1_opy_ = bstack11_opy_ (u"ࠨࡕࡷࡳࡵࡶࡩ࡯ࡩࠣࡆࡷࡵࡷࡴࡧࡵࡷࡹࡧࡣ࡬ࠢࡏࡳࡨࡧ࡬ࠨ੉")
+bstack1lll111l1_opy_ = bstack11_opy_ (u"ࠩࡅࡶࡴࡽࡳࡦࡴࡶࡸࡦࡩ࡫ࠡࡎࡲࡧࡦࡲࠠࡪࡵࠣࡲࡴࡽࠠࡳࡷࡱࡲ࡮ࡴࡧࠢࠩ੊")
+bstack1ll11l11_opy_ = bstack11_opy_ (u"ࠪࡇࡴࡻ࡬ࡥࠢࡱࡳࡹࠦࡳࡵࡣࡵࡸࠥࡈࡲࡰࡹࡶࡩࡷࡹࡴࡢࡥ࡮ࠤࡑࡵࡣࡢ࡮࠽ࠤࢀࢃࠧੋ")
+bstack11l1lll_opy_ = bstack11_opy_ (u"ࠫࡘࡺࡡࡳࡶ࡬ࡲ࡬ࠦ࡬ࡰࡥࡤࡰࠥࡨࡩ࡯ࡣࡵࡽࠥࡽࡩࡵࡪࠣࡳࡵࡺࡩࡰࡰࡶ࠾ࠥࢁࡽࠨੌ")
+bstack1ll1lll_opy_ = bstack11_opy_ (u"࡛ࠬࡰࡥࡣࡷ࡭ࡳ࡭ࠠࡴࡧࡶࡷ࡮ࡵ࡮ࠡࡦࡨࡸࡦ࡯࡬ࡴ࠼ࠣࡿࢂ੍࠭")
+bstack11l11111_opy_ = bstack11_opy_ (u"࠭ࡅࡳࡴࡲࡶࠥ࡯࡮ࠡࡵࡨࡸࡹ࡯࡮ࡨࠢࡸࡴࡩࡧࡴࡪࡰࡪࠤࡹ࡫ࡳࡵࠢࡶࡸࡦࡺࡵࡴࠢࡾࢁࠬ੎")
+bstack111ll111_opy_ = bstack11_opy_ (u"ࠧࡑ࡮ࡨࡥࡸ࡫ࠠࡱࡴࡲࡺ࡮ࡪࡥࠡࡣࡱࠤࡦࡶࡰࡳࡱࡳࡶ࡮ࡧࡴࡦࠢࡉ࡛ࠥ࠮ࡲࡰࡤࡲࡸ࠴ࡶࡡࡣࡱࡷ࠭ࠥ࡯࡮ࠡࡥࡲࡲ࡫࡯ࡧࠡࡨ࡬ࡰࡪ࠲ࠠࡴ࡭࡬ࡴࠥࡺࡨࡦࠢࡩࡶࡦࡳࡥࡸࡱࡵ࡯ࠥࡱࡥࡺࠢ࡬ࡲࠥࡩ࡯࡯ࡨ࡬࡫ࠥ࡯ࡦࠡࡴࡸࡲࡳ࡯࡮ࡨࠢࡶ࡭ࡲࡶ࡬ࡦࠢࡳࡽࡹ࡮࡯࡯ࠢࡶࡧࡷ࡯ࡰࡵࠢࡺ࡭ࡹ࡮࡯ࡶࡶࠣࡥࡳࡿࠠࡇ࡙࠱ࠫ੏")
+bstack1llll11ll_opy_ = bstack11_opy_ (u"ࠨࡕࡨࡸࡹ࡯࡮ࡨࠢ࡫ࡸࡹࡶࡐࡳࡱࡻࡽ࠴࡮ࡴࡵࡲࡶࡔࡷࡵࡸࡺࠢ࡬ࡷࠥࡴ࡯ࡵࠢࡶࡹࡵࡶ࡯ࡳࡶࡨࡨࠥࡵ࡮ࠡࡥࡸࡶࡷ࡫࡮ࡵ࡮ࡼࠤ࡮ࡴࡳࡵࡣ࡯ࡰࡪࡪࠠࡷࡧࡵࡷ࡮ࡵ࡮ࠡࡱࡩࠤࡸ࡫࡬ࡦࡰ࡬ࡹࡲࠦࠨࡼࡿࠬ࠰ࠥࡶ࡬ࡦࡣࡶࡩࠥࡻࡰࡨࡴࡤࡨࡪࠦࡴࡰࠢࡖࡩࡱ࡫࡮ࡪࡷࡰࡂࡂ࠺࠮࠱࠰࠳ࠤࡴࡸࠠࡳࡧࡩࡩࡷࠦࡴࡰࠢ࡫ࡸࡹࡶࡳ࠻࠱࠲ࡻࡼࡽ࠮ࡣࡴࡲࡻࡸ࡫ࡲࡴࡶࡤࡧࡰ࠴ࡣࡰ࡯࠲ࡨࡴࡩࡳ࠰ࡣࡸࡸࡴࡳࡡࡵࡧ࠲ࡷࡪࡲࡥ࡯࡫ࡸࡱ࠴ࡸࡵ࡯࠯ࡷࡩࡸࡺࡳ࠮ࡤࡨ࡬࡮ࡴࡤ࠮ࡲࡵࡳࡽࡿࠣࡱࡻࡷ࡬ࡴࡴࠠࡧࡱࡵࠤࡦࠦࡷࡰࡴ࡮ࡥࡷࡵࡵ࡯ࡦ࠱ࠫ੐")
+bstack1lll111ll_opy_ = bstack11_opy_ (u"ࠩࡊࡩࡳ࡫ࡲࡢࡶ࡬ࡲ࡬ࠦࡢࡳࡱࡺࡷࡪࡸࡳࡵࡣࡦ࡯ࠥࡩ࡯࡯ࡨ࡬࡫ࡺࡸࡡࡵ࡫ࡲࡲࠥࡿ࡭࡭ࠢࡩ࡭ࡱ࡫࠮࠯ࠩੑ")
+bstack1lll1l1l1_opy_ = bstack11_opy_ (u"ࠪࡗࡺࡩࡣࡦࡵࡶࡪࡺࡲ࡬ࡺࠢࡪࡩࡳ࡫ࡲࡢࡶࡨࡨࠥࡺࡨࡦࠢࡦࡳࡳ࡬ࡩࡨࡷࡵࡥࡹ࡯࡯࡯ࠢࡩ࡭ࡱ࡫ࠡࠨ੒")
+bstack11l1llll_opy_ = bstack11_opy_ (u"ࠫࡋࡧࡩ࡭ࡧࡧࠤࡹࡵࠠࡨࡧࡱࡩࡷࡧࡴࡦࠢࡷ࡬ࡪࠦࡢࡳࡱࡺࡷࡪࡸࡳࡵࡣࡦ࡯ࠥࡩ࡯࡯ࡨ࡬࡫ࡺࡸࡡࡵ࡫ࡲࡲࠥ࡬ࡩ࡭ࡧ࠱ࠤࢀࢃࠧ੓")
+bstack1l11l1l1_opy_ = bstack11_opy_ (u"ࠬࡋࡸࡱࡧࡦࡸࡪࡪࠠࡢࡶࠣࡰࡪࡧࡳࡵࠢ࠴ࠤ࡮ࡴࡰࡶࡶ࠯ࠤࡷ࡫ࡣࡦ࡫ࡹࡩࡩࠦ࠰ࠨ੔")
+bstack11111ll1_opy_ = bstack11_opy_ (u"࠭ࡅࡳࡴࡲࡶࠥࡪࡵࡳ࡫ࡱ࡫ࠥࡇࡰࡱࠢࡸࡴࡱࡵࡡࡥ࠰ࠣࡿࢂ࠭੕")
+bstack1ll1111l_opy_ = bstack11_opy_ (u"ࠧࡇࡣ࡬ࡰࡪࡪࠠࡵࡱࠣࡹࡵࡲ࡯ࡢࡦࠣࡅࡵࡶ࠮ࠡࡋࡱࡺࡦࡲࡩࡥࠢࡩ࡭ࡱ࡫ࠠࡱࡣࡷ࡬ࠥࡶࡲࡰࡸ࡬ࡨࡪࡪࠠࡼࡿ࠱ࠫ੖")
+bstack11l1l11l_opy_ = bstack11_opy_ (u"ࠨࡍࡨࡽࡸࠦࡣࡢࡰࡱࡳࡹࠦࡣࡰ࠯ࡨࡼ࡮ࡹࡴࠡࡣࡶࠤࡦࡶࡰࠡࡸࡤࡰࡺ࡫ࡳ࠭ࠢࡸࡷࡪࠦࡡ࡯ࡻࠣࡳࡳ࡫ࠠࡱࡴࡲࡴࡪࡸࡴࡺࠢࡩࡶࡴࡳࠠࡼ࡫ࡧࡀࡸࡺࡲࡪࡰࡪࡂ࠱ࠦࡰࡢࡶ࡫ࡀࡸࡺࡲࡪࡰࡪࡂ࠱ࠦࡣࡶࡵࡷࡳࡲࡥࡩࡥ࠾ࡶࡸࡷ࡯࡮ࡨࡀ࠯ࠤࡸ࡮ࡡࡳࡧࡤࡦࡱ࡫࡟ࡪࡦ࠿ࡷࡹࡸࡩ࡯ࡩࡁࢁ࠱ࠦ࡯࡯࡮ࡼࠤࠧࡶࡡࡵࡪࠥࠤࡦࡴࡤࠡࠤࡦࡹࡸࡺ࡯࡮ࡡ࡬ࡨࠧࠦࡣࡢࡰࠣࡧࡴ࠳ࡥࡹ࡫ࡶࡸࠥࡺ࡯ࡨࡧࡷ࡬ࡪࡸ࠮ࠨ੗")
+bstack11ll1_opy_ = bstack11_opy_ (u"ࠩ࡞ࡍࡳࡼࡡ࡭࡫ࡧࠤࡦࡶࡰࠡࡲࡵࡳࡵ࡫ࡲࡵࡻࡠࠤࡸࡻࡰࡱࡱࡵࡸࡪࡪࠠࡱࡴࡲࡴࡪࡸࡴࡪࡧࡶࠤࡦࡸࡥࠡࡽ࡬ࡨࡁࡹࡴࡳ࡫ࡱ࡫ࡃ࠲ࠠࡱࡣࡷ࡬ࡁࡹࡴࡳ࡫ࡱ࡫ࡃ࠲ࠠࡤࡷࡶࡸࡴࡳ࡟ࡪࡦ࠿ࡷࡹࡸࡩ࡯ࡩࡁ࠰ࠥࡹࡨࡢࡴࡨࡥࡧࡲࡥࡠ࡫ࡧࡀࡸࡺࡲࡪࡰࡪࡂࢂ࠴ࠠࡇࡱࡵࠤࡲࡵࡲࡦࠢࡧࡩࡹࡧࡩ࡭ࡵࠣࡴࡱ࡫ࡡࡴࡧࠣࡺ࡮ࡹࡩࡵࠢ࡫ࡸࡹࡶࡳ࠻࠱࠲ࡻࡼࡽ࠮ࡣࡴࡲࡻࡸ࡫ࡲࡴࡶࡤࡧࡰ࠴ࡣࡰ࡯࠲ࡨࡴࡩࡳ࠰ࡣࡳࡴ࠲ࡧࡵࡵࡱࡰࡥࡹ࡫࠯ࡢࡲࡳ࡭ࡺࡳ࠯ࡴࡧࡷ࠱ࡺࡶ࠭ࡵࡧࡶࡸࡸ࠵ࡳࡱࡧࡦ࡭࡫ࡿ࠭ࡢࡲࡳࠫ੘")
+bstack11l1ll_opy_ = bstack11_opy_ (u"ࠪ࡟ࡎࡴࡶࡢ࡮࡬ࡨࠥࡧࡰࡱࠢࡳࡶࡴࡶࡥࡳࡶࡼࡡ࡙ࠥࡵࡱࡲࡲࡶࡹ࡫ࡤࠡࡸࡤࡰࡺ࡫ࡳࠡࡱࡩࠤࡦࡶࡰࠡࡣࡵࡩࠥࡵࡦࠡࡽ࡬ࡨࡁࡹࡴࡳ࡫ࡱ࡫ࡃ࠲ࠠࡱࡣࡷ࡬ࡁࡹࡴࡳ࡫ࡱ࡫ࡃ࠲ࠠࡤࡷࡶࡸࡴࡳ࡟ࡪࡦ࠿ࡷࡹࡸࡩ࡯ࡩࡁ࠰ࠥࡹࡨࡢࡴࡨࡥࡧࡲࡥࡠ࡫ࡧࡀࡸࡺࡲࡪࡰࡪࡂࢂ࠴ࠠࡇࡱࡵࠤࡲࡵࡲࡦࠢࡧࡩࡹࡧࡩ࡭ࡵࠣࡴࡱ࡫ࡡࡴࡧࠣࡺ࡮ࡹࡩࡵࠢ࡫ࡸࡹࡶࡳ࠻࠱࠲ࡻࡼࡽ࠮ࡣࡴࡲࡻࡸ࡫ࡲࡴࡶࡤࡧࡰ࠴ࡣࡰ࡯࠲ࡨࡴࡩࡳ࠰ࡣࡳࡴ࠲ࡧࡵࡵࡱࡰࡥࡹ࡫࠯ࡢࡲࡳ࡭ࡺࡳ࠯ࡴࡧࡷ࠱ࡺࡶ࠭ࡵࡧࡶࡸࡸ࠵ࡳࡱࡧࡦ࡭࡫ࡿ࠭ࡢࡲࡳࠫਖ਼")
+bstack1l1ll11ll_opy_ = bstack11_opy_ (u"࡚ࠫࡹࡩ࡯ࡩࠣࡩࡽ࡯ࡳࡵ࡫ࡱ࡫ࠥࡧࡰࡱࠢ࡬ࡨࠥࢁࡽࠡࡨࡲࡶࠥ࡮ࡡࡴࡪࠣ࠾ࠥࢁࡽ࠯ࠩਗ਼")
+bstack1l1l1lll1_opy_ = bstack11_opy_ (u"ࠬࡇࡰࡱࠢࡘࡴࡱࡵࡡࡥࡧࡧࠤࡘࡻࡣࡤࡧࡶࡷ࡫ࡻ࡬࡭ࡻ࠱ࠤࡎࡊࠠ࠻ࠢࡾࢁࠬਜ਼")
+bstack1ll1ll111_opy_ = bstack11_opy_ (u"࠭ࡕࡴ࡫ࡱ࡫ࠥࡇࡰࡱࠢ࠽ࠤࢀࢃ࠮ࠨੜ")
+bstack1l111l1l_opy_ = bstack11_opy_ (u"ࠧࡱࡣࡵࡥࡱࡲࡥ࡭ࡵࡓࡩࡷࡖ࡬ࡢࡶࡩࡳࡷࡳࠠࡪࡵࠣࡲࡴࡺࠠࡴࡷࡳࡴࡴࡸࡴࡦࡦࠣࡪࡴࡸࠠࡷࡣࡱ࡭ࡱࡲࡡࠡࡲࡼࡸ࡭ࡵ࡮ࠡࡶࡨࡷࡹࡹࠬࠡࡴࡸࡲࡳ࡯࡮ࡨࠢࡺ࡭ࡹ࡮ࠠࡱࡣࡵࡥࡱࡲࡥ࡭ࡒࡨࡶࡕࡲࡡࡵࡨࡲࡶࡲࠦ࠽ࠡ࠳ࠪ੝")
+bstack1l1ll1l1_opy_ = bstack11_opy_ (u"ࠨࡇࡵࡶࡴࡸࠠࡪࡰࠣࡧࡷ࡫ࡡࡵ࡫ࡱ࡫ࠥࡨࡵࡪ࡮ࡧࡍࡩ࡫࡮ࡵ࡫ࡩ࡭ࡪࡸ࠺ࠡࡽࢀࠫਫ਼")
+bstack1ll1lll1_opy_ = bstack11_opy_ (u"ࠩࡆࡳࡺࡲࡤࠡࡰࡲࡸࠥࡩ࡬ࡰࡵࡨࠤࡧࡸ࡯ࡸࡵࡨࡶ࠿ࠦࡻࡾࠩ੟")
+bstack1l1l1ll_opy_ = bstack11_opy_ (u"ࠪࡇࡴࡻ࡬ࡥࠢࡱࡳࡹࠦࡧࡦࡶࠣࡶࡪࡧࡳࡰࡰࠣࡪࡴࡸࠠࡣࡧ࡫ࡥࡻ࡫ࠠࡧࡧࡤࡸࡺࡸࡥࠡࡨࡤ࡭ࡱࡻࡲࡦ࠰ࠣࡿࢂ࠭੠")
+bstack1llll1_opy_ = bstack11_opy_ (u"ࠫࡊࡸࡲࡰࡴࠣࡻ࡭࡯࡬ࡦࠢࡪࡩࡹࡺࡩ࡯ࡩࠣࡶࡪࡹࡰࡰࡰࡶࡩࠥ࡬ࡲࡰ࡯ࠣࡥࡵ࡯ࠠࡤࡣ࡯ࡰ࠳ࠦࡅࡳࡴࡲࡶ࠿ࠦࡻࡾࠩ੡")
+bstack1l111lll1_opy_ = bstack11_opy_ (u"࡛ࠬ࡮ࡢࡤ࡯ࡩࠥࡺ࡯ࠡࡵ࡫ࡳࡼࠦࡢࡶ࡫࡯ࡨ࡛ࠥࡒࡍ࠮ࠣࡥࡸࠦࡢࡶ࡫࡯ࡨࠥࡩࡡࡱࡣࡥ࡭ࡱ࡯ࡴࡺࠢ࡬ࡷࠥࡴ࡯ࡵࠢࡸࡷࡪࡪ࠮ࠨ੢")
+bstack111111l_opy_ = bstack11_opy_ (u"࠭ࡓࡦࡴࡹࡩࡷࠦࡳࡪࡦࡨࠤࡧࡻࡩ࡭ࡦࡑࡥࡲ࡫ࠨࡼࡿࠬࠤ࡮ࡹࠠ࡯ࡱࡷࠤࡸࡧ࡭ࡦࠢࡤࡷࠥࡩ࡬ࡪࡧࡱࡸࠥࡹࡩࡥࡧࠣࡦࡺ࡯࡬ࡥࡐࡤࡱࡪ࠮ࡻࡾࠫࠪ੣")
+bstack11l11l_opy_ = bstack11_opy_ (u"ࠧࡗ࡫ࡨࡻࠥࡨࡵࡪ࡮ࡧࠤࡴࡴࠠࡃࡴࡲࡻࡸ࡫ࡲࡔࡶࡤࡧࡰࠦࡤࡢࡵ࡫ࡦࡴࡧࡲࡥ࠼ࠣࡿࢂ࠭੤")
+bstack1lll11ll1_opy_ = bstack11_opy_ (u"ࠨࡗࡱࡥࡧࡲࡥࠡࡶࡲࠤࡦࡩࡣࡦࡵࡶࠤࡦࠦࡰࡳ࡫ࡹࡥࡹ࡫ࠠࡥࡱࡰࡥ࡮ࡴ࠺ࠡࡽࢀࠤ࠳ࠦࡓࡦࡶࠣࡸ࡭࡫ࠠࡧࡱ࡯ࡰࡴࡽࡩ࡯ࡩࠣࡧࡴࡴࡦࡪࡩࠣ࡭ࡳࠦࡹࡰࡷࡵࠤࡧࡸ࡯ࡸࡵࡨࡶࡸࡺࡡࡤ࡭࠱ࡽࡲࡲࠠࡧ࡫࡯ࡩ࠿ࠦ࡜࡯࠯࠰࠱࠲࠳࠭࠮࠯࠰࠱࠲ࠦ࡜࡯ࠢࡥࡶࡴࡽࡳࡦࡴࡶࡸࡦࡩ࡫ࡍࡱࡦࡥࡱࡀࠠࡵࡴࡸࡩࠥࡢ࡮࠮࠯࠰࠱࠲࠳࠭࠮࠯࠰࠱ࠬ੥")
+bstack1l1l11l1_opy_ = bstack11_opy_ (u"ࠩࡖࡳࡲ࡫ࡴࡩ࡫ࡱ࡫ࠥࡽࡥ࡯ࡶࠣࡻࡷࡵ࡮ࡨࠢࡺ࡬࡮ࡲࡥࠡࡧࡻࡩࡨࡻࡴࡪࡰࡪࠤ࡬࡫ࡴࡠࡰࡸࡨ࡬࡫࡟࡭ࡱࡦࡥࡱࡥࡥࡳࡴࡲࡶࠥࡀࠠࡼࡿࠪ੦")
+bstack1l1llllll_opy_ = bstack11_opy_ (u"ࠥࡉࡷࡸ࡯ࡳࠢ࡬ࡲࠥࡹࡥ࡯ࡦࡢࡥࡲࡶ࡬ࡪࡶࡸࡨࡪࡥࡥࡷࡧࡱࡸࠥ࡬࡯ࡳࠢࡖࡈࡐ࡙ࡥࡵࡷࡳࠤࢀࢃࠢ੧")
+bstack1l11l111l_opy_ = bstack11_opy_ (u"ࠦࡊࡸࡲࡰࡴࠣ࡭ࡳࠦࡳࡦࡰࡧࡣࡦࡳࡰ࡭࡫ࡷࡹࡩ࡫࡟ࡦࡸࡨࡲࡹࠦࡦࡰࡴࠣࡗࡉࡑࡔࡦࡵࡷࡅࡹࡺࡥ࡮ࡲࡷࡩࡩࠦࡻࡾࠤ੨")
+bstack11111l1l_opy_ = bstack11_opy_ (u"ࠧࡋࡲࡳࡱࡵࠤ࡮ࡴࠠࡴࡧࡱࡨࡤࡧ࡭ࡱ࡮࡬ࡸࡺࡪࡥࡠࡧࡹࡩࡳࡺࠠࡧࡱࡵࠤࡘࡊࡋࡕࡧࡶࡸࡘࡻࡣࡤࡧࡶࡷ࡫ࡻ࡬ࠡࡽࢀࠦ੩")
+bstack11ll11ll_opy_ = bstack11_opy_ (u"ࠨࡅࡳࡴࡲࡶࠥ࡯࡮ࠡࡨ࡬ࡶࡪࡥࡲࡦࡳࡸࡩࡸࡺࠠࡼࡿࠥ੪")
+bstack1lll1l1ll_opy_ = bstack11_opy_ (u"ࠢࡑࡑࡖࡘࠥࡋࡶࡦࡰࡷࠤࢀࢃࠠࡳࡧࡶࡴࡴࡴࡳࡦࠢ࠽ࠤࢀࢃࠢ੫")
+bstack11ll11_opy_ = bstack11_opy_ (u"ࠨࡈࡤ࡭ࡱ࡫ࡤࠡࡶࡲࠤࡨࡵ࡮ࡧ࡫ࡪࡹࡷ࡫ࠠࡱࡴࡲࡼࡾࠦࡳࡦࡶࡷ࡭ࡳ࡭ࡳ࠭ࠢࡨࡶࡷࡵࡲ࠻ࠢࡾࢁࠬ੬")
+bstack1l11lll_opy_ = bstack11_opy_ (u"ࠩࡕࡩࡸࡶ࡯࡯ࡵࡨࠤ࡫ࡸ࡯࡮ࠢ࠲ࡲࡪࡾࡴࡠࡪࡸࡦࡸࠦࡻࡾࠩ੭")
+bstack1ll11l11l_opy_ = bstack11_opy_ (u"ࠪࡉࡷࡸ࡯ࡳࠢ࡬ࡲࠥ࡭ࡥࡵࡶ࡬ࡲ࡬ࠦࡲࡦࡵࡳࡳࡳࡹࡥࠡࡨࡵࡳࡲࠦ࠯࡯ࡧࡻࡸࡤ࡮ࡵࡣࡵ࠽ࠤࢀࢃࠧ੮")
+bstack111l_opy_ = bstack11_opy_ (u"ࠫࡓ࡫ࡡࡳࡧࡶࡸࠥ࡮ࡵࡣࠢࡤࡰࡱࡵࡣࡢࡶࡨࡨࠥ࡯ࡳ࠻ࠢࡾࢁࠬ੯")
+bstack1lllll_opy_ = bstack11_opy_ (u"ࠬࡋࡒࡓࡑࡕࠤࡎࡔࠠࡂࡎࡏࡓࡈࡇࡔࡆࠢࡋ࡙ࡇࠦࡻࡾࠩੰ")
+bstack1lllll1l_opy_ = bstack11_opy_ (u"࠭ࡌࡢࡶࡨࡲࡨࡿࠠࡰࡨࠣ࡬ࡺࡨ࠺ࠡࡽࢀࠤ࡮ࡹ࠺ࠡࡽࢀࠫੱ")
+bstack11lll1l1_opy_ = bstack11_opy_ (u"ࠧࡆࡴࡵࡳࡷࠦࡩ࡯ࠢࡪࡩࡹࡺࡩ࡯ࡩࠣࡰࡦࡺࡥ࡯ࡥࡼࠤ࡫ࡵࡲࠡࡽࢀࠤ࡭ࡻࡢ࠻ࠢࡾࢁࠬੲ")
+bstack1l1l1ll1l_opy_ = bstack11_opy_ (u"ࠨࡊࡸࡦࠥࡻࡲ࡭ࠢࡦ࡬ࡦࡴࡧࡦࡦࠣࡸࡴࠦࡴࡩࡧࠣࡳࡵࡺࡩ࡮ࡣ࡯ࠤ࡭ࡻࡢ࠻ࠢࡾࢁࠬੳ")
+bstack1l11l11l_opy_ = bstack11_opy_ (u"ࠩࡈࡶࡷࡵࡲࠡࡹ࡫࡭ࡱ࡫ࠠࡴࡧࡷࡸ࡮ࡴࡧࠡࡶ࡫ࡩࠥࡵࡰࡵ࡫ࡰࡥࡱࠦࡨࡶࡤࠣࡹࡷࡲ࠺ࠡࡽࢀࠫੴ")
+bstack111llll_opy_ = bstack11_opy_ (u"ࠪࠤࠥ࠵ࠪࠡ࠿ࡀࡁࡂࡃ࠽࠾࠿ࡀࡁࡂࡃ࠽࠾࠿ࡀࡁࡂࡃ࠽࠾࠿ࡀࡁࡂࡃ࠽࠾࠿ࡀࡁࡂࡃ࠽࠾࠿ࡀࡁࡂࡃ࠽࠾࠿ࡀࡁࡂࡃ࠽࠾࠿ࡀࡁࡂࡃ࠽࠾࠿ࡀࡁࡂࡃ࠽࠾࠿ࡀࡁࡂࡃ࠽࠾࠿ࡀࡁࡂࡃ࠽࠾࠿ࡀࡁࡂࡃ࠽࠾࠿ࡀࡁࡂࡃ࠽࠾࠿ࡀࡁࡂࡃ࠽࠾࠿ࡀࡁࡂࡃ࠽࠾࠿ࡀࡁࡂࡃ࠽࠾࠿ࡀࡁࡂࡃ࠽࠾࠿ࡀࡁࠥ࠰࠯࡝ࡰࠣࠤ࡮࡬ࠨࡱࡣࡪࡩࠥࡃ࠽࠾ࠢࡹࡳ࡮ࡪࠠ࠱ࠫࠣࡿࡡࡴࠠࠡࠢࡷࡶࡾࢁ࡜࡯ࠢࡦࡳࡳࡹࡴࠡࡨࡶࠤࡂࠦࡲࡦࡳࡸ࡭ࡷ࡫ࠨ࡝ࠩࡩࡷࡡ࠭ࠩ࠼࡞ࡱࠤࠥࠦࠠࠡࡨࡶ࠲ࡦࡶࡰࡦࡰࡧࡊ࡮ࡲࡥࡔࡻࡱࡧ࠭ࡨࡳࡵࡣࡦ࡯ࡤࡶࡡࡵࡪ࠯ࠤࡏ࡙ࡏࡏ࠰ࡶࡸࡷ࡯࡮ࡨ࡫ࡩࡽ࠭ࡶ࡟ࡪࡰࡧࡩࡽ࠯ࠠࠬࠢࠥ࠾ࠧࠦࠫࠡࡌࡖࡓࡓ࠴ࡳࡵࡴ࡬ࡲ࡬࡯ࡦࡺࠪࡍࡗࡔࡔ࠮ࡱࡣࡵࡷࡪ࠮ࠨࡢࡹࡤ࡭ࡹࠦ࡮ࡦࡹࡓࡥ࡬࡫࠲࠯ࡧࡹࡥࡱࡻࡡࡵࡧࠫࠦ࠭࠯ࠠ࠾ࡀࠣࡿࢂࠨࠬࠡ࡞ࠪࡦࡷࡵࡷࡴࡧࡵࡷࡹࡧࡣ࡬ࡡࡨࡼࡪࡩࡵࡵࡱࡵ࠾ࠥࢁࠢࡢࡥࡷ࡭ࡴࡴࠢ࠻ࠢࠥ࡫ࡪࡺࡓࡦࡵࡶ࡭ࡴࡴࡄࡦࡶࡤ࡭ࡱࡹࠢࡾ࡞ࠪ࠭࠮࠯࡛ࠣࡪࡤࡷ࡭࡫ࡤࡠ࡫ࡧࠦࡢ࠯ࠠࠬࠢࠥ࠰ࡡࡢ࡮ࠣࠫ࡟ࡲࠥࠦࠠࠡࡿࡦࡥࡹࡩࡨࠩࡧࡻ࠭ࢀࡢ࡮ࠡࠢࠣࠤࢂࡢ࡮ࠡࠢࢀࡠࡳࠦࠠ࠰ࠬࠣࡁࡂࡃ࠽࠾࠿ࡀࡁࡂࡃ࠽࠾࠿ࡀࡁࡂࡃ࠽࠾࠿ࡀࡁࡂࡃ࠽࠾࠿ࡀࡁࡂࡃ࠽࠾࠿ࡀࡁࡂࡃ࠽࠾࠿ࡀࡁࡂࡃ࠽࠾࠿ࡀࡁࡂࡃ࠽࠾࠿ࡀࡁࡂࡃ࠽࠾࠿ࡀࡁࡂࡃ࠽࠾࠿ࡀࡁࡂࡃ࠽࠾࠿ࡀࡁࡂࡃ࠽࠾࠿ࡀࡁࡂࡃ࠽࠾࠿ࡀࡁࡂࡃ࠽࠾࠿ࡀࡁࡂࡃ࠽࠾࠿ࡀࡁࡂࡃ࠽࠾࠿ࡀࡁࡂࡃ࠽࠾࠿ࡀࡁࡂࡃࠠࠫ࠱ࠪੵ")
+bstack1lll1l11l_opy_ = bstack11_opy_ (u"ࠫࡡࡴ࠯ࠫࠢࡀࡁࡂࡃ࠽࠾࠿ࡀࡁࡂࡃ࠽࠾࠿ࡀࡁࡂࡃ࠽࠾࠿ࡀࡁࡂࡃ࠽࠾࠿ࡀࡁࡂࡃ࠽࠾࠿ࡀࡁࡂࡃ࠽࠾࠿ࡀࡁࡂࡃ࠽࠾࠿ࡀࡁࡂࡃ࠽࠾࠿ࡀࡁࡂࡃ࠽࠾࠿ࡀࡁࡂࡃ࠽࠾࠿ࡀࡁࡂࡃ࠽࠾࠿ࡀࡁࡂࡃ࠽࠾࠿ࡀࡁࡂࡃ࠽࠾࠿ࡀࡁࡂࡃ࠽࠾࠿ࡀࡁࡂࡃ࠽࠾࠿ࡀࡁࡂࡃ࠽࠾࠿ࡀࡁࡂࡃ࠽࠾࠿ࡀࡁࡂࠦࠪ࠰࡞ࡱࡧࡴࡴࡳࡵࠢࡥࡷࡹࡧࡣ࡬ࡡࡳࡥࡹ࡮ࠠ࠾ࠢࡳࡶࡴࡩࡥࡴࡵ࠱ࡥࡷ࡭ࡶ࡜ࡲࡵࡳࡨ࡫ࡳࡴ࠰ࡤࡶ࡬ࡼ࠮࡭ࡧࡱ࡫ࡹ࡮ࠠ࠮ࠢ࠶ࡡࡡࡴࡣࡰࡰࡶࡸࠥࡨࡳࡵࡣࡦ࡯ࡤࡩࡡࡱࡵࠣࡁࠥࡶࡲࡰࡥࡨࡷࡸ࠴ࡡࡳࡩࡹ࡟ࡵࡸ࡯ࡤࡧࡶࡷ࠳ࡧࡲࡨࡸ࠱ࡰࡪࡴࡧࡵࡪࠣ࠱ࠥ࠷࡝࡝ࡰࡦࡳࡳࡹࡴࠡࡲࡢ࡭ࡳࡪࡥࡹࠢࡀࠤࡵࡸ࡯ࡤࡧࡶࡷ࠳ࡧࡲࡨࡸ࡞ࡴࡷࡵࡣࡦࡵࡶ࠲ࡦࡸࡧࡷ࠰࡯ࡩࡳ࡭ࡴࡩࠢ࠰ࠤ࠷ࡣ࡜࡯ࡲࡵࡳࡨ࡫ࡳࡴ࠰ࡤࡶ࡬ࡼࠠ࠾ࠢࡳࡶࡴࡩࡥࡴࡵ࠱ࡥࡷ࡭ࡶ࠯ࡵ࡯࡭ࡨ࡫ࠨ࠱࠮ࠣࡴࡷࡵࡣࡦࡵࡶ࠲ࡦࡸࡧࡷ࠰࡯ࡩࡳ࡭ࡴࡩࠢ࠰ࠤ࠸࠯࡜࡯ࡥࡲࡲࡸࡺࠠࡪ࡯ࡳࡳࡷࡺ࡟ࡱ࡮ࡤࡽࡼࡸࡩࡨࡪࡷ࠸ࡤࡨࡳࡵࡣࡦ࡯ࠥࡃࠠࡳࡧࡴࡹ࡮ࡸࡥࠩࠤࡳࡰࡦࡿࡷࡳ࡫ࡪ࡬ࡹࠨࠩ࠼࡞ࡱ࡭ࡲࡶ࡯ࡳࡶࡢࡴࡱࡧࡹࡸࡴ࡬࡫࡭ࡺ࠴ࡠࡤࡶࡸࡦࡩ࡫࠯ࡥ࡫ࡶࡴࡳࡩࡶ࡯࠱ࡰࡦࡻ࡮ࡤࡪࠣࡁࠥࡧࡳࡺࡰࡦࠤ࠭ࡲࡡࡶࡰࡦ࡬ࡔࡶࡴࡪࡱࡱࡷ࠮ࠦ࠽࠿ࠢࡾࡠࡳࡲࡥࡵࠢࡦࡥࡵࡹ࠻࡝ࡰࡷࡶࡾࠦࡻ࡝ࡰࡦࡥࡵࡹࠠ࠾ࠢࡍࡗࡔࡔ࠮ࡱࡣࡵࡷࡪ࠮ࡢࡴࡶࡤࡧࡰࡥࡣࡢࡲࡶ࠭ࡡࡴࠠࠡࡿࠣࡧࡦࡺࡣࡩࠪࡨࡼ࠮ࠦࡻ࡝ࡰࠣࠤࠥࠦࡽ࡝ࡰࠣࠤࡷ࡫ࡴࡶࡴࡱࠤࡦࡽࡡࡪࡶࠣ࡭ࡲࡶ࡯ࡳࡶࡢࡴࡱࡧࡹࡸࡴ࡬࡫࡭ࡺ࠴ࡠࡤࡶࡸࡦࡩ࡫࠯ࡥ࡫ࡶࡴࡳࡩࡶ࡯࠱ࡧࡴࡴ࡮ࡦࡥࡷࠬࢀࡢ࡮ࠡࠢࠣࠤࡼࡹࡅ࡯ࡦࡳࡳ࡮ࡴࡴ࠻ࠢࡣࡻࡸࡹ࠺࠰࠱ࡦࡨࡵ࠴ࡢࡳࡱࡺࡷࡪࡸࡳࡵࡣࡦ࡯࠳ࡩ࡯࡮࠱ࡳࡰࡦࡿࡷࡳ࡫ࡪ࡬ࡹࡅࡣࡢࡲࡶࡁࠩࢁࡥ࡯ࡥࡲࡨࡪ࡛ࡒࡊࡅࡲࡱࡵࡵ࡮ࡦࡰࡷࠬࡏ࡙ࡏࡏ࠰ࡶࡸࡷ࡯࡮ࡨ࡫ࡩࡽ࠭ࡩࡡࡱࡵࠬ࠭ࢂࡦࠬ࡝ࡰࠣࠤࠥࠦ࠮࠯࠰࡯ࡥࡺࡴࡣࡩࡑࡳࡸ࡮ࡵ࡮ࡴ࡞ࡱࠤࠥࢃࠩ࡝ࡰࢀࡠࡳ࠵ࠪࠡ࠿ࡀࡁࡂࡃ࠽࠾࠿ࡀࡁࡂࡃ࠽࠾࠿ࡀࡁࡂࡃ࠽࠾࠿ࡀࡁࡂࡃ࠽࠾࠿ࡀࡁࡂࡃ࠽࠾࠿ࡀࡁࡂࡃ࠽࠾࠿ࡀࡁࡂࡃ࠽࠾࠿ࡀࡁࡂࡃ࠽࠾࠿ࡀࡁࡂࡃ࠽࠾࠿ࡀࡁࡂࡃ࠽࠾࠿ࡀࡁࡂࡃ࠽࠾࠿ࡀࡁࡂࡃ࠽࠾࠿ࡀࡁࡂࡃ࠽࠾࠿ࡀࡁࡂࡃ࠽࠾࠿ࡀࡁࡂࡃ࠽࠾࠿ࡀࡁࡂࡃ࠽࠾࠿ࡀࡁࡂࡃ࠽࠾࠿ࡀࡁࠥ࠰࠯࡝ࡰࠪ੶")
 from ._version import __version__
-bstack11llll11_opy_ = None
+bstack111ll11_opy_ = None
 CONFIG = {}
-bstack1111l1l_opy_ = {}
-bstack1lll1111l_opy_ = {}
-bstack1111111_opy_ = None
-bstack111lll_opy_ = None
-bstack1ll111ll_opy_ = None
-bstack1111ll_opy_ = -1
-bstack1ll1lll1_opy_ = DEFAULT_LOG_LEVEL
-bstack1llll1_opy_ = 1
-bstack1l1ll1l_opy_ = False
-bstack1l1l1l11_opy_ = bstack1ll1_opy_ (u"ࠩࠪ੟")
-bstack111l1lll_opy_ = bstack1ll1_opy_ (u"ࠪࠫ੠")
-bstack1ll11111l_opy_ = False
-bstack111lllll_opy_ = True
-bstack11l1l11l_opy_ = bstack1ll1_opy_ (u"ࠫࠬ੡")
-bstack111l_opy_ = []
-bstack1lll1_opy_ = None
-bstack1ll1l11l_opy_ = None
-bstack1111l11l_opy_ = None
-bstack11l11ll1_opy_ = None
-bstack1ll111_opy_ = None
-bstack1111l1ll_opy_ = None
-bstack1ll11111_opy_ = None
-bstack111lll1l_opy_ = None
-bstack1ll1l1ll1_opy_ = None
-bstack1l1lll_opy_ = None
-bstack1lll1l_opy_ = None
-bstack11ll1l1l_opy_ = None
-bstack1l1ll_opy_ = bstack1ll1_opy_ (u"ࠧࠨ੢")
-class bstack11lll1ll_opy_(threading.Thread):
+bstack1lll1lll_opy_ = {}
+bstack1l111_opy_ = {}
+bstack1l1lll1ll_opy_ = None
+bstack1l1l1lll_opy_ = None
+bstack1ll1l11_opy_ = None
+bstack1l111l11l_opy_ = -1
+bstack1ll1l111l_opy_ = DEFAULT_LOG_LEVEL
+bstack1l11ll1ll_opy_ = 1
+bstack1l11llll_opy_ = False
+bstack1l1lll1l_opy_ = bstack11_opy_ (u"ࠬ࠭੷")
+bstack1l11l111_opy_ = bstack11_opy_ (u"࠭ࠧ੸")
+bstack1llll1l_opy_ = False
+bstack11llll11_opy_ = True
+bstack11llll1l_opy_ = bstack11_opy_ (u"ࠧࠨ੹")
+bstack1ll1l1l1_opy_ = []
+bstack1l1ll11_opy_ = bstack11_opy_ (u"ࠨࠩ੺")
+bstack1ll1l11ll_opy_ = None
+bstack11111ll_opy_ = None
+bstack1lll1ll1_opy_ = None
+bstack11ll_opy_ = None
+bstack1l11ll1_opy_ = None
+bstack11ll1l_opy_ = None
+bstack1111ll11_opy_ = None
+bstack111ll_opy_ = None
+bstack1lll1llll_opy_ = None
+bstack1lllll11_opy_ = None
+bstack1ll1ll1ll_opy_ = None
+bstack1l11lll11_opy_ = None
+bstack11l1l1_opy_ = bstack11_opy_ (u"ࠤࠥ੻")
+class bstack11l1l1ll_opy_(threading.Thread):
   def run(self):
     self.exc = None
     try:
       self.ret = self._target(*self._args, **self._kwargs)
     except Exception as e:
       self.exc = e
   def join(self, timeout=None):
-    super(bstack11lll1ll_opy_, self).join(timeout)
+    super(bstack11l1l1ll_opy_, self).join(timeout)
     if self.exc:
       raise self.exc
     return self.ret
 logger = logging.getLogger(__name__)
-logging.basicConfig(level=bstack1ll1lll1_opy_,
-                    format=bstack1ll1_opy_ (u"࠭࡜࡯ࠧࠫࡥࡸࡩࡴࡪ࡯ࡨ࠭ࡸ࡛ࠦࠦࠪࡱࡥࡲ࡫ࠩࡴ࡟࡞ࠩ࠭ࡲࡥࡷࡧ࡯ࡲࡦࡳࡥࠪࡵࡠࠤ࠲ࠦࠥࠩ࡯ࡨࡷࡸࡧࡧࡦࠫࡶࠫ੣"),
-                    datefmt=bstack1ll1_opy_ (u"ࠧࠦࡊ࠽ࠩࡒࡀࠥࡔࠩ੤"))
-def bstack11l111ll_opy_():
-  global CONFIG
-  global bstack1ll1lll1_opy_
-  if bstack1ll1_opy_ (u"ࠨ࡮ࡲ࡫ࡑ࡫ࡶࡦ࡮ࠪ੥") in CONFIG:
-    bstack1ll1lll1_opy_ = bstack1ll1l1_opy_[CONFIG[bstack1ll1_opy_ (u"ࠩ࡯ࡳ࡬ࡒࡥࡷࡧ࡯ࠫ੦")]]
-    logging.getLogger().setLevel(bstack1ll1lll1_opy_)
-def bstack1lllll1_opy_():
+logging.basicConfig(level=bstack1ll1l111l_opy_,
+                    format=bstack11_opy_ (u"ࠪࡠࡳࠫࠨࡢࡵࡦࡸ࡮ࡳࡥࠪࡵࠣ࡟ࠪ࠮࡮ࡢ࡯ࡨ࠭ࡸࡣ࡛ࠦࠪ࡯ࡩࡻ࡫࡬࡯ࡣࡰࡩ࠮ࡹ࡝ࠡ࠯ࠣࠩ࠭ࡳࡥࡴࡵࡤ࡫ࡪ࠯ࡳࠨ੼"),
+                    datefmt=bstack11_opy_ (u"ࠫࠪࡎ࠺ࠦࡏ࠽ࠩࡘ࠭੽"))
+def bstack1l1l1111_opy_():
+  global CONFIG
+  global bstack1ll1l111l_opy_
+  if bstack11_opy_ (u"ࠬࡲ࡯ࡨࡎࡨࡺࡪࡲࠧ੾") in CONFIG:
+    bstack1ll1l111l_opy_ = bstack1l1ll_opy_[CONFIG[bstack11_opy_ (u"࠭࡬ࡰࡩࡏࡩࡻ࡫࡬ࠨ੿")]]
+    logging.getLogger().setLevel(bstack1ll1l111l_opy_)
+def bstack1l111ll1l_opy_():
   from appium.version import version as appium_version
   return version.parse(appium_version)
-def bstack1ll1llll_opy_():
+def bstack1ll11l1ll_opy_():
   from selenium import webdriver
   return version.parse(webdriver.__version__)
-def bstack1ll1ll111_opy_():
+def bstack1ll1l1lll_opy_():
   args = sys.argv
   for i in range(len(args)):
-    if bstack1ll1_opy_ (u"ࠥ࠱࠲ࡨࡲࡰࡹࡶࡩࡷࡹࡴࡢࡥ࡮ࡧࡴࡴࡦࡪࡩࡩ࡭ࡱ࡫ࠢ੧") == args[i].lower() or bstack1ll1_opy_ (u"ࠦ࠲࠳ࡢࡳࡱࡺࡷࡪࡸࡳࡵࡣࡦ࡯࠳ࡩ࡯࡯ࡨ࡬࡫ࠧ੨") == args[i].lower():
+    if bstack11_opy_ (u"ࠢ࠮࠯ࡥࡶࡴࡽࡳࡦࡴࡶࡸࡦࡩ࡫ࡤࡱࡱࡪ࡮࡭ࡦࡪ࡮ࡨࠦ઀") == args[i].lower() or bstack11_opy_ (u"ࠣ࠯࠰ࡦࡷࡵࡷࡴࡧࡵࡷࡹࡧࡣ࡬࠰ࡦࡳࡳ࡬ࡩࡨࠤઁ") == args[i].lower():
       path = args[i+1]
       sys.argv.remove(args[i])
       sys.argv.remove(path)
-      global bstack11l1l11l_opy_
-      bstack11l1l11l_opy_ += bstack1ll1_opy_ (u"ࠬ࠳࠭ࡣࡴࡲࡻࡸ࡫ࡲࡴࡶࡤࡧࡰࡉ࡯࡯ࡨ࡬࡫ࡋ࡯࡬ࡦࠢࠪ੩") + path
+      global bstack11llll1l_opy_
+      bstack11llll1l_opy_ += bstack11_opy_ (u"ࠩ࠰࠱ࡧࡸ࡯ࡸࡵࡨࡶࡸࡺࡡࡤ࡭ࡆࡳࡳ࡬ࡩࡨࡈ࡬ࡰࡪࠦࠧં") + path
       return path
   return None
-def bstack1l1ll1ll_opy_():
-  bstack111llll_opy_ = bstack1ll1ll111_opy_()
-  if bstack111llll_opy_ and os.path.exists(os.path.abspath(bstack111llll_opy_)):
-    fileName = bstack111llll_opy_
-  if bstack1ll1_opy_ (u"࠭ࡂࡓࡑ࡚ࡗࡊࡘࡓࡕࡃࡆࡏࡤࡉࡏࡏࡈࡌࡋࡤࡌࡉࡍࡇࠪ੪") in os.environ and os.path.exists(os.path.abspath(os.environ[bstack1ll1_opy_ (u"ࠧࡃࡔࡒ࡛ࡘࡋࡒࡔࡖࡄࡇࡐࡥࡃࡐࡐࡉࡍࡌࡥࡆࡊࡎࡈࠫ੫")])) and not bstack1ll1_opy_ (u"ࠨࡨ࡬ࡰࡪࡔࡡ࡮ࡧࠪ੬") in locals():
-    fileName = os.environ[bstack1ll1_opy_ (u"ࠩࡅࡖࡔ࡝ࡓࡆࡔࡖࡘࡆࡉࡋࡠࡅࡒࡒࡋࡏࡇࡠࡈࡌࡐࡊ࠭੭")]
-  if bstack1ll1_opy_ (u"ࠪࡪ࡮ࡲࡥࡏࡣࡰࡩࠬ੮") in locals():
-    bstack1l11_opy_ = os.path.abspath(fileName)
+def bstack1lll111l_opy_():
+  bstack1l1ll11l_opy_ = bstack1ll1l1lll_opy_()
+  if bstack1l1ll11l_opy_ and os.path.exists(os.path.abspath(bstack1l1ll11l_opy_)):
+    fileName = bstack1l1ll11l_opy_
+  if bstack11_opy_ (u"ࠪࡆࡗࡕࡗࡔࡇࡕࡗ࡙ࡇࡃࡌࡡࡆࡓࡓࡌࡉࡈࡡࡉࡍࡑࡋࠧઃ") in os.environ and os.path.exists(os.path.abspath(os.environ[bstack11_opy_ (u"ࠫࡇࡘࡏࡘࡕࡈࡖࡘ࡚ࡁࡄࡍࡢࡇࡔࡔࡆࡊࡉࡢࡊࡎࡒࡅࠨ઄")])) and not bstack11_opy_ (u"ࠬ࡬ࡩ࡭ࡧࡑࡥࡲ࡫ࠧઅ") in locals():
+    fileName = os.environ[bstack11_opy_ (u"࠭ࡂࡓࡑ࡚ࡗࡊࡘࡓࡕࡃࡆࡏࡤࡉࡏࡏࡈࡌࡋࡤࡌࡉࡍࡇࠪઆ")]
+  if bstack11_opy_ (u"ࠧࡧ࡫࡯ࡩࡓࡧ࡭ࡦࠩઇ") in locals():
+    bstack1l1111ll_opy_ = os.path.abspath(fileName)
   else:
-    bstack1l11_opy_ = bstack1ll1_opy_ (u"ࠫࠬ੯")
-  bstack1ll1l1l11_opy_ = os.getcwd()
-  bstack1ll11l1_opy_ = bstack1ll1_opy_ (u"ࠬࡨࡲࡰࡹࡶࡩࡷࡹࡴࡢࡥ࡮࠲ࡾࡳ࡬ࠨੰ")
-  bstack1l1l111_opy_ = bstack1ll1_opy_ (u"࠭ࡢࡳࡱࡺࡷࡪࡸࡳࡵࡣࡦ࡯࠳ࡿࡡ࡮࡮ࠪੱ")
-  while (not os.path.exists(bstack1l11_opy_)) and bstack1ll1l1l11_opy_ != bstack1ll1_opy_ (u"ࠢࠣੲ"):
-    bstack1l11_opy_ = os.path.join(bstack1ll1l1l11_opy_, bstack1ll11l1_opy_)
-    if not os.path.exists(bstack1l11_opy_):
-      bstack1l11_opy_ = os.path.join(bstack1ll1l1l11_opy_, bstack1l1l111_opy_)
-    if bstack1ll1l1l11_opy_ != os.path.dirname(bstack1ll1l1l11_opy_):
-      bstack1ll1l1l11_opy_ = os.path.dirname(bstack1ll1l1l11_opy_)
-    else:
-      bstack1ll1l1l11_opy_ = bstack1ll1_opy_ (u"ࠣࠤੳ")
-  if not os.path.exists(bstack1l11_opy_):
-    bstack1ll1lll_opy_(
-      bstack1lllll_opy_.format(os.getcwd()))
-  with open(bstack1l11_opy_, bstack1ll1_opy_ (u"ࠩࡵࠫੴ")) as stream:
+    bstack1l1111ll_opy_ = bstack11_opy_ (u"ࠨࠩઈ")
+  bstack1lll1ll1l_opy_ = os.getcwd()
+  bstack1l11111ll_opy_ = bstack11_opy_ (u"ࠩࡥࡶࡴࡽࡳࡦࡴࡶࡸࡦࡩ࡫࠯ࡻࡰࡰࠬઉ")
+  bstack1111111l_opy_ = bstack11_opy_ (u"ࠪࡦࡷࡵࡷࡴࡧࡵࡷࡹࡧࡣ࡬࠰ࡼࡥࡲࡲࠧઊ")
+  while (not os.path.exists(bstack1l1111ll_opy_)) and bstack1lll1ll1l_opy_ != bstack11_opy_ (u"ࠦࠧઋ"):
+    bstack1l1111ll_opy_ = os.path.join(bstack1lll1ll1l_opy_, bstack1l11111ll_opy_)
+    if not os.path.exists(bstack1l1111ll_opy_):
+      bstack1l1111ll_opy_ = os.path.join(bstack1lll1ll1l_opy_, bstack1111111l_opy_)
+    if bstack1lll1ll1l_opy_ != os.path.dirname(bstack1lll1ll1l_opy_):
+      bstack1lll1ll1l_opy_ = os.path.dirname(bstack1lll1ll1l_opy_)
+    else:
+      bstack1lll1ll1l_opy_ = bstack11_opy_ (u"ࠧࠨઌ")
+  if not os.path.exists(bstack1l1111ll_opy_):
+    bstack11111l11_opy_(
+      bstack11l11_opy_.format(os.getcwd()))
+  with open(bstack1l1111ll_opy_, bstack11_opy_ (u"࠭ࡲࠨઍ")) as stream:
     try:
       config = yaml.safe_load(stream)
       return config
     except yaml.YAMLError as exc:
-      bstack1ll1lll_opy_(bstack1ll11ll11_opy_.format(str(exc)))
-def bstack11ll1lll_opy_(config):
-  bstack1ll1ll1_opy_ = bstack1ll11l11l_opy_(config)
-  for option in list(bstack1ll1ll1_opy_):
-    if option.lower() in bstack1ll111l1l_opy_ and option != bstack1ll111l1l_opy_[option.lower()]:
-      bstack1ll1ll1_opy_[bstack1ll111l1l_opy_[option.lower()]] = bstack1ll1ll1_opy_[option]
-      del bstack1ll1ll1_opy_[option]
+      bstack11111l11_opy_(bstack11l1l11_opy_.format(str(exc)))
+def bstack1lll1l11_opy_(config):
+  bstack1l1llll1l_opy_ = bstack111lll11_opy_(config)
+  for option in list(bstack1l1llll1l_opy_):
+    if option.lower() in bstack1l111l1l1_opy_ and option != bstack1l111l1l1_opy_[option.lower()]:
+      bstack1l1llll1l_opy_[bstack1l111l1l1_opy_[option.lower()]] = bstack1l1llll1l_opy_[option]
+      del bstack1l1llll1l_opy_[option]
   return config
-def bstack1lll1ll1_opy_():
-  global bstack1lll1111l_opy_
-  for key, bstack1111lll1_opy_ in bstack1l111l_opy_.items():
-    if isinstance(bstack1111lll1_opy_, list):
-      for var in bstack1111lll1_opy_:
+def bstack111l11ll_opy_():
+  global bstack1l111_opy_
+  for key, bstack1lll1l1l_opy_ in bstack1ll111ll_opy_.items():
+    if isinstance(bstack1lll1l1l_opy_, list):
+      for var in bstack1lll1l1l_opy_:
         if var in os.environ:
-          bstack1lll1111l_opy_[key] = os.environ[var]
+          bstack1l111_opy_[key] = os.environ[var]
           break
-    elif bstack1111lll1_opy_ in os.environ:
-      bstack1lll1111l_opy_[key] = os.environ[bstack1111lll1_opy_]
-  if bstack1ll1_opy_ (u"ࠪࡆࡗࡕࡗࡔࡇࡕࡗ࡙ࡇࡃࡌࡡࡏࡓࡈࡇࡌࡠࡋࡇࡉࡓ࡚ࡉࡇࡋࡈࡖࠬੵ") in os.environ:
-    bstack1lll1111l_opy_[bstack1ll1_opy_ (u"ࠫࡧࡸ࡯ࡸࡵࡨࡶࡘࡺࡡࡤ࡭ࡏࡳࡨࡧ࡬ࡐࡲࡷ࡭ࡴࡴࡳࠨ੶")] = {}
-    bstack1lll1111l_opy_[bstack1ll1_opy_ (u"ࠬࡨࡲࡰࡹࡶࡩࡷ࡙ࡴࡢࡥ࡮ࡐࡴࡩࡡ࡭ࡑࡳࡸ࡮ࡵ࡮ࡴࠩ੷")][bstack1ll1_opy_ (u"࠭࡬ࡰࡥࡤࡰࡎࡪࡥ࡯ࡶ࡬ࡪ࡮࡫ࡲࠨ੸")] = os.environ[bstack1ll1_opy_ (u"ࠧࡃࡔࡒ࡛ࡘࡋࡒࡔࡖࡄࡇࡐࡥࡌࡐࡅࡄࡐࡤࡏࡄࡆࡐࡗࡍࡋࡏࡅࡓࠩ੹")]
-def bstack1l11l_opy_():
-  global bstack1111l1l_opy_
-  global bstack11l1l11l_opy_
+    elif bstack1lll1l1l_opy_ in os.environ:
+      bstack1l111_opy_[key] = os.environ[bstack1lll1l1l_opy_]
+  if bstack11_opy_ (u"ࠧࡃࡔࡒ࡛ࡘࡋࡒࡔࡖࡄࡇࡐࡥࡌࡐࡅࡄࡐࡤࡏࡄࡆࡐࡗࡍࡋࡏࡅࡓࠩ઎") in os.environ:
+    bstack1l111_opy_[bstack11_opy_ (u"ࠨࡤࡵࡳࡼࡹࡥࡳࡕࡷࡥࡨࡱࡌࡰࡥࡤࡰࡔࡶࡴࡪࡱࡱࡷࠬએ")] = {}
+    bstack1l111_opy_[bstack11_opy_ (u"ࠩࡥࡶࡴࡽࡳࡦࡴࡖࡸࡦࡩ࡫ࡍࡱࡦࡥࡱࡕࡰࡵ࡫ࡲࡲࡸ࠭ઐ")][bstack11_opy_ (u"ࠪࡰࡴࡩࡡ࡭ࡋࡧࡩࡳࡺࡩࡧ࡫ࡨࡶࠬઑ")] = os.environ[bstack11_opy_ (u"ࠫࡇࡘࡏࡘࡕࡈࡖࡘ࡚ࡁࡄࡍࡢࡐࡔࡉࡁࡍࡡࡌࡈࡊࡔࡔࡊࡈࡌࡉࡗ࠭઒")]
+def bstack1l11l11_opy_():
+  global bstack1lll1lll_opy_
+  global bstack11llll1l_opy_
   for idx, val in enumerate(sys.argv):
-    if idx<len(sys.argv) and bstack1ll1_opy_ (u"ࠨ࠯࠰ࡦࡷࡵࡷࡴࡧࡵࡷࡹࡧࡣ࡬࠰࡯ࡳࡨࡧ࡬ࡊࡦࡨࡲࡹ࡯ࡦࡪࡧࡵࠫ੺").lower() == val.lower():
-      bstack1111l1l_opy_[bstack1ll1_opy_ (u"ࠩࡥࡶࡴࡽࡳࡦࡴࡖࡸࡦࡩ࡫ࡍࡱࡦࡥࡱࡕࡰࡵ࡫ࡲࡲࡸ࠭੻")] = {}
-      bstack1111l1l_opy_[bstack1ll1_opy_ (u"ࠪࡦࡷࡵࡷࡴࡧࡵࡗࡹࡧࡣ࡬ࡎࡲࡧࡦࡲࡏࡱࡶ࡬ࡳࡳࡹࠧ੼")][bstack1ll1_opy_ (u"ࠫࡱࡵࡣࡢ࡮ࡌࡨࡪࡴࡴࡪࡨ࡬ࡩࡷ࠭੽")] = sys.argv[idx+1]
+    if idx<len(sys.argv) and bstack11_opy_ (u"ࠬ࠳࠭ࡣࡴࡲࡻࡸ࡫ࡲࡴࡶࡤࡧࡰ࠴࡬ࡰࡥࡤࡰࡎࡪࡥ࡯ࡶ࡬ࡪ࡮࡫ࡲࠨઓ").lower() == val.lower():
+      bstack1lll1lll_opy_[bstack11_opy_ (u"࠭ࡢࡳࡱࡺࡷࡪࡸࡓࡵࡣࡦ࡯ࡑࡵࡣࡢ࡮ࡒࡴࡹ࡯࡯࡯ࡵࠪઔ")] = {}
+      bstack1lll1lll_opy_[bstack11_opy_ (u"ࠧࡣࡴࡲࡻࡸ࡫ࡲࡔࡶࡤࡧࡰࡒ࡯ࡤࡣ࡯ࡓࡵࡺࡩࡰࡰࡶࠫક")][bstack11_opy_ (u"ࠨ࡮ࡲࡧࡦࡲࡉࡥࡧࡱࡸ࡮࡬ࡩࡦࡴࠪખ")] = sys.argv[idx+1]
       del sys.argv[idx:idx+2]
       break
-  for key, bstack1lll111l_opy_ in bstack11l11lll_opy_.items():
-    if isinstance(bstack1lll111l_opy_, list):
+  for key, bstack1l11l1l1l_opy_ in bstack1ll111111_opy_.items():
+    if isinstance(bstack1l11l1l1l_opy_, list):
       for idx, val in enumerate(sys.argv):
-        for var in bstack1lll111l_opy_:
-          if idx<len(sys.argv) and bstack1ll1_opy_ (u"ࠬ࠳࠭ࠨ੾") + var.lower() == val.lower() and not key in bstack1111l1l_opy_:
-            bstack1111l1l_opy_[key] = sys.argv[idx+1]
-            bstack11l1l11l_opy_ += bstack1ll1_opy_ (u"࠭ࠠ࠮࠯ࠪ੿") + var + bstack1ll1_opy_ (u"ࠧࠡࠩ઀") + sys.argv[idx+1]
+        for var in bstack1l11l1l1l_opy_:
+          if idx<len(sys.argv) and bstack11_opy_ (u"ࠩ࠰࠱ࠬગ") + var.lower() == val.lower() and not key in bstack1lll1lll_opy_:
+            bstack1lll1lll_opy_[key] = sys.argv[idx+1]
+            bstack11llll1l_opy_ += bstack11_opy_ (u"ࠪࠤ࠲࠳ࠧઘ") + var + bstack11_opy_ (u"ࠫࠥ࠭ઙ") + sys.argv[idx+1]
             del sys.argv[idx:idx+2]
             break
     else:
       for idx, val in enumerate(sys.argv):
-        if idx<len(sys.argv) and bstack1ll1_opy_ (u"ࠨ࠯࠰ࠫઁ") + bstack1lll111l_opy_.lower() == val.lower() and not key in bstack1111l1l_opy_:
-          bstack1111l1l_opy_[key] = sys.argv[idx+1]
-          bstack11l1l11l_opy_ += bstack1ll1_opy_ (u"ࠩࠣ࠱࠲࠭ં") + bstack1lll111l_opy_ + bstack1ll1_opy_ (u"ࠪࠤࠬઃ") + sys.argv[idx+1]
+        if idx<len(sys.argv) and bstack11_opy_ (u"ࠬ࠳࠭ࠨચ") + bstack1l11l1l1l_opy_.lower() == val.lower() and not key in bstack1lll1lll_opy_:
+          bstack1lll1lll_opy_[key] = sys.argv[idx+1]
+          bstack11llll1l_opy_ += bstack11_opy_ (u"࠭ࠠ࠮࠯ࠪછ") + bstack1l11l1l1l_opy_ + bstack11_opy_ (u"ࠧࠡࠩજ") + sys.argv[idx+1]
           del sys.argv[idx:idx+2]
-def bstack1ll11lll_opy_(config):
-  bstack1l11111_opy_ = config.keys()
-  for bstack11l1111l_opy_, bstack1l1l111ll_opy_ in bstack111l11l_opy_.items():
-    if bstack1l1l111ll_opy_ in bstack1l11111_opy_:
-      config[bstack11l1111l_opy_] = config[bstack1l1l111ll_opy_]
-      del config[bstack1l1l111ll_opy_]
-  for bstack11l1111l_opy_, bstack1l1l111ll_opy_ in bstack1l1ll1111_opy_.items():
-    if isinstance(bstack1l1l111ll_opy_, list):
-      for bstack1lllll1l1_opy_ in bstack1l1l111ll_opy_:
-        if bstack1lllll1l1_opy_ in bstack1l11111_opy_:
-          config[bstack11l1111l_opy_] = config[bstack1lllll1l1_opy_]
-          del config[bstack1lllll1l1_opy_]
+def bstack11lllll1_opy_(config):
+  bstack1lll1lll1_opy_ = config.keys()
+  for bstack1l1111ll1_opy_, bstack1l1111l1_opy_ in bstack1l1ll11l1_opy_.items():
+    if bstack1l1111l1_opy_ in bstack1lll1lll1_opy_:
+      config[bstack1l1111ll1_opy_] = config[bstack1l1111l1_opy_]
+      del config[bstack1l1111l1_opy_]
+  for bstack1l1111ll1_opy_, bstack1l1111l1_opy_ in bstack1ll111l1l_opy_.items():
+    if isinstance(bstack1l1111l1_opy_, list):
+      for bstack1llll1ll1_opy_ in bstack1l1111l1_opy_:
+        if bstack1llll1ll1_opy_ in bstack1lll1lll1_opy_:
+          config[bstack1l1111ll1_opy_] = config[bstack1llll1ll1_opy_]
+          del config[bstack1llll1ll1_opy_]
           break
-    elif bstack1l1l111ll_opy_ in bstack1l11111_opy_:
-        config[bstack11l1111l_opy_] = config[bstack1l1l111ll_opy_]
-        del config[bstack1l1l111ll_opy_]
-  for bstack1lllll1l1_opy_ in list(config):
-    for bstack1l1lllll_opy_ in bstack11111l1l_opy_:
-      if bstack1lllll1l1_opy_.lower() == bstack1l1lllll_opy_.lower() and bstack1lllll1l1_opy_ != bstack1l1lllll_opy_:
-        config[bstack1l1lllll_opy_] = config[bstack1lllll1l1_opy_]
-        del config[bstack1lllll1l1_opy_]
-  bstack1l1l1l11l_opy_ = []
-  if bstack1ll1_opy_ (u"ࠫࡵࡲࡡࡵࡨࡲࡶࡲࡹࠧ઄") in config:
-    bstack1l1l1l11l_opy_ = config[bstack1ll1_opy_ (u"ࠬࡶ࡬ࡢࡶࡩࡳࡷࡳࡳࠨઅ")]
-  for platform in bstack1l1l1l11l_opy_:
-    for bstack1lllll1l1_opy_ in list(platform):
-      for bstack1l1lllll_opy_ in bstack11111l1l_opy_:
-        if bstack1lllll1l1_opy_.lower() == bstack1l1lllll_opy_.lower() and bstack1lllll1l1_opy_ != bstack1l1lllll_opy_:
-          platform[bstack1l1lllll_opy_] = platform[bstack1lllll1l1_opy_]
-          del platform[bstack1lllll1l1_opy_]
-  for bstack11l1111l_opy_, bstack1l1l111ll_opy_ in bstack1l1ll1111_opy_.items():
-    for platform in bstack1l1l1l11l_opy_:
-      if isinstance(bstack1l1l111ll_opy_, list):
-        for bstack1lllll1l1_opy_ in bstack1l1l111ll_opy_:
-          if bstack1lllll1l1_opy_ in platform:
-            platform[bstack11l1111l_opy_] = platform[bstack1lllll1l1_opy_]
-            del platform[bstack1lllll1l1_opy_]
+    elif bstack1l1111l1_opy_ in bstack1lll1lll1_opy_:
+        config[bstack1l1111ll1_opy_] = config[bstack1l1111l1_opy_]
+        del config[bstack1l1111l1_opy_]
+  for bstack1llll1ll1_opy_ in list(config):
+    for bstack1ll11l_opy_ in bstack11l11lll_opy_:
+      if bstack1llll1ll1_opy_.lower() == bstack1ll11l_opy_.lower() and bstack1llll1ll1_opy_ != bstack1ll11l_opy_:
+        config[bstack1ll11l_opy_] = config[bstack1llll1ll1_opy_]
+        del config[bstack1llll1ll1_opy_]
+  bstack1l11l11ll_opy_ = []
+  if bstack11_opy_ (u"ࠨࡲ࡯ࡥࡹ࡬࡯ࡳ࡯ࡶࠫઝ") in config:
+    bstack1l11l11ll_opy_ = config[bstack11_opy_ (u"ࠩࡳࡰࡦࡺࡦࡰࡴࡰࡷࠬઞ")]
+  for platform in bstack1l11l11ll_opy_:
+    for bstack1llll1ll1_opy_ in list(platform):
+      for bstack1ll11l_opy_ in bstack11l11lll_opy_:
+        if bstack1llll1ll1_opy_.lower() == bstack1ll11l_opy_.lower() and bstack1llll1ll1_opy_ != bstack1ll11l_opy_:
+          platform[bstack1ll11l_opy_] = platform[bstack1llll1ll1_opy_]
+          del platform[bstack1llll1ll1_opy_]
+  for bstack1l1111ll1_opy_, bstack1l1111l1_opy_ in bstack1ll111l1l_opy_.items():
+    for platform in bstack1l11l11ll_opy_:
+      if isinstance(bstack1l1111l1_opy_, list):
+        for bstack1llll1ll1_opy_ in bstack1l1111l1_opy_:
+          if bstack1llll1ll1_opy_ in platform:
+            platform[bstack1l1111ll1_opy_] = platform[bstack1llll1ll1_opy_]
+            del platform[bstack1llll1ll1_opy_]
             break
-      elif bstack1l1l111ll_opy_ in platform:
-        platform[bstack11l1111l_opy_] = platform[bstack1l1l111ll_opy_]
-        del platform[bstack1l1l111ll_opy_]
-  for bstack1lll11lll_opy_ in bstack11l1ll11_opy_:
-    if bstack1lll11lll_opy_ in config:
-      if not bstack11l1ll11_opy_[bstack1lll11lll_opy_] in config:
-        config[bstack11l1ll11_opy_[bstack1lll11lll_opy_]] = {}
-      config[bstack11l1ll11_opy_[bstack1lll11lll_opy_]].update(config[bstack1lll11lll_opy_])
-      del config[bstack1lll11lll_opy_]
-  for platform in bstack1l1l1l11l_opy_:
-    for bstack1lll11lll_opy_ in bstack11l1ll11_opy_:
-      if bstack1lll11lll_opy_ in list(platform):
-        if not bstack11l1ll11_opy_[bstack1lll11lll_opy_] in platform:
-          platform[bstack11l1ll11_opy_[bstack1lll11lll_opy_]] = {}
-        platform[bstack11l1ll11_opy_[bstack1lll11lll_opy_]].update(platform[bstack1lll11lll_opy_])
-        del platform[bstack1lll11lll_opy_]
-  config = bstack11ll1lll_opy_(config)
+      elif bstack1l1111l1_opy_ in platform:
+        platform[bstack1l1111ll1_opy_] = platform[bstack1l1111l1_opy_]
+        del platform[bstack1l1111l1_opy_]
+  for bstack111l1ll1_opy_ in bstack1ll111l1_opy_:
+    if bstack111l1ll1_opy_ in config:
+      if not bstack1ll111l1_opy_[bstack111l1ll1_opy_] in config:
+        config[bstack1ll111l1_opy_[bstack111l1ll1_opy_]] = {}
+      config[bstack1ll111l1_opy_[bstack111l1ll1_opy_]].update(config[bstack111l1ll1_opy_])
+      del config[bstack111l1ll1_opy_]
+  for platform in bstack1l11l11ll_opy_:
+    for bstack111l1ll1_opy_ in bstack1ll111l1_opy_:
+      if bstack111l1ll1_opy_ in list(platform):
+        if not bstack1ll111l1_opy_[bstack111l1ll1_opy_] in platform:
+          platform[bstack1ll111l1_opy_[bstack111l1ll1_opy_]] = {}
+        platform[bstack1ll111l1_opy_[bstack111l1ll1_opy_]].update(platform[bstack111l1ll1_opy_])
+        del platform[bstack111l1ll1_opy_]
+  config = bstack1lll1l11_opy_(config)
   return config
-def bstack1ll111lll_opy_(config):
-  global bstack111l1lll_opy_
-  if bstack1ll1_opy_ (u"࠭ࡢࡳࡱࡺࡷࡪࡸࡳࡵࡣࡦ࡯ࡑࡵࡣࡢ࡮ࠪઆ") in config and str(config[bstack1ll1_opy_ (u"ࠧࡣࡴࡲࡻࡸ࡫ࡲࡴࡶࡤࡧࡰࡒ࡯ࡤࡣ࡯ࠫઇ")]).lower() != bstack1ll1_opy_ (u"ࠨࡨࡤࡰࡸ࡫ࠧઈ"):
-    if not bstack1ll1_opy_ (u"ࠩࡥࡶࡴࡽࡳࡦࡴࡖࡸࡦࡩ࡫ࡍࡱࡦࡥࡱࡕࡰࡵ࡫ࡲࡲࡸ࠭ઉ") in config:
-      config[bstack1ll1_opy_ (u"ࠪࡦࡷࡵࡷࡴࡧࡵࡗࡹࡧࡣ࡬ࡎࡲࡧࡦࡲࡏࡱࡶ࡬ࡳࡳࡹࠧઊ")] = {}
-    if not bstack1ll1_opy_ (u"ࠫࡱࡵࡣࡢ࡮ࡌࡨࡪࡴࡴࡪࡨ࡬ࡩࡷ࠭ઋ") in config[bstack1ll1_opy_ (u"ࠬࡨࡲࡰࡹࡶࡩࡷ࡙ࡴࡢࡥ࡮ࡐࡴࡩࡡ࡭ࡑࡳࡸ࡮ࡵ࡮ࡴࠩઌ")]:
-      bstack1lll11l1l_opy_ = datetime.datetime.now()
-      bstack1lll11l11_opy_ = bstack1lll11l1l_opy_.strftime(bstack1ll1_opy_ (u"࠭ࠥࡥࡡࠨࡦࡤࠫࡈࠦࡏࠪઍ"))
+def bstack1l11ll1l_opy_(config):
+  global bstack1l11l111_opy_
+  if bstack11_opy_ (u"ࠪࡦࡷࡵࡷࡴࡧࡵࡷࡹࡧࡣ࡬ࡎࡲࡧࡦࡲࠧટ") in config and str(config[bstack11_opy_ (u"ࠫࡧࡸ࡯ࡸࡵࡨࡶࡸࡺࡡࡤ࡭ࡏࡳࡨࡧ࡬ࠨઠ")]).lower() != bstack11_opy_ (u"ࠬ࡬ࡡ࡭ࡵࡨࠫડ"):
+    if not bstack11_opy_ (u"࠭ࡢࡳࡱࡺࡷࡪࡸࡓࡵࡣࡦ࡯ࡑࡵࡣࡢ࡮ࡒࡴࡹ࡯࡯࡯ࡵࠪઢ") in config:
+      config[bstack11_opy_ (u"ࠧࡣࡴࡲࡻࡸ࡫ࡲࡔࡶࡤࡧࡰࡒ࡯ࡤࡣ࡯ࡓࡵࡺࡩࡰࡰࡶࠫણ")] = {}
+    if not bstack11_opy_ (u"ࠨ࡮ࡲࡧࡦࡲࡉࡥࡧࡱࡸ࡮࡬ࡩࡦࡴࠪત") in config[bstack11_opy_ (u"ࠩࡥࡶࡴࡽࡳࡦࡴࡖࡸࡦࡩ࡫ࡍࡱࡦࡥࡱࡕࡰࡵ࡫ࡲࡲࡸ࠭થ")]:
+      bstack1lll11ll_opy_ = datetime.datetime.now()
+      bstack11l11l11_opy_ = bstack1lll11ll_opy_.strftime(bstack11_opy_ (u"ࠪࠩࡩࡥࠥࡣࡡࠨࡌࠪࡓࠧદ"))
       hostname = socket.gethostname()
-      bstack1ll11_opy_ = bstack1ll1_opy_ (u"ࠧࠨ઎").join(random.choices(string.ascii_lowercase + string.digits, k=4))
-      identifier = bstack1ll1_opy_ (u"ࠨࡽࢀࡣࢀࢃ࡟ࡼࡿࠪએ").format(bstack1lll11l11_opy_, hostname, bstack1ll11_opy_)
-      config[bstack1ll1_opy_ (u"ࠩࡥࡶࡴࡽࡳࡦࡴࡖࡸࡦࡩ࡫ࡍࡱࡦࡥࡱࡕࡰࡵ࡫ࡲࡲࡸ࠭ઐ")][bstack1ll1_opy_ (u"ࠪࡰࡴࡩࡡ࡭ࡋࡧࡩࡳࡺࡩࡧ࡫ࡨࡶࠬઑ")] = identifier
-    bstack111l1lll_opy_ = config[bstack1ll1_opy_ (u"ࠫࡧࡸ࡯ࡸࡵࡨࡶࡘࡺࡡࡤ࡭ࡏࡳࡨࡧ࡬ࡐࡲࡷ࡭ࡴࡴࡳࠨ઒")][bstack1ll1_opy_ (u"ࠬࡲ࡯ࡤࡣ࡯ࡍࡩ࡫࡮ࡵ࡫ࡩ࡭ࡪࡸࠧઓ")]
+      bstack1ll111_opy_ = bstack11_opy_ (u"ࠫࠬધ").join(random.choices(string.ascii_lowercase + string.digits, k=4))
+      identifier = bstack11_opy_ (u"ࠬࢁࡽࡠࡽࢀࡣࢀࢃࠧન").format(bstack11l11l11_opy_, hostname, bstack1ll111_opy_)
+      config[bstack11_opy_ (u"࠭ࡢࡳࡱࡺࡷࡪࡸࡓࡵࡣࡦ࡯ࡑࡵࡣࡢ࡮ࡒࡴࡹ࡯࡯࡯ࡵࠪ઩")][bstack11_opy_ (u"ࠧ࡭ࡱࡦࡥࡱࡏࡤࡦࡰࡷ࡭࡫࡯ࡥࡳࠩપ")] = identifier
+    bstack1l11l111_opy_ = config[bstack11_opy_ (u"ࠨࡤࡵࡳࡼࡹࡥࡳࡕࡷࡥࡨࡱࡌࡰࡥࡤࡰࡔࡶࡴࡪࡱࡱࡷࠬફ")][bstack11_opy_ (u"ࠩ࡯ࡳࡨࡧ࡬ࡊࡦࡨࡲࡹ࡯ࡦࡪࡧࡵࠫબ")]
   return config
-def bstack1lll1l11_opy_():
+def bstack11111_opy_():
   if (
-    isinstance(os.getenv(bstack1ll1_opy_ (u"࠭ࡊࡆࡐࡎࡍࡓ࡙࡟ࡖࡔࡏࠫઔ")), str) and len(os.getenv(bstack1ll1_opy_ (u"ࠧࡋࡇࡑࡏࡎࡔࡓࡠࡗࡕࡐࠬક"))) > 0
+    isinstance(os.getenv(bstack11_opy_ (u"ࠪࡎࡊࡔࡋࡊࡐࡖࡣ࡚ࡘࡌࠨભ")), str) and len(os.getenv(bstack11_opy_ (u"ࠫࡏࡋࡎࡌࡋࡑࡗࡤ࡛ࡒࡍࠩમ"))) > 0
   ) or (
-    isinstance(os.getenv(bstack1ll1_opy_ (u"ࠨࡌࡈࡒࡐࡏࡎࡔࡡࡋࡓࡒࡋࠧખ")), str) and len(os.getenv(bstack1ll1_opy_ (u"ࠩࡍࡉࡓࡑࡉࡏࡕࡢࡌࡔࡓࡅࠨગ"))) > 0
+    isinstance(os.getenv(bstack11_opy_ (u"ࠬࡐࡅࡏࡍࡌࡒࡘࡥࡈࡐࡏࡈࠫય")), str) and len(os.getenv(bstack11_opy_ (u"࠭ࡊࡆࡐࡎࡍࡓ࡙࡟ࡉࡑࡐࡉࠬર"))) > 0
   ):
-    return os.getenv(bstack1ll1_opy_ (u"ࠪࡆ࡚ࡏࡌࡅࡡࡑ࡙ࡒࡈࡅࡓࠩઘ"), 0)
-  if str(os.getenv(bstack1ll1_opy_ (u"ࠫࡈࡏࠧઙ"))).lower() == bstack1ll1_opy_ (u"ࠬࡺࡲࡶࡧࠪચ") and str(os.getenv(bstack1ll1_opy_ (u"࠭ࡃࡊࡔࡆࡐࡊࡉࡉࠨછ"))).lower() == bstack1ll1_opy_ (u"ࠧࡵࡴࡸࡩࠬજ"):
-    return os.getenv(bstack1ll1_opy_ (u"ࠨࡅࡌࡖࡈࡒࡅࡠࡄࡘࡍࡑࡊ࡟ࡏࡗࡐࠫઝ"), 0)
-  if str(os.getenv(bstack1ll1_opy_ (u"ࠩࡆࡍࠬઞ"))).lower() == bstack1ll1_opy_ (u"ࠪࡸࡷࡻࡥࠨટ") and str(os.getenv(bstack1ll1_opy_ (u"࡙ࠫࡘࡁࡗࡋࡖࠫઠ"))).lower() == bstack1ll1_opy_ (u"ࠬࡺࡲࡶࡧࠪડ"):
-    return os.getenv(bstack1ll1_opy_ (u"࠭ࡔࡓࡃ࡙ࡍࡘࡥࡂࡖࡋࡏࡈࡤࡔࡕࡎࡄࡈࡖࠬઢ"), 0)
-  if str(os.getenv(bstack1ll1_opy_ (u"ࠧࡄࡋࠪણ"))).lower() == bstack1ll1_opy_ (u"ࠨࡶࡵࡹࡪ࠭ત") and str(os.getenv(bstack1ll1_opy_ (u"ࠩࡆࡍࡤࡔࡁࡎࡇࠪથ"))).lower() == bstack1ll1_opy_ (u"ࠪࡧࡴࡪࡥࡴࡪ࡬ࡴࠬદ"):
-    return 0 # bstack1ll111111_opy_ bstack1l1lll1l_opy_ not set build number env
-  if os.getenv(bstack1ll1_opy_ (u"ࠫࡇࡏࡔࡃࡗࡆࡏࡊ࡚࡟ࡃࡔࡄࡒࡈࡎࠧધ")) and os.getenv(bstack1ll1_opy_ (u"ࠬࡈࡉࡕࡄࡘࡇࡐࡋࡔࡠࡅࡒࡑࡒࡏࡔࠨન")):
-    return os.getenv(bstack1ll1_opy_ (u"࠭ࡂࡊࡖࡅ࡙ࡈࡑࡅࡕࡡࡅ࡙ࡎࡒࡄࡠࡐࡘࡑࡇࡋࡒࠨ઩"), 0)
-  if str(os.getenv(bstack1ll1_opy_ (u"ࠧࡄࡋࠪપ"))).lower() == bstack1ll1_opy_ (u"ࠨࡶࡵࡹࡪ࠭ફ") and str(os.getenv(bstack1ll1_opy_ (u"ࠩࡇࡖࡔࡔࡅࠨબ"))).lower() == bstack1ll1_opy_ (u"ࠪࡸࡷࡻࡥࠨભ"):
-    return os.getenv(bstack1ll1_opy_ (u"ࠫࡉࡘࡏࡏࡇࡢࡆ࡚ࡏࡌࡅࡡࡑ࡙ࡒࡈࡅࡓࠩમ"), 0)
-  if str(os.getenv(bstack1ll1_opy_ (u"ࠬࡉࡉࠨય"))).lower() == bstack1ll1_opy_ (u"࠭ࡴࡳࡷࡨࠫર") and str(os.getenv(bstack1ll1_opy_ (u"ࠧࡔࡇࡐࡅࡕࡎࡏࡓࡇࠪ઱"))).lower() == bstack1ll1_opy_ (u"ࠨࡶࡵࡹࡪ࠭લ"):
-    return os.getenv(bstack1ll1_opy_ (u"ࠩࡖࡉࡒࡇࡐࡉࡑࡕࡉࡤࡐࡏࡃࡡࡌࡈࠬળ"), 0)
-  if str(os.getenv(bstack1ll1_opy_ (u"ࠪࡇࡎ࠭઴"))).lower() == bstack1ll1_opy_ (u"ࠫࡹࡸࡵࡦࠩવ") and str(os.getenv(bstack1ll1_opy_ (u"ࠬࡍࡉࡕࡎࡄࡆࡤࡉࡉࠨશ"))).lower() == bstack1ll1_opy_ (u"࠭ࡴࡳࡷࡨࠫષ"):
-    return os.getenv(bstack1ll1_opy_ (u"ࠧࡄࡋࡢࡎࡔࡈ࡟ࡊࡆࠪસ"), 0)
-  if str(os.getenv(bstack1ll1_opy_ (u"ࠨࡅࡌࠫહ"))).lower() == bstack1ll1_opy_ (u"ࠩࡷࡶࡺ࡫ࠧ઺") and str(os.getenv(bstack1ll1_opy_ (u"ࠪࡆ࡚ࡏࡌࡅࡍࡌࡘࡊ࠭઻"))).lower() == bstack1ll1_opy_ (u"ࠫࡹࡸࡵࡦ઼ࠩ"):
-    return os.getenv(bstack1ll1_opy_ (u"ࠬࡈࡕࡊࡎࡇࡏࡎ࡚ࡅࡠࡄࡘࡍࡑࡊ࡟ࡏࡗࡐࡆࡊࡘࠧઽ"), 0)
-  if str(os.getenv(bstack1ll1_opy_ (u"࠭ࡔࡇࡡࡅ࡙ࡎࡒࡄࠨા"))).lower() == bstack1ll1_opy_ (u"ࠧࡵࡴࡸࡩࠬિ"):
-    return os.getenv(bstack1ll1_opy_ (u"ࠨࡄࡘࡍࡑࡊ࡟ࡃࡗࡌࡐࡉࡏࡄࠨી"), 0)
+    return os.getenv(bstack11_opy_ (u"ࠧࡃࡗࡌࡐࡉࡥࡎࡖࡏࡅࡉࡗ࠭઱"), 0)
+  if str(os.getenv(bstack11_opy_ (u"ࠨࡅࡌࠫલ"))).lower() == bstack11_opy_ (u"ࠩࡷࡶࡺ࡫ࠧળ") and str(os.getenv(bstack11_opy_ (u"ࠪࡇࡎࡘࡃࡍࡇࡆࡍࠬ઴"))).lower() == bstack11_opy_ (u"ࠫࡹࡸࡵࡦࠩવ"):
+    return os.getenv(bstack11_opy_ (u"ࠬࡉࡉࡓࡅࡏࡉࡤࡈࡕࡊࡎࡇࡣࡓ࡛ࡍࠨશ"), 0)
+  if str(os.getenv(bstack11_opy_ (u"࠭ࡃࡊࠩષ"))).lower() == bstack11_opy_ (u"ࠧࡵࡴࡸࡩࠬસ") and str(os.getenv(bstack11_opy_ (u"ࠨࡖࡕࡅ࡛ࡏࡓࠨહ"))).lower() == bstack11_opy_ (u"ࠩࡷࡶࡺ࡫ࠧ઺"):
+    return os.getenv(bstack11_opy_ (u"ࠪࡘࡗࡇࡖࡊࡕࡢࡆ࡚ࡏࡌࡅࡡࡑ࡙ࡒࡈࡅࡓࠩ઻"), 0)
+  if str(os.getenv(bstack11_opy_ (u"ࠫࡈࡏ઼ࠧ"))).lower() == bstack11_opy_ (u"ࠬࡺࡲࡶࡧࠪઽ") and str(os.getenv(bstack11_opy_ (u"࠭ࡃࡊࡡࡑࡅࡒࡋࠧા"))).lower() == bstack11_opy_ (u"ࠧࡤࡱࡧࡩࡸ࡮ࡩࡱࠩિ"):
+    return 0 # bstack1l1l1l1l1_opy_ bstack1l1l11111_opy_ not set build number env
+  if os.getenv(bstack11_opy_ (u"ࠨࡄࡌࡘࡇ࡛ࡃࡌࡇࡗࡣࡇࡘࡁࡏࡅࡋࠫી")) and os.getenv(bstack11_opy_ (u"ࠩࡅࡍ࡙ࡈࡕࡄࡍࡈࡘࡤࡉࡏࡎࡏࡌࡘࠬુ")):
+    return os.getenv(bstack11_opy_ (u"ࠪࡆࡎ࡚ࡂࡖࡅࡎࡉ࡙ࡥࡂࡖࡋࡏࡈࡤࡔࡕࡎࡄࡈࡖࠬૂ"), 0)
+  if str(os.getenv(bstack11_opy_ (u"ࠫࡈࡏࠧૃ"))).lower() == bstack11_opy_ (u"ࠬࡺࡲࡶࡧࠪૄ") and str(os.getenv(bstack11_opy_ (u"࠭ࡄࡓࡑࡑࡉࠬૅ"))).lower() == bstack11_opy_ (u"ࠧࡵࡴࡸࡩࠬ૆"):
+    return os.getenv(bstack11_opy_ (u"ࠨࡆࡕࡓࡓࡋ࡟ࡃࡗࡌࡐࡉࡥࡎࡖࡏࡅࡉࡗ࠭ે"), 0)
+  if str(os.getenv(bstack11_opy_ (u"ࠩࡆࡍࠬૈ"))).lower() == bstack11_opy_ (u"ࠪࡸࡷࡻࡥࠨૉ") and str(os.getenv(bstack11_opy_ (u"ࠫࡘࡋࡍࡂࡒࡋࡓࡗࡋࠧ૊"))).lower() == bstack11_opy_ (u"ࠬࡺࡲࡶࡧࠪો"):
+    return os.getenv(bstack11_opy_ (u"࠭ࡓࡆࡏࡄࡔࡍࡕࡒࡆࡡࡍࡓࡇࡥࡉࡅࠩૌ"), 0)
+  if str(os.getenv(bstack11_opy_ (u"ࠧࡄࡋ્ࠪ"))).lower() == bstack11_opy_ (u"ࠨࡶࡵࡹࡪ࠭૎") and str(os.getenv(bstack11_opy_ (u"ࠩࡊࡍ࡙ࡒࡁࡃࡡࡆࡍࠬ૏"))).lower() == bstack11_opy_ (u"ࠪࡸࡷࡻࡥࠨૐ"):
+    return os.getenv(bstack11_opy_ (u"ࠫࡈࡏ࡟ࡋࡑࡅࡣࡎࡊࠧ૑"), 0)
+  if str(os.getenv(bstack11_opy_ (u"ࠬࡉࡉࠨ૒"))).lower() == bstack11_opy_ (u"࠭ࡴࡳࡷࡨࠫ૓") and str(os.getenv(bstack11_opy_ (u"ࠧࡃࡗࡌࡐࡉࡑࡉࡕࡇࠪ૔"))).lower() == bstack11_opy_ (u"ࠨࡶࡵࡹࡪ࠭૕"):
+    return os.getenv(bstack11_opy_ (u"ࠩࡅ࡙ࡎࡒࡄࡌࡋࡗࡉࡤࡈࡕࡊࡎࡇࡣࡓ࡛ࡍࡃࡇࡕࠫ૖"), 0)
+  if str(os.getenv(bstack11_opy_ (u"ࠪࡘࡋࡥࡂࡖࡋࡏࡈࠬ૗"))).lower() == bstack11_opy_ (u"ࠫࡹࡸࡵࡦࠩ૘"):
+    return os.getenv(bstack11_opy_ (u"ࠬࡈࡕࡊࡎࡇࡣࡇ࡛ࡉࡍࡆࡌࡈࠬ૙"), 0)
   return -1
-def bstack1ll111l_opy_(bstack1ll11l_opy_):
+def bstack1ll11l1_opy_(bstack1111l11l_opy_):
   global CONFIG
-  if not bstack1ll1_opy_ (u"ࠩࠧࡿࡇ࡛ࡉࡍࡆࡢࡒ࡚ࡓࡂࡆࡔࢀࠫુ") in CONFIG[bstack1ll1_opy_ (u"ࠪࡦࡺ࡯࡬ࡥࡋࡧࡩࡳࡺࡩࡧ࡫ࡨࡶࠬૂ")]:
+  if not bstack11_opy_ (u"࠭ࠤࡼࡄࡘࡍࡑࡊ࡟ࡏࡗࡐࡆࡊࡘࡽࠨ૚") in CONFIG[bstack11_opy_ (u"ࠧࡣࡷ࡬ࡰࡩࡏࡤࡦࡰࡷ࡭࡫࡯ࡥࡳࠩ૛")]:
     return
-  CONFIG[bstack1ll1_opy_ (u"ࠫࡧࡻࡩ࡭ࡦࡌࡨࡪࡴࡴࡪࡨ࡬ࡩࡷ࠭ૃ")] = CONFIG[bstack1ll1_opy_ (u"ࠬࡨࡵࡪ࡮ࡧࡍࡩ࡫࡮ࡵ࡫ࡩ࡭ࡪࡸࠧૄ")].replace(
-    bstack1ll1_opy_ (u"࠭ࠤࡼࡄࡘࡍࡑࡊ࡟ࡏࡗࡐࡆࡊࡘࡽࠨૅ"),
-    str(bstack1ll11l_opy_)
+  CONFIG[bstack11_opy_ (u"ࠨࡤࡸ࡭ࡱࡪࡉࡥࡧࡱࡸ࡮࡬ࡩࡦࡴࠪ૜")] = CONFIG[bstack11_opy_ (u"ࠩࡥࡹ࡮ࡲࡤࡊࡦࡨࡲࡹ࡯ࡦࡪࡧࡵࠫ૝")].replace(
+    bstack11_opy_ (u"ࠪࠨࢀࡈࡕࡊࡎࡇࡣࡓ࡛ࡍࡃࡇࡕࢁࠬ૞"),
+    str(bstack1111l11l_opy_)
   )
-def bstack1ll1l111_opy_():
+def bstack1ll111l_opy_():
   global CONFIG
-  if not bstack1ll1_opy_ (u"ࠧࠥࡽࡇࡅ࡙ࡋ࡟ࡕࡋࡐࡉࢂ࠭૆") in CONFIG[bstack1ll1_opy_ (u"ࠨࡤࡸ࡭ࡱࡪࡉࡥࡧࡱࡸ࡮࡬ࡩࡦࡴࠪે")]:
+  if not bstack11_opy_ (u"ࠫࠩࢁࡄࡂࡖࡈࡣ࡙ࡏࡍࡆࡿࠪ૟") in CONFIG[bstack11_opy_ (u"ࠬࡨࡵࡪ࡮ࡧࡍࡩ࡫࡮ࡵ࡫ࡩ࡭ࡪࡸࠧૠ")]:
     return
-  bstack1lll11l1l_opy_ = datetime.datetime.now()
-  bstack1lll11l11_opy_ = bstack1lll11l1l_opy_.strftime(bstack1ll1_opy_ (u"ࠩࠨࡨ࠲ࠫࡢ࠮ࠧࡋ࠾ࠪࡓࠧૈ"))
-  CONFIG[bstack1ll1_opy_ (u"ࠪࡦࡺ࡯࡬ࡥࡋࡧࡩࡳࡺࡩࡧ࡫ࡨࡶࠬૉ")] = CONFIG[bstack1ll1_opy_ (u"ࠫࡧࡻࡩ࡭ࡦࡌࡨࡪࡴࡴࡪࡨ࡬ࡩࡷ࠭૊")].replace(
-    bstack1ll1_opy_ (u"ࠬࠪࡻࡅࡃࡗࡉࡤ࡚ࡉࡎࡇࢀࠫો"),
-    bstack1lll11l11_opy_
+  bstack1lll11ll_opy_ = datetime.datetime.now()
+  bstack11l11l11_opy_ = bstack1lll11ll_opy_.strftime(bstack11_opy_ (u"࠭ࠥࡥ࠯ࠨࡦ࠲ࠫࡈ࠻ࠧࡐࠫૡ"))
+  CONFIG[bstack11_opy_ (u"ࠧࡣࡷ࡬ࡰࡩࡏࡤࡦࡰࡷ࡭࡫࡯ࡥࡳࠩૢ")] = CONFIG[bstack11_opy_ (u"ࠨࡤࡸ࡭ࡱࡪࡉࡥࡧࡱࡸ࡮࡬ࡩࡦࡴࠪૣ")].replace(
+    bstack11_opy_ (u"ࠩࠧࡿࡉࡇࡔࡆࡡࡗࡍࡒࡋࡽࠨ૤"),
+    bstack11l11l11_opy_
   )
-def bstack1l1l1_opy_():
+def bstack1ll111l11_opy_():
   global CONFIG
-  if bstack1ll1_opy_ (u"࠭ࡢࡶ࡫࡯ࡨࡎࡪࡥ࡯ࡶ࡬ࡪ࡮࡫ࡲࠨૌ") in CONFIG and not bool(CONFIG[bstack1ll1_opy_ (u"ࠧࡣࡷ࡬ࡰࡩࡏࡤࡦࡰࡷ࡭࡫࡯ࡥࡳ્ࠩ")]):
-    del CONFIG[bstack1ll1_opy_ (u"ࠨࡤࡸ࡭ࡱࡪࡉࡥࡧࡱࡸ࡮࡬ࡩࡦࡴࠪ૎")]
+  if bstack11_opy_ (u"ࠪࡦࡺ࡯࡬ࡥࡋࡧࡩࡳࡺࡩࡧ࡫ࡨࡶࠬ૥") in CONFIG and not bool(CONFIG[bstack11_opy_ (u"ࠫࡧࡻࡩ࡭ࡦࡌࡨࡪࡴࡴࡪࡨ࡬ࡩࡷ࠭૦")]):
+    del CONFIG[bstack11_opy_ (u"ࠬࡨࡵࡪ࡮ࡧࡍࡩ࡫࡮ࡵ࡫ࡩ࡭ࡪࡸࠧ૧")]
     return
-  if not bstack1ll1_opy_ (u"ࠩࡥࡹ࡮ࡲࡤࡊࡦࡨࡲࡹ࡯ࡦࡪࡧࡵࠫ૏") in CONFIG:
-    CONFIG[bstack1ll1_opy_ (u"ࠪࡦࡺ࡯࡬ࡥࡋࡧࡩࡳࡺࡩࡧ࡫ࡨࡶࠬૐ")] = bstack1ll1_opy_ (u"ࠫࠨࠪࡻࡃࡗࡌࡐࡉࡥࡎࡖࡏࡅࡉࡗࢃࠧ૑")
-  if bstack1ll1_opy_ (u"ࠬࠪࡻࡅࡃࡗࡉࡤ࡚ࡉࡎࡇࢀࠫ૒") in CONFIG[bstack1ll1_opy_ (u"࠭ࡢࡶ࡫࡯ࡨࡎࡪࡥ࡯ࡶ࡬ࡪ࡮࡫ࡲࠨ૓")]:
-    bstack1ll1l111_opy_()
-    os.environ[bstack1ll1_opy_ (u"ࠧࡃࡕࡗࡅࡈࡑ࡟ࡄࡑࡐࡆࡎࡔࡅࡅࡡࡅ࡙ࡎࡒࡄࡠࡋࡇࠫ૔")] = CONFIG[bstack1ll1_opy_ (u"ࠨࡤࡸ࡭ࡱࡪࡉࡥࡧࡱࡸ࡮࡬ࡩࡦࡴࠪ૕")]
-  if not bstack1ll1_opy_ (u"ࠩࠧࡿࡇ࡛ࡉࡍࡆࡢࡒ࡚ࡓࡂࡆࡔࢀࠫ૖") in CONFIG[bstack1ll1_opy_ (u"ࠪࡦࡺ࡯࡬ࡥࡋࡧࡩࡳࡺࡩࡧ࡫ࡨࡶࠬ૗")]:
+  if not bstack11_opy_ (u"࠭ࡢࡶ࡫࡯ࡨࡎࡪࡥ࡯ࡶ࡬ࡪ࡮࡫ࡲࠨ૨") in CONFIG:
+    CONFIG[bstack11_opy_ (u"ࠧࡣࡷ࡬ࡰࡩࡏࡤࡦࡰࡷ࡭࡫࡯ࡥࡳࠩ૩")] = bstack11_opy_ (u"ࠨࠥࠧࡿࡇ࡛ࡉࡍࡆࡢࡒ࡚ࡓࡂࡆࡔࢀࠫ૪")
+  if bstack11_opy_ (u"ࠩࠧࡿࡉࡇࡔࡆࡡࡗࡍࡒࡋࡽࠨ૫") in CONFIG[bstack11_opy_ (u"ࠪࡦࡺ࡯࡬ࡥࡋࡧࡩࡳࡺࡩࡧ࡫ࡨࡶࠬ૬")]:
+    bstack1ll111l_opy_()
+    os.environ[bstack11_opy_ (u"ࠫࡇ࡙ࡔࡂࡅࡎࡣࡈࡕࡍࡃࡋࡑࡉࡉࡥࡂࡖࡋࡏࡈࡤࡏࡄࠨ૭")] = CONFIG[bstack11_opy_ (u"ࠬࡨࡵࡪ࡮ࡧࡍࡩ࡫࡮ࡵ࡫ࡩ࡭ࡪࡸࠧ૮")]
+  if not bstack11_opy_ (u"࠭ࠤࡼࡄࡘࡍࡑࡊ࡟ࡏࡗࡐࡆࡊࡘࡽࠨ૯") in CONFIG[bstack11_opy_ (u"ࠧࡣࡷ࡬ࡰࡩࡏࡤࡦࡰࡷ࡭࡫࡯ࡥࡳࠩ૰")]:
     return
-  bstack1ll11l_opy_ = bstack1ll1_opy_ (u"ࠫࠬ૘")
-  bstack1ll1l1l1l_opy_ = bstack1lll1l11_opy_()
-  if bstack1ll1l1l1l_opy_ != -1:
-    bstack1ll11l_opy_ = bstack1ll1_opy_ (u"ࠬࡉࡉࠡࠩ૙") + str(bstack1ll1l1l1l_opy_)
-  if bstack1ll11l_opy_ == bstack1ll1_opy_ (u"࠭ࠧ૚"):
-    bstack11l1111_opy_ = bstack1ll111l1_opy_(CONFIG[bstack1ll1_opy_ (u"ࠧࡣࡷ࡬ࡰࡩࡔࡡ࡮ࡧࠪ૛")])
-    if bstack11l1111_opy_ != -1:
-      bstack1ll11l_opy_ = str(bstack11l1111_opy_)
-  if bstack1ll11l_opy_:
-    bstack1ll111l_opy_(bstack1ll11l_opy_)
-    os.environ[bstack1ll1_opy_ (u"ࠨࡄࡖࡘࡆࡉࡋࡠࡅࡒࡑࡇࡏࡎࡆࡆࡢࡆ࡚ࡏࡌࡅࡡࡌࡈࠬ૜")] = CONFIG[bstack1ll1_opy_ (u"ࠩࡥࡹ࡮ࡲࡤࡊࡦࡨࡲࡹ࡯ࡦࡪࡧࡵࠫ૝")]
-def bstack1ll1l1111_opy_(bstack1ll1l1l1_opy_, bstack111l1l1_opy_, path):
-  bstack1l1lll1_opy_ = {
-    bstack1ll1_opy_ (u"ࠪ࡭ࡩ࡫࡮ࡵ࡫ࡩ࡭ࡪࡸࠧ૞"): bstack111l1l1_opy_
+  bstack1111l11l_opy_ = bstack11_opy_ (u"ࠨࠩ૱")
+  bstack1ll1lllll_opy_ = bstack11111_opy_()
+  if bstack1ll1lllll_opy_ != -1:
+    bstack1111l11l_opy_ = bstack11_opy_ (u"ࠩࡆࡍࠥ࠭૲") + str(bstack1ll1lllll_opy_)
+  if bstack1111l11l_opy_ == bstack11_opy_ (u"ࠪࠫ૳"):
+    bstack1l11l1ll1_opy_ = bstack1lll1ll_opy_(CONFIG[bstack11_opy_ (u"ࠫࡧࡻࡩ࡭ࡦࡑࡥࡲ࡫ࠧ૴")])
+    if bstack1l11l1ll1_opy_ != -1:
+      bstack1111l11l_opy_ = str(bstack1l11l1ll1_opy_)
+  if bstack1111l11l_opy_:
+    bstack1ll11l1_opy_(bstack1111l11l_opy_)
+    os.environ[bstack11_opy_ (u"ࠬࡈࡓࡕࡃࡆࡏࡤࡉࡏࡎࡄࡌࡒࡊࡊ࡟ࡃࡗࡌࡐࡉࡥࡉࡅࠩ૵")] = CONFIG[bstack11_opy_ (u"࠭ࡢࡶ࡫࡯ࡨࡎࡪࡥ࡯ࡶ࡬ࡪ࡮࡫ࡲࠨ૶")]
+def bstack111ll1_opy_(bstack11l1l_opy_, bstack1lll1111l_opy_, path):
+  bstack1lll11l1l_opy_ = {
+    bstack11_opy_ (u"ࠧࡪࡦࡨࡲࡹ࡯ࡦࡪࡧࡵࠫ૷"): bstack1lll1111l_opy_
   }
   if os.path.exists(path):
-    bstack1111ll1_opy_ = json.load(open(path, bstack1ll1_opy_ (u"ࠫࡷࡨࠧ૟")))
+    bstack1l1l1_opy_ = json.load(open(path, bstack11_opy_ (u"ࠨࡴࡥࠫ૸")))
   else:
-    bstack1111ll1_opy_ = {}
-  bstack1111ll1_opy_[bstack1ll1l1l1_opy_] = bstack1l1lll1_opy_
-  with open(path, bstack1ll1_opy_ (u"ࠧࡽࠫࠣૠ")) as outfile:
-    json.dump(bstack1111ll1_opy_, outfile)
-def bstack1ll111l1_opy_(bstack1ll1l1l1_opy_):
-  bstack1ll1l1l1_opy_ = str(bstack1ll1l1l1_opy_)
-  bstack11ll11ll_opy_ = os.path.join(os.path.expanduser(bstack1ll1_opy_ (u"࠭ࡾࠨૡ")), bstack1ll1_opy_ (u"ࠧ࠯ࡤࡵࡳࡼࡹࡥࡳࡵࡷࡥࡨࡱࠧૢ"))
-  try:
-    if not os.path.exists(bstack11ll11ll_opy_):
-      os.makedirs(bstack11ll11ll_opy_)
-    file_path = os.path.join(os.path.expanduser(bstack1ll1_opy_ (u"ࠨࢀࠪૣ")), bstack1ll1_opy_ (u"ࠩ࠱ࡦࡷࡵࡷࡴࡧࡵࡷࡹࡧࡣ࡬ࠩ૤"), bstack1ll1_opy_ (u"ࠪ࠲ࡧࡻࡩ࡭ࡦ࠰ࡲࡦࡳࡥ࠮ࡥࡤࡧ࡭࡫࠮࡫ࡵࡲࡲࠬ૥"))
+    bstack1l1l1_opy_ = {}
+  bstack1l1l1_opy_[bstack11l1l_opy_] = bstack1lll11l1l_opy_
+  with open(path, bstack11_opy_ (u"ࠤࡺ࠯ࠧૹ")) as outfile:
+    json.dump(bstack1l1l1_opy_, outfile)
+def bstack1lll1ll_opy_(bstack11l1l_opy_):
+  bstack11l1l_opy_ = str(bstack11l1l_opy_)
+  bstack1l1lll11_opy_ = os.path.join(os.path.expanduser(bstack11_opy_ (u"ࠪࢂࠬૺ")), bstack11_opy_ (u"ࠫ࠳ࡨࡲࡰࡹࡶࡩࡷࡹࡴࡢࡥ࡮ࠫૻ"))
+  try:
+    if not os.path.exists(bstack1l1lll11_opy_):
+      os.makedirs(bstack1l1lll11_opy_)
+    file_path = os.path.join(os.path.expanduser(bstack11_opy_ (u"ࠬࢄࠧૼ")), bstack11_opy_ (u"࠭࠮ࡣࡴࡲࡻࡸ࡫ࡲࡴࡶࡤࡧࡰ࠭૽"), bstack11_opy_ (u"ࠧ࠯ࡤࡸ࡭ࡱࡪ࠭࡯ࡣࡰࡩ࠲ࡩࡡࡤࡪࡨ࠲࡯ࡹ࡯࡯ࠩ૾"))
     if not os.path.isfile(file_path):
-      with open(file_path, bstack1ll1_opy_ (u"ࠫࡼ࠭૦")):
+      with open(file_path, bstack11_opy_ (u"ࠨࡹࠪ૿")):
         pass
-      with open(file_path, bstack1ll1_opy_ (u"ࠧࡽࠫࠣ૧")) as outfile:
+      with open(file_path, bstack11_opy_ (u"ࠤࡺ࠯ࠧ଀")) as outfile:
         json.dump({}, outfile)
-    with open(file_path, bstack1ll1_opy_ (u"࠭ࡲࠨ૨")) as bstack1llll1l_opy_:
-      bstack1ll1l_opy_ = json.load(bstack1llll1l_opy_)
-    if bstack1ll1l1l1_opy_ in bstack1ll1l_opy_:
-      bstack1ll1l11ll_opy_ = bstack1ll1l_opy_[bstack1ll1l1l1_opy_][bstack1ll1_opy_ (u"ࠧࡪࡦࡨࡲࡹ࡯ࡦࡪࡧࡵࠫ૩")]
-      bstack1l11ll1l1_opy_ = int(bstack1ll1l11ll_opy_) + 1
-      bstack1ll1l1111_opy_(bstack1ll1l1l1_opy_, bstack1l11ll1l1_opy_, file_path)
-      return bstack1l11ll1l1_opy_
+    with open(file_path, bstack11_opy_ (u"ࠪࡶࠬଁ")) as bstack1111111_opy_:
+      bstack1ll11l1l1_opy_ = json.load(bstack1111111_opy_)
+    if bstack11l1l_opy_ in bstack1ll11l1l1_opy_:
+      bstack1llll1ll_opy_ = bstack1ll11l1l1_opy_[bstack11l1l_opy_][bstack11_opy_ (u"ࠫ࡮ࡪࡥ࡯ࡶ࡬ࡪ࡮࡫ࡲࠨଂ")]
+      bstack111l1l_opy_ = int(bstack1llll1ll_opy_) + 1
+      bstack111ll1_opy_(bstack11l1l_opy_, bstack111l1l_opy_, file_path)
+      return bstack111l1l_opy_
     else:
-      bstack1ll1l1111_opy_(bstack1ll1l1l1_opy_, 1, file_path)
+      bstack111ll1_opy_(bstack11l1l_opy_, 1, file_path)
       return 1
   except Exception as e:
-    logger.warn(bstack11111l_opy_.format(str(e)))
+    logger.warn(bstack1l1ll1l1_opy_.format(str(e)))
     return -1
-def bstack1ll1l111l_opy_(config):
-  if not config[bstack1ll1_opy_ (u"ࠨࡷࡶࡩࡷࡔࡡ࡮ࡧࠪ૪")] or not config[bstack1ll1_opy_ (u"ࠩࡤࡧࡨ࡫ࡳࡴࡍࡨࡽࠬ૫")]:
+def bstack11ll1ll1_opy_(config):
+  if not config[bstack11_opy_ (u"ࠬࡻࡳࡦࡴࡑࡥࡲ࡫ࠧଃ")] or not config[bstack11_opy_ (u"࠭ࡡࡤࡥࡨࡷࡸࡑࡥࡺࠩ଄")]:
     return True
   else:
     return False
-def bstack1l11l1_opy_(config):
-  if bstack1ll1llll_opy_() < version.parse(bstack1ll1_opy_ (u"ࠪ࠷࠳࠺࠮࠱ࠩ૬")):
+def bstack1ll11111_opy_(config):
+  if bstack1ll11l1ll_opy_() < version.parse(bstack11_opy_ (u"ࠧ࠴࠰࠷࠲࠵࠭ଅ")):
     return False
-  if bstack1ll1llll_opy_() >= version.parse(bstack1ll1_opy_ (u"ࠫ࠹࠴࠱࠯࠷ࠪ૭")):
+  if bstack1ll11l1ll_opy_() >= version.parse(bstack11_opy_ (u"ࠨ࠶࠱࠵࠳࠻ࠧଆ")):
     return True
-  if bstack1ll1_opy_ (u"ࠬࡻࡳࡦ࡙࠶ࡇࠬ૮") in config and config[bstack1ll1_opy_ (u"࠭ࡵࡴࡧ࡚࠷ࡈ࠭૯")] == False:
+  if bstack11_opy_ (u"ࠩࡸࡷࡪ࡝࠳ࡄࠩଇ") in config and config[bstack11_opy_ (u"ࠪࡹࡸ࡫ࡗ࠴ࡅࠪଈ")] == False:
     return False
   else:
     return True
-def bstack1111l_opy_(config, index = 0):
-  global bstack1ll11111l_opy_
-  bstack11l1l111_opy_ = {}
-  caps = bstack1llll_opy_ + bstack111ll_opy_
-  if bstack1ll11111l_opy_:
-    caps += bstack1l11l1lll_opy_
+def bstack111llll1_opy_(config, index = 0):
+  global bstack1llll1l_opy_
+  bstack11l1111l_opy_ = {}
+  caps = bstack1l111l1_opy_ + bstack1l11ll11l_opy_
+  if bstack1llll1l_opy_:
+    caps += bstack1l1l1l_opy_
   for key in config:
-    if key in caps + [bstack1ll1_opy_ (u"ࠧࡱ࡮ࡤࡸ࡫ࡵࡲ࡮ࡵࠪ૰")]:
+    if key in caps + [bstack11_opy_ (u"ࠫࡵࡲࡡࡵࡨࡲࡶࡲࡹࠧଉ")]:
       continue
-    bstack11l1l111_opy_[key] = config[key]
-  if bstack1ll1_opy_ (u"ࠨࡲ࡯ࡥࡹ࡬࡯ࡳ࡯ࡶࠫ૱") in config:
-    for bstack111ll1ll_opy_ in config[bstack1ll1_opy_ (u"ࠩࡳࡰࡦࡺࡦࡰࡴࡰࡷࠬ૲")][index]:
-      if bstack111ll1ll_opy_ in caps + [bstack1ll1_opy_ (u"ࠪࡦࡷࡵࡷࡴࡧࡵࡒࡦࡳࡥࠨ૳"), bstack1ll1_opy_ (u"ࠫࡧࡸ࡯ࡸࡵࡨࡶ࡛࡫ࡲࡴ࡫ࡲࡲࠬ૴")]:
+    bstack11l1111l_opy_[key] = config[key]
+  if bstack11_opy_ (u"ࠬࡶ࡬ࡢࡶࡩࡳࡷࡳࡳࠨଊ") in config:
+    for bstack111l11l_opy_ in config[bstack11_opy_ (u"࠭ࡰ࡭ࡣࡷࡪࡴࡸ࡭ࡴࠩଋ")][index]:
+      if bstack111l11l_opy_ in caps + [bstack11_opy_ (u"ࠧࡣࡴࡲࡻࡸ࡫ࡲࡏࡣࡰࡩࠬଌ"), bstack11_opy_ (u"ࠨࡤࡵࡳࡼࡹࡥࡳࡘࡨࡶࡸ࡯࡯࡯ࠩ଍")]:
         continue
-      bstack11l1l111_opy_[bstack111ll1ll_opy_] = config[bstack1ll1_opy_ (u"ࠬࡶ࡬ࡢࡶࡩࡳࡷࡳࡳࠨ૵")][index][bstack111ll1ll_opy_]
-  bstack11l1l111_opy_[bstack1ll1_opy_ (u"࠭ࡨࡰࡵࡷࡒࡦࡳࡥࠨ૶")] = socket.gethostname()
-  if bstack1ll1_opy_ (u"ࠧࡷࡧࡵࡷ࡮ࡵ࡮ࠨ૷") in bstack11l1l111_opy_:
-    del(bstack11l1l111_opy_[bstack1ll1_opy_ (u"ࠨࡸࡨࡶࡸ࡯࡯࡯ࠩ૸")])
-  return bstack11l1l111_opy_
-def bstack1l1l11l11_opy_(config):
-  global bstack1ll11111l_opy_
-  bstack11ll1l11_opy_ = {}
-  caps = bstack111ll_opy_
-  if bstack1ll11111l_opy_:
-    caps+= bstack1l11l1lll_opy_
+      bstack11l1111l_opy_[bstack111l11l_opy_] = config[bstack11_opy_ (u"ࠩࡳࡰࡦࡺࡦࡰࡴࡰࡷࠬ଎")][index][bstack111l11l_opy_]
+  bstack11l1111l_opy_[bstack11_opy_ (u"ࠪ࡬ࡴࡹࡴࡏࡣࡰࡩࠬଏ")] = socket.gethostname()
+  if bstack11_opy_ (u"ࠫࡻ࡫ࡲࡴ࡫ࡲࡲࠬଐ") in bstack11l1111l_opy_:
+    del(bstack11l1111l_opy_[bstack11_opy_ (u"ࠬࡼࡥࡳࡵ࡬ࡳࡳ࠭଑")])
+  return bstack11l1111l_opy_
+def bstack111l1l1l_opy_(config):
+  global bstack1llll1l_opy_
+  bstack11l111_opy_ = {}
+  caps = bstack1l11ll11l_opy_
+  if bstack1llll1l_opy_:
+    caps+= bstack1l1l1l_opy_
   for key in caps:
     if key in config:
-      bstack11ll1l11_opy_[key] = config[key]
-  return bstack11ll1l11_opy_
-def bstack1ll111l11_opy_(bstack11l1l111_opy_, bstack11ll1l11_opy_):
-  bstack1llll11ll_opy_ = {}
-  for key in bstack11l1l111_opy_.keys():
-    if key in bstack111l11l_opy_:
-      bstack1llll11ll_opy_[bstack111l11l_opy_[key]] = bstack11l1l111_opy_[key]
-    else:
-      bstack1llll11ll_opy_[key] = bstack11l1l111_opy_[key]
-  for key in bstack11ll1l11_opy_:
-    if key in bstack111l11l_opy_:
-      bstack1llll11ll_opy_[bstack111l11l_opy_[key]] = bstack11ll1l11_opy_[key]
-    else:
-      bstack1llll11ll_opy_[key] = bstack11ll1l11_opy_[key]
-  return bstack1llll11ll_opy_
-def bstack1llll11l1_opy_(config, index = 0):
-  global bstack1ll11111l_opy_
+      bstack11l111_opy_[key] = config[key]
+  return bstack11l111_opy_
+def bstack1l111l_opy_(bstack11l1111l_opy_, bstack11l111_opy_):
+  bstack1l11l_opy_ = {}
+  for key in bstack11l1111l_opy_.keys():
+    if key in bstack1l1ll11l1_opy_:
+      bstack1l11l_opy_[bstack1l1ll11l1_opy_[key]] = bstack11l1111l_opy_[key]
+    else:
+      bstack1l11l_opy_[key] = bstack11l1111l_opy_[key]
+  for key in bstack11l111_opy_:
+    if key in bstack1l1ll11l1_opy_:
+      bstack1l11l_opy_[bstack1l1ll11l1_opy_[key]] = bstack11l111_opy_[key]
+    else:
+      bstack1l11l_opy_[key] = bstack11l111_opy_[key]
+  return bstack1l11l_opy_
+def bstack1l111l1ll_opy_(config, index = 0):
+  global bstack1llll1l_opy_
   caps = {}
-  bstack11ll1l11_opy_ = bstack1l1l11l11_opy_(config)
-  bstack1l111l11_opy_ = bstack111ll_opy_
-  bstack1l111l11_opy_ += bstack11111l11_opy_
-  if bstack1ll11111l_opy_:
-    bstack1l111l11_opy_ += bstack1l11l1lll_opy_
-  if bstack1ll1_opy_ (u"ࠩࡳࡰࡦࡺࡦࡰࡴࡰࡷࠬૹ") in config:
-    if bstack1ll1_opy_ (u"ࠪࡦࡷࡵࡷࡴࡧࡵࡒࡦࡳࡥࠨૺ") in config[bstack1ll1_opy_ (u"ࠫࡵࡲࡡࡵࡨࡲࡶࡲࡹࠧૻ")][index]:
-      caps[bstack1ll1_opy_ (u"ࠬࡨࡲࡰࡹࡶࡩࡷࡔࡡ࡮ࡧࠪૼ")] = config[bstack1ll1_opy_ (u"࠭ࡰ࡭ࡣࡷࡪࡴࡸ࡭ࡴࠩ૽")][index][bstack1ll1_opy_ (u"ࠧࡣࡴࡲࡻࡸ࡫ࡲࡏࡣࡰࡩࠬ૾")]
-    if bstack1ll1_opy_ (u"ࠨࡤࡵࡳࡼࡹࡥࡳࡘࡨࡶࡸ࡯࡯࡯ࠩ૿") in config[bstack1ll1_opy_ (u"ࠩࡳࡰࡦࡺࡦࡰࡴࡰࡷࠬ଀")][index]:
-      caps[bstack1ll1_opy_ (u"ࠪࡦࡷࡵࡷࡴࡧࡵ࡚ࡪࡸࡳࡪࡱࡱࠫଁ")] = str(config[bstack1ll1_opy_ (u"ࠫࡵࡲࡡࡵࡨࡲࡶࡲࡹࠧଂ")][index][bstack1ll1_opy_ (u"ࠬࡨࡲࡰࡹࡶࡩࡷ࡜ࡥࡳࡵ࡬ࡳࡳ࠭ଃ")])
-    bstack1111l11_opy_ = {}
-    for bstack11111111_opy_ in bstack1l111l11_opy_:
-      if bstack11111111_opy_ in config[bstack1ll1_opy_ (u"࠭ࡰ࡭ࡣࡷࡪࡴࡸ࡭ࡴࠩ଄")][index]:
-        if bstack11111111_opy_ == bstack1ll1_opy_ (u"ࠧࡱ࡮ࡤࡸ࡫ࡵࡲ࡮ࡘࡨࡶࡸ࡯࡯࡯ࠩଅ"):
-          bstack1111l11_opy_[bstack11111111_opy_] = str(config[bstack1ll1_opy_ (u"ࠨࡲ࡯ࡥࡹ࡬࡯ࡳ࡯ࡶࠫଆ")][index][bstack11111111_opy_] * 1.0)
+  bstack11l111_opy_ = bstack111l1l1l_opy_(config)
+  bstack1ll1l1l_opy_ = bstack1l11ll11l_opy_
+  bstack1ll1l1l_opy_ += bstack1l111l11_opy_
+  if bstack1llll1l_opy_:
+    bstack1ll1l1l_opy_ += bstack1l1l1l_opy_
+  if bstack11_opy_ (u"࠭ࡰ࡭ࡣࡷࡪࡴࡸ࡭ࡴࠩ଒") in config:
+    if bstack11_opy_ (u"ࠧࡣࡴࡲࡻࡸ࡫ࡲࡏࡣࡰࡩࠬଓ") in config[bstack11_opy_ (u"ࠨࡲ࡯ࡥࡹ࡬࡯ࡳ࡯ࡶࠫଔ")][index]:
+      caps[bstack11_opy_ (u"ࠩࡥࡶࡴࡽࡳࡦࡴࡑࡥࡲ࡫ࠧକ")] = config[bstack11_opy_ (u"ࠪࡴࡱࡧࡴࡧࡱࡵࡱࡸ࠭ଖ")][index][bstack11_opy_ (u"ࠫࡧࡸ࡯ࡸࡵࡨࡶࡓࡧ࡭ࡦࠩଗ")]
+    if bstack11_opy_ (u"ࠬࡨࡲࡰࡹࡶࡩࡷ࡜ࡥࡳࡵ࡬ࡳࡳ࠭ଘ") in config[bstack11_opy_ (u"࠭ࡰ࡭ࡣࡷࡪࡴࡸ࡭ࡴࠩଙ")][index]:
+      caps[bstack11_opy_ (u"ࠧࡣࡴࡲࡻࡸ࡫ࡲࡗࡧࡵࡷ࡮ࡵ࡮ࠨଚ")] = str(config[bstack11_opy_ (u"ࠨࡲ࡯ࡥࡹ࡬࡯ࡳ࡯ࡶࠫଛ")][index][bstack11_opy_ (u"ࠩࡥࡶࡴࡽࡳࡦࡴ࡙ࡩࡷࡹࡩࡰࡰࠪଜ")])
+    bstack111lllll_opy_ = {}
+    for bstack1ll1l1ll1_opy_ in bstack1ll1l1l_opy_:
+      if bstack1ll1l1ll1_opy_ in config[bstack11_opy_ (u"ࠪࡴࡱࡧࡴࡧࡱࡵࡱࡸ࠭ଝ")][index]:
+        if bstack1ll1l1ll1_opy_ == bstack11_opy_ (u"ࠫࡵࡲࡡࡵࡨࡲࡶࡲ࡜ࡥࡳࡵ࡬ࡳࡳ࠭ଞ"):
+          bstack111lllll_opy_[bstack1ll1l1ll1_opy_] = str(config[bstack11_opy_ (u"ࠬࡶ࡬ࡢࡶࡩࡳࡷࡳࡳࠨଟ")][index][bstack1ll1l1ll1_opy_] * 1.0)
         else:
-          bstack1111l11_opy_[bstack11111111_opy_] = config[bstack1ll1_opy_ (u"ࠩࡳࡰࡦࡺࡦࡰࡴࡰࡷࠬଇ")][index][bstack11111111_opy_]
-        del(config[bstack1ll1_opy_ (u"ࠪࡴࡱࡧࡴࡧࡱࡵࡱࡸ࠭ଈ")][index][bstack11111111_opy_])
-    bstack11ll1l11_opy_ = update(bstack11ll1l11_opy_, bstack1111l11_opy_)
-  bstack11l1l111_opy_ = bstack1111l_opy_(config, index)
-  for bstack1lllll1l1_opy_ in bstack111ll_opy_ + [bstack1ll1_opy_ (u"ࠫࡧࡸ࡯ࡸࡵࡨࡶࡓࡧ࡭ࡦࠩଉ"), bstack1ll1_opy_ (u"ࠬࡨࡲࡰࡹࡶࡩࡷ࡜ࡥࡳࡵ࡬ࡳࡳ࠭ଊ")]:
-    if bstack1lllll1l1_opy_ in bstack11l1l111_opy_:
-      bstack11ll1l11_opy_[bstack1lllll1l1_opy_] = bstack11l1l111_opy_[bstack1lllll1l1_opy_]
-      del(bstack11l1l111_opy_[bstack1lllll1l1_opy_])
-  if bstack1l11l1_opy_(config):
-    bstack11l1l111_opy_[bstack1ll1_opy_ (u"࠭ࡵࡴࡧ࡚࠷ࡈ࠭ଋ")] = True
-    caps.update(bstack11ll1l11_opy_)
-    caps[bstack1ll1_opy_ (u"ࠧࡣࡵࡷࡥࡨࡱ࠺ࡰࡲࡷ࡭ࡴࡴࡳࠨଌ")] = bstack11l1l111_opy_
+          bstack111lllll_opy_[bstack1ll1l1ll1_opy_] = config[bstack11_opy_ (u"࠭ࡰ࡭ࡣࡷࡪࡴࡸ࡭ࡴࠩଠ")][index][bstack1ll1l1ll1_opy_]
+        del(config[bstack11_opy_ (u"ࠧࡱ࡮ࡤࡸ࡫ࡵࡲ࡮ࡵࠪଡ")][index][bstack1ll1l1ll1_opy_])
+    bstack11l111_opy_ = update(bstack11l111_opy_, bstack111lllll_opy_)
+  bstack11l1111l_opy_ = bstack111llll1_opy_(config, index)
+  for bstack1llll1ll1_opy_ in bstack1l11ll11l_opy_ + [bstack11_opy_ (u"ࠨࡤࡵࡳࡼࡹࡥࡳࡐࡤࡱࡪ࠭ଢ"), bstack11_opy_ (u"ࠩࡥࡶࡴࡽࡳࡦࡴ࡙ࡩࡷࡹࡩࡰࡰࠪଣ")]:
+    if bstack1llll1ll1_opy_ in bstack11l1111l_opy_:
+      bstack11l111_opy_[bstack1llll1ll1_opy_] = bstack11l1111l_opy_[bstack1llll1ll1_opy_]
+      del(bstack11l1111l_opy_[bstack1llll1ll1_opy_])
+  if bstack1ll11111_opy_(config):
+    bstack11l1111l_opy_[bstack11_opy_ (u"ࠪࡹࡸ࡫ࡗ࠴ࡅࠪତ")] = True
+    caps.update(bstack11l111_opy_)
+    caps[bstack11_opy_ (u"ࠫࡧࡹࡴࡢࡥ࡮࠾ࡴࡶࡴࡪࡱࡱࡷࠬଥ")] = bstack11l1111l_opy_
   else:
-    bstack11l1l111_opy_[bstack1ll1_opy_ (u"ࠨࡷࡶࡩ࡜࠹ࡃࠨ଍")] = False
-    caps.update(bstack1ll111l11_opy_(bstack11l1l111_opy_, bstack11ll1l11_opy_))
-    if bstack1ll1_opy_ (u"ࠩࡥࡶࡴࡽࡳࡦࡴࡑࡥࡲ࡫ࠧ଎") in caps:
-      caps[bstack1ll1_opy_ (u"ࠪࡦࡷࡵࡷࡴࡧࡵࠫଏ")] = caps[bstack1ll1_opy_ (u"ࠫࡧࡸ࡯ࡸࡵࡨࡶࡓࡧ࡭ࡦࠩଐ")]
-      del(caps[bstack1ll1_opy_ (u"ࠬࡨࡲࡰࡹࡶࡩࡷࡔࡡ࡮ࡧࠪ଑")])
-    if bstack1ll1_opy_ (u"࠭ࡢࡳࡱࡺࡷࡪࡸࡖࡦࡴࡶ࡭ࡴࡴࠧ଒") in caps:
-      caps[bstack1ll1_opy_ (u"ࠧࡣࡴࡲࡻࡸ࡫ࡲࡠࡸࡨࡶࡸ࡯࡯࡯ࠩଓ")] = caps[bstack1ll1_opy_ (u"ࠨࡤࡵࡳࡼࡹࡥࡳࡘࡨࡶࡸ࡯࡯࡯ࠩଔ")]
-      del(caps[bstack1ll1_opy_ (u"ࠩࡥࡶࡴࡽࡳࡦࡴ࡙ࡩࡷࡹࡩࡰࡰࠪକ")])
+    bstack11l1111l_opy_[bstack11_opy_ (u"ࠬࡻࡳࡦ࡙࠶ࡇࠬଦ")] = False
+    caps.update(bstack1l111l_opy_(bstack11l1111l_opy_, bstack11l111_opy_))
+    if bstack11_opy_ (u"࠭ࡢࡳࡱࡺࡷࡪࡸࡎࡢ࡯ࡨࠫଧ") in caps:
+      caps[bstack11_opy_ (u"ࠧࡣࡴࡲࡻࡸ࡫ࡲࠨନ")] = caps[bstack11_opy_ (u"ࠨࡤࡵࡳࡼࡹࡥࡳࡐࡤࡱࡪ࠭଩")]
+      del(caps[bstack11_opy_ (u"ࠩࡥࡶࡴࡽࡳࡦࡴࡑࡥࡲ࡫ࠧପ")])
+    if bstack11_opy_ (u"ࠪࡦࡷࡵࡷࡴࡧࡵ࡚ࡪࡸࡳࡪࡱࡱࠫଫ") in caps:
+      caps[bstack11_opy_ (u"ࠫࡧࡸ࡯ࡸࡵࡨࡶࡤࡼࡥࡳࡵ࡬ࡳࡳ࠭ବ")] = caps[bstack11_opy_ (u"ࠬࡨࡲࡰࡹࡶࡩࡷ࡜ࡥࡳࡵ࡬ࡳࡳ࠭ଭ")]
+      del(caps[bstack11_opy_ (u"࠭ࡢࡳࡱࡺࡷࡪࡸࡖࡦࡴࡶ࡭ࡴࡴࠧମ")])
   return caps
-def bstack1l1l11ll_opy_():
-  if bstack1ll1llll_opy_() <= version.parse(bstack1ll1_opy_ (u"ࠪ࠷࠳࠷࠳࠯࠲ࠪଖ")):
-    return bstack1l1ll111l_opy_
-  return bstack11lll1_opy_
-def bstack11l1lll1_opy_(options):
-  return hasattr(options, bstack1ll1_opy_ (u"ࠫࡸ࡫ࡴࡠࡥࡤࡴࡦࡨࡩ࡭࡫ࡷࡽࠬଗ"))
+def bstack11l1ll11_opy_():
+  global bstack1l1ll11_opy_
+  if bstack1ll11l1ll_opy_() <= version.parse(bstack11_opy_ (u"ࠧ࠴࠰࠴࠷࠳࠶ࠧଯ")):
+    if bstack1l1ll11_opy_ != bstack11_opy_ (u"ࠨࠩର"):
+      return bstack11_opy_ (u"ࠤ࡫ࡸࡹࡶ࠺࠰࠱ࠥ଱") + bstack1l1ll11_opy_ + bstack11_opy_ (u"ࠥ࠾࠽࠶࠯ࡸࡦ࠲࡬ࡺࡨࠢଲ")
+    return bstack111l111_opy_
+  if  bstack1l1ll11_opy_ != bstack11_opy_ (u"ࠫࠬଳ"):
+    return bstack11_opy_ (u"ࠧ࡮ࡴࡵࡲࡶ࠾࠴࠵ࠢ଴") + bstack1l1ll11_opy_ + bstack11_opy_ (u"ࠨ࠯ࡸࡦ࠲࡬ࡺࡨࠢଵ")
+  return bstack1lll11111_opy_
+def bstack11111111_opy_(options):
+  return hasattr(options, bstack11_opy_ (u"ࠧࡴࡧࡷࡣࡨࡧࡰࡢࡤ࡬ࡰ࡮ࡺࡹࠨଶ"))
 def update(d, u):
   for k, v in u.items():
     if isinstance(v, collections.abc.Mapping):
       d[k] = update(d.get(k, {}), v)
     else:
       if isinstance(v, list):
         d[k] = d.get(k, []) + v
       else:
         d[k] = v
   return d
-def bstack1llll1l1l_opy_(options, bstack1l11ll11l_opy_):
-  for bstack1llllll_opy_ in bstack1l11ll11l_opy_:
-    if bstack1llllll_opy_ in [bstack1ll1_opy_ (u"ࠬࡧࡲࡨࡵࠪଘ"), bstack1ll1_opy_ (u"࠭ࡥࡹࡶࡨࡲࡸ࡯࡯࡯ࡵࠪଙ")]:
+def bstack1l1l1llll_opy_(options, bstack1l11lllll_opy_):
+  for bstack11l1ll1_opy_ in bstack1l11lllll_opy_:
+    if bstack11l1ll1_opy_ in [bstack11_opy_ (u"ࠨࡣࡵ࡫ࡸ࠭ଷ"), bstack11_opy_ (u"ࠩࡨࡼࡹ࡫࡮ࡴ࡫ࡲࡲࡸ࠭ସ")]:
       next
-    if bstack1llllll_opy_ in options._experimental_options:
-      options._experimental_options[bstack1llllll_opy_]= update(options._experimental_options[bstack1llllll_opy_], bstack1l11ll11l_opy_[bstack1llllll_opy_])
+    if bstack11l1ll1_opy_ in options._experimental_options:
+      options._experimental_options[bstack11l1ll1_opy_]= update(options._experimental_options[bstack11l1ll1_opy_], bstack1l11lllll_opy_[bstack11l1ll1_opy_])
     else:
-      options.add_experimental_option(bstack1llllll_opy_, bstack1l11ll11l_opy_[bstack1llllll_opy_])
-  if bstack1ll1_opy_ (u"ࠧࡢࡴࡪࡷࠬଚ") in bstack1l11ll11l_opy_:
-    for arg in bstack1l11ll11l_opy_[bstack1ll1_opy_ (u"ࠨࡣࡵ࡫ࡸ࠭ଛ")]:
+      options.add_experimental_option(bstack11l1ll1_opy_, bstack1l11lllll_opy_[bstack11l1ll1_opy_])
+  if bstack11_opy_ (u"ࠪࡥࡷ࡭ࡳࠨହ") in bstack1l11lllll_opy_:
+    for arg in bstack1l11lllll_opy_[bstack11_opy_ (u"ࠫࡦࡸࡧࡴࠩ଺")]:
       options.add_argument(arg)
-    del(bstack1l11ll11l_opy_[bstack1ll1_opy_ (u"ࠩࡤࡶ࡬ࡹࠧଜ")])
-  if bstack1ll1_opy_ (u"ࠪࡩࡽࡺࡥ࡯ࡵ࡬ࡳࡳࡹࠧଝ") in bstack1l11ll11l_opy_:
-    for ext in bstack1l11ll11l_opy_[bstack1ll1_opy_ (u"ࠫࡪࡾࡴࡦࡰࡶ࡭ࡴࡴࡳࠨଞ")]:
+    del(bstack1l11lllll_opy_[bstack11_opy_ (u"ࠬࡧࡲࡨࡵࠪ଻")])
+  if bstack11_opy_ (u"࠭ࡥࡹࡶࡨࡲࡸ࡯࡯࡯ࡵ଼ࠪ") in bstack1l11lllll_opy_:
+    for ext in bstack1l11lllll_opy_[bstack11_opy_ (u"ࠧࡦࡺࡷࡩࡳࡹࡩࡰࡰࡶࠫଽ")]:
       options.add_extension(ext)
-    del(bstack1l11ll11l_opy_[bstack1ll1_opy_ (u"ࠬ࡫ࡸࡵࡧࡱࡷ࡮ࡵ࡮ࡴࠩଟ")])
-def bstack1llll1l1_opy_(options, bstack11l111l_opy_):
-  if bstack1ll1_opy_ (u"࠭ࡰࡳࡧࡩࡷࠬଠ") in bstack11l111l_opy_:
-    for bstack1ll1lll1l_opy_ in bstack11l111l_opy_[bstack1ll1_opy_ (u"ࠧࡱࡴࡨࡪࡸ࠭ଡ")]:
-      if bstack1ll1lll1l_opy_ in options._preferences:
-        options._preferences[bstack1ll1lll1l_opy_] = update(options._preferences[bstack1ll1lll1l_opy_], bstack11l111l_opy_[bstack1ll1_opy_ (u"ࠨࡲࡵࡩ࡫ࡹࠧଢ")][bstack1ll1lll1l_opy_])
+    del(bstack1l11lllll_opy_[bstack11_opy_ (u"ࠨࡧࡻࡸࡪࡴࡳࡪࡱࡱࡷࠬା")])
+def bstack11lll1ll_opy_(options, bstack1l1ll1_opy_):
+  if bstack11_opy_ (u"ࠩࡳࡶࡪ࡬ࡳࠨି") in bstack1l1ll1_opy_:
+    for bstack111l1111_opy_ in bstack1l1ll1_opy_[bstack11_opy_ (u"ࠪࡴࡷ࡫ࡦࡴࠩୀ")]:
+      if bstack111l1111_opy_ in options._preferences:
+        options._preferences[bstack111l1111_opy_] = update(options._preferences[bstack111l1111_opy_], bstack1l1ll1_opy_[bstack11_opy_ (u"ࠫࡵࡸࡥࡧࡵࠪୁ")][bstack111l1111_opy_])
       else:
-        options.set_preference(bstack1ll1lll1l_opy_, bstack11l111l_opy_[bstack1ll1_opy_ (u"ࠩࡳࡶࡪ࡬ࡳࠨଣ")][bstack1ll1lll1l_opy_])
-  if bstack1ll1_opy_ (u"ࠪࡥࡷ࡭ࡳࠨତ") in bstack11l111l_opy_:
-    for arg in bstack11l111l_opy_[bstack1ll1_opy_ (u"ࠫࡦࡸࡧࡴࠩଥ")]:
+        options.set_preference(bstack111l1111_opy_, bstack1l1ll1_opy_[bstack11_opy_ (u"ࠬࡶࡲࡦࡨࡶࠫୂ")][bstack111l1111_opy_])
+  if bstack11_opy_ (u"࠭ࡡࡳࡩࡶࠫୃ") in bstack1l1ll1_opy_:
+    for arg in bstack1l1ll1_opy_[bstack11_opy_ (u"ࠧࡢࡴࡪࡷࠬୄ")]:
       options.add_argument(arg)
-def bstack1lll1ll1l_opy_(options, bstack111l1l1l_opy_):
-  if bstack1ll1_opy_ (u"ࠬࡽࡥࡣࡸ࡬ࡩࡼ࠭ଦ") in bstack111l1l1l_opy_:
-    options.use_webview(bool(bstack111l1l1l_opy_[bstack1ll1_opy_ (u"࠭ࡷࡦࡤࡹ࡭ࡪࡽࠧଧ")]))
-  bstack1llll1l1l_opy_(options, bstack111l1l1l_opy_)
-def bstack1ll11l1l_opy_(options, bstack1lll11l1_opy_):
-  for bstack11l1l_opy_ in bstack1lll11l1_opy_:
-    if bstack11l1l_opy_ in [bstack1ll1_opy_ (u"ࠧࡵࡧࡦ࡬ࡳࡵ࡬ࡰࡩࡼࡔࡷ࡫ࡶࡪࡧࡺࠫନ"), bstack1ll1_opy_ (u"ࠨࡣࡵ࡫ࡸ࠭଩")]:
+def bstack1ll1l1ll_opy_(options, bstack11lll1_opy_):
+  if bstack11_opy_ (u"ࠨࡹࡨࡦࡻ࡯ࡥࡸࠩ୅") in bstack11lll1_opy_:
+    options.use_webview(bool(bstack11lll1_opy_[bstack11_opy_ (u"ࠩࡺࡩࡧࡼࡩࡦࡹࠪ୆")]))
+  bstack1l1l1llll_opy_(options, bstack11lll1_opy_)
+def bstack1lllll11l_opy_(options, bstack1l1lll_opy_):
+  for bstack1l1111l_opy_ in bstack1l1lll_opy_:
+    if bstack1l1111l_opy_ in [bstack11_opy_ (u"ࠪࡸࡪࡩࡨ࡯ࡱ࡯ࡳ࡬ࡿࡐࡳࡧࡹ࡭ࡪࡽࠧେ"), bstack11_opy_ (u"ࠫࡦࡸࡧࡴࠩୈ")]:
       next
-    options.set_capability(bstack11l1l_opy_, bstack1lll11l1_opy_[bstack11l1l_opy_])
-  if bstack1ll1_opy_ (u"ࠩࡤࡶ࡬ࡹࠧପ") in bstack1lll11l1_opy_:
-    for arg in bstack1lll11l1_opy_[bstack1ll1_opy_ (u"ࠪࡥࡷ࡭ࡳࠨଫ")]:
+    options.set_capability(bstack1l1111l_opy_, bstack1l1lll_opy_[bstack1l1111l_opy_])
+  if bstack11_opy_ (u"ࠬࡧࡲࡨࡵࠪ୉") in bstack1l1lll_opy_:
+    for arg in bstack1l1lll_opy_[bstack11_opy_ (u"࠭ࡡࡳࡩࡶࠫ୊")]:
       options.add_argument(arg)
-  if bstack1ll1_opy_ (u"ࠫࡹ࡫ࡣࡩࡰࡲࡰࡴ࡭ࡹࡑࡴࡨࡺ࡮࡫ࡷࠨବ") in bstack1lll11l1_opy_:
-    options.use_technology_preview(bool(bstack1lll11l1_opy_[bstack1ll1_opy_ (u"ࠬࡺࡥࡤࡪࡱࡳࡱࡵࡧࡺࡒࡵࡩࡻ࡯ࡥࡸࠩଭ")]))
-def bstack1l1ll1l1_opy_(options, bstack111l111_opy_):
-  for bstack1ll1111ll_opy_ in bstack111l111_opy_:
-    if bstack1ll1111ll_opy_ in [bstack1ll1_opy_ (u"࠭ࡡࡥࡦ࡬ࡸ࡮ࡵ࡮ࡢ࡮ࡒࡴࡹ࡯࡯࡯ࡵࠪମ"), bstack1ll1_opy_ (u"ࠧࡢࡴࡪࡷࠬଯ")]:
+  if bstack11_opy_ (u"ࠧࡵࡧࡦ࡬ࡳࡵ࡬ࡰࡩࡼࡔࡷ࡫ࡶࡪࡧࡺࠫୋ") in bstack1l1lll_opy_:
+    options.use_technology_preview(bool(bstack1l1lll_opy_[bstack11_opy_ (u"ࠨࡶࡨࡧ࡭ࡴ࡯࡭ࡱࡪࡽࡕࡸࡥࡷ࡫ࡨࡻࠬୌ")]))
+def bstack1ll11lll_opy_(options, bstack1111llll_opy_):
+  for bstack11l1l1l_opy_ in bstack1111llll_opy_:
+    if bstack11l1l1l_opy_ in [bstack11_opy_ (u"ࠩࡤࡨࡩ࡯ࡴࡪࡱࡱࡥࡱࡕࡰࡵ࡫ࡲࡲࡸ୍࠭"), bstack11_opy_ (u"ࠪࡥࡷ࡭ࡳࠨ୎")]:
       next
-    options._options[bstack1ll1111ll_opy_] = bstack111l111_opy_[bstack1ll1111ll_opy_]
-  if bstack1ll1_opy_ (u"ࠨࡣࡧࡨ࡮ࡺࡩࡰࡰࡤࡰࡔࡶࡴࡪࡱࡱࡷࠬର") in bstack111l111_opy_:
-    for bstack1l111lll_opy_ in bstack111l111_opy_[bstack1ll1_opy_ (u"ࠩࡤࡨࡩ࡯ࡴࡪࡱࡱࡥࡱࡕࡰࡵ࡫ࡲࡲࡸ࠭଱")]:
+    options._options[bstack11l1l1l_opy_] = bstack1111llll_opy_[bstack11l1l1l_opy_]
+  if bstack11_opy_ (u"ࠫࡦࡪࡤࡪࡶ࡬ࡳࡳࡧ࡬ࡐࡲࡷ࡭ࡴࡴࡳࠨ୏") in bstack1111llll_opy_:
+    for bstack1l1lll1_opy_ in bstack1111llll_opy_[bstack11_opy_ (u"ࠬࡧࡤࡥ࡫ࡷ࡭ࡴࡴࡡ࡭ࡑࡳࡸ࡮ࡵ࡮ࡴࠩ୐")]:
       options.add_additional_option(
-          bstack1l111lll_opy_, bstack111l111_opy_[bstack1ll1_opy_ (u"ࠪࡥࡩࡪࡩࡵ࡫ࡲࡲࡦࡲࡏࡱࡶ࡬ࡳࡳࡹࠧଲ")][bstack1l111lll_opy_])
-  if bstack1ll1_opy_ (u"ࠫࡦࡸࡧࡴࠩଳ") in bstack111l111_opy_:
-    for arg in bstack111l111_opy_[bstack1ll1_opy_ (u"ࠬࡧࡲࡨࡵࠪ଴")]:
+          bstack1l1lll1_opy_, bstack1111llll_opy_[bstack11_opy_ (u"࠭ࡡࡥࡦ࡬ࡸ࡮ࡵ࡮ࡢ࡮ࡒࡴࡹ࡯࡯࡯ࡵࠪ୑")][bstack1l1lll1_opy_])
+  if bstack11_opy_ (u"ࠧࡢࡴࡪࡷࠬ୒") in bstack1111llll_opy_:
+    for arg in bstack1111llll_opy_[bstack11_opy_ (u"ࠨࡣࡵ࡫ࡸ࠭୓")]:
       options.add_argument(arg)
-def bstack1l11ll111_opy_(options, caps):
-  if not hasattr(options, bstack1ll1_opy_ (u"࠭ࡋࡆ࡛ࠪଵ")):
+def bstack1l11lll1_opy_(options, caps):
+  if not hasattr(options, bstack11_opy_ (u"ࠩࡎࡉ࡞࠭୔")):
     return
-  if options.KEY == bstack1ll1_opy_ (u"ࠧࡨࡱࡲ࡫࠿ࡩࡨࡳࡱࡰࡩࡔࡶࡴࡪࡱࡱࡷࠬଶ") and options.KEY in caps:
-    bstack1llll1l1l_opy_(options, caps[bstack1ll1_opy_ (u"ࠨࡩࡲࡳ࡬ࡀࡣࡩࡴࡲࡱࡪࡕࡰࡵ࡫ࡲࡲࡸ࠭ଷ")])
-  elif options.KEY == bstack1ll1_opy_ (u"ࠩࡰࡳࡿࡀࡦࡪࡴࡨࡪࡴࡾࡏࡱࡶ࡬ࡳࡳࡹࠧସ") and options.KEY in caps:
-    bstack1llll1l1_opy_(options, caps[bstack1ll1_opy_ (u"ࠪࡱࡴࢀ࠺ࡧ࡫ࡵࡩ࡫ࡵࡸࡐࡲࡷ࡭ࡴࡴࡳࠨହ")])
-  elif options.KEY == bstack1ll1_opy_ (u"ࠫࡸࡧࡦࡢࡴ࡬࠲ࡴࡶࡴࡪࡱࡱࡷࠬ଺") and options.KEY in caps:
-    bstack1ll11l1l_opy_(options, caps[bstack1ll1_opy_ (u"ࠬࡹࡡࡧࡣࡵ࡭࠳ࡵࡰࡵ࡫ࡲࡲࡸ࠭଻")])
-  elif options.KEY == bstack1ll1_opy_ (u"࠭࡭ࡴ࠼ࡨࡨ࡬࡫ࡏࡱࡶ࡬ࡳࡳࡹ଼ࠧ") and options.KEY in caps:
-    bstack1lll1ll1l_opy_(options, caps[bstack1ll1_opy_ (u"ࠧ࡮ࡵ࠽ࡩࡩ࡭ࡥࡐࡲࡷ࡭ࡴࡴࡳࠨଽ")])
-  elif options.KEY == bstack1ll1_opy_ (u"ࠨࡵࡨ࠾࡮࡫ࡏࡱࡶ࡬ࡳࡳࡹࠧା") and options.KEY in caps:
-    bstack1l1ll1l1_opy_(options, caps[bstack1ll1_opy_ (u"ࠩࡶࡩ࠿࡯ࡥࡐࡲࡷ࡭ࡴࡴࡳࠨି")])
-def bstack11l11ll_opy_(caps):
-  global bstack1ll11111l_opy_
-  if bstack1ll11111l_opy_:
-    if bstack1lllll1_opy_() < version.parse(bstack1ll1_opy_ (u"ࠪ࠶࠳࠹࠮࠱ࠩୀ")):
+  if options.KEY == bstack11_opy_ (u"ࠪ࡫ࡴࡵࡧ࠻ࡥ࡫ࡶࡴࡳࡥࡐࡲࡷ࡭ࡴࡴࡳࠨ୕") and options.KEY in caps:
+    bstack1l1l1llll_opy_(options, caps[bstack11_opy_ (u"ࠫ࡬ࡵ࡯ࡨ࠼ࡦ࡬ࡷࡵ࡭ࡦࡑࡳࡸ࡮ࡵ࡮ࡴࠩୖ")])
+  elif options.KEY == bstack11_opy_ (u"ࠬࡳ࡯ࡻ࠼ࡩ࡭ࡷ࡫ࡦࡰࡺࡒࡴࡹ࡯࡯࡯ࡵࠪୗ") and options.KEY in caps:
+    bstack11lll1ll_opy_(options, caps[bstack11_opy_ (u"࠭࡭ࡰࡼ࠽ࡪ࡮ࡸࡥࡧࡱࡻࡓࡵࡺࡩࡰࡰࡶࠫ୘")])
+  elif options.KEY == bstack11_opy_ (u"ࠧࡴࡣࡩࡥࡷ࡯࠮ࡰࡲࡷ࡭ࡴࡴࡳࠨ୙") and options.KEY in caps:
+    bstack1lllll11l_opy_(options, caps[bstack11_opy_ (u"ࠨࡵࡤࡪࡦࡸࡩ࠯ࡱࡳࡸ࡮ࡵ࡮ࡴࠩ୚")])
+  elif options.KEY == bstack11_opy_ (u"ࠩࡰࡷ࠿࡫ࡤࡨࡧࡒࡴࡹ࡯࡯࡯ࡵࠪ୛") and options.KEY in caps:
+    bstack1ll1l1ll_opy_(options, caps[bstack11_opy_ (u"ࠪࡱࡸࡀࡥࡥࡩࡨࡓࡵࡺࡩࡰࡰࡶࠫଡ଼")])
+  elif options.KEY == bstack11_opy_ (u"ࠫࡸ࡫࠺ࡪࡧࡒࡴࡹ࡯࡯࡯ࡵࠪଢ଼") and options.KEY in caps:
+    bstack1ll11lll_opy_(options, caps[bstack11_opy_ (u"ࠬࡹࡥ࠻࡫ࡨࡓࡵࡺࡩࡰࡰࡶࠫ୞")])
+def bstack1ll11l1l_opy_(caps):
+  global bstack1llll1l_opy_
+  if bstack1llll1l_opy_:
+    if bstack1l111ll1l_opy_() < version.parse(bstack11_opy_ (u"࠭࠲࠯࠵࠱࠴ࠬୟ")):
       return None
     else:
       from appium.options.common.base import AppiumOptions
       options = AppiumOptions().load_capabilities(caps)
       return options
   else:
-    browser = bstack1ll1_opy_ (u"ࠫࡨ࡮ࡲࡰ࡯ࡨࠫୁ")
-    if bstack1ll1_opy_ (u"ࠬࡨࡲࡰࡹࡶࡩࡷࡔࡡ࡮ࡧࠪୂ") in caps:
-      browser = caps[bstack1ll1_opy_ (u"࠭ࡢࡳࡱࡺࡷࡪࡸࡎࡢ࡯ࡨࠫୃ")]
-    elif bstack1ll1_opy_ (u"ࠧࡣࡴࡲࡻࡸ࡫ࡲࠨୄ") in caps:
-      browser = caps[bstack1ll1_opy_ (u"ࠨࡤࡵࡳࡼࡹࡥࡳࠩ୅")]
+    browser = bstack11_opy_ (u"ࠧࡤࡪࡵࡳࡲ࡫ࠧୠ")
+    if bstack11_opy_ (u"ࠨࡤࡵࡳࡼࡹࡥࡳࡐࡤࡱࡪ࠭ୡ") in caps:
+      browser = caps[bstack11_opy_ (u"ࠩࡥࡶࡴࡽࡳࡦࡴࡑࡥࡲ࡫ࠧୢ")]
+    elif bstack11_opy_ (u"ࠪࡦࡷࡵࡷࡴࡧࡵࠫୣ") in caps:
+      browser = caps[bstack11_opy_ (u"ࠫࡧࡸ࡯ࡸࡵࡨࡶࠬ୤")]
     browser = str(browser).lower()
-    if browser == bstack1ll1_opy_ (u"ࠩ࡬ࡴ࡭ࡵ࡮ࡦࠩ୆") or browser == bstack1ll1_opy_ (u"ࠪ࡭ࡵࡧࡤࠨେ"):
-      browser = bstack1ll1_opy_ (u"ࠫࡸࡧࡦࡢࡴ࡬ࠫୈ")
-    if browser == bstack1ll1_opy_ (u"ࠬࡹࡡ࡮ࡵࡸࡲ࡬࠭୉"):
-      browser = bstack1ll1_opy_ (u"࠭ࡣࡩࡴࡲࡱࡪ࠭୊")
-    if browser not in [bstack1ll1_opy_ (u"ࠧࡤࡪࡵࡳࡲ࡫ࠧୋ"), bstack1ll1_opy_ (u"ࠨࡧࡧ࡫ࡪ࠭ୌ"), bstack1ll1_opy_ (u"ࠩ࡬ࡩ୍ࠬ"), bstack1ll1_opy_ (u"ࠪࡷࡦ࡬ࡡࡳ࡫ࠪ୎"), bstack1ll1_opy_ (u"ࠫ࡫࡯ࡲࡦࡨࡲࡼࠬ୏")]:
+    if browser == bstack11_opy_ (u"ࠬ࡯ࡰࡩࡱࡱࡩࠬ୥") or browser == bstack11_opy_ (u"࠭ࡩࡱࡣࡧࠫ୦"):
+      browser = bstack11_opy_ (u"ࠧࡴࡣࡩࡥࡷ࡯ࠧ୧")
+    if browser == bstack11_opy_ (u"ࠨࡵࡤࡱࡸࡻ࡮ࡨࠩ୨"):
+      browser = bstack11_opy_ (u"ࠩࡦ࡬ࡷࡵ࡭ࡦࠩ୩")
+    if browser not in [bstack11_opy_ (u"ࠪࡧ࡭ࡸ࡯࡮ࡧࠪ୪"), bstack11_opy_ (u"ࠫࡪࡪࡧࡦࠩ୫"), bstack11_opy_ (u"ࠬ࡯ࡥࠨ୬"), bstack11_opy_ (u"࠭ࡳࡢࡨࡤࡶ࡮࠭୭"), bstack11_opy_ (u"ࠧࡧ࡫ࡵࡩ࡫ࡵࡸࠨ୮")]:
       return None
     try:
-      package = bstack1ll1_opy_ (u"ࠬࡹࡥ࡭ࡧࡱ࡭ࡺࡳ࠮ࡸࡧࡥࡨࡷ࡯ࡶࡦࡴ࠱ࡿࢂ࠴࡯ࡱࡶ࡬ࡳࡳࡹࠧ୐").format(browser)
-      name = bstack1ll1_opy_ (u"࠭ࡏࡱࡶ࡬ࡳࡳࡹࠧ୑")
+      package = bstack11_opy_ (u"ࠨࡵࡨࡰࡪࡴࡩࡶ࡯࠱ࡻࡪࡨࡤࡳ࡫ࡹࡩࡷ࠴ࡻࡾ࠰ࡲࡴࡹ࡯࡯࡯ࡵࠪ୯").format(browser)
+      name = bstack11_opy_ (u"ࠩࡒࡴࡹ࡯࡯࡯ࡵࠪ୰")
       browser_options = getattr(__import__(package, fromlist=[name]), name)
       options = browser_options()
-      if not bstack11l1lll1_opy_(options):
+      if not bstack11111111_opy_(options):
         return None
-      for bstack1lllll1l1_opy_ in caps.keys():
-        options.set_capability(bstack1lllll1l1_opy_, caps[bstack1lllll1l1_opy_])
-      bstack1l11ll111_opy_(options, caps)
+      for bstack1llll1ll1_opy_ in caps.keys():
+        options.set_capability(bstack1llll1ll1_opy_, caps[bstack1llll1ll1_opy_])
+      bstack1l11lll1_opy_(options, caps)
       return options
     except Exception as e:
       logger.debug(str(e))
       return None
-def bstack1llllllll_opy_(options, bstack11l1l1l1_opy_):
-  if not bstack11l1lll1_opy_(options):
+def bstack1llll1111_opy_(options, bstack1lll11l_opy_):
+  if not bstack11111111_opy_(options):
     return
-  for bstack1lllll1l1_opy_ in bstack11l1l1l1_opy_.keys():
-    if bstack1lllll1l1_opy_ in bstack11111l11_opy_:
+  for bstack1llll1ll1_opy_ in bstack1lll11l_opy_.keys():
+    if bstack1llll1ll1_opy_ in bstack1l111l11_opy_:
       next
-    if bstack1lllll1l1_opy_ in options._caps and type(options._caps[bstack1lllll1l1_opy_]) in [dict, list]:
-      options._caps[bstack1lllll1l1_opy_] = update(options._caps[bstack1lllll1l1_opy_], bstack11l1l1l1_opy_[bstack1lllll1l1_opy_])
+    if bstack1llll1ll1_opy_ in options._caps and type(options._caps[bstack1llll1ll1_opy_]) in [dict, list]:
+      options._caps[bstack1llll1ll1_opy_] = update(options._caps[bstack1llll1ll1_opy_], bstack1lll11l_opy_[bstack1llll1ll1_opy_])
     else:
-      options.set_capability(bstack1lllll1l1_opy_, bstack11l1l1l1_opy_[bstack1lllll1l1_opy_])
-  bstack1l11ll111_opy_(options, bstack11l1l1l1_opy_)
-  if bstack1ll1_opy_ (u"ࠧ࡮ࡱࡽ࠾ࡩ࡫ࡢࡶࡩࡪࡩࡷࡇࡤࡥࡴࡨࡷࡸ࠭୒") in options._caps:
-    if options._caps[bstack1ll1_opy_ (u"ࠨࡤࡵࡳࡼࡹࡥࡳࡐࡤࡱࡪ࠭୓")] and options._caps[bstack1ll1_opy_ (u"ࠩࡥࡶࡴࡽࡳࡦࡴࡑࡥࡲ࡫ࠧ୔")].lower() != bstack1ll1_opy_ (u"ࠪࡪ࡮ࡸࡥࡧࡱࡻࠫ୕"):
-      del options._caps[bstack1ll1_opy_ (u"ࠫࡲࡵࡺ࠻ࡦࡨࡦࡺ࡭ࡧࡦࡴࡄࡨࡩࡸࡥࡴࡵࠪୖ")]
-def bstack1l11lll_opy_(proxy_config):
-  if bstack1ll1_opy_ (u"ࠬ࡮ࡴࡵࡲࡶࡔࡷࡵࡸࡺࠩୗ") in proxy_config:
-    proxy_config[bstack1ll1_opy_ (u"࠭ࡳࡴ࡮ࡓࡶࡴࡾࡹࠨ୘")] = proxy_config[bstack1ll1_opy_ (u"ࠧࡩࡶࡷࡴࡸࡖࡲࡰࡺࡼࠫ୙")]
-    del(proxy_config[bstack1ll1_opy_ (u"ࠨࡪࡷࡸࡵࡹࡐࡳࡱࡻࡽࠬ୚")])
-  if bstack1ll1_opy_ (u"ࠩࡳࡶࡴࡾࡹࡕࡻࡳࡩࠬ୛") in proxy_config and proxy_config[bstack1ll1_opy_ (u"ࠪࡴࡷࡵࡸࡺࡖࡼࡴࡪ࠭ଡ଼")].lower() != bstack1ll1_opy_ (u"ࠫࡩ࡯ࡲࡦࡥࡷࠫଢ଼"):
-    proxy_config[bstack1ll1_opy_ (u"ࠬࡶࡲࡰࡺࡼࡘࡾࡶࡥࠨ୞")] = bstack1ll1_opy_ (u"࠭࡭ࡢࡰࡸࡥࡱ࠭ୟ")
-  if bstack1ll1_opy_ (u"ࠧࡱࡴࡲࡼࡾࡇࡵࡵࡱࡦࡳࡳ࡬ࡩࡨࡗࡵࡰࠬୠ") in proxy_config:
-    proxy_config[bstack1ll1_opy_ (u"ࠨࡲࡵࡳࡽࡿࡔࡺࡲࡨࠫୡ")] = bstack1ll1_opy_ (u"ࠩࡳࡥࡨ࠭ୢ")
+      options.set_capability(bstack1llll1ll1_opy_, bstack1lll11l_opy_[bstack1llll1ll1_opy_])
+  bstack1l11lll1_opy_(options, bstack1lll11l_opy_)
+  if bstack11_opy_ (u"ࠪࡱࡴࢀ࠺ࡥࡧࡥࡹ࡬࡭ࡥࡳࡃࡧࡨࡷ࡫ࡳࡴࠩୱ") in options._caps:
+    if options._caps[bstack11_opy_ (u"ࠫࡧࡸ࡯ࡸࡵࡨࡶࡓࡧ࡭ࡦࠩ୲")] and options._caps[bstack11_opy_ (u"ࠬࡨࡲࡰࡹࡶࡩࡷࡔࡡ࡮ࡧࠪ୳")].lower() != bstack11_opy_ (u"࠭ࡦࡪࡴࡨࡪࡴࡾࠧ୴"):
+      del options._caps[bstack11_opy_ (u"ࠧ࡮ࡱࡽ࠾ࡩ࡫ࡢࡶࡩࡪࡩࡷࡇࡤࡥࡴࡨࡷࡸ࠭୵")]
+def bstack1lll111_opy_(proxy_config):
+  if bstack11_opy_ (u"ࠨࡪࡷࡸࡵࡹࡐࡳࡱࡻࡽࠬ୶") in proxy_config:
+    proxy_config[bstack11_opy_ (u"ࠩࡶࡷࡱࡖࡲࡰࡺࡼࠫ୷")] = proxy_config[bstack11_opy_ (u"ࠪ࡬ࡹࡺࡰࡴࡒࡵࡳࡽࡿࠧ୸")]
+    del(proxy_config[bstack11_opy_ (u"ࠫ࡭ࡺࡴࡱࡵࡓࡶࡴࡾࡹࠨ୹")])
+  if bstack11_opy_ (u"ࠬࡶࡲࡰࡺࡼࡘࡾࡶࡥࠨ୺") in proxy_config and proxy_config[bstack11_opy_ (u"࠭ࡰࡳࡱࡻࡽ࡙ࡿࡰࡦࠩ୻")].lower() != bstack11_opy_ (u"ࠧࡥ࡫ࡵࡩࡨࡺࠧ୼"):
+    proxy_config[bstack11_opy_ (u"ࠨࡲࡵࡳࡽࡿࡔࡺࡲࡨࠫ୽")] = bstack11_opy_ (u"ࠩࡰࡥࡳࡻࡡ࡭ࠩ୾")
+  if bstack11_opy_ (u"ࠪࡴࡷࡵࡸࡺࡃࡸࡸࡴࡩ࡯࡯ࡨ࡬࡫࡚ࡸ࡬ࠨ୿") in proxy_config:
+    proxy_config[bstack11_opy_ (u"ࠫࡵࡸ࡯ࡹࡻࡗࡽࡵ࡫ࠧ஀")] = bstack11_opy_ (u"ࠬࡶࡡࡤࠩ஁")
   return proxy_config
-def bstack1ll1l11l1_opy_(config, proxy):
+def bstack1l11111l_opy_(config, proxy):
   from selenium.webdriver.common.proxy import Proxy
-  if not bstack1ll1_opy_ (u"ࠪࡴࡷࡵࡸࡺࠩୣ") in config:
+  if not bstack11_opy_ (u"࠭ࡰࡳࡱࡻࡽࠬஂ") in config:
     return proxy
-  config[bstack1ll1_opy_ (u"ࠫࡵࡸ࡯ࡹࡻࠪ୤")] = bstack1l11lll_opy_(config[bstack1ll1_opy_ (u"ࠬࡶࡲࡰࡺࡼࠫ୥")])
+  config[bstack11_opy_ (u"ࠧࡱࡴࡲࡼࡾ࠭ஃ")] = bstack1lll111_opy_(config[bstack11_opy_ (u"ࠨࡲࡵࡳࡽࡿࠧ஄")])
   if proxy == None:
-    proxy = Proxy(config[bstack1ll1_opy_ (u"࠭ࡰࡳࡱࡻࡽࠬ୦")])
+    proxy = Proxy(config[bstack11_opy_ (u"ࠩࡳࡶࡴࡾࡹࠨஅ")])
   return proxy
-def bstack111l1ll1_opy_(self):
+def bstack1l1l111l1_opy_(self):
   global CONFIG
-  global bstack111lll1l_opy_
-  if bstack1ll1_opy_ (u"ࠧࡩࡶࡷࡴࡕࡸ࡯ࡹࡻࠪ୧") in CONFIG:
-    return CONFIG[bstack1ll1_opy_ (u"ࠨࡪࡷࡸࡵࡖࡲࡰࡺࡼࠫ୨")]
-  elif bstack1ll1_opy_ (u"ࠩ࡫ࡸࡹࡶࡳࡑࡴࡲࡼࡾ࠭୩") in CONFIG:
-    return CONFIG[bstack1ll1_opy_ (u"ࠪ࡬ࡹࡺࡰࡴࡒࡵࡳࡽࡿࠧ୪")]
+  global bstack111ll_opy_
+  if bstack11_opy_ (u"ࠪ࡬ࡹࡺࡰࡑࡴࡲࡼࡾ࠭ஆ") in CONFIG:
+    return CONFIG[bstack11_opy_ (u"ࠫ࡭ࡺࡴࡱࡒࡵࡳࡽࡿࠧஇ")]
+  elif bstack11_opy_ (u"ࠬ࡮ࡴࡵࡲࡶࡔࡷࡵࡸࡺࠩஈ") in CONFIG:
+    return CONFIG[bstack11_opy_ (u"࠭ࡨࡵࡶࡳࡷࡕࡸ࡯ࡹࡻࠪஉ")]
   else:
-    return bstack111lll1l_opy_(self)
-def bstack11l1l1ll_opy_():
+    return bstack111ll_opy_(self)
+def bstack1111ll1_opy_():
   global CONFIG
-  return bstack1ll1_opy_ (u"ࠫ࡭ࡺࡴࡱࡒࡵࡳࡽࡿࠧ୫") in CONFIG or bstack1ll1_opy_ (u"ࠬ࡮ࡴࡵࡲࡶࡔࡷࡵࡸࡺࠩ୬") in CONFIG
-def bstack111l1111_opy_(config):
-  if not bstack11l1l1ll_opy_():
+  return bstack11_opy_ (u"ࠧࡩࡶࡷࡴࡕࡸ࡯ࡹࡻࠪஊ") in CONFIG or bstack11_opy_ (u"ࠨࡪࡷࡸࡵࡹࡐࡳࡱࡻࡽࠬ஋") in CONFIG
+def bstack1ll11ll1l_opy_(config):
+  if not bstack1111ll1_opy_():
     return
-  if config.get(bstack1ll1_opy_ (u"࠭ࡨࡵࡶࡳࡔࡷࡵࡸࡺࠩ୭")):
-    return config.get(bstack1ll1_opy_ (u"ࠧࡩࡶࡷࡴࡕࡸ࡯ࡹࡻࠪ୮"))
-  if config.get(bstack1ll1_opy_ (u"ࠨࡪࡷࡸࡵࡹࡐࡳࡱࡻࡽࠬ୯")):
-    return config.get(bstack1ll1_opy_ (u"ࠩ࡫ࡸࡹࡶࡳࡑࡴࡲࡼࡾ࠭୰"))
-def bstack1ll1l1ll_opy_():
-  return bstack11l1l1ll_opy_() and bstack1ll1llll_opy_() >= version.parse(bstack1lllll1l_opy_)
-def bstack1ll11l11l_opy_(config):
-  if bstack1ll1_opy_ (u"ࠪࡦࡷࡵࡷࡴࡧࡵࡗࡹࡧࡣ࡬ࡎࡲࡧࡦࡲࡏࡱࡶ࡬ࡳࡳࡹࠧୱ") in config:
-    return config[bstack1ll1_opy_ (u"ࠫࡧࡸ࡯ࡸࡵࡨࡶࡘࡺࡡࡤ࡭ࡏࡳࡨࡧ࡬ࡐࡲࡷ࡭ࡴࡴࡳࠨ୲")]
-  if bstack1ll1_opy_ (u"ࠬࡲ࡯ࡤࡣ࡯ࡓࡵࡺࡩࡰࡰࡶࠫ୳") in config:
-    return config[bstack1ll1_opy_ (u"࠭࡬ࡰࡥࡤࡰࡔࡶࡴࡪࡱࡱࡷࠬ୴")]
+  if config.get(bstack11_opy_ (u"ࠩ࡫ࡸࡹࡶࡐࡳࡱࡻࡽࠬ஌")):
+    return config.get(bstack11_opy_ (u"ࠪ࡬ࡹࡺࡰࡑࡴࡲࡼࡾ࠭஍"))
+  if config.get(bstack11_opy_ (u"ࠫ࡭ࡺࡴࡱࡵࡓࡶࡴࡾࡹࠨஎ")):
+    return config.get(bstack11_opy_ (u"ࠬ࡮ࡴࡵࡲࡶࡔࡷࡵࡸࡺࠩஏ"))
+def bstack1111l1l_opy_():
+  return bstack1111ll1_opy_() and bstack1ll11l1ll_opy_() >= version.parse(bstack1l1ll111_opy_)
+def bstack111lll11_opy_(config):
+  if bstack11_opy_ (u"࠭ࡢࡳࡱࡺࡷࡪࡸࡓࡵࡣࡦ࡯ࡑࡵࡣࡢ࡮ࡒࡴࡹ࡯࡯࡯ࡵࠪஐ") in config:
+    return config[bstack11_opy_ (u"ࠧࡣࡴࡲࡻࡸ࡫ࡲࡔࡶࡤࡧࡰࡒ࡯ࡤࡣ࡯ࡓࡵࡺࡩࡰࡰࡶࠫ஑")]
+  if bstack11_opy_ (u"ࠨ࡮ࡲࡧࡦࡲࡏࡱࡶ࡬ࡳࡳࡹࠧஒ") in config:
+    return config[bstack11_opy_ (u"ࠩ࡯ࡳࡨࡧ࡬ࡐࡲࡷ࡭ࡴࡴࡳࠨஓ")]
   return {}
-def bstack11l1l1l_opy_(caps):
-  global bstack111l1lll_opy_
-  if bstack1ll1_opy_ (u"ࠧࡣࡵࡷࡥࡨࡱ࠺ࡰࡲࡷ࡭ࡴࡴࡳࠨ୵") in caps:
-    caps[bstack1ll1_opy_ (u"ࠨࡤࡶࡸࡦࡩ࡫࠻ࡱࡳࡸ࡮ࡵ࡮ࡴࠩ୶")][bstack1ll1_opy_ (u"ࠩ࡯ࡳࡨࡧ࡬ࠨ୷")] = True
-    if bstack111l1lll_opy_:
-      caps[bstack1ll1_opy_ (u"ࠪࡦࡸࡺࡡࡤ࡭࠽ࡳࡵࡺࡩࡰࡰࡶࠫ୸")][bstack1ll1_opy_ (u"ࠫࡱࡵࡣࡢ࡮ࡌࡨࡪࡴࡴࡪࡨ࡬ࡩࡷ࠭୹")] = bstack111l1lll_opy_
+def bstack1l1lll111_opy_(caps):
+  global bstack1l11l111_opy_
+  if bstack11_opy_ (u"ࠪࡦࡸࡺࡡࡤ࡭࠽ࡳࡵࡺࡩࡰࡰࡶࠫஔ") in caps:
+    caps[bstack11_opy_ (u"ࠫࡧࡹࡴࡢࡥ࡮࠾ࡴࡶࡴࡪࡱࡱࡷࠬக")][bstack11_opy_ (u"ࠬࡲ࡯ࡤࡣ࡯ࠫ஖")] = True
+    if bstack1l11l111_opy_:
+      caps[bstack11_opy_ (u"࠭ࡢࡴࡶࡤࡧࡰࡀ࡯ࡱࡶ࡬ࡳࡳࡹࠧ஗")][bstack11_opy_ (u"ࠧ࡭ࡱࡦࡥࡱࡏࡤࡦࡰࡷ࡭࡫࡯ࡥࡳࠩ஘")] = bstack1l11l111_opy_
   else:
-    caps[bstack1ll1_opy_ (u"ࠬࡨࡲࡰࡹࡶࡩࡷࡹࡴࡢࡥ࡮࠲ࡱࡵࡣࡢ࡮ࠪ୺")] = True
-    if bstack111l1lll_opy_:
-      caps[bstack1ll1_opy_ (u"࠭ࡢࡳࡱࡺࡷࡪࡸࡳࡵࡣࡦ࡯࠳ࡲ࡯ࡤࡣ࡯ࡍࡩ࡫࡮ࡵ࡫ࡩ࡭ࡪࡸࠧ୻")] = bstack111l1lll_opy_
-def bstack1l1l1111l_opy_():
-  global CONFIG
-  if bstack1ll1_opy_ (u"ࠧࡣࡴࡲࡻࡸ࡫ࡲࡴࡶࡤࡧࡰࡒ࡯ࡤࡣ࡯ࠫ୼") in CONFIG and CONFIG[bstack1ll1_opy_ (u"ࠨࡤࡵࡳࡼࡹࡥࡳࡵࡷࡥࡨࡱࡌࡰࡥࡤࡰࠬ୽")]:
-    bstack1ll1ll1_opy_ = bstack1ll11l11l_opy_(CONFIG)
-    bstack1lll1111_opy_(CONFIG[bstack1ll1_opy_ (u"ࠩࡤࡧࡨ࡫ࡳࡴࡍࡨࡽࠬ୾")], bstack1ll1ll1_opy_)
-def bstack1lll1111_opy_(key, bstack1ll1ll1_opy_):
-  global bstack11llll11_opy_
-  logger.info(bstack1l111l1_opy_)
+    caps[bstack11_opy_ (u"ࠨࡤࡵࡳࡼࡹࡥࡳࡵࡷࡥࡨࡱ࠮࡭ࡱࡦࡥࡱ࠭ங")] = True
+    if bstack1l11l111_opy_:
+      caps[bstack11_opy_ (u"ࠩࡥࡶࡴࡽࡳࡦࡴࡶࡸࡦࡩ࡫࠯࡮ࡲࡧࡦࡲࡉࡥࡧࡱࡸ࡮࡬ࡩࡦࡴࠪச")] = bstack1l11l111_opy_
+def bstack1lll11l1_opy_():
+  global CONFIG
+  if bstack11_opy_ (u"ࠪࡦࡷࡵࡷࡴࡧࡵࡷࡹࡧࡣ࡬ࡎࡲࡧࡦࡲࠧ஛") in CONFIG and CONFIG[bstack11_opy_ (u"ࠫࡧࡸ࡯ࡸࡵࡨࡶࡸࡺࡡࡤ࡭ࡏࡳࡨࡧ࡬ࠨஜ")]:
+    bstack1l1llll1l_opy_ = bstack111lll11_opy_(CONFIG)
+    bstack1lll11_opy_(CONFIG[bstack11_opy_ (u"ࠬࡧࡣࡤࡧࡶࡷࡐ࡫ࡹࠨ஝")], bstack1l1llll1l_opy_)
+def bstack1lll11_opy_(key, bstack1l1llll1l_opy_):
+  global bstack111ll11_opy_
+  logger.info(bstack1llllll_opy_)
   try:
-    bstack11llll11_opy_ = Local()
-    bstack11ll_opy_ = {bstack1ll1_opy_ (u"ࠪ࡯ࡪࡿࠧ୿"): key}
-    bstack11ll_opy_.update(bstack1ll1ll1_opy_)
-    logger.debug(bstack11l1ll1l_opy_.format(str(bstack11ll_opy_)))
-    bstack11llll11_opy_.start(**bstack11ll_opy_)
-    if bstack11llll11_opy_.isRunning():
-      logger.info(bstack1ll11ll1_opy_)
+    bstack111ll11_opy_ = Local()
+    bstack1l11ll_opy_ = {bstack11_opy_ (u"࠭࡫ࡦࡻࠪஞ"): key}
+    bstack1l11ll_opy_.update(bstack1l1llll1l_opy_)
+    logger.debug(bstack11l1lll_opy_.format(str(bstack1l11ll_opy_)))
+    bstack111ll11_opy_.start(**bstack1l11ll_opy_)
+    if bstack111ll11_opy_.isRunning():
+      logger.info(bstack1lll111l1_opy_)
   except Exception as e:
-    bstack1ll1lll_opy_(bstack1llll1ll_opy_.format(str(e)))
-def bstack1lllll1ll_opy_():
-  global bstack11llll11_opy_
-  if bstack11llll11_opy_.isRunning():
-    logger.info(bstack1l11l111_opy_)
-    bstack11llll11_opy_.stop()
-  bstack11llll11_opy_ = None
-def bstack1l1l11l1l_opy_():
-  global bstack1l1ll_opy_
-  global bstack111l_opy_
-  if bstack1l1ll_opy_:
-    logger.warning(bstack1111111l_opy_.format(str(bstack1l1ll_opy_)))
-  logger.info(bstack1l11l11l_opy_)
-  global bstack11llll11_opy_
-  if bstack11llll11_opy_:
-    bstack1lllll1ll_opy_()
+    bstack11111l11_opy_(bstack1ll11l11_opy_.format(str(e)))
+def bstack1ll1111l1_opy_():
+  global bstack111ll11_opy_
+  if bstack111ll11_opy_.isRunning():
+    logger.info(bstack1llllll1_opy_)
+    bstack111ll11_opy_.stop()
+  bstack111ll11_opy_ = None
+def bstack1111l_opy_():
+  global bstack11l1l1_opy_
+  global bstack1ll1l1l1_opy_
+  if bstack11l1l1_opy_:
+    logger.warning(bstack1lll11ll1_opy_.format(str(bstack11l1l1_opy_)))
+  logger.info(bstack1l1l11ll1_opy_)
+  global bstack111ll11_opy_
+  if bstack111ll11_opy_:
+    bstack1ll1111l1_opy_()
   try:
-    for driver in bstack111l_opy_:
+    for driver in bstack1ll1l1l1_opy_:
       driver.quit()
   except Exception as e:
     pass
-  logger.info(bstack1l11lllll_opy_)
-  bstack11111l1_opy_()
-def bstack1l1llll11_opy_(self, *args):
-  logger.error(bstack1l1l11l1_opy_)
-  bstack1l1l11l1l_opy_()
+  logger.info(bstack1l1111lll_opy_)
+  bstack1ll1ll1_opy_()
+def bstack1ll11llll_opy_(self, *args):
+  logger.error(bstack1ll1l1l1l_opy_)
+  bstack1111l_opy_()
   sys.exit(1)
-def bstack1ll1lll_opy_(err):
-  logger.critical(bstack111ll11_opy_.format(str(err)))
-  bstack11111l1_opy_(bstack111ll11_opy_.format(str(err)))
-  atexit.unregister(bstack1l1l11l1l_opy_)
+def bstack11111l11_opy_(err):
+  logger.critical(bstack11ll1lll_opy_.format(str(err)))
+  bstack1ll1ll1_opy_(bstack11ll1lll_opy_.format(str(err)))
+  atexit.unregister(bstack1111l_opy_)
   sys.exit(1)
-def bstack11l1_opy_(error, message):
+def bstack111lll1l_opy_(error, message):
   logger.critical(str(error))
   logger.critical(message)
-  bstack11111l1_opy_(message)
-  atexit.unregister(bstack1l1l11l1l_opy_)
+  bstack1ll1ll1_opy_(message)
+  atexit.unregister(bstack1111l_opy_)
   sys.exit(1)
-def bstack1lll1ll11_opy_():
+def bstack111ll1ll_opy_():
   global CONFIG
-  global bstack1111l1l_opy_
-  global bstack1lll1111l_opy_
-  global bstack111lllll_opy_
-  CONFIG = bstack1l1ll1ll_opy_()
-  bstack1lll1ll1_opy_()
-  bstack1l11l_opy_()
-  CONFIG = bstack1ll11lll_opy_(CONFIG)
-  update(CONFIG, bstack1lll1111l_opy_)
-  update(CONFIG, bstack1111l1l_opy_)
-  CONFIG = bstack1ll111lll_opy_(CONFIG)
-  if bstack1ll1_opy_ (u"ࠫࡦࡻࡴࡰ࡯ࡤࡸ࡮ࡵ࡮ࠨ஀") in CONFIG and str(CONFIG[bstack1ll1_opy_ (u"ࠬࡧࡵࡵࡱࡰࡥࡹ࡯࡯࡯ࠩ஁")]).lower() == bstack1ll1_opy_ (u"࠭ࡦࡢ࡮ࡶࡩࠬஂ"):
-    bstack111lllll_opy_ = False
-  if (bstack1ll1_opy_ (u"ࠧࡣࡷ࡬ࡰࡩࡔࡡ࡮ࡧࠪஃ") in CONFIG and bstack1ll1_opy_ (u"ࠨࡤࡸ࡭ࡱࡪࡎࡢ࡯ࡨࠫ஄") in bstack1111l1l_opy_) or (bstack1ll1_opy_ (u"ࠩࡥࡹ࡮ࡲࡤࡏࡣࡰࡩࠬஅ") in CONFIG and bstack1ll1_opy_ (u"ࠪࡦࡺ࡯࡬ࡥࡐࡤࡱࡪ࠭ஆ") not in bstack1lll1111l_opy_):
-    if os.getenv(bstack1ll1_opy_ (u"ࠫࡇ࡙ࡔࡂࡅࡎࡣࡈࡕࡍࡃࡋࡑࡉࡉࡥࡂࡖࡋࡏࡈࡤࡏࡄࠨஇ")):
-      CONFIG[bstack1ll1_opy_ (u"ࠬࡨࡵࡪ࡮ࡧࡍࡩ࡫࡮ࡵ࡫ࡩ࡭ࡪࡸࠧஈ")] = os.getenv(bstack1ll1_opy_ (u"࠭ࡂࡔࡖࡄࡇࡐࡥࡃࡐࡏࡅࡍࡓࡋࡄࡠࡄࡘࡍࡑࡊ࡟ࡊࡆࠪஉ"))
-    else:
-      bstack1l1l1_opy_()
-  elif (bstack1ll1_opy_ (u"ࠧࡣࡷ࡬ࡰࡩࡔࡡ࡮ࡧࠪஊ") not in CONFIG and bstack1ll1_opy_ (u"ࠨࡤࡸ࡭ࡱࡪࡉࡥࡧࡱࡸ࡮࡬ࡩࡦࡴࠪ஋") in CONFIG) or (bstack1ll1_opy_ (u"ࠩࡥࡹ࡮ࡲࡤࡏࡣࡰࡩࠬ஌") in bstack1lll1111l_opy_ and bstack1ll1_opy_ (u"ࠪࡦࡺ࡯࡬ࡥࡐࡤࡱࡪ࠭஍") not in bstack1111l1l_opy_):
-    del(CONFIG[bstack1ll1_opy_ (u"ࠫࡧࡻࡩ࡭ࡦࡌࡨࡪࡴࡴࡪࡨ࡬ࡩࡷ࠭எ")])
-  if bstack1ll1l111l_opy_(CONFIG):
-    bstack1ll1lll_opy_(bstack11l1llll_opy_)
-  bstack11l1ll1_opy_()
-  bstack1ll11llll_opy_()
-  if bstack1ll11111l_opy_:
-    CONFIG[bstack1ll1_opy_ (u"ࠬࡧࡰࡱࠩஏ")] = bstack1l11ll1_opy_(CONFIG)
-    logger.info(bstack1l11l11_opy_.format(CONFIG[bstack1ll1_opy_ (u"࠭ࡡࡱࡲࠪஐ")]))
-def bstack1ll11llll_opy_():
+  global bstack1lll1lll_opy_
+  global bstack1l111_opy_
+  global bstack11llll11_opy_
+  CONFIG = bstack1lll111l_opy_()
+  bstack111l11ll_opy_()
+  bstack1l11l11_opy_()
+  CONFIG = bstack11lllll1_opy_(CONFIG)
+  update(CONFIG, bstack1l111_opy_)
+  update(CONFIG, bstack1lll1lll_opy_)
+  CONFIG = bstack1l11ll1l_opy_(CONFIG)
+  if bstack11_opy_ (u"ࠧࡢࡷࡷࡳࡲࡧࡴࡪࡱࡱࠫட") in CONFIG and str(CONFIG[bstack11_opy_ (u"ࠨࡣࡸࡸࡴࡳࡡࡵ࡫ࡲࡲࠬ஠")]).lower() == bstack11_opy_ (u"ࠩࡩࡥࡱࡹࡥࠨ஡"):
+    bstack11llll11_opy_ = False
+  if (bstack11_opy_ (u"ࠪࡦࡺ࡯࡬ࡥࡐࡤࡱࡪ࠭஢") in CONFIG and bstack11_opy_ (u"ࠫࡧࡻࡩ࡭ࡦࡑࡥࡲ࡫ࠧண") in bstack1lll1lll_opy_) or (bstack11_opy_ (u"ࠬࡨࡵࡪ࡮ࡧࡒࡦࡳࡥࠨத") in CONFIG and bstack11_opy_ (u"࠭ࡢࡶ࡫࡯ࡨࡓࡧ࡭ࡦࠩ஥") not in bstack1l111_opy_):
+    if os.getenv(bstack11_opy_ (u"ࠧࡃࡕࡗࡅࡈࡑ࡟ࡄࡑࡐࡆࡎࡔࡅࡅࡡࡅ࡙ࡎࡒࡄࡠࡋࡇࠫ஦")):
+      CONFIG[bstack11_opy_ (u"ࠨࡤࡸ࡭ࡱࡪࡉࡥࡧࡱࡸ࡮࡬ࡩࡦࡴࠪ஧")] = os.getenv(bstack11_opy_ (u"ࠩࡅࡗ࡙ࡇࡃࡌࡡࡆࡓࡒࡈࡉࡏࡇࡇࡣࡇ࡛ࡉࡍࡆࡢࡍࡉ࠭ந"))
+    else:
+      bstack1ll111l11_opy_()
+  elif (bstack11_opy_ (u"ࠪࡦࡺ࡯࡬ࡥࡐࡤࡱࡪ࠭ன") not in CONFIG and bstack11_opy_ (u"ࠫࡧࡻࡩ࡭ࡦࡌࡨࡪࡴࡴࡪࡨ࡬ࡩࡷ࠭ப") in CONFIG) or (bstack11_opy_ (u"ࠬࡨࡵࡪ࡮ࡧࡒࡦࡳࡥࠨ஫") in bstack1l111_opy_ and bstack11_opy_ (u"࠭ࡢࡶ࡫࡯ࡨࡓࡧ࡭ࡦࠩ஬") not in bstack1lll1lll_opy_):
+    del(CONFIG[bstack11_opy_ (u"ࠧࡣࡷ࡬ࡰࡩࡏࡤࡦࡰࡷ࡭࡫࡯ࡥࡳࠩ஭")])
+  if bstack11ll1ll1_opy_(CONFIG):
+    bstack11111l11_opy_(bstack1l1l11_opy_)
+  bstack11lll11l_opy_()
+  bstack111ll1l1_opy_()
+  if bstack1llll1l_opy_:
+    CONFIG[bstack11_opy_ (u"ࠨࡣࡳࡴࠬம")] = bstack1ll1111_opy_(CONFIG)
+    logger.info(bstack1ll1ll111_opy_.format(CONFIG[bstack11_opy_ (u"ࠩࡤࡴࡵ࠭ய")]))
+def bstack111ll1l1_opy_():
   global CONFIG
-  global bstack1ll11111l_opy_
-  if bstack1ll1_opy_ (u"ࠧࡢࡲࡳࠫ஑") in CONFIG:
+  global bstack1llll1l_opy_
+  if bstack11_opy_ (u"ࠪࡥࡵࡶࠧர") in CONFIG:
     try:
       from appium import version
     except Exception as e:
-      bstack11l1_opy_(e, bstack1l11lll1l_opy_)
-    bstack1ll11111l_opy_ = True
-def bstack1l11ll1_opy_(config):
-  bstack1111l111_opy_ = bstack1ll1_opy_ (u"ࠨࠩஒ")
-  app = config[bstack1ll1_opy_ (u"ࠩࡤࡴࡵ࠭ஓ")]
+      bstack111lll1l_opy_(e, bstack11ll1l11_opy_)
+    bstack1llll1l_opy_ = True
+def bstack1ll1111_opy_(config):
+  bstack1ll111lll_opy_ = bstack11_opy_ (u"ࠫࠬற")
+  app = config[bstack11_opy_ (u"ࠬࡧࡰࡱࠩல")]
   if isinstance(app, str):
-    if os.path.splitext(app)[1] in bstack1l1l1l1_opy_:
+    if os.path.splitext(app)[1] in bstack1lll1l_opy_:
       if os.path.exists(app):
-        bstack1111l111_opy_ = bstack11111lll_opy_(config, app)
-      elif bstack1ll1l11_opy_(app):
-        bstack1111l111_opy_ = app
+        bstack1ll111lll_opy_ = bstack11111l1_opy_(config, app)
+      elif bstack1lll1l1_opy_(app):
+        bstack1ll111lll_opy_ = app
       else:
-        bstack1ll1lll_opy_(bstack111ll11l_opy_.format(app))
+        bstack11111l11_opy_(bstack1ll1111l_opy_.format(app))
     else:
-      if bstack1ll1l11_opy_(app):
-        bstack1111l111_opy_ = app
+      if bstack1lll1l1_opy_(app):
+        bstack1ll111lll_opy_ = app
       elif os.path.exists(app):
-        bstack1111l111_opy_ = bstack11111lll_opy_(app)
+        bstack1ll111lll_opy_ = bstack11111l1_opy_(app)
       else:
-        bstack1ll1lll_opy_(bstack111ll1l1_opy_)
+        bstack11111l11_opy_(bstack11l1ll_opy_)
   else:
     if len(app) > 2:
-      bstack1ll1lll_opy_(bstack1ll11ll_opy_)
+      bstack11111l11_opy_(bstack11l1l11l_opy_)
     elif len(app) == 2:
-      if bstack1ll1_opy_ (u"ࠪࡴࡦࡺࡨࠨஔ") in app and bstack1ll1_opy_ (u"ࠫࡨࡻࡳࡵࡱࡰࡣ࡮ࡪࠧக") in app:
-        if os.path.exists(app[bstack1ll1_opy_ (u"ࠬࡶࡡࡵࡪࠪ஖")]):
-          bstack1111l111_opy_ = bstack11111lll_opy_(config, app[bstack1ll1_opy_ (u"࠭ࡰࡢࡶ࡫ࠫ஗")], app[bstack1ll1_opy_ (u"ࠧࡤࡷࡶࡸࡴࡳ࡟ࡪࡦࠪ஘")])
+      if bstack11_opy_ (u"࠭ࡰࡢࡶ࡫ࠫள") in app and bstack11_opy_ (u"ࠧࡤࡷࡶࡸࡴࡳ࡟ࡪࡦࠪழ") in app:
+        if os.path.exists(app[bstack11_opy_ (u"ࠨࡲࡤࡸ࡭࠭வ")]):
+          bstack1ll111lll_opy_ = bstack11111l1_opy_(config, app[bstack11_opy_ (u"ࠩࡳࡥࡹ࡮ࠧஶ")], app[bstack11_opy_ (u"ࠪࡧࡺࡹࡴࡰ࡯ࡢ࡭ࡩ࠭ஷ")])
         else:
-          bstack1ll1lll_opy_(bstack111ll11l_opy_.format(app))
+          bstack11111l11_opy_(bstack1ll1111l_opy_.format(app))
       else:
-        bstack1ll1lll_opy_(bstack1ll11ll_opy_)
+        bstack11111l11_opy_(bstack11l1l11l_opy_)
     else:
       for key in app:
-        if key in bstack1l11l1l1l_opy_:
-          if key == bstack1ll1_opy_ (u"ࠨࡲࡤࡸ࡭࠭ங"):
+        if key in bstack1l1l1l1l_opy_:
+          if key == bstack11_opy_ (u"ࠫࡵࡧࡴࡩࠩஸ"):
             if os.path.exists(app[key]):
-              bstack1111l111_opy_ = bstack11111lll_opy_(config, app[key])
+              bstack1ll111lll_opy_ = bstack11111l1_opy_(config, app[key])
             else:
-              bstack1ll1lll_opy_(bstack111ll11l_opy_.format(app))
+              bstack11111l11_opy_(bstack1ll1111l_opy_.format(app))
           else:
-            bstack1111l111_opy_ = app[key]
+            bstack1ll111lll_opy_ = app[key]
         else:
-          bstack1ll1lll_opy_(bstack1l1ll1l1l_opy_)
-  return bstack1111l111_opy_
-def bstack1ll1l11_opy_(bstack1111l111_opy_):
+          bstack11111l11_opy_(bstack11ll1_opy_)
+  return bstack1ll111lll_opy_
+def bstack1lll1l1_opy_(bstack1ll111lll_opy_):
   import re
-  bstack1l1llllll_opy_ = re.compile(bstack1ll1_opy_ (u"ࡴࠥࡢࡠࡧ࠭ࡻࡃ࠰࡞࠵࠳࠹࡝ࡡ࠱ࡠ࠲ࡣࠪࠥࠤச"))
-  bstack111l1_opy_ = re.compile(bstack1ll1_opy_ (u"ࡵࠦࡣࡡࡡ࠮ࡼࡄ࠱࡟࠶࠭࠺࡞ࡢ࠲ࡡ࠳࡝ࠫ࠱࡞ࡥ࠲ࢀࡁ࠮࡜࠳࠱࠾ࡢ࡟࠯࡞࠰ࡡ࠯ࠪࠢ஛"))
-  if bstack1ll1_opy_ (u"ࠫࡧࡹ࠺࠰࠱ࠪஜ") in bstack1111l111_opy_ or re.fullmatch(bstack1l1llllll_opy_, bstack1111l111_opy_) or re.fullmatch(bstack111l1_opy_, bstack1111l111_opy_):
+  bstack11lll11_opy_ = re.compile(bstack11_opy_ (u"ࡷࠨ࡞࡜ࡣ࠰ࡾࡆ࠳࡚࠱࠯࠼ࡠࡤ࠴࡜࠮࡟࠭ࠨࠧஹ"))
+  bstack1ll1llll1_opy_ = re.compile(bstack11_opy_ (u"ࡸࠢ࡟࡝ࡤ࠱ࡿࡇ࡛࠭࠲࠰࠽ࡡࡥ࠮࡝࠯ࡠ࠮࠴ࡡࡡ࠮ࡼࡄ࠱࡟࠶࠭࠺࡞ࡢ࠲ࡡ࠳࡝ࠫࠦࠥ஺"))
+  if bstack11_opy_ (u"ࠧࡣࡵ࠽࠳࠴࠭஻") in bstack1ll111lll_opy_ or re.fullmatch(bstack11lll11_opy_, bstack1ll111lll_opy_) or re.fullmatch(bstack1ll1llll1_opy_, bstack1ll111lll_opy_):
     return True
   else:
     return False
-def bstack11111lll_opy_(config, path, bstack1l11l1l11_opy_=None):
+def bstack11111l1_opy_(config, path, bstack1llll11l_opy_=None):
   import requests
   from requests_toolbelt.multipart.encoder import MultipartEncoder
   import hashlib
-  md5_hash = hashlib.md5(open(os.path.abspath(path), bstack1ll1_opy_ (u"ࠬࡸࡢࠨ஝")).read()).hexdigest()
-  bstack1ll11l1l1_opy_ = bstack1lll11l_opy_(md5_hash)
-  bstack1111l111_opy_ = None
-  if bstack1ll11l1l1_opy_:
-    logger.info(bstack1llllll1l_opy_.format(bstack1ll11l1l1_opy_, md5_hash))
-    return bstack1ll11l1l1_opy_
-  bstack1ll1111l1_opy_ = MultipartEncoder(
+  md5_hash = hashlib.md5(open(os.path.abspath(path), bstack11_opy_ (u"ࠨࡴࡥࠫ஼")).read()).hexdigest()
+  bstack1lllllll_opy_ = bstack1l11l1l_opy_(md5_hash)
+  bstack1ll111lll_opy_ = None
+  if bstack1lllllll_opy_:
+    logger.info(bstack1l1ll11ll_opy_.format(bstack1lllllll_opy_, md5_hash))
+    return bstack1lllllll_opy_
+  bstack1ll1l1_opy_ = MultipartEncoder(
     fields={
-        bstack1ll1_opy_ (u"࠭ࡦࡪ࡮ࡨࠫஞ"): (os.path.basename(path), open(os.path.abspath(path), bstack1ll1_opy_ (u"ࠧࡳࡤࠪட")), bstack1ll1_opy_ (u"ࠨࡶࡨࡼࡹ࠵ࡰ࡭ࡣ࡬ࡲࠬ஠")),
-        bstack1ll1_opy_ (u"ࠩࡦࡹࡸࡺ࡯࡮ࡡ࡬ࡨࠬ஡"): bstack1l11l1l11_opy_
+        bstack11_opy_ (u"ࠩࡩ࡭ࡱ࡫ࠧ஽"): (os.path.basename(path), open(os.path.abspath(path), bstack11_opy_ (u"ࠪࡶࡧ࠭ா")), bstack11_opy_ (u"ࠫࡹ࡫ࡸࡵ࠱ࡳࡰࡦ࡯࡮ࠨி")),
+        bstack11_opy_ (u"ࠬࡩࡵࡴࡶࡲࡱࡤ࡯ࡤࠨீ"): bstack1llll11l_opy_
     }
   )
-  response = requests.post(bstack1l1llll1_opy_, data=bstack1ll1111l1_opy_,
-                         headers={bstack1ll1_opy_ (u"ࠪࡇࡴࡴࡴࡦࡰࡷ࠱࡙ࡿࡰࡦࠩ஢"): bstack1ll1111l1_opy_.content_type}, auth=(config[bstack1ll1_opy_ (u"ࠫࡺࡹࡥࡳࡐࡤࡱࡪ࠭ண")], config[bstack1ll1_opy_ (u"ࠬࡧࡣࡤࡧࡶࡷࡐ࡫ࡹࠨத")]))
+  response = requests.post(bstack1l111lll_opy_, data=bstack1ll1l1_opy_,
+                         headers={bstack11_opy_ (u"࠭ࡃࡰࡰࡷࡩࡳࡺ࠭ࡕࡻࡳࡩࠬு"): bstack1ll1l1_opy_.content_type}, auth=(config[bstack11_opy_ (u"ࠧࡶࡵࡨࡶࡓࡧ࡭ࡦࠩூ")], config[bstack11_opy_ (u"ࠨࡣࡦࡧࡪࡹࡳࡌࡧࡼࠫ௃")]))
   try:
     res = json.loads(response.text)
-    bstack1111l111_opy_ = res[bstack1ll1_opy_ (u"࠭ࡡࡱࡲࡢࡹࡷࡲࠧ஥")]
-    logger.info(bstack11lllll1_opy_.format(bstack1111l111_opy_))
-    bstack11ll1111_opy_(md5_hash, bstack1111l111_opy_)
+    bstack1ll111lll_opy_ = res[bstack11_opy_ (u"ࠩࡤࡴࡵࡥࡵࡳ࡮ࠪ௄")]
+    logger.info(bstack1l1l1lll1_opy_.format(bstack1ll111lll_opy_))
+    bstack1ll1ll1l1_opy_(md5_hash, bstack1ll111lll_opy_)
   except ValueError as err:
-    bstack1ll1lll_opy_(bstack111llll1_opy_.format(str(err)))
-  return bstack1111l111_opy_
-def bstack11l1ll1_opy_():
-  global CONFIG
-  global bstack1llll1_opy_
-  bstack1lll1llll_opy_ = 0
-  bstack11ll1_opy_ = 1
-  if bstack1ll1_opy_ (u"ࠧࡱࡣࡵࡥࡱࡲࡥ࡭ࡵࡓࡩࡷࡖ࡬ࡢࡶࡩࡳࡷࡳࠧ஦") in CONFIG:
-    bstack11ll1_opy_ = CONFIG[bstack1ll1_opy_ (u"ࠨࡲࡤࡶࡦࡲ࡬ࡦ࡮ࡶࡔࡪࡸࡐ࡭ࡣࡷࡪࡴࡸ࡭ࠨ஧")]
-  if bstack1ll1_opy_ (u"ࠩࡳࡰࡦࡺࡦࡰࡴࡰࡷࠬந") in CONFIG:
-    bstack1lll1llll_opy_ = len(CONFIG[bstack1ll1_opy_ (u"ࠪࡴࡱࡧࡴࡧࡱࡵࡱࡸ࠭ன")])
-  bstack1llll1_opy_ = int(bstack11ll1_opy_) * int(bstack1lll1llll_opy_)
-def bstack1lll11l_opy_(md5_hash):
-  bstack1l1ll111_opy_ = os.path.join(os.path.expanduser(bstack1ll1_opy_ (u"ࠫࢃ࠭ப")), bstack1ll1_opy_ (u"ࠬ࠴ࡢࡳࡱࡺࡷࡪࡸࡳࡵࡣࡦ࡯ࠬ஫"), bstack1ll1_opy_ (u"࠭ࡡࡱࡲࡘࡴࡱࡵࡡࡥࡏࡇ࠹ࡍࡧࡳࡩ࠰࡭ࡷࡴࡴࠧ஬"))
-  if os.path.exists(bstack1l1ll111_opy_):
-    bstack1l111ll1_opy_ = json.load(open(bstack1l1ll111_opy_,bstack1ll1_opy_ (u"ࠧࡳࡤࠪ஭")))
-    if md5_hash in bstack1l111ll1_opy_:
-      bstack11l111_opy_ = bstack1l111ll1_opy_[md5_hash]
-      bstack1l1l1ll11_opy_ = datetime.datetime.now()
-      bstack1l1ll1ll1_opy_ = datetime.datetime.strptime(bstack11l111_opy_[bstack1ll1_opy_ (u"ࠨࡶ࡬ࡱࡪࡹࡴࡢ࡯ࡳࠫம")], bstack1ll1_opy_ (u"ࠩࠨࡨ࠴ࠫ࡭࠰ࠧ࡜ࠤࠪࡎ࠺ࠦࡏ࠽ࠩࡘ࠭ய"))
-      if (bstack1l1l1ll11_opy_ - bstack1l1ll1ll1_opy_).days > 60:
+    bstack11111l11_opy_(bstack11111ll1_opy_.format(str(err)))
+  return bstack1ll111lll_opy_
+def bstack11lll11l_opy_():
+  global CONFIG
+  global bstack1l11ll1ll_opy_
+  bstack111lll1_opy_ = 0
+  bstack11ll111l_opy_ = 1
+  if bstack11_opy_ (u"ࠪࡴࡦࡸࡡ࡭࡮ࡨࡰࡸࡖࡥࡳࡒ࡯ࡥࡹ࡬࡯ࡳ࡯ࠪ௅") in CONFIG:
+    bstack11ll111l_opy_ = CONFIG[bstack11_opy_ (u"ࠫࡵࡧࡲࡢ࡮࡯ࡩࡱࡹࡐࡦࡴࡓࡰࡦࡺࡦࡰࡴࡰࠫெ")]
+  if bstack11_opy_ (u"ࠬࡶ࡬ࡢࡶࡩࡳࡷࡳࡳࠨே") in CONFIG:
+    bstack111lll1_opy_ = len(CONFIG[bstack11_opy_ (u"࠭ࡰ࡭ࡣࡷࡪࡴࡸ࡭ࡴࠩை")])
+  bstack1l11ll1ll_opy_ = int(bstack11ll111l_opy_) * int(bstack111lll1_opy_)
+def bstack1l11l1l_opy_(md5_hash):
+  bstack11l1l111_opy_ = os.path.join(os.path.expanduser(bstack11_opy_ (u"ࠧࡿࠩ௉")), bstack11_opy_ (u"ࠨ࠰ࡥࡶࡴࡽࡳࡦࡴࡶࡸࡦࡩ࡫ࠨொ"), bstack11_opy_ (u"ࠩࡤࡴࡵ࡛ࡰ࡭ࡱࡤࡨࡒࡊ࠵ࡉࡣࡶ࡬࠳ࡰࡳࡰࡰࠪோ"))
+  if os.path.exists(bstack11l1l111_opy_):
+    bstack11ll1111_opy_ = json.load(open(bstack11l1l111_opy_,bstack11_opy_ (u"ࠪࡶࡧ࠭ௌ")))
+    if md5_hash in bstack11ll1111_opy_:
+      bstack1llll1l11_opy_ = bstack11ll1111_opy_[md5_hash]
+      bstack1l1ll1lll_opy_ = datetime.datetime.now()
+      bstack1l1111l11_opy_ = datetime.datetime.strptime(bstack1llll1l11_opy_[bstack11_opy_ (u"ࠫࡹ࡯࡭ࡦࡵࡷࡥࡲࡶ்ࠧ")], bstack11_opy_ (u"ࠬࠫࡤ࠰ࠧࡰ࠳ࠪ࡟ࠠࠦࡊ࠽ࠩࡒࡀࠥࡔࠩ௎"))
+      if (bstack1l1ll1lll_opy_ - bstack1l1111l11_opy_).days > 60:
         return None
-      elif version.parse(str(__version__)) > version.parse(bstack11l111_opy_[bstack1ll1_opy_ (u"ࠪࡷࡩࡱ࡟ࡷࡧࡵࡷ࡮ࡵ࡮ࠨர")]):
+      elif version.parse(str(__version__)) > version.parse(bstack1llll1l11_opy_[bstack11_opy_ (u"࠭ࡳࡥ࡭ࡢࡺࡪࡸࡳࡪࡱࡱࠫ௏")]):
         return None
-      return bstack11l111_opy_[bstack1ll1_opy_ (u"ࠫ࡮ࡪࠧற")]
+      return bstack1llll1l11_opy_[bstack11_opy_ (u"ࠧࡪࡦࠪௐ")]
   else:
     return None
-def bstack11ll1111_opy_(md5_hash, bstack1111l111_opy_):
-  bstack11ll11ll_opy_ = os.path.join(os.path.expanduser(bstack1ll1_opy_ (u"ࠬࢄࠧல")), bstack1ll1_opy_ (u"࠭࠮ࡣࡴࡲࡻࡸ࡫ࡲࡴࡶࡤࡧࡰ࠭ள"))
-  if not os.path.exists(bstack11ll11ll_opy_):
-    os.makedirs(bstack11ll11ll_opy_)
-  bstack1l1ll111_opy_ = os.path.join(os.path.expanduser(bstack1ll1_opy_ (u"ࠧࡿࠩழ")), bstack1ll1_opy_ (u"ࠨ࠰ࡥࡶࡴࡽࡳࡦࡴࡶࡸࡦࡩ࡫ࠨவ"), bstack1ll1_opy_ (u"ࠩࡤࡴࡵ࡛ࡰ࡭ࡱࡤࡨࡒࡊ࠵ࡉࡣࡶ࡬࠳ࡰࡳࡰࡰࠪஶ"))
-  bstack1l11ll1l_opy_ = {
-    bstack1ll1_opy_ (u"ࠪ࡭ࡩ࠭ஷ"): bstack1111l111_opy_,
-    bstack1ll1_opy_ (u"ࠫࡹ࡯࡭ࡦࡵࡷࡥࡲࡶࠧஸ"): datetime.datetime.strftime(datetime.datetime.now(), bstack1ll1_opy_ (u"ࠬࠫࡤ࠰ࠧࡰ࠳ࠪ࡟ࠠࠦࡊ࠽ࠩࡒࡀࠥࡔࠩஹ")),
-    bstack1ll1_opy_ (u"࠭ࡳࡥ࡭ࡢࡺࡪࡸࡳࡪࡱࡱࠫ஺"): str(__version__)
+def bstack1ll1ll1l1_opy_(md5_hash, bstack1ll111lll_opy_):
+  bstack1l1lll11_opy_ = os.path.join(os.path.expanduser(bstack11_opy_ (u"ࠨࢀࠪ௑")), bstack11_opy_ (u"ࠩ࠱ࡦࡷࡵࡷࡴࡧࡵࡷࡹࡧࡣ࡬ࠩ௒"))
+  if not os.path.exists(bstack1l1lll11_opy_):
+    os.makedirs(bstack1l1lll11_opy_)
+  bstack11l1l111_opy_ = os.path.join(os.path.expanduser(bstack11_opy_ (u"ࠪࢂࠬ௓")), bstack11_opy_ (u"ࠫ࠳ࡨࡲࡰࡹࡶࡩࡷࡹࡴࡢࡥ࡮ࠫ௔"), bstack11_opy_ (u"ࠬࡧࡰࡱࡗࡳࡰࡴࡧࡤࡎࡆ࠸ࡌࡦࡹࡨ࠯࡬ࡶࡳࡳ࠭௕"))
+  bstack1l111ll_opy_ = {
+    bstack11_opy_ (u"࠭ࡩࡥࠩ௖"): bstack1ll111lll_opy_,
+    bstack11_opy_ (u"ࠧࡵ࡫ࡰࡩࡸࡺࡡ࡮ࡲࠪௗ"): datetime.datetime.strftime(datetime.datetime.now(), bstack11_opy_ (u"ࠨࠧࡧ࠳ࠪࡳ࠯࡛ࠦࠣࠩࡍࡀࠥࡎ࠼ࠨࡗࠬ௘")),
+    bstack11_opy_ (u"ࠩࡶࡨࡰࡥࡶࡦࡴࡶ࡭ࡴࡴࠧ௙"): str(__version__)
   }
-  if os.path.exists(bstack1l1ll111_opy_):
-    bstack1l111ll1_opy_ = json.load(open(bstack1l1ll111_opy_,bstack1ll1_opy_ (u"ࠧࡳࡤࠪ஻")))
+  if os.path.exists(bstack11l1l111_opy_):
+    bstack11ll1111_opy_ = json.load(open(bstack11l1l111_opy_,bstack11_opy_ (u"ࠪࡶࡧ࠭௚")))
   else:
-    bstack1l111ll1_opy_ = {}
-  bstack1l111ll1_opy_[md5_hash] = bstack1l11ll1l_opy_
-  with open(bstack1l1ll111_opy_, bstack1ll1_opy_ (u"ࠣࡹ࠮ࠦ஼")) as outfile:
-    json.dump(bstack1l111ll1_opy_, outfile)
-def bstack1lll11111_opy_(self):
+    bstack11ll1111_opy_ = {}
+  bstack11ll1111_opy_[md5_hash] = bstack1l111ll_opy_
+  with open(bstack11l1l111_opy_, bstack11_opy_ (u"ࠦࡼ࠱ࠢ௛")) as outfile:
+    json.dump(bstack11ll1111_opy_, outfile)
+def bstack11ll1l1l_opy_(self):
   return
-def bstack1llll1l11_opy_(self):
+def bstack11l1lll1_opy_(self):
   return
-def bstack111l11ll_opy_(self):
+def bstack11l11l1_opy_(self):
   from selenium.webdriver.remote.webdriver import WebDriver
   WebDriver.quit(self)
-def bstack1llll1111_opy_(self, command_executor,
+def bstack1l1l1111l_opy_(self, command_executor,
         desired_capabilities=None, browser_profile=None, proxy=None,
         keep_alive=True, file_detector=None, options=None):
   global CONFIG
-  global bstack1111111_opy_
-  global bstack1111ll_opy_
-  global bstack1ll111ll_opy_
-  global bstack1l1ll1l_opy_
-  global bstack1l1l1l11_opy_
-  global bstack1lll1_opy_
-  global bstack111l_opy_
-  CONFIG[bstack1ll1_opy_ (u"ࠩࡥࡶࡴࡽࡳࡦࡴࡶࡸࡦࡩ࡫ࡔࡆࡎࠫ஽")] = str(bstack1l1l1l11_opy_) + str(__version__)
-  command_executor = bstack1l1l11ll_opy_()
-  logger.debug(bstack1lll1ll_opy_.format(command_executor))
-  proxy = bstack1ll1l11l1_opy_(CONFIG, proxy)
-  bstack111111l_opy_ = 0 if bstack1111ll_opy_ < 0 else bstack1111ll_opy_
-  if bstack1l1ll1l_opy_ is True:
-    bstack111111l_opy_ = int(threading.current_thread().getName())
-  bstack11l1l1l1_opy_ = bstack1llll11l1_opy_(CONFIG, bstack111111l_opy_)
-  logger.debug(bstack11lll11_opy_.format(str(bstack11l1l1l1_opy_)))
-  if bstack1ll1_opy_ (u"ࠪࡦࡷࡵࡷࡴࡧࡵࡷࡹࡧࡣ࡬ࡎࡲࡧࡦࡲࠧா") in CONFIG and CONFIG[bstack1ll1_opy_ (u"ࠫࡧࡸ࡯ࡸࡵࡨࡶࡸࡺࡡࡤ࡭ࡏࡳࡨࡧ࡬ࠨி")]:
-    bstack11l1l1l_opy_(bstack11l1l1l1_opy_)
+  global bstack1l1lll1ll_opy_
+  global bstack1l111l11l_opy_
+  global bstack1ll1l11_opy_
+  global bstack1l11llll_opy_
+  global bstack1l1lll1l_opy_
+  global bstack1ll1l11ll_opy_
+  global bstack1ll1l1l1_opy_
+  CONFIG[bstack11_opy_ (u"ࠬࡨࡲࡰࡹࡶࡩࡷࡹࡴࡢࡥ࡮ࡗࡉࡑࠧ௜")] = str(bstack1l1lll1l_opy_) + str(__version__)
+  command_executor = bstack11l1ll11_opy_()
+  logger.debug(bstack1lll1111_opy_.format(command_executor))
+  proxy = bstack1l11111l_opy_(CONFIG, proxy)
+  bstack1l1l111ll_opy_ = 0 if bstack1l111l11l_opy_ < 0 else bstack1l111l11l_opy_
+  if bstack1l11llll_opy_ is True:
+    bstack1l1l111ll_opy_ = int(threading.current_thread().getName())
+  bstack1lll11l_opy_ = bstack1l111l1ll_opy_(CONFIG, bstack1l1l111ll_opy_)
+  logger.debug(bstack1ll11l111_opy_.format(str(bstack1lll11l_opy_)))
+  if bstack11_opy_ (u"࠭ࡢࡳࡱࡺࡷࡪࡸࡳࡵࡣࡦ࡯ࡑࡵࡣࡢ࡮ࠪ௝") in CONFIG and CONFIG[bstack11_opy_ (u"ࠧࡣࡴࡲࡻࡸ࡫ࡲࡴࡶࡤࡧࡰࡒ࡯ࡤࡣ࡯ࠫ௞")]:
+    bstack1l1lll111_opy_(bstack1lll11l_opy_)
   if desired_capabilities:
-    bstack11lll111_opy_ = bstack1ll11lll_opy_(desired_capabilities)
-    bstack11lll111_opy_[bstack1ll1_opy_ (u"ࠬࡻࡳࡦ࡙࠶ࡇࠬீ")] = bstack1l11l1_opy_(CONFIG)
-    bstack111ll111_opy_ = bstack1llll11l1_opy_(bstack11lll111_opy_)
-    if bstack111ll111_opy_:
-      bstack11l1l1l1_opy_ = update(bstack111ll111_opy_, bstack11l1l1l1_opy_)
+    bstack111l1l1_opy_ = bstack11lllll1_opy_(desired_capabilities)
+    bstack111l1l1_opy_[bstack11_opy_ (u"ࠨࡷࡶࡩ࡜࠹ࡃࠨ௟")] = bstack1ll11111_opy_(CONFIG)
+    bstack1l1111_opy_ = bstack1l111l1ll_opy_(bstack111l1l1_opy_)
+    if bstack1l1111_opy_:
+      bstack1lll11l_opy_ = update(bstack1l1111_opy_, bstack1lll11l_opy_)
     desired_capabilities = None
   if options:
-    bstack1llllllll_opy_(options, bstack11l1l1l1_opy_)
+    bstack1llll1111_opy_(options, bstack1lll11l_opy_)
   if not options:
-    options = bstack11l11ll_opy_(bstack11l1l1l1_opy_)
-  if options and bstack1ll1llll_opy_() >= version.parse(bstack1ll1_opy_ (u"࠭࠳࠯࠺࠱࠴ࠬு")):
+    options = bstack1ll11l1l_opy_(bstack1lll11l_opy_)
+  if options and bstack1ll11l1ll_opy_() >= version.parse(bstack11_opy_ (u"ࠩ࠶࠲࠽࠴࠰ࠨ௠")):
     desired_capabilities = None
   if (
       not options and not desired_capabilities
   ) or (
-      bstack1ll1llll_opy_() < version.parse(bstack1ll1_opy_ (u"ࠧ࠴࠰࠻࠲࠵࠭ூ")) and not desired_capabilities
+      bstack1ll11l1ll_opy_() < version.parse(bstack11_opy_ (u"ࠪ࠷࠳࠾࠮࠱ࠩ௡")) and not desired_capabilities
   ):
     desired_capabilities = {}
-    desired_capabilities.update(bstack11l1l1l1_opy_)
-  logger.info(bstack1l1llll_opy_)
-  if bstack1ll1llll_opy_() >= version.parse(bstack1ll1_opy_ (u"ࠨ࠵࠱࠼࠳࠶ࠧ௃")):
-    bstack1lll1_opy_(self, command_executor=command_executor,
+    desired_capabilities.update(bstack1lll11l_opy_)
+  logger.info(bstack111111_opy_)
+  if bstack1ll11l1ll_opy_() >= version.parse(bstack11_opy_ (u"ࠫ࠸࠴࠸࠯࠲ࠪ௢")):
+    bstack1ll1l11ll_opy_(self, command_executor=command_executor,
           desired_capabilities=desired_capabilities, options=options,
           browser_profile=browser_profile, proxy=proxy,
           keep_alive=keep_alive, file_detector=file_detector)
-  elif bstack1ll1llll_opy_() >= version.parse(bstack1ll1_opy_ (u"ࠩ࠵࠲࠺࠹࠮࠱ࠩ௄")):
-    bstack1lll1_opy_(self, command_executor=command_executor,
+  elif bstack1ll11l1ll_opy_() >= version.parse(bstack11_opy_ (u"ࠬ࠸࠮࠶࠵࠱࠴ࠬ௣")):
+    bstack1ll1l11ll_opy_(self, command_executor=command_executor,
           desired_capabilities=desired_capabilities,
           browser_profile=browser_profile, proxy=proxy,
           keep_alive=keep_alive, file_detector=file_detector)
   else:
-    bstack1lll1_opy_(self, command_executor=command_executor,
+    bstack1ll1l11ll_opy_(self, command_executor=command_executor,
           desired_capabilities=desired_capabilities,
           browser_profile=browser_profile, proxy=proxy,
           keep_alive=keep_alive)
-  bstack1111111_opy_ = self.session_id
-  bstack111l_opy_.append(self)
-  if bstack1ll1_opy_ (u"ࠪࡴࡱࡧࡴࡧࡱࡵࡱࡸ࠭௅") in CONFIG and bstack1ll1_opy_ (u"ࠫࡸ࡫ࡳࡴ࡫ࡲࡲࡓࡧ࡭ࡦࠩெ") in CONFIG[bstack1ll1_opy_ (u"ࠬࡶ࡬ࡢࡶࡩࡳࡷࡳࡳࠨே")][bstack111111l_opy_]:
-    bstack1ll111ll_opy_ = CONFIG[bstack1ll1_opy_ (u"࠭ࡰ࡭ࡣࡷࡪࡴࡸ࡭ࡴࠩை")][bstack111111l_opy_][bstack1ll1_opy_ (u"ࠧࡴࡧࡶࡷ࡮ࡵ࡮ࡏࡣࡰࡩࠬ௉")]
-  logger.debug(bstack11lll11l_opy_.format(bstack1111111_opy_))
+  try:
+    bstack1l11111_opy_ = bstack11_opy_ (u"࠭ࠧ௤")
+    if bstack1ll11l1ll_opy_() >= version.parse(bstack11_opy_ (u"ࠧ࠵࠰࠳࠲࠵ࡨ࠱ࠨ௥")):
+      bstack1l11111_opy_ = self.caps.get(bstack11_opy_ (u"ࠣࡱࡳࡸ࡮ࡳࡡ࡭ࡊࡸࡦ࡚ࡸ࡬ࠣ௦"))
+    else:
+      bstack1l11111_opy_ = self.capabilities.get(bstack11_opy_ (u"ࠤࡲࡴࡹ࡯࡭ࡢ࡮ࡋࡹࡧ࡛ࡲ࡭ࠤ௧"))
+    if bstack1l11111_opy_:
+      if bstack1ll11l1ll_opy_() <= version.parse(bstack11_opy_ (u"ࠪ࠷࠳࠷࠳࠯࠲ࠪ௨")):
+        self.command_executor._url = bstack11_opy_ (u"ࠦ࡭ࡺࡴࡱ࠼࠲࠳ࠧ௩") + bstack1l1ll11_opy_ + bstack11_opy_ (u"ࠧࡀ࠸࠱࠱ࡺࡨ࠴࡮ࡵࡣࠤ௪")
+      else:
+        self.command_executor._url = bstack11_opy_ (u"ࠨࡨࡵࡶࡳࡷ࠿࠵࠯ࠣ௫") + bstack1l11111_opy_ + bstack11_opy_ (u"ࠢ࠰ࡹࡧ࠳࡭ࡻࡢࠣ௬")
+      logger.debug(bstack1l1l1ll1l_opy_.format(bstack1l11111_opy_))
+    else:
+      logger.debug(bstack1l11l11l_opy_.format(bstack11_opy_ (u"ࠣࡑࡳࡸ࡮ࡳࡡ࡭ࠢࡋࡹࡧࠦ࡮ࡰࡶࠣࡪࡴࡻ࡮ࡥࠤ௭")))
+  except Exception as e:
+    logger.debug(bstack1l11l11l_opy_.format(e))
+  bstack1l1lll1ll_opy_ = self.session_id
+  bstack1ll1l1l1_opy_.append(self)
+  if bstack11_opy_ (u"ࠩࡳࡰࡦࡺࡦࡰࡴࡰࡷࠬ௮") in CONFIG and bstack11_opy_ (u"ࠪࡷࡪࡹࡳࡪࡱࡱࡒࡦࡳࡥࠨ௯") in CONFIG[bstack11_opy_ (u"ࠫࡵࡲࡡࡵࡨࡲࡶࡲࡹࠧ௰")][bstack1l1l111ll_opy_]:
+    bstack1ll1l11_opy_ = CONFIG[bstack11_opy_ (u"ࠬࡶ࡬ࡢࡶࡩࡳࡷࡳࡳࠨ௱")][bstack1l1l111ll_opy_][bstack11_opy_ (u"࠭ࡳࡦࡵࡶ࡭ࡴࡴࡎࡢ࡯ࡨࠫ௲")]
+  logger.debug(bstack111111l1_opy_.format(bstack1l1lll1ll_opy_))
 try:
   try:
     import Browser
     from subprocess import Popen
-    def bstack111l11l1_opy_(self, args, bufsize=-1, executable=None,
+    def bstack1l1llll11_opy_(self, args, bufsize=-1, executable=None,
               stdin=None, stdout=None, stderr=None,
               preexec_fn=None, close_fds=True,
               shell=False, cwd=None, env=None, universal_newlines=None,
               startupinfo=None, creationflags=0,
               restore_signals=True, start_new_session=False,
               pass_fds=(), *, user=None, group=None, extra_groups=None,
               encoding=None, errors=None, text=None, umask=-1, pipesize=-1):
       global CONFIG
-      if(bstack1ll1_opy_ (u"ࠣ࡫ࡱࡨࡪࡾ࠮࡫ࡵࠥொ") in args[1]):
-        with open(os.path.join(os.path.expanduser(bstack1ll1_opy_ (u"ࠩࢁࠫோ")), bstack1ll1_opy_ (u"ࠪ࠲ࡧࡸ࡯ࡸࡵࡨࡶࡸࡺࡡࡤ࡭ࠪௌ"), bstack1ll1_opy_ (u"ࠫ࠳ࡹࡥࡴࡵ࡬ࡳࡳ࡯ࡤࡴ࠰ࡷࡼࡹ்࠭")), bstack1ll1_opy_ (u"ࠬࡽࠧ௎")) as fp:
-          fp.write(bstack1ll1_opy_ (u"ࠨࠢ௏"))
-        if(not os.path.exists(os.path.join(os.path.dirname(args[1]), bstack1ll1_opy_ (u"ࠢࡪࡰࡧࡩࡽࡥࡢࡴࡶࡤࡧࡰ࠴ࡪࡴࠤௐ")))):
-          with open(args[1], bstack1ll1_opy_ (u"ࠨࡴࠪ௑")) as f:
+      if(bstack11_opy_ (u"ࠢࡪࡰࡧࡩࡽ࠴ࡪࡴࠤ௳") in args[1]):
+        with open(os.path.join(os.path.expanduser(bstack11_opy_ (u"ࠨࢀࠪ௴")), bstack11_opy_ (u"ࠩ࠱ࡦࡷࡵࡷࡴࡧࡵࡷࡹࡧࡣ࡬ࠩ௵"), bstack11_opy_ (u"ࠪ࠲ࡸ࡫ࡳࡴ࡫ࡲࡲ࡮ࡪࡳ࠯ࡶࡻࡸࠬ௶")), bstack11_opy_ (u"ࠫࡼ࠭௷")) as fp:
+          fp.write(bstack11_opy_ (u"ࠧࠨ௸"))
+        if(not os.path.exists(os.path.join(os.path.dirname(args[1]), bstack11_opy_ (u"ࠨࡩ࡯ࡦࡨࡼࡤࡨࡳࡵࡣࡦ࡯࠳ࡰࡳࠣ௹")))):
+          with open(args[1], bstack11_opy_ (u"ࠧࡳࠩ௺")) as f:
             lines = f.readlines()
-            index = next((i for i, line in enumerate(lines) if bstack1ll1_opy_ (u"ࠩࡤࡷࡾࡴࡣࠡࡨࡸࡲࡨࡺࡩࡰࡰࠣࡣࡳ࡫ࡷࡑࡣࡪࡩ࠭ࡩ࡯࡯ࡶࡨࡼࡹ࠲ࠠࡱࡣࡪࡩࠥࡃࠠࡷࡱ࡬ࡨࠥ࠶ࠩࠨ௒") in line), None)
+            index = next((i for i, line in enumerate(lines) if bstack11_opy_ (u"ࠨࡣࡶࡽࡳࡩࠠࡧࡷࡱࡧࡹ࡯࡯࡯ࠢࡢࡲࡪࡽࡐࡢࡩࡨࠬࡨࡵ࡮ࡵࡧࡻࡸ࠱ࠦࡰࡢࡩࡨࠤࡂࠦࡶࡰ࡫ࡧࠤ࠵࠯ࠧ௻") in line), None)
             if index is not None:
-                lines.insert(index+2, bstack11l111l1_opy_)
-            lines.insert(1, bstack1ll1llll1_opy_)
+                lines.insert(index+2, bstack111llll_opy_)
+            lines.insert(1, bstack1lll1l11l_opy_)
             f.seek(0)
-            with open(os.path.join(os.path.dirname(args[1]), bstack1ll1_opy_ (u"ࠥ࡭ࡳࡪࡥࡹࡡࡥࡷࡹࡧࡣ࡬࠰࡭ࡷࠧ௓")), bstack1ll1_opy_ (u"ࠫࡼ࠭௔")) as bstack1ll1ll_opy_:
-              bstack1ll1ll_opy_.writelines(lines)
-        CONFIG[bstack1ll1_opy_ (u"ࠬࡨࡲࡰࡹࡶࡩࡷࡹࡴࡢࡥ࡮ࡗࡉࡑࠧ௕")] = str(bstack1l1l1l11_opy_) + str(__version__)
-        bstack111111l_opy_ = 0 if bstack1111ll_opy_ < 0 else bstack1111ll_opy_
-        if bstack1l1ll1l_opy_ is True:
-          bstack111111l_opy_ = int(threading.current_thread().getName())
-        CONFIG[bstack1ll1_opy_ (u"ࠨࡵࡴࡧ࡚࠷ࡈࠨ௖")] = False
-        bstack11l1l1l1_opy_ = bstack1llll11l1_opy_(CONFIG, bstack111111l_opy_)
-        logger.debug(bstack11lll11_opy_.format(str(bstack11l1l1l1_opy_)))
-        if CONFIG[bstack1ll1_opy_ (u"ࠧࡣࡴࡲࡻࡸ࡫ࡲࡴࡶࡤࡧࡰࡒ࡯ࡤࡣ࡯ࠫௗ")]:
-          bstack11l1l1l_opy_(bstack11l1l1l1_opy_)
-        if bstack1ll1_opy_ (u"ࠨࡲ࡯ࡥࡹ࡬࡯ࡳ࡯ࡶࠫ௘") in CONFIG and bstack1ll1_opy_ (u"ࠩࡶࡩࡸࡹࡩࡰࡰࡑࡥࡲ࡫ࠧ௙") in CONFIG[bstack1ll1_opy_ (u"ࠪࡴࡱࡧࡴࡧࡱࡵࡱࡸ࠭௚")][bstack111111l_opy_]:
-          bstack1ll111ll_opy_ = CONFIG[bstack1ll1_opy_ (u"ࠫࡵࡲࡡࡵࡨࡲࡶࡲࡹࠧ௛")][bstack111111l_opy_][bstack1ll1_opy_ (u"ࠬࡹࡥࡴࡵ࡬ࡳࡳࡔࡡ࡮ࡧࠪ௜")]
-        args.append(os.path.join(os.path.expanduser(bstack1ll1_opy_ (u"࠭ࡾࠨ௝")), bstack1ll1_opy_ (u"ࠧ࠯ࡤࡵࡳࡼࡹࡥࡳࡵࡷࡥࡨࡱࠧ௞"), bstack1ll1_opy_ (u"ࠨ࠰ࡶࡩࡸࡹࡩࡰࡰ࡬ࡨࡸ࠴ࡴࡹࡶࠪ௟")))
+            with open(os.path.join(os.path.dirname(args[1]), bstack11_opy_ (u"ࠤ࡬ࡲࡩ࡫ࡸࡠࡤࡶࡸࡦࡩ࡫࠯࡬ࡶࠦ௼")), bstack11_opy_ (u"ࠪࡻࠬ௽")) as bstack1ll11111l_opy_:
+              bstack1ll11111l_opy_.writelines(lines)
+        CONFIG[bstack11_opy_ (u"ࠫࡧࡸ࡯ࡸࡵࡨࡶࡸࡺࡡࡤ࡭ࡖࡈࡐ࠭௾")] = str(bstack1l1lll1l_opy_) + str(__version__)
+        bstack1l1l111ll_opy_ = 0 if bstack1l111l11l_opy_ < 0 else bstack1l111l11l_opy_
+        if bstack1l11llll_opy_ is True:
+          bstack1l1l111ll_opy_ = int(threading.current_thread().getName())
+        CONFIG[bstack11_opy_ (u"ࠧࡻࡳࡦ࡙࠶ࡇࠧ௿")] = False
+        bstack1lll11l_opy_ = bstack1l111l1ll_opy_(CONFIG, bstack1l1l111ll_opy_)
+        logger.debug(bstack1ll11l111_opy_.format(str(bstack1lll11l_opy_)))
+        if CONFIG[bstack11_opy_ (u"࠭ࡢࡳࡱࡺࡷࡪࡸࡳࡵࡣࡦ࡯ࡑࡵࡣࡢ࡮ࠪఀ")]:
+          bstack1l1lll111_opy_(bstack1lll11l_opy_)
+        if bstack11_opy_ (u"ࠧࡱ࡮ࡤࡸ࡫ࡵࡲ࡮ࡵࠪఁ") in CONFIG and bstack11_opy_ (u"ࠨࡵࡨࡷࡸ࡯࡯࡯ࡐࡤࡱࡪ࠭ం") in CONFIG[bstack11_opy_ (u"ࠩࡳࡰࡦࡺࡦࡰࡴࡰࡷࠬః")][bstack1l1l111ll_opy_]:
+          bstack1ll1l11_opy_ = CONFIG[bstack11_opy_ (u"ࠪࡴࡱࡧࡴࡧࡱࡵࡱࡸ࠭ఄ")][bstack1l1l111ll_opy_][bstack11_opy_ (u"ࠫࡸ࡫ࡳࡴ࡫ࡲࡲࡓࡧ࡭ࡦࠩఅ")]
+        args.append(os.path.join(os.path.expanduser(bstack11_opy_ (u"ࠬࢄࠧఆ")), bstack11_opy_ (u"࠭࠮ࡣࡴࡲࡻࡸ࡫ࡲࡴࡶࡤࡧࡰ࠭ఇ"), bstack11_opy_ (u"ࠧ࠯ࡵࡨࡷࡸ࡯࡯࡯࡫ࡧࡷ࠳ࡺࡸࡵࠩఈ")))
         args.append(str(threading.get_ident()))
-        args.append(json.dumps(bstack11l1l1l1_opy_))
-        args[1] = os.path.join(os.path.dirname(args[1]), bstack1ll1_opy_ (u"ࠤ࡬ࡲࡩ࡫ࡸࡠࡤࡶࡸࡦࡩ࡫࠯࡬ࡶࠦ௠"))
-      return bstack1lll1l_opy_(self, args, bufsize=bufsize, executable=executable,
+        args.append(json.dumps(bstack1lll11l_opy_))
+        args[1] = os.path.join(os.path.dirname(args[1]), bstack11_opy_ (u"ࠣ࡫ࡱࡨࡪࡾ࡟ࡣࡵࡷࡥࡨࡱ࠮࡫ࡵࠥఉ"))
+      return bstack1ll1ll1ll_opy_(self, args, bufsize=bufsize, executable=executable,
                     stdin=stdin, stdout=stdout, stderr=stderr,
                     preexec_fn=preexec_fn, close_fds=close_fds,
                     shell=shell, cwd=cwd, env=env, universal_newlines=universal_newlines,
                     startupinfo=startupinfo, creationflags=creationflags,
                     restore_signals=restore_signals, start_new_session=start_new_session,
                     pass_fds=pass_fds, user=user, group=group, extra_groups=extra_groups,
                     encoding=encoding, errors=errors, text=text, umask=umask, pipesize=pipesize)
   except Exception as e:
-    logger.debug(bstack1llll111l_opy_ + str(e))
+    logger.debug(bstack1ll1lll11_opy_ + str(e))
   import playwright._impl._api_structures
   import playwright._impl._helper
-  def bstack111ll1_opy_(self,
+  def bstack1ll1111ll_opy_(self,
         executablePath = None,
         channel = None,
         args = None,
         ignoreDefaultArgs = None,
         handleSIGINT = None,
         handleSIGTERM = None,
         handleSIGHUP = None,
@@ -1474,941 +1564,943 @@
         downloadsPath = None,
         slowMo = None,
         tracesDir = None,
         chromiumSandbox = None,
         firefoxUserPrefs = None
         ):
     global CONFIG
-    global bstack1111111_opy_
-    global bstack1111ll_opy_
-    global bstack1ll111ll_opy_
-    global bstack1l1ll1l_opy_
-    global bstack1l1l1l11_opy_
-    global bstack1lll1_opy_
-    CONFIG[bstack1ll1_opy_ (u"ࠪࡦࡷࡵࡷࡴࡧࡵࡷࡹࡧࡣ࡬ࡕࡇࡏࠬ௡")] = str(bstack1l1l1l11_opy_) + str(__version__)
-    bstack111111l_opy_ = 0 if bstack1111ll_opy_ < 0 else bstack1111ll_opy_
-    if bstack1l1ll1l_opy_ is True:
-      bstack111111l_opy_ = int(threading.current_thread().getName())
-    CONFIG[bstack1ll1_opy_ (u"ࠦࡺࡹࡥࡘ࠵ࡆࠦ௢")] = False
-    bstack11l1l1l1_opy_ = bstack1llll11l1_opy_(CONFIG, bstack111111l_opy_)
-    logger.debug(bstack11lll11_opy_.format(str(bstack11l1l1l1_opy_)))
-    if CONFIG[bstack1ll1_opy_ (u"ࠬࡨࡲࡰࡹࡶࡩࡷࡹࡴࡢࡥ࡮ࡐࡴࡩࡡ࡭ࠩ௣")]:
-      bstack11l1l1l_opy_(bstack11l1l1l1_opy_)
-    if bstack1ll1_opy_ (u"࠭ࡰ࡭ࡣࡷࡪࡴࡸ࡭ࡴࠩ௤") in CONFIG and bstack1ll1_opy_ (u"ࠧࡴࡧࡶࡷ࡮ࡵ࡮ࡏࡣࡰࡩࠬ௥") in CONFIG[bstack1ll1_opy_ (u"ࠨࡲ࡯ࡥࡹ࡬࡯ࡳ࡯ࡶࠫ௦")][bstack111111l_opy_]:
-      bstack1ll111ll_opy_ = CONFIG[bstack1ll1_opy_ (u"ࠩࡳࡰࡦࡺࡦࡰࡴࡰࡷࠬ௧")][bstack111111l_opy_][bstack1ll1_opy_ (u"ࠪࡷࡪࡹࡳࡪࡱࡱࡒࡦࡳࡥࠨ௨")]
+    global bstack1l1lll1ll_opy_
+    global bstack1l111l11l_opy_
+    global bstack1ll1l11_opy_
+    global bstack1l11llll_opy_
+    global bstack1l1lll1l_opy_
+    global bstack1ll1l11ll_opy_
+    CONFIG[bstack11_opy_ (u"ࠩࡥࡶࡴࡽࡳࡦࡴࡶࡸࡦࡩ࡫ࡔࡆࡎࠫఊ")] = str(bstack1l1lll1l_opy_) + str(__version__)
+    bstack1l1l111ll_opy_ = 0 if bstack1l111l11l_opy_ < 0 else bstack1l111l11l_opy_
+    if bstack1l11llll_opy_ is True:
+      bstack1l1l111ll_opy_ = int(threading.current_thread().getName())
+    CONFIG[bstack11_opy_ (u"ࠥࡹࡸ࡫ࡗ࠴ࡅࠥఋ")] = False
+    bstack1lll11l_opy_ = bstack1l111l1ll_opy_(CONFIG, bstack1l1l111ll_opy_)
+    logger.debug(bstack1ll11l111_opy_.format(str(bstack1lll11l_opy_)))
+    if CONFIG[bstack11_opy_ (u"ࠫࡧࡸ࡯ࡸࡵࡨࡶࡸࡺࡡࡤ࡭ࡏࡳࡨࡧ࡬ࠨఌ")]:
+      bstack1l1lll111_opy_(bstack1lll11l_opy_)
+    if bstack11_opy_ (u"ࠬࡶ࡬ࡢࡶࡩࡳࡷࡳࡳࠨ఍") in CONFIG and bstack11_opy_ (u"࠭ࡳࡦࡵࡶ࡭ࡴࡴࡎࡢ࡯ࡨࠫఎ") in CONFIG[bstack11_opy_ (u"ࠧࡱ࡮ࡤࡸ࡫ࡵࡲ࡮ࡵࠪఏ")][bstack1l1l111ll_opy_]:
+      bstack1ll1l11_opy_ = CONFIG[bstack11_opy_ (u"ࠨࡲ࡯ࡥࡹ࡬࡯ࡳ࡯ࡶࠫఐ")][bstack1l1l111ll_opy_][bstack11_opy_ (u"ࠩࡶࡩࡸࡹࡩࡰࡰࡑࡥࡲ࡫ࠧ఑")]
     import urllib
     import json
-    bstack111lll11_opy_ = bstack1ll1_opy_ (u"ࠫࡼࡹࡳ࠻࠱࠲ࡧࡩࡶ࠮ࡣࡴࡲࡻࡸ࡫ࡲࡴࡶࡤࡧࡰ࠴ࡣࡰ࡯࠲ࡴࡱࡧࡹࡸࡴ࡬࡫࡭ࡺ࠿ࡤࡣࡳࡷࡂ࠭௩") + urllib.parse.quote(json.dumps(bstack11l1l1l1_opy_))
-    browser = self.connect(bstack111lll11_opy_)
+    bstack1l1l111l_opy_ = bstack11_opy_ (u"ࠪࡻࡸࡹ࠺࠰࠱ࡦࡨࡵ࠴ࡢࡳࡱࡺࡷࡪࡸࡳࡵࡣࡦ࡯࠳ࡩ࡯࡮࠱ࡳࡰࡦࡿࡷࡳ࡫ࡪ࡬ࡹࡅࡣࡢࡲࡶࡁࠬఒ") + urllib.parse.quote(json.dumps(bstack1lll11l_opy_))
+    browser = self.connect(bstack1l1l111l_opy_)
     return browser
 except Exception as e:
-    logger.debug(bstack1llll111l_opy_ + str(e))
-def bstack1ll1ll1l_opy_():
+    logger.debug(bstack1ll1lll11_opy_ + str(e))
+def bstack11l111l_opy_():
     try:
         from playwright._impl._browser_type import BrowserType
-        BrowserType.launch = bstack111ll1_opy_
+        BrowserType.launch = bstack1ll1111ll_opy_
     except Exception as e:
-        logger.debug(bstack1llll111l_opy_ + str(e))
+        logger.debug(bstack1ll1lll11_opy_ + str(e))
     try:
       import Browser
       from subprocess import Popen
-      Popen.__init__ = bstack111l11l1_opy_
+      Popen.__init__ = bstack1l1llll11_opy_
     except Exception as e:
-      logger.debug(bstack1llll111l_opy_ + str(e))
-def bstack11llll_opy_(context, bstack11l11l1_opy_):
+      logger.debug(bstack1ll1lll11_opy_ + str(e))
+def bstack1l11lll1l_opy_(context, bstack1lllllll1_opy_):
   try:
-    context.page.evaluate(bstack1ll1_opy_ (u"ࠧࡥࠠ࠾ࡀࠣࡿࢂࠨ௪"), bstack1ll1_opy_ (u"࠭ࡢࡳࡱࡺࡷࡪࡸࡳࡵࡣࡦ࡯ࡤ࡫ࡸࡦࡥࡸࡸࡴࡸ࠺ࠡࡽࠥࡥࡨࡺࡩࡰࡰࠥ࠾ࠥࠨࡳࡦࡶࡖࡩࡸࡹࡩࡰࡰࡑࡥࡲ࡫ࠢ࠭ࠢࠥࡥࡷ࡭ࡵ࡮ࡧࡱࡸࡸࠨ࠺ࠡࡽࠥࡲࡦࡳࡥࠣ࠼ࠪ௫")+ json.dumps(bstack11l11l1_opy_) + bstack1ll1_opy_ (u"ࠢࡾࡿࠥ௬"))
+    context.page.evaluate(bstack11_opy_ (u"ࠦࡤࠦ࠽࠿ࠢࡾࢁࠧఓ"), bstack11_opy_ (u"ࠬࡨࡲࡰࡹࡶࡩࡷࡹࡴࡢࡥ࡮ࡣࡪࡾࡥࡤࡷࡷࡳࡷࡀࠠࡼࠤࡤࡧࡹ࡯࡯࡯ࠤ࠽ࠤࠧࡹࡥࡵࡕࡨࡷࡸ࡯࡯࡯ࡐࡤࡱࡪࠨࠬࠡࠤࡤࡶ࡬ࡻ࡭ࡦࡰࡷࡷࠧࡀࠠࡼࠤࡱࡥࡲ࡫ࠢ࠻ࠩఔ")+ json.dumps(bstack1lllllll1_opy_) + bstack11_opy_ (u"ࠨࡽࡾࠤక"))
   except Exception as e:
-    logger.debug(bstack1ll1_opy_ (u"ࠣࡧࡻࡧࡪࡶࡴࡪࡱࡱࠤ࡮ࡴࠠࡱ࡮ࡤࡽࡼࡸࡩࡨࡪࡷࠤࡸ࡫ࡳࡴ࡫ࡲࡲࠥࡴࡡ࡮ࡧࠣࡿࢂࠨ௭"), e)
-def bstack1ll1l1l_opy_(context, message, level):
+    logger.debug(bstack11_opy_ (u"ࠢࡦࡺࡦࡩࡵࡺࡩࡰࡰࠣ࡭ࡳࠦࡰ࡭ࡣࡼࡻࡷ࡯ࡧࡩࡶࠣࡷࡪࡹࡳࡪࡱࡱࠤࡳࡧ࡭ࡦࠢࡾࢁࠧఖ"), e)
+def bstack11l1111_opy_(context, message, level):
   try:
-    context.page.evaluate(bstack1ll1_opy_ (u"ࠤࡢࠤࡂࡄࠠࡼࡿࠥ௮"), bstack1ll1_opy_ (u"ࠪࡦࡷࡵࡷࡴࡧࡵࡷࡹࡧࡣ࡬ࡡࡨࡼࡪࡩࡵࡵࡱࡵ࠾ࠥࢁࠢࡢࡥࡷ࡭ࡴࡴࠢ࠻ࠢࠥࡥࡳࡴ࡯ࡵࡣࡷࡩࠧ࠲ࠠࠣࡣࡵ࡫ࡺࡳࡥ࡯ࡶࡶࠦ࠿ࠦࡻࠣࡦࡤࡸࡦࠨ࠺ࠨ௯") + json.dumps(message) + bstack1ll1_opy_ (u"ࠫ࠱ࠨ࡬ࡦࡸࡨࡰࠧࡀࠧ௰") + json.dumps(level) + bstack1ll1_opy_ (u"ࠬࢃࡽࠨ௱"))
+    context.page.evaluate(bstack11_opy_ (u"ࠣࡡࠣࡁࡃࠦࡻࡾࠤగ"), bstack11_opy_ (u"ࠩࡥࡶࡴࡽࡳࡦࡴࡶࡸࡦࡩ࡫ࡠࡧࡻࡩࡨࡻࡴࡰࡴ࠽ࠤࢀࠨࡡࡤࡶ࡬ࡳࡳࠨ࠺ࠡࠤࡤࡲࡳࡵࡴࡢࡶࡨࠦ࠱ࠦࠢࡢࡴࡪࡹࡲ࡫࡮ࡵࡵࠥ࠾ࠥࢁࠢࡥࡣࡷࡥࠧࡀࠧఘ") + json.dumps(message) + bstack11_opy_ (u"ࠪ࠰ࠧࡲࡥࡷࡧ࡯ࠦ࠿࠭ఙ") + json.dumps(level) + bstack11_opy_ (u"ࠫࢂࢃࠧచ"))
   except Exception as e:
-    logger.debug(bstack1ll1_opy_ (u"ࠨࡥࡹࡥࡨࡴࡹ࡯࡯࡯ࠢ࡬ࡲࠥࡶ࡬ࡢࡻࡺࡶ࡮࡭ࡨࡵࠢࡤࡲࡳࡵࡴࡢࡶ࡬ࡳࡳࠦࡻࡾࠤ௲"), e)
-def bstack11ll1ll1_opy_(context, status, message = bstack1ll1_opy_ (u"ࠢࠣ௳")):
+    logger.debug(bstack11_opy_ (u"ࠧ࡫ࡸࡤࡧࡳࡸ࡮ࡵ࡮ࠡ࡫ࡱࠤࡵࡲࡡࡺࡹࡵ࡭࡬࡮ࡴࠡࡣࡱࡲࡴࡺࡡࡵ࡫ࡲࡲࠥࢁࡽࠣఛ"), e)
+def bstack1llll111l_opy_(context, status, message = bstack11_opy_ (u"ࠨࠢజ")):
   try:
-    if(status == bstack1ll1_opy_ (u"ࠣࡨࡤ࡭ࡱ࡫ࡤࠣ௴")):
-      context.page.evaluate(bstack1ll1_opy_ (u"ࠤࡢࠤࡂࡄࠠࡼࡿࠥ௵"), bstack1ll1_opy_ (u"ࠪࡦࡷࡵࡷࡴࡧࡵࡷࡹࡧࡣ࡬ࡡࡨࡼࡪࡩࡵࡵࡱࡵ࠾ࠥࢁࠢࡢࡥࡷ࡭ࡴࡴࠢ࠻ࠢࠥࡷࡪࡺࡓࡦࡵࡶ࡭ࡴࡴࡓࡵࡣࡷࡹࡸࠨࠬࠡࠤࡤࡶ࡬ࡻ࡭ࡦࡰࡷࡷࠧࡀࠠࡼࠤࡵࡩࡦࡹ࡯࡯ࠤ࠽ࠫ௶") + json.dumps(bstack1ll1_opy_ (u"ࠦࡘࡩࡥ࡯ࡣࡵ࡭ࡴࠦࡦࡢ࡫࡯ࡩࡩࠦࡷࡪࡶ࡫࠾ࠥࠨ௷") + str(message)) + bstack1ll1_opy_ (u"ࠬ࠲ࠢࡴࡶࡤࡸࡺࡹࠢ࠻ࠩ௸") + json.dumps(status) + bstack1ll1_opy_ (u"ࠨࡽࡾࠤ௹"))
+    if(status == bstack11_opy_ (u"ࠢࡧࡣ࡬ࡰࡪࡪࠢఝ")):
+      context.page.evaluate(bstack11_opy_ (u"ࠣࡡࠣࡁࡃࠦࡻࡾࠤఞ"), bstack11_opy_ (u"ࠩࡥࡶࡴࡽࡳࡦࡴࡶࡸࡦࡩ࡫ࡠࡧࡻࡩࡨࡻࡴࡰࡴ࠽ࠤࢀࠨࡡࡤࡶ࡬ࡳࡳࠨ࠺ࠡࠤࡶࡩࡹ࡙ࡥࡴࡵ࡬ࡳࡳ࡙ࡴࡢࡶࡸࡷࠧ࠲ࠠࠣࡣࡵ࡫ࡺࡳࡥ࡯ࡶࡶࠦ࠿ࠦࡻࠣࡴࡨࡥࡸࡵ࡮ࠣ࠼ࠪట") + json.dumps(bstack11_opy_ (u"ࠥࡗࡨ࡫࡮ࡢࡴ࡬ࡳࠥ࡬ࡡࡪ࡮ࡨࡨࠥࡽࡩࡵࡪ࠽ࠤࠧఠ") + str(message)) + bstack11_opy_ (u"ࠫ࠱ࠨࡳࡵࡣࡷࡹࡸࠨ࠺ࠨడ") + json.dumps(status) + bstack11_opy_ (u"ࠧࢃࡽࠣఢ"))
     else:
-      context.page.evaluate(bstack1ll1_opy_ (u"ࠢࡠࠢࡀࡂࠥࢁࡽࠣ௺"), bstack1ll1_opy_ (u"ࠨࡤࡵࡳࡼࡹࡥࡳࡵࡷࡥࡨࡱ࡟ࡦࡺࡨࡧࡺࡺ࡯ࡳ࠼ࠣࡿࠧࡧࡣࡵ࡫ࡲࡲࠧࡀࠠࠣࡵࡨࡸࡘ࡫ࡳࡴ࡫ࡲࡲࡘࡺࡡࡵࡷࡶࠦ࠱ࠦࠢࡢࡴࡪࡹࡲ࡫࡮ࡵࡵࠥ࠾ࠥࢁࠢࡴࡶࡤࡸࡺࡹࠢ࠻ࠩ௻") + json.dumps(status) + bstack1ll1_opy_ (u"ࠤࢀࢁࠧ௼"))
+      context.page.evaluate(bstack11_opy_ (u"ࠨ࡟ࠡ࠿ࡁࠤࢀࢃࠢణ"), bstack11_opy_ (u"ࠧࡣࡴࡲࡻࡸ࡫ࡲࡴࡶࡤࡧࡰࡥࡥࡹࡧࡦࡹࡹࡵࡲ࠻ࠢࡾࠦࡦࡩࡴࡪࡱࡱࠦ࠿ࠦࠢࡴࡧࡷࡗࡪࡹࡳࡪࡱࡱࡗࡹࡧࡴࡶࡵࠥ࠰ࠥࠨࡡࡳࡩࡸࡱࡪࡴࡴࡴࠤ࠽ࠤࢀࠨࡳࡵࡣࡷࡹࡸࠨ࠺ࠨత") + json.dumps(status) + bstack11_opy_ (u"ࠣࡿࢀࠦథ"))
   except Exception as e:
-    logger.debug(bstack1ll1_opy_ (u"ࠥࡩࡽࡩࡥࡱࡶ࡬ࡳࡳࠦࡩ࡯ࠢࡳࡰࡦࡿࡷࡳ࡫ࡪ࡬ࡹࠦࡳࡦࡶࠣࡷࡪࡹࡳࡪࡱࡱࠤࡸࡺࡡࡵࡷࡶࠤࢀࢃࠢ௽"), e)
-def bstack11llll1l_opy_(self, url):
-  global bstack1l1lll_opy_
+    logger.debug(bstack11_opy_ (u"ࠤࡨࡼࡨ࡫ࡰࡵ࡫ࡲࡲࠥ࡯࡮ࠡࡲ࡯ࡥࡾࡽࡲࡪࡩ࡫ࡸࠥࡹࡥࡵࠢࡶࡩࡸࡹࡩࡰࡰࠣࡷࡹࡧࡴࡶࡵࠣࡿࢂࠨద"), e)
+def bstack1l1l1l1_opy_(self, url):
+  global bstack1lllll11_opy_
   try:
-    bstack1lll111_opy_(url)
+    bstack1l1l1l11l_opy_(url)
   except Exception as err:
-    logger.debug(bstack1l1l1ll1_opy_.format(str(err)))
+    logger.debug(bstack1l1l11l1_opy_.format(str(err)))
   try:
-    bstack1l1lll_opy_(self, url)
+    bstack1lllll11_opy_(self, url)
   except Exception as e:
     try:
-      bstack11llllll_opy_ = str(e)
-      if any(err_msg in bstack11llllll_opy_ for err_msg in bstack1l1l1llll_opy_):
-        bstack1lll111_opy_(url, True)
+      bstack11lllll_opy_ = str(e)
+      if any(err_msg in bstack11lllll_opy_ for err_msg in bstack1l1lll11l_opy_):
+        bstack1l1l1l11l_opy_(url, True)
     except Exception as err:
-      logger.debug(bstack1l1l1ll1_opy_.format(str(err)))
+      logger.debug(bstack1l1l11l1_opy_.format(str(err)))
     raise e
-def bstack11llll1_opy_(self, test):
+def bstack11l111l1_opy_(self, test):
   global CONFIG
-  global bstack1111111_opy_
-  global bstack111lll_opy_
-  global bstack1ll111ll_opy_
-  global bstack1ll1l11l_opy_
-  try:
-    if not bstack1111111_opy_:
-      with open(os.path.join(os.path.expanduser(bstack1ll1_opy_ (u"ࠫࢃ࠭௾")), bstack1ll1_opy_ (u"ࠬ࠴ࡢࡳࡱࡺࡷࡪࡸࡳࡵࡣࡦ࡯ࠬ௿"), bstack1ll1_opy_ (u"࠭࠮ࡴࡧࡶࡷ࡮ࡵ࡮ࡪࡦࡶ࠲ࡹࡾࡴࠨఀ"))) as f:
-        bstack1ll1lllll_opy_ = json.loads(bstack1ll1_opy_ (u"ࠢࡼࠤఁ") + f.read().strip() + bstack1ll1_opy_ (u"ࠨࠤࡻࠦ࠿ࠦࠢࡺࠤࠪం") + bstack1ll1_opy_ (u"ࠤࢀࠦః"))
-        bstack1111111_opy_ = bstack1ll1lllll_opy_[str(threading.get_ident())]
+  global bstack1l1lll1ll_opy_
+  global bstack1l1l1lll_opy_
+  global bstack1ll1l11_opy_
+  global bstack11111ll_opy_
+  try:
+    if not bstack1l1lll1ll_opy_:
+      with open(os.path.join(os.path.expanduser(bstack11_opy_ (u"ࠪࢂࠬధ")), bstack11_opy_ (u"ࠫ࠳ࡨࡲࡰࡹࡶࡩࡷࡹࡴࡢࡥ࡮ࠫన"), bstack11_opy_ (u"ࠬ࠴ࡳࡦࡵࡶ࡭ࡴࡴࡩࡥࡵ࠱ࡸࡽࡺࠧ఩"))) as f:
+        bstack1ll1ll1l_opy_ = json.loads(bstack11_opy_ (u"ࠨࡻࠣప") + f.read().strip() + bstack11_opy_ (u"ࠧࠣࡺࠥ࠾ࠥࠨࡹࠣࠩఫ") + bstack11_opy_ (u"ࠣࡿࠥబ"))
+        bstack1l1lll1ll_opy_ = bstack1ll1ll1l_opy_[str(threading.get_ident())]
   except:
     pass
-  if bstack1111111_opy_:
+  if bstack1l1lll1ll_opy_:
     try:
       data = {}
-      bstack1l1lll1ll_opy_ = None
+      bstack111ll1l_opy_ = None
       if test:
-        bstack1l1lll1ll_opy_ = str(test.data)
-      if bstack1l1lll1ll_opy_ and not bstack1ll111ll_opy_:
-        data[bstack1ll1_opy_ (u"ࠪࡲࡦࡳࡥࠨఄ")] = bstack1l1lll1ll_opy_
-      if bstack111lll_opy_:
-        if bstack111lll_opy_.status == bstack1ll1_opy_ (u"ࠫࡕࡇࡓࡔࠩఅ"):
-          data[bstack1ll1_opy_ (u"ࠬࡹࡴࡢࡶࡸࡷࠬఆ")] = bstack1ll1_opy_ (u"࠭ࡰࡢࡵࡶࡩࡩ࠭ఇ")
-        elif bstack111lll_opy_.status == bstack1ll1_opy_ (u"ࠧࡇࡃࡌࡐࠬఈ"):
-          data[bstack1ll1_opy_ (u"ࠨࡵࡷࡥࡹࡻࡳࠨఉ")] = bstack1ll1_opy_ (u"ࠩࡩࡥ࡮ࡲࡥࡥࠩఊ")
-          if bstack111lll_opy_.message:
-            data[bstack1ll1_opy_ (u"ࠪࡶࡪࡧࡳࡰࡰࠪఋ")] = str(bstack111lll_opy_.message)
-      user = CONFIG[bstack1ll1_opy_ (u"ࠫࡺࡹࡥࡳࡐࡤࡱࡪ࠭ఌ")]
-      key = CONFIG[bstack1ll1_opy_ (u"ࠬࡧࡣࡤࡧࡶࡷࡐ࡫ࡹࠨ఍")]
-      url = bstack1ll1_opy_ (u"࠭ࡨࡵࡶࡳࡷ࠿࠵࠯ࡼࡿ࠽ࡿࢂࡆࡡࡱ࡫࠱ࡦࡷࡵࡷࡴࡧࡵࡷࡹࡧࡣ࡬࠰ࡦࡳࡲ࠵ࡡࡶࡶࡲࡱࡦࡺࡥ࠰ࡵࡨࡷࡸ࡯࡯࡯ࡵ࠲ࡿࢂ࠴ࡪࡴࡱࡱࠫఎ").format(user, key, bstack1111111_opy_)
+        bstack111ll1l_opy_ = str(test.data)
+      if bstack111ll1l_opy_ and not bstack1ll1l11_opy_:
+        data[bstack11_opy_ (u"ࠩࡱࡥࡲ࡫ࠧభ")] = bstack111ll1l_opy_
+      if bstack1l1l1lll_opy_:
+        if bstack1l1l1lll_opy_.status == bstack11_opy_ (u"ࠪࡔࡆ࡙ࡓࠨమ"):
+          data[bstack11_opy_ (u"ࠫࡸࡺࡡࡵࡷࡶࠫయ")] = bstack11_opy_ (u"ࠬࡶࡡࡴࡵࡨࡨࠬర")
+        elif bstack1l1l1lll_opy_.status == bstack11_opy_ (u"࠭ࡆࡂࡋࡏࠫఱ"):
+          data[bstack11_opy_ (u"ࠧࡴࡶࡤࡸࡺࡹࠧల")] = bstack11_opy_ (u"ࠨࡨࡤ࡭ࡱ࡫ࡤࠨళ")
+          if bstack1l1l1lll_opy_.message:
+            data[bstack11_opy_ (u"ࠩࡵࡩࡦࡹ࡯࡯ࠩఴ")] = str(bstack1l1l1lll_opy_.message)
+      user = CONFIG[bstack11_opy_ (u"ࠪࡹࡸ࡫ࡲࡏࡣࡰࡩࠬవ")]
+      key = CONFIG[bstack11_opy_ (u"ࠫࡦࡩࡣࡦࡵࡶࡏࡪࡿࠧశ")]
+      url = bstack11_opy_ (u"ࠬ࡮ࡴࡵࡲࡶ࠾࠴࠵ࡻࡾ࠼ࡾࢁࡅࡧࡰࡪ࠰ࡥࡶࡴࡽࡳࡦࡴࡶࡸࡦࡩ࡫࠯ࡥࡲࡱ࠴ࡧࡵࡵࡱࡰࡥࡹ࡫࠯ࡴࡧࡶࡷ࡮ࡵ࡮ࡴ࠱ࡾࢁ࠳ࡰࡳࡰࡰࠪష").format(user, key, bstack1l1lll1ll_opy_)
       headers = {
-        bstack1ll1_opy_ (u"ࠧࡄࡱࡱࡸࡪࡴࡴ࠮ࡶࡼࡴࡪ࠭ఏ"): bstack1ll1_opy_ (u"ࠨࡣࡳࡴࡱ࡯ࡣࡢࡶ࡬ࡳࡳ࠵ࡪࡴࡱࡱࠫఐ"),
+        bstack11_opy_ (u"࠭ࡃࡰࡰࡷࡩࡳࡺ࠭ࡵࡻࡳࡩࠬస"): bstack11_opy_ (u"ࠧࡢࡲࡳࡰ࡮ࡩࡡࡵ࡫ࡲࡲ࠴ࡰࡳࡰࡰࠪహ"),
       }
       if bool(data):
         requests.put(url, json=data, headers=headers)
     except Exception as e:
-      logger.error(bstack1l1l1ll_opy_.format(str(e)))
-  bstack1ll1l11l_opy_(self, test)
-def bstack1llll1lll_opy_(self, parent, test, skip_on_failure=None, rpa=False):
-  global bstack1111l11l_opy_
-  bstack1111l11l_opy_(self, parent, test, skip_on_failure=skip_on_failure, rpa=rpa)
-  global bstack111lll_opy_
-  bstack111lll_opy_ = self._test
-def bstack1l111_opy_(outs_dir, options, tests_root_name, stats, copied_artifacts, outputfile=None):
+      logger.error(bstack11l11111_opy_.format(str(e)))
+  bstack11111ll_opy_(self, test)
+def bstack1l1ll1l11_opy_(self, parent, test, skip_on_failure=None, rpa=False):
+  global bstack1lll1ll1_opy_
+  bstack1lll1ll1_opy_(self, parent, test, skip_on_failure=skip_on_failure, rpa=rpa)
+  global bstack1l1l1lll_opy_
+  bstack1l1l1lll_opy_ = self._test
+def bstack1lll11l11_opy_(outs_dir, options, tests_root_name, stats, copied_artifacts, outputfile=None):
   from pabot import pabot
-  outputfile = outputfile or options.get(bstack1ll1_opy_ (u"ࠤࡲࡹࡹࡶࡵࡵࠤ఑"), bstack1ll1_opy_ (u"ࠥࡳࡺࡺࡰࡶࡶ࠱ࡼࡲࡲࠢఒ"))
+  outputfile = outputfile or options.get(bstack11_opy_ (u"ࠣࡱࡸࡸࡵࡻࡴࠣ఺"), bstack11_opy_ (u"ࠤࡲࡹࡹࡶࡵࡵ࠰ࡻࡱࡱࠨ఻"))
   output_path = os.path.abspath(
-    os.path.join(options.get(bstack1ll1_opy_ (u"ࠦࡴࡻࡴࡱࡷࡷࡨ࡮ࡸࠢఓ"), bstack1ll1_opy_ (u"ࠧ࠴ࠢఔ")), outputfile)
+    os.path.join(options.get(bstack11_opy_ (u"ࠥࡳࡺࡺࡰࡶࡶࡧ࡭ࡷࠨ఼"), bstack11_opy_ (u"ࠦ࠳ࠨఽ")), outputfile)
   )
-  files = sorted(pabot.glob(os.path.join(pabot._glob_escape(outs_dir), bstack1ll1_opy_ (u"ࠨࠪ࠯ࡺࡰࡰࠧక"))))
+  files = sorted(pabot.glob(os.path.join(pabot._glob_escape(outs_dir), bstack11_opy_ (u"ࠧ࠰࠮ࡹ࡯࡯ࠦా"))))
   if not files:
-    pabot._write(bstack1ll1_opy_ (u"ࠧࡘࡃࡕࡒ࠿ࠦࡎࡰࠢࡲࡹࡹࡶࡵࡵࠢࡩ࡭ࡱ࡫ࡳࠡ࡫ࡱࠤࠧࠫࡳࠣࠩఖ") % outs_dir, pabot.Color.YELLOW)
-    return bstack1ll1_opy_ (u"ࠣࠤగ")
+    pabot._write(bstack11_opy_ (u"࠭ࡗࡂࡔࡑ࠾ࠥࡔ࡯ࠡࡱࡸࡸࡵࡻࡴࠡࡨ࡬ࡰࡪࡹࠠࡪࡰࠣࠦࠪࡹࠢࠨి") % outs_dir, pabot.Color.YELLOW)
+    return bstack11_opy_ (u"ࠢࠣీ")
   def invalid_xml_callback():
     global _ABNORMAL_EXIT_HAPPENED
     _ABNORMAL_EXIT_HAPPENED = True
   resu = pabot.merge(
     files, options, tests_root_name, copied_artifacts, invalid_xml_callback
   )
   pabot._update_stats(resu, stats)
   resu.save(output_path)
   return output_path
-def bstack11111ll1_opy_(outs_dir, pabot_args, options, start_time_string, tests_root_name):
+def bstack1l11ll1l1_opy_(outs_dir, pabot_args, options, start_time_string, tests_root_name):
   from pabot import pabot
   from robot import __version__ as ROBOT_VERSION
   from robot import rebot
-  if bstack1ll1_opy_ (u"ࠤࡳࡽࡹ࡮࡯࡯ࡲࡤࡸ࡭ࠨఘ") in options:
-    del options[bstack1ll1_opy_ (u"ࠥࡴࡾࡺࡨࡰࡰࡳࡥࡹ࡮ࠢఙ")]
-  if ROBOT_VERSION < bstack1ll1_opy_ (u"ࠦ࠹࠴࠰ࠣచ"):
+  if bstack11_opy_ (u"ࠣࡲࡼࡸ࡭ࡵ࡮ࡱࡣࡷ࡬ࠧు") in options:
+    del options[bstack11_opy_ (u"ࠤࡳࡽࡹ࡮࡯࡯ࡲࡤࡸ࡭ࠨూ")]
+  if ROBOT_VERSION < bstack11_opy_ (u"ࠥ࠸࠳࠶ࠢృ"):
     stats = {
-      bstack1ll1_opy_ (u"ࠧࡩࡲࡪࡶ࡬ࡧࡦࡲࠢఛ"): {bstack1ll1_opy_ (u"ࠨࡴࡰࡶࡤࡰࠧజ"): 0, bstack1ll1_opy_ (u"ࠢࡱࡣࡶࡷࡪࡪࠢఝ"): 0, bstack1ll1_opy_ (u"ࠣࡨࡤ࡭ࡱ࡫ࡤࠣఞ"): 0},
-      bstack1ll1_opy_ (u"ࠤࡤࡰࡱࠨట"): {bstack1ll1_opy_ (u"ࠥࡸࡴࡺࡡ࡭ࠤఠ"): 0, bstack1ll1_opy_ (u"ࠦࡵࡧࡳࡴࡧࡧࠦడ"): 0, bstack1ll1_opy_ (u"ࠧ࡬ࡡࡪ࡮ࡨࡨࠧఢ"): 0},
+      bstack11_opy_ (u"ࠦࡨࡸࡩࡵ࡫ࡦࡥࡱࠨౄ"): {bstack11_opy_ (u"ࠧࡺ࡯ࡵࡣ࡯ࠦ౅"): 0, bstack11_opy_ (u"ࠨࡰࡢࡵࡶࡩࡩࠨె"): 0, bstack11_opy_ (u"ࠢࡧࡣ࡬ࡰࡪࡪࠢే"): 0},
+      bstack11_opy_ (u"ࠣࡣ࡯ࡰࠧై"): {bstack11_opy_ (u"ࠤࡷࡳࡹࡧ࡬ࠣ౉"): 0, bstack11_opy_ (u"ࠥࡴࡦࡹࡳࡦࡦࠥొ"): 0, bstack11_opy_ (u"ࠦ࡫ࡧࡩ࡭ࡧࡧࠦో"): 0},
     }
   else:
     stats = {
-      bstack1ll1_opy_ (u"ࠨࡴࡰࡶࡤࡰࠧణ"): 0,
-      bstack1ll1_opy_ (u"ࠢࡱࡣࡶࡷࡪࡪࠢత"): 0,
-      bstack1ll1_opy_ (u"ࠣࡨࡤ࡭ࡱ࡫ࡤࠣథ"): 0,
-      bstack1ll1_opy_ (u"ࠤࡶ࡯࡮ࡶࡰࡦࡦࠥద"): 0,
+      bstack11_opy_ (u"ࠧࡺ࡯ࡵࡣ࡯ࠦౌ"): 0,
+      bstack11_opy_ (u"ࠨࡰࡢࡵࡶࡩࡩࠨ్"): 0,
+      bstack11_opy_ (u"ࠢࡧࡣ࡬ࡰࡪࡪࠢ౎"): 0,
+      bstack11_opy_ (u"ࠣࡵ࡮࡭ࡵࡶࡥࡥࠤ౏"): 0,
     }
-  if pabot_args[bstack1ll1_opy_ (u"ࠥࡆࡘ࡚ࡁࡄࡍࡢࡔࡆࡘࡁࡍࡎࡈࡐࡤࡘࡕࡏࠤధ")]:
+  if pabot_args[bstack11_opy_ (u"ࠤࡅࡗ࡙ࡇࡃࡌࡡࡓࡅࡗࡇࡌࡍࡇࡏࡣࡗ࡛ࡎࠣ౐")]:
     outputs = []
-    for index, _ in enumerate(pabot_args[bstack1ll1_opy_ (u"ࠦࡇ࡙ࡔࡂࡅࡎࡣࡕࡇࡒࡂࡎࡏࡉࡑࡥࡒࡖࡐࠥన")]):
+    for index, _ in enumerate(pabot_args[bstack11_opy_ (u"ࠥࡆࡘ࡚ࡁࡄࡍࡢࡔࡆࡘࡁࡍࡎࡈࡐࡤࡘࡕࡏࠤ౑")]):
       copied_artifacts = pabot._copy_output_artifacts(
-        options, pabot_args[bstack1ll1_opy_ (u"ࠧࡧࡲࡵ࡫ࡩࡥࡨࡺࡳࠣ఩")], pabot_args[bstack1ll1_opy_ (u"ࠨࡡࡳࡶ࡬ࡪࡦࡩࡴࡴ࡫ࡱࡷࡺࡨࡦࡰ࡮ࡧࡩࡷࡹࠢప")]
+        options, pabot_args[bstack11_opy_ (u"ࠦࡦࡸࡴࡪࡨࡤࡧࡹࡹࠢ౒")], pabot_args[bstack11_opy_ (u"ࠧࡧࡲࡵ࡫ࡩࡥࡨࡺࡳࡪࡰࡶࡹࡧ࡬࡯࡭ࡦࡨࡶࡸࠨ౓")]
       )
       outputs += [
-        bstack1l111_opy_(
-          os.path.join(outs_dir, str(index)+ bstack1ll1_opy_ (u"ࠢ࠰ࠤఫ")),
+        bstack1lll11l11_opy_(
+          os.path.join(outs_dir, str(index)+ bstack11_opy_ (u"ࠨ࠯ࠣ౔")),
           options,
           tests_root_name,
           stats,
           copied_artifacts,
-          outputfile=os.path.join(bstack1ll1_opy_ (u"ࠣࡲࡤࡦࡴࡺ࡟ࡳࡧࡶࡹࡱࡺࡳࠣబ"), bstack1ll1_opy_ (u"ࠤࡲࡹࡹࡶࡵࡵࠧࡶ࠲ࡽࡳ࡬ࠣభ") % index),
+          outputfile=os.path.join(bstack11_opy_ (u"ࠢࡱࡣࡥࡳࡹࡥࡲࡦࡵࡸࡰࡹࡹౕࠢ"), bstack11_opy_ (u"ࠣࡱࡸࡸࡵࡻࡴࠦࡵ࠱ࡼࡲࡲౖࠢ") % index),
         )
       ]
-    if bstack1ll1_opy_ (u"ࠥࡳࡺࡺࡰࡶࡶࠥమ") not in options:
-      options[bstack1ll1_opy_ (u"ࠦࡴࡻࡴࡱࡷࡷࠦయ")] = bstack1ll1_opy_ (u"ࠧࡵࡵࡵࡲࡸࡸ࠳ࡾ࡭࡭ࠤర")
+    if bstack11_opy_ (u"ࠤࡲࡹࡹࡶࡵࡵࠤ౗") not in options:
+      options[bstack11_opy_ (u"ࠥࡳࡺࡺࡰࡶࡶࠥౘ")] = bstack11_opy_ (u"ࠦࡴࡻࡴࡱࡷࡷ࠲ࡽࡳ࡬ࠣౙ")
     pabot._write_stats(stats)
     return rebot(*outputs, **pabot._options_for_rebot(options, start_time_string, pabot._now()))
   else:
     return pabot._report_results(outs_dir, pabot_args, options, start_time_string, tests_root_name)
-def bstack1l111l1l_opy_(self, ff_profile_dir):
-  global bstack11l11ll1_opy_
+def bstack1l11l1_opy_(self, ff_profile_dir):
+  global bstack11ll_opy_
   if not ff_profile_dir:
     return None
-  return bstack11l11ll1_opy_(self, ff_profile_dir)
-def bstack1ll11ll1l_opy_(datasources, opts_for_run, outs_dir, pabot_args, suite_group):
+  return bstack11ll_opy_(self, ff_profile_dir)
+def bstack11l1_opy_(datasources, opts_for_run, outs_dir, pabot_args, suite_group):
   from pabot.pabot import QueueItem
   global CONFIG
-  global bstack111l1lll_opy_
-  bstack1l1l1l1l1_opy_ = []
-  if bstack1ll1_opy_ (u"࠭ࡰ࡭ࡣࡷࡪࡴࡸ࡭ࡴࠩఱ") in CONFIG:
-    bstack1l1l1l1l1_opy_ = CONFIG[bstack1ll1_opy_ (u"ࠧࡱ࡮ࡤࡸ࡫ࡵࡲ࡮ࡵࠪల")]
-  bstack1lll1l1_opy_ = len(suite_group) * len(pabot_args[bstack1ll1_opy_ (u"ࠣࡣࡵ࡫ࡺࡳࡥ࡯ࡶࡩ࡭ࡱ࡫ࡳࠣళ")] or [(bstack1ll1_opy_ (u"ࠤࠥఴ"), None)]) * len(bstack1l1l1l1l1_opy_)
-  pabot_args[bstack1ll1_opy_ (u"ࠥࡆࡘ࡚ࡁࡄࡍࡢࡔࡆࡘࡁࡍࡎࡈࡐࡤࡘࡕࡏࠤవ")] = []
-  for q in range(bstack1lll1l1_opy_):
-    pabot_args[bstack1ll1_opy_ (u"ࠦࡇ࡙ࡔࡂࡅࡎࡣࡕࡇࡒࡂࡎࡏࡉࡑࡥࡒࡖࡐࠥశ")].append(str(q))
+  global bstack1l11l111_opy_
+  bstack1l1llll1_opy_ = []
+  if bstack11_opy_ (u"ࠬࡶ࡬ࡢࡶࡩࡳࡷࡳࡳࠨౚ") in CONFIG:
+    bstack1l1llll1_opy_ = CONFIG[bstack11_opy_ (u"࠭ࡰ࡭ࡣࡷࡪࡴࡸ࡭ࡴࠩ౛")]
+  bstack1lllll1ll_opy_ = len(suite_group) * len(pabot_args[bstack11_opy_ (u"ࠢࡢࡴࡪࡹࡲ࡫࡮ࡵࡨ࡬ࡰࡪࡹࠢ౜")] or [(bstack11_opy_ (u"ࠣࠤౝ"), None)]) * len(bstack1l1llll1_opy_)
+  pabot_args[bstack11_opy_ (u"ࠤࡅࡗ࡙ࡇࡃࡌࡡࡓࡅࡗࡇࡌࡍࡇࡏࡣࡗ࡛ࡎࠣ౞")] = []
+  for q in range(bstack1lllll1ll_opy_):
+    pabot_args[bstack11_opy_ (u"ࠥࡆࡘ࡚ࡁࡄࡍࡢࡔࡆࡘࡁࡍࡎࡈࡐࡤࡘࡕࡏࠤ౟")].append(str(q))
   return [
     QueueItem(
       datasources,
       outs_dir,
       opts_for_run,
       suite,
-      pabot_args[bstack1ll1_opy_ (u"ࠧࡩ࡯࡮࡯ࡤࡲࡩࠨష")],
-      pabot_args[bstack1ll1_opy_ (u"ࠨࡶࡦࡴࡥࡳࡸ࡫ࠢస")],
+      pabot_args[bstack11_opy_ (u"ࠦࡨࡵ࡭࡮ࡣࡱࡨࠧౠ")],
+      pabot_args[bstack11_opy_ (u"ࠧࡼࡥࡳࡤࡲࡷࡪࠨౡ")],
       argfile,
-      pabot_args.get(bstack1ll1_opy_ (u"ࠢࡩ࡫ࡹࡩࠧహ")),
-      pabot_args[bstack1ll1_opy_ (u"ࠣࡲࡵࡳࡨ࡫ࡳࡴࡧࡶࠦ఺")],
+      pabot_args.get(bstack11_opy_ (u"ࠨࡨࡪࡸࡨࠦౢ")),
+      pabot_args[bstack11_opy_ (u"ࠢࡱࡴࡲࡧࡪࡹࡳࡦࡵࠥౣ")],
       platform[0],
-      bstack111l1lll_opy_
+      bstack1l11l111_opy_
     )
     for suite in suite_group
-    for argfile in pabot_args[bstack1ll1_opy_ (u"ࠤࡤࡶ࡬ࡻ࡭ࡦࡰࡷࡪ࡮ࡲࡥࡴࠤ఻")] or [(bstack1ll1_opy_ (u"఼ࠥࠦ"), None)]
-    for platform in enumerate(bstack1l1l1l1l1_opy_)
+    for argfile in pabot_args[bstack11_opy_ (u"ࠣࡣࡵ࡫ࡺࡳࡥ࡯ࡶࡩ࡭ࡱ࡫ࡳࠣ౤")] or [(bstack11_opy_ (u"ࠤࠥ౥"), None)]
+    for platform in enumerate(bstack1l1llll1_opy_)
   ]
-def bstack1l1111_opy_(self, datasources, outs_dir, options,
+def bstack1ll1l11l1_opy_(self, datasources, outs_dir, options,
   execution_item, command, verbose, argfile,
-  hive=None, processes=0,platform_index=0,bstack1l1lll111_opy_=bstack1ll1_opy_ (u"ࠫࠬఽ")):
-  global bstack1111l1ll_opy_
+  hive=None, processes=0,platform_index=0,bstack1ll1l_opy_=bstack11_opy_ (u"ࠪࠫ౦")):
+  global bstack11ll1l_opy_
   self.platform_index = platform_index
-  self.bstack1111l1_opy_ = bstack1l1lll111_opy_
-  bstack1111l1ll_opy_(self, datasources, outs_dir, options,
+  self.bstack1l11ll11_opy_ = bstack1ll1l_opy_
+  bstack11ll1l_opy_(self, datasources, outs_dir, options,
     execution_item, command, verbose, argfile, hive, processes)
-def bstack1ll1ll1l1_opy_(caller_id, datasources, is_last, item, outs_dir):
-  global bstack1ll11111_opy_
-  global bstack11l1l11l_opy_
-  if not bstack1ll1_opy_ (u"ࠬࡼࡡࡳ࡫ࡤࡦࡱ࡫ࠧా") in item.options:
-    item.options[bstack1ll1_opy_ (u"࠭ࡶࡢࡴ࡬ࡥࡧࡲࡥࠨి")] = []
-  for v in item.options[bstack1ll1_opy_ (u"ࠧࡷࡣࡵ࡭ࡦࡨ࡬ࡦࠩీ")]:
-    if bstack1ll1_opy_ (u"ࠨࡄࡖࡘࡆࡉࡋࡑࡎࡄࡘࡋࡕࡒࡎࡋࡑࡈࡊ࡞ࠧు") in v:
-      item.options[bstack1ll1_opy_ (u"ࠩࡹࡥࡷ࡯ࡡࡣ࡮ࡨࠫూ")].remove(v)
-    if bstack1ll1_opy_ (u"ࠪࡆࡘ࡚ࡁࡄࡍࡆࡐࡎࡇࡒࡈࡕࠪృ") in v:
-      item.options[bstack1ll1_opy_ (u"ࠫࡻࡧࡲࡪࡣࡥࡰࡪ࠭ౄ")].remove(v)
-  item.options[bstack1ll1_opy_ (u"ࠬࡼࡡࡳ࡫ࡤࡦࡱ࡫ࠧ౅")].insert(0, bstack1ll1_opy_ (u"࠭ࡂࡔࡖࡄࡇࡐࡖࡌࡂࡖࡉࡓࡗࡓࡉࡏࡆࡈ࡜࠿ࢁࡽࠨె").format(item.platform_index))
-  item.options[bstack1ll1_opy_ (u"ࠧࡷࡣࡵ࡭ࡦࡨ࡬ࡦࠩే")].insert(0, bstack1ll1_opy_ (u"ࠨࡄࡖࡘࡆࡉࡋࡅࡇࡉࡐࡔࡉࡁࡍࡋࡇࡉࡓ࡚ࡉࡇࡋࡈࡖ࠿ࢁࡽࠨై").format(item.bstack1111l1_opy_))
-  if bstack11l1l11l_opy_:
-    item.options[bstack1ll1_opy_ (u"ࠩࡹࡥࡷ࡯ࡡࡣ࡮ࡨࠫ౉")].insert(0, bstack1ll1_opy_ (u"ࠪࡆࡘ࡚ࡁࡄࡍࡆࡐࡎࡇࡒࡈࡕ࠽ࡿࢂ࠭ొ").format(bstack11l1l11l_opy_))
-  return bstack1ll11111_opy_(caller_id, datasources, is_last, item, outs_dir)
-def bstack1111ll1l_opy_(command):
-  global bstack11l1l11l_opy_
-  if bstack11l1l11l_opy_:
-    command[0] = command[0].replace(bstack1ll1_opy_ (u"ࠫࡷࡵࡢࡰࡶࠪో"), bstack1ll1_opy_ (u"ࠬࡨࡲࡰࡹࡶࡩࡷࡹࡴࡢࡥ࡮࠱ࡸࡪ࡫ࠡࡴࡲࡦࡴࡺ࠭ࡪࡰࡷࡩࡷࡴࡡ࡭ࠢࠪౌ") + bstack11l1l11l_opy_, 1)
+def bstack1ll11_opy_(caller_id, datasources, is_last, item, outs_dir):
+  global bstack1111ll11_opy_
+  global bstack11llll1l_opy_
+  if not bstack11_opy_ (u"ࠫࡻࡧࡲࡪࡣࡥࡰࡪ࠭౧") in item.options:
+    item.options[bstack11_opy_ (u"ࠬࡼࡡࡳ࡫ࡤࡦࡱ࡫ࠧ౨")] = []
+  for v in item.options[bstack11_opy_ (u"࠭ࡶࡢࡴ࡬ࡥࡧࡲࡥࠨ౩")]:
+    if bstack11_opy_ (u"ࠧࡃࡕࡗࡅࡈࡑࡐࡍࡃࡗࡊࡔࡘࡍࡊࡐࡇࡉ࡝࠭౪") in v:
+      item.options[bstack11_opy_ (u"ࠨࡸࡤࡶ࡮ࡧࡢ࡭ࡧࠪ౫")].remove(v)
+    if bstack11_opy_ (u"ࠩࡅࡗ࡙ࡇࡃࡌࡅࡏࡍࡆࡘࡇࡔࠩ౬") in v:
+      item.options[bstack11_opy_ (u"ࠪࡺࡦࡸࡩࡢࡤ࡯ࡩࠬ౭")].remove(v)
+  item.options[bstack11_opy_ (u"ࠫࡻࡧࡲࡪࡣࡥࡰࡪ࠭౮")].insert(0, bstack11_opy_ (u"ࠬࡈࡓࡕࡃࡆࡏࡕࡒࡁࡕࡈࡒࡖࡒࡏࡎࡅࡇ࡛࠾ࢀࢃࠧ౯").format(item.platform_index))
+  item.options[bstack11_opy_ (u"࠭ࡶࡢࡴ࡬ࡥࡧࡲࡥࠨ౰")].insert(0, bstack11_opy_ (u"ࠧࡃࡕࡗࡅࡈࡑࡄࡆࡈࡏࡓࡈࡇࡌࡊࡆࡈࡒ࡙ࡏࡆࡊࡇࡕ࠾ࢀࢃࠧ౱").format(item.bstack1l11ll11_opy_))
+  if bstack11llll1l_opy_:
+    item.options[bstack11_opy_ (u"ࠨࡸࡤࡶ࡮ࡧࡢ࡭ࡧࠪ౲")].insert(0, bstack11_opy_ (u"ࠩࡅࡗ࡙ࡇࡃࡌࡅࡏࡍࡆࡘࡇࡔ࠼ࡾࢁࠬ౳").format(bstack11llll1l_opy_))
+  return bstack1111ll11_opy_(caller_id, datasources, is_last, item, outs_dir)
+def bstack1lll1ll11_opy_(command):
+  global bstack11llll1l_opy_
+  if bstack11llll1l_opy_:
+    command[0] = command[0].replace(bstack11_opy_ (u"ࠪࡶࡴࡨ࡯ࡵࠩ౴"), bstack11_opy_ (u"ࠫࡧࡸ࡯ࡸࡵࡨࡶࡸࡺࡡࡤ࡭࠰ࡷࡩࡱࠠࡳࡱࡥࡳࡹ࠳ࡩ࡯ࡶࡨࡶࡳࡧ࡬ࠡࠩ౵") + bstack11llll1l_opy_, 1)
   else:
-    command[0] = command[0].replace(bstack1ll1_opy_ (u"࠭ࡲࡰࡤࡲࡸ్ࠬ"), bstack1ll1_opy_ (u"ࠧࡣࡴࡲࡻࡸ࡫ࡲࡴࡶࡤࡧࡰ࠳ࡳࡥ࡭ࠣࡶࡴࡨ࡯ࡵ࠯࡬ࡲࡹ࡫ࡲ࡯ࡣ࡯ࠫ౎"), 1)
-def bstack1lll1l1ll_opy_(command, stderr, stdout, item_name, verbose, pool_id, item_index):
-  global bstack1ll111_opy_
-  bstack1111ll1l_opy_(command)
-  return bstack1ll111_opy_(command, stderr, stdout, item_name, verbose, pool_id, item_index)
-def bstack1l1111ll_opy_(command, stderr, stdout, item_name, verbose, pool_id, item_index, outs_dir):
-  global bstack1ll111_opy_
-  bstack1111ll1l_opy_(command)
-  return bstack1ll111_opy_(command, stderr, stdout, item_name, verbose, pool_id, item_index, outs_dir)
-def bstack1ll1ll11l_opy_(command, stderr, stdout, item_name, verbose, pool_id, item_index, outs_dir, process_timeout):
-  global bstack1ll111_opy_
-  bstack1111ll1l_opy_(command)
-  return bstack1ll111_opy_(command, stderr, stdout, item_name, verbose, pool_id, item_index, outs_dir, process_timeout)
-def bstack1ll11l111_opy_(self, runner, quiet=False, capture=True):
-  global bstack1ll1111_opy_
-  bstack1l11llll_opy_ = bstack1ll1111_opy_(self, runner, quiet=False, capture=True)
+    command[0] = command[0].replace(bstack11_opy_ (u"ࠬࡸ࡯ࡣࡱࡷࠫ౶"), bstack11_opy_ (u"࠭ࡢࡳࡱࡺࡷࡪࡸࡳࡵࡣࡦ࡯࠲ࡹࡤ࡬ࠢࡵࡳࡧࡵࡴ࠮࡫ࡱࡸࡪࡸ࡮ࡢ࡮ࠪ౷"), 1)
+def bstack1l1l11lll_opy_(command, stderr, stdout, item_name, verbose, pool_id, item_index):
+  global bstack1l11ll1_opy_
+  bstack1lll1ll11_opy_(command)
+  return bstack1l11ll1_opy_(command, stderr, stdout, item_name, verbose, pool_id, item_index)
+def bstack1l11llll1_opy_(command, stderr, stdout, item_name, verbose, pool_id, item_index, outs_dir):
+  global bstack1l11ll1_opy_
+  bstack1lll1ll11_opy_(command)
+  return bstack1l11ll1_opy_(command, stderr, stdout, item_name, verbose, pool_id, item_index, outs_dir)
+def bstack1l11_opy_(command, stderr, stdout, item_name, verbose, pool_id, item_index, outs_dir, process_timeout):
+  global bstack1l11ll1_opy_
+  bstack1lll1ll11_opy_(command)
+  return bstack1l11ll1_opy_(command, stderr, stdout, item_name, verbose, pool_id, item_index, outs_dir, process_timeout)
+def bstack1111lll_opy_(self, runner, quiet=False, capture=True):
+  global bstack111l1ll_opy_
+  bstack1111l1l1_opy_ = bstack111l1ll_opy_(self, runner, quiet=False, capture=True)
   if self.exception:
-    if not hasattr(runner, bstack1ll1_opy_ (u"ࠨࡧࡻࡧࡪࡶࡴࡪࡱࡱࡣࡦࡸࡲࠨ౏")):
+    if not hasattr(runner, bstack11_opy_ (u"ࠧࡦࡺࡦࡩࡵࡺࡩࡰࡰࡢࡥࡷࡸࠧ౸")):
       runner.exception_arr = []
-    if not hasattr(runner, bstack1ll1_opy_ (u"ࠩࡨࡼࡨࡥࡴࡳࡣࡦࡩࡧࡧࡣ࡬ࡡࡤࡶࡷ࠭౐")):
+    if not hasattr(runner, bstack11_opy_ (u"ࠨࡧࡻࡧࡤࡺࡲࡢࡥࡨࡦࡦࡩ࡫ࡠࡣࡵࡶࠬ౹")):
       runner.exc_traceback_arr = []
     runner.exception = self.exception
     runner.exc_traceback = self.exc_traceback
     runner.exception_arr.append(self.exception)
     runner.exc_traceback_arr.append(self.exc_traceback)
-  return bstack1l11llll_opy_
-def bstack1l1l111l1_opy_(self, name, context, *args):
-  global bstack1l1ll11ll_opy_
-  if name in [bstack1ll1_opy_ (u"ࠪࡦࡪ࡬࡯ࡳࡧࡢࡪࡪࡧࡴࡶࡴࡨࠫ౑"), bstack1ll1_opy_ (u"ࠫࡧ࡫ࡦࡰࡴࡨࡣࡸࡩࡥ࡯ࡣࡵ࡭ࡴ࠭౒")]:
-    bstack1l1ll11ll_opy_(self, name, context, *args)
-  if name == bstack1ll1_opy_ (u"ࠬࡨࡥࡧࡱࡵࡩࡤ࡬ࡥࡢࡶࡸࡶࡪ࠭౓"):
-    try:
-      bstack11l11l1_opy_ = str(self.feature.name)
-      bstack11llll_opy_(context, bstack11l11l1_opy_)
-      context.browser.execute_script(bstack1ll1_opy_ (u"࠭ࡢࡳࡱࡺࡷࡪࡸࡳࡵࡣࡦ࡯ࡤ࡫ࡸࡦࡥࡸࡸࡴࡸ࠺ࠡࡽࠥࡥࡨࡺࡩࡰࡰࠥ࠾ࠥࠨࡳࡦࡶࡖࡩࡸࡹࡩࡰࡰࡑࡥࡲ࡫ࠢ࠭ࠢࠥࡥࡷ࡭ࡵ࡮ࡧࡱࡸࡸࠨ࠺ࠡࡽࠥࡲࡦࡳࡥࠣ࠼ࠣࠫ౔") + json.dumps(bstack11l11l1_opy_) + bstack1ll1_opy_ (u"ࠧࡾࡿౕࠪ"))
+  return bstack1111l1l1_opy_
+def bstack1ll1l1111_opy_(self, name, context, *args):
+  global bstack11l11ll1_opy_
+  if name in [bstack11_opy_ (u"ࠩࡥࡩ࡫ࡵࡲࡦࡡࡩࡩࡦࡺࡵࡳࡧࠪ౺"), bstack11_opy_ (u"ࠪࡦࡪ࡬࡯ࡳࡧࡢࡷࡨ࡫࡮ࡢࡴ࡬ࡳࠬ౻")]:
+    bstack11l11ll1_opy_(self, name, context, *args)
+  if name == bstack11_opy_ (u"ࠫࡧ࡫ࡦࡰࡴࡨࡣ࡫࡫ࡡࡵࡷࡵࡩࠬ౼"):
+    try:
+      bstack1lllllll1_opy_ = str(self.feature.name)
+      bstack1l11lll1l_opy_(context, bstack1lllllll1_opy_)
+      context.browser.execute_script(bstack11_opy_ (u"ࠬࡨࡲࡰࡹࡶࡩࡷࡹࡴࡢࡥ࡮ࡣࡪࡾࡥࡤࡷࡷࡳࡷࡀࠠࡼࠤࡤࡧࡹ࡯࡯࡯ࠤ࠽ࠤࠧࡹࡥࡵࡕࡨࡷࡸ࡯࡯࡯ࡐࡤࡱࡪࠨࠬࠡࠤࡤࡶ࡬ࡻ࡭ࡦࡰࡷࡷࠧࡀࠠࡼࠤࡱࡥࡲ࡫ࠢ࠻ࠢࠪ౽") + json.dumps(bstack1lllllll1_opy_) + bstack11_opy_ (u"࠭ࡽࡾࠩ౾"))
       self.driver_before_scenario = False
     except Exception as e:
-      logger.debug(bstack1ll1_opy_ (u"ࠨࡈࡤ࡭ࡱ࡫ࡤࠡࡶࡲࠤࡸ࡫ࡴࠡࡵࡨࡷࡸ࡯࡯࡯ࠢࡱࡥࡲ࡫ࠠࡪࡰࠣࡦࡪ࡬࡯ࡳࡧࠣࡪࡪࡧࡴࡶࡴࡨ࠾ࠥࢁࡽࠨౖ").format(str(e)))
-  if name == bstack1ll1_opy_ (u"ࠩࡥࡩ࡫ࡵࡲࡦࡡࡶࡧࡪࡴࡡࡳ࡫ࡲࠫ౗"):
+      logger.debug(bstack11_opy_ (u"ࠧࡇࡣ࡬ࡰࡪࡪࠠࡵࡱࠣࡷࡪࡺࠠࡴࡧࡶࡷ࡮ࡵ࡮ࠡࡰࡤࡱࡪࠦࡩ࡯ࠢࡥࡩ࡫ࡵࡲࡦࠢࡩࡩࡦࡺࡵࡳࡧ࠽ࠤࢀࢃࠧ౿").format(str(e)))
+  if name == bstack11_opy_ (u"ࠨࡤࡨࡪࡴࡸࡥࡠࡵࡦࡩࡳࡧࡲࡪࡱࠪಀ"):
     try:
-      if not hasattr(self, bstack1ll1_opy_ (u"ࠪࡨࡷ࡯ࡶࡦࡴࡢࡦࡪ࡬࡯ࡳࡧࡢࡷࡨ࡫࡮ࡢࡴ࡬ࡳࠬౘ")):
+      if not hasattr(self, bstack11_opy_ (u"ࠩࡧࡶ࡮ࡼࡥࡳࡡࡥࡩ࡫ࡵࡲࡦࡡࡶࡧࡪࡴࡡࡳ࡫ࡲࠫಁ")):
         self.driver_before_scenario = True
-      bstack1l11ll_opy_ = args[0].name
-      bstack1l1lll11_opy_ = bstack11l11l1_opy_ = str(self.feature.name)
-      bstack11l11l1_opy_ = bstack1l1lll11_opy_ + bstack1ll1_opy_ (u"ࠫࠥ࠳ࠠࠨౙ") + bstack1l11ll_opy_
+      bstack1lll1l111_opy_ = args[0].name
+      bstack1ll1l11l_opy_ = bstack1lllllll1_opy_ = str(self.feature.name)
+      bstack1lllllll1_opy_ = bstack1ll1l11l_opy_ + bstack11_opy_ (u"ࠪࠤ࠲ࠦࠧಂ") + bstack1lll1l111_opy_
       if self.driver_before_scenario:
-        bstack11llll_opy_(context, bstack11l11l1_opy_)
-        context.browser.execute_script(bstack1ll1_opy_ (u"ࠬࡨࡲࡰࡹࡶࡩࡷࡹࡴࡢࡥ࡮ࡣࡪࡾࡥࡤࡷࡷࡳࡷࡀࠠࡼࠤࡤࡧࡹ࡯࡯࡯ࠤ࠽ࠤࠧࡹࡥࡵࡕࡨࡷࡸ࡯࡯࡯ࡐࡤࡱࡪࠨࠬࠡࠤࡤࡶ࡬ࡻ࡭ࡦࡰࡷࡷࠧࡀࠠࡼࠤࡱࡥࡲ࡫ࠢ࠻ࠢࠪౚ") + json.dumps(bstack11l11l1_opy_) + bstack1ll1_opy_ (u"࠭ࡽࡾࠩ౛"))
+        bstack1l11lll1l_opy_(context, bstack1lllllll1_opy_)
+        context.browser.execute_script(bstack11_opy_ (u"ࠫࡧࡸ࡯ࡸࡵࡨࡶࡸࡺࡡࡤ࡭ࡢࡩࡽ࡫ࡣࡶࡶࡲࡶ࠿ࠦࡻࠣࡣࡦࡸ࡮ࡵ࡮ࠣ࠼ࠣࠦࡸ࡫ࡴࡔࡧࡶࡷ࡮ࡵ࡮ࡏࡣࡰࡩࠧ࠲ࠠࠣࡣࡵ࡫ࡺࡳࡥ࡯ࡶࡶࠦ࠿ࠦࡻࠣࡰࡤࡱࡪࠨ࠺ࠡࠩಃ") + json.dumps(bstack1lllllll1_opy_) + bstack11_opy_ (u"ࠬࢃࡽࠨ಄"))
     except Exception as e:
-      logger.debug(bstack1ll1_opy_ (u"ࠧࡇࡣ࡬ࡰࡪࡪࠠࡵࡱࠣࡷࡪࡺࠠࡴࡧࡶࡷ࡮ࡵ࡮ࠡࡰࡤࡱࡪࠦࡩ࡯ࠢࡥࡩ࡫ࡵࡲࡦࠢࡶࡧࡪࡴࡡࡳ࡫ࡲ࠾ࠥࢁࡽࠨ౜").format(str(e)))
-  if name == bstack1ll1_opy_ (u"ࠨࡣࡩࡸࡪࡸ࡟ࡴࡥࡨࡲࡦࡸࡩࡰࠩౝ"):
+      logger.debug(bstack11_opy_ (u"࠭ࡆࡢ࡫࡯ࡩࡩࠦࡴࡰࠢࡶࡩࡹࠦࡳࡦࡵࡶ࡭ࡴࡴࠠ࡯ࡣࡰࡩࠥ࡯࡮ࠡࡤࡨࡪࡴࡸࡥࠡࡵࡦࡩࡳࡧࡲࡪࡱ࠽ࠤࢀࢃࠧಅ").format(str(e)))
+  if name == bstack11_opy_ (u"ࠧࡢࡨࡷࡩࡷࡥࡳࡤࡧࡱࡥࡷ࡯࡯ࠨಆ"):
     try:
-      bstack1llll11_opy_ = args[0].status.name
-      if str(bstack1llll11_opy_).lower() == bstack1ll1_opy_ (u"ࠩࡩࡥ࡮ࡲࡥࡥࠩ౞"):
-        bstack11lll1l_opy_ = bstack1ll1_opy_ (u"ࠪࠫ౟")
-        bstack1l1lllll1_opy_ = bstack1ll1_opy_ (u"ࠫࠬౠ")
-        bstack1llllll1_opy_ = bstack1ll1_opy_ (u"ࠬ࠭ౡ")
+      bstack1llll1l1_opy_ = args[0].status.name
+      if str(bstack1llll1l1_opy_).lower() == bstack11_opy_ (u"ࠨࡨࡤ࡭ࡱ࡫ࡤࠨಇ"):
+        bstack11ll1l1_opy_ = bstack11_opy_ (u"ࠩࠪಈ")
+        bstack1l11111l1_opy_ = bstack11_opy_ (u"ࠪࠫಉ")
+        bstack1l1ll1111_opy_ = bstack11_opy_ (u"ࠫࠬಊ")
         try:
           import traceback
-          bstack11lll1l_opy_ = self.exception.__class__.__name__
-          bstack1lll1l1l1_opy_ = traceback.format_tb(self.exc_traceback)
-          bstack1l1lllll1_opy_ = bstack1ll1_opy_ (u"࠭ࠠࠨౢ").join(bstack1lll1l1l1_opy_)
-          bstack1llllll1_opy_ = bstack1lll1l1l1_opy_[-1]
+          bstack11ll1l1_opy_ = self.exception.__class__.__name__
+          bstack11llll_opy_ = traceback.format_tb(self.exc_traceback)
+          bstack1l11111l1_opy_ = bstack11_opy_ (u"ࠬࠦࠧಋ").join(bstack11llll_opy_)
+          bstack1l1ll1111_opy_ = bstack11llll_opy_[-1]
         except Exception as e:
-          logger.debug(bstack1l1l1ll1l_opy_.format(str(e)))
-        bstack11lll1l_opy_ += bstack1llllll1_opy_
-        bstack1ll1l1l_opy_(context, json.dumps(str(args[0].name) + bstack1ll1_opy_ (u"ࠢࠡ࠯ࠣࡊࡦ࡯࡬ࡦࡦࠤࡠࡳࠨౣ") + str(bstack1l1lllll1_opy_)), bstack1ll1_opy_ (u"ࠣࡧࡵࡶࡴࡸࠢ౤"))
+          logger.debug(bstack1l1l1ll_opy_.format(str(e)))
+        bstack11ll1l1_opy_ += bstack1l1ll1111_opy_
+        bstack11l1111_opy_(context, json.dumps(str(args[0].name) + bstack11_opy_ (u"ࠨࠠ࠮ࠢࡉࡥ࡮ࡲࡥࡥࠣ࡟ࡲࠧಌ") + str(bstack1l11111l1_opy_)), bstack11_opy_ (u"ࠢࡦࡴࡵࡳࡷࠨ಍"))
         if self.driver_before_scenario:
-          bstack11ll1ll1_opy_(context, bstack1ll1_opy_ (u"ࠤࡩࡥ࡮ࡲࡥࡥࠤ౥"), bstack11lll1l_opy_)
-        context.browser.execute_script(bstack1ll1_opy_ (u"ࠪࡦࡷࡵࡷࡴࡧࡵࡷࡹࡧࡣ࡬ࡡࡨࡼࡪࡩࡵࡵࡱࡵ࠾ࠥࢁࠢࡢࡥࡷ࡭ࡴࡴࠢ࠻ࠢࠥࡥࡳࡴ࡯ࡵࡣࡷࡩࠧ࠲ࠠࠣࡣࡵ࡫ࡺࡳࡥ࡯ࡶࡶࠦ࠿ࠦࡻࠣࡦࡤࡸࡦࠨ࠺ࠨ౦") + json.dumps(str(args[0].name) + bstack1ll1_opy_ (u"ࠦࠥ࠳ࠠࡇࡣ࡬ࡰࡪࡪࠡ࡝ࡰࠥ౧") + str(bstack1l1lllll1_opy_)) + bstack1ll1_opy_ (u"ࠬ࠲ࠠࠣ࡮ࡨࡺࡪࡲࠢ࠻ࠢࠥࡩࡷࡸ࡯ࡳࠤࢀࢁࠬ౨"))
+          bstack1llll111l_opy_(context, bstack11_opy_ (u"ࠣࡨࡤ࡭ࡱ࡫ࡤࠣಎ"), bstack11ll1l1_opy_)
+        context.browser.execute_script(bstack11_opy_ (u"ࠩࡥࡶࡴࡽࡳࡦࡴࡶࡸࡦࡩ࡫ࡠࡧࡻࡩࡨࡻࡴࡰࡴ࠽ࠤࢀࠨࡡࡤࡶ࡬ࡳࡳࠨ࠺ࠡࠤࡤࡲࡳࡵࡴࡢࡶࡨࠦ࠱ࠦࠢࡢࡴࡪࡹࡲ࡫࡮ࡵࡵࠥ࠾ࠥࢁࠢࡥࡣࡷࡥࠧࡀࠧಏ") + json.dumps(str(args[0].name) + bstack11_opy_ (u"ࠥࠤ࠲ࠦࡆࡢ࡫࡯ࡩࡩࠧ࡜࡯ࠤಐ") + str(bstack1l11111l1_opy_)) + bstack11_opy_ (u"ࠫ࠱ࠦࠢ࡭ࡧࡹࡩࡱࠨ࠺ࠡࠤࡨࡶࡷࡵࡲࠣࡿࢀࠫ಑"))
         if self.driver_before_scenario:
-          context.browser.execute_script(bstack1ll1_opy_ (u"࠭ࡢࡳࡱࡺࡷࡪࡸࡳࡵࡣࡦ࡯ࡤ࡫ࡸࡦࡥࡸࡸࡴࡸ࠺ࠡࡽࠥࡥࡨࡺࡩࡰࡰࠥ࠾ࠥࠨࡳࡦࡶࡖࡩࡸࡹࡩࡰࡰࡖࡸࡦࡺࡵࡴࠤ࠯ࠤࠧࡧࡲࡨࡷࡰࡩࡳࡺࡳࠣ࠼ࠣࡿࠧࡹࡴࡢࡶࡸࡷࠧࡀࠢࡧࡣ࡬ࡰࡪࡪࠢ࠭ࠢࠥࡶࡪࡧࡳࡰࡰࠥ࠾ࠥ࠭౩") + json.dumps(bstack1ll1_opy_ (u"ࠢࡔࡥࡨࡲࡦࡸࡩࡰࠢࡩࡥ࡮ࡲࡥࡥࠢࡺ࡭ࡹ࡮࠺ࠡ࡞ࡱࠦ౪") + str(bstack11lll1l_opy_)) + bstack1ll1_opy_ (u"ࠨࡿࢀࠫ౫"))
+          context.browser.execute_script(bstack11_opy_ (u"ࠬࡨࡲࡰࡹࡶࡩࡷࡹࡴࡢࡥ࡮ࡣࡪࡾࡥࡤࡷࡷࡳࡷࡀࠠࡼࠤࡤࡧࡹ࡯࡯࡯ࠤ࠽ࠤࠧࡹࡥࡵࡕࡨࡷࡸ࡯࡯࡯ࡕࡷࡥࡹࡻࡳࠣ࠮ࠣࠦࡦࡸࡧࡶ࡯ࡨࡲࡹࡹࠢ࠻ࠢࡾࠦࡸࡺࡡࡵࡷࡶࠦ࠿ࠨࡦࡢ࡫࡯ࡩࡩࠨࠬࠡࠤࡵࡩࡦࡹ࡯࡯ࠤ࠽ࠤࠬಒ") + json.dumps(bstack11_opy_ (u"ࠨࡓࡤࡧࡱࡥࡷ࡯࡯ࠡࡨࡤ࡭ࡱ࡫ࡤࠡࡹ࡬ࡸ࡭ࡀࠠ࡝ࡰࠥಓ") + str(bstack11ll1l1_opy_)) + bstack11_opy_ (u"ࠧࡾࡿࠪಔ"))
       else:
-        bstack1ll1l1l_opy_(context, bstack1ll1_opy_ (u"ࠤࡓࡥࡸࡹࡥࡥࠣࠥ౬"), bstack1ll1_opy_ (u"ࠥ࡭ࡳ࡬࡯ࠣ౭"))
+        bstack11l1111_opy_(context, bstack11_opy_ (u"ࠣࡒࡤࡷࡸ࡫ࡤࠢࠤಕ"), bstack11_opy_ (u"ࠤ࡬ࡲ࡫ࡵࠢಖ"))
         if self.driver_before_scenario:
-          bstack11ll1ll1_opy_(context, bstack1ll1_opy_ (u"ࠦࡵࡧࡳࡴࡧࡧࠦ౮"))
-        context.browser.execute_script(bstack1ll1_opy_ (u"ࠬࡨࡲࡰࡹࡶࡩࡷࡹࡴࡢࡥ࡮ࡣࡪࡾࡥࡤࡷࡷࡳࡷࡀࠠࡼࠤࡤࡧࡹ࡯࡯࡯ࠤ࠽ࠤࠧࡧ࡮࡯ࡱࡷࡥࡹ࡫ࠢ࠭ࠢࠥࡥࡷ࡭ࡵ࡮ࡧࡱࡸࡸࠨ࠺ࠡࡽࠥࡨࡦࡺࡡࠣ࠼ࠪ౯") + json.dumps(str(args[0].name) + bstack1ll1_opy_ (u"ࠨࠠ࠮ࠢࡓࡥࡸࡹࡥࡥࠣࠥ౰")) + bstack1ll1_opy_ (u"ࠧ࠭ࠢࠥࡰࡪࡼࡥ࡭ࠤ࠽ࠤࠧ࡯࡮ࡧࡱࠥࢁࢂ࠭౱"))
+          bstack1llll111l_opy_(context, bstack11_opy_ (u"ࠥࡴࡦࡹࡳࡦࡦࠥಗ"))
+        context.browser.execute_script(bstack11_opy_ (u"ࠫࡧࡸ࡯ࡸࡵࡨࡶࡸࡺࡡࡤ࡭ࡢࡩࡽ࡫ࡣࡶࡶࡲࡶ࠿ࠦࡻࠣࡣࡦࡸ࡮ࡵ࡮ࠣ࠼ࠣࠦࡦࡴ࡮ࡰࡶࡤࡸࡪࠨࠬࠡࠤࡤࡶ࡬ࡻ࡭ࡦࡰࡷࡷࠧࡀࠠࡼࠤࡧࡥࡹࡧࠢ࠻ࠩಘ") + json.dumps(str(args[0].name) + bstack11_opy_ (u"ࠧࠦ࠭ࠡࡒࡤࡷࡸ࡫ࡤࠢࠤಙ")) + bstack11_opy_ (u"࠭ࠬࠡࠤ࡯ࡩࡻ࡫࡬ࠣ࠼ࠣࠦ࡮ࡴࡦࡰࠤࢀࢁࠬಚ"))
         if self.driver_before_scenario:
-          context.browser.execute_script(bstack1ll1_opy_ (u"ࠨࡤࡵࡳࡼࡹࡥࡳࡵࡷࡥࡨࡱ࡟ࡦࡺࡨࡧࡺࡺ࡯ࡳ࠼ࠣࡿࠧࡧࡣࡵ࡫ࡲࡲࠧࡀࠠࠣࡵࡨࡸࡘ࡫ࡳࡴ࡫ࡲࡲࡘࡺࡡࡵࡷࡶࠦ࠱ࠦࠢࡢࡴࡪࡹࡲ࡫࡮ࡵࡵࠥ࠾ࠥࢁࠢࡴࡶࡤࡸࡺࡹࠢ࠻ࠤࡳࡥࡸࡹࡥࡥࠤࢀࢁࠬ౲"))
+          context.browser.execute_script(bstack11_opy_ (u"ࠧࡣࡴࡲࡻࡸ࡫ࡲࡴࡶࡤࡧࡰࡥࡥࡹࡧࡦࡹࡹࡵࡲ࠻ࠢࡾࠦࡦࡩࡴࡪࡱࡱࠦ࠿ࠦࠢࡴࡧࡷࡗࡪࡹࡳࡪࡱࡱࡗࡹࡧࡴࡶࡵࠥ࠰ࠥࠨࡡࡳࡩࡸࡱࡪࡴࡴࡴࠤ࠽ࠤࢀࠨࡳࡵࡣࡷࡹࡸࠨ࠺ࠣࡲࡤࡷࡸ࡫ࡤࠣࡿࢀࠫಛ"))
     except Exception as e:
-      logger.debug(bstack1ll1_opy_ (u"ࠩࡉࡥ࡮ࡲࡥࡥࠢࡷࡳࠥࡳࡡࡳ࡭ࠣࡷࡪࡹࡳࡪࡱࡱࠤࡸࡺࡡࡵࡷࡶࠤ࡮ࡴࠠࡢࡨࡷࡩࡷࠦࡦࡦࡣࡷࡹࡷ࡫࠺ࠡࡽࢀࠫ౳").format(str(e)))
-  if name == bstack1ll1_opy_ (u"ࠪࡥ࡫ࡺࡥࡳࡡࡩࡩࡦࡺࡵࡳࡧࠪ౴"):
+      logger.debug(bstack11_opy_ (u"ࠨࡈࡤ࡭ࡱ࡫ࡤࠡࡶࡲࠤࡲࡧࡲ࡬ࠢࡶࡩࡸࡹࡩࡰࡰࠣࡷࡹࡧࡴࡶࡵࠣ࡭ࡳࠦࡡࡧࡶࡨࡶࠥ࡬ࡥࡢࡶࡸࡶࡪࡀࠠࡼࡿࠪಜ").format(str(e)))
+  if name == bstack11_opy_ (u"ࠩࡤࡪࡹ࡫ࡲࡠࡨࡨࡥࡹࡻࡲࡦࠩಝ"):
     try:
       if context.failed is True:
-        bstack11l1l1_opy_ = []
-        bstack1ll11lll1_opy_ = []
-        bstack111111_opy_ = []
-        bstack111ll1l_opy_ = bstack1ll1_opy_ (u"ࠫࠬ౵")
+        bstack11llllll_opy_ = []
+        bstack1111l1ll_opy_ = []
+        bstack1llllllll_opy_ = []
+        bstack1ll1llll_opy_ = bstack11_opy_ (u"ࠪࠫಞ")
         try:
           import traceback
           for exc in self.exception_arr:
-            bstack11l1l1_opy_.append(exc.__class__.__name__)
+            bstack11llllll_opy_.append(exc.__class__.__name__)
           for exc_tb in self.exc_traceback_arr:
-            bstack1lll1l1l1_opy_ = traceback.format_tb(exc_tb)
-            bstack1llll111_opy_ = bstack1ll1_opy_ (u"ࠬࠦࠧ౶").join(bstack1lll1l1l1_opy_)
-            bstack1ll11lll1_opy_.append(bstack1llll111_opy_)
-            bstack111111_opy_.append(bstack1lll1l1l1_opy_[-1])
+            bstack11llll_opy_ = traceback.format_tb(exc_tb)
+            bstack1l11l1lll_opy_ = bstack11_opy_ (u"ࠫࠥ࠭ಟ").join(bstack11llll_opy_)
+            bstack1111l1ll_opy_.append(bstack1l11l1lll_opy_)
+            bstack1llllllll_opy_.append(bstack11llll_opy_[-1])
         except Exception as e:
-          logger.debug(bstack1l1l1ll1l_opy_.format(str(e)))
-        bstack11lll1l_opy_ = bstack1ll1_opy_ (u"࠭ࠧ౷")
-        for i in range(len(bstack11l1l1_opy_)):
-          bstack11lll1l_opy_ += bstack11l1l1_opy_[i] + bstack111111_opy_[i] + bstack1ll1_opy_ (u"ࠧ࡝ࡰࠪ౸")
-        bstack111ll1l_opy_ = bstack1ll1_opy_ (u"ࠨࠢࠪ౹").join(bstack1ll11lll1_opy_)
+          logger.debug(bstack1l1l1ll_opy_.format(str(e)))
+        bstack11ll1l1_opy_ = bstack11_opy_ (u"ࠬ࠭ಠ")
+        for i in range(len(bstack11llllll_opy_)):
+          bstack11ll1l1_opy_ += bstack11llllll_opy_[i] + bstack1llllllll_opy_[i] + bstack11_opy_ (u"࠭࡜࡯ࠩಡ")
+        bstack1ll1llll_opy_ = bstack11_opy_ (u"ࠧࠡࠩಢ").join(bstack1111l1ll_opy_)
         if not self.driver_before_scenario:
-          bstack1ll1l1l_opy_(context, bstack111ll1l_opy_, bstack1ll1_opy_ (u"ࠤࡨࡶࡷࡵࡲࠣ౺"))
-          bstack11ll1ll1_opy_(context, bstack1ll1_opy_ (u"ࠥࡪࡦ࡯࡬ࡦࡦࠥ౻"), bstack11lll1l_opy_)
-          context.browser.execute_script(bstack1ll1_opy_ (u"ࠫࡧࡸ࡯ࡸࡵࡨࡶࡸࡺࡡࡤ࡭ࡢࡩࡽ࡫ࡣࡶࡶࡲࡶ࠿ࠦࡻࠣࡣࡦࡸ࡮ࡵ࡮ࠣ࠼ࠣࠦࡦࡴ࡮ࡰࡶࡤࡸࡪࠨࠬࠡࠤࡤࡶ࡬ࡻ࡭ࡦࡰࡷࡷࠧࡀࠠࡼࠤࡧࡥࡹࡧࠢ࠻ࠩ౼") + json.dumps(bstack111ll1l_opy_) + bstack1ll1_opy_ (u"ࠬ࠲ࠠࠣ࡮ࡨࡺࡪࡲࠢ࠻ࠢࠥࡩࡷࡸ࡯ࡳࠤࢀࢁࠬ౽"))
-          context.browser.execute_script(bstack1ll1_opy_ (u"࠭ࡢࡳࡱࡺࡷࡪࡸࡳࡵࡣࡦ࡯ࡤ࡫ࡸࡦࡥࡸࡸࡴࡸ࠺ࠡࡽࠥࡥࡨࡺࡩࡰࡰࠥ࠾ࠥࠨࡳࡦࡶࡖࡩࡸࡹࡩࡰࡰࡖࡸࡦࡺࡵࡴࠤ࠯ࠤࠧࡧࡲࡨࡷࡰࡩࡳࡺࡳࠣ࠼ࠣࡿࠧࡹࡴࡢࡶࡸࡷࠧࡀࠢࡧࡣ࡬ࡰࡪࡪࠢ࠭ࠢࠥࡶࡪࡧࡳࡰࡰࠥ࠾ࠥ࠭౾") + json.dumps(bstack1ll1_opy_ (u"ࠢࡔࡱࡰࡩࠥࡹࡣࡦࡰࡤࡶ࡮ࡵࡳࠡࡨࡤ࡭ࡱ࡫ࡤ࠻ࠢ࡟ࡲࠧ౿") + str(bstack11lll1l_opy_)) + bstack1ll1_opy_ (u"ࠨࡿࢀࠫಀ"))
+          bstack11l1111_opy_(context, bstack1ll1llll_opy_, bstack11_opy_ (u"ࠣࡧࡵࡶࡴࡸࠢಣ"))
+          bstack1llll111l_opy_(context, bstack11_opy_ (u"ࠤࡩࡥ࡮ࡲࡥࡥࠤತ"), bstack11ll1l1_opy_)
+          context.browser.execute_script(bstack11_opy_ (u"ࠪࡦࡷࡵࡷࡴࡧࡵࡷࡹࡧࡣ࡬ࡡࡨࡼࡪࡩࡵࡵࡱࡵ࠾ࠥࢁࠢࡢࡥࡷ࡭ࡴࡴࠢ࠻ࠢࠥࡥࡳࡴ࡯ࡵࡣࡷࡩࠧ࠲ࠠࠣࡣࡵ࡫ࡺࡳࡥ࡯ࡶࡶࠦ࠿ࠦࡻࠣࡦࡤࡸࡦࠨ࠺ࠨಥ") + json.dumps(bstack1ll1llll_opy_) + bstack11_opy_ (u"ࠫ࠱ࠦࠢ࡭ࡧࡹࡩࡱࠨ࠺ࠡࠤࡨࡶࡷࡵࡲࠣࡿࢀࠫದ"))
+          context.browser.execute_script(bstack11_opy_ (u"ࠬࡨࡲࡰࡹࡶࡩࡷࡹࡴࡢࡥ࡮ࡣࡪࡾࡥࡤࡷࡷࡳࡷࡀࠠࡼࠤࡤࡧࡹ࡯࡯࡯ࠤ࠽ࠤࠧࡹࡥࡵࡕࡨࡷࡸ࡯࡯࡯ࡕࡷࡥࡹࡻࡳࠣ࠮ࠣࠦࡦࡸࡧࡶ࡯ࡨࡲࡹࡹࠢ࠻ࠢࡾࠦࡸࡺࡡࡵࡷࡶࠦ࠿ࠨࡦࡢ࡫࡯ࡩࡩࠨࠬࠡࠤࡵࡩࡦࡹ࡯࡯ࠤ࠽ࠤࠬಧ") + json.dumps(bstack11_opy_ (u"ࠨࡓࡰ࡯ࡨࠤࡸࡩࡥ࡯ࡣࡵ࡭ࡴࡹࠠࡧࡣ࡬ࡰࡪࡪ࠺ࠡ࡞ࡱࠦನ") + str(bstack11ll1l1_opy_)) + bstack11_opy_ (u"ࠧࡾࡿࠪ಩"))
       else:
         if not self.driver_before_scenario:
-          bstack1ll1l1l_opy_(context, bstack1ll1_opy_ (u"ࠤࡉࡩࡦࡺࡵࡳࡧ࠽ࠤࠧಁ") + str(self.feature.name) + bstack1ll1_opy_ (u"ࠥࠤࡵࡧࡳࡴࡧࡧࠥࠧಂ"), bstack1ll1_opy_ (u"ࠦ࡮ࡴࡦࡰࠤಃ"))
-          bstack11ll1ll1_opy_(context, bstack1ll1_opy_ (u"ࠧࡶࡡࡴࡵࡨࡨࠧ಄"))
-          context.browser.execute_script(bstack1ll1_opy_ (u"࠭ࡢࡳࡱࡺࡷࡪࡸࡳࡵࡣࡦ࡯ࡤ࡫ࡸࡦࡥࡸࡸࡴࡸ࠺ࠡࡽࠥࡥࡨࡺࡩࡰࡰࠥ࠾ࠥࠨࡡ࡯ࡰࡲࡸࡦࡺࡥࠣ࠮ࠣࠦࡦࡸࡧࡶ࡯ࡨࡲࡹࡹࠢ࠻ࠢࡾࠦࡩࡧࡴࡢࠤ࠽ࠫಅ") + json.dumps(bstack1ll1_opy_ (u"ࠢࡇࡧࡤࡸࡺࡸࡥ࠻ࠢࠥಆ") + str(self.feature.name) + bstack1ll1_opy_ (u"ࠣࠢࡳࡥࡸࡹࡥࡥࠣࠥಇ")) + bstack1ll1_opy_ (u"ࠩ࠯ࠤࠧࡲࡥࡷࡧ࡯ࠦ࠿ࠦࠢࡪࡰࡩࡳࠧࢃࡽࠨಈ"))
-          context.browser.execute_script(bstack1ll1_opy_ (u"ࠪࡦࡷࡵࡷࡴࡧࡵࡷࡹࡧࡣ࡬ࡡࡨࡼࡪࡩࡵࡵࡱࡵ࠾ࠥࢁࠢࡢࡥࡷ࡭ࡴࡴࠢ࠻ࠢࠥࡷࡪࡺࡓࡦࡵࡶ࡭ࡴࡴࡓࡵࡣࡷࡹࡸࠨࠬࠡࠤࡤࡶ࡬ࡻ࡭ࡦࡰࡷࡷࠧࡀࠠࡼࠤࡶࡸࡦࡺࡵࡴࠤ࠽ࠦࡵࡧࡳࡴࡧࡧࠦࢂࢃࠧಉ"))
-    except Exception as e:
-      logger.debug(bstack1ll1_opy_ (u"ࠫࡋࡧࡩ࡭ࡧࡧࠤࡹࡵࠠ࡮ࡣࡵ࡯ࠥࡹࡥࡴࡵ࡬ࡳࡳࠦࡳࡵࡣࡷࡹࡸࠦࡩ࡯ࠢࡤࡪࡹ࡫ࡲࠡࡨࡨࡥࡹࡻࡲࡦ࠼ࠣࡿࢂ࠭ಊ").format(str(e)))
-  if name in [bstack1ll1_opy_ (u"ࠬࡧࡦࡵࡧࡵࡣ࡫࡫ࡡࡵࡷࡵࡩࠬಋ"), bstack1ll1_opy_ (u"࠭ࡡࡧࡶࡨࡶࡤࡹࡣࡦࡰࡤࡶ࡮ࡵࠧಌ")]:
-    bstack1l1ll11ll_opy_(self, name, context, *args)
-    if (name == bstack1ll1_opy_ (u"ࠧࡢࡨࡷࡩࡷࡥࡳࡤࡧࡱࡥࡷ࡯࡯ࠨ಍") and self.driver_before_scenario) or (name == bstack1ll1_opy_ (u"ࠨࡣࡩࡸࡪࡸ࡟ࡧࡧࡤࡸࡺࡸࡥࠨಎ") and not self.driver_before_scenario):
+          bstack11l1111_opy_(context, bstack11_opy_ (u"ࠣࡈࡨࡥࡹࡻࡲࡦ࠼ࠣࠦಪ") + str(self.feature.name) + bstack11_opy_ (u"ࠤࠣࡴࡦࡹࡳࡦࡦࠤࠦಫ"), bstack11_opy_ (u"ࠥ࡭ࡳ࡬࡯ࠣಬ"))
+          bstack1llll111l_opy_(context, bstack11_opy_ (u"ࠦࡵࡧࡳࡴࡧࡧࠦಭ"))
+          context.browser.execute_script(bstack11_opy_ (u"ࠬࡨࡲࡰࡹࡶࡩࡷࡹࡴࡢࡥ࡮ࡣࡪࡾࡥࡤࡷࡷࡳࡷࡀࠠࡼࠤࡤࡧࡹ࡯࡯࡯ࠤ࠽ࠤࠧࡧ࡮࡯ࡱࡷࡥࡹ࡫ࠢ࠭ࠢࠥࡥࡷ࡭ࡵ࡮ࡧࡱࡸࡸࠨ࠺ࠡࡽࠥࡨࡦࡺࡡࠣ࠼ࠪಮ") + json.dumps(bstack11_opy_ (u"ࠨࡆࡦࡣࡷࡹࡷ࡫࠺ࠡࠤಯ") + str(self.feature.name) + bstack11_opy_ (u"ࠢࠡࡲࡤࡷࡸ࡫ࡤࠢࠤರ")) + bstack11_opy_ (u"ࠨ࠮ࠣࠦࡱ࡫ࡶࡦ࡮ࠥ࠾ࠥࠨࡩ࡯ࡨࡲࠦࢂࢃࠧಱ"))
+          context.browser.execute_script(bstack11_opy_ (u"ࠩࡥࡶࡴࡽࡳࡦࡴࡶࡸࡦࡩ࡫ࡠࡧࡻࡩࡨࡻࡴࡰࡴ࠽ࠤࢀࠨࡡࡤࡶ࡬ࡳࡳࠨ࠺ࠡࠤࡶࡩࡹ࡙ࡥࡴࡵ࡬ࡳࡳ࡙ࡴࡢࡶࡸࡷࠧ࠲ࠠࠣࡣࡵ࡫ࡺࡳࡥ࡯ࡶࡶࠦ࠿ࠦࡻࠣࡵࡷࡥࡹࡻࡳࠣ࠼ࠥࡴࡦࡹࡳࡦࡦࠥࢁࢂ࠭ಲ"))
+    except Exception as e:
+      logger.debug(bstack11_opy_ (u"ࠪࡊࡦ࡯࡬ࡦࡦࠣࡸࡴࠦ࡭ࡢࡴ࡮ࠤࡸ࡫ࡳࡴ࡫ࡲࡲࠥࡹࡴࡢࡶࡸࡷࠥ࡯࡮ࠡࡣࡩࡸࡪࡸࠠࡧࡧࡤࡸࡺࡸࡥ࠻ࠢࡾࢁࠬಳ").format(str(e)))
+  if name in [bstack11_opy_ (u"ࠫࡦ࡬ࡴࡦࡴࡢࡪࡪࡧࡴࡶࡴࡨࠫ಴"), bstack11_opy_ (u"ࠬࡧࡦࡵࡧࡵࡣࡸࡩࡥ࡯ࡣࡵ࡭ࡴ࠭ವ")]:
+    bstack11l11ll1_opy_(self, name, context, *args)
+    if (name == bstack11_opy_ (u"࠭ࡡࡧࡶࡨࡶࡤࡹࡣࡦࡰࡤࡶ࡮ࡵࠧಶ") and self.driver_before_scenario) or (name == bstack11_opy_ (u"ࠧࡢࡨࡷࡩࡷࡥࡦࡦࡣࡷࡹࡷ࡫ࠧಷ") and not self.driver_before_scenario):
       try:
         context.browser.quit()
       except Exception:
         pass
-def bstack1lllllll1_opy_(config, startdir):
-  return bstack1ll1_opy_ (u"ࠤࡧࡶ࡮ࡼࡥࡳ࠼ࠣࡿ࠵ࢃࠢಏ").format(bstack1ll1_opy_ (u"ࠥࡆࡷࡵࡷࡴࡧࡵࡗࡹࡧࡣ࡬ࠤಐ"))
+def bstack1lllll1l1_opy_(config, startdir):
+  return bstack11_opy_ (u"ࠣࡦࡵ࡭ࡻ࡫ࡲ࠻ࠢࡾ࠴ࢂࠨಸ").format(bstack11_opy_ (u"ࠤࡅࡶࡴࡽࡳࡦࡴࡖࡸࡦࡩ࡫ࠣಹ"))
 class Notset:
   def __repr__(self):
-    return bstack1ll1_opy_ (u"ࠦࡁࡔࡏࡕࡕࡈࡘࡃࠨ಑")
+    return bstack11_opy_ (u"ࠥࡀࡓࡕࡔࡔࡇࡗࡂࠧ಺")
 notset = Notset()
-def bstack1ll1ll11_opy_(self, name: str, default=notset, skip: bool = False):
-  global bstack11ll1l1l_opy_
-  if str(name).lower() == bstack1ll1_opy_ (u"ࠬࡪࡲࡪࡸࡨࡶࠬಒ"):
-    return bstack1ll1_opy_ (u"ࠨࡂࡳࡱࡺࡷࡪࡸࡓࡵࡣࡦ࡯ࠧಓ")
+def bstack111l11l1_opy_(self, name: str, default=notset, skip: bool = False):
+  global bstack1l11lll11_opy_
+  if str(name).lower() == bstack11_opy_ (u"ࠫࡩࡸࡩࡷࡧࡵࠫ಻"):
+    return bstack11_opy_ (u"ࠧࡈࡲࡰࡹࡶࡩࡷ࡙ࡴࡢࡥ࡮಼ࠦ")
   else:
-    return bstack11ll1l1l_opy_(self, name, default, skip)
-def bstack111l111l_opy_(bstack11l1l11_opy_):
-  global bstack1l1l1l11_opy_
-  bstack1l1l1l11_opy_ = bstack11l1l11_opy_
-  logger.info(bstack1l1l1l1ll_opy_.format(bstack1l1l1l11_opy_.split(bstack1ll1_opy_ (u"ࠧ࠮ࠩಔ"))[0]))
+    return bstack1l11lll11_opy_(self, name, default, skip)
+def bstack1l111ll1_opy_(bstack1ll1l111_opy_):
+  global bstack1l1lll1l_opy_
+  bstack1l1lll1l_opy_ = bstack1ll1l111_opy_
+  logger.info(bstack1111ll_opy_.format(bstack1l1lll1l_opy_.split(bstack11_opy_ (u"࠭࠭ࠨಽ"))[0]))
   try:
     from selenium import webdriver
     from selenium.webdriver.common.service import Service
     from selenium.webdriver.remote.webdriver import WebDriver
   except Exception as e:
-    logger.warn(bstack11l11_opy_ + str(e))
-  Service.start = bstack1lll11111_opy_
-  Service.stop = bstack1llll1l11_opy_
-  webdriver.Remote.__init__ = bstack1llll1111_opy_
-  webdriver.Remote.get = bstack11llll1l_opy_
-  WebDriver.close = bstack111l11ll_opy_
-  bstack1ll1ll1l_opy_()
-  if bstack1ll1l1ll_opy_():
+    logger.warn(bstack11l1l1l1_opy_ + str(e))
+  Service.start = bstack11ll1l1l_opy_
+  Service.stop = bstack11l1lll1_opy_
+  webdriver.Remote.__init__ = bstack1l1l1111l_opy_
+  webdriver.Remote.get = bstack1l1l1l1_opy_
+  WebDriver.close = bstack11l11l1_opy_
+  bstack11l111l_opy_()
+  if bstack1111l1l_opy_():
     try:
       from selenium.webdriver.remote.remote_connection import RemoteConnection
-      RemoteConnection._get_proxy_url = bstack111l1ll1_opy_
+      RemoteConnection._get_proxy_url = bstack1l1l111l1_opy_
     except Exception as e:
-      logger.error(bstack1l11ll1ll_opy_.format(str(e)))
-  if (bstack1ll1_opy_ (u"ࠨࡴࡲࡦࡴࡺࠧಕ") in str(bstack11l1l11_opy_).lower()):
+      logger.error(bstack11ll11_opy_.format(str(e)))
+  if (bstack11_opy_ (u"ࠧࡳࡱࡥࡳࡹ࠭ಾ") in str(bstack1ll1l111_opy_).lower()):
     try:
       from robot import run_cli
       from robot.output import Output
       from robot.running.status import TestStatus
       from pabot.pabot import QueueItem
       from pabot import pabot
       try:
         from SeleniumLibrary.keywords.webdrivertools.webdrivertools import WebDriverCreator
-        WebDriverCreator._get_ff_profile = bstack1l111l1l_opy_
+        WebDriverCreator._get_ff_profile = bstack1l11l1_opy_
       except Exception as e:
-        logger.warn(bstack1llll1ll1_opy_ + str(e))
+        logger.warn(bstack11l111ll_opy_ + str(e))
     except Exception as e:
-      bstack11l1_opy_(e, bstack1llll1ll1_opy_)
-    Output.end_test = bstack11llll1_opy_
-    TestStatus.__init__ = bstack1llll1lll_opy_
-    QueueItem.__init__ = bstack1l1111_opy_
-    pabot._create_items = bstack1ll11ll1l_opy_
-    try:
-      from pabot import __version__ as bstack11l11111_opy_
-      if version.parse(bstack11l11111_opy_) >= version.parse(bstack1ll1_opy_ (u"ࠩ࠵࠲࠶࠻࠮࠱ࠩಖ")):
-        pabot._run = bstack1ll1ll11l_opy_
-      elif version.parse(bstack11l11111_opy_) >= version.parse(bstack1ll1_opy_ (u"ࠪ࠶࠳࠷࠳࠯࠲ࠪಗ")):
-        pabot._run = bstack1l1111ll_opy_
+      bstack111lll1l_opy_(e, bstack11l111ll_opy_)
+    Output.end_test = bstack11l111l1_opy_
+    TestStatus.__init__ = bstack1l1ll1l11_opy_
+    QueueItem.__init__ = bstack1ll1l11l1_opy_
+    pabot._create_items = bstack11l1_opy_
+    try:
+      from pabot import __version__ as bstack1l11l1ll_opy_
+      if version.parse(bstack1l11l1ll_opy_) >= version.parse(bstack11_opy_ (u"ࠨ࠴࠱࠵࠺࠴࠰ࠨಿ")):
+        pabot._run = bstack1l11_opy_
+      elif version.parse(bstack1l11l1ll_opy_) >= version.parse(bstack11_opy_ (u"ࠩ࠵࠲࠶࠹࠮࠱ࠩೀ")):
+        pabot._run = bstack1l11llll1_opy_
       else:
-        pabot._run = bstack1lll1l1ll_opy_
+        pabot._run = bstack1l1l11lll_opy_
     except Exception as e:
-      pabot._run = bstack1lll1l1ll_opy_
-    pabot._create_command_for_execution = bstack1ll1ll1l1_opy_
-    pabot._report_results = bstack11111ll1_opy_
-  if bstack1ll1_opy_ (u"ࠫࡧ࡫ࡨࡢࡸࡨࠫಘ") in str(bstack11l1l11_opy_).lower():
+      pabot._run = bstack1l1l11lll_opy_
+    pabot._create_command_for_execution = bstack1ll11_opy_
+    pabot._report_results = bstack1l11ll1l1_opy_
+  if bstack11_opy_ (u"ࠪࡦࡪ࡮ࡡࡷࡧࠪು") in str(bstack1ll1l111_opy_).lower():
     try:
       from behave.runner import Runner
       from behave.model import Step
     except Exception as e:
-      bstack11l1_opy_(e, bstack1l111ll_opy_)
-    Runner.run_hook = bstack1l1l111l1_opy_
-    Step.run = bstack1ll11l111_opy_
-  if bstack1ll1_opy_ (u"ࠬࡶࡹࡵࡧࡶࡸࠬಙ") in str(bstack11l1l11_opy_).lower():
+      bstack111lll1l_opy_(e, bstack111111ll_opy_)
+    Runner.run_hook = bstack1ll1l1111_opy_
+    Step.run = bstack1111lll_opy_
+  if bstack11_opy_ (u"ࠫࡵࡿࡴࡦࡵࡷࠫೂ") in str(bstack1ll1l111_opy_).lower():
     try:
       from pytest_selenium import pytest_selenium
       from _pytest.config import Config
     except Exception as e:
-      bstack11l1_opy_(e, bstack1lll11ll1_opy_)
-    pytest_selenium.pytest_report_header = bstack1lllllll1_opy_
-    Config.getoption = bstack1ll1ll11_opy_
-def bstack1lll1l11l_opy_():
-  global CONFIG
-  if bstack1ll1_opy_ (u"࠭ࡰࡢࡴࡤࡰࡱ࡫࡬ࡴࡒࡨࡶࡕࡲࡡࡵࡨࡲࡶࡲ࠭ಚ") in CONFIG and int(CONFIG[bstack1ll1_opy_ (u"ࠧࡱࡣࡵࡥࡱࡲࡥ࡭ࡵࡓࡩࡷࡖ࡬ࡢࡶࡩࡳࡷࡳࠧಛ")]) > 1:
-    logger.warn(bstack11ll1l_opy_)
-def bstack1l1ll11l1_opy_(bstack1l1l11l_opy_, index):
-  bstack111l111l_opy_(bstack1lllll111_opy_)
-  exec(open(bstack1l1l11l_opy_).read())
-def bstack1l11l1ll_opy_(arg):
-  global CONFIG
-  bstack111l111l_opy_(bstack1l11l1ll1_opy_)
-  os.environ[bstack1ll1_opy_ (u"ࠨࡄࡕࡓ࡜࡙ࡅࡓࡕࡗࡅࡈࡑ࡟ࡖࡕࡈࡖࡓࡇࡍࡆࠩಜ")] = CONFIG[bstack1ll1_opy_ (u"ࠩࡸࡷࡪࡸࡎࡢ࡯ࡨࠫಝ")]
-  os.environ[bstack1ll1_opy_ (u"ࠪࡆࡗࡕࡗࡔࡇࡕࡗ࡙ࡇࡃࡌࡡࡄࡇࡈࡋࡓࡔࡡࡎࡉ࡞࠭ಞ")] = CONFIG[bstack1ll1_opy_ (u"ࠫࡦࡩࡣࡦࡵࡶࡏࡪࡿࠧಟ")]
-  from _pytest.config import main as bstack1lll11ll_opy_
-  bstack1lll11ll_opy_(arg)
-def bstack1l1111l_opy_(arg):
-  bstack111l111l_opy_(bstack1lllll11_opy_)
-  from behave.__main__ import main as bstack1111lll_opy_
-  bstack1111lll_opy_(arg)
-def bstack11ll111_opy_():
-  logger.info(bstack1111llll_opy_)
+      bstack111lll1l_opy_(e, bstack111lll_opy_)
+    pytest_selenium.pytest_report_header = bstack1lllll1l1_opy_
+    Config.getoption = bstack111l11l1_opy_
+def bstack1ll111ll1_opy_():
+  global CONFIG
+  if bstack11_opy_ (u"ࠬࡶࡡࡳࡣ࡯ࡰࡪࡲࡳࡑࡧࡵࡔࡱࡧࡴࡧࡱࡵࡱࠬೃ") in CONFIG and int(CONFIG[bstack11_opy_ (u"࠭ࡰࡢࡴࡤࡰࡱ࡫࡬ࡴࡒࡨࡶࡕࡲࡡࡵࡨࡲࡶࡲ࠭ೄ")]) > 1:
+    logger.warn(bstack1l111l1l_opy_)
+def bstack1l11l11l1_opy_(bstack1llllll1l_opy_, index):
+  bstack1l111ll1_opy_(bstack111l1_opy_)
+  exec(open(bstack1llllll1l_opy_).read())
+def bstack1111_opy_(arg):
+  global CONFIG
+  bstack1l111ll1_opy_(bstack1l1l11l_opy_)
+  os.environ[bstack11_opy_ (u"ࠧࡃࡔࡒ࡛ࡘࡋࡒࡔࡖࡄࡇࡐࡥࡕࡔࡇࡕࡒࡆࡓࡅࠨ೅")] = CONFIG[bstack11_opy_ (u"ࠨࡷࡶࡩࡷࡔࡡ࡮ࡧࠪೆ")]
+  os.environ[bstack11_opy_ (u"ࠩࡅࡖࡔ࡝ࡓࡆࡔࡖࡘࡆࡉࡋࡠࡃࡆࡇࡊ࡙ࡓࡠࡍࡈ࡝ࠬೇ")] = CONFIG[bstack11_opy_ (u"ࠪࡥࡨࡩࡥࡴࡵࡎࡩࡾ࠭ೈ")]
+  from _pytest.config import main as bstack1lllll1_opy_
+  bstack1lllll1_opy_(arg)
+def bstack1ll11ll_opy_(arg):
+  bstack1l111ll1_opy_(bstack1llll11_opy_)
+  from behave.__main__ import main as bstack1l1l1ll1_opy_
+  bstack1l1l1ll1_opy_(arg)
+def bstack1111l11_opy_():
+  logger.info(bstack1lll111ll_opy_)
   import argparse
   parser = argparse.ArgumentParser()
-  parser.add_argument(bstack1ll1_opy_ (u"ࠬࡹࡥࡵࡷࡳࠫಠ"), help=bstack1ll1_opy_ (u"࠭ࡇࡦࡰࡨࡶࡦࡺࡥࠡࡤࡵࡳࡼࡹࡥࡳࡵࡷࡥࡨࡱࠠࡤࡱࡱࡪ࡮࡭ࠧಡ"))
-  parser.add_argument(bstack1ll1_opy_ (u"ࠧ࠮ࡷࠪಢ"), bstack1ll1_opy_ (u"ࠨ࠯࠰ࡹࡸ࡫ࡲ࡯ࡣࡰࡩࠬಣ"), help=bstack1ll1_opy_ (u"ࠩ࡜ࡳࡺࡸࠠࡣࡴࡲࡻࡸ࡫ࡲࡴࡶࡤࡧࡰࠦࡵࡴࡧࡵࡲࡦࡳࡥࠨತ"))
-  parser.add_argument(bstack1ll1_opy_ (u"ࠪ࠱ࡰ࠭ಥ"), bstack1ll1_opy_ (u"ࠫ࠲࠳࡫ࡦࡻࠪದ"), help=bstack1ll1_opy_ (u"ࠬ࡟࡯ࡶࡴࠣࡦࡷࡵࡷࡴࡧࡵࡷࡹࡧࡣ࡬ࠢࡤࡧࡨ࡫ࡳࡴࠢ࡮ࡩࡾ࠭ಧ"))
-  parser.add_argument(bstack1ll1_opy_ (u"࠭࠭ࡧࠩನ"), bstack1ll1_opy_ (u"ࠧ࠮࠯ࡩࡶࡦࡳࡥࡸࡱࡵ࡯ࠬ಩"), help=bstack1ll1_opy_ (u"ࠨ࡛ࡲࡹࡷࠦࡴࡦࡵࡷࠤ࡫ࡸࡡ࡮ࡧࡺࡳࡷࡱࠧಪ"))
-  bstack1l1ll11_opy_ = parser.parse_args()
-  try:
-    bstack1l11lll11_opy_ = bstack1ll1_opy_ (u"ࠩࡥࡶࡴࡽࡳࡦࡴࡶࡸࡦࡩ࡫࠯ࡩࡨࡲࡪࡸࡩࡤ࠰ࡼࡱࡱ࠴ࡳࡢ࡯ࡳࡰࡪ࠭ಫ")
-    if bstack1l1ll11_opy_.framework and bstack1l1ll11_opy_.framework not in (bstack1ll1_opy_ (u"ࠪࡴࡾࡺࡨࡰࡰࠪಬ"), bstack1ll1_opy_ (u"ࠫࡵࡿࡴࡩࡱࡱ࠷ࠬಭ")):
-      bstack1l11lll11_opy_ = bstack1ll1_opy_ (u"ࠬࡨࡲࡰࡹࡶࡩࡷࡹࡴࡢࡥ࡮࠲࡫ࡸࡡ࡮ࡧࡺࡳࡷࡱ࠮ࡺ࡯࡯࠲ࡸࡧ࡭ࡱ࡮ࡨࠫಮ")
-    bstack1l1l1l1l_opy_ = os.path.join(os.path.dirname(os.path.realpath(__file__)), bstack1l11lll11_opy_)
-    bstack1l11111l_opy_ = open(bstack1l1l1l1l_opy_, bstack1ll1_opy_ (u"࠭ࡲࠨಯ"))
-    bstack111lll1_opy_ = bstack1l11111l_opy_.read()
-    bstack1l11111l_opy_.close()
-    if bstack1l1ll11_opy_.username:
-      bstack111lll1_opy_ = bstack111lll1_opy_.replace(bstack1ll1_opy_ (u"࡚ࠧࡑࡘࡖࡤ࡛ࡓࡆࡔࡑࡅࡒࡋࠧರ"), bstack1l1ll11_opy_.username)
-    if bstack1l1ll11_opy_.key:
-      bstack111lll1_opy_ = bstack111lll1_opy_.replace(bstack1ll1_opy_ (u"ࠨ࡛ࡒ࡙ࡗࡥࡁࡄࡅࡈࡗࡘࡥࡋࡆ࡛ࠪಱ"), bstack1l1ll11_opy_.key)
-    if bstack1l1ll11_opy_.framework:
-      bstack111lll1_opy_ = bstack111lll1_opy_.replace(bstack1ll1_opy_ (u"ࠩ࡜ࡓ࡚ࡘ࡟ࡇࡔࡄࡑࡊ࡝ࡏࡓࡍࠪಲ"), bstack1l1ll11_opy_.framework)
-    file_name = bstack1ll1_opy_ (u"ࠪࡦࡷࡵࡷࡴࡧࡵࡷࡹࡧࡣ࡬࠰ࡼࡱࡱ࠭ಳ")
+  parser.add_argument(bstack11_opy_ (u"ࠫࡸ࡫ࡴࡶࡲࠪ೉"), help=bstack11_opy_ (u"ࠬࡍࡥ࡯ࡧࡵࡥࡹ࡫ࠠࡣࡴࡲࡻࡸ࡫ࡲࡴࡶࡤࡧࡰࠦࡣࡰࡰࡩ࡭࡬࠭ೊ"))
+  parser.add_argument(bstack11_opy_ (u"࠭࠭ࡶࠩೋ"), bstack11_opy_ (u"ࠧ࠮࠯ࡸࡷࡪࡸ࡮ࡢ࡯ࡨࠫೌ"), help=bstack11_opy_ (u"ࠨ࡛ࡲࡹࡷࠦࡢࡳࡱࡺࡷࡪࡸࡳࡵࡣࡦ࡯ࠥࡻࡳࡦࡴࡱࡥࡲ࡫್ࠧ"))
+  parser.add_argument(bstack11_opy_ (u"ࠩ࠰࡯ࠬ೎"), bstack11_opy_ (u"ࠪ࠱࠲ࡱࡥࡺࠩ೏"), help=bstack11_opy_ (u"ࠫ࡞ࡵࡵࡳࠢࡥࡶࡴࡽࡳࡦࡴࡶࡸࡦࡩ࡫ࠡࡣࡦࡧࡪࡹࡳࠡ࡭ࡨࡽࠬ೐"))
+  parser.add_argument(bstack11_opy_ (u"ࠬ࠳ࡦࠨ೑"), bstack11_opy_ (u"࠭࠭࠮ࡨࡵࡥࡲ࡫ࡷࡰࡴ࡮ࠫ೒"), help=bstack11_opy_ (u"࡚ࠧࡱࡸࡶࠥࡺࡥࡴࡶࠣࡪࡷࡧ࡭ࡦࡹࡲࡶࡰ࠭೓"))
+  bstack1l1l1l11_opy_ = parser.parse_args()
+  try:
+    bstack11ll11l1_opy_ = bstack11_opy_ (u"ࠨࡤࡵࡳࡼࡹࡥࡳࡵࡷࡥࡨࡱ࠮ࡨࡧࡱࡩࡷ࡯ࡣ࠯ࡻࡰࡰ࠳ࡹࡡ࡮ࡲ࡯ࡩࠬ೔")
+    if bstack1l1l1l11_opy_.framework and bstack1l1l1l11_opy_.framework not in (bstack11_opy_ (u"ࠩࡳࡽࡹ࡮࡯࡯ࠩೕ"), bstack11_opy_ (u"ࠪࡴࡾࡺࡨࡰࡰ࠶ࠫೖ")):
+      bstack11ll11l1_opy_ = bstack11_opy_ (u"ࠫࡧࡸ࡯ࡸࡵࡨࡶࡸࡺࡡࡤ࡭࠱ࡪࡷࡧ࡭ࡦࡹࡲࡶࡰ࠴ࡹ࡮࡮࠱ࡷࡦࡳࡰ࡭ࡧࠪ೗")
+    bstack11ll111_opy_ = os.path.join(os.path.dirname(os.path.realpath(__file__)), bstack11ll11l1_opy_)
+    bstack1ll1ll_opy_ = open(bstack11ll111_opy_, bstack11_opy_ (u"ࠬࡸࠧ೘"))
+    bstack1l1ll1l_opy_ = bstack1ll1ll_opy_.read()
+    bstack1ll1ll_opy_.close()
+    if bstack1l1l1l11_opy_.username:
+      bstack1l1ll1l_opy_ = bstack1l1ll1l_opy_.replace(bstack11_opy_ (u"࡙࠭ࡐࡗࡕࡣ࡚࡙ࡅࡓࡐࡄࡑࡊ࠭೙"), bstack1l1l1l11_opy_.username)
+    if bstack1l1l1l11_opy_.key:
+      bstack1l1ll1l_opy_ = bstack1l1ll1l_opy_.replace(bstack11_opy_ (u"࡚ࠧࡑࡘࡖࡤࡇࡃࡄࡇࡖࡗࡤࡑࡅ࡚ࠩ೚"), bstack1l1l1l11_opy_.key)
+    if bstack1l1l1l11_opy_.framework:
+      bstack1l1ll1l_opy_ = bstack1l1ll1l_opy_.replace(bstack11_opy_ (u"ࠨ࡛ࡒ࡙ࡗࡥࡆࡓࡃࡐࡉ࡜ࡕࡒࡌࠩ೛"), bstack1l1l1l11_opy_.framework)
+    file_name = bstack11_opy_ (u"ࠩࡥࡶࡴࡽࡳࡦࡴࡶࡸࡦࡩ࡫࠯ࡻࡰࡰࠬ೜")
     file_path = os.path.abspath(file_name)
-    bstack11111_opy_ = open(file_path, bstack1ll1_opy_ (u"ࠫࡼ࠭಴"))
-    bstack11111_opy_.write(bstack111lll1_opy_)
-    bstack11111_opy_.close()
-    logger.info(bstack11111ll_opy_)
-    try:
-      os.environ[bstack1ll1_opy_ (u"ࠬࡈࡒࡐ࡙ࡖࡉࡗ࡙ࡔࡂࡅࡎࡣࡋࡘࡁࡎࡇ࡚ࡓࡗࡑࠧವ")] = bstack1l1ll11_opy_.framework if bstack1l1ll11_opy_.framework != None else bstack1ll1_opy_ (u"ࠨࠢಶ")
-      config = yaml.safe_load(bstack111lll1_opy_)
-      config[bstack1ll1_opy_ (u"ࠧࡴࡱࡸࡶࡨ࡫ࠧಷ")] = bstack1ll1_opy_ (u"ࠨࡲࡼࡸ࡭ࡵ࡮࠮ࡵࡨࡸࡺࡶࠧಸ")
-      bstack1l11l1l_opy_(bstack1l11l1l1_opy_, config)
-    except Exception as e:
-      logger.debug(bstack11ll11l_opy_.format(str(e)))
-  except Exception as e:
-    logger.error(bstack1l111111_opy_.format(str(e)))
-def bstack1l11l1l_opy_(bstack111l1l11_opy_, config, bstack111l1ll_opy_ = {}):
-  global bstack111lllll_opy_
+    bstack1llll11l1_opy_ = open(file_path, bstack11_opy_ (u"ࠪࡻࠬೝ"))
+    bstack1llll11l1_opy_.write(bstack1l1ll1l_opy_)
+    bstack1llll11l1_opy_.close()
+    logger.info(bstack1lll1l1l1_opy_)
+    try:
+      os.environ[bstack11_opy_ (u"ࠫࡇࡘࡏࡘࡕࡈࡖࡘ࡚ࡁࡄࡍࡢࡊࡗࡇࡍࡆ࡙ࡒࡖࡐ࠭ೞ")] = bstack1l1l1l11_opy_.framework if bstack1l1l1l11_opy_.framework != None else bstack11_opy_ (u"ࠧࠨ೟")
+      config = yaml.safe_load(bstack1l1ll1l_opy_)
+      config[bstack11_opy_ (u"࠭ࡳࡰࡷࡵࡧࡪ࠭ೠ")] = bstack11_opy_ (u"ࠧࡱࡻࡷ࡬ࡴࡴ࠭ࡴࡧࡷࡹࡵ࠭ೡ")
+      bstack111l1lll_opy_(bstack1llll_opy_, config)
+    except Exception as e:
+      logger.debug(bstack1l1llllll_opy_.format(str(e)))
+  except Exception as e:
+    logger.error(bstack11l1llll_opy_.format(str(e)))
+def bstack111l1lll_opy_(bstack1111lll1_opy_, config, bstack11lll111_opy_ = {}):
+  global bstack11llll11_opy_
   if not config:
     return
-  bstack1llllll11_opy_ = bstack11ll111l_opy_ if not bstack111lllll_opy_ else ( bstack1l1l1l111_opy_ if bstack1ll1_opy_ (u"ࠩࡤࡴࡵ࠭ಹ") in config else bstack1lllllll_opy_ )
+  bstack1l1llll_opy_ = bstack11ll11l_opy_ if not bstack11llll11_opy_ else ( bstack1llll1lll_opy_ if bstack11_opy_ (u"ࠨࡣࡳࡴࠬೢ") in config else bstack1l111111_opy_ )
   data = {
-    bstack1ll1_opy_ (u"ࠪࡹࡸ࡫ࡲࡏࡣࡰࡩࠬ಺"): config[bstack1ll1_opy_ (u"ࠫࡺࡹࡥࡳࡐࡤࡱࡪ࠭಻")],
-    bstack1ll1_opy_ (u"ࠬࡧࡣࡤࡧࡶࡷࡐ࡫ࡹࠨ಼"): config[bstack1ll1_opy_ (u"࠭ࡡࡤࡥࡨࡷࡸࡑࡥࡺࠩಽ")],
-    bstack1ll1_opy_ (u"ࠧࡦࡸࡨࡲࡹࡥࡴࡺࡲࡨࠫಾ"): bstack111l1l11_opy_,
-    bstack1ll1_opy_ (u"ࠨࡧࡹࡩࡳࡺ࡟ࡱࡴࡲࡴࡪࡸࡴࡪࡧࡶࠫಿ"): {
-      bstack1ll1_opy_ (u"ࠩ࡯ࡥࡳ࡭ࡵࡢࡩࡨࡣ࡫ࡸࡡ࡮ࡧࡺࡳࡷࡱࠧೀ"): str(config[bstack1ll1_opy_ (u"ࠪࡷࡴࡻࡲࡤࡧࠪು")]) if bstack1ll1_opy_ (u"ࠫࡸࡵࡵࡳࡥࡨࠫೂ") in config else bstack1ll1_opy_ (u"ࠧࡻ࡮࡬ࡰࡲࡻࡳࠨೃ"),
-      bstack1ll1_opy_ (u"࠭ࡲࡦࡨࡨࡶࡷ࡫ࡲࠨೄ"): bstack1111ll11_opy_(os.getenv(bstack1ll1_opy_ (u"ࠢࡃࡔࡒ࡛ࡘࡋࡒࡔࡖࡄࡇࡐࡥࡆࡓࡃࡐࡉ࡜ࡕࡒࡌࠤ೅"), bstack1ll1_opy_ (u"ࠣࠤೆ"))),
-      bstack1ll1_opy_ (u"ࠩ࡯ࡥࡳ࡭ࡵࡢࡩࡨࠫೇ"): bstack1ll1_opy_ (u"ࠪࡴࡾࡺࡨࡰࡰࠪೈ"),
-      bstack1ll1_opy_ (u"ࠫࡵࡸ࡯ࡥࡷࡦࡸࠬ೉"): bstack1llllll11_opy_,
-      bstack1ll1_opy_ (u"ࠬࡨࡵࡪ࡮ࡧࡒࡦࡳࡥࠨೊ"): config[bstack1ll1_opy_ (u"࠭ࡢࡶ࡫࡯ࡨࡓࡧ࡭ࡦࠩೋ")]if config[bstack1ll1_opy_ (u"ࠧࡣࡷ࡬ࡰࡩࡔࡡ࡮ࡧࠪೌ")] else bstack1ll1_opy_ (u"ࠣࡷࡱ࡯ࡳࡵࡷ࡯ࠤ್"),
-      bstack1ll1_opy_ (u"ࠩࡥࡹ࡮ࡲࡤࡊࡦࡨࡲࡹ࡯ࡦࡪࡧࡵࠫ೎"): str(config[bstack1ll1_opy_ (u"ࠪࡦࡺ࡯࡬ࡥࡋࡧࡩࡳࡺࡩࡧ࡫ࡨࡶࠬ೏")]) if bstack1ll1_opy_ (u"ࠫࡧࡻࡩ࡭ࡦࡌࡨࡪࡴࡴࡪࡨ࡬ࡩࡷ࠭೐") in config else bstack1ll1_opy_ (u"ࠧࡻ࡮࡬ࡰࡲࡻࡳࠨ೑"),
-      bstack1ll1_opy_ (u"࠭࡯ࡴࠩ೒"): sys.platform,
-      bstack1ll1_opy_ (u"ࠧࡩࡱࡶࡸࡳࡧ࡭ࡦࠩ೓"): socket.gethostname()
+    bstack11_opy_ (u"ࠩࡸࡷࡪࡸࡎࡢ࡯ࡨࠫೣ"): config[bstack11_opy_ (u"ࠪࡹࡸ࡫ࡲࡏࡣࡰࡩࠬ೤")],
+    bstack11_opy_ (u"ࠫࡦࡩࡣࡦࡵࡶࡏࡪࡿࠧ೥"): config[bstack11_opy_ (u"ࠬࡧࡣࡤࡧࡶࡷࡐ࡫ࡹࠨ೦")],
+    bstack11_opy_ (u"࠭ࡥࡷࡧࡱࡸࡤࡺࡹࡱࡧࠪ೧"): bstack1111lll1_opy_,
+    bstack11_opy_ (u"ࠧࡦࡸࡨࡲࡹࡥࡰࡳࡱࡳࡩࡷࡺࡩࡦࡵࠪ೨"): {
+      bstack11_opy_ (u"ࠨ࡮ࡤࡲ࡬ࡻࡡࡨࡧࡢࡪࡷࡧ࡭ࡦࡹࡲࡶࡰ࠭೩"): str(config[bstack11_opy_ (u"ࠩࡶࡳࡺࡸࡣࡦࠩ೪")]) if bstack11_opy_ (u"ࠪࡷࡴࡻࡲࡤࡧࠪ೫") in config else bstack11_opy_ (u"ࠦࡺࡴ࡫࡯ࡱࡺࡲࠧ೬"),
+      bstack11_opy_ (u"ࠬࡸࡥࡧࡧࡵࡶࡪࡸࠧ೭"): bstack1l111llll_opy_(os.getenv(bstack11_opy_ (u"ࠨࡂࡓࡑ࡚ࡗࡊࡘࡓࡕࡃࡆࡏࡤࡌࡒࡂࡏࡈ࡛ࡔࡘࡋࠣ೮"), bstack11_opy_ (u"ࠢࠣ೯"))),
+      bstack11_opy_ (u"ࠨ࡮ࡤࡲ࡬ࡻࡡࡨࡧࠪ೰"): bstack11_opy_ (u"ࠩࡳࡽࡹ࡮࡯࡯ࠩೱ"),
+      bstack11_opy_ (u"ࠪࡴࡷࡵࡤࡶࡥࡷࠫೲ"): bstack1l1llll_opy_,
+      bstack11_opy_ (u"ࠫࡧࡻࡩ࡭ࡦࡑࡥࡲ࡫ࠧೳ"): config[bstack11_opy_ (u"ࠬࡨࡵࡪ࡮ࡧࡒࡦࡳࡥࠨ೴")]if config[bstack11_opy_ (u"࠭ࡢࡶ࡫࡯ࡨࡓࡧ࡭ࡦࠩ೵")] else bstack11_opy_ (u"ࠢࡶࡰ࡮ࡲࡴࡽ࡮ࠣ೶"),
+      bstack11_opy_ (u"ࠨࡤࡸ࡭ࡱࡪࡉࡥࡧࡱࡸ࡮࡬ࡩࡦࡴࠪ೷"): str(config[bstack11_opy_ (u"ࠩࡥࡹ࡮ࡲࡤࡊࡦࡨࡲࡹ࡯ࡦࡪࡧࡵࠫ೸")]) if bstack11_opy_ (u"ࠪࡦࡺ࡯࡬ࡥࡋࡧࡩࡳࡺࡩࡧ࡫ࡨࡶࠬ೹") in config else bstack11_opy_ (u"ࠦࡺࡴ࡫࡯ࡱࡺࡲࠧ೺"),
+      bstack11_opy_ (u"ࠬࡵࡳࠨ೻"): sys.platform,
+      bstack11_opy_ (u"࠭ࡨࡰࡵࡷࡲࡦࡳࡥࠨ೼"): socket.gethostname()
     }
   }
-  update(data[bstack1ll1_opy_ (u"ࠨࡧࡹࡩࡳࡺ࡟ࡱࡴࡲࡴࡪࡸࡴࡪࡧࡶࠫ೔")], bstack111l1ll_opy_)
+  update(data[bstack11_opy_ (u"ࠧࡦࡸࡨࡲࡹࡥࡰࡳࡱࡳࡩࡷࡺࡩࡦࡵࠪ೽")], bstack11lll111_opy_)
   try:
-    response = bstack1l11lll1_opy_(bstack1ll1_opy_ (u"ࠩࡓࡓࡘ࡚ࠧೕ"), bstack1llll11l_opy_, data, config)
+    response = bstack1lll1_opy_(bstack11_opy_ (u"ࠨࡒࡒࡗ࡙࠭೾"), bstack1l11ll111_opy_, data, config)
     if response:
-      logger.debug(bstack11ll11_opy_.format(bstack111l1l11_opy_, str(response.json())))
+      logger.debug(bstack1lll1l1ll_opy_.format(bstack1111lll1_opy_, str(response.json())))
   except Exception as e:
-    logger.debug(bstack1l1l11111_opy_.format(str(e)))
-def bstack1l11lll1_opy_(type, url, data, config):
-  bstack1lll1lll1_opy_ = bstack1l1l11_opy_.format(url)
-  proxy = bstack111l1111_opy_(config)
+    logger.debug(bstack11ll11ll_opy_.format(str(e)))
+def bstack1lll1_opy_(type, url, data, config):
+  bstack111l11_opy_ = bstack1l1l111_opy_.format(url)
+  proxy = bstack1ll11ll1l_opy_(config)
   proxies = {}
   response = {}
-  if config.get(bstack1ll1_opy_ (u"ࠪ࡬ࡹࡺࡰࡑࡴࡲࡼࡾ࠭ೖ")):
+  if config.get(bstack11_opy_ (u"ࠩ࡫ࡸࡹࡶࡐࡳࡱࡻࡽࠬ೿")) or config.get(bstack11_opy_ (u"ࠪ࡬ࡹࡺࡰࡴࡒࡵࡳࡽࡿࠧഀ")):
     proxies = {
-      bstack1ll1_opy_ (u"ࠫ࡭ࡺࡴࡱࡵࠪ೗"): proxy
+      bstack11_opy_ (u"ࠫ࡭ࡺࡴࡱࡵࠪഁ"): proxy
     }
-  if config.get(bstack1ll1_opy_ (u"ࠬ࡮ࡴࡵࡲࡶࡔࡷࡵࡸࡺࠩ೘")):
-    proxies = {
-      bstack1ll1_opy_ (u"࠭ࡨࡵࡶࡳࡷࠬ೙"): proxy
-    }
-  if type == bstack1ll1_opy_ (u"ࠧࡑࡑࡖࡘࠬ೚"):
-    response = requests.post(bstack1lll1lll1_opy_, json=data,
-                    headers={bstack1ll1_opy_ (u"ࠨࡅࡲࡲࡹ࡫࡮ࡵ࠯ࡗࡽࡵ࡫ࠧ೛"): bstack1ll1_opy_ (u"ࠩࡤࡴࡵࡲࡩࡤࡣࡷ࡭ࡴࡴ࠯࡫ࡵࡲࡲࠬ೜")}, auth=(config[bstack1ll1_opy_ (u"ࠪࡹࡸ࡫ࡲࡏࡣࡰࡩࠬೝ")], config[bstack1ll1_opy_ (u"ࠫࡦࡩࡣࡦࡵࡶࡏࡪࡿࠧೞ")]), proxies=proxies)
+  if type == bstack11_opy_ (u"ࠬࡖࡏࡔࡖࠪം"):
+    response = requests.post(bstack111l11_opy_, json=data,
+                    headers={bstack11_opy_ (u"࠭ࡃࡰࡰࡷࡩࡳࡺ࠭ࡕࡻࡳࡩࠬഃ"): bstack11_opy_ (u"ࠧࡢࡲࡳࡰ࡮ࡩࡡࡵ࡫ࡲࡲ࠴ࡰࡳࡰࡰࠪഄ")}, auth=(config[bstack11_opy_ (u"ࠨࡷࡶࡩࡷࡔࡡ࡮ࡧࠪഅ")], config[bstack11_opy_ (u"ࠩࡤࡧࡨ࡫ࡳࡴࡍࡨࡽࠬആ")]), proxies=proxies)
   return response
-def bstack1111ll11_opy_(framework):
-  return bstack1ll1_opy_ (u"ࠧࢁࡽ࠮ࡲࡼࡸ࡭ࡵ࡮ࡢࡩࡨࡲࡹ࠵ࡻࡾࠤ೟").format(str(framework), __version__) if framework else bstack1ll1_opy_ (u"ࠨࡰࡺࡶ࡫ࡳࡳࡧࡧࡦࡰࡷ࠳ࢀࢃࠢೠ").format(__version__)
-def bstack1ll11l1ll_opy_():
+def bstack1l111llll_opy_(framework):
+  return bstack11_opy_ (u"ࠥࡿࢂ࠳ࡰࡺࡶ࡫ࡳࡳࡧࡧࡦࡰࡷ࠳ࢀࢃࠢഇ").format(str(framework), __version__) if framework else bstack11_opy_ (u"ࠦࡵࡿࡴࡩࡱࡱࡥ࡬࡫࡮ࡵ࠱ࡾࢁࠧഈ").format(__version__)
+def bstack1l1lll1l1_opy_():
   global CONFIG
   if bool(CONFIG):
     return
-  bstack1lll1ll11_opy_()
-  logger.debug(bstack1l1ll1_opy_.format(str(CONFIG)))
-  bstack11l111ll_opy_()
-  sys.excepthook = bstack11l11l1l_opy_
-  atexit.register(bstack1l1l11l1l_opy_)
-  signal.signal(signal.SIGINT, bstack1l1llll11_opy_)
-  signal.signal(signal.SIGTERM, bstack1l1llll11_opy_)
-def bstack11l11l1l_opy_(exctype, value, traceback):
-  global bstack111l_opy_
   try:
-    for driver in bstack111l_opy_:
+    bstack111ll1ll_opy_()
+    logger.debug(bstack1l1l1ll11_opy_.format(str(CONFIG)))
+    bstack1l1l1111_opy_()
+  except Exception as e:
+    logger.error(bstack11_opy_ (u"ࠧࡌࡡࡪ࡮ࡨࡨࠥࡺ࡯ࠡࡵࡨࡸࡺࡶࠬࠡࡧࡵࡶࡴࡸ࠺ࠡࠤഉ") + str(e))
+    sys.exit(1)
+  sys.excepthook = bstack1l1l1l111_opy_
+  atexit.register(bstack1111l_opy_)
+  signal.signal(signal.SIGINT, bstack1ll11llll_opy_)
+  signal.signal(signal.SIGTERM, bstack1ll11llll_opy_)
+def bstack1l1l1l111_opy_(exctype, value, traceback):
+  global bstack1ll1l1l1_opy_
+  try:
+    for driver in bstack1ll1l1l1_opy_:
       driver.execute_script(
-        bstack1ll1_opy_ (u"ࠧࡣࡴࡲࡻࡸ࡫ࡲࡴࡶࡤࡧࡰࡥࡥࡹࡧࡦࡹࡹࡵࡲ࠻ࠢࡾࠦࡦࡩࡴࡪࡱࡱࠦ࠿ࠦࠢࡴࡧࡷࡗࡪࡹࡳࡪࡱࡱࡗࡹࡧࡴࡶࡵࠥ࠰ࠥࠨࡡࡳࡩࡸࡱࡪࡴࡴࡴࠤ࠽ࠤࢀࠨࡳࡵࡣࡷࡹࡸࠨ࠺ࠣࡨࡤ࡭ࡱ࡫ࡤࠣ࠮ࠣࠦࡷ࡫ࡡࡴࡱࡱࠦ࠿ࠦࠧೡ") + json.dumps(bstack1ll1_opy_ (u"ࠣࡕࡨࡷࡸ࡯࡯࡯ࠢࡩࡥ࡮ࡲࡥࡥࠢࡺ࡭ࡹ࡮࠺ࠡ࡞ࡱࠦೢ") + str(value)) + bstack1ll1_opy_ (u"ࠩࢀࢁࠬೣ"))
+        bstack11_opy_ (u"࠭ࡢࡳࡱࡺࡷࡪࡸࡳࡵࡣࡦ࡯ࡤ࡫ࡸࡦࡥࡸࡸࡴࡸ࠺ࠡࡽࠥࡥࡨࡺࡩࡰࡰࠥ࠾ࠥࠨࡳࡦࡶࡖࡩࡸࡹࡩࡰࡰࡖࡸࡦࡺࡵࡴࠤ࠯ࠤࠧࡧࡲࡨࡷࡰࡩࡳࡺࡳࠣ࠼ࠣࡿࠧࡹࡴࡢࡶࡸࡷࠧࡀࠢࡧࡣ࡬ࡰࡪࡪࠢ࠭ࠢࠥࡶࡪࡧࡳࡰࡰࠥ࠾ࠥ࠭ഊ") + json.dumps(bstack11_opy_ (u"ࠢࡔࡧࡶࡷ࡮ࡵ࡮ࠡࡨࡤ࡭ࡱ࡫ࡤࠡࡹ࡬ࡸ࡭ࡀࠠ࡝ࡰࠥഋ") + str(value)) + bstack11_opy_ (u"ࠨࡿࢀࠫഌ"))
   except Exception:
     pass
-  bstack11111l1_opy_(value)
+  bstack1ll1ll1_opy_(value)
   sys.__excepthook__(exctype, value, traceback)
-def bstack11111l1_opy_(message = bstack1ll1_opy_ (u"ࠪࠫ೤")):
+  sys.exit(1)
+def bstack1ll1ll1_opy_(message = bstack11_opy_ (u"ࠩࠪ഍")):
   global CONFIG
   try:
     if message:
-      bstack111l1ll_opy_ = {
-        bstack1ll1_opy_ (u"ࠫࡪࡸࡲࡰࡴࠪ೥"): str(message)
+      bstack11lll111_opy_ = {
+        bstack11_opy_ (u"ࠪࡩࡷࡸ࡯ࡳࠩഎ"): str(message)
       }
-      bstack1l11l1l_opy_(bstack1lll1l111_opy_, CONFIG, bstack111l1ll_opy_)
+      bstack111l1lll_opy_(bstack1llll111_opy_, CONFIG, bstack11lll111_opy_)
     else:
-      bstack1l11l1l_opy_(bstack1lll1l111_opy_, CONFIG)
+      bstack111l1lll_opy_(bstack1llll111_opy_, CONFIG)
   except Exception as e:
-    logger.debug(bstack1l1lll11l_opy_.format(str(e)))
-def bstack11l1lll_opy_(bstack11lll1l1_opy_, size):
-  bstack1ll111ll1_opy_ = []
-  while len(bstack11lll1l1_opy_) > size:
-    bstack1l1111l1_opy_ = bstack11lll1l1_opy_[:size]
-    bstack1ll111ll1_opy_.append(bstack1l1111l1_opy_)
-    bstack11lll1l1_opy_   = bstack11lll1l1_opy_[size:]
-  bstack1ll111ll1_opy_.append(bstack11lll1l1_opy_)
-  return bstack1ll111ll1_opy_
+    logger.debug(bstack11111l1l_opy_.format(str(e)))
+def bstack1111ll1l_opy_(bstack1ll1lll1l_opy_, size):
+  bstack1lllll111_opy_ = []
+  while len(bstack1ll1lll1l_opy_) > size:
+    bstack1l1111l1l_opy_ = bstack1ll1lll1l_opy_[:size]
+    bstack1lllll111_opy_.append(bstack1l1111l1l_opy_)
+    bstack1ll1lll1l_opy_   = bstack1ll1lll1l_opy_[size:]
+  bstack1lllll111_opy_.append(bstack1ll1lll1l_opy_)
+  return bstack1lllll111_opy_
 def run_on_browserstack():
   if len(sys.argv) <= 1:
-    logger.critical(bstack1lll1lll_opy_)
+    logger.critical(bstack1l11l1l1_opy_)
     return
-  if sys.argv[1] == bstack1ll1_opy_ (u"ࠬ࠳࠭ࡷࡧࡵࡷ࡮ࡵ࡮ࠨ೦")  or sys.argv[1] == bstack1ll1_opy_ (u"࠭࠭ࡷࠩ೧"):
-    logger.info(bstack1ll1_opy_ (u"ࠧࡃࡴࡲࡻࡸ࡫ࡲࡴࡶࡤࡧࡰࠦࡐࡺࡶ࡫ࡳࡳࠦࡓࡅࡍࠣࡺࢀࢃࠧ೨").format(__version__))
+  if sys.argv[1] == bstack11_opy_ (u"ࠫ࠲࠳ࡶࡦࡴࡶ࡭ࡴࡴࠧഏ")  or sys.argv[1] == bstack11_opy_ (u"ࠬ࠳ࡶࠨഐ"):
+    logger.info(bstack11_opy_ (u"࠭ࡂࡳࡱࡺࡷࡪࡸࡳࡵࡣࡦ࡯ࠥࡖࡹࡵࡪࡲࡲ࡙ࠥࡄࡌࠢࡹࡿࢂ࠭഑").format(__version__))
     return
-  if sys.argv[1] == bstack1ll1_opy_ (u"ࠨࡵࡨࡸࡺࡶࠧ೩"):
-    bstack11ll111_opy_()
+  if sys.argv[1] == bstack11_opy_ (u"ࠧࡴࡧࡷࡹࡵ࠭ഒ"):
+    bstack1111l11_opy_()
     return
   args = sys.argv
-  bstack1ll11l1ll_opy_()
+  bstack1l1lll1l1_opy_()
   global CONFIG
-  global bstack1llll1_opy_
-  global bstack1l1ll1l_opy_
-  global bstack1111ll_opy_
-  global bstack111l1lll_opy_
-  global bstack11l1l11l_opy_
-  bstack1l1ll1lll_opy_ = bstack1ll1_opy_ (u"ࠩࠪ೪")
-  if args[1] == bstack1ll1_opy_ (u"ࠪࡴࡾࡺࡨࡰࡰࠪ೫") or args[1] == bstack1ll1_opy_ (u"ࠫࡵࡿࡴࡩࡱࡱ࠷ࠬ೬"):
-    bstack1l1ll1lll_opy_ = bstack1ll1_opy_ (u"ࠬࡶࡹࡵࡪࡲࡲࠬ೭")
+  global bstack1l11ll1ll_opy_
+  global bstack1l11llll_opy_
+  global bstack1l111l11l_opy_
+  global bstack1l11l111_opy_
+  global bstack11llll1l_opy_
+  bstack1l1l11l11_opy_ = bstack11_opy_ (u"ࠨࠩഓ")
+  if args[1] == bstack11_opy_ (u"ࠩࡳࡽࡹ࡮࡯࡯ࠩഔ") or args[1] == bstack11_opy_ (u"ࠪࡴࡾࡺࡨࡰࡰ࠶ࠫക"):
+    bstack1l1l11l11_opy_ = bstack11_opy_ (u"ࠫࡵࡿࡴࡩࡱࡱࠫഖ")
     args = args[2:]
-  elif args[1] == bstack1ll1_opy_ (u"࠭ࡲࡰࡤࡲࡸࠬ೮"):
-    bstack1l1ll1lll_opy_ = bstack1ll1_opy_ (u"ࠧࡳࡱࡥࡳࡹ࠭೯")
+  elif args[1] == bstack11_opy_ (u"ࠬࡸ࡯ࡣࡱࡷࠫഗ"):
+    bstack1l1l11l11_opy_ = bstack11_opy_ (u"࠭ࡲࡰࡤࡲࡸࠬഘ")
     args = args[2:]
-  elif args[1] == bstack1ll1_opy_ (u"ࠨࡲࡤࡦࡴࡺࠧ೰"):
-    bstack1l1ll1lll_opy_ = bstack1ll1_opy_ (u"ࠩࡳࡥࡧࡵࡴࠨೱ")
+  elif args[1] == bstack11_opy_ (u"ࠧࡱࡣࡥࡳࡹ࠭ങ"):
+    bstack1l1l11l11_opy_ = bstack11_opy_ (u"ࠨࡲࡤࡦࡴࡺࠧച")
     args = args[2:]
-  elif args[1] == bstack1ll1_opy_ (u"ࠪࡶࡴࡨ࡯ࡵ࠯࡬ࡲࡹ࡫ࡲ࡯ࡣ࡯ࠫೲ"):
-    bstack1l1ll1lll_opy_ = bstack1ll1_opy_ (u"ࠫࡷࡵࡢࡰࡶ࠰࡭ࡳࡺࡥࡳࡰࡤࡰࠬೳ")
+  elif args[1] == bstack11_opy_ (u"ࠩࡵࡳࡧࡵࡴ࠮࡫ࡱࡸࡪࡸ࡮ࡢ࡮ࠪഛ"):
+    bstack1l1l11l11_opy_ = bstack11_opy_ (u"ࠪࡶࡴࡨ࡯ࡵ࠯࡬ࡲࡹ࡫ࡲ࡯ࡣ࡯ࠫജ")
     args = args[2:]
-  elif args[1] == bstack1ll1_opy_ (u"ࠬࡶࡹࡵࡧࡶࡸࠬ೴"):
-    bstack1l1ll1lll_opy_ = bstack1ll1_opy_ (u"࠭ࡰࡺࡶࡨࡷࡹ࠭೵")
+  elif args[1] == bstack11_opy_ (u"ࠫࡵࡿࡴࡦࡵࡷࠫഝ"):
+    bstack1l1l11l11_opy_ = bstack11_opy_ (u"ࠬࡶࡹࡵࡧࡶࡸࠬഞ")
     args = args[2:]
-  elif args[1] == bstack1ll1_opy_ (u"ࠧࡣࡧ࡫ࡥࡻ࡫ࠧ೶"):
-    bstack1l1ll1lll_opy_ = bstack1ll1_opy_ (u"ࠨࡤࡨ࡬ࡦࡼࡥࠨ೷")
+  elif args[1] == bstack11_opy_ (u"࠭ࡢࡦࡪࡤࡺࡪ࠭ട"):
+    bstack1l1l11l11_opy_ = bstack11_opy_ (u"ࠧࡣࡧ࡫ࡥࡻ࡫ࠧഠ")
     args = args[2:]
   else:
-    if not bstack1ll1_opy_ (u"ࠩࡩࡶࡦࡳࡥࡸࡱࡵ࡯ࠬ೸") in CONFIG or str(CONFIG[bstack1ll1_opy_ (u"ࠪࡪࡷࡧ࡭ࡦࡹࡲࡶࡰ࠭೹")]).lower() in [bstack1ll1_opy_ (u"ࠫࡵࡿࡴࡩࡱࡱࠫ೺"), bstack1ll1_opy_ (u"ࠬࡶࡹࡵࡪࡲࡲ࠸࠭೻")]:
-      bstack1l1ll1lll_opy_ = bstack1ll1_opy_ (u"࠭ࡰࡺࡶ࡫ࡳࡳ࠭೼")
+    if not bstack11_opy_ (u"ࠨࡨࡵࡥࡲ࡫ࡷࡰࡴ࡮ࠫഡ") in CONFIG or str(CONFIG[bstack11_opy_ (u"ࠩࡩࡶࡦࡳࡥࡸࡱࡵ࡯ࠬഢ")]).lower() in [bstack11_opy_ (u"ࠪࡴࡾࡺࡨࡰࡰࠪണ"), bstack11_opy_ (u"ࠫࡵࡿࡴࡩࡱࡱ࠷ࠬത")]:
+      bstack1l1l11l11_opy_ = bstack11_opy_ (u"ࠬࡶࡹࡵࡪࡲࡲࠬഥ")
       args = args[1:]
-    elif str(CONFIG[bstack1ll1_opy_ (u"ࠧࡧࡴࡤࡱࡪࡽ࡯ࡳ࡭ࠪ೽")]).lower() == bstack1ll1_opy_ (u"ࠨࡴࡲࡦࡴࡺࠧ೾"):
-      bstack1l1ll1lll_opy_ = bstack1ll1_opy_ (u"ࠩࡵࡳࡧࡵࡴࠨ೿")
+    elif str(CONFIG[bstack11_opy_ (u"࠭ࡦࡳࡣࡰࡩࡼࡵࡲ࡬ࠩദ")]).lower() == bstack11_opy_ (u"ࠧࡳࡱࡥࡳࡹ࠭ധ"):
+      bstack1l1l11l11_opy_ = bstack11_opy_ (u"ࠨࡴࡲࡦࡴࡺࠧന")
       args = args[1:]
-    elif str(CONFIG[bstack1ll1_opy_ (u"ࠪࡪࡷࡧ࡭ࡦࡹࡲࡶࡰ࠭ഀ")]).lower() == bstack1ll1_opy_ (u"ࠫࡵࡧࡢࡰࡶࠪഁ"):
-      bstack1l1ll1lll_opy_ = bstack1ll1_opy_ (u"ࠬࡶࡡࡣࡱࡷࠫം")
+    elif str(CONFIG[bstack11_opy_ (u"ࠩࡩࡶࡦࡳࡥࡸࡱࡵ࡯ࠬഩ")]).lower() == bstack11_opy_ (u"ࠪࡴࡦࡨ࡯ࡵࠩപ"):
+      bstack1l1l11l11_opy_ = bstack11_opy_ (u"ࠫࡵࡧࡢࡰࡶࠪഫ")
       args = args[1:]
-    elif str(CONFIG[bstack1ll1_opy_ (u"࠭ࡦࡳࡣࡰࡩࡼࡵࡲ࡬ࠩഃ")]).lower() == bstack1ll1_opy_ (u"ࠧࡱࡻࡷࡩࡸࡺࠧഄ"):
-      bstack1l1ll1lll_opy_ = bstack1ll1_opy_ (u"ࠨࡲࡼࡸࡪࡹࡴࠨഅ")
+    elif str(CONFIG[bstack11_opy_ (u"ࠬ࡬ࡲࡢ࡯ࡨࡻࡴࡸ࡫ࠨബ")]).lower() == bstack11_opy_ (u"࠭ࡰࡺࡶࡨࡷࡹ࠭ഭ"):
+      bstack1l1l11l11_opy_ = bstack11_opy_ (u"ࠧࡱࡻࡷࡩࡸࡺࠧമ")
       args = args[1:]
-    elif str(CONFIG[bstack1ll1_opy_ (u"ࠩࡩࡶࡦࡳࡥࡸࡱࡵ࡯ࠬആ")]).lower() == bstack1ll1_opy_ (u"ࠪࡦࡪ࡮ࡡࡷࡧࠪഇ"):
-      bstack1l1ll1lll_opy_ = bstack1ll1_opy_ (u"ࠫࡧ࡫ࡨࡢࡸࡨࠫഈ")
+    elif str(CONFIG[bstack11_opy_ (u"ࠨࡨࡵࡥࡲ࡫ࡷࡰࡴ࡮ࠫയ")]).lower() == bstack11_opy_ (u"ࠩࡥࡩ࡭ࡧࡶࡦࠩര"):
+      bstack1l1l11l11_opy_ = bstack11_opy_ (u"ࠪࡦࡪ࡮ࡡࡷࡧࠪറ")
       args = args[1:]
     else:
-      os.environ[bstack1ll1_opy_ (u"ࠬࡈࡒࡐ࡙ࡖࡉࡗ࡙ࡔࡂࡅࡎࡣࡋࡘࡁࡎࡇ࡚ࡓࡗࡑࠧഉ")] = bstack1l1ll1lll_opy_
-      bstack1ll1lll_opy_(bstack1111l1l1_opy_)
-  global bstack1lll1l_opy_
-  try:
-    os.environ[bstack1ll1_opy_ (u"࠭ࡂࡓࡑ࡚ࡗࡊࡘࡓࡕࡃࡆࡏࡤࡌࡒࡂࡏࡈ࡛ࡔࡘࡋࠨഊ")] = bstack1l1ll1lll_opy_
-    bstack1l11l1l_opy_(bstack1l1llll1l_opy_, CONFIG)
-  except Exception as e:
-    logger.debug(bstack1l1lll11l_opy_.format(str(e)))
-  global bstack1lll1_opy_
-  global bstack1ll1l11l_opy_
-  global bstack1111l11l_opy_
+      os.environ[bstack11_opy_ (u"ࠫࡇࡘࡏࡘࡕࡈࡖࡘ࡚ࡁࡄࡍࡢࡊࡗࡇࡍࡆ࡙ࡒࡖࡐ࠭ല")] = bstack1l1l11l11_opy_
+      bstack11111l11_opy_(bstack111ll111_opy_)
+  global bstack1ll1ll1ll_opy_
+  try:
+    os.environ[bstack11_opy_ (u"ࠬࡈࡒࡐ࡙ࡖࡉࡗ࡙ࡔࡂࡅࡎࡣࡋࡘࡁࡎࡇ࡚ࡓࡗࡑࠧള")] = bstack1l1l11l11_opy_
+    bstack111l1lll_opy_(bstack1l1ll1ll1_opy_, CONFIG)
+  except Exception as e:
+    logger.debug(bstack11111l1l_opy_.format(str(e)))
+  global bstack1ll1l11ll_opy_
+  global bstack11111ll_opy_
+  global bstack1lll1ll1_opy_
+  global bstack11ll_opy_
+  global bstack1l11ll1_opy_
+  global bstack11ll1l_opy_
+  global bstack1111ll11_opy_
+  global bstack1lll1llll_opy_
   global bstack11l11ll1_opy_
-  global bstack1ll111_opy_
-  global bstack1111l1ll_opy_
-  global bstack1ll11111_opy_
-  global bstack1ll1l1ll1_opy_
-  global bstack1l1ll11ll_opy_
-  global bstack1ll1111_opy_
-  global bstack1l1lll_opy_
-  global bstack111lll1l_opy_
-  global bstack11ll1l1l_opy_
+  global bstack111l1ll_opy_
+  global bstack1lllll11_opy_
+  global bstack111ll_opy_
+  global bstack1l11lll11_opy_
   try:
     from selenium import webdriver
     from selenium.webdriver.remote.webdriver import WebDriver
   except Exception as e:
-    logger.warn(bstack11l11_opy_ + str(e))
-  bstack1lll1_opy_ = webdriver.Remote.__init__
-  bstack1ll1l1ll1_opy_ = WebDriver.close
+    logger.warn(bstack11l1l1l1_opy_ + str(e))
+  bstack1ll1l11ll_opy_ = webdriver.Remote.__init__
+  bstack1lll1llll_opy_ = WebDriver.close
   try:
     import Browser
     from subprocess import Popen
-    bstack1lll1l_opy_ = Popen.__init__
+    bstack1ll1ll1ll_opy_ = Popen.__init__
   except Exception as e:
-    logger.debug(bstack1llll111l_opy_ + str(e))
-  bstack1l1lll_opy_ = WebDriver.get
-  if bstack11l1l1ll_opy_():
-    if bstack1ll1llll_opy_() < version.parse(bstack1lllll1l_opy_):
-      logger.error(bstack11lllll_opy_.format(bstack1ll1llll_opy_()))
+    logger.debug(bstack1ll1lll11_opy_ + str(e))
+  bstack1lllll11_opy_ = WebDriver.get
+  if bstack1111ll1_opy_():
+    if bstack1ll11l1ll_opy_() < version.parse(bstack1l1ll111_opy_):
+      logger.error(bstack1llll11ll_opy_.format(bstack1ll11l1ll_opy_()))
     else:
       try:
         from selenium.webdriver.remote.remote_connection import RemoteConnection
-        bstack111lll1l_opy_ = RemoteConnection._get_proxy_url
+        bstack111ll_opy_ = RemoteConnection._get_proxy_url
       except Exception as e:
-        logger.error(bstack1l11ll1ll_opy_.format(str(e)))
-  if (bstack1l1ll1lll_opy_ in [bstack1ll1_opy_ (u"ࠧࡱࡣࡥࡳࡹ࠭ഋ"), bstack1ll1_opy_ (u"ࠨࡴࡲࡦࡴࡺࠧഌ"), bstack1ll1_opy_ (u"ࠩࡵࡳࡧࡵࡴ࠮࡫ࡱࡸࡪࡸ࡮ࡢ࡮ࠪ഍")]):
+        logger.error(bstack11ll11_opy_.format(str(e)))
+  bstack11l11l1l_opy_()
+  if (bstack1l1l11l11_opy_ in [bstack11_opy_ (u"࠭ࡰࡢࡤࡲࡸࠬഴ"), bstack11_opy_ (u"ࠧࡳࡱࡥࡳࡹ࠭വ"), bstack11_opy_ (u"ࠨࡴࡲࡦࡴࡺ࠭ࡪࡰࡷࡩࡷࡴࡡ࡭ࠩശ")]):
     try:
       from robot import run_cli
       from robot.output import Output
       from robot.running.status import TestStatus
       from pabot.pabot import QueueItem
       from pabot import pabot
       try:
         from SeleniumLibrary.keywords.webdrivertools.webdrivertools import WebDriverCreator
-        WebDriverCreator._get_ff_profile = bstack1l111l1l_opy_
+        WebDriverCreator._get_ff_profile = bstack1l11l1_opy_
       except Exception as e:
-        logger.warn(bstack1llll1ll1_opy_ + str(e))
+        logger.warn(bstack11l111ll_opy_ + str(e))
     except Exception as e:
-      bstack11l1_opy_(e, bstack1llll1ll1_opy_)
-    bstack1ll1l11l_opy_ = Output.end_test
-    bstack1111l11l_opy_ = TestStatus.__init__
-    bstack1ll111_opy_ = pabot._run
-    bstack1111l1ll_opy_ = QueueItem.__init__
-    bstack1ll11111_opy_ = pabot._create_command_for_execution
-  if bstack1l1ll1lll_opy_ == bstack1ll1_opy_ (u"ࠪࡦࡪ࡮ࡡࡷࡧࠪഎ"):
+      bstack111lll1l_opy_(e, bstack11l111ll_opy_)
+    bstack11111ll_opy_ = Output.end_test
+    bstack1lll1ll1_opy_ = TestStatus.__init__
+    bstack1l11ll1_opy_ = pabot._run
+    bstack11ll1l_opy_ = QueueItem.__init__
+    bstack1111ll11_opy_ = pabot._create_command_for_execution
+  if bstack1l1l11l11_opy_ == bstack11_opy_ (u"ࠩࡥࡩ࡭ࡧࡶࡦࠩഷ"):
     try:
       from behave.runner import Runner
       from behave.model import Step
     except Exception as e:
-      bstack11l1_opy_(e, bstack1l111ll_opy_)
-    bstack1l1ll11ll_opy_ = Runner.run_hook
-    bstack1ll1111_opy_ = Step.run
-  if bstack1l1ll1lll_opy_ == bstack1ll1_opy_ (u"ࠫࡵࡿࡴࡦࡵࡷࠫഏ"):
+      bstack111lll1l_opy_(e, bstack111111ll_opy_)
+    bstack11l11ll1_opy_ = Runner.run_hook
+    bstack111l1ll_opy_ = Step.run
+  if bstack1l1l11l11_opy_ == bstack11_opy_ (u"ࠪࡴࡾࡺࡥࡴࡶࠪസ"):
     try:
       from _pytest.config import Config
     except Exception as e:
-      bstack11l1_opy_(e, bstack1lll11ll1_opy_)
-    bstack11ll1l1l_opy_ = Config.getoption
-  if bstack1l1ll1lll_opy_ == bstack1ll1_opy_ (u"ࠬࡶࡹࡵࡪࡲࡲࠬഐ"):
-    bstack1l1l1111l_opy_()
-    bstack1lll1l11l_opy_()
-    if bstack1ll1_opy_ (u"࠭ࡰ࡭ࡣࡷࡪࡴࡸ࡭ࡴࠩ഑") in CONFIG:
-      bstack1l1ll1l_opy_ = True
-      bstack1l1l1111_opy_ = []
-      for index, platform in enumerate(CONFIG[bstack1ll1_opy_ (u"ࠧࡱ࡮ࡤࡸ࡫ࡵࡲ࡮ࡵࠪഒ")]):
-        bstack1l1l1111_opy_.append(bstack11lll1ll_opy_(name=str(index),
-                                      target=bstack1l1ll11l1_opy_, args=(args[0], index)))
-      for t in bstack1l1l1111_opy_:
+      bstack111lll1l_opy_(e, bstack111lll_opy_)
+    bstack1l11lll11_opy_ = Config.getoption
+  if bstack1l1l11l11_opy_ == bstack11_opy_ (u"ࠫࡵࡿࡴࡩࡱࡱࠫഹ"):
+    bstack1lll11l1_opy_()
+    bstack1ll111ll1_opy_()
+    if bstack11_opy_ (u"ࠬࡶ࡬ࡢࡶࡩࡳࡷࡳࡳࠨഺ") in CONFIG:
+      bstack1l11llll_opy_ = True
+      bstack1llllll11_opy_ = []
+      for index, platform in enumerate(CONFIG[bstack11_opy_ (u"࠭ࡰ࡭ࡣࡷࡪࡴࡸ࡭ࡴ഻ࠩ")]):
+        bstack1llllll11_opy_.append(bstack11l1l1ll_opy_(name=str(index),
+                                      target=bstack1l11l11l1_opy_, args=(args[0], index)))
+      for t in bstack1llllll11_opy_:
         t.start()
-      for t in bstack1l1l1111_opy_:
+      for t in bstack1llllll11_opy_:
         t.join()
     else:
-      bstack111l111l_opy_(bstack1lllll111_opy_)
+      bstack1l111ll1_opy_(bstack111l1_opy_)
       exec(open(args[0]).read())
-  elif bstack1l1ll1lll_opy_ == bstack1ll1_opy_ (u"ࠨࡲࡤࡦࡴࡺࠧഓ") or bstack1l1ll1lll_opy_ == bstack1ll1_opy_ (u"ࠩࡵࡳࡧࡵࡴࠨഔ"):
+  elif bstack1l1l11l11_opy_ == bstack11_opy_ (u"ࠧࡱࡣࡥࡳࡹ഼࠭") or bstack1l1l11l11_opy_ == bstack11_opy_ (u"ࠨࡴࡲࡦࡴࡺࠧഽ"):
     try:
       from pabot import pabot
     except Exception as e:
-      bstack11l1_opy_(e, bstack1llll1ll1_opy_)
-    bstack1l1l1111l_opy_()
-    bstack111l111l_opy_(bstack1l1l1l_opy_)
-    if bstack1ll1_opy_ (u"ࠪ࠱࠲ࡶࡲࡰࡥࡨࡷࡸ࡫ࡳࠨക") in args:
-      i = args.index(bstack1ll1_opy_ (u"ࠫ࠲࠳ࡰࡳࡱࡦࡩࡸࡹࡥࡴࠩഖ"))
+      bstack111lll1l_opy_(e, bstack11l111ll_opy_)
+    bstack1lll11l1_opy_()
+    bstack1l111ll1_opy_(bstack1l111l111_opy_)
+    if bstack11_opy_ (u"ࠩ࠰࠱ࡵࡸ࡯ࡤࡧࡶࡷࡪࡹࠧാ") in args:
+      i = args.index(bstack11_opy_ (u"ࠪ࠱࠲ࡶࡲࡰࡥࡨࡷࡸ࡫ࡳࠨി"))
       args.pop(i)
       args.pop(i)
-    args.insert(0, str(bstack1llll1_opy_))
-    args.insert(0, str(bstack1ll1_opy_ (u"ࠬ࠳࠭ࡱࡴࡲࡧࡪࡹࡳࡦࡵࠪഗ")))
+    args.insert(0, str(bstack1l11ll1ll_opy_))
+    args.insert(0, str(bstack11_opy_ (u"ࠫ࠲࠳ࡰࡳࡱࡦࡩࡸࡹࡥࡴࠩീ")))
     pabot.main(args)
-  elif bstack1l1ll1lll_opy_ == bstack1ll1_opy_ (u"࠭ࡲࡰࡤࡲࡸ࠲࡯࡮ࡵࡧࡵࡲࡦࡲࠧഘ"):
+  elif bstack1l1l11l11_opy_ == bstack11_opy_ (u"ࠬࡸ࡯ࡣࡱࡷ࠱࡮ࡴࡴࡦࡴࡱࡥࡱ࠭ു"):
     try:
       from robot import run_cli
     except Exception as e:
-      bstack11l1_opy_(e, bstack1llll1ll1_opy_)
+      bstack111lll1l_opy_(e, bstack11l111ll_opy_)
     for a in args:
-      if bstack1ll1_opy_ (u"ࠧࡃࡕࡗࡅࡈࡑࡐࡍࡃࡗࡊࡔࡘࡍࡊࡐࡇࡉ࡝࠭ങ") in a:
-        bstack1111ll_opy_ = int(a.split(bstack1ll1_opy_ (u"ࠨ࠼ࠪച"))[1])
-      if bstack1ll1_opy_ (u"ࠩࡅࡗ࡙ࡇࡃࡌࡆࡈࡊࡑࡕࡃࡂࡎࡌࡈࡊࡔࡔࡊࡈࡌࡉࡗ࠭ഛ") in a:
-        bstack111l1lll_opy_ = str(a.split(bstack1ll1_opy_ (u"ࠪ࠾ࠬജ"))[1])
-      if bstack1ll1_opy_ (u"ࠫࡇ࡙ࡔࡂࡅࡎࡇࡑࡏࡁࡓࡉࡖࠫഝ") in a:
-        bstack11l1l11l_opy_ = str(a.split(bstack1ll1_opy_ (u"ࠬࡀࠧഞ"))[1])
-    bstack111l111l_opy_(bstack1l1l1l_opy_)
+      if bstack11_opy_ (u"࠭ࡂࡔࡖࡄࡇࡐࡖࡌࡂࡖࡉࡓࡗࡓࡉࡏࡆࡈ࡜ࠬൂ") in a:
+        bstack1l111l11l_opy_ = int(a.split(bstack11_opy_ (u"ࠧ࠻ࠩൃ"))[1])
+      if bstack11_opy_ (u"ࠨࡄࡖࡘࡆࡉࡋࡅࡇࡉࡐࡔࡉࡁࡍࡋࡇࡉࡓ࡚ࡉࡇࡋࡈࡖࠬൄ") in a:
+        bstack1l11l111_opy_ = str(a.split(bstack11_opy_ (u"ࠩ࠽ࠫ൅"))[1])
+      if bstack11_opy_ (u"ࠪࡆࡘ࡚ࡁࡄࡍࡆࡐࡎࡇࡒࡈࡕࠪെ") in a:
+        bstack11llll1l_opy_ = str(a.split(bstack11_opy_ (u"ࠫ࠿࠭േ"))[1])
+    bstack1l111ll1_opy_(bstack1l111l111_opy_)
     run_cli(args)
-  elif bstack1l1ll1lll_opy_ == bstack1ll1_opy_ (u"࠭ࡰࡺࡶࡨࡷࡹ࠭ട"):
+  elif bstack1l1l11l11_opy_ == bstack11_opy_ (u"ࠬࡶࡹࡵࡧࡶࡸࠬൈ"):
     try:
       from _pytest.config import _prepareconfig
       from _pytest.config import Config
       import importlib
-      bstack1ll1111l_opy_ = importlib.find_loader(bstack1ll1_opy_ (u"ࠧࡱࡻࡷࡩࡸࡺ࡟ࡴࡧ࡯ࡩࡳ࡯ࡵ࡮ࠩഠ"))
-      if bstack1ll1111l_opy_ is None:
-        bstack11l1_opy_(e, bstack1lll11ll1_opy_)
+      bstack11ll1ll_opy_ = importlib.find_loader(bstack11_opy_ (u"࠭ࡰࡺࡶࡨࡷࡹࡥࡳࡦ࡮ࡨࡲ࡮ࡻ࡭ࠨ൉"))
+      if bstack11ll1ll_opy_ is None:
+        bstack111lll1l_opy_(e, bstack111lll_opy_)
     except Exception as e:
-      bstack11l1_opy_(e, bstack1lll11ll1_opy_)
-    bstack1l1l1111l_opy_()
+      bstack111lll1l_opy_(e, bstack111lll_opy_)
+    bstack1lll11l1_opy_()
     try:
-      if bstack1ll1_opy_ (u"ࠨ࠯࠰ࡨࡷ࡯ࡶࡦࡴࠪഡ") in args:
-        i = args.index(bstack1ll1_opy_ (u"ࠩ࠰࠱ࡩࡸࡩࡷࡧࡵࠫഢ"))
+      if bstack11_opy_ (u"ࠧ࠮࠯ࡧࡶ࡮ࡼࡥࡳࠩൊ") in args:
+        i = args.index(bstack11_opy_ (u"ࠨ࠯࠰ࡨࡷ࡯ࡶࡦࡴࠪോ"))
         args.pop(i+1)
         args.pop(i)
-      if bstack1ll1_opy_ (u"ࠪ࠱࠲ࡶ࡬ࡶࡩ࡬ࡲࡸ࠭ണ") in args:
-        i = args.index(bstack1ll1_opy_ (u"ࠫ࠲࠳ࡰ࡭ࡷࡪ࡭ࡳࡹࠧത"))
+      if bstack11_opy_ (u"ࠩ࠰࠱ࡵࡲࡵࡨ࡫ࡱࡷࠬൌ") in args:
+        i = args.index(bstack11_opy_ (u"ࠪ࠱࠲ࡶ࡬ࡶࡩ࡬ࡲࡸ്࠭"))
         args.pop(i+1)
         args.pop(i)
-      if bstack1ll1_opy_ (u"ࠬ࠳ࡰࠨഥ") in args:
-        i = args.index(bstack1ll1_opy_ (u"࠭࠭ࡱࠩദ"))
+      if bstack11_opy_ (u"ࠫ࠲ࡶࠧൎ") in args:
+        i = args.index(bstack11_opy_ (u"ࠬ࠳ࡰࠨ൏"))
         args.pop(i+1)
         args.pop(i)
-      if bstack1ll1_opy_ (u"ࠧ࠮࠯ࡱࡹࡲࡶࡲࡰࡥࡨࡷࡸ࡫ࡳࠨധ") in args:
-        i = args.index(bstack1ll1_opy_ (u"ࠨ࠯࠰ࡲࡺࡳࡰࡳࡱࡦࡩࡸࡹࡥࡴࠩന"))
+      if bstack11_opy_ (u"࠭࠭࠮ࡰࡸࡱࡵࡸ࡯ࡤࡧࡶࡷࡪࡹࠧ൐") in args:
+        i = args.index(bstack11_opy_ (u"ࠧ࠮࠯ࡱࡹࡲࡶࡲࡰࡥࡨࡷࡸ࡫ࡳࠨ൑"))
         args.pop(i+1)
         args.pop(i)
-      if bstack1ll1_opy_ (u"ࠩ࠰ࡲࠬഩ") in args:
-        i = args.index(bstack1ll1_opy_ (u"ࠪ࠱ࡳ࠭പ"))
+      if bstack11_opy_ (u"ࠨ࠯ࡱࠫ൒") in args:
+        i = args.index(bstack11_opy_ (u"ࠩ࠰ࡲࠬ൓"))
         args.pop(i+1)
         args.pop(i)
     except Exception as exc:
       logger.error(str(exc))
     config = _prepareconfig(args)
-    bstack1l1ll11l_opy_ = config.args
-    bstack111l1l_opy_ = config.invocation_params.args
-    bstack111l1l_opy_ = list(bstack111l1l_opy_)
-    bstack1l1lll1l1_opy_ = []
-    for arg in bstack111l1l_opy_:
-      for spec in bstack1l1ll11l_opy_:
+    bstack1l1ll1ll_opy_ = config.args
+    bstack1l111ll11_opy_ = config.invocation_params.args
+    bstack1l111ll11_opy_ = list(bstack1l111ll11_opy_)
+    bstack1l1l1l1ll_opy_ = []
+    for arg in bstack1l111ll11_opy_:
+      for spec in bstack1l1ll1ll_opy_:
         if os.path.normpath(arg) != os.path.normpath(spec):
-          bstack1l1lll1l1_opy_.append(arg)
+          bstack1l1l1l1ll_opy_.append(arg)
     import platform as pf
-    if pf.system().lower() == bstack1ll1_opy_ (u"ࠫࡼ࡯࡮ࡥࡱࡺࡷࠬഫ"):
+    if pf.system().lower() == bstack11_opy_ (u"ࠪࡻ࡮ࡴࡤࡰࡹࡶࠫൔ"):
       from pathlib import PureWindowsPath, PurePosixPath
-      bstack1l1ll11l_opy_ = [str(PurePosixPath(PureWindowsPath(bstack11lll_opy_)))
-                    for bstack11lll_opy_ in bstack1l1ll11l_opy_]
-    bstack1l1lll1l1_opy_.append(bstack1ll1_opy_ (u"ࠬ࠳ࡰࠨബ"))
-    bstack1l1lll1l1_opy_.append(bstack1ll1_opy_ (u"࠭ࡰࡺࡶࡨࡷࡹࡥࡢࡳࡱࡺࡷࡪࡸࡳࡵࡣࡦ࡯ࡵࡲࡵࡨ࡫ࡱࠫഭ"))
-    bstack1l1lll1l1_opy_.append(bstack1ll1_opy_ (u"ࠧ࠮࠯ࡧࡶ࡮ࡼࡥࡳࠩമ"))
-    bstack1l1lll1l1_opy_.append(bstack1ll1_opy_ (u"ࠨࡥ࡫ࡶࡴࡳࡥࠨയ"))
-    bstack1lllll11l_opy_ = []
-    for spec in bstack1l1ll11l_opy_:
-      bstack111l11_opy_ = []
-      bstack111l11_opy_.append(spec)
-      bstack111l11_opy_ += bstack1l1lll1l1_opy_
-      bstack1lllll11l_opy_.append(bstack111l11_opy_)
-    bstack1l1ll1l_opy_ = True
-    bstack1l1l1lll1_opy_ = 1
-    if bstack1ll1_opy_ (u"ࠩࡳࡥࡷࡧ࡬࡭ࡧ࡯ࡷࡕ࡫ࡲࡑ࡮ࡤࡸ࡫ࡵࡲ࡮ࠩര") in CONFIG:
-      bstack1l1l1lll1_opy_ = CONFIG[bstack1ll1_opy_ (u"ࠪࡴࡦࡸࡡ࡭࡮ࡨࡰࡸࡖࡥࡳࡒ࡯ࡥࡹ࡬࡯ࡳ࡯ࠪറ")]
-    bstack11l1ll_opy_ = int(bstack1l1l1lll1_opy_)*int(len(CONFIG[bstack1ll1_opy_ (u"ࠫࡵࡲࡡࡵࡨࡲࡶࡲࡹࠧല")]))
+      bstack1l1ll1ll_opy_ = [str(PurePosixPath(PureWindowsPath(bstack11l11ll_opy_)))
+                    for bstack11l11ll_opy_ in bstack1l1ll1ll_opy_]
+    bstack1l1l1l1ll_opy_.append(bstack11_opy_ (u"ࠫ࠲ࡶࠧൕ"))
+    bstack1l1l1l1ll_opy_.append(bstack11_opy_ (u"ࠬࡶࡹࡵࡧࡶࡸࡤࡨࡲࡰࡹࡶࡩࡷࡹࡴࡢࡥ࡮ࡴࡱࡻࡧࡪࡰࠪൖ"))
+    bstack1l1l1l1ll_opy_.append(bstack11_opy_ (u"࠭࠭࠮ࡦࡵ࡭ࡻ࡫ࡲࠨൗ"))
+    bstack1l1l1l1ll_opy_.append(bstack11_opy_ (u"ࠧࡤࡪࡵࡳࡲ࡫ࠧ൘"))
+    bstack1l1ll111l_opy_ = []
+    for spec in bstack1l1ll1ll_opy_:
+      bstack111ll11l_opy_ = []
+      bstack111ll11l_opy_.append(spec)
+      bstack111ll11l_opy_ += bstack1l1l1l1ll_opy_
+      bstack1l1ll111l_opy_.append(bstack111ll11l_opy_)
+    bstack1l11llll_opy_ = True
+    bstack1l11l1l11_opy_ = 1
+    if bstack11_opy_ (u"ࠨࡲࡤࡶࡦࡲ࡬ࡦ࡮ࡶࡔࡪࡸࡐ࡭ࡣࡷࡪࡴࡸ࡭ࠨ൙") in CONFIG:
+      bstack1l11l1l11_opy_ = CONFIG[bstack11_opy_ (u"ࠩࡳࡥࡷࡧ࡬࡭ࡧ࡯ࡷࡕ࡫ࡲࡑ࡮ࡤࡸ࡫ࡵࡲ࡮ࠩ൚")]
+    bstack1ll11ll1_opy_ = int(bstack1l11l1l11_opy_)*int(len(CONFIG[bstack11_opy_ (u"ࠪࡴࡱࡧࡴࡧࡱࡵࡱࡸ࠭൛")]))
     execution_items = []
-    for index, _ in enumerate(CONFIG[bstack1ll1_opy_ (u"ࠬࡶ࡬ࡢࡶࡩࡳࡷࡳࡳࠨള")]):
-      for bstack111l11_opy_ in bstack1lllll11l_opy_:
+    for index, _ in enumerate(CONFIG[bstack11_opy_ (u"ࠫࡵࡲࡡࡵࡨࡲࡶࡲࡹࠧ൜")]):
+      for bstack111ll11l_opy_ in bstack1l1ll111l_opy_:
         item = {}
-        item[bstack1ll1_opy_ (u"࠭ࡡࡳࡩࠪഴ")] = bstack111l11_opy_
-        item[bstack1ll1_opy_ (u"ࠧࡪࡰࡧࡩࡽ࠭വ")] = index
+        item[bstack11_opy_ (u"ࠬࡧࡲࡨࠩ൝")] = bstack111ll11l_opy_
+        item[bstack11_opy_ (u"࠭ࡩ࡯ࡦࡨࡼࠬ൞")] = index
         execution_items.append(item)
-    bstack111111l1_opy_ = bstack11l1lll_opy_(execution_items, bstack11l1ll_opy_)
-    for execution_item in bstack111111l1_opy_:
-      bstack1l1l1111_opy_ = []
+    bstack1llll1l1l_opy_ = bstack1111ll1l_opy_(execution_items, bstack1ll11ll1_opy_)
+    for execution_item in bstack1llll1l1l_opy_:
+      bstack1llllll11_opy_ = []
       for item in execution_item:
-        bstack1l1l1111_opy_.append(bstack11lll1ll_opy_(name=str(item[bstack1ll1_opy_ (u"ࠨ࡫ࡱࡨࡪࡾࠧശ")]),
-                                            target=bstack1l11l1ll_opy_,
-                                            args=(item[bstack1ll1_opy_ (u"ࠩࡤࡶ࡬࠭ഷ")],)))
-      for t in bstack1l1l1111_opy_:
+        bstack1llllll11_opy_.append(bstack11l1l1ll_opy_(name=str(item[bstack11_opy_ (u"ࠧࡪࡰࡧࡩࡽ࠭ൟ")]),
+                                            target=bstack1111_opy_,
+                                            args=(item[bstack11_opy_ (u"ࠨࡣࡵ࡫ࠬൠ")],)))
+      for t in bstack1llllll11_opy_:
         t.start()
-      for t in bstack1l1l1111_opy_:
+      for t in bstack1llllll11_opy_:
         t.join()
-  elif bstack1l1ll1lll_opy_ == bstack1ll1_opy_ (u"ࠪࡦࡪ࡮ࡡࡷࡧࠪസ"):
+  elif bstack1l1l11l11_opy_ == bstack11_opy_ (u"ࠩࡥࡩ࡭ࡧࡶࡦࠩൡ"):
     try:
-      from behave.__main__ import main as bstack1111lll_opy_
+      from behave.__main__ import main as bstack1l1l1ll1_opy_
       from behave.configuration import Configuration
     except Exception as e:
-      bstack11l1_opy_(e, bstack1l111ll_opy_)
-    bstack1l1l1111l_opy_()
-    bstack1l1ll1l_opy_ = True
-    bstack1l1l1lll1_opy_ = 1
-    if bstack1ll1_opy_ (u"ࠫࡵࡧࡲࡢ࡮࡯ࡩࡱࡹࡐࡦࡴࡓࡰࡦࡺࡦࡰࡴࡰࠫഹ") in CONFIG:
-      bstack1l1l1lll1_opy_ = CONFIG[bstack1ll1_opy_ (u"ࠬࡶࡡࡳࡣ࡯ࡰࡪࡲࡳࡑࡧࡵࡔࡱࡧࡴࡧࡱࡵࡱࠬഺ")]
-    bstack11l1ll_opy_ = int(bstack1l1l1lll1_opy_)*int(len(CONFIG[bstack1ll1_opy_ (u"࠭ࡰ࡭ࡣࡷࡪࡴࡸ࡭ࡴ഻ࠩ")]))
+      bstack111lll1l_opy_(e, bstack111111ll_opy_)
+    bstack1lll11l1_opy_()
+    bstack1l11llll_opy_ = True
+    bstack1l11l1l11_opy_ = 1
+    if bstack11_opy_ (u"ࠪࡴࡦࡸࡡ࡭࡮ࡨࡰࡸࡖࡥࡳࡒ࡯ࡥࡹ࡬࡯ࡳ࡯ࠪൢ") in CONFIG:
+      bstack1l11l1l11_opy_ = CONFIG[bstack11_opy_ (u"ࠫࡵࡧࡲࡢ࡮࡯ࡩࡱࡹࡐࡦࡴࡓࡰࡦࡺࡦࡰࡴࡰࠫൣ")]
+    bstack1ll11ll1_opy_ = int(bstack1l11l1l11_opy_)*int(len(CONFIG[bstack11_opy_ (u"ࠬࡶ࡬ࡢࡶࡩࡳࡷࡳࡳࠨ൤")]))
     config = Configuration(args)
-    bstack1l1ll11l_opy_ = config.paths
-    bstack11l11l11_opy_ = []
+    bstack1l1ll1ll_opy_ = config.paths
+    bstack1ll11ll11_opy_ = []
     for arg in args:
-      if os.path.normpath(arg) not in bstack1l1ll11l_opy_:
-        bstack11l11l11_opy_.append(arg)
+      if os.path.normpath(arg) not in bstack1l1ll1ll_opy_:
+        bstack1ll11ll11_opy_.append(arg)
     import platform as pf
-    if pf.system().lower() == bstack1ll1_opy_ (u"ࠧࡸ࡫ࡱࡨࡴࡽࡳࠨ഼"):
+    if pf.system().lower() == bstack11_opy_ (u"࠭ࡷࡪࡰࡧࡳࡼࡹࠧ൥"):
       from pathlib import PureWindowsPath, PurePosixPath
-      bstack1l1ll11l_opy_ = [str(PurePosixPath(PureWindowsPath(bstack11lll_opy_)))
-                    for bstack11lll_opy_ in bstack1l1ll11l_opy_]
-    bstack1lllll11l_opy_ = []
-    for spec in bstack1l1ll11l_opy_:
-      bstack111l11_opy_ = []
-      bstack111l11_opy_ += bstack11l11l11_opy_
-      bstack111l11_opy_.append(spec)
-      bstack1lllll11l_opy_.append(bstack111l11_opy_)
+      bstack1l1ll1ll_opy_ = [str(PurePosixPath(PureWindowsPath(bstack11l11ll_opy_)))
+                    for bstack11l11ll_opy_ in bstack1l1ll1ll_opy_]
+    bstack1l1ll111l_opy_ = []
+    for spec in bstack1l1ll1ll_opy_:
+      bstack111ll11l_opy_ = []
+      bstack111ll11l_opy_ += bstack1ll11ll11_opy_
+      bstack111ll11l_opy_.append(spec)
+      bstack1l1ll111l_opy_.append(bstack111ll11l_opy_)
     execution_items = []
-    for index, _ in enumerate(CONFIG[bstack1ll1_opy_ (u"ࠨࡲ࡯ࡥࡹ࡬࡯ࡳ࡯ࡶࠫഽ")]):
-      for bstack111l11_opy_ in bstack1lllll11l_opy_:
+    for index, _ in enumerate(CONFIG[bstack11_opy_ (u"ࠧࡱ࡮ࡤࡸ࡫ࡵࡲ࡮ࡵࠪ൦")]):
+      for bstack111ll11l_opy_ in bstack1l1ll111l_opy_:
         item = {}
-        item[bstack1ll1_opy_ (u"ࠩࡤࡶ࡬࠭ാ")] = bstack1ll1_opy_ (u"ࠪࠤࠬി").join(bstack111l11_opy_)
-        item[bstack1ll1_opy_ (u"ࠫ࡮ࡴࡤࡦࡺࠪീ")] = index
+        item[bstack11_opy_ (u"ࠨࡣࡵ࡫ࠬ൧")] = bstack11_opy_ (u"ࠩࠣࠫ൨").join(bstack111ll11l_opy_)
+        item[bstack11_opy_ (u"ࠪ࡭ࡳࡪࡥࡹࠩ൩")] = index
         execution_items.append(item)
-    bstack111111l1_opy_ = bstack11l1lll_opy_(execution_items, bstack11l1ll_opy_)
-    for execution_item in bstack111111l1_opy_:
-      bstack1l1l1111_opy_ = []
+    bstack1llll1l1l_opy_ = bstack1111ll1l_opy_(execution_items, bstack1ll11ll1_opy_)
+    for execution_item in bstack1llll1l1l_opy_:
+      bstack1llllll11_opy_ = []
       for item in execution_item:
-        bstack1l1l1111_opy_.append(bstack11lll1ll_opy_(name=str(item[bstack1ll1_opy_ (u"ࠬ࡯࡮ࡥࡧࡻࠫു")]),
-                                            target=bstack1l1111l_opy_,
-                                            args=(item[bstack1ll1_opy_ (u"࠭ࡡࡳࡩࠪൂ")],)))
-      for t in bstack1l1l1111_opy_:
+        bstack1llllll11_opy_.append(bstack11l1l1ll_opy_(name=str(item[bstack11_opy_ (u"ࠫ࡮ࡴࡤࡦࡺࠪ൪")]),
+                                            target=bstack1ll11ll_opy_,
+                                            args=(item[bstack11_opy_ (u"ࠬࡧࡲࡨࠩ൫")],)))
+      for t in bstack1llllll11_opy_:
         t.start()
-      for t in bstack1l1l1111_opy_:
+      for t in bstack1llllll11_opy_:
         t.join()
   else:
-    bstack1ll1lll_opy_(bstack1111l1l1_opy_)
-  bstack1l1l11lll_opy_()
-def bstack1l1l11lll_opy_():
+    bstack11111l11_opy_(bstack111ll111_opy_)
+  bstack11111lll_opy_()
+def bstack11111lll_opy_():
   global CONFIG
   try:
-    if bstack1ll1_opy_ (u"ࠧࡣࡷ࡬ࡰࡩࡔࡡ࡮ࡧࠪൃ") in CONFIG:
-      host = bstack1ll1_opy_ (u"ࠨࡣࡳ࡭࠲ࡩ࡬ࡰࡷࡧࠫൄ") if bstack1ll1_opy_ (u"ࠩࡤࡴࡵ࠭൅") in CONFIG else bstack1ll1_opy_ (u"ࠪࡥࡵ࡯ࠧെ")
-      user = CONFIG[bstack1ll1_opy_ (u"ࠫࡺࡹࡥࡳࡐࡤࡱࡪ࠭േ")]
-      key = CONFIG[bstack1ll1_opy_ (u"ࠬࡧࡣࡤࡧࡶࡷࡐ࡫ࡹࠨൈ")]
-      bstack1l1ll1l11_opy_ = bstack1ll1_opy_ (u"࠭ࡡࡱࡲ࠰ࡥࡺࡺ࡯࡮ࡣࡷࡩࠬ൉") if bstack1ll1_opy_ (u"ࠧࡢࡲࡳࠫൊ") in CONFIG else bstack1ll1_opy_ (u"ࠨࡣࡸࡸࡴࡳࡡࡵࡧࠪോ")
-      url = bstack1ll1_opy_ (u"ࠩ࡫ࡸࡹࡶࡳ࠻࠱࠲ࡿࢂࡀࡻࡾࡂࡾࢁ࠳ࡨࡲࡰࡹࡶࡩࡷࡹࡴࡢࡥ࡮࠲ࡨࡵ࡭࠰ࡽࢀ࠳ࡧࡻࡩ࡭ࡦࡶ࠲࡯ࡹ࡯࡯ࠩൌ").format(user, key, host, bstack1l1ll1l11_opy_)
+    if bstack11_opy_ (u"࠭ࡢࡶ࡫࡯ࡨࡓࡧ࡭ࡦࠩ൬") in CONFIG:
+      host = bstack11_opy_ (u"ࠧࡢࡲ࡬࠱ࡨࡲ࡯ࡶࡦࠪ൭") if bstack11_opy_ (u"ࠨࡣࡳࡴࠬ൮") in CONFIG else bstack11_opy_ (u"ࠩࡤࡴ࡮࠭൯")
+      user = CONFIG[bstack11_opy_ (u"ࠪࡹࡸ࡫ࡲࡏࡣࡰࡩࠬ൰")]
+      key = CONFIG[bstack11_opy_ (u"ࠫࡦࡩࡣࡦࡵࡶࡏࡪࡿࠧ൱")]
+      bstack1l1l11l1l_opy_ = bstack11_opy_ (u"ࠬࡧࡰࡱ࠯ࡤࡹࡹࡵ࡭ࡢࡶࡨࠫ൲") if bstack11_opy_ (u"࠭ࡡࡱࡲࠪ൳") in CONFIG else bstack11_opy_ (u"ࠧࡢࡷࡷࡳࡲࡧࡴࡦࠩ൴")
+      url = bstack11_opy_ (u"ࠨࡪࡷࡸࡵࡹ࠺࠰࠱ࡾࢁ࠿ࢁࡽࡁࡽࢀ࠲ࡧࡸ࡯ࡸࡵࡨࡶࡸࡺࡡࡤ࡭࠱ࡧࡴࡳ࠯ࡼࡿ࠲ࡦࡺ࡯࡬ࡥࡵ࠱࡮ࡸࡵ࡮ࠨ൵").format(user, key, host, bstack1l1l11l1l_opy_)
       headers = {
-        bstack1ll1_opy_ (u"ࠪࡇࡴࡴࡴࡦࡰࡷ࠱ࡹࡿࡰࡦ്ࠩ"): bstack1ll1_opy_ (u"ࠫࡦࡶࡰ࡭࡫ࡦࡥࡹ࡯࡯࡯࠱࡭ࡷࡴࡴࠧൎ"),
+        bstack11_opy_ (u"ࠩࡆࡳࡳࡺࡥ࡯ࡶ࠰ࡸࡾࡶࡥࠨ൶"): bstack11_opy_ (u"ࠪࡥࡵࡶ࡬ࡪࡥࡤࡸ࡮ࡵ࡮࠰࡬ࡶࡳࡳ࠭൷"),
       }
-      if bstack1ll1_opy_ (u"ࠬࡨࡵࡪ࡮ࡧࡍࡩ࡫࡮ࡵ࡫ࡩ࡭ࡪࡸࠧ൏") in CONFIG:
-        params = {bstack1ll1_opy_ (u"࠭࡮ࡢ࡯ࡨࠫ൐"):CONFIG[bstack1ll1_opy_ (u"ࠧࡣࡷ࡬ࡰࡩࡔࡡ࡮ࡧࠪ൑")], bstack1ll1_opy_ (u"ࠨࡤࡸ࡭ࡱࡪ࡟ࡪࡦࡨࡲࡹ࡯ࡦࡪࡧࡵࠫ൒"):CONFIG[bstack1ll1_opy_ (u"ࠩࡥࡹ࡮ࡲࡤࡊࡦࡨࡲࡹ࡯ࡦࡪࡧࡵࠫ൓")]}
+      if bstack11_opy_ (u"ࠫࡧࡻࡩ࡭ࡦࡌࡨࡪࡴࡴࡪࡨ࡬ࡩࡷ࠭൸") in CONFIG:
+        params = {bstack11_opy_ (u"ࠬࡴࡡ࡮ࡧࠪ൹"):CONFIG[bstack11_opy_ (u"࠭ࡢࡶ࡫࡯ࡨࡓࡧ࡭ࡦࠩൺ")], bstack11_opy_ (u"ࠧࡣࡷ࡬ࡰࡩࡥࡩࡥࡧࡱࡸ࡮࡬ࡩࡦࡴࠪൻ"):CONFIG[bstack11_opy_ (u"ࠨࡤࡸ࡭ࡱࡪࡉࡥࡧࡱࡸ࡮࡬ࡩࡦࡴࠪർ")]}
       else:
-        params = {bstack1ll1_opy_ (u"ࠪࡲࡦࡳࡥࠨൔ"):CONFIG[bstack1ll1_opy_ (u"ࠫࡧࡻࡩ࡭ࡦࡑࡥࡲ࡫ࠧൕ")]}
+        params = {bstack11_opy_ (u"ࠩࡱࡥࡲ࡫ࠧൽ"):CONFIG[bstack11_opy_ (u"ࠪࡦࡺ࡯࡬ࡥࡐࡤࡱࡪ࠭ൾ")]}
       response = requests.get(url, params=params, headers=headers)
       if response.json():
-        bstack1ll1l1lll_opy_ = response.json()[0][bstack1ll1_opy_ (u"ࠬࡧࡵࡵࡱࡰࡥࡹ࡯࡯࡯ࡡࡥࡹ࡮ࡲࡤࠨൖ")]
-        if bstack1ll1l1lll_opy_:
-          bstack11ll11l1_opy_ = bstack1ll1l1lll_opy_[bstack1ll1_opy_ (u"࠭ࡰࡶࡤ࡯࡭ࡨࡥࡵࡳ࡮ࠪൗ")].split(bstack1ll1_opy_ (u"ࠧࡱࡷࡥࡰ࡮ࡩ࠭ࡣࡷ࡬ࡰࡩ࠭൘"))[0] + bstack1ll1_opy_ (u"ࠨࡤࡸ࡭ࡱࡪࡳ࠰ࠩ൙") + bstack1ll1l1lll_opy_[bstack1ll1_opy_ (u"ࠩ࡫ࡥࡸ࡮ࡥࡥࡡ࡬ࡨࠬ൚")]
-          logger.info(bstack1lll11_opy_.format(bstack11ll11l1_opy_))
-          bstack1lll111l1_opy_ = CONFIG[bstack1ll1_opy_ (u"ࠪࡦࡺ࡯࡬ࡥࡐࡤࡱࡪ࠭൛")]
-          if bstack1ll1_opy_ (u"ࠫࡧࡻࡩ࡭ࡦࡌࡨࡪࡴࡴࡪࡨ࡬ࡩࡷ࠭൜") in CONFIG:
-            bstack1lll111l1_opy_ += bstack1ll1_opy_ (u"ࠬࠦࠧ൝") + CONFIG[bstack1ll1_opy_ (u"࠭ࡢࡶ࡫࡯ࡨࡎࡪࡥ࡯ࡶ࡬ࡪ࡮࡫ࡲࠨ൞")]
-          if bstack1lll111l1_opy_!= bstack1ll1l1lll_opy_[bstack1ll1_opy_ (u"ࠧ࡯ࡣࡰࡩࠬൟ")]:
-            logger.debug(bstack1111_opy_.format(bstack1ll1l1lll_opy_[bstack1ll1_opy_ (u"ࠨࡰࡤࡱࡪ࠭ൠ")], bstack1lll111l1_opy_))
-    else:
-      logger.warn(bstack11ll1ll_opy_)
-  except Exception as e:
-    logger.debug(bstack11ll1l1_opy_.format(str(e)))
-def bstack1lll111_opy_(url, bstack1l1l111l_opy_=False):
-  global CONFIG
-  global bstack1l1ll_opy_
-  if not bstack1l1ll_opy_:
-    hostname = bstack1l11ll11_opy_(url)
-    is_private = bstack1ll11l11_opy_(hostname)
-    if (bstack1ll1_opy_ (u"ࠩࡥࡶࡴࡽࡳࡦࡴࡶࡸࡦࡩ࡫ࡍࡱࡦࡥࡱ࠭ൡ") in CONFIG and not CONFIG[bstack1ll1_opy_ (u"ࠪࡦࡷࡵࡷࡴࡧࡵࡷࡹࡧࡣ࡬ࡎࡲࡧࡦࡲࠧൢ")]) and (is_private or bstack1l1l111l_opy_):
-      bstack1l1ll_opy_ = hostname
-def bstack1l11ll11_opy_(url):
+        bstack1l11l1111_opy_ = response.json()[0][bstack11_opy_ (u"ࠫࡦࡻࡴࡰ࡯ࡤࡸ࡮ࡵ࡮ࡠࡤࡸ࡭ࡱࡪࠧൿ")]
+        if bstack1l11l1111_opy_:
+          bstack1ll1ll11l_opy_ = bstack1l11l1111_opy_[bstack11_opy_ (u"ࠬࡶࡵࡣ࡮࡬ࡧࡤࡻࡲ࡭ࠩ඀")].split(bstack11_opy_ (u"࠭ࡰࡶࡤ࡯࡭ࡨ࠳ࡢࡶ࡫࡯ࡨࠬඁ"))[0] + bstack11_opy_ (u"ࠧࡣࡷ࡬ࡰࡩࡹ࠯ࠨං") + bstack1l11l1111_opy_[bstack11_opy_ (u"ࠨࡪࡤࡷ࡭࡫ࡤࡠ࡫ࡧࠫඃ")]
+          logger.info(bstack11l11l_opy_.format(bstack1ll1ll11l_opy_))
+          bstack1ll1l1l11_opy_ = CONFIG[bstack11_opy_ (u"ࠩࡥࡹ࡮ࡲࡤࡏࡣࡰࡩࠬ඄")]
+          if bstack11_opy_ (u"ࠪࡦࡺ࡯࡬ࡥࡋࡧࡩࡳࡺࡩࡧ࡫ࡨࡶࠬඅ") in CONFIG:
+            bstack1ll1l1l11_opy_ += bstack11_opy_ (u"ࠫࠥ࠭ආ") + CONFIG[bstack11_opy_ (u"ࠬࡨࡵࡪ࡮ࡧࡍࡩ࡫࡮ࡵ࡫ࡩ࡭ࡪࡸࠧඇ")]
+          if bstack1ll1l1l11_opy_!= bstack1l11l1111_opy_[bstack11_opy_ (u"࠭࡮ࡢ࡯ࡨࠫඈ")]:
+            logger.debug(bstack111111l_opy_.format(bstack1l11l1111_opy_[bstack11_opy_ (u"ࠧ࡯ࡣࡰࡩࠬඉ")], bstack1ll1l1l11_opy_))
+    else:
+      logger.warn(bstack1l111lll1_opy_)
+  except Exception as e:
+    logger.debug(bstack1llll1_opy_.format(str(e)))
+def bstack1l1l1l11l_opy_(url, bstack11llll1_opy_=False):
+  global CONFIG
+  global bstack11l1l1_opy_
+  if not bstack11l1l1_opy_:
+    hostname = bstack111l111l_opy_(url)
+    is_private = bstack1l1ll1l1l_opy_(hostname)
+    if (bstack11_opy_ (u"ࠨࡤࡵࡳࡼࡹࡥࡳࡵࡷࡥࡨࡱࡌࡰࡥࡤࡰࠬඊ") in CONFIG and not CONFIG[bstack11_opy_ (u"ࠩࡥࡶࡴࡽࡳࡦࡴࡶࡸࡦࡩ࡫ࡍࡱࡦࡥࡱ࠭උ")]) and (is_private or bstack11llll1_opy_):
+      bstack11l1l1_opy_ = hostname
+def bstack111l111l_opy_(url):
   return urlparse(url).hostname
-def bstack1ll11l11_opy_(hostname):
-  for bstack1l1l11ll1_opy_ in bstack1lll111ll_opy_:
-    regex = re.compile(bstack1l1l11ll1_opy_)
+def bstack1l1ll1l1l_opy_(hostname):
+  for bstack11111l_opy_ in bstack1l1l11ll_opy_:
+    regex = re.compile(bstack11111l_opy_)
     if regex.match(hostname):
       return True
   return False
```

### Comparing `browserstack_sdk-1.8.1/browserstack_sdk/browserstack.framework.yml.sample` & `browserstack_sdk-1.9.2/browserstack_sdk/browserstack.framework.yml.sample`

 * *Files identical despite different names*

### Comparing `browserstack_sdk-1.8.1/browserstack_sdk/browserstack.generic.yml.sample` & `browserstack_sdk-1.9.2/browserstack_sdk/browserstack.generic.yml.sample`

 * *Files identical despite different names*

### Comparing `browserstack_sdk-1.8.1/browserstack_sdk.egg-info/PKG-INFO` & `browserstack_sdk-1.9.2/browserstack_sdk.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: browserstack-sdk
-Version: 1.8.1
+Version: 1.9.2
 Summary: Python SDK for browserstack selenium-webdriver tests
 Author: BrowserStack
 Author-email: support@browserstack.com
 License: BrowserStack Software License Agreement
         The “Licensed Software” under this BrowserStack Software License Agreement (“Agreement”) shall be used by
         you only if You agree to the following terms and conditions. Downloading the Licensed Software and indicating
         your consent to the terms of this license constitutes a binding Agreement between BrowserStack and You. If
```

### Comparing `browserstack_sdk-1.8.1/pytest_browserstackplugin/plugin.py` & `browserstack_sdk-1.9.2/pytest_browserstackplugin/plugin.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,133 +1,133 @@
 # coding: UTF-8
 import sys
-bstack11_opy_ = sys.version_info [0] == 2
-bstack1_opy_ = 2048
-bstack1l_opy_ = 7
-def bstack1l1_opy_ (bstack11ll_opy_):
-    global bstack11l_opy_
-    stringNr = ord (bstack11ll_opy_ [-1])
-    bstack1lll_opy_ = bstack11ll_opy_ [:-1]
-    bstack111l_opy_ = stringNr % len (bstack1lll_opy_)
-    bstack1111_opy_ = bstack1lll_opy_ [:bstack111l_opy_] + bstack1lll_opy_ [bstack111l_opy_:]
-    if bstack11_opy_:
-        bstack1ll_opy_ = unicode () .join ([unichr (ord (char) - bstack1_opy_ - (bstack1llll_opy_ + stringNr) % bstack1l_opy_) for bstack1llll_opy_, char in enumerate (bstack1111_opy_)])
+bstack11l_opy_ = sys.version_info [0] == 2
+bstack1l1_opy_ = 2048
+bstackl_opy_ = 7
+def bstack11ll_opy_ (bstack1_opy_):
+    global bstack1l11_opy_
+    stringNr = ord (bstack1_opy_ [-1])
+    bstack1lll1_opy_ = bstack1_opy_ [:-1]
+    bstack11_opy_ = stringNr % len (bstack1lll1_opy_)
+    bstack1ll1_opy_ = bstack1lll1_opy_ [:bstack11_opy_] + bstack1lll1_opy_ [bstack11_opy_:]
+    if bstack11l_opy_:
+        bstack1ll_opy_ = unicode () .join ([unichr (ord (char) - bstack1l1_opy_ - (bstack1111_opy_ + stringNr) % bstackl_opy_) for bstack1111_opy_, char in enumerate (bstack1ll1_opy_)])
     else:
-        bstack1ll_opy_ = str () .join ([chr (ord (char) - bstack1_opy_ - (bstack1llll_opy_ + stringNr) % bstack1l_opy_) for bstack1llll_opy_, char in enumerate (bstack1111_opy_)])
+        bstack1ll_opy_ = str () .join ([chr (ord (char) - bstack1l1_opy_ - (bstack1111_opy_ + stringNr) % bstackl_opy_) for bstack1111_opy_, char in enumerate (bstack1ll1_opy_)])
     return eval (bstack1ll_opy_)
 import pytest
 try:
     from playwright.sync_api import (
         BrowserContext,
         Page
     )
 except:
     pass
 import json
-def bstack1ll1_opy_(page, bstack11l1_opy_):
+def bstack1l1l_opy_(page, bstack1lll_opy_):
   try:
-    page.evaluate(bstack1l1_opy_ (u"ࠦࡤࠦ࠽࠿ࠢࡾࢁࠧࠀ"), bstack1l1_opy_ (u"ࠬࡨࡲࡰࡹࡶࡩࡷࡹࡴࡢࡥ࡮ࡣࡪࡾࡥࡤࡷࡷࡳࡷࡀࠠࡼࠤࡤࡧࡹ࡯࡯࡯ࠤ࠽ࠤࠧࡹࡥࡵࡕࡨࡷࡸ࡯࡯࡯ࡐࡤࡱࡪࠨࠬࠡࠤࡤࡶ࡬ࡻ࡭ࡦࡰࡷࡷࠧࡀࠠࡼࠤࡱࡥࡲ࡫ࠢ࠻ࠩࠁ")+ json.dumps(bstack11l1_opy_) + bstack1l1_opy_ (u"ࠨࡽࡾࠤࠂ"))
+    page.evaluate(bstack11ll_opy_ (u"ࠦࡤࠦ࠽࠿ࠢࡾࢁࠧࠀ"), bstack11ll_opy_ (u"ࠬࡨࡲࡰࡹࡶࡩࡷࡹࡴࡢࡥ࡮ࡣࡪࡾࡥࡤࡷࡷࡳࡷࡀࠠࡼࠤࡤࡧࡹ࡯࡯࡯ࠤ࠽ࠤࠧࡹࡥࡵࡕࡨࡷࡸ࡯࡯࡯ࡐࡤࡱࡪࠨࠬࠡࠤࡤࡶ࡬ࡻ࡭ࡦࡰࡷࡷࠧࡀࠠࡼࠤࡱࡥࡲ࡫ࠢ࠻ࠩࠁ")+ json.dumps(bstack1lll_opy_) + bstack11ll_opy_ (u"ࠨࡽࡾࠤࠂ"))
   except Exception as e:
-    print(bstack1l1_opy_ (u"ࠢࡦࡺࡦࡩࡵࡺࡩࡰࡰࠣ࡭ࡳࠦࡰ࡭ࡣࡼࡻࡷ࡯ࡧࡩࡶࠣࡷࡪࡹࡳࡪࡱࡱࠤࡳࡧ࡭ࡦࠢࡾࢁࠧࠃ"), e)
-def bstack111_opy_(page, message, level):
+    print(bstack11ll_opy_ (u"ࠢࡦࡺࡦࡩࡵࡺࡩࡰࡰࠣ࡭ࡳࠦࡰ࡭ࡣࡼࡻࡷ࡯ࡧࡩࡶࠣࡷࡪࡹࡳࡪࡱࡱࠤࡳࡧ࡭ࡦࠢࡾࢁࠧࠃ"), e)
+def bstack111l_opy_(page, message, level):
   try:
-    page.evaluate(bstack1l1_opy_ (u"ࠣࡡࠣࡁࡃࠦࡻࡾࠤࠄ"), bstack1l1_opy_ (u"ࠩࡥࡶࡴࡽࡳࡦࡴࡶࡸࡦࡩ࡫ࡠࡧࡻࡩࡨࡻࡴࡰࡴ࠽ࠤࢀࠨࡡࡤࡶ࡬ࡳࡳࠨ࠺ࠡࠤࡤࡲࡳࡵࡴࡢࡶࡨࠦ࠱ࠦࠢࡢࡴࡪࡹࡲ࡫࡮ࡵࡵࠥ࠾ࠥࢁࠢࡥࡣࡷࡥࠧࡀࠧࠅ") + json.dumps(message) + bstack1l1_opy_ (u"ࠪ࠰ࠧࡲࡥࡷࡧ࡯ࠦ࠿࠭ࠆ") + json.dumps(level) + bstack1l1_opy_ (u"ࠫࢂࢃࠧࠇ"))
+    page.evaluate(bstack11ll_opy_ (u"ࠣࡡࠣࡁࡃࠦࡻࡾࠤࠄ"), bstack11ll_opy_ (u"ࠩࡥࡶࡴࡽࡳࡦࡴࡶࡸࡦࡩ࡫ࡠࡧࡻࡩࡨࡻࡴࡰࡴ࠽ࠤࢀࠨࡡࡤࡶ࡬ࡳࡳࠨ࠺ࠡࠤࡤࡲࡳࡵࡴࡢࡶࡨࠦ࠱ࠦࠢࡢࡴࡪࡹࡲ࡫࡮ࡵࡵࠥ࠾ࠥࢁࠢࡥࡣࡷࡥࠧࡀࠧࠅ") + json.dumps(message) + bstack11ll_opy_ (u"ࠪ࠰ࠧࡲࡥࡷࡧ࡯ࠦ࠿࠭ࠆ") + json.dumps(level) + bstack11ll_opy_ (u"ࠫࢂࢃࠧࠇ"))
   except Exception as e:
-    print(bstack1l1_opy_ (u"ࠧ࡫ࡸࡤࡧࡳࡸ࡮ࡵ࡮ࠡ࡫ࡱࠤࡵࡲࡡࡺࡹࡵ࡭࡬࡮ࡴࠡࡣࡱࡲࡴࡺࡡࡵ࡫ࡲࡲࠥࢁࡽࠣࠈ"), e)
-def bstackl_opy_(page, status, message = bstack1l1_opy_ (u"ࠨࠢࠉ")):
+    print(bstack11ll_opy_ (u"ࠧ࡫ࡸࡤࡧࡳࡸ࡮ࡵ࡮ࠡ࡫ࡱࠤࡵࡲࡡࡺࡹࡵ࡭࡬࡮ࡴࠡࡣࡱࡲࡴࡺࡡࡵ࡫ࡲࡲࠥࢁࡽࠣࠈ"), e)
+def bstack111_opy_(page, status, message = bstack11ll_opy_ (u"ࠨࠢࠉ")):
   try:
-    if(status == bstack1l1_opy_ (u"ࠢࡧࡣ࡬ࡰࡪࡪࠢࠊ")):
-      page.evaluate(bstack1l1_opy_ (u"ࠣࡡࠣࡁࡃࠦࡻࡾࠤࠋ"), bstack1l1_opy_ (u"ࠩࡥࡶࡴࡽࡳࡦࡴࡶࡸࡦࡩ࡫ࡠࡧࡻࡩࡨࡻࡴࡰࡴ࠽ࠤࢀࠨࡡࡤࡶ࡬ࡳࡳࠨ࠺ࠡࠤࡶࡩࡹ࡙ࡥࡴࡵ࡬ࡳࡳ࡙ࡴࡢࡶࡸࡷࠧ࠲ࠠࠣࡣࡵ࡫ࡺࡳࡥ࡯ࡶࡶࠦ࠿ࠦࡻࠣࡴࡨࡥࡸࡵ࡮ࠣ࠼ࠪࠌ") + json.dumps(bstack1l1_opy_ (u"ࠥࡗࡨ࡫࡮ࡢࡴ࡬ࡳࠥ࡬ࡡࡪ࡮ࡨࡨࠥࡽࡩࡵࡪ࠽ࠤࠧࠍ") + str(message)) + bstack1l1_opy_ (u"ࠫ࠱ࠨࡳࡵࡣࡷࡹࡸࠨ࠺ࠨࠎ") + json.dumps(status) + bstack1l1_opy_ (u"ࠧࢃࡽࠣࠏ"))
+    if(status == bstack11ll_opy_ (u"ࠢࡧࡣ࡬ࡰࡪࡪࠢࠊ")):
+      page.evaluate(bstack11ll_opy_ (u"ࠣࡡࠣࡁࡃࠦࡻࡾࠤࠋ"), bstack11ll_opy_ (u"ࠩࡥࡶࡴࡽࡳࡦࡴࡶࡸࡦࡩ࡫ࡠࡧࡻࡩࡨࡻࡴࡰࡴ࠽ࠤࢀࠨࡡࡤࡶ࡬ࡳࡳࠨ࠺ࠡࠤࡶࡩࡹ࡙ࡥࡴࡵ࡬ࡳࡳ࡙ࡴࡢࡶࡸࡷࠧ࠲ࠠࠣࡣࡵ࡫ࡺࡳࡥ࡯ࡶࡶࠦ࠿ࠦࡻࠣࡴࡨࡥࡸࡵ࡮ࠣ࠼ࠪࠌ") + json.dumps(bstack11ll_opy_ (u"ࠥࡗࡨ࡫࡮ࡢࡴ࡬ࡳࠥ࡬ࡡࡪ࡮ࡨࡨࠥࡽࡩࡵࡪ࠽ࠤࠧࠍ") + str(message)) + bstack11ll_opy_ (u"ࠫ࠱ࠨࡳࡵࡣࡷࡹࡸࠨ࠺ࠨࠎ") + json.dumps(status) + bstack11ll_opy_ (u"ࠧࢃࡽࠣࠏ"))
     else:
-      page.evaluate(bstack1l1_opy_ (u"ࠨ࡟ࠡ࠿ࡁࠤࢀࢃࠢࠐ"), bstack1l1_opy_ (u"ࠧࡣࡴࡲࡻࡸ࡫ࡲࡴࡶࡤࡧࡰࡥࡥࡹࡧࡦࡹࡹࡵࡲ࠻ࠢࡾࠦࡦࡩࡴࡪࡱࡱࠦ࠿ࠦࠢࡴࡧࡷࡗࡪࡹࡳࡪࡱࡱࡗࡹࡧࡴࡶࡵࠥ࠰ࠥࠨࡡࡳࡩࡸࡱࡪࡴࡴࡴࠤ࠽ࠤࢀࠨࡳࡵࡣࡷࡹࡸࠨ࠺ࠨࠑ") + json.dumps(status) + bstack1l1_opy_ (u"ࠣࡿࢀࠦࠒ"))
+      page.evaluate(bstack11ll_opy_ (u"ࠨ࡟ࠡ࠿ࡁࠤࢀࢃࠢࠐ"), bstack11ll_opy_ (u"ࠧࡣࡴࡲࡻࡸ࡫ࡲࡴࡶࡤࡧࡰࡥࡥࡹࡧࡦࡹࡹࡵࡲ࠻ࠢࡾࠦࡦࡩࡴࡪࡱࡱࠦ࠿ࠦࠢࡴࡧࡷࡗࡪࡹࡳࡪࡱࡱࡗࡹࡧࡴࡶࡵࠥ࠰ࠥࠨࡡࡳࡩࡸࡱࡪࡴࡴࡴࠤ࠽ࠤࢀࠨࡳࡵࡣࡷࡹࡸࠨ࠺ࠨࠑ") + json.dumps(status) + bstack11ll_opy_ (u"ࠣࡿࢀࠦࠒ"))
   except Exception as e:
-    print(bstack1l1_opy_ (u"ࠤࡨࡼࡨ࡫ࡰࡵ࡫ࡲࡲࠥ࡯࡮ࠡࡲ࡯ࡥࡾࡽࡲࡪࡩ࡫ࡸࠥࡹࡥࡵࠢࡶࡩࡸࡹࡩࡰࡰࠣࡷࡹࡧࡴࡶࡵࠣࡿࢂࠨࠓ"), e)
+    print(bstack11ll_opy_ (u"ࠤࡨࡼࡨ࡫ࡰࡵ࡫ࡲࡲࠥ࡯࡮ࠡࡲ࡯ࡥࡾࡽࡲࡪࡩ࡫ࡸࠥࡹࡥࡵࠢࡶࡩࡸࡹࡩࡰࡰࠣࡷࡹࡧࡴࡶࡵࠣࡿࢂࠨࠓ"), e)
 @pytest.mark.hookwrapper
 def pytest_runtest_makereport(item, call):
     outcome = yield
-    plugins = item.config.getoption(bstack1l1_opy_ (u"ࠥࡴࡱࡻࡧࡪࡰࡶࠦࠔ"))
-    if(bstack1l1_opy_ (u"ࠦࡵࡿࡴࡦࡵࡷࡣࡧࡸ࡯ࡸࡵࡨࡶࡸࡺࡡࡤ࡭ࡳࡰࡺ࡭ࡩ࡯ࠤࠕ") not in plugins):
+    plugins = item.config.getoption(bstack11ll_opy_ (u"ࠥࡴࡱࡻࡧࡪࡰࡶࠦࠔ"))
+    if(bstack11ll_opy_ (u"ࠦࡵࡿࡴࡦࡵࡷࡣࡧࡸ࡯ࡸࡵࡨࡶࡸࡺࡡࡤ࡭ࡳࡰࡺ࡭ࡩ࡯ࠤࠕ") not in plugins):
         return
     report = outcome.get_result()
     summary = []
-    driver = getattr(item, bstack1l1_opy_ (u"ࠧࡥࡤࡳ࡫ࡹࡩࡷࠨࠖ"), None)
-    page = getattr(item, bstack1l1_opy_ (u"ࠨ࡟ࡱࡣࡪࡩࠧࠗ"), None)
+    driver = getattr(item, bstack11ll_opy_ (u"ࠧࡥࡤࡳ࡫ࡹࡩࡷࠨࠖ"), None)
+    page = getattr(item, bstack11ll_opy_ (u"ࠨ࡟ࡱࡣࡪࡩࠧࠗ"), None)
     if(driver is not None):
-        bstack1l1l_opy_(item, report, summary)
+        bstack1l_opy_(item, report, summary)
     if(page is not None):
-        bstack1l11_opy_(item, report, summary)
-def bstack1l1l_opy_(item, report, summary):
-    if report.when in [bstack1l1_opy_ (u"ࠢࡴࡧࡷࡹࡵࠨ࠘"), bstack1l1_opy_ (u"ࠣࡶࡨࡥࡷࡪ࡯ࡸࡰࠥ࠙")]:
+        bstack11l1_opy_(item, report, summary)
+def bstack1l_opy_(item, report, summary):
+    if report.when in [bstack11ll_opy_ (u"ࠢࡴࡧࡷࡹࡵࠨ࠘"), bstack11ll_opy_ (u"ࠣࡶࡨࡥࡷࡪ࡯ࡸࡰࠥ࠙")]:
             return
-    item._driver.execute_script(bstack1l1_opy_ (u"ࠩࡥࡶࡴࡽࡳࡦࡴࡶࡸࡦࡩ࡫ࡠࡧࡻࡩࡨࡻࡴࡰࡴ࠽ࠤࢀࠨࡡࡤࡶ࡬ࡳࡳࠨ࠺ࠡࠤࡶࡩࡹ࡙ࡥࡴࡵ࡬ࡳࡳࡔࡡ࡮ࡧࠥ࠰ࠥࠨࡡࡳࡩࡸࡱࡪࡴࡴࡴࠤ࠽ࠤࢀࠨ࡮ࡢ࡯ࡨࠦ࠿ࠦࠧࠚ") + json.dumps(report.nodeid) + bstack1l1_opy_ (u"ࠪࢁࢂ࠭ࠛ"))
-    passed = report.passed or (report.failed and hasattr(report, bstack1l1_opy_ (u"ࠦࡼࡧࡳࡹࡨࡤ࡭ࡱࠨࠜ")))
-    bstack1lll1_opy_ = bstack1l1_opy_ (u"ࠧࠨࠝ")
+    item._driver.execute_script(bstack11ll_opy_ (u"ࠩࡥࡶࡴࡽࡳࡦࡴࡶࡸࡦࡩ࡫ࡠࡧࡻࡩࡨࡻࡴࡰࡴ࠽ࠤࢀࠨࡡࡤࡶ࡬ࡳࡳࠨ࠺ࠡࠤࡶࡩࡹ࡙ࡥࡴࡵ࡬ࡳࡳࡔࡡ࡮ࡧࠥ࠰ࠥࠨࡡࡳࡩࡸࡱࡪࡴࡴࡴࠤ࠽ࠤࢀࠨ࡮ࡢ࡯ࡨࠦ࠿ࠦࠧࠚ") + json.dumps(report.nodeid) + bstack11ll_opy_ (u"ࠪࢁࢂ࠭ࠛ"))
+    passed = report.passed or (report.failed and hasattr(report, bstack11ll_opy_ (u"ࠦࡼࡧࡳࡹࡨࡤ࡭ࡱࠨࠜ")))
+    bstack1llll_opy_ = bstack11ll_opy_ (u"ࠧࠨࠝ")
     if not passed:
         try:
-            bstack1lll1_opy_ = report.longrepr.reprcrash
+            bstack1llll_opy_ = report.longrepr.reprcrash
         except Exception as e:
             summary.append(
-                bstack1l1_opy_ (u"ࠨࡗࡂࡔࡑࡍࡓࡍ࠺ࠡࡈࡤ࡭ࡱ࡫ࡤࠡࡶࡲࠤࡩ࡫ࡴࡦࡴࡰ࡭ࡳ࡫ࠠࡧࡣ࡬ࡰࡺࡸࡥࠡࡴࡨࡥࡸࡵ࡮࠻ࠢࡾ࠴ࢂࠨࠞ").format(e)
+                bstack11ll_opy_ (u"ࠨࡗࡂࡔࡑࡍࡓࡍ࠺ࠡࡈࡤ࡭ࡱ࡫ࡤࠡࡶࡲࠤࡩ࡫ࡴࡦࡴࡰ࡭ࡳ࡫ࠠࡧࡣ࡬ࡰࡺࡸࡥࠡࡴࡨࡥࡸࡵ࡮࠻ࠢࡾ࠴ࢂࠨࠞ").format(e)
             )
     try:
         if passed:
             item._driver.execute_script(
-                bstack1l1_opy_ (u"ࠧࡣࡴࡲࡻࡸ࡫ࡲࡴࡶࡤࡧࡰࡥࡥࡹࡧࡦࡹࡹࡵࡲ࠻ࠢࡾࠤࡡࠐࠠࠡࠢࠣࠤࠥࠦࠠࠡࠢࠣࠤࠥࠦࠠࠡࠢࠣࠤࠥࠨࡡࡤࡶ࡬ࡳࡳࠨ࠺ࠡࠤࡶࡩࡹ࡙ࡥࡴࡵ࡬ࡳࡳ࡙ࡴࡢࡶࡸࡷࠧ࠲ࠠ࡝ࠌࠣࠤࠥࠦࠠࠡࠢࠣࠤࠥࠦࠠࠡࠢࠣࠤࠥࠦࠠࠡࠤࡤࡶ࡬ࡻ࡭ࡦࡰࡷࡷࠧࡀࠠࡼࠢࠥࡷࡹࡧࡴࡶࡵࠥ࠾ࠧࡶࡡࡴࡵࡨࡨࠧࠦࡽࠡ࡞ࠍࠤࠥࠦࠠࠡࠢࠣࠤࠥࠦࠠࠡࠢࠣࠤࠥࢃࠧࠟ")
+                bstack11ll_opy_ (u"ࠧࡣࡴࡲࡻࡸ࡫ࡲࡴࡶࡤࡧࡰࡥࡥࡹࡧࡦࡹࡹࡵࡲ࠻ࠢࡾࠤࡡࠐࠠࠡࠢࠣࠤࠥࠦࠠࠡࠢࠣࠤࠥࠦࠠࠡࠢࠣࠤࠥࠨࡡࡤࡶ࡬ࡳࡳࠨ࠺ࠡࠤࡶࡩࡹ࡙ࡥࡴࡵ࡬ࡳࡳ࡙ࡴࡢࡶࡸࡷࠧ࠲ࠠ࡝ࠌࠣࠤࠥࠦࠠࠡࠢࠣࠤࠥࠦࠠࠡࠢࠣࠤࠥࠦࠠࠡࠤࡤࡶ࡬ࡻ࡭ࡦࡰࡷࡷࠧࡀࠠࡼࠢࠥࡷࡹࡧࡴࡶࡵࠥ࠾ࠧࡶࡡࡴࡵࡨࡨࠧࠦࡽࠡ࡞ࠍࠤࠥࠦࠠࠡࠢࠣࠤࠥࠦࠠࠡࠢࠣࠤࠥࢃࠧࠟ")
             )
         else:
-            if bstack1lll1_opy_:
+            if bstack1llll_opy_:
                 item._driver.execute_script(
-                    bstack1l1_opy_ (u"ࠨࡤࡵࡳࡼࡹࡥࡳࡵࡷࡥࡨࡱ࡟ࡦࡺࡨࡧࡺࡺ࡯ࡳ࠼ࠣࡿࡡࠐࠠࠡࠢࠣࠤࠥࠦࠠࠡࠢࠣࠤࠥࠦࠠࠡࠢࠣࠤࠥࠦࠠࠡࠢࠥࡥࡨࡺࡩࡰࡰࠥ࠾ࠥࠨࡡ࡯ࡰࡲࡸࡦࡺࡥࠣ࠮ࠣࡠࠏࠦࠠࠡࠢࠣࠤࠥࠦࠠࠡࠢࠣࠤࠥࠦࠠࠡࠢࠣࠤࠥࠦࠠࠡࠤࡤࡶ࡬ࡻ࡭ࡦࡰࡷࡷࠧࡀࠠࡼ࡞ࠍࠤࠥࠦࠠࠡࠢࠣࠤࠥࠦࠠࠡࠢࠣࠤࠥࠦࠠࠡࠢࠣࠤࠥࠦࠠࠡࠢࠣࠦࡱ࡫ࡶࡦ࡮ࠥ࠾ࠥࠨࡥࡳࡴࡲࡶࠧ࠲ࠠ࡝ࠌࠣࠤࠥࠦࠠࠡࠢࠣࠤࠥࠦࠠࠡࠢࠣࠤࠥࠦࠠࠡࠢࠣࠤࠥࠦࠠࠡࠢࠥࡨࡦࡺࡡࠣ࠼ࠣࠫࠠ")
-                    + json.dumps(str(bstack1lll1_opy_))
-                    + bstack1l1_opy_ (u"ࠤ࡟ࠎࠥࠦࠠࠡࠢࠣࠤࠥࠦࠠࠡࠢࠣࠤࠥࠦࠠࠡࠢࠣࠤࠥࠦࠠࡾ࡞ࠍࠤࠥࠦࠠࠡࠢࠣࠤࠥࠦࠠࠡࠢࠣࠤࠥࠦࠠࠡࠢࢀࠦࠡ")
+                    bstack11ll_opy_ (u"ࠨࡤࡵࡳࡼࡹࡥࡳࡵࡷࡥࡨࡱ࡟ࡦࡺࡨࡧࡺࡺ࡯ࡳ࠼ࠣࡿࡡࠐࠠࠡࠢࠣࠤࠥࠦࠠࠡࠢࠣࠤࠥࠦࠠࠡࠢࠣࠤࠥࠦࠠࠡࠢࠥࡥࡨࡺࡩࡰࡰࠥ࠾ࠥࠨࡡ࡯ࡰࡲࡸࡦࡺࡥࠣ࠮ࠣࡠࠏࠦࠠࠡࠢࠣࠤࠥࠦࠠࠡࠢࠣࠤࠥࠦࠠࠡࠢࠣࠤࠥࠦࠠࠡࠤࡤࡶ࡬ࡻ࡭ࡦࡰࡷࡷࠧࡀࠠࡼ࡞ࠍࠤࠥࠦࠠࠡࠢࠣࠤࠥࠦࠠࠡࠢࠣࠤࠥࠦࠠࠡࠢࠣࠤࠥࠦࠠࠡࠢࠣࠦࡱ࡫ࡶࡦ࡮ࠥ࠾ࠥࠨࡥࡳࡴࡲࡶࠧ࠲ࠠ࡝ࠌࠣࠤࠥࠦࠠࠡࠢࠣࠤࠥࠦࠠࠡࠢࠣࠤࠥࠦࠠࠡࠢࠣࠤࠥࠦࠠࠡࠢࠥࡨࡦࡺࡡࠣ࠼ࠣࠫࠠ")
+                    + json.dumps(str(bstack1llll_opy_))
+                    + bstack11ll_opy_ (u"ࠤ࡟ࠎࠥࠦࠠࠡࠢࠣࠤࠥࠦࠠࠡࠢࠣࠤࠥࠦࠠࠡࠢࠣࠤࠥࠦࠠࡾ࡞ࠍࠤࠥࠦࠠࠡࠢࠣࠤࠥࠦࠠࠡࠢࠣࠤࠥࠦࠠࠡࠢࢀࠦࠡ")
                 )
                 item._driver.execute_script(
-                    bstack1l1_opy_ (u"ࠪࡦࡷࡵࡷࡴࡧࡵࡷࡹࡧࡣ࡬ࡡࡨࡼࡪࡩࡵࡵࡱࡵ࠾ࠥࢁ࡜ࠋࠢࠣࠤࠥࠦࠠࠡࠢࠣࠤࠥࠦࠠࠡࠢࠣࠤࠥࠦࠠࠡࠢࠣࠤࠧࡧࡣࡵ࡫ࡲࡲࠧࡀࠠࠣࡵࡨࡸࡘ࡫ࡳࡴ࡫ࡲࡲࡘࡺࡡࡵࡷࡶࠦ࠱ࠦ࡜ࠋࠢࠣࠤࠥࠦࠠࠡࠢࠣࠤࠥࠦࠠࠡࠢࠣࠤࠥࠦࠠࠡࠢࠣࠤࠧࡧࡲࡨࡷࡰࡩࡳࡺࡳࠣ࠼ࠣࡿࡡࠐࠠࠡࠢࠣࠤࠥࠦࠠࠡࠢࠣࠤࠥࠦࠠࠡࠢࠣࠤࠥࠦࠠࠡࠢࠣࠤࠥࠦࠢࡴࡶࡤࡸࡺࡹࠢ࠻ࠢࠥࡪࡦ࡯࡬ࡦࡦࠥ࠰ࠥࡢࠊࠡࠢࠣࠤࠥࠦࠠࠡࠢࠣࠤࠥࠦࠠࠡࠢࠣࠤࠥࠦࠠࠡࠢࠣࠤࠥࠦࠠࠣࡴࡨࡥࡸࡵ࡮ࠣ࠼ࠣࠫࠢ")
-                    + json.dumps(str(bstack1lll1_opy_))
-                    + bstack1l1_opy_ (u"ࠦࡡࠐࠠࠡࠢࠣࠤࠥࠦࠠࠡࠢࠣࠤࠥࠦࠠࠡࠢࠣࠤࠥࠦࠠࠡࠢࢀࡠࠏࠦࠠࠡࠢࠣࠤࠥࠦࠠࠡࠢࠣࠤࠥࠦࠠࠡࠢࠣࠤࢂࠨࠣ")
+                    bstack11ll_opy_ (u"ࠪࡦࡷࡵࡷࡴࡧࡵࡷࡹࡧࡣ࡬ࡡࡨࡼࡪࡩࡵࡵࡱࡵ࠾ࠥࢁ࡜ࠋࠢࠣࠤࠥࠦࠠࠡࠢࠣࠤࠥࠦࠠࠡࠢࠣࠤࠥࠦࠠࠡࠢࠣࠤࠧࡧࡣࡵ࡫ࡲࡲࠧࡀࠠࠣࡵࡨࡸࡘ࡫ࡳࡴ࡫ࡲࡲࡘࡺࡡࡵࡷࡶࠦ࠱ࠦ࡜ࠋࠢࠣࠤࠥࠦࠠࠡࠢࠣࠤࠥࠦࠠࠡࠢࠣࠤࠥࠦࠠࠡࠢࠣࠤࠧࡧࡲࡨࡷࡰࡩࡳࡺࡳࠣ࠼ࠣࡿࡡࠐࠠࠡࠢࠣࠤࠥࠦࠠࠡࠢࠣࠤࠥࠦࠠࠡࠢࠣࠤࠥࠦࠠࠡࠢࠣࠤࠥࠦࠢࡴࡶࡤࡸࡺࡹࠢ࠻ࠢࠥࡪࡦ࡯࡬ࡦࡦࠥ࠰ࠥࡢࠊࠡࠢࠣࠤࠥࠦࠠࠡࠢࠣࠤࠥࠦࠠࠡࠢࠣࠤࠥࠦࠠࠡࠢࠣࠤࠥࠦࠠࠣࡴࡨࡥࡸࡵ࡮ࠣ࠼ࠣࠫࠢ")
+                    + json.dumps(str(bstack1llll_opy_))
+                    + bstack11ll_opy_ (u"ࠦࡡࠐࠠࠡࠢࠣࠤࠥࠦࠠࠡࠢࠣࠤࠥࠦࠠࠡࠢࠣࠤࠥࠦࠠࠡࠢࢀࡠࠏࠦࠠࠡࠢࠣࠤࠥࠦࠠࠡࠢࠣࠤࠥࠦࠠࠡࠢࠣࠤࢂࠨࠣ")
                 )
             else:
                 item._driver.execute_script(
-                    bstack1l1_opy_ (u"ࠬࡨࡲࡰࡹࡶࡩࡷࡹࡴࡢࡥ࡮ࡣࡪࡾࡥࡤࡷࡷࡳࡷࡀࠠࡼࠢ࡟ࠎࠥࠦࠠࠡࠢࠣࠤࠥࠦࠠࠡࠢࠣࠤࠥࠦࠠࠡࠢࠣࠤࠥࠦࠠࠣࡣࡦࡸ࡮ࡵ࡮ࠣ࠼ࠣࠦࡸ࡫ࡴࡔࡧࡶࡷ࡮ࡵ࡮ࡔࡶࡤࡸࡺࡹࠢ࠭ࠢ࡟ࠎࠥࠦࠠࠡࠢࠣࠤࠥࠦࠠࠡࠢࠣࠤࠥࠦࠠࠡࠢࠣࠤࠥࠦࠠࠣࡣࡵ࡫ࡺࡳࡥ࡯ࡶࡶࠦ࠿ࠦࡻࠡࠤࡶࡸࡦࡺࡵࡴࠤ࠽ࠦ࡫ࡧࡩ࡭ࡧࡧࠦࠥࢃࠠ࡝ࠌࠣࠤࠥࠦࠠࠡࠢࠣࠤࠥࠦࠠࠡࠢࠣࠤࠥࠦࠠࠡࡿࠪࠤ")
+                    bstack11ll_opy_ (u"ࠬࡨࡲࡰࡹࡶࡩࡷࡹࡴࡢࡥ࡮ࡣࡪࡾࡥࡤࡷࡷࡳࡷࡀࠠࡼࠢ࡟ࠎࠥࠦࠠࠡࠢࠣࠤࠥࠦࠠࠡࠢࠣࠤࠥࠦࠠࠡࠢࠣࠤࠥࠦࠠࠣࡣࡦࡸ࡮ࡵ࡮ࠣ࠼ࠣࠦࡸ࡫ࡴࡔࡧࡶࡷ࡮ࡵ࡮ࡔࡶࡤࡸࡺࡹࠢ࠭ࠢ࡟ࠎࠥࠦࠠࠡࠢࠣࠤࠥࠦࠠࠡࠢࠣࠤࠥࠦࠠࠡࠢࠣࠤࠥࠦࠠࠣࡣࡵ࡫ࡺࡳࡥ࡯ࡶࡶࠦ࠿ࠦࡻࠡࠤࡶࡸࡦࡺࡵࡴࠤ࠽ࠦ࡫ࡧࡩ࡭ࡧࡧࠦࠥࢃࠠ࡝ࠌࠣࠤࠥࠦࠠࠡࠢࠣࠤࠥࠦࠠࠡࠢࠣࠤࠥࠦࠠࠡࡿࠪࠤ")
                 )
     except Exception as e:
-        summary.append(bstack1l1_opy_ (u"ࠨࡗࡂࡔࡑࡍࡓࡍ࠺ࠡࡈࡤ࡭ࡱ࡫ࡤࠡࡶࡲࠤࡺࡶࡤࡢࡶࡨࠤࡸ࡫ࡳࡴ࡫ࡲࡲࠥࡹࡴࡢࡶࡸࡷ࠿ࠦࡻ࠱ࡿࠥࠥ").format(e))
-def bstack1l11_opy_(item, report, summary):
-    if report.when in [bstack1l1_opy_ (u"ࠢࡴࡧࡷࡹࡵࠨࠦ"), bstack1l1_opy_ (u"ࠣࡶࡨࡥࡷࡪ࡯ࡸࡰࠥࠧ")]:
+        summary.append(bstack11ll_opy_ (u"ࠨࡗࡂࡔࡑࡍࡓࡍ࠺ࠡࡈࡤ࡭ࡱ࡫ࡤࠡࡶࡲࠤࡺࡶࡤࡢࡶࡨࠤࡸ࡫ࡳࡴ࡫ࡲࡲࠥࡹࡴࡢࡶࡸࡷ࠿ࠦࡻ࠱ࡿࠥࠥ").format(e))
+def bstack11l1_opy_(item, report, summary):
+    if report.when in [bstack11ll_opy_ (u"ࠢࡴࡧࡷࡹࡵࠨࠦ"), bstack11ll_opy_ (u"ࠣࡶࡨࡥࡷࡪ࡯ࡸࡰࠥࠧ")]:
             return
-    bstack1ll1_opy_(item._page, report.nodeid)
-    passed = report.passed or (report.failed and hasattr(report, bstack1l1_opy_ (u"ࠤࡺࡥࡸࡾࡦࡢ࡫࡯ࠦࠨ")))
-    bstack1lll1_opy_ = bstack1l1_opy_ (u"ࠥࠦࠩ")
+    bstack1l1l_opy_(item._page, report.nodeid)
+    passed = report.passed or (report.failed and hasattr(report, bstack11ll_opy_ (u"ࠤࡺࡥࡸࡾࡦࡢ࡫࡯ࠦࠨ")))
+    bstack1llll_opy_ = bstack11ll_opy_ (u"ࠥࠦࠩ")
     if not passed:
         try:
-            bstack1lll1_opy_ = report.longrepr.reprcrash
+            bstack1llll_opy_ = report.longrepr.reprcrash
         except Exception as e:
             summary.append(
-                bstack1l1_opy_ (u"ࠦ࡜ࡇࡒࡏࡋࡑࡋ࠿ࠦࡆࡢ࡫࡯ࡩࡩࠦࡴࡰࠢࡧࡩࡹ࡫ࡲ࡮࡫ࡱࡩࠥ࡬ࡡࡪ࡮ࡸࡶࡪࠦࡲࡦࡣࡶࡳࡳࡀࠠࡼ࠲ࢀࠦࠪ").format(e)
+                bstack11ll_opy_ (u"ࠦ࡜ࡇࡒࡏࡋࡑࡋ࠿ࠦࡆࡢ࡫࡯ࡩࡩࠦࡴࡰࠢࡧࡩࡹ࡫ࡲ࡮࡫ࡱࡩࠥ࡬ࡡࡪ࡮ࡸࡶࡪࠦࡲࡦࡣࡶࡳࡳࡀࠠࡼ࠲ࢀࠦࠪ").format(e)
             )
     try:
         if passed:
-            bstackl_opy_(item._page, bstack1l1_opy_ (u"ࠧࡶࡡࡴࡵࡨࡨࠧࠫ"))
+            bstack111_opy_(item._page, bstack11ll_opy_ (u"ࠧࡶࡡࡴࡵࡨࡨࠧࠫ"))
         else:
-            if bstack1lll1_opy_:
-                bstack111_opy_(item._page, str(bstack1lll1_opy_), bstack1l1_opy_ (u"ࠨࡥࡳࡴࡲࡶࠧࠬ"))
-                bstackl_opy_(item._page, bstack1l1_opy_ (u"ࠢࡧࡣ࡬ࡰࡪࡪࠢ࠭"), str(bstack1lll1_opy_))
+            if bstack1llll_opy_:
+                bstack111l_opy_(item._page, str(bstack1llll_opy_), bstack11ll_opy_ (u"ࠨࡥࡳࡴࡲࡶࠧࠬ"))
+                bstack111_opy_(item._page, bstack11ll_opy_ (u"ࠢࡧࡣ࡬ࡰࡪࡪࠢ࠭"), str(bstack1llll_opy_))
             else:
-                bstackl_opy_(item._page, bstack1l1_opy_ (u"ࠣࡨࡤ࡭ࡱ࡫ࡤࠣ࠮"))
+                bstack111_opy_(item._page, bstack11ll_opy_ (u"ࠣࡨࡤ࡭ࡱ࡫ࡤࠣ࠮"))
     except Exception as e:
-        summary.append(bstack1l1_opy_ (u"ࠤ࡚ࡅࡗࡔࡉࡏࡉ࠽ࠤࡋࡧࡩ࡭ࡧࡧࠤࡹࡵࠠࡶࡲࡧࡥࡹ࡫ࠠࡴࡧࡶࡷ࡮ࡵ࡮ࠡࡵࡷࡥࡹࡻࡳ࠻ࠢࡾ࠴ࢂࠨ࠯").format(e))
+        summary.append(bstack11ll_opy_ (u"ࠤ࡚ࡅࡗࡔࡉࡏࡉ࠽ࠤࡋࡧࡩ࡭ࡧࡧࠤࡹࡵࠠࡶࡲࡧࡥࡹ࡫ࠠࡴࡧࡶࡷ࡮ࡵ࡮ࠡࡵࡷࡥࡹࡻࡳ࠻ࠢࡾ࠴ࢂࠨ࠯").format(e))
 try:
     from typing import Generator
     import pytest_playwright.pytest_playwright as p
     @pytest.fixture
     def page(context: BrowserContext, request: pytest.FixtureRequest) -> Generator[Page, None, None]:
         page = context.new_page()
         request.node._page = page
         yield page
 except:
     pass
 def pytest_addoption(parser):
     try:
         import pytest_selenium.pytest_selenium
     except:
-        parser.addoption(bstack1l1_opy_ (u"ࠥ࠱࠲ࡪࡲࡪࡸࡨࡶࠧ࠰"), action=bstack1l1_opy_ (u"ࠦࡸࡺ࡯ࡳࡧࠥ࠱"), default=bstack1l1_opy_ (u"ࠧࡩࡨࡳࡱࡰࡩࠧ࠲"),
-                        help=bstack1l1_opy_ (u"ࠨࡄࡳ࡫ࡹࡩࡷࠦࡴࡰࠢࡵࡹࡳࠦࡴࡦࡵࡷࡷࠧ࠳"))
+        parser.addoption(bstack11ll_opy_ (u"ࠥ࠱࠲ࡪࡲࡪࡸࡨࡶࠧ࠰"), action=bstack11ll_opy_ (u"ࠦࡸࡺ࡯ࡳࡧࠥ࠱"), default=bstack11ll_opy_ (u"ࠧࡩࡨࡳࡱࡰࡩࠧ࠲"),
+                        help=bstack11ll_opy_ (u"ࠨࡄࡳ࡫ࡹࡩࡷࠦࡴࡰࠢࡵࡹࡳࠦࡴࡦࡵࡷࡷࠧ࠳"))
```

### Comparing `browserstack_sdk-1.8.1/setup.py` & `browserstack_sdk-1.9.2/setup.py`

 * *Files identical despite different names*

