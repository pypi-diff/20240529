# Comparing `tmp/chip_cud_prompt-0.0.1.tar.gz` & `tmp/chip_cud_prompt-0.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "chip_cud_prompt-0.0.1.tar", last modified: Wed May 29 03:21:40 2024, max compression
+gzip compressed data, was "chip_cud_prompt-0.0.2.tar", last modified: Wed May 29 03:42:31 2024, max compression
```

## Comparing `chip_cud_prompt-0.0.1.tar` & `chip_cud_prompt-0.0.2.tar`

### file list

```diff
@@ -1,11 +1,16 @@
-drwxr-xr-x   0 zhangkaihua   (501) staff       (20)        0 2024-05-29 03:21:40.925362 chip_cud_prompt-0.0.1/
--rw-r--r--   0 zhangkaihua   (501) staff       (20)     1074 2024-05-29 03:20:58.000000 chip_cud_prompt-0.0.1/LICENSE
--rw-r--r--   0 zhangkaihua   (501) staff       (20)      567 2024-05-29 03:21:40.925214 chip_cud_prompt-0.0.1/PKG-INFO
--rw-r--r--   0 zhangkaihua   (501) staff       (20)       59 2024-05-29 02:43:10.000000 chip_cud_prompt-0.0.1/README.md
-drwxr-xr-x   0 zhangkaihua   (501) staff       (20)        0 2024-05-29 03:21:40.925054 chip_cud_prompt-0.0.1/chip_cud_prompt.egg-info/
--rw-r--r--   0 zhangkaihua   (501) staff       (20)      567 2024-05-29 03:21:40.000000 chip_cud_prompt-0.0.1/chip_cud_prompt.egg-info/PKG-INFO
--rw-r--r--   0 zhangkaihua   (501) staff       (20)      188 2024-05-29 03:21:40.000000 chip_cud_prompt-0.0.1/chip_cud_prompt.egg-info/SOURCES.txt
--rw-r--r--   0 zhangkaihua   (501) staff       (20)        1 2024-05-29 03:21:40.000000 chip_cud_prompt-0.0.1/chip_cud_prompt.egg-info/dependency_links.txt
--rw-r--r--   0 zhangkaihua   (501) staff       (20)        1 2024-05-29 03:21:40.000000 chip_cud_prompt-0.0.1/chip_cud_prompt.egg-info/top_level.txt
--rw-r--r--   0 zhangkaihua   (501) staff       (20)      577 2024-05-29 03:19:38.000000 chip_cud_prompt-0.0.1/pyproject.toml
--rw-r--r--   0 zhangkaihua   (501) staff       (20)       38 2024-05-29 03:21:40.925395 chip_cud_prompt-0.0.1/setup.cfg
+drwxr-xr-x   0 zhangkaihua   (501) staff       (20)        0 2024-05-29 03:42:31.882403 chip_cud_prompt-0.0.2/
+-rw-r--r--   0 zhangkaihua   (501) staff       (20)     1074 2024-05-29 03:20:58.000000 chip_cud_prompt-0.0.2/LICENSE
+-rw-r--r--   0 zhangkaihua   (501) staff       (20)      612 2024-05-29 03:42:31.882229 chip_cud_prompt-0.0.2/PKG-INFO
+-rw-r--r--   0 zhangkaihua   (501) staff       (20)      105 2024-05-29 03:32:59.000000 chip_cud_prompt-0.0.2/README.md
+-rw-r--r--   0 zhangkaihua   (501) staff       (20)      577 2024-05-29 03:42:18.000000 chip_cud_prompt-0.0.2/pyproject.toml
+-rw-r--r--   0 zhangkaihua   (501) staff       (20)       38 2024-05-29 03:42:31.882445 chip_cud_prompt-0.0.2/setup.cfg
+drwxr-xr-x   0 zhangkaihua   (501) staff       (20)        0 2024-05-29 03:42:31.880003 chip_cud_prompt-0.0.2/src/
+drwxr-xr-x   0 zhangkaihua   (501) staff       (20)        0 2024-05-29 03:42:31.881305 chip_cud_prompt-0.0.2/src/chip-cud-prompt/
+-rw-r--r--   0 zhangkaihua   (501) staff       (20)      168 2024-05-29 03:01:12.000000 chip_cud_prompt-0.0.2/src/chip-cud-prompt/__init__.py
+-rw-r--r--   0 zhangkaihua   (501) staff       (20)      413 2024-05-29 02:37:45.000000 chip_cud_prompt-0.0.2/src/chip-cud-prompt/abstract_prompt_manager.py
+-rw-r--r--   0 zhangkaihua   (501) staff       (20)      605 2024-05-29 03:18:53.000000 chip_cud_prompt-0.0.2/src/chip-cud-prompt/chip_create_prompt.py
+drwxr-xr-x   0 zhangkaihua   (501) staff       (20)        0 2024-05-29 03:42:31.882053 chip_cud_prompt-0.0.2/src/chip_cud_prompt.egg-info/
+-rw-r--r--   0 zhangkaihua   (501) staff       (20)      612 2024-05-29 03:42:31.000000 chip_cud_prompt-0.0.2/src/chip_cud_prompt.egg-info/PKG-INFO
+-rw-r--r--   0 zhangkaihua   (501) staff       (20)      325 2024-05-29 03:42:31.000000 chip_cud_prompt-0.0.2/src/chip_cud_prompt.egg-info/SOURCES.txt
+-rw-r--r--   0 zhangkaihua   (501) staff       (20)        1 2024-05-29 03:42:31.000000 chip_cud_prompt-0.0.2/src/chip_cud_prompt.egg-info/dependency_links.txt
+-rw-r--r--   0 zhangkaihua   (501) staff       (20)       16 2024-05-29 03:42:31.000000 chip_cud_prompt-0.0.2/src/chip_cud_prompt.egg-info/top_level.txt
```

### Comparing `chip_cud_prompt-0.0.1/LICENSE` & `chip_cud_prompt-0.0.2/LICENSE`

 * *Files identical despite different names*

### Comparing `chip_cud_prompt-0.0.1/PKG-INFO` & `chip_cud_prompt-0.0.2/PKG-INFO`

 * *Files 13% similar despite different names*

```diff
@@ -1,17 +1,24 @@
 Metadata-Version: 2.1
 Name: chip-cud-prompt
