# Comparing `tmp/dkist-processing-core-3.1.0rc2.tar.gz` & `tmp/dkist-processing-core-3.2.0rc1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dkist-processing-core-3.1.0rc2.tar", last modified: Tue Mar 12 21:18:01 2024, max compression
+gzip compressed data, was "dkist-processing-core-3.2.0rc1.tar", last modified: Wed May 29 15:51:01 2024, max compression
```

## Comparing `dkist-processing-core-3.1.0rc2.tar` & `dkist-processing-core-3.2.0rc1.tar`

### file list

```diff
@@ -1,60 +1,62 @@
-drwxrwxrwx   0 root         (0) root         (0)        0 2024-03-12 21:18:01.065446 dkist-processing-core-3.1.0rc2/
--rw-rw-rw-   0 root         (0) root         (0)     2448 2024-03-12 21:17:55.000000 dkist-processing-core-3.1.0rc2/.gitignore
--rw-rw-rw-   0 root         (0) root         (0)      811 2024-03-12 21:17:55.000000 dkist-processing-core-3.1.0rc2/.pre-commit-config.yaml
--rw-rw-rw-   0 root         (0) root         (0)      306 2024-03-12 21:17:55.000000 dkist-processing-core-3.1.0rc2/.readthedocs.yml
--rw-rw-rw-   0 root         (0) root         (0)     5409 2024-03-12 21:17:55.000000 dkist-processing-core-3.1.0rc2/CHANGELOG.rst
--rw-rw-rw-   0 root         (0) root         (0)     7965 2024-03-12 21:18:01.065446 dkist-processing-core-3.1.0rc2/PKG-INFO
--rw-rw-rw-   0 root         (0) root         (0)     7351 2024-03-12 21:17:55.000000 dkist-processing-core-3.1.0rc2/README.rst
--rw-rw-rw-   0 root         (0) root         (0)     2816 2024-03-12 21:17:55.000000 dkist-processing-core-3.1.0rc2/bitbucket-pipelines.yml
-drwxrwxrwx   0 root         (0) root         (0)        0 2024-03-12 21:18:01.061446 dkist-processing-core-3.1.0rc2/changelog/
--rw-rw-rw-   0 root         (0) root         (0)        0 2024-03-12 21:17:55.000000 dkist-processing-core-3.1.0rc2/changelog/.gitempty
--rw-rw-rw-   0 root         (0) root         (0)      105 2024-03-12 21:17:55.000000 dkist-processing-core-3.1.0rc2/changelog/32.feature.rst
--rwxrwxrwx   0 root         (0) root         (0)      436 2024-03-12 21:17:55.000000 dkist-processing-core-3.1.0rc2/check_changelog_updated.sh
-drwxrwxrwx   0 root         (0) root         (0)        0 2024-03-12 21:18:01.061446 dkist-processing-core-3.1.0rc2/dkist_processing_core/
--rw-rw-rw-   0 root         (0) root         (0)      440 2024-03-12 21:17:55.000000 dkist-processing-core-3.1.0rc2/dkist_processing_core/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     3272 2024-03-12 21:17:55.000000 dkist-processing-core-3.1.0rc2/dkist_processing_core/_failure_callback.py
--rw-rw-rw-   0 root         (0) root         (0)     5525 2024-03-12 21:17:55.000000 dkist-processing-core-3.1.0rc2/dkist_processing_core/_node.py
--rw-rw-rw-   0 root         (0) root         (0)     6096 2024-03-12 21:17:55.000000 dkist-processing-core-3.1.0rc2/dkist_processing_core/build_utils.py
--rw-rw-rw-   0 root         (0) root         (0)      256 2024-03-12 21:17:55.000000 dkist-processing-core-3.1.0rc2/dkist_processing_core/resource_queue.py
--rw-rw-rw-   0 root         (0) root         (0)    10316 2024-03-12 21:17:55.000000 dkist-processing-core-3.1.0rc2/dkist_processing_core/task.py
-drwxrwxrwx   0 root         (0) root         (0)        0 2024-03-12 21:18:01.065446 dkist-processing-core-3.1.0rc2/dkist_processing_core/tests/
--rw-rw-rw-   0 root         (0) root         (0)       12 2024-03-12 21:17:55.000000 dkist-processing-core-3.1.0rc2/dkist_processing_core/tests/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     4533 2024-03-12 21:17:55.000000 dkist-processing-core-3.1.0rc2/dkist_processing_core/tests/conftest.py
-drwxrwxrwx   0 root         (0) root         (0)        0 2024-03-12 21:18:01.065446 dkist-processing-core-3.1.0rc2/dkist_processing_core/tests/invalid_workflow_package/
--rw-rw-rw-   0 root         (0) root         (0)       12 2024-03-12 21:17:55.000000 dkist-processing-core-3.1.0rc2/dkist_processing_core/tests/invalid_workflow_package/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)      470 2024-03-12 21:17:55.000000 dkist-processing-core-3.1.0rc2/dkist_processing_core/tests/invalid_workflow_package/workflow.py
--rw-rw-rw-   0 root         (0) root         (0)     1039 2024-03-12 21:17:55.000000 dkist-processing-core-3.1.0rc2/dkist_processing_core/tests/task_example.py
--rw-rw-rw-   0 root         (0) root         (0)     3470 2024-03-12 21:17:55.000000 dkist-processing-core-3.1.0rc2/dkist_processing_core/tests/test_build_utils.py
--rw-rw-rw-   0 root         (0) root         (0)     2563 2024-03-12 21:17:55.000000 dkist-processing-core-3.1.0rc2/dkist_processing_core/tests/test_export.py
--rw-rw-rw-   0 root         (0) root         (0)     4030 2024-03-12 21:17:55.000000 dkist-processing-core-3.1.0rc2/dkist_processing_core/tests/test_failure_callback.py
--rw-rw-rw-   0 root         (0) root         (0)     4525 2024-03-12 21:17:55.000000 dkist-processing-core-3.1.0rc2/dkist_processing_core/tests/test_node.py
--rw-rw-rw-   0 root         (0) root         (0)     2078 2024-03-12 21:17:55.000000 dkist-processing-core-3.1.0rc2/dkist_processing_core/tests/test_task.py
--rw-rw-rw-   0 root         (0) root         (0)     4348 2024-03-12 21:17:55.000000 dkist-processing-core-3.1.0rc2/dkist_processing_core/tests/test_workflow.py
-drwxrwxrwx   0 root         (0) root         (0)        0 2024-03-12 21:18:01.065446 dkist-processing-core-3.1.0rc2/dkist_processing_core/tests/valid_workflow_package/
--rw-rw-rw-   0 root         (0) root         (0)       12 2024-03-12 21:17:55.000000 dkist-processing-core-3.1.0rc2/dkist_processing_core/tests/valid_workflow_package/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)      721 2024-03-12 21:17:55.000000 dkist-processing-core-3.1.0rc2/dkist_processing_core/tests/valid_workflow_package/workflow.py
-drwxrwxrwx   0 root         (0) root         (0)        0 2024-03-12 21:18:01.065446 dkist-processing-core-3.1.0rc2/dkist_processing_core/tests/zero_node_workflow_package/
--rw-rw-rw-   0 root         (0) root         (0)       32 2024-03-12 21:17:55.000000 dkist-processing-core-3.1.0rc2/dkist_processing_core/tests/zero_node_workflow_package/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)      227 2024-03-12 21:17:55.000000 dkist-processing-core-3.1.0rc2/dkist_processing_core/tests/zero_node_workflow_package/workflow.py
--rw-rw-rw-   0 root         (0) root         (0)    10181 2024-03-12 21:17:55.000000 dkist-processing-core-3.1.0rc2/dkist_processing_core/workflow.py
-drwxrwxrwx   0 root         (0) root         (0)        0 2024-03-12 21:18:01.061446 dkist-processing-core-3.1.0rc2/dkist_processing_core.egg-info/
--rw-rw-rw-   0 root         (0) root         (0)     7965 2024-03-12 21:18:01.000000 dkist-processing-core-3.1.0rc2/dkist_processing_core.egg-info/PKG-INFO
--rw-rw-rw-   0 root         (0) root         (0)     1679 2024-03-12 21:18:01.000000 dkist-processing-core-3.1.0rc2/dkist_processing_core.egg-info/SOURCES.txt
--rw-rw-rw-   0 root         (0) root         (0)        1 2024-03-12 21:18:01.000000 dkist-processing-core-3.1.0rc2/dkist_processing_core.egg-info/dependency_links.txt
--rw-rw-rw-   0 root         (0) root         (0)      278 2024-03-12 21:18:01.000000 dkist-processing-core-3.1.0rc2/dkist_processing_core.egg-info/requires.txt
--rw-rw-rw-   0 root         (0) root         (0)       22 2024-03-12 21:18:01.000000 dkist-processing-core-3.1.0rc2/dkist_processing_core.egg-info/top_level.txt
-drwxrwxrwx   0 root         (0) root         (0)        0 2024-03-12 21:18:01.065446 dkist-processing-core-3.1.0rc2/docs/
--rw-rw-rw-   0 root         (0) root         (0)     4598 2024-03-12 21:17:55.000000 dkist-processing-core-3.1.0rc2/docs/Makefile
--rw-rw-rw-   0 root         (0) root         (0)    85295 2024-03-12 21:17:55.000000 dkist-processing-core-3.1.0rc2/docs/auto-proc-concept-model.png
--rw-rw-rw-   0 root         (0) root         (0)    26060 2024-03-12 21:17:55.000000 dkist-processing-core-3.1.0rc2/docs/auto_proc_brick.png
--rw-rw-rw-   0 root         (0) root         (0)   267222 2024-03-12 21:17:55.000000 dkist-processing-core-3.1.0rc2/docs/automated-processing-deployed.png
--rw-rw-rw-   0 root         (0) root         (0)      119 2024-03-12 21:17:55.000000 dkist-processing-core-3.1.0rc2/docs/changelog.rst
--rw-rw-rw-   0 root         (0) root         (0)     1854 2024-03-12 21:17:55.000000 dkist-processing-core-3.1.0rc2/docs/conf.py
--rw-rw-rw-   0 root         (0) root         (0)      103 2024-03-12 21:17:55.000000 dkist-processing-core-3.1.0rc2/docs/index.rst
--rw-rw-rw-   0 root         (0) root         (0)     4513 2024-03-12 21:17:55.000000 dkist-processing-core-3.1.0rc2/docs/make.bat
--rw-rw-rw-   0 root         (0) root         (0)       29 2024-03-12 21:17:55.000000 dkist-processing-core-3.1.0rc2/docs/requirements.txt
-drwxrwxrwx   0 root         (0) root         (0)        0 2024-03-12 21:18:01.065446 dkist-processing-core-3.1.0rc2/licenses/
--rw-rw-rw-   0 root         (0) root         (0)     1462 2024-03-12 21:17:55.000000 dkist-processing-core-3.1.0rc2/licenses/LICENSE.rst
--rw-rw-rw-   0 root         (0) root         (0)      776 2024-03-12 21:17:55.000000 dkist-processing-core-3.1.0rc2/pyproject.toml
--rw-rw-rw-   0 root         (0) root         (0)     1334 2024-03-12 21:18:01.065446 dkist-processing-core-3.1.0rc2/setup.cfg
--rw-rw-rw-   0 root         (0) root         (0)      102 2024-03-12 21:17:55.000000 dkist-processing-core-3.1.0rc2/setup.py
+drwxrwxrwx   0 root         (0) root         (0)        0 2024-05-29 15:51:01.800341 dkist-processing-core-3.2.0rc1/
+-rw-rw-rw-   0 root         (0) root         (0)     2448 2024-05-29 15:50:56.000000 dkist-processing-core-3.2.0rc1/.gitignore
+-rw-rw-rw-   0 root         (0) root         (0)      811 2024-05-29 15:50:56.000000 dkist-processing-core-3.2.0rc1/.pre-commit-config.yaml
+-rw-rw-rw-   0 root         (0) root         (0)      306 2024-05-29 15:50:56.000000 dkist-processing-core-3.2.0rc1/.readthedocs.yml
+-rw-rw-rw-   0 root         (0) root         (0)     5659 2024-05-29 15:50:56.000000 dkist-processing-core-3.2.0rc1/CHANGELOG.rst
+-rw-rw-rw-   0 root         (0) root         (0)     8063 2024-05-29 15:51:01.800341 dkist-processing-core-3.2.0rc1/PKG-INFO
+-rw-rw-rw-   0 root         (0) root         (0)     7449 2024-05-29 15:50:56.000000 dkist-processing-core-3.2.0rc1/README.rst
+-rw-rw-rw-   0 root         (0) root         (0)     2913 2024-05-29 15:50:56.000000 dkist-processing-core-3.2.0rc1/bitbucket-pipelines.yml
+drwxrwxrwx   0 root         (0) root         (0)        0 2024-05-29 15:51:01.796341 dkist-processing-core-3.2.0rc1/changelog/
+-rw-rw-rw-   0 root         (0) root         (0)        0 2024-05-29 15:50:56.000000 dkist-processing-core-3.2.0rc1/changelog/.gitempty
+-rw-rw-rw-   0 root         (0) root         (0)       70 2024-05-29 15:50:56.000000 dkist-processing-core-3.2.0rc1/changelog/33.bugfix.rst
+-rw-rw-rw-   0 root         (0) root         (0)      166 2024-05-29 15:50:56.000000 dkist-processing-core-3.2.0rc1/changelog/34.misc.rst
+-rwxrwxrwx   0 root         (0) root         (0)      436 2024-05-29 15:50:56.000000 dkist-processing-core-3.2.0rc1/check_changelog_updated.sh
+drwxrwxrwx   0 root         (0) root         (0)        0 2024-05-29 15:51:01.796341 dkist-processing-core-3.2.0rc1/dkist_processing_core/
+-rw-rw-rw-   0 root         (0) root         (0)      440 2024-05-29 15:50:56.000000 dkist-processing-core-3.2.0rc1/dkist_processing_core/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     3033 2024-05-29 15:50:56.000000 dkist-processing-core-3.2.0rc1/dkist_processing_core/_config.py
+-rw-rw-rw-   0 root         (0) root         (0)     3311 2024-05-29 15:50:56.000000 dkist-processing-core-3.2.0rc1/dkist_processing_core/_failure_callback.py
+-rw-rw-rw-   0 root         (0) root         (0)     5532 2024-05-29 15:50:56.000000 dkist-processing-core-3.2.0rc1/dkist_processing_core/_node.py
+-rw-rw-rw-   0 root         (0) root         (0)     6096 2024-05-29 15:50:56.000000 dkist-processing-core-3.2.0rc1/dkist_processing_core/build_utils.py
+-rw-rw-rw-   0 root         (0) root         (0)      256 2024-05-29 15:50:56.000000 dkist-processing-core-3.2.0rc1/dkist_processing_core/resource_queue.py
+-rw-rw-rw-   0 root         (0) root         (0)     9294 2024-05-29 15:50:56.000000 dkist-processing-core-3.2.0rc1/dkist_processing_core/task.py
+drwxrwxrwx   0 root         (0) root         (0)        0 2024-05-29 15:51:01.796341 dkist-processing-core-3.2.0rc1/dkist_processing_core/tests/
+-rw-rw-rw-   0 root         (0) root         (0)       12 2024-05-29 15:50:56.000000 dkist-processing-core-3.2.0rc1/dkist_processing_core/tests/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     4505 2024-05-29 15:50:56.000000 dkist-processing-core-3.2.0rc1/dkist_processing_core/tests/conftest.py
+drwxrwxrwx   0 root         (0) root         (0)        0 2024-05-29 15:51:01.800341 dkist-processing-core-3.2.0rc1/dkist_processing_core/tests/invalid_workflow_package/
+-rw-rw-rw-   0 root         (0) root         (0)       12 2024-05-29 15:50:56.000000 dkist-processing-core-3.2.0rc1/dkist_processing_core/tests/invalid_workflow_package/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)      470 2024-05-29 15:50:56.000000 dkist-processing-core-3.2.0rc1/dkist_processing_core/tests/invalid_workflow_package/workflow.py
+-rw-rw-rw-   0 root         (0) root         (0)     1039 2024-05-29 15:50:56.000000 dkist-processing-core-3.2.0rc1/dkist_processing_core/tests/task_example.py
+-rw-rw-rw-   0 root         (0) root         (0)     3490 2024-05-29 15:50:56.000000 dkist-processing-core-3.2.0rc1/dkist_processing_core/tests/test_build_utils.py
+-rw-rw-rw-   0 root         (0) root         (0)     2563 2024-05-29 15:50:56.000000 dkist-processing-core-3.2.0rc1/dkist_processing_core/tests/test_export.py
+-rw-rw-rw-   0 root         (0) root         (0)     3118 2024-05-29 15:50:56.000000 dkist-processing-core-3.2.0rc1/dkist_processing_core/tests/test_failure_callback.py
+-rw-rw-rw-   0 root         (0) root         (0)     4565 2024-05-29 15:50:56.000000 dkist-processing-core-3.2.0rc1/dkist_processing_core/tests/test_node.py
+-rw-rw-rw-   0 root         (0) root         (0)     2487 2024-05-29 15:50:56.000000 dkist-processing-core-3.2.0rc1/dkist_processing_core/tests/test_task.py
+-rw-rw-rw-   0 root         (0) root         (0)     4348 2024-05-29 15:50:56.000000 dkist-processing-core-3.2.0rc1/dkist_processing_core/tests/test_workflow.py
+drwxrwxrwx   0 root         (0) root         (0)        0 2024-05-29 15:51:01.800341 dkist-processing-core-3.2.0rc1/dkist_processing_core/tests/valid_workflow_package/
+-rw-rw-rw-   0 root         (0) root         (0)       12 2024-05-29 15:50:56.000000 dkist-processing-core-3.2.0rc1/dkist_processing_core/tests/valid_workflow_package/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)      721 2024-05-29 15:50:56.000000 dkist-processing-core-3.2.0rc1/dkist_processing_core/tests/valid_workflow_package/workflow.py
+drwxrwxrwx   0 root         (0) root         (0)        0 2024-05-29 15:51:01.800341 dkist-processing-core-3.2.0rc1/dkist_processing_core/tests/zero_node_workflow_package/
+-rw-rw-rw-   0 root         (0) root         (0)       32 2024-05-29 15:50:56.000000 dkist-processing-core-3.2.0rc1/dkist_processing_core/tests/zero_node_workflow_package/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)      227 2024-05-29 15:50:56.000000 dkist-processing-core-3.2.0rc1/dkist_processing_core/tests/zero_node_workflow_package/workflow.py
+-rw-rw-rw-   0 root         (0) root         (0)    10181 2024-05-29 15:50:56.000000 dkist-processing-core-3.2.0rc1/dkist_processing_core/workflow.py
+drwxrwxrwx   0 root         (0) root         (0)        0 2024-05-29 15:51:01.796341 dkist-processing-core-3.2.0rc1/dkist_processing_core.egg-info/
+-rw-rw-rw-   0 root         (0) root         (0)     8063 2024-05-29 15:51:01.000000 dkist-processing-core-3.2.0rc1/dkist_processing_core.egg-info/PKG-INFO
+-rw-rw-rw-   0 root         (0) root         (0)     1733 2024-05-29 15:51:01.000000 dkist-processing-core-3.2.0rc1/dkist_processing_core.egg-info/SOURCES.txt
+-rw-rw-rw-   0 root         (0) root         (0)        1 2024-05-29 15:51:01.000000 dkist-processing-core-3.2.0rc1/dkist_processing_core.egg-info/dependency_links.txt
+-rw-rw-rw-   0 root         (0) root         (0)      348 2024-05-29 15:51:01.000000 dkist-processing-core-3.2.0rc1/dkist_processing_core.egg-info/requires.txt
+-rw-rw-rw-   0 root         (0) root         (0)       22 2024-05-29 15:51:01.000000 dkist-processing-core-3.2.0rc1/dkist_processing_core.egg-info/top_level.txt
+drwxrwxrwx   0 root         (0) root         (0)        0 2024-05-29 15:51:01.800341 dkist-processing-core-3.2.0rc1/docs/
+-rw-rw-rw-   0 root         (0) root         (0)     4598 2024-05-29 15:50:56.000000 dkist-processing-core-3.2.0rc1/docs/Makefile
+-rw-rw-rw-   0 root         (0) root         (0)    85295 2024-05-29 15:50:56.000000 dkist-processing-core-3.2.0rc1/docs/auto-proc-concept-model.png
+-rw-rw-rw-   0 root         (0) root         (0)    26060 2024-05-29 15:50:56.000000 dkist-processing-core-3.2.0rc1/docs/auto_proc_brick.png
+-rw-rw-rw-   0 root         (0) root         (0)   267222 2024-05-29 15:50:56.000000 dkist-processing-core-3.2.0rc1/docs/automated-processing-deployed.png
+-rw-rw-rw-   0 root         (0) root         (0)      119 2024-05-29 15:50:56.000000 dkist-processing-core-3.2.0rc1/docs/changelog.rst
+-rw-rw-rw-   0 root         (0) root         (0)     1854 2024-05-29 15:50:56.000000 dkist-processing-core-3.2.0rc1/docs/conf.py
+-rw-rw-rw-   0 root         (0) root         (0)      103 2024-05-29 15:50:56.000000 dkist-processing-core-3.2.0rc1/docs/index.rst
+-rw-rw-rw-   0 root         (0) root         (0)     4513 2024-05-29 15:50:56.000000 dkist-processing-core-3.2.0rc1/docs/make.bat
+-rw-rw-rw-   0 root         (0) root         (0)       29 2024-05-29 15:50:56.000000 dkist-processing-core-3.2.0rc1/docs/requirements.txt
+drwxrwxrwx   0 root         (0) root         (0)        0 2024-05-29 15:51:01.800341 dkist-processing-core-3.2.0rc1/licenses/
+-rw-rw-rw-   0 root         (0) root         (0)     1462 2024-05-29 15:50:56.000000 dkist-processing-core-3.2.0rc1/licenses/LICENSE.rst
+-rw-rw-rw-   0 root         (0) root         (0)      776 2024-05-29 15:50:56.000000 dkist-processing-core-3.2.0rc1/pyproject.toml
+-rw-rw-rw-   0 root         (0) root         (0)     1549 2024-05-29 15:51:01.800341 dkist-processing-core-3.2.0rc1/setup.cfg
+-rw-rw-rw-   0 root         (0) root         (0)      102 2024-05-29 15:50:56.000000 dkist-processing-core-3.2.0rc1/setup.py
```

### Comparing `dkist-processing-core-3.1.0rc2/.gitignore` & `dkist-processing-core-3.2.0rc1/.gitignore`

 * *Files identical despite different names*

### Comparing `dkist-processing-core-3.1.0rc2/.pre-commit-config.yaml` & `dkist-processing-core-3.2.0rc1/.pre-commit-config.yaml`

 * *Files identical despite different names*

### Comparing `dkist-processing-core-3.1.0rc2/CHANGELOG.rst` & `dkist-processing-core-3.2.0rc1/CHANGELOG.rst`

 * *Files 3% similar despite different names*

```diff
@@ -1,7 +1,16 @@
+v3.1.0 (2024-04-02)
+===================
+
+Features
+--------
+
+- Add a 'rollback' method to the Task API for removing changes to persistent stores performed by the task. (`#32 <https://bitbucket.org/dkistdc/dkist-processing-core/pull-requests/32>`__)
+
+
 v3.0.1 (2023-12-20)
 ===================
 
 Features
 --------
 
 - Remove the build extra because there isn't enough separation of deps yet. (`#29 <https://bitbucket.org/dkistdc/dkist-processing-core/pull-requests/29>`__)
