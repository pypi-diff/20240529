# Comparing `tmp/django-autotyping-0.5.0.tar.gz` & `tmp/django_autotyping-0.5.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "django-autotyping-0.5.0.tar", last modified: Sun Feb 18 08:39:42 2024, max compression
+gzip compressed data, was "django_autotyping-0.5.1.tar", last modified: Wed May 29 14:46:45 2024, max compression
```

## Comparing `django-autotyping-0.5.0.tar` & `django_autotyping-0.5.1.tar`

### file list

```diff
@@ -1,67 +1,67 @@
-drwxrwxr-x   0 victorien  (1000) victorien  (1000)        0 2024-02-18 08:39:42.412471 django-autotyping-0.5.0/
--rw-rw-r--   0 victorien  (1000) victorien  (1000)     1063 2023-12-04 16:49:51.000000 django-autotyping-0.5.0/LICENSE
--rw-r--r--   0 victorien  (1000) victorien  (1000)     5477 2024-02-18 08:39:42.412471 django-autotyping-0.5.0/PKG-INFO
--rw-rw-r--   0 victorien  (1000) victorien  (1000)     2886 2024-02-14 19:43:47.000000 django-autotyping-0.5.0/README.md
--rw-rw-r--   0 victorien  (1000) victorien  (1000)     2776 2024-02-04 16:10:12.000000 django-autotyping-0.5.0/pyproject.toml
--rw-rw-r--   0 victorien  (1000) victorien  (1000)       38 2024-02-18 08:39:42.412471 django-autotyping-0.5.0/setup.cfg
--rw-rw-r--   0 victorien  (1000) victorien  (1000)      465 2024-01-24 17:44:25.000000 django-autotyping-0.5.0/setup.py
-drwxrwxr-x   0 victorien  (1000) victorien  (1000)        0 2024-02-18 08:39:42.404471 django-autotyping-0.5.0/src/
-drwxrwxr-x   0 victorien  (1000) victorien  (1000)        0 2024-02-18 08:39:42.404471 django-autotyping-0.5.0/src/django_autotyping/
--rw-rw-r--   0 victorien  (1000) victorien  (1000)       22 2024-02-18 08:38:17.000000 django-autotyping-0.5.0/src/django_autotyping/__init__.py
--rw-rw-r--   0 victorien  (1000) victorien  (1000)      645 2024-02-04 11:19:47.000000 django-autotyping-0.5.0/src/django_autotyping/_compat.py
--rw-rw-r--   0 victorien  (1000) victorien  (1000)     4920 2024-02-14 19:43:47.000000 django-autotyping-0.5.0/src/django_autotyping/app_settings.py
--rw-rw-r--   0 victorien  (1000) victorien  (1000)      111 2024-01-06 14:34:40.000000 django-autotyping-0.5.0/src/django_autotyping/apps.py
-drwxrwxr-x   0 victorien  (1000) victorien  (1000)        0 2024-02-18 08:39:42.408471 django-autotyping-0.5.0/src/django_autotyping/codemodding/
--rw-rw-r--   0 victorien  (1000) victorien  (1000)       90 2024-01-06 14:34:40.000000 django-autotyping-0.5.0/src/django_autotyping/codemodding/__init__.py
-drwxrwxr-x   0 victorien  (1000) victorien  (1000)        0 2024-02-18 08:39:42.408471 django-autotyping-0.5.0/src/django_autotyping/codemodding/codemods/
--rw-rw-r--   0 victorien  (1000) victorien  (1000)      750 2024-02-04 16:10:12.000000 django-autotyping-0.5.0/src/django_autotyping/codemodding/codemods/__init__.py
--rw-rw-r--   0 victorien  (1000) victorien  (1000)      722 2024-01-06 14:34:40.000000 django-autotyping-0.5.0/src/django_autotyping/codemodding/codemods/base.py
--rw-rw-r--   0 victorien  (1000) victorien  (1000)     7957 2024-02-04 16:10:12.000000 django-autotyping-0.5.0/src/django_autotyping/codemodding/codemods/forward_relation_typing_codemod.py
--rw-rw-r--   0 victorien  (1000) victorien  (1000)      932 2024-01-06 14:34:40.000000 django-autotyping-0.5.0/src/django_autotyping/codemodding/django_context.py
--rw-rw-r--   0 victorien  (1000) victorien  (1000)     1654 2024-01-09 17:15:46.000000 django-autotyping-0.5.0/src/django_autotyping/codemodding/main.py
--rw-rw-r--   0 victorien  (1000) victorien  (1000)     2511 2023-12-17 18:18:13.000000 django-autotyping-0.5.0/src/django_autotyping/codemodding/models.py
-drwxrwxr-x   0 victorien  (1000) victorien  (1000)        0 2024-02-18 08:39:42.408471 django-autotyping-0.5.0/src/django_autotyping/codemodding/vendoring/
--rw-rw-r--   0 victorien  (1000) victorien  (1000)        0 2023-12-17 18:18:13.000000 django-autotyping-0.5.0/src/django_autotyping/codemodding/vendoring/__init__.py
-drwxrwxr-x   0 victorien  (1000) victorien  (1000)        0 2024-02-18 08:39:42.408471 django-autotyping-0.5.0/src/django_autotyping/codemodding/vendoring/monkeytype/
--rw-rw-r--   0 victorien  (1000) victorien  (1000)     2504 2023-12-17 18:18:13.000000 django-autotyping-0.5.0/src/django_autotyping/codemodding/vendoring/monkeytype/__init__.py
--rw-rw-r--   0 victorien  (1000) victorien  (1000)     7563 2023-12-17 18:18:13.000000 django-autotyping-0.5.0/src/django_autotyping/codemodding/vendoring/monkeytype/type_checking_imports_transformer.py
-drwxrwxr-x   0 victorien  (1000) victorien  (1000)        0 2024-02-18 08:39:42.408471 django-autotyping-0.5.0/src/django_autotyping/management/
--rw-rw-r--   0 victorien  (1000) victorien  (1000)        0 2024-01-06 14:34:40.000000 django-autotyping-0.5.0/src/django_autotyping/management/__init__.py
-drwxrwxr-x   0 victorien  (1000) victorien  (1000)        0 2024-02-18 08:39:42.408471 django-autotyping-0.5.0/src/django_autotyping/management/commands/
--rw-rw-r--   0 victorien  (1000) victorien  (1000)        0 2024-01-06 14:34:40.000000 django-autotyping-0.5.0/src/django_autotyping/management/commands/__init__.py
--rw-rw-r--   0 victorien  (1000) victorien  (1000)      999 2024-01-06 14:34:40.000000 django-autotyping-0.5.0/src/django_autotyping/management/commands/_utils.py
--rw-rw-r--   0 victorien  (1000) victorien  (1000)     3344 2024-02-04 16:10:12.000000 django-autotyping-0.5.0/src/django_autotyping/management/commands/add_type_hints.py
--rw-rw-r--   0 victorien  (1000) victorien  (1000)     1856 2024-02-14 19:43:42.000000 django-autotyping-0.5.0/src/django_autotyping/management/commands/generate_stubs.py
--rw-rw-r--   0 victorien  (1000) victorien  (1000)        0 2023-12-04 16:49:51.000000 django-autotyping-0.5.0/src/django_autotyping/py.typed
-drwxrwxr-x   0 victorien  (1000) victorien  (1000)        0 2024-02-18 08:39:42.408471 django-autotyping-0.5.0/src/django_autotyping/stubbing/
--rw-rw-r--   0 victorien  (1000) victorien  (1000)     2398 2024-02-14 19:43:42.000000 django-autotyping-0.5.0/src/django_autotyping/stubbing/__init__.py
-drwxrwxr-x   0 victorien  (1000) victorien  (1000)        0 2024-02-18 08:39:42.412471 django-autotyping-0.5.0/src/django_autotyping/stubbing/codemods/
--rw-rw-r--   0 victorien  (1000) victorien  (1000)     2022 2024-02-18 08:30:43.000000 django-autotyping-0.5.0/src/django_autotyping/stubbing/codemods/__init__.py
--rw-rw-r--   0 victorien  (1000) victorien  (1000)   145865 2024-01-23 20:52:58.000000 django-autotyping-0.5.0/src/django_autotyping/stubbing/codemods/_global_settings_types.py
--rw-rw-r--   0 victorien  (1000) victorien  (1000)     9379 2024-02-16 17:32:36.000000 django-autotyping-0.5.0/src/django_autotyping/stubbing/codemods/_model_creation.py
--rw-rw-r--   0 victorien  (1000) victorien  (1000)     5365 2024-02-18 08:30:43.000000 django-autotyping-0.5.0/src/django_autotyping/stubbing/codemods/_utils.py
--rw-rw-r--   0 victorien  (1000) victorien  (1000)     4076 2024-02-04 16:10:05.000000 django-autotyping-0.5.0/src/django_autotyping/stubbing/codemods/auth_functions_codemod.py
--rw-rw-r--   0 victorien  (1000) victorien  (1000)     3701 2024-02-04 11:19:47.000000 django-autotyping-0.5.0/src/django_autotyping/stubbing/codemods/base.py
--rw-rw-r--   0 victorien  (1000) victorien  (1000)     8466 2024-02-06 20:38:31.000000 django-autotyping-0.5.0/src/django_autotyping/stubbing/codemods/call_command_codemod.py
--rw-rw-r--   0 victorien  (1000) victorien  (1000)       89 2023-12-21 07:17:05.000000 django-autotyping-0.5.0/src/django_autotyping/stubbing/codemods/constants.py
--rw-rw-r--   0 victorien  (1000) victorien  (1000)     2214 2024-02-04 11:19:47.000000 django-autotyping-0.5.0/src/django_autotyping/stubbing/codemods/create_overload_codemod.py
--rw-rw-r--   0 victorien  (1000) victorien  (1000)    12885 2024-02-18 08:32:58.000000 django-autotyping-0.5.0/src/django_autotyping/stubbing/codemods/forward_relation_overload_codemod.py
--rw-rw-r--   0 victorien  (1000) victorien  (1000)     3447 2024-01-23 20:52:58.000000 django-autotyping-0.5.0/src/django_autotyping/stubbing/codemods/get_model_overload_codemod.py
--rw-rw-r--   0 victorien  (1000) victorien  (1000)     2738 2024-02-04 11:19:47.000000 django-autotyping-0.5.0/src/django_autotyping/stubbing/codemods/model_init_overload_codemod.py
--rw-rw-r--   0 victorien  (1000) victorien  (1000)     3521 2024-02-04 16:34:38.000000 django-autotyping-0.5.0/src/django_autotyping/stubbing/codemods/query_lookups_overload_codemod.py
--rw-rw-r--   0 victorien  (1000) victorien  (1000)     7375 2024-02-04 16:10:12.000000 django-autotyping-0.5.0/src/django_autotyping/stubbing/codemods/reverse_overload_codemod.py
--rw-rw-r--   0 victorien  (1000) victorien  (1000)     7034 2024-02-04 16:10:12.000000 django-autotyping-0.5.0/src/django_autotyping/stubbing/codemods/settings_codemod.py
--rw-rw-r--   0 victorien  (1000) victorien  (1000)     6194 2024-02-18 08:30:43.000000 django-autotyping-0.5.0/src/django_autotyping/stubbing/codemods/template_loading_codemod.py
-drwxrwxr-x   0 victorien  (1000) victorien  (1000)        0 2024-02-18 08:39:42.412471 django-autotyping-0.5.0/src/django_autotyping/stubbing/django_context/
--rw-rw-r--   0 victorien  (1000) victorien  (1000)       88 2024-02-04 10:15:26.000000 django-autotyping-0.5.0/src/django_autotyping/stubbing/django_context/__init__.py
--rw-rw-r--   0 victorien  (1000) victorien  (1000)    13594 2024-02-04 16:10:12.000000 django-autotyping-0.5.0/src/django_autotyping/stubbing/django_context/_management_utils.py
--rw-rw-r--   0 victorien  (1000) victorien  (1000)     1352 2024-02-18 08:30:43.000000 django-autotyping-0.5.0/src/django_autotyping/stubbing/django_context/_template_utils.py
--rw-rw-r--   0 victorien  (1000) victorien  (1000)     5239 2024-02-04 16:10:12.000000 django-autotyping-0.5.0/src/django_autotyping/stubbing/django_context/_url_utils.py
--rw-rw-r--   0 victorien  (1000) victorien  (1000)     3997 2024-02-18 08:30:43.000000 django-autotyping-0.5.0/src/django_autotyping/stubbing/django_context/django_context.py
--rw-rw-r--   0 victorien  (1000) victorien  (1000)     4425 2024-02-18 08:30:43.000000 django-autotyping-0.5.0/src/django_autotyping/typing.py
-drwxrwxr-x   0 victorien  (1000) victorien  (1000)        0 2024-02-18 08:39:42.412471 django-autotyping-0.5.0/src/django_autotyping.egg-info/
--rw-r--r--   0 victorien  (1000) victorien  (1000)     5477 2024-02-18 08:39:42.000000 django-autotyping-0.5.0/src/django_autotyping.egg-info/PKG-INFO
--rw-rw-r--   0 victorien  (1000) victorien  (1000)     2687 2024-02-18 08:39:42.000000 django-autotyping-0.5.0/src/django_autotyping.egg-info/SOURCES.txt
--rw-rw-r--   0 victorien  (1000) victorien  (1000)        1 2024-02-18 08:39:42.000000 django-autotyping-0.5.0/src/django_autotyping.egg-info/dependency_links.txt
--rw-rw-r--   0 victorien  (1000) victorien  (1000)       75 2024-02-18 08:39:42.000000 django-autotyping-0.5.0/src/django_autotyping.egg-info/requires.txt
--rw-rw-r--   0 victorien  (1000) victorien  (1000)       18 2024-02-18 08:39:42.000000 django-autotyping-0.5.0/src/django_autotyping.egg-info/top_level.txt
+drwxrwxr-x   0 victorien  (1000) victorien  (1000)        0 2024-05-29 14:46:45.861453 django_autotyping-0.5.1/
+-rw-rw-r--   0 victorien  (1000) victorien  (1000)     1063 2023-12-04 16:49:51.000000 django_autotyping-0.5.1/LICENSE
+-rw-r--r--   0 victorien  (1000) victorien  (1000)     5477 2024-05-29 14:46:45.861453 django_autotyping-0.5.1/PKG-INFO
+-rw-rw-r--   0 victorien  (1000) victorien  (1000)     2886 2024-02-14 19:43:47.000000 django_autotyping-0.5.1/README.md
+-rw-rw-r--   0 victorien  (1000) victorien  (1000)     2776 2024-02-23 18:32:47.000000 django_autotyping-0.5.1/pyproject.toml
+-rw-rw-r--   0 victorien  (1000) victorien  (1000)       38 2024-05-29 14:46:45.861453 django_autotyping-0.5.1/setup.cfg
+-rw-rw-r--   0 victorien  (1000) victorien  (1000)      465 2024-01-24 17:44:25.000000 django_autotyping-0.5.1/setup.py
+drwxrwxr-x   0 victorien  (1000) victorien  (1000)        0 2024-05-29 14:46:45.849453 django_autotyping-0.5.1/src/
+drwxrwxr-x   0 victorien  (1000) victorien  (1000)        0 2024-05-29 14:46:45.853453 django_autotyping-0.5.1/src/django_autotyping/
+-rw-rw-r--   0 victorien  (1000) victorien  (1000)       22 2024-05-29 14:45:26.000000 django_autotyping-0.5.1/src/django_autotyping/__init__.py
+-rw-rw-r--   0 victorien  (1000) victorien  (1000)      645 2024-02-04 11:19:47.000000 django_autotyping-0.5.1/src/django_autotyping/_compat.py
+-rw-rw-r--   0 victorien  (1000) victorien  (1000)     4920 2024-03-21 18:28:54.000000 django_autotyping-0.5.1/src/django_autotyping/app_settings.py
+-rw-rw-r--   0 victorien  (1000) victorien  (1000)      111 2024-01-06 14:34:40.000000 django_autotyping-0.5.1/src/django_autotyping/apps.py
+drwxrwxr-x   0 victorien  (1000) victorien  (1000)        0 2024-05-29 14:46:45.853453 django_autotyping-0.5.1/src/django_autotyping/codemodding/
+-rw-rw-r--   0 victorien  (1000) victorien  (1000)       90 2024-01-06 14:34:40.000000 django_autotyping-0.5.1/src/django_autotyping/codemodding/__init__.py
+drwxrwxr-x   0 victorien  (1000) victorien  (1000)        0 2024-05-29 14:46:45.853453 django_autotyping-0.5.1/src/django_autotyping/codemodding/codemods/
+-rw-rw-r--   0 victorien  (1000) victorien  (1000)      750 2024-02-04 16:10:12.000000 django_autotyping-0.5.1/src/django_autotyping/codemodding/codemods/__init__.py
+-rw-rw-r--   0 victorien  (1000) victorien  (1000)      722 2024-01-06 14:34:40.000000 django_autotyping-0.5.1/src/django_autotyping/codemodding/codemods/base.py
+-rw-rw-r--   0 victorien  (1000) victorien  (1000)     7957 2024-02-04 16:10:12.000000 django_autotyping-0.5.1/src/django_autotyping/codemodding/codemods/forward_relation_typing_codemod.py
+-rw-rw-r--   0 victorien  (1000) victorien  (1000)      932 2024-01-06 14:34:40.000000 django_autotyping-0.5.1/src/django_autotyping/codemodding/django_context.py
+-rw-rw-r--   0 victorien  (1000) victorien  (1000)     1654 2024-01-09 17:15:46.000000 django_autotyping-0.5.1/src/django_autotyping/codemodding/main.py
+-rw-rw-r--   0 victorien  (1000) victorien  (1000)     2511 2023-12-17 18:18:13.000000 django_autotyping-0.5.1/src/django_autotyping/codemodding/models.py
+drwxrwxr-x   0 victorien  (1000) victorien  (1000)        0 2024-05-29 14:46:45.853453 django_autotyping-0.5.1/src/django_autotyping/codemodding/vendoring/
+-rw-rw-r--   0 victorien  (1000) victorien  (1000)        0 2023-12-17 18:18:13.000000 django_autotyping-0.5.1/src/django_autotyping/codemodding/vendoring/__init__.py
+drwxrwxr-x   0 victorien  (1000) victorien  (1000)        0 2024-05-29 14:46:45.857453 django_autotyping-0.5.1/src/django_autotyping/codemodding/vendoring/monkeytype/
+-rw-rw-r--   0 victorien  (1000) victorien  (1000)     2504 2023-12-17 18:18:13.000000 django_autotyping-0.5.1/src/django_autotyping/codemodding/vendoring/monkeytype/__init__.py
+-rw-rw-r--   0 victorien  (1000) victorien  (1000)     7563 2023-12-17 18:18:13.000000 django_autotyping-0.5.1/src/django_autotyping/codemodding/vendoring/monkeytype/type_checking_imports_transformer.py
+drwxrwxr-x   0 victorien  (1000) victorien  (1000)        0 2024-05-29 14:46:45.857453 django_autotyping-0.5.1/src/django_autotyping/management/
+-rw-rw-r--   0 victorien  (1000) victorien  (1000)        0 2024-01-06 14:34:40.000000 django_autotyping-0.5.1/src/django_autotyping/management/__init__.py
+drwxrwxr-x   0 victorien  (1000) victorien  (1000)        0 2024-05-29 14:46:45.857453 django_autotyping-0.5.1/src/django_autotyping/management/commands/
+-rw-rw-r--   0 victorien  (1000) victorien  (1000)        0 2024-01-06 14:34:40.000000 django_autotyping-0.5.1/src/django_autotyping/management/commands/__init__.py
+-rw-rw-r--   0 victorien  (1000) victorien  (1000)      999 2024-01-06 14:34:40.000000 django_autotyping-0.5.1/src/django_autotyping/management/commands/_utils.py
+-rw-rw-r--   0 victorien  (1000) victorien  (1000)     3344 2024-02-04 16:10:12.000000 django_autotyping-0.5.1/src/django_autotyping/management/commands/add_type_hints.py
+-rw-rw-r--   0 victorien  (1000) victorien  (1000)     1856 2024-02-14 19:43:42.000000 django_autotyping-0.5.1/src/django_autotyping/management/commands/generate_stubs.py
+-rw-rw-r--   0 victorien  (1000) victorien  (1000)        0 2023-12-04 16:49:51.000000 django_autotyping-0.5.1/src/django_autotyping/py.typed
+drwxrwxr-x   0 victorien  (1000) victorien  (1000)        0 2024-05-29 14:46:45.857453 django_autotyping-0.5.1/src/django_autotyping/stubbing/
+-rw-rw-r--   0 victorien  (1000) victorien  (1000)     2398 2024-02-14 19:43:42.000000 django_autotyping-0.5.1/src/django_autotyping/stubbing/__init__.py
+drwxrwxr-x   0 victorien  (1000) victorien  (1000)        0 2024-05-29 14:46:45.857453 django_autotyping-0.5.1/src/django_autotyping/stubbing/codemods/
+-rw-rw-r--   0 victorien  (1000) victorien  (1000)     2022 2024-02-18 08:30:43.000000 django_autotyping-0.5.1/src/django_autotyping/stubbing/codemods/__init__.py
+-rw-rw-r--   0 victorien  (1000) victorien  (1000)   145865 2024-01-23 20:52:58.000000 django_autotyping-0.5.1/src/django_autotyping/stubbing/codemods/_global_settings_types.py
+-rw-rw-r--   0 victorien  (1000) victorien  (1000)     9379 2024-05-29 14:44:38.000000 django_autotyping-0.5.1/src/django_autotyping/stubbing/codemods/_model_creation.py
+-rw-rw-r--   0 victorien  (1000) victorien  (1000)     5365 2024-02-18 08:30:43.000000 django_autotyping-0.5.1/src/django_autotyping/stubbing/codemods/_utils.py
+-rw-rw-r--   0 victorien  (1000) victorien  (1000)     4076 2024-02-04 16:10:05.000000 django_autotyping-0.5.1/src/django_autotyping/stubbing/codemods/auth_functions_codemod.py
+-rw-rw-r--   0 victorien  (1000) victorien  (1000)     3701 2024-02-04 11:19:47.000000 django_autotyping-0.5.1/src/django_autotyping/stubbing/codemods/base.py
+-rw-rw-r--   0 victorien  (1000) victorien  (1000)     8466 2024-02-06 20:38:31.000000 django_autotyping-0.5.1/src/django_autotyping/stubbing/codemods/call_command_codemod.py
+-rw-rw-r--   0 victorien  (1000) victorien  (1000)       89 2023-12-21 07:17:05.000000 django_autotyping-0.5.1/src/django_autotyping/stubbing/codemods/constants.py
+-rw-rw-r--   0 victorien  (1000) victorien  (1000)     2214 2024-02-04 11:19:47.000000 django_autotyping-0.5.1/src/django_autotyping/stubbing/codemods/create_overload_codemod.py
+-rw-rw-r--   0 victorien  (1000) victorien  (1000)    12885 2024-02-18 08:32:58.000000 django_autotyping-0.5.1/src/django_autotyping/stubbing/codemods/forward_relation_overload_codemod.py
+-rw-rw-r--   0 victorien  (1000) victorien  (1000)     3447 2024-01-23 20:52:58.000000 django_autotyping-0.5.1/src/django_autotyping/stubbing/codemods/get_model_overload_codemod.py
+-rw-rw-r--   0 victorien  (1000) victorien  (1000)     2738 2024-02-04 11:19:47.000000 django_autotyping-0.5.1/src/django_autotyping/stubbing/codemods/model_init_overload_codemod.py
+-rw-rw-r--   0 victorien  (1000) victorien  (1000)     3521 2024-02-04 16:34:38.000000 django_autotyping-0.5.1/src/django_autotyping/stubbing/codemods/query_lookups_overload_codemod.py
+-rw-rw-r--   0 victorien  (1000) victorien  (1000)     7375 2024-02-04 16:10:12.000000 django_autotyping-0.5.1/src/django_autotyping/stubbing/codemods/reverse_overload_codemod.py
+-rw-rw-r--   0 victorien  (1000) victorien  (1000)     7034 2024-02-04 16:10:12.000000 django_autotyping-0.5.1/src/django_autotyping/stubbing/codemods/settings_codemod.py
+-rw-rw-r--   0 victorien  (1000) victorien  (1000)     6194 2024-02-18 08:30:43.000000 django_autotyping-0.5.1/src/django_autotyping/stubbing/codemods/template_loading_codemod.py
+drwxrwxr-x   0 victorien  (1000) victorien  (1000)        0 2024-05-29 14:46:45.861453 django_autotyping-0.5.1/src/django_autotyping/stubbing/django_context/
+-rw-rw-r--   0 victorien  (1000) victorien  (1000)       88 2024-02-04 10:15:26.000000 django_autotyping-0.5.1/src/django_autotyping/stubbing/django_context/__init__.py
+-rw-rw-r--   0 victorien  (1000) victorien  (1000)    13594 2024-02-04 16:10:12.000000 django_autotyping-0.5.1/src/django_autotyping/stubbing/django_context/_management_utils.py
+-rw-rw-r--   0 victorien  (1000) victorien  (1000)     1352 2024-02-18 08:30:43.000000 django_autotyping-0.5.1/src/django_autotyping/stubbing/django_context/_template_utils.py
+-rw-rw-r--   0 victorien  (1000) victorien  (1000)     5239 2024-02-04 16:10:12.000000 django_autotyping-0.5.1/src/django_autotyping/stubbing/django_context/_url_utils.py
+-rw-rw-r--   0 victorien  (1000) victorien  (1000)     4619 2024-05-29 14:39:32.000000 django_autotyping-0.5.1/src/django_autotyping/stubbing/django_context/django_context.py
+-rw-rw-r--   0 victorien  (1000) victorien  (1000)     4425 2024-02-18 08:30:43.000000 django_autotyping-0.5.1/src/django_autotyping/typing.py
+drwxrwxr-x   0 victorien  (1000) victorien  (1000)        0 2024-05-29 14:46:45.861453 django_autotyping-0.5.1/src/django_autotyping.egg-info/
+-rw-r--r--   0 victorien  (1000) victorien  (1000)     5477 2024-05-29 14:46:45.000000 django_autotyping-0.5.1/src/django_autotyping.egg-info/PKG-INFO
+-rw-rw-r--   0 victorien  (1000) victorien  (1000)     2687 2024-05-29 14:46:45.000000 django_autotyping-0.5.1/src/django_autotyping.egg-info/SOURCES.txt
+-rw-rw-r--   0 victorien  (1000) victorien  (1000)        1 2024-05-29 14:46:45.000000 django_autotyping-0.5.1/src/django_autotyping.egg-info/dependency_links.txt
+-rw-rw-r--   0 victorien  (1000) victorien  (1000)       75 2024-05-29 14:46:45.000000 django_autotyping-0.5.1/src/django_autotyping.egg-info/requires.txt
+-rw-rw-r--   0 victorien  (1000) victorien  (1000)       18 2024-05-29 14:46:45.000000 django_autotyping-0.5.1/src/django_autotyping.egg-info/top_level.txt
```

### Comparing `django-autotyping-0.5.0/LICENSE` & `django_autotyping-0.5.1/LICENSE`

 * *Files identical despite different names*

### Comparing `django-autotyping-0.5.0/PKG-INFO` & `django_autotyping-0.5.1/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: django-autotyping
-Version: 0.5.0
+Version: 0.5.1
 Summary: Automatically add type hints for Django powered applications.
 Author-email: Viicos <65306057+Viicos@users.noreply.github.com>
 License: MIT License
         
         Copyright (c) 2023 Viicos
         
         Permission is hereby granted, free of charge, to any person obtaining a copy
