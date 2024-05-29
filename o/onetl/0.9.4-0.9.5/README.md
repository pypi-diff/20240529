# Comparing `tmp/onetl-0.9.4.tar.gz` & `tmp/onetl-0.9.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "onetl-0.9.4.tar", last modified: Tue Sep 26 12:34:22 2023, max compression
+gzip compressed data, was "onetl-0.9.5.tar", last modified: Tue Oct 10 11:38:46 2023, max compression
```

## Comparing `onetl-0.9.4.tar` & `onetl-0.9.5.tar`

### file list

```diff
@@ -1,304 +1,306 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-09-26 12:34:22.234914 onetl-0.9.4/
--rw-r--r--   0 runner    (1001) docker     (127)    11421 2023-09-26 12:33:49.000000 onetl-0.9.4/LICENSE.txt
--rw-r--r--   0 runner    (1001) docker     (127)      257 2023-09-26 12:33:49.000000 onetl-0.9.4/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (127)    28903 2023-09-26 12:34:22.234914 onetl-0.9.4/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)    25793 2023-09-26 12:33:49.000000 onetl-0.9.4/README.rst
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-09-26 12:34:22.182914 onetl-0.9.4/onetl/
--rw-r--r--   0 runner    (1001) docker     (127)        6 2023-09-26 12:33:49.000000 onetl-0.9.4/onetl/VERSION
--rw-r--r--   0 runner    (1001) docker     (127)     1301 2023-09-26 12:33:49.000000 onetl-0.9.4/onetl/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     5860 2023-09-26 12:33:49.000000 onetl-0.9.4/onetl/_internal.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-09-26 12:34:22.182914 onetl-0.9.4/onetl/_util/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2023-09-26 12:33:49.000000 onetl-0.9.4/onetl/_util/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1080 2023-09-26 12:33:49.000000 onetl-0.9.4/onetl/_util/classproperty.py
--rw-r--r--   0 runner    (1001) docker     (127)     1665 2023-09-26 12:33:49.000000 onetl-0.9.4/onetl/_util/file.py
--rw-r--r--   0 runner    (1001) docker     (127)     1320 2023-09-26 12:33:49.000000 onetl-0.9.4/onetl/_util/hadoop.py
--rw-r--r--   0 runner    (1001) docker     (127)     1224 2023-09-26 12:33:49.000000 onetl-0.9.4/onetl/_util/java.py
--rw-r--r--   0 runner    (1001) docker     (127)      904 2023-09-26 12:33:49.000000 onetl-0.9.4/onetl/_util/scala.py
--rw-r--r--   0 runner    (1001) docker     (127)     4747 2023-09-26 12:33:49.000000 onetl-0.9.4/onetl/_util/spark.py
--rw-r--r--   0 runner    (1001) docker     (127)     5511 2023-09-26 12:33:49.000000 onetl-0.9.4/onetl/_util/version.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-09-26 12:34:22.186914 onetl-0.9.4/onetl/base/
--rw-r--r--   0 runner    (1001) docker     (127)     1568 2023-09-26 12:33:49.000000 onetl-0.9.4/onetl/base/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1167 2023-09-26 12:33:49.000000 onetl-0.9.4/onetl/base/base_connection.py
--rw-r--r--   0 runner    (1001) docker     (127)     5070 2023-09-26 12:33:49.000000 onetl-0.9.4/onetl/base/base_db_connection.py
--rw-r--r--   0 runner    (1001) docker     (127)    19414 2023-09-26 12:33:49.000000 onetl-0.9.4/onetl/base/base_file_connection.py
--rw-r--r--   0 runner    (1001) docker     (127)     4064 2023-09-26 12:33:49.000000 onetl-0.9.4/onetl/base/base_file_df_connection.py
--rw-r--r--   0 runner    (1001) docker     (127)     1466 2023-09-26 12:33:49.000000 onetl-0.9.4/onetl/base/base_file_filter.py
--rw-r--r--   0 runner    (1001) docker     (127)     2848 2023-09-26 12:33:49.000000 onetl-0.9.4/onetl/base/base_file_format.py
--rw-r--r--   0 runner    (1001) docker     (127)     3120 2023-09-26 12:33:49.000000 onetl-0.9.4/onetl/base/base_file_limit.py
--rw-r--r--   0 runner    (1001) docker     (127)      907 2023-09-26 12:33:49.000000 onetl-0.9.4/onetl/base/contains_exception.py
--rw-r--r--   0 runner    (1001) docker     (127)     1151 2023-09-26 12:33:49.000000 onetl-0.9.4/onetl/base/contains_get_df_schema.py
--rw-r--r--   0 runner    (1001) docker     (127)     1179 2023-09-26 12:33:49.000000 onetl-0.9.4/onetl/base/contains_get_min_max_bounds.py
--rw-r--r--   0 runner    (1001) docker     (127)     1713 2023-09-26 12:33:49.000000 onetl-0.9.4/onetl/base/path_protocol.py
--rw-r--r--   0 runner    (1001) docker     (127)     1468 2023-09-26 12:33:49.000000 onetl-0.9.4/onetl/base/path_stat_protocol.py
--rw-r--r--   0 runner    (1001) docker     (127)     2380 2023-09-26 12:33:49.000000 onetl-0.9.4/onetl/base/pure_path_protocol.py
--rw-r--r--   0 runner    (1001) docker     (127)     1092 2023-09-26 12:33:49.000000 onetl-0.9.4/onetl/base/supports_rename_dir.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-09-26 12:34:22.186914 onetl-0.9.4/onetl/connection/
--rw-r--r--   0 runner    (1001) docker     (127)     3479 2023-09-26 12:33:49.000000 onetl-0.9.4/onetl/connection/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-09-26 12:34:22.186914 onetl-0.9.4/onetl/connection/db_connection/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2023-09-26 12:33:49.000000 onetl-0.9.4/onetl/connection/db_connection/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-09-26 12:34:22.186914 onetl-0.9.4/onetl/connection/db_connection/clickhouse/
--rw-r--r--   0 runner    (1001) docker     (127)      785 2023-09-26 12:33:49.000000 onetl-0.9.4/onetl/connection/db_connection/clickhouse/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     5706 2023-09-26 12:33:49.000000 onetl-0.9.4/onetl/connection/db_connection/clickhouse/connection.py
--rw-r--r--   0 runner    (1001) docker     (127)     1468 2023-09-26 12:33:49.000000 onetl-0.9.4/onetl/connection/db_connection/clickhouse/dialect.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-09-26 12:34:22.190914 onetl-0.9.4/onetl/connection/db_connection/db_connection/
--rw-r--r--   0 runner    (1001) docker     (127)      755 2023-09-26 12:33:49.000000 onetl-0.9.4/onetl/connection/db_connection/db_connection/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1876 2023-09-26 12:33:49.000000 onetl-0.9.4/onetl/connection/db_connection/db_connection/connection.py
--rw-r--r--   0 runner    (1001) docker     (127)     3952 2023-09-26 12:33:49.000000 onetl-0.9.4/onetl/connection/db_connection/db_connection/dialect.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-09-26 12:34:22.190914 onetl-0.9.4/onetl/connection/db_connection/dialect_mixins/
--rw-r--r--   0 runner    (1001) docker     (127)     1412 2023-09-26 12:33:49.000000 onetl-0.9.4/onetl/connection/db_connection/dialect_mixins/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      354 2023-09-26 12:33:49.000000 onetl-0.9.4/onetl/connection/db_connection/dialect_mixins/support_columns_list.py
--rw-r--r--   0 runner    (1001) docker     (127)      396 2023-09-26 12:33:49.000000 onetl-0.9.4/onetl/connection/db_connection/dialect_mixins/support_columns_none.py
--rw-r--r--   0 runner    (1001) docker     (127)      481 2023-09-26 12:33:49.000000 onetl-0.9.4/onetl/connection/db_connection/dialect_mixins/support_df_schema_none.py
--rw-r--r--   0 runner    (1001) docker     (127)      511 2023-09-26 12:33:49.000000 onetl-0.9.4/onetl/connection/db_connection/dialect_mixins/support_df_schema_struct.py
--rw-r--r--   0 runner    (1001) docker     (127)      380 2023-09-26 12:33:49.000000 onetl-0.9.4/onetl/connection/db_connection/dialect_mixins/support_hint_none.py
--rw-r--r--   0 runner    (1001) docker     (127)      555 2023-09-26 12:33:49.000000 onetl-0.9.4/onetl/connection/db_connection/dialect_mixins/support_hint_str.py
--rw-r--r--   0 runner    (1001) docker     (127)      515 2023-09-26 12:33:49.000000 onetl-0.9.4/onetl/connection/db_connection/dialect_mixins/support_hwm_column_str.py
--rw-r--r--   0 runner    (1001) docker     (127)      439 2023-09-26 12:33:49.000000 onetl-0.9.4/onetl/connection/db_connection/dialect_mixins/support_hwm_expression_none.py
--rw-r--r--   0 runner    (1001) docker     (127)      558 2023-09-26 12:33:49.000000 onetl-0.9.4/onetl/connection/db_connection/dialect_mixins/support_hwm_expression_str.py
--rw-r--r--   0 runner    (1001) docker     (127)      251 2023-09-26 12:33:49.000000 onetl-0.9.4/onetl/connection/db_connection/dialect_mixins/support_name_any.py
--rw-r--r--   0 runner    (1001) docker     (127)      427 2023-09-26 12:33:49.000000 onetl-0.9.4/onetl/connection/db_connection/dialect_mixins/support_name_with_schema_only.py
--rw-r--r--   0 runner    (1001) docker     (127)      984 2023-09-26 12:33:49.000000 onetl-0.9.4/onetl/connection/db_connection/dialect_mixins/support_where_none.py
--rw-r--r--   0 runner    (1001) docker     (127)      563 2023-09-26 12:33:49.000000 onetl-0.9.4/onetl/connection/db_connection/dialect_mixins/support_where_str.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-09-26 12:34:22.194914 onetl-0.9.4/onetl/connection/db_connection/greenplum/
--rw-r--r--   0 runner    (1001) docker     (127)      902 2023-09-26 12:33:49.000000 onetl-0.9.4/onetl/connection/db_connection/greenplum/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    20429 2023-09-26 12:33:49.000000 onetl-0.9.4/onetl/connection/db_connection/greenplum/connection.py
--rw-r--r--   0 runner    (1001) docker     (127)     1271 2023-09-26 12:33:49.000000 onetl-0.9.4/onetl/connection/db_connection/greenplum/connection_limit.py
--rw-r--r--   0 runner    (1001) docker     (127)     1525 2023-09-26 12:33:49.000000 onetl-0.9.4/onetl/connection/db_connection/greenplum/dialect.py
--rw-r--r--   0 runner    (1001) docker     (127)    10152 2023-09-26 12:33:49.000000 onetl-0.9.4/onetl/connection/db_connection/greenplum/options.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-09-26 12:34:22.194914 onetl-0.9.4/onetl/connection/db_connection/hive/
--rw-r--r--   0 runner    (1001) docker     (127)      928 2023-09-26 12:33:49.000000 onetl-0.9.4/onetl/connection/db_connection/hive/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    19727 2023-09-26 12:33:49.000000 onetl-0.9.4/onetl/connection/db_connection/hive/connection.py
--rw-r--r--   0 runner    (1001) docker     (127)     1262 2023-09-26 12:33:49.000000 onetl-0.9.4/onetl/connection/db_connection/hive/dialect.py
--rw-r--r--   0 runner    (1001) docker     (127)    14206 2023-09-26 12:33:49.000000 onetl-0.9.4/onetl/connection/db_connection/hive/options.py
--rw-r--r--   0 runner    (1001) docker     (127)     3291 2023-09-26 12:33:49.000000 onetl-0.9.4/onetl/connection/db_connection/hive/slots.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-09-26 12:34:22.194914 onetl-0.9.4/onetl/connection/db_connection/jdbc_connection/
--rw-r--r--   0 runner    (1001) docker     (127)      931 2023-09-26 12:33:49.000000 onetl-0.9.4/onetl/connection/db_connection/jdbc_connection/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    13494 2023-09-26 12:33:49.000000 onetl-0.9.4/onetl/connection/db_connection/jdbc_connection/connection.py
--rw-r--r--   0 runner    (1001) docker     (127)     1483 2023-09-26 12:33:49.000000 onetl-0.9.4/onetl/connection/db_connection/jdbc_connection/dialect.py
--rw-r--r--   0 runner    (1001) docker     (127)    16808 2023-09-26 12:33:49.000000 onetl-0.9.4/onetl/connection/db_connection/jdbc_connection/options.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-09-26 12:34:22.194914 onetl-0.9.4/onetl/connection/db_connection/jdbc_mixin/
--rw-r--r--   0 runner    (1001) docker     (127)      780 2023-09-26 12:33:49.000000 onetl-0.9.4/onetl/connection/db_connection/jdbc_mixin/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    23548 2023-09-26 12:33:49.000000 onetl-0.9.4/onetl/connection/db_connection/jdbc_mixin/connection.py
--rw-r--r--   0 runner    (1001) docker     (127)     1845 2023-09-26 12:33:49.000000 onetl-0.9.4/onetl/connection/db_connection/jdbc_mixin/options.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-09-26 12:34:22.198914 onetl-0.9.4/onetl/connection/db_connection/kafka/
--rw-r--r--   0 runner    (1001) docker     (127)      665 2023-09-26 12:33:49.000000 onetl-0.9.4/onetl/connection/db_connection/kafka/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    21626 2023-09-26 12:33:49.000000 onetl-0.9.4/onetl/connection/db_connection/kafka/connection.py
--rw-r--r--   0 runner    (1001) docker     (127)     2458 2023-09-26 12:33:49.000000 onetl-0.9.4/onetl/connection/db_connection/kafka/dialect.py
--rw-r--r--   0 runner    (1001) docker     (127)     1708 2023-09-26 12:33:49.000000 onetl-0.9.4/onetl/connection/db_connection/kafka/extra.py
--rw-r--r--   0 runner    (1001) docker     (127)     1618 2023-09-26 12:33:49.000000 onetl-0.9.4/onetl/connection/db_connection/kafka/kafka_auth.py
--rw-r--r--   0 runner    (1001) docker     (127)     1929 2023-09-26 12:33:49.000000 onetl-0.9.4/onetl/connection/db_connection/kafka/kafka_basic_auth.py
--rw-r--r--   0 runner    (1001) docker     (127)     7327 2023-09-26 12:33:49.000000 onetl-0.9.4/onetl/connection/db_connection/kafka/kafka_kerberos_auth.py
--rw-r--r--   0 runner    (1001) docker     (127)     1693 2023-09-26 12:33:49.000000 onetl-0.9.4/onetl/connection/db_connection/kafka/kafka_plaintext_protocol.py
--rw-r--r--   0 runner    (1001) docker     (127)     1626 2023-09-26 12:33:49.000000 onetl-0.9.4/onetl/connection/db_connection/kafka/kafka_protocol.py
--rw-r--r--   0 runner    (1001) docker     (127)     3118 2023-09-26 12:33:49.000000 onetl-0.9.4/onetl/connection/db_connection/kafka/kafka_scram_auth.py
--rw-r--r--   0 runner    (1001) docker     (127)     6879 2023-09-26 12:33:49.000000 onetl-0.9.4/onetl/connection/db_connection/kafka/kafka_ssl_protocol.py
--rw-r--r--   0 runner    (1001) docker     (127)     4843 2023-09-26 12:33:49.000000 onetl-0.9.4/onetl/connection/db_connection/kafka/options.py
--rw-r--r--   0 runner    (1001) docker     (127)     4514 2023-09-26 12:33:49.000000 onetl-0.9.4/onetl/connection/db_connection/kafka/slots.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-09-26 12:34:22.198914 onetl-0.9.4/onetl/connection/db_connection/mongodb/
--rw-r--r--   0 runner    (1001) docker     (127)      933 2023-09-26 12:33:49.000000 onetl-0.9.4/onetl/connection/db_connection/mongodb/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    19323 2023-09-26 12:33:49.000000 onetl-0.9.4/onetl/connection/db_connection/mongodb/connection.py
--rw-r--r--   0 runner    (1001) docker     (127)     6066 2023-09-26 12:33:49.000000 onetl-0.9.4/onetl/connection/db_connection/mongodb/dialect.py
--rw-r--r--   0 runner    (1001) docker     (127)     7826 2023-09-26 12:33:49.000000 onetl-0.9.4/onetl/connection/db_connection/mongodb/options.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-09-26 12:34:22.198914 onetl-0.9.4/onetl/connection/db_connection/mssql/
--rw-r--r--   0 runner    (1001) docker     (127)      747 2023-09-26 12:33:49.000000 onetl-0.9.4/onetl/connection/db_connection/mssql/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     7185 2023-09-26 12:33:49.000000 onetl-0.9.4/onetl/connection/db_connection/mssql/connection.py
--rw-r--r--   0 runner    (1001) docker     (127)     1564 2023-09-26 12:33:49.000000 onetl-0.9.4/onetl/connection/db_connection/mssql/dialect.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-09-26 12:34:22.198914 onetl-0.9.4/onetl/connection/db_connection/mysql/
--rw-r--r--   0 runner    (1001) docker     (127)      747 2023-09-26 12:33:49.000000 onetl-0.9.4/onetl/connection/db_connection/mysql/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     5104 2023-09-26 12:33:49.000000 onetl-0.9.4/onetl/connection/db_connection/mysql/connection.py
--rw-r--r--   0 runner    (1001) docker     (127)     1623 2023-09-26 12:33:49.000000 onetl-0.9.4/onetl/connection/db_connection/mysql/dialect.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-09-26 12:34:22.202914 onetl-0.9.4/onetl/connection/db_connection/oracle/
--rw-r--r--   0 runner    (1001) docker     (127)      752 2023-09-26 12:33:49.000000 onetl-0.9.4/onetl/connection/db_connection/oracle/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    14603 2023-09-26 12:33:49.000000 onetl-0.9.4/onetl/connection/db_connection/oracle/connection.py
--rw-r--r--   0 runner    (1001) docker     (127)     1486 2023-09-26 12:33:49.000000 onetl-0.9.4/onetl/connection/db_connection/oracle/dialect.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-09-26 12:34:22.202914 onetl-0.9.4/onetl/connection/db_connection/postgres/
--rw-r--r--   0 runner    (1001) docker     (127)      762 2023-09-26 12:33:49.000000 onetl-0.9.4/onetl/connection/db_connection/postgres/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     5701 2023-09-26 12:33:49.000000 onetl-0.9.4/onetl/connection/db_connection/postgres/connection.py
--rw-r--r--   0 runner    (1001) docker     (127)     1583 2023-09-26 12:33:49.000000 onetl-0.9.4/onetl/connection/db_connection/postgres/dialect.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-09-26 12:34:22.202914 onetl-0.9.4/onetl/connection/db_connection/teradata/
--rw-r--r--   0 runner    (1001) docker     (127)      762 2023-09-26 12:33:49.000000 onetl-0.9.4/onetl/connection/db_connection/teradata/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     5930 2023-09-26 12:33:49.000000 onetl-0.9.4/onetl/connection/db_connection/teradata/connection.py
--rw-r--r--   0 runner    (1001) docker     (127)     1538 2023-09-26 12:33:49.000000 onetl-0.9.4/onetl/connection/db_connection/teradata/dialect.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-09-26 12:34:22.202914 onetl-0.9.4/onetl/connection/file_connection/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2023-09-26 12:33:49.000000 onetl-0.9.4/onetl/connection/file_connection/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    26612 2023-09-26 12:33:49.000000 onetl-0.9.4/onetl/connection/file_connection/file_connection.py
--rw-r--r--   0 runner    (1001) docker     (127)     6587 2023-09-26 12:33:49.000000 onetl-0.9.4/onetl/connection/file_connection/ftp.py
--rw-r--r--   0 runner    (1001) docker     (127)     3429 2023-09-26 12:33:49.000000 onetl-0.9.4/onetl/connection/file_connection/ftps.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-09-26 12:34:22.202914 onetl-0.9.4/onetl/connection/file_connection/hdfs/
--rw-r--r--   0 runner    (1001) docker     (127)      731 2023-09-26 12:33:49.000000 onetl-0.9.4/onetl/connection/file_connection/hdfs/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    18985 2023-09-26 12:33:49.000000 onetl-0.9.4/onetl/connection/file_connection/hdfs/connection.py
--rw-r--r--   0 runner    (1001) docker     (127)     7727 2023-09-26 12:33:49.000000 onetl-0.9.4/onetl/connection/file_connection/hdfs/slots.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-09-26 12:34:22.206914 onetl-0.9.4/onetl/connection/file_connection/mixins/
--rw-r--r--   0 runner    (1001) docker     (127)      683 2023-09-26 12:33:49.000000 onetl-0.9.4/onetl/connection/file_connection/mixins/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     3102 2023-09-26 12:33:49.000000 onetl-0.9.4/onetl/connection/file_connection/mixins/rename_dir_mixin.py
--rw-r--r--   0 runner    (1001) docker     (127)    10241 2023-09-26 12:33:49.000000 onetl-0.9.4/onetl/connection/file_connection/s3.py
--rw-r--r--   0 runner    (1001) docker     (127)    10509 2023-09-26 12:33:49.000000 onetl-0.9.4/onetl/connection/file_connection/samba.py
--rw-r--r--   0 runner    (1001) docker     (127)     8915 2023-09-26 12:33:49.000000 onetl-0.9.4/onetl/connection/file_connection/sftp.py
--rw-r--r--   0 runner    (1001) docker     (127)     7957 2023-09-26 12:33:49.000000 onetl-0.9.4/onetl/connection/file_connection/webdav.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-09-26 12:34:22.206914 onetl-0.9.4/onetl/connection/file_df_connection/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2023-09-26 12:33:49.000000 onetl-0.9.4/onetl/connection/file_df_connection/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     6592 2023-09-26 12:33:49.000000 onetl-0.9.4/onetl/connection/file_df_connection/spark_file_df_connection.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-09-26 12:34:22.206914 onetl-0.9.4/onetl/connection/file_df_connection/spark_hdfs/
--rw-r--r--   0 runner    (1001) docker     (127)      759 2023-09-26 12:33:49.000000 onetl-0.9.4/onetl/connection/file_df_connection/spark_hdfs/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    12785 2023-09-26 12:33:49.000000 onetl-0.9.4/onetl/connection/file_df_connection/spark_hdfs/connection.py
--rw-r--r--   0 runner    (1001) docker     (127)     7755 2023-09-26 12:33:49.000000 onetl-0.9.4/onetl/connection/file_df_connection/spark_hdfs/slots.py
--rw-r--r--   0 runner    (1001) docker     (127)     3251 2023-09-26 12:33:49.000000 onetl-0.9.4/onetl/connection/file_df_connection/spark_local_fs.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-09-26 12:34:22.206914 onetl-0.9.4/onetl/connection/file_df_connection/spark_s3/
--rw-r--r--   0 runner    (1001) docker     (127)      751 2023-09-26 12:33:49.000000 onetl-0.9.4/onetl/connection/file_df_connection/spark_s3/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    18097 2023-09-26 12:33:49.000000 onetl-0.9.4/onetl/connection/file_df_connection/spark_s3/connection.py
--rw-r--r--   0 runner    (1001) docker     (127)     1403 2023-09-26 12:33:49.000000 onetl-0.9.4/onetl/connection/file_df_connection/spark_s3/extra.py
--rw-r--r--   0 runner    (1001) docker     (127)     1723 2023-09-26 12:33:49.000000 onetl-0.9.4/onetl/connection/kerberos_helpers.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-09-26 12:34:22.206914 onetl-0.9.4/onetl/core/
--rw-r--r--   0 runner    (1001) docker     (127)     1586 2023-09-26 12:33:49.000000 onetl-0.9.4/onetl/core/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-09-26 12:34:22.206914 onetl-0.9.4/onetl/core/file_filter/
--rw-r--r--   0 runner    (1001) docker     (127)      657 2023-09-26 12:33:49.000000 onetl-0.9.4/onetl/core/file_filter/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     6269 2023-09-26 12:33:49.000000 onetl-0.9.4/onetl/core/file_filter/file_filter.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-09-26 12:34:22.206914 onetl-0.9.4/onetl/core/file_limit/
--rw-r--r--   0 runner    (1001) docker     (127)      654 2023-09-26 12:33:49.000000 onetl-0.9.4/onetl/core/file_limit/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2640 2023-09-26 12:33:49.000000 onetl-0.9.4/onetl/core/file_limit/file_limit.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-09-26 12:34:22.206914 onetl-0.9.4/onetl/db/
--rw-r--r--   0 runner    (1001) docker     (127)      679 2023-09-26 12:33:49.000000 onetl-0.9.4/onetl/db/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-09-26 12:34:22.206914 onetl-0.9.4/onetl/db/db_reader/
--rw-r--r--   0 runner    (1001) docker     (127)      649 2023-09-26 12:33:49.000000 onetl-0.9.4/onetl/db/db_reader/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    22004 2023-09-26 12:33:49.000000 onetl-0.9.4/onetl/db/db_reader/db_reader.py
--rw-r--r--   0 runner    (1001) docker     (127)     8218 2023-09-26 12:33:49.000000 onetl-0.9.4/onetl/db/db_reader/strategy_helper.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-09-26 12:34:22.210914 onetl-0.9.4/onetl/db/db_writer/
--rw-r--r--   0 runner    (1001) docker     (127)      649 2023-09-26 12:33:49.000000 onetl-0.9.4/onetl/db/db_writer/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     6950 2023-09-26 12:33:49.000000 onetl-0.9.4/onetl/db/db_writer/db_writer.py
--rw-r--r--   0 runner    (1001) docker     (127)     3129 2023-09-26 12:33:49.000000 onetl-0.9.4/onetl/exception.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-09-26 12:34:22.210914 onetl-0.9.4/onetl/file/
--rw-r--r--   0 runner    (1001) docker     (127)      891 2023-09-26 12:33:49.000000 onetl-0.9.4/onetl/file/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-09-26 12:34:22.210914 onetl-0.9.4/onetl/file/file_df_reader/
--rw-r--r--   0 runner    (1001) docker     (127)      665 2023-09-26 12:33:49.000000 onetl-0.9.4/onetl/file/file_df_reader/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     9741 2023-09-26 12:33:49.000000 onetl-0.9.4/onetl/file/file_df_reader/file_df_reader.py
--rw-r--r--   0 runner    (1001) docker     (127)     2795 2023-09-26 12:33:49.000000 onetl-0.9.4/onetl/file/file_df_reader/options.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-09-26 12:34:22.210914 onetl-0.9.4/onetl/file/file_df_writer/
--rw-r--r--   0 runner    (1001) docker     (127)      665 2023-09-26 12:33:49.000000 onetl-0.9.4/onetl/file/file_df_writer/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     4993 2023-09-26 12:33:49.000000 onetl-0.9.4/onetl/file/file_df_writer/file_df_writer.py
--rw-r--r--   0 runner    (1001) docker     (127)    11545 2023-09-26 12:33:49.000000 onetl-0.9.4/onetl/file/file_df_writer/options.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-09-26 12:34:22.210914 onetl-0.9.4/onetl/file/file_downloader/
--rw-r--r--   0 runner    (1001) docker     (127)      799 2023-09-26 12:33:49.000000 onetl-0.9.4/onetl/file/file_downloader/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    29610 2023-09-26 12:33:49.000000 onetl-0.9.4/onetl/file/file_downloader/file_downloader.py
--rw-r--r--   0 runner    (1001) docker     (127)     2186 2023-09-26 12:33:49.000000 onetl-0.9.4/onetl/file/file_downloader/options.py
--rw-r--r--   0 runner    (1001) docker     (127)     2450 2023-09-26 12:33:49.000000 onetl-0.9.4/onetl/file/file_downloader/result.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-09-26 12:34:22.210914 onetl-0.9.4/onetl/file/file_mover/
--rw-r--r--   0 runner    (1001) docker     (127)      765 2023-09-26 12:33:49.000000 onetl-0.9.4/onetl/file/file_mover/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    19634 2023-09-26 12:33:49.000000 onetl-0.9.4/onetl/file/file_mover/file_mover.py
--rw-r--r--   0 runner    (1001) docker     (127)     1983 2023-09-26 12:33:49.000000 onetl-0.9.4/onetl/file/file_mover/options.py
--rw-r--r--   0 runner    (1001) docker     (127)     2385 2023-09-26 12:33:49.000000 onetl-0.9.4/onetl/file/file_mover/result.py
--rw-r--r--   0 runner    (1001) docker     (127)    18628 2023-09-26 12:33:49.000000 onetl-0.9.4/onetl/file/file_result.py
--rw-r--r--   0 runner    (1001) docker     (127)     5919 2023-09-26 12:33:49.000000 onetl-0.9.4/onetl/file/file_set.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-09-26 12:34:22.214914 onetl-0.9.4/onetl/file/file_uploader/
--rw-r--r--   0 runner    (1001) docker     (127)      785 2023-09-26 12:33:49.000000 onetl-0.9.4/onetl/file/file_uploader/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    21738 2023-09-26 12:33:49.000000 onetl-0.9.4/onetl/file/file_uploader/file_uploader.py
--rw-r--r--   0 runner    (1001) docker     (127)     2171 2023-09-26 12:33:49.000000 onetl-0.9.4/onetl/file/file_uploader/options.py
--rw-r--r--   0 runner    (1001) docker     (127)     2408 2023-09-26 12:33:49.000000 onetl-0.9.4/onetl/file/file_uploader/result.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-09-26 12:34:22.214914 onetl-0.9.4/onetl/file/filter/
--rw-r--r--   0 runner    (1001) docker     (127)      856 2023-09-26 12:33:49.000000 onetl-0.9.4/onetl/file/filter/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1988 2023-09-26 12:33:49.000000 onetl-0.9.4/onetl/file/filter/exclude_dir.py
--rw-r--r--   0 runner    (1001) docker     (127)     1421 2023-09-26 12:33:49.000000 onetl-0.9.4/onetl/file/filter/file_hwm.py
--rw-r--r--   0 runner    (1001) docker     (127)     1855 2023-09-26 12:33:49.000000 onetl-0.9.4/onetl/file/filter/glob.py
--rw-r--r--   0 runner    (1001) docker     (127)     2274 2023-09-26 12:33:49.000000 onetl-0.9.4/onetl/file/filter/match_all_filters.py
--rw-r--r--   0 runner    (1001) docker     (127)     2434 2023-09-26 12:33:49.000000 onetl-0.9.4/onetl/file/filter/regexp.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-09-26 12:34:22.214914 onetl-0.9.4/onetl/file/format/
--rw-r--r--   0 runner    (1001) docker     (127)      892 2023-09-26 12:33:49.000000 onetl-0.9.4/onetl/file/format/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     6444 2023-09-26 12:33:49.000000 onetl-0.9.4/onetl/file/format/avro.py
--rw-r--r--   0 runner    (1001) docker     (127)     3028 2023-09-26 12:33:49.000000 onetl-0.9.4/onetl/file/format/csv.py
--rw-r--r--   0 runner    (1001) docker     (127)     7270 2023-09-26 12:33:49.000000 onetl-0.9.4/onetl/file/format/excel.py
--rw-r--r--   0 runner    (1001) docker     (127)     1958 2023-09-26 12:33:49.000000 onetl-0.9.4/onetl/file/format/file_format.py
--rw-r--r--   0 runner    (1001) docker     (127)     3007 2023-09-26 12:33:49.000000 onetl-0.9.4/onetl/file/format/json.py
--rw-r--r--   0 runner    (1001) docker     (127)     2954 2023-09-26 12:33:49.000000 onetl-0.9.4/onetl/file/format/jsonline.py
--rw-r--r--   0 runner    (1001) docker     (127)     2125 2023-09-26 12:33:49.000000 onetl-0.9.4/onetl/file/format/orc.py
--rw-r--r--   0 runner    (1001) docker     (127)     2236 2023-09-26 12:33:49.000000 onetl-0.9.4/onetl/file/format/parquet.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-09-26 12:34:22.218914 onetl-0.9.4/onetl/file/limit/
--rw-r--r--   0 runner    (1001) docker     (127)      832 2023-09-26 12:33:49.000000 onetl-0.9.4/onetl/file/limit/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1920 2023-09-26 12:33:49.000000 onetl-0.9.4/onetl/file/limit/limits_reached.py
--rw-r--r--   0 runner    (1001) docker     (127)     1862 2023-09-26 12:33:49.000000 onetl-0.9.4/onetl/file/limit/limits_stop_at.py
--rw-r--r--   0 runner    (1001) docker     (127)     1987 2023-09-26 12:33:49.000000 onetl-0.9.4/onetl/file/limit/max_files_count.py
--rw-r--r--   0 runner    (1001) docker     (127)     1696 2023-09-26 12:33:49.000000 onetl-0.9.4/onetl/file/limit/reset_limits.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-09-26 12:34:22.218914 onetl-0.9.4/onetl/hooks/
--rw-r--r--   0 runner    (1001) docker     (127)      219 2023-09-26 12:33:49.000000 onetl-0.9.4/onetl/hooks/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    11851 2023-09-26 12:33:49.000000 onetl-0.9.4/onetl/hooks/hook.py
--rw-r--r--   0 runner    (1001) docker     (127)     6781 2023-09-26 12:33:49.000000 onetl-0.9.4/onetl/hooks/hook_collection.py
--rw-r--r--   0 runner    (1001) docker     (127)     3156 2023-09-26 12:33:49.000000 onetl-0.9.4/onetl/hooks/hooks_state.py
--rw-r--r--   0 runner    (1001) docker     (127)     2224 2023-09-26 12:33:49.000000 onetl-0.9.4/onetl/hooks/method_inheritance_stack.py
--rw-r--r--   0 runner    (1001) docker     (127)    21270 2023-09-26 12:33:49.000000 onetl-0.9.4/onetl/hooks/slot.py
--rw-r--r--   0 runner    (1001) docker     (127)     4948 2023-09-26 12:33:49.000000 onetl-0.9.4/onetl/hooks/support_hooks.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-09-26 12:34:22.218914 onetl-0.9.4/onetl/hwm/
--rw-r--r--   0 runner    (1001) docker     (127)       42 2023-09-26 12:33:49.000000 onetl-0.9.4/onetl/hwm/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      197 2023-09-26 12:33:49.000000 onetl-0.9.4/onetl/hwm/statement.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-09-26 12:34:22.222914 onetl-0.9.4/onetl/hwm/store/
--rw-r--r--   0 runner    (1001) docker     (127)     1082 2023-09-26 12:33:49.000000 onetl-0.9.4/onetl/hwm/store/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     3472 2023-09-26 12:33:49.000000 onetl-0.9.4/onetl/hwm/store/base_hwm_store.py
--rw-r--r--   0 runner    (1001) docker     (127)     3132 2023-09-26 12:33:49.000000 onetl-0.9.4/onetl/hwm/store/hwm_class_registry.py
--rw-r--r--   0 runner    (1001) docker     (127)     6828 2023-09-26 12:33:49.000000 onetl-0.9.4/onetl/hwm/store/hwm_store_class_registry.py
--rw-r--r--   0 runner    (1001) docker     (127)     1356 2023-09-26 12:33:49.000000 onetl-0.9.4/onetl/hwm/store/hwm_store_manager.py
--rw-r--r--   0 runner    (1001) docker     (127)     2863 2023-09-26 12:33:49.000000 onetl-0.9.4/onetl/hwm/store/memory_hwm_store.py
--rw-r--r--   0 runner    (1001) docker     (127)     6487 2023-09-26 12:33:49.000000 onetl-0.9.4/onetl/hwm/store/yaml_hwm_store.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-09-26 12:34:22.222914 onetl-0.9.4/onetl/impl/
--rw-r--r--   0 runner    (1001) docker     (127)     1171 2023-09-26 12:33:49.000000 onetl-0.9.4/onetl/impl/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1952 2023-09-26 12:33:49.000000 onetl-0.9.4/onetl/impl/base_model.py
--rw-r--r--   0 runner    (1001) docker     (127)     1771 2023-09-26 12:33:49.000000 onetl-0.9.4/onetl/impl/failed_local_file.py
--rw-r--r--   0 runner    (1001) docker     (127)     1676 2023-09-26 12:33:49.000000 onetl-0.9.4/onetl/impl/file_exist_behavior.py
--rw-r--r--   0 runner    (1001) docker     (127)      751 2023-09-26 12:33:49.000000 onetl-0.9.4/onetl/impl/frozen_model.py
--rw-r--r--   0 runner    (1001) docker     (127)     5093 2023-09-26 12:33:49.000000 onetl-0.9.4/onetl/impl/generic_options.py
--rw-r--r--   0 runner    (1001) docker     (127)     1028 2023-09-26 12:33:49.000000 onetl-0.9.4/onetl/impl/local_path.py
--rw-r--r--   0 runner    (1001) docker     (127)     3700 2023-09-26 12:33:49.000000 onetl-0.9.4/onetl/impl/path_container.py
--rw-r--r--   0 runner    (1001) docker     (127)     5384 2023-09-26 12:33:49.000000 onetl-0.9.4/onetl/impl/path_repr.py
--rw-r--r--   0 runner    (1001) docker     (127)     1865 2023-09-26 12:33:49.000000 onetl-0.9.4/onetl/impl/remote_directory.py
--rw-r--r--   0 runner    (1001) docker     (127)     2331 2023-09-26 12:33:49.000000 onetl-0.9.4/onetl/impl/remote_file.py
--rw-r--r--   0 runner    (1001) docker     (127)      677 2023-09-26 12:33:49.000000 onetl-0.9.4/onetl/impl/remote_path.py
--rw-r--r--   0 runner    (1001) docker     (127)     1563 2023-09-26 12:33:49.000000 onetl-0.9.4/onetl/impl/remote_path_stat.py
--rw-r--r--   0 runner    (1001) docker     (127)    14108 2023-09-26 12:33:49.000000 onetl-0.9.4/onetl/log.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-09-26 12:34:22.222914 onetl-0.9.4/onetl/plugins/
--rw-r--r--   0 runner    (1001) docker     (127)       56 2023-09-26 12:33:49.000000 onetl-0.9.4/onetl/plugins/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     4464 2023-09-26 12:33:49.000000 onetl-0.9.4/onetl/plugins/import_plugins.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-09-26 12:34:22.226914 onetl-0.9.4/onetl/strategy/
--rw-r--r--   0 runner    (1001) docker     (127)      905 2023-09-26 12:33:49.000000 onetl-0.9.4/onetl/strategy/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2420 2023-09-26 12:33:49.000000 onetl-0.9.4/onetl/strategy/base_strategy.py
--rw-r--r--   0 runner    (1001) docker     (127)     5059 2023-09-26 12:33:49.000000 onetl-0.9.4/onetl/strategy/batch_hwm_strategy.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-09-26 12:34:22.226914 onetl-0.9.4/onetl/strategy/hwm_store/
--rw-r--r--   0 runner    (1001) docker     (127)     1819 2023-09-26 12:33:49.000000 onetl-0.9.4/onetl/strategy/hwm_store/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     3978 2023-09-26 12:33:49.000000 onetl-0.9.4/onetl/strategy/hwm_strategy.py
--rw-r--r--   0 runner    (1001) docker     (127)    19405 2023-09-26 12:33:49.000000 onetl-0.9.4/onetl/strategy/incremental_strategy.py
--rw-r--r--   0 runner    (1001) docker     (127)    12810 2023-09-26 12:33:49.000000 onetl-0.9.4/onetl/strategy/snapshot_strategy.py
--rw-r--r--   0 runner    (1001) docker     (127)     1391 2023-09-26 12:33:49.000000 onetl-0.9.4/onetl/strategy/strategy_manager.py
--rw-r--r--   0 runner    (1001) docker     (127)      814 2023-09-26 12:33:49.000000 onetl-0.9.4/onetl/version.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-09-26 12:34:22.182914 onetl-0.9.4/onetl.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)    28903 2023-09-26 12:34:22.000000 onetl-0.9.4/onetl.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     9740 2023-09-26 12:34:22.000000 onetl-0.9.4/onetl.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2023-09-26 12:34:22.000000 onetl-0.9.4/onetl.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2023-09-26 12:34:22.000000 onetl-0.9.4/onetl.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (127)      606 2023-09-26 12:34:22.000000 onetl-0.9.4/onetl.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)        6 2023-09-26 12:34:22.000000 onetl-0.9.4/onetl.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)     1180 2023-09-26 12:33:49.000000 onetl-0.9.4/pyproject.toml
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-09-26 12:34:22.226914 onetl-0.9.4/requirements/
--rw-r--r--   0 runner    (1001) docker     (127)      503 2023-09-26 12:33:49.000000 onetl-0.9.4/requirements/core.txt
--rw-r--r--   0 runner    (1001) docker     (127)       96 2023-09-26 12:33:49.000000 onetl-0.9.4/requirements/dev.txt
--rw-r--r--   0 runner    (1001) docker     (127)      233 2023-09-26 12:33:49.000000 onetl-0.9.4/requirements/docs.txt
--rw-r--r--   0 runner    (1001) docker     (127)       60 2023-09-26 12:33:49.000000 onetl-0.9.4/requirements/ftp.txt
--rw-r--r--   0 runner    (1001) docker     (127)        7 2023-09-26 12:33:49.000000 onetl-0.9.4/requirements/hdfs.txt
--rw-r--r--   0 runner    (1001) docker     (127)       85 2023-09-26 12:33:49.000000 onetl-0.9.4/requirements/kerberos.txt
--rw-r--r--   0 runner    (1001) docker     (127)        6 2023-09-26 12:33:49.000000 onetl-0.9.4/requirements/s3.txt
--rw-r--r--   0 runner    (1001) docker     (127)        6 2023-09-26 12:33:49.000000 onetl-0.9.4/requirements/samba.txt
--rw-r--r--   0 runner    (1001) docker     (127)        9 2023-09-26 12:33:49.000000 onetl-0.9.4/requirements/sftp.txt
--rw-r--r--   0 runner    (1001) docker     (127)        8 2023-09-26 12:33:49.000000 onetl-0.9.4/requirements/spark.txt
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-09-26 12:34:22.230914 onetl-0.9.4/requirements/tests/
--rw-r--r--   0 runner    (1001) docker     (127)       79 2023-09-26 12:33:49.000000 onetl-0.9.4/requirements/tests/base.txt
--rw-r--r--   0 runner    (1001) docker     (127)       18 2023-09-26 12:33:49.000000 onetl-0.9.4/requirements/tests/clickhouse.txt
--rw-r--r--   0 runner    (1001) docker     (127)       16 2023-09-26 12:33:49.000000 onetl-0.9.4/requirements/tests/kafka.txt
--rw-r--r--   0 runner    (1001) docker     (127)        8 2023-09-26 12:33:49.000000 onetl-0.9.4/requirements/tests/mongodb.txt
--rw-r--r--   0 runner    (1001) docker     (127)       62 2023-09-26 12:33:49.000000 onetl-0.9.4/requirements/tests/mssql.txt
--rw-r--r--   0 runner    (1001) docker     (127)       13 2023-09-26 12:33:49.000000 onetl-0.9.4/requirements/tests/mysql.txt
--rw-r--r--   0 runner    (1001) docker     (127)       10 2023-09-26 12:33:49.000000 onetl-0.9.4/requirements/tests/oracle.txt
--rw-r--r--   0 runner    (1001) docker     (127)       16 2023-09-26 12:33:49.000000 onetl-0.9.4/requirements/tests/postgres.txt
--rw-r--r--   0 runner    (1001) docker     (127)        6 2023-09-26 12:33:49.000000 onetl-0.9.4/requirements/tests/samba.txt
--rw-r--r--   0 runner    (1001) docker     (127)       86 2023-09-26 12:33:49.000000 onetl-0.9.4/requirements/tests/spark-2.3.1.txt
--rw-r--r--   0 runner    (1001) docker     (127)       86 2023-09-26 12:33:49.000000 onetl-0.9.4/requirements/tests/spark-2.4.8.txt
--rw-r--r--   0 runner    (1001) docker     (127)       76 2023-09-26 12:33:49.000000 onetl-0.9.4/requirements/tests/spark-3.2.4.txt
--rw-r--r--   0 runner    (1001) docker     (127)       76 2023-09-26 12:33:49.000000 onetl-0.9.4/requirements/tests/spark-3.3.2.txt
--rw-r--r--   0 runner    (1001) docker     (127)       63 2023-09-26 12:33:49.000000 onetl-0.9.4/requirements/tests/spark-3.4.1.txt
--rw-r--r--   0 runner    (1001) docker     (127)       56 2023-09-26 12:33:49.000000 onetl-0.9.4/requirements/tests/spark-latest.txt
--rw-r--r--   0 runner    (1001) docker     (127)       14 2023-09-26 12:33:49.000000 onetl-0.9.4/requirements/webdav.txt
--rw-r--r--   0 runner    (1001) docker     (127)     3243 2023-09-26 12:34:22.234914 onetl-0.9.4/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)     3935 2023-09-26 12:33:49.000000 onetl-0.9.4/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-10-10 11:38:46.490232 onetl-0.9.5/
+-rw-r--r--   0 runner    (1001) docker     (127)    11421 2023-10-10 11:38:18.000000 onetl-0.9.5/LICENSE.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      257 2023-10-10 11:38:18.000000 onetl-0.9.5/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (127)    29105 2023-10-10 11:38:46.490232 onetl-0.9.5/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)    25995 2023-10-10 11:38:18.000000 onetl-0.9.5/README.rst
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-10-10 11:38:46.386233 onetl-0.9.5/onetl/
+-rw-r--r--   0 runner    (1001) docker     (127)        6 2023-10-10 11:38:18.000000 onetl-0.9.5/onetl/VERSION
+-rw-r--r--   0 runner    (1001) docker     (127)     1301 2023-10-10 11:38:18.000000 onetl-0.9.5/onetl/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5860 2023-10-10 11:38:18.000000 onetl-0.9.5/onetl/_internal.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-10-10 11:38:46.390233 onetl-0.9.5/onetl/_util/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2023-10-10 11:38:18.000000 onetl-0.9.5/onetl/_util/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1080 2023-10-10 11:38:18.000000 onetl-0.9.5/onetl/_util/classproperty.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1665 2023-10-10 11:38:18.000000 onetl-0.9.5/onetl/_util/file.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1320 2023-10-10 11:38:18.000000 onetl-0.9.5/onetl/_util/hadoop.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1224 2023-10-10 11:38:18.000000 onetl-0.9.5/onetl/_util/java.py
+-rw-r--r--   0 runner    (1001) docker     (127)      904 2023-10-10 11:38:18.000000 onetl-0.9.5/onetl/_util/scala.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4747 2023-10-10 11:38:18.000000 onetl-0.9.5/onetl/_util/spark.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5511 2023-10-10 11:38:18.000000 onetl-0.9.5/onetl/_util/version.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-10-10 11:38:46.402233 onetl-0.9.5/onetl/base/
+-rw-r--r--   0 runner    (1001) docker     (127)     1568 2023-10-10 11:38:18.000000 onetl-0.9.5/onetl/base/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1167 2023-10-10 11:38:18.000000 onetl-0.9.5/onetl/base/base_connection.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5070 2023-10-10 11:38:18.000000 onetl-0.9.5/onetl/base/base_db_connection.py
+-rw-r--r--   0 runner    (1001) docker     (127)    19414 2023-10-10 11:38:18.000000 onetl-0.9.5/onetl/base/base_file_connection.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4064 2023-10-10 11:38:18.000000 onetl-0.9.5/onetl/base/base_file_df_connection.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1466 2023-10-10 11:38:18.000000 onetl-0.9.5/onetl/base/base_file_filter.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2848 2023-10-10 11:38:18.000000 onetl-0.9.5/onetl/base/base_file_format.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3120 2023-10-10 11:38:18.000000 onetl-0.9.5/onetl/base/base_file_limit.py
+-rw-r--r--   0 runner    (1001) docker     (127)      907 2023-10-10 11:38:18.000000 onetl-0.9.5/onetl/base/contains_exception.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1151 2023-10-10 11:38:18.000000 onetl-0.9.5/onetl/base/contains_get_df_schema.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1179 2023-10-10 11:38:18.000000 onetl-0.9.5/onetl/base/contains_get_min_max_bounds.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1713 2023-10-10 11:38:18.000000 onetl-0.9.5/onetl/base/path_protocol.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1468 2023-10-10 11:38:18.000000 onetl-0.9.5/onetl/base/path_stat_protocol.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2380 2023-10-10 11:38:18.000000 onetl-0.9.5/onetl/base/pure_path_protocol.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1092 2023-10-10 11:38:18.000000 onetl-0.9.5/onetl/base/supports_rename_dir.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-10-10 11:38:46.402233 onetl-0.9.5/onetl/connection/
+-rw-r--r--   0 runner    (1001) docker     (127)     3479 2023-10-10 11:38:18.000000 onetl-0.9.5/onetl/connection/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-10-10 11:38:46.402233 onetl-0.9.5/onetl/connection/db_connection/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2023-10-10 11:38:18.000000 onetl-0.9.5/onetl/connection/db_connection/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-10-10 11:38:46.402233 onetl-0.9.5/onetl/connection/db_connection/clickhouse/
+-rw-r--r--   0 runner    (1001) docker     (127)      785 2023-10-10 11:38:18.000000 onetl-0.9.5/onetl/connection/db_connection/clickhouse/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5706 2023-10-10 11:38:18.000000 onetl-0.9.5/onetl/connection/db_connection/clickhouse/connection.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1468 2023-10-10 11:38:18.000000 onetl-0.9.5/onetl/connection/db_connection/clickhouse/dialect.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-10-10 11:38:46.406233 onetl-0.9.5/onetl/connection/db_connection/db_connection/
+-rw-r--r--   0 runner    (1001) docker     (127)      755 2023-10-10 11:38:18.000000 onetl-0.9.5/onetl/connection/db_connection/db_connection/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2321 2023-10-10 11:38:18.000000 onetl-0.9.5/onetl/connection/db_connection/db_connection/connection.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3952 2023-10-10 11:38:18.000000 onetl-0.9.5/onetl/connection/db_connection/db_connection/dialect.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-10-10 11:38:46.414233 onetl-0.9.5/onetl/connection/db_connection/dialect_mixins/
+-rw-r--r--   0 runner    (1001) docker     (127)     1412 2023-10-10 11:38:18.000000 onetl-0.9.5/onetl/connection/db_connection/dialect_mixins/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      354 2023-10-10 11:38:18.000000 onetl-0.9.5/onetl/connection/db_connection/dialect_mixins/support_columns_list.py
+-rw-r--r--   0 runner    (1001) docker     (127)      396 2023-10-10 11:38:18.000000 onetl-0.9.5/onetl/connection/db_connection/dialect_mixins/support_columns_none.py
+-rw-r--r--   0 runner    (1001) docker     (127)      481 2023-10-10 11:38:18.000000 onetl-0.9.5/onetl/connection/db_connection/dialect_mixins/support_df_schema_none.py
+-rw-r--r--   0 runner    (1001) docker     (127)      511 2023-10-10 11:38:18.000000 onetl-0.9.5/onetl/connection/db_connection/dialect_mixins/support_df_schema_struct.py
+-rw-r--r--   0 runner    (1001) docker     (127)      380 2023-10-10 11:38:18.000000 onetl-0.9.5/onetl/connection/db_connection/dialect_mixins/support_hint_none.py
+-rw-r--r--   0 runner    (1001) docker     (127)      555 2023-10-10 11:38:18.000000 onetl-0.9.5/onetl/connection/db_connection/dialect_mixins/support_hint_str.py
+-rw-r--r--   0 runner    (1001) docker     (127)      515 2023-10-10 11:38:18.000000 onetl-0.9.5/onetl/connection/db_connection/dialect_mixins/support_hwm_column_str.py
+-rw-r--r--   0 runner    (1001) docker     (127)      439 2023-10-10 11:38:18.000000 onetl-0.9.5/onetl/connection/db_connection/dialect_mixins/support_hwm_expression_none.py
+-rw-r--r--   0 runner    (1001) docker     (127)      558 2023-10-10 11:38:18.000000 onetl-0.9.5/onetl/connection/db_connection/dialect_mixins/support_hwm_expression_str.py
+-rw-r--r--   0 runner    (1001) docker     (127)      251 2023-10-10 11:38:18.000000 onetl-0.9.5/onetl/connection/db_connection/dialect_mixins/support_name_any.py
+-rw-r--r--   0 runner    (1001) docker     (127)      427 2023-10-10 11:38:18.000000 onetl-0.9.5/onetl/connection/db_connection/dialect_mixins/support_name_with_schema_only.py
+-rw-r--r--   0 runner    (1001) docker     (127)      984 2023-10-10 11:38:18.000000 onetl-0.9.5/onetl/connection/db_connection/dialect_mixins/support_where_none.py
+-rw-r--r--   0 runner    (1001) docker     (127)      563 2023-10-10 11:38:18.000000 onetl-0.9.5/onetl/connection/db_connection/dialect_mixins/support_where_str.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-10-10 11:38:46.418233 onetl-0.9.5/onetl/connection/db_connection/greenplum/
+-rw-r--r--   0 runner    (1001) docker     (127)      902 2023-10-10 11:38:18.000000 onetl-0.9.5/onetl/connection/db_connection/greenplum/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    20429 2023-10-10 11:38:18.000000 onetl-0.9.5/onetl/connection/db_connection/greenplum/connection.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1271 2023-10-10 11:38:18.000000 onetl-0.9.5/onetl/connection/db_connection/greenplum/connection_limit.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1525 2023-10-10 11:38:18.000000 onetl-0.9.5/onetl/connection/db_connection/greenplum/dialect.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10152 2023-10-10 11:38:18.000000 onetl-0.9.5/onetl/connection/db_connection/greenplum/options.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-10-10 11:38:46.422233 onetl-0.9.5/onetl/connection/db_connection/hive/
+-rw-r--r--   0 runner    (1001) docker     (127)      928 2023-10-10 11:38:18.000000 onetl-0.9.5/onetl/connection/db_connection/hive/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    19752 2023-10-10 11:38:18.000000 onetl-0.9.5/onetl/connection/db_connection/hive/connection.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1262 2023-10-10 11:38:18.000000 onetl-0.9.5/onetl/connection/db_connection/hive/dialect.py
+-rw-r--r--   0 runner    (1001) docker     (127)    14206 2023-10-10 11:38:18.000000 onetl-0.9.5/onetl/connection/db_connection/hive/options.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3291 2023-10-10 11:38:18.000000 onetl-0.9.5/onetl/connection/db_connection/hive/slots.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-10-10 11:38:46.422233 onetl-0.9.5/onetl/connection/db_connection/jdbc_connection/
+-rw-r--r--   0 runner    (1001) docker     (127)      931 2023-10-10 11:38:18.000000 onetl-0.9.5/onetl/connection/db_connection/jdbc_connection/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    13494 2023-10-10 11:38:18.000000 onetl-0.9.5/onetl/connection/db_connection/jdbc_connection/connection.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1483 2023-10-10 11:38:18.000000 onetl-0.9.5/onetl/connection/db_connection/jdbc_connection/dialect.py
+-rw-r--r--   0 runner    (1001) docker     (127)    16808 2023-10-10 11:38:18.000000 onetl-0.9.5/onetl/connection/db_connection/jdbc_connection/options.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-10-10 11:38:46.426233 onetl-0.9.5/onetl/connection/db_connection/jdbc_mixin/
+-rw-r--r--   0 runner    (1001) docker     (127)      780 2023-10-10 11:38:18.000000 onetl-0.9.5/onetl/connection/db_connection/jdbc_mixin/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    23548 2023-10-10 11:38:18.000000 onetl-0.9.5/onetl/connection/db_connection/jdbc_mixin/connection.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1845 2023-10-10 11:38:18.000000 onetl-0.9.5/onetl/connection/db_connection/jdbc_mixin/options.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-10-10 11:38:46.434233 onetl-0.9.5/onetl/connection/db_connection/kafka/
+-rw-r--r--   0 runner    (1001) docker     (127)      665 2023-10-10 11:38:18.000000 onetl-0.9.5/onetl/connection/db_connection/kafka/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    21626 2023-10-10 11:38:18.000000 onetl-0.9.5/onetl/connection/db_connection/kafka/connection.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2458 2023-10-10 11:38:18.000000 onetl-0.9.5/onetl/connection/db_connection/kafka/dialect.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1708 2023-10-10 11:38:18.000000 onetl-0.9.5/onetl/connection/db_connection/kafka/extra.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1618 2023-10-10 11:38:18.000000 onetl-0.9.5/onetl/connection/db_connection/kafka/kafka_auth.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1929 2023-10-10 11:38:18.000000 onetl-0.9.5/onetl/connection/db_connection/kafka/kafka_basic_auth.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7327 2023-10-10 11:38:18.000000 onetl-0.9.5/onetl/connection/db_connection/kafka/kafka_kerberos_auth.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1693 2023-10-10 11:38:18.000000 onetl-0.9.5/onetl/connection/db_connection/kafka/kafka_plaintext_protocol.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1626 2023-10-10 11:38:18.000000 onetl-0.9.5/onetl/connection/db_connection/kafka/kafka_protocol.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3118 2023-10-10 11:38:18.000000 onetl-0.9.5/onetl/connection/db_connection/kafka/kafka_scram_auth.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6879 2023-10-10 11:38:18.000000 onetl-0.9.5/onetl/connection/db_connection/kafka/kafka_ssl_protocol.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4843 2023-10-10 11:38:18.000000 onetl-0.9.5/onetl/connection/db_connection/kafka/options.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4514 2023-10-10 11:38:18.000000 onetl-0.9.5/onetl/connection/db_connection/kafka/slots.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-10-10 11:38:46.434233 onetl-0.9.5/onetl/connection/db_connection/mongodb/
+-rw-r--r--   0 runner    (1001) docker     (127)      933 2023-10-10 11:38:18.000000 onetl-0.9.5/onetl/connection/db_connection/mongodb/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    19399 2023-10-10 11:38:18.000000 onetl-0.9.5/onetl/connection/db_connection/mongodb/connection.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6066 2023-10-10 11:38:18.000000 onetl-0.9.5/onetl/connection/db_connection/mongodb/dialect.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7826 2023-10-10 11:38:18.000000 onetl-0.9.5/onetl/connection/db_connection/mongodb/options.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-10-10 11:38:46.438233 onetl-0.9.5/onetl/connection/db_connection/mssql/
+-rw-r--r--   0 runner    (1001) docker     (127)      747 2023-10-10 11:38:18.000000 onetl-0.9.5/onetl/connection/db_connection/mssql/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7185 2023-10-10 11:38:18.000000 onetl-0.9.5/onetl/connection/db_connection/mssql/connection.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1564 2023-10-10 11:38:18.000000 onetl-0.9.5/onetl/connection/db_connection/mssql/dialect.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-10-10 11:38:46.438233 onetl-0.9.5/onetl/connection/db_connection/mysql/
+-rw-r--r--   0 runner    (1001) docker     (127)      747 2023-10-10 11:38:18.000000 onetl-0.9.5/onetl/connection/db_connection/mysql/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5104 2023-10-10 11:38:18.000000 onetl-0.9.5/onetl/connection/db_connection/mysql/connection.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1623 2023-10-10 11:38:18.000000 onetl-0.9.5/onetl/connection/db_connection/mysql/dialect.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-10-10 11:38:46.438233 onetl-0.9.5/onetl/connection/db_connection/oracle/
+-rw-r--r--   0 runner    (1001) docker     (127)      752 2023-10-10 11:38:18.000000 onetl-0.9.5/onetl/connection/db_connection/oracle/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    14603 2023-10-10 11:38:18.000000 onetl-0.9.5/onetl/connection/db_connection/oracle/connection.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1486 2023-10-10 11:38:18.000000 onetl-0.9.5/onetl/connection/db_connection/oracle/dialect.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-10-10 11:38:46.442233 onetl-0.9.5/onetl/connection/db_connection/postgres/
+-rw-r--r--   0 runner    (1001) docker     (127)      762 2023-10-10 11:38:18.000000 onetl-0.9.5/onetl/connection/db_connection/postgres/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5701 2023-10-10 11:38:18.000000 onetl-0.9.5/onetl/connection/db_connection/postgres/connection.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1583 2023-10-10 11:38:18.000000 onetl-0.9.5/onetl/connection/db_connection/postgres/dialect.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-10-10 11:38:46.442233 onetl-0.9.5/onetl/connection/db_connection/teradata/
+-rw-r--r--   0 runner    (1001) docker     (127)      762 2023-10-10 11:38:18.000000 onetl-0.9.5/onetl/connection/db_connection/teradata/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5930 2023-10-10 11:38:18.000000 onetl-0.9.5/onetl/connection/db_connection/teradata/connection.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1538 2023-10-10 11:38:18.000000 onetl-0.9.5/onetl/connection/db_connection/teradata/dialect.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-10-10 11:38:46.446233 onetl-0.9.5/onetl/connection/file_connection/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2023-10-10 11:38:18.000000 onetl-0.9.5/onetl/connection/file_connection/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    26612 2023-10-10 11:38:18.000000 onetl-0.9.5/onetl/connection/file_connection/file_connection.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6587 2023-10-10 11:38:18.000000 onetl-0.9.5/onetl/connection/file_connection/ftp.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3429 2023-10-10 11:38:18.000000 onetl-0.9.5/onetl/connection/file_connection/ftps.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-10-10 11:38:46.450233 onetl-0.9.5/onetl/connection/file_connection/hdfs/
+-rw-r--r--   0 runner    (1001) docker     (127)      731 2023-10-10 11:38:18.000000 onetl-0.9.5/onetl/connection/file_connection/hdfs/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    18985 2023-10-10 11:38:18.000000 onetl-0.9.5/onetl/connection/file_connection/hdfs/connection.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7727 2023-10-10 11:38:18.000000 onetl-0.9.5/onetl/connection/file_connection/hdfs/slots.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-10-10 11:38:46.450233 onetl-0.9.5/onetl/connection/file_connection/mixins/
+-rw-r--r--   0 runner    (1001) docker     (127)      683 2023-10-10 11:38:18.000000 onetl-0.9.5/onetl/connection/file_connection/mixins/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3102 2023-10-10 11:38:18.000000 onetl-0.9.5/onetl/connection/file_connection/mixins/rename_dir_mixin.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10241 2023-10-10 11:38:18.000000 onetl-0.9.5/onetl/connection/file_connection/s3.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10509 2023-10-10 11:38:18.000000 onetl-0.9.5/onetl/connection/file_connection/samba.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8915 2023-10-10 11:38:18.000000 onetl-0.9.5/onetl/connection/file_connection/sftp.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7957 2023-10-10 11:38:18.000000 onetl-0.9.5/onetl/connection/file_connection/webdav.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-10-10 11:38:46.450233 onetl-0.9.5/onetl/connection/file_df_connection/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2023-10-10 11:38:18.000000 onetl-0.9.5/onetl/connection/file_df_connection/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7037 2023-10-10 11:38:18.000000 onetl-0.9.5/onetl/connection/file_df_connection/spark_file_df_connection.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-10-10 11:38:46.454233 onetl-0.9.5/onetl/connection/file_df_connection/spark_hdfs/
+-rw-r--r--   0 runner    (1001) docker     (127)      759 2023-10-10 11:38:18.000000 onetl-0.9.5/onetl/connection/file_df_connection/spark_hdfs/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12785 2023-10-10 11:38:18.000000 onetl-0.9.5/onetl/connection/file_df_connection/spark_hdfs/connection.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7755 2023-10-10 11:38:18.000000 onetl-0.9.5/onetl/connection/file_df_connection/spark_hdfs/slots.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3251 2023-10-10 11:38:18.000000 onetl-0.9.5/onetl/connection/file_df_connection/spark_local_fs.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-10-10 11:38:46.454233 onetl-0.9.5/onetl/connection/file_df_connection/spark_s3/
+-rw-r--r--   0 runner    (1001) docker     (127)      751 2023-10-10 11:38:18.000000 onetl-0.9.5/onetl/connection/file_df_connection/spark_s3/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    18097 2023-10-10 11:38:18.000000 onetl-0.9.5/onetl/connection/file_df_connection/spark_s3/connection.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1403 2023-10-10 11:38:18.000000 onetl-0.9.5/onetl/connection/file_df_connection/spark_s3/extra.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1723 2023-10-10 11:38:18.000000 onetl-0.9.5/onetl/connection/kerberos_helpers.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-10-10 11:38:46.458232 onetl-0.9.5/onetl/core/
+-rw-r--r--   0 runner    (1001) docker     (127)     1586 2023-10-10 11:38:18.000000 onetl-0.9.5/onetl/core/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-10-10 11:38:46.458232 onetl-0.9.5/onetl/core/file_filter/
+-rw-r--r--   0 runner    (1001) docker     (127)      657 2023-10-10 11:38:18.000000 onetl-0.9.5/onetl/core/file_filter/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6269 2023-10-10 11:38:18.000000 onetl-0.9.5/onetl/core/file_filter/file_filter.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-10-10 11:38:46.458232 onetl-0.9.5/onetl/core/file_limit/
+-rw-r--r--   0 runner    (1001) docker     (127)      654 2023-10-10 11:38:18.000000 onetl-0.9.5/onetl/core/file_limit/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2640 2023-10-10 11:38:18.000000 onetl-0.9.5/onetl/core/file_limit/file_limit.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-10-10 11:38:46.458232 onetl-0.9.5/onetl/db/
+-rw-r--r--   0 runner    (1001) docker     (127)      679 2023-10-10 11:38:18.000000 onetl-0.9.5/onetl/db/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-10-10 11:38:46.462232 onetl-0.9.5/onetl/db/db_reader/
+-rw-r--r--   0 runner    (1001) docker     (127)      649 2023-10-10 11:38:18.000000 onetl-0.9.5/onetl/db/db_reader/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    22004 2023-10-10 11:38:18.000000 onetl-0.9.5/onetl/db/db_reader/db_reader.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8218 2023-10-10 11:38:18.000000 onetl-0.9.5/onetl/db/db_reader/strategy_helper.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-10-10 11:38:46.462232 onetl-0.9.5/onetl/db/db_writer/
+-rw-r--r--   0 runner    (1001) docker     (127)      649 2023-10-10 11:38:18.000000 onetl-0.9.5/onetl/db/db_writer/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6950 2023-10-10 11:38:18.000000 onetl-0.9.5/onetl/db/db_writer/db_writer.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3129 2023-10-10 11:38:18.000000 onetl-0.9.5/onetl/exception.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-10-10 11:38:46.462232 onetl-0.9.5/onetl/file/
+-rw-r--r--   0 runner    (1001) docker     (127)      891 2023-10-10 11:38:18.000000 onetl-0.9.5/onetl/file/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-10-10 11:38:46.466232 onetl-0.9.5/onetl/file/file_df_reader/
+-rw-r--r--   0 runner    (1001) docker     (127)      665 2023-10-10 11:38:18.000000 onetl-0.9.5/onetl/file/file_df_reader/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9741 2023-10-10 11:38:18.000000 onetl-0.9.5/onetl/file/file_df_reader/file_df_reader.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2795 2023-10-10 11:38:18.000000 onetl-0.9.5/onetl/file/file_df_reader/options.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-10-10 11:38:46.466232 onetl-0.9.5/onetl/file/file_df_writer/
+-rw-r--r--   0 runner    (1001) docker     (127)      665 2023-10-10 11:38:18.000000 onetl-0.9.5/onetl/file/file_df_writer/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4993 2023-10-10 11:38:18.000000 onetl-0.9.5/onetl/file/file_df_writer/file_df_writer.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11545 2023-10-10 11:38:18.000000 onetl-0.9.5/onetl/file/file_df_writer/options.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-10-10 11:38:46.466232 onetl-0.9.5/onetl/file/file_downloader/
+-rw-r--r--   0 runner    (1001) docker     (127)      799 2023-10-10 11:38:18.000000 onetl-0.9.5/onetl/file/file_downloader/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    29610 2023-10-10 11:38:18.000000 onetl-0.9.5/onetl/file/file_downloader/file_downloader.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2203 2023-10-10 11:38:18.000000 onetl-0.9.5/onetl/file/file_downloader/options.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2450 2023-10-10 11:38:18.000000 onetl-0.9.5/onetl/file/file_downloader/result.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-10-10 11:38:46.466232 onetl-0.9.5/onetl/file/file_mover/
+-rw-r--r--   0 runner    (1001) docker     (127)      765 2023-10-10 11:38:18.000000 onetl-0.9.5/onetl/file/file_mover/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    19634 2023-10-10 11:38:18.000000 onetl-0.9.5/onetl/file/file_mover/file_mover.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2000 2023-10-10 11:38:18.000000 onetl-0.9.5/onetl/file/file_mover/options.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2385 2023-10-10 11:38:18.000000 onetl-0.9.5/onetl/file/file_mover/result.py
+-rw-r--r--   0 runner    (1001) docker     (127)    18628 2023-10-10 11:38:18.000000 onetl-0.9.5/onetl/file/file_result.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5919 2023-10-10 11:38:18.000000 onetl-0.9.5/onetl/file/file_set.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-10-10 11:38:46.466232 onetl-0.9.5/onetl/file/file_uploader/
+-rw-r--r--   0 runner    (1001) docker     (127)      785 2023-10-10 11:38:18.000000 onetl-0.9.5/onetl/file/file_uploader/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    21738 2023-10-10 11:38:18.000000 onetl-0.9.5/onetl/file/file_uploader/file_uploader.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2188 2023-10-10 11:38:18.000000 onetl-0.9.5/onetl/file/file_uploader/options.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2408 2023-10-10 11:38:18.000000 onetl-0.9.5/onetl/file/file_uploader/result.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-10-10 11:38:46.470232 onetl-0.9.5/onetl/file/filter/
+-rw-r--r--   0 runner    (1001) docker     (127)      856 2023-10-10 11:38:18.000000 onetl-0.9.5/onetl/file/filter/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1988 2023-10-10 11:38:18.000000 onetl-0.9.5/onetl/file/filter/exclude_dir.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1421 2023-10-10 11:38:18.000000 onetl-0.9.5/onetl/file/filter/file_hwm.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1855 2023-10-10 11:38:18.000000 onetl-0.9.5/onetl/file/filter/glob.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2274 2023-10-10 11:38:18.000000 onetl-0.9.5/onetl/file/filter/match_all_filters.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2434 2023-10-10 11:38:18.000000 onetl-0.9.5/onetl/file/filter/regexp.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-10-10 11:38:46.470232 onetl-0.9.5/onetl/file/format/
+-rw-r--r--   0 runner    (1001) docker     (127)      930 2023-10-10 11:38:18.000000 onetl-0.9.5/onetl/file/format/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6444 2023-10-10 11:38:18.000000 onetl-0.9.5/onetl/file/format/avro.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3028 2023-10-10 11:38:18.000000 onetl-0.9.5/onetl/file/format/csv.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7270 2023-10-10 11:38:18.000000 onetl-0.9.5/onetl/file/format/excel.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1958 2023-10-10 11:38:18.000000 onetl-0.9.5/onetl/file/format/file_format.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3007 2023-10-10 11:38:18.000000 onetl-0.9.5/onetl/file/format/json.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2954 2023-10-10 11:38:18.000000 onetl-0.9.5/onetl/file/format/jsonline.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2125 2023-10-10 11:38:18.000000 onetl-0.9.5/onetl/file/format/orc.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2236 2023-10-10 11:38:18.000000 onetl-0.9.5/onetl/file/format/parquet.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7201 2023-10-10 11:38:18.000000 onetl-0.9.5/onetl/file/format/xml.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-10-10 11:38:46.474232 onetl-0.9.5/onetl/file/limit/
+-rw-r--r--   0 runner    (1001) docker     (127)      832 2023-10-10 11:38:18.000000 onetl-0.9.5/onetl/file/limit/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1920 2023-10-10 11:38:18.000000 onetl-0.9.5/onetl/file/limit/limits_reached.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1862 2023-10-10 11:38:18.000000 onetl-0.9.5/onetl/file/limit/limits_stop_at.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1987 2023-10-10 11:38:18.000000 onetl-0.9.5/onetl/file/limit/max_files_count.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1696 2023-10-10 11:38:18.000000 onetl-0.9.5/onetl/file/limit/reset_limits.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-10-10 11:38:46.474232 onetl-0.9.5/onetl/hooks/
+-rw-r--r--   0 runner    (1001) docker     (127)      219 2023-10-10 11:38:18.000000 onetl-0.9.5/onetl/hooks/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11851 2023-10-10 11:38:18.000000 onetl-0.9.5/onetl/hooks/hook.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6781 2023-10-10 11:38:18.000000 onetl-0.9.5/onetl/hooks/hook_collection.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3156 2023-10-10 11:38:18.000000 onetl-0.9.5/onetl/hooks/hooks_state.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2224 2023-10-10 11:38:18.000000 onetl-0.9.5/onetl/hooks/method_inheritance_stack.py
+-rw-r--r--   0 runner    (1001) docker     (127)    21270 2023-10-10 11:38:18.000000 onetl-0.9.5/onetl/hooks/slot.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4948 2023-10-10 11:38:18.000000 onetl-0.9.5/onetl/hooks/support_hooks.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-10-10 11:38:46.474232 onetl-0.9.5/onetl/hwm/
+-rw-r--r--   0 runner    (1001) docker     (127)       42 2023-10-10 11:38:18.000000 onetl-0.9.5/onetl/hwm/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      197 2023-10-10 11:38:18.000000 onetl-0.9.5/onetl/hwm/statement.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-10-10 11:38:46.474232 onetl-0.9.5/onetl/hwm/store/
+-rw-r--r--   0 runner    (1001) docker     (127)     1082 2023-10-10 11:38:18.000000 onetl-0.9.5/onetl/hwm/store/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3472 2023-10-10 11:38:18.000000 onetl-0.9.5/onetl/hwm/store/base_hwm_store.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3132 2023-10-10 11:38:18.000000 onetl-0.9.5/onetl/hwm/store/hwm_class_registry.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6828 2023-10-10 11:38:18.000000 onetl-0.9.5/onetl/hwm/store/hwm_store_class_registry.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1356 2023-10-10 11:38:18.000000 onetl-0.9.5/onetl/hwm/store/hwm_store_manager.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2863 2023-10-10 11:38:18.000000 onetl-0.9.5/onetl/hwm/store/memory_hwm_store.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6487 2023-10-10 11:38:18.000000 onetl-0.9.5/onetl/hwm/store/yaml_hwm_store.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-10-10 11:38:46.478232 onetl-0.9.5/onetl/impl/
+-rw-r--r--   0 runner    (1001) docker     (127)     1171 2023-10-10 11:38:18.000000 onetl-0.9.5/onetl/impl/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1952 2023-10-10 11:38:18.000000 onetl-0.9.5/onetl/impl/base_model.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1771 2023-10-10 11:38:18.000000 onetl-0.9.5/onetl/impl/failed_local_file.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1676 2023-10-10 11:38:18.000000 onetl-0.9.5/onetl/impl/file_exist_behavior.py
+-rw-r--r--   0 runner    (1001) docker     (127)      751 2023-10-10 11:38:18.000000 onetl-0.9.5/onetl/impl/frozen_model.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5093 2023-10-10 11:38:18.000000 onetl-0.9.5/onetl/impl/generic_options.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1028 2023-10-10 11:38:18.000000 onetl-0.9.5/onetl/impl/local_path.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3700 2023-10-10 11:38:18.000000 onetl-0.9.5/onetl/impl/path_container.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5384 2023-10-10 11:38:18.000000 onetl-0.9.5/onetl/impl/path_repr.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1865 2023-10-10 11:38:18.000000 onetl-0.9.5/onetl/impl/remote_directory.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2331 2023-10-10 11:38:18.000000 onetl-0.9.5/onetl/impl/remote_file.py
+-rw-r--r--   0 runner    (1001) docker     (127)      677 2023-10-10 11:38:18.000000 onetl-0.9.5/onetl/impl/remote_path.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1563 2023-10-10 11:38:18.000000 onetl-0.9.5/onetl/impl/remote_path_stat.py
+-rw-r--r--   0 runner    (1001) docker     (127)    14108 2023-10-10 11:38:18.000000 onetl-0.9.5/onetl/log.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-10-10 11:38:46.478232 onetl-0.9.5/onetl/plugins/
+-rw-r--r--   0 runner    (1001) docker     (127)       56 2023-10-10 11:38:18.000000 onetl-0.9.5/onetl/plugins/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4464 2023-10-10 11:38:18.000000 onetl-0.9.5/onetl/plugins/import_plugins.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-10-10 11:38:46.482232 onetl-0.9.5/onetl/strategy/
+-rw-r--r--   0 runner    (1001) docker     (127)      905 2023-10-10 11:38:18.000000 onetl-0.9.5/onetl/strategy/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2420 2023-10-10 11:38:18.000000 onetl-0.9.5/onetl/strategy/base_strategy.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5059 2023-10-10 11:38:18.000000 onetl-0.9.5/onetl/strategy/batch_hwm_strategy.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-10-10 11:38:46.482232 onetl-0.9.5/onetl/strategy/hwm_store/
+-rw-r--r--   0 runner    (1001) docker     (127)     1819 2023-10-10 11:38:18.000000 onetl-0.9.5/onetl/strategy/hwm_store/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3978 2023-10-10 11:38:18.000000 onetl-0.9.5/onetl/strategy/hwm_strategy.py
+-rw-r--r--   0 runner    (1001) docker     (127)    19405 2023-10-10 11:38:18.000000 onetl-0.9.5/onetl/strategy/incremental_strategy.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12810 2023-10-10 11:38:18.000000 onetl-0.9.5/onetl/strategy/snapshot_strategy.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1391 2023-10-10 11:38:18.000000 onetl-0.9.5/onetl/strategy/strategy_manager.py
+-rw-r--r--   0 runner    (1001) docker     (127)      814 2023-10-10 11:38:18.000000 onetl-0.9.5/onetl/version.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-10-10 11:38:46.386233 onetl-0.9.5/onetl.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)    29105 2023-10-10 11:38:46.000000 onetl-0.9.5/onetl.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     9800 2023-10-10 11:38:46.000000 onetl-0.9.5/onetl.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2023-10-10 11:38:46.000000 onetl-0.9.5/onetl.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2023-10-10 11:38:46.000000 onetl-0.9.5/onetl.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (127)      606 2023-10-10 11:38:46.000000 onetl-0.9.5/onetl.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        6 2023-10-10 11:38:46.000000 onetl-0.9.5/onetl.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)     1189 2023-10-10 11:38:18.000000 onetl-0.9.5/pyproject.toml
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-10-10 11:38:46.482232 onetl-0.9.5/requirements/
+-rw-r--r--   0 runner    (1001) docker     (127)      503 2023-10-10 11:38:18.000000 onetl-0.9.5/requirements/core.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       96 2023-10-10 11:38:18.000000 onetl-0.9.5/requirements/dev.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      233 2023-10-10 11:38:18.000000 onetl-0.9.5/requirements/docs.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       60 2023-10-10 11:38:18.000000 onetl-0.9.5/requirements/ftp.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        7 2023-10-10 11:38:18.000000 onetl-0.9.5/requirements/hdfs.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       85 2023-10-10 11:38:18.000000 onetl-0.9.5/requirements/kerberos.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        6 2023-10-10 11:38:18.000000 onetl-0.9.5/requirements/s3.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        6 2023-10-10 11:38:18.000000 onetl-0.9.5/requirements/samba.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        9 2023-10-10 11:38:18.000000 onetl-0.9.5/requirements/sftp.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        8 2023-10-10 11:38:18.000000 onetl-0.9.5/requirements/spark.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-10-10 11:38:46.486232 onetl-0.9.5/requirements/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)       79 2023-10-10 11:38:18.000000 onetl-0.9.5/requirements/tests/base.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       18 2023-10-10 11:38:18.000000 onetl-0.9.5/requirements/tests/clickhouse.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       16 2023-10-10 11:38:18.000000 onetl-0.9.5/requirements/tests/kafka.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        8 2023-10-10 11:38:18.000000 onetl-0.9.5/requirements/tests/mongodb.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       62 2023-10-10 11:38:18.000000 onetl-0.9.5/requirements/tests/mssql.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       13 2023-10-10 11:38:18.000000 onetl-0.9.5/requirements/tests/mysql.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       10 2023-10-10 11:38:18.000000 onetl-0.9.5/requirements/tests/oracle.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       16 2023-10-10 11:38:18.000000 onetl-0.9.5/requirements/tests/postgres.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        6 2023-10-10 11:38:18.000000 onetl-0.9.5/requirements/tests/samba.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       86 2023-10-10 11:38:18.000000 onetl-0.9.5/requirements/tests/spark-2.3.1.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       86 2023-10-10 11:38:18.000000 onetl-0.9.5/requirements/tests/spark-2.4.8.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       76 2023-10-10 11:38:18.000000 onetl-0.9.5/requirements/tests/spark-3.2.4.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       76 2023-10-10 11:38:18.000000 onetl-0.9.5/requirements/tests/spark-3.3.2.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       63 2023-10-10 11:38:18.000000 onetl-0.9.5/requirements/tests/spark-3.4.1.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       63 2023-10-10 11:38:18.000000 onetl-0.9.5/requirements/tests/spark-3.5.0.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       56 2023-10-10 11:38:18.000000 onetl-0.9.5/requirements/tests/spark-latest.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       14 2023-10-10 11:38:18.000000 onetl-0.9.5/requirements/webdav.txt
+-rw-r--r--   0 runner    (1001) docker     (127)     3243 2023-10-10 11:38:46.490232 onetl-0.9.5/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)     3935 2023-10-10 11:38:18.000000 onetl-0.9.5/setup.py
```

### Comparing `onetl-0.9.4/LICENSE.txt` & `onetl-0.9.5/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `onetl-0.9.4/PKG-INFO` & `onetl-0.9.5/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: onetl
-Version: 0.9.4
+Version: 0.9.5
 Summary: One ETL tool to rule them all
 Home-page: https://github.com/MobileTeleSystems/onetl
 Author: DataOps.ETL
 Author-email: onetools@mts.ru
 License: Apache License 2.0
 Project-URL: Documentation, https://onetl.readthedocs.io/
 Project-URL: Source, https://github.com/MobileTeleSystems/onetl
@@ -127,15 +127,15 @@
 * onETL is not a framework, as it does not have requirements to project structure, naming, the way of running ETL/ELT processes, configuration, etc. All of that should be implemented in some other tool.
 * onETL is deliberately developed without any integration with scheduling software like Apache Airflow. All integrations should be implemented as separated tools.
 * Only batch operations, no streaming. For streaming prefer `Apache Flink <https://flink.apache.org/>`_.
 
 Requirements
 ------------
 * **Python 3.7 - 3.11**
