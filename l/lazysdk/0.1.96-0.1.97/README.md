# Comparing `tmp/lazysdk-0.1.96.tar.gz` & `tmp/lazysdk-0.1.97.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "lazysdk-0.1.96.tar", last modified: Tue May 28 09:19:46 2024, max compression
+gzip compressed data, was "lazysdk-0.1.97.tar", last modified: Tue May 28 10:42:54 2024, max compression
```

## Comparing `lazysdk-0.1.96.tar` & `lazysdk-0.1.97.tar`

### file list

```diff
@@ -1,47 +1,47 @@
-drwxr-xr-x   0 zeroseeker   (501) staff       (20)        0 2024-05-28 09:19:46.138380 lazysdk-0.1.96/
--rw-r--r--   0 zeroseeker   (501) staff       (20)     1088 2023-12-14 08:15:44.000000 lazysdk-0.1.96/LICENSE
--rw-r--r--   0 zeroseeker   (501) staff       (20)     1898 2024-05-28 09:19:46.138159 lazysdk-0.1.96/PKG-INFO
--rw-r--r--   0 zeroseeker   (501) staff       (20)     1073 2023-12-30 02:37:03.000000 lazysdk-0.1.96/README.md
-drwxr-xr-x   0 zeroseeker   (501) staff       (20)        0 2024-05-28 09:19:46.137003 lazysdk-0.1.96/lazysdk/
--rw-r--r--   0 zeroseeker   (501) staff       (20)      184 2023-12-14 08:15:44.000000 lazysdk-0.1.96/lazysdk/__init__.py
--rw-r--r--   0 zeroseeker   (501) staff       (20)      389 2023-12-14 08:15:44.000000 lazysdk-0.1.96/lazysdk/lazyCrypto.py
--rw-r--r--   0 zeroseeker   (501) staff       (20)     2797 2023-12-14 08:15:44.000000 lazysdk-0.1.96/lazysdk/lazy_id_card.py
--rw-r--r--   0 zeroseeker   (501) staff       (20)      669 2023-12-14 08:15:44.000000 lazysdk-0.1.96/lazysdk/lazybase64.py
--rw-r--r--   0 zeroseeker   (501) staff       (20)      571 2024-02-02 03:54:22.000000 lazysdk-0.1.96/lazysdk/lazycache.py
--rw-r--r--   0 zeroseeker   (501) staff       (20)    15383 2023-12-25 11:22:47.000000 lazysdk-0.1.96/lazysdk/lazychromedriver.py
--rw-r--r--   0 zeroseeker   (501) staff       (20)      414 2024-02-01 03:07:43.000000 lazysdk-0.1.96/lazysdk/lazydecode.py
--rw-r--r--   0 zeroseeker   (501) staff       (20)     8883 2024-01-09 11:35:26.000000 lazysdk-0.1.96/lazysdk/lazydict.py
--rw-r--r--   0 zeroseeker   (501) staff       (20)     3024 2023-12-14 08:15:44.000000 lazysdk-0.1.96/lazysdk/lazyenv.py
--rw-r--r--   0 zeroseeker   (501) staff       (20)    15835 2024-02-02 07:00:02.000000 lazysdk-0.1.96/lazysdk/lazyexcel.py
--rw-r--r--   0 zeroseeker   (501) staff       (20)    20263 2024-02-04 08:23:46.000000 lazysdk-0.1.96/lazysdk/lazyfile.py
--rw-r--r--   0 zeroseeker   (501) staff       (20)      727 2023-12-14 08:15:44.000000 lazysdk-0.1.96/lazysdk/lazyflask.py
--rw-r--r--   0 zeroseeker   (501) staff       (20)     2403 2024-05-09 08:02:54.000000 lazysdk-0.1.96/lazysdk/lazyhtml.py
--rw-r--r--   0 zeroseeker   (501) staff       (20)     1388 2024-05-08 00:15:57.000000 lazysdk-0.1.96/lazysdk/lazyid.py
--rw-r--r--   0 zeroseeker   (501) staff       (20)     3673 2023-12-14 08:15:44.000000 lazysdk-0.1.96/lazysdk/lazyinfo.py
--rw-r--r--   0 zeroseeker   (501) staff       (20)     1364 2023-12-14 08:15:44.000000 lazysdk-0.1.96/lazysdk/lazyip.py
--rw-r--r--   0 zeroseeker   (501) staff       (20)      867 2024-01-18 03:56:02.000000 lazysdk-0.1.96/lazysdk/lazyjson.py
--rw-r--r--   0 zeroseeker   (501) staff       (20)      363 2024-04-24 09:30:41.000000 lazysdk-0.1.96/lazysdk/lazylist.py
--rw-r--r--   0 zeroseeker   (501) staff       (20)    31937 2023-12-14 08:15:44.000000 lazysdk-0.1.96/lazysdk/lazym3u8.py
--rw-r--r--   0 zeroseeker   (501) staff       (20)     1112 2023-12-14 08:15:44.000000 lazysdk-0.1.96/lazysdk/lazymd5.py
--rw-r--r--   0 zeroseeker   (501) staff       (20)     6052 2024-05-28 09:17:29.000000 lazysdk-0.1.96/lazysdk/lazypath.py
--rw-r--r--   0 zeroseeker   (501) staff       (20)    17702 2023-12-14 08:15:44.000000 lazysdk-0.1.96/lazysdk/lazyprocess.py
--rw-r--r--   0 zeroseeker   (501) staff       (20)      546 2023-12-14 08:15:44.000000 lazysdk-0.1.96/lazysdk/lazyproxies.py
--rw-r--r--   0 zeroseeker   (501) staff       (20)     1420 2023-12-14 08:15:44.000000 lazysdk-0.1.96/lazysdk/lazyrandom.py
--rw-r--r--   0 zeroseeker   (501) staff       (20)    37918 2023-12-14 08:15:44.000000 lazysdk-0.1.96/lazysdk/lazyredis.py
--rw-r--r--   0 zeroseeker   (501) staff       (20)     3750 2023-12-14 08:15:44.000000 lazysdk-0.1.96/lazysdk/lazyrequests.py
--rw-r--r--   0 zeroseeker   (501) staff       (20)     2627 2024-03-22 06:24:43.000000 lazysdk-0.1.96/lazysdk/lazytext.py
--rw-r--r--   0 zeroseeker   (501) staff       (20)    26530 2024-02-02 08:29:53.000000 lazysdk-0.1.96/lazysdk/lazytime.py
--rw-r--r--   0 zeroseeker   (501) staff       (20)     4827 2023-12-14 08:15:44.000000 lazysdk-0.1.96/lazysdk/lazyua.py
--rw-r--r--   0 zeroseeker   (501) staff       (20)     1550 2023-12-14 08:15:44.000000 lazysdk-0.1.96/lazysdk/lazyurl.py
--rw-r--r--   0 zeroseeker   (501) staff       (20)     8937 2024-05-07 04:00:07.000000 lazysdk-0.1.96/lazysdk/lazywebhook.py
--rw-r--r--   0 zeroseeker   (501) staff       (20)      716 2023-12-14 08:15:44.000000 lazysdk-0.1.96/lazysdk/lazywifi.py
--rw-r--r--   0 zeroseeker   (501) staff       (20)      770 2024-03-22 06:19:36.000000 lazysdk-0.1.96/lazysdk/lazyxml.py
--rw-r--r--   0 zeroseeker   (501) staff       (20)     1683 2023-12-26 07:19:36.000000 lazysdk-0.1.96/lazysdk/showdata.py
-drwxr-xr-x   0 zeroseeker   (501) staff       (20)        0 2024-05-28 09:19:46.137896 lazysdk-0.1.96/lazysdk.egg-info/
--rw-r--r--   0 zeroseeker   (501) staff       (20)     1898 2024-05-28 09:19:46.000000 lazysdk-0.1.96/lazysdk.egg-info/PKG-INFO
--rw-r--r--   0 zeroseeker   (501) staff       (20)      887 2024-05-28 09:19:46.000000 lazysdk-0.1.96/lazysdk.egg-info/SOURCES.txt
--rw-r--r--   0 zeroseeker   (501) staff       (20)        1 2024-05-28 09:19:46.000000 lazysdk-0.1.96/lazysdk.egg-info/dependency_links.txt
--rw-r--r--   0 zeroseeker   (501) staff       (20)      216 2024-05-28 09:19:46.000000 lazysdk-0.1.96/lazysdk.egg-info/requires.txt
--rw-r--r--   0 zeroseeker   (501) staff       (20)        8 2024-05-28 09:19:46.000000 lazysdk-0.1.96/lazysdk.egg-info/top_level.txt
--rw-r--r--   0 zeroseeker   (501) staff       (20)       38 2024-05-28 09:19:46.138424 lazysdk-0.1.96/setup.cfg
--rw-r--r--   0 zeroseeker   (501) staff       (20)     1208 2024-05-28 09:19:01.000000 lazysdk-0.1.96/setup.py
+drwxr-xr-x   0 zeroseeker   (501) staff       (20)        0 2024-05-28 10:42:54.547576 lazysdk-0.1.97/
+-rw-r--r--   0 zeroseeker   (501) staff       (20)     1088 2023-12-14 08:15:44.000000 lazysdk-0.1.97/LICENSE
+-rw-r--r--   0 zeroseeker   (501) staff       (20)     1898 2024-05-28 10:42:54.547355 lazysdk-0.1.97/PKG-INFO
+-rw-r--r--   0 zeroseeker   (501) staff       (20)     1073 2023-12-30 02:37:03.000000 lazysdk-0.1.97/README.md
+drwxr-xr-x   0 zeroseeker   (501) staff       (20)        0 2024-05-28 10:42:54.546330 lazysdk-0.1.97/lazysdk/
+-rw-r--r--   0 zeroseeker   (501) staff       (20)      184 2023-12-14 08:15:44.000000 lazysdk-0.1.97/lazysdk/__init__.py
+-rw-r--r--   0 zeroseeker   (501) staff       (20)      389 2023-12-14 08:15:44.000000 lazysdk-0.1.97/lazysdk/lazyCrypto.py
+-rw-r--r--   0 zeroseeker   (501) staff       (20)     2797 2023-12-14 08:15:44.000000 lazysdk-0.1.97/lazysdk/lazy_id_card.py
+-rw-r--r--   0 zeroseeker   (501) staff       (20)      669 2023-12-14 08:15:44.000000 lazysdk-0.1.97/lazysdk/lazybase64.py
+-rw-r--r--   0 zeroseeker   (501) staff       (20)      571 2024-02-02 03:54:22.000000 lazysdk-0.1.97/lazysdk/lazycache.py
+-rw-r--r--   0 zeroseeker   (501) staff       (20)    15383 2023-12-25 11:22:47.000000 lazysdk-0.1.97/lazysdk/lazychromedriver.py
+-rw-r--r--   0 zeroseeker   (501) staff       (20)      414 2024-02-01 03:07:43.000000 lazysdk-0.1.97/lazysdk/lazydecode.py
+-rw-r--r--   0 zeroseeker   (501) staff       (20)     8883 2024-01-09 11:35:26.000000 lazysdk-0.1.97/lazysdk/lazydict.py
+-rw-r--r--   0 zeroseeker   (501) staff       (20)     3024 2023-12-14 08:15:44.000000 lazysdk-0.1.97/lazysdk/lazyenv.py
+-rw-r--r--   0 zeroseeker   (501) staff       (20)    15835 2024-02-02 07:00:02.000000 lazysdk-0.1.97/lazysdk/lazyexcel.py
+-rw-r--r--   0 zeroseeker   (501) staff       (20)    20263 2024-02-04 08:23:46.000000 lazysdk-0.1.97/lazysdk/lazyfile.py
+-rw-r--r--   0 zeroseeker   (501) staff       (20)      727 2023-12-14 08:15:44.000000 lazysdk-0.1.97/lazysdk/lazyflask.py
+-rw-r--r--   0 zeroseeker   (501) staff       (20)     2403 2024-05-09 08:02:54.000000 lazysdk-0.1.97/lazysdk/lazyhtml.py
+-rw-r--r--   0 zeroseeker   (501) staff       (20)     1388 2024-05-08 00:15:57.000000 lazysdk-0.1.97/lazysdk/lazyid.py
+-rw-r--r--   0 zeroseeker   (501) staff       (20)     3673 2023-12-14 08:15:44.000000 lazysdk-0.1.97/lazysdk/lazyinfo.py
+-rw-r--r--   0 zeroseeker   (501) staff       (20)     1364 2023-12-14 08:15:44.000000 lazysdk-0.1.97/lazysdk/lazyip.py
+-rw-r--r--   0 zeroseeker   (501) staff       (20)      867 2024-01-18 03:56:02.000000 lazysdk-0.1.97/lazysdk/lazyjson.py
+-rw-r--r--   0 zeroseeker   (501) staff       (20)      363 2024-04-24 09:30:41.000000 lazysdk-0.1.97/lazysdk/lazylist.py
+-rw-r--r--   0 zeroseeker   (501) staff       (20)    31937 2023-12-14 08:15:44.000000 lazysdk-0.1.97/lazysdk/lazym3u8.py
+-rw-r--r--   0 zeroseeker   (501) staff       (20)     1112 2023-12-14 08:15:44.000000 lazysdk-0.1.97/lazysdk/lazymd5.py
+-rw-r--r--   0 zeroseeker   (501) staff       (20)     6052 2024-05-28 09:17:29.000000 lazysdk-0.1.97/lazysdk/lazypath.py
+-rw-r--r--   0 zeroseeker   (501) staff       (20)    17702 2023-12-14 08:15:44.000000 lazysdk-0.1.97/lazysdk/lazyprocess.py
+-rw-r--r--   0 zeroseeker   (501) staff       (20)      546 2023-12-14 08:15:44.000000 lazysdk-0.1.97/lazysdk/lazyproxies.py
+-rw-r--r--   0 zeroseeker   (501) staff       (20)     1420 2023-12-14 08:15:44.000000 lazysdk-0.1.97/lazysdk/lazyrandom.py
+-rw-r--r--   0 zeroseeker   (501) staff       (20)    37918 2023-12-14 08:15:44.000000 lazysdk-0.1.97/lazysdk/lazyredis.py
+-rw-r--r--   0 zeroseeker   (501) staff       (20)     3750 2023-12-14 08:15:44.000000 lazysdk-0.1.97/lazysdk/lazyrequests.py
+-rw-r--r--   0 zeroseeker   (501) staff       (20)     2672 2024-05-28 10:17:19.000000 lazysdk-0.1.97/lazysdk/lazytext.py
+-rw-r--r--   0 zeroseeker   (501) staff       (20)    26530 2024-02-02 08:29:53.000000 lazysdk-0.1.97/lazysdk/lazytime.py
+-rw-r--r--   0 zeroseeker   (501) staff       (20)     4827 2023-12-14 08:15:44.000000 lazysdk-0.1.97/lazysdk/lazyua.py
+-rw-r--r--   0 zeroseeker   (501) staff       (20)     1550 2023-12-14 08:15:44.000000 lazysdk-0.1.97/lazysdk/lazyurl.py
+-rw-r--r--   0 zeroseeker   (501) staff       (20)     8937 2024-05-07 04:00:07.000000 lazysdk-0.1.97/lazysdk/lazywebhook.py
+-rw-r--r--   0 zeroseeker   (501) staff       (20)      716 2023-12-14 08:15:44.000000 lazysdk-0.1.97/lazysdk/lazywifi.py
+-rw-r--r--   0 zeroseeker   (501) staff       (20)      770 2024-03-22 06:19:36.000000 lazysdk-0.1.97/lazysdk/lazyxml.py
+-rw-r--r--   0 zeroseeker   (501) staff       (20)     1683 2023-12-26 07:19:36.000000 lazysdk-0.1.97/lazysdk/showdata.py
+drwxr-xr-x   0 zeroseeker   (501) staff       (20)        0 2024-05-28 10:42:54.547115 lazysdk-0.1.97/lazysdk.egg-info/
+-rw-r--r--   0 zeroseeker   (501) staff       (20)     1898 2024-05-28 10:42:54.000000 lazysdk-0.1.97/lazysdk.egg-info/PKG-INFO
+-rw-r--r--   0 zeroseeker   (501) staff       (20)      887 2024-05-28 10:42:54.000000 lazysdk-0.1.97/lazysdk.egg-info/SOURCES.txt
+-rw-r--r--   0 zeroseeker   (501) staff       (20)        1 2024-05-28 10:42:54.000000 lazysdk-0.1.97/lazysdk.egg-info/dependency_links.txt
+-rw-r--r--   0 zeroseeker   (501) staff       (20)      216 2024-05-28 10:42:54.000000 lazysdk-0.1.97/lazysdk.egg-info/requires.txt
+-rw-r--r--   0 zeroseeker   (501) staff       (20)        8 2024-05-28 10:42:54.000000 lazysdk-0.1.97/lazysdk.egg-info/top_level.txt
+-rw-r--r--   0 zeroseeker   (501) staff       (20)       38 2024-05-28 10:42:54.547634 lazysdk-0.1.97/setup.cfg
+-rw-r--r--   0 zeroseeker   (501) staff       (20)     1208 2024-05-28 10:17:19.000000 lazysdk-0.1.97/setup.py
```

### Comparing `lazysdk-0.1.96/LICENSE` & `lazysdk-0.1.97/LICENSE`

 * *Files identical despite different names*

### Comparing `lazysdk-0.1.96/PKG-INFO` & `lazysdk-0.1.97/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: lazysdk
-Version: 0.1.96
+Version: 0.1.97
 Summary: 基于Python的懒人包
 Home-page: https://gitee.com/ZeroSeeker/lazysdk
 Author: ZeroSeeker
 Author-email: zeroseeker@foxmail.com
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

