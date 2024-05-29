# Comparing `tmp/dbt-databricks-1.8.1b2.tar.gz` & `tmp/dbt-databricks-2.0.0rc1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dbt-databricks-1.8.1b2.tar", last modified: Thu May 23 20:32:00 2024, max compression
+gzip compressed data, was "dbt-databricks-2.0.0rc1.tar", last modified: Wed May  8 19:39:36 2024, max compression
```

## Comparing `dbt-databricks-1.8.1b2.tar` & `dbt-databricks-2.0.0rc1.tar`

### file list

```diff
@@ -1,112 +1,112 @@
-drwxr-xr-x   0 ben.cassell   (502) staff       (20)        0 2024-05-23 20:32:00.150573 dbt-databricks-1.8.1b2/
--rw-r--r--   0 ben.cassell   (502) staff       (20)       47 2024-05-21 22:25:06.000000 dbt-databricks-1.8.1b2/MANIFEST.in
--rw-r--r--   0 ben.cassell   (502) staff       (20)     5378 2024-05-23 20:32:00.150366 dbt-databricks-1.8.1b2/PKG-INFO
--rw-r--r--   0 ben.cassell   (502) staff       (20)     4624 2024-01-19 01:37:59.000000 dbt-databricks-1.8.1b2/README.md
-drwxr-xr-x   0 ben.cassell   (502) staff       (20)        0 2024-05-23 20:32:00.105805 dbt-databricks-1.8.1b2/dbt/
--rw-r--r--   0 ben.cassell   (502) staff       (20)       76 2024-01-25 18:09:59.000000 dbt-databricks-1.8.1b2/dbt/__init__.py
-drwxr-xr-x   0 ben.cassell   (502) staff       (20)        0 2024-05-23 20:32:00.100672 dbt-databricks-1.8.1b2/dbt/adapters/
-drwxr-xr-x   0 ben.cassell   (502) staff       (20)        0 2024-05-23 20:32:00.109610 dbt-databricks-1.8.1b2/dbt/adapters/databricks/
--rw-r--r--   0 ben.cassell   (502) staff       (20)      625 2024-05-21 22:25:06.000000 dbt-databricks-1.8.1b2/dbt/adapters/databricks/__init__.py
--rw-r--r--   0 ben.cassell   (502) staff       (20)       25 2024-05-23 20:31:34.000000 dbt-databricks-1.8.1b2/dbt/adapters/databricks/__version__.py
--rw-r--r--   0 ben.cassell   (502) staff       (20)     3513 2024-05-21 22:25:06.000000 dbt-databricks-1.8.1b2/dbt/adapters/databricks/auth.py
--rw-r--r--   0 ben.cassell   (502) staff       (20)      707 2024-05-21 22:25:06.000000 dbt-databricks-1.8.1b2/dbt/adapters/databricks/column.py
--rw-r--r--   0 ben.cassell   (502) staff       (20)    46828 2024-05-23 20:25:14.000000 dbt-databricks-1.8.1b2/dbt/adapters/databricks/connections.py
--rw-r--r--   0 ben.cassell   (502) staff       (20)    15743 2024-05-21 22:25:06.000000 dbt-databricks-1.8.1b2/dbt/adapters/databricks/credentials.py
-drwxr-xr-x   0 ben.cassell   (502) staff       (20)        0 2024-05-23 20:32:00.111695 dbt-databricks-1.8.1b2/dbt/adapters/databricks/events/
--rw-r--r--   0 ben.cassell   (502) staff       (20)      796 2024-05-10 19:26:33.000000 dbt-databricks-1.8.1b2/dbt/adapters/databricks/events/base.py
--rw-r--r--   0 ben.cassell   (502) staff       (20)     3956 2024-05-22 17:36:31.000000 dbt-databricks-1.8.1b2/dbt/adapters/databricks/events/connection_events.py
--rw-r--r--   0 ben.cassell   (502) staff       (20)      616 2024-05-10 19:26:33.000000 dbt-databricks-1.8.1b2/dbt/adapters/databricks/events/credential_events.py
--rw-r--r--   0 ben.cassell   (502) staff       (20)     1826 2024-05-10 19:26:33.000000 dbt-databricks-1.8.1b2/dbt/adapters/databricks/events/cursor_events.py
--rw-r--r--   0 ben.cassell   (502) staff       (20)      250 2024-05-10 19:26:33.000000 dbt-databricks-1.8.1b2/dbt/adapters/databricks/events/other_events.py
--rw-r--r--   0 ben.cassell   (502) staff       (20)      785 2024-05-23 20:25:14.000000 dbt-databricks-1.8.1b2/dbt/adapters/databricks/events/pipeline_events.py
--rw-r--r--   0 ben.cassell   (502) staff       (20)    32121 2024-05-23 20:31:45.000000 dbt-databricks-1.8.1b2/dbt/adapters/databricks/impl.py
--rw-r--r--   0 ben.cassell   (502) staff       (20)      995 2024-05-21 22:25:06.000000 dbt-databricks-1.8.1b2/dbt/adapters/databricks/logging.py
--rw-r--r--   0 ben.cassell   (502) staff       (20)    19165 2024-05-21 22:25:06.000000 dbt-databricks-1.8.1b2/dbt/adapters/databricks/python_submissions.py
--rw-r--r--   0 ben.cassell   (502) staff       (20)     5311 2024-05-23 20:25:14.000000 dbt-databricks-1.8.1b2/dbt/adapters/databricks/relation.py
-drwxr-xr-x   0 ben.cassell   (502) staff       (20)        0 2024-05-23 20:32:00.115100 dbt-databricks-1.8.1b2/dbt/adapters/databricks/relation_configs/
--rw-r--r--   0 ben.cassell   (502) staff       (20)     6157 2024-05-23 17:32:12.000000 dbt-databricks-1.8.1b2/dbt/adapters/databricks/relation_configs/base.py
--rw-r--r--   0 ben.cassell   (502) staff       (20)     1268 2024-05-23 20:25:14.000000 dbt-databricks-1.8.1b2/dbt/adapters/databricks/relation_configs/comment.py
--rw-r--r--   0 ben.cassell   (502) staff       (20)     1040 2024-05-21 22:25:06.000000 dbt-databricks-1.8.1b2/dbt/adapters/databricks/relation_configs/incremental.py
--rw-r--r--   0 ben.cassell   (502) staff       (20)     1700 2024-05-23 17:32:12.000000 dbt-databricks-1.8.1b2/dbt/adapters/databricks/relation_configs/materialized_view.py
--rw-r--r--   0 ben.cassell   (502) staff       (20)     1699 2024-05-23 17:32:12.000000 dbt-databricks-1.8.1b2/dbt/adapters/databricks/relation_configs/partitioning.py
--rw-r--r--   0 ben.cassell   (502) staff       (20)     1182 2024-05-23 17:32:12.000000 dbt-databricks-1.8.1b2/dbt/adapters/databricks/relation_configs/query.py
--rw-r--r--   0 ben.cassell   (502) staff       (20)     2954 2024-05-23 20:25:14.000000 dbt-databricks-1.8.1b2/dbt/adapters/databricks/relation_configs/refresh.py
--rw-r--r--   0 ben.cassell   (502) staff       (20)     1802 2024-05-23 17:32:12.000000 dbt-databricks-1.8.1b2/dbt/adapters/databricks/relation_configs/streaming_table.py
--rw-r--r--   0 ben.cassell   (502) staff       (20)     1850 2024-05-21 22:25:06.000000 dbt-databricks-1.8.1b2/dbt/adapters/databricks/relation_configs/tags.py
--rw-r--r--   0 ben.cassell   (502) staff       (20)     2852 2024-05-23 20:25:14.000000 dbt-databricks-1.8.1b2/dbt/adapters/databricks/relation_configs/tblproperties.py
--rw-r--r--   0 ben.cassell   (502) staff       (20)     2637 2024-05-23 20:25:14.000000 dbt-databricks-1.8.1b2/dbt/adapters/databricks/utils.py
-drwxr-xr-x   0 ben.cassell   (502) staff       (20)        0 2024-05-23 20:32:00.101375 dbt-databricks-1.8.1b2/dbt/include/
-drwxr-xr-x   0 ben.cassell   (502) staff       (20)        0 2024-05-23 20:32:00.116767 dbt-databricks-1.8.1b2/dbt/include/databricks/
--rw-r--r--   0 ben.cassell   (502) staff       (20)       52 2023-05-30 21:40:46.000000 dbt-databricks-1.8.1b2/dbt/include/databricks/__init__.py
--rw-r--r--   0 ben.cassell   (502) staff       (20)       77 2023-05-30 21:40:46.000000 dbt-databricks-1.8.1b2/dbt/include/databricks/dbt_project.yml
-drwxr-xr-x   0 ben.cassell   (502) staff       (20)        0 2024-05-23 20:32:00.104065 dbt-databricks-1.8.1b2/dbt/include/databricks/macros/
-drwxr-xr-x   0 ben.cassell   (502) staff       (20)        0 2024-05-23 20:32:00.120517 dbt-databricks-1.8.1b2/dbt/include/databricks/macros/adapters/
--rw-r--r--   0 ben.cassell   (502) staff       (20)     3393 2024-05-23 20:25:14.000000 dbt-databricks-1.8.1b2/dbt/include/databricks/macros/adapters/catalog.sql
--rw-r--r--   0 ben.cassell   (502) staff       (20)     2409 2024-03-26 16:27:09.000000 dbt-databricks-1.8.1b2/dbt/include/databricks/macros/adapters/copy_into.sql
--rw-r--r--   0 ben.cassell   (502) staff       (20)      592 2024-05-21 22:25:06.000000 dbt-databricks-1.8.1b2/dbt/include/databricks/macros/adapters/databricks_catalog.sql
--rw-r--r--   0 ben.cassell   (502) staff       (20)     3958 2024-05-23 20:25:14.000000 dbt-databricks-1.8.1b2/dbt/include/databricks/macros/adapters/metadata.sql
--rw-r--r--   0 ben.cassell   (502) staff       (20)     1984 2024-05-21 22:25:06.000000 dbt-databricks-1.8.1b2/dbt/include/databricks/macros/adapters/persist_docs.sql
--rw-r--r--   0 ben.cassell   (502) staff       (20)     3861 2024-05-23 20:25:14.000000 dbt-databricks-1.8.1b2/dbt/include/databricks/macros/adapters/python.sql
--rw-r--r--   0 ben.cassell   (502) staff       (20)     1158 2024-05-21 22:25:06.000000 dbt-databricks-1.8.1b2/dbt/include/databricks/macros/adapters/relation.sql
-drwxr-xr-x   0 ben.cassell   (502) staff       (20)        0 2024-05-23 20:32:00.120916 dbt-databricks-1.8.1b2/dbt/include/databricks/macros/etc/
--rw-r--r--   0 ben.cassell   (502) staff       (20)      648 2024-03-26 16:27:09.000000 dbt-databricks-1.8.1b2/dbt/include/databricks/macros/etc/statement.sql
-drwxr-xr-x   0 ben.cassell   (502) staff       (20)        0 2024-05-23 20:32:00.121315 dbt-databricks-1.8.1b2/dbt/include/databricks/macros/get_custom_name/
--rw-r--r--   0 ben.cassell   (502) staff       (20)      458 2024-05-21 22:25:06.000000 dbt-databricks-1.8.1b2/dbt/include/databricks/macros/get_custom_name/get_custom_database.sql
-drwxr-xr-x   0 ben.cassell   (502) staff       (20)        0 2024-05-23 20:32:00.124619 dbt-databricks-1.8.1b2/dbt/include/databricks/macros/materializations/
--rw-r--r--   0 ben.cassell   (502) staff       (20)     2803 2024-05-21 22:25:06.000000 dbt-databricks-1.8.1b2/dbt/include/databricks/macros/materializations/clone.sql
-drwxr-xr-x   0 ben.cassell   (502) staff       (20)        0 2024-05-23 20:32:00.126334 dbt-databricks-1.8.1b2/dbt/include/databricks/macros/materializations/incremental/
--rw-r--r--   0 ben.cassell   (502) staff       (20)     4875 2024-05-21 22:25:06.000000 dbt-databricks-1.8.1b2/dbt/include/databricks/macros/materializations/incremental/incremental.sql
--rw-r--r--   0 ben.cassell   (502) staff       (20)     5522 2024-05-21 22:25:06.000000 dbt-databricks-1.8.1b2/dbt/include/databricks/macros/materializations/incremental/strategies.sql
--rw-r--r--   0 ben.cassell   (502) staff       (20)     1896 2024-05-21 22:25:06.000000 dbt-databricks-1.8.1b2/dbt/include/databricks/macros/materializations/incremental/validate.sql
--rw-r--r--   0 ben.cassell   (502) staff       (20)     3657 2024-05-23 17:32:12.000000 dbt-databricks-1.8.1b2/dbt/include/databricks/macros/materializations/materialized_view.sql
-drwxr-xr-x   0 ben.cassell   (502) staff       (20)        0 2024-05-23 20:32:00.127141 dbt-databricks-1.8.1b2/dbt/include/databricks/macros/materializations/seeds/
--rw-r--r--   0 ben.cassell   (502) staff       (20)     4183 2024-05-23 20:25:14.000000 dbt-databricks-1.8.1b2/dbt/include/databricks/macros/materializations/seeds/helpers.sql
--rw-r--r--   0 ben.cassell   (502) staff       (20)     2513 2024-05-23 20:25:14.000000 dbt-databricks-1.8.1b2/dbt/include/databricks/macros/materializations/seeds/seeds.sql
--rw-r--r--   0 ben.cassell   (502) staff       (20)     5397 2024-03-29 15:20:41.000000 dbt-databricks-1.8.1b2/dbt/include/databricks/macros/materializations/snapshot.sql
--rw-r--r--   0 ben.cassell   (502) staff       (20)     3623 2024-05-23 17:32:12.000000 dbt-databricks-1.8.1b2/dbt/include/databricks/macros/materializations/streaming_table.sql
--rw-r--r--   0 ben.cassell   (502) staff       (20)     1966 2024-05-21 22:25:06.000000 dbt-databricks-1.8.1b2/dbt/include/databricks/macros/materializations/table.sql
--rw-r--r--   0 ben.cassell   (502) staff       (20)     1364 2024-05-21 22:25:06.000000 dbt-databricks-1.8.1b2/dbt/include/databricks/macros/materializations/view.sql
-drwxr-xr-x   0 ben.cassell   (502) staff       (20)        0 2024-05-23 20:32:00.133102 dbt-databricks-1.8.1b2/dbt/include/databricks/macros/relations/
-drwxr-xr-x   0 ben.cassell   (502) staff       (20)        0 2024-05-23 20:32:00.141484 dbt-databricks-1.8.1b2/dbt/include/databricks/macros/relations/components/
--rw-r--r--   0 ben.cassell   (502) staff       (20)      131 2024-05-21 22:25:06.000000 dbt-databricks-1.8.1b2/dbt/include/databricks/macros/relations/components/comment.sql
--rw-r--r--   0 ben.cassell   (502) staff       (20)      217 2024-05-21 22:25:06.000000 dbt-databricks-1.8.1b2/dbt/include/databricks/macros/relations/components/partitioning.sql
--rw-r--r--   0 ben.cassell   (502) staff       (20)      670 2024-05-21 22:25:06.000000 dbt-databricks-1.8.1b2/dbt/include/databricks/macros/relations/components/refresh_schedule.sql
--rw-r--r--   0 ben.cassell   (502) staff       (20)      310 2024-05-21 22:25:06.000000 dbt-databricks-1.8.1b2/dbt/include/databricks/macros/relations/components/tblproperties.sql
--rw-r--r--   0 ben.cassell   (502) staff       (20)    10574 2024-05-21 22:25:06.000000 dbt-databricks-1.8.1b2/dbt/include/databricks/macros/relations/constraints.sql
--rw-r--r--   0 ben.cassell   (502) staff       (20)      629 2024-05-23 17:32:12.000000 dbt-databricks-1.8.1b2/dbt/include/databricks/macros/relations/create.sql
--rw-r--r--   0 ben.cassell   (502) staff       (20)      564 2024-05-21 22:25:06.000000 dbt-databricks-1.8.1b2/dbt/include/databricks/macros/relations/drop.sql
--rw-r--r--   0 ben.cassell   (502) staff       (20)      147 2024-05-21 22:25:06.000000 dbt-databricks-1.8.1b2/dbt/include/databricks/macros/relations/file_format.sql
--rw-r--r--   0 ben.cassell   (502) staff       (20)      615 2024-05-21 22:25:06.000000 dbt-databricks-1.8.1b2/dbt/include/databricks/macros/relations/location.sql
-drwxr-xr-x   0 ben.cassell   (502) staff       (20)        0 2024-05-23 20:32:00.143024 dbt-databricks-1.8.1b2/dbt/include/databricks/macros/relations/materialized_view/
--rw-r--r--   0 ben.cassell   (502) staff       (20)     1801 2024-05-23 17:32:12.000000 dbt-databricks-1.8.1b2/dbt/include/databricks/macros/relations/materialized_view/alter.sql
--rw-r--r--   0 ben.cassell   (502) staff       (20)      756 2024-05-21 22:25:06.000000 dbt-databricks-1.8.1b2/dbt/include/databricks/macros/relations/materialized_view/create.sql
--rw-r--r--   0 ben.cassell   (502) staff       (20)      126 2024-05-21 22:25:06.000000 dbt-databricks-1.8.1b2/dbt/include/databricks/macros/relations/materialized_view/drop.sql
--rw-r--r--   0 ben.cassell   (502) staff       (20)      119 2024-05-21 22:25:06.000000 dbt-databricks-1.8.1b2/dbt/include/databricks/macros/relations/materialized_view/refresh.sql
--rw-r--r--   0 ben.cassell   (502) staff       (20)     1372 2024-05-21 22:25:06.000000 dbt-databricks-1.8.1b2/dbt/include/databricks/macros/relations/optimize.sql
--rw-r--r--   0 ben.cassell   (502) staff       (20)     2273 2024-05-23 17:32:12.000000 dbt-databricks-1.8.1b2/dbt/include/databricks/macros/relations/replace.sql
-drwxr-xr-x   0 ben.cassell   (502) staff       (20)        0 2024-05-23 20:32:00.145365 dbt-databricks-1.8.1b2/dbt/include/databricks/macros/relations/streaming_table/
--rw-r--r--   0 ben.cassell   (502) staff       (20)     3212 2024-05-23 17:32:12.000000 dbt-databricks-1.8.1b2/dbt/include/databricks/macros/relations/streaming_table/alter.sql
--rw-r--r--   0 ben.cassell   (502) staff       (20)      904 2024-05-21 22:25:06.000000 dbt-databricks-1.8.1b2/dbt/include/databricks/macros/relations/streaming_table/create.sql
--rw-r--r--   0 ben.cassell   (502) staff       (20)      246 2024-05-21 22:25:06.000000 dbt-databricks-1.8.1b2/dbt/include/databricks/macros/relations/streaming_table/drop.sql
--rw-r--r--   0 ben.cassell   (502) staff       (20)      292 2024-05-21 22:25:06.000000 dbt-databricks-1.8.1b2/dbt/include/databricks/macros/relations/streaming_table/refresh.sql
-drwxr-xr-x   0 ben.cassell   (502) staff       (20)        0 2024-05-23 20:32:00.145949 dbt-databricks-1.8.1b2/dbt/include/databricks/macros/relations/table/
--rw-r--r--   0 ben.cassell   (502) staff       (20)     3161 2024-05-21 22:25:06.000000 dbt-databricks-1.8.1b2/dbt/include/databricks/macros/relations/table/create.sql
--rw-r--r--   0 ben.cassell   (502) staff       (20)      102 2024-05-21 22:25:06.000000 dbt-databricks-1.8.1b2/dbt/include/databricks/macros/relations/table/drop.sql
--rw-r--r--   0 ben.cassell   (502) staff       (20)     1604 2024-05-21 22:25:06.000000 dbt-databricks-1.8.1b2/dbt/include/databricks/macros/relations/tags.sql
--rw-r--r--   0 ben.cassell   (502) staff       (20)      764 2024-05-10 19:26:33.000000 dbt-databricks-1.8.1b2/dbt/include/databricks/macros/relations/tblproperties.sql
-drwxr-xr-x   0 ben.cassell   (502) staff       (20)        0 2024-05-23 20:32:00.146888 dbt-databricks-1.8.1b2/dbt/include/databricks/macros/relations/view/
--rw-r--r--   0 ben.cassell   (502) staff       (20)      643 2024-05-21 22:25:06.000000 dbt-databricks-1.8.1b2/dbt/include/databricks/macros/relations/view/create.sql
--rw-r--r--   0 ben.cassell   (502) staff       (20)      100 2024-05-21 22:25:06.000000 dbt-databricks-1.8.1b2/dbt/include/databricks/macros/relations/view/drop.sql
-drwxr-xr-x   0 ben.cassell   (502) staff       (20)        0 2024-05-23 20:32:00.147350 dbt-databricks-1.8.1b2/dbt/include/databricks/macros/utils/
--rw-r--r--   0 ben.cassell   (502) staff       (20)      318 2023-05-30 21:40:46.000000 dbt-databricks-1.8.1b2/dbt/include/databricks/macros/utils/dateadd.sql
--rw-r--r--   0 ben.cassell   (502) staff       (20)      338 2023-10-26 17:27:28.000000 dbt-databricks-1.8.1b2/dbt/include/databricks/macros/utils/datediff.sql
--rw-r--r--   0 ben.cassell   (502) staff       (20)      535 2023-05-30 21:40:46.000000 dbt-databricks-1.8.1b2/dbt/include/databricks/profile_template.yml
-drwxr-xr-x   0 ben.cassell   (502) staff       (20)        0 2024-05-23 20:32:00.149982 dbt-databricks-1.8.1b2/dbt_databricks.egg-info/
--rw-r--r--   0 ben.cassell   (502) staff       (20)     5378 2024-05-23 20:32:00.000000 dbt-databricks-1.8.1b2/dbt_databricks.egg-info/PKG-INFO
--rw-r--r--   0 ben.cassell   (502) staff       (20)     4441 2024-05-23 20:32:00.000000 dbt-databricks-1.8.1b2/dbt_databricks.egg-info/SOURCES.txt
--rw-r--r--   0 ben.cassell   (502) staff       (20)        1 2024-05-23 20:32:00.000000 dbt-databricks-1.8.1b2/dbt_databricks.egg-info/dependency_links.txt
--rw-r--r--   0 ben.cassell   (502) staff       (20)        1 2024-05-21 17:42:21.000000 dbt-databricks-1.8.1b2/dbt_databricks.egg-info/not-zip-safe
--rw-r--r--   0 ben.cassell   (502) staff       (20)      160 2024-05-23 20:32:00.000000 dbt-databricks-1.8.1b2/dbt_databricks.egg-info/requires.txt
--rw-r--r--   0 ben.cassell   (502) staff       (20)        4 2024-05-23 20:32:00.000000 dbt-databricks-1.8.1b2/dbt_databricks.egg-info/top_level.txt
--rw-r--r--   0 ben.cassell   (502) staff       (20)       38 2024-05-23 20:32:00.150712 dbt-databricks-1.8.1b2/setup.cfg
--rw-r--r--   0 ben.cassell   (502) staff       (20)     2623 2024-05-23 20:28:14.000000 dbt-databricks-1.8.1b2/setup.py
+drwxr-xr-x   0 ben.cassell   (502) staff       (20)        0 2024-05-08 19:39:36.521535 dbt-databricks-2.0.0rc1/
+-rw-r--r--   0 ben.cassell   (502) staff       (20)       47 2024-05-08 18:44:23.000000 dbt-databricks-2.0.0rc1/MANIFEST.in
+-rw-r--r--   0 ben.cassell   (502) staff       (20)     5379 2024-05-08 19:39:36.521361 dbt-databricks-2.0.0rc1/PKG-INFO
+-rw-r--r--   0 ben.cassell   (502) staff       (20)     4624 2024-01-19 01:37:59.000000 dbt-databricks-2.0.0rc1/README.md
+drwxr-xr-x   0 ben.cassell   (502) staff       (20)        0 2024-05-08 19:39:36.494981 dbt-databricks-2.0.0rc1/dbt/
+-rw-r--r--   0 ben.cassell   (502) staff       (20)       76 2024-01-25 18:09:59.000000 dbt-databricks-2.0.0rc1/dbt/__init__.py
+drwxr-xr-x   0 ben.cassell   (502) staff       (20)        0 2024-05-08 19:39:36.491260 dbt-databricks-2.0.0rc1/dbt/adapters/
+drwxr-xr-x   0 ben.cassell   (502) staff       (20)        0 2024-05-08 19:39:36.498675 dbt-databricks-2.0.0rc1/dbt/adapters/databricks/
+-rw-r--r--   0 ben.cassell   (502) staff       (20)      625 2024-05-08 18:44:23.000000 dbt-databricks-2.0.0rc1/dbt/adapters/databricks/__init__.py
+-rw-r--r--   0 ben.cassell   (502) staff       (20)       26 2024-05-08 18:44:23.000000 dbt-databricks-2.0.0rc1/dbt/adapters/databricks/__version__.py
+-rw-r--r--   0 ben.cassell   (502) staff       (20)     3513 2024-05-08 18:44:23.000000 dbt-databricks-2.0.0rc1/dbt/adapters/databricks/auth.py
+-rw-r--r--   0 ben.cassell   (502) staff       (20)      707 2024-05-08 18:44:23.000000 dbt-databricks-2.0.0rc1/dbt/adapters/databricks/column.py
+-rw-r--r--   0 ben.cassell   (502) staff       (20)    48111 2024-05-08 18:44:27.000000 dbt-databricks-2.0.0rc1/dbt/adapters/databricks/connections.py
+-rw-r--r--   0 ben.cassell   (502) staff       (20)    15743 2024-05-08 18:44:23.000000 dbt-databricks-2.0.0rc1/dbt/adapters/databricks/credentials.py
+drwxr-xr-x   0 ben.cassell   (502) staff       (20)        0 2024-05-08 19:39:36.500789 dbt-databricks-2.0.0rc1/dbt/adapters/databricks/events/
+-rw-r--r--   0 ben.cassell   (502) staff       (20)      796 2024-05-02 16:13:11.000000 dbt-databricks-2.0.0rc1/dbt/adapters/databricks/events/base.py
+-rw-r--r--   0 ben.cassell   (502) staff       (20)     3996 2024-05-08 18:44:27.000000 dbt-databricks-2.0.0rc1/dbt/adapters/databricks/events/connection_events.py
+-rw-r--r--   0 ben.cassell   (502) staff       (20)      616 2024-05-02 16:13:11.000000 dbt-databricks-2.0.0rc1/dbt/adapters/databricks/events/credential_events.py
+-rw-r--r--   0 ben.cassell   (502) staff       (20)     1826 2024-05-02 16:13:11.000000 dbt-databricks-2.0.0rc1/dbt/adapters/databricks/events/cursor_events.py
+-rw-r--r--   0 ben.cassell   (502) staff       (20)      250 2024-05-02 16:13:11.000000 dbt-databricks-2.0.0rc1/dbt/adapters/databricks/events/other_events.py
+-rw-r--r--   0 ben.cassell   (502) staff       (20)      842 2024-05-02 16:13:11.000000 dbt-databricks-2.0.0rc1/dbt/adapters/databricks/events/pipeline_events.py
+-rw-r--r--   0 ben.cassell   (502) staff       (20)    33226 2024-05-08 18:44:23.000000 dbt-databricks-2.0.0rc1/dbt/adapters/databricks/impl.py
+-rw-r--r--   0 ben.cassell   (502) staff       (20)      995 2024-05-08 18:44:23.000000 dbt-databricks-2.0.0rc1/dbt/adapters/databricks/logging.py
+-rw-r--r--   0 ben.cassell   (502) staff       (20)    19165 2024-05-08 18:44:23.000000 dbt-databricks-2.0.0rc1/dbt/adapters/databricks/python_submissions.py
+-rw-r--r--   0 ben.cassell   (502) staff       (20)     5313 2024-05-08 18:44:23.000000 dbt-databricks-2.0.0rc1/dbt/adapters/databricks/relation.py
+drwxr-xr-x   0 ben.cassell   (502) staff       (20)        0 2024-05-08 19:39:36.503801 dbt-databricks-2.0.0rc1/dbt/adapters/databricks/relation_configs/
+-rw-r--r--   0 ben.cassell   (502) staff       (20)     6157 2024-05-08 18:44:23.000000 dbt-databricks-2.0.0rc1/dbt/adapters/databricks/relation_configs/base.py
+-rw-r--r--   0 ben.cassell   (502) staff       (20)     1085 2024-05-08 18:44:23.000000 dbt-databricks-2.0.0rc1/dbt/adapters/databricks/relation_configs/comment.py
+-rw-r--r--   0 ben.cassell   (502) staff       (20)     1040 2024-05-08 18:44:23.000000 dbt-databricks-2.0.0rc1/dbt/adapters/databricks/relation_configs/incremental.py
+-rw-r--r--   0 ben.cassell   (502) staff       (20)     1700 2024-05-08 18:44:23.000000 dbt-databricks-2.0.0rc1/dbt/adapters/databricks/relation_configs/materialized_view.py
+-rw-r--r--   0 ben.cassell   (502) staff       (20)     1699 2024-05-08 18:44:23.000000 dbt-databricks-2.0.0rc1/dbt/adapters/databricks/relation_configs/partitioning.py
+-rw-r--r--   0 ben.cassell   (502) staff       (20)     1182 2024-05-08 18:44:23.000000 dbt-databricks-2.0.0rc1/dbt/adapters/databricks/relation_configs/query.py
+-rw-r--r--   0 ben.cassell   (502) staff       (20)     2955 2024-05-08 18:44:23.000000 dbt-databricks-2.0.0rc1/dbt/adapters/databricks/relation_configs/refresh.py
+-rw-r--r--   0 ben.cassell   (502) staff       (20)     1802 2024-05-08 18:44:23.000000 dbt-databricks-2.0.0rc1/dbt/adapters/databricks/relation_configs/streaming_table.py
+-rw-r--r--   0 ben.cassell   (502) staff       (20)     1850 2024-05-08 18:44:23.000000 dbt-databricks-2.0.0rc1/dbt/adapters/databricks/relation_configs/tags.py
+-rw-r--r--   0 ben.cassell   (502) staff       (20)     2631 2024-05-08 18:44:23.000000 dbt-databricks-2.0.0rc1/dbt/adapters/databricks/relation_configs/tblproperties.py
+-rw-r--r--   0 ben.cassell   (502) staff       (20)     2503 2024-05-08 18:44:23.000000 dbt-databricks-2.0.0rc1/dbt/adapters/databricks/utils.py
+drwxr-xr-x   0 ben.cassell   (502) staff       (20)        0 2024-05-08 19:39:36.491927 dbt-databricks-2.0.0rc1/dbt/include/
+drwxr-xr-x   0 ben.cassell   (502) staff       (20)        0 2024-05-08 19:39:36.504794 dbt-databricks-2.0.0rc1/dbt/include/databricks/
+-rw-r--r--   0 ben.cassell   (502) staff       (20)       52 2023-05-30 21:40:46.000000 dbt-databricks-2.0.0rc1/dbt/include/databricks/__init__.py
+-rw-r--r--   0 ben.cassell   (502) staff       (20)       77 2023-05-30 21:40:46.000000 dbt-databricks-2.0.0rc1/dbt/include/databricks/dbt_project.yml
+drwxr-xr-x   0 ben.cassell   (502) staff       (20)        0 2024-05-08 19:39:36.493824 dbt-databricks-2.0.0rc1/dbt/include/databricks/macros/
+drwxr-xr-x   0 ben.cassell   (502) staff       (20)        0 2024-05-08 19:39:36.506895 dbt-databricks-2.0.0rc1/dbt/include/databricks/macros/adapters/
+-rw-r--r--   0 ben.cassell   (502) staff       (20)     3445 2024-05-08 18:44:23.000000 dbt-databricks-2.0.0rc1/dbt/include/databricks/macros/adapters/catalog.sql
+-rw-r--r--   0 ben.cassell   (502) staff       (20)     2409 2024-03-26 16:27:09.000000 dbt-databricks-2.0.0rc1/dbt/include/databricks/macros/adapters/copy_into.sql
+-rw-r--r--   0 ben.cassell   (502) staff       (20)      592 2024-05-08 18:44:23.000000 dbt-databricks-2.0.0rc1/dbt/include/databricks/macros/adapters/databricks_catalog.sql
+-rw-r--r--   0 ben.cassell   (502) staff       (20)     5153 2024-05-08 18:44:23.000000 dbt-databricks-2.0.0rc1/dbt/include/databricks/macros/adapters/metadata.sql
+-rw-r--r--   0 ben.cassell   (502) staff       (20)     1984 2024-05-08 18:44:23.000000 dbt-databricks-2.0.0rc1/dbt/include/databricks/macros/adapters/persist_docs.sql
+-rw-r--r--   0 ben.cassell   (502) staff       (20)     3540 2024-05-08 18:44:23.000000 dbt-databricks-2.0.0rc1/dbt/include/databricks/macros/adapters/python.sql
+-rw-r--r--   0 ben.cassell   (502) staff       (20)     1158 2024-05-08 18:44:23.000000 dbt-databricks-2.0.0rc1/dbt/include/databricks/macros/adapters/relation.sql
+drwxr-xr-x   0 ben.cassell   (502) staff       (20)        0 2024-05-08 19:39:36.507117 dbt-databricks-2.0.0rc1/dbt/include/databricks/macros/etc/
+-rw-r--r--   0 ben.cassell   (502) staff       (20)      648 2024-03-26 16:27:09.000000 dbt-databricks-2.0.0rc1/dbt/include/databricks/macros/etc/statement.sql
+drwxr-xr-x   0 ben.cassell   (502) staff       (20)        0 2024-05-08 19:39:36.507337 dbt-databricks-2.0.0rc1/dbt/include/databricks/macros/get_custom_name/
+-rw-r--r--   0 ben.cassell   (502) staff       (20)      458 2024-05-08 18:44:23.000000 dbt-databricks-2.0.0rc1/dbt/include/databricks/macros/get_custom_name/get_custom_database.sql
+drwxr-xr-x   0 ben.cassell   (502) staff       (20)        0 2024-05-08 19:39:36.509359 dbt-databricks-2.0.0rc1/dbt/include/databricks/macros/materializations/
+-rw-r--r--   0 ben.cassell   (502) staff       (20)     2803 2024-05-08 18:44:23.000000 dbt-databricks-2.0.0rc1/dbt/include/databricks/macros/materializations/clone.sql
+drwxr-xr-x   0 ben.cassell   (502) staff       (20)        0 2024-05-08 19:39:36.510259 dbt-databricks-2.0.0rc1/dbt/include/databricks/macros/materializations/incremental/
+-rw-r--r--   0 ben.cassell   (502) staff       (20)     4875 2024-05-08 18:44:23.000000 dbt-databricks-2.0.0rc1/dbt/include/databricks/macros/materializations/incremental/incremental.sql
+-rw-r--r--   0 ben.cassell   (502) staff       (20)     5522 2024-05-08 18:44:23.000000 dbt-databricks-2.0.0rc1/dbt/include/databricks/macros/materializations/incremental/strategies.sql
+-rw-r--r--   0 ben.cassell   (502) staff       (20)     1896 2024-05-08 18:44:23.000000 dbt-databricks-2.0.0rc1/dbt/include/databricks/macros/materializations/incremental/validate.sql
+-rw-r--r--   0 ben.cassell   (502) staff       (20)     3657 2024-05-08 18:44:23.000000 dbt-databricks-2.0.0rc1/dbt/include/databricks/macros/materializations/materialized_view.sql
+drwxr-xr-x   0 ben.cassell   (502) staff       (20)        0 2024-05-08 19:39:36.510888 dbt-databricks-2.0.0rc1/dbt/include/databricks/macros/materializations/seeds/
+-rw-r--r--   0 ben.cassell   (502) staff       (20)     2849 2024-05-08 18:44:23.000000 dbt-databricks-2.0.0rc1/dbt/include/databricks/macros/materializations/seeds/helpers.sql
+-rw-r--r--   0 ben.cassell   (502) staff       (20)     2477 2024-05-08 18:44:23.000000 dbt-databricks-2.0.0rc1/dbt/include/databricks/macros/materializations/seeds/seeds.sql
+-rw-r--r--   0 ben.cassell   (502) staff       (20)     5397 2024-03-29 15:20:41.000000 dbt-databricks-2.0.0rc1/dbt/include/databricks/macros/materializations/snapshot.sql
+-rw-r--r--   0 ben.cassell   (502) staff       (20)     3623 2024-05-08 18:44:23.000000 dbt-databricks-2.0.0rc1/dbt/include/databricks/macros/materializations/streaming_table.sql
+-rw-r--r--   0 ben.cassell   (502) staff       (20)     1966 2024-05-08 18:44:23.000000 dbt-databricks-2.0.0rc1/dbt/include/databricks/macros/materializations/table.sql
+-rw-r--r--   0 ben.cassell   (502) staff       (20)     1364 2024-05-08 18:44:23.000000 dbt-databricks-2.0.0rc1/dbt/include/databricks/macros/materializations/view.sql
+drwxr-xr-x   0 ben.cassell   (502) staff       (20)        0 2024-05-08 19:39:36.513975 dbt-databricks-2.0.0rc1/dbt/include/databricks/macros/relations/
+drwxr-xr-x   0 ben.cassell   (502) staff       (20)        0 2024-05-08 19:39:36.515305 dbt-databricks-2.0.0rc1/dbt/include/databricks/macros/relations/components/
+-rw-r--r--   0 ben.cassell   (502) staff       (20)      131 2024-05-08 18:44:23.000000 dbt-databricks-2.0.0rc1/dbt/include/databricks/macros/relations/components/comment.sql
+-rw-r--r--   0 ben.cassell   (502) staff       (20)      217 2024-05-08 18:44:23.000000 dbt-databricks-2.0.0rc1/dbt/include/databricks/macros/relations/components/partitioning.sql
+-rw-r--r--   0 ben.cassell   (502) staff       (20)      670 2024-05-08 18:44:23.000000 dbt-databricks-2.0.0rc1/dbt/include/databricks/macros/relations/components/refresh_schedule.sql
+-rw-r--r--   0 ben.cassell   (502) staff       (20)      310 2024-05-08 18:44:23.000000 dbt-databricks-2.0.0rc1/dbt/include/databricks/macros/relations/components/tblproperties.sql
+-rw-r--r--   0 ben.cassell   (502) staff       (20)    10574 2024-05-08 18:44:23.000000 dbt-databricks-2.0.0rc1/dbt/include/databricks/macros/relations/constraints.sql
+-rw-r--r--   0 ben.cassell   (502) staff       (20)      629 2024-05-08 18:44:23.000000 dbt-databricks-2.0.0rc1/dbt/include/databricks/macros/relations/create.sql
+-rw-r--r--   0 ben.cassell   (502) staff       (20)      564 2024-05-08 18:44:23.000000 dbt-databricks-2.0.0rc1/dbt/include/databricks/macros/relations/drop.sql
+-rw-r--r--   0 ben.cassell   (502) staff       (20)      147 2024-05-08 18:44:23.000000 dbt-databricks-2.0.0rc1/dbt/include/databricks/macros/relations/file_format.sql
+-rw-r--r--   0 ben.cassell   (502) staff       (20)      615 2024-05-08 18:44:23.000000 dbt-databricks-2.0.0rc1/dbt/include/databricks/macros/relations/location.sql
+drwxr-xr-x   0 ben.cassell   (502) staff       (20)        0 2024-05-08 19:39:36.516644 dbt-databricks-2.0.0rc1/dbt/include/databricks/macros/relations/materialized_view/
+-rw-r--r--   0 ben.cassell   (502) staff       (20)     1801 2024-05-08 18:44:23.000000 dbt-databricks-2.0.0rc1/dbt/include/databricks/macros/relations/materialized_view/alter.sql
+-rw-r--r--   0 ben.cassell   (502) staff       (20)      756 2024-05-08 18:44:23.000000 dbt-databricks-2.0.0rc1/dbt/include/databricks/macros/relations/materialized_view/create.sql
+-rw-r--r--   0 ben.cassell   (502) staff       (20)      126 2024-05-08 18:44:23.000000 dbt-databricks-2.0.0rc1/dbt/include/databricks/macros/relations/materialized_view/drop.sql
+-rw-r--r--   0 ben.cassell   (502) staff       (20)      119 2024-05-08 18:44:23.000000 dbt-databricks-2.0.0rc1/dbt/include/databricks/macros/relations/materialized_view/refresh.sql
+-rw-r--r--   0 ben.cassell   (502) staff       (20)     1372 2024-05-08 18:44:23.000000 dbt-databricks-2.0.0rc1/dbt/include/databricks/macros/relations/optimize.sql
+-rw-r--r--   0 ben.cassell   (502) staff       (20)     2273 2024-05-08 18:44:23.000000 dbt-databricks-2.0.0rc1/dbt/include/databricks/macros/relations/replace.sql
+drwxr-xr-x   0 ben.cassell   (502) staff       (20)        0 2024-05-08 19:39:36.517490 dbt-databricks-2.0.0rc1/dbt/include/databricks/macros/relations/streaming_table/
+-rw-r--r--   0 ben.cassell   (502) staff       (20)     3212 2024-05-08 18:44:23.000000 dbt-databricks-2.0.0rc1/dbt/include/databricks/macros/relations/streaming_table/alter.sql
+-rw-r--r--   0 ben.cassell   (502) staff       (20)      904 2024-05-08 18:44:23.000000 dbt-databricks-2.0.0rc1/dbt/include/databricks/macros/relations/streaming_table/create.sql
+-rw-r--r--   0 ben.cassell   (502) staff       (20)      246 2024-05-08 18:44:23.000000 dbt-databricks-2.0.0rc1/dbt/include/databricks/macros/relations/streaming_table/drop.sql
+-rw-r--r--   0 ben.cassell   (502) staff       (20)      292 2024-05-08 18:44:23.000000 dbt-databricks-2.0.0rc1/dbt/include/databricks/macros/relations/streaming_table/refresh.sql
+drwxr-xr-x   0 ben.cassell   (502) staff       (20)        0 2024-05-08 19:39:36.518192 dbt-databricks-2.0.0rc1/dbt/include/databricks/macros/relations/table/
+-rw-r--r--   0 ben.cassell   (502) staff       (20)     3161 2024-05-08 18:44:23.000000 dbt-databricks-2.0.0rc1/dbt/include/databricks/macros/relations/table/create.sql
+-rw-r--r--   0 ben.cassell   (502) staff       (20)      102 2024-05-08 18:44:23.000000 dbt-databricks-2.0.0rc1/dbt/include/databricks/macros/relations/table/drop.sql
+-rw-r--r--   0 ben.cassell   (502) staff       (20)     1604 2024-05-08 18:44:23.000000 dbt-databricks-2.0.0rc1/dbt/include/databricks/macros/relations/tags.sql
+-rw-r--r--   0 ben.cassell   (502) staff       (20)      764 2024-05-01 20:15:21.000000 dbt-databricks-2.0.0rc1/dbt/include/databricks/macros/relations/tblproperties.sql
+drwxr-xr-x   0 ben.cassell   (502) staff       (20)        0 2024-05-08 19:39:36.518815 dbt-databricks-2.0.0rc1/dbt/include/databricks/macros/relations/view/
+-rw-r--r--   0 ben.cassell   (502) staff       (20)      643 2024-05-08 18:44:23.000000 dbt-databricks-2.0.0rc1/dbt/include/databricks/macros/relations/view/create.sql
+-rw-r--r--   0 ben.cassell   (502) staff       (20)      100 2024-05-08 18:44:23.000000 dbt-databricks-2.0.0rc1/dbt/include/databricks/macros/relations/view/drop.sql
+drwxr-xr-x   0 ben.cassell   (502) staff       (20)        0 2024-05-08 19:39:36.519299 dbt-databricks-2.0.0rc1/dbt/include/databricks/macros/utils/
+-rw-r--r--   0 ben.cassell   (502) staff       (20)      318 2023-05-30 21:40:46.000000 dbt-databricks-2.0.0rc1/dbt/include/databricks/macros/utils/dateadd.sql
+-rw-r--r--   0 ben.cassell   (502) staff       (20)      338 2023-10-26 17:27:28.000000 dbt-databricks-2.0.0rc1/dbt/include/databricks/macros/utils/datediff.sql
+-rw-r--r--   0 ben.cassell   (502) staff       (20)      535 2023-05-30 21:40:46.000000 dbt-databricks-2.0.0rc1/dbt/include/databricks/profile_template.yml
+drwxr-xr-x   0 ben.cassell   (502) staff       (20)        0 2024-05-08 19:39:36.520890 dbt-databricks-2.0.0rc1/dbt_databricks.egg-info/
+-rw-r--r--   0 ben.cassell   (502) staff       (20)     5379 2024-05-08 19:39:36.000000 dbt-databricks-2.0.0rc1/dbt_databricks.egg-info/PKG-INFO
+-rw-r--r--   0 ben.cassell   (502) staff       (20)     4441 2024-05-08 19:39:36.000000 dbt-databricks-2.0.0rc1/dbt_databricks.egg-info/SOURCES.txt
+-rw-r--r--   0 ben.cassell   (502) staff       (20)        1 2024-05-08 19:39:36.000000 dbt-databricks-2.0.0rc1/dbt_databricks.egg-info/dependency_links.txt
+-rw-r--r--   0 ben.cassell   (502) staff       (20)        1 2024-05-08 19:39:36.000000 dbt-databricks-2.0.0rc1/dbt_databricks.egg-info/not-zip-safe
+-rw-r--r--   0 ben.cassell   (502) staff       (20)      166 2024-05-08 19:39:36.000000 dbt-databricks-2.0.0rc1/dbt_databricks.egg-info/requires.txt
+-rw-r--r--   0 ben.cassell   (502) staff       (20)        4 2024-05-08 19:39:36.000000 dbt-databricks-2.0.0rc1/dbt_databricks.egg-info/top_level.txt
+-rw-r--r--   0 ben.cassell   (502) staff       (20)       38 2024-05-08 19:39:36.521583 dbt-databricks-2.0.0rc1/setup.cfg
+-rw-r--r--   0 ben.cassell   (502) staff       (20)     2629 2024-05-08 18:44:27.000000 dbt-databricks-2.0.0rc1/setup.py
```

### Comparing `dbt-databricks-1.8.1b2/PKG-INFO` & `dbt-databricks-2.0.0rc1/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: dbt-databricks
-Version: 1.8.1b2
+Version: 2.0.0rc1
 Summary: The Databricks adapter plugin for dbt
 Home-page: https://github.com/databricks/dbt-databricks
 Author: Databricks
 Author-email: feedback@databricks.com
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Operating System :: Microsoft :: Windows
```

### Comparing `dbt-databricks-1.8.1b2/README.md` & `dbt-databricks-2.0.0rc1/README.md`

 * *Files identical despite different names*

### Comparing `dbt-databricks-1.8.1b2/dbt/adapters/databricks/__init__.py` & `dbt-databricks-2.0.0rc1/dbt/adapters/databricks/__init__.py`

 * *Files identical despite different names*

### Comparing `dbt-databricks-1.8.1b2/dbt/adapters/databricks/auth.py` & `dbt-databricks-2.0.0rc1/dbt/adapters/databricks/auth.py`

 * *Files identical despite different names*

### Comparing `dbt-databricks-1.8.1b2/dbt/adapters/databricks/column.py` & `dbt-databricks-2.0.0rc1/dbt/adapters/databricks/column.py`

 * *Files identical despite different names*

### Comparing `dbt-databricks-1.8.1b2/dbt/adapters/databricks/connections.py` & `dbt-databricks-2.0.0rc1/dbt/adapters/databricks/connections.py`

 * *Files 2% similar despite different names*

```diff
@@ -16,17 +16,17 @@
 from typing import Dict
 from typing import Hashable
 from typing import Iterator
 from typing import List
 from typing import Optional
 from typing import Sequence
 from typing import Tuple
