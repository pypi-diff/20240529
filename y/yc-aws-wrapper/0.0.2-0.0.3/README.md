# Comparing `tmp/yc_aws_wrapper-0.0.2.tar.gz` & `tmp/yc_aws_wrapper-0.0.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "yc_aws_wrapper-0.0.2.tar", last modified: Tue May 28 07:50:49 2024, max compression
+gzip compressed data, was "yc_aws_wrapper-0.0.3.tar", last modified: Tue May 28 10:53:29 2024, max compression
```

## Comparing `yc_aws_wrapper-0.0.2.tar` & `yc_aws_wrapper-0.0.3.tar`

### file list

```diff
@@ -1,28 +1,30 @@
-drwxr-xr-x   0 macuser    (502) staff       (20)        0 2024-05-28 07:50:49.028074 yc_aws_wrapper-0.0.2/
--rw-r--r--   0 macuser    (502) staff       (20)     1226 2024-05-22 15:24:12.000000 yc_aws_wrapper-0.0.2/COPYRIGHT
--rw-r--r--   0 macuser    (502) staff       (20)    35149 2024-05-20 12:22:26.000000 yc_aws_wrapper-0.0.2/LICENSE
--rw-r--r--   0 macuser    (502) staff       (20)       52 2024-05-22 15:24:12.000000 yc_aws_wrapper-0.0.2/MANIFEST.in
--rw-r--r--   0 macuser    (502) staff       (20)     3204 2024-05-28 07:50:49.027840 yc_aws_wrapper-0.0.2/PKG-INFO
--rw-r--r--   0 macuser    (502) staff       (20)     1865 2024-05-27 15:43:12.000000 yc_aws_wrapper-0.0.2/README.md
--rw-r--r--   0 macuser    (502) staff       (20)       38 2024-05-28 07:50:49.028113 yc_aws_wrapper-0.0.2/setup.cfg
--rw-r--r--   0 macuser    (502) staff       (20)     3713 2024-05-22 15:24:55.000000 yc_aws_wrapper-0.0.2/setup.py
-drwxr-xr-x   0 macuser    (502) staff       (20)        0 2024-05-28 07:50:49.025238 yc_aws_wrapper-0.0.2/tests/
--rw-r--r--   0 macuser    (502) staff       (20)     2375 2024-05-28 07:47:49.000000 yc_aws_wrapper-0.0.2/tests/test_s3.py
--rw-r--r--   0 macuser    (502) staff       (20)     2379 2024-05-28 07:47:10.000000 yc_aws_wrapper-0.0.2/tests/test_sqs.py
-drwxr-xr-x   0 macuser    (502) staff       (20)        0 2024-05-28 07:50:49.025871 yc_aws_wrapper-0.0.2/yc_aws_wrapper/
--rw-r--r--   0 macuser    (502) staff       (20)     1966 2024-05-28 07:50:27.000000 yc_aws_wrapper-0.0.2/yc_aws_wrapper/__about__.py
--rw-r--r--   0 macuser    (502) staff       (20)     1703 2024-05-22 15:24:12.000000 yc_aws_wrapper-0.0.2/yc_aws_wrapper/__init__.py
--rw-r--r--   0 macuser    (502) staff       (20)     4001 2024-05-28 07:43:12.000000 yc_aws_wrapper-0.0.2/yc_aws_wrapper/base.py
-drwxr-xr-x   0 macuser    (502) staff       (20)        0 2024-05-28 07:50:49.026820 yc_aws_wrapper-0.0.2/yc_aws_wrapper/kinesis/
--rw-r--r--   0 macuser    (502) staff       (20)      600 2024-05-22 15:24:12.000000 yc_aws_wrapper-0.0.2/yc_aws_wrapper/kinesis/__init__.py
-drwxr-xr-x   0 macuser    (502) staff       (20)        0 2024-05-28 07:50:49.027063 yc_aws_wrapper-0.0.2/yc_aws_wrapper/s3/
--rw-r--r--   0 macuser    (502) staff       (20)     1696 2024-05-27 15:02:06.000000 yc_aws_wrapper-0.0.2/yc_aws_wrapper/s3/__init__.py
-drwxr-xr-x   0 macuser    (502) staff       (20)        0 2024-05-28 07:50:49.027273 yc_aws_wrapper-0.0.2/yc_aws_wrapper/sqs/
--rw-r--r--   0 macuser    (502) staff       (20)     3108 2024-05-27 14:45:14.000000 yc_aws_wrapper-0.0.2/yc_aws_wrapper/sqs/__init__.py
-drwxr-xr-x   0 macuser    (502) staff       (20)        0 2024-05-28 07:50:49.027559 yc_aws_wrapper-0.0.2/yc_aws_wrapper.egg-info/
--rw-r--r--   0 macuser    (502) staff       (20)     3204 2024-05-28 07:50:49.000000 yc_aws_wrapper-0.0.2/yc_aws_wrapper.egg-info/PKG-INFO
--rw-r--r--   0 macuser    (502) staff       (20)      483 2024-05-28 07:50:49.000000 yc_aws_wrapper-0.0.2/yc_aws_wrapper.egg-info/SOURCES.txt
--rw-r--r--   0 macuser    (502) staff       (20)        1 2024-05-28 07:50:49.000000 yc_aws_wrapper-0.0.2/yc_aws_wrapper.egg-info/dependency_links.txt
--rw-r--r--   0 macuser    (502) staff       (20)        1 2024-05-28 07:50:48.000000 yc_aws_wrapper-0.0.2/yc_aws_wrapper.egg-info/not-zip-safe
--rw-r--r--   0 macuser    (502) staff       (20)       31 2024-05-28 07:50:49.000000 yc_aws_wrapper-0.0.2/yc_aws_wrapper.egg-info/requires.txt
--rw-r--r--   0 macuser    (502) staff       (20)       15 2024-05-28 07:50:49.000000 yc_aws_wrapper-0.0.2/yc_aws_wrapper.egg-info/top_level.txt
+drwxr-xr-x   0 macuser    (502) staff       (20)        0 2024-05-28 10:53:29.229492 yc_aws_wrapper-0.0.3/
+-rw-r--r--   0 macuser    (502) staff       (20)     1226 2024-05-22 15:24:12.000000 yc_aws_wrapper-0.0.3/COPYRIGHT
+-rw-r--r--   0 macuser    (502) staff       (20)    35149 2024-05-20 12:22:26.000000 yc_aws_wrapper-0.0.3/LICENSE
+-rw-r--r--   0 macuser    (502) staff       (20)       76 2024-05-28 09:34:25.000000 yc_aws_wrapper-0.0.3/MANIFEST.in
+-rw-r--r--   0 macuser    (502) staff       (20)     3207 2024-05-28 10:53:29.229309 yc_aws_wrapper-0.0.3/PKG-INFO
+-rw-r--r--   0 macuser    (502) staff       (20)     1868 2024-05-28 07:58:22.000000 yc_aws_wrapper-0.0.3/README.md
+-rw-r--r--   0 macuser    (502) staff       (20)       30 2024-05-22 15:24:12.000000 yc_aws_wrapper-0.0.3/requirements.txt
+-rw-r--r--   0 macuser    (502) staff       (20)       38 2024-05-28 10:53:29.229533 yc_aws_wrapper-0.0.3/setup.cfg
+-rw-r--r--   0 macuser    (502) staff       (20)     3713 2024-05-28 10:48:54.000000 yc_aws_wrapper-0.0.3/setup.py
+drwxr-xr-x   0 macuser    (502) staff       (20)        0 2024-05-28 10:53:29.226678 yc_aws_wrapper-0.0.3/tests/
+-rw-r--r--   0 macuser    (502) staff       (20)     2375 2024-05-28 07:55:43.000000 yc_aws_wrapper-0.0.3/tests/test_s3.py
+-rw-r--r--   0 macuser    (502) staff       (20)     2379 2024-05-28 09:17:38.000000 yc_aws_wrapper-0.0.3/tests/test_sqs.py
+drwxr-xr-x   0 macuser    (502) staff       (20)        0 2024-05-28 10:53:29.227461 yc_aws_wrapper-0.0.3/yc_aws_wrapper/
+-rw-r--r--   0 macuser    (502) staff       (20)     1966 2024-05-28 09:27:15.000000 yc_aws_wrapper-0.0.3/yc_aws_wrapper/__about__.py
+-rw-r--r--   0 macuser    (502) staff       (20)     1703 2024-05-22 15:24:12.000000 yc_aws_wrapper-0.0.3/yc_aws_wrapper/__init__.py
+-rw-r--r--   0 macuser    (502) staff       (20)     4040 2024-05-28 09:16:17.000000 yc_aws_wrapper-0.0.3/yc_aws_wrapper/base.py
+-rw-r--r--   0 macuser    (502) staff       (20)      527 2024-05-28 09:15:25.000000 yc_aws_wrapper-0.0.3/yc_aws_wrapper/exceptions.py
+drwxr-xr-x   0 macuser    (502) staff       (20)        0 2024-05-28 10:53:29.228424 yc_aws_wrapper-0.0.3/yc_aws_wrapper/kinesis/
+-rw-r--r--   0 macuser    (502) staff       (20)      600 2024-05-22 15:24:12.000000 yc_aws_wrapper-0.0.3/yc_aws_wrapper/kinesis/__init__.py
+drwxr-xr-x   0 macuser    (502) staff       (20)        0 2024-05-28 10:53:29.228657 yc_aws_wrapper-0.0.3/yc_aws_wrapper/s3/
+-rw-r--r--   0 macuser    (502) staff       (20)     1589 2024-05-28 09:15:25.000000 yc_aws_wrapper-0.0.3/yc_aws_wrapper/s3/__init__.py
+drwxr-xr-x   0 macuser    (502) staff       (20)        0 2024-05-28 10:53:29.228868 yc_aws_wrapper-0.0.3/yc_aws_wrapper/sqs/
+-rw-r--r--   0 macuser    (502) staff       (20)     3154 2024-05-28 09:09:20.000000 yc_aws_wrapper-0.0.3/yc_aws_wrapper/sqs/__init__.py
+drwxr-xr-x   0 macuser    (502) staff       (20)        0 2024-05-28 10:53:29.229121 yc_aws_wrapper-0.0.3/yc_aws_wrapper.egg-info/
+-rw-r--r--   0 macuser    (502) staff       (20)     3207 2024-05-28 10:53:29.000000 yc_aws_wrapper-0.0.3/yc_aws_wrapper.egg-info/PKG-INFO
+-rw-r--r--   0 macuser    (502) staff       (20)      529 2024-05-28 10:53:29.000000 yc_aws_wrapper-0.0.3/yc_aws_wrapper.egg-info/SOURCES.txt
+-rw-r--r--   0 macuser    (502) staff       (20)        1 2024-05-28 10:53:29.000000 yc_aws_wrapper-0.0.3/yc_aws_wrapper.egg-info/dependency_links.txt
+-rw-r--r--   0 macuser    (502) staff       (20)        1 2024-05-28 10:53:29.000000 yc_aws_wrapper-0.0.3/yc_aws_wrapper.egg-info/not-zip-safe
+-rw-r--r--   0 macuser    (502) staff       (20)       31 2024-05-28 10:53:29.000000 yc_aws_wrapper-0.0.3/yc_aws_wrapper.egg-info/requires.txt
+-rw-r--r--   0 macuser    (502) staff       (20)       15 2024-05-28 10:53:29.000000 yc_aws_wrapper-0.0.3/yc_aws_wrapper.egg-info/top_level.txt
```

### Comparing `yc_aws_wrapper-0.0.2/COPYRIGHT` & `yc_aws_wrapper-0.0.3/COPYRIGHT`

 * *Files identical despite different names*

### Comparing `yc_aws_wrapper-0.0.2/LICENSE` & `yc_aws_wrapper-0.0.3/LICENSE`

 * *Files identical despite different names*

### Comparing `yc_aws_wrapper-0.0.2/PKG-INFO` & `yc_aws_wrapper-0.0.3/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: yc-aws-wrapper
-Version: 0.0.2
+Version: 0.0.3
 Summary: yc-aws-wrapper.
 Home-page: https://github.com/mcode-cc/python-yandex-cloud-sdk-wrapper/
 Author: MCode GmbH
 Author-email: python-yandex-cloud-sdk-wrapper@mcode.cc
 License: GNU AFFERO GENERAL PUBLIC LICENSE Version 3, 29 June 2007
 Project-URL: Bug Tracker, https://github.com/mcode-cc/python-yandex-cloud-sdk-wrapper/issues
 Keywords: Wrapper for yandex cloud services