```

### Comparing `django-autotyping-0.5.0/README.md` & `django_autotyping-0.5.1/README.md`

 * *Files identical despite different names*

### Comparing `django-autotyping-0.5.0/pyproject.toml` & `django_autotyping-0.5.1/pyproject.toml`

 * *Files identical despite different names*

### Comparing `django-autotyping-0.5.0/src/django_autotyping/_compat.py` & `django_autotyping-0.5.1/src/django_autotyping/_compat.py`

 * *Files identical despite different names*

### Comparing `django-autotyping-0.5.0/src/django_autotyping/app_settings.py` & `django_autotyping-0.5.1/src/django_autotyping/app_settings.py`

 * *Files identical despite different names*

### Comparing `django-autotyping-0.5.0/src/django_autotyping/codemodding/codemods/__init__.py` & `django_autotyping-0.5.1/src/django_autotyping/codemodding/codemods/__init__.py`

 * *Files identical despite different names*

### Comparing `django-autotyping-0.5.0/src/django_autotyping/codemodding/codemods/base.py` & `django_autotyping-0.5.1/src/django_autotyping/codemodding/codemods/base.py`

 * *Files identical despite different names*

### Comparing `django-autotyping-0.5.0/src/django_autotyping/codemodding/codemods/forward_relation_typing_codemod.py` & `django_autotyping-0.5.1/src/django_autotyping/codemodding/codemods/forward_relation_typing_codemod.py`

 * *Files identical despite different names*

### Comparing `django-autotyping-0.5.0/src/django_autotyping/codemodding/django_context.py` & `django_autotyping-0.5.1/src/django_autotyping/codemodding/django_context.py`

 * *Files identical despite different names*

### Comparing `django-autotyping-0.5.0/src/django_autotyping/codemodding/main.py` & `django_autotyping-0.5.1/src/django_autotyping/codemodding/main.py`

 * *Files identical despite different names*

### Comparing `django-autotyping-0.5.0/src/django_autotyping/codemodding/models.py` & `django_autotyping-0.5.1/src/django_autotyping/codemodding/models.py`

 * *Files identical despite different names*

### Comparing `django-autotyping-0.5.0/src/django_autotyping/codemodding/vendoring/monkeytype/__init__.py` & `django_autotyping-0.5.1/src/django_autotyping/codemodding/vendoring/monkeytype/__init__.py`

 * *Files identical despite different names*

### Comparing `django-autotyping-0.5.0/src/django_autotyping/codemodding/vendoring/monkeytype/type_checking_imports_transformer.py` & `django_autotyping-0.5.1/src/django_autotyping/codemodding/vendoring/monkeytype/type_checking_imports_transformer.py`

 * *Files identical despite different names*

### Comparing `django-autotyping-0.5.0/src/django_autotyping/management/commands/_utils.py` & `django_autotyping-0.5.1/src/django_autotyping/management/commands/_utils.py`

 * *Files identical despite different names*

### Comparing `django-autotyping-0.5.0/src/django_autotyping/management/commands/add_type_hints.py` & `django_autotyping-0.5.1/src/django_autotyping/management/commands/add_type_hints.py`

 * *Files identical despite different names*

### Comparing `django-autotyping-0.5.0/src/django_autotyping/management/commands/generate_stubs.py` & `django_autotyping-0.5.1/src/django_autotyping/management/commands/generate_stubs.py`

 * *Files identical despite different names*

### Comparing `django-autotyping-0.5.0/src/django_autotyping/stubbing/__init__.py` & `django_autotyping-0.5.1/src/django_autotyping/stubbing/__init__.py`

 * *Files identical despite different names*

### Comparing `django-autotyping-0.5.0/src/django_autotyping/stubbing/codemods/__init__.py` & `django_autotyping-0.5.1/src/django_autotyping/stubbing/codemods/__init__.py`

 * *Files identical despite different names*

### Comparing `django-autotyping-0.5.0/src/django_autotyping/stubbing/codemods/_global_settings_types.py` & `django_autotyping-0.5.1/src/django_autotyping/stubbing/codemods/_global_settings_types.py`

 * *Files identical despite different names*

### Comparing `django-autotyping-0.5.0/src/django_autotyping/stubbing/codemods/_model_creation.py` & `django_autotyping-0.5.1/src/django_autotyping/stubbing/codemods/_model_creation.py`

 * *Files 1% similar despite different names*

```diff
@@ -65,15 +65,15 @@
     GenericIPAddressField: {
         "type": "str | int | Callable[..., Any] | Combinable",  # TODO, Callable, really?
         "typing_imports": ["Any", "Callable"],
     },
     # For datetime related fields, we use `datetime.x` because `datetime`
     # is already imported in `db/models/manager.pyi`:
     DateTimeField: {
-        "type": "str | datetime.datetime | datetime.Date | Combinable",
+        "type": "str | datetime.datetime | datetime.date | Combinable",
         "extra_imports": [ImportItem("datetime")],
     },
     DateField: {
         "type": "str | datetime.date | Combinable",
         "extra_imports": [ImportItem("datetime")],
     },
     TimeField: {
```

### Comparing `django-autotyping-0.5.0/src/django_autotyping/stubbing/codemods/_utils.py` & `django_autotyping-0.5.1/src/django_autotyping/stubbing/codemods/_utils.py`

 * *Files identical despite different names*

### Comparing `django-autotyping-0.5.0/src/django_autotyping/stubbing/codemods/auth_functions_codemod.py` & `django_autotyping-0.5.1/src/django_autotyping/stubbing/codemods/auth_functions_codemod.py`

 * *Files identical despite different names*

### Comparing `django-autotyping-0.5.0/src/django_autotyping/stubbing/codemods/base.py` & `django_autotyping-0.5.1/src/django_autotyping/stubbing/codemods/base.py`

 * *Files identical despite different names*

### Comparing `django-autotyping-0.5.0/src/django_autotyping/stubbing/codemods/call_command_codemod.py` & `django_autotyping-0.5.1/src/django_autotyping/stubbing/codemods/call_command_codemod.py`

 * *Files identical despite different names*

### Comparing `django-autotyping-0.5.0/src/django_autotyping/stubbing/codemods/create_overload_codemod.py` & `django_autotyping-0.5.1/src/django_autotyping/stubbing/codemods/create_overload_codemod.py`

 * *Files identical despite different names*

### Comparing `django-autotyping-0.5.0/src/django_autotyping/stubbing/codemods/forward_relation_overload_codemod.py` & `django_autotyping-0.5.1/src/django_autotyping/stubbing/codemods/forward_relation_overload_codemod.py`

 * *Files identical despite different names*

### Comparing `django-autotyping-0.5.0/src/django_autotyping/stubbing/codemods/get_model_overload_codemod.py` & `django_autotyping-0.5.1/src/django_autotyping/stubbing/codemods/get_model_overload_codemod.py`

 * *Files identical despite different names*

### Comparing `django-autotyping-0.5.0/src/django_autotyping/stubbing/codemods/model_init_overload_codemod.py` & `django_autotyping-0.5.1/src/django_autotyping/stubbing/codemods/model_init_overload_codemod.py`

 * *Files identical despite different names*

### Comparing `django-autotyping-0.5.0/src/django_autotyping/stubbing/codemods/query_lookups_overload_codemod.py` & `django_autotyping-0.5.1/src/django_autotyping/stubbing/codemods/query_lookups_overload_codemod.py`

 * *Files identical despite different names*

### Comparing `django-autotyping-0.5.0/src/django_autotyping/stubbing/codemods/reverse_overload_codemod.py` & `django_autotyping-0.5.1/src/django_autotyping/stubbing/codemods/reverse_overload_codemod.py`

 * *Files identical despite different names*

### Comparing `django-autotyping-0.5.0/src/django_autotyping/stubbing/codemods/settings_codemod.py` & `django_autotyping-0.5.1/src/django_autotyping/stubbing/codemods/settings_codemod.py`

 * *Files identical despite different names*

### Comparing `django-autotyping-0.5.0/src/django_autotyping/stubbing/codemods/template_loading_codemod.py` & `django_autotyping-0.5.1/src/django_autotyping/stubbing/codemods/template_loading_codemod.py`

 * *Files identical despite different names*

### Comparing `django-autotyping-0.5.0/src/django_autotyping/stubbing/django_context/_management_utils.py` & `django_autotyping-0.5.1/src/django_autotyping/stubbing/django_context/_management_utils.py`

 * *Files identical despite different names*

### Comparing `django-autotyping-0.5.0/src/django_autotyping/stubbing/django_context/_template_utils.py` & `django_autotyping-0.5.1/src/django_autotyping/stubbing/django_context/_template_utils.py`

 * *Files identical despite different names*

### Comparing `django-autotyping-0.5.0/src/django_autotyping/stubbing/django_context/_url_utils.py` & `django_autotyping-0.5.1/src/django_autotyping/stubbing/django_context/_url_utils.py`

 * *Files identical despite different names*

### Comparing `django-autotyping-0.5.0/src/django_autotyping/stubbing/django_context/django_context.py` & `django_autotyping-0.5.1/src/django_autotyping/stubbing/django_context/django_context.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,10 +1,12 @@
 from __future__ import annotations
 
+import inspect
 from collections import defaultdict
+from types import ModuleType
 
 from django.apps.registry import Apps
 from django.conf import LazySettings
 from django.core.management import get_commands
 from django.db.models import NOT_PROVIDED, DateField, Field
 from django.template import engines
 from django.urls import get_resolver
@@ -21,35 +23,49 @@
 class DjangoStubbingContext:
     def __init__(self, apps: Apps, settings: LazySettings) -> None:
         self.apps = apps
         self.settings = settings
 
     @staticmethod
     def _get_model_alias(model: ModelType) -> str:
-        """Return an alias of the model, by converting the app label to PascalCase and joining
+        """Return an alias of the model.
+
+        The alias is constructed by converting the app label to PascalCase and joining
         the app label to the model name.
         """
         app_label = to_pascal(model._meta.app_label)
         return f"{app_label}{model.__name__}"
 
+    @staticmethod
+    def _get_model_module(model: ModelType) -> ModuleType:
+        """Return the module object where the model class is exported or defined.
+
+        Use the models module of the app where the model is defined, and fallback
+        to the actual module of the model class in case the model is not exported
+        or present in the models module.
+        """
+        if model._meta.app_config.models_module is not None:
+            return model._meta.app_config.models_module
+        return inspect.getmodule(model)  # type: ignore
+
     @property
     def models(self) -> list[ModelType]:
         """All the defined models. Abstract models are not included."""
         return self.apps.get_models()
 
     @property
     def model_imports(self) -> list[ImportItem]:
         """A list of `ImportItem` instances.
 
         Can be used to easily import all models in a stub file.
         """
 
         return [
             ImportItem(
-                module_name=model._meta.app_config.models_module.__name__,
+                module_name=self._get_model_module(model).__name__,
                 obj_name=model.__name__,
                 alias=self._get_model_alias(model) if self.is_duplicate(model) else None,
             )
             for model in self.models
         ]
 
     @property
```

### Comparing `django-autotyping-0.5.0/src/django_autotyping/typing.py` & `django_autotyping-0.5.1/src/django_autotyping/typing.py`

 * *Files identical despite different names*

### Comparing `django-autotyping-0.5.0/src/django_autotyping.egg-info/PKG-INFO` & `django_autotyping-0.5.1/src/django_autotyping.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: django-autotyping
-Version: 0.5.0
+Version: 0.5.1
 Summary: Automatically add type hints for Django powered applications.
 Author-email: Viicos <65306057+Viicos@users.noreply.github.com>
 License: MIT License
         
         Copyright (c) 2023 Viicos
         
         Permission is hereby granted, free of charge, to any person obtaining a copy
```

### Comparing `django-autotyping-0.5.0/src/django_autotyping.egg-info/SOURCES.txt` & `django_autotyping-0.5.1/src/django_autotyping.egg-info/SOURCES.txt`

 * *Files identical despite different names*

