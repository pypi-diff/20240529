# Comparing `tmp/whataspp_message_inforu_local-0.0.14.tar.gz` & `tmp/whataspp_message_inforu_local-0.0.15.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "whataspp_message_inforu_local-0.0.14.tar", last modified: Thu May  9 06:38:26 2024, max compression
+gzip compressed data, was "whataspp_message_inforu_local-0.0.15.tar", last modified: Wed May 29 10:24:34 2024, max compression
```

## Comparing `whataspp_message_inforu_local-0.0.14.tar` & `whataspp_message_inforu_local-0.0.15.tar`

### file list

```diff
@@ -1,17 +1,17 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-09 06:38:26.725224 whataspp_message_inforu_local-0.0.14/
--rw-r--r--   0 runner    (1001) docker     (127)      703 2024-05-09 06:38:26.725224 whataspp_message_inforu_local-0.0.14/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     3259 2024-05-09 06:38:00.000000 whataspp_message_inforu_local-0.0.14/README.md
--rw-r--r--   0 runner    (1001) docker     (127)      732 2024-05-09 06:38:00.000000 whataspp_message_inforu_local-0.0.14/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-09 06:38:26.725224 whataspp_message_inforu_local-0.0.14/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)     1245 2024-05-09 06:38:00.000000 whataspp_message_inforu_local-0.0.14/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-09 06:38:26.725224 whataspp_message_inforu_local-0.0.14/whataspp_message_inforu_local/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-09 06:38:26.725224 whataspp_message_inforu_local-0.0.14/whataspp_message_inforu_local/src/
--rw-r--r--   0 runner    (1001) docker     (127)     1126 2024-05-09 06:38:00.000000 whataspp_message_inforu_local-0.0.14/whataspp_message_inforu_local/src/WhatsAppLocalConstants.py
--rw-r--r--   0 runner    (1001) docker     (127)     5247 2024-05-09 06:38:00.000000 whataspp_message_inforu_local-0.0.14/whataspp_message_inforu_local/src/WhatsAppMessageInforuLocal.py
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-09 06:38:00.000000 whataspp_message_inforu_local-0.0.14/whataspp_message_inforu_local/src/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-09 06:38:26.725224 whataspp_message_inforu_local-0.0.14/whataspp_message_inforu_local.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)      703 2024-05-09 06:38:26.000000 whataspp_message_inforu_local-0.0.14/whataspp_message_inforu_local.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      467 2024-05-09 06:38:26.000000 whataspp_message_inforu_local-0.0.14/whataspp_message_inforu_local.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-09 06:38:26.000000 whataspp_message_inforu_local-0.0.14/whataspp_message_inforu_local.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       88 2024-05-09 06:38:26.000000 whataspp_message_inforu_local-0.0.14/whataspp_message_inforu_local.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       30 2024-05-09 06:38:26.000000 whataspp_message_inforu_local-0.0.14/whataspp_message_inforu_local.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-29 10:24:34.255179 whataspp_message_inforu_local-0.0.15/
+-rw-r--r--   0 runner    (1001) docker     (127)      703 2024-05-29 10:24:34.255179 whataspp_message_inforu_local-0.0.15/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     3259 2024-05-29 10:23:51.000000 whataspp_message_inforu_local-0.0.15/README.md
+-rw-r--r--   0 runner    (1001) docker     (127)      732 2024-05-29 10:23:57.000000 whataspp_message_inforu_local-0.0.15/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-29 10:24:34.255179 whataspp_message_inforu_local-0.0.15/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)     1245 2024-05-29 10:23:51.000000 whataspp_message_inforu_local-0.0.15/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-29 10:24:34.251179 whataspp_message_inforu_local-0.0.15/whataspp_message_inforu_local/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-29 10:24:34.251179 whataspp_message_inforu_local-0.0.15/whataspp_message_inforu_local/src/
+-rw-r--r--   0 runner    (1001) docker     (127)     1126 2024-05-29 10:23:51.000000 whataspp_message_inforu_local-0.0.15/whataspp_message_inforu_local/src/WhatsAppLocalConstants.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4137 2024-05-29 10:23:51.000000 whataspp_message_inforu_local-0.0.15/whataspp_message_inforu_local/src/WhatsAppMessageInforuLocal.py
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-29 10:23:51.000000 whataspp_message_inforu_local-0.0.15/whataspp_message_inforu_local/src/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-29 10:24:34.255179 whataspp_message_inforu_local-0.0.15/whataspp_message_inforu_local.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)      703 2024-05-29 10:24:34.000000 whataspp_message_inforu_local-0.0.15/whataspp_message_inforu_local.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      467 2024-05-29 10:24:34.000000 whataspp_message_inforu_local-0.0.15/whataspp_message_inforu_local.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-29 10:24:34.000000 whataspp_message_inforu_local-0.0.15/whataspp_message_inforu_local.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       88 2024-05-29 10:24:34.000000 whataspp_message_inforu_local-0.0.15/whataspp_message_inforu_local.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       30 2024-05-29 10:24:34.000000 whataspp_message_inforu_local-0.0.15/whataspp_message_inforu_local.egg-info/top_level.txt
```

### Comparing `whataspp_message_inforu_local-0.0.14/PKG-INFO` & `whataspp_message_inforu_local-0.0.15/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: whataspp-message-inforu-local
-Version: 0.0.14
+Version: 0.0.15
 Summary: PyPI Package for Circles whataspp_inforu_local Python
 Home-page: https://github.com/circles-zone/whatsapp-message-inforu-local-python-package
 Author: Circles
 Author-email: info@circlez.ai
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: Other/Proprietary License
 Classifier: Operating System :: OS Independent
