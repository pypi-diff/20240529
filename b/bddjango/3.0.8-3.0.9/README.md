# Comparing `tmp/bddjango-3.0.8.tar.gz` & `tmp/bddjango-3.0.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/bddjango-3.0.8.tar", last modified: Tue Feb 20 09:29:44 2024, max compression
+gzip compressed data, was "bddjango-3.0.9.tar", last modified: Wed May 29 08:47:22 2024, max compression
```

## Comparing `bddjango-3.0.8.tar` & `bddjango-3.0.9.tar`

### file list

```diff
@@ -1,83 +1,87 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-02-20 09:29:44.000000 bddjango-3.0.8/
--rw-r--r--   0 root         (0) root         (0)     1141 2024-02-20 09:29:13.000000 bddjango-3.0.8/setup.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-02-20 09:29:44.000000 bddjango-3.0.8/bddjango/
--rw-r--r--   0 root         (0) root         (0)    15976 2024-02-20 09:29:13.000000 bddjango-3.0.8/bddjango/MultipleConditionSearch.py
--rw-r--r--   0 root         (0) root         (0)      271 2024-02-20 09:29:13.000000 bddjango-3.0.8/bddjango/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-02-20 09:29:44.000000 bddjango-3.0.8/bddjango/tools/
--rw-r--r--   0 root         (0) root         (0)      393 2024-02-20 09:29:13.000000 bddjango-3.0.8/bddjango/tools/__init__.py
--rw-r--r--   0 root         (0) root         (0)     1248 2024-02-20 09:29:13.000000 bddjango-3.0.8/bddjango/tools/extractPdf.py
--rw-r--r--   0 root         (0) root         (0)      908 2024-02-20 09:29:13.000000 bddjango-3.0.8/bddjango/tools/nginx_config.py
--rw-r--r--   0 root         (0) root         (0)     4162 2024-02-20 09:29:13.000000 bddjango-3.0.8/bddjango/tools/zipDir.py
--rw-r--r--   0 root         (0) root         (0)     2452 2024-02-20 09:29:13.000000 bddjango-3.0.8/bddjango/tools/getshells.py
--rw-r--r--   0 root         (0) root         (0)     3846 2024-02-20 09:29:13.000000 bddjango-3.0.8/bddjango/tools/db_utils.py
--rw-r--r--   0 root         (0) root         (0)      904 2024-02-20 09:29:13.000000 bddjango-3.0.8/bddjango/tools/create_user.py
--rw-r--r--   0 root         (0) root         (0)     5974 2024-02-20 09:29:13.000000 bddjango-3.0.8/bddjango/tools/statistic_keywords_mixin.py
--rw-r--r--   0 root         (0) root         (0)      238 2024-02-20 09:29:13.000000 bddjango-3.0.8/bddjango/tools/csrf_exempt.py
--rw-r--r--   0 root         (0) root         (0)      395 2024-02-20 09:29:13.000000 bddjango-3.0.8/bddjango/tools/sort_dc_ls1_by_ls2.py
--rw-r--r--   0 root         (0) root         (0)     9054 2024-02-20 09:29:13.000000 bddjango-3.0.8/bddjango/tools/base_orm_search.py
--rw-r--r--   0 root         (0) root         (0)     4048 2024-02-20 09:29:13.000000 bddjango-3.0.8/bddjango/tools/get_hot_keywords.py
--rw-r--r--   0 root         (0) root         (0)      296 2024-02-20 09:29:13.000000 bddjango-3.0.8/bddjango/tools/get_user_ip.py
--rw-r--r--   0 root         (0) root         (0)      735 2024-02-20 09:29:13.000000 bddjango-3.0.8/bddjango/tools/default
--rw-r--r--   0 root         (0) root         (0)     8382 2024-02-20 09:29:13.000000 bddjango-3.0.8/bddjango/tools/generateModelCodeFromExcel.py
--rw-r--r--   0 root         (0) root         (0)      175 2024-02-20 09:29:13.000000 bddjango-3.0.8/bddjango/tools/mylogger.py
--rw-r--r--   0 root         (0) root         (0)      162 2024-02-20 09:29:13.000000 bddjango-3.0.8/bddjango/tools/fake_model.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-02-20 09:29:44.000000 bddjango-3.0.8/bddjango/tools/extract_keyword/
--rw-r--r--   0 root         (0) root         (0)       63 2024-02-20 09:29:13.000000 bddjango-3.0.8/bddjango/tools/extract_keyword/__init__.py
--rw-r--r--   0 root         (0) root         (0)       46 2024-02-20 09:29:13.000000 bddjango-3.0.8/bddjango/tools/extract_keyword/user_dict.txt
--rw-r--r--   0 root         (0) root         (0)      199 2024-02-20 09:29:13.000000 bddjango-3.0.8/bddjango/tools/extract_keyword/stopwords.txt
--rw-r--r--   0 root         (0) root         (0)       34 2024-02-20 09:29:13.000000 bddjango-3.0.8/bddjango/tools/extract_keyword/synonym_dict.txt
--rw-r--r--   0 root         (0) root         (0)     6908 2024-02-20 09:29:13.000000 bddjango-3.0.8/bddjango/tools/extract_keyword/extract_keyword.py
--rw-r--r--   0 root         (0) root         (0)     3936 2024-02-20 09:29:13.000000 bddjango-3.0.8/bddjango/tools/init_import_data_mixin.py
--rw-r--r--   0 root         (0) root         (0)     1300 2024-02-20 09:29:13.000000 bddjango-3.0.8/bddjango/tools/myflask.py
--rw-r--r--   0 root         (0) root         (0)     2472 2024-02-20 09:29:13.000000 bddjango-3.0.8/bddjango/tools/copy_to.py
--rw-r--r--   0 root         (0) root         (0)     3849 2024-02-20 09:29:13.000000 bddjango-3.0.8/bddjango/tools/unzip_to.py
--rw-r--r--   0 root         (0) root         (0)      351 2024-02-20 09:29:13.000000 bddjango-3.0.8/bddjango/tools/remove_path.py
--rw-r--r--   0 root         (0) root         (0)     2298 2024-02-20 09:29:13.000000 bddjango-3.0.8/bddjango/tools/remove_temp_file.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-02-20 09:29:44.000000 bddjango-3.0.8/bddjango/django/
--rw-r--r--   0 root         (0) root         (0)      275 2024-02-20 09:29:13.000000 bddjango-3.0.8/bddjango/django/__init__.py
--rw-r--r--   0 root         (0) root         (0)     9039 2024-02-20 09:29:13.000000 bddjango-3.0.8/bddjango/django/models.py
--rw-r--r--   0 root         (0) root         (0)     9856 2024-02-20 09:29:13.000000 bddjango-3.0.8/bddjango/django/mixins.py
--rw-r--r--   0 root         (0) root         (0)    38375 2024-02-20 09:29:13.000000 bddjango-3.0.8/bddjango/django/utils.py
--rw-r--r--   0 root         (0) root         (0)     7902 2024-02-20 09:29:13.000000 bddjango-3.0.8/bddjango/django/auth.py
--rw-r--r--   0 root         (0) root         (0)    28678 2024-02-20 09:29:13.000000 bddjango-3.0.8/bddjango/django/views.py
--rw-r--r--   0 root         (0) root         (0)      549 2024-02-20 09:29:13.000000 bddjango-3.0.8/bddjango/django/conf.py
--rw-r--r--   0 root         (0) root         (0)     3391 2024-02-20 09:29:13.000000 bddjango-3.0.8/bddjango/baseSearchView.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-02-20 09:29:44.000000 bddjango-3.0.8/bddjango/adminclass/
--rw-r--r--   0 root         (0) root         (0)       97 2024-02-20 09:29:13.000000 bddjango-3.0.8/bddjango/adminclass/__init__.py
--rw-r--r--   0 root         (0) root         (0)    56987 2024-02-20 09:29:13.000000 bddjango-3.0.8/bddjango/adminclass/adminclass.py
--rw-r--r--   0 root         (0) root         (0)     2557 2024-02-20 09:29:13.000000 bddjango-3.0.8/bddjango/adminclass/admin_env_init.py
--rw-r--r--   0 root         (0) root         (0)      198 2024-02-20 09:29:13.000000 bddjango-3.0.8/bddjango/PypiReadme.md
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-02-20 09:29:44.000000 bddjango-3.0.8/bddjango/logs/
--rw-r--r--   0 root         (0) root         (0)     2217 2024-02-20 09:29:13.000000 bddjango-3.0.8/bddjango/logs/log2.md
--rw-r--r--   0 root         (0) root         (0)      404 2024-02-20 09:29:13.000000 bddjango-3.0.8/bddjango/Readme.md
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-02-20 09:29:44.000000 bddjango-3.0.8/bddjango/templates/
--rw-r--r--   0 root         (0) root         (0)     2175 2024-02-20 09:29:13.000000 bddjango-3.0.8/bddjango/templates/autoWiki.html
--rw-r--r--   0 root         (0) root         (0)     1754 2024-02-20 09:29:13.000000 bddjango-3.0.8/bddjango/templates/autoCode.html
--rw-r--r--   0 root         (0) root         (0)     4721 2024-02-20 09:29:13.000000 bddjango-3.0.8/bddjango/templates/copyCode.html
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-02-20 09:29:44.000000 bddjango-3.0.8/bddjango/templates/entities/
--rw-r--r--   0 root         (0) root         (0)     1682 2024-02-20 09:29:13.000000 bddjango-3.0.8/bddjango/templates/entities/simpleui_change_list0.html
--rw-r--r--   0 root         (0) root         (0)     2190 2024-02-20 09:29:13.000000 bddjango-3.0.8/bddjango/templates/entities/simpleui_change_list.html
--rw-r--r--   0 root         (0) root         (0)     6136 2024-02-20 09:29:13.000000 bddjango-3.0.8/bddjango/templates/entities/simpleui_change_list_actions.html
--rw-r--r--   0 root         (0) root         (0)     2267 2024-02-20 09:29:13.000000 bddjango-3.0.8/bddjango/templates/entities/base_change_list.html
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-02-20 09:29:44.000000 bddjango-3.0.8/bddjango/templates/admin/
--rw-r--r--   0 root         (0) root         (0)    21079 2024-02-20 09:29:13.000000 bddjango-3.0.8/bddjango/templates/admin/simpleui_admin_actions.html
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-02-20 09:29:44.000000 bddjango-3.0.8/bddjango/templates/admin/guardian/
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-02-20 09:29:44.000000 bddjango-3.0.8/bddjango/templates/admin/guardian/model/
--rw-r--r--   0 root         (0) root         (0)     1155 2024-02-20 09:29:13.000000 bddjango-3.0.8/bddjango/templates/admin/guardian/model/simpleui_guardian_change_form.html
--rw-r--r--   0 root         (0) root         (0)     1531 2024-02-20 09:29:13.000000 bddjango-3.0.8/bddjango/templates/admin/csv_form.html
--rw-r--r--   0 root         (0) root         (0)     6122 2024-02-20 09:29:13.000000 bddjango-3.0.8/bddjango/templates/admin/import_progress_bar.html
--rw-r--r--   0 root         (0) root         (0)    28553 2024-02-20 09:29:13.000000 bddjango-3.0.8/bddjango/autoWiki.py
--rw-r--r--   0 root         (0) root         (0)     2291 2024-02-20 09:29:13.000000 bddjango-3.0.8/bddjango/log.md
--rw-r--r--   0 root         (0) root         (0)     9839 2024-02-20 09:29:13.000000 bddjango-3.0.8/bddjango/pure.py
--rw-r--r--   0 root         (0) root         (0)    24661 2024-02-20 09:29:13.000000 bddjango-3.0.8/bddjango/autoCode.py
-lrwxrwxrwx   0 root         (0) root         (0)        0 2022-09-30 08:46:24.000000 bddjango-3.0.8/PypiReadme.md -> bddjango/PypiReadme.md
-lrwxrwxrwx   0 root         (0) root         (0)        0 2022-09-30 08:28:31.000000 bddjango-3.0.8/Readme.md -> bddjango/Readme.md
--rw-r--r--   0 root         (0) root         (0)       99 2021-11-28 06:23:01.000000 bddjango-3.0.8/MANIFEST.in
--rw-r--r--   0 root         (0) root         (0)       59 2024-02-20 09:29:44.000000 bddjango-3.0.8/setup.cfg
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-02-20 09:29:44.000000 bddjango-3.0.8/bddjango.egg-info/
--rw-r--r--   0 root         (0) root         (0)        9 2024-02-20 09:29:43.000000 bddjango-3.0.8/bddjango.egg-info/top_level.txt
--rw-r--r--   0 root         (0) root         (0)       44 2024-02-20 09:29:43.000000 bddjango-3.0.8/bddjango.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)     2191 2024-02-20 09:29:43.000000 bddjango-3.0.8/bddjango.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2024-02-20 09:29:43.000000 bddjango-3.0.8/bddjango.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)      748 2024-02-20 09:29:43.000000 bddjango-3.0.8/bddjango.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)      748 2024-02-20 09:29:44.000000 bddjango-3.0.8/PKG-INFO
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-29 08:47:22.392694 bddjango-3.0.9/
+-rw-r--r--   0 root         (0) root         (0)       99 2021-11-28 06:23:01.000000 bddjango-3.0.9/MANIFEST.in
+-rw-r--r--   0 root         (0) root         (0)      664 2024-05-29 08:47:22.388694 bddjango-3.0.9/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)      198 2024-02-20 09:29:13.000000 bddjango-3.0.9/PypiReadme.md
+-rw-r--r--   0 root         (0) root         (0)      404 2024-02-20 09:29:13.000000 bddjango-3.0.9/Readme.md
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-29 08:47:22.372693 bddjango-3.0.9/bddjango/
+-rw-r--r--   0 root         (0) root         (0)    15976 2024-03-19 03:28:12.000000 bddjango-3.0.9/bddjango/MultipleConditionSearch.py
+-rw-r--r--   0 root         (0) root         (0)      198 2024-03-19 03:28:12.000000 bddjango-3.0.9/bddjango/PypiReadme.md
+-rw-r--r--   0 root         (0) root         (0)      404 2024-03-19 03:28:12.000000 bddjango-3.0.9/bddjango/Readme.md
+-rw-r--r--   0 root         (0) root         (0)      674 2024-05-29 08:45:34.000000 bddjango-3.0.9/bddjango/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-29 08:47:22.372693 bddjango-3.0.9/bddjango/adminclass/
+-rw-r--r--   0 root         (0) root         (0)       97 2024-03-19 03:28:12.000000 bddjango-3.0.9/bddjango/adminclass/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     2557 2024-03-19 03:28:12.000000 bddjango-3.0.9/bddjango/adminclass/admin_env_init.py
+-rw-r--r--   0 root         (0) root         (0)    56992 2024-05-29 08:45:34.000000 bddjango-3.0.9/bddjango/adminclass/adminclass.py
+-rw-r--r--   0 root         (0) root         (0)    24522 2024-05-29 08:15:59.000000 bddjango-3.0.9/bddjango/autoCode.py
+-rw-r--r--   0 root         (0) root         (0)    28553 2024-03-19 03:28:12.000000 bddjango-3.0.9/bddjango/autoWiki.py
+-rw-r--r--   0 root         (0) root         (0)     3391 2024-03-19 03:28:12.000000 bddjango-3.0.9/bddjango/baseSearchView.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-29 08:47:22.376693 bddjango-3.0.9/bddjango/django/
+-rw-r--r--   0 root         (0) root         (0)      275 2024-03-19 03:28:12.000000 bddjango-3.0.9/bddjango/django/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     7836 2024-05-29 08:11:58.000000 bddjango-3.0.9/bddjango/django/auth.py
+-rw-r--r--   0 root         (0) root         (0)      549 2024-03-19 03:28:12.000000 bddjango-3.0.9/bddjango/django/conf.py
+-rw-r--r--   0 root         (0) root         (0)     9856 2024-03-19 03:28:12.000000 bddjango-3.0.9/bddjango/django/mixins.py
+-rw-r--r--   0 root         (0) root         (0)     9039 2024-03-19 03:28:12.000000 bddjango-3.0.9/bddjango/django/models.py
+-rw-r--r--   0 root         (0) root         (0)    38375 2024-03-19 03:28:12.000000 bddjango-3.0.9/bddjango/django/utils.py
+-rw-r--r--   0 root         (0) root         (0)    28678 2024-03-19 03:28:12.000000 bddjango-3.0.9/bddjango/django/views.py
+-rw-r--r--   0 root         (0) root         (0)     2473 2024-05-29 08:16:28.000000 bddjango-3.0.9/bddjango/log.md
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-29 08:47:22.376693 bddjango-3.0.9/bddjango/logs/
+-rw-r--r--   0 root         (0) root         (0)     2217 2024-03-19 03:28:12.000000 bddjango-3.0.9/bddjango/logs/log2.md
+-rw-r--r--   0 root         (0) root         (0)     9839 2024-03-19 03:28:12.000000 bddjango-3.0.9/bddjango/pure.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-29 08:47:22.376693 bddjango-3.0.9/bddjango/templates/
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-29 08:47:22.380693 bddjango-3.0.9/bddjango/templates/admin/
+-rw-r--r--   0 root         (0) root         (0)     1531 2024-03-19 03:28:12.000000 bddjango-3.0.9/bddjango/templates/admin/csv_form.html
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-29 08:47:22.368693 bddjango-3.0.9/bddjango/templates/admin/guardian/
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-29 08:47:22.380693 bddjango-3.0.9/bddjango/templates/admin/guardian/model/
+-rw-r--r--   0 root         (0) root         (0)     1155 2024-03-19 03:28:12.000000 bddjango-3.0.9/bddjango/templates/admin/guardian/model/simpleui_guardian_change_form.html
+-rw-r--r--   0 root         (0) root         (0)     6122 2024-03-19 03:28:12.000000 bddjango-3.0.9/bddjango/templates/admin/import_progress_bar.html
+-rw-r--r--   0 root         (0) root         (0)    21079 2024-03-19 03:28:12.000000 bddjango-3.0.9/bddjango/templates/admin/simpleui_admin_actions.html
+-rw-r--r--   0 root         (0) root         (0)     1754 2024-03-19 03:28:12.000000 bddjango-3.0.9/bddjango/templates/autoCode.html
+-rw-r--r--   0 root         (0) root         (0)     2175 2024-03-19 03:28:12.000000 bddjango-3.0.9/bddjango/templates/autoWiki.html
+-rw-r--r--   0 root         (0) root         (0)     4721 2024-03-19 03:28:12.000000 bddjango-3.0.9/bddjango/templates/copyCode.html
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-29 08:47:22.380693 bddjango-3.0.9/bddjango/templates/entities/
+-rw-r--r--   0 root         (0) root         (0)     2267 2024-03-19 03:28:12.000000 bddjango-3.0.9/bddjango/templates/entities/base_change_list.html
+-rw-r--r--   0 root         (0) root         (0)     2190 2024-03-19 03:28:12.000000 bddjango-3.0.9/bddjango/templates/entities/simpleui_change_list.html
+-rw-r--r--   0 root         (0) root         (0)     1682 2024-03-19 03:28:12.000000 bddjango-3.0.9/bddjango/templates/entities/simpleui_change_list0.html
+-rw-r--r--   0 root         (0) root         (0)     6136 2024-03-19 03:28:12.000000 bddjango-3.0.9/bddjango/templates/entities/simpleui_change_list_actions.html
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-29 08:47:22.388694 bddjango-3.0.9/bddjango/tools/
+-rw-r--r--   0 root         (0) root         (0)      393 2024-03-19 03:28:12.000000 bddjango-3.0.9/bddjango/tools/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     9054 2024-03-19 03:28:12.000000 bddjango-3.0.9/bddjango/tools/base_orm_search.py
+-rw-r--r--   0 root         (0) root         (0)     2472 2024-03-19 03:28:12.000000 bddjango-3.0.9/bddjango/tools/copy_to.py
+-rw-r--r--   0 root         (0) root         (0)      904 2024-03-19 03:28:12.000000 bddjango-3.0.9/bddjango/tools/create_user.py
+-rw-r--r--   0 root         (0) root         (0)      238 2024-03-19 03:28:12.000000 bddjango-3.0.9/bddjango/tools/csrf_exempt.py
+-rw-r--r--   0 root         (0) root         (0)     3846 2024-03-19 03:28:12.000000 bddjango-3.0.9/bddjango/tools/db_utils.py
+-rw-r--r--   0 root         (0) root         (0)      735 2024-03-19 03:28:12.000000 bddjango-3.0.9/bddjango/tools/default
+-rw-r--r--   0 root         (0) root         (0)     1248 2024-03-19 03:28:12.000000 bddjango-3.0.9/bddjango/tools/extractPdf.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-29 08:47:22.388694 bddjango-3.0.9/bddjango/tools/extract_keyword/
+-rw-r--r--   0 root         (0) root         (0)       63 2024-03-19 03:28:12.000000 bddjango-3.0.9/bddjango/tools/extract_keyword/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     6908 2024-03-19 03:28:12.000000 bddjango-3.0.9/bddjango/tools/extract_keyword/extract_keyword.py
+-rw-r--r--   0 root         (0) root         (0)      199 2024-03-19 03:28:12.000000 bddjango-3.0.9/bddjango/tools/extract_keyword/stopwords.txt
+-rw-r--r--   0 root         (0) root         (0)       34 2024-03-19 03:28:12.000000 bddjango-3.0.9/bddjango/tools/extract_keyword/synonym_dict.txt
+-rw-r--r--   0 root         (0) root         (0)       46 2024-03-19 03:28:12.000000 bddjango-3.0.9/bddjango/tools/extract_keyword/user_dict.txt
+-rw-r--r--   0 root         (0) root         (0)      162 2024-03-19 03:28:12.000000 bddjango-3.0.9/bddjango/tools/fake_model.py
+-rw-r--r--   0 root         (0) root         (0)     8382 2024-03-19 03:28:12.000000 bddjango-3.0.9/bddjango/tools/generateModelCodeFromExcel.py
+-rw-r--r--   0 root         (0) root         (0)     4048 2024-03-19 03:28:12.000000 bddjango-3.0.9/bddjango/tools/get_hot_keywords.py
+-rw-r--r--   0 root         (0) root         (0)      296 2024-03-19 03:28:12.000000 bddjango-3.0.9/bddjango/tools/get_user_ip.py
+-rw-r--r--   0 root         (0) root         (0)     2452 2024-03-19 03:28:12.000000 bddjango-3.0.9/bddjango/tools/getshells.py
+-rw-r--r--   0 root         (0) root         (0)     3936 2024-03-19 03:28:12.000000 bddjango-3.0.9/bddjango/tools/init_import_data_mixin.py
+-rw-r--r--   0 root         (0) root         (0)     1300 2024-03-19 03:28:12.000000 bddjango-3.0.9/bddjango/tools/myflask.py
+-rw-r--r--   0 root         (0) root         (0)      175 2024-03-19 03:28:12.000000 bddjango-3.0.9/bddjango/tools/mylogger.py
+-rw-r--r--   0 root         (0) root         (0)      908 2024-03-19 03:28:12.000000 bddjango-3.0.9/bddjango/tools/nginx_config.py
+-rw-r--r--   0 root         (0) root         (0)      351 2024-03-19 03:28:12.000000 bddjango-3.0.9/bddjango/tools/remove_path.py
+-rw-r--r--   0 root         (0) root         (0)     2298 2024-03-19 03:28:12.000000 bddjango-3.0.9/bddjango/tools/remove_temp_file.py
+-rw-r--r--   0 root         (0) root         (0)      395 2024-03-19 03:28:12.000000 bddjango-3.0.9/bddjango/tools/sort_dc_ls1_by_ls2.py
+-rw-r--r--   0 root         (0) root         (0)     5974 2024-03-19 03:28:12.000000 bddjango-3.0.9/bddjango/tools/statistic_keywords_mixin.py
+-rw-r--r--   0 root         (0) root         (0)     3849 2024-03-19 03:28:12.000000 bddjango-3.0.9/bddjango/tools/unzip_to.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-29 08:47:22.388694 bddjango-3.0.9/bddjango/tools/version_monkey_patch/
+-rw-r--r--   0 root         (0) root         (0)        0 2024-05-29 08:10:03.000000 bddjango-3.0.9/bddjango/tools/version_monkey_patch/__init__.py
+-rw-r--r--   0 root         (0) root         (0)      648 2024-05-29 08:05:21.000000 bddjango-3.0.9/bddjango/tools/version_monkey_patch/package_version_utils.py
+-rw-r--r--   0 root         (0) root         (0)      791 2024-05-29 08:11:17.000000 bddjango-3.0.9/bddjango/tools/version_monkey_patch/save_excel.py
+-rw-r--r--   0 root         (0) root         (0)     4162 2024-03-19 03:28:12.000000 bddjango-3.0.9/bddjango/tools/zipDir.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-29 08:47:22.372693 bddjango-3.0.9/bddjango.egg-info/
+-rw-r--r--   0 root         (0) root         (0)      664 2024-05-29 08:47:22.000000 bddjango-3.0.9/bddjango.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)     2350 2024-05-29 08:47:22.000000 bddjango-3.0.9/bddjango.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2024-05-29 08:47:22.000000 bddjango-3.0.9/bddjango.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)       44 2024-05-29 08:47:22.000000 bddjango-3.0.9/bddjango.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)        9 2024-05-29 08:47:22.000000 bddjango-3.0.9/bddjango.egg-info/top_level.txt
+-rw-r--r--   0 root         (0) root         (0)       38 2024-05-29 08:47:22.392694 bddjango-3.0.9/setup.cfg
+-rw-r--r--   0 root         (0) root         (0)     1141 2024-02-20 09:29:13.000000 bddjango-3.0.9/setup.py
```

### filetype from file(1)

```diff
@@ -1 +1 @@
-POSIX tar archive (GNU)
+POSIX tar archive
```

### Comparing `bddjango-3.0.8/setup.py` & `bddjango-3.0.9/setup.py`

 * *Files identical despite different names*

### Comparing `bddjango-3.0.8/bddjango/MultipleConditionSearch.py` & `bddjango-3.0.9/bddjango/MultipleConditionSearch.py`

 * *Files identical despite different names*

### Comparing `bddjango-3.0.8/bddjango/tools/extractPdf.py` & `bddjango-3.0.9/bddjango/tools/extractPdf.py`

 * *Files identical despite different names*

### Comparing `bddjango-3.0.8/bddjango/tools/nginx_config.py` & `bddjango-3.0.9/bddjango/tools/nginx_config.py`

 * *Files identical despite different names*

### Comparing `bddjango-3.0.8/bddjango/tools/zipDir.py` & `bddjango-3.0.9/bddjango/tools/zipDir.py`

 * *Files identical despite different names*

### Comparing `bddjango-3.0.8/bddjango/tools/getshells.py` & `bddjango-3.0.9/bddjango/tools/getshells.py`

 * *Files identical despite different names*

### Comparing `bddjango-3.0.8/bddjango/tools/db_utils.py` & `bddjango-3.0.9/bddjango/tools/db_utils.py`

 * *Files identical despite different names*

### Comparing `bddjango-3.0.8/bddjango/tools/create_user.py` & `bddjango-3.0.9/bddjango/tools/create_user.py`

 * *Files identical despite different names*

### Comparing `bddjango-3.0.8/bddjango/tools/statistic_keywords_mixin.py` & `bddjango-3.0.9/bddjango/tools/statistic_keywords_mixin.py`

 * *Files identical despite different names*

### Comparing `bddjango-3.0.8/bddjango/tools/base_orm_search.py` & `bddjango-3.0.9/bddjango/tools/base_orm_search.py`

 * *Files identical despite different names*

### Comparing `bddjango-3.0.8/bddjango/tools/get_hot_keywords.py` & `bddjango-3.0.9/bddjango/tools/get_hot_keywords.py`

 * *Files identical despite different names*

### Comparing `bddjango-3.0.8/bddjango/tools/default` & `bddjango-3.0.9/bddjango/tools/default`

 * *Files identical despite different names*

### Comparing `bddjango-3.0.8/bddjango/tools/generateModelCodeFromExcel.py` & `bddjango-3.0.9/bddjango/tools/generateModelCodeFromExcel.py`

 * *Files identical despite different names*

### Comparing `bddjango-3.0.8/bddjango/tools/extract_keyword/extract_keyword.py` & `bddjango-3.0.9/bddjango/tools/extract_keyword/extract_keyword.py`

 * *Files identical despite different names*

### Comparing `bddjango-3.0.8/bddjango/tools/init_import_data_mixin.py` & `bddjango-3.0.9/bddjango/tools/init_import_data_mixin.py`

 * *Files identical despite different names*

### Comparing `bddjango-3.0.8/bddjango/tools/myflask.py` & `bddjango-3.0.9/bddjango/tools/myflask.py`

 * *Files identical despite different names*

### Comparing `bddjango-3.0.8/bddjango/tools/copy_to.py` & `bddjango-3.0.9/bddjango/tools/copy_to.py`

 * *Files identical despite different names*

### Comparing `bddjango-3.0.8/bddjango/tools/unzip_to.py` & `bddjango-3.0.9/bddjango/tools/unzip_to.py`

 * *Files identical despite different names*

### Comparing `bddjango-3.0.8/bddjango/tools/remove_temp_file.py` & `bddjango-3.0.9/bddjango/tools/remove_temp_file.py`

 * *Files identical despite different names*

### Comparing `bddjango-3.0.8/bddjango/django/models.py` & `bddjango-3.0.9/bddjango/django/models.py`

 * *Files identical despite different names*

### Comparing `bddjango-3.0.8/bddjango/django/mixins.py` & `bddjango-3.0.9/bddjango/django/mixins.py`

 * *Files identical despite different names*

### Comparing `bddjango-3.0.8/bddjango/django/utils.py` & `bddjango-3.0.9/bddjango/django/utils.py`

 * *Files identical despite different names*

### Comparing `bddjango-3.0.8/bddjango/django/auth.py` & `bddjango-3.0.9/bddjango/django/auth.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,11 +1,10 @@
 from django.utils.encoding import force_str
 from rest_framework.utils.serializer_helpers import ReturnList, ReturnDict
 from rest_framework.exceptions import APIException, ErrorDetail, status
