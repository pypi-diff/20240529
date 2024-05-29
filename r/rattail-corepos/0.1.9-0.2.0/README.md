# Comparing `tmp/rattail_corepos-0.1.9.tar.gz` & `tmp/rattail_corepos-0.2.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/rattail_corepos-0.1.9.tar", last modified: Sat Nov  6 01:37:44 2021, max compression
+gzip compressed data, was "rattail_corepos-0.2.0.tar", last modified: Wed May 29 15:12:37 2024, max compression
```

## Comparing `rattail_corepos-0.1.9.tar` & `rattail_corepos-0.2.0.tar`

### file list

```diff
@@ -1,97 +1,144 @@
-drwxr-xr-x   0 lance     (1000) lance     (1000)        0 2021-11-06 01:37:44.000000 rattail_corepos-0.1.9/
--rw-r--r--   0 lance     (1000) lance     (1000)     1255 2021-11-06 01:37:19.000000 rattail_corepos-0.1.9/CHANGELOG.md
--rw-r--r--   0 lance     (1000) lance     (1000)    35147 2017-07-07 15:32:34.000000 rattail_corepos-0.1.9/COPYING.txt
--rw-r--r--   0 lance     (1000) lance     (1000)       93 2020-09-17 00:57:42.000000 rattail_corepos-0.1.9/MANIFEST.in
--rw-r--r--   0 lance     (1000) lance     (1000)     1201 2021-11-06 01:37:44.000000 rattail_corepos-0.1.9/PKG-INFO
--rw-r--r--   0 lance     (1000) lance     (1000)      345 2018-06-01 04:09:00.000000 rattail_corepos-0.1.9/README.rst
-drwxr-xr-x   0 lance     (1000) lance     (1000)        0 2021-11-06 01:37:44.000000 rattail_corepos-0.1.9/rattail_corepos/
--rw-r--r--   0 lance     (1000) lance     (1000)     1070 2018-06-01 04:33:19.000000 rattail_corepos-0.1.9/rattail_corepos/__init__.py
--rw-r--r--   0 lance     (1000) lance     (1000)       48 2021-11-06 01:37:23.000000 rattail_corepos-0.1.9/rattail_corepos/_version.py
-drwxr-xr-x   0 lance     (1000) lance     (1000)        0 2021-11-06 01:37:44.000000 rattail_corepos-0.1.9/rattail_corepos/batch/
--rw-r--r--   0 lance     (1000) lance     (1000)        0 2021-02-09 20:26:04.000000 rattail_corepos-0.1.9/rattail_corepos/batch/__init__.py
--rw-r--r--   0 lance     (1000) lance     (1000)    10044 2021-11-06 01:35:33.000000 rattail_corepos-0.1.9/rattail_corepos/batch/coremember.py
--rw-r--r--   0 lance     (1000) lance     (1000)     6505 2021-02-09 21:31:06.000000 rattail_corepos-0.1.9/rattail_corepos/batch/vendorcatalog.py
--rw-r--r--   0 lance     (1000) lance     (1000)     3667 2020-03-15 17:44:02.000000 rattail_corepos-0.1.9/rattail_corepos/commands.py
--rw-r--r--   0 lance     (1000) lance     (1000)     3244 2021-07-22 01:02:53.000000 rattail_corepos-0.1.9/rattail_corepos/config.py
-drwxr-xr-x   0 lance     (1000) lance     (1000)        0 2021-11-06 01:37:44.000000 rattail_corepos-0.1.9/rattail_corepos/corepos/
--rw-r--r--   0 lance     (1000) lance     (1000)        0 2017-02-13 03:47:53.000000 rattail_corepos-0.1.9/rattail_corepos/corepos/__init__.py
--rw-r--r--   0 lance     (1000) lance     (1000)     1168 2021-02-06 22:45:25.000000 rattail_corepos-0.1.9/rattail_corepos/corepos/api.py
--rw-r--r--   0 lance     (1000) lance     (1000)     6461 2020-03-27 23:34:20.000000 rattail_corepos-0.1.9/rattail_corepos/corepos/commands.py
-drwxr-xr-x   0 lance     (1000) lance     (1000)        0 2021-11-06 01:37:44.000000 rattail_corepos-0.1.9/rattail_corepos/corepos/common/
--rw-r--r--   0 lance     (1000) lance     (1000)        0 2017-02-13 03:47:53.000000 rattail_corepos-0.1.9/rattail_corepos/corepos/common/__init__.py
--rw-r--r--   0 lance     (1000) lance     (1000)     2498 2021-07-22 01:03:31.000000 rattail_corepos-0.1.9/rattail_corepos/corepos/common/importing.py
-drwxr-xr-x   0 lance     (1000) lance     (1000)        0 2021-11-06 01:37:44.000000 rattail_corepos-0.1.9/rattail_corepos/corepos/importing/
--rw-r--r--   0 lance     (1000) lance     (1000)      993 2020-03-04 05:05:54.000000 rattail_corepos-0.1.9/rattail_corepos/corepos/importing/__init__.py
-drwxr-xr-x   0 lance     (1000) lance     (1000)        0 2021-11-06 01:37:44.000000 rattail_corepos-0.1.9/rattail_corepos/corepos/importing/db/
--rw-r--r--   0 lance     (1000) lance     (1000)     1005 2020-03-04 05:01:24.000000 rattail_corepos-0.1.9/rattail_corepos/corepos/importing/db/__init__.py
--rw-r--r--   0 lance     (1000) lance     (1000)     4856 2021-01-30 02:05:34.000000 rattail_corepos-0.1.9/rattail_corepos/corepos/importing/db/corepos.py
--rw-r--r--   0 lance     (1000) lance     (1000)     1711 2020-03-04 05:00:32.000000 rattail_corepos-0.1.9/rattail_corepos/corepos/importing/db/csv.py
-drwxr-xr-x   0 lance     (1000) lance     (1000)        0 2021-11-06 01:37:44.000000 rattail_corepos-0.1.9/rattail_corepos/corepos/importing/db/exporters/
--rw-r--r--   0 lance     (1000) lance     (1000)      984 2020-03-27 23:33:53.000000 rattail_corepos-0.1.9/rattail_corepos/corepos/importing/db/exporters/__init__.py
--rw-r--r--   0 lance     (1000) lance     (1000)    27835 2020-04-16 01:54:35.000000 rattail_corepos-0.1.9/rattail_corepos/corepos/importing/db/exporters/catapult_inventory.py
--rw-r--r--   0 lance     (1000) lance     (1000)     7020 2020-07-21 20:07:49.000000 rattail_corepos-0.1.9/rattail_corepos/corepos/importing/db/exporters/catapult_membership.py
--rw-r--r--   0 lance     (1000) lance     (1000)     1642 2020-03-28 00:11:26.000000 rattail_corepos-0.1.9/rattail_corepos/corepos/importing/db/exporters/csv.py
--rw-r--r--   0 lance     (1000) lance     (1000)     4728 2021-01-30 02:05:22.000000 rattail_corepos-0.1.9/rattail_corepos/corepos/importing/db/model.py
--rw-r--r--   0 lance     (1000) lance     (1000)     6231 2020-03-04 05:02:05.000000 rattail_corepos-0.1.9/rattail_corepos/corepos/importing/db/square.py
--rw-r--r--   0 lance     (1000) lance     (1000)    14030 2021-02-09 21:41:22.000000 rattail_corepos-0.1.9/rattail_corepos/corepos/importing/model.py
--rw-r--r--   0 lance     (1000) lance     (1000)    10715 2021-01-22 00:15:49.000000 rattail_corepos-0.1.9/rattail_corepos/corepos/importing/rattail.py
-drwxr-xr-x   0 lance     (1000) lance     (1000)        0 2021-11-06 01:37:44.000000 rattail_corepos-0.1.9/rattail_corepos/corepos/lane/
--rw-r--r--   0 lance     (1000) lance     (1000)        0 2017-02-13 03:47:53.000000 rattail_corepos-0.1.9/rattail_corepos/corepos/lane/__init__.py
-drwxr-xr-x   0 lance     (1000) lance     (1000)        0 2021-11-06 01:37:44.000000 rattail_corepos-0.1.9/rattail_corepos/corepos/lane/importing/
--rw-r--r--   0 lance     (1000) lance     (1000)        0 2021-07-22 00:10:59.000000 rattail_corepos-0.1.9/rattail_corepos/corepos/lane/importing/__init__.py
-drwxr-xr-x   0 lance     (1000) lance     (1000)        0 2021-11-06 01:37:44.000000 rattail_corepos-0.1.9/rattail_corepos/corepos/lane/importing/op/
--rw-r--r--   0 lance     (1000) lance     (1000)     1008 2021-07-22 00:13:03.000000 rattail_corepos-0.1.9/rattail_corepos/corepos/lane/importing/op/__init__.py
--rw-r--r--   0 lance     (1000) lance     (1000)     1724 2021-11-04 22:15:41.000000 rattail_corepos-0.1.9/rattail_corepos/corepos/lane/importing/op/model.py
--rw-r--r--   0 lance     (1000) lance     (1000)     6393 2021-11-04 22:30:07.000000 rattail_corepos-0.1.9/rattail_corepos/corepos/lane/importing/op/office.py
-drwxr-xr-x   0 lance     (1000) lance     (1000)        0 2021-11-06 01:37:44.000000 rattail_corepos-0.1.9/rattail_corepos/corepos/office/
--rw-r--r--   0 lance     (1000) lance     (1000)        0 2017-02-13 03:47:53.000000 rattail_corepos-0.1.9/rattail_corepos/corepos/office/__init__.py
--rw-r--r--   0 lance     (1000) lance     (1000)     2884 2021-07-22 01:03:08.000000 rattail_corepos-0.1.9/rattail_corepos/corepos/office/commands.py
--rw-r--r--   0 lance     (1000) lance     (1000)     2682 2020-07-07 02:09:12.000000 rattail_corepos-0.1.9/rattail_corepos/corepos/util.py
-drwxr-xr-x   0 lance     (1000) lance     (1000)        0 2021-11-06 01:37:44.000000 rattail_corepos-0.1.9/rattail_corepos/datasync/
--rw-r--r--   0 lance     (1000) lance     (1000)        0 2020-03-15 18:37:54.000000 rattail_corepos-0.1.9/rattail_corepos/datasync/__init__.py
--rw-r--r--   0 lance     (1000) lance     (1000)    11303 2020-07-09 21:43:01.000000 rattail_corepos-0.1.9/rattail_corepos/datasync/corepos.py
--rw-r--r--   0 lance     (1000) lance     (1000)     7008 2021-02-09 22:10:46.000000 rattail_corepos-0.1.9/rattail_corepos/datasync/rattail.py
-drwxr-xr-x   0 lance     (1000) lance     (1000)        0 2021-11-06 01:37:44.000000 rattail_corepos-0.1.9/rattail_corepos/db/
--rw-r--r--   0 lance     (1000) lance     (1000)     1057 2018-06-01 04:32:57.000000 rattail_corepos-0.1.9/rattail_corepos/db/__init__.py
-drwxr-xr-x   0 lance     (1000) lance     (1000)        0 2021-11-06 01:37:44.000000 rattail_corepos-0.1.9/rattail_corepos/db/alembic/
-drwxr-xr-x   0 lance     (1000) lance     (1000)        0 2021-11-06 01:37:44.000000 rattail_corepos-0.1.9/rattail_corepos/db/alembic/versions/
--rw-r--r--   0 lance     (1000) lance     (1000)     2292 2020-09-04 23:30:43.000000 rattail_corepos-0.1.9/rattail_corepos/db/alembic/versions/130e4632a28a_add_corepos_product_cost.py
--rw-r--r--   0 lance     (1000) lance     (1000)     4955 2021-11-05 01:44:47.000000 rattail_corepos-0.1.9/rattail_corepos/db/alembic/versions/50961b4b854a_add_corepos_member_batch.py
--rw-r--r--   0 lance     (1000) lance     (1000)     2190 2021-01-28 03:02:23.000000 rattail_corepos-0.1.9/rattail_corepos/db/alembic/versions/7fea5aebddfb_add_store_extension.py
--rw-r--r--   0 lance     (1000) lance     (1000)     9679 2020-07-07 01:23:08.000000 rattail_corepos-0.1.9/rattail_corepos/db/alembic/versions/9c5029effe93_more_model_extensions.py
--rw-r--r--   0 lance     (1000) lance     (1000)     2191 2020-03-04 20:24:30.000000 rattail_corepos-0.1.9/rattail_corepos/db/alembic/versions/b43e93d32275_initial_core_pos_integration_tables.py
--rw-r--r--   0 lance     (1000) lance     (1000)     2188 2020-03-16 21:57:07.000000 rattail_corepos-0.1.9/rattail_corepos/db/alembic/versions/c61f78243ff3_add_person_extension.py
-drwxr-xr-x   0 lance     (1000) lance     (1000)        0 2021-11-06 01:37:44.000000 rattail_corepos-0.1.9/rattail_corepos/db/model/
--rw-r--r--   0 lance     (1000) lance     (1000)     1273 2021-11-04 23:26:04.000000 rattail_corepos-0.1.9/rattail_corepos/db/model/__init__.py
-drwxr-xr-x   0 lance     (1000) lance     (1000)        0 2021-11-06 01:37:44.000000 rattail_corepos-0.1.9/rattail_corepos/db/model/batch/
--rw-r--r--   0 lance     (1000) lance     (1000)        0 2021-11-04 23:20:13.000000 rattail_corepos-0.1.9/rattail_corepos/db/model/batch/__init__.py
--rw-r--r--   0 lance     (1000) lance     (1000)     3611 2021-11-05 01:44:43.000000 rattail_corepos-0.1.9/rattail_corepos/db/model/batch/coremember.py
--rw-r--r--   0 lance     (1000) lance     (1000)     4253 2020-07-31 02:07:27.000000 rattail_corepos-0.1.9/rattail_corepos/db/model/people.py
--rw-r--r--   0 lance     (1000) lance     (1000)     6396 2020-09-04 23:29:54.000000 rattail_corepos-0.1.9/rattail_corepos/db/model/products.py
--rw-r--r--   0 lance     (1000) lance     (1000)     2085 2021-01-28 03:09:50.000000 rattail_corepos-0.1.9/rattail_corepos/db/model/stores.py
--rw-r--r--   0 lance     (1000) lance     (1000)     1786 2021-07-22 16:43:47.000000 rattail_corepos-0.1.9/rattail_corepos/emails.py
-drwxr-xr-x   0 lance     (1000) lance     (1000)        0 2021-11-06 01:37:44.000000 rattail_corepos-0.1.9/rattail_corepos/importing/
--rw-r--r--   0 lance     (1000) lance     (1000)      992 2020-03-04 20:32:59.000000 rattail_corepos-0.1.9/rattail_corepos/importing/__init__.py
-drwxr-xr-x   0 lance     (1000) lance     (1000)        0 2021-11-06 01:37:44.000000 rattail_corepos-0.1.9/rattail_corepos/importing/corepos/
--rw-r--r--   0 lance     (1000) lance     (1000)     1029 2020-03-15 17:33:25.000000 rattail_corepos-0.1.9/rattail_corepos/importing/corepos/__init__.py
--rw-r--r--   0 lance     (1000) lance     (1000)    28359 2021-02-06 22:46:00.000000 rattail_corepos-0.1.9/rattail_corepos/importing/corepos/api.py
--rw-r--r--   0 lance     (1000) lance     (1000)     7254 2021-01-21 23:39:47.000000 rattail_corepos-0.1.9/rattail_corepos/importing/corepos/db.py
--rw-r--r--   0 lance     (1000) lance     (1000)     5555 2021-01-28 03:09:22.000000 rattail_corepos-0.1.9/rattail_corepos/importing/model.py
--rw-r--r--   0 lance     (1000) lance     (1000)     3037 2021-01-28 04:20:06.000000 rattail_corepos-0.1.9/rattail_corepos/importing/versions.py
--rw-r--r--   0 lance     (1000) lance     (1000)     1830 2021-01-21 23:40:04.000000 rattail_corepos-0.1.9/rattail_corepos/products.py
-drwxr-xr-x   0 lance     (1000) lance     (1000)        0 2021-11-06 01:37:44.000000 rattail_corepos-0.1.9/rattail_corepos/trainwreck/
--rw-r--r--   0 lance     (1000) lance     (1000)        0 2021-02-17 18:51:19.000000 rattail_corepos-0.1.9/rattail_corepos/trainwreck/__init__.py
--rw-r--r--   0 lance     (1000) lance     (1000)     1243 2021-02-19 00:01:32.000000 rattail_corepos-0.1.9/rattail_corepos/trainwreck/commands.py
-drwxr-xr-x   0 lance     (1000) lance     (1000)        0 2021-11-06 01:37:44.000000 rattail_corepos-0.1.9/rattail_corepos/trainwreck/importing/
--rw-r--r--   0 lance     (1000) lance     (1000)        0 2021-02-17 18:51:19.000000 rattail_corepos-0.1.9/rattail_corepos/trainwreck/importing/__init__.py
--rw-r--r--   0 lance     (1000) lance     (1000)     9071 2021-02-19 01:54:43.000000 rattail_corepos-0.1.9/rattail_corepos/trainwreck/importing/corepos.py
-drwxr-xr-x   0 lance     (1000) lance     (1000)        0 2021-11-06 01:37:44.000000 rattail_corepos-0.1.9/rattail_corepos.egg-info/
--rw-r--r--   0 lance     (1000) lance     (1000)     1201 2021-11-06 01:37:44.000000 rattail_corepos-0.1.9/rattail_corepos.egg-info/PKG-INFO
--rw-r--r--   0 lance     (1000) lance     (1000)     3026 2021-11-06 01:37:44.000000 rattail_corepos-0.1.9/rattail_corepos.egg-info/SOURCES.txt
--rw-r--r--   0 lance     (1000) lance     (1000)        1 2021-11-06 01:37:44.000000 rattail_corepos-0.1.9/rattail_corepos.egg-info/dependency_links.txt
--rw-r--r--   0 lance     (1000) lance     (1000)      910 2021-11-06 01:37:44.000000 rattail_corepos-0.1.9/rattail_corepos.egg-info/entry_points.txt
--rw-r--r--   0 lance     (1000) lance     (1000)        1 2021-11-06 01:37:44.000000 rattail_corepos-0.1.9/rattail_corepos.egg-info/not-zip-safe
--rw-r--r--   0 lance     (1000) lance     (1000)       18 2021-11-06 01:37:44.000000 rattail_corepos-0.1.9/rattail_corepos.egg-info/requires.txt
--rw-r--r--   0 lance     (1000) lance     (1000)       16 2021-11-06 01:37:44.000000 rattail_corepos-0.1.9/rattail_corepos.egg-info/top_level.txt
--rw-r--r--   0 lance     (1000) lance     (1000)       38 2021-11-06 01:37:44.000000 rattail_corepos-0.1.9/setup.cfg
--rw-r--r--   0 lance     (1000) lance     (1000)     4947 2021-07-22 00:36:59.000000 rattail_corepos-0.1.9/setup.py
+drwxr-xr-x   0 lance     (1000) lance     (1000)        0 2024-05-29 15:12:37.829058 rattail_corepos-0.2.0/
+-rw-r--r--   0 lance     (1000) lance     (1000)     6876 2024-05-29 15:12:13.000000 rattail_corepos-0.2.0/CHANGELOG.md
+-rw-r--r--   0 lance     (1000) lance     (1000)    35147 2017-07-07 15:32:34.000000 rattail_corepos-0.2.0/COPYING.txt
+-rw-r--r--   0 lance     (1000) lance     (1000)      209 2023-06-02 19:16:03.000000 rattail_corepos-0.2.0/MANIFEST.in
+-rw-r--r--   0 lance     (1000) lance     (1000)     1229 2024-05-29 15:12:37.829058 rattail_corepos-0.2.0/PKG-INFO
+-rw-r--r--   0 lance     (1000) lance     (1000)      345 2018-06-01 04:09:00.000000 rattail_corepos-0.2.0/README.rst
+drwxr-xr-x   0 lance     (1000) lance     (1000)        0 2024-05-29 15:12:37.813058 rattail_corepos-0.2.0/rattail_corepos/
+-rw-r--r--   0 lance     (1000) lance     (1000)     1070 2018-06-01 04:33:19.000000 rattail_corepos-0.2.0/rattail_corepos/__init__.py
+-rw-r--r--   0 lance     (1000) lance     (1000)       48 2024-05-29 15:12:22.000000 rattail_corepos-0.2.0/rattail_corepos/_version.py
+-rw-r--r--   0 lance     (1000) lance     (1000)     5387 2024-05-09 01:13:48.000000 rattail_corepos-0.2.0/rattail_corepos/app.py
+-rw-r--r--   0 lance     (1000) lance     (1000)     2996 2023-10-02 00:42:13.000000 rattail_corepos-0.2.0/rattail_corepos/auth.py
+drwxr-xr-x   0 lance     (1000) lance     (1000)        0 2024-05-29 15:12:37.813058 rattail_corepos-0.2.0/rattail_corepos/batch/
+-rw-r--r--   0 lance     (1000) lance     (1000)        0 2021-02-09 20:26:04.000000 rattail_corepos-0.2.0/rattail_corepos/batch/__init__.py
+-rw-r--r--   0 lance     (1000) lance     (1000)    10140 2023-06-12 22:39:50.000000 rattail_corepos-0.2.0/rattail_corepos/batch/coremember.py
+-rw-r--r--   0 lance     (1000) lance     (1000)     7199 2023-11-05 20:07:57.000000 rattail_corepos-0.2.0/rattail_corepos/batch/equityimport.py
+-rw-r--r--   0 lance     (1000) lance     (1000)    10103 2023-10-20 19:35:51.000000 rattail_corepos-0.2.0/rattail_corepos/batch/pos.py
+-rw-r--r--   0 lance     (1000) lance     (1000)     6461 2023-09-19 11:49:12.000000 rattail_corepos-0.2.0/rattail_corepos/batch/vendorcatalog.py
+-rw-r--r--   0 lance     (1000) lance     (1000)     6071 2024-05-17 00:15:47.000000 rattail_corepos-0.2.0/rattail_corepos/commands.py
+-rw-r--r--   0 lance     (1000) lance     (1000)    11507 2023-10-05 16:51:47.000000 rattail_corepos-0.2.0/rattail_corepos/config.py
+drwxr-xr-x   0 lance     (1000) lance     (1000)        0 2024-05-29 15:12:37.817058 rattail_corepos-0.2.0/rattail_corepos/corepos/
+-rw-r--r--   0 lance     (1000) lance     (1000)        0 2017-02-13 03:47:53.000000 rattail_corepos-0.2.0/rattail_corepos/corepos/__init__.py
+-rw-r--r--   0 lance     (1000) lance     (1000)     1303 2023-09-17 17:15:46.000000 rattail_corepos-0.2.0/rattail_corepos/corepos/api.py
+-rw-r--r--   0 lance     (1000) lance     (1000)     2997 2024-05-16 04:11:41.000000 rattail_corepos-0.2.0/rattail_corepos/corepos/commands.py
+drwxr-xr-x   0 lance     (1000) lance     (1000)        0 2024-05-29 15:12:37.817058 rattail_corepos-0.2.0/rattail_corepos/corepos/common/
+-rw-r--r--   0 lance     (1000) lance     (1000)        0 2017-02-13 03:47:53.000000 rattail_corepos-0.2.0/rattail_corepos/corepos/common/__init__.py
+-rw-r--r--   0 lance     (1000) lance     (1000)     2498 2021-07-22 01:03:31.000000 rattail_corepos-0.2.0/rattail_corepos/corepos/common/importing.py
+drwxr-xr-x   0 lance     (1000) lance     (1000)        0 2024-05-29 15:12:37.817058 rattail_corepos-0.2.0/rattail_corepos/corepos/importing/
+-rw-r--r--   0 lance     (1000) lance     (1000)     1237 2023-05-08 19:41:30.000000 rattail_corepos-0.2.0/rattail_corepos/corepos/importing/__init__.py
+drwxr-xr-x   0 lance     (1000) lance     (1000)        0 2024-05-29 15:12:37.817058 rattail_corepos-0.2.0/rattail_corepos/corepos/importing/db/
+-rw-r--r--   0 lance     (1000) lance     (1000)     1252 2023-05-08 19:43:31.000000 rattail_corepos-0.2.0/rattail_corepos/corepos/importing/db/__init__.py
+-rw-r--r--   0 lance     (1000) lance     (1000)     1252 2023-05-08 19:42:56.000000 rattail_corepos-0.2.0/rattail_corepos/corepos/importing/db/corepos.py
+-rw-r--r--   0 lance     (1000) lance     (1000)     1239 2023-05-08 19:43:19.000000 rattail_corepos-0.2.0/rattail_corepos/corepos/importing/db/csv.py
+drwxr-xr-x   0 lance     (1000) lance     (1000)        0 2024-05-29 15:12:37.817058 rattail_corepos-0.2.0/rattail_corepos/corepos/importing/db/exporters/
+-rw-r--r--   0 lance     (1000) lance     (1000)     1262 2023-05-08 19:45:26.000000 rattail_corepos-0.2.0/rattail_corepos/corepos/importing/db/exporters/__init__.py
+-rw-r--r--   0 lance     (1000) lance     (1000)     1280 2023-05-08 19:44:49.000000 rattail_corepos-0.2.0/rattail_corepos/corepos/importing/db/exporters/catapult_inventory.py
+-rw-r--r--   0 lance     (1000) lance     (1000)     1282 2023-05-08 19:45:01.000000 rattail_corepos-0.2.0/rattail_corepos/corepos/importing/db/exporters/catapult_membership.py
+-rw-r--r--   0 lance     (1000) lance     (1000)     1246 2023-05-08 19:45:16.000000 rattail_corepos-0.2.0/rattail_corepos/corepos/importing/db/exporters/csv.py
+-rw-r--r--   0 lance     (1000) lance     (1000)     1254 2023-05-08 19:43:51.000000 rattail_corepos-0.2.0/rattail_corepos/corepos/importing/db/model.py
+-rw-r--r--   0 lance     (1000) lance     (1000)     1252 2023-05-08 19:44:03.000000 rattail_corepos-0.2.0/rattail_corepos/corepos/importing/db/square.py
+-rw-r--r--   0 lance     (1000) lance     (1000)     1257 2023-05-08 19:41:53.000000 rattail_corepos-0.2.0/rattail_corepos/corepos/importing/model.py
+-rw-r--r--   0 lance     (1000) lance     (1000)     1248 2023-05-08 19:42:03.000000 rattail_corepos-0.2.0/rattail_corepos/corepos/importing/rattail.py
+drwxr-xr-x   0 lance     (1000) lance     (1000)        0 2024-05-29 15:12:37.817058 rattail_corepos-0.2.0/rattail_corepos/corepos/lane/
+-rw-r--r--   0 lance     (1000) lance     (1000)        0 2017-02-13 03:47:53.000000 rattail_corepos-0.2.0/rattail_corepos/corepos/lane/__init__.py
+drwxr-xr-x   0 lance     (1000) lance     (1000)        0 2024-05-29 15:12:37.817058 rattail_corepos-0.2.0/rattail_corepos/corepos/lane/importing/
+-rw-r--r--   0 lance     (1000) lance     (1000)        0 2021-07-22 00:10:59.000000 rattail_corepos-0.2.0/rattail_corepos/corepos/lane/importing/__init__.py
+drwxr-xr-x   0 lance     (1000) lance     (1000)        0 2024-05-29 15:12:37.817058 rattail_corepos-0.2.0/rattail_corepos/corepos/lane/importing/op/
+-rw-r--r--   0 lance     (1000) lance     (1000)     1008 2021-07-22 00:13:03.000000 rattail_corepos-0.2.0/rattail_corepos/corepos/lane/importing/op/__init__.py
+-rw-r--r--   0 lance     (1000) lance     (1000)     1738 2023-06-13 01:04:31.000000 rattail_corepos-0.2.0/rattail_corepos/corepos/lane/importing/op/model.py
+-rw-r--r--   0 lance     (1000) lance     (1000)     6600 2023-06-13 01:04:31.000000 rattail_corepos-0.2.0/rattail_corepos/corepos/lane/importing/op/office.py
+drwxr-xr-x   0 lance     (1000) lance     (1000)        0 2024-05-29 15:12:37.817058 rattail_corepos-0.2.0/rattail_corepos/corepos/office/
+-rw-r--r--   0 lance     (1000) lance     (1000)        0 2017-02-13 03:47:53.000000 rattail_corepos-0.2.0/rattail_corepos/corepos/office/__init__.py
+-rw-r--r--   0 lance     (1000) lance     (1000)     5098 2024-05-16 03:09:10.000000 rattail_corepos-0.2.0/rattail_corepos/corepos/office/anonymize.py
+-rw-r--r--   0 lance     (1000) lance     (1000)     7546 2024-05-16 23:59:46.000000 rattail_corepos-0.2.0/rattail_corepos/corepos/office/commands.py
+drwxr-xr-x   0 lance     (1000) lance     (1000)        0 2024-05-29 15:12:37.821058 rattail_corepos-0.2.0/rattail_corepos/corepos/office/importing/
+-rw-r--r--   0 lance     (1000) lance     (1000)      993 2023-05-08 19:39:54.000000 rattail_corepos-0.2.0/rattail_corepos/corepos/office/importing/__init__.py
+drwxr-xr-x   0 lance     (1000) lance     (1000)        0 2024-05-29 15:12:37.821058 rattail_corepos-0.2.0/rattail_corepos/corepos/office/importing/db/
+-rw-r--r--   0 lance     (1000) lance     (1000)     1005 2023-05-08 19:39:54.000000 rattail_corepos-0.2.0/rattail_corepos/corepos/office/importing/db/__init__.py
+-rw-r--r--   0 lance     (1000) lance     (1000)     4818 2023-10-05 16:59:20.000000 rattail_corepos-0.2.0/rattail_corepos/corepos/office/importing/db/corepos.py
+-rw-r--r--   0 lance     (1000) lance     (1000)     2134 2024-05-08 19:50:25.000000 rattail_corepos-0.2.0/rattail_corepos/corepos/office/importing/db/csv.py
+drwxr-xr-x   0 lance     (1000) lance     (1000)        0 2024-05-29 15:12:37.821058 rattail_corepos-0.2.0/rattail_corepos/corepos/office/importing/db/exporters/
+-rw-r--r--   0 lance     (1000) lance     (1000)      984 2023-05-08 19:39:54.000000 rattail_corepos-0.2.0/rattail_corepos/corepos/office/importing/db/exporters/__init__.py
+-rw-r--r--   0 lance     (1000) lance     (1000)    27834 2023-05-08 19:39:54.000000 rattail_corepos-0.2.0/rattail_corepos/corepos/office/importing/db/exporters/catapult_inventory.py
+-rw-r--r--   0 lance     (1000) lance     (1000)     7075 2023-06-13 01:04:31.000000 rattail_corepos-0.2.0/rattail_corepos/corepos/office/importing/db/exporters/catapult_membership.py
+-rw-r--r--   0 lance     (1000) lance     (1000)     1649 2023-10-04 04:14:39.000000 rattail_corepos-0.2.0/rattail_corepos/corepos/office/importing/db/exporters/csv.py
+-rw-r--r--   0 lance     (1000) lance     (1000)     3164 2023-10-04 23:24:32.000000 rattail_corepos-0.2.0/rattail_corepos/corepos/office/importing/db/local.py
+-rw-r--r--   0 lance     (1000) lance     (1000)    11105 2024-05-08 19:50:43.000000 rattail_corepos-0.2.0/rattail_corepos/corepos/office/importing/db/model.py
+-rw-r--r--   0 lance     (1000) lance     (1000)     6237 2023-05-08 19:56:46.000000 rattail_corepos-0.2.0/rattail_corepos/corepos/office/importing/db/square.py
+-rw-r--r--   0 lance     (1000) lance     (1000)    15816 2023-09-18 13:11:31.000000 rattail_corepos-0.2.0/rattail_corepos/corepos/office/importing/model.py
+-rw-r--r--   0 lance     (1000) lance     (1000)    11291 2023-09-08 01:59:06.000000 rattail_corepos-0.2.0/rattail_corepos/corepos/office/importing/rattail.py
+-rw-r--r--   0 lance     (1000) lance     (1000)     3712 2024-05-16 03:46:38.000000 rattail_corepos-0.2.0/rattail_corepos/corepos/office/patcher.py
+drwxr-xr-x   0 lance     (1000) lance     (1000)        0 2024-05-29 15:12:37.821058 rattail_corepos-0.2.0/rattail_corepos/corepos/office/scripts/
+-rw-r--r--   0 lance     (1000) lance     (1000)      738 2021-07-22 15:07:25.000000 rattail_corepos-0.2.0/rattail_corepos/corepos/office/scripts/parse-fannie-config.php
+-rw-r--r--   0 lance     (1000) lance     (1000)     1013 2023-11-18 15:22:35.000000 rattail_corepos-0.2.0/rattail_corepos/corepos/office/scripts/update-fannie-config.php
+-rw-r--r--   0 lance     (1000) lance     (1000)     4472 2023-11-18 18:11:03.000000 rattail_corepos-0.2.0/rattail_corepos/corepos/office/util.py
+-rw-r--r--   0 lance     (1000) lance     (1000)     2819 2023-10-04 23:06:22.000000 rattail_corepos-0.2.0/rattail_corepos/corepos/util.py
+drwxr-xr-x   0 lance     (1000) lance     (1000)        0 2024-05-29 15:12:37.821058 rattail_corepos-0.2.0/rattail_corepos/datasync/
+-rw-r--r--   0 lance     (1000) lance     (1000)        0 2020-03-15 18:37:54.000000 rattail_corepos-0.2.0/rattail_corepos/datasync/__init__.py
+-rw-r--r--   0 lance     (1000) lance     (1000)    11582 2023-06-11 03:26:38.000000 rattail_corepos-0.2.0/rattail_corepos/datasync/corepos.py
+-rw-r--r--   0 lance     (1000) lance     (1000)     6936 2023-09-18 13:09:54.000000 rattail_corepos-0.2.0/rattail_corepos/datasync/rattail.py
+drwxr-xr-x   0 lance     (1000) lance     (1000)        0 2024-05-29 15:12:37.821058 rattail_corepos-0.2.0/rattail_corepos/db/
+-rw-r--r--   0 lance     (1000) lance     (1000)     1041 2021-12-31 03:48:53.000000 rattail_corepos-0.2.0/rattail_corepos/db/__init__.py
+drwxr-xr-x   0 lance     (1000) lance     (1000)        0 2024-05-29 15:12:37.809057 rattail_corepos-0.2.0/rattail_corepos/db/alembic/
+drwxr-xr-x   0 lance     (1000) lance     (1000)        0 2024-05-29 15:12:37.825058 rattail_corepos-0.2.0/rattail_corepos/db/alembic/versions/
+-rw-r--r--   0 lance     (1000) lance     (1000)     3144 2023-09-06 22:47:24.000000 rattail_corepos-0.2.0/rattail_corepos/db/alembic/versions/08d879bbe118_add_memberequitypayment_extension.py
+-rw-r--r--   0 lance     (1000) lance     (1000)     2292 2020-09-04 23:30:43.000000 rattail_corepos-0.2.0/rattail_corepos/db/alembic/versions/130e4632a28a_add_corepos_product_cost.py
+-rw-r--r--   0 lance     (1000) lance     (1000)     1070 2023-10-12 14:50:06.000000 rattail_corepos-0.2.0/rattail_corepos/db/alembic/versions/15bf65f68c52_add_core_member_corepos_card_number.py
+-rw-r--r--   0 lance     (1000) lance     (1000)     2249 2023-10-02 00:42:13.000000 rattail_corepos-0.2.0/rattail_corepos/db/alembic/versions/1f2e2f57c90b_add_core_employee.py
+-rw-r--r--   0 lance     (1000) lance     (1000)     4955 2021-11-05 01:44:47.000000 rattail_corepos-0.2.0/rattail_corepos/db/alembic/versions/50961b4b854a_add_corepos_member_batch.py
+-rw-r--r--   0 lance     (1000) lance     (1000)     2135 2023-10-07 21:27:51.000000 rattail_corepos-0.2.0/rattail_corepos/db/alembic/versions/673ff7088d35_add_corepos_tax.py
+-rw-r--r--   0 lance     (1000) lance     (1000)     2190 2021-01-28 03:02:23.000000 rattail_corepos-0.2.0/rattail_corepos/db/alembic/versions/7fea5aebddfb_add_store_extension.py
+-rw-r--r--   0 lance     (1000) lance     (1000)     4538 2023-09-13 17:29:14.000000 rattail_corepos-0.2.0/rattail_corepos/db/alembic/versions/93978a7adc66_add_equity_import_batch.py
+-rw-r--r--   0 lance     (1000) lance     (1000)     9679 2020-07-07 01:23:08.000000 rattail_corepos-0.2.0/rattail_corepos/db/alembic/versions/9c5029effe93_more_model_extensions.py
+-rw-r--r--   0 lance     (1000) lance     (1000)     1076 2023-06-06 00:10:10.000000 rattail_corepos-0.2.0/rattail_corepos/db/alembic/versions/ae74c537ea51_add_customer_card_number.py
+-rw-r--r--   0 lance     (1000) lance     (1000)     2440 2023-06-10 18:47:42.000000 rattail_corepos-0.2.0/rattail_corepos/db/alembic/versions/b025df7cf41b_add_customershopper_corepos_customer_id.py
+-rw-r--r--   0 lance     (1000) lance     (1000)     2191 2020-03-04 20:24:30.000000 rattail_corepos-0.2.0/rattail_corepos/db/alembic/versions/b43e93d32275_initial_core_pos_integration_tables.py
+-rw-r--r--   0 lance     (1000) lance     (1000)     1391 2023-10-20 16:39:23.000000 rattail_corepos-0.2.0/rattail_corepos/db/alembic/versions/b5a8734b1fe0_fix_fk_for_coreproductcost.py
+-rw-r--r--   0 lance     (1000) lance     (1000)     2193 2023-09-26 23:22:59.000000 rattail_corepos-0.2.0/rattail_corepos/db/alembic/versions/c40a6ec00428_add_tender.py
+-rw-r--r--   0 lance     (1000) lance     (1000)     2188 2020-03-16 21:57:07.000000 rattail_corepos-0.2.0/rattail_corepos/db/alembic/versions/c61f78243ff3_add_person_extension.py
+-rw-r--r--   0 lance     (1000) lance     (1000)      884 2023-09-14 02:24:51.000000 rattail_corepos-0.2.0/rattail_corepos/db/alembic/versions/d426a274f0c2_add_equity_payment_corepos_datetime.py
+-rw-r--r--   0 lance     (1000) lance     (1000)      691 2022-03-15 16:25:01.000000 rattail_corepos-0.2.0/rattail_corepos/db/alembic/versions/d6a0f21a6a94_add_card_number_raw_for_member_import.py
+-rw-r--r--   0 lance     (1000) lance     (1000)      661 2023-09-16 20:38:40.000000 rattail_corepos-0.2.0/rattail_corepos/db/alembic/versions/f8df04546a59_add_equity_import_tender_code.py
+drwxr-xr-x   0 lance     (1000) lance     (1000)        0 2024-05-29 15:12:37.825058 rattail_corepos-0.2.0/rattail_corepos/db/model/
+-rw-r--r--   0 lance     (1000) lance     (1000)     1478 2023-10-07 02:00:49.000000 rattail_corepos-0.2.0/rattail_corepos/db/model/__init__.py
+-rw-r--r--   0 lance     (1000) lance     (1000)     1069 2023-10-02 00:42:13.000000 rattail_corepos-0.2.0/rattail_corepos/db/model/_complete.py
+drwxr-xr-x   0 lance     (1000) lance     (1000)        0 2024-05-29 15:12:37.829058 rattail_corepos-0.2.0/rattail_corepos/db/model/batch/
+-rw-r--r--   0 lance     (1000) lance     (1000)        0 2021-11-04 23:20:13.000000 rattail_corepos-0.2.0/rattail_corepos/db/model/batch/__init__.py
+-rw-r--r--   0 lance     (1000) lance     (1000)     3680 2022-03-15 16:23:44.000000 rattail_corepos-0.2.0/rattail_corepos/db/model/batch/coremember.py
+-rw-r--r--   0 lance     (1000) lance     (1000)     3923 2023-09-16 20:37:58.000000 rattail_corepos-0.2.0/rattail_corepos/db/model/batch/equityimport.py
+-rw-r--r--   0 lance     (1000) lance     (1000)     9354 2023-10-12 13:54:51.000000 rattail_corepos-0.2.0/rattail_corepos/db/model/people.py
+-rw-r--r--   0 lance     (1000) lance     (1000)     6894 2023-10-20 16:39:07.000000 rattail_corepos-0.2.0/rattail_corepos/db/model/products.py
+-rw-r--r--   0 lance     (1000) lance     (1000)     4086 2023-10-07 02:00:42.000000 rattail_corepos-0.2.0/rattail_corepos/db/model/stores.py
+-rw-r--r--   0 lance     (1000) lance     (1000)     3452 2023-09-02 18:41:04.000000 rattail_corepos-0.2.0/rattail_corepos/emails.py
+drwxr-xr-x   0 lance     (1000) lance     (1000)        0 2024-05-29 15:12:37.829058 rattail_corepos-0.2.0/rattail_corepos/importing/
+-rw-r--r--   0 lance     (1000) lance     (1000)      992 2020-03-04 20:32:59.000000 rattail_corepos-0.2.0/rattail_corepos/importing/__init__.py
+drwxr-xr-x   0 lance     (1000) lance     (1000)        0 2024-05-29 15:12:37.829058 rattail_corepos-0.2.0/rattail_corepos/importing/corepos/
+-rw-r--r--   0 lance     (1000) lance     (1000)     1029 2020-03-15 17:33:25.000000 rattail_corepos-0.2.0/rattail_corepos/importing/corepos/__init__.py
+-rw-r--r--   0 lance     (1000) lance     (1000)    31089 2024-05-10 01:46:32.000000 rattail_corepos-0.2.0/rattail_corepos/importing/corepos/api.py
+-rw-r--r--   0 lance     (1000) lance     (1000)    33939 2023-11-15 17:38:27.000000 rattail_corepos-0.2.0/rattail_corepos/importing/corepos/db.py
+-rw-r--r--   0 lance     (1000) lance     (1000)     6511 2023-10-20 16:36:12.000000 rattail_corepos-0.2.0/rattail_corepos/importing/model.py
+-rw-r--r--   0 lance     (1000) lance     (1000)     3764 2023-10-02 00:42:13.000000 rattail_corepos-0.2.0/rattail_corepos/importing/versions.py
+drwxr-xr-x   0 lance     (1000) lance     (1000)        0 2024-05-29 15:12:37.829058 rattail_corepos-0.2.0/rattail_corepos/problems/
+-rw-r--r--   0 lance     (1000) lance     (1000)        0 2023-06-02 18:35:56.000000 rattail_corepos-0.2.0/rattail_corepos/problems/__init__.py
+-rw-r--r--   0 lance     (1000) lance     (1000)     3002 2023-09-02 18:47:42.000000 rattail_corepos-0.2.0/rattail_corepos/problems/corepos.py
+-rw-r--r--   0 lance     (1000) lance     (1000)     1830 2021-01-21 23:40:04.000000 rattail_corepos-0.2.0/rattail_corepos/products.py
+drwxr-xr-x   0 lance     (1000) lance     (1000)        0 2024-05-29 15:12:37.809057 rattail_corepos-0.2.0/rattail_corepos/templates/
+drwxr-xr-x   0 lance     (1000) lance     (1000)        0 2024-05-29 15:12:37.829058 rattail_corepos-0.2.0/rattail_corepos/templates/mail/
+-rw-r--r--   0 lance     (1000) lance     (1000)      769 2023-06-02 18:47:54.000000 rattail_corepos-0.2.0/rattail_corepos/templates/mail/corepos_problems_invalid_person_numbers.html.mako
+-rw-r--r--   0 lance     (1000) lance     (1000)      503 2023-09-02 18:38:37.000000 rattail_corepos-0.2.0/rattail_corepos/templates/mail/corepos_problems_phone_numbers_too_long.html.mako
+drwxr-xr-x   0 lance     (1000) lance     (1000)        0 2024-05-29 15:12:37.829058 rattail_corepos-0.2.0/rattail_corepos/trainwreck/
+-rw-r--r--   0 lance     (1000) lance     (1000)        0 2021-02-17 18:51:19.000000 rattail_corepos-0.2.0/rattail_corepos/trainwreck/__init__.py
+-rw-r--r--   0 lance     (1000) lance     (1000)     1638 2024-05-16 01:48:36.000000 rattail_corepos-0.2.0/rattail_corepos/trainwreck/commands.py
+drwxr-xr-x   0 lance     (1000) lance     (1000)        0 2024-05-29 15:12:37.829058 rattail_corepos-0.2.0/rattail_corepos/trainwreck/importing/
+-rw-r--r--   0 lance     (1000) lance     (1000)        0 2021-02-17 18:51:19.000000 rattail_corepos-0.2.0/rattail_corepos/trainwreck/importing/__init__.py
+-rw-r--r--   0 lance     (1000) lance     (1000)     9165 2023-06-13 01:04:31.000000 rattail_corepos-0.2.0/rattail_corepos/trainwreck/importing/corepos.py
+drwxr-xr-x   0 lance     (1000) lance     (1000)        0 2024-05-29 15:12:37.829058 rattail_corepos-0.2.0/rattail_corepos.egg-info/
+-rw-r--r--   0 lance     (1000) lance     (1000)     1229 2024-05-29 15:12:37.000000 rattail_corepos-0.2.0/rattail_corepos.egg-info/PKG-INFO
+-rw-r--r--   0 lance     (1000) lance     (1000)     5438 2024-05-29 15:12:37.000000 rattail_corepos-0.2.0/rattail_corepos.egg-info/SOURCES.txt
+-rw-r--r--   0 lance     (1000) lance     (1000)        1 2024-05-29 15:12:37.000000 rattail_corepos-0.2.0/rattail_corepos.egg-info/dependency_links.txt
+-rw-r--r--   0 lance     (1000) lance     (1000)     1346 2024-05-29 15:12:37.000000 rattail_corepos-0.2.0/rattail_corepos.egg-info/entry_points.txt
+-rw-r--r--   0 lance     (1000) lance     (1000)        1 2024-05-29 15:12:37.000000 rattail_corepos-0.2.0/rattail_corepos.egg-info/not-zip-safe
+-rw-r--r--   0 lance     (1000) lance     (1000)       18 2024-05-29 15:12:37.000000 rattail_corepos-0.2.0/rattail_corepos.egg-info/requires.txt
+-rw-r--r--   0 lance     (1000) lance     (1000)       16 2024-05-29 15:12:37.000000 rattail_corepos-0.2.0/rattail_corepos.egg-info/top_level.txt
+-rw-r--r--   0 lance     (1000) lance     (1000)     2289 2024-05-29 15:12:37.829058 rattail_corepos-0.2.0/setup.cfg
+-rw-r--r--   0 lance     (1000) lance     (1000)      974 2023-05-16 18:14:04.000000 rattail_corepos-0.2.0/setup.py
```

### filetype from file(1)

```diff
@@ -1 +1 @@
-POSIX tar archive (GNU)
+POSIX tar archive
```

### Comparing `rattail_corepos-0.1.9/COPYING.txt` & `rattail_corepos-0.2.0/COPYING.txt`

 * *Files identical despite different names*

### Comparing `rattail_corepos-0.1.9/PKG-INFO` & `rattail_corepos-0.2.0/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,29 +1,30 @@
 Metadata-Version: 2.1
 Name: rattail_corepos
