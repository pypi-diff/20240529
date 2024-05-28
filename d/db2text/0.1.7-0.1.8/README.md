# Comparing `tmp/db2text-0.1.7.tar.gz` & `tmp/db2text-0.1.8.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "db2text-0.1.7.tar", last modified: Wed Jan 10 12:03:30 2024, max compression
+gzip compressed data, was "db2text-0.1.8.tar", last modified: Sun Jan 28 13:58:13 2024, max compression
```

## Comparing `db2text-0.1.7.tar` & `db2text-0.1.8.tar`

### file list

```diff
@@ -1,27 +1,25 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-01-10 12:03:30.000000 db2text-0.1.7/
--rwxr--r--   0 root         (0) root         (0)     1063 2021-03-12 13:21:32.000000 db2text-0.1.7/LICENSE
--rwxr--r--   0 root         (0) root         (0)       44 2021-06-03 14:29:28.000000 db2text-0.1.7/MANIFEST.in
--rw-r--r--   0 root         (0) root         (0)      553 2024-01-10 12:03:30.000000 db2text-0.1.7/PKG-INFO
--rwxr--r--   0 root         (0) root         (0)      154 2021-03-14 10:39:32.000000 db2text-0.1.7/README.md
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-01-10 12:03:30.000000 db2text-0.1.7/bin/
--rwxr--r--   0 root         (0) root         (0)     1862 2021-07-28 13:44:51.000000 db2text-0.1.7/bin/dbt
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-01-10 12:03:30.000000 db2text-0.1.7/database2text/
--rwxr--r--   0 root         (0) root         (0)        0 2020-03-05 08:42:50.000000 db2text-0.1.7/database2text/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-01-10 12:03:30.000000 db2text-0.1.7/database2text/datafile/
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-01-10 12:03:30.000000 db2text-0.1.7/database2text/datafile/sample/
--rwxr--r--   0 root         (0) root         (0)      988 2021-07-12 14:11:19.000000 db2text-0.1.7/database2text/datafile/sample/dbt_oracle11.txt
--rwxr--r--   0 root         (0) root         (0)     4807 2024-01-09 03:24:09.000000 db2text-0.1.7/database2text/datafile/usermenual.md
--rwxrw-rw-   0 root         (0) root         (0)     2002 2024-01-09 11:48:50.000000 db2text-0.1.7/database2text/dbt.py
--rwxr--r--   0 root         (0) root         (0)     1363 2022-03-25 06:10:04.000000 db2text-0.1.7/database2text/mysql.py
--rwxr--r--   0 root         (0) root         (0)     6328 2023-09-08 06:12:36.000000 db2text-0.1.7/database2text/oracle11.py
--rwxr--r--   0 root         (0) root         (0)     6001 2024-01-09 12:19:57.000000 db2text-0.1.7/database2text/tool.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-01-10 12:03:30.000000 db2text-0.1.7/db2text.egg-info/
--rwxr--r--   0 root         (0) root         (0)      553 2024-01-10 12:03:30.000000 db2text-0.1.7/db2text.egg-info/PKG-INFO
--rwxr--r--   0 root         (0) root         (0)      466 2024-01-10 12:03:30.000000 db2text-0.1.7/db2text.egg-info/SOURCES.txt
--rwxr--r--   0 root         (0) root         (0)        1 2024-01-10 12:03:30.000000 db2text-0.1.7/db2text.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)       47 2024-01-10 12:03:30.000000 db2text-0.1.7/db2text.egg-info/entry_points.txt
--rwxr--r--   0 root         (0) root         (0)        1 2021-06-03 14:11:16.000000 db2text-0.1.7/db2text.egg-info/not-zip-safe
--rw-r--r--   0 root         (0) root         (0)        7 2024-01-10 12:03:30.000000 db2text-0.1.7/db2text.egg-info/requires.txt
--rwxr--r--   0 root         (0) root         (0)       14 2024-01-10 12:03:30.000000 db2text-0.1.7/db2text.egg-info/top_level.txt
--rw-r--r--   0 root         (0) root         (0)       38 2024-01-10 12:03:30.000000 db2text-0.1.7/setup.cfg
--rwxr-xr-x   0 root         (0) root         (0)      940 2023-12-18 13:21:58.000000 db2text-0.1.7/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-01-28 13:58:13.000000 db2text-0.1.8/
+-rwxr--r--   0 root         (0) root         (0)     1063 2021-03-12 13:21:32.000000 db2text-0.1.8/LICENSE
+-rwxr--r--   0 root         (0) root         (0)       44 2021-06-03 14:29:28.000000 db2text-0.1.8/MANIFEST.in
+-rw-r--r--   0 root         (0) root         (0)      553 2024-01-28 13:58:13.000000 db2text-0.1.8/PKG-INFO
+-rwxr--r--   0 root         (0) root         (0)      154 2021-03-14 10:39:32.000000 db2text-0.1.8/README.md
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-01-28 13:58:13.000000 db2text-0.1.8/database2text/
+-rwxr--r--   0 root         (0) root         (0)        0 2020-03-05 08:42:50.000000 db2text-0.1.8/database2text/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-01-28 13:58:13.000000 db2text-0.1.8/database2text/datafile/
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-01-28 13:58:13.000000 db2text-0.1.8/database2text/datafile/sample/
+-rwxr--r--   0 root         (0) root         (0)      988 2021-07-12 14:11:19.000000 db2text-0.1.8/database2text/datafile/sample/dbt_oracle11.txt
+-rwxr--r--   0 root         (0) root         (0)     4807 2024-01-09 03:24:09.000000 db2text-0.1.8/database2text/datafile/usermenual.md
+-rwxrw-rw-   0 root         (0) root         (0)     2101 2024-01-28 13:52:59.000000 db2text-0.1.8/database2text/dbt.py
+-rwxr--r--   0 root         (0) root         (0)     1363 2022-03-25 06:10:04.000000 db2text-0.1.8/database2text/mysql.py
+-rwxr--r--   0 root         (0) root         (0)     6328 2023-09-08 06:12:36.000000 db2text-0.1.8/database2text/oracle11.py
+-rwxr--r--   0 root         (0) root         (0)     6001 2024-01-09 12:19:57.000000 db2text-0.1.8/database2text/tool.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-01-28 13:58:13.000000 db2text-0.1.8/db2text.egg-info/
+-rwxr--r--   0 root         (0) root         (0)      553 2024-01-28 13:58:13.000000 db2text-0.1.8/db2text.egg-info/PKG-INFO
+-rwxr--r--   0 root         (0) root         (0)      458 2024-01-28 13:58:13.000000 db2text-0.1.8/db2text.egg-info/SOURCES.txt
+-rwxr--r--   0 root         (0) root         (0)        1 2024-01-28 13:58:13.000000 db2text-0.1.8/db2text.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)       47 2024-01-28 13:58:13.000000 db2text-0.1.8/db2text.egg-info/entry_points.txt
+-rwxr--r--   0 root         (0) root         (0)        1 2021-06-03 14:11:16.000000 db2text-0.1.8/db2text.egg-info/not-zip-safe
+-rw-r--r--   0 root         (0) root         (0)        7 2024-01-28 13:58:13.000000 db2text-0.1.8/db2text.egg-info/requires.txt
+-rwxr--r--   0 root         (0) root         (0)       14 2024-01-28 13:58:13.000000 db2text-0.1.8/db2text.egg-info/top_level.txt
+-rw-r--r--   0 root         (0) root         (0)       38 2024-01-28 13:58:13.000000 db2text-0.1.8/setup.cfg
+-rwxr-xr-x   0 root         (0) root         (0)      940 2024-01-10 12:03:30.000000 db2text-0.1.8/setup.py
```

### Comparing `db2text-0.1.7/LICENSE` & `db2text-0.1.8/LICENSE`

 * *Files identical despite different names*

### Comparing `db2text-0.1.7/PKG-INFO` & `db2text-0.1.8/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: db2text
-Version: 0.1.7
+Version: 0.1.8
 Summary: database to text
 Home-page: https://gitee.com/chenc224/dbt
 Author: Chen chuan
 Author-email: kcchen@139.com
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