-from django.utils.translation import ugettext_lazy
 from rest_framework.authentication import BaseAuthentication
 from rest_framework import exceptions
 from rest_framework.authtoken.models import Token
 from rest_framework import HTTP_HEADER_ENCODING
 from django.contrib.auth.models import AnonymousUser
 
 
@@ -104,15 +103,15 @@
     def authenticate(self, request):
         auth = get_authorization_header(request)
         if not auth:
             return None
         try:
             token = auth.decode()
         except UnicodeError:
-            msg = ugettext_lazy("无效的Token， Token头不应包含无效字符")
+            msg = "无效的Token， Token头不应包含无效字符"
             raise exceptions.AuthenticationFailed(msg)
 
         return self.authenticate_credentials(token)
 
     def authenticate_credentials(self, key):
         # 尝试从缓存获取用户信息（设置中配置了缓存的可以添加，不加也不影响正常功能）
         # token_cache = 'token_' + key
```

### Comparing `bddjango-3.0.8/bddjango/django/views.py` & `bddjango-3.0.9/bddjango/django/views.py`

 * *Files identical despite different names*

### Comparing `bddjango-3.0.8/bddjango/django/conf.py` & `bddjango-3.0.9/bddjango/django/conf.py`

 * *Files identical despite different names*

### Comparing `bddjango-3.0.8/bddjango/baseSearchView.py` & `bddjango-3.0.9/bddjango/baseSearchView.py`

 * *Files identical despite different names*

### Comparing `bddjango-3.0.8/bddjango/adminclass/adminclass.py` & `bddjango-3.0.9/bddjango/adminclass/adminclass.py`

 * *Files 1% similar despite different names*

```diff
@@ -38,15 +38,16 @@
 from openpyxl import Workbook
 from bdtime import Time
 from django import forms
 from django.shortcuts import render, redirect, HttpResponse
 from django.urls import path
 from django.contrib import admin
 from django.contrib import messages