```

### Comparing `dkist-processing-core-3.1.0rc2/PKG-INFO` & `dkist-processing-core-3.2.0rc1/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: dkist-processing-core
-Version: 3.1.0rc2
+Version: 3.2.0rc1
 Summary: Abstraction layer that is used by the DKIST Science Data Processing pipelines to process DKIST data using Apache Airflow.
 Home-page: https://bitbucket.org/dkistdc/dkist-processing-core/src/main/
 Author: NSO / AURA
 Author-email: "dkistdc@nso.edu"
 License: MIT
 Project-URL: Documentation, https://docs.dkist.nso.edu/projects/core
 Classifier: Programming Language :: Python
@@ -119,14 +119,18 @@
      - Message broker user name
      - STR
      -
    * - ISB_PASSWORD
      - Message broker password
      - STR
      -
+   * - ISB_EXCHANGE
+     - Message Broker Exchange name for publishing messages
+     - STR
+     -
 
 Development
 -----------
 .. code-block:: bash
 
     git clone git@bitbucket.org:dkistdc/dkist-processing-core.git
     cd dkist-processing-core
```

### Comparing `dkist-processing-core-3.1.0rc2/README.rst` & `dkist-processing-core-3.2.0rc1/README.rst`

 * *Files 1% similar despite different names*

```diff
@@ -103,14 +103,18 @@
      - Message broker user name
      - STR
      -
    * - ISB_PASSWORD
      - Message broker password
      - STR
      -
