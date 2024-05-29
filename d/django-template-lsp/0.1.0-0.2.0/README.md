# Comparing `tmp/django_template_lsp-0.1.0.tar.gz` & `tmp/django_template_lsp-0.2.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "django_template_lsp-0.1.0.tar", last modified: Fri May 17 13:08:41 2024, max compression
+gzip compressed data, was "django_template_lsp-0.2.0.tar", last modified: Wed May 29 14:46:25 2024, max compression
```

## Comparing `django_template_lsp-0.1.0.tar` & `django_template_lsp-0.2.0.tar`

### file list

```diff
@@ -1,18 +1,21 @@
-drwxr-xr-x   0 maikel    (1000) maikel    (1000)        0 2024-05-17 13:08:41.765181 django_template_lsp-0.1.0/
--rw-r--r--   0 maikel    (1000) maikel    (1000)      784 2024-05-17 13:08:41.765181 django_template_lsp-0.1.0/PKG-INFO
--rw-r--r--   0 maikel    (1000) maikel    (1000)      350 2024-05-17 12:59:53.000000 django_template_lsp-0.1.0/README.md
-drwxr-xr-x   0 maikel    (1000) maikel    (1000)        0 2024-05-17 13:08:41.765181 django_template_lsp-0.1.0/django_template_lsp.egg-info/
--rw-r--r--   0 maikel    (1000) maikel    (1000)      784 2024-05-17 13:08:41.000000 django_template_lsp-0.1.0/django_template_lsp.egg-info/PKG-INFO
--rw-r--r--   0 maikel    (1000) maikel    (1000)      363 2024-05-17 13:08:41.000000 django_template_lsp-0.1.0/django_template_lsp.egg-info/SOURCES.txt
--rw-r--r--   0 maikel    (1000) maikel    (1000)        1 2024-05-17 13:08:41.000000 django_template_lsp-0.1.0/django_template_lsp.egg-info/dependency_links.txt
--rw-r--r--   0 maikel    (1000) maikel    (1000)       78 2024-05-17 13:08:41.000000 django_template_lsp-0.1.0/django_template_lsp.egg-info/entry_points.txt
--rw-r--r--   0 maikel    (1000) maikel    (1000)       63 2024-05-17 13:08:41.000000 django_template_lsp-0.1.0/django_template_lsp.egg-info/requires.txt
--rw-r--r--   0 maikel    (1000) maikel    (1000)        6 2024-05-17 13:08:41.000000 django_template_lsp-0.1.0/django_template_lsp.egg-info/top_level.txt
-drwxr-xr-x   0 maikel    (1000) maikel    (1000)        0 2024-05-17 13:08:41.765181 django_template_lsp-0.1.0/djlsp/
--rw-r--r--   0 maikel    (1000) maikel    (1000)       22 2024-05-17 13:06:53.000000 django_template_lsp-0.1.0/djlsp/__init__.py
--rw-r--r--   0 maikel    (1000) maikel    (1000)       35 2024-05-17 11:41:45.000000 django_template_lsp-0.1.0/djlsp/__main__.py
--rw-r--r--   0 maikel    (1000) maikel    (1000)       68 2024-05-17 11:41:01.000000 django_template_lsp-0.1.0/djlsp/cli.py
--rw-r--r--   0 maikel    (1000) maikel    (1000)     2793 2024-05-17 12:56:07.000000 django_template_lsp-0.1.0/djlsp/completion.py
--rw-r--r--   0 maikel    (1000) maikel    (1000)      931 2024-05-17 12:56:16.000000 django_template_lsp-0.1.0/djlsp/server.py
--rw-r--r--   0 maikel    (1000) maikel    (1000)       38 2024-05-17 13:08:41.765181 django_template_lsp-0.1.0/setup.cfg
--rw-r--r--   0 maikel    (1000) maikel    (1000)      842 2024-05-17 11:44:53.000000 django_template_lsp-0.1.0/setup.py
+drwxr-xr-x   0 maikel    (1000) maikel    (1000)        0 2024-05-29 14:46:25.049451 django_template_lsp-0.2.0/
+-rw-r--r--   0 maikel    (1000) maikel    (1000)     1331 2024-05-29 14:46:25.049451 django_template_lsp-0.2.0/PKG-INFO
+-rw-r--r--   0 maikel    (1000) maikel    (1000)      862 2024-05-29 14:45:50.000000 django_template_lsp-0.2.0/README.md
+drwxr-xr-x   0 maikel    (1000) maikel    (1000)        0 2024-05-29 14:46:25.049451 django_template_lsp-0.2.0/django_template_lsp.egg-info/
+-rw-r--r--   0 maikel    (1000) maikel    (1000)     1331 2024-05-29 14:46:25.000000 django_template_lsp-0.2.0/django_template_lsp.egg-info/PKG-INFO
+-rw-r--r--   0 maikel    (1000) maikel    (1000)      419 2024-05-29 14:46:25.000000 django_template_lsp-0.2.0/django_template_lsp.egg-info/SOURCES.txt
+-rw-r--r--   0 maikel    (1000) maikel    (1000)        1 2024-05-29 14:46:25.000000 django_template_lsp-0.2.0/django_template_lsp.egg-info/dependency_links.txt
+-rw-r--r--   0 maikel    (1000) maikel    (1000)       78 2024-05-29 14:46:25.000000 django_template_lsp-0.2.0/django_template_lsp.egg-info/entry_points.txt
+-rw-r--r--   0 maikel    (1000) maikel    (1000)       67 2024-05-29 14:46:25.000000 django_template_lsp-0.2.0/django_template_lsp.egg-info/requires.txt
+-rw-r--r--   0 maikel    (1000) maikel    (1000)        6 2024-05-29 14:46:25.000000 django_template_lsp-0.2.0/django_template_lsp.egg-info/top_level.txt
+drwxr-xr-x   0 maikel    (1000) maikel    (1000)        0 2024-05-29 14:46:25.049451 django_template_lsp-0.2.0/djlsp/
+-rw-r--r--   0 maikel    (1000) maikel    (1000)       22 2024-05-29 14:46:03.000000 django_template_lsp-0.2.0/djlsp/__init__.py
+-rw-r--r--   0 maikel    (1000) maikel    (1000)       35 2024-05-17 11:41:45.000000 django_template_lsp-0.2.0/djlsp/__main__.py
+-rw-r--r--   0 maikel    (1000) maikel    (1000)      515 2024-05-29 14:45:50.000000 django_template_lsp-0.2.0/djlsp/cli.py
+-rw-r--r--   0 maikel    (1000) maikel    (1000)     4103 2024-05-29 14:45:50.000000 django_template_lsp-0.2.0/djlsp/constants.py
+-rw-r--r--   0 maikel    (1000) maikel    (1000)     4255 2024-05-29 14:45:50.000000 django_template_lsp-0.2.0/djlsp/parser.py
+-rw-r--r--   0 maikel    (1000) maikel    (1000)     6881 2024-05-29 14:45:50.000000 django_template_lsp-0.2.0/djlsp/server.py
+-rw-r--r--   0 maikel    (1000) maikel    (1000)      141 2024-05-29 14:46:25.049451 django_template_lsp-0.2.0/setup.cfg
+-rw-r--r--   0 maikel    (1000) maikel    (1000)      841 2024-05-29 14:45:50.000000 django_template_lsp-0.2.0/setup.py
+drwxr-xr-x   0 maikel    (1000) maikel    (1000)        0 2024-05-29 14:46:25.049451 django_template_lsp-0.2.0/tests/
+-rw-r--r--   0 maikel    (1000) maikel    (1000)     1036 2024-05-29 14:45:50.000000 django_template_lsp-0.2.0/tests/test_django_collector.py
```

### Comparing `django_template_lsp-0.1.0/setup.py` & `django_template_lsp-0.2.0/setup.py`

 * *Files 9% similar despite different names*

```diff
@@ -1,10 +1,8 @@
-import os
-
-from setuptools import Command, find_packages, setup
+from setuptools import find_packages, setup
 
 from djlsp import __version__
 
 
 def readme():
     with open("README.md") as f:
         return f.read()
@@ -25,14 +23,15 @@
     },
     python_requires=">= 3.9",
     install_requires=[
         "pygls",
     ],
     extras_require={
         "dev": [
+            "tox",
             "black",
             "isort",
             "flake8",
             "pytest",
             "pytest-check",
             "pytest-cov",
         ]
```