-Version: 0.1.9
+Version: 0.2.0
 Summary: Rattail Software Interfaces for CORE POS
 Home-page: https://rattailproject.org/
 Author: Lance Edgar
 Author-email: lance@edbob.org
 License: GNU GPL v3
-Platform: UNKNOWN
 Classifier: Development Status :: 3 - Alpha
 Classifier: Environment :: Console
 Classifier: Environment :: Web Environment
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: GNU General Public License v3 or later (GPLv3+)
 Classifier: Natural Language :: English
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.5
 Classifier: Topic :: Office/Business
 Classifier: Topic :: Software Development :: Libraries :: Python Modules
 License-File: COPYING.txt
+Requires-Dist: pyCOREPOS
+Requires-Dist: rattail
 
 
 rattail_corepos
 ===============
 
 Rattail is a retail software framework, released under the GNU General Public
 License.
@@ -31,9 +32,7 @@
 This package contains software interfaces for the `CORE POS`_ system.
 
 .. _`CORE POS`: https://github.com/CORE-POS/IS4C
 
 Please see Rattail's `home page`_ for more information.
 
 .. _`home page`: https://rattailproject.org/
-
-
```

### Comparing `rattail_corepos-0.1.9/rattail_corepos/__init__.py` & `rattail_corepos-0.2.0/rattail_corepos/__init__.py`

 * *Files identical despite different names*

### Comparing `rattail_corepos-0.1.9/rattail_corepos/batch/coremember.py` & `rattail_corepos-0.2.0/rattail_corepos/batch/coremember.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 # -*- coding: utf-8; -*-
 ################################################################################
 #
 #  Rattail -- Retail Software Framework
