# Comparing `tmp/alibabacloud_intelligentcreation20240313-1.0.0.tar.gz` & `tmp/alibabacloud_intelligentcreation20240313-2.0.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/alibabacloud_intelligentcreation20240313-1.0.0.tar", last modified: Mon May 20 10:54:56 2024, max compression
+gzip compressed data, was "dist/alibabacloud_intelligentcreation20240313-2.0.0.tar", last modified: Wed May 29 05:39:01 2024, max compression
```

## Comparing `alibabacloud_intelligentcreation20240313-1.0.0.tar` & `alibabacloud_intelligentcreation20240313-2.0.0.tar`

### file list

```diff
@@ -1,18 +1,19 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-20 10:54:56.000000 alibabacloud_intelligentcreation20240313-1.0.0/
--rw-r--r--   0 root         (0) root         (0)      600 2024-05-20 10:54:56.000000 alibabacloud_intelligentcreation20240313-1.0.0/LICENSE
--rw-r--r--   0 root         (0) root         (0)       29 2024-05-20 10:54:56.000000 alibabacloud_intelligentcreation20240313-1.0.0/MANIFEST.in
--rw-r--r--   0 root         (0) root         (0)     2513 2024-05-20 10:54:56.000000 alibabacloud_intelligentcreation20240313-1.0.0/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)     1159 2024-05-20 10:54:56.000000 alibabacloud_intelligentcreation20240313-1.0.0/README-CN.md
--rw-r--r--   0 root         (0) root         (0)     1244 2024-05-20 10:54:56.000000 alibabacloud_intelligentcreation20240313-1.0.0/README.md
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-20 10:54:56.000000 alibabacloud_intelligentcreation20240313-1.0.0/alibabacloud_intelligentcreation20240313/
--rw-r--r--   0 root         (0) root         (0)       21 2024-05-20 10:54:56.000000 alibabacloud_intelligentcreation20240313-1.0.0/alibabacloud_intelligentcreation20240313/__init__.py
--rw-r--r--   0 root         (0) root         (0)    28534 2024-05-20 10:54:56.000000 alibabacloud_intelligentcreation20240313-1.0.0/alibabacloud_intelligentcreation20240313/client.py
--rw-r--r--   0 root         (0) root         (0)    38821 2024-05-20 10:54:56.000000 alibabacloud_intelligentcreation20240313-1.0.0/alibabacloud_intelligentcreation20240313/models.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-20 10:54:56.000000 alibabacloud_intelligentcreation20240313-1.0.0/alibabacloud_intelligentcreation20240313.egg-info/
--rw-r--r--   0 root         (0) root         (0)     2513 2024-05-20 10:54:56.000000 alibabacloud_intelligentcreation20240313-1.0.0/alibabacloud_intelligentcreation20240313.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)      535 2024-05-20 10:54:56.000000 alibabacloud_intelligentcreation20240313-1.0.0/alibabacloud_intelligentcreation20240313.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2024-05-20 10:54:56.000000 alibabacloud_intelligentcreation20240313-1.0.0/alibabacloud_intelligentcreation20240313.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)      157 2024-05-20 10:54:56.000000 alibabacloud_intelligentcreation20240313-1.0.0/alibabacloud_intelligentcreation20240313.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)       41 2024-05-20 10:54:56.000000 alibabacloud_intelligentcreation20240313-1.0.0/alibabacloud_intelligentcreation20240313.egg-info/top_level.txt
--rw-r--r--   0 root         (0) root         (0)       73 2024-05-20 10:54:56.000000 alibabacloud_intelligentcreation20240313-1.0.0/setup.cfg
--rw-r--r--   0 root         (0) root         (0)     2691 2024-05-20 10:54:56.000000 alibabacloud_intelligentcreation20240313-1.0.0/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-29 05:39:01.000000 alibabacloud_intelligentcreation20240313-2.0.0/
+-rw-r--r--   0 root         (0) root         (0)       82 2024-05-29 05:39:01.000000 alibabacloud_intelligentcreation20240313-2.0.0/ChangeLog.md
+-rw-r--r--   0 root         (0) root         (0)      600 2024-05-29 05:39:01.000000 alibabacloud_intelligentcreation20240313-2.0.0/LICENSE
+-rw-r--r--   0 root         (0) root         (0)       29 2024-05-29 05:39:01.000000 alibabacloud_intelligentcreation20240313-2.0.0/MANIFEST.in
+-rw-r--r--   0 root         (0) root         (0)     2513 2024-05-29 05:39:01.000000 alibabacloud_intelligentcreation20240313-2.0.0/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)     1159 2024-05-29 05:39:01.000000 alibabacloud_intelligentcreation20240313-2.0.0/README-CN.md
+-rw-r--r--   0 root         (0) root         (0)     1244 2024-05-29 05:39:01.000000 alibabacloud_intelligentcreation20240313-2.0.0/README.md
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-29 05:39:01.000000 alibabacloud_intelligentcreation20240313-2.0.0/alibabacloud_intelligentcreation20240313/
+-rw-r--r--   0 root         (0) root         (0)       21 2024-05-29 05:39:01.000000 alibabacloud_intelligentcreation20240313-2.0.0/alibabacloud_intelligentcreation20240313/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    34470 2024-05-29 05:39:01.000000 alibabacloud_intelligentcreation20240313-2.0.0/alibabacloud_intelligentcreation20240313/client.py
+-rw-r--r--   0 root         (0) root         (0)    45460 2024-05-29 05:39:01.000000 alibabacloud_intelligentcreation20240313-2.0.0/alibabacloud_intelligentcreation20240313/models.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-29 05:39:01.000000 alibabacloud_intelligentcreation20240313-2.0.0/alibabacloud_intelligentcreation20240313.egg-info/
+-rw-r--r--   0 root         (0) root         (0)     2513 2024-05-29 05:39:01.000000 alibabacloud_intelligentcreation20240313-2.0.0/alibabacloud_intelligentcreation20240313.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)      548 2024-05-29 05:39:01.000000 alibabacloud_intelligentcreation20240313-2.0.0/alibabacloud_intelligentcreation20240313.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2024-05-29 05:39:01.000000 alibabacloud_intelligentcreation20240313-2.0.0/alibabacloud_intelligentcreation20240313.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)      157 2024-05-29 05:39:01.000000 alibabacloud_intelligentcreation20240313-2.0.0/alibabacloud_intelligentcreation20240313.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)       41 2024-05-29 05:39:01.000000 alibabacloud_intelligentcreation20240313-2.0.0/alibabacloud_intelligentcreation20240313.egg-info/top_level.txt
+-rw-r--r--   0 root         (0) root         (0)       73 2024-05-29 05:39:01.000000 alibabacloud_intelligentcreation20240313-2.0.0/setup.cfg
+-rw-r--r--   0 root         (0) root         (0)     2691 2024-05-29 05:39:01.000000 alibabacloud_intelligentcreation20240313-2.0.0/setup.py
```

### Comparing `alibabacloud_intelligentcreation20240313-1.0.0/LICENSE` & `alibabacloud_intelligentcreation20240313-2.0.0/LICENSE`

 * *Files identical despite different names*

### Comparing `alibabacloud_intelligentcreation20240313-1.0.0/PKG-INFO` & `alibabacloud_intelligentcreation20240313-2.0.0/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: alibabacloud_intelligentcreation20240313
-Version: 1.0.0
+Version: 2.0.0
 Summary: Alibaba Cloud IntelligentCreation (20240313) SDK Library for Python
 Home-page: https://github.com/aliyun/alibabacloud-python-sdk
 Author: Alibaba Cloud SDK
 Author-email: sdk-team@alibabacloud.com
 License: Apache License 2.0
 Description: English | [简体中文](README-CN.md)
         ![](https://aliyunsdk-pages.alicdn.com/icons/AlibabaCloud.svg)
```

### Comparing `alibabacloud_intelligentcreation20240313-1.0.0/README-CN.md` & `alibabacloud_intelligentcreation20240313-2.0.0/README-CN.md`

 * *Files identical despite different names*

### Comparing `alibabacloud_intelligentcreation20240313-1.0.0/README.md` & `alibabacloud_intelligentcreation20240313-2.0.0/README.md`

 * *Files identical despite different names*

### Comparing `alibabacloud_intelligentcreation20240313-1.0.0/alibabacloud_intelligentcreation20240313/client.py` & `alibabacloud_intelligentcreation20240313-2.0.0/alibabacloud_intelligentcreation20240313/client.py`

 * *Files 10% similar despite different names*

```diff
@@ -715,26 +715,33 @@
         """
         runtime = util_models.RuntimeOptions()
         headers = {}
         return await self.get_text_task_with_options_async(text_task_id, headers, runtime)
 
     def list_text_themes_with_options(
         self,
+        request: intelligent_creation_20240313_models.ListTextThemesRequest,
         headers: Dict[str, str],
         runtime: util_models.RuntimeOptions,
     ) -> intelligent_creation_20240313_models.ListTextThemesResponse:
         """
         @summary 查询文案主题列表
         
+        @param request: ListTextThemesRequest
         @param headers: map
         @param runtime: runtime options for this request RuntimeOptions
         @return: ListTextThemesResponse
         """
+        UtilClient.validate_model(request)
+        query = {}
+        if not UtilClient.is_unset(request.industry):
+            query['industry'] = request.industry
         req = open_api_models.OpenApiRequest(
-            headers=headers
+            headers=headers,
+            query=OpenApiUtilClient.query(query)
         )
         params = open_api_models.Params(
             action='ListTextThemes',
             version='2024-03-13',
             protocol='HTTPS',
             pathname=f'/yic/yic-console/openService/v1/textThemes',
             method='GET',
@@ -746,26 +753,33 @@
         return TeaCore.from_map(
             intelligent_creation_20240313_models.ListTextThemesResponse(),
             self.call_api(params, req, runtime)
         )
 
     async def list_text_themes_with_options_async(
         self,
+        request: intelligent_creation_20240313_models.ListTextThemesRequest,
         headers: Dict[str, str],
         runtime: util_models.RuntimeOptions,
     ) -> intelligent_creation_20240313_models.ListTextThemesResponse:
         """
         @summary 查询文案主题列表
         
+        @param request: ListTextThemesRequest
         @param headers: map
         @param runtime: runtime options for this request RuntimeOptions
         @return: ListTextThemesResponse
         """
+        UtilClient.validate_model(request)
+        query = {}
+        if not UtilClient.is_unset(request.industry):
+            query['industry'] = request.industry
         req = open_api_models.OpenApiRequest(
-            headers=headers
+            headers=headers,
+            query=OpenApiUtilClient.query(query)
         )
         params = open_api_models.Params(
             action='ListTextThemes',
             version='2024-03-13',
             protocol='HTTPS',
             pathname=f'/yic/yic-console/openService/v1/textThemes',
             method='GET',
@@ -775,26 +789,162 @@
             body_type='json'
         )
         return TeaCore.from_map(
             intelligent_creation_20240313_models.ListTextThemesResponse(),
             await self.call_api_async(params, req, runtime)
         )
 
-    def list_text_themes(self) -> intelligent_creation_20240313_models.ListTextThemesResponse:
+    def list_text_themes(
+        self,
+        request: intelligent_creation_20240313_models.ListTextThemesRequest,
+    ) -> intelligent_creation_20240313_models.ListTextThemesResponse:
         """
         @summary 查询文案主题列表
         
+        @param request: ListTextThemesRequest
         @return: ListTextThemesResponse
         """
         runtime = util_models.RuntimeOptions()
         headers = {}
-        return self.list_text_themes_with_options(headers, runtime)
+        return self.list_text_themes_with_options(request, headers, runtime)
 
-    async def list_text_themes_async(self) -> intelligent_creation_20240313_models.ListTextThemesResponse:
+    async def list_text_themes_async(
+        self,
+        request: intelligent_creation_20240313_models.ListTextThemesRequest,
+    ) -> intelligent_creation_20240313_models.ListTextThemesResponse:
         """
         @summary 查询文案主题列表
         
+        @param request: ListTextThemesRequest
         @return: ListTextThemesResponse
         """
         runtime = util_models.RuntimeOptions()
         headers = {}
-        return await self.list_text_themes_with_options_async(headers, runtime)
+        return await self.list_text_themes_with_options_async(request, headers, runtime)
+
+    def list_texts_with_options(
+        self,
+        request: intelligent_creation_20240313_models.ListTextsRequest,
+        headers: Dict[str, str],
+        runtime: util_models.RuntimeOptions,
+    ) -> intelligent_creation_20240313_models.ListTextsResponse:
+        """
+        @summary 列举文案
+        
+        @param request: ListTextsRequest
+        @param headers: map
+        @param runtime: runtime options for this request RuntimeOptions
+        @return: ListTextsResponse
+        """
+        UtilClient.validate_model(request)
+        query = {}
+        if not UtilClient.is_unset(request.generation_source):
+            query['generationSource'] = request.generation_source
+        if not UtilClient.is_unset(request.industry):
+            query['industry'] = request.industry
+        if not UtilClient.is_unset(request.page_number):
+            query['pageNumber'] = request.page_number
+        if not UtilClient.is_unset(request.page_size):
+            query['pageSize'] = request.page_size
+        if not UtilClient.is_unset(request.publish_status):
+            query['publishStatus'] = request.publish_status
+        if not UtilClient.is_unset(request.text_style_type):
+            query['textStyleType'] = request.text_style_type
+        if not UtilClient.is_unset(request.text_theme):
+            query['textTheme'] = request.text_theme
+        req = open_api_models.OpenApiRequest(
+            headers=headers,
+            query=OpenApiUtilClient.query(query)
+        )
+        params = open_api_models.Params(
+            action='ListTexts',
+            version='2024-03-13',
+            protocol='HTTPS',
+            pathname=f'/yic/yic-console/openService/v1/texts',
+            method='GET',
+            auth_type='AK',
+            style='ROA',
+            req_body_type='json',
+            body_type='json'
+        )
+        return TeaCore.from_map(
+            intelligent_creation_20240313_models.ListTextsResponse(),
+            self.call_api(params, req, runtime)
+        )
+
+    async def list_texts_with_options_async(
+        self,
+        request: intelligent_creation_20240313_models.ListTextsRequest,
+        headers: Dict[str, str],
+        runtime: util_models.RuntimeOptions,
+    ) -> intelligent_creation_20240313_models.ListTextsResponse:
+        """
+        @summary 列举文案
+        
+        @param request: ListTextsRequest
+        @param headers: map
+        @param runtime: runtime options for this request RuntimeOptions
+        @return: ListTextsResponse
+        """
+        UtilClient.validate_model(request)
+        query = {}
+        if not UtilClient.is_unset(request.generation_source):
+            query['generationSource'] = request.generation_source
+        if not UtilClient.is_unset(request.industry):
+            query['industry'] = request.industry
+        if not UtilClient.is_unset(request.page_number):
+            query['pageNumber'] = request.page_number
+        if not UtilClient.is_unset(request.page_size):
+            query['pageSize'] = request.page_size
+        if not UtilClient.is_unset(request.publish_status):
+            query['publishStatus'] = request.publish_status
+        if not UtilClient.is_unset(request.text_style_type):
+            query['textStyleType'] = request.text_style_type
+        if not UtilClient.is_unset(request.text_theme):
+            query['textTheme'] = request.text_theme
+        req = open_api_models.OpenApiRequest(
+            headers=headers,
+            query=OpenApiUtilClient.query(query)
+        )
+        params = open_api_models.Params(
+            action='ListTexts',
+            version='2024-03-13',
+            protocol='HTTPS',
+            pathname=f'/yic/yic-console/openService/v1/texts',
+            method='GET',
+            auth_type='AK',
+            style='ROA',
+            req_body_type='json',
+            body_type='json'
+        )
+        return TeaCore.from_map(
+            intelligent_creation_20240313_models.ListTextsResponse(),
+            await self.call_api_async(params, req, runtime)
+        )
+
+    def list_texts(
+        self,
+        request: intelligent_creation_20240313_models.ListTextsRequest,
+    ) -> intelligent_creation_20240313_models.ListTextsResponse:
+        """
+        @summary 列举文案
+        
+        @param request: ListTextsRequest
+        @return: ListTextsResponse
+        """
+        runtime = util_models.RuntimeOptions()
+        headers = {}
+        return self.list_texts_with_options(request, headers, runtime)
+
+    async def list_texts_async(
+        self,
+        request: intelligent_creation_20240313_models.ListTextsRequest,
+    ) -> intelligent_creation_20240313_models.ListTextsResponse:
+        """
+        @summary 列举文案
+        
+        @param request: ListTextsRequest
+        @return: ListTextsResponse
+        """
+        runtime = util_models.RuntimeOptions()
+        headers = {}
+        return await self.list_texts_with_options_async(request, headers, runtime)
```

### Comparing `alibabacloud_intelligentcreation20240313-1.0.0/alibabacloud_intelligentcreation20240313/models.py` & `alibabacloud_intelligentcreation20240313-2.0.0/alibabacloud_intelligentcreation20240313/models.py`

 * *Files 9% similar despite different names*

```diff
@@ -361,38 +361,44 @@
 class Text(TeaModel):
     def __init__(
         self,
         desc: str = None,
         gmt_create: str = None,
         gmt_modified: str = None,
         illustration_task_id_list: List[int] = None,
+        publish_status: str = None,
         text_content: str = None,
         text_id: int = None,
         text_illustration_tag: bool = None,
         text_mode_type: str = None,
         text_status: str = None,
+        text_style_type: str = None,
         text_task_id: int = None,
+        text_themes: List[str] = None,
         title: str = None,
         user_name_create: str = None,
         user_name_modified: str = None,
     ):
         # This parameter is required.
         self.desc = desc
         self.gmt_create = gmt_create
         self.gmt_modified = gmt_modified
         self.illustration_task_id_list = illustration_task_id_list
+        self.publish_status = publish_status
         self.text_content = text_content
         # This parameter is required.
         self.text_id = text_id
         self.text_illustration_tag = text_illustration_tag
         self.text_mode_type = text_mode_type
         # This parameter is required.
         self.text_status = text_status
+        self.text_style_type = text_style_type
         # This parameter is required.
         self.text_task_id = text_task_id
+        self.text_themes = text_themes
         self.title = title
         # This parameter is required.
         self.user_name_create = user_name_create
         # This parameter is required.
         self.user_name_modified = user_name_modified
 
     def validate(self):
@@ -408,26 +414,32 @@
             result['desc'] = self.desc
         if self.gmt_create is not None:
             result['gmtCreate'] = self.gmt_create
         if self.gmt_modified is not None:
             result['gmtModified'] = self.gmt_modified
         if self.illustration_task_id_list is not None:
             result['illustrationTaskIdList'] = self.illustration_task_id_list
+        if self.publish_status is not None:
+            result['publishStatus'] = self.publish_status
         if self.text_content is not None:
             result['textContent'] = self.text_content
         if self.text_id is not None:
             result['textId'] = self.text_id
         if self.text_illustration_tag is not None:
             result['textIllustrationTag'] = self.text_illustration_tag
         if self.text_mode_type is not None:
             result['textModeType'] = self.text_mode_type
         if self.text_status is not None:
             result['textStatus'] = self.text_status
+        if self.text_style_type is not None:
+            result['textStyleType'] = self.text_style_type
         if self.text_task_id is not None:
             result['textTaskId'] = self.text_task_id
+        if self.text_themes is not None:
+            result['textThemes'] = self.text_themes
         if self.title is not None:
             result['title'] = self.title
         if self.user_name_create is not None:
             result['userNameCreate'] = self.user_name_create
         if self.user_name_modified is not None:
             result['userNameModified'] = self.user_name_modified
         return result
@@ -438,35 +450,88 @@
             self.desc = m.get('desc')
         if m.get('gmtCreate') is not None:
             self.gmt_create = m.get('gmtCreate')
         if m.get('gmtModified') is not None:
             self.gmt_modified = m.get('gmtModified')
         if m.get('illustrationTaskIdList') is not None:
             self.illustration_task_id_list = m.get('illustrationTaskIdList')
+        if m.get('publishStatus') is not None:
+            self.publish_status = m.get('publishStatus')
         if m.get('textContent') is not None:
             self.text_content = m.get('textContent')
         if m.get('textId') is not None:
             self.text_id = m.get('textId')
         if m.get('textIllustrationTag') is not None:
             self.text_illustration_tag = m.get('textIllustrationTag')
         if m.get('textModeType') is not None:
             self.text_mode_type = m.get('textModeType')
         if m.get('textStatus') is not None:
             self.text_status = m.get('textStatus')
+        if m.get('textStyleType') is not None:
+            self.text_style_type = m.get('textStyleType')
         if m.get('textTaskId') is not None:
             self.text_task_id = m.get('textTaskId')
+        if m.get('textThemes') is not None:
+            self.text_themes = m.get('textThemes')
         if m.get('title') is not None:
             self.title = m.get('title')
         if m.get('userNameCreate') is not None:
             self.user_name_create = m.get('userNameCreate')
         if m.get('userNameModified') is not None:
             self.user_name_modified = m.get('userNameModified')
         return self
 
 
+class TextQueryResult(TeaModel):
+    def __init__(
+        self,
+        request_id: str = None,
+        texts: List[Text] = None,
+        total: int = None,
+    ):
+        self.request_id = request_id
+        self.texts = texts
+        self.total = total
+
+    def validate(self):
+        if self.texts:
+            for k in self.texts:
+                if k:
+                    k.validate()
+
+    def to_map(self):
+        _map = super().to_map()
+        if _map is not None:
+            return _map
+
+        result = dict()
+        if self.request_id is not None:
+            result['requestId'] = self.request_id
+        result['texts'] = []
+        if self.texts is not None:
+            for k in self.texts:
+                result['texts'].append(k.to_map() if k else None)
+        if self.total is not None:
+            result['total'] = self.total
+        return result
+
+    def from_map(self, m: dict = None):
+        m = m or dict()
+        if m.get('requestId') is not None:
+            self.request_id = m.get('requestId')
+        self.texts = []
+        if m.get('texts') is not None:
+            for k in m.get('texts'):
+                temp_model = Text()
+                self.texts.append(temp_model.from_map(k))
+        if m.get('total') is not None:
+            self.total = m.get('total')
+        return self
+
+
 class TextResult(TeaModel):
     def __init__(
         self,
         request_id: str = None,
         text: Text = None,
     ):
         self.request_id = request_id
@@ -622,38 +687,42 @@
 
 
 class TextTaskCreateCmd(TeaModel):
     def __init__(
         self,
         content_requirement: str = None,
         idempotent_id: str = None,
+        industry: str = None,
         introduction: str = None,
         number: int = None,
         point: str = None,
         reference_tag: ReferenceTag = None,
         related_rag_ids: List[int] = None,
         style: str = None,
         target: str = None,
         text_mode_type: str = None,
         theme: str = None,
+        themes: List[str] = None,
     ):
         self.content_requirement = content_requirement
         self.idempotent_id = idempotent_id
+        self.industry = industry
         self.introduction = introduction
         # This parameter is required.
         self.number = number
         self.point = point
         self.reference_tag = reference_tag
         self.related_rag_ids = related_rag_ids
         # This parameter is required.
         self.style = style
         self.target = target
         # This parameter is required.
         self.text_mode_type = text_mode_type
         self.theme = theme
+        self.themes = themes
 
     def validate(self):
         if self.reference_tag:
             self.reference_tag.validate()
 
     def to_map(self):
         _map = super().to_map()
@@ -661,14 +730,16 @@
             return _map
 
         result = dict()
         if self.content_requirement is not None:
             result['contentRequirement'] = self.content_requirement
         if self.idempotent_id is not None:
             result['idempotentId'] = self.idempotent_id
+        if self.industry is not None:
+            result['industry'] = self.industry
         if self.introduction is not None:
             result['introduction'] = self.introduction
         if self.number is not None:
             result['number'] = self.number
         if self.point is not None:
             result['point'] = self.point
         if self.reference_tag is not None:
@@ -679,22 +750,26 @@
             result['style'] = self.style
         if self.target is not None:
             result['target'] = self.target
         if self.text_mode_type is not None:
             result['textModeType'] = self.text_mode_type
         if self.theme is not None:
             result['theme'] = self.theme
+        if self.themes is not None:
+            result['themes'] = self.themes
         return result
 
     def from_map(self, m: dict = None):
         m = m or dict()
         if m.get('contentRequirement') is not None:
             self.content_requirement = m.get('contentRequirement')
         if m.get('idempotentId') is not None:
             self.idempotent_id = m.get('idempotentId')
+        if m.get('industry') is not None:
+            self.industry = m.get('industry')
         if m.get('introduction') is not None:
             self.introduction = m.get('introduction')
         if m.get('number') is not None:
             self.number = m.get('number')
         if m.get('point') is not None:
             self.point = m.get('point')
         if m.get('referenceTag') is not None:
@@ -706,14 +781,16 @@
             self.style = m.get('style')
         if m.get('target') is not None:
             self.target = m.get('target')
         if m.get('textModeType') is not None:
             self.text_mode_type = m.get('textModeType')
         if m.get('theme') is not None:
             self.theme = m.get('theme')
+        if m.get('themes') is not None:
+            self.themes = m.get('themes')
         return self
 
 
 class TextTaskResult(TeaModel):
     def __init__(
         self,
         text_task: TextTask = None,
@@ -1193,14 +1270,41 @@
             self.status_code = m.get('statusCode')
         if m.get('body') is not None:
             temp_model = TextTaskResult()
             self.body = temp_model.from_map(m['body'])
         return self
 
 
+class ListTextThemesRequest(TeaModel):
+    def __init__(
+        self,
+        industry: str = None,
+    ):
+        self.industry = industry
+
+    def validate(self):
+        pass
+
+    def to_map(self):
+        _map = super().to_map()
+        if _map is not None:
+            return _map
+
+        result = dict()
+        if self.industry is not None:
+            result['industry'] = self.industry
+        return result
+
+    def from_map(self, m: dict = None):
+        m = m or dict()
+        if m.get('industry') is not None:
+            self.industry = m.get('industry')
+        return self
+
+
 class ListTextThemesResponse(TeaModel):
     def __init__(
         self,
         headers: Dict[str, str] = None,
         status_code: int = None,
         body: TextThemeListResult = None,
     ):
@@ -1234,7 +1338,111 @@
             self.status_code = m.get('statusCode')
         if m.get('body') is not None:
             temp_model = TextThemeListResult()
             self.body = temp_model.from_map(m['body'])
         return self
 
 
+class ListTextsRequest(TeaModel):
+    def __init__(
+        self,
+        generation_source: str = None,
+        industry: str = None,
+        page_number: int = None,
+        page_size: int = None,
+        publish_status: str = None,
+        text_style_type: str = None,
+        text_theme: str = None,
+    ):
+        self.generation_source = generation_source
+        self.industry = industry
+        self.page_number = page_number
+        self.page_size = page_size
+        self.publish_status = publish_status
+        self.text_style_type = text_style_type
+        self.text_theme = text_theme
+
+    def validate(self):
+        pass
+
+    def to_map(self):
+        _map = super().to_map()
+        if _map is not None:
+            return _map
+
+        result = dict()
+        if self.generation_source is not None:
+            result['generationSource'] = self.generation_source
+        if self.industry is not None:
+            result['industry'] = self.industry
+        if self.page_number is not None:
+            result['pageNumber'] = self.page_number
+        if self.page_size is not None:
+            result['pageSize'] = self.page_size
+        if self.publish_status is not None:
+            result['publishStatus'] = self.publish_status
+        if self.text_style_type is not None:
+            result['textStyleType'] = self.text_style_type
+        if self.text_theme is not None:
+            result['textTheme'] = self.text_theme
+        return result
+
+    def from_map(self, m: dict = None):
+        m = m or dict()
+        if m.get('generationSource') is not None:
+            self.generation_source = m.get('generationSource')
+        if m.get('industry') is not None:
+            self.industry = m.get('industry')
+        if m.get('pageNumber') is not None:
+            self.page_number = m.get('pageNumber')
+        if m.get('pageSize') is not None:
+            self.page_size = m.get('pageSize')
+        if m.get('publishStatus') is not None:
+            self.publish_status = m.get('publishStatus')
+        if m.get('textStyleType') is not None:
+            self.text_style_type = m.get('textStyleType')
+        if m.get('textTheme') is not None:
+            self.text_theme = m.get('textTheme')
+        return self
+
+
+class ListTextsResponse(TeaModel):
+    def __init__(
+        self,
+        headers: Dict[str, str] = None,
+        status_code: int = None,
+        body: TextQueryResult = None,
+    ):
+        self.headers = headers
+        self.status_code = status_code
+        self.body = body
+
+    def validate(self):
+        if self.body:
+            self.body.validate()
+
+    def to_map(self):
+        _map = super().to_map()
+        if _map is not None:
+            return _map
+
+        result = dict()
+        if self.headers is not None:
+            result['headers'] = self.headers
+        if self.status_code is not None:
+            result['statusCode'] = self.status_code
+        if self.body is not None:
+            result['body'] = self.body.to_map()
+        return result
+
+    def from_map(self, m: dict = None):
+        m = m or dict()
+        if m.get('headers') is not None:
+            self.headers = m.get('headers')
+        if m.get('statusCode') is not None:
+            self.status_code = m.get('statusCode')
+        if m.get('body') is not None:
+            temp_model = TextQueryResult()
+            self.body = temp_model.from_map(m['body'])
+        return self
+
+
```

### Comparing `alibabacloud_intelligentcreation20240313-1.0.0/alibabacloud_intelligentcreation20240313.egg-info/PKG-INFO` & `alibabacloud_intelligentcreation20240313-2.0.0/alibabacloud_intelligentcreation20240313.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: alibabacloud-intelligentcreation20240313
-Version: 1.0.0
+Version: 2.0.0
 Summary: Alibaba Cloud IntelligentCreation (20240313) SDK Library for Python
 Home-page: https://github.com/aliyun/alibabacloud-python-sdk
 Author: Alibaba Cloud SDK
 Author-email: sdk-team@alibabacloud.com
 License: Apache License 2.0
 Description: English | [简体中文](README-CN.md)
         ![](https://aliyunsdk-pages.alicdn.com/icons/AlibabaCloud.svg)
```

### Comparing `alibabacloud_intelligentcreation20240313-1.0.0/alibabacloud_intelligentcreation20240313.egg-info/SOURCES.txt` & `alibabacloud_intelligentcreation20240313-2.0.0/alibabacloud_intelligentcreation20240313.egg-info/SOURCES.txt`

 * *Files 15% similar despite different names*

```diff
@@ -1,7 +1,8 @@
+ChangeLog.md
 LICENSE
 MANIFEST.in
 README-CN.md
 README.md
 setup.cfg
 setup.py
 alibabacloud_intelligentcreation20240313/__init__.py
```

### Comparing `alibabacloud_intelligentcreation20240313-1.0.0/setup.py` & `alibabacloud_intelligentcreation20240313-2.0.0/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -20,15 +20,15 @@
 
 import os
 from setuptools import setup, find_packages
 
 """
 setup module for alibabacloud_intelligentcreation20240313.
 
-Created on 20/05/2024
+Created on 29/05/2024
 
 @author: Alibaba Cloud SDK
 """
 
 PACKAGE = "alibabacloud_intelligentcreation20240313"
 NAME = "alibabacloud_intelligentcreation20240313" or "alibabacloud-package"
 DESCRIPTION = "Alibaba Cloud IntelligentCreation (20240313) SDK Library for Python"
```

