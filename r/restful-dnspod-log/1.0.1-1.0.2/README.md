# Comparing `tmp/restful_dnspod_log-1.0.1.tar.gz` & `tmp/restful_dnspod_log-1.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/restful_dnspod_log-1.0.1.tar", last modified: Mon Mar  4 02:20:59 2024, max compression
+gzip compressed data, was "dist/restful_dnspod_log-1.0.2.tar", last modified: Wed May 29 07:08:16 2024, max compression
```

## Comparing `restful_dnspod_log-1.0.1.tar` & `restful_dnspod_log-1.0.2.tar`

### file list

```diff
@@ -1,14 +1,14 @@
-drwxr-xr-x   0 xiaofeng   (502) staff       (20)        0 2024-03-04 02:20:59.898942 restful_dnspod_log-1.0.1/
--rw-r--r--   0 xiaofeng   (502) staff       (20)     1364 2024-03-04 02:20:59.898375 restful_dnspod_log-1.0.1/PKG-INFO
--rw-r--r--   0 xiaofeng   (502) staff       (20)      363 2024-03-01 08:30:04.000000 restful_dnspod_log-1.0.1/README.rst
-drwxr-xr-x   0 xiaofeng   (502) staff       (20)        0 2024-03-04 02:20:59.894852 restful_dnspod_log-1.0.1/restful_dnspod_log/
--rw-r--r--   0 xiaofeng   (502) staff       (20)      124 2024-03-01 08:19:10.000000 restful_dnspod_log-1.0.1/restful_dnspod_log/__init__.py
--rw-r--r--   0 xiaofeng   (502) staff       (20)     3265 2024-03-01 08:33:57.000000 restful_dnspod_log-1.0.1/restful_dnspod_log/main.py
-drwxr-xr-x   0 xiaofeng   (502) staff       (20)        0 2024-03-04 02:20:59.897769 restful_dnspod_log-1.0.1/restful_dnspod_log.egg-info/
--rw-r--r--   0 xiaofeng   (502) staff       (20)     1364 2024-03-04 02:20:59.000000 restful_dnspod_log-1.0.1/restful_dnspod_log.egg-info/PKG-INFO
--rw-r--r--   0 xiaofeng   (502) staff       (20)      286 2024-03-04 02:20:59.000000 restful_dnspod_log-1.0.1/restful_dnspod_log.egg-info/SOURCES.txt
--rw-r--r--   0 xiaofeng   (502) staff       (20)        1 2024-03-04 02:20:59.000000 restful_dnspod_log-1.0.1/restful_dnspod_log.egg-info/dependency_links.txt
--rw-r--r--   0 xiaofeng   (502) staff       (20)       51 2024-03-04 02:20:59.000000 restful_dnspod_log-1.0.1/restful_dnspod_log.egg-info/requires.txt
--rw-r--r--   0 xiaofeng   (502) staff       (20)       19 2024-03-04 02:20:59.000000 restful_dnspod_log-1.0.1/restful_dnspod_log.egg-info/top_level.txt
--rw-r--r--   0 xiaofeng   (502) staff       (20)       38 2024-03-04 02:20:59.899048 restful_dnspod_log-1.0.1/setup.cfg
--rw-r--r--   0 xiaofeng   (502) staff       (20)     1473 2024-03-04 02:20:29.000000 restful_dnspod_log-1.0.1/setup.py
+drwxr-xr-x   0 xf.shen    (502) staff       (20)        0 2024-05-29 07:08:16.000000 restful_dnspod_log-1.0.2/
+-rw-r--r--   0 xf.shen    (502) staff       (20)     1392 2024-05-29 07:08:16.000000 restful_dnspod_log-1.0.2/PKG-INFO
+-rw-r--r--   0 xf.shen    (502) staff       (20)      363 2024-05-29 07:04:31.000000 restful_dnspod_log-1.0.2/README.rst
+drwxr-xr-x   0 xf.shen    (502) staff       (20)        0 2024-05-29 07:08:16.000000 restful_dnspod_log-1.0.2/restful_dnspod_log/
+-rw-r--r--   0 xf.shen    (502) staff       (20)      124 2024-05-29 07:04:31.000000 restful_dnspod_log-1.0.2/restful_dnspod_log/__init__.py
+-rw-r--r--   0 xf.shen    (502) staff       (20)     3265 2024-05-29 07:04:31.000000 restful_dnspod_log-1.0.2/restful_dnspod_log/main.py
+drwxr-xr-x   0 xf.shen    (502) staff       (20)        0 2024-05-29 07:08:16.000000 restful_dnspod_log-1.0.2/restful_dnspod_log.egg-info/
+-rw-r--r--   0 xf.shen    (502) staff       (20)     1392 2024-05-29 07:08:16.000000 restful_dnspod_log-1.0.2/restful_dnspod_log.egg-info/PKG-INFO
+-rw-r--r--   0 xf.shen    (502) staff       (20)      286 2024-05-29 07:08:16.000000 restful_dnspod_log-1.0.2/restful_dnspod_log.egg-info/SOURCES.txt
+-rw-r--r--   0 xf.shen    (502) staff       (20)        1 2024-05-29 07:08:16.000000 restful_dnspod_log-1.0.2/restful_dnspod_log.egg-info/dependency_links.txt
+-rw-r--r--   0 xf.shen    (502) staff       (20)       74 2024-05-29 07:08:16.000000 restful_dnspod_log-1.0.2/restful_dnspod_log.egg-info/requires.txt
+-rw-r--r--   0 xf.shen    (502) staff       (20)       19 2024-05-29 07:08:16.000000 restful_dnspod_log-1.0.2/restful_dnspod_log.egg-info/top_level.txt
+-rw-r--r--   0 xf.shen    (502) staff       (20)       38 2024-05-29 07:08:16.000000 restful_dnspod_log-1.0.2/setup.cfg
+-rw-r--r--   0 xf.shen    (502) staff       (20)     1499 2024-05-29 07:06:30.000000 restful_dnspod_log-1.0.2/setup.py
```

### filetype from file(1)

```diff
@@ -1 +1 @@
-POSIX tar archive
+POSIX tar archive (GNU)
```

### Comparing `restful_dnspod_log-1.0.1/PKG-INFO` & `restful_dnspod_log-1.0.2/PKG-INFO`

 * *Files 7% similar despite different names*

```diff
@@ -1,37 +1,35 @@
-Metadata-Version: 2.1
+Metadata-Version: 1.1
 Name: restful_dnspod_log