@@ -72,10 +72,10 @@
 > response = sqs.baz.send("Hellow World")   
 > type(response) is None   
 
 code_2:
 > import from yc_aws_wrapper.s3 import SQS   
 >   
 > sqs = SQS()   
-> sqs.load_all_clients()
+> sqs.load_all_clients()   
 > for el in sqs:   
 >   el.send("Hellow World")
```

### Comparing `yc_aws_wrapper-0.0.2/README.md` & `yc_aws_wrapper-0.0.3/README.md`

 * *Files 0% similar despite different names*

```diff
@@ -41,10 +41,10 @@
 > response = sqs.baz.send("Hellow World")   
 > type(response) is None   
 
 code_2:
 > import from yc_aws_wrapper.s3 import SQS   
 >   
 > sqs = SQS()   
-> sqs.load_all_clients()
+> sqs.load_all_clients()   
 > for el in sqs:   
 >   el.send("Hellow World")
```

### Comparing `yc_aws_wrapper-0.0.2/setup.py` & `yc_aws_wrapper-0.0.3/setup.py`

 * *Files identical despite different names*

### Comparing `yc_aws_wrapper-0.0.2/tests/test_s3.py` & `yc_aws_wrapper-0.0.3/tests/test_s3.py`

 * *Files identical despite different names*

### Comparing `yc_aws_wrapper-0.0.2/tests/test_sqs.py` & `yc_aws_wrapper-0.0.3/tests/test_sqs.py`

 * *Files identical despite different names*

### Comparing `yc_aws_wrapper-0.0.2/yc_aws_wrapper/__about__.py` & `yc_aws_wrapper-0.0.3/yc_aws_wrapper/__about__.py`

 * *Files 5% similar despite different names*

```diff
@@ -38,12 +38,12 @@
     "__license__",
     "__copyright__"
 ]
 
 __title__ = "yc-aws-wrapper"
 __summary__ = "yc-aws-wrapper."
 __uri__ = "https://github.com/mcode-cc/python-yandex-cloud-sdk-wrapper/"
