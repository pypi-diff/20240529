# Comparing `tmp/latp-0.0.3.tar.gz` & `tmp/latp-0.0.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "latp-0.0.3.tar", last modified: Tue May 28 08:25:51 2024, max compression
+gzip compressed data, was "latp-0.0.4.tar", last modified: Tue May 28 08:47:36 2024, max compression
```

## Comparing `latp-0.0.3.tar` & `latp-0.0.4.tar`

### file list

```diff
@@ -1,31 +1,31 @@
-drwxrwxrwx   0        0        0        0 2024-05-28 08:25:51.383251 latp-0.0.3/
--rw-rw-rw-   0        0        0       45 2024-05-24 07:53:12.000000 latp-0.0.3/MANIFEST.in
--rw-rw-rw-   0        0        0      502 2024-05-28 08:25:51.371006 latp-0.0.3/PKG-INFO
--rw-rw-rw-   0        0        0       12 2024-05-24 08:58:32.000000 latp-0.0.3/README.md
-drwxrwxrwx   0        0        0        0 2024-05-28 08:25:51.371006 latp-0.0.3/latp/
--rw-rw-rw-   0        0        0      309 2024-05-28 08:25:47.000000 latp-0.0.3/latp/__init__.py
--rw-rw-rw-   0        0        0      351 2024-05-28 07:22:32.000000 latp-0.0.3/latp/base_request.py
--rw-rw-rw-   0        0        0     2744 2024-05-28 07:58:35.000000 latp-0.0.3/latp/cli.py
--rw-rw-rw-   0        0        0      655 2024-05-28 08:16:05.000000 latp-0.0.3/latp/config.yaml
--rw-rw-rw-   0        0        0     2444 2024-05-28 06:48:58.000000 latp-0.0.3/latp/decorators.py
--rw-rw-rw-   0        0        0     1616 2024-05-28 07:27:26.000000 latp-0.0.3/latp/exceptions.py
--rw-rw-rw-   0        0        0     6315 2024-05-28 07:23:34.000000 latp-0.0.3/latp/http_request.py
--rw-rw-rw-   0        0        0     2320 2024-05-28 07:26:13.000000 latp-0.0.3/latp/models.py
--rw-rw-rw-   0        0        0     1019 2024-05-28 07:24:54.000000 latp-0.0.3/latp/request_manager.py
--rw-rw-rw-   0        0        0     8229 2024-05-28 08:22:23.000000 latp-0.0.3/latp/runner.py
--rw-rw-rw-   0        0        0     5786 2024-05-28 07:26:51.000000 latp-0.0.3/latp/utils.py
--rw-rw-rw-   0        0        0      652 2024-05-28 07:24:23.000000 latp-0.0.3/latp/websocket_request.py
-drwxrwxrwx   0        0        0        0 2024-05-28 08:25:51.371006 latp-0.0.3/latp.egg-info/
--rw-rw-rw-   0        0        0      502 2024-05-28 08:25:51.000000 latp-0.0.3/latp.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      517 2024-05-28 08:25:51.000000 latp-0.0.3/latp.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-05-28 08:25:51.000000 latp-0.0.3/latp.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       39 2024-05-28 08:25:51.000000 latp-0.0.3/latp.egg-info/entry_points.txt
--rw-rw-rw-   0        0        0        2 2024-05-24 07:53:22.000000 latp-0.0.3/latp.egg-info/not-zip-safe
--rw-rw-rw-   0        0        0       39 2024-05-28 08:25:51.000000 latp-0.0.3/latp.egg-info/requires.txt
--rw-rw-rw-   0        0        0       15 2024-05-28 08:25:51.000000 latp-0.0.3/latp.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2024-05-28 08:25:51.383251 latp-0.0.3/setup.cfg
--rw-rw-rw-   0        0        0     1044 2024-05-28 07:48:49.000000 latp-0.0.3/setup.py
-drwxrwxrwx   0        0        0        0 2024-05-28 08:25:51.371006 latp-0.0.3/test_case/
--rw-rw-rw-   0        0        0      128 2024-05-24 08:02:17.000000 latp-0.0.3/test_case/__init__.py
--rw-rw-rw-   0        0        0      874 2024-05-24 08:05:10.000000 latp-0.0.3/test_case/test_latp1.py
--rw-rw-rw-   0        0        0     1037 2024-05-24 08:05:10.000000 latp-0.0.3/test_case/test_latp2.py
+drwxrwxrwx   0        0        0        0 2024-05-28 08:47:36.277367 latp-0.0.4/
+-rw-rw-rw-   0        0        0       45 2024-05-24 07:53:12.000000 latp-0.0.4/MANIFEST.in
+-rw-rw-rw-   0        0        0      502 2024-05-28 08:47:36.277367 latp-0.0.4/PKG-INFO
+-rw-rw-rw-   0        0        0       12 2024-05-24 08:58:32.000000 latp-0.0.4/README.md
+drwxrwxrwx   0        0        0        0 2024-05-28 08:47:36.270275 latp-0.0.4/latp/
+-rw-rw-rw-   0        0        0      309 2024-05-28 08:47:17.000000 latp-0.0.4/latp/__init__.py
+-rw-rw-rw-   0        0        0      351 2024-05-28 07:22:32.000000 latp-0.0.4/latp/base_request.py
+-rw-rw-rw-   0        0        0     2759 2024-05-28 08:44:45.000000 latp-0.0.4/latp/cli.py
+-rw-rw-rw-   0        0        0      655 2024-05-28 08:16:05.000000 latp-0.0.4/latp/config.yaml
+-rw-rw-rw-   0        0        0     2444 2024-05-28 06:48:58.000000 latp-0.0.4/latp/decorators.py
+-rw-rw-rw-   0        0        0     1616 2024-05-28 07:27:26.000000 latp-0.0.4/latp/exceptions.py
+-rw-rw-rw-   0        0        0     6315 2024-05-28 07:23:34.000000 latp-0.0.4/latp/http_request.py
+-rw-rw-rw-   0        0        0     2320 2024-05-28 07:26:13.000000 latp-0.0.4/latp/models.py
+-rw-rw-rw-   0        0        0     1019 2024-05-28 07:24:54.000000 latp-0.0.4/latp/request_manager.py
+-rw-rw-rw-   0        0        0     8586 2024-05-28 08:46:44.000000 latp-0.0.4/latp/runner.py
+-rw-rw-rw-   0        0        0     5786 2024-05-28 07:26:51.000000 latp-0.0.4/latp/utils.py
+-rw-rw-rw-   0        0        0      652 2024-05-28 07:24:23.000000 latp-0.0.4/latp/websocket_request.py
+drwxrwxrwx   0        0        0        0 2024-05-28 08:47:36.277367 latp-0.0.4/latp.egg-info/
+-rw-rw-rw-   0        0        0      502 2024-05-28 08:47:36.000000 latp-0.0.4/latp.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      517 2024-05-28 08:47:36.000000 latp-0.0.4/latp.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-05-28 08:47:36.000000 latp-0.0.4/latp.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       39 2024-05-28 08:47:36.000000 latp-0.0.4/latp.egg-info/entry_points.txt
+-rw-rw-rw-   0        0        0        2 2024-05-24 07:53:22.000000 latp-0.0.4/latp.egg-info/not-zip-safe
+-rw-rw-rw-   0        0        0       39 2024-05-28 08:47:36.000000 latp-0.0.4/latp.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       15 2024-05-28 08:47:36.000000 latp-0.0.4/latp.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2024-05-28 08:47:36.277367 latp-0.0.4/setup.cfg
+-rw-rw-rw-   0        0        0     1044 2024-05-28 07:48:49.000000 latp-0.0.4/setup.py
+drwxrwxrwx   0        0        0        0 2024-05-28 08:47:36.277367 latp-0.0.4/test_case/
+-rw-rw-rw-   0        0        0      128 2024-05-24 08:02:17.000000 latp-0.0.4/test_case/__init__.py
+-rw-rw-rw-   0        0        0      874 2024-05-24 08:05:10.000000 latp-0.0.4/test_case/test_latp1.py
+-rw-rw-rw-   0        0        0     1037 2024-05-24 08:05:10.000000 latp-0.0.4/test_case/test_latp2.py
```

### Comparing `latp-0.0.3/latp/cli.py` & `latp-0.0.4/latp/cli.py`

 * *Files 4% similar despite different names*

```diff
@@ -43,15 +43,15 @@
     parser.add_argument(
         "-m", default=None, action="store", help="run tests with same marks")
     parser.add_argument(
         "-c", "--config", default=None, action="store", help="path to config file")
     parser.add_argument(
         "--collect-only", action="store_true", help="collect only testcase counts")
     parser.add_argument(
-        "path", nargs='?', help="please input test folder", action="store")
+        "path", nargs='?', help="please input test folder or module file", action="store")
 
     args = parser.parse_args()
 
     # 加载配置文件
     config_path = args.config if args.config else os.path.join(os.path.dirname(__file__), 'config.yaml')
     config = load_config(config_path)
