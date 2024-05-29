# Comparing `tmp/alibabacloud_eiam20211201-1.3.2.tar.gz` & `tmp/alibabacloud_eiam20211201-1.3.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/alibabacloud_eiam20211201-1.3.2.tar", last modified: Tue Mar 12 17:16:20 2024, max compression
+gzip compressed data, was "dist/alibabacloud_eiam20211201-1.3.3.tar", last modified: Wed May 29 17:10:23 2024, max compression
```

## Comparing `alibabacloud_eiam20211201-1.3.2.tar` & `alibabacloud_eiam20211201-1.3.3.tar`

### file list

```diff
@@ -1,19 +1,19 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-03-12 17:16:20.000000 alibabacloud_eiam20211201-1.3.2/
--rw-r--r--   0 root         (0) root         (0)      268 2024-03-12 17:16:20.000000 alibabacloud_eiam20211201-1.3.2/ChangeLog.md
--rw-r--r--   0 root         (0) root         (0)      600 2024-03-12 17:16:20.000000 alibabacloud_eiam20211201-1.3.2/LICENSE
--rw-r--r--   0 root         (0) root         (0)       29 2024-03-12 17:16:20.000000 alibabacloud_eiam20211201-1.3.2/MANIFEST.in
--rw-r--r--   0 root         (0) root         (0)     2408 2024-03-12 17:16:20.000000 alibabacloud_eiam20211201-1.3.2/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)     1099 2024-03-12 17:16:20.000000 alibabacloud_eiam20211201-1.3.2/README-CN.md
--rw-r--r--   0 root         (0) root         (0)     1184 2024-03-12 17:16:20.000000 alibabacloud_eiam20211201-1.3.2/README.md
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-03-12 17:16:20.000000 alibabacloud_eiam20211201-1.3.2/alibabacloud_eiam20211201/
--rw-r--r--   0 root         (0) root         (0)       21 2024-03-12 17:16:20.000000 alibabacloud_eiam20211201-1.3.2/alibabacloud_eiam20211201/__init__.py
--rw-r--r--   0 root         (0) root         (0)   367256 2024-03-12 17:16:20.000000 alibabacloud_eiam20211201-1.3.2/alibabacloud_eiam20211201/client.py
--rw-r--r--   0 root         (0) root         (0)   617276 2024-03-12 17:16:20.000000 alibabacloud_eiam20211201-1.3.2/alibabacloud_eiam20211201/models.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-03-12 17:16:20.000000 alibabacloud_eiam20211201-1.3.2/alibabacloud_eiam20211201.egg-info/
--rw-r--r--   0 root         (0) root         (0)     2408 2024-03-12 17:16:20.000000 alibabacloud_eiam20211201-1.3.2/alibabacloud_eiam20211201.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)      428 2024-03-12 17:16:20.000000 alibabacloud_eiam20211201-1.3.2/alibabacloud_eiam20211201.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2024-03-12 17:16:20.000000 alibabacloud_eiam20211201-1.3.2/alibabacloud_eiam20211201.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)      157 2024-03-12 17:16:20.000000 alibabacloud_eiam20211201-1.3.2/alibabacloud_eiam20211201.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)       26 2024-03-12 17:16:20.000000 alibabacloud_eiam20211201-1.3.2/alibabacloud_eiam20211201.egg-info/top_level.txt
--rw-r--r--   0 root         (0) root         (0)       73 2024-03-12 17:16:20.000000 alibabacloud_eiam20211201-1.3.2/setup.cfg
--rw-r--r--   0 root         (0) root         (0)     2616 2024-03-12 17:16:20.000000 alibabacloud_eiam20211201-1.3.2/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-29 17:10:23.000000 alibabacloud_eiam20211201-1.3.3/
+-rw-r--r--   0 root         (0) root         (0)      395 2024-05-29 17:10:22.000000 alibabacloud_eiam20211201-1.3.3/ChangeLog.md
+-rw-r--r--   0 root         (0) root         (0)      600 2024-05-29 17:10:22.000000 alibabacloud_eiam20211201-1.3.3/LICENSE
+-rw-r--r--   0 root         (0) root         (0)       29 2024-05-29 17:10:22.000000 alibabacloud_eiam20211201-1.3.3/MANIFEST.in
+-rw-r--r--   0 root         (0) root         (0)     2408 2024-05-29 17:10:23.000000 alibabacloud_eiam20211201-1.3.3/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)     1099 2024-05-29 17:10:22.000000 alibabacloud_eiam20211201-1.3.3/README-CN.md
+-rw-r--r--   0 root         (0) root         (0)     1184 2024-05-29 17:10:22.000000 alibabacloud_eiam20211201-1.3.3/README.md
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-29 17:10:23.000000 alibabacloud_eiam20211201-1.3.3/alibabacloud_eiam20211201/
+-rw-r--r--   0 root         (0) root         (0)       21 2024-05-29 17:10:22.000000 alibabacloud_eiam20211201-1.3.3/alibabacloud_eiam20211201/__init__.py
+-rw-r--r--   0 root         (0) root         (0)   500248 2024-05-29 17:10:22.000000 alibabacloud_eiam20211201-1.3.3/alibabacloud_eiam20211201/client.py
+-rw-r--r--   0 root         (0) root         (0)   631061 2024-05-29 17:10:22.000000 alibabacloud_eiam20211201-1.3.3/alibabacloud_eiam20211201/models.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-29 17:10:23.000000 alibabacloud_eiam20211201-1.3.3/alibabacloud_eiam20211201.egg-info/
+-rw-r--r--   0 root         (0) root         (0)     2408 2024-05-29 17:10:23.000000 alibabacloud_eiam20211201-1.3.3/alibabacloud_eiam20211201.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)      428 2024-05-29 17:10:23.000000 alibabacloud_eiam20211201-1.3.3/alibabacloud_eiam20211201.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2024-05-29 17:10:23.000000 alibabacloud_eiam20211201-1.3.3/alibabacloud_eiam20211201.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)      157 2024-05-29 17:10:23.000000 alibabacloud_eiam20211201-1.3.3/alibabacloud_eiam20211201.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)       26 2024-05-29 17:10:23.000000 alibabacloud_eiam20211201-1.3.3/alibabacloud_eiam20211201.egg-info/top_level.txt
+-rw-r--r--   0 root         (0) root         (0)       73 2024-05-29 17:10:23.000000 alibabacloud_eiam20211201-1.3.3/setup.cfg
+-rw-r--r--   0 root         (0) root         (0)     2616 2024-05-29 17:10:22.000000 alibabacloud_eiam20211201-1.3.3/setup.py
```

### Comparing `alibabacloud_eiam20211201-1.3.2/LICENSE` & `alibabacloud_eiam20211201-1.3.3/LICENSE`

 * *Files identical despite different names*

### Comparing `alibabacloud_eiam20211201-1.3.2/PKG-INFO` & `alibabacloud_eiam20211201-1.3.3/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: alibabacloud_eiam20211201
-Version: 1.3.2
+Version: 1.3.3
 Summary: Alibaba Cloud Eiam (20211201) SDK Library for Python
 Home-page: https://github.com/aliyun/alibabacloud-python-sdk
 Author: Alibaba Cloud SDK
 Author-email: sdk-team@alibabacloud.com
 License: Apache License 2.0
 Description: English | [简体中文](README-CN.md)
         ![](https://aliyunsdk-pages.alicdn.com/icons/AlibabaCloud.svg)
```

### Comparing `alibabacloud_eiam20211201-1.3.2/README-CN.md` & `alibabacloud_eiam20211201-1.3.3/README-CN.md`

 * *Files identical despite different names*

### Comparing `alibabacloud_eiam20211201-1.3.2/README.md` & `alibabacloud_eiam20211201-1.3.3/README.md`

 * *Files identical despite different names*

### Comparing `alibabacloud_eiam20211201-1.3.2/alibabacloud_eiam20211201/models.py` & `alibabacloud_eiam20211201-1.3.3/alibabacloud_eiam20211201/models.py`

 * *Files 5% similar despite different names*

```diff
@@ -8,18 +8,24 @@
     def __init__(
         self,
         instance_id: str = None,
         organizational_unit_ids: List[str] = None,
         user_id: str = None,
     ):
         # The instance ID.
+        # 
+        # This parameter is required.
         self.instance_id = instance_id
         # The organization IDs. You can add an account to a maximum of 100 organizations.
+        # 
+        # This parameter is required.
         self.organizational_unit_ids = organizational_unit_ids
         # The account ID.
+        # 
+        # This parameter is required.
         self.user_id = user_id
 
     def validate(self):
         pass
 
     def to_map(self):
         _map = super().to_map()
@@ -119,18 +125,24 @@
     def __init__(
         self,
         group_id: str = None,
         instance_id: str = None,
         user_ids: List[str] = None,
     ):
         # The group ID.
+        # 
+        # This parameter is required.
         self.group_id = group_id
         # The instance ID.
+        # 
+        # This parameter is required.
         self.instance_id = instance_id
         # The account IDs.
+        # 
+        # This parameter is required.
         self.user_ids = user_ids
 
     def validate(self):
         pass
 
     def to_map(self):
         _map = super().to_map()
@@ -230,18 +242,24 @@
     def __init__(
         self,
         application_id: str = None,
         group_ids: List[str] = None,
         instance_id: str = None,
     ):
         # The application ID.
+        # 
+        # This parameter is required.
         self.application_id = application_id
         # The group IDs. You can specify up to 100 group IDs at a time.
+        # 
+        # This parameter is required.
         self.group_ids = group_ids
         # The instance ID.
+        # 
+        # This parameter is required.
         self.instance_id = instance_id
 
     def validate(self):
         pass
 
     def to_map(self):
         _map = super().to_map()
@@ -341,18 +359,24 @@
     def __init__(
         self,
         application_id: str = None,
         instance_id: str = None,
         organizational_unit_ids: List[str] = None,
     ):
         # The ID of the application on which you want to grant permissions.
+        # 
+        # This parameter is required.
         self.application_id = application_id
         # The ID of the instance.
+        # 
+        # This parameter is required.
         self.instance_id = instance_id
         # The IDs of the organizations to which you want to grant permissions. You can grant permissions to a maximum of 100 organizations at a time.
+        # 
+        # This parameter is required.
         self.organizational_unit_ids = organizational_unit_ids
 
     def validate(self):
         pass
 
     def to_map(self):
         _map = super().to_map()
@@ -452,18 +476,24 @@
     def __init__(
         self,
         application_id: str = None,
         instance_id: str = None,
         user_ids: List[str] = None,
     ):
         # The ID of the application on which you want to grant permissions.
+        # 
+        # This parameter is required.
         self.application_id = application_id
         # The ID of the instance.
+        # 
+        # This parameter is required.
         self.instance_id = instance_id
         # The IDs of the accounts to which you want to grant permissions. You can grant permissions to a maximum of 100 accounts at a time.
+        # 
+        # This parameter is required.
         self.user_ids = user_ids
 
     def validate(self):
         pass
 
     def to_map(self):
         _map = super().to_map()
@@ -567,32 +597,40 @@
         application_template_id: str = None,
         description: str = None,
         instance_id: str = None,
         logo_url: str = None,
         sso_type: str = None,
     ):
         # The name of the application.
