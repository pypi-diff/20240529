# Comparing `tmp/latp-0.0.5.tar.gz` & `tmp/latp-0.0.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "latp-0.0.5.tar", last modified: Wed May 29 05:16:09 2024, max compression
+gzip compressed data, was "latp-0.0.6.tar", last modified: Wed May 29 05:30:48 2024, max compression
```

## Comparing `latp-0.0.5.tar` & `latp-0.0.6.tar`

### file list

```diff
@@ -1,53 +1,53 @@
-drwxrwxrwx   0        0        0        0 2024-05-29 05:16:09.523167 latp-0.0.5/
--rw-rw-rw-   0        0        0       45 2024-05-24 07:53:12.000000 latp-0.0.5/MANIFEST.in
--rw-rw-rw-   0        0        0      491 2024-05-29 05:16:09.523167 latp-0.0.5/PKG-INFO
--rw-rw-rw-   0        0        0       12 2024-05-24 08:58:32.000000 latp-0.0.5/README.md
-drwxrwxrwx   0        0        0        0 2024-05-29 05:16:09.503094 latp-0.0.5/latp/
--rw-rw-rw-   0        0        0     1267 2024-05-29 04:26:35.000000 latp-0.0.5/latp/__init__.py
--rw-rw-rw-   0        0        0      351 2024-05-28 07:22:32.000000 latp-0.0.5/latp/base_request.py
-drwxrwxrwx   0        0        0        0 2024-05-29 05:16:09.513155 latp-0.0.5/latp/case_generator/
--rw-rw-rw-   0        0        0       66 2024-05-29 03:07:31.000000 latp-0.0.5/latp/case_generator/__init__.py
--rw-rw-rw-   0        0        0     2854 2024-05-29 04:53:51.000000 latp-0.0.5/latp/case_generator/core.py
-drwxrwxrwx   0        0        0        0 2024-05-29 05:16:09.518660 latp-0.0.5/latp/case_generator/parsers/
--rw-rw-rw-   0        0        0       66 2024-05-29 03:07:31.000000 latp-0.0.5/latp/case_generator/parsers/__init__.py
--rw-rw-rw-   0        0        0      374 2024-05-29 03:28:53.000000 latp-0.0.5/latp/case_generator/parsers/base_parser.py
--rw-rw-rw-   0        0        0     1368 2024-05-29 04:11:02.000000 latp-0.0.5/latp/case_generator/parsers/har_parser.py
--rw-rw-rw-   0        0        0     2010 2024-05-29 04:11:48.000000 latp-0.0.5/latp/case_generator/parsers/postman_parser.py
--rw-rw-rw-   0        0        0     3127 2024-05-29 04:11:26.000000 latp-0.0.5/latp/case_generator/parsers/swagger_parser.py
--rw-rw-rw-   0        0        0    11314 2024-05-29 03:19:31.000000 latp-0.0.5/latp/case_generator/template.py
-drwxrwxrwx   0        0        0        0 2024-05-29 05:16:09.518660 latp-0.0.5/latp/case_generator/templates/
--rw-rw-rw-   0        0        0      289 2024-05-29 04:12:44.000000 latp-0.0.5/latp/case_generator/templates/__init__.py
--rw-rw-rw-   0        0        0     1117 2024-05-29 04:54:42.000000 latp-0.0.5/latp/case_generator/templates/pytest_template.py
--rw-rw-rw-   0        0        0     9133 2024-05-29 05:12:21.000000 latp-0.0.5/latp/case_generator/templates/robot_template.py
--rw-rw-rw-   0        0        0     1169 2024-05-29 04:54:13.000000 latp-0.0.5/latp/case_generator/templates/unittest_template.py
--rw-rw-rw-   0        0        0     1619 2024-05-29 04:18:02.000000 latp-0.0.5/latp/case_generator/utils.py
--rw-rw-rw-   0        0        0     3348 2024-05-29 03:07:21.000000 latp-0.0.5/latp/cli.py
--rw-rw-rw-   0        0        0      670 2024-05-29 03:35:26.000000 latp-0.0.5/latp/config.yaml
--rw-rw-rw-   0        0        0     2444 2024-05-28 06:48:58.000000 latp-0.0.5/latp/decorators.py
--rw-rw-rw-   0        0        0     1616 2024-05-28 07:27:26.000000 latp-0.0.5/latp/exceptions.py
--rw-rw-rw-   0        0        0     6315 2024-05-28 07:23:34.000000 latp-0.0.5/latp/http_request.py
--rw-rw-rw-   0        0        0     2320 2024-05-28 07:26:13.000000 latp-0.0.5/latp/models.py
-drwxrwxrwx   0        0        0        0 2024-05-29 05:16:09.523167 latp-0.0.5/latp/request/
--rw-rw-rw-   0        0        0      235 2024-05-29 04:46:45.000000 latp-0.0.5/latp/request/__init__.py
--rw-rw-rw-   0        0        0      353 2024-05-29 04:47:01.000000 latp-0.0.5/latp/request/base_request.py
--rw-rw-rw-   0        0        0     6303 2024-05-29 04:47:12.000000 latp-0.0.5/latp/request/http_request.py
--rw-rw-rw-   0        0        0     1013 2024-05-29 04:47:55.000000 latp-0.0.5/latp/request/request_manager.py
--rw-rw-rw-   0        0        0      646 2024-05-29 04:47:39.000000 latp-0.0.5/latp/request/websocket_request.py
--rw-rw-rw-   0        0        0     1019 2024-05-28 07:24:54.000000 latp-0.0.5/latp/request_manager.py
--rw-rw-rw-   0        0        0     4907 2024-05-29 04:30:53.000000 latp-0.0.5/latp/runner.py
--rw-rw-rw-   0        0        0     5786 2024-05-28 07:26:51.000000 latp-0.0.5/latp/utils.py
--rw-rw-rw-   0        0        0      652 2024-05-28 07:24:23.000000 latp-0.0.5/latp/websocket_request.py
-drwxrwxrwx   0        0        0        0 2024-05-29 05:16:09.523167 latp-0.0.5/latp.egg-info/
--rw-rw-rw-   0        0        0      491 2024-05-29 05:16:09.000000 latp-0.0.5/latp.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0     1194 2024-05-29 05:16:09.000000 latp-0.0.5/latp.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-05-29 05:16:09.000000 latp-0.0.5/latp.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       39 2024-05-29 05:16:09.000000 latp-0.0.5/latp.egg-info/entry_points.txt
--rw-rw-rw-   0        0        0        2 2024-05-24 07:53:22.000000 latp-0.0.5/latp.egg-info/not-zip-safe
--rw-rw-rw-   0        0        0       30 2024-05-29 05:16:09.000000 latp-0.0.5/latp.egg-info/requires.txt
--rw-rw-rw-   0        0        0       15 2024-05-29 05:16:09.000000 latp-0.0.5/latp.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2024-05-29 05:16:09.523167 latp-0.0.5/setup.cfg
--rw-rw-rw-   0        0        0     1084 2024-05-29 03:35:02.000000 latp-0.0.5/setup.py
-drwxrwxrwx   0        0        0        0 2024-05-29 05:16:09.523167 latp-0.0.5/test_case/
--rw-rw-rw-   0        0        0      128 2024-05-24 08:02:17.000000 latp-0.0.5/test_case/__init__.py
--rw-rw-rw-   0        0        0      874 2024-05-24 08:05:10.000000 latp-0.0.5/test_case/test_latp1.py
--rw-rw-rw-   0        0        0     1037 2024-05-24 08:05:10.000000 latp-0.0.5/test_case/test_latp2.py
+drwxrwxrwx   0        0        0        0 2024-05-29 05:30:48.635859 latp-0.0.6/
+-rw-rw-rw-   0        0        0       45 2024-05-24 07:53:12.000000 latp-0.0.6/MANIFEST.in
+-rw-rw-rw-   0        0        0      491 2024-05-29 05:30:48.635859 latp-0.0.6/PKG-INFO
+-rw-rw-rw-   0        0        0       12 2024-05-24 08:58:32.000000 latp-0.0.6/README.md
+drwxrwxrwx   0        0        0        0 2024-05-29 05:30:48.614302 latp-0.0.6/latp/
+-rw-rw-rw-   0        0        0     1267 2024-05-29 05:30:38.000000 latp-0.0.6/latp/__init__.py
+-rw-rw-rw-   0        0        0      351 2024-05-28 07:22:32.000000 latp-0.0.6/latp/base_request.py
+drwxrwxrwx   0        0        0        0 2024-05-29 05:30:48.624350 latp-0.0.6/latp/case_generator/
+-rw-rw-rw-   0        0        0       66 2024-05-29 03:07:31.000000 latp-0.0.6/latp/case_generator/__init__.py
+-rw-rw-rw-   0        0        0     2854 2024-05-29 04:53:51.000000 latp-0.0.6/latp/case_generator/core.py
+drwxrwxrwx   0        0        0        0 2024-05-29 05:30:48.624350 latp-0.0.6/latp/case_generator/parsers/
+-rw-rw-rw-   0        0        0       66 2024-05-29 03:07:31.000000 latp-0.0.6/latp/case_generator/parsers/__init__.py
+-rw-rw-rw-   0        0        0      374 2024-05-29 03:28:53.000000 latp-0.0.6/latp/case_generator/parsers/base_parser.py
+-rw-rw-rw-   0        0        0     1368 2024-05-29 04:11:02.000000 latp-0.0.6/latp/case_generator/parsers/har_parser.py
+-rw-rw-rw-   0        0        0     2010 2024-05-29 04:11:48.000000 latp-0.0.6/latp/case_generator/parsers/postman_parser.py
+-rw-rw-rw-   0        0        0     3127 2024-05-29 04:11:26.000000 latp-0.0.6/latp/case_generator/parsers/swagger_parser.py
+-rw-rw-rw-   0        0        0    11314 2024-05-29 03:19:31.000000 latp-0.0.6/latp/case_generator/template.py
+drwxrwxrwx   0        0        0        0 2024-05-29 05:30:48.624350 latp-0.0.6/latp/case_generator/templates/
+-rw-rw-rw-   0        0        0      289 2024-05-29 04:12:44.000000 latp-0.0.6/latp/case_generator/templates/__init__.py
+-rw-rw-rw-   0        0        0     1117 2024-05-29 04:54:42.000000 latp-0.0.6/latp/case_generator/templates/pytest_template.py
+-rw-rw-rw-   0        0        0     9133 2024-05-29 05:12:21.000000 latp-0.0.6/latp/case_generator/templates/robot_template.py
+-rw-rw-rw-   0        0        0     1169 2024-05-29 04:54:13.000000 latp-0.0.6/latp/case_generator/templates/unittest_template.py
+-rw-rw-rw-   0        0        0     1619 2024-05-29 04:18:02.000000 latp-0.0.6/latp/case_generator/utils.py
+-rw-rw-rw-   0        0        0     3535 2024-05-29 05:29:59.000000 latp-0.0.6/latp/cli.py
+-rw-rw-rw-   0        0        0      670 2024-05-29 03:35:26.000000 latp-0.0.6/latp/config.yaml
+-rw-rw-rw-   0        0        0     2444 2024-05-28 06:48:58.000000 latp-0.0.6/latp/decorators.py
+-rw-rw-rw-   0        0        0     1616 2024-05-28 07:27:26.000000 latp-0.0.6/latp/exceptions.py
+-rw-rw-rw-   0        0        0     6315 2024-05-28 07:23:34.000000 latp-0.0.6/latp/http_request.py
+-rw-rw-rw-   0        0        0     2320 2024-05-28 07:26:13.000000 latp-0.0.6/latp/models.py
+drwxrwxrwx   0        0        0        0 2024-05-29 05:30:48.624350 latp-0.0.6/latp/request/
+-rw-rw-rw-   0        0        0      235 2024-05-29 04:46:45.000000 latp-0.0.6/latp/request/__init__.py
+-rw-rw-rw-   0        0        0      353 2024-05-29 04:47:01.000000 latp-0.0.6/latp/request/base_request.py
+-rw-rw-rw-   0        0        0     6303 2024-05-29 04:47:12.000000 latp-0.0.6/latp/request/http_request.py
+-rw-rw-rw-   0        0        0     1013 2024-05-29 04:47:55.000000 latp-0.0.6/latp/request/request_manager.py
+-rw-rw-rw-   0        0        0      646 2024-05-29 04:47:39.000000 latp-0.0.6/latp/request/websocket_request.py
+-rw-rw-rw-   0        0        0     1019 2024-05-28 07:24:54.000000 latp-0.0.6/latp/request_manager.py
+-rw-rw-rw-   0        0        0     9017 2024-05-29 05:27:01.000000 latp-0.0.6/latp/runner.py
+-rw-rw-rw-   0        0        0     5786 2024-05-28 07:26:51.000000 latp-0.0.6/latp/utils.py
+-rw-rw-rw-   0        0        0      652 2024-05-28 07:24:23.000000 latp-0.0.6/latp/websocket_request.py
+drwxrwxrwx   0        0        0        0 2024-05-29 05:30:48.635859 latp-0.0.6/latp.egg-info/
+-rw-rw-rw-   0        0        0      491 2024-05-29 05:30:48.000000 latp-0.0.6/latp.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0     1194 2024-05-29 05:30:48.000000 latp-0.0.6/latp.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-05-29 05:30:48.000000 latp-0.0.6/latp.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       39 2024-05-29 05:30:48.000000 latp-0.0.6/latp.egg-info/entry_points.txt
+-rw-rw-rw-   0        0        0        2 2024-05-24 07:53:22.000000 latp-0.0.6/latp.egg-info/not-zip-safe
+-rw-rw-rw-   0        0        0       30 2024-05-29 05:30:48.000000 latp-0.0.6/latp.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       15 2024-05-29 05:30:48.000000 latp-0.0.6/latp.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2024-05-29 05:30:48.635859 latp-0.0.6/setup.cfg
+-rw-rw-rw-   0        0        0     1084 2024-05-29 03:35:02.000000 latp-0.0.6/setup.py
+drwxrwxrwx   0        0        0        0 2024-05-29 05:30:48.635859 latp-0.0.6/test_case/
+-rw-rw-rw-   0        0        0      128 2024-05-24 08:02:17.000000 latp-0.0.6/test_case/__init__.py
+-rw-rw-rw-   0        0        0      874 2024-05-24 08:05:10.000000 latp-0.0.6/test_case/test_latp1.py
+-rw-rw-rw-   0        0        0     1037 2024-05-24 08:05:10.000000 latp-0.0.6/test_case/test_latp2.py
```

### Comparing `latp-0.0.5/latp/__init__.py` & `latp-0.0.6/latp/__init__.py`

 * *Files 7% similar despite different names*

```diff
@@ -7,15 +7,15 @@
 
 import logging
 import yaml
 import os
 
 # 包信息管理
 __description__ = "A custom testing framework based on pytest"