```

### Comparing `latp-0.0.3/latp/config.yaml` & `latp-0.0.4/latp/config.yaml`

 * *Files identical despite different names*

### Comparing `latp-0.0.3/latp/decorators.py` & `latp-0.0.4/latp/decorators.py`

 * *Files identical despite different names*

### Comparing `latp-0.0.3/latp/exceptions.py` & `latp-0.0.4/latp/exceptions.py`

 * *Files identical despite different names*

### Comparing `latp-0.0.3/latp/http_request.py` & `latp-0.0.4/latp/http_request.py`

 * *Files identical despite different names*

### Comparing `latp-0.0.3/latp/models.py` & `latp-0.0.4/latp/models.py`

 * *Files identical despite different names*

### Comparing `latp-0.0.3/latp/request_manager.py` & `latp-0.0.4/latp/request_manager.py`

 * *Files identical despite different names*

### Comparing `latp-0.0.3/latp/runner.py` & `latp-0.0.4/latp/runner.py`

 * *Files 4% similar despite different names*

```diff
@@ -53,15 +53,14 @@
         folder: 文件夹路径。
         module_pattern: 模块名称匹配模式（正则表达式）。
 
     Returns:
         模块名称和路径的列表。
     """
     absolute_f = os.path.abspath(folder)
-    print(f"文件夹路径为: {absolute_f}")
     modules = glob.glob(os.path.join(absolute_f, "**", "*.py"), recursive=True)
     pattern = re.compile(module_pattern)
     return [(os.path.relpath(f, start=absolute_f)[:-3].replace(os.sep, '.'), f) for f in modules if
             os.path.isfile(f) and not f.endswith('__init__.py') and pattern.match(os.path.basename(f)[:-3])]
 
 
 def import_modules_dynamically(module, file_path):
@@ -106,15 +105,21 @@
 
     logger.info(f"关键字过滤表达式: {keyword}")
     logger.info(f"标记过滤表达式: {mark}")
     logger.info(f"模块匹配模式: {module_pattern}")
     logger.info(f"类匹配模式: {class_pattern}")
     logger.info(f"函数/方法匹配模式: {function_pattern}")
 
-    module_list = find_modules_from_folder(test_path, module_pattern)
+    if os.path.isfile(test_path):
+        # 单个文件模式
+        module_list = [(os.path.splitext(os.path.basename(test_path))[0], test_path)]
+    else:
+        # 文件夹模式
+        module_list = find_modules_from_folder(test_path, module_pattern)
+
     logger.info(f"找到的模块: {[module[0] for module in module_list]}")
 
     test_case_list = []
     for module in module_list:
         module_name, module_file = module
         logger.info(f"正在导入模块: {module_name}，路径: {module_file}")
         _module = import_modules_dynamically(module_name, module_file)
@@ -213,15 +218,21 @@
         test_path: 测试用例路径。
 
     Returns:
         测试用例数量。
     """
     config_path = os.path.join(os.path.dirname(__file__), 'config.yaml')
     config = load_config(config_path)
