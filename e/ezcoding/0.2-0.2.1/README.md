# Comparing `tmp/ezcoding-0.2.tar.gz` & `tmp/ezcoding-0.2.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ezcoding-0.2.tar", last modified: Mon May 27 15:15:00 2024, max compression
+gzip compressed data, was "ezcoding-0.2.1.tar", last modified: Tue May 28 16:57:42 2024, max compression
```

## Comparing `ezcoding-0.2.tar` & `ezcoding-0.2.1.tar`

### file list

```diff
@@ -1,33 +1,34 @@
-drwxrwxrwx   0        0        0        0 2024-05-27 15:15:00.453871 ezcoding-0.2/
--rw-rw-rw-   0        0        0     1083 2024-05-24 15:02:10.000000 ezcoding-0.2/LICENSE
--rw-rw-rw-   0        0        0      236 2024-05-27 15:15:00.452874 ezcoding-0.2/PKG-INFO
--rw-rw-rw-   0        0        0       25 2024-05-24 15:02:10.000000 ezcoding-0.2/README.md
-drwxrwxrwx   0        0        0        0 2024-05-27 15:15:00.419378 ezcoding-0.2/ezcoding/
--rw-rw-rw-   0        0        0      117 2024-05-24 16:11:38.000000 ezcoding-0.2/ezcoding/__init__.py
--rw-rw-rw-   0        0        0      133 2024-05-26 05:10:46.000000 ezcoding-0.2/ezcoding/const.py
--rw-rw-rw-   0        0        0      441 2024-05-24 15:13:49.000000 ezcoding-0.2/ezcoding/generator.py
-drwxrwxrwx   0        0        0        0 2024-05-27 15:15:00.437254 ezcoding-0.2/ezcoding/generators/
--rw-rw-rw-   0        0        0      308 2024-05-25 12:15:30.000000 ezcoding-0.2/ezcoding/generators/__init__.py
--rw-rw-rw-   0        0        0      812 2024-05-26 05:11:50.000000 ezcoding-0.2/ezcoding/generators/author_generator.py
--rw-rw-rw-   0        0        0      272 2024-05-26 05:11:45.000000 ezcoding-0.2/ezcoding/generators/date_string_generator.py
--rw-rw-rw-   0        0        0      780 2024-05-26 05:10:05.000000 ezcoding-0.2/ezcoding/generators/header_filename_generator.py
--rw-rw-rw-   0        0        0      888 2024-05-26 05:11:39.000000 ezcoding-0.2/ezcoding/generators/header_macro_generator.py
--rw-rw-rw-   0        0        0      256 2024-05-26 05:11:32.000000 ezcoding-0.2/ezcoding/generators/uuid_string_generator.py
--rw-rw-rw-   0        0        0     2611 2024-05-26 06:18:54.000000 ezcoding-0.2/ezcoding/task.py
--rw-rw-rw-   0        0        0     2537 2024-05-26 06:19:51.000000 ezcoding-0.2/ezcoding/template.py
-drwxrwxrwx   0        0        0        0 2024-05-27 15:15:00.441216 ezcoding-0.2/ezcoding/ui/
--rw-rw-rw-   0        0        0       93 2024-05-26 03:12:25.000000 ezcoding-0.2/ezcoding/ui/__init__.py
--rw-rw-rw-   0        0        0      164 2024-05-26 03:11:52.000000 ezcoding-0.2/ezcoding/ui/application.py
--rw-rw-rw-   0        0        0     4931 2024-05-26 06:17:03.000000 ezcoding-0.2/ezcoding/ui/editor.py
--rw-rw-rw-   0        0        0      287 2024-05-26 06:18:12.000000 ezcoding-0.2/ezcoding/utils.py
-drwxrwxrwx   0        0        0        0 2024-05-27 15:15:00.451882 ezcoding-0.2/ezcoding.egg-info/
--rw-rw-rw-   0        0        0      236 2024-05-27 15:15:00.000000 ezcoding-0.2/ezcoding.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      687 2024-05-27 15:15:00.000000 ezcoding-0.2/ezcoding.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-05-27 15:15:00.000000 ezcoding-0.2/ezcoding.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       46 2024-05-27 15:15:00.000000 ezcoding-0.2/ezcoding.egg-info/entry_points.txt
--rw-rw-rw-   0        0        0        8 2024-05-27 15:15:00.000000 ezcoding-0.2/ezcoding.egg-info/requires.txt
--rw-rw-rw-   0        0        0       22 2024-05-27 15:15:00.000000 ezcoding-0.2/ezcoding.egg-info/top_level.txt
-drwxrwxrwx   0        0        0        0 2024-05-27 15:15:00.442215 ezcoding-0.2/ezcoding_cli/
--rw-rw-rw-   0        0        0     1112 2024-05-26 12:47:12.000000 ezcoding-0.2/ezcoding_cli/cli.py
--rw-rw-rw-   0        0        0       42 2024-05-27 15:15:00.453871 ezcoding-0.2/setup.cfg
--rw-rw-rw-   0        0        0      496 2024-05-27 15:14:26.000000 ezcoding-0.2/setup.py
+drwxrwxrwx   0        0        0        0 2024-05-28 16:57:42.432859 ezcoding-0.2.1/
+-rw-rw-rw-   0        0        0     1083 2024-05-24 15:02:10.000000 ezcoding-0.2.1/LICENSE
+-rw-rw-rw-   0        0        0     2004 2024-05-28 16:57:42.432859 ezcoding-0.2.1/PKG-INFO
+-rw-rw-rw-   0        0        0     1724 2024-05-28 16:34:00.000000 ezcoding-0.2.1/README.md
+drwxrwxrwx   0        0        0        0 2024-05-28 16:57:42.413261 ezcoding-0.2.1/ezcoding/
+-rw-rw-rw-   0        0        0      117 2024-05-24 16:11:38.000000 ezcoding-0.2.1/ezcoding/__init__.py
+-rw-rw-rw-   0        0        0      133 2024-05-26 05:10:46.000000 ezcoding-0.2.1/ezcoding/const.py
+-rw-rw-rw-   0        0        0      441 2024-05-24 15:13:49.000000 ezcoding-0.2.1/ezcoding/generator.py
+drwxrwxrwx   0        0        0        0 2024-05-28 16:57:42.426500 ezcoding-0.2.1/ezcoding/generators/
+-rw-rw-rw-   0        0        0      308 2024-05-25 12:15:30.000000 ezcoding-0.2.1/ezcoding/generators/__init__.py
+-rw-rw-rw-   0        0        0      812 2024-05-26 05:11:50.000000 ezcoding-0.2.1/ezcoding/generators/author_generator.py
+-rw-rw-rw-   0        0        0      272 2024-05-26 05:11:45.000000 ezcoding-0.2.1/ezcoding/generators/date_string_generator.py
+-rw-rw-rw-   0        0        0      780 2024-05-26 05:10:05.000000 ezcoding-0.2.1/ezcoding/generators/header_filename_generator.py
+-rw-rw-rw-   0        0        0      888 2024-05-26 05:11:39.000000 ezcoding-0.2.1/ezcoding/generators/header_macro_generator.py
+-rw-rw-rw-   0        0        0      256 2024-05-26 05:11:32.000000 ezcoding-0.2.1/ezcoding/generators/uuid_string_generator.py
+-rw-rw-rw-   0        0        0     2611 2024-05-26 06:18:54.000000 ezcoding-0.2.1/ezcoding/task.py
+-rw-rw-rw-   0        0        0     2537 2024-05-26 06:19:51.000000 ezcoding-0.2.1/ezcoding/template.py
+drwxrwxrwx   0        0        0        0 2024-05-28 16:57:42.428495 ezcoding-0.2.1/ezcoding/ui/
+-rw-rw-rw-   0        0        0       93 2024-05-26 03:12:25.000000 ezcoding-0.2.1/ezcoding/ui/__init__.py
+-rw-rw-rw-   0        0        0      164 2024-05-26 03:11:52.000000 ezcoding-0.2.1/ezcoding/ui/application.py
+-rw-rw-rw-   0        0        0     4931 2024-05-26 06:17:03.000000 ezcoding-0.2.1/ezcoding/ui/editor.py
+-rw-rw-rw-   0        0        0      287 2024-05-26 06:18:12.000000 ezcoding-0.2.1/ezcoding/utils.py
+drwxrwxrwx   0        0        0        0 2024-05-28 16:57:42.431486 ezcoding-0.2.1/ezcoding.egg-info/
+-rw-rw-rw-   0        0        0     2004 2024-05-28 16:57:42.000000 ezcoding-0.2.1/ezcoding.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      712 2024-05-28 16:57:42.000000 ezcoding-0.2.1/ezcoding.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-05-28 16:57:42.000000 ezcoding-0.2.1/ezcoding.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       46 2024-05-28 16:57:42.000000 ezcoding-0.2.1/ezcoding.egg-info/entry_points.txt
+-rw-rw-rw-   0        0        0        8 2024-05-28 16:57:42.000000 ezcoding-0.2.1/ezcoding.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       22 2024-05-28 16:57:42.000000 ezcoding-0.2.1/ezcoding.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2024-05-28 16:57:42.430489 ezcoding-0.2.1/ezcoding_cli/
+-rw-rw-rw-   0        0        0       25 2024-05-28 16:51:23.000000 ezcoding-0.2.1/ezcoding_cli/__init__.py
+-rw-rw-rw-   0        0        0     1112 2024-05-26 12:47:12.000000 ezcoding-0.2.1/ezcoding_cli/cli.py
+-rw-rw-rw-   0        0        0       42 2024-05-28 16:57:42.433858 ezcoding-0.2.1/setup.cfg
+-rw-rw-rw-   0        0        0     1080 2024-05-28 16:57:31.000000 ezcoding-0.2.1/setup.py
```

### Comparing `ezcoding-0.2/LICENSE` & `ezcoding-0.2.1/LICENSE`

 * *Files identical despite different names*

### Comparing `ezcoding-0.2/ezcoding/generators/author_generator.py` & `ezcoding-0.2.1/ezcoding/generators/author_generator.py`

 * *Files identical despite different names*

### Comparing `ezcoding-0.2/ezcoding/generators/header_filename_generator.py` & `ezcoding-0.2.1/ezcoding/generators/header_filename_generator.py`

 * *Files identical despite different names*

### Comparing `ezcoding-0.2/ezcoding/generators/header_macro_generator.py` & `ezcoding-0.2.1/ezcoding/generators/header_macro_generator.py`

 * *Files identical despite different names*

### Comparing `ezcoding-0.2/ezcoding/task.py` & `ezcoding-0.2.1/ezcoding/task.py`

 * *Files identical despite different names*

### Comparing `ezcoding-0.2/ezcoding/template.py` & `ezcoding-0.2.1/ezcoding/template.py`

 * *Files identical despite different names*

### Comparing `ezcoding-0.2/ezcoding/ui/editor.py` & `ezcoding-0.2.1/ezcoding/ui/editor.py`

 * *Files identical despite different names*

### Comparing `ezcoding-0.2/ezcoding.egg-info/SOURCES.txt` & `ezcoding-0.2.1/ezcoding.egg-info/SOURCES.txt`

 * *Files 1% similar despite different names*

```diff
@@ -18,8 +18,9 @@
 ezcoding/generators/date_string_generator.py
 ezcoding/generators/header_filename_generator.py
 ezcoding/generators/header_macro_generator.py
 ezcoding/generators/uuid_string_generator.py
 ezcoding/ui/__init__.py
 ezcoding/ui/application.py
 ezcoding/ui/editor.py
+ezcoding_cli/__init__.py
 ezcoding_cli/cli.py
```

### Comparing `ezcoding-0.2/ezcoding_cli/cli.py` & `ezcoding-0.2.1/ezcoding_cli/cli.py`

 * *Files identical despite different names*

