# Comparing `tmp/jsondataferret-0.7.0.tar.gz` & `tmp/jsondataferret-0.7.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/jsondataferret-0.7.0.tar", last modified: Wed Oct 26 11:26:54 2022, max compression
+gzip compressed data, was "jsondataferret-0.7.1.tar", last modified: Wed May 29 12:09:55 2024, max compression
```

## Comparing `jsondataferret-0.7.0.tar` & `jsondataferret-0.7.1.tar`

### file list

```diff
@@ -1,94 +1,92 @@
-drwxrwxr-x   0 odscjames  (1000) odscjames  (1000)        0 2022-10-26 11:26:54.000000 jsondataferret-0.7.0/
-drwxrwxr-x   0 odscjames  (1000) odscjames  (1000)        0 2022-10-26 11:26:54.000000 jsondataferret-0.7.0/jsondataferret.egg-info/
--rw-r--r--   0 odscjames  (1000) odscjames  (1000)        1 2022-10-26 11:26:54.000000 jsondataferret-0.7.0/jsondataferret.egg-info/dependency_links.txt
--rw-r--r--   0 odscjames  (1000) odscjames  (1000)     3205 2022-10-26 11:26:54.000000 jsondataferret-0.7.0/jsondataferret.egg-info/SOURCES.txt
--rw-r--r--   0 odscjames  (1000) odscjames  (1000)      156 2022-10-26 11:26:54.000000 jsondataferret-0.7.0/jsondataferret.egg-info/requires.txt
--rw-r--r--   0 odscjames  (1000) odscjames  (1000)       40 2022-10-26 11:26:54.000000 jsondataferret-0.7.0/jsondataferret.egg-info/top_level.txt
--rw-r--r--   0 odscjames  (1000) odscjames  (1000)      328 2022-10-26 11:26:54.000000 jsondataferret-0.7.0/jsondataferret.egg-info/PKG-INFO
--rw-r--r--   0 odscjames  (1000) odscjames  (1000)      148 2020-08-10 14:27:25.000000 jsondataferret-0.7.0/README.md
--rw-r--r--   0 odscjames  (1000) odscjames  (1000)       61 2022-10-26 11:26:54.000000 jsondataferret-0.7.0/setup.cfg
--rw-rw-r--   0 odscjames  (1000) odscjames  (1000)      969 2022-10-26 11:25:08.000000 jsondataferret-0.7.0/setup.py
--rw-r--r--   0 odscjames  (1000) odscjames  (1000)     1106 2020-05-21 15:56:04.000000 jsondataferret-0.7.0/LICENSE
-drwxrwxr-x   0 odscjames  (1000) odscjames  (1000)        0 2022-10-26 11:26:54.000000 jsondataferret-0.7.0/jsondataferretexampleapp/
--rw-rw-r--   0 odscjames  (1000) odscjames  (1000)      543 2022-05-27 12:19:37.000000 jsondataferret-0.7.0/jsondataferretexampleapp/forms.py
--rwxr-xr-x   0 odscjames  (1000) odscjames  (1000)       71 2020-05-21 15:56:03.000000 jsondataferret-0.7.0/jsondataferretexampleapp/admin.py
--rw-r--r--   0 odscjames  (1000) odscjames  (1000)     3142 2020-05-29 11:16:21.000000 jsondataferret-0.7.0/jsondataferretexampleapp/updatedata.py
--rwxrwxr-x   0 odscjames  (1000) odscjames  (1000)    16618 2022-06-09 12:48:41.000000 jsondataferret-0.7.0/jsondataferretexampleapp/views.py
--rw-rw-r--   0 odscjames  (1000) odscjames  (1000)     3681 2022-05-27 12:19:37.000000 jsondataferret-0.7.0/jsondataferretexampleapp/urls.py
--rwxrwxr-x   0 odscjames  (1000) odscjames  (1000)      177 2022-05-27 12:19:37.000000 jsondataferret-0.7.0/jsondataferretexampleapp/apps.py
--rw-r--r--   0 odscjames  (1000) odscjames  (1000)      346 2020-05-21 15:56:03.000000 jsondataferret-0.7.0/jsondataferretexampleapp/jsondataferret.py
--rwxr-xr-x   0 odscjames  (1000) odscjames  (1000)       68 2020-05-21 15:56:03.000000 jsondataferret-0.7.0/jsondataferretexampleapp/tests.py
--rwxrwxr-x   0 odscjames  (1000) odscjames  (1000)     1735 2022-05-27 12:19:37.000000 jsondataferret-0.7.0/jsondataferretexampleapp/models.py
--rwxr-xr-x   0 odscjames  (1000) odscjames  (1000)     1418 2020-05-28 09:58:06.000000 jsondataferret-0.7.0/jsondataferretexampleapp/__init__.py
-drwxrwxr-x   0 odscjames  (1000) odscjames  (1000)        0 2022-10-26 11:26:54.000000 jsondataferret-0.7.0/jsondataferretexampleapp/management/
-drwxrwxr-x   0 odscjames  (1000) odscjames  (1000)        0 2022-10-26 11:26:54.000000 jsondataferret-0.7.0/jsondataferretexampleapp/management/commands/
--rw-r--r--   0 odscjames  (1000) odscjames  (1000)      319 2020-05-21 15:56:03.000000 jsondataferret-0.7.0/jsondataferretexampleapp/management/commands/updatedata.py
--rw-r--r--   0 odscjames  (1000) odscjames  (1000)        0 2020-05-21 15:56:02.000000 jsondataferret-0.7.0/jsondataferretexampleapp/management/commands/__init__.py
--rw-r--r--   0 odscjames  (1000) odscjames  (1000)        0 2020-05-21 15:56:02.000000 jsondataferret-0.7.0/jsondataferretexampleapp/management/__init__.py
-drwxrwxr-x   0 odscjames  (1000) odscjames  (1000)        0 2022-10-26 11:26:54.000000 jsondataferret-0.7.0/jsondataferretexampleapp/migrations/
--rw-rw-r--   0 odscjames  (1000) odscjames  (1000)     2237 2022-05-27 12:19:37.000000 jsondataferret-0.7.0/jsondataferretexampleapp/migrations/0001_initial.py
--rwxr-xr-x   0 odscjames  (1000) odscjames  (1000)        0 2020-05-21 15:56:01.000000 jsondataferret-0.7.0/jsondataferretexampleapp/migrations/__init__.py
--rw-rw-r--   0 odscjames  (1000) odscjames  (1000)      884 2022-05-27 12:19:37.000000 jsondataferret-0.7.0/jsondataferretexampleapp/migrations/0002_auto_20220526_0940.py
-drwxrwxr-x   0 odscjames  (1000) odscjames  (1000)        0 2022-10-26 11:26:54.000000 jsondataferret-0.7.0/jsondataferret/
--rw-r--r--   0 odscjames  (1000) odscjames  (1000)      145 2020-05-29 15:46:45.000000 jsondataferret-0.7.0/jsondataferret/forms.py
--rwxrwxr-x   0 odscjames  (1000) odscjames  (1000)      778 2022-06-09 12:48:41.000000 jsondataferret-0.7.0/jsondataferret/filters.py
--rwxr-xr-x   0 odscjames  (1000) odscjames  (1000)       86 2020-05-21 15:56:01.000000 jsondataferret-0.7.0/jsondataferret/admin.py
--rwxrwxr-x   0 odscjames  (1000) odscjames  (1000)    14250 2022-06-15 07:47:42.000000 jsondataferret-0.7.0/jsondataferret/views.py
--rw-rw-r--   0 odscjames  (1000) odscjames  (1000)     1994 2022-06-10 12:27:41.000000 jsondataferret-0.7.0/jsondataferret/urls.py
--rwxrwxr-x   0 odscjames  (1000) odscjames  (1000)      157 2022-05-27 12:19:37.000000 jsondataferret-0.7.0/jsondataferret/apps.py
-drwxrwxr-x   0 odscjames  (1000) odscjames  (1000)        0 2022-10-26 11:26:54.000000 jsondataferret-0.7.0/jsondataferret/tests/
--rwxrwxr-x   0 odscjames  (1000) odscjames  (1000)     4781 2022-10-26 11:25:08.000000 jsondataferret-0.7.0/jsondataferret/tests/test_pythonapi_newevent.py
--rwxrwxr-x   0 odscjames  (1000) odscjames  (1000)     6169 2022-06-10 16:28:26.000000 jsondataferret-0.7.0/jsondataferret/tests/test_model_edit.py
--rw-r--r--   0 odscjames  (1000) odscjames  (1000)     1043 2021-01-06 11:41:02.000000 jsondataferret-0.7.0/jsondataferret/tests/test_purge_record.py
--rwxrwxr-x   0 odscjames  (1000) odscjames  (1000)     8132 2022-06-10 16:28:26.000000 jsondataferret-0.7.0/jsondataferret/tests/test_model_cachedrecordhistory.py
--rwxrwxr-x   0 odscjames  (1000) odscjames  (1000)     1985 2022-06-09 12:48:41.000000 jsondataferret-0.7.0/jsondataferret/tests/test_model_event.py
--rw-r--r--   0 odscjames  (1000) odscjames  (1000)        0 2020-06-10 12:38:17.000000 jsondataferret-0.7.0/jsondataferret/tests/__init__.py
--rwxrwxr-x   0 odscjames  (1000) odscjames  (1000)     3808 2022-06-10 16:28:26.000000 jsondataferret-0.7.0/jsondataferret/tests/test_model_record.py
--rw-rw-r--   0 odscjames  (1000) odscjames  (1000)     1354 2022-06-09 12:48:41.000000 jsondataferret-0.7.0/jsondataferret/tests/test_get_field_list_from_json.py
-drwxrwxr-x   0 odscjames  (1000) odscjames  (1000)        0 2022-10-26 11:26:54.000000 jsondataferret-0.7.0/jsondataferret/pythonapi/
--rw-rw-r--   0 odscjames  (1000) odscjames  (1000)     5079 2022-10-26 11:25:08.000000 jsondataferret-0.7.0/jsondataferret/pythonapi/newevent.py
--rw-r--r--   0 odscjames  (1000) odscjames  (1000)      751 2021-01-06 11:41:02.000000 jsondataferret-0.7.0/jsondataferret/pythonapi/purge.py
--rw-r--r--   0 odscjames  (1000) odscjames  (1000)        0 2020-05-21 15:56:02.000000 jsondataferret-0.7.0/jsondataferret/pythonapi/__init__.py
--rwxrwxr-x   0 odscjames  (1000) odscjames  (1000)     2401 2022-06-10 16:28:26.000000 jsondataferret-0.7.0/jsondataferret/pythonapi/runevents.py
-drwxrwxr-x   0 odscjames  (1000) odscjames  (1000)        0 2022-10-26 11:26:54.000000 jsondataferret-0.7.0/jsondataferret/templates/
-drwxrwxr-x   0 odscjames  (1000) odscjames  (1000)        0 2022-10-26 11:26:54.000000 jsondataferret-0.7.0/jsondataferret/templates/jsondataferret/
-drwxrwxr-x   0 odscjames  (1000) odscjames  (1000)        0 2022-10-26 11:26:54.000000 jsondataferret-0.7.0/jsondataferret/templates/jsondataferret/common/
--rw-rw-r--   0 odscjames  (1000) odscjames  (1000)      799 2022-06-09 12:48:41.000000 jsondataferret-0.7.0/jsondataferret/templates/jsondataferret/common/pagination.html
-drwxrwxr-x   0 odscjames  (1000) odscjames  (1000)        0 2022-10-26 11:26:54.000000 jsondataferret-0.7.0/jsondataferret/templates/jsondataferret/type/
--rw-r--r--   0 odscjames  (1000) odscjames  (1000)     1360 2020-08-14 10:54:47.000000 jsondataferret-0.7.0/jsondataferret/templates/jsondataferret/type/records.html
--rw-r--r--   0 odscjames  (1000) odscjames  (1000)      994 2020-06-12 15:03:16.000000 jsondataferret-0.7.0/jsondataferret/templates/jsondataferret/type/index.html
-drwxrwxr-x   0 odscjames  (1000) odscjames  (1000)        0 2022-10-26 11:26:54.000000 jsondataferret-0.7.0/jsondataferret/templates/jsondataferret/type/record/
--rw-rw-r--   0 odscjames  (1000) odscjames  (1000)     5199 2022-06-09 12:48:41.000000 jsondataferret-0.7.0/jsondataferret/templates/jsondataferret/type/record/moderate.html
--rw-r--r--   0 odscjames  (1000) odscjames  (1000)     2658 2020-06-12 16:07:24.000000 jsondataferret-0.7.0/jsondataferret/templates/jsondataferret/type/record/edit_json_schema.html
--rw-r--r--   0 odscjames  (1000) odscjames  (1000)      978 2020-06-12 15:03:16.000000 jsondataferret-0.7.0/jsondataferret/templates/jsondataferret/type/record/import_form.html
--rw-r--r--   0 odscjames  (1000) odscjames  (1000)     4368 2020-06-12 16:07:24.000000 jsondataferret-0.7.0/jsondataferret/templates/jsondataferret/type/record/index.html
--rw-r--r--   0 odscjames  (1000) odscjames  (1000)     1544 2020-06-12 15:03:16.000000 jsondataferret-0.7.0/jsondataferret/templates/jsondataferret/type/record/events.html
--rw-r--r--   0 odscjames  (1000) odscjames  (1000)     1380 2020-08-14 10:54:47.000000 jsondataferret-0.7.0/jsondataferret/templates/jsondataferret/type/records_needing_moderation.html
--rw-r--r--   0 odscjames  (1000) odscjames  (1000)      970 2020-06-12 15:03:16.000000 jsondataferret-0.7.0/jsondataferret/templates/jsondataferret/types.html
--rw-r--r--   0 odscjames  (1000) odscjames  (1000)      472 2020-06-12 15:03:16.000000 jsondataferret-0.7.0/jsondataferret/templates/jsondataferret/index.html
--rw-r--r--   0 odscjames  (1000) odscjames  (1000)     2009 2020-06-12 15:03:16.000000 jsondataferret-0.7.0/jsondataferret/templates/jsondataferret/base.html
--rw-rw-r--   0 odscjames  (1000) odscjames  (1000)     1994 2022-06-09 12:48:41.000000 jsondataferret-0.7.0/jsondataferret/templates/jsondataferret/events.html
-drwxrwxr-x   0 odscjames  (1000) odscjames  (1000)        0 2022-10-26 11:26:54.000000 jsondataferret-0.7.0/jsondataferret/templates/jsondataferret/edit/
--rw-rw-r--   0 odscjames  (1000) odscjames  (1000)     3039 2022-06-10 16:28:26.000000 jsondataferret-0.7.0/jsondataferret/templates/jsondataferret/edit/index_table_contents.html
--rw-rw-r--   0 odscjames  (1000) odscjames  (1000)     2166 2022-06-10 12:27:41.000000 jsondataferret-0.7.0/jsondataferret/templates/jsondataferret/edit/index.html
-drwxrwxr-x   0 odscjames  (1000) odscjames  (1000)        0 2022-10-26 11:26:54.000000 jsondataferret-0.7.0/jsondataferret/templates/jsondataferret/event/
--rw-rw-r--   0 odscjames  (1000) odscjames  (1000)    10323 2022-06-10 12:27:41.000000 jsondataferret-0.7.0/jsondataferret/templates/jsondataferret/event/index.html
--rwxrwxr-x   0 odscjames  (1000) odscjames  (1000)    15529 2022-06-24 15:11:57.000000 jsondataferret-0.7.0/jsondataferret/models.py
--rwxr-xr-x   0 odscjames  (1000) odscjames  (1000)       58 2020-05-21 15:56:03.000000 jsondataferret-0.7.0/jsondataferret/__init__.py
--rw-rw-r--   0 odscjames  (1000) odscjames  (1000)     3629 2022-06-10 16:28:26.000000 jsondataferret-0.7.0/jsondataferret/utils.py
-drwxrwxr-x   0 odscjames  (1000) odscjames  (1000)        0 2022-10-26 11:26:54.000000 jsondataferret-0.7.0/jsondataferret/management/
-drwxrwxr-x   0 odscjames  (1000) odscjames  (1000)        0 2022-10-26 11:26:54.000000 jsondataferret-0.7.0/jsondataferret/management/commands/
--rwxrwxrwx   0 odscjames  (1000) odscjames  (1000)     1305 2022-06-10 15:03:31.000000 jsondataferret-0.7.0/jsondataferret/management/commands/createtest1.py
--rw-r--r--   0 odscjames  (1000) odscjames  (1000)        0 2020-05-21 15:56:02.000000 jsondataferret-0.7.0/jsondataferret/management/commands/__init__.py
--rw-r--r--   0 odscjames  (1000) odscjames  (1000)      632 2021-01-06 11:41:02.000000 jsondataferret-0.7.0/jsondataferret/management/commands/purgerecord.py
--rw-r--r--   0 odscjames  (1000) odscjames  (1000)      336 2020-05-21 15:56:03.000000 jsondataferret-0.7.0/jsondataferret/management/commands/runeventstreamtodatabase.py
--rw-rw-r--   0 odscjames  (1000) odscjames  (1000)     1639 2022-06-02 11:04:32.000000 jsondataferret-0.7.0/jsondataferret/management/commands/createtest.py
--rw-r--r--   0 odscjames  (1000) odscjames  (1000)      699 2020-07-02 13:20:27.000000 jsondataferret-0.7.0/jsondataferret/management/commands/updatejsonschemavalidations.py
--rw-r--r--   0 odscjames  (1000) odscjames  (1000)        0 2020-05-21 15:56:02.000000 jsondataferret-0.7.0/jsondataferret/management/__init__.py
-drwxrwxr-x   0 odscjames  (1000) odscjames  (1000)        0 2022-10-26 11:26:54.000000 jsondataferret-0.7.0/jsondataferret/migrations/
--rwxrwxr-x   0 odscjames  (1000) odscjames  (1000)     1291 2022-06-10 12:27:41.000000 jsondataferret-0.7.0/jsondataferret/migrations/0004_auto_20220603_0827.py
--rw-r--r--   0 odscjames  (1000) odscjames  (1000)      840 2020-05-29 11:16:21.000000 jsondataferret-0.7.0/jsondataferret/migrations/0002_jsondataferret.py
--rw-rw-r--   0 odscjames  (1000) odscjames  (1000)     5206 2022-05-27 12:19:37.000000 jsondataferret-0.7.0/jsondataferret/migrations/0001_initial.py
--rwxr-xr-x   0 odscjames  (1000) odscjames  (1000)        0 2020-05-21 15:56:01.000000 jsondataferret-0.7.0/jsondataferret/migrations/__init__.py
--rw-rw-r--   0 odscjames  (1000) odscjames  (1000)      732 2022-05-27 12:19:37.000000 jsondataferret-0.7.0/jsondataferret/migrations/0003_auto_20220526_0923.py
--rw-rw-r--   0 odscjames  (1000) odscjames  (1000)      328 2022-10-26 11:26:54.000000 jsondataferret-0.7.0/PKG-INFO
+drwxrwxr-x   0 bjwebb    (1000) bjwebb    (1000)        0 2024-05-29 12:09:55.756866 jsondataferret-0.7.1/
+-rw-rw-r--   0 bjwebb    (1000) bjwebb    (1000)     1106 2024-05-29 12:08:43.000000 jsondataferret-0.7.1/LICENSE
+-rw-rw-r--   0 bjwebb    (1000) bjwebb    (1000)      339 2024-05-29 12:09:55.756866 jsondataferret-0.7.1/PKG-INFO
+-rw-rw-r--   0 bjwebb    (1000) bjwebb    (1000)      148 2024-05-29 12:08:43.000000 jsondataferret-0.7.1/README.md
+drwxrwxr-x   0 bjwebb    (1000) bjwebb    (1000)        0 2024-05-29 12:09:55.752866 jsondataferret-0.7.1/jsondataferret/
+-rwxrwxr-x   0 bjwebb    (1000) bjwebb    (1000)       58 2024-05-29 12:08:43.000000 jsondataferret-0.7.1/jsondataferret/__init__.py
+-rwxrwxr-x   0 bjwebb    (1000) bjwebb    (1000)       86 2024-05-29 12:08:43.000000 jsondataferret-0.7.1/jsondataferret/admin.py
+-rwxrwxr-x   0 bjwebb    (1000) bjwebb    (1000)      157 2024-05-29 12:08:43.000000 jsondataferret-0.7.1/jsondataferret/apps.py
+-rwxrwxr-x   0 bjwebb    (1000) bjwebb    (1000)      778 2024-05-29 12:08:43.000000 jsondataferret-0.7.1/jsondataferret/filters.py
+-rw-rw-r--   0 bjwebb    (1000) bjwebb    (1000)      145 2024-05-29 12:08:43.000000 jsondataferret-0.7.1/jsondataferret/forms.py
+drwxrwxr-x   0 bjwebb    (1000) bjwebb    (1000)        0 2024-05-29 12:09:55.752866 jsondataferret-0.7.1/jsondataferret/management/
+-rw-rw-r--   0 bjwebb    (1000) bjwebb    (1000)        0 2024-05-29 12:08:43.000000 jsondataferret-0.7.1/jsondataferret/management/__init__.py
+drwxrwxr-x   0 bjwebb    (1000) bjwebb    (1000)        0 2024-05-29 12:09:55.752866 jsondataferret-0.7.1/jsondataferret/management/commands/
+-rw-rw-r--   0 bjwebb    (1000) bjwebb    (1000)        0 2024-05-29 12:08:43.000000 jsondataferret-0.7.1/jsondataferret/management/commands/__init__.py
+-rw-rw-r--   0 bjwebb    (1000) bjwebb    (1000)      632 2024-05-29 12:08:43.000000 jsondataferret-0.7.1/jsondataferret/management/commands/purgerecord.py
+-rw-rw-r--   0 bjwebb    (1000) bjwebb    (1000)      336 2024-05-29 12:08:43.000000 jsondataferret-0.7.1/jsondataferret/management/commands/runeventstreamtodatabase.py
+-rw-rw-r--   0 bjwebb    (1000) bjwebb    (1000)      699 2024-05-29 12:08:43.000000 jsondataferret-0.7.1/jsondataferret/management/commands/updatejsonschemavalidations.py
+drwxrwxr-x   0 bjwebb    (1000) bjwebb    (1000)        0 2024-05-29 12:09:55.752866 jsondataferret-0.7.1/jsondataferret/migrations/
+-rw-rw-r--   0 bjwebb    (1000) bjwebb    (1000)     5206 2024-05-29 12:08:43.000000 jsondataferret-0.7.1/jsondataferret/migrations/0001_initial.py
+-rw-rw-r--   0 bjwebb    (1000) bjwebb    (1000)      840 2024-05-29 12:08:43.000000 jsondataferret-0.7.1/jsondataferret/migrations/0002_jsondataferret.py
+-rw-rw-r--   0 bjwebb    (1000) bjwebb    (1000)      732 2024-05-29 12:08:43.000000 jsondataferret-0.7.1/jsondataferret/migrations/0003_auto_20220526_0923.py
+-rwxrwxr-x   0 bjwebb    (1000) bjwebb    (1000)     1291 2024-05-29 12:08:43.000000 jsondataferret-0.7.1/jsondataferret/migrations/0004_auto_20220603_0827.py
+-rwxrwxr-x   0 bjwebb    (1000) bjwebb    (1000)        0 2024-05-29 12:08:43.000000 jsondataferret-0.7.1/jsondataferret/migrations/__init__.py
+-rwxrwxr-x   0 bjwebb    (1000) bjwebb    (1000)    15530 2024-05-29 12:08:43.000000 jsondataferret-0.7.1/jsondataferret/models.py
+drwxrwxr-x   0 bjwebb    (1000) bjwebb    (1000)        0 2024-05-29 12:09:55.752866 jsondataferret-0.7.1/jsondataferret/pythonapi/
+-rw-rw-r--   0 bjwebb    (1000) bjwebb    (1000)        0 2024-05-29 12:08:43.000000 jsondataferret-0.7.1/jsondataferret/pythonapi/__init__.py
+-rw-rw-r--   0 bjwebb    (1000) bjwebb    (1000)     5079 2024-05-29 12:08:43.000000 jsondataferret-0.7.1/jsondataferret/pythonapi/newevent.py
+-rw-rw-r--   0 bjwebb    (1000) bjwebb    (1000)      751 2024-05-29 12:08:43.000000 jsondataferret-0.7.1/jsondataferret/pythonapi/purge.py
+-rwxrwxr-x   0 bjwebb    (1000) bjwebb    (1000)     2401 2024-05-29 12:08:43.000000 jsondataferret-0.7.1/jsondataferret/pythonapi/runevents.py
+drwxrwxr-x   0 bjwebb    (1000) bjwebb    (1000)        0 2024-05-29 12:09:55.752866 jsondataferret-0.7.1/jsondataferret/templates/
+drwxrwxr-x   0 bjwebb    (1000) bjwebb    (1000)        0 2024-05-29 12:09:55.756866 jsondataferret-0.7.1/jsondataferret/templates/jsondataferret/
+-rw-rw-r--   0 bjwebb    (1000) bjwebb    (1000)     2009 2024-05-29 12:08:43.000000 jsondataferret-0.7.1/jsondataferret/templates/jsondataferret/base.html
+drwxrwxr-x   0 bjwebb    (1000) bjwebb    (1000)        0 2024-05-29 12:09:55.756866 jsondataferret-0.7.1/jsondataferret/templates/jsondataferret/common/
+-rw-rw-r--   0 bjwebb    (1000) bjwebb    (1000)      799 2024-05-29 12:08:43.000000 jsondataferret-0.7.1/jsondataferret/templates/jsondataferret/common/pagination.html
+drwxrwxr-x   0 bjwebb    (1000) bjwebb    (1000)        0 2024-05-29 12:09:55.756866 jsondataferret-0.7.1/jsondataferret/templates/jsondataferret/edit/
+-rw-rw-r--   0 bjwebb    (1000) bjwebb    (1000)     2166 2024-05-29 12:08:43.000000 jsondataferret-0.7.1/jsondataferret/templates/jsondataferret/edit/index.html
+-rw-rw-r--   0 bjwebb    (1000) bjwebb    (1000)     3039 2024-05-29 12:08:43.000000 jsondataferret-0.7.1/jsondataferret/templates/jsondataferret/edit/index_table_contents.html
+drwxrwxr-x   0 bjwebb    (1000) bjwebb    (1000)        0 2024-05-29 12:09:55.756866 jsondataferret-0.7.1/jsondataferret/templates/jsondataferret/event/
+-rw-rw-r--   0 bjwebb    (1000) bjwebb    (1000)    10323 2024-05-29 12:08:43.000000 jsondataferret-0.7.1/jsondataferret/templates/jsondataferret/event/index.html
+-rw-rw-r--   0 bjwebb    (1000) bjwebb    (1000)     1994 2024-05-29 12:08:43.000000 jsondataferret-0.7.1/jsondataferret/templates/jsondataferret/events.html
+-rw-rw-r--   0 bjwebb    (1000) bjwebb    (1000)      472 2024-05-29 12:08:43.000000 jsondataferret-0.7.1/jsondataferret/templates/jsondataferret/index.html
+drwxrwxr-x   0 bjwebb    (1000) bjwebb    (1000)        0 2024-05-29 12:09:55.756866 jsondataferret-0.7.1/jsondataferret/templates/jsondataferret/type/
+-rw-rw-r--   0 bjwebb    (1000) bjwebb    (1000)      994 2024-05-29 12:08:43.000000 jsondataferret-0.7.1/jsondataferret/templates/jsondataferret/type/index.html
+drwxrwxr-x   0 bjwebb    (1000) bjwebb    (1000)        0 2024-05-29 12:09:55.756866 jsondataferret-0.7.1/jsondataferret/templates/jsondataferret/type/record/
+-rw-rw-r--   0 bjwebb    (1000) bjwebb    (1000)     2658 2024-05-29 12:08:43.000000 jsondataferret-0.7.1/jsondataferret/templates/jsondataferret/type/record/edit_json_schema.html
+-rw-rw-r--   0 bjwebb    (1000) bjwebb    (1000)     1544 2024-05-29 12:08:43.000000 jsondataferret-0.7.1/jsondataferret/templates/jsondataferret/type/record/events.html
+-rw-rw-r--   0 bjwebb    (1000) bjwebb    (1000)      978 2024-05-29 12:08:43.000000 jsondataferret-0.7.1/jsondataferret/templates/jsondataferret/type/record/import_form.html
+-rw-rw-r--   0 bjwebb    (1000) bjwebb    (1000)     4368 2024-05-29 12:08:43.000000 jsondataferret-0.7.1/jsondataferret/templates/jsondataferret/type/record/index.html
+-rw-rw-r--   0 bjwebb    (1000) bjwebb    (1000)     5199 2024-05-29 12:08:43.000000 jsondataferret-0.7.1/jsondataferret/templates/jsondataferret/type/record/moderate.html
+-rw-rw-r--   0 bjwebb    (1000) bjwebb    (1000)     1360 2024-05-29 12:08:43.000000 jsondataferret-0.7.1/jsondataferret/templates/jsondataferret/type/records.html
+-rw-rw-r--   0 bjwebb    (1000) bjwebb    (1000)     1380 2024-05-29 12:08:43.000000 jsondataferret-0.7.1/jsondataferret/templates/jsondataferret/type/records_needing_moderation.html
+-rw-rw-r--   0 bjwebb    (1000) bjwebb    (1000)      970 2024-05-29 12:08:43.000000 jsondataferret-0.7.1/jsondataferret/templates/jsondataferret/types.html
+drwxrwxr-x   0 bjwebb    (1000) bjwebb    (1000)        0 2024-05-29 12:09:55.756866 jsondataferret-0.7.1/jsondataferret/tests/
+-rw-rw-r--   0 bjwebb    (1000) bjwebb    (1000)        0 2024-05-29 12:08:43.000000 jsondataferret-0.7.1/jsondataferret/tests/__init__.py
+-rw-rw-r--   0 bjwebb    (1000) bjwebb    (1000)     1354 2024-05-29 12:08:43.000000 jsondataferret-0.7.1/jsondataferret/tests/test_get_field_list_from_json.py
+-rwxrwxr-x   0 bjwebb    (1000) bjwebb    (1000)     8132 2024-05-29 12:08:43.000000 jsondataferret-0.7.1/jsondataferret/tests/test_model_cachedrecordhistory.py
+-rwxrwxr-x   0 bjwebb    (1000) bjwebb    (1000)     6169 2024-05-29 12:08:43.000000 jsondataferret-0.7.1/jsondataferret/tests/test_model_edit.py
+-rwxrwxr-x   0 bjwebb    (1000) bjwebb    (1000)     1985 2024-05-29 12:08:43.000000 jsondataferret-0.7.1/jsondataferret/tests/test_model_event.py
+-rwxrwxr-x   0 bjwebb    (1000) bjwebb    (1000)     3808 2024-05-29 12:08:43.000000 jsondataferret-0.7.1/jsondataferret/tests/test_model_record.py
+-rw-rw-r--   0 bjwebb    (1000) bjwebb    (1000)     1043 2024-05-29 12:08:43.000000 jsondataferret-0.7.1/jsondataferret/tests/test_purge_record.py
+-rwxrwxr-x   0 bjwebb    (1000) bjwebb    (1000)     4781 2024-05-29 12:08:43.000000 jsondataferret-0.7.1/jsondataferret/tests/test_pythonapi_newevent.py
+-rw-rw-r--   0 bjwebb    (1000) bjwebb    (1000)     1994 2024-05-29 12:08:43.000000 jsondataferret-0.7.1/jsondataferret/urls.py
+-rw-rw-r--   0 bjwebb    (1000) bjwebb    (1000)     3629 2024-05-29 12:08:43.000000 jsondataferret-0.7.1/jsondataferret/utils.py
+-rwxrwxr-x   0 bjwebb    (1000) bjwebb    (1000)    14250 2024-05-29 12:08:43.000000 jsondataferret-0.7.1/jsondataferret/views.py
+drwxrwxr-x   0 bjwebb    (1000) bjwebb    (1000)        0 2024-05-29 12:09:55.752866 jsondataferret-0.7.1/jsondataferret.egg-info/
+-rw-rw-r--   0 bjwebb    (1000) bjwebb    (1000)      339 2024-05-29 12:09:55.000000 jsondataferret-0.7.1/jsondataferret.egg-info/PKG-INFO
+-rw-rw-r--   0 bjwebb    (1000) bjwebb    (1000)     3106 2024-05-29 12:09:55.000000 jsondataferret-0.7.1/jsondataferret.egg-info/SOURCES.txt
+-rw-rw-r--   0 bjwebb    (1000) bjwebb    (1000)        1 2024-05-29 12:09:55.000000 jsondataferret-0.7.1/jsondataferret.egg-info/dependency_links.txt
+-rw-rw-r--   0 bjwebb    (1000) bjwebb    (1000)      156 2024-05-29 12:09:55.000000 jsondataferret-0.7.1/jsondataferret.egg-info/requires.txt
+-rw-rw-r--   0 bjwebb    (1000) bjwebb    (1000)       40 2024-05-29 12:09:55.000000 jsondataferret-0.7.1/jsondataferret.egg-info/top_level.txt
+drwxrwxr-x   0 bjwebb    (1000) bjwebb    (1000)        0 2024-05-29 12:09:55.756866 jsondataferret-0.7.1/jsondataferretexampleapp/
+-rwxrwxr-x   0 bjwebb    (1000) bjwebb    (1000)     1418 2024-05-29 12:08:43.000000 jsondataferret-0.7.1/jsondataferretexampleapp/__init__.py
+-rwxrwxr-x   0 bjwebb    (1000) bjwebb    (1000)       71 2024-05-29 12:08:43.000000 jsondataferret-0.7.1/jsondataferretexampleapp/admin.py
+-rwxrwxr-x   0 bjwebb    (1000) bjwebb    (1000)      177 2024-05-29 12:08:43.000000 jsondataferret-0.7.1/jsondataferretexampleapp/apps.py
+-rw-rw-r--   0 bjwebb    (1000) bjwebb    (1000)      543 2024-05-29 12:08:43.000000 jsondataferret-0.7.1/jsondataferretexampleapp/forms.py
+-rw-rw-r--   0 bjwebb    (1000) bjwebb    (1000)      346 2024-05-29 12:08:43.000000 jsondataferret-0.7.1/jsondataferretexampleapp/jsondataferret.py
+drwxrwxr-x   0 bjwebb    (1000) bjwebb    (1000)        0 2024-05-29 12:09:55.756866 jsondataferret-0.7.1/jsondataferretexampleapp/management/
+-rw-rw-r--   0 bjwebb    (1000) bjwebb    (1000)        0 2024-05-29 12:08:43.000000 jsondataferret-0.7.1/jsondataferretexampleapp/management/__init__.py
+drwxrwxr-x   0 bjwebb    (1000) bjwebb    (1000)        0 2024-05-29 12:09:55.756866 jsondataferret-0.7.1/jsondataferretexampleapp/management/commands/
+-rw-rw-r--   0 bjwebb    (1000) bjwebb    (1000)        0 2024-05-29 12:08:43.000000 jsondataferret-0.7.1/jsondataferretexampleapp/management/commands/__init__.py
+-rw-rw-r--   0 bjwebb    (1000) bjwebb    (1000)      319 2024-05-29 12:08:43.000000 jsondataferret-0.7.1/jsondataferretexampleapp/management/commands/updatedata.py
+drwxrwxr-x   0 bjwebb    (1000) bjwebb    (1000)        0 2024-05-29 12:09:55.756866 jsondataferret-0.7.1/jsondataferretexampleapp/migrations/
+-rw-rw-r--   0 bjwebb    (1000) bjwebb    (1000)     2237 2024-05-29 12:08:43.000000 jsondataferret-0.7.1/jsondataferretexampleapp/migrations/0001_initial.py
+-rw-rw-r--   0 bjwebb    (1000) bjwebb    (1000)      884 2024-05-29 12:08:43.000000 jsondataferret-0.7.1/jsondataferretexampleapp/migrations/0002_auto_20220526_0940.py
+-rwxrwxr-x   0 bjwebb    (1000) bjwebb    (1000)        0 2024-05-29 12:08:43.000000 jsondataferret-0.7.1/jsondataferretexampleapp/migrations/__init__.py
+-rwxrwxr-x   0 bjwebb    (1000) bjwebb    (1000)     1735 2024-05-29 12:08:43.000000 jsondataferret-0.7.1/jsondataferretexampleapp/models.py
+-rwxrwxr-x   0 bjwebb    (1000) bjwebb    (1000)       68 2024-05-29 12:08:43.000000 jsondataferret-0.7.1/jsondataferretexampleapp/tests.py
+-rw-rw-r--   0 bjwebb    (1000) bjwebb    (1000)     3142 2024-05-29 12:08:43.000000 jsondataferret-0.7.1/jsondataferretexampleapp/updatedata.py
+-rw-rw-r--   0 bjwebb    (1000) bjwebb    (1000)     3681 2024-05-29 12:08:43.000000 jsondataferret-0.7.1/jsondataferretexampleapp/urls.py
+-rwxrwxr-x   0 bjwebb    (1000) bjwebb    (1000)    16618 2024-05-29 12:08:43.000000 jsondataferret-0.7.1/jsondataferretexampleapp/views.py
+-rw-rw-r--   0 bjwebb    (1000) bjwebb    (1000)       61 2024-05-29 12:09:55.756866 jsondataferret-0.7.1/setup.cfg
+-rw-rw-r--   0 bjwebb    (1000) bjwebb    (1000)      969 2024-05-29 12:08:43.000000 jsondataferret-0.7.1/setup.py
```

### filetype from file(1)

```diff
@@ -1 +1 @@
-POSIX tar archive (GNU)
+POSIX tar archive
```

### Comparing `jsondataferret-0.7.0/jsondataferret.egg-info/SOURCES.txt` & `jsondataferret-0.7.1/jsondataferret.egg-info/SOURCES.txt`

 * *Files 1% similar despite different names*

```diff
@@ -14,16 +14,14 @@
 jsondataferret.egg-info/PKG-INFO
 jsondataferret.egg-info/SOURCES.txt
 jsondataferret.egg-info/dependency_links.txt
 jsondataferret.egg-info/requires.txt
 jsondataferret.egg-info/top_level.txt
 jsondataferret/management/__init__.py
 jsondataferret/management/commands/__init__.py
