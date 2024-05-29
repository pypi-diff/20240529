# Comparing `tmp/assessment_episode_matcher-0.5.4.tar.gz` & `tmp/assessment_episode_matcher-0.5.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "assessment_episode_matcher-0.5.4.tar", last modified: Tue May 28 08:33:56 2024, max compression
+gzip compressed data, was "assessment_episode_matcher-0.5.5.tar", last modified: Wed May 29 21:36:01 2024, max compression
```

## Comparing `assessment_episode_matcher-0.5.4.tar` & `assessment_episode_matcher-0.5.5.tar`

### file list

```diff
@@ -1,69 +1,69 @@
-drwxrwxrwx   0        0        0        0 2024-05-28 08:33:56.429695 assessment_episode_matcher-0.5.4/
--rw-rw-rw-   0        0        0     1235 2024-05-17 18:46:24.000000 assessment_episode_matcher-0.5.4/LICENSE
--rw-rw-rw-   0        0        0       26 2024-05-23 22:46:12.000000 assessment_episode_matcher-0.5.4/MANIFEST.in
--rw-rw-rw-   0        0        0      523 2024-05-28 08:33:56.417680 assessment_episode_matcher-0.5.4/PKG-INFO
--rw-rw-rw-   0        0        0      935 2024-05-28 08:06:39.000000 assessment_episode_matcher-0.5.4/README.md
-drwxrwxrwx   0        0        0        0 2024-05-28 08:33:55.789668 assessment_episode_matcher-0.5.4/assessment_episode_matcher/
--rw-rw-rw-   0        0        0      275 2024-05-23 23:19:26.000000 assessment_episode_matcher-0.5.4/assessment_episode_matcher/__init__.py
--rw-rw-rw-   0        0        0      267 2024-05-17 18:43:59.000000 assessment_episode_matcher-0.5.4/assessment_episode_matcher/audits.py
-drwxrwxrwx   0        0        0        0 2024-05-28 08:33:55.937622 assessment_episode_matcher-0.5.4/assessment_episode_matcher/azutil/
--rw-rw-rw-   0        0        0        0 2024-05-17 18:43:59.000000 assessment_episode_matcher-0.5.4/assessment_episode_matcher/azutil/__init__.py
--rw-rw-rw-   0        0        0     5203 2024-05-27 23:08:56.000000 assessment_episode_matcher-0.5.4/assessment_episode_matcher/azutil/az_blob_query.py
--rw-rw-rw-   0        0        0     9425 2024-05-27 23:09:54.000000 assessment_episode_matcher-0.5.4/assessment_episode_matcher/azutil/az_tables_query.py
--rw-rw-rw-   0        0        0     1594 2024-05-27 02:50:37.000000 assessment_episode_matcher-0.5.4/assessment_episode_matcher/azutil/file_types.py
--rw-rw-rw-   0        0        0     3921 2024-05-18 20:57:07.000000 assessment_episode_matcher-0.5.4/assessment_episode_matcher/azutil/helper.py
-drwxrwxrwx   0        0        0        0 2024-05-28 08:33:55.973808 assessment_episode_matcher-0.5.4/assessment_episode_matcher/configs/
--rw-rw-rw-   0        0        0        0 2024-05-24 21:35:01.000000 assessment_episode_matcher-0.5.4/assessment_episode_matcher/configs/__init__.py
--rw-rw-rw-   0        0        0     1331 2024-05-28 07:17:39.000000 assessment_episode_matcher-0.5.4/assessment_episode_matcher/configs/audit.py
--rw-rw-rw-   0        0        0      631 2024-05-26 21:44:37.000000 assessment_episode_matcher-0.5.4/assessment_episode_matcher/configs/episodes.py
--rw-rw-rw-   0        0        0     8591 2024-05-17 22:40:20.000000 assessment_episode_matcher-0.5.4/assessment_episode_matcher/data_config.py
--rw-rw-rw-   0        0        0     5899 2024-05-27 00:25:15.000000 assessment_episode_matcher-0.5.4/assessment_episode_matcher/data_prep.py
-drwxrwxrwx   0        0        0        0 2024-05-28 08:33:56.015705 assessment_episode_matcher-0.5.4/assessment_episode_matcher/exporters/
--rw-rw-rw-   0        0        0     1848 2024-05-26 23:42:24.000000 assessment_episode_matcher-0.5.4/assessment_episode_matcher/exporters/NADAbase.py
--rw-rw-rw-   0        0        0        0 2024-05-17 18:43:59.000000 assessment_episode_matcher-0.5.4/assessment_episode_matcher/exporters/__init__.py
--rw-rw-rw-   0        0        0     3850 2024-05-27 01:14:46.000000 assessment_episode_matcher-0.5.4/assessment_episode_matcher/exporters/main.py
-drwxrwxrwx   0        0        0        0 2024-05-28 08:33:56.137002 assessment_episode_matcher-0.5.4/assessment_episode_matcher/importers/
--rw-rw-rw-   0        0        0        0 2024-05-17 18:43:59.000000 assessment_episode_matcher-0.5.4/assessment_episode_matcher/importers/__init__.py
--rw-rw-rw-   0        0        0    14368 2024-05-27 02:49:09.000000 assessment_episode_matcher-0.5.4/assessment_episode_matcher/importers/aod.py
--rw-rw-rw-   0        0        0     8836 2024-05-26 22:49:07.000000 assessment_episode_matcher-0.5.4/assessment_episode_matcher/importers/assessments.py
--rw-rw-rw-   0        0        0     6681 2024-05-26 21:50:05.000000 assessment_episode_matcher-0.5.4/assessment_episode_matcher/importers/episodes.py
--rw-rw-rw-   0        0        0     3749 2024-05-27 00:19:22.000000 assessment_episode_matcher-0.5.4/assessment_episode_matcher/importers/main.py
--rw-rw-rw-   0        0        0     1485 2024-05-26 23:26:37.000000 assessment_episode_matcher-0.5.4/assessment_episode_matcher/importers/nada_indexed.py
-drwxrwxrwx   0        0        0        0 2024-05-28 08:33:56.215312 assessment_episode_matcher-0.5.4/assessment_episode_matcher/matching/
--rw-rw-rw-   0        0        0        0 2024-05-17 18:43:59.000000 assessment_episode_matcher-0.5.4/assessment_episode_matcher/matching/__init__.py
--rw-rw-rw-   0        0        0     4474 2024-05-27 22:25:32.000000 assessment_episode_matcher-0.5.4/assessment_episode_matcher/matching/date_checks.py
--rw-rw-rw-   0        0        0     4736 2024-05-28 08:31:07.000000 assessment_episode_matcher-0.5.4/assessment_episode_matcher/matching/errors.py
--rw-rw-rw-   0        0        0     5321 2024-05-18 20:55:18.000000 assessment_episode_matcher-0.5.4/assessment_episode_matcher/matching/increasing_slack.py
--rw-rw-rw-   0        0        0    22363 2024-05-28 07:22:56.000000 assessment_episode_matcher-0.5.4/assessment_episode_matcher/matching/main.py
--rw-rw-rw-   0        0        0     1004 2024-05-17 18:43:59.000000 assessment_episode_matcher-0.5.4/assessment_episode_matcher/matching/matching_stats.py
--rw-rw-rw-   0        0        0     2506 2024-05-27 22:23:53.000000 assessment_episode_matcher-0.5.4/assessment_episode_matcher/mytypes.py
--rw-rw-rw-   0        0        0     3965 2024-05-27 03:29:54.000000 assessment_episode_matcher-0.5.4/assessment_episode_matcher/nada.py
-drwxrwxrwx   0        0        0        0 2024-05-28 08:33:56.251090 assessment_episode_matcher-0.5.4/assessment_episode_matcher/setup/
--rw-rw-rw-   0        0        0        0 2024-05-19 22:35:00.000000 assessment_episode_matcher-0.5.4/assessment_episode_matcher/setup/__init__.py
--rw-rw-rw-   0        0        0     4933 2024-05-26 00:16:34.000000 assessment_episode_matcher-0.5.4/assessment_episode_matcher/setup/bootstrap.py
--rw-rw-rw-   0        0        0     2318 2024-05-19 22:34:48.000000 assessment_episode_matcher-0.5.4/assessment_episode_matcher/setup/log_management.py
--rw-rw-rw-   0        0        0     9282 2024-05-28 08:31:15.000000 assessment_episode_matcher-0.5.4/assessment_episode_matcher/test_surveytxt.py
--rw-rw-rw-   0        0        0     8363 2024-05-27 22:54:01.000000 assessment_episode_matcher-0.5.4/assessment_episode_matcher/test_surveytxt_local.py
-drwxrwxrwx   0        0        0        0 2024-05-28 08:33:56.278094 assessment_episode_matcher-0.5.4/assessment_episode_matcher/tests/
--rw-rw-rw-   0        0        0       23 2024-05-17 18:43:59.000000 assessment_episode_matcher-0.5.4/assessment_episode_matcher/tests/__init__.py
--rw-rw-rw-   0        0        0     1377 2024-05-17 18:43:59.000000 assessment_episode_matcher-0.5.4/assessment_episode_matcher/tests/matching_test.py
-drwxrwxrwx   0        0        0        0 2024-05-28 08:33:56.388330 assessment_episode_matcher-0.5.4/assessment_episode_matcher/utils/
--rw-rw-rw-   0        0        0        0 2024-05-17 21:30:48.000000 assessment_episode_matcher-0.5.4/assessment_episode_matcher/utils/__init__.py
--rw-rw-rw-   0        0        0     1270 2024-05-18 20:54:35.000000 assessment_episode_matcher-0.5.4/assessment_episode_matcher/utils/base.py
--rw-rw-rw-   0        0        0     1693 2024-05-17 18:43:59.000000 assessment_episode_matcher-0.5.4/assessment_episode_matcher/utils/ccare_to_aztable.py
--rw-rw-rw-   0        0        0    13615 2024-05-19 23:11:34.000000 assessment_episode_matcher-0.5.4/assessment_episode_matcher/utils/df_ops_base.py
--rw-rw-rw-   0        0        0     7323 2024-05-18 19:37:57.000000 assessment_episode_matcher-0.5.4/assessment_episode_matcher/utils/dtypes.py
--rw-rw-rw-   0        0        0     1303 2024-05-27 04:43:32.000000 assessment_episode_matcher-0.5.4/assessment_episode_matcher/utils/environment.py
--rw-rw-rw-   0        0        0     2247 2024-05-28 06:45:09.000000 assessment_episode_matcher-0.5.4/assessment_episode_matcher/utils/fromstr.py
--rw-rw-rw-   0        0        0      748 2024-05-17 18:43:59.000000 assessment_episode_matcher-0.5.4/assessment_episode_matcher/utils/group_utils.py
--rw-rw-rw-   0        0        0    11458 2024-05-25 23:06:26.000000 assessment_episode_matcher-0.5.4/assessment_episode_matcher/utils/io.py
--rw-rw-rw-   0        0        0       21 2024-05-28 08:33:30.000000 assessment_episode_matcher-0.5.4/assessment_episode_matcher/version.py
-drwxrwxrwx   0        0        0        0 2024-05-28 08:33:56.409491 assessment_episode_matcher-0.5.4/assessment_episode_matcher.egg-info/
--rw-rw-rw-   0        0        0      523 2024-05-28 08:33:55.000000 assessment_episode_matcher-0.5.4/assessment_episode_matcher.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0     2429 2024-05-28 08:33:55.000000 assessment_episode_matcher-0.5.4/assessment_episode_matcher.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-05-28 08:33:55.000000 assessment_episode_matcher-0.5.4/assessment_episode_matcher.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0      105 2024-05-28 08:33:55.000000 assessment_episode_matcher-0.5.4/assessment_episode_matcher.egg-info/requires.txt
--rw-rw-rw-   0        0        0       27 2024-05-28 08:33:55.000000 assessment_episode_matcher-0.5.4/assessment_episode_matcher.egg-info/top_level.txt
--rw-rw-rw-   0        0        0      110 2024-05-17 19:08:24.000000 assessment_episode_matcher-0.5.4/requirements.txt
--rw-rw-rw-   0        0        0       42 2024-05-28 08:33:56.431815 assessment_episode_matcher-0.5.4/setup.cfg
--rw-rw-rw-   0        0        0     1342 2024-05-24 03:53:56.000000 assessment_episode_matcher-0.5.4/setup.py
+drwxrwxrwx   0        0        0        0 2024-05-29 21:36:01.240163 assessment_episode_matcher-0.5.5/
+-rw-rw-rw-   0        0        0     1235 2024-05-17 18:46:24.000000 assessment_episode_matcher-0.5.5/LICENSE
+-rw-rw-rw-   0        0        0       26 2024-05-23 22:46:12.000000 assessment_episode_matcher-0.5.5/MANIFEST.in
+-rw-rw-rw-   0        0        0      523 2024-05-29 21:36:01.237442 assessment_episode_matcher-0.5.5/PKG-INFO
+-rw-rw-rw-   0        0        0     1065 2024-05-29 20:13:46.000000 assessment_episode_matcher-0.5.5/README.md
+drwxrwxrwx   0        0        0        0 2024-05-29 21:36:00.904522 assessment_episode_matcher-0.5.5/assessment_episode_matcher/
+-rw-rw-rw-   0        0        0      275 2024-05-23 23:19:26.000000 assessment_episode_matcher-0.5.5/assessment_episode_matcher/__init__.py
+-rw-rw-rw-   0        0        0      267 2024-05-17 18:43:59.000000 assessment_episode_matcher-0.5.5/assessment_episode_matcher/audits.py
+drwxrwxrwx   0        0        0        0 2024-05-29 21:36:00.982628 assessment_episode_matcher-0.5.5/assessment_episode_matcher/azutil/
+-rw-rw-rw-   0        0        0        0 2024-05-17 18:43:59.000000 assessment_episode_matcher-0.5.5/assessment_episode_matcher/azutil/__init__.py
+-rw-rw-rw-   0        0        0     5203 2024-05-27 23:08:56.000000 assessment_episode_matcher-0.5.5/assessment_episode_matcher/azutil/az_blob_query.py
+-rw-rw-rw-   0        0        0     9425 2024-05-27 23:09:54.000000 assessment_episode_matcher-0.5.5/assessment_episode_matcher/azutil/az_tables_query.py
+-rw-rw-rw-   0        0        0     1594 2024-05-27 02:50:37.000000 assessment_episode_matcher-0.5.5/assessment_episode_matcher/azutil/file_types.py
+-rw-rw-rw-   0        0        0     3921 2024-05-18 20:57:07.000000 assessment_episode_matcher-0.5.5/assessment_episode_matcher/azutil/helper.py
+drwxrwxrwx   0        0        0        0 2024-05-29 21:36:01.000341 assessment_episode_matcher-0.5.5/assessment_episode_matcher/configs/
+-rw-rw-rw-   0        0        0      372 2024-05-29 21:16:18.000000 assessment_episode_matcher-0.5.5/assessment_episode_matcher/configs/__init__.py
+-rw-rw-rw-   0        0        0     1331 2024-05-28 07:17:39.000000 assessment_episode_matcher-0.5.5/assessment_episode_matcher/configs/audit.py
+-rw-rw-rw-   0        0        0      631 2024-05-26 21:44:37.000000 assessment_episode_matcher-0.5.5/assessment_episode_matcher/configs/episodes.py
+-rw-rw-rw-   0        0        0     8591 2024-05-17 22:40:20.000000 assessment_episode_matcher-0.5.5/assessment_episode_matcher/data_config.py
+-rw-rw-rw-   0        0        0     5899 2024-05-27 00:25:15.000000 assessment_episode_matcher-0.5.5/assessment_episode_matcher/data_prep.py
+drwxrwxrwx   0        0        0        0 2024-05-29 21:36:01.021514 assessment_episode_matcher-0.5.5/assessment_episode_matcher/exporters/
+-rw-rw-rw-   0        0        0     1848 2024-05-26 23:42:24.000000 assessment_episode_matcher-0.5.5/assessment_episode_matcher/exporters/NADAbase.py
+-rw-rw-rw-   0        0        0        0 2024-05-17 18:43:59.000000 assessment_episode_matcher-0.5.5/assessment_episode_matcher/exporters/__init__.py
+-rw-rw-rw-   0        0        0     3850 2024-05-27 01:14:46.000000 assessment_episode_matcher-0.5.5/assessment_episode_matcher/exporters/main.py
+drwxrwxrwx   0        0        0        0 2024-05-29 21:36:01.067553 assessment_episode_matcher-0.5.5/assessment_episode_matcher/importers/
+-rw-rw-rw-   0        0        0        0 2024-05-17 18:43:59.000000 assessment_episode_matcher-0.5.5/assessment_episode_matcher/importers/__init__.py
+-rw-rw-rw-   0        0        0    14368 2024-05-27 02:49:09.000000 assessment_episode_matcher-0.5.5/assessment_episode_matcher/importers/aod.py
+-rw-rw-rw-   0        0        0     8836 2024-05-26 22:49:07.000000 assessment_episode_matcher-0.5.5/assessment_episode_matcher/importers/assessments.py
+-rw-rw-rw-   0        0        0     6923 2024-05-29 20:10:49.000000 assessment_episode_matcher-0.5.5/assessment_episode_matcher/importers/episodes.py
+-rw-rw-rw-   0        0        0     3749 2024-05-27 00:19:22.000000 assessment_episode_matcher-0.5.5/assessment_episode_matcher/importers/main.py
+-rw-rw-rw-   0        0        0     1487 2024-05-29 18:44:02.000000 assessment_episode_matcher-0.5.5/assessment_episode_matcher/importers/nada_indexed.py
+drwxrwxrwx   0        0        0        0 2024-05-29 21:36:01.111349 assessment_episode_matcher-0.5.5/assessment_episode_matcher/matching/
+-rw-rw-rw-   0        0        0        0 2024-05-17 18:43:59.000000 assessment_episode_matcher-0.5.5/assessment_episode_matcher/matching/__init__.py
+-rw-rw-rw-   0        0        0     4474 2024-05-27 22:25:32.000000 assessment_episode_matcher-0.5.5/assessment_episode_matcher/matching/date_checks.py
+-rw-rw-rw-   0        0        0     5076 2024-05-29 21:33:28.000000 assessment_episode_matcher-0.5.5/assessment_episode_matcher/matching/errors.py
+-rw-rw-rw-   0        0        0     5321 2024-05-18 20:55:18.000000 assessment_episode_matcher-0.5.5/assessment_episode_matcher/matching/increasing_slack.py
+-rw-rw-rw-   0        0        0    22363 2024-05-28 07:22:56.000000 assessment_episode_matcher-0.5.5/assessment_episode_matcher/matching/main.py
+-rw-rw-rw-   0        0        0     1004 2024-05-17 18:43:59.000000 assessment_episode_matcher-0.5.5/assessment_episode_matcher/matching/matching_stats.py
+-rw-rw-rw-   0        0        0     2506 2024-05-27 22:23:53.000000 assessment_episode_matcher-0.5.5/assessment_episode_matcher/mytypes.py
+-rw-rw-rw-   0        0        0     4202 2024-05-29 20:38:39.000000 assessment_episode_matcher-0.5.5/assessment_episode_matcher/nada.py
+drwxrwxrwx   0        0        0        0 2024-05-29 21:36:01.130630 assessment_episode_matcher-0.5.5/assessment_episode_matcher/setup/
+-rw-rw-rw-   0        0        0        0 2024-05-19 22:35:00.000000 assessment_episode_matcher-0.5.5/assessment_episode_matcher/setup/__init__.py
+-rw-rw-rw-   0        0        0     4933 2024-05-26 00:16:34.000000 assessment_episode_matcher-0.5.5/assessment_episode_matcher/setup/bootstrap.py
+-rw-rw-rw-   0        0        0     2318 2024-05-19 22:34:48.000000 assessment_episode_matcher-0.5.5/assessment_episode_matcher/setup/log_management.py
+-rw-rw-rw-   0        0        0     9467 2024-05-29 20:17:37.000000 assessment_episode_matcher-0.5.5/assessment_episode_matcher/test_surveytxt.py
+-rw-rw-rw-   0        0        0     8555 2024-05-29 18:45:50.000000 assessment_episode_matcher-0.5.5/assessment_episode_matcher/test_surveytxt_local.py
+drwxrwxrwx   0        0        0        0 2024-05-29 21:36:01.143977 assessment_episode_matcher-0.5.5/assessment_episode_matcher/tests/
+-rw-rw-rw-   0        0        0       23 2024-05-17 18:43:59.000000 assessment_episode_matcher-0.5.5/assessment_episode_matcher/tests/__init__.py
+-rw-rw-rw-   0        0        0     1377 2024-05-17 18:43:59.000000 assessment_episode_matcher-0.5.5/assessment_episode_matcher/tests/matching_test.py
+drwxrwxrwx   0        0        0        0 2024-05-29 21:36:01.220367 assessment_episode_matcher-0.5.5/assessment_episode_matcher/utils/
+-rw-rw-rw-   0        0        0        0 2024-05-17 21:30:48.000000 assessment_episode_matcher-0.5.5/assessment_episode_matcher/utils/__init__.py
+-rw-rw-rw-   0        0        0     1270 2024-05-18 20:54:35.000000 assessment_episode_matcher-0.5.5/assessment_episode_matcher/utils/base.py
+-rw-rw-rw-   0        0        0     1693 2024-05-17 18:43:59.000000 assessment_episode_matcher-0.5.5/assessment_episode_matcher/utils/ccare_to_aztable.py
+-rw-rw-rw-   0        0        0    13615 2024-05-19 23:11:34.000000 assessment_episode_matcher-0.5.5/assessment_episode_matcher/utils/df_ops_base.py
+-rw-rw-rw-   0        0        0     7323 2024-05-18 19:37:57.000000 assessment_episode_matcher-0.5.5/assessment_episode_matcher/utils/dtypes.py
+-rw-rw-rw-   0        0        0     1355 2024-05-29 18:41:20.000000 assessment_episode_matcher-0.5.5/assessment_episode_matcher/utils/environment.py
+-rw-rw-rw-   0        0        0     2247 2024-05-28 06:45:09.000000 assessment_episode_matcher-0.5.5/assessment_episode_matcher/utils/fromstr.py
+-rw-rw-rw-   0        0        0      748 2024-05-17 18:43:59.000000 assessment_episode_matcher-0.5.5/assessment_episode_matcher/utils/group_utils.py
+-rw-rw-rw-   0        0        0    11458 2024-05-25 23:06:26.000000 assessment_episode_matcher-0.5.5/assessment_episode_matcher/utils/io.py
+-rw-rw-rw-   0        0        0       21 2024-05-29 20:11:05.000000 assessment_episode_matcher-0.5.5/assessment_episode_matcher/version.py
+drwxrwxrwx   0        0        0        0 2024-05-29 21:36:01.232649 assessment_episode_matcher-0.5.5/assessment_episode_matcher.egg-info/
+-rw-rw-rw-   0        0        0      523 2024-05-29 21:36:00.000000 assessment_episode_matcher-0.5.5/assessment_episode_matcher.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0     2429 2024-05-29 21:36:00.000000 assessment_episode_matcher-0.5.5/assessment_episode_matcher.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-05-29 21:36:00.000000 assessment_episode_matcher-0.5.5/assessment_episode_matcher.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0      105 2024-05-29 21:36:00.000000 assessment_episode_matcher-0.5.5/assessment_episode_matcher.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       27 2024-05-29 21:36:00.000000 assessment_episode_matcher-0.5.5/assessment_episode_matcher.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0      110 2024-05-17 19:08:24.000000 assessment_episode_matcher-0.5.5/requirements.txt
+-rw-rw-rw-   0        0        0       42 2024-05-29 21:36:01.241166 assessment_episode_matcher-0.5.5/setup.cfg
+-rw-rw-rw-   0        0        0     1342 2024-05-24 03:53:56.000000 assessment_episode_matcher-0.5.5/setup.py
```

### Comparing `assessment_episode_matcher-0.5.4/LICENSE` & `assessment_episode_matcher-0.5.5/LICENSE`

 * *Files identical despite different names*

### Comparing `assessment_episode_matcher-0.5.4/PKG-INFO` & `assessment_episode_matcher-0.5.5/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: assessment_episode_matcher
-Version: 0.5.4
+Version: 0.5.5
 Author: Aftab Jalal
 Author-email: mj@auditlytics.nz
 License: MIT
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.10
```

### Comparing `assessment_episode_matcher-0.5.4/README.md` & `assessment_episode_matcher-0.5.5/README.md`

 * *Files 14% similar despite different names*

```diff
@@ -25,8 +25,10 @@
 
 0.3.1 - removing disk writes as read-only on cloud fs
 0.4.0 - remove all local writes and reads, refactor, fix errors_warning writes
 0.5.0 - write redindexed to csv (instead of parq).
          Survey.txt write to blob storage.
 0.5.1 - AOD warnings, rename reindexed file to match format prefix_date-range_suffix: prefix:forstxt_
 0.5.2 - Fixed Destination Paths (on blob storage)
