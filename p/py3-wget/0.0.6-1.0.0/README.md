# Comparing `tmp/py3_wget-0.0.6.tar.gz` & `tmp/py3_wget-1.0.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "py3_wget-0.0.6.tar", last modified: Mon Apr 29 14:11:54 2024, max compression
+gzip compressed data, was "py3_wget-1.0.0.tar", last modified: Wed May 29 03:35:56 2024, max compression
```

## Comparing `py3_wget-0.0.6.tar` & `py3_wget-1.0.0.tar`

### file list

```diff
@@ -1,18 +1,19 @@
-drwxrwxr-x   0 gaber     (1000) gaber     (1000)        0 2024-04-29 14:11:54.143618 py3_wget-0.0.6/
--rw-rw-r--   0 gaber     (1000) gaber     (1000)     1072 2024-04-29 14:09:48.000000 py3_wget-0.0.6/LICENSE
--rw-r--r--   0 gaber     (1000) gaber     (1000)     1072 2024-04-29 14:11:54.143618 py3_wget-0.0.6/PKG-INFO
--rw-rw-r--   0 gaber     (1000) gaber     (1000)      452 2024-04-29 14:09:48.000000 py3_wget-0.0.6/README.md
-drwxrwxr-x   0 gaber     (1000) gaber     (1000)        0 2024-04-29 14:11:54.139618 py3_wget-0.0.6/py3_wget/
--rw-rw-r--   0 gaber     (1000) gaber     (1000)       32 2024-04-29 14:09:48.000000 py3_wget-0.0.6/py3_wget/__init__.py
--rw-rw-r--   0 gaber     (1000) gaber     (1000)     2494 2024-04-29 14:10:30.000000 py3_wget-0.0.6/py3_wget/main.py
-drwxrwxr-x   0 gaber     (1000) gaber     (1000)        0 2024-04-29 14:11:54.143618 py3_wget-0.0.6/py3_wget.egg-info/
--rw-r--r--   0 gaber     (1000) gaber     (1000)     1072 2024-04-29 14:11:54.000000 py3_wget-0.0.6/py3_wget.egg-info/PKG-INFO
--rw-rw-r--   0 gaber     (1000) gaber     (1000)      255 2024-04-29 14:11:54.000000 py3_wget-0.0.6/py3_wget.egg-info/SOURCES.txt
--rw-rw-r--   0 gaber     (1000) gaber     (1000)        1 2024-04-29 14:11:54.000000 py3_wget-0.0.6/py3_wget.egg-info/dependency_links.txt
--rw-rw-r--   0 gaber     (1000) gaber     (1000)       14 2024-04-29 14:11:54.000000 py3_wget-0.0.6/py3_wget.egg-info/requires.txt
--rw-rw-r--   0 gaber     (1000) gaber     (1000)       15 2024-04-29 14:11:54.000000 py3_wget-0.0.6/py3_wget.egg-info/top_level.txt
--rw-rw-r--   0 gaber     (1000) gaber     (1000)       38 2024-04-29 14:11:54.143618 py3_wget-0.0.6/setup.cfg
--rw-rw-r--   0 gaber     (1000) gaber     (1000)     1022 2024-04-29 14:11:44.000000 py3_wget-0.0.6/setup.py
-drwxrwxr-x   0 gaber     (1000) gaber     (1000)        0 2024-04-29 14:11:54.143618 py3_wget-0.0.6/tests/
--rw-rw-r--   0 gaber     (1000) gaber     (1000)        0 2024-04-29 14:09:48.000000 py3_wget-0.0.6/tests/__init__.py
--rw-rw-r--   0 gaber     (1000) gaber     (1000)     1619 2024-04-29 14:09:48.000000 py3_wget-0.0.6/tests/test.py
+drwxrwxr-x   0 gaber     (1000) gaber     (1000)        0 2024-05-29 03:35:56.342220 py3_wget-1.0.0/
+-rw-rw-r--   0 gaber     (1000) gaber     (1000)     1072 2024-04-29 15:48:44.000000 py3_wget-1.0.0/LICENSE
+-rw-r--r--   0 gaber     (1000) gaber     (1000)     1187 2024-05-29 03:35:56.342220 py3_wget-1.0.0/PKG-INFO
+-rw-rw-r--   0 gaber     (1000) gaber     (1000)      591 2024-05-29 03:34:46.000000 py3_wget-1.0.0/README.md
+drwxrwxr-x   0 gaber     (1000) gaber     (1000)        0 2024-05-29 03:35:56.342220 py3_wget-1.0.0/py3_wget/
+-rw-rw-r--   0 gaber     (1000) gaber     (1000)       31 2024-05-29 01:53:49.000000 py3_wget-1.0.0/py3_wget/__init__.py
+-rw-rw-r--   0 gaber     (1000) gaber     (1000)     5494 2024-05-28 21:41:26.000000 py3_wget-1.0.0/py3_wget/cksum.py
+-rw-rw-r--   0 gaber     (1000) gaber     (1000)     4543 2024-05-29 03:34:15.000000 py3_wget-1.0.0/py3_wget/main.py
+drwxrwxr-x   0 gaber     (1000) gaber     (1000)        0 2024-05-29 03:35:56.342220 py3_wget-1.0.0/py3_wget.egg-info/
+-rw-r--r--   0 gaber     (1000) gaber     (1000)     1187 2024-05-29 03:35:56.000000 py3_wget-1.0.0/py3_wget.egg-info/PKG-INFO
+-rw-rw-r--   0 gaber     (1000) gaber     (1000)      273 2024-05-29 03:35:56.000000 py3_wget-1.0.0/py3_wget.egg-info/SOURCES.txt
+-rw-rw-r--   0 gaber     (1000) gaber     (1000)        1 2024-05-29 03:35:56.000000 py3_wget-1.0.0/py3_wget.egg-info/dependency_links.txt
+-rw-rw-r--   0 gaber     (1000) gaber     (1000)        5 2024-05-29 03:35:56.000000 py3_wget-1.0.0/py3_wget.egg-info/requires.txt
+-rw-rw-r--   0 gaber     (1000) gaber     (1000)       15 2024-05-29 03:35:56.000000 py3_wget-1.0.0/py3_wget.egg-info/top_level.txt
+-rw-rw-r--   0 gaber     (1000) gaber     (1000)       38 2024-05-29 03:35:56.346221 py3_wget-1.0.0/setup.cfg
+-rw-rw-r--   0 gaber     (1000) gaber     (1000)     1010 2024-05-29 03:35:22.000000 py3_wget-1.0.0/setup.py
+drwxrwxr-x   0 gaber     (1000) gaber     (1000)        0 2024-05-29 03:35:56.342220 py3_wget-1.0.0/tests/
+-rw-rw-r--   0 gaber     (1000) gaber     (1000)        0 2024-04-29 15:48:44.000000 py3_wget-1.0.0/tests/__init__.py
+-rw-rw-r--   0 gaber     (1000) gaber     (1000)     1361 2024-05-29 03:29:21.000000 py3_wget-1.0.0/tests/test.py
```

### Comparing `py3_wget-0.0.6/LICENSE` & `py3_wget-1.0.0/LICENSE`

 * *Files identical despite different names*

### Comparing `py3_wget-0.0.6/PKG-INFO` & `py3_wget-1.0.0/PKG-INFO`

 * *Files 22% similar despite different names*

```diff
@@ -1,39 +1,40 @@
 Metadata-Version: 2.1
 Name: py3_wget