-#  Copyright © 2010-2021 Lance Edgar
+#  Copyright © 2010-2023 Lance Edgar
 #
 #  This file is part of Rattail.
 #
 #  Rattail is free software: you can redistribute it and/or modify it under the
 #  terms of the GNU General Public License as published by the Free Software
 #  Foundation, either version 3 of the License, or (at your option) any later
 #  version.
@@ -102,15 +102,17 @@
 
         maxlens = {}
         for field in fields:
             maxlens[field] = maxlen(getattr(CoreMemberBatchRow, field))
 
         def append(csvrow, i):
             row = self.make_row()
-            row.card_number = int(csvrow['external_id'])
+            row.card_number_raw = csvrow['external_id']
+            if csvrow['external_id'].isdigit():
+                row.card_number = int(csvrow['external_id'])
             row.first_name = csvrow['first_name']
             row.last_name = csvrow['last_name']
             row.street = csvrow['primary_address1']
             row.city = csvrow['primary_city']
             row.state = csvrow['primary_state']
             row.zipcode = csvrow['primary_zip']
             row.phone = csvrow['phone_number']
@@ -181,15 +183,15 @@
         row.status_text = None
 
         if not row.card_number:
             row.status_code = row.STATUS_MEMBER_NOT_FOUND
             row.status_text = "row has no card number"
             return
 
-        core_member = self.core_session.query(corepos.MemberInfo).get(row.card_number)
+        core_member = self.core_session.get(corepos.MemberInfo, row.card_number)
         if not core_member:
             row.status_code = row.STATUS_MEMBER_NOT_FOUND
             row.status_text = "matching record not found in CORE"
             return
 
         core_customer = core_member.customers[0] if core_member.customers else None
 
@@ -244,15 +246,15 @@
         directly via SQL, for the fields which are specified in the
         batch params.
         """
         core_session = CoreSession()
         fields = batch.get_param('fields')
 
         def update(row, i):
-            core_member = core_session.query(corepos.MemberInfo).get(row.card_number)
+            core_member = core_session.get(corepos.MemberInfo, row.card_number)
             if not core_member:
                 log.warning("CORE member not found for row %s with card number: %s",
                             row.uuid, row.card_number)
                 return
 
             if 'street' in fields:
                 core_member.street = row.street
```

### Comparing `rattail_corepos-0.1.9/rattail_corepos/batch/vendorcatalog.py` & `rattail_corepos-0.2.0/rattail_corepos/batch/vendorcatalog.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 # -*- coding: utf-8; -*-
 ################################################################################
 #
 #  Rattail -- Retail Software Framework
-#  Copyright © 2010-2021 Lance Edgar
+#  Copyright © 2010-2023 Lance Edgar
 #
 #  This file is part of Rattail.
 #
 #  Rattail is free software: you can redistribute it and/or modify it under the
 #  terms of the GNU General Public License as published by the Free Software
 #  Foundation, either version 3 of the License, or (at your option) any later
 #  version.
@@ -23,15 +23,14 @@
 """
 Handler for Vendor Catalog batches
 """
 
 import decimal
 
 from rattail.batch import vendorcatalog as base
-from rattail_corepos.corepos.api import make_corepos_api
 
 
 class VendorCatalogHandler(base.VendorCatalogHandler):
     """
     Handler for vendor catalog batches.
     """
     # default logic tries to update versions after execution, but since we just
@@ -69,15 +68,15 @@
                                        row.STATUS_CHANGE_COST)]
 
         if rows:
             vendor_id = batch.vendor.corepos_id
             if not vendor_id:
                 raise ValueError("Batch vendor does not have valid CORE-POS ID")
 
-            self.api = make_corepos_api(self.config)
+            self.api = self.app.get_corepos_handler.make_webapi()
             self.update_corepos(batch, rows, vendor_id, progress=progress,
                                 # update_product_costs=kwargs.get('update_product_costs', False),
             )
 
         return True
 
     def update_corepos(self, batch, rows, vendor_id, progress=None,
```

### Comparing `rattail_corepos-0.1.9/rattail_corepos/corepos/api.py` & `rattail_corepos-0.2.0/rattail_corepos/corepos/office/importing/db/__init__.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 # -*- coding: utf-8; -*-
 ################################################################################
 #
 #  Rattail -- Retail Software Framework
-#  Copyright © 2010-2021 Lance Edgar
+#  Copyright © 2010-2020 Lance Edgar
 #
 #  This file is part of Rattail.
 #
 #  Rattail is free software: you can redistribute it and/or modify it under the
 #  terms of the GNU General Public License as published by the Free Software
 #  Foundation, either version 3 of the License, or (at your option) any later
 #  version.
@@ -17,19 +17,11 @@
 #  details.
 #
 #  You should have received a copy of the GNU General Public License along with
 #  Rattail.  If not, see <http://www.gnu.org/licenses/>.
 #
 ################################################################################
 """
-CORE-POS API
+Importing data into CORE-POS (direct DB)
 """
 
-from corepos.api import CoreWebAPI
-
-
-def make_corepos_api(config):
-    """
-    Make and return a new CORE-POS API client object.
-    """
-    url = config.require('corepos.api', 'url')
-    return CoreWebAPI(url)
+from . import model
```

### Comparing `rattail_corepos-0.1.9/rattail_corepos/corepos/common/importing.py` & `rattail_corepos-0.2.0/rattail_corepos/corepos/common/importing.py`

 * *Files identical despite different names*

### Comparing `rattail_corepos-0.1.9/rattail_corepos/corepos/importing/__init__.py` & `rattail_corepos-0.2.0/rattail_corepos/corepos/office/importing/__init__.py`

 * *Files identical despite different names*

### Comparing `rattail_corepos-0.1.9/rattail_corepos/corepos/importing/db/__init__.py` & `rattail_corepos-0.2.0/rattail_corepos/corepos/office/importing/db/exporters/__init__.py`

 * *Files 6% similar despite different names*

```diff
@@ -17,11 +17,9 @@
 #  details.
 #
 #  You should have received a copy of the GNU General Public License along with
 #  Rattail.  If not, see <http://www.gnu.org/licenses/>.
 #
 ################################################################################
 """
-Importing data into CORE-POS (direct DB)
+Exporting data from CORE-POS (direct DB)
 """
-
-from . import model
```

### Comparing `rattail_corepos-0.1.9/rattail_corepos/corepos/importing/db/corepos.py` & `rattail_corepos-0.2.0/rattail_corepos/corepos/office/importing/db/corepos.py`

 * *Files 9% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 # -*- coding: utf-8; -*-
 ################################################################################
 #
 #  Rattail -- Retail Software Framework
-#  Copyright © 2010-2020 Lance Edgar
+#  Copyright © 2010-2023 Lance Edgar
 #
 #  This file is part of Rattail.
 #
 #  Rattail is free software: you can redistribute it and/or modify it under the
 #  terms of the GNU General Public License as published by the Free Software
 #  Foundation, either version 3 of the License, or (at your option) any later
 #  version.
@@ -20,40 +20,36 @@
 #  Rattail.  If not, see <http://www.gnu.org/licenses/>.
 #
 ################################################################################
 """
 CORE-POS -> CORE-POS data import
 """
 
+from collections import OrderedDict
+
 from corepos.db.office_op import Session as CoreSession
 
-from rattail.importing.handlers import FromSQLAlchemyHandler, ToSQLAlchemyHandler
+from rattail.importing.handlers import FromSQLAlchemyHandler
 from rattail.importing.sqlalchemy import FromSQLAlchemySameToSame
-from rattail.util import OrderedDict
-from rattail_corepos.corepos.importing import db as corepos_importing
+from rattail_corepos.corepos.office.importing import db as corepos_importing
 
 
 class FromCoreHandler(FromSQLAlchemyHandler):
     """
     Base class for import handlers which use a CORE database as the host / source.
     """
     host_title = "CORE"
+    host_key = 'corepos_db_office_op'
 
     def make_host_session(self):
         return CoreSession()
 
 
-class ToCoreHandler(ToSQLAlchemyHandler):
-    """
-    Base class for import handlers which target a CORE database on the local side.
-    """
-    local_title = "CORE"
-
-    def make_session(self):
-        return CoreSession()
+# TODO: deprecate / remove this
+ToCoreHandler = corepos_importing.model.ToCoreHandler
 
 
 class FromCoreToCoreBase(object):
     """
     Common base class for Core -> Core data import/export handlers.
     """
 
@@ -63,22 +59,22 @@
         importers['Subdepartment'] = SubdepartmentImporter
         importers['Vendor'] = VendorImporter
         importers['VendorContact'] = VendorContactImporter
         importers['Product'] = ProductImporter
         importers['ProductFlag'] = ProductFlagImporter
         importers['VendorItem'] = VendorItemImporter
         importers['Employee'] = EmployeeImporter
-        importers['CustData'] = CustDataImporter
+        importers['CustomerClassic'] = CustomerClassicImporter
         importers['MemberType'] = MemberTypeImporter
         importers['MemberInfo'] = MemberInfoImporter
         importers['HouseCoupon'] = HouseCouponImporter
         return importers
 
 
-class FromCoreToCoreImport(FromCoreToCoreBase, FromCoreHandler, ToCoreHandler):
+class FromCoreToCoreImport(FromCoreToCoreBase, FromCoreHandler, corepos_importing.model.ToCoreHandler):
     """
     Handler for CORE (other) -> CORE (local) data import.
 
     .. attribute:: direction
 
        Value is ``'import'`` - see also
        :attr:`rattail.importing.handlers.ImportHandler.direction`.
