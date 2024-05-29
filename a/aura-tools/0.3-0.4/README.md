# Comparing `tmp/aura_tools-0.3.tar.gz` & `tmp/aura_tools-0.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "aura_tools-0.3.tar", last modified: Wed May 29 11:43:22 2024, max compression
+gzip compressed data, was "aura_tools-0.4.tar", last modified: Wed May 29 11:45:55 2024, max compression
```

## Comparing `aura_tools-0.3.tar` & `aura_tools-0.4.tar`

### file list

```diff
@@ -1,26 +1,26 @@
-drwxrwxrwx   0        0        0        0 2024-05-29 11:43:22.600726 aura_tools-0.3/
--rw-rw-rw-   0        0        0        0 2024-05-29 09:52:44.000000 aura_tools-0.3/LICENSE
--rw-rw-rw-   0        0        0      428 2024-05-29 11:43:22.598517 aura_tools-0.3/PKG-INFO
--rw-rw-rw-   0        0        0        0 2024-05-29 09:52:34.000000 aura_tools-0.3/README.md
-drwxrwxrwx   0        0        0        0 2024-05-29 11:43:22.576916 aura_tools-0.3/aura_tools/
--rw-rw-rw-   0        0        0        0 2024-05-29 09:51:35.000000 aura_tools-0.3/aura_tools/__init__.py
--rw-rw-rw-   0        0        0     4853 2024-05-29 11:43:02.000000 aura_tools-0.3/aura_tools/code_explanation_generator.py
--rw-rw-rw-   0        0        0     2382 2024-05-27 01:35:26.000000 aura_tools-0.3/aura_tools/director_scanner.py
--rw-rw-rw-   0        0        0     3370 2024-05-27 01:35:26.000000 aura_tools-0.3/aura_tools/github_repository_downloader.py
--rw-rw-rw-   0        0        0     1905 2024-05-29 10:00:36.000000 aura_tools-0.3/aura_tools/java_function_extractor.py
--rw-rw-rw-   0        0        0     2242 2024-05-27 09:22:00.000000 aura_tools-0.3/aura_tools/json_file_util.py
-drwxrwxrwx   0        0        0        0 2024-05-29 11:43:22.591926 aura_tools-0.3/aura_tools/llm/
--rw-rw-rw-   0        0        0        0 2024-05-29 11:30:16.000000 aura_tools-0.3/aura_tools/llm/__init__.py
--rw-rw-rw-   0        0        0     3465 2024-05-29 09:58:21.000000 aura_tools-0.3/aura_tools/llm/baidu_ai_client.py
-drwxrwxrwx   0        0        0        0 2024-05-29 11:43:22.595587 aura_tools-0.3/aura_tools/llm/base/
--rw-rw-rw-   0        0        0        0 2024-05-29 11:30:35.000000 aura_tools-0.3/aura_tools/llm/base/__init__.py
--rw-rw-rw-   0        0        0      444 2024-05-29 09:04:11.000000 aura_tools-0.3/aura_tools/llm/base/llm_base_client.py
--rw-rw-rw-   0        0        0     2689 2024-05-29 10:05:42.000000 aura_tools-0.3/aura_tools/llm/tongyi_ai_client.py
-drwxrwxrwx   0        0        0        0 2024-05-29 11:43:22.597582 aura_tools-0.3/aura_tools.egg-info/
--rw-rw-rw-   0        0        0      428 2024-05-29 11:43:22.000000 aura_tools-0.3/aura_tools.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      571 2024-05-29 11:43:22.000000 aura_tools-0.3/aura_tools.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-05-29 11:43:22.000000 aura_tools-0.3/aura_tools.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       59 2024-05-29 11:43:22.000000 aura_tools-0.3/aura_tools.egg-info/entry_points.txt
--rw-rw-rw-   0        0        0       11 2024-05-29 11:43:22.000000 aura_tools-0.3/aura_tools.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2024-05-29 11:43:22.600726 aura_tools-0.3/setup.cfg
--rw-rw-rw-   0        0        0      872 2024-05-29 11:43:10.000000 aura_tools-0.3/setup.py
+drwxrwxrwx   0        0        0        0 2024-05-29 11:45:55.573463 aura_tools-0.4/
+-rw-rw-rw-   0        0        0        0 2024-05-29 09:52:44.000000 aura_tools-0.4/LICENSE
+-rw-rw-rw-   0        0        0      428 2024-05-29 11:45:55.570474 aura_tools-0.4/PKG-INFO
+-rw-rw-rw-   0        0        0        0 2024-05-29 09:52:34.000000 aura_tools-0.4/README.md
+drwxrwxrwx   0        0        0        0 2024-05-29 11:45:55.541390 aura_tools-0.4/aura_tools/
+-rw-rw-rw-   0        0        0        0 2024-05-29 09:51:35.000000 aura_tools-0.4/aura_tools/__init__.py
+-rw-rw-rw-   0        0        0     4853 2024-05-29 11:43:02.000000 aura_tools-0.4/aura_tools/code_explanation_generator.py
+-rw-rw-rw-   0        0        0     2382 2024-05-27 01:35:26.000000 aura_tools-0.4/aura_tools/director_scanner.py
+-rw-rw-rw-   0        0        0     3370 2024-05-27 01:35:26.000000 aura_tools-0.4/aura_tools/github_repository_downloader.py
+-rw-rw-rw-   0        0        0     1905 2024-05-29 10:00:36.000000 aura_tools-0.4/aura_tools/java_function_extractor.py
+-rw-rw-rw-   0        0        0     2242 2024-05-27 09:22:00.000000 aura_tools-0.4/aura_tools/json_file_util.py
+drwxrwxrwx   0        0        0        0 2024-05-29 11:45:55.558774 aura_tools-0.4/aura_tools/llm/
+-rw-rw-rw-   0        0        0        0 2024-05-29 11:30:16.000000 aura_tools-0.4/aura_tools/llm/__init__.py
+-rw-rw-rw-   0        0        0     3481 2024-05-29 11:44:56.000000 aura_tools-0.4/aura_tools/llm/baidu_ai_client.py
+drwxrwxrwx   0        0        0        0 2024-05-29 11:45:55.563186 aura_tools-0.4/aura_tools/llm/base/
+-rw-rw-rw-   0        0        0        0 2024-05-29 11:30:35.000000 aura_tools-0.4/aura_tools/llm/base/__init__.py
+-rw-rw-rw-   0        0        0      444 2024-05-29 09:04:11.000000 aura_tools-0.4/aura_tools/llm/base/llm_base_client.py
+-rw-rw-rw-   0        0        0     2769 2024-05-29 11:45:24.000000 aura_tools-0.4/aura_tools/llm/tongyi_ai_client.py
+drwxrwxrwx   0        0        0        0 2024-05-29 11:45:55.567923 aura_tools-0.4/aura_tools.egg-info/
+-rw-rw-rw-   0        0        0      428 2024-05-29 11:45:55.000000 aura_tools-0.4/aura_tools.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      571 2024-05-29 11:45:55.000000 aura_tools-0.4/aura_tools.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-05-29 11:45:55.000000 aura_tools-0.4/aura_tools.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       59 2024-05-29 11:45:55.000000 aura_tools-0.4/aura_tools.egg-info/entry_points.txt
+-rw-rw-rw-   0        0        0       11 2024-05-29 11:45:55.000000 aura_tools-0.4/aura_tools.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2024-05-29 11:45:55.573463 aura_tools-0.4/setup.cfg
+-rw-rw-rw-   0        0        0      872 2024-05-29 11:45:38.000000 aura_tools-0.4/setup.py
```

### Comparing `aura_tools-0.3/aura_tools/code_explanation_generator.py` & `aura_tools-0.4/aura_tools/code_explanation_generator.py`

 * *Files identical despite different names*

### Comparing `aura_tools-0.3/aura_tools/director_scanner.py` & `aura_tools-0.4/aura_tools/director_scanner.py`

 * *Files identical despite different names*

### Comparing `aura_tools-0.3/aura_tools/github_repository_downloader.py` & `aura_tools-0.4/aura_tools/github_repository_downloader.py`

 * *Files identical despite different names*

### Comparing `aura_tools-0.3/aura_tools/java_function_extractor.py` & `aura_tools-0.4/aura_tools/java_function_extractor.py`

 * *Files identical despite different names*

### Comparing `aura_tools-0.3/aura_tools/json_file_util.py` & `aura_tools-0.4/aura_tools/json_file_util.py`

 * *Files identical despite different names*

### Comparing `aura_tools-0.3/aura_tools/llm/baidu_ai_client.py` & `aura_tools-0.4/aura_tools/llm/baidu_ai_client.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,11 +1,12 @@
 import requests
 import json
 import time