-Version: 0.0.6
+Version: 1.0.0
 Summary: A simple tool to download files with python, supporting a progress bar
 Author: Gabriele Berton
 Author-email: <berton.gabri@gmail.com>
 Keywords: python,download,progress bar
 Classifier: Development Status :: 1 - Planning
 Classifier: Intended Audience :: Developers
 Classifier: Programming Language :: Python :: 3
 Classifier: Operating System :: Unix
 Classifier: Operating System :: MacOS :: MacOS X
 Classifier: Operating System :: Microsoft :: Windows
 Description-Content-Type: text/markdown
 License-File: LICENSE
-Requires-Dist: Requests
 Requires-Dist: tqdm
 
 
 # py3_wget
-A tool like wget for python, supporting a progress bar
+A tool like wget for python, supporting a (optional) progress bar, cksum, timeout, retry failed download.
 
 Install with
 ```
 pip install py3_wget
 ```
 
-and use simply like
+and use as simply as (for example)
 ```
 import py3_wget
 py3_wget.download_file(
-    url="https://universityofadelaide.app.box.com/index.php?rm=box_download_shared_file&shared_name=zkfk1akpbo5318fzqmtvlpp7030ex4up&file_id=f_1424424688104",
-    output_path="winter.tar.gz"
+    url="https://zenodo.org/record/1243106/files/Eynsham.zip?download=1",
+    output_path="Eynsham.zip"
 )
 ```
 
 ### TODO list
-- Improve tests
-- Add possibility to resume from partial download
+- [ ] Optionally resume from partial download
+- [x] Optionally pass cksum to downloader to ensure file is correctly downloaded
+- [x] Optionally turn off tqdm (silent download)
+- [x] Optionally set timeout for download request
```

### Comparing `py3_wget-0.0.6/setup.py` & `py3_wget-1.0.0/setup.py`

 * *Files 12% similar despite different names*

```diff
@@ -3,28 +3,28 @@
 import os
 
 here = os.path.abspath(os.path.dirname(__file__))
 
 with codecs.open(os.path.join(here, "README.md"), encoding="utf-8") as fh:
     long_description = "\n" + fh.read()
 
-VERSION = '0.0.6'
+VERSION = '1.0.0'
 DESCRIPTION = 'A simple tool to download files with python, supporting a progress bar'
 
 # Setting up
 setup(
     name="py3_wget",
     version=VERSION,
     author="Gabriele Berton",
     author_email="<berton.gabri@gmail.com>",
     description=DESCRIPTION,
     long_description_content_type="text/markdown",
     long_description=long_description,
     packages=find_packages(),
-    install_requires=['Requests', 'tqdm'],
+    install_requires=['tqdm'],
     keywords=['python', 'download', 'progress bar'],
     classifiers=[
         "Development Status :: 1 - Planning",
         "Intended Audience :: Developers",
         "Programming Language :: Python :: 3",
         "Operating System :: Unix",
         "Operating System :: MacOS :: MacOS X",
```

