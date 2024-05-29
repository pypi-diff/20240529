# Comparing `tmp/zsx_pack-1.0.0.tar.gz` & `tmp/zsx_pack-1.0.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "zsx_pack-1.0.0.tar", last modified: Sun Apr  7 03:38:47 2024, max compression
+gzip compressed data, was "zsx_pack-1.0.1.tar", last modified: Wed May 29 08:39:57 2024, max compression
```

## Comparing `zsx_pack-1.0.0.tar` & `zsx_pack-1.0.1.tar`

### file list

```diff
@@ -1,15 +1,16 @@
-drwxrwxrwx   0        0        0        0 2024-04-07 03:38:47.214203 zsx_pack-1.0.0/
--rw-rw-rw-   0        0        0     1091 2024-04-03 09:09:05.000000 zsx_pack-1.0.0/LICENSE.txt
--rw-rw-rw-   0        0        0     1587 2024-04-07 03:38:47.210168 zsx_pack-1.0.0/PKG-INFO
--rw-rw-rw-   0        0        0      984 2024-04-07 01:39:14.000000 zsx_pack-1.0.0/README.md
-drwxrwxrwx   0        0        0        0 2024-04-07 03:38:47.192202 zsx_pack-1.0.0/logger/
--rw-rw-rw-   0        0        0      171 2024-04-03 09:06:53.000000 zsx_pack-1.0.0/logger/__init__.py
--rw-rw-rw-   0        0        0    17681 2024-04-03 09:04:55.000000 zsx_pack-1.0.0/logger/logger.py
-drwxrwxrwx   0        0        0        0 2024-04-07 03:38:47.207169 zsx_pack-1.0.0/logger/zsx_pack.egg-info/
--rw-rw-rw-   0        0        0     1587 2024-04-07 03:38:47.000000 zsx_pack-1.0.0/logger/zsx_pack.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      237 2024-04-07 03:38:47.000000 zsx_pack-1.0.0/logger/zsx_pack.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-04-07 03:38:47.000000 zsx_pack-1.0.0/logger/zsx_pack.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       16 2024-04-07 03:38:47.000000 zsx_pack-1.0.0/logger/zsx_pack.egg-info/top_level.txt
--rw-rw-rw-   0        0        0      135 2024-04-03 09:58:39.000000 zsx_pack-1.0.0/pyproject.toml
--rw-rw-rw-   0        0        0       42 2024-04-07 03:38:47.214203 zsx_pack-1.0.0/setup.cfg
--rw-rw-rw-   0        0        0     1022 2024-04-07 03:38:44.000000 zsx_pack-1.0.0/setup.py
+drwxrwxrwx   0        0        0        0 2024-05-29 08:39:57.668409 zsx_pack-1.0.1/
+-rw-rw-rw-   0        0        0     1091 2024-04-03 09:09:05.000000 zsx_pack-1.0.1/LICENSE.txt
+-rw-rw-rw-   0        0        0     1825 2024-05-29 08:39:57.665378 zsx_pack-1.0.1/PKG-INFO
+-rw-rw-rw-   0        0        0      984 2024-04-07 01:39:14.000000 zsx_pack-1.0.1/README.md
+drwxrwxrwx   0        0        0        0 2024-05-29 08:39:57.630378 zsx_pack-1.0.1/logger/
+-rw-rw-rw-   0        0        0      171 2024-04-03 09:06:53.000000 zsx_pack-1.0.1/logger/__init__.py
+-rw-rw-rw-   0        0        0    17738 2024-04-16 01:12:48.000000 zsx_pack-1.0.1/logger/logger.py
+-rw-rw-rw-   0        0        0      135 2024-04-03 09:58:39.000000 zsx_pack-1.0.1/pyproject.toml
+-rw-rw-rw-   0        0        0       42 2024-05-29 08:39:57.668409 zsx_pack-1.0.1/setup.cfg
+-rw-rw-rw-   0        0        0     2079 2024-05-29 08:31:54.000000 zsx_pack-1.0.1/setup.py
+drwxrwxrwx   0        0        0        0 2024-05-29 08:39:57.659378 zsx_pack-1.0.1/zsx_pack.egg-info/
+-rw-rw-rw-   0        0        0     1825 2024-05-29 08:39:57.000000 zsx_pack-1.0.1/zsx_pack.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      240 2024-05-29 08:39:57.000000 zsx_pack-1.0.1/zsx_pack.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-05-29 08:39:57.000000 zsx_pack-1.0.1/zsx_pack.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       16 2024-05-29 08:39:57.000000 zsx_pack-1.0.1/zsx_pack.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        7 2024-05-29 08:39:57.000000 zsx_pack-1.0.1/zsx_pack.egg-info/top_level.txt
```

### Comparing `zsx_pack-1.0.0/LICENSE.txt` & `zsx_pack-1.0.1/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `zsx_pack-1.0.0/PKG-INFO` & `zsx_pack-1.0.1/PKG-INFO`

 * *Files 12% similar despite different names*