```

### Comparing `whataspp_message_inforu_local-0.0.14/README.md` & `whataspp_message_inforu_local-0.0.15/README.md`

 * *Files identical despite different names*

### Comparing `whataspp_message_inforu_local-0.0.14/pyproject.toml` & `whataspp_message_inforu_local-0.0.15/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -7,13 +7,13 @@
 requires = ["setuptools>=61.0"]
 build-backend = "setuptools.build_meta"
 
 [tool.poetry]
 # TODO: Please update the name, similar to storage-local (suffix -local)
 name = "<project-name>"
 # I believe we are still using the version from setup.py and not from here until potery will work
-version = "0.0.1" # https://pypi.org/project/<project-name> i.e. https://pypi.org/project/storage-local/
+version = "0.0.2" # https://pypi.org/project/<project-name> i.e. https://pypi.org/project/storage-local/
 description = "<project-name> Python Package"
 readme = "README.md"
 authors = [
     "Circlez.ai <info@circlez.ai>",
 ]
```

### Comparing `whataspp_message_inforu_local-0.0.14/setup.py` & `whataspp_message_inforu_local-0.0.15/setup.py`

 * *Files 10% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 
 PACKAGE_NAME = "whataspp-message-inforu-local"
 # Since all PACAKGE_NAMEs are with an underscore, we don't need this. Why do we need it?
 package_dir = PACKAGE_NAME.replace("-", "_")
 
 setuptools.setup(
     name=PACKAGE_NAME,
-    version='0.0.14',  # update only the minor version each time # https://pypi.org/project/whataspp-inforu-local/
+    version='0.0.15',  # update only the minor version each time # https://pypi.org/project/whataspp-inforu-local/
     author="Circles",
     author_email="info@circlez.ai",
     description="PyPI Package for Circles whataspp_inforu_local Python",
     long_description="This is a package for sharing common whataspp_inforu_local function used in different repositories",
     long_description_content_type='text/markdown',
     url="https://github.com/circles-zone/whatsapp-message-inforu-local-python-package",
     # packages=setuptools.find_packages(),
```

### Comparing `whataspp_message_inforu_local-0.0.14/whataspp_message_inforu_local/src/WhatsAppLocalConstants.py` & `whataspp_message_inforu_local-0.0.15/whataspp_message_inforu_local/src/WhatsAppLocalConstants.py`

 * *Files identical despite different names*

### Comparing `whataspp_message_inforu_local-0.0.14/whataspp_message_inforu_local/src/WhatsAppMessageInforuLocal.py` & `whataspp_message_inforu_local-0.0.15/whataspp_message_inforu_local/src/WhatsAppMessageInforuLocal.py`

 * *Files 18% similar despite different names*

