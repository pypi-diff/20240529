# Comparing `tmp/clinvar-this-0.8.0.tar.gz` & `tmp/clinvar-this-0.9.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "clinvar-this-0.8.0.tar", last modified: Fri Sep  8 07:31:44 2023, max compression
+gzip compressed data, was "clinvar-this-0.9.0.tar", last modified: Fri Sep  8 12:12:14 2023, max compression
```

## Comparing `clinvar-this-0.8.0.tar` & `clinvar-this-0.9.0.tar`

### file list

```diff
@@ -1,86 +1,86 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-09-08 07:31:44.914453 clinvar-this-0.8.0/
--rw-r--r--   0 runner    (1001) docker     (127)      173 2023-09-08 07:31:39.000000 clinvar-this-0.8.0/AUTHORS.rst
--rw-r--r--   0 runner    (1001) docker     (127)    12200 2023-09-08 07:31:39.000000 clinvar-this-0.8.0/CHANGELOG.md
--rw-r--r--   0 runner    (1001) docker     (127)     3043 2023-09-08 07:31:39.000000 clinvar-this-0.8.0/CONTRIBUTING.rst
--rw-r--r--   0 runner    (1001) docker     (127)     1075 2023-09-08 07:31:39.000000 clinvar-this-0.8.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)      332 2023-09-08 07:31:39.000000 clinvar-this-0.8.0/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (127)    14368 2023-09-08 07:31:44.914453 clinvar-this-0.8.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     1357 2023-09-08 07:31:39.000000 clinvar-this-0.8.0/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-09-08 07:31:44.902453 clinvar-this-0.8.0/clinvar_api/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2023-09-08 07:31:39.000000 clinvar-this-0.8.0/clinvar_api/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     8399 2023-09-08 07:31:39.000000 clinvar-this-0.8.0/clinvar_api/client.py
--rw-r--r--   0 runner    (1001) docker     (127)     1243 2023-09-08 07:31:39.000000 clinvar-this-0.8.0/clinvar_api/common.py
--rw-r--r--   0 runner    (1001) docker     (127)        0 2023-09-08 07:31:39.000000 clinvar-this-0.8.0/clinvar_api/constants.py
--rw-r--r--   0 runner    (1001) docker     (127)      333 2023-09-08 07:31:39.000000 clinvar-this-0.8.0/clinvar_api/exceptions.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-09-08 07:31:44.902453 clinvar-this-0.8.0/clinvar_api/models/
--rw-r--r--   0 runner    (1001) docker     (127)      347 2023-09-08 07:31:39.000000 clinvar-this-0.8.0/clinvar_api/models/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     3878 2023-09-08 07:31:39.000000 clinvar-this-0.8.0/clinvar_api/models/query_response.py
--rw-r--r--   0 runner    (1001) docker     (127)    17079 2023-09-08 07:31:39.000000 clinvar-this-0.8.0/clinvar_api/models/sub_payload.py
--rw-r--r--   0 runner    (1001) docker     (127)     6908 2023-09-08 07:31:39.000000 clinvar-this-0.8.0/clinvar_api/models/sub_response.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-09-08 07:31:44.902453 clinvar-this-0.8.0/clinvar_api/msg/
--rw-r--r--   0 runner    (1001) docker     (127)      356 2023-09-08 07:31:39.000000 clinvar-this-0.8.0/clinvar_api/msg/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2604 2023-09-08 07:31:39.000000 clinvar-this-0.8.0/clinvar_api/msg/query_response.py
--rw-r--r--   0 runner    (1001) docker     (127)    11495 2023-09-08 07:31:39.000000 clinvar-this-0.8.0/clinvar_api/msg/sub_payload.py
--rw-r--r--   0 runner    (1001) docker     (127)     2981 2023-09-08 07:31:39.000000 clinvar-this-0.8.0/clinvar_api/msg/sub_response.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-09-08 07:31:44.902453 clinvar-this-0.8.0/clinvar_api/schemas/
--rw-r--r--   0 runner    (1001) docker     (127)      626 2023-09-08 07:31:39.000000 clinvar-this-0.8.0/clinvar_api/schemas/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-09-08 07:31:44.906453 clinvar-this-0.8.0/clinvar_data/
--rw-r--r--   0 runner    (1001) docker     (127)       35 2023-09-08 07:31:39.000000 clinvar-this-0.8.0/clinvar_data/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      501 2023-09-08 07:31:39.000000 clinvar-this-0.8.0/clinvar_data/cattrs_helpers.py
--rw-r--r--   0 runner    (1001) docker     (127)     3480 2023-09-08 07:31:39.000000 clinvar-this-0.8.0/clinvar_data/class_by_freq.py
--rw-r--r--   0 runner    (1001) docker     (127)     3369 2023-09-08 07:31:39.000000 clinvar-this-0.8.0/clinvar_data/conversion.py
--rw-r--r--   0 runner    (1001) docker     (127)     6054 2023-09-08 07:31:39.000000 clinvar-this-0.8.0/clinvar_data/extract_vars.py
--rw-r--r--   0 runner    (1001) docker     (127)     5756 2023-09-08 07:31:39.000000 clinvar-this-0.8.0/clinvar_data/gene_impact.py
--rw-r--r--   0 runner    (1001) docker     (127)   102937 2023-09-08 07:31:39.000000 clinvar-this-0.8.0/clinvar_data/models.py
--rw-r--r--   0 runner    (1001) docker     (127)     4073 2023-09-08 07:31:39.000000 clinvar-this-0.8.0/clinvar_data/phenotype_link.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-09-08 07:31:44.906453 clinvar-this-0.8.0/clinvar_this/
--rw-r--r--   0 runner    (1001) docker     (127)      197 2023-09-08 07:31:39.000000 clinvar-this-0.8.0/clinvar_this/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)       22 2023-09-08 07:31:39.000000 clinvar-this-0.8.0/clinvar_this/_version.py
--rw-r--r--   0 runner    (1001) docker     (127)    13810 2023-09-08 07:31:39.000000 clinvar-this-0.8.0/clinvar_this/batches.py
--rw-r--r--   0 runner    (1001) docker     (127)     8543 2023-09-08 07:31:39.000000 clinvar-this-0.8.0/clinvar_this/cli.py
--rw-r--r--   0 runner    (1001) docker     (127)     2952 2023-09-08 07:31:39.000000 clinvar-this-0.8.0/clinvar_this/config.py
--rw-r--r--   0 runner    (1001) docker     (127)      659 2023-09-08 07:31:39.000000 clinvar-this-0.8.0/clinvar_this/exceptions.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-09-08 07:31:44.910453 clinvar-this-0.8.0/clinvar_this/io/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2023-09-08 07:31:39.000000 clinvar-this-0.8.0/clinvar_this/io/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    36408 2023-09-08 07:31:39.000000 clinvar-this-0.8.0/clinvar_this/io/tsv.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-09-08 07:31:44.906453 clinvar-this-0.8.0/clinvar_this.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)    14368 2023-09-08 07:31:44.000000 clinvar-this-0.8.0/clinvar_this.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     1783 2023-09-08 07:31:44.000000 clinvar-this-0.8.0/clinvar_this.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2023-09-08 07:31:44.000000 clinvar-this-0.8.0/clinvar_this.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       54 2023-09-08 07:31:44.000000 clinvar-this-0.8.0/clinvar_this.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2023-09-08 07:31:44.000000 clinvar-this-0.8.0/clinvar_this.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (127)      222 2023-09-08 07:31:44.000000 clinvar-this-0.8.0/clinvar_this.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       38 2023-09-08 07:31:44.000000 clinvar-this-0.8.0/clinvar_this.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-09-08 07:31:44.910453 clinvar-this-0.8.0/docs/
--rw-r--r--   0 runner    (1001) docker     (127)      613 2023-09-08 07:31:39.000000 clinvar-this-0.8.0/docs/Makefile
--rw-r--r--   0 runner    (1001) docker     (127)     2720 2023-09-08 07:31:39.000000 clinvar-this-0.8.0/docs/api_vs_cli.rst
--rw-r--r--   0 runner    (1001) docker     (127)       28 2023-09-08 07:31:39.000000 clinvar-this-0.8.0/docs/authors.rst
--rw-r--r--   0 runner    (1001) docker     (127)      154 2023-09-08 07:31:39.000000 clinvar-this-0.8.0/docs/cli.rst
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-09-08 07:31:44.914453 clinvar-this-0.8.0/docs/clinvar_api/
--rw-r--r--   0 runner    (1001) docker     (127)      763 2023-09-08 07:31:39.000000 clinvar-this-0.8.0/docs/clinvar_api/clinvar_api.models.rst
--rw-r--r--   0 runner    (1001) docker     (127)      727 2023-09-08 07:31:39.000000 clinvar-this-0.8.0/docs/clinvar_api/clinvar_api.msg.rst
--rw-r--r--   0 runner    (1001) docker     (127)      879 2023-09-08 07:31:39.000000 clinvar-this-0.8.0/docs/clinvar_api/clinvar_api.rst
--rw-r--r--   0 runner    (1001) docker     (127)       70 2023-09-08 07:31:39.000000 clinvar-this-0.8.0/docs/clinvar_api/modules.rst
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-09-08 07:31:44.914453 clinvar-this-0.8.0/docs/clinvar_this/
--rw-r--r--   0 runner    (1001) docker     (127)      622 2023-09-08 07:31:39.000000 clinvar-this-0.8.0/docs/clinvar_this/clinvar_this.rst
--rw-r--r--   0 runner    (1001) docker     (127)       73 2023-09-08 07:31:39.000000 clinvar-this-0.8.0/docs/clinvar_this/modules.rst
--rw-r--r--   0 runner    (1001) docker     (127)     2312 2023-09-08 07:31:39.000000 clinvar-this-0.8.0/docs/common_errors.rst
--rwxr-xr-x   0 runner    (1001) docker     (127)     4952 2023-09-08 07:31:39.000000 clinvar-this-0.8.0/docs/conf.py
--rw-r--r--   0 runner    (1001) docker     (127)       33 2023-09-08 07:31:39.000000 clinvar-this-0.8.0/docs/contributing.rst
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-09-08 07:31:44.914453 clinvar-this-0.8.0/docs/figures/
--rw-r--r--   0 runner    (1001) docker     (127)    36166 2023-09-08 07:31:39.000000 clinvar-this-0.8.0/docs/figures/clinvar-this-workflow.png
--rw-r--r--   0 runner    (1001) docker     (127)    12734 2023-09-08 07:31:39.000000 clinvar-this-0.8.0/docs/file_formats.rst
--rw-r--r--   0 runner    (1001) docker     (127)     6495 2023-09-08 07:31:39.000000 clinvar-this-0.8.0/docs/getting_started.rst
--rw-r--r--   0 runner    (1001) docker     (127)       31 2023-09-08 07:31:39.000000 clinvar-this-0.8.0/docs/history.rst
--rw-r--r--   0 runner    (1001) docker     (127)     1138 2023-09-08 07:31:39.000000 clinvar-this-0.8.0/docs/index.rst
--rw-r--r--   0 runner    (1001) docker     (127)     1334 2023-09-08 07:31:39.000000 clinvar-this-0.8.0/docs/installation.rst
--rw-r--r--   0 runner    (1001) docker     (127)     3723 2023-09-08 07:31:39.000000 clinvar-this-0.8.0/docs/limitations.rst
--rw-r--r--   0 runner    (1001) docker     (127)      810 2023-09-08 07:31:39.000000 clinvar-this-0.8.0/docs/make.bat
--rw-r--r--   0 runner    (1001) docker     (127)     8337 2023-09-08 07:31:39.000000 clinvar-this-0.8.0/docs/usage_cli.rst
--rw-r--r--   0 runner    (1001) docker     (127)      212 2023-09-08 07:31:39.000000 clinvar-this-0.8.0/docs/usage_library.rst
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-09-08 07:31:44.914453 clinvar-this-0.8.0/requirements/
--rw-r--r--   0 runner    (1001) docker     (127)      244 2023-09-08 07:31:39.000000 clinvar-this-0.8.0/requirements/base.txt
--rw-r--r--   0 runner    (1001) docker     (127)       12 2023-09-08 07:31:39.000000 clinvar-this-0.8.0/requirements/dev.txt
--rw-r--r--   0 runner    (1001) docker     (127)      436 2023-09-08 07:31:39.000000 clinvar-this-0.8.0/requirements/test.txt
--rw-r--r--   0 runner    (1001) docker     (127)      405 2023-09-08 07:31:44.914453 clinvar-this-0.8.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)     2473 2023-09-08 07:31:39.000000 clinvar-this-0.8.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-09-08 12:12:14.756389 clinvar-this-0.9.0/
+-rw-r--r--   0 runner    (1001) docker     (127)      173 2023-09-08 12:12:07.000000 clinvar-this-0.9.0/AUTHORS.rst
+-rw-r--r--   0 runner    (1001) docker     (127)    12747 2023-09-08 12:12:07.000000 clinvar-this-0.9.0/CHANGELOG.md
+-rw-r--r--   0 runner    (1001) docker     (127)     3043 2023-09-08 12:12:07.000000 clinvar-this-0.9.0/CONTRIBUTING.rst
+-rw-r--r--   0 runner    (1001) docker     (127)     1075 2023-09-08 12:12:07.000000 clinvar-this-0.9.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)      332 2023-09-08 12:12:07.000000 clinvar-this-0.9.0/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (127)    14915 2023-09-08 12:12:14.756389 clinvar-this-0.9.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     1357 2023-09-08 12:12:07.000000 clinvar-this-0.9.0/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-09-08 12:12:14.748389 clinvar-this-0.9.0/clinvar_api/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2023-09-08 12:12:07.000000 clinvar-this-0.9.0/clinvar_api/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8399 2023-09-08 12:12:07.000000 clinvar-this-0.9.0/clinvar_api/client.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1243 2023-09-08 12:12:07.000000 clinvar-this-0.9.0/clinvar_api/common.py
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2023-09-08 12:12:07.000000 clinvar-this-0.9.0/clinvar_api/constants.py
+-rw-r--r--   0 runner    (1001) docker     (127)      333 2023-09-08 12:12:07.000000 clinvar-this-0.9.0/clinvar_api/exceptions.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-09-08 12:12:14.748389 clinvar-this-0.9.0/clinvar_api/models/
+-rw-r--r--   0 runner    (1001) docker     (127)      347 2023-09-08 12:12:07.000000 clinvar-this-0.9.0/clinvar_api/models/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3878 2023-09-08 12:12:07.000000 clinvar-this-0.9.0/clinvar_api/models/query_response.py
+-rw-r--r--   0 runner    (1001) docker     (127)    17079 2023-09-08 12:12:07.000000 clinvar-this-0.9.0/clinvar_api/models/sub_payload.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6908 2023-09-08 12:12:07.000000 clinvar-this-0.9.0/clinvar_api/models/sub_response.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-09-08 12:12:14.748389 clinvar-this-0.9.0/clinvar_api/msg/
+-rw-r--r--   0 runner    (1001) docker     (127)      356 2023-09-08 12:12:07.000000 clinvar-this-0.9.0/clinvar_api/msg/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2604 2023-09-08 12:12:07.000000 clinvar-this-0.9.0/clinvar_api/msg/query_response.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11495 2023-09-08 12:12:07.000000 clinvar-this-0.9.0/clinvar_api/msg/sub_payload.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2981 2023-09-08 12:12:07.000000 clinvar-this-0.9.0/clinvar_api/msg/sub_response.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-09-08 12:12:14.748389 clinvar-this-0.9.0/clinvar_api/schemas/
+-rw-r--r--   0 runner    (1001) docker     (127)      626 2023-09-08 12:12:07.000000 clinvar-this-0.9.0/clinvar_api/schemas/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-09-08 12:12:14.752389 clinvar-this-0.9.0/clinvar_data/
+-rw-r--r--   0 runner    (1001) docker     (127)       35 2023-09-08 12:12:07.000000 clinvar-this-0.9.0/clinvar_data/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      501 2023-09-08 12:12:07.000000 clinvar-this-0.9.0/clinvar_data/cattrs_helpers.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3480 2023-09-08 12:12:07.000000 clinvar-this-0.9.0/clinvar_data/class_by_freq.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3369 2023-09-08 12:12:07.000000 clinvar-this-0.9.0/clinvar_data/conversion.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6566 2023-09-08 12:12:07.000000 clinvar-this-0.9.0/clinvar_data/extract_vars.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5854 2023-09-08 12:12:07.000000 clinvar-this-0.9.0/clinvar_data/gene_impact.py
+-rw-r--r--   0 runner    (1001) docker     (127)   102937 2023-09-08 12:12:07.000000 clinvar-this-0.9.0/clinvar_data/models.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4073 2023-09-08 12:12:07.000000 clinvar-this-0.9.0/clinvar_data/phenotype_link.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-09-08 12:12:14.752389 clinvar-this-0.9.0/clinvar_this/
+-rw-r--r--   0 runner    (1001) docker     (127)      197 2023-09-08 12:12:07.000000 clinvar-this-0.9.0/clinvar_this/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)       22 2023-09-08 12:12:07.000000 clinvar-this-0.9.0/clinvar_this/_version.py
+-rw-r--r--   0 runner    (1001) docker     (127)    13810 2023-09-08 12:12:07.000000 clinvar-this-0.9.0/clinvar_this/batches.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8543 2023-09-08 12:12:07.000000 clinvar-this-0.9.0/clinvar_this/cli.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2952 2023-09-08 12:12:07.000000 clinvar-this-0.9.0/clinvar_this/config.py
+-rw-r--r--   0 runner    (1001) docker     (127)      659 2023-09-08 12:12:07.000000 clinvar-this-0.9.0/clinvar_this/exceptions.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-09-08 12:12:14.752389 clinvar-this-0.9.0/clinvar_this/io/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2023-09-08 12:12:07.000000 clinvar-this-0.9.0/clinvar_this/io/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    36408 2023-09-08 12:12:07.000000 clinvar-this-0.9.0/clinvar_this/io/tsv.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-09-08 12:12:14.752389 clinvar-this-0.9.0/clinvar_this.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)    14915 2023-09-08 12:12:14.000000 clinvar-this-0.9.0/clinvar_this.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     1783 2023-09-08 12:12:14.000000 clinvar-this-0.9.0/clinvar_this.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2023-09-08 12:12:14.000000 clinvar-this-0.9.0/clinvar_this.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       54 2023-09-08 12:12:14.000000 clinvar-this-0.9.0/clinvar_this.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2023-09-08 12:12:14.000000 clinvar-this-0.9.0/clinvar_this.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (127)      222 2023-09-08 12:12:14.000000 clinvar-this-0.9.0/clinvar_this.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2023-09-08 12:12:14.000000 clinvar-this-0.9.0/clinvar_this.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-09-08 12:12:14.752389 clinvar-this-0.9.0/docs/
+-rw-r--r--   0 runner    (1001) docker     (127)      613 2023-09-08 12:12:07.000000 clinvar-this-0.9.0/docs/Makefile
+-rw-r--r--   0 runner    (1001) docker     (127)     2720 2023-09-08 12:12:07.000000 clinvar-this-0.9.0/docs/api_vs_cli.rst
+-rw-r--r--   0 runner    (1001) docker     (127)       28 2023-09-08 12:12:07.000000 clinvar-this-0.9.0/docs/authors.rst
+-rw-r--r--   0 runner    (1001) docker     (127)      154 2023-09-08 12:12:07.000000 clinvar-this-0.9.0/docs/cli.rst
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-09-08 12:12:14.752389 clinvar-this-0.9.0/docs/clinvar_api/
+-rw-r--r--   0 runner    (1001) docker     (127)      763 2023-09-08 12:12:07.000000 clinvar-this-0.9.0/docs/clinvar_api/clinvar_api.models.rst
+-rw-r--r--   0 runner    (1001) docker     (127)      727 2023-09-08 12:12:07.000000 clinvar-this-0.9.0/docs/clinvar_api/clinvar_api.msg.rst
+-rw-r--r--   0 runner    (1001) docker     (127)      879 2023-09-08 12:12:07.000000 clinvar-this-0.9.0/docs/clinvar_api/clinvar_api.rst
+-rw-r--r--   0 runner    (1001) docker     (127)       70 2023-09-08 12:12:07.000000 clinvar-this-0.9.0/docs/clinvar_api/modules.rst
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-09-08 12:12:14.752389 clinvar-this-0.9.0/docs/clinvar_this/
+-rw-r--r--   0 runner    (1001) docker     (127)      622 2023-09-08 12:12:07.000000 clinvar-this-0.9.0/docs/clinvar_this/clinvar_this.rst
+-rw-r--r--   0 runner    (1001) docker     (127)       73 2023-09-08 12:12:07.000000 clinvar-this-0.9.0/docs/clinvar_this/modules.rst
+-rw-r--r--   0 runner    (1001) docker     (127)     2312 2023-09-08 12:12:07.000000 clinvar-this-0.9.0/docs/common_errors.rst
+-rwxr-xr-x   0 runner    (1001) docker     (127)     4952 2023-09-08 12:12:07.000000 clinvar-this-0.9.0/docs/conf.py
+-rw-r--r--   0 runner    (1001) docker     (127)       33 2023-09-08 12:12:07.000000 clinvar-this-0.9.0/docs/contributing.rst
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-09-08 12:12:14.752389 clinvar-this-0.9.0/docs/figures/
+-rw-r--r--   0 runner    (1001) docker     (127)    36166 2023-09-08 12:12:07.000000 clinvar-this-0.9.0/docs/figures/clinvar-this-workflow.png
+-rw-r--r--   0 runner    (1001) docker     (127)    12734 2023-09-08 12:12:07.000000 clinvar-this-0.9.0/docs/file_formats.rst
+-rw-r--r--   0 runner    (1001) docker     (127)     6495 2023-09-08 12:12:07.000000 clinvar-this-0.9.0/docs/getting_started.rst
+-rw-r--r--   0 runner    (1001) docker     (127)       31 2023-09-08 12:12:07.000000 clinvar-this-0.9.0/docs/history.rst
+-rw-r--r--   0 runner    (1001) docker     (127)     1138 2023-09-08 12:12:07.000000 clinvar-this-0.9.0/docs/index.rst
+-rw-r--r--   0 runner    (1001) docker     (127)     1334 2023-09-08 12:12:07.000000 clinvar-this-0.9.0/docs/installation.rst
+-rw-r--r--   0 runner    (1001) docker     (127)     3723 2023-09-08 12:12:07.000000 clinvar-this-0.9.0/docs/limitations.rst
+-rw-r--r--   0 runner    (1001) docker     (127)      810 2023-09-08 12:12:07.000000 clinvar-this-0.9.0/docs/make.bat
+-rw-r--r--   0 runner    (1001) docker     (127)     8337 2023-09-08 12:12:07.000000 clinvar-this-0.9.0/docs/usage_cli.rst
+-rw-r--r--   0 runner    (1001) docker     (127)      212 2023-09-08 12:12:07.000000 clinvar-this-0.9.0/docs/usage_library.rst
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-09-08 12:12:14.752389 clinvar-this-0.9.0/requirements/
+-rw-r--r--   0 runner    (1001) docker     (127)      244 2023-09-08 12:12:07.000000 clinvar-this-0.9.0/requirements/base.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       12 2023-09-08 12:12:07.000000 clinvar-this-0.9.0/requirements/dev.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      436 2023-09-08 12:12:07.000000 clinvar-this-0.9.0/requirements/test.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      405 2023-09-08 12:12:14.756389 clinvar-this-0.9.0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)     2473 2023-09-08 12:12:07.000000 clinvar-this-0.9.0/setup.py
```

### Comparing `clinvar-this-0.8.0/CHANGELOG.md` & `clinvar-this-0.9.0/CHANGELOG.md`

 * *Files 1% similar despite different names*

```diff
@@ -1,9 +1,21 @@
 # Changelog
 
