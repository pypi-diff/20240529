# Comparing `tmp/erp_apis_temp-1.0.19-py3-none-any.whl.zip` & `tmp/erp_apis_temp-1.0.20-py3-none-any.whl.zip`

## zipinfo {}

```diff
@@ -1,17 +1,17 @@
-Zip file size: 14818 bytes, number of entries: 15
+Zip file size: 14821 bytes, number of entries: 15
 -rw-rw-rw-  2.0 fat     2347 b- defN 24-May-15 02:53 erp_apis_temp/config.py
--rw-rw-rw-  2.0 fat     3636 b- defN 24-May-13 01:43 erp_apis_temp/erpRequest.py
+-rw-rw-rw-  2.0 fat     3641 b- defN 24-May-29 00:58 erp_apis_temp/erpRequest.py
 -rw-rw-rw-  2.0 fat     4748 b- defN 24-May-28 10:52 erp_apis_temp/apis/afterSales.py
 -rw-rw-rw-  2.0 fat     4471 b- defN 24-May-13 09:46 erp_apis_temp/apis/aftersale_test.py
 -rw-rw-rw-  2.0 fat     1548 b- defN 24-May-28 10:56 erp_apis_temp/apis/goods.py
 -rw-rw-rw-  2.0 fat     1013 b- defN 24-May-28 10:29 erp_apis_temp/apis/inventory.py
 -rw-rw-rw-  2.0 fat     4381 b- defN 24-May-28 10:56 erp_apis_temp/apis/order.py
 -rw-rw-rw-  2.0 fat     3083 b- defN 24-May-28 10:45 erp_apis_temp/apis/refund.py
 -rw-rw-rw-  2.0 fat     2499 b- defN 24-May-13 01:44 erp_apis_temp/apis/test.py
 -rw-rw-rw-  2.0 fat     1144 b- defN 24-May-28 10:45 erp_apis_temp/apis/user.py
 -rw-rw-rw-  2.0 fat     2163 b- defN 24-May-13 07:20 erp_apis_temp/utils/util.py
--rw-rw-rw-  2.0 fat     1540 b- defN 24-May-28 10:56 erp_apis_temp-1.0.19.dist-info/METADATA
--rw-rw-rw-  2.0 fat       92 b- defN 24-May-28 10:56 erp_apis_temp-1.0.19.dist-info/WHEEL
--rw-rw-rw-  2.0 fat       53 b- defN 24-May-28 10:56 erp_apis_temp-1.0.19.dist-info/top_level.txt
--rw-rw-r--  2.0 fat     1263 b- defN 24-May-28 10:56 erp_apis_temp-1.0.19.dist-info/RECORD
-15 files, 33981 bytes uncompressed, 12724 bytes compressed:  62.6%
+-rw-rw-rw-  2.0 fat     1540 b- defN 24-May-29 01:07 erp_apis_temp-1.0.20.dist-info/METADATA
+-rw-rw-rw-  2.0 fat       92 b- defN 24-May-29 01:07 erp_apis_temp-1.0.20.dist-info/WHEEL
+-rw-rw-rw-  2.0 fat       53 b- defN 24-May-29 01:07 erp_apis_temp-1.0.20.dist-info/top_level.txt
+-rw-rw-r--  2.0 fat     1263 b- defN 24-May-29 01:07 erp_apis_temp-1.0.20.dist-info/RECORD
+15 files, 33986 bytes uncompressed, 12727 bytes compressed:  62.6%
```

## zipnote {}

```diff
@@ -27,20 +27,20 @@
 
 Filename: erp_apis_temp/apis/user.py
 Comment: 
 
 Filename: erp_apis_temp/utils/util.py
 Comment: 
 
-Filename: erp_apis_temp-1.0.19.dist-info/METADATA
+Filename: erp_apis_temp-1.0.20.dist-info/METADATA
 Comment: 
 
-Filename: erp_apis_temp-1.0.19.dist-info/WHEEL
+Filename: erp_apis_temp-1.0.20.dist-info/WHEEL
 Comment: 
 
-Filename: erp_apis_temp-1.0.19.dist-info/top_level.txt
+Filename: erp_apis_temp-1.0.20.dist-info/top_level.txt
 Comment: 
 
-Filename: erp_apis_temp-1.0.19.dist-info/RECORD
+Filename: erp_apis_temp-1.0.20.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## erp_apis_temp/erpRequest.py

```diff
@@ -7,15 +7,15 @@
 import os
 from dataclasses import dataclass
 from typing import Optional
 from urllib.parse import urljoin
 from lxml import etree
 from requests import Session as S, Request as Req, Response as Res
 import time, json as j
