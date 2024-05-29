# Comparing `tmp/digitalhub_data-0.5.0b4.tar.gz` & `tmp/digitalhub_data-0.5.0b5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "digitalhub_data-0.5.0b4.tar", last modified: Mon May 27 13:53:47 2024, max compression
+gzip compressed data, was "digitalhub_data-0.5.0b5.tar", last modified: Wed May 29 09:48:12 2024, max compression
```

## Comparing `digitalhub_data-0.5.0b4.tar` & `digitalhub_data-0.5.0b5.tar`

### file list

```diff
@@ -1,62 +1,62 @@
-drwxrwxr-x   0 mmartini  (1000) mmartini  (1000)        0 2024-05-27 13:53:47.562883 digitalhub_data-0.5.0b4/
--rw-r--r--   0 mmartini  (1000) mmartini  (1000)     1024 2024-05-27 13:53:47.562883 digitalhub_data-0.5.0b4/PKG-INFO
--rw-rw-r--   0 mmartini  (1000) mmartini  (1000)      468 2024-04-23 09:36:04.000000 digitalhub_data-0.5.0b4/README.md
-drwxrwxr-x   0 mmartini  (1000) mmartini  (1000)        0 2024-05-27 13:53:47.554883 digitalhub_data-0.5.0b4/digitalhub_data/
--rw-rw-r--   0 mmartini  (1000) mmartini  (1000)      329 2024-05-27 13:03:31.000000 digitalhub_data-0.5.0b4/digitalhub_data/__init__.py
-drwxrwxr-x   0 mmartini  (1000) mmartini  (1000)        0 2024-05-27 13:53:47.558883 digitalhub_data-0.5.0b4/digitalhub_data/datastores/
--rw-rw-r--   0 mmartini  (1000) mmartini  (1000)        0 2024-05-21 09:37:15.000000 digitalhub_data-0.5.0b4/digitalhub_data/datastores/__init__.py
--rw-rw-r--   0 mmartini  (1000) mmartini  (1000)     3209 2024-05-23 09:43:05.000000 digitalhub_data-0.5.0b4/digitalhub_data/datastores/builder.py
-drwxrwxr-x   0 mmartini  (1000) mmartini  (1000)        0 2024-05-27 13:53:47.558883 digitalhub_data-0.5.0b4/digitalhub_data/datastores/objects/
--rw-rw-r--   0 mmartini  (1000) mmartini  (1000)        0 2024-05-21 09:37:57.000000 digitalhub_data-0.5.0b4/digitalhub_data/datastores/objects/__init__.py
--rw-rw-r--   0 mmartini  (1000) mmartini  (1000)     3443 2024-05-22 13:22:43.000000 digitalhub_data-0.5.0b4/digitalhub_data/datastores/objects/base.py
--rw-rw-r--   0 mmartini  (1000) mmartini  (1000)     1350 2024-05-23 09:43:30.000000 digitalhub_data-0.5.0b4/digitalhub_data/datastores/objects/local.py
--rw-rw-r--   0 mmartini  (1000) mmartini  (1000)      667 2024-05-23 09:43:30.000000 digitalhub_data-0.5.0b4/digitalhub_data/datastores/objects/remote.py
--rw-rw-r--   0 mmartini  (1000) mmartini  (1000)     1202 2024-05-23 09:43:30.000000 digitalhub_data-0.5.0b4/digitalhub_data/datastores/objects/s3.py
--rw-rw-r--   0 mmartini  (1000) mmartini  (1000)     1863 2024-05-23 09:43:30.000000 digitalhub_data-0.5.0b4/digitalhub_data/datastores/objects/sql.py
-drwxrwxr-x   0 mmartini  (1000) mmartini  (1000)        0 2024-05-27 13:53:47.558883 digitalhub_data-0.5.0b4/digitalhub_data/entities/
--rw-rw-r--   0 mmartini  (1000) mmartini  (1000)        0 2024-01-30 10:40:56.000000 digitalhub_data-0.5.0b4/digitalhub_data/entities/__init__.py
-drwxrwxr-x   0 mmartini  (1000) mmartini  (1000)        0 2024-05-27 13:53:47.558883 digitalhub_data-0.5.0b4/digitalhub_data/entities/dataitems/
--rw-rw-r--   0 mmartini  (1000) mmartini  (1000)        0 2024-01-30 10:40:45.000000 digitalhub_data-0.5.0b4/digitalhub_data/entities/dataitems/__init__.py
--rw-rw-r--   0 mmartini  (1000) mmartini  (1000)     3322 2024-05-27 13:03:31.000000 digitalhub_data-0.5.0b4/digitalhub_data/entities/dataitems/builder.py
--rw-rw-r--   0 mmartini  (1000) mmartini  (1000)     6484 2024-05-27 13:03:31.000000 digitalhub_data-0.5.0b4/digitalhub_data/entities/dataitems/crud.py
-drwxrwxr-x   0 mmartini  (1000) mmartini  (1000)        0 2024-05-27 13:53:47.558883 digitalhub_data-0.5.0b4/digitalhub_data/entities/dataitems/entity/
--rw-rw-r--   0 mmartini  (1000) mmartini  (1000)        0 2024-03-04 14:42:21.000000 digitalhub_data-0.5.0b4/digitalhub_data/entities/dataitems/entity/__init__.py
--rw-rw-r--   0 mmartini  (1000) mmartini  (1000)     6975 2024-05-27 13:03:31.000000 digitalhub_data-0.5.0b4/digitalhub_data/entities/dataitems/entity/_base.py
--rw-rw-r--   0 mmartini  (1000) mmartini  (1000)      180 2024-03-15 13:13:54.000000 digitalhub_data-0.5.0b4/digitalhub_data/entities/dataitems/entity/dataitem.py
--rw-rw-r--   0 mmartini  (1000) mmartini  (1000)      142 2024-03-04 15:16:25.000000 digitalhub_data-0.5.0b4/digitalhub_data/entities/dataitems/entity/iceberg.py
--rw-rw-r--   0 mmartini  (1000) mmartini  (1000)     2958 2024-05-27 13:03:31.000000 digitalhub_data-0.5.0b4/digitalhub_data/entities/dataitems/entity/table.py
--rw-rw-r--   0 mmartini  (1000) mmartini  (1000)      582 2024-04-23 09:36:04.000000 digitalhub_data-0.5.0b4/digitalhub_data/entities/dataitems/metadata.py
--rw-rw-r--   0 mmartini  (1000) mmartini  (1000)     1093 2024-04-08 13:12:06.000000 digitalhub_data-0.5.0b4/digitalhub_data/entities/dataitems/models.py
--rw-rw-r--   0 mmartini  (1000) mmartini  (1000)     1418 2024-04-08 13:12:04.000000 digitalhub_data-0.5.0b4/digitalhub_data/entities/dataitems/spec.py
--rw-rw-r--   0 mmartini  (1000) mmartini  (1000)      863 2024-03-15 12:04:24.000000 digitalhub_data-0.5.0b4/digitalhub_data/entities/dataitems/status.py
--rw-rw-r--   0 mmartini  (1000) mmartini  (1000)      415 2024-05-06 11:22:14.000000 digitalhub_data-0.5.0b4/digitalhub_data/entities/entity_types.py
-drwxrwxr-x   0 mmartini  (1000) mmartini  (1000)        0 2024-05-27 13:53:47.558883 digitalhub_data-0.5.0b4/digitalhub_data/entities/projects/
--rw-rw-r--   0 mmartini  (1000) mmartini  (1000)        0 2024-01-31 10:03:33.000000 digitalhub_data-0.5.0b4/digitalhub_data/entities/projects/__init__.py
--rw-rw-r--   0 mmartini  (1000) mmartini  (1000)     6053 2024-05-27 13:03:31.000000 digitalhub_data-0.5.0b4/digitalhub_data/entities/projects/crud.py
--rw-rw-r--   0 mmartini  (1000) mmartini  (1000)     6000 2024-05-27 13:03:31.000000 digitalhub_data-0.5.0b4/digitalhub_data/entities/projects/entity.py
--rw-rw-r--   0 mmartini  (1000) mmartini  (1000)      950 2024-02-15 10:15:41.000000 digitalhub_data-0.5.0b4/digitalhub_data/entities/projects/spec.py
--rw-rw-r--   0 mmartini  (1000) mmartini  (1000)      773 2024-05-06 11:19:40.000000 digitalhub_data-0.5.0b4/digitalhub_data/entities/registries.py
-drwxrwxr-x   0 mmartini  (1000) mmartini  (1000)        0 2024-05-27 13:53:47.558883 digitalhub_data-0.5.0b4/digitalhub_data/entities/runs/
--rw-rw-r--   0 mmartini  (1000) mmartini  (1000)        0 2024-01-22 14:51:32.000000 digitalhub_data-0.5.0b4/digitalhub_data/entities/runs/__init__.py
--rw-rw-r--   0 mmartini  (1000) mmartini  (1000)      300 2024-03-07 13:39:55.000000 digitalhub_data-0.5.0b4/digitalhub_data/entities/runs/models.py
--rw-rw-r--   0 mmartini  (1000) mmartini  (1000)      407 2024-03-08 13:54:39.000000 digitalhub_data-0.5.0b4/digitalhub_data/entities/runs/spec.py
--rw-rw-r--   0 mmartini  (1000) mmartini  (1000)      351 2024-03-14 13:46:16.000000 digitalhub_data-0.5.0b4/digitalhub_data/entities/runs/status.py
-drwxrwxr-x   0 mmartini  (1000) mmartini  (1000)        0 2024-05-27 13:53:47.558883 digitalhub_data-0.5.0b4/digitalhub_data/readers/
--rw-rw-r--   0 mmartini  (1000) mmartini  (1000)        0 2024-05-21 09:54:41.000000 digitalhub_data-0.5.0b4/digitalhub_data/readers/__init__.py
--rw-rw-r--   0 mmartini  (1000) mmartini  (1000)     1148 2024-05-21 12:30:09.000000 digitalhub_data-0.5.0b4/digitalhub_data/readers/builder.py
-drwxrwxr-x   0 mmartini  (1000) mmartini  (1000)        0 2024-05-27 13:53:47.558883 digitalhub_data-0.5.0b4/digitalhub_data/readers/objects/
--rw-rw-r--   0 mmartini  (1000) mmartini  (1000)        0 2024-05-21 10:51:19.000000 digitalhub_data-0.5.0b4/digitalhub_data/readers/objects/__init__.py
--rw-rw-r--   0 mmartini  (1000) mmartini  (1000)      667 2024-05-21 13:09:30.000000 digitalhub_data-0.5.0b4/digitalhub_data/readers/objects/base.py
--rw-rw-r--   0 mmartini  (1000) mmartini  (1000)     1902 2024-05-21 13:14:39.000000 digitalhub_data-0.5.0b4/digitalhub_data/readers/objects/pandas.py
--rw-rw-r--   0 mmartini  (1000) mmartini  (1000)      358 2024-05-23 13:24:44.000000 digitalhub_data-0.5.0b4/digitalhub_data/readers/registry.py
-drwxrwxr-x   0 mmartini  (1000) mmartini  (1000)        0 2024-05-27 13:53:47.562883 digitalhub_data-0.5.0b4/digitalhub_data/utils/
--rw-rw-r--   0 mmartini  (1000) mmartini  (1000)        0 2024-01-29 10:07:05.000000 digitalhub_data-0.5.0b4/digitalhub_data/utils/__init__.py
--rw-rw-r--   0 mmartini  (1000) mmartini  (1000)     2440 2024-02-05 09:25:21.000000 digitalhub_data-0.5.0b4/digitalhub_data/utils/data_utils.py
-drwxrwxr-x   0 mmartini  (1000) mmartini  (1000)        0 2024-05-27 13:53:47.562883 digitalhub_data-0.5.0b4/digitalhub_data.egg-info/
--rw-r--r--   0 mmartini  (1000) mmartini  (1000)     1024 2024-05-27 13:53:47.000000 digitalhub_data-0.5.0b4/digitalhub_data.egg-info/PKG-INFO
--rw-rw-r--   0 mmartini  (1000) mmartini  (1000)     1918 2024-05-27 13:53:47.000000 digitalhub_data-0.5.0b4/digitalhub_data.egg-info/SOURCES.txt
--rw-rw-r--   0 mmartini  (1000) mmartini  (1000)        1 2024-05-27 13:53:47.000000 digitalhub_data-0.5.0b4/digitalhub_data.egg-info/dependency_links.txt
--rw-rw-r--   0 mmartini  (1000) mmartini  (1000)       52 2024-05-27 13:53:47.000000 digitalhub_data-0.5.0b4/digitalhub_data.egg-info/requires.txt
--rw-rw-r--   0 mmartini  (1000) mmartini  (1000)       21 2024-05-27 13:53:47.000000 digitalhub_data-0.5.0b4/digitalhub_data.egg-info/top_level.txt
--rw-rw-r--   0 mmartini  (1000) mmartini  (1000)     1130 2024-05-27 12:34:24.000000 digitalhub_data-0.5.0b4/pyproject.toml
--rw-rw-r--   0 mmartini  (1000) mmartini  (1000)       38 2024-05-27 13:53:47.562883 digitalhub_data-0.5.0b4/setup.cfg
+drwxrwxr-x   0 mmartini  (1000) mmartini  (1000)        0 2024-05-29 09:48:12.237434 digitalhub_data-0.5.0b5/
+-rw-r--r--   0 mmartini  (1000) mmartini  (1000)     1028 2024-05-29 09:48:12.237434 digitalhub_data-0.5.0b5/PKG-INFO
+-rw-rw-r--   0 mmartini  (1000) mmartini  (1000)      468 2024-04-23 09:36:04.000000 digitalhub_data-0.5.0b5/README.md
+drwxrwxr-x   0 mmartini  (1000) mmartini  (1000)        0 2024-05-29 09:48:12.229434 digitalhub_data-0.5.0b5/digitalhub_data/
+-rw-rw-r--   0 mmartini  (1000) mmartini  (1000)      329 2024-05-27 14:03:58.000000 digitalhub_data-0.5.0b5/digitalhub_data/__init__.py
+drwxrwxr-x   0 mmartini  (1000) mmartini  (1000)        0 2024-05-29 09:48:12.229434 digitalhub_data-0.5.0b5/digitalhub_data/datastores/
+-rw-rw-r--   0 mmartini  (1000) mmartini  (1000)        0 2024-05-21 09:37:15.000000 digitalhub_data-0.5.0b5/digitalhub_data/datastores/__init__.py
+-rw-rw-r--   0 mmartini  (1000) mmartini  (1000)     3209 2024-05-23 09:43:05.000000 digitalhub_data-0.5.0b5/digitalhub_data/datastores/builder.py
+drwxrwxr-x   0 mmartini  (1000) mmartini  (1000)        0 2024-05-29 09:48:12.233434 digitalhub_data-0.5.0b5/digitalhub_data/datastores/objects/
+-rw-rw-r--   0 mmartini  (1000) mmartini  (1000)        0 2024-05-21 09:37:57.000000 digitalhub_data-0.5.0b5/digitalhub_data/datastores/objects/__init__.py
+-rw-rw-r--   0 mmartini  (1000) mmartini  (1000)     3443 2024-05-22 13:22:43.000000 digitalhub_data-0.5.0b5/digitalhub_data/datastores/objects/base.py
+-rw-rw-r--   0 mmartini  (1000) mmartini  (1000)     1350 2024-05-23 09:43:30.000000 digitalhub_data-0.5.0b5/digitalhub_data/datastores/objects/local.py
+-rw-rw-r--   0 mmartini  (1000) mmartini  (1000)      667 2024-05-23 09:43:30.000000 digitalhub_data-0.5.0b5/digitalhub_data/datastores/objects/remote.py
+-rw-rw-r--   0 mmartini  (1000) mmartini  (1000)     1202 2024-05-23 09:43:30.000000 digitalhub_data-0.5.0b5/digitalhub_data/datastores/objects/s3.py
+-rw-rw-r--   0 mmartini  (1000) mmartini  (1000)     1863 2024-05-23 09:43:30.000000 digitalhub_data-0.5.0b5/digitalhub_data/datastores/objects/sql.py
+drwxrwxr-x   0 mmartini  (1000) mmartini  (1000)        0 2024-05-29 09:48:12.233434 digitalhub_data-0.5.0b5/digitalhub_data/entities/
+-rw-rw-r--   0 mmartini  (1000) mmartini  (1000)        0 2024-01-30 10:40:56.000000 digitalhub_data-0.5.0b5/digitalhub_data/entities/__init__.py
+drwxrwxr-x   0 mmartini  (1000) mmartini  (1000)        0 2024-05-29 09:48:12.233434 digitalhub_data-0.5.0b5/digitalhub_data/entities/dataitems/
+-rw-rw-r--   0 mmartini  (1000) mmartini  (1000)        0 2024-01-30 10:40:45.000000 digitalhub_data-0.5.0b5/digitalhub_data/entities/dataitems/__init__.py
+-rw-rw-r--   0 mmartini  (1000) mmartini  (1000)     3322 2024-05-27 14:03:58.000000 digitalhub_data-0.5.0b5/digitalhub_data/entities/dataitems/builder.py
+-rw-rw-r--   0 mmartini  (1000) mmartini  (1000)     6484 2024-05-27 14:03:58.000000 digitalhub_data-0.5.0b5/digitalhub_data/entities/dataitems/crud.py
+drwxrwxr-x   0 mmartini  (1000) mmartini  (1000)        0 2024-05-29 09:48:12.233434 digitalhub_data-0.5.0b5/digitalhub_data/entities/dataitems/entity/
+-rw-rw-r--   0 mmartini  (1000) mmartini  (1000)        0 2024-03-04 14:42:21.000000 digitalhub_data-0.5.0b5/digitalhub_data/entities/dataitems/entity/__init__.py
+-rw-rw-r--   0 mmartini  (1000) mmartini  (1000)     6975 2024-05-27 14:03:58.000000 digitalhub_data-0.5.0b5/digitalhub_data/entities/dataitems/entity/_base.py
+-rw-rw-r--   0 mmartini  (1000) mmartini  (1000)      180 2024-03-15 13:13:54.000000 digitalhub_data-0.5.0b5/digitalhub_data/entities/dataitems/entity/dataitem.py
+-rw-rw-r--   0 mmartini  (1000) mmartini  (1000)      142 2024-03-04 15:16:25.000000 digitalhub_data-0.5.0b5/digitalhub_data/entities/dataitems/entity/iceberg.py
+-rw-rw-r--   0 mmartini  (1000) mmartini  (1000)     2958 2024-05-27 14:03:58.000000 digitalhub_data-0.5.0b5/digitalhub_data/entities/dataitems/entity/table.py
+-rw-rw-r--   0 mmartini  (1000) mmartini  (1000)      582 2024-04-23 09:36:04.000000 digitalhub_data-0.5.0b5/digitalhub_data/entities/dataitems/metadata.py
+-rw-rw-r--   0 mmartini  (1000) mmartini  (1000)     1093 2024-04-08 13:12:06.000000 digitalhub_data-0.5.0b5/digitalhub_data/entities/dataitems/models.py
+-rw-rw-r--   0 mmartini  (1000) mmartini  (1000)     1418 2024-04-08 13:12:04.000000 digitalhub_data-0.5.0b5/digitalhub_data/entities/dataitems/spec.py
+-rw-rw-r--   0 mmartini  (1000) mmartini  (1000)      863 2024-03-15 12:04:24.000000 digitalhub_data-0.5.0b5/digitalhub_data/entities/dataitems/status.py
+-rw-rw-r--   0 mmartini  (1000) mmartini  (1000)      415 2024-05-06 11:22:14.000000 digitalhub_data-0.5.0b5/digitalhub_data/entities/entity_types.py
+drwxrwxr-x   0 mmartini  (1000) mmartini  (1000)        0 2024-05-29 09:48:12.237434 digitalhub_data-0.5.0b5/digitalhub_data/entities/projects/
+-rw-rw-r--   0 mmartini  (1000) mmartini  (1000)        0 2024-01-31 10:03:33.000000 digitalhub_data-0.5.0b5/digitalhub_data/entities/projects/__init__.py
+-rw-rw-r--   0 mmartini  (1000) mmartini  (1000)     6053 2024-05-27 14:03:58.000000 digitalhub_data-0.5.0b5/digitalhub_data/entities/projects/crud.py
+-rw-rw-r--   0 mmartini  (1000) mmartini  (1000)     6000 2024-05-27 14:03:58.000000 digitalhub_data-0.5.0b5/digitalhub_data/entities/projects/entity.py
+-rw-rw-r--   0 mmartini  (1000) mmartini  (1000)      950 2024-02-15 10:15:41.000000 digitalhub_data-0.5.0b5/digitalhub_data/entities/projects/spec.py
+-rw-rw-r--   0 mmartini  (1000) mmartini  (1000)      773 2024-05-06 11:19:40.000000 digitalhub_data-0.5.0b5/digitalhub_data/entities/registries.py
+drwxrwxr-x   0 mmartini  (1000) mmartini  (1000)        0 2024-05-29 09:48:12.237434 digitalhub_data-0.5.0b5/digitalhub_data/entities/runs/
+-rw-rw-r--   0 mmartini  (1000) mmartini  (1000)        0 2024-01-22 14:51:32.000000 digitalhub_data-0.5.0b5/digitalhub_data/entities/runs/__init__.py
+-rw-rw-r--   0 mmartini  (1000) mmartini  (1000)      300 2024-03-07 13:39:55.000000 digitalhub_data-0.5.0b5/digitalhub_data/entities/runs/models.py
+-rw-rw-r--   0 mmartini  (1000) mmartini  (1000)      407 2024-03-08 13:54:39.000000 digitalhub_data-0.5.0b5/digitalhub_data/entities/runs/spec.py
+-rw-rw-r--   0 mmartini  (1000) mmartini  (1000)      351 2024-03-14 13:46:16.000000 digitalhub_data-0.5.0b5/digitalhub_data/entities/runs/status.py
+drwxrwxr-x   0 mmartini  (1000) mmartini  (1000)        0 2024-05-29 09:48:12.237434 digitalhub_data-0.5.0b5/digitalhub_data/readers/
+-rw-rw-r--   0 mmartini  (1000) mmartini  (1000)        0 2024-05-21 09:54:41.000000 digitalhub_data-0.5.0b5/digitalhub_data/readers/__init__.py
+-rw-rw-r--   0 mmartini  (1000) mmartini  (1000)     1148 2024-05-21 12:30:09.000000 digitalhub_data-0.5.0b5/digitalhub_data/readers/builder.py
+drwxrwxr-x   0 mmartini  (1000) mmartini  (1000)        0 2024-05-29 09:48:12.237434 digitalhub_data-0.5.0b5/digitalhub_data/readers/objects/
+-rw-rw-r--   0 mmartini  (1000) mmartini  (1000)        0 2024-05-21 10:51:19.000000 digitalhub_data-0.5.0b5/digitalhub_data/readers/objects/__init__.py
+-rw-rw-r--   0 mmartini  (1000) mmartini  (1000)      667 2024-05-21 13:09:30.000000 digitalhub_data-0.5.0b5/digitalhub_data/readers/objects/base.py
+-rw-rw-r--   0 mmartini  (1000) mmartini  (1000)     1902 2024-05-21 13:14:39.000000 digitalhub_data-0.5.0b5/digitalhub_data/readers/objects/pandas.py
+-rw-rw-r--   0 mmartini  (1000) mmartini  (1000)      358 2024-05-23 13:24:44.000000 digitalhub_data-0.5.0b5/digitalhub_data/readers/registry.py
+drwxrwxr-x   0 mmartini  (1000) mmartini  (1000)        0 2024-05-29 09:48:12.237434 digitalhub_data-0.5.0b5/digitalhub_data/utils/
+-rw-rw-r--   0 mmartini  (1000) mmartini  (1000)        0 2024-01-29 10:07:05.000000 digitalhub_data-0.5.0b5/digitalhub_data/utils/__init__.py
+-rw-rw-r--   0 mmartini  (1000) mmartini  (1000)     2440 2024-02-05 09:25:21.000000 digitalhub_data-0.5.0b5/digitalhub_data/utils/data_utils.py
+drwxrwxr-x   0 mmartini  (1000) mmartini  (1000)        0 2024-05-29 09:48:12.237434 digitalhub_data-0.5.0b5/digitalhub_data.egg-info/
+-rw-r--r--   0 mmartini  (1000) mmartini  (1000)     1028 2024-05-29 09:48:12.000000 digitalhub_data-0.5.0b5/digitalhub_data.egg-info/PKG-INFO
+-rw-rw-r--   0 mmartini  (1000) mmartini  (1000)     1918 2024-05-29 09:48:12.000000 digitalhub_data-0.5.0b5/digitalhub_data.egg-info/SOURCES.txt
+-rw-rw-r--   0 mmartini  (1000) mmartini  (1000)        1 2024-05-29 09:48:12.000000 digitalhub_data-0.5.0b5/digitalhub_data.egg-info/dependency_links.txt
+-rw-rw-r--   0 mmartini  (1000) mmartini  (1000)       56 2024-05-29 09:48:12.000000 digitalhub_data-0.5.0b5/digitalhub_data.egg-info/requires.txt
+-rw-rw-r--   0 mmartini  (1000) mmartini  (1000)       21 2024-05-29 09:48:12.000000 digitalhub_data-0.5.0b5/digitalhub_data.egg-info/top_level.txt
+-rw-rw-r--   0 mmartini  (1000) mmartini  (1000)     1135 2024-05-28 11:34:48.000000 digitalhub_data-0.5.0b5/pyproject.toml
+-rw-rw-r--   0 mmartini  (1000) mmartini  (1000)       38 2024-05-29 09:48:12.237434 digitalhub_data-0.5.0b5/setup.cfg
```

### Comparing `digitalhub_data-0.5.0b4/PKG-INFO` & `digitalhub_data-0.5.0b5/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,19 +1,19 @@
 Metadata-Version: 2.1
 Name: digitalhub-data
