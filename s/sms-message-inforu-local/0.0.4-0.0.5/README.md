# Comparing `tmp/sms_message_inforu_local-0.0.4.tar.gz` & `tmp/sms_message_inforu_local-0.0.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "sms_message_inforu_local-0.0.4.tar", last modified: Sat May 18 22:01:49 2024, max compression
+gzip compressed data, was "sms_message_inforu_local-0.0.5.tar", last modified: Wed May 29 09:17:29 2024, max compression
```

## Comparing `sms_message_inforu_local-0.0.4.tar` & `sms_message_inforu_local-0.0.5.tar`

### file list

```diff
@@ -1,16 +1,16 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-18 22:01:49.689939 sms_message_inforu_local-0.0.4/
--rw-r--r--   0 runner    (1001) docker     (127)      628 2024-05-18 22:01:49.689939 sms_message_inforu_local-0.0.4/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     3214 2024-05-18 22:01:14.000000 sms_message_inforu_local-0.0.4/README.md
--rw-r--r--   0 runner    (1001) docker     (127)      807 2024-05-18 22:01:14.000000 sms_message_inforu_local-0.0.4/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-18 22:01:49.689939 sms_message_inforu_local-0.0.4/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)     1075 2024-05-18 22:01:14.000000 sms_message_inforu_local-0.0.4/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-18 22:01:49.685939 sms_message_inforu_local-0.0.4/sms_message_inforu_local/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-18 22:01:49.689939 sms_message_inforu_local-0.0.4/sms_message_inforu_local/src/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-18 22:01:14.000000 sms_message_inforu_local-0.0.4/sms_message_inforu_local/src/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     3680 2024-05-18 22:01:14.000000 sms_message_inforu_local-0.0.4/sms_message_inforu_local/src/sms_message_inforu.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-18 22:01:49.689939 sms_message_inforu_local-0.0.4/sms_message_inforu_local.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)      628 2024-05-18 22:01:49.000000 sms_message_inforu_local-0.0.4/sms_message_inforu_local.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      364 2024-05-18 22:01:49.000000 sms_message_inforu_local-0.0.4/sms_message_inforu_local.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-18 22:01:49.000000 sms_message_inforu_local-0.0.4/sms_message_inforu_local.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)      101 2024-05-18 22:01:49.000000 sms_message_inforu_local-0.0.4/sms_message_inforu_local.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       25 2024-05-18 22:01:49.000000 sms_message_inforu_local-0.0.4/sms_message_inforu_local.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-29 09:17:29.015810 sms_message_inforu_local-0.0.5/
+-rw-r--r--   0 runner    (1001) docker     (127)      628 2024-05-29 09:17:29.015810 sms_message_inforu_local-0.0.5/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     3214 2024-05-29 09:16:49.000000 sms_message_inforu_local-0.0.5/README.md
+-rw-r--r--   0 runner    (1001) docker     (127)      807 2024-05-29 09:16:55.000000 sms_message_inforu_local-0.0.5/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-29 09:17:29.015810 sms_message_inforu_local-0.0.5/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)     1075 2024-05-29 09:16:49.000000 sms_message_inforu_local-0.0.5/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-29 09:17:29.011810 sms_message_inforu_local-0.0.5/sms_message_inforu_local/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-29 09:17:29.011810 sms_message_inforu_local-0.0.5/sms_message_inforu_local/src/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-29 09:16:49.000000 sms_message_inforu_local-0.0.5/sms_message_inforu_local/src/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3701 2024-05-29 09:16:49.000000 sms_message_inforu_local-0.0.5/sms_message_inforu_local/src/sms_message_inforu.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-29 09:17:29.011810 sms_message_inforu_local-0.0.5/sms_message_inforu_local.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)      628 2024-05-29 09:17:29.000000 sms_message_inforu_local-0.0.5/sms_message_inforu_local.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      364 2024-05-29 09:17:29.000000 sms_message_inforu_local-0.0.5/sms_message_inforu_local.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-29 09:17:29.000000 sms_message_inforu_local-0.0.5/sms_message_inforu_local.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      101 2024-05-29 09:17:29.000000 sms_message_inforu_local-0.0.5/sms_message_inforu_local.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       25 2024-05-29 09:17:29.000000 sms_message_inforu_local-0.0.5/sms_message_inforu_local.egg-info/top_level.txt
```

### Comparing `sms_message_inforu_local-0.0.4/PKG-INFO` & `sms_message_inforu_local-0.0.5/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: sms-message-inforu-local
-Version: 0.0.4
+Version: 0.0.5
 Summary: PyPI Package for Circles Project SMS
 Home-page: https://github.com/circles-zone/sms-message-inforu-local-python-package
 Author: Circles
 Author-email: info@circles.life
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: Other/Proprietary License
 Classifier: Operating System :: OS Independent