### Comparing `lazysdk-0.1.96/README.md` & `lazysdk-0.1.97/README.md`

 * *Files identical despite different names*

### Comparing `lazysdk-0.1.96/lazysdk/lazy_id_card.py` & `lazysdk-0.1.97/lazysdk/lazy_id_card.py`

 * *Files identical despite different names*

### Comparing `lazysdk-0.1.96/lazysdk/lazybase64.py` & `lazysdk-0.1.97/lazysdk/lazybase64.py`

 * *Files identical despite different names*

### Comparing `lazysdk-0.1.96/lazysdk/lazycache.py` & `lazysdk-0.1.97/lazysdk/lazycache.py`

 * *Files identical despite different names*

### Comparing `lazysdk-0.1.96/lazysdk/lazychromedriver.py` & `lazysdk-0.1.97/lazysdk/lazychromedriver.py`

 * *Files identical despite different names*

### Comparing `lazysdk-0.1.96/lazysdk/lazydict.py` & `lazysdk-0.1.97/lazysdk/lazydict.py`

 * *Files identical despite different names*

### Comparing `lazysdk-0.1.96/lazysdk/lazyenv.py` & `lazysdk-0.1.97/lazysdk/lazyenv.py`

 * *Files identical despite different names*

### Comparing `lazysdk-0.1.96/lazysdk/lazyexcel.py` & `lazysdk-0.1.97/lazysdk/lazyexcel.py`

 * *Files identical despite different names*

