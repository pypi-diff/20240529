# Comparing `tmp/chatchat-0.1.2.tar.gz` & `tmp/chatchat-0.1.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "chatchat-0.1.2.tar", last modified: Sun May 26 00:51:38 2024, max compression
+gzip compressed data, was "chatchat-0.1.3.tar", last modified: Tue May 28 23:05:00 2024, max compression
```

## Comparing `chatchat-0.1.2.tar` & `chatchat-0.1.3.tar`

### file list

```diff
@@ -1,21 +1,21 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-26 00:51:38.736480 chatchat-0.1.2/
--rw-r--r--   0 runner    (1001) docker     (127)    18092 2024-05-26 00:51:26.000000 chatchat-0.1.2/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)     1271 2024-05-26 00:51:38.736480 chatchat-0.1.2/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      752 2024-05-26 00:51:26.000000 chatchat-0.1.2/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-26 00:51:38.736480 chatchat-0.1.2/chatchat/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-26 00:51:26.000000 chatchat-0.1.2/chatchat/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1904 2024-05-26 00:51:26.000000 chatchat-0.1.2/chatchat/__main__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1876 2024-05-26 00:51:26.000000 chatchat-0.1.2/chatchat/alibaba.py
--rw-r--r--   0 runner    (1001) docker     (127)     3790 2024-05-26 00:51:26.000000 chatchat-0.1.2/chatchat/baidu.py
--rw-r--r--   0 runner    (1001) docker     (127)     1089 2024-05-26 00:51:26.000000 chatchat-0.1.2/chatchat/base.py
--rw-r--r--   0 runner    (1001) docker     (127)     4401 2024-05-26 00:51:26.000000 chatchat-0.1.2/chatchat/tencent.py
--rw-r--r--   0 runner    (1001) docker     (127)     5316 2024-05-26 00:51:26.000000 chatchat-0.1.2/chatchat/xunfei.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-26 00:51:38.736480 chatchat-0.1.2/chatchat.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     1271 2024-05-26 00:51:38.000000 chatchat-0.1.2/chatchat.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      356 2024-05-26 00:51:38.000000 chatchat-0.1.2/chatchat.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-26 00:51:38.000000 chatchat-0.1.2/chatchat.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       52 2024-05-26 00:51:38.000000 chatchat-0.1.2/chatchat.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (127)       23 2024-05-26 00:51:38.000000 chatchat-0.1.2/chatchat.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)        9 2024-05-26 00:51:38.000000 chatchat-0.1.2/chatchat.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-26 00:51:38.736480 chatchat-0.1.2/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)      891 2024-05-26 00:51:26.000000 chatchat-0.1.2/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-28 23:05:00.057630 chatchat-0.1.3/
+-rw-r--r--   0 runner    (1001) docker     (127)    18092 2024-05-28 23:04:54.000000 chatchat-0.1.3/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)     1271 2024-05-28 23:05:00.057630 chatchat-0.1.3/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      752 2024-05-28 23:04:54.000000 chatchat-0.1.3/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-28 23:05:00.057630 chatchat-0.1.3/chatchat/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-28 23:04:54.000000 chatchat-0.1.3/chatchat/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2079 2024-05-28 23:04:54.000000 chatchat-0.1.3/chatchat/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1876 2024-05-28 23:04:54.000000 chatchat-0.1.3/chatchat/alibaba.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3790 2024-05-28 23:04:54.000000 chatchat-0.1.3/chatchat/baidu.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1089 2024-05-28 23:04:54.000000 chatchat-0.1.3/chatchat/base.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4401 2024-05-28 23:04:54.000000 chatchat-0.1.3/chatchat/tencent.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5316 2024-05-28 23:04:54.000000 chatchat-0.1.3/chatchat/xunfei.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-28 23:05:00.057630 chatchat-0.1.3/chatchat.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     1271 2024-05-28 23:05:00.000000 chatchat-0.1.3/chatchat.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      356 2024-05-28 23:05:00.000000 chatchat-0.1.3/chatchat.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-28 23:05:00.000000 chatchat-0.1.3/chatchat.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       52 2024-05-28 23:05:00.000000 chatchat-0.1.3/chatchat.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       23 2024-05-28 23:05:00.000000 chatchat-0.1.3/chatchat.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        9 2024-05-28 23:05:00.000000 chatchat-0.1.3/chatchat.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-28 23:05:00.057630 chatchat-0.1.3/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)      891 2024-05-28 23:04:54.000000 chatchat-0.1.3/setup.py
```

### Comparing `chatchat-0.1.2/LICENSE` & `chatchat-0.1.3/LICENSE`

 * *Files identical despite different names*

### Comparing `chatchat-0.1.2/PKG-INFO` & `chatchat-0.1.3/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: chatchat
-Version: 0.1.2
+Version: 0.1.3
 Summary: Large Language Model API
 Home-page: https://github.com/JiauZhang/chatchat
 Author: JiauZhang
 Author-email: jiauzhang@163.com
 License: GPL-2.0
 Keywords: llm,chatapi,chatbot
 Classifier: Intended Audience :: Developers
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: chatchat Version: 0.1.2 Summary: Large Language
+Metadata-Version: 2.1 Name: chatchat Version: 0.1.3 Summary: Large Language
 Model API Home-page: https://github.com/JiauZhang/chatchat Author: JiauZhang
 Author-email: jiauzhang@163.com License: GPL-2.0 Keywords: llm,chatapi,chatbot
 Classifier: Intended Audience :: Developers Classifier: License :: OSI Approved
 :: GNU General Public License v2 (GPLv2) Classifier: Programming Language ::
 Python :: 3.8 Description-Content-Type: text/markdown License-File: LICENSE
 Requires-Dist: httpx Requires-Dist: websocket-client ### Large Language Models
 Python API - â ç¾åº¦æå¿ä¸è¨/ERNIE - â é¿ééä¹åé®/QWen - â
