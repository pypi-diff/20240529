# Comparing `tmp/oarepo-model-builder-drafts-files-4.0.8.tar.gz` & `tmp/oarepo-model-builder-drafts-files-4.0.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "oarepo-model-builder-drafts-files-4.0.8.tar", last modified: Tue Feb 20 15:28:47 2024, max compression
+gzip compressed data, was "oarepo-model-builder-drafts-files-4.0.9.tar", last modified: Sun Mar 10 21:53:42 2024, max compression
```

## Comparing `oarepo-model-builder-drafts-files-4.0.8.tar` & `oarepo-model-builder-drafts-files-4.0.9.tar`

### file list

```diff
@@ -1,55 +1,58 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-20 15:28:47.231244 oarepo-model-builder-drafts-files-4.0.8/
--rw-r--r--   0 runner    (1001) docker     (127)      812 2024-02-20 15:28:47.231244 oarepo-model-builder-drafts-files-4.0.8/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      503 2024-02-20 15:25:22.000000 oarepo-model-builder-drafts-files-4.0.8/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-20 15:28:47.223244 oarepo-model-builder-drafts-files-4.0.8/oarepo_model_builder_drafts_files/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-02-20 15:25:22.000000 oarepo-model-builder-drafts-files-4.0.8/oarepo_model_builder_drafts_files/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-20 15:28:47.223244 oarepo-model-builder-drafts-files-4.0.8/oarepo_model_builder_drafts_files/builders/
--rw-r--r--   0 runner    (1001) docker     (127)      106 2024-02-20 15:25:22.000000 oarepo-model-builder-drafts-files-4.0.8/oarepo_model_builder_drafts_files/builders/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      290 2024-02-20 15:25:22.000000 oarepo-model-builder-drafts-files-4.0.8/oarepo_model_builder_drafts_files/builders/files_service_config_disable_upload.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-20 15:28:47.227244 oarepo-model-builder-drafts-files-4.0.8/oarepo_model_builder_drafts_files/builders/templates/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-02-20 15:25:22.000000 oarepo-model-builder-drafts-files-4.0.8/oarepo_model_builder_drafts_files/builders/templates/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)       70 2024-02-20 15:25:22.000000 oarepo-model-builder-drafts-files-4.0.8/oarepo_model_builder_drafts_files/builders/templates/service_config_disable_upload.py.jinja2
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-20 15:28:47.227244 oarepo-model-builder-drafts-files-4.0.8/oarepo_model_builder_drafts_files/builders/tests/
--rw-r--r--   0 runner    (1001) docker     (127)      238 2024-02-20 15:25:22.000000 oarepo-model-builder-drafts-files-4.0.8/oarepo_model_builder_drafts_files/builders/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      608 2024-02-20 15:25:22.000000 oarepo-model-builder-drafts-files-4.0.8/oarepo_model_builder_drafts_files/builders/tests/conftest.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-20 15:28:47.227244 oarepo-model-builder-drafts-files-4.0.8/oarepo_model_builder_drafts_files/builders/tests/templates/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-02-20 15:25:22.000000 oarepo-model-builder-drafts-files-4.0.8/oarepo_model_builder_drafts_files/builders/tests/templates/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      198 2024-02-20 15:25:22.000000 oarepo-model-builder-drafts-files-4.0.8/oarepo_model_builder_drafts_files/builders/tests/templates/conftest.py.jinja2
--rw-r--r--   0 runner    (1001) docker     (127)    10148 2024-02-20 15:25:22.000000 oarepo-model-builder-drafts-files-4.0.8/oarepo_model_builder_drafts_files/builders/tests/templates/test_files_resource.py.jinja2
--rw-r--r--   0 runner    (1001) docker     (127)      126 2024-02-20 15:25:22.000000 oarepo-model-builder-drafts-files-4.0.8/oarepo_model_builder_drafts_files/builders/tests/templates/test_resource_input_data.py.jinja2
--rw-r--r--   0 runner    (1001) docker     (127)      652 2024-02-20 15:25:22.000000 oarepo-model-builder-drafts-files-4.0.8/oarepo_model_builder_drafts_files/builders/tests/test_resource.py
--rw-r--r--   0 runner    (1001) docker     (127)      352 2024-02-20 15:25:22.000000 oarepo-model-builder-drafts-files-4.0.8/oarepo_model_builder_drafts_files/builders/tests/test_resource_input_data.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-20 15:28:47.227244 oarepo-model-builder-drafts-files-4.0.8/oarepo_model_builder_drafts_files/datatypes/
--rw-r--r--   0 runner    (1001) docker     (127)       86 2024-02-20 15:25:22.000000 oarepo-model-builder-drafts-files-4.0.8/oarepo_model_builder_drafts_files/datatypes/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-20 15:28:47.227244 oarepo-model-builder-drafts-files-4.0.8/oarepo_model_builder_drafts_files/datatypes/components/
--rw-r--r--   0 runner    (1001) docker     (127)     1255 2024-02-20 15:25:22.000000 oarepo-model-builder-drafts-files-4.0.8/oarepo_model_builder_drafts_files/datatypes/components/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-20 15:28:47.231244 oarepo-model-builder-drafts-files-4.0.8/oarepo_model_builder_drafts_files/datatypes/components/draft_file_model/
--rw-r--r--   0 runner    (1001) docker     (127)     1068 2024-02-20 15:25:22.000000 oarepo-model-builder-drafts-files-4.0.8/oarepo_model_builder_drafts_files/datatypes/components/draft_file_model/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1089 2024-02-20 15:25:22.000000 oarepo-model-builder-drafts-files-4.0.8/oarepo_model_builder_drafts_files/datatypes/components/draft_file_model/blueprints.py
--rw-r--r--   0 runner    (1001) docker     (127)     1137 2024-02-20 15:25:22.000000 oarepo-model-builder-drafts-files-4.0.8/oarepo_model_builder_drafts_files/datatypes/components/draft_file_model/defaults.py
--rw-r--r--   0 runner    (1001) docker     (127)     1246 2024-02-20 15:25:22.000000 oarepo-model-builder-drafts-files-4.0.8/oarepo_model_builder_drafts_files/datatypes/components/draft_file_model/ext_resource.py
--rw-r--r--   0 runner    (1001) docker     (127)     1511 2024-02-20 15:25:22.000000 oarepo-model-builder-drafts-files-4.0.8/oarepo_model_builder_drafts_files/datatypes/components/draft_file_model/files_field.py
--rw-r--r--   0 runner    (1001) docker     (127)      800 2024-02-20 15:25:22.000000 oarepo-model-builder-drafts-files-4.0.8/oarepo_model_builder_drafts_files/datatypes/components/draft_file_model/marshmallow.py
--rw-r--r--   0 runner    (1001) docker     (127)     1142 2024-02-20 15:25:22.000000 oarepo-model-builder-drafts-files-4.0.8/oarepo_model_builder_drafts_files/datatypes/components/draft_file_model/parent_record.py
--rw-r--r--   0 runner    (1001) docker     (127)      811 2024-02-20 15:25:22.000000 oarepo-model-builder-drafts-files-4.0.8/oarepo_model_builder_drafts_files/datatypes/components/draft_file_model/pid.py
--rw-r--r--   0 runner    (1001) docker     (127)     1012 2024-02-20 15:25:22.000000 oarepo-model-builder-drafts-files-4.0.8/oarepo_model_builder_drafts_files/datatypes/components/draft_file_model/record.py
--rw-r--r--   0 runner    (1001) docker     (127)     1013 2024-02-20 15:25:22.000000 oarepo-model-builder-drafts-files-4.0.8/oarepo_model_builder_drafts_files/datatypes/components/draft_file_model/record_metadata.py
--rw-r--r--   0 runner    (1001) docker     (127)      974 2024-02-20 15:25:22.000000 oarepo-model-builder-drafts-files-4.0.8/oarepo_model_builder_drafts_files/datatypes/components/draft_file_model/resource.py
--rw-r--r--   0 runner    (1001) docker     (127)      540 2024-02-20 15:25:22.000000 oarepo-model-builder-drafts-files-4.0.8/oarepo_model_builder_drafts_files/datatypes/components/draft_file_model/service.py
--rw-r--r--   0 runner    (1001) docker     (127)     5372 2024-02-20 15:25:22.000000 oarepo-model-builder-drafts-files-4.0.8/oarepo_model_builder_drafts_files/datatypes/components/draft_file_profile.py
--rw-r--r--   0 runner    (1001) docker     (127)     2459 2024-02-20 15:25:22.000000 oarepo-model-builder-drafts-files-4.0.8/oarepo_model_builder_drafts_files/datatypes/components/draft_files_tests.py
--rw-r--r--   0 runner    (1001) docker     (127)     1058 2024-02-20 15:25:22.000000 oarepo-model-builder-drafts-files-4.0.8/oarepo_model_builder_drafts_files/datatypes/components/drafts_files_record.py
--rw-r--r--   0 runner    (1001) docker     (127)      534 2024-02-20 15:25:22.000000 oarepo-model-builder-drafts-files-4.0.8/oarepo_model_builder_drafts_files/datatypes/draft_file.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-20 15:28:47.231244 oarepo-model-builder-drafts-files-4.0.8/oarepo_model_builder_drafts_files/profiles/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-02-20 15:25:22.000000 oarepo-model-builder-drafts-files-4.0.8/oarepo_model_builder_drafts_files/profiles/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2442 2024-02-20 15:25:22.000000 oarepo-model-builder-drafts-files-4.0.8/oarepo_model_builder_drafts_files/profiles/draft_files.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-20 15:28:47.231244 oarepo-model-builder-drafts-files-4.0.8/oarepo_model_builder_drafts_files.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)      812 2024-02-20 15:28:47.000000 oarepo-model-builder-drafts-files-4.0.8/oarepo_model_builder_drafts_files.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     2874 2024-02-20 15:28:47.000000 oarepo-model-builder-drafts-files-4.0.8/oarepo_model_builder_drafts_files.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-02-20 15:28:47.000000 oarepo-model-builder-drafts-files-4.0.8/oarepo_model_builder_drafts_files.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)     1870 2024-02-20 15:28:47.000000 oarepo-model-builder-drafts-files-4.0.8/oarepo_model_builder_drafts_files.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (127)      131 2024-02-20 15:28:47.000000 oarepo-model-builder-drafts-files-4.0.8/oarepo_model_builder_drafts_files.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       34 2024-02-20 15:28:47.000000 oarepo-model-builder-drafts-files-4.0.8/oarepo_model_builder_drafts_files.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)      102 2024-02-20 15:25:22.000000 oarepo-model-builder-drafts-files-4.0.8/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)     2421 2024-02-20 15:28:47.231244 oarepo-model-builder-drafts-files-4.0.8/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-02-20 15:25:22.000000 oarepo-model-builder-drafts-files-4.0.8/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-10 21:53:42.088071 oarepo-model-builder-drafts-files-4.0.9/
+-rw-r--r--   0 runner    (1001) docker     (127)      812 2024-03-10 21:53:42.088071 oarepo-model-builder-drafts-files-4.0.9/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      503 2024-03-10 21:50:20.000000 oarepo-model-builder-drafts-files-4.0.9/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-10 21:53:42.080072 oarepo-model-builder-drafts-files-4.0.9/oarepo_model_builder_drafts_files/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-03-10 21:50:20.000000 oarepo-model-builder-drafts-files-4.0.9/oarepo_model_builder_drafts_files/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-10 21:53:42.084071 oarepo-model-builder-drafts-files-4.0.9/oarepo_model_builder_drafts_files/builders/
+-rw-r--r--   0 runner    (1001) docker     (127)      194 2024-03-10 21:50:20.000000 oarepo-model-builder-drafts-files-4.0.9/oarepo_model_builder_drafts_files/builders/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      290 2024-03-10 21:50:20.000000 oarepo-model-builder-drafts-files-4.0.9/oarepo_model_builder_drafts_files/builders/files_service_config_disable_upload.py
+-rw-r--r--   0 runner    (1001) docker     (127)      280 2024-03-10 21:50:20.000000 oarepo-model-builder-drafts-files-4.0.9/oarepo_model_builder_drafts_files/builders/published_service_files_link.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-10 21:53:42.084071 oarepo-model-builder-drafts-files-4.0.9/oarepo_model_builder_drafts_files/builders/templates/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-03-10 21:50:20.000000 oarepo-model-builder-drafts-files-4.0.9/oarepo_model_builder_drafts_files/builders/templates/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      259 2024-03-10 21:50:20.000000 oarepo-model-builder-drafts-files-4.0.9/oarepo_model_builder_drafts_files/builders/templates/published_service_files_link.py.jinja2
+-rw-r--r--   0 runner    (1001) docker     (127)       70 2024-03-10 21:50:20.000000 oarepo-model-builder-drafts-files-4.0.9/oarepo_model_builder_drafts_files/builders/templates/service_config_disable_upload.py.jinja2
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-10 21:53:42.084071 oarepo-model-builder-drafts-files-4.0.9/oarepo_model_builder_drafts_files/builders/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)      238 2024-03-10 21:50:20.000000 oarepo-model-builder-drafts-files-4.0.9/oarepo_model_builder_drafts_files/builders/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      608 2024-03-10 21:50:20.000000 oarepo-model-builder-drafts-files-4.0.9/oarepo_model_builder_drafts_files/builders/tests/conftest.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-10 21:53:42.084071 oarepo-model-builder-drafts-files-4.0.9/oarepo_model_builder_drafts_files/builders/tests/templates/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-03-10 21:50:20.000000 oarepo-model-builder-drafts-files-4.0.9/oarepo_model_builder_drafts_files/builders/tests/templates/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      198 2024-03-10 21:50:20.000000 oarepo-model-builder-drafts-files-4.0.9/oarepo_model_builder_drafts_files/builders/tests/templates/conftest.py.jinja2
+-rw-r--r--   0 runner    (1001) docker     (127)    10148 2024-03-10 21:50:20.000000 oarepo-model-builder-drafts-files-4.0.9/oarepo_model_builder_drafts_files/builders/tests/templates/test_files_resource.py.jinja2
+-rw-r--r--   0 runner    (1001) docker     (127)      126 2024-03-10 21:50:20.000000 oarepo-model-builder-drafts-files-4.0.9/oarepo_model_builder_drafts_files/builders/tests/templates/test_resource_input_data.py.jinja2
+-rw-r--r--   0 runner    (1001) docker     (127)      652 2024-03-10 21:50:20.000000 oarepo-model-builder-drafts-files-4.0.9/oarepo_model_builder_drafts_files/builders/tests/test_resource.py
+-rw-r--r--   0 runner    (1001) docker     (127)      352 2024-03-10 21:50:20.000000 oarepo-model-builder-drafts-files-4.0.9/oarepo_model_builder_drafts_files/builders/tests/test_resource_input_data.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-10 21:53:42.084071 oarepo-model-builder-drafts-files-4.0.9/oarepo_model_builder_drafts_files/datatypes/
+-rw-r--r--   0 runner    (1001) docker     (127)       86 2024-03-10 21:50:20.000000 oarepo-model-builder-drafts-files-4.0.9/oarepo_model_builder_drafts_files/datatypes/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-10 21:53:42.088071 oarepo-model-builder-drafts-files-4.0.9/oarepo_model_builder_drafts_files/datatypes/components/
+-rw-r--r--   0 runner    (1001) docker     (127)     1444 2024-03-10 21:50:20.000000 oarepo-model-builder-drafts-files-4.0.9/oarepo_model_builder_drafts_files/datatypes/components/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-10 21:53:42.088071 oarepo-model-builder-drafts-files-4.0.9/oarepo_model_builder_drafts_files/datatypes/components/draft_file_model/
+-rw-r--r--   0 runner    (1001) docker     (127)     1068 2024-03-10 21:50:20.000000 oarepo-model-builder-drafts-files-4.0.9/oarepo_model_builder_drafts_files/datatypes/components/draft_file_model/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1089 2024-03-10 21:50:20.000000 oarepo-model-builder-drafts-files-4.0.9/oarepo_model_builder_drafts_files/datatypes/components/draft_file_model/blueprints.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1137 2024-03-10 21:50:20.000000 oarepo-model-builder-drafts-files-4.0.9/oarepo_model_builder_drafts_files/datatypes/components/draft_file_model/defaults.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1246 2024-03-10 21:50:20.000000 oarepo-model-builder-drafts-files-4.0.9/oarepo_model_builder_drafts_files/datatypes/components/draft_file_model/ext_resource.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1450 2024-03-10 21:50:20.000000 oarepo-model-builder-drafts-files-4.0.9/oarepo_model_builder_drafts_files/datatypes/components/draft_file_model/files_field.py
+-rw-r--r--   0 runner    (1001) docker     (127)      800 2024-03-10 21:50:20.000000 oarepo-model-builder-drafts-files-4.0.9/oarepo_model_builder_drafts_files/datatypes/components/draft_file_model/marshmallow.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1142 2024-03-10 21:50:20.000000 oarepo-model-builder-drafts-files-4.0.9/oarepo_model_builder_drafts_files/datatypes/components/draft_file_model/parent_record.py
+-rw-r--r--   0 runner    (1001) docker     (127)      811 2024-03-10 21:50:20.000000 oarepo-model-builder-drafts-files-4.0.9/oarepo_model_builder_drafts_files/datatypes/components/draft_file_model/pid.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1012 2024-03-10 21:50:20.000000 oarepo-model-builder-drafts-files-4.0.9/oarepo_model_builder_drafts_files/datatypes/components/draft_file_model/record.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1013 2024-03-10 21:50:20.000000 oarepo-model-builder-drafts-files-4.0.9/oarepo_model_builder_drafts_files/datatypes/components/draft_file_model/record_metadata.py
+-rw-r--r--   0 runner    (1001) docker     (127)      974 2024-03-10 21:50:20.000000 oarepo-model-builder-drafts-files-4.0.9/oarepo_model_builder_drafts_files/datatypes/components/draft_file_model/resource.py
+-rw-r--r--   0 runner    (1001) docker     (127)      540 2024-03-10 21:50:20.000000 oarepo-model-builder-drafts-files-4.0.9/oarepo_model_builder_drafts_files/datatypes/components/draft_file_model/service.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5375 2024-03-10 21:50:20.000000 oarepo-model-builder-drafts-files-4.0.9/oarepo_model_builder_drafts_files/datatypes/components/draft_file_profile.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2459 2024-03-10 21:50:20.000000 oarepo-model-builder-drafts-files-4.0.9/oarepo_model_builder_drafts_files/datatypes/components/draft_files_tests.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1046 2024-03-10 21:50:20.000000 oarepo-model-builder-drafts-files-4.0.9/oarepo_model_builder_drafts_files/datatypes/components/drafts_files_record.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1786 2024-03-10 21:50:20.000000 oarepo-model-builder-drafts-files-4.0.9/oarepo_model_builder_drafts_files/datatypes/components/published_service.py
+-rw-r--r--   0 runner    (1001) docker     (127)      534 2024-03-10 21:50:20.000000 oarepo-model-builder-drafts-files-4.0.9/oarepo_model_builder_drafts_files/datatypes/draft_file.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-10 21:53:42.088071 oarepo-model-builder-drafts-files-4.0.9/oarepo_model_builder_drafts_files/profiles/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-03-10 21:50:20.000000 oarepo-model-builder-drafts-files-4.0.9/oarepo_model_builder_drafts_files/profiles/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2442 2024-03-10 21:50:20.000000 oarepo-model-builder-drafts-files-4.0.9/oarepo_model_builder_drafts_files/profiles/draft_files.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-10 21:53:42.088071 oarepo-model-builder-drafts-files-4.0.9/oarepo_model_builder_drafts_files.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)      812 2024-03-10 21:53:42.000000 oarepo-model-builder-drafts-files-4.0.9/oarepo_model_builder_drafts_files.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     3117 2024-03-10 21:53:42.000000 oarepo-model-builder-drafts-files-4.0.9/oarepo_model_builder_drafts_files.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-03-10 21:53:42.000000 oarepo-model-builder-drafts-files-4.0.9/oarepo_model_builder_drafts_files.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)     2948 2024-03-10 21:53:42.000000 oarepo-model-builder-drafts-files-4.0.9/oarepo_model_builder_drafts_files.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      131 2024-03-10 21:53:42.000000 oarepo-model-builder-drafts-files-4.0.9/oarepo_model_builder_drafts_files.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       34 2024-03-10 21:53:42.000000 oarepo-model-builder-drafts-files-4.0.9/oarepo_model_builder_drafts_files.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      102 2024-03-10 21:50:20.000000 oarepo-model-builder-drafts-files-4.0.9/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)     3508 2024-03-10 21:53:42.092071 oarepo-model-builder-drafts-files-4.0.9/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-03-10 21:50:20.000000 oarepo-model-builder-drafts-files-4.0.9/setup.py
```

### Comparing `oarepo-model-builder-drafts-files-4.0.8/PKG-INFO` & `oarepo-model-builder-drafts-files-4.0.9/PKG-INFO`

 * *Files 11% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: oarepo-model-builder-drafts-files
-Version: 4.0.8
+Version: 4.0.9
 Description-Content-Type: text/markdown
 Requires-Dist: oarepo-model-builder-tests>=4.0.0
 Requires-Dist: oarepo-model-builder>=4.0.0
 Requires-Dist: oarepo-model-builder-files>=4.0.0
 Requires-Dist: oarepo-model-builder-drafts>=1.0.4
 
 # OARepo model builder drafts files
```

