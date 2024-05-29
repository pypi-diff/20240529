# Comparing `tmp/anonipy-0.0.4.tar.gz` & `tmp/anonipy-0.0.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "anonipy-0.0.4.tar", last modified: Mon May 27 20:23:33 2024, max compression
+gzip compressed data, was "anonipy-0.0.5.tar", last modified: Wed May 29 17:35:23 2024, max compression
```

## Comparing `anonipy-0.0.4.tar` & `anonipy-0.0.5.tar`

### file list

```diff
@@ -1,50 +1,51 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-27 20:23:33.356148 anonipy-0.0.4/
--rw-r--r--   0 runner    (1001) docker     (127)     1319 2024-05-27 20:23:29.000000 anonipy-0.0.4/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)     7601 2024-05-27 20:23:33.356148 anonipy-0.0.4/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     4569 2024-05-27 20:23:29.000000 anonipy-0.0.4/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-27 20:23:33.348147 anonipy-0.0.4/anonipy/
--rw-r--r--   0 runner    (1001) docker     (127)      455 2024-05-27 20:23:29.000000 anonipy-0.0.4/anonipy/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-27 20:23:33.352148 anonipy-0.0.4/anonipy/anonymize/
--rw-r--r--   0 runner    (1001) docker     (127)      159 2024-05-27 20:23:29.000000 anonipy-0.0.4/anonipy/anonymize/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-27 20:23:33.352148 anonipy-0.0.4/anonipy/anonymize/extractors/
--rw-r--r--   0 runner    (1001) docker     (127)      141 2024-05-27 20:23:29.000000 anonipy-0.0.4/anonipy/anonymize/extractors/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2825 2024-05-27 20:23:29.000000 anonipy-0.0.4/anonipy/anonymize/extractors/entity_extractor.py
--rw-r--r--   0 runner    (1001) docker     (127)      292 2024-05-27 20:23:29.000000 anonipy-0.0.4/anonipy/anonymize/extractors/interface.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-27 20:23:33.352148 anonipy-0.0.4/anonipy/anonymize/generators/
--rw-r--r--   0 runner    (1001) docker     (127)      370 2024-05-27 20:23:29.000000 anonipy-0.0.4/anonipy/anonymize/generators/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2249 2024-05-27 20:23:29.000000 anonipy-0.0.4/anonipy/anonymize/generators/date_generator.py
--rw-r--r--   0 runner    (1001) docker     (127)      287 2024-05-27 20:23:29.000000 anonipy-0.0.4/anonipy/anonymize/generators/interface.py
--rw-r--r--   0 runner    (1001) docker     (127)     5452 2024-05-27 20:23:29.000000 anonipy-0.0.4/anonipy/anonymize/generators/llm_label_generator.py
--rw-r--r--   0 runner    (1001) docker     (127)     3954 2024-05-27 20:23:29.000000 anonipy-0.0.4/anonipy/anonymize/generators/mask_label_generator.py
--rw-r--r--   0 runner    (1001) docker     (127)      882 2024-05-27 20:23:29.000000 anonipy-0.0.4/anonipy/anonymize/generators/number_generator.py
--rw-r--r--   0 runner    (1001) docker     (127)      317 2024-05-27 20:23:29.000000 anonipy-0.0.4/anonipy/anonymize/helpers.py
--rw-r--r--   0 runner    (1001) docker     (127)     1537 2024-05-27 20:23:29.000000 anonipy-0.0.4/anonipy/anonymize/regex.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-27 20:23:33.352148 anonipy-0.0.4/anonipy/anonymize/strategies/
--rw-r--r--   0 runner    (1001) docker     (127)      295 2024-05-27 20:23:29.000000 anonipy-0.0.4/anonipy/anonymize/strategies/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      374 2024-05-27 20:23:29.000000 anonipy-0.0.4/anonipy/anonymize/strategies/interface.py
--rw-r--r--   0 runner    (1001) docker     (127)     1334 2024-05-27 20:23:29.000000 anonipy-0.0.4/anonipy/anonymize/strategies/masking.py
--rw-r--r--   0 runner    (1001) docker     (127)     1762 2024-05-27 20:23:29.000000 anonipy-0.0.4/anonipy/anonymize/strategies/pseudonymization.py
--rw-r--r--   0 runner    (1001) docker     (127)     1095 2024-05-27 20:23:29.000000 anonipy-0.0.4/anonipy/anonymize/strategies/redaction.py
--rw-r--r--   0 runner    (1001) docker     (127)      752 2024-05-27 20:23:29.000000 anonipy-0.0.4/anonipy/constants.py
--rw-r--r--   0 runner    (1001) docker     (127)      446 2024-05-27 20:23:29.000000 anonipy-0.0.4/anonipy/definitions.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-27 20:23:33.352148 anonipy-0.0.4/anonipy/utils/
--rw-r--r--   0 runner    (1001) docker     (127)      107 2024-05-27 20:23:29.000000 anonipy-0.0.4/anonipy/utils/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1598 2024-05-27 20:23:29.000000 anonipy-0.0.4/anonipy/utils/file_system.py
--rw-r--r--   0 runner    (1001) docker     (127)      907 2024-05-27 20:23:29.000000 anonipy-0.0.4/anonipy/utils/language_detector.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-27 20:23:33.356148 anonipy-0.0.4/anonipy.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     7601 2024-05-27 20:23:33.000000 anonipy-0.0.4/anonipy.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     1250 2024-05-27 20:23:33.000000 anonipy-0.0.4/anonipy.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-27 20:23:33.000000 anonipy-0.0.4/anonipy.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)      238 2024-05-27 20:23:33.000000 anonipy-0.0.4/anonipy.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)        8 2024-05-27 20:23:33.000000 anonipy-0.0.4/anonipy.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)     1295 2024-05-27 20:23:29.000000 anonipy-0.0.4/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)      164 2024-05-27 20:23:29.000000 anonipy-0.0.4/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (127)       70 2024-05-27 20:23:33.356148 anonipy-0.0.4/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-27 20:23:33.356148 anonipy-0.0.4/test/
--rw-r--r--   0 runner    (1001) docker     (127)      621 2024-05-27 20:23:29.000000 anonipy-0.0.4/test/test_entity.py
--rw-r--r--   0 runner    (1001) docker     (127)     3632 2024-05-27 20:23:29.000000 anonipy-0.0.4/test/test_extractors.py
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-27 20:23:29.000000 anonipy-0.0.4/test/test_file_system.py
--rw-r--r--   0 runner    (1001) docker     (127)     7563 2024-05-27 20:23:29.000000 anonipy-0.0.4/test/test_generators.py
--rw-r--r--   0 runner    (1001) docker     (127)     3883 2024-05-27 20:23:29.000000 anonipy-0.0.4/test/test_language_detector.py
--rw-r--r--   0 runner    (1001) docker     (127)     1949 2024-05-27 20:23:29.000000 anonipy-0.0.4/test/test_regex.py
--rw-r--r--   0 runner    (1001) docker     (127)     8353 2024-05-27 20:23:29.000000 anonipy-0.0.4/test/test_strategies.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-29 17:35:23.054713 anonipy-0.0.5/
+-rw-r--r--   0 runner    (1001) docker     (127)     1319 2024-05-29 17:35:19.000000 anonipy-0.0.5/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)     7635 2024-05-29 17:35:23.054713 anonipy-0.0.5/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     4579 2024-05-29 17:35:19.000000 anonipy-0.0.5/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-29 17:35:23.046712 anonipy-0.0.5/anonipy/
+-rw-r--r--   0 runner    (1001) docker     (127)      488 2024-05-29 17:35:19.000000 anonipy-0.0.5/anonipy/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-29 17:35:23.050713 anonipy-0.0.5/anonipy/anonymize/
+-rw-r--r--   0 runner    (1001) docker     (127)      159 2024-05-29 17:35:19.000000 anonipy-0.0.5/anonipy/anonymize/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-29 17:35:23.050713 anonipy-0.0.5/anonipy/anonymize/extractors/
+-rw-r--r--   0 runner    (1001) docker     (127)      141 2024-05-29 17:35:19.000000 anonipy-0.0.5/anonipy/anonymize/extractors/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2825 2024-05-29 17:35:19.000000 anonipy-0.0.5/anonipy/anonymize/extractors/entity_extractor.py
+-rw-r--r--   0 runner    (1001) docker     (127)      292 2024-05-29 17:35:19.000000 anonipy-0.0.5/anonipy/anonymize/extractors/interface.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-29 17:35:23.050713 anonipy-0.0.5/anonipy/anonymize/generators/
+-rw-r--r--   0 runner    (1001) docker     (127)      370 2024-05-29 17:35:19.000000 anonipy-0.0.5/anonipy/anonymize/generators/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2249 2024-05-29 17:35:19.000000 anonipy-0.0.5/anonipy/anonymize/generators/date_generator.py
+-rw-r--r--   0 runner    (1001) docker     (127)      287 2024-05-29 17:35:19.000000 anonipy-0.0.5/anonipy/anonymize/generators/interface.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5452 2024-05-29 17:35:19.000000 anonipy-0.0.5/anonipy/anonymize/generators/llm_label_generator.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3954 2024-05-29 17:35:19.000000 anonipy-0.0.5/anonipy/anonymize/generators/mask_label_generator.py
+-rw-r--r--   0 runner    (1001) docker     (127)      882 2024-05-29 17:35:19.000000 anonipy-0.0.5/anonipy/anonymize/generators/number_generator.py
+-rw-r--r--   0 runner    (1001) docker     (127)      317 2024-05-29 17:35:19.000000 anonipy-0.0.5/anonipy/anonymize/helpers.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1537 2024-05-29 17:35:19.000000 anonipy-0.0.5/anonipy/anonymize/regex.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-29 17:35:23.050713 anonipy-0.0.5/anonipy/anonymize/strategies/
+-rw-r--r--   0 runner    (1001) docker     (127)      295 2024-05-29 17:35:19.000000 anonipy-0.0.5/anonipy/anonymize/strategies/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      374 2024-05-29 17:35:19.000000 anonipy-0.0.5/anonipy/anonymize/strategies/interface.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1334 2024-05-29 17:35:19.000000 anonipy-0.0.5/anonipy/anonymize/strategies/masking.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1762 2024-05-29 17:35:19.000000 anonipy-0.0.5/anonipy/anonymize/strategies/pseudonymization.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1095 2024-05-29 17:35:19.000000 anonipy-0.0.5/anonipy/anonymize/strategies/redaction.py
+-rw-r--r--   0 runner    (1001) docker     (127)      752 2024-05-29 17:35:19.000000 anonipy-0.0.5/anonipy/constants.py
+-rw-r--r--   0 runner    (1001) docker     (127)      446 2024-05-29 17:35:19.000000 anonipy-0.0.5/anonipy/definitions.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-29 17:35:23.050713 anonipy-0.0.5/anonipy/utils/
+-rw-r--r--   0 runner    (1001) docker     (127)      107 2024-05-29 17:35:19.000000 anonipy-0.0.5/anonipy/utils/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3784 2024-05-29 17:35:19.000000 anonipy-0.0.5/anonipy/utils/file_system.py
+-rw-r--r--   0 runner    (1001) docker     (127)      907 2024-05-29 17:35:19.000000 anonipy-0.0.5/anonipy/utils/language_detector.py
+-rw-r--r--   0 runner    (1001) docker     (127)       22 2024-05-29 17:35:19.000000 anonipy-0.0.5/anonipy/version.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-29 17:35:23.054713 anonipy-0.0.5/anonipy.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     7635 2024-05-29 17:35:23.000000 anonipy-0.0.5/anonipy.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     1269 2024-05-29 17:35:23.000000 anonipy-0.0.5/anonipy.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-29 17:35:23.000000 anonipy-0.0.5/anonipy.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      247 2024-05-29 17:35:23.000000 anonipy-0.0.5/anonipy.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        8 2024-05-29 17:35:23.000000 anonipy-0.0.5/anonipy.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)     1295 2024-05-29 17:35:19.000000 anonipy-0.0.5/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)      173 2024-05-29 17:35:19.000000 anonipy-0.0.5/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       70 2024-05-29 17:35:23.054713 anonipy-0.0.5/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-29 17:35:23.054713 anonipy-0.0.5/test/
+-rw-r--r--   0 runner    (1001) docker     (127)      621 2024-05-29 17:35:19.000000 anonipy-0.0.5/test/test_entity.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3867 2024-05-29 17:35:19.000000 anonipy-0.0.5/test/test_extractors.py
+-rw-r--r--   0 runner    (1001) docker     (127)      883 2024-05-29 17:35:19.000000 anonipy-0.0.5/test/test_file_system.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7797 2024-05-29 17:35:19.000000 anonipy-0.0.5/test/test_generators.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4117 2024-05-29 17:35:19.000000 anonipy-0.0.5/test/test_language_detector.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1949 2024-05-29 17:35:19.000000 anonipy-0.0.5/test/test_regex.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8353 2024-05-29 17:35:19.000000 anonipy-0.0.5/test/test_strategies.py
```

### Comparing `anonipy-0.0.4/LICENSE` & `anonipy-0.0.5/LICENSE`

 * *Files identical despite different names*

### Comparing `anonipy-0.0.4/PKG-INFO` & `anonipy-0.0.5/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: anonipy
-Version: 0.0.4
+Version: 0.0.5
 Summary: The data anonymization package
 Author-email: Erik Novak <erik.novak@ijs.si>
 License: BSD 2-Clause License
         
         Copyright (c) 2024, Erik Novak
         All rights reserved.
         