-* PySpark 2.3.x - 3.4.x (depends on used connector)
+* PySpark 2.3.x - 3.5.x (depends on used connector)
 * Java 8+ (required by Spark, see below)
 * Kerberos libs & GCC (required by ``Hive``, ``HDFS`` and ``SparkHDFS`` connectors)
 
 Supported storages
 ------------------
 
 +--------------------+--------------+----------------------------------------------------------------------------------------------------------------------+
@@ -171,15 +171,15 @@
 +                    +--------------+                                                                                                                      +
 |                    | FTPS         |                                                                                                                      |
 +                    +--------------+----------------------------------------------------------------------------------------------------------------------+
 |                    | WebDAV       | `WebdavClient3 library <https://pypi.org/project/webdavclient3/>`_                                                   |
 +                    +--------------+----------------------------------------------------------------------------------------------------------------------+
 |                    | Samba        | `pysmb library <https://pypi.org/project/pysmb/>`_                                                                   |
 +--------------------+--------------+----------------------------------------------------------------------------------------------------------------------+
-| Files as DataFrame | SparkLocalFS | Apache Spark `File Data Source <https://spark.apache.org/docs/3.4.1/sql-data-sources-generic-options.html>`_         |
+| Files as DataFrame | SparkLocalFS | Apache Spark `File Data Source <https://spark.apache.org/docs/latest/sql-data-sources-generic-options.html>`_        |
 |                    +--------------+                                                                                                                      +
 |                    | SparkHDFS    |                                                                                                                      |
 |                    +--------------+----------------------------------------------------------------------------------------------------------------------+
 |                    | SparkS3      | `Hadoop AWS <https://hadoop.apache.org/docs/current3/hadoop-aws/tools/hadoop-aws/index.html>`_ library               |
 +--------------------+--------------+----------------------------------------------------------------------------------------------------------------------+
 
 