-from django.utils.http import urlquote
+
+from urllib.parse import quote as urlquote
 
 from .. import reset_db_sequence
 from ..pure import remove_temp_file
 
 # --- 初始化环境 ---
 from .admin_env_init import CHANGE_LIST_HTML_PATH, TEMPDIR, BD_USE_GUARDIAN, CHANGE_FORM_TEMPLATE, BD_USE_SIMPLEUI
 from .admin_env_init import BD_USE_AJAX_ADMIN
```

### Comparing `bddjango-3.0.8/bddjango/adminclass/admin_env_init.py` & `bddjango-3.0.9/bddjango/adminclass/admin_env_init.py`

 * *Files identical despite different names*

### Comparing `bddjango-3.0.8/bddjango/logs/log2.md` & `bddjango-3.0.9/bddjango/logs/log2.md`

 * *Files identical despite different names*

### Comparing `bddjango-3.0.8/bddjango/templates/autoWiki.html` & `bddjango-3.0.9/bddjango/templates/autoWiki.html`

 * *Files identical despite different names*

### Comparing `bddjango-3.0.8/bddjango/templates/autoCode.html` & `bddjango-3.0.9/bddjango/templates/autoCode.html`

 * *Files identical despite different names*

### Comparing `bddjango-3.0.8/bddjango/templates/copyCode.html` & `bddjango-3.0.9/bddjango/templates/copyCode.html`

 * *Files identical despite different names*

### Comparing `bddjango-3.0.8/bddjango/templates/entities/simpleui_change_list0.html` & `bddjango-3.0.9/bddjango/templates/entities/simpleui_change_list0.html`

 * *Files identical despite different names*

### Comparing `bddjango-3.0.8/bddjango/templates/entities/simpleui_change_list.html` & `bddjango-3.0.9/bddjango/templates/entities/simpleui_change_list.html`

 * *Files identical despite different names*

### Comparing `bddjango-3.0.8/bddjango/templates/entities/simpleui_change_list_actions.html` & `bddjango-3.0.9/bddjango/templates/entities/simpleui_change_list_actions.html`

 * *Files identical despite different names*

### Comparing `bddjango-3.0.8/bddjango/templates/entities/base_change_list.html` & `bddjango-3.0.9/bddjango/templates/entities/base_change_list.html`

 * *Files identical despite different names*

### Comparing `bddjango-3.0.8/bddjango/templates/admin/simpleui_admin_actions.html` & `bddjango-3.0.9/bddjango/templates/admin/simpleui_admin_actions.html`

 * *Files identical despite different names*

### Comparing `bddjango-3.0.8/bddjango/templates/admin/guardian/model/simpleui_guardian_change_form.html` & `bddjango-3.0.9/bddjango/templates/admin/guardian/model/simpleui_guardian_change_form.html`

 * *Files identical despite different names*

### Comparing `bddjango-3.0.8/bddjango/templates/admin/csv_form.html` & `bddjango-3.0.9/bddjango/templates/admin/csv_form.html`

 * *Files identical despite different names*

### Comparing `bddjango-3.0.8/bddjango/templates/admin/import_progress_bar.html` & `bddjango-3.0.9/bddjango/templates/admin/import_progress_bar.html`

 * *Files identical despite different names*

### Comparing `bddjango-3.0.8/bddjango/autoWiki.py` & `bddjango-3.0.9/bddjango/autoWiki.py`

 * *Files identical despite different names*

### Comparing `bddjango-3.0.8/bddjango/log.md` & `bddjango-3.0.9/bddjango/log.md`

 * *Files 12% similar despite different names*

```diff
@@ -62,8 +62,15 @@
 
 # 3.0.7
 - get_key_from_request_data_or_self_obj优化为False的条件
 
 # 3.0.8
 - 生成代码与xlrd解耦
 
