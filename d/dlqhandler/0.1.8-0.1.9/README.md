# Comparing `tmp/dlqhandler-0.1.8.tar.gz` & `tmp/dlqhandler-0.1.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dlqhandler-0.1.8.tar", last modified: Wed May 29 19:12:49 2024, max compression
+gzip compressed data, was "dlqhandler-0.1.9.tar", last modified: Wed May 29 21:27:26 2024, max compression
```

## Comparing `dlqhandler-0.1.8.tar` & `dlqhandler-0.1.9.tar`

### file list

```diff
@@ -1,22 +1,22 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-29 19:12:49.368278 dlqhandler-0.1.8/
--rw-r--r--   0 runner    (1001) docker     (127)     1064 2024-05-29 19:12:39.000000 dlqhandler-0.1.8/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)     1228 2024-05-29 19:12:49.368278 dlqhandler-0.1.8/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      731 2024-05-29 19:12:39.000000 dlqhandler-0.1.8/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-29 19:12:49.364278 dlqhandler-0.1.8/dlqhandler/
--rw-r--r--   0 runner    (1001) docker     (127)       44 2024-05-29 19:12:39.000000 dlqhandler-0.1.8/dlqhandler/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-29 19:12:49.368278 dlqhandler-0.1.8/dlqhandler/dataprovider/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-29 19:12:39.000000 dlqhandler-0.1.8/dlqhandler/dataprovider/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      846 2024-05-29 19:12:39.000000 dlqhandler-0.1.8/dlqhandler/dataprovider/send_to_aws_sqs.py
--rw-r--r--   0 runner    (1001) docker     (127)     1513 2024-05-29 19:12:39.000000 dlqhandler-0.1.8/dlqhandler/dataprovider/sqs_queue.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-29 19:12:49.368278 dlqhandler-0.1.8/dlqhandler/services/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-29 19:12:39.000000 dlqhandler-0.1.8/dlqhandler/services/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1696 2024-05-29 19:12:39.000000 dlqhandler-0.1.8/dlqhandler/services/cloudwatch.py
--rw-r--r--   0 runner    (1001) docker     (127)     2759 2024-05-29 19:12:39.000000 dlqhandler-0.1.8/dlqhandler/services/process.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-29 19:12:49.368278 dlqhandler-0.1.8/dlqhandler.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     1228 2024-05-29 19:12:49.000000 dlqhandler-0.1.8/dlqhandler.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      431 2024-05-29 19:12:49.000000 dlqhandler-0.1.8/dlqhandler.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-29 19:12:49.000000 dlqhandler-0.1.8/dlqhandler.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       11 2024-05-29 19:12:49.000000 dlqhandler-0.1.8/dlqhandler.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       11 2024-05-29 19:12:49.000000 dlqhandler-0.1.8/dlqhandler.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-29 19:12:49.368278 dlqhandler-0.1.8/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)      729 2024-05-29 19:12:39.000000 dlqhandler-0.1.8/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-29 21:27:26.277616 dlqhandler-0.1.9/
+-rw-r--r--   0 runner    (1001) docker     (127)     1064 2024-05-29 21:27:16.000000 dlqhandler-0.1.9/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)     1377 2024-05-29 21:27:26.277616 dlqhandler-0.1.9/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      880 2024-05-29 21:27:16.000000 dlqhandler-0.1.9/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-29 21:27:26.277616 dlqhandler-0.1.9/dlqhandler/
+-rw-r--r--   0 runner    (1001) docker     (127)       44 2024-05-29 21:27:16.000000 dlqhandler-0.1.9/dlqhandler/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-29 21:27:26.277616 dlqhandler-0.1.9/dlqhandler/dataprovider/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-29 21:27:16.000000 dlqhandler-0.1.9/dlqhandler/dataprovider/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      846 2024-05-29 21:27:16.000000 dlqhandler-0.1.9/dlqhandler/dataprovider/send_to_aws_sqs.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1513 2024-05-29 21:27:16.000000 dlqhandler-0.1.9/dlqhandler/dataprovider/sqs_queue.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-29 21:27:26.277616 dlqhandler-0.1.9/dlqhandler/services/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-29 21:27:16.000000 dlqhandler-0.1.9/dlqhandler/services/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1696 2024-05-29 21:27:16.000000 dlqhandler-0.1.9/dlqhandler/services/cloudwatch.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2759 2024-05-29 21:27:16.000000 dlqhandler-0.1.9/dlqhandler/services/process.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-29 21:27:26.277616 dlqhandler-0.1.9/dlqhandler.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     1377 2024-05-29 21:27:26.000000 dlqhandler-0.1.9/dlqhandler.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      431 2024-05-29 21:27:26.000000 dlqhandler-0.1.9/dlqhandler.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-29 21:27:26.000000 dlqhandler-0.1.9/dlqhandler.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       11 2024-05-29 21:27:26.000000 dlqhandler-0.1.9/dlqhandler.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       11 2024-05-29 21:27:26.000000 dlqhandler-0.1.9/dlqhandler.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-29 21:27:26.277616 dlqhandler-0.1.9/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)      729 2024-05-29 21:27:16.000000 dlqhandler-0.1.9/setup.py
```

### Comparing `dlqhandler-0.1.8/LICENSE` & `dlqhandler-0.1.9/LICENSE`

 * *Files identical despite different names*

### Comparing `dlqhandler-0.1.8/PKG-INFO` & `dlqhandler-0.1.9/PKG-INFO`

 * *Files 13% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: dlqhandler
-Version: 0.1.8
+Version: 0.1.9
 Summary: A library for handling DLQ messages in AWS SQS
 Home-page: https://github.com/seuusuario/dlq_handler_lib
 Author: Marcelo Ferreira
 Author-email: jaytilangus@gmail.com
 License: UNKNOWN
 Platform: UNKNOWN
 Classifier: Programming Language :: Python :: 3
@@ -23,18 +23,22 @@
 To install the library, use `pip`:
 
 ```sh
 pip install dlq_handler_lib
 
 from dlq_handler_lib import DLQHandler
 