### Comparing `lazysdk-0.1.96/lazysdk/lazyfile.py` & `lazysdk-0.1.97/lazysdk/lazyfile.py`

 * *Files identical despite different names*

### Comparing `lazysdk-0.1.96/lazysdk/lazyflask.py` & `lazysdk-0.1.97/lazysdk/lazyflask.py`

 * *Files identical despite different names*

### Comparing `lazysdk-0.1.96/lazysdk/lazyhtml.py` & `lazysdk-0.1.97/lazysdk/lazyhtml.py`

 * *Files identical despite different names*

### Comparing `lazysdk-0.1.96/lazysdk/lazyid.py` & `lazysdk-0.1.97/lazysdk/lazyid.py`

 * *Files identical despite different names*

### Comparing `lazysdk-0.1.96/lazysdk/lazyinfo.py` & `lazysdk-0.1.97/lazysdk/lazyinfo.py`

 * *Files identical despite different names*

### Comparing `lazysdk-0.1.96/lazysdk/lazyip.py` & `lazysdk-0.1.97/lazysdk/lazyip.py`

 * *Files identical despite different names*

### Comparing `lazysdk-0.1.96/lazysdk/lazyjson.py` & `lazysdk-0.1.97/lazysdk/lazyjson.py`

 * *Files identical despite different names*