### Comparing `oarepo-model-builder-drafts-files-4.0.8/oarepo_model_builder_drafts_files/builders/tests/conftest.py` & `oarepo-model-builder-drafts-files-4.0.9/oarepo_model_builder_drafts_files/builders/tests/conftest.py`

 * *Files identical despite different names*

### Comparing `oarepo-model-builder-drafts-files-4.0.8/oarepo_model_builder_drafts_files/builders/tests/templates/test_files_resource.py.jinja2` & `oarepo-model-builder-drafts-files-4.0.9/oarepo_model_builder_drafts_files/builders/tests/templates/test_files_resource.py.jinja2`

 * *Files identical despite different names*

### Comparing `oarepo-model-builder-drafts-files-4.0.8/oarepo_model_builder_drafts_files/builders/tests/test_resource.py` & `oarepo-model-builder-drafts-files-4.0.9/oarepo_model_builder_drafts_files/builders/tests/test_resource.py`

 * *Files identical despite different names*

### Comparing `oarepo-model-builder-drafts-files-4.0.8/oarepo_model_builder_drafts_files/datatypes/components/draft_file_model/__init__.py` & `oarepo-model-builder-drafts-files-4.0.9/oarepo_model_builder_drafts_files/datatypes/components/draft_file_model/__init__.py`

 * *Files identical despite different names*

