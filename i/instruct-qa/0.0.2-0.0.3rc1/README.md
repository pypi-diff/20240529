# Comparing `tmp/instruct-qa-0.0.2.tar.gz` & `tmp/instruct-qa-0.0.3rc1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "instruct-qa-0.0.2.tar", last modified: Tue Sep 19 19:46:09 2023, max compression
+gzip compressed data, was "instruct-qa-0.0.3rc1.tar", last modified: Wed May 29 03:10:01 2024, max compression
```

## Comparing `instruct-qa-0.0.2.tar` & `instruct-qa-0.0.3rc1.tar`

### file list

```diff
@@ -1,56 +1,56 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-09-19 19:46:09.838400 instruct-qa-0.0.2/
--rw-r--r--   0 runner    (1001) docker     (127)    11356 2023-09-19 19:45:56.000000 instruct-qa-0.0.2/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)     8403 2023-09-19 19:46:09.838400 instruct-qa-0.0.2/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     6480 2023-09-19 19:45:56.000000 instruct-qa-0.0.2/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-09-19 19:46:09.830400 instruct-qa-0.0.2/instruct_qa/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2023-09-19 19:45:56.000000 instruct-qa-0.0.2/instruct_qa/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-09-19 19:46:09.834400 instruct-qa-0.0.2/instruct_qa/collections/
--rw-r--r--   0 runner    (1001) docker     (127)      843 2023-09-19 19:45:56.000000 instruct-qa-0.0.2/instruct_qa/collections/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2620 2023-09-19 19:45:56.000000 instruct-qa-0.0.2/instruct_qa/collections/dpr_wiki_collection.py
--rw-r--r--   0 runner    (1001) docker     (127)     1229 2023-09-19 19:45:56.000000 instruct-qa-0.0.2/instruct_qa/collections/faithdial_collection.py
--rw-r--r--   0 runner    (1001) docker     (127)     1789 2023-09-19 19:45:56.000000 instruct-qa-0.0.2/instruct_qa/collections/hotpot_wiki_collection.py
--rw-r--r--   0 runner    (1001) docker     (127)     2746 2023-09-19 19:45:56.000000 instruct-qa-0.0.2/instruct_qa/collections/topiocqa_wiki_collection.py
--rw-r--r--   0 runner    (1001) docker     (127)     1244 2023-09-19 19:45:56.000000 instruct-qa-0.0.2/instruct_qa/collections/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-09-19 19:46:09.834400 instruct-qa-0.0.2/instruct_qa/dataset/
--rw-r--r--   0 runner    (1001) docker     (127)      152 2023-09-19 19:45:56.000000 instruct-qa-0.0.2/instruct_qa/dataset/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-09-19 19:46:09.834400 instruct-qa-0.0.2/instruct_qa/dataset/convqa/
--rw-r--r--   0 runner    (1001) docker     (127)       78 2023-09-19 19:45:56.000000 instruct-qa-0.0.2/instruct_qa/dataset/convqa/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1726 2023-09-19 19:45:56.000000 instruct-qa-0.0.2/instruct_qa/dataset/convqa/faithdial.py
--rw-r--r--   0 runner    (1001) docker     (127)     2680 2023-09-19 19:45:56.000000 instruct-qa-0.0.2/instruct_qa/dataset/convqa/topiocqa.py
--rw-r--r--   0 runner    (1001) docker     (127)      562 2023-09-19 19:45:56.000000 instruct-qa-0.0.2/instruct_qa/dataset/dataset.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-09-19 19:46:09.834400 instruct-qa-0.0.2/instruct_qa/dataset/qa/
--rw-r--r--   0 runner    (1001) docker     (127)      134 2023-09-19 19:45:56.000000 instruct-qa-0.0.2/instruct_qa/dataset/qa/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      982 2023-09-19 19:45:56.000000 instruct-qa-0.0.2/instruct_qa/dataset/qa/generic_qa.py
--rw-r--r--   0 runner    (1001) docker     (127)     1346 2023-09-19 19:45:56.000000 instruct-qa-0.0.2/instruct_qa/dataset/qa/hotpot_qa.py
--rw-r--r--   0 runner    (1001) docker     (127)     1391 2023-09-19 19:45:56.000000 instruct-qa-0.0.2/instruct_qa/dataset/qa/natural_questions.py
--rw-r--r--   0 runner    (1001) docker     (127)      971 2023-09-19 19:45:56.000000 instruct-qa-0.0.2/instruct_qa/dataset/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-09-19 19:46:09.834400 instruct-qa-0.0.2/instruct_qa/evaluation/
--rw-r--r--   0 runner    (1001) docker     (127)     1396 2023-09-19 19:45:56.000000 instruct-qa-0.0.2/instruct_qa/evaluation/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    36883 2023-09-19 19:45:56.000000 instruct-qa-0.0.2/instruct_qa/evaluation/faithfulness_metrics.py
--rw-r--r--   0 runner    (1001) docker     (127)    24453 2023-09-19 19:45:56.000000 instruct-qa-0.0.2/instruct_qa/evaluation/metrics.py
--rw-r--r--   0 runner    (1001) docker     (127)     1475 2023-09-19 19:45:56.000000 instruct-qa-0.0.2/instruct_qa/evaluation/utils.py
--rw-r--r--   0 runner    (1001) docker     (127)     4898 2023-09-19 19:45:56.000000 instruct-qa-0.0.2/instruct_qa/experiment_utils.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-09-19 19:46:09.834400 instruct-qa-0.0.2/instruct_qa/generation/
--rw-r--r--   0 runner    (1001) docker     (127)      139 2023-09-19 19:45:56.000000 instruct-qa-0.0.2/instruct_qa/generation/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    13036 2023-09-19 19:45:56.000000 instruct-qa-0.0.2/instruct_qa/generation/generator.py
--rw-r--r--   0 runner    (1001) docker     (127)     1128 2023-09-19 19:45:56.000000 instruct-qa-0.0.2/instruct_qa/generation/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-09-19 19:46:09.834400 instruct-qa-0.0.2/instruct_qa/prompt/
--rw-r--r--   0 runner    (1001) docker     (127)      279 2023-09-19 19:45:56.000000 instruct-qa-0.0.2/instruct_qa/prompt/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     7875 2023-09-19 19:45:56.000000 instruct-qa-0.0.2/instruct_qa/prompt/templates.py
--rw-r--r--   0 runner    (1001) docker     (127)     1131 2023-09-19 19:45:56.000000 instruct-qa-0.0.2/instruct_qa/prompt/utils.py
--rw-r--r--   0 runner    (1001) docker     (127)     5405 2023-09-19 19:45:56.000000 instruct-qa-0.0.2/instruct_qa/response_runner.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-09-19 19:46:09.838400 instruct-qa-0.0.2/instruct_qa/retrieval/
--rw-r--r--   0 runner    (1001) docker     (127)     6821 2023-09-19 19:45:56.000000 instruct-qa-0.0.2/instruct_qa/retrieval/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    15445 2023-09-19 19:45:56.000000 instruct-qa-0.0.2/instruct_qa/retrieval/index.py
--rw-r--r--   0 runner    (1001) docker     (127)     7320 2023-09-19 19:45:56.000000 instruct-qa-0.0.2/instruct_qa/retrieval/pyserini_utils.py
--rw-r--r--   0 runner    (1001) docker     (127)     8462 2023-09-19 19:45:56.000000 instruct-qa-0.0.2/instruct_qa/retrieval/utils.py
--rw-r--r--   0 runner    (1001) docker     (127)       22 2023-09-19 19:45:56.000000 instruct-qa-0.0.2/instruct_qa/version.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-09-19 19:46:09.830400 instruct-qa-0.0.2/instruct_qa.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     8403 2023-09-19 19:46:09.000000 instruct-qa-0.0.2/instruct_qa.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     1450 2023-09-19 19:46:09.000000 instruct-qa-0.0.2/instruct_qa.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2023-09-19 19:46:09.000000 instruct-qa-0.0.2/instruct_qa.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2023-09-19 19:46:09.000000 instruct-qa-0.0.2/instruct_qa.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (127)      231 2023-09-19 19:46:09.000000 instruct-qa-0.0.2/instruct_qa.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       12 2023-09-19 19:46:09.000000 instruct-qa-0.0.2/instruct_qa.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)       38 2023-09-19 19:46:09.838400 instruct-qa-0.0.2/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)     1363 2023-09-19 19:45:56.000000 instruct-qa-0.0.2/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-29 03:10:01.594276 instruct-qa-0.0.3rc1/
+-rw-r--r--   0 runner    (1001) docker     (127)    11356 2024-05-29 03:09:53.000000 instruct-qa-0.0.3rc1/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)    10358 2024-05-29 03:10:01.594276 instruct-qa-0.0.3rc1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     8184 2024-05-29 03:09:53.000000 instruct-qa-0.0.3rc1/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-29 03:10:01.590275 instruct-qa-0.0.3rc1/instruct_qa/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-29 03:09:53.000000 instruct-qa-0.0.3rc1/instruct_qa/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-29 03:10:01.590275 instruct-qa-0.0.3rc1/instruct_qa/collections/
+-rw-r--r--   0 runner    (1001) docker     (127)      843 2024-05-29 03:09:53.000000 instruct-qa-0.0.3rc1/instruct_qa/collections/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2620 2024-05-29 03:09:53.000000 instruct-qa-0.0.3rc1/instruct_qa/collections/dpr_wiki_collection.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1229 2024-05-29 03:09:53.000000 instruct-qa-0.0.3rc1/instruct_qa/collections/faithdial_collection.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1789 2024-05-29 03:09:53.000000 instruct-qa-0.0.3rc1/instruct_qa/collections/hotpot_wiki_collection.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2747 2024-05-29 03:09:53.000000 instruct-qa-0.0.3rc1/instruct_qa/collections/topiocqa_wiki_collection.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1244 2024-05-29 03:09:53.000000 instruct-qa-0.0.3rc1/instruct_qa/collections/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-29 03:10:01.590275 instruct-qa-0.0.3rc1/instruct_qa/dataset/
+-rw-r--r--   0 runner    (1001) docker     (127)      152 2024-05-29 03:09:53.000000 instruct-qa-0.0.3rc1/instruct_qa/dataset/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-29 03:10:01.594276 instruct-qa-0.0.3rc1/instruct_qa/dataset/convqa/
+-rw-r--r--   0 runner    (1001) docker     (127)       78 2024-05-29 03:09:53.000000 instruct-qa-0.0.3rc1/instruct_qa/dataset/convqa/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1726 2024-05-29 03:09:53.000000 instruct-qa-0.0.3rc1/instruct_qa/dataset/convqa/faithdial.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2680 2024-05-29 03:09:53.000000 instruct-qa-0.0.3rc1/instruct_qa/dataset/convqa/topiocqa.py
+-rw-r--r--   0 runner    (1001) docker     (127)      562 2024-05-29 03:09:53.000000 instruct-qa-0.0.3rc1/instruct_qa/dataset/dataset.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-29 03:10:01.594276 instruct-qa-0.0.3rc1/instruct_qa/dataset/qa/
+-rw-r--r--   0 runner    (1001) docker     (127)      134 2024-05-29 03:09:53.000000 instruct-qa-0.0.3rc1/instruct_qa/dataset/qa/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      982 2024-05-29 03:09:53.000000 instruct-qa-0.0.3rc1/instruct_qa/dataset/qa/generic_qa.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1346 2024-05-29 03:09:53.000000 instruct-qa-0.0.3rc1/instruct_qa/dataset/qa/hotpot_qa.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1391 2024-05-29 03:09:53.000000 instruct-qa-0.0.3rc1/instruct_qa/dataset/qa/natural_questions.py
+-rw-r--r--   0 runner    (1001) docker     (127)      971 2024-05-29 03:09:53.000000 instruct-qa-0.0.3rc1/instruct_qa/dataset/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-29 03:10:01.594276 instruct-qa-0.0.3rc1/instruct_qa/evaluation/
+-rw-r--r--   0 runner    (1001) docker     (127)     1396 2024-05-29 03:09:53.000000 instruct-qa-0.0.3rc1/instruct_qa/evaluation/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    36811 2024-05-29 03:09:53.000000 instruct-qa-0.0.3rc1/instruct_qa/evaluation/faithfulness_metrics.py
+-rw-r--r--   0 runner    (1001) docker     (127)    24381 2024-05-29 03:09:53.000000 instruct-qa-0.0.3rc1/instruct_qa/evaluation/metrics.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1475 2024-05-29 03:09:53.000000 instruct-qa-0.0.3rc1/instruct_qa/evaluation/utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4898 2024-05-29 03:09:53.000000 instruct-qa-0.0.3rc1/instruct_qa/experiment_utils.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-29 03:10:01.594276 instruct-qa-0.0.3rc1/instruct_qa/generation/
+-rw-r--r--   0 runner    (1001) docker     (127)      139 2024-05-29 03:09:53.000000 instruct-qa-0.0.3rc1/instruct_qa/generation/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    14023 2024-05-29 03:09:53.000000 instruct-qa-0.0.3rc1/instruct_qa/generation/generator.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1128 2024-05-29 03:09:53.000000 instruct-qa-0.0.3rc1/instruct_qa/generation/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-29 03:10:01.594276 instruct-qa-0.0.3rc1/instruct_qa/prompt/
+-rw-r--r--   0 runner    (1001) docker     (127)      279 2024-05-29 03:09:53.000000 instruct-qa-0.0.3rc1/instruct_qa/prompt/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7875 2024-05-29 03:09:53.000000 instruct-qa-0.0.3rc1/instruct_qa/prompt/templates.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1131 2024-05-29 03:09:53.000000 instruct-qa-0.0.3rc1/instruct_qa/prompt/utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5376 2024-05-29 03:09:53.000000 instruct-qa-0.0.3rc1/instruct_qa/response_runner.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-29 03:10:01.594276 instruct-qa-0.0.3rc1/instruct_qa/retrieval/
+-rw-r--r--   0 runner    (1001) docker     (127)     6821 2024-05-29 03:09:53.000000 instruct-qa-0.0.3rc1/instruct_qa/retrieval/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    15445 2024-05-29 03:09:53.000000 instruct-qa-0.0.3rc1/instruct_qa/retrieval/index.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7320 2024-05-29 03:09:53.000000 instruct-qa-0.0.3rc1/instruct_qa/retrieval/pyserini_utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8462 2024-05-29 03:09:53.000000 instruct-qa-0.0.3rc1/instruct_qa/retrieval/utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)       25 2024-05-29 03:09:53.000000 instruct-qa-0.0.3rc1/instruct_qa/version.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-29 03:10:01.590275 instruct-qa-0.0.3rc1/instruct_qa.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)    10358 2024-05-29 03:10:01.000000 instruct-qa-0.0.3rc1/instruct_qa.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     1450 2024-05-29 03:10:01.000000 instruct-qa-0.0.3rc1/instruct_qa.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-29 03:10:01.000000 instruct-qa-0.0.3rc1/instruct_qa.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-29 03:10:01.000000 instruct-qa-0.0.3rc1/instruct_qa.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (127)      355 2024-05-29 03:10:01.000000 instruct-qa-0.0.3rc1/instruct_qa.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       12 2024-05-29 03:10:01.000000 instruct-qa-0.0.3rc1/instruct_qa.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-29 03:10:01.594276 instruct-qa-0.0.3rc1/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)     1479 2024-05-29 03:09:53.000000 instruct-qa-0.0.3rc1/setup.py
```

### Comparing `instruct-qa-0.0.2/LICENSE` & `instruct-qa-0.0.3rc1/LICENSE`

 * *Files identical despite different names*

### Comparing `instruct-qa-0.0.2/PKG-INFO` & `instruct-qa-0.0.3rc1/PKG-INFO`

 * *Files 16% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: instruct-qa
-Version: 0.0.2
+Version: 0.0.3rc1
 Summary: Empirical evaluation of retrieval-augmented instruction-following models.
 Home-page: https://github.com/McGill-NLP/instruct-qa
 Author: McGill NLP
 License: UNKNOWN
 Description: # Evaluating Correctness and Faithfulness of Instruction-Following Models for Question Answering
         
         [![arXiv](https://img.shields.io/badge/arXiv-2307.16877-b31b1b.svg)](https://arxiv.org/abs/2307.16877)
@@ -112,15 +112,17 @@
         --prompt_type qa \
         --dataset_name natural_questions \
         --document_collection_name dpr_wiki_collection \
         --index_name dpr-nq-multi-hnsw \
         --retriever_name facebook-dpr-question_encoder-multiset-base \
         --batch_size 1 \
         --model_name flan-t5-xxl \
-        --k 8
+        --k 8 \
+        --max_new_tokens 500 \
+        --post_process_response
         ```
         
         By default, a `results` directory is created within the repository that stores the model responses. The default directory location can be overidden by providing an additional command line argument `--persistent_dir <OUTPUT_DIR>` More examples are present in the [examples](examples) directory.
         
         ## Download model responses and human evaluation data
         We release the model responses generated using the above commands for all three datasets. The scores reported in the paper are based on these responses. The responses can be downloaded with the following command:
         ```bash
@@ -158,14 +160,43 @@
         │   │   ├── {model}_human_eval_results.json
         ```
         
         ## Evaluating model responses (Coming soon!)
         
         Documentation to evaluate model responses and add your own evaluation criterion coming soon! Stay tuned!
         
