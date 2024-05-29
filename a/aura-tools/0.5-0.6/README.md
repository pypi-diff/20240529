# Comparing `tmp/aura_tools-0.5.tar.gz` & `tmp/aura_tools-0.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "aura_tools-0.5.tar", last modified: Wed May 29 11:56:08 2024, max compression
+gzip compressed data, was "aura_tools-0.6.tar", last modified: Wed May 29 11:57:57 2024, max compression
```

## Comparing `aura_tools-0.5.tar` & `aura_tools-0.6.tar`

### file list

```diff
@@ -1,29 +1,29 @@
-drwxrwxrwx   0        0        0        0 2024-05-29 11:56:08.745885 aura_tools-0.5/
--rw-rw-rw-   0        0        0        0 2024-05-29 09:52:44.000000 aura_tools-0.5/LICENSE
--rw-rw-rw-   0        0        0      428 2024-05-29 11:56:08.744382 aura_tools-0.5/PKG-INFO
--rw-rw-rw-   0        0        0        0 2024-05-29 09:52:34.000000 aura_tools-0.5/README.md
-drwxrwxrwx   0        0        0        0 2024-05-29 11:56:08.721675 aura_tools-0.5/aura_tools/
--rw-rw-rw-   0        0        0        0 2024-05-29 09:51:35.000000 aura_tools-0.5/aura_tools/__init__.py
--rw-rw-rw-   0        0        0     4853 2024-05-29 11:43:02.000000 aura_tools-0.5/aura_tools/code_explanation_generator.py
--rw-rw-rw-   0        0        0     2382 2024-05-27 01:35:26.000000 aura_tools-0.5/aura_tools/director_scanner.py
--rw-rw-rw-   0        0        0     3370 2024-05-27 01:35:26.000000 aura_tools-0.5/aura_tools/github_repository_downloader.py
--rw-rw-rw-   0        0        0     1905 2024-05-29 10:00:36.000000 aura_tools-0.5/aura_tools/java_function_extractor.py
--rw-rw-rw-   0        0        0     2242 2024-05-27 09:22:00.000000 aura_tools-0.5/aura_tools/json_file_util.py
-drwxrwxrwx   0        0        0        0 2024-05-29 11:56:08.734408 aura_tools-0.5/aura_tools/llm/
--rw-rw-rw-   0        0        0        0 2024-05-29 11:30:16.000000 aura_tools-0.5/aura_tools/llm/__init__.py
--rw-rw-rw-   0        0        0     3481 2024-05-29 11:44:56.000000 aura_tools-0.5/aura_tools/llm/baidu_ai_client.py
-drwxrwxrwx   0        0        0        0 2024-05-29 11:56:08.737836 aura_tools-0.5/aura_tools/llm/base/
--rw-rw-rw-   0        0        0        0 2024-05-29 11:30:35.000000 aura_tools-0.5/aura_tools/llm/base/__init__.py
--rw-rw-rw-   0        0        0      444 2024-05-29 09:04:11.000000 aura_tools-0.5/aura_tools/llm/base/llm_base_client.py
--rw-rw-rw-   0        0        0     2769 2024-05-29 11:45:24.000000 aura_tools-0.5/aura_tools/llm/tongyi_ai_client.py
-drwxrwxrwx   0        0        0        0 2024-05-29 11:56:08.741440 aura_tools-0.5/aura_tools/process/
--rw-rw-rw-   0        0        0        0 2024-05-29 11:54:58.000000 aura_tools-0.5/aura_tools/process/__init__.py
--rw-rw-rw-   0        0        0     2165 2024-05-29 11:54:22.000000 aura_tools-0.5/aura_tools/process/multi_process_handler.py
-drwxrwxrwx   0        0        0        0 2024-05-29 11:56:08.743414 aura_tools-0.5/aura_tools.egg-info/
--rw-rw-rw-   0        0        0      428 2024-05-29 11:56:08.000000 aura_tools-0.5/aura_tools.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      646 2024-05-29 11:56:08.000000 aura_tools-0.5/aura_tools.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-05-29 11:56:08.000000 aura_tools-0.5/aura_tools.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       59 2024-05-29 11:56:08.000000 aura_tools-0.5/aura_tools.egg-info/entry_points.txt
--rw-rw-rw-   0        0        0       11 2024-05-29 11:56:08.000000 aura_tools-0.5/aura_tools.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2024-05-29 11:56:08.745885 aura_tools-0.5/setup.cfg
--rw-rw-rw-   0        0        0      872 2024-05-29 11:55:22.000000 aura_tools-0.5/setup.py
+drwxrwxrwx   0        0        0        0 2024-05-29 11:57:57.227437 aura_tools-0.6/
+-rw-rw-rw-   0        0        0        0 2024-05-29 09:52:44.000000 aura_tools-0.6/LICENSE
+-rw-rw-rw-   0        0        0      428 2024-05-29 11:57:57.225532 aura_tools-0.6/PKG-INFO
+-rw-rw-rw-   0        0        0        0 2024-05-29 09:52:34.000000 aura_tools-0.6/README.md
+drwxrwxrwx   0        0        0        0 2024-05-29 11:57:57.197924 aura_tools-0.6/aura_tools/
+-rw-rw-rw-   0        0        0        0 2024-05-29 09:51:35.000000 aura_tools-0.6/aura_tools/__init__.py
+-rw-rw-rw-   0        0        0     4853 2024-05-29 11:43:02.000000 aura_tools-0.6/aura_tools/code_explanation_generator.py
+-rw-rw-rw-   0        0        0     2382 2024-05-27 01:35:26.000000 aura_tools-0.6/aura_tools/director_scanner.py
+-rw-rw-rw-   0        0        0     3370 2024-05-27 01:35:26.000000 aura_tools-0.6/aura_tools/github_repository_downloader.py
+-rw-rw-rw-   0        0        0     1905 2024-05-29 10:00:36.000000 aura_tools-0.6/aura_tools/java_function_extractor.py
+-rw-rw-rw-   0        0        0     2242 2024-05-27 09:22:00.000000 aura_tools-0.6/aura_tools/json_file_util.py
+drwxrwxrwx   0        0        0        0 2024-05-29 11:57:57.212689 aura_tools-0.6/aura_tools/llm/
+-rw-rw-rw-   0        0        0        0 2024-05-29 11:30:16.000000 aura_tools-0.6/aura_tools/llm/__init__.py
+-rw-rw-rw-   0        0        0     3481 2024-05-29 11:44:56.000000 aura_tools-0.6/aura_tools/llm/baidu_ai_client.py
+drwxrwxrwx   0        0        0        0 2024-05-29 11:57:57.216341 aura_tools-0.6/aura_tools/llm/base/
+-rw-rw-rw-   0        0        0        0 2024-05-29 11:30:35.000000 aura_tools-0.6/aura_tools/llm/base/__init__.py
+-rw-rw-rw-   0        0        0      444 2024-05-29 09:04:11.000000 aura_tools-0.6/aura_tools/llm/base/llm_base_client.py
+-rw-rw-rw-   0        0        0     2769 2024-05-29 11:45:24.000000 aura_tools-0.6/aura_tools/llm/tongyi_ai_client.py
+drwxrwxrwx   0        0        0        0 2024-05-29 11:57:57.221584 aura_tools-0.6/aura_tools/process/
+-rw-rw-rw-   0        0        0        0 2024-05-29 11:54:58.000000 aura_tools-0.6/aura_tools/process/__init__.py
+-rw-rw-rw-   0        0        0     2121 2024-05-29 11:57:29.000000 aura_tools-0.6/aura_tools/process/multi_process_handler.py
+drwxrwxrwx   0        0        0        0 2024-05-29 11:57:57.223592 aura_tools-0.6/aura_tools.egg-info/
+-rw-rw-rw-   0        0        0      428 2024-05-29 11:57:57.000000 aura_tools-0.6/aura_tools.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      646 2024-05-29 11:57:57.000000 aura_tools-0.6/aura_tools.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-05-29 11:57:57.000000 aura_tools-0.6/aura_tools.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       59 2024-05-29 11:57:57.000000 aura_tools-0.6/aura_tools.egg-info/entry_points.txt
+-rw-rw-rw-   0        0        0       11 2024-05-29 11:57:57.000000 aura_tools-0.6/aura_tools.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2024-05-29 11:57:57.227437 aura_tools-0.6/setup.cfg
+-rw-rw-rw-   0        0        0      872 2024-05-29 11:57:35.000000 aura_tools-0.6/setup.py
```

### Comparing `aura_tools-0.5/aura_tools/code_explanation_generator.py` & `aura_tools-0.6/aura_tools/code_explanation_generator.py`

 * *Files identical despite different names*

### Comparing `aura_tools-0.5/aura_tools/director_scanner.py` & `aura_tools-0.6/aura_tools/director_scanner.py`

 * *Files identical despite different names*

### Comparing `aura_tools-0.5/aura_tools/github_repository_downloader.py` & `aura_tools-0.6/aura_tools/github_repository_downloader.py`

 * *Files identical despite different names*

### Comparing `aura_tools-0.5/aura_tools/java_function_extractor.py` & `aura_tools-0.6/aura_tools/java_function_extractor.py`

 * *Files identical despite different names*

### Comparing `aura_tools-0.5/aura_tools/json_file_util.py` & `aura_tools-0.6/aura_tools/json_file_util.py`

 * *Files identical despite different names*

### Comparing `aura_tools-0.5/aura_tools/llm/baidu_ai_client.py` & `aura_tools-0.6/aura_tools/llm/baidu_ai_client.py`

 * *Files identical despite different names*

### Comparing `aura_tools-0.5/aura_tools/llm/tongyi_ai_client.py` & `aura_tools-0.6/aura_tools/llm/tongyi_ai_client.py`

 * *Files identical despite different names*

### Comparing `aura_tools-0.5/aura_tools/process/multi_process_handler.py` & `aura_tools-0.6/aura_tools/process/multi_process_handler.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,9 +1,10 @@
 from multiprocessing import Process