@@ -46,15 +46,16 @@
 Requires-Dist: gliner
 Requires-Dist: gliner-spacy
 Requires-Dist: transformers
 Requires-Dist: bitsandbytes
 Requires-Dist: lingua-language-detector
 Requires-Dist: guidance==0.1.14
 Requires-Dist: sentencepiece
-Requires-Dist: textract
+Requires-Dist: pypdf
+Requires-Dist: python-docx
 Requires-Dist: tqdm
 Provides-Extra: dev
 Requires-Dist: black; extra == "dev"
 Requires-Dist: flake8; extra == "dev"
 Requires-Dist: python-githooks; extra == "dev"
 Requires-Dist: mkdocs-material; extra == "dev"
 Requires-Dist: mkdocs-jupyter; extra == "dev"
@@ -95,15 +96,15 @@
 ---
 
 The anonipy package is a python package for data anonymization. It is designed to be simple to use and highly customizable, supporting different anonymization strategies. Powered by LLMs.
 
 ## ✅ Requirements
 Before starting the project make sure these requirements are available:
 
-- [python]. The python programming language (v3.8 or higher).
+- [python]. The python programming language (v3.8, v3.9, v3.10, v3.11).
 
 ## 💾 Install
 
 ```bash
 pip install anonipy
 ```
