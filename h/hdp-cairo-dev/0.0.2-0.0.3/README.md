# Comparing `tmp/hdp_cairo_dev-0.0.2.tar.gz` & `tmp/hdp_cairo_dev-0.0.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "hdp_cairo_dev-0.0.2.tar", last modified: Mon May 20 10:59:05 2024, max compression
+gzip compressed data, was "hdp_cairo_dev-0.0.3.tar", last modified: Wed May 29 14:19:04 2024, max compression
```

## Comparing `hdp_cairo_dev-0.0.2.tar` & `hdp_cairo_dev-0.0.3.tar`

### file list

```diff
@@ -1,42 +1,42 @@
-drwxr-xr-x   0 piapark    (501) staff       (20)        0 2024-05-20 10:59:05.988884 hdp_cairo_dev-0.0.2/
--rw-r--r--   0 piapark    (501) staff       (20)    11357 2024-05-09 07:20:00.000000 hdp_cairo_dev-0.0.2/LICENSE
--rw-r--r--   0 piapark    (501) staff       (20)     1163 2024-05-20 10:59:05.988654 hdp_cairo_dev-0.0.2/PKG-INFO
--rw-r--r--   0 piapark    (501) staff       (20)     4209 2024-05-07 06:11:21.000000 hdp_cairo_dev-0.0.2/README.md
-drwxr-xr-x   0 piapark    (501) staff       (20)        0 2024-05-20 10:59:05.988418 hdp_cairo_dev-0.0.2/hdp_cairo_dev.egg-info/
--rw-r--r--   0 piapark    (501) staff       (20)     1163 2024-05-20 10:59:05.000000 hdp_cairo_dev-0.0.2/hdp_cairo_dev.egg-info/PKG-INFO
--rw-r--r--   0 piapark    (501) staff       (20)      980 2024-05-20 10:59:05.000000 hdp_cairo_dev-0.0.2/hdp_cairo_dev.egg-info/SOURCES.txt
--rw-r--r--   0 piapark    (501) staff       (20)        1 2024-05-20 10:59:05.000000 hdp_cairo_dev-0.0.2/hdp_cairo_dev.egg-info/dependency_links.txt
--rw-r--r--   0 piapark    (501) staff       (20)        1 2024-05-20 09:52:51.000000 hdp_cairo_dev-0.0.2/hdp_cairo_dev.egg-info/not-zip-safe
--rw-r--r--   0 piapark    (501) staff       (20)      117 2024-05-20 10:59:05.000000 hdp_cairo_dev-0.0.2/hdp_cairo_dev.egg-info/requires.txt
--rw-r--r--   0 piapark    (501) staff       (20)       45 2024-05-20 10:59:05.000000 hdp_cairo_dev-0.0.2/hdp_cairo_dev.egg-info/top_level.txt
-drwxr-xr-x   0 piapark    (501) staff       (20)        0 2024-05-20 10:59:05.983559 hdp_cairo_dev-0.0.2/packages/
-drwxr-xr-x   0 piapark    (501) staff       (20)        0 2024-05-20 10:59:05.983680 hdp_cairo_dev-0.0.2/packages/hdp_bootloader/
-drwxr-xr-x   0 piapark    (501) staff       (20)        0 2024-05-20 10:59:05.986014 hdp_cairo_dev-0.0.2/packages/hdp_bootloader/bootloader/
--rw-r--r--   0 piapark    (501) staff       (20)      230 2024-05-13 12:30:29.000000 hdp_cairo_dev-0.0.2/packages/hdp_bootloader/bootloader/builtins.py
--rw-r--r--   0 piapark    (501) staff       (20)     9162 2024-05-15 09:37:59.000000 hdp_cairo_dev-0.0.2/packages/hdp_bootloader/bootloader/execute_task.cairo
--rw-r--r--   0 piapark    (501) staff       (20)     5320 2024-05-15 09:38:00.000000 hdp_cairo_dev-0.0.2/packages/hdp_bootloader/bootloader/hdp_bootloader.cairo
--rw-r--r--   0 piapark    (501) staff       (20)     5620 2024-05-17 05:44:46.000000 hdp_cairo_dev-0.0.2/packages/hdp_bootloader/bootloader/objects.py
--rw-r--r--   0 piapark    (501) staff       (20)    11723 2024-05-17 05:44:46.000000 hdp_cairo_dev-0.0.2/packages/hdp_bootloader/bootloader/utils.py
-drwxr-xr-x   0 piapark    (501) staff       (20)        0 2024-05-20 10:59:05.986494 hdp_cairo_dev-0.0.2/packages/hdp_bootloader/builtin_selection/
--rw-r--r--   0 piapark    (501) staff       (20)     3287 2024-05-13 12:30:29.000000 hdp_cairo_dev-0.0.2/packages/hdp_bootloader/builtin_selection/inner_select_builtins.cairo
--rw-r--r--   0 piapark    (501) staff       (20)     1861 2024-05-15 09:38:00.000000 hdp_cairo_dev-0.0.2/packages/hdp_bootloader/builtin_selection/select_input_builtins.cairo
--rw-r--r--   0 piapark    (501) staff       (20)     2238 2024-05-13 12:30:29.000000 hdp_cairo_dev-0.0.2/packages/hdp_bootloader/builtin_selection/validate_builtins.cairo
--rw-r--r--   0 piapark    (501) staff       (20)       38 2024-05-20 10:59:05.988927 hdp_cairo_dev-0.0.2/setup.cfg
--rw-r--r--   0 piapark    (501) staff       (20)     1293 2024-05-20 10:58:54.000000 hdp_cairo_dev-0.0.2/setup.py
-drwxr-xr-x   0 piapark    (501) staff       (20)        0 2024-05-20 10:59:05.983806 hdp_cairo_dev-0.0.2/src/
-drwxr-xr-x   0 piapark    (501) staff       (20)        0 2024-05-20 10:59:05.983858 hdp_cairo_dev-0.0.2/src/cairo1/
-drwxr-xr-x   0 piapark    (501) staff       (20)        0 2024-05-20 10:59:05.983907 hdp_cairo_dev-0.0.2/src/cairo1/simple_linear_regression/
-drwxr-xr-x   0 piapark    (501) staff       (20)        0 2024-05-20 10:59:05.983959 hdp_cairo_dev-0.0.2/src/cairo1/simple_linear_regression/target/
-drwxr-xr-x   0 piapark    (501) staff       (20)        0 2024-05-20 10:59:05.986642 hdp_cairo_dev-0.0.2/src/cairo1/simple_linear_regression/target/dev/
--rw-r--r--   0 piapark    (501) staff       (20)   495851 2024-05-20 09:44:37.000000 hdp_cairo_dev-0.0.2/src/cairo1/simple_linear_regression/target/dev/simple_linear_regression.sierra.json
-drwxr-xr-x   0 piapark    (501) staff       (20)        0 2024-05-20 10:59:05.984154 hdp_cairo_dev-0.0.2/tools/
-drwxr-xr-x   0 piapark    (501) staff       (20)        0 2024-05-20 10:59:05.987246 hdp_cairo_dev-0.0.2/tools/make/
--rw-r--r--   0 piapark    (501) staff       (20)        0 2024-05-13 12:30:29.000000 hdp_cairo_dev-0.0.2/tools/make/__init__.py
--rwxr-xr-x   0 piapark    (501) staff       (20)     7746 2024-05-08 07:04:44.000000 hdp_cairo_dev-0.0.2/tools/make/launch_cairo_files.py
-drwxr-xr-x   0 piapark    (501) staff       (20)        0 2024-05-20 10:59:05.988216 hdp_cairo_dev-0.0.2/tools/py/
--rw-r--r--   0 piapark    (501) staff       (20)        0 2024-05-13 12:30:29.000000 hdp_cairo_dev-0.0.2/tools/py/__init__.py
--rw-r--r--   0 piapark    (501) staff       (20)     7204 2024-05-07 06:11:21.000000 hdp_cairo_dev-0.0.2/tools/py/block_header.py
--rw-r--r--   0 piapark    (501) staff       (20)     2653 2024-05-07 06:11:21.000000 hdp_cairo_dev-0.0.2/tools/py/fetch_block_headers.py
--rw-r--r--   0 piapark    (501) staff       (20)     1313 2024-05-08 07:04:44.000000 hdp_cairo_dev-0.0.2/tools/py/fetch_tx.py
--rw-r--r--   0 piapark    (501) staff       (20)    11579 2024-05-08 07:04:44.000000 hdp_cairo_dev-0.0.2/tools/py/transaction.py
--rw-r--r--   0 piapark    (501) staff       (20)     7368 2024-05-08 07:04:44.000000 hdp_cairo_dev-0.0.2/tools/py/utils.py
+drwxr-xr-x   0 piapark    (501) staff       (20)        0 2024-05-29 14:19:04.421631 hdp_cairo_dev-0.0.3/
+-rw-r--r--   0 piapark    (501) staff       (20)    11357 2024-05-09 07:20:00.000000 hdp_cairo_dev-0.0.3/LICENSE
+-rw-r--r--   0 piapark    (501) staff       (20)     1163 2024-05-29 14:19:04.421411 hdp_cairo_dev-0.0.3/PKG-INFO
+-rw-r--r--   0 piapark    (501) staff       (20)     4209 2024-05-07 06:11:21.000000 hdp_cairo_dev-0.0.3/README.md
+drwxr-xr-x   0 piapark    (501) staff       (20)        0 2024-05-29 14:19:04.421170 hdp_cairo_dev-0.0.3/hdp_cairo_dev.egg-info/
+-rw-r--r--   0 piapark    (501) staff       (20)     1163 2024-05-29 14:19:04.000000 hdp_cairo_dev-0.0.3/hdp_cairo_dev.egg-info/PKG-INFO
+-rw-r--r--   0 piapark    (501) staff       (20)      980 2024-05-29 14:19:04.000000 hdp_cairo_dev-0.0.3/hdp_cairo_dev.egg-info/SOURCES.txt
+-rw-r--r--   0 piapark    (501) staff       (20)        1 2024-05-29 14:19:04.000000 hdp_cairo_dev-0.0.3/hdp_cairo_dev.egg-info/dependency_links.txt
+-rw-r--r--   0 piapark    (501) staff       (20)        1 2024-05-20 09:52:51.000000 hdp_cairo_dev-0.0.3/hdp_cairo_dev.egg-info/not-zip-safe
+-rw-r--r--   0 piapark    (501) staff       (20)      117 2024-05-29 14:19:04.000000 hdp_cairo_dev-0.0.3/hdp_cairo_dev.egg-info/requires.txt
+-rw-r--r--   0 piapark    (501) staff       (20)       45 2024-05-29 14:19:04.000000 hdp_cairo_dev-0.0.3/hdp_cairo_dev.egg-info/top_level.txt
+drwxr-xr-x   0 piapark    (501) staff       (20)        0 2024-05-29 14:19:04.415339 hdp_cairo_dev-0.0.3/packages/
+drwxr-xr-x   0 piapark    (501) staff       (20)        0 2024-05-29 14:19:04.415454 hdp_cairo_dev-0.0.3/packages/hdp_bootloader/
+drwxr-xr-x   0 piapark    (501) staff       (20)        0 2024-05-29 14:19:04.418616 hdp_cairo_dev-0.0.3/packages/hdp_bootloader/bootloader/
+-rw-r--r--   0 piapark    (501) staff       (20)      230 2024-05-13 12:30:29.000000 hdp_cairo_dev-0.0.3/packages/hdp_bootloader/bootloader/builtins.py
+-rw-r--r--   0 piapark    (501) staff       (20)     9162 2024-05-15 09:37:59.000000 hdp_cairo_dev-0.0.3/packages/hdp_bootloader/bootloader/execute_task.cairo
+-rw-r--r--   0 piapark    (501) staff       (20)     5320 2024-05-15 09:38:00.000000 hdp_cairo_dev-0.0.3/packages/hdp_bootloader/bootloader/hdp_bootloader.cairo
+-rw-r--r--   0 piapark    (501) staff       (20)     5620 2024-05-17 05:44:46.000000 hdp_cairo_dev-0.0.3/packages/hdp_bootloader/bootloader/objects.py
+-rw-r--r--   0 piapark    (501) staff       (20)    11723 2024-05-17 05:44:46.000000 hdp_cairo_dev-0.0.3/packages/hdp_bootloader/bootloader/utils.py
+drwxr-xr-x   0 piapark    (501) staff       (20)        0 2024-05-29 14:19:04.419093 hdp_cairo_dev-0.0.3/packages/hdp_bootloader/builtin_selection/
+-rw-r--r--   0 piapark    (501) staff       (20)     3287 2024-05-13 12:30:29.000000 hdp_cairo_dev-0.0.3/packages/hdp_bootloader/builtin_selection/inner_select_builtins.cairo
+-rw-r--r--   0 piapark    (501) staff       (20)     1861 2024-05-15 09:38:00.000000 hdp_cairo_dev-0.0.3/packages/hdp_bootloader/builtin_selection/select_input_builtins.cairo
+-rw-r--r--   0 piapark    (501) staff       (20)     2238 2024-05-13 12:30:29.000000 hdp_cairo_dev-0.0.3/packages/hdp_bootloader/builtin_selection/validate_builtins.cairo
+-rw-r--r--   0 piapark    (501) staff       (20)       38 2024-05-29 14:19:04.421677 hdp_cairo_dev-0.0.3/setup.cfg
+-rw-r--r--   0 piapark    (501) staff       (20)     1294 2024-05-29 10:43:53.000000 hdp_cairo_dev-0.0.3/setup.py
+drwxr-xr-x   0 piapark    (501) staff       (20)        0 2024-05-29 14:19:04.415570 hdp_cairo_dev-0.0.3/src/
+drwxr-xr-x   0 piapark    (501) staff       (20)        0 2024-05-29 14:19:04.415618 hdp_cairo_dev-0.0.3/src/cairo1/
+drwxr-xr-x   0 piapark    (501) staff       (20)        0 2024-05-29 14:19:04.415668 hdp_cairo_dev-0.0.3/src/cairo1/simple_linear_regression/
+drwxr-xr-x   0 piapark    (501) staff       (20)        0 2024-05-29 14:19:04.415716 hdp_cairo_dev-0.0.3/src/cairo1/simple_linear_regression/target/
+drwxr-xr-x   0 piapark    (501) staff       (20)        0 2024-05-29 14:19:04.419236 hdp_cairo_dev-0.0.3/src/cairo1/simple_linear_regression/target/dev/
+-rw-r--r--   0 piapark    (501) staff       (20)   663527 2024-05-29 14:16:42.000000 hdp_cairo_dev-0.0.3/src/cairo1/simple_linear_regression/target/dev/simple_linear_regression.sierra.json
+drwxr-xr-x   0 piapark    (501) staff       (20)        0 2024-05-29 14:19:04.415888 hdp_cairo_dev-0.0.3/tools/
+drwxr-xr-x   0 piapark    (501) staff       (20)        0 2024-05-29 14:19:04.419844 hdp_cairo_dev-0.0.3/tools/make/
+-rw-r--r--   0 piapark    (501) staff       (20)        0 2024-05-13 12:30:29.000000 hdp_cairo_dev-0.0.3/tools/make/__init__.py
+-rwxr-xr-x   0 piapark    (501) staff       (20)     7746 2024-05-08 07:04:44.000000 hdp_cairo_dev-0.0.3/tools/make/launch_cairo_files.py
+drwxr-xr-x   0 piapark    (501) staff       (20)        0 2024-05-29 14:19:04.420889 hdp_cairo_dev-0.0.3/tools/py/
+-rw-r--r--   0 piapark    (501) staff       (20)        0 2024-05-13 12:30:29.000000 hdp_cairo_dev-0.0.3/tools/py/__init__.py
+-rw-r--r--   0 piapark    (501) staff       (20)     7204 2024-05-07 06:11:21.000000 hdp_cairo_dev-0.0.3/tools/py/block_header.py
+-rw-r--r--   0 piapark    (501) staff       (20)     2653 2024-05-07 06:11:21.000000 hdp_cairo_dev-0.0.3/tools/py/fetch_block_headers.py
+-rw-r--r--   0 piapark    (501) staff       (20)     1313 2024-05-08 07:04:44.000000 hdp_cairo_dev-0.0.3/tools/py/fetch_tx.py
+-rw-r--r--   0 piapark    (501) staff       (20)    11579 2024-05-08 07:04:44.000000 hdp_cairo_dev-0.0.3/tools/py/transaction.py
+-rw-r--r--   0 piapark    (501) staff       (20)     7368 2024-05-08 07:04:44.000000 hdp_cairo_dev-0.0.3/tools/py/utils.py
```

### Comparing `hdp_cairo_dev-0.0.2/LICENSE` & `hdp_cairo_dev-0.0.3/LICENSE`

 * *Files identical despite different names*

### Comparing `hdp_cairo_dev-0.0.2/PKG-INFO` & `hdp_cairo_dev-0.0.3/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: hdp-cairo-dev
-Version: 0.0.2
+Version: 0.0.3
 Description-Content-Type: text/markdown
 License-File: LICENSE
 Requires-Dist: aiofiles==23.2.1
 Requires-Dist: cairo-lang==0.13.1
 Requires-Dist: typeguard==2.13.3
 Requires-Dist: protobuf==3.20.3
 Requires-Dist: inquirer