-Version: 1.0.1
+Version: 1.0.2
 Summary: return the log for dns resolution
 Home-page: https://github.com/hanyan007/RESTful_DNSPOD_LOG.git
 Author: hanyan_news
 Author-email: hanyan0572@gmail.com
 License: BSD License
 Project-URL: Source, https://github.com/hanyan007/RESTful_DNSPOD_LOG.git
+Description: 
+        ========
+        工程说明
+        ========
+        
+        DNSPod 提供域名一站式服务，包括域名注册、DNS 管理、SSL 证书、网站备案等，您都可以在这方便、快捷的管理这一切，而且大部分服务是免费的。
+        
+        - 链接 https://www.dnspod.cn/
+        
+        - FLask+ Python2.7
+        
+        - 使用base64.b64encode 加密生成token，再调用dnspod API，查看解析log
+        
 Platform: all
 Classifier: Intended Audience :: Developers
 Classifier: Operating System :: OS Independent
 Classifier: Natural Language :: Chinese (Simplified)
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 2
 Classifier: Programming Language :: Python :: 2.7
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.5
 Classifier: Programming Language :: Python :: 3.6
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Topic :: Software Development :: Libraries
-Requires-Dist: package-tea-hanyan==1.0.2
-Requires-Dist: dnspod-domain-log==1.0.2
-
-
-========
-工程说明
-========
-
-DNSPod 提供域名一站式服务，包括域名注册、DNS 管理、SSL 证书、网站备案等，您都可以在这方便、快捷的管理这一切，而且大部分服务是免费的。
-
-- 链接 https://www.dnspod.cn/
-
-- FLask+ Python2.7
-
-- 使用base64.b64encode 加密生成token，再调用dnspod API，查看解析log
```

### Comparing `restful_dnspod_log-1.0.1/restful_dnspod_log/main.py` & `restful_dnspod_log-1.0.2/restful_dnspod_log/main.py`

 * *Files identical despite different names*

### Comparing `restful_dnspod_log-1.0.1/restful_dnspod_log.egg-info/PKG-INFO` & `restful_dnspod_log-1.0.2/restful_dnspod_log.egg-info/PKG-INFO`

 * *Files 16% similar despite different names*

```diff
@@ -1,37 +1,35 @@
-Metadata-Version: 2.1
-Name: restful_dnspod_log
-Version: 1.0.1
+Metadata-Version: 1.1
+Name: restful-dnspod-log
+Version: 1.0.2
 Summary: return the log for dns resolution
 Home-page: https://github.com/hanyan007/RESTful_DNSPOD_LOG.git
 Author: hanyan_news
 Author-email: hanyan0572@gmail.com
 License: BSD License
 Project-URL: Source, https://github.com/hanyan007/RESTful_DNSPOD_LOG.git
