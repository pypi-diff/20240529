# Comparing `tmp/dlqhandler-0.1.6.tar.gz` & `tmp/dlqhandler-0.1.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dlqhandler-0.1.6.tar", last modified: Tue May 28 05:37:52 2024, max compression
+gzip compressed data, was "dlqhandler-0.1.7.tar", last modified: Wed May 29 06:47:12 2024, max compression
```

## Comparing `dlqhandler-0.1.6.tar` & `dlqhandler-0.1.7.tar`

### file list

```diff
@@ -1,16 +1,22 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-28 05:37:52.775684 dlqhandler-0.1.6/
--rw-r--r--   0 runner    (1001) docker     (127)     1064 2024-05-28 05:37:34.000000 dlqhandler-0.1.6/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)     1228 2024-05-28 05:37:52.775684 dlqhandler-0.1.6/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      731 2024-05-28 05:37:34.000000 dlqhandler-0.1.6/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-28 05:37:52.771684 dlqhandler-0.1.6/dlqhandler/
--rw-r--r--   0 runner    (1001) docker     (127)       31 2024-05-28 05:37:34.000000 dlqhandler-0.1.6/dlqhandler/__ini__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1647 2024-05-28 05:37:34.000000 dlqhandler-0.1.6/dlqhandler/process.py
--rw-r--r--   0 runner    (1001) docker     (127)     1611 2024-05-28 05:37:34.000000 dlqhandler-0.1.6/dlqhandler/sqs_queue.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-28 05:37:52.775684 dlqhandler-0.1.6/dlqhandler.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     1228 2024-05-28 05:37:52.000000 dlqhandler-0.1.6/dlqhandler.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      263 2024-05-28 05:37:52.000000 dlqhandler-0.1.6/dlqhandler.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-28 05:37:52.000000 dlqhandler-0.1.6/dlqhandler.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       11 2024-05-28 05:37:52.000000 dlqhandler-0.1.6/dlqhandler.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       11 2024-05-28 05:37:52.000000 dlqhandler-0.1.6/dlqhandler.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-28 05:37:52.775684 dlqhandler-0.1.6/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)     1416 2024-05-28 05:37:34.000000 dlqhandler-0.1.6/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-29 06:47:12.258133 dlqhandler-0.1.7/
+-rw-r--r--   0 runner    (1001) docker     (127)     1064 2024-05-29 06:47:02.000000 dlqhandler-0.1.7/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)     1228 2024-05-29 06:47:12.258133 dlqhandler-0.1.7/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      731 2024-05-29 06:47:02.000000 dlqhandler-0.1.7/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-29 06:47:12.258133 dlqhandler-0.1.7/dlqhandler.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     1228 2024-05-29 06:47:12.000000 dlqhandler-0.1.7/dlqhandler.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      407 2024-05-29 06:47:12.000000 dlqhandler-0.1.7/dlqhandler.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-29 06:47:12.000000 dlqhandler-0.1.7/dlqhandler.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       11 2024-05-29 06:47:12.000000 dlqhandler-0.1.7/dlqhandler.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        8 2024-05-29 06:47:12.000000 dlqhandler-0.1.7/dlqhandler.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-29 06:47:12.258133 dlqhandler-0.1.7/handler/
+-rw-r--r--   0 runner    (1001) docker     (127)       44 2024-05-29 06:47:02.000000 dlqhandler-0.1.7/handler/__ini__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-29 06:47:12.258133 dlqhandler-0.1.7/handler/dataprovider/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-29 06:47:02.000000 dlqhandler-0.1.7/handler/dataprovider/__ini__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      846 2024-05-29 06:47:02.000000 dlqhandler-0.1.7/handler/dataprovider/send_to_aws_sqs.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1513 2024-05-29 06:47:02.000000 dlqhandler-0.1.7/handler/dataprovider/sqs_queue.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-29 06:47:12.258133 dlqhandler-0.1.7/handler/services/
+-rw-r--r--   0 runner    (1001) docker     (127)       35 2024-05-29 06:47:02.000000 dlqhandler-0.1.7/handler/services/__ini__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1696 2024-05-29 06:47:02.000000 dlqhandler-0.1.7/handler/services/cloudwatch.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2753 2024-05-29 06:47:02.000000 dlqhandler-0.1.7/handler/services/process.py
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-29 06:47:12.258133 dlqhandler-0.1.7/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)      720 2024-05-29 06:47:02.000000 dlqhandler-0.1.7/setup.py
```

### Comparing `dlqhandler-0.1.6/LICENSE` & `dlqhandler-0.1.7/LICENSE`

 * *Files identical despite different names*

### Comparing `dlqhandler-0.1.6/PKG-INFO` & `dlqhandler-0.1.7/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: dlqhandler
-Version: 0.1.6
+Version: 0.1.7
 Summary: A library for handling DLQ messages in AWS SQS
 Home-page: https://github.com/seuusuario/dlq_handler_lib
 Author: Marcelo Ferreira
 Author-email: jaytilangus@gmail.com
 License: UNKNOWN
 Platform: UNKNOWN
 Classifier: Programming Language :: Python :: 3