```

### Comparing `anonipy-0.0.4/README.md` & `anonipy-0.0.5/README.md`

 * *Files 2% similar despite different names*

```diff
@@ -29,15 +29,15 @@
 ---
 
 The anonipy package is a python package for data anonymization. It is designed to be simple to use and highly customizable, supporting different anonymization strategies. Powered by LLMs.
 
 ## ✅ Requirements
 Before starting the project make sure these requirements are available:
 
-- [python]. The python programming language (v3.8 or higher).
+- [python]. The python programming language (v3.8, v3.9, v3.10, v3.11).
 
 ## 💾 Install
 
 ```bash
 pip install anonipy
 ```
```

### Comparing `anonipy-0.0.4/anonipy/anonymize/extractors/entity_extractor.py` & `anonipy-0.0.5/anonipy/anonymize/extractors/entity_extractor.py`

 * *Files identical despite different names*

### Comparing `anonipy-0.0.4/anonipy/anonymize/generators/date_generator.py` & `anonipy-0.0.5/anonipy/anonymize/generators/date_generator.py`

 * *Files identical despite different names*

### Comparing `anonipy-0.0.4/anonipy/anonymize/generators/llm_label_generator.py` & `anonipy-0.0.5/anonipy/anonymize/generators/llm_label_generator.py`

 * *Files identical despite different names*

### Comparing `anonipy-0.0.4/anonipy/anonymize/generators/mask_label_generator.py` & `anonipy-0.0.5/anonipy/anonymize/generators/mask_label_generator.py`

 * *Files identical despite different names*

### Comparing `anonipy-0.0.4/anonipy/anonymize/generators/number_generator.py` & `anonipy-0.0.5/anonipy/anonymize/generators/number_generator.py`

 * *Files identical despite different names*

### Comparing `anonipy-0.0.4/anonipy/anonymize/regex.py` & `anonipy-0.0.5/anonipy/anonymize/regex.py`

 * *Files identical despite different names*

### Comparing `anonipy-0.0.4/anonipy/anonymize/strategies/masking.py` & `anonipy-0.0.5/anonipy/anonymize/strategies/masking.py`

 * *Files identical despite different names*

### Comparing `anonipy-0.0.4/anonipy/anonymize/strategies/pseudonymization.py` & `anonipy-0.0.5/anonipy/anonymize/strategies/pseudonymization.py`

 * *Files identical despite different names*

### Comparing `anonipy-0.0.4/anonipy/anonymize/strategies/redaction.py` & `anonipy-0.0.5/anonipy/anonymize/strategies/redaction.py`

 * *Files identical despite different names*

### Comparing `anonipy-0.0.4/anonipy/constants.py` & `anonipy-0.0.5/anonipy/constants.py`

 * *Files identical despite different names*

### Comparing `anonipy-0.0.4/anonipy/utils/language_detector.py` & `anonipy-0.0.5/anonipy/utils/language_detector.py`

 * *Files identical despite different names*

### Comparing `anonipy-0.0.4/anonipy.egg-info/PKG-INFO` & `anonipy-0.0.5/anonipy.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: anonipy
-Version: 0.0.4
+Version: 0.0.5
 Summary: The data anonymization package
 Author-email: Erik Novak <erik.novak@ijs.si>
 License: BSD 2-Clause License
         
         Copyright (c) 2024, Erik Novak
         All rights reserved.
         