@@ -90,15 +86,15 @@
     def host_title(self):
         return "CORE ({})".format(self.dbkey)
 
     def make_host_session(self):
         return CoreSession(bind=self.config.corepos_engines[self.dbkey])
 
 
-class FromCoreToCoreExport(FromCoreToCoreBase, FromCoreHandler, ToCoreHandler):
+class FromCoreToCoreExport(FromCoreToCoreBase, FromCoreHandler, corepos_importing.model.ToCoreHandler):
     """
     Handler for CORE (local) -> CORE (other) data export.
 
     .. attribute:: direction
 
        Value is ``'export'`` - see also
        :attr:`rattail.importing.handlers.ImportHandler.direction`.
@@ -140,15 +136,15 @@
 
 class VendorItemImporter(FromCore, corepos_importing.model.VendorItemImporter):
     pass
 
 class EmployeeImporter(FromCore, corepos_importing.model.EmployeeImporter):
     pass
 
-class CustDataImporter(FromCore, corepos_importing.model.CustDataImporter):
+class CustomerClassicImporter(FromCore, corepos_importing.model.CustomerClassicImporter):
     pass
 
 class MemberTypeImporter(FromCore, corepos_importing.model.MemberTypeImporter):
     pass
 
 class MemberInfoImporter(FromCore, corepos_importing.model.MemberInfoImporter):
     pass
```

### Comparing `rattail_corepos-0.1.9/rattail_corepos/corepos/importing/db/csv.py` & `rattail_corepos-0.2.0/rattail_corepos/corepos/office/importing/db/exporters/csv.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 # -*- coding: utf-8; -*-
 ################################################################################
 #
 #  Rattail -- Retail Software Framework
-#  Copyright © 2010-2020 Lance Edgar
+#  Copyright © 2010-2023 Lance Edgar
 #
 #  This file is part of Rattail.
 #
 #  Rattail is free software: you can redistribute it and/or modify it under the
 #  terms of the GNU General Public License as published by the Free Software
 #  Foundation, either version 3 of the License, or (at your option) any later
 #  version.
@@ -17,34 +17,32 @@
 #  details.
 #
 #  You should have received a copy of the GNU General Public License along with
 #  Rattail.  If not, see <http://www.gnu.org/licenses/>.
 #
 ################################################################################
 """
-CSV -> CORE data import
+CORE-POS Data Export
 """
 
-from corepos.db.office_op import model as corepos, Session as CoreSession
+from corepos.db.office_op import model as corepos
 
-from rattail.importing.handlers import FromFileHandler
-from rattail.importing.csv import FromCSVToSQLAlchemyMixin
-from rattail_corepos.corepos.importing.db.model import ToCore
-from rattail_corepos.corepos.importing.db.corepos import ToCoreHandler
+from rattail.importing.handlers import ToCSVHandler
+from rattail.importing.exporters import FromSQLAlchemyToCSVMixin
+from rattail_corepos.corepos.office.importing.db.corepos import FromCoreHandler, FromCore
 
 
-class FromCSVToCore(FromCSVToSQLAlchemyMixin, FromFileHandler, ToCoreHandler):
+class FromCoreToCSV(FromSQLAlchemyToCSVMixin, FromCoreHandler, ToCSVHandler):
     """
-    Handler for CSV -> CORE data import
+    Handler for CORE -> CSV data export.
     """
-    host_title = "CSV"
-    ToParent = ToCore
+    direction = 'export'
+    local_title = "CSV"
+    FromParent = FromCore
+    ignored_model_names = ['Change'] # omit the datasync change model
 
     @property
-    def local_title(self):
-        return "CORE ({})".format(self.dbkey)
+    def host_title(self):
+        return self.config.node_title(default="CORE")
 
     def get_model(self):
         return corepos
-
-    def make_session(self):
-        return CoreSession(bind=self.config.corepos_engines[self.dbkey])
```

### Comparing `rattail_corepos-0.1.9/rattail_corepos/corepos/importing/db/exporters/__init__.py` & `rattail_corepos-0.2.0/setup.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 # -*- coding: utf-8; -*-
 ################################################################################
 #
 #  Rattail -- Retail Software Framework
-#  Copyright © 2010-2020 Lance Edgar
+#  Copyright © 2010-2023 Lance Edgar
 #
 #  This file is part of Rattail.
 #
 #  Rattail is free software: you can redistribute it and/or modify it under the
 #  terms of the GNU General Public License as published by the Free Software
 #  Foundation, either version 3 of the License, or (at your option) any later
 #  version.
@@ -16,10 +16,11 @@
 #  FOR A PARTICULAR PURPOSE.  See the GNU General Public License for more
 #  details.
 #
 #  You should have received a copy of the GNU General Public License along with
 #  Rattail.  If not, see <http://www.gnu.org/licenses/>.
 #
 ################################################################################
-"""
-Exporting data from CORE-POS (direct DB)
-"""
+
+from setuptools import setup
+
+setup()
```

### Comparing `rattail_corepos-0.1.9/rattail_corepos/corepos/importing/db/exporters/catapult_inventory.py` & `rattail_corepos-0.2.0/rattail_corepos/corepos/office/importing/db/exporters/catapult_inventory.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 # -*- coding: utf-8; -*-
 ################################################################################
 #
 #  Rattail -- Retail Software Framework
-#  Copyright © 2010-2020 Lance Edgar
+#  Copyright © 2010-2023 Lance Edgar
 #
 #  This file is part of Rattail.
 #
 #  Rattail is free software: you can redistribute it and/or modify it under the
 #  terms of the GNU General Public License as published by the Free Software
 #  Foundation, either version 3 of the License, or (at your option) any later
 #  version.
@@ -24,26 +24,26 @@
 CORE-POS -> Catapult Inventory Workbook
 """
 
 import re
 import datetime
 import decimal
 import logging
+from collections import OrderedDict
 
 from sqlalchemy.exc import ProgrammingError
 from sqlalchemy import orm
 from sqlalchemy.orm.exc import NoResultFound
 
 from corepos import enum as corepos_enum
 from corepos.db.office_op import model as corepos
 from corepos.db.util import table_exists
 
 from rattail.gpc import GPC
 from rattail.core import get_uuid
-from rattail.util import OrderedDict
 from rattail.importing.handlers import ToFileHandler
 from rattail_corepos.corepos.importing.db.corepos import FromCoreHandler, FromCore
 from rattail_onager.catapult.importing import inventory as catapult_importing
 
 
 log = logging.getLogger(__name__)
```

### Comparing `rattail_corepos-0.1.9/rattail_corepos/corepos/importing/db/exporters/catapult_membership.py` & `rattail_corepos-0.2.0/rattail_corepos/corepos/office/importing/db/exporters/catapult_membership.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 # -*- coding: utf-8; -*-
 ################################################################################
 #
 #  Rattail -- Retail Software Framework
-#  Copyright © 2010-2020 Lance Edgar
+#  Copyright © 2010-2023 Lance Edgar
 #
 #  This file is part of Rattail.
 #
 #  Rattail is free software: you can redistribute it and/or modify it under the
 #  terms of the GNU General Public License as published by the Free Software
 #  Foundation, either version 3 of the License, or (at your option) any later
 #  version.
@@ -22,20 +22,20 @@
 ################################################################################
 """
 CORE-POS -> Catapult Membership Workbook
 """
 
 import decimal
 import logging
+from collections import OrderedDict
 
 from sqlalchemy import orm
 
 from corepos.db.office_op import model as corepos
 
-from rattail.util import OrderedDict
 from rattail.importing.handlers import ToFileHandler
 from rattail.time import localtime
 from rattail.excel import ExcelReader
 from rattail_corepos.corepos.importing.db.corepos import FromCoreHandler, FromCore
 from rattail_onager.catapult.importing import membership as catapult_importing
 
 
@@ -56,15 +56,15 @@
         return importers
 
 
 class MemberImporter(FromCore, catapult_importing.model.MemberImporter):
     """
     Member data importer.
     """