-jsondataferret/management/commands/createtest.py
-jsondataferret/management/commands/createtest1.py
 jsondataferret/management/commands/purgerecord.py
 jsondataferret/management/commands/runeventstreamtodatabase.py
 jsondataferret/management/commands/updatejsonschemavalidations.py
 jsondataferret/migrations/0001_initial.py
 jsondataferret/migrations/0002_jsondataferret.py
 jsondataferret/migrations/0003_auto_20220526_0923.py
 jsondataferret/migrations/0004_auto_20220603_0827.py
```

### Comparing `jsondataferret-0.7.0/setup.py` & `jsondataferret-0.7.1/setup.py`

 * *Files 11% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from setuptools import find_packages, setup
 
 setup(
     name="jsondataferret",
-    version="0.7.0",
+    version="0.7.1",
     author="Open Data Services",
     author_email="code@opendataservices.coop",
     packages=[p for p in find_packages() if p.startswith("jsondataferret")],
     package_data={
         "jsondataferret": [
             "templates/*",
             "templates/*/*",
```

### Comparing `jsondataferret-0.7.0/LICENSE` & `jsondataferret-0.7.1/LICENSE`

 * *Files identical despite different names*

### Comparing `jsondataferret-0.7.0/jsondataferretexampleapp/forms.py` & `jsondataferret-0.7.1/jsondataferretexampleapp/forms.py`

 * *Files identical despite different names*

