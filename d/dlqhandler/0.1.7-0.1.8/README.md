# Comparing `tmp/dlqhandler-0.1.7.tar.gz` & `tmp/dlqhandler-0.1.8.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dlqhandler-0.1.7.tar", last modified: Wed May 29 06:47:12 2024, max compression
+gzip compressed data, was "dlqhandler-0.1.8.tar", last modified: Wed May 29 19:12:49 2024, max compression
```

## Comparing `dlqhandler-0.1.7.tar` & `dlqhandler-0.1.8.tar`

### file list

```diff
@@ -1,22 +1,22 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-29 06:47:12.258133 dlqhandler-0.1.7/
--rw-r--r--   0 runner    (1001) docker     (127)     1064 2024-05-29 06:47:02.000000 dlqhandler-0.1.7/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)     1228 2024-05-29 06:47:12.258133 dlqhandler-0.1.7/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      731 2024-05-29 06:47:02.000000 dlqhandler-0.1.7/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-29 06:47:12.258133 dlqhandler-0.1.7/dlqhandler.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     1228 2024-05-29 06:47:12.000000 dlqhandler-0.1.7/dlqhandler.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      407 2024-05-29 06:47:12.000000 dlqhandler-0.1.7/dlqhandler.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-29 06:47:12.000000 dlqhandler-0.1.7/dlqhandler.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       11 2024-05-29 06:47:12.000000 dlqhandler-0.1.7/dlqhandler.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)        8 2024-05-29 06:47:12.000000 dlqhandler-0.1.7/dlqhandler.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-29 06:47:12.258133 dlqhandler-0.1.7/handler/
--rw-r--r--   0 runner    (1001) docker     (127)       44 2024-05-29 06:47:02.000000 dlqhandler-0.1.7/handler/__ini__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-29 06:47:12.258133 dlqhandler-0.1.7/handler/dataprovider/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-29 06:47:02.000000 dlqhandler-0.1.7/handler/dataprovider/__ini__.py
--rw-r--r--   0 runner    (1001) docker     (127)      846 2024-05-29 06:47:02.000000 dlqhandler-0.1.7/handler/dataprovider/send_to_aws_sqs.py
--rw-r--r--   0 runner    (1001) docker     (127)     1513 2024-05-29 06:47:02.000000 dlqhandler-0.1.7/handler/dataprovider/sqs_queue.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-29 06:47:12.258133 dlqhandler-0.1.7/handler/services/
--rw-r--r--   0 runner    (1001) docker     (127)       35 2024-05-29 06:47:02.000000 dlqhandler-0.1.7/handler/services/__ini__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1696 2024-05-29 06:47:02.000000 dlqhandler-0.1.7/handler/services/cloudwatch.py
--rw-r--r--   0 runner    (1001) docker     (127)     2753 2024-05-29 06:47:02.000000 dlqhandler-0.1.7/handler/services/process.py
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-29 06:47:12.258133 dlqhandler-0.1.7/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)      720 2024-05-29 06:47:02.000000 dlqhandler-0.1.7/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-29 19:12:49.368278 dlqhandler-0.1.8/
+-rw-r--r--   0 runner    (1001) docker     (127)     1064 2024-05-29 19:12:39.000000 dlqhandler-0.1.8/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)     1228 2024-05-29 19:12:49.368278 dlqhandler-0.1.8/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      731 2024-05-29 19:12:39.000000 dlqhandler-0.1.8/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-29 19:12:49.364278 dlqhandler-0.1.8/dlqhandler/
+-rw-r--r--   0 runner    (1001) docker     (127)       44 2024-05-29 19:12:39.000000 dlqhandler-0.1.8/dlqhandler/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-29 19:12:49.368278 dlqhandler-0.1.8/dlqhandler/dataprovider/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-29 19:12:39.000000 dlqhandler-0.1.8/dlqhandler/dataprovider/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      846 2024-05-29 19:12:39.000000 dlqhandler-0.1.8/dlqhandler/dataprovider/send_to_aws_sqs.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1513 2024-05-29 19:12:39.000000 dlqhandler-0.1.8/dlqhandler/dataprovider/sqs_queue.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-29 19:12:49.368278 dlqhandler-0.1.8/dlqhandler/services/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-29 19:12:39.000000 dlqhandler-0.1.8/dlqhandler/services/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1696 2024-05-29 19:12:39.000000 dlqhandler-0.1.8/dlqhandler/services/cloudwatch.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2759 2024-05-29 19:12:39.000000 dlqhandler-0.1.8/dlqhandler/services/process.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-29 19:12:49.368278 dlqhandler-0.1.8/dlqhandler.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     1228 2024-05-29 19:12:49.000000 dlqhandler-0.1.8/dlqhandler.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      431 2024-05-29 19:12:49.000000 dlqhandler-0.1.8/dlqhandler.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-29 19:12:49.000000 dlqhandler-0.1.8/dlqhandler.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       11 2024-05-29 19:12:49.000000 dlqhandler-0.1.8/dlqhandler.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       11 2024-05-29 19:12:49.000000 dlqhandler-0.1.8/dlqhandler.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-29 19:12:49.368278 dlqhandler-0.1.8/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)      729 2024-05-29 19:12:39.000000 dlqhandler-0.1.8/setup.py
```

### Comparing `dlqhandler-0.1.7/LICENSE` & `dlqhandler-0.1.8/LICENSE`

 * *Files identical despite different names*

### Comparing `dlqhandler-0.1.7/PKG-INFO` & `dlqhandler-0.1.8/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: dlqhandler
-Version: 0.1.7
+Version: 0.1.8
 Summary: A library for handling DLQ messages in AWS SQS
 Home-page: https://github.com/seuusuario/dlq_handler_lib
 Author: Marcelo Ferreira
 Author-email: jaytilangus@gmail.com
 License: UNKNOWN
 Platform: UNKNOWN
 Classifier: Programming Language :: Python :: 3