+        ## LLM-based evaluation
+        The following prompt templates and instructions were used for LLM-based evaluation.
+        
+        ### Correctness
+        ```
+        System prompt: You are CompareGPT, a machine to verify the correctness of predictions. Answer with only yes/no.
+        
+        You are given a question, the corresponding ground-truth answer and a prediction from a model. Compare the "Ground-truth answer" and the "Prediction" to determine whether the prediction correctly answers the question. All information in the ground-truth answer must be present in the prediction, including numbers and dates. You must answer "no" if there are any specific details in the ground-truth answer that are not mentioned in the prediction. There should be no contradicting statements in the prediction. The prediction may contain extra information. If the prediction states something as a possibility, treat it as a definitive answer.
+        
+        Question: {Question}
+        Ground-truth answer: {Reference answer}
+        Prediction:  {{Model response}
+        
+        CompareGPT response:
+        ```
+        
+        ### Faithfulness
+        ```
+        System prompt: You are CompareGPT, a machine to verify the groundedness of predictions. Answer with only yes/no.
+        
+        You are given a question, the corresponding evidence and a prediction from a model. Compare the "Prediction" and the "Evidence" to determine whether all the information of the prediction in present in the evidence or can be inferred from the evidence. You must answer "no" if there are any specific details in the prediction that are not mentioned in the evidence or cannot be inferred from the evidence.
+        
+        Question: {Question}
+        Prediction:  {Model response}
+        Evidence: {Reference passage}
+        
+        CompareGPT response:
+        ```
+        
         ## License
         
         This work is licensed under the Apache 2 license. See [LICENSE](LICENSE) for details.
         
         ## Citation