```diff
@@ -4,15 +4,15 @@
 from typing import List
 
 import requests
 from python_sdk_remote.utilities import our_get_env
 from logger_local.MetaLogger import MetaLogger
 from message_local.MessageLocal import MessageLocal
 from message_local.Recipient import Recipient
-from python_sdk_remote.utilities import create_return_http_headers
+from python_sdk_remote.http_response import create_authorization_http_headers
 
 from .WhatsAppLocalConstants import (WHATSAPP_API_URL,
                                      WHATSAPP_MESSAGE_INFORU_API_TYPE_ID,
                                      get_logger_object)
 
 REALLY_SEND_WHATSAPP = our_get_env("REALLY_SEND_WHATSAPP", "false")
 REALLY_SEND_WHATSAPP = REALLY_SEND_WHATSAPP and REALLY_SEND_WHATSAPP.lower() in ("1", "true")
@@ -27,77 +27,55 @@
     message_local.send(...)  # calling the "send" of WhatsAppMessageInforuLocal
     """
 
     def __init__(self, **kwargs) -> None:  # noqa
         # Don't call super().__init__(), we already have the message_local object
         self._api_type_id = WHATSAPP_MESSAGE_INFORU_API_TYPE_ID  # used by MessageLocal
 
-    def build_body(self, message_dict: dict):
-        pass
-
     def send(self, body: str = None, compound_message_dict: dict = None,
              recipients: List[Recipient] = None, cc: List[Recipient] = None, bcc: List[Recipient] = None,
              scheduled_timestamp_start: datetime = None,
              scheduled_timestamp_end: datetime = None, **kwargs) -> dict:  # TODO: return ids
         recipients = recipients or self.get_recipients()
-        try:
-            # Can also add: "FirstName", "LastName", "CouponCode", "MessageMedia"
-            recipients_details = [{"Phone": recipient.get_normizalied_phone()}
-                                  for recipient in recipients]
-            # TODO: should we POST for each recipient or can we use the same message for all of them?
-            # self.get_body_after_text_template(...)
-            self.logger.start("WhatsApp message send", object={
-                "message": body, "kwargs": kwargs})
-            message_media = kwargs.get("message_media")
-            payload = {
-                "Data": {
-                    "Message": body,
-                    "Recipients": recipients_details
-                }
-            }
-            if message_media:
-                payload["Data"]["messageMedia"] = message_media
-            url = WHATSAPP_API_URL
-            headers = {
-                **create_return_http_headers(),
-                'Authorization': INFORU_AUTH_TOKEN
+        # Can also add: "FirstName", "LastName", "CouponCode", "MessageMedia"
+        recipients_details = [{"Phone": recipient.get_phone_number_full_normalized()}
+                              for recipient in recipients]
+        # TODO: should we POST for each recipient or can we use the same message for all of them?
+        # self.get_body_after_text_template(...)
+        message_media = kwargs.get("message_media")
+        payload = {
+            "Data": {
+                "Message": body,
+                "Recipients": recipients_details
             }
-            payload_json = json.dumps(payload)
-            if (REALLY_SEND_WHATSAPP and
-                    self.can_send(api_data=payload, outgoing_body=payload,
-                                  sender_profile_id=self.get_sender_profile_id())):
-                response = requests.post(url, headers=headers, json=payload_json)
-                self.after_send_attempt(outgoing_body=payload,
-                                        incoming_message=response.json(),
-                                        http_status_code=response.status_code,
-                                        response_body=response.text)
-            else:
-                print("Supposed to send the following payload to InforU: " + payload_json)
-                return {"status": "success", "message": "Message sent successfully"}
-
-            # Check the response using HTTPStatus.OK from the http library.
-            if response.status_code == HTTPStatus.OK:
-                self.logger.info("Request Payload: " + json.dumps(payload))
-                self.logger.info("Request Headers: " + str(headers))
-                self.logger.info("Response Status Code: " + str(response.status_code))
-                self.logger.info("Response Content: " + response.text)
-                self.logger.info(f"WhatsApp sent successfully to {recipients_details}.")
-                self.logger.info("Response: " + response.text)
-            else:
-                self.logger.error(
-                    f"SMS sending failed to {recipients_details} with status code: {response.status_code}")
-
-            # Assuming the function returns a dictionary with some data
+        }
+        if message_media:
+            payload["Data"]["messageMedia"] = message_media
+        url = WHATSAPP_API_URL
+
+        payload_json = json.dumps(payload)
+        if (REALLY_SEND_WHATSAPP and
+                self.can_send(api_data=payload, outgoing_body=payload)):
+            headers = create_authorization_http_headers(INFORU_AUTH_TOKEN)
+            response = requests.post(url, headers=headers, json=payload_json)
+            self.after_send_attempt(outgoing_body=payload,
+                                    incoming_message=response.json(),
+                                    http_status_code=response.status_code,
+                                    response_body=response.text)
+        else:
+            print("Supposed to send the following payload to InforU: " + payload_json)
             return {"status": "success", "message": "Message sent successfully"}
 
-        except Exception as e:
-            self.logger.exception("Sending to WhatsApp via InforU failed", object=e)
-            self.logger.end()
-            raise
-        finally:
-            self.logger.end("WhatsApp message send")
-
-    # TODO We should move this method out of here to identity-local-python-package
-    def get_sender_profile_id(self) -> int:
-        # TODO We need to move this function outside i.e. to identity-local-python-package and make sure all packages are using it.
-        #  The function should get the following parameters: user_external_id, lang_code, recipient groups, recipient locations ...
-        return 1
+        # Check the response using HTTPStatus.OK from the http library.
+        if response.status_code == HTTPStatus.OK:
+            self.logger.info("Request Payload: " + json.dumps(payload))
+            self.logger.info("Request Headers: " + str(headers))
+            self.logger.info("Response Status Code: " + str(response.status_code))
+            self.logger.info("Response Content: " + response.text)
+            self.logger.info(f"WhatsApp sent successfully to {recipients_details}.")
+            self.logger.info("Response: " + response.text)
+        else:
+            self.logger.error(
+                f"SMS sending failed to {recipients_details} with status code: {response.status_code}")
+
+        # Assuming the function returns a dictionary with some data
+        return {"status": "success", "message": "Message sent successfully"}
```

### Comparing `whataspp_message_inforu_local-0.0.14/whataspp_message_inforu_local.egg-info/PKG-INFO` & `whataspp_message_inforu_local-0.0.15/whataspp_message_inforu_local.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: whataspp-message-inforu-local
-Version: 0.0.14
+Version: 0.0.15
 Summary: PyPI Package for Circles whataspp_inforu_local Python
 Home-page: https://github.com/circles-zone/whatsapp-message-inforu-local-python-package
 Author: Circles
 Author-email: info@circlez.ai
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: Other/Proprietary License
 Classifier: Operating System :: OS Independent
```