@@ -46,15 +46,16 @@
 Requires-Dist: gliner
 Requires-Dist: gliner-spacy
 Requires-Dist: transformers
 Requires-Dist: bitsandbytes
 Requires-Dist: lingua-language-detector
 Requires-Dist: guidance==0.1.14
 Requires-Dist: sentencepiece
-Requires-Dist: textract
+Requires-Dist: pypdf
+Requires-Dist: python-docx
 Requires-Dist: tqdm
 Provides-Extra: dev
 Requires-Dist: black; extra == "dev"
 Requires-Dist: flake8; extra == "dev"
 Requires-Dist: python-githooks; extra == "dev"
 Requires-Dist: mkdocs-material; extra == "dev"
 Requires-Dist: mkdocs-jupyter; extra == "dev"
@@ -95,15 +96,15 @@
 ---
 
 The anonipy package is a python package for data anonymization. It is designed to be simple to use and highly customizable, supporting different anonymization strategies. Powered by LLMs.
 
 ## ✅ Requirements
 Before starting the project make sure these requirements are available:
 
-- [python]. The python programming language (v3.8 or higher).
+- [python]. The python programming language (v3.8, v3.9, v3.10, v3.11).
 
 ## 💾 Install
 
 ```bash
 pip install anonipy
 ```
