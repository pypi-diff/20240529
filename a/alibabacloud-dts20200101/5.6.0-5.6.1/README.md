# Comparing `tmp/alibabacloud_dts20200101-5.6.0.tar.gz` & `tmp/alibabacloud_dts20200101-5.6.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/alibabacloud_dts20200101-5.6.0.tar", last modified: Thu May  9 17:10:30 2024, max compression
+gzip compressed data, was "dist/alibabacloud_dts20200101-5.6.1.tar", last modified: Wed May 29 17:12:54 2024, max compression
```

## Comparing `alibabacloud_dts20200101-5.6.0.tar` & `alibabacloud_dts20200101-5.6.1.tar`

### file list

```diff
@@ -1,19 +1,19 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-09 17:10:30.000000 alibabacloud_dts20200101-5.6.0/
--rw-r--r--   0 root         (0) root         (0)    10418 2024-05-09 17:10:30.000000 alibabacloud_dts20200101-5.6.0/ChangeLog.md
--rw-r--r--   0 root         (0) root         (0)      600 2024-05-09 17:10:30.000000 alibabacloud_dts20200101-5.6.0/LICENSE
--rw-r--r--   0 root         (0) root         (0)       29 2024-05-09 17:10:30.000000 alibabacloud_dts20200101-5.6.0/MANIFEST.in
--rw-r--r--   0 root         (0) root         (0)     2415 2024-05-09 17:10:30.000000 alibabacloud_dts20200101-5.6.0/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)     1095 2024-05-09 17:10:30.000000 alibabacloud_dts20200101-5.6.0/README-CN.md
--rw-r--r--   0 root         (0) root         (0)     1180 2024-05-09 17:10:30.000000 alibabacloud_dts20200101-5.6.0/README.md
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-09 17:10:30.000000 alibabacloud_dts20200101-5.6.0/alibabacloud_dts20200101/
--rw-r--r--   0 root         (0) root         (0)       21 2024-05-09 17:10:30.000000 alibabacloud_dts20200101-5.6.0/alibabacloud_dts20200101/__init__.py
--rw-r--r--   0 root         (0) root         (0)   610240 2024-05-09 17:10:30.000000 alibabacloud_dts20200101-5.6.0/alibabacloud_dts20200101/client.py
--rw-r--r--   0 root         (0) root         (0)  1720696 2024-05-09 17:10:30.000000 alibabacloud_dts20200101-5.6.0/alibabacloud_dts20200101/models.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-09 17:10:30.000000 alibabacloud_dts20200101-5.6.0/alibabacloud_dts20200101.egg-info/
--rw-r--r--   0 root         (0) root         (0)     2415 2024-05-09 17:10:30.000000 alibabacloud_dts20200101-5.6.0/alibabacloud_dts20200101.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)      420 2024-05-09 17:10:30.000000 alibabacloud_dts20200101-5.6.0/alibabacloud_dts20200101.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2024-05-09 17:10:30.000000 alibabacloud_dts20200101-5.6.0/alibabacloud_dts20200101.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)      316 2024-05-09 17:10:30.000000 alibabacloud_dts20200101-5.6.0/alibabacloud_dts20200101.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)       25 2024-05-09 17:10:30.000000 alibabacloud_dts20200101-5.6.0/alibabacloud_dts20200101.egg-info/top_level.txt
--rw-r--r--   0 root         (0) root         (0)       73 2024-05-09 17:10:30.000000 alibabacloud_dts20200101-5.6.0/setup.cfg
--rw-r--r--   0 root         (0) root         (0)     2816 2024-05-09 17:10:30.000000 alibabacloud_dts20200101-5.6.0/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-29 17:12:54.000000 alibabacloud_dts20200101-5.6.1/
+-rw-r--r--   0 root         (0) root         (0)    10540 2024-05-29 17:12:54.000000 alibabacloud_dts20200101-5.6.1/ChangeLog.md
+-rw-r--r--   0 root         (0) root         (0)      600 2024-05-29 17:12:54.000000 alibabacloud_dts20200101-5.6.1/LICENSE
+-rw-r--r--   0 root         (0) root         (0)       29 2024-05-29 17:12:54.000000 alibabacloud_dts20200101-5.6.1/MANIFEST.in
+-rw-r--r--   0 root         (0) root         (0)     2415 2024-05-29 17:12:54.000000 alibabacloud_dts20200101-5.6.1/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)     1095 2024-05-29 17:12:54.000000 alibabacloud_dts20200101-5.6.1/README-CN.md
+-rw-r--r--   0 root         (0) root         (0)     1180 2024-05-29 17:12:54.000000 alibabacloud_dts20200101-5.6.1/README.md
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-29 17:12:54.000000 alibabacloud_dts20200101-5.6.1/alibabacloud_dts20200101/
+-rw-r--r--   0 root         (0) root         (0)       21 2024-05-29 17:12:54.000000 alibabacloud_dts20200101-5.6.1/alibabacloud_dts20200101/__init__.py
+-rw-r--r--   0 root         (0) root         (0)   681248 2024-05-29 17:12:54.000000 alibabacloud_dts20200101-5.6.1/alibabacloud_dts20200101/client.py
+-rw-r--r--   0 root         (0) root         (0)  1740699 2024-05-29 17:12:54.000000 alibabacloud_dts20200101-5.6.1/alibabacloud_dts20200101/models.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-29 17:12:54.000000 alibabacloud_dts20200101-5.6.1/alibabacloud_dts20200101.egg-info/
+-rw-r--r--   0 root         (0) root         (0)     2415 2024-05-29 17:12:54.000000 alibabacloud_dts20200101-5.6.1/alibabacloud_dts20200101.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)      420 2024-05-29 17:12:54.000000 alibabacloud_dts20200101-5.6.1/alibabacloud_dts20200101.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2024-05-29 17:12:54.000000 alibabacloud_dts20200101-5.6.1/alibabacloud_dts20200101.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)      316 2024-05-29 17:12:54.000000 alibabacloud_dts20200101-5.6.1/alibabacloud_dts20200101.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)       25 2024-05-29 17:12:54.000000 alibabacloud_dts20200101-5.6.1/alibabacloud_dts20200101.egg-info/top_level.txt
+-rw-r--r--   0 root         (0) root         (0)       73 2024-05-29 17:12:54.000000 alibabacloud_dts20200101-5.6.1/setup.cfg
+-rw-r--r--   0 root         (0) root         (0)     2816 2024-05-29 17:12:54.000000 alibabacloud_dts20200101-5.6.1/setup.py
```

### Comparing `alibabacloud_dts20200101-5.6.0/ChangeLog.md` & `alibabacloud_dts20200101-5.6.1/ChangeLog.md`

 * *Files 1% similar despite different names*

```diff
@@ -1,7 +1,12 @@
+2024-05-09 Version: 5.6.0
+- Support API DescribeSyncStatus.
+- Update API ModifyDtsJobEndpoint: add param ModifyAccount.
+
+
 2024-04-25 Version: 5.5.5
 - Update API CreateReverseDtsJob: add param ShardPassword.
 - Update API CreateReverseDtsJob: add param ShardUsername.
 - Update API ModifyDtsJobEndpoint: add param EndpointRegionId.
 - Update API ModifyDtsJobEndpoint: update param RegionId.
```

### Comparing `alibabacloud_dts20200101-5.6.0/LICENSE` & `alibabacloud_dts20200101-5.6.1/LICENSE`

 * *Files identical despite different names*

### Comparing `alibabacloud_dts20200101-5.6.0/PKG-INFO` & `alibabacloud_dts20200101-5.6.1/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: alibabacloud_dts20200101
-Version: 5.6.0
+Version: 5.6.1
 Summary: Alibaba Cloud Data Transmission (20200101) SDK Library for Python
 Home-page: https://github.com/aliyun/alibabacloud-python-sdk
 Author: Alibaba Cloud SDK
 Author-email: sdk-team@alibabacloud.com
 License: Apache License 2.0
 Description: English | [简体中文](README-CN.md)
         ![](https://aliyunsdk-pages.alicdn.com/icons/AlibabaCloud.svg)
```

### Comparing `alibabacloud_dts20200101-5.6.0/README-CN.md` & `alibabacloud_dts20200101-5.6.1/README-CN.md`

 * *Files identical despite different names*

### Comparing `alibabacloud_dts20200101-5.6.0/README.md` & `alibabacloud_dts20200101-5.6.1/README.md`

 * *Files identical despite different names*

### Comparing `alibabacloud_dts20200101-5.6.0/alibabacloud_dts20200101/client.py` & `alibabacloud_dts20200101-5.6.1/alibabacloud_dts20200101/client.py`

 * *Files 8% similar despite different names*

```diff
@@ -9,17 +9,17 @@
 from alibabacloud_endpoint_util.client import Client as EndpointUtilClient
 from alibabacloud_dts20200101 import models as dts_20200101_models
 from alibabacloud_tea_util import models as util_models
 from alibabacloud_openapi_util.client import Client as OpenApiUtilClient
 from alibabacloud_openplatform20191219.client import Client as OpenPlatformClient
 from alibabacloud_openplatform20191219 import models as open_platform_models
 from alibabacloud_oss_sdk import models as oss_models
+from alibabacloud_oss_sdk.client import Client as OSSClient
 from alibabacloud_tea_fileform import models as file_form_models
 from alibabacloud_oss_util import models as ossutil_models
-from alibabacloud_oss_sdk.client import Client as OSSClient
 
 
 class Client(OpenApiClient):
     """
     *\
     """
     def __init__(
@@ -106,15 +106,17 @@
 
     def configure_dts_job_with_options(
         self,
         request: dts_20200101_models.ConfigureDtsJobRequest,
         runtime: util_models.RuntimeOptions,
     ) -> dts_20200101_models.ConfigureDtsJobResponse:
         """
-        The name of the DTS instance.
+        @summary 配置DTS任务
+        
+        @description The name of the DTS instance.
         
         @param request: ConfigureDtsJobRequest
         @param runtime: runtime options for this request RuntimeOptions
         @return: ConfigureDtsJobResponse
         """
         UtilClient.validate_model(request)
         query = {}
@@ -251,15 +253,17 @@
 
     async def configure_dts_job_with_options_async(
         self,
         request: dts_20200101_models.ConfigureDtsJobRequest,
         runtime: util_models.RuntimeOptions,
     ) -> dts_20200101_models.ConfigureDtsJobResponse:
         """
-        The name of the DTS instance.
+        @summary 配置DTS任务
+        
+        @description The name of the DTS instance.
         
         @param request: ConfigureDtsJobRequest
         @param runtime: runtime options for this request RuntimeOptions
         @return: ConfigureDtsJobResponse
         """
         UtilClient.validate_model(request)
         query = {}
@@ -395,28 +399,32 @@
         )
 
     def configure_dts_job(
         self,
         request: dts_20200101_models.ConfigureDtsJobRequest,
     ) -> dts_20200101_models.ConfigureDtsJobResponse:
         """
-        The name of the DTS instance.
+        @summary 配置DTS任务
+        
+        @description The name of the DTS instance.
         
         @param request: ConfigureDtsJobRequest
         @return: ConfigureDtsJobResponse
         """
         runtime = util_models.RuntimeOptions()
         return self.configure_dts_job_with_options(request, runtime)
 
     async def configure_dts_job_async(
         self,
         request: dts_20200101_models.ConfigureDtsJobRequest,
     ) -> dts_20200101_models.ConfigureDtsJobResponse:
         """
-        The name of the DTS instance.
+        @summary 配置DTS任务
+        
+        @description The name of the DTS instance.
         
         @param request: ConfigureDtsJobRequest
         @return: ConfigureDtsJobResponse
         """
         runtime = util_models.RuntimeOptions()
         return await self.configure_dts_job_with_options_async(request, runtime)
 
@@ -427,15 +435,15 @@
     ) -> dts_20200101_models.ConfigureDtsJobResponse:
         # Step 0: init client
         access_key_id = self._credential.get_access_key_id()
         access_key_secret = self._credential.get_access_key_secret()
         security_token = self._credential.get_security_token()
         credential_type = self._credential.get_type()
         open_platform_endpoint = self._open_platform_endpoint
-        if UtilClient.is_unset(open_platform_endpoint):
+        if UtilClient.empty(open_platform_endpoint):
             open_platform_endpoint = 'openplatform.aliyuncs.com'
         if UtilClient.is_unset(credential_type):
             credential_type = 'access_key'
         auth_config = open_api_models.Config(
             access_key_id=access_key_id,
             access_key_secret=access_key_secret,
             security_token=security_token,
@@ -447,20 +455,21 @@
         auth_client = OpenPlatformClient(auth_config)
         auth_request = open_platform_models.AuthorizeFileUploadRequest(
             product='Dts',
             region_id=self._region_id
         )
         auth_response = open_platform_models.AuthorizeFileUploadResponse()
         oss_config = oss_models.Config(
+            access_key_id=access_key_id,
             access_key_secret=access_key_secret,
             type='access_key',
             protocol=self._protocol,
             region_id=self._region_id
         )
-        oss_client = None
+        oss_client = OSSClient(oss_config)
         file_obj = file_form_models.FileField()
         oss_header = oss_models.PostObjectRequestHeader()
         upload_request = oss_models.PostObjectRequest()
         oss_runtime = ossutil_models.RuntimeOptions()
         OpenApiUtilClient.convert(runtime, oss_runtime)
         configure_dts_job_req = dts_20200101_models.ConfigureDtsJobRequest()
         OpenApiUtilClient.convert(request, configure_dts_job_req)
@@ -498,15 +507,15 @@
     ) -> dts_20200101_models.ConfigureDtsJobResponse:
         # Step 0: init client
         access_key_id = await self._credential.get_access_key_id_async()
         access_key_secret = await self._credential.get_access_key_secret_async()
         security_token = await self._credential.get_security_token_async()
         credential_type = self._credential.get_type()
         open_platform_endpoint = self._open_platform_endpoint
-        if UtilClient.is_unset(open_platform_endpoint):
+        if UtilClient.empty(open_platform_endpoint):
             open_platform_endpoint = 'openplatform.aliyuncs.com'
         if UtilClient.is_unset(credential_type):
             credential_type = 'access_key'
         auth_config = open_api_models.Config(
             access_key_id=access_key_id,
             access_key_secret=access_key_secret,
             security_token=security_token,
@@ -518,20 +527,21 @@
         auth_client = OpenPlatformClient(auth_config)
         auth_request = open_platform_models.AuthorizeFileUploadRequest(
             product='Dts',
             region_id=self._region_id
         )
         auth_response = open_platform_models.AuthorizeFileUploadResponse()
         oss_config = oss_models.Config(
+            access_key_id=access_key_id,
             access_key_secret=access_key_secret,
             type='access_key',
             protocol=self._protocol,
             region_id=self._region_id
         )
-        oss_client = None
+        oss_client = OSSClient(oss_config)
         file_obj = file_form_models.FileField()
         oss_header = oss_models.PostObjectRequestHeader()
         upload_request = oss_models.PostObjectRequest()
         oss_runtime = ossutil_models.RuntimeOptions()
         OpenApiUtilClient.convert(runtime, oss_runtime)
         configure_dts_job_req = dts_20200101_models.ConfigureDtsJobRequest()
         OpenApiUtilClient.convert(request, configure_dts_job_req)
@@ -564,16 +574,18 @@
 
     def configure_migration_job_with_options(
         self,
         request: dts_20200101_models.ConfigureMigrationJobRequest,
         runtime: util_models.RuntimeOptions,
     ) -> dts_20200101_models.ConfigureMigrationJobResponse:
         """
-        After you call this operation to configure a data migration task, the task will be automatically started. You do not need to call the [StartMigrationJob](~~49429~~) operation to start the task.
-        A data migration task may fail to be started due to precheck failures. You can call the [DescribeMigrationJobStatus](~~49433~~) operation to query the error messages about precheck failures. Then, you can fix the issue based on the error messages. After you fix the issue, you must call the [StartMigrationJob](~~49429~~) operation to restart the data migration task.
+        @summary Configures a data migration task.
+        
+        @description After you call this operation to configure a data migration task, the task will be automatically started. You do not need to call the [StartMigrationJob](https://help.aliyun.com/document_detail/49429.html) operation to start the task.
+        A data migration task may fail to be started due to precheck failures. You can call the [DescribeMigrationJobStatus](https://help.aliyun.com/document_detail/49433.html) operation to query the error messages about precheck failures. Then, you can fix the issue based on the error messages. After you fix the issue, you must call the [StartMigrationJob](https://help.aliyun.com/document_detail/49429.html) operation to restart the data migration task.
         
         @param request: ConfigureMigrationJobRequest
         @param runtime: runtime options for this request RuntimeOptions
         @return: ConfigureMigrationJobResponse
         """
         UtilClient.validate_model(request)
         query = {}
@@ -624,16 +636,18 @@
 
     async def configure_migration_job_with_options_async(
         self,
         request: dts_20200101_models.ConfigureMigrationJobRequest,
         runtime: util_models.RuntimeOptions,
     ) -> dts_20200101_models.ConfigureMigrationJobResponse:
         """
-        After you call this operation to configure a data migration task, the task will be automatically started. You do not need to call the [StartMigrationJob](~~49429~~) operation to start the task.
-        A data migration task may fail to be started due to precheck failures. You can call the [DescribeMigrationJobStatus](~~49433~~) operation to query the error messages about precheck failures. Then, you can fix the issue based on the error messages. After you fix the issue, you must call the [StartMigrationJob](~~49429~~) operation to restart the data migration task.
+        @summary Configures a data migration task.
+        
+        @description After you call this operation to configure a data migration task, the task will be automatically started. You do not need to call the [StartMigrationJob](https://help.aliyun.com/document_detail/49429.html) operation to start the task.
+        A data migration task may fail to be started due to precheck failures. You can call the [DescribeMigrationJobStatus](https://help.aliyun.com/document_detail/49433.html) operation to query the error messages about precheck failures. Then, you can fix the issue based on the error messages. After you fix the issue, you must call the [StartMigrationJob](https://help.aliyun.com/document_detail/49429.html) operation to restart the data migration task.
         
         @param request: ConfigureMigrationJobRequest
         @param runtime: runtime options for this request RuntimeOptions
         @return: ConfigureMigrationJobResponse
         """
         UtilClient.validate_model(request)
         query = {}
@@ -683,42 +697,51 @@
         )
 
     def configure_migration_job(
         self,
         request: dts_20200101_models.ConfigureMigrationJobRequest,
     ) -> dts_20200101_models.ConfigureMigrationJobResponse:
         """
-        After you call this operation to configure a data migration task, the task will be automatically started. You do not need to call the [StartMigrationJob](~~49429~~) operation to start the task.
-        A data migration task may fail to be started due to precheck failures. You can call the [DescribeMigrationJobStatus](~~49433~~) operation to query the error messages about precheck failures. Then, you can fix the issue based on the error messages. After you fix the issue, you must call the [StartMigrationJob](~~49429~~) operation to restart the data migration task.
+        @summary Configures a data migration task.
+        
+        @description After you call this operation to configure a data migration task, the task will be automatically started. You do not need to call the [StartMigrationJob](https://help.aliyun.com/document_detail/49429.html) operation to start the task.
+        A data migration task may fail to be started due to precheck failures. You can call the [DescribeMigrationJobStatus](https://help.aliyun.com/document_detail/49433.html) operation to query the error messages about precheck failures. Then, you can fix the issue based on the error messages. After you fix the issue, you must call the [StartMigrationJob](https://help.aliyun.com/document_detail/49429.html) operation to restart the data migration task.
         
         @param request: ConfigureMigrationJobRequest
         @return: ConfigureMigrationJobResponse
         """
         runtime = util_models.RuntimeOptions()
         return self.configure_migration_job_with_options(request, runtime)
 
     async def configure_migration_job_async(
         self,
         request: dts_20200101_models.ConfigureMigrationJobRequest,
     ) -> dts_20200101_models.ConfigureMigrationJobResponse:
         """
-        After you call this operation to configure a data migration task, the task will be automatically started. You do not need to call the [StartMigrationJob](~~49429~~) operation to start the task.
-        A data migration task may fail to be started due to precheck failures. You can call the [DescribeMigrationJobStatus](~~49433~~) operation to query the error messages about precheck failures. Then, you can fix the issue based on the error messages. After you fix the issue, you must call the [StartMigrationJob](~~49429~~) operation to restart the data migration task.
+        @summary Configures a data migration task.
+        
+        @description After you call this operation to configure a data migration task, the task will be automatically started. You do not need to call the [StartMigrationJob](https://help.aliyun.com/document_detail/49429.html) operation to start the task.
+        A data migration task may fail to be started due to precheck failures. You can call the [DescribeMigrationJobStatus](https://help.aliyun.com/document_detail/49433.html) operation to query the error messages about precheck failures. Then, you can fix the issue based on the error messages. After you fix the issue, you must call the [StartMigrationJob](https://help.aliyun.com/document_detail/49429.html) operation to restart the data migration task.
         
         @param request: ConfigureMigrationJobRequest
         @return: ConfigureMigrationJobResponse
         """
         runtime = util_models.RuntimeOptions()
         return await self.configure_migration_job_with_options_async(request, runtime)
 
     def configure_migration_job_alert_with_options(
         self,
         request: dts_20200101_models.ConfigureMigrationJobAlertRequest,
         runtime: util_models.RuntimeOptions,
     ) -> dts_20200101_models.ConfigureMigrationJobAlertResponse:
+        """
+        @param request: ConfigureMigrationJobAlertRequest
+        @param runtime: runtime options for this request RuntimeOptions
+        @return: ConfigureMigrationJobAlertResponse
+        """
         UtilClient.validate_model(request)
         query = {}
         if not UtilClient.is_unset(request.account_id):
             query['AccountId'] = request.account_id
         if not UtilClient.is_unset(request.delay_alert_phone):
             query['DelayAlertPhone'] = request.delay_alert_phone
         if not UtilClient.is_unset(request.delay_alert_status):
@@ -757,14 +780,19 @@
         )
 
     async def configure_migration_job_alert_with_options_async(
         self,
         request: dts_20200101_models.ConfigureMigrationJobAlertRequest,
         runtime: util_models.RuntimeOptions,
     ) -> dts_20200101_models.ConfigureMigrationJobAlertResponse:
+        """
+        @param request: ConfigureMigrationJobAlertRequest
+        @param runtime: runtime options for this request RuntimeOptions
+        @return: ConfigureMigrationJobAlertResponse
+        """
         UtilClient.validate_model(request)
         query = {}
         if not UtilClient.is_unset(request.account_id):
             query['AccountId'] = request.account_id
         if not UtilClient.is_unset(request.delay_alert_phone):
             query['DelayAlertPhone'] = request.delay_alert_phone
         if not UtilClient.is_unset(request.delay_alert_status):
@@ -802,29 +830,42 @@
             await self.call_api_async(params, req, runtime)
         )
 
     def configure_migration_job_alert(
         self,
         request: dts_20200101_models.ConfigureMigrationJobAlertRequest,
     ) -> dts_20200101_models.ConfigureMigrationJobAlertResponse:
+        """
+        @param request: ConfigureMigrationJobAlertRequest
+        @return: ConfigureMigrationJobAlertResponse
+        """
         runtime = util_models.RuntimeOptions()
         return self.configure_migration_job_alert_with_options(request, runtime)
 
     async def configure_migration_job_alert_async(
         self,
         request: dts_20200101_models.ConfigureMigrationJobAlertRequest,
     ) -> dts_20200101_models.ConfigureMigrationJobAlertResponse:
+        """
+        @param request: ConfigureMigrationJobAlertRequest
+        @return: ConfigureMigrationJobAlertResponse
+        """
         runtime = util_models.RuntimeOptions()
         return await self.configure_migration_job_alert_with_options_async(request, runtime)
 
     def configure_subscription_with_options(
         self,
         request: dts_20200101_models.ConfigureSubscriptionRequest,
         runtime: util_models.RuntimeOptions,
     ) -> dts_20200101_models.ConfigureSubscriptionResponse:
+        """
+        @param request: ConfigureSubscriptionRequest
+        @param runtime: runtime options for this request RuntimeOptions
+        @return: ConfigureSubscriptionResponse
+        """
         UtilClient.validate_model(request)
         query = {}
         if not UtilClient.is_unset(request.checkpoint):
             query['Checkpoint'] = request.checkpoint
         if not UtilClient.is_unset(request.db_list):
             query['DbList'] = request.db_list
         if not UtilClient.is_unset(request.dedicated_cluster_id):
@@ -911,14 +952,19 @@
         )
 
     async def configure_subscription_with_options_async(
         self,
         request: dts_20200101_models.ConfigureSubscriptionRequest,
         runtime: util_models.RuntimeOptions,
     ) -> dts_20200101_models.ConfigureSubscriptionResponse:
+        """
+        @param request: ConfigureSubscriptionRequest
+        @param runtime: runtime options for this request RuntimeOptions
+        @return: ConfigureSubscriptionResponse
+        """
         UtilClient.validate_model(request)
         query = {}
         if not UtilClient.is_unset(request.checkpoint):
             query['Checkpoint'] = request.checkpoint
         if not UtilClient.is_unset(request.db_list):
             query['DbList'] = request.db_list
         if not UtilClient.is_unset(request.dedicated_cluster_id):
@@ -1004,31 +1050,41 @@
             await self.call_api_async(params, req, runtime)
         )
 
     def configure_subscription(
         self,
         request: dts_20200101_models.ConfigureSubscriptionRequest,
     ) -> dts_20200101_models.ConfigureSubscriptionResponse:
+        """
+        @param request: ConfigureSubscriptionRequest
+        @return: ConfigureSubscriptionResponse
+        """
         runtime = util_models.RuntimeOptions()
         return self.configure_subscription_with_options(request, runtime)
 
     async def configure_subscription_async(
         self,
         request: dts_20200101_models.ConfigureSubscriptionRequest,
     ) -> dts_20200101_models.ConfigureSubscriptionResponse:
+        """
+        @param request: ConfigureSubscriptionRequest
+        @return: ConfigureSubscriptionResponse
+        """
         runtime = util_models.RuntimeOptions()
         return await self.configure_subscription_with_options_async(request, runtime)
 
     def configure_subscription_instance_with_options(
         self,
         request: dts_20200101_models.ConfigureSubscriptionInstanceRequest,
         runtime: util_models.RuntimeOptions,
     ) -> dts_20200101_models.ConfigureSubscriptionInstanceResponse:
         """
-        The operation that you want to perform. Set the value to *ConfigureSubscriptionInstance**.
+        @summary Before you call this operation, you must call the [CreateSubscriptionInstance](https://help.aliyun.com/document_detail/49436.html) operation to create a change tracking instance.
+        
+        @description The operation that you want to perform. Set the value to *ConfigureSubscriptionInstance**.
         
         @param request: ConfigureSubscriptionInstanceRequest
         @param runtime: runtime options for this request RuntimeOptions
         @return: ConfigureSubscriptionInstanceResponse
         """
         UtilClient.validate_model(request)
         query = {}
@@ -1077,15 +1133,17 @@
 
     async def configure_subscription_instance_with_options_async(
         self,
         request: dts_20200101_models.ConfigureSubscriptionInstanceRequest,
         runtime: util_models.RuntimeOptions,
     ) -> dts_20200101_models.ConfigureSubscriptionInstanceResponse:
         """
-        The operation that you want to perform. Set the value to *ConfigureSubscriptionInstance**.
+        @summary Before you call this operation, you must call the [CreateSubscriptionInstance](https://help.aliyun.com/document_detail/49436.html) operation to create a change tracking instance.
+        
+        @description The operation that you want to perform. Set the value to *ConfigureSubscriptionInstance**.
         
         @param request: ConfigureSubscriptionInstanceRequest
         @param runtime: runtime options for this request RuntimeOptions
         @return: ConfigureSubscriptionInstanceResponse
         """
         UtilClient.validate_model(request)
         query = {}
@@ -1133,40 +1191,49 @@
         )
 
     def configure_subscription_instance(
         self,
         request: dts_20200101_models.ConfigureSubscriptionInstanceRequest,
     ) -> dts_20200101_models.ConfigureSubscriptionInstanceResponse:
         """
-        The operation that you want to perform. Set the value to *ConfigureSubscriptionInstance**.
+        @summary Before you call this operation, you must call the [CreateSubscriptionInstance](https://help.aliyun.com/document_detail/49436.html) operation to create a change tracking instance.
+        
+        @description The operation that you want to perform. Set the value to *ConfigureSubscriptionInstance**.
         
         @param request: ConfigureSubscriptionInstanceRequest
         @return: ConfigureSubscriptionInstanceResponse
         """
         runtime = util_models.RuntimeOptions()
         return self.configure_subscription_instance_with_options(request, runtime)
 
     async def configure_subscription_instance_async(
         self,
         request: dts_20200101_models.ConfigureSubscriptionInstanceRequest,
     ) -> dts_20200101_models.ConfigureSubscriptionInstanceResponse:
         """
-        The operation that you want to perform. Set the value to *ConfigureSubscriptionInstance**.
+        @summary Before you call this operation, you must call the [CreateSubscriptionInstance](https://help.aliyun.com/document_detail/49436.html) operation to create a change tracking instance.
+        
+        @description The operation that you want to perform. Set the value to *ConfigureSubscriptionInstance**.
         
         @param request: ConfigureSubscriptionInstanceRequest
         @return: ConfigureSubscriptionInstanceResponse
         """
         runtime = util_models.RuntimeOptions()
         return await self.configure_subscription_instance_with_options_async(request, runtime)
 
     def configure_subscription_instance_alert_with_options(
         self,
         request: dts_20200101_models.ConfigureSubscriptionInstanceAlertRequest,
         runtime: util_models.RuntimeOptions,
     ) -> dts_20200101_models.ConfigureSubscriptionInstanceAlertResponse:
+        """
+        @param request: ConfigureSubscriptionInstanceAlertRequest
+        @param runtime: runtime options for this request RuntimeOptions
+        @return: ConfigureSubscriptionInstanceAlertResponse
+        """
         UtilClient.validate_model(request)
         query = {}
         if not UtilClient.is_unset(request.account_id):
             query['AccountId'] = request.account_id
         if not UtilClient.is_unset(request.delay_alert_phone):
             query['DelayAlertPhone'] = request.delay_alert_phone
         if not UtilClient.is_unset(request.delay_alert_status):
@@ -1205,14 +1272,19 @@
         )
 
     async def configure_subscription_instance_alert_with_options_async(
         self,
         request: dts_20200101_models.ConfigureSubscriptionInstanceAlertRequest,
         runtime: util_models.RuntimeOptions,
     ) -> dts_20200101_models.ConfigureSubscriptionInstanceAlertResponse:
+        """
+        @param request: ConfigureSubscriptionInstanceAlertRequest
+        @param runtime: runtime options for this request RuntimeOptions
+        @return: ConfigureSubscriptionInstanceAlertResponse
+        """
         UtilClient.validate_model(request)
         query = {}
         if not UtilClient.is_unset(request.account_id):
             query['AccountId'] = request.account_id
         if not UtilClient.is_unset(request.delay_alert_phone):
             query['DelayAlertPhone'] = request.delay_alert_phone
         if not UtilClient.is_unset(request.delay_alert_status):
@@ -1250,34 +1322,42 @@
             await self.call_api_async(params, req, runtime)
         )
 
     def configure_subscription_instance_alert(
         self,
         request: dts_20200101_models.ConfigureSubscriptionInstanceAlertRequest,
     ) -> dts_20200101_models.ConfigureSubscriptionInstanceAlertResponse:
+        """
+        @param request: ConfigureSubscriptionInstanceAlertRequest
+        @return: ConfigureSubscriptionInstanceAlertResponse
+        """
         runtime = util_models.RuntimeOptions()
         return self.configure_subscription_instance_alert_with_options(request, runtime)
 
     async def configure_subscription_instance_alert_async(
         self,
         request: dts_20200101_models.ConfigureSubscriptionInstanceAlertRequest,
     ) -> dts_20200101_models.ConfigureSubscriptionInstanceAlertResponse:
+        """
+        @param request: ConfigureSubscriptionInstanceAlertRequest
+        @return: ConfigureSubscriptionInstanceAlertResponse
+        """
         runtime = util_models.RuntimeOptions()
         return await self.configure_subscription_instance_alert_with_options_async(request, runtime)
 
     def configure_synchronization_job_with_options(
         self,
         request: dts_20200101_models.ConfigureSynchronizationJobRequest,
         runtime: util_models.RuntimeOptions,
     ) -> dts_20200101_models.ConfigureSynchronizationJobResponse:
         """
-        Before you call this operation, you must call the [CreateSynchronizationJob](~~49446~~) operation to create a data synchronization instance.
+        @description Before you call this operation, you must call the [CreateSynchronizationJob](https://help.aliyun.com/document_detail/49446.html) operation to create a data synchronization instance.
         >
-        *   After you call this operation to configure a data synchronization task, the task will be automatically started and prechecked. You do not need to call the [StartSynchronizationJob](~~49448~~) operation to start the task.
-        *   A data synchronization task may fail to be started due to precheck failures. You can call the [DescribeSynchronizationJobStatus](~~49453~~) operation to query the status of the task. Then, you can change parameter settings based on the error messages about the precheck failures. After you fix the issue, you must call the [StartSynchronizationJob](~~49448~~) operation to restart the data synchronization task.
+        After you call this operation to configure a data synchronization task, the task will be automatically started and prechecked. You do not need to call the [StartSynchronizationJob](https://help.aliyun.com/document_detail/49448.html) operation to start the task.
+        A data synchronization task may fail to be started due to precheck failures. You can call the [DescribeSynchronizationJobStatus](https://help.aliyun.com/document_detail/49453.html) operation to query the status of the task. Then, you can change parameter settings based on the error messages about the precheck failures. After you fix the issue, you must call the [StartSynchronizationJob](https://help.aliyun.com/document_detail/49448.html) operation to restart the data synchronization task.
         
         @param request: ConfigureSynchronizationJobRequest
         @param runtime: runtime options for this request RuntimeOptions
         @return: ConfigureSynchronizationJobResponse
         """
         UtilClient.validate_model(request)
         query = {}
@@ -1334,18 +1414,18 @@
 
     async def configure_synchronization_job_with_options_async(
         self,
         request: dts_20200101_models.ConfigureSynchronizationJobRequest,
         runtime: util_models.RuntimeOptions,
     ) -> dts_20200101_models.ConfigureSynchronizationJobResponse:
         """
-        Before you call this operation, you must call the [CreateSynchronizationJob](~~49446~~) operation to create a data synchronization instance.
+        @description Before you call this operation, you must call the [CreateSynchronizationJob](https://help.aliyun.com/document_detail/49446.html) operation to create a data synchronization instance.
         >
-        *   After you call this operation to configure a data synchronization task, the task will be automatically started and prechecked. You do not need to call the [StartSynchronizationJob](~~49448~~) operation to start the task.
-        *   A data synchronization task may fail to be started due to precheck failures. You can call the [DescribeSynchronizationJobStatus](~~49453~~) operation to query the status of the task. Then, you can change parameter settings based on the error messages about the precheck failures. After you fix the issue, you must call the [StartSynchronizationJob](~~49448~~) operation to restart the data synchronization task.
+        After you call this operation to configure a data synchronization task, the task will be automatically started and prechecked. You do not need to call the [StartSynchronizationJob](https://help.aliyun.com/document_detail/49448.html) operation to start the task.
+        A data synchronization task may fail to be started due to precheck failures. You can call the [DescribeSynchronizationJobStatus](https://help.aliyun.com/document_detail/49453.html) operation to query the status of the task. Then, you can change parameter settings based on the error messages about the precheck failures. After you fix the issue, you must call the [StartSynchronizationJob](https://help.aliyun.com/document_detail/49448.html) operation to restart the data synchronization task.
         
         @param request: ConfigureSynchronizationJobRequest
         @param runtime: runtime options for this request RuntimeOptions
         @return: ConfigureSynchronizationJobResponse
         """
         UtilClient.validate_model(request)
         query = {}
@@ -1401,46 +1481,51 @@
         )
 
     def configure_synchronization_job(
         self,
         request: dts_20200101_models.ConfigureSynchronizationJobRequest,
     ) -> dts_20200101_models.ConfigureSynchronizationJobResponse:
         """
-        Before you call this operation, you must call the [CreateSynchronizationJob](~~49446~~) operation to create a data synchronization instance.
+        @description Before you call this operation, you must call the [CreateSynchronizationJob](https://help.aliyun.com/document_detail/49446.html) operation to create a data synchronization instance.
         >
-        *   After you call this operation to configure a data synchronization task, the task will be automatically started and prechecked. You do not need to call the [StartSynchronizationJob](~~49448~~) operation to start the task.
-        *   A data synchronization task may fail to be started due to precheck failures. You can call the [DescribeSynchronizationJobStatus](~~49453~~) operation to query the status of the task. Then, you can change parameter settings based on the error messages about the precheck failures. After you fix the issue, you must call the [StartSynchronizationJob](~~49448~~) operation to restart the data synchronization task.
+        After you call this operation to configure a data synchronization task, the task will be automatically started and prechecked. You do not need to call the [StartSynchronizationJob](https://help.aliyun.com/document_detail/49448.html) operation to start the task.
+        A data synchronization task may fail to be started due to precheck failures. You can call the [DescribeSynchronizationJobStatus](https://help.aliyun.com/document_detail/49453.html) operation to query the status of the task. Then, you can change parameter settings based on the error messages about the precheck failures. After you fix the issue, you must call the [StartSynchronizationJob](https://help.aliyun.com/document_detail/49448.html) operation to restart the data synchronization task.
         
         @param request: ConfigureSynchronizationJobRequest
         @return: ConfigureSynchronizationJobResponse
         """
         runtime = util_models.RuntimeOptions()
         return self.configure_synchronization_job_with_options(request, runtime)
 
     async def configure_synchronization_job_async(
         self,
         request: dts_20200101_models.ConfigureSynchronizationJobRequest,
     ) -> dts_20200101_models.ConfigureSynchronizationJobResponse:
         """
-        Before you call this operation, you must call the [CreateSynchronizationJob](~~49446~~) operation to create a data synchronization instance.
+        @description Before you call this operation, you must call the [CreateSynchronizationJob](https://help.aliyun.com/document_detail/49446.html) operation to create a data synchronization instance.
         >
-        *   After you call this operation to configure a data synchronization task, the task will be automatically started and prechecked. You do not need to call the [StartSynchronizationJob](~~49448~~) operation to start the task.
-        *   A data synchronization task may fail to be started due to precheck failures. You can call the [DescribeSynchronizationJobStatus](~~49453~~) operation to query the status of the task. Then, you can change parameter settings based on the error messages about the precheck failures. After you fix the issue, you must call the [StartSynchronizationJob](~~49448~~) operation to restart the data synchronization task.
+        After you call this operation to configure a data synchronization task, the task will be automatically started and prechecked. You do not need to call the [StartSynchronizationJob](https://help.aliyun.com/document_detail/49448.html) operation to start the task.
+        A data synchronization task may fail to be started due to precheck failures. You can call the [DescribeSynchronizationJobStatus](https://help.aliyun.com/document_detail/49453.html) operation to query the status of the task. Then, you can change parameter settings based on the error messages about the precheck failures. After you fix the issue, you must call the [StartSynchronizationJob](https://help.aliyun.com/document_detail/49448.html) operation to restart the data synchronization task.
         
         @param request: ConfigureSynchronizationJobRequest
         @return: ConfigureSynchronizationJobResponse
         """
         runtime = util_models.RuntimeOptions()
         return await self.configure_synchronization_job_with_options_async(request, runtime)
 
     def configure_synchronization_job_alert_with_options(
         self,
         request: dts_20200101_models.ConfigureSynchronizationJobAlertRequest,
         runtime: util_models.RuntimeOptions,
     ) -> dts_20200101_models.ConfigureSynchronizationJobAlertResponse:
+        """
+        @param request: ConfigureSynchronizationJobAlertRequest
+        @param runtime: runtime options for this request RuntimeOptions
+        @return: ConfigureSynchronizationJobAlertResponse
+        """
         UtilClient.validate_model(request)
         query = {}
         if not UtilClient.is_unset(request.account_id):
             query['AccountId'] = request.account_id
         if not UtilClient.is_unset(request.delay_alert_phone):
             query['DelayAlertPhone'] = request.delay_alert_phone
         if not UtilClient.is_unset(request.delay_alert_status):
@@ -1481,14 +1566,19 @@
         )
 
     async def configure_synchronization_job_alert_with_options_async(
         self,
         request: dts_20200101_models.ConfigureSynchronizationJobAlertRequest,
         runtime: util_models.RuntimeOptions,
     ) -> dts_20200101_models.ConfigureSynchronizationJobAlertResponse:
+        """
+        @param request: ConfigureSynchronizationJobAlertRequest
+        @param runtime: runtime options for this request RuntimeOptions
+        @return: ConfigureSynchronizationJobAlertResponse
+        """
         UtilClient.validate_model(request)
         query = {}
         if not UtilClient.is_unset(request.account_id):
             query['AccountId'] = request.account_id
         if not UtilClient.is_unset(request.delay_alert_phone):
             query['DelayAlertPhone'] = request.delay_alert_phone
         if not UtilClient.is_unset(request.delay_alert_status):
@@ -1528,32 +1618,40 @@
             await self.call_api_async(params, req, runtime)
         )
 
     def configure_synchronization_job_alert(
         self,
         request: dts_20200101_models.ConfigureSynchronizationJobAlertRequest,
     ) -> dts_20200101_models.ConfigureSynchronizationJobAlertResponse:
+        """
+        @param request: ConfigureSynchronizationJobAlertRequest
+        @return: ConfigureSynchronizationJobAlertResponse
+        """
         runtime = util_models.RuntimeOptions()
         return self.configure_synchronization_job_alert_with_options(request, runtime)
 
     async def configure_synchronization_job_alert_async(
         self,
         request: dts_20200101_models.ConfigureSynchronizationJobAlertRequest,
     ) -> dts_20200101_models.ConfigureSynchronizationJobAlertResponse:
+        """
+        @param request: ConfigureSynchronizationJobAlertRequest
+        @return: ConfigureSynchronizationJobAlertResponse
+        """
         runtime = util_models.RuntimeOptions()
         return await self.configure_synchronization_job_alert_with_options_async(request, runtime)
 
     def configure_synchronization_job_replicator_compare_with_options(
         self,
         request: dts_20200101_models.ConfigureSynchronizationJobReplicatorCompareRequest,
         runtime: util_models.RuntimeOptions,
     ) -> dts_20200101_models.ConfigureSynchronizationJobReplicatorCompareResponse:
         """
-        When you use Data Transmission Service (DTS) to synchronize data, other data sources may write data to the destination instance. In this case, data may become inconsistent between the source and destination instances. To ensure data consistency, you can enable image matching.
-        After you call this operation, you can call the [DescribeSynchronizationJobReplicatorCompare](~~199183~~) operation to verify whether image matching is enabled for the data synchronization instance.
+        @description When you use Data Transmission Service (DTS) to synchronize data, other data sources may write data to the destination instance. In this case, data may become inconsistent between the source and destination instances. To ensure data consistency, you can enable image matching.
+        After you call this operation, you can call the [DescribeSynchronizationJobReplicatorCompare](https://help.aliyun.com/document_detail/199183.html) operation to verify whether image matching is enabled for the data synchronization instance.
         
         @param request: ConfigureSynchronizationJobReplicatorCompareRequest
         @param runtime: runtime options for this request RuntimeOptions
         @return: ConfigureSynchronizationJobReplicatorCompareResponse
         """
         UtilClient.validate_model(request)
         query = {}
@@ -1594,16 +1692,16 @@
 
     async def configure_synchronization_job_replicator_compare_with_options_async(
         self,
         request: dts_20200101_models.ConfigureSynchronizationJobReplicatorCompareRequest,
         runtime: util_models.RuntimeOptions,
     ) -> dts_20200101_models.ConfigureSynchronizationJobReplicatorCompareResponse:
         """
-        When you use Data Transmission Service (DTS) to synchronize data, other data sources may write data to the destination instance. In this case, data may become inconsistent between the source and destination instances. To ensure data consistency, you can enable image matching.
-        After you call this operation, you can call the [DescribeSynchronizationJobReplicatorCompare](~~199183~~) operation to verify whether image matching is enabled for the data synchronization instance.
+        @description When you use Data Transmission Service (DTS) to synchronize data, other data sources may write data to the destination instance. In this case, data may become inconsistent between the source and destination instances. To ensure data consistency, you can enable image matching.
+        After you call this operation, you can call the [DescribeSynchronizationJobReplicatorCompare](https://help.aliyun.com/document_detail/199183.html) operation to verify whether image matching is enabled for the data synchronization instance.
         
         @param request: ConfigureSynchronizationJobReplicatorCompareRequest
         @param runtime: runtime options for this request RuntimeOptions
         @return: ConfigureSynchronizationJobReplicatorCompareResponse
         """
         UtilClient.validate_model(request)
         query = {}
@@ -1643,42 +1741,49 @@
         )
 
     def configure_synchronization_job_replicator_compare(
         self,
         request: dts_20200101_models.ConfigureSynchronizationJobReplicatorCompareRequest,
     ) -> dts_20200101_models.ConfigureSynchronizationJobReplicatorCompareResponse:
         """
-        When you use Data Transmission Service (DTS) to synchronize data, other data sources may write data to the destination instance. In this case, data may become inconsistent between the source and destination instances. To ensure data consistency, you can enable image matching.
-        After you call this operation, you can call the [DescribeSynchronizationJobReplicatorCompare](~~199183~~) operation to verify whether image matching is enabled for the data synchronization instance.
+        @description When you use Data Transmission Service (DTS) to synchronize data, other data sources may write data to the destination instance. In this case, data may become inconsistent between the source and destination instances. To ensure data consistency, you can enable image matching.
+        After you call this operation, you can call the [DescribeSynchronizationJobReplicatorCompare](https://help.aliyun.com/document_detail/199183.html) operation to verify whether image matching is enabled for the data synchronization instance.
         
         @param request: ConfigureSynchronizationJobReplicatorCompareRequest
         @return: ConfigureSynchronizationJobReplicatorCompareResponse
         """
         runtime = util_models.RuntimeOptions()
         return self.configure_synchronization_job_replicator_compare_with_options(request, runtime)
 
     async def configure_synchronization_job_replicator_compare_async(
         self,
         request: dts_20200101_models.ConfigureSynchronizationJobReplicatorCompareRequest,
     ) -> dts_20200101_models.ConfigureSynchronizationJobReplicatorCompareResponse:
         """
-        When you use Data Transmission Service (DTS) to synchronize data, other data sources may write data to the destination instance. In this case, data may become inconsistent between the source and destination instances. To ensure data consistency, you can enable image matching.
-        After you call this operation, you can call the [DescribeSynchronizationJobReplicatorCompare](~~199183~~) operation to verify whether image matching is enabled for the data synchronization instance.
+        @description When you use Data Transmission Service (DTS) to synchronize data, other data sources may write data to the destination instance. In this case, data may become inconsistent between the source and destination instances. To ensure data consistency, you can enable image matching.
+        After you call this operation, you can call the [DescribeSynchronizationJobReplicatorCompare](https://help.aliyun.com/document_detail/199183.html) operation to verify whether image matching is enabled for the data synchronization instance.
         
         @param request: ConfigureSynchronizationJobReplicatorCompareRequest
         @return: ConfigureSynchronizationJobReplicatorCompareResponse
         """
         runtime = util_models.RuntimeOptions()
         return await self.configure_synchronization_job_replicator_compare_with_options_async(request, runtime)
 
     def count_job_by_condition_with_options(
         self,
         request: dts_20200101_models.CountJobByConditionRequest,
         runtime: util_models.RuntimeOptions,
     ) -> dts_20200101_models.CountJobByConditionResponse:
+        """
+        @summary 查询符合条件的任务数
+        
+        @param request: CountJobByConditionRequest
+        @param runtime: runtime options for this request RuntimeOptions
+        @return: CountJobByConditionResponse
+        """
         UtilClient.validate_model(request)
         query = {}
         if not UtilClient.is_unset(request.dest_db_type):
             query['DestDbType'] = request.dest_db_type
         if not UtilClient.is_unset(request.group_id):
             query['GroupId'] = request.group_id
         if not UtilClient.is_unset(request.job_type):
@@ -1717,14 +1822,21 @@
         )
 
     async def count_job_by_condition_with_options_async(
         self,
         request: dts_20200101_models.CountJobByConditionRequest,
         runtime: util_models.RuntimeOptions,
     ) -> dts_20200101_models.CountJobByConditionResponse:
+        """
+        @summary 查询符合条件的任务数
+        
+        @param request: CountJobByConditionRequest
+        @param runtime: runtime options for this request RuntimeOptions
+        @return: CountJobByConditionResponse
+        """
         UtilClient.validate_model(request)
         query = {}
         if not UtilClient.is_unset(request.dest_db_type):
             query['DestDbType'] = request.dest_db_type
         if not UtilClient.is_unset(request.group_id):
             query['GroupId'] = request.group_id
         if not UtilClient.is_unset(request.job_type):
@@ -1762,29 +1874,46 @@
             await self.call_api_async(params, req, runtime)
         )
 
     def count_job_by_condition(
         self,
         request: dts_20200101_models.CountJobByConditionRequest,
     ) -> dts_20200101_models.CountJobByConditionResponse:
+        """
+        @summary 查询符合条件的任务数
+        
+        @param request: CountJobByConditionRequest
+        @return: CountJobByConditionResponse
+        """
         runtime = util_models.RuntimeOptions()
         return self.count_job_by_condition_with_options(request, runtime)
 
     async def count_job_by_condition_async(
         self,
         request: dts_20200101_models.CountJobByConditionRequest,
     ) -> dts_20200101_models.CountJobByConditionResponse:
+        """
+        @summary 查询符合条件的任务数
+        
+        @param request: CountJobByConditionRequest
+        @return: CountJobByConditionResponse
+        """
         runtime = util_models.RuntimeOptions()
         return await self.count_job_by_condition_with_options_async(request, runtime)
 
     def create_consumer_channel_with_options(
         self,
         request: dts_20200101_models.CreateConsumerChannelRequest,
         runtime: util_models.RuntimeOptions,
     ) -> dts_20200101_models.CreateConsumerChannelResponse:
+        """
+        @param request: CreateConsumerChannelRequest
+        @param runtime: runtime options for this request RuntimeOptions
+        @return: CreateConsumerChannelResponse
+        """
         UtilClient.validate_model(request)
         query = {}
         if not UtilClient.is_unset(request.consumer_group_name):
             query['ConsumerGroupName'] = request.consumer_group_name
         if not UtilClient.is_unset(request.consumer_group_password):
             query['ConsumerGroupPassword'] = request.consumer_group_password
         if not UtilClient.is_unset(request.consumer_group_user_name):
@@ -1817,14 +1946,19 @@
         )
 
     async def create_consumer_channel_with_options_async(
         self,
         request: dts_20200101_models.CreateConsumerChannelRequest,
         runtime: util_models.RuntimeOptions,
     ) -> dts_20200101_models.CreateConsumerChannelResponse:
+        """
+        @param request: CreateConsumerChannelRequest
+        @param runtime: runtime options for this request RuntimeOptions
+        @return: CreateConsumerChannelResponse
+        """
         UtilClient.validate_model(request)
         query = {}
         if not UtilClient.is_unset(request.consumer_group_name):
             query['ConsumerGroupName'] = request.consumer_group_name
         if not UtilClient.is_unset(request.consumer_group_password):
             query['ConsumerGroupPassword'] = request.consumer_group_password
         if not UtilClient.is_unset(request.consumer_group_user_name):
@@ -1856,29 +1990,42 @@
             await self.call_api_async(params, req, runtime)
         )
 
     def create_consumer_channel(
         self,
         request: dts_20200101_models.CreateConsumerChannelRequest,
     ) -> dts_20200101_models.CreateConsumerChannelResponse:
+        """
+        @param request: CreateConsumerChannelRequest
+        @return: CreateConsumerChannelResponse
+        """
         runtime = util_models.RuntimeOptions()
         return self.create_consumer_channel_with_options(request, runtime)
 
     async def create_consumer_channel_async(
         self,
         request: dts_20200101_models.CreateConsumerChannelRequest,
     ) -> dts_20200101_models.CreateConsumerChannelResponse:
+        """
+        @param request: CreateConsumerChannelRequest
+        @return: CreateConsumerChannelResponse
+        """
         runtime = util_models.RuntimeOptions()
         return await self.create_consumer_channel_with_options_async(request, runtime)
 
     def create_consumer_group_with_options(
         self,
         request: dts_20200101_models.CreateConsumerGroupRequest,
         runtime: util_models.RuntimeOptions,
     ) -> dts_20200101_models.CreateConsumerGroupResponse:
+        """
+        @param request: CreateConsumerGroupRequest
+        @param runtime: runtime options for this request RuntimeOptions
+        @return: CreateConsumerGroupResponse
+        """
         UtilClient.validate_model(request)
         query = {}
         if not UtilClient.is_unset(request.account_id):
             query['AccountId'] = request.account_id
         if not UtilClient.is_unset(request.consumer_group_name):
             query['ConsumerGroupName'] = request.consumer_group_name
         if not UtilClient.is_unset(request.consumer_group_password):
@@ -1913,14 +2060,19 @@
         )
 
     async def create_consumer_group_with_options_async(
         self,
         request: dts_20200101_models.CreateConsumerGroupRequest,
         runtime: util_models.RuntimeOptions,
     ) -> dts_20200101_models.CreateConsumerGroupResponse:
+        """
+        @param request: CreateConsumerGroupRequest
+        @param runtime: runtime options for this request RuntimeOptions
+        @return: CreateConsumerGroupResponse
+        """
         UtilClient.validate_model(request)
         query = {}
         if not UtilClient.is_unset(request.account_id):
             query['AccountId'] = request.account_id
         if not UtilClient.is_unset(request.consumer_group_name):
             query['ConsumerGroupName'] = request.consumer_group_name
         if not UtilClient.is_unset(request.consumer_group_password):
@@ -1954,29 +2106,44 @@
             await self.call_api_async(params, req, runtime)
         )
 
     def create_consumer_group(
         self,
         request: dts_20200101_models.CreateConsumerGroupRequest,
     ) -> dts_20200101_models.CreateConsumerGroupResponse:
+        """
+        @param request: CreateConsumerGroupRequest
+        @return: CreateConsumerGroupResponse
+        """
         runtime = util_models.RuntimeOptions()
         return self.create_consumer_group_with_options(request, runtime)
 
     async def create_consumer_group_async(
         self,
         request: dts_20200101_models.CreateConsumerGroupRequest,
     ) -> dts_20200101_models.CreateConsumerGroupResponse:
+        """
+        @param request: CreateConsumerGroupRequest
+        @return: CreateConsumerGroupResponse
+        """
         runtime = util_models.RuntimeOptions()
         return await self.create_consumer_group_with_options_async(request, runtime)
 
     def create_dedicated_cluster_monitor_rule_with_options(
         self,
         request: dts_20200101_models.CreateDedicatedClusterMonitorRuleRequest,
         runtime: util_models.RuntimeOptions,
     ) -> dts_20200101_models.CreateDedicatedClusterMonitorRuleResponse:
+        """
+        @summary Creates an alert rule.
+        
+        @param request: CreateDedicatedClusterMonitorRuleRequest
+        @param runtime: runtime options for this request RuntimeOptions
+        @return: CreateDedicatedClusterMonitorRuleResponse
+        """
         UtilClient.validate_model(request)
         query = {}
         if not UtilClient.is_unset(request.cpu_alarm_threshold):
             query['CpuAlarmThreshold'] = request.cpu_alarm_threshold
         if not UtilClient.is_unset(request.dedicated_cluster_id):
             query['DedicatedClusterId'] = request.dedicated_cluster_id
         if not UtilClient.is_unset(request.disk_alarm_threshold):
@@ -2017,14 +2184,21 @@
         )
 
     async def create_dedicated_cluster_monitor_rule_with_options_async(
         self,
         request: dts_20200101_models.CreateDedicatedClusterMonitorRuleRequest,
         runtime: util_models.RuntimeOptions,
     ) -> dts_20200101_models.CreateDedicatedClusterMonitorRuleResponse:
+        """
+        @summary Creates an alert rule.
+        
+        @param request: CreateDedicatedClusterMonitorRuleRequest
+        @param runtime: runtime options for this request RuntimeOptions
+        @return: CreateDedicatedClusterMonitorRuleResponse
+        """
         UtilClient.validate_model(request)
         query = {}
         if not UtilClient.is_unset(request.cpu_alarm_threshold):
             query['CpuAlarmThreshold'] = request.cpu_alarm_threshold
         if not UtilClient.is_unset(request.dedicated_cluster_id):
             query['DedicatedClusterId'] = request.dedicated_cluster_id
         if not UtilClient.is_unset(request.disk_alarm_threshold):
@@ -2064,32 +2238,44 @@
             await self.call_api_async(params, req, runtime)
         )
 
     def create_dedicated_cluster_monitor_rule(
         self,
         request: dts_20200101_models.CreateDedicatedClusterMonitorRuleRequest,
     ) -> dts_20200101_models.CreateDedicatedClusterMonitorRuleResponse:
+        """
+        @summary Creates an alert rule.
+        
+        @param request: CreateDedicatedClusterMonitorRuleRequest
+        @return: CreateDedicatedClusterMonitorRuleResponse
+        """
         runtime = util_models.RuntimeOptions()
         return self.create_dedicated_cluster_monitor_rule_with_options(request, runtime)
 
     async def create_dedicated_cluster_monitor_rule_async(
         self,
         request: dts_20200101_models.CreateDedicatedClusterMonitorRuleRequest,
     ) -> dts_20200101_models.CreateDedicatedClusterMonitorRuleResponse:
+        """
+        @summary Creates an alert rule.
+        
+        @param request: CreateDedicatedClusterMonitorRuleRequest
+        @return: CreateDedicatedClusterMonitorRuleResponse
+        """
         runtime = util_models.RuntimeOptions()
         return await self.create_dedicated_cluster_monitor_rule_with_options_async(request, runtime)
 
     def create_dts_instance_with_options(
         self,
         request: dts_20200101_models.CreateDtsInstanceRequest,
         runtime: util_models.RuntimeOptions,
     ) -> dts_20200101_models.CreateDtsInstanceResponse:
         """
-        Before you call this operation, make sure that you fully understand the billing methods and [pricing](https://www.alibabacloud.com/zh/product/apsaradb-for-mongodb/pricing) of DTS.
-        *   If you want to run a DTS task on a DTS dedicated cluster, you must configure the task before you purchase a DTS instance. You can call the [ConfigureDtsJob](~~208399~~) operation to configure a DTS task.
+        @description    Before you call this operation, make sure that you fully understand the billing methods and [pricing](https://www.alibabacloud.com/zh/product/apsaradb-for-mongodb/pricing) of DTS.
+        If you want to run a DTS task on a DTS dedicated cluster, you must configure the task before you purchase a DTS instance. You can call the [ConfigureDtsJob](https://help.aliyun.com/document_detail/208399.html) operation to configure a DTS task.
         
         @param request: CreateDtsInstanceRequest
         @param runtime: runtime options for this request RuntimeOptions
         @return: CreateDtsInstanceResponse
         """
         UtilClient.validate_model(request)
         query = {}
@@ -2158,16 +2344,16 @@
 
     async def create_dts_instance_with_options_async(
         self,
         request: dts_20200101_models.CreateDtsInstanceRequest,
         runtime: util_models.RuntimeOptions,
     ) -> dts_20200101_models.CreateDtsInstanceResponse:
         """
-        Before you call this operation, make sure that you fully understand the billing methods and [pricing](https://www.alibabacloud.com/zh/product/apsaradb-for-mongodb/pricing) of DTS.
-        *   If you want to run a DTS task on a DTS dedicated cluster, you must configure the task before you purchase a DTS instance. You can call the [ConfigureDtsJob](~~208399~~) operation to configure a DTS task.
+        @description    Before you call this operation, make sure that you fully understand the billing methods and [pricing](https://www.alibabacloud.com/zh/product/apsaradb-for-mongodb/pricing) of DTS.
+        If you want to run a DTS task on a DTS dedicated cluster, you must configure the task before you purchase a DTS instance. You can call the [ConfigureDtsJob](https://help.aliyun.com/document_detail/208399.html) operation to configure a DTS task.
         
         @param request: CreateDtsInstanceRequest
         @param runtime: runtime options for this request RuntimeOptions
         @return: CreateDtsInstanceResponse
         """
         UtilClient.validate_model(request)
         query = {}
@@ -2235,47 +2421,47 @@
         )
 
     def create_dts_instance(
         self,
         request: dts_20200101_models.CreateDtsInstanceRequest,
     ) -> dts_20200101_models.CreateDtsInstanceResponse:
         """
-        Before you call this operation, make sure that you fully understand the billing methods and [pricing](https://www.alibabacloud.com/zh/product/apsaradb-for-mongodb/pricing) of DTS.
-        *   If you want to run a DTS task on a DTS dedicated cluster, you must configure the task before you purchase a DTS instance. You can call the [ConfigureDtsJob](~~208399~~) operation to configure a DTS task.
+        @description    Before you call this operation, make sure that you fully understand the billing methods and [pricing](https://www.alibabacloud.com/zh/product/apsaradb-for-mongodb/pricing) of DTS.
+        If you want to run a DTS task on a DTS dedicated cluster, you must configure the task before you purchase a DTS instance. You can call the [ConfigureDtsJob](https://help.aliyun.com/document_detail/208399.html) operation to configure a DTS task.
         
         @param request: CreateDtsInstanceRequest
         @return: CreateDtsInstanceResponse
         """
         runtime = util_models.RuntimeOptions()
         return self.create_dts_instance_with_options(request, runtime)
 
     async def create_dts_instance_async(
         self,
         request: dts_20200101_models.CreateDtsInstanceRequest,
     ) -> dts_20200101_models.CreateDtsInstanceResponse:
         """
-        Before you call this operation, make sure that you fully understand the billing methods and [pricing](https://www.alibabacloud.com/zh/product/apsaradb-for-mongodb/pricing) of DTS.
-        *   If you want to run a DTS task on a DTS dedicated cluster, you must configure the task before you purchase a DTS instance. You can call the [ConfigureDtsJob](~~208399~~) operation to configure a DTS task.
+        @description    Before you call this operation, make sure that you fully understand the billing methods and [pricing](https://www.alibabacloud.com/zh/product/apsaradb-for-mongodb/pricing) of DTS.
+        If you want to run a DTS task on a DTS dedicated cluster, you must configure the task before you purchase a DTS instance. You can call the [ConfigureDtsJob](https://help.aliyun.com/document_detail/208399.html) operation to configure a DTS task.
         
         @param request: CreateDtsInstanceRequest
         @return: CreateDtsInstanceResponse
         """
         runtime = util_models.RuntimeOptions()
         return await self.create_dts_instance_with_options_async(request, runtime)
 
     def create_job_monitor_rule_with_options(
         self,
         request: dts_20200101_models.CreateJobMonitorRuleRequest,
         runtime: util_models.RuntimeOptions,
     ) -> dts_20200101_models.CreateJobMonitorRuleResponse:
         """
-        DTS provides the following metrics for DTS tasks:***********\
-        *   **Latency**: DTS monitors the latency of a DTS task. If the latency of the task exceeds the specified threshold, an alert is triggered. Unit: seconds.
-        *   **Status**: DTS monitors the status of a DTS task. If the state of the task changes to **Error** or **Restore**, an alert is triggered.
-        *   **Full Timeout**: DTS monitors the duration of a DTS task. If the duration of the task exceeds the specified threshold, an alert is triggered. Unit: hours.
+        @description DTS provides the following metrics for DTS tasks:***********\
+        **Latency**: DTS monitors the latency of a DTS task. If the latency of the task exceeds the specified threshold, an alert is triggered. Unit: seconds.
+        **Status**: DTS monitors the status of a DTS task. If the state of the task changes to **Error** or **Restore**, an alert is triggered.
+        **Full Timeout**: DTS monitors the duration of a DTS task. If the duration of the task exceeds the specified threshold, an alert is triggered. Unit: hours.
         
         @param request: CreateJobMonitorRuleRequest
         @param runtime: runtime options for this request RuntimeOptions
         @return: CreateJobMonitorRuleResponse
         """
         UtilClient.validate_model(request)
         query = {}
@@ -2320,18 +2506,18 @@
 
     async def create_job_monitor_rule_with_options_async(
         self,
         request: dts_20200101_models.CreateJobMonitorRuleRequest,
         runtime: util_models.RuntimeOptions,
     ) -> dts_20200101_models.CreateJobMonitorRuleResponse:
         """
-        DTS provides the following metrics for DTS tasks:***********\
-        *   **Latency**: DTS monitors the latency of a DTS task. If the latency of the task exceeds the specified threshold, an alert is triggered. Unit: seconds.
-        *   **Status**: DTS monitors the status of a DTS task. If the state of the task changes to **Error** or **Restore**, an alert is triggered.
-        *   **Full Timeout**: DTS monitors the duration of a DTS task. If the duration of the task exceeds the specified threshold, an alert is triggered. Unit: hours.
+        @description DTS provides the following metrics for DTS tasks:***********\
+        **Latency**: DTS monitors the latency of a DTS task. If the latency of the task exceeds the specified threshold, an alert is triggered. Unit: seconds.
+        **Status**: DTS monitors the status of a DTS task. If the state of the task changes to **Error** or **Restore**, an alert is triggered.
+        **Full Timeout**: DTS monitors the duration of a DTS task. If the duration of the task exceeds the specified threshold, an alert is triggered. Unit: hours.
         
         @param request: CreateJobMonitorRuleRequest
         @param runtime: runtime options for this request RuntimeOptions
         @return: CreateJobMonitorRuleResponse
         """
         UtilClient.validate_model(request)
         query = {}
@@ -2375,50 +2561,50 @@
         )
 
     def create_job_monitor_rule(
         self,
         request: dts_20200101_models.CreateJobMonitorRuleRequest,
     ) -> dts_20200101_models.CreateJobMonitorRuleResponse:
         """
-        DTS provides the following metrics for DTS tasks:***********\
-        *   **Latency**: DTS monitors the latency of a DTS task. If the latency of the task exceeds the specified threshold, an alert is triggered. Unit: seconds.
-        *   **Status**: DTS monitors the status of a DTS task. If the state of the task changes to **Error** or **Restore**, an alert is triggered.
-        *   **Full Timeout**: DTS monitors the duration of a DTS task. If the duration of the task exceeds the specified threshold, an alert is triggered. Unit: hours.
+        @description DTS provides the following metrics for DTS tasks:***********\
+        **Latency**: DTS monitors the latency of a DTS task. If the latency of the task exceeds the specified threshold, an alert is triggered. Unit: seconds.
+        **Status**: DTS monitors the status of a DTS task. If the state of the task changes to **Error** or **Restore**, an alert is triggered.
+        **Full Timeout**: DTS monitors the duration of a DTS task. If the duration of the task exceeds the specified threshold, an alert is triggered. Unit: hours.
         
         @param request: CreateJobMonitorRuleRequest
         @return: CreateJobMonitorRuleResponse
         """
         runtime = util_models.RuntimeOptions()
         return self.create_job_monitor_rule_with_options(request, runtime)
 
     async def create_job_monitor_rule_async(
         self,
         request: dts_20200101_models.CreateJobMonitorRuleRequest,
     ) -> dts_20200101_models.CreateJobMonitorRuleResponse:
         """
-        DTS provides the following metrics for DTS tasks:***********\
-        *   **Latency**: DTS monitors the latency of a DTS task. If the latency of the task exceeds the specified threshold, an alert is triggered. Unit: seconds.
-        *   **Status**: DTS monitors the status of a DTS task. If the state of the task changes to **Error** or **Restore**, an alert is triggered.
-        *   **Full Timeout**: DTS monitors the duration of a DTS task. If the duration of the task exceeds the specified threshold, an alert is triggered. Unit: hours.
+        @description DTS provides the following metrics for DTS tasks:***********\
+        **Latency**: DTS monitors the latency of a DTS task. If the latency of the task exceeds the specified threshold, an alert is triggered. Unit: seconds.
+        **Status**: DTS monitors the status of a DTS task. If the state of the task changes to **Error** or **Restore**, an alert is triggered.
+        **Full Timeout**: DTS monitors the duration of a DTS task. If the duration of the task exceeds the specified threshold, an alert is triggered. Unit: hours.
         
         @param request: CreateJobMonitorRuleRequest
         @return: CreateJobMonitorRuleResponse
         """
         runtime = util_models.RuntimeOptions()
         return await self.create_job_monitor_rule_with_options_async(request, runtime)
 
     def create_migration_job_with_options(
         self,
         request: dts_20200101_models.CreateMigrationJobRequest,
         runtime: util_models.RuntimeOptions,
     ) -> dts_20200101_models.CreateMigrationJobResponse:
         """
-        >  This API operation is outdated. We recommend that you use the new version. For more information, see [CreateDtsInstance](~~208270~~).
+        @description >  This API operation is outdated. We recommend that you use the new version. For more information, see [CreateDtsInstance](https://help.aliyun.com/document_detail/208270.html).
         Before you call this operation, make sure that you fully understand the billing methods and [pricing](https://www.alibabacloud.com/zh/product/data-transmission-service/pricing) of Data Transmission Service (DTS).
-        After you purchase a data migration instance, you must call the [ConfigureMigrationJob](~~324260~~) operation to configure a data migration task.
+        After you purchase a data migration instance, you must call the [ConfigureMigrationJob](https://help.aliyun.com/document_detail/324260.html) operation to configure a data migration task.
         
         @param request: CreateMigrationJobRequest
         @param runtime: runtime options for this request RuntimeOptions
         @return: CreateMigrationJobResponse
         """
         UtilClient.validate_model(request)
         query = {}
@@ -2457,17 +2643,17 @@
 
     async def create_migration_job_with_options_async(
         self,
         request: dts_20200101_models.CreateMigrationJobRequest,
         runtime: util_models.RuntimeOptions,
     ) -> dts_20200101_models.CreateMigrationJobResponse:
         """
-        >  This API operation is outdated. We recommend that you use the new version. For more information, see [CreateDtsInstance](~~208270~~).
+        @description >  This API operation is outdated. We recommend that you use the new version. For more information, see [CreateDtsInstance](https://help.aliyun.com/document_detail/208270.html).
         Before you call this operation, make sure that you fully understand the billing methods and [pricing](https://www.alibabacloud.com/zh/product/data-transmission-service/pricing) of Data Transmission Service (DTS).
-        After you purchase a data migration instance, you must call the [ConfigureMigrationJob](~~324260~~) operation to configure a data migration task.
+        After you purchase a data migration instance, you must call the [ConfigureMigrationJob](https://help.aliyun.com/document_detail/324260.html) operation to configure a data migration task.
         
         @param request: CreateMigrationJobRequest
         @param runtime: runtime options for this request RuntimeOptions
         @return: CreateMigrationJobResponse
         """
         UtilClient.validate_model(request)
         query = {}
@@ -2505,44 +2691,51 @@
         )
 
     def create_migration_job(
         self,
         request: dts_20200101_models.CreateMigrationJobRequest,
     ) -> dts_20200101_models.CreateMigrationJobResponse:
         """
-        >  This API operation is outdated. We recommend that you use the new version. For more information, see [CreateDtsInstance](~~208270~~).
+        @description >  This API operation is outdated. We recommend that you use the new version. For more information, see [CreateDtsInstance](https://help.aliyun.com/document_detail/208270.html).
         Before you call this operation, make sure that you fully understand the billing methods and [pricing](https://www.alibabacloud.com/zh/product/data-transmission-service/pricing) of Data Transmission Service (DTS).
-        After you purchase a data migration instance, you must call the [ConfigureMigrationJob](~~324260~~) operation to configure a data migration task.
+        After you purchase a data migration instance, you must call the [ConfigureMigrationJob](https://help.aliyun.com/document_detail/324260.html) operation to configure a data migration task.
         
         @param request: CreateMigrationJobRequest
         @return: CreateMigrationJobResponse
         """
         runtime = util_models.RuntimeOptions()
         return self.create_migration_job_with_options(request, runtime)
 
     async def create_migration_job_async(
         self,
         request: dts_20200101_models.CreateMigrationJobRequest,
     ) -> dts_20200101_models.CreateMigrationJobResponse:
         """
-        >  This API operation is outdated. We recommend that you use the new version. For more information, see [CreateDtsInstance](~~208270~~).
+        @description >  This API operation is outdated. We recommend that you use the new version. For more information, see [CreateDtsInstance](https://help.aliyun.com/document_detail/208270.html).
         Before you call this operation, make sure that you fully understand the billing methods and [pricing](https://www.alibabacloud.com/zh/product/data-transmission-service/pricing) of Data Transmission Service (DTS).
-        After you purchase a data migration instance, you must call the [ConfigureMigrationJob](~~324260~~) operation to configure a data migration task.
+        After you purchase a data migration instance, you must call the [ConfigureMigrationJob](https://help.aliyun.com/document_detail/324260.html) operation to configure a data migration task.
         
         @param request: CreateMigrationJobRequest
         @return: CreateMigrationJobResponse
         """
         runtime = util_models.RuntimeOptions()
         return await self.create_migration_job_with_options_async(request, runtime)
 
     def create_reverse_dts_job_with_options(
         self,
         request: dts_20200101_models.CreateReverseDtsJobRequest,
         runtime: util_models.RuntimeOptions,
     ) -> dts_20200101_models.CreateReverseDtsJobResponse:
+        """
+        @summary 创建DTS反向增量同步任务
+        
+        @param request: CreateReverseDtsJobRequest
+        @param runtime: runtime options for this request RuntimeOptions
+        @return: CreateReverseDtsJobResponse
+        """
         UtilClient.validate_model(request)
         query = {}
         if not UtilClient.is_unset(request.dts_job_id):
             query['DtsJobId'] = request.dts_job_id
         if not UtilClient.is_unset(request.resource_group_id):
             query['ResourceGroupId'] = request.resource_group_id
         if not UtilClient.is_unset(request.shard_password):
@@ -2569,14 +2762,21 @@
         )
 
     async def create_reverse_dts_job_with_options_async(
         self,
         request: dts_20200101_models.CreateReverseDtsJobRequest,
         runtime: util_models.RuntimeOptions,
     ) -> dts_20200101_models.CreateReverseDtsJobResponse:
+        """
+        @summary 创建DTS反向增量同步任务
+        
+        @param request: CreateReverseDtsJobRequest
+        @param runtime: runtime options for this request RuntimeOptions
+        @return: CreateReverseDtsJobResponse
+        """
         UtilClient.validate_model(request)
         query = {}
         if not UtilClient.is_unset(request.dts_job_id):
             query['DtsJobId'] = request.dts_job_id
         if not UtilClient.is_unset(request.resource_group_id):
             query['ResourceGroupId'] = request.resource_group_id
         if not UtilClient.is_unset(request.shard_password):
@@ -2602,31 +2802,43 @@
             await self.call_api_async(params, req, runtime)
         )
 
     def create_reverse_dts_job(
         self,
         request: dts_20200101_models.CreateReverseDtsJobRequest,
     ) -> dts_20200101_models.CreateReverseDtsJobResponse:
+        """
+        @summary 创建DTS反向增量同步任务
+        
+        @param request: CreateReverseDtsJobRequest
+        @return: CreateReverseDtsJobResponse
+        """
         runtime = util_models.RuntimeOptions()
         return self.create_reverse_dts_job_with_options(request, runtime)
 
     async def create_reverse_dts_job_async(
         self,
         request: dts_20200101_models.CreateReverseDtsJobRequest,
     ) -> dts_20200101_models.CreateReverseDtsJobResponse:
+        """
+        @summary 创建DTS反向增量同步任务
+        
+        @param request: CreateReverseDtsJobRequest
+        @return: CreateReverseDtsJobResponse
+        """
         runtime = util_models.RuntimeOptions()
         return await self.create_reverse_dts_job_with_options_async(request, runtime)
 
     def create_subscription_instance_with_options(
         self,
         request: dts_20200101_models.CreateSubscriptionInstanceRequest,
         runtime: util_models.RuntimeOptions,
     ) -> dts_20200101_models.CreateSubscriptionInstanceResponse:
         """
-        Before you call this operation, make sure that you fully understand the billing methods and [pricing](https://www.alibabacloud.com/zh/product/data-transmission-service/pricing) of Data Transmission Service (DTS).
+        @description Before you call this operation, make sure that you fully understand the billing methods and [pricing](https://www.alibabacloud.com/zh/product/data-transmission-service/pricing) of Data Transmission Service (DTS).
         
         @param request: CreateSubscriptionInstanceRequest
         @param runtime: runtime options for this request RuntimeOptions
         @return: CreateSubscriptionInstanceResponse
         """
         UtilClient.validate_model(request)
         query = {}
@@ -2671,15 +2883,15 @@
 
     async def create_subscription_instance_with_options_async(
         self,
         request: dts_20200101_models.CreateSubscriptionInstanceRequest,
         runtime: util_models.RuntimeOptions,
     ) -> dts_20200101_models.CreateSubscriptionInstanceResponse:
         """
-        Before you call this operation, make sure that you fully understand the billing methods and [pricing](https://www.alibabacloud.com/zh/product/data-transmission-service/pricing) of Data Transmission Service (DTS).
+        @description Before you call this operation, make sure that you fully understand the billing methods and [pricing](https://www.alibabacloud.com/zh/product/data-transmission-service/pricing) of Data Transmission Service (DTS).
         
         @param request: CreateSubscriptionInstanceRequest
         @param runtime: runtime options for this request RuntimeOptions
         @return: CreateSubscriptionInstanceResponse
         """
         UtilClient.validate_model(request)
         query = {}
@@ -2723,43 +2935,43 @@
         )
 
     def create_subscription_instance(
         self,
         request: dts_20200101_models.CreateSubscriptionInstanceRequest,
     ) -> dts_20200101_models.CreateSubscriptionInstanceResponse:
         """
-        Before you call this operation, make sure that you fully understand the billing methods and [pricing](https://www.alibabacloud.com/zh/product/data-transmission-service/pricing) of Data Transmission Service (DTS).
+        @description Before you call this operation, make sure that you fully understand the billing methods and [pricing](https://www.alibabacloud.com/zh/product/data-transmission-service/pricing) of Data Transmission Service (DTS).
         
         @param request: CreateSubscriptionInstanceRequest
         @return: CreateSubscriptionInstanceResponse
         """
         runtime = util_models.RuntimeOptions()
         return self.create_subscription_instance_with_options(request, runtime)
 
     async def create_subscription_instance_async(
         self,
         request: dts_20200101_models.CreateSubscriptionInstanceRequest,
     ) -> dts_20200101_models.CreateSubscriptionInstanceResponse:
         """
-        Before you call this operation, make sure that you fully understand the billing methods and [pricing](https://www.alibabacloud.com/zh/product/data-transmission-service/pricing) of Data Transmission Service (DTS).
+        @description Before you call this operation, make sure that you fully understand the billing methods and [pricing](https://www.alibabacloud.com/zh/product/data-transmission-service/pricing) of Data Transmission Service (DTS).
         
         @param request: CreateSubscriptionInstanceRequest
         @return: CreateSubscriptionInstanceResponse
         """
         runtime = util_models.RuntimeOptions()
         return await self.create_subscription_instance_with_options_async(request, runtime)
 
     def create_synchronization_job_with_options(
         self,
         request: dts_20200101_models.CreateSynchronizationJobRequest,
         runtime: util_models.RuntimeOptions,
     ) -> dts_20200101_models.CreateSynchronizationJobResponse:
         """
-        Before you call this operation, make sure that you fully understand the billing methods and [pricing](https://www.alibabacloud.com/zh/product/data-transmission-service/pricing) of Data Transmission Service (DTS).
-        After you purchase a data synchronization instance, you must call the [ConfigureSynchronizationJob](~~49447~~) operation to configure a data synchronization task. Then, the task is automatically started.
+        @description Before you call this operation, make sure that you fully understand the billing methods and [pricing](https://www.alibabacloud.com/zh/product/data-transmission-service/pricing) of Data Transmission Service (DTS).
+        After you purchase a data synchronization instance, you must call the [ConfigureSynchronizationJob](https://help.aliyun.com/document_detail/49447.html) operation to configure a data synchronization task. Then, the task is automatically started.
         
         @param request: CreateSynchronizationJobRequest
         @param runtime: runtime options for this request RuntimeOptions
         @return: CreateSynchronizationJobResponse
         """
         UtilClient.validate_model(request)
         query = {}
@@ -2816,16 +3028,16 @@
 
     async def create_synchronization_job_with_options_async(
         self,
         request: dts_20200101_models.CreateSynchronizationJobRequest,
         runtime: util_models.RuntimeOptions,
     ) -> dts_20200101_models.CreateSynchronizationJobResponse:
         """
-        Before you call this operation, make sure that you fully understand the billing methods and [pricing](https://www.alibabacloud.com/zh/product/data-transmission-service/pricing) of Data Transmission Service (DTS).
-        After you purchase a data synchronization instance, you must call the [ConfigureSynchronizationJob](~~49447~~) operation to configure a data synchronization task. Then, the task is automatically started.
+        @description Before you call this operation, make sure that you fully understand the billing methods and [pricing](https://www.alibabacloud.com/zh/product/data-transmission-service/pricing) of Data Transmission Service (DTS).
+        After you purchase a data synchronization instance, you must call the [ConfigureSynchronizationJob](https://help.aliyun.com/document_detail/49447.html) operation to configure a data synchronization task. Then, the task is automatically started.
         
         @param request: CreateSynchronizationJobRequest
         @param runtime: runtime options for this request RuntimeOptions
         @return: CreateSynchronizationJobResponse
         """
         UtilClient.validate_model(request)
         query = {}
@@ -2881,42 +3093,47 @@
         )
 
     def create_synchronization_job(
         self,
         request: dts_20200101_models.CreateSynchronizationJobRequest,
     ) -> dts_20200101_models.CreateSynchronizationJobResponse:
         """
-        Before you call this operation, make sure that you fully understand the billing methods and [pricing](https://www.alibabacloud.com/zh/product/data-transmission-service/pricing) of Data Transmission Service (DTS).
-        After you purchase a data synchronization instance, you must call the [ConfigureSynchronizationJob](~~49447~~) operation to configure a data synchronization task. Then, the task is automatically started.
+        @description Before you call this operation, make sure that you fully understand the billing methods and [pricing](https://www.alibabacloud.com/zh/product/data-transmission-service/pricing) of Data Transmission Service (DTS).
+        After you purchase a data synchronization instance, you must call the [ConfigureSynchronizationJob](https://help.aliyun.com/document_detail/49447.html) operation to configure a data synchronization task. Then, the task is automatically started.
         
         @param request: CreateSynchronizationJobRequest
         @return: CreateSynchronizationJobResponse
         """
         runtime = util_models.RuntimeOptions()
         return self.create_synchronization_job_with_options(request, runtime)
 
     async def create_synchronization_job_async(
         self,
         request: dts_20200101_models.CreateSynchronizationJobRequest,
     ) -> dts_20200101_models.CreateSynchronizationJobResponse:
         """
-        Before you call this operation, make sure that you fully understand the billing methods and [pricing](https://www.alibabacloud.com/zh/product/data-transmission-service/pricing) of Data Transmission Service (DTS).
-        After you purchase a data synchronization instance, you must call the [ConfigureSynchronizationJob](~~49447~~) operation to configure a data synchronization task. Then, the task is automatically started.
+        @description Before you call this operation, make sure that you fully understand the billing methods and [pricing](https://www.alibabacloud.com/zh/product/data-transmission-service/pricing) of Data Transmission Service (DTS).
+        After you purchase a data synchronization instance, you must call the [ConfigureSynchronizationJob](https://help.aliyun.com/document_detail/49447.html) operation to configure a data synchronization task. Then, the task is automatically started.
         
         @param request: CreateSynchronizationJobRequest
         @return: CreateSynchronizationJobResponse
         """
         runtime = util_models.RuntimeOptions()
         return await self.create_synchronization_job_with_options_async(request, runtime)
 
     def delete_consumer_channel_with_options(
         self,
         request: dts_20200101_models.DeleteConsumerChannelRequest,
         runtime: util_models.RuntimeOptions,
     ) -> dts_20200101_models.DeleteConsumerChannelResponse:
+        """
+        @param request: DeleteConsumerChannelRequest
+        @param runtime: runtime options for this request RuntimeOptions
+        @return: DeleteConsumerChannelResponse
+        """
         UtilClient.validate_model(request)
         query = {}
         if not UtilClient.is_unset(request.consumer_group_id):
             query['ConsumerGroupId'] = request.consumer_group_id
         if not UtilClient.is_unset(request.dts_instance_id):
             query['DtsInstanceId'] = request.dts_instance_id
         if not UtilClient.is_unset(request.dts_job_id):
@@ -2945,14 +3162,19 @@
         )
 
     async def delete_consumer_channel_with_options_async(
         self,
         request: dts_20200101_models.DeleteConsumerChannelRequest,
         runtime: util_models.RuntimeOptions,
     ) -> dts_20200101_models.DeleteConsumerChannelResponse:
+        """
+        @param request: DeleteConsumerChannelRequest
+        @param runtime: runtime options for this request RuntimeOptions
+        @return: DeleteConsumerChannelResponse
+        """
         UtilClient.validate_model(request)
         query = {}
         if not UtilClient.is_unset(request.consumer_group_id):
             query['ConsumerGroupId'] = request.consumer_group_id
         if not UtilClient.is_unset(request.dts_instance_id):
             query['DtsInstanceId'] = request.dts_instance_id
         if not UtilClient.is_unset(request.dts_job_id):
@@ -2980,29 +3202,42 @@
             await self.call_api_async(params, req, runtime)
         )
 
     def delete_consumer_channel(
         self,
         request: dts_20200101_models.DeleteConsumerChannelRequest,
     ) -> dts_20200101_models.DeleteConsumerChannelResponse:
+        """
+        @param request: DeleteConsumerChannelRequest
+        @return: DeleteConsumerChannelResponse
+        """
         runtime = util_models.RuntimeOptions()
         return self.delete_consumer_channel_with_options(request, runtime)
 
     async def delete_consumer_channel_async(
         self,
         request: dts_20200101_models.DeleteConsumerChannelRequest,
     ) -> dts_20200101_models.DeleteConsumerChannelResponse:
+        """
+        @param request: DeleteConsumerChannelRequest
+        @return: DeleteConsumerChannelResponse
+        """
         runtime = util_models.RuntimeOptions()
         return await self.delete_consumer_channel_with_options_async(request, runtime)
 
     def delete_consumer_group_with_options(
         self,
         request: dts_20200101_models.DeleteConsumerGroupRequest,
         runtime: util_models.RuntimeOptions,
     ) -> dts_20200101_models.DeleteConsumerGroupResponse:
+        """
+        @param request: DeleteConsumerGroupRequest
+        @param runtime: runtime options for this request RuntimeOptions
+        @return: DeleteConsumerGroupResponse
+        """
         UtilClient.validate_model(request)
         query = {}
         if not UtilClient.is_unset(request.account_id):
             query['AccountId'] = request.account_id
         if not UtilClient.is_unset(request.consumer_group_id):
             query['ConsumerGroupID'] = request.consumer_group_id
         if not UtilClient.is_unset(request.owner_id):
@@ -3033,14 +3268,19 @@
         )
 
     async def delete_consumer_group_with_options_async(
         self,
         request: dts_20200101_models.DeleteConsumerGroupRequest,
         runtime: util_models.RuntimeOptions,
     ) -> dts_20200101_models.DeleteConsumerGroupResponse:
+        """
+        @param request: DeleteConsumerGroupRequest
+        @param runtime: runtime options for this request RuntimeOptions
+        @return: DeleteConsumerGroupResponse
+        """
         UtilClient.validate_model(request)
         query = {}
         if not UtilClient.is_unset(request.account_id):
             query['AccountId'] = request.account_id
         if not UtilClient.is_unset(request.consumer_group_id):
             query['ConsumerGroupID'] = request.consumer_group_id
         if not UtilClient.is_unset(request.owner_id):
@@ -3070,29 +3310,44 @@
             await self.call_api_async(params, req, runtime)
         )
 
     def delete_consumer_group(
         self,
         request: dts_20200101_models.DeleteConsumerGroupRequest,
     ) -> dts_20200101_models.DeleteConsumerGroupResponse:
+        """
+        @param request: DeleteConsumerGroupRequest
+        @return: DeleteConsumerGroupResponse
+        """
         runtime = util_models.RuntimeOptions()
         return self.delete_consumer_group_with_options(request, runtime)
 
     async def delete_consumer_group_async(
         self,
         request: dts_20200101_models.DeleteConsumerGroupRequest,
     ) -> dts_20200101_models.DeleteConsumerGroupResponse:
+        """
+        @param request: DeleteConsumerGroupRequest
+        @return: DeleteConsumerGroupResponse
+        """
         runtime = util_models.RuntimeOptions()
         return await self.delete_consumer_group_with_options_async(request, runtime)
 
     def delete_dts_job_with_options(
         self,
         request: dts_20200101_models.DeleteDtsJobRequest,
         runtime: util_models.RuntimeOptions,
     ) -> dts_20200101_models.DeleteDtsJobResponse:
+        """
+        @summary The HTTP status code.
+        
+        @param request: DeleteDtsJobRequest
+        @param runtime: runtime options for this request RuntimeOptions
+        @return: DeleteDtsJobResponse
+        """
         UtilClient.validate_model(request)
         query = {}
         if not UtilClient.is_unset(request.dts_instance_id):
             query['DtsInstanceId'] = request.dts_instance_id
         if not UtilClient.is_unset(request.dts_job_id):
             query['DtsJobId'] = request.dts_job_id
         if not UtilClient.is_unset(request.job_type):
@@ -3125,14 +3380,21 @@
         )
 
     async def delete_dts_job_with_options_async(
         self,
         request: dts_20200101_models.DeleteDtsJobRequest,
         runtime: util_models.RuntimeOptions,
     ) -> dts_20200101_models.DeleteDtsJobResponse:
+        """
+        @summary The HTTP status code.
+        
+        @param request: DeleteDtsJobRequest
+        @param runtime: runtime options for this request RuntimeOptions
+        @return: DeleteDtsJobResponse
+        """
         UtilClient.validate_model(request)
         query = {}
         if not UtilClient.is_unset(request.dts_instance_id):
             query['DtsInstanceId'] = request.dts_instance_id
         if not UtilClient.is_unset(request.dts_job_id):
             query['DtsJobId'] = request.dts_job_id
         if not UtilClient.is_unset(request.job_type):
@@ -3164,29 +3426,48 @@
             await self.call_api_async(params, req, runtime)
         )
 
     def delete_dts_job(
         self,
         request: dts_20200101_models.DeleteDtsJobRequest,
     ) -> dts_20200101_models.DeleteDtsJobResponse:
+        """
+        @summary The HTTP status code.
+        
+        @param request: DeleteDtsJobRequest
+        @return: DeleteDtsJobResponse
+        """
         runtime = util_models.RuntimeOptions()
         return self.delete_dts_job_with_options(request, runtime)
 
     async def delete_dts_job_async(
         self,
         request: dts_20200101_models.DeleteDtsJobRequest,
     ) -> dts_20200101_models.DeleteDtsJobResponse:
+        """
+        @summary The HTTP status code.
+        
+        @param request: DeleteDtsJobRequest
+        @return: DeleteDtsJobResponse
+        """
         runtime = util_models.RuntimeOptions()
         return await self.delete_dts_job_with_options_async(request, runtime)
 
     def delete_dts_jobs_with_options(
         self,
         request: dts_20200101_models.DeleteDtsJobsRequest,
         runtime: util_models.RuntimeOptions,
     ) -> dts_20200101_models.DeleteDtsJobsResponse:
+        """
+        @summary Deletes multiple data migration, data synchronization, or change tracking tasks.
+        
+        @param request: DeleteDtsJobsRequest
+        @param runtime: runtime options for this request RuntimeOptions
+        @return: DeleteDtsJobsResponse
+        """
         UtilClient.validate_model(request)
         query = {}
         if not UtilClient.is_unset(request.dts_job_ids):
             query['DtsJobIds'] = request.dts_job_ids
         if not UtilClient.is_unset(request.region_id):
             query['RegionId'] = request.region_id
         if not UtilClient.is_unset(request.resource_group_id):
@@ -3213,14 +3494,21 @@
         )
 
     async def delete_dts_jobs_with_options_async(
         self,
         request: dts_20200101_models.DeleteDtsJobsRequest,
         runtime: util_models.RuntimeOptions,
     ) -> dts_20200101_models.DeleteDtsJobsResponse:
+        """
+        @summary Deletes multiple data migration, data synchronization, or change tracking tasks.
+        
+        @param request: DeleteDtsJobsRequest
+        @param runtime: runtime options for this request RuntimeOptions
+        @return: DeleteDtsJobsResponse
+        """
         UtilClient.validate_model(request)
         query = {}
         if not UtilClient.is_unset(request.dts_job_ids):
             query['DtsJobIds'] = request.dts_job_ids
         if not UtilClient.is_unset(request.region_id):
             query['RegionId'] = request.region_id
         if not UtilClient.is_unset(request.resource_group_id):
@@ -3246,31 +3534,43 @@
             await self.call_api_async(params, req, runtime)
         )
 
     def delete_dts_jobs(
         self,
         request: dts_20200101_models.DeleteDtsJobsRequest,
     ) -> dts_20200101_models.DeleteDtsJobsResponse:
+        """
+        @summary Deletes multiple data migration, data synchronization, or change tracking tasks.
+        
+        @param request: DeleteDtsJobsRequest
+        @return: DeleteDtsJobsResponse
+        """
         runtime = util_models.RuntimeOptions()
         return self.delete_dts_jobs_with_options(request, runtime)
 
     async def delete_dts_jobs_async(
         self,
         request: dts_20200101_models.DeleteDtsJobsRequest,
     ) -> dts_20200101_models.DeleteDtsJobsResponse:
+        """
+        @summary Deletes multiple data migration, data synchronization, or change tracking tasks.
+        
+        @param request: DeleteDtsJobsRequest
+        @return: DeleteDtsJobsResponse
+        """
         runtime = util_models.RuntimeOptions()
         return await self.delete_dts_jobs_with_options_async(request, runtime)
 
     def delete_migration_job_with_options(
         self,
         request: dts_20200101_models.DeleteMigrationJobRequest,
         runtime: util_models.RuntimeOptions,
     ) -> dts_20200101_models.DeleteMigrationJobResponse:
         """
-        >  After a data migration instance is released, it cannot be recovered.
+        @description >  After a data migration instance is released, it cannot be recovered.
         
         @param request: DeleteMigrationJobRequest
         @param runtime: runtime options for this request RuntimeOptions
         @return: DeleteMigrationJobResponse
         """
         UtilClient.validate_model(request)
         query = {}
@@ -3305,15 +3605,15 @@
 
     async def delete_migration_job_with_options_async(
         self,
         request: dts_20200101_models.DeleteMigrationJobRequest,
         runtime: util_models.RuntimeOptions,
     ) -> dts_20200101_models.DeleteMigrationJobResponse:
         """
-        >  After a data migration instance is released, it cannot be recovered.
+        @description >  After a data migration instance is released, it cannot be recovered.
         
         @param request: DeleteMigrationJobRequest
         @param runtime: runtime options for this request RuntimeOptions
         @return: DeleteMigrationJobResponse
         """
         UtilClient.validate_model(request)
         query = {}
@@ -3347,42 +3647,42 @@
         )
 
     def delete_migration_job(
         self,
         request: dts_20200101_models.DeleteMigrationJobRequest,
     ) -> dts_20200101_models.DeleteMigrationJobResponse:
         """
-        >  After a data migration instance is released, it cannot be recovered.
+        @description >  After a data migration instance is released, it cannot be recovered.
         
         @param request: DeleteMigrationJobRequest
         @return: DeleteMigrationJobResponse
         """
         runtime = util_models.RuntimeOptions()
         return self.delete_migration_job_with_options(request, runtime)
 
     async def delete_migration_job_async(
         self,
         request: dts_20200101_models.DeleteMigrationJobRequest,
     ) -> dts_20200101_models.DeleteMigrationJobResponse:
         """
-        >  After a data migration instance is released, it cannot be recovered.
+        @description >  After a data migration instance is released, it cannot be recovered.
         
         @param request: DeleteMigrationJobRequest
         @return: DeleteMigrationJobResponse
         """
         runtime = util_models.RuntimeOptions()
         return await self.delete_migration_job_with_options_async(request, runtime)
 
     def delete_subscription_instance_with_options(
         self,
         request: dts_20200101_models.DeleteSubscriptionInstanceRequest,
         runtime: util_models.RuntimeOptions,
     ) -> dts_20200101_models.DeleteSubscriptionInstanceResponse:
         """
-        >  After a change tracking instance is released, it cannot be recovered.
+        @description >  After a change tracking instance is released, it cannot be recovered.
         
         @param request: DeleteSubscriptionInstanceRequest
         @param runtime: runtime options for this request RuntimeOptions
         @return: DeleteSubscriptionInstanceResponse
         """
         UtilClient.validate_model(request)
         query = {}
@@ -3417,15 +3717,15 @@
 
     async def delete_subscription_instance_with_options_async(
         self,
         request: dts_20200101_models.DeleteSubscriptionInstanceRequest,
         runtime: util_models.RuntimeOptions,
     ) -> dts_20200101_models.DeleteSubscriptionInstanceResponse:
         """
-        >  After a change tracking instance is released, it cannot be recovered.
+        @description >  After a change tracking instance is released, it cannot be recovered.
         
         @param request: DeleteSubscriptionInstanceRequest
         @param runtime: runtime options for this request RuntimeOptions
         @return: DeleteSubscriptionInstanceResponse
         """
         UtilClient.validate_model(request)
         query = {}
@@ -3459,42 +3759,42 @@
         )
 
     def delete_subscription_instance(
         self,
         request: dts_20200101_models.DeleteSubscriptionInstanceRequest,
     ) -> dts_20200101_models.DeleteSubscriptionInstanceResponse:
         """
-        >  After a change tracking instance is released, it cannot be recovered.
+        @description >  After a change tracking instance is released, it cannot be recovered.
         
         @param request: DeleteSubscriptionInstanceRequest
         @return: DeleteSubscriptionInstanceResponse
         """
         runtime = util_models.RuntimeOptions()
         return self.delete_subscription_instance_with_options(request, runtime)
 
     async def delete_subscription_instance_async(
         self,
         request: dts_20200101_models.DeleteSubscriptionInstanceRequest,
     ) -> dts_20200101_models.DeleteSubscriptionInstanceResponse:
         """
-        >  After a change tracking instance is released, it cannot be recovered.
+        @description >  After a change tracking instance is released, it cannot be recovered.
         
         @param request: DeleteSubscriptionInstanceRequest
         @return: DeleteSubscriptionInstanceResponse
         """
         runtime = util_models.RuntimeOptions()
         return await self.delete_subscription_instance_with_options_async(request, runtime)
 
     def delete_synchronization_job_with_options(
         self,
         request: dts_20200101_models.DeleteSynchronizationJobRequest,
         runtime: util_models.RuntimeOptions,
     ) -> dts_20200101_models.DeleteSynchronizationJobResponse:
         """
-        >  After a data synchronization instance is released, it cannot be recovered.
+        @description >  After a data synchronization instance is released, it cannot be recovered.
         
         @param request: DeleteSynchronizationJobRequest
         @param runtime: runtime options for this request RuntimeOptions
         @return: DeleteSynchronizationJobResponse
         """
         UtilClient.validate_model(request)
         query = {}
@@ -3529,15 +3829,15 @@
 
     async def delete_synchronization_job_with_options_async(
         self,
         request: dts_20200101_models.DeleteSynchronizationJobRequest,
         runtime: util_models.RuntimeOptions,
     ) -> dts_20200101_models.DeleteSynchronizationJobResponse:
         """
-        >  After a data synchronization instance is released, it cannot be recovered.
+        @description >  After a data synchronization instance is released, it cannot be recovered.
         
         @param request: DeleteSynchronizationJobRequest
         @param runtime: runtime options for this request RuntimeOptions
         @return: DeleteSynchronizationJobResponse
         """
         UtilClient.validate_model(request)
         query = {}
@@ -3571,40 +3871,47 @@
         )
 
     def delete_synchronization_job(
         self,
         request: dts_20200101_models.DeleteSynchronizationJobRequest,
     ) -> dts_20200101_models.DeleteSynchronizationJobResponse:
         """
-        >  After a data synchronization instance is released, it cannot be recovered.
+        @description >  After a data synchronization instance is released, it cannot be recovered.
         
         @param request: DeleteSynchronizationJobRequest
         @return: DeleteSynchronizationJobResponse
         """
         runtime = util_models.RuntimeOptions()
         return self.delete_synchronization_job_with_options(request, runtime)
 
     async def delete_synchronization_job_async(
         self,
         request: dts_20200101_models.DeleteSynchronizationJobRequest,
     ) -> dts_20200101_models.DeleteSynchronizationJobResponse:
         """
-        >  After a data synchronization instance is released, it cannot be recovered.
+        @description >  After a data synchronization instance is released, it cannot be recovered.
         
         @param request: DeleteSynchronizationJobRequest
         @return: DeleteSynchronizationJobResponse
         """
         runtime = util_models.RuntimeOptions()
         return await self.delete_synchronization_job_with_options_async(request, runtime)
 
     def describe_channel_account_with_options(
         self,
         request: dts_20200101_models.DescribeChannelAccountRequest,
         runtime: util_models.RuntimeOptions,
     ) -> dts_20200101_models.DescribeChannelAccountResponse:
+        """
+        @summary 查询数据投递链路store账号
+        
+        @param request: DescribeChannelAccountRequest
+        @param runtime: runtime options for this request RuntimeOptions
+        @return: DescribeChannelAccountResponse
+        """
         UtilClient.validate_model(request)
         query = {}
         if not UtilClient.is_unset(request.dts_job_id):
             query['DtsJobId'] = request.dts_job_id
         if not UtilClient.is_unset(request.owner_id):
             query['OwnerId'] = request.owner_id
         if not UtilClient.is_unset(request.region):
@@ -3637,14 +3944,21 @@
         )
 
     async def describe_channel_account_with_options_async(
         self,
         request: dts_20200101_models.DescribeChannelAccountRequest,
         runtime: util_models.RuntimeOptions,
     ) -> dts_20200101_models.DescribeChannelAccountResponse:
+        """
+        @summary 查询数据投递链路store账号
+        
+        @param request: DescribeChannelAccountRequest
+        @param runtime: runtime options for this request RuntimeOptions
+        @return: DescribeChannelAccountResponse
+        """
         UtilClient.validate_model(request)
         query = {}
         if not UtilClient.is_unset(request.dts_job_id):
             query['DtsJobId'] = request.dts_job_id
         if not UtilClient.is_unset(request.owner_id):
             query['OwnerId'] = request.owner_id
         if not UtilClient.is_unset(request.region):
@@ -3676,29 +3990,48 @@
             await self.call_api_async(params, req, runtime)
         )
 
     def describe_channel_account(
         self,
         request: dts_20200101_models.DescribeChannelAccountRequest,
     ) -> dts_20200101_models.DescribeChannelAccountResponse:
+        """
+        @summary 查询数据投递链路store账号
+        
+        @param request: DescribeChannelAccountRequest
+        @return: DescribeChannelAccountResponse
+        """
         runtime = util_models.RuntimeOptions()
         return self.describe_channel_account_with_options(request, runtime)
 
     async def describe_channel_account_async(
         self,
         request: dts_20200101_models.DescribeChannelAccountRequest,
     ) -> dts_20200101_models.DescribeChannelAccountResponse:
+        """
+        @summary 查询数据投递链路store账号
+        
+        @param request: DescribeChannelAccountRequest
+        @return: DescribeChannelAccountResponse
+        """
         runtime = util_models.RuntimeOptions()
         return await self.describe_channel_account_with_options_async(request, runtime)
 
     def describe_check_jobs_with_options(
         self,
         request: dts_20200101_models.DescribeCheckJobsRequest,
         runtime: util_models.RuntimeOptions,
     ) -> dts_20200101_models.DescribeCheckJobsResponse:
+        """
+        @summary 请求所有数据校验任务数据
+        
+        @param request: DescribeCheckJobsRequest
+        @param runtime: runtime options for this request RuntimeOptions
+        @return: DescribeCheckJobsResponse
+        """
         UtilClient.validate_model(request)
         query = {}
         if not UtilClient.is_unset(request.check_type):
             query['CheckType'] = request.check_type
         if not UtilClient.is_unset(request.instance_id):
             query['InstanceId'] = request.instance_id
         if not UtilClient.is_unset(request.job_name):
@@ -3729,14 +4062,21 @@
         )
 
     async def describe_check_jobs_with_options_async(
         self,
         request: dts_20200101_models.DescribeCheckJobsRequest,
         runtime: util_models.RuntimeOptions,
     ) -> dts_20200101_models.DescribeCheckJobsResponse:
+        """
+        @summary 请求所有数据校验任务数据
+        
+        @param request: DescribeCheckJobsRequest
+        @param runtime: runtime options for this request RuntimeOptions
+        @return: DescribeCheckJobsResponse
+        """
         UtilClient.validate_model(request)
         query = {}
         if not UtilClient.is_unset(request.check_type):
             query['CheckType'] = request.check_type
         if not UtilClient.is_unset(request.instance_id):
             query['InstanceId'] = request.instance_id
         if not UtilClient.is_unset(request.job_name):
@@ -3766,29 +4106,48 @@
             await self.call_api_async(params, req, runtime)
         )
 
     def describe_check_jobs(
         self,
         request: dts_20200101_models.DescribeCheckJobsRequest,
     ) -> dts_20200101_models.DescribeCheckJobsResponse:
+        """
+        @summary 请求所有数据校验任务数据
+        
+        @param request: DescribeCheckJobsRequest
+        @return: DescribeCheckJobsResponse
+        """
         runtime = util_models.RuntimeOptions()
         return self.describe_check_jobs_with_options(request, runtime)
 
     async def describe_check_jobs_async(
         self,
         request: dts_20200101_models.DescribeCheckJobsRequest,
     ) -> dts_20200101_models.DescribeCheckJobsResponse:
+        """
+        @summary 请求所有数据校验任务数据
+        
+        @param request: DescribeCheckJobsRequest
+        @return: DescribeCheckJobsResponse
+        """
         runtime = util_models.RuntimeOptions()
         return await self.describe_check_jobs_with_options_async(request, runtime)
 
     def describe_cluster_operate_logs_with_options(
         self,
         request: dts_20200101_models.DescribeClusterOperateLogsRequest,
         runtime: util_models.RuntimeOptions,
     ) -> dts_20200101_models.DescribeClusterOperateLogsResponse:
+        """
+        @summary Queries operation logs of a Data Transmission Service (DTS) dedicated cluster.
+        
+        @param request: DescribeClusterOperateLogsRequest
+        @param runtime: runtime options for this request RuntimeOptions
+        @return: DescribeClusterOperateLogsResponse
+        """
         UtilClient.validate_model(request)
         query = {}
         if not UtilClient.is_unset(request.resource_group_id):
             query['ResourceGroupId'] = request.resource_group_id
         body = {}
         if not UtilClient.is_unset(request.account_id):
             body['AccountId'] = request.account_id
@@ -3829,14 +4188,21 @@
         )
 
     async def describe_cluster_operate_logs_with_options_async(
         self,
         request: dts_20200101_models.DescribeClusterOperateLogsRequest,
         runtime: util_models.RuntimeOptions,
     ) -> dts_20200101_models.DescribeClusterOperateLogsResponse:
+        """
+        @summary Queries operation logs of a Data Transmission Service (DTS) dedicated cluster.
+        
+        @param request: DescribeClusterOperateLogsRequest
+        @param runtime: runtime options for this request RuntimeOptions
+        @return: DescribeClusterOperateLogsResponse
+        """
         UtilClient.validate_model(request)
         query = {}
         if not UtilClient.is_unset(request.resource_group_id):
             query['ResourceGroupId'] = request.resource_group_id
         body = {}
         if not UtilClient.is_unset(request.account_id):
             body['AccountId'] = request.account_id
@@ -3876,29 +4242,48 @@
             await self.call_api_async(params, req, runtime)
         )
 
     def describe_cluster_operate_logs(
         self,
         request: dts_20200101_models.DescribeClusterOperateLogsRequest,
     ) -> dts_20200101_models.DescribeClusterOperateLogsResponse:
+        """
+        @summary Queries operation logs of a Data Transmission Service (DTS) dedicated cluster.
+        
+        @param request: DescribeClusterOperateLogsRequest
+        @return: DescribeClusterOperateLogsResponse
+        """
         runtime = util_models.RuntimeOptions()
         return self.describe_cluster_operate_logs_with_options(request, runtime)
 
     async def describe_cluster_operate_logs_async(
         self,
         request: dts_20200101_models.DescribeClusterOperateLogsRequest,
     ) -> dts_20200101_models.DescribeClusterOperateLogsResponse:
+        """
+        @summary Queries operation logs of a Data Transmission Service (DTS) dedicated cluster.
+        
+        @param request: DescribeClusterOperateLogsRequest
+        @return: DescribeClusterOperateLogsResponse
+        """
         runtime = util_models.RuntimeOptions()
         return await self.describe_cluster_operate_logs_with_options_async(request, runtime)
 
     def describe_cluster_used_utilization_with_options(
         self,
         request: dts_20200101_models.DescribeClusterUsedUtilizationRequest,
         runtime: util_models.RuntimeOptions,
     ) -> dts_20200101_models.DescribeClusterUsedUtilizationResponse:
+        """
+        @summary Queries the resource usage of a cluster.
+        
+        @param request: DescribeClusterUsedUtilizationRequest
+        @param runtime: runtime options for this request RuntimeOptions
+        @return: DescribeClusterUsedUtilizationResponse
+        """
         UtilClient.validate_model(request)
         query = {}
         if not UtilClient.is_unset(request.resource_group_id):
             query['ResourceGroupId'] = request.resource_group_id
         body = {}
         if not UtilClient.is_unset(request.account_id):
             body['AccountId'] = request.account_id
@@ -3939,14 +4324,21 @@
         )
 
     async def describe_cluster_used_utilization_with_options_async(
         self,
         request: dts_20200101_models.DescribeClusterUsedUtilizationRequest,
         runtime: util_models.RuntimeOptions,
     ) -> dts_20200101_models.DescribeClusterUsedUtilizationResponse:
+        """
+        @summary Queries the resource usage of a cluster.
+        
+        @param request: DescribeClusterUsedUtilizationRequest
+        @param runtime: runtime options for this request RuntimeOptions
+        @return: DescribeClusterUsedUtilizationResponse
+        """
         UtilClient.validate_model(request)
         query = {}
         if not UtilClient.is_unset(request.resource_group_id):
             query['ResourceGroupId'] = request.resource_group_id
         body = {}
         if not UtilClient.is_unset(request.account_id):
             body['AccountId'] = request.account_id
@@ -3986,29 +4378,46 @@
             await self.call_api_async(params, req, runtime)
         )
 
     def describe_cluster_used_utilization(
         self,
         request: dts_20200101_models.DescribeClusterUsedUtilizationRequest,
     ) -> dts_20200101_models.DescribeClusterUsedUtilizationResponse:
+        """
+        @summary Queries the resource usage of a cluster.
+        
+        @param request: DescribeClusterUsedUtilizationRequest
+        @return: DescribeClusterUsedUtilizationResponse
+        """
         runtime = util_models.RuntimeOptions()
         return self.describe_cluster_used_utilization_with_options(request, runtime)
 
     async def describe_cluster_used_utilization_async(
         self,
         request: dts_20200101_models.DescribeClusterUsedUtilizationRequest,
     ) -> dts_20200101_models.DescribeClusterUsedUtilizationResponse:
+        """
+        @summary Queries the resource usage of a cluster.
+        
+        @param request: DescribeClusterUsedUtilizationRequest
+        @return: DescribeClusterUsedUtilizationResponse
+        """
         runtime = util_models.RuntimeOptions()
         return await self.describe_cluster_used_utilization_with_options_async(request, runtime)
 
     def describe_connection_status_with_options(
         self,
         request: dts_20200101_models.DescribeConnectionStatusRequest,
         runtime: util_models.RuntimeOptions,
     ) -> dts_20200101_models.DescribeConnectionStatusResponse:
+        """
+        @param request: DescribeConnectionStatusRequest
+        @param runtime: runtime options for this request RuntimeOptions
+        @return: DescribeConnectionStatusResponse
+        """
         UtilClient.validate_model(request)
         query = {}
         if not UtilClient.is_unset(request.destination_endpoint_architecture):
             query['DestinationEndpointArchitecture'] = request.destination_endpoint_architecture
         if not UtilClient.is_unset(request.destination_endpoint_database_name):
             query['DestinationEndpointDatabaseName'] = request.destination_endpoint_database_name
         if not UtilClient.is_unset(request.destination_endpoint_engine_name):
@@ -4075,14 +4484,19 @@
         )
 
     async def describe_connection_status_with_options_async(
         self,
         request: dts_20200101_models.DescribeConnectionStatusRequest,
         runtime: util_models.RuntimeOptions,
     ) -> dts_20200101_models.DescribeConnectionStatusResponse:
+        """
+        @param request: DescribeConnectionStatusRequest
+        @param runtime: runtime options for this request RuntimeOptions
+        @return: DescribeConnectionStatusResponse
+        """
         UtilClient.validate_model(request)
         query = {}
         if not UtilClient.is_unset(request.destination_endpoint_architecture):
             query['DestinationEndpointArchitecture'] = request.destination_endpoint_architecture
         if not UtilClient.is_unset(request.destination_endpoint_database_name):
             query['DestinationEndpointDatabaseName'] = request.destination_endpoint_database_name
         if not UtilClient.is_unset(request.destination_endpoint_engine_name):
@@ -4148,29 +4562,42 @@
             await self.call_api_async(params, req, runtime)
         )
 
     def describe_connection_status(
         self,
         request: dts_20200101_models.DescribeConnectionStatusRequest,
     ) -> dts_20200101_models.DescribeConnectionStatusResponse:
+        """
+        @param request: DescribeConnectionStatusRequest
+        @return: DescribeConnectionStatusResponse
+        """
         runtime = util_models.RuntimeOptions()
         return self.describe_connection_status_with_options(request, runtime)
 
     async def describe_connection_status_async(
         self,
         request: dts_20200101_models.DescribeConnectionStatusRequest,
     ) -> dts_20200101_models.DescribeConnectionStatusResponse:
+        """
+        @param request: DescribeConnectionStatusRequest
+        @return: DescribeConnectionStatusResponse
+        """
         runtime = util_models.RuntimeOptions()
         return await self.describe_connection_status_with_options_async(request, runtime)
 
     def describe_consumer_channel_with_options(
         self,
         request: dts_20200101_models.DescribeConsumerChannelRequest,
         runtime: util_models.RuntimeOptions,
     ) -> dts_20200101_models.DescribeConsumerChannelResponse:
+        """
+        @param request: DescribeConsumerChannelRequest
+        @param runtime: runtime options for this request RuntimeOptions
+        @return: DescribeConsumerChannelResponse
+        """
         UtilClient.validate_model(request)
         query = {}
         if not UtilClient.is_unset(request.dts_instance_id):
             query['DtsInstanceId'] = request.dts_instance_id
         if not UtilClient.is_unset(request.dts_job_id):
             query['DtsJobId'] = request.dts_job_id
         if not UtilClient.is_unset(request.page_number):
@@ -4203,14 +4630,19 @@
         )
 
     async def describe_consumer_channel_with_options_async(
         self,
         request: dts_20200101_models.DescribeConsumerChannelRequest,
         runtime: util_models.RuntimeOptions,
     ) -> dts_20200101_models.DescribeConsumerChannelResponse:
+        """
+        @param request: DescribeConsumerChannelRequest
+        @param runtime: runtime options for this request RuntimeOptions
+        @return: DescribeConsumerChannelResponse
+        """
         UtilClient.validate_model(request)
         query = {}
         if not UtilClient.is_unset(request.dts_instance_id):
             query['DtsInstanceId'] = request.dts_instance_id
         if not UtilClient.is_unset(request.dts_job_id):
             query['DtsJobId'] = request.dts_job_id
         if not UtilClient.is_unset(request.page_number):
@@ -4242,29 +4674,44 @@
             await self.call_api_async(params, req, runtime)
         )
 
     def describe_consumer_channel(
         self,
         request: dts_20200101_models.DescribeConsumerChannelRequest,
     ) -> dts_20200101_models.DescribeConsumerChannelResponse:
+        """
+        @param request: DescribeConsumerChannelRequest
+        @return: DescribeConsumerChannelResponse
+        """
         runtime = util_models.RuntimeOptions()
         return self.describe_consumer_channel_with_options(request, runtime)
 
     async def describe_consumer_channel_async(
         self,
         request: dts_20200101_models.DescribeConsumerChannelRequest,
     ) -> dts_20200101_models.DescribeConsumerChannelResponse:
+        """
+        @param request: DescribeConsumerChannelRequest
+        @return: DescribeConsumerChannelResponse
+        """
         runtime = util_models.RuntimeOptions()
         return await self.describe_consumer_channel_with_options_async(request, runtime)
 
     def describe_consumer_group_with_options(
         self,
         request: dts_20200101_models.DescribeConsumerGroupRequest,
         runtime: util_models.RuntimeOptions,
     ) -> dts_20200101_models.DescribeConsumerGroupResponse:
+        """
+        @summary Queries the details of consumer groups in a change tracking instance.
+        
+        @param request: DescribeConsumerGroupRequest
+        @param runtime: runtime options for this request RuntimeOptions
+        @return: DescribeConsumerGroupResponse
+        """
         UtilClient.validate_model(request)
         query = {}
         if not UtilClient.is_unset(request.account_id):
             query['AccountId'] = request.account_id
         if not UtilClient.is_unset(request.owner_id):
             query['OwnerId'] = request.owner_id
         if not UtilClient.is_unset(request.page_num):
@@ -4297,14 +4744,21 @@
         )
 
     async def describe_consumer_group_with_options_async(
         self,
         request: dts_20200101_models.DescribeConsumerGroupRequest,
         runtime: util_models.RuntimeOptions,
     ) -> dts_20200101_models.DescribeConsumerGroupResponse:
+        """
+        @summary Queries the details of consumer groups in a change tracking instance.
+        
+        @param request: DescribeConsumerGroupRequest
+        @param runtime: runtime options for this request RuntimeOptions
+        @return: DescribeConsumerGroupResponse
+        """
         UtilClient.validate_model(request)
         query = {}
         if not UtilClient.is_unset(request.account_id):
             query['AccountId'] = request.account_id
         if not UtilClient.is_unset(request.owner_id):
             query['OwnerId'] = request.owner_id
         if not UtilClient.is_unset(request.page_num):
@@ -4336,32 +4790,44 @@
             await self.call_api_async(params, req, runtime)
         )
 
     def describe_consumer_group(
         self,
         request: dts_20200101_models.DescribeConsumerGroupRequest,
     ) -> dts_20200101_models.DescribeConsumerGroupResponse:
+        """
+        @summary Queries the details of consumer groups in a change tracking instance.
+        
+        @param request: DescribeConsumerGroupRequest
+        @return: DescribeConsumerGroupResponse
+        """
         runtime = util_models.RuntimeOptions()
         return self.describe_consumer_group_with_options(request, runtime)
 
     async def describe_consumer_group_async(
         self,
         request: dts_20200101_models.DescribeConsumerGroupRequest,
     ) -> dts_20200101_models.DescribeConsumerGroupResponse:
+        """
+        @summary Queries the details of consumer groups in a change tracking instance.
+        
+        @param request: DescribeConsumerGroupRequest
+        @return: DescribeConsumerGroupResponse
+        """
         runtime = util_models.RuntimeOptions()
         return await self.describe_consumer_group_with_options_async(request, runtime)
 
     def describe_dtsipwith_options(
         self,
         request: dts_20200101_models.DescribeDTSIPRequest,
         runtime: util_models.RuntimeOptions,
     ) -> dts_20200101_models.DescribeDTSIPResponse:
         """
-        If the *source or destination instance** is an **on-premises database**, you need to call this operation to query the CIDR blocks of DTS servers. Then, you need to add the CIDR blocks of DTS servers to the security settings of the source or destination instance, for example, the firewall of your database. For more information, see [Add the CIDR blocks of DTS servers to the security settings of on-premises databases](~~176627~~).
-        >  If the **source or destination database** is an **ApsaraDB database instance** (such as RDS instance and ApsaraDB for MongoDB instance) or a **self-managed database hosted on ECS**, you do not need to add the CIDR blocks. When you click **Set Whitelist and Next** in the DTS console, DTS automatically add the CIDR blocks of DTS servers to the security settings of the source or destination instance.
+        @description If the *source or destination instance** is an **on-premises database**, you need to call this operation to query the CIDR blocks of DTS servers. Then, you need to add the CIDR blocks of DTS servers to the security settings of the source or destination instance, for example, the firewall of your database. For more information, see [Add the CIDR blocks of DTS servers to the security settings of on-premises databases](https://help.aliyun.com/document_detail/176627.html).
+        >  If the *source or destination database** is an **ApsaraDB database instance** (such as RDS instance and ApsaraDB for MongoDB instance) or a **self-managed database hosted on ECS**, you do not need to add the CIDR blocks. When you click **Set Whitelist and Next** in the DTS console, DTS automatically add the CIDR blocks of DTS servers to the security settings of the source or destination instance.
         
         @param request: DescribeDTSIPRequest
         @param runtime: runtime options for this request RuntimeOptions
         @return: DescribeDTSIPResponse
         """
         UtilClient.validate_model(request)
         query = {}
@@ -4394,16 +4860,16 @@
 
     async def describe_dtsipwith_options_async(
         self,
         request: dts_20200101_models.DescribeDTSIPRequest,
         runtime: util_models.RuntimeOptions,
     ) -> dts_20200101_models.DescribeDTSIPResponse:
         """
-        If the *source or destination instance** is an **on-premises database**, you need to call this operation to query the CIDR blocks of DTS servers. Then, you need to add the CIDR blocks of DTS servers to the security settings of the source or destination instance, for example, the firewall of your database. For more information, see [Add the CIDR blocks of DTS servers to the security settings of on-premises databases](~~176627~~).
-        >  If the **source or destination database** is an **ApsaraDB database instance** (such as RDS instance and ApsaraDB for MongoDB instance) or a **self-managed database hosted on ECS**, you do not need to add the CIDR blocks. When you click **Set Whitelist and Next** in the DTS console, DTS automatically add the CIDR blocks of DTS servers to the security settings of the source or destination instance.
+        @description If the *source or destination instance** is an **on-premises database**, you need to call this operation to query the CIDR blocks of DTS servers. Then, you need to add the CIDR blocks of DTS servers to the security settings of the source or destination instance, for example, the firewall of your database. For more information, see [Add the CIDR blocks of DTS servers to the security settings of on-premises databases](https://help.aliyun.com/document_detail/176627.html).
+        >  If the *source or destination database** is an **ApsaraDB database instance** (such as RDS instance and ApsaraDB for MongoDB instance) or a **self-managed database hosted on ECS**, you do not need to add the CIDR blocks. When you click **Set Whitelist and Next** in the DTS console, DTS automatically add the CIDR blocks of DTS servers to the security settings of the source or destination instance.
         
         @param request: DescribeDTSIPRequest
         @param runtime: runtime options for this request RuntimeOptions
         @return: DescribeDTSIPResponse
         """
         UtilClient.validate_model(request)
         query = {}
@@ -4435,42 +4901,49 @@
         )
 
     def describe_dtsip(
         self,
         request: dts_20200101_models.DescribeDTSIPRequest,
     ) -> dts_20200101_models.DescribeDTSIPResponse:
         """
-        If the *source or destination instance** is an **on-premises database**, you need to call this operation to query the CIDR blocks of DTS servers. Then, you need to add the CIDR blocks of DTS servers to the security settings of the source or destination instance, for example, the firewall of your database. For more information, see [Add the CIDR blocks of DTS servers to the security settings of on-premises databases](~~176627~~).
-        >  If the **source or destination database** is an **ApsaraDB database instance** (such as RDS instance and ApsaraDB for MongoDB instance) or a **self-managed database hosted on ECS**, you do not need to add the CIDR blocks. When you click **Set Whitelist and Next** in the DTS console, DTS automatically add the CIDR blocks of DTS servers to the security settings of the source or destination instance.
+        @description If the *source or destination instance** is an **on-premises database**, you need to call this operation to query the CIDR blocks of DTS servers. Then, you need to add the CIDR blocks of DTS servers to the security settings of the source or destination instance, for example, the firewall of your database. For more information, see [Add the CIDR blocks of DTS servers to the security settings of on-premises databases](https://help.aliyun.com/document_detail/176627.html).
+        >  If the *source or destination database** is an **ApsaraDB database instance** (such as RDS instance and ApsaraDB for MongoDB instance) or a **self-managed database hosted on ECS**, you do not need to add the CIDR blocks. When you click **Set Whitelist and Next** in the DTS console, DTS automatically add the CIDR blocks of DTS servers to the security settings of the source or destination instance.
         
         @param request: DescribeDTSIPRequest
         @return: DescribeDTSIPResponse
         """
         runtime = util_models.RuntimeOptions()
         return self.describe_dtsipwith_options(request, runtime)
 
     async def describe_dtsip_async(
         self,
         request: dts_20200101_models.DescribeDTSIPRequest,
     ) -> dts_20200101_models.DescribeDTSIPResponse:
         """
-        If the *source or destination instance** is an **on-premises database**, you need to call this operation to query the CIDR blocks of DTS servers. Then, you need to add the CIDR blocks of DTS servers to the security settings of the source or destination instance, for example, the firewall of your database. For more information, see [Add the CIDR blocks of DTS servers to the security settings of on-premises databases](~~176627~~).
-        >  If the **source or destination database** is an **ApsaraDB database instance** (such as RDS instance and ApsaraDB for MongoDB instance) or a **self-managed database hosted on ECS**, you do not need to add the CIDR blocks. When you click **Set Whitelist and Next** in the DTS console, DTS automatically add the CIDR blocks of DTS servers to the security settings of the source or destination instance.
+        @description If the *source or destination instance** is an **on-premises database**, you need to call this operation to query the CIDR blocks of DTS servers. Then, you need to add the CIDR blocks of DTS servers to the security settings of the source or destination instance, for example, the firewall of your database. For more information, see [Add the CIDR blocks of DTS servers to the security settings of on-premises databases](https://help.aliyun.com/document_detail/176627.html).
+        >  If the *source or destination database** is an **ApsaraDB database instance** (such as RDS instance and ApsaraDB for MongoDB instance) or a **self-managed database hosted on ECS**, you do not need to add the CIDR blocks. When you click **Set Whitelist and Next** in the DTS console, DTS automatically add the CIDR blocks of DTS servers to the security settings of the source or destination instance.
         
         @param request: DescribeDTSIPRequest
         @return: DescribeDTSIPResponse
         """
         runtime = util_models.RuntimeOptions()
         return await self.describe_dtsipwith_options_async(request, runtime)
 
     def describe_data_check_report_url_with_options(
         self,
         request: dts_20200101_models.DescribeDataCheckReportUrlRequest,
         runtime: util_models.RuntimeOptions,
     ) -> dts_20200101_models.DescribeDataCheckReportUrlResponse:
+        """
+        @summary Queries the download URL of the data consistency verification report.
+        
+        @param request: DescribeDataCheckReportUrlRequest
+        @param runtime: runtime options for this request RuntimeOptions
+        @return: DescribeDataCheckReportUrlResponse
+        """
         UtilClient.validate_model(request)
         query = {}
         if not UtilClient.is_unset(request.check_type):
             query['CheckType'] = request.check_type
         if not UtilClient.is_unset(request.db_name):
             query['DbName'] = request.db_name
         if not UtilClient.is_unset(request.dts_job_id):
@@ -4499,14 +4972,21 @@
         )
 
     async def describe_data_check_report_url_with_options_async(
         self,
         request: dts_20200101_models.DescribeDataCheckReportUrlRequest,
         runtime: util_models.RuntimeOptions,
     ) -> dts_20200101_models.DescribeDataCheckReportUrlResponse:
+        """
+        @summary Queries the download URL of the data consistency verification report.
+        
+        @param request: DescribeDataCheckReportUrlRequest
+        @param runtime: runtime options for this request RuntimeOptions
+        @return: DescribeDataCheckReportUrlResponse
+        """
         UtilClient.validate_model(request)
         query = {}
         if not UtilClient.is_unset(request.check_type):
             query['CheckType'] = request.check_type
         if not UtilClient.is_unset(request.db_name):
             query['DbName'] = request.db_name
         if not UtilClient.is_unset(request.dts_job_id):
@@ -4534,29 +5014,48 @@
             await self.call_api_async(params, req, runtime)
         )
 
     def describe_data_check_report_url(
         self,
         request: dts_20200101_models.DescribeDataCheckReportUrlRequest,
     ) -> dts_20200101_models.DescribeDataCheckReportUrlResponse:
+        """
+        @summary Queries the download URL of the data consistency verification report.
+        
+        @param request: DescribeDataCheckReportUrlRequest
+        @return: DescribeDataCheckReportUrlResponse
+        """
         runtime = util_models.RuntimeOptions()
         return self.describe_data_check_report_url_with_options(request, runtime)
 
     async def describe_data_check_report_url_async(
         self,
         request: dts_20200101_models.DescribeDataCheckReportUrlRequest,
     ) -> dts_20200101_models.DescribeDataCheckReportUrlResponse:
+        """
+        @summary Queries the download URL of the data consistency verification report.
+        
+        @param request: DescribeDataCheckReportUrlRequest
+        @return: DescribeDataCheckReportUrlResponse
+        """
         runtime = util_models.RuntimeOptions()
         return await self.describe_data_check_report_url_with_options_async(request, runtime)
 
     def describe_data_check_table_details_with_options(
         self,
         request: dts_20200101_models.DescribeDataCheckTableDetailsRequest,
         runtime: util_models.RuntimeOptions,
     ) -> dts_20200101_models.DescribeDataCheckTableDetailsResponse:
+        """
+        @summary Queries the details of a data verification task.
+        
+        @param request: DescribeDataCheckTableDetailsRequest
+        @param runtime: runtime options for this request RuntimeOptions
+        @return: DescribeDataCheckTableDetailsResponse
+        """
         UtilClient.validate_model(request)
         query = {}
         if not UtilClient.is_unset(request.check_type):
             query['CheckType'] = request.check_type
         if not UtilClient.is_unset(request.dts_job_id):
             query['DtsJobId'] = request.dts_job_id
         if not UtilClient.is_unset(request.page_number):
@@ -4591,14 +5090,21 @@
         )
 
     async def describe_data_check_table_details_with_options_async(
         self,
         request: dts_20200101_models.DescribeDataCheckTableDetailsRequest,
         runtime: util_models.RuntimeOptions,
     ) -> dts_20200101_models.DescribeDataCheckTableDetailsResponse:
+        """
+        @summary Queries the details of a data verification task.
+        
+        @param request: DescribeDataCheckTableDetailsRequest
+        @param runtime: runtime options for this request RuntimeOptions
+        @return: DescribeDataCheckTableDetailsResponse
+        """
         UtilClient.validate_model(request)
         query = {}
         if not UtilClient.is_unset(request.check_type):
             query['CheckType'] = request.check_type
         if not UtilClient.is_unset(request.dts_job_id):
             query['DtsJobId'] = request.dts_job_id
         if not UtilClient.is_unset(request.page_number):
@@ -4632,29 +5138,46 @@
             await self.call_api_async(params, req, runtime)
         )
 
     def describe_data_check_table_details(
         self,
         request: dts_20200101_models.DescribeDataCheckTableDetailsRequest,
     ) -> dts_20200101_models.DescribeDataCheckTableDetailsResponse:
+        """
+        @summary Queries the details of a data verification task.
+        
+        @param request: DescribeDataCheckTableDetailsRequest
+        @return: DescribeDataCheckTableDetailsResponse
+        """
         runtime = util_models.RuntimeOptions()
         return self.describe_data_check_table_details_with_options(request, runtime)
 
     async def describe_data_check_table_details_async(
         self,
         request: dts_20200101_models.DescribeDataCheckTableDetailsRequest,
     ) -> dts_20200101_models.DescribeDataCheckTableDetailsResponse:
+        """
+        @summary Queries the details of a data verification task.
+        
+        @param request: DescribeDataCheckTableDetailsRequest
+        @return: DescribeDataCheckTableDetailsResponse
+        """
         runtime = util_models.RuntimeOptions()
         return await self.describe_data_check_table_details_with_options_async(request, runtime)
 
     def describe_data_check_table_diff_details_with_options(
         self,
         request: dts_20200101_models.DescribeDataCheckTableDiffDetailsRequest,
         runtime: util_models.RuntimeOptions,
     ) -> dts_20200101_models.DescribeDataCheckTableDiffDetailsResponse:
+        """
+        @param request: DescribeDataCheckTableDiffDetailsRequest
+        @param runtime: runtime options for this request RuntimeOptions
+        @return: DescribeDataCheckTableDiffDetailsResponse
+        """
         UtilClient.validate_model(request)
         query = {}
         if not UtilClient.is_unset(request.check_type):
             query['CheckType'] = request.check_type
         if not UtilClient.is_unset(request.db_name):
             query['DbName'] = request.db_name
         if not UtilClient.is_unset(request.dts_job_id):
@@ -4687,14 +5210,19 @@
         )
 
     async def describe_data_check_table_diff_details_with_options_async(
         self,
         request: dts_20200101_models.DescribeDataCheckTableDiffDetailsRequest,
         runtime: util_models.RuntimeOptions,
     ) -> dts_20200101_models.DescribeDataCheckTableDiffDetailsResponse:
+        """
+        @param request: DescribeDataCheckTableDiffDetailsRequest
+        @param runtime: runtime options for this request RuntimeOptions
+        @return: DescribeDataCheckTableDiffDetailsResponse
+        """
         UtilClient.validate_model(request)
         query = {}
         if not UtilClient.is_unset(request.check_type):
             query['CheckType'] = request.check_type
         if not UtilClient.is_unset(request.db_name):
             query['DbName'] = request.db_name
         if not UtilClient.is_unset(request.dts_job_id):
@@ -4726,29 +5254,44 @@
             await self.call_api_async(params, req, runtime)
         )
 
     def describe_data_check_table_diff_details(
         self,
         request: dts_20200101_models.DescribeDataCheckTableDiffDetailsRequest,
     ) -> dts_20200101_models.DescribeDataCheckTableDiffDetailsResponse:
+        """
+        @param request: DescribeDataCheckTableDiffDetailsRequest
+        @return: DescribeDataCheckTableDiffDetailsResponse
+        """
         runtime = util_models.RuntimeOptions()
         return self.describe_data_check_table_diff_details_with_options(request, runtime)
 
     async def describe_data_check_table_diff_details_async(
         self,
         request: dts_20200101_models.DescribeDataCheckTableDiffDetailsRequest,
     ) -> dts_20200101_models.DescribeDataCheckTableDiffDetailsResponse:
+        """
+        @param request: DescribeDataCheckTableDiffDetailsRequest
+        @return: DescribeDataCheckTableDiffDetailsResponse
+        """
         runtime = util_models.RuntimeOptions()
         return await self.describe_data_check_table_diff_details_with_options_async(request, runtime)
 
     def describe_dedicated_cluster_with_options(
         self,
         request: dts_20200101_models.DescribeDedicatedClusterRequest,
         runtime: util_models.RuntimeOptions,
     ) -> dts_20200101_models.DescribeDedicatedClusterResponse:
+        """
+        @summary Queries the information about a dedicated cluster.
+        
+        @param request: DescribeDedicatedClusterRequest
+        @param runtime: runtime options for this request RuntimeOptions
+        @return: DescribeDedicatedClusterResponse
+        """
         UtilClient.validate_model(request)
         query = {}
         if not UtilClient.is_unset(request.dedicated_cluster_id):
             query['DedicatedClusterId'] = request.dedicated_cluster_id
         if not UtilClient.is_unset(request.owner_id):
             query['OwnerId'] = request.owner_id
         if not UtilClient.is_unset(request.region_id):
@@ -4775,14 +5318,21 @@
         )
 
     async def describe_dedicated_cluster_with_options_async(
         self,
         request: dts_20200101_models.DescribeDedicatedClusterRequest,
         runtime: util_models.RuntimeOptions,
     ) -> dts_20200101_models.DescribeDedicatedClusterResponse:
+        """
+        @summary Queries the information about a dedicated cluster.
+        
+        @param request: DescribeDedicatedClusterRequest
+        @param runtime: runtime options for this request RuntimeOptions
+        @return: DescribeDedicatedClusterResponse
+        """
         UtilClient.validate_model(request)
         query = {}
         if not UtilClient.is_unset(request.dedicated_cluster_id):
             query['DedicatedClusterId'] = request.dedicated_cluster_id
         if not UtilClient.is_unset(request.owner_id):
             query['OwnerId'] = request.owner_id
         if not UtilClient.is_unset(request.region_id):
@@ -4808,29 +5358,48 @@
             await self.call_api_async(params, req, runtime)
         )
 
     def describe_dedicated_cluster(
         self,
         request: dts_20200101_models.DescribeDedicatedClusterRequest,
     ) -> dts_20200101_models.DescribeDedicatedClusterResponse:
+        """
+        @summary Queries the information about a dedicated cluster.
+        
+        @param request: DescribeDedicatedClusterRequest
+        @return: DescribeDedicatedClusterResponse
+        """
         runtime = util_models.RuntimeOptions()
         return self.describe_dedicated_cluster_with_options(request, runtime)
 
     async def describe_dedicated_cluster_async(
         self,
         request: dts_20200101_models.DescribeDedicatedClusterRequest,
     ) -> dts_20200101_models.DescribeDedicatedClusterResponse:
+        """
+        @summary Queries the information about a dedicated cluster.
+        
+        @param request: DescribeDedicatedClusterRequest
+        @return: DescribeDedicatedClusterResponse
+        """
         runtime = util_models.RuntimeOptions()
         return await self.describe_dedicated_cluster_with_options_async(request, runtime)
 
     def describe_dedicated_cluster_monitor_rule_with_options(
         self,
         request: dts_20200101_models.DescribeDedicatedClusterMonitorRuleRequest,
         runtime: util_models.RuntimeOptions,
     ) -> dts_20200101_models.DescribeDedicatedClusterMonitorRuleResponse:
+        """
+        @summary The mobile phone number to which alerts are sent. Separate multiple mobile phone numbers with commas (,).
+        
+        @param request: DescribeDedicatedClusterMonitorRuleRequest
+        @param runtime: runtime options for this request RuntimeOptions
+        @return: DescribeDedicatedClusterMonitorRuleResponse
+        """
         UtilClient.validate_model(request)
         query = {}
         if not UtilClient.is_unset(request.dedicated_cluster_id):
             query['DedicatedClusterId'] = request.dedicated_cluster_id
         if not UtilClient.is_unset(request.owner_id):
             query['OwnerId'] = request.owner_id
         if not UtilClient.is_unset(request.region_id):
@@ -4857,14 +5426,21 @@
         )
 
     async def describe_dedicated_cluster_monitor_rule_with_options_async(
         self,
         request: dts_20200101_models.DescribeDedicatedClusterMonitorRuleRequest,
         runtime: util_models.RuntimeOptions,
     ) -> dts_20200101_models.DescribeDedicatedClusterMonitorRuleResponse:
+        """
+        @summary The mobile phone number to which alerts are sent. Separate multiple mobile phone numbers with commas (,).
+        
+        @param request: DescribeDedicatedClusterMonitorRuleRequest
+        @param runtime: runtime options for this request RuntimeOptions
+        @return: DescribeDedicatedClusterMonitorRuleResponse
+        """
         UtilClient.validate_model(request)
         query = {}
         if not UtilClient.is_unset(request.dedicated_cluster_id):
             query['DedicatedClusterId'] = request.dedicated_cluster_id
         if not UtilClient.is_unset(request.owner_id):
             query['OwnerId'] = request.owner_id
         if not UtilClient.is_unset(request.region_id):
@@ -4890,29 +5466,48 @@
             await self.call_api_async(params, req, runtime)
         )
 
     def describe_dedicated_cluster_monitor_rule(
         self,
         request: dts_20200101_models.DescribeDedicatedClusterMonitorRuleRequest,
     ) -> dts_20200101_models.DescribeDedicatedClusterMonitorRuleResponse:
+        """
+        @summary The mobile phone number to which alerts are sent. Separate multiple mobile phone numbers with commas (,).
+        
+        @param request: DescribeDedicatedClusterMonitorRuleRequest
+        @return: DescribeDedicatedClusterMonitorRuleResponse
+        """
         runtime = util_models.RuntimeOptions()
         return self.describe_dedicated_cluster_monitor_rule_with_options(request, runtime)
 
     async def describe_dedicated_cluster_monitor_rule_async(
         self,
         request: dts_20200101_models.DescribeDedicatedClusterMonitorRuleRequest,
     ) -> dts_20200101_models.DescribeDedicatedClusterMonitorRuleResponse:
+        """
+        @summary The mobile phone number to which alerts are sent. Separate multiple mobile phone numbers with commas (,).
+        
+        @param request: DescribeDedicatedClusterMonitorRuleRequest
+        @return: DescribeDedicatedClusterMonitorRuleResponse
+        """
         runtime = util_models.RuntimeOptions()
         return await self.describe_dedicated_cluster_monitor_rule_with_options_async(request, runtime)
 
     def describe_dts_etl_job_version_info_with_options(
         self,
         request: dts_20200101_models.DescribeDtsEtlJobVersionInfoRequest,
         runtime: util_models.RuntimeOptions,
     ) -> dts_20200101_models.DescribeDtsEtlJobVersionInfoResponse:
+        """
+        @summary 查询ETL任务版本信息
+        
+        @param request: DescribeDtsEtlJobVersionInfoRequest
+        @param runtime: runtime options for this request RuntimeOptions
+        @return: DescribeDtsEtlJobVersionInfoResponse
+        """
         UtilClient.validate_model(request)
         query = {}
         if not UtilClient.is_unset(request.dts_instance_id):
             query['DtsInstanceId'] = request.dts_instance_id
         if not UtilClient.is_unset(request.dts_job_id):
             query['DtsJobId'] = request.dts_job_id
         if not UtilClient.is_unset(request.page_number):
@@ -4943,14 +5538,21 @@
         )
 
     async def describe_dts_etl_job_version_info_with_options_async(
         self,
         request: dts_20200101_models.DescribeDtsEtlJobVersionInfoRequest,
         runtime: util_models.RuntimeOptions,
     ) -> dts_20200101_models.DescribeDtsEtlJobVersionInfoResponse:
+        """
+        @summary 查询ETL任务版本信息
+        
+        @param request: DescribeDtsEtlJobVersionInfoRequest
+        @param runtime: runtime options for this request RuntimeOptions
+        @return: DescribeDtsEtlJobVersionInfoResponse
+        """
         UtilClient.validate_model(request)
         query = {}
         if not UtilClient.is_unset(request.dts_instance_id):
             query['DtsInstanceId'] = request.dts_instance_id
         if not UtilClient.is_unset(request.dts_job_id):
             query['DtsJobId'] = request.dts_job_id
         if not UtilClient.is_unset(request.page_number):
@@ -4980,29 +5582,49 @@
             await self.call_api_async(params, req, runtime)
         )
 
     def describe_dts_etl_job_version_info(
         self,
         request: dts_20200101_models.DescribeDtsEtlJobVersionInfoRequest,
     ) -> dts_20200101_models.DescribeDtsEtlJobVersionInfoResponse:
+        """
+        @summary 查询ETL任务版本信息
+        
+        @param request: DescribeDtsEtlJobVersionInfoRequest
+        @return: DescribeDtsEtlJobVersionInfoResponse
+        """
         runtime = util_models.RuntimeOptions()
         return self.describe_dts_etl_job_version_info_with_options(request, runtime)
 
     async def describe_dts_etl_job_version_info_async(
         self,
         request: dts_20200101_models.DescribeDtsEtlJobVersionInfoRequest,
     ) -> dts_20200101_models.DescribeDtsEtlJobVersionInfoResponse:
+        """
+        @summary 查询ETL任务版本信息
+        
+        @param request: DescribeDtsEtlJobVersionInfoRequest
+        @return: DescribeDtsEtlJobVersionInfoResponse
+        """
         runtime = util_models.RuntimeOptions()
         return await self.describe_dts_etl_job_version_info_with_options_async(request, runtime)
 
     def describe_dts_job_detail_with_options(
         self,
         request: dts_20200101_models.DescribeDtsJobDetailRequest,
         runtime: util_models.RuntimeOptions,
     ) -> dts_20200101_models.DescribeDtsJobDetailResponse:
+        """
+        @summary The latency of incremental data migration or synchronization.
+        >  If you query data migration tasks, the unit of this parameter is milliseconds. If you query data synchronization tasks, the unit of this parameter is seconds.
+        
+        @param request: DescribeDtsJobDetailRequest
+        @param runtime: runtime options for this request RuntimeOptions
+        @return: DescribeDtsJobDetailResponse
+        """
         UtilClient.validate_model(request)
         query = {}
         if not UtilClient.is_unset(request.dts_instance_id):
             query['DtsInstanceID'] = request.dts_instance_id
         if not UtilClient.is_unset(request.dts_job_id):
             query['DtsJobId'] = request.dts_job_id
         if not UtilClient.is_unset(request.region_id):
@@ -5035,14 +5657,22 @@
         )
 
     async def describe_dts_job_detail_with_options_async(
         self,
         request: dts_20200101_models.DescribeDtsJobDetailRequest,
         runtime: util_models.RuntimeOptions,
     ) -> dts_20200101_models.DescribeDtsJobDetailResponse:
+        """
+        @summary The latency of incremental data migration or synchronization.
+        >  If you query data migration tasks, the unit of this parameter is milliseconds. If you query data synchronization tasks, the unit of this parameter is seconds.
+        
+        @param request: DescribeDtsJobDetailRequest
+        @param runtime: runtime options for this request RuntimeOptions
+        @return: DescribeDtsJobDetailResponse
+        """
         UtilClient.validate_model(request)
         query = {}
         if not UtilClient.is_unset(request.dts_instance_id):
             query['DtsInstanceID'] = request.dts_instance_id
         if not UtilClient.is_unset(request.dts_job_id):
             query['DtsJobId'] = request.dts_job_id
         if not UtilClient.is_unset(request.region_id):
@@ -5074,31 +5704,47 @@
             await self.call_api_async(params, req, runtime)
         )
 
     def describe_dts_job_detail(
         self,
         request: dts_20200101_models.DescribeDtsJobDetailRequest,
     ) -> dts_20200101_models.DescribeDtsJobDetailResponse:
+        """
+        @summary The latency of incremental data migration or synchronization.
+        >  If you query data migration tasks, the unit of this parameter is milliseconds. If you query data synchronization tasks, the unit of this parameter is seconds.
+        
+        @param request: DescribeDtsJobDetailRequest
+        @return: DescribeDtsJobDetailResponse
+        """
         runtime = util_models.RuntimeOptions()
         return self.describe_dts_job_detail_with_options(request, runtime)
 
     async def describe_dts_job_detail_async(
         self,
         request: dts_20200101_models.DescribeDtsJobDetailRequest,
     ) -> dts_20200101_models.DescribeDtsJobDetailResponse:
+        """
+        @summary The latency of incremental data migration or synchronization.
+        >  If you query data migration tasks, the unit of this parameter is milliseconds. If you query data synchronization tasks, the unit of this parameter is seconds.
+        
+        @param request: DescribeDtsJobDetailRequest
+        @return: DescribeDtsJobDetailResponse
+        """
         runtime = util_models.RuntimeOptions()
         return await self.describe_dts_job_detail_with_options_async(request, runtime)
 
     def describe_dts_jobs_with_options(
         self,
         request: dts_20200101_models.DescribeDtsJobsRequest,
         runtime: util_models.RuntimeOptions,
     ) -> dts_20200101_models.DescribeDtsJobsResponse:
         """
-        ## Debugging
+        @summary Queries the list of Data Transmission Service (DTS) tasks and the details of each task.
+        
+        @description ## Debugging
         [OpenAPI Explorer automatically calculates the signature value. For your convenience, we recommend that you call this operation in OpenAPI Explorer. OpenAPI Explorer dynamically generates the sample code of the operation for different SDKs.](https://api.aliyun.com/#product=Dts\\&api=DescribeDtsJobs\\&type=RPC\\&version=2020-01-01)
         
         @param request: DescribeDtsJobsRequest
         @param runtime: runtime options for this request RuntimeOptions
         @return: DescribeDtsJobsResponse
         """
         UtilClient.validate_model(request)
@@ -5168,15 +5814,17 @@
 
     async def describe_dts_jobs_with_options_async(
         self,
         request: dts_20200101_models.DescribeDtsJobsRequest,
         runtime: util_models.RuntimeOptions,
     ) -> dts_20200101_models.DescribeDtsJobsResponse:
         """
-        ## Debugging
+        @summary Queries the list of Data Transmission Service (DTS) tasks and the details of each task.
+        
+        @description ## Debugging
         [OpenAPI Explorer automatically calculates the signature value. For your convenience, we recommend that you call this operation in OpenAPI Explorer. OpenAPI Explorer dynamically generates the sample code of the operation for different SDKs.](https://api.aliyun.com/#product=Dts\\&api=DescribeDtsJobs\\&type=RPC\\&version=2020-01-01)
         
         @param request: DescribeDtsJobsRequest
         @param runtime: runtime options for this request RuntimeOptions
         @return: DescribeDtsJobsResponse
         """
         UtilClient.validate_model(request)
@@ -5245,42 +5893,53 @@
         )
 
     def describe_dts_jobs(
         self,
         request: dts_20200101_models.DescribeDtsJobsRequest,
     ) -> dts_20200101_models.DescribeDtsJobsResponse:
         """
-        ## Debugging
+        @summary Queries the list of Data Transmission Service (DTS) tasks and the details of each task.
+        
+        @description ## Debugging
         [OpenAPI Explorer automatically calculates the signature value. For your convenience, we recommend that you call this operation in OpenAPI Explorer. OpenAPI Explorer dynamically generates the sample code of the operation for different SDKs.](https://api.aliyun.com/#product=Dts\\&api=DescribeDtsJobs\\&type=RPC\\&version=2020-01-01)
         
         @param request: DescribeDtsJobsRequest
         @return: DescribeDtsJobsResponse
         """
         runtime = util_models.RuntimeOptions()
         return self.describe_dts_jobs_with_options(request, runtime)
 
     async def describe_dts_jobs_async(
         self,
         request: dts_20200101_models.DescribeDtsJobsRequest,
     ) -> dts_20200101_models.DescribeDtsJobsResponse:
         """
-        ## Debugging
+        @summary Queries the list of Data Transmission Service (DTS) tasks and the details of each task.
+        
+        @description ## Debugging
         [OpenAPI Explorer automatically calculates the signature value. For your convenience, we recommend that you call this operation in OpenAPI Explorer. OpenAPI Explorer dynamically generates the sample code of the operation for different SDKs.](https://api.aliyun.com/#product=Dts\\&api=DescribeDtsJobs\\&type=RPC\\&version=2020-01-01)
         
         @param request: DescribeDtsJobsRequest
         @return: DescribeDtsJobsResponse
         """
         runtime = util_models.RuntimeOptions()
         return await self.describe_dts_jobs_with_options_async(request, runtime)
 
     def describe_dts_service_log_with_options(
         self,
         request: dts_20200101_models.DescribeDtsServiceLogRequest,
         runtime: util_models.RuntimeOptions,
     ) -> dts_20200101_models.DescribeDtsServiceLogResponse:
+        """
+        @summary Queries the logs of a data migration or synchronization task.
+        
+        @param request: DescribeDtsServiceLogRequest
+        @param runtime: runtime options for this request RuntimeOptions
+        @return: DescribeDtsServiceLogResponse
+        """
         UtilClient.validate_model(request)
         query = {}
         if not UtilClient.is_unset(request.dts_job_id):
             query['DtsJobId'] = request.dts_job_id
         if not UtilClient.is_unset(request.end_time):
             query['EndTime'] = request.end_time
         if not UtilClient.is_unset(request.keyword):
@@ -5321,14 +5980,21 @@
         )
 
     async def describe_dts_service_log_with_options_async(
         self,
         request: dts_20200101_models.DescribeDtsServiceLogRequest,
         runtime: util_models.RuntimeOptions,
     ) -> dts_20200101_models.DescribeDtsServiceLogResponse:
+        """
+        @summary Queries the logs of a data migration or synchronization task.
+        
+        @param request: DescribeDtsServiceLogRequest
+        @param runtime: runtime options for this request RuntimeOptions
+        @return: DescribeDtsServiceLogResponse
+        """
         UtilClient.validate_model(request)
         query = {}
         if not UtilClient.is_unset(request.dts_job_id):
             query['DtsJobId'] = request.dts_job_id
         if not UtilClient.is_unset(request.end_time):
             query['EndTime'] = request.end_time
         if not UtilClient.is_unset(request.keyword):
@@ -5368,31 +6034,43 @@
             await self.call_api_async(params, req, runtime)
         )
 
     def describe_dts_service_log(
         self,
         request: dts_20200101_models.DescribeDtsServiceLogRequest,
     ) -> dts_20200101_models.DescribeDtsServiceLogResponse:
+        """
+        @summary Queries the logs of a data migration or synchronization task.
+        
+        @param request: DescribeDtsServiceLogRequest
+        @return: DescribeDtsServiceLogResponse
+        """
         runtime = util_models.RuntimeOptions()
         return self.describe_dts_service_log_with_options(request, runtime)
 
     async def describe_dts_service_log_async(
         self,
         request: dts_20200101_models.DescribeDtsServiceLogRequest,
     ) -> dts_20200101_models.DescribeDtsServiceLogResponse:
+        """
+        @summary Queries the logs of a data migration or synchronization task.
+        
+        @param request: DescribeDtsServiceLogRequest
+        @return: DescribeDtsServiceLogResponse
+        """
         runtime = util_models.RuntimeOptions()
         return await self.describe_dts_service_log_with_options_async(request, runtime)
 
     def describe_endpoint_switch_status_with_options(
         self,
         request: dts_20200101_models.DescribeEndpointSwitchStatusRequest,
         runtime: util_models.RuntimeOptions,
     ) -> dts_20200101_models.DescribeEndpointSwitchStatusResponse:
         """
-        Before you call this operation, you must call the [SwitchSynchronizationEndpoint](~~201858~~) operation to change the database connection settings.
+        @description Before you call this operation, you must call the [SwitchSynchronizationEndpoint](https://help.aliyun.com/document_detail/201858.html) operation to change the database connection settings.
         
         @param request: DescribeEndpointSwitchStatusRequest
         @param runtime: runtime options for this request RuntimeOptions
         @return: DescribeEndpointSwitchStatusResponse
         """
         UtilClient.validate_model(request)
         query = {}
@@ -5429,15 +6107,15 @@
 
     async def describe_endpoint_switch_status_with_options_async(
         self,
         request: dts_20200101_models.DescribeEndpointSwitchStatusRequest,
         runtime: util_models.RuntimeOptions,
     ) -> dts_20200101_models.DescribeEndpointSwitchStatusResponse:
         """
-        Before you call this operation, you must call the [SwitchSynchronizationEndpoint](~~201858~~) operation to change the database connection settings.
+        @description Before you call this operation, you must call the [SwitchSynchronizationEndpoint](https://help.aliyun.com/document_detail/201858.html) operation to change the database connection settings.
         
         @param request: DescribeEndpointSwitchStatusRequest
         @param runtime: runtime options for this request RuntimeOptions
         @return: DescribeEndpointSwitchStatusResponse
         """
         UtilClient.validate_model(request)
         query = {}
@@ -5473,40 +6151,45 @@
         )
 
     def describe_endpoint_switch_status(
         self,
         request: dts_20200101_models.DescribeEndpointSwitchStatusRequest,
     ) -> dts_20200101_models.DescribeEndpointSwitchStatusResponse:
         """
-        Before you call this operation, you must call the [SwitchSynchronizationEndpoint](~~201858~~) operation to change the database connection settings.
+        @description Before you call this operation, you must call the [SwitchSynchronizationEndpoint](https://help.aliyun.com/document_detail/201858.html) operation to change the database connection settings.
         
         @param request: DescribeEndpointSwitchStatusRequest
         @return: DescribeEndpointSwitchStatusResponse
         """
         runtime = util_models.RuntimeOptions()
         return self.describe_endpoint_switch_status_with_options(request, runtime)
 
     async def describe_endpoint_switch_status_async(
         self,
         request: dts_20200101_models.DescribeEndpointSwitchStatusRequest,
     ) -> dts_20200101_models.DescribeEndpointSwitchStatusResponse:
         """
-        Before you call this operation, you must call the [SwitchSynchronizationEndpoint](~~201858~~) operation to change the database connection settings.
+        @description Before you call this operation, you must call the [SwitchSynchronizationEndpoint](https://help.aliyun.com/document_detail/201858.html) operation to change the database connection settings.
         
         @param request: DescribeEndpointSwitchStatusRequest
         @return: DescribeEndpointSwitchStatusResponse
         """
         runtime = util_models.RuntimeOptions()
         return await self.describe_endpoint_switch_status_with_options_async(request, runtime)
 
     def describe_etl_job_logs_with_options(
         self,
         request: dts_20200101_models.DescribeEtlJobLogsRequest,
         runtime: util_models.RuntimeOptions,
     ) -> dts_20200101_models.DescribeEtlJobLogsResponse:
+        """
+        @param request: DescribeEtlJobLogsRequest
+        @param runtime: runtime options for this request RuntimeOptions
+        @return: DescribeEtlJobLogsResponse
+        """
         UtilClient.validate_model(request)
         query = {}
         if not UtilClient.is_unset(request.dts_job_id):
             query['DtsJobId'] = request.dts_job_id
         if not UtilClient.is_unset(request.region_id):
             query['RegionId'] = request.region_id
         if not UtilClient.is_unset(request.resource_group_id):
@@ -5531,14 +6214,19 @@
         )
 
     async def describe_etl_job_logs_with_options_async(
         self,
         request: dts_20200101_models.DescribeEtlJobLogsRequest,
         runtime: util_models.RuntimeOptions,
     ) -> dts_20200101_models.DescribeEtlJobLogsResponse:
+        """
+        @param request: DescribeEtlJobLogsRequest
+        @param runtime: runtime options for this request RuntimeOptions
+        @return: DescribeEtlJobLogsResponse
+        """
         UtilClient.validate_model(request)
         query = {}
         if not UtilClient.is_unset(request.dts_job_id):
             query['DtsJobId'] = request.dts_job_id
         if not UtilClient.is_unset(request.region_id):
             query['RegionId'] = request.region_id
         if not UtilClient.is_unset(request.resource_group_id):
@@ -5562,29 +6250,42 @@
             await self.call_api_async(params, req, runtime)
         )
 
     def describe_etl_job_logs(
         self,
         request: dts_20200101_models.DescribeEtlJobLogsRequest,
     ) -> dts_20200101_models.DescribeEtlJobLogsResponse:
+        """
+        @param request: DescribeEtlJobLogsRequest
+        @return: DescribeEtlJobLogsResponse
+        """
         runtime = util_models.RuntimeOptions()
         return self.describe_etl_job_logs_with_options(request, runtime)
 
     async def describe_etl_job_logs_async(
         self,
         request: dts_20200101_models.DescribeEtlJobLogsRequest,
     ) -> dts_20200101_models.DescribeEtlJobLogsResponse:
+        """
+        @param request: DescribeEtlJobLogsRequest
+        @return: DescribeEtlJobLogsResponse
+        """
         runtime = util_models.RuntimeOptions()
         return await self.describe_etl_job_logs_with_options_async(request, runtime)
 
     def describe_initialization_status_with_options(
         self,
         request: dts_20200101_models.DescribeInitializationStatusRequest,
         runtime: util_models.RuntimeOptions,
     ) -> dts_20200101_models.DescribeInitializationStatusResponse:
+        """
+        @param request: DescribeInitializationStatusRequest
+        @param runtime: runtime options for this request RuntimeOptions
+        @return: DescribeInitializationStatusResponse
+        """
         UtilClient.validate_model(request)
         query = {}
         if not UtilClient.is_unset(request.account_id):
             query['AccountId'] = request.account_id
         if not UtilClient.is_unset(request.owner_id):
             query['OwnerId'] = request.owner_id
         if not UtilClient.is_unset(request.page_num):
@@ -5617,14 +6318,19 @@
         )
 
     async def describe_initialization_status_with_options_async(
         self,
         request: dts_20200101_models.DescribeInitializationStatusRequest,
         runtime: util_models.RuntimeOptions,
     ) -> dts_20200101_models.DescribeInitializationStatusResponse:
+        """
+        @param request: DescribeInitializationStatusRequest
+        @param runtime: runtime options for this request RuntimeOptions
+        @return: DescribeInitializationStatusResponse
+        """
         UtilClient.validate_model(request)
         query = {}
         if not UtilClient.is_unset(request.account_id):
             query['AccountId'] = request.account_id
         if not UtilClient.is_unset(request.owner_id):
             query['OwnerId'] = request.owner_id
         if not UtilClient.is_unset(request.page_num):
@@ -5656,29 +6362,42 @@
             await self.call_api_async(params, req, runtime)
         )
 
     def describe_initialization_status(
         self,
         request: dts_20200101_models.DescribeInitializationStatusRequest,
     ) -> dts_20200101_models.DescribeInitializationStatusResponse:
+        """
+        @param request: DescribeInitializationStatusRequest
+        @return: DescribeInitializationStatusResponse
+        """
         runtime = util_models.RuntimeOptions()
         return self.describe_initialization_status_with_options(request, runtime)
 
     async def describe_initialization_status_async(
         self,
         request: dts_20200101_models.DescribeInitializationStatusRequest,
     ) -> dts_20200101_models.DescribeInitializationStatusResponse:
+        """
+        @param request: DescribeInitializationStatusRequest
+        @return: DescribeInitializationStatusResponse
+        """
         runtime = util_models.RuntimeOptions()
         return await self.describe_initialization_status_with_options_async(request, runtime)
 
     def describe_job_monitor_rule_with_options(
         self,
         request: dts_20200101_models.DescribeJobMonitorRuleRequest,
         runtime: util_models.RuntimeOptions,
     ) -> dts_20200101_models.DescribeJobMonitorRuleResponse:
+        """
+        @param request: DescribeJobMonitorRuleRequest
+        @param runtime: runtime options for this request RuntimeOptions
+        @return: DescribeJobMonitorRuleResponse
+        """
         UtilClient.validate_model(request)
         query = {}
         if not UtilClient.is_unset(request.dts_job_id):
             query['DtsJobId'] = request.dts_job_id
         if not UtilClient.is_unset(request.region_id):
             query['RegionId'] = request.region_id
         if not UtilClient.is_unset(request.resource_group_id):
@@ -5703,14 +6422,19 @@
         )
 
     async def describe_job_monitor_rule_with_options_async(
         self,
         request: dts_20200101_models.DescribeJobMonitorRuleRequest,
         runtime: util_models.RuntimeOptions,
     ) -> dts_20200101_models.DescribeJobMonitorRuleResponse:
+        """
+        @param request: DescribeJobMonitorRuleRequest
+        @param runtime: runtime options for this request RuntimeOptions
+        @return: DescribeJobMonitorRuleResponse
+        """
         UtilClient.validate_model(request)
         query = {}
         if not UtilClient.is_unset(request.dts_job_id):
             query['DtsJobId'] = request.dts_job_id
         if not UtilClient.is_unset(request.region_id):
             query['RegionId'] = request.region_id
         if not UtilClient.is_unset(request.resource_group_id):
@@ -5734,29 +6458,44 @@
             await self.call_api_async(params, req, runtime)
         )
 
     def describe_job_monitor_rule(
         self,
         request: dts_20200101_models.DescribeJobMonitorRuleRequest,
     ) -> dts_20200101_models.DescribeJobMonitorRuleResponse:
+        """
+        @param request: DescribeJobMonitorRuleRequest
+        @return: DescribeJobMonitorRuleResponse
+        """
         runtime = util_models.RuntimeOptions()
         return self.describe_job_monitor_rule_with_options(request, runtime)
 
     async def describe_job_monitor_rule_async(
         self,
         request: dts_20200101_models.DescribeJobMonitorRuleRequest,
     ) -> dts_20200101_models.DescribeJobMonitorRuleResponse:
+        """
+        @param request: DescribeJobMonitorRuleRequest
+        @return: DescribeJobMonitorRuleResponse
+        """
         runtime = util_models.RuntimeOptions()
         return await self.describe_job_monitor_rule_with_options_async(request, runtime)
 
     def describe_metric_list_with_options(
         self,
         request: dts_20200101_models.DescribeMetricListRequest,
         runtime: util_models.RuntimeOptions,
     ) -> dts_20200101_models.DescribeMetricListResponse:
+        """
+        @summary Queries the metrics of a cluster.
+        
+        @param request: DescribeMetricListRequest
+        @param runtime: runtime options for this request RuntimeOptions
+        @return: DescribeMetricListResponse
+        """
         UtilClient.validate_model(request)
         query = {}
         if not UtilClient.is_unset(request.resource_group_id):
             query['ResourceGroupId'] = request.resource_group_id
         body = {}
         if not UtilClient.is_unset(request.account_id):
             body['AccountId'] = request.account_id
@@ -5801,14 +6540,21 @@
         )
 
     async def describe_metric_list_with_options_async(
         self,
         request: dts_20200101_models.DescribeMetricListRequest,
         runtime: util_models.RuntimeOptions,
     ) -> dts_20200101_models.DescribeMetricListResponse:
+        """
+        @summary Queries the metrics of a cluster.
+        
+        @param request: DescribeMetricListRequest
+        @param runtime: runtime options for this request RuntimeOptions
+        @return: DescribeMetricListResponse
+        """
         UtilClient.validate_model(request)
         query = {}
         if not UtilClient.is_unset(request.resource_group_id):
             query['ResourceGroupId'] = request.resource_group_id
         body = {}
         if not UtilClient.is_unset(request.account_id):
             body['AccountId'] = request.account_id
@@ -5852,29 +6598,46 @@
             await self.call_api_async(params, req, runtime)
         )
 
     def describe_metric_list(
         self,
         request: dts_20200101_models.DescribeMetricListRequest,
     ) -> dts_20200101_models.DescribeMetricListResponse:
+        """
+        @summary Queries the metrics of a cluster.
+        
+        @param request: DescribeMetricListRequest
+        @return: DescribeMetricListResponse
+        """
         runtime = util_models.RuntimeOptions()
         return self.describe_metric_list_with_options(request, runtime)
 
     async def describe_metric_list_async(
         self,
         request: dts_20200101_models.DescribeMetricListRequest,
     ) -> dts_20200101_models.DescribeMetricListResponse:
+        """
+        @summary Queries the metrics of a cluster.
+        
+        @param request: DescribeMetricListRequest
+        @return: DescribeMetricListResponse
+        """
         runtime = util_models.RuntimeOptions()
         return await self.describe_metric_list_with_options_async(request, runtime)
 
     def describe_migration_job_alert_with_options(
         self,
         request: dts_20200101_models.DescribeMigrationJobAlertRequest,
         runtime: util_models.RuntimeOptions,
     ) -> dts_20200101_models.DescribeMigrationJobAlertResponse:
+        """
+        @param request: DescribeMigrationJobAlertRequest
+        @param runtime: runtime options for this request RuntimeOptions
+        @return: DescribeMigrationJobAlertResponse
+        """
         UtilClient.validate_model(request)
         query = {}
         if not UtilClient.is_unset(request.account_id):
             query['AccountId'] = request.account_id
         if not UtilClient.is_unset(request.client_token):
             query['ClientToken'] = request.client_token
         if not UtilClient.is_unset(request.migration_job_id):
@@ -5905,14 +6668,19 @@
         )
 
     async def describe_migration_job_alert_with_options_async(
         self,
         request: dts_20200101_models.DescribeMigrationJobAlertRequest,
         runtime: util_models.RuntimeOptions,
     ) -> dts_20200101_models.DescribeMigrationJobAlertResponse:
+        """
+        @param request: DescribeMigrationJobAlertRequest
+        @param runtime: runtime options for this request RuntimeOptions
+        @return: DescribeMigrationJobAlertResponse
+        """
         UtilClient.validate_model(request)
         query = {}
         if not UtilClient.is_unset(request.account_id):
             query['AccountId'] = request.account_id
         if not UtilClient.is_unset(request.client_token):
             query['ClientToken'] = request.client_token
         if not UtilClient.is_unset(request.migration_job_id):
@@ -5942,31 +6710,41 @@
             await self.call_api_async(params, req, runtime)
         )
 
     def describe_migration_job_alert(
         self,
         request: dts_20200101_models.DescribeMigrationJobAlertRequest,
     ) -> dts_20200101_models.DescribeMigrationJobAlertResponse:
+        """
+        @param request: DescribeMigrationJobAlertRequest
+        @return: DescribeMigrationJobAlertResponse
+        """
         runtime = util_models.RuntimeOptions()
         return self.describe_migration_job_alert_with_options(request, runtime)
 
     async def describe_migration_job_alert_async(
         self,
         request: dts_20200101_models.DescribeMigrationJobAlertRequest,
     ) -> dts_20200101_models.DescribeMigrationJobAlertResponse:
+        """
+        @param request: DescribeMigrationJobAlertRequest
+        @return: DescribeMigrationJobAlertResponse
+        """
         runtime = util_models.RuntimeOptions()
         return await self.describe_migration_job_alert_with_options_async(request, runtime)
 
     def describe_migration_job_detail_with_options(
         self,
         request: dts_20200101_models.DescribeMigrationJobDetailRequest,
         runtime: util_models.RuntimeOptions,
     ) -> dts_20200101_models.DescribeMigrationJobDetailResponse:
         """
-        When you call this operation, the data migration task must be in the Migrating, Failed, Paused, or Finished state.
+        @summary Queries the details of a data migration task.
+        
+        @description When you call this operation, the data migration task must be in the Migrating, Failed, Paused, or Finished state.
         
         @param request: DescribeMigrationJobDetailRequest
         @param runtime: runtime options for this request RuntimeOptions
         @return: DescribeMigrationJobDetailResponse
         """
         UtilClient.validate_model(request)
         query = {}
@@ -6009,15 +6787,17 @@
 
     async def describe_migration_job_detail_with_options_async(
         self,
         request: dts_20200101_models.DescribeMigrationJobDetailRequest,
         runtime: util_models.RuntimeOptions,
     ) -> dts_20200101_models.DescribeMigrationJobDetailResponse:
         """
-        When you call this operation, the data migration task must be in the Migrating, Failed, Paused, or Finished state.
+        @summary Queries the details of a data migration task.
+        
+        @description When you call this operation, the data migration task must be in the Migrating, Failed, Paused, or Finished state.
         
         @param request: DescribeMigrationJobDetailRequest
         @param runtime: runtime options for this request RuntimeOptions
         @return: DescribeMigrationJobDetailResponse
         """
         UtilClient.validate_model(request)
         query = {}
@@ -6059,40 +6839,51 @@
         )
 
     def describe_migration_job_detail(
         self,
         request: dts_20200101_models.DescribeMigrationJobDetailRequest,
     ) -> dts_20200101_models.DescribeMigrationJobDetailResponse:
         """
-        When you call this operation, the data migration task must be in the Migrating, Failed, Paused, or Finished state.
+        @summary Queries the details of a data migration task.
+        
+        @description When you call this operation, the data migration task must be in the Migrating, Failed, Paused, or Finished state.
         
         @param request: DescribeMigrationJobDetailRequest
         @return: DescribeMigrationJobDetailResponse
         """
         runtime = util_models.RuntimeOptions()
         return self.describe_migration_job_detail_with_options(request, runtime)
 
     async def describe_migration_job_detail_async(
         self,
         request: dts_20200101_models.DescribeMigrationJobDetailRequest,
     ) -> dts_20200101_models.DescribeMigrationJobDetailResponse:
         """
-        When you call this operation, the data migration task must be in the Migrating, Failed, Paused, or Finished state.
+        @summary Queries the details of a data migration task.
+        
+        @description When you call this operation, the data migration task must be in the Migrating, Failed, Paused, or Finished state.
         
         @param request: DescribeMigrationJobDetailRequest
         @return: DescribeMigrationJobDetailResponse
         """
         runtime = util_models.RuntimeOptions()
         return await self.describe_migration_job_detail_with_options_async(request, runtime)
 
     def describe_migration_job_status_with_options(
         self,
         request: dts_20200101_models.DescribeMigrationJobStatusRequest,
         runtime: util_models.RuntimeOptions,
     ) -> dts_20200101_models.DescribeMigrationJobStatusResponse:
+        """
+        @summary Queries the status of a data migration task.
+        
+        @param request: DescribeMigrationJobStatusRequest
+        @param runtime: runtime options for this request RuntimeOptions
+        @return: DescribeMigrationJobStatusResponse
+        """
         UtilClient.validate_model(request)
         query = {}
         if not UtilClient.is_unset(request.account_id):
             query['AccountId'] = request.account_id
         if not UtilClient.is_unset(request.client_token):
             query['ClientToken'] = request.client_token
         if not UtilClient.is_unset(request.migration_job_id):
@@ -6123,14 +6914,21 @@
         )
 
     async def describe_migration_job_status_with_options_async(
         self,
         request: dts_20200101_models.DescribeMigrationJobStatusRequest,
         runtime: util_models.RuntimeOptions,
     ) -> dts_20200101_models.DescribeMigrationJobStatusResponse:
+        """
+        @summary Queries the status of a data migration task.
+        
+        @param request: DescribeMigrationJobStatusRequest
+        @param runtime: runtime options for this request RuntimeOptions
+        @return: DescribeMigrationJobStatusResponse
+        """
         UtilClient.validate_model(request)
         query = {}
         if not UtilClient.is_unset(request.account_id):
             query['AccountId'] = request.account_id
         if not UtilClient.is_unset(request.client_token):
             query['ClientToken'] = request.client_token
         if not UtilClient.is_unset(request.migration_job_id):
@@ -6160,29 +6958,48 @@
             await self.call_api_async(params, req, runtime)
         )
 
     def describe_migration_job_status(
         self,
         request: dts_20200101_models.DescribeMigrationJobStatusRequest,
     ) -> dts_20200101_models.DescribeMigrationJobStatusResponse:
+        """
+        @summary Queries the status of a data migration task.
+        
+        @param request: DescribeMigrationJobStatusRequest
+        @return: DescribeMigrationJobStatusResponse
+        """
         runtime = util_models.RuntimeOptions()
         return self.describe_migration_job_status_with_options(request, runtime)
 
     async def describe_migration_job_status_async(
         self,
         request: dts_20200101_models.DescribeMigrationJobStatusRequest,
     ) -> dts_20200101_models.DescribeMigrationJobStatusResponse:
+        """
+        @summary Queries the status of a data migration task.
+        
+        @param request: DescribeMigrationJobStatusRequest
+        @return: DescribeMigrationJobStatusResponse
+        """
         runtime = util_models.RuntimeOptions()
         return await self.describe_migration_job_status_with_options_async(request, runtime)
 
     def describe_migration_jobs_with_options(
         self,
         request: dts_20200101_models.DescribeMigrationJobsRequest,
         runtime: util_models.RuntimeOptions,
     ) -> dts_20200101_models.DescribeMigrationJobsResponse:
+        """
+        @summary Queries the list of data migration instances and the details of each instance.
+        
+        @param request: DescribeMigrationJobsRequest
+        @param runtime: runtime options for this request RuntimeOptions
+        @return: DescribeMigrationJobsResponse
+        """
         UtilClient.validate_model(request)
         query = {}
         if not UtilClient.is_unset(request.account_id):
             query['AccountId'] = request.account_id
         if not UtilClient.is_unset(request.migration_job_name):
             query['MigrationJobName'] = request.migration_job_name
         if not UtilClient.is_unset(request.owner_id):
@@ -6217,14 +7034,21 @@
         )
 
     async def describe_migration_jobs_with_options_async(
         self,
         request: dts_20200101_models.DescribeMigrationJobsRequest,
         runtime: util_models.RuntimeOptions,
     ) -> dts_20200101_models.DescribeMigrationJobsResponse:
+        """
+        @summary Queries the list of data migration instances and the details of each instance.
+        
+        @param request: DescribeMigrationJobsRequest
+        @param runtime: runtime options for this request RuntimeOptions
+        @return: DescribeMigrationJobsResponse
+        """
         UtilClient.validate_model(request)
         query = {}
         if not UtilClient.is_unset(request.account_id):
             query['AccountId'] = request.account_id
         if not UtilClient.is_unset(request.migration_job_name):
             query['MigrationJobName'] = request.migration_job_name
         if not UtilClient.is_unset(request.owner_id):
@@ -6258,29 +7082,46 @@
             await self.call_api_async(params, req, runtime)
         )
 
     def describe_migration_jobs(
         self,
         request: dts_20200101_models.DescribeMigrationJobsRequest,
     ) -> dts_20200101_models.DescribeMigrationJobsResponse:
+        """
+        @summary Queries the list of data migration instances and the details of each instance.
+        
+        @param request: DescribeMigrationJobsRequest
+        @return: DescribeMigrationJobsResponse
+        """
         runtime = util_models.RuntimeOptions()
         return self.describe_migration_jobs_with_options(request, runtime)
 
     async def describe_migration_jobs_async(
         self,
         request: dts_20200101_models.DescribeMigrationJobsRequest,
     ) -> dts_20200101_models.DescribeMigrationJobsResponse:
+        """
+        @summary Queries the list of data migration instances and the details of each instance.
+        
+        @param request: DescribeMigrationJobsRequest
+        @return: DescribeMigrationJobsResponse
+        """
         runtime = util_models.RuntimeOptions()
         return await self.describe_migration_jobs_with_options_async(request, runtime)
 
     def describe_pre_check_status_with_options(
         self,
         request: dts_20200101_models.DescribePreCheckStatusRequest,
         runtime: util_models.RuntimeOptions,
     ) -> dts_20200101_models.DescribePreCheckStatusResponse:
+        """
+        @param request: DescribePreCheckStatusRequest
+        @param runtime: runtime options for this request RuntimeOptions
+        @return: DescribePreCheckStatusResponse
+        """
         UtilClient.validate_model(request)
         query = {}
         if not UtilClient.is_unset(request.dts_job_id):
             query['DtsJobId'] = request.dts_job_id
         if not UtilClient.is_unset(request.job_code):
             query['JobCode'] = request.job_code
         if not UtilClient.is_unset(request.name):
@@ -6319,14 +7160,19 @@
         )
 
     async def describe_pre_check_status_with_options_async(
         self,
         request: dts_20200101_models.DescribePreCheckStatusRequest,
         runtime: util_models.RuntimeOptions,
     ) -> dts_20200101_models.DescribePreCheckStatusResponse:
+        """
+        @param request: DescribePreCheckStatusRequest
+        @param runtime: runtime options for this request RuntimeOptions
+        @return: DescribePreCheckStatusResponse
+        """
         UtilClient.validate_model(request)
         query = {}
         if not UtilClient.is_unset(request.dts_job_id):
             query['DtsJobId'] = request.dts_job_id
         if not UtilClient.is_unset(request.job_code):
             query['JobCode'] = request.job_code
         if not UtilClient.is_unset(request.name):
@@ -6364,29 +7210,42 @@
             await self.call_api_async(params, req, runtime)
         )
 
     def describe_pre_check_status(
         self,
         request: dts_20200101_models.DescribePreCheckStatusRequest,
     ) -> dts_20200101_models.DescribePreCheckStatusResponse:
+        """
+        @param request: DescribePreCheckStatusRequest
+        @return: DescribePreCheckStatusResponse
+        """
         runtime = util_models.RuntimeOptions()
         return self.describe_pre_check_status_with_options(request, runtime)
 
     async def describe_pre_check_status_async(
         self,
         request: dts_20200101_models.DescribePreCheckStatusRequest,
     ) -> dts_20200101_models.DescribePreCheckStatusResponse:
+        """
+        @param request: DescribePreCheckStatusRequest
+        @return: DescribePreCheckStatusResponse
+        """
         runtime = util_models.RuntimeOptions()
         return await self.describe_pre_check_status_with_options_async(request, runtime)
 
     def describe_subscription_instance_alert_with_options(
         self,
         request: dts_20200101_models.DescribeSubscriptionInstanceAlertRequest,
         runtime: util_models.RuntimeOptions,
     ) -> dts_20200101_models.DescribeSubscriptionInstanceAlertResponse:
+        """
+        @param request: DescribeSubscriptionInstanceAlertRequest
+        @param runtime: runtime options for this request RuntimeOptions
+        @return: DescribeSubscriptionInstanceAlertResponse
+        """
         UtilClient.validate_model(request)
         query = {}
         if not UtilClient.is_unset(request.account_id):
             query['AccountId'] = request.account_id
         if not UtilClient.is_unset(request.client_token):
             query['ClientToken'] = request.client_token
         if not UtilClient.is_unset(request.owner_id):
@@ -6417,14 +7276,19 @@
         )
 
     async def describe_subscription_instance_alert_with_options_async(
         self,
         request: dts_20200101_models.DescribeSubscriptionInstanceAlertRequest,
         runtime: util_models.RuntimeOptions,
     ) -> dts_20200101_models.DescribeSubscriptionInstanceAlertResponse:
+        """
+        @param request: DescribeSubscriptionInstanceAlertRequest
+        @param runtime: runtime options for this request RuntimeOptions
+        @return: DescribeSubscriptionInstanceAlertResponse
+        """
         UtilClient.validate_model(request)
         query = {}
         if not UtilClient.is_unset(request.account_id):
             query['AccountId'] = request.account_id
         if not UtilClient.is_unset(request.client_token):
             query['ClientToken'] = request.client_token
         if not UtilClient.is_unset(request.owner_id):
@@ -6454,29 +7318,44 @@
             await self.call_api_async(params, req, runtime)
         )
 
     def describe_subscription_instance_alert(
         self,
         request: dts_20200101_models.DescribeSubscriptionInstanceAlertRequest,
     ) -> dts_20200101_models.DescribeSubscriptionInstanceAlertResponse:
+        """
+        @param request: DescribeSubscriptionInstanceAlertRequest
+        @return: DescribeSubscriptionInstanceAlertResponse
+        """
         runtime = util_models.RuntimeOptions()
         return self.describe_subscription_instance_alert_with_options(request, runtime)
 
     async def describe_subscription_instance_alert_async(
         self,
         request: dts_20200101_models.DescribeSubscriptionInstanceAlertRequest,
     ) -> dts_20200101_models.DescribeSubscriptionInstanceAlertResponse:
+        """
+        @param request: DescribeSubscriptionInstanceAlertRequest
+        @return: DescribeSubscriptionInstanceAlertResponse
+        """
         runtime = util_models.RuntimeOptions()
         return await self.describe_subscription_instance_alert_with_options_async(request, runtime)
 
     def describe_subscription_instance_status_with_options(
         self,
         request: dts_20200101_models.DescribeSubscriptionInstanceStatusRequest,
         runtime: util_models.RuntimeOptions,
     ) -> dts_20200101_models.DescribeSubscriptionInstanceStatusResponse:
+        """
+        @summary Queries the status of a change tracking instance.
+        
+        @param request: DescribeSubscriptionInstanceStatusRequest
+        @param runtime: runtime options for this request RuntimeOptions
+        @return: DescribeSubscriptionInstanceStatusResponse
+        """
         UtilClient.validate_model(request)
         query = {}
         if not UtilClient.is_unset(request.account_id):
             query['AccountId'] = request.account_id
         if not UtilClient.is_unset(request.owner_id):
             query['OwnerId'] = request.owner_id
         if not UtilClient.is_unset(request.region_id):
@@ -6505,14 +7384,21 @@
         )
 
     async def describe_subscription_instance_status_with_options_async(
         self,
         request: dts_20200101_models.DescribeSubscriptionInstanceStatusRequest,
         runtime: util_models.RuntimeOptions,
     ) -> dts_20200101_models.DescribeSubscriptionInstanceStatusResponse:
+        """
+        @summary Queries the status of a change tracking instance.
+        
+        @param request: DescribeSubscriptionInstanceStatusRequest
+        @param runtime: runtime options for this request RuntimeOptions
+        @return: DescribeSubscriptionInstanceStatusResponse
+        """
         UtilClient.validate_model(request)
         query = {}
         if not UtilClient.is_unset(request.account_id):
             query['AccountId'] = request.account_id
         if not UtilClient.is_unset(request.owner_id):
             query['OwnerId'] = request.owner_id
         if not UtilClient.is_unset(request.region_id):
@@ -6540,29 +7426,48 @@
             await self.call_api_async(params, req, runtime)
         )
 
     def describe_subscription_instance_status(
         self,
         request: dts_20200101_models.DescribeSubscriptionInstanceStatusRequest,
     ) -> dts_20200101_models.DescribeSubscriptionInstanceStatusResponse:
+        """
+        @summary Queries the status of a change tracking instance.
+        
+        @param request: DescribeSubscriptionInstanceStatusRequest
+        @return: DescribeSubscriptionInstanceStatusResponse
+        """
         runtime = util_models.RuntimeOptions()
         return self.describe_subscription_instance_status_with_options(request, runtime)
 
     async def describe_subscription_instance_status_async(
         self,
         request: dts_20200101_models.DescribeSubscriptionInstanceStatusRequest,
     ) -> dts_20200101_models.DescribeSubscriptionInstanceStatusResponse:
+        """
+        @summary Queries the status of a change tracking instance.
+        
+        @param request: DescribeSubscriptionInstanceStatusRequest
+        @return: DescribeSubscriptionInstanceStatusResponse
+        """
         runtime = util_models.RuntimeOptions()
         return await self.describe_subscription_instance_status_with_options_async(request, runtime)
 
     def describe_subscription_instances_with_options(
         self,
         request: dts_20200101_models.DescribeSubscriptionInstancesRequest,
         runtime: util_models.RuntimeOptions,
     ) -> dts_20200101_models.DescribeSubscriptionInstancesResponse:
+        """
+        @summary Queries the list of change tracking instances and the details of each instance.
+        
+        @param request: DescribeSubscriptionInstancesRequest
+        @param runtime: runtime options for this request RuntimeOptions
+        @return: DescribeSubscriptionInstancesResponse
+        """
         UtilClient.validate_model(request)
         query = {}
         if not UtilClient.is_unset(request.account_id):
             query['AccountId'] = request.account_id
         if not UtilClient.is_unset(request.client_token):
             query['ClientToken'] = request.client_token
         if not UtilClient.is_unset(request.owner_id):
@@ -6599,14 +7504,21 @@
         )
 
     async def describe_subscription_instances_with_options_async(
         self,
         request: dts_20200101_models.DescribeSubscriptionInstancesRequest,
         runtime: util_models.RuntimeOptions,
     ) -> dts_20200101_models.DescribeSubscriptionInstancesResponse:
+        """
+        @summary Queries the list of change tracking instances and the details of each instance.
+        
+        @param request: DescribeSubscriptionInstancesRequest
+        @param runtime: runtime options for this request RuntimeOptions
+        @return: DescribeSubscriptionInstancesResponse
+        """
         UtilClient.validate_model(request)
         query = {}
         if not UtilClient.is_unset(request.account_id):
             query['AccountId'] = request.account_id
         if not UtilClient.is_unset(request.client_token):
             query['ClientToken'] = request.client_token
         if not UtilClient.is_unset(request.owner_id):
@@ -6642,32 +7554,44 @@
             await self.call_api_async(params, req, runtime)
         )
 
     def describe_subscription_instances(
         self,
         request: dts_20200101_models.DescribeSubscriptionInstancesRequest,
     ) -> dts_20200101_models.DescribeSubscriptionInstancesResponse:
+        """
+        @summary Queries the list of change tracking instances and the details of each instance.
+        
+        @param request: DescribeSubscriptionInstancesRequest
+        @return: DescribeSubscriptionInstancesResponse
+        """
         runtime = util_models.RuntimeOptions()
         return self.describe_subscription_instances_with_options(request, runtime)
 
     async def describe_subscription_instances_async(
         self,
         request: dts_20200101_models.DescribeSubscriptionInstancesRequest,
     ) -> dts_20200101_models.DescribeSubscriptionInstancesResponse:
+        """
+        @summary Queries the list of change tracking instances and the details of each instance.
+        
+        @param request: DescribeSubscriptionInstancesRequest
+        @return: DescribeSubscriptionInstancesResponse
+        """
         runtime = util_models.RuntimeOptions()
         return await self.describe_subscription_instances_with_options_async(request, runtime)
 
     def describe_subscription_meta_with_options(
         self,
         tmp_req: dts_20200101_models.DescribeSubscriptionMetaRequest,
         runtime: util_models.RuntimeOptions,
     ) -> dts_20200101_models.DescribeSubscriptionMetaResponse:
         """
-        When Data Transmission Service (DTS) tracks data changes from a PolarDB-X 1.0 instance, data is distributed across the attached ApsaraDB RDS for MySQL instances. DTS runs a subtask for each ApsaraDB RDS for MySQL instance. You can call this operation to query the details of the subtasks in a distributed change tracking task.
-        *   You can call the [DescribeDtsJobs](~~209702~~) operation to query the ID of the change tracking instance and the ID of the consumer group.
+        @description    When Data Transmission Service (DTS) tracks data changes from a PolarDB-X 1.0 instance, data is distributed across the attached ApsaraDB RDS for MySQL instances. DTS runs a subtask for each ApsaraDB RDS for MySQL instance. You can call this operation to query the details of the subtasks in a distributed change tracking task.
+        You can call the [DescribeDtsJobs](https://help.aliyun.com/document_detail/209702.html) operation to query the ID of the change tracking instance and the ID of the consumer group.
         
         @param tmp_req: DescribeSubscriptionMetaRequest
         @param runtime: runtime options for this request RuntimeOptions
         @return: DescribeSubscriptionMetaResponse
         """
         UtilClient.validate_model(tmp_req)
         request = dts_20200101_models.DescribeSubscriptionMetaShrinkRequest()
@@ -6710,16 +7634,16 @@
 
     async def describe_subscription_meta_with_options_async(
         self,
         tmp_req: dts_20200101_models.DescribeSubscriptionMetaRequest,
         runtime: util_models.RuntimeOptions,
     ) -> dts_20200101_models.DescribeSubscriptionMetaResponse:
         """
-        When Data Transmission Service (DTS) tracks data changes from a PolarDB-X 1.0 instance, data is distributed across the attached ApsaraDB RDS for MySQL instances. DTS runs a subtask for each ApsaraDB RDS for MySQL instance. You can call this operation to query the details of the subtasks in a distributed change tracking task.
-        *   You can call the [DescribeDtsJobs](~~209702~~) operation to query the ID of the change tracking instance and the ID of the consumer group.
+        @description    When Data Transmission Service (DTS) tracks data changes from a PolarDB-X 1.0 instance, data is distributed across the attached ApsaraDB RDS for MySQL instances. DTS runs a subtask for each ApsaraDB RDS for MySQL instance. You can call this operation to query the details of the subtasks in a distributed change tracking task.
+        You can call the [DescribeDtsJobs](https://help.aliyun.com/document_detail/209702.html) operation to query the ID of the change tracking instance and the ID of the consumer group.
         
         @param tmp_req: DescribeSubscriptionMetaRequest
         @param runtime: runtime options for this request RuntimeOptions
         @return: DescribeSubscriptionMetaResponse
         """
         UtilClient.validate_model(tmp_req)
         request = dts_20200101_models.DescribeSubscriptionMetaShrinkRequest()
@@ -6761,42 +7685,49 @@
         )
 
     def describe_subscription_meta(
         self,
         request: dts_20200101_models.DescribeSubscriptionMetaRequest,
     ) -> dts_20200101_models.DescribeSubscriptionMetaResponse:
         """
-        When Data Transmission Service (DTS) tracks data changes from a PolarDB-X 1.0 instance, data is distributed across the attached ApsaraDB RDS for MySQL instances. DTS runs a subtask for each ApsaraDB RDS for MySQL instance. You can call this operation to query the details of the subtasks in a distributed change tracking task.
-        *   You can call the [DescribeDtsJobs](~~209702~~) operation to query the ID of the change tracking instance and the ID of the consumer group.
+        @description    When Data Transmission Service (DTS) tracks data changes from a PolarDB-X 1.0 instance, data is distributed across the attached ApsaraDB RDS for MySQL instances. DTS runs a subtask for each ApsaraDB RDS for MySQL instance. You can call this operation to query the details of the subtasks in a distributed change tracking task.
+        You can call the [DescribeDtsJobs](https://help.aliyun.com/document_detail/209702.html) operation to query the ID of the change tracking instance and the ID of the consumer group.
         
         @param request: DescribeSubscriptionMetaRequest
         @return: DescribeSubscriptionMetaResponse
         """
         runtime = util_models.RuntimeOptions()
         return self.describe_subscription_meta_with_options(request, runtime)
 
     async def describe_subscription_meta_async(
         self,
         request: dts_20200101_models.DescribeSubscriptionMetaRequest,
     ) -> dts_20200101_models.DescribeSubscriptionMetaResponse:
         """
-        When Data Transmission Service (DTS) tracks data changes from a PolarDB-X 1.0 instance, data is distributed across the attached ApsaraDB RDS for MySQL instances. DTS runs a subtask for each ApsaraDB RDS for MySQL instance. You can call this operation to query the details of the subtasks in a distributed change tracking task.
-        *   You can call the [DescribeDtsJobs](~~209702~~) operation to query the ID of the change tracking instance and the ID of the consumer group.
+        @description    When Data Transmission Service (DTS) tracks data changes from a PolarDB-X 1.0 instance, data is distributed across the attached ApsaraDB RDS for MySQL instances. DTS runs a subtask for each ApsaraDB RDS for MySQL instance. You can call this operation to query the details of the subtasks in a distributed change tracking task.
+        You can call the [DescribeDtsJobs](https://help.aliyun.com/document_detail/209702.html) operation to query the ID of the change tracking instance and the ID of the consumer group.
         
         @param request: DescribeSubscriptionMetaRequest
         @return: DescribeSubscriptionMetaResponse
         """
         runtime = util_models.RuntimeOptions()
         return await self.describe_subscription_meta_with_options_async(request, runtime)
 
     def describe_sync_status_with_options(
         self,
         request: dts_20200101_models.DescribeSyncStatusRequest,
         runtime: util_models.RuntimeOptions,
     ) -> dts_20200101_models.DescribeSyncStatusResponse:
+        """
+        @summary 查看同步和迁移任务的增量写入延迟信息
+        
+        @param request: DescribeSyncStatusRequest
+        @param runtime: runtime options for this request RuntimeOptions
+        @return: DescribeSyncStatusResponse
+        """
         UtilClient.validate_model(request)
         query = {}
         if not UtilClient.is_unset(request.direction):
             query['Direction'] = request.direction
         if not UtilClient.is_unset(request.dts_instance_id):
             query['DtsInstanceId'] = request.dts_instance_id
         if not UtilClient.is_unset(request.dts_job_id):
@@ -6825,14 +7756,21 @@
         )
 
     async def describe_sync_status_with_options_async(
         self,
         request: dts_20200101_models.DescribeSyncStatusRequest,
         runtime: util_models.RuntimeOptions,
     ) -> dts_20200101_models.DescribeSyncStatusResponse:
+        """
+        @summary 查看同步和迁移任务的增量写入延迟信息
+        
+        @param request: DescribeSyncStatusRequest
+        @param runtime: runtime options for this request RuntimeOptions
+        @return: DescribeSyncStatusResponse
+        """
         UtilClient.validate_model(request)
         query = {}
         if not UtilClient.is_unset(request.direction):
             query['Direction'] = request.direction
         if not UtilClient.is_unset(request.dts_instance_id):
             query['DtsInstanceId'] = request.dts_instance_id
         if not UtilClient.is_unset(request.dts_job_id):
@@ -6860,29 +7798,46 @@
             await self.call_api_async(params, req, runtime)
         )
 
     def describe_sync_status(
         self,
         request: dts_20200101_models.DescribeSyncStatusRequest,
     ) -> dts_20200101_models.DescribeSyncStatusResponse:
+        """
+        @summary 查看同步和迁移任务的增量写入延迟信息
+        
+        @param request: DescribeSyncStatusRequest
+        @return: DescribeSyncStatusResponse
+        """
         runtime = util_models.RuntimeOptions()
         return self.describe_sync_status_with_options(request, runtime)
 
     async def describe_sync_status_async(
         self,
         request: dts_20200101_models.DescribeSyncStatusRequest,
     ) -> dts_20200101_models.DescribeSyncStatusResponse:
+        """
+        @summary 查看同步和迁移任务的增量写入延迟信息
+        
+        @param request: DescribeSyncStatusRequest
+        @return: DescribeSyncStatusResponse
+        """
         runtime = util_models.RuntimeOptions()
         return await self.describe_sync_status_with_options_async(request, runtime)
 
     def describe_synchronization_job_alert_with_options(
         self,
         request: dts_20200101_models.DescribeSynchronizationJobAlertRequest,
         runtime: util_models.RuntimeOptions,
     ) -> dts_20200101_models.DescribeSynchronizationJobAlertResponse:
+        """
+        @param request: DescribeSynchronizationJobAlertRequest
+        @param runtime: runtime options for this request RuntimeOptions
+        @return: DescribeSynchronizationJobAlertResponse
+        """
         UtilClient.validate_model(request)
         query = {}
         if not UtilClient.is_unset(request.account_id):
             query['AccountId'] = request.account_id
         if not UtilClient.is_unset(request.client_token):
             query['ClientToken'] = request.client_token
         if not UtilClient.is_unset(request.owner_id):
@@ -6915,14 +7870,19 @@
         )
 
     async def describe_synchronization_job_alert_with_options_async(
         self,
         request: dts_20200101_models.DescribeSynchronizationJobAlertRequest,
         runtime: util_models.RuntimeOptions,
     ) -> dts_20200101_models.DescribeSynchronizationJobAlertResponse:
+        """
+        @param request: DescribeSynchronizationJobAlertRequest
+        @param runtime: runtime options for this request RuntimeOptions
+        @return: DescribeSynchronizationJobAlertResponse
+        """
         UtilClient.validate_model(request)
         query = {}
         if not UtilClient.is_unset(request.account_id):
             query['AccountId'] = request.account_id
         if not UtilClient.is_unset(request.client_token):
             query['ClientToken'] = request.client_token
         if not UtilClient.is_unset(request.owner_id):
@@ -6954,29 +7914,42 @@
             await self.call_api_async(params, req, runtime)
         )
 
     def describe_synchronization_job_alert(
         self,
         request: dts_20200101_models.DescribeSynchronizationJobAlertRequest,
     ) -> dts_20200101_models.DescribeSynchronizationJobAlertResponse:
+        """
+        @param request: DescribeSynchronizationJobAlertRequest
+        @return: DescribeSynchronizationJobAlertResponse
+        """
         runtime = util_models.RuntimeOptions()
         return self.describe_synchronization_job_alert_with_options(request, runtime)
 
     async def describe_synchronization_job_alert_async(
         self,
         request: dts_20200101_models.DescribeSynchronizationJobAlertRequest,
     ) -> dts_20200101_models.DescribeSynchronizationJobAlertResponse:
+        """
+        @param request: DescribeSynchronizationJobAlertRequest
+        @return: DescribeSynchronizationJobAlertResponse
+        """
         runtime = util_models.RuntimeOptions()
         return await self.describe_synchronization_job_alert_with_options_async(request, runtime)
 
     def describe_synchronization_job_replicator_compare_with_options(
         self,
         request: dts_20200101_models.DescribeSynchronizationJobReplicatorCompareRequest,
         runtime: util_models.RuntimeOptions,
     ) -> dts_20200101_models.DescribeSynchronizationJobReplicatorCompareResponse:
+        """
+        @param request: DescribeSynchronizationJobReplicatorCompareRequest
+        @param runtime: runtime options for this request RuntimeOptions
+        @return: DescribeSynchronizationJobReplicatorCompareResponse
+        """
         UtilClient.validate_model(request)
         query = {}
         if not UtilClient.is_unset(request.account_id):
             query['AccountId'] = request.account_id
         if not UtilClient.is_unset(request.client_token):
             query['ClientToken'] = request.client_token
         if not UtilClient.is_unset(request.owner_id):
@@ -7009,14 +7982,19 @@
         )
 
     async def describe_synchronization_job_replicator_compare_with_options_async(
         self,
         request: dts_20200101_models.DescribeSynchronizationJobReplicatorCompareRequest,
         runtime: util_models.RuntimeOptions,
     ) -> dts_20200101_models.DescribeSynchronizationJobReplicatorCompareResponse:
+        """
+        @param request: DescribeSynchronizationJobReplicatorCompareRequest
+        @param runtime: runtime options for this request RuntimeOptions
+        @return: DescribeSynchronizationJobReplicatorCompareResponse
+        """
         UtilClient.validate_model(request)
         query = {}
         if not UtilClient.is_unset(request.account_id):
             query['AccountId'] = request.account_id
         if not UtilClient.is_unset(request.client_token):
             query['ClientToken'] = request.client_token
         if not UtilClient.is_unset(request.owner_id):
@@ -7048,29 +8026,44 @@
             await self.call_api_async(params, req, runtime)
         )
 
     def describe_synchronization_job_replicator_compare(
         self,
         request: dts_20200101_models.DescribeSynchronizationJobReplicatorCompareRequest,
     ) -> dts_20200101_models.DescribeSynchronizationJobReplicatorCompareResponse:
+        """
+        @param request: DescribeSynchronizationJobReplicatorCompareRequest
+        @return: DescribeSynchronizationJobReplicatorCompareResponse
+        """
         runtime = util_models.RuntimeOptions()
         return self.describe_synchronization_job_replicator_compare_with_options(request, runtime)
 
     async def describe_synchronization_job_replicator_compare_async(
         self,
         request: dts_20200101_models.DescribeSynchronizationJobReplicatorCompareRequest,
     ) -> dts_20200101_models.DescribeSynchronizationJobReplicatorCompareResponse:
+        """
+        @param request: DescribeSynchronizationJobReplicatorCompareRequest
+        @return: DescribeSynchronizationJobReplicatorCompareResponse
+        """
         runtime = util_models.RuntimeOptions()
         return await self.describe_synchronization_job_replicator_compare_with_options_async(request, runtime)
 
     def describe_synchronization_job_status_with_options(
         self,
         request: dts_20200101_models.DescribeSynchronizationJobStatusRequest,
         runtime: util_models.RuntimeOptions,
     ) -> dts_20200101_models.DescribeSynchronizationJobStatusResponse:
+        """
+        @summary Queries the status of a data synchronization instance.
+        
+        @param request: DescribeSynchronizationJobStatusRequest
+        @param runtime: runtime options for this request RuntimeOptions
+        @return: DescribeSynchronizationJobStatusResponse
+        """
         UtilClient.validate_model(request)
         query = {}
         if not UtilClient.is_unset(request.account_id):
             query['AccountId'] = request.account_id
         if not UtilClient.is_unset(request.client_token):
             query['ClientToken'] = request.client_token
         if not UtilClient.is_unset(request.owner_id):
@@ -7103,14 +8096,21 @@
         )
 
     async def describe_synchronization_job_status_with_options_async(
         self,
         request: dts_20200101_models.DescribeSynchronizationJobStatusRequest,
         runtime: util_models.RuntimeOptions,
     ) -> dts_20200101_models.DescribeSynchronizationJobStatusResponse:
+        """
+        @summary Queries the status of a data synchronization instance.
+        
+        @param request: DescribeSynchronizationJobStatusRequest
+        @param runtime: runtime options for this request RuntimeOptions
+        @return: DescribeSynchronizationJobStatusResponse
+        """
         UtilClient.validate_model(request)
         query = {}
         if not UtilClient.is_unset(request.account_id):
             query['AccountId'] = request.account_id
         if not UtilClient.is_unset(request.client_token):
             query['ClientToken'] = request.client_token
         if not UtilClient.is_unset(request.owner_id):
@@ -7142,29 +8142,46 @@
             await self.call_api_async(params, req, runtime)
         )
 
     def describe_synchronization_job_status(
         self,
         request: dts_20200101_models.DescribeSynchronizationJobStatusRequest,
     ) -> dts_20200101_models.DescribeSynchronizationJobStatusResponse:
+        """
+        @summary Queries the status of a data synchronization instance.
+        
+        @param request: DescribeSynchronizationJobStatusRequest
+        @return: DescribeSynchronizationJobStatusResponse
+        """
         runtime = util_models.RuntimeOptions()
         return self.describe_synchronization_job_status_with_options(request, runtime)
 
     async def describe_synchronization_job_status_async(
         self,
         request: dts_20200101_models.DescribeSynchronizationJobStatusRequest,
     ) -> dts_20200101_models.DescribeSynchronizationJobStatusResponse:
+        """
+        @summary Queries the status of a data synchronization instance.
+        
+        @param request: DescribeSynchronizationJobStatusRequest
+        @return: DescribeSynchronizationJobStatusResponse
+        """
         runtime = util_models.RuntimeOptions()
         return await self.describe_synchronization_job_status_with_options_async(request, runtime)
 
     def describe_synchronization_job_status_list_with_options(
         self,
         request: dts_20200101_models.DescribeSynchronizationJobStatusListRequest,
         runtime: util_models.RuntimeOptions,
     ) -> dts_20200101_models.DescribeSynchronizationJobStatusListResponse:
+        """
+        @param request: DescribeSynchronizationJobStatusListRequest
+        @param runtime: runtime options for this request RuntimeOptions
+        @return: DescribeSynchronizationJobStatusListResponse
+        """
         UtilClient.validate_model(request)
         query = {}
         if not UtilClient.is_unset(request.account_id):
             query['AccountId'] = request.account_id
         if not UtilClient.is_unset(request.client_token):
             query['ClientToken'] = request.client_token
         if not UtilClient.is_unset(request.owner_id):
@@ -7195,14 +8212,19 @@
         )
 
     async def describe_synchronization_job_status_list_with_options_async(
         self,
         request: dts_20200101_models.DescribeSynchronizationJobStatusListRequest,
         runtime: util_models.RuntimeOptions,
     ) -> dts_20200101_models.DescribeSynchronizationJobStatusListResponse:
+        """
+        @param request: DescribeSynchronizationJobStatusListRequest
+        @param runtime: runtime options for this request RuntimeOptions
+        @return: DescribeSynchronizationJobStatusListResponse
+        """
         UtilClient.validate_model(request)
         query = {}
         if not UtilClient.is_unset(request.account_id):
             query['AccountId'] = request.account_id
         if not UtilClient.is_unset(request.client_token):
             query['ClientToken'] = request.client_token
         if not UtilClient.is_unset(request.owner_id):
@@ -7232,29 +8254,44 @@
             await self.call_api_async(params, req, runtime)
         )
 
     def describe_synchronization_job_status_list(
         self,
         request: dts_20200101_models.DescribeSynchronizationJobStatusListRequest,
     ) -> dts_20200101_models.DescribeSynchronizationJobStatusListResponse:
+        """
+        @param request: DescribeSynchronizationJobStatusListRequest
+        @return: DescribeSynchronizationJobStatusListResponse
+        """
         runtime = util_models.RuntimeOptions()
         return self.describe_synchronization_job_status_list_with_options(request, runtime)
 
     async def describe_synchronization_job_status_list_async(
         self,
         request: dts_20200101_models.DescribeSynchronizationJobStatusListRequest,
     ) -> dts_20200101_models.DescribeSynchronizationJobStatusListResponse:
+        """
+        @param request: DescribeSynchronizationJobStatusListRequest
+        @return: DescribeSynchronizationJobStatusListResponse
+        """
         runtime = util_models.RuntimeOptions()
         return await self.describe_synchronization_job_status_list_with_options_async(request, runtime)
 
     def describe_synchronization_jobs_with_options(
         self,
         request: dts_20200101_models.DescribeSynchronizationJobsRequest,
         runtime: util_models.RuntimeOptions,
     ) -> dts_20200101_models.DescribeSynchronizationJobsResponse:
+        """
+        @summary The number of entries to return on each page. Valid values: *30**, **50**, and **100**. Default value: **30**.
+        
+        @param request: DescribeSynchronizationJobsRequest
+        @param runtime: runtime options for this request RuntimeOptions
+        @return: DescribeSynchronizationJobsResponse
+        """
         UtilClient.validate_model(request)
         query = {}
         if not UtilClient.is_unset(request.account_id):
             query['AccountId'] = request.account_id
         if not UtilClient.is_unset(request.client_token):
             query['ClientToken'] = request.client_token
         if not UtilClient.is_unset(request.owner_id):
@@ -7291,14 +8328,21 @@
         )
 
     async def describe_synchronization_jobs_with_options_async(
         self,
         request: dts_20200101_models.DescribeSynchronizationJobsRequest,
         runtime: util_models.RuntimeOptions,
     ) -> dts_20200101_models.DescribeSynchronizationJobsResponse:
+        """
+        @summary The number of entries to return on each page. Valid values: *30**, **50**, and **100**. Default value: **30**.
+        
+        @param request: DescribeSynchronizationJobsRequest
+        @param runtime: runtime options for this request RuntimeOptions
+        @return: DescribeSynchronizationJobsResponse
+        """
         UtilClient.validate_model(request)
         query = {}
         if not UtilClient.is_unset(request.account_id):
             query['AccountId'] = request.account_id
         if not UtilClient.is_unset(request.client_token):
             query['ClientToken'] = request.client_token
         if not UtilClient.is_unset(request.owner_id):
@@ -7334,31 +8378,43 @@
             await self.call_api_async(params, req, runtime)
         )
 
     def describe_synchronization_jobs(
         self,
         request: dts_20200101_models.DescribeSynchronizationJobsRequest,
     ) -> dts_20200101_models.DescribeSynchronizationJobsResponse:
+        """
+        @summary The number of entries to return on each page. Valid values: *30**, **50**, and **100**. Default value: **30**.
+        
+        @param request: DescribeSynchronizationJobsRequest
+        @return: DescribeSynchronizationJobsResponse
+        """
         runtime = util_models.RuntimeOptions()
         return self.describe_synchronization_jobs_with_options(request, runtime)
 
     async def describe_synchronization_jobs_async(
         self,
         request: dts_20200101_models.DescribeSynchronizationJobsRequest,
     ) -> dts_20200101_models.DescribeSynchronizationJobsResponse:
+        """
+        @summary The number of entries to return on each page. Valid values: *30**, **50**, and **100**. Default value: **30**.
+        
+        @param request: DescribeSynchronizationJobsRequest
+        @return: DescribeSynchronizationJobsResponse
+        """
         runtime = util_models.RuntimeOptions()
         return await self.describe_synchronization_jobs_with_options_async(request, runtime)
 
     def describe_synchronization_object_modify_status_with_options(
         self,
         request: dts_20200101_models.DescribeSynchronizationObjectModifyStatusRequest,
         runtime: util_models.RuntimeOptions,
     ) -> dts_20200101_models.DescribeSynchronizationObjectModifyStatusResponse:
         """
-        Before you call this operation, you must call the [ModifySynchronizationObject](~~49451~~) operation to obtain the task ID.
+        @description Before you call this operation, you must call the [ModifySynchronizationObject](https://help.aliyun.com/document_detail/49451.html) operation to obtain the task ID.
         
         @param request: DescribeSynchronizationObjectModifyStatusRequest
         @param runtime: runtime options for this request RuntimeOptions
         @return: DescribeSynchronizationObjectModifyStatusResponse
         """
         UtilClient.validate_model(request)
         query = {}
@@ -7395,15 +8451,15 @@
 
     async def describe_synchronization_object_modify_status_with_options_async(
         self,
         request: dts_20200101_models.DescribeSynchronizationObjectModifyStatusRequest,
         runtime: util_models.RuntimeOptions,
     ) -> dts_20200101_models.DescribeSynchronizationObjectModifyStatusResponse:
         """
-        Before you call this operation, you must call the [ModifySynchronizationObject](~~49451~~) operation to obtain the task ID.
+        @description Before you call this operation, you must call the [ModifySynchronizationObject](https://help.aliyun.com/document_detail/49451.html) operation to obtain the task ID.
         
         @param request: DescribeSynchronizationObjectModifyStatusRequest
         @param runtime: runtime options for this request RuntimeOptions
         @return: DescribeSynchronizationObjectModifyStatusResponse
         """
         UtilClient.validate_model(request)
         query = {}
@@ -7439,40 +8495,45 @@
         )
 
     def describe_synchronization_object_modify_status(
         self,
         request: dts_20200101_models.DescribeSynchronizationObjectModifyStatusRequest,
     ) -> dts_20200101_models.DescribeSynchronizationObjectModifyStatusResponse:
         """
-        Before you call this operation, you must call the [ModifySynchronizationObject](~~49451~~) operation to obtain the task ID.
+        @description Before you call this operation, you must call the [ModifySynchronizationObject](https://help.aliyun.com/document_detail/49451.html) operation to obtain the task ID.
         
         @param request: DescribeSynchronizationObjectModifyStatusRequest
         @return: DescribeSynchronizationObjectModifyStatusResponse
         """
         runtime = util_models.RuntimeOptions()
         return self.describe_synchronization_object_modify_status_with_options(request, runtime)
 
     async def describe_synchronization_object_modify_status_async(
         self,
         request: dts_20200101_models.DescribeSynchronizationObjectModifyStatusRequest,
     ) -> dts_20200101_models.DescribeSynchronizationObjectModifyStatusResponse:
         """
-        Before you call this operation, you must call the [ModifySynchronizationObject](~~49451~~) operation to obtain the task ID.
+        @description Before you call this operation, you must call the [ModifySynchronizationObject](https://help.aliyun.com/document_detail/49451.html) operation to obtain the task ID.
         
         @param request: DescribeSynchronizationObjectModifyStatusRequest
         @return: DescribeSynchronizationObjectModifyStatusResponse
         """
         runtime = util_models.RuntimeOptions()
         return await self.describe_synchronization_object_modify_status_with_options_async(request, runtime)
 
     def describe_tag_keys_with_options(
         self,
         request: dts_20200101_models.DescribeTagKeysRequest,
         runtime: util_models.RuntimeOptions,
     ) -> dts_20200101_models.DescribeTagKeysResponse:
+        """
+        @param request: DescribeTagKeysRequest
+        @param runtime: runtime options for this request RuntimeOptions
+        @return: DescribeTagKeysResponse
+        """
         UtilClient.validate_model(request)
         query = {}
         if not UtilClient.is_unset(request.category):
             query['Category'] = request.category
         if not UtilClient.is_unset(request.page_number):
             query['PageNumber'] = request.page_number
         if not UtilClient.is_unset(request.page_size):
@@ -7505,14 +8566,19 @@
         )
 
     async def describe_tag_keys_with_options_async(
         self,
         request: dts_20200101_models.DescribeTagKeysRequest,
         runtime: util_models.RuntimeOptions,
     ) -> dts_20200101_models.DescribeTagKeysResponse:
+        """
+        @param request: DescribeTagKeysRequest
+        @param runtime: runtime options for this request RuntimeOptions
+        @return: DescribeTagKeysResponse
+        """
         UtilClient.validate_model(request)
         query = {}
         if not UtilClient.is_unset(request.category):
             query['Category'] = request.category
         if not UtilClient.is_unset(request.page_number):
             query['PageNumber'] = request.page_number
         if not UtilClient.is_unset(request.page_size):
@@ -7544,29 +8610,42 @@
             await self.call_api_async(params, req, runtime)
         )
 
     def describe_tag_keys(
         self,
         request: dts_20200101_models.DescribeTagKeysRequest,
     ) -> dts_20200101_models.DescribeTagKeysResponse:
+        """
+        @param request: DescribeTagKeysRequest
+        @return: DescribeTagKeysResponse
+        """
         runtime = util_models.RuntimeOptions()
         return self.describe_tag_keys_with_options(request, runtime)
 
     async def describe_tag_keys_async(
         self,
         request: dts_20200101_models.DescribeTagKeysRequest,
     ) -> dts_20200101_models.DescribeTagKeysResponse:
+        """
+        @param request: DescribeTagKeysRequest
+        @return: DescribeTagKeysResponse
+        """
         runtime = util_models.RuntimeOptions()
         return await self.describe_tag_keys_with_options_async(request, runtime)
 
     def describe_tag_values_with_options(
         self,
         request: dts_20200101_models.DescribeTagValuesRequest,
         runtime: util_models.RuntimeOptions,
     ) -> dts_20200101_models.DescribeTagValuesResponse:
+        """
+        @param request: DescribeTagValuesRequest
+        @param runtime: runtime options for this request RuntimeOptions
+        @return: DescribeTagValuesResponse
+        """
         UtilClient.validate_model(request)
         query = {}
         if not UtilClient.is_unset(request.category):
             query['Category'] = request.category
         if not UtilClient.is_unset(request.key):
             query['Key'] = request.key
         if not UtilClient.is_unset(request.page_number):
@@ -7601,14 +8680,19 @@
         )
 
     async def describe_tag_values_with_options_async(
         self,
         request: dts_20200101_models.DescribeTagValuesRequest,
         runtime: util_models.RuntimeOptions,
     ) -> dts_20200101_models.DescribeTagValuesResponse:
+        """
+        @param request: DescribeTagValuesRequest
+        @param runtime: runtime options for this request RuntimeOptions
+        @return: DescribeTagValuesResponse
+        """
         UtilClient.validate_model(request)
         query = {}
         if not UtilClient.is_unset(request.category):
             query['Category'] = request.category
         if not UtilClient.is_unset(request.key):
             query['Key'] = request.key
         if not UtilClient.is_unset(request.page_number):
@@ -7642,32 +8726,42 @@
             await self.call_api_async(params, req, runtime)
         )
 
     def describe_tag_values(
         self,
         request: dts_20200101_models.DescribeTagValuesRequest,
     ) -> dts_20200101_models.DescribeTagValuesResponse:
+        """
+        @param request: DescribeTagValuesRequest
+        @return: DescribeTagValuesResponse
+        """
         runtime = util_models.RuntimeOptions()
         return self.describe_tag_values_with_options(request, runtime)
 
     async def describe_tag_values_async(
         self,
         request: dts_20200101_models.DescribeTagValuesRequest,
     ) -> dts_20200101_models.DescribeTagValuesResponse:
+        """
+        @param request: DescribeTagValuesRequest
+        @return: DescribeTagValuesResponse
+        """
         runtime = util_models.RuntimeOptions()
         return await self.describe_tag_values_with_options_async(request, runtime)
 
     def init_dts_rds_instance_with_options(
         self,
         request: dts_20200101_models.InitDtsRdsInstanceRequest,
         runtime: util_models.RuntimeOptions,
     ) -> dts_20200101_models.InitDtsRdsInstanceResponse:
         """
-        The node must be an ApsaraDB RDS for MySQL instance or a self-managed MySQL database that is connected over Cloud Enterprise Network (CEN).
-        *   This operation is used to initialize the built-in account named rdsdt_dtsacct on a node of an active geo-redundancy database cluster. DTS uses this account to connect to the node and perform data synchronization tasks.
+        @summary Initializes a built-in account on a node of an active geo-redundancy database cluster. Data Transmission Service (DTS) uses the built-in account to connect to the node and perform data synchronization tasks.
+        
+        @description    The node must be an ApsaraDB RDS for MySQL instance or a self-managed MySQL database that is connected over Cloud Enterprise Network (CEN).
+        This operation is used to initialize the built-in account named rdsdt_dtsacct on a node of an active geo-redundancy database cluster. DTS uses this account to connect to the node and perform data synchronization tasks.
         
         @param request: InitDtsRdsInstanceRequest
         @param runtime: runtime options for this request RuntimeOptions
         @return: InitDtsRdsInstanceResponse
         """
         UtilClient.validate_model(request)
         query = {}
@@ -7706,16 +8800,18 @@
 
     async def init_dts_rds_instance_with_options_async(
         self,
         request: dts_20200101_models.InitDtsRdsInstanceRequest,
         runtime: util_models.RuntimeOptions,
     ) -> dts_20200101_models.InitDtsRdsInstanceResponse:
         """
-        The node must be an ApsaraDB RDS for MySQL instance or a self-managed MySQL database that is connected over Cloud Enterprise Network (CEN).
-        *   This operation is used to initialize the built-in account named rdsdt_dtsacct on a node of an active geo-redundancy database cluster. DTS uses this account to connect to the node and perform data synchronization tasks.
+        @summary Initializes a built-in account on a node of an active geo-redundancy database cluster. Data Transmission Service (DTS) uses the built-in account to connect to the node and perform data synchronization tasks.
+        
+        @description    The node must be an ApsaraDB RDS for MySQL instance or a self-managed MySQL database that is connected over Cloud Enterprise Network (CEN).
+        This operation is used to initialize the built-in account named rdsdt_dtsacct on a node of an active geo-redundancy database cluster. DTS uses this account to connect to the node and perform data synchronization tasks.
         
         @param request: InitDtsRdsInstanceRequest
         @param runtime: runtime options for this request RuntimeOptions
         @return: InitDtsRdsInstanceResponse
         """
         UtilClient.validate_model(request)
         query = {}
@@ -7753,42 +8849,53 @@
         )
 
     def init_dts_rds_instance(
         self,
         request: dts_20200101_models.InitDtsRdsInstanceRequest,
     ) -> dts_20200101_models.InitDtsRdsInstanceResponse:
         """
-        The node must be an ApsaraDB RDS for MySQL instance or a self-managed MySQL database that is connected over Cloud Enterprise Network (CEN).
-        *   This operation is used to initialize the built-in account named rdsdt_dtsacct on a node of an active geo-redundancy database cluster. DTS uses this account to connect to the node and perform data synchronization tasks.
+        @summary Initializes a built-in account on a node of an active geo-redundancy database cluster. Data Transmission Service (DTS) uses the built-in account to connect to the node and perform data synchronization tasks.
+        
+        @description    The node must be an ApsaraDB RDS for MySQL instance or a self-managed MySQL database that is connected over Cloud Enterprise Network (CEN).
+        This operation is used to initialize the built-in account named rdsdt_dtsacct on a node of an active geo-redundancy database cluster. DTS uses this account to connect to the node and perform data synchronization tasks.
         
         @param request: InitDtsRdsInstanceRequest
         @return: InitDtsRdsInstanceResponse
         """
         runtime = util_models.RuntimeOptions()
         return self.init_dts_rds_instance_with_options(request, runtime)
 
     async def init_dts_rds_instance_async(
         self,
         request: dts_20200101_models.InitDtsRdsInstanceRequest,
     ) -> dts_20200101_models.InitDtsRdsInstanceResponse:
         """
-        The node must be an ApsaraDB RDS for MySQL instance or a self-managed MySQL database that is connected over Cloud Enterprise Network (CEN).
-        *   This operation is used to initialize the built-in account named rdsdt_dtsacct on a node of an active geo-redundancy database cluster. DTS uses this account to connect to the node and perform data synchronization tasks.
+        @summary Initializes a built-in account on a node of an active geo-redundancy database cluster. Data Transmission Service (DTS) uses the built-in account to connect to the node and perform data synchronization tasks.
+        
+        @description    The node must be an ApsaraDB RDS for MySQL instance or a self-managed MySQL database that is connected over Cloud Enterprise Network (CEN).
+        This operation is used to initialize the built-in account named rdsdt_dtsacct on a node of an active geo-redundancy database cluster. DTS uses this account to connect to the node and perform data synchronization tasks.
         
         @param request: InitDtsRdsInstanceRequest
         @return: InitDtsRdsInstanceResponse
         """
         runtime = util_models.RuntimeOptions()
         return await self.init_dts_rds_instance_with_options_async(request, runtime)
 
     def list_dedicated_cluster_with_options(
         self,
         request: dts_20200101_models.ListDedicatedClusterRequest,
         runtime: util_models.RuntimeOptions,
     ) -> dts_20200101_models.ListDedicatedClusterResponse:
+        """
+        @summary Queries all clusters that are created within an Alibaba Cloud account. You can also query clusters based on the specified conditions.
+        
+        @param request: ListDedicatedClusterRequest
+        @param runtime: runtime options for this request RuntimeOptions
+        @return: ListDedicatedClusterResponse
+        """
         UtilClient.validate_model(request)
         query = {}
         if not UtilClient.is_unset(request.order_column):
             query['OrderColumn'] = request.order_column
         if not UtilClient.is_unset(request.order_direction):
             query['OrderDirection'] = request.order_direction
         if not UtilClient.is_unset(request.owner_id):
@@ -7827,14 +8934,21 @@
         )
 
     async def list_dedicated_cluster_with_options_async(
         self,
         request: dts_20200101_models.ListDedicatedClusterRequest,
         runtime: util_models.RuntimeOptions,
     ) -> dts_20200101_models.ListDedicatedClusterResponse:
+        """
+        @summary Queries all clusters that are created within an Alibaba Cloud account. You can also query clusters based on the specified conditions.
+        
+        @param request: ListDedicatedClusterRequest
+        @param runtime: runtime options for this request RuntimeOptions
+        @return: ListDedicatedClusterResponse
+        """
         UtilClient.validate_model(request)
         query = {}
         if not UtilClient.is_unset(request.order_column):
             query['OrderColumn'] = request.order_column
         if not UtilClient.is_unset(request.order_direction):
             query['OrderDirection'] = request.order_direction
         if not UtilClient.is_unset(request.owner_id):
@@ -7872,31 +8986,43 @@
             await self.call_api_async(params, req, runtime)
         )
 
     def list_dedicated_cluster(
         self,
         request: dts_20200101_models.ListDedicatedClusterRequest,
     ) -> dts_20200101_models.ListDedicatedClusterResponse:
+        """
+        @summary Queries all clusters that are created within an Alibaba Cloud account. You can also query clusters based on the specified conditions.
+        
+        @param request: ListDedicatedClusterRequest
+        @return: ListDedicatedClusterResponse
+        """
         runtime = util_models.RuntimeOptions()
         return self.list_dedicated_cluster_with_options(request, runtime)
 
     async def list_dedicated_cluster_async(
         self,
         request: dts_20200101_models.ListDedicatedClusterRequest,
     ) -> dts_20200101_models.ListDedicatedClusterResponse:
+        """
+        @summary Queries all clusters that are created within an Alibaba Cloud account. You can also query clusters based on the specified conditions.
+        
+        @param request: ListDedicatedClusterRequest
+        @return: ListDedicatedClusterResponse
+        """
         runtime = util_models.RuntimeOptions()
         return await self.list_dedicated_cluster_with_options_async(request, runtime)
 
     def list_tag_resources_with_options(
         self,
         request: dts_20200101_models.ListTagResourcesRequest,
         runtime: util_models.RuntimeOptions,
     ) -> dts_20200101_models.ListTagResourcesResponse:
         """
-        ***\
+        @description ***\
         
         @param request: ListTagResourcesRequest
         @param runtime: runtime options for this request RuntimeOptions
         @return: ListTagResourcesResponse
         """
         UtilClient.validate_model(request)
         query = {}
@@ -7933,15 +9059,15 @@
 
     async def list_tag_resources_with_options_async(
         self,
         request: dts_20200101_models.ListTagResourcesRequest,
         runtime: util_models.RuntimeOptions,
     ) -> dts_20200101_models.ListTagResourcesResponse:
         """
-        ***\
+        @description ***\
         
         @param request: ListTagResourcesRequest
         @param runtime: runtime options for this request RuntimeOptions
         @return: ListTagResourcesResponse
         """
         UtilClient.validate_model(request)
         query = {}
@@ -7977,40 +9103,45 @@
         )
 
     def list_tag_resources(
         self,
         request: dts_20200101_models.ListTagResourcesRequest,
     ) -> dts_20200101_models.ListTagResourcesResponse:
         """
-        ***\
+        @description ***\
         
         @param request: ListTagResourcesRequest
         @return: ListTagResourcesResponse
         """
         runtime = util_models.RuntimeOptions()
         return self.list_tag_resources_with_options(request, runtime)
 
     async def list_tag_resources_async(
         self,
         request: dts_20200101_models.ListTagResourcesRequest,
     ) -> dts_20200101_models.ListTagResourcesResponse:
         """
-        ***\
+        @description ***\
         
         @param request: ListTagResourcesRequest
         @return: ListTagResourcesResponse
         """
         runtime = util_models.RuntimeOptions()
         return await self.list_tag_resources_with_options_async(request, runtime)
 
     def modify_consumer_channel_with_options(
         self,
         request: dts_20200101_models.ModifyConsumerChannelRequest,
         runtime: util_models.RuntimeOptions,
     ) -> dts_20200101_models.ModifyConsumerChannelResponse:
+        """
+        @param request: ModifyConsumerChannelRequest
+        @param runtime: runtime options for this request RuntimeOptions
+        @return: ModifyConsumerChannelResponse
+        """
         UtilClient.validate_model(request)
         query = {}
         if not UtilClient.is_unset(request.consumer_group_id):
             query['ConsumerGroupId'] = request.consumer_group_id
         if not UtilClient.is_unset(request.consumer_group_name):
             query['ConsumerGroupName'] = request.consumer_group_name
         if not UtilClient.is_unset(request.consumer_group_password):
@@ -8045,14 +9176,19 @@
         )
 
     async def modify_consumer_channel_with_options_async(
         self,
         request: dts_20200101_models.ModifyConsumerChannelRequest,
         runtime: util_models.RuntimeOptions,
     ) -> dts_20200101_models.ModifyConsumerChannelResponse:
+        """
+        @param request: ModifyConsumerChannelRequest
+        @param runtime: runtime options for this request RuntimeOptions
+        @return: ModifyConsumerChannelResponse
+        """
         UtilClient.validate_model(request)
         query = {}
         if not UtilClient.is_unset(request.consumer_group_id):
             query['ConsumerGroupId'] = request.consumer_group_id
         if not UtilClient.is_unset(request.consumer_group_name):
             query['ConsumerGroupName'] = request.consumer_group_name
         if not UtilClient.is_unset(request.consumer_group_password):
@@ -8086,33 +9222,41 @@
             await self.call_api_async(params, req, runtime)
         )
 
     def modify_consumer_channel(
         self,
         request: dts_20200101_models.ModifyConsumerChannelRequest,
     ) -> dts_20200101_models.ModifyConsumerChannelResponse:
+        """
+        @param request: ModifyConsumerChannelRequest
+        @return: ModifyConsumerChannelResponse
+        """
         runtime = util_models.RuntimeOptions()
         return self.modify_consumer_channel_with_options(request, runtime)
 
     async def modify_consumer_channel_async(
         self,
         request: dts_20200101_models.ModifyConsumerChannelRequest,
     ) -> dts_20200101_models.ModifyConsumerChannelResponse:
+        """
+        @param request: ModifyConsumerChannelRequest
+        @return: ModifyConsumerChannelResponse
+        """
         runtime = util_models.RuntimeOptions()
         return await self.modify_consumer_channel_with_options_async(request, runtime)
 
     def modify_consumer_group_password_with_options(
         self,
         request: dts_20200101_models.ModifyConsumerGroupPasswordRequest,
         runtime: util_models.RuntimeOptions,
     ) -> dts_20200101_models.ModifyConsumerGroupPasswordResponse:
         """
-        >
-        *   This operation is applicable to only the new version of the change tracking feature. To use the new version, you must specify the SubscriptionInstanceNetworkType parameter when you call the ConfigureSubscriptionInstance operation. If you use the previous version, you do not need to specify the **SubscriptionInstanceNetworkType** parameter.
-        *   When you call this operation, the change tracking task must be in the NotStarted, Failed, Normal, or Abnormal state.
+        @description >
+        This operation is applicable to only the new version of the change tracking feature. To use the new version, you must specify the SubscriptionInstanceNetworkType parameter when you call the ConfigureSubscriptionInstance operation. If you use the previous version, you do not need to specify the **SubscriptionInstanceNetworkType** parameter.
+        When you call this operation, the change tracking task must be in the NotStarted, Failed, Normal, or Abnormal state.
         
         @param request: ModifyConsumerGroupPasswordRequest
         @param runtime: runtime options for this request RuntimeOptions
         @return: ModifyConsumerGroupPasswordResponse
         """
         UtilClient.validate_model(request)
         query = {}
@@ -8157,17 +9301,17 @@
 
     async def modify_consumer_group_password_with_options_async(
         self,
         request: dts_20200101_models.ModifyConsumerGroupPasswordRequest,
         runtime: util_models.RuntimeOptions,
     ) -> dts_20200101_models.ModifyConsumerGroupPasswordResponse:
         """
-        >
-        *   This operation is applicable to only the new version of the change tracking feature. To use the new version, you must specify the SubscriptionInstanceNetworkType parameter when you call the ConfigureSubscriptionInstance operation. If you use the previous version, you do not need to specify the **SubscriptionInstanceNetworkType** parameter.
-        *   When you call this operation, the change tracking task must be in the NotStarted, Failed, Normal, or Abnormal state.
+        @description >
+        This operation is applicable to only the new version of the change tracking feature. To use the new version, you must specify the SubscriptionInstanceNetworkType parameter when you call the ConfigureSubscriptionInstance operation. If you use the previous version, you do not need to specify the **SubscriptionInstanceNetworkType** parameter.
+        When you call this operation, the change tracking task must be in the NotStarted, Failed, Normal, or Abnormal state.
         
         @param request: ModifyConsumerGroupPasswordRequest
         @param runtime: runtime options for this request RuntimeOptions
         @return: ModifyConsumerGroupPasswordResponse
         """
         UtilClient.validate_model(request)
         query = {}
@@ -8211,49 +9355,49 @@
         )
 
     def modify_consumer_group_password(
         self,
         request: dts_20200101_models.ModifyConsumerGroupPasswordRequest,
     ) -> dts_20200101_models.ModifyConsumerGroupPasswordResponse:
         """
-        >
-        *   This operation is applicable to only the new version of the change tracking feature. To use the new version, you must specify the SubscriptionInstanceNetworkType parameter when you call the ConfigureSubscriptionInstance operation. If you use the previous version, you do not need to specify the **SubscriptionInstanceNetworkType** parameter.
-        *   When you call this operation, the change tracking task must be in the NotStarted, Failed, Normal, or Abnormal state.
+        @description >
+        This operation is applicable to only the new version of the change tracking feature. To use the new version, you must specify the SubscriptionInstanceNetworkType parameter when you call the ConfigureSubscriptionInstance operation. If you use the previous version, you do not need to specify the **SubscriptionInstanceNetworkType** parameter.
+        When you call this operation, the change tracking task must be in the NotStarted, Failed, Normal, or Abnormal state.
         
         @param request: ModifyConsumerGroupPasswordRequest
         @return: ModifyConsumerGroupPasswordResponse
         """
         runtime = util_models.RuntimeOptions()
         return self.modify_consumer_group_password_with_options(request, runtime)
 
     async def modify_consumer_group_password_async(
         self,
         request: dts_20200101_models.ModifyConsumerGroupPasswordRequest,
     ) -> dts_20200101_models.ModifyConsumerGroupPasswordResponse:
         """
-        >
-        *   This operation is applicable to only the new version of the change tracking feature. To use the new version, you must specify the SubscriptionInstanceNetworkType parameter when you call the ConfigureSubscriptionInstance operation. If you use the previous version, you do not need to specify the **SubscriptionInstanceNetworkType** parameter.
-        *   When you call this operation, the change tracking task must be in the NotStarted, Failed, Normal, or Abnormal state.
+        @description >
+        This operation is applicable to only the new version of the change tracking feature. To use the new version, you must specify the SubscriptionInstanceNetworkType parameter when you call the ConfigureSubscriptionInstance operation. If you use the previous version, you do not need to specify the **SubscriptionInstanceNetworkType** parameter.
+        When you call this operation, the change tracking task must be in the NotStarted, Failed, Normal, or Abnormal state.
         
         @param request: ModifyConsumerGroupPasswordRequest
         @return: ModifyConsumerGroupPasswordResponse
         """
         runtime = util_models.RuntimeOptions()
         return await self.modify_consumer_group_password_with_options_async(request, runtime)
 
     def modify_consumption_timestamp_with_options(
         self,
         request: dts_20200101_models.ModifyConsumptionTimestampRequest,
         runtime: util_models.RuntimeOptions,
     ) -> dts_20200101_models.ModifyConsumptionTimestampResponse:
         """
-        >
-        *   This operation is applicable to only the previous version of the change tracking feature. To use the new version, you must specify the SubscriptionInstanceNetworkType parameter when you call the [ConfigureSubscriptionInstance](~~49437~~) operation. If you use the previous version, you do not need to specify the **SubscriptionInstanceNetworkType** parameter.
-        *   If you use the new version, you need to set the consumption checkpoint on the change tracking client.
-        *   When you call this operation, you must stop the change tracking client, and the change tracking task must be in the Normal state.
+        @description >
+        This operation is applicable to only the previous version of the change tracking feature. To use the new version, you must specify the SubscriptionInstanceNetworkType parameter when you call the [ConfigureSubscriptionInstance](https://help.aliyun.com/document_detail/49437.html) operation. If you use the previous version, you do not need to specify the **SubscriptionInstanceNetworkType** parameter.
+        If you use the new version, you need to set the consumption checkpoint on the change tracking client.
+        When you call this operation, you must stop the change tracking client, and the change tracking task must be in the Normal state.
         
         @param request: ModifyConsumptionTimestampRequest
         @param runtime: runtime options for this request RuntimeOptions
         @return: ModifyConsumptionTimestampResponse
         """
         UtilClient.validate_model(request)
         query = {}
@@ -8290,18 +9434,18 @@
 
     async def modify_consumption_timestamp_with_options_async(
         self,
         request: dts_20200101_models.ModifyConsumptionTimestampRequest,
         runtime: util_models.RuntimeOptions,
     ) -> dts_20200101_models.ModifyConsumptionTimestampResponse:
         """
-        >
-        *   This operation is applicable to only the previous version of the change tracking feature. To use the new version, you must specify the SubscriptionInstanceNetworkType parameter when you call the [ConfigureSubscriptionInstance](~~49437~~) operation. If you use the previous version, you do not need to specify the **SubscriptionInstanceNetworkType** parameter.
-        *   If you use the new version, you need to set the consumption checkpoint on the change tracking client.
-        *   When you call this operation, you must stop the change tracking client, and the change tracking task must be in the Normal state.
+        @description >
+        This operation is applicable to only the previous version of the change tracking feature. To use the new version, you must specify the SubscriptionInstanceNetworkType parameter when you call the [ConfigureSubscriptionInstance](https://help.aliyun.com/document_detail/49437.html) operation. If you use the previous version, you do not need to specify the **SubscriptionInstanceNetworkType** parameter.
+        If you use the new version, you need to set the consumption checkpoint on the change tracking client.
+        When you call this operation, you must stop the change tracking client, and the change tracking task must be in the Normal state.
         
         @param request: ModifyConsumptionTimestampRequest
         @param runtime: runtime options for this request RuntimeOptions
         @return: ModifyConsumptionTimestampResponse
         """
         UtilClient.validate_model(request)
         query = {}
@@ -8337,48 +9481,50 @@
         )
 
     def modify_consumption_timestamp(
         self,
         request: dts_20200101_models.ModifyConsumptionTimestampRequest,
     ) -> dts_20200101_models.ModifyConsumptionTimestampResponse:
         """
-        >
-        *   This operation is applicable to only the previous version of the change tracking feature. To use the new version, you must specify the SubscriptionInstanceNetworkType parameter when you call the [ConfigureSubscriptionInstance](~~49437~~) operation. If you use the previous version, you do not need to specify the **SubscriptionInstanceNetworkType** parameter.
-        *   If you use the new version, you need to set the consumption checkpoint on the change tracking client.
-        *   When you call this operation, you must stop the change tracking client, and the change tracking task must be in the Normal state.
+        @description >
+        This operation is applicable to only the previous version of the change tracking feature. To use the new version, you must specify the SubscriptionInstanceNetworkType parameter when you call the [ConfigureSubscriptionInstance](https://help.aliyun.com/document_detail/49437.html) operation. If you use the previous version, you do not need to specify the **SubscriptionInstanceNetworkType** parameter.
+        If you use the new version, you need to set the consumption checkpoint on the change tracking client.
+        When you call this operation, you must stop the change tracking client, and the change tracking task must be in the Normal state.
         
         @param request: ModifyConsumptionTimestampRequest
         @return: ModifyConsumptionTimestampResponse
         """
         runtime = util_models.RuntimeOptions()
         return self.modify_consumption_timestamp_with_options(request, runtime)
 
     async def modify_consumption_timestamp_async(
         self,
         request: dts_20200101_models.ModifyConsumptionTimestampRequest,
     ) -> dts_20200101_models.ModifyConsumptionTimestampResponse:
         """
-        >
-        *   This operation is applicable to only the previous version of the change tracking feature. To use the new version, you must specify the SubscriptionInstanceNetworkType parameter when you call the [ConfigureSubscriptionInstance](~~49437~~) operation. If you use the previous version, you do not need to specify the **SubscriptionInstanceNetworkType** parameter.
-        *   If you use the new version, you need to set the consumption checkpoint on the change tracking client.
-        *   When you call this operation, you must stop the change tracking client, and the change tracking task must be in the Normal state.
+        @description >
+        This operation is applicable to only the previous version of the change tracking feature. To use the new version, you must specify the SubscriptionInstanceNetworkType parameter when you call the [ConfigureSubscriptionInstance](https://help.aliyun.com/document_detail/49437.html) operation. If you use the previous version, you do not need to specify the **SubscriptionInstanceNetworkType** parameter.
+        If you use the new version, you need to set the consumption checkpoint on the change tracking client.
+        When you call this operation, you must stop the change tracking client, and the change tracking task must be in the Normal state.
         
         @param request: ModifyConsumptionTimestampRequest
         @return: ModifyConsumptionTimestampResponse
         """
         runtime = util_models.RuntimeOptions()
         return await self.modify_consumption_timestamp_with_options_async(request, runtime)
 
     def modify_dedicated_cluster_with_options(
         self,
         request: dts_20200101_models.ModifyDedicatedClusterRequest,
         runtime: util_models.RuntimeOptions,
     ) -> dts_20200101_models.ModifyDedicatedClusterResponse:
         """
-        You can modify only the overcommit ratio.
+        @summary Modifies the configuration of a cluster.
+        
+        @description You can modify only the overcommit ratio.
         
         @param request: ModifyDedicatedClusterRequest
         @param runtime: runtime options for this request RuntimeOptions
         @return: ModifyDedicatedClusterResponse
         """
         UtilClient.validate_model(request)
         query = {}
@@ -8417,15 +9563,17 @@
 
     async def modify_dedicated_cluster_with_options_async(
         self,
         request: dts_20200101_models.ModifyDedicatedClusterRequest,
         runtime: util_models.RuntimeOptions,
     ) -> dts_20200101_models.ModifyDedicatedClusterResponse:
         """
-        You can modify only the overcommit ratio.
+        @summary Modifies the configuration of a cluster.
+        
+        @description You can modify only the overcommit ratio.
         
         @param request: ModifyDedicatedClusterRequest
         @param runtime: runtime options for this request RuntimeOptions
         @return: ModifyDedicatedClusterResponse
         """
         UtilClient.validate_model(request)
         query = {}
@@ -8463,42 +9611,48 @@
         )
 
     def modify_dedicated_cluster(
         self,
         request: dts_20200101_models.ModifyDedicatedClusterRequest,
     ) -> dts_20200101_models.ModifyDedicatedClusterResponse:
         """
-        You can modify only the overcommit ratio.
+        @summary Modifies the configuration of a cluster.
+        
+        @description You can modify only the overcommit ratio.
         
         @param request: ModifyDedicatedClusterRequest
         @return: ModifyDedicatedClusterResponse
         """
         runtime = util_models.RuntimeOptions()
         return self.modify_dedicated_cluster_with_options(request, runtime)
 
     async def modify_dedicated_cluster_async(
         self,
         request: dts_20200101_models.ModifyDedicatedClusterRequest,
     ) -> dts_20200101_models.ModifyDedicatedClusterResponse:
         """
-        You can modify only the overcommit ratio.
+        @summary Modifies the configuration of a cluster.
+        
+        @description You can modify only the overcommit ratio.
         
         @param request: ModifyDedicatedClusterRequest
         @return: ModifyDedicatedClusterResponse
         """
         runtime = util_models.RuntimeOptions()
         return await self.modify_dedicated_cluster_with_options_async(request, runtime)
 
     def modify_dts_job_with_options(
         self,
         tmp_req: dts_20200101_models.ModifyDtsJobRequest,
         runtime: util_models.RuntimeOptions,
     ) -> dts_20200101_models.ModifyDtsJobResponse:
         """
-        When you configure a data synchronization task in the Data Transmission Service (DTS) console, you can move the pointer over *Next: Save Task Settings and Precheck** in the **Advanced Settings** step and click **Preview OpenAPI parameters** to view the parameters that are used to configure the task by calling an API operation.
+        @summary Modifies the configurations of a data synchronization task.
+        
+        @description When you configure a data synchronization task in the Data Transmission Service (DTS) console, you can move the pointer over *Next: Save Task Settings and Precheck** in the **Advanced Settings** step and click **Preview OpenAPI parameters** to view the parameters that are used to configure the task by calling an API operation.
         
         @param tmp_req: ModifyDtsJobRequest
         @param runtime: runtime options for this request RuntimeOptions
         @return: ModifyDtsJobResponse
         """
         UtilClient.validate_model(tmp_req)
         request = dts_20200101_models.ModifyDtsJobShrinkRequest()
@@ -8561,15 +9715,17 @@
 
     async def modify_dts_job_with_options_async(
         self,
         tmp_req: dts_20200101_models.ModifyDtsJobRequest,
         runtime: util_models.RuntimeOptions,
     ) -> dts_20200101_models.ModifyDtsJobResponse:
         """
-        When you configure a data synchronization task in the Data Transmission Service (DTS) console, you can move the pointer over *Next: Save Task Settings and Precheck** in the **Advanced Settings** step and click **Preview OpenAPI parameters** to view the parameters that are used to configure the task by calling an API operation.
+        @summary Modifies the configurations of a data synchronization task.
+        
+        @description When you configure a data synchronization task in the Data Transmission Service (DTS) console, you can move the pointer over *Next: Save Task Settings and Precheck** in the **Advanced Settings** step and click **Preview OpenAPI parameters** to view the parameters that are used to configure the task by calling an API operation.
         
         @param tmp_req: ModifyDtsJobRequest
         @param runtime: runtime options for this request RuntimeOptions
         @return: ModifyDtsJobResponse
         """
         UtilClient.validate_model(tmp_req)
         request = dts_20200101_models.ModifyDtsJobShrinkRequest()
@@ -8631,28 +9787,32 @@
         )
 
     def modify_dts_job(
         self,
         request: dts_20200101_models.ModifyDtsJobRequest,
     ) -> dts_20200101_models.ModifyDtsJobResponse:
         """
-        When you configure a data synchronization task in the Data Transmission Service (DTS) console, you can move the pointer over *Next: Save Task Settings and Precheck** in the **Advanced Settings** step and click **Preview OpenAPI parameters** to view the parameters that are used to configure the task by calling an API operation.
+        @summary Modifies the configurations of a data synchronization task.
+        
+        @description When you configure a data synchronization task in the Data Transmission Service (DTS) console, you can move the pointer over *Next: Save Task Settings and Precheck** in the **Advanced Settings** step and click **Preview OpenAPI parameters** to view the parameters that are used to configure the task by calling an API operation.
         
         @param request: ModifyDtsJobRequest
         @return: ModifyDtsJobResponse
         """
         runtime = util_models.RuntimeOptions()
         return self.modify_dts_job_with_options(request, runtime)
 
     async def modify_dts_job_async(
         self,
         request: dts_20200101_models.ModifyDtsJobRequest,
     ) -> dts_20200101_models.ModifyDtsJobResponse:
         """
-        When you configure a data synchronization task in the Data Transmission Service (DTS) console, you can move the pointer over *Next: Save Task Settings and Precheck** in the **Advanced Settings** step and click **Preview OpenAPI parameters** to view the parameters that are used to configure the task by calling an API operation.
+        @summary Modifies the configurations of a data synchronization task.
+        
+        @description When you configure a data synchronization task in the Data Transmission Service (DTS) console, you can move the pointer over *Next: Save Task Settings and Precheck** in the **Advanced Settings** step and click **Preview OpenAPI parameters** to view the parameters that are used to configure the task by calling an API operation.
         
         @param request: ModifyDtsJobRequest
         @return: ModifyDtsJobResponse
         """
         runtime = util_models.RuntimeOptions()
         return await self.modify_dts_job_with_options_async(request, runtime)
 
@@ -8663,15 +9823,15 @@
     ) -> dts_20200101_models.ModifyDtsJobResponse:
         # Step 0: init client
         access_key_id = self._credential.get_access_key_id()
         access_key_secret = self._credential.get_access_key_secret()
         security_token = self._credential.get_security_token()
         credential_type = self._credential.get_type()
         open_platform_endpoint = self._open_platform_endpoint
-        if UtilClient.is_unset(open_platform_endpoint):
+        if UtilClient.empty(open_platform_endpoint):
             open_platform_endpoint = 'openplatform.aliyuncs.com'
         if UtilClient.is_unset(credential_type):
             credential_type = 'access_key'
         auth_config = open_api_models.Config(
             access_key_id=access_key_id,
             access_key_secret=access_key_secret,
             security_token=security_token,
@@ -8683,20 +9843,21 @@
         auth_client = OpenPlatformClient(auth_config)
         auth_request = open_platform_models.AuthorizeFileUploadRequest(
             product='Dts',
             region_id=self._region_id
         )
         auth_response = open_platform_models.AuthorizeFileUploadResponse()
         oss_config = oss_models.Config(
+            access_key_id=access_key_id,
             access_key_secret=access_key_secret,
             type='access_key',
             protocol=self._protocol,
             region_id=self._region_id
         )
-        oss_client = None
+        oss_client = OSSClient(oss_config)
         file_obj = file_form_models.FileField()
         oss_header = oss_models.PostObjectRequestHeader()
         upload_request = oss_models.PostObjectRequest()
         oss_runtime = ossutil_models.RuntimeOptions()
         OpenApiUtilClient.convert(runtime, oss_runtime)
         modify_dts_job_req = dts_20200101_models.ModifyDtsJobRequest()
         OpenApiUtilClient.convert(request, modify_dts_job_req)
@@ -8734,15 +9895,15 @@
     ) -> dts_20200101_models.ModifyDtsJobResponse:
         # Step 0: init client
         access_key_id = await self._credential.get_access_key_id_async()
         access_key_secret = await self._credential.get_access_key_secret_async()
         security_token = await self._credential.get_security_token_async()
         credential_type = self._credential.get_type()
         open_platform_endpoint = self._open_platform_endpoint
-        if UtilClient.is_unset(open_platform_endpoint):
+        if UtilClient.empty(open_platform_endpoint):
             open_platform_endpoint = 'openplatform.aliyuncs.com'
         if UtilClient.is_unset(credential_type):
             credential_type = 'access_key'
         auth_config = open_api_models.Config(
             access_key_id=access_key_id,
             access_key_secret=access_key_secret,
             security_token=security_token,
@@ -8754,20 +9915,21 @@
         auth_client = OpenPlatformClient(auth_config)
         auth_request = open_platform_models.AuthorizeFileUploadRequest(
             product='Dts',
             region_id=self._region_id
         )
         auth_response = open_platform_models.AuthorizeFileUploadResponse()
         oss_config = oss_models.Config(
+            access_key_id=access_key_id,
             access_key_secret=access_key_secret,
             type='access_key',
             protocol=self._protocol,
             region_id=self._region_id
         )
-        oss_client = None
+        oss_client = OSSClient(oss_config)
         file_obj = file_form_models.FileField()
         oss_header = oss_models.PostObjectRequestHeader()
         upload_request = oss_models.PostObjectRequest()
         oss_runtime = ossutil_models.RuntimeOptions()
         OpenApiUtilClient.convert(runtime, oss_runtime)
         modify_dts_job_req = dts_20200101_models.ModifyDtsJobRequest()
         OpenApiUtilClient.convert(request, modify_dts_job_req)
@@ -8799,14 +9961,21 @@
         return modify_dts_job_resp
 
     def modify_dts_job_config_with_options(
         self,
         request: dts_20200101_models.ModifyDtsJobConfigRequest,
         runtime: util_models.RuntimeOptions,
     ) -> dts_20200101_models.ModifyDtsJobConfigResponse:
+        """
+        @summary 修改DTS任务配置
+        
+        @param request: ModifyDtsJobConfigRequest
+        @param runtime: runtime options for this request RuntimeOptions
+        @return: ModifyDtsJobConfigResponse
+        """
         UtilClient.validate_model(request)
         query = {}
         if not UtilClient.is_unset(request.dts_job_id):
             query['DtsJobId'] = request.dts_job_id
         if not UtilClient.is_unset(request.owner_id):
             query['OwnerId'] = request.owner_id
         if not UtilClient.is_unset(request.parameters):
@@ -8835,14 +10004,21 @@
         )
 
     async def modify_dts_job_config_with_options_async(
         self,
         request: dts_20200101_models.ModifyDtsJobConfigRequest,
         runtime: util_models.RuntimeOptions,
     ) -> dts_20200101_models.ModifyDtsJobConfigResponse:
+        """
+        @summary 修改DTS任务配置
+        
+        @param request: ModifyDtsJobConfigRequest
+        @param runtime: runtime options for this request RuntimeOptions
+        @return: ModifyDtsJobConfigResponse
+        """
         UtilClient.validate_model(request)
         query = {}
         if not UtilClient.is_unset(request.dts_job_id):
             query['DtsJobId'] = request.dts_job_id
         if not UtilClient.is_unset(request.owner_id):
             query['OwnerId'] = request.owner_id
         if not UtilClient.is_unset(request.parameters):
@@ -8870,29 +10046,48 @@
             await self.call_api_async(params, req, runtime)
         )
 
     def modify_dts_job_config(
         self,
         request: dts_20200101_models.ModifyDtsJobConfigRequest,
     ) -> dts_20200101_models.ModifyDtsJobConfigResponse:
+        """
+        @summary 修改DTS任务配置
+        
+        @param request: ModifyDtsJobConfigRequest
+        @return: ModifyDtsJobConfigResponse
+        """
         runtime = util_models.RuntimeOptions()
         return self.modify_dts_job_config_with_options(request, runtime)
 
     async def modify_dts_job_config_async(
         self,
         request: dts_20200101_models.ModifyDtsJobConfigRequest,
     ) -> dts_20200101_models.ModifyDtsJobConfigResponse:
+        """
+        @summary 修改DTS任务配置
+        
+        @param request: ModifyDtsJobConfigRequest
+        @return: ModifyDtsJobConfigResponse
+        """
         runtime = util_models.RuntimeOptions()
         return await self.modify_dts_job_config_with_options_async(request, runtime)
 
     def modify_dts_job_dedicated_cluster_with_options(
         self,
         request: dts_20200101_models.ModifyDtsJobDedicatedClusterRequest,
         runtime: util_models.RuntimeOptions,
     ) -> dts_20200101_models.ModifyDtsJobDedicatedClusterResponse:
+        """
+        @summary 迁移专属集群任务
+        
+        @param request: ModifyDtsJobDedicatedClusterRequest
+        @param runtime: runtime options for this request RuntimeOptions
+        @return: ModifyDtsJobDedicatedClusterResponse
+        """
         UtilClient.validate_model(request)
         query = {}
         if not UtilClient.is_unset(request.dedicated_cluster_id):
             query['DedicatedClusterId'] = request.dedicated_cluster_id
         if not UtilClient.is_unset(request.dts_job_ids):
             query['DtsJobIds'] = request.dts_job_ids
         if not UtilClient.is_unset(request.owner_id):
@@ -8921,14 +10116,21 @@
         )
 
     async def modify_dts_job_dedicated_cluster_with_options_async(
         self,
         request: dts_20200101_models.ModifyDtsJobDedicatedClusterRequest,
         runtime: util_models.RuntimeOptions,
     ) -> dts_20200101_models.ModifyDtsJobDedicatedClusterResponse:
+        """
+        @summary 迁移专属集群任务
+        
+        @param request: ModifyDtsJobDedicatedClusterRequest
+        @param runtime: runtime options for this request RuntimeOptions
+        @return: ModifyDtsJobDedicatedClusterResponse
+        """
         UtilClient.validate_model(request)
         query = {}
         if not UtilClient.is_unset(request.dedicated_cluster_id):
             query['DedicatedClusterId'] = request.dedicated_cluster_id
         if not UtilClient.is_unset(request.dts_job_ids):
             query['DtsJobIds'] = request.dts_job_ids
         if not UtilClient.is_unset(request.owner_id):
@@ -8956,32 +10158,46 @@
             await self.call_api_async(params, req, runtime)
         )
 
     def modify_dts_job_dedicated_cluster(
         self,
         request: dts_20200101_models.ModifyDtsJobDedicatedClusterRequest,
     ) -> dts_20200101_models.ModifyDtsJobDedicatedClusterResponse:
+        """
+        @summary 迁移专属集群任务
+        
+        @param request: ModifyDtsJobDedicatedClusterRequest
+        @return: ModifyDtsJobDedicatedClusterResponse
+        """
         runtime = util_models.RuntimeOptions()
         return self.modify_dts_job_dedicated_cluster_with_options(request, runtime)
 
     async def modify_dts_job_dedicated_cluster_async(
         self,
         request: dts_20200101_models.ModifyDtsJobDedicatedClusterRequest,
     ) -> dts_20200101_models.ModifyDtsJobDedicatedClusterResponse:
+        """
+        @summary 迁移专属集群任务
+        
+        @param request: ModifyDtsJobDedicatedClusterRequest
+        @return: ModifyDtsJobDedicatedClusterResponse
+        """
         runtime = util_models.RuntimeOptions()
         return await self.modify_dts_job_dedicated_cluster_with_options_async(request, runtime)
 
     def modify_dts_job_du_limit_with_options(
         self,
         request: dts_20200101_models.ModifyDtsJobDuLimitRequest,
         runtime: util_models.RuntimeOptions,
     ) -> dts_20200101_models.ModifyDtsJobDuLimitResponse:
         """
-        DTS allows you to upgrade or downgrade the configurations of DTS instances in a dedicated cluster. You can adjust the resources that are occupied for task execution to dynamically adjust the number of tasks that can be scheduled in the cluster. This way, you can reduce the total number of DUs required for the cluster or release DUs.
-        *   Before you modify the upper limit of DUs for a DTS task, make sure that sufficient DUs are available.
+        @summary Modifies the upper limit of DTS units (DUs) for a Data Transmission Service (DTS) task.
+        
+        @description    DTS allows you to upgrade or downgrade the configurations of DTS instances in a dedicated cluster. You can adjust the resources that are occupied for task execution to dynamically adjust the number of tasks that can be scheduled in the cluster. This way, you can reduce the total number of DUs required for the cluster or release DUs.
+        Before you modify the upper limit of DUs for a DTS task, make sure that sufficient DUs are available.
         
         @param request: ModifyDtsJobDuLimitRequest
         @param runtime: runtime options for this request RuntimeOptions
         @return: ModifyDtsJobDuLimitResponse
         """
         UtilClient.validate_model(request)
         query = {}
@@ -9016,16 +10232,18 @@
 
     async def modify_dts_job_du_limit_with_options_async(
         self,
         request: dts_20200101_models.ModifyDtsJobDuLimitRequest,
         runtime: util_models.RuntimeOptions,
     ) -> dts_20200101_models.ModifyDtsJobDuLimitResponse:
         """
-        DTS allows you to upgrade or downgrade the configurations of DTS instances in a dedicated cluster. You can adjust the resources that are occupied for task execution to dynamically adjust the number of tasks that can be scheduled in the cluster. This way, you can reduce the total number of DUs required for the cluster or release DUs.
-        *   Before you modify the upper limit of DUs for a DTS task, make sure that sufficient DUs are available.
+        @summary Modifies the upper limit of DTS units (DUs) for a Data Transmission Service (DTS) task.
+        
+        @description    DTS allows you to upgrade or downgrade the configurations of DTS instances in a dedicated cluster. You can adjust the resources that are occupied for task execution to dynamically adjust the number of tasks that can be scheduled in the cluster. This way, you can reduce the total number of DUs required for the cluster or release DUs.
+        Before you modify the upper limit of DUs for a DTS task, make sure that sufficient DUs are available.
         
         @param request: ModifyDtsJobDuLimitRequest
         @param runtime: runtime options for this request RuntimeOptions
         @return: ModifyDtsJobDuLimitResponse
         """
         UtilClient.validate_model(request)
         query = {}
@@ -9059,42 +10277,53 @@
         )
 
     def modify_dts_job_du_limit(
         self,
         request: dts_20200101_models.ModifyDtsJobDuLimitRequest,
     ) -> dts_20200101_models.ModifyDtsJobDuLimitResponse:
         """
-        DTS allows you to upgrade or downgrade the configurations of DTS instances in a dedicated cluster. You can adjust the resources that are occupied for task execution to dynamically adjust the number of tasks that can be scheduled in the cluster. This way, you can reduce the total number of DUs required for the cluster or release DUs.
-        *   Before you modify the upper limit of DUs for a DTS task, make sure that sufficient DUs are available.
+        @summary Modifies the upper limit of DTS units (DUs) for a Data Transmission Service (DTS) task.
+        
+        @description    DTS allows you to upgrade or downgrade the configurations of DTS instances in a dedicated cluster. You can adjust the resources that are occupied for task execution to dynamically adjust the number of tasks that can be scheduled in the cluster. This way, you can reduce the total number of DUs required for the cluster or release DUs.
+        Before you modify the upper limit of DUs for a DTS task, make sure that sufficient DUs are available.
         
         @param request: ModifyDtsJobDuLimitRequest
         @return: ModifyDtsJobDuLimitResponse
         """
         runtime = util_models.RuntimeOptions()
         return self.modify_dts_job_du_limit_with_options(request, runtime)
 
     async def modify_dts_job_du_limit_async(
         self,
         request: dts_20200101_models.ModifyDtsJobDuLimitRequest,
     ) -> dts_20200101_models.ModifyDtsJobDuLimitResponse:
         """
-        DTS allows you to upgrade or downgrade the configurations of DTS instances in a dedicated cluster. You can adjust the resources that are occupied for task execution to dynamically adjust the number of tasks that can be scheduled in the cluster. This way, you can reduce the total number of DUs required for the cluster or release DUs.
-        *   Before you modify the upper limit of DUs for a DTS task, make sure that sufficient DUs are available.
+        @summary Modifies the upper limit of DTS units (DUs) for a Data Transmission Service (DTS) task.
+        
+        @description    DTS allows you to upgrade or downgrade the configurations of DTS instances in a dedicated cluster. You can adjust the resources that are occupied for task execution to dynamically adjust the number of tasks that can be scheduled in the cluster. This way, you can reduce the total number of DUs required for the cluster or release DUs.
+        Before you modify the upper limit of DUs for a DTS task, make sure that sufficient DUs are available.
         
         @param request: ModifyDtsJobDuLimitRequest
         @return: ModifyDtsJobDuLimitResponse
         """
         runtime = util_models.RuntimeOptions()
         return await self.modify_dts_job_du_limit_with_options_async(request, runtime)
 
     def modify_dts_job_endpoint_with_options(
         self,
         request: dts_20200101_models.ModifyDtsJobEndpointRequest,
         runtime: util_models.RuntimeOptions,
     ) -> dts_20200101_models.ModifyDtsJobEndpointResponse:
+        """
+        @summary 替换源端或目标端实例
+        
+        @param request: ModifyDtsJobEndpointRequest
+        @param runtime: runtime options for this request RuntimeOptions
+        @return: ModifyDtsJobEndpointResponse
+        """
         UtilClient.validate_model(request)
         query = {}
         if not UtilClient.is_unset(request.aliyun_uid):
             query['AliyunUid'] = request.aliyun_uid
         if not UtilClient.is_unset(request.database):
             query['Database'] = request.database
         if not UtilClient.is_unset(request.dry_run):
@@ -9153,14 +10382,21 @@
         )
 
     async def modify_dts_job_endpoint_with_options_async(
         self,
         request: dts_20200101_models.ModifyDtsJobEndpointRequest,
         runtime: util_models.RuntimeOptions,
     ) -> dts_20200101_models.ModifyDtsJobEndpointResponse:
+        """
+        @summary 替换源端或目标端实例
+        
+        @param request: ModifyDtsJobEndpointRequest
+        @param runtime: runtime options for this request RuntimeOptions
+        @return: ModifyDtsJobEndpointResponse
+        """
         UtilClient.validate_model(request)
         query = {}
         if not UtilClient.is_unset(request.aliyun_uid):
             query['AliyunUid'] = request.aliyun_uid
         if not UtilClient.is_unset(request.database):
             query['Database'] = request.database
         if not UtilClient.is_unset(request.dry_run):
@@ -9218,29 +10454,46 @@
             await self.call_api_async(params, req, runtime)
         )
 
     def modify_dts_job_endpoint(
         self,
         request: dts_20200101_models.ModifyDtsJobEndpointRequest,
     ) -> dts_20200101_models.ModifyDtsJobEndpointResponse:
+        """
+        @summary 替换源端或目标端实例
+        
+        @param request: ModifyDtsJobEndpointRequest
+        @return: ModifyDtsJobEndpointResponse
+        """
         runtime = util_models.RuntimeOptions()
         return self.modify_dts_job_endpoint_with_options(request, runtime)
 
     async def modify_dts_job_endpoint_async(
         self,
         request: dts_20200101_models.ModifyDtsJobEndpointRequest,
     ) -> dts_20200101_models.ModifyDtsJobEndpointResponse:
+        """
+        @summary 替换源端或目标端实例
+        
+        @param request: ModifyDtsJobEndpointRequest
+        @return: ModifyDtsJobEndpointResponse
+        """
         runtime = util_models.RuntimeOptions()
         return await self.modify_dts_job_endpoint_with_options_async(request, runtime)
 
     def modify_dts_job_name_with_options(
         self,
         request: dts_20200101_models.ModifyDtsJobNameRequest,
         runtime: util_models.RuntimeOptions,
     ) -> dts_20200101_models.ModifyDtsJobNameResponse:
+        """
+        @param request: ModifyDtsJobNameRequest
+        @param runtime: runtime options for this request RuntimeOptions
+        @return: ModifyDtsJobNameResponse
+        """
         UtilClient.validate_model(request)
         query = {}
         if not UtilClient.is_unset(request.dts_job_id):
             query['DtsJobId'] = request.dts_job_id
         if not UtilClient.is_unset(request.dts_job_name):
             query['DtsJobName'] = request.dts_job_name
         if not UtilClient.is_unset(request.region_id):
@@ -9269,14 +10522,19 @@
         )
 
     async def modify_dts_job_name_with_options_async(
         self,
         request: dts_20200101_models.ModifyDtsJobNameRequest,
         runtime: util_models.RuntimeOptions,
     ) -> dts_20200101_models.ModifyDtsJobNameResponse:
+        """
+        @param request: ModifyDtsJobNameRequest
+        @param runtime: runtime options for this request RuntimeOptions
+        @return: ModifyDtsJobNameResponse
+        """
         UtilClient.validate_model(request)
         query = {}
         if not UtilClient.is_unset(request.dts_job_id):
             query['DtsJobId'] = request.dts_job_id
         if not UtilClient.is_unset(request.dts_job_name):
             query['DtsJobName'] = request.dts_job_name
         if not UtilClient.is_unset(request.region_id):
@@ -9304,29 +10562,42 @@
             await self.call_api_async(params, req, runtime)
         )
 
     def modify_dts_job_name(
         self,
         request: dts_20200101_models.ModifyDtsJobNameRequest,
     ) -> dts_20200101_models.ModifyDtsJobNameResponse:
+        """
+        @param request: ModifyDtsJobNameRequest
+        @return: ModifyDtsJobNameResponse
+        """
         runtime = util_models.RuntimeOptions()
         return self.modify_dts_job_name_with_options(request, runtime)
 
     async def modify_dts_job_name_async(
         self,
         request: dts_20200101_models.ModifyDtsJobNameRequest,
     ) -> dts_20200101_models.ModifyDtsJobNameResponse:
+        """
+        @param request: ModifyDtsJobNameRequest
+        @return: ModifyDtsJobNameResponse
+        """
         runtime = util_models.RuntimeOptions()
         return await self.modify_dts_job_name_with_options_async(request, runtime)
 
     def modify_dts_job_password_with_options(
         self,
         request: dts_20200101_models.ModifyDtsJobPasswordRequest,
         runtime: util_models.RuntimeOptions,
     ) -> dts_20200101_models.ModifyDtsJobPasswordResponse:
+        """
+        @param request: ModifyDtsJobPasswordRequest
+        @param runtime: runtime options for this request RuntimeOptions
+        @return: ModifyDtsJobPasswordResponse
+        """
         UtilClient.validate_model(request)
         query = {}
         if not UtilClient.is_unset(request.dts_job_id):
             query['DtsJobId'] = request.dts_job_id
         if not UtilClient.is_unset(request.endpoint):
             query['Endpoint'] = request.endpoint
         if not UtilClient.is_unset(request.password):
@@ -9359,14 +10630,19 @@
         )
 
     async def modify_dts_job_password_with_options_async(
         self,
         request: dts_20200101_models.ModifyDtsJobPasswordRequest,
         runtime: util_models.RuntimeOptions,
     ) -> dts_20200101_models.ModifyDtsJobPasswordResponse:
+        """
+        @param request: ModifyDtsJobPasswordRequest
+        @param runtime: runtime options for this request RuntimeOptions
+        @return: ModifyDtsJobPasswordResponse
+        """
         UtilClient.validate_model(request)
         query = {}
         if not UtilClient.is_unset(request.dts_job_id):
             query['DtsJobId'] = request.dts_job_id
         if not UtilClient.is_unset(request.endpoint):
             query['Endpoint'] = request.endpoint
         if not UtilClient.is_unset(request.password):
@@ -9398,29 +10674,42 @@
             await self.call_api_async(params, req, runtime)
         )
 
     def modify_dts_job_password(
         self,
         request: dts_20200101_models.ModifyDtsJobPasswordRequest,
     ) -> dts_20200101_models.ModifyDtsJobPasswordResponse:
+        """
+        @param request: ModifyDtsJobPasswordRequest
+        @return: ModifyDtsJobPasswordResponse
+        """
         runtime = util_models.RuntimeOptions()
         return self.modify_dts_job_password_with_options(request, runtime)
 
     async def modify_dts_job_password_async(
         self,
         request: dts_20200101_models.ModifyDtsJobPasswordRequest,
     ) -> dts_20200101_models.ModifyDtsJobPasswordResponse:
+        """
+        @param request: ModifyDtsJobPasswordRequest
+        @return: ModifyDtsJobPasswordResponse
+        """
         runtime = util_models.RuntimeOptions()
         return await self.modify_dts_job_password_with_options_async(request, runtime)
 
     def modify_dynamic_config_with_options(
         self,
         request: dts_20200101_models.ModifyDynamicConfigRequest,
         runtime: util_models.RuntimeOptions,
     ) -> dts_20200101_models.ModifyDynamicConfigResponse:
+        """
+        @param request: ModifyDynamicConfigRequest
+        @param runtime: runtime options for this request RuntimeOptions
+        @return: ModifyDynamicConfigResponse
+        """
         UtilClient.validate_model(request)
         query = {}
         if not UtilClient.is_unset(request.config_list):
             query['ConfigList'] = request.config_list
         if not UtilClient.is_unset(request.dts_job_id):
             query['DtsJobId'] = request.dts_job_id
         if not UtilClient.is_unset(request.enable_limit):
@@ -9451,14 +10740,19 @@
         )
 
     async def modify_dynamic_config_with_options_async(
         self,
         request: dts_20200101_models.ModifyDynamicConfigRequest,
         runtime: util_models.RuntimeOptions,
     ) -> dts_20200101_models.ModifyDynamicConfigResponse:
+        """
+        @param request: ModifyDynamicConfigRequest
+        @param runtime: runtime options for this request RuntimeOptions
+        @return: ModifyDynamicConfigResponse
+        """
         UtilClient.validate_model(request)
         query = {}
         if not UtilClient.is_unset(request.config_list):
             query['ConfigList'] = request.config_list
         if not UtilClient.is_unset(request.dts_job_id):
             query['DtsJobId'] = request.dts_job_id
         if not UtilClient.is_unset(request.enable_limit):
@@ -9488,29 +10782,42 @@
             await self.call_api_async(params, req, runtime)
         )
 
     def modify_dynamic_config(
         self,
         request: dts_20200101_models.ModifyDynamicConfigRequest,
     ) -> dts_20200101_models.ModifyDynamicConfigResponse:
+        """
+        @param request: ModifyDynamicConfigRequest
+        @return: ModifyDynamicConfigResponse
+        """
         runtime = util_models.RuntimeOptions()
         return self.modify_dynamic_config_with_options(request, runtime)
 
     async def modify_dynamic_config_async(
         self,
         request: dts_20200101_models.ModifyDynamicConfigRequest,
     ) -> dts_20200101_models.ModifyDynamicConfigResponse:
+        """
+        @param request: ModifyDynamicConfigRequest
+        @return: ModifyDynamicConfigResponse
+        """
         runtime = util_models.RuntimeOptions()
         return await self.modify_dynamic_config_with_options_async(request, runtime)
 
     def modify_subscription_with_options(
         self,
         request: dts_20200101_models.ModifySubscriptionRequest,
         runtime: util_models.RuntimeOptions,
     ) -> dts_20200101_models.ModifySubscriptionResponse:
+        """
+        @param request: ModifySubscriptionRequest
+        @param runtime: runtime options for this request RuntimeOptions
+        @return: ModifySubscriptionResponse
+        """
         UtilClient.validate_model(request)
         query = {}
         if not UtilClient.is_unset(request.db_list):
             query['DbList'] = request.db_list
         if not UtilClient.is_unset(request.dts_instance_id):
             query['DtsInstanceId'] = request.dts_instance_id
         if not UtilClient.is_unset(request.dts_job_id):
@@ -9543,14 +10850,19 @@
         )
 
     async def modify_subscription_with_options_async(
         self,
         request: dts_20200101_models.ModifySubscriptionRequest,
         runtime: util_models.RuntimeOptions,
     ) -> dts_20200101_models.ModifySubscriptionResponse:
+        """
+        @param request: ModifySubscriptionRequest
+        @param runtime: runtime options for this request RuntimeOptions
+        @return: ModifySubscriptionResponse
+        """
         UtilClient.validate_model(request)
         query = {}
         if not UtilClient.is_unset(request.db_list):
             query['DbList'] = request.db_list
         if not UtilClient.is_unset(request.dts_instance_id):
             query['DtsInstanceId'] = request.dts_instance_id
         if not UtilClient.is_unset(request.dts_job_id):
@@ -9582,34 +10894,42 @@
             await self.call_api_async(params, req, runtime)
         )
 
     def modify_subscription(
         self,
         request: dts_20200101_models.ModifySubscriptionRequest,
     ) -> dts_20200101_models.ModifySubscriptionResponse:
+        """
+        @param request: ModifySubscriptionRequest
+        @return: ModifySubscriptionResponse
+        """
         runtime = util_models.RuntimeOptions()
         return self.modify_subscription_with_options(request, runtime)
 
     async def modify_subscription_async(
         self,
         request: dts_20200101_models.ModifySubscriptionRequest,
     ) -> dts_20200101_models.ModifySubscriptionResponse:
+        """
+        @param request: ModifySubscriptionRequest
+        @return: ModifySubscriptionResponse
+        """
         runtime = util_models.RuntimeOptions()
         return await self.modify_subscription_with_options_async(request, runtime)
 
     def modify_subscription_object_with_options(
         self,
         request: dts_20200101_models.ModifySubscriptionObjectRequest,
         runtime: util_models.RuntimeOptions,
     ) -> dts_20200101_models.ModifySubscriptionObjectResponse:
         """
-        When you call this operation, the change tracking task must be in the Normal, NotStarted, or Failed state.
+        @description When you call this operation, the change tracking task must be in the Normal, NotStarted, or Failed state.
         >
-        *   If you call this operation to modify the objects of a change tracking task that is in the Normal state, DTS automatically calls the [StartSubscriptionInstance](~~49438~~) to restart the task.
-        *   If you call this operation to modify the objects of a change tracking task that is in the NotStarted or Failed state, DTS does not automatically start the task. You must call the [StartSubscriptionInstance](~~49438~~) to restart the task.
+        If you call this operation to modify the objects of a change tracking task that is in the Normal state, DTS automatically calls the [StartSubscriptionInstance](https://help.aliyun.com/document_detail/49438.html) to restart the task.
+        If you call this operation to modify the objects of a change tracking task that is in the NotStarted or Failed state, DTS does not automatically start the task. You must call the [StartSubscriptionInstance](https://help.aliyun.com/document_detail/49438.html) to restart the task.
         
         @param request: ModifySubscriptionObjectRequest
         @param runtime: runtime options for this request RuntimeOptions
         @return: ModifySubscriptionObjectResponse
         """
         UtilClient.validate_model(request)
         query = {}
@@ -9646,18 +10966,18 @@
 
     async def modify_subscription_object_with_options_async(
         self,
         request: dts_20200101_models.ModifySubscriptionObjectRequest,
         runtime: util_models.RuntimeOptions,
     ) -> dts_20200101_models.ModifySubscriptionObjectResponse:
         """
-        When you call this operation, the change tracking task must be in the Normal, NotStarted, or Failed state.
+        @description When you call this operation, the change tracking task must be in the Normal, NotStarted, or Failed state.
         >
-        *   If you call this operation to modify the objects of a change tracking task that is in the Normal state, DTS automatically calls the [StartSubscriptionInstance](~~49438~~) to restart the task.
-        *   If you call this operation to modify the objects of a change tracking task that is in the NotStarted or Failed state, DTS does not automatically start the task. You must call the [StartSubscriptionInstance](~~49438~~) to restart the task.
+        If you call this operation to modify the objects of a change tracking task that is in the Normal state, DTS automatically calls the [StartSubscriptionInstance](https://help.aliyun.com/document_detail/49438.html) to restart the task.
+        If you call this operation to modify the objects of a change tracking task that is in the NotStarted or Failed state, DTS does not automatically start the task. You must call the [StartSubscriptionInstance](https://help.aliyun.com/document_detail/49438.html) to restart the task.
         
         @param request: ModifySubscriptionObjectRequest
         @param runtime: runtime options for this request RuntimeOptions
         @return: ModifySubscriptionObjectResponse
         """
         UtilClient.validate_model(request)
         query = {}
@@ -9693,48 +11013,48 @@
         )
 
     def modify_subscription_object(
         self,
         request: dts_20200101_models.ModifySubscriptionObjectRequest,
     ) -> dts_20200101_models.ModifySubscriptionObjectResponse:
         """
-        When you call this operation, the change tracking task must be in the Normal, NotStarted, or Failed state.
+        @description When you call this operation, the change tracking task must be in the Normal, NotStarted, or Failed state.
         >
-        *   If you call this operation to modify the objects of a change tracking task that is in the Normal state, DTS automatically calls the [StartSubscriptionInstance](~~49438~~) to restart the task.
-        *   If you call this operation to modify the objects of a change tracking task that is in the NotStarted or Failed state, DTS does not automatically start the task. You must call the [StartSubscriptionInstance](~~49438~~) to restart the task.
+        If you call this operation to modify the objects of a change tracking task that is in the Normal state, DTS automatically calls the [StartSubscriptionInstance](https://help.aliyun.com/document_detail/49438.html) to restart the task.
+        If you call this operation to modify the objects of a change tracking task that is in the NotStarted or Failed state, DTS does not automatically start the task. You must call the [StartSubscriptionInstance](https://help.aliyun.com/document_detail/49438.html) to restart the task.
         
         @param request: ModifySubscriptionObjectRequest
         @return: ModifySubscriptionObjectResponse
         """
         runtime = util_models.RuntimeOptions()
         return self.modify_subscription_object_with_options(request, runtime)
 
     async def modify_subscription_object_async(
         self,
         request: dts_20200101_models.ModifySubscriptionObjectRequest,
     ) -> dts_20200101_models.ModifySubscriptionObjectResponse:
         """
-        When you call this operation, the change tracking task must be in the Normal, NotStarted, or Failed state.
+        @description When you call this operation, the change tracking task must be in the Normal, NotStarted, or Failed state.
         >
-        *   If you call this operation to modify the objects of a change tracking task that is in the Normal state, DTS automatically calls the [StartSubscriptionInstance](~~49438~~) to restart the task.
-        *   If you call this operation to modify the objects of a change tracking task that is in the NotStarted or Failed state, DTS does not automatically start the task. You must call the [StartSubscriptionInstance](~~49438~~) to restart the task.
+        If you call this operation to modify the objects of a change tracking task that is in the Normal state, DTS automatically calls the [StartSubscriptionInstance](https://help.aliyun.com/document_detail/49438.html) to restart the task.
+        If you call this operation to modify the objects of a change tracking task that is in the NotStarted or Failed state, DTS does not automatically start the task. You must call the [StartSubscriptionInstance](https://help.aliyun.com/document_detail/49438.html) to restart the task.
         
         @param request: ModifySubscriptionObjectRequest
         @return: ModifySubscriptionObjectResponse
         """
         runtime = util_models.RuntimeOptions()
         return await self.modify_subscription_object_with_options_async(request, runtime)
 
     def modify_synchronization_object_with_options(
         self,
         request: dts_20200101_models.ModifySynchronizationObjectRequest,
         runtime: util_models.RuntimeOptions,
     ) -> dts_20200101_models.ModifySynchronizationObjectResponse:
         """
-        >  When you call this operation, the data synchronization task must be in the Not Started or Synchronizing state.
+        @description >  When you call this operation, the data synchronization task must be in the Not Started or Synchronizing state.
         
         @param request: ModifySynchronizationObjectRequest
         @param runtime: runtime options for this request RuntimeOptions
         @return: ModifySynchronizationObjectResponse
         """
         UtilClient.validate_model(request)
         query = {}
@@ -9775,15 +11095,15 @@
 
     async def modify_synchronization_object_with_options_async(
         self,
         request: dts_20200101_models.ModifySynchronizationObjectRequest,
         runtime: util_models.RuntimeOptions,
     ) -> dts_20200101_models.ModifySynchronizationObjectResponse:
         """
-        >  When you call this operation, the data synchronization task must be in the Not Started or Synchronizing state.
+        @description >  When you call this operation, the data synchronization task must be in the Not Started or Synchronizing state.
         
         @param request: ModifySynchronizationObjectRequest
         @param runtime: runtime options for this request RuntimeOptions
         @return: ModifySynchronizationObjectResponse
         """
         UtilClient.validate_model(request)
         query = {}
@@ -9823,40 +11143,45 @@
         )
 
     def modify_synchronization_object(
         self,
         request: dts_20200101_models.ModifySynchronizationObjectRequest,
     ) -> dts_20200101_models.ModifySynchronizationObjectResponse:
         """
-        >  When you call this operation, the data synchronization task must be in the Not Started or Synchronizing state.
+        @description >  When you call this operation, the data synchronization task must be in the Not Started or Synchronizing state.
         
         @param request: ModifySynchronizationObjectRequest
         @return: ModifySynchronizationObjectResponse
         """
         runtime = util_models.RuntimeOptions()
         return self.modify_synchronization_object_with_options(request, runtime)
 
     async def modify_synchronization_object_async(
         self,
         request: dts_20200101_models.ModifySynchronizationObjectRequest,
     ) -> dts_20200101_models.ModifySynchronizationObjectResponse:
         """
-        >  When you call this operation, the data synchronization task must be in the Not Started or Synchronizing state.
+        @description >  When you call this operation, the data synchronization task must be in the Not Started or Synchronizing state.
         
         @param request: ModifySynchronizationObjectRequest
         @return: ModifySynchronizationObjectResponse
         """
         runtime = util_models.RuntimeOptions()
         return await self.modify_synchronization_object_with_options_async(request, runtime)
 
     def renew_instance_with_options(
         self,
         request: dts_20200101_models.RenewInstanceRequest,
         runtime: util_models.RuntimeOptions,
     ) -> dts_20200101_models.RenewInstanceResponse:
+        """
+        @param request: RenewInstanceRequest
+        @param runtime: runtime options for this request RuntimeOptions
+        @return: RenewInstanceResponse
+        """
         UtilClient.validate_model(request)
         query = {}
         if not UtilClient.is_unset(request.buy_count):
             query['BuyCount'] = request.buy_count
         if not UtilClient.is_unset(request.charge_type):
             query['ChargeType'] = request.charge_type
         if not UtilClient.is_unset(request.dts_job_id):
@@ -9887,14 +11212,19 @@
         )
 
     async def renew_instance_with_options_async(
         self,
         request: dts_20200101_models.RenewInstanceRequest,
         runtime: util_models.RuntimeOptions,
     ) -> dts_20200101_models.RenewInstanceResponse:
+        """
+        @param request: RenewInstanceRequest
+        @param runtime: runtime options for this request RuntimeOptions
+        @return: RenewInstanceResponse
+        """
         UtilClient.validate_model(request)
         query = {}
         if not UtilClient.is_unset(request.buy_count):
             query['BuyCount'] = request.buy_count
         if not UtilClient.is_unset(request.charge_type):
             query['ChargeType'] = request.charge_type
         if not UtilClient.is_unset(request.dts_job_id):
@@ -9924,31 +11254,39 @@
             await self.call_api_async(params, req, runtime)
         )
 
     def renew_instance(
         self,
         request: dts_20200101_models.RenewInstanceRequest,
     ) -> dts_20200101_models.RenewInstanceResponse:
+        """
+        @param request: RenewInstanceRequest
+        @return: RenewInstanceResponse
+        """
         runtime = util_models.RuntimeOptions()
         return self.renew_instance_with_options(request, runtime)
 
     async def renew_instance_async(
         self,
         request: dts_20200101_models.RenewInstanceRequest,
     ) -> dts_20200101_models.RenewInstanceResponse:
+        """
+        @param request: RenewInstanceRequest
+        @return: RenewInstanceResponse
+        """
         runtime = util_models.RuntimeOptions()
         return await self.renew_instance_with_options_async(request, runtime)
 
     def reset_dts_job_with_options(
         self,
         request: dts_20200101_models.ResetDtsJobRequest,
         runtime: util_models.RuntimeOptions,
     ) -> dts_20200101_models.ResetDtsJobResponse:
         """
-        >  If you clear the configurations of a data synchronization or change tracking task, DTS deletes the task. Then, DTS creates another task. The task is in the Not Configured state. You must call the [ConfigureDtsJob](~~208399~~) operation reconfigure the task.
+        @description >  If you clear the configurations of a data synchronization or change tracking task, DTS deletes the task. Then, DTS creates another task. The task is in the Not Configured state. You must call the [ConfigureDtsJob](https://help.aliyun.com/document_detail/208399.html) operation reconfigure the task.
         
         @param request: ResetDtsJobRequest
         @param runtime: runtime options for this request RuntimeOptions
         @return: ResetDtsJobResponse
         """
         UtilClient.validate_model(request)
         query = {}
@@ -9983,15 +11321,15 @@
 
     async def reset_dts_job_with_options_async(
         self,
         request: dts_20200101_models.ResetDtsJobRequest,
         runtime: util_models.RuntimeOptions,
     ) -> dts_20200101_models.ResetDtsJobResponse:
         """
-        >  If you clear the configurations of a data synchronization or change tracking task, DTS deletes the task. Then, DTS creates another task. The task is in the Not Configured state. You must call the [ConfigureDtsJob](~~208399~~) operation reconfigure the task.
+        @description >  If you clear the configurations of a data synchronization or change tracking task, DTS deletes the task. Then, DTS creates another task. The task is in the Not Configured state. You must call the [ConfigureDtsJob](https://help.aliyun.com/document_detail/208399.html) operation reconfigure the task.
         
         @param request: ResetDtsJobRequest
         @param runtime: runtime options for this request RuntimeOptions
         @return: ResetDtsJobResponse
         """
         UtilClient.validate_model(request)
         query = {}
@@ -10025,42 +11363,42 @@
         )
 
     def reset_dts_job(
         self,
         request: dts_20200101_models.ResetDtsJobRequest,
     ) -> dts_20200101_models.ResetDtsJobResponse:
         """
-        >  If you clear the configurations of a data synchronization or change tracking task, DTS deletes the task. Then, DTS creates another task. The task is in the Not Configured state. You must call the [ConfigureDtsJob](~~208399~~) operation reconfigure the task.
+        @description >  If you clear the configurations of a data synchronization or change tracking task, DTS deletes the task. Then, DTS creates another task. The task is in the Not Configured state. You must call the [ConfigureDtsJob](https://help.aliyun.com/document_detail/208399.html) operation reconfigure the task.
         
         @param request: ResetDtsJobRequest
         @return: ResetDtsJobResponse
         """
         runtime = util_models.RuntimeOptions()
         return self.reset_dts_job_with_options(request, runtime)
 
     async def reset_dts_job_async(
         self,
         request: dts_20200101_models.ResetDtsJobRequest,
     ) -> dts_20200101_models.ResetDtsJobResponse:
         """
-        >  If you clear the configurations of a data synchronization or change tracking task, DTS deletes the task. Then, DTS creates another task. The task is in the Not Configured state. You must call the [ConfigureDtsJob](~~208399~~) operation reconfigure the task.
+        @description >  If you clear the configurations of a data synchronization or change tracking task, DTS deletes the task. Then, DTS creates another task. The task is in the Not Configured state. You must call the [ConfigureDtsJob](https://help.aliyun.com/document_detail/208399.html) operation reconfigure the task.
         
         @param request: ResetDtsJobRequest
         @return: ResetDtsJobResponse
         """
         runtime = util_models.RuntimeOptions()
         return await self.reset_dts_job_with_options_async(request, runtime)
 
     def reset_synchronization_job_with_options(
         self,
         request: dts_20200101_models.ResetSynchronizationJobRequest,
         runtime: util_models.RuntimeOptions,
     ) -> dts_20200101_models.ResetSynchronizationJobResponse:
         """
-        >  If you clear the configurations of a data synchronization task, the task will be released. To start the task again, you must call the *ConfigureSynchronizationJob** operation to reconfigure the task.
+        @description >  If you clear the configurations of a data synchronization task, the task will be released. To start the task again, you must call the *ConfigureSynchronizationJob** operation to reconfigure the task.
         
         @param request: ResetSynchronizationJobRequest
         @param runtime: runtime options for this request RuntimeOptions
         @return: ResetSynchronizationJobResponse
         """
         UtilClient.validate_model(request)
         query = {}
@@ -10097,15 +11435,15 @@
 
     async def reset_synchronization_job_with_options_async(
         self,
         request: dts_20200101_models.ResetSynchronizationJobRequest,
         runtime: util_models.RuntimeOptions,
     ) -> dts_20200101_models.ResetSynchronizationJobResponse:
         """
-        >  If you clear the configurations of a data synchronization task, the task will be released. To start the task again, you must call the *ConfigureSynchronizationJob** operation to reconfigure the task.
+        @description >  If you clear the configurations of a data synchronization task, the task will be released. To start the task again, you must call the *ConfigureSynchronizationJob** operation to reconfigure the task.
         
         @param request: ResetSynchronizationJobRequest
         @param runtime: runtime options for this request RuntimeOptions
         @return: ResetSynchronizationJobResponse
         """
         UtilClient.validate_model(request)
         query = {}
@@ -10141,40 +11479,47 @@
         )
 
     def reset_synchronization_job(
         self,
         request: dts_20200101_models.ResetSynchronizationJobRequest,
     ) -> dts_20200101_models.ResetSynchronizationJobResponse:
         """
-        >  If you clear the configurations of a data synchronization task, the task will be released. To start the task again, you must call the *ConfigureSynchronizationJob** operation to reconfigure the task.
+        @description >  If you clear the configurations of a data synchronization task, the task will be released. To start the task again, you must call the *ConfigureSynchronizationJob** operation to reconfigure the task.
         
         @param request: ResetSynchronizationJobRequest
         @return: ResetSynchronizationJobResponse
         """
         runtime = util_models.RuntimeOptions()
         return self.reset_synchronization_job_with_options(request, runtime)
 
     async def reset_synchronization_job_async(
         self,
         request: dts_20200101_models.ResetSynchronizationJobRequest,
     ) -> dts_20200101_models.ResetSynchronizationJobResponse:
         """
-        >  If you clear the configurations of a data synchronization task, the task will be released. To start the task again, you must call the *ConfigureSynchronizationJob** operation to reconfigure the task.
+        @description >  If you clear the configurations of a data synchronization task, the task will be released. To start the task again, you must call the *ConfigureSynchronizationJob** operation to reconfigure the task.
         
         @param request: ResetSynchronizationJobRequest
         @return: ResetSynchronizationJobResponse
         """
         runtime = util_models.RuntimeOptions()
         return await self.reset_synchronization_job_with_options_async(request, runtime)
 
     def reverse_two_way_direction_with_options(
         self,
         request: dts_20200101_models.ReverseTwoWayDirectionRequest,
         runtime: util_models.RuntimeOptions,
     ) -> dts_20200101_models.ReverseTwoWayDirectionResponse:
+        """
+        @summary 调转双向任务的方向
+        
+        @param request: ReverseTwoWayDirectionRequest
+        @param runtime: runtime options for this request RuntimeOptions
+        @return: ReverseTwoWayDirectionResponse
+        """
         UtilClient.validate_model(request)
         query = {}
         if not UtilClient.is_unset(request.dts_instance_id):
             query['DtsInstanceId'] = request.dts_instance_id
         if not UtilClient.is_unset(request.ignore_error_sub_job):
             query['IgnoreErrorSubJob'] = request.ignore_error_sub_job
         if not UtilClient.is_unset(request.region_id):
@@ -10201,14 +11546,21 @@
         )
 
     async def reverse_two_way_direction_with_options_async(
         self,
         request: dts_20200101_models.ReverseTwoWayDirectionRequest,
         runtime: util_models.RuntimeOptions,
     ) -> dts_20200101_models.ReverseTwoWayDirectionResponse:
+        """
+        @summary 调转双向任务的方向
+        
+        @param request: ReverseTwoWayDirectionRequest
+        @param runtime: runtime options for this request RuntimeOptions
+        @return: ReverseTwoWayDirectionResponse
+        """
         UtilClient.validate_model(request)
         query = {}
         if not UtilClient.is_unset(request.dts_instance_id):
             query['DtsInstanceId'] = request.dts_instance_id
         if not UtilClient.is_unset(request.ignore_error_sub_job):
             query['IgnoreErrorSubJob'] = request.ignore_error_sub_job
         if not UtilClient.is_unset(request.region_id):
@@ -10234,31 +11586,45 @@
             await self.call_api_async(params, req, runtime)
         )
 
     def reverse_two_way_direction(
         self,
         request: dts_20200101_models.ReverseTwoWayDirectionRequest,
     ) -> dts_20200101_models.ReverseTwoWayDirectionResponse:
+        """
+        @summary 调转双向任务的方向
+        
+        @param request: ReverseTwoWayDirectionRequest
+        @return: ReverseTwoWayDirectionResponse
+        """
         runtime = util_models.RuntimeOptions()
         return self.reverse_two_way_direction_with_options(request, runtime)
 
     async def reverse_two_way_direction_async(
         self,
         request: dts_20200101_models.ReverseTwoWayDirectionRequest,
     ) -> dts_20200101_models.ReverseTwoWayDirectionResponse:
+        """
+        @summary 调转双向任务的方向
+        
+        @param request: ReverseTwoWayDirectionRequest
+        @return: ReverseTwoWayDirectionResponse
+        """
         runtime = util_models.RuntimeOptions()
         return await self.reverse_two_way_direction_with_options_async(request, runtime)
 
     def shield_precheck_with_options(
         self,
         request: dts_20200101_models.ShieldPrecheckRequest,
         runtime: util_models.RuntimeOptions,
     ) -> dts_20200101_models.ShieldPrecheckResponse:
         """
-        If you call this operation to ignore all precheck items, you must call the [StartMigrationJob](https://www.alibabacloud.com/help/zh/doc-detail/49429.htm) or [StartSynchronizationJob](https://www.alibabacloud.com/help/zh/doc-detail/49448.htm) operation. DTS performs a precheck again. After the data migration or synchronization task passes the precheck, the task will be automatically started.
+        @summary Ignores the precheck items that a data migration or synchronization task may fail to pass.
+        
+        @description If you call this operation to ignore all precheck items, you must call the [StartMigrationJob](https://www.alibabacloud.com/help/zh/doc-detail/49429.htm) or [StartSynchronizationJob](https://www.alibabacloud.com/help/zh/doc-detail/49448.htm) operation. DTS performs a precheck again. After the data migration or synchronization task passes the precheck, the task will be automatically started.
         
         @param request: ShieldPrecheckRequest
         @param runtime: runtime options for this request RuntimeOptions
         @return: ShieldPrecheckResponse
         """
         UtilClient.validate_model(request)
         query = {}
@@ -10291,15 +11657,17 @@
 
     async def shield_precheck_with_options_async(
         self,
         request: dts_20200101_models.ShieldPrecheckRequest,
         runtime: util_models.RuntimeOptions,
     ) -> dts_20200101_models.ShieldPrecheckResponse:
         """
-        If you call this operation to ignore all precheck items, you must call the [StartMigrationJob](https://www.alibabacloud.com/help/zh/doc-detail/49429.htm) or [StartSynchronizationJob](https://www.alibabacloud.com/help/zh/doc-detail/49448.htm) operation. DTS performs a precheck again. After the data migration or synchronization task passes the precheck, the task will be automatically started.
+        @summary Ignores the precheck items that a data migration or synchronization task may fail to pass.
+        
+        @description If you call this operation to ignore all precheck items, you must call the [StartMigrationJob](https://www.alibabacloud.com/help/zh/doc-detail/49429.htm) or [StartSynchronizationJob](https://www.alibabacloud.com/help/zh/doc-detail/49448.htm) operation. DTS performs a precheck again. After the data migration or synchronization task passes the precheck, the task will be automatically started.
         
         @param request: ShieldPrecheckRequest
         @param runtime: runtime options for this request RuntimeOptions
         @return: ShieldPrecheckResponse
         """
         UtilClient.validate_model(request)
         query = {}
@@ -10331,40 +11699,51 @@
         )
 
     def shield_precheck(
         self,
         request: dts_20200101_models.ShieldPrecheckRequest,
     ) -> dts_20200101_models.ShieldPrecheckResponse:
         """
-        If you call this operation to ignore all precheck items, you must call the [StartMigrationJob](https://www.alibabacloud.com/help/zh/doc-detail/49429.htm) or [StartSynchronizationJob](https://www.alibabacloud.com/help/zh/doc-detail/49448.htm) operation. DTS performs a precheck again. After the data migration or synchronization task passes the precheck, the task will be automatically started.
+        @summary Ignores the precheck items that a data migration or synchronization task may fail to pass.
+        
+        @description If you call this operation to ignore all precheck items, you must call the [StartMigrationJob](https://www.alibabacloud.com/help/zh/doc-detail/49429.htm) or [StartSynchronizationJob](https://www.alibabacloud.com/help/zh/doc-detail/49448.htm) operation. DTS performs a precheck again. After the data migration or synchronization task passes the precheck, the task will be automatically started.
         
         @param request: ShieldPrecheckRequest
         @return: ShieldPrecheckResponse
         """
         runtime = util_models.RuntimeOptions()
         return self.shield_precheck_with_options(request, runtime)
 
     async def shield_precheck_async(
         self,
         request: dts_20200101_models.ShieldPrecheckRequest,
     ) -> dts_20200101_models.ShieldPrecheckResponse:
         """
-        If you call this operation to ignore all precheck items, you must call the [StartMigrationJob](https://www.alibabacloud.com/help/zh/doc-detail/49429.htm) or [StartSynchronizationJob](https://www.alibabacloud.com/help/zh/doc-detail/49448.htm) operation. DTS performs a precheck again. After the data migration or synchronization task passes the precheck, the task will be automatically started.
+        @summary Ignores the precheck items that a data migration or synchronization task may fail to pass.
+        
+        @description If you call this operation to ignore all precheck items, you must call the [StartMigrationJob](https://www.alibabacloud.com/help/zh/doc-detail/49429.htm) or [StartSynchronizationJob](https://www.alibabacloud.com/help/zh/doc-detail/49448.htm) operation. DTS performs a precheck again. After the data migration or synchronization task passes the precheck, the task will be automatically started.
         
         @param request: ShieldPrecheckRequest
         @return: ShieldPrecheckResponse
         """
         runtime = util_models.RuntimeOptions()
         return await self.shield_precheck_with_options_async(request, runtime)
 
     def skip_pre_check_with_options(
         self,
         request: dts_20200101_models.SkipPreCheckRequest,
         runtime: util_models.RuntimeOptions,
     ) -> dts_20200101_models.SkipPreCheckResponse:
+        """
+        @summary Skips one or more precheck items.
+        
+        @param request: SkipPreCheckRequest
+        @param runtime: runtime options for this request RuntimeOptions
+        @return: SkipPreCheckResponse
+        """
         UtilClient.validate_model(request)
         query = {}
         if not UtilClient.is_unset(request.dts_job_id):
             query['DtsJobId'] = request.dts_job_id
         if not UtilClient.is_unset(request.job_id):
             query['JobId'] = request.job_id
         if not UtilClient.is_unset(request.region_id):
@@ -10397,14 +11776,21 @@
         )
 
     async def skip_pre_check_with_options_async(
         self,
         request: dts_20200101_models.SkipPreCheckRequest,
         runtime: util_models.RuntimeOptions,
     ) -> dts_20200101_models.SkipPreCheckResponse:
+        """
+        @summary Skips one or more precheck items.
+        
+        @param request: SkipPreCheckRequest
+        @param runtime: runtime options for this request RuntimeOptions
+        @return: SkipPreCheckResponse
+        """
         UtilClient.validate_model(request)
         query = {}
         if not UtilClient.is_unset(request.dts_job_id):
             query['DtsJobId'] = request.dts_job_id
         if not UtilClient.is_unset(request.job_id):
             query['JobId'] = request.job_id
         if not UtilClient.is_unset(request.region_id):
@@ -10436,29 +11822,46 @@
             await self.call_api_async(params, req, runtime)
         )
 
     def skip_pre_check(
         self,
         request: dts_20200101_models.SkipPreCheckRequest,
     ) -> dts_20200101_models.SkipPreCheckResponse:
+        """
+        @summary Skips one or more precheck items.
+        
+        @param request: SkipPreCheckRequest
+        @return: SkipPreCheckResponse
+        """
         runtime = util_models.RuntimeOptions()
         return self.skip_pre_check_with_options(request, runtime)
 
     async def skip_pre_check_async(
         self,
         request: dts_20200101_models.SkipPreCheckRequest,
     ) -> dts_20200101_models.SkipPreCheckResponse:
+        """
+        @summary Skips one or more precheck items.
+        
+        @param request: SkipPreCheckRequest
+        @return: SkipPreCheckResponse
+        """
         runtime = util_models.RuntimeOptions()
         return await self.skip_pre_check_with_options_async(request, runtime)
 
     def start_dts_job_with_options(
         self,
         request: dts_20200101_models.StartDtsJobRequest,
         runtime: util_models.RuntimeOptions,
     ) -> dts_20200101_models.StartDtsJobResponse:
+        """
+        @param request: StartDtsJobRequest
+        @param runtime: runtime options for this request RuntimeOptions
+        @return: StartDtsJobResponse
+        """
         UtilClient.validate_model(request)
         query = {}
         if not UtilClient.is_unset(request.dts_instance_id):
             query['DtsInstanceId'] = request.dts_instance_id
         if not UtilClient.is_unset(request.dts_job_id):
             query['DtsJobId'] = request.dts_job_id
         if not UtilClient.is_unset(request.region_id):
@@ -10489,14 +11892,19 @@
         )
 
     async def start_dts_job_with_options_async(
         self,
         request: dts_20200101_models.StartDtsJobRequest,
         runtime: util_models.RuntimeOptions,
     ) -> dts_20200101_models.StartDtsJobResponse:
+        """
+        @param request: StartDtsJobRequest
+        @param runtime: runtime options for this request RuntimeOptions
+        @return: StartDtsJobResponse
+        """
         UtilClient.validate_model(request)
         query = {}
         if not UtilClient.is_unset(request.dts_instance_id):
             query['DtsInstanceId'] = request.dts_instance_id
         if not UtilClient.is_unset(request.dts_job_id):
             query['DtsJobId'] = request.dts_job_id
         if not UtilClient.is_unset(request.region_id):
@@ -10526,29 +11934,42 @@
             await self.call_api_async(params, req, runtime)
         )
 
     def start_dts_job(
         self,
         request: dts_20200101_models.StartDtsJobRequest,
     ) -> dts_20200101_models.StartDtsJobResponse:
+        """
+        @param request: StartDtsJobRequest
+        @return: StartDtsJobResponse
+        """
         runtime = util_models.RuntimeOptions()
         return self.start_dts_job_with_options(request, runtime)
 
     async def start_dts_job_async(
         self,
         request: dts_20200101_models.StartDtsJobRequest,
     ) -> dts_20200101_models.StartDtsJobResponse:
+        """
+        @param request: StartDtsJobRequest
+        @return: StartDtsJobResponse
+        """
         runtime = util_models.RuntimeOptions()
         return await self.start_dts_job_with_options_async(request, runtime)
 
     def start_dts_jobs_with_options(
         self,
         request: dts_20200101_models.StartDtsJobsRequest,
         runtime: util_models.RuntimeOptions,
     ) -> dts_20200101_models.StartDtsJobsResponse:
+        """
+        @param request: StartDtsJobsRequest
+        @param runtime: runtime options for this request RuntimeOptions
+        @return: StartDtsJobsResponse
+        """
         UtilClient.validate_model(request)
         query = {}
         if not UtilClient.is_unset(request.dts_job_ids):
             query['DtsJobIds'] = request.dts_job_ids
         if not UtilClient.is_unset(request.region_id):
             query['RegionId'] = request.region_id
         if not UtilClient.is_unset(request.resource_group_id):
@@ -10575,14 +11996,19 @@
         )
 
     async def start_dts_jobs_with_options_async(
         self,
         request: dts_20200101_models.StartDtsJobsRequest,
         runtime: util_models.RuntimeOptions,
     ) -> dts_20200101_models.StartDtsJobsResponse:
+        """
+        @param request: StartDtsJobsRequest
+        @param runtime: runtime options for this request RuntimeOptions
+        @return: StartDtsJobsResponse
+        """
         UtilClient.validate_model(request)
         query = {}
         if not UtilClient.is_unset(request.dts_job_ids):
             query['DtsJobIds'] = request.dts_job_ids
         if not UtilClient.is_unset(request.region_id):
             query['RegionId'] = request.region_id
         if not UtilClient.is_unset(request.resource_group_id):
@@ -10608,31 +12034,39 @@
             await self.call_api_async(params, req, runtime)
         )
 
     def start_dts_jobs(
         self,
         request: dts_20200101_models.StartDtsJobsRequest,
     ) -> dts_20200101_models.StartDtsJobsResponse:
+        """
+        @param request: StartDtsJobsRequest
+        @return: StartDtsJobsResponse
+        """
         runtime = util_models.RuntimeOptions()
         return self.start_dts_jobs_with_options(request, runtime)
 
     async def start_dts_jobs_async(
         self,
         request: dts_20200101_models.StartDtsJobsRequest,
     ) -> dts_20200101_models.StartDtsJobsResponse:
+        """
+        @param request: StartDtsJobsRequest
+        @return: StartDtsJobsResponse
+        """
         runtime = util_models.RuntimeOptions()
         return await self.start_dts_jobs_with_options_async(request, runtime)
 
     def start_migration_job_with_options(
         self,
         request: dts_20200101_models.StartMigrationJobRequest,
         runtime: util_models.RuntimeOptions,
     ) -> dts_20200101_models.StartMigrationJobResponse:
         """
-        >  When you call this operation, the data migration task must be in the Not Started, Paused, or Migration Failed state.
+        @description >  When you call this operation, the data migration task must be in the Not Started, Paused, or Migration Failed state.
         
         @param request: StartMigrationJobRequest
         @param runtime: runtime options for this request RuntimeOptions
         @return: StartMigrationJobResponse
         """
         UtilClient.validate_model(request)
         query = {}
@@ -10667,15 +12101,15 @@
 
     async def start_migration_job_with_options_async(
         self,
         request: dts_20200101_models.StartMigrationJobRequest,
         runtime: util_models.RuntimeOptions,
     ) -> dts_20200101_models.StartMigrationJobResponse:
         """
-        >  When you call this operation, the data migration task must be in the Not Started, Paused, or Migration Failed state.
+        @description >  When you call this operation, the data migration task must be in the Not Started, Paused, or Migration Failed state.
         
         @param request: StartMigrationJobRequest
         @param runtime: runtime options for this request RuntimeOptions
         @return: StartMigrationJobResponse
         """
         UtilClient.validate_model(request)
         query = {}
@@ -10709,42 +12143,44 @@
         )
 
     def start_migration_job(
         self,
         request: dts_20200101_models.StartMigrationJobRequest,
     ) -> dts_20200101_models.StartMigrationJobResponse:
         """
-        >  When you call this operation, the data migration task must be in the Not Started, Paused, or Migration Failed state.
+        @description >  When you call this operation, the data migration task must be in the Not Started, Paused, or Migration Failed state.
         
         @param request: StartMigrationJobRequest
         @return: StartMigrationJobResponse
         """
         runtime = util_models.RuntimeOptions()
         return self.start_migration_job_with_options(request, runtime)
 
     async def start_migration_job_async(
         self,
         request: dts_20200101_models.StartMigrationJobRequest,
     ) -> dts_20200101_models.StartMigrationJobResponse:
         """
-        >  When you call this operation, the data migration task must be in the Not Started, Paused, or Migration Failed state.
+        @description >  When you call this operation, the data migration task must be in the Not Started, Paused, or Migration Failed state.
         
         @param request: StartMigrationJobRequest
         @return: StartMigrationJobResponse
         """
         runtime = util_models.RuntimeOptions()
         return await self.start_migration_job_with_options_async(request, runtime)
 
     def start_reverse_writer_with_options(
         self,
         request: dts_20200101_models.StartReverseWriterRequest,
         runtime: util_models.RuntimeOptions,
     ) -> dts_20200101_models.StartReverseWriterResponse:
         """
-        Before you call this operation, make sure that your instance is not released and is paused. You can check the status of the instance in the Data Transmission Service (DTS) console or by calling the [DescribeDtsJobDetail](~~208925~~) operation.
+        @summary Starts the reverse task that is created by calling the CreateReverseDtsJob operation.
+        
+        @description Before you call this operation, make sure that your instance is not released and is paused. You can check the status of the instance in the Data Transmission Service (DTS) console or by calling the [DescribeDtsJobDetail](https://help.aliyun.com/document_detail/208925.html) operation.
         
         @param request: StartReverseWriterRequest
         @param runtime: runtime options for this request RuntimeOptions
         @return: StartReverseWriterResponse
         """
         UtilClient.validate_model(request)
         query = {}
@@ -10775,15 +12211,17 @@
 
     async def start_reverse_writer_with_options_async(
         self,
         request: dts_20200101_models.StartReverseWriterRequest,
         runtime: util_models.RuntimeOptions,
     ) -> dts_20200101_models.StartReverseWriterResponse:
         """
-        Before you call this operation, make sure that your instance is not released and is paused. You can check the status of the instance in the Data Transmission Service (DTS) console or by calling the [DescribeDtsJobDetail](~~208925~~) operation.
+        @summary Starts the reverse task that is created by calling the CreateReverseDtsJob operation.
+        
+        @description Before you call this operation, make sure that your instance is not released and is paused. You can check the status of the instance in the Data Transmission Service (DTS) console or by calling the [DescribeDtsJobDetail](https://help.aliyun.com/document_detail/208925.html) operation.
         
         @param request: StartReverseWriterRequest
         @param runtime: runtime options for this request RuntimeOptions
         @return: StartReverseWriterResponse
         """
         UtilClient.validate_model(request)
         query = {}
@@ -10813,42 +12251,46 @@
         )
 
     def start_reverse_writer(
         self,
         request: dts_20200101_models.StartReverseWriterRequest,
     ) -> dts_20200101_models.StartReverseWriterResponse:
         """
-        Before you call this operation, make sure that your instance is not released and is paused. You can check the status of the instance in the Data Transmission Service (DTS) console or by calling the [DescribeDtsJobDetail](~~208925~~) operation.
+        @summary Starts the reverse task that is created by calling the CreateReverseDtsJob operation.
+        
+        @description Before you call this operation, make sure that your instance is not released and is paused. You can check the status of the instance in the Data Transmission Service (DTS) console or by calling the [DescribeDtsJobDetail](https://help.aliyun.com/document_detail/208925.html) operation.
         
         @param request: StartReverseWriterRequest
         @return: StartReverseWriterResponse
         """
         runtime = util_models.RuntimeOptions()
         return self.start_reverse_writer_with_options(request, runtime)
 
     async def start_reverse_writer_async(
         self,
         request: dts_20200101_models.StartReverseWriterRequest,
     ) -> dts_20200101_models.StartReverseWriterResponse:
         """
-        Before you call this operation, make sure that your instance is not released and is paused. You can check the status of the instance in the Data Transmission Service (DTS) console or by calling the [DescribeDtsJobDetail](~~208925~~) operation.
+        @summary Starts the reverse task that is created by calling the CreateReverseDtsJob operation.
+        
+        @description Before you call this operation, make sure that your instance is not released and is paused. You can check the status of the instance in the Data Transmission Service (DTS) console or by calling the [DescribeDtsJobDetail](https://help.aliyun.com/document_detail/208925.html) operation.
         
         @param request: StartReverseWriterRequest
         @return: StartReverseWriterResponse
         """
         runtime = util_models.RuntimeOptions()
         return await self.start_reverse_writer_with_options_async(request, runtime)
 
     def start_subscription_instance_with_options(
         self,
         request: dts_20200101_models.StartSubscriptionInstanceRequest,
         runtime: util_models.RuntimeOptions,
     ) -> dts_20200101_models.StartSubscriptionInstanceResponse:
         """
-        When you call this operation, the change tracking task must be in the NotStarted or Failed state.
+        @description When you call this operation, the change tracking task must be in the NotStarted or Failed state.
         
         @param request: StartSubscriptionInstanceRequest
         @param runtime: runtime options for this request RuntimeOptions
         @return: StartSubscriptionInstanceResponse
         """
         UtilClient.validate_model(request)
         query = {}
@@ -10883,15 +12325,15 @@
 
     async def start_subscription_instance_with_options_async(
         self,
         request: dts_20200101_models.StartSubscriptionInstanceRequest,
         runtime: util_models.RuntimeOptions,
     ) -> dts_20200101_models.StartSubscriptionInstanceResponse:
         """
-        When you call this operation, the change tracking task must be in the NotStarted or Failed state.
+        @description When you call this operation, the change tracking task must be in the NotStarted or Failed state.
         
         @param request: StartSubscriptionInstanceRequest
         @param runtime: runtime options for this request RuntimeOptions
         @return: StartSubscriptionInstanceResponse
         """
         UtilClient.validate_model(request)
         query = {}
@@ -10925,40 +12367,47 @@
         )
 
     def start_subscription_instance(
         self,
         request: dts_20200101_models.StartSubscriptionInstanceRequest,
     ) -> dts_20200101_models.StartSubscriptionInstanceResponse:
         """
-        When you call this operation, the change tracking task must be in the NotStarted or Failed state.
+        @description When you call this operation, the change tracking task must be in the NotStarted or Failed state.
         
         @param request: StartSubscriptionInstanceRequest
         @return: StartSubscriptionInstanceResponse
         """
         runtime = util_models.RuntimeOptions()
         return self.start_subscription_instance_with_options(request, runtime)
 
     async def start_subscription_instance_async(
         self,
         request: dts_20200101_models.StartSubscriptionInstanceRequest,
     ) -> dts_20200101_models.StartSubscriptionInstanceResponse:
         """
-        When you call this operation, the change tracking task must be in the NotStarted or Failed state.
+        @description When you call this operation, the change tracking task must be in the NotStarted or Failed state.
         
         @param request: StartSubscriptionInstanceRequest
         @return: StartSubscriptionInstanceResponse
         """
         runtime = util_models.RuntimeOptions()
         return await self.start_subscription_instance_with_options_async(request, runtime)
 
     def start_synchronization_job_with_options(
         self,
         request: dts_20200101_models.StartSynchronizationJobRequest,
         runtime: util_models.RuntimeOptions,
     ) -> dts_20200101_models.StartSynchronizationJobResponse:
+        """
+        @summary Starts a data synchronization task.
+        
+        @param request: StartSynchronizationJobRequest
+        @param runtime: runtime options for this request RuntimeOptions
+        @return: StartSynchronizationJobResponse
+        """
         UtilClient.validate_model(request)
         query = {}
         if not UtilClient.is_unset(request.account_id):
             query['AccountId'] = request.account_id
         if not UtilClient.is_unset(request.owner_id):
             query['OwnerId'] = request.owner_id
         if not UtilClient.is_unset(request.region_id):
@@ -10989,14 +12438,21 @@
         )
 
     async def start_synchronization_job_with_options_async(
         self,
         request: dts_20200101_models.StartSynchronizationJobRequest,
         runtime: util_models.RuntimeOptions,
     ) -> dts_20200101_models.StartSynchronizationJobResponse:
+        """
+        @summary Starts a data synchronization task.
+        
+        @param request: StartSynchronizationJobRequest
+        @param runtime: runtime options for this request RuntimeOptions
+        @return: StartSynchronizationJobResponse
+        """
         UtilClient.validate_model(request)
         query = {}
         if not UtilClient.is_unset(request.account_id):
             query['AccountId'] = request.account_id
         if not UtilClient.is_unset(request.owner_id):
             query['OwnerId'] = request.owner_id
         if not UtilClient.is_unset(request.region_id):
@@ -11026,29 +12482,48 @@
             await self.call_api_async(params, req, runtime)
         )
 
     def start_synchronization_job(
         self,
         request: dts_20200101_models.StartSynchronizationJobRequest,
     ) -> dts_20200101_models.StartSynchronizationJobResponse:
+        """
+        @summary Starts a data synchronization task.
+        
+        @param request: StartSynchronizationJobRequest
+        @return: StartSynchronizationJobResponse
+        """
         runtime = util_models.RuntimeOptions()
         return self.start_synchronization_job_with_options(request, runtime)
 
     async def start_synchronization_job_async(
         self,
         request: dts_20200101_models.StartSynchronizationJobRequest,
     ) -> dts_20200101_models.StartSynchronizationJobResponse:
+        """
+        @summary Starts a data synchronization task.
+        
+        @param request: StartSynchronizationJobRequest
+        @return: StartSynchronizationJobResponse
+        """
         runtime = util_models.RuntimeOptions()
         return await self.start_synchronization_job_with_options_async(request, runtime)
 
     def stop_dedicated_cluster_with_options(
         self,
         request: dts_20200101_models.StopDedicatedClusterRequest,
         runtime: util_models.RuntimeOptions,
     ) -> dts_20200101_models.StopDedicatedClusterResponse:
+        """
+        @summary Releases a cluster.
+        
+        @param request: StopDedicatedClusterRequest
+        @param runtime: runtime options for this request RuntimeOptions
+        @return: StopDedicatedClusterResponse
+        """
         UtilClient.validate_model(request)
         query = {}
         if not UtilClient.is_unset(request.dedicated_cluster_id):
             query['DedicatedClusterId'] = request.dedicated_cluster_id
         if not UtilClient.is_unset(request.dedicated_cluster_name):
             query['DedicatedClusterName'] = request.dedicated_cluster_name
         if not UtilClient.is_unset(request.instance_id):
@@ -11079,14 +12554,21 @@
         )
 
     async def stop_dedicated_cluster_with_options_async(
         self,
         request: dts_20200101_models.StopDedicatedClusterRequest,
         runtime: util_models.RuntimeOptions,
     ) -> dts_20200101_models.StopDedicatedClusterResponse:
+        """
+        @summary Releases a cluster.
+        
+        @param request: StopDedicatedClusterRequest
+        @param runtime: runtime options for this request RuntimeOptions
+        @return: StopDedicatedClusterResponse
+        """
         UtilClient.validate_model(request)
         query = {}
         if not UtilClient.is_unset(request.dedicated_cluster_id):
             query['DedicatedClusterId'] = request.dedicated_cluster_id
         if not UtilClient.is_unset(request.dedicated_cluster_name):
             query['DedicatedClusterName'] = request.dedicated_cluster_name
         if not UtilClient.is_unset(request.instance_id):
@@ -11116,29 +12598,46 @@
             await self.call_api_async(params, req, runtime)
         )
 
     def stop_dedicated_cluster(
         self,
         request: dts_20200101_models.StopDedicatedClusterRequest,
     ) -> dts_20200101_models.StopDedicatedClusterResponse:
+        """
+        @summary Releases a cluster.
+        
+        @param request: StopDedicatedClusterRequest
+        @return: StopDedicatedClusterResponse
+        """
         runtime = util_models.RuntimeOptions()
         return self.stop_dedicated_cluster_with_options(request, runtime)
 
     async def stop_dedicated_cluster_async(
         self,
         request: dts_20200101_models.StopDedicatedClusterRequest,
     ) -> dts_20200101_models.StopDedicatedClusterResponse:
+        """
+        @summary Releases a cluster.
+        
+        @param request: StopDedicatedClusterRequest
+        @return: StopDedicatedClusterResponse
+        """
         runtime = util_models.RuntimeOptions()
         return await self.stop_dedicated_cluster_with_options_async(request, runtime)
 
     def stop_dts_job_with_options(
         self,
         request: dts_20200101_models.StopDtsJobRequest,
         runtime: util_models.RuntimeOptions,
     ) -> dts_20200101_models.StopDtsJobResponse:
+        """
+        @param request: StopDtsJobRequest
+        @param runtime: runtime options for this request RuntimeOptions
+        @return: StopDtsJobResponse
+        """
         UtilClient.validate_model(request)
         query = {}
         if not UtilClient.is_unset(request.dts_instance_id):
             query['DtsInstanceId'] = request.dts_instance_id
         if not UtilClient.is_unset(request.dts_job_id):
             query['DtsJobId'] = request.dts_job_id
         if not UtilClient.is_unset(request.region_id):
@@ -11169,14 +12668,19 @@
         )
 
     async def stop_dts_job_with_options_async(
         self,
         request: dts_20200101_models.StopDtsJobRequest,
         runtime: util_models.RuntimeOptions,
     ) -> dts_20200101_models.StopDtsJobResponse:
+        """
+        @param request: StopDtsJobRequest
+        @param runtime: runtime options for this request RuntimeOptions
+        @return: StopDtsJobResponse
+        """
         UtilClient.validate_model(request)
         query = {}
         if not UtilClient.is_unset(request.dts_instance_id):
             query['DtsInstanceId'] = request.dts_instance_id
         if not UtilClient.is_unset(request.dts_job_id):
             query['DtsJobId'] = request.dts_job_id
         if not UtilClient.is_unset(request.region_id):
@@ -11206,29 +12710,42 @@
             await self.call_api_async(params, req, runtime)
         )
 
     def stop_dts_job(
         self,
         request: dts_20200101_models.StopDtsJobRequest,
     ) -> dts_20200101_models.StopDtsJobResponse:
+        """
+        @param request: StopDtsJobRequest
+        @return: StopDtsJobResponse
+        """
         runtime = util_models.RuntimeOptions()
         return self.stop_dts_job_with_options(request, runtime)
 
     async def stop_dts_job_async(
         self,
         request: dts_20200101_models.StopDtsJobRequest,
     ) -> dts_20200101_models.StopDtsJobResponse:
+        """
+        @param request: StopDtsJobRequest
+        @return: StopDtsJobResponse
+        """
         runtime = util_models.RuntimeOptions()
         return await self.stop_dts_job_with_options_async(request, runtime)
 
     def stop_dts_jobs_with_options(
         self,
         request: dts_20200101_models.StopDtsJobsRequest,
         runtime: util_models.RuntimeOptions,
     ) -> dts_20200101_models.StopDtsJobsResponse:
+        """
+        @param request: StopDtsJobsRequest
+        @param runtime: runtime options for this request RuntimeOptions
+        @return: StopDtsJobsResponse
+        """
         UtilClient.validate_model(request)
         query = {}
         if not UtilClient.is_unset(request.dts_job_ids):
             query['DtsJobIds'] = request.dts_job_ids
         if not UtilClient.is_unset(request.region_id):
             query['RegionId'] = request.region_id
         if not UtilClient.is_unset(request.resource_group_id):
@@ -11255,14 +12772,19 @@
         )
 
     async def stop_dts_jobs_with_options_async(
         self,
         request: dts_20200101_models.StopDtsJobsRequest,
         runtime: util_models.RuntimeOptions,
     ) -> dts_20200101_models.StopDtsJobsResponse:
+        """
+        @param request: StopDtsJobsRequest
+        @param runtime: runtime options for this request RuntimeOptions
+        @return: StopDtsJobsResponse
+        """
         UtilClient.validate_model(request)
         query = {}
         if not UtilClient.is_unset(request.dts_job_ids):
             query['DtsJobIds'] = request.dts_job_ids
         if not UtilClient.is_unset(request.region_id):
             query['RegionId'] = request.region_id
         if not UtilClient.is_unset(request.resource_group_id):
@@ -11288,31 +12810,39 @@
             await self.call_api_async(params, req, runtime)
         )
 
     def stop_dts_jobs(
         self,
         request: dts_20200101_models.StopDtsJobsRequest,
     ) -> dts_20200101_models.StopDtsJobsResponse:
+        """
+        @param request: StopDtsJobsRequest
+        @return: StopDtsJobsResponse
+        """
         runtime = util_models.RuntimeOptions()
         return self.stop_dts_jobs_with_options(request, runtime)
 
     async def stop_dts_jobs_async(
         self,
         request: dts_20200101_models.StopDtsJobsRequest,
     ) -> dts_20200101_models.StopDtsJobsResponse:
+        """
+        @param request: StopDtsJobsRequest
+        @return: StopDtsJobsResponse
+        """
         runtime = util_models.RuntimeOptions()
         return await self.stop_dts_jobs_with_options_async(request, runtime)
 
     def stop_migration_job_with_options(
         self,
         request: dts_20200101_models.StopMigrationJobRequest,
         runtime: util_models.RuntimeOptions,
     ) -> dts_20200101_models.StopMigrationJobResponse:
         """
-        >  After you call this operation to stop a data migration task, the status of the task changes to Finished and you cannot restart the task by calling the [StartMigrationJob](~~49429~~) operation.
+        @description >  After you call this operation to stop a data migration task, the status of the task changes to Finished and you cannot restart the task by calling the [StartMigrationJob](https://help.aliyun.com/document_detail/49429.html) operation.
         
         @param request: StopMigrationJobRequest
         @param runtime: runtime options for this request RuntimeOptions
         @return: StopMigrationJobResponse
         """
         UtilClient.validate_model(request)
         query = {}
@@ -11349,15 +12879,15 @@
 
     async def stop_migration_job_with_options_async(
         self,
         request: dts_20200101_models.StopMigrationJobRequest,
         runtime: util_models.RuntimeOptions,
     ) -> dts_20200101_models.StopMigrationJobResponse:
         """
-        >  After you call this operation to stop a data migration task, the status of the task changes to Finished and you cannot restart the task by calling the [StartMigrationJob](~~49429~~) operation.
+        @description >  After you call this operation to stop a data migration task, the status of the task changes to Finished and you cannot restart the task by calling the [StartMigrationJob](https://help.aliyun.com/document_detail/49429.html) operation.
         
         @param request: StopMigrationJobRequest
         @param runtime: runtime options for this request RuntimeOptions
         @return: StopMigrationJobResponse
         """
         UtilClient.validate_model(request)
         query = {}
@@ -11393,40 +12923,45 @@
         )
 
     def stop_migration_job(
         self,
         request: dts_20200101_models.StopMigrationJobRequest,
     ) -> dts_20200101_models.StopMigrationJobResponse:
         """
-        >  After you call this operation to stop a data migration task, the status of the task changes to Finished and you cannot restart the task by calling the [StartMigrationJob](~~49429~~) operation.
+        @description >  After you call this operation to stop a data migration task, the status of the task changes to Finished and you cannot restart the task by calling the [StartMigrationJob](https://help.aliyun.com/document_detail/49429.html) operation.
         
         @param request: StopMigrationJobRequest
         @return: StopMigrationJobResponse
         """
         runtime = util_models.RuntimeOptions()
         return self.stop_migration_job_with_options(request, runtime)
 
     async def stop_migration_job_async(
         self,
         request: dts_20200101_models.StopMigrationJobRequest,
     ) -> dts_20200101_models.StopMigrationJobResponse:
         """
-        >  After you call this operation to stop a data migration task, the status of the task changes to Finished and you cannot restart the task by calling the [StartMigrationJob](~~49429~~) operation.
+        @description >  After you call this operation to stop a data migration task, the status of the task changes to Finished and you cannot restart the task by calling the [StartMigrationJob](https://help.aliyun.com/document_detail/49429.html) operation.
         
         @param request: StopMigrationJobRequest
         @return: StopMigrationJobResponse
         """
         runtime = util_models.RuntimeOptions()
         return await self.stop_migration_job_with_options_async(request, runtime)
 
     def summary_job_detail_with_options(
         self,
         request: dts_20200101_models.SummaryJobDetailRequest,
         runtime: util_models.RuntimeOptions,
     ) -> dts_20200101_models.SummaryJobDetailResponse:
+        """
+        @param request: SummaryJobDetailRequest
+        @param runtime: runtime options for this request RuntimeOptions
+        @return: SummaryJobDetailResponse
+        """
         UtilClient.validate_model(request)
         query = {}
         if not UtilClient.is_unset(request.dts_instance_id):
             query['DtsInstanceId'] = request.dts_instance_id
         if not UtilClient.is_unset(request.dts_job_id):
             query['DtsJobId'] = request.dts_job_id
         if not UtilClient.is_unset(request.job_code):
@@ -11461,14 +12996,19 @@
         )
 
     async def summary_job_detail_with_options_async(
         self,
         request: dts_20200101_models.SummaryJobDetailRequest,
         runtime: util_models.RuntimeOptions,
     ) -> dts_20200101_models.SummaryJobDetailResponse:
+        """
+        @param request: SummaryJobDetailRequest
+        @param runtime: runtime options for this request RuntimeOptions
+        @return: SummaryJobDetailResponse
+        """
         UtilClient.validate_model(request)
         query = {}
         if not UtilClient.is_unset(request.dts_instance_id):
             query['DtsInstanceId'] = request.dts_instance_id
         if not UtilClient.is_unset(request.dts_job_id):
             query['DtsJobId'] = request.dts_job_id
         if not UtilClient.is_unset(request.job_code):
@@ -11502,31 +13042,39 @@
             await self.call_api_async(params, req, runtime)
         )
 
     def summary_job_detail(
         self,
         request: dts_20200101_models.SummaryJobDetailRequest,
     ) -> dts_20200101_models.SummaryJobDetailResponse:
+        """
+        @param request: SummaryJobDetailRequest
+        @return: SummaryJobDetailResponse
+        """
         runtime = util_models.RuntimeOptions()
         return self.summary_job_detail_with_options(request, runtime)
 
     async def summary_job_detail_async(
         self,
         request: dts_20200101_models.SummaryJobDetailRequest,
     ) -> dts_20200101_models.SummaryJobDetailResponse:
+        """
+        @param request: SummaryJobDetailRequest
+        @return: SummaryJobDetailResponse
+        """
         runtime = util_models.RuntimeOptions()
         return await self.summary_job_detail_with_options_async(request, runtime)
 
     def suspend_dts_job_with_options(
         self,
         request: dts_20200101_models.SuspendDtsJobRequest,
         runtime: util_models.RuntimeOptions,
     ) -> dts_20200101_models.SuspendDtsJobResponse:
         """
-        ***\
+        @description ***\
         
         @param request: SuspendDtsJobRequest
         @param runtime: runtime options for this request RuntimeOptions
         @return: SuspendDtsJobResponse
         """
         UtilClient.validate_model(request)
         query = {}
@@ -11563,15 +13111,15 @@
 
     async def suspend_dts_job_with_options_async(
         self,
         request: dts_20200101_models.SuspendDtsJobRequest,
         runtime: util_models.RuntimeOptions,
     ) -> dts_20200101_models.SuspendDtsJobResponse:
         """
-        ***\
+        @description ***\
         
         @param request: SuspendDtsJobRequest
         @param runtime: runtime options for this request RuntimeOptions
         @return: SuspendDtsJobResponse
         """
         UtilClient.validate_model(request)
         query = {}
@@ -11607,40 +13155,45 @@
         )
 
     def suspend_dts_job(
         self,
         request: dts_20200101_models.SuspendDtsJobRequest,
     ) -> dts_20200101_models.SuspendDtsJobResponse:
         """
-        ***\
+        @description ***\
         
         @param request: SuspendDtsJobRequest
         @return: SuspendDtsJobResponse
         """
         runtime = util_models.RuntimeOptions()
         return self.suspend_dts_job_with_options(request, runtime)
 
     async def suspend_dts_job_async(
         self,
         request: dts_20200101_models.SuspendDtsJobRequest,
     ) -> dts_20200101_models.SuspendDtsJobResponse:
         """
-        ***\
+        @description ***\
         
         @param request: SuspendDtsJobRequest
         @return: SuspendDtsJobResponse
         """
         runtime = util_models.RuntimeOptions()
         return await self.suspend_dts_job_with_options_async(request, runtime)
 
     def suspend_dts_jobs_with_options(
         self,
         request: dts_20200101_models.SuspendDtsJobsRequest,
         runtime: util_models.RuntimeOptions,
     ) -> dts_20200101_models.SuspendDtsJobsResponse:
+        """
+        @param request: SuspendDtsJobsRequest
+        @param runtime: runtime options for this request RuntimeOptions
+        @return: SuspendDtsJobsResponse
+        """
         UtilClient.validate_model(request)
         query = {}
         if not UtilClient.is_unset(request.dts_job_ids):
             query['DtsJobIds'] = request.dts_job_ids
         if not UtilClient.is_unset(request.region_id):
             query['RegionId'] = request.region_id
         if not UtilClient.is_unset(request.resource_group_id):
@@ -11667,14 +13220,19 @@
         )
 
     async def suspend_dts_jobs_with_options_async(
         self,
         request: dts_20200101_models.SuspendDtsJobsRequest,
         runtime: util_models.RuntimeOptions,
     ) -> dts_20200101_models.SuspendDtsJobsResponse:
+        """
+        @param request: SuspendDtsJobsRequest
+        @param runtime: runtime options for this request RuntimeOptions
+        @return: SuspendDtsJobsResponse
+        """
         UtilClient.validate_model(request)
         query = {}
         if not UtilClient.is_unset(request.dts_job_ids):
             query['DtsJobIds'] = request.dts_job_ids
         if not UtilClient.is_unset(request.region_id):
             query['RegionId'] = request.region_id
         if not UtilClient.is_unset(request.resource_group_id):
@@ -11700,33 +13258,41 @@
             await self.call_api_async(params, req, runtime)
         )
 
     def suspend_dts_jobs(
         self,
         request: dts_20200101_models.SuspendDtsJobsRequest,
     ) -> dts_20200101_models.SuspendDtsJobsResponse:
+        """
+        @param request: SuspendDtsJobsRequest
+        @return: SuspendDtsJobsResponse
+        """
         runtime = util_models.RuntimeOptions()
         return self.suspend_dts_jobs_with_options(request, runtime)
 
     async def suspend_dts_jobs_async(
         self,
         request: dts_20200101_models.SuspendDtsJobsRequest,
     ) -> dts_20200101_models.SuspendDtsJobsResponse:
+        """
+        @param request: SuspendDtsJobsRequest
+        @return: SuspendDtsJobsResponse
+        """
         runtime = util_models.RuntimeOptions()
         return await self.suspend_dts_jobs_with_options_async(request, runtime)
 
     def suspend_migration_job_with_options(
         self,
         request: dts_20200101_models.SuspendMigrationJobRequest,
         runtime: util_models.RuntimeOptions,
     ) -> dts_20200101_models.SuspendMigrationJobResponse:
         """
-        >
-        *   If a data migration task is performing incremental data migration, we recommend that you do not pause the task for more than 6 hours. Otherwise, you will not be able to call the [StartMigrationJob](~~49429~~) operation to restart the task.
-        *   If you select incremental data migration as the migration type for a pay-as-you-go instance, DTS charges a fee even when the task is paused. This is because DTS only stops writing data to the destination database. DTS continues to pull the logs of the source database so that the task can resume quickly after it is restarted. Therefore, incremental data migration consumes resources such as the bandwidth of the source database.
+        @description >
+        If a data migration task is performing incremental data migration, we recommend that you do not pause the task for more than 6 hours. Otherwise, you will not be able to call the [StartMigrationJob](https://help.aliyun.com/document_detail/49429.html) operation to restart the task.
+        If you select incremental data migration as the migration type for a pay-as-you-go instance, DTS charges a fee even when the task is paused. This is because DTS only stops writing data to the destination database. DTS continues to pull the logs of the source database so that the task can resume quickly after it is restarted. Therefore, incremental data migration consumes resources such as the bandwidth of the source database.
         
         @param request: SuspendMigrationJobRequest
         @param runtime: runtime options for this request RuntimeOptions
         @return: SuspendMigrationJobResponse
         """
         UtilClient.validate_model(request)
         query = {}
@@ -11763,17 +13329,17 @@
 
     async def suspend_migration_job_with_options_async(
         self,
         request: dts_20200101_models.SuspendMigrationJobRequest,
         runtime: util_models.RuntimeOptions,
     ) -> dts_20200101_models.SuspendMigrationJobResponse:
         """
-        >
-        *   If a data migration task is performing incremental data migration, we recommend that you do not pause the task for more than 6 hours. Otherwise, you will not be able to call the [StartMigrationJob](~~49429~~) operation to restart the task.
-        *   If you select incremental data migration as the migration type for a pay-as-you-go instance, DTS charges a fee even when the task is paused. This is because DTS only stops writing data to the destination database. DTS continues to pull the logs of the source database so that the task can resume quickly after it is restarted. Therefore, incremental data migration consumes resources such as the bandwidth of the source database.
+        @description >
+        If a data migration task is performing incremental data migration, we recommend that you do not pause the task for more than 6 hours. Otherwise, you will not be able to call the [StartMigrationJob](https://help.aliyun.com/document_detail/49429.html) operation to restart the task.
+        If you select incremental data migration as the migration type for a pay-as-you-go instance, DTS charges a fee even when the task is paused. This is because DTS only stops writing data to the destination database. DTS continues to pull the logs of the source database so that the task can resume quickly after it is restarted. Therefore, incremental data migration consumes resources such as the bandwidth of the source database.
         
         @param request: SuspendMigrationJobRequest
         @param runtime: runtime options for this request RuntimeOptions
         @return: SuspendMigrationJobResponse
         """
         UtilClient.validate_model(request)
         query = {}
@@ -11809,49 +13375,49 @@
         )
 
     def suspend_migration_job(
         self,
         request: dts_20200101_models.SuspendMigrationJobRequest,
     ) -> dts_20200101_models.SuspendMigrationJobResponse:
         """
-        >
-        *   If a data migration task is performing incremental data migration, we recommend that you do not pause the task for more than 6 hours. Otherwise, you will not be able to call the [StartMigrationJob](~~49429~~) operation to restart the task.
-        *   If you select incremental data migration as the migration type for a pay-as-you-go instance, DTS charges a fee even when the task is paused. This is because DTS only stops writing data to the destination database. DTS continues to pull the logs of the source database so that the task can resume quickly after it is restarted. Therefore, incremental data migration consumes resources such as the bandwidth of the source database.
+        @description >
+        If a data migration task is performing incremental data migration, we recommend that you do not pause the task for more than 6 hours. Otherwise, you will not be able to call the [StartMigrationJob](https://help.aliyun.com/document_detail/49429.html) operation to restart the task.
+        If you select incremental data migration as the migration type for a pay-as-you-go instance, DTS charges a fee even when the task is paused. This is because DTS only stops writing data to the destination database. DTS continues to pull the logs of the source database so that the task can resume quickly after it is restarted. Therefore, incremental data migration consumes resources such as the bandwidth of the source database.
         
         @param request: SuspendMigrationJobRequest
         @return: SuspendMigrationJobResponse
         """
         runtime = util_models.RuntimeOptions()
         return self.suspend_migration_job_with_options(request, runtime)
 
     async def suspend_migration_job_async(
         self,
         request: dts_20200101_models.SuspendMigrationJobRequest,
     ) -> dts_20200101_models.SuspendMigrationJobResponse:
         """
-        >
-        *   If a data migration task is performing incremental data migration, we recommend that you do not pause the task for more than 6 hours. Otherwise, you will not be able to call the [StartMigrationJob](~~49429~~) operation to restart the task.
-        *   If you select incremental data migration as the migration type for a pay-as-you-go instance, DTS charges a fee even when the task is paused. This is because DTS only stops writing data to the destination database. DTS continues to pull the logs of the source database so that the task can resume quickly after it is restarted. Therefore, incremental data migration consumes resources such as the bandwidth of the source database.
+        @description >
+        If a data migration task is performing incremental data migration, we recommend that you do not pause the task for more than 6 hours. Otherwise, you will not be able to call the [StartMigrationJob](https://help.aliyun.com/document_detail/49429.html) operation to restart the task.
+        If you select incremental data migration as the migration type for a pay-as-you-go instance, DTS charges a fee even when the task is paused. This is because DTS only stops writing data to the destination database. DTS continues to pull the logs of the source database so that the task can resume quickly after it is restarted. Therefore, incremental data migration consumes resources such as the bandwidth of the source database.
         
         @param request: SuspendMigrationJobRequest
         @return: SuspendMigrationJobResponse
         """
         runtime = util_models.RuntimeOptions()
         return await self.suspend_migration_job_with_options_async(request, runtime)
 
     def suspend_synchronization_job_with_options(
         self,
         request: dts_20200101_models.SuspendSynchronizationJobRequest,
         runtime: util_models.RuntimeOptions,
     ) -> dts_20200101_models.SuspendSynchronizationJobResponse:
         """
-        >
-        *   When you call this operation, the data synchronization task must be in the Synchronizing state.
-        *   We recommend that you do not pause a data synchronization task for more than 6 hours. Otherwise, the task cannot be started again.
-        *   If the billing method is pay-as-you-go, DTS charges a fee even when the task is paused. This is because DTS only stops writing data to the destination database. DTS continues to pull the logs of the source database so that the task can resume quickly after it is restarted. Therefore, data synchronization consumes resources such as the bandwidth of the source database.
+        @description >
+        When you call this operation, the data synchronization task must be in the Synchronizing state.
+        We recommend that you do not pause a data synchronization task for more than 6 hours. Otherwise, the task cannot be started again.
+        If the billing method is pay-as-you-go, DTS charges a fee even when the task is paused. This is because DTS only stops writing data to the destination database. DTS continues to pull the logs of the source database so that the task can resume quickly after it is restarted. Therefore, data synchronization consumes resources such as the bandwidth of the source database.
         
         @param request: SuspendSynchronizationJobRequest
         @param runtime: runtime options for this request RuntimeOptions
         @return: SuspendSynchronizationJobResponse
         """
         UtilClient.validate_model(request)
         query = {}
@@ -11888,18 +13454,18 @@
 
     async def suspend_synchronization_job_with_options_async(
         self,
         request: dts_20200101_models.SuspendSynchronizationJobRequest,
         runtime: util_models.RuntimeOptions,
     ) -> dts_20200101_models.SuspendSynchronizationJobResponse:
         """
-        >
-        *   When you call this operation, the data synchronization task must be in the Synchronizing state.
-        *   We recommend that you do not pause a data synchronization task for more than 6 hours. Otherwise, the task cannot be started again.
-        *   If the billing method is pay-as-you-go, DTS charges a fee even when the task is paused. This is because DTS only stops writing data to the destination database. DTS continues to pull the logs of the source database so that the task can resume quickly after it is restarted. Therefore, data synchronization consumes resources such as the bandwidth of the source database.
+        @description >
+        When you call this operation, the data synchronization task must be in the Synchronizing state.
+        We recommend that you do not pause a data synchronization task for more than 6 hours. Otherwise, the task cannot be started again.
+        If the billing method is pay-as-you-go, DTS charges a fee even when the task is paused. This is because DTS only stops writing data to the destination database. DTS continues to pull the logs of the source database so that the task can resume quickly after it is restarted. Therefore, data synchronization consumes resources such as the bandwidth of the source database.
         
         @param request: SuspendSynchronizationJobRequest
         @param runtime: runtime options for this request RuntimeOptions
         @return: SuspendSynchronizationJobResponse
         """
         UtilClient.validate_model(request)
         query = {}
@@ -11935,46 +13501,53 @@
         )
 
     def suspend_synchronization_job(
         self,
         request: dts_20200101_models.SuspendSynchronizationJobRequest,
     ) -> dts_20200101_models.SuspendSynchronizationJobResponse:
         """
-        >
-        *   When you call this operation, the data synchronization task must be in the Synchronizing state.
-        *   We recommend that you do not pause a data synchronization task for more than 6 hours. Otherwise, the task cannot be started again.
-        *   If the billing method is pay-as-you-go, DTS charges a fee even when the task is paused. This is because DTS only stops writing data to the destination database. DTS continues to pull the logs of the source database so that the task can resume quickly after it is restarted. Therefore, data synchronization consumes resources such as the bandwidth of the source database.
+        @description >
+        When you call this operation, the data synchronization task must be in the Synchronizing state.
+        We recommend that you do not pause a data synchronization task for more than 6 hours. Otherwise, the task cannot be started again.
+        If the billing method is pay-as-you-go, DTS charges a fee even when the task is paused. This is because DTS only stops writing data to the destination database. DTS continues to pull the logs of the source database so that the task can resume quickly after it is restarted. Therefore, data synchronization consumes resources such as the bandwidth of the source database.
         
         @param request: SuspendSynchronizationJobRequest
         @return: SuspendSynchronizationJobResponse
         """
         runtime = util_models.RuntimeOptions()
         return self.suspend_synchronization_job_with_options(request, runtime)
 
     async def suspend_synchronization_job_async(
         self,
         request: dts_20200101_models.SuspendSynchronizationJobRequest,
     ) -> dts_20200101_models.SuspendSynchronizationJobResponse:
         """
-        >
-        *   When you call this operation, the data synchronization task must be in the Synchronizing state.
-        *   We recommend that you do not pause a data synchronization task for more than 6 hours. Otherwise, the task cannot be started again.
-        *   If the billing method is pay-as-you-go, DTS charges a fee even when the task is paused. This is because DTS only stops writing data to the destination database. DTS continues to pull the logs of the source database so that the task can resume quickly after it is restarted. Therefore, data synchronization consumes resources such as the bandwidth of the source database.
+        @description >
+        When you call this operation, the data synchronization task must be in the Synchronizing state.
+        We recommend that you do not pause a data synchronization task for more than 6 hours. Otherwise, the task cannot be started again.
+        If the billing method is pay-as-you-go, DTS charges a fee even when the task is paused. This is because DTS only stops writing data to the destination database. DTS continues to pull the logs of the source database so that the task can resume quickly after it is restarted. Therefore, data synchronization consumes resources such as the bandwidth of the source database.
         
         @param request: SuspendSynchronizationJobRequest
         @return: SuspendSynchronizationJobResponse
         """
         runtime = util_models.RuntimeOptions()
         return await self.suspend_synchronization_job_with_options_async(request, runtime)
 
     def switch_physical_dts_job_to_cloud_with_options(
         self,
         request: dts_20200101_models.SwitchPhysicalDtsJobToCloudRequest,
         runtime: util_models.RuntimeOptions,
     ) -> dts_20200101_models.SwitchPhysicalDtsJobToCloudResponse:
+        """
+        @summary 物理迁移任务切换上云
+        
+        @param request: SwitchPhysicalDtsJobToCloudRequest
+        @param runtime: runtime options for this request RuntimeOptions
+        @return: SwitchPhysicalDtsJobToCloudResponse
+        """
         UtilClient.validate_model(request)
         query = {}
         if not UtilClient.is_unset(request.dts_instance_id):
             query['DtsInstanceId'] = request.dts_instance_id
         if not UtilClient.is_unset(request.dts_job_id):
             query['DtsJobId'] = request.dts_job_id
         if not UtilClient.is_unset(request.region_id):
@@ -12003,14 +13576,21 @@
         )
 
     async def switch_physical_dts_job_to_cloud_with_options_async(
         self,
         request: dts_20200101_models.SwitchPhysicalDtsJobToCloudRequest,
         runtime: util_models.RuntimeOptions,
     ) -> dts_20200101_models.SwitchPhysicalDtsJobToCloudResponse:
+        """
+        @summary 物理迁移任务切换上云
+        
+        @param request: SwitchPhysicalDtsJobToCloudRequest
+        @param runtime: runtime options for this request RuntimeOptions
+        @return: SwitchPhysicalDtsJobToCloudResponse
+        """
         UtilClient.validate_model(request)
         query = {}
         if not UtilClient.is_unset(request.dts_instance_id):
             query['DtsInstanceId'] = request.dts_instance_id
         if not UtilClient.is_unset(request.dts_job_id):
             query['DtsJobId'] = request.dts_job_id
         if not UtilClient.is_unset(request.region_id):
@@ -12038,34 +13618,46 @@
             await self.call_api_async(params, req, runtime)
         )
 
     def switch_physical_dts_job_to_cloud(
         self,
         request: dts_20200101_models.SwitchPhysicalDtsJobToCloudRequest,
     ) -> dts_20200101_models.SwitchPhysicalDtsJobToCloudResponse:
+        """
+        @summary 物理迁移任务切换上云
+        
+        @param request: SwitchPhysicalDtsJobToCloudRequest
+        @return: SwitchPhysicalDtsJobToCloudResponse
+        """
         runtime = util_models.RuntimeOptions()
         return self.switch_physical_dts_job_to_cloud_with_options(request, runtime)
 
     async def switch_physical_dts_job_to_cloud_async(
         self,
         request: dts_20200101_models.SwitchPhysicalDtsJobToCloudRequest,
     ) -> dts_20200101_models.SwitchPhysicalDtsJobToCloudResponse:
+        """
+        @summary 物理迁移任务切换上云
+        
+        @param request: SwitchPhysicalDtsJobToCloudRequest
+        @return: SwitchPhysicalDtsJobToCloudResponse
+        """
         runtime = util_models.RuntimeOptions()
         return await self.switch_physical_dts_job_to_cloud_with_options_async(request, runtime)
 
     def switch_synchronization_endpoint_with_options(
         self,
         request: dts_20200101_models.SwitchSynchronizationEndpointRequest,
         runtime: util_models.RuntimeOptions,
     ) -> dts_20200101_models.SwitchSynchronizationEndpointResponse:
         """
-        If the source or destination database is a self-managed MySQL database connected over the Internet, Elastic Compute Service (ECS) or Express Connect, you must call this operation to update the connection settings.
-        *   If the source or destination database is hosted on an ApsaraDB instance (such as ApsaraDB RDS instance and ApsaraDB for MongoDB instance), DTS automatically updates the connection settings. You do not need to call this operation.
-        > *   For two-way synchronization tasks, if you perform a primary/secondary switchover on the source or destination database, you must call this operation twice to update the connection settings.
-        For example, if you perform a primary/secondary switchover on the destination database of the forward direction, you must call this operation twice. In the first call, set the **SynchronizationDirection** parameter to **Forward**, set the **Endpoint.Type **parameter to **Destination**, and configure the connection settings. In the second call, set the **SynchronizationDirection** parameter to **Reverse**, set the **Endpoint.Type **parameter to **Source**, and configure the connection settings.
+        @description    If the source or destination database is a self-managed MySQL database connected over the Internet, Elastic Compute Service (ECS) or Express Connect, you must call this operation to update the connection settings.
+        If the source or destination database is hosted on an ApsaraDB instance (such as ApsaraDB RDS instance and ApsaraDB for MongoDB instance), DTS automatically updates the connection settings. You do not need to call this operation.
+        >    For two-way synchronization tasks, if you perform a primary/secondary switchover on the source or destination database, you must call this operation twice to update the connection settings.
+        For example, if you perform a primary/secondary switchover on the destination database of the forward direction, you must call this operation twice. In the first call, set the *SynchronizationDirection** parameter to **Forward**, set the **Endpoint.Type **parameter to **Destination**, and configure the connection settings. In the second call, set the **SynchronizationDirection** parameter to **Reverse**, set the **Endpoint.Type **parameter to **Source**, and configure the connection settings.
         
         @param request: SwitchSynchronizationEndpointRequest
         @param runtime: runtime options for this request RuntimeOptions
         @return: SwitchSynchronizationEndpointResponse
         """
         UtilClient.validate_model(request)
         query = {}
@@ -12106,18 +13698,18 @@
 
     async def switch_synchronization_endpoint_with_options_async(
         self,
         request: dts_20200101_models.SwitchSynchronizationEndpointRequest,
         runtime: util_models.RuntimeOptions,
     ) -> dts_20200101_models.SwitchSynchronizationEndpointResponse:
         """
-        If the source or destination database is a self-managed MySQL database connected over the Internet, Elastic Compute Service (ECS) or Express Connect, you must call this operation to update the connection settings.
-        *   If the source or destination database is hosted on an ApsaraDB instance (such as ApsaraDB RDS instance and ApsaraDB for MongoDB instance), DTS automatically updates the connection settings. You do not need to call this operation.
-        > *   For two-way synchronization tasks, if you perform a primary/secondary switchover on the source or destination database, you must call this operation twice to update the connection settings.
-        For example, if you perform a primary/secondary switchover on the destination database of the forward direction, you must call this operation twice. In the first call, set the **SynchronizationDirection** parameter to **Forward**, set the **Endpoint.Type **parameter to **Destination**, and configure the connection settings. In the second call, set the **SynchronizationDirection** parameter to **Reverse**, set the **Endpoint.Type **parameter to **Source**, and configure the connection settings.
+        @description    If the source or destination database is a self-managed MySQL database connected over the Internet, Elastic Compute Service (ECS) or Express Connect, you must call this operation to update the connection settings.
+        If the source or destination database is hosted on an ApsaraDB instance (such as ApsaraDB RDS instance and ApsaraDB for MongoDB instance), DTS automatically updates the connection settings. You do not need to call this operation.
+        >    For two-way synchronization tasks, if you perform a primary/secondary switchover on the source or destination database, you must call this operation twice to update the connection settings.
+        For example, if you perform a primary/secondary switchover on the destination database of the forward direction, you must call this operation twice. In the first call, set the *SynchronizationDirection** parameter to **Forward**, set the **Endpoint.Type **parameter to **Destination**, and configure the connection settings. In the second call, set the **SynchronizationDirection** parameter to **Reverse**, set the **Endpoint.Type **parameter to **Source**, and configure the connection settings.
         
         @param request: SwitchSynchronizationEndpointRequest
         @param runtime: runtime options for this request RuntimeOptions
         @return: SwitchSynchronizationEndpointResponse
         """
         UtilClient.validate_model(request)
         query = {}
@@ -12157,53 +13749,53 @@
         )
 
     def switch_synchronization_endpoint(
         self,
         request: dts_20200101_models.SwitchSynchronizationEndpointRequest,
     ) -> dts_20200101_models.SwitchSynchronizationEndpointResponse:
         """
-        If the source or destination database is a self-managed MySQL database connected over the Internet, Elastic Compute Service (ECS) or Express Connect, you must call this operation to update the connection settings.
-        *   If the source or destination database is hosted on an ApsaraDB instance (such as ApsaraDB RDS instance and ApsaraDB for MongoDB instance), DTS automatically updates the connection settings. You do not need to call this operation.
-        > *   For two-way synchronization tasks, if you perform a primary/secondary switchover on the source or destination database, you must call this operation twice to update the connection settings.
-        For example, if you perform a primary/secondary switchover on the destination database of the forward direction, you must call this operation twice. In the first call, set the **SynchronizationDirection** parameter to **Forward**, set the **Endpoint.Type **parameter to **Destination**, and configure the connection settings. In the second call, set the **SynchronizationDirection** parameter to **Reverse**, set the **Endpoint.Type **parameter to **Source**, and configure the connection settings.
+        @description    If the source or destination database is a self-managed MySQL database connected over the Internet, Elastic Compute Service (ECS) or Express Connect, you must call this operation to update the connection settings.
+        If the source or destination database is hosted on an ApsaraDB instance (such as ApsaraDB RDS instance and ApsaraDB for MongoDB instance), DTS automatically updates the connection settings. You do not need to call this operation.
+        >    For two-way synchronization tasks, if you perform a primary/secondary switchover on the source or destination database, you must call this operation twice to update the connection settings.
+        For example, if you perform a primary/secondary switchover on the destination database of the forward direction, you must call this operation twice. In the first call, set the *SynchronizationDirection** parameter to **Forward**, set the **Endpoint.Type **parameter to **Destination**, and configure the connection settings. In the second call, set the **SynchronizationDirection** parameter to **Reverse**, set the **Endpoint.Type **parameter to **Source**, and configure the connection settings.
         
         @param request: SwitchSynchronizationEndpointRequest
         @return: SwitchSynchronizationEndpointResponse
         """
         runtime = util_models.RuntimeOptions()
         return self.switch_synchronization_endpoint_with_options(request, runtime)
 
     async def switch_synchronization_endpoint_async(
         self,
         request: dts_20200101_models.SwitchSynchronizationEndpointRequest,
     ) -> dts_20200101_models.SwitchSynchronizationEndpointResponse:
         """
-        If the source or destination database is a self-managed MySQL database connected over the Internet, Elastic Compute Service (ECS) or Express Connect, you must call this operation to update the connection settings.
-        *   If the source or destination database is hosted on an ApsaraDB instance (such as ApsaraDB RDS instance and ApsaraDB for MongoDB instance), DTS automatically updates the connection settings. You do not need to call this operation.
-        > *   For two-way synchronization tasks, if you perform a primary/secondary switchover on the source or destination database, you must call this operation twice to update the connection settings.
-        For example, if you perform a primary/secondary switchover on the destination database of the forward direction, you must call this operation twice. In the first call, set the **SynchronizationDirection** parameter to **Forward**, set the **Endpoint.Type **parameter to **Destination**, and configure the connection settings. In the second call, set the **SynchronizationDirection** parameter to **Reverse**, set the **Endpoint.Type **parameter to **Source**, and configure the connection settings.
+        @description    If the source or destination database is a self-managed MySQL database connected over the Internet, Elastic Compute Service (ECS) or Express Connect, you must call this operation to update the connection settings.
+        If the source or destination database is hosted on an ApsaraDB instance (such as ApsaraDB RDS instance and ApsaraDB for MongoDB instance), DTS automatically updates the connection settings. You do not need to call this operation.
+        >    For two-way synchronization tasks, if you perform a primary/secondary switchover on the source or destination database, you must call this operation twice to update the connection settings.
+        For example, if you perform a primary/secondary switchover on the destination database of the forward direction, you must call this operation twice. In the first call, set the *SynchronizationDirection** parameter to **Forward**, set the **Endpoint.Type **parameter to **Destination**, and configure the connection settings. In the second call, set the **SynchronizationDirection** parameter to **Reverse**, set the **Endpoint.Type **parameter to **Source**, and configure the connection settings.
         
         @param request: SwitchSynchronizationEndpointRequest
         @return: SwitchSynchronizationEndpointResponse
         """
         runtime = util_models.RuntimeOptions()
         return await self.switch_synchronization_endpoint_with_options_async(request, runtime)
 
     def tag_resources_with_options(
         self,
         request: dts_20200101_models.TagResourcesRequest,
         runtime: util_models.RuntimeOptions,
     ) -> dts_20200101_models.TagResourcesResponse:
         """
-        If you have a large number of instances, you can create multiple tags and bind these tags to the instances. Then, you can filter the instances by tag.
-        *   A tag consists of a key and a value. Each key must be unique in a region for an Alibaba Cloud account. Different keys can be mapped to the same value.
-        *   If the tag that you specify does not exist, this tag is automatically created and bound to the specified instance.
-        *   If the key of the specified tag is the same as that of an existing tag, the specified tag overwrites the existing tag.
-        *   You can bind up to 20 tags to each instance.
-        *   You can bind tags to up to 50 instances in each call.
+        @description If you have a large number of instances, you can create multiple tags and bind these tags to the instances. Then, you can filter the instances by tag.
+        A tag consists of a key and a value. Each key must be unique in a region for an Alibaba Cloud account. Different keys can be mapped to the same value.
+        If the tag that you specify does not exist, this tag is automatically created and bound to the specified instance.
+        If the key of the specified tag is the same as that of an existing tag, the specified tag overwrites the existing tag.
+        You can bind up to 20 tags to each instance.
+        You can bind tags to up to 50 instances in each call.
         
         @param request: TagResourcesRequest
         @param runtime: runtime options for this request RuntimeOptions
         @return: TagResourcesResponse
         """
         UtilClient.validate_model(request)
         query = {}
@@ -12238,20 +13830,20 @@
 
     async def tag_resources_with_options_async(
         self,
         request: dts_20200101_models.TagResourcesRequest,
         runtime: util_models.RuntimeOptions,
     ) -> dts_20200101_models.TagResourcesResponse:
         """
-        If you have a large number of instances, you can create multiple tags and bind these tags to the instances. Then, you can filter the instances by tag.
-        *   A tag consists of a key and a value. Each key must be unique in a region for an Alibaba Cloud account. Different keys can be mapped to the same value.
-        *   If the tag that you specify does not exist, this tag is automatically created and bound to the specified instance.
-        *   If the key of the specified tag is the same as that of an existing tag, the specified tag overwrites the existing tag.
-        *   You can bind up to 20 tags to each instance.
-        *   You can bind tags to up to 50 instances in each call.
+        @description If you have a large number of instances, you can create multiple tags and bind these tags to the instances. Then, you can filter the instances by tag.
+        A tag consists of a key and a value. Each key must be unique in a region for an Alibaba Cloud account. Different keys can be mapped to the same value.
+        If the tag that you specify does not exist, this tag is automatically created and bound to the specified instance.
+        If the key of the specified tag is the same as that of an existing tag, the specified tag overwrites the existing tag.
+        You can bind up to 20 tags to each instance.
+        You can bind tags to up to 50 instances in each call.
         
         @param request: TagResourcesRequest
         @param runtime: runtime options for this request RuntimeOptions
         @return: TagResourcesResponse
         """
         UtilClient.validate_model(request)
         query = {}
@@ -12285,50 +13877,55 @@
         )
 
     def tag_resources(
         self,
         request: dts_20200101_models.TagResourcesRequest,
     ) -> dts_20200101_models.TagResourcesResponse:
         """
-        If you have a large number of instances, you can create multiple tags and bind these tags to the instances. Then, you can filter the instances by tag.
-        *   A tag consists of a key and a value. Each key must be unique in a region for an Alibaba Cloud account. Different keys can be mapped to the same value.
-        *   If the tag that you specify does not exist, this tag is automatically created and bound to the specified instance.
-        *   If the key of the specified tag is the same as that of an existing tag, the specified tag overwrites the existing tag.
-        *   You can bind up to 20 tags to each instance.
-        *   You can bind tags to up to 50 instances in each call.
+        @description If you have a large number of instances, you can create multiple tags and bind these tags to the instances. Then, you can filter the instances by tag.
+        A tag consists of a key and a value. Each key must be unique in a region for an Alibaba Cloud account. Different keys can be mapped to the same value.
+        If the tag that you specify does not exist, this tag is automatically created and bound to the specified instance.
+        If the key of the specified tag is the same as that of an existing tag, the specified tag overwrites the existing tag.
+        You can bind up to 20 tags to each instance.
+        You can bind tags to up to 50 instances in each call.
         
         @param request: TagResourcesRequest
         @return: TagResourcesResponse
         """
         runtime = util_models.RuntimeOptions()
         return self.tag_resources_with_options(request, runtime)
 
     async def tag_resources_async(
         self,
         request: dts_20200101_models.TagResourcesRequest,
     ) -> dts_20200101_models.TagResourcesResponse:
         """
-        If you have a large number of instances, you can create multiple tags and bind these tags to the instances. Then, you can filter the instances by tag.
-        *   A tag consists of a key and a value. Each key must be unique in a region for an Alibaba Cloud account. Different keys can be mapped to the same value.
-        *   If the tag that you specify does not exist, this tag is automatically created and bound to the specified instance.
-        *   If the key of the specified tag is the same as that of an existing tag, the specified tag overwrites the existing tag.
-        *   You can bind up to 20 tags to each instance.
-        *   You can bind tags to up to 50 instances in each call.
+        @description If you have a large number of instances, you can create multiple tags and bind these tags to the instances. Then, you can filter the instances by tag.
+        A tag consists of a key and a value. Each key must be unique in a region for an Alibaba Cloud account. Different keys can be mapped to the same value.
+        If the tag that you specify does not exist, this tag is automatically created and bound to the specified instance.
+        If the key of the specified tag is the same as that of an existing tag, the specified tag overwrites the existing tag.
+        You can bind up to 20 tags to each instance.
+        You can bind tags to up to 50 instances in each call.
         
         @param request: TagResourcesRequest
         @return: TagResourcesResponse
         """
         runtime = util_models.RuntimeOptions()
         return await self.tag_resources_with_options_async(request, runtime)
 
     def transfer_instance_class_with_options(
         self,
         request: dts_20200101_models.TransferInstanceClassRequest,
         runtime: util_models.RuntimeOptions,
     ) -> dts_20200101_models.TransferInstanceClassResponse:
+        """
+        @param request: TransferInstanceClassRequest
+        @param runtime: runtime options for this request RuntimeOptions
+        @return: TransferInstanceClassResponse
+        """
         UtilClient.validate_model(request)
         query = {}
         if not UtilClient.is_unset(request.dts_job_id):
             query['DtsJobId'] = request.dts_job_id
         if not UtilClient.is_unset(request.instance_class):
             query['InstanceClass'] = request.instance_class
         if not UtilClient.is_unset(request.order_type):
@@ -12357,14 +13954,19 @@
         )
 
     async def transfer_instance_class_with_options_async(
         self,
         request: dts_20200101_models.TransferInstanceClassRequest,
         runtime: util_models.RuntimeOptions,
     ) -> dts_20200101_models.TransferInstanceClassResponse:
+        """
+        @param request: TransferInstanceClassRequest
+        @param runtime: runtime options for this request RuntimeOptions
+        @return: TransferInstanceClassResponse
+        """
         UtilClient.validate_model(request)
         query = {}
         if not UtilClient.is_unset(request.dts_job_id):
             query['DtsJobId'] = request.dts_job_id
         if not UtilClient.is_unset(request.instance_class):
             query['InstanceClass'] = request.instance_class
         if not UtilClient.is_unset(request.order_type):
@@ -12392,41 +13994,51 @@
             await self.call_api_async(params, req, runtime)
         )
 
     def transfer_instance_class(
         self,
         request: dts_20200101_models.TransferInstanceClassRequest,
     ) -> dts_20200101_models.TransferInstanceClassResponse:
+        """
+        @param request: TransferInstanceClassRequest
+        @return: TransferInstanceClassResponse
+        """
         runtime = util_models.RuntimeOptions()
         return self.transfer_instance_class_with_options(request, runtime)
 
     async def transfer_instance_class_async(
         self,
         request: dts_20200101_models.TransferInstanceClassRequest,
     ) -> dts_20200101_models.TransferInstanceClassResponse:
+        """
+        @param request: TransferInstanceClassRequest
+        @return: TransferInstanceClassResponse
+        """
         runtime = util_models.RuntimeOptions()
         return await self.transfer_instance_class_with_options_async(request, runtime)
 
     def transfer_pay_type_with_options(
         self,
         request: dts_20200101_models.TransferPayTypeRequest,
         runtime: util_models.RuntimeOptions,
     ) -> dts_20200101_models.TransferPayTypeResponse:
         """
-        Before you call this operation, make sure that you fully understand the billing methods and [pricing](https://www.alibabacloud.com/zh/product/data-transmission-service/pricing) of DTS.
-        *   The billing method of subscription instances cannot be changed to pay-as-you-go. To prevent resource waste, determine whether you need to change the billing method of your resources.
-        *   Data migration instances are all pay-as-you-go instances. You do not need to change the billing method of data migration instances.
-        *   After you change the billing method from pay-as-you-go to subscription, the DTS instance is not affected.
+        @description Before you call this operation, make sure that you fully understand the billing methods and [pricing](https://www.alibabacloud.com/zh/product/data-transmission-service/pricing) of DTS.
+        The billing method of subscription instances cannot be changed to pay-as-you-go. To prevent resource waste, determine whether you need to change the billing method of your resources.
+        Data migration instances are all pay-as-you-go instances. You do not need to change the billing method of data migration instances.
+        After you change the billing method from pay-as-you-go to subscription, the DTS instance is not affected.
         
         @param request: TransferPayTypeRequest
         @param runtime: runtime options for this request RuntimeOptions
         @return: TransferPayTypeResponse
         """
         UtilClient.validate_model(request)
         query = {}
+        if not UtilClient.is_unset(request.auto_pay):
+            query['AutoPay'] = request.auto_pay
         if not UtilClient.is_unset(request.buy_count):
             query['BuyCount'] = request.buy_count
         if not UtilClient.is_unset(request.charge_type):
             query['ChargeType'] = request.charge_type
         if not UtilClient.is_unset(request.dts_job_id):
             query['DtsJobId'] = request.dts_job_id
         if not UtilClient.is_unset(request.max_du):
@@ -12460,25 +14072,27 @@
 
     async def transfer_pay_type_with_options_async(
         self,
         request: dts_20200101_models.TransferPayTypeRequest,
         runtime: util_models.RuntimeOptions,
     ) -> dts_20200101_models.TransferPayTypeResponse:
         """
-        Before you call this operation, make sure that you fully understand the billing methods and [pricing](https://www.alibabacloud.com/zh/product/data-transmission-service/pricing) of DTS.
-        *   The billing method of subscription instances cannot be changed to pay-as-you-go. To prevent resource waste, determine whether you need to change the billing method of your resources.
-        *   Data migration instances are all pay-as-you-go instances. You do not need to change the billing method of data migration instances.
-        *   After you change the billing method from pay-as-you-go to subscription, the DTS instance is not affected.
+        @description Before you call this operation, make sure that you fully understand the billing methods and [pricing](https://www.alibabacloud.com/zh/product/data-transmission-service/pricing) of DTS.
+        The billing method of subscription instances cannot be changed to pay-as-you-go. To prevent resource waste, determine whether you need to change the billing method of your resources.
+        Data migration instances are all pay-as-you-go instances. You do not need to change the billing method of data migration instances.
+        After you change the billing method from pay-as-you-go to subscription, the DTS instance is not affected.
         
         @param request: TransferPayTypeRequest
         @param runtime: runtime options for this request RuntimeOptions
         @return: TransferPayTypeResponse
         """
         UtilClient.validate_model(request)
         query = {}
+        if not UtilClient.is_unset(request.auto_pay):
+            query['AutoPay'] = request.auto_pay
         if not UtilClient.is_unset(request.buy_count):
             query['BuyCount'] = request.buy_count
         if not UtilClient.is_unset(request.charge_type):
             query['ChargeType'] = request.charge_type
         if not UtilClient.is_unset(request.dts_job_id):
             query['DtsJobId'] = request.dts_job_id
         if not UtilClient.is_unset(request.max_du):
@@ -12511,48 +14125,48 @@
         )
 
     def transfer_pay_type(
         self,
         request: dts_20200101_models.TransferPayTypeRequest,
     ) -> dts_20200101_models.TransferPayTypeResponse:
         """
-        Before you call this operation, make sure that you fully understand the billing methods and [pricing](https://www.alibabacloud.com/zh/product/data-transmission-service/pricing) of DTS.
-        *   The billing method of subscription instances cannot be changed to pay-as-you-go. To prevent resource waste, determine whether you need to change the billing method of your resources.
-        *   Data migration instances are all pay-as-you-go instances. You do not need to change the billing method of data migration instances.
-        *   After you change the billing method from pay-as-you-go to subscription, the DTS instance is not affected.
+        @description Before you call this operation, make sure that you fully understand the billing methods and [pricing](https://www.alibabacloud.com/zh/product/data-transmission-service/pricing) of DTS.
+        The billing method of subscription instances cannot be changed to pay-as-you-go. To prevent resource waste, determine whether you need to change the billing method of your resources.
+        Data migration instances are all pay-as-you-go instances. You do not need to change the billing method of data migration instances.
+        After you change the billing method from pay-as-you-go to subscription, the DTS instance is not affected.
         
         @param request: TransferPayTypeRequest
         @return: TransferPayTypeResponse
         """
         runtime = util_models.RuntimeOptions()
         return self.transfer_pay_type_with_options(request, runtime)
 
     async def transfer_pay_type_async(
         self,
         request: dts_20200101_models.TransferPayTypeRequest,
     ) -> dts_20200101_models.TransferPayTypeResponse:
         """
-        Before you call this operation, make sure that you fully understand the billing methods and [pricing](https://www.alibabacloud.com/zh/product/data-transmission-service/pricing) of DTS.
-        *   The billing method of subscription instances cannot be changed to pay-as-you-go. To prevent resource waste, determine whether you need to change the billing method of your resources.
-        *   Data migration instances are all pay-as-you-go instances. You do not need to change the billing method of data migration instances.
-        *   After you change the billing method from pay-as-you-go to subscription, the DTS instance is not affected.
+        @description Before you call this operation, make sure that you fully understand the billing methods and [pricing](https://www.alibabacloud.com/zh/product/data-transmission-service/pricing) of DTS.
+        The billing method of subscription instances cannot be changed to pay-as-you-go. To prevent resource waste, determine whether you need to change the billing method of your resources.
+        Data migration instances are all pay-as-you-go instances. You do not need to change the billing method of data migration instances.
+        After you change the billing method from pay-as-you-go to subscription, the DTS instance is not affected.
         
         @param request: TransferPayTypeRequest
         @return: TransferPayTypeResponse
         """
         runtime = util_models.RuntimeOptions()
         return await self.transfer_pay_type_with_options_async(request, runtime)
 
     def untag_resources_with_options(
         self,
         request: dts_20200101_models.UntagResourcesRequest,
         runtime: util_models.RuntimeOptions,
     ) -> dts_20200101_models.UntagResourcesResponse:
         """
-        >  If a tag is unbound from an instance and is not bound to other instances, the tag is deleted.
+        @description >  If a tag is unbound from an instance and is not bound to other instances, the tag is deleted.
         
         @param request: UntagResourcesRequest
         @param runtime: runtime options for this request RuntimeOptions
         @return: UntagResourcesResponse
         """
         UtilClient.validate_model(request)
         query = {}
@@ -12589,15 +14203,15 @@
 
     async def untag_resources_with_options_async(
         self,
         request: dts_20200101_models.UntagResourcesRequest,
         runtime: util_models.RuntimeOptions,
     ) -> dts_20200101_models.UntagResourcesResponse:
         """
-        >  If a tag is unbound from an instance and is not bound to other instances, the tag is deleted.
+        @description >  If a tag is unbound from an instance and is not bound to other instances, the tag is deleted.
         
         @param request: UntagResourcesRequest
         @param runtime: runtime options for this request RuntimeOptions
         @return: UntagResourcesResponse
         """
         UtilClient.validate_model(request)
         query = {}
@@ -12633,47 +14247,47 @@
         )
 
     def untag_resources(
         self,
         request: dts_20200101_models.UntagResourcesRequest,
     ) -> dts_20200101_models.UntagResourcesResponse:
         """
-        >  If a tag is unbound from an instance and is not bound to other instances, the tag is deleted.
+        @description >  If a tag is unbound from an instance and is not bound to other instances, the tag is deleted.
         
         @param request: UntagResourcesRequest
         @return: UntagResourcesResponse
         """
         runtime = util_models.RuntimeOptions()
         return self.untag_resources_with_options(request, runtime)
 
     async def untag_resources_async(
         self,
         request: dts_20200101_models.UntagResourcesRequest,
     ) -> dts_20200101_models.UntagResourcesResponse:
         """
-        >  If a tag is unbound from an instance and is not bound to other instances, the tag is deleted.
+        @description >  If a tag is unbound from an instance and is not bound to other instances, the tag is deleted.
         
         @param request: UntagResourcesRequest
         @return: UntagResourcesResponse
         """
         runtime = util_models.RuntimeOptions()
         return await self.untag_resources_with_options_async(request, runtime)
 
     def upgrade_two_way_with_options(
         self,
         request: dts_20200101_models.UpgradeTwoWayRequest,
         runtime: util_models.RuntimeOptions,
     ) -> dts_20200101_models.UpgradeTwoWayResponse:
         """
-        Before you call this operation, make sure that you fully understand the billing methods and [pricing](https://www.alibabacloud.com/zh/product/data-transmission-service/pricing) of Data Transmission Service (DTS)
+        @description Before you call this operation, make sure that you fully understand the billing methods and [pricing](https://www.alibabacloud.com/zh/product/data-transmission-service/pricing) of Data Transmission Service (DTS)
         When you call this operation, take note of the following information:
-        *   The source and destination databases of the data synchronization task are both **MySQL** databases.
-        *   The synchronization topology of the data synchronization task is **one-way synchronization**.
-        *   The data synchronization task is in the **Synchronizing** state.
-        *   The upgrade operation causes data synchronization latency of about 5 seconds. We recommend that you perform this operation during off-peak hours.
+        The source and destination databases of the data synchronization task are both **MySQL** databases.
+        The synchronization topology of the data synchronization task is **one-way synchronization**.
+        The data synchronization task is in the **Synchronizing** state.
+        The upgrade operation causes data synchronization latency of about 5 seconds. We recommend that you perform this operation during off-peak hours.
         
         @param request: UpgradeTwoWayRequest
         @param runtime: runtime options for this request RuntimeOptions
         @return: UpgradeTwoWayResponse
         """
         UtilClient.validate_model(request)
         query = {}
@@ -12706,20 +14320,20 @@
 
     async def upgrade_two_way_with_options_async(
         self,
         request: dts_20200101_models.UpgradeTwoWayRequest,
         runtime: util_models.RuntimeOptions,
     ) -> dts_20200101_models.UpgradeTwoWayResponse:
         """
-        Before you call this operation, make sure that you fully understand the billing methods and [pricing](https://www.alibabacloud.com/zh/product/data-transmission-service/pricing) of Data Transmission Service (DTS)
+        @description Before you call this operation, make sure that you fully understand the billing methods and [pricing](https://www.alibabacloud.com/zh/product/data-transmission-service/pricing) of Data Transmission Service (DTS)
         When you call this operation, take note of the following information:
-        *   The source and destination databases of the data synchronization task are both **MySQL** databases.
-        *   The synchronization topology of the data synchronization task is **one-way synchronization**.
-        *   The data synchronization task is in the **Synchronizing** state.
-        *   The upgrade operation causes data synchronization latency of about 5 seconds. We recommend that you perform this operation during off-peak hours.
+        The source and destination databases of the data synchronization task are both **MySQL** databases.
+        The synchronization topology of the data synchronization task is **one-way synchronization**.
+        The data synchronization task is in the **Synchronizing** state.
+        The upgrade operation causes data synchronization latency of about 5 seconds. We recommend that you perform this operation during off-peak hours.
         
         @param request: UpgradeTwoWayRequest
         @param runtime: runtime options for this request RuntimeOptions
         @return: UpgradeTwoWayResponse
         """
         UtilClient.validate_model(request)
         query = {}
@@ -12751,52 +14365,55 @@
         )
 
     def upgrade_two_way(
         self,
         request: dts_20200101_models.UpgradeTwoWayRequest,
     ) -> dts_20200101_models.UpgradeTwoWayResponse:
         """
-        Before you call this operation, make sure that you fully understand the billing methods and [pricing](https://www.alibabacloud.com/zh/product/data-transmission-service/pricing) of Data Transmission Service (DTS)
+        @description Before you call this operation, make sure that you fully understand the billing methods and [pricing](https://www.alibabacloud.com/zh/product/data-transmission-service/pricing) of Data Transmission Service (DTS)
         When you call this operation, take note of the following information:
-        *   The source and destination databases of the data synchronization task are both **MySQL** databases.
-        *   The synchronization topology of the data synchronization task is **one-way synchronization**.
-        *   The data synchronization task is in the **Synchronizing** state.
-        *   The upgrade operation causes data synchronization latency of about 5 seconds. We recommend that you perform this operation during off-peak hours.
+        The source and destination databases of the data synchronization task are both **MySQL** databases.
+        The synchronization topology of the data synchronization task is **one-way synchronization**.
+        The data synchronization task is in the **Synchronizing** state.
+        The upgrade operation causes data synchronization latency of about 5 seconds. We recommend that you perform this operation during off-peak hours.
         
         @param request: UpgradeTwoWayRequest
         @return: UpgradeTwoWayResponse
         """
         runtime = util_models.RuntimeOptions()
         return self.upgrade_two_way_with_options(request, runtime)
 
     async def upgrade_two_way_async(
         self,
         request: dts_20200101_models.UpgradeTwoWayRequest,
     ) -> dts_20200101_models.UpgradeTwoWayResponse:
         """
-        Before you call this operation, make sure that you fully understand the billing methods and [pricing](https://www.alibabacloud.com/zh/product/data-transmission-service/pricing) of Data Transmission Service (DTS)
+        @description Before you call this operation, make sure that you fully understand the billing methods and [pricing](https://www.alibabacloud.com/zh/product/data-transmission-service/pricing) of Data Transmission Service (DTS)
         When you call this operation, take note of the following information:
-        *   The source and destination databases of the data synchronization task are both **MySQL** databases.
-        *   The synchronization topology of the data synchronization task is **one-way synchronization**.
-        *   The data synchronization task is in the **Synchronizing** state.
-        *   The upgrade operation causes data synchronization latency of about 5 seconds. We recommend that you perform this operation during off-peak hours.
+        The source and destination databases of the data synchronization task are both **MySQL** databases.
+        The synchronization topology of the data synchronization task is **one-way synchronization**.
+        The data synchronization task is in the **Synchronizing** state.
+        The upgrade operation causes data synchronization latency of about 5 seconds. We recommend that you perform this operation during off-peak hours.
         
         @param request: UpgradeTwoWayRequest
         @return: UpgradeTwoWayResponse
         """
         runtime = util_models.RuntimeOptions()
         return await self.upgrade_two_way_with_options_async(request, runtime)
 
     def white_ip_list_with_options(
         self,
         request: dts_20200101_models.WhiteIpListRequest,
         runtime: util_models.RuntimeOptions,
     ) -> dts_20200101_models.WhiteIpListResponse:
         """
-        The operation that you want to perform. Set the value to *WhiteIpList**.
+        @summary If the *source or destination instance** is a **self-managed database** or a **third-party cloud database**, you need to call this operation to query the CIDR blocks of DTS servers. Then, you need to add the CIDR blocks of DTS servers to the security settings of the source or destination instance, for example, the firewall of your database. For more information, see [Add the CIDR blocks of DTS servers to the security settings of on-premises databases](https://help.aliyun.com/document_detail/176627.html).
+        >  If the *source or destination database** is an **ApsaraDB database instance** (such as RDS instance and ApsaraDB for MongoDB instance) or a **self-managed database hosted on Elastic Compute Service (ECS)**, you do not need to add the CIDR blocks. When you click **Set Whitelist and Next** in the DTS console, DTS automatically adds the CIDR blocks of DTS servers to the security settings of the source or destination instance.
+        
+        @description The operation that you want to perform. Set the value to *WhiteIpList**.
         
         @param request: WhiteIpListRequest
         @param runtime: runtime options for this request RuntimeOptions
         @return: WhiteIpListResponse
         """
         UtilClient.validate_model(request)
         query = {}
@@ -12833,15 +14450,18 @@
 
     async def white_ip_list_with_options_async(
         self,
         request: dts_20200101_models.WhiteIpListRequest,
         runtime: util_models.RuntimeOptions,
     ) -> dts_20200101_models.WhiteIpListResponse:
         """
-        The operation that you want to perform. Set the value to *WhiteIpList**.
+        @summary If the *source or destination instance** is a **self-managed database** or a **third-party cloud database**, you need to call this operation to query the CIDR blocks of DTS servers. Then, you need to add the CIDR blocks of DTS servers to the security settings of the source or destination instance, for example, the firewall of your database. For more information, see [Add the CIDR blocks of DTS servers to the security settings of on-premises databases](https://help.aliyun.com/document_detail/176627.html).
+        >  If the *source or destination database** is an **ApsaraDB database instance** (such as RDS instance and ApsaraDB for MongoDB instance) or a **self-managed database hosted on Elastic Compute Service (ECS)**, you do not need to add the CIDR blocks. When you click **Set Whitelist and Next** in the DTS console, DTS automatically adds the CIDR blocks of DTS servers to the security settings of the source or destination instance.
+        
+        @description The operation that you want to perform. Set the value to *WhiteIpList**.
         
         @param request: WhiteIpListRequest
         @param runtime: runtime options for this request RuntimeOptions
         @return: WhiteIpListResponse
         """
         UtilClient.validate_model(request)
         query = {}
@@ -12877,27 +14497,33 @@
         )
 
     def white_ip_list(
         self,
         request: dts_20200101_models.WhiteIpListRequest,
     ) -> dts_20200101_models.WhiteIpListResponse:
         """
-        The operation that you want to perform. Set the value to *WhiteIpList**.
+        @summary If the *source or destination instance** is a **self-managed database** or a **third-party cloud database**, you need to call this operation to query the CIDR blocks of DTS servers. Then, you need to add the CIDR blocks of DTS servers to the security settings of the source or destination instance, for example, the firewall of your database. For more information, see [Add the CIDR blocks of DTS servers to the security settings of on-premises databases](https://help.aliyun.com/document_detail/176627.html).
+        >  If the *source or destination database** is an **ApsaraDB database instance** (such as RDS instance and ApsaraDB for MongoDB instance) or a **self-managed database hosted on Elastic Compute Service (ECS)**, you do not need to add the CIDR blocks. When you click **Set Whitelist and Next** in the DTS console, DTS automatically adds the CIDR blocks of DTS servers to the security settings of the source or destination instance.
+        
+        @description The operation that you want to perform. Set the value to *WhiteIpList**.
         
         @param request: WhiteIpListRequest
         @return: WhiteIpListResponse
         """
         runtime = util_models.RuntimeOptions()
         return self.white_ip_list_with_options(request, runtime)
 
     async def white_ip_list_async(
         self,
         request: dts_20200101_models.WhiteIpListRequest,
     ) -> dts_20200101_models.WhiteIpListResponse:
         """
-        The operation that you want to perform. Set the value to *WhiteIpList**.
+        @summary If the *source or destination instance** is a **self-managed database** or a **third-party cloud database**, you need to call this operation to query the CIDR blocks of DTS servers. Then, you need to add the CIDR blocks of DTS servers to the security settings of the source or destination instance, for example, the firewall of your database. For more information, see [Add the CIDR blocks of DTS servers to the security settings of on-premises databases](https://help.aliyun.com/document_detail/176627.html).
+        >  If the *source or destination database** is an **ApsaraDB database instance** (such as RDS instance and ApsaraDB for MongoDB instance) or a **self-managed database hosted on Elastic Compute Service (ECS)**, you do not need to add the CIDR blocks. When you click **Set Whitelist and Next** in the DTS console, DTS automatically adds the CIDR blocks of DTS servers to the security settings of the source or destination instance.
+        
+        @description The operation that you want to perform. Set the value to *WhiteIpList**.
         
         @param request: WhiteIpListRequest
         @return: WhiteIpListResponse
         """
         runtime = util_models.RuntimeOptions()
         return await self.white_ip_list_with_options_async(request, runtime)
```

#### encoding

```diff
@@ -1 +1 @@
-us-ascii
+utf-8
```

### Comparing `alibabacloud_dts20200101-5.6.0/alibabacloud_dts20200101/models.py` & `alibabacloud_dts20200101-5.6.1/alibabacloud_dts20200101/models.py`

 * *Files 2% similar despite different names*

```diff
@@ -66,21 +66,25 @@
         # The type of the task. Valid values:
         # 
         # *   **MIGRATION**: data migration task
         # *   **SYNC**: data synchronization task
         self.checkpoint = checkpoint
         # The HTTP status code.
         self.data_check_configure = data_check_configure
-        # The objects that you want to migrate or synchronize. The value is a JSON string. For more information, see [Objects of DTS tasks](~~209545~~).
+        # The objects that you want to migrate or synchronize. The value is a JSON string. For more information, see [Objects of DTS tasks](https://help.aliyun.com/document_detail/209545.html).
+        # 
+        # This parameter is required.
         self.data_initialization = data_initialization
-        # The reserved parameter of DTS. The value is a JSON string. You can specify this parameter to add more configurations of the source or destination instance to the DTS task. For example, you can specify the data storage format of the destination Kafka database and the ID of the CEN instance. For more information, see [Reserve](~~273111~~).
+        # The reserved parameter of DTS. The value is a JSON string. You can specify this parameter to add more configurations of the source or destination instance to the DTS task. For example, you can specify the data storage format of the destination Kafka database and the ID of the CEN instance. For more information, see [Reserve](https://help.aliyun.com/document_detail/273111.html).
+        # 
+        # This parameter is required.
         self.data_synchronization = data_synchronization
         # The start offset of incremental data migration or synchronization. The value is a UNIX timestamp. Unit: seconds.
         self.db_list = db_list
-        # The data verification task for a data migration or synchronization instance. The value is a JSON string that indicates parameter limits or alert configurations. For more information, see [DataCheckConfigure](~~459023~~).
+        # The data verification task for a data migration or synchronization instance. The value is a JSON string that indicates parameter limits or alert configurations. For more information, see [DataCheckConfigure](https://help.aliyun.com/document_detail/459023.html).
         self.dedicated_cluster_id = dedicated_cluster_id
         # Specifies whether to monitor the task status. Valid values:
         # 
         # *   **true**: monitors the task status.
         # *   **false**: does not monitor the task status.
         self.delay_notice = delay_notice
         # Specifies whether to monitor the task latency. Valid values:
@@ -88,33 +92,33 @@
         # *   **true**: monitors the task latency.
         # *   **false**: does not monitor the task latency.
         self.delay_phone = delay_phone
         # The mobile numbers that receive status-related alerts. Separate multiple mobile numbers with commas (,).
         # 
         # > 
         # *   This parameter is available only for China site (aliyun.com) users. Only mobile numbers in the Chinese mainland are supported. Up to 10 mobile numbers can be specified.
-        # *   International site (alibabacloud.com) users cannot receive alerts by using mobile phones, but can [set alert rules for DTS tasks in the CloudMonitor console](~~175876~~).
+        # *   International site (alibabacloud.com) users cannot receive alerts by using mobile phones, but can [set alert rules for DTS tasks in the CloudMonitor console](https://help.aliyun.com/document_detail/175876.html).
         self.delay_rule_time = delay_rule_time
         self.dest_ca_certificate_oss_url = dest_ca_certificate_oss_url
         self.dest_ca_certificate_password = dest_ca_certificate_password
         # The password of the destination database account.
         # 
-        # >  If the destination database is a MaxCompute project, you must specify the AccessKey secret of your Alibaba Cloud account. For information about how to obtain your AccessKey pair, see [Create an AccessKey pair](~~116401~~).
+        # >  If the destination database is a MaxCompute project, you must specify the AccessKey secret of your Alibaba Cloud account. For information about how to obtain your AccessKey pair, see [Create an AccessKey pair](https://help.aliyun.com/document_detail/116401.html).
         self.destination_endpoint_data_base_name = destination_endpoint_data_base_name
         # The IP address of the destination instance.
         # 
         # >  If the **DestinationEndpointInstanceType** parameter is set to **OTHER**, **EXPRESS**, **DG**, or **CEN**, this parameter is available and required.
         self.destination_endpoint_engine_name = destination_endpoint_engine_name
         # The name of the database to which the objects migrated to the destination instance belong.
         # 
         # > 
         # *   If the destination instance is a PolarDB for Oracle cluster, an AnalyticDB for PostgreSQL instance, a PostgreSQL database, a MaxCompute project, or a MongoDB database, this parameter is available and required.
         # *   If the destination instance is a MaxCompute project, you must specify the ID of the MaxCompute project.
         self.destination_endpoint_ip = destination_endpoint_ip
-        # The ID of the region in which the destination instance resides. For more information, see [List of supported regions](~~141033~~).
+        # The ID of the region in which the destination instance resides. For more information, see [List of supported regions](https://help.aliyun.com/document_detail/141033.html).
         # 
         # >  If the destination instance is an Alibaba Cloud database instance, this parameter is required.
         self.destination_endpoint_instance_id = destination_endpoint_instance_id
         # The database engine of the destination instance. Valid values:
         # 
         # *   **MySQL**: ApsaraDB RDS for MySQL instance or self-managed MySQL database
         # *   **MARIADB**: ApsaraDB RDS for MariaDB instance
@@ -136,32 +140,34 @@
         # *   **ODPS**: MaxCompute project
         # *   **Tablestore**: Tablestore instance
         # *   **ELK**: Elasticsearch cluster
         # *   **REDIS**: ApsaraDB for Redis instance or self-managed Redis database
         # 
         # > 
         # *   Default value: **MYSQL**.
-        # *   If the DestinationEndpointEngineName parameter is set to **KAFKA**, **MONGODB**, or **PolarDB**, you must also specify the database information in the Reserve parameter. For more information, see [Reserve](~~273111~~).
+        # *   If the DestinationEndpointEngineName parameter is set to **KAFKA**, **MONGODB**, or **PolarDB**, you must also specify the database information in the Reserve parameter. For more information, see [Reserve](https://help.aliyun.com/document_detail/273111.html).
+        # 
+        # This parameter is required.
         self.destination_endpoint_instance_type = destination_endpoint_instance_type
         # The ID of the data migration or synchronization task.
         # 
-        # >  You must specify at least one of the DtsJobId and **DtsInstanceId** parameters. You can call the [DescribeDtsJobs](~~209702~~) operation to query the task ID.
+        # >  You must specify at least one of the DtsJobId and **DtsInstanceId** parameters. You can call the [DescribeDtsJobs](https://help.aliyun.com/document_detail/209702.html) operation to query the task ID.
         self.destination_endpoint_oracle_sid = destination_endpoint_oracle_sid
         self.destination_endpoint_owner_id = destination_endpoint_owner_id
         # Specifies whether to perform full data migration or synchronization. Default value: true. Valid values:
         # 
         # *   **true**: performs full data migration or synchronization.
         # *   **false**: does not perform full data migration or synchronization.
         self.destination_endpoint_password = destination_endpoint_password
         # The database account of the destination database.
         # 
         # > 
         # *   In most cases, this parameter is required.
-        # *   The permissions that are required for the database account vary with the migration or synchronization scenario. For more information, see [Prepare the database accounts for data migration](~~175878~~) or [Prepare the database accounts for data synchronization](~~213152~~).
-        # *   If the destination database is a MaxCompute project, you must specify the AccessKey ID of your Alibaba Cloud account. For information about how to obtain your AccessKey pair, see [Create an AccessKey pair](~~116401~~).
+        # *   The permissions that are required for the database account vary with the migration or synchronization scenario. For more information, see [Prepare the database accounts for data migration](https://help.aliyun.com/document_detail/175878.html) or [Prepare the database accounts for data synchronization](https://help.aliyun.com/document_detail/213152.html).
+        # *   If the destination database is a MaxCompute project, you must specify the AccessKey ID of your Alibaba Cloud account. For information about how to obtain your AccessKey pair, see [Create an AccessKey pair](https://help.aliyun.com/document_detail/116401.html).
         self.destination_endpoint_port = destination_endpoint_port
         # The database service port of the destination instance.
         # 
         # >  If the destination instance is a self-managed database, this parameter is available and required.
         self.destination_endpoint_region = destination_endpoint_region
         self.destination_endpoint_role = destination_endpoint_role
         # Specifies whether to perform schema migration or synchronization. Default value: true. Valid values:
@@ -176,29 +182,31 @@
         # 
         # >  If the **DelayNotice** parameter is set to **true**, this parameter is required.
         self.dts_instance_id = dts_instance_id
         # The mobile numbers that receive latency-related alerts. Separate multiple mobile numbers with commas (,).
         # 
         # > 
         # *   This parameter is available only for China site (aliyun.com) users. Only mobile numbers in the Chinese mainland are supported. Up to 10 mobile numbers can be specified.
-        # *   International site (alibabacloud.com) users cannot receive alerts by using mobile phones, but can [set alert rules for DTS tasks in the CloudMonitor console](~~175876~~).
+        # *   International site (alibabacloud.com) users cannot receive alerts by using mobile phones, but can [set alert rules for DTS tasks in the CloudMonitor console](https://help.aliyun.com/document_detail/175876.html).
         self.dts_job_id = dts_job_id
         # The ID of the source instance.
         # 
         # If the source instance is an Alibaba Cloud database instance, you must specify the ID of the database instance. For example, if the source instance is an ApsaraDB RDS for MySQL instance, you must specify the ID of the ApsaraDB RDS for MySQL instance.
         # 
         # If the source instance is a self-managed database, the value of this parameter varies with the value of the **SourceEndpointInstanceType** parameter.****\
         # 
         # *   If the SourceEndpointInstanceType parameter is set to **ECS**, you must specify the ID of the ECS instance.
         # *   If the SourceEndpointInstanceType parameter is set to **DG**, you must specify the ID of the database gateway.
         # *   If the SourceEndpointInstanceType parameter is set to **EXPRESS** or **CEN**, you must specify the ID of the VPC that is connected to the source instance.
         # 
-        # >  If the SourceEndpointInstanceType parameter is set to **CEN**, you must also specify the ID of the CEN instance in the Reserve parameter. For more information, see [Reserve](~~273111~~).
+        # >  If the SourceEndpointInstanceType parameter is set to **CEN**, you must also specify the ID of the CEN instance in the Reserve parameter. For more information, see [Reserve](https://help.aliyun.com/document_detail/273111.html).
+        # 
+        # This parameter is required.
         self.dts_job_name = dts_job_name
-        # The ID of the region in which the DTS instance resides. For more information, see [List of supported regions](~~141033~~).
+        # The ID of the region in which the DTS instance resides. For more information, see [List of supported regions](https://help.aliyun.com/document_detail/141033.html).
         self.error_notice = error_notice
         # The synchronization direction. Valid values:
         # 
         # *   **Forward**: Data is synchronized from the source database to the destination database.
         # *   **Reverse**: Data is synchronized from the destination database to the source database.
         # 
         # > 
@@ -208,15 +216,17 @@
         # Specifies whether the instance is a disaster recovery instance.
         # 
         # *   **true**: The instance is a disaster recovery instance.
         # *   **false**: The instance is not a disaster recovery instance.
         self.file_oss_url = file_oss_url
         # The ID of the data migration or synchronization instance.
         # 
-        # >  You must specify at least one of the **DtsJobId** and DtsInstanceId parameters. You can call the [DescribeDtsJobs](~~209702~~) operation to query the instance ID.
+        # >  You must specify at least one of the **DtsJobId** and DtsInstanceId parameters. You can call the [DescribeDtsJobs](https://help.aliyun.com/document_detail/209702.html) operation to query the instance ID.
+        # 
+        # This parameter is required.
         self.job_type = job_type
         self.max_du = max_du
         self.min_du = min_du
         self.owner_id = owner_id
         # The URL of the Object Storage Service (OSS) bucket that stores the files related to the DTS task.
         self.region_id = region_id
         # The SID of the Oracle database.
@@ -230,15 +240,15 @@
         # 
         # >  If the **SourceEndpointInstanceType** parameter is set to **OTHER**, **EXPRESS**, **DG**, or **CEN**, this parameter is available and required.
         self.source_endpoint_engine_name = source_endpoint_engine_name
         # The system ID (SID) of the Oracle database.
         # 
         # >  If the **SourceEndpointEngineName** parameter is set to **ORACLE** and the **Oracle** database is deployed in an architecture that is not a Real Application Cluster (RAC), this parameter is available and required.
         self.source_endpoint_ip = source_endpoint_ip
-        # The ID of the region in which the source instance resides. For more information, see [List of supported regions](~~141033~~).
+        # The ID of the region in which the source instance resides. For more information, see [List of supported regions](https://help.aliyun.com/document_detail/141033.html).
         # 
         # >  If the source instance is an Alibaba Cloud database instance, this parameter is required.
         self.source_endpoint_instance_id = source_endpoint_instance_id
         # The database engine of the source instance. Valid values:
         # 
         # *   **MYSQL**: ApsaraDB RDS for MySQL instance or self-managed MySQL database
         # *   **MARIADB**: ApsaraDB RDS for MariaDB instance
@@ -256,21 +266,23 @@
         # *   **HBASE**: self-managed HBase database
         # *   **TERADATA**: Teradata database
         # *   **TiDB**: TiDB database
         # *   **REDIS**: ApsaraDB for Redis instance or self-managed Redis database
         # 
         # > 
         # *   Default value: **MYSQL**.
-        # *   If the SourceEndpointEngineName parameter is set to **MONGODB**, you must also specify the architecture type of the MongoDB database in the Reserve parameter. For more information, see [Reserve](~~273111~~).
+        # *   If the SourceEndpointEngineName parameter is set to **MONGODB**, you must also specify the architecture type of the MongoDB database in the Reserve parameter. For more information, see [Reserve](https://help.aliyun.com/document_detail/273111.html).
+        # 
+        # This parameter is required.
         self.source_endpoint_instance_type = source_endpoint_instance_type
         # The database account of the source database.
         # 
         # > 
         # *   In most cases, this parameter is required.
-        # *   The permissions that are required for the database account vary with the migration or synchronization scenario. For more information, see [Prepare the database accounts for data migration](~~175878~~) or [Prepare the database accounts for data synchronization](~~213152~~).
+        # *   The permissions that are required for the database account vary with the migration or synchronization scenario. For more information, see [Prepare the database accounts for data migration](https://help.aliyun.com/document_detail/175878.html) or [Prepare the database accounts for data synchronization](https://help.aliyun.com/document_detail/213152.html).
         self.source_endpoint_oracle_sid = source_endpoint_oracle_sid
         # The type of the destination instance. Valid values:
         # 
         # **Alibaba Cloud database instances**\
         # 
         # *   **RDS**: ApsaraDB RDS for MySQL instance, ApsaraDB RDS for SQL Server instance, ApsaraDB RDS for PostgreSQL instance, or ApsaraDB RDS for MariaDB instance
         # *   **PolarDB**: PolarDB for MySQL cluster
@@ -292,20 +304,20 @@
         # *   **EXPRESS**: self-managed database connected over Express Connect
         # *   **CEN**: self-managed database connected over CEN
         # *   **DG**: self-managed database connected over Database Gateway
         # 
         # > 
         # *   If the destination instance is a PolarDB for Oracle cluster, you must set this parameter to **OTHER** or **EXPRESS** because you can use a PolarDB for Oracle cluster only as a self-managed database connected over the Internet or Express Connect.
         # *   If the destination instance is a Message Queue for Apache Kafka instance, you must set this parameter to **ECS** or **EXPRESS** because you can use a Message Queue for Apache Kafka instance only as a self-managed database connected over ECS or Express Connect.
-        # *   For more information, see [Supported databases](~~176064~~).
-        # *   If the destination instance is a self-managed database, you must deploy the network environment for the database. For more information, see [Preparation overview](~~146958~~).
+        # *   For more information, see [Supported databases](https://help.aliyun.com/document_detail/176064.html).
+        # *   If the destination instance is a self-managed database, you must deploy the network environment for the database. For more information, see [Preparation overview](https://help.aliyun.com/document_detail/146958.html).
         self.source_endpoint_owner_id = source_endpoint_owner_id
         # The name of the RAM role configured for the Alibaba Cloud account that owns the source instance.
         # 
-        # >  This parameter is required when you migrate or synchronize data across different Alibaba Cloud accounts. For information about the permissions and authorization methods of the RAM role, see [Configure RAM authorization for cross-account data migration and synchronization](~~48468~~).
+        # >  This parameter is required when you migrate or synchronize data across different Alibaba Cloud accounts. For information about the permissions and authorization methods of the RAM role, see [Configure RAM authorization for cross-account data migration and synchronization](https://help.aliyun.com/document_detail/48468.html).
         self.source_endpoint_password = source_endpoint_password
         # The name of the database to which the objects to be migrated in the source instance belong.
         # 
         # >  If the source instance is a PolarDB for Oracle cluster, a PostgreSQL database, or a MongoDB database, this parameter is available and required.
         self.source_endpoint_port = source_endpoint_port
         # The database service port of the source instance.
         # 
@@ -317,28 +329,30 @@
         # 
         # If the destination instance is a self-managed database, the value of this parameter varies with the value of the **DestinationEndpointInstanceType** parameter.****\
         # 
         # *   If the DestinationEndpointInstanceType parameter is set to **ECS**, you must specify the ID of the ECS instance.
         # *   If the DestinationEndpointInstanceType parameter is set to **DG**, you must specify the ID of the database gateway.
         # *   If the DestinationEndpointInstanceType parameter is set to **EXPRESS** or **CEN**, you must specify the ID of the VPC that is connected to the source instance.
         # 
-        # >  If the DestinationEndpointInstanceType parameter is set to **CEN**, you must also specify the ID of the CEN instance in the Reserve parameter. For more information, see [Reserve](~~273111~~).
+        # >  If the DestinationEndpointInstanceType parameter is set to **CEN**, you must also specify the ID of the CEN instance in the Reserve parameter. For more information, see [Reserve](https://help.aliyun.com/document_detail/273111.html).
         self.source_endpoint_role = source_endpoint_role
         # The ID of the Alibaba Cloud account to which the source instance belongs.
         # 
         # >  You can specify this parameter to migrate or synchronize data across different Alibaba Cloud accounts. In this case, you must specify the **SourceEndpointRole** parameter.
         self.source_endpoint_user_name = source_endpoint_user_name
         # 数据投递链路交换机实例id
         self.source_endpoint_vswitch_id = source_endpoint_vswitch_id
         self.src_ca_certificate_oss_url = src_ca_certificate_oss_url
         self.src_ca_certificate_password = src_ca_certificate_password
         # Specifies whether to perform incremental data migration or synchronization. Default value: false. Valid values:
         # 
         # *   **false**: does not perform incremental data migration or synchronization.
         # *   **true**: performs incremental data migration or synchronization.
+        # 
+        # This parameter is required.
         self.structure_initialization = structure_initialization
         # The ID of the DTS dedicated cluster on which the task runs.
         # 
         # >  If this parameter is specified, the task is scheduled to the specified DTS dedicated cluster.
         self.synchronization_direction = synchronization_direction
 
     def validate(self):
@@ -639,21 +653,25 @@
         # The type of the task. Valid values:
         # 
         # *   **MIGRATION**: data migration task
         # *   **SYNC**: data synchronization task
         self.checkpoint = checkpoint
         # The HTTP status code.
         self.data_check_configure = data_check_configure
-        # The objects that you want to migrate or synchronize. The value is a JSON string. For more information, see [Objects of DTS tasks](~~209545~~).
+        # The objects that you want to migrate or synchronize. The value is a JSON string. For more information, see [Objects of DTS tasks](https://help.aliyun.com/document_detail/209545.html).
+        # 
+        # This parameter is required.
         self.data_initialization = data_initialization
-        # The reserved parameter of DTS. The value is a JSON string. You can specify this parameter to add more configurations of the source or destination instance to the DTS task. For example, you can specify the data storage format of the destination Kafka database and the ID of the CEN instance. For more information, see [Reserve](~~273111~~).
+        # The reserved parameter of DTS. The value is a JSON string. You can specify this parameter to add more configurations of the source or destination instance to the DTS task. For example, you can specify the data storage format of the destination Kafka database and the ID of the CEN instance. For more information, see [Reserve](https://help.aliyun.com/document_detail/273111.html).
+        # 
+        # This parameter is required.
         self.data_synchronization = data_synchronization
         # The start offset of incremental data migration or synchronization. The value is a UNIX timestamp. Unit: seconds.
         self.db_list = db_list
-        # The data verification task for a data migration or synchronization instance. The value is a JSON string that indicates parameter limits or alert configurations. For more information, see [DataCheckConfigure](~~459023~~).
+        # The data verification task for a data migration or synchronization instance. The value is a JSON string that indicates parameter limits or alert configurations. For more information, see [DataCheckConfigure](https://help.aliyun.com/document_detail/459023.html).
         self.dedicated_cluster_id = dedicated_cluster_id
         # Specifies whether to monitor the task status. Valid values:
         # 
         # *   **true**: monitors the task status.
         # *   **false**: does not monitor the task status.
         self.delay_notice = delay_notice
         # Specifies whether to monitor the task latency. Valid values:
@@ -661,33 +679,33 @@
         # *   **true**: monitors the task latency.
         # *   **false**: does not monitor the task latency.
         self.delay_phone = delay_phone
         # The mobile numbers that receive status-related alerts. Separate multiple mobile numbers with commas (,).
         # 
         # > 
         # *   This parameter is available only for China site (aliyun.com) users. Only mobile numbers in the Chinese mainland are supported. Up to 10 mobile numbers can be specified.
-        # *   International site (alibabacloud.com) users cannot receive alerts by using mobile phones, but can [set alert rules for DTS tasks in the CloudMonitor console](~~175876~~).
+        # *   International site (alibabacloud.com) users cannot receive alerts by using mobile phones, but can [set alert rules for DTS tasks in the CloudMonitor console](https://help.aliyun.com/document_detail/175876.html).
         self.delay_rule_time = delay_rule_time
         self.dest_ca_certificate_oss_url = dest_ca_certificate_oss_url
         self.dest_ca_certificate_password = dest_ca_certificate_password
         # The password of the destination database account.
         # 
-        # >  If the destination database is a MaxCompute project, you must specify the AccessKey secret of your Alibaba Cloud account. For information about how to obtain your AccessKey pair, see [Create an AccessKey pair](~~116401~~).
+        # >  If the destination database is a MaxCompute project, you must specify the AccessKey secret of your Alibaba Cloud account. For information about how to obtain your AccessKey pair, see [Create an AccessKey pair](https://help.aliyun.com/document_detail/116401.html).
         self.destination_endpoint_data_base_name = destination_endpoint_data_base_name
         # The IP address of the destination instance.
         # 
         # >  If the **DestinationEndpointInstanceType** parameter is set to **OTHER**, **EXPRESS**, **DG**, or **CEN**, this parameter is available and required.
         self.destination_endpoint_engine_name = destination_endpoint_engine_name
         # The name of the database to which the objects migrated to the destination instance belong.
         # 
         # > 
         # *   If the destination instance is a PolarDB for Oracle cluster, an AnalyticDB for PostgreSQL instance, a PostgreSQL database, a MaxCompute project, or a MongoDB database, this parameter is available and required.
         # *   If the destination instance is a MaxCompute project, you must specify the ID of the MaxCompute project.
         self.destination_endpoint_ip = destination_endpoint_ip
-        # The ID of the region in which the destination instance resides. For more information, see [List of supported regions](~~141033~~).
+        # The ID of the region in which the destination instance resides. For more information, see [List of supported regions](https://help.aliyun.com/document_detail/141033.html).
         # 
         # >  If the destination instance is an Alibaba Cloud database instance, this parameter is required.
         self.destination_endpoint_instance_id = destination_endpoint_instance_id
         # The database engine of the destination instance. Valid values:
         # 
         # *   **MySQL**: ApsaraDB RDS for MySQL instance or self-managed MySQL database
         # *   **MARIADB**: ApsaraDB RDS for MariaDB instance
@@ -709,32 +727,34 @@
         # *   **ODPS**: MaxCompute project
         # *   **Tablestore**: Tablestore instance
         # *   **ELK**: Elasticsearch cluster
         # *   **REDIS**: ApsaraDB for Redis instance or self-managed Redis database
         # 
         # > 
         # *   Default value: **MYSQL**.
-        # *   If the DestinationEndpointEngineName parameter is set to **KAFKA**, **MONGODB**, or **PolarDB**, you must also specify the database information in the Reserve parameter. For more information, see [Reserve](~~273111~~).
+        # *   If the DestinationEndpointEngineName parameter is set to **KAFKA**, **MONGODB**, or **PolarDB**, you must also specify the database information in the Reserve parameter. For more information, see [Reserve](https://help.aliyun.com/document_detail/273111.html).
+        # 
+        # This parameter is required.
         self.destination_endpoint_instance_type = destination_endpoint_instance_type
         # The ID of the data migration or synchronization task.
         # 
-        # >  You must specify at least one of the DtsJobId and **DtsInstanceId** parameters. You can call the [DescribeDtsJobs](~~209702~~) operation to query the task ID.
+        # >  You must specify at least one of the DtsJobId and **DtsInstanceId** parameters. You can call the [DescribeDtsJobs](https://help.aliyun.com/document_detail/209702.html) operation to query the task ID.
         self.destination_endpoint_oracle_sid = destination_endpoint_oracle_sid
         self.destination_endpoint_owner_id = destination_endpoint_owner_id
         # Specifies whether to perform full data migration or synchronization. Default value: true. Valid values:
         # 
         # *   **true**: performs full data migration or synchronization.
         # *   **false**: does not perform full data migration or synchronization.
         self.destination_endpoint_password = destination_endpoint_password
         # The database account of the destination database.
         # 
         # > 
         # *   In most cases, this parameter is required.
-        # *   The permissions that are required for the database account vary with the migration or synchronization scenario. For more information, see [Prepare the database accounts for data migration](~~175878~~) or [Prepare the database accounts for data synchronization](~~213152~~).
-        # *   If the destination database is a MaxCompute project, you must specify the AccessKey ID of your Alibaba Cloud account. For information about how to obtain your AccessKey pair, see [Create an AccessKey pair](~~116401~~).
+        # *   The permissions that are required for the database account vary with the migration or synchronization scenario. For more information, see [Prepare the database accounts for data migration](https://help.aliyun.com/document_detail/175878.html) or [Prepare the database accounts for data synchronization](https://help.aliyun.com/document_detail/213152.html).
+        # *   If the destination database is a MaxCompute project, you must specify the AccessKey ID of your Alibaba Cloud account. For information about how to obtain your AccessKey pair, see [Create an AccessKey pair](https://help.aliyun.com/document_detail/116401.html).
         self.destination_endpoint_port = destination_endpoint_port
         # The database service port of the destination instance.
         # 
         # >  If the destination instance is a self-managed database, this parameter is available and required.
         self.destination_endpoint_region = destination_endpoint_region
         self.destination_endpoint_role = destination_endpoint_role
         # Specifies whether to perform schema migration or synchronization. Default value: true. Valid values:
@@ -749,29 +769,31 @@
         # 
         # >  If the **DelayNotice** parameter is set to **true**, this parameter is required.
         self.dts_instance_id = dts_instance_id
         # The mobile numbers that receive latency-related alerts. Separate multiple mobile numbers with commas (,).
         # 
         # > 
         # *   This parameter is available only for China site (aliyun.com) users. Only mobile numbers in the Chinese mainland are supported. Up to 10 mobile numbers can be specified.
-        # *   International site (alibabacloud.com) users cannot receive alerts by using mobile phones, but can [set alert rules for DTS tasks in the CloudMonitor console](~~175876~~).
+        # *   International site (alibabacloud.com) users cannot receive alerts by using mobile phones, but can [set alert rules for DTS tasks in the CloudMonitor console](https://help.aliyun.com/document_detail/175876.html).
         self.dts_job_id = dts_job_id
         # The ID of the source instance.
         # 
         # If the source instance is an Alibaba Cloud database instance, you must specify the ID of the database instance. For example, if the source instance is an ApsaraDB RDS for MySQL instance, you must specify the ID of the ApsaraDB RDS for MySQL instance.
         # 
         # If the source instance is a self-managed database, the value of this parameter varies with the value of the **SourceEndpointInstanceType** parameter.****\
         # 
         # *   If the SourceEndpointInstanceType parameter is set to **ECS**, you must specify the ID of the ECS instance.
         # *   If the SourceEndpointInstanceType parameter is set to **DG**, you must specify the ID of the database gateway.
         # *   If the SourceEndpointInstanceType parameter is set to **EXPRESS** or **CEN**, you must specify the ID of the VPC that is connected to the source instance.
         # 
-        # >  If the SourceEndpointInstanceType parameter is set to **CEN**, you must also specify the ID of the CEN instance in the Reserve parameter. For more information, see [Reserve](~~273111~~).
+        # >  If the SourceEndpointInstanceType parameter is set to **CEN**, you must also specify the ID of the CEN instance in the Reserve parameter. For more information, see [Reserve](https://help.aliyun.com/document_detail/273111.html).
+        # 
+        # This parameter is required.
         self.dts_job_name = dts_job_name
-        # The ID of the region in which the DTS instance resides. For more information, see [List of supported regions](~~141033~~).
+        # The ID of the region in which the DTS instance resides. For more information, see [List of supported regions](https://help.aliyun.com/document_detail/141033.html).
         self.error_notice = error_notice
         # The synchronization direction. Valid values:
         # 
         # *   **Forward**: Data is synchronized from the source database to the destination database.
         # *   **Reverse**: Data is synchronized from the destination database to the source database.
         # 
         # > 
@@ -781,15 +803,17 @@
         # Specifies whether the instance is a disaster recovery instance.
         # 
         # *   **true**: The instance is a disaster recovery instance.
         # *   **false**: The instance is not a disaster recovery instance.
         self.file_oss_url_object = file_oss_url_object
         # The ID of the data migration or synchronization instance.
         # 
-        # >  You must specify at least one of the **DtsJobId** and DtsInstanceId parameters. You can call the [DescribeDtsJobs](~~209702~~) operation to query the instance ID.
+        # >  You must specify at least one of the **DtsJobId** and DtsInstanceId parameters. You can call the [DescribeDtsJobs](https://help.aliyun.com/document_detail/209702.html) operation to query the instance ID.
+        # 
+        # This parameter is required.
         self.job_type = job_type
         self.max_du = max_du
         self.min_du = min_du
         self.owner_id = owner_id
         # The URL of the Object Storage Service (OSS) bucket that stores the files related to the DTS task.
         self.region_id = region_id
         # The SID of the Oracle database.
@@ -803,15 +827,15 @@
         # 
         # >  If the **SourceEndpointInstanceType** parameter is set to **OTHER**, **EXPRESS**, **DG**, or **CEN**, this parameter is available and required.
         self.source_endpoint_engine_name = source_endpoint_engine_name
         # The system ID (SID) of the Oracle database.
         # 
         # >  If the **SourceEndpointEngineName** parameter is set to **ORACLE** and the **Oracle** database is deployed in an architecture that is not a Real Application Cluster (RAC), this parameter is available and required.
         self.source_endpoint_ip = source_endpoint_ip
-        # The ID of the region in which the source instance resides. For more information, see [List of supported regions](~~141033~~).
+        # The ID of the region in which the source instance resides. For more information, see [List of supported regions](https://help.aliyun.com/document_detail/141033.html).
         # 
         # >  If the source instance is an Alibaba Cloud database instance, this parameter is required.
         self.source_endpoint_instance_id = source_endpoint_instance_id
         # The database engine of the source instance. Valid values:
         # 
         # *   **MYSQL**: ApsaraDB RDS for MySQL instance or self-managed MySQL database
         # *   **MARIADB**: ApsaraDB RDS for MariaDB instance
@@ -829,21 +853,23 @@
         # *   **HBASE**: self-managed HBase database
         # *   **TERADATA**: Teradata database
         # *   **TiDB**: TiDB database
         # *   **REDIS**: ApsaraDB for Redis instance or self-managed Redis database
         # 
         # > 
         # *   Default value: **MYSQL**.
-        # *   If the SourceEndpointEngineName parameter is set to **MONGODB**, you must also specify the architecture type of the MongoDB database in the Reserve parameter. For more information, see [Reserve](~~273111~~).
+        # *   If the SourceEndpointEngineName parameter is set to **MONGODB**, you must also specify the architecture type of the MongoDB database in the Reserve parameter. For more information, see [Reserve](https://help.aliyun.com/document_detail/273111.html).
+        # 
+        # This parameter is required.
         self.source_endpoint_instance_type = source_endpoint_instance_type
         # The database account of the source database.
         # 
         # > 
         # *   In most cases, this parameter is required.
-        # *   The permissions that are required for the database account vary with the migration or synchronization scenario. For more information, see [Prepare the database accounts for data migration](~~175878~~) or [Prepare the database accounts for data synchronization](~~213152~~).
+        # *   The permissions that are required for the database account vary with the migration or synchronization scenario. For more information, see [Prepare the database accounts for data migration](https://help.aliyun.com/document_detail/175878.html) or [Prepare the database accounts for data synchronization](https://help.aliyun.com/document_detail/213152.html).
         self.source_endpoint_oracle_sid = source_endpoint_oracle_sid
         # The type of the destination instance. Valid values:
         # 
         # **Alibaba Cloud database instances**\
         # 
         # *   **RDS**: ApsaraDB RDS for MySQL instance, ApsaraDB RDS for SQL Server instance, ApsaraDB RDS for PostgreSQL instance, or ApsaraDB RDS for MariaDB instance
         # *   **PolarDB**: PolarDB for MySQL cluster
@@ -865,20 +891,20 @@
         # *   **EXPRESS**: self-managed database connected over Express Connect
         # *   **CEN**: self-managed database connected over CEN
         # *   **DG**: self-managed database connected over Database Gateway
         # 
         # > 
         # *   If the destination instance is a PolarDB for Oracle cluster, you must set this parameter to **OTHER** or **EXPRESS** because you can use a PolarDB for Oracle cluster only as a self-managed database connected over the Internet or Express Connect.
         # *   If the destination instance is a Message Queue for Apache Kafka instance, you must set this parameter to **ECS** or **EXPRESS** because you can use a Message Queue for Apache Kafka instance only as a self-managed database connected over ECS or Express Connect.
-        # *   For more information, see [Supported databases](~~176064~~).
-        # *   If the destination instance is a self-managed database, you must deploy the network environment for the database. For more information, see [Preparation overview](~~146958~~).
+        # *   For more information, see [Supported databases](https://help.aliyun.com/document_detail/176064.html).
+        # *   If the destination instance is a self-managed database, you must deploy the network environment for the database. For more information, see [Preparation overview](https://help.aliyun.com/document_detail/146958.html).
         self.source_endpoint_owner_id = source_endpoint_owner_id
         # The name of the RAM role configured for the Alibaba Cloud account that owns the source instance.
         # 
-        # >  This parameter is required when you migrate or synchronize data across different Alibaba Cloud accounts. For information about the permissions and authorization methods of the RAM role, see [Configure RAM authorization for cross-account data migration and synchronization](~~48468~~).
+        # >  This parameter is required when you migrate or synchronize data across different Alibaba Cloud accounts. For information about the permissions and authorization methods of the RAM role, see [Configure RAM authorization for cross-account data migration and synchronization](https://help.aliyun.com/document_detail/48468.html).
         self.source_endpoint_password = source_endpoint_password
         # The name of the database to which the objects to be migrated in the source instance belong.
         # 
         # >  If the source instance is a PolarDB for Oracle cluster, a PostgreSQL database, or a MongoDB database, this parameter is available and required.
         self.source_endpoint_port = source_endpoint_port
         # The database service port of the source instance.
         # 
@@ -890,28 +916,30 @@
         # 
         # If the destination instance is a self-managed database, the value of this parameter varies with the value of the **DestinationEndpointInstanceType** parameter.****\
         # 
         # *   If the DestinationEndpointInstanceType parameter is set to **ECS**, you must specify the ID of the ECS instance.
         # *   If the DestinationEndpointInstanceType parameter is set to **DG**, you must specify the ID of the database gateway.
         # *   If the DestinationEndpointInstanceType parameter is set to **EXPRESS** or **CEN**, you must specify the ID of the VPC that is connected to the source instance.
         # 
-        # >  If the DestinationEndpointInstanceType parameter is set to **CEN**, you must also specify the ID of the CEN instance in the Reserve parameter. For more information, see [Reserve](~~273111~~).
+        # >  If the DestinationEndpointInstanceType parameter is set to **CEN**, you must also specify the ID of the CEN instance in the Reserve parameter. For more information, see [Reserve](https://help.aliyun.com/document_detail/273111.html).
         self.source_endpoint_role = source_endpoint_role
         # The ID of the Alibaba Cloud account to which the source instance belongs.
         # 
         # >  You can specify this parameter to migrate or synchronize data across different Alibaba Cloud accounts. In this case, you must specify the **SourceEndpointRole** parameter.
         self.source_endpoint_user_name = source_endpoint_user_name
         # 数据投递链路交换机实例id
         self.source_endpoint_vswitch_id = source_endpoint_vswitch_id
         self.src_ca_certificate_oss_url = src_ca_certificate_oss_url
         self.src_ca_certificate_password = src_ca_certificate_password
         # Specifies whether to perform incremental data migration or synchronization. Default value: false. Valid values:
         # 
         # *   **false**: does not perform incremental data migration or synchronization.
         # *   **true**: performs incremental data migration or synchronization.
+        # 
+        # This parameter is required.
         self.structure_initialization = structure_initialization
         # The ID of the DTS dedicated cluster on which the task runs.
         # 
         # >  If this parameter is specified, the task is scheduled to the specified DTS dedicated cluster.
         self.synchronization_direction = synchronization_direction
 
     def validate(self):
@@ -1300,32 +1328,34 @@
         # *   **MongoDB**: ApsaraDB for MongoDB instance
         # *   **Redis**: ApsaraDB for Redis instance
         # *   **PetaData**: HybridDB for MySQL instance
         # *   **POLARDB**: PolarDB for MySQL cluster or PolarDB for PostgreSQL cluster
         # *   **PolarDB_o**: PolarDB O Edition cluster
         # *   **AnalyticDB**: AnalyticDB for MySQL cluster V3.0 or V2.0
         # *   **Greenplum**: AnalyticDB for PostgreSQL instance
+        # 
+        # This parameter is required.
         self.instance_type = instance_type
         # The SID of the Oracle database.
         # 
         # >  You must specify this parameter only if the **DestinationEndpoint.EngineName** parameter is set to **Oracle** and the **Oracle** database is deployed in a non-RAC architecture.
         self.oracle_sid = oracle_sid
         # The password of the destination database account.
         self.password = password
         # The service port number of the destination database.
         # 
         # >  You must specify the service port number only if the **DestinationEndpoint.InstanceType** parameter is set to **ECS**, **LocalInstance**, or **Express**.
         self.port = port
         # The region ID of the destination database.
         # 
-        # >  If the **DestinationEndpoint.InstanceType** parameter is set to **LocalInstance**, you can enter **cn-hangzhou** or the ID of the region closest to the self-managed database. For more information, see [List of supported regions](~~141033~~).
+        # >  If the **DestinationEndpoint.InstanceType** parameter is set to **LocalInstance**, you can enter **cn-hangzhou** or the ID of the region closest to the self-managed database. For more information, see [List of supported regions](https://help.aliyun.com/document_detail/141033.html).
         self.region = region
         # The database account of the destination database.
         # 
-        # >  The permissions that are required for database accounts vary with the migration scenario. For more information, see [Overview of data migration scenarios](~~26618~~).
+        # >  The permissions that are required for database accounts vary with the migration scenario. For more information, see [Overview of data migration scenarios](https://help.aliyun.com/document_detail/26618.html).
         self.user_name = user_name
 
     def validate(self):
         pass
 
     def to_map(self):
         _map = super().to_map()
@@ -1388,29 +1418,35 @@
         structure_intialization: bool = None,
     ):
         # Specifies whether to perform full data migration. Valid values:
         # 
         # *   **true**: yes
         # *   **false**: no
         # 
-        # >  For more information about databases that support full data migration, see [Supported databases and migration types](~~26618~~).
+        # >  For more information about databases that support full data migration, see [Supported databases and migration types](https://help.aliyun.com/document_detail/26618.html).
+        # 
+        # This parameter is required.
         self.data_intialization = data_intialization
         # Specifies whether to perform incremental data migration. Valid values:
         # 
         # *   **true**: yes
         # *   **false**: no
         # 
-        # >  For more information about databases that support incremental data migration, see [Supported databases and migration types](~~26618~~).
+        # >  For more information about databases that support incremental data migration, see [Supported databases and migration types](https://help.aliyun.com/document_detail/26618.html).
+        # 
+        # This parameter is required.
         self.data_synchronization = data_synchronization
         # Specifies whether to perform schema migration. Valid values:
         # 
         # *   **true**: yes
         # *   **false**: no
         # 
-        # >  For more information about databases that support schema migration, see [Supported databases and migration types](~~26618~~).
+        # >  For more information about databases that support schema migration, see [Supported databases and migration types](https://help.aliyun.com/document_detail/26618.html).
+        # 
+        # This parameter is required.
         self.structure_intialization = structure_intialization
 
     def validate(self):
         pass
 
     def to_map(self):
         _map = super().to_map()
@@ -1480,14 +1516,16 @@
         # *   **LocalInstance**: self-managed database with a public IP address
         # *   **Express**: self-managed database that is connected over Express Connect, VPN Gateway, or Smart Access Gateway
         # *   **dg**: self-managed database that is connected over Database Gateway
         # *   **cen**: self-managed database that is connected over Cloud Enterprise Network (CEN)
         # *   **MongoDB**: ApsaraDB for MongoDB instance
         # *   **POLARDB**: PolarDB for MySQL cluster or PolarDB for PostgreSQL cluster
         # *   **PolarDB_o**: PolarDB O Edition cluster
+        # 
+        # This parameter is required.
         self.instance_type = instance_type
         # The system ID (SID) of the Oracle database.
         # 
         # >  You must specify this parameter only if the **SourceEndpoint.EngineName** parameter is set to **Oracle** and the **Oracle** database is deployed in a non-RAC architecture.
         self.oracle_sid = oracle_sid
         # The ID of the Alibaba Cloud account to which the source instance belongs.
         # 
@@ -1497,23 +1535,23 @@
         self.password = password
         # The service port number of the source database.
         # 
         # >  You must specify the service port number only if the **SourceEndpoint.InstanceType** parameter is set to **ECS**, **LocalInstance**, or **Express**.
         self.port = port
         # The region ID of the source database.
         # 
-        # >  If the **SourceEndpoint.InstanceType** parameter is set to **LocalInstance**, you can enter **cn-hangzhou** or the ID of the region closest to the self-managed database. For more information, see [List of supported regions](~~141033~~).
+        # >  If the **SourceEndpoint.InstanceType** parameter is set to **LocalInstance**, you can enter **cn-hangzhou** or the ID of the region closest to the self-managed database. For more information, see [List of supported regions](https://help.aliyun.com/document_detail/141033.html).
         self.region = region
         # The authorized RAM role of the source instance. You must specify the RAM role only if the source instance and the destination instance belong to different Alibaba Cloud accounts. You can use the RAM role to allow the Alibaba Cloud account that owns the destination instance to access the source instance.
         # 
-        # >  For information about the permissions and authorization methods of the RAM role, see [Configure RAM authorization for cross-account data migration and synchronization](~~48468~~).
+        # >  For information about the permissions and authorization methods of the RAM role, see [Configure RAM authorization for cross-account data migration and synchronization](https://help.aliyun.com/document_detail/48468.html).
         self.role = role
         # The database account of the source database.
         # 
-        # >  The permissions that are required for database accounts vary with the migration scenario. For more information, see [Overview of data migration scenarios](~~26618~~).
+        # >  The permissions that are required for database accounts vary with the migration scenario. For more information, see [Overview of data migration scenarios](https://help.aliyun.com/document_detail/26618.html).
         self.user_name = user_name
 
     def validate(self):
         pass
 
     def to_map(self):
         _map = super().to_map()
@@ -1596,25 +1634,31 @@
         self.migration_mode = migration_mode
         self.source_endpoint = source_endpoint
         # The ID of the Alibaba Cloud account. You do not need to specify this parameter because this parameter will be removed in the future.
         self.account_id = account_id
         # The start offset of incremental data migration. The value is a UNIX timestamp. Unit: seconds.
         self.checkpoint = checkpoint
         # The ID of the data migration instance. You can call the **DescribeMigrationJobs** operation to query the instance ID.
+        # 
+        # This parameter is required.
         self.migration_job_id = migration_job_id
         # The name of the data migration task. The name can be up to 32 characters in length. We recommend that you specify an informative name to identify the task. You do not need to use a unique task name.
+        # 
+        # This parameter is required.
         self.migration_job_name = migration_job_name
         # The objects that you want to migrate. The value is a JSON string and can contain regular expressions.
         # 
-        # For more information, see [MigrationObject](~~141227~~).
+        # For more information, see [MigrationObject](https://help.aliyun.com/document_detail/141227.html).
+        # 
+        # This parameter is required.
         self.migration_object = migration_object
-        # The reserved parameter of DTS. The value is a JSON string. You can specify this parameter to meet special requirements, for example, whether to automatically start a precheck. For more information, see [MigrationReserved](~~176470~~).
+        # The reserved parameter of DTS. The value is a JSON string. You can specify this parameter to meet special requirements, for example, whether to automatically start a precheck. For more information, see [MigrationReserved](https://help.aliyun.com/document_detail/176470.html).
         self.migration_reserved = migration_reserved
         self.owner_id = owner_id
-        # The ID of the region where the data migration instance resides. For more information, see [List of supported regions](~~141033~~).
+        # The ID of the region where the data migration instance resides. For more information, see [List of supported regions](https://help.aliyun.com/document_detail/141033.html).
         # 
         # >  The region ID of the data migration instance is the same as that of the destination database.
         self.region_id = region_id
         self.resource_group_id = resource_group_id
 
     def validate(self):
         if self.destination_endpoint:
@@ -1794,15 +1838,15 @@
     ):
         # The ID of the Alibaba Cloud account. You do not need to specify this parameter because this parameter will be removed in the future.
         self.account_id = account_id
         # The mobile phone numbers that receive latency-related alerts. Separate mobile phone numbers with commas (,).
         # 
         # > 
         # *   This parameter is available only for China site (aliyun.com) users. Only mobile phone numbers in the Chinese mainland are supported. Up to 10 mobile phone numbers can be specified.
-        # *   International site (alibabacloud.com) users cannot receive alerts by using mobile phones, but can [set alert rules for DTS tasks in the Cloud Monitor console](~~175876~~).
+        # *   International site (alibabacloud.com) users cannot receive alerts by using mobile phones, but can [set alert rules for DTS tasks in the Cloud Monitor console](https://help.aliyun.com/document_detail/175876.html).
         self.delay_alert_phone = delay_alert_phone
         # Specifies whether to monitor task latency. Valid values:
         # 
         # *   **enable**: yes
         # *   **disable**: no
         # 
         # > 
@@ -1813,27 +1857,29 @@
         # 
         # >  If the **DelayAlertStatus** parameter is set to **enable**, this parameter must be specified.
         self.delay_over_seconds = delay_over_seconds
         # The mobile phone numbers that receive status-related alerts. Separate mobile phone numbers with commas (,).
         # 
         # > 
         # *   This parameter is available only for China site (aliyun.com) users. Only mobile phone numbers in the Chinese mainland are supported. Up to 10 mobile phone numbers can be specified.
-        # *   International site (alibabacloud.com) users cannot receive alerts by using mobile phones, but can [set alert rules for DTS tasks in the Cloud Monitor console](~~175876~~).
+        # *   International site (alibabacloud.com) users cannot receive alerts by using mobile phones, but can [set alert rules for DTS tasks in the Cloud Monitor console](https://help.aliyun.com/document_detail/175876.html).
         self.error_alert_phone = error_alert_phone
         # Specifies whether to monitor task status. Valid values:
         # 
         # *   **enable**: yes
         # *   **disable**: no
         # 
         # > 
         # *   The default value is **enable**.
         # *   You must specify at least one of the **DelayAlertStatus** and ErrorAlertStatus parameters.
         # *   If the task that you monitor enters an abnormal state, an alert is triggered.
         self.error_alert_status = error_alert_status
         # The ID of the data migration instance. You can call the **DescribeMigrationJobs** operation to query the instance ID.
+        # 
+        # This parameter is required.
         self.migration_job_id = migration_job_id
         self.owner_id = owner_id
         self.region_id = region_id
         self.resource_group_id = resource_group_id
 
     def validate(self):
         pass
@@ -2019,58 +2065,64 @@
         subscription_instance_vpcid: str = None,
         subscription_instance_vswitch_id: str = None,
     ):
         # The UNIX timestamp that represents the start time of change tracking. Unit: seconds.
         # 
         # >  You can use a search engine to obtain a UNIX timestamp converter.
         self.checkpoint = checkpoint
-        # The objects for which you want to track data changes. The value must be a JSON string. For more information, see [Objects of DTS tasks](~~209545~~).
+        # The objects for which you want to track data changes. The value must be a JSON string. For more information, see [Objects of DTS tasks](https://help.aliyun.com/document_detail/209545.html).
+        # 
+        # This parameter is required.
         self.db_list = db_list
         # The ID of the DTS dedicated cluster on which the change tracking task is scheduled to run.
         self.dedicated_cluster_id = dedicated_cluster_id
         # Specifies whether to monitor the task latency. Valid values:
         # 
         # *   **true**: monitors the task latency.
         # *   **false**: does not monitor the task latency.
         self.delay_notice = delay_notice
         # The mobile numbers to which latency-related alerts are sent. Separate multiple mobile numbers with commas (,).
         # 
         # > 
         # *   This parameter is available only for users of the China site (aliyun.com). Only mobile numbers in the Chinese mainland are supported. You can specify up to 10 mobile numbers.
-        # *   Users of the international site (alibabacloud.com) cannot receive alerts by using mobile phones, but can [configure alert rules for DTS tasks in the CloudMonitor console](~~175876~~).
+        # *   Users of the international site (alibabacloud.com) cannot receive alerts by using mobile phones, but can [configure alert rules for DTS tasks in the CloudMonitor console](https://help.aliyun.com/document_detail/175876.html).
         self.delay_phone = delay_phone
         # The threshold for triggering latency-related alerts. Unit: seconds. The value must be an integer. You can set the threshold based on your business needs. To prevent jitters caused by network and database overloads, we recommend that you set the threshold to more than 10 seconds.
         # 
         # >  If the **DelayNotice** parameter is set to **true**, this parameter is required.
         self.delay_rule_time = delay_rule_time
         self.dts_bis_label = dts_bis_label
-        # The ID of the change tracking instance. You can call the [DescribeDtsJobs](~~209702~~) operation to query the instance ID.
+        # The ID of the change tracking instance. You can call the [DescribeDtsJobs](https://help.aliyun.com/document_detail/209702.html) operation to query the instance ID.
         self.dts_instance_id = dts_instance_id
-        # The ID of the change tracking task. You can call the [DescribeDtsJobs](~~209702~~) operation to query the task ID.
+        # The ID of the change tracking task. You can call the [DescribeDtsJobs](https://help.aliyun.com/document_detail/209702.html) operation to query the task ID.
         self.dts_job_id = dts_job_id
         # The name of the change tracking task.
         # 
         # >  We recommend that you specify a descriptive name for easy identification. You do not need to use a unique name.
+        # 
+        # This parameter is required.
         self.dts_job_name = dts_job_name
         # Specifies whether to monitor the task status. Valid values:
         # 
         # *   **true**: monitors the task status.
         # *   **false**: does not monitor the task status.
         self.error_notice = error_notice
         # The mobile numbers to which status-related alerts are sent. Separate multiple mobile numbers with commas (,).
         # 
         # > 
         # *   This parameter is available only for users of the China site (aliyun.com). Only mobile numbers in the Chinese mainland are supported. You can specify up to 10 mobile numbers.
-        # *   Users of the international site (alibabacloud.com) cannot receive alerts by using mobile phones, but can [configure alert rules for DTS tasks in the CloudMonitor console](~~175876~~).
+        # *   Users of the international site (alibabacloud.com) cannot receive alerts by using mobile phones, but can [configure alert rules for DTS tasks in the CloudMonitor console](https://help.aliyun.com/document_detail/175876.html).
         self.error_phone = error_phone
         self.max_du = max_du
         self.min_du = min_du
-        # The ID of the region in which the Data Transmission Service (DTS) instance resides. For more information, see [List of supported regions](~~141033~~).
+        # The ID of the region in which the Data Transmission Service (DTS) instance resides. For more information, see [List of supported regions](https://help.aliyun.com/document_detail/141033.html).
+        # 
+        # This parameter is required.
         self.region_id = region_id
-        # The reserved parameter of DTS. The value must be a JSON string. You can specify this parameter to add more configurations of the source or destination database to the DTS task. For example, you can specify the data storage format of the destination Kafka database and the ID of the CEN instance. For more information, see [MigrationReserved](~~176470~~).
+        # The reserved parameter of DTS. The value must be a JSON string. You can specify this parameter to add more configurations of the source or destination database to the DTS task. For example, you can specify the data storage format of the destination Kafka database and the ID of the CEN instance. For more information, see [MigrationReserved](https://help.aliyun.com/document_detail/176470.html).
         self.reserve = reserve
         self.resource_group_id = resource_group_id
         # The name of the source database.
         self.source_endpoint_database_name = source_endpoint_database_name
         # The engine of the source database. Valid values: **MySQL**, **PostgreSQL**, and **Oracle**.
         # 
         # >  If the source database is a self-managed database, you must specify this parameter.
@@ -2104,25 +2156,25 @@
         self.source_endpoint_owner_id = source_endpoint_owner_id
         # The password of the account that is used to connect to the source database.
         self.source_endpoint_password = source_endpoint_password
         # The service port number of the source database.
         # 
         # >  This parameter is required only when the source database is a self-managed database.
         self.source_endpoint_port = source_endpoint_port
-        # The ID of the region in which the source database resides. For more information, see [List of supported regions](~~141033~~).
+        # The ID of the region in which the source database resides. For more information, see [List of supported regions](https://help.aliyun.com/document_detail/141033.html).
         # 
         # >  If the source database is a self-managed database with a public IP address, you can set the value of this parameter to **cn-hangzhou** or the ID of the region that is closest to the region in which the self-managed database resides.
         self.source_endpoint_region = source_endpoint_region
         # The RAM role that is authorized to access the source database. This parameter is required if the source database does not belong to the Alibaba Cloud account that you use to configure the change tracking task. In this case, you must authorize the Alibaba Cloud account to access the source database by using a RAM role.
         # 
-        # >  For more information about the permissions that are required for the RAM role and how to grant the permissions to the RAM role, see [Configure RAM authorization for cross-account data migration and synchronization](~~48468~~).
+        # >  For more information about the permissions that are required for the RAM role and how to grant the permissions to the RAM role, see [Configure RAM authorization for cross-account data migration and synchronization](https://help.aliyun.com/document_detail/48468.html).
         self.source_endpoint_role = source_endpoint_role
         # The username of the account that is used to connect to the source database.
         # 
-        # >  The permissions that are required for the database account vary with the change tracking scenario. For more information, see [Prepare the source database account for change tracking](~~212653~~).
+        # >  The permissions that are required for the database account vary with the change tracking scenario. For more information, see [Prepare the source database account for change tracking](https://help.aliyun.com/document_detail/212653.html).
         self.source_endpoint_user_name = source_endpoint_user_name
         # Specifies whether to track DDL statements. Default value: true. Valid values:
         # 
         # *   **true**: tracks DDL statements.
         # *   **false**: does not track DDL statements.
         self.subscription_data_type_ddl = subscription_data_type_ddl
         # Specifies whether to track DML statements. Default value: true. Valid values:
@@ -2131,14 +2183,16 @@
         # *   **false**: does not track DML statements.
         self.subscription_data_type_dml = subscription_data_type_dml
         # The network type of the change tracking task. Set the value to **vpc**. A value of vpc indicates the Virtual Private Cloud (VPC) network type.
         # 
         # > 
         # *   To use the new version of the change tracking feature, you must specify the SubscriptionInstanceNetworkType parameter. You must also specify the **SubscriptionInstanceVPCId** and **SubscriptionInstanceVSwitchID** parameters. If you do not specify the SubscriptionInstanceNetworkType parameter, the previous version of the change tracking feature is used.
         # *   The previous version of the change tracking feature supports self-managed MySQL databases, ApsaraDB RDS for MySQL instances, and PolarDB-X 1.0 instances. The new version of the change tracking feature supports self-managed MySQL databases, ApsaraDB RDS for MySQL instances, PolarDB for MySQL clusters, and Oracle databases.
+        # 
+        # This parameter is required.
         self.subscription_instance_network_type = subscription_instance_network_type
         # The ID of the VPC in which the change tracking instance is deployed.
         # 
         # >  This parameter is required only when the **SubscriptionInstanceNetworkType** parameter is set to **vpc**.
         self.subscription_instance_vpcid = subscription_instance_vpcid
         # The ID of the vSwitch in the specified VPC.
         # 
@@ -2438,15 +2492,15 @@
         # *   **PolarDB**: PolarDB for MySQL cluster
         # *   **LocalInstance**: self-managed database with a public IP address
         # *   **ECS**: self-managed database hosted on an Elastic Compute Service (ECS) instance
         # *   **Express**: self-managed database connected over Express Connect
         # *   **CEN**: self-managed database connected over Cloud Enterprise Network (CEN)
         # *   **dg**: self-managed database connected over Database Gateway
         # 
-        # >  The engine of a self-managed database can be MySQL or Oracle. You must specify the engine type when you call the [CreateSubscriptionInstance](~~49436~~) operation.
+        # >  The engine of a self-managed database can be MySQL or Oracle. You must specify the engine type when you call the [CreateSubscriptionInstance](https://help.aliyun.com/document_detail/49436.html) operation.
         self.instance_type = instance_type
         # The system ID (SID) of the Oracle database.
         # 
         # >  This parameter is required only when the source database is a self-managed Oracle database and is not deployed in the Real Application Clusters (RAC) architecture.
         self.oracle_sid = oracle_sid
         # The ID of the Alibaba Cloud account to which the source database belongs.
         # 
@@ -2456,19 +2510,19 @@
         self.password = password
         # The service port number of the source database.
         # 
         # >  This parameter is required only when the source database is a self-managed database.
         self.port = port
         # The RAM role that is authorized to access the source database. This parameter is required if the source database does not belong to the Alibaba Cloud account that you use to configure the change tracking instance. In this case, you must authorize the Alibaba Cloud account to access the source database by using a RAM role.
         # 
-        # >  For more information about the permissions that are required for the RAM role and how to grant permissions to the RAM role, see [Configure RAM authorization for cross-account data migration and synchronization](~~48468~~).
+        # >  For more information about the permissions that are required for the RAM role and how to grant permissions to the RAM role, see [Configure RAM authorization for cross-account data migration and synchronization](https://help.aliyun.com/document_detail/48468.html).
         self.role = role
         # The username of the account that is used to connect to the source database.
         # 
-        # >  The permissions that are required for the database account vary with the change tracking scenario. For more information, see [Overview of change tracking scenarios](~~145715~~).
+        # >  The permissions that are required for the database account vary with the change tracking scenario. For more information, see [Overview of change tracking scenarios](https://help.aliyun.com/document_detail/145715.html).
         self.user_name = user_name
 
     def validate(self):
         pass
 
     def to_map(self):
         _map = super().to_map()
@@ -2529,19 +2583,23 @@
         ddl: bool = None,
         dml: bool = None,
     ):
         # Specifies whether to track DDL statements. Default value: true. Valid values:
         # 
         # *   **true**: tracks DDL statements.
         # *   **false**: does not track DDL statements.
+        # 
+        # This parameter is required.
         self.ddl = ddl
         # Specifies whether to track DML statements. Default value: true. Valid values:
         # 
         # *   **true**: tracks DML statements.
         # *   **false**: does not tack DML statements.
+        # 
+        # This parameter is required.
         self.dml = dml
 
     def validate(self):
         pass
 
     def to_map(self):
         _map = super().to_map()
@@ -2622,25 +2680,29 @@
         self.subscription_data_type = subscription_data_type
         self.subscription_instance = subscription_instance
         # The ID of the Alibaba Cloud account. You do not need to specify this parameter because this parameter is discontinued.
         self.account_id = account_id
         self.owner_id = owner_id
         self.region_id = region_id
         self.resource_group_id = resource_group_id
-        # The ID of the region in which the change tracking instance resides. For more information, see [List of supported regions](~~141033~~).
+        # The ID of the region in which the change tracking instance resides. For more information, see [List of supported regions](https://help.aliyun.com/document_detail/141033.html).
+        # 
+        # This parameter is required.
         self.subscription_instance_id = subscription_instance_id
-        # The ID of the change tracking instance. You can call the [DescribeSubscriptionInstances](~~49442~~) operation to query the instance ID.
+        # The ID of the change tracking instance. You can call the [DescribeSubscriptionInstances](https://help.aliyun.com/document_detail/49442.html) operation to query the instance ID.
         self.subscription_instance_name = subscription_instance_name
         # The network type of the change tracking instance. Set the value to **vpc**. A value of vpc indicates the Virtual Private Cloud (VPC) network type.
         # 
         # > 
         # *   To use the new version of the change tracking feature, you must specify the SubscriptionInstanceNetworkType parameter. You must also specify the **SubscriptionInstance.VPCId** and **SubscriptionInstance.VSwitchID** parameters. If you do not specify the SubscriptionInstanceNetworkType parameter, the previous version of the change tracking feature is used.
         # *   The previous version of the change tracking feature supports self-managed MySQL databases, ApsaraDB RDS for MySQL instances, and PolarDB-X 1.0 instances. The new version of the change tracking feature supports self-managed MySQL databases, ApsaraDB RDS for MySQL instances, PolarDB for MySQL clusters, and Oracle databases.
         self.subscription_instance_network_type = subscription_instance_network_type
-        # The objects for which you want to track data changes. The value is a JSON string and can contain regular expressions. For more information, see [SubscriptionObjects](~~141902~~).
+        # The objects for which you want to track data changes. The value is a JSON string and can contain regular expressions. For more information, see [SubscriptionObjects](https://help.aliyun.com/document_detail/141902.html).
+        # 
+        # This parameter is required.
         self.subscription_object = subscription_object
 
     def validate(self):
         if self.source_endpoint:
             self.source_endpoint.validate()
         if self.subscription_data_type:
             self.subscription_data_type.validate()
@@ -2813,15 +2875,15 @@
     ):
         # The ID of the Alibaba Cloud account. You do not need to specify this parameter because this parameter will be removed in the future.
         self.account_id = account_id
         # The mobile phone numbers that receive latency-related alerts. Separate mobile phone numbers with commas (,).
         # 
         # > 
         # *   This parameter is available only for China site (aliyun.com) users. Only mobile phone numbers in the Chinese mainland are supported. Up to 10 mobile phone numbers can be specified.
-        # *   International site (alibabacloud.com) users cannot receive alerts by using mobile phones, but can [set alert rules for DTS tasks in the Cloud Monitor console](~~175876~~).
+        # *   International site (alibabacloud.com) users cannot receive alerts by using mobile phones, but can [set alert rules for DTS tasks in the Cloud Monitor console](https://help.aliyun.com/document_detail/175876.html).
         self.delay_alert_phone = delay_alert_phone
         # Specifies whether to monitor task latency. Valid values:
         # 
         # *   **enable**: yes
         # *   **disable**: no
         # 
         # > 
@@ -2832,15 +2894,15 @@
         # 
         # >  If the **DelayAlertStatus** parameter is set to **enable**, this parameter must be specified.
         self.delay_over_seconds = delay_over_seconds
         # The mobile phone numbers that receive status-related alerts. Separate mobile phone numbers with commas (,).
         # 
         # > 
         # *   This parameter is available only for China site (aliyun.com) users. Only mobile phone numbers in the Chinese mainland are supported. Up to 10 mobile phone numbers can be specified.
-        # *   International site (alibabacloud.com) users cannot receive alerts by using mobile phones, but can [set alert rules for DTS tasks in the Cloud Monitor console](~~175876~~).
+        # *   International site (alibabacloud.com) users cannot receive alerts by using mobile phones, but can [set alert rules for DTS tasks in the Cloud Monitor console](https://help.aliyun.com/document_detail/175876.html).
         self.error_alert_phone = error_alert_phone
         # Specifies whether to monitor task status. Valid values:
         # 
         # *   **enable**: yes
         # *   **disable**: no
         # 
         # > 
@@ -2848,14 +2910,16 @@
         # *   You must specify at least one of the **DelayAlertStatus** and ErrorAlertStatus parameters.
         # *   If the task that you monitor enters an abnormal state, an alert is triggered.
         self.error_alert_status = error_alert_status
         self.owner_id = owner_id
         self.region_id = region_id
         self.resource_group_id = resource_group_id
         # The ID of the change tracking instance. You can call the DescribeSubscriptionInstances operation to query the instance ID.
+        # 
+        # This parameter is required.
         self.subscription_instance_id = subscription_instance_id
 
     def validate(self):
         pass
 
     def to_map(self):
         _map = super().to_map()
@@ -3045,15 +3109,15 @@
         # The service port number of the destination database.
         # 
         # >  You must specify this parameter only if the **DestinationEndpoint.InstanceType** parameter is set to **ECS**, **Express**, **dg**, or **cen**.
         self.port = port
         # The database account of the destination database.
         # 
         # > 
-        # *   The permissions that are required for database accounts vary with the synchronization scenario. For more information, see [Overview of data synchronization scenarios](~~140954~~).
+        # *   The permissions that are required for database accounts vary with the synchronization scenario. For more information, see [Overview of data synchronization scenarios](https://help.aliyun.com/document_detail/140954.html).
         # *   If the **DestinationEndpoint.InstanceType** parameter is set to **ECS**, **Express**, **dg**, or **cen**, you must specify the DestinationEndpoint.UserName parameter.
         # *   If the **DestinationEndpoint.InstanceType** parameter is set to RDS and the database version is MySQL 5.5 or MySQL 5.6, you do not need to specify the DestinationEndpoint.UserName and **DestinationEndpoint.Password** parameters.
         # *   If the **DestinationEndpoint.InstanceType** parameter is set to **Redis**, you do not need to specify the DestinationEndpoint.UserName parameter.
         self.user_name = user_name
 
     def validate(self):
         pass
@@ -3208,22 +3272,22 @@
         self.password = password
         # The service port number of the source database.
         # 
         # >  You must specify this parameter only if the **SourceEndpoint.InstanceType** parameter is set to **ECS**, **Express**, **dg**, or **cen**.
         self.port = port
         # The name of the RAM role configured for the Alibaba Cloud account that owns the source instance.
         # 
-        # >  You must specify this parameter when you synchronize data across different Alibaba Cloud accounts. For information about the permissions and authorization methods of the RAM role, see [Configure RAM authorization for cross-account data migration and synchronization](~~48468~~).
+        # >  You must specify this parameter when you synchronize data across different Alibaba Cloud accounts. For information about the permissions and authorization methods of the RAM role, see [Configure RAM authorization for cross-account data migration and synchronization](https://help.aliyun.com/document_detail/48468.html).
         self.role = role
         # The database account of the source database.
         # 
         # > 
         # *   You must specify this parameter only if the **SourceEndpoint.InstanceType** parameter is set to **ECS**, **Express**, **dg**, or **cen**.
         # *   If the **SourceEndpoint.InstanceType** parameter is set to **Redis**, you do not need to specify the database account.
-        # *   The permissions that are required for database accounts vary with the synchronization scenario. For more information, see [Overview of data synchronization scenarios](~~140954~~).
+        # *   The permissions that are required for database accounts vary with the synchronization scenario. For more information, see [Overview of data synchronization scenarios](https://help.aliyun.com/document_detail/140954.html).
         self.user_name = user_name
 
     def validate(self):
         pass
 
     def to_map(self):
         _map = super().to_map()
@@ -3302,45 +3366,53 @@
         self.checkpoint = checkpoint
         # Specifies whether to perform initial full data synchronization. Valid values:
         # 
         # *   **true**: yes
         # *   **false**: no
         # 
         # >  Default value: **true**.
+        # 
+        # This parameter is required.
         self.data_initialization = data_initialization
-        # The reserved parameter of DTS. The value is a JSON string. You can specify this parameter to meet special requirements, for example, whether to automatically start a precheck. For more information, see [MigrationReserved](~~176470~~).
+        # The reserved parameter of DTS. The value is a JSON string. You can specify this parameter to meet special requirements, for example, whether to automatically start a precheck. For more information, see [MigrationReserved](https://help.aliyun.com/document_detail/176470.html).
         # 
-        # >  This parameter can be used for data synchronization between ApsaraDB for Redis Enterprise Edition instances. For more information, see [Use OpenAPI Explorer to configure one-way or two-way data synchronization between ApsaraDB for Redis Enterprise Edition instances](~~155967~~).
+        # >  This parameter can be used for data synchronization between ApsaraDB for Redis Enterprise Edition instances. For more information, see [Use OpenAPI Explorer to configure one-way or two-way data synchronization between ApsaraDB for Redis Enterprise Edition instances](https://help.aliyun.com/document_detail/155967.html).
         self.migration_reserved = migration_reserved
         self.owner_id = owner_id
         self.region_id = region_id
         self.resource_group_id = resource_group_id
         # Specifies whether to perform initial schema synchronization. Valid values:
         # 
         # *   **true**: yes
         # *   **false**: no
         # 
         # >  Default value: **true**.
+        # 
+        # This parameter is required.
         self.structure_initialization = structure_initialization
         # The synchronization direction. Valid values:
         # 
         # *   **Forward**\
         # *   **Reverse**\
         # 
         # > 
         # *   Default value: **Forward**.
         # *   The value **Reverse** takes effect only if the topology of the data synchronization instance is two-way synchronization.
         self.synchronization_direction = synchronization_direction
-        # The ID of the data synchronization instance. You can call the [DescribeSynchronizationJobs](~~49454~~) operation to query the instance ID.
+        # The ID of the data synchronization instance. You can call the [DescribeSynchronizationJobs](https://help.aliyun.com/document_detail/49454.html) operation to query the instance ID.
+        # 
+        # This parameter is required.
         self.synchronization_job_id = synchronization_job_id
         # The name of the data synchronization task.
         # 
         # >  We recommend that you specify an informative name for easy identification. You do not need to use a unique task name.
         self.synchronization_job_name = synchronization_job_name
-        # The objects that you want to synchronize. The value is a JSON string and can contain regular expressions. For more information, see [SynchronizationObjects](~~141901~~).
+        # The objects that you want to synchronize. The value is a JSON string and can contain regular expressions. For more information, see [SynchronizationObjects](https://help.aliyun.com/document_detail/141901.html).
+        # 
+        # This parameter is required.
         self.synchronization_objects = synchronization_objects
 
     def validate(self):
         if self.destination_endpoint:
             self.destination_endpoint.validate()
         if self.partition_key:
             self.partition_key.validate()
@@ -3530,15 +3602,15 @@
     ):
         # The ID of the Alibaba Cloud account. You do not need to specify this parameter because this parameter will be removed in the future.
         self.account_id = account_id
         # The mobile phone numbers that receive latency-related alerts. Separate mobile phone numbers with commas (,).
         # 
         # > 
         # *   This parameter is available only for China site (aliyun.com) users. Only mobile phone numbers in the Chinese mainland are supported. Up to 10 mobile phone numbers can be specified.
-        # *   International site (alibabacloud.com) users cannot receive alerts by using mobile phones, but can [set alert rules for DTS tasks in the Cloud Monitor console](~~175876~~).
+        # *   International site (alibabacloud.com) users cannot receive alerts by using mobile phones, but can [set alert rules for DTS tasks in the Cloud Monitor console](https://help.aliyun.com/document_detail/175876.html).
         self.delay_alert_phone = delay_alert_phone
         # Specifies whether to monitor task latency. Valid values:
         # 
         # *   **enable**: yes
         # *   **disable**: no
         # 
         # > 
@@ -3549,15 +3621,15 @@
         # 
         # >  If the **DelayAlertStatus** parameter is set to **enable**, this parameter must be specified.
         self.delay_over_seconds = delay_over_seconds
         # The mobile phone numbers that receive status-related alerts. Separate mobile phone numbers with commas (,).
         # 
         # > 
         # *   This parameter is available only for China site (aliyun.com) users. Only mobile phone numbers in the Chinese mainland are supported. Up to 10 mobile phone numbers can be specified.
-        # *   International site (alibabacloud.com) users cannot receive alerts by using mobile phones, but can [set alert rules for DTS tasks in the Cloud Monitor console](~~175876~~).
+        # *   International site (alibabacloud.com) users cannot receive alerts by using mobile phones, but can [set alert rules for DTS tasks in the Cloud Monitor console](https://help.aliyun.com/document_detail/175876.html).
         self.error_alert_phone = error_alert_phone
         # Specifies whether to monitor task status. Valid values:
         # 
         # *   **enable**: yes
         # *   **disable**: no
         # 
         # > 
@@ -3572,14 +3644,16 @@
         # 
         # *   **Forward**\
         # *   **Reverse**\
         # 
         # >  Default value: **Forward**.
         self.synchronization_direction = synchronization_direction
         # The ID of the data synchronization instance. You can call the DescribeSynchronizationJobs operation to query the instance ID.
+        # 
+        # This parameter is required.
         self.synchronization_job_id = synchronization_job_id
 
     def validate(self):
         pass
 
     def to_map(self):
         _map = super().to_map()
@@ -3752,15 +3826,17 @@
         # *   **Forward**\
         # *   **Reverse**\
         # 
         # > 
         # *   Default value: **Forward**.
         # *   This parameter is required only when the topology of the data synchronization instance is two-way synchronization.
         self.synchronization_direction = synchronization_direction
-        # The ID of the data synchronization instance. You can call the [DescribeSynchronizationJobs](~~49454~~) operation to query the instance ID.
+        # The ID of the data synchronization instance. You can call the [DescribeSynchronizationJobs](https://help.aliyun.com/document_detail/49454.html) operation to query the instance ID.
+        # 
+        # This parameter is required.
         self.synchronization_job_id = synchronization_job_id
         # Specifies whether to enable image matching. Valid values:
         # 
         # *   **true**: enables image matching
         # *   **false**: disables image matching
         self.synchronization_replicator_compare_enable = synchronization_replicator_compare_enable
 
@@ -3924,17 +4000,21 @@
         # 
         # *   **MIGRATION**: data migration task
         # *   **SYNC**: data synchronization task
         # *   **SUBSCRIBE**: change tracking task
         self.job_type = job_type
         # The content of the query condition, which corresponds to the value of the JobType parameter.
         self.params = params
-        # One of the query conditions. The ID of the region. For more information, see [Supported regions](~~141033~~).
+        # One of the query conditions. The ID of the region. For more information, see [Supported regions](https://help.aliyun.com/document_detail/141033.html).
+        # 
+        # This parameter is required.
         self.region = region
-        # The ID of the region in which the DTS instance resides. For more information, see [Supported regions](~~141033~~).
+        # The ID of the region in which the DTS instance resides. For more information, see [Supported regions](https://help.aliyun.com/document_detail/141033.html).
+        # 
+        # This parameter is required.
         self.region_id = region_id
         self.resource_group_id = resource_group_id
         # The type of the source database.
         self.src_db_type = src_db_type
         # The status of the DTS task.
         # 
         # Valid values for a data migration task:
@@ -4181,34 +4261,42 @@
         consumer_group_user_name: str = None,
         dts_instance_id: str = None,
         dts_job_id: str = None,
         region_id: str = None,
         resource_group_id: str = None,
     ):
         # The name of the consumer group. The name can be up to 128 characters in length. We recommend that you use an informative name for easy identification.
+        # 
+        # This parameter is required.
         self.consumer_group_name = consumer_group_name
         # The password of the consumer group.
         # 
         # *   A password must contain two or more of the following characters: uppercase letters, lowercase letters, digits, and special characters.
         # *   A password must be 8 to 32 characters in length.
+        # 
+        # This parameter is required.
         self.consumer_group_password = consumer_group_password
         # The username of the consumer group.
         # 
-        # *   A username must contain one or more of the following characters: uppercase letters, lowercase letters, digits, and underscores (\_).
+        # *   A username must contain one or more of the following characters: uppercase letters, lowercase letters, digits, and underscores (_).
         # *   A username cannot exceed 16 characters in length.
+        # 
+        # This parameter is required.
         self.consumer_group_user_name = consumer_group_user_name
-        # The ID of the change tracking instance. You can call the [DescribeDtsJobs](~~209702~~) operation to query the instance ID.
+        # The ID of the change tracking instance. You can call the [DescribeDtsJobs](https://help.aliyun.com/document_detail/209702.html) operation to query the instance ID.
         # 
         # >  You must specify at least one of the **DtsInstanceId** and **DtsJobId**. parameters.
         self.dts_instance_id = dts_instance_id
-        # The ID of the change tracking task. You can call the [DescribeDtsJobs](~~209702~~) operation to query the task ID.
+        # The ID of the change tracking task. You can call the [DescribeDtsJobs](https://help.aliyun.com/document_detail/209702.html) operation to query the task ID.
         # 
         # >  You must specify at least one of the **DtsInstanceId** and **DtsJobId**. parameters.
         self.dts_job_id = dts_job_id
-        # The ID of the region where the change tracking instance resides. For more information, see [List of supported regions](~~141033~~).
+        # The ID of the region where the change tracking instance resides. For more information, see [List of supported regions](https://help.aliyun.com/document_detail/141033.html).
+        # 
+        # This parameter is required.
         self.region_id = region_id
         self.resource_group_id = resource_group_id
 
     def validate(self):
         pass
 
     def to_map(self):
@@ -4367,29 +4455,37 @@
         region_id: str = None,
         resource_group_id: str = None,
         subscription_instance_id: str = None,
     ):
         # The ID of the Alibaba Cloud account. You do not need to specify this parameter because this parameter will be removed in the future.
         self.account_id = account_id
         # The name of the consumer group. The name cannot exceed 128 characters in length. We recommend that you use an informative name for easy identification.
+        # 
+        # This parameter is required.
         self.consumer_group_name = consumer_group_name
         # The password that corresponds to the username of the consumer group.
         # 
         # *   A password must contain two or more of the following characters: uppercase letters, lowercase letters, digits, and special characters.
         # *   A password must be 8 to 32 characters in length.
+        # 
+        # This parameter is required.
         self.consumer_group_password = consumer_group_password
         # The username of the consumer group.
         # 
-        # *   A username must contain one or more of the following characters: uppercase letters, lowercase letters, digits, and underscores (\_).
+        # *   A username must contain one or more of the following characters: uppercase letters, lowercase letters, digits, and underscores (_).
         # *   A username cannot exceed 16 characters in length.
+        # 
+        # This parameter is required.
         self.consumer_group_user_name = consumer_group_user_name
         self.owner_id = owner_id
         self.region_id = region_id
         self.resource_group_id = resource_group_id
         # The ID of the change tracking instance. You can call the DescribeSubscriptionInstances operation to query the instance ID.
+        # 
+        # This parameter is required.
         self.subscription_instance_id = subscription_instance_id
 
     def validate(self):
         pass
 
     def to_map(self):
         _map = super().to_map()
@@ -4547,14 +4643,16 @@
         phones: str = None,
         region_id: str = None,
         resource_group_id: str = None,
     ):
         # The alert threshold for CPU utilization. Unit: percentage.
         self.cpu_alarm_threshold = cpu_alarm_threshold
         # The ID of the cluster.
+        # 
+        # This parameter is required.
         self.dedicated_cluster_id = dedicated_cluster_id
         # The alert threshold for disk usage. Unit: percentage.
         self.disk_alarm_threshold = disk_alarm_threshold
         # The alert threshold for DTS Unit (DU) usage. Unit: percentage.
         self.du_alarm_threshold = du_alarm_threshold
         # The ID of the instance.
         self.instance_id = instance_id
@@ -4563,14 +4661,16 @@
         # Specifies whether to enable the alert feature. Valid values:
         # 
         # *   **1**: enables the alert feature.
         # *   **0**: disables the alert feature.
         self.notice_switch = notice_switch
         self.owner_id = owner_id
         # The mobile phone number to which alerts are sent. Separate multiple mobile phone numbers with commas (,).
+        # 
+        # This parameter is required.
         self.phones = phones
         # The ID of the region in which the Data Transmission Service (DTS) instance resides.
         self.region_id = region_id
         self.resource_group_id = resource_group_id
 
     def validate(self):
         pass
@@ -4792,18 +4892,18 @@
         # *   **DataHub**: DataHub project
         # *   **DB2**: self-managed Db2 for LUW database
         # *   **as400**: AS/400
         # *   **Tablestore**: Tablestore instance
         # 
         # > 
         # *   The default value is **MySQL**.
-        # *   For more information about the supported source and destination databases, see [Overview of data synchronization scenarios](~~130744~~) and [Overview of data migration scenarios](~~26618~~).
+        # *   For more information about the supported source and destination databases, see [Overview of data synchronization scenarios](https://help.aliyun.com/document_detail/130744.html) and [Overview of data migration scenarios](https://help.aliyun.com/document_detail/26618.html).
         # *   You must specify one of this parameter and the **JobId** parameter.
         self.destination_endpoint_engine_name = destination_endpoint_engine_name
-        # The ID of the region in which the destination instance resides. For more information, see [List of supported regions](~~141033~~).
+        # The ID of the region in which the destination instance resides. For more information, see [List of supported regions](https://help.aliyun.com/document_detail/141033.html).
         # 
         # >  You must specify one of this parameter and the **JobId** parameter.
         self.destination_region = destination_region
         # The number of DTS units (DUs) that are assigned to a DTS task that is run on a DTS dedicated cluster. Valid values: **1** to **100**.
         # 
         # > 
         # *   The value of this parameter must be within the range of the number of DUs available for the DTS dedicated cluster.
@@ -4811,15 +4911,15 @@
         # The billing type for a change tracking instance. Valid values: ONLY_CONFIGURATION_FEE and CONFIGURATION_FEE_AND_DATA_FEE. ONLY_CONFIGURATION_FEE: charges only configuration fees. CONFIGURATION_FEE_AND_DATA_FEE: charges configuration fees and data traffic fees.
         self.fee_type = fee_type
         # The instance class.
         # 
         # *   DTS supports the following instance classes for a data migration instance: **xxlarge**, **xlarge**, **large**, **medium**, and **small**.
         # *   DTS supports the following instance classes for a data synchronization instance: **large**, **medium**, **small**, and **micro**.
         # 
-        # >  For more information about the test performance of each instance class, see [Specifications of data migration instances](~~26606~~) and [Specifications of data synchronization instances](~~26605~~).
+        # >  For more information about the test performance of each instance class, see [Specifications of data migration instances](https://help.aliyun.com/document_detail/26606.html) and [Specifications of data synchronization instances](https://help.aliyun.com/document_detail/26605.html).
         self.instance_class = instance_class
         # The ID of the task. You can call the **ConfigureDtsJob** operation to obtain the task ID from the **DtsJobId** parameter.
         # 
         # >  If this parameter is specified, you do not need to specify the **SourceRegion**, **DestinationRegion**, **Type**, **SourceEndpointEngineName**, or **DestinationEndpointEngineName** parameter. Even if these parameters are specified, the value of the **JobId** parameter takes precedence.
         self.job_id = job_id
         self.max_du = max_du
         self.min_du = min_du
@@ -4834,15 +4934,15 @@
         # 
         # >  You must specify this parameter only if the **PayType** parameter is set to **PrePaid**.
         self.period = period
         # The number of DTS instances that you want to purchase.
         # 
         # >  Only a single instance can be purchased each time.
         self.quantity = quantity
-        # The ID of the region in which the DTS instance resides. For more information, see [List of supported regions](~~141033~~).
+        # The ID of the region in which the DTS instance resides. For more information, see [List of supported regions](https://help.aliyun.com/document_detail/141033.html).
         self.region_id = region_id
         # The ID of the resource group.
         self.resource_group_id = resource_group_id
         # The database engine of the source instance.
         # 
         # *   **MySQL**: ApsaraDB RDS for MySQL instance or self-managed MySQL database
         # *   **PolarDB**: PolarDB for MySQL cluster
@@ -4863,18 +4963,18 @@
         # *   **DataHub**: DataHub project
         # *   **DB2**: self-managed Db2 for LUW database
         # *   **as400**: AS/400
         # *   **Tablestore**: Tablestore instance
         # 
         # > 
         # *   The default value is **MySQL**.
-        # *   For more information about the supported source and destination databases, see [Overview of data synchronization scenarios](~~130744~~) and [Overview of data migration scenarios](~~26618~~).
+        # *   For more information about the supported source and destination databases, see [Overview of data synchronization scenarios](https://help.aliyun.com/document_detail/130744.html) and [Overview of data migration scenarios](https://help.aliyun.com/document_detail/26618.html).
         # *   You must specify one of this parameter and the **JobId** parameter.
         self.source_endpoint_engine_name = source_endpoint_engine_name
-        # The ID of the region in which the source instance resides. For more information, see [List of supported regions](~~141033~~).
+        # The ID of the region in which the source instance resides. For more information, see [List of supported regions](https://help.aliyun.com/document_detail/141033.html).
         # 
         # >  You must specify one of this parameter and the **JobId** parameter.
         self.source_region = source_region
         # The synchronization topology. Valid values:
         # 
         # *   **oneway**: one-way synchronization. This is the default value.
         # *   **bidirectional**: two-way synchronization.
@@ -5124,29 +5224,31 @@
         # The threshold for triggering latency alerts.
         # 
         # *   If the **Type** parameter is set to **delay**, the threshold must be an integer. You can set the threshold based on your requirements. To prevent jitters caused by network and database overloads, we recommend that you set the threshold to more than 10 seconds. Unit: seconds.
         # *   If the **Type** parameter is set to **full_timeout**, the threshold must be an integer. Unit: hours.
         # 
         # >  This parameter is required if the **Type** parameter is set to **delay** or **full_timeout** and the **State** parameter is set to **Y**.
         self.delay_rule_time = delay_rule_time
-        # The ID of the data migration, data synchronization, or change tracking task. You can call the [DescribeDtsJobs](~~209702~~) operation to query the task ID.
+        # The ID of the data migration, data synchronization, or change tracking task. You can call the [DescribeDtsJobs](https://help.aliyun.com/document_detail/209702.html) operation to query the task ID.
+        # 
+        # This parameter is required.
         self.dts_job_id = dts_job_id
         # The alert threshold.
         self.notice_value = notice_value
         # The statistical period of the incremental data verification task. Unit: minutes.
         # 
         # >  Valid values: 1, 3, 5, and 30.
         self.period = period
         # The mobile numbers that receive alert notifications. Separate multiple mobile numbers with commas (,).
         # 
         # > 
         # *   This parameter is available only for users of the China site (aliyun.com). Only mobile numbers in the Chinese mainland are supported. You can specify up to 10 mobile numbers.
-        # *   Users of the international site (alibabacloud.com) cannot receive alerts by using mobile phones, but can [configure alert rules for DTS tasks in the CloudMonitor console](~~175876~~).
+        # *   Users of the international site (alibabacloud.com) cannot receive alerts by using mobile phones, but can [configure alert rules for DTS tasks in the CloudMonitor console](https://help.aliyun.com/document_detail/175876.html).
         self.phone = phone
-        # The region ID of the DTS instance. For more information, see [List of supported regions](~~141033~~).
+        # The region ID of the DTS instance. For more information, see [List of supported regions](https://help.aliyun.com/document_detail/141033.html).
         self.region_id = region_id
         self.resource_group_id = resource_group_id
         # Specifies whether to enable the alert rule. Valid values:
         # 
         # *   **Y**: enables the alert rule.
         # *   **N**: disables the alert rule.
         # 
@@ -5356,19 +5458,23 @@
         # The ID of the Alibaba Cloud account. You do not need to specify this parameter because this parameter will be removed in the future.
         self.account_id = account_id
         # The client token that is used to ensure the idempotence of the request. You can use the client to generate the value, but you must make sure that the value is unique among different requests. The **ClientToken** parameter can contain only ASCII characters and cannot exceed 64 characters in length.
         self.client_token = client_token
         # The specification of the data migration instance. Valid values: **small**, **medium**, **large**, **xlarge**, and **2xlarge**.
         # 
         # > 
-        # *   For more information about the test performance of each specification, see [Specifications of data migration instances](~~26606~~).
-        # *   For more information about the pricing of data migration instances, see [Pricing](~~117780~~).
+        # *   For more information about the test performance of each specification, see [Specifications of data migration instances](https://help.aliyun.com/document_detail/26606.html).
+        # *   For more information about the pricing of data migration instances, see [Pricing](https://help.aliyun.com/document_detail/117780.html).
+        # 
+        # This parameter is required.
         self.migration_job_class = migration_job_class
         self.owner_id = owner_id
-        # The ID of the region where the data migration instance resides. The region ID of the data migration instance is the same as that of the destination database. For more information, see [List of supported regions](~~141033~~).
+        # The ID of the region where the data migration instance resides. The region ID of the data migration instance is the same as that of the destination database. For more information, see [List of supported regions](https://help.aliyun.com/document_detail/141033.html).
+        # 
+        # This parameter is required.
         self.region = region
         # The ID of the region where the data migration instance resides. You do not need to specify this parameter because this parameter will be removed in the future.
         self.region_id = region_id
         self.resource_group_id = resource_group_id
 
     def validate(self):
         pass
@@ -5515,14 +5621,15 @@
     def __init__(
         self,
         dts_job_id: str = None,
         resource_group_id: str = None,
         shard_password: str = None,
         shard_username: str = None,
     ):
+        # This parameter is required.
         self.dts_job_id = dts_job_id
         self.resource_group_id = resource_group_id
         self.shard_password = shard_password
         self.shard_username = shard_username
 
     def validate(self):
         pass
@@ -5718,15 +5825,17 @@
         # The billing cycle of the subscription instance. Valid values:
         # 
         # *   **Year**\
         # *   **Month**\
         # 
         # >  You must specify this parameter only if you set the PayType parameter to **Prepaid**.
         self.period = period
-        # The region ID of the change tracking instance. The region ID is the same as that of the source instance. For more information, see [List of supported regions](~~141033~~).
+        # The region ID of the change tracking instance. The region ID is the same as that of the source instance. For more information, see [List of supported regions](https://help.aliyun.com/document_detail/141033.html).
+        # 
+        # This parameter is required.
         self.region = region
         self.region_id = region_id
         self.resource_group_id = resource_group_id
         # The subscription length.
         # 
         # *   If the billing cycle is **Year**, the value range is **1 to 5**.
         # *   If the billing cycle is **Month**, the value range is **1 to 60**.
@@ -5899,15 +6008,15 @@
         # *   **MySQL**: ApsaraDB RDS for MySQL instance or self-managed MySQL database
         # *   **PolarDB**: PolarDB for MySQL cluster or PolarDB O Edition cluster
         # *   **Redis**: Redis database
         # *   **MaxCompute**: MaxCompute project
         # 
         # > 
         # *   Default value: **MySQL**.
-        # *   For more information about the supported source and destination databases, see [Database types, initial synchronization types, and synchronization topologies](~~130744~~).
+        # *   For more information about the supported source and destination databases, see [Database types, initial synchronization types, and synchronization topologies](https://help.aliyun.com/document_detail/130744.html).
         self.instance_type = instance_type
 
     def validate(self):
         pass
 
     def to_map(self):
         _map = super().to_map()
@@ -5936,15 +6045,15 @@
         # *   **MySQL**: ApsaraDB RDS for MySQL instance or self-managed MySQL database
         # *   **PolarDB**: PolarDB for MySQL cluster or PolarDB O Edition cluster
         # *   **Redis**: Redis database
         # *   **DRDS**: PolarDB-X instance V1.0
         # 
         # > 
         # *   Default value: **MySQL**.
-        # *   For more information about the supported source and destination databases, see [Database types, initial synchronization types, and synchronization topologies](~~130744~~).
+        # *   For more information about the supported source and destination databases, see [Database types, initial synchronization types, and synchronization topologies](https://help.aliyun.com/document_detail/130744.html).
         self.instance_type = instance_type
 
     def validate(self):
         pass
 
     def to_map(self):
         _map = super().to_map()
@@ -5987,38 +6096,46 @@
         self.source_endpoint = source_endpoint
         # The ID of the Alibaba Cloud account. You do not need to specify this parameter because this parameter will be removed in the future.
         self.account_id = account_id
         # The client token that is used to ensure the idempotence of the request. You can use the client to generate the value, but you must make sure that it is unique among different requests. The **ClientToken** parameter can contain only ASCII characters and cannot exceed 64 characters in length.
         self.client_token = client_token
         # If you set the **SourceEndpoint.InstanceType** parameter to **DRDS**, you must specify the DBInstanceCount parameter. This parameter specifies the number of private RDS instances attached to the source PolarDB-X instance. Default value: **1**.
         self.dbinstance_count = dbinstance_count
-        # The ID of the region where the destination database resides. For more information, see [List of supported regions](~~141033~~).
+        # The ID of the region where the destination database resides. For more information, see [List of supported regions](https://help.aliyun.com/document_detail/141033.html).
         # 
         # >  If the **SourceRegion** parameter is set to the China (Hong Kong) region or a region outside the Chinese mainland, you must set the DestRegion parameter to the same region ID.
+        # 
+        # This parameter is required.
         self.dest_region = dest_region
         self.owner_id = owner_id
         # The billing method of the data synchronization instance.
         # 
         # *   **PrePaid**: subscription
         # *   **PostPaid** (default value): pay-as-you-go
+        # 
+        # This parameter is required.
         self.pay_type = pay_type
         # The billing cycle of the subscription instance. Valid values:
         # 
         # *   **Year**\
         # *   **Month**\
         # 
         # >  You must specify this parameter only if you set the PayType parameter to **PrePaid**.
         self.period = period
         self.region_id = region_id
         self.resource_group_id = resource_group_id
-        # The ID of the region where the source database resides. For more information, see [List of supported regions](~~141033~~).
+        # The ID of the region where the source database resides. For more information, see [List of supported regions](https://help.aliyun.com/document_detail/141033.html).
+        # 
+        # This parameter is required.
         self.source_region = source_region
         # The specification of the data synchronization instance. Valid values: **micro**, **small**, **medium**, and **large**.
         # 
-        # >  For more information about the test performance of each specification, see [Specifications of data synchronization instances](~~26605~~).
+        # >  For more information about the test performance of each specification, see [Specifications of data synchronization instances](https://help.aliyun.com/document_detail/26605.html).
+        # 
+        # This parameter is required.
         self.synchronization_job_class = synchronization_job_class
         # The synchronization topology. Valid values:
         # 
         # *   **oneway**: one-way synchronization
         # *   **bidirectional**: two-way synchronization
         # 
         # > 
@@ -6222,25 +6339,29 @@
         self,
         consumer_group_id: str = None,
         dts_instance_id: str = None,
         dts_job_id: str = None,
         region_id: str = None,
         resource_group_id: str = None,
     ):
-        # The ID of the consumer group. You can call the [DescribeConsumerChannel](~~264169~~) operation to query the consumer group ID.
+        # The ID of the consumer group. You can call the [DescribeConsumerChannel](https://help.aliyun.com/document_detail/264169.html) operation to query the consumer group ID.
+        # 
+        # This parameter is required.
         self.consumer_group_id = consumer_group_id
-        # The ID of the change tracking instance. You can call the [DescribeDtsJobs](~~209702~~) operation to query the instance ID.
+        # The ID of the change tracking instance. You can call the [DescribeDtsJobs](https://help.aliyun.com/document_detail/209702.html) operation to query the instance ID.
         # 
         # >  You must specify at least one of the **DtsInstanceId** and **DtsJobId** parameters.
         self.dts_instance_id = dts_instance_id
-        # The ID of the change tracking task. You can call the [DescribeDtsJobs](~~209702~~) operation to query the task ID.
+        # The ID of the change tracking task. You can call the [DescribeDtsJobs](https://help.aliyun.com/document_detail/209702.html) operation to query the task ID.
         # 
         # >  You must specify at least one of the **DtsInstanceId** and **DtsJobId** parameters.
         self.dts_job_id = dts_job_id
-        # The ID of the region where the change tracking instance resides. For more information, see [List of supported regions](~~141033~~).
+        # The ID of the region where the change tracking instance resides. For more information, see [List of supported regions](https://help.aliyun.com/document_detail/141033.html).
+        # 
+        # This parameter is required.
         self.region_id = region_id
         self.resource_group_id = resource_group_id
 
     def validate(self):
         pass
 
     def to_map(self):
@@ -6381,20 +6502,24 @@
         owner_id: str = None,
         region_id: str = None,
         resource_group_id: str = None,
         subscription_instance_id: str = None,
     ):
         # The ID of the Alibaba Cloud account. You do not need to specify this parameter because this parameter will be removed in the future.
         self.account_id = account_id
-        # The ID of the consumer group. You can call the [DescribeConsumerGroup](~~122886~~) operation to query the consumer group ID.
+        # The ID of the consumer group. You can call the [DescribeConsumerGroup](https://help.aliyun.com/document_detail/122886.html) operation to query the consumer group ID.
+        # 
+        # This parameter is required.
         self.consumer_group_id = consumer_group_id
         self.owner_id = owner_id
         self.region_id = region_id
         self.resource_group_id = resource_group_id
         # The ID of the change tracking instance. You can call the **DescribeSubscriptionInstances** operation to query the instance ID.
+        # 
+        # This parameter is required.
         self.subscription_instance_id = subscription_instance_id
 
     def validate(self):
         pass
 
     def to_map(self):
         _map = super().to_map()
@@ -6619,15 +6744,15 @@
         # *   **Reverse**: Data is synchronized from the destination database to the source database.
         # 
         # > 
         # 
         # *   Default value: **Forward**.
         # *   You can set this parameter to **Reverse** to delete the reverse synchronization task only if the topology is two-way synchronization.
         self.request_id = request_id
-        # The ID of the region in which the data migration or synchronization task resides. For more information, see [List of supported regions](~~141033~~).
+        # The ID of the region in which the data migration or synchronization task resides. For more information, see [List of supported regions](https://help.aliyun.com/document_detail/141033.html).
         self.success = success
 
     def validate(self):
         pass
 
     def to_map(self):
         _map = super().to_map()
@@ -6718,17 +6843,19 @@
         region_id: str = None,
         resource_group_id: str = None,
         zero_etl_job: bool = None,
     ):
         # The ID of the data migration, data synchronization, or change tracking task.
         # 
         # > *   Separate multiple task IDs with commas (,).
-        # > *   You can call the [DescribeDtsJobs](~~209702~~) operation to query task IDs.
+        # > *   You can call the [DescribeDtsJobs](https://help.aliyun.com/document_detail/209702.html) operation to query task IDs.
+        # 
+        # This parameter is required.
         self.dts_job_ids = dts_job_ids
-        # The ID of the region in which the DTS instance resides. For more information, see [List of supported regions](~~141033~~).
+        # The ID of the region in which the DTS instance resides. For more information, see [List of supported regions](https://help.aliyun.com/document_detail/141033.html).
         self.region_id = region_id
         self.resource_group_id = resource_group_id
         self.zero_etl_job = zero_etl_job
 
     def validate(self):
         pass
 
@@ -6770,15 +6897,15 @@
         err_message: str = None,
         http_status_code: int = None,
         request_id: str = None,
         success: bool = None,
     ):
         # The dynamic error code. This parameter will be removed soon.
         self.dynamic_code = dynamic_code
-        # The dynamic part in the error message. This parameter is used to replace the \*\*%s\*\* variable in the **ErrMessage** parameter.
+        # The dynamic part in the error message. This parameter is used to replace the \\*\\*%s\\*\\* variable in the **ErrMessage** parameter.
         # 
         # > If the return value of the **ErrMessage** parameter is **The Value of Input Parameter %s is not valid** and the return value of the **DynamicMessage** parameter is **DtsJobId**, the specified **DtsJobId** parameter is invalid.
         self.dynamic_message = dynamic_message
         # The error code returned if the request failed.
         self.err_code = err_code
         # The error message returned if the request failed.
         self.err_message = err_message
@@ -6882,14 +7009,16 @@
         owner_id: str = None,
         region_id: str = None,
         resource_group_id: str = None,
     ):
         # The ID of the Alibaba Cloud account. You do not need to specify this parameter because this parameter will be removed in the future.
         self.account_id = account_id
         # The ID of the data migration instance. You can call the **DescribeMigrationJobs** operation to query all data migration instances.
+        # 
+        # This parameter is required.
         self.migration_job_id = migration_job_id
         self.owner_id = owner_id
         self.region_id = region_id
         self.resource_group_id = resource_group_id
 
     def validate(self):
         pass
@@ -7028,14 +7157,16 @@
     ):
         # The ID of the Alibaba Cloud account. You do not need to specify this parameter because this parameter will be removed in the future.
         self.account_id = account_id
         self.owner_id = owner_id
         self.region_id = region_id
         self.resource_group_id = resource_group_id
         # The ID of the change tracking instance. You can call the DescribeSubscriptionInstances operation to query the instance ID.
+        # 
+        # This parameter is required.
         self.subscription_instance_id = subscription_instance_id
 
     def validate(self):
         pass
 
     def to_map(self):
         _map = super().to_map()
@@ -7171,14 +7302,16 @@
     ):
         # The ID of the Alibaba Cloud account. You do not need to specify this parameter because this parameter will be removed in the future.
         self.account_id = account_id
         self.owner_id = owner_id
         self.region_id = region_id
         self.resource_group_id = resource_group_id
         # The ID of the data synchronization instance. You can call the DescribeSynchronizationJobs operation to query the instance ID.
+        # 
+        # This parameter is required.
         self.synchronization_job_id = synchronization_job_id
 
     def validate(self):
         pass
 
     def to_map(self):
         _map = super().to_map()
@@ -7310,14 +7443,15 @@
         owner_id: str = None,
         region: str = None,
         region_id: str = None,
         resource_group_id: str = None,
         tags: str = None,
         type: str = None,
     ):
+        # This parameter is required.
         self.dts_job_id = dts_job_id
         self.owner_id = owner_id
         self.region = region
         self.region_id = region_id
         self.resource_group_id = resource_group_id
         self.tags = tags
         self.type = type
@@ -7807,14 +7941,16 @@
         start_time: int = None,
     ):
         # The ID of the Alibaba Cloud account.
         self.account_id = account_id
         # The client token that is used to ensure the idempotence of the request. You can use the client to generate the token, but you must make sure that the token is unique among different requests. **The token can contain only ASCII characters and cannot exceed 64 characters in length.
         self.client_token = client_token
         # The ID of the DTS dedicated cluster on which a DTS task runs.
+        # 
+        # This parameter is required.
         self.dedicated_cluster_id = dedicated_cluster_id
         # The ID of the data migration or synchronization task.
         self.dts_job_id = dts_job_id
         # The end of the time range to query. The value must be in the UNIX timestamp format. Unit: milliseconds.
         self.end_time = end_time
         self.owner_id = owner_id
         # The number of the page to return. The value must be an integer that is greater than 0. Default value: **1**.
@@ -8120,14 +8256,16 @@
         security_token: str = None,
     ):
         # The ID of the Alibaba Cloud account. You do not need to specify this parameter because this parameter is discontinued.
         self.account_id = account_id
         # The client token that is used to ensure the idempotence of the request. You can use the client to generate the token, but you must make sure that the token is unique among different requests. **The token can contain only ASCII characters and cannot exceed 64 characters in length.
         self.client_token = client_token
         # The ID of the cluster. If the **MetricType** parameter is set to **CLUSTER**, enter the ID of the exclusive cluster. Otherwise, set this parameter to a node ID.
+        # 
+        # This parameter is required.
         self.dedicated_cluster_id = dedicated_cluster_id
         # The ID of the data migration or synchronization task.
         self.dts_job_id = dts_job_id
         # The cluster environment. Default value: **ALIYUN**.
         self.env = env
         # Specifies whether to query the metrics of the cluster or a node. Default value: CLUSTER. Valid values:
         # 
@@ -8439,35 +8577,37 @@
         # *   **MongoDB**: ApsaraDB for MongoDB instance
         # *   **Redis**: ApsaraDB for Redis instance
         # *   **PetaData**: HybridDB for MySQL instance
         # *   **POLARDB**: PolarDB for MySQL cluster
         # *   **PolarDB_o**: PolarDB for Oracle cluster
         # *   **AnalyticDB**: AnalyticDB for MySQL cluster V3.0 or V2.0
         # *   **Greenplum**: AnalyticDB for PostgreSQL instance
+        # 
+        # This parameter is required.
         self.destination_endpoint_instance_type = destination_endpoint_instance_type
         # You must specify this parameter only if the **DestinationEndpointEngineName** parameter is set to **Oracle**. Valid values:
         # 
         # *   **SID**: non-RAC architecture
         # *   **RAC**: RAC architecture
         # 
         # >  This parameter is optional. The data type of this parameter is String.
         self.destination_endpoint_oracle_sid = destination_endpoint_oracle_sid
         # The password of the destination database account.
         self.destination_endpoint_password = destination_endpoint_password
         # The service port number of the source database.
         # 
         # >  You must specify this parameter only if the **SourceEndpointInstanceType** parameter is set to **ECS**, **LocalInstance**, or **Express**.
         self.destination_endpoint_port = destination_endpoint_port
-        # The ID of the region where the destination instance resides. For more information, see [List of supported regions](~~141033~~).
+        # The ID of the region where the destination instance resides. For more information, see [List of supported regions](https://help.aliyun.com/document_detail/141033.html).
         self.destination_endpoint_region = destination_endpoint_region
         # The database account of the destination database.
         # 
-        # >  The permissions that are required for database accounts vary with the migration or synchronization scenario. For more information, see [Overview of data migration scenarios](~~26618~~) and [Overview of data synchronization scenarios](~~130744~~).
+        # >  The permissions that are required for database accounts vary with the migration or synchronization scenario. For more information, see [Overview of data migration scenarios](https://help.aliyun.com/document_detail/26618.html) and [Overview of data synchronization scenarios](https://help.aliyun.com/document_detail/130744.html).
         self.destination_endpoint_user_name = destination_endpoint_user_name
-        # The ID of the region where the DTS instance resides. For more information, see [List of supported regions](~~141033~~).
+        # The ID of the region where the DTS instance resides. For more information, see [List of supported regions](https://help.aliyun.com/document_detail/141033.html).
         self.region_id = region_id
         self.resource_group_id = resource_group_id
         # You must specify this parameter only if the **SourceEndpointEngineName** parameter is set to **Oracle**. Valid values:
         # 
         # *   **SID**: non-RAC architecture
         # *   **RAC**: RAC architecture
         # 
@@ -8496,30 +8636,32 @@
         # *   **LocalInstance**: self-managed database with a public IP address
         # *   **ECS**: self-managed database that is hosted on ECS
         # *   **Express**: self-managed database that is connected over Express Connect
         # *   **dg**: self-managed database that is connected over Database Gateway
         # *   **MongoDB**: ApsaraDB for MongoDB instance
         # *   **POLARDB**: PolarDB for MySQL cluster
         # *   **PolarDB_o**: PolarDB for Oracle cluster
+        # 
+        # This parameter is required.
         self.source_endpoint_instance_type = source_endpoint_instance_type
         # The SID of the Oracle database.
         # 
         # >  You must specify this parameter only if the **SourceEndpointEngineName** parameter is set to **Oracle** and the Oracle database is deployed in a non-RAC architecture.
         self.source_endpoint_oracle_sid = source_endpoint_oracle_sid
         # The password of the source database account.
         self.source_endpoint_password = source_endpoint_password
         # The service port number of the source database.
         # 
         # >  You must specify this parameter only if the **SourceEndpointInstanceType** parameter is set to **ECS**, **LocalInstance**, or **Express**.
         self.source_endpoint_port = source_endpoint_port
-        # The ID of the region where the source instance resides. For more information, see [List of supported regions](~~141033~~).
+        # The ID of the region where the source instance resides. For more information, see [List of supported regions](https://help.aliyun.com/document_detail/141033.html).
         self.source_endpoint_region = source_endpoint_region
         # The database account of the source database.
         # 
-        # >  The permissions that are required for database accounts vary with the migration or synchronization scenario. For more information, see [Overview of data migration scenarios](~~26618~~) and [Overview of data synchronization scenarios](~~130744~~).
+        # >  The permissions that are required for database accounts vary with the migration or synchronization scenario. For more information, see [Overview of data migration scenarios](https://help.aliyun.com/document_detail/26618.html) and [Overview of data synchronization scenarios](https://help.aliyun.com/document_detail/130744.html).
         self.source_endpoint_user_name = source_endpoint_user_name
 
     def validate(self):
         pass
 
     def to_map(self):
         _map = super().to_map()
@@ -8741,29 +8883,31 @@
         dts_job_id: str = None,
         page_number: int = None,
         page_size: int = None,
         parent_channel_id: str = None,
         region_id: str = None,
         resource_group_id: str = None,
     ):
-        # The ID of the change tracking instance. You can call the [DescribeDtsJobs](~~209702~~) operation to query the instance ID.
+        # The ID of the change tracking instance. You can call the [DescribeDtsJobs](https://help.aliyun.com/document_detail/209702.html) operation to query the instance ID.
         # 
         # >  You must specify at least one of the **DtsInstanceId** and **DtsJobId** parameters.
         self.dts_instance_id = dts_instance_id
-        # The ID of the change tracking task. You can call the [DescribeDtsJobs](~~209702~~) operation to query the task ID.
+        # The ID of the change tracking task. You can call the [DescribeDtsJobs](https://help.aliyun.com/document_detail/209702.html) operation to query the task ID.
         # 
         # >  You must specify at least one of the **DtsInstanceId** and **DtsJobId** parameters.
         self.dts_job_id = dts_job_id
         # The number of the page to return. The value must be an integer that is greater than **0** and does not exceed the maximum value of the Integer data type. Default value: **1**.
         self.page_number = page_number
         # The number of entries to return on each page. Valid values: **1** to **100**. Default value: **20**.
         self.page_size = page_size
         # The parent task ID of the distributed task.
         self.parent_channel_id = parent_channel_id
-        # The ID of the region in which the change tracking instance resides. For more information, see [List of supported regions](~~141033~~).
+        # The ID of the region in which the change tracking instance resides. For more information, see [List of supported regions](https://help.aliyun.com/document_detail/141033.html).
+        # 
+        # This parameter is required.
         self.region_id = region_id
         self.resource_group_id = resource_group_id
 
     def validate(self):
         pass
 
     def to_map(self):
@@ -9026,14 +9170,16 @@
         # The number of the page to return. The value must be an integer that is greater than **0** and does not exceed the maximum value of the Integer data type. Default value: **1**.
         self.page_num = page_num
         # The number of entries to return on each page. Valid values: **30**, **50**, and **100**. Default value: **30**.
         self.page_size = page_size
         self.region_id = region_id
         self.resource_group_id = resource_group_id
         # The ID of the change tracking instance. You can call the DescribeSubscriptionInstances operation to query the instance ID.
+        # 
+        # This parameter is required.
         self.subscription_instance_id = subscription_instance_id
 
     def validate(self):
         pass
 
     def to_map(self):
         _map = super().to_map()
@@ -9302,23 +9448,25 @@
     def __init__(
         self,
         destination_endpoint_region: str = None,
         region_id: str = None,
         resource_group_id: str = None,
         source_endpoint_region: str = None,
     ):
-        # The ID of the region where the destination instance resides. For more information, see [List of supported regions](~~141033~~).
+        # The ID of the region where the destination instance resides. For more information, see [List of supported regions](https://help.aliyun.com/document_detail/141033.html).
         # 
         # >  If the destination instance is a self-managed database with a public IP address, you can set the parameter to **cn-hangzhou** or the ID of the closest region.
         self.destination_endpoint_region = destination_endpoint_region
         self.region_id = region_id
         self.resource_group_id = resource_group_id
-        # The ID of the region where the source instance resides. For more information, see [List of supported regions](~~141033~~).
+        # The ID of the region where the source instance resides. For more information, see [List of supported regions](https://help.aliyun.com/document_detail/141033.html).
         # 
         # >  If the source instance is a self-managed database with a public IP address, you can set the parameter to **cn-hangzhou** or the ID of the closest region.
+        # 
+        # This parameter is required.
         self.source_endpoint_region = source_endpoint_region
 
     def validate(self):
         pass
 
     def to_map(self):
         _map = super().to_map()
@@ -9462,21 +9610,29 @@
         resource_group_id: str = None,
         tb_name: str = None,
     ):
         # The data verification method. Valid values:
         # 
         # *   **1**: full data verification.
         # *   **2**: incremental data verification.
+        # 
+        # This parameter is required.
         self.check_type = check_type
         # The name of the verified source database.
+        # 
+        # This parameter is required.
         self.db_name = db_name
-        # The ID of the Data Transmission Service (DTS) task. You can call the [DescribeDtsJobs](~~209702~~) operation to query the task ID.
+        # The ID of the Data Transmission Service (DTS) task. You can call the [DescribeDtsJobs](https://help.aliyun.com/document_detail/209702.html) operation to query the task ID.
+        # 
+        # This parameter is required.
         self.dts_job_id = dts_job_id
         self.resource_group_id = resource_group_id
         # The name of the table verified in the source database.
+        # 
+        # This parameter is required.
         self.tb_name = tb_name
 
     def validate(self):
         pass
 
     def to_map(self):
         _map = super().to_map()
@@ -9627,16 +9783,20 @@
         status: str = None,
         table_name: str = None,
     ):
         # The data verification method. Valid values:
         # 
         # *   **1**: full data verification.
         # *   **2**: incremental data verification.
+        # 
+        # This parameter is required.
         self.check_type = check_type
-        # The ID of the data migration or data synchronization task. You can call the [DescribeDtsJobs](~~209702~~) operation to query the task ID.
+        # The ID of the data migration or data synchronization task. You can call the [DescribeDtsJobs](https://help.aliyun.com/document_detail/209702.html) operation to query the task ID.
+        # 
+        # This parameter is required.
         self.dts_job_id = dts_job_id
         # The number of the page to return. The value must be an integer that is greater than **0**. Default value: **1**.
         self.page_number = page_number
         # The number of entries to return on each page.
         self.page_size = page_size
         self.resource_group_id = resource_group_id
         # The name of the schema whose data is verified in the source database.
@@ -9821,15 +9981,15 @@
         table_details: List[DescribeDataCheckTableDetailsResponseBodyTableDetails] = None,
         total_count: int = None,
     ):
         # The number of tables that contain inconsistent data.
         self.diff_table_count = diff_table_count
         # The dynamic error code. This parameter will be discontinued in the future.
         self.dynamic_code = dynamic_code
-        # The dynamic part in the error message. This parameter is used to replace the \*\*%s\*\* variable in the **ErrMessage** parameter.
+        # The dynamic part in the error message. This parameter is used to replace the \\*\\*%s\\*\\* variable in the **ErrMessage** parameter.
         # 
         # > For example, if the returned value of the **ErrMessage** parameter is **The Value of Input Parameter %s is not valid** and the return value of the **DynamicMessage** parameter is **Type**, the specified **Type** parameter is invalid.
         self.dynamic_message = dynamic_message
         # The error code returned if the request failed.
         self.err_code = err_code
         # The error message returned if the request failed.
         self.err_message = err_message
@@ -9968,20 +10128,24 @@
         db_name: str = None,
         dts_job_id: str = None,
         page_number: int = None,
         page_size: int = None,
         resource_group_id: str = None,
         tb_name: str = None,
     ):
+        # This parameter is required.
         self.check_type = check_type
+        # This parameter is required.
         self.db_name = db_name
+        # This parameter is required.
         self.dts_job_id = dts_job_id
         self.page_number = page_number
         self.page_size = page_size
         self.resource_group_id = resource_group_id
+        # This parameter is required.
         self.tb_name = tb_name
 
     def validate(self):
         pass
 
     def to_map(self):
         _map = super().to_map()
@@ -10204,14 +10368,16 @@
         self,
         dedicated_cluster_id: str = None,
         owner_id: str = None,
         region_id: str = None,
         resource_group_id: str = None,
     ):
         # The ID of the cluster.
+        # 
+        # This parameter is required.
         self.dedicated_cluster_id = dedicated_cluster_id
         self.owner_id = owner_id
         # The ID of the region in which the instance resides.
         self.region_id = region_id
         self.resource_group_id = resource_group_id
 
     def validate(self):
@@ -10684,23 +10850,25 @@
         dts_instance_id: str = None,
         dts_job_id: str = None,
         page_number: int = None,
         page_size: int = None,
         region_id: str = None,
         resource_group_id: str = None,
     ):
-        # The ID of the Data Transmission Service (DTS) instance. You can call the [DescribeDtsJobs](~~209702~~) operation to query the instance ID.
+        # The ID of the Data Transmission Service (DTS) instance. You can call the [DescribeDtsJobs](https://help.aliyun.com/document_detail/209702.html) operation to query the instance ID.
+        # 
+        # This parameter is required.
         self.dts_instance_id = dts_instance_id
-        # The ID of the ETL task. You can call the [DescribeDtsJobs](~~209702~~) operation to query the task ID.
+        # The ID of the ETL task. You can call the [DescribeDtsJobs](https://help.aliyun.com/document_detail/209702.html) operation to query the task ID.
         self.dts_job_id = dts_job_id
         # The number of the page to return. Default value: 1.
         self.page_number = page_number
         # The number of entries to return on each page. Default value: 20.
         self.page_size = page_size
-        # The ID of the region in which the DTS instance resides. You can call the [DescribeRegions](~~25609~~) operation to query the available Alibaba Cloud regions.
+        # The ID of the region in which the DTS instance resides. You can call the [DescribeRegions](https://help.aliyun.com/document_detail/25609.html) operation to query the available Alibaba Cloud regions.
         self.region_id = region_id
         self.resource_group_id = resource_group_id
 
     def validate(self):
         pass
 
     def to_map(self):
@@ -11193,22 +11361,22 @@
         self.instance_type = instance_type
         # The SID of the Oracle database.
         # 
         # >  This parameter is returned only if the **EngineName** parameter of the destination instance is set to **Oracle** and the Oracle database is deployed in a non-RAC architecture.
         self.ip = ip
         # The username of the account that is used to connect to the source database.
         self.oracle_sid = oracle_sid
-        # The ID of the region in which the destination instance resides. For more information, see [List of supported regions](~~141033~~).
+        # The ID of the region in which the destination instance resides. For more information, see [List of supported regions](https://help.aliyun.com/document_detail/141033.html).
         self.port = port
         # Indicates whether SSL encryption is enabled. Valid values:
         # 
         # *   **DISABLE**: SSL encryption is disabled.
         # *   **ENABLE_WITH_CERTIFICATE**: SSL encryption is enabled, and the CA certificate is uploaded.
-        # *   **ENABLE_ONLY\_4\_MONGODB_ALTAS**: SSL encryption is enabled for the connection to an AWS MongoDB Altas database.
-        # *   **ENABLE_ONLY\_4\_KAFKA_SCRAM_SHA\_256**: SCRAM-SHA-256 is used to encrypt the connection to a Kafka cluster.
+        # *   **ENABLE_ONLY_4_MONGODB_ALTAS**: SSL encryption is enabled for the connection to an AWS MongoDB Altas database.
+        # *   **ENABLE_ONLY_4_KAFKA_SCRAM_SHA_256**: SCRAM-SHA-256 is used to encrypt the connection to a Kafka cluster.
         self.region = region
         # The ID of the Alibaba Cloud account to which the source ApsaraDB RDS instance belongs.
         self.ssl_solution_enum = ssl_solution_enum
         # The ID of the destination instance.
         self.user_name = user_name
 
     def validate(self):
@@ -11433,25 +11601,25 @@
         self.port = port
         # The type of the source instance.
         self.region = region
         # Indicates whether SSL encryption is enabled. Valid values:
         # 
         # *   **DISABLE**: SSL encryption is disabled.
         # *   **ENABLE_WITH_CERTIFICATE**: SSL encryption is enabled, and the CA certificate is uploaded.
-        # *   **ENABLE_ONLY\_4\_MONGODB_ALTAS**: SSL encryption is enabled for the connection to an AWS MongoDB Altas database.
-        # *   **ENABLE_ONLY\_4\_KAFKA_SCRAM_SHA\_256**: SCRAM-SHA-256 is used to encrypt the connection to a Kafka cluster.
+        # *   **ENABLE_ONLY_4_MONGODB_ALTAS**: SSL encryption is enabled for the connection to an AWS MongoDB Altas database.
+        # *   **ENABLE_ONLY_4_KAFKA_SCRAM_SHA_256**: SCRAM-SHA-256 is used to encrypt the connection to a Kafka cluster.
         self.role_name = role_name
         # The synchronization direction. Valid values:
         # 
         # *   **Forward**: Data is synchronized from the source database to the destination database.
         # *   **Reverse**: Data is synchronized from the destination database to the source database.
         # 
         # >  This parameter is returned only if the topology of the data synchronization instance is two-way synchronization.
         self.ssl_solution_enum = ssl_solution_enum
-        # The ID of the region in which the source instance resides. For more information, see [List of supported regions](~~141033~~).
+        # The ID of the region in which the source instance resides. For more information, see [List of supported regions](https://help.aliyun.com/document_detail/141033.html).
         self.user_name = user_name
 
     def validate(self):
         pass
 
     def to_map(self):
         _map = super().to_map()
@@ -16300,17 +16468,17 @@
         self.binlog_site = binlog_site
         self.binlog_time = binlog_time
         self.boot_time = boot_time
         # The ID of the data migration, data synchronization, or change tracking instance.
         self.checkpoint = checkpoint
         # The topic of the change tracking instance.
         # 
-        # >  This parameter is returned only if your change tracking instances are of the new version and you have called the [CreateConsumerGroup](~~122863~~) operation to create a consumer group.
+        # >  This parameter is returned only if your change tracking instances are of the new version and you have called the [CreateConsumerGroup](https://help.aliyun.com/document_detail/122863.html) operation to create a consumer group.
         self.code = code
-        # The downstream client information in the following format: \<IP address of the downstream client>:\<Random ID generated by DTS>.
+        # The downstream client information in the following format: \\<IP address of the downstream client>:\\<Random ID generated by DTS>.
         self.consumption_checkpoint = consumption_checkpoint
         # The error code returned if the request failed.
         self.consumption_client = consumption_client
         # The end time of the task. The time follows the ISO 8601 standard in the *yyyy-MM-dd*T*HH:mm:ss*Z format. The time is displayed in UTC.
         self.create_time = create_time
         self.data_delivery_channel_info = data_delivery_channel_info
         self.data_synchronization_status = data_synchronization_status
@@ -16320,15 +16488,15 @@
         self.db_object = db_object
         self.dedicated_cluster_id = dedicated_cluster_id
         # The ID of the request.
         self.delay = delay
         self.demo_job = demo_job
         # The instance class.
         # 
-        # >  For more information about the test performance of each instance class, see [Specifications of data migration instances](~~26606~~) and [Specifications of data synchronization instances](~~26605~~).
+        # >  For more information about the test performance of each instance class, see [Specifications of data migration instances](https://help.aliyun.com/document_detail/26606.html) and [Specifications of data synchronization instances](https://help.aliyun.com/document_detail/26605.html).
         self.dest_net_type = dest_net_type
         # The name of the database that contains the objects to be migrated from the source instance.
         self.destination_endpoint = destination_endpoint
         self.dts_bis_label = dts_bis_label
         # Indicates whether the new change tracking feature is used.
         # 
         # >  This parameter is returned only for change tracking instances of the new version.
@@ -16349,25 +16517,25 @@
         # 
         # > 
         # *   Default value: **Forward**.
         # *   The value **Reverse** takes effect only if the topology of the data synchronization instance is two-way synchronization.
         self.dts_job_name = dts_job_name
         # The error message returned if the request failed.
         self.dynamic_message = dynamic_message
-        # The reserved parameter of DTS. The value is a JSON string. You can specify this parameter to meet specific requirements, for example, whether to automatically start a precheck. For more information, see [MigrationReserved](~~176470~~).
+        # The reserved parameter of DTS. The value is a JSON string. You can specify this parameter to meet specific requirements, for example, whether to automatically start a precheck. For more information, see [MigrationReserved](https://help.aliyun.com/document_detail/176470.html).
         self.end_timestamp = end_timestamp
         # The start offset of incremental data migration or synchronization. The value is a UNIX timestamp. Unit: seconds.
         self.err_code = err_code
         # The point in time when the instance expires. The time follows the ISO 8601 standard in the *yyyy-MM-dd*T*HH:mm:ss*Z format. The time is displayed in UTC.
         # 
         # >  This parameter is returned only if the return value of the **PayType** parameter is **PrePaid**.
         self.err_message = err_message
         # The name of the data migration, data synchronization, or change tracking task.
         self.error_message = error_message
-        # The objects of the data migration, data synchronization, or change tracking task. For more information, see [Objects of DTS tasks](~~209545~~).
+        # The objects of the data migration, data synchronization, or change tracking task. For more information, see [Objects of DTS tasks](https://help.aliyun.com/document_detail/209545.html).
         self.etl_calculator = etl_calculator
         # The error code. This parameter will be removed in the future.
         self.expire_time = expire_time
         # The state of the data migration or data synchronization task.
         # 
         # Valid values for a data migration task:
         # 
@@ -16389,15 +16557,15 @@
         # *   **Modifying**: The objects in the task are being modified.
         # *   **Finished**: The task is complete.
         self.finish_time = finish_time
         # The operator information of the extract, transform, and load (ETL) task.
         # 
         # >  This parameter is returned only if you query the details of an ETL task.
         self.group_id = group_id
-        # The dynamic part in the error message. This parameter is used to replace the \*\*%s\*\* variable in the **ErrMessage** parameter.
+        # The dynamic part in the error message. This parameter is used to replace the \\*\\*%s\\*\\* variable in the **ErrMessage** parameter.
         # 
         # >  If the return value of the **ErrMessage** parameter is **The Value of Input Parameter %s is not valid** and the return value of the **DynamicMessage** parameter is **DtsJobId**, the specified **DtsJobId** parameter is invalid.
         self.http_status_code = http_status_code
         self.job_type = job_type
         self.last_update_time = last_update_time
         self.max_du = max_du
         # The type of the destination instance.
@@ -16831,15 +16999,15 @@
         self.page_number = page_number
         # The number of entries to return on each page. Valid values: **30**, **50**, and **100**. Default value: **30**.
         self.page_size = page_size
         # The content of the query condition.
         # 
         # >  You must set the **Type** parameter to specify the type of the query condition.
         self.params = params
-        # The ID of the region in which the DTS instance resides. For more information, see [List of supported regions](~~141033~~).
+        # The ID of the region in which the DTS instance resides. For more information, see [List of supported regions](https://help.aliyun.com/document_detail/141033.html).
         self.region = region
         # This parameter is discontinued.
         self.region_id = region_id
         # The resource group ID.
         self.resource_group_id = resource_group_id
         # The state of the DTS task.
         # 
@@ -17197,15 +17365,15 @@
         # The error message returned if incremental data migration or synchronization failed.
         self.error_message = error_message
         # Indicates whether the instance needs to be upgraded. Valid values:
         # 
         # *   **true**: yes
         # *   **false**: no
         # 
-        # >  To upgrade a DTS instance, call the [TransferInstanceClass](~~281093~~) operation.
+        # >  To upgrade a DTS instance, call the [TransferInstanceClass](https://help.aliyun.com/document_detail/281093.html) operation.
         self.need_upgrade = need_upgrade
         # The progress of incremental data migration or synchronization.
         self.percent = percent
         # The number of records that have been migrated or synchronized during incremental data migration or synchronization.
         self.progress = progress
         # The state of incremental data migration or synchronization. Valid values:
         # 
@@ -17278,22 +17446,22 @@
         self.ip = ip
         # The SID of the Oracle database.
         # 
         # >  This parameter is returned only if the **EngineName** parameter of the destination instance is set to **Oracle** and the Oracle database is deployed in a non-RAC architecture.
         self.oracle_sid = oracle_sid
         # The database service port of the destination instance.
         self.port = port
-        # The ID of the region in which the destination instance resides. For more information, see [List of supported regions](~~141033~~).
+        # The ID of the region in which the destination instance resides. For more information, see [List of supported regions](https://help.aliyun.com/document_detail/141033.html).
         self.region = region
         # Indicates whether SSL encryption is enabled. Valid values:
         # 
         # *   **DISABLE**: SSL encryption is disabled.
         # *   **ENABLE_WITH_CERTIFICATE**: SSL encryption is enabled, and the CA certificate is uploaded.
-        # *   **ENABLE_ONLY\_4\_MONGODB_ALTAS**: SSL encryption is enabled for the connection to an AWS MongoDB Altas database.
-        # *   **ENABLE_ONLY\_4\_KAFKA_SCRAM_SHA\_256**: SCRAM-SHA-256 is used to encrypt the connection to a Kafka cluster.
+        # *   **ENABLE_ONLY_4_MONGODB_ALTAS**: SSL encryption is enabled for the connection to an AWS MongoDB Altas database.
+        # *   **ENABLE_ONLY_4_KAFKA_SCRAM_SHA_256**: SCRAM-SHA-256 is used to encrypt the connection to a Kafka cluster.
         self.ssl_solution_enum = ssl_solution_enum
         # The database account of the destination instance.
         self.user_name = user_name
 
     def validate(self):
         pass
 
@@ -17915,15 +18083,15 @@
         # The error message returned if incremental data synchronization failed.
         self.error_message = error_message
         # Indicates whether the instance needs to be upgraded. Valid values:
         # 
         # - **true**\
         # - **false**\
         # 
-        # > To upgrade a DTS instance, call the [TransferInstanceClass](~~281093~~) operation.
+        # > To upgrade a DTS instance, call the [TransferInstanceClass](https://help.aliyun.com/document_detail/281093.html) operation.
         self.need_upgrade = need_upgrade
         # The progress of incremental data synchronization. Unit: percentage.
         self.percent = percent
         # The number of entries that have been migrated or synchronized during incremental data migration or synchronization.
         self.progress = progress
         # The state of incremental data synchronization.
         self.status = status
@@ -17990,15 +18158,15 @@
         self.ip = ip
         # The SID of the Oracle database. 
         # 
         # > This parameter is returned only if the returned value of **EngineName** of the destination instance is **Oracle** and the Oracle database is deployed in a non-RAC architecture.
         self.oracle_sid = oracle_sid
         # The port number of the destination instance.
         self.port = port
-        # The ID of the region in which the destination instance resides. For more information, see [List of supported regions](~~141033~~).
+        # The ID of the region in which the destination instance resides. For more information, see [List of supported regions](https://help.aliyun.com/document_detail/141033.html).
         self.region = region
         # Indicates whether SSL encryption is enabled. Valid values:
         # 
         # - **DISABLE**: SSL encryption is disabled. 
         # - **ENABLE_WITH_CERTIFICATE**: SSL encryption is enabled and the CA certificate is uploaded. 
         # - **ENABLE_ONLY_4_MONGODB_ALTAS**: SSL encryption is enabled for the connection with an AWS MongoDB Altas database. 
         # - **ENABLE_ONLY_4_KAFKA_SCRAM_SHA_256**: SCRAM-SHA-256 is used to encrypt the connection with a Kafka cluster.
@@ -18455,15 +18623,15 @@
         self.ip = ip
         # The SID of the Oracle database. 
         # 
         # > This parameter is returned only if the returned value of **EngineName** of the source instance is **Oracle** and the Oracle database is deployed in a non-RAC architecture.
         self.oracle_sid = oracle_sid
         # The port number of the source instance.
         self.port = port
-        # The ID of the region in which the source instance resides. For more information, see [Supported regions](~~141033~~).
+        # The ID of the region in which the source instance resides. For more information, see [Supported regions](https://help.aliyun.com/document_detail/141033.html).
         self.region = region
         # Indicates whether SSL encryption is enabled. Valid values:
         # 
         # - **DISABLE**: SSL encryption is disabled. 
         # - **ENABLE_WITH_CERTIFICATE**: SSL encryption is enabled and the CA certificate is uploaded. 
         # - **ENABLE_ONLY_4_MONGODB_ALTAS**: SSL encryption is enabled for the connection with an AWS MongoDB Altas database. 
         # - **ENABLE_ONLY_4_KAFKA_SCRAM_SHA_256**: SCRAM-SHA-256 is used to encrypt the connection with a Kafka cluster.
@@ -18635,15 +18803,15 @@
         self.delay = delay
         # The connection settings of the destination instance.
         self.destination_endpoint = destination_endpoint
         # The ID of the data synchronization instance.
         self.dts_instance_id = dts_instance_id
         # The instance class. 
         # 
-        # > For more information about the test performance of each instance class, see [Specifications of data synchronization instances](~~26605~~).
+        # > For more information about the test performance of each instance class, see [Specifications of data synchronization instances](https://help.aliyun.com/document_detail/26605.html).
         self.dts_job_class = dts_job_class
         # The synchronization direction. **Reverse** is returned.
         self.dts_job_direction = dts_job_direction
         # The ID of the synchronization task.
         self.dts_job_id = dts_job_id
         # The name of the data synchronization task.
         self.dts_job_name = dts_job_name
@@ -18674,15 +18842,15 @@
         # - **PrePaid**: subscription
         # - **PostPaid**: pay-as-you-go
         self.pay_type = pay_type
         # The performance of the data synchronization instance.
         self.performance = performance
         # The precheck state.
         self.precheck_status = precheck_status
-        # The reserved parameter of DTS. The value is a JSON string. You can specify this parameter to meet specific requirements, for example, whether to automatically start a precheck. For more information, see [MigrationReserved](~~176470~~).
+        # The reserved parameter of DTS. The value is a JSON string. You can specify this parameter to meet specific requirements, for example, whether to automatically start a precheck. For more information, see [MigrationReserved](https://help.aliyun.com/document_detail/176470.html).
         self.reserved = reserved
         # The connection settings of the source instance.
         self.source_endpoint = source_endpoint
         # The state of the DTS instance. For more information about the valid values, see the description of the request parameter **Status**.
         self.status = status
         # The state of initial schema synchronization.
         self.structure_initialization_status = structure_initialization_status
@@ -18895,15 +19063,15 @@
         self.ip = ip
         # The SID of the Oracle database. 
         # 
         # > This parameter is returned only if the returned value of **EngineName** of the source instance is **Oracle** and the Oracle database is deployed in a non-RAC architecture.
         self.oracle_sid = oracle_sid
         # The port number of the source instance.
         self.port = port
-        # The ID of the region in which the source instance resides. For more information, see [Supported regions](~~141033~~).
+        # The ID of the region in which the source instance resides. For more information, see [Supported regions](https://help.aliyun.com/document_detail/141033.html).
         self.region = region
         # Indicates whether SSL encryption is enabled. Valid values:
         # 
         # - **DISABLE**: SSL encryption is disabled. 
         # - **ENABLE_WITH_CERTIFICAT**E: SSL encryption is enabled and the CA certificate is uploaded. 
         # - **ENABLE_ONLY_4_MONGODB_ALTAS**: SSL encryption is enabled for the connection with an AWS MongoDB Altas database. 
         # - **ENABLE_ONLY_4_KAFKA_SCRAM_SHA_256**: SCRAM-SHA-256 is used to encrypt the connection with a Kafka cluster.
@@ -19119,15 +19287,15 @@
         self.app_name = app_name
         # The start of the time range for change tracking. The time follows the ISO 8601 standard in the *yyyy-MM-dd*T*HH:mm:ss*Z format. The time is displayed in UTC.
         self.begin_timestamp = begin_timestamp
         # The start offset of incremental data synchronization. The value is a UNIX timestamp representing the number of seconds that have elapsed since the epoch time January 1, 1970, 00:00:00 UTC.
         self.checkpoint = checkpoint
         # The consumption checkpoint of the change tracking instance. The time follows the ISO 8601 standard in the *yyyy-MM-dd*T*HH:mm:ss*Z format. The time is displayed in UTC.
         self.consumption_checkpoint = consumption_checkpoint
-        # The downstream client information, in the following format: \<IP address of the downstream client>:\<Random ID generated by DTS>.
+        # The downstream client information, in the following format: \\<IP address of the downstream client>:\\<Random ID generated by DTS>.
         self.consumption_client = consumption_client
         # The CPU utilization of the instance. Unit: percentage.
         self.cpu_usage = cpu_usage
         # The point in time when the task was created. The time follows the ISO 8601 standard in the *yyyy-MM-dd*T*HH:mm:ss*Z format. The time is displayed in UTC.
         self.create_time = create_time
         # The state of the physical gateway-based migration task.
         self.data_cloud_status = data_cloud_status
@@ -19152,15 +19320,15 @@
         # - **normal**\
         # - **online**\
         self.dts_bis_label = dts_bis_label
         # The ID of the data synchronization instance.
         self.dts_instance_id = dts_instance_id
         # The instance class.
         # 
-        # >  For more information about the test performance of each instance class, see [Specifications of data synchronization instances](~~26605~~).
+        # >  For more information about the test performance of each instance class, see [Specifications of data synchronization instances](https://help.aliyun.com/document_detail/26605.html).
         self.dts_job_class = dts_job_class
         # The synchronization direction. The value is **Reverse**.
         self.dts_job_direction = dts_job_direction
         # The ID of the data synchronization task.
         self.dts_job_id = dts_job_id
         # The name of the data synchronization task.
         self.dts_job_name = dts_job_name
@@ -19217,15 +19385,15 @@
         # *   **PrePaid**: subscription
         # *   **PostPaid**: pay-as-you-go
         self.pay_type = pay_type
         # The performance of the data migration or synchronization instance.
         self.performance = performance
         # The precheck state.
         self.precheck_status = precheck_status
-        # The reserved parameter of DTS. The value is a JSON string. You can specify this parameter to meet specific requirements, for example, whether to automatically start a precheck. For more information, see [MigrationReserved](~~176470~~).
+        # The reserved parameter of DTS. The value is a JSON string. You can specify this parameter to meet specific requirements, for example, whether to automatically start a precheck. For more information, see [MigrationReserved](https://help.aliyun.com/document_detail/176470.html).
         self.reserved = reserved
         # The name of the resource group.
         self.resource_group_display_name = resource_group_display_name
         # The resource group ID.
         self.resource_group_id = resource_group_id
         # The information about the retries performed by DTS due to an exception.
         self.retry_state = retry_state
@@ -19650,15 +19818,15 @@
         # The error message returned if incremental data migration or synchronization failed.
         self.error_message = error_message
         # Indicates whether the instance needs to be upgraded. Valid values:
         # 
         # - **true**\
         # - **false**\
         # 
-        # > To upgrade a DTS instance, call the [TransferInstanceClass](~~281093~~) operation.
+        # > To upgrade a DTS instance, call the [TransferInstanceClass](https://help.aliyun.com/document_detail/281093.html) operation.
         self.need_upgrade = need_upgrade
         # The progress of incremental data migration or synchronization. Unit: percentage.
         self.percent = percent
         # The number of entries that have been migrated or synchronized during incremental data migration or synchronization.
         self.progress = progress
         # The state of incremental data migration or synchronization. Valid values:
         # 
@@ -19731,15 +19899,15 @@
         self.ip = ip
         # The SID of the Oracle database. 
         # 
         # > This parameter is returned only if the returned value of **EngineName** of the destination instance is **Oracle** and the Oracle database is deployed in a non-RAC architecture.
         self.oracle_sid = oracle_sid
         # The port number of the destination instance.
         self.port = port
-        # The ID of the region in which the destination instance resides. For more information, see [Supported regions](~~141033~~).
+        # The ID of the region in which the destination instance resides. For more information, see [Supported regions](https://help.aliyun.com/document_detail/141033.html).
         self.region = region
         # Indicates whether SSL encryption is enabled. Valid values:
         # 
         # - **DISABLE**: SSL encryption is disabled. 
         # - **ENABLE_WITH_CERTIFICATE**: SSL encryption is enabled and the CA certificate is uploaded. 
         # - **ENABLE_ONLY_4_MONGODB_ALTAS**: SSL encryption is enabled for the connection with an AWS MongoDB Altas database. 
         # - **ENABLE_ONLY_4_KAFKA_SCRAM_SHA_256**: SCRAM-SHA-256 is used to encrypt the connection with a Kafka cluster.
@@ -20165,15 +20333,15 @@
         # The error message returned if incremental data synchronization failed.
         self.error_message = error_message
         # Indicates whether the instance needs to be upgraded. Valid values:
         # 
         # - **true**\
         # - **false**\
         # 
-        # > To upgrade a DTS instance, call the [TransferInstanceClass](~~281093~~) operation.
+        # > To upgrade a DTS instance, call the [TransferInstanceClass](https://help.aliyun.com/document_detail/281093.html) operation.
         self.need_upgrade = need_upgrade
         # The progress of incremental data synchronization. Unit: percentage.
         self.percent = percent
         # The number of entries that have been migrated or synchronized during incremental data migration or synchronization.
         self.progress = progress
         # The state of incremental data synchronization.
         self.status = status
@@ -20240,15 +20408,15 @@
         self.ip = ip
         # The SID of the Oracle database. 
         # 
         # > This parameter is returned only if the returned value of **EngineName** of the destination instance is **Oracle** and the Oracle database is deployed in a non-RAC architecture.
         self.oracle_sid = oracle_sid
         # The port number of the destination instance.
         self.port = port
-        # The ID of the region in which the destination instance resides. For more information, see [Supported regions](~~141033~~).
+        # The ID of the region in which the destination instance resides. For more information, see [Supported regions](https://help.aliyun.com/document_detail/141033.html).
         self.region = region
         # Indicates whether SSL encryption is enabled. Valid values:
         # 
         # - **DISABLE**: SSL encryption is disabled. 
         # - **ENABLE_WITH_CERTIFICATE**: SSL encryption is enabled and the CA certificate is uploaded. 
         # - **ENABLE_ONLY_4_MONGODB_ALTAS**: SSL encryption is enabled for the connection with an AWS MongoDB Altas database. 
         # - **ENABLE_ONLY_4_KAFKA_SCRAM_SHA_256**: SCRAM-SHA-256 is used to encrypt the connection with a Kafka cluster.
@@ -20550,15 +20718,15 @@
         self.ip = ip
         # The SID of the Oracle database. 
         # 
         # > This parameter is returned only if the returned value of **EngineName** of the source instance is **Oracle** and the Oracle database is deployed in a non-RAC architecture.
         self.oracle_sid = oracle_sid
         # The port number of the source instance.
         self.port = port
-        # The ID of the region in which the source instance resides. For more information, see [Supported regions](~~141033~~).
+        # The ID of the region in which the source instance resides. For more information, see [Supported regions](https://help.aliyun.com/document_detail/141033.html).
         self.region = region
         # Indicates whether SSL encryption is enabled. Valid values:
         # 
         # - **DISABLE**: SSL encryption is disabled. 
         # - **ENABLE_WITH_CERTIFICATE**: SSL encryption is enabled and the CA certificate is uploaded. 
         # - **ENABLE_ONLY_4_MONGODB_ALTAS**: SSL encryption is enabled for the connection with an AWS MongoDB Altas database. 
         # - **ENABLE_ONLY_4_KAFKA_SCRAM_SHA_256**: SCRAM-SHA-256 is used to encrypt the connection with a Kafka cluster.
@@ -20717,15 +20885,15 @@
         self.delay = delay
         # The connection settings of the destination instance.
         self.destination_endpoint = destination_endpoint
         # The ID of the data synchronization instance.
         self.dts_instance_id = dts_instance_id
         # The instance class. 
         # 
-        # > For more information about the test performance of each instance class, see [Specifications of data synchronization instances](~~26605~~).
+        # > For more information about the test performance of each instance class, see [Specifications of data synchronization instances](https://help.aliyun.com/document_detail/26605.html).
         self.dts_job_class = dts_job_class
         # The synchronization direction. **Reverse** is returned.
         self.dts_job_direction = dts_job_direction
         # The ID of the synchronization task.
         self.dts_job_id = dts_job_id
         # The name of the data synchronization task.
         self.dts_job_name = dts_job_name
@@ -20744,15 +20912,15 @@
         # - **PrePaid**: subscription
         # - **PostPaid**: pay-as-you-go
         self.pay_type = pay_type
         # The performance of the data migration or synchronization instance.
         self.performance = performance
         # The precheck state.
         self.precheck_status = precheck_status
-        # The reserved parameter of DTS. The value is a JSON string. You can specify this parameter to meet specific requirements, for example, whether to automatically start a precheck. For more information, see [MigrationReserved](~~176470~~).
+        # The reserved parameter of DTS. The value is a JSON string. You can specify this parameter to meet specific requirements, for example, whether to automatically start a precheck. For more information, see [MigrationReserved](https://help.aliyun.com/document_detail/176470.html).
         self.reserved = reserved
         # The connection settings of the source instance.
         self.source_endpoint = source_endpoint
         # The state of the DTS instance. For more information about the valid values, see the description of the request parameter **Status**.
         self.status = status
         # The state of initial schema synchronization.
         self.structure_initialization_status = structure_initialization_status
@@ -20914,15 +21082,15 @@
         self.ip = ip
         # The SID of the Oracle database. 
         # 
         # > This parameter is returned only if the returned value of **EngineName** of the source instance is **Oracle** and the Oracle database is deployed in a non-RAC architecture.
         self.oracle_sid = oracle_sid
         # The port number of the source instance.
         self.port = port
-        # The ID of the region in which the source instance resides. For more information, see [Supported regions](~~141033~~).
+        # The ID of the region in which the source instance resides. For more information, see [Supported regions](https://help.aliyun.com/document_detail/141033.html).
         self.region = region
         # Indicates whether SSL encryption is enabled. Valid values:
         # 
         # - **DISABLE**: SSL encryption is disabled. 
         # - **ENABLE_WITH_CERTIFICATE**: SSL encryption is enabled and the CA certificate is uploaded. 
         # - **ENABLE_ONLY_4_MONGODB_ALTAS**: SSL encryption is enabled for the connection with an AWS MongoDB Altas database. 
         # - **ENABLE_ONLY_4_KAFKA_SCRAM_SHA_256**: SCRAM-SHA-256 is used to encrypt the connection with a Kafka cluster.
@@ -21133,27 +21301,27 @@
         # 
         # > This parameter collection is returned only if an ETL task is configured.
         self.data_etl_status = data_etl_status
         # The state of full data migration or initial full data synchronization.
         self.data_initialization_status = data_initialization_status
         # The state of incremental data migration or synchronization.
         self.data_synchronization_status = data_synchronization_status
-        # The objects of the data migration, data synchronization, or change tracking task. For more information, see [Objects of DTS tasks](~~209545~~).
+        # The objects of the data migration, data synchronization, or change tracking task. For more information, see [Objects of DTS tasks](https://help.aliyun.com/document_detail/209545.html).
         self.db_object = db_object
         # The latency of incremental data migration or synchronization. 
         # 
         # > If you query data migration tasks, the unit of this parameter is milliseconds. If you query data synchronization tasks, the unit of this parameter is seconds.
         self.delay = delay
         # The connection settings of the destination instance.
         self.destination_endpoint = destination_endpoint
         # The ID of the data migration, data synchronization, or change tracking instance.
         self.dts_instance_id = dts_instance_id
         # The instance class. 
         # 
-        # > For more information about the test performance of each instance class, see [Specifications of data migration instances](~~26606~~) and [Specifications of data synchronization instances](~~26605~~).
+        # > For more information about the test performance of each instance class, see [Specifications of data migration instances](https://help.aliyun.com/document_detail/26606.html) and [Specifications of data synchronization instances](https://help.aliyun.com/document_detail/26605.html).
         self.dts_job_class = dts_job_class
         # The synchronization direction. Valid values:
         # 
         # - **Forward**\
         # - **Reverse**\
         # 
         # > This parameter is returned only if the topology of the data synchronization instance is two-way synchronization.
@@ -21190,15 +21358,15 @@
         # - **PrePaid**: subscription 
         # - **PostPaid**: pay-as-you-go
         self.pay_type = pay_type
         # The performance of the data migration or synchronization instance.
         self.performance = performance
         # The precheck state.
         self.precheck_status = precheck_status
-        # The reserved parameter of DTS. The value is a JSON string. You can specify this parameter to meet specific requirements, for example, whether to automatically start a precheck. For more information, see [MigrationReserved](~~176470~~).
+        # The reserved parameter of DTS. The value is a JSON string. You can specify this parameter to meet specific requirements, for example, whether to automatically start a precheck. For more information, see [MigrationReserved](https://help.aliyun.com/document_detail/176470.html).
         self.reserved = reserved
         # The name of the resource group.
         self.resource_group_display_name = resource_group_display_name
         # The resource group ID.
         self.resource_group_id = resource_group_id
         # The information about the retries performed by DTS due to an exception.
         self.retry_state = retry_state
@@ -21594,33 +21762,33 @@
         start_time: int = None,
         status: str = None,
         sub_job_type: str = None,
         zero_etl_job: bool = None,
     ):
         # The ID of the data migration or synchronization task.
         self.dts_job_id = dts_job_id
-        # The end of the time range to query. You can call the [DescribePreCheckStatus](~~209718~~) operation to query the execution time of the subtasks.
+        # The end of the time range to query. You can call the [DescribePreCheckStatus](https://help.aliyun.com/document_detail/209718.html) operation to query the execution time of the subtasks.
         # 
-        # > *   To obtain the logs that are generated for DTS subtasks within a specific period of time, you can call the [DescribePreCheckStatus](~~209718~~) operation to query the execution time of the subtasks.
+        # > *   To obtain the logs that are generated for DTS subtasks within a specific period of time, you can call the [DescribePreCheckStatus](https://help.aliyun.com/document_detail/209718.html) operation to query the execution time of the subtasks.
         # >*   Specify the time in the 13-digit UNIX timestamp format. Unit: milliseconds. You can use a search engine to obtain a UNIX timestamp converter.
         self.end_time = end_time
         # The keyword that is passed to specify the query content.
         # 
         # >  Fuzzy match is used and the keyword is case-sensitive.
         self.keyword = keyword
         # The number of the page to return. The value must be an integer that is greater than 0 and less than or equal to the maximum value supported by the integer data type. Default value: **1**.
         self.page_number = page_number
         # The number of log entries to return on each page. Valid values: **20**, **50**, **100**, **500**, and **1000**. Default value: **20**.
         self.page_size = page_size
-        # The ID of the region in which the DTS instance resides. For more information, see [List of supported regions](~~141033~~).
+        # The ID of the region in which the DTS instance resides. For more information, see [List of supported regions](https://help.aliyun.com/document_detail/141033.html).
         self.region_id = region_id
         self.resource_group_id = resource_group_id
         # The beginning of the time range to query.
         # 
-        # > *   To obtain the logs that are generated for Data Transmission Service (DTS) subtasks within a specific period of time, you can call the [DescribePreCheckStatus](~~209718~~) operation to query the execution time of the subtasks.
+        # > *   To obtain the logs that are generated for Data Transmission Service (DTS) subtasks within a specific period of time, you can call the [DescribePreCheckStatus](https://help.aliyun.com/document_detail/209718.html) operation to query the execution time of the subtasks.
         # >*   Specify the time in the 13-digit UNIX timestamp format. Unit: milliseconds. You can use a search engine to obtain a UNIX timestamp converter.
         self.start_time = start_time
         # The log level. Separate multiple log levels with commas (,). Valid values:
         # 
         # *   **NORMAL**: displays the logs that are generated when the DTS task runs as expected.
         # *   **WARN**: displays the logs about severe issues that stop the DTS task from running.
         # *   **ERROR**: displays the logs about unexpected issues that stop specific processes form running.
@@ -21748,15 +21916,15 @@
         request_id: str = None,
         service_log_contexts: List[DescribeDtsServiceLogResponseBodyServiceLogContexts] = None,
         success: bool = None,
         total_record_count: int = None,
     ):
         # The dynamic error code. This parameter will be removed soon.
         self.dynamic_code = dynamic_code
-        # The dynamic part in the error message. This parameter is used to replace the \*\*%s\*\* variable in the **ErrMessage** parameter.
+        # The dynamic part in the error message. This parameter is used to replace the \\*\\*%s\\*\\* variable in the **ErrMessage** parameter.
         self.dynamic_message = dynamic_message
         # The error code returned if the request fails.
         self.err_code = err_code
         # The error message returned if the request fails.
         self.err_message = err_message
         # The HTTP status code that is returned.
         self.http_status_code = http_status_code
@@ -21895,15 +22063,17 @@
         # The ID of the Alibaba Cloud account. You do not need to specify this parameter because this parameter will be removed in the future.
         self.account_id = account_id
         # The client token that is used to ensure the idempotence of the request. You can use the client to generate the value, but you must ensure that it is unique among different requests. The **ClientToken** parameter can contain only ASCII characters and cannot exceed 64 characters in length.
         self.client_token = client_token
         self.owner_id = owner_id
         self.region_id = region_id
         self.resource_group_id = resource_group_id
-        # The task ID, which is returned after you call the [SwitchSynchronizationEndpoint](~~201858~~) operation.
+        # The task ID, which is returned after you call the [SwitchSynchronizationEndpoint](https://help.aliyun.com/document_detail/201858.html) operation.
+        # 
+        # This parameter is required.
         self.task_id = task_id
 
     def validate(self):
         pass
 
     def to_map(self):
         _map = super().to_map()
@@ -22055,17 +22225,19 @@
 class DescribeEtlJobLogsRequest(TeaModel):
     def __init__(
         self,
         dts_job_id: str = None,
         region_id: str = None,
         resource_group_id: str = None,
     ):
-        # The ID of the ETL task. You can call the [DescribeDtsJobs](~~209702~~) operation to query the task ID.
+        # The ID of the ETL task. You can call the [DescribeDtsJobs](https://help.aliyun.com/document_detail/209702.html) operation to query the task ID.
+        # 
+        # This parameter is required.
         self.dts_job_id = dts_job_id
-        # The ID of the region in which the Data Transmission Service (DTS) instance resides. You can call the [DescribeRegions](~~25609~~) operation to query the available Alibaba Cloud regions.
+        # The ID of the region in which the Data Transmission Service (DTS) instance resides. You can call the [DescribeRegions](https://help.aliyun.com/document_detail/25609.html) operation to query the available Alibaba Cloud regions.
         self.region_id = region_id
         self.resource_group_id = resource_group_id
 
     def validate(self):
         pass
 
     def to_map(self):
@@ -22298,15 +22470,17 @@
         self.owner_id = owner_id
         # The number of the page to return. The value must be an integer that is greater than **0** and does not exceed the maximum value of the Integer data type. Default value: **1**.
         self.page_num = page_num
         # The number of entries to return on each page. Valid values: **1** to **100**. Default value: **30**.
         self.page_size = page_size
         self.region_id = region_id
         self.resource_group_id = resource_group_id
-        # The ID of the data synchronization instance. You can call the [DescribeSynchronizationJobs](~~49454~~) operation to query the instance ID.
+        # The ID of the data synchronization instance. You can call the [DescribeSynchronizationJobs](https://help.aliyun.com/document_detail/49454.html) operation to query the instance ID.
+        # 
+        # This parameter is required.
         self.synchronization_job_id = synchronization_job_id
 
     def validate(self):
         pass
 
     def to_map(self):
         _map = super().to_map()
@@ -22807,17 +22981,19 @@
 class DescribeJobMonitorRuleRequest(TeaModel):
     def __init__(
         self,
         dts_job_id: str = None,
         region_id: str = None,
         resource_group_id: str = None,
     ):
-        # The ID of the data migration, data synchronization, or change tracking task. You can call the [DescribeDtsJobs](~~209702~~) operation to query the task ID.
+        # The ID of the data migration, data synchronization, or change tracking task. You can call the [DescribeDtsJobs](https://help.aliyun.com/document_detail/209702.html) operation to query the task ID.
+        # 
+        # This parameter is required.
         self.dts_job_id = dts_job_id
-        # The region ID of the DTS instance. For more information, see [List of supported regions](~~141033~~).
+        # The region ID of the DTS instance. For more information, see [List of supported regions](https://help.aliyun.com/document_detail/141033.html).
         self.region_id = region_id
         self.resource_group_id = resource_group_id
 
     def validate(self):
         pass
 
     def to_map(self):
@@ -22856,16 +23032,16 @@
         phone: str = None,
         state: str = None,
         times: int = None,
         type: str = None,
     ):
         # The threshold that triggers the alert.
         # 
-        # *   If the request parameter **Type** of the [CreateJobMonitorRule](~~212332~~) operation is set to **delay**, the unit of DelayRuleTime is seconds.
-        # *   If the request parameter **Type** of the [CreateJobMonitorRule](~~212332~~) operation is set to **full_timeout**, the unit of DelayRuleTime is hours.
+        # *   If the request parameter **Type** of the [CreateJobMonitorRule](https://help.aliyun.com/document_detail/212332.html) operation is set to **delay**, the unit of DelayRuleTime is seconds.
+        # *   If the request parameter **Type** of the [CreateJobMonitorRule](https://help.aliyun.com/document_detail/212332.html) operation is set to **full_timeout**, the unit of DelayRuleTime is hours.
         self.delay_rule_time = delay_rule_time
         self.job_id = job_id
         self.job_type = job_type
         self.notice_value = notice_value
         self.period = period
         # The mobile phone numbers that receive alert notifications. Multiple mobile numbers are separated by commas (,).
         self.phone = phone
@@ -23107,22 +23283,26 @@
         # *   **InternetOut**: the outbound traffic over the Internet. Unit: byte.
         # *   **diskusage_utilization**: the disk usage.
         # *   **IntranetInRate**: the inbound traffic over the internal network. Unit: byte.
         # *   **InternetIn**: the inbound traffic from the Internet. Unit: byte.
         # *   **cpu_total**: the CPU utilization.
         # *   **memory_usedutilization**: the memory usage.
         # *   **IntranetOutRate**: the outbound traffic over the internal network. Unit: byte.
+        # 
+        # This parameter is required.
         self.metric_name = metric_name
         # Specifies whether to query the metrics of the cluster or a node. Valid values:
         # 
         # *   **CLUSTER**: query the metrics of the cluster.
         # *   **NODE**: query the metrics of a node.
         self.metric_type = metric_type
         self.owner_id = owner_id
         # The monitored object. If the **MetricType** parameter is set to **NODE**, set this parameter to the ID of the node that is monitored.
+        # 
+        # This parameter is required.
         self.param = param
         # The monitoring interval. Unit: seconds. Minimum value: 15.
         self.period = period
         self.resource_group_id = resource_group_id
         # The timestamp that indicates the beginning of the time range to query. Unit: milliseconds.
         self.start_time = start_time
 
@@ -23402,14 +23582,16 @@
         resource_group_id: str = None,
     ):
         # The ID of the Alibaba Cloud account. You do not need to specify this parameter because this parameter will be removed in the future.
         self.account_id = account_id
         # The client token that is used to ensure the idempotence of the request. You can use the client to generate the value, but you must make sure that it is unique among different requests. The token can contain only ASCII characters and cannot exceed 64 characters in length.
         self.client_token = client_token
         # The ID of the data migration instance. You can call the **DescribeMigrationJobs** operation to query the instance ID.
+        # 
+        # This parameter is required.
         self.migration_job_id = migration_job_id
         self.owner_id = owner_id
         self.region_id = region_id
         self.resource_group_id = resource_group_id
 
     def validate(self):
         pass
@@ -23671,21 +23853,23 @@
     ):
         self.migration_mode = migration_mode
         # The ID of the Alibaba Cloud account. You do not need to specify this parameter because this parameter will be removed in the future.
         self.account_id = account_id
         # The client token that is used to ensure the idempotence of the request. You can use the client to generate the value, but you must make sure that the value is unique among different requests. The **ClientToken** value can contain only ASCII characters and cannot exceed 64 characters in length.
         self.client_token = client_token
         # The ID of the data migration instance. You can call the **DescribeMigrationJobs** operation to query the instance ID.
+        # 
+        # This parameter is required.
         self.migration_job_id = migration_job_id
         self.owner_id = owner_id
         # The number of the page to return. The value must be an integer that is greater than **0** and does not exceed the maximum value of the Integer data type. Default value: **1**.
         self.page_num = page_num
         # The number of entries to return on each page. Valid values: **30**, **50**, and **100**. Default value: **30**.
         self.page_size = page_size
-        # The ID of the region where the data migration instance resides. For more information, see [List of supported regions](~~141033~~).
+        # The ID of the region where the data migration instance resides. For more information, see [List of supported regions](https://help.aliyun.com/document_detail/141033.html).
         self.region_id = region_id
         self.resource_group_id = resource_group_id
 
     def validate(self):
         if self.migration_mode:
             self.migration_mode.validate()
 
@@ -24334,14 +24518,16 @@
         resource_group_id: str = None,
     ):
         # The ID of the Alibaba Cloud account. You do not need to specify this parameter because this parameter will be removed in the future.
         self.account_id = account_id
         # The client token that is used to ensure the idempotence of the request. You can use the client to generate the value, but you must make sure that the value is unique among different requests. The **ClientToken** value can contain only ASCII characters and cannot exceed 64 characters in length.
         self.client_token = client_token
         # The ID of the data migration instance. You can call the **DescribeMigrationJobs** operation to query the instance ID.
+        # 
+        # This parameter is required.
         self.migration_job_id = migration_job_id
         self.owner_id = owner_id
         self.region_id = region_id
         self.resource_group_id = resource_group_id
 
     def validate(self):
         pass
@@ -24938,15 +25124,15 @@
         self.data_synchronization_status = data_synchronization_status
         # The connection settings of the destination instance.
         self.destination_endpoint = destination_endpoint
         # The error code returned if the call failed.
         self.err_code = err_code
         # The error message returned if the call failed.
         self.err_message = err_message
-        # The specification of the data migration instance. Valid values: **small**, **medium**, **large**, **xlarge**, and **2xlarge**. For more information, see [Specifications of data migration instances](~~26606~~).
+        # The specification of the data migration instance. Valid values: **small**, **medium**, **large**, **xlarge**, and **2xlarge**. For more information, see [Specifications of data migration instances](https://help.aliyun.com/document_detail/26606.html).
         self.migration_job_class = migration_job_class
         # The ID of the data migration instance.
         self.migration_job_id = migration_job_id
         # The name of the data migration task.
         self.migration_job_name = migration_job_name
         # The status of the data migration task. Valid values:
         # 
@@ -25127,21 +25313,23 @@
 
 class DescribeMigrationJobsRequestTag(TeaModel):
     def __init__(
         self,
         key: str = None,
         value: str = None,
     ):
-        # The tag key. You can call the [ListTagResources](~~191187~~) operation to query the tag key.
+        # The tag key. You can call the [ListTagResources](https://help.aliyun.com/document_detail/191187.html) operation to query the tag key.
         # 
         # > 
         # *   N specifies the serial number of the tag. For example, Tag.1.Key specifies the key of the first tag and Tag.2.Key specifies the key of the second tag. You can specify 1 to 20 tag keys at a time.
         # *   This parameter cannot be an empty string.
+        # 
+        # This parameter is required.
         self.key = key
-        # The tag value. You can call the [ListTagResources](~~191187~~) operation to query the tag value.
+        # The tag value. You can call the [ListTagResources](https://help.aliyun.com/document_detail/191187.html) operation to query the tag value.
         # 
         # > 
         # *   N specifies the serial number of the tag. For example, Tag.1.Value specifies the value of the first tag and Tag.2.Value specifies the value of the second tag. You can specify 1 to 20 tag values at a time.
         # *   This parameter can be an empty string.
         self.value = value
 
     def validate(self):
@@ -25187,15 +25375,15 @@
         # >  Fuzzy match is supported.
         self.migration_job_name = migration_job_name
         self.owner_id = owner_id
         # The number of the page to return. The value must be an integer that is greater than **0** and does not exceed the maximum value of the Integer data type. Default value: **1**.
         self.page_num = page_num
         # The number of entries to return on each page. Valid values: **30**, **50**, and **100**. Default value: **30**.
         self.page_size = page_size
-        # The ID of the region where the data migration instances reside. For more information, see [List of supported regions](~~141033~~).
+        # The ID of the region where the data migration instances reside. For more information, see [List of supported regions](https://help.aliyun.com/document_detail/141033.html).
         self.region_id = region_id
         self.resource_group_id = resource_group_id
         self.tag = tag
 
     def validate(self):
         if self.tag:
             for k in self.tag:
@@ -25863,15 +26051,15 @@
         self.data_synchronization = data_synchronization
         # The connection settings of the destination instance.
         self.destination_endpoint = destination_endpoint
         # The time when the data migration instance was created. The time is displayed in the *yyyy-MM-dd*T*HH:mm:ss*Z format in UTC.
         self.instance_create_time = instance_create_time
         # The time when the data migration task was created. The time is displayed in the *yyyy-MM-dd*T*HH:mm:ss*Z format in UTC.
         self.job_create_time = job_create_time
-        # The specification of the data migration instance. Valid values: **small**, **medium**, **large**, **xlarge**, and **2xlarge**. For more information, see [Specifications of data migration instances](~~26606~~).
+        # The specification of the data migration instance. Valid values: **small**, **medium**, **large**, **xlarge**, and **2xlarge**. For more information, see [Specifications of data migration instances](https://help.aliyun.com/document_detail/26606.html).
         self.migration_job_class = migration_job_class
         # The ID of the data migration instance.
         self.migration_job_id = migration_job_id
         # The name of the data migration task.
         self.migration_job_name = migration_job_name
         # The status of the data migration task. Valid values:
         # 
@@ -26170,29 +26358,33 @@
         region_id: str = None,
         resource_group_id: str = None,
         struct_phase: str = None,
         struct_type: str = None,
         zero_etl_job: bool = None,
     ):
         # The ID of the data migration, data synchronization, or change tracking task.
+        # 
+        # This parameter is required.
         self.dts_job_id = dts_job_id
         # The task code that specifies the type of the DTS subtask. Valid values:
         # 
         # *   **01**: precheck
         # *   **02**: schema migration or initial schema synchronization
         # *   **03**: full data migration or initial full data synchronization
         # *   **04**: incremental data migration or synchronization
+        # 
+        # This parameter is required.
         self.job_code = job_code
         # The filter item used to filter tables in fuzzy match.
         self.name = name
         # The number of the page to return. The value must be an integer that is greater than **0** and does not exceed the maximum value of the Integer data type. Default value: **1**.
         self.page_no = page_no
         # The number of entries to return on each page. Default value: **20**.
         self.page_size = page_size
-        # The region ID of the DTS instance. For more information, see [List of supported regions](~~141033~~).
+        # The region ID of the DTS instance. For more information, see [List of supported regions](https://help.aliyun.com/document_detail/141033.html).
         self.region_id = region_id
         self.resource_group_id = resource_group_id
         # The filter item used to filter tables, views, and functions during schema migration.
         self.struct_phase = struct_phase
         # The type of schema definition. Valid values:
         # 
         # *   **before**: schema migration or initial schema synchronization
@@ -26952,15 +27144,15 @@
         # *   **Migrating**: The subtask is in progress. Data is being migrated.
         # *   **Failed**: The subtask failed.
         # *   **Warning**: The subtask encounters an exception.
         # *   **Success**: The subtask is complete.
         self.state = state
         # The sub-item progress of the subtask.
         # 
-        # >  If **\[]** is returned, the subtask has no sub-items.
+        # >  If **[]** is returned, the subtask has no sub-items.
         self.sub = sub
         # The names of the objects that are migrated or synchronized.
         self.target_names = target_names
         # The total number of subtasks.
         self.total = total
 
     def validate(self):
@@ -27316,15 +27508,15 @@
         # *   **Migrating**: The subtask is in progress. Data is being migrated.
         # *   **Failed**: The subtask failed.
         # *   **Catched**: The subtask is in progress. Incremental data is being migrated or synchronized.
         # *   **Finished**: The subtask is complete.
         self.state = state
         # The sub-item progress of the subtask.
         # 
-        # >  If **\[]** is returned, the subtask has no sub-items.
+        # >  If **[]** is returned, the subtask has no sub-items.
         self.sub = sub
         # The names of the objects that are migrated or synchronized.
         self.target_names = target_names
         # The total number of subtasks.
         self.total = total
 
     def validate(self):
@@ -27791,14 +27983,16 @@
         self.account_id = account_id
         # The client token that is used to ensure the idempotence of the request. You can use the client to generate the value, but you must ensure that it is unique among different requests. The token can contain only ASCII characters and cannot exceed 64 characters in length.
         self.client_token = client_token
         self.owner_id = owner_id
         self.region_id = region_id
         self.resource_group_id = resource_group_id
         # The ID of the change tracking instance. You can call the DescribeSubscriptionInstances operation to query the instance ID.
+        # 
+        # This parameter is required.
         self.subscription_instance_id = subscription_instance_id
 
     def validate(self):
         pass
 
     def to_map(self):
         _map = super().to_map()
@@ -27992,15 +28186,17 @@
         subscription_instance_id: str = None,
     ):
         # The ID of the Alibaba Cloud account. You do not need to specify this parameter because this parameter will be removed in the future.
         self.account_id = account_id
         self.owner_id = owner_id
         self.region_id = region_id
         self.resource_group_id = resource_group_id
-        # The ID of the change tracking instance. You can call the [DescribeSubscriptionInstances](~~49442~~) operation to query the instance ID.
+        # The ID of the change tracking instance. You can call the [DescribeSubscriptionInstances](https://help.aliyun.com/document_detail/49442.html) operation to query the instance ID.
+        # 
+        # This parameter is required.
         self.subscription_instance_id = subscription_instance_id
 
     def validate(self):
         pass
 
     def to_map(self):
         _map = super().to_map()
@@ -28287,15 +28483,15 @@
         success: str = None,
         task_id: str = None,
     ):
         # The start of the time range for change tracking. The time is displayed in the *yyyy-MM-dd*T*HH:mm:ss*Z format in UTC.
         self.begin_timestamp = begin_timestamp
         # The consumption checkpoint of the change tracking instance. The time is displayed in the *yyyy-MM-dd*T*HH:mm:ss*Z format in UTC.
         self.consumption_checkpoint = consumption_checkpoint
-        # The downstream client information, in the following format: \<IP address of the downstream client>:\<Random ID generated by DTS>.
+        # The downstream client information, in the following format: \\<IP address of the downstream client>:\\<Random ID generated by DTS>.
         self.consumption_client = consumption_client
         # The end of the time range for change tracking. The time is displayed in the *yyyy-MM-dd*T*HH:mm:ss*Z format in UTC.
         self.end_timestamp = end_timestamp
         # The error code returned if the call failed.
         self.err_code = err_code
         # The error message returned if the call failed.
         self.err_message = err_message
@@ -28317,15 +28513,15 @@
         # *   **PrecheckFailed**: The task failed to pass the precheck.
         # *   **Starting**: The task is being started.
         # *   **Normal**: The task is running as expected.
         # *   **Abnormal**: The task is not running as expected.
         self.status = status
         # The topic of the change tracking instance.
         # 
-        # >  This parameter is returned only if your change tracking instance is of the new version and you have called the [CreateConsumerGroup](~~122863~~) operation to create a consumer group.
+        # >  This parameter is returned only if your change tracking instance is of the new version and you have called the [CreateConsumerGroup](https://help.aliyun.com/document_detail/122863.html) operation to create a consumer group.
         self.subscribe_topic = subscribe_topic
         # The types of operations that are tracked by the task.
         self.subscription_data_type = subscription_data_type
         # The endpoint of the change tracking instance.
         self.subscription_host = subscription_host
         # The ID of the change tracking instance.
         self.subscription_instance_id = subscription_instance_id
@@ -28489,14 +28685,16 @@
         value: str = None,
     ):
         # The tag key.
         # 
         # > 
         # *   N specifies the serial number of the tag. For example, Tag.1.Key specifies the key of the first tag and Tag.2.Key specifies the key of the second tag. You can specify 1 to 20 tag keys at a time.
         # *   This parameter cannot be an empty string.
+        # 
+        # This parameter is required.
         self.key = key
         # The tag value.
         # 
         # > 
         # *   N specifies the serial number of the tag. For example, Tag.1.Value specifies the value of the first tag and Tag.2.Value specifies the value of the second tag. You can specify 1 to 20 tag values at a time.
         # *   This parameter can be an empty string.
         self.value = value
@@ -28543,15 +28741,15 @@
         # The client token that is used to ensure the idempotence of the request. You can use the client to generate the value, but you must make sure that it is unique among different requests. The **ClientToken** parameter can contain only ASCII characters and cannot exceed 64 characters in length.
         self.client_token = client_token
         self.owner_id = owner_id
         # The number of the page to return. The value must be an integer that is greater than **0** and does not exceed the maximum value of the Integer data type. Default value: **1**.
         self.page_num = page_num
         # The number of entries to return on each page. Valid values: **30**, **50**, and **100**. Default value: **30**.
         self.page_size = page_size
-        # The ID of the region where the change tracking instance resides. For more information, see [List of supported regions](~~49442~~).
+        # The ID of the region where the change tracking instance resides. For more information, see [List of supported regions](https://help.aliyun.com/document_detail/49442.html).
         self.region_id = region_id
         self.resource_group_id = resource_group_id
         # The name of the change tracking instance.
         # 
         # >  If you specify this parameter, DTS returns all the change tracking instances that match the specified name.
         self.subscription_instance_name = subscription_instance_name
         self.tag = tag
@@ -28936,15 +29134,15 @@
         subscription_object: DescribeSubscriptionInstancesResponseBodySubscriptionInstancesSubscriptionInstanceSubscriptionObject = None,
         tags: DescribeSubscriptionInstancesResponseBodySubscriptionInstancesSubscriptionInstanceTags = None,
     ):
         # The start of the time range for change tracking. The time is displayed in the *yyyy-MM-dd*T*HH:mm:ss*Z format in UTC.
         self.begin_timestamp = begin_timestamp
         # The consumption checkpoint of the change tracking instance. The time is displayed in the *yyyy-MM-dd*T*HH:mm:ss*Z format in UTC.
         self.consumption_checkpoint = consumption_checkpoint
-        # The downstream client information, in the following format: \<IP address of the downstream client>:\<Random ID generated by DTS>.
+        # The downstream client information, in the following format: \\<IP address of the downstream client>:\\<Random ID generated by DTS>.
         self.consumption_client = consumption_client
         # The end of the time range for change tracking. The time is displayed in the *yyyy-MM-dd*T*HH:mm:ss*Z format in UTC.
         self.end_timestamp = end_timestamp
         # The error message returned if change tracking failed.
         self.error_message = error_message
         # The time when the change tracking instance was created. The time is displayed in the *yyyy-MM-dd*T*HH:mm:ss*Z format. The time must be in UTC.
         self.instance_create_time = instance_create_time
@@ -28964,15 +29162,15 @@
         # *   **PrecheckFailed**: The task failed to pass the precheck.
         # *   **Starting**: The task is being started.
         # *   **Normal**: The task is running as expected.
         # *   **Abnormal**: The task is not running as expected.
         self.status = status
         # The topic of the change tracking instance.
         # 
-        # >  This parameter is returned only if your change tracking instances are of the new version and you have called the [CreateConsumerGroup](~~122863~~) operation to create a consumer group.
+        # >  This parameter is returned only if your change tracking instances are of the new version and you have called the [CreateConsumerGroup](https://help.aliyun.com/document_detail/122863.html) operation to create a consumer group.
         self.subscribe_topic = subscribe_topic
         # The types of operations that are tracked by the task.
         self.subscription_data_type = subscription_data_type
         # The endpoint of the change tracking instance.
         self.subscription_host = subscription_host
         # The ID of the change tracking instance.
         self.subscription_instance_id = subscription_instance_id
@@ -29248,14 +29446,16 @@
     ):
         # The ID of the distributed change tracking instance.
         self.dts_instance_id = dts_instance_id
         # The ID of the region in which the change tracking instance resides.
         self.region_id = region_id
         self.resource_group_id = resource_group_id
         # The ID of the consumer group.
+        # 
+        # This parameter is required.
         self.sid = sid
         # The IDs of all subtasks in the distributed change tracking task. Separate multiple subtask IDs with commas (,).
         # 
         # >  You must specify at least one of the SubMigrationJobIds and **Topics** parameters. We recommend that you specify the SubMigrationJobIds parameter.
         self.sub_migration_job_ids = sub_migration_job_ids
         # The topics of all subtasks in the distributed change tracking task. Separate multiple topics with commas (,).
         # 
@@ -29314,14 +29514,16 @@
     ):
         # The ID of the distributed change tracking instance.
         self.dts_instance_id = dts_instance_id
         # The ID of the region in which the change tracking instance resides.
         self.region_id = region_id
         self.resource_group_id = resource_group_id
         # The ID of the consumer group.
+        # 
+        # This parameter is required.
         self.sid = sid
         # The IDs of all subtasks in the distributed change tracking task. Separate multiple subtask IDs with commas (,).
         # 
         # >  You must specify at least one of the SubMigrationJobIds and **Topics** parameters. We recommend that you specify the SubMigrationJobIds parameter.
         self.sub_migration_job_ids_shrink = sub_migration_job_ids_shrink
         # The topics of all subtasks in the distributed change tracking task. Separate multiple topics with commas (,).
         # 
@@ -29377,15 +29579,15 @@
         sid: str = None,
         topic: str = None,
     ):
         # The consumer offset of the subtask. It is a UNIX timestamp that is generated when the client consumes the first data record. Unit: seconds.
         # 
         # >  You can use a search engine to obtain a UNIX timestamp converter.
         self.checkpoint = checkpoint
-        # The objects of the subtask. For more information, see [Objects of DTS tasks](~~209545~~).
+        # The objects of the subtask. For more information, see [Objects of DTS tasks](https://help.aliyun.com/document_detail/209545.html).
         self.dblist = dblist
         # The endpoint and port number of the change tracking instance.
         self.dproxy_url = dproxy_url
         # The consumer group ID of the subtask.
         self.sid = sid
         # The topic of the subtask.
         self.topic = topic
@@ -29792,14 +29994,16 @@
         # 
         # *   **Forward**\
         # *   **Reverse**\
         # 
         # >  Default value: **Forward**.
         self.synchronization_direction = synchronization_direction
         # The ID of the data synchronization instance. You can call the **DescribeSynchronizationJobs** operation to query the instance ID.
+        # 
+        # This parameter is required.
         self.synchronization_job_id = synchronization_job_id
 
     def validate(self):
         pass
 
     def to_map(self):
         _map = super().to_map()
@@ -30023,15 +30227,17 @@
         # *   **Forward**\
         # *   **Reverse**\
         # 
         # > 
         # *   Default value: **Forward**.
         # *   This parameter is required only when the topology of the data synchronization instance is two-way synchronization.
         self.synchronization_direction = synchronization_direction
-        # The ID of the data synchronization instance. You can call the [DescribeSynchronizationJobs](~~49454~~) operation to query the instance ID.
+        # The ID of the data synchronization instance. You can call the [DescribeSynchronizationJobs](https://help.aliyun.com/document_detail/49454.html) operation to query the instance ID.
+        # 
+        # This parameter is required.
         self.synchronization_job_id = synchronization_job_id
 
     def validate(self):
         pass
 
     def to_map(self):
         _map = super().to_map()
@@ -30186,27 +30392,29 @@
         synchronization_job_id: str = None,
     ):
         # The ID of the Alibaba Cloud account. You do not need to specify this parameter because this parameter will be removed in the future.
         self.account_id = account_id
         # The client token that is used to ensure the idempotence of the request. You can use the client to generate the value, but you must make sure that the value is unique among different requests. The **ClientToken** value can contain only ASCII characters and cannot exceed 64 characters in length.
         self.client_token = client_token
         self.owner_id = owner_id
-        # The ID of the region where the data synchronization instance resides. For more information, see [List of supported regions](~~141033~~).
+        # The ID of the region where the data synchronization instance resides. For more information, see [List of supported regions](https://help.aliyun.com/document_detail/141033.html).
         self.region_id = region_id
         self.resource_group_id = resource_group_id
         # The synchronization direction. Valid values:
         # 
         # *   **Forward**\
         # *   **Reverse**\
         # 
         # >  Default value: **Forward**.
         # 
         # The value **Reverse** takes effect only if the topology of the data synchronization instance is two-way synchronization.
         self.synchronization_direction = synchronization_direction
-        # The ID of the data synchronization instance. You can call the [DescribeSynchronizationJobs](~~49454~~) operation to query the instance ID.
+        # The ID of the data synchronization instance. You can call the [DescribeSynchronizationJobs](https://help.aliyun.com/document_detail/49454.html) operation to query the instance ID.
+        # 
+        # This parameter is required.
         self.synchronization_job_id = synchronization_job_id
 
     def validate(self):
         pass
 
     def to_map(self):
         _map = super().to_map()
@@ -31129,15 +31337,17 @@
         # The ID of the Alibaba Cloud account. You do not need to specify this parameter because this parameter will be removed in the future.
         self.account_id = account_id
         # The client token that is used to ensure the idempotence of the request. You can use the client to generate the value, but you must ensure that it is unique among different requests. The **ClientToken** parameter can contain only ASCII characters and cannot exceed 64 characters in length.
         self.client_token = client_token
         self.owner_id = owner_id
         self.region_id = region_id
         self.resource_group_id = resource_group_id
-        # The IDs of the data synchronization instances. The value is a JSON array. You can call the [DescribeSynchronizationJobs](~~49454~~) operation to query the instance IDs.
+        # The IDs of the data synchronization instances. The value is a JSON array. You can call the [DescribeSynchronizationJobs](https://help.aliyun.com/document_detail/49454.html) operation to query the instance IDs.
+        # 
+        # This parameter is required.
         self.synchronization_job_id_list_json_str = synchronization_job_id_list_json_str
 
     def validate(self):
         pass
 
     def to_map(self):
         _map = super().to_map()
@@ -31406,14 +31616,16 @@
 class DescribeSynchronizationJobsRequestTag(TeaModel):
     def __init__(
         self,
         key: str = None,
         value: str = None,
     ):
         # The ID of the request.
+        # 
+        # This parameter is required.
         self.key = key
         # The maximum number of entries that can be displayed on the current page.
         self.value = value
 
     def validate(self):
         pass
 
@@ -31449,15 +31661,15 @@
         region_id: str = None,
         resource_group_id: str = None,
         synchronization_job_name: str = None,
         tag: List[DescribeSynchronizationJobsRequestTag] = None,
     ):
         # The page number of the returned page.
         self.account_id = account_id
-        # The tag value. You can call the [ListTagResources](~~191187~~) operation to query the tag value.
+        # The tag value. You can call the [ListTagResources](https://help.aliyun.com/document_detail/191187.html) operation to query the tag value.
         # 
         # > 
         # *   N specifies the serial number of the tag. For example, Tag.1.Value specifies the value of the first tag and Tag.2.Value specifies the value of the second tag. You can specify 1 to 20 tag values at a time.
         # *   This parameter can be an empty string.
         self.client_token = client_token
         self.owner_id = owner_id
         # The ID of the Alibaba Cloud account. You do not need to specify this parameter because this parameter will be removed in the future.
@@ -31465,15 +31677,15 @@
         # The client token that is used to ensure the idempotence of the request. You can use the client to generate the value, but you must make sure that the value is unique among different requests. The **ClientToken** value can contain only ASCII characters and cannot exceed 64 characters in length.
         self.page_size = page_size
         # The name of the data synchronization task.
         # 
         # >  Fuzzy matching is supported.
         self.region_id = region_id
         self.resource_group_id = resource_group_id
-        # The tag key. You can call the [ListTagResources](~~191187~~) operation to query the tag key.
+        # The tag key. You can call the [ListTagResources](https://help.aliyun.com/document_detail/191187.html) operation to query the tag key.
         # 
         # > 
         # *   N specifies the serial number of the tag. For example, Tag.1.Key specifies the key of the first tag and Tag.2.Key specifies the key of the second tag. You can specify 1 to 20 tag keys at a time.
         # *   This parameter cannot be an empty string.
         self.synchronization_job_name = synchronization_job_name
         self.tag = tag
 
@@ -32489,18 +32701,20 @@
         task_id: str = None,
     ):
         # The ID of the Alibaba Cloud account. You do not need to specify this parameter because this parameter will be removed in the future.
         self.account_id = account_id
         # The client token that is used to ensure the idempotence of the request. You can use the client to generate the value, but you must make sure that the value is unique among different requests. The **ClientToken** value can contain only ASCII characters and cannot exceed 64 characters in length.
         self.client_token = client_token
         self.owner_id = owner_id
-        # The ID of the region where the data synchronization instance resides. For more information, see [List of supported regions](~~141033~~).
+        # The ID of the region where the data synchronization instance resides. For more information, see [List of supported regions](https://help.aliyun.com/document_detail/141033.html).
         self.region_id = region_id
         self.resource_group_id = resource_group_id
-        # The task ID, which is returned after you call the [ModifySynchronizationObject](~~49451~~) operation to modify the objects to be synchronized.
+        # The task ID, which is returned after you call the [ModifySynchronizationObject](https://help.aliyun.com/document_detail/49451.html) operation to modify the objects to be synchronized.
+        # 
+        # This parameter is required.
         self.task_id = task_id
 
     def validate(self):
         pass
 
     def to_map(self):
         _map = super().to_map()
@@ -32977,18 +33191,18 @@
         # 
         # >  By default, if the parameter is left empty, custom tags and system tags are returned.
         self.category = category
         # The number of the page to return. Pages start from page 1. Default value: 1. This parameter is used together with PageSize.
         self.page_number = page_number
         # The number of tags to return on each page if the DTS instance has multiple tags. Default value: 20.
         self.page_size = page_size
-        # The region ID of the DTS instance. For more information, see [List of supported regions](~~141033~~).
+        # The region ID of the DTS instance. For more information, see [List of supported regions](https://help.aliyun.com/document_detail/141033.html).
         self.region_id = region_id
         self.resource_group_id = resource_group_id
-        # The ID of the data migration, data synchronization, or change tracking instance. You can call the [DescribeDtsJobs](~~209702~~) operation to query the instance ID.
+        # The ID of the data migration, data synchronization, or change tracking instance. You can call the [DescribeDtsJobs](https://help.aliyun.com/document_detail/209702.html) operation to query the instance ID.
         self.resource_id = resource_id
         # The resource type. Set the value to **ALIYUN::DTS::INSTANCE**.
         self.resource_type = resource_type
 
     def validate(self):
         pass
 
@@ -33160,18 +33374,18 @@
         # 
         # >  This parameter is required.
         self.key = key
         # The page number of the start page to return for a tag key that has multiple values. The valid value ranges from 1 to the maximum value of the INTEGER data type. This parameter is often used with the PageSize parameter. Default value: 1.
         self.page_number = page_number
         # The number of tag values to return each time for a tag key that has multiple values. Default value: 20.
         self.page_size = page_size
-        # The region ID of the DTS instance. For more information, see [List of supported regions](~~141033~~).
+        # The region ID of the DTS instance. For more information, see [List of supported regions](https://help.aliyun.com/document_detail/141033.html).
         self.region_id = region_id
         self.resource_group_id = resource_group_id
-        # The ID of the data migration, data synchronization, or change tracking instance. You can call the [DescribeDtsJobs](~~209702~~) operation to query the instance ID.
+        # The ID of the data migration, data synchronization, or change tracking instance. You can call the [DescribeDtsJobs](https://help.aliyun.com/document_detail/209702.html) operation to query the instance ID.
         # 
         # >  If this parameter is left empty, the values of all tag keys of the current user are returned.
         self.resource_id = resource_id
         # The resource type. Set the value to **ALIYUN::DTS::INSTANCE**.
         self.resource_type = resource_type
 
     def validate(self):
@@ -34014,19 +34228,23 @@
         resource_type: str = None,
         tag: List[ListTagResourcesRequestTag] = None,
     ):
         # The query token.
         # 
         # >  If a query does not return all results, you can specify the returned **NextToken** parameter in the next query to obtain more results.
         self.next_token = next_token
-        # The ID of the region where the data migration, data synchronization, or change tracking instance resides. For more information, see [List of supported regions](~~141033~~).
+        # The ID of the region where the data migration, data synchronization, or change tracking instance resides. For more information, see [List of supported regions](https://help.aliyun.com/document_detail/141033.html).
+        # 
+        # This parameter is required.
         self.region_id = region_id
         self.resource_group_id = resource_group_id
         self.resource_id = resource_id
         # The resource type. Valid value: **ALIYUN::DTS::INSTANCE**.
+        # 
+        # This parameter is required.
         self.resource_type = resource_type
         self.tag = tag
 
     def validate(self):
         if self.tag:
             for k in self.tag:
                 if k:
@@ -34274,37 +34492,41 @@
         consumer_group_password: str = None,
         consumer_group_user_name: str = None,
         dts_instance_id: str = None,
         dts_job_id: str = None,
         region_id: str = None,
         resource_group_id: str = None,
     ):
-        # The ID of the consumer group. You can call the [DescribeConsumerChannel](~~264169~~) operation to query the consumer group ID.
+        # The ID of the consumer group. You can call the [DescribeConsumerChannel](https://help.aliyun.com/document_detail/264169.html) operation to query the consumer group ID.
+        # 
+        # This parameter is required.
         self.consumer_group_id = consumer_group_id
         # The name of the consumer group. The name cannot exceed 128 characters in length. We recommend that you use an informative name for easy identification.
         self.consumer_group_name = consumer_group_name
         # The new password of the consumer group.
         # 
         # *   A password must contain two or more of the following characters: uppercase letters, lowercase letters, digits, and special characters.
         # *   A password must be 8 to 32 characters in length.
         self.consumer_group_password = consumer_group_password
         # The new username of the consumer group.
         # 
-        # *   A username can contain one or more of the following character types: uppercase letters, lowercase letters, digits, and underscores (\_).
+        # *   A username can contain one or more of the following character types: uppercase letters, lowercase letters, digits, and underscores (_).
         # *   A username cannot exceed 16 characters in length.
         self.consumer_group_user_name = consumer_group_user_name
-        # The ID of the change tracking instance. You can call the [DescribeDtsJobs](~~209702~~) operation to query the instance ID.
+        # The ID of the change tracking instance. You can call the [DescribeDtsJobs](https://help.aliyun.com/document_detail/209702.html) operation to query the instance ID.
         # 
         # >  You must specify at least one of the **DtsInstanceId** and **DtsJobId** parameters.
         self.dts_instance_id = dts_instance_id
-        # The ID of the change tracking task. You can call the [DescribeDtsJobs](~~209702~~) operation to query the task ID.
+        # The ID of the change tracking task. You can call the [DescribeDtsJobs](https://help.aliyun.com/document_detail/209702.html) operation to query the task ID.
         # 
         # >  You must specify at least one of the **DtsInstanceId** and **DtsJobId** parameters.
         self.dts_job_id = dts_job_id
-        # The ID of the region where the change tracking instance resides. For more information, see [List of supported regions](~~141033~~).
+        # The ID of the region where the change tracking instance resides. For more information, see [List of supported regions](https://help.aliyun.com/document_detail/141033.html).
+        # 
+        # This parameter is required.
         self.region_id = region_id
         self.resource_group_id = resource_group_id
 
     def validate(self):
         pass
 
     def to_map(self):
@@ -34463,31 +34685,39 @@
         subscription_instance_id: str = None,
         consumer_group_new_password: str = None,
     ):
         # The ID of the Alibaba Cloud account. You do not need to specify this parameter because this parameter will be removed in the future.
         self.account_id = account_id
         # The ID of the consumer group.
         # 
-        # You can call the [DescribeConsumerGroup](~~122886~~) operation to query the consumer group ID.
+        # You can call the [DescribeConsumerGroup](https://help.aliyun.com/document_detail/122886.html) operation to query the consumer group ID.
+        # 
+        # This parameter is required.
         self.consumer_group_id = consumer_group_id
-        # The name of the consumer group. You can call the [DescribeConsumerGroup](~~122886~~) operation to query the consumer group name.
+        # The name of the consumer group. You can call the [DescribeConsumerGroup](https://help.aliyun.com/document_detail/122886.html) operation to query the consumer group name.
         self.consumer_group_name = consumer_group_name
         # The current password of the consumer group.
+        # 
+        # This parameter is required.
         self.consumer_group_password = consumer_group_password
-        # The username of the consumer group. You can call the [DescribeConsumerGroup](~~122886~~) operation to query the username.
+        # The username of the consumer group. You can call the [DescribeConsumerGroup](https://help.aliyun.com/document_detail/122886.html) operation to query the username.
         self.consumer_group_user_name = consumer_group_user_name
         self.owner_id = owner_id
         self.region_id = region_id
         self.resource_group_id = resource_group_id
         # The ID of the change tracking instance. You can call the DescribeSubscriptionInstances operation to query the instance ID.
+        # 
+        # This parameter is required.
         self.subscription_instance_id = subscription_instance_id
         # The new password of the consumer group.
         # 
         # *   A password must contain two or more of the following characters: uppercase letters, lowercase letters, digits, and special characters.
         # *   A password must be 8 to 32 characters in length.
+        # 
+        # This parameter is required.
         self.consumer_group_new_password = consumer_group_new_password
 
     def validate(self):
         pass
 
     def to_map(self):
         _map = super().to_map()
@@ -34641,19 +34871,23 @@
         region_id: str = None,
         resource_group_id: str = None,
         subscription_instance_id: str = None,
     ):
         # The ID of the Alibaba Cloud account. You do not need to specify this parameter because this parameter will be removed in the future.
         self.account_id = account_id
         # The consumption checkpoint. The format is *yyyy-MM-dd*T*HH:mm:ss*Z. The time is displayed in UTC.
+        # 
+        # This parameter is required.
         self.consumption_timestamp = consumption_timestamp
         self.owner_id = owner_id
         self.region_id = region_id
         self.resource_group_id = resource_group_id
         # The ID of the change tracking instance. You can call the **DescribeSubscriptionInstances** operation to query the instance ID.
+        # 
+        # This parameter is required.
         self.subscription_instance_id = subscription_instance_id
 
     def validate(self):
         pass
 
     def to_map(self):
         _map = super().to_map()
@@ -34986,37 +35220,39 @@
         # *   **false**\
         self.data_initialization = data_initialization
         # Specifies whether to perform incremental data migration or synchronization. Valid values:
         # 
         # *   **false**\
         # *   **true**\
         self.data_synchronization = data_synchronization
-        # The objects of the data synchronization task after modification. The value must be a JSON string. For more information, see [Objects of DTS tasks](~~209545~~).
+        # The objects of the data synchronization task after modification. The value must be a JSON string. For more information, see [Objects of DTS tasks](https://help.aliyun.com/document_detail/209545.html).
         # 
         # > 
         # 
         # *   The new value of DbList overwrites the original value. Make sure that all the objects that you want to synchronize are specified. Otherwise, some objects may be lost. Specify this parameter with caution.
         # 
-        # *   Before you call the ModifyDtsJob operation, we recommend that you call the [DescribeDtsJobDetail](~~208925~~) operation to query the current objects of the data synchronization task. Then, you can specify the new objects based on your business requirements. For example, if the current objects are Table A and Table B and you need to add Table C, you must specify Table A, Table B, and Table C for this parameter.
+        # *   Before you call the ModifyDtsJob operation, we recommend that you call the [DescribeDtsJobDetail](https://help.aliyun.com/document_detail/208925.html) operation to query the current objects of the data synchronization task. Then, you can specify the new objects based on your business requirements. For example, if the current objects are Table A and Table B and you need to add Table C, you must specify Table A, Table B, and Table C for this parameter.
         self.db_list = db_list
         # The ID of the data synchronization instance.
+        # 
+        # This parameter is required.
         self.dts_instance_id = dts_instance_id
-        # The synchronization task ID. You can call the [DescribeDtsJobs](~~209702~~) operation to query the task ID.
+        # The synchronization task ID. You can call the [DescribeDtsJobs](https://help.aliyun.com/document_detail/209702.html) operation to query the task ID.
         self.dts_job_id = dts_job_id
         # The operator that is related to the extract, transform, and load (ETL) feature and dedicated to T+1 business.
         self.etl_operator_column_reference = etl_operator_column_reference
         # The endpoint of the Object Storage Service (OSS) bucket in which the files to be synchronized are stored.
         self.file_oss_url = file_oss_url
         # The name of the table to be filtered.
         self.filter_table_name = filter_table_name
         # The method that is used to modify the data synchronization task. If you do not specify the parameter, the objects of the data synchronization task are modified by default. If you specify UPDATE_RESERVED for the parameter, the reserved parameters are modified.
         self.modify_type_enum = modify_type_enum
-        # The ID of the region in which the data synchronization instance resides. For more information, see [List of supported regions](~~141033~~).
+        # The ID of the region in which the data synchronization instance resides. For more information, see [List of supported regions](https://help.aliyun.com/document_detail/141033.html).
         self.region_id = region_id
-        # The reserved parameters of the data synchronization task. You can add reserved parameters instead of overwriting the existing reserved parameters. The value of the parameter is a MAP JSON string. You can specify this parameter to meet special requirements, such as specifying whether to automatically start the precheck of the data synchronization task. For more information, see [MigrationReserved](~~176470~~).
+        # The reserved parameters of the data synchronization task. You can add reserved parameters instead of overwriting the existing reserved parameters. The value of the parameter is a MAP JSON string. You can specify this parameter to meet special requirements, such as specifying whether to automatically start the precheck of the data synchronization task. For more information, see [MigrationReserved](https://help.aliyun.com/document_detail/176470.html).
         self.reserved = reserved
         self.resource_group_id = resource_group_id
         # Specifies whether to perform schema migration or synchronization. Valid values:
         # 
         # *   **true**\
         # *   **false**\
         self.structure_initialization = structure_initialization
@@ -35139,37 +35375,39 @@
         # *   **false**\
         self.data_initialization = data_initialization
         # Specifies whether to perform incremental data migration or synchronization. Valid values:
         # 
         # *   **false**\
         # *   **true**\
         self.data_synchronization = data_synchronization
-        # The objects of the data synchronization task after modification. The value must be a JSON string. For more information, see [Objects of DTS tasks](~~209545~~).
+        # The objects of the data synchronization task after modification. The value must be a JSON string. For more information, see [Objects of DTS tasks](https://help.aliyun.com/document_detail/209545.html).
         # 
         # > 
         # 
         # *   The new value of DbList overwrites the original value. Make sure that all the objects that you want to synchronize are specified. Otherwise, some objects may be lost. Specify this parameter with caution.
         # 
-        # *   Before you call the ModifyDtsJob operation, we recommend that you call the [DescribeDtsJobDetail](~~208925~~) operation to query the current objects of the data synchronization task. Then, you can specify the new objects based on your business requirements. For example, if the current objects are Table A and Table B and you need to add Table C, you must specify Table A, Table B, and Table C for this parameter.
+        # *   Before you call the ModifyDtsJob operation, we recommend that you call the [DescribeDtsJobDetail](https://help.aliyun.com/document_detail/208925.html) operation to query the current objects of the data synchronization task. Then, you can specify the new objects based on your business requirements. For example, if the current objects are Table A and Table B and you need to add Table C, you must specify Table A, Table B, and Table C for this parameter.
         self.db_list = db_list
         # The ID of the data synchronization instance.
+        # 
+        # This parameter is required.
         self.dts_instance_id = dts_instance_id
-        # The synchronization task ID. You can call the [DescribeDtsJobs](~~209702~~) operation to query the task ID.
+        # The synchronization task ID. You can call the [DescribeDtsJobs](https://help.aliyun.com/document_detail/209702.html) operation to query the task ID.
         self.dts_job_id = dts_job_id
         # The operator that is related to the extract, transform, and load (ETL) feature and dedicated to T+1 business.
         self.etl_operator_column_reference = etl_operator_column_reference
         # The endpoint of the Object Storage Service (OSS) bucket in which the files to be synchronized are stored.
         self.file_oss_url_object = file_oss_url_object
         # The name of the table to be filtered.
         self.filter_table_name = filter_table_name
         # The method that is used to modify the data synchronization task. If you do not specify the parameter, the objects of the data synchronization task are modified by default. If you specify UPDATE_RESERVED for the parameter, the reserved parameters are modified.
         self.modify_type_enum = modify_type_enum
-        # The ID of the region in which the data synchronization instance resides. For more information, see [List of supported regions](~~141033~~).
+        # The ID of the region in which the data synchronization instance resides. For more information, see [List of supported regions](https://help.aliyun.com/document_detail/141033.html).
         self.region_id = region_id
-        # The reserved parameters of the data synchronization task. You can add reserved parameters instead of overwriting the existing reserved parameters. The value of the parameter is a MAP JSON string. You can specify this parameter to meet special requirements, such as specifying whether to automatically start the precheck of the data synchronization task. For more information, see [MigrationReserved](~~176470~~).
+        # The reserved parameters of the data synchronization task. You can add reserved parameters instead of overwriting the existing reserved parameters. The value of the parameter is a MAP JSON string. You can specify this parameter to meet special requirements, such as specifying whether to automatically start the precheck of the data synchronization task. For more information, see [MigrationReserved](https://help.aliyun.com/document_detail/176470.html).
         self.reserved = reserved
         self.resource_group_id = resource_group_id
         # Specifies whether to perform schema migration or synchronization. Valid values:
         # 
         # *   **true**\
         # *   **false**\
         self.structure_initialization = structure_initialization
@@ -35292,37 +35530,39 @@
         # *   **false**\
         self.data_initialization = data_initialization
         # Specifies whether to perform incremental data migration or synchronization. Valid values:
         # 
         # *   **false**\
         # *   **true**\
         self.data_synchronization = data_synchronization
-        # The objects of the data synchronization task after modification. The value must be a JSON string. For more information, see [Objects of DTS tasks](~~209545~~).
+        # The objects of the data synchronization task after modification. The value must be a JSON string. For more information, see [Objects of DTS tasks](https://help.aliyun.com/document_detail/209545.html).
         # 
         # > 
         # 
         # *   The new value of DbList overwrites the original value. Make sure that all the objects that you want to synchronize are specified. Otherwise, some objects may be lost. Specify this parameter with caution.
         # 
-        # *   Before you call the ModifyDtsJob operation, we recommend that you call the [DescribeDtsJobDetail](~~208925~~) operation to query the current objects of the data synchronization task. Then, you can specify the new objects based on your business requirements. For example, if the current objects are Table A and Table B and you need to add Table C, you must specify Table A, Table B, and Table C for this parameter.
+        # *   Before you call the ModifyDtsJob operation, we recommend that you call the [DescribeDtsJobDetail](https://help.aliyun.com/document_detail/208925.html) operation to query the current objects of the data synchronization task. Then, you can specify the new objects based on your business requirements. For example, if the current objects are Table A and Table B and you need to add Table C, you must specify Table A, Table B, and Table C for this parameter.
         self.db_list_shrink = db_list_shrink
         # The ID of the data synchronization instance.
+        # 
+        # This parameter is required.
         self.dts_instance_id = dts_instance_id
-        # The synchronization task ID. You can call the [DescribeDtsJobs](~~209702~~) operation to query the task ID.
+        # The synchronization task ID. You can call the [DescribeDtsJobs](https://help.aliyun.com/document_detail/209702.html) operation to query the task ID.
         self.dts_job_id = dts_job_id
         # The operator that is related to the extract, transform, and load (ETL) feature and dedicated to T+1 business.
         self.etl_operator_column_reference = etl_operator_column_reference
         # The endpoint of the Object Storage Service (OSS) bucket in which the files to be synchronized are stored.
         self.file_oss_url = file_oss_url
         # The name of the table to be filtered.
         self.filter_table_name = filter_table_name
         # The method that is used to modify the data synchronization task. If you do not specify the parameter, the objects of the data synchronization task are modified by default. If you specify UPDATE_RESERVED for the parameter, the reserved parameters are modified.
         self.modify_type_enum = modify_type_enum
-        # The ID of the region in which the data synchronization instance resides. For more information, see [List of supported regions](~~141033~~).
+        # The ID of the region in which the data synchronization instance resides. For more information, see [List of supported regions](https://help.aliyun.com/document_detail/141033.html).
         self.region_id = region_id
-        # The reserved parameters of the data synchronization task. You can add reserved parameters instead of overwriting the existing reserved parameters. The value of the parameter is a MAP JSON string. You can specify this parameter to meet special requirements, such as specifying whether to automatically start the precheck of the data synchronization task. For more information, see [MigrationReserved](~~176470~~).
+        # The reserved parameters of the data synchronization task. You can add reserved parameters instead of overwriting the existing reserved parameters. The value of the parameter is a MAP JSON string. You can specify this parameter to meet special requirements, such as specifying whether to automatically start the precheck of the data synchronization task. For more information, see [MigrationReserved](https://help.aliyun.com/document_detail/176470.html).
         self.reserved = reserved
         self.resource_group_id = resource_group_id
         # Specifies whether to perform schema migration or synchronization. Valid values:
         # 
         # *   **true**\
         # *   **false**\
         self.structure_initialization = structure_initialization
@@ -35803,18 +36043,22 @@
         dts_job_id: str = None,
         du_limit: int = None,
         owner_id: str = None,
         region_id: str = None,
         resource_group_id: str = None,
     ):
         # The ID of the data migration, data synchronization, or change tracking task.
+        # 
+        # This parameter is required.
         self.dts_job_id = dts_job_id
         # The upper limit of DUs for the DTS task.
         # 
         # >  Minimum value: **1**.
+        # 
+        # This parameter is required.
         self.du_limit = du_limit
         self.owner_id = owner_id
         # The ID of the region in which the DTS instance resides.
         self.region_id = region_id
         self.resource_group_id = resource_group_id
 
     def validate(self):
@@ -35989,16 +36233,18 @@
         username: str = None,
     ):
         self.aliyun_uid = aliyun_uid
         self.database = database
         self.dry_run = dry_run
         self.dts_instance_id = dts_instance_id
         self.dts_job_id = dts_job_id
+        # This parameter is required.
         self.endpoint = endpoint
         self.endpoint_instance_id = endpoint_instance_id
+        # This parameter is required.
         self.endpoint_instance_type = endpoint_instance_type
         self.endpoint_ip = endpoint_ip
         self.endpoint_port = endpoint_port
         self.endpoint_region_id = endpoint_region_id
         self.modify_account = modify_account
         self.password = password
         self.region_id = region_id
@@ -36203,20 +36449,24 @@
         dts_job_id: str = None,
         dts_job_name: str = None,
         region_id: str = None,
         resource_group_id: str = None,
         zero_etl_job: bool = None,
     ):
         # The ID of the data migration, data synchronization, or change tracking task.
+        # 
+        # This parameter is required.
         self.dts_job_id = dts_job_id
         # The new name of the DTS task.
         # 
         # >  We recommend that you specify a descriptive name for easy identification. You do not need to use a unique name.
+        # 
+        # This parameter is required.
         self.dts_job_name = dts_job_name
-        # The ID of the region in which the DTS instance resides. For more information, see [List of supported regions](~~141033~~).
+        # The ID of the region in which the DTS instance resides. For more information, see [List of supported regions](https://help.aliyun.com/document_detail/141033.html).
         self.region_id = region_id
         self.resource_group_id = resource_group_id
         self.zero_etl_job = zero_etl_job
 
     def validate(self):
         pass
 
@@ -36374,27 +36624,29 @@
         password: str = None,
         region_id: str = None,
         resource_group_id: str = None,
         user_name: str = None,
         zero_etl_job: bool = None,
     ):
         # The ID of the data migration, data synchronization, or change tracking task.
+        # 
+        # This parameter is required.
         self.dts_job_id = dts_job_id
         # Specifies the database to which the password belongs. Valid values:
         # 
         # *   **src**: source database
         # *   **dest**: destination database
         # 
         # >  This parameter must be specified.
         self.endpoint = endpoint
         # The new password of the account.
         # 
         # >  This parameter must be specified and cannot be the same as the current password.
         self.password = password
-        # The ID of the region where the DTS instance resides. For more information, see [List of supported regions](~~141033~~).
+        # The ID of the region where the DTS instance resides. For more information, see [List of supported regions](https://help.aliyun.com/document_detail/141033.html).
         self.region_id = region_id
         self.resource_group_id = resource_group_id
         # The account of the source or destination database.
         # 
         # >  This parameter must be specified.
         self.user_name = user_name
         self.zero_etl_job = zero_etl_job
@@ -36563,16 +36815,18 @@
         dts_job_id: str = None,
         enable_limit: bool = None,
         job_code: str = None,
         region_id: str = None,
         resource_group_id: str = None,
     ):
         self.config_list = config_list
+        # This parameter is required.
         self.dts_job_id = dts_job_id
         self.enable_limit = enable_limit
+        # This parameter is required.
         self.job_code = job_code
         self.region_id = region_id
         self.resource_group_id = resource_group_id
 
     def validate(self):
         pass
 
@@ -36724,34 +36978,40 @@
         dts_instance_id: str = None,
         dts_job_id: str = None,
         region_id: str = None,
         resource_group_id: str = None,
         subscription_data_type_ddl: bool = None,
         subscription_data_type_dml: bool = None,
     ):
-        # The objects of the change tracking task. The value is a JSON string. For more information, see [Objects of DTS tasks](~~209545~~).
+        # The objects of the change tracking task. The value is a JSON string. For more information, see [Objects of DTS tasks](https://help.aliyun.com/document_detail/209545.html).
         # 
-        # >  You can call the [DescribeDtsJobDetail](~~208925~~) operation to query the original objects of the task.
+        # >  You can call the [DescribeDtsJobDetail](https://help.aliyun.com/document_detail/208925.html) operation to query the original objects of the task.
+        # 
+        # This parameter is required.
         self.db_list = db_list
-        # The ID of the change tracking instance. You can call the [DescribeDtsJobs](~~209702~~) operation to query the instance ID.
+        # The ID of the change tracking instance. You can call the [DescribeDtsJobs](https://help.aliyun.com/document_detail/209702.html) operation to query the instance ID.
         self.dts_instance_id = dts_instance_id
-        # The ID of the change tracking task. You can call the [DescribeDtsJobs](~~209702~~) operation to query the task ID.
+        # The ID of the change tracking task. You can call the [DescribeDtsJobs](https://help.aliyun.com/document_detail/209702.html) operation to query the task ID.
         self.dts_job_id = dts_job_id
-        # The ID of the region where the change tracking instance resides. For more information, see [List of supported regions](~~141033~~).
+        # The ID of the region where the change tracking instance resides. For more information, see [List of supported regions](https://help.aliyun.com/document_detail/141033.html).
         self.region_id = region_id
         self.resource_group_id = resource_group_id
         # Specifies whether to retrieve data definition language (DDL) statements. Valid values:
         # 
         # *   **true**: yes
         # *   **false**: no
+        # 
+        # This parameter is required.
         self.subscription_data_type_ddl = subscription_data_type_ddl
         # Specifies whether to retrieve data manipulation language (DML) statements. Valid values:
         # 
         # *   **true**: yes
         # *   **false**: no
+        # 
+        # This parameter is required.
         self.subscription_data_type_dml = subscription_data_type_dml
 
     def validate(self):
         pass
 
     def to_map(self):
         _map = super().to_map()
@@ -36902,17 +37162,21 @@
         subscription_object: str = None,
     ):
         # The ID of the Alibaba Cloud account. You do not need to specify this parameter because this parameter will be removed in the future.
         self.account_id = account_id
         self.owner_id = owner_id
         self.region_id = region_id
         self.resource_group_id = resource_group_id
-        # The ID of the change tracking instance. You can call the [DescribeSubscriptionInstances](~~49442~~) operation to query the instance ID.
+        # The ID of the change tracking instance. You can call the [DescribeSubscriptionInstances](https://help.aliyun.com/document_detail/49442.html) operation to query the instance ID.
+        # 
+        # This parameter is required.
         self.subscription_instance_id = subscription_instance_id
-        # The objects from which you want to track data changes. The value is a JSON string and can contain regular expressions. For more information, see [SubscriptionObjects](~~141902~~).
+        # The objects from which you want to track data changes. The value is a JSON string and can contain regular expressions. For more information, see [SubscriptionObjects](https://help.aliyun.com/document_detail/141902.html).
+        # 
+        # This parameter is required.
         self.subscription_object = subscription_object
 
     def validate(self):
         pass
 
     def to_map(self):
         _map = super().to_map()
@@ -37063,15 +37327,18 @@
         # *   **Reverse**\
         # 
         # > 
         # *   Default value: **Forward**.
         # *   This parameter is required only when the topology of the data synchronization instance is two-way synchronization.
         self.synchronization_direction = synchronization_direction
         # The ID of the data synchronization instance. You can call the DescribeSynchronizationJobs operation to query the instance ID.
+        # 
+        # This parameter is required.
         self.synchronization_job_id = synchronization_job_id
+        # This parameter is required.
         self.synchronization_objects = synchronization_objects
 
     def validate(self):
         pass
 
     def to_map(self):
         _map = super().to_map()
@@ -37223,23 +37490,27 @@
     ):
         # The subscription duration of the DTS instance after renewal. Default value: 1.
         # 
         # *   If the **Period** parameter is set to **Year**, the valid values are **1 to 5**.
         # *   If the **Period** parameter is set to **Month**, the valid values are **1 to 60**.
         self.buy_count = buy_count
         # The billing method of the DTS instance. Set the value to **PREPAY**, which indicates the subscription billing method.
+        # 
+        # This parameter is required.
         self.charge_type = charge_type
-        # The ID of the data synchronization or change tracking task. You can call the [DescribeDtsJobs](~~209702~~) operation to query the task ID.
+        # The ID of the data synchronization or change tracking task. You can call the [DescribeDtsJobs](https://help.aliyun.com/document_detail/209702.html) operation to query the task ID.
+        # 
+        # This parameter is required.
         self.dts_job_id = dts_job_id
         # The billing cycle of the DTS instance after renewal. Valid values:
         # 
         # *   **Year**: annual subscription.
         # *   **Month**: monthly subscription. This is the default value.
         self.period = period
-        # The region ID of the DTS instance. For more information, see [List of supported regions](~~141033~~).
+        # The region ID of the DTS instance. For more information, see [List of supported regions](https://help.aliyun.com/document_detail/141033.html).
         self.region_id = region_id
         self.resource_group_id = resource_group_id
 
     def validate(self):
         pass
 
     def to_map(self):
@@ -37622,14 +37893,16 @@
         # *   **Reverse**\
         # 
         # > 
         # *   Default value: **Forward**.
         # *   You can set this parameter to **Reverse** to stop reverse synchronization only when the topology is two-way synchronization.
         self.synchronization_direction = synchronization_direction
         # The ID of the data synchronization instance. You can call the **DescribeSynchronizationJobs** operation to query the instance ID.
+        # 
+        # This parameter is required.
         self.synchronization_job_id = synchronization_job_id
 
     def validate(self):
         pass
 
     def to_map(self):
         _map = super().to_map()
@@ -37764,14 +38037,15 @@
         dts_instance_id: str = None,
         ignore_error_sub_job: bool = None,
         region_id: str = None,
         resource_group_id: str = None,
     ):
         self.dts_instance_id = dts_instance_id
         self.ignore_error_sub_job = ignore_error_sub_job
+        # This parameter is required.
         self.region_id = region_id
         self.resource_group_id = resource_group_id
 
     def validate(self):
         pass
 
     def to_map(self):
@@ -37912,28 +38186,32 @@
         self,
         dts_instance_id: str = None,
         precheck_items: str = None,
         region_id: str = None,
         resource_group_id: str = None,
     ):
         # The ID of the data migration or data synchronization instance. You can call the **DescribeMigrationJobs** or DescribeSynchronizationJobs operation to query the instance ID.
+        # 
+        # This parameter is required.
         self.dts_instance_id = dts_instance_id
         # The precheck items that you want to ignore. Separate multiple items with commas (,). Valid values:
         # 
         # *   **CHECK_SAME_OBJ**: schema name conflict
         # 
         # *   **CHECK_SAME_USER**: multiple usernames for one instance
         # 
         # *   **CHECK_SRC**: source database version
         # 
         # *   **CHECK_TOPOLOGY**: topology
         # 
-        # > For more information about the topologies supported by DTS, see [Synchronization topologies](~~124115~~).
+        # > For more information about the topologies supported by DTS, see [Synchronization topologies](https://help.aliyun.com/document_detail/124115.html).
         # 
         # *   **CHECK_SERVER_ID**: value of server_id in the source database
+        # 
+        # This parameter is required.
         self.precheck_items = precheck_items
         self.region_id = region_id
         self.resource_group_id = resource_group_id
 
     def validate(self):
         pass
 
@@ -38064,38 +38342,42 @@
         region_id: str = None,
         resource_group_id: str = None,
         skip: bool = None,
         skip_pre_check_items: str = None,
         skip_pre_check_names: str = None,
     ):
         # The ID of the data migration, data synchronization, or change tracking task.
+        # 
+        # This parameter is required.
         self.dts_job_id = dts_job_id
         # The ID of the precheck task. You can call the **DescribePreCheckStatus** operation to query the task ID.
         self.job_id = job_id
-        # The region ID of the DTS instance. For more information, see [List of supported regions](~~141033~~).
+        # The region ID of the DTS instance. For more information, see [List of supported regions](https://help.aliyun.com/document_detail/141033.html).
         self.region_id = region_id
         self.resource_group_id = resource_group_id
         # Specifies whether to skip the precheck item. Valid values:
         # 
         # *   **true**: skips the precheck item.
         # *   **false**: does not skip the precheck item.
         # 
         # >  This parameter is required.
+        # 
+        # This parameter is required.
         self.skip = skip
         # The shortened name of the precheck item. Valid values:
         # 
         # *   **CHECK_SAME_OBJ**: object name conflict
         # 
         # *   **CHECK_SAME_USER**: multiple usernames for one instance
         # 
         # *   **CHECK_SRC**: source database version
         # 
         # *   **CHECK_TOPOLOGY**: topology type
         # 
-        # > For more information about the topologies supported by DTS, see [Synchronization topologies](~~124115~~).
+        # > For more information about the topologies supported by DTS, see [Synchronization topologies](https://help.aliyun.com/document_detail/124115.html).
         # 
         # *   **CHECK_SERVER_ID**: the server ID of the source database
         # 
         # >  Separate multiple shortened names with commas (,).
         self.skip_pre_check_items = skip_pre_check_items
         # The name of the precheck item. This parameter corresponds to the **SkipPreCheckItems** parameter. Valid values:
         # 
@@ -38103,15 +38385,15 @@
         # 
         # *   **CHECK_SAME_USER_DETAIL**: multiple usernames for one instance
         # 
         # *   **CHECK_SRC_DETAIL**: source database version
         # 
         # *   **CHECK_TOPOLOGY_DETAIL**: topology type
         # 
-        # > For more information about the topologies supported by DTS, see [Synchronization topologies](~~124115~~).
+        # > For more information about the topologies supported by DTS, see [Synchronization topologies](https://help.aliyun.com/document_detail/124115.html).
         # 
         # *   **CHECK_SERVER_ID_DETAIL**: the server ID of the source database
         # 
         # >  Separate multiple item names with commas (,).
         self.skip_pre_check_names = skip_pre_check_names
 
     def validate(self):
@@ -38307,19 +38589,19 @@
         region_id: str = None,
         resource_group_id: str = None,
         synchronization_direction: str = None,
         zero_etl_job: bool = None,
     ):
         # The ID of the data migration, data synchronization, or change tracking instance.
         # 
-        # >  You can call the [DescribeMigrationJobs](~~208139~~), [DescribeSubscriptionInstances](~~49442~~), or [DescribeSynchronizationJobs](~~49454~~) operation to query the instance ID
+        # >  You can call the [DescribeMigrationJobs](https://help.aliyun.com/document_detail/208139.html), [DescribeSubscriptionInstances](https://help.aliyun.com/document_detail/49442.html), or [DescribeSynchronizationJobs](https://help.aliyun.com/document_detail/49454.html) operation to query the instance ID
         self.dts_instance_id = dts_instance_id
         # The ID of the data migration, data synchronization, or change tracking task.
         self.dts_job_id = dts_job_id
-        # The region ID of the Data Transmission Service (DTS) instance. For more information, see [List of supported regions](~~141033~~).
+        # The region ID of the Data Transmission Service (DTS) instance. For more information, see [List of supported regions](https://help.aliyun.com/document_detail/141033.html).
         self.region_id = region_id
         self.resource_group_id = resource_group_id
         # The synchronization direction. Default value: Forward. Valid values:
         # 
         # *   **Forward**: Data is synchronized from the source database to the destination database.
         # 
         # *   **Reverse**: Data is synchronized from the destination database to the source database.
@@ -38489,17 +38771,19 @@
         resource_group_id: str = None,
         zero_etl_job: bool = None,
     ):
         # The ID of the data migration or data synchronization task.
         # 
         # > 
         # *   For multiple tasks, separate them with commas (**,**).
-        # *   You can call the [DescribeDtsJobs](~~209702~~) operation to query the task ID.
+        # *   You can call the [DescribeDtsJobs](https://help.aliyun.com/document_detail/209702.html) operation to query the task ID.
+        # 
+        # This parameter is required.
         self.dts_job_ids = dts_job_ids
-        # The region ID of the DTS instance. For more information, see [List of supported regions](~~141033~~).
+        # The region ID of the DTS instance. For more information, see [List of supported regions](https://help.aliyun.com/document_detail/141033.html).
         self.region_id = region_id
         self.resource_group_id = resource_group_id
         self.zero_etl_job = zero_etl_job
 
     def validate(self):
         pass
 
@@ -38653,14 +38937,16 @@
         owner_id: str = None,
         region_id: str = None,
         resource_group_id: str = None,
     ):
         # The ID of the Alibaba Cloud account. You do not need to specify this parameter because this parameter will be removed in the future.
         self.account_id = account_id
         # The ID of the data migration instance. You can call the **DescribeMigrationJobs** operation to query all data migration instances.
+        # 
+        # This parameter is required.
         self.migration_job_id = migration_job_id
         self.owner_id = owner_id
         self.region_id = region_id
         self.resource_group_id = resource_group_id
 
     def validate(self):
         pass
@@ -38796,14 +39082,16 @@
         resource_group_id: str = None,
     ):
         # The offset of the Incremental Write module. Specify a UNIX timestamp representing the number of milliseconds that have elapsed since January 1, 1970, 00:00:00 UTC. 
         # 
         # > The default value is the offset that is automatically saved by DTS when the task is paused.
         self.check_point = check_point
         # The ID of the reverse task that was created by calling the CreateReverseDtsJob operation.
+        # 
+        # This parameter is required.
         self.dts_job_id = dts_job_id
         self.resource_group_id = resource_group_id
 
     def validate(self):
         pass
 
     def to_map(self):
@@ -38932,14 +39220,16 @@
     ):
         # The ID of the Alibaba Cloud account. You do not need to specify this parameter because this parameter will be removed in the future.
         self.account_id = account_id
         self.owner_id = owner_id
         self.region_id = region_id
         self.resource_group_id = resource_group_id
         # The ID of the change tracking instance. You can call the DescribeSubscriptionInstances operation to query the instance ID.
+        # 
+        # This parameter is required.
         self.subscription_instance_id = subscription_instance_id
 
     def validate(self):
         pass
 
     def to_map(self):
         _map = super().to_map()
@@ -39092,14 +39382,16 @@
         # *   **Reverse**\
         # 
         # > 
         # *   Default value: **Forward**.
         # *   You can set this parameter to **Reverse** to start the reverse synchronization task only when the topology is two-way synchronization.
         self.synchronization_direction = synchronization_direction
         # The ID of the data synchronization instance. You can call the **DescribeSynchronizationJobs** operation to query the instance ID.
+        # 
+        # This parameter is required.
         self.synchronization_job_id = synchronization_job_id
 
     def validate(self):
         pass
 
     def to_map(self):
         _map = super().to_map()
@@ -39578,17 +39870,19 @@
         resource_group_id: str = None,
         zero_etl_job: bool = None,
     ):
         # The ID of the data migration or data synchronization task.
         # 
         # > 
         # *   Separate multiple task IDs by **,** (commas).
-        # *   You can call the [DescribeDtsJobs](~~209702~~) operation to query task IDs.
+        # *   You can call the [DescribeDtsJobs](https://help.aliyun.com/document_detail/209702.html) operation to query task IDs.
+        # 
+        # This parameter is required.
         self.dts_job_ids = dts_job_ids
-        # The region ID of the DTS instance. For more information, see [List of supported regions](~~141033~~).
+        # The region ID of the DTS instance. For more information, see [List of supported regions](https://help.aliyun.com/document_detail/141033.html).
         self.region_id = region_id
         self.resource_group_id = resource_group_id
         self.zero_etl_job = zero_etl_job
 
     def validate(self):
         pass
 
@@ -39745,14 +40039,16 @@
         resource_group_id: str = None,
     ):
         # The ID of the Alibaba Cloud account. You do not need to specify this parameter because this parameter will be removed in the future.
         self.account_id = account_id
         # The client token that is used to ensure the idempotence of the request. You can use the client to generate the value, but you must ensure that it is unique among different requests. The **ClientToken** parameter can contain only ASCII characters and cannot exceed 64 characters in length.
         self.client_token = client_token
         # The ID of the data migration instance. You can call the **DescribeMigrationJobs** operation to query all data migration instances.
+        # 
+        # This parameter is required.
         self.migration_job_id = migration_job_id
         self.owner_id = owner_id
         self.region_id = region_id
         self.resource_group_id = resource_group_id
 
     def validate(self):
         pass
@@ -39899,21 +40195,25 @@
         # The ID of the data migration or data synchronization instance.
         # 
         # >  You must specify at least one of the DtsJobId and DtsInstanceId parameters.
         self.dts_instance_id = dts_instance_id
         # The ID of the data migration or data synchronization task.
         # 
         # >  You must specify at least one of the DtsJobId and DtsInstanceId parameters.
+        # 
+        # This parameter is required.
         self.dts_job_id = dts_job_id
         # The phase of the data migration task. Valid values:
         # 
         # *   **02**: The task is in the schema migration phase.
         # *   **03**: The task is in the incremental migration phase.
+        # 
+        # This parameter is required.
         self.job_code = job_code
-        # The region ID of the DTS instance. For more information, see [List of supported regions](~~141033~~).
+        # The region ID of the DTS instance. For more information, see [List of supported regions](https://help.aliyun.com/document_detail/141033.html).
         self.region_id = region_id
         self.resource_group_id = resource_group_id
         # The type of schema definition. Valid values:
         # 
         # *   **before**: schema migration or initial schema synchronization
         # *   **after**: DDL operations performed during incremental data migration or synchronization
         self.struct_type = struct_type
@@ -40039,15 +40339,15 @@
         self.code = code
         # The HTTP status code.
         self.http_status_code = http_status_code
         # The ID of the data migration or data synchronization task.
         self.job_id = job_id
         # The returned information about the migrated or synchronized objects in arrays.
         # 
-        # >  The arrays are in the following format: \[{"key":"Function","state":5,"totalCount":22},{"key":"Procedure","state":5,"totalCount":26},{"key":"Table","state":0,"totalCount":68},{"key":"View","state":5,"totalCount":100}].
+        # >  The arrays are in the following format: [{"key":"Function","state":5,"totalCount":22},{"key":"Procedure","state":5,"totalCount":26},{"key":"Table","state":0,"totalCount":68},{"key":"View","state":5,"totalCount":100}].
         self.progress_summary_details = progress_summary_details
         # The ID of the request.
         self.request_id = request_id
         # Indicates whether the request was successful. Valid values:
         # 
         # *   **true**: The request was successful.
         # *   **false**: The request failed.
@@ -40152,17 +40452,17 @@
         synchronization_direction: str = None,
         zero_etl_job: bool = None,
     ):
         # The ID of the data migration, data synchronization, or change tracking instance.
         self.dts_instance_id = dts_instance_id
         # The ID of the data migration, data synchronization, or change tracking task.
         # 
-        # >  You can call the [DescribeDtsJobs](~~209702~~) operation to obtain the task ID.
+        # >  You can call the [DescribeDtsJobs](https://help.aliyun.com/document_detail/209702.html) operation to obtain the task ID.
         self.dts_job_id = dts_job_id
-        # The ID of the region in which the DTS instance resides. For more information, see [List of supported regions](~~141033~~).
+        # The ID of the region in which the DTS instance resides. For more information, see [List of supported regions](https://help.aliyun.com/document_detail/141033.html).
         self.region_id = region_id
         self.resource_group_id = resource_group_id
         # The synchronization direction. Valid values:
         # 
         # *   **Forward**: Data is synchronized from the source database to the destination database.
         # *   **Reverse**: Data is synchronized from the destination database to the source database.
         # 
@@ -40333,17 +40633,19 @@
         resource_group_id: str = None,
         zero_etl_job: bool = None,
     ):
         # The ID of the data migration or data synchronization task.
         # 
         # > 
         # *   For multiple tasks, separate them with commas (,).
-        # *   You can call the [DescribeDtsJobs](~~209702~~) operation to query the task ID.
+        # *   You can call the [DescribeDtsJobs](https://help.aliyun.com/document_detail/209702.html) operation to query the task ID.
+        # 
+        # This parameter is required.
         self.dts_job_ids = dts_job_ids
-        # The ID of the region in which the DTS instance resides. For more information, see [List of supported regions](~~141033~~).
+        # The ID of the region in which the DTS instance resides. For more information, see [List of supported regions](https://help.aliyun.com/document_detail/141033.html).
         self.region_id = region_id
         self.resource_group_id = resource_group_id
         self.zero_etl_job = zero_etl_job
 
     def validate(self):
         pass
 
@@ -40500,14 +40802,16 @@
         resource_group_id: str = None,
     ):
         # The ID of the Alibaba Cloud account. You do not need to specify this parameter because this parameter will be removed in the future.
         self.account_id = account_id
         # The client token that is used to ensure the idempotence of the request. You can use the client to generate the value, but you must ensure that it is unique among different requests. The **ClientToken** parameter can contain only ASCII characters and cannot exceed 64 characters in length.
         self.client_token = client_token
         # The ID of the data migration instance. You can call the **DescribeMigrationJobs** operation to query all data migration instances.
+        # 
+        # This parameter is required.
         self.migration_job_id = migration_job_id
         self.owner_id = owner_id
         self.region_id = region_id
         self.resource_group_id = resource_group_id
 
     def validate(self):
         pass
@@ -40660,14 +40964,16 @@
         # *   **Reverse**\
         # 
         # > 
         # *   Default value: **Forward**.
         # *   You can set this parameter to **Reverse** to pause reverse synchronization only when the topology is two-way synchronization.
         self.synchronization_direction = synchronization_direction
         # The ID of the data synchronization instance. You can call the **DescribeSynchronizationJobs** operation to query the instance ID.
+        # 
+        # This parameter is required.
         self.synchronization_job_id = synchronization_job_id
 
     def validate(self):
         pass
 
     def to_map(self):
         _map = super().to_map()
@@ -40965,27 +41271,35 @@
         # >  You must specify the IP address only if the **Endpoint.InstanceType** parameter is set to **Express**.
         self.ip = ip
         # The ID of the ECS instance or the virtual private cloud (VPC).
         # 
         # > 
         # *   If the **Endpoint.InstanceType** parameter is set to **ECS**, you must specify the ID of the ECS instance.
         # *   If the **Endpoint.InstanceType** parameter is set to **Express**, you must specify the ID of the VPC.
+        # 
+        # This parameter is required.
         self.instance_id = instance_id
         # The instance type of the database. Valid values:
         # 
         # *   **LocalInstance**: self-managed database with a public IP address
         # *   **ECS**: self-managed database that is hosted on ECS
         # *   **Express**: self-managed database that is connected over Express Connect
+        # 
+        # This parameter is required.
         self.instance_type = instance_type
         # The service port number of the database.
+        # 
+        # This parameter is required.
         self.port = port
         # Specifies whether to update the connection settings of the source instance or the destination instance. Valid values:
         # 
         # *   **Source**\
         # *   **Destination**\
+        # 
+        # This parameter is required.
         self.type = type
 
     def validate(self):
         pass
 
     def to_map(self):
         _map = super().to_map()
@@ -41026,15 +41340,15 @@
         owner_id: str = None,
         role: str = None,
     ):
         # The ID of the Alibaba Cloud account to which the source instance belongs. You must specify this parameter only if the source instance and the destination instance belong to different Alibaba Cloud accounts.
         self.owner_id = owner_id
         # The authorized Resource Access Management (RAM) role of the source instance. You must specify the RAM role only if the source instance and the destination instance belong to different Alibaba Cloud accounts. You can use the RAM role to allow the Alibaba Cloud account that owns the destination instance to access the source instance.
         # 
-        # >  For information about the permissions and authorization methods of the RAM role, see [Configure RAM authorization for cross-account data migration and synchronization](~~48468~~).
+        # >  For information about the permissions and authorization methods of the RAM role, see [Configure RAM authorization for cross-account data migration and synchronization](https://help.aliyun.com/document_detail/48468.html).
         self.role = role
 
     def validate(self):
         pass
 
     def to_map(self):
         _map = super().to_map()
@@ -41082,14 +41396,16 @@
         # *   **Reverse**\
         # 
         # >  Default value: **Forward**.
         # 
         # The value **Reverse** takes effect only if the topology of the data synchronization instance is two-way synchronization.
         self.synchronization_direction = synchronization_direction
         # The ID of the data synchronization instance. You can call the DescribeSynchronizationJobs operation to query the instance ID.
+        # 
+        # This parameter is required.
         self.synchronization_job_id = synchronization_job_id
 
     def validate(self):
         if self.endpoint:
             self.endpoint.validate()
         if self.source_endpoint:
             self.source_endpoint.validate()
@@ -41154,15 +41470,15 @@
         self.err_code = err_code
         # The error message returned if the call failed.
         self.err_message = err_message
         # The ID of the request.
         self.request_id = request_id
         # Indicates whether the call was successful.
         self.success = success
-        # The task ID. You must specify the task ID when you call the [DescribeEndpointSwitchStatus](~~135598~~) operation to query the execution status of the task.
+        # The task ID. You must specify the task ID when you call the [DescribeEndpointSwitchStatus](https://help.aliyun.com/document_detail/135598.html) operation to query the execution status of the task.
         self.task_id = task_id
 
     def validate(self):
         pass
 
     def to_map(self):
         _map = super().to_map()
@@ -41245,20 +41561,24 @@
         value: str = None,
     ):
         # The tag key.
         # 
         # > 
         # *   N specifies the serial number of the tag. For example, Tag.1.Key specifies the key of the first tag and Tag.2.Key specifies the key of the second tag.
         # *   This parameter cannot be an empty string.
+        # 
+        # This parameter is required.
         self.key = key
         # The tag value.
         # 
         # > 
         # *   N specifies the serial number of the tag. For example, Tag.1.Value specifies the value of the first tag and Tag.2.Value specifies the value of the second tag.
         # *   This parameter can be an empty string.
+        # 
+        # This parameter is required.
         self.value = value
 
     def validate(self):
         pass
 
     def to_map(self):
         _map = super().to_map()
@@ -41286,20 +41606,24 @@
         self,
         region_id: str = None,
         resource_group_id: str = None,
         resource_id: List[str] = None,
         resource_type: str = None,
         tag: List[TagResourcesRequestTag] = None,
     ):
-        # The ID of the region where the data migration, data synchronization, or change tracking instance resides. For more information, see [List of supported regions](~~141033~~).
+        # The ID of the region where the data migration, data synchronization, or change tracking instance resides. For more information, see [List of supported regions](https://help.aliyun.com/document_detail/141033.html).
+        # 
+        # This parameter is required.
         self.region_id = region_id
         self.resource_group_id = resource_group_id
+        # This parameter is required.
         self.resource_id = resource_id
         # The resource type. Valid value: **ALIYUN::DTS::INSTANCE**.
         self.resource_type = resource_type
+        # This parameter is required.
         self.tag = tag
 
     def validate(self):
         if self.tag:
             for k in self.tag:
                 if k:
                     k.validate()
@@ -41437,29 +41761,35 @@
         self,
         dts_job_id: str = None,
         instance_class: str = None,
         order_type: str = None,
         region_id: str = None,
         resource_group_id: str = None,
     ):
-        # The ID of the data migration or data synchronization task. You can call the [DescribeDtsJobs](~~209702~~) operation to query the task ID.
+        # The ID of the data migration or data synchronization task. You can call the [DescribeDtsJobs](https://help.aliyun.com/document_detail/209702.html) operation to query the task ID.
+        # 
+        # This parameter is required.
         self.dts_job_id = dts_job_id
-        # The new instance class of the DTS instance. You can call the [DescribeDtsJobDetail](~~208925~~) operation to query the original instance class of the DTS instance.
+        # The new instance class of the DTS instance. You can call the [DescribeDtsJobDetail](https://help.aliyun.com/document_detail/208925.html) operation to query the original instance class of the DTS instance.
         # 
         # *   DTS supports the following instance classes for a data migration instance: **xxlarge**, **xlarge**, **large**, **medium**, and **small**.
         # *   DTS supports the following instance classes for a data synchronization instance: **large**, **medium**, **small**, and **micro**.
         # 
-        # >  For more information about the test performance of each instance class, see [Specifications of data migration instances](~~26606~~) and [Specifications of data synchronization instances](~~26605~~).
+        # >  For more information about the test performance of each instance class, see [Specifications of data migration instances](https://help.aliyun.com/document_detail/26606.html) and [Specifications of data synchronization instances](https://help.aliyun.com/document_detail/26605.html).
+        # 
+        # This parameter is required.
         self.instance_class = instance_class
         # Specifies whether to upgrade or downgrade the DTS instance. Valid values:
         # 
         # *   **UPGRADE**\
         # *   **DOWNGRADE**\
+        # 
+        # This parameter is required.
         self.order_type = order_type
-        # The ID of the region where the DTS instance resides. For more information, see [List of supported regions](~~141033~~).
+        # The ID of the region where the DTS instance resides. For more information, see [List of supported regions](https://help.aliyun.com/document_detail/141033.html).
         self.region_id = region_id
         self.resource_group_id = resource_group_id
 
     def validate(self):
         pass
 
     def to_map(self):
@@ -41643,23 +41973,25 @@
             self.body = temp_model.from_map(m['body'])
         return self
 
 
 class TransferPayTypeRequest(TeaModel):
     def __init__(
         self,
+        auto_pay: bool = None,
         buy_count: str = None,
         charge_type: str = None,
         dts_job_id: str = None,
         max_du: int = None,
         min_du: int = None,
         period: str = None,
         region_id: str = None,
         resource_group_id: str = None,
     ):
+        self.auto_pay = auto_pay
         # The subscription length.
         # 
         # *   If the **Period** parameter is set to **Year**, the value range is **1** to **5**.
         # *   If the **Period** parameter is set to **Month**, the value range is **1** to **60**.
         # 
         # >  You must specify this parameter only if you set the **ChargeType** parameter to **PrePaid**.
         self.buy_count = buy_count
@@ -41667,39 +41999,45 @@
         # 
         # *   **PrePaid**: subscription
         # *   **PostPaid**: pay-as-you-go
         # 
         # > 
         # *   The billing method of subscription instances cannot be changed to pay-as-you-go. To prevent resource waste, determine whether you need to change the billing method of your resources.
         # *   If you do not need to change the billing method, specify the current billing method.
+        # 
+        # This parameter is required.
         self.charge_type = charge_type
-        # The ID of the data synchronization or change tracking task. You can call the [DescribeDtsJobs](~~209702~~) operation to query the task ID.
+        # The ID of the data synchronization or change tracking task. You can call the [DescribeDtsJobs](https://help.aliyun.com/document_detail/209702.html) operation to query the task ID.
+        # 
+        # This parameter is required.
         self.dts_job_id = dts_job_id
         self.max_du = max_du
         self.min_du = min_du
         # The billing cycle of the subscription instance. Valid values:
         # 
         # *   **Year**\
         # *   **Month** (default value)
         # 
         # >  You must specify this parameter only if you set the **ChargeType** parameter to **PrePaid**.
         self.period = period
-        # The ID of the region where the DTS instance resides. For more information, see [List of supported regions](~~141033~~).
+        # The ID of the region where the DTS instance resides. For more information, see [List of supported regions](https://help.aliyun.com/document_detail/141033.html).
         self.region_id = region_id
         self.resource_group_id = resource_group_id
 
     def validate(self):
         pass
 
     def to_map(self):
         _map = super().to_map()
         if _map is not None:
             return _map
 
         result = dict()
+        if self.auto_pay is not None:
+            result['AutoPay'] = self.auto_pay
         if self.buy_count is not None:
             result['BuyCount'] = self.buy_count
         if self.charge_type is not None:
             result['ChargeType'] = self.charge_type
         if self.dts_job_id is not None:
             result['DtsJobId'] = self.dts_job_id
         if self.max_du is not None:
@@ -41712,14 +42050,16 @@
             result['RegionId'] = self.region_id
         if self.resource_group_id is not None:
             result['ResourceGroupId'] = self.resource_group_id
         return result
 
     def from_map(self, m: dict = None):
         m = m or dict()
+        if m.get('AutoPay') is not None:
+            self.auto_pay = m.get('AutoPay')
         if m.get('BuyCount') is not None:
             self.buy_count = m.get('BuyCount')
         if m.get('ChargeType') is not None:
             self.charge_type = m.get('ChargeType')
         if m.get('DtsJobId') is not None:
             self.dts_job_id = m.get('DtsJobId')
         if m.get('MaxDu') is not None:
@@ -41901,17 +42241,20 @@
         # *   **true**: unbinds all tags from the specified instances.
         # *   **false**: To unbind only specific tags, you must specify the **TagKey.N** parameter.
         # 
         # > 
         # *   You must specify at least one of the All and **TagKey.N** parameters.
         # *   If you specify both the All parameter and the **TagKey.N** parameter, the All parameter does not take effect.
         self.all = all
-        # The ID of the region where the data migration, data synchronization, or change tracking instance resides. For more information, see [List of supported regions](~~141033~~).
+        # The ID of the region where the data migration, data synchronization, or change tracking instance resides. For more information, see [List of supported regions](https://help.aliyun.com/document_detail/141033.html).
+        # 
+        # This parameter is required.
         self.region_id = region_id
         self.resource_group_id = resource_group_id
+        # This parameter is required.
         self.resource_id = resource_id
         # The resource type. Valid value: **ALIYUN::DTS::INSTANCE**.
         self.resource_type = resource_type
         self.tag_key = tag_key
 
     def validate(self):
         pass
@@ -42049,19 +42392,23 @@
         instance_class: str = None,
         instance_id: str = None,
         region_id: str = None,
         resource_group_id: str = None,
     ):
         # The instance class of the two-way synchronization task. Valid values: **large**, **medium**, **micro**, and **small**.
         # 
-        # >  For more information, see [Specifications of data synchronization instances](~~26605~~).
+        # >  For more information, see [Specifications of data synchronization instances](https://help.aliyun.com/document_detail/26605.html).
+        # 
+        # This parameter is required.
         self.instance_class = instance_class
-        # The ID of the data synchronization instance. You can call the [DescribeDtsJobs](~~209702~~) operation to query the instance ID.
+        # The ID of the data synchronization instance. You can call the [DescribeDtsJobs](https://help.aliyun.com/document_detail/209702.html) operation to query the instance ID.
+        # 
+        # This parameter is required.
         self.instance_id = instance_id
-        # The region ID of the DTS instance. For more information, see [List of supported regions](~~141033~~).
+        # The region ID of the DTS instance. For more information, see [List of supported regions](https://help.aliyun.com/document_detail/141033.html).
         self.region_id = region_id
         self.resource_group_id = resource_group_id
 
     def validate(self):
         pass
 
     def to_map(self):
@@ -42217,25 +42564,29 @@
         region_id: str = None,
         resource_group_id: str = None,
         type: str = None,
         zero_etl_job: bool = None,
     ):
         # The HTTP status code.
         self.destination_region = destination_region
-        # The ID of the region where the destination instance resides. For more information, see [List of supported regions](~~141033~~).
+        # The ID of the region where the destination instance resides. For more information, see [List of supported regions](https://help.aliyun.com/document_detail/141033.html).
         # 
         # > 
         # *   If the destination instance is a self-managed database with a public IP address or a third-party cloud database, you can set the parameter to **cn-hangzhou** or the ID of the closest region.
         # *   If the DTS task is a data migration or data synchronization task, you must specify this parameter.
+        # 
+        # This parameter is required.
         self.region = region
         self.region_id = region_id
         self.resource_group_id = resource_group_id
-        # The ID of the region where the source instance resides. For more information, see [List of supported regions](~~141033~~).
+        # The ID of the region where the source instance resides. For more information, see [List of supported regions](https://help.aliyun.com/document_detail/141033.html).
         # 
         # >  If the source instance is a self-managed database with a public IP address or a third-party cloud database, you can set the parameter to **cn-hangzhou** or the ID of the closest region.
+        # 
+        # This parameter is required.
         self.type = type
         self.zero_etl_job = zero_etl_job
 
     def validate(self):
         pass
 
     def to_map(self):
```

### Comparing `alibabacloud_dts20200101-5.6.0/alibabacloud_dts20200101.egg-info/PKG-INFO` & `alibabacloud_dts20200101-5.6.1/alibabacloud_dts20200101.egg-info/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: alibabacloud-dts20200101
-Version: 5.6.0
+Version: 5.6.1
 Summary: Alibaba Cloud Data Transmission (20200101) SDK Library for Python
 Home-page: https://github.com/aliyun/alibabacloud-python-sdk
 Author: Alibaba Cloud SDK
 Author-email: sdk-team@alibabacloud.com
 License: Apache License 2.0
 Description: English | [简体中文](README-CN.md)
         ![](https://aliyunsdk-pages.alicdn.com/icons/AlibabaCloud.svg)
```

### Comparing `alibabacloud_dts20200101-5.6.0/setup.py` & `alibabacloud_dts20200101-5.6.1/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -20,33 +20,33 @@
 
 import os
 from setuptools import setup, find_packages
 
 """
 setup module for alibabacloud_dts20200101.
 
-Created on 09/05/2024
+Created on 29/05/2024
 
 @author: Alibaba Cloud SDK
 """
 
 PACKAGE = "alibabacloud_dts20200101"
 NAME = "alibabacloud_dts20200101" or "alibabacloud-package"
 DESCRIPTION = "Alibaba Cloud Data Transmission (20200101) SDK Library for Python"
 AUTHOR = "Alibaba Cloud SDK"
 AUTHOR_EMAIL = "sdk-team@alibabacloud.com"
 URL = "https://github.com/aliyun/alibabacloud-python-sdk"
 VERSION = __import__(PACKAGE).__version__
 REQUIRES = [
-    "alibabacloud_tea_util>=0.3.11, <1.0.0",
+    "alibabacloud_tea_util>=0.3.12, <1.0.0",
     "alibabacloud_oss_sdk>=0.1.0, <1.0.0",
     "alibabacloud_openplatform20191219>=2.0.0, <3.0.0",
     "alibabacloud_oss_util>=0.0.5, <1.0.0",
     "alibabacloud_tea_fileform>=0.0.3, <1.0.0",
-    "alibabacloud_tea_openapi>=0.3.8, <1.0.0",
+    "alibabacloud_tea_openapi>=0.3.9, <1.0.0",
     "alibabacloud_openapi_util>=0.2.1, <1.0.0",
     "alibabacloud_endpoint_util>=0.0.3, <1.0.0"
 ]
 
 LONG_DESCRIPTION = ''
 if os.path.exists('./README.md'):
     with open("README.md", encoding='utf-8') as fp:
```