+   * - ISB_EXCHANGE
+     - Message Broker Exchange name for publishing messages
+     - STR
+     -
 
 Development
 -----------
 .. code-block:: bash
 
     git clone git@bitbucket.org:dkistdc/dkist-processing-core.git
     cd dkist-processing-core
```

### Comparing `dkist-processing-core-3.1.0rc2/bitbucket-pipelines.yml` & `dkist-processing-core-3.2.0rc1/bitbucket-pipelines.yml`

 * *Files 6% similar despite different names*

```diff
@@ -1,9 +1,14 @@
 image: python:3.11
 definitions:
+  services:
+    broker:
+      image: rabbitmq:3
+      ports:
+        - 5672:5672
   steps:
     - step: &lint
         caches:
           - pip
         name: Lint
         script:
           - pip install pre-commit
@@ -20,15 +25,15 @@
           - git fetch origin main
           - towncrier check --compare-with origin/main
     - step: &scan
         caches:
           - pip
         name: Scan
         script:
-          - pip install -e .
+          - pip install .
           - pip freeze | grep -v @ > requirements.txt
           - cat requirements.txt
           - echo $SNYK_VERSION
           - curl -L -o snyk https://github.com/snyk/snyk/releases/download/$SNYK_VERSION/snyk-linux
           - chmod 755 snyk
           - ./snyk -d auth $SNYK_TOKEN
           - echo $SNYK_IGNORE