```

### Comparing `dlqhandler-0.1.7/README.md` & `dlqhandler-0.1.8/README.md`

 * *Files identical despite different names*

### Comparing `dlqhandler-0.1.7/dlqhandler.egg-info/PKG-INFO` & `dlqhandler-0.1.8/dlqhandler.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: dlqhandler
-Version: 0.1.7
+Version: 0.1.8
 Summary: A library for handling DLQ messages in AWS SQS
 Home-page: https://github.com/seuusuario/dlq_handler_lib
 Author: Marcelo Ferreira
 Author-email: jaytilangus@gmail.com
 License: UNKNOWN
 Platform: UNKNOWN
 Classifier: Programming Language :: Python :: 3
```

### Comparing `dlqhandler-0.1.7/handler/dataprovider/send_to_aws_sqs.py` & `dlqhandler-0.1.8/dlqhandler/dataprovider/send_to_aws_sqs.py`

 * *Files identical despite different names*

### Comparing `dlqhandler-0.1.7/handler/dataprovider/sqs_queue.py` & `dlqhandler-0.1.8/dlqhandler/dataprovider/sqs_queue.py`

 * *Files identical despite different names*

### Comparing `dlqhandler-0.1.7/handler/services/cloudwatch.py` & `dlqhandler-0.1.8/dlqhandler/services/cloudwatch.py`

 * *Files identical despite different names*

### Comparing `dlqhandler-0.1.7/handler/services/process.py` & `dlqhandler-0.1.8/dlqhandler/services/process.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 import json
 import logging
-from handler.dataprovider.send_to_aws_sqs import SendToAwsSqs
+from dlqhandler.dataprovider.send_to_aws_sqs import SendToAwsSqs
 from .cloudwatch import CloudWatch
-from handler.dataprovider.sqs_queue import SQSQueue
+from dlqhandler.dataprovider.sqs_queue import SQSQueue
 
 ERROR_STATUS = "ERRO"
 ERROR_MESSAGE = "Número de retentativas excedido"
 REPROCESSING_STATUS = "REPROCESSANDO"
 ATTEMPTS_KEY = "processamento_tentativas"
 STATUS_KEY = "processamento_status"
 MESSAGE_KEY = "processamento_mensagem"
```

### Comparing `dlqhandler-0.1.7/setup.py` & `dlqhandler-0.1.8/setup.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 from setuptools import setup, find_packages
 
 setup(
     name='dlqhandler',
-    version="0.1.7",
-    packages=['handler', 'handler.services', 'handler.dataprovider'],
+    version="0.1.8",
+    packages=['dlqhandler', 'dlqhandler.services', 'dlqhandler.dataprovider'],
     install_requires=[
         'boto3',
         'mock'
     ],
     author="Marcelo Ferreira",
     author_email="jaytilangus@gmail.com",
     description="A library for handling DLQ messages in AWS SQS",
```