### Comparing `db2text-0.1.7/bin/dbt` & `db2text-0.1.8/database2text/dbt.py`

 * *Files 8% similar despite different names*

```diff
@@ -12,27 +12,33 @@
         fn="dbt.txt"
         if len(sys.argv)>1:
             fn=sys.argv[1]
         if not os.path.isfile(fn):
             print("can't open %s. you must create it or tell us another file name." %(fn))
             print("for help, you may need the file in %s" %(os.path.join(os.path.dirname(os.path.abspath(dbtt.__file__)),"datafile")))
             sys.exit(-1)
-        f=open(fn)
+        f=open(fn,"rb")
         section="global"
+        文件编码="utf8"
+        dbt=""
         for s in f.readlines():
+            s=s.decode(文件编码)
+            print(s)
             if s.startswith(":"):
                 if section=="end":
                     break
                 if section=="global":
-                    driver=stdata["driver"]
+                    文件编码=stdata.get("coding") or 文件编码
+                if section in ["connect","global"] and "driver" in stdata:
                     dbt=importlib.import_module('database2text.%s' %(stdata["driver"]))
-                if not dbt:
-                    print("can't find driver=xxx , need it in begin of config's file")
-                    sys.exit(-1)
+                    stdata.pop("driver")
                 if section!="global":
+                    if not dbt:
+                        print("需要在配置文件里设置driver")
+                        sys.exit(-1)
                     if hasattr(dbt,section):
                         getattr(dbt,section)()
                     elif hasattr(dbtt,section):
                         getattr(dbtt,section)()
                     else:
                         print("can't find function %s in driver %s and dbtt" %(section,driver))
                         sys.exit(-2)
```