-Version: 0.5.0b4
+Version: 0.5.0b5
 Summary: Python SDK for DHCore
 Author-email: Fondazione Bruno Kessler <dslab@fbk.eu>, Matteo Martini <mmartini@fbk.eu>
 Keywords: data,dataops,kubernetes
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Requires-Python: >=3.9
 Description-Content-Type: text/markdown
-Requires-Dist: digitalhub-core==0.5.0b4
+Requires-Dist: digitalhub-core<0.6,~=0.5.0b
 Provides-Extra: pandas
 Requires-Dist: pandas<2.2,>=1.2; extra == "pandas"
 
 # Digitalhub-data Library
 
 The Digitalhub-data SDK library is used to manage entities and executions in Digitalhub from Python.
 The Digitalhub-data layer is the second layer of the Digitalhub Data platform, focused on operations on data.
```

### Comparing `digitalhub_data-0.5.0b4/digitalhub_data/datastores/builder.py` & `digitalhub_data-0.5.0b5/digitalhub_data/datastores/builder.py`

 * *Files identical despite different names*

### Comparing `digitalhub_data-0.5.0b4/digitalhub_data/datastores/objects/base.py` & `digitalhub_data-0.5.0b5/digitalhub_data/datastores/objects/base.py`

 * *Files identical despite different names*

### Comparing `digitalhub_data-0.5.0b4/digitalhub_data/datastores/objects/local.py` & `digitalhub_data-0.5.0b5/digitalhub_data/datastores/objects/local.py`

 * *Files identical despite different names*

### Comparing `digitalhub_data-0.5.0b4/digitalhub_data/datastores/objects/remote.py` & `digitalhub_data-0.5.0b5/digitalhub_data/datastores/objects/remote.py`

 * *Files identical despite different names*

### Comparing `digitalhub_data-0.5.0b4/digitalhub_data/datastores/objects/s3.py` & `digitalhub_data-0.5.0b5/digitalhub_data/datastores/objects/s3.py`

 * *Files identical despite different names*

### Comparing `digitalhub_data-0.5.0b4/digitalhub_data/datastores/objects/sql.py` & `digitalhub_data-0.5.0b5/digitalhub_data/datastores/objects/sql.py`

 * *Files identical despite different names*

### Comparing `digitalhub_data-0.5.0b4/digitalhub_data/entities/dataitems/builder.py` & `digitalhub_data-0.5.0b5/digitalhub_data/entities/dataitems/builder.py`

 * *Files identical despite different names*

### Comparing `digitalhub_data-0.5.0b4/digitalhub_data/entities/dataitems/crud.py` & `digitalhub_data-0.5.0b5/digitalhub_data/entities/dataitems/crud.py`

 * *Files identical despite different names*

### Comparing `digitalhub_data-0.5.0b4/digitalhub_data/entities/dataitems/entity/_base.py` & `digitalhub_data-0.5.0b5/digitalhub_data/entities/dataitems/entity/_base.py`

 * *Files identical despite different names*

### Comparing `digitalhub_data-0.5.0b4/digitalhub_data/entities/dataitems/entity/table.py` & `digitalhub_data-0.5.0b5/digitalhub_data/entities/dataitems/entity/table.py`

 * *Files identical despite different names*

### Comparing `digitalhub_data-0.5.0b4/digitalhub_data/entities/dataitems/metadata.py` & `digitalhub_data-0.5.0b5/digitalhub_data/entities/dataitems/metadata.py`

 * *Files identical despite different names*

### Comparing `digitalhub_data-0.5.0b4/digitalhub_data/entities/dataitems/models.py` & `digitalhub_data-0.5.0b5/digitalhub_data/entities/dataitems/models.py`

 * *Files identical despite different names*

### Comparing `digitalhub_data-0.5.0b4/digitalhub_data/entities/dataitems/spec.py` & `digitalhub_data-0.5.0b5/digitalhub_data/entities/dataitems/spec.py`

 * *Files identical despite different names*

### Comparing `digitalhub_data-0.5.0b4/digitalhub_data/entities/dataitems/status.py` & `digitalhub_data-0.5.0b5/digitalhub_data/entities/dataitems/status.py`

 * *Files identical despite different names*

### Comparing `digitalhub_data-0.5.0b4/digitalhub_data/entities/projects/crud.py` & `digitalhub_data-0.5.0b5/digitalhub_data/entities/projects/crud.py`

 * *Files identical despite different names*

### Comparing `digitalhub_data-0.5.0b4/digitalhub_data/entities/projects/entity.py` & `digitalhub_data-0.5.0b5/digitalhub_data/entities/projects/entity.py`

 * *Files identical despite different names*

### Comparing `digitalhub_data-0.5.0b4/digitalhub_data/entities/projects/spec.py` & `digitalhub_data-0.5.0b5/digitalhub_data/entities/projects/spec.py`

 * *Files identical despite different names*

### Comparing `digitalhub_data-0.5.0b4/digitalhub_data/entities/registries.py` & `digitalhub_data-0.5.0b5/digitalhub_data/entities/registries.py`

 * *Files identical despite different names*

### Comparing `digitalhub_data-0.5.0b4/digitalhub_data/readers/builder.py` & `digitalhub_data-0.5.0b5/digitalhub_data/readers/builder.py`

 * *Files identical despite different names*

### Comparing `digitalhub_data-0.5.0b4/digitalhub_data/readers/objects/base.py` & `digitalhub_data-0.5.0b5/digitalhub_data/readers/objects/base.py`

 * *Files identical despite different names*

### Comparing `digitalhub_data-0.5.0b4/digitalhub_data/readers/objects/pandas.py` & `digitalhub_data-0.5.0b5/digitalhub_data/readers/objects/pandas.py`

 * *Files identical despite different names*

### Comparing `digitalhub_data-0.5.0b4/digitalhub_data/utils/data_utils.py` & `digitalhub_data-0.5.0b5/digitalhub_data/utils/data_utils.py`

 * *Files identical despite different names*

### Comparing `digitalhub_data-0.5.0b4/digitalhub_data.egg-info/PKG-INFO` & `digitalhub_data-0.5.0b5/digitalhub_data.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,19 +1,19 @@
 Metadata-Version: 2.1
 Name: digitalhub-data