-    host_model_class = corepos.CustData
+    host_model_class = corepos.CustomerClassic
     supported_fields = [
         'member_id',
         'first_name',
         'last_name',
         'address_1',
         'address_2',
         'city',
@@ -104,22 +104,22 @@
             if profile['Please indicate Default Profile'] == 'X':
                 self.default_membership_profile = profile
                 break
         if not self.default_membership_profile:
             raise RuntimeError("cannot determine default membership profile")
 
     def query(self):
-        return self.host_session.query(corepos.CustData)\
-                                .order_by(corepos.CustData.card_number,
-                                          corepos.CustData.person_number,
-                                          corepos.CustData.id)\
-                                .options(orm.joinedload(corepos.CustData.member_type))\
-                                .options(orm.joinedload(corepos.CustData.member_info)\
+        return self.host_session.query(corepos.CustomerClassic)\
+                                .order_by(corepos.CustomerClassic.card_number,
+                                          corepos.CustomerClassic.person_number,
+                                          corepos.CustomerClassic.id)\
+                                .options(orm.joinedload(corepos.CustomerClassic.member_type))\
+                                .options(orm.joinedload(corepos.CustomerClassic.member_info)\
                                          .joinedload(corepos.MemberInfo.dates))\
-                                .options(orm.joinedload(corepos.CustData.member_info)\
+                                .options(orm.joinedload(corepos.CustomerClassic.member_info)\
                                          .joinedload(corepos.MemberInfo.notes))
 
     def normalize_host_object(self, custdata):
 
         if custdata.person_number == 1:
             family_affiliation = False
         elif custdata.person_number > 1:
```

### Comparing `rattail_corepos-0.1.9/rattail_corepos/corepos/importing/db/exporters/csv.py` & `rattail_corepos-0.2.0/rattail_corepos/trainwreck/commands.py`

 * *Files 26% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 # -*- coding: utf-8; -*-
 ################################################################################
 #
 #  Rattail -- Retail Software Framework
-#  Copyright © 2010-2020 Lance Edgar
+#  Copyright © 2010-2024 Lance Edgar
 #
 #  This file is part of Rattail.
 #
 #  Rattail is free software: you can redistribute it and/or modify it under the
 #  terms of the GNU General Public License as published by the Free Software
 #  Foundation, either version 3 of the License, or (at your option) any later
 #  version.
@@ -17,32 +17,32 @@
 #  details.
 #
 #  You should have received a copy of the GNU General Public License along with
 #  Rattail.  If not, see <http://www.gnu.org/licenses/>.
 #
 ################################################################################
 """
-CORE-POS Data Export
+Trainwreck Commands
 """
 
-from corepos.db.office_op import model as corepos
+import typer
 
-from rattail.importing.handlers import ToCSVHandler
-from rattail.importing.exporters import FromSQLAlchemyToCSVMixin
-from rattail_corepos.corepos.importing.db.corepos import FromCoreHandler, FromCore
+from rattail.trainwreck.commands import trainwreck_typer
+from rattail.commands.typer import importer_command, typer_get_runas_user
+from rattail.commands.importing import ImportCommandHandler
 
 
-class FromCoreToCSV(FromSQLAlchemyToCSVMixin, FromCoreHandler, ToCSVHandler):
+@trainwreck_typer.command()
+@importer_command
+def import_corepos(
+        ctx: typer.Context,
+        **kwargs
+):
     """
-    Handler for CORE -> CSV data export.
+    Import data from CORE-POS "trans" DB
     """
-    direction = 'export'
-    local_title = "CSV"
-    FromParent = FromCore
-    ignored_model_names = ['Change'] # omit the datasync change model
-
-    @property
-    def host_title(self):
-        return self.config.node_title(default="CORE")
-
-    def get_model(self):
-        return corepos
+    config = ctx.parent.rattail_config
+    progress = ctx.parent.rattail_progress
+    handler = ImportCommandHandler(
+        config, import_handler_key='to_trainwreck.from_corepos_db_office_trans.import')
+    kwargs['user'] = typer_get_runas_user(ctx)
+    handler.run(kwargs, progress=progress)
```

### Comparing `rattail_corepos-0.1.9/rattail_corepos/corepos/importing/db/square.py` & `rattail_corepos-0.2.0/rattail_corepos/corepos/office/importing/db/square.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 # -*- coding: utf-8; -*-
 ################################################################################
 #
 #  Rattail -- Retail Software Framework
-#  Copyright © 2010-2020 Lance Edgar
+#  Copyright © 2010-2023 Lance Edgar
 #
 #  This file is part of Rattail.
 #
 #  Rattail is free software: you can redistribute it and/or modify it under the
 #  terms of the GNU General Public License as published by the Free Software
 #  Foundation, either version 3 of the License, or (at your option) any later
 #  version.
@@ -23,22 +23,22 @@
 """
 Square -> CORE-POS data importing
 """
 
 import re
 import datetime
 import decimal
+from collections import OrderedDict
 
 import sqlalchemy as sa
 
 from corepos.db.office_trans import Session as CoreTransSession, model as coretrans
 
 from rattail import importing
-from rattail.util import OrderedDict
-from rattail_corepos.corepos.importing import db as corepos_importing
+from rattail_corepos.corepos.office.importing import db as corepos_importing
 
 
 class FromSquareToCoreTrans(importing.ToSQLAlchemyHandler):
     """
     Square -> CORE-POS import handler.
     """
     host_title = "Square"
```

### Comparing `rattail_corepos-0.1.9/rattail_corepos/corepos/importing/model.py` & `rattail_corepos-0.2.0/rattail_corepos/corepos/office/importing/model.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 # -*- coding: utf-8; -*-
 ################################################################################
 #
 #  Rattail -- Retail Software Framework
-#  Copyright © 2010-2021 Lance Edgar
+#  Copyright © 2010-2023 Lance Edgar
 #
 #  This file is part of Rattail.
 #
 #  Rattail is free software: you can redistribute it and/or modify it under the
 #  terms of the GNU General Public License as published by the Free Software
 #  Foundation, either version 3 of the License, or (at your option) any later
 #  version.
@@ -23,15 +23,52 @@
 """
 CORE-POS model importers (webservices API)
 """
 
 from rattail import importing
 from rattail.util import data_diffs
 from rattail_corepos.corepos.util import get_core_members
-from rattail_corepos.corepos.api import make_corepos_api
+
+
+class ToCOREAPIHandler(importing.ImportHandler):
+    """
+    Base class for handlers targeting the CORE API.
+    """
+    local_key = 'corepos_api'
+    generic_local_title = "CORE Office (API)"
+
+    @property
+    def local_title(self):
+        return "CORE-POS (API)"
+
+    def process_changes(self, changes):
+
+        if 'Member' in changes:
+            member_changes = changes['Member']
+            member_importer = self.importers['Member']
+            created, updated, deleted = changes['Member']
+            if updated:
+
+                # explode the 'customers' field so email will show
+                # diffs for each subrecord field
+                for update in updated:
+                    local_object, local_data, host_data = update
+
+                    local_customers = local_data.pop('customers')
+                    for i, customer in enumerate(local_customers, 1):
+                        for key in customer:
+                            local_data[f'customers.{i}.{key}'] = customer[key]
+
+                    host_customers = host_data.pop('customers')
+                    for i, customer in enumerate(host_customers, 1):
+                        for key in customer:
+                            host_data[f'customers.{i}.{key}'] = customer[key]
+
+        # do normal logic for the rest
+        super().process_changes(changes)
 
 
 class ToCoreAPI(importing.Importer):
     """
     Base class for all CORE "operational" model importers, which use the API.
     """
     # TODO: these importers are in a bit of an experimental state at the
@@ -41,15 +78,15 @@
 
     caches_local_data = True
 
     def setup(self):
         self.establish_api()
 
     def establish_api(self):
-        self.api = make_corepos_api(self.config)
+        self.api = self.app.get_corepos_handler().make_webapi()
 
     def ensure_fields(self, data):
         """
         Ensure each of our supported fields are included in the data.  This is
         to handle cases where the API does not return all fields, e.g. when
         some of them are empty.
         """
@@ -117,18 +154,19 @@
         'email',
         # 'memberPricingAllowed',
         # 'memberCouponsAllowed',
         # 'lowIncomeBenefits',
         # 'modified',
     ]
 
-    empty_date_value = '0000-00-00 00:00:00'
+    #empty_date_value = '0000-00-00 00:00:00'
+    empty_date_value = '1900-01-01 00:00:00'
 
     def get_local_objects(self, host_data=None):
-        return get_core_members(self.api, progress=self.progress)
+        return get_core_members(self.config, self.api, progress=self.progress)
 
     def get_single_local_object(self, key):
         assert len(self.key) == 1
         assert self.key[0] == 'cardNo'
         return self.api.get_member(key[0])
 
     def normalize_local_object(self, member):
@@ -140,22 +178,22 @@
 
         # the 'customers' field requires a more granular approach, since the
         # data coming from API may have different fields than our local data
         if 'customers' in self.fields and 'customers' in diffs:
             if not self.customer_data_differs(local_data, host_data):
                 diffs.remove('customers')
 
-        # also the start/end dates should be looked at more closely.  if they
-        # contain the special '__omit__' value then we won't ever count as diff
-        if 'startDate' in self.fields and 'startDate' in diffs:
-            if host_data['startDate'] == '__omit__':
-                diffs.remove('startDate')
-        if 'endDate' in self.fields and 'endDate' in diffs:
-            if host_data['endDate'] == '__omit__':
-                diffs.remove('endDate')
+        # # also the start/end dates should be looked at more closely.  if they
+        # # contain the special '__omit__' value then we won't ever count as diff
+        # if 'startDate' in self.fields and 'startDate' in diffs:
+        #     if host_data['startDate'] == '__omit__':
+        #         diffs.remove('startDate')
+        # if 'endDate' in self.fields and 'endDate' in diffs:
+        #     if host_data['endDate'] == '__omit__':
+        #         diffs.remove('endDate')
 
         return diffs
 
     def customer_data_differs(self, local_data, host_data):
         local_customers = local_data['customers']
         host_customers = host_data['customers']
 
@@ -171,17 +209,24 @@
         for host_customer in host_customers:
 
             # we differ if can't locate corresponding "old" local record
             local_customer = self.find_local_customer(local_customers, host_customer)
             if not local_customer:
                 return True
 
-            # we differ if old and new records differ
-            if data_diffs(local_customer, host_customer,
-                          fields=self.supported_customer_fields):
+            # we differ if old and new records differ, but...
+            diffs = data_diffs(local_customer, host_customer,
+                               fields=self.supported_customer_fields)
+
+            # nb. the customerID field is sometimes int, sometimes str
+            # (?)  so we must coerce both sides to str for proper
+            # comparison, otherwise false diffs happen
+            if diffs and (
+                    diffs != ['customerID']
+                    or str(local_customer['customerID']) != str(host_customer['customerID'])):
                 return True
 
         # okay, now let's traverse the "old" list
         for local_customer in local_customers:
 
             # we differ if can't locate corresponding "new" host record
             host_customer = self.find_host_customer(host_customers, local_customer)
@@ -194,41 +239,41 @@
     def find_local_customer(self, local_customers, host_customer):
         assert 'customerID' in self.supported_customer_fields
 
         if not host_customer['customerID']:
             return              # new customer
 
         for local_customer in local_customers:
-            if local_customer['customerID'] == host_customer['customerID']:
+            if str(local_customer['customerID']) == str(host_customer['customerID']):
                 return local_customer
 
     def find_host_customer(self, host_customers, local_customer):
         assert 'customerID' in self.supported_customer_fields
 
         for host_customer in host_customers:
-            if host_customer['customerID'] == local_customer['customerID']:
+            if str(host_customer['customerID']) == str(local_customer['customerID']):
                 return host_customer
 
     def create_object(self, key, data):
         # we can get away with using the same logic for both here
         return self.update_object(None, data)
 
     def update_object(self, member, data, local_data=None):
         """
         Push an update for the member, via the CORE API.
         """
         if self.dry_run:
             return data
 
         cardNo = data.pop('cardNo')
-        data = dict(data)
-        if data.get('startDate') == '__omit__':
-            data.pop('startDate')
-        if data.get('endDate') == '__omit__':
-            data.pop('endDate')
+        # data = dict(data)
+        # if data.get('startDate') == '__omit__':
+        #     data.pop('startDate')
+        # if data.get('endDate') == '__omit__':
+        #     data.pop('endDate')
         member = self.api.set_member(cardNo, **data)
         return member
 
 
 class DepartmentImporter(ToCoreAPI):
     """
     Department model importer for CORE-POS
```

### Comparing `rattail_corepos-0.1.9/rattail_corepos/corepos/importing/rattail.py` & `rattail_corepos-0.2.0/rattail_corepos/corepos/office/importing/rattail.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 # -*- coding: utf-8; -*-
 ################################################################################
 #
 #  Rattail -- Retail Software Framework
-#  Copyright © 2010-2021 Lance Edgar
+#  Copyright © 2010-2023 Lance Edgar
 #
 #  This file is part of Rattail.
 #
 #  Rattail is free software: you can redistribute it and/or modify it under the
 #  terms of the GNU General Public License as published by the Free Software
 #  Foundation, either version 3 of the License, or (at your option) any later
 #  version.
@@ -21,35 +21,34 @@
 #
 ################################################################################
 """
 Rattail -> CORE-POS data export
 """
 
 import logging
+from collections import OrderedDict
 
 from sqlalchemy import orm
 
 from rattail import importing
 from rattail.db import model
-from rattail.db.util import short_session
-from rattail.util import OrderedDict, pretty_quantity
-from rattail_corepos.corepos import importing as corepos_importing
+from rattail.util import pretty_quantity
+from rattail_corepos.corepos.office import importing as corepos_importing
 from rattail_corepos.corepos.util import get_max_existing_vendor_id
 
 
 log = logging.getLogger(__name__)
 
 
-class FromRattailToCore(importing.FromRattailHandler):
+class FromRattailToCore(importing.FromRattailHandler, corepos_importing.model.ToCOREAPIHandler):
     """
     Rattail -> CORE-POS export handler
     """
-    host_title = "Rattail"
-    local_title = "CORE-POS"
     direction = 'export'
+    safe_for_web_app = True
 
     def get_importers(self):
         importers = OrderedDict()
         importers['Member'] = MemberImporter
         importers['Department'] = DepartmentImporter
         importers['Subdepartment'] = SubdepartmentImporter
         importers['Vendor'] = VendorImporter
@@ -88,69 +87,79 @@
         'accountHolder',
         'phone',
         'altPhone',
         'email',
     ]
 
     def query(self):
-        query = super(MemberImporter, self).query()
-        query = query.options(orm.joinedload(model.Customer.addresses))\
-                .options(orm.joinedload(model.Customer._people)\
-                         .joinedload(model.CustomerPerson.person)\
-                         .joinedload(model.Person.phones))\
-                .options(orm.joinedload(model.Customer._people)\
-                         .joinedload(model.CustomerPerson.person)\
-                         .joinedload(model.Person.emails))
+        query = super().query()
+        model = self.model
+
+        query = query.options(orm.joinedload(model.Customer.members))\
+                     .options(orm.joinedload(model.Customer._corepos))\
+                     .options(orm.joinedload(model.Customer.addresses))\
+                     .options(orm.joinedload(model.Customer.shoppers)\
+                              .joinedload(model.CustomerShopper._corepos))\
+                     .options(orm.joinedload(model.Customer.shoppers)\
+                              .joinedload(model.CustomerShopper.person)\
+                              .joinedload(model.Person.phones))\
+                     .options(orm.joinedload(model.Customer.shoppers)\
+                              .joinedload(model.CustomerShopper.person)\
+                              .joinedload(model.Person.emails))
+
         return query
 
     def normalize_host_object(self, customer):
 
         address = customer.addresses[0] if customer.addresses else None
 
-        people = []
-        for i, person in enumerate(customer.people, 1):
+        shoppers = []
+        for shopper in customer.shoppers:
+            person = shopper.person
             phones = person.phones
             phone1 = phones[0] if phones else None
             phone2 = phones[1] if len(phones) > 1 else None
             email = person.emails[0] if person.emails else None
-            people.append({
-                'customerID': str(person.corepos_customer_id),
+            shoppers.append({
+                'customerID': str(shopper.corepos_customer_id),
                 'firstName': person.first_name,
                 'lastName': person.last_name,
-                'accountHolder': i == 1,
+                'accountHolder': 1 if shopper.shopper_number == 1 else 0,
                 'phone': phone1.number if phone1 else '',
                 'altPhone': phone2.number if phone2 else '',
                 'email': email.address if email else '',
             })
 
-        member = customer.only_member(require=False)
+        member = self.app.get_member(customer)
         if member:
             if member.joined:
                 start_date = member.joined.strftime('%Y-%m-%d 00:00:00')
             else:
                 start_date = self.empty_date_value
             if member.withdrew:
                 end_date = member.withdrew.strftime('%Y-%m-%d 00:00:00')
             else:
                 end_date = self.empty_date_value
         else:
-            start_date = '__omit__'
-            end_date = '__omit__'
+            # start_date = '__omit__'
+            # end_date = '__omit__'
+            start_date = self.empty_date_value
+            end_date = self.empty_date_value
 
         return {
             'cardNo': customer.number,
-            'customerAccountID': customer.id,
-            'addressFirstLine': address.street if address else '',
-            'addressSecondLine': address.street2 if address else '',
-            'city': address.city if address else '',
-            'state': address.state if address else '',
-            'zip': address.zipcode if address else '',
+            'customerAccountID': str(customer.corepos_account_id or ''),
+            'addressFirstLine': (address.street or '') if address else '',
+            'addressSecondLine': (address.street2 or '') if address else '',
+            'city': (address.city or '') if address else '',
+            'state': (address.state or '') if address else '',
+            'zip': (address.zipcode or '') if address else '',
             'startDate': start_date,
             'endDate': end_date,
-            'customers': people,
+            'customers': shoppers,
         }
 
 
 class DepartmentImporter(FromRattail, corepos_importing.model.DepartmentImporter):
     """
     Department data exporter
     """
@@ -205,23 +214,23 @@
         'email',
     ]
 
     def setup(self):
         super(VendorImporter, self).setup()
 
         # self.max_existing_vendor_id = self.get_max_existing_vendor_id()
-        self.max_existing_vendor_id = get_max_existing_vendor_id()
+        self.max_existing_vendor_id = get_max_existing_vendor_id(self.config)
         self.last_vendor_id = self.max_existing_vendor_id
 
     def get_next_vendor_id(self):
         if hasattr(self, 'last_vendor_id'):
             self.last_vendor_id += 1
             return self.last_vendor_id
 
-        last_vendor_id = get_max_existing_vendor_id()
+        last_vendor_id = get_max_existing_vendor_id(self.config)
         return last_vendor_id + 1
 
     def normalize_host_object(self, vendor):
         vendor_id = vendor.corepos_id
         if not vendor_id:
             vendor_id = self.get_next_vendor_id()
```

### Comparing `rattail_corepos-0.1.9/rattail_corepos/corepos/lane/importing/op/__init__.py` & `rattail_corepos-0.2.0/rattail_corepos/corepos/lane/importing/op/__init__.py`

 * *Files identical despite different names*

### Comparing `rattail_corepos-0.1.9/rattail_corepos/corepos/lane/importing/op/model.py` & `rattail_corepos-0.2.0/rattail_corepos/corepos/lane/importing/op/model.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 # -*- coding: utf-8; -*-
 ################################################################################
 #
 #  Rattail -- Retail Software Framework
-#  Copyright © 2010-2021 Lance Edgar
+#  Copyright © 2010-2023 Lance Edgar
 #
 #  This file is part of Rattail.
 #
 #  Rattail is free software: you can redistribute it and/or modify it under the
 #  terms of the GNU General Public License as published by the Free Software
 #  Foundation, either version 3 of the License, or (at your option) any later
 #  version.
@@ -43,10 +43,10 @@
 
 
 class ProductImporter(ToCore):
     model_class = corepos.Product
     key = 'id'
 
 
-class CustDataImporter(ToCore):
-    model_class = corepos.CustData
+class CustomerClassicImporter(ToCore):
+    model_class = corepos.CustomerClassic
     key = 'id'
```

### Comparing `rattail_corepos-0.1.9/rattail_corepos/corepos/lane/importing/op/office.py` & `rattail_corepos-0.2.0/rattail_corepos/corepos/lane/importing/op/office.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 # -*- coding: utf-8; -*-
 ################################################################################
 #
 #  Rattail -- Retail Software Framework
-#  Copyright © 2010-2021 Lance Edgar
+#  Copyright © 2010-2023 Lance Edgar
 #
 #  This file is part of Rattail.
 #
 #  Rattail is free software: you can redistribute it and/or modify it under the
 #  terms of the GNU General Public License as published by the Free Software
 #  Foundation, either version 3 of the License, or (at your option) any later
 #  version.
@@ -20,40 +20,45 @@
 #  Rattail.  If not, see <http://www.gnu.org/licenses/>.
 #
 ################################################################################
 """
 CORE Office -> CORE Lane import
 """
 
+from collections import OrderedDict
+
 from corepos.db.office_op import Session as CoreOfficeSession, model as coreoffice
 from corepos.db.lane_op import Session as CoreLaneSession
 
 from rattail import importing
 from rattail.importing.handlers import FromSQLAlchemyHandler, ToSQLAlchemyHandler
-from rattail.util import OrderedDict
 from rattail_corepos.corepos.lane.importing import op as corepos_importing
 
 
 # TODO: this surely belongs in some other/common place? (is not lane-specific)
 class FromCoreOfficeHandler(FromSQLAlchemyHandler):
     """
     Base class for import handlers which use CORE Office as the host.
     """
+    host_key = 'corepos_db_office_op'
+    generic_host_title = 'CORE Office (DB "op")'
     host_title = "CORE Office"
 
     def make_host_session(self):
         return CoreOfficeSession()
 
 
 # TODO: this surely belongs in some other/common place? (is not office-specific)
 class ToCoreLaneHandler(ToSQLAlchemyHandler):
     """
     Base class for import handlers which target CORE Lane on the local side.
     """
     local_title = "CORE Lane"
+    local_key = 'corepos_db_lane_op'
+    generic_local_title = 'CORE Lane (DB "op")'
 
     def make_session(self):
         return CoreLaneSession()
 
 
 class FromCoreOfficeToCoreLane(FromCoreOfficeHandler, ToCoreLaneHandler):
     """
@@ -69,15 +74,15 @@
     def make_session(self):
         return CoreLaneSession(bind=self.config.core_lane_op_engines[self.dbkey])
 
     def get_importers(self):
         importers = OrderedDict()
         importers['Department'] = DepartmentImporter
         importers['Product'] = ProductImporter
-        importers['CustData'] = CustDataImporter
+        importers['CustomerClassic'] = CustomerClassicImporter
         return importers
 
 
 class FromCore(importing.FromSQLAlchemy):
     """
     Base class for CORE Office -> CORE Lane data importers.
     """
@@ -182,16 +187,16 @@
 
     def normalize_host_object(self, product):
         data = dict([(field, getattr(product, field))
                      for field in self.common_fields])
         return data
 
 
-class CustDataImporter(FromCore, corepos_importing.model.CustDataImporter):
-    host_model_class = coreoffice.CustData
+class CustomerClassicImporter(FromCore, corepos_importing.model.CustomerClassicImporter):
+    host_model_class = coreoffice.CustomerClassic
 
     # these fields are held in common, between Office and Lane tables
     common_fields = [
         'id',
         'card_number',
         'person_number',
         'first_name',
```

### Comparing `rattail_corepos-0.1.9/rattail_corepos/corepos/office/commands.py` & `rattail_corepos-0.2.0/rattail_corepos/corepos/commands.py`

 * *Files 23% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 # -*- coding: utf-8; -*-
 ################################################################################
 #
 #  Rattail -- Retail Software Framework
-#  Copyright © 2010-2021 Lance Edgar
+#  Copyright © 2010-2024 Lance Edgar
 #
 #  This file is part of Rattail.
 #
 #  Rattail is free software: you can redistribute it and/or modify it under the
 #  terms of the GNU General Public License as published by the Free Software
 #  Foundation, either version 3 of the License, or (at your option) any later
 #  version.
@@ -17,71 +17,69 @@
 #  details.
 #
 #  You should have received a copy of the GNU General Public License along with
 #  Rattail.  If not, see <http://www.gnu.org/licenses/>.
 #
 ################################################################################
 """
-CORE Office commands
+CORE-POS commands
 """
 
-import sys
+import typer
+from typing_extensions import Annotated
 
-from rattail import commands
-from rattail_corepos import __version__
-from rattail.util import load_object
+from rattail.commands.typer import make_typer, importer_command, typer_get_runas_user
+from rattail.commands.importing import ImportCommandHandler
 
 
-def main(*args):
-    """
-    Entry point for 'core-office' commands
-    """
-    if args:
-        args = list(args)
-    else:
-        args = sys.argv[1:]
-
-    cmd = Command()
-    cmd.run(*args)
-
-
-class Command(commands.Command):
-    """
-    Primary command for CORE Office
-    """
-    name = 'core-office'
-    version = __version__
-    description = "core-office -- command line interface for CORE Office"
-    long_description = ""
-
 
-class ExportLaneOp(commands.ImportSubcommand):
-    """
-    Export "op" data from CORE Office to CORE Lane
-    """
-    name = 'export-lane-op'
-    description = __doc__.strip()
-    default_handler_spec = 'rattail_corepos.corepos.lane.importing.op.office:FromCoreOfficeToCoreLane'
-    default_dbkey = 'default'
-
-    def get_handler_factory(self, **kwargs):
-        if self.config:
-            spec = self.config.get('corepos.lane.importing', 'office.handler',
-                                   default=self.default_handler_spec)
-        else:
-            # just use default, for sake of cmd line help
-            spec = self.default_handler_spec
-        return load_object(spec)
-
-    def add_parser_args(self, parser):
-        super(ExportLaneOp, self).add_parser_args(parser)
-        parser.add_argument('--dbkey', metavar='KEY', default=self.default_dbkey,
-                            help="Config key for database engine to be used as the "
-                            "\"target\" CORE Lane DB, i.e. where data will be "
-                            " exported.  This key must be defined in the "
-                            " [rattail_corepos.db.lane_op] section of your "
-                            "config file.")
-
-    def get_handler_kwargs(self, **kwargs):
-        if 'args' in kwargs:
-            kwargs['dbkey'] = kwargs['args'].dbkey
-        return kwargs
+crepes_typer = make_typer(
+    name='crepes',
+    help="Crepes -- command line interface for CORE-POS"
+)
+
+
+@crepes_typer.command()
+@importer_command
+def export_core(
+        ctx: typer.Context,
+        dbkey: Annotated[
+            str,
+            typer.Option(help="Config key for database engine to be used as the \"target\" "
+                         "CORE DB, i.e. where data will be exported.  This key must be "
+                         "defined in the [rattail_corepos.db] section of your config file.")] = 'host',
+        **kwargs
+):
+    """
+    Export data to another CORE database
+    """
+    config = ctx.parent.rattail_config
+    progress = ctx.parent.rattail_progress
+    handler = ImportCommandHandler(
+        config, import_handler_key='to_corepos_db_office_op.from_corepos_db_office_op.export')
+    kwargs['user'] = typer_get_runas_user(ctx)
+    kwargs['handler_kwargs'] = {'dbkey': dbkey}
+    handler.run(kwargs, progress=progress)
+
+
+@crepes_typer.command()
+@importer_command
+def import_core(
+        ctx: typer.Context,
+        dbkey: Annotated[
+            str,
+            typer.Option(help="Config key for database engine to be used as the CORE "
+                         "\"host\", i.e. the source of the data to be imported.  This key "
+                         "must be defined in the [rattail_corepos.db] section of your "
+                         "config file.")] = 'host',
+        **kwargs
+):
+    """
+    Import data from another CORE database
+    """
+    config = ctx.parent.rattail_config
+    progress = ctx.parent.rattail_progress
+    handler = ImportCommandHandler(
+        config, import_handler_key='to_corepos_db_office_op.from_corepos_db_office_op.import')
+    kwargs['user'] = typer_get_runas_user(ctx)
+    kwargs['handler_kwargs'] = {'dbkey': dbkey}
+    handler.run(kwargs, progress=progress)
```

### Comparing `rattail_corepos-0.1.9/rattail_corepos/corepos/util.py` & `rattail_corepos-0.2.0/rattail_corepos/corepos/util.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 # -*- coding: utf-8; -*-
 ################################################################################
 #
 #  Rattail -- Retail Software Framework
-#  Copyright © 2010-2020 Lance Edgar
+#  Copyright © 2010-2023 Lance Edgar
 #
 #  This file is part of Rattail.
 #
 #  Rattail is free software: you can redistribute it and/or modify it under the
 #  terms of the GNU General Public License as published by the Free Software
 #  Foundation, either version 3 of the License, or (at your option) any later
 #  version.
@@ -21,58 +21,61 @@
 #
 ################################################################################
 """
 CORE-POS misc. utilities
 """
 
 import logging
+from collections import OrderedDict
 
 import sqlalchemy as sa
 
 from corepos.db.office_op import Session as CoreSession, model as corepos
 
-from rattail.db.util import short_session
-from rattail.util import OrderedDict, progress_loop
-
 
 log = logging.getLogger(__name__)
 
 
-def get_core_members(api, progress=None):
+def get_core_members(config, api, progress=None):
     """
     Shared logic for fetching *all* customer accounts from CORE-POS API.
     """
+    app = config.get_app()
+
     # TODO: ideally could do this, but API doesn't let us fetch "all"
     # return api.get_members()
 
     # first we fetch all customer records from CORE DB
-    with short_session(Session=CoreSession) as s:
-        db_customers = s.query(corepos.Customer).all()
+    with app.short_session(factory=CoreSession) as s:
+        db_customers = s.query(corepos.CustomerClassic)\
+                        .order_by(corepos.CustomerClassic.card_number)\
+                        .all()
         s.expunge_all()
 
     # now we must fetch each customer account individually from API
     members = OrderedDict()
 
     def fetch(dbcust, i):
         if dbcust.card_number in members:
             return          # already fetched this one
         member = api.get_member(dbcust.card_number)
         if member:
             members[dbcust.card_number] = member
         else:
-            logger = log.warning if dbcust.account_holder else log.debug
+            logger = log.warning if dbcust.person_number == 1 else log.debug
             logger("could not fetch member from CORE API: %s",
                    dbcust.card_number)
 
-    progress_loop(fetch, db_customers, progress,
-                  message="Fetching Member data from CORE API")
+    app.progress_loop(fetch, db_customers, progress,
+                      message="Fetching Member data from CORE API")
     return list(members.values())
 
 
-def get_max_existing_vendor_id(session=None):
+def get_max_existing_vendor_id(config, session=None):
     """
     Returns the "last" (max) existing value for the ``vendors.vendorID``
     column, for use when creating new records, since it is not auto-increment.
     """
-    with short_session(Session=CoreSession, session=session) as s:
+    app = config.get_app()
+    with app.short_session(factory=CoreSession, session=session) as s:
         return s.query(sa.func.max(corepos.Vendor.id))\
                 .scalar() or 0
```

### Comparing `rattail_corepos-0.1.9/rattail_corepos/datasync/corepos.py` & `rattail_corepos-0.2.0/rattail_corepos/datasync/corepos.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 # -*- coding: utf-8; -*-
 ################################################################################
 #
 #  Rattail -- Retail Software Framework
-#  Copyright © 2010-2020 Lance Edgar
+#  Copyright © 2010-2023 Lance Edgar
 #
 #  This file is part of Rattail.
 #
 #  Rattail is free software: you can redistribute it and/or modify it under the
 #  terms of the GNU General Public License as published by the Free Software
 #  Foundation, either version 3 of the License, or (at your option) any later
 #  version.
@@ -25,15 +25,15 @@
 """
 
 import sqlalchemy as sa
 
 from corepos.db.office_op import Session as CoreSession, model as corepos
 
 from rattail.db import model
-from rattail.datasync import DataSyncWatcher, NewDataSyncImportConsumer
+from rattail.datasync import DataSyncWatcher, DataSyncImportConsumer
 
 
 class CoreOfficeOpWatcher(DataSyncWatcher):
     """
     DataSync watcher for the CORE ``office_op`` database.
     """
     prunes_changes = True
@@ -50,15 +50,15 @@
             sa.Column('id', sa.Integer(), nullable=False, primary_key=True),
             sa.Column('object_type', sa.String(length=255), nullable=False),
             sa.Column('object_key', sa.String(length=255), nullable=False),
             sa.Column('deleted', sa.Boolean(), nullable=False, default=False))
 
     def get_changes(self, lastrun):
         session = CoreSession()
-        result = session.execute(sa.sql.select([self.corepos_changes]))
+        result = session.execute(self.corepos_changes.select())
         changes = result.fetchall()
         session.close()
         if changes:
             return [
                 (c.id,
                  model.DataSyncChange(
                      payload_type=c.object_type,
@@ -145,15 +145,15 @@
                 for product in products
                 if product.upc])
 
         session.close()
         return changes
 
 
-class FromRattailToCore(NewDataSyncImportConsumer):
+class FromRattailToCore(DataSyncImportConsumer):
     """
     Rattail -> CORE POS datasync consumer
     """
     handler_spec = 'rattail_corepos.corepos.importing.rattail:FromRattailToCore'
 
     def process_changes(self, session, changes):
         """
@@ -165,17 +165,18 @@
 
         # update all importers with current session
         for importer in self.importers.values():
             importer.host_session = session
             # also establish the API client for each!
             importer.establish_api()
 
-        # sync all Customer changes
+        # sync all Member changes
         types = [
             'Customer',
+            'CustomerShopper',
             'Person',
             'CustomerPerson',
             'CustomerMailingAddress',
             'PersonPhoneNumber',
             'PersonEmailAddress',
             'Member',
         ]
@@ -231,73 +232,78 @@
             'Department',
             'Subdepartment',
         ]
         for change in [c for c in changes if c.payload_type in types]:
             self.invoke_importer(session, change)
 
     def get_host_object(self, session, change):
-        return session.query(getattr(model, change.payload_type))\
-                      .get(change.payload_key)
+        return session.get(getattr(model, change.payload_type), change.payload_key)
 
     def get_customers(self, session, change):
+        clientele = self.app.get_clientele_handler()
 
         if change.payload_type == 'Customer':
-            customer = session.query(model.Customer).get(change.payload_key)
+            customer = session.get(model.Customer, change.payload_key)
             if customer:
                 return [customer]
 
-        if change.payload_type == 'CustomerPerson':
-            cp = session.query(model.CustomerPerson).get(change.payload_key)
+        elif change.payload_type == 'CustomerShopper':
+            shopper = session.get(model.CustomerShopper, change.payload_key)
+            if shopper:
+                return [shopper.customer]
+
+        elif change.payload_type == 'CustomerPerson':
+            cp = session.get(model.CustomerPerson, change.payload_key)
             if cp:
                 return [cp.customer]
 
-        if change.payload_type == 'Person':
-            person = session.query(model.Person).get(change.payload_key)
+        elif change.payload_type == 'Person':
+            person = session.get(model.Person, change.payload_key)
             if person:
-                return person.customers
+                return clientele.get_customers_for_account_holder(person)
 
-        if change.payload_type == 'CustomerMailingAddress':
-            address = session.query(model.CustomerMailingAddress).get(change.payload_key)
+        elif change.payload_type == 'CustomerMailingAddress':
+            address = session.get(model.CustomerMailingAddress, change.payload_key)
             if address:
                 return [address.customer]
 
-        if change.payload_type == 'PersonPhoneNumber':
-            phone = session.query(model.PersonPhoneNumber).get(change.payload_key)
+        elif change.payload_type == 'PersonPhoneNumber':
+            phone = session.get(model.PersonPhoneNumber, change.payload_key)
             if phone:
-                return phone.person.customers
+                return clientele.get_customers_for_account_holder(phone.person)
 
-        if change.payload_type == 'PersonEmailAddress':
-            email = session.query(model.PersonEmailAddress).get(change.payload_key)
+        elif change.payload_type == 'PersonEmailAddress':
+            email = session.get(model.PersonEmailAddress, change.payload_key)
             if email:
-                return email.person.customers
+                return clientele.get_customers_for_account_holder(email.person)
 
-        if change.payload_type == 'Member':
-            member = session.query(model.Member).get(change.payload_key)
+        elif change.payload_type == 'Member':
+            member = session.get(model.Member, change.payload_key)
             if member:
                 return [member.customer]
 
         return []
 
     def get_vendor(self, session, change):
 
         if change.payload_type == 'Vendor':
-            return session.query(model.Vendor).get(change.payload_key)
+            return session.get(model.Vendor, change.payload_key)
 
         if change.payload_type == 'VendorPhoneNumber':
-            phone = session.query(model.VendorPhoneNumber).get(change.payload_key)
+            phone = session.get(model.VendorPhoneNumber, change.payload_key)
             if phone:
                 return phone.vendor
 
         if change.payload_type == 'VendorEmailAddress':
-            email = session.query(model.VendorEmailAddress).get(change.payload_key)
+            email = session.get(model.VendorEmailAddress, change.payload_key)
             if email:
                 return email.vendor
 
     def get_product(self, session, change):
 
         if change.payload_type == 'Product':
-            return session.query(model.Product).get(change.payload_key)
+            return session.get(model.Product, change.payload_key)
 
         if change.payload_type == 'ProductPrice':
-            price = session.query(model.ProductPrice).get(change.payload_key)
+            price = session.get(model.ProductPrice, change.payload_key)
             if price:
                 return price.product
```

### Comparing `rattail_corepos-0.1.9/rattail_corepos/datasync/rattail.py` & `rattail_corepos-0.2.0/rattail_corepos/datasync/rattail.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 # -*- coding: utf-8; -*-
 ################################################################################
 #
 #  Rattail -- Retail Software Framework
-#  Copyright © 2010-2021 Lance Edgar
+#  Copyright © 2010-2023 Lance Edgar
 #
 #  This file is part of Rattail.
 #
 #  Rattail is free software: you can redistribute it and/or modify it under the
 #  terms of the GNU General Public License as published by the Free Software
 #  Foundation, either version 3 of the License, or (at your option) any later
 #  version.
@@ -20,65 +20,67 @@
 #  Rattail.  If not, see <http://www.gnu.org/licenses/>.
 #
 ################################################################################
 """
 DataSync for Rattail DB
 """
 
-from sqlalchemy.orm.exc import NoResultFound
+from sqlalchemy import orm
 
 from corepos.db.office_op import Session as CoreSession, model as corepos
 
-from rattail.datasync import NewDataSyncImportConsumer
-from rattail_corepos.corepos.api import make_corepos_api
+from rattail.datasync import DataSyncImportConsumer
 
 
-class FromCOREAPIToRattail(NewDataSyncImportConsumer):
+class FromCOREAPIToRattail(DataSyncImportConsumer):
     """
     Consumer for CORE POS (API) -> Rattail datasync
     """
     handler_spec = 'rattail_corepos.importing.corepos.api:FromCOREPOSToRattail'
     model_map = {
         'VendorItem': 'ProductCost',
     }
 
     def setup(self):
-        super(FromCOREAPIToRattail, self).setup()
+        super().setup()
         self.establish_api()
 
     def establish_api(self):
-        self.api = make_corepos_api(self.config)
+        self.api = self.app.get_corepos_handler().make_webapi()
 
-    def process_changes(self, session, changes):
+    def pre_process_changes(self, session, changes):
+
+        # declare user responsible
         if self.runas_username:
             session.set_continuum_user(self.runas_username)
 
         # update all importers with current Rattail session
         for importer in self.importers.values():
             importer.session = session
-            # also establish the API client for each!
-            importer.establish_api()
+            importer.datasync_setup()
+
+    def process_changes_proper(self, session, changes):
 
         # sync all Customer-related changes
         types = [
             'Member',
         ]
         for change in [c for c in changes if c.payload_type in types]:
             if change.deletion:
                 # normal logic works fine for this (maybe?)
                 self.invoke_importer(session, change)
             else:
                 # import member data from API, into various Rattail tables
                 member = self.get_host_object(session, change)
                 self.process_change(session, self.importers['Customer'],
                                     host_object=member)
-                people = self.importers['Person'].get_person_objects_for_member(member)
-                for person in people:
-                    self.process_change(session, self.importers['Person'],
-                                        host_object=person)
+                shoppers = self.importers['CustomerShopper'].get_shoppers_for_member(member)
+                for shopper in shoppers:
+                    self.process_change(session, self.importers['CustomerShopper'],
+                                        host_object=shopper)
                 self.process_change(session, self.importers['Member'],
                                     host_object=member)
 
         # sync all "product meta" changes
         types = [
             'Department',
             'Subdepartment',
@@ -141,15 +143,15 @@
             if len(fields) == 2:
                 sku, vendorID = fields
                 vendor_item = self.api.get_vendor_item(sku, vendorID)
                 if vendor_item:
                     return self.api.get_product(vendor_item['upc'])
 
 
-class FromCOREPOSToRattailBase(NewDataSyncImportConsumer):
+class FromCOREPOSToRattailBase(DataSyncImportConsumer):
     """
     Base class for CORE POS -> Rattail data sync consumers.
     """
     handler_spec = 'rattail_corepos.importing.corepos.db:FromCOREPOSToRattail'
 
     def begin_transaction(self):
         self.corepos_session = CoreSession()
@@ -172,15 +174,14 @@
     def get_host_object(self, session, change):
 
         if change.payload_type == 'Product':
             try:
                 return self.corepos_session.query(corepos.Product)\
                                            .filter(corepos.Product.upc == change.payload_key)\
                                            .one()
-            except NoResultFound:
+            except orm.exc.NoResultFound:
                 pass
 
         else:
             # try to fetch CORE POS object via typical method
             Model = getattr(corepos, change.payload_type)
-            return self.corepos_session.query(Model)\
-                                       .get(int(change.payload_key))
+            return self.corepos_session.get(Model, int(change.payload_key))
```

### Comparing `rattail_corepos-0.1.9/rattail_corepos/db/__init__.py` & `rattail_corepos-0.2.0/rattail_corepos/importing/__init__.py`

 * *Files 25% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 # -*- coding: utf-8; -*-
 ################################################################################
 #
 #  Rattail -- Retail Software Framework
-#  Copyright © 2010-2018 Lance Edgar
+#  Copyright © 2010-2020 Lance Edgar
 #
 #  This file is part of Rattail.
 #
 #  Rattail is free software: you can redistribute it and/or modify it under the
 #  terms of the GNU General Public License as published by the Free Software
 #  Foundation, either version 3 of the License, or (at your option) any later
 #  version.
@@ -17,13 +17,11 @@
 #  details.
 #
 #  You should have received a copy of the GNU General Public License along with
 #  Rattail.  If not, see <http://www.gnu.org/licenses/>.
 #
 ################################################################################
 """
-CORE POS Database Stuff
+Importing data into Rattail
 """
 
-from __future__ import unicode_literals, absolute_import
-
-from corepos.db import Session
+from . import model
```

### Comparing `rattail_corepos-0.1.9/rattail_corepos/db/alembic/versions/130e4632a28a_add_corepos_product_cost.py` & `rattail_corepos-0.2.0/rattail_corepos/db/alembic/versions/130e4632a28a_add_corepos_product_cost.py`

 * *Files identical despite different names*

### Comparing `rattail_corepos-0.1.9/rattail_corepos/db/alembic/versions/50961b4b854a_add_corepos_member_batch.py` & `rattail_corepos-0.2.0/rattail_corepos/db/alembic/versions/50961b4b854a_add_corepos_member_batch.py`

 * *Files identical despite different names*

### Comparing `rattail_corepos-0.1.9/rattail_corepos/db/alembic/versions/7fea5aebddfb_add_store_extension.py` & `rattail_corepos-0.2.0/rattail_corepos/db/alembic/versions/7fea5aebddfb_add_store_extension.py`

 * *Files identical despite different names*

### Comparing `rattail_corepos-0.1.9/rattail_corepos/db/alembic/versions/9c5029effe93_more_model_extensions.py` & `rattail_corepos-0.2.0/rattail_corepos/db/alembic/versions/9c5029effe93_more_model_extensions.py`

 * *Files identical despite different names*

### Comparing `rattail_corepos-0.1.9/rattail_corepos/db/alembic/versions/b43e93d32275_initial_core_pos_integration_tables.py` & `rattail_corepos-0.2.0/rattail_corepos/db/alembic/versions/b43e93d32275_initial_core_pos_integration_tables.py`

 * *Files identical despite different names*

### Comparing `rattail_corepos-0.1.9/rattail_corepos/db/alembic/versions/c61f78243ff3_add_person_extension.py` & `rattail_corepos-0.2.0/rattail_corepos/db/alembic/versions/c61f78243ff3_add_person_extension.py`

 * *Files identical despite different names*

### Comparing `rattail_corepos-0.1.9/rattail_corepos/db/model/__init__.py` & `rattail_corepos-0.2.0/rattail_corepos/corepos/importing/db/exporters/catapult_membership.py`

 * *Files 24% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 # -*- coding: utf-8; -*-
 ################################################################################
 #
 #  Rattail -- Retail Software Framework
-#  Copyright © 2010-2021 Lance Edgar
+#  Copyright © 2010-2023 Lance Edgar
 #
 #  This file is part of Rattail.
 #
 #  Rattail is free software: you can redistribute it and/or modify it under the
 #  terms of the GNU General Public License as published by the Free Software
 #  Foundation, either version 3 of the License, or (at your option) any later
 #  version.
@@ -17,16 +17,17 @@
 #  details.
 #
 #  You should have received a copy of the GNU General Public License along with
 #  Rattail.  If not, see <http://www.gnu.org/licenses/>.
 #
 ################################################################################
 """
-Database schema extensions for CORE-POS integration
+CORE-POS -> Catapult Membership Workbook
 """
 
-from .stores import CoreStore
-from .people import CorePerson, CoreCustomer, CoreMember
-from .products import (CoreDepartment, CoreSubdepartment,
-                       CoreVendor, CoreProduct, CoreProductCost)
+import warnings
 
-from .batch.coremember import CoreMemberBatch, CoreMemberBatchRow
+warnings.warn("rattail_corepos.corepos.importing is deprecated; "
+              "please use rattail_corepos.corepos.office.importing instead",
+              DeprecationWarning, stacklevel=2)
+
+from rattail_corepos.corepos.office.importing.db.exporters.catapult_membership import *
```

### Comparing `rattail_corepos-0.1.9/rattail_corepos/db/model/batch/coremember.py` & `rattail_corepos-0.2.0/rattail_corepos/db/model/batch/coremember.py`

 * *Files 2% similar despite different names*

```diff
@@ -66,14 +66,15 @@
 
     STATUS = {
         STATUS_NO_CHANGE                : "no change",
         STATUS_MEMBER_NOT_FOUND         : "member not found",
         STATUS_FIELDS_CHANGED           : "update member",
     }
 
+    card_number_raw = sa.Column(sa.String(length=20), nullable=True)
     card_number = sa.Column(sa.Integer(), nullable=True)
 
     first_name = sa.Column(sa.String(length=30), nullable=True)
     first_name_old = sa.Column(sa.String(length=30), nullable=True)
     last_name = sa.Column(sa.String(length=30), nullable=True)
     last_name_old = sa.Column(sa.String(length=30), nullable=True)
```

### Comparing `rattail_corepos-0.1.9/rattail_corepos/db/model/products.py` & `rattail_corepos-0.2.0/rattail_corepos/db/model/products.py`

 * *Files 7% similar despite different names*

```diff
@@ -191,15 +191,28 @@
             '_corepos',
             uselist=False,
             cascade='all, delete-orphan',
             doc="""
             Reference to the CORE-POS extension record for this product cost.
             """))
 
-    corepos_id = sa.Column(sa.Integer(), nullable=False, doc="""
-    ``vendorItemID`` value for the corresponding record within CORE-POS.
+    corepos_vendor_id = sa.Column(sa.Integer(), nullable=False, doc="""
+    ``vendorItems.vendorID`` value for the corresponding record within
+    CORE-POS.
+    """)
+
+    corepos_sku = sa.Column(sa.String(length=13), nullable=False, doc="""
+    ``vendorItems.sku`` value for the corresponding record within
+    CORE-POS.
+    """)
+
+    corepos_id = sa.Column(sa.Integer(), nullable=True, doc="""
+    ``vendorItems.vendorItemID`` value for the corresponding record
+    within CORE-POS.
     """)
 
     def __str__(self):
         return str(self.cost)
 
+CoreProductCost.make_proxy(model.ProductCost, '_corepos', 'corepos_vendor_id')
+CoreProductCost.make_proxy(model.ProductCost, '_corepos', 'corepos_sku')
 CoreProductCost.make_proxy(model.ProductCost, '_corepos', 'corepos_id')
```

### Comparing `rattail_corepos-0.1.9/rattail_corepos/importing/__init__.py` & `rattail_corepos-0.2.0/rattail_corepos/db/__init__.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 # -*- coding: utf-8; -*-
 ################################################################################
 #
 #  Rattail -- Retail Software Framework
-#  Copyright © 2010-2020 Lance Edgar
+#  Copyright © 2010-2021 Lance Edgar
 #
 #  This file is part of Rattail.
 #
 #  Rattail is free software: you can redistribute it and/or modify it under the
 #  terms of the GNU General Public License as published by the Free Software
 #  Foundation, either version 3 of the License, or (at your option) any later
 #  version.
@@ -17,11 +17,12 @@
 #  details.
 #
 #  You should have received a copy of the GNU General Public License along with
 #  Rattail.  If not, see <http://www.gnu.org/licenses/>.
 #
 ################################################################################
 """
-Importing data into Rattail
+CORE POS Database Stuff
 """
 
-from . import model
+# TODO: deprecate / remove this
+from corepos.db.office_op import Session
```

### Comparing `rattail_corepos-0.1.9/rattail_corepos/importing/corepos/__init__.py` & `rattail_corepos-0.2.0/rattail_corepos/importing/corepos/__init__.py`

 * *Files identical despite different names*

### Comparing `rattail_corepos-0.1.9/rattail_corepos/importing/corepos/api.py` & `rattail_corepos-0.2.0/rattail_corepos/importing/corepos/api.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 # -*- coding: utf-8; -*-
 ################################################################################
 #
 #  Rattail -- Retail Software Framework
-#  Copyright © 2010-2021 Lance Edgar
+#  Copyright © 2010-2024 Lance Edgar
 #
 #  This file is part of Rattail.
 #
 #  Rattail is free software: you can redistribute it and/or modify it under the
 #  terms of the GNU General Public License as published by the Free Software
 #  Foundation, either version 3 of the License, or (at your option) any later
 #  version.
@@ -23,101 +23,142 @@
 """
 CORE POS (API) -> Rattail data importing
 """
 
 import datetime
 import decimal
 import logging
+from collections import OrderedDict
 
 from sqlalchemy import orm
 
 from rattail import importing
-from rattail.gpc import GPC
-from rattail.util import OrderedDict
-from rattail.time import localtime, make_utc
-from rattail.core import get_uuid
 from rattail.db.util import normalize_full_name
 from rattail_corepos import importing as corepos_importing
 from rattail_corepos.corepos.util import get_core_members
-from rattail_corepos.corepos.api import make_corepos_api
 
 
 log = logging.getLogger(__name__)
 
 
 class FromCOREPOSToRattail(importing.ToRattailHandler):
     """
     Import handler for data coming from a CORE POS API.
     """
+    host_key = 'corepos_api'
+    generic_host_title = "CORE Office (API)"
     host_title = "CORE-POS (API)"
+    safe_for_web_app = True
 
     def get_importers(self):
         importers = OrderedDict()
         importers['Customer'] = CustomerImporter
-        importers['Person'] = PersonImporter
-        importers['CustomerPerson'] = CustomerPersonImporter
+        importers['CustomerShopper'] = CustomerShopperImporter
+        importers['MembershipType'] = MembershipTypeImporter
         importers['Member'] = MemberImporter
         importers['Store'] = StoreImporter
         importers['Department'] = DepartmentImporter
         importers['Subdepartment'] = SubdepartmentImporter
         importers['Vendor'] = VendorImporter
         importers['Product'] = ProductImporter
         importers['ProductCost'] = ProductCostImporter
         importers['ProductMovement'] = ProductMovementImporter
         return importers
 
     def get_default_keys(self):
-        keys = super(FromCOREPOSToRattail, self).get_default_keys()
+        keys = super().get_default_keys()
+
         if 'ProductMovement' in keys:
             keys.remove('ProductMovement')
         return keys
 
+    def get_core_members(self, api, progress=None):
+        if not hasattr(self, 'cached_core_members'):
+            self.cached_core_members = get_core_members(
+                self.config, api, progress=progress)
+        return self.cached_core_members
+
 
 class FromCOREPOSAPI(importing.Importer):
     """
     Base class for all CORE POS API data importers.
     """
 
     def setup(self):
-        super(FromCOREPOSAPI, self).setup()
+        super().setup()
+
+        self.establish_api()
+
+        self.ignore_new_members = self.should_ignore_new_members()
+
+    def datasync_setup(self):
+        super().datasync_setup()
+
         self.establish_api()
 
     def establish_api(self):
-        self.api = make_corepos_api(self.config)
+        self.api = self.app.get_corepos_handler().make_webapi()
+
+    def should_ignore_new_members(self):
+        if hasattr(self, 'ignore_new_members'):
+            return self.ignore_new_members
+
+        return self.config.getbool('rattail_corepos',
+                                   'importing_ignore_new_members',
+                                   default=False)
 
     def get_core_members(self):
-        return get_core_members(self.api, progress=self.progress)
+        members = self.handler.get_core_members(self.api, progress=self.progress)
+
+        # maybe ignore NEW MEMBER accounts
+        if self.should_ignore_new_members():
+            members = [member for member in members
+                       if not self.is_new_member(member)]
+
+        return members
+
+    def is_new_member(self, member):
+        """
+        Convenience method to check if the given member represents a
+        "NEW MEMBER" record in CORE-POS, and hence it should be
+        ignored for the import.
+        """
+        customers = member['customers']
+        if customers:
+            customer = customers[0]
+            if (not customer['firstName']
+                and customer['lastName'] == 'NEW MEMBER'):
+                return True
+        return False
 
 
 class CustomerImporter(FromCOREPOSAPI, corepos_importing.model.CustomerImporter):
     """
     Importer for customer data from CORE POS API.
     """
-    key = 'corepos_account_id'
+    key = 'corepos_card_number'
     supported_fields = [
+        'corepos_card_number',
         'corepos_account_id',
-        'id',
         'number',
         'name',
+        # 'account_holder_first_name',
+        # 'account_holder_last_name',
         'address_street',
         'address_street2',
         'address_city',
         'address_state',
         'address_zipcode',
     ]
 
     def get_host_objects(self):
         return self.get_core_members()
 
     def normalize_host_object(self, member):
-
-        if member['customerAccountID'] == 0:
-            log.debug("member %s has customerAccountID of 0: %s",
-                      member['cardNo'], member)
-            return
+        card_number = int(member['cardNo'])
 
         # figure out the "account holder" customer for the member.  note that
         # we only use this to determine the `Customer.name` in Rattail
         customers = member['customers']
         account_holders = [customer for customer in customers
                            if customer['accountHolder']]
         if account_holders:
@@ -129,73 +170,105 @@
             if len(customers) > 1:
                 log.warning("member %s has %s customers but no account holders: %s",
                             member['cardNo'], len(customers), member)
             customer = customers[0]
         else:
             raise NotImplementedError("TODO: how to handle member with no customers?")
 
-        return {
+        data = {
+            'corepos_card_number': card_number,
             'corepos_account_id': int(member['customerAccountID']),
-            'id': member['customerAccountID'],
-            'number': int(member['cardNo']),
+            'number': card_number,
             'name': normalize_full_name(customer['firstName'],
                                         customer['lastName']),
 
+            # 'account_holder_first_name': customer['firstName'],
+            # 'account_holder_last_name': customer['lastName'],
             'address_street': member['addressFirstLine'] or None,
             'address_street2': member['addressSecondLine'] or None,
             'address_city': member['city'] or None,
             'address_state': member['state'] or None,
             'address_zipcode': member['zip'] or None,
         }
 
+        return data
+
 
-class PersonImporter(FromCOREPOSAPI, corepos_importing.model.PersonImporter):
+class CustomerShopperImporter(FromCOREPOSAPI, corepos_importing.model.CustomerShopperImporter):
     """
-    Importer for person data from CORE POS API.
+    Importer for customer shopper data from CORE POS API.
     """
-    key = 'corepos_customer_id'
+    key = ('customer_uuid', 'shopper_number')
     supported_fields = [
+        'customer_uuid',
+        'shopper_number',
         'corepos_customer_id',
         'first_name',
         'last_name',
         'display_name',
-        'customer_uuid',
-        'customer_person_ordinal',
+        'active',
         'phone_number',
         'phone_number_2',
         'email_address',
+        'account_holder',
     ]
 
     def setup(self):
-        super(PersonImporter, self).setup()
-        model = self.config.get_model()
+        super().setup()
+        model = self.model
 
-        self.customers = self.cache_model(model.Customer, key='id')
+        self.maxlen_phone_number = self.get_maxlen_phone_number()
+
+        self.customers_by_card_number = self.app.cache_model(
+            self.session,
+            model.Customer,
+            key='corepos_card_number',
+            query_options=[orm.joinedload(model.Customer._corepos)])
+
+    def get_maxlen_phone_number(self):
+        if hasattr(self, 'maxlen_phone_number'):
+            return self.maxlen_phone_number
+
+        model = self.model
+        return self.app.maxlen(model.PhoneNumber.number)
 
     def get_host_objects(self):
 
         # first get all member data from CORE API
         members = self.get_core_members()
         normalized = []
 
-        # then collect all the "person" records
+        # then collect all the "shopper" records
         def normalize(member, i):
-            normalized.extend(self.get_person_objects_for_member(member))
+            normalized.extend(self.get_shoppers_for_member(member))
 
         self.progress_loop(normalize, members,
                            message="Collecting Person data from CORE")
         return normalized
 
-    def get_person_objects_for_member(self, member):
+    def get_customer_by_card_number(self, card_number):
+        if hasattr(self, 'customers_by_card_number'):
+            return self.customers_by_card_number.get(card_number)
+
+        model = self.model
+        try:
+            return self.session.query(model.Customer)\
+                               .join(model.CoreCustomer)\
+                               .filter(model.CoreCustomer.corepos_card_number == card_number)\
+                               .one()
+        except orm.exc.NoResultFound:
+            pass
+
+    def get_shoppers_for_member(self, member):
         """
-        Return a list of Person data objects for the given Member.  This
-        logic is split out separately so that datasync can leverage it too.
+        Return a list of shopper info dicts associated with the given
+        member info dict (latter having come from the CORE API).
         """
         customers = member['customers']
-        people = []
+        shoppers = []
 
         # make sure account holder is listed first
         account_holder = None
         secondary = False
         mixedup = False
         for customer in customers:
             if customer['accountHolder'] and not secondary:
@@ -204,152 +277,71 @@
                 secondary = True
             elif customer['accountHolder'] and secondary:
                 mixedup = True
         if mixedup:
             raise NotImplementedError("TODO: should re-sort the customers list for member {}".format(member['cardNo']))
 
         for i, customer in enumerate(customers, 1):
-            person = dict(customer)
-            person['customer_person_ordinal'] = i
-            people.append(person)
-
-        return people
-
-    def get_customer(self, id):
-        if hasattr(self, 'customers'):
-            return self.customers.get(id)
+            shopper = dict(customer)
+            shopper['card_number'] = member['cardNo']
+            shopper['shopper_number'] = i
+            shoppers.append(shopper)
 
-        model = self.config.get_model()
-        try:
-            return self.session.query(model.Customer)\
-                               .filter(model.Customer.id == id)\
-                               .one()
-        except orm.exc.NoResultFound:
-            pass
+        return shoppers
 
-    def normalize_host_object(self, person):
+    def normalize_host_object(self, shopper):
+        card_number = shopper['card_number']
 
-        customer = self.get_customer(person['customerAccountID'])
+        customer = self.get_customer_by_card_number(card_number)
         if not customer:
-            log.warning("Rattail customer not found for customerAccountID: %s",
-                        person['customerAccountID'])
+            log.warning("Rattail customer not found for CardNo %s: %s",
+                        card_number, shopper)
             return
 
-        return {
-            'corepos_customer_id': int(person['customerID']),
-            'first_name': person['firstName'],
-            'last_name': person['lastName'],
-            'display_name': normalize_full_name(person['firstName'],
-                                                person['lastName']),
+        data = {
             'customer_uuid': customer.uuid,
-            'customer_person_ordinal': person['customer_person_ordinal'],
-            'phone_number': person['phone'] or None,
-            'phone_number_2': person['altPhone'] or None,
-            'email_address': person['email'] or None,
-        }
-
-
-class CustomerPersonImporter(FromCOREPOSAPI, importing.model.CustomerPersonImporter):
-    """
-    Importer for customer-person linkage data from CORE POS API.
-
-    Note that we don't use this one in datasync, it's just for nightly
-    double-check.
-    """
-    key = ('customer_uuid', 'person_uuid')
-    supported_fields = [
-        'customer_uuid',
-        'person_uuid',
-        'ordinal',
-    ]
-
-    def setup(self):
-        super(CustomerPersonImporter, self).setup()
-        model = self.config.get_model()
-
-        query = self.session.query(model.Customer)\
-                            .join(model.CoreCustomer)
-        self.customers = self.cache_model(model.Customer, query=query,
-                                          key='corepos_account_id')
-
-        query = self.session.query(model.Person)\
-                            .join(model.CorePerson)\
-                            .filter(model.CorePerson.corepos_customer_id != None)
-        self.people = self.cache_model(model.Person, query=query,
-                                       key='corepos_customer_id',
-                                       query_options=[orm.joinedload(model.Person._corepos)])
-
-    def get_host_objects(self):
-
-        # first get all member data from CORE API
-        members = self.get_core_members()
-        normalized = []
-
-        # then collect all customer/person combination records
-        def normalize(member, i):
-            # make sure we put the account holder first in the list!
-            customers = sorted(member['customers'],
-                               key=lambda cust: 1 if cust['accountHolder'] else 0,
-                               reverse=True)
-            for i, customer in enumerate(customers, 1):
-                normalized.append({
-                    'customer_account_id': int(member['customerAccountID']),
-                    'person_customer_id': customer['customerID'],
-                    'ordinal': i,
-                })
+            'shopper_number': shopper['shopper_number'],
+            'corepos_customer_id': int(shopper['customerID']),
 
-        self.progress_loop(normalize, members,
-                           message="Collecting CustomerPerson data from CORE")
-        return normalized
-
-    def get_customer(self, account_id):
-        if hasattr(self, 'customers'):
-            return self.customers.get(account_id)
-
-        model = self.config.get_model()
-        try:
-            return self.session.query(model.Customer)\
-                               .join(model.CoreCustomer)\
-                               .filter(model.CoreCustomer.corepos_account_id == account_id)\
-                               .one()
-        except orm.exc.NoResultFound:
-            pass
-
-    def get_person(self, corepos_customer_id):
-        if hasattr(self, 'people'):
-            return self.people.get(corepos_customer_id)
-
-        model = self.config.get_model()
-        try:
-            return self.session.query(model.Person)\
-                               .join(model.CorePerson)\
-                               .filter(model.CorePerson.corepos_customer_id == corepos_customer_id)\
-                               .one()
-        except orm.exc.NoResultFound:
-            pass
+            'first_name': shopper['firstName'],
+            'last_name': shopper['lastName'],
+            'display_name': normalize_full_name(shopper['firstName'],
+                                                shopper['lastName']),
+
+            # TODO: can a CORE shopper be *not* active?
+            'active': True,
+
+            'phone_number': shopper['phone'] or None,
+            'phone_number_2': shopper['altPhone'] or None,
+
+            'email_address': shopper['email'] or None,
+            'account_holder': bool(shopper['accountHolder']),
+        }
+
+        # truncate phone number data if needed
+        maxlen_phone_number = self.get_maxlen_phone_number()
+        if data['phone_number'] and len(data['phone_number']) > maxlen_phone_number:
+            log.warning("phone_number is too long (%s chars), "
+                        "will truncate to %s chars: %s",
+                        len(data['phone_number']),
+                        maxlen_phone_number,
+                        data['phone_number'])
+            data['phone_number'] = data['phone_number'][:maxlen_phone_number]
+        if data['phone_number_2'] and len(data['phone_number_2']) > maxlen_phone_number:
+            log.warning("phone_number_2 is too long (%s chars), "
+                        "will truncate to %s chars: %s",
+                        len(data['phone_number_2']),
+                        maxlen_phone_number,
+                        data['phone_number_2'])
+            data['phone_number_2'] = data['phone_number_2'][:maxlen_phone_number]
 
-    def normalize_host_object(self, cp):
+        # swap 1st and 2nd phone numbers if only latter has value
+        self.prioritize_2(data, 'phone_number')
 
-        customer = self.get_customer(cp['customer_account_id'])
-        if not customer:
-            log.warning("Rattail customer not found for customerAccountID: %s",
-                        cp['customer_account_id'])
-            return
-
-        person = self.get_person(int(cp['person_customer_id']))
-        if not person:
-            log.warning("Rattail person not found for customerID: %s",
-                        cp['person_customer_id'])
-            return
-
-        return {
-            'customer_uuid': customer.uuid,
-            'person_uuid': person.uuid,
-            'ordinal': cp['ordinal'],
-        }
+        return data
 
 
 class StoreImporter(FromCOREPOSAPI, corepos_importing.model.StoreImporter):
     """
     Importer for store data from CORE POS API.
     """
     key = 'corepos_id'
@@ -411,15 +403,15 @@
         department_number = None
         if 'dept_ID' in subdepartment:
             department_number = int(subdepartment['dept_ID'])
 
         return {
             'corepos_number': int(subdepartment['subdept_no']),
             'number': int(subdepartment['subdept_no']),
-            'name': subdepartment['subdept_name'],
+            'name': subdepartment.get('subdept_name'),
             'department_number': department_number,
         }
 
 
 class VendorImporter(FromCOREPOSAPI, corepos_importing.model.VendorImporter):
     """
     Importer for vendor data from CORE POS API.
@@ -439,15 +431,15 @@
     def get_host_objects(self):
         return self.api.get_vendors()
 
     def normalize_host_object(self, vendor):
         return {
             'corepos_id': int(vendor['vendorID']),
             'id': str(vendor['vendorID']),
-            'name': vendor['vendorName'],
+            'name': vendor.get('vendorName'),
             'abbreviation': vendor.get('vendorAbbreviation') or None,
             'special_discount': decimal.Decimal(vendor['discountRate']),
             'phone_number': vendor.get('phone') or None,
             'fax_number': vendor.get('fax') or None,
             'email_address': vendor.get('email') or None,
         }
 
@@ -477,32 +469,36 @@
         'food_stampable',
         # 'tax1',
         # 'tax2',
         'case_size',
     ]
 
     def setup(self):
-        super(ProductImporter, self).setup()
+        super().setup()
         model = self.model
 
         query = self.session.query(model.Product)\
                             .join(model.CoreProduct)\
                             .filter(model.CoreProduct.corepos_id != None)\
                             .options(orm.joinedload(model.Product._corepos))
-        self.core_existing = self.cache_model(model.Product, key='corepos_id',
-                                              query=query)
+        self.core_existing = self.app.cache_model(self.session,
+                                                  model.Product,
+                                                  key='corepos_id',
+                                                  query=query)
 
         self.vendor_items_by_upc = {}
 
         def cache(item, i):
             self.vendor_items_by_upc.setdefault(item['upc'], []).append(item)
 
         self.progress_loop(cache, self.api.get_vendor_items(),
                            message="Caching CORE Vendor Items")
 
+        self.maxval_unit_size = self.app.maxval(model.Product.unit_size)
+
     def get_host_objects(self):
         return self.api.get_products()
 
     def identify_product(self, corepos_product):
         model = self.config.get_model()
         corepos_id = int(corepos_product['id'])
 
@@ -527,25 +523,29 @@
                            .filter(model.Product.item_id == corepos_product['upc'])\
                            .first()
 
     def identify_product_uuid(self, corepos_product):
         product = self.identify_product(corepos_product)
         if product:
             return product.uuid
-        return get_uuid()
+        return self.app.make_uuid()
 
     def get_vendor_items(self, api_product):
         if hasattr(self, 'vendor_items_by_upc'):
             return self.vendor_items_by_upc.get(api_product['upc'])
 
         return self.api.get_vendor_items(upc=api_product['upc'])
 
     def normalize_host_object(self, product):
+        if 'upc' not in product:
+            log.warning("CORE-POS product has no UPC: %s", product)
+            return
+
         try:
-            upc = GPC(product['upc'], calc_check_digit='upc')
+            upc = self.app.make_gpc(product['upc'], calc_check_digit='upc')
         except (TypeError, ValueError):
             log.debug("CORE POS product has invalid UPC: %s", product['upc'])
             if len(self.key) == 1 and self.key[0] == 'upc':
                 return
             upc = None
 
         department_number = None
@@ -567,33 +567,41 @@
             'upc': upc,
             'brand_name': product.get('brand') or None,
             'description': product.get('description') or '',
 
             'department_number': department_number,
             'subdepartment_number': subdepartment_number,
 
-            'weighed': product['scale'] == '1',
-            'food_stampable': product['foodstamp'] == '1',
+            'weighed': product.get('scale') == '1',
+            'food_stampable': None,
             # 'tax1': product['tax'] == '1', # TODO: is this right?
             # 'tax2': product['tax'] == '2', # TODO: is this right?
 
             'regular_price_price': price,
             'regular_price_multiple': 1 if price is not None else None,
             'regular_price_type': self.enum.PRICE_TYPE_REGULAR if price is not None else None,
         }
 
