# Comparing `tmp/arcdlnexus-0.1.3.tar.gz` & `tmp/arcdlnexus-0.1.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "arcdlnexus-0.1.3.tar", last modified: Wed May 29 11:22:39 2024, max compression
+gzip compressed data, was "arcdlnexus-0.1.4.tar", last modified: Wed May 29 12:03:16 2024, max compression
```

## Comparing `arcdlnexus-0.1.3.tar` & `arcdlnexus-0.1.4.tar`

### file list

```diff
@@ -1,15 +1,15 @@
-drwxrwxrwx   0        0        0        0 2024-05-29 11:22:39.445900 arcdlnexus-0.1.3/
-drwxrwxrwx   0        0        0        0 2024-05-29 11:22:39.416977 arcdlnexus-0.1.3/ArcDLNexus/
--rw-rw-rw-   0        0        0       46 2024-05-29 11:22:35.000000 arcdlnexus-0.1.3/ArcDLNexus/__init__.py
--rw-rw-rw-   0        0        0     8290 2024-05-29 11:19:20.000000 arcdlnexus-0.1.3/ArcDLNexus/main.py
-drwxrwxrwx   0        0        0        0 2024-05-29 11:22:39.443923 arcdlnexus-0.1.3/ArcDLNexus.egg-info/
--rw-rw-rw-   0        0        0     6134 2024-05-29 11:22:39.000000 arcdlnexus-0.1.3/ArcDLNexus.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      237 2024-05-29 11:22:39.000000 arcdlnexus-0.1.3/ArcDLNexus.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-05-29 11:22:39.000000 arcdlnexus-0.1.3/ArcDLNexus.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       17 2024-05-29 11:22:39.000000 arcdlnexus-0.1.3/ArcDLNexus.egg-info/requires.txt
--rw-rw-rw-   0        0        0       11 2024-05-29 11:22:39.000000 arcdlnexus-0.1.3/ArcDLNexus.egg-info/top_level.txt
--rw-rw-rw-   0        0        0     1324 2024-05-28 13:09:40.000000 arcdlnexus-0.1.3/LICENSE
--rw-rw-rw-   0        0        0     6134 2024-05-29 11:22:39.444903 arcdlnexus-0.1.3/PKG-INFO
--rw-rw-rw-   0        0        0     4892 2024-05-29 10:33:49.000000 arcdlnexus-0.1.3/README.md
--rw-rw-rw-   0        0        0       42 2024-05-29 11:22:39.445900 arcdlnexus-0.1.3/setup.cfg
--rw-rw-rw-   0        0        0     2186 2024-05-29 10:16:04.000000 arcdlnexus-0.1.3/setup.py
+drwxrwxrwx   0        0        0        0 2024-05-29 12:03:16.482826 arcdlnexus-0.1.4/
+drwxrwxrwx   0        0        0        0 2024-05-29 12:03:16.455897 arcdlnexus-0.1.4/ArcDLNexus/
+-rw-rw-rw-   0        0        0       46 2024-05-29 12:02:09.000000 arcdlnexus-0.1.4/ArcDLNexus/__init__.py
+-rw-rw-rw-   0        0        0     8333 2024-05-29 12:02:09.000000 arcdlnexus-0.1.4/ArcDLNexus/main.py
+drwxrwxrwx   0        0        0        0 2024-05-29 12:03:16.480830 arcdlnexus-0.1.4/ArcDLNexus.egg-info/
+-rw-rw-rw-   0        0        0     6173 2024-05-29 12:03:16.000000 arcdlnexus-0.1.4/ArcDLNexus.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      237 2024-05-29 12:03:16.000000 arcdlnexus-0.1.4/ArcDLNexus.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-05-29 12:03:16.000000 arcdlnexus-0.1.4/ArcDLNexus.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       40 2024-05-29 12:03:16.000000 arcdlnexus-0.1.4/ArcDLNexus.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       11 2024-05-29 12:03:16.000000 arcdlnexus-0.1.4/ArcDLNexus.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0     1324 2024-05-28 13:09:40.000000 arcdlnexus-0.1.4/LICENSE
+-rw-rw-rw-   0        0        0     6173 2024-05-29 12:03:16.481828 arcdlnexus-0.1.4/PKG-INFO
+-rw-rw-rw-   0        0        0     4892 2024-05-29 10:33:49.000000 arcdlnexus-0.1.4/README.md
+-rw-rw-rw-   0        0        0       42 2024-05-29 12:03:16.482826 arcdlnexus-0.1.4/setup.cfg
+-rw-rw-rw-   0        0        0     2186 2024-05-29 10:16:04.000000 arcdlnexus-0.1.4/setup.py
```

### Comparing `arcdlnexus-0.1.3/ArcDLNexus/main.py` & `arcdlnexus-0.1.4/ArcDLNexus/main.py`

 * *Files 1% similar despite different names*

```diff
@@ -36,19 +36,21 @@
     "Connection": "keep-alive",
     "Upgrade-Insecure-Requests": "1",
     "Cache-Control": "max-age=0"
 }
 
 
 def download(url, path="./archive_download", mode=0):