+        # 
+        # This parameter is required.
         self.application_name = application_name
         # The type of the application source. Valid values:
         # 
         # *   urn:alibaba:idaas:app:source:template: application template
         # *   urn:alibaba:idaas:app:source:standard: standard protocol
+        # 
+        # This parameter is required.
         self.application_source_type = application_source_type
         # The ID of the application template. This parameter is required if you set the ApplicationSourceType parameter to urn:alibaba:idaas:app:source:template.
         self.application_template_id = application_template_id
         # The description of the application.
         self.description = description
         # The ID of the instance.
+        # 
+        # This parameter is required.
         self.instance_id = instance_id
         # The URL of the application logo.
         self.logo_url = logo_url
         # The SSO protocol. Valid values:
         # 
         # *   saml2: the SAML 2.0 protocol.
         # *   oidc: the OpenID Connect protocol.
+        # 
+        # This parameter is required.
         self.sso_type = sso_type
 
     def validate(self):
         pass
 
     def to_map(self):
         _map = super().to_map()
@@ -714,16 +752,20 @@
 class CreateApplicationClientSecretRequest(TeaModel):
     def __init__(
         self,
         application_id: str = None,
         instance_id: str = None,
     ):
         # The ID of the application for which you want to create a client key.
+        # 
+        # This parameter is required.
         self.application_id = application_id
         # The ID of the instance.
+        # 
+        # This parameter is required.
         self.instance_id = instance_id
 
     def validate(self):
         pass
 
     def to_map(self):
         _map = super().to_map()
@@ -898,18 +940,22 @@
     def __init__(
         self,
         domain: str = None,
         filing: CreateDomainRequestFiling = None,
         instance_id: str = None,
     ):
         # 域名。最大长度限制255，格式由数字、字母、横线（-）点（.）组成;
+        # 
+        # This parameter is required.
         self.domain = domain
         # 备案信息参数。
         self.filing = filing
         # IDaaS EIAM实例的ID。
+        # 
+        # This parameter is required.
         self.instance_id = instance_id
 
     def validate(self):
         if self.filing:
             self.filing.validate()
 
     def to_map(self):
@@ -1015,16 +1061,20 @@
 class CreateDomainProxyTokenRequest(TeaModel):
     def __init__(
         self,
         domain_id: str = None,
         instance_id: str = None,
     ):
         # 域名ID。
+        # 
+        # This parameter is required.
         self.domain_id = domain_id
         # IDaaS EIAM实例的ID。
+        # 
+        # This parameter is required.
         self.instance_id = instance_id
 
     def validate(self):
         pass
 
     def to_map(self):
         _map = super().to_map()
@@ -1130,16 +1180,20 @@
         instance_id: str = None,
     ):
         # The description of the group. The value can be up to 256 characters in length.
         self.description = description
         # The external ID of the group, which can be used to associate the group with an external system. By default, the external ID is the group ID. The value can be up to 64 characters in length.
         self.group_external_id = group_external_id
         # The name of the group. The name can be up to 64 characters in length.
+        # 
+        # This parameter is required.
         self.group_name = group_name
         # The instance ID.
+        # 
+        # This parameter is required.
         self.instance_id = instance_id
 
     def validate(self):
         pass
 
     def to_map(self):
         _map = super().to_map()
@@ -1359,22 +1413,30 @@
         v_switch_ids: List[str] = None,
         vpc_id: str = None,
         vpc_region_id: str = None,
     ):
         # 保证请求幂等性。从您的客户端生成一个参数值，确保不同请求间该参数值唯一。ClientToken只支持ASCII字符，且不能超过64个字符。
         self.client_token = client_token
         # IDaaS EIAM实例的ID。
+        # 
+        # This parameter is required.
         self.instance_id = instance_id
         # 专属网络端点名称。
+        # 
+        # This parameter is required.
         self.network_access_endpoint_name = network_access_endpoint_name
         # 专属网络端点连接的指定vSwitch。
         self.v_switch_ids = v_switch_ids
         # 专属网络端点连接的VpcID。
+        # 
+        # This parameter is required.
         self.vpc_id = vpc_id
         # 专属网络端点连接的VpcID所属地域，该地域取值必须在ListNetworkAccessEndpointAvailableRegions接口中返回。
+        # 
+        # This parameter is required.
         self.vpc_region_id = vpc_region_id
 
     def validate(self):
         pass
 
     def to_map(self):
         _map = super().to_map()
@@ -1495,20 +1557,26 @@
         organizational_unit_external_id: str = None,
         organizational_unit_name: str = None,
         parent_id: str = None,
     ):
         # The description of the organization. The value can be up to 256 characters in length.
         self.description = description
         # The instance ID.
+        # 
+        # This parameter is required.
         self.instance_id = instance_id
         # The external ID of the organization, which can be used to associate the organization with an external system. By default, the external ID is the organization ID. The value can be up to 64 characters in length.
         self.organizational_unit_external_id = organizational_unit_external_id
         # The name of the organization. The name can be up to 64 characters in length.
+        # 
+        # This parameter is required.
         self.organizational_unit_name = organizational_unit_name
         # The parent organization ID.
+        # 
+        # This parameter is required.
         self.parent_id = parent_id
 
     def validate(self):
         pass
 
     def to_map(self):
         _map = super().to_map()
@@ -1732,37 +1800,43 @@
     ):
         # The extended fields.
         self.custom_fields = custom_fields
         # The description of the organizational unit. The description can be up to 256 characters in length.
         self.description = description
         # The display name of the account. The display name can be up to 64 characters in length.
         self.display_name = display_name
-        # The email address of the user who owns the account. The email address prefix can contain letters, digits, underscores (\_), periods (.), and hyphens (-).
+        # The email address of the user who owns the account. The email address prefix can contain letters, digits, underscores (_), periods (.), and hyphens (-).
         self.email = email
         # Specifies whether the email address is a trusted email address. This parameter is required if the Email parameter is specified. If you have no special business requirements, set this parameter to true.
         self.email_verified = email_verified
         # The ID of the instance.
+        # 
+        # This parameter is required.
         self.instance_id = instance_id
         # The IDs of organizational units to which the account belongs. An account can belong to multiple organizational units.
         self.organizational_unit_ids = organizational_unit_ids
         # The password of the account. For more information, view the password policy of the instance in the IDaaS console.
         self.password = password
         # The configurations for password initialization.
         self.password_initialization_config = password_initialization_config
         # The mobile phone number, which contains 6 to 15 digits.
         self.phone_number = phone_number
         # Specifies whether the mobile phone number is a trusted mobile phone number. This parameter is required if the PhoneNumber parameter is specified. If you have no special business requirements, set this parameter to true.
         self.phone_number_verified = phone_number_verified
         # The country code of the mobile phone number. The country code contains only digits and does not contain a plus sign (+).
         self.phone_region = phone_region
         # The ID of the primary organizational unit to which the account belongs.
+        # 
+        # This parameter is required.
         self.primary_organizational_unit_id = primary_organizational_unit_id
         # The external ID of the account. The external ID can be used to associate the account with an external system. The external ID can be up to 64 characters in length. If you do not specify an external ID for the account, the ID of the account is used as the external ID by default.
         self.user_external_id = user_external_id
-        # The name of the account. The name can be up to 64 characters in length and can contain letters, digits, underscores (\_), periods (.), at signs (@), and hyphens (-).
+        # The name of the account. The name can be up to 64 characters in length and can contain letters, digits, underscores (_), periods (.), at signs (@), and hyphens (-).
+        # 
+        # This parameter is required.
         self.username = username
 
     def validate(self):
         if self.custom_fields:
             for k in self.custom_fields:
                 if k:
                     k.validate()
@@ -1927,16 +2001,20 @@
 class DeleteApplicationRequest(TeaModel):
     def __init__(
         self,
         application_id: str = None,
         instance_id: str = None,
     ):
         # The ID of the application that you want to delete.
+        # 
+        # This parameter is required.
         self.application_id = application_id
         # The ID of the instance.
+        # 
+        # This parameter is required.
         self.instance_id = instance_id
 
     def validate(self):
         pass
 
     def to_map(self):
         _map = super().to_map()
@@ -2032,18 +2110,24 @@
     def __init__(
         self,
         application_id: str = None,
         instance_id: str = None,
         secret_id: str = None,
     ):
         # The ID of the application for which you want to delete a client key.
+        # 
+        # This parameter is required.
         self.application_id = application_id
         # The ID of the instance.
+        # 
+        # This parameter is required.
         self.instance_id = instance_id
         # The ID of the client key that you want to delete for the application.
+        # 
+        # This parameter is required.
         self.secret_id = secret_id
 
     def validate(self):
         pass
 
     def to_map(self):
         _map = super().to_map()
@@ -2142,16 +2226,20 @@
 class DeleteDomainRequest(TeaModel):
     def __init__(
         self,
         domain_id: str = None,
         instance_id: str = None,
     ):
         # 域名ID。
+        # 
+        # This parameter is required.
         self.domain_id = domain_id
         # IDaaS EIAM实例的ID。
+        # 
+        # This parameter is required.
         self.instance_id = instance_id
 
     def validate(self):
         pass
 
     def to_map(self):
         _map = super().to_map()
@@ -2246,18 +2334,24 @@
     def __init__(
         self,
         domain_id: str = None,
         domain_proxy_token_id: str = None,
         instance_id: str = None,
     ):
         # 域名ID。