```

### Comparing `hdp_cairo_dev-0.0.2/README.md` & `hdp_cairo_dev-0.0.3/README.md`

 * *Files identical despite different names*

### Comparing `hdp_cairo_dev-0.0.2/hdp_cairo_dev.egg-info/PKG-INFO` & `hdp_cairo_dev-0.0.3/hdp_cairo_dev.egg-info/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: hdp-cairo-dev
-Version: 0.0.2
+Version: 0.0.3
 Description-Content-Type: text/markdown
 License-File: LICENSE
 Requires-Dist: aiofiles==23.2.1
 Requires-Dist: cairo-lang==0.13.1
 Requires-Dist: typeguard==2.13.3
 Requires-Dist: protobuf==3.20.3
 Requires-Dist: inquirer
```

### Comparing `hdp_cairo_dev-0.0.2/hdp_cairo_dev.egg-info/SOURCES.txt` & `hdp_cairo_dev-0.0.3/hdp_cairo_dev.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `hdp_cairo_dev-0.0.2/packages/hdp_bootloader/bootloader/execute_task.cairo` & `hdp_cairo_dev-0.0.3/packages/hdp_bootloader/bootloader/execute_task.cairo`

 * *Files identical despite different names*

### Comparing `hdp_cairo_dev-0.0.2/packages/hdp_bootloader/bootloader/hdp_bootloader.cairo` & `hdp_cairo_dev-0.0.3/packages/hdp_bootloader/bootloader/hdp_bootloader.cairo`

 * *Files identical despite different names*

