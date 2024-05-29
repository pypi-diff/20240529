# Comparing `tmp/antchain_bot-1.9.7.tar.gz` & `tmp/antchain_bot-1.9.8.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/antchain_bot-1.9.7.tar", last modified: Wed Nov 29 11:02:59 2023, max compression
+gzip compressed data, was "dist/antchain_bot-1.9.8.tar", last modified: Tue Dec 12 03:28:50 2023, max compression
```

## Comparing `antchain_bot-1.9.7.tar` & `antchain_bot-1.9.8.tar`

### file list

```diff
@@ -1,18 +1,18 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-11-29 11:02:59.000000 antchain_bot-1.9.7/
--rw-r--r--   0 root         (0) root         (0)      600 2023-11-29 11:02:59.000000 antchain_bot-1.9.7/LICENSE
--rw-r--r--   0 root         (0) root         (0)       29 2023-11-29 11:02:59.000000 antchain_bot-1.9.7/MANIFEST.in
--rw-r--r--   0 root         (0) root         (0)     2162 2023-11-29 11:02:59.000000 antchain_bot-1.9.7/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)      804 2023-11-29 11:02:59.000000 antchain_bot-1.9.7/README-CN.md
--rw-r--r--   0 root         (0) root         (0)      990 2023-11-29 11:02:59.000000 antchain_bot-1.9.7/README.md
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-11-29 11:02:59.000000 antchain_bot-1.9.7/antchain_bot.egg-info/
--rw-r--r--   0 root         (0) root         (0)     2162 2023-11-29 11:02:59.000000 antchain_bot-1.9.7/antchain_bot.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)      323 2023-11-29 11:02:59.000000 antchain_bot-1.9.7/antchain_bot.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2023-11-29 11:02:59.000000 antchain_bot-1.9.7/antchain_bot.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)      108 2023-11-29 11:02:59.000000 antchain_bot-1.9.7/antchain_bot.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)       17 2023-11-29 11:02:59.000000 antchain_bot-1.9.7/antchain_bot.egg-info/top_level.txt
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-11-29 11:02:59.000000 antchain_bot-1.9.7/antchain_sdk_bot/
--rw-r--r--   0 root         (0) root         (0)       21 2023-11-29 11:02:59.000000 antchain_bot-1.9.7/antchain_sdk_bot/__init__.py
--rw-r--r--   0 root         (0) root         (0)   464972 2023-11-29 11:02:59.000000 antchain_bot-1.9.7/antchain_sdk_bot/client.py
--rw-r--r--   0 root         (0) root         (0)  1237783 2023-11-29 11:02:59.000000 antchain_bot-1.9.7/antchain_sdk_bot/models.py
--rw-r--r--   0 root         (0) root         (0)       73 2023-11-29 11:02:59.000000 antchain_bot-1.9.7/setup.cfg
--rw-r--r--   0 root         (0) root         (0)     2489 2023-11-29 11:02:59.000000 antchain_bot-1.9.7/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-12-12 03:28:50.000000 antchain_bot-1.9.8/
+-rw-r--r--   0 root         (0) root         (0)      600 2023-12-12 03:28:50.000000 antchain_bot-1.9.8/LICENSE
+-rw-r--r--   0 root         (0) root         (0)       29 2023-12-12 03:28:50.000000 antchain_bot-1.9.8/MANIFEST.in
+-rw-r--r--   0 root         (0) root         (0)     2162 2023-12-12 03:28:50.000000 antchain_bot-1.9.8/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)      804 2023-12-12 03:28:50.000000 antchain_bot-1.9.8/README-CN.md
+-rw-r--r--   0 root         (0) root         (0)      990 2023-12-12 03:28:50.000000 antchain_bot-1.9.8/README.md
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-12-12 03:28:50.000000 antchain_bot-1.9.8/antchain_bot.egg-info/
+-rw-r--r--   0 root         (0) root         (0)     2162 2023-12-12 03:28:50.000000 antchain_bot-1.9.8/antchain_bot.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)      323 2023-12-12 03:28:50.000000 antchain_bot-1.9.8/antchain_bot.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2023-12-12 03:28:50.000000 antchain_bot-1.9.8/antchain_bot.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)      108 2023-12-12 03:28:50.000000 antchain_bot-1.9.8/antchain_bot.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)       17 2023-12-12 03:28:50.000000 antchain_bot-1.9.8/antchain_bot.egg-info/top_level.txt
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-12-12 03:28:50.000000 antchain_bot-1.9.8/antchain_sdk_bot/
+-rw-r--r--   0 root         (0) root         (0)       21 2023-12-12 03:28:50.000000 antchain_bot-1.9.8/antchain_sdk_bot/__init__.py
+-rw-r--r--   0 root         (0) root         (0)   464972 2023-12-12 03:28:50.000000 antchain_bot-1.9.8/antchain_sdk_bot/client.py
+-rw-r--r--   0 root         (0) root         (0)  1238069 2023-12-12 03:28:50.000000 antchain_bot-1.9.8/antchain_sdk_bot/models.py
+-rw-r--r--   0 root         (0) root         (0)       73 2023-12-12 03:28:50.000000 antchain_bot-1.9.8/setup.cfg
+-rw-r--r--   0 root         (0) root         (0)     2489 2023-12-12 03:28:50.000000 antchain_bot-1.9.8/setup.py
```

### Comparing `antchain_bot-1.9.7/LICENSE` & `antchain_bot-1.9.8/LICENSE`

 * *Files identical despite different names*

### Comparing `antchain_bot-1.9.7/PKG-INFO` & `antchain_bot-1.9.8/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: antchain_bot
-Version: 1.9.7
+Version: 1.9.8
 Summary: Ant Chain BOT SDK Library for Python
 Home-page: https://github.com/alipay/antchain-openapi-prod-sdk
 Author: Ant Chain SDK
 Author-email: sdk-team@alibabacloud.com
 License: Apache License 2.0
 Description: English | [简体中文](README-CN.md)
