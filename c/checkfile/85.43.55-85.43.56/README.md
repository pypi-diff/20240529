# Comparing `tmp/checkfile-85.43.55.tar.gz` & `tmp/checkfile-85.43.56.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "checkfile-85.43.55.tar", last modified: Wed May 29 00:40:28 2024, max compression
+gzip compressed data, was "checkfile-85.43.56.tar", last modified: Wed May 29 00:42:02 2024, max compression
```

## Comparing `checkfile-85.43.55.tar` & `checkfile-85.43.56.tar`

### file list

```diff
@@ -1,12 +1,12 @@
-drwxrwxrwx   0        0        0        0 2024-05-29 00:40:28.166942 checkfile-85.43.55/
--rw-rw-rw-   0        0        0      211 2024-05-29 00:40:28.164472 checkfile-85.43.55/PKG-INFO
--rw-rw-rw-   0        0        0        0 2024-05-29 00:24:36.000000 checkfile-85.43.55/README.md
-drwxrwxrwx   0        0        0        0 2024-05-29 00:40:28.139009 checkfile-85.43.55/checkfile/
--rw-rw-rw-   0        0        0      772 2024-05-29 00:39:48.000000 checkfile-85.43.55/checkfile/__init__.py
-drwxrwxrwx   0        0        0        0 2024-05-29 00:40:28.163472 checkfile-85.43.55/checkfile.egg-info/
--rw-rw-rw-   0        0        0      211 2024-05-29 00:40:27.000000 checkfile-85.43.55/checkfile.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      172 2024-05-29 00:40:28.000000 checkfile-85.43.55/checkfile.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-05-29 00:40:27.000000 checkfile-85.43.55/checkfile.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       10 2024-05-29 00:40:27.000000 checkfile-85.43.55/checkfile.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2024-05-29 00:40:28.166942 checkfile-85.43.55/setup.cfg
--rw-rw-rw-   0        0        0      426 2024-05-29 00:40:24.000000 checkfile-85.43.55/setup.py
+drwxrwxrwx   0        0        0        0 2024-05-29 00:42:02.582556 checkfile-85.43.56/
+-rw-rw-rw-   0        0        0      211 2024-05-29 00:42:02.563989 checkfile-85.43.56/PKG-INFO
+-rw-rw-rw-   0        0        0        0 2024-05-29 00:24:36.000000 checkfile-85.43.56/README.md
+drwxrwxrwx   0        0        0        0 2024-05-29 00:42:02.543524 checkfile-85.43.56/checkfile/
+-rw-rw-rw-   0        0        0      832 2024-05-29 00:41:51.000000 checkfile-85.43.56/checkfile/__init__.py
+drwxrwxrwx   0        0        0        0 2024-05-29 00:42:02.562592 checkfile-85.43.56/checkfile.egg-info/
+-rw-rw-rw-   0        0        0      211 2024-05-29 00:42:02.000000 checkfile-85.43.56/checkfile.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      172 2024-05-29 00:42:02.000000 checkfile-85.43.56/checkfile.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-05-29 00:42:02.000000 checkfile-85.43.56/checkfile.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       10 2024-05-29 00:42:02.000000 checkfile-85.43.56/checkfile.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2024-05-29 00:42:02.583558 checkfile-85.43.56/setup.cfg
+-rw-rw-rw-   0        0        0      426 2024-05-29 00:41:59.000000 checkfile-85.43.56/setup.py
```

### Comparing `checkfile-85.43.55/checkfile/__init__.py` & `checkfile-85.43.56/checkfile/__init__.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,25 +1,26 @@
 import sys
 import time
 def type(txt):
     for char in txt:
         sys.stdout.write(char)
         sys.stdout.flush()
         time.sleep(0.005)
+
 def check_file(file, file_content_file):
     with open(file, "r") as file1:
         read_file = file1.read()
         act_file = open(file_content_file, "r")
         read_act_file = act_file.read()
         if read_file != read_act_file:
             update_file(file, file_content_file)
 
 def update_file(file, file_content_file):
     with open(file,"w") as real_file:
         act_file = open(file_content_file, "r")
         read_act_file = act_file.read()
         try:
             real_file.write(read_act_file)
-            
+            type("Quiting Program Because File(s) Was/Were Edited...")
             quit()
         except Exception as e:
             print(f"Error: {e}")
```