@@ -254,28 +254,30 @@
 +--------------------------------------------------------------+-------------+-------------+-------+
 | `3.2.x <https://spark.apache.org/docs/3.2.4/#downloading>`_  | 3.7 - 3.10  | 8u201 - 11  | 2.12  |
 +--------------------------------------------------------------+-------------+-------------+-------+
 | `3.3.x <https://spark.apache.org/docs/3.3.3/#downloading>`_  | 3.7 - 3.10  | 8u201 - 17  | 2.12  |
 +--------------------------------------------------------------+-------------+-------------+-------+
 | `3.4.x <https://spark.apache.org/docs/3.4.1/#downloading>`_  | 3.7 - 3.11  | 8u362 - 20  | 2.12  |
 +--------------------------------------------------------------+-------------+-------------+-------+
+| `3.5.x <https://spark.apache.org/docs/3.5.0/#downloading>`_  | 3.8 - 3.11  | 8u371 - 20  | 2.12  |
++--------------------------------------------------------------+-------------+-------------+-------+
 
 .. _pyspark-install:
 
 Then you should install PySpark via passing ``spark`` to ``extras``:
 
 .. code:: bash
 
     pip install onetl[spark]  # install latest PySpark
 
 or install PySpark explicitly:
 
 .. code:: bash
 