+Description: 
+        ========
+        工程说明
+        ========
+        
+        DNSPod 提供域名一站式服务，包括域名注册、DNS 管理、SSL 证书、网站备案等，您都可以在这方便、快捷的管理这一切，而且大部分服务是免费的。
+        
+        - 链接 https://www.dnspod.cn/
+        
+        - FLask+ Python2.7
+        
+        - 使用base64.b64encode 加密生成token，再调用dnspod API，查看解析log
+        
 Platform: all
 Classifier: Intended Audience :: Developers
 Classifier: Operating System :: OS Independent
 Classifier: Natural Language :: Chinese (Simplified)
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 2
 Classifier: Programming Language :: Python :: 2.7
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.5
 Classifier: Programming Language :: Python :: 3.6
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Topic :: Software Development :: Libraries
-Requires-Dist: package-tea-hanyan==1.0.2
-Requires-Dist: dnspod-domain-log==1.0.2
-
-
-========
-工程说明
-========
-
-DNSPod 提供域名一站式服务，包括域名注册、DNS 管理、SSL 证书、网站备案等，您都可以在这方便、快捷的管理这一切，而且大部分服务是免费的。
-
-- 链接 https://www.dnspod.cn/
-
-- FLask+ Python2.7
-
-- 使用base64.b64encode 加密生成token，再调用dnspod API，查看解析log
```

### Comparing `restful_dnspod_log-1.0.1/setup.py` & `restful_dnspod_log-1.0.2/setup.py`

 * *Files 7% similar despite different names*

```diff
@@ -10,24 +10,24 @@
 
 
 with open("README.rst", "r") as f:
   long_description = f.read()
 
 
 setup(name='restful_dnspod_log',  # 包名
-      version='1.0.1',  # 版本号
+      version='1.0.2',  # 版本号
       description='return the log for dns resolution',
       long_description=long_description,
       author='hanyan_news',
       author_email='hanyan0572@gmail.com',
       url='https://github.com/hanyan007/RESTful_DNSPOD_LOG.git',
       project_urls={  # Optional
           "Source": 'https://github.com/hanyan007/RESTful_DNSPOD_LOG.git',
       },
-      install_requires=["package-tea-hanyan==1.0.2", "dnspod-domain-log==1.0.2"],
+      install_requires=["package-tea-hanyan==1.0.4", "dnspod-domain-log==1.0.2", "package-tea-one==1.0.0"],
       license='BSD License',
       packages=find_packages(),
       platforms=["all"],
       classifiers=[
           'Intended Audience :: Developers',
           'Operating System :: OS Independent',
           'Natural Language :: Chinese (Simplified)',
```

