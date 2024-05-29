# Comparing `tmp/dlqhandler-0.1.9.tar.gz` & `tmp/dlqhandler-0.2.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dlqhandler-0.1.9.tar", last modified: Wed May 29 21:27:26 2024, max compression
+gzip compressed data, was "dlqhandler-0.2.1.tar", last modified: Wed May 29 21:36:37 2024, max compression
```

## Comparing `dlqhandler-0.1.9.tar` & `dlqhandler-0.2.1.tar`

### file list

```diff
@@ -1,22 +1,22 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-29 21:27:26.277616 dlqhandler-0.1.9/
--rw-r--r--   0 runner    (1001) docker     (127)     1064 2024-05-29 21:27:16.000000 dlqhandler-0.1.9/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)     1377 2024-05-29 21:27:26.277616 dlqhandler-0.1.9/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      880 2024-05-29 21:27:16.000000 dlqhandler-0.1.9/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-29 21:27:26.277616 dlqhandler-0.1.9/dlqhandler/
--rw-r--r--   0 runner    (1001) docker     (127)       44 2024-05-29 21:27:16.000000 dlqhandler-0.1.9/dlqhandler/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-29 21:27:26.277616 dlqhandler-0.1.9/dlqhandler/dataprovider/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-29 21:27:16.000000 dlqhandler-0.1.9/dlqhandler/dataprovider/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      846 2024-05-29 21:27:16.000000 dlqhandler-0.1.9/dlqhandler/dataprovider/send_to_aws_sqs.py
--rw-r--r--   0 runner    (1001) docker     (127)     1513 2024-05-29 21:27:16.000000 dlqhandler-0.1.9/dlqhandler/dataprovider/sqs_queue.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-29 21:27:26.277616 dlqhandler-0.1.9/dlqhandler/services/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-29 21:27:16.000000 dlqhandler-0.1.9/dlqhandler/services/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1696 2024-05-29 21:27:16.000000 dlqhandler-0.1.9/dlqhandler/services/cloudwatch.py
--rw-r--r--   0 runner    (1001) docker     (127)     2759 2024-05-29 21:27:16.000000 dlqhandler-0.1.9/dlqhandler/services/process.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-29 21:27:26.277616 dlqhandler-0.1.9/dlqhandler.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     1377 2024-05-29 21:27:26.000000 dlqhandler-0.1.9/dlqhandler.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      431 2024-05-29 21:27:26.000000 dlqhandler-0.1.9/dlqhandler.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-29 21:27:26.000000 dlqhandler-0.1.9/dlqhandler.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       11 2024-05-29 21:27:26.000000 dlqhandler-0.1.9/dlqhandler.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       11 2024-05-29 21:27:26.000000 dlqhandler-0.1.9/dlqhandler.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-29 21:27:26.277616 dlqhandler-0.1.9/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)      729 2024-05-29 21:27:16.000000 dlqhandler-0.1.9/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-29 21:36:37.738782 dlqhandler-0.2.1/
+-rw-r--r--   0 runner    (1001) docker     (127)     1064 2024-05-29 21:36:25.000000 dlqhandler-0.2.1/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)     1375 2024-05-29 21:36:37.738782 dlqhandler-0.2.1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      878 2024-05-29 21:36:25.000000 dlqhandler-0.2.1/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-29 21:36:37.734782 dlqhandler-0.2.1/dlqhandler/
+-rw-r--r--   0 runner    (1001) docker     (127)       44 2024-05-29 21:36:25.000000 dlqhandler-0.2.1/dlqhandler/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-29 21:36:37.734782 dlqhandler-0.2.1/dlqhandler/dataprovider/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-29 21:36:25.000000 dlqhandler-0.2.1/dlqhandler/dataprovider/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      846 2024-05-29 21:36:25.000000 dlqhandler-0.2.1/dlqhandler/dataprovider/send_to_aws_sqs.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1513 2024-05-29 21:36:25.000000 dlqhandler-0.2.1/dlqhandler/dataprovider/sqs_queue.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-29 21:36:37.738782 dlqhandler-0.2.1/dlqhandler/services/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-29 21:36:25.000000 dlqhandler-0.2.1/dlqhandler/services/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1696 2024-05-29 21:36:25.000000 dlqhandler-0.2.1/dlqhandler/services/cloudwatch.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2759 2024-05-29 21:36:25.000000 dlqhandler-0.2.1/dlqhandler/services/process.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-29 21:36:37.734782 dlqhandler-0.2.1/dlqhandler.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     1375 2024-05-29 21:36:37.000000 dlqhandler-0.2.1/dlqhandler.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      431 2024-05-29 21:36:37.000000 dlqhandler-0.2.1/dlqhandler.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-29 21:36:37.000000 dlqhandler-0.2.1/dlqhandler.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       11 2024-05-29 21:36:37.000000 dlqhandler-0.2.1/dlqhandler.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       11 2024-05-29 21:36:37.000000 dlqhandler-0.2.1/dlqhandler.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-29 21:36:37.738782 dlqhandler-0.2.1/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)      729 2024-05-29 21:36:25.000000 dlqhandler-0.2.1/setup.py
```

### Comparing `dlqhandler-0.1.9/LICENSE` & `dlqhandler-0.2.1/LICENSE`

 * *Files identical despite different names*

### Comparing `dlqhandler-0.1.9/PKG-INFO` & `dlqhandler-0.2.1/PKG-INFO`

 * *Files 14% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: dlqhandler
-Version: 0.1.9
+Version: 0.2.1
 Summary: A library for handling DLQ messages in AWS SQS
 Home-page: https://github.com/seuusuario/dlq_handler_lib
 Author: Marcelo Ferreira
 Author-email: jaytilangus@gmail.com
 License: UNKNOWN
 Platform: UNKNOWN
 Classifier: Programming Language :: Python :: 3
@@ -19,20 +19,20 @@
 A library for handling DLQ (Dead Letter Queue) messages in AWS SQS. This library allows you to reprocess messages from a DLQ with specified parameters such as the queue URL, original queue URL, and maximum number of attempts.
 
 ## Installation
 
 To install the library, use `pip`:
 
 ```sh