### Comparing `hdp_cairo_dev-0.0.2/packages/hdp_bootloader/bootloader/objects.py` & `hdp_cairo_dev-0.0.3/packages/hdp_bootloader/bootloader/objects.py`

 * *Files identical despite different names*

### Comparing `hdp_cairo_dev-0.0.2/packages/hdp_bootloader/bootloader/utils.py` & `hdp_cairo_dev-0.0.3/packages/hdp_bootloader/bootloader/utils.py`

 * *Files identical despite different names*

### Comparing `hdp_cairo_dev-0.0.2/packages/hdp_bootloader/builtin_selection/inner_select_builtins.cairo` & `hdp_cairo_dev-0.0.3/packages/hdp_bootloader/builtin_selection/inner_select_builtins.cairo`

 * *Files identical despite different names*

### Comparing `hdp_cairo_dev-0.0.2/packages/hdp_bootloader/builtin_selection/select_input_builtins.cairo` & `hdp_cairo_dev-0.0.3/packages/hdp_bootloader/builtin_selection/select_input_builtins.cairo`

 * *Files identical despite different names*

### Comparing `hdp_cairo_dev-0.0.2/packages/hdp_bootloader/builtin_selection/validate_builtins.cairo` & `hdp_cairo_dev-0.0.3/packages/hdp_bootloader/builtin_selection/validate_builtins.cairo`

 * *Files identical despite different names*