-from typing import TYPE_CHECKING
 
 import databricks.sql as dbsql
+from agate import Table
 from databricks.sql.client import Connection as DatabricksSQLConnection
 from databricks.sql.client import Cursor as DatabricksSQLCursor
 from databricks.sql.exc import Error
 from dbt.adapters.base.query_headers import MacroQueryStringSetter
 from dbt.adapters.contracts.connection import AdapterRequiredConfig
 from dbt.adapters.contracts.connection import AdapterResponse
 from dbt.adapters.contracts.connection import Connection
@@ -66,24 +66,22 @@
 from dbt.adapters.events.types import ConnectionLeftOpenInCleanup
 from dbt.adapters.events.types import ConnectionReused
 from dbt.adapters.events.types import ConnectionUsed
 from dbt.adapters.events.types import NewConnection
 from dbt.adapters.events.types import SQLQuery
 from dbt.adapters.events.types import SQLQueryStatus
 from dbt.adapters.spark.connections import SparkConnectionManager
+from dbt_common.clients import agate_helper
 from dbt_common.events.contextvars import get_node_info
 from dbt_common.events.functions import fire_event
 from dbt_common.exceptions import DbtInternalError
 from dbt_common.exceptions import DbtRuntimeError
 from dbt_common.utils import cast_to_str
 from requests import Session
 