### Comparing `lazysdk-0.1.96/lazysdk/lazym3u8.py` & `lazysdk-0.1.97/lazysdk/lazym3u8.py`

 * *Files identical despite different names*

### Comparing `lazysdk-0.1.96/lazysdk/lazymd5.py` & `lazysdk-0.1.97/lazysdk/lazymd5.py`

 * *Files identical despite different names*

### Comparing `lazysdk-0.1.96/lazysdk/lazypath.py` & `lazysdk-0.1.97/lazysdk/lazypath.py`

 * *Files identical despite different names*

### Comparing `lazysdk-0.1.96/lazysdk/lazyprocess.py` & `lazysdk-0.1.97/lazysdk/lazyprocess.py`

 * *Files identical despite different names*

### Comparing `lazysdk-0.1.96/lazysdk/lazyproxies.py` & `lazysdk-0.1.97/lazysdk/lazyproxies.py`

 * *Files identical despite different names*

### Comparing `lazysdk-0.1.96/lazysdk/lazyrandom.py` & `lazysdk-0.1.97/lazysdk/lazyrandom.py`

 * *Files identical despite different names*

### Comparing `lazysdk-0.1.96/lazysdk/lazyredis.py` & `lazysdk-0.1.97/lazysdk/lazyredis.py`

 * *Files identical despite different names*