-    module_list = find_modules_from_folder(test_path, config['tests']['module_pattern'])
+    if os.path.isfile(test_path):
+        # 单个文件模式
+        module_list = [(os.path.splitext(os.path.basename(test_path))[0], test_path)]
+    else:
+        # 文件夹模式
+        module_list = find_modules_from_folder(test_path, config['tests']['module_pattern'])
+
     test_case_count = 0
     for module in module_list:
         module_name, module_file = module
         _module = import_modules_dynamically(module_name, module_file)
         test_case_list = []
         collect_test_cases(_module, test_case_list, module_file, config['tests']['class_pattern'],
                            config['tests']['function_pattern'])
@@ -229,14 +240,14 @@
     return test_case_count
 
 
 if __name__ == "__main__":
     import argparse
 
     parser = argparse.ArgumentParser(description="Test Runner")
-    parser.add_argument('test_path', type=str, help="Path to the test files")
+    parser.add_argument('test_path', type=str, help="Path to the test files or directory")
     parser.add_argument('-k', type=str, help="Only run tests that match the given substring expression")
     parser.add_argument('-m', type=str, help="Only run tests that have the given mark expression")
     parser.add_argument('-c', '--config', type=str, default='config.yaml', help="Path to the config file")
     args = parser.parse_args()
 
     run(args, args.test_path)
```

### Comparing `latp-0.0.3/latp/utils.py` & `latp-0.0.4/latp/utils.py`

 * *Files identical despite different names*

### Comparing `latp-0.0.3/latp/websocket_request.py` & `latp-0.0.4/latp/websocket_request.py`

 * *Files identical despite different names*

### Comparing `latp-0.0.3/latp.egg-info/SOURCES.txt` & `latp-0.0.4/latp.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `latp-0.0.3/setup.py` & `latp-0.0.4/setup.py`

 * *Files identical despite different names*

### Comparing `latp-0.0.3/test_case/test_latp1.py` & `latp-0.0.4/test_case/test_latp1.py`

 * *Files identical despite different names*

### Comparing `latp-0.0.3/test_case/test_latp2.py` & `latp-0.0.4/test_case/test_latp2.py`

 * *Files identical despite different names*