-    pip install onetl pyspark==3.4.1  # install a specific PySpark version
+    pip install onetl pyspark==3.5.0  # install a specific PySpark version
 
 or inject PySpark to ``sys.path`` in some other way BEFORE creating a class instance.
 **Otherwise connection object cannot be created.**
 
 With File connections
 ~~~~~~~~~~~~~~~~~~~~~
 
@@ -605,15 +607,15 @@
     # Import onETL classes to write data
     from onetl.db import DBWriter
 
     # change logging level to INFO, and set up default logging format and handler
     setup_logging()
 
     # Initialize new SparkSession with Hadoop AWS libraries and Postgres driver loaded
-    maven_packages = SparkS3.get_packages(spark_version="3.4.1") + Postgres.get_packages()
+    maven_packages = SparkS3.get_packages(spark_version="3.5.0") + Postgres.get_packages()
     spark = (
         SparkSession.builder.appName("spark_app_onetl_demo")
         .config("spark.jars.packages", ",".join(maven_packages))
         .getOrCreate()
     )
 
     # Initialize S3 connection and check it
```

### Comparing `onetl-0.9.4/README.rst` & `onetl-0.9.5/README.rst`

 * *Files 2% similar despite different names*

```diff
@@ -48,15 +48,15 @@
 * onETL is not a framework, as it does not have requirements to project structure, naming, the way of running ETL/ELT processes, configuration, etc. All of that should be implemented in some other tool.
 * onETL is deliberately developed without any integration with scheduling software like Apache Airflow. All integrations should be implemented as separated tools.
 * Only batch operations, no streaming. For streaming prefer `Apache Flink <https://flink.apache.org/>`_.
 
 Requirements
 ------------
 * **Python 3.7 - 3.11**