-# Initialize the DLQHandler with the queue URL, original queue URL, and maximum attempts
+# Initialize the DLQHandler with the required parameters
 handler = DLQHandler(
-    queue_url='https://sqs.us-east-1.amazonaws.com/123456789012/my-dlq',
+    dlq_queue_url='https://sqs.us-east-1.amazonaws.com/123456789012/my-dlq',
     original_queue_url='https://sqs.us-east-1.amazonaws.com/123456789012/my-queue',
-    max_attempts=5
+    max_attempts=5,
+    region_name='us-east-1',
+    env=my_env_config,  # replace with your actual environment config
+    nome_lambda='lambda-reprocessamento-dlq',
+    namespace='DLQ-Mensageria'
 )
 
 # Process the messages from the DLQ
 handler.process_messages()
```

### Comparing `dlqhandler-0.1.8/README.md` & `dlqhandler-0.1.9/dlqhandler.egg-info/PKG-INFO`

 * *Files 26% similar despite different names*

```diff
@@ -1,22 +1,44 @@
+Metadata-Version: 2.1
+Name: dlqhandler
+Version: 0.1.9
+Summary: A library for handling DLQ messages in AWS SQS
+Home-page: https://github.com/seuusuario/dlq_handler_lib
+Author: Marcelo Ferreira
+Author-email: jaytilangus@gmail.com
+License: UNKNOWN
+Platform: UNKNOWN
+Classifier: Programming Language :: Python :: 3
+Classifier: License :: OSI Approved :: MIT License
+Classifier: Operating System :: OS Independent
+Requires-Python: >=3.6
+Description-Content-Type: text/markdown
+License-File: LICENSE
+
 # DLQ Handler Library
 
 A library for handling DLQ (Dead Letter Queue) messages in AWS SQS. This library allows you to reprocess messages from a DLQ with specified parameters such as the queue URL, original queue URL, and maximum number of attempts.
 
 ## Installation
 
 To install the library, use `pip`:
 
 ```sh
 pip install dlq_handler_lib
 
 from dlq_handler_lib import DLQHandler
 
-# Initialize the DLQHandler with the queue URL, original queue URL, and maximum attempts
+# Initialize the DLQHandler with the required parameters
 handler = DLQHandler(
-    queue_url='https://sqs.us-east-1.amazonaws.com/123456789012/my-dlq',
+    dlq_queue_url='https://sqs.us-east-1.amazonaws.com/123456789012/my-dlq',
     original_queue_url='https://sqs.us-east-1.amazonaws.com/123456789012/my-queue',
-    max_attempts=5
+    max_attempts=5,
+    region_name='us-east-1',
+    env=my_env_config,  # replace with your actual environment config
+    nome_lambda='lambda-reprocessamento-dlq',
+    namespace='DLQ-Mensageria'
 )
 
 # Process the messages from the DLQ
 handler.process_messages()
+
+
```

### Comparing `dlqhandler-0.1.8/dlqhandler/dataprovider/send_to_aws_sqs.py` & `dlqhandler-0.1.9/dlqhandler/dataprovider/send_to_aws_sqs.py`

 * *Files identical despite different names*

### Comparing `dlqhandler-0.1.8/dlqhandler/dataprovider/sqs_queue.py` & `dlqhandler-0.1.9/dlqhandler/dataprovider/sqs_queue.py`

 * *Files identical despite different names*

### Comparing `dlqhandler-0.1.8/dlqhandler/services/cloudwatch.py` & `dlqhandler-0.1.9/dlqhandler/services/cloudwatch.py`

 * *Files identical despite different names*

### Comparing `dlqhandler-0.1.8/dlqhandler/services/process.py` & `dlqhandler-0.1.9/dlqhandler/services/process.py`

 * *Files identical despite different names*

### Comparing `dlqhandler-0.1.8/setup.py` & `dlqhandler-0.1.9/setup.py`

 * *Files 17% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from setuptools import setup, find_packages
 
 setup(
     name='dlqhandler',
-    version="0.1.8",
+    version="0.1.9",
     packages=['dlqhandler', 'dlqhandler.services', 'dlqhandler.dataprovider'],
     install_requires=[
         'boto3',
         'mock'
     ],
     author="Marcelo Ferreira",
     author_email="jaytilangus@gmail.com",
```