-0.5.3 - Load Blob Config for drug Mapping, etc
+0.5.3 - Load Blob Config for drug Mapping, etc
+0.5.4 - code path - no config - errors columns
+0.5.5 - LogWarn: imported dataset doesn't have one or more columns of interest
```

### Comparing `assessment_episode_matcher-0.5.4/assessment_episode_matcher/azutil/az_blob_query.py` & `assessment_episode_matcher-0.5.5/assessment_episode_matcher/azutil/az_blob_query.py`

 * *Files identical despite different names*

### Comparing `assessment_episode_matcher-0.5.4/assessment_episode_matcher/azutil/az_tables_query.py` & `assessment_episode_matcher-0.5.5/assessment_episode_matcher/azutil/az_tables_query.py`

 * *Files identical despite different names*

### Comparing `assessment_episode_matcher-0.5.4/assessment_episode_matcher/azutil/file_types.py` & `assessment_episode_matcher-0.5.5/assessment_episode_matcher/azutil/file_types.py`

 * *Files identical despite different names*

### Comparing `assessment_episode_matcher-0.5.4/assessment_episode_matcher/azutil/helper.py` & `assessment_episode_matcher-0.5.5/assessment_episode_matcher/azutil/helper.py`

 * *Files identical despite different names*

### Comparing `assessment_episode_matcher-0.5.4/assessment_episode_matcher/configs/audit.py` & `assessment_episode_matcher-0.5.5/assessment_episode_matcher/configs/audit.py`

 * *Files identical despite different names*

### Comparing `assessment_episode_matcher-0.5.4/assessment_episode_matcher/configs/episodes.py` & `assessment_episode_matcher-0.5.5/assessment_episode_matcher/configs/episodes.py`

 * *Files identical despite different names*

### Comparing `assessment_episode_matcher-0.5.4/assessment_episode_matcher/data_config.py` & `assessment_episode_matcher-0.5.5/assessment_episode_matcher/data_config.py`

 * *Files identical despite different names*

### Comparing `assessment_episode_matcher-0.5.4/assessment_episode_matcher/data_prep.py` & `assessment_episode_matcher-0.5.5/assessment_episode_matcher/data_prep.py`

 * *Files identical despite different names*

### Comparing `assessment_episode_matcher-0.5.4/assessment_episode_matcher/exporters/NADAbase.py` & `assessment_episode_matcher-0.5.5/assessment_episode_matcher/exporters/NADAbase.py`

 * *Files identical despite different names*

### Comparing `assessment_episode_matcher-0.5.4/assessment_episode_matcher/exporters/main.py` & `assessment_episode_matcher-0.5.5/assessment_episode_matcher/exporters/main.py`

 * *Files identical despite different names*

### Comparing `assessment_episode_matcher-0.5.4/assessment_episode_matcher/importers/aod.py` & `assessment_episode_matcher-0.5.5/assessment_episode_matcher/importers/aod.py`

 * *Files identical despite different names*

### Comparing `assessment_episode_matcher-0.5.4/assessment_episode_matcher/importers/assessments.py` & `assessment_episode_matcher-0.5.5/assessment_episode_matcher/importers/assessments.py`

 * *Files identical despite different names*

### Comparing `assessment_episode_matcher-0.5.4/assessment_episode_matcher/importers/episodes.py` & `assessment_episode_matcher-0.5.5/assessment_episode_matcher/importers/episodes.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,24 +1,32 @@
-from pathlib import Path
 import logging
 import pandas as pd
 from assessment_episode_matcher.configs import episodes as EpCfg
 from assessment_episode_matcher.data_config import EstablishmentID_Program
 from assessment_episode_matcher.importers.main import FileSource
 from assessment_episode_matcher.utils.dtypes import blank_to_today_str, convert_to_datetime
 from assessment_episode_matcher.utils.df_ops_base import has_data
 from assessment_episode_matcher.utils import io
 # from assessment_episode_matcher.setup.bootstrap import Bootstrap
 
 # from utils.io import read_parquet, write_parquet