-if TYPE_CHECKING:
-    from agate import Table
-
 
 mv_refresh_regex = re.compile(r"refresh\s+materialized\s+view\s+([`\w.]+)", re.IGNORECASE)
 st_refresh_regex = re.compile(
     r"create\s+or\s+refresh\s+streaming\s+table\s+([`\w.]+)", re.IGNORECASE
 )
 
 
@@ -224,41 +222,54 @@
         # print(f"execute: {sql}")
         if sql.strip().endswith(";"):
             sql = sql.strip()[:-1]
         if bindings is not None:
             bindings = [self._fix_binding(binding) for binding in bindings]
         self._cursor.execute(sql, bindings)
 
-    def poll_refresh_pipeline(self, pipeline_id: str) -> None:
+        # if the command was to refresh a materialized view we need to poll
+        # the pipeline until the refresh is finished.
+        self.pollRefreshPipeline(sql)
+
+    def pollRefreshPipeline(
+        self,
+        sql: str,
+    ) -> None:
+        should_poll, model_name = _should_poll_refresh(sql)
+        if not should_poll:
+            return
+
         # interval in seconds
         polling_interval = 10
 
         # timeout in seconds
         timeout = 60 * 60
 
         stopped_states = ("COMPLETED", "FAILED", "CANCELED")
         host: str = self._creds.host or ""
         headers = (
             self._cursor.connection.thrift_backend._auth_provider._header_factory  # type: ignore
         )
         session = Session()
         session.auth = BearerAuth(headers)
         session.headers = {"User-Agent": self._user_agent}