@@ -38,14 +43,15 @@
           - $SNYK_CLI_COMMAND
     - step: &test
         caches:
           - pip
 #          - docker # excluded on purpose
         services:
           - docker
+          - broker
         name: Test
         script:
           - pip install .[test]
           - pytest -m "not development" --cov dkist_processing_core
 
     - step: &push
         caches:
```

### Comparing `dkist-processing-core-3.1.0rc2/dkist_processing_core/_failure_callback.py` & `dkist-processing-core-3.2.0rc1/dkist_processing_core/_failure_callback.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,65 +1,57 @@
 """Define the failure callback functionality."""
-import json
 import logging
 from contextlib import contextmanager
-from os import environ
-from uuid import uuid4
+from typing import Callable
+from typing import Type
 
-from talus import DurableBlockingProducerWrapper
-from talus.message import message_class
+from talus import Binding
+from talus import DurableProducer
+from talus import MessageBodyBase
+from talus import PublishMessageBase
+from talus import Queue
+
+from dkist_processing_core._config import core_configurations
 
 logger = logging.getLogger(__name__)
 
 
-@message_class(routing_key="recipe.run.failure.m", queues=["recipe.run.failure.q"])
-class RecipeRunFailureMessage:
-    """Message keys for recipe run failure messages."""
+# Recipe run failure message Definition
+class RecipeRunFailureMessageBody(MessageBodyBase):
+    """Schema for the recipe run failure message body."""
 
     workflowName: str
     workflowVersion: str
     taskName: str
     dagRunId: str | None = None
     logUrl: str | None = None