+        # 
+        # This parameter is required.
         self.domain_id = domain_id
         # 域名代理Token ID。
+        # 
+        # This parameter is required.
         self.domain_proxy_token_id = domain_proxy_token_id
         # IDaaS EIAM实例的ID。
+        # 
+        # This parameter is required.
         self.instance_id = instance_id
 
     def validate(self):
         pass
 
     def to_map(self):
         _map = super().to_map()
@@ -2355,16 +2449,20 @@
 class DeleteGroupRequest(TeaModel):
     def __init__(
         self,
         group_id: str = None,
         instance_id: str = None,
     ):
         # The group ID.
+        # 
+        # This parameter is required.
         self.group_id = group_id
         # The instance ID.
+        # 
+        # This parameter is required.
         self.instance_id = instance_id
 
     def validate(self):
         pass
 
     def to_map(self):
         _map = super().to_map()
@@ -2458,14 +2556,16 @@
 
 class DeleteInstanceRequest(TeaModel):
     def __init__(
         self,
         instance_id: str = None,
     ):
         # The ID of the instance to be deleted.
+        # 
+        # This parameter is required.
         self.instance_id = instance_id
 
     def validate(self):
         pass
 
     def to_map(self):
         _map = super().to_map()
@@ -2556,16 +2656,20 @@
 class DeleteNetworkAccessEndpointRequest(TeaModel):
     def __init__(
         self,
         instance_id: str = None,
         network_access_endpoint_id: str = None,
     ):
         # IDaaS EIAM实例的ID。
+        # 
+        # This parameter is required.
         self.instance_id = instance_id
         # 专属网络端点ID。
+        # 
+        # This parameter is required.
         self.network_access_endpoint_id = network_access_endpoint_id
 
     def validate(self):
         pass
 
     def to_map(self):
         _map = super().to_map()
@@ -2659,16 +2763,20 @@
 class DeleteOrganizationalUnitRequest(TeaModel):
     def __init__(
         self,
         instance_id: str = None,
         organizational_unit_id: str = None,
     ):
         # The instance ID.
+        # 
+        # This parameter is required.
         self.instance_id = instance_id
         # The organization ID.
+        # 
+        # This parameter is required.
         self.organizational_unit_id = organizational_unit_id
 
     def validate(self):
         pass
 
     def to_map(self):
         _map = super().to_map()
@@ -2763,16 +2871,20 @@
 class DeleteUserRequest(TeaModel):
     def __init__(
         self,
         instance_id: str = None,
         user_id: str = None,
     ):
         # The instance ID.
+        # 
+        # This parameter is required.
         self.instance_id = instance_id
         # The account ID.
+        # 
+        # This parameter is required.
         self.user_id = user_id
 
     def validate(self):
         pass
 
     def to_map(self):
         _map = super().to_map()
@@ -2867,16 +2979,20 @@
 class DisableApplicationRequest(TeaModel):
     def __init__(
         self,
         application_id: str = None,
         instance_id: str = None,
     ):
         # The ID of the application that you want to disable.
+        # 
+        # This parameter is required.
         self.application_id = application_id
         # The ID of the instance.
+        # 
+        # This parameter is required.
         self.instance_id = instance_id
 
     def validate(self):
         pass
 
     def to_map(self):
         _map = super().to_map()
@@ -2971,16 +3087,20 @@
 class DisableApplicationApiInvokeRequest(TeaModel):
     def __init__(
         self,
         application_id: str = None,
         instance_id: str = None,
     ):
         # The ID of the application.
+        # 
+        # This parameter is required.
         self.application_id = application_id
         # The ID of the instance.
+        # 
+        # This parameter is required.
         self.instance_id = instance_id
 
     def validate(self):
         pass
 
     def to_map(self):
         _map = super().to_map()
@@ -3076,18 +3196,24 @@
     def __init__(
         self,
         application_id: str = None,
         instance_id: str = None,
         secret_id: str = None,
     ):
         # The ID of the application for which you want to disable a client key.
+        # 
+        # This parameter is required.
         self.application_id = application_id
         # The ID of the instance.
+        # 
+        # This parameter is required.
         self.instance_id = instance_id
         # The client key ID of the application.
+        # 
+        # This parameter is required.
         self.secret_id = secret_id
 
     def validate(self):
         pass
 
     def to_map(self):
         _map = super().to_map()
@@ -3186,16 +3312,20 @@
 class DisableApplicationProvisioningRequest(TeaModel):
     def __init__(
         self,
         application_id: str = None,
         instance_id: str = None,
     ):
         # The ID of the application.
+        # 
+        # This parameter is required.
         self.application_id = application_id
         # The ID of the instance.
+        # 
+        # This parameter is required.
         self.instance_id = instance_id
 
     def validate(self):
         pass
 
     def to_map(self):
         _map = super().to_map()
@@ -3290,16 +3420,20 @@
 class DisableApplicationSsoRequest(TeaModel):
     def __init__(
         self,
         application_id: str = None,
         instance_id: str = None,
     ):
         # IDaaS的应用主键id
+        # 
+        # This parameter is required.
         self.application_id = application_id
         # IDaaS EIAM的实例id
+        # 
+        # This parameter is required.
         self.instance_id = instance_id
 
     def validate(self):
         pass
 
     def to_map(self):
         _map = super().to_map()
@@ -3394,18 +3528,24 @@
     def __init__(
         self,
         domain_id: str = None,
         domain_proxy_token_id: str = None,
         instance_id: str = None,
     ):
         # 域名ID。
+        # 
+        # This parameter is required.
         self.domain_id = domain_id
         # 域名代理Token ID。
+        # 
+        # This parameter is required.
         self.domain_proxy_token_id = domain_proxy_token_id
         # IDaaS EIAM实例的ID。
+        # 
+        # This parameter is required.
         self.instance_id = instance_id
 
     def validate(self):
         pass
 
     def to_map(self):
         _map = super().to_map()
@@ -3502,14 +3642,16 @@
 
 class DisableInitDomainAutoRedirectRequest(TeaModel):
     def __init__(
         self,
         instance_id: str = None,
     ):
         # IDaaS EIAM实例的ID。
+        # 
+        # This parameter is required.
         self.instance_id = instance_id
 
     def validate(self):
         pass
 
     def to_map(self):
         _map = super().to_map()
@@ -3599,16 +3741,20 @@
 class DisableUserRequest(TeaModel):
     def __init__(
         self,
         instance_id: str = None,
         user_id: str = None,
     ):
         # The instance ID.
+        # 
+        # This parameter is required.
         self.instance_id = instance_id
         # The ID of the account.
+        # 
+        # This parameter is required.
         self.user_id = user_id
 
     def validate(self):
         pass
 
     def to_map(self):
         _map = super().to_map()
@@ -3703,16 +3849,20 @@
 class EnableApplicationRequest(TeaModel):
     def __init__(
         self,
         application_id: str = None,
         instance_id: str = None,
     ):
         # The ID of the application that you want to enable.
+        # 
+        # This parameter is required.
         self.application_id = application_id
         # The ID of the instance.
+        # 
+        # This parameter is required.
         self.instance_id = instance_id
 
     def validate(self):
         pass
 
     def to_map(self):
         _map = super().to_map()
@@ -3807,16 +3957,20 @@
 class EnableApplicationApiInvokeRequest(TeaModel):
     def __init__(
         self,
         application_id: str = None,
         instance_id: str = None,
     ):
         # The ID of the application.
+        # 
+        # This parameter is required.
         self.application_id = application_id
         # The ID of the instance.
+        # 
+        # This parameter is required.
         self.instance_id = instance_id
 
     def validate(self):
         pass
 
     def to_map(self):
         _map = super().to_map()
@@ -3912,18 +4066,24 @@
     def __init__(
         self,
         application_id: str = None,
         instance_id: str = None,
         secret_id: str = None,
     ):
         # The ID of the application.
+        # 
+        # This parameter is required.
         self.application_id = application_id
         # The ID of the instance.
+        # 
+        # This parameter is required.
         self.instance_id = instance_id
         # The client key ID of the application.
+        # 
+        # This parameter is required.
         self.secret_id = secret_id
 
     def validate(self):
         pass
 
     def to_map(self):
         _map = super().to_map()
@@ -4022,16 +4182,20 @@
 class EnableApplicationProvisioningRequest(TeaModel):
     def __init__(
         self,
         application_id: str = None,
         instance_id: str = None,
     ):
         # The ID of the application.
+        # 
+        # This parameter is required.
         self.application_id = application_id
         # The ID of the instance.
+        # 
+        # This parameter is required.
         self.instance_id = instance_id
 
     def validate(self):
         pass
 
     def to_map(self):
         _map = super().to_map()
@@ -4126,16 +4290,20 @@
 class EnableApplicationSsoRequest(TeaModel):
     def __init__(
         self,
         application_id: str = None,
         instance_id: str = None,
     ):
         # IDaaS的应用主键id
+        # 
+        # This parameter is required.
         self.application_id = application_id
         # IDaaS EIAM的实例id
+        # 
+        # This parameter is required.
         self.instance_id = instance_id
 
     def validate(self):
         pass
 
     def to_map(self):
         _map = super().to_map()
@@ -4230,18 +4398,24 @@
     def __init__(
         self,
         domain_id: str = None,
         domain_proxy_token_id: str = None,
         instance_id: str = None,
     ):
         # 域名ID。
+        # 
+        # This parameter is required.
         self.domain_id = domain_id
         # 域名代理Token ID。
+        # 
+        # This parameter is required.
         self.domain_proxy_token_id = domain_proxy_token_id
         # IDaaS EIAM实例的ID。
+        # 
+        # This parameter is required.
         self.instance_id = instance_id
 
     def validate(self):
         pass
 
     def to_map(self):
         _map = super().to_map()
@@ -4338,14 +4512,16 @@
 
 class EnableInitDomainAutoRedirectRequest(TeaModel):
     def __init__(
         self,
         instance_id: str = None,
     ):
         # IDaaS EIAM实例的ID。
+        # 
+        # This parameter is required.
         self.instance_id = instance_id
 
     def validate(self):
         pass
 
     def to_map(self):
         _map = super().to_map()
@@ -4435,16 +4611,20 @@
 class EnableUserRequest(TeaModel):
     def __init__(
         self,
         instance_id: str = None,
         user_id: str = None,
     ):
         # The instance ID.