### Comparing `oarepo-model-builder-drafts-files-4.0.8/oarepo_model_builder_drafts_files/datatypes/components/draft_file_model/blueprints.py` & `oarepo-model-builder-drafts-files-4.0.9/oarepo_model_builder_drafts_files/datatypes/components/draft_file_model/blueprints.py`

 * *Files identical despite different names*

### Comparing `oarepo-model-builder-drafts-files-4.0.8/oarepo_model_builder_drafts_files/datatypes/components/draft_file_model/defaults.py` & `oarepo-model-builder-drafts-files-4.0.9/oarepo_model_builder_drafts_files/datatypes/components/draft_file_model/defaults.py`

 * *Files identical despite different names*

### Comparing `oarepo-model-builder-drafts-files-4.0.8/oarepo_model_builder_drafts_files/datatypes/components/draft_file_model/ext_resource.py` & `oarepo-model-builder-drafts-files-4.0.9/oarepo_model_builder_drafts_files/datatypes/components/draft_file_model/ext_resource.py`

 * *Files identical despite different names*

### Comparing `oarepo-model-builder-drafts-files-4.0.8/oarepo_model_builder_drafts_files/datatypes/components/draft_file_model/files_field.py` & `oarepo-model-builder-drafts-files-4.0.9/oarepo_model_builder_drafts_files/datatypes/components/draft_file_model/files_field.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,9 @@
 from oarepo_model_builder.datatypes.components import RecordModelComponent
 from oarepo_model_builder.datatypes.components.model.utils import set_default