### Comparing `jsondataferret-0.7.0/jsondataferretexampleapp/updatedata.py` & `jsondataferret-0.7.1/jsondataferretexampleapp/updatedata.py`

 * *Files identical despite different names*

### Comparing `jsondataferret-0.7.0/jsondataferretexampleapp/views.py` & `jsondataferret-0.7.1/jsondataferretexampleapp/views.py`

 * *Files identical despite different names*

### Comparing `jsondataferret-0.7.0/jsondataferretexampleapp/urls.py` & `jsondataferret-0.7.1/jsondataferretexampleapp/urls.py`

 * *Files identical despite different names*

### Comparing `jsondataferret-0.7.0/jsondataferretexampleapp/models.py` & `jsondataferret-0.7.1/jsondataferretexampleapp/models.py`

 * *Files identical despite different names*

### Comparing `jsondataferret-0.7.0/jsondataferretexampleapp/__init__.py` & `jsondataferret-0.7.1/jsondataferretexampleapp/__init__.py`

 * *Files identical despite different names*

### Comparing `jsondataferret-0.7.0/jsondataferretexampleapp/migrations/0001_initial.py` & `jsondataferret-0.7.1/jsondataferretexampleapp/migrations/0001_initial.py`

 * *Files identical despite different names*

### Comparing `jsondataferret-0.7.0/jsondataferretexampleapp/migrations/0002_auto_20220526_0940.py` & `jsondataferret-0.7.1/jsondataferretexampleapp/migrations/0002_auto_20220526_0940.py`

 * *Files identical despite different names*