+        if 'foodstamp' in product:
+            data['food_stampable'] = product['foodstamp'] == '1'
+
         if self.fields_active(self.size_fields):
             size_info = self.normalize_size_info(product)
             data.update({
                 'size': size_info['size'],
                 'unit_size': size_info['unit_size'],
                 'unit_of_measure': size_info['uom_code'],
-                'uom_abbreviation': size_info['uom_abbrev'],
+                'uom_abbreviation': (size_info['uom_abbrev'] or '').strip() or None,
             })
 
+            if data['unit_size'] and data['unit_size'] >= self.maxval_unit_size:
+                log.warning("unit_size too large (%s) for product %s, will use null instead: %s",
+                            data['unit_size'], data['upc'], product)
+                data['unit_size'] = None
+
         if 'case_size' in self.fields:
             case_size = None
             items = self.get_vendor_items(product)
             if items:
                 # here we sort by `modified DESC` to get the "deterministic
                 # pseudo-default" vendorItems record
 
@@ -629,59 +637,66 @@
         return self.api.get_products()
 
     def normalize_host_object(self, product):
 
         last_sold = None
         if 'last_sold' in product:
             last_sold = datetime.datetime.strptime(product['last_sold'], '%Y-%m-%d %H:%M:%S')
-            last_sold = localtime(self.config, last_sold)
-            last_sold = make_utc(last_sold)
+            last_sold = self.app.localtime(last_sold)
+            last_sold = self.app.make_utc(last_sold)
 
         return {
             'corepos_id': int(product['id']),
             'last_sold': last_sold,
         }
 
 
 class ProductCostImporter(FromCOREPOSAPI, corepos_importing.model.ProductCostImporter):
     """
     Importer for product cost data from CORE POS API.
     """