### Comparing `lazysdk-0.1.96/lazysdk/lazyrequests.py` & `lazysdk-0.1.97/lazysdk/lazyrequests.py`

 * *Files identical despite different names*

### Comparing `lazysdk-0.1.96/lazysdk/lazytext.py` & `lazysdk-0.1.97/lazysdk/lazytext.py`

 * *Files 2% similar despite different names*

```diff
@@ -54,15 +54,17 @@
     return url_list
 
 
 def path_clean(content):
     """
     清除路径前后可能出现的引号
     """
-    if content[0] == '"' and content[-1] == '"':
+    if not content:
+        return content
+    elif content[0] == '"' and content[-1] == '"':
         content = content[1:-1]
     elif content[0] == '“' and content[-1] == '”':
         content = content[1:-1]
     elif content[0] == "'" and content[-1] == "'":
         content = content[1:-1]
     else:
         pass
```

### Comparing `lazysdk-0.1.96/lazysdk/lazytime.py` & `lazysdk-0.1.97/lazysdk/lazytime.py`

 * *Files identical despite different names*

### Comparing `lazysdk-0.1.96/lazysdk/lazyua.py` & `lazysdk-0.1.97/lazysdk/lazyua.py`

 * *Files identical despite different names*

### Comparing `lazysdk-0.1.96/lazysdk/lazyurl.py` & `lazysdk-0.1.97/lazysdk/lazyurl.py`

 * *Files identical despite different names*