-Version: 0.0.1
+Version: 0.0.2
 Summary: A prompt package
 Author-email: zkhCreator <zkh90644@gmail.com>
 Project-URL: Homepage, https://github.com/zkhCreator/chip-cud-prompt
 Project-URL: Issues, https://github.com/zkhCreator/chip-cud-prompt/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.10
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
 # chip-cud-prompt
 
 用于管理存放入 ChipCud 的 prompt
+
+# Distribute
+
+```bash
+python3 -m build
+```
+
```

### Comparing `chip_cud_prompt-0.0.1/chip_cud_prompt.egg-info/PKG-INFO` & `chip_cud_prompt-0.0.2/src/chip_cud_prompt.egg-info/PKG-INFO`

 * *Files 13% similar despite different names*

```diff
@@ -1,17 +1,24 @@
 Metadata-Version: 2.1
 Name: chip-cud-prompt
-Version: 0.0.1
+Version: 0.0.2
 Summary: A prompt package
 Author-email: zkhCreator <zkh90644@gmail.com>
 Project-URL: Homepage, https://github.com/zkhCreator/chip-cud-prompt
 Project-URL: Issues, https://github.com/zkhCreator/chip-cud-prompt/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.10
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
 # chip-cud-prompt
 
 用于管理存放入 ChipCud 的 prompt
+
+# Distribute
+
+```bash
+python3 -m build
+```
+
```

### Comparing `chip_cud_prompt-0.0.1/pyproject.toml` & `chip_cud_prompt-0.0.2/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["setuptools>=61.0"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "chip-cud-prompt"
-version = "0.0.1"
+version = "0.0.2"
 authors = [
   { name="zkhCreator", email="zkh90644@gmail.com" },
 ]
 description = "A prompt package"
 readme = "README.md"
 requires-python = ">=3.10"
 classifiers = [
```

