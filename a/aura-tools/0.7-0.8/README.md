# Comparing `tmp/aura_tools-0.7.tar.gz` & `tmp/aura_tools-0.8.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "aura_tools-0.7.tar", last modified: Wed May 29 12:04:02 2024, max compression
+gzip compressed data, was "aura_tools-0.8.tar", last modified: Wed May 29 12:29:20 2024, max compression
```

## Comparing `aura_tools-0.7.tar` & `aura_tools-0.8.tar`

### file list

```diff
@@ -1,29 +1,30 @@
-drwxrwxrwx   0        0        0        0 2024-05-29 12:04:02.231241 aura_tools-0.7/
--rw-rw-rw-   0        0        0        0 2024-05-29 09:52:44.000000 aura_tools-0.7/LICENSE
--rw-rw-rw-   0        0        0      428 2024-05-29 12:04:02.230152 aura_tools-0.7/PKG-INFO
--rw-rw-rw-   0        0        0        0 2024-05-29 09:52:34.000000 aura_tools-0.7/README.md
-drwxrwxrwx   0        0        0        0 2024-05-29 12:04:02.208308 aura_tools-0.7/aura_tools/
--rw-rw-rw-   0        0        0        0 2024-05-29 09:51:35.000000 aura_tools-0.7/aura_tools/__init__.py
--rw-rw-rw-   0        0        0     4853 2024-05-29 11:43:02.000000 aura_tools-0.7/aura_tools/code_explanation_generator.py
--rw-rw-rw-   0        0        0     2382 2024-05-27 01:35:26.000000 aura_tools-0.7/aura_tools/director_scanner.py
--rw-rw-rw-   0        0        0     3370 2024-05-27 01:35:26.000000 aura_tools-0.7/aura_tools/github_repository_downloader.py
--rw-rw-rw-   0        0        0     1905 2024-05-29 10:00:36.000000 aura_tools-0.7/aura_tools/java_function_extractor.py
--rw-rw-rw-   0        0        0     2242 2024-05-27 09:22:00.000000 aura_tools-0.7/aura_tools/json_file_util.py
-drwxrwxrwx   0        0        0        0 2024-05-29 12:04:02.220457 aura_tools-0.7/aura_tools/llm/
--rw-rw-rw-   0        0        0        0 2024-05-29 11:30:16.000000 aura_tools-0.7/aura_tools/llm/__init__.py
--rw-rw-rw-   0        0        0     3486 2024-05-29 12:03:32.000000 aura_tools-0.7/aura_tools/llm/baidu_ai_client.py
-drwxrwxrwx   0        0        0        0 2024-05-29 12:04:02.223461 aura_tools-0.7/aura_tools/llm/base/
--rw-rw-rw-   0        0        0        0 2024-05-29 11:30:35.000000 aura_tools-0.7/aura_tools/llm/base/__init__.py
--rw-rw-rw-   0        0        0      444 2024-05-29 09:04:11.000000 aura_tools-0.7/aura_tools/llm/base/llm_base_client.py
--rw-rw-rw-   0        0        0     2769 2024-05-29 11:45:24.000000 aura_tools-0.7/aura_tools/llm/tongyi_ai_client.py
-drwxrwxrwx   0        0        0        0 2024-05-29 12:04:02.227181 aura_tools-0.7/aura_tools/process/
--rw-rw-rw-   0        0        0        0 2024-05-29 11:54:58.000000 aura_tools-0.7/aura_tools/process/__init__.py
--rw-rw-rw-   0        0        0     2121 2024-05-29 11:57:29.000000 aura_tools-0.7/aura_tools/process/multi_process_handler.py
-drwxrwxrwx   0        0        0        0 2024-05-29 12:04:02.228566 aura_tools-0.7/aura_tools.egg-info/
--rw-rw-rw-   0        0        0      428 2024-05-29 12:04:02.000000 aura_tools-0.7/aura_tools.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      646 2024-05-29 12:04:02.000000 aura_tools-0.7/aura_tools.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-05-29 12:04:02.000000 aura_tools-0.7/aura_tools.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       59 2024-05-29 12:04:02.000000 aura_tools-0.7/aura_tools.egg-info/entry_points.txt
--rw-rw-rw-   0        0        0       11 2024-05-29 12:04:02.000000 aura_tools-0.7/aura_tools.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2024-05-29 12:04:02.232141 aura_tools-0.7/setup.cfg
--rw-rw-rw-   0        0        0      872 2024-05-29 12:03:44.000000 aura_tools-0.7/setup.py
+drwxrwxrwx   0        0        0        0 2024-05-29 12:29:20.995993 aura_tools-0.8/
+-rw-rw-rw-   0        0        0        0 2024-05-29 09:52:44.000000 aura_tools-0.8/LICENSE
+-rw-rw-rw-   0        0        0      428 2024-05-29 12:29:20.995059 aura_tools-0.8/PKG-INFO
+-rw-rw-rw-   0        0        0        0 2024-05-29 09:52:34.000000 aura_tools-0.8/README.md
+drwxrwxrwx   0        0        0        0 2024-05-29 12:29:20.964664 aura_tools-0.8/aura_tools/
+-rw-rw-rw-   0        0        0        0 2024-05-29 09:51:35.000000 aura_tools-0.8/aura_tools/__init__.py
+-rw-rw-rw-   0        0        0     4868 2024-05-29 12:26:52.000000 aura_tools-0.8/aura_tools/code_explanation_generator.py
+-rw-rw-rw-   0        0        0     1554 2024-05-29 12:23:18.000000 aura_tools-0.8/aura_tools/count_functions.py
+-rw-rw-rw-   0        0        0     2382 2024-05-27 01:35:26.000000 aura_tools-0.8/aura_tools/director_scanner.py
+-rw-rw-rw-   0        0        0     3370 2024-05-27 01:35:26.000000 aura_tools-0.8/aura_tools/github_repository_downloader.py
+-rw-rw-rw-   0        0        0     1905 2024-05-29 10:00:36.000000 aura_tools-0.8/aura_tools/java_function_extractor.py
+-rw-rw-rw-   0        0        0     2242 2024-05-27 09:22:00.000000 aura_tools-0.8/aura_tools/json_file_util.py
+drwxrwxrwx   0        0        0        0 2024-05-29 12:29:20.980980 aura_tools-0.8/aura_tools/llm/
+-rw-rw-rw-   0        0        0        0 2024-05-29 11:30:16.000000 aura_tools-0.8/aura_tools/llm/__init__.py
+-rw-rw-rw-   0        0        0     3486 2024-05-29 12:03:32.000000 aura_tools-0.8/aura_tools/llm/baidu_ai_client.py
+drwxrwxrwx   0        0        0        0 2024-05-29 12:29:20.986993 aura_tools-0.8/aura_tools/llm/base/
+-rw-rw-rw-   0        0        0        0 2024-05-29 11:30:35.000000 aura_tools-0.8/aura_tools/llm/base/__init__.py
+-rw-rw-rw-   0        0        0      444 2024-05-29 09:04:11.000000 aura_tools-0.8/aura_tools/llm/base/llm_base_client.py
+-rw-rw-rw-   0        0        0     2769 2024-05-29 11:45:24.000000 aura_tools-0.8/aura_tools/llm/tongyi_ai_client.py
+drwxrwxrwx   0        0        0        0 2024-05-29 12:29:20.991088 aura_tools-0.8/aura_tools/process/
+-rw-rw-rw-   0        0        0        0 2024-05-29 11:54:58.000000 aura_tools-0.8/aura_tools/process/__init__.py
+-rw-rw-rw-   0        0        0     2121 2024-05-29 11:57:29.000000 aura_tools-0.8/aura_tools/process/multi_process_handler.py
+drwxrwxrwx   0        0        0        0 2024-05-29 12:29:20.993012 aura_tools-0.8/aura_tools.egg-info/
+-rw-rw-rw-   0        0        0      428 2024-05-29 12:29:20.000000 aura_tools-0.8/aura_tools.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      676 2024-05-29 12:29:20.000000 aura_tools-0.8/aura_tools.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-05-29 12:29:20.000000 aura_tools-0.8/aura_tools.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       59 2024-05-29 12:29:20.000000 aura_tools-0.8/aura_tools.egg-info/entry_points.txt
+-rw-rw-rw-   0        0        0       11 2024-05-29 12:29:20.000000 aura_tools-0.8/aura_tools.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2024-05-29 12:29:20.996905 aura_tools-0.8/setup.cfg
+-rw-rw-rw-   0        0        0      872 2024-05-29 12:29:08.000000 aura_tools-0.8/setup.py
```

### Comparing `aura_tools-0.7/aura_tools/code_explanation_generator.py` & `aura_tools-0.8/aura_tools/code_explanation_generator.py`

 * *Files 4% similar despite different names*

```diff
@@ -69,15 +69,15 @@
                 self.result_file.append_json_line(json.dumps(result, ensure_ascii=False))
         except Exception as e:
             print(f"Error: {e}")
             timestamp = datetime.now().strftime("%Y-%m-%d %H:%M:%S")
             self.error_file.append_json_line(f"{timestamp} Error: {e} , file = {file}")
 
     @staticmethod