+## [0.9.0](https://www.github.com/bihealth/clinvar-this/compare/v0.8.0...v0.9.0) (2023-09-08)
+
+
+### Features
+
+* write assessment to extract variants ([#128](https://www.github.com/bihealth/clinvar-this/issues/128)) ([dd72c90](https://www.github.com/bihealth/clinvar-this/commit/dd72c90a68f0e2cbd0306301de77985c0acb521e))
+
+
+### Bug Fixes
+
+* normalizing molecular consequence ([#126](https://www.github.com/bihealth/clinvar-this/issues/126)) ([c2a72cf](https://www.github.com/bihealth/clinvar-this/commit/c2a72cfcaea94752fdb8e278bc0a6d48748650a6))
+
 ## [0.8.0](https://www.github.com/bihealth/clinvar-this/compare/v0.7.0...v0.8.0) (2023-09-08)
 
 
 ### Features
 
 * variant extraction ([#124](https://www.github.com/bihealth/clinvar-this/issues/124)) ([c7bb7c9](https://www.github.com/bihealth/clinvar-this/commit/c7bb7c9a2376d37b512b494631cf62dfcc23b19b))
```

### Comparing `clinvar-this-0.8.0/CONTRIBUTING.rst` & `clinvar-this-0.9.0/CONTRIBUTING.rst`

 * *Files identical despite different names*

### Comparing `clinvar-this-0.8.0/LICENSE` & `clinvar-this-0.9.0/LICENSE`

 * *Files identical despite different names*

### Comparing `clinvar-this-0.8.0/PKG-INFO` & `clinvar-this-0.9.0/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: clinvar-this
-Version: 0.8.0
+Version: 0.9.0
 Summary: ClinVar Submission via API Made Easy
 Home-page: https://github.com/bihealth/clinvar-this
 Author: Manuel Holtgrewe
 Author-email: manuel.holtgrewe@bih-charite.de
 License: MIT license
 Keywords: clinvar
 Classifier: Development Status :: 2 - Pre-Alpha
@@ -49,14 +49,26 @@
 A good place to start is:
 
 - ["Getting Started" in the documentation](https://clinvar-this.readthedocs.io/en/latest/getting_started.html)
 
 
 # Changelog
 
+## [0.9.0](https://www.github.com/bihealth/clinvar-this/compare/v0.8.0...v0.9.0) (2023-09-08)
+
+
+### Features
+
+* write assessment to extract variants ([#128](https://www.github.com/bihealth/clinvar-this/issues/128)) ([dd72c90](https://www.github.com/bihealth/clinvar-this/commit/dd72c90a68f0e2cbd0306301de77985c0acb521e))
+
+
+### Bug Fixes
+
+* normalizing molecular consequence ([#126](https://www.github.com/bihealth/clinvar-this/issues/126)) ([c2a72cf](https://www.github.com/bihealth/clinvar-this/commit/c2a72cfcaea94752fdb8e278bc0a6d48748650a6))
+
 ## [0.8.0](https://www.github.com/bihealth/clinvar-this/compare/v0.7.0...v0.8.0) (2023-09-08)
 
 
 ### Features
 
 * variant extraction ([#124](https://www.github.com/bihealth/clinvar-this/issues/124)) ([c7bb7c9](https://www.github.com/bihealth/clinvar-this/commit/c7bb7c9a2376d37b512b494631cf62dfcc23b19b))
```

### Comparing `clinvar-this-0.8.0/README.md` & `clinvar-this-0.9.0/README.md`

 * *Files identical despite different names*

### Comparing `clinvar-this-0.8.0/clinvar_api/client.py` & `clinvar-this-0.9.0/clinvar_api/client.py`

 * *Files identical despite different names*

### Comparing `clinvar-this-0.8.0/clinvar_api/common.py` & `clinvar-this-0.9.0/clinvar_api/common.py`

 * *Files identical despite different names*

### Comparing `clinvar-this-0.8.0/clinvar_api/models/query_response.py` & `clinvar-this-0.9.0/clinvar_api/models/query_response.py`

 * *Files identical despite different names*

### Comparing `clinvar-this-0.8.0/clinvar_api/models/sub_payload.py` & `clinvar-this-0.9.0/clinvar_api/models/sub_payload.py`

 * *Files identical despite different names*

### Comparing `clinvar-this-0.8.0/clinvar_api/models/sub_response.py` & `clinvar-this-0.9.0/clinvar_api/models/sub_response.py`

 * *Files identical despite different names*

### Comparing `clinvar-this-0.8.0/clinvar_api/msg/query_response.py` & `clinvar-this-0.9.0/clinvar_api/msg/query_response.py`

 * *Files identical despite different names*

### Comparing `clinvar-this-0.8.0/clinvar_api/msg/sub_payload.py` & `clinvar-this-0.9.0/clinvar_api/msg/sub_payload.py`

 * *Files identical despite different names*

### Comparing `clinvar-this-0.8.0/clinvar_api/msg/sub_response.py` & `clinvar-this-0.9.0/clinvar_api/msg/sub_response.py`

 * *Files identical despite different names*

### Comparing `clinvar-this-0.8.0/clinvar_api/schemas/__init__.py` & `clinvar-this-0.9.0/clinvar_api/schemas/__init__.py`

 * *Files identical despite different names*

### Comparing `clinvar-this-0.8.0/clinvar_data/class_by_freq.py` & `clinvar-this-0.9.0/clinvar_data/class_by_freq.py`

 * *Files identical despite different names*

### Comparing `clinvar-this-0.8.0/clinvar_data/conversion.py` & `clinvar-this-0.9.0/clinvar_data/conversion.py`

 * *Files identical despite different names*

### Comparing `clinvar-this-0.8.0/clinvar_data/extract_vars.py` & `clinvar-this-0.9.0/clinvar_data/extract_vars.py`

 * *Files 22% similar despite different names*

```diff
@@ -5,27 +5,26 @@
 import gzip
 import json
 import os
 import typing
 
 import attrs
 import cattrs
-from logzero import logger
 import tqdm
 
 from clinvar_data import models
 from clinvar_data.cattrs_helpers import CONVERTER
 from clinvar_data.models import MeasureAttributeType
 
 
 class OutputFilesHandler:
     def __init__(self, output_dir: str, gzip_output: bool):
         self.output_dir = output_dir
         self.gzip_output = gzip_output
-        self.suffix = "tsv.gz" if self.gzip_output else "tsv"
+        self.suffix = "jsonl.gz" if self.gzip_output else "jsonl"
         self.files: typing.Dict[typing.Tuple[str, str], typing.TextIO] = {}
 
     def get_file(self, stack: contextlib.ExitStack, assembly: str, variant_size: str):
         key = (assembly, variant_size)
         if key not in self.files:
             file_path = os.path.join(
                 self.output_dir, f"clinvar-variants-{assembly}-{variant_size}.{self.suffix}"
@@ -71,14 +70,16 @@
         return mapping.get(mt, VariantType.OTHER)
 
 
 @attrs.frozen(auto_attribs=True)
 class VariantRecord:
     rcv: str
     variant_type: VariantType
+    clinical_significance: typing.Optional[models.ClinicalSignificanceDescription]
+    review_status: typing.Optional[models.ReviewStatus]
     sequence_location: models.SequenceLocation
     absolute_copy_number: typing.Union[None, str, int, float] = None
     reference_copy_number: typing.Union[None, str, int, float] = None
     copy_number_tuple: typing.Union[None, str, int, float] = None
 
 
 def run(path_input: str, output_dir: str, gzip_output: bool):
@@ -95,15 +96,14 @@
         for line in tqdm.tqdm(inputf, desc="processing", unit=" JSONL records"):
             dict_value = json.loads(line)
             clinvar_set = CONVERTER.structure(dict_value, models.ClinVarSet)
             rca = clinvar_set.reference_clinvar_assertion
 
             if rca.measures:
                 for measure in rca.measures.measures or []:
-                    # print(measure.sequence_locations)
                     if not measure.sequence_locations:
                         continue
 
                     absolute_copy_number = None
                     reference_copy_number = None
                     copy_number_tuple = None
                     for attribute in measure.attributes or []:
@@ -111,19 +111,27 @@
                         if attribute.type == MeasureAttributeType.ABSOLUTE_COPY_NUMBER:
                             absolute_copy_number = value
                         elif attribute.type == MeasureAttributeType.REFERENCE_COPY_NUMBER:
                             reference_copy_number = value
                         elif attribute.type == MeasureAttributeType.COPY_NUMBER_TUPLE:
                             copy_number_tuple = value
 
+                    if rca.clinical_significance and rca.clinical_significance.description:
+                        clinical_significance = rca.clinical_significance.description
+                        review_status = rca.clinical_significance.review_status
+                    else:
+                        clinical_significance = None
+                        review_status = None
+
                     # The structural variants that we saw had the sequence location directly on the measure.
                     for sequence_location in measure.sequence_locations:
-                        logger.info("%s", sequence_location)
                         record = VariantRecord(
                             rcv=rca.clinvar_accession.acc,
+                            clinical_significance=clinical_significance,
+                            review_status=review_status,
                             variant_type=VariantType.from_measure_type(measure.type),
                             sequence_location=sequence_location,
                             absolute_copy_number=absolute_copy_number,
                             reference_copy_number=reference_copy_number,
                             copy_number_tuple=copy_number_tuple,
                         )
                         if record.variant_type == VariantType.OTHER:
```

### Comparing `clinvar-this-0.8.0/clinvar_data/gene_impact.py` & `clinvar-this-0.9.0/clinvar_data/gene_impact.py`

 * *Files 2% similar despite different names*

```diff
@@ -32,27 +32,27 @@
     STOP_LOST = "stop_lost"
     SYNONYMOUS_VARIANT = "synonymous_variant"
     UPSTREAM_TRANSCRIPT_VARIANT = "upstream_gene_variant"
 
 
 #: Mapping from strings used in ClinVar XML to ``IMPACT``.
 GENE_IMPACT_MAP = {
-    "3 prime UTR variant": Impact.THREE_PRIME_UTR_VARIANT,
-    "5 prime UTR variant": Impact.FIVE_PRIME_UTR_VARIANT,
+    "3 prime utr variant": Impact.THREE_PRIME_UTR_VARIANT,
+    "5 prime utr variant": Impact.FIVE_PRIME_UTR_VARIANT,
     "downstream transcript variant": Impact.DOWNSTREAM_TRANSCRIPT_VARIANT,
     "frameshift variant": Impact.FRAMESHIFT_VARIANT,
     "genic downstream transcript variant": Impact.DOWNSTREAM_TRANSCRIPT_VARIANT,
     "genic upstream transcript variant": Impact.UPSTREAM_TRANSCRIPT_VARIANT,
-    "inframe_deletion": Impact.INFRAME_INDEL,
-    "inframe_indel": Impact.INFRAME_INDEL,
-    "inframe_insertion": Impact.INFRAME_INDEL,
+    "inframe deletion": Impact.INFRAME_INDEL,
+    "inframe indel": Impact.INFRAME_INDEL,
+    "inframe insertion": Impact.INFRAME_INDEL,
     "initiatior codon variant": Impact.START_LOST,
     "intron variant": Impact.INTRON_VARIANT,
     "missense variant": Impact.MISSENSE_VARIANT,
-    "non-coding transcript variant": Impact.NON_CODING_TRANSCRIPT_VARIANT,
+    "non coding transcript variant": Impact.NON_CODING_TRANSCRIPT_VARIANT,
     "nonsense": Impact.STOP_GAINED,
     "no sequence alteration": Impact.NO_SEQUENCE_ALTERATION,
     "splice acceptor variant": Impact.SPLICE_ACCEPTOR_VARIANT,
     "splice donor variant": Impact.SPLICE_DONOR_VARIANT,
     "stop lost": Impact.STOP_LOST,
     "synonymous variant": Impact.SYNONYMOUS_VARIANT,
     "upstream transcript variant": Impact.UPSTREAM_TRANSCRIPT_VARIANT,
@@ -122,17 +122,19 @@
             for measure in clinvar_set.reference_clinvar_assertion.measures.measures:
                 for attribute in measure.attributes:
                     if attribute.type == models.MeasureAttributeType.MOLECULAR_CONSEQUENCE:
                         csq = attribute.value
                         break
             if not csq:
                 continue  # skip, no molecular consequence
-            elif csq not in GENE_IMPACT_MAP:
-                print(f"WARNING: unknown molecular consequence {csq}", file=sys.stderr)
-                continue
+            else:
+                csq = csq.lower().replace("_", " ").replace("-", " ")
+                if csq not in GENE_IMPACT_MAP:
+                    print(f"WARNING: unknown molecular consequence {csq}", file=sys.stderr)
+                    continue
 
             hgnc = None
             for measure in clinvar_set.reference_clinvar_assertion.measures.measures:
                 for measure_relationship in measure.measure_relationship:
                     for xref in measure_relationship.xrefs:
                         if xref.db == "HGNC":
                             hgnc = xref.id
```

### Comparing `clinvar-this-0.8.0/clinvar_data/models.py` & `clinvar-this-0.9.0/clinvar_data/models.py`

 * *Files identical despite different names*

### Comparing `clinvar-this-0.8.0/clinvar_data/phenotype_link.py` & `clinvar-this-0.9.0/clinvar_data/phenotype_link.py`

 * *Files identical despite different names*

### Comparing `clinvar-this-0.8.0/clinvar_this/batches.py` & `clinvar-this-0.9.0/clinvar_this/batches.py`

 * *Files identical despite different names*

### Comparing `clinvar-this-0.8.0/clinvar_this/cli.py` & `clinvar-this-0.9.0/clinvar_this/cli.py`

 * *Files identical despite different names*

### Comparing `clinvar-this-0.8.0/clinvar_this/config.py` & `clinvar-this-0.9.0/clinvar_this/config.py`

 * *Files identical despite different names*

### Comparing `clinvar-this-0.8.0/clinvar_this/exceptions.py` & `clinvar-this-0.9.0/clinvar_this/exceptions.py`

 * *Files identical despite different names*

### Comparing `clinvar-this-0.8.0/clinvar_this/io/tsv.py` & `clinvar-this-0.9.0/clinvar_this/io/tsv.py`

 * *Files identical despite different names*

### Comparing `clinvar-this-0.8.0/clinvar_this.egg-info/PKG-INFO` & `clinvar-this-0.9.0/clinvar_this.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: clinvar-this
-Version: 0.8.0
+Version: 0.9.0
 Summary: ClinVar Submission via API Made Easy
 Home-page: https://github.com/bihealth/clinvar-this
 Author: Manuel Holtgrewe
 Author-email: manuel.holtgrewe@bih-charite.de
 License: MIT license
 Keywords: clinvar
 Classifier: Development Status :: 2 - Pre-Alpha
@@ -49,14 +49,26 @@
 A good place to start is:
 
 - ["Getting Started" in the documentation](https://clinvar-this.readthedocs.io/en/latest/getting_started.html)
 
 
 # Changelog
 
+## [0.9.0](https://www.github.com/bihealth/clinvar-this/compare/v0.8.0...v0.9.0) (2023-09-08)
+
+
+### Features
+
+* write assessment to extract variants ([#128](https://www.github.com/bihealth/clinvar-this/issues/128)) ([dd72c90](https://www.github.com/bihealth/clinvar-this/commit/dd72c90a68f0e2cbd0306301de77985c0acb521e))
+
+
+### Bug Fixes
+
+* normalizing molecular consequence ([#126](https://www.github.com/bihealth/clinvar-this/issues/126)) ([c2a72cf](https://www.github.com/bihealth/clinvar-this/commit/c2a72cfcaea94752fdb8e278bc0a6d48748650a6))
+
 ## [0.8.0](https://www.github.com/bihealth/clinvar-this/compare/v0.7.0...v0.8.0) (2023-09-08)
 
 
 ### Features
 
 * variant extraction ([#124](https://www.github.com/bihealth/clinvar-this/issues/124)) ([c7bb7c9](https://www.github.com/bihealth/clinvar-this/commit/c7bb7c9a2376d37b512b494631cf62dfcc23b19b))
```

### Comparing `clinvar-this-0.8.0/clinvar_this.egg-info/SOURCES.txt` & `clinvar-this-0.9.0/clinvar_this.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `clinvar-this-0.8.0/docs/Makefile` & `clinvar-this-0.9.0/docs/Makefile`

 * *Files identical despite different names*

### Comparing `clinvar-this-0.8.0/docs/api_vs_cli.rst` & `clinvar-this-0.9.0/docs/api_vs_cli.rst`

 * *Files identical despite different names*

### Comparing `clinvar-this-0.8.0/docs/clinvar_api/clinvar_api.models.rst` & `clinvar-this-0.9.0/docs/clinvar_api/clinvar_api.models.rst`

 * *Files identical despite different names*

### Comparing `clinvar-this-0.8.0/docs/clinvar_api/clinvar_api.msg.rst` & `clinvar-this-0.9.0/docs/clinvar_api/clinvar_api.msg.rst`

 * *Files identical despite different names*

### Comparing `clinvar-this-0.8.0/docs/clinvar_api/clinvar_api.rst` & `clinvar-this-0.9.0/docs/clinvar_api/clinvar_api.rst`

 * *Files identical despite different names*

### Comparing `clinvar-this-0.8.0/docs/clinvar_this/clinvar_this.rst` & `clinvar-this-0.9.0/docs/clinvar_this/clinvar_this.rst`

 * *Files identical despite different names*

### Comparing `clinvar-this-0.8.0/docs/common_errors.rst` & `clinvar-this-0.9.0/docs/common_errors.rst`

 * *Files identical despite different names*

### Comparing `clinvar-this-0.8.0/docs/conf.py` & `clinvar-this-0.9.0/docs/conf.py`

 * *Files identical despite different names*

### Comparing `clinvar-this-0.8.0/docs/figures/clinvar-this-workflow.png` & `clinvar-this-0.9.0/docs/figures/clinvar-this-workflow.png`

 * *Files identical despite different names*

### Comparing `clinvar-this-0.8.0/docs/file_formats.rst` & `clinvar-this-0.9.0/docs/file_formats.rst`

 * *Files identical despite different names*

### Comparing `clinvar-this-0.8.0/docs/getting_started.rst` & `clinvar-this-0.9.0/docs/getting_started.rst`

 * *Files identical despite different names*

### Comparing `clinvar-this-0.8.0/docs/index.rst` & `clinvar-this-0.9.0/docs/index.rst`

 * *Files identical despite different names*

### Comparing `clinvar-this-0.8.0/docs/installation.rst` & `clinvar-this-0.9.0/docs/installation.rst`

 * *Files identical despite different names*

### Comparing `clinvar-this-0.8.0/docs/limitations.rst` & `clinvar-this-0.9.0/docs/limitations.rst`

 * *Files identical despite different names*

### Comparing `clinvar-this-0.8.0/docs/make.bat` & `clinvar-this-0.9.0/docs/make.bat`

 * *Files identical despite different names*

### Comparing `clinvar-this-0.8.0/docs/usage_cli.rst` & `clinvar-this-0.9.0/docs/usage_cli.rst`

 * *Files identical despite different names*

### Comparing `clinvar-this-0.8.0/setup.py` & `clinvar-this-0.9.0/setup.py`

 * *Files identical despite different names*

