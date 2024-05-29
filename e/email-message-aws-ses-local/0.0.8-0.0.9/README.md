# Comparing `tmp/email-message-aws-ses-local-0.0.8.tar.gz` & `tmp/email-message-aws-ses-local-0.0.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "email-message-aws-ses-local-0.0.8.tar", last modified: Tue Jan 23 18:57:39 2024, max compression
+gzip compressed data, was "email-message-aws-ses-local-0.0.9.tar", last modified: Mon Jan 29 21:48:29 2024, max compression
```

## Comparing `email-message-aws-ses-local-0.0.8.tar` & `email-message-aws-ses-local-0.0.9.tar`

### file list

```diff
@@ -1,16 +1,16 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-23 18:57:39.960863 email-message-aws-ses-local-0.0.8/
--rw-r--r--   0 runner    (1001) docker     (127)      637 2024-01-23 18:57:39.960863 email-message-aws-ses-local-0.0.8/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     3259 2024-01-23 18:57:05.000000 email-message-aws-ses-local-0.0.8/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-23 18:57:39.956863 email-message-aws-ses-local-0.0.8/email_message_aws_ses_local/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-23 18:57:39.960863 email-message-aws-ses-local-0.0.8/email_message_aws_ses_local/src/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-01-23 18:57:05.000000 email-message-aws-ses-local-0.0.8/email_message_aws_ses_local/src/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     6158 2024-01-23 18:57:05.000000 email-message-aws-ses-local-0.0.8/email_message_aws_ses_local/src/ses_email.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-23 18:57:39.960863 email-message-aws-ses-local-0.0.8/email_message_aws_ses_local.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)      637 2024-01-23 18:57:39.000000 email-message-aws-ses-local-0.0.8/email_message_aws_ses_local.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      376 2024-01-23 18:57:39.000000 email-message-aws-ses-local-0.0.8/email_message_aws_ses_local.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-01-23 18:57:39.000000 email-message-aws-ses-local-0.0.8/email_message_aws_ses_local.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       95 2024-01-23 18:57:39.000000 email-message-aws-ses-local-0.0.8/email_message_aws_ses_local.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       28 2024-01-23 18:57:39.000000 email-message-aws-ses-local-0.0.8/email_message_aws_ses_local.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)      732 2024-01-23 18:57:05.000000 email-message-aws-ses-local-0.0.8/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-01-23 18:57:39.960863 email-message-aws-ses-local-0.0.8/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)      927 2024-01-23 18:57:05.000000 email-message-aws-ses-local-0.0.8/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-29 21:48:29.675915 email-message-aws-ses-local-0.0.9/
+-rw-r--r--   0 runner    (1001) docker     (127)      595 2024-01-29 21:48:29.675915 email-message-aws-ses-local-0.0.9/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     3259 2024-01-29 21:47:50.000000 email-message-aws-ses-local-0.0.9/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-29 21:48:29.671915 email-message-aws-ses-local-0.0.9/email_message_aws_ses_local/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-29 21:48:29.675915 email-message-aws-ses-local-0.0.9/email_message_aws_ses_local/src/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-01-29 21:47:50.000000 email-message-aws-ses-local-0.0.9/email_message_aws_ses_local/src/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6206 2024-01-29 21:47:50.000000 email-message-aws-ses-local-0.0.9/email_message_aws_ses_local/src/ses_email.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-29 21:48:29.675915 email-message-aws-ses-local-0.0.9/email_message_aws_ses_local.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)      595 2024-01-29 21:48:29.000000 email-message-aws-ses-local-0.0.9/email_message_aws_ses_local.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      376 2024-01-29 21:48:29.000000 email-message-aws-ses-local-0.0.9/email_message_aws_ses_local.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-01-29 21:48:29.000000 email-message-aws-ses-local-0.0.9/email_message_aws_ses_local.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       68 2024-01-29 21:48:29.000000 email-message-aws-ses-local-0.0.9/email_message_aws_ses_local.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       28 2024-01-29 21:48:29.000000 email-message-aws-ses-local-0.0.9/email_message_aws_ses_local.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      732 2024-01-29 21:47:50.000000 email-message-aws-ses-local-0.0.9/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-01-29 21:48:29.675915 email-message-aws-ses-local-0.0.9/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)      952 2024-01-29 21:47:50.000000 email-message-aws-ses-local-0.0.9/setup.py
```

### Comparing `email-message-aws-ses-local-0.0.8/README.md` & `email-message-aws-ses-local-0.0.9/README.md`

 * *Files identical despite different names*

### Comparing `email-message-aws-ses-local-0.0.8/email_message_aws_ses_local/src/ses_email.py` & `email-message-aws-ses-local-0.0.9/email_message_aws_ses_local/src/ses_email.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,54 +1,53 @@
-import os
 from datetime import datetime
 from typing import List, Union
 
 import boto3
 from botocore.exceptions import ClientError