-__version__ = "0.0.2"
+__version__ = "0.0.3"
 __author__ = "MCode GmbH"
 __email__ = "python-yandex-cloud-sdk-wrapper@mcode.cc"
 __license__ = "GNU AFFERO GENERAL PUBLIC LICENSE Version 3, 29 June 2007"
 __copyright__ = "2021 %s" % __author__
```

### Comparing `yc_aws_wrapper-0.0.2/yc_aws_wrapper/__init__.py` & `yc_aws_wrapper-0.0.3/yc_aws_wrapper/__init__.py`

 * *Files identical despite different names*

### Comparing `yc_aws_wrapper-0.0.2/yc_aws_wrapper/base.py` & `yc_aws_wrapper-0.0.3/yc_aws_wrapper/base.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,11 @@
 import io
 import json
 import os
+import re
 from typing import Optional
 
 import boto3
 from botocore.config import Config
 
 
 class Stub:
@@ -98,20 +99,20 @@
         _path = self._env(self.__prefix, value)
         if _path is not None:
             self.__clients[value] = self.__client(client=self.client, path=_path)
             return self.__clients[value]
         return None
 
     def load_all_clients(self):
-        _prefix = "{}_{}_".format(self.name, self.__prefix).upper()
+        pattern = "^{}_{}_([a-zA-Z][a-zA-Z0-9]*)$".format(self.name.upper(), self.__prefix)
         for k in os.environ.keys():