-* PySpark 2.3.x - 3.4.x (depends on used connector)
+* PySpark 2.3.x - 3.5.x (depends on used connector)
 * Java 8+ (required by Spark, see below)
 * Kerberos libs & GCC (required by ``Hive``, ``HDFS`` and ``SparkHDFS`` connectors)
 
 Supported storages
 ------------------
 
 +--------------------+--------------+----------------------------------------------------------------------------------------------------------------------+
@@ -92,15 +92,15 @@
 +                    +--------------+                                                                                                                      +
 |                    | FTPS         |                                                                                                                      |
 +                    +--------------+----------------------------------------------------------------------------------------------------------------------+
 |                    | WebDAV       | `WebdavClient3 library <https://pypi.org/project/webdavclient3/>`_                                                   |
 +                    +--------------+----------------------------------------------------------------------------------------------------------------------+
 |                    | Samba        | `pysmb library <https://pypi.org/project/pysmb/>`_                                                                   |
 +--------------------+--------------+----------------------------------------------------------------------------------------------------------------------+
-| Files as DataFrame | SparkLocalFS | Apache Spark `File Data Source <https://spark.apache.org/docs/3.4.1/sql-data-sources-generic-options.html>`_         |
+| Files as DataFrame | SparkLocalFS | Apache Spark `File Data Source <https://spark.apache.org/docs/latest/sql-data-sources-generic-options.html>`_        |
 |                    +--------------+                                                                                                                      +
 |                    | SparkHDFS    |                                                                                                                      |
 |                    +--------------+----------------------------------------------------------------------------------------------------------------------+
 |                    | SparkS3      | `Hadoop AWS <https://hadoop.apache.org/docs/current3/hadoop-aws/tools/hadoop-aws/index.html>`_ library               |
 +--------------------+--------------+----------------------------------------------------------------------------------------------------------------------+
 
 
@@ -175,28 +175,30 @@
 +--------------------------------------------------------------+-------------+-------------+-------+
 | `3.2.x <https://spark.apache.org/docs/3.2.4/#downloading>`_  | 3.7 - 3.10  | 8u201 - 11  | 2.12  |
 +--------------------------------------------------------------+-------------+-------------+-------+
 | `3.3.x <https://spark.apache.org/docs/3.3.3/#downloading>`_  | 3.7 - 3.10  | 8u201 - 17  | 2.12  |
 +--------------------------------------------------------------+-------------+-------------+-------+
 | `3.4.x <https://spark.apache.org/docs/3.4.1/#downloading>`_  | 3.7 - 3.11  | 8u362 - 20  | 2.12  |
 +--------------------------------------------------------------+-------------+-------------+-------+
+| `3.5.x <https://spark.apache.org/docs/3.5.0/#downloading>`_  | 3.8 - 3.11  | 8u371 - 20  | 2.12  |
++--------------------------------------------------------------+-------------+-------------+-------+
 
 .. _pyspark-install:
 
 Then you should install PySpark via passing ``spark`` to ``extras``:
 
 .. code:: bash
 
     pip install onetl[spark]  # install latest PySpark
 
 or install PySpark explicitly:
 
 .. code:: bash
 
-    pip install onetl pyspark==3.4.1  # install a specific PySpark version
+    pip install onetl pyspark==3.5.0  # install a specific PySpark version
 
 or inject PySpark to ``sys.path`` in some other way BEFORE creating a class instance.
 **Otherwise connection object cannot be created.**
 
 With File connections
 ~~~~~~~~~~~~~~~~~~~~~
 
@@ -526,15 +528,15 @@
     # Import onETL classes to write data
     from onetl.db import DBWriter
 
     # change logging level to INFO, and set up default logging format and handler
     setup_logging()
 
     # Initialize new SparkSession with Hadoop AWS libraries and Postgres driver loaded
-    maven_packages = SparkS3.get_packages(spark_version="3.4.1") + Postgres.get_packages()
+    maven_packages = SparkS3.get_packages(spark_version="3.5.0") + Postgres.get_packages()
     spark = (
         SparkSession.builder.appName("spark_app_onetl_demo")
         .config("spark.jars.packages", ",".join(maven_packages))
         .getOrCreate()
     )
 
     # Initialize S3 connection and check it
```

### Comparing `onetl-0.9.4/onetl/__init__.py` & `onetl-0.9.5/onetl/__init__.py`

 * *Files identical despite different names*

### Comparing `onetl-0.9.4/onetl/_internal.py` & `onetl-0.9.5/onetl/_internal.py`

 * *Files identical despite different names*

### Comparing `onetl-0.9.4/onetl/_util/classproperty.py` & `onetl-0.9.5/onetl/_util/classproperty.py`

 * *Files identical despite different names*

### Comparing `onetl-0.9.4/onetl/_util/file.py` & `onetl-0.9.5/onetl/_util/file.py`

 * *Files identical despite different names*

### Comparing `onetl-0.9.4/onetl/_util/hadoop.py` & `onetl-0.9.5/onetl/_util/hadoop.py`

 * *Files identical despite different names*

### Comparing `onetl-0.9.4/onetl/_util/java.py` & `onetl-0.9.5/onetl/_util/java.py`

 * *Files identical despite different names*

### Comparing `onetl-0.9.4/onetl/_util/scala.py` & `onetl-0.9.5/onetl/_util/scala.py`

 * *Files identical despite different names*

### Comparing `onetl-0.9.4/onetl/_util/spark.py` & `onetl-0.9.5/onetl/_util/spark.py`

 * *Files identical despite different names*

### Comparing `onetl-0.9.4/onetl/_util/version.py` & `onetl-0.9.5/onetl/_util/version.py`

 * *Files identical despite different names*

### Comparing `onetl-0.9.4/onetl/base/__init__.py` & `onetl-0.9.5/onetl/base/__init__.py`

 * *Files identical despite different names*

### Comparing `onetl-0.9.4/onetl/base/base_connection.py` & `onetl-0.9.5/onetl/base/base_connection.py`

 * *Files identical despite different names*

### Comparing `onetl-0.9.4/onetl/base/base_db_connection.py` & `onetl-0.9.5/onetl/base/base_db_connection.py`

 * *Files identical despite different names*

### Comparing `onetl-0.9.4/onetl/base/base_file_connection.py` & `onetl-0.9.5/onetl/base/base_file_connection.py`

 * *Files identical despite different names*

### Comparing `onetl-0.9.4/onetl/base/base_file_df_connection.py` & `onetl-0.9.5/onetl/base/base_file_df_connection.py`

 * *Files identical despite different names*

### Comparing `onetl-0.9.4/onetl/base/base_file_filter.py` & `onetl-0.9.5/onetl/base/base_file_filter.py`

 * *Files identical despite different names*

### Comparing `onetl-0.9.4/onetl/base/base_file_format.py` & `onetl-0.9.5/onetl/base/base_file_format.py`

 * *Files identical despite different names*

### Comparing `onetl-0.9.4/onetl/base/base_file_limit.py` & `onetl-0.9.5/onetl/base/base_file_limit.py`

 * *Files identical despite different names*

### Comparing `onetl-0.9.4/onetl/base/contains_exception.py` & `onetl-0.9.5/onetl/base/contains_exception.py`

 * *Files identical despite different names*

### Comparing `onetl-0.9.4/onetl/base/contains_get_df_schema.py` & `onetl-0.9.5/onetl/base/contains_get_df_schema.py`

 * *Files identical despite different names*

### Comparing `onetl-0.9.4/onetl/base/contains_get_min_max_bounds.py` & `onetl-0.9.5/onetl/base/contains_get_min_max_bounds.py`

 * *Files identical despite different names*

### Comparing `onetl-0.9.4/onetl/base/path_protocol.py` & `onetl-0.9.5/onetl/base/path_protocol.py`

 * *Files identical despite different names*

### Comparing `onetl-0.9.4/onetl/base/path_stat_protocol.py` & `onetl-0.9.5/onetl/base/path_stat_protocol.py`

 * *Files identical despite different names*

### Comparing `onetl-0.9.4/onetl/base/pure_path_protocol.py` & `onetl-0.9.5/onetl/base/pure_path_protocol.py`

 * *Files identical despite different names*

### Comparing `onetl-0.9.4/onetl/base/supports_rename_dir.py` & `onetl-0.9.5/onetl/base/supports_rename_dir.py`

 * *Files identical despite different names*

### Comparing `onetl-0.9.4/onetl/connection/__init__.py` & `onetl-0.9.5/onetl/connection/__init__.py`

 * *Files identical despite different names*

### Comparing `onetl-0.9.4/onetl/connection/db_connection/clickhouse/__init__.py` & `onetl-0.9.5/onetl/connection/db_connection/clickhouse/__init__.py`

 * *Files identical despite different names*

### Comparing `onetl-0.9.4/onetl/connection/db_connection/clickhouse/connection.py` & `onetl-0.9.5/onetl/connection/db_connection/clickhouse/connection.py`

 * *Files 0% similar despite different names*

```diff
@@ -42,15 +42,15 @@
 
     Based on Maven package ``ru.yandex.clickhouse:clickhouse-jdbc:0.3.2``
     (`official Clickhouse JDBC driver <https://github.com/ClickHouse/clickhouse-jdbc>`_).
 
     .. dropdown:: Version compatibility
 
         * Clickhouse server versions: 20.7 or higher
-        * Spark versions: 2.3.x - 3.4.x
+        * Spark versions: 2.3.x - 3.5.x
         * Java versions: 8 - 20
 
         See `official documentation <https://clickhouse.com/docs/en/integrations/java#jdbc-driver>`_.
 
     .. warning::
 
         To use Clickhouse connector you should have PySpark installed (or injected to ``sys.path``)
@@ -59,15 +59,15 @@
         You can install PySpark as follows:
 
         .. code:: bash
 
             pip install onetl[spark]  # latest PySpark version
 
             # or
-            pip install onetl pyspark=3.4.1  # pass specific PySpark version
+            pip install onetl pyspark=3.5.0  # pass specific PySpark version
 
         See :ref:`install-spark` installation instruction for more details.
 
     Parameters
     ----------
     host : str
         Host of Clickhouse database. For example: ``test.clickhouse.domain.com`` or ``193.168.1.11``
```

### Comparing `onetl-0.9.4/onetl/connection/db_connection/clickhouse/dialect.py` & `onetl-0.9.5/onetl/connection/db_connection/clickhouse/dialect.py`

 * *Files identical despite different names*

### Comparing `onetl-0.9.4/onetl/connection/db_connection/db_connection/__init__.py` & `onetl-0.9.5/onetl/connection/db_connection/db_connection/__init__.py`

 * *Files identical despite different names*

### Comparing `onetl-0.9.4/onetl/connection/db_connection/db_connection/connection.py` & `onetl-0.9.5/onetl/connection/db_connection/db_connection/connection.py`

 * *Files 10% similar despite different names*

```diff
@@ -13,15 +13,15 @@
 #  limitations under the License.
 
 from __future__ import annotations
 
 from logging import getLogger
 from typing import TYPE_CHECKING
 
-from pydantic import Field
+from pydantic import Field, validator
 
 from onetl._util.spark import try_import_pyspark
 from onetl.base import BaseDBConnection
 from onetl.connection.db_connection.db_connection.dialect import DBDialect
 from onetl.impl import FrozenModel
 from onetl.log import log_with_indent
 
@@ -44,12 +44,25 @@
 
         # avoid importing pyspark unless user called the constructor,
         # as we allow user to use `Connection.get_packages()` for creating Spark session
         refs = super()._forward_refs()
         refs["SparkSession"] = SparkSession
         return refs
 
+    @validator("spark")
+    def _check_spark_session_alive(cls, spark):
+        # https://stackoverflow.com/a/36044685
+        msg = "Spark session is stopped. Please recreate Spark session."
+        try:
+            if not spark._jsc.sc().isStopped():
+                return spark
+        except Exception as e:
+            # None has no attribute "something"
+            raise ValueError(msg) from e
+
+        raise ValueError(msg)
+
     def _log_parameters(self):
         log.info("|%s| Using connection parameters:", self.__class__.__name__)
         parameters = self.dict(exclude_none=True, exclude={"spark"})
         for attr, value in parameters.items():
             log_with_indent(log, "%s = %r", attr, value)