#### encoding

```diff
@@ -1 +1 @@
-us-ascii
+utf-8
```

### Comparing `db2text-0.1.7/database2text/datafile/sample/dbt_oracle11.txt` & `db2text-0.1.8/database2text/datafile/sample/dbt_oracle11.txt`

 * *Files identical despite different names*

### Comparing `db2text-0.1.7/database2text/datafile/usermenual.md` & `db2text-0.1.8/database2text/datafile/usermenual.md`

 * *Files identical despite different names*

### Comparing `db2text-0.1.7/database2text/mysql.py` & `db2text-0.1.8/database2text/mysql.py`

 * *Files identical despite different names*

### Comparing `db2text-0.1.7/database2text/oracle11.py` & `db2text-0.1.8/database2text/oracle11.py`

 * *Files identical despite different names*

### Comparing `db2text-0.1.7/database2text/tool.py` & `db2text-0.1.8/database2text/tool.py`

 * *Files identical despite different names*

### Comparing `db2text-0.1.7/db2text.egg-info/PKG-INFO` & `db2text-0.1.8/db2text.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: db2text
-Version: 0.1.7
+Version: 0.1.8
 Summary: database to text
 Home-page: https://gitee.com/chenc224/dbt
 Author: Chen chuan
 Author-email: kcchen@139.com
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

### Comparing `db2text-0.1.7/setup.py` & `db2text-0.1.8/setup.py`

 * *Files 12% similar despite different names*

```diff
@@ -4,15 +4,15 @@
 import setuptools,distutils,shutil,re,os
 
 with open("README.md", "r",encoding='utf-8') as fh:
     long_description = fh.read()
 
 setuptools.setup(
     name="db2text",
-    version="0.1.7",
+    version="0.1.8",
     author="Chen chuan",
     author_email="kcchen@139.com",
     description="database to text",
     long_description=long_description,
     long_description_content_type="text/markdown",
     url="https://gitee.com/chenc224/dbt",
     packages=setuptools.find_packages(),
```

