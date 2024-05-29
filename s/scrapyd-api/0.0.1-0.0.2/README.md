# Comparing `tmp/scrapyd-api-0.0.1.tar.gz` & `tmp/scrapyd_api-0.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/scrapyd-api-0.0.1.tar", last modified: Mon Jan 25 10:33:00 2021, max compression
+gzip compressed data, was "scrapyd_api-0.0.2.tar", last modified: Wed May 29 10:00:56 2024, max compression
```

## Comparing `scrapyd-api-0.0.1.tar` & `scrapyd_api-0.0.2.tar`

### file list

```diff
@@ -1,20 +1,20 @@
-drwxr-xr-x   0 hina       (501) staff       (20)        0 2021-01-25 10:33:00.000000 scrapyd-api-0.0.1/
--rwxr-xr-x   0 hina       (501) staff       (20)      276 2021-01-25 10:10:44.000000 scrapyd-api-0.0.1/MANIFEST.in
--rw-r--r--   0 hina       (501) staff       (20)     3282 2021-01-25 10:33:00.000000 scrapyd-api-0.0.1/PKG-INFO
--rw-r--r--   0 hina       (501) staff       (20)     2248 2021-01-25 10:31:59.000000 scrapyd-api-0.0.1/README.md
--rwxr-xr-x   0 hina       (501) staff       (20)       25 2021-01-25 10:09:48.000000 scrapyd-api-0.0.1/requirements.txt
-drwxr-xr-x   0 hina       (501) staff       (20)        0 2021-01-25 10:33:00.000000 scrapyd-api-0.0.1/scrapyd_api/
--rw-r--r--   0 hina       (501) staff       (20)      103 2021-01-25 10:03:29.000000 scrapyd-api-0.0.1/scrapyd_api/__init__.py
--rw-r--r--   0 hina       (501) staff       (20)      115 2021-01-25 10:12:21.000000 scrapyd-api-0.0.1/scrapyd_api/constants.py
--rw-r--r--   0 hina       (501) staff       (20)      128 2021-01-18 13:28:23.000000 scrapyd-api-0.0.1/scrapyd_api/exceptions.py
--rwxr-xr-x   0 hina       (501) staff       (20)     5778 2021-01-25 09:52:40.000000 scrapyd-api-0.0.1/scrapyd_api/scrapyd_api.py
--rw-r--r--   0 hina       (501) staff       (20)     9462 2021-01-25 10:26:45.000000 scrapyd-api-0.0.1/scrapyd_api/scrapyd_client.py
-drwxr-xr-x   0 hina       (501) staff       (20)        0 2021-01-25 10:33:00.000000 scrapyd-api-0.0.1/scrapyd_api.egg-info/
--rw-r--r--   0 hina       (501) staff       (20)     3282 2021-01-25 10:33:00.000000 scrapyd-api-0.0.1/scrapyd_api.egg-info/PKG-INFO
--rw-r--r--   0 hina       (501) staff       (20)      383 2021-01-25 10:33:00.000000 scrapyd-api-0.0.1/scrapyd_api.egg-info/SOURCES.txt
--rw-r--r--   0 hina       (501) staff       (20)        1 2021-01-25 10:33:00.000000 scrapyd-api-0.0.1/scrapyd_api.egg-info/dependency_links.txt
--rw-r--r--   0 hina       (501) staff       (20)       23 2021-01-25 10:33:00.000000 scrapyd-api-0.0.1/scrapyd_api.egg-info/requires.txt
--rw-r--r--   0 hina       (501) staff       (20)       12 2021-01-25 10:33:00.000000 scrapyd-api-0.0.1/scrapyd_api.egg-info/top_level.txt
--rw-r--r--   0 hina       (501) staff       (20)        1 2021-01-25 10:33:00.000000 scrapyd-api-0.0.1/scrapyd_api.egg-info/zip-safe
--rw-r--r--   0 hina       (501) staff       (20)       38 2021-01-25 10:33:00.000000 scrapyd-api-0.0.1/setup.cfg
--rwxr-xr-x   0 hina       (501) staff       (20)     1669 2021-01-25 10:00:33.000000 scrapyd-api-0.0.1/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-29 10:00:56.228744 scrapyd_api-0.0.2/
+-rwxr-xr-x   0 runner    (1001) docker     (127)      276 2024-05-29 10:00:48.000000 scrapyd_api-0.0.2/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (127)     2657 2024-05-29 10:00:56.228744 scrapyd_api-0.0.2/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     2248 2024-05-29 10:00:48.000000 scrapyd_api-0.0.2/README.md
+-rwxr-xr-x   0 runner    (1001) docker     (127)       25 2024-05-29 10:00:48.000000 scrapyd_api-0.0.2/requirements.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-29 10:00:56.224744 scrapyd_api-0.0.2/scrapyd_api/
+-rw-r--r--   0 runner    (1001) docker     (127)      103 2024-05-29 10:00:48.000000 scrapyd_api-0.0.2/scrapyd_api/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      115 2024-05-29 10:00:48.000000 scrapyd_api-0.0.2/scrapyd_api/constants.py
+-rw-r--r--   0 runner    (1001) docker     (127)      128 2024-05-29 10:00:48.000000 scrapyd_api-0.0.2/scrapyd_api/exceptions.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)     5778 2024-05-29 10:00:48.000000 scrapyd_api-0.0.2/scrapyd_api/scrapyd_api.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9516 2024-05-29 10:00:48.000000 scrapyd_api-0.0.2/scrapyd_api/scrapyd_client.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-29 10:00:56.228744 scrapyd_api-0.0.2/scrapyd_api.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     2657 2024-05-29 10:00:56.000000 scrapyd_api-0.0.2/scrapyd_api.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      383 2024-05-29 10:00:56.000000 scrapyd_api-0.0.2/scrapyd_api.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-29 10:00:56.000000 scrapyd_api-0.0.2/scrapyd_api.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       23 2024-05-29 10:00:56.000000 scrapyd_api-0.0.2/scrapyd_api.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       12 2024-05-29 10:00:56.000000 scrapyd_api-0.0.2/scrapyd_api.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-29 10:00:56.000000 scrapyd_api-0.0.2/scrapyd_api.egg-info/zip-safe
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-29 10:00:56.228744 scrapyd_api-0.0.2/setup.cfg
+-rwxr-xr-x   0 runner    (1001) docker     (127)     1669 2024-05-29 10:00:48.000000 scrapyd_api-0.0.2/setup.py
```

### filetype from file(1)

```diff
@@ -1 +1 @@
-POSIX tar archive (GNU)
+POSIX tar archive
```

### Comparing `scrapyd-api-0.0.1/PKG-INFO` & `scrapyd_api-0.0.2/PKG-INFO`

 * *Files 16% similar despite different names*

```diff
@@ -1,95 +1,97 @@
 Metadata-Version: 2.1
 Name: scrapyd-api