-from erp_apis.config import DEFAULT_HEADERS, Erp321BaseUrl, ErpApiBaseUrl
+from erp_apis_temp.config import DEFAULT_HEADERS, Erp321BaseUrl, ErpApiBaseUrl
 
 
 @dataclass
 class UserInfoType:
     u_cid: Optional[str]
     u_co_id: Optional[str]
     u_co_name: Optional[str]
```

## Comparing `erp_apis_temp-1.0.19.dist-info/METADATA` & `erp_apis_temp-1.0.20.dist-info/METADATA`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: erp_apis_temp
-Version: 1.0.19
+Version: 1.0.20
 Summary: erp_apis_temp
 Author: 李福成
 Author-email: lfct@qq.com
 License: MIT
 Project-URL: Bug Tracker, https://gitee.com/li_fucheng/erp_sdk_python/issues
 Project-URL: Documentation, https://gitee.com/li_fucheng/erp_sdk_python
 Project-URL: Source Code, https://gitee.com/li_fucheng/erp_sdk_python
```

## Comparing `erp_apis_temp-1.0.19.dist-info/RECORD` & `erp_apis_temp-1.0.20.dist-info/RECORD`

 * *Files 18% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 erp_apis_temp/config.py,sha256=RVm2hs1j0J_Kb8sYbd-r29bzNRWSpR-gJcYnNc3RNPY,2347
-erp_apis_temp/erpRequest.py,sha256=b_6Z9glqi0wkvSG4LKgRx-Z53CXgK2ihycN61D8g20A,3636
+erp_apis_temp/erpRequest.py,sha256=lceObPaa-80sOVdM7tRNAVVXa_PJeOm9fJIM-UWAX74,3641
 erp_apis_temp/apis/afterSales.py,sha256=LoEQJQfvM3gPSpDLN52y3XmGfolbnBH5hlPAFIplzds,4748
 erp_apis_temp/apis/aftersale_test.py,sha256=FjsYknNWL-It4otccyMtqNmcNqLgLIgXG3RqWxcgUdo,4471
 erp_apis_temp/apis/goods.py,sha256=oOkaBEBux_CMw6RJnJ3miHigE2sg0g3-gW8AoS6fWl0,1548
 erp_apis_temp/apis/inventory.py,sha256=ktCBMrKRdHKSOKZIgCCWan0cTYNKm-ddpFNe1hkxgGk,1013
 erp_apis_temp/apis/order.py,sha256=7dwtAHum_hSLZgphhs7MLZt2JyrM6hmCSu1_RlO-bbs,4381
 erp_apis_temp/apis/refund.py,sha256=AgNEEy71L-2p-fd5REZ1fI0RY6b2tmYhBR_tclToq2Y,3083
 erp_apis_temp/apis/test.py,sha256=XrWoVqJFoZxm1MTZcQ8h5kn341VWjPNGfvxg12mUXkE,2499
 erp_apis_temp/apis/user.py,sha256=hloc5Clmx9mIadM56N39MsDOUMrIRefv9cLFHJBM540,1144
 erp_apis_temp/utils/util.py,sha256=Jb9GOlGrYJDLuE8EjsjUbKb_L-VzdqTZkIN4Mgm18Yc,2163
-erp_apis_temp-1.0.19.dist-info/METADATA,sha256=A2D3yZT4yIxaotOH6shXYNHIdK9iTEbaROj79gioXPQ,1540
-erp_apis_temp-1.0.19.dist-info/WHEEL,sha256=GJ7t_kWBFywbagK5eo9IoUwLW6oyOeTKmQ-9iHFVNxQ,92
-erp_apis_temp-1.0.19.dist-info/top_level.txt,sha256=aTOkhDHreCOYKk-4ZEmPt3WkWpC71zChCYS9RykowuI,53
-erp_apis_temp-1.0.19.dist-info/RECORD,,
+erp_apis_temp-1.0.20.dist-info/METADATA,sha256=z1PVtKW0-2xoDHsONxy5l2bcAdgjNMQg3aD21fXOiZE,1540
+erp_apis_temp-1.0.20.dist-info/WHEEL,sha256=GJ7t_kWBFywbagK5eo9IoUwLW6oyOeTKmQ-9iHFVNxQ,92
+erp_apis_temp-1.0.20.dist-info/top_level.txt,sha256=aTOkhDHreCOYKk-4ZEmPt3WkWpC71zChCYS9RykowuI,53
+erp_apis_temp-1.0.20.dist-info/RECORD,,
```