### Comparing `jsondataferret-0.7.0/jsondataferret/filters.py` & `jsondataferret-0.7.1/jsondataferret/filters.py`

 * *Files identical despite different names*

### Comparing `jsondataferret-0.7.0/jsondataferret/views.py` & `jsondataferret-0.7.1/jsondataferret/views.py`

 * *Files identical despite different names*

### Comparing `jsondataferret-0.7.0/jsondataferret/urls.py` & `jsondataferret-0.7.1/jsondataferret/urls.py`

 * *Files identical despite different names*

### Comparing `jsondataferret-0.7.0/jsondataferret/tests/test_pythonapi_newevent.py` & `jsondataferret-0.7.1/jsondataferret/tests/test_pythonapi_newevent.py`

 * *Files identical despite different names*

### Comparing `jsondataferret-0.7.0/jsondataferret/tests/test_model_edit.py` & `jsondataferret-0.7.1/jsondataferret/tests/test_model_edit.py`

 * *Files identical despite different names*

### Comparing `jsondataferret-0.7.0/jsondataferret/tests/test_purge_record.py` & `jsondataferret-0.7.1/jsondataferret/tests/test_purge_record.py`

 * *Files identical despite different names*

### Comparing `jsondataferret-0.7.0/jsondataferret/tests/test_model_cachedrecordhistory.py` & `jsondataferret-0.7.1/jsondataferret/tests/test_model_cachedrecordhistory.py`

 * *Files identical despite different names*