-__version__ = "0.0.5"
+__version__ = "0.0.6"
 __pro_name__ = "latp"
 
 
 def configure_logging(config_file='config.yaml'):
     if os.path.exists(config_file):
         with open(config_file, 'r', encoding='utf-8') as f:
             config = yaml.safe_load(f)
```

### Comparing `latp-0.0.5/latp/case_generator/core.py` & `latp-0.0.6/latp/case_generator/core.py`

 * *Files identical despite different names*

### Comparing `latp-0.0.5/latp/case_generator/parsers/har_parser.py` & `latp-0.0.6/latp/case_generator/parsers/har_parser.py`

 * *Files identical despite different names*

### Comparing `latp-0.0.5/latp/case_generator/parsers/postman_parser.py` & `latp-0.0.6/latp/case_generator/parsers/postman_parser.py`

 * *Files identical despite different names*

### Comparing `latp-0.0.5/latp/case_generator/parsers/swagger_parser.py` & `latp-0.0.6/latp/case_generator/parsers/swagger_parser.py`

 * *Files identical despite different names*

### Comparing `latp-0.0.5/latp/case_generator/template.py` & `latp-0.0.6/latp/case_generator/template.py`

 * *Files identical despite different names*

### Comparing `latp-0.0.5/latp/case_generator/templates/pytest_template.py` & `latp-0.0.6/latp/case_generator/templates/pytest_template.py`

 * *Files identical despite different names*

### Comparing `latp-0.0.5/latp/case_generator/templates/robot_template.py` & `latp-0.0.6/latp/case_generator/templates/robot_template.py`

 * *Files identical despite different names*

### Comparing `latp-0.0.5/latp/case_generator/templates/unittest_template.py` & `latp-0.0.6/latp/case_generator/templates/unittest_template.py`

 * *Files identical despite different names*

### Comparing `latp-0.0.5/latp/case_generator/utils.py` & `latp-0.0.6/latp/case_generator/utils.py`

 * *Files identical despite different names*

### Comparing `latp-0.0.5/latp/cli.py` & `latp-0.0.6/latp/cli.py`

 * *Files 3% similar despite different names*

```diff
@@ -37,29 +37,32 @@
     主函数，解析命令行参数并运行测试。
     """
     parser = argparse.ArgumentParser(prog=__pro_name__, description=__description__)
     parser.add_argument("-V", "--version", dest="version", action="store_true", help="show version")
     parser.add_argument("-k", default=None, action="store", help="run tests which match the given substring expression")
     parser.add_argument("-m", default=None, action="store", help="run tests with same marks")
     parser.add_argument("-c", "--config", default=None, action="store", help="path to config file")
-    parser.add_argument("--collect-only", action="store_true", help="collect only testcase counts")
+    parser.add_argument("-co", "--collect-only", action="store_true", help="only collect testcase counts")
     parser.add_argument("--input-type", choices=["har", "swagger", "postman"], help="specify the input file type")
     parser.add_argument("--input-file", help="path to input file (HAR, Swagger JSON, Postman)")
     parser.add_argument("--output-type", choices=["unittest", "pytest", "robot"],
                         help="specify the output test case type")
     parser.add_argument("--output-dir", default=".", help="path to save generated test cases")
     parser.add_argument("path", nargs='?', help="please input test folder or module file", action="store")
 
     args = parser.parse_args()
 
     if args.version:
         print(f"{__version__}")
         sys.exit(0)
 
     if args.input_file:
+        if not args.input_type or not args.output_type:
+            logger.error("生成测试用例需要指定 --input-type 和 --output-type 参数。")
+            sys.exit(1)
         generate_testcases(args.input_file, args.input_type, args.output_dir, args.output_type)
         print(f"Test cases generated and saved to: {os.path.abspath(args.output_dir)}")
         sys.exit(0)
 
     config = load_config(args.config if args.config else 'config.yaml')
 
     test_path = args.path if args.path else config['tests']['test_path']
```

### Comparing `latp-0.0.5/latp/config.yaml` & `latp-0.0.6/latp/config.yaml`

 * *Files identical despite different names*

### Comparing `latp-0.0.5/latp/decorators.py` & `latp-0.0.6/latp/decorators.py`

 * *Files identical despite different names*

### Comparing `latp-0.0.5/latp/exceptions.py` & `latp-0.0.6/latp/exceptions.py`

 * *Files identical despite different names*

### Comparing `latp-0.0.5/latp/http_request.py` & `latp-0.0.6/latp/http_request.py`

 * *Files identical despite different names*

### Comparing `latp-0.0.5/latp/models.py` & `latp-0.0.6/latp/models.py`

 * *Files identical despite different names*

### Comparing `latp-0.0.5/latp/request/http_request.py` & `latp-0.0.6/latp/request/http_request.py`

 * *Files identical despite different names*

### Comparing `latp-0.0.5/latp/request/request_manager.py` & `latp-0.0.6/latp/request/request_manager.py`

 * *Files identical despite different names*

### Comparing `latp-0.0.5/latp/request/websocket_request.py` & `latp-0.0.6/latp/request/websocket_request.py`

 * *Files identical despite different names*

### Comparing `latp-0.0.5/latp/request_manager.py` & `latp-0.0.6/latp/request_manager.py`

 * *Files identical despite different names*

### Comparing `latp-0.0.5/latp/utils.py` & `latp-0.0.6/latp/utils.py`

 * *Files identical despite different names*

### Comparing `latp-0.0.5/latp/websocket_request.py` & `latp-0.0.6/latp/websocket_request.py`

 * *Files identical despite different names*

### Comparing `latp-0.0.5/latp.egg-info/SOURCES.txt` & `latp-0.0.6/latp.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `latp-0.0.5/setup.py` & `latp-0.0.6/setup.py`

 * *Files identical despite different names*

### Comparing `latp-0.0.5/test_case/test_latp1.py` & `latp-0.0.6/test_case/test_latp1.py`

 * *Files identical despite different names*

### Comparing `latp-0.0.5/test_case/test_latp2.py` & `latp-0.0.6/test_case/test_latp2.py`

 * *Files identical despite different names*