```

### Comparing `anonipy-0.0.4/anonipy.egg-info/SOURCES.txt` & `anonipy-0.0.5/anonipy.egg-info/SOURCES.txt`

 * *Files 4% similar despite different names*

```diff
@@ -2,14 +2,15 @@
 README.md
 pyproject.toml
 requirements.txt
 setup.cfg
 anonipy/__init__.py
 anonipy/constants.py
 anonipy/definitions.py
+anonipy/version.py
 anonipy.egg-info/PKG-INFO
 anonipy.egg-info/SOURCES.txt
 anonipy.egg-info/dependency_links.txt
 anonipy.egg-info/requires.txt
 anonipy.egg-info/top_level.txt
 anonipy/anonymize/__init__.py
 anonipy/anonymize/helpers.py
```

### Comparing `anonipy-0.0.4/pyproject.toml` & `anonipy-0.0.5/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 [build-system]
 requires = ['setuptools>=42']
 build-backend = 'setuptools.build_meta'
 
 [project]
-version = "0.0.4"
+version = "0.0.5"
 name = "anonipy"
 description = "The data anonymization package"
 authors=[{ name = "Erik Novak", email = "erik.novak@ijs.si" }]
 readme = "README.md"
 license = { file = "LICENSE" }
 dynamic = ["dependencies"]
 keywords = ["python", "machine learning", "natural language processing", "anonymization"]