```

### Comparing `antchain_bot-1.9.7/README-CN.md` & `antchain_bot-1.9.8/README-CN.md`

 * *Files identical despite different names*

### Comparing `antchain_bot-1.9.7/README.md` & `antchain_bot-1.9.8/README.md`

 * *Files identical despite different names*

### Comparing `antchain_bot-1.9.7/antchain_bot.egg-info/PKG-INFO` & `antchain_bot-1.9.8/antchain_bot.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: antchain-bot
-Version: 1.9.7
+Version: 1.9.8
 Summary: Ant Chain BOT SDK Library for Python
 Home-page: https://github.com/alipay/antchain-openapi-prod-sdk
 Author: Ant Chain SDK
 Author-email: sdk-team@alibabacloud.com
 License: Apache License 2.0
 Description: English | [简体中文](README-CN.md)
```

### Comparing `antchain_bot-1.9.7/antchain_sdk_bot/client.py` & `antchain_bot-1.9.8/antchain_sdk_bot/client.py`

 * *Files 1% similar despite different names*

```diff
@@ -131,15 +131,15 @@
                     'method': action,
                     'version': version,
                     'sign_type': 'HmacSHA1',
                     'req_time': AntchainUtils.get_timestamp(),
                     'req_msg_id': AntchainUtils.get_nonce(),
                     'access_key': self._access_key_id,
                     'base_sdk_version': 'TeaSDK-2.0',
