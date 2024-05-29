# Comparing `tmp/aura_tools-0.1.tar.gz` & `tmp/aura_tools-0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "aura_tools-0.1.tar", last modified: Wed May 29 11:08:26 2024, max compression
+gzip compressed data, was "aura_tools-0.2.tar", last modified: Wed May 29 11:31:48 2024, max compression
```

## Comparing `aura_tools-0.1.tar` & `aura_tools-0.2.tar`

### file list

```diff
@@ -1,19 +1,26 @@
-drwxrwxrwx   0        0        0        0 2024-05-29 11:08:26.855510 aura_tools-0.1/
--rw-rw-rw-   0        0        0        0 2024-05-29 09:52:44.000000 aura_tools-0.1/LICENSE
--rw-rw-rw-   0        0        0      428 2024-05-29 11:08:26.853325 aura_tools-0.1/PKG-INFO
--rw-rw-rw-   0        0        0        0 2024-05-29 09:52:34.000000 aura_tools-0.1/README.md
-drwxrwxrwx   0        0        0        0 2024-05-29 11:08:26.842214 aura_tools-0.1/aura_tools/
--rw-rw-rw-   0        0        0        0 2024-05-29 09:51:35.000000 aura_tools-0.1/aura_tools/__init__.py
--rw-rw-rw-   0        0        0     4796 2024-05-29 10:03:44.000000 aura_tools-0.1/aura_tools/code_explanation_generator.py
--rw-rw-rw-   0        0        0     2382 2024-05-27 01:35:26.000000 aura_tools-0.1/aura_tools/director_scanner.py
--rw-rw-rw-   0        0        0     3370 2024-05-27 01:35:26.000000 aura_tools-0.1/aura_tools/github_repository_downloader.py
--rw-rw-rw-   0        0        0     1905 2024-05-29 10:00:36.000000 aura_tools-0.1/aura_tools/java_function_extractor.py
--rw-rw-rw-   0        0        0     2242 2024-05-27 09:22:00.000000 aura_tools-0.1/aura_tools/json_file_util.py
-drwxrwxrwx   0        0        0        0 2024-05-29 11:08:26.852132 aura_tools-0.1/aura_tools.egg-info/
--rw-rw-rw-   0        0        0      428 2024-05-29 11:08:26.000000 aura_tools-0.1/aura_tools.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      404 2024-05-29 11:08:26.000000 aura_tools-0.1/aura_tools.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-05-29 11:08:26.000000 aura_tools-0.1/aura_tools.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       59 2024-05-29 11:08:26.000000 aura_tools-0.1/aura_tools.egg-info/entry_points.txt
--rw-rw-rw-   0        0        0       11 2024-05-29 11:08:26.000000 aura_tools-0.1/aura_tools.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2024-05-29 11:08:26.855510 aura_tools-0.1/setup.cfg
--rw-rw-rw-   0        0        0      872 2024-05-29 11:08:15.000000 aura_tools-0.1/setup.py
+drwxrwxrwx   0        0        0        0 2024-05-29 11:31:48.827835 aura_tools-0.2/
+-rw-rw-rw-   0        0        0        0 2024-05-29 09:52:44.000000 aura_tools-0.2/LICENSE
+-rw-rw-rw-   0        0        0      428 2024-05-29 11:31:48.825646 aura_tools-0.2/PKG-INFO
+-rw-rw-rw-   0        0        0        0 2024-05-29 09:52:34.000000 aura_tools-0.2/README.md
+drwxrwxrwx   0        0        0        0 2024-05-29 11:31:48.803716 aura_tools-0.2/aura_tools/
+-rw-rw-rw-   0        0        0        0 2024-05-29 09:51:35.000000 aura_tools-0.2/aura_tools/__init__.py
+-rw-rw-rw-   0        0        0     4796 2024-05-29 10:03:44.000000 aura_tools-0.2/aura_tools/code_explanation_generator.py
+-rw-rw-rw-   0        0        0     2382 2024-05-27 01:35:26.000000 aura_tools-0.2/aura_tools/director_scanner.py
+-rw-rw-rw-   0        0        0     3370 2024-05-27 01:35:26.000000 aura_tools-0.2/aura_tools/github_repository_downloader.py
+-rw-rw-rw-   0        0        0     1905 2024-05-29 10:00:36.000000 aura_tools-0.2/aura_tools/java_function_extractor.py
+-rw-rw-rw-   0        0        0     2242 2024-05-27 09:22:00.000000 aura_tools-0.2/aura_tools/json_file_util.py
+drwxrwxrwx   0        0        0        0 2024-05-29 11:31:48.818613 aura_tools-0.2/aura_tools/llm/
+-rw-rw-rw-   0        0        0        0 2024-05-29 11:30:16.000000 aura_tools-0.2/aura_tools/llm/__init__.py
+-rw-rw-rw-   0        0        0     3465 2024-05-29 09:58:21.000000 aura_tools-0.2/aura_tools/llm/baidu_ai_client.py
+drwxrwxrwx   0        0        0        0 2024-05-29 11:31:48.821966 aura_tools-0.2/aura_tools/llm/base/
+-rw-rw-rw-   0        0        0        0 2024-05-29 11:30:35.000000 aura_tools-0.2/aura_tools/llm/base/__init__.py
+-rw-rw-rw-   0        0        0      444 2024-05-29 09:04:11.000000 aura_tools-0.2/aura_tools/llm/base/llm_base_client.py
+-rw-rw-rw-   0        0        0     2689 2024-05-29 10:05:42.000000 aura_tools-0.2/aura_tools/llm/tongyi_ai_client.py
+drwxrwxrwx   0        0        0        0 2024-05-29 11:31:48.824776 aura_tools-0.2/aura_tools.egg-info/
+-rw-rw-rw-   0        0        0      428 2024-05-29 11:31:48.000000 aura_tools-0.2/aura_tools.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      571 2024-05-29 11:31:48.000000 aura_tools-0.2/aura_tools.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-05-29 11:31:48.000000 aura_tools-0.2/aura_tools.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       59 2024-05-29 11:31:48.000000 aura_tools-0.2/aura_tools.egg-info/entry_points.txt
+-rw-rw-rw-   0        0        0       11 2024-05-29 11:31:48.000000 aura_tools-0.2/aura_tools.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2024-05-29 11:31:48.827940 aura_tools-0.2/setup.cfg
+-rw-rw-rw-   0        0        0      872 2024-05-29 11:31:11.000000 aura_tools-0.2/setup.py
```

### Comparing `aura_tools-0.1/aura_tools/code_explanation_generator.py` & `aura_tools-0.2/aura_tools/code_explanation_generator.py`

 * *Files identical despite different names*

### Comparing `aura_tools-0.1/aura_tools/director_scanner.py` & `aura_tools-0.2/aura_tools/director_scanner.py`

 * *Files identical despite different names*

### Comparing `aura_tools-0.1/aura_tools/github_repository_downloader.py` & `aura_tools-0.2/aura_tools/github_repository_downloader.py`

 * *Files identical despite different names*

### Comparing `aura_tools-0.1/aura_tools/java_function_extractor.py` & `aura_tools-0.2/aura_tools/java_function_extractor.py`

 * *Files identical despite different names*

### Comparing `aura_tools-0.1/aura_tools/json_file_util.py` & `aura_tools-0.2/aura_tools/json_file_util.py`

 * *Files identical despite different names*

### Comparing `aura_tools-0.1/setup.py` & `aura_tools-0.2/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from setuptools import setup, find_packages
 
 setup(
     name='aura_tools',  # 包名
-    version='0.1',  # 版本号
+    version='0.2',  # 版本号
     packages=find_packages(),  # 自动找到包目录
     install_requires=[  # 依赖包
         # 'some_package>=1.0',
     ],
     entry_points={  # 可选的命令行工具
         'console_scripts': [
             'my_command=my_project.some_module:main',
```