```

### Comparing `anonipy-0.0.4/test/test_entity.py` & `anonipy-0.0.5/test/test_entity.py`

 * *Files identical despite different names*

### Comparing `anonipy-0.0.4/test/test_extractors.py` & `anonipy-0.0.5/test/test_extractors.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,8 +1,9 @@
 import unittest
+import warnings
 
 from anonipy.definitions import Entity
 from anonipy.anonymize.extractors import EntityExtractor
 from anonipy.constants import LANGUAGES
 
 # =====================================
 # Helper functions
@@ -93,14 +94,20 @@
 
 # =====================================
 # Test Entity Extractor
 # =====================================
 
 
 class TestEntityExtractor(unittest.TestCase):
+
+    def setUp(self):
+        warnings.filterwarnings("ignore", category=ImportWarning)
+        warnings.filterwarnings("ignore", category=UserWarning)
+        warnings.filterwarnings("ignore", category=FutureWarning)
+
     def test_init(self):
         try:
             EntityExtractor()
         except Exception as e:
             self.assertRaises(TypeError, e)
 
     def test_init_inputs(self):
```

### Comparing `anonipy-0.0.4/test/test_generators.py` & `anonipy-0.0.5/test/test_generators.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,9 +1,10 @@
 import re
 import unittest
+import warnings
 
 import torch
 
 from anonipy.definitions import Entity
 from anonipy.anonymize.generators import (
     LLMLabelGenerator,
     MaskLabelGenerator,
@@ -120,14 +121,19 @@
 
 class TestMaskLabelGenerator(unittest.TestCase):
 
     @classmethod
     def setUpClass(self):
         self.generator = MaskLabelGenerator()
 
+    def setUp(self):
+        warnings.filterwarnings("ignore", category=ImportWarning)
+        warnings.filterwarnings("ignore", category=UserWarning)
+        warnings.filterwarnings("ignore", category=FutureWarning)
+
     def test_has_methods(self):
         self.assertEqual(hasattr(self.generator, "generate"), True)
 
     def test_generate_default(self):
         entity = test_entities["name"]
         generated_text = self.generator.generate(entity, text=original_text)
         match = re.match(entity.regex, generated_text)
```

### Comparing `anonipy-0.0.4/test/test_language_detector.py` & `anonipy-0.0.5/test/test_language_detector.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,19 +1,25 @@
 import unittest
+import warnings
 
 from anonipy.utils.language_detector import LanguageDetector
 from anonipy.constants import LANGUAGES
 
 # =====================================
 # Test Language Detector
 # =====================================
 
 
 class TestLanguageDetector(unittest.TestCase):
 
+    def setUp(self):
+        warnings.filterwarnings("ignore", category=ImportWarning)
+        warnings.filterwarnings("ignore", category=UserWarning)
+        warnings.filterwarnings("ignore", category=FutureWarning)
+
     def test_init(self):
         language_detector = LanguageDetector()
         self.assertEqual(language_detector.__class__, LanguageDetector)
 
     def test_has_methods(self):
         language_detector = LanguageDetector()
         self.assertEqual(hasattr(language_detector, "detect"), True)
```

### Comparing `anonipy-0.0.4/test/test_regex.py` & `anonipy-0.0.5/test/test_regex.py`

 * *Files identical despite different names*

### Comparing `anonipy-0.0.4/test/test_strategies.py` & `anonipy-0.0.5/test/test_strategies.py`

 * *Files identical despite different names*