+    # TODO: should change key after live sites are updated
     key = ('vendor_uuid', 'code')
+    # key = ('corepos_vendor_id', 'corepos_sku')
     supported_fields = [
-        'corepos_id',
+        'corepos_vendor_id',
+        'corepos_sku',
         'product_uuid',
         'vendor_uuid',
         'code',
         'case_size',
         'case_cost',
         'unit_cost',
         'preferred',
     ]
 
     def setup(self):
-        super(ProductCostImporter, self).setup()
+        super().setup()
         model = self.config.get_model()
 
         query = self.session.query(model.Vendor)\
                             .join(model.CoreVendor)\
                             .filter(model.CoreVendor.corepos_id != None)
-        self.vendors = self.cache_model(model.Vendor, query=query,
-                                        key='corepos_id')
+        self.vendors = self.app.cache_model(self.session,
+                                            model.Vendor,
+                                            query=query,
+                                            key='corepos_id')
 
         self.corepos_products = {}
 
         def cache(product, i):
-            self.corepos_products[product['upc']] = product
+            if 'upc' in product:
+                self.corepos_products[product['upc']] = product
 
         self.progress_loop(cache, self.api.get_products(),
                            message="Caching Products from CORE-POS API")
 
-        self.products_by_item_id = self.cache_model(model.Product,
-                                                    key='item_id')
+        self.products_by_item_id = self.app.cache_model(self.session,
+                                                        model.Product,
+                                                        key='item_id')
 
     def get_host_objects(self):
         return self.api.get_vendor_items()
 
     def get_vendor(self, item):
         corepos_id = int(item['vendorID'])
 