### Comparing `jsondataferret-0.7.0/jsondataferret/tests/test_model_event.py` & `jsondataferret-0.7.1/jsondataferret/tests/test_model_event.py`

 * *Files identical despite different names*

### Comparing `jsondataferret-0.7.0/jsondataferret/tests/test_model_record.py` & `jsondataferret-0.7.1/jsondataferret/tests/test_model_record.py`

 * *Files identical despite different names*

### Comparing `jsondataferret-0.7.0/jsondataferret/tests/test_get_field_list_from_json.py` & `jsondataferret-0.7.1/jsondataferret/tests/test_get_field_list_from_json.py`

 * *Files identical despite different names*

### Comparing `jsondataferret-0.7.0/jsondataferret/pythonapi/newevent.py` & `jsondataferret-0.7.1/jsondataferret/pythonapi/newevent.py`

 * *Files identical despite different names*

### Comparing `jsondataferret-0.7.0/jsondataferret/pythonapi/purge.py` & `jsondataferret-0.7.1/jsondataferret/pythonapi/purge.py`

 * *Files identical despite different names*

### Comparing `jsondataferret-0.7.0/jsondataferret/pythonapi/runevents.py` & `jsondataferret-0.7.1/jsondataferret/pythonapi/runevents.py`

 * *Files identical despite different names*