-from code_explanation_generator import CodeExplanationGenerator;
+
+from aura_tools.code_explanation_generator import CodeExplanationGenerator
 
 
 class MultiProcessHandler:
     def __init__(self, data, process_func, num_processes=None, **kwargs):
         self.data = data
         self.process_func = process_func
         self.num_processes = num_processes or len(data)
@@ -41,16 +42,16 @@
     generator = CodeExplanationGenerator(api_key, secret_key,
                                          result_file=f"outputs/result{process_id}.json",
                                          error_file=f"outputs/error{process_id}.json")
     generator.process_files(data_chunk)
 
 
 if __name__ == '__main__':
-    api_key = "koFGGYEM9zD9u8NapXZmqVit"
-    secret_key = "A9o1RGt27CwrbT6pTnuuhaHAOciuBesw"
+    api_key = ""
+    secret_key = ""
 
     java_files = CodeExplanationGenerator(api_key, secret_key).download_and_scan(
         'https://github.com/langchain4j/langchain4j')
 
     handler = MultiProcessHandler(data=java_files,
                                   process_func=process_files,
                                   num_processes=6,
```

### Comparing `aura_tools-0.5/aura_tools.egg-info/SOURCES.txt` & `aura_tools-0.6/aura_tools.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `aura_tools-0.5/setup.py` & `aura_tools-0.6/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from setuptools import setup, find_packages
 
 setup(
     name='aura_tools',  # 包名
-    version='0.5',  # 版本号
+    version='0.6',  # 版本号
     packages=find_packages(),  # 自动找到包目录
     install_requires=[  # 依赖包
         # 'some_package>=1.0',
     ],
     entry_points={  # 可选的命令行工具
         'console_scripts': [
             'my_command=my_project.some_module:main',
```

