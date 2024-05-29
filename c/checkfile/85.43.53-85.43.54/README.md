# Comparing `tmp/checkfile-85.43.53.tar.gz` & `tmp/checkfile-85.43.54.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "checkfile-85.43.53.tar", last modified: Wed May 29 00:25:54 2024, max compression
+gzip compressed data, was "checkfile-85.43.54.tar", last modified: Wed May 29 00:32:34 2024, max compression
```

## Comparing `checkfile-85.43.53.tar` & `checkfile-85.43.54.tar`

### file list

```diff
@@ -1,12 +1,12 @@
-drwxrwxrwx   0        0        0        0 2024-05-29 00:25:54.325398 checkfile-85.43.53/
--rw-rw-rw-   0        0        0      211 2024-05-29 00:25:54.323417 checkfile-85.43.53/PKG-INFO
--rw-rw-rw-   0        0        0        0 2024-05-29 00:24:36.000000 checkfile-85.43.53/README.md
-drwxrwxrwx   0        0        0        0 2024-05-29 00:25:54.287422 checkfile-85.43.53/checkfile/
--rw-rw-rw-   0        0        0      588 2024-05-29 00:20:05.000000 checkfile-85.43.53/checkfile/__init__.py
-drwxrwxrwx   0        0        0        0 2024-05-29 00:25:54.321405 checkfile-85.43.53/checkfile.egg-info/
--rw-rw-rw-   0        0        0      211 2024-05-29 00:25:54.000000 checkfile-85.43.53/checkfile.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      172 2024-05-29 00:25:54.000000 checkfile-85.43.53/checkfile.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-05-29 00:25:54.000000 checkfile-85.43.53/checkfile.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       10 2024-05-29 00:25:54.000000 checkfile-85.43.53/checkfile.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2024-05-29 00:25:54.326424 checkfile-85.43.53/setup.cfg
--rw-rw-rw-   0        0        0      426 2024-05-29 00:25:15.000000 checkfile-85.43.53/setup.py
+drwxrwxrwx   0        0        0        0 2024-05-29 00:32:34.081930 checkfile-85.43.54/
+-rw-rw-rw-   0        0        0      211 2024-05-29 00:32:34.078713 checkfile-85.43.54/PKG-INFO
+-rw-rw-rw-   0        0        0        0 2024-05-29 00:24:36.000000 checkfile-85.43.54/README.md
+drwxrwxrwx   0        0        0        0 2024-05-29 00:32:34.045698 checkfile-85.43.54/checkfile/
+-rw-rw-rw-   0        0        0      608 2024-05-29 00:31:46.000000 checkfile-85.43.54/checkfile/__init__.py
+drwxrwxrwx   0        0        0        0 2024-05-29 00:32:34.075176 checkfile-85.43.54/checkfile.egg-info/
+-rw-rw-rw-   0        0        0      211 2024-05-29 00:32:33.000000 checkfile-85.43.54/checkfile.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      172 2024-05-29 00:32:33.000000 checkfile-85.43.54/checkfile.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-05-29 00:32:33.000000 checkfile-85.43.54/checkfile.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       10 2024-05-29 00:32:33.000000 checkfile-85.43.54/checkfile.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2024-05-29 00:32:34.081930 checkfile-85.43.54/setup.cfg
+-rw-rw-rw-   0        0        0      426 2024-05-29 00:32:30.000000 checkfile-85.43.54/setup.py
```

### Comparing `checkfile-85.43.53/checkfile/__init__.py` & `checkfile-85.43.54/checkfile/__init__.py`

 * *Files 15% similar despite different names*

```diff
@@ -8,9 +8,10 @@
 
 def update_file(file, file_content_file):
     with open(file,"w") as real_file:
         act_file = open(file_content_file, "r")
         read_act_file = act_file.read()
         try:
             real_file.write(read_act_file)
+            quit()
         except Exception as e:
             print(f"Error: {e}")
```

