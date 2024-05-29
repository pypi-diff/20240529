# Comparing `tmp/instruct-qa-0.0.3rc2.tar.gz` & `tmp/instruct-qa-0.0.3rc3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "instruct-qa-0.0.3rc2.tar", last modified: Wed May 29 03:23:30 2024, max compression
+gzip compressed data, was "instruct-qa-0.0.3rc3.tar", last modified: Wed May 29 06:08:12 2024, max compression
```

## Comparing `instruct-qa-0.0.3rc2.tar` & `instruct-qa-0.0.3rc3.tar`

### file list

```diff
@@ -1,56 +1,56 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-29 03:23:30.115282 instruct-qa-0.0.3rc2/
--rw-r--r--   0 runner    (1001) docker     (127)    11356 2024-05-29 03:23:17.000000 instruct-qa-0.0.3rc2/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)    10421 2024-05-29 03:23:30.111282 instruct-qa-0.0.3rc2/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     8184 2024-05-29 03:23:17.000000 instruct-qa-0.0.3rc2/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-29 03:23:30.107282 instruct-qa-0.0.3rc2/instruct_qa/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-29 03:23:17.000000 instruct-qa-0.0.3rc2/instruct_qa/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-29 03:23:30.107282 instruct-qa-0.0.3rc2/instruct_qa/collections/
--rw-r--r--   0 runner    (1001) docker     (127)      843 2024-05-29 03:23:17.000000 instruct-qa-0.0.3rc2/instruct_qa/collections/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2620 2024-05-29 03:23:17.000000 instruct-qa-0.0.3rc2/instruct_qa/collections/dpr_wiki_collection.py
--rw-r--r--   0 runner    (1001) docker     (127)     1229 2024-05-29 03:23:17.000000 instruct-qa-0.0.3rc2/instruct_qa/collections/faithdial_collection.py
--rw-r--r--   0 runner    (1001) docker     (127)     1789 2024-05-29 03:23:17.000000 instruct-qa-0.0.3rc2/instruct_qa/collections/hotpot_wiki_collection.py
--rw-r--r--   0 runner    (1001) docker     (127)     2747 2024-05-29 03:23:17.000000 instruct-qa-0.0.3rc2/instruct_qa/collections/topiocqa_wiki_collection.py
--rw-r--r--   0 runner    (1001) docker     (127)     1244 2024-05-29 03:23:17.000000 instruct-qa-0.0.3rc2/instruct_qa/collections/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-29 03:23:30.107282 instruct-qa-0.0.3rc2/instruct_qa/dataset/
--rw-r--r--   0 runner    (1001) docker     (127)      152 2024-05-29 03:23:17.000000 instruct-qa-0.0.3rc2/instruct_qa/dataset/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-29 03:23:30.111282 instruct-qa-0.0.3rc2/instruct_qa/dataset/convqa/
--rw-r--r--   0 runner    (1001) docker     (127)       78 2024-05-29 03:23:17.000000 instruct-qa-0.0.3rc2/instruct_qa/dataset/convqa/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1726 2024-05-29 03:23:17.000000 instruct-qa-0.0.3rc2/instruct_qa/dataset/convqa/faithdial.py
--rw-r--r--   0 runner    (1001) docker     (127)     2680 2024-05-29 03:23:17.000000 instruct-qa-0.0.3rc2/instruct_qa/dataset/convqa/topiocqa.py
--rw-r--r--   0 runner    (1001) docker     (127)      562 2024-05-29 03:23:17.000000 instruct-qa-0.0.3rc2/instruct_qa/dataset/dataset.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-29 03:23:30.111282 instruct-qa-0.0.3rc2/instruct_qa/dataset/qa/
--rw-r--r--   0 runner    (1001) docker     (127)      134 2024-05-29 03:23:17.000000 instruct-qa-0.0.3rc2/instruct_qa/dataset/qa/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      982 2024-05-29 03:23:17.000000 instruct-qa-0.0.3rc2/instruct_qa/dataset/qa/generic_qa.py
--rw-r--r--   0 runner    (1001) docker     (127)     1346 2024-05-29 03:23:17.000000 instruct-qa-0.0.3rc2/instruct_qa/dataset/qa/hotpot_qa.py
--rw-r--r--   0 runner    (1001) docker     (127)     1391 2024-05-29 03:23:17.000000 instruct-qa-0.0.3rc2/instruct_qa/dataset/qa/natural_questions.py
--rw-r--r--   0 runner    (1001) docker     (127)      971 2024-05-29 03:23:17.000000 instruct-qa-0.0.3rc2/instruct_qa/dataset/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-29 03:23:30.111282 instruct-qa-0.0.3rc2/instruct_qa/evaluation/
--rw-r--r--   0 runner    (1001) docker     (127)     1396 2024-05-29 03:23:17.000000 instruct-qa-0.0.3rc2/instruct_qa/evaluation/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    36811 2024-05-29 03:23:17.000000 instruct-qa-0.0.3rc2/instruct_qa/evaluation/faithfulness_metrics.py
--rw-r--r--   0 runner    (1001) docker     (127)    24381 2024-05-29 03:23:17.000000 instruct-qa-0.0.3rc2/instruct_qa/evaluation/metrics.py
--rw-r--r--   0 runner    (1001) docker     (127)     1475 2024-05-29 03:23:17.000000 instruct-qa-0.0.3rc2/instruct_qa/evaluation/utils.py
--rw-r--r--   0 runner    (1001) docker     (127)     4898 2024-05-29 03:23:17.000000 instruct-qa-0.0.3rc2/instruct_qa/experiment_utils.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-29 03:23:30.111282 instruct-qa-0.0.3rc2/instruct_qa/generation/
--rw-r--r--   0 runner    (1001) docker     (127)      139 2024-05-29 03:23:17.000000 instruct-qa-0.0.3rc2/instruct_qa/generation/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    14023 2024-05-29 03:23:17.000000 instruct-qa-0.0.3rc2/instruct_qa/generation/generator.py
--rw-r--r--   0 runner    (1001) docker     (127)     1128 2024-05-29 03:23:17.000000 instruct-qa-0.0.3rc2/instruct_qa/generation/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-29 03:23:30.111282 instruct-qa-0.0.3rc2/instruct_qa/prompt/
--rw-r--r--   0 runner    (1001) docker     (127)      279 2024-05-29 03:23:17.000000 instruct-qa-0.0.3rc2/instruct_qa/prompt/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     7875 2024-05-29 03:23:17.000000 instruct-qa-0.0.3rc2/instruct_qa/prompt/templates.py
--rw-r--r--   0 runner    (1001) docker     (127)     1131 2024-05-29 03:23:17.000000 instruct-qa-0.0.3rc2/instruct_qa/prompt/utils.py
--rw-r--r--   0 runner    (1001) docker     (127)     5376 2024-05-29 03:23:17.000000 instruct-qa-0.0.3rc2/instruct_qa/response_runner.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-29 03:23:30.111282 instruct-qa-0.0.3rc2/instruct_qa/retrieval/
--rw-r--r--   0 runner    (1001) docker     (127)     6821 2024-05-29 03:23:17.000000 instruct-qa-0.0.3rc2/instruct_qa/retrieval/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    15445 2024-05-29 03:23:17.000000 instruct-qa-0.0.3rc2/instruct_qa/retrieval/index.py
--rw-r--r--   0 runner    (1001) docker     (127)     7320 2024-05-29 03:23:17.000000 instruct-qa-0.0.3rc2/instruct_qa/retrieval/pyserini_utils.py
--rw-r--r--   0 runner    (1001) docker     (127)     8462 2024-05-29 03:23:17.000000 instruct-qa-0.0.3rc2/instruct_qa/retrieval/utils.py
--rw-r--r--   0 runner    (1001) docker     (127)       25 2024-05-29 03:23:18.000000 instruct-qa-0.0.3rc2/instruct_qa/version.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-29 03:23:30.107282 instruct-qa-0.0.3rc2/instruct_qa.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)    10421 2024-05-29 03:23:29.000000 instruct-qa-0.0.3rc2/instruct_qa.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     1450 2024-05-29 03:23:30.000000 instruct-qa-0.0.3rc2/instruct_qa.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-29 03:23:29.000000 instruct-qa-0.0.3rc2/instruct_qa.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-29 03:23:29.000000 instruct-qa-0.0.3rc2/instruct_qa.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (127)      733 2024-05-29 03:23:29.000000 instruct-qa-0.0.3rc2/instruct_qa.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       12 2024-05-29 03:23:29.000000 instruct-qa-0.0.3rc2/instruct_qa.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-29 03:23:30.115282 instruct-qa-0.0.3rc2/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)     2143 2024-05-29 03:23:17.000000 instruct-qa-0.0.3rc2/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-29 06:08:12.547660 instruct-qa-0.0.3rc3/
+-rw-r--r--   0 runner    (1001) docker     (127)    11356 2024-05-29 06:08:03.000000 instruct-qa-0.0.3rc3/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)    10421 2024-05-29 06:08:12.547660 instruct-qa-0.0.3rc3/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     8184 2024-05-29 06:08:03.000000 instruct-qa-0.0.3rc3/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-29 06:08:12.539660 instruct-qa-0.0.3rc3/instruct_qa/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-29 06:08:03.000000 instruct-qa-0.0.3rc3/instruct_qa/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-29 06:08:12.543660 instruct-qa-0.0.3rc3/instruct_qa/collections/
+-rw-r--r--   0 runner    (1001) docker     (127)      843 2024-05-29 06:08:03.000000 instruct-qa-0.0.3rc3/instruct_qa/collections/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2620 2024-05-29 06:08:03.000000 instruct-qa-0.0.3rc3/instruct_qa/collections/dpr_wiki_collection.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1229 2024-05-29 06:08:03.000000 instruct-qa-0.0.3rc3/instruct_qa/collections/faithdial_collection.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1789 2024-05-29 06:08:03.000000 instruct-qa-0.0.3rc3/instruct_qa/collections/hotpot_wiki_collection.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2747 2024-05-29 06:08:03.000000 instruct-qa-0.0.3rc3/instruct_qa/collections/topiocqa_wiki_collection.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1244 2024-05-29 06:08:03.000000 instruct-qa-0.0.3rc3/instruct_qa/collections/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-29 06:08:12.543660 instruct-qa-0.0.3rc3/instruct_qa/dataset/
+-rw-r--r--   0 runner    (1001) docker     (127)      152 2024-05-29 06:08:03.000000 instruct-qa-0.0.3rc3/instruct_qa/dataset/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-29 06:08:12.543660 instruct-qa-0.0.3rc3/instruct_qa/dataset/convqa/
+-rw-r--r--   0 runner    (1001) docker     (127)       78 2024-05-29 06:08:03.000000 instruct-qa-0.0.3rc3/instruct_qa/dataset/convqa/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1726 2024-05-29 06:08:03.000000 instruct-qa-0.0.3rc3/instruct_qa/dataset/convqa/faithdial.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2680 2024-05-29 06:08:03.000000 instruct-qa-0.0.3rc3/instruct_qa/dataset/convqa/topiocqa.py
+-rw-r--r--   0 runner    (1001) docker     (127)      562 2024-05-29 06:08:03.000000 instruct-qa-0.0.3rc3/instruct_qa/dataset/dataset.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-29 06:08:12.543660 instruct-qa-0.0.3rc3/instruct_qa/dataset/qa/
+-rw-r--r--   0 runner    (1001) docker     (127)      134 2024-05-29 06:08:03.000000 instruct-qa-0.0.3rc3/instruct_qa/dataset/qa/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      982 2024-05-29 06:08:03.000000 instruct-qa-0.0.3rc3/instruct_qa/dataset/qa/generic_qa.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1346 2024-05-29 06:08:03.000000 instruct-qa-0.0.3rc3/instruct_qa/dataset/qa/hotpot_qa.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1391 2024-05-29 06:08:03.000000 instruct-qa-0.0.3rc3/instruct_qa/dataset/qa/natural_questions.py
+-rw-r--r--   0 runner    (1001) docker     (127)      971 2024-05-29 06:08:03.000000 instruct-qa-0.0.3rc3/instruct_qa/dataset/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-29 06:08:12.543660 instruct-qa-0.0.3rc3/instruct_qa/evaluation/
+-rw-r--r--   0 runner    (1001) docker     (127)     1396 2024-05-29 06:08:03.000000 instruct-qa-0.0.3rc3/instruct_qa/evaluation/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    36811 2024-05-29 06:08:03.000000 instruct-qa-0.0.3rc3/instruct_qa/evaluation/faithfulness_metrics.py
+-rw-r--r--   0 runner    (1001) docker     (127)    24381 2024-05-29 06:08:03.000000 instruct-qa-0.0.3rc3/instruct_qa/evaluation/metrics.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1475 2024-05-29 06:08:03.000000 instruct-qa-0.0.3rc3/instruct_qa/evaluation/utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4898 2024-05-29 06:08:03.000000 instruct-qa-0.0.3rc3/instruct_qa/experiment_utils.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-29 06:08:12.547660 instruct-qa-0.0.3rc3/instruct_qa/generation/
+-rw-r--r--   0 runner    (1001) docker     (127)      139 2024-05-29 06:08:03.000000 instruct-qa-0.0.3rc3/instruct_qa/generation/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    14144 2024-05-29 06:08:03.000000 instruct-qa-0.0.3rc3/instruct_qa/generation/generator.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1128 2024-05-29 06:08:03.000000 instruct-qa-0.0.3rc3/instruct_qa/generation/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-29 06:08:12.547660 instruct-qa-0.0.3rc3/instruct_qa/prompt/
+-rw-r--r--   0 runner    (1001) docker     (127)      279 2024-05-29 06:08:03.000000 instruct-qa-0.0.3rc3/instruct_qa/prompt/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7875 2024-05-29 06:08:03.000000 instruct-qa-0.0.3rc3/instruct_qa/prompt/templates.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1131 2024-05-29 06:08:03.000000 instruct-qa-0.0.3rc3/instruct_qa/prompt/utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5376 2024-05-29 06:08:03.000000 instruct-qa-0.0.3rc3/instruct_qa/response_runner.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-29 06:08:12.547660 instruct-qa-0.0.3rc3/instruct_qa/retrieval/
+-rw-r--r--   0 runner    (1001) docker     (127)     6821 2024-05-29 06:08:03.000000 instruct-qa-0.0.3rc3/instruct_qa/retrieval/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    15445 2024-05-29 06:08:03.000000 instruct-qa-0.0.3rc3/instruct_qa/retrieval/index.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7320 2024-05-29 06:08:03.000000 instruct-qa-0.0.3rc3/instruct_qa/retrieval/pyserini_utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8462 2024-05-29 06:08:03.000000 instruct-qa-0.0.3rc3/instruct_qa/retrieval/utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)       25 2024-05-29 06:08:03.000000 instruct-qa-0.0.3rc3/instruct_qa/version.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-29 06:08:12.543660 instruct-qa-0.0.3rc3/instruct_qa.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)    10421 2024-05-29 06:08:12.000000 instruct-qa-0.0.3rc3/instruct_qa.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     1450 2024-05-29 06:08:12.000000 instruct-qa-0.0.3rc3/instruct_qa.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-29 06:08:12.000000 instruct-qa-0.0.3rc3/instruct_qa.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-29 06:08:12.000000 instruct-qa-0.0.3rc3/instruct_qa.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (127)      733 2024-05-29 06:08:12.000000 instruct-qa-0.0.3rc3/instruct_qa.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       12 2024-05-29 06:08:12.000000 instruct-qa-0.0.3rc3/instruct_qa.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-29 06:08:12.547660 instruct-qa-0.0.3rc3/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)     2143 2024-05-29 06:08:03.000000 instruct-qa-0.0.3rc3/setup.py
```

### Comparing `instruct-qa-0.0.3rc2/LICENSE` & `instruct-qa-0.0.3rc3/LICENSE`

 * *Files identical despite different names*

### Comparing `instruct-qa-0.0.3rc2/PKG-INFO` & `instruct-qa-0.0.3rc3/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: instruct-qa
-Version: 0.0.3rc2
+Version: 0.0.3rc3
 Summary: Empirical evaluation of retrieval-augmented instruction-following models.
 Home-page: https://github.com/McGill-NLP/instruct-qa
 Author: McGill NLP
 License: UNKNOWN
 Description: # Evaluating Correctness and Faithfulness of Instruction-Following Models for Question Answering
         
         [![arXiv](https://img.shields.io/badge/arXiv-2307.16877-b31b1b.svg)](https://arxiv.org/abs/2307.16877)
```

### Comparing `instruct-qa-0.0.3rc2/README.md` & `instruct-qa-0.0.3rc3/README.md`

 * *Files identical despite different names*

### Comparing `instruct-qa-0.0.3rc2/instruct_qa/collections/__init__.py` & `instruct-qa-0.0.3rc3/instruct_qa/collections/__init__.py`

 * *Files identical despite different names*

### Comparing `instruct-qa-0.0.3rc2/instruct_qa/collections/dpr_wiki_collection.py` & `instruct-qa-0.0.3rc3/instruct_qa/collections/dpr_wiki_collection.py`

 * *Files identical despite different names*

### Comparing `instruct-qa-0.0.3rc2/instruct_qa/collections/faithdial_collection.py` & `instruct-qa-0.0.3rc3/instruct_qa/collections/faithdial_collection.py`

 * *Files identical despite different names*

### Comparing `instruct-qa-0.0.3rc2/instruct_qa/collections/hotpot_wiki_collection.py` & `instruct-qa-0.0.3rc3/instruct_qa/collections/hotpot_wiki_collection.py`

 * *Files identical despite different names*

### Comparing `instruct-qa-0.0.3rc2/instruct_qa/collections/topiocqa_wiki_collection.py` & `instruct-qa-0.0.3rc3/instruct_qa/collections/topiocqa_wiki_collection.py`

 * *Files identical despite different names*

### Comparing `instruct-qa-0.0.3rc2/instruct_qa/collections/utils.py` & `instruct-qa-0.0.3rc3/instruct_qa/collections/utils.py`

 * *Files identical despite different names*

### Comparing `instruct-qa-0.0.3rc2/instruct_qa/dataset/convqa/faithdial.py` & `instruct-qa-0.0.3rc3/instruct_qa/dataset/convqa/faithdial.py`

 * *Files identical despite different names*

### Comparing `instruct-qa-0.0.3rc2/instruct_qa/dataset/convqa/topiocqa.py` & `instruct-qa-0.0.3rc3/instruct_qa/dataset/convqa/topiocqa.py`

 * *Files identical despite different names*

### Comparing `instruct-qa-0.0.3rc2/instruct_qa/dataset/dataset.py` & `instruct-qa-0.0.3rc3/instruct_qa/dataset/dataset.py`

 * *Files identical despite different names*

### Comparing `instruct-qa-0.0.3rc2/instruct_qa/dataset/qa/generic_qa.py` & `instruct-qa-0.0.3rc3/instruct_qa/dataset/qa/generic_qa.py`

 * *Files identical despite different names*

### Comparing `instruct-qa-0.0.3rc2/instruct_qa/dataset/qa/hotpot_qa.py` & `instruct-qa-0.0.3rc3/instruct_qa/dataset/qa/hotpot_qa.py`

 * *Files identical despite different names*

### Comparing `instruct-qa-0.0.3rc2/instruct_qa/dataset/qa/natural_questions.py` & `instruct-qa-0.0.3rc3/instruct_qa/dataset/qa/natural_questions.py`

 * *Files identical despite different names*

### Comparing `instruct-qa-0.0.3rc2/instruct_qa/dataset/utils.py` & `instruct-qa-0.0.3rc3/instruct_qa/dataset/utils.py`

 * *Files identical despite different names*

### Comparing `instruct-qa-0.0.3rc2/instruct_qa/evaluation/__init__.py` & `instruct-qa-0.0.3rc3/instruct_qa/evaluation/__init__.py`

 * *Files identical despite different names*

### Comparing `instruct-qa-0.0.3rc2/instruct_qa/evaluation/faithfulness_metrics.py` & `instruct-qa-0.0.3rc3/instruct_qa/evaluation/faithfulness_metrics.py`

 * *Files identical despite different names*

### Comparing `instruct-qa-0.0.3rc2/instruct_qa/evaluation/metrics.py` & `instruct-qa-0.0.3rc3/instruct_qa/evaluation/metrics.py`

 * *Files identical despite different names*

### Comparing `instruct-qa-0.0.3rc2/instruct_qa/evaluation/utils.py` & `instruct-qa-0.0.3rc3/instruct_qa/evaluation/utils.py`

 * *Files identical despite different names*

### Comparing `instruct-qa-0.0.3rc2/instruct_qa/experiment_utils.py` & `instruct-qa-0.0.3rc3/instruct_qa/experiment_utils.py`

 * *Files identical despite different names*

### Comparing `instruct-qa-0.0.3rc2/instruct_qa/generation/generator.py` & `instruct-qa-0.0.3rc3/instruct_qa/generation/generator.py`

 * *Files 1% similar despite different names*

```diff
@@ -66,14 +66,17 @@
         openai.api_key = self.api_key
         self.model_map = {
             "gpt-3.5-turbo": "chat",
             "gpt-4": "chat",
             "text-davinci-003": "completions",
             "text-davinci-002": "completions",
         }
+        if "completion_type" in kwargs:
+            self.model_map[self.model_name] = kwargs["completion_type"]
+        
         assert (
             self.model_name in self.model_map
         ), "You should add the model name to the model -> endpoint compatibility mappings."
         assert self.model_map[self.model_name] in [
             "chat",
             "completions",
         ], "Only chat and completions endpoints are implemented. You may want to add other configurations."
```

### Comparing `instruct-qa-0.0.3rc2/instruct_qa/generation/utils.py` & `instruct-qa-0.0.3rc3/instruct_qa/generation/utils.py`

 * *Files identical despite different names*

### Comparing `instruct-qa-0.0.3rc2/instruct_qa/prompt/templates.py` & `instruct-qa-0.0.3rc3/instruct_qa/prompt/templates.py`

 * *Files identical despite different names*

### Comparing `instruct-qa-0.0.3rc2/instruct_qa/prompt/utils.py` & `instruct-qa-0.0.3rc3/instruct_qa/prompt/utils.py`

 * *Files identical despite different names*

### Comparing `instruct-qa-0.0.3rc2/instruct_qa/response_runner.py` & `instruct-qa-0.0.3rc3/instruct_qa/response_runner.py`

 * *Files identical despite different names*

### Comparing `instruct-qa-0.0.3rc2/instruct_qa/retrieval/__init__.py` & `instruct-qa-0.0.3rc3/instruct_qa/retrieval/__init__.py`

 * *Files identical despite different names*

### Comparing `instruct-qa-0.0.3rc2/instruct_qa/retrieval/index.py` & `instruct-qa-0.0.3rc3/instruct_qa/retrieval/index.py`

 * *Files identical despite different names*

### Comparing `instruct-qa-0.0.3rc2/instruct_qa/retrieval/pyserini_utils.py` & `instruct-qa-0.0.3rc3/instruct_qa/retrieval/pyserini_utils.py`

 * *Files identical despite different names*

### Comparing `instruct-qa-0.0.3rc2/instruct_qa/retrieval/utils.py` & `instruct-qa-0.0.3rc3/instruct_qa/retrieval/utils.py`

 * *Files identical despite different names*

### Comparing `instruct-qa-0.0.3rc2/instruct_qa.egg-info/PKG-INFO` & `instruct-qa-0.0.3rc3/instruct_qa.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: instruct-qa
-Version: 0.0.3rc2
+Version: 0.0.3rc3
 Summary: Empirical evaluation of retrieval-augmented instruction-following models.
 Home-page: https://github.com/McGill-NLP/instruct-qa
 Author: McGill NLP
 License: UNKNOWN
 Description: # Evaluating Correctness and Faithfulness of Instruction-Following Models for Question Answering
         
         [![arXiv](https://img.shields.io/badge/arXiv-2307.16877-b31b1b.svg)](https://arxiv.org/abs/2307.16877)
```

### Comparing `instruct-qa-0.0.3rc2/instruct_qa.egg-info/SOURCES.txt` & `instruct-qa-0.0.3rc3/instruct_qa.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `instruct-qa-0.0.3rc2/instruct_qa.egg-info/requires.txt` & `instruct-qa-0.0.3rc3/instruct_qa.egg-info/requires.txt`

 * *Files identical despite different names*

### Comparing `instruct-qa-0.0.3rc2/setup.py` & `instruct-qa-0.0.3rc3/setup.py`

 * *Files identical despite different names*