@@ -721,54 +736,88 @@
         vendor = self.get_vendor(item)
         if not vendor:
             log.warning("CORE POS vendor not found for item: %s", item)
             return
 
         product = self.get_product(item)
         if not product:
-            log.warning("product not found for CORE vendor item: %s", item)
+            # just debug logging since this is a common scenario; the
+            # CORE table is for items "available from vendor" but not
+            # necssarily items carried by store
+            log.debug("product not found for CORE vendor item: %s", item)
             return
 
         core_product = self.get_corepos_product(item)
         # if not product:
         #     log.warning("CORE POS product not found for item: %s", item)
         #     return
 
         preferred = False
         if core_product and core_product['default_vendor_id'] == item['vendorID']:
             preferred = True
 
         case_size = decimal.Decimal(item['units'])
-        unit_cost = decimal.Decimal(item['cost'])
+        unit_cost = item.get('cost')
+        if unit_cost is not None:
+            unit_cost = decimal.Decimal(unit_cost)
+        case_cost = None
+        if unit_cost is not None:
+            case_cost = unit_cost * case_size
 
         return {
-            'corepos_id': int(item['vendorItemID']),
+            'corepos_vendor_id': int(item['vendorID']),
+            'corepos_sku': item['sku'],
             'product_uuid': product.uuid,
             'vendor_uuid': vendor.uuid,
             'code': (item['sku'] or '').strip() or None,
             'case_size': case_size,
-            'case_cost': case_size * unit_cost,
+            'case_cost': case_cost,
             'unit_cost': unit_cost,
             'preferred': preferred,
         }
 
 
+class MembershipTypeImporter(FromCOREPOSAPI, importing.model.MembershipTypeImporter):
+    """
+    Imports membership type data from CORE-POS API
+    """
+    key = 'number'
+    supported_fields = [
+        'number',
+        'name',
+    ]
+
+    def get_host_objects(self):
+        return self.api.get_member_types()
+
+    def normalize_host_object(self, memtype):
+        return {
+            'number': int(memtype['memtype']),
+            'name': memtype['memDesc'],
+        }
+
+
 class MemberImporter(FromCOREPOSAPI, corepos_importing.model.MemberImporter):
     """
     Importer for member data from CORE POS API.
     """
-    key = 'corepos_account_id'
+    # TODO use this key instead
+    #key = 'corepos_card_number'
+    key = 'number'
     supported_fields = [
-        'corepos_account_id',
         'number',
-        'id',
+        'corepos_account_id',
+        'corepos_card_number',
         'customer_uuid',
-        'person_uuid',
+        'person_first_name',
+        'person_last_name',
+        'membership_type_number',
         'joined',
         'withdrew',
+        'active',
     ]
 
     # TODO: should make this configurable
     member_status_codes = [
         'PC',
         'TERM',
     ]
@@ -776,69 +825,94 @@
     # TODO: should make this configurable
     non_member_status_codes = [
         'REG',
         'INACT',
     ]
 
     def setup(self):
-        super(MemberImporter, self).setup()
-        model = self.config.get_model()
-        self.customers = self.cache_model(model.Customer, key='number')
+        super().setup()
+        model = self.model
+
+        self.customers_by_number = self.app.cache_model(
+            self.session,
+            model.Customer,
+            key='number')
 
     def get_host_objects(self):
         return self.get_core_members()
 
-    def get_customer(self, number):
-        if hasattr(self, 'customers'):
-            return self.customers.get(number)
+    def get_customer_by_number(self, number):
+        if hasattr(self, 'customers_by_number'):
+            return self.customers_by_number.get(number)
 
-        model = self.config.get_model()
+        model = self.model
         try:
             return self.session.query(model.Customer)\
                                .filter(model.Customer.number == number)\
                                .one()
         except orm.exc.NoResultFound:
             pass
 
-    def normalize_host_object(self, member):
-        customer = self.get_customer(member['cardNo'])
-        if not customer:
-            log.warning("Rattail customer not found for cardNo %s: %s",
-                        member['cardNo'], member)
-            return
+    def get_corepos_customer(self, corepos_member):
+        for customer in corepos_member['customers']:
+            if customer['accountHolder']:
+                return customer
 
-        person = customer.first_person()
-        if not person:
-            log.warning("Rattail person not found for cardNo %s: %s",
-                        member['cardNo'], member)
-            return
+    def normalize_host_object(self, member):
+        card_number = member['cardNo']
+        customer = self.get_customer_by_number(card_number)
 
-        if member['memberStatus'] in self.non_member_status_codes:
-            log.debug("skipping non-member %s with status '%s': %s",
-                      member['memberStatus'], member['cardNo'], member)
-            return
-        if member['memberStatus'] not in self.member_status_codes:
-            # note that we will still import this one! we don't skip it
+        # TODO: at first i was *skipping* non-member status records,
+        # but since CORE sort of assumes all customers are members,
+        # probably not worth making the distinction here..?  it is
+        # important to import the full member info from CORE, so that
+        # we have it to sync back.  therefore can't afford to "skip"
+        # any member records here
+        if (member['memberStatus'] not in self.member_status_codes
+            and member['memberStatus'] not in self.non_member_status_codes):
             log.warning("unexpected status '%s' for member %s: %s",
-                        member['memberStatus'], member['cardNo'], member)
+                        member['memberStatus'], card_number, member)
 
         joined = None
         if member['startDate'] and member['startDate'] != '0000-00-00 00:00:00':
             joined = datetime.datetime.strptime(member['startDate'],
                                                 '%Y-%m-%d %H:%M:%S')
             joined = joined.date()
+            if joined == datetime.date(1900, 1, 1):
+                joined = None
 
         withdrew = None
-        if member['endDate'] and member['endDate'] != '0000-00-00 00:00:00':
+        if (member['endDate']
+            and member['endDate'] != '0000-00-00 00:00:00'
+            and member['endDate'] != '1900-01-01 00:00:00'):
             withdrew = datetime.datetime.strptime(member['endDate'],
                                                   '%Y-%m-%d %H:%M:%S')
             withdrew = withdrew.date()
+            if withdrew == datetime.date(1900, 1, 1):
+                withdrew = None
 
-        return {
+        typeno = int(member['customerTypeID'] or 0)
+        memtype = self.get_membership_type_by_number(typeno)
+        if not memtype:
+            log.warning("unknown customerTypeID (membership_type_number) '%s' for: %s",
+                        member['customerTypeID'], member)
+            typeno = None
+
+        data = {
+            'number': card_number,
             'corepos_account_id': int(member['customerAccountID']),
-            'number': int(member['cardNo']),
-            'id': str(member['customerAccountID']),
-            'customer_uuid': customer.uuid,
-            'person_uuid': person.uuid,
+            'corepos_card_number': card_number,
+            'customer_uuid': customer.uuid if customer else None,
+            'person_first_name': None,
+            'person_last_name': None,
+            'membership_type_number': typeno,
             'joined': joined,
             'withdrew': withdrew,
+            'active': not bool(withdrew),
         }
+
+        corepos_customer = self.get_corepos_customer(member)
+        if corepos_customer:
+            data['person_first_name'] = corepos_customer['firstName']
+            data['person_last_name'] = corepos_customer['lastName']
+
+        return data
```

### Comparing `rattail_corepos-0.1.9/rattail_corepos/importing/versions.py` & `rattail_corepos-0.2.0/rattail_corepos/importing/versions.py`

 * *Files 26% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 # -*- coding: utf-8; -*-
 ################################################################################
 #
 #  Rattail -- Retail Software Framework
-#  Copyright © 2010-2021 Lance Edgar
+#  Copyright © 2010-2023 Lance Edgar
 #
 #  This file is part of Rattail.
 #
 #  Rattail is free software: you can redistribute it and/or modify it under the
 #  terms of the GNU General Public License as published by the Free Software
 #  Foundation, either version 3 of the License, or (at your option) any later
 #  version.
@@ -30,16 +30,19 @@
 class CoreposVersionMixin(object):
     """
     Add default registration of custom importers
     """
 
     def add_corepos_importers(self, importers):
         importers['CorePerson'] = CorePersonImporter
+        importers['CoreEmployee'] = CoreEmployeeImporter
         importers['CoreCustomer'] = CoreCustomerImporter
+        importers['CoreCustomerShopper'] = CoreCustomerShopperImporter
         importers['CoreMember'] = CoreMemberImporter
+        importers['CoreMemberEquityPayment'] = CoreMemberEquityPaymentImporter
         importers['CoreStore'] = CoreStoreImporter
         importers['CoreDepartment'] = CoreDepartmentImporter
         importers['CoreSubdepartment'] = CoreSubdepartmentImporter
         importers['CoreVendor'] = CoreVendorImporter
         importers['CoreProduct'] = CoreProductImporter
         return importers
 
@@ -48,30 +51,53 @@
 
     @property
     def host_model_class(self):
         model = self.config.get_model()
         return model.CorePerson
 
 
+class CoreEmployeeImporter(base.VersionImporter):
+
+    @property
+    def host_model_class(self):
+        model = self.config.get_model()
+        return model.CoreEmployee
+
+
 class CoreCustomerImporter(base.VersionImporter):
 
     @property
     def host_model_class(self):
         model = self.config.get_model()
         return model.CoreCustomer
 
 
+class CoreCustomerShopperImporter(base.VersionImporter):
+
+    @property
+    def host_model_class(self):
+        return self.model.CoreCustomerShopper
+
+
 class CoreMemberImporter(base.VersionImporter):
 
     @property
     def host_model_class(self):
         model = self.config.get_model()
         return model.CoreMember
 
 
+class CoreMemberEquityPaymentImporter(base.VersionImporter):
+
+    @property
+    def host_model_class(self):
+        model = self.config.get_model()
+        return model.CoreMemberEquityPayment
+
+
 class CoreStoreImporter(base.VersionImporter):
 
     @property
     def host_model_class(self):
         model = self.config.get_model()
         return model.CoreStore
```

### Comparing `rattail_corepos-0.1.9/rattail_corepos/products.py` & `rattail_corepos-0.2.0/rattail_corepos/products.py`

 * *Files identical despite different names*

### Comparing `rattail_corepos-0.1.9/rattail_corepos/trainwreck/importing/corepos.py` & `rattail_corepos-0.2.0/rattail_corepos/trainwreck/importing/corepos.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 # -*- coding: utf-8; -*-
 ################################################################################
 #
 #  Rattail -- Retail Software Framework
-#  Copyright © 2010-2021 Lance Edgar
+#  Copyright © 2010-2023 Lance Edgar
 #
 #  This file is part of Rattail.
 #
 #  Rattail is free software: you can redistribute it and/or modify it under the
 #  terms of the GNU General Public License as published by the Free Software
 #  Foundation, either version 3 of the License, or (at your option) any later
 #  version.
@@ -20,28 +20,31 @@
 #  Rattail.  If not, see <http://www.gnu.org/licenses/>.
 #
 ################################################################################
 """
 CORE-POS -> Trainwreck data importing
 """
 
+from collections import OrderedDict
+
 from corepos.db.office_trans import Session as CoreTransSession, model as coretrans
 from corepos.db.office_op import Session as CoreSession, model as corepos
 
 from rattail import importing
-from rattail.util import OrderedDict
 from rattail.time import localtime, make_utc
 from rattail.trainwreck import importing as trainwreck_importing
 
 
 class FromCoreToTrainwreck(importing.FromSQLAlchemyHandler, trainwreck_importing.ToTrainwreckHandler):
     """
     Import data from CORE-POS into Trainwreck
     """
+    host_key = 'corepos_db_office_trans'
     host_title = "CORE-POS"
+    generic_host_title = 'CORE Office (DB "trans")'
     corepos_dbkey = 'default'
 
     def make_host_session(self):
         return CoreTransSession(bind=self.config.coretrans_engines[self.corepos_dbkey])
 
     def get_importer_kwargs(self, key, **kwargs):
         kwargs = super(FromCoreToTrainwreck, self).get_importer_kwargs(key, **kwargs)
@@ -133,44 +136,44 @@
 
         if 'cashier_name' in self.fields:
             self.corepos_employees = self.cache_model(corepos.Employee,
                                                       session=self.core_op_session,
                                                       key='number')
 
         if 'customer_name' in self.fields:
-            query = self.core_op_session.query(corepos.CustData)\
-                                        .filter(corepos.CustData.person_number == 1)
-            self.corepos_customers = self.cache_model(corepos.CustData,
+            query = self.core_op_session.query(corepos.CustomerClassic)\
+                                        .filter(corepos.CustomerClassic.person_number == 1)
+            self.corepos_customers = self.cache_model(corepos.CustomerClassic,
                                                       session=self.core_op_session,
                                                       query=query,
                                                       key='card_number')
 
     def get_host_objects(self):
         details = self.fetch_details()
         transactions = []
         current = {}
 
         def collect(detail, i):
-            receipt_number = str(detail.transaction_number)
+
+            system_id = self.make_system_id(detail)
+            if current and current['system_id'] != system_id:
+                transactions.append(dict(current))
+                current.clear()
 
             date_time = detail.date_time
             if date_time:
                 date_time = localtime(self.config, date_time)
                 date_time = make_utc(date_time)
 
-            if current and current['receipt_number'] != receipt_number:
-                transactions.append(dict(current))
-                current.clear()
-
             if not current:
                 current.update({
                     'system': self.enum.TRAINWRECK_SYSTEM_COREPOS,
-                    'system_id': self.make_system_id(detail),
+                    'system_id': system_id,
                     'terminal_id': str(detail.register_number),
-                    'receipt_number': receipt_number,
+                    'receipt_number': str(detail.transaction_number),
                     'cashier_id': str(detail.employee_number) if detail.employee_number else None,
                     'customer_id': str(detail.card_number) if detail.card_number else None,
                     'start_time': date_time,
                     'end_time': date_time,
                 })
 
             if detail.transaction_type == 'C':
```

### Comparing `rattail_corepos-0.1.9/rattail_corepos.egg-info/PKG-INFO` & `rattail_corepos-0.2.0/rattail_corepos.egg-info/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,29 +1,30 @@
 Metadata-Version: 2.1
-Name: rattail-corepos
-Version: 0.1.9
+Name: rattail_corepos
+Version: 0.2.0
 Summary: Rattail Software Interfaces for CORE POS
 Home-page: https://rattailproject.org/
 Author: Lance Edgar
 Author-email: lance@edbob.org
 License: GNU GPL v3
-Platform: UNKNOWN
 Classifier: Development Status :: 3 - Alpha
 Classifier: Environment :: Console
 Classifier: Environment :: Web Environment
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: GNU General Public License v3 or later (GPLv3+)
 Classifier: Natural Language :: English
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.5
 Classifier: Topic :: Office/Business
 Classifier: Topic :: Software Development :: Libraries :: Python Modules
 License-File: COPYING.txt
+Requires-Dist: pyCOREPOS
+Requires-Dist: rattail
 
 
 rattail_corepos
 ===============
 
 Rattail is a retail software framework, released under the GNU General Public
 License.
@@ -31,9 +32,7 @@
 This package contains software interfaces for the `CORE POS`_ system.
 
 .. _`CORE POS`: https://github.com/CORE-POS/IS4C
 
 Please see Rattail's `home page`_ for more information.
 
 .. _`home page`: https://rattailproject.org/
-
-
```