### Comparing `hdp_cairo_dev-0.0.2/setup.py` & `hdp_cairo_dev-0.0.3/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,11 +1,12 @@
 from setuptools import setup
 from setuptools.command.install import install
 
 from pathlib import Path
+
 this_directory = Path(__file__).parent
 long_description = (this_directory / "package.md").read_text()
 
 
 class PostInstallCommand(install):
     """Custom post-installation for installation mode."""
 
@@ -17,16 +18,16 @@
 # Read the requirements from the requirements.txt file
 with open("tools/make/requirements.txt") as requirements_file:
     requirements = requirements_file.read().splitlines()
 
 setup(
     name="hdp-cairo-dev",
     long_description=long_description,
-    long_description_content_type='text/markdown',
-    version="0.0.2",
+    long_description_content_type="text/markdown",
+    version="0.0.3",
     packages=["hdp_bootloader", "tools", "compiled_cairo1_modules"],
     install_requires=requirements,
     package_dir={
         "tools": "tools",
         "hdp_bootloader": "packages/hdp_bootloader",
         "compiled_cairo1_modules": "src/cairo1",
     },
```

### Comparing `hdp_cairo_dev-0.0.2/tools/make/launch_cairo_files.py` & `hdp_cairo_dev-0.0.3/tools/make/launch_cairo_files.py`

 * *Files identical despite different names*

### Comparing `hdp_cairo_dev-0.0.2/tools/py/block_header.py` & `hdp_cairo_dev-0.0.3/tools/py/block_header.py`

 * *Files identical despite different names*

### Comparing `hdp_cairo_dev-0.0.2/tools/py/fetch_block_headers.py` & `hdp_cairo_dev-0.0.3/tools/py/fetch_block_headers.py`

 * *Files identical despite different names*

### Comparing `hdp_cairo_dev-0.0.2/tools/py/fetch_tx.py` & `hdp_cairo_dev-0.0.3/tools/py/fetch_tx.py`

 * *Files identical despite different names*

### Comparing `hdp_cairo_dev-0.0.2/tools/py/transaction.py` & `hdp_cairo_dev-0.0.3/tools/py/transaction.py`

 * *Files identical despite different names*

### Comparing `hdp_cairo_dev-0.0.2/tools/py/utils.py` & `hdp_cairo_dev-0.0.3/tools/py/utils.py`

 * *Files identical despite different names*