```diff
@@ -1,22 +1,30 @@
 Metadata-Version: 2.1
 Name: zsx_pack
-Version: 1.0.0
+Version: 1.0.1
 Summary: 自用包，主要是为了logger无法屏蔽第三方包日志而开发的
 Home-page: https://github.com/ziyueguyi/zsx_pack
 Author: zsx
 Author-email: 17630583910@163.com
+Maintainer: zsx
+Maintainer-email: 17630583910@163.com
+License: MIT
 Project-URL: Bug Tracker, https://github.com/ziyueguyi/zsx_pack
-Classifier: Programming Language :: Python :: 3
+Platform: Windows
+Platform: Linux
+Classifier: Development Status :: 3 - Alpha
+Classifier: Intended Audience :: Developers
+Classifier: Topic :: Software Development :: Build Tools
 Classifier: License :: OSI Approved :: MIT License
-Classifier: Operating System :: OS Independent
 Classifier: Natural Language :: Chinese (Simplified)
+Classifier: Programming Language :: Python :: 3
 Requires-Python: >=3.6
 Description-Content-Type: text/markdown
 License-File: LICENSE.txt
+Requires-Dist: colorama>=0.4.6
 
 # Example Package
 
 #在此文件内，可使用markdown撰写对包的详细介绍和说明，便于别人熟悉和使用，在此不再赘述
 This is a simple example package. You can use
 [Github-flavored Markdown](https://github.com/ziyueguyi/zsx_pack)
 本函数主要作用是开发一个日志系统，本日志系统不使用logger包，可以有效屏蔽第三方日志信息，
```

### Comparing `zsx_pack-1.0.0/README.md` & `zsx_pack-1.0.1/README.md`

 * *Files identical despite different names*

### Comparing `zsx_pack-1.0.0/logger/logger.py` & `zsx_pack-1.0.1/logger/logger.py`

 * *Files 1% similar despite different names*

```diff
@@ -531,16 +531,17 @@
         严重的错误
         :param message:
         :param extra:
         :return:
         """
         self.__format_message(self.__log_level.critical, message, extra)
 
-    def exception(self, message, extra=None):
+    def exception(self, message, extra=None, exc_info=Exception):
         """
         严重的错误
         :param message:
         :param extra:
+        :param exc_info:异常类型
         :return:
         """
         self.__format_message(self.__log_level.critical, message, extra)
-        raise Exception(message)
+        raise exc_info(message)
```

### Comparing `zsx_pack-1.0.0/logger/zsx_pack.egg-info/PKG-INFO` & `zsx_pack-1.0.1/zsx_pack.egg-info/PKG-INFO`

 * *Files 12% similar despite different names*

```diff
@@ -1,22 +1,30 @@
 Metadata-Version: 2.1
 Name: zsx_pack
-Version: 1.0.0
+Version: 1.0.1
 Summary: 自用包，主要是为了logger无法屏蔽第三方包日志而开发的
 Home-page: https://github.com/ziyueguyi/zsx_pack
 Author: zsx
 Author-email: 17630583910@163.com
+Maintainer: zsx
+Maintainer-email: 17630583910@163.com
+License: MIT
 Project-URL: Bug Tracker, https://github.com/ziyueguyi/zsx_pack
-Classifier: Programming Language :: Python :: 3
+Platform: Windows
+Platform: Linux
+Classifier: Development Status :: 3 - Alpha
+Classifier: Intended Audience :: Developers
+Classifier: Topic :: Software Development :: Build Tools
 Classifier: License :: OSI Approved :: MIT License
-Classifier: Operating System :: OS Independent
 Classifier: Natural Language :: Chinese (Simplified)
+Classifier: Programming Language :: Python :: 3
 Requires-Python: >=3.6
 Description-Content-Type: text/markdown
 License-File: LICENSE.txt
+Requires-Dist: colorama>=0.4.6
 
 # Example Package
 
 #在此文件内，可使用markdown撰写对包的详细介绍和说明，便于别人熟悉和使用，在此不再赘述
 This is a simple example package. You can use
 [Github-flavored Markdown](https://github.com/ziyueguyi/zsx_pack)
 本函数主要作用是开发一个日志系统，本日志系统不使用logger包，可以有效屏蔽第三方日志信息，
```