-            if k.startswith(_prefix):
-                _k = k.replace(_prefix, "")
-                if _k not in self.__clients:
-                    self.__update(_k)
+            match = re.findall(pattern, k)
+            if len(match) == 1:
+                if match[0] not in self.__clients:
+                    self.__update(match[0])
 
     def __getattr__(self, item: str):
         _item = item.upper()
         attr = self.__clients[_item] if _item in self.__clients else self.__update(_item)
         if attr is not None:
             return attr
         return Stub()
```

### Comparing `yc_aws_wrapper-0.0.2/yc_aws_wrapper/kinesis/__init__.py` & `yc_aws_wrapper-0.0.3/yc_aws_wrapper/kinesis/__init__.py`

 * *Files identical despite different names*

### Comparing `yc_aws_wrapper-0.0.2/yc_aws_wrapper/s3/__init__.py` & `yc_aws_wrapper-0.0.3/yc_aws_wrapper/s3/__init__.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,28 +1,24 @@
 from datetime import datetime
 
 from botocore.exceptions import ClientError
 
 from ..base import DynamicService, DynamicClient, Base
+from ..exceptions import boto_exception
 
 
 class S3Client(DynamicClient):
     def get(self, key: str, version: str = None):
         try:
-            result = self.client.get_object(Bucket=self.path, Key=key) if version is None else \
+            return self.client.get_object(Bucket=self.path, Key=key) if version is None else \
                 self.client.get_object(Bucket=self.path, Key=key, VersionId=version)
         except ClientError as e:
-            try:
-                if e.response["Error"]["Code"] == "NoSuchKey":
-                    result = None
-                else:
-                    raise e
-            except Exception:
-                raise e
-        return result
+            if boto_exception(e, "NoSuchKey"):
+                return None
+            raise e
 
     def put(self, key: str, body: bytes, acl: str = None, expires: datetime = None):
         params = {}
         if acl is not None:
             params["ACL"] = acl
         if isinstance(expires, datetime):
             params["Expires"] = expires
```

### Comparing `yc_aws_wrapper-0.0.2/yc_aws_wrapper/sqs/__init__.py` & `yc_aws_wrapper-0.0.3/yc_aws_wrapper/sqs/__init__.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,14 +1,15 @@
 import json
 from typing import Optional, Union
 
 import boto3
 from botocore.exceptions import ClientError
 
 from ..base import DynamicClient, DynamicService
+from ..exceptions import boto_exception
 
 
 class SQSClient(DynamicClient):
     def __init__(self, client: boto3.client, path: str):
         super().__init__(client, path)
         self.queue = self.client.get_queue_url(QueueName=path).get("QueueUrl", None)
 
@@ -47,29 +48,29 @@
             **kwargs
         }
         return self.client.receive_message(**params).get("Messages", [])
 
     def delete_message(self, receipt: str) -> bool:
         try:
             self.client.delete_message(QueueUrl=self.queue, ReceiptHandle=receipt)
-            result = True
+            return True
         except ClientError as e:
-            try:
-                if e.response["Error"]["Code"] == "ReceiptHandleIsInvalid":
-                    result = False
-                else:
-                    raise e
-            except Exception:
-                raise e
-        return result
+            if boto_exception(e, "ReceiptHandleIsInvalid"):
+                return False
+            raise e
 
 
 class SQS(DynamicService):
     def __init__(self, name: str = "sqs", prefix: str = "TUBE",
                  client_class=SQSClient, auth: bool = True, config: dict = None):
         super().__init__(name=name, prefix=prefix, client_class=client_class, auth=auth, config=config)
 
     def get_url(self, queue: str) -> Optional[str]:
-        return self.client.get_queue_url(QueueName=queue).get("QueueUrl", None)
+        try:
+            return self.client.get_queue_url(QueueName=queue).get("QueueUrl", None)
+        except ClientError as e:
+            if boto_exception(e, "QueueDoesNotExist"):
+                return None
+            raise e
 
     def __getattr__(self, item: str) -> SQSClient:
         return super().__getattr__(item)
```

### Comparing `yc_aws_wrapper-0.0.2/yc_aws_wrapper.egg-info/PKG-INFO` & `yc_aws_wrapper-0.0.3/yc_aws_wrapper.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: yc-aws-wrapper
-Version: 0.0.2
+Version: 0.0.3
 Summary: yc-aws-wrapper.
 Home-page: https://github.com/mcode-cc/python-yandex-cloud-sdk-wrapper/
 Author: MCode GmbH
 Author-email: python-yandex-cloud-sdk-wrapper@mcode.cc
 License: GNU AFFERO GENERAL PUBLIC LICENSE Version 3, 29 June 2007
 Project-URL: Bug Tracker, https://github.com/mcode-cc/python-yandex-cloud-sdk-wrapper/issues
 Keywords: Wrapper for yandex cloud services
@@ -72,10 +72,10 @@
 > response = sqs.baz.send("Hellow World")   
 > type(response) is None   
 
 code_2:
 > import from yc_aws_wrapper.s3 import SQS   
 >   
 > sqs = SQS()   
-> sqs.load_all_clients()
+> sqs.load_all_clients()   
 > for el in sqs:   
 >   el.send("Hellow World")
```