+# 3.0.9
+- 兼容高版本pandas, 解决read_excel中去掉了encoding参数导致代码出错的问题
+- 兼容4.2版本django和对应的drf, tools中增加version_monkey_patch
+
+
+
+
```

### Comparing `bddjango-3.0.8/bddjango/pure.py` & `bddjango-3.0.9/bddjango/pure.py`

 * *Files identical despite different names*

### Comparing `bddjango-3.0.8/bddjango/autoCode.py` & `bddjango-3.0.9/bddjango/autoCode.py`

 * *Files 1% similar despite different names*

```diff
@@ -9,14 +9,16 @@
 from django.contrib.contenttypes.models import ContentType
 from bddjango import convert_query_parameter_to_bool, my_api_assert_function
 from bddjango import find_indexes_in_dc_ls
 from bddjango import get_base_model
 from bddjango import get_field_names_by_model
 
 import sys
+from .tools.version_monkey_patch.save_excel import save_excel
+
 
 tmp_urls = None
 tmp_views = None
 
 
 def get_my_apps():
     my_apps = []
@@ -512,21 +514,18 @@
                 file_data = file_contents.decode(encoding)
 
             with open(f_path, 'w', encoding=encoding) as f:
                 f.write(file_data)
 
             # # 为解决字段内有逗号导致分割错误问题, 只能采用pd了
             # df = pd.read_csv(fname, encoding=encoding)