-Version: 0.0.1
+Version: 0.0.2
 Summary: scrapyd api
 Home-page: https://github.com/mouday/scrapyd-api
 Author: Peng Shiyu
 Author-email: pengshiyuyx@gmail.com
 License: MIT
-Description: # scrapyd API
-        
-        Github: [https://github.com/mouday/scrapyd-api](https://github.com/mouday/scrapyd-api)
-        
-        Gitee: [https://gitee.com/mouday/scrapyd-api](https://gitee.com/mouday/scrapyd-api)
-        
-        Pypi: [https://pypi.org/project/scrapyd-api](https://pypi.org/project/scrapyd-api)
-        
-        
-        ## 安装
-        ```bash
-        pip install scrapyd-api
-        ```
-        
-        ## 使用示例
-        ```python
-        # -*- coding: utf-8 -*-
-        from pprint import pprint
-        
-        from scrapyd_api import ScrapydClient
-        
-        client = ScrapydClient()
-        pprint(client.daemon_status())
-        """
-        {'finished': 67,
-         'node_name': 'localhost',
-         'pending': 0,
-         'running': 0,
-         'status': 'ok',
-         'total': 67}
-        """
-        ``` 
-        
-        
-        ## 简介
-        
-        说明，基于`scrapyd 1.2.1`进行调用，如果版本差异大，可能会出现异常
-        
-        
-        ScrapydAPI对原有的Scrapyd api进行原样返回，有利于二次开发
-        
-        接口文档：[https://scrapyd.readthedocs.io/en/stable/api.html](https://scrapyd.readthedocs.io/en/stable/api.html)
-        
-        ```bash
-        class ScrapydAPI:
-            add_version
-            cancel
-            delete_project
-            delete_version
-            list_jobs
-            list_projects
-            list_spiders
-            list_versions
-            schedule
-            daemon_status
-        ```
-        
-        ScrapydClient类继承自 ScrapydAPI，对其进行了扩展和加强
-        
-        ```bash
-        class ScrapydClient(ScrapydAPI):
-            # 加强的数据接口
-            daemon_status             # 增加了返回参数 total
-            add_version               # 添加version 默认值为当前时间戳 10位
-            list_spiders              # 返回值：列表+字符串 改为 列表+字典
-            list_projects             # 返回值：列表+字符串 改为 列表+字典
-            list_versions             # 返回值：列表+字符串 改为 列表+字典  
-        
-            # 扩展的数据接口
-            job_status                # 查询任务状态
-            list_versions_format      # 格式化版本号为日期时间格式 '%Y-%m-%d %H:%M:%S'
-            list_jobs_merge           # 合并后的任务列表
-            cancel_all_project_job    # 取消所有项目下的任务
-            cancel_all_job            # 取消指定项目下的任务
-        
-            # 扩展的日志接口
-            logs                      # 获取日志-项目列表
-            project_logs              # 获取日志-爬虫列表
-            spider_logs               # 获取日志-任务列表
-            job_log                   # 获取job日志
-            
-        ```
 Keywords: spider admin
-Platform: UNKNOWN
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.6
 Description-Content-Type: text/markdown
+Requires-Dist: parsel
+Requires-Dist: session_request
+
+# scrapyd API
+
+Github: [https://github.com/mouday/scrapyd-api](https://github.com/mouday/scrapyd-api)
+
+Gitee: [https://gitee.com/mouday/scrapyd-api](https://gitee.com/mouday/scrapyd-api)
+
+Pypi: [https://pypi.org/project/scrapyd-api](https://pypi.org/project/scrapyd-api)
+
+
+## 安装
+```bash
+pip install scrapyd-api
+```
+
+## 使用示例
+```python
+# -*- coding: utf-8 -*-
+from pprint import pprint
+
+from scrapyd_api import ScrapydClient
+
+client = ScrapydClient()
+pprint(client.daemon_status())
+"""
+{'finished': 67,
+ 'node_name': 'localhost',
+ 'pending': 0,
+ 'running': 0,
+ 'status': 'ok',
+ 'total': 67}
+"""
+``` 
+
+
+## 简介
+
+说明，基于`scrapyd 1.2.1`进行调用，如果版本差异大，可能会出现异常
+
+
+ScrapydAPI对原有的Scrapyd api进行原样返回，有利于二次开发
+
+接口文档：[https://scrapyd.readthedocs.io/en/stable/api.html](https://scrapyd.readthedocs.io/en/stable/api.html)
+
+```bash
+class ScrapydAPI:
+    add_version
+    cancel
+    delete_project
+    delete_version
+    list_jobs
+    list_projects
+    list_spiders
+    list_versions
+    schedule
+    daemon_status
+```
+
+ScrapydClient类继承自 ScrapydAPI，对其进行了扩展和加强
+
+```bash
+class ScrapydClient(ScrapydAPI):
+    # 加强的数据接口
+    daemon_status             # 增加了返回参数 total
+    add_version               # 添加version 默认值为当前时间戳 10位
+    list_spiders              # 返回值：列表+字符串 改为 列表+字典
+    list_projects             # 返回值：列表+字符串 改为 列表+字典
+    list_versions             # 返回值：列表+字符串 改为 列表+字典  
+
+    # 扩展的数据接口
+    job_status                # 查询任务状态
+    list_versions_format      # 格式化版本号为日期时间格式 '%Y-%m-%d %H:%M:%S'
+    list_jobs_merge           # 合并后的任务列表
+    cancel_all_project_job    # 取消所有项目下的任务
+    cancel_all_job            # 取消指定项目下的任务
+
+    # 扩展的日志接口
+    logs                      # 获取日志-项目列表
+    project_logs              # 获取日志-爬虫列表
+    spider_logs               # 获取日志-任务列表
+    job_log                   # 获取job日志
+    
+```
```

### Comparing `scrapyd-api-0.0.1/README.md` & `scrapyd_api-0.0.2/README.md`

 * *Files identical despite different names*

### Comparing `scrapyd-api-0.0.1/scrapyd_api/scrapyd_api.py` & `scrapyd_api-0.0.2/scrapyd_api/scrapyd_api.py`

 * *Files identical despite different names*

### Comparing `scrapyd-api-0.0.1/scrapyd_api/scrapyd_client.py` & `scrapyd_api-0.0.2/scrapyd_api/scrapyd_client.py`

 * *Files 2% similar despite different names*

```diff
@@ -39,15 +39,16 @@
         else:
             response.encoding = response.apparent_encoding
 
             for error_name in self.ERROR_LIST:
 
                 if error_name in response.text:
                     msg = self._match_error_message('RuntimeError', response.text)
-                    raise ScrapydException(msg)
+                    if msg:
+                        raise ScrapydException(msg)
 
             return response.text
 
     #####################################################
     # 加强的数据接口
     #####################################################
 
@@ -310,8 +311,9 @@
             lst.append(item)
 
         return lst
 
     def _match_error_message(self, keywords, text):
         """从返回的文本中搜索报错信息"""
         match = re.search(f'{keywords}:.*', text)
-        return match.group(0)
+        if match:
+            return match.group(0)
```

### Comparing `scrapyd-api-0.0.1/scrapyd_api.egg-info/PKG-INFO` & `scrapyd_api-0.0.2/scrapyd_api.egg-info/PKG-INFO`

 * *Files 16% similar despite different names*

```diff
@@ -1,95 +1,97 @@
 Metadata-Version: 2.1
 Name: scrapyd-api
-Version: 0.0.1
+Version: 0.0.2
 Summary: scrapyd api
 Home-page: https://github.com/mouday/scrapyd-api
 Author: Peng Shiyu
 Author-email: pengshiyuyx@gmail.com
 License: MIT
-Description: # scrapyd API
-        
-        Github: [https://github.com/mouday/scrapyd-api](https://github.com/mouday/scrapyd-api)
-        
-        Gitee: [https://gitee.com/mouday/scrapyd-api](https://gitee.com/mouday/scrapyd-api)
-        
-        Pypi: [https://pypi.org/project/scrapyd-api](https://pypi.org/project/scrapyd-api)
-        
-        
-        ## 安装
-        ```bash
-        pip install scrapyd-api
-        ```
-        
-        ## 使用示例
-        ```python
-        # -*- coding: utf-8 -*-
-        from pprint import pprint
-        
-        from scrapyd_api import ScrapydClient
-        
-        client = ScrapydClient()
-        pprint(client.daemon_status())
-        """
-        {'finished': 67,
-         'node_name': 'localhost',
-         'pending': 0,
-         'running': 0,
-         'status': 'ok',
-         'total': 67}
-        """
-        ``` 
-        
-        
-        ## 简介
-        
-        说明，基于`scrapyd 1.2.1`进行调用，如果版本差异大，可能会出现异常
-        
-        
-        ScrapydAPI对原有的Scrapyd api进行原样返回，有利于二次开发
-        
-        接口文档：[https://scrapyd.readthedocs.io/en/stable/api.html](https://scrapyd.readthedocs.io/en/stable/api.html)
-        
-        ```bash
-        class ScrapydAPI:
-            add_version
-            cancel
-            delete_project
-            delete_version
-            list_jobs
-            list_projects
-            list_spiders
-            list_versions
-            schedule
-            daemon_status
-        ```
-        
-        ScrapydClient类继承自 ScrapydAPI，对其进行了扩展和加强
-        
-        ```bash
-        class ScrapydClient(ScrapydAPI):
-            # 加强的数据接口
-            daemon_status             # 增加了返回参数 total
-            add_version               # 添加version 默认值为当前时间戳 10位
-            list_spiders              # 返回值：列表+字符串 改为 列表+字典
-            list_projects             # 返回值：列表+字符串 改为 列表+字典
-            list_versions             # 返回值：列表+字符串 改为 列表+字典  
-        
-            # 扩展的数据接口
-            job_status                # 查询任务状态
-            list_versions_format      # 格式化版本号为日期时间格式 '%Y-%m-%d %H:%M:%S'
-            list_jobs_merge           # 合并后的任务列表
-            cancel_all_project_job    # 取消所有项目下的任务
-            cancel_all_job            # 取消指定项目下的任务
-        
-            # 扩展的日志接口
-            logs                      # 获取日志-项目列表
-            project_logs              # 获取日志-爬虫列表
-            spider_logs               # 获取日志-任务列表
-            job_log                   # 获取job日志
-            
-        ```
 Keywords: spider admin
-Platform: UNKNOWN
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.6
 Description-Content-Type: text/markdown
+Requires-Dist: parsel
+Requires-Dist: session_request
+
+# scrapyd API
+
+Github: [https://github.com/mouday/scrapyd-api](https://github.com/mouday/scrapyd-api)
+
+Gitee: [https://gitee.com/mouday/scrapyd-api](https://gitee.com/mouday/scrapyd-api)
+
+Pypi: [https://pypi.org/project/scrapyd-api](https://pypi.org/project/scrapyd-api)
+
+
+## 安装
+```bash
+pip install scrapyd-api
+```
+
+## 使用示例
+```python
+# -*- coding: utf-8 -*-
+from pprint import pprint
+
+from scrapyd_api import ScrapydClient
+
+client = ScrapydClient()
+pprint(client.daemon_status())
+"""
+{'finished': 67,
+ 'node_name': 'localhost',
+ 'pending': 0,
+ 'running': 0,
+ 'status': 'ok',
+ 'total': 67}
+"""
+``` 
+
+
+## 简介
+
+说明，基于`scrapyd 1.2.1`进行调用，如果版本差异大，可能会出现异常
+
+
+ScrapydAPI对原有的Scrapyd api进行原样返回，有利于二次开发
+
+接口文档：[https://scrapyd.readthedocs.io/en/stable/api.html](https://scrapyd.readthedocs.io/en/stable/api.html)
+
+```bash
+class ScrapydAPI:
+    add_version
+    cancel
+    delete_project
+    delete_version
+    list_jobs
+    list_projects
+    list_spiders
+    list_versions
+    schedule
+    daemon_status
+```
+
+ScrapydClient类继承自 ScrapydAPI，对其进行了扩展和加强
+
+```bash
+class ScrapydClient(ScrapydAPI):
+    # 加强的数据接口
+    daemon_status             # 增加了返回参数 total
+    add_version               # 添加version 默认值为当前时间戳 10位
+    list_spiders              # 返回值：列表+字符串 改为 列表+字典
+    list_projects             # 返回值：列表+字符串 改为 列表+字典
+    list_versions             # 返回值：列表+字符串 改为 列表+字典  
+
+    # 扩展的数据接口
+    job_status                # 查询任务状态
+    list_versions_format      # 格式化版本号为日期时间格式 '%Y-%m-%d %H:%M:%S'
+    list_jobs_merge           # 合并后的任务列表
+    cancel_all_project_job    # 取消所有项目下的任务
+    cancel_all_job            # 取消指定项目下的任务
+
+    # 扩展的日志接口
+    logs                      # 获取日志-项目列表
+    project_logs              # 获取日志-爬虫列表
+    spider_logs               # 获取日志-任务列表
+    job_log                   # 获取job日志
+    
+```
```

### Comparing `scrapyd-api-0.0.1/setup.py` & `scrapyd_api-0.0.2/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -46,15 +46,15 @@
 参考：
 https://packaging.python.org/guides/making-a-pypi-friendly-readme/
 
 """
 
 base_dir = os.path.dirname(os.path.abspath(__file__))
 
-version = '0.0.1'
+version = '0.0.2'
 
 with io.open("README.md", 'r', encoding='utf-8') as f:
     long_description = f.read()
 
 with io.open("requirements.txt", 'r') as f:
     install_requires = f.read().split(os.sep)
```