+
+        pipeline_id = _get_table_view_pipeline_id(session, host, model_name)
         pipeline = _get_pipeline_state(session, host, pipeline_id)
         # get the most recently created update for the pipeline
         latest_update = _find_update(pipeline)
         if not latest_update:
             raise DbtRuntimeError(f"No update created for pipeline: {pipeline_id}")
 
         state = latest_update.get("state")
         # we use update_id to retrieve the update in the polling loop
         update_id = latest_update.get("update_id", "")
         prev_state = state
 
-        logger.info(PipelineRefresh(pipeline_id, update_id, str(state)))
+        logger.info(PipelineRefresh(pipeline_id, update_id, model_name, str(state)))
 
         start = time.time()
         exceeded_timeout = False
         while state not in stopped_states:
             if time.time() - start > timeout:
                 exceeded_timeout = True
                 break
@@ -272,15 +283,15 @@
             if not update:
                 raise DbtRuntimeError(
                     f"Error getting pipeline update info: {pipeline_id}, update: {update_id}"
                 )
 
             state = update.get("state")
             if state != prev_state:
-                logger.info(PipelineRefresh(pipeline_id, update_id, str(state)))
+                logger.info(PipelineRefresh(pipeline_id, update_id, model_name, str(state)))
                 prev_state = state
 
             if state == "FAILED":
                 logger.error(
                     PipelineRefreshError(
                         pipeline_id,
                         update_id,
@@ -300,18 +311,18 @@
                     state = None
 
         if exceeded_timeout:
             raise DbtRuntimeError("timed out waiting for materialized view refresh")
 
         if state == "FAILED":
             msg = _get_update_error_msg(session, host, pipeline_id, update_id)
-            raise DbtRuntimeError(f"Error refreshing pipeline {pipeline_id} {msg}")
+            raise DbtRuntimeError(f"error refreshing model {model_name} {msg}")
 
         if state == "CANCELED":
-            raise DbtRuntimeError(f"Refreshing pipeline {pipeline_id} cancelled")
+            raise DbtRuntimeError(f"refreshing model {model_name} cancelled")
 
         return
 
     @classmethod
     def findUpdate(cls, updates: List, id: str) -> Optional[Dict]:
         matches = [x for x in updates if x.get("update_id") == id]
         if matches:
@@ -606,33 +617,30 @@
 
     def execute(
         self,
         sql: str,
         auto_begin: bool = False,
         fetch: bool = False,
         limit: Optional[int] = None,
-    ) -> Tuple[DatabricksAdapterResponse, "Table"]:
+    ) -> Tuple[DatabricksAdapterResponse, Table]:
         sql = self._add_query_comment(sql)
         _, cursor = self.add_query(sql, auto_begin)
         try:
             response = self.get_response(cursor)
             if fetch:
                 table = self.get_result_from_cursor(cursor, limit)
             else:
-                # Lazy import agate to improve CLI startup time
-                from dbt_common.clients import agate_helper
-
                 table = agate_helper.empty_table()
             return response, table
         finally:
             cursor.close()
 
     def _execute_cursor(
         self, log_sql: str, f: Callable[[DatabricksSQLCursorWrapper], None]
-    ) -> "Table":
+    ) -> Table:
         connection = self.get_thread_connection()
 
         fire_event(ConnectionUsed(conn_type=self.TYPE, conn_name=cast_to_str(connection.name)))
 
         with self.exception_handler(log_sql):
             cursor: Optional[DatabricksSQLCursorWrapper] = None
             try:
@@ -659,24 +667,24 @@
                 )
 
                 return self.get_result_from_cursor(cursor, None)
             finally:
                 if cursor is not None:
                     cursor.close()
 
-    def list_schemas(self, database: str, schema: Optional[str] = None) -> "Table":
+    def list_schemas(self, database: str, schema: Optional[str] = None) -> Table:
         database = database.strip("`")
         if schema:
             schema = schema.strip("`").lower()
         return self._execute_cursor(
             f"GetSchemas(database={database}, schema={schema})",
             lambda cursor: cursor.schemas(catalog_name=database, schema_name=schema),
         )
 
