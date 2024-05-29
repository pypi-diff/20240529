# Comparing `tmp/ratteil-1.0.2.tar.gz` & `tmp/ratteil-2024.5.29b0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ratteil-1.0.2.tar", last modified: Wed May 29 09:43:31 2024, max compression
+gzip compressed data, was "ratteil-2024.5.29b0.tar", last modified: Wed May 29 10:16:59 2024, max compression
```

## Comparing `ratteil-1.0.2.tar` & `ratteil-2024.5.29b0.tar`

### file list

```diff
@@ -1,42 +1,43 @@
-drwxrwxrwx   0 codespace  (1000) codespace  (1000)        0 2024-05-29 09:43:31.864148 ratteil-1.0.2/
--rw-rw-r--   0 codespace  (1000) codespace  (1000)    35148 2024-04-19 05:51:48.000000 ratteil-1.0.2/LICENSE
--rw-rw-r--   0 codespace  (1000) codespace  (1000)      217 2024-04-23 10:07:52.000000 ratteil-1.0.2/MANIFEST.in
--rw-rw-r--   0 codespace  (1000) codespace  (1000)      687 2024-04-16 18:09:28.000000 ratteil-1.0.2/NOTICE
--rw-r--r--   0 codespace  (1000) codespace  (1000)    42837 2024-05-29 09:43:31.864148 ratteil-1.0.2/PKG-INFO
--rw-rw-r--   0 codespace  (1000) codespace  (1000)     1427 2024-04-19 05:57:10.000000 ratteil-1.0.2/README.md
--rw-rw-r--   0 codespace  (1000) codespace  (1000)     1185 2024-05-28 15:39:48.000000 ratteil-1.0.2/pyproject.toml
--rw-rw-rw-   0 codespace  (1000) codespace  (1000)       38 2024-05-29 09:43:31.864148 ratteil-1.0.2/setup.cfg
-drwxrwxrwx   0 codespace  (1000) codespace  (1000)        0 2024-05-29 09:43:31.840147 ratteil-1.0.2/src/
-drwxrwxrwx   0 codespace  (1000) codespace  (1000)        0 2024-05-29 09:43:31.848147 ratteil-1.0.2/src/ratteil/
--rw-rw-r--   0 codespace  (1000) codespace  (1000)     6381 2024-04-19 05:46:42.000000 ratteil-1.0.2/src/ratteil/__init__.py
--rw-rw-r--   0 codespace  (1000) codespace  (1000)       62 2024-04-15 17:19:30.000000 ratteil-1.0.2/src/ratteil/__main__.py
--rw-rw-r--   0 codespace  (1000) codespace  (1000)    10678 2024-04-19 05:44:28.000000 ratteil-1.0.2/src/ratteil/base.py
--rw-rw-r--   0 codespace  (1000) codespace  (1000)      544 2024-04-15 14:13:52.000000 ratteil-1.0.2/src/ratteil/base_test.py
--rw-rw-r--   0 codespace  (1000) codespace  (1000)     6498 2024-04-16 18:07:00.000000 ratteil-1.0.2/src/ratteil/create_stream.py
--rw-rw-r--   0 codespace  (1000) codespace  (1000)     1924 2024-04-16 14:01:00.000000 ratteil-1.0.2/src/ratteil/dl.py
-drwxrwxrwx   0 codespace  (1000) codespace  (1000)        0 2024-05-29 09:43:31.848147 ratteil-1.0.2/src/ratteil/docs/
--rw-rw-r--   0 codespace  (1000) codespace  (1000)     3320 2024-04-19 06:08:02.000000 ratteil-1.0.2/src/ratteil/docs/README.md
-drwxrwxrwx   0 codespace  (1000) codespace  (1000)        0 2024-05-29 09:43:31.848147 ratteil-1.0.2/src/ratteil/fixer/
--rw-rw-r--   0 codespace  (1000) codespace  (1000)   138922 2024-04-15 14:13:52.000000 ratteil-1.0.2/src/ratteil/fixer/conclusion.mp4
--rw-rw-r--   0 codespace  (1000) codespace  (1000)  3128195 2024-04-15 14:13:52.000000 ratteil-1.0.2/src/ratteil/fixer/introduction.mp4
-drwxrwxrwx   0 codespace  (1000) codespace  (1000)        0 2024-05-29 09:43:31.864148 ratteil-1.0.2/src/ratteil/imgs/
--rw-rw-r--   0 codespace  (1000) codespace  (1000)   320917 2024-04-15 14:13:52.000000 ratteil-1.0.2/src/ratteil/imgs/0.jpg
--rw-rw-r--   0 codespace  (1000) codespace  (1000)   140530 2024-04-21 06:27:48.000000 ratteil-1.0.2/src/ratteil/imgs/1.jpg
--rw-rw-r--   0 codespace  (1000) codespace  (1000)   133913 2024-04-21 06:27:48.000000 ratteil-1.0.2/src/ratteil/imgs/2.jpg
--rw-rw-r--   0 codespace  (1000) codespace  (1000)    98140 2024-04-21 06:27:46.000000 ratteil-1.0.2/src/ratteil/imgs/3.jpg
--rw-rw-r--   0 codespace  (1000) codespace  (1000)   286669 2024-04-21 06:23:50.000000 ratteil-1.0.2/src/ratteil/imgs/4.jpg
--rw-rw-r--   0 codespace  (1000) codespace  (1000)   307462 2024-04-20 08:53:28.000000 ratteil-1.0.2/src/ratteil/imgs/5.jpg
--rw-rw-r--   0 codespace  (1000) codespace  (1000)   383225 2024-04-20 08:53:28.000000 ratteil-1.0.2/src/ratteil/imgs/6.jpg
--rw-rw-r--   0 codespace  (1000) codespace  (1000)   222475 2024-04-20 16:12:26.000000 ratteil-1.0.2/src/ratteil/imgs/7.jpg
--rw-rw-r--   0 codespace  (1000) codespace  (1000)   233836 2024-04-21 06:23:50.000000 ratteil-1.0.2/src/ratteil/imgs/8.jpg
--rw-rw-r--   0 codespace  (1000) codespace  (1000)       55 2024-04-17 08:12:06.000000 ratteil-1.0.2/src/ratteil/install.sh
--rw-rw-r--   0 codespace  (1000) codespace  (1000)   138328 2024-04-15 14:13:52.000000 ratteil-1.0.2/src/ratteil/reciters.py
--rw-rw-r--   0 codespace  (1000) codespace  (1000)      107 2024-04-15 14:13:52.000000 ratteil-1.0.2/src/ratteil/requirements.txt
--rw-rw-r--   0 codespace  (1000) codespace  (1000)    12274 2024-04-15 14:13:52.000000 ratteil-1.0.2/src/ratteil/surahs.py
-drwxrwxrwx   0 codespace  (1000) codespace  (1000)        0 2024-05-29 09:43:31.864148 ratteil-1.0.2/src/ratteil.egg-info/
--rw-r--r--   0 codespace  (1000) codespace  (1000)    42837 2024-05-29 09:43:31.000000 ratteil-1.0.2/src/ratteil.egg-info/PKG-INFO
--rw-rw-rw-   0 codespace  (1000) codespace  (1000)      803 2024-05-29 09:43:31.000000 ratteil-1.0.2/src/ratteil.egg-info/SOURCES.txt
--rw-rw-rw-   0 codespace  (1000) codespace  (1000)        1 2024-05-29 09:43:31.000000 ratteil-1.0.2/src/ratteil.egg-info/dependency_links.txt
--rw-rw-rw-   0 codespace  (1000) codespace  (1000)       44 2024-05-29 09:43:31.000000 ratteil-1.0.2/src/ratteil.egg-info/entry_points.txt
--rw-rw-rw-   0 codespace  (1000) codespace  (1000)      120 2024-05-29 09:43:31.000000 ratteil-1.0.2/src/ratteil.egg-info/requires.txt
--rw-rw-rw-   0 codespace  (1000) codespace  (1000)        8 2024-05-29 09:43:31.000000 ratteil-1.0.2/src/ratteil.egg-info/top_level.txt
+drwxrwxrwx   0 codespace  (1000) codespace  (1000)        0 2024-05-29 10:16:59.763590 ratteil-2024.5.29b0/
+-rw-rw-r--   0 codespace  (1000) codespace  (1000)    35148 2024-04-19 05:51:48.000000 ratteil-2024.5.29b0/LICENSE
+-rw-rw-r--   0 codespace  (1000) codespace  (1000)      258 2024-05-29 10:15:05.000000 ratteil-2024.5.29b0/MANIFEST.in
+-rw-rw-r--   0 codespace  (1000) codespace  (1000)      687 2024-04-16 18:09:28.000000 ratteil-2024.5.29b0/NOTICE
+-rw-r--r--   0 codespace  (1000) codespace  (1000)    42843 2024-05-29 10:16:59.763590 ratteil-2024.5.29b0/PKG-INFO
+-rw-rw-r--   0 codespace  (1000) codespace  (1000)     1427 2024-04-19 05:57:10.000000 ratteil-2024.5.29b0/README.md
+-rw-rw-r--   0 codespace  (1000) codespace  (1000)     1196 2024-05-29 10:16:41.000000 ratteil-2024.5.29b0/pyproject.toml
+-rw-rw-rw-   0 codespace  (1000) codespace  (1000)       38 2024-05-29 10:16:59.763590 ratteil-2024.5.29b0/setup.cfg
+drwxrwxrwx   0 codespace  (1000) codespace  (1000)        0 2024-05-29 10:16:59.715590 ratteil-2024.5.29b0/src/
+drwxrwxrwx   0 codespace  (1000) codespace  (1000)        0 2024-05-29 10:16:59.735590 ratteil-2024.5.29b0/src/ratteil/
+-rw-rw-r--   0 codespace  (1000) codespace  (1000)     6381 2024-04-19 05:46:42.000000 ratteil-2024.5.29b0/src/ratteil/__init__.py
+-rw-rw-r--   0 codespace  (1000) codespace  (1000)       62 2024-04-15 17:19:30.000000 ratteil-2024.5.29b0/src/ratteil/__main__.py
+-rw-rw-r--   0 codespace  (1000) codespace  (1000)    10678 2024-04-19 05:44:28.000000 ratteil-2024.5.29b0/src/ratteil/base.py
+-rw-rw-r--   0 codespace  (1000) codespace  (1000)      544 2024-04-15 14:13:52.000000 ratteil-2024.5.29b0/src/ratteil/base_test.py
+-rw-rw-r--   0 codespace  (1000) codespace  (1000)      396 2024-04-15 14:13:52.000000 ratteil-2024.5.29b0/src/ratteil/client_secrets.json
+-rw-rw-r--   0 codespace  (1000) codespace  (1000)     6498 2024-04-16 18:07:00.000000 ratteil-2024.5.29b0/src/ratteil/create_stream.py
+-rw-rw-r--   0 codespace  (1000) codespace  (1000)     1924 2024-04-16 14:01:00.000000 ratteil-2024.5.29b0/src/ratteil/dl.py
+drwxrwxrwx   0 codespace  (1000) codespace  (1000)        0 2024-05-29 10:16:59.739590 ratteil-2024.5.29b0/src/ratteil/docs/
+-rw-rw-r--   0 codespace  (1000) codespace  (1000)     3320 2024-04-19 06:08:02.000000 ratteil-2024.5.29b0/src/ratteil/docs/README.md
+drwxrwxrwx   0 codespace  (1000) codespace  (1000)        0 2024-05-29 10:16:59.743590 ratteil-2024.5.29b0/src/ratteil/fixer/
+-rw-rw-r--   0 codespace  (1000) codespace  (1000)   138922 2024-04-15 14:13:52.000000 ratteil-2024.5.29b0/src/ratteil/fixer/conclusion.mp4
+-rw-rw-r--   0 codespace  (1000) codespace  (1000)  3128195 2024-04-15 14:13:52.000000 ratteil-2024.5.29b0/src/ratteil/fixer/introduction.mp4
+drwxrwxrwx   0 codespace  (1000) codespace  (1000)        0 2024-05-29 10:16:59.759590 ratteil-2024.5.29b0/src/ratteil/imgs/
+-rw-rw-r--   0 codespace  (1000) codespace  (1000)   320917 2024-04-15 14:13:52.000000 ratteil-2024.5.29b0/src/ratteil/imgs/0.jpg
+-rw-rw-r--   0 codespace  (1000) codespace  (1000)   140530 2024-04-21 06:27:48.000000 ratteil-2024.5.29b0/src/ratteil/imgs/1.jpg
+-rw-rw-r--   0 codespace  (1000) codespace  (1000)   133913 2024-04-21 06:27:48.000000 ratteil-2024.5.29b0/src/ratteil/imgs/2.jpg
+-rw-rw-r--   0 codespace  (1000) codespace  (1000)    98140 2024-04-21 06:27:46.000000 ratteil-2024.5.29b0/src/ratteil/imgs/3.jpg
+-rw-rw-r--   0 codespace  (1000) codespace  (1000)   286669 2024-04-21 06:23:50.000000 ratteil-2024.5.29b0/src/ratteil/imgs/4.jpg
+-rw-rw-r--   0 codespace  (1000) codespace  (1000)   307462 2024-04-20 08:53:28.000000 ratteil-2024.5.29b0/src/ratteil/imgs/5.jpg
+-rw-rw-r--   0 codespace  (1000) codespace  (1000)   383225 2024-04-20 08:53:28.000000 ratteil-2024.5.29b0/src/ratteil/imgs/6.jpg
+-rw-rw-r--   0 codespace  (1000) codespace  (1000)   222475 2024-04-20 16:12:26.000000 ratteil-2024.5.29b0/src/ratteil/imgs/7.jpg
+-rw-rw-r--   0 codespace  (1000) codespace  (1000)   233836 2024-04-21 06:23:50.000000 ratteil-2024.5.29b0/src/ratteil/imgs/8.jpg
+-rwxrwxr-x   0 codespace  (1000) codespace  (1000)       55 2024-04-17 08:12:06.000000 ratteil-2024.5.29b0/src/ratteil/install.sh
+-rw-rw-r--   0 codespace  (1000) codespace  (1000)   138328 2024-04-15 14:13:52.000000 ratteil-2024.5.29b0/src/ratteil/reciters.py
+-rw-rw-r--   0 codespace  (1000) codespace  (1000)      107 2024-04-15 14:13:52.000000 ratteil-2024.5.29b0/src/ratteil/requirements.txt
+-rw-rw-r--   0 codespace  (1000) codespace  (1000)    12274 2024-04-15 14:13:52.000000 ratteil-2024.5.29b0/src/ratteil/surahs.py
+drwxrwxrwx   0 codespace  (1000) codespace  (1000)        0 2024-05-29 10:16:59.763590 ratteil-2024.5.29b0/src/ratteil.egg-info/
+-rw-r--r--   0 codespace  (1000) codespace  (1000)    42843 2024-05-29 10:16:59.000000 ratteil-2024.5.29b0/src/ratteil.egg-info/PKG-INFO
+-rw-rw-rw-   0 codespace  (1000) codespace  (1000)      835 2024-05-29 10:16:59.000000 ratteil-2024.5.29b0/src/ratteil.egg-info/SOURCES.txt
+-rw-rw-rw-   0 codespace  (1000) codespace  (1000)        1 2024-05-29 10:16:59.000000 ratteil-2024.5.29b0/src/ratteil.egg-info/dependency_links.txt
+-rw-rw-rw-   0 codespace  (1000) codespace  (1000)       44 2024-05-29 10:16:59.000000 ratteil-2024.5.29b0/src/ratteil.egg-info/entry_points.txt
+-rw-rw-rw-   0 codespace  (1000) codespace  (1000)      120 2024-05-29 10:16:59.000000 ratteil-2024.5.29b0/src/ratteil.egg-info/requires.txt
+-rw-rw-rw-   0 codespace  (1000) codespace  (1000)        8 2024-05-29 10:16:59.000000 ratteil-2024.5.29b0/src/ratteil.egg-info/top_level.txt
```

### Comparing `ratteil-1.0.2/LICENSE` & `ratteil-2024.5.29b0/LICENSE`

 * *Files identical despite different names*

### Comparing `ratteil-1.0.2/NOTICE` & `ratteil-2024.5.29b0/NOTICE`

 * *Files identical despite different names*

### Comparing `ratteil-1.0.2/PKG-INFO` & `ratteil-2024.5.29b0/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ratteil
-Version: 1.0.2
+Version: 2024.5.29b0
 Summary: Livestreaming the Holly Quran to youtube
 Author-email: Ali Elfatih <alielfatih@hotmail.com>
 License:                     GNU GENERAL PUBLIC LICENSE
                                Version 3, 29 June 2007
         
          Copyright (C) 2007 Free Software Foundation, Inc. <https://fsf.org/>
          Everyone is permitted to copy and distribute verbatim copies