-                    'sdk_version': '1.9.7',
+                    'sdk_version': '1.9.8',
                     '_prod_code': 'BOT',
                     '_prod_channel': 'undefined'
                 }
                 if not UtilClient.empty(self._security_token):
                     _request.query['security_token'] = self._security_token
                 _request.headers = TeaCore.merge({
                     'host': UtilClient.default_string(self._endpoint, 'openapi.antchain.antgroup.com'),
@@ -235,15 +235,15 @@
                     'method': action,
                     'version': version,
                     'sign_type': 'HmacSHA1',
                     'req_time': AntchainUtils.get_timestamp(),
                     'req_msg_id': AntchainUtils.get_nonce(),
                     'access_key': self._access_key_id,
                     'base_sdk_version': 'TeaSDK-2.0',
-                    'sdk_version': '1.9.7',
+                    'sdk_version': '1.9.8',
                     '_prod_code': 'BOT',
                     '_prod_channel': 'undefined'
                 }
                 if not UtilClient.empty(self._security_token):
                     _request.query['security_token'] = self._security_token
                 _request.headers = TeaCore.merge({
                     'host': UtilClient.default_string(self._endpoint, 'openapi.antchain.antgroup.com'),
```

### Comparing `antchain_bot-1.9.7/antchain_sdk_bot/models.py` & `antchain_bot-1.9.8/antchain_sdk_bot/models.py`

 * *Files 0% similar despite different names*

```diff
@@ -1484,14 +1484,15 @@
         trustiot_id: int = None,
         trustiot_entity_id: int = None,
         processed_content: str = None,
         delta_mileage: int = None,
         biz_type: str = None,
         alarm_sub_type: int = None,
         related_trust_entity_id: str = None,
+        report_date: str = None,
     ):
         # 数据的可信平台唯一ID
         self.trustiot_id = trustiot_id
         # IoT可信平台设备唯一ID
         self.trustiot_entity_id = trustiot_entity_id
         # 上报原文解析处理之后的数据
         self.processed_content = processed_content
@@ -1522,14 +1523,16 @@
         # //加速度
         # 11701: 急加速
         # 11702: 急减速
         # 11703: 急转弯
         self.alarm_sub_type = alarm_sub_type
         # 关联设备唯一ID
         self.related_trust_entity_id = related_trust_entity_id
+        # 日报日期
+        self.report_date = report_date
 
     def validate(self):
         self.validate_required(self.trustiot_id, 'trustiot_id')
         self.validate_required(self.trustiot_entity_id, 'trustiot_entity_id')
         self.validate_required(self.processed_content, 'processed_content')
         self.validate_required(self.biz_type, 'biz_type')
 
@@ -1549,14 +1552,16 @@
             result['delta_mileage'] = self.delta_mileage
         if self.biz_type is not None:
             result['biz_type'] = self.biz_type
         if self.alarm_sub_type is not None:
             result['alarm_sub_type'] = self.alarm_sub_type
         if self.related_trust_entity_id is not None:
             result['related_trust_entity_id'] = self.related_trust_entity_id
+        if self.report_date is not None:
+            result['report_date'] = self.report_date
         return result
 
     def from_map(self, m: dict = None):
         m = m or dict()
         if m.get('trustiot_id') is not None:
             self.trustiot_id = m.get('trustiot_id')
         if m.get('trustiot_entity_id') is not None:
@@ -1567,14 +1572,16 @@
             self.delta_mileage = m.get('delta_mileage')
         if m.get('biz_type') is not None:
             self.biz_type = m.get('biz_type')
         if m.get('alarm_sub_type') is not None:
             self.alarm_sub_type = m.get('alarm_sub_type')
         if m.get('related_trust_entity_id') is not None:
             self.related_trust_entity_id = m.get('related_trust_entity_id')
+        if m.get('report_date') is not None:
+            self.report_date = m.get('report_date')
         return self
 
 
 class RentContractInfo(TeaModel):
     def __init__(
         self,
         contract_id: str = None,
```

### Comparing `antchain_bot-1.9.7/setup.py` & `antchain_bot-1.9.8/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -20,15 +20,15 @@
 
 import os
 from setuptools import setup, find_packages
 
 """
 setup module for antchain_bot.
 
-Created on 29/11/2023
+Created on 12/12/2023
 
 @author: Ant Chain SDK
 """
 
 PACKAGE = "antchain_sdk_bot"
 NAME = "antchain_bot" or "alibabacloud-package"
 DESCRIPTION = "Ant Chain BOT SDK Library for Python"
```