```

### Comparing `chatchat-0.1.2/README.md` & `chatchat-0.1.3/README.md`

 * *Files identical despite different names*

### Comparing `chatchat-0.1.2/chatchat/__main__.py` & `chatchat-0.1.3/chatchat/__main__.py`

 * *Files 11% similar despite different names*

```diff
@@ -23,48 +23,52 @@
         usage = 'Usage: chatchat config platform.key=value'
         if len(cfg) != 2:
             print(usage)
             return
 
         plat = cfg[0]
         if plat not in __platform_config__:
+            print(f'Platform <{plat}> is currently NOT supported!')
             supported_platforms()
             return
 
         kv = cfg[1].split('=')
         if len(kv) != 2:
             print(usage)
             return
         key, value = kv
 
         if key not in __platform_config__[plat]:
-            supported_platforms()
+            print(f'Platform <{plat}> do NOT has secret key <{key}>!\nYou can set the following keys:')
+            for key in __platform_config__[plat]:
+                print(f'\t{key}')
             return
 
-        home = str(pathlib.Path.home())
-        dot_filename = os.path.join(home, '.chatchat.json')
-
         util = Base()
-        dot_content = {}
-        if os.path.exists(dot_filename):
-            dot_content = util.load_json(dot_filename)
+        dot_filename = util.secret_file
+        dot_content = util.secret_data
+
         if plat in dot_content:
             dot_content[plat][key] = value
         else:
             dot_content[plat] = {key: value}
         util.write_json(dot_filename, dot_content)
 
 parser = argparse.ArgumentParser()
+parser.set_defaults(parser=None)
 subparser = parser.add_subparsers()
 
 config_parser = subparser.add_parser('config', help='config platform secret key')
 config_parser.add_argument('cfgs', type=str, nargs='?')
 config_parser.add_argument('--list', action='store_true')
 config_parser.set_defaults(parser=parse_config)
 
 args = parser.parse_args()
 
 def main():
-    args.parser(args)
+    if args.parser:
+        args.parser(args)
+    else:
+        parser.print_help()
 
 if __name__ == '__main__':
     main()
```

### Comparing `chatchat-0.1.2/chatchat/alibaba.py` & `chatchat-0.1.3/chatchat/alibaba.py`

 * *Files identical despite different names*

### Comparing `chatchat-0.1.2/chatchat/baidu.py` & `chatchat-0.1.3/chatchat/baidu.py`

 * *Files identical despite different names*

### Comparing `chatchat-0.1.2/chatchat/base.py` & `chatchat-0.1.3/chatchat/base.py`

 * *Files identical despite different names*

### Comparing `chatchat-0.1.2/chatchat/tencent.py` & `chatchat-0.1.3/chatchat/tencent.py`

 * *Files identical despite different names*

### Comparing `chatchat-0.1.2/chatchat/xunfei.py` & `chatchat-0.1.3/chatchat/xunfei.py`

 * *Files identical despite different names*

### Comparing `chatchat-0.1.2/chatchat.egg-info/PKG-INFO` & `chatchat-0.1.3/chatchat.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: chatchat
-Version: 0.1.2
+Version: 0.1.3
 Summary: Large Language Model API
 Home-page: https://github.com/JiauZhang/chatchat
 Author: JiauZhang
 Author-email: jiauzhang@163.com
 License: GPL-2.0
 Keywords: llm,chatapi,chatbot
 Classifier: Intended Audience :: Developers
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: chatchat Version: 0.1.2 Summary: Large Language
+Metadata-Version: 2.1 Name: chatchat Version: 0.1.3 Summary: Large Language
 Model API Home-page: https://github.com/JiauZhang/chatchat Author: JiauZhang
 Author-email: jiauzhang@163.com License: GPL-2.0 Keywords: llm,chatapi,chatbot
 Classifier: Intended Audience :: Developers Classifier: License :: OSI Approved
 :: GNU General Public License v2 (GPLv2) Classifier: Programming Language ::
 Python :: 3.8 Description-Content-Type: text/markdown License-File: LICENSE
 Requires-Dist: httpx Requires-Dist: websocket-client ### Large Language Models
 Python API - â ç¾åº¦æå¿ä¸è¨/ERNIE - â é¿ééä¹åé®/QWen - â
```

### Comparing `chatchat-0.1.2/setup.py` & `chatchat-0.1.3/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 from setuptools import setup, find_packages
 
 setup(
     name = 'chatchat',
     packages = find_packages(exclude=['examples']),
-    version = '0.1.2',
+    version = '0.1.3',
     license = 'GPL-2.0',
     description = 'Large Language Model API',
     author = 'JiauZhang',
     author_email = 'jiauzhang@163.com',
     url = 'https://github.com/JiauZhang/chatchat',
     long_description=open("README.md", "r", encoding="utf-8").read(),
     long_description_content_type = 'text/markdown',
```