+def get_cols_of_interest(df_columns) -> list[str]:
+  cols = [] 
+  for c in EpCfg.columns_of_interest:
+    if c in df_columns:
+      cols.append(c)
+    else:
+      logging.warn(f"Skipping Column from MDS dataset: {c}")
+  return cols
+  
 
 def prepare(ep_df1:pd.DataFrame) -> pd.DataFrame:
   # processed_folder = Bootstrap.get_path("processed_dir")
-
-  ep_df = ep_df1[EpCfg.columns_of_interest].copy()
+  cols = get_cols_of_interest(ep_df1.columns)
+  ep_df = ep_df1[cols].copy()
   ep_df['Program'] = ep_df['ESTABLISHMENT IDENTIFIER'].map(EstablishmentID_Program)
   
 #  convert_to_datetime(atom_df['AssessmentDate'], format='%Y%m%d')
   ep_df[EpCfg.date_cols[0]] = convert_to_datetime(ep_df[EpCfg.date_cols[0]],  format='%d%m%Y'
                                                   , fill_blanks=False)
   ep_df[EpCfg.date_cols[1]] = convert_to_datetime(ep_df[EpCfg.date_cols[1]],  format='%d%m%Y')
```

### Comparing `assessment_episode_matcher-0.5.4/assessment_episode_matcher/importers/main.py` & `assessment_episode_matcher-0.5.5/assessment_episode_matcher/importers/main.py`

 * *Files identical despite different names*

### Comparing `assessment_episode_matcher-0.5.4/assessment_episode_matcher/importers/nada_indexed.py` & `assessment_episode_matcher-0.5.5/assessment_episode_matcher/importers/nada_indexed.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 import logging
-from datetime import datetime
+# from datetime import datetime
 # from pathlib import Path
 import pandas as pd
 from assessment_episode_matcher.importers.main import FileSource, BlobFileSource
 from assessment_episode_matcher.utils import io
 
 #NADA
 def import_data(start_date:str, end_date:str
```

### Comparing `assessment_episode_matcher-0.5.4/assessment_episode_matcher/matching/date_checks.py` & `assessment_episode_matcher-0.5.5/assessment_episode_matcher/matching/date_checks.py`

 * *Files identical despite different names*

### Comparing `assessment_episode_matcher-0.5.4/assessment_episode_matcher/matching/errors.py` & `assessment_episode_matcher-0.5.5/assessment_episode_matcher/matching/errors.py`

 * *Files 8% similar despite different names*

```diff
@@ -34,15 +34,15 @@
     # only_in_errors = pd.concat([slk_prog_new, slk_onlyin_new])
 
     return slk_onlyin_error, slk_prog_warn
 
 
 def process_errors_warnings(ew:dict, warning_asmt_ids, merge_key2:str
                             ,period_start:date, period_end:date
-                            , audit_exporter:DataExporter):
+                            , audit_exporter:DataExporter) -> dict:
 
 
     slkonlyin_amst_error, slkprogonlyin_amst_warn = key_matching_errwarn_names(
         merge_key2
         , ew['slk_prog_onlyinass'], IssueType.SLKPROG_ONLY_IN_ASSESSMENT  # warni
         , ew['slk_onlyinass'], IssueType.CLIENT_ONLYIN_ASMT)  # error
 