-from oarepo_model_builder.utils.python_name import base_name
 from oarepo_model_builder_files.datatypes import FileDataType
 from oarepo_model_builder_files.datatypes.components import FilesFieldModelComponent
 
 
 class DraftFilesFieldModelComponent(FilesFieldModelComponent):
     eligible_datatypes = [FileDataType]
     depends_on = [RecordModelComponent]
```

### Comparing `oarepo-model-builder-drafts-files-4.0.8/oarepo_model_builder_drafts_files/datatypes/components/draft_file_model/marshmallow.py` & `oarepo-model-builder-drafts-files-4.0.9/oarepo_model_builder_drafts_files/datatypes/components/draft_file_model/marshmallow.py`

 * *Files identical despite different names*

### Comparing `oarepo-model-builder-drafts-files-4.0.8/oarepo_model_builder_drafts_files/datatypes/components/draft_file_model/parent_record.py` & `oarepo-model-builder-drafts-files-4.0.9/oarepo_model_builder_drafts_files/datatypes/components/draft_file_model/parent_record.py`

 * *Files identical despite different names*

### Comparing `oarepo-model-builder-drafts-files-4.0.8/oarepo_model_builder_drafts_files/datatypes/components/draft_file_model/pid.py` & `oarepo-model-builder-drafts-files-4.0.9/oarepo_model_builder_drafts_files/datatypes/components/draft_file_model/pid.py`

 * *Files identical despite different names*

### Comparing `oarepo-model-builder-drafts-files-4.0.8/oarepo_model_builder_drafts_files/datatypes/components/draft_file_model/record.py` & `oarepo-model-builder-drafts-files-4.0.9/oarepo_model_builder_drafts_files/datatypes/components/draft_file_model/record.py`

 * *Files identical despite different names*

### Comparing `oarepo-model-builder-drafts-files-4.0.8/oarepo_model_builder_drafts_files/datatypes/components/draft_file_model/record_metadata.py` & `oarepo-model-builder-drafts-files-4.0.9/oarepo_model_builder_drafts_files/datatypes/components/draft_file_model/record_metadata.py`

 * *Files identical despite different names*

### Comparing `oarepo-model-builder-drafts-files-4.0.8/oarepo_model_builder_drafts_files/datatypes/components/draft_file_model/resource.py` & `oarepo-model-builder-drafts-files-4.0.9/oarepo_model_builder_drafts_files/datatypes/components/draft_file_model/resource.py`

 * *Files identical despite different names*

### Comparing `oarepo-model-builder-drafts-files-4.0.8/oarepo_model_builder_drafts_files/datatypes/components/draft_file_model/service.py` & `oarepo-model-builder-drafts-files-4.0.9/oarepo_model_builder_drafts_files/datatypes/components/draft_file_model/service.py`

 * *Files identical despite different names*

### Comparing `oarepo-model-builder-drafts-files-4.0.8/oarepo_model_builder_drafts_files/datatypes/components/draft_file_profile.py` & `oarepo-model-builder-drafts-files-4.0.9/oarepo_model_builder_drafts_files/datatypes/components/draft_file_profile.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,19 +1,19 @@
 import marshmallow as ma
 from oarepo_model_builder.datatypes import (
     DataType,
     DataTypeComponent,
     ModelDataType,
     Section,
 )