```

### Comparing `dlqhandler-0.1.6/README.md` & `dlqhandler-0.1.7/README.md`

 * *Files identical despite different names*

### Comparing `dlqhandler-0.1.6/dlqhandler/sqs_queue.py` & `dlqhandler-0.1.7/handler/dataprovider/sqs_queue.py`

 * *Files 23% similar despite different names*

```diff
@@ -1,43 +1,42 @@
 import boto3
 import logging
 
 logger = logging.getLogger()
 logger.setLevel(logging.INFO)
 
 class SQSQueue:
-    def __init__(self, queue_url, max_attempts=5):
+    def __init__(self, queue_url, region_name='us-east-1'):
         self.queue_url = queue_url
-        self.max_attempts = max_attempts
-        self.sqs_client = boto3.client("sqs", region_name="sa-east-1")
-    def receive_messages(self, max_number=10, wait_time=0):
+        self.sqs_client = boto3.client("sqs", region_name=region_name)
+
+    def receive_messages_dlq(self, event=None, max_number=10, wait_time=0):
         try:
-            logger.info('Fetching messages from SQS queue')
+            logger.info('Starting to read messages from the queue')
+            
             messages = self.sqs_client.receive_message(
                 QueueUrl=self.queue_url,
                 AttributeNames=['All'],
                 MaxNumberOfMessages=max_number,
                 WaitTimeSeconds=wait_time
             )
-            logger.info('Received messages from SQS: %s', messages)
 
+            logger.info('Received messages: %s', messages)
             if 'Messages' not in messages:
                 logger.info('No messages to retrieve from SQS: Empty content')
                 return []
 
-            parsed_messages = [(msg['Body'], msg['ReceiptHandle']) for msg in messages['Messages']]
-            logger.debug('Parsed messages: %s', parsed_messages)
-            return parsed_messages
+            return [(msg['Body'], msg['ReceiptHandle']) for msg in messages['Messages']]
         except Exception as e:
             logger.exception("Error receiving messages: %s", e)
             return []
 
-    def delete_message(self, receipt_handle):
+    def delete_message_dlq(self, receipt_handle):
         try:
-            response = self.sqs_client.delete_message(
+            self.sqs_client.delete_message(
                 QueueUrl=self.queue_url,
                 ReceiptHandle=receipt_handle
             )
-            logger.info("Message deleted from the queue: %s", response)
+            logger.info(f"Message with receipt handle {receipt_handle} deleted successfully.")
         except Exception as e:
             logger.exception("Error deleting message: %s", e)
             raise e
```

### Comparing `dlqhandler-0.1.6/dlqhandler.egg-info/PKG-INFO` & `dlqhandler-0.1.7/dlqhandler.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: dlqhandler
-Version: 0.1.6
+Version: 0.1.7
 Summary: A library for handling DLQ messages in AWS SQS
 Home-page: https://github.com/seuusuario/dlq_handler_lib
 Author: Marcelo Ferreira
 Author-email: jaytilangus@gmail.com
 License: UNKNOWN
 Platform: UNKNOWN
 Classifier: Programming Language :: Python :: 3
```

### Comparing `dlqhandler-0.1.6/setup.py` & `dlqhandler-0.1.7/setup.py`

 * *Files 24% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 from setuptools import setup, find_packages
 
 setup(
     name='dlqhandler',
-    version="0.1.6",
-    packages=['dlqhandler'],
+    version="0.1.7",
+    packages=['handler', 'handler.services', 'handler.dataprovider'],
     install_requires=[
         'boto3',
         'mock'
     ],
     author="Marcelo Ferreira",
     author_email="jaytilangus@gmail.com",
     description="A library for handling DLQ messages in AWS SQS",
@@ -16,31 +16,8 @@
     url="https://github.com/seuusuario/dlq_handler_lib",
     classifiers=[
         "Programming Language :: Python :: 3",
         "License :: OSI Approved :: MIT License",
         "Operating System :: OS Independent",
     ],
     python_requires='>=3.6',
-)
-
-# setup(
-#     name='dlq_handler_lib',
-#     version='0.1.6',
-#     description='A library for handling DLQ messages in AWS SQS',
-#     long_description=open('README.md').read(),
-#     long_description_content_type='text/markdown',
-#     url='https://github.com/MarceloJay/lambda-dlq-reprocess-message.git',
-#     author='Marcelo Ferreira',
-#     author_email='jaytilangus@gmail.com',
-#     license='MIT',
-#     packages=find_packages(),
-#     install_requires=[
-#         'boto3>=1.16.0',
-#         'mock>=4.0.3'
-#     ],
-#     classifiers=[
-#         'Programming Language :: Python :: 3',
-#         'License :: OSI Approved :: MIT License',
-#         'Operating System :: OS Independent',
-#     ],
-#     python_requires='>=3.6',
-# )
+)
```