```

### Comparing `onetl-0.9.4/onetl/connection/db_connection/db_connection/dialect.py` & `onetl-0.9.5/onetl/connection/db_connection/db_connection/dialect.py`

 * *Files identical despite different names*

### Comparing `onetl-0.9.4/onetl/connection/db_connection/dialect_mixins/__init__.py` & `onetl-0.9.5/onetl/connection/db_connection/dialect_mixins/__init__.py`

 * *Files identical despite different names*

### Comparing `onetl-0.9.4/onetl/connection/db_connection/dialect_mixins/support_hint_str.py` & `onetl-0.9.5/onetl/connection/db_connection/dialect_mixins/support_hint_str.py`

 * *Files identical despite different names*

### Comparing `onetl-0.9.4/onetl/connection/db_connection/dialect_mixins/support_hwm_column_str.py` & `onetl-0.9.5/onetl/connection/db_connection/dialect_mixins/support_hwm_column_str.py`

 * *Files identical despite different names*

### Comparing `onetl-0.9.4/onetl/connection/db_connection/dialect_mixins/support_hwm_expression_str.py` & `onetl-0.9.5/onetl/connection/db_connection/dialect_mixins/support_hwm_expression_str.py`

 * *Files identical despite different names*

### Comparing `onetl-0.9.4/onetl/connection/db_connection/dialect_mixins/support_where_none.py` & `onetl-0.9.5/onetl/connection/db_connection/dialect_mixins/support_where_none.py`

 * *Files identical despite different names*

### Comparing `onetl-0.9.4/onetl/connection/db_connection/dialect_mixins/support_where_str.py` & `onetl-0.9.5/onetl/connection/db_connection/dialect_mixins/support_where_str.py`

 * *Files identical despite different names*

### Comparing `onetl-0.9.4/onetl/connection/db_connection/greenplum/__init__.py` & `onetl-0.9.5/onetl/connection/db_connection/greenplum/__init__.py`

 * *Files identical despite different names*

### Comparing `onetl-0.9.4/onetl/connection/db_connection/greenplum/connection.py` & `onetl-0.9.5/onetl/connection/db_connection/greenplum/connection.py`

 * *Files identical despite different names*

### Comparing `onetl-0.9.4/onetl/connection/db_connection/greenplum/connection_limit.py` & `onetl-0.9.5/onetl/connection/db_connection/greenplum/connection_limit.py`

 * *Files identical despite different names*

### Comparing `onetl-0.9.4/onetl/connection/db_connection/greenplum/dialect.py` & `onetl-0.9.5/onetl/connection/db_connection/greenplum/dialect.py`

 * *Files identical despite different names*

### Comparing `onetl-0.9.4/onetl/connection/db_connection/greenplum/options.py` & `onetl-0.9.5/onetl/connection/db_connection/greenplum/options.py`

 * *Files identical despite different names*

### Comparing `onetl-0.9.4/onetl/connection/db_connection/hive/__init__.py` & `onetl-0.9.5/onetl/connection/db_connection/hive/__init__.py`

 * *Files identical despite different names*

### Comparing `onetl-0.9.4/onetl/connection/db_connection/hive/connection.py` & `onetl-0.9.5/onetl/connection/db_connection/hive/connection.py`

 * *Files 0% similar despite different names*

```diff
@@ -48,30 +48,30 @@
     """Spark connection with Hive MetaStore support. |support_hooks|
 
     You don't need a Hive server to use this connector.
 
     .. dropdown:: Version compatibility
 
         * Hive metastore version: 0.12 - 3.1.2 (may require to add proper .jar file explicitly)
-        * Spark versions: 2.3.x - 3.4.x
+        * Spark versions: 2.3.x - 3.5.x
         * Java versions: 8 - 20
 
     .. warning::
 
         To use Hive connector you should have PySpark installed (or injected to ``sys.path``)
         BEFORE creating the connector instance.
 
         You can install PySpark as follows:
 
         .. code:: bash
 
             pip install onetl[spark]  # latest PySpark version
 
             # or
-            pip install onetl pyspark=3.4.1  # pass specific PySpark version
+            pip install onetl pyspark=3.5.0  # pass specific PySpark version
 
         See :ref:`install-spark` installation instruction for more details.
 
     .. warning::
 
         This connector requires some additional configuration files to be present (``hive-site.xml`` and so on),
         as well as .jar files with Hive MetaStore client.
@@ -142,15 +142,15 @@
     Dialect = HiveDialect
     WriteOptions = HiveWriteOptions
     Options = HiveLegacyOptions
     Slots = HiveSlots
     # TODO: remove in v1.0.0
     slots = HiveSlots
 
-    _CHECK_QUERY: ClassVar[str] = "SELECT 1"
+    _CHECK_QUERY: ClassVar[str] = "SHOW DATABASES"
 
     @slot
     @classmethod
     def get_current(cls, spark: SparkSession):
         """
         Create connection for current cluster. |support_hooks|
 
@@ -203,15 +203,15 @@
         log.info("|%s| Checking connection availability...", self.__class__.__name__)
         self._log_parameters()
 
         log.debug("|%s| Executing SQL query:", self.__class__.__name__)
         log_lines(log, self._CHECK_QUERY, level=logging.DEBUG)
 
         try:
-            self._execute_sql(self._CHECK_QUERY)
+            self._execute_sql(self._CHECK_QUERY).limit(1).collect()
             log.info("|%s| Connection is available.", self.__class__.__name__)
         except Exception as e:
             log.exception("|%s| Connection is unavailable", self.__class__.__name__)
             raise RuntimeError("Connection is unavailable") from e
 
         return self
```

### Comparing `onetl-0.9.4/onetl/connection/db_connection/hive/dialect.py` & `onetl-0.9.5/onetl/connection/db_connection/hive/dialect.py`

 * *Files identical despite different names*

### Comparing `onetl-0.9.4/onetl/connection/db_connection/hive/options.py` & `onetl-0.9.5/onetl/connection/db_connection/hive/options.py`

 * *Files identical despite different names*

### Comparing `onetl-0.9.4/onetl/connection/db_connection/hive/slots.py` & `onetl-0.9.5/onetl/connection/db_connection/hive/slots.py`

 * *Files identical despite different names*

### Comparing `onetl-0.9.4/onetl/connection/db_connection/jdbc_connection/__init__.py` & `onetl-0.9.5/onetl/connection/db_connection/jdbc_connection/__init__.py`

 * *Files identical despite different names*

### Comparing `onetl-0.9.4/onetl/connection/db_connection/jdbc_connection/connection.py` & `onetl-0.9.5/onetl/connection/db_connection/jdbc_connection/connection.py`

 * *Files identical despite different names*

### Comparing `onetl-0.9.4/onetl/connection/db_connection/jdbc_connection/dialect.py` & `onetl-0.9.5/onetl/connection/db_connection/jdbc_connection/dialect.py`

 * *Files identical despite different names*

### Comparing `onetl-0.9.4/onetl/connection/db_connection/jdbc_connection/options.py` & `onetl-0.9.5/onetl/connection/db_connection/jdbc_connection/options.py`

 * *Files identical despite different names*

### Comparing `onetl-0.9.4/onetl/connection/db_connection/jdbc_mixin/__init__.py` & `onetl-0.9.5/onetl/connection/db_connection/jdbc_mixin/__init__.py`

 * *Files identical despite different names*

### Comparing `onetl-0.9.4/onetl/connection/db_connection/jdbc_mixin/connection.py` & `onetl-0.9.5/onetl/connection/db_connection/jdbc_mixin/connection.py`

 * *Files identical despite different names*

### Comparing `onetl-0.9.4/onetl/connection/db_connection/jdbc_mixin/options.py` & `onetl-0.9.5/onetl/connection/db_connection/jdbc_mixin/options.py`

 * *Files identical despite different names*

### Comparing `onetl-0.9.4/onetl/connection/db_connection/kafka/__init__.py` & `onetl-0.9.5/onetl/connection/db_connection/kafka/__init__.py`

 * *Files identical despite different names*

### Comparing `onetl-0.9.4/onetl/connection/db_connection/kafka/connection.py` & `onetl-0.9.5/onetl/connection/db_connection/kafka/connection.py`

 * *Files 0% similar despite different names*

```diff
@@ -67,15 +67,15 @@
     .. note::
 
         This connector is for batch download from kafka and not streaming.
 
     .. dropdown:: Version compatibility
 
         * Apache Kafka versions: 0.10 or higher
-        * Spark versions: 2.4.x - 3.4.x
+        * Spark versions: 2.4.x - 3.5.x
         * Scala versions: 2.11 - 2.13
 
     Parameters
     ----------
 
     addresses : list[str]
         A list of broker addresses, for example ``["192.168.1.10:9092", "192.168.1.11:9092"]``.
@@ -313,15 +313,15 @@
         if "topic" in df.columns:
             log.warning("The 'topic' column in the DataFrame will be overridden with value %r", target)
 
         write_options = {f"kafka.{key}": value for key, value in self._get_connection_properties().items()}
         write_options.update(options.dict(by_alias=True, exclude_none=True, exclude={"if_exists"}))
         write_options["topic"] = target
 
-        # As of Apache Spark version 3.4.1, the mode 'error' is not functioning as expected.
+        # As of Apache Spark version 3.5.0, the mode 'error' is not functioning as expected.
         # This issue has been reported and can be tracked at:
         # https://issues.apache.org/jira/browse/SPARK-44774
         mode = options.if_exists
         if mode == KafkaTopicExistBehaviorKafka.ERROR and target in self._get_topics():
             raise TargetAlreadyExistsError(f"Topic {target} already exists")
 
         log.info("|%s| Saving data to a topic %r", self.__class__.__name__, target)
```

### Comparing `onetl-0.9.4/onetl/connection/db_connection/kafka/dialect.py` & `onetl-0.9.5/onetl/connection/db_connection/kafka/dialect.py`

 * *Files identical despite different names*

### Comparing `onetl-0.9.4/onetl/connection/db_connection/kafka/extra.py` & `onetl-0.9.5/onetl/connection/db_connection/kafka/extra.py`

 * *Files identical despite different names*

### Comparing `onetl-0.9.4/onetl/connection/db_connection/kafka/kafka_auth.py` & `onetl-0.9.5/onetl/connection/db_connection/kafka/kafka_auth.py`

 * *Files identical despite different names*

### Comparing `onetl-0.9.4/onetl/connection/db_connection/kafka/kafka_basic_auth.py` & `onetl-0.9.5/onetl/connection/db_connection/kafka/kafka_basic_auth.py`

 * *Files identical despite different names*

### Comparing `onetl-0.9.4/onetl/connection/db_connection/kafka/kafka_kerberos_auth.py` & `onetl-0.9.5/onetl/connection/db_connection/kafka/kafka_kerberos_auth.py`

 * *Files identical despite different names*

### Comparing `onetl-0.9.4/onetl/connection/db_connection/kafka/kafka_plaintext_protocol.py` & `onetl-0.9.5/onetl/connection/db_connection/kafka/kafka_plaintext_protocol.py`

 * *Files identical despite different names*

### Comparing `onetl-0.9.4/onetl/connection/db_connection/kafka/kafka_protocol.py` & `onetl-0.9.5/onetl/connection/db_connection/kafka/kafka_protocol.py`

 * *Files identical despite different names*

### Comparing `onetl-0.9.4/onetl/connection/db_connection/kafka/kafka_scram_auth.py` & `onetl-0.9.5/onetl/connection/db_connection/kafka/kafka_scram_auth.py`

 * *Files identical despite different names*

### Comparing `onetl-0.9.4/onetl/connection/db_connection/kafka/kafka_ssl_protocol.py` & `onetl-0.9.5/onetl/connection/db_connection/kafka/kafka_ssl_protocol.py`

 * *Files identical despite different names*

### Comparing `onetl-0.9.4/onetl/connection/db_connection/kafka/options.py` & `onetl-0.9.5/onetl/connection/db_connection/kafka/options.py`

 * *Files identical despite different names*

### Comparing `onetl-0.9.4/onetl/connection/db_connection/kafka/slots.py` & `onetl-0.9.5/onetl/connection/db_connection/kafka/slots.py`

 * *Files identical despite different names*

### Comparing `onetl-0.9.4/onetl/connection/db_connection/mongodb/__init__.py` & `onetl-0.9.5/onetl/connection/db_connection/mongodb/__init__.py`

 * *Files identical despite different names*

### Comparing `onetl-0.9.4/onetl/connection/db_connection/mongodb/connection.py` & `onetl-0.9.5/onetl/connection/db_connection/mongodb/connection.py`

 * *Files 0% similar despite different names*

```diff
@@ -503,14 +503,15 @@
         mode = (
             "overwrite"
             if write_options.if_exists == MongoDBCollectionExistBehavior.REPLACE_ENTIRE_COLLECTION
             else "append"
         )
 
         if self._collection_exists(target):
+            # MongoDB connector does not support mode=ignore and mode=error
             if write_options.if_exists == MongoDBCollectionExistBehavior.ERROR:
                 raise ValueError("Operation stopped due to MongoDB.WriteOptions(if_exists='error')")
             elif write_options.if_exists == MongoDBCollectionExistBehavior.IGNORE:
                 log.info(
                     "|%s| Skip writing to existing collection because of MongoDB.WriteOptions(if_exists='ignore')",
                     self.__class__.__name__,
                 )
```

### Comparing `onetl-0.9.4/onetl/connection/db_connection/mongodb/dialect.py` & `onetl-0.9.5/onetl/connection/db_connection/mongodb/dialect.py`

 * *Files identical despite different names*

### Comparing `onetl-0.9.4/onetl/connection/db_connection/mongodb/options.py` & `onetl-0.9.5/onetl/connection/db_connection/mongodb/options.py`

 * *Files identical despite different names*

### Comparing `onetl-0.9.4/onetl/connection/db_connection/mssql/__init__.py` & `onetl-0.9.5/onetl/connection/db_connection/mssql/__init__.py`

 * *Files identical despite different names*

### Comparing `onetl-0.9.4/onetl/connection/db_connection/mssql/connection.py` & `onetl-0.9.5/onetl/connection/db_connection/mssql/connection.py`

 * *Files 1% similar despite different names*

```diff
@@ -40,15 +40,15 @@
     Based on Maven package ``com.microsoft.sqlserver:mssql-jdbc:12.2.0.jre8``
     (`official MSSQL JDBC driver
     <https://docs.microsoft.com/en-us/sql/connect/jdbc/download-microsoft-jdbc-driver-for-sql-server>`_).
 
     .. dropdown:: Version compatibility
 
         * SQL Server versions: 2014 - 2022
-        * Spark versions: 2.3.x - 3.4.x
+        * Spark versions: 2.3.x - 3.5.x
         * Java versions: 8 - 20
 
         See `official documentation <https://learn.microsoft.com/en-us/sql/connect/jdbc/system-requirements-for-the-jdbc-driver>`_
         and `official compatibility matrix <https://learn.microsoft.com/en-us/sql/connect/jdbc/microsoft-jdbc-driver-for-sql-server-support-matrix>`_.
 
     .. warning::
 
@@ -58,15 +58,15 @@
         You can install PySpark as follows:
 
         .. code:: bash
 
             pip install onetl[spark]  # latest PySpark version
 
             # or
-            pip install onetl pyspark=3.4.1  # pass specific PySpark version
+            pip install onetl pyspark=3.5.0  # pass specific PySpark version
 
         See :ref:`install-spark` installation instruction for more details.
 
     Parameters
     ----------
     host : str
         Host of MSSQL database. For example: ``test.mssql.domain.com`` or ``192.168.1.14``
```

### Comparing `onetl-0.9.4/onetl/connection/db_connection/mssql/dialect.py` & `onetl-0.9.5/onetl/connection/db_connection/mssql/dialect.py`

 * *Files identical despite different names*

### Comparing `onetl-0.9.4/onetl/connection/db_connection/mysql/__init__.py` & `onetl-0.9.5/onetl/connection/db_connection/mysql/__init__.py`

 * *Files identical despite different names*

### Comparing `onetl-0.9.4/onetl/connection/db_connection/mysql/connection.py` & `onetl-0.9.5/onetl/connection/db_connection/mysql/connection.py`

 * *Files 2% similar despite different names*

```diff
@@ -40,15 +40,15 @@
 
     Based on Maven package ``com.mysql:mysql-connector-j:8.0.33``
     (`official MySQL JDBC driver <https://dev.mysql.com/downloads/connector/j/8.0.html>`_).
 
     .. dropdown:: Version compatibility
 
         * MySQL server versions: 5.7, 8.0
-        * Spark versions: 2.3.x - 3.4.x
+        * Spark versions: 2.3.x - 3.5.x
         * Java versions: 8 - 20
 
         See `official documentation <https://dev.mysql.com/doc/connector-j/8.0/en/connector-j-versions.html>`_.
 
     .. warning::
 
         To use MySQL connector you should have PySpark installed (or injected to ``sys.path``)
@@ -57,15 +57,15 @@
         You can install PySpark as follows:
 
         .. code:: bash
 
             pip install onetl[spark]  # latest PySpark version
 
             # or
-            pip install onetl pyspark=3.4.1  # pass specific PySpark version
+            pip install onetl pyspark=3.5.0  # pass specific PySpark version
 
         See :ref:`install-spark` installation instruction for more details.
 
     Parameters
     ----------
     host : str
         Host of MySQL database. For example: ``mysql0012.domain.com`` or ``192.168.1.11``