@@ -81,32 +81,38 @@
     slkprogonlyin_ep_warn = slkprogonlyin_ep_warn[
        audit_cfg.COLUMNS_AUDIT_EPKEY_CLIENTPROG
         ]
     slkonlyin_amst_error = slkonlyin_amst_error[
         [k for k in audit_cfg.COLUMNS_AUDIT_ASMTKEY_CLIENT
         if k in slkonlyin_amst_error.columns
         ]
-    ]
-       
-
+    ]  
     slkprogonlyin_amst_warn = slkprogonlyin_amst_warn[audit_cfg.COLUMNS_AUDIT_ASMTKEY_CLIENTPROG]
 
-
     ew2 = {
        'dates_ew':final_dates_ew,
        'asmt_key_errors': slkonlyin_amst_error,
        'ep_key_errors': slkonlyin_ep_error,
        'asmt_key_warn': slkprogonlyin_amst_warn,
        'ep_key_warn': slkprogonlyin_ep_warn,
     }
     # write_validation_results(good_df, dates_ewdf, slk_program_keys_ewdf)
-    write_validation_results(ew2, audit_exporter)        
-
-
+    write_validation_results(ew2, audit_exporter)
 
+    return {
+       'errors' :{    
+          'dates_ew': len(final_dates_ew),
+          'asmt_key_errors': len(slkonlyin_amst_error),
+          'ep_key_errors': len(slkonlyin_ep_error),    
+       },
+       'warnings':{
+        'asmt_key_warn': len(slkprogonlyin_amst_warn),
+        'ep_key_warn': len(slkprogonlyin_ep_warn),
+       }
+    }  
 
 
 def write_validation_results(errors_warnings:dict[str, pd.DataFrame]
                              , audit_exporter: DataExporter):
     
     for ew_type_name, errs_warns in errors_warnings.items():
       if utdf.has_data(errs_warns):