-    def list_tables(self, database: str, schema: str, identifier: Optional[str] = None) -> "Table":
+    def list_tables(self, database: str, schema: str, identifier: Optional[str] = None) -> Table:
         database = database.strip("`")
         schema = schema.strip("`").lower()
         if identifier:
             identifier = identifier.strip("`")
         return self._execute_cursor(
             f"GetTables(database={database}, schema={schema}, identifier={identifier})",
             lambda cursor: cursor.tables(
@@ -752,15 +760,15 @@
                 return DatabricksSQLConnectionWrapper(
                     conn,
                     is_cluster=creds.cluster_id is not None,
                     creds=creds,
                     user_agent=user_agent_entry,
                 )
             except Error as exc:
-                logger.error(ConnectionCreateError(exc))
+                logger.error(ConnectionCreateError(conn, exc))
                 raise
 
         def exponential_backoff(attempt: int) -> int:
             return attempt * attempt
 
         retryable_exceptions = []
         # this option is for backwards compatibility
@@ -1050,15 +1058,15 @@
                 return DatabricksSQLConnectionWrapper(
                     conn,
                     is_cluster=creds.cluster_id is not None,
                     creds=creds,
                     user_agent=user_agent_entry,
                 )
             except Error as exc:
-                logger.error(ConnectionCreateError(exc))
+                logger.error(ConnectionCreateError(None, exc))
                 raise
 
         def exponential_backoff(attempt: int) -> int:
             return attempt * attempt
 
         retryable_exceptions = []
         # this option is for backwards compatibility
@@ -1071,14 +1079,45 @@
             logger=logger,
             retryable_exceptions=retryable_exceptions,
             retry_limit=creds.connect_retries,
             retry_timeout=(timeout if timeout is not None else exponential_backoff),
         )
 
 
+def _should_poll_refresh(sql: str) -> Tuple[bool, str]:
+    # if the command was to refresh a materialized view we need to poll
+    # the pipeline until the refresh is finished.
+    name = ""
+    refresh_search = mv_refresh_regex.search(sql)
+    if not refresh_search:
+        refresh_search = st_refresh_regex.search(sql)
+
+    if refresh_search:
+        name = refresh_search.group(1).replace("`", "")
+
+    return refresh_search is not None, name
+
+
+def _get_table_view_pipeline_id(session: Session, host: str, name: str) -> str:
+    table_url = f"https://{host}/api/2.1/unity-catalog/tables/{name}"
+    resp1 = session.get(table_url)
+    if resp1.status_code != 200:
+        raise DbtRuntimeError(
+            f"Error getting info for materialized view/streaming table {name}: {resp1.text}"
+        )
+
+    pipeline_id = resp1.json().get("pipeline_id", "")
+    if not pipeline_id:
+        raise DbtRuntimeError(
+            f"Materialized view/streaming table {name} does not have a pipeline id"
+        )
+
+    return pipeline_id
+
+
 def _get_pipeline_state(session: Session, host: str, pipeline_id: str) -> dict:
     pipeline_url = f"https://{host}/api/2.0/pipelines/{pipeline_id}"
 
     response = session.get(pipeline_url)
     if response.status_code != 200:
         raise DbtRuntimeError(f"Error getting pipeline info for {pipeline_id}: {response.text}")
```

### Comparing `dbt-databricks-1.8.1b2/dbt/adapters/databricks/credentials.py` & `dbt-databricks-2.0.0rc1/dbt/adapters/databricks/credentials.py`

 * *Files identical despite different names*

### Comparing `dbt-databricks-1.8.1b2/dbt/adapters/databricks/events/base.py` & `dbt-databricks-2.0.0rc1/dbt/adapters/databricks/events/base.py`

 * *Files identical despite different names*

### Comparing `dbt-databricks-1.8.1b2/dbt/adapters/databricks/events/connection_events.py` & `dbt-databricks-2.0.0rc1/dbt/adapters/databricks/events/connection_events.py`

 * *Files 4% similar despite different names*

```diff
@@ -39,17 +39,17 @@
     def __init__(self, connection: Optional[Connection], exception: Exception):
         super().__init__(
             connection, str(SQLErrorEvent(exception, "Exception while trying to close connection"))
         )
 
 
 class ConnectionCreateError(ConnectionEvent):
-    def __init__(self, exception: Exception):
+    def __init__(self, connection: Optional[Connection], exception: Exception):
         super().__init__(
-            None, str(SQLErrorEvent(exception, "Exception while trying to create connection"))
+            connection, str(SQLErrorEvent(exception, "Exception while trying to create connection"))
         )
 
 
 class ConnectionWrapperEvent(ABC):
     def __init__(self, description: str, message: str):
         self.message = message
         self.description = description
```

### Comparing `dbt-databricks-1.8.1b2/dbt/adapters/databricks/events/credential_events.py` & `dbt-databricks-2.0.0rc1/dbt/adapters/databricks/events/credential_events.py`

 * *Files identical despite different names*

### Comparing `dbt-databricks-1.8.1b2/dbt/adapters/databricks/events/cursor_events.py` & `dbt-databricks-2.0.0rc1/dbt/adapters/databricks/events/cursor_events.py`

 * *Files identical despite different names*

### Comparing `dbt-databricks-1.8.1b2/dbt/adapters/databricks/events/pipeline_events.py` & `dbt-databricks-2.0.0rc1/dbt/adapters/databricks/events/pipeline_events.py`

 * *Files 10% similar despite different names*

```diff
@@ -10,14 +10,16 @@
     def __str__(self) -> str:
         return (
             f"Pipeline(pipeline-id={self.pipeline_id}, update-id={self.update_id}) - {self.message}"
         )
 
 
 class PipelineRefresh(PipelineEvent):
-    def __init__(self, pipeline_id: str, update_id: str, state: str):
-        super().__init__(pipeline_id, update_id, f"Refreshing - got state {state}")
+    def __init__(self, pipeline_id: str, update_id: str, model_name: str, state: str):
+        super().__init__(
+            pipeline_id, update_id, f"Refreshing model {model_name} with state {state}"
+        )
 
 
 class PipelineRefreshError(PipelineEvent):
     def __init__(self, pipeline_id: str, update_id: str, message: str):
         super().__init__(pipeline_id, update_id, f"Error refreshing pipeline: {message}")
```

### Comparing `dbt-databricks-1.8.1b2/dbt/adapters/databricks/impl.py` & `dbt-databricks-2.0.0rc1/dbt/adapters/databricks/impl.py`

 * *Files 12% similar despite different names*

```diff
@@ -3,87 +3,82 @@
 from abc import ABC
 from abc import abstractmethod
 from collections import defaultdict
 from concurrent.futures import Future
 from contextlib import contextmanager
 from dataclasses import dataclass
 from typing import Any
-from typing import Callable
-from typing import cast
 from typing import ClassVar
 from typing import Dict
 from typing import FrozenSet
 from typing import Generic
 from typing import Iterable
 from typing import Iterator
 from typing import List
 from typing import Optional
 from typing import Set
 from typing import Tuple
 from typing import Type
-from typing import TYPE_CHECKING
-from typing import TypeVar
 from typing import Union
 
+from agate import Row
+from agate import Table
+from agate import Text
 from dbt.adapters.base import AdapterConfig
 from dbt.adapters.base import PythonJobHelper
 from dbt.adapters.base.impl import catch_as_completed
 from dbt.adapters.base.meta import available
 from dbt.adapters.base.relation import BaseRelation
+from dbt.adapters.base.relation import InformationSchema
 from dbt.adapters.capability import Capability
 from dbt.adapters.capability import CapabilityDict
 from dbt.adapters.capability import CapabilitySupport
 from dbt.adapters.capability import Support
 from dbt.adapters.contracts.connection import AdapterResponse
 from dbt.adapters.contracts.connection import Connection
 from dbt.adapters.contracts.relation import RelationConfig
 from dbt.adapters.contracts.relation import RelationType
 from dbt.adapters.databricks.column import DatabricksColumn
 from dbt.adapters.databricks.connections import DatabricksConnectionManager
-from dbt.adapters.databricks.connections import DatabricksDBTConnection
-from dbt.adapters.databricks.connections import DatabricksSQLConnectionWrapper
 from dbt.adapters.databricks.connections import ExtendedSessionConnectionManager
 from dbt.adapters.databricks.connections import USE_LONG_SESSIONS
+from dbt.adapters.databricks.logging import logger
 from dbt.adapters.databricks.python_submissions import (
     DbtDatabricksAllPurposeClusterPythonJobHelper,
 )
 from dbt.adapters.databricks.python_submissions import (
     DbtDatabricksJobClusterPythonJobHelper,
 )
 from dbt.adapters.databricks.relation import DatabricksRelation
 from dbt.adapters.databricks.relation import DatabricksRelationType
-from dbt.adapters.databricks.relation import KEY_TABLE_PROVIDER
+from dbt.adapters.databricks.relation import extract_identifiers
+from dbt.adapters.databricks.relation import is_hive_metastore
 from dbt.adapters.databricks.relation_configs.base import DatabricksRelationConfig
 from dbt.adapters.databricks.relation_configs.base import DatabricksRelationConfigBase
 from dbt.adapters.databricks.relation_configs.incremental import IncrementalTableConfig
 from dbt.adapters.databricks.relation_configs.materialized_view import (
     MaterializedViewConfig,
 )
 from dbt.adapters.databricks.relation_configs.streaming_table import (
     StreamingTableConfig,
 )
-from dbt.adapters.databricks.relation_configs.tblproperties import TblPropertiesConfig
 from dbt.adapters.databricks.utils import get_first_row
 from dbt.adapters.databricks.utils import redact_credentials
 from dbt.adapters.databricks.utils import undefined_proof
 from dbt.adapters.relation_configs import RelationResults
 from dbt.adapters.spark.impl import DESCRIBE_TABLE_EXTENDED_MACRO_NAME
 from dbt.adapters.spark.impl import GET_COLUMNS_IN_RELATION_RAW_MACRO_NAME
 from dbt.adapters.spark.impl import KEY_TABLE_OWNER
 from dbt.adapters.spark.impl import KEY_TABLE_STATISTICS
 from dbt.adapters.spark.impl import LIST_SCHEMAS_MACRO_NAME
 from dbt.adapters.spark.impl import SparkAdapter
 from dbt.adapters.spark.impl import TABLE_OR_VIEW_NOT_FOUND_MESSAGES
+from dbt_common.clients.agate_helper import DEFAULT_TYPE_TESTER
 from dbt_common.exceptions import DbtRuntimeError
 from dbt_common.utils import executor
-from dbt_common.utils.dict import AttrDict
-
-if TYPE_CHECKING:
-    from agate import Row
-    from agate import Table
 
 CURRENT_CATALOG_MACRO_NAME = "current_catalog"
 USE_CATALOG_MACRO_NAME = "use_catalog"
 GET_CATALOG_MACRO_NAME = "get_catalog"
 SHOW_TABLE_EXTENDED_MACRO_NAME = "show_table_extended"
 SHOW_TABLES_MACRO_NAME = "show_tables"
 SHOW_VIEWS_MACRO_NAME = "show_views"
@@ -104,29 +99,15 @@
     tblproperties: Optional[Dict[str, str]] = None
     zorder: Optional[Union[List[str], str]] = None
 
 
 def check_not_found_error(errmsg: str) -> bool:
     new_error = "[SCHEMA_NOT_FOUND]" in errmsg
     old_error = re.match(r".*(Database).*(not found).*", errmsg, re.DOTALL)
-    found_msgs = (msg in errmsg for msg in TABLE_OR_VIEW_NOT_FOUND_MESSAGES)
-    return new_error or old_error is not None or any(found_msgs)
-
-
-T = TypeVar("T")
-
-
-def handle_missing_objects(exec: Callable[[], T], default: T) -> T:
-    try:
-        return exec()
-    except DbtRuntimeError as e:
-        errmsg = getattr(e, "msg", "")
-        if check_not_found_error(errmsg):
-            return default
-        raise e
+    return new_error or old_error is not None
 
 
 def get_identifier_list_string(table_names: Set[str]) -> str:
     """Returns `"|".join(table_names)` by default.
 
     Returns `"*"` if `DBT_DESCRIBE_TABLE_2048_CHAR_BYPASS` == `"true"`
     and the joined string exceeds 2048 characters
@@ -156,15 +137,15 @@
     connections: DatabricksConnectionManager
 
     AdapterSpecificConfigs = DatabricksConfig
 
     _capabilities = CapabilityDict(
         {
             Capability.TableLastModifiedMetadata: CapabilitySupport(support=Support.Full),
-            Capability.SchemaMetadataByRelations: CapabilitySupport(support=Support.Full),
+            Capability.SchemaMetadataByRelations: CapabilitySupport(support=Support.NotImplemented),
         }
     )
 
     # override/overload
     def acquire_connection(
         self, name: Optional[str] = None, query_header_context: Any = None
     ) -> Connection:
@@ -217,80 +198,117 @@
         self,
         sql: str,
         auto_begin: bool = False,
         fetch: bool = False,
         limit: Optional[int] = None,
         *,
         staging_table: Optional[BaseRelation] = None,
-    ) -> Tuple[AdapterResponse, "Table"]:
+    ) -> Tuple[AdapterResponse, Table]:
         try:
             return super().execute(sql=sql, auto_begin=auto_begin, fetch=fetch, limit=limit)
         finally:
             if staging_table is not None:
                 self.drop_relation(staging_table)
 
     def list_relations_without_caching(  # type: ignore[override]
         self, schema_relation: DatabricksRelation
     ) -> List[DatabricksRelation]:
-        empty: List[Tuple[Optional[str], Optional[str], Optional[str], Optional[str]]] = []
-        results = handle_missing_objects(
-            lambda: self.get_relations_without_caching(schema_relation), empty
-        )
+        try:
+            results = self.get_relations_without_caching(schema_relation)
+        except DbtRuntimeError as e:
+            errmsg = getattr(e, "msg", "")
+            if check_not_found_error(errmsg):
+                return []
+            else:
+                description = "Error while retrieving information about"
+                logger.debug(f"{description} {schema_relation}: {e.msg}")
+                raise e
+
+        return [
+            self.Relation.create(
+                database=schema_relation.database,
+                schema=schema_relation.schema,
+                identifier=name,
+                type=self.Relation.get_relation_type(kind),
+                comment=comment if comment != "" else None,
+                file_format=file_format,
+                owner=owner,
+            )
+            for name, comment, kind, file_format, owner in results.select(
+                ["name", "comment", "kind", "file_format", "owner"]
+            )
+        ]
+
+    def _list_relations_with_information(
+        self, schema_relation: DatabricksRelation
+    ) -> List[Tuple[DatabricksRelation, str]]:
+        results: List[Row]
+        kwargs = {"schema_relation": schema_relation}
+        try:
+            # The catalog for `show table extended` needs to match the current catalog.
+            with self._catalog(schema_relation.database):
+                results = list(self.execute_macro(SHOW_TABLE_EXTENDED_MACRO_NAME, kwargs=kwargs))
+        except DbtRuntimeError as e:
+            errmsg = getattr(e, "msg", "")
+            if check_not_found_error(errmsg):
+                results = []
+            else:
+                description = "Error while retrieving information about"
+                logger.debug(f"{description} {schema_relation.without_identifier()}: {e.msg}")
+                raise e
 
-        relations = []
+        relations: List[Tuple[DatabricksRelation, str]] = []
         for row in results:
-            name, kind, file_format, owner = row
-            metadata = None
-            if file_format:
-                metadata = {KEY_TABLE_OWNER: owner, KEY_TABLE_PROVIDER: file_format}
-            relations.append(
-                self.Relation.create(
-                    database=schema_relation.database,
-                    schema=schema_relation.schema,
-                    identifier=name,
-                    type=self.Relation.get_relation_type(kind),
-                    metadata=metadata,
+            if len(row) != 4:
+                raise DbtRuntimeError(
+                    f'Invalid value from "show table extended ...", '
+                    f"got {len(row)} values, expected 4"
                 )
+            _schema, name, _, information = row
+            rel_type = RelationType.View if "Type: VIEW" in information else RelationType.Table
+            relation = self.Relation.create(
+                database=schema_relation.database,
+                # Use `_schema` retrieved from the cluster to avoid mismatched case
+                # between the profile and the cluster.
+                schema=_schema,
+                identifier=name,
+                type=rel_type,
             )
+            relations.append((relation, information))
 
         return relations
 
-    def get_relations_without_caching(
-        self, relation: DatabricksRelation
-    ) -> List[Tuple[Optional[str], Optional[str], Optional[str], Optional[str]]]:
+    def get_relations_without_caching(self, relation: DatabricksRelation) -> Table:
         if relation.is_hive_metastore():
             return self._get_hive_relations(relation)
         return self._get_uc_relations(relation)
 
-    def _get_uc_relations(
-        self, relation: DatabricksRelation
-    ) -> List[Tuple[Optional[str], Optional[str], Optional[str], Optional[str]]]:
+    def _get_uc_relations(self, relation: DatabricksRelation) -> Table:
         kwargs = {"relation": relation}
-        results = self.execute_macro("get_uc_tables", kwargs=kwargs)
-        return [
-            (row["table_name"], row["table_type"], row["file_format"], row["table_owner"])
-            for row in results
-        ]
+        tables = self.execute_macro("get_uc_tables", kwargs=kwargs)
+        return Table(
+            tables,
+            column_names=["name", "comment", "kind", "file_format", "owner"],
+            column_types=[Text(), Text(), Text(), Text(), Text()],
+        )
 
-    def _get_hive_relations(
-        self, relation: DatabricksRelation
-    ) -> List[Tuple[Optional[str], Optional[str], Optional[str], Optional[str]]]:
+    def _get_hive_relations(self, relation: DatabricksRelation) -> Table:
         kwargs = {"relation": relation}
 
         new_rows: List[Tuple[str, Optional[str]]]
         if all([relation.database, relation.schema]):
             tables = self.connections.list_tables(
                 database=relation.database, schema=relation.schema  # type: ignore[arg-type]
             )
 
             new_rows = []
             for row in tables:
                 # list_tables returns TABLE_TYPE as view for both materialized views and for
                 # streaming tables.  Set type to "" in this case and it will be resolved below.
-                type = row["TABLE_TYPE"].lower() if row["TABLE_TYPE"] else None
+                type = row["TABLE_TYPE"].lower() if row["TABLE_TYPE"].lower() != "view" else None
                 row = (row["TABLE_NAME"], type)
                 new_rows.append(row)
 
         else:
             tables = self.execute_macro(SHOW_TABLES_MACRO_NAME, kwargs=kwargs)
             new_rows = [(row["tableName"], None) for row in tables]
 
@@ -300,15 +318,19 @@
                 views = self.execute_macro(SHOW_VIEWS_MACRO_NAME, kwargs=kwargs)
                 view_names = set(views.columns["viewName"].values())  # type: ignore[attr-defined]
                 new_rows = [
                     (row[0], str(RelationType.View if row[0] in view_names else RelationType.Table))
                     for row in new_rows
                 ]
 
-        return [(row[0], row[1], None, None) for row in new_rows]
+        return Table(
+            [(row[0], None, row[1], None, None) for row in new_rows],
+            column_names=["name", "comment", "kind", "file_format", "owner"],
+            column_types=[Text(), Text(), Text(), Text(), Text()],
+        )
 
     def get_relation(
         self,
         database: Optional[str],
         schema: str,
         identifier: str,
         *,
@@ -320,21 +342,22 @@
 
         if not needs_information:
             return cached
 
         return self._set_relation_information(cached) if cached else None
 
     def parse_describe_extended(  # type: ignore[override]
-        self, relation: DatabricksRelation, raw_rows: List["Row"]
+        self, relation: DatabricksRelation, raw_rows: List[Row]
     ) -> Tuple[Dict[str, Any], List[DatabricksColumn]]:
         # Convert the Row to a dict
         dict_rows = [dict(zip(row._keys, row._values)) for row in raw_rows]
         # Find the separator between the rows and the metadata provided
         # by the DESCRIBE TABLE EXTENDED statement
         pos = self.find_table_information_separator(dict_rows)
+
         # Remove rows that start with a hash, they are comments
         rows = [row for row in raw_rows[0:pos] if not row["col_name"].startswith("#")]
         metadata = {col["col_name"]: col["data_type"] for col in raw_rows[pos + 1 :]}
 
         raw_table_stats = metadata.get(KEY_TABLE_STATISTICS)
         table_stats = DatabricksColumn.convert_table_stats(raw_table_stats)
         return metadata, [
@@ -353,48 +376,60 @@
             )
             for idx, column in enumerate(rows)
         ]
 
     def get_columns_in_relation(  # type: ignore[override]
         self, relation: DatabricksRelation
     ) -> List[DatabricksColumn]:
-        rows = list(
-            handle_missing_objects(
-                lambda: self.execute_macro(
-                    GET_COLUMNS_COMMENTS_MACRO_NAME, kwargs={"relation": relation}
-                ),
-                AttrDict(),
+        try:
+            rows: List[Row] = list(
+                self.execute_macro(GET_COLUMNS_COMMENTS_MACRO_NAME, kwargs={"relation": relation})
             )
-        )
-
-        columns = []
-        for row in rows:
-            if row["col_name"].startswith("#"):
-                break
-            columns.append(
-                DatabricksColumn(
-                    column=row["col_name"], dtype=row["data_type"], comment=row["comment"]
+            columns = []
+            for row in rows:
+                if row["col_name"].startswith("#"):
+                    break
+                columns.append(
+                    DatabricksColumn(
+                        column=row["col_name"], dtype=row["data_type"], comment=row["comment"]
+                    )
                 )
-            )
+        except DbtRuntimeError as e:
+            # spark would throw error when table doesn't exist, where other
+            # CDW would just return and empty list, normalizing the behavior here
+            errmsg = getattr(e, "msg", "")
+            found_msgs = (msg in errmsg for msg in TABLE_OR_VIEW_NOT_FOUND_MESSAGES)
+            if any(found_msgs):
+                columns = []
+            else:
+                raise e
 
         return columns
 
     def _get_updated_relation(
         self, relation: DatabricksRelation
     ) -> Tuple[DatabricksRelation, List[DatabricksColumn]]:
-        rows = list(
-            handle_missing_objects(
-                lambda: self.execute_macro(
+        try:
+            rows: List[Row] = list(
+                self.execute_macro(
                     GET_COLUMNS_IN_RELATION_RAW_MACRO_NAME,
                     kwargs={"relation": relation},
-                ),
-                AttrDict(),
+                )
             )
-        )
-        metadata, columns = self.parse_describe_extended(relation, rows)
+            metadata, columns = self.parse_describe_extended(relation, rows)
+        except DbtRuntimeError as e:
+            # spark would throw error when table doesn't exist, where other
+            # CDW would just return and empty list, normalizing the behavior here
+            errmsg = getattr(e, "msg", "")
+            found_msgs = (msg in errmsg for msg in TABLE_OR_VIEW_NOT_FOUND_MESSAGES)
+            if any(found_msgs):
+                metadata = None
+                columns = []
+            else:
+                raise e
 
         # strip hudi metadata columns.
         columns = [x for x in columns if x.name not in self.HUDI_METADATA_COLUMNS]
 
         return (
             self.Relation.create(
                 database=relation.database,
@@ -414,24 +449,24 @@
         return self._get_updated_relation(relation)[0]
 
     def parse_columns_from_information(  # type: ignore[override]
         self, relation: DatabricksRelation, information: str
     ) -> List[DatabricksColumn]:
         owner_match = re.findall(self.INFORMATION_OWNER_REGEX, information)
         owner = owner_match[0] if owner_match else None
-        matches = re.finditer(self.INFORMATION_COLUMNS_REGEX, information)
         comment_match = re.findall(self.INFORMATION_COMMENT_REGEX, information)
         table_comment = comment_match[0] if comment_match else None
+        matches = re.finditer(self.INFORMATION_COLUMNS_REGEX, information)
         columns = []
         stats_match = re.findall(self.INFORMATION_STATISTICS_REGEX, information)
         raw_table_stats = stats_match[0] if stats_match else None
         table_stats = DatabricksColumn.convert_table_stats(raw_table_stats)
 
         for match_num, match in enumerate(matches):
-            column_name, column_type, _ = match.groups()
+            column_name, column_type, nullable = match.groups()
             column = DatabricksColumn(
                 table_database=relation.database,
                 table_schema=relation.schema,
                 table_name=relation.table,
                 table_type=relation.type,
                 table_comment=table_comment,
                 column_index=match_num,
@@ -439,101 +474,101 @@
                 column=column_name,
                 dtype=DatabricksColumn.translate_type(column_type),
                 table_stats=table_stats,
             )
             columns.append(column)
         return columns
 
-    def get_catalog_by_relations(
-        self, used_schemas: FrozenSet[Tuple[str, str]], relations: Set[BaseRelation]
-    ) -> Tuple["Table", List[Exception]]:
-        relation_map: Dict[Tuple[str, str], Set[str]] = defaultdict(set)
-        for relation in relations:
-            if relation.identifier:
-                relation_map[
-                    (relation.database or "hive_metastore", relation.schema or "schema")
-                ].add(relation.identifier)
-
-        return self._get_catalog_for_relation_map(relation_map, used_schemas)
-
     def get_catalog(
         self,
         relation_configs: Iterable[RelationConfig],
         used_schemas: FrozenSet[Tuple[str, str]],
-    ) -> Tuple["Table", List[Exception]]:
-        relation_map: Dict[Tuple[str, str], Set[str]] = defaultdict(set)
-        for relation in relation_configs:
-            relation_map[(relation.database or "hive_metastore", relation.schema or "default")].add(
-                relation.identifier
-            )
+    ) -> Tuple[Table, List[Exception]]:  # type: ignore
+        schema_map = self._get_catalog_schemas(relation_configs)
 
-        return self._get_catalog_for_relation_map(relation_map, used_schemas)
-
-    def _get_catalog_for_relation_map(
-        self,
-        relation_map: Dict[Tuple[str, str], Set[str]],
-        used_schemas: FrozenSet[Tuple[str, str]],
-    ) -> Tuple["Table", List[Exception]]:
         with executor(self.config) as tpe:
-            futures: List[Future["Table"]] = []
-            for schema, relations in relation_map.items():
-                if schema in used_schemas:
-                    identifier = get_identifier_list_string(relations)
-                    if identifier:
+            futures: List[Future[Table]] = []
+            for info, schemas in schema_map.items():
+                if is_hive_metastore(info.database):
+                    for schema in schemas:
                         futures.append(
                             tpe.submit_connected(
                                 self,
-                                str(schema),
-                                self._get_schema_for_catalog,
-                                schema[0],
-                                schema[1],
-                                identifier,
+                                "hive_metastore",
+                                self._get_hive_catalog,
+                                schema,
+                                "*",
                             )
                         )
+                else:
+                    name = ".".join([str(info.database), "information_schema"])
+                    fut = tpe.submit_connected(
+                        self, name, self._get_one_unity_catalog, info, used_schemas
+                    )
+                    futures.append(fut)
             catalogs, exceptions = catch_as_completed(futures)
         return catalogs, exceptions
 
-    def _list_relations_with_information(
-        self, schema_relation: DatabricksRelation
-    ) -> List[Tuple[DatabricksRelation, str]]:
-        results = self._show_table_extended(schema_relation)
-
-        relations: List[Tuple[DatabricksRelation, str]] = []
-        if results:
-            for name, information in results.select(["tableName", "information"]):
-                rel_type = RelationType.View if "Type: VIEW" in information else RelationType.Table
-                relation = self.Relation.create(
-                    database=schema_relation.database.lower() if schema_relation.database else None,
-                    schema=schema_relation.schema.lower() if schema_relation.schema else None,
-                    identifier=name,
-                    type=rel_type,
-                )
-                relations.append((relation, information))
+    def _get_one_unity_catalog(
+        self, info: InformationSchema, schemas: FrozenSet[Tuple[str, str]]
+    ) -> Table:
+        kwargs = {
+            "information_schema": info,
+            "schemas": schemas,
+        }
+        table = self.execute_macro(GET_CATALOG_MACRO_NAME, kwargs=kwargs)
 
-        return relations
+        results = self._catalog_filter_table(table, schemas)
+        return results
 
-    def _show_table_extended(self, schema_relation: DatabricksRelation) -> Optional["Table"]:
-        kwargs = {"schema_relation": schema_relation}
+    def get_catalog_by_relations(
+        self, used_schemas: FrozenSet[Tuple[str, str]], relations: Set[BaseRelation]
+    ) -> Tuple[Table, List[Exception]]:
+        with executor(self.config) as tpe:
+            relations_by_catalog = self._get_catalog_relations_by_info_schema(relations)
+            futures: List[Future[Table]] = []
 
-        def exec() -> AttrDict:
-            with self._catalog(schema_relation.database):
-                return self.execute_macro(SHOW_TABLE_EXTENDED_MACRO_NAME, kwargs=kwargs)
+            for info_schema, catalog_relations in relations_by_catalog.items():
+                if is_hive_metastore(info_schema.database):
+                    schema_map = defaultdict(list)
+                    for relation in catalog_relations:
+                        schema_map[relation.schema].append(relation)
 
-        return handle_missing_objects(exec, None)
+                    for schema, schema_relations in schema_map.items():
+                        table_names = extract_identifiers(schema_relations)
+                        futures.append(
+                            tpe.submit_connected(
+                                self,
+                                "hive_metastore",
+                                self._get_hive_catalog,
+                                schema,
+                                get_identifier_list_string(table_names),
+                            )
+                        )
+                else:
+                    name = ".".join([str(info_schema.database), "information_schema"])
+                    fut = tpe.submit_connected(
+                        self,
+                        name,
+                        self._get_one_catalog_by_relations,
+                        info_schema,
+                        catalog_relations,
+                        used_schemas,
+                    )
+                    futures.append(fut)
 
-    def _get_schema_for_catalog(self, catalog: str, schema: str, identifier: str) -> "Table":
-        # Lazy load to improve startup time
-        from agate import Table
-        from dbt_common.clients.agate_helper import DEFAULT_TYPE_TESTER
+            catalogs, exceptions = catch_as_completed(futures)
+        return catalogs, exceptions
 
+    def _get_hive_catalog(self, schema: str, identifier: str) -> Table:
         columns: List[Dict[str, Any]] = []
 
         if identifier:
             schema_relation = self.Relation.create(
-                database=catalog or "hive_metastore",
+                database="hive_metastore",
                 schema=schema,
                 identifier=identifier,
                 quote_policy=self.config.quoting,
             )
             for relation, information in self._list_relations_with_information(schema_relation):
                 columns.extend(self._get_columns_for_catalog(relation, information))
         return Table.from_object(columns, column_types=DEFAULT_TYPE_TESTER)
@@ -703,33 +738,15 @@
         cls, adapter: DatabricksAdapter, relation: DatabricksRelation
     ) -> RelationResults:
         """Describe the relation and return the results."""
 
         raise NotImplementedError("Must be implemented by subclass")
 
 
-class DeltaLiveTableAPIBase(RelationAPIBase[DatabricksRelationConfig]):
-    @classmethod
-    def get_from_relation(
-        cls, adapter: DatabricksAdapter, relation: DatabricksRelation
-    ) -> DatabricksRelationConfig:
-        """Get the relation config from the relation."""
-
-        relation_config = super(DeltaLiveTableAPIBase, cls).get_from_relation(adapter, relation)
-        connection = cast(DatabricksDBTConnection, adapter.connections.get_thread_connection())
-        wrapper: DatabricksSQLConnectionWrapper = connection.handle
-
-        # Ensure any current refreshes are completed before returning the relation config
-        tblproperties = cast(TblPropertiesConfig, relation_config.config["tblproperties"])
-        if tblproperties.pipeline_id:
-            wrapper.cursor().poll_refresh_pipeline(tblproperties.pipeline_id)
-        return relation_config
-
-
-class MaterializedViewAPI(DeltaLiveTableAPIBase[MaterializedViewConfig]):
+class MaterializedViewAPI(RelationAPIBase[MaterializedViewConfig]):
     relation_type = DatabricksRelationType.MaterializedView
 
     @classmethod
     def config_type(cls) -> Type[MaterializedViewConfig]:
         return MaterializedViewConfig
 
     @classmethod
@@ -744,22 +761,22 @@
 
         kwargs = {"relation": relation}
         results["information_schema.views"] = cls._get_information_schema_views(adapter, kwargs)
         results["show_tblproperties"] = adapter.execute_macro("fetch_tbl_properties", kwargs=kwargs)
         return results
 
     @staticmethod
-    def _get_information_schema_views(adapter: DatabricksAdapter, kwargs: Dict[str, Any]) -> "Row":
+    def _get_information_schema_views(adapter: DatabricksAdapter, kwargs: Dict[str, Any]) -> Row:
         row = get_first_row(adapter.execute_macro("get_view_description", kwargs=kwargs))
         if "view_definition" in row.keys() and row["view_definition"] is not None:
             return row
         return get_first_row(adapter.execute_macro("get_view_description_alt", kwargs=kwargs))
 
 
-class StreamingTableAPI(DeltaLiveTableAPIBase[StreamingTableConfig]):
+class StreamingTableAPI(RelationAPIBase[StreamingTableConfig]):
     relation_type = DatabricksRelationType.StreamingTable
 
     @classmethod
     def config_type(cls) -> Type[StreamingTableConfig]:
         return StreamingTableConfig
 
     @classmethod
```

### Comparing `dbt-databricks-1.8.1b2/dbt/adapters/databricks/logging.py` & `dbt-databricks-2.0.0rc1/dbt/adapters/databricks/logging.py`

 * *Files identical despite different names*

### Comparing `dbt-databricks-1.8.1b2/dbt/adapters/databricks/python_submissions.py` & `dbt-databricks-2.0.0rc1/dbt/adapters/databricks/python_submissions.py`

 * *Files identical despite different names*

### Comparing `dbt-databricks-1.8.1b2/dbt/adapters/databricks/relation.py` & `dbt-databricks-2.0.0rc1/dbt/adapters/databricks/relation.py`

 * *Files 2% similar despite different names*

```diff
@@ -39,15 +39,15 @@
 
 
 class DatabricksRelationType(StrEnum):
     Table = "table"
     View = "view"
     CTE = "cte"
     MaterializedView = "materialized_view"
-    Foreign = "foreign"
+    External = "external"
     StreamingTable = "streaming_table"
     Unknown = "unknown"
 
 
 @dataclass(frozen=True, eq=False, repr=False)
 class DatabricksInformationSchema(InformationSchema):
     quote_policy: Policy = field(default_factory=lambda: DatabricksQuotePolicy())
```

### Comparing `dbt-databricks-1.8.1b2/dbt/adapters/databricks/relation_configs/base.py` & `dbt-databricks-2.0.0rc1/dbt/adapters/databricks/relation_configs/base.py`

 * *Files identical despite different names*

### Comparing `dbt-databricks-1.8.1b2/dbt/adapters/databricks/relation_configs/comment.py` & `dbt-databricks-2.0.0rc1/dbt/adapters/databricks/relation_configs/comment.py`

 * *Files 6% similar despite different names*

```diff
@@ -17,19 +17,13 @@
     name: ClassVar[str] = "comment"
 
     @classmethod
     def from_relation_results(cls, results: RelationResults) -> CommentConfig:
         table = results["describe_extended"]
         for row in table.rows:
             if row[0] == "Comment":
-                if row[1]:
-                    return CommentConfig(comment=row[1])
-                else:
-                    return CommentConfig()
+                return CommentConfig(comment=row[1])
         return CommentConfig()
 
     @classmethod
     def from_relation_config(cls, relation_config: RelationConfig) -> CommentConfig:
-        comment = getattr(relation_config, "description", None)
-        if comment:
-            return CommentConfig(comment=comment)
-        return CommentConfig()
+        return CommentConfig(comment=getattr(relation_config, "description"))
```

### Comparing `dbt-databricks-1.8.1b2/dbt/adapters/databricks/relation_configs/incremental.py` & `dbt-databricks-2.0.0rc1/dbt/adapters/databricks/relation_configs/incremental.py`

 * *Files identical despite different names*

### Comparing `dbt-databricks-1.8.1b2/dbt/adapters/databricks/relation_configs/materialized_view.py` & `dbt-databricks-2.0.0rc1/dbt/adapters/databricks/relation_configs/materialized_view.py`

 * *Files identical despite different names*

### Comparing `dbt-databricks-1.8.1b2/dbt/adapters/databricks/relation_configs/partitioning.py` & `dbt-databricks-2.0.0rc1/dbt/adapters/databricks/relation_configs/partitioning.py`

 * *Files identical despite different names*

### Comparing `dbt-databricks-1.8.1b2/dbt/adapters/databricks/relation_configs/query.py` & `dbt-databricks-2.0.0rc1/dbt/adapters/databricks/relation_configs/query.py`

 * *Files identical despite different names*

### Comparing `dbt-databricks-1.8.1b2/dbt/adapters/databricks/relation_configs/refresh.py` & `dbt-databricks-2.0.0rc1/dbt/adapters/databricks/relation_configs/refresh.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,17 +1,18 @@
 import re
 from typing import ClassVar
 from typing import Optional
 
+from dbt_common.exceptions import DbtRuntimeError
+
 from dbt.adapters.contracts.relation import RelationConfig
 from dbt.adapters.databricks.relation_configs import base
 from dbt.adapters.databricks.relation_configs.base import DatabricksComponentConfig
 from dbt.adapters.databricks.relation_configs.base import DatabricksComponentProcessor
 from dbt.adapters.relation_configs.config_base import RelationResults
-from dbt_common.exceptions import DbtRuntimeError
 
 SCHEDULE_REGEX = re.compile(r"CRON '(.*)' AT TIME ZONE '(.*)'")
 
 
 class RefreshConfig(DatabricksComponentConfig):
     """Component encapsulating the refresh schedule of a relation."""
```

### Comparing `dbt-databricks-1.8.1b2/dbt/adapters/databricks/relation_configs/streaming_table.py` & `dbt-databricks-2.0.0rc1/dbt/adapters/databricks/relation_configs/streaming_table.py`

 * *Files identical despite different names*

### Comparing `dbt-databricks-1.8.1b2/dbt/adapters/databricks/relation_configs/tags.py` & `dbt-databricks-2.0.0rc1/dbt/adapters/databricks/relation_configs/tags.py`

 * *Files identical despite different names*

### Comparing `dbt-databricks-1.8.1b2/dbt/adapters/databricks/relation_configs/tblproperties.py` & `dbt-databricks-2.0.0rc1/dbt/adapters/databricks/relation_configs/tblproperties.py`

 * *Files 26% similar despite different names*

```diff
@@ -1,26 +1,25 @@
 from typing import Any
 from typing import ClassVar
 from typing import Dict
 from typing import List
-from typing import Optional
+
+from dbt_common.exceptions import DbtRuntimeError
 
 from dbt.adapters.contracts.relation import RelationConfig
 from dbt.adapters.databricks.relation_configs import base
 from dbt.adapters.databricks.relation_configs.base import DatabricksComponentConfig
 from dbt.adapters.databricks.relation_configs.base import DatabricksComponentProcessor
 from dbt.adapters.relation_configs.config_base import RelationResults
-from dbt_common.exceptions import DbtRuntimeError
 
 
 class TblPropertiesConfig(DatabricksComponentConfig):
     """Component encapsulating the tblproperties of a relation."""
 
     tblproperties: Dict[str, str]
-    pipeline_id: Optional[str] = None
 
     # List of tblproperties that should be ignored when comparing configs. These are generally
     # set by Databricks and are not user-configurable.
     ignore_list: List[str] = [
         "pipelines.pipelineId",
         "delta.enableChangeDataFeed",
         "delta.minReaderVersion",
@@ -47,23 +46,20 @@
 class TblPropertiesProcessor(DatabricksComponentProcessor[TblPropertiesConfig]):
     name: ClassVar[str] = "tblproperties"
 
     @classmethod
     def from_relation_results(cls, results: RelationResults) -> TblPropertiesConfig:
         table = results.get("show_tblproperties")
         tblproperties = dict()
-        pipeline_id = None
 
         if table:
             for row in table.rows:
-                if str(row[0]) == "pipelines.pipelineId":
-                    pipeline_id = str(row[1])
                 tblproperties[str(row[0])] = str(row[1])
 
-        return TblPropertiesConfig(tblproperties=tblproperties, pipeline_id=pipeline_id)
+        return TblPropertiesConfig(tblproperties=tblproperties)
 
     @classmethod
     def from_relation_config(cls, relation_config: RelationConfig) -> TblPropertiesConfig:
         tblproperties = base.get_config_value(relation_config, "tblproperties")
         if not tblproperties:
             return TblPropertiesConfig(tblproperties=dict())
         if isinstance(tblproperties, Dict):
```

### Comparing `dbt-databricks-1.8.1b2/dbt/adapters/databricks/utils.py` & `dbt-databricks-2.0.0rc1/dbt/adapters/databricks/utils.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,22 +1,20 @@
 import functools
 import inspect
 import re
 from typing import Any
 from typing import Callable
 from typing import Type
-from typing import TYPE_CHECKING
 from typing import TypeVar
 
-from dbt.adapters.base import BaseAdapter
-from jinja2 import Undefined
+from agate import Row
+from agate import Table
+from jinja2.runtime import Undefined
 
-if TYPE_CHECKING:
-    from agate import Row
-    from agate import Table
+from dbt.adapters.base import BaseAdapter
 
 
 A = TypeVar("A", bound=BaseAdapter)
 
 
 CREDENTIAL_IN_COPY_INTO_REGEX = re.compile(
     r"(?<=credential)\s*?\((\s*?'\w*?'\s*?=\s*?'.*?'\s*?(?:,\s*?'\w*?'\s*?=\s*?'.*?'\s*?)*?)\)"
@@ -83,14 +81,11 @@
 
 
 def remove_ansi(line: str) -> str:
     ansi_escape = re.compile(r"(?:\x1B[@-_]|[\x80-\x9F])[0-?]*[ -/]*[@-~]")
     return ansi_escape.sub("", line)
 
 
-def get_first_row(results: "Table") -> "Row":
+def get_first_row(results: Table) -> Row:
     if len(results.rows) == 0:
-        # Lazy load to improve CLI startup time
-        from agate import Row
-
         return Row(values=set())
     return results.rows[0]
```

### Comparing `dbt-databricks-1.8.1b2/dbt/include/databricks/macros/adapters/catalog.sql` & `dbt-databricks-2.0.0rc1/dbt/include/databricks/macros/adapters/catalog.sql`

 * *Files 5% similar despite different names*

```diff
@@ -33,15 +33,15 @@
 {%- endmacro %}
 
 {% macro databricks__get_catalog_tables_sql(information_schema) -%}
     select
         table_catalog as table_database,
         table_schema,
         table_name,
-        lower(table_type) as table_type,
+        lower(if(table_type in ('MANAGED', 'EXTERNAL'), 'table', table_type)) as table_type,
         comment as table_comment,
         table_owner,
         'Last Modified' as `stats:last_modified:label`,
         last_altered as `stats:last_modified:value`,
         'The timestamp for last update/change' as `stats:last_modified:description`,
         (last_altered is not null and table_type not ilike '%VIEW%') as `stats:last_modified:include`
     from {{ information_schema }}.tables
```

### Comparing `dbt-databricks-1.8.1b2/dbt/include/databricks/macros/adapters/copy_into.sql` & `dbt-databricks-2.0.0rc1/dbt/include/databricks/macros/adapters/copy_into.sql`

 * *Files identical despite different names*

### Comparing `dbt-databricks-1.8.1b2/dbt/include/databricks/macros/adapters/databricks_catalog.sql` & `dbt-databricks-2.0.0rc1/dbt/include/databricks/macros/adapters/databricks_catalog.sql`

 * *Files identical despite different names*

### Comparing `dbt-databricks-1.8.1b2/dbt/include/databricks/macros/adapters/metadata.sql` & `dbt-databricks-2.0.0rc1/dbt/include/databricks/macros/adapters/metadata.sql`

 * *Files 20% similar despite different names*

```diff
@@ -90,19 +90,57 @@
       and table_schema = '{{ relation.schema }}'
       and table_name = '{{ relation.identifier }}'
   {% endcall %}
 
   {% do return(load_result('get_view_description_alt').table) %}
 {% endmacro %}
 
+
+{% macro get_uc_tables_with_columns(relation) %}
+  {% call statement('get_uc_tables_with_columns', fetch_result=True) -%}
+    with tables as (
+      select
+        table_name,
+        comment,
+        if(table_type = 'EXTERNAL' or table_type = 'MANAGED', 'table', lower(table_type)) as table_type,
+        lower(data_source_format) as file_format,
+        table_owner
+      from `{{ relation.database }}`.`information_schema`.`tables`
+      where table_schema = '{{ relation.schema }}'
+      {% if relation.identifier %}
+        and table_name = '{{ relation.identifier }}'
+      {% endif %}
+    ),
+    columns as (
+      select
+        table_name,
+        to_json(collect_list(array(column_name, data_type, comment))) as columns
+      from `{{ relation.database }}`.`information_schema`.`columns`
+      where table_schema = '{{ relation.schema }}'
+      {% if relation.identifier %}
+        and table_name = '{{ relation.identifier }}'
+      {% endif %}
+      group by table_name
+    )
+    select
+      tables.*,
+      columns.columns
+    from tables
+    left join columns using(table_name)
+  {% endcall %}
+
+  {% do return(load_result('get_uc_tables_with_columns').table) %}
+{% endmacro %}
+
 {% macro get_uc_tables(relation) %}
   {% call statement('get_uc_tables', fetch_result=True) -%}
     select
       table_name,
-      if(table_type in ('EXTERNAL', 'MANAGED', 'MANAGED_SHALLOW_CLONE'), 'table', lower(table_type)) as table_type,
+      comment,
+      if(table_type = 'EXTERNAL' or table_type = 'MANAGED', 'table', lower(table_type)) as table_type,
       lower(data_source_format) as file_format,
       table_owner
     from `{{ relation.database }}`.`information_schema`.`tables`
     where table_schema = '{{ relation.schema }}'
     {% if relation.identifier %}
       and table_name = '{{ relation.identifier }}'
     {% endif %}
```

### Comparing `dbt-databricks-1.8.1b2/dbt/include/databricks/macros/adapters/persist_docs.sql` & `dbt-databricks-2.0.0rc1/dbt/include/databricks/macros/adapters/persist_docs.sql`

 * *Files identical despite different names*

### Comparing `dbt-databricks-1.8.1b2/dbt/include/databricks/macros/adapters/python.sql` & `dbt-databricks-2.0.0rc1/dbt/include/databricks/macros/adapters/python.sql`

 * *Files 8% similar despite different names*

```diff
@@ -51,15 +51,14 @@
 # merged in using a SQL statement.  To see your incremental config in action,
 # look in the dbt.log
 
 {%- macro py_get_writer_options() -%}
 {%- set location_root = config.get('location_root', validator=validation.any[basestring]) -%}
 {%- set file_format = config.get('file_format', validator=validation.any[basestring])|default('delta', true) -%}
 {%- set partition_by = config.get('partition_by', validator=validation.any[list, basestring]) -%}
-{%- set liquid_clustered_by = config.get('liquid_clustered_by', validator=validation.any[list, basestring]) -%}
 {%- set clustered_by = config.get('clustered_by', validator=validation.any[list, basestring]) -%}
 {%- set buckets = config.get('buckets', validator=validation.any[int]) -%}
 .format("{{ file_format }}")
 {%- if location_root is not none %}
 {%- set identifier = model['alias'] %}
 {%- if is_incremental() %}
 {%- set identifier = identifier + '__dbt_tmp' %}
@@ -68,20 +67,14 @@
 {%- endif -%}
 {%- if partition_by is not none -%}
     {%- if partition_by is string -%}
         {%- set partition_by = [partition_by] -%}
     {%- endif %}
 .partitionBy({{ partition_by }})
 {%- endif -%}
-{%- if liquid_clustered_by -%}
-    {%- if liquid_clustered_by is string -%}
-        {%- set liquid_clustered_by = [liquid_clustered_by] -%}
-    {%- endif %}
-.clusterBy({{ liquid_clustered_by }})
-{%- endif -%}
 {%- if (clustered_by is not none) and (buckets is not none) -%}
     {%- if clustered_by is string -%}
         {%- set clustered_by = [clustered_by] -%}
     {%- endif %}
 .bucketBy({{ buckets }}, {{ clustered_by }})
 {%- endif -%}
 {% endmacro -%}
```

### Comparing `dbt-databricks-1.8.1b2/dbt/include/databricks/macros/adapters/relation.sql` & `dbt-databricks-2.0.0rc1/dbt/include/databricks/macros/adapters/relation.sql`

 * *Files identical despite different names*

### Comparing `dbt-databricks-1.8.1b2/dbt/include/databricks/macros/etc/statement.sql` & `dbt-databricks-2.0.0rc1/dbt/include/databricks/macros/etc/statement.sql`

 * *Files identical despite different names*

### Comparing `dbt-databricks-1.8.1b2/dbt/include/databricks/macros/materializations/clone.sql` & `dbt-databricks-2.0.0rc1/dbt/include/databricks/macros/materializations/clone.sql`

 * *Files identical despite different names*

### Comparing `dbt-databricks-1.8.1b2/dbt/include/databricks/macros/materializations/incremental/incremental.sql` & `dbt-databricks-2.0.0rc1/dbt/include/databricks/macros/materializations/incremental/incremental.sql`

 * *Files identical despite different names*

### Comparing `dbt-databricks-1.8.1b2/dbt/include/databricks/macros/materializations/incremental/strategies.sql` & `dbt-databricks-2.0.0rc1/dbt/include/databricks/macros/materializations/incremental/strategies.sql`

 * *Files identical despite different names*

### Comparing `dbt-databricks-1.8.1b2/dbt/include/databricks/macros/materializations/incremental/validate.sql` & `dbt-databricks-2.0.0rc1/dbt/include/databricks/macros/materializations/incremental/validate.sql`

 * *Files identical despite different names*

### Comparing `dbt-databricks-1.8.1b2/dbt/include/databricks/macros/materializations/materialized_view.sql` & `dbt-databricks-2.0.0rc1/dbt/include/databricks/macros/materializations/materialized_view.sql`

 * *Files identical despite different names*

### Comparing `dbt-databricks-1.8.1b2/dbt/include/databricks/macros/materializations/seeds/seeds.sql` & `dbt-databricks-2.0.0rc1/dbt/include/databricks/macros/materializations/seeds/seeds.sql`

 * *Files 4% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 {% materialization seed, adapter='databricks' %}
 
   {%- set identifier = model['alias'] -%}
   {%- set full_refresh_mode = (should_full_refresh()) -%}
 
-  {%- set old_relation = adapter.get_relation(database=database, schema=schema, identifier=identifier, needs_information=True) -%}
+  {%- set old_relation = adapter.get_relation(database=database, schema=schema, identifier=identifier) -%}
 
   {%- set exists_as_table = (old_relation is not none and old_relation.is_table) -%}
   {%- set exists_as_view = (old_relation is not none and (old_relation.is_view or old_relation.is_materialized_view)) -%}
   {%- set exists_as_streaming_table = (old_relation is not none and old_relation.is_streaming_table) -%}
 
   {%- set grant_config = config.get('grants') -%}
   {%- set agate_table = load_agate_table() -%}
@@ -40,15 +40,16 @@
     {{ get_csv_sql(create_table_sql, sql) }};
   {% endcall %}
 
   {% set target_relation = this.incorporate(type='table') %}
 
   {% set should_revoke = should_revoke(old_relation, full_refresh_mode) %}
   {% do apply_grants(target_relation, grant_config, should_revoke=should_revoke) %}
-  -- No need to persist docs, already handled in seed create
+
+  {% do persist_docs(target_relation, model) %}
 
   {% if full_refresh_mode or not exists_as_table %}
     {% do create_indexes(target_relation) %}
   {% endif %}
 
   {{ run_hooks(post_hooks, inside_transaction=True) }}
```

### Comparing `dbt-databricks-1.8.1b2/dbt/include/databricks/macros/materializations/snapshot.sql` & `dbt-databricks-2.0.0rc1/dbt/include/databricks/macros/materializations/snapshot.sql`

 * *Files identical despite different names*

### Comparing `dbt-databricks-1.8.1b2/dbt/include/databricks/macros/materializations/streaming_table.sql` & `dbt-databricks-2.0.0rc1/dbt/include/databricks/macros/materializations/streaming_table.sql`

 * *Files identical despite different names*

### Comparing `dbt-databricks-1.8.1b2/dbt/include/databricks/macros/materializations/table.sql` & `dbt-databricks-2.0.0rc1/dbt/include/databricks/macros/materializations/table.sql`

 * *Files identical despite different names*

### Comparing `dbt-databricks-1.8.1b2/dbt/include/databricks/macros/materializations/view.sql` & `dbt-databricks-2.0.0rc1/dbt/include/databricks/macros/materializations/view.sql`

 * *Files identical despite different names*

### Comparing `dbt-databricks-1.8.1b2/dbt/include/databricks/macros/relations/components/refresh_schedule.sql` & `dbt-databricks-2.0.0rc1/dbt/include/databricks/macros/relations/components/refresh_schedule.sql`

 * *Files identical despite different names*

### Comparing `dbt-databricks-1.8.1b2/dbt/include/databricks/macros/relations/constraints.sql` & `dbt-databricks-2.0.0rc1/dbt/include/databricks/macros/relations/constraints.sql`

 * *Files identical despite different names*

### Comparing `dbt-databricks-1.8.1b2/dbt/include/databricks/macros/relations/create.sql` & `dbt-databricks-2.0.0rc1/dbt/include/databricks/macros/relations/create.sql`

 * *Files identical despite different names*

### Comparing `dbt-databricks-1.8.1b2/dbt/include/databricks/macros/relations/drop.sql` & `dbt-databricks-2.0.0rc1/dbt/include/databricks/macros/relations/drop.sql`

 * *Files identical despite different names*

### Comparing `dbt-databricks-1.8.1b2/dbt/include/databricks/macros/relations/location.sql` & `dbt-databricks-2.0.0rc1/dbt/include/databricks/macros/relations/location.sql`

 * *Files identical despite different names*

### Comparing `dbt-databricks-1.8.1b2/dbt/include/databricks/macros/relations/materialized_view/alter.sql` & `dbt-databricks-2.0.0rc1/dbt/include/databricks/macros/relations/materialized_view/alter.sql`

 * *Files identical despite different names*

### Comparing `dbt-databricks-1.8.1b2/dbt/include/databricks/macros/relations/materialized_view/create.sql` & `dbt-databricks-2.0.0rc1/dbt/include/databricks/macros/relations/materialized_view/create.sql`

 * *Files identical despite different names*

### Comparing `dbt-databricks-1.8.1b2/dbt/include/databricks/macros/relations/optimize.sql` & `dbt-databricks-2.0.0rc1/dbt/include/databricks/macros/relations/optimize.sql`

 * *Files identical despite different names*

### Comparing `dbt-databricks-1.8.1b2/dbt/include/databricks/macros/relations/replace.sql` & `dbt-databricks-2.0.0rc1/dbt/include/databricks/macros/relations/replace.sql`

 * *Files identical despite different names*

### Comparing `dbt-databricks-1.8.1b2/dbt/include/databricks/macros/relations/streaming_table/alter.sql` & `dbt-databricks-2.0.0rc1/dbt/include/databricks/macros/relations/streaming_table/alter.sql`

 * *Files identical despite different names*

### Comparing `dbt-databricks-1.8.1b2/dbt/include/databricks/macros/relations/streaming_table/create.sql` & `dbt-databricks-2.0.0rc1/dbt/include/databricks/macros/relations/streaming_table/create.sql`

 * *Files identical despite different names*

### Comparing `dbt-databricks-1.8.1b2/dbt/include/databricks/macros/relations/table/create.sql` & `dbt-databricks-2.0.0rc1/dbt/include/databricks/macros/relations/table/create.sql`

 * *Files identical despite different names*

### Comparing `dbt-databricks-1.8.1b2/dbt/include/databricks/macros/relations/tags.sql` & `dbt-databricks-2.0.0rc1/dbt/include/databricks/macros/relations/tags.sql`

 * *Files identical despite different names*

### Comparing `dbt-databricks-1.8.1b2/dbt/include/databricks/macros/relations/tblproperties.sql` & `dbt-databricks-2.0.0rc1/dbt/include/databricks/macros/relations/tblproperties.sql`

 * *Files identical despite different names*

### Comparing `dbt-databricks-1.8.1b2/dbt/include/databricks/macros/relations/view/create.sql` & `dbt-databricks-2.0.0rc1/dbt/include/databricks/macros/relations/view/create.sql`

 * *Files identical despite different names*

### Comparing `dbt-databricks-1.8.1b2/dbt/include/databricks/profile_template.yml` & `dbt-databricks-2.0.0rc1/dbt/include/databricks/profile_template.yml`

 * *Files identical despite different names*

### Comparing `dbt-databricks-1.8.1b2/dbt_databricks.egg-info/PKG-INFO` & `dbt-databricks-2.0.0rc1/dbt_databricks.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: dbt-databricks
-Version: 1.8.1b2
+Version: 2.0.0rc1
 Summary: The Databricks adapter plugin for dbt
 Home-page: https://github.com/databricks/dbt-databricks
 Author: Databricks
 Author-email: feedback@databricks.com
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Operating System :: Microsoft :: Windows
```

### Comparing `dbt-databricks-1.8.1b2/dbt_databricks.egg-info/SOURCES.txt` & `dbt-databricks-2.0.0rc1/dbt_databricks.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `dbt-databricks-1.8.1b2/setup.py` & `dbt-databricks-2.0.0rc1/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -50,16 +50,16 @@
     long_description_content_type="text/markdown",
     author="Databricks",
     author_email="feedback@databricks.com",
     url="https://github.com/databricks/dbt-databricks",
     packages=find_namespace_packages(include=["dbt", "dbt.*"]),
     include_package_data=True,
     install_requires=[
-        "dbt-spark~=1.8.0",
-        "dbt-core~=1.8.0",
+        "dbt-spark~=1.8.0rc1",
+        "dbt-core~=1.8.0rc2",
         "dbt-adapters~=1.1.1",
         "databricks-sql-connector>=3.1.0, <3.2.0",
         "databricks-sdk==0.17.0",
         "keyring>=23.13.0",
         "pandas<2.2.0",
         "protobuf<5.0.0",
     ],
```

