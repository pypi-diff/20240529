# Comparing `tmp/aura_tools-0.2.tar.gz` & `tmp/aura_tools-0.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "aura_tools-0.2.tar", last modified: Wed May 29 11:31:48 2024, max compression
+gzip compressed data, was "aura_tools-0.3.tar", last modified: Wed May 29 11:43:22 2024, max compression
```

## Comparing `aura_tools-0.2.tar` & `aura_tools-0.3.tar`

### file list

```diff
@@ -1,26 +1,26 @@
-drwxrwxrwx   0        0        0        0 2024-05-29 11:31:48.827835 aura_tools-0.2/
--rw-rw-rw-   0        0        0        0 2024-05-29 09:52:44.000000 aura_tools-0.2/LICENSE
--rw-rw-rw-   0        0        0      428 2024-05-29 11:31:48.825646 aura_tools-0.2/PKG-INFO
--rw-rw-rw-   0        0        0        0 2024-05-29 09:52:34.000000 aura_tools-0.2/README.md
-drwxrwxrwx   0        0        0        0 2024-05-29 11:31:48.803716 aura_tools-0.2/aura_tools/
--rw-rw-rw-   0        0        0        0 2024-05-29 09:51:35.000000 aura_tools-0.2/aura_tools/__init__.py
--rw-rw-rw-   0        0        0     4796 2024-05-29 10:03:44.000000 aura_tools-0.2/aura_tools/code_explanation_generator.py
--rw-rw-rw-   0        0        0     2382 2024-05-27 01:35:26.000000 aura_tools-0.2/aura_tools/director_scanner.py
--rw-rw-rw-   0        0        0     3370 2024-05-27 01:35:26.000000 aura_tools-0.2/aura_tools/github_repository_downloader.py
--rw-rw-rw-   0        0        0     1905 2024-05-29 10:00:36.000000 aura_tools-0.2/aura_tools/java_function_extractor.py
--rw-rw-rw-   0        0        0     2242 2024-05-27 09:22:00.000000 aura_tools-0.2/aura_tools/json_file_util.py
-drwxrwxrwx   0        0        0        0 2024-05-29 11:31:48.818613 aura_tools-0.2/aura_tools/llm/
--rw-rw-rw-   0        0        0        0 2024-05-29 11:30:16.000000 aura_tools-0.2/aura_tools/llm/__init__.py
--rw-rw-rw-   0        0        0     3465 2024-05-29 09:58:21.000000 aura_tools-0.2/aura_tools/llm/baidu_ai_client.py
-drwxrwxrwx   0        0        0        0 2024-05-29 11:31:48.821966 aura_tools-0.2/aura_tools/llm/base/
--rw-rw-rw-   0        0        0        0 2024-05-29 11:30:35.000000 aura_tools-0.2/aura_tools/llm/base/__init__.py
--rw-rw-rw-   0        0        0      444 2024-05-29 09:04:11.000000 aura_tools-0.2/aura_tools/llm/base/llm_base_client.py
--rw-rw-rw-   0        0        0     2689 2024-05-29 10:05:42.000000 aura_tools-0.2/aura_tools/llm/tongyi_ai_client.py
-drwxrwxrwx   0        0        0        0 2024-05-29 11:31:48.824776 aura_tools-0.2/aura_tools.egg-info/
--rw-rw-rw-   0        0        0      428 2024-05-29 11:31:48.000000 aura_tools-0.2/aura_tools.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      571 2024-05-29 11:31:48.000000 aura_tools-0.2/aura_tools.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-05-29 11:31:48.000000 aura_tools-0.2/aura_tools.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       59 2024-05-29 11:31:48.000000 aura_tools-0.2/aura_tools.egg-info/entry_points.txt
--rw-rw-rw-   0        0        0       11 2024-05-29 11:31:48.000000 aura_tools-0.2/aura_tools.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2024-05-29 11:31:48.827940 aura_tools-0.2/setup.cfg
--rw-rw-rw-   0        0        0      872 2024-05-29 11:31:11.000000 aura_tools-0.2/setup.py
+drwxrwxrwx   0        0        0        0 2024-05-29 11:43:22.600726 aura_tools-0.3/
+-rw-rw-rw-   0        0        0        0 2024-05-29 09:52:44.000000 aura_tools-0.3/LICENSE
+-rw-rw-rw-   0        0        0      428 2024-05-29 11:43:22.598517 aura_tools-0.3/PKG-INFO
+-rw-rw-rw-   0        0        0        0 2024-05-29 09:52:34.000000 aura_tools-0.3/README.md
+drwxrwxrwx   0        0        0        0 2024-05-29 11:43:22.576916 aura_tools-0.3/aura_tools/
+-rw-rw-rw-   0        0        0        0 2024-05-29 09:51:35.000000 aura_tools-0.3/aura_tools/__init__.py
+-rw-rw-rw-   0        0        0     4853 2024-05-29 11:43:02.000000 aura_tools-0.3/aura_tools/code_explanation_generator.py
+-rw-rw-rw-   0        0        0     2382 2024-05-27 01:35:26.000000 aura_tools-0.3/aura_tools/director_scanner.py
+-rw-rw-rw-   0        0        0     3370 2024-05-27 01:35:26.000000 aura_tools-0.3/aura_tools/github_repository_downloader.py
+-rw-rw-rw-   0        0        0     1905 2024-05-29 10:00:36.000000 aura_tools-0.3/aura_tools/java_function_extractor.py
+-rw-rw-rw-   0        0        0     2242 2024-05-27 09:22:00.000000 aura_tools-0.3/aura_tools/json_file_util.py
+drwxrwxrwx   0        0        0        0 2024-05-29 11:43:22.591926 aura_tools-0.3/aura_tools/llm/
+-rw-rw-rw-   0        0        0        0 2024-05-29 11:30:16.000000 aura_tools-0.3/aura_tools/llm/__init__.py
+-rw-rw-rw-   0        0        0     3465 2024-05-29 09:58:21.000000 aura_tools-0.3/aura_tools/llm/baidu_ai_client.py
+drwxrwxrwx   0        0        0        0 2024-05-29 11:43:22.595587 aura_tools-0.3/aura_tools/llm/base/
+-rw-rw-rw-   0        0        0        0 2024-05-29 11:30:35.000000 aura_tools-0.3/aura_tools/llm/base/__init__.py
+-rw-rw-rw-   0        0        0      444 2024-05-29 09:04:11.000000 aura_tools-0.3/aura_tools/llm/base/llm_base_client.py
+-rw-rw-rw-   0        0        0     2689 2024-05-29 10:05:42.000000 aura_tools-0.3/aura_tools/llm/tongyi_ai_client.py
+drwxrwxrwx   0        0        0        0 2024-05-29 11:43:22.597582 aura_tools-0.3/aura_tools.egg-info/
+-rw-rw-rw-   0        0        0      428 2024-05-29 11:43:22.000000 aura_tools-0.3/aura_tools.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      571 2024-05-29 11:43:22.000000 aura_tools-0.3/aura_tools.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-05-29 11:43:22.000000 aura_tools-0.3/aura_tools.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       59 2024-05-29 11:43:22.000000 aura_tools-0.3/aura_tools.egg-info/entry_points.txt
+-rw-rw-rw-   0        0        0       11 2024-05-29 11:43:22.000000 aura_tools-0.3/aura_tools.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2024-05-29 11:43:22.600726 aura_tools-0.3/setup.cfg
+-rw-rw-rw-   0        0        0      872 2024-05-29 11:43:10.000000 aura_tools-0.3/setup.py
```

### Comparing `aura_tools-0.2/aura_tools/code_explanation_generator.py` & `aura_tools-0.3/aura_tools/code_explanation_generator.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,15 +1,16 @@
 import json
 from datetime import datetime
 