```

### Comparing `assessment_episode_matcher-0.5.4/assessment_episode_matcher/matching/increasing_slack.py` & `assessment_episode_matcher-0.5.5/assessment_episode_matcher/matching/increasing_slack.py`

 * *Files identical despite different names*

### Comparing `assessment_episode_matcher-0.5.4/assessment_episode_matcher/matching/main.py` & `assessment_episode_matcher-0.5.5/assessment_episode_matcher/matching/main.py`

 * *Files identical despite different names*

### Comparing `assessment_episode_matcher-0.5.4/assessment_episode_matcher/matching/matching_stats.py` & `assessment_episode_matcher-0.5.5/assessment_episode_matcher/matching/matching_stats.py`

 * *Files identical despite different names*

### Comparing `assessment_episode_matcher-0.5.4/assessment_episode_matcher/mytypes.py` & `assessment_episode_matcher-0.5.5/assessment_episode_matcher/mytypes.py`

 * *Files identical despite different names*

### Comparing `assessment_episode_matcher-0.5.4/assessment_episode_matcher/nada.py` & `assessment_episode_matcher-0.5.5/assessment_episode_matcher/nada.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,14 +1,14 @@
-# from pathlib import Path
+import os
 import logging
 import pandas as pd
 
 from assessment_episode_matcher import project_directory
 from assessment_episode_matcher.setup.bootstrap import Bootstrap