+        # 
+        # This parameter is required.
         self.instance_id = instance_id
         # The account ID.
+        # 
+        # This parameter is required.
         self.user_id = user_id
 
     def validate(self):
         pass
 
     def to_map(self):
         _map = super().to_map()
@@ -4539,16 +4719,20 @@
 class GetApplicationRequest(TeaModel):
     def __init__(
         self,
         application_id: str = None,
         instance_id: str = None,
     ):
         # The ID of the application that you want to query.
+        # 
+        # This parameter is required.
         self.application_id = application_id
         # The ID of the instance.
+        # 
+        # This parameter is required.
         self.instance_id = instance_id
 
     def validate(self):
         pass
 
     def to_map(self):
         _map = super().to_map()
@@ -4811,16 +4995,20 @@
 class GetApplicationGrantScopeRequest(TeaModel):
     def __init__(
         self,
         application_id: str = None,
         instance_id: str = None,
     ):
         # The ID of the application.
+        # 
+        # This parameter is required.
         self.application_id = application_id
         # The ID of the instance.
+        # 
+        # This parameter is required.
         self.instance_id = instance_id
 
     def validate(self):
         pass
 
     def to_map(self):
         _map = super().to_map()
@@ -4952,16 +5140,20 @@
 class GetApplicationProvisioningConfigRequest(TeaModel):
     def __init__(
         self,
         application_id: str = None,
         instance_id: str = None,
     ):
         # The ID of the application.
+        # 
+        # This parameter is required.
         self.application_id = application_id
         # The ID of the instance.
+        # 
+        # This parameter is required.
         self.instance_id = instance_id
 
     def validate(self):
         pass
 
     def to_map(self):
         _map = super().to_map()
@@ -5385,16 +5577,20 @@
 class GetApplicationProvisioningScopeRequest(TeaModel):
     def __init__(
         self,
         application_id: str = None,
         instance_id: str = None,
     ):
         # The ID of the application.
+        # 
+        # This parameter is required.
         self.application_id = application_id
         # The ID of the instance.
+        # 
+        # This parameter is required.
         self.instance_id = instance_id
 
     def validate(self):
         pass
 
     def to_map(self):
         _map = super().to_map()
@@ -5416,36 +5612,57 @@
             self.instance_id = m.get('InstanceId')
         return self
 
 
 class GetApplicationProvisioningScopeResponseBodyApplicationProvisioningScope(TeaModel):
     def __init__(
         self,
+        group_ids: List[str] = None,
+        max_quota: int = None,
         organizational_unit_ids: List[str] = None,
+        used_quota: int = None,
     ):
+        # 同步授权的组列表
+        self.group_ids = group_ids
+        # 租户最大授权主体quota数量
+        self.max_quota = max_quota
         # The list of organizational units that are authorized for account synchronization.
         self.organizational_unit_ids = organizational_unit_ids
+        # 已使用授权主体quota数量
+        self.used_quota = used_quota
 
     def validate(self):
         pass
 
     def to_map(self):
         _map = super().to_map()
         if _map is not None:
             return _map
 
         result = dict()
+        if self.group_ids is not None:
+            result['GroupIds'] = self.group_ids
+        if self.max_quota is not None:
+            result['MaxQuota'] = self.max_quota
         if self.organizational_unit_ids is not None:
             result['OrganizationalUnitIds'] = self.organizational_unit_ids
+        if self.used_quota is not None:
+            result['UsedQuota'] = self.used_quota
         return result
 
     def from_map(self, m: dict = None):
         m = m or dict()
+        if m.get('GroupIds') is not None:
+            self.group_ids = m.get('GroupIds')
+        if m.get('MaxQuota') is not None:
+            self.max_quota = m.get('MaxQuota')
         if m.get('OrganizationalUnitIds') is not None:
             self.organizational_unit_ids = m.get('OrganizationalUnitIds')
+        if m.get('UsedQuota') is not None:
+            self.used_quota = m.get('UsedQuota')
         return self
 
 
 class GetApplicationProvisioningScopeResponseBody(TeaModel):
     def __init__(
         self,
         application_provisioning_scope: GetApplicationProvisioningScopeResponseBodyApplicationProvisioningScope = None,
@@ -5526,16 +5743,20 @@
 class GetApplicationSsoConfigRequest(TeaModel):
     def __init__(
         self,
         application_id: str = None,
         instance_id: str = None,
     ):
         # The ID of the application.
+        # 
+        # This parameter is required.
         self.application_id = application_id
         # The ID of the instance.
+        # 
+        # This parameter is required.
         self.instance_id = instance_id
 
     def validate(self):
         pass
 
     def to_map(self):
         _map = super().to_map()
@@ -6108,16 +6329,20 @@
 class GetDomainRequest(TeaModel):
     def __init__(
         self,
         domain_id: str = None,
         instance_id: str = None,
     ):
         # 域名ID。
+        # 
+        # This parameter is required.
         self.domain_id = domain_id
         # IDaaS EIAM实例的ID。
+        # 
+        # This parameter is required.
         self.instance_id = instance_id
 
     def validate(self):
         pass
 
     def to_map(self):
         _map = super().to_map()
@@ -6333,16 +6558,20 @@
 class GetDomainDnsChallengeRequest(TeaModel):
     def __init__(
         self,
         domain: str = None,
         instance_id: str = None,
     ):
         # 域名。
+        # 
+        # This parameter is required.
         self.domain = domain
         # IDaaS EIAM实例的ID。
+        # 
+        # This parameter is required.
         self.instance_id = instance_id
 
     def validate(self):
         pass
 
     def to_map(self):
         _map = super().to_map()
@@ -6485,14 +6714,16 @@
 
 class GetForgetPasswordConfigurationRequest(TeaModel):
     def __init__(
         self,
         instance_id: str = None,
     ):
         # The instance ID.
+        # 
+        # This parameter is required.
         self.instance_id = instance_id
 
     def validate(self):
         pass
 
     def to_map(self):
         _map = super().to_map()
@@ -6648,16 +6879,20 @@
 class GetGroupRequest(TeaModel):
     def __init__(
         self,
         group_id: str = None,
         instance_id: str = None,
     ):
         # The group ID.
+        # 
+        # This parameter is required.
         self.group_id = group_id
         # The instance ID.
+        # 
+        # This parameter is required.
         self.instance_id = instance_id
 
     def validate(self):
         pass
 
     def to_map(self):
         _map = super().to_map()
@@ -6846,14 +7081,16 @@
 
 class GetInstanceRequest(TeaModel):
     def __init__(
         self,
         instance_id: str = None,
     ):
         # The instance ID.
+        # 
+        # This parameter is required.
         self.instance_id = instance_id
 
     def validate(self):
         pass
 
     def to_map(self):
         _map = super().to_map()
@@ -7114,16 +7351,20 @@
 class GetNetworkAccessEndpointRequest(TeaModel):
     def __init__(
         self,
         instance_id: str = None,
         network_access_endpoint_id: str = None,
     ):
         # IDaaS EIAM实例的ID。
+        # 
+        # This parameter is required.
         self.instance_id = instance_id
         # 专属网络端点ID。
+        # 
+        # This parameter is required.
         self.network_access_endpoint_id = network_access_endpoint_id
 
     def validate(self):
         pass
 
     def to_map(self):
         _map = super().to_map()
@@ -7337,16 +7578,20 @@
 class GetOrganizationalUnitRequest(TeaModel):
     def __init__(
         self,
         instance_id: str = None,
         organizational_unit_id: str = None,
     ):
         # The ID of the instance.
+        # 
+        # This parameter is required.
         self.instance_id = instance_id
         # The ID of the organizational unit.
+        # 
+        # This parameter is required.
         self.organizational_unit_id = organizational_unit_id
 
     def validate(self):
         pass
 
     def to_map(self):
         _map = super().to_map()
@@ -7556,14 +7801,16 @@
 
 class GetPasswordComplexityConfigurationRequest(TeaModel):
     def __init__(
         self,
         instance_id: str = None,
     ):
         # The instance ID.
+        # 
+        # This parameter is required.
         self.instance_id = instance_id
 
     def validate(self):
         pass
 
     def to_map(self):
         _map = super().to_map()
@@ -7587,15 +7834,15 @@
         self,
         password_check_type: str = None,
     ):
         # The type of the password check. Valid values:
         # 
         # *   inclusion_upper_case: The password must contain uppercase letters.
         # *   inclusion_lower_case: The password must contain lowercase letters.
-        # *   inclusion_special_case: The password must contain one or more of the following special characters: @ % + \ / \" ! # $ ^ ? : , ( ) { } \[ ] ~ - \_ .
+        # *   inclusion_special_case: The password must contain one or more of the following special characters: @ % + \\ / \\" ! # $ ^ ? : , ( ) { } [ ] ~ - _ .
         # *   inclusion_number: The password must contain digits.
         # *   exclusion_username: The password cannot contain a username.
         # *   exclusion_email: The password cannot contain an email prefix.
         # *   exclusion_phone_number: The password cannot contain a mobile number.
         # *   exclusion_display_name: The password cannot contain a display name.
         self.password_check_type = password_check_type
 
@@ -7742,14 +7989,16 @@
 
 class GetPasswordExpirationConfigurationRequest(TeaModel):
     def __init__(
         self,
         instance_id: str = None,
     ):
         # The ID of the instance.
+        # 
+        # This parameter is required.
         self.instance_id = instance_id
 
     def validate(self):
         pass
 
     def to_map(self):
         _map = super().to_map()
@@ -7928,14 +8177,16 @@
 
 class GetPasswordHistoryConfigurationRequest(TeaModel):
     def __init__(
         self,
         instance_id: str = None,
     ):
         # The instance ID.
+        # 
+        # This parameter is required.
         self.instance_id = instance_id
 
     def validate(self):
         pass
 
     def to_map(self):
         _map = super().to_map()
@@ -8072,14 +8323,16 @@
 
 class GetPasswordInitializationConfigurationRequest(TeaModel):
     def __init__(
         self,
         instance_id: str = None,
     ):
         # The instance ID.
+        # 
+        # This parameter is required.
         self.instance_id = instance_id
 
     def validate(self):
         pass
 
     def to_map(self):
         _map = super().to_map()