-    conversationId: str = uuid4().hex
 
 
-def _isb_connection_info() -> dict:
-    try:
-        mesh_config = environ["MESH_CONFIG"]
-        mesh_config = json.loads(mesh_config)
-        # Interservice bus
-        rabbitmq_config = {
-            "rabbitmq_host": mesh_config["interservice-bus"]["mesh_address"],
-            "rabbitmq_port": mesh_config["interservice-bus"]["mesh_port"],
-            "rabbitmq_user": environ["ISB_USERNAME"],
-            "rabbitmq_pass": environ["ISB_PASSWORD"],
-            "retry_tries": 5,
-        }
-        return rabbitmq_config
-    except (KeyError, TypeError, ValueError, UnicodeDecodeError):
-        logger.warning(f"Using default rabbit mq config.  Dev Only")
-        default = {
-            "rabbitmq_host": "127.0.0.1",
-            "rabbitmq_port": 5672,
-            "rabbitmq_user": "guest",
-            "rabbitmq_pass": "guest",
-            "retry_tries": 1,
-        }
-        return default
+class RecipeRunFailureMessage(PublishMessageBase):
+    """Recipe run failure message including the message body and other publication information."""
+
+    message_body_cls: Type[RecipeRunFailureMessageBody] = RecipeRunFailureMessageBody
+    default_routing_key: str = "recipe.run.failure.m"
 
 
 @contextmanager
-def recipe_run_failure_message_producer_factory() -> DurableBlockingProducerWrapper:
+def recipe_run_failure_message_producer_factory() -> DurableProducer:
     """Create message producer for recipe run failure messages."""
+    # Configure the queue the messages should be routed to
+    recipe_run_failure_queue = Queue(
+        name="recipe.run.failure.q", arguments=core_configurations.isb_queue_arguments
+    )
+    # Configure the exchange and queue bindings for publishing
+    bindings = [Binding(queue=recipe_run_failure_queue, message=RecipeRunFailureMessage)]
     try:
-        with DurableBlockingProducerWrapper(
-            producer_queue_bindings=RecipeRunFailureMessage.binding(),
-            publish_exchange="master.direct.x",
-            **_isb_connection_info(),
+        with DurableProducer(
+            queue_bindings=bindings,
+            publish_exchange=core_configurations.isb_publish_exchange,
+            connection_parameters=core_configurations.isb_producer_connection_parameters,
+            connection_retryer=core_configurations.isb_connection_retryer,
         ) as producer:
             yield producer
     finally:
         pass
 
 
 def parse_dag_run_id_from_context(context: dict) -> str | None:
@@ -77,26 +69,28 @@
 
 
 def chat_ops_notification(
     context: dict,
     workflow_name: str,
     workflow_version: str,
     task_name: str,
-    producer_factory=recipe_run_failure_message_producer_factory,
-) -> None:
+    producer_factory: Callable[[], DurableProducer] = recipe_run_failure_message_producer_factory,
+) -> RecipeRunFailureMessage:
     """Publish message with information regarding a task failure for publication to a chat service."""
     dag_run_id = parse_dag_run_id_from_context(context)
     log_url = parse_log_url_from_context(context)
-    message = RecipeRunFailureMessage(
+    body = RecipeRunFailureMessageBody(
         workflowName=workflow_name,
         workflowVersion=workflow_version,
         taskName=task_name,
         logUrl=log_url,
         dagRunId=dag_run_id,
     )
+    message = RecipeRunFailureMessage(body)
 
     try:
         with producer_factory() as producer:
             logger.warning(f"Publishing failure callback message: {message=}")
-            return producer.publish_message(message)
-    except Exception as e:
-        logger.error(f"Error raised executing failure callback: {e=}")
+            producer.publish(message)
+            return message
+    except Exception as e:  # pragma: no cover
+        logger.error(f"Error raised executing failure callback: {e=}")  # pragma: no cover
```

### Comparing `dkist-processing-core-3.1.0rc2/dkist_processing_core/_node.py` & `dkist-processing-core-3.2.0rc1/dkist_processing_core/_node.py`

 * *Files 0% similar despite different names*

```diff
@@ -106,15 +106,15 @@
 echo NOMAD_GROUP_NAME
 echo $NOMAD_GROUP_NAME
 echo NOMAD_HOST_ADDR_worker
 echo $NOMAD_HOST_ADDR_worker
 echo NOMAD_ALLOC_NAME
 echo $NOMAD_ALLOC_NAME
 echo Host Python Environment i.e. system-site-packages
-python3 -m pip install --upgrade pip
+python3 -m pip install --upgrade --user pip
 pip list
 echo Creating Virtual Environment
 python3 -m venv --system-site-packages .task_venv
 echo Activate Environment
 . .task_venv/bin/activate
 echo Python Interpreter Location
 which python
```

### Comparing `dkist-processing-core-3.1.0rc2/dkist_processing_core/build_utils.py` & `dkist-processing-core-3.2.0rc1/dkist_processing_core/build_utils.py`

 * *Files identical despite different names*

### Comparing `dkist-processing-core-3.1.0rc2/dkist_processing_core/task.py` & `dkist-processing-core-3.2.0rc1/dkist_processing_core/task.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,113 +1,84 @@
 """
 Base class that is used to wrap the various DAG task methods.
 
 It provides support for user-defined setup and cleanup, task monitoring using Elastic APM,
 standardized logging and exception handling.
 """
-import json
 import logging
 from abc import ABC
 from abc import abstractmethod
 from contextlib import contextmanager
-from os import environ
 
 import elasticapm
 
+from dkist_processing_core._config import core_configurations
+
 
 __all__ = ["TaskBase"]
 
 logger = logging.getLogger(__name__)
 
 
 class ApmTransaction:
     """
     Elastic APM transaction manager for a DAG Task.
 
-    Without configuration it disables itself.
+    Without configuration, it disables itself.
     """
 
     @property
-    def _apm_server_url(self) -> str | None:
-        # Environment variable indicating how to connect to dependencies on the service mesh
-        raw_mesh_config = environ.get("MESH_CONFIG", default="null")
-        mesh_config = json.loads(raw_mesh_config)
-        if not mesh_config:  # no mesh config at all
-            return None
-        if not mesh_config.get("system-monitoring-log-apm"):  # no mesh config for apm
-            return None
-        return f"http://{mesh_config['system-monitoring-log-apm']['mesh_address']}:{mesh_config['system-monitoring-log-apm']['mesh_port']}"
-
-    @property
-    def _apm_other_options(self) -> dict:
-        raw_options = environ.get("ELASTIC_APM_OTHER_OPTIONS", "{}")
-        return json.loads(raw_options)
-
-    @property
     def _apm_service_name(self) -> str:
         name = f"{self._workflow_name}-{self._workflow_version}"
         name = name.replace("_", "-")
         name = name.replace(".", "-")
         return name
 
     @property
-    def _apm_is_active(self) -> bool:
-        if not self._apm_server_url:
-            return False
-        value = environ.get("ELASTIC_APM_ENABLED", "false")
-        return json.loads(value)
-
-    @property
-    def _apm_config(self) -> dict | None:
-        if not self._apm_is_active:
-            return None
-        apm_client_config = {
-            "SERVICE_NAME": self._apm_service_name,
-            "SERVER_URL": self._apm_server_url,
-            "ENVIRONMENT": "Workflows",
-            **self._apm_other_options,
-        }
-        return apm_client_config
+    def _apm_config(self) -> dict:
+        core_config = core_configurations.apm_config
+        #  Override the service name with the workflow specific name
+        core_config["SERVICE_NAME"] = self._apm_service_name
+        return core_config
 
     def __init__(self, transaction_name: str, workflow_name: str, workflow_version: str) -> None:
         self._workflow_name = workflow_name
         self._workflow_version = workflow_version
-        self.configured = bool(self._apm_config)
-        if self.configured:
-            self.transaction_name = transaction_name
+        self.transaction_name = transaction_name
+
+        if core_configurations.elastic_apm_enabled:
             self.client = elasticapm.Client(self._apm_config)
             self.instrument()
             self.client.begin_transaction(transaction_type="Task")
-            logger.info(f"APM Configured: config={self._apm_config}")
+            logger.info(f"APM Configured: {self=} {self._apm_config=}")
         else:
             logger.warning(f"APM Not Configured")
 
     @contextmanager
     def capture_span(self, name: str, *args, **kwargs):
-        if not self.configured:
+        if core_configurations.elastic_apm_enabled:
             try:
-                yield
+                with elasticapm.capture_span(name, *args, **kwargs):
+                    yield
             finally:
                 pass
         else:
             try:
-                with elasticapm.capture_span(name, *args, **kwargs):
-                    yield
+                yield
             finally:
                 pass
 
     def close(self, exc_type=None):
-        if not self.configured:
-            return
-        result = "Success"
-        if exc_type is not None:
-            result = "Error"
-            self.client.capture_exception(handled=False)
-        self.client.end_transaction(name=self.transaction_name, result=result)
-        self.client.close()
+        if core_configurations.elastic_apm_enabled:
+            result = "Success"
+            if exc_type is not None:
+                result = "Error"  # pragma: no cover
+                self.client.capture_exception(handled=False)  # pragma: no cover
+            self.client.end_transaction(name=self.transaction_name, result=result)
+            self.client.close()
 
     @staticmethod
     def instrument():
         """Vendored implementation of elasticapm.instrumentation.control.instrument changed to omit certain frameworks."""
         omit_frameworks = {
             "elasticapm.instrumentation.packages.redis.RedisInstrumentation",
             "elasticapm.instrumentation.packages.redis.RedisPipelineInstrumentation",
@@ -131,20 +102,16 @@
                 if cls_str not in _instrumentation_singletons:
                     cls = import_string(cls_str)
                     _instrumentation_singletons[cls_str] = cls()
                 obj = _instrumentation_singletons[cls_str]
                 # from elasticapm.instrumentation.control.instrument
                 obj.instrument()
 
-    def __enter__(self):
-        return self
-
-    def __exit__(self, exc_type, exc_val, exc_tb):
-        self.close(exc_type)
-        # note: exception not captured through apm due to potential size of local variables
+    def __repr__(self):
+        return f"{self.__class__.__name__}(transaction_name={self.transaction_name}, workflow_name={self._workflow_name}, workflow_version={self._workflow_version})"
 
 
 class TaskBase(ABC):
     """
     A Task is the interface between processing code and its execution.  Processing code can follow this interface through subclassing remain agnostic to the execution environment.
 
     Each DAG task must implement its own subclass of this abstract wrapper class.
```

### Comparing `dkist-processing-core-3.1.0rc2/dkist_processing_core/tests/conftest.py` & `dkist-processing-core-3.2.0rc1/dkist_processing_core/tests/conftest.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,14 +1,16 @@
 """Global test fixtures."""
 from contextlib import contextmanager
 from pathlib import Path
 from shutil import rmtree
 from typing import Any
+from unittest.mock import MagicMock
 
 import pytest
+from talus import DurableProducer
 
 from dkist_processing_core import ResourceQueue
 from dkist_processing_core import TaskBase
 from dkist_processing_core import Workflow
 from dkist_processing_core._node import Node
 from dkist_processing_core._node import task_type_hint
 from dkist_processing_core.tests.task_example import Task
@@ -26,15 +28,15 @@
 def task_subclass():
     """Sub class of the abstract task base class implementing methods that are expected to be subclassed with inspect-able metadata."""
     return Task
 
 
 @pytest.fixture(scope="session")
 def error_task_subclass():
-    """Sub class of the abstract task base class implementing methods that are expected to be subclassed with inspect-able metadata."""
+    """Subclass of the abstract task base class implementing methods that are expected to be subclassed with inspect-able metadata."""
 
     class Task(TaskBase):
         def __init__(self, *args, **kwargs):
             self.run_was_called = False
             self.post_run_was_called = False
             super().__init__(*args, **kwargs)
 
@@ -151,20 +153,15 @@
         name,
         version,
     )
 
 
 @pytest.fixture()
 def fake_producer():
-    class FakeProducer:
-        @classmethod
-        def publish_message(cls, message):
-            return message
-
-    return FakeProducer
+    return MagicMock(spec=DurableProducer)
 
 
 @pytest.fixture()
 def fake_producer_factory(fake_producer):
     @contextmanager
     def fake_factory():
         try:
```

### Comparing `dkist-processing-core-3.1.0rc2/dkist_processing_core/tests/task_example.py` & `dkist-processing-core-3.2.0rc1/dkist_processing_core/tests/task_example.py`

 * *Files identical despite different names*

### Comparing `dkist-processing-core-3.1.0rc2/dkist_processing_core/tests/test_build_utils.py` & `dkist-processing-core-3.2.0rc1/dkist_processing_core/tests/test_build_utils.py`

 * *Files 2% similar despite different names*

```diff
@@ -85,14 +85,15 @@
 def notebook_export_path(repository_root_path) -> Path:
     """Return a directory relative to repository root"""
     export_path = Path("notebooks/")
     yield Path("notebooks/")
     rmtree(export_path, ignore_errors=True)
 
 
+@pytest.mark.long()
 def test_export_notebook_dockerfile(repository_root_path, notebook_export_path):
     """
     Given: A path to export to and a package containing a valid workflow.
     When: Workflows in the package are exported as a valid Dockerfile.
     Then: Expected export file exists.
     """
     os.chdir(str(repository_root_path))
```

### Comparing `dkist-processing-core-3.1.0rc2/dkist_processing_core/tests/test_export.py` & `dkist-processing-core-3.2.0rc1/dkist_processing_core/tests/test_export.py`

 * *Files identical despite different names*

### Comparing `dkist-processing-core-3.1.0rc2/dkist_processing_core/tests/test_node.py` & `dkist-processing-core-3.2.0rc1/dkist_processing_core/tests/test_node.py`

 * *Files 2% similar despite different names*

```diff
@@ -44,26 +44,28 @@
     assert node.upstreams == upstream
     assert node.task == task
     assert node.workflow_version == version
     assert node.resource_queue == queue_name
     assert node.pip_extras == pip_extras
 
 
+@pytest.mark.long()
 def test_node_bash_template_return_0(node):
     """
     Given: A valid node instance.
     When: Running the bash script template WITHOUT an error producing python call.
     Then: It returns a 0.
     """
     node, *args = node
     cmd = 'python -c "pass"'
     result = subprocess.run(node._bash_template(cmd), shell=True, check=True)
     assert result.returncode == 0
 
 
+@pytest.mark.long()
 def test_node_bash_template_return_1(node):
     """
     Given: A valid node instance.
     When: Running the bash script template WITH an error producing python call.
     Then: It returns a 1.
     """
     node, *args = node
```

### Comparing `dkist-processing-core-3.1.0rc2/dkist_processing_core/tests/test_workflow.py` & `dkist-processing-core-3.2.0rc1/dkist_processing_core/tests/test_workflow.py`

 * *Files identical despite different names*

### Comparing `dkist-processing-core-3.1.0rc2/dkist_processing_core/tests/valid_workflow_package/workflow.py` & `dkist-processing-core-3.2.0rc1/dkist_processing_core/tests/valid_workflow_package/workflow.py`

 * *Files identical despite different names*

### Comparing `dkist-processing-core-3.1.0rc2/dkist_processing_core/workflow.py` & `dkist-processing-core-3.2.0rc1/dkist_processing_core/workflow.py`

 * *Files identical despite different names*

### Comparing `dkist-processing-core-3.1.0rc2/dkist_processing_core.egg-info/PKG-INFO` & `dkist-processing-core-3.2.0rc1/dkist_processing_core.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: dkist-processing-core
-Version: 3.1.0rc2
+Version: 3.2.0rc1
 Summary: Abstraction layer that is used by the DKIST Science Data Processing pipelines to process DKIST data using Apache Airflow.
 Home-page: https://bitbucket.org/dkistdc/dkist-processing-core/src/main/
 Author: NSO / AURA
 Author-email: "dkistdc@nso.edu"
 License: MIT
 Project-URL: Documentation, https://docs.dkist.nso.edu/projects/core
 Classifier: Programming Language :: Python
@@ -119,14 +119,18 @@
      - Message broker user name
      - STR
      -
    * - ISB_PASSWORD
      - Message broker password
      - STR
      -
+   * - ISB_EXCHANGE
+     - Message Broker Exchange name for publishing messages
+     - STR
+     -
 
 Development
 -----------
 .. code-block:: bash
 
     git clone git@bitbucket.org:dkistdc/dkist-processing-core.git
     cd dkist-processing-core
```

### Comparing `dkist-processing-core-3.1.0rc2/dkist_processing_core.egg-info/SOURCES.txt` & `dkist-processing-core-3.2.0rc1/dkist_processing_core.egg-info/SOURCES.txt`

 * *Files 4% similar despite different names*

```diff
@@ -5,16 +5,18 @@
 README.rst
 bitbucket-pipelines.yml
 check_changelog_updated.sh
 pyproject.toml
 setup.cfg
 setup.py
 changelog/.gitempty
-changelog/32.feature.rst
+changelog/33.bugfix.rst
+changelog/34.misc.rst
 dkist_processing_core/__init__.py
+dkist_processing_core/_config.py
 dkist_processing_core/_failure_callback.py
 dkist_processing_core/_node.py
 dkist_processing_core/build_utils.py
 dkist_processing_core/resource_queue.py
 dkist_processing_core/task.py
 dkist_processing_core/workflow.py
 dkist_processing_core.egg-info/PKG-INFO
```

### Comparing `dkist-processing-core-3.1.0rc2/docs/Makefile` & `dkist-processing-core-3.2.0rc1/docs/Makefile`

 * *Files identical despite different names*

### Comparing `dkist-processing-core-3.1.0rc2/docs/auto-proc-concept-model.png` & `dkist-processing-core-3.2.0rc1/docs/auto-proc-concept-model.png`

 * *Files identical despite different names*

### Comparing `dkist-processing-core-3.1.0rc2/docs/auto_proc_brick.png` & `dkist-processing-core-3.2.0rc1/docs/auto_proc_brick.png`

 * *Files identical despite different names*

### Comparing `dkist-processing-core-3.1.0rc2/docs/automated-processing-deployed.png` & `dkist-processing-core-3.2.0rc1/docs/automated-processing-deployed.png`

 * *Files identical despite different names*

### Comparing `dkist-processing-core-3.1.0rc2/docs/conf.py` & `dkist-processing-core-3.2.0rc1/docs/conf.py`

 * *Files identical despite different names*

### Comparing `dkist-processing-core-3.1.0rc2/docs/make.bat` & `dkist-processing-core-3.2.0rc1/docs/make.bat`

 * *Files identical despite different names*

### Comparing `dkist-processing-core-3.1.0rc2/licenses/LICENSE.rst` & `dkist-processing-core-3.2.0rc1/licenses/LICENSE.rst`

 * *Files identical despite different names*

### Comparing `dkist-processing-core-3.1.0rc2/pyproject.toml` & `dkist-processing-core-3.2.0rc1/pyproject.toml`

 * *Files identical despite different names*

### Comparing `dkist-processing-core-3.1.0rc2/setup.cfg` & `dkist-processing-core-3.2.0rc1/setup.cfg`

 * *Files 10% similar despite different names*

```diff
@@ -15,25 +15,28 @@
 
 [options]
 python_requires = >=3.11
 setup_requires = setuptools_scm
 packages = find:
 include_package_data = True
 install_requires = 
-	apache-airflow[postgres, celery] == 2.7.3
+	apache-airflow[postgres, celery] == 2.9.1
 	elastic-apm < 7.0.0
 	requests >= 2.23
-	talus >= 0.2.0
+	talus >= 1.1.0, <2.0
 	pendulum
 	nbformat >= 5.9.2
+	dkist-service-configuration >=2.0.1, <3.0
+	pydantic > 2.0
 
 [options.extras_require]
 test = 
 	pytest
 	pytest-cov
+	pytest-mock
 	jinja2
 	towncrier
 	nbconvert
 docs = 
 	sphinx
 	sphinx-astropy
 	sphinx-changelog
@@ -52,12 +55,18 @@
 [upload_docs]
 upload-dir = docs/_build/html
 show-response = 1
 
 [tool:pytest]
 markers = 
 	development: For tests that can only be  run while developing with a sidecar proxy (as opposed to in bitbucket pipelines)
+	long: For tests that take a long time to run.
+
+[coverage:run]
+omit = 
+	dkist_processing_core/tests/*
+	dkist_processing_core/__init__.py
 
 [egg_info]
 tag_build = 
 tag_date = 0
```