-pip install dlq_handler_lib
+pip install dlqhandler
 
-from dlq_handler_lib import DLQHandler
+from dlqhandler import ProcessMessage
 
 # Initialize the DLQHandler with the required parameters
-handler = DLQHandler(
+handler = ProcessMessage(
     dlq_queue_url='https://sqs.us-east-1.amazonaws.com/123456789012/my-dlq',
     original_queue_url='https://sqs.us-east-1.amazonaws.com/123456789012/my-queue',
     max_attempts=5,
     region_name='us-east-1',
     env=my_env_config,  # replace with your actual environment config
     nome_lambda='lambda-reprocessamento-dlq',
     namespace='DLQ-Mensageria'
```

### Comparing `dlqhandler-0.1.9/README.md` & `dlqhandler-0.2.1/README.md`

 * *Files 18% similar despite different names*

```diff
@@ -3,20 +3,20 @@
 A library for handling DLQ (Dead Letter Queue) messages in AWS SQS. This library allows you to reprocess messages from a DLQ with specified parameters such as the queue URL, original queue URL, and maximum number of attempts.
 
 ## Installation
 
 To install the library, use `pip`:
 
 ```sh
-pip install dlq_handler_lib
+pip install dlqhandler
 
-from dlq_handler_lib import DLQHandler
+from dlqhandler import ProcessMessage
 
 # Initialize the DLQHandler with the required parameters
-handler = DLQHandler(
+handler = ProcessMessage(
     dlq_queue_url='https://sqs.us-east-1.amazonaws.com/123456789012/my-dlq',
     original_queue_url='https://sqs.us-east-1.amazonaws.com/123456789012/my-queue',
     max_attempts=5,
     region_name='us-east-1',
     env=my_env_config,  # replace with your actual environment config
     nome_lambda='lambda-reprocessamento-dlq',
     namespace='DLQ-Mensageria'
```

### Comparing `dlqhandler-0.1.9/dlqhandler/dataprovider/send_to_aws_sqs.py` & `dlqhandler-0.2.1/dlqhandler/dataprovider/send_to_aws_sqs.py`

 * *Files identical despite different names*

### Comparing `dlqhandler-0.1.9/dlqhandler/dataprovider/sqs_queue.py` & `dlqhandler-0.2.1/dlqhandler/dataprovider/sqs_queue.py`

 * *Files identical despite different names*

### Comparing `dlqhandler-0.1.9/dlqhandler/services/cloudwatch.py` & `dlqhandler-0.2.1/dlqhandler/services/cloudwatch.py`

 * *Files identical despite different names*

### Comparing `dlqhandler-0.1.9/dlqhandler/services/process.py` & `dlqhandler-0.2.1/dlqhandler/services/process.py`

 * *Files identical despite different names*

### Comparing `dlqhandler-0.1.9/dlqhandler.egg-info/PKG-INFO` & `dlqhandler-0.2.1/dlqhandler.egg-info/PKG-INFO`

 * *Files 14% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: dlqhandler
-Version: 0.1.9
+Version: 0.2.1
 Summary: A library for handling DLQ messages in AWS SQS
 Home-page: https://github.com/seuusuario/dlq_handler_lib
 Author: Marcelo Ferreira
 Author-email: jaytilangus@gmail.com
 License: UNKNOWN
 Platform: UNKNOWN
 Classifier: Programming Language :: Python :: 3
@@ -19,20 +19,20 @@
 A library for handling DLQ (Dead Letter Queue) messages in AWS SQS. This library allows you to reprocess messages from a DLQ with specified parameters such as the queue URL, original queue URL, and maximum number of attempts.
 
 ## Installation
 
 To install the library, use `pip`:
 
 ```sh
-pip install dlq_handler_lib
+pip install dlqhandler
 
-from dlq_handler_lib import DLQHandler
+from dlqhandler import ProcessMessage
 
 # Initialize the DLQHandler with the required parameters
-handler = DLQHandler(
+handler = ProcessMessage(
     dlq_queue_url='https://sqs.us-east-1.amazonaws.com/123456789012/my-dlq',
     original_queue_url='https://sqs.us-east-1.amazonaws.com/123456789012/my-queue',
     max_attempts=5,
     region_name='us-east-1',
     env=my_env_config,  # replace with your actual environment config
     nome_lambda='lambda-reprocessamento-dlq',
     namespace='DLQ-Mensageria'
```

### Comparing `dlqhandler-0.1.9/setup.py` & `dlqhandler-0.2.1/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from setuptools import setup, find_packages
 
 setup(
     name='dlqhandler',
-    version="0.1.9",
+    version="0.2.1",
     packages=['dlqhandler', 'dlqhandler.services', 'dlqhandler.dataprovider'],
     install_requires=[
         'boto3',
         'mock'
     ],
     author="Marcelo Ferreira",
     author_email="jaytilangus@gmail.com",
```