@@ -8235,14 +8488,16 @@
 
 class GetRootOrganizationalUnitRequest(TeaModel):
     def __init__(
         self,
         instance_id: str = None,
     ):
         # The ID of the instance.
+        # 
+        # This parameter is required.
         self.instance_id = instance_id
 
     def validate(self):
         pass
 
     def to_map(self):
         _map = super().to_map()
@@ -8405,16 +8660,20 @@
 class GetUserRequest(TeaModel):
     def __init__(
         self,
         instance_id: str = None,
         user_id: str = None,
     ):
         # The ID of the instance.
+        # 
+        # This parameter is required.
         self.instance_id = instance_id
         # The ID of the account.
+        # 
+        # This parameter is required.
         self.user_id = user_id
 
     def validate(self):
         pass
 
     def to_map(self):
         _map = super().to_map()
@@ -8881,16 +9140,20 @@
 class ListApplicationClientSecretsRequest(TeaModel):
     def __init__(
         self,
         application_id: str = None,
         instance_id: str = None,
     ):
         # The ID of the application that you want to query.
+        # 
+        # This parameter is required.
         self.application_id = application_id
         # The ID of the instance.
+        # 
+        # This parameter is required.
         self.instance_id = instance_id
 
     def validate(self):
         pass
 
     def to_map(self):
         _map = super().to_map()
@@ -9094,14 +9357,16 @@
         self.application_name = application_name
         # The authorization of the application. Valid values:
         # 
         # *   authorize_required: Only the user with explicit authorization can access the application.
         # *   default_all: By default, all users can access the application.
         self.authorization_type = authorization_type
         # The ID of the instance.
+        # 
+        # This parameter is required.
         self.instance_id = instance_id
         # The number of the page to return.
         self.page_number = page_number
         # The number of entries to return on each page.
         self.page_size = page_size
         # The status of the application. Valid values:
         # 
@@ -9391,16 +9656,20 @@
         organizational_unit_id: str = None,
         page_number: int = None,
         page_size: int = None,
     ):
         # The IDs of the applications that the EIAM organization can access. You can query a maximum of 100 application IDs at a time.
         self.application_ids = application_ids
         # The ID of the instance.
+        # 
+        # This parameter is required.
         self.instance_id = instance_id
         # The ID of the EIAM organization.
+        # 
+        # This parameter is required.
         self.organizational_unit_id = organizational_unit_id
         # The number of the page to return.
         self.page_number = page_number
         # The number of entries to return on each page.
         self.page_size = page_size
 
     def validate(self):
@@ -9567,25 +9836,29 @@
         page_size: int = None,
         query_mode: str = None,
         user_id: str = None,
     ):
         # The IDs of the applications that the EIAM account can access. You can query a maximum of 100 application IDs at a time.
         self.application_ids = application_ids
         # The ID of the instance.
+        # 
+        # This parameter is required.
         self.instance_id = instance_id
         # The number of the page to return.
         self.page_number = page_number
         # The number of entries to return on each page.
         self.page_size = page_size
         # The query mode. Default value: **OnlyDirect**. Valid values:
         # 
         # *   OnlyDirect: Only the direct permissions are queried. Direct permissions are the permissions that are directly granted to the account.
         # *   IncludeInherit: Both the permissions that are directly granted to the account and the inherited permissions are queried. Inherited permissions are the permissions that an account inherits from the parent organization or the group to which the account belongs.
         self.query_mode = query_mode
         # The ID of the EIAM account.
+        # 
+        # This parameter is required.
         self.user_id = user_id
 
     def validate(self):
         pass
 
     def to_map(self):
         _map = super().to_map()
@@ -9766,16 +10039,20 @@
 class ListDomainProxyTokensRequest(TeaModel):
     def __init__(
         self,
         domain_id: str = None,
         instance_id: str = None,
     ):
         # 域名ID。
+        # 
+        # This parameter is required.
         self.domain_id = domain_id
         # IDaaS EIAM实例的ID。
+        # 
+        # This parameter is required.
         self.instance_id = instance_id
 
     def validate(self):
         pass
 
     def to_map(self):
         _map = super().to_map()
@@ -9959,14 +10236,16 @@
 
 class ListDomainsRequest(TeaModel):
     def __init__(
         self,
         instance_id: str = None,
     ):
         # IDaaS EIAM实例的ID。
+        # 
+        # This parameter is required.
         self.instance_id = instance_id
 
     def validate(self):
         pass
 
     def to_map(self):
         _map = super().to_map()
@@ -10522,14 +10801,16 @@
         # The group IDs.
         self.group_ids = group_ids
         # The name of the group. If you specify this parameter, the query is based on an exact match.
         self.group_name = group_name
         # The prefix of the group name. If you specify this parameter, the query follows the leftmost matching principle.
         self.group_name_starts_with = group_name_starts_with
         # The instance ID.
+        # 
+        # This parameter is required.
         self.instance_id = instance_id
         # The number of the page to return.
         self.page_number = page_number
         # The number of entries to return on each page.
         self.page_size = page_size
 
     def validate(self):
@@ -10759,18 +11040,22 @@
         application_id: str = None,
         group_ids: List[str] = None,
         instance_id: str = None,
         page_number: int = None,
         page_size: int = None,
     ):
         # The application ID.
+        # 
+        # This parameter is required.
         self.application_id = application_id
         # The group IDs. You can specify up to 100 group IDs at a time.
         self.group_ids = group_ids
         # The instance ID.
+        # 
+        # This parameter is required.
         self.instance_id = instance_id
         # The page number.
         self.page_number = page_number
         # The number of entries per page.
         self.page_size = page_size
 
     def validate(self):
@@ -10933,20 +11218,24 @@
         self,
         instance_id: str = None,
         page_number: int = None,
         page_size: int = None,
         user_id: str = None,
     ):
         # The instance ID.
+        # 
+        # This parameter is required.
         self.instance_id = instance_id
         # The number of the page to return.
         self.page_number = page_number
         # The number of entries to return on each page.
         self.page_size = page_size
         # The account ID.
+        # 
+        # This parameter is required.
         self.user_id = user_id
 
     def validate(self):
         pass
 
     def to_map(self):
         _map = super().to_map()
@@ -10977,35 +11266,47 @@
         return self
 
 
 class ListGroupsForUserResponseBodyGroups(TeaModel):
     def __init__(
         self,
         group_id: str = None,
+        group_member_relation_source_id: str = None,
+        group_member_relation_source_type: str = None,
     ):
         # The group ID.
         self.group_id = group_id
+        self.group_member_relation_source_id = group_member_relation_source_id
+        self.group_member_relation_source_type = group_member_relation_source_type
 
     def validate(self):
         pass
 
     def to_map(self):
         _map = super().to_map()
         if _map is not None:
             return _map
 
         result = dict()
         if self.group_id is not None:
             result['GroupId'] = self.group_id
+        if self.group_member_relation_source_id is not None:
+            result['GroupMemberRelationSourceId'] = self.group_member_relation_source_id
+        if self.group_member_relation_source_type is not None:
+            result['GroupMemberRelationSourceType'] = self.group_member_relation_source_type
         return result
 
     def from_map(self, m: dict = None):
         m = m or dict()
         if m.get('GroupId') is not None:
             self.group_id = m.get('GroupId')
+        if m.get('GroupMemberRelationSourceId') is not None:
+            self.group_member_relation_source_id = m.get('GroupMemberRelationSourceId')
+        if m.get('GroupMemberRelationSourceType') is not None:
+            self.group_member_relation_source_type = m.get('GroupMemberRelationSourceType')
         return self
 
 
 class ListGroupsForUserResponseBody(TeaModel):
     def __init__(
         self,
         groups: List[ListGroupsForUserResponseBodyGroups] = None,
@@ -11457,14 +11758,16 @@
 
 class ListNetworkAccessEndpointAvailableZonesRequest(TeaModel):
     def __init__(
         self,
         nae_region_id: str = None,
     ):
         # 专属网络端点支持的地域
+        # 
+        # This parameter is required.
         self.nae_region_id = nae_region_id
 
     def validate(self):
         pass
 
     def to_map(self):
         _map = super().to_map()
@@ -11608,14 +11911,16 @@
         network_access_endpoint_status: str = None,
         network_access_endpoint_type: str = None,
         next_token: str = None,
         vpc_id: str = None,
         vpc_region_id: str = None,
     ):
         # IDaaS EIAM实例的ID。
+        # 
+        # This parameter is required.
         self.instance_id = instance_id
         # 分页查询时每页行数。默认值为20，最大值为100。
         self.max_results = max_results
         # 专属网络端点连接的状态。NetworkAccessEndpointType取值为shared时不生效。
         self.network_access_endpoint_status = network_access_endpoint_status
         # 专属网络端点连接的类型。取值可选范围：1. private - 专属网络端点；2. shared - 共享网络端点
         self.network_access_endpoint_type = network_access_endpoint_type
@@ -11866,16 +12171,20 @@
 class ListNetworkAccessPathsRequest(TeaModel):
     def __init__(
         self,
         instance_id: str = None,
         network_access_endpoint_id: str = None,
     ):
         # IDaaS EIAM实例的ID。
+        # 
+        # This parameter is required.
         self.instance_id = instance_id
         # 专属网络端点ID。
+        # 
+        # This parameter is required.
         self.network_access_endpoint_id = network_access_endpoint_id
 
     def validate(self):
         pass
 
     def to_map(self):
         _map = super().to_map()
@@ -12067,16 +12376,20 @@
 class ListOrganizationalUnitParentsRequest(TeaModel):
     def __init__(
         self,
         instance_id: str = None,
         organizational_unit_id: str = None,
     ):
         # IDaaS EIAM实例的ID。
+        # 
+        # This parameter is required.
         self.instance_id = instance_id
         # 组织ID。
+        # 
+        # This parameter is required.
         self.organizational_unit_id = organizational_unit_id
 
     def validate(self):
         pass
 
     def to_map(self):
         _map = super().to_map()
@@ -12224,14 +12537,16 @@
         organizational_unit_name: str = None,
         organizational_unit_name_starts_with: str = None,
         page_number: int = None,
         page_size: int = None,
         parent_id: str = None,
     ):
         # The ID of the instance.
+        # 
+        # This parameter is required.
         self.instance_id = instance_id
         # 组织ID列表。size限制最大100。
         self.organizational_unit_ids = organizational_unit_ids
         # The name of the organizational unit.
         self.organizational_unit_name = organizational_unit_name
         # 组织名称，左匹配
         self.organizational_unit_name_starts_with = organizational_unit_name_starts_with
