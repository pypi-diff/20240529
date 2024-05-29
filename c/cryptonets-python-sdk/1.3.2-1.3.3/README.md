# Comparing `tmp/cryptonets_python_sdk-1.3.2.tar.gz` & `tmp/cryptonets_python_sdk-1.3.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "cryptonets_python_sdk-1.3.2.tar", last modified: Thu May 23 10:37:55 2024, max compression
+gzip compressed data, was "cryptonets_python_sdk-1.3.3.tar", last modified: Wed May 29 13:21:31 2024, max compression
```

## Comparing `cryptonets_python_sdk-1.3.2.tar` & `cryptonets_python_sdk-1.3.3.tar`

### file list

```diff
@@ -1,47 +1,48 @@
-drwxrwxr-x   0 azam      (1000) azam      (1000)        0 2024-05-23 10:37:55.093851 cryptonets_python_sdk-1.3.2/
--rw-rw-r--   0 azam      (1000) azam      (1000)        0 2023-09-26 12:09:24.000000 cryptonets_python_sdk-1.3.2/LICENSE
--rw-rw-r--   0 azam      (1000) azam      (1000)       28 2023-09-26 12:09:24.000000 cryptonets_python_sdk-1.3.2/MANIFEST.in
--rw-rw-r--   0 azam      (1000) azam      (1000)     3625 2024-05-23 10:37:55.093851 cryptonets_python_sdk-1.3.2/PKG-INFO
--rw-rw-r--   0 azam      (1000) azam      (1000)     2511 2024-03-20 06:22:40.000000 cryptonets_python_sdk-1.3.2/README.md
--rw-rw-r--   0 azam      (1000) azam      (1000)       38 2024-05-23 10:37:55.093851 cryptonets_python_sdk-1.3.2/setup.cfg
--rw-rw-r--   0 azam      (1000) azam      (1000)     3798 2024-05-23 10:35:08.000000 cryptonets_python_sdk-1.3.2/setup.py
-drwxrwxr-x   0 azam      (1000) azam      (1000)        0 2024-05-23 10:37:55.089851 cryptonets_python_sdk-1.3.2/src/
-drwxrwxr-x   0 azam      (1000) azam      (1000)        0 2024-05-23 10:37:55.089851 cryptonets_python_sdk-1.3.2/src/cryptonets_python_sdk/
--rw-rw-r--   0 azam      (1000) azam      (1000)        0 2024-03-20 06:22:40.000000 cryptonets_python_sdk-1.3.2/src/cryptonets_python_sdk/__init__.py
--rw-rw-r--   0 azam      (1000) azam      (1000)    31186 2024-04-08 11:43:05.000000 cryptonets_python_sdk-1.3.2/src/cryptonets_python_sdk/factor.py
-drwxrwxr-x   0 azam      (1000) azam      (1000)        0 2024-05-23 10:37:55.089851 cryptonets_python_sdk-1.3.2/src/cryptonets_python_sdk/factor_modules/
--rw-rw-r--   0 azam      (1000) azam      (1000)    19933 2024-04-24 15:45:32.000000 cryptonets_python_sdk-1.3.2/src/cryptonets_python_sdk/factor_modules/FaceModule.py
--rw-rw-r--   0 azam      (1000) azam      (1000)        0 2024-03-20 06:22:40.000000 cryptonets_python_sdk-1.3.2/src/cryptonets_python_sdk/factor_modules/__init__.py
-drwxrwxr-x   0 azam      (1000) azam      (1000)        0 2024-05-23 10:37:55.089851 cryptonets_python_sdk-1.3.2/src/cryptonets_python_sdk/handler/
--rw-rw-r--   0 azam      (1000) azam      (1000)        0 2024-03-20 06:22:40.000000 cryptonets_python_sdk-1.3.2/src/cryptonets_python_sdk/handler/__init__.py
-drwxrwxr-x   0 azam      (1000) azam      (1000)        0 2024-05-23 10:37:55.089851 cryptonets_python_sdk-1.3.2/src/cryptonets_python_sdk/handler/lib/
--rw-rw-r--   0 azam      (1000) azam      (1000)        0 2024-03-20 06:22:40.000000 cryptonets_python_sdk-1.3.2/src/cryptonets_python_sdk/handler/lib/__init__.py
--rw-rw-r--   0 azam      (1000) azam      (1000)    45211 2024-05-16 12:12:36.000000 cryptonets_python_sdk-1.3.2/src/cryptonets_python_sdk/handler/nativeMethods.py
-drwxrwxr-x   0 azam      (1000) azam      (1000)        0 2024-05-23 10:37:55.089851 cryptonets_python_sdk-1.3.2/src/cryptonets_python_sdk/helper/
--rw-rw-r--   0 azam      (1000) azam      (1000)        0 2024-03-20 06:22:40.000000 cryptonets_python_sdk-1.3.2/src/cryptonets_python_sdk/helper/__init__.py
--rw-rw-r--   0 azam      (1000) azam      (1000)     3060 2024-03-20 06:22:40.000000 cryptonets_python_sdk-1.3.2/src/cryptonets_python_sdk/helper/decorators.py
--rw-rw-r--   0 azam      (1000) azam      (1000)     3383 2024-04-24 15:45:32.000000 cryptonets_python_sdk-1.3.2/src/cryptonets_python_sdk/helper/messages.py
-drwxrwxr-x   0 azam      (1000) azam      (1000)        0 2024-05-23 10:37:55.089851 cryptonets_python_sdk-1.3.2/src/cryptonets_python_sdk/helper/result_objects/
--rw-rw-r--   0 azam      (1000) azam      (1000)        0 2024-03-20 06:22:40.000000 cryptonets_python_sdk-1.3.2/src/cryptonets_python_sdk/helper/result_objects/__init__.py
--rw-rw-r--   0 azam      (1000) azam      (1000)     3293 2024-04-08 11:44:23.000000 cryptonets_python_sdk-1.3.2/src/cryptonets_python_sdk/helper/result_objects/compareResult.py
--rw-rw-r--   0 azam      (1000) azam      (1000)      664 2024-03-20 06:22:40.000000 cryptonets_python_sdk-1.3.2/src/cryptonets_python_sdk/helper/result_objects/deleteResult.py
--rw-rw-r--   0 azam      (1000) azam      (1000)     2946 2024-03-20 07:33:12.000000 cryptonets_python_sdk-1.3.2/src/cryptonets_python_sdk/helper/result_objects/enrollPredictResult.py
--rw-rw-r--   0 azam      (1000) azam      (1000)     1575 2024-03-20 06:22:40.000000 cryptonets_python_sdk-1.3.2/src/cryptonets_python_sdk/helper/result_objects/faceObjectResult.py
--rw-rw-r--   0 azam      (1000) azam      (1000)     1463 2024-03-20 06:22:40.000000 cryptonets_python_sdk-1.3.2/src/cryptonets_python_sdk/helper/result_objects/faceValidationResult.py
--rw-rw-r--   0 azam      (1000) azam      (1000)     2228 2024-03-20 06:22:40.000000 cryptonets_python_sdk-1.3.2/src/cryptonets_python_sdk/helper/result_objects/isoFaceResult.py
--rw-rw-r--   0 azam      (1000) azam      (1000)     4476 2024-04-24 15:45:32.000000 cryptonets_python_sdk-1.3.2/src/cryptonets_python_sdk/helper/utils.py
-drwxrwxr-x   0 azam      (1000) azam      (1000)        0 2024-05-23 10:37:55.089851 cryptonets_python_sdk-1.3.2/src/cryptonets_python_sdk/settings/
--rw-rw-r--   0 azam      (1000) azam      (1000)        0 2024-03-20 06:22:40.000000 cryptonets_python_sdk-1.3.2/src/cryptonets_python_sdk/settings/__init__.py
--rw-rw-r--   0 azam      (1000) azam      (1000)      239 2024-03-20 06:22:40.000000 cryptonets_python_sdk-1.3.2/src/cryptonets_python_sdk/settings/cacheType.py
--rw-rw-r--   0 azam      (1000) azam      (1000)    17666 2024-05-23 10:35:08.000000 cryptonets_python_sdk-1.3.2/src/cryptonets_python_sdk/settings/configuration.py
--rw-rw-r--   0 azam      (1000) azam      (1000)      298 2024-03-20 06:22:40.000000 cryptonets_python_sdk-1.3.2/src/cryptonets_python_sdk/settings/loggingLevel.py
--rw-rw-r--   0 azam      (1000) azam      (1000)      113 2024-04-12 17:30:20.000000 cryptonets_python_sdk-1.3.2/src/cryptonets_python_sdk/settings/supportedPlatforms.py
-drwxrwxr-x   0 azam      (1000) azam      (1000)        0 2024-05-23 10:37:55.089851 cryptonets_python_sdk-1.3.2/src/cryptonets_python_sdk.egg-info/
--rw-rw-r--   0 azam      (1000) azam      (1000)     3625 2024-05-23 10:37:54.000000 cryptonets_python_sdk-1.3.2/src/cryptonets_python_sdk.egg-info/PKG-INFO
--rw-rw-r--   0 azam      (1000) azam      (1000)     1544 2024-05-23 10:37:55.000000 cryptonets_python_sdk-1.3.2/src/cryptonets_python_sdk.egg-info/SOURCES.txt
--rw-rw-r--   0 azam      (1000) azam      (1000)        1 2024-05-23 10:37:54.000000 cryptonets_python_sdk-1.3.2/src/cryptonets_python_sdk.egg-info/dependency_links.txt
--rw-rw-r--   0 azam      (1000) azam      (1000)       48 2024-05-23 10:37:54.000000 cryptonets_python_sdk-1.3.2/src/cryptonets_python_sdk.egg-info/requires.txt
--rw-rw-r--   0 azam      (1000) azam      (1000)       22 2024-05-23 10:37:54.000000 cryptonets_python_sdk-1.3.2/src/cryptonets_python_sdk.egg-info/top_level.txt
-drwxrwxr-x   0 azam      (1000) azam      (1000)        0 2024-05-23 10:37:55.093851 cryptonets_python_sdk-1.3.2/tests/
--rw-rw-r--   0 azam      (1000) azam      (1000)    19957 2024-04-15 21:47:15.000000 cryptonets_python_sdk-1.3.2/tests/test.py
--rw-rw-r--   0 azam      (1000) azam      (1000)     8913 2024-03-20 06:22:40.000000 cryptonets_python_sdk-1.3.2/tests/test_suite.py
+drwxrwxr-x   0 azam      (1000) azam      (1000)        0 2024-05-29 13:21:31.194344 cryptonets_python_sdk-1.3.3/
+-rw-rw-r--   0 azam      (1000) azam      (1000)        0 2023-09-26 12:09:24.000000 cryptonets_python_sdk-1.3.3/LICENSE
+-rw-rw-r--   0 azam      (1000) azam      (1000)       28 2023-09-26 12:09:24.000000 cryptonets_python_sdk-1.3.3/MANIFEST.in
+-rw-rw-r--   0 azam      (1000) azam      (1000)     3625 2024-05-29 13:21:31.194344 cryptonets_python_sdk-1.3.3/PKG-INFO
+-rw-rw-r--   0 azam      (1000) azam      (1000)     2511 2024-03-20 06:22:40.000000 cryptonets_python_sdk-1.3.3/README.md
+-rw-rw-r--   0 azam      (1000) azam      (1000)       38 2024-05-29 13:21:31.194344 cryptonets_python_sdk-1.3.3/setup.cfg
+-rw-rw-r--   0 azam      (1000) azam      (1000)     3798 2024-05-29 13:19:59.000000 cryptonets_python_sdk-1.3.3/setup.py
+drwxrwxr-x   0 azam      (1000) azam      (1000)        0 2024-05-29 13:21:31.190344 cryptonets_python_sdk-1.3.3/src/
+drwxrwxr-x   0 azam      (1000) azam      (1000)        0 2024-05-29 13:21:31.194344 cryptonets_python_sdk-1.3.3/src/cryptonets_python_sdk/
+-rw-rw-r--   0 azam      (1000) azam      (1000)        0 2024-03-20 06:22:40.000000 cryptonets_python_sdk-1.3.3/src/cryptonets_python_sdk/__init__.py
+-rw-rw-r--   0 azam      (1000) azam      (1000)    34014 2024-05-29 13:19:59.000000 cryptonets_python_sdk-1.3.3/src/cryptonets_python_sdk/factor.py
+drwxrwxr-x   0 azam      (1000) azam      (1000)        0 2024-05-29 13:21:31.194344 cryptonets_python_sdk-1.3.3/src/cryptonets_python_sdk/factor_modules/
+-rw-rw-r--   0 azam      (1000) azam      (1000)    22181 2024-05-29 13:19:59.000000 cryptonets_python_sdk-1.3.3/src/cryptonets_python_sdk/factor_modules/FaceModule.py
+-rw-rw-r--   0 azam      (1000) azam      (1000)        0 2024-03-20 06:22:40.000000 cryptonets_python_sdk-1.3.3/src/cryptonets_python_sdk/factor_modules/__init__.py
+drwxrwxr-x   0 azam      (1000) azam      (1000)        0 2024-05-29 13:21:31.194344 cryptonets_python_sdk-1.3.3/src/cryptonets_python_sdk/handler/
+-rw-rw-r--   0 azam      (1000) azam      (1000)        0 2024-03-20 06:22:40.000000 cryptonets_python_sdk-1.3.3/src/cryptonets_python_sdk/handler/__init__.py
+drwxrwxr-x   0 azam      (1000) azam      (1000)        0 2024-05-29 13:21:31.194344 cryptonets_python_sdk-1.3.3/src/cryptonets_python_sdk/handler/lib/
+-rw-rw-r--   0 azam      (1000) azam      (1000)        0 2024-03-20 06:22:40.000000 cryptonets_python_sdk-1.3.3/src/cryptonets_python_sdk/handler/lib/__init__.py
+-rw-rw-r--   0 azam      (1000) azam      (1000)    45250 2024-05-29 13:19:59.000000 cryptonets_python_sdk-1.3.3/src/cryptonets_python_sdk/handler/nativeMethods.py
+drwxrwxr-x   0 azam      (1000) azam      (1000)        0 2024-05-29 13:21:31.194344 cryptonets_python_sdk-1.3.3/src/cryptonets_python_sdk/helper/
+-rw-rw-r--   0 azam      (1000) azam      (1000)        0 2024-03-20 06:22:40.000000 cryptonets_python_sdk-1.3.3/src/cryptonets_python_sdk/helper/__init__.py
+-rw-rw-r--   0 azam      (1000) azam      (1000)     3060 2024-03-20 06:22:40.000000 cryptonets_python_sdk-1.3.3/src/cryptonets_python_sdk/helper/decorators.py
+-rw-rw-r--   0 azam      (1000) azam      (1000)     4000 2024-05-29 13:19:59.000000 cryptonets_python_sdk-1.3.3/src/cryptonets_python_sdk/helper/messages.py
+drwxrwxr-x   0 azam      (1000) azam      (1000)        0 2024-05-29 13:21:31.194344 cryptonets_python_sdk-1.3.3/src/cryptonets_python_sdk/helper/result_objects/
+-rw-rw-r--   0 azam      (1000) azam      (1000)        0 2024-03-20 06:22:40.000000 cryptonets_python_sdk-1.3.3/src/cryptonets_python_sdk/helper/result_objects/__init__.py
+-rw-rw-r--   0 azam      (1000) azam      (1000)      995 2024-05-29 13:19:59.000000 cryptonets_python_sdk-1.3.3/src/cryptonets_python_sdk/helper/result_objects/antispoofCheckResult.py
+-rw-rw-r--   0 azam      (1000) azam      (1000)     3293 2024-04-08 11:44:23.000000 cryptonets_python_sdk-1.3.3/src/cryptonets_python_sdk/helper/result_objects/compareResult.py
+-rw-rw-r--   0 azam      (1000) azam      (1000)      664 2024-03-20 06:22:40.000000 cryptonets_python_sdk-1.3.3/src/cryptonets_python_sdk/helper/result_objects/deleteResult.py
+-rw-rw-r--   0 azam      (1000) azam      (1000)     2946 2024-03-20 07:33:12.000000 cryptonets_python_sdk-1.3.3/src/cryptonets_python_sdk/helper/result_objects/enrollPredictResult.py
+-rw-rw-r--   0 azam      (1000) azam      (1000)     1575 2024-03-20 06:22:40.000000 cryptonets_python_sdk-1.3.3/src/cryptonets_python_sdk/helper/result_objects/faceObjectResult.py
+-rw-rw-r--   0 azam      (1000) azam      (1000)     1463 2024-03-20 06:22:40.000000 cryptonets_python_sdk-1.3.3/src/cryptonets_python_sdk/helper/result_objects/faceValidationResult.py
+-rw-rw-r--   0 azam      (1000) azam      (1000)     2228 2024-03-20 06:22:40.000000 cryptonets_python_sdk-1.3.3/src/cryptonets_python_sdk/helper/result_objects/isoFaceResult.py
+-rw-rw-r--   0 azam      (1000) azam      (1000)     4476 2024-04-24 15:45:32.000000 cryptonets_python_sdk-1.3.3/src/cryptonets_python_sdk/helper/utils.py
+drwxrwxr-x   0 azam      (1000) azam      (1000)        0 2024-05-29 13:21:31.194344 cryptonets_python_sdk-1.3.3/src/cryptonets_python_sdk/settings/
+-rw-rw-r--   0 azam      (1000) azam      (1000)        0 2024-03-20 06:22:40.000000 cryptonets_python_sdk-1.3.3/src/cryptonets_python_sdk/settings/__init__.py
+-rw-rw-r--   0 azam      (1000) azam      (1000)      239 2024-03-20 06:22:40.000000 cryptonets_python_sdk-1.3.3/src/cryptonets_python_sdk/settings/cacheType.py
+-rw-rw-r--   0 azam      (1000) azam      (1000)    17666 2024-05-23 10:35:08.000000 cryptonets_python_sdk-1.3.3/src/cryptonets_python_sdk/settings/configuration.py
+-rw-rw-r--   0 azam      (1000) azam      (1000)      298 2024-03-20 06:22:40.000000 cryptonets_python_sdk-1.3.3/src/cryptonets_python_sdk/settings/loggingLevel.py
+-rw-rw-r--   0 azam      (1000) azam      (1000)      113 2024-04-12 17:30:20.000000 cryptonets_python_sdk-1.3.3/src/cryptonets_python_sdk/settings/supportedPlatforms.py
+drwxrwxr-x   0 azam      (1000) azam      (1000)        0 2024-05-29 13:21:31.194344 cryptonets_python_sdk-1.3.3/src/cryptonets_python_sdk.egg-info/
+-rw-rw-r--   0 azam      (1000) azam      (1000)     3625 2024-05-29 13:21:31.000000 cryptonets_python_sdk-1.3.3/src/cryptonets_python_sdk.egg-info/PKG-INFO
+-rw-rw-r--   0 azam      (1000) azam      (1000)     1616 2024-05-29 13:21:31.000000 cryptonets_python_sdk-1.3.3/src/cryptonets_python_sdk.egg-info/SOURCES.txt
+-rw-rw-r--   0 azam      (1000) azam      (1000)        1 2024-05-29 13:21:31.000000 cryptonets_python_sdk-1.3.3/src/cryptonets_python_sdk.egg-info/dependency_links.txt
+-rw-rw-r--   0 azam      (1000) azam      (1000)       48 2024-05-29 13:21:31.000000 cryptonets_python_sdk-1.3.3/src/cryptonets_python_sdk.egg-info/requires.txt
+-rw-rw-r--   0 azam      (1000) azam      (1000)       22 2024-05-29 13:21:31.000000 cryptonets_python_sdk-1.3.3/src/cryptonets_python_sdk.egg-info/top_level.txt
+drwxrwxr-x   0 azam      (1000) azam      (1000)        0 2024-05-29 13:21:31.194344 cryptonets_python_sdk-1.3.3/tests/
+-rw-rw-r--   0 azam      (1000) azam      (1000)    19957 2024-04-15 21:47:15.000000 cryptonets_python_sdk-1.3.3/tests/test.py
+-rw-rw-r--   0 azam      (1000) azam      (1000)     8913 2024-03-20 06:22:40.000000 cryptonets_python_sdk-1.3.3/tests/test_suite.py
```

### Comparing `cryptonets_python_sdk-1.3.2/PKG-INFO` & `cryptonets_python_sdk-1.3.3/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: cryptonets_python_sdk
-Version: 1.3.2
+Version: 1.3.3
 Summary: Cryptonets SDK Library for Python
 Home-page: https://privateid.com/
 Author: Private Identity
 Author-email: support@private.id
 Project-URL: Bug Reports, https://github.com/prividentity/cryptonets-python-sdk/issues
 Project-URL: Source, https://github.com/prividentity/cryptonets-python-sdk
 Project-URL: Documentation, https://docs.private.id/cryptonets-python-sdk/index.html