-from director_scanner import DirectoryScanner
-from github_repository_downloader import GithubRepositoryDownloader
-from java_function_extractor import JavaFunctionExtractor
-from json_file_util import JsonFileUtils
-from llm.baidu_ai_client import BaiduAIClient
+from aura_tools.director_scanner import DirectoryScanner
+
+from aura_tools.github_repository_downloader import GithubRepositoryDownloader
+from aura_tools.java_function_extractor import JavaFunctionExtractor
+from aura_tools.json_file_util import JsonFileUtils
+from aura_tools.llm.baidu_ai_client import BaiduAIClient
 
 
 class CodeExplanationGenerator:
     def __init__(self, client, result_file='outputs/result.json', error_file='outputs/error.json', description=""):
         self.client = client
         self.result_file = JsonFileUtils(result_file)
         self.error_file = JsonFileUtils(error_file)
```

### Comparing `aura_tools-0.2/aura_tools/director_scanner.py` & `aura_tools-0.3/aura_tools/director_scanner.py`

 * *Files identical despite different names*

### Comparing `aura_tools-0.2/aura_tools/github_repository_downloader.py` & `aura_tools-0.3/aura_tools/github_repository_downloader.py`

 * *Files identical despite different names*

### Comparing `aura_tools-0.2/aura_tools/java_function_extractor.py` & `aura_tools-0.3/aura_tools/java_function_extractor.py`

 * *Files identical despite different names*

### Comparing `aura_tools-0.2/aura_tools/json_file_util.py` & `aura_tools-0.3/aura_tools/json_file_util.py`

 * *Files identical despite different names*

### Comparing `aura_tools-0.2/aura_tools/llm/baidu_ai_client.py` & `aura_tools-0.3/aura_tools/llm/baidu_ai_client.py`

 * *Files identical despite different names*

### Comparing `aura_tools-0.2/aura_tools/llm/tongyi_ai_client.py` & `aura_tools-0.3/aura_tools/llm/tongyi_ai_client.py`

 * *Files identical despite different names*

### Comparing `aura_tools-0.2/aura_tools.egg-info/SOURCES.txt` & `aura_tools-0.3/aura_tools.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `aura_tools-0.2/setup.py` & `aura_tools-0.3/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from setuptools import setup, find_packages
 
 setup(
     name='aura_tools',  # 包名
-    version='0.2',  # 版本号
+    version='0.3',  # 版本号
     packages=find_packages(),  # 自动找到包目录
     install_requires=[  # 依赖包
         # 'some_package>=1.0',
     ],
     entry_points={  # 可选的命令行工具
         'console_scripts': [
             'my_command=my_project.some_module:main',
```