-
+from assessment_episode_matcher.utils.environment import ConfigKeys
 from assessment_episode_matcher.exporters.main import AzureBlobExporter
 from assessment_episode_matcher.data_prep import prep_dataframe_nada
 from assessment_episode_matcher.exporters import NADAbase as nada_df_generator
 from assessment_episode_matcher.importers.main import  BlobFileSource
 from assessment_episode_matcher.mytypes import AODWarning, CSVTypeObject
 import assessment_episode_matcher.utils.df_ops_base as utdf
 import assessment_episode_matcher.importers.nada_indexed as io
@@ -42,59 +42,63 @@
               , prefix="forstxt_" #f"{st_dt}-{end_dt}"
               , suffix="_reindexed")
   return df, fname
 
 
 def generate_nada_save(reporting_start_str:str
                        , reporting_end_str :str
-                       , config:dict) -> list[AODWarning]|None:
-  container_name="atom-matching" 
+                       , config:dict
+                       , container:str) -> list[AODWarning]|None:
+
   p_str = f"{reporting_start_str}-{reporting_end_str}"
 
-  df_reindexed, fname  = get_matched_assessments(container_name, reporting_start_str, reporting_end_str)
+  df_reindexed, fname  = get_matched_assessments(container, reporting_start_str, reporting_end_str)
   if not utdf.has_data(df_reindexed):
     logging.error(f"No Indexed NADA data file with name {fname} could be found")
     return None
   
   nada, warnings_aod = generate_nada_export(df_reindexed, config)
   outfile = f"{p_str}/surveytxt_{p_str}.csv"
 