-from base.llm_base_client import LLMBaseClient
+
+from aura_tools.llm.base.llm_base_client import LLMBaseClient
 
 
 class BaiduAIClient(LLMBaseClient):
     def __init__(self, api_key, model="", max_retries=3, retry_interval=60):
         keys = api_key.split("|");
         self.api_key = keys[0]
         self.secret_key = keys[1]
```

### Comparing `aura_tools-0.3/aura_tools/llm/tongyi_ai_client.py` & `aura_tools-0.4/aura_tools/llm/tongyi_ai_client.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,13 +1,15 @@
 import requests
 import json
 import time
 
+from aura_tools.llm.base.llm_base_client import LLMBaseClient
 
-class TongYiQianWenClient:
+
+class TongYiQianWenClient(LLMBaseClient):
     def __init__(self, api_key, model, max_retries=3, retry_interval=60):
         self.api_key = api_key
         self.model = model
         self.max_retries = max_retries
         self.retry_interval = retry_interval
         self.base_url = "https://dashscope.aliyuncs.com/compatible-mode/v1/chat/completions"
         self.headers = {
```

### Comparing `aura_tools-0.3/aura_tools.egg-info/SOURCES.txt` & `aura_tools-0.4/aura_tools.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `aura_tools-0.3/setup.py` & `aura_tools-0.4/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from setuptools import setup, find_packages
 
 setup(
     name='aura_tools',  # 包名
-    version='0.3',  # 版本号
+    version='0.4',  # 版本号
     packages=find_packages(),  # 自动找到包目录
     install_requires=[  # 依赖包
         # 'some_package>=1.0',
     ],
     entry_points={  # 可选的命令行工具
         'console_scripts': [
             'my_command=my_project.some_module:main',
```