-from dotenv import load_dotenv
 from logger_local.Logger import Logger
 # from message_local.MessageImportance import MessageImportance
 from message_local.MessageLocal import MessageLocal
 from message_local.Recipient import Recipient
-
-load_dotenv()
+from python_sdk_remote.utilities import our_get_env
 
 EMAIL_MESSAGE_AWS_SES_LOCAL_PYTHON_PACKAGE_COMPONENT_ID = 208
 EMAIL_MESSAGE_AWS_SES_LOCAL_PYTHON_PACKAGE_COMPONENT_NAME = "email_message_aws_ses_local_python_package"
 DEVELOPER_EMAIL = "emad.a@circ.zone"
 
 logger = Logger.create_logger(object={
     "component_id": EMAIL_MESSAGE_AWS_SES_LOCAL_PYTHON_PACKAGE_COMPONENT_ID,
     "component_name": EMAIL_MESSAGE_AWS_SES_LOCAL_PYTHON_PACKAGE_COMPONENT_NAME,
     "component_category": "Code",
     "developer_email": DEVELOPER_EMAIL
 })
 
-MAIL_TYPE_ID = 1
-AWS_REGION = os.getenv('AWS_DEFAULT_REGION', 'us-west-2')
-FROM_EMAIL = os.getenv('FROM_EMAIL', 'info@circ.zone')
-DEFAULT_CONFIGURATION_SET = os.getenv('CONFIGURATION_SET')
+EMAIL_AWS_SES_API_TYPE = 1
+MESSAGE_NOT_SENT = 0
+
+AWS_REGION = our_get_env('AWS_DEFAULT_REGION', 'us-west-2')
+FROM_EMAIL = our_get_env('FROM_EMAIL', 'info@circ.zone')
+AWS_SES_DEFAULT_CONFIGURATION_SET = our_get_env('CONFIGURATION_SET')
 
 
 class EmailMessageAwsSesLocal(MessageLocal):
     """Assuming the usage is as follows:
     message_local = MessageLocal(...)
     message_local.__class__ = EmailMessageAwsSesLocal
     message_local.__init__()  # calling the "init" of EmailMessageAwsSesLocal
     message_local.send(...)  # calling the "send" of EmailMessageAwsSesLocal
     """
 
-    def __init__(self, subject: str, ses_resource=None, api_type_id=MAIL_TYPE_ID, from_email=FROM_EMAIL,  # noqa
-                 configuration_set=DEFAULT_CONFIGURATION_SET):
+    def __init__(self, subject: str, ses_resource=None, api_type_id=EMAIL_AWS_SES_API_TYPE, from_email=FROM_EMAIL,
+                 aws_ses_configuration_set=AWS_SES_DEFAULT_CONFIGURATION_SET, **kwargs):
         # Don't call super().__init__(), we already have the message_local object
         self.ses_resource = ses_resource or boto3.client('ses', region_name=AWS_REGION)
         self.subject = subject
         self._api_type_id = api_type_id  # used by MessageLocal
         self.from_email = from_email