-  save_nada_data(nada, container=container_name, outfile=outfile)
+  save_nada_data(nada, container=container, outfile=outfile)
   msg = f"saved {len(nada)} NADA COMS records to {outfile}"
   logging.info(msg)
   return warnings_aod
   # print("Done. New file : ", nada_importfile.absolute())
 
 
-def load_blob_config():
-  config_file_source = BlobFileSource(container_name="atom-matching"
+def load_blob_config(container:str):
+  config_file_source = BlobFileSource(container_name=container
                                             , folder_path=".")
   config = config_file_source.load_json_file(filename="configuration.json", dtype=str)
   # print(config)
   return config
 
 
 def write_aod_warnings(data:list[AODWarning]
-                       , container_name:str, period_str:str) -> str:
+                       , container:str, period_str:str) -> str:
 
   outfile = f"NADA/{period_str}/aod_{period_str}_warn.csv"
   logging.info("Going to write AOD Warnings")
-  save_aod_warnings(data, container_name, outfile=outfile)
+  save_aod_warnings(data, container, outfile=outfile)
   return outfile
 
 
 def main ():
     # reporting_start_str, reporting_end_str =  '20231001', '20231231' # Q4 2023
-  config = load_blob_config()
+  container  = os.environ.get(ConfigKeys.AZURE_BLOB_CONTAINER.value)
+  if not container:
+      logging.exception(f"unable to proceed without app config {ConfigKeys.AZURE_BLOB_CONTAINER.value} ")
+      return
+  config = load_blob_config(container)
   reporting_start_str, reporting_end_str =  '20240101', '20240331' # Q1 2024
-  warnings_aod = generate_nada_save(reporting_start_str, reporting_end_str, config)
-  if warnings_aod:
-    container_name="atom-matching" 
+  warnings_aod = generate_nada_save(reporting_start_str, reporting_end_str, config, container)
+  if warnings_aod:    
     p_str = f"{reporting_start_str}-{reporting_end_str}"
-    outfile = write_aod_warnings(warnings_aod, container_name, period_str=p_str)
+    outfile = write_aod_warnings(warnings_aod, container, period_str=p_str)
     logging.info(f"Wrote AOD Warnings to {outfile}") 
 
 
 if __name__ == "__main__":
-  bstrap = Bootstrap.setup(project_directory, env="prod")
+  bstrap = Bootstrap.setup(project_directory, env="dev")
   res = main()
```

### Comparing `assessment_episode_matcher-0.5.4/assessment_episode_matcher/setup/bootstrap.py` & `assessment_episode_matcher-0.5.5/assessment_episode_matcher/setup/bootstrap.py`

 * *Files identical despite different names*

### Comparing `assessment_episode_matcher-0.5.4/assessment_episode_matcher/setup/log_management.py` & `assessment_episode_matcher-0.5.5/assessment_episode_matcher/setup/log_management.py`

 * *Files identical despite different names*

### Comparing `assessment_episode_matcher-0.5.4/assessment_episode_matcher/test_surveytxt.py` & `assessment_episode_matcher-0.5.5/assessment_episode_matcher/test_surveytxt.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,11 @@
+import os
 import logging
 import json
-from datetime import datetime
+
 # from pathlib import Path
 # import pandas as pd
 from assessment_episode_matcher import project_directory
 from assessment_episode_matcher.importers.main import BlobFileSource, FileSource
 from assessment_episode_matcher.setup.bootstrap import Bootstrap
 from assessment_episode_matcher.utils.environment import ConfigKeys
 from assessment_episode_matcher.utils.fromstr import get_date_from_str
@@ -40,34 +41,38 @@
 
 #     st = out_exporter.generate_finaloutput_df(res)
 #     # st.to_parquet('/data/out/surveytxt.parquet')
 #     st.to_csv(outfile, index=False)
         
 #     return st
 