```

### Comparing `ratteil-1.0.2/README.md` & `ratteil-2024.5.29b0/README.md`

 * *Files identical despite different names*

### Comparing `ratteil-1.0.2/pyproject.toml` & `ratteil-2024.5.29b0/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["setuptools"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "ratteil"
-version = "1.0.2"
+version = "2024.05.29-beta"
 authors = [
   {name = "Ali Elfatih", email = "alielfatih@hotmail.com"},
 ]
 description = "Livestreaming the Holly Quran to youtube"
 requires-python = ">=3.7"
 keywords = ["Quran", "the Holly Quran", "Youtube", "streaming", "Live stream"]
 license = {file = "LICENSE"}
@@ -40,8 +40,8 @@
 [tool.setuptools]
 package-dir = {"" = "src"}
 
 [tool.setuptools.dynamic]
 readme = {file = ["README.md"], content-type = "text/markdown"}
 
 [project.scripts]
-ratteil = "ratteil:ratteil"
+ratteil = "ratteil:ratteil"
```

### Comparing `ratteil-1.0.2/src/ratteil/__init__.py` & `ratteil-2024.5.29b0/src/ratteil/__init__.py`

 * *Files identical despite different names*

### Comparing `ratteil-1.0.2/src/ratteil/base.py` & `ratteil-2024.5.29b0/src/ratteil/base.py`

 * *Files identical despite different names*

### Comparing `ratteil-1.0.2/src/ratteil/base_test.py` & `ratteil-2024.5.29b0/src/ratteil/base_test.py`

 * *Files identical despite different names*

### Comparing `ratteil-1.0.2/src/ratteil/create_stream.py` & `ratteil-2024.5.29b0/src/ratteil/create_stream.py`

 * *Files identical despite different names*

### Comparing `ratteil-1.0.2/src/ratteil/dl.py` & `ratteil-2024.5.29b0/src/ratteil/dl.py`

 * *Files identical despite different names*

### Comparing `ratteil-1.0.2/src/ratteil/docs/README.md` & `ratteil-2024.5.29b0/src/ratteil/docs/README.md`

 * *Files identical despite different names*

### Comparing `ratteil-1.0.2/src/ratteil/fixer/conclusion.mp4` & `ratteil-2024.5.29b0/src/ratteil/fixer/conclusion.mp4`

 * *Files identical despite different names*

### Comparing `ratteil-1.0.2/src/ratteil/fixer/introduction.mp4` & `ratteil-2024.5.29b0/src/ratteil/fixer/introduction.mp4`

 * *Files identical despite different names*

### Comparing `ratteil-1.0.2/src/ratteil/imgs/0.jpg` & `ratteil-2024.5.29b0/src/ratteil/imgs/0.jpg`

 * *Files identical despite different names*

### Comparing `ratteil-1.0.2/src/ratteil/imgs/1.jpg` & `ratteil-2024.5.29b0/src/ratteil/imgs/1.jpg`

 * *Files identical despite different names*

### Comparing `ratteil-1.0.2/src/ratteil/imgs/2.jpg` & `ratteil-2024.5.29b0/src/ratteil/imgs/2.jpg`

 * *Files identical despite different names*

### Comparing `ratteil-1.0.2/src/ratteil/imgs/3.jpg` & `ratteil-2024.5.29b0/src/ratteil/imgs/3.jpg`

 * *Files identical despite different names*

### Comparing `ratteil-1.0.2/src/ratteil/imgs/4.jpg` & `ratteil-2024.5.29b0/src/ratteil/imgs/4.jpg`

 * *Files identical despite different names*

### Comparing `ratteil-1.0.2/src/ratteil/imgs/5.jpg` & `ratteil-2024.5.29b0/src/ratteil/imgs/5.jpg`

 * *Files identical despite different names*

### Comparing `ratteil-1.0.2/src/ratteil/imgs/6.jpg` & `ratteil-2024.5.29b0/src/ratteil/imgs/6.jpg`

 * *Files identical despite different names*

### Comparing `ratteil-1.0.2/src/ratteil/imgs/7.jpg` & `ratteil-2024.5.29b0/src/ratteil/imgs/7.jpg`

 * *Files identical despite different names*

### Comparing `ratteil-1.0.2/src/ratteil/imgs/8.jpg` & `ratteil-2024.5.29b0/src/ratteil/imgs/8.jpg`

 * *Files identical despite different names*

### Comparing `ratteil-1.0.2/src/ratteil/reciters.py` & `ratteil-2024.5.29b0/src/ratteil/reciters.py`

 * *Files identical despite different names*

### Comparing `ratteil-1.0.2/src/ratteil/surahs.py` & `ratteil-2024.5.29b0/src/ratteil/surahs.py`

 * *Files identical despite different names*

### Comparing `ratteil-1.0.2/src/ratteil.egg-info/PKG-INFO` & `ratteil-2024.5.29b0/src/ratteil.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ratteil
-Version: 1.0.2
+Version: 2024.5.29b0
 Summary: Livestreaming the Holly Quran to youtube
 Author-email: Ali Elfatih <alielfatih@hotmail.com>
 License:                     GNU GENERAL PUBLIC LICENSE
                                Version 3, 29 June 2007
         
          Copyright (C) 2007 Free Software Foundation, Inc. <https://fsf.org/>
          Everyone is permitted to copy and distribute verbatim copies
```

### Comparing `ratteil-1.0.2/src/ratteil.egg-info/SOURCES.txt` & `ratteil-2024.5.29b0/src/ratteil.egg-info/SOURCES.txt`

 * *Files 6% similar despite different names*

```diff
@@ -3,14 +3,15 @@
 NOTICE
 README.md
 pyproject.toml
 src/ratteil/__init__.py
 src/ratteil/__main__.py
 src/ratteil/base.py
 src/ratteil/base_test.py
+src/ratteil/client_secrets.json
 src/ratteil/create_stream.py
 src/ratteil/dl.py
 src/ratteil/install.sh
 src/ratteil/reciters.py
 src/ratteil/requirements.txt
 src/ratteil/surahs.py
 src/ratteil.egg-info/PKG-INFO
```