```

### Comparing `instruct-qa-0.0.2/README.md` & `instruct-qa-0.0.3rc1/README.md`

 * *Files 19% similar despite different names*

```diff
@@ -105,15 +105,17 @@
 --prompt_type qa \
 --dataset_name natural_questions \
 --document_collection_name dpr_wiki_collection \
 --index_name dpr-nq-multi-hnsw \
 --retriever_name facebook-dpr-question_encoder-multiset-base \
 --batch_size 1 \
 --model_name flan-t5-xxl \
---k 8
+--k 8 \
+--max_new_tokens 500 \
+--post_process_response
 ```
 
 By default, a `results` directory is created within the repository that stores the model responses. The default directory location can be overidden by providing an additional command line argument `--persistent_dir <OUTPUT_DIR>` More examples are present in the [examples](examples) directory.
 
 ## Download model responses and human evaluation data
 We release the model responses generated using the above commands for all three datasets. The scores reported in the paper are based on these responses. The responses can be downloaded with the following command:
 ```bash
@@ -151,14 +153,43 @@
 │   │   ├── {model}_human_eval_results.json
 ```
 
 ## Evaluating model responses (Coming soon!)
 
 Documentation to evaluate model responses and add your own evaluation criterion coming soon! Stay tuned!
 
+## LLM-based evaluation
+The following prompt templates and instructions were used for LLM-based evaluation.
+
+### Correctness
+```
+System prompt: You are CompareGPT, a machine to verify the correctness of predictions. Answer with only yes/no.
+
+You are given a question, the corresponding ground-truth answer and a prediction from a model. Compare the "Ground-truth answer" and the "Prediction" to determine whether the prediction correctly answers the question. All information in the ground-truth answer must be present in the prediction, including numbers and dates. You must answer "no" if there are any specific details in the ground-truth answer that are not mentioned in the prediction. There should be no contradicting statements in the prediction. The prediction may contain extra information. If the prediction states something as a possibility, treat it as a definitive answer.
+
+Question: {Question}
+Ground-truth answer: {Reference answer}
+Prediction:  {{Model response}
+
+CompareGPT response:
+```
+
+### Faithfulness
+```
+System prompt: You are CompareGPT, a machine to verify the groundedness of predictions. Answer with only yes/no.
+
+You are given a question, the corresponding evidence and a prediction from a model. Compare the "Prediction" and the "Evidence" to determine whether all the information of the prediction in present in the evidence or can be inferred from the evidence. You must answer "no" if there are any specific details in the prediction that are not mentioned in the evidence or cannot be inferred from the evidence.
+
+Question: {Question}
+Prediction:  {Model response}
+Evidence: {Reference passage}
+
+CompareGPT response:
+```
+
 ## License
 
 This work is licensed under the Apache 2 license. See [LICENSE](LICENSE) for details.
 
 ## Citation
```

### Comparing `instruct-qa-0.0.2/instruct_qa/collections/__init__.py` & `instruct-qa-0.0.3rc1/instruct_qa/collections/__init__.py`

 * *Files identical despite different names*

### Comparing `instruct-qa-0.0.2/instruct_qa/collections/dpr_wiki_collection.py` & `instruct-qa-0.0.3rc1/instruct_qa/collections/dpr_wiki_collection.py`

 * *Files identical despite different names*

### Comparing `instruct-qa-0.0.2/instruct_qa/collections/faithdial_collection.py` & `instruct-qa-0.0.3rc1/instruct_qa/collections/faithdial_collection.py`

 * *Files identical despite different names*

### Comparing `instruct-qa-0.0.2/instruct_qa/collections/hotpot_wiki_collection.py` & `instruct-qa-0.0.3rc1/instruct_qa/collections/hotpot_wiki_collection.py`

 * *Files identical despite different names*

### Comparing `instruct-qa-0.0.2/instruct_qa/collections/topiocqa_wiki_collection.py` & `instruct-qa-0.0.3rc1/instruct_qa/collections/topiocqa_wiki_collection.py`

 * *Files 0% similar despite different names*

```diff
@@ -5,15 +5,15 @@
 import requests
 from tqdm import tqdm
 
 import instruct_qa.experiment_utils as utils
 
 from . import PassageCollection
 
-TOPIOCQA_WIKI_DOWNLOAD_URL = "https://zenodo.org/record/6149599/files/data/wikipedia_split/full_wiki_segments.tsv"
+TOPIOCQA_WIKI_DOWNLOAD_URL = "https://zenodo.org/records/6149599/files/data/wikipedia_split/full_wiki_segments.tsv"
 
 
 class TopiocqaWikiCollection(PassageCollection):
     def __init__(
         self,
         name: str = "topiocqa_wiki",
         file_name: str = "full_wiki_segments.tsv",
```

### Comparing `instruct-qa-0.0.2/instruct_qa/collections/utils.py` & `instruct-qa-0.0.3rc1/instruct_qa/collections/utils.py`

 * *Files identical despite different names*

### Comparing `instruct-qa-0.0.2/instruct_qa/dataset/convqa/faithdial.py` & `instruct-qa-0.0.3rc1/instruct_qa/dataset/convqa/faithdial.py`

 * *Files identical despite different names*

### Comparing `instruct-qa-0.0.2/instruct_qa/dataset/convqa/topiocqa.py` & `instruct-qa-0.0.3rc1/instruct_qa/dataset/convqa/topiocqa.py`

 * *Files identical despite different names*

### Comparing `instruct-qa-0.0.2/instruct_qa/dataset/dataset.py` & `instruct-qa-0.0.3rc1/instruct_qa/dataset/dataset.py`

 * *Files identical despite different names*

### Comparing `instruct-qa-0.0.2/instruct_qa/dataset/qa/generic_qa.py` & `instruct-qa-0.0.3rc1/instruct_qa/dataset/qa/generic_qa.py`

 * *Files identical despite different names*

### Comparing `instruct-qa-0.0.2/instruct_qa/dataset/qa/hotpot_qa.py` & `instruct-qa-0.0.3rc1/instruct_qa/dataset/qa/hotpot_qa.py`

 * *Files identical despite different names*

### Comparing `instruct-qa-0.0.2/instruct_qa/dataset/qa/natural_questions.py` & `instruct-qa-0.0.3rc1/instruct_qa/dataset/qa/natural_questions.py`

 * *Files identical despite different names*

### Comparing `instruct-qa-0.0.2/instruct_qa/dataset/utils.py` & `instruct-qa-0.0.3rc1/instruct_qa/dataset/utils.py`

 * *Files identical despite different names*

### Comparing `instruct-qa-0.0.2/instruct_qa/evaluation/__init__.py` & `instruct-qa-0.0.3rc1/instruct_qa/evaluation/__init__.py`

 * *Files identical despite different names*

### Comparing `instruct-qa-0.0.2/instruct_qa/evaluation/faithfulness_metrics.py` & `instruct-qa-0.0.3rc1/instruct_qa/evaluation/faithfulness_metrics.py`

 * *Files 0% similar despite different names*

```diff
@@ -2,18 +2,17 @@
 import json
 import os
 import re
 import string
 import time
 import evaluate
 import openai
-from openai.error import (
+from openai import (
     RateLimitError,
     APIConnectionError,
-    ServiceUnavailableError,
     APIError,
 )
 
 from tqdm import tqdm
 from instruct_qa.evaluation import Metric
 from instruct_qa.evaluation.metrics import BERTScore, F1
 import torch
@@ -887,15 +886,14 @@
                 presence_penalty=self.presence_penalty,
                 frequency_penalty=self.frequency_penalty,
             )
         # Except multiple errors in one except block
         except (
             RateLimitError,
             APIConnectionError,
-            ServiceUnavailableError,
             APIError,
         ) as e:
             print(f"Error: {e}. Waiting {self.wait} seconds before retrying.")
             time.sleep(self.wait)
             return self._llm_score(history, response, evidence, id_)
 
         response = (
```

### Comparing `instruct-qa-0.0.2/instruct_qa/evaluation/metrics.py` & `instruct-qa-0.0.3rc1/instruct_qa/evaluation/metrics.py`

 * *Files 1% similar despite different names*

```diff
@@ -4,18 +4,17 @@
 import string
 from collections import Counter
 import time
 
 import evaluate
 import numpy as np
 import openai
-from openai.error import (
+from openai import (
     RateLimitError,
     APIConnectionError,
-    ServiceUnavailableError,
     APIError,
 )
 import torch
 from tqdm import tqdm
 
 from transformers import (
     AutoModelForSequenceClassification,
@@ -528,15 +527,14 @@
                 presence_penalty=self.presence_penalty,
                 frequency_penalty=self.frequency_penalty,
             )
         # Except multiple errors in one except block
         except (
             RateLimitError,
             APIConnectionError,
-            ServiceUnavailableError,
             APIError,
         ) as e:
             print(f"Error: {e}. Waiting {self.wait} seconds before retrying.")
             time.sleep(self.wait)
             return self._llm_score_single(prediction, reference, question)
 
         response = response["choices"][0]["message"]["content"].strip().strip('.').strip(',')
```

### Comparing `instruct-qa-0.0.2/instruct_qa/evaluation/utils.py` & `instruct-qa-0.0.3rc1/instruct_qa/evaluation/utils.py`

 * *Files identical despite different names*

### Comparing `instruct-qa-0.0.2/instruct_qa/experiment_utils.py` & `instruct-qa-0.0.3rc1/instruct_qa/experiment_utils.py`

 * *Files identical despite different names*

### Comparing `instruct-qa-0.0.2/instruct_qa/generation/generator.py` & `instruct-qa-0.0.3rc1/instruct_qa/generation/generator.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,28 +1,31 @@
 from math import inf
 import time
 import openai
-from openai.error import (
+from openai import (
     RateLimitError,
     APIConnectionError,
-    ServiceUnavailableError,
     APIError,
     Timeout,
 )
 import torch
 from transformers import pipeline
 from transformers import (
     AutoTokenizer,
     AutoModelForCausalLM,
     AutoModelForSeq2SeqLM,
     OPTForCausalLM,
 )
 
 max_length = 1900
 
+import logging
+logger = logging.getLogger(__name__)
+logging.basicConfig(level=logging.INFO)
+
 
 class BaseGenerator:
     def __init__(
         self,
         model_name=None,
         weights_path=None,
         api_key=None,
@@ -49,14 +52,17 @@
         self.clean_up_tokenization_spaces = clean_up_tokenization_spaces
         self.device = device
         self.wait = 10
 
     def __call__(self, prompt, **kwargs):
         raise NotImplementedError()
 
+    def post_process_response(self, response):
+        return response
+
 
 class GPTx(BaseGenerator):
     def __init__(self, *args, **kwargs):
         super().__init__(*args, **kwargs)
         openai.api_key = self.api_key
         self.model_map = {
             "gpt-3.5-turbo": "chat",
@@ -105,15 +111,14 @@
                 res = openai.Completion.create(
                     model=self.model_name, prompt=prompt, **kwargs
                 )
                 return [r.text for r in res.choices]
         except (
             RateLimitError,
             APIConnectionError,
-            ServiceUnavailableError,
             APIError,
             Timeout,
         ) as e:
             print(f"Error: {e}. Waiting {self.wait} seconds before retrying.")
             time.sleep(self.wait)
             return self.api_request(prompt, **kwargs)
 
@@ -163,14 +168,33 @@
                 generate_ids[i, _input.input_ids.size(1) :],
                 skip_special_tokens=self.skip_special_tokens,
                 clean_up_tokenization_spaces=self.clean_up_tokenization_spaces,
             )
             for i in range(generate_ids.size(0))
         ]
 
+    def post_process_response(self, response):
+        keywords = {"user:", "User:", "assistant:", "- Title:", "Question:"}
+        end_keywords = {"Agent:", "Answer:"}
+
+        response_lines = response.split("\n")
+        response_lines = [x for x in response_lines if x.strip() not in ["", " "]]
+
+        for j, line in enumerate(response_lines):
+            if any(line.startswith(kw) for kw in keywords):
+                response_lines = response_lines[:j]
+                break
+
+        for j, line in enumerate(response_lines):
+            if j > 0 and any(line.startswith(kw) for kw in end_keywords):
+                response_lines = response_lines[:j]
+                break
+
+        return "\n".join(response_lines)
+
 
 class Vicuna(BaseGenerator):
     def __init__(self, *args, **kwargs):
         super().__init__(*args, **kwargs)
         self.tokenizer = AutoTokenizer.from_pretrained(
             f"lmsys/{self.model_name}", cache_dir=self.cache_dir, padding_side="left"
         )
@@ -258,29 +282,33 @@
         )
         self.model = AutoModelForSeq2SeqLM.from_pretrained(
             f"google/{self.model_name}",
             cache_dir=self.cache_dir,
             torch_dtype=self.torch_dtype,
             device_map="auto",
         )
+        if self.min_new_tokens is not None:
+            logger.warning(
+                "min_new_tokens is not supported for Flan. It will be ignored."
+            )
 
     def __call__(self, prompts):
         _input = self.tokenizer(
             prompts,
             return_tensors="pt",
             padding=True,
             max_length=max_length,
             truncation=True,
         ).to(self.device)
         generate_ids = self.model.generate(
             _input.input_ids,
             temperature=self.temperature,
             top_p=self.top_p,
             max_new_tokens=self.max_new_tokens,
-            min_new_tokens=self.min_new_tokens,
+            # min_new_tokens=self.min_new_tokens,
         )
         return self.tokenizer.batch_decode(
             generate_ids,
             skip_special_tokens=self.skip_special_tokens,
             clean_up_tokenization_spaces=self.clean_up_tokenization_spaces,
         )
```

### Comparing `instruct-qa-0.0.2/instruct_qa/generation/utils.py` & `instruct-qa-0.0.3rc1/instruct_qa/generation/utils.py`

 * *Files identical despite different names*

### Comparing `instruct-qa-0.0.2/instruct_qa/prompt/templates.py` & `instruct-qa-0.0.3rc1/instruct_qa/prompt/templates.py`

 * *Files identical despite different names*

### Comparing `instruct-qa-0.0.2/instruct_qa/prompt/utils.py` & `instruct-qa-0.0.3rc1/instruct_qa/prompt/utils.py`

 * *Files identical despite different names*

### Comparing `instruct-qa-0.0.2/instruct_qa/response_runner.py` & `instruct-qa-0.0.3rc1/instruct_qa/response_runner.py`

 * *Files 8% similar despite different names*

```diff
@@ -45,16 +45,15 @@
         self._use_hosted_retriever = use_hosted_retriever
         self._hosted_retriever_url = hosted_retriever_url
         self._use_cached_retrieved_results = use_cached_retrieved_results
         self._collection_name = document_collection.get_name()
         self._post_process_response = post_process_response
 
     def post_process_response(self, response):
-        response = re.sub(r"^\n+", "", response)
-        return response.split("\n")[0]
+        return self._model.post_process_response(response)
 
     def __call__(self):
         if self._output_path and os.path.exists(self._output_path):
             with open(self._output_path, "r") as f:
                 existing_results = [json.loads(line) for line in f.readlines()]
             num_done = len(existing_results)
             if num_done >= len(self._dataset):
```

### Comparing `instruct-qa-0.0.2/instruct_qa/retrieval/__init__.py` & `instruct-qa-0.0.3rc1/instruct_qa/retrieval/__init__.py`

 * *Files identical despite different names*

### Comparing `instruct-qa-0.0.2/instruct_qa/retrieval/index.py` & `instruct-qa-0.0.3rc1/instruct_qa/retrieval/index.py`

 * *Files identical despite different names*

### Comparing `instruct-qa-0.0.2/instruct_qa/retrieval/pyserini_utils.py` & `instruct-qa-0.0.3rc1/instruct_qa/retrieval/pyserini_utils.py`

 * *Files identical despite different names*

### Comparing `instruct-qa-0.0.2/instruct_qa/retrieval/utils.py` & `instruct-qa-0.0.3rc1/instruct_qa/retrieval/utils.py`

 * *Files identical despite different names*

### Comparing `instruct-qa-0.0.2/instruct_qa.egg-info/PKG-INFO` & `instruct-qa-0.0.3rc1/instruct_qa.egg-info/PKG-INFO`

 * *Files 16% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: instruct-qa
-Version: 0.0.2
+Version: 0.0.3rc1
 Summary: Empirical evaluation of retrieval-augmented instruction-following models.
 Home-page: https://github.com/McGill-NLP/instruct-qa
 Author: McGill NLP
 License: UNKNOWN
 Description: # Evaluating Correctness and Faithfulness of Instruction-Following Models for Question Answering
         
         [![arXiv](https://img.shields.io/badge/arXiv-2307.16877-b31b1b.svg)](https://arxiv.org/abs/2307.16877)
@@ -112,15 +112,17 @@
         --prompt_type qa \
         --dataset_name natural_questions \
         --document_collection_name dpr_wiki_collection \
         --index_name dpr-nq-multi-hnsw \
         --retriever_name facebook-dpr-question_encoder-multiset-base \
         --batch_size 1 \
         --model_name flan-t5-xxl \
-        --k 8
+        --k 8 \
+        --max_new_tokens 500 \
+        --post_process_response
         ```
         
         By default, a `results` directory is created within the repository that stores the model responses. The default directory location can be overidden by providing an additional command line argument `--persistent_dir <OUTPUT_DIR>` More examples are present in the [examples](examples) directory.
         
         ## Download model responses and human evaluation data
         We release the model responses generated using the above commands for all three datasets. The scores reported in the paper are based on these responses. The responses can be downloaded with the following command:
         ```bash
@@ -158,14 +160,43 @@
         │   │   ├── {model}_human_eval_results.json
         ```
         
         ## Evaluating model responses (Coming soon!)
         
         Documentation to evaluate model responses and add your own evaluation criterion coming soon! Stay tuned!
         
+        ## LLM-based evaluation
+        The following prompt templates and instructions were used for LLM-based evaluation.
+        
+        ### Correctness
+        ```
+        System prompt: You are CompareGPT, a machine to verify the correctness of predictions. Answer with only yes/no.
+        
+        You are given a question, the corresponding ground-truth answer and a prediction from a model. Compare the "Ground-truth answer" and the "Prediction" to determine whether the prediction correctly answers the question. All information in the ground-truth answer must be present in the prediction, including numbers and dates. You must answer "no" if there are any specific details in the ground-truth answer that are not mentioned in the prediction. There should be no contradicting statements in the prediction. The prediction may contain extra information. If the prediction states something as a possibility, treat it as a definitive answer.
+        
+        Question: {Question}
+        Ground-truth answer: {Reference answer}
+        Prediction:  {{Model response}
+        
+        CompareGPT response:
+        ```
+        
+        ### Faithfulness
+        ```
+        System prompt: You are CompareGPT, a machine to verify the groundedness of predictions. Answer with only yes/no.
+        
+        You are given a question, the corresponding evidence and a prediction from a model. Compare the "Prediction" and the "Evidence" to determine whether all the information of the prediction in present in the evidence or can be inferred from the evidence. You must answer "no" if there are any specific details in the prediction that are not mentioned in the evidence or cannot be inferred from the evidence.
+        
+        Question: {Question}
+        Prediction:  {Model response}
+        Evidence: {Reference passage}
+        
+        CompareGPT response:
+        ```
+        
         ## License
         
         This work is licensed under the Apache 2 license. See [LICENSE](LICENSE) for details.
         
         ## Citation
```

### Comparing `instruct-qa-0.0.2/instruct_qa.egg-info/SOURCES.txt` & `instruct-qa-0.0.3rc1/instruct_qa.egg-info/SOURCES.txt`

 * *Files identical despite different names*