-def load_blob_config():
-  config_file_source = BlobFileSource(container_name="atom-matching"
+def load_blob_config(container_name:str):
+  config_file_source = BlobFileSource(container_name=container_name
                                             , folder_path=".")
   config = config_file_source.load_json_file(filename="configuration.json", dtype=str)
   # print(config)
   return config
 
 def main3():
     # TODO:
     # envinronemnt setup : Config setup, Expected Directories create, logging setup
-    bstrap = Bootstrap.setup(project_directory, env="prod")
-    container = "atom-matching"
+    bstrap = Bootstrap.setup(project_directory, env="dev")
+    container  = os.environ.get(ConfigKeys.AZURE_BLOB_CONTAINER.value)
+    if not container:
+       logging.exception(f"unable to proceed without app config {ConfigKeys.AZURE_BLOB_CONTAINER.value} ")
+       return
+
     ep_folder, asmt_folder = "MDS", "ATOM"
     
     cfg = bstrap.config #, bstrap.logger
     # ConfigManager.setup('dev')
     # cfg = ConfigManager().config
     slack_for_matching = int(cfg.get(ConfigKeys.MATCHING_NDAYS_SLACK.value, 7))
     
-    reporting_start_str, reporting_end_str =  '20220101', '20240331'
+    reporting_start_str, reporting_end_str =  '20220101', '20231231'
 
     reporting_start, reporting_end = get_date_from_str (reporting_start_str,"%Y%m%d") \
                                       , get_date_from_str (reporting_end_str,"%Y%m%d")
 
     ep_file_source:FileSource = BlobFileSource(container_name=container
                                             , folder_path=ep_folder)
```

### Comparing `assessment_episode_matcher-0.5.4/assessment_episode_matcher/test_surveytxt_local.py` & `assessment_episode_matcher-0.5.5/assessment_episode_matcher/test_surveytxt_local.py`

 * *Files 2% similar despite different names*

```diff
@@ -39,16 +39,20 @@
         
 #     return st
     
 
 def main3():
     # TODO:
     # envinronemnt setup : Config setup, Expected Directories create, logging setup
-    # bstrap = Bootstrap.setup(project_directory, env="prod")
-    container = "atom-matching"
+    bstrap = Bootstrap.setup(project_directory, env="dev")
+    container  = os.environ.get(ConfigKeys.AZURE_BLOB_CONTAINER.value)
+    if not container:
+       logging.exception(f"unable to proceed without app config {ConfigKeys.AZURE_BLOB_CONTAINER.value} ")
+       return    
+    
     ep_folder, asmt_folder = "MDS", "ATOM"
     
     slack_for_matching = 7 # int(cfg.get(ConfigKeys.MATCHING_NDAYS_SLACK.value, 7))
     
     reporting_start_str, reporting_end_str =  '20220101', '20240331'
 
     reporting_start, reporting_end = get_date_from_str (reporting_start_str,"%Y%m%d") \
```

### Comparing `assessment_episode_matcher-0.5.4/assessment_episode_matcher/tests/matching_test.py` & `assessment_episode_matcher-0.5.5/assessment_episode_matcher/tests/matching_test.py`

 * *Files identical despite different names*

### Comparing `assessment_episode_matcher-0.5.4/assessment_episode_matcher/utils/base.py` & `assessment_episode_matcher-0.5.5/assessment_episode_matcher/utils/base.py`

 * *Files identical despite different names*

### Comparing `assessment_episode_matcher-0.5.4/assessment_episode_matcher/utils/ccare_to_aztable.py` & `assessment_episode_matcher-0.5.5/assessment_episode_matcher/utils/ccare_to_aztable.py`

 * *Files identical despite different names*

### Comparing `assessment_episode_matcher-0.5.4/assessment_episode_matcher/utils/df_ops_base.py` & `assessment_episode_matcher-0.5.5/assessment_episode_matcher/utils/df_ops_base.py`

 * *Files identical despite different names*

### Comparing `assessment_episode_matcher-0.5.4/assessment_episode_matcher/utils/dtypes.py` & `assessment_episode_matcher-0.5.5/assessment_episode_matcher/utils/dtypes.py`

 * *Files identical despite different names*

### Comparing `assessment_episode_matcher-0.5.4/assessment_episode_matcher/utils/environment.py` & `assessment_episode_matcher-0.5.5/assessment_episode_matcher/utils/environment.py`

 * *Files 5% similar despite different names*

```diff
@@ -8,15 +8,17 @@
 class ConfigKeys(Enum):
   REFRESH_ATOM_DATA = 'REFRESH_ATOM_DATA'
   TABLES_STORAGE_ENDPOINT_SUFFIX = 'TABLES_STORAGE_ENDPOINT_SUFFIX'
   TABLES_STORAGE_ACCOUNT_NAME = 'TABLES_STORAGE_ACCOUNT_NAME'
   AZURE_STORAGE_CONNECTION_STRING = 'AZURE_STORAGE_CONNECTION_STRING'
   AZURE_BLOB_CONNECTION_STRING ='AZURE_BLOB_CONNECTION_STRING'
   SURVEY_TABLE_NAME =  'SURVEY_TABLE_NAME'
-  MATCHING_NDAYS_SLACK = 'MATCHING_NDAYS_SLACK'
+  MATCHING_NDAYS_SLACK = 'MATCHING_NDAYS_SLACK',
+  AZURE_BLOB_CONTAINER = 'AZURE_BLOB_CONTAINER'
+
 
 class ConfigManager:
     _instance = None
     env:str
     env_config:dict
 
     def __new__(cls):
```

### Comparing `assessment_episode_matcher-0.5.4/assessment_episode_matcher/utils/fromstr.py` & `assessment_episode_matcher-0.5.5/assessment_episode_matcher/utils/fromstr.py`

 * *Files identical despite different names*

### Comparing `assessment_episode_matcher-0.5.4/assessment_episode_matcher/utils/group_utils.py` & `assessment_episode_matcher-0.5.5/assessment_episode_matcher/utils/group_utils.py`

 * *Files identical despite different names*

### Comparing `assessment_episode_matcher-0.5.4/assessment_episode_matcher/utils/io.py` & `assessment_episode_matcher-0.5.5/assessment_episode_matcher/utils/io.py`

 * *Files identical despite different names*

### Comparing `assessment_episode_matcher-0.5.4/assessment_episode_matcher.egg-info/PKG-INFO` & `assessment_episode_matcher-0.5.5/assessment_episode_matcher.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: assessment_episode_matcher
-Version: 0.5.4
+Version: 0.5.5
 Author: Aftab Jalal
 Author-email: mj@auditlytics.nz
 License: MIT
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.10
```

### Comparing `assessment_episode_matcher-0.5.4/assessment_episode_matcher.egg-info/SOURCES.txt` & `assessment_episode_matcher-0.5.5/assessment_episode_matcher.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `assessment_episode_matcher-0.5.4/setup.py` & `assessment_episode_matcher-0.5.5/setup.py`

 * *Files identical despite different names*