@@ -12488,16 +12803,20 @@
         application_id: str = None,
         instance_id: str = None,
         organizational_unit_ids: List[str] = None,
         page_number: int = None,
         page_size: int = None,
     ):
         # The ID of the application that you want to query.
+        # 
+        # This parameter is required.
         self.application_id = application_id
         # The ID of the instance.
+        # 
+        # This parameter is required.
         self.instance_id = instance_id
         # The IDs of the organizations that are allowed to access the application. You can query a maximum of 100 organization IDs at a time.
         self.organizational_unit_ids = organizational_unit_ids
         # The number of the page to return.
         self.page_number = page_number
         # The number of entries to return on each page.
         self.page_size = page_size
@@ -12802,14 +13121,16 @@
         username_starts_with: str = None,
     ):
         # 账户展示名，模糊匹配
         self.display_name_starts_with = display_name_starts_with
         # The email address of the user who owns the account.
         self.email = email
         # The ID of the instance.
+        # 
+        # This parameter is required.
         self.instance_id = instance_id
         # The ID of the organizational unit.
         self.organizational_unit_id = organizational_unit_id
         # The number of the page to return. Default value: 1.
         self.page_number = page_number
         # The number of entries to return on each page. Default value: 20.
         self.page_size = page_size
@@ -13191,16 +13512,20 @@
         application_id: str = None,
         instance_id: str = None,
         page_number: int = None,
         page_size: int = None,
         user_ids: List[str] = None,
     ):
         # The ID of the application.
+        # 
+        # This parameter is required.
         self.application_id = application_id
         # The ID of the instance.
+        # 
+        # This parameter is required.
         self.instance_id = instance_id
         # The number of the page to return
         self.page_number = page_number
         # The number of entries to return on each page.
         self.page_size = page_size
         # The IDs of the accounts. You can query a maximum of 100 accounts at a time.
         self.user_ids = user_ids
@@ -13366,16 +13691,20 @@
         group_id: str = None,
         instance_id: str = None,
         page_number: int = None,
         page_size: int = None,
         user_ids: List[str] = None,
     ):
         # The group ID.
+        # 
+        # This parameter is required.
         self.group_id = group_id
         # The instance ID.
+        # 
+        # This parameter is required.
         self.instance_id = instance_id
         # The number of the page to return. Default value: 1.
         self.page_number = page_number
         # The number of entries to return on each page. Default value: 20. Maximum value: 100.
         self.page_size = page_size
         # The account IDs. A maximum of 100 accounts can be queried.
         self.user_ids = user_ids
@@ -13415,34 +13744,46 @@
             self.user_ids = m.get('UserIds')
         return self
 
 
 class ListUsersForGroupResponseBodyUsers(TeaModel):
     def __init__(
         self,
+        group_member_relation_source_id: str = None,
+        group_member_relation_source_type: str = None,
         user_id: str = None,
     ):
+        self.group_member_relation_source_id = group_member_relation_source_id
+        self.group_member_relation_source_type = group_member_relation_source_type
         # The account ID.
         self.user_id = user_id
 
     def validate(self):
         pass
 
     def to_map(self):
         _map = super().to_map()
         if _map is not None:
             return _map
 
         result = dict()
+        if self.group_member_relation_source_id is not None:
+            result['GroupMemberRelationSourceId'] = self.group_member_relation_source_id
+        if self.group_member_relation_source_type is not None:
+            result['GroupMemberRelationSourceType'] = self.group_member_relation_source_type
         if self.user_id is not None:
             result['UserId'] = self.user_id
         return result
 
     def from_map(self, m: dict = None):
         m = m or dict()
+        if m.get('GroupMemberRelationSourceId') is not None:
+            self.group_member_relation_source_id = m.get('GroupMemberRelationSourceId')
+        if m.get('GroupMemberRelationSourceType') is not None:
+            self.group_member_relation_source_type = m.get('GroupMemberRelationSourceType')
         if m.get('UserId') is not None:
             self.user_id = m.get('UserId')
         return self
 
 
 class ListUsersForGroupResponseBody(TeaModel):
     def __init__(
@@ -13539,18 +13880,24 @@
     def __init__(
         self,
         application_id: str = None,
         instance_id: str = None,
         secret_id: str = None,
     ):
         # The ID of the application whose client key you want to query.
+        # 
+        # This parameter is required.
         self.application_id = application_id
         # The ID of the instance.
+        # 
+        # This parameter is required.
         self.instance_id = instance_id
         # The client key ID of the application.
+        # 
+        # This parameter is required.
         self.secret_id = secret_id
 
     def validate(self):
         pass
 
     def to_map(self):
         _map = super().to_map()
@@ -13732,18 +14079,24 @@
     def __init__(
         self,
         domain_id: str = None,
         domain_proxy_token_id: str = None,
         instance_id: str = None,
     ):
         # 域名ID。
+        # 
+        # This parameter is required.
         self.domain_id = domain_id
         # 域名代理Token ID。
+        # 
+        # This parameter is required.
         self.domain_proxy_token_id = domain_proxy_token_id
         # IDaaS EIAM实例的ID。
+        # 
+        # This parameter is required.
         self.instance_id = instance_id
 
     def validate(self):
         pass
 
     def to_map(self):
         _map = super().to_map()
@@ -13927,18 +14280,24 @@
     def __init__(
         self,
         instance_id: str = None,
         organizational_unit_ids: List[str] = None,
         user_id: str = None,
     ):
         # The instance ID.
+        # 
+        # This parameter is required.
         self.instance_id = instance_id
         # The organization IDs. You can remove an account from a maximum of 100 organizations.
+        # 
+        # This parameter is required.
         self.organizational_unit_ids = organizational_unit_ids
         # The account ID.
+        # 
+        # This parameter is required.
         self.user_id = user_id
 
     def validate(self):
         pass
 
     def to_map(self):
         _map = super().to_map()
@@ -14038,18 +14397,24 @@
     def __init__(
         self,
         group_id: str = None,
         instance_id: str = None,
         user_ids: List[str] = None,
     ):
         # The group ID.
+        # 
+        # This parameter is required.
         self.group_id = group_id
         # The instance ID.
+        # 
+        # This parameter is required.
         self.instance_id = instance_id
         # The account IDs. A maximum of 100 accounts can be removed from a group.
+        # 
+        # This parameter is required.
         self.user_ids = user_ids
 
     def validate(self):
         pass
 
     def to_map(self):
         _map = super().to_map()
@@ -14149,18 +14514,24 @@
     def __init__(
         self,
         application_id: str = None,
         group_ids: List[str] = None,
         instance_id: str = None,
     ):
         # The application ID.
+        # 
+        # This parameter is required.
         self.application_id = application_id
         # The group IDs. You can specify up to 100 group IDs at a time.
+        # 
+        # This parameter is required.
         self.group_ids = group_ids
         # The instance ID.
+        # 
+        # This parameter is required.
         self.instance_id = instance_id
 
     def validate(self):
         pass
 
     def to_map(self):
         _map = super().to_map()
@@ -14260,18 +14631,24 @@
     def __init__(
         self,
         application_id: str = None,
         instance_id: str = None,
         organizational_unit_ids: List[str] = None,
     ):
         # The ID of the application.
+        # 
+        # This parameter is required.
         self.application_id = application_id
         # The ID of the instance.
+        # 
+        # This parameter is required.
         self.instance_id = instance_id
         # The IDs of the organizations. You can revoke the access permissions from a maximum of 100 organizations at a time.
+        # 
+        # This parameter is required.
         self.organizational_unit_ids = organizational_unit_ids
 
     def validate(self):
         pass
 
     def to_map(self):
         _map = super().to_map()
@@ -14371,18 +14748,24 @@
     def __init__(
         self,
         application_id: str = None,
         instance_id: str = None,
         user_ids: List[str] = None,
     ):
         # The ID of the application.
+        # 
+        # This parameter is required.
         self.application_id = application_id
         # The ID of the instance.
+        # 
+        # This parameter is required.
         self.instance_id = instance_id
         # The IDs of the accounts. You can revoke the access permissions from a maximum of 100 accounts at a time.
+        # 
+        # This parameter is required.
         self.user_ids = user_ids
 
     def validate(self):
         pass
 
     def to_map(self):
         _map = super().to_map()
@@ -14482,18 +14865,22 @@
     def __init__(
         self,
         application_id: str = None,
         grant_scopes: List[str] = None,
         instance_id: str = None,
     ):
         # The ID of the application that you want to configure.
+        # 
+        # This parameter is required.
         self.application_id = application_id
         # The permissions of the Developer API feature.
         self.grant_scopes = grant_scopes
         # The ID of the instance.
+        # 
+        # This parameter is required.
         self.instance_id = instance_id
 
     def validate(self):
         pass
 
     def to_map(self):
         _map = super().to_map()
@@ -14816,28 +15203,34 @@
         callback_provisioning_config: SetApplicationProvisioningConfigRequestCallbackProvisioningConfig = None,
         instance_id: str = None,
         provision_password: bool = None,
         provision_protocol_type: str = None,
         scim_provisioning_config: SetApplicationProvisioningConfigRequestScimProvisioningConfig = None,
     ):
         # The ID of the application.
+        # 
+        # This parameter is required.
         self.application_id = application_id
         # The configuration of event callback synchronization. This parameter is required when the ProvisionProtocolType parameter is set to idaas_callback.
         self.callback_provisioning_config = callback_provisioning_config
         # The ID of the instance.
+        # 
+        # This parameter is required.
         self.instance_id = instance_id
         # Specifies whether to synchronize the password in IDaaS user event callbacks. Valid values:
         # 
         # *   true: synchronize the password.
         # *   false: do not synchronize the password.
         self.provision_password = provision_password
         # The synchronization protocol type of the application. Valid values:
         # 
         # *   idaas_callback: custom event callback protocol of IDaaS.
         # *   scim2: System for Cross-domain Identity Management (SCIM) protocol.
+        # 
+        # This parameter is required.
         self.provision_protocol_type = provision_protocol_type
         # The configuration of SCIM-based IDaaS synchronization. This parameter is required when the ProvisionProtocolType parameter is set to scim2.
         self.scim_provisioning_config = scim_provisioning_config
 
     def validate(self):
         if self.callback_provisioning_config:
             self.callback_provisioning_config.validate()