-from oarepo_model_builder.utils.python_name import Import
 from oarepo_model_builder.datatypes.components import DefaultsModelComponent
 from oarepo_model_builder.datatypes.components.model.utils import set_default
 from oarepo_model_builder.datatypes.model import Link
 from oarepo_model_builder.utils.links import url_prefix2link
+from oarepo_model_builder.utils.python_name import Import
 
 
 def get_draft_file_schema():
     from ..draft_file import DraftFileDataType
 
     return DraftFileDataType.validator()
 
@@ -26,17 +26,17 @@
         draft_files = ma.fields.Nested(
             get_draft_file_schema, data_key="draft-files", attribute="draft-files"
         )
 
     def process_mb_invenio_record_service_config(self, *, datatype, section, **kwargs):
         if datatype.root.profile == "draft_files":
             # override class as it has to be a parent class
-            section.config.setdefault("record", {})[
-                "class"
-            ] = datatype.draft_record.definition["record"]["class"]
+            section.config.setdefault("record", {})["class"] = (
+                datatype.draft_record.definition["record"]["class"]
+            )
 
     def process_links(self, datatype, section: Section, **kwargs):
         url_prefix = url_prefix2link(datatype.definition["resource-config"]["base-url"])
 
         if datatype.root.profile == "record":
             has_files = "files" in datatype.definition
             if not has_files:
@@ -121,8 +121,8 @@
 
         set_default(datatype, "json-schema-settings", {}).setdefault("skip", True)
         set_default(datatype, "record-dumper", {}).setdefault("skip", True)
         set_default(datatype, "pid", {}).setdefault("skip", True)
         set_default(datatype, "search-options", {}).setdefault("skip", True)
         set_default(datatype, "record-item", {}).setdefault("skip", True)
         set_default(datatype, "record-list", {}).setdefault("skip", True)
-        set_default(datatype, "permissions", {}).setdefault("skip", True)
+        set_default(datatype, "permissions", {}).setdefault("skip", True)
```

### Comparing `oarepo-model-builder-drafts-files-4.0.8/oarepo_model_builder_drafts_files/datatypes/components/draft_files_tests.py` & `oarepo-model-builder-drafts-files-4.0.9/oarepo_model_builder_drafts_files/datatypes/components/draft_files_tests.py`

 * *Files identical despite different names*

### Comparing `oarepo-model-builder-drafts-files-4.0.8/oarepo_model_builder_drafts_files/datatypes/components/drafts_files_record.py` & `oarepo-model-builder-drafts-files-4.0.9/oarepo_model_builder_drafts_files/datatypes/components/drafts_files_record.py`

 * *Files 0% similar despite different names*

```diff
@@ -19,10 +19,10 @@
                 "service-config",
                 "components",
                 "{{invenio_drafts_resources.services.records.components.DraftFilesComponent}}",
             )
             service = set_default(datatype, "service", {})
             service.setdefault("additional-args", {})
             service["additional-args"] += [
-                    f"files_service=self.service_files",
-                    f"draft_files_service=self.service_draft_files",
-                ]
+                f"files_service=self.service_files",
+                f"draft_files_service=self.service_draft_files",
+            ]
```

### Comparing `oarepo-model-builder-drafts-files-4.0.8/oarepo_model_builder_drafts_files/datatypes/draft_file.py` & `oarepo-model-builder-drafts-files-4.0.9/oarepo_model_builder_drafts_files/datatypes/draft_file.py`

 * *Files identical despite different names*

### Comparing `oarepo-model-builder-drafts-files-4.0.8/oarepo_model_builder_drafts_files/profiles/draft_files.py` & `oarepo-model-builder-drafts-files-4.0.9/oarepo_model_builder_drafts_files/profiles/draft_files.py`

 * *Files identical despite different names*

### Comparing `oarepo-model-builder-drafts-files-4.0.8/oarepo_model_builder_drafts_files.egg-info/PKG-INFO` & `oarepo-model-builder-drafts-files-4.0.9/oarepo_model_builder_drafts_files.egg-info/PKG-INFO`

 * *Files 11% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: oarepo-model-builder-drafts-files
-Version: 4.0.8
+Version: 4.0.9
 Description-Content-Type: text/markdown
 Requires-Dist: oarepo-model-builder-tests>=4.0.0
 Requires-Dist: oarepo-model-builder>=4.0.0
 Requires-Dist: oarepo-model-builder-files>=4.0.0
 Requires-Dist: oarepo-model-builder-drafts>=1.0.4
 
 # OARepo model builder drafts files
```