-Version: 0.5.0b4
+Version: 0.5.0b5
 Summary: Python SDK for DHCore
 Author-email: Fondazione Bruno Kessler <dslab@fbk.eu>, Matteo Martini <mmartini@fbk.eu>
 Keywords: data,dataops,kubernetes
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Requires-Python: >=3.9
 Description-Content-Type: text/markdown
-Requires-Dist: digitalhub-core==0.5.0b4
+Requires-Dist: digitalhub-core<0.6,~=0.5.0b
 Provides-Extra: pandas
 Requires-Dist: pandas<2.2,>=1.2; extra == "pandas"
 
 # Digitalhub-data Library
 
 The Digitalhub-data SDK library is used to manage entities and executions in Digitalhub from Python.
 The Digitalhub-data layer is the second layer of the Digitalhub Data platform, focused on operations on data.
```

### Comparing `digitalhub_data-0.5.0b4/digitalhub_data.egg-info/SOURCES.txt` & `digitalhub_data-0.5.0b5/digitalhub_data.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `digitalhub_data-0.5.0b4/pyproject.toml` & `digitalhub_data-0.5.0b5/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["setuptools", "wheel"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "digitalhub-data"
-version = "0.5.0b4"
+version = "0.5.0b5"
 description = "Python SDK for DHCore"
 readme = "README.md"
 authors = [
     { name = "Fondazione Bruno Kessler", email = "dslab@fbk.eu" },
     { name = "Matteo Martini", email = "mmartini@fbk.eu" }
 ]
 license = { file = "LICENSE.txt" }
@@ -16,26 +16,26 @@
     "License :: OSI Approved :: Apache Software License",
     "Programming Language :: Python :: 3.9",
     "Programming Language :: Python :: 3.10"
 ]
 keywords = ["data", "dataops", "kubernetes"]
 requires-python = ">=3.9"
 dependencies = [
-    "digitalhub-core==0.5.0b4",
+    "digitalhub-core~=0.5.0b, <0.6",
 ]
 [project.optional-dependencies]
 pandas = [
     "pandas>=1.2, <2.2",
 ]
 
 [tool.setuptools.packages.find]
 exclude = ["modules*"]
 
 [tool.bumpver]
-current_version = "0.5.0b4"
+current_version = "0.5.0b5"
 version_pattern = "MAJOR.MINOR.PATCH[PYTAGNUM]"
 commit_message  = "Bump version {old_version} -> {new_version}"
 commit          = false
 tag             = false
 push            = false
 
 [tool.bumpver.file_patterns]
```