@@ -14952,20 +15345,27 @@
         return self
 
 
 class SetApplicationProvisioningScopeRequest(TeaModel):
     def __init__(
         self,
         application_id: str = None,
+        group_ids: List[str] = None,
         instance_id: str = None,
         organizational_unit_ids: List[str] = None,
     ):
         # The ID of the application.
+        # 
+        # This parameter is required.
         self.application_id = application_id
+        # 授权同步出的组列表
+        self.group_ids = group_ids
         # The ID of the instance.
+        # 
+        # This parameter is required.
         self.instance_id = instance_id
         # The list of organizational units that are authorized for account synchronization.
         self.organizational_unit_ids = organizational_unit_ids
 
     def validate(self):
         pass
 
@@ -14973,24 +15373,28 @@
         _map = super().to_map()
         if _map is not None:
             return _map
 
         result = dict()
         if self.application_id is not None:
             result['ApplicationId'] = self.application_id
+        if self.group_ids is not None:
+            result['GroupIds'] = self.group_ids
         if self.instance_id is not None:
             result['InstanceId'] = self.instance_id
         if self.organizational_unit_ids is not None:
             result['OrganizationalUnitIds'] = self.organizational_unit_ids
         return result
 
     def from_map(self, m: dict = None):
         m = m or dict()
         if m.get('ApplicationId') is not None:
             self.application_id = m.get('ApplicationId')
+        if m.get('GroupIds') is not None:
+            self.group_ids = m.get('GroupIds')
         if m.get('InstanceId') is not None:
             self.instance_id = m.get('InstanceId')
         if m.get('OrganizationalUnitIds') is not None:
             self.organizational_unit_ids = m.get('OrganizationalUnitIds')
         return self
 
 
@@ -15371,23 +15775,27 @@
         init_login_type: str = None,
         init_login_url: str = None,
         instance_id: str = None,
         oidc_sso_config: SetApplicationSsoConfigRequestOidcSsoConfig = None,
         saml_sso_config: SetApplicationSsoConfigRequestSamlSsoConfig = None,
     ):
         # The ID of the application.
+        # 
+        # This parameter is required.
         self.application_id = application_id
         # The initial SSO method. Valid values:
         # 
         # *   only_app_init_sso: Only application-initiated SSO is allowed. This method is selected by default when the SSO protocol of the application is an OIDC protocol. If this method is selected when the SSO protocol of the application is SAML, the InitLoginUrl parameter is required.
         # *   idaas_or_app_init_sso: IDaaS-initiated SSO and application-initiated SSO are allowed. This method is selected by default when the SSO protocol of the application is SAML. If this method is selected when the SSO protocol of the application is an OIDC protocol, the InitLoginUrl parameter is required.
         self.init_login_type = init_login_type
         # The initial webhook URL of SSO. This parameter is required when the SSO protocol of the application is an OIDC protocol and the InitLoginType parameters is set to idaas_or_app_init_sso or when the SSO protocol of the application is SAML and the InitLoginType parameter is set to only_app_init_sso.
         self.init_login_url = init_login_url
         # The ID of the instance.
+        # 
+        # This parameter is required.
         self.instance_id = instance_id
         # The Open ID Connect (OIDC)-based SSO configuration attributes of the application.
         self.oidc_sso_config = oidc_sso_config
         # The Security Assertion Markup Language (SAML)-based SSO configuration attributes of the application.
         self.saml_sso_config = saml_sso_config
 
     def validate(self):
@@ -15507,16 +15915,20 @@
 class SetDefaultDomainRequest(TeaModel):
     def __init__(
         self,
         domain_id: str = None,
         instance_id: str = None,
     ):
         # 域名ID。
+        # 
+        # This parameter is required.
         self.domain_id = domain_id
         # IDaaS EIAM实例的ID。
+        # 
+        # This parameter is required.
         self.instance_id = instance_id
 
     def validate(self):
         pass
 
     def to_map(self):
         _map = super().to_map()
@@ -15613,16 +16025,20 @@
         authentication_channels: List[str] = None,
         forget_password_status: str = None,
         instance_id: str = None,
     ):
         # 身份认证渠道。枚举取值:email(邮件)、sms(短信)
         self.authentication_channels = authentication_channels
         # 忘记密码配置状态。枚举取值:enabled(开启)、disabled(禁用)
+        # 
+        # This parameter is required.
         self.forget_password_status = forget_password_status
         # The instance ID.
+        # 
+        # This parameter is required.
         self.instance_id = instance_id
 
     def validate(self):
         pass
 
     def to_map(self):
         _map = super().to_map()
@@ -15723,15 +16139,15 @@
         self,
         password_check_type: str = None,
     ):
         # The type of the password check. Valid values:
         # 
         # *   inclusion_upper_case: The password must contain uppercase letters.
         # *   inclusion_lower_case: The password must contain lowercase letters.
-        # *   inclusion_special_case: The password must contain one or more of the following special characters: @ % + \ / \" ! # $ ^ ? : , ( ) { } \[ ] ~ - \_ .
+        # *   inclusion_special_case: The password must contain one or more of the following special characters: @ % + \\ / \\" ! # $ ^ ? : , ( ) { } [ ] ~ - _ .
         # *   inclusion_number: The password must contain digits.
         # *   exclusion_username: The password cannot contain a username.
         # *   exclusion_email: The password cannot contain an email prefix.
         # *   exclusion_phone_number: The password cannot contain a mobile number.
         # *   exclusion_display_name: The password cannot contain a display name.
         self.password_check_type = password_check_type
 
@@ -15759,18 +16175,22 @@
     def __init__(
         self,
         instance_id: str = None,
         password_complexity_rules: List[SetPasswordComplexityConfigurationRequestPasswordComplexityRules] = None,
         password_min_length: int = None,
     ):
         # The instance ID.
+        # 
+        # This parameter is required.
         self.instance_id = instance_id
         # The password complexity rules.
         self.password_complexity_rules = password_complexity_rules
         # The minimum number of characters in a password.
+        # 
+        # This parameter is required.
         self.password_min_length = password_min_length
 
     def validate(self):
         if self.password_complexity_rules:
             for k in self.password_complexity_rules:
                 if k:
                     k.validate()
@@ -15883,14 +16303,16 @@
         password_expiration_notification_duration: int = None,
         password_expiration_notification_status: str = None,
         password_expiration_status: str = None,
         password_forced_update_duration: int = None,
         password_valid_max_day: int = None,
     ):
         # The instance ID.
+        # 
+        # This parameter is required.
         self.instance_id = instance_id
         # The action to take upon password expiration. This parameter must be specified when PasswordExpirationStatus is set to enabled. Valid values:
         # 
         # *   forbid_login: Users cannot log on to IDaaS.
         # *   force_update_password: Users must change the password.
         # *   remind_update_password: IDaaS reminds users to change the password upon each logon.
         self.password_expiration_action = password_expiration_action
@@ -15903,14 +16325,16 @@
         # *   enabled
         # *   disabled
         self.password_expiration_notification_status = password_expiration_notification_status
         # Specifies whether to enable the password expiration feature. Valid values:
         # 
         # *   enabled
         # *   disabled
+        # 
+        # This parameter is required.
         self.password_expiration_status = password_expiration_status
         # The number of days before which users must change the password to prevent password expiration. Unit: day. You must set this parameter to a value greater than the value of PasswordExpirationNotificationDuration.
         self.password_forced_update_duration = password_forced_update_duration
         # The validity period of a password. Unit: day. This parameter must be specified when PasswordExpirationStatus is set to enabled.
         self.password_valid_max_day = password_valid_max_day
 
     def validate(self):
@@ -16034,21 +16458,25 @@
     def __init__(
         self,
         instance_id: str = None,
         password_history_max_retention: int = None,
         password_history_status: str = None,
     ):
         # The instance ID.
+        # 
+        # This parameter is required.
         self.instance_id = instance_id
         # The maximum number of recent passwords that can be retained. This parameter must be specified when PasswordHistoryStatus is set to enabled.
         self.password_history_max_retention = password_history_max_retention
         # Specifies whether to enable the password history feature. Valid values:
         # 
         # *   enabled
         # *   disabled
+        # 
+        # This parameter is required.
         self.password_history_status = password_history_status
 
     def validate(self):
         pass
 
     def to_map(self):
         _map = super().to_map()
@@ -16150,26 +16578,30 @@
         instance_id: str = None,
         password_forced_update_status: str = None,
         password_initialization_notification_channels: List[str] = None,
         password_initialization_status: str = None,
         password_initialization_type: str = None,
     ):
         # The ID of the instance.
+        # 
+        # This parameter is required.
         self.instance_id = instance_id
         # Specifies whether to enable forcible password change upon first logon. Valid values:
         # 
         # *   enabled
         # *   disabled
         self.password_forced_update_status = password_forced_update_status
         # The methods for receiving password initialization notifications.
         self.password_initialization_notification_channels = password_initialization_notification_channels
         # Specifies whether to enable password initialization. Valid values:
         # 
         # *   enabled
         # *   disabled
+        # 
+        # This parameter is required.
         self.password_initialization_status = password_initialization_status
         # The password initialization method. This parameter is required when PasswordInitializationStatus is set to enabled. Set the value to random.
         # 
         # *   random: A randomly generated password is used.
         self.password_initialization_type = password_initialization_type
 
     def validate(self):
@@ -16281,18 +16713,24 @@
     def __init__(
         self,
         instance_id: str = None,
         organizational_unit_id: str = None,
         user_id: str = None,
     ):
         # The instance ID.
+        # 
+        # This parameter is required.
         self.instance_id = instance_id
         # The ID of the new primary organizational unit.
+        # 
+        # This parameter is required.
         self.organizational_unit_id = organizational_unit_id
         # The ID of the account.
+        # 
+        # This parameter is required.
         self.user_id = user_id
 
     def validate(self):
         pass
 
     def to_map(self):
         _map = super().to_map()
@@ -16391,16 +16829,20 @@
 class UnlockUserRequest(TeaModel):
     def __init__(
         self,
         instance_id: str = None,
         user_id: str = None,
     ):
         # The instance ID.
+        # 
+        # This parameter is required.
         self.instance_id = instance_id
         # The account ID.