```

### Comparing `cryptonets_python_sdk-1.3.2/README.md` & `cryptonets_python_sdk-1.3.3/README.md`

 * *Files identical despite different names*

### Comparing `cryptonets_python_sdk-1.3.2/setup.py` & `cryptonets_python_sdk-1.3.3/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -32,15 +32,15 @@
 @author: Private Identity
 """
 NAME = "cryptonets_python_sdk"
 DESCRIPTION = "Cryptonets SDK Library for Python"
 AUTHOR = "Private Identity"
 AUTHOR_EMAIL = "support@private.id"
 URL = "https://privateid.com/"
-VERSION = "1.3.2"
+VERSION = "1.3.3"
 REQUIRES = ["numpy >= 1.21.0", "pillow >= 9.1.0","boto3","tqdm","exifread"]
 
 LONG_DESCRIPTION = ""
 if os.path.exists("./README.md"):
     with open("README.md", encoding="utf-8") as fp:
         LONG_DESCRIPTION = fp.read()
 setup(
```

### Comparing `cryptonets_python_sdk-1.3.2/src/cryptonets_python_sdk/factor.py` & `cryptonets_python_sdk-1.3.3/src/cryptonets_python_sdk/factor.py`

 * *Files 2% similar despite different names*

```diff
@@ -11,14 +11,15 @@
 from .factor_modules.FaceModule import Face
 from .helper.decorators import Singleton
 from .helper.messages import Message
 from .helper.result_objects.compareResult import FaceCompareResult
 from .helper.result_objects.deleteResult import FaceDeleteResult
 from .helper.result_objects.enrollPredictResult import FaceEnrollPredictResult
 from .helper.result_objects.faceValidationResult import FaceValidationResult
+from .helper.result_objects.antispoofCheckResult import AntispoofCheckResult
 from .helper.result_objects.isoFaceResult import ISOFaceResult
 from .helper.utils import image_path_to_array
 from .settings.cacheType import CacheType
 from .settings.configuration import ConfigObject, PARAMETERS
 from .settings.loggingLevel import LoggingLevel
 from .settings.supportedPlatforms import SupportedPlatforms
 
@@ -817,14 +818,85 @@
             )
         except Exception as e:
             print("Oops: {}\nTrace: {}".format(e, traceback.format_exc()))
             print(
                 "Issue Tracker:: \nhttps://github.com/prividentity/cryptonets-python-sdk/issues"
             )
             return FaceCompareResult(message=self.message.EXCEPTION_ERROR_COMPARE)
+    def antispoof_check(
+        self,
+        image_path: str = None,
+        image_data: np.array = None,
+        config: ConfigObject = None,
+    ) -> AntispoofCheckResult:
+        """Check if the image is spoofed or not
+
+        Parameters
+        ----------
+        image_path
+            Directory path to the image file
+
+        config (Optional)
+            Additional configuration parameters for the operation
+
+        image_data (Optional)
+            Image data in numpy RGB format
+
+        Returns
+        -------
+        AntispoofCheckResult
+
+            status: int [0 if successful -1 if unsuccessful]
+            
+            message: str [Message from the operation]
+
+            is_antispoof: bool [True if spoofed, False if not spoofed]
+        
+        """
+        try:
+            if (
+                config is not None
+                and PARAMETERS.INPUT_IMAGE_FORMAT in config.config_param
+            ):
+                input_format = config.config_param[PARAMETERS.INPUT_IMAGE_FORMAT]
+            elif (
+                self.config is not None
+                and PARAMETERS.INPUT_IMAGE_FORMAT in self.config.config_param
+            ):
+                input_format = self.config.config_param[PARAMETERS.INPUT_IMAGE_FORMAT]
+            else:
+                input_format = "rgb"
+            if (image_path is not None and image_data is not None) or (
+                image_path is None and image_data is None
+            ):
+                return AntispoofCheckResult(
+                    message="Specify either image_path or image_data"
+                )
+            img_data = None
+            if image_data is not None:
+                if not isinstance(image_data, np.ndarray):
+                    return AntispoofCheckResult(
+                        message="Required numpy array in RGB/RGBA/BGR format"
+                    )
+                img_data = image_data
+            if image_path is not None and len(image_path) > 0:
+                if not os.path.exists(image_path):
+                    return AntispoofCheckResult(message=self.message.get_message(101))
+                img_data = image_path_to_array(image_path, input_format=input_format)
+            if img_data is None:
+                return AntispoofCheckResult(message=self.message.ANTISPOOF_CHECK_ERROR)
+            return self.face_factor.antispoof_check(
+                image_data=img_data, config_object=config
+            )
+        except Exception as e:
+            print("Oops: {}\nTrace: {}".format(e, traceback.format_exc()))
+            print(
+                "Issue Tracker:: \nhttps://github.com/prividentity/cryptonets-python-sdk/issues"
+            )
+            return AntispoofCheckResult(message=self.message.ANTISPOOF_CHECK_ERROR)
 
     @property
     def api_key(self) -> str:
         return self._api_key
 
     @property
     def server_url(self) -> str:
```

### Comparing `cryptonets_python_sdk-1.3.2/src/cryptonets_python_sdk/factor_modules/FaceModule.py` & `cryptonets_python_sdk-1.3.3/src/cryptonets_python_sdk/factor_modules/FaceModule.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,20 +1,22 @@
 import string
 import traceback
-from typing import Union, List
+
+from typing import Union, List, Optional
 import numpy as np
 import json
 from ..handler.nativeMethods import NativeMethods
 from ..helper.decorators import Singleton
 from ..helper.messages import Message
 from ..helper.result_objects.compareResult import FaceCompareResult
 from ..helper.result_objects.deleteResult import FaceDeleteResult
 from ..helper.result_objects.enrollPredictResult import FaceEnrollPredictResult
 from ..helper.result_objects.faceValidationResult import FaceValidationResult
 from ..helper.result_objects.isoFaceResult import ISOFaceResult
+from ..helper.result_objects.antispoofCheckResult import AntispoofCheckResult
 from ..helper.utils import FaceValidationCode
 from ..settings.cacheType import CacheType
 from ..settings.configuration import ConfigObject
 from ..settings.loggingLevel import LoggingLevel
 
 
 class Face(metaclass=Singleton):
@@ -199,18 +201,21 @@
         face_data: np.array,
         doc_data: np.array,
         config_object: ConfigObject = None,
     ) -> FaceCompareResult:
         try:
             processed_document=self._doc_scan_face(image_data=doc_data)
             if processed_document.get("doc_face",{}).get("document_data",{}).get("document_validation_status",-1)!=0:
-                 return FaceCompareResult(message= processed_document.get("doc_face",{}).get("document_data",{}).get("status_message","Something went wrong while processing document image"))
+                 if processed_document.get("doc_face",{}).get("document_data",{}).get("status_message","Unable to detect face in the document.").strip()=="":
+                        return FaceCompareResult(message="Unable to detect face in the document.")
+                 return FaceCompareResult(message= processed_document.get("doc_face",{}).get("document_data",{}).get("status_message","Unable to detect face in the document."))
         
             cropped_face_array = processed_document.get("doc_face",{}).get("cropped_face")
-            
+            if cropped_face_array is None:
+                 return FaceCompareResult(message= "Unable to detect face in the document.")
             if cropped_face_array is not None:
             
                 face_compare_json_data_all = self.face_factor_processor.compare_files(
                     face_data, processed_document.get("doc_face",{}).get("cropped_face"), config_object=config_object
                 )
             else:
                 return FaceCompareResult(message=self.message.EXCEPTION_ERROR_COMPARE)
@@ -406,7 +411,31 @@
                 status=json_data.get("status", -1),
                 message=json_data.get("message", "OK"),
             )
 
         except Exception as e:
             print(e, traceback.format_exc())
             return ISOFaceResult(message=self.message.EXCEPTION_ERROR_GET_ISO_FACE)
+   
+    def antispoof_check(self, image_data: np.array, config_object: Optional[ConfigObject] = None) -> AntispoofCheckResult:
+            try:
+                # Call the processor to check for antispoofing
+                json_data = self.face_factor_processor.antispoof_check(image_data, config_object=config_object)
+
+                # Validate response
+                if json_data is None:
+                    return AntispoofCheckResult(status=-100, message="No response from antispoofing processor.", is_antispoof=False)
+
+                # Check if there is an error in processing
+                if json_data.get("call_status", {}).get("return_status",0) != 0:
+                    error_message = json_data.get("call_status", {}).get("return_message", "Error during antispoofing check.")
+                    return AntispoofCheckResult(status=json_data.get("call_status", {}).get("return_status"), message=error_message, is_antispoof=False)
+                
+                if json_data.get("antispoofing", 0) in [-1,-2,-3,-4,-5,-6,-100]:
+                    return AntispoofCheckResult(status=json_data.get("antispoofing", 0), message=self.message.APP_MESSAGES.get(json_data.get("antispoofing", 0), "Error during antispoofing check."), is_antispoof=False)
+                # Check antispoofing result
+                is_spoof_detected = json_data.get("antispoofing", 0) == 1
+                return AntispoofCheckResult(status=0, message="No spoofing detected." if not is_spoof_detected else "Spoofing detected.", is_antispoof=is_spoof_detected)
+
+            except Exception as e:
+                print("Exception occurred:", e, traceback.format_exc())
+                return AntispoofCheckResult(status=-100, message="Exception occurred during antispoofing check.", is_antispoof=False)
```

### Comparing `cryptonets_python_sdk-1.3.2/src/cryptonets_python_sdk/handler/nativeMethods.py` & `cryptonets_python_sdk-1.3.3/src/cryptonets_python_sdk/handler/nativeMethods.py`

 * *Files 1% similar despite different names*

```diff
@@ -190,21 +190,21 @@
         c_config_param = c_char_p(bytes(config_json, "utf-8"))
         c_config_param_len = c_int(len(config_json))
 
         return_type = self._spl_so_face.privid_initialize_session(
             c_config_param, c_config_param_len,
             byref(self._spl_so_face.handle))
 
-        # self._spl_so_face.privid_get_version.argtypes = []
-        # self._spl_so_face.privid_get_version.restype = c_char_p
+        self._spl_so_face.privid_get_version.argtypes = []
+        self._spl_so_face.privid_get_version.restype = c_char_p
 
-        # # Call the function and decode the byte string to print
-        # version_bytes = self._spl_so_face.privid_get_version()
-        # version_str = version_bytes.decode('utf-8')  # Decoding to string
-        # print(version_str)
+        # Call the function and decode the byte string to print
+        version_bytes = self._spl_so_face.privid_get_version()
+        version_str = version_bytes.decode('utf-8')  # Decoding to string
+        print(version_str)
 
         if not return_type:
             raise Exception("Wrong API_KEY or Server URL.")
         ##############################################################################################
 
         ##############################################################################################
         # (ok) PRIVID_API_ATTRIB bool privid_set_configuration(void *session_ptr, const char *user_config,
@@ -855,35 +855,37 @@
                 output = json.loads(output_json_str)
                 return output
             return False
         except Exception as e:
             print("Error :", e)
             return False
 
-    def antispoofing(
+    def antispoof_check(
         self, image_data: np.array, config_object: ConfigObject = None
     ) -> Any:
         try:
-            img = image_data
-            im_width = img.shape[1]
-            im_height = img.shape[0]
+            img_data = image_data
+            im_height, im_width, im_channel = img_data.shape
 
-            p_buffer_images_in = img.flatten()
+            p_buffer_images_in = img_data
             c_p_buffer_images_in = p_buffer_images_in.ctypes.data_as(POINTER(c_uint8))
+            im_size = im_height * im_width * im_channel
 
             c_result = c_char_p()
             c_result_len = c_int()
+            
             if config_object and config_object.get_config_param():
                 c_config_param = c_char_p(
                     bytes(config_object.get_config_param(), "utf-8")
                 )
                 c_config_param_len = c_int(len(config_object.get_config_param()))
             else:
-                c_config_param = c_char_p(bytes("", "utf-8"))
-                c_config_param_len = c_int(0)
+                c_config_param = c_char_p(bytes(json.dumps({}), "utf-8"))
+                c_config_param_len = c_int(2)
+
             self._spl_so_face.privid_anti_spoofing(
                 self._spl_so_face.handle,
                 c_p_buffer_images_in,
                 c_int(im_width),
                 c_int(im_height),
                 c_config_param,
                 c_config_param_len,
@@ -893,19 +895,17 @@
 
             if not c_result.value or not c_result_len.value:
                 raise Exception(
                     "Something went wrong. Couldn't process the image for antispoofing API. "
                 )
             output_json = c_result.value[: c_result_len.value].decode()
             self._spl_so_face.privid_free_char_buffer(c_result)
-
             output = json.loads(output_json)
             return output
         except Exception as e:
-            print(e)
             return False
     
     def doc_scan_face(self, image_data: np.array, config_object: ConfigObject = None) -> Any:
         try:
             img = image_data
             im_width = img.shape[1]
             im_height = img.shape[0]
```

### Comparing `cryptonets_python_sdk-1.3.2/src/cryptonets_python_sdk/helper/decorators.py` & `cryptonets_python_sdk-1.3.3/src/cryptonets_python_sdk/helper/decorators.py`

 * *Files identical despite different names*

### Comparing `cryptonets_python_sdk-1.3.2/src/cryptonets_python_sdk/helper/messages.py` & `cryptonets_python_sdk-1.3.3/src/cryptonets_python_sdk/helper/messages.py`

 * *Files 13% similar despite different names*

```diff
@@ -3,23 +3,30 @@
         self.IS_VALID_ERROR = "Unknown error while validating the image"
         self.AGE_ESTIMATE_ERROR = "Unknown error while predicting the age."
         self.EXCEPTION_ERROR_ENROLL = "Something went wrong while doing enroll."
         self.EXCEPTION_ERROR_GET_ISO_FACE = "ISO face validation failed."
         self.EXCEPTION_ERROR_PREDICT = "Something went wrong while doing predict."
         self.EXCEPTION_ERROR_DELETE = "Something went wrong while doing delete."
         self.EXCEPTION_ERROR_COMPARE = "Something went wrong while doing compare."
+        self.EXCEPTION_ERROR_ANTISPOOF_CHECK = "Something went wrong while doing antispoof."
         self.ENROLL_PROCESSED = (
             "Enroll request successfully processed, Waiting for server response."
         )
         self.PREDICT_PROCESSED = (
             "Predict request successfully processed, Waiting for server response."
         )
 
         self.APP_MESSAGES = {
-             -1: "Invalid image.",
+            -100:"	Error occurred during the antispoofing.",
+             -6: "Antispoofing detection was not performed and was skipped.",
+            -5: "A grayscale image has been detected, which may indicate a spoof attempt.",
+            -4: "Invalid face detected, unable to apply antispoofing procedures.",
+            -3: "Face too close to the edge; please center your face in the image.",
+            -2: "Mobile phone detected in the vicinity, which may indicate a spoof attempt.",
+             -1: "Invalid image, No face detected in the image.",
             0: "Valid face.",
             1: "Error Description: Image spoof detected. Please provide a live facial image.",
             2: "Error Description: Video spoof detected. Please provide a live facial image.",
             3: "Error Description: Face too close to the camera. Please move back.",
             4: "Error Description: Face too far from the camera.",
             5: "Error Description: Face too close to the right edge of the frame.",
             6: "Error Description: Face too close to the left edge of the frame.",
```

### Comparing `cryptonets_python_sdk-1.3.2/src/cryptonets_python_sdk/helper/result_objects/compareResult.py` & `cryptonets_python_sdk-1.3.3/src/cryptonets_python_sdk/helper/result_objects/compareResult.py`

 * *Files identical despite different names*

### Comparing `cryptonets_python_sdk-1.3.2/src/cryptonets_python_sdk/helper/result_objects/deleteResult.py` & `cryptonets_python_sdk-1.3.3/src/cryptonets_python_sdk/helper/result_objects/deleteResult.py`

 * *Files identical despite different names*

### Comparing `cryptonets_python_sdk-1.3.2/src/cryptonets_python_sdk/helper/result_objects/enrollPredictResult.py` & `cryptonets_python_sdk-1.3.3/src/cryptonets_python_sdk/helper/result_objects/enrollPredictResult.py`

 * *Files identical despite different names*

### Comparing `cryptonets_python_sdk-1.3.2/src/cryptonets_python_sdk/helper/result_objects/faceObjectResult.py` & `cryptonets_python_sdk-1.3.3/src/cryptonets_python_sdk/helper/result_objects/faceObjectResult.py`

 * *Files identical despite different names*

### Comparing `cryptonets_python_sdk-1.3.2/src/cryptonets_python_sdk/helper/result_objects/faceValidationResult.py` & `cryptonets_python_sdk-1.3.3/src/cryptonets_python_sdk/helper/result_objects/faceValidationResult.py`

 * *Files identical despite different names*

### Comparing `cryptonets_python_sdk-1.3.2/src/cryptonets_python_sdk/helper/result_objects/isoFaceResult.py` & `cryptonets_python_sdk-1.3.3/src/cryptonets_python_sdk/helper/result_objects/isoFaceResult.py`

 * *Files identical despite different names*

### Comparing `cryptonets_python_sdk-1.3.2/src/cryptonets_python_sdk/helper/utils.py` & `cryptonets_python_sdk-1.3.3/src/cryptonets_python_sdk/helper/utils.py`

 * *Files identical despite different names*

### Comparing `cryptonets_python_sdk-1.3.2/src/cryptonets_python_sdk/settings/configuration.py` & `cryptonets_python_sdk-1.3.3/src/cryptonets_python_sdk/settings/configuration.py`

 * *Files identical despite different names*

### Comparing `cryptonets_python_sdk-1.3.2/src/cryptonets_python_sdk.egg-info/PKG-INFO` & `cryptonets_python_sdk-1.3.3/src/cryptonets_python_sdk.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: cryptonets-python-sdk
-Version: 1.3.2
+Version: 1.3.3
 Summary: Cryptonets SDK Library for Python
 Home-page: https://privateid.com/
 Author: Private Identity
 Author-email: support@private.id
 Project-URL: Bug Reports, https://github.com/prividentity/cryptonets-python-sdk/issues
 Project-URL: Source, https://github.com/prividentity/cryptonets-python-sdk
 Project-URL: Documentation, https://docs.private.id/cryptonets-python-sdk/index.html
```

### Comparing `cryptonets_python_sdk-1.3.2/src/cryptonets_python_sdk.egg-info/SOURCES.txt` & `cryptonets_python_sdk-1.3.3/src/cryptonets_python_sdk.egg-info/SOURCES.txt`

 * *Files 2% similar despite different names*

```diff
@@ -15,14 +15,15 @@
 src/cryptonets_python_sdk/handler/nativeMethods.py
 src/cryptonets_python_sdk/handler/lib/__init__.py
 src/cryptonets_python_sdk/helper/__init__.py
 src/cryptonets_python_sdk/helper/decorators.py
 src/cryptonets_python_sdk/helper/messages.py
 src/cryptonets_python_sdk/helper/utils.py
 src/cryptonets_python_sdk/helper/result_objects/__init__.py
+src/cryptonets_python_sdk/helper/result_objects/antispoofCheckResult.py
 src/cryptonets_python_sdk/helper/result_objects/compareResult.py
 src/cryptonets_python_sdk/helper/result_objects/deleteResult.py
 src/cryptonets_python_sdk/helper/result_objects/enrollPredictResult.py
 src/cryptonets_python_sdk/helper/result_objects/faceObjectResult.py
 src/cryptonets_python_sdk/helper/result_objects/faceValidationResult.py
 src/cryptonets_python_sdk/helper/result_objects/isoFaceResult.py
 src/cryptonets_python_sdk/settings/__init__.py
```

### Comparing `cryptonets_python_sdk-1.3.2/tests/test.py` & `cryptonets_python_sdk-1.3.3/tests/test.py`

 * *Files identical despite different names*

### Comparing `cryptonets_python_sdk-1.3.2/tests/test_suite.py` & `cryptonets_python_sdk-1.3.3/tests/test_suite.py`

 * *Files identical despite different names*