### Comparing `oarepo-model-builder-drafts-files-4.0.8/oarepo_model_builder_drafts_files.egg-info/SOURCES.txt` & `oarepo-model-builder-drafts-files-4.0.9/oarepo_model_builder_drafts_files.egg-info/SOURCES.txt`

 * *Files 9% similar despite different names*

```diff
@@ -7,15 +7,17 @@
 oarepo_model_builder_drafts_files.egg-info/SOURCES.txt
 oarepo_model_builder_drafts_files.egg-info/dependency_links.txt
 oarepo_model_builder_drafts_files.egg-info/entry_points.txt
 oarepo_model_builder_drafts_files.egg-info/requires.txt
 oarepo_model_builder_drafts_files.egg-info/top_level.txt
 oarepo_model_builder_drafts_files/builders/__init__.py
 oarepo_model_builder_drafts_files/builders/files_service_config_disable_upload.py
+oarepo_model_builder_drafts_files/builders/published_service_files_link.py
 oarepo_model_builder_drafts_files/builders/templates/__init__.py
+oarepo_model_builder_drafts_files/builders/templates/published_service_files_link.py.jinja2
 oarepo_model_builder_drafts_files/builders/templates/service_config_disable_upload.py.jinja2
 oarepo_model_builder_drafts_files/builders/tests/__init__.py
 oarepo_model_builder_drafts_files/builders/tests/conftest.py
 oarepo_model_builder_drafts_files/builders/tests/test_resource.py
 oarepo_model_builder_drafts_files/builders/tests/test_resource_input_data.py
 oarepo_model_builder_drafts_files/builders/tests/templates/__init__.py
 oarepo_model_builder_drafts_files/builders/tests/templates/conftest.py.jinja2
@@ -23,14 +25,15 @@
 oarepo_model_builder_drafts_files/builders/tests/templates/test_resource_input_data.py.jinja2
 oarepo_model_builder_drafts_files/datatypes/__init__.py
 oarepo_model_builder_drafts_files/datatypes/draft_file.py
 oarepo_model_builder_drafts_files/datatypes/components/__init__.py
 oarepo_model_builder_drafts_files/datatypes/components/draft_file_profile.py
 oarepo_model_builder_drafts_files/datatypes/components/draft_files_tests.py
 oarepo_model_builder_drafts_files/datatypes/components/drafts_files_record.py
+oarepo_model_builder_drafts_files/datatypes/components/published_service.py
 oarepo_model_builder_drafts_files/datatypes/components/draft_file_model/__init__.py
 oarepo_model_builder_drafts_files/datatypes/components/draft_file_model/blueprints.py
 oarepo_model_builder_drafts_files/datatypes/components/draft_file_model/defaults.py
 oarepo_model_builder_drafts_files/datatypes/components/draft_file_model/ext_resource.py
 oarepo_model_builder_drafts_files/datatypes/components/draft_file_model/files_field.py
 oarepo_model_builder_drafts_files/datatypes/components/draft_file_model/marshmallow.py
 oarepo_model_builder_drafts_files/datatypes/components/draft_file_model/parent_record.py
```

### Comparing `oarepo-model-builder-drafts-files-4.0.8/oarepo_model_builder_drafts_files.egg-info/entry_points.txt` & `oarepo-model-builder-drafts-files-4.0.9/oarepo_model_builder_drafts_files.egg-info/entry_points.txt`

 * *Files 25% similar despite different names*