```

### Comparing `onetl-0.9.4/onetl/connection/db_connection/mysql/dialect.py` & `onetl-0.9.5/onetl/connection/db_connection/mysql/dialect.py`

 * *Files identical despite different names*

### Comparing `onetl-0.9.4/onetl/connection/db_connection/oracle/__init__.py` & `onetl-0.9.5/onetl/connection/db_connection/oracle/__init__.py`

 * *Files identical despite different names*

### Comparing `onetl-0.9.4/onetl/connection/db_connection/oracle/connection.py` & `onetl-0.9.5/onetl/connection/db_connection/oracle/connection.py`

 * *Files 0% similar despite different names*

```diff
@@ -80,15 +80,15 @@
 
     Based on Maven package ``com.oracle.database.jdbc:ojdbc8:23.2.0.0``
     (`official Oracle JDBC driver <https://www.oracle.com/cis/database/technologies/appdev/jdbc-downloads.html>`_).
 
     .. dropdown:: Version compatibility
 
         * Oracle Server versions: 23c, 21c, 19c, 18c, 12.2 and probably 11.2 (tested, but that's not official).
-        * Spark versions: 2.3.x - 3.4.x
+        * Spark versions: 2.3.x - 3.5.x
         * Java versions: 8 - 20
 
         See `official documentation <https://www.oracle.com/cis/database/technologies/appdev/jdbc-downloads.html>`_.
 
     .. warning::
 
         To use Oracle connector you should have PySpark installed (or injected to ``sys.path``)
@@ -97,15 +97,15 @@
         You can install PySpark as follows:
 
         .. code:: bash
 
             pip install onetl[spark]  # latest PySpark version
 
             # or
-            pip install onetl pyspark=3.4.1  # pass specific PySpark version
+            pip install onetl pyspark=3.5.0  # pass specific PySpark version
 
         See :ref:`install-spark` installation instruction for more details.
 
     Parameters
     ----------
     host : str
         Host of Oracle database. For example: ``test.oracle.domain.com`` or ``193.168.1.10``
```

### Comparing `onetl-0.9.4/onetl/connection/db_connection/oracle/dialect.py` & `onetl-0.9.5/onetl/connection/db_connection/oracle/dialect.py`

 * *Files identical despite different names*

### Comparing `onetl-0.9.4/onetl/connection/db_connection/postgres/__init__.py` & `onetl-0.9.5/onetl/connection/db_connection/postgres/__init__.py`

 * *Files identical despite different names*

### Comparing `onetl-0.9.4/onetl/connection/db_connection/postgres/connection.py` & `onetl-0.9.5/onetl/connection/db_connection/postgres/connection.py`

 * *Files 0% similar despite different names*

```diff
@@ -38,15 +38,15 @@
 
     Based on Maven package ``org.postgresql:postgresql:42.6.0``
     (`official Postgres JDBC driver <https://jdbc.postgresql.org/>`_).
 
     .. dropdown:: Version compatibility
 
         * PostgreSQL server versions: 8.2 or higher
-        * Spark versions: 2.3.x - 3.4.x
+        * Spark versions: 2.3.x - 3.5.x
         * Java versions: 8 - 20
 
         See `official documentation <https://jdbc.postgresql.org/download/>`_.
 
     .. warning::
 
         To use Postgres connector you should have PySpark installed (or injected to ``sys.path``)
@@ -55,15 +55,15 @@
         You can install PySpark as follows:
 
         .. code:: bash
 
             pip install onetl[spark]  # latest PySpark version
 
             # or
-            pip install onetl pyspark=3.4.1  # pass specific PySpark version
+            pip install onetl pyspark=3.5.0  # pass specific PySpark version
 
         See :ref:`install-spark` installation instruction for more details.
 
     Parameters
     ----------
     host : str
         Host of Postgres database. For example: ``test.postgres.domain.com`` or ``193.168.1.11``
```

### Comparing `onetl-0.9.4/onetl/connection/db_connection/postgres/dialect.py` & `onetl-0.9.5/onetl/connection/db_connection/postgres/dialect.py`

 * *Files identical despite different names*

### Comparing `onetl-0.9.4/onetl/connection/db_connection/teradata/__init__.py` & `onetl-0.9.5/onetl/connection/db_connection/teradata/__init__.py`

 * *Files identical despite different names*

### Comparing `onetl-0.9.4/onetl/connection/db_connection/teradata/connection.py` & `onetl-0.9.5/onetl/connection/db_connection/teradata/connection.py`

 * *Files 1% similar despite different names*

```diff
@@ -43,15 +43,15 @@
 
     Based on package ``com.teradata.jdbc:terajdbc:17.20.00.15``
     (`official Teradata JDBC driver <https://downloads.teradata.com/download/connectivity/jdbc-driver>`_).
 
     .. dropdown:: Version compatibility
 
         * Teradata server versions: 16.10 - 20.0
-        * Spark versions: 2.3.x - 3.4.x
+        * Spark versions: 2.3.x - 3.5.x
         * Java versions: 8 - 20
 
         See `official documentation <https://teradata-docs.s3.amazonaws.com/doc/connectivity/jdbc/reference/current/platformMatrix.html>`_.
 
     .. warning::
 
         To use Teradata connector you should have PySpark installed (or injected to ``sys.path``)
@@ -60,15 +60,15 @@
         You can install PySpark as follows:
 
         .. code:: bash
 
             pip install onetl[spark]  # latest PySpark version
 
             # or
-            pip install onetl pyspark=3.4.1  # pass specific PySpark version
+            pip install onetl pyspark=3.5.0  # pass specific PySpark version
 
         See :ref:`install-spark` installation instruction for more details.
 
     Parameters
     ----------
     host : str
         Host of Teradata database. For example: ``test.teradata.domain.com`` or ``193.168.1.12``
```

### Comparing `onetl-0.9.4/onetl/connection/db_connection/teradata/dialect.py` & `onetl-0.9.5/onetl/connection/db_connection/teradata/dialect.py`

 * *Files identical despite different names*

### Comparing `onetl-0.9.4/onetl/connection/file_connection/file_connection.py` & `onetl-0.9.5/onetl/connection/file_connection/file_connection.py`

 * *Files identical despite different names*

### Comparing `onetl-0.9.4/onetl/connection/file_connection/ftp.py` & `onetl-0.9.5/onetl/connection/file_connection/ftp.py`

 * *Files identical despite different names*

### Comparing `onetl-0.9.4/onetl/connection/file_connection/ftps.py` & `onetl-0.9.5/onetl/connection/file_connection/ftps.py`

 * *Files identical despite different names*

### Comparing `onetl-0.9.4/onetl/connection/file_connection/hdfs/__init__.py` & `onetl-0.9.5/onetl/connection/file_connection/hdfs/__init__.py`

 * *Files identical despite different names*

### Comparing `onetl-0.9.4/onetl/connection/file_connection/hdfs/connection.py` & `onetl-0.9.5/onetl/connection/file_connection/hdfs/connection.py`

 * *Files identical despite different names*

### Comparing `onetl-0.9.4/onetl/connection/file_connection/hdfs/slots.py` & `onetl-0.9.5/onetl/connection/file_connection/hdfs/slots.py`

 * *Files identical despite different names*

### Comparing `onetl-0.9.4/onetl/connection/file_connection/mixins/__init__.py` & `onetl-0.9.5/onetl/connection/file_connection/mixins/__init__.py`

 * *Files identical despite different names*

### Comparing `onetl-0.9.4/onetl/connection/file_connection/mixins/rename_dir_mixin.py` & `onetl-0.9.5/onetl/connection/file_connection/mixins/rename_dir_mixin.py`

 * *Files identical despite different names*

### Comparing `onetl-0.9.4/onetl/connection/file_connection/s3.py` & `onetl-0.9.5/onetl/connection/file_connection/s3.py`

 * *Files identical despite different names*

### Comparing `onetl-0.9.4/onetl/connection/file_connection/samba.py` & `onetl-0.9.5/onetl/connection/file_connection/samba.py`

 * *Files identical despite different names*

### Comparing `onetl-0.9.4/onetl/connection/file_connection/sftp.py` & `onetl-0.9.5/onetl/connection/file_connection/sftp.py`

 * *Files identical despite different names*

### Comparing `onetl-0.9.4/onetl/connection/file_connection/webdav.py` & `onetl-0.9.5/onetl/connection/file_connection/webdav.py`

 * *Files identical despite different names*

### Comparing `onetl-0.9.4/onetl/connection/file_df_connection/spark_file_df_connection.py` & `onetl-0.9.5/onetl/connection/file_df_connection/spark_file_df_connection.py`

 * *Files 4% similar despite different names*

```diff
@@ -15,15 +15,15 @@
 from __future__ import annotations
 
 from abc import abstractmethod
 from contextlib import AbstractContextManager, ExitStack
 from logging import getLogger
 from typing import TYPE_CHECKING
 
-from pydantic import Field
+from pydantic import Field, validator
 
 from onetl._util.hadoop import get_hadoop_config
 from onetl._util.spark import try_import_pyspark
 from onetl.base import (
     BaseFileDFConnection,
     BaseReadableFileFormat,
     BaseWritableFileFormat,
@@ -178,12 +178,25 @@
 
         # avoid importing pyspark unless user called the constructor,
         # as we allow user to use `Connection.get_packages()` for creating Spark session
         refs = super()._forward_refs()
         refs["SparkSession"] = SparkSession
         return refs
 
+    @validator("spark")
+    def _check_spark_session_alive(cls, spark):
+        # https://stackoverflow.com/a/36044685
+        msg = "Spark session is stopped. Please recreate Spark session."
+        try:
+            if not spark._jsc.sc().isStopped():
+                return spark
+        except Exception as e:
+            # None has no attribute "something"
+            raise ValueError(msg) from e
+
+        raise ValueError(msg)
+
     def _log_parameters(self):
         log.info("|%s| Using connection parameters:", self.__class__.__name__)
         parameters = self.dict(exclude_none=True, exclude={"spark"})
         for attr, value in parameters.items():
             log_with_indent(log, "%s = %r", attr, value)
```

### Comparing `onetl-0.9.4/onetl/connection/file_df_connection/spark_hdfs/__init__.py` & `onetl-0.9.5/onetl/connection/file_df_connection/spark_hdfs/__init__.py`

 * *Files identical despite different names*

### Comparing `onetl-0.9.4/onetl/connection/file_df_connection/spark_hdfs/connection.py` & `onetl-0.9.5/onetl/connection/file_df_connection/spark_hdfs/connection.py`

 * *Files 1% similar despite different names*

```diff
@@ -53,15 +53,15 @@
         You can install PySpark as follows:
 
         .. code:: bash
 
             pip install onetl[spark]  # latest PySpark version
 
             # or
-            pip install onetl pyspark=3.4.1  # pass specific PySpark version
+            pip install onetl pyspark=3.5.0  # pass specific PySpark version
 
         See :ref:`install-spark` installation instruction for more details.
 
     .. note::
 
         Most of Hadoop instances use Kerberos authentication. In this case, you should call ``kinit``
         **BEFORE** starting Spark session to generate Kerberos ticket. See :ref:`install-kerberos`.
```

### Comparing `onetl-0.9.4/onetl/connection/file_df_connection/spark_hdfs/slots.py` & `onetl-0.9.5/onetl/connection/file_df_connection/spark_hdfs/slots.py`

 * *Files identical despite different names*

### Comparing `onetl-0.9.4/onetl/connection/file_df_connection/spark_local_fs.py` & `onetl-0.9.5/onetl/connection/file_df_connection/spark_local_fs.py`

 * *Files 0% similar despite different names*

```diff
@@ -43,15 +43,15 @@
         You can install PySpark as follows:
 
         .. code:: bash
 
             pip install onetl[spark]  # latest PySpark version
 
             # or
-            pip install onetl pyspark=3.4.1  # pass specific PySpark version
+            pip install onetl pyspark=3.5.0  # pass specific PySpark version
 
         See :ref:`install-spark` installation instruction for more details.
 
     .. warning::
 
         Currently supports only Spark sessions created with option ``spark.master: local``.
```

### Comparing `onetl-0.9.4/onetl/connection/file_df_connection/spark_s3/__init__.py` & `onetl-0.9.5/onetl/connection/file_df_connection/spark_s3/__init__.py`

 * *Files identical despite different names*

### Comparing `onetl-0.9.4/onetl/connection/file_df_connection/spark_s3/connection.py` & `onetl-0.9.5/onetl/connection/file_df_connection/spark_s3/connection.py`

 * *Files 1% similar despite different names*

```diff
@@ -58,15 +58,15 @@
     Spark connection to S3 filesystem. |support_hooks|
 
     Based on `Hadoop-AWS module <https://hadoop.apache.org/docs/current3/hadoop-aws/tools/hadoop-aws/index.html>`_
     and `Spark integration with Cloud Infrastructures <https://spark.apache.org/docs/latest/cloud-integration.html>`_.
 
     .. dropdown:: Version compatibility
 
-        * Spark versions: 3.2.x - 3.4.x (only with Hadoop 3.x libraries)
+        * Spark versions: 3.2.x - 3.5.x (only with Hadoop 3.x libraries)
         * Java versions: 8 - 20
         * Scala versions: 2.11 - 2.13
 
     .. warning::
 
         See :ref:`spark-s3-troubleshooting` guide.
 
@@ -78,15 +78,15 @@
         You can install PySpark as follows:
 
         .. code:: bash
 
             pip install onetl[spark]  # latest PySpark version
 
             # or
-            pip install onetl pyspark=3.4.1  # pass specific PySpark version
+            pip install onetl pyspark=3.5.0  # pass specific PySpark version
 
         See :ref:`install-spark` installation instruction for more details.
 
     .. note::
 
         Supports only reading files as Spark DataFrame and writing DataFrame to files.
 
@@ -157,15 +157,15 @@
 
     .. code:: python
 
         from onetl.connection import SparkS3
         from pyspark.sql import SparkSession
 
         # Create Spark session with Hadoop AWS libraries loaded
-        maven_packages = SparkS3.get_packages(spark_version="3.4.1")
+        maven_packages = SparkS3.get_packages(spark_version="3.5.0")
         # Some dependencies are not used, but downloading takes a lot of time. Skipping them.
         excluded_packages = [
             "com.google.cloud.bigdataoss:gcs-connector",
             "org.apache.hadoop:hadoop-aliyun",
             "org.apache.hadoop:hadoop-azure-datalake",
             "org.apache.hadoop:hadoop-azure",
         ]
@@ -258,16 +258,16 @@
         Examples
         --------
 
         .. code:: python
 
             from onetl.connection import SparkS3
 
-            SparkS3.get_packages(spark_version="3.4.1")
-            SparkS3.get_packages(spark_version="3.4.1", scala_version="2.12")
+            SparkS3.get_packages(spark_version="3.5.0")
+            SparkS3.get_packages(spark_version="3.5.0", scala_version="2.12")
 
         """
 
         spark_ver = Version.parse(spark_version)
         if spark_ver.major < 3:
             # https://issues.apache.org/jira/browse/SPARK-23977
             raise ValueError(f"Spark version must be at least 3.x, got {spark_ver}")
```

### Comparing `onetl-0.9.4/onetl/connection/file_df_connection/spark_s3/extra.py` & `onetl-0.9.5/onetl/connection/file_df_connection/spark_s3/extra.py`

 * *Files identical despite different names*

### Comparing `onetl-0.9.4/onetl/connection/kerberos_helpers.py` & `onetl-0.9.5/onetl/connection/kerberos_helpers.py`

 * *Files identical despite different names*

### Comparing `onetl-0.9.4/onetl/core/__init__.py` & `onetl-0.9.5/onetl/core/__init__.py`

 * *Files identical despite different names*

### Comparing `onetl-0.9.4/onetl/core/file_filter/__init__.py` & `onetl-0.9.5/onetl/core/file_filter/__init__.py`

 * *Files identical despite different names*

### Comparing `onetl-0.9.4/onetl/core/file_filter/file_filter.py` & `onetl-0.9.5/onetl/core/file_filter/file_filter.py`

 * *Files identical despite different names*

### Comparing `onetl-0.9.4/onetl/core/file_limit/__init__.py` & `onetl-0.9.5/onetl/core/file_limit/__init__.py`

 * *Files identical despite different names*

### Comparing `onetl-0.9.4/onetl/core/file_limit/file_limit.py` & `onetl-0.9.5/onetl/core/file_limit/file_limit.py`

 * *Files identical despite different names*

### Comparing `onetl-0.9.4/onetl/db/__init__.py` & `onetl-0.9.5/onetl/db/__init__.py`

 * *Files identical despite different names*

### Comparing `onetl-0.9.4/onetl/db/db_reader/__init__.py` & `onetl-0.9.5/onetl/db/db_reader/__init__.py`

 * *Files identical despite different names*

### Comparing `onetl-0.9.4/onetl/db/db_reader/db_reader.py` & `onetl-0.9.5/onetl/db/db_reader/db_reader.py`

 * *Files identical despite different names*

### Comparing `onetl-0.9.4/onetl/db/db_reader/strategy_helper.py` & `onetl-0.9.5/onetl/db/db_reader/strategy_helper.py`

 * *Files identical despite different names*

### Comparing `onetl-0.9.4/onetl/db/db_writer/__init__.py` & `onetl-0.9.5/onetl/db/db_writer/__init__.py`

 * *Files identical despite different names*

### Comparing `onetl-0.9.4/onetl/db/db_writer/db_writer.py` & `onetl-0.9.5/onetl/db/db_writer/db_writer.py`

 * *Files identical despite different names*

### Comparing `onetl-0.9.4/onetl/exception.py` & `onetl-0.9.5/onetl/exception.py`

 * *Files identical despite different names*

### Comparing `onetl-0.9.4/onetl/file/__init__.py` & `onetl-0.9.5/onetl/file/__init__.py`

 * *Files identical despite different names*

### Comparing `onetl-0.9.4/onetl/file/file_df_reader/__init__.py` & `onetl-0.9.5/onetl/file/file_df_reader/__init__.py`

 * *Files identical despite different names*

### Comparing `onetl-0.9.4/onetl/file/file_df_reader/file_df_reader.py` & `onetl-0.9.5/onetl/file/file_df_reader/file_df_reader.py`

 * *Files identical despite different names*

### Comparing `onetl-0.9.4/onetl/file/file_df_reader/options.py` & `onetl-0.9.5/onetl/file/file_df_reader/options.py`

 * *Files identical despite different names*

### Comparing `onetl-0.9.4/onetl/file/file_df_writer/__init__.py` & `onetl-0.9.5/onetl/file/file_df_writer/__init__.py`

 * *Files identical despite different names*

### Comparing `onetl-0.9.4/onetl/file/file_df_writer/file_df_writer.py` & `onetl-0.9.5/onetl/file/file_df_writer/file_df_writer.py`

 * *Files identical despite different names*

### Comparing `onetl-0.9.4/onetl/file/file_df_writer/options.py` & `onetl-0.9.5/onetl/file/file_df_writer/options.py`

 * *Files identical despite different names*

### Comparing `onetl-0.9.4/onetl/file/file_downloader/__init__.py` & `onetl-0.9.5/onetl/file/file_downloader/__init__.py`

 * *Files identical despite different names*

### Comparing `onetl-0.9.4/onetl/file/file_downloader/file_downloader.py` & `onetl-0.9.5/onetl/file/file_downloader/file_downloader.py`

 * *Files identical despite different names*

### Comparing `onetl-0.9.4/onetl/file/file_downloader/options.py` & `onetl-0.9.5/onetl/file/file_downloader/options.py`

 * *Files 6% similar despite different names*

```diff
@@ -27,16 +27,16 @@
     if_exists: FileExistBehavior = Field(default=FileExistBehavior.ERROR, alias="mode")
     """
     How to handle existing files in the local directory.
 
     Possible values:
         * ``error`` (default) - do nothing, mark file as failed
         * ``ignore`` - do nothing, mark file as ignored
-        * ``overwrite`` - replace existing file with a new one
-        * ``delete_all`` - delete local directory content before downloading files
+        * ``replace_file`` - replace existing file with a new one
+        * ``replace_entire_directory`` - delete local directory content before downloading files
     """
 
     delete_source: bool = False
     """
     If ``True``, remove source file after successful download.
 
     If download failed, file will left intact.
```

### Comparing `onetl-0.9.4/onetl/file/file_downloader/result.py` & `onetl-0.9.5/onetl/file/file_downloader/result.py`

 * *Files identical despite different names*

### Comparing `onetl-0.9.4/onetl/file/file_mover/__init__.py` & `onetl-0.9.5/onetl/file/file_mover/__init__.py`

 * *Files identical despite different names*

### Comparing `onetl-0.9.4/onetl/file/file_mover/file_mover.py` & `onetl-0.9.5/onetl/file/file_mover/file_mover.py`

 * *Files identical despite different names*

### Comparing `onetl-0.9.4/onetl/file/file_mover/options.py` & `onetl-0.9.5/onetl/file/file_mover/options.py`

 * *Files 14% similar despite different names*

```diff
@@ -27,16 +27,16 @@
     if_exists: FileExistBehavior = Field(default=FileExistBehavior.ERROR, alias="mode")
     """
     How to handle existing files in the local directory.
 
     Possible values:
         * ``error`` (default) - do nothing, mark file as failed
         * ``ignore`` - do nothing, mark file as ignored
-        * ``overwrite`` - replace existing file with a new one
-        * ``delete_all`` - delete directory content before moving files
+        * ``replace_file`` - replace existing file with a new one
+        * ``replace_entire_directory`` - delete directory content before moving files
     """
 
     workers: int = Field(default=1, ge=1)
     """
     Number of workers to create for parallel file moving.
 
     1 (default) means files will me moved sequentially.
```

### Comparing `onetl-0.9.4/onetl/file/file_mover/result.py` & `onetl-0.9.5/onetl/file/file_mover/result.py`

 * *Files identical despite different names*

### Comparing `onetl-0.9.4/onetl/file/file_result.py` & `onetl-0.9.5/onetl/file/file_result.py`

 * *Files identical despite different names*

### Comparing `onetl-0.9.4/onetl/file/file_set.py` & `onetl-0.9.5/onetl/file/file_set.py`

 * *Files identical despite different names*

### Comparing `onetl-0.9.4/onetl/file/file_uploader/__init__.py` & `onetl-0.9.5/onetl/file/file_uploader/__init__.py`

 * *Files identical despite different names*

### Comparing `onetl-0.9.4/onetl/file/file_uploader/file_uploader.py` & `onetl-0.9.5/onetl/file/file_uploader/file_uploader.py`

 * *Files identical despite different names*

### Comparing `onetl-0.9.4/onetl/file/file_uploader/options.py` & `onetl-0.9.5/onetl/file/file_uploader/options.py`

 * *Files 4% similar despite different names*

```diff
@@ -27,16 +27,16 @@
     if_exists: FileExistBehavior = Field(default=FileExistBehavior.ERROR, alias="mode")
     """
     How to handle existing files in the target directory.
 
     Possible values:
         * ``error`` (default) - do nothing, mark file as failed
         * ``ignore`` - do nothing, mark file as ignored
-        * ``overwrite`` - replace existing file with a new one
-        * ``delete_all`` - delete local directory content before downloading files
+        * ``replace_file`` - replace existing file with a new one
+        * ``replace_entire_directory`` - delete local directory content before downloading files
     """
 
     delete_local: bool = False
     """
     If ``True``, remove local file after successful download.
 
     If download failed, file will left intact.
```

### Comparing `onetl-0.9.4/onetl/file/file_uploader/result.py` & `onetl-0.9.5/onetl/file/file_uploader/result.py`

 * *Files identical despite different names*

### Comparing `onetl-0.9.4/onetl/file/filter/__init__.py` & `onetl-0.9.5/onetl/file/filter/__init__.py`

 * *Files identical despite different names*

### Comparing `onetl-0.9.4/onetl/file/filter/exclude_dir.py` & `onetl-0.9.5/onetl/file/filter/exclude_dir.py`

 * *Files identical despite different names*

### Comparing `onetl-0.9.4/onetl/file/filter/file_hwm.py` & `onetl-0.9.5/onetl/file/filter/file_hwm.py`

 * *Files identical despite different names*

### Comparing `onetl-0.9.4/onetl/file/filter/glob.py` & `onetl-0.9.5/onetl/file/filter/glob.py`

 * *Files identical despite different names*

### Comparing `onetl-0.9.4/onetl/file/filter/match_all_filters.py` & `onetl-0.9.5/onetl/file/filter/match_all_filters.py`

 * *Files identical despite different names*

### Comparing `onetl-0.9.4/onetl/file/filter/regexp.py` & `onetl-0.9.5/onetl/file/filter/regexp.py`

 * *Files identical despite different names*

### Comparing `onetl-0.9.4/onetl/file/format/__init__.py` & `onetl-0.9.5/onetl/file/format/__init__.py`

 * *Files 8% similar despite different names*

```diff
@@ -16,7 +16,8 @@
 from onetl.file.format.avro import Avro
 from onetl.file.format.csv import CSV
 from onetl.file.format.excel import Excel
 from onetl.file.format.json import JSON
 from onetl.file.format.jsonline import JSONLine
 from onetl.file.format.orc import ORC
 from onetl.file.format.parquet import Parquet
+from onetl.file.format.xml import XML
```

### Comparing `onetl-0.9.4/onetl/file/format/avro.py` & `onetl-0.9.5/onetl/file/format/avro.py`

 * *Files 2% similar despite different names*

```diff
@@ -67,15 +67,15 @@
 
     Based on `Spark Avro <https://spark.apache.org/docs/latest/sql-data-sources-avro.html>`_ file format.
 
     Supports reading/writing files with ``.avro`` extension.
 
     .. dropdown:: Version compatibility
 
-        * Spark versions: 2.4.x - 3.4.x
+        * Spark versions: 2.4.x - 3.5.x
         * Java versions: 8 - 20
         * Scala versions: 2.11 - 2.13
 
         See documentation from link above.
 
     .. note ::
 
@@ -91,15 +91,15 @@
 
     .. code:: python
 
         from onetl.file.format import Avro
         from pyspark.sql import SparkSession
 
         # Create Spark session with Avro package loaded
-        maven_packages = Avro.get_packages(spark_version="3.4.1")
+        maven_packages = Avro.get_packages(spark_version="3.5.0")
         spark = (
             SparkSession.builder.appName("spark-app-name")
             .config("spark.jars.packages", ",".join(maven_packages))
             .getOrCreate()
         )
 
         # Describe file format
```

### Comparing `onetl-0.9.4/onetl/file/format/csv.py` & `onetl-0.9.5/onetl/file/format/csv.py`

 * *Files identical despite different names*

### Comparing `onetl-0.9.4/onetl/file/format/excel.py` & `onetl-0.9.5/onetl/file/format/excel.py`

 * *Files identical despite different names*

### Comparing `onetl-0.9.4/onetl/file/format/file_format.py` & `onetl-0.9.5/onetl/file/format/file_format.py`

 * *Files identical despite different names*

### Comparing `onetl-0.9.4/onetl/file/format/json.py` & `onetl-0.9.5/onetl/file/format/json.py`

 * *Files identical despite different names*

### Comparing `onetl-0.9.4/onetl/file/format/jsonline.py` & `onetl-0.9.5/onetl/file/format/jsonline.py`

 * *Files identical despite different names*

### Comparing `onetl-0.9.4/onetl/file/format/orc.py` & `onetl-0.9.5/onetl/file/format/orc.py`

 * *Files identical despite different names*

### Comparing `onetl-0.9.4/onetl/file/format/parquet.py` & `onetl-0.9.5/onetl/file/format/parquet.py`

 * *Files identical despite different names*

### Comparing `onetl-0.9.4/onetl/file/limit/__init__.py` & `onetl-0.9.5/onetl/file/limit/__init__.py`

 * *Files identical despite different names*

### Comparing `onetl-0.9.4/onetl/file/limit/limits_reached.py` & `onetl-0.9.5/onetl/file/limit/limits_reached.py`

 * *Files identical despite different names*

### Comparing `onetl-0.9.4/onetl/file/limit/limits_stop_at.py` & `onetl-0.9.5/onetl/file/limit/limits_stop_at.py`

 * *Files identical despite different names*

### Comparing `onetl-0.9.4/onetl/file/limit/max_files_count.py` & `onetl-0.9.5/onetl/file/limit/max_files_count.py`

 * *Files identical despite different names*

### Comparing `onetl-0.9.4/onetl/file/limit/reset_limits.py` & `onetl-0.9.5/onetl/file/limit/reset_limits.py`

 * *Files identical despite different names*

### Comparing `onetl-0.9.4/onetl/hooks/hook.py` & `onetl-0.9.5/onetl/hooks/hook.py`

 * *Files identical despite different names*

### Comparing `onetl-0.9.4/onetl/hooks/hook_collection.py` & `onetl-0.9.5/onetl/hooks/hook_collection.py`

 * *Files identical despite different names*

### Comparing `onetl-0.9.4/onetl/hooks/hooks_state.py` & `onetl-0.9.5/onetl/hooks/hooks_state.py`

 * *Files identical despite different names*

### Comparing `onetl-0.9.4/onetl/hooks/method_inheritance_stack.py` & `onetl-0.9.5/onetl/hooks/method_inheritance_stack.py`

 * *Files identical despite different names*

### Comparing `onetl-0.9.4/onetl/hooks/slot.py` & `onetl-0.9.5/onetl/hooks/slot.py`

 * *Files identical despite different names*

### Comparing `onetl-0.9.4/onetl/hooks/support_hooks.py` & `onetl-0.9.5/onetl/hooks/support_hooks.py`

 * *Files identical despite different names*

### Comparing `onetl-0.9.4/onetl/hwm/store/__init__.py` & `onetl-0.9.5/onetl/hwm/store/__init__.py`

 * *Files identical despite different names*

### Comparing `onetl-0.9.4/onetl/hwm/store/base_hwm_store.py` & `onetl-0.9.5/onetl/hwm/store/base_hwm_store.py`

 * *Files identical despite different names*

### Comparing `onetl-0.9.4/onetl/hwm/store/hwm_class_registry.py` & `onetl-0.9.5/onetl/hwm/store/hwm_class_registry.py`

 * *Files identical despite different names*

### Comparing `onetl-0.9.4/onetl/hwm/store/hwm_store_class_registry.py` & `onetl-0.9.5/onetl/hwm/store/hwm_store_class_registry.py`

 * *Files identical despite different names*

### Comparing `onetl-0.9.4/onetl/hwm/store/hwm_store_manager.py` & `onetl-0.9.5/onetl/hwm/store/hwm_store_manager.py`

 * *Files identical despite different names*

### Comparing `onetl-0.9.4/onetl/hwm/store/memory_hwm_store.py` & `onetl-0.9.5/onetl/hwm/store/memory_hwm_store.py`

 * *Files identical despite different names*

### Comparing `onetl-0.9.4/onetl/hwm/store/yaml_hwm_store.py` & `onetl-0.9.5/onetl/hwm/store/yaml_hwm_store.py`

 * *Files identical despite different names*

### Comparing `onetl-0.9.4/onetl/impl/__init__.py` & `onetl-0.9.5/onetl/impl/__init__.py`

 * *Files identical despite different names*

### Comparing `onetl-0.9.4/onetl/impl/base_model.py` & `onetl-0.9.5/onetl/impl/base_model.py`

 * *Files identical despite different names*

### Comparing `onetl-0.9.4/onetl/impl/failed_local_file.py` & `onetl-0.9.5/onetl/impl/failed_local_file.py`

 * *Files identical despite different names*

### Comparing `onetl-0.9.4/onetl/impl/file_exist_behavior.py` & `onetl-0.9.5/onetl/impl/file_exist_behavior.py`

 * *Files identical despite different names*

### Comparing `onetl-0.9.4/onetl/impl/frozen_model.py` & `onetl-0.9.5/onetl/impl/frozen_model.py`

 * *Files identical despite different names*

### Comparing `onetl-0.9.4/onetl/impl/generic_options.py` & `onetl-0.9.5/onetl/impl/generic_options.py`

 * *Files identical despite different names*

### Comparing `onetl-0.9.4/onetl/impl/local_path.py` & `onetl-0.9.5/onetl/impl/local_path.py`

 * *Files identical despite different names*

### Comparing `onetl-0.9.4/onetl/impl/path_container.py` & `onetl-0.9.5/onetl/impl/path_container.py`

 * *Files identical despite different names*

### Comparing `onetl-0.9.4/onetl/impl/path_repr.py` & `onetl-0.9.5/onetl/impl/path_repr.py`

 * *Files identical despite different names*

### Comparing `onetl-0.9.4/onetl/impl/remote_directory.py` & `onetl-0.9.5/onetl/impl/remote_directory.py`

 * *Files identical despite different names*

### Comparing `onetl-0.9.4/onetl/impl/remote_file.py` & `onetl-0.9.5/onetl/impl/remote_file.py`

 * *Files identical despite different names*

### Comparing `onetl-0.9.4/onetl/impl/remote_path.py` & `onetl-0.9.5/onetl/impl/remote_path.py`

 * *Files identical despite different names*

### Comparing `onetl-0.9.4/onetl/impl/remote_path_stat.py` & `onetl-0.9.5/onetl/impl/remote_path_stat.py`

 * *Files identical despite different names*

### Comparing `onetl-0.9.4/onetl/log.py` & `onetl-0.9.5/onetl/log.py`

 * *Files identical despite different names*

### Comparing `onetl-0.9.4/onetl/plugins/import_plugins.py` & `onetl-0.9.5/onetl/plugins/import_plugins.py`

 * *Files identical despite different names*

### Comparing `onetl-0.9.4/onetl/strategy/__init__.py` & `onetl-0.9.5/onetl/strategy/__init__.py`

 * *Files identical despite different names*

### Comparing `onetl-0.9.4/onetl/strategy/base_strategy.py` & `onetl-0.9.5/onetl/strategy/base_strategy.py`

 * *Files identical despite different names*

### Comparing `onetl-0.9.4/onetl/strategy/batch_hwm_strategy.py` & `onetl-0.9.5/onetl/strategy/batch_hwm_strategy.py`

 * *Files identical despite different names*

### Comparing `onetl-0.9.4/onetl/strategy/hwm_store/__init__.py` & `onetl-0.9.5/onetl/strategy/hwm_store/__init__.py`

 * *Files identical despite different names*

### Comparing `onetl-0.9.4/onetl/strategy/hwm_strategy.py` & `onetl-0.9.5/onetl/strategy/hwm_strategy.py`

 * *Files identical despite different names*

### Comparing `onetl-0.9.4/onetl/strategy/incremental_strategy.py` & `onetl-0.9.5/onetl/strategy/incremental_strategy.py`

 * *Files identical despite different names*

### Comparing `onetl-0.9.4/onetl/strategy/snapshot_strategy.py` & `onetl-0.9.5/onetl/strategy/snapshot_strategy.py`

 * *Files identical despite different names*

### Comparing `onetl-0.9.4/onetl/strategy/strategy_manager.py` & `onetl-0.9.5/onetl/strategy/strategy_manager.py`

 * *Files identical despite different names*

### Comparing `onetl-0.9.4/onetl/version.py` & `onetl-0.9.5/onetl/version.py`

 * *Files identical despite different names*

### Comparing `onetl-0.9.4/onetl.egg-info/PKG-INFO` & `onetl-0.9.5/onetl.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: onetl
-Version: 0.9.4
+Version: 0.9.5
 Summary: One ETL tool to rule them all
 Home-page: https://github.com/MobileTeleSystems/onetl
 Author: DataOps.ETL
 Author-email: onetools@mts.ru
 License: Apache License 2.0
 Project-URL: Documentation, https://onetl.readthedocs.io/
 Project-URL: Source, https://github.com/MobileTeleSystems/onetl
@@ -127,15 +127,15 @@
 * onETL is not a framework, as it does not have requirements to project structure, naming, the way of running ETL/ELT processes, configuration, etc. All of that should be implemented in some other tool.
 * onETL is deliberately developed without any integration with scheduling software like Apache Airflow. All integrations should be implemented as separated tools.
 * Only batch operations, no streaming. For streaming prefer `Apache Flink <https://flink.apache.org/>`_.
 
 Requirements
 ------------
 * **Python 3.7 - 3.11**
-* PySpark 2.3.x - 3.4.x (depends on used connector)
+* PySpark 2.3.x - 3.5.x (depends on used connector)
 * Java 8+ (required by Spark, see below)
 * Kerberos libs & GCC (required by ``Hive``, ``HDFS`` and ``SparkHDFS`` connectors)
 
 Supported storages
 ------------------
 
 +--------------------+--------------+----------------------------------------------------------------------------------------------------------------------+
@@ -171,15 +171,15 @@
 +                    +--------------+                                                                                                                      +
 |                    | FTPS         |                                                                                                                      |
 +                    +--------------+----------------------------------------------------------------------------------------------------------------------+
 |                    | WebDAV       | `WebdavClient3 library <https://pypi.org/project/webdavclient3/>`_                                                   |
 +                    +--------------+----------------------------------------------------------------------------------------------------------------------+
 |                    | Samba        | `pysmb library <https://pypi.org/project/pysmb/>`_                                                                   |
 +--------------------+--------------+----------------------------------------------------------------------------------------------------------------------+
-| Files as DataFrame | SparkLocalFS | Apache Spark `File Data Source <https://spark.apache.org/docs/3.4.1/sql-data-sources-generic-options.html>`_         |
+| Files as DataFrame | SparkLocalFS | Apache Spark `File Data Source <https://spark.apache.org/docs/latest/sql-data-sources-generic-options.html>`_        |
 |                    +--------------+                                                                                                                      +
 |                    | SparkHDFS    |                                                                                                                      |
 |                    +--------------+----------------------------------------------------------------------------------------------------------------------+
 |                    | SparkS3      | `Hadoop AWS <https://hadoop.apache.org/docs/current3/hadoop-aws/tools/hadoop-aws/index.html>`_ library               |
 +--------------------+--------------+----------------------------------------------------------------------------------------------------------------------+
 
 
@@ -254,28 +254,30 @@
 +--------------------------------------------------------------+-------------+-------------+-------+
 | `3.2.x <https://spark.apache.org/docs/3.2.4/#downloading>`_  | 3.7 - 3.10  | 8u201 - 11  | 2.12  |
 +--------------------------------------------------------------+-------------+-------------+-------+
 | `3.3.x <https://spark.apache.org/docs/3.3.3/#downloading>`_  | 3.7 - 3.10  | 8u201 - 17  | 2.12  |
 +--------------------------------------------------------------+-------------+-------------+-------+
 | `3.4.x <https://spark.apache.org/docs/3.4.1/#downloading>`_  | 3.7 - 3.11  | 8u362 - 20  | 2.12  |
 +--------------------------------------------------------------+-------------+-------------+-------+
+| `3.5.x <https://spark.apache.org/docs/3.5.0/#downloading>`_  | 3.8 - 3.11  | 8u371 - 20  | 2.12  |
++--------------------------------------------------------------+-------------+-------------+-------+
 
 .. _pyspark-install:
 
 Then you should install PySpark via passing ``spark`` to ``extras``:
 
 .. code:: bash
 
     pip install onetl[spark]  # install latest PySpark
 
 or install PySpark explicitly:
 
 .. code:: bash
 
-    pip install onetl pyspark==3.4.1  # install a specific PySpark version
+    pip install onetl pyspark==3.5.0  # install a specific PySpark version
 
 or inject PySpark to ``sys.path`` in some other way BEFORE creating a class instance.
 **Otherwise connection object cannot be created.**
 
 With File connections
 ~~~~~~~~~~~~~~~~~~~~~
 
@@ -605,15 +607,15 @@
     # Import onETL classes to write data
     from onetl.db import DBWriter
 
     # change logging level to INFO, and set up default logging format and handler
     setup_logging()
 
     # Initialize new SparkSession with Hadoop AWS libraries and Postgres driver loaded
-    maven_packages = SparkS3.get_packages(spark_version="3.4.1") + Postgres.get_packages()
+    maven_packages = SparkS3.get_packages(spark_version="3.5.0") + Postgres.get_packages()
     spark = (
         SparkSession.builder.appName("spark_app_onetl_demo")
         .config("spark.jars.packages", ",".join(maven_packages))
         .getOrCreate()
     )
 
     # Initialize S3 connection and check it
```

### Comparing `onetl-0.9.4/onetl.egg-info/SOURCES.txt` & `onetl-0.9.5/onetl.egg-info/SOURCES.txt`

 * *Files 1% similar despite different names*

```diff
@@ -176,14 +176,15 @@
 onetl/file/format/csv.py
 onetl/file/format/excel.py
 onetl/file/format/file_format.py
 onetl/file/format/json.py
 onetl/file/format/jsonline.py
 onetl/file/format/orc.py
 onetl/file/format/parquet.py
+onetl/file/format/xml.py
 onetl/file/limit/__init__.py
 onetl/file/limit/limits_reached.py
 onetl/file/limit/limits_stop_at.py
 onetl/file/limit/max_files_count.py
 onetl/file/limit/reset_limits.py
 onetl/hooks/__init__.py
 onetl/hooks/hook.py
@@ -245,8 +246,9 @@
 requirements/tests/postgres.txt
 requirements/tests/samba.txt
 requirements/tests/spark-2.3.1.txt
 requirements/tests/spark-2.4.8.txt
 requirements/tests/spark-3.2.4.txt
 requirements/tests/spark-3.3.2.txt
 requirements/tests/spark-3.4.1.txt
+requirements/tests/spark-3.5.0.txt
 requirements/tests/spark-latest.txt
```

### Comparing `onetl-0.9.4/onetl.egg-info/requires.txt` & `onetl-0.9.5/onetl.egg-info/requires.txt`

 * *Files identical despite different names*

### Comparing `onetl-0.9.4/pyproject.toml` & `onetl-0.9.5/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [tool.isort]
 profile = "black"
 multi_line_output = 3
 
 [tool.black]
 line-length = 120
-target-version = ['py37', 'py38', 'py39', 'py310', 'py311']
+target-version = ['py37', 'py38', 'py39', 'py310', 'py311', 'py312']
 include = '\.pyi?$'
 exclude = '''(\.eggs|\.git|\.mypy_cache|\.tox|\.venv|_build|buck-out|build|dist)'''
 
 [tool.towncrier]
 name = "onETL"
 package = "onetl"
 filename = "docs/changelog/NEXT_RELEASE.rst"
```

### Comparing `onetl-0.9.4/setup.cfg` & `onetl-0.9.5/setup.cfg`

 * *Files identical despite different names*

### Comparing `onetl-0.9.4/setup.py` & `onetl-0.9.5/setup.py`

 * *Files identical despite different names*