+        # 
+        # This parameter is required.
         self.user_id = user_id
 
     def validate(self):
         pass
 
     def to_map(self):
         _map = super().to_map()
@@ -16496,21 +16938,27 @@
     def __init__(
         self,
         application_id: str = None,
         authorization_type: str = None,
         instance_id: str = None,
     ):
         # The ID of the application that you want to modify.
+        # 
+        # This parameter is required.
         self.application_id = application_id
         # The authorization type of the application. Valid values:
         # 
         # *   authorize_required: Only the user with explicit authorization can access the application.
         # *   default_all: By default, all users can access the application.
+        # 
+        # This parameter is required.
         self.authorization_type = authorization_type
         # The ID of the instance.
+        # 
+        # This parameter is required.
         self.instance_id = instance_id
 
     def validate(self):
         pass
 
     def to_map(self):
         _map = super().to_map()
@@ -16610,18 +17058,22 @@
     def __init__(
         self,
         application_id: str = None,
         description: str = None,
         instance_id: str = None,
     ):
         # The ID of the application that you want to modify.
+        # 
+        # This parameter is required.
         self.application_id = application_id
         # The description of the application.
         self.description = description
         # The ID of the instance.
+        # 
+        # This parameter is required.
         self.instance_id = instance_id
 
     def validate(self):
         pass
 
     def to_map(self):
         _map = super().to_map()
@@ -16724,18 +17176,22 @@
         group_id: str = None,
         group_name: str = None,
         instance_id: str = None,
     ):
         # The external ID of the group.
         self.group_external_id = group_external_id
         # The group ID.
+        # 
+        # This parameter is required.
         self.group_id = group_id
         # The name of the group.
         self.group_name = group_name
         # The instance ID.
+        # 
+        # This parameter is required.
         self.instance_id = instance_id
 
     def validate(self):
         pass
 
     def to_map(self):
         _map = super().to_map()
@@ -16841,16 +17297,20 @@
         description: str = None,
         group_id: str = None,
         instance_id: str = None,
     ):
         # The description of the account group. The value can be up to 256 characters in length.
         self.description = description
         # The ID of the account group.
+        # 
+        # This parameter is required.
         self.group_id = group_id
         # The instance ID.
+        # 
+        # This parameter is required.
         self.instance_id = instance_id
 
     def validate(self):
         pass
 
     def to_map(self):
         _map = super().to_map()
@@ -16951,14 +17411,16 @@
         self,
         description: str = None,
         instance_id: str = None,
     ):
         # The new description of the instance.
         self.description = description
         # The ID of the instance whose description you want to modify.
+        # 
+        # This parameter is required.
         self.instance_id = instance_id
 
     def validate(self):
         pass
 
     def to_map(self):
         _map = super().to_map()
@@ -17054,18 +17516,24 @@
     def __init__(
         self,
         instance_id: str = None,
         network_access_endpoint_id: str = None,
         network_access_endpoint_name: str = None,
     ):
         # IDaaS EIAM实例的ID。
+        # 
+        # This parameter is required.
         self.instance_id = instance_id
         # 专属网络端点ID。
+        # 
+        # This parameter is required.
         self.network_access_endpoint_id = network_access_endpoint_id
         # 专属网络端点名称。
+        # 
+        # This parameter is required.
         self.network_access_endpoint_name = network_access_endpoint_name
 
     def validate(self):
         pass
 
     def to_map(self):
         _map = super().to_map()
@@ -17164,16 +17632,20 @@
     def __init__(
         self,
         instance_id: str = None,
         organizational_unit_id: str = None,
         organizational_unit_name: str = None,
     ):
         # The instance ID.
+        # 
+        # This parameter is required.
         self.instance_id = instance_id
         # The organization ID.
+        # 
+        # This parameter is required.
         self.organizational_unit_id = organizational_unit_id
         # The name of the organization. The name can be up to 64 characters in length and must be unique in the same parent organization.
         self.organizational_unit_name = organizational_unit_name
 
     def validate(self):
         pass
 
@@ -17277,16 +17749,20 @@
         description: str = None,
         instance_id: str = None,
         organizational_unit_id: str = None,
     ):
         # The description of the organization. The value can be up to 256 characters in length.
         self.description = description
         # The instance ID.
+        # 
+        # This parameter is required.
         self.instance_id = instance_id
         # The organization ID.
+        # 
+        # This parameter is required.
         self.organizational_unit_id = organizational_unit_id
 
     def validate(self):
         pass
 
     def to_map(self):
         _map = super().to_map()
@@ -17386,18 +17862,24 @@
     def __init__(
         self,
         instance_id: str = None,
         organizational_unit_id: str = None,
         parent_id: str = None,
     ):
         # The instance ID.
+        # 
+        # This parameter is required.
         self.instance_id = instance_id
         # The organization ID.
+        # 
+        # This parameter is required.
         self.organizational_unit_id = organizational_unit_id
         # The parent organization ID.
+        # 
+        # This parameter is required.
         self.parent_id = parent_id
 
     def validate(self):
         pass
 
     def to_map(self):
         _map = super().to_map()
@@ -17553,29 +18035,33 @@
         user_id: str = None,
         username: str = None,
     ):
         # The custom extended fields.
         self.custom_fields = custom_fields
         # The display name of the account. The display name can be up to 64 characters in length.
         self.display_name = display_name
-        # The email address. The prefix of the email address can contain letters, digits, periods (.), underscores (\_), and hyphens (-).
+        # The email address. The prefix of the email address can contain letters, digits, periods (.), underscores (_), and hyphens (-).
         self.email = email
         # Specifies whether the email address is verified. This parameter must be specified if you specify Email. You can set this parameter to true if you have no special business requirements.
         self.email_verified = email_verified
         # The instance ID.
+        # 
+        # This parameter is required.
         self.instance_id = instance_id
         # The mobile number. The mobile number must be 6 to 15 digits in length.
         self.phone_number = phone_number
         # Specifies whether the mobile number is verified. This parameter must be specified if you specify PhoneNumber. You can set this parameter to true if you have no special business requirements.
         self.phone_number_verified = phone_number_verified
         # The area code of the mobile number. For example, the area code of a mobile number in the Chinese mainland is 86 without 00 or the plus sign (+). This parameter must be specified if you specify PhoneNumber.
         self.phone_region = phone_region
         # The account ID.
+        # 
+        # This parameter is required.
         self.user_id = user_id
-        # The name of the account. The name can be up to 64 characters in length. It can contain letters, digits, and the following special characters: \_ . @ -\
+        # The name of the account. The name can be up to 64 characters in length. It can contain letters, digits, and the following special characters: _ . @ -\
         self.username = username
 
     def validate(self):
         if self.custom_fields:
             for k in self.custom_fields:
                 if k:
                     k.validate()
@@ -17713,16 +18199,20 @@
         description: str = None,
         instance_id: str = None,
         user_id: str = None,
     ):
         # The description of the account. The value can be up to 256 characters in length.
         self.description = description
         # The ID of the instance.
+        # 
+        # This parameter is required.
         self.instance_id = instance_id
         # The ID of the account.
+        # 
+        # This parameter is required.
         self.user_id = user_id
 
     def validate(self):
         pass
 
     def to_map(self):
         _map = super().to_map()
@@ -17824,23 +18314,29 @@
         instance_id: str = None,
         password: str = None,
         password_forced_update_status: str = None,
         user_id: str = None,
         user_notification_channels: List[str] = None,
     ):
         # The instance ID.
+        # 
+        # This parameter is required.
         self.instance_id = instance_id
         # The new password of the account. For more information about the password format, see the "Password Policies" topic.
+        # 
+        # This parameter is required.
         self.password = password
         # Specifies whether to enable forcible password change upon first logon. Default value: disabled. Valid values:
         # 
         # *   enabled
         # *   disabled
         self.password_forced_update_status = password_forced_update_status
         # The account ID.
+        # 
+        # This parameter is required.
         self.user_id = user_id
         # The methods for receiving password notifications.
         self.user_notification_channels = user_notification_channels
 
     def validate(self):
         pass
```

### Comparing `alibabacloud_eiam20211201-1.3.2/alibabacloud_eiam20211201.egg-info/PKG-INFO` & `alibabacloud_eiam20211201-1.3.3/alibabacloud_eiam20211201.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: alibabacloud-eiam20211201
-Version: 1.3.2
+Version: 1.3.3
 Summary: Alibaba Cloud Eiam (20211201) SDK Library for Python
 Home-page: https://github.com/aliyun/alibabacloud-python-sdk
 Author: Alibaba Cloud SDK
 Author-email: sdk-team@alibabacloud.com
 License: Apache License 2.0
 Description: English | [简体中文](README-CN.md)
         ![](https://aliyunsdk-pages.alicdn.com/icons/AlibabaCloud.svg)
```

### Comparing `alibabacloud_eiam20211201-1.3.2/setup.py` & `alibabacloud_eiam20211201-1.3.3/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -20,29 +20,29 @@
 
 import os
 from setuptools import setup, find_packages
 
 """
 setup module for alibabacloud_eiam20211201.
 
-Created on 12/03/2024
+Created on 29/05/2024
 
 @author: Alibaba Cloud SDK
 """
 
 PACKAGE = "alibabacloud_eiam20211201"
 NAME = "alibabacloud_eiam20211201" or "alibabacloud-package"
 DESCRIPTION = "Alibaba Cloud Eiam (20211201) SDK Library for Python"
 AUTHOR = "Alibaba Cloud SDK"
 AUTHOR_EMAIL = "sdk-team@alibabacloud.com"
 URL = "https://github.com/aliyun/alibabacloud-python-sdk"
 VERSION = __import__(PACKAGE).__version__
 REQUIRES = [
-    "alibabacloud_tea_util>=0.3.11, <1.0.0",
-    "alibabacloud_tea_openapi>=0.3.8, <1.0.0",
+    "alibabacloud_tea_util>=0.3.12, <1.0.0",
+    "alibabacloud_tea_openapi>=0.3.9, <1.0.0",
     "alibabacloud_openapi_util>=0.2.1, <1.0.0",
     "alibabacloud_endpoint_util>=0.0.3, <1.0.0"
 ]
 
 LONG_DESCRIPTION = ''
 if os.path.exists('./README.md'):
     with open("README.md", encoding='utf-8') as fp:
```