### Comparing `jsondataferret-0.7.0/jsondataferret/templates/jsondataferret/common/pagination.html` & `jsondataferret-0.7.1/jsondataferret/templates/jsondataferret/common/pagination.html`

 * *Files identical despite different names*

### Comparing `jsondataferret-0.7.0/jsondataferret/templates/jsondataferret/type/records.html` & `jsondataferret-0.7.1/jsondataferret/templates/jsondataferret/type/records.html`

 * *Files identical despite different names*

### Comparing `jsondataferret-0.7.0/jsondataferret/templates/jsondataferret/type/index.html` & `jsondataferret-0.7.1/jsondataferret/templates/jsondataferret/type/index.html`

 * *Files identical despite different names*

### Comparing `jsondataferret-0.7.0/jsondataferret/templates/jsondataferret/type/record/moderate.html` & `jsondataferret-0.7.1/jsondataferret/templates/jsondataferret/type/record/moderate.html`

 * *Files identical despite different names*

### Comparing `jsondataferret-0.7.0/jsondataferret/templates/jsondataferret/type/record/edit_json_schema.html` & `jsondataferret-0.7.1/jsondataferret/templates/jsondataferret/type/record/edit_json_schema.html`

 * *Files identical despite different names*

### Comparing `jsondataferret-0.7.0/jsondataferret/templates/jsondataferret/type/record/import_form.html` & `jsondataferret-0.7.1/jsondataferret/templates/jsondataferret/type/record/import_form.html`

 * *Files identical despite different names*