-    html_path = path
+    print(path[-1])
     if not path[-1] == "/":
         path += "/"
+    html_path = path
     html_path += "index.html"
     tmp_path = ""
+    print(html_path)
     for tmp in html_path.split("/"):
         tmp_path += tmp + "/"
         if not os.path.exists(tmp_path) and not "." in tmp:
             os.mkdir(tmp_path)
     session = requests.session()
     while True:
         try:
```

### Comparing `arcdlnexus-0.1.3/ArcDLNexus.egg-info/PKG-INFO` & `arcdlnexus-0.1.4/ArcDLNexus.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ArcDLNexus
-Version: 0.1.3
+Version: 0.1.4
 Summary: ArcDLNexus: PythonからWayback Machineのアーカイブ（サイト）をダウンロードするモジュールです。
 Home-page: https://github.com/harumaki4649/ArcDLNexus
 Download-URL: https://github.com/harumaki4649/ArcDLNexus
 Author: ArcDLNexus
 Author-email: support@disnana.com
 Maintainer: ArcDLNexus
 Maintainer-email: support@disnana.com
@@ -22,14 +22,15 @@
 Classifier: Topic :: Scientific/Engineering :: Artificial Intelligence
 Classifier: Topic :: Multimedia :: Graphics
 Classifier: Framework :: Matplotlib
 Requires-Python: >=3.9
 Description-Content-Type: text/markdown
 License-File: LICENSE
 Requires-Dist: requests==2.32.2
+Requires-Dist: beautifulsoup4==4.12.3
 
 # PayNexus
 
 ## 目次
 
 >1. [プロジェクトについて](#プロジェクトについて)
 >2. [インストール方法](#インストール方法)
```

### Comparing `arcdlnexus-0.1.3/LICENSE` & `arcdlnexus-0.1.4/LICENSE`

 * *Files identical despite different names*

### Comparing `arcdlnexus-0.1.3/PKG-INFO` & `arcdlnexus-0.1.4/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ArcDLNexus
-Version: 0.1.3
+Version: 0.1.4
 Summary: ArcDLNexus: PythonからWayback Machineのアーカイブ（サイト）をダウンロードするモジュールです。
 Home-page: https://github.com/harumaki4649/ArcDLNexus
 Download-URL: https://github.com/harumaki4649/ArcDLNexus
 Author: ArcDLNexus
 Author-email: support@disnana.com
 Maintainer: ArcDLNexus
 Maintainer-email: support@disnana.com
@@ -22,14 +22,15 @@
 Classifier: Topic :: Scientific/Engineering :: Artificial Intelligence
 Classifier: Topic :: Multimedia :: Graphics
 Classifier: Framework :: Matplotlib
 Requires-Python: >=3.9
 Description-Content-Type: text/markdown
 License-File: LICENSE
 Requires-Dist: requests==2.32.2
+Requires-Dist: beautifulsoup4==4.12.3
 
 # PayNexus
 
 ## 目次
 
 >1. [プロジェクトについて](#プロジェクトについて)
 >2. [インストール方法](#インストール方法)
```

### Comparing `arcdlnexus-0.1.3/README.md` & `arcdlnexus-0.1.4/README.md`

 * *Files identical despite different names*

### Comparing `arcdlnexus-0.1.3/setup.py` & `arcdlnexus-0.1.4/setup.py`

 * *Files identical despite different names*