### Comparing `lazysdk-0.1.96/lazysdk/lazywebhook.py` & `lazysdk-0.1.97/lazysdk/lazywebhook.py`

 * *Files identical despite different names*

### Comparing `lazysdk-0.1.96/lazysdk/lazywifi.py` & `lazysdk-0.1.97/lazysdk/lazywifi.py`

 * *Files identical despite different names*

### Comparing `lazysdk-0.1.96/lazysdk/lazyxml.py` & `lazysdk-0.1.97/lazysdk/lazyxml.py`

 * *Files identical despite different names*

### Comparing `lazysdk-0.1.96/lazysdk/showdata.py` & `lazysdk-0.1.97/lazysdk/showdata.py`

 * *Files identical despite different names*

### Comparing `lazysdk-0.1.96/lazysdk.egg-info/PKG-INFO` & `lazysdk-0.1.97/lazysdk.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: lazysdk
-Version: 0.1.96
+Version: 0.1.97
 Summary: 基于Python的懒人包
 Home-page: https://gitee.com/ZeroSeeker/lazysdk
 Author: ZeroSeeker
 Author-email: zeroseeker@foxmail.com
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

### Comparing `lazysdk-0.1.96/lazysdk.egg-info/SOURCES.txt` & `lazysdk-0.1.97/lazysdk.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `lazysdk-0.1.96/setup.py` & `lazysdk-0.1.97/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -9,15 +9,15 @@
 import setuptools
 
 with open("README.md", "r", encoding='utf-8') as fh:
     long_description = fh.read()
 
 setuptools.setup(
     name="lazysdk",
-    version="0.1.96",
+    version="0.1.97",
     description="基于Python的懒人包",
     long_description=long_description,
     long_description_content_type="text/markdown",
     author="ZeroSeeker",
     author_email="zeroseeker@foxmail.com",
     url="https://gitee.com/ZeroSeeker/lazysdk",
     packages=setuptools.find_packages(),
```