### Comparing `jsondataferret-0.7.0/jsondataferret/templates/jsondataferret/type/record/index.html` & `jsondataferret-0.7.1/jsondataferret/templates/jsondataferret/type/record/index.html`

 * *Files identical despite different names*

### Comparing `jsondataferret-0.7.0/jsondataferret/templates/jsondataferret/type/record/events.html` & `jsondataferret-0.7.1/jsondataferret/templates/jsondataferret/type/record/events.html`

 * *Files identical despite different names*

### Comparing `jsondataferret-0.7.0/jsondataferret/templates/jsondataferret/type/records_needing_moderation.html` & `jsondataferret-0.7.1/jsondataferret/templates/jsondataferret/type/records_needing_moderation.html`

 * *Files identical despite different names*

### Comparing `jsondataferret-0.7.0/jsondataferret/templates/jsondataferret/types.html` & `jsondataferret-0.7.1/jsondataferret/templates/jsondataferret/types.html`

 * *Files identical despite different names*

### Comparing `jsondataferret-0.7.0/jsondataferret/templates/jsondataferret/base.html` & `jsondataferret-0.7.1/jsondataferret/templates/jsondataferret/base.html`

 * *Files identical despite different names*

### Comparing `jsondataferret-0.7.0/jsondataferret/templates/jsondataferret/events.html` & `jsondataferret-0.7.1/jsondataferret/templates/jsondataferret/events.html`

 * *Files identical despite different names*