```diff
@@ -7,14 +7,21 @@
 5200-test_resource_input_data = oarepo_model_builder_drafts_files.builders.tests.test_resource_input_data:TestResourceInputDataBuilder
 5300-invenio_files_drats_test_files_resources = oarepo_model_builder_drafts_files.builders.tests.test_resource:TestResourcesBuilder
 
 [oarepo_model_builder.builders.draft_files.inherit]
 0100-model = oarepo_model_builder.builders.base
 
 [oarepo_model_builder.builders.files]
+3000-invenio_drafts_published_record_service_config = oarepo_model_builder_drafts.invenio.invenio_drafts_published_record_service_config:InvenioDraftsPublishedRecordServiceConfigBuilder
+3100-invenio_drafts_published_record_service = oarepo_model_builder_drafts.invenio.invenio_drafts_published_record_service:InvenioDraftsPublishedRecordServiceBuilder
+3200-invenio_drafts_published_record_service_ext = oarepo_model_builder_drafts.invenio.invenio_drafts_published_invenio_ext_service:InvenioExtPublishedServiceBuilder
+3300-invenio_drafts_published_api_views = oarepo_model_builder_drafts.invenio.invenio_drafts_published_api_views:InvenioDraftsPublishedApiViewsBuilder
+3400-invenio_drafts_published_app_views = oarepo_model_builder_drafts.invenio.invenio_drafts_published_app_views:InvenioDraftsPublishedAppViewsBuilder
+3500-invenio_drafts_proxies = oarepo_model_builder_drafts.invenio.invenio_drafts_proxies:InvenioDraftsProxiesBuilder
+3600-published_service_files_link = oarepo_model_builder_drafts_files.builders.published_service_files_link:PublishedServiceFilesLinkBuilder
 5000-files-service-config-disable-upload = oarepo_model_builder_drafts_files.builders.files_service_config_disable_upload:FilesServiceConfigDisableUploadBuilder
 
 [oarepo_model_builder.datatypes]
 invenio_files = oarepo_model_builder_drafts_files.datatypes:draft_file_datatypes
 
 [oarepo_model_builder.datatypes.components]
 invenio_drafts_files = oarepo_model_builder_drafts_files.datatypes.components:DRAFTS_FILES_COMPONENTS
```

### Comparing `oarepo-model-builder-drafts-files-4.0.8/setup.cfg` & `oarepo-model-builder-drafts-files-4.0.9/setup.cfg`

 * *Files 27% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [metadata]
 name = oarepo-model-builder-drafts-files
-version = 4.0.8
+version = 4.0.9
 description = 
 authors = Ronald Krist <krist@cesnet.cz>
 readme = README.md
 long_description = file:README.md
 long_description_content_type = text/markdown
 
 [options]
@@ -18,14 +18,22 @@
 [options.package_data]
 * = *.json, *.rst, *.md, *.json5, *.jinja2
 
 [options.entry_points]
 oarepo_model_builder.datatypes.components = 
 	invenio_drafts_files = oarepo_model_builder_drafts_files.datatypes.components:DRAFTS_FILES_COMPONENTS
 oarepo_model_builder.builders.files = 
+	3000-invenio_drafts_published_record_service_config = oarepo_model_builder_drafts.invenio.invenio_drafts_published_record_service_config:InvenioDraftsPublishedRecordServiceConfigBuilder
+	3100-invenio_drafts_published_record_service = oarepo_model_builder_drafts.invenio.invenio_drafts_published_record_service:InvenioDraftsPublishedRecordServiceBuilder
+	3200-invenio_drafts_published_record_service_ext = oarepo_model_builder_drafts.invenio.invenio_drafts_published_invenio_ext_service:InvenioExtPublishedServiceBuilder
+	3300-invenio_drafts_published_api_views = oarepo_model_builder_drafts.invenio.invenio_drafts_published_api_views:InvenioDraftsPublishedApiViewsBuilder
+	3400-invenio_drafts_published_app_views = oarepo_model_builder_drafts.invenio.invenio_drafts_published_app_views:InvenioDraftsPublishedAppViewsBuilder
+	3500-invenio_drafts_proxies = oarepo_model_builder_drafts.invenio.invenio_drafts_proxies:InvenioDraftsProxiesBuilder
+	3600-published_service_files_link = oarepo_model_builder_drafts_files.builders.published_service_files_link:PublishedServiceFilesLinkBuilder
+	
 	5000-files-service-config-disable-upload = oarepo_model_builder_drafts_files.builders.files_service_config_disable_upload:FilesServiceConfigDisableUploadBuilder
 oarepo_model_builder.builders.draft_files.inherit = 
 	0100-model = oarepo_model_builder.builders.base
 oarepo_model_builder.builders.draft_files = 
 	2010-invenio_files_record = oarepo_model_builder_files.builders.invenio.invenio_files_record:InvenioFilesRecordBuilder
 	2010-invenio_files_record_metadata = oarepo_model_builder_files.builders.invenio.invenio_files_record_metadata:InvenioFilesRecordMetadataBuilder
 	2030-invenio_files_parent_record = oarepo_model_builder_files.builders.invenio_parent.invenio_files_parent_record:InvenioFilesParentRecordBuilder
```