-    def download_and_scan(repo_url):
+    def download_and_scan(repo_url,target_dir='.'):
         """下载仓库并扫描Java文件"""
         dir_path = GithubRepositoryDownloader(repo_url).download()
         print(f"仓库已下载到: {dir_path}")
 
         scanner = DirectoryScanner(dir_path, filter_types=['.java'])
         all_files = scanner.scan_all()
         java_files = scanner.filter_files_by_type(all_files)
```

### Comparing `aura_tools-0.7/aura_tools/director_scanner.py` & `aura_tools-0.8/aura_tools/director_scanner.py`

 * *Files identical despite different names*

### Comparing `aura_tools-0.7/aura_tools/github_repository_downloader.py` & `aura_tools-0.8/aura_tools/github_repository_downloader.py`

 * *Files identical despite different names*

### Comparing `aura_tools-0.7/aura_tools/java_function_extractor.py` & `aura_tools-0.8/aura_tools/java_function_extractor.py`

 * *Files identical despite different names*

### Comparing `aura_tools-0.7/aura_tools/json_file_util.py` & `aura_tools-0.8/aura_tools/json_file_util.py`

 * *Files identical despite different names*

### Comparing `aura_tools-0.7/aura_tools/llm/baidu_ai_client.py` & `aura_tools-0.8/aura_tools/llm/baidu_ai_client.py`

 * *Files identical despite different names*

### Comparing `aura_tools-0.7/aura_tools/llm/tongyi_ai_client.py` & `aura_tools-0.8/aura_tools/llm/tongyi_ai_client.py`

 * *Files identical despite different names*

### Comparing `aura_tools-0.7/aura_tools/process/multi_process_handler.py` & `aura_tools-0.8/aura_tools/process/multi_process_handler.py`

 * *Files identical despite different names*

### Comparing `aura_tools-0.7/aura_tools.egg-info/SOURCES.txt` & `aura_tools-0.8/aura_tools.egg-info/SOURCES.txt`

 * *Files 4% similar despite different names*

```diff
@@ -1,12 +1,13 @@
 LICENSE
 README.md
 setup.py
 aura_tools/__init__.py
 aura_tools/code_explanation_generator.py
+aura_tools/count_functions.py
 aura_tools/director_scanner.py
 aura_tools/github_repository_downloader.py
 aura_tools/java_function_extractor.py
 aura_tools/json_file_util.py
 aura_tools.egg-info/PKG-INFO
 aura_tools.egg-info/SOURCES.txt
 aura_tools.egg-info/dependency_links.txt
```

### Comparing `aura_tools-0.7/setup.py` & `aura_tools-0.8/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from setuptools import setup, find_packages
 
 setup(
     name='aura_tools',  # 包名
-    version='0.7',  # 版本号
+    version='0.8',  # 版本号
     packages=find_packages(),  # 自动找到包目录
     install_requires=[  # 依赖包
         # 'some_package>=1.0',
     ],
     entry_points={  # 可选的命令行工具
         'console_scripts': [
             'my_command=my_project.some_module:main',
```