### Comparing `jsondataferret-0.7.0/jsondataferret/templates/jsondataferret/edit/index_table_contents.html` & `jsondataferret-0.7.1/jsondataferret/templates/jsondataferret/edit/index_table_contents.html`

 * *Files identical despite different names*

### Comparing `jsondataferret-0.7.0/jsondataferret/templates/jsondataferret/edit/index.html` & `jsondataferret-0.7.1/jsondataferret/templates/jsondataferret/edit/index.html`

 * *Files identical despite different names*

### Comparing `jsondataferret-0.7.0/jsondataferret/templates/jsondataferret/event/index.html` & `jsondataferret-0.7.1/jsondataferret/templates/jsondataferret/event/index.html`

 * *Files identical despite different names*

### Comparing `jsondataferret-0.7.0/jsondataferret/models.py` & `jsondataferret-0.7.1/jsondataferret/models.py`

 * *Files 1% similar despite different names*

```diff
@@ -124,15 +124,15 @@
             "SELECT jsondataferret_record.id, jsondataferret_record.public_id, "
             + "max(jsondataferret_type.public_id) AS type_public_id, max(jsondataferret_type.title) AS type_title  FROM jsondataferret_record "
             + "JOIN jsondataferret_edit ON jsondataferret_edit.record_id = jsondataferret_record.id "
             + "JOIN jsondataferret_type ON jsondataferret_record.type_id = jsondataferret_type.id "
             + (
                 "WHERE jsondataferret_edit.approval_event_id = %(event_id)s "
                 if approved_edits_only
-                else "WHERE jsondataferret_edit.creation_event_id = %(event_id)s OR jsondataferret_edit.refusal_event_id = %(event_id)s OR jsondataferret_edit.approval_event_id = %(event_id)s"
+                else "WHERE jsondataferret_edit.creation_event_id = %(event_id)s OR jsondataferret_edit.refusal_event_id = %(event_id)s OR jsondataferret_edit.approval_event_id = %(event_id)s "
             )
             + "GROUP BY jsondataferret_record.id "
             + "ORDER BY max(jsondataferret_type.title) ASC,  jsondataferret_record.public_id ASC"
         )
         params = {"event_id": self.id}
         if int(limit) > 0:
             sql += " LIMIT %(limit)s"
```

### Comparing `jsondataferret-0.7.0/jsondataferret/utils.py` & `jsondataferret-0.7.1/jsondataferret/utils.py`

 * *Files identical despite different names*

### Comparing `jsondataferret-0.7.0/jsondataferret/management/commands/purgerecord.py` & `jsondataferret-0.7.1/jsondataferret/management/commands/purgerecord.py`

 * *Files identical despite different names*

### Comparing `jsondataferret-0.7.0/jsondataferret/management/commands/updatejsonschemavalidations.py` & `jsondataferret-0.7.1/jsondataferret/management/commands/updatejsonschemavalidations.py`

 * *Files identical despite different names*

### Comparing `jsondataferret-0.7.0/jsondataferret/migrations/0004_auto_20220603_0827.py` & `jsondataferret-0.7.1/jsondataferret/migrations/0004_auto_20220603_0827.py`

 * *Files identical despite different names*

### Comparing `jsondataferret-0.7.0/jsondataferret/migrations/0002_jsondataferret.py` & `jsondataferret-0.7.1/jsondataferret/migrations/0002_jsondataferret.py`

 * *Files identical despite different names*

### Comparing `jsondataferret-0.7.0/jsondataferret/migrations/0001_initial.py` & `jsondataferret-0.7.1/jsondataferret/migrations/0001_initial.py`

 * *Files identical despite different names*

### Comparing `jsondataferret-0.7.0/jsondataferret/migrations/0003_auto_20220526_0923.py` & `jsondataferret-0.7.1/jsondataferret/migrations/0003_auto_20220526_0923.py`

 * *Files identical despite different names*