-        elif f_format == 'xls':
-            df = pd.read_excel(file_contents, engine='openpyxl', keep_default_na=False)
-            df.to_excel(f_path, index=False, encoding='utf-8')
-        elif f_format == 'xlsx':
+        elif f_format in ['xls', 'xlsx']:
             try:
                 df = pd.read_excel(file_contents, engine='openpyxl', keep_default_na=False)
-                df.to_excel(f_path, index=False, encoding='utf-8')
+                save_excel(df, f_path)
             except Exception as e:
                 raise TypeError(f'文件读入错误! 可转换为`xls`格式后重试. msg: {e}')
 
         model_info = get_model_info(f_path, add_db_column=add_db_column)
         content = model_info.get('model_code')
         output_fname = model_info.get('model_name')
```

### Comparing `bddjango-3.0.8/bddjango.egg-info/SOURCES.txt` & `bddjango-3.0.9/bddjango.egg-info/SOURCES.txt`

 * *Files 11% similar despite different names*

```diff
@@ -61,8 +61,11 @@
 bddjango/tools/statistic_keywords_mixin.py
 bddjango/tools/unzip_to.py
 bddjango/tools/zipDir.py
 bddjango/tools/extract_keyword/__init__.py
 bddjango/tools/extract_keyword/extract_keyword.py
 bddjango/tools/extract_keyword/stopwords.txt
 bddjango/tools/extract_keyword/synonym_dict.txt
-bddjango/tools/extract_keyword/user_dict.txt
+bddjango/tools/extract_keyword/user_dict.txt
+bddjango/tools/version_monkey_patch/__init__.py
+bddjango/tools/version_monkey_patch/package_version_utils.py
+bddjango/tools/version_monkey_patch/save_excel.py
```