```

### Comparing `sms_message_inforu_local-0.0.4/README.md` & `sms_message_inforu_local-0.0.5/README.md`

 * *Files identical despite different names*

### Comparing `sms_message_inforu_local-0.0.4/pyproject.toml` & `sms_message_inforu_local-0.0.5/pyproject.toml`

 * *Files 12% similar despite different names*

```diff
@@ -7,13 +7,13 @@
 requires = ["setuptools>=61.0"]
 build-backend = "setuptools.build_meta"
 
 [tool.poetry]
 # TODO: Please update the name, similar to storage-local (suffix -local)
 name = "sms-message-inforu-local-python-package"
 # I believe we are still using the version from setup.py and not from here until potery will work
-version = "0.0.1" # https://pypi.org/project/sms-message-inforu-local-python-package i.e. https://pypi.org/project/storage-local/
+version = "0.0.2" # https://pypi.org/project/sms-message-inforu-local-python-package i.e. https://pypi.org/project/storage-local/
 description = "sms-message-inforu-local-python-package Python Package"
 readme = "README.md"
 authors = [
     "Circlez.ai <info@circlez.ai>",
 ]
```

### Comparing `sms_message_inforu_local-0.0.4/setup.py` & `sms_message_inforu_local-0.0.5/setup.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 import setuptools
 PACKAGE_NAME = "sms-message-inforu-local"
 package_dir = PACKAGE_NAME.replace("-", "_")
 
 setuptools.setup(
     name=PACKAGE_NAME,
-    version='0.0.4',  # https://pypi.org/project/sms-message-inforu-local/
+    version='0.0.5',  # https://pypi.org/project/sms-message-inforu-local/
     author="Circles",
     author_email="info@circles.life",
     description="PyPI Package for Circles Project SMS",
     long_description="PyPI Package for Circles Project SMS",
     long_description_content_type='text/markdown',
     url=f"https://github.com/circles-zone/{PACKAGE_NAME}-python-package",
     packages=[package_dir],
```

### Comparing `sms_message_inforu_local-0.0.4/sms_message_inforu_local/src/sms_message_inforu.py` & `sms_message_inforu_local-0.0.5/sms_message_inforu_local/src/sms_message_inforu.py`

 * *Files 2% similar despite different names*

```diff
@@ -37,16 +37,16 @@
              cc: List[Recipient] = None, bcc: List[Recipient] = None,
              scheduled_timestamp_start: datetime = None,
              scheduled_timestamp_end: datetime = None, **kwargs) -> list[int]:
         try:
             recipients = recipients or self.get_recipients()
 
             for recipient in recipients:
-                message = body or self.get_body_text_after_template_processing(recipient)
-                phone = recipient.get_normizalied_phone()
+                message = body or self.get_body_text_after_template_processing(recipient=recipient)
+                phone = recipient.get_phone_number_full_normalized()
                 payload = {
                     "Data": {
                         "Message": message,
                         "Recipients": [
                             {
                                 "Phone": phone,
                             }
```

### Comparing `sms_message_inforu_local-0.0.4/sms_message_inforu_local.egg-info/PKG-INFO` & `sms_message_inforu_local-0.0.5/sms_message_inforu_local.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: sms-message-inforu-local
-Version: 0.0.4
+Version: 0.0.5
 Summary: PyPI Package for Circles Project SMS
 Home-page: https://github.com/circles-zone/sms-message-inforu-local-python-package
 Author: Circles
 Author-email: info@circles.life
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: Other/Proprietary License
 Classifier: Operating System :: OS Independent
```