-        self.configuration_set = configuration_set
+        self.configuration_set = aws_ses_configuration_set
 
     def __send_email(self, recipient_email: str, body: str) -> str:
         """Returns the message ID of the email sent and the message ID of the email saved in the database"""
         try:
             api_data = {
                 'Body': {
                     'Text': {
@@ -59,64 +58,61 @@
                 'Subject': {
                     'Charset': 'UTF-8',
                     'Data': self.subject,
                 },
             }
 
             if self.can_send(api_data=api_data, outgoing_body=api_data["Body"],
-                             sender_profile_id=self.get_sender_profile_id()):
+                             sender_profile_id=self.sender_profile_id):
                 response = self.ses_resource.send_email(
                     Destination={'ToAddresses': [recipient_email]},
                     Message=api_data,
-                    Source=os.getenv('FROM_EMAIL', 'info@circ.zone'),  # Use provided or default sender email
-                    ConfigurationSetName=os.getenv('CONFIGURATION_SET', None)  # Set Configuration Set if provided
+                    Source=our_get_env('FROM_EMAIL', 'info@circ.zone'),  # Use provided or default sender email
+                    ConfigurationSetName=our_get_env('CONFIGURATION_SET', None)  # Set Configuration Set if provided
                 )
                 # Example MessageId: '0100018c9e7552b1-b8932399-7049-492d-ae47-8f60967f49f1-000000'
-                email_messageid = response['MessageId']
-                logger.info(f"Email sent to {recipient_email} with message ID: {email_messageid}, "
+                email_message_id = response['MessageId']
+                logger.info(f"Email sent to {recipient_email} with message ID: {email_message_id}, "
                             f"subject: {self.subject}, body: {body}, recipient_email: {recipient_email}",
-                            object={"email_messageid": email_messageid, "destination_emails": recipient_email})
+                            object={"email_message_id": email_message_id, "destination_emails": recipient_email})
                 self.after_send_attempt(outgoing_body=api_data, incoming_message=response['ResponseMetadata'],
                                         http_status_code=response['ResponseMetadata']['HTTPStatusCode'],
                                         response_body=response)
             else:
                 logger.warn(f"EmailMessageAwsSesLocal.__send_email can_send is False: "
                             f"supposed to send email to {recipient_email} with body {body}")
-                email_messageid = '0'
+                email_message_id = '0'
         except ClientError as e:
             logger.exception(f"Couldn't send email to {recipient_email}. Error: {e}")
             raise
-        return email_messageid
+        return email_message_id
 
-    def send(self, body: str = None, compound_message: dict = None,
-             to_recipients: List[Recipient] = None, cc: List[Recipient] = None, bcc: List[Recipient] = None,
+    def send(self, body: str = None, compound_message_dict: dict = None, recipients: List[Recipient] = None,
+             cc: List[Recipient] = None, bcc: List[Recipient] = None,
              scheduled_timestamp_start: Union[str, datetime] = None,
-             scheduled_timestamp_end: Union[str, datetime] = None) -> list[int]:
-        to_recipients = to_recipients or self.get_recipients()
-        logger.start(object={"body": body, "recipients": to_recipients})
+             scheduled_timestamp_end: Union[str, datetime] = None, **kwargs) -> list[int]:
+        recipients = recipients or self.get_recipients()
+        logger.start(object={"body": body, "recipients": recipients})
         messages_ids = []
-        for recipient in to_recipients:
+        for recipient in recipients:
             message_body = body or self.get_body_after_text_template(recipient)
             recipient_email = recipient.get_email_address()
             if recipient_email is not None:
-                if os.getenv("REALLY_SEND_EMAIL") == '1':
-                    email_messageid = self.__send_email(recipient_email, message_body)
+                if our_get_env("REALLY_SEND_EMAIL"):
+                    email_message_id = self.__send_email(recipient_email, message_body)
                     # TODO: subject and body should be inside ml table
                     self.set_schema("message")
-                    message_id = self.insert(data_json={"email_messageid": email_messageid,
+                    message_id = self.insert(data_json={"email_message_id": email_message_id,
                                                         "body": body,
                                                         "subject": self.subject,
                                                         "to_profile_id": recipient.get_profile_id(),
                                                         "to_email": recipient_email,
                                                         })
                 else:
                     logger.info(f"EmailMessageAwsSesLocal.send REALLY_SEND_EMAIL is off: "
                                 f"supposed to send email to {recipient_email} with body {message_body}")
-                    message_id = 0
+                    message_id = MESSAGE_NOT_SENT
             else:
                 logger.warn(f"recipient.get_email() is None: {recipient}")
-                message_id = 0
+                message_id = MESSAGE_NOT_SENT
             messages_ids.append(message_id)
         return messages_ids
-
-    def get_sender_profile_id(self) -> int:
-        return 1
```

### Comparing `email-message-aws-ses-local-0.0.8/pyproject.toml` & `email-message-aws-ses-local-0.0.9/pyproject.toml`

 * *Files identical despite different names*

### Comparing `email-message-aws-ses-local-0.0.8/setup.py` & `email-message-aws-ses-local-0.0.9/setup.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,26 +1,28 @@
 import setuptools
 
 PACKAGE_NAME = "email-message-aws-ses-local"
 package_dir = PACKAGE_NAME.replace("-", "_")
 
 setuptools.setup(
     name=PACKAGE_NAME,
-    version='0.0.8',
+    version='0.0.9',
     author="Circles",
     author_email="info@circlez.ai",
     description="PyPI Package for Circles AWS email",
     long_description="PyPI Package for Circles AWS email",
     long_description_content_type='text/markdown',
-    url="https://github.com/circles-zone/email-message-aws-ses-local-python-package",
-
+    url=f"https://github.com/circles-zone/{PACKAGE_NAME}-python-package",
     packages=[package_dir],
     package_dir={package_dir: f'{package_dir}/src'},
     package_data={package_dir: ['*.py']},
-    install_requires=["api-management-local", "variable-local", "boto3>=1.28.70", "message-local",
-                      "database-mysql-local>=0.0.121"],
+    install_requires=["boto3>=1.28.70",
+                      "logger-local>=0.0.51 ",
+                      "message-local",
+                      "python_sdk_remote"
+                      ],
     classifiers=[
         "Programming Language :: Python :: 3",
         "License :: Other/Proprietary License",
         "Operating System :: OS Independent",
     ],
 )
```

