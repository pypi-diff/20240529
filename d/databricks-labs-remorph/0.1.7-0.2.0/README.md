# Comparing `tmp/databricks_labs_remorph-0.1.7.tar.gz` & `tmp/databricks_labs_remorph-0.2.0.tar.gz`

## Comparing `databricks_labs_remorph-0.1.7.tar` & `databricks_labs_remorph-0.2.0.tar`

### file list

```diff
@@ -1,97 +1,108 @@
--rw-r--r--   0        0        0        3 2020-02-02 00:00:00.000000 databricks_labs_remorph-0.1.7/core/src/main/antlr4/com/databricks/labs/remorph/parsers/snowflake/.gitignore
--rw-r--r--   0        0        0    54055 2020-02-02 00:00:00.000000 databricks_labs_remorph-0.1.7/core/src/main/antlr4/com/databricks/labs/remorph/parsers/snowflake/SnowflakeLexer.g4
--rw-r--r--   0        0        0   112460 2020-02-02 00:00:00.000000 databricks_labs_remorph-0.1.7/core/src/main/antlr4/com/databricks/labs/remorph/parsers/snowflake/SnowflakeParser.g4
--rw-r--r--   0        0        0        3 2020-02-02 00:00:00.000000 databricks_labs_remorph-0.1.7/core/src/main/antlr4/com/databricks/labs/remorph/parsers/tsql/.gitignore
--rw-r--r--   0        0        0    71070 2020-02-02 00:00:00.000000 databricks_labs_remorph-0.1.7/core/src/main/antlr4/com/databricks/labs/remorph/parsers/tsql/TSqlLexer.g4
--rw-r--r--   0        0        0   207140 2020-02-02 00:00:00.000000 databricks_labs_remorph-0.1.7/core/src/main/antlr4/com/databricks/labs/remorph/parsers/tsql/TSqlParser.g4
--rw-r--r--   0        0        0       75 2020-02-02 00:00:00.000000 databricks_labs_remorph-0.1.7/core/src/main/scala/com/databricks/labs/remorph/Main.scala
--rw-r--r--   0        0        0      516 2020-02-02 00:00:00.000000 databricks_labs_remorph-0.1.7/core/src/main/scala/com/databricks/labs/remorph/parsers/IncompleteParser.scala
--rw-r--r--   0        0        0      278 2020-02-02 00:00:00.000000 databricks_labs_remorph-0.1.7/core/src/main/scala/com/databricks/labs/remorph/parsers/ParserCommon.scala
--rw-r--r--   0        0        0      408 2020-02-02 00:00:00.000000 databricks_labs_remorph-0.1.7/core/src/main/scala/com/databricks/labs/remorph/parsers/intermediate/Plan.scala
--rw-r--r--   0        0        0      356 2020-02-02 00:00:00.000000 databricks_labs_remorph-0.1.7/core/src/main/scala/com/databricks/labs/remorph/parsers/intermediate/TreeNode.scala
--rw-r--r--   0        0        0     2253 2020-02-02 00:00:00.000000 databricks_labs_remorph-0.1.7/core/src/main/scala/com/databricks/labs/remorph/parsers/intermediate/catalog.scala
--rw-r--r--   0        0        0     2758 2020-02-02 00:00:00.000000 databricks_labs_remorph-0.1.7/core/src/main/scala/com/databricks/labs/remorph/parsers/intermediate/commands.scala
--rw-r--r--   0        0        0      277 2020-02-02 00:00:00.000000 databricks_labs_remorph-0.1.7/core/src/main/scala/com/databricks/labs/remorph/parsers/intermediate/common.scala
--rw-r--r--   0        0        0     4545 2020-02-02 00:00:00.000000 databricks_labs_remorph-0.1.7/core/src/main/scala/com/databricks/labs/remorph/parsers/intermediate/expressions.scala
--rw-r--r--   0        0        0     5893 2020-02-02 00:00:00.000000 databricks_labs_remorph-0.1.7/core/src/main/scala/com/databricks/labs/remorph/parsers/intermediate/extensions.scala
--rw-r--r--   0        0        0     8466 2020-02-02 00:00:00.000000 databricks_labs_remorph-0.1.7/core/src/main/scala/com/databricks/labs/remorph/parsers/intermediate/relations.scala
--rw-r--r--   0        0        0     1317 2020-02-02 00:00:00.000000 databricks_labs_remorph-0.1.7/core/src/main/scala/com/databricks/labs/remorph/parsers/intermediate/types.scala
--rw-r--r--   0        0        0      389 2020-02-02 00:00:00.000000 databricks_labs_remorph-0.1.7/core/src/main/scala/com/databricks/labs/remorph/parsers/intermediate/unresolved.scala
--rw-r--r--   0        0        0     1315 2020-02-02 00:00:00.000000 databricks_labs_remorph-0.1.7/core/src/main/scala/com/databricks/labs/remorph/parsers/snowflake/DataTypeBuilder.scala
--rw-r--r--   0        0        0     2024 2020-02-02 00:00:00.000000 databricks_labs_remorph-0.1.7/core/src/main/scala/com/databricks/labs/remorph/parsers/snowflake/SnowflakeAstBuilder.scala
--rw-r--r--   0        0        0     6830 2020-02-02 00:00:00.000000 databricks_labs_remorph-0.1.7/core/src/main/scala/com/databricks/labs/remorph/parsers/snowflake/SnowflakeDDLBuilder.scala
--rw-r--r--   0        0        0    10725 2020-02-02 00:00:00.000000 databricks_labs_remorph-0.1.7/core/src/main/scala/com/databricks/labs/remorph/parsers/snowflake/SnowflakeExpressionBuilder.scala
--rw-r--r--   0        0        0     8581 2020-02-02 00:00:00.000000 databricks_labs_remorph-0.1.7/core/src/main/scala/com/databricks/labs/remorph/parsers/snowflake/SnowflakeRelationBuilder.scala
--rw-r--r--   0        0        0      531 2020-02-02 00:00:00.000000 databricks_labs_remorph-0.1.7/core/src/main/scala/com/databricks/labs/remorph/parsers/snowflake/package.scala
--rw-r--r--   0        0        0     1431 2020-02-02 00:00:00.000000 databricks_labs_remorph-0.1.7/core/src/main/scala/com/databricks/labs/remorph/parsers/tsql/TSqlAstBuilder.scala
--rw-r--r--   0        0        0     5777 2020-02-02 00:00:00.000000 databricks_labs_remorph-0.1.7/core/src/main/scala/com/databricks/labs/remorph/parsers/tsql/TSqlExpressionBuilder.scala
--rw-r--r--   0        0        0     2008 2020-02-02 00:00:00.000000 databricks_labs_remorph-0.1.7/core/src/main/scala/com/databricks/labs/remorph/parsers/tsql/TSqlRelationBuilder.scala
--rw-r--r--   0        0        0      159 2020-02-02 00:00:00.000000 databricks_labs_remorph-0.1.7/core/src/test/scala/com/databricks/labs/remorph/MainTest.scala
--rw-r--r--   0        0        0     1412 2020-02-02 00:00:00.000000 databricks_labs_remorph-0.1.7/core/src/test/scala/com/databricks/labs/remorph/parsers/ParserTestCommon.scala
--rw-r--r--   0        0        0     1466 2020-02-02 00:00:00.000000 databricks_labs_remorph-0.1.7/core/src/test/scala/com/databricks/labs/remorph/parsers/snowflake/DataTypeBuilderSpec.scala
--rw-r--r--   0        0        0    15017 2020-02-02 00:00:00.000000 databricks_labs_remorph-0.1.7/core/src/test/scala/com/databricks/labs/remorph/parsers/snowflake/SnowflakeAstBuilderSpec.scala
--rw-r--r--   0        0        0     9428 2020-02-02 00:00:00.000000 databricks_labs_remorph-0.1.7/core/src/test/scala/com/databricks/labs/remorph/parsers/snowflake/SnowflakeDDLBuilderSpec.scala
--rw-r--r--   0        0        0    12839 2020-02-02 00:00:00.000000 databricks_labs_remorph-0.1.7/core/src/test/scala/com/databricks/labs/remorph/parsers/snowflake/SnowflakeExpressionBuilderSpec.scala
--rw-r--r--   0        0        0      537 2020-02-02 00:00:00.000000 databricks_labs_remorph-0.1.7/core/src/test/scala/com/databricks/labs/remorph/parsers/snowflake/SnowflakeParserTestCommon.scala
--rw-r--r--   0        0        0     5919 2020-02-02 00:00:00.000000 databricks_labs_remorph-0.1.7/core/src/test/scala/com/databricks/labs/remorph/parsers/snowflake/SnowflakeRelationBuilderSpec.scala
--rw-r--r--   0        0        0     4720 2020-02-02 00:00:00.000000 databricks_labs_remorph-0.1.7/core/src/test/scala/com/databricks/labs/remorph/parsers/tsql/TSqlAstBuilderSpec.scala
--rw-r--r--   0        0        0     7189 2020-02-02 00:00:00.000000 databricks_labs_remorph-0.1.7/core/src/test/scala/com/databricks/labs/remorph/parsers/tsql/TSqlExpressionBuilderSpec.scala
--rw-r--r--   0        0        0      506 2020-02-02 00:00:00.000000 databricks_labs_remorph-0.1.7/core/src/test/scala/com/databricks/labs/remorph/parsers/tsql/TSqlParserTestCommon.scala
--rw-r--r--   0        0        0      261 2020-02-02 00:00:00.000000 databricks_labs_remorph-0.1.7/databricks/__init__.py
--rw-r--r--   0        0        0      261 2020-02-02 00:00:00.000000 databricks_labs_remorph-0.1.7/databricks/labs/__init__.py
--rw-r--r--   0        0        0       48 2020-02-02 00:00:00.000000 databricks_labs_remorph-0.1.7/databricks/labs/remorph/__about__.py
--rw-r--r--   0        0        0       78 2020-02-02 00:00:00.000000 databricks_labs_remorph-0.1.7/databricks/labs/remorph/__init__.py
--rw-r--r--   0        0        0     5082 2020-02-02 00:00:00.000000 databricks_labs_remorph-0.1.7/databricks/labs/remorph/cli.py
--rw-r--r--   0        0        0     1895 2020-02-02 00:00:00.000000 databricks_labs_remorph-0.1.7/databricks/labs/remorph/config.py
--rw-r--r--   0        0        0     8693 2020-02-02 00:00:00.000000 databricks_labs_remorph-0.1.7/databricks/labs/remorph/install.py
--rw-r--r--   0        0        0     1691 2020-02-02 00:00:00.000000 databricks_labs_remorph-0.1.7/databricks/labs/remorph/lineage.py
--rw-r--r--   0        0        0     1965 2020-02-02 00:00:00.000000 databricks_labs_remorph-0.1.7/databricks/labs/remorph/uninstall.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 databricks_labs_remorph-0.1.7/databricks/labs/remorph/coverage/__init__.py
--rw-r--r--   0        0        0     5749 2020-02-02 00:00:00.000000 databricks_labs_remorph-0.1.7/databricks/labs/remorph/coverage/commons.py
--rw-r--r--   0        0        0      799 2020-02-02 00:00:00.000000 databricks_labs_remorph-0.1.7/databricks/labs/remorph/coverage/remorph_snow_transpilation_coverage.py
--rw-r--r--   0        0        0      651 2020-02-02 00:00:00.000000 databricks_labs_remorph-0.1.7/databricks/labs/remorph/coverage/sqlglot_snow_transpilation_coverage.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 databricks_labs_remorph-0.1.7/databricks/labs/remorph/helpers/__init__.py
--rw-r--r--   0        0        0     1519 2020-02-02 00:00:00.000000 databricks_labs_remorph-0.1.7/databricks/labs/remorph/helpers/db_sql.py
--rw-r--r--   0        0        0      533 2020-02-02 00:00:00.000000 databricks_labs_remorph-0.1.7/databricks/labs/remorph/helpers/execution_time.py
--rw-r--r--   0        0        0     3913 2020-02-02 00:00:00.000000 databricks_labs_remorph-0.1.7/databricks/labs/remorph/helpers/file_utils.py
--rw-r--r--   0        0        0      378 2020-02-02 00:00:00.000000 databricks_labs_remorph-0.1.7/databricks/labs/remorph/helpers/morph_status.py
--rw-r--r--   0        0        0     7412 2020-02-02 00:00:00.000000 databricks_labs_remorph-0.1.7/databricks/labs/remorph/helpers/recon_config_utils.py
--rw-r--r--   0        0        0     4242 2020-02-02 00:00:00.000000 databricks_labs_remorph-0.1.7/databricks/labs/remorph/helpers/validation.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 databricks_labs_remorph-0.1.7/databricks/labs/remorph/intermediate/__init__.py
--rw-r--r--   0        0        0     3112 2020-02-02 00:00:00.000000 databricks_labs_remorph-0.1.7/databricks/labs/remorph/intermediate/dag.py
--rw-r--r--   0        0        0      913 2020-02-02 00:00:00.000000 databricks_labs_remorph-0.1.7/databricks/labs/remorph/intermediate/engine_adapter.py
--rw-r--r--   0        0        0     1394 2020-02-02 00:00:00.000000 databricks_labs_remorph-0.1.7/databricks/labs/remorph/intermediate/root_tables.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 databricks_labs_remorph-0.1.7/databricks/labs/remorph/reconcile/__init__.py
--rw-r--r--   0        0        0     4696 2020-02-02 00:00:00.000000 databricks_labs_remorph-0.1.7/databricks/labs/remorph/reconcile/compare.py
--rw-r--r--   0        0        0     2495 2020-02-02 00:00:00.000000 databricks_labs_remorph-0.1.7/databricks/labs/remorph/reconcile/constants.py
--rw-r--r--   0        0        0      127 2020-02-02 00:00:00.000000 databricks_labs_remorph-0.1.7/databricks/labs/remorph/reconcile/exception.py
--rw-r--r--   0        0        0     1307 2020-02-02 00:00:00.000000 databricks_labs_remorph-0.1.7/databricks/labs/remorph/reconcile/execute.py
--rw-r--r--   0        0        0     5635 2020-02-02 00:00:00.000000 databricks_labs_remorph-0.1.7/databricks/labs/remorph/reconcile/recon_config.py
--rw-r--r--   0        0        0     5049 2020-02-02 00:00:00.000000 databricks_labs_remorph-0.1.7/databricks/labs/remorph/reconcile/schema_compare.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 databricks_labs_remorph-0.1.7/databricks/labs/remorph/reconcile/connectors/__init__.py
--rw-r--r--   0        0        0     1967 2020-02-02 00:00:00.000000 databricks_labs_remorph-0.1.7/databricks/labs/remorph/reconcile/connectors/data_source.py
--rw-r--r--   0        0        0     2396 2020-02-02 00:00:00.000000 databricks_labs_remorph-0.1.7/databricks/labs/remorph/reconcile/connectors/databricks.py
--rw-r--r--   0        0        0     3806 2020-02-02 00:00:00.000000 databricks_labs_remorph-0.1.7/databricks/labs/remorph/reconcile/connectors/oracle.py
--rw-r--r--   0        0        0     3657 2020-02-02 00:00:00.000000 databricks_labs_remorph-0.1.7/databricks/labs/remorph/reconcile/connectors/snowflake.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 databricks_labs_remorph-0.1.7/databricks/labs/remorph/reconcile/query_builder/__init__.py
--rw-r--r--   0        0        0     4246 2020-02-02 00:00:00.000000 databricks_labs_remorph-0.1.7/databricks/labs/remorph/reconcile/query_builder/base.py
--rw-r--r--   0        0        0     8512 2020-02-02 00:00:00.000000 databricks_labs_remorph-0.1.7/databricks/labs/remorph/reconcile/query_builder/expression_generator.py
--rw-r--r--   0        0        0     1892 2020-02-02 00:00:00.000000 databricks_labs_remorph-0.1.7/databricks/labs/remorph/reconcile/query_builder/hash_query.py
--rw-r--r--   0        0        0     2333 2020-02-02 00:00:00.000000 databricks_labs_remorph-0.1.7/databricks/labs/remorph/reconcile/query_builder/sampling_query.py
--rw-r--r--   0        0        0     7481 2020-02-02 00:00:00.000000 databricks_labs_remorph-0.1.7/databricks/labs/remorph/reconcile/query_builder/threshold_query.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 databricks_labs_remorph-0.1.7/databricks/labs/remorph/snow/__init__.py
--rw-r--r--   0        0        0    26739 2020-02-02 00:00:00.000000 databricks_labs_remorph-0.1.7/databricks/labs/remorph/snow/databricks.py
--rw-r--r--   0        0        0      628 2020-02-02 00:00:00.000000 databricks_labs_remorph-0.1.7/databricks/labs/remorph/snow/experimental.py
--rw-r--r--   0        0        0     4805 2020-02-02 00:00:00.000000 databricks_labs_remorph-0.1.7/databricks/labs/remorph/snow/lca_utils.py
--rw-r--r--   0        0        0     3408 2020-02-02 00:00:00.000000 databricks_labs_remorph-0.1.7/databricks/labs/remorph/snow/local_expression.py
--rw-r--r--   0        0        0      315 2020-02-02 00:00:00.000000 databricks_labs_remorph-0.1.7/databricks/labs/remorph/snow/oracle.py
--rw-r--r--   0        0        0    22385 2020-02-02 00:00:00.000000 databricks_labs_remorph-0.1.7/databricks/labs/remorph/snow/snowflake.py
--rw-r--r--   0        0        0     2103 2020-02-02 00:00:00.000000 databricks_labs_remorph-0.1.7/databricks/labs/remorph/snow/sql_transpiler.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 databricks_labs_remorph-0.1.7/databricks/labs/remorph/transpiler/__init__.py
--rw-r--r--   0        0        0     7048 2020-02-02 00:00:00.000000 databricks_labs_remorph-0.1.7/databricks/labs/remorph/transpiler/execute.py
--rw-r--r--   0        0        0      117 2020-02-02 00:00:00.000000 databricks_labs_remorph-0.1.7/.gitignore
--rw-r--r--   0        0        0     3862 2020-02-02 00:00:00.000000 databricks_labs_remorph-0.1.7/LICENSE
--rw-r--r--   0        0        0     2238 2020-02-02 00:00:00.000000 databricks_labs_remorph-0.1.7/NOTICE
--rw-r--r--   0        0        0     6443 2020-02-02 00:00:00.000000 databricks_labs_remorph-0.1.7/README.md
--rw-r--r--   0        0        0    26966 2020-02-02 00:00:00.000000 databricks_labs_remorph-0.1.7/pyproject.toml
--rw-r--r--   0        0        0     7367 2020-02-02 00:00:00.000000 databricks_labs_remorph-0.1.7/PKG-INFO
+-rw-r--r--   0        0        0        3 2020-02-02 00:00:00.000000 databricks_labs_remorph-0.2.0/core/src/main/antlr4/com/databricks/labs/remorph/parsers/snowflake/.gitignore
+-rw-r--r--   0        0        0    54096 2020-02-02 00:00:00.000000 databricks_labs_remorph-0.2.0/core/src/main/antlr4/com/databricks/labs/remorph/parsers/snowflake/SnowflakeLexer.g4
+-rw-r--r--   0        0        0   113632 2020-02-02 00:00:00.000000 databricks_labs_remorph-0.2.0/core/src/main/antlr4/com/databricks/labs/remorph/parsers/snowflake/SnowflakeParser.g4
+-rw-r--r--   0        0        0        3 2020-02-02 00:00:00.000000 databricks_labs_remorph-0.2.0/core/src/main/antlr4/com/databricks/labs/remorph/parsers/tsql/.gitignore
+-rw-r--r--   0        0        0    59513 2020-02-02 00:00:00.000000 databricks_labs_remorph-0.2.0/core/src/main/antlr4/com/databricks/labs/remorph/parsers/tsql/TSqlLexer.g4
+-rw-r--r--   0        0        0   158742 2020-02-02 00:00:00.000000 databricks_labs_remorph-0.2.0/core/src/main/antlr4/com/databricks/labs/remorph/parsers/tsql/TSqlParser.g4
+-rw-r--r--   0        0        0       75 2020-02-02 00:00:00.000000 databricks_labs_remorph-0.2.0/core/src/main/scala/com/databricks/labs/remorph/Main.scala
+-rw-r--r--   0        0        0     3899 2020-02-02 00:00:00.000000 databricks_labs_remorph-0.2.0/core/src/main/scala/com/databricks/labs/remorph/parsers/ErrorCollector.scala
+-rw-r--r--   0        0        0    13194 2020-02-02 00:00:00.000000 databricks_labs_remorph-0.2.0/core/src/main/scala/com/databricks/labs/remorph/parsers/FunctionBuilder.scala
+-rw-r--r--   0        0        0      516 2020-02-02 00:00:00.000000 databricks_labs_remorph-0.2.0/core/src/main/scala/com/databricks/labs/remorph/parsers/IncompleteParser.scala
+-rw-r--r--   0        0        0      278 2020-02-02 00:00:00.000000 databricks_labs_remorph-0.2.0/core/src/main/scala/com/databricks/labs/remorph/parsers/ParserCommon.scala
+-rw-r--r--   0        0        0      408 2020-02-02 00:00:00.000000 databricks_labs_remorph-0.2.0/core/src/main/scala/com/databricks/labs/remorph/parsers/intermediate/Plan.scala
+-rw-r--r--   0        0        0      356 2020-02-02 00:00:00.000000 databricks_labs_remorph-0.2.0/core/src/main/scala/com/databricks/labs/remorph/parsers/intermediate/TreeNode.scala
+-rw-r--r--   0        0        0     2253 2020-02-02 00:00:00.000000 databricks_labs_remorph-0.2.0/core/src/main/scala/com/databricks/labs/remorph/parsers/intermediate/catalog.scala
+-rw-r--r--   0        0        0     2758 2020-02-02 00:00:00.000000 databricks_labs_remorph-0.2.0/core/src/main/scala/com/databricks/labs/remorph/parsers/intermediate/commands.scala
+-rw-r--r--   0        0        0      277 2020-02-02 00:00:00.000000 databricks_labs_remorph-0.2.0/core/src/main/scala/com/databricks/labs/remorph/parsers/intermediate/common.scala
+-rw-r--r--   0        0        0     4639 2020-02-02 00:00:00.000000 databricks_labs_remorph-0.2.0/core/src/main/scala/com/databricks/labs/remorph/parsers/intermediate/expressions.scala
+-rw-r--r--   0        0        0     8742 2020-02-02 00:00:00.000000 databricks_labs_remorph-0.2.0/core/src/main/scala/com/databricks/labs/remorph/parsers/intermediate/extensions.scala
+-rw-r--r--   0        0        0     8466 2020-02-02 00:00:00.000000 databricks_labs_remorph-0.2.0/core/src/main/scala/com/databricks/labs/remorph/parsers/intermediate/relations.scala
+-rw-r--r--   0        0        0     1399 2020-02-02 00:00:00.000000 databricks_labs_remorph-0.2.0/core/src/main/scala/com/databricks/labs/remorph/parsers/intermediate/types.scala
+-rw-r--r--   0        0        0      389 2020-02-02 00:00:00.000000 databricks_labs_remorph-0.2.0/core/src/main/scala/com/databricks/labs/remorph/parsers/intermediate/unresolved.scala
+-rw-r--r--   0        0        0     1315 2020-02-02 00:00:00.000000 databricks_labs_remorph-0.2.0/core/src/main/scala/com/databricks/labs/remorph/parsers/snowflake/DataTypeBuilder.scala
+-rw-r--r--   0        0        0     2024 2020-02-02 00:00:00.000000 databricks_labs_remorph-0.2.0/core/src/main/scala/com/databricks/labs/remorph/parsers/snowflake/SnowflakeAstBuilder.scala
+-rw-r--r--   0        0        0    10307 2020-02-02 00:00:00.000000 databricks_labs_remorph-0.2.0/core/src/main/scala/com/databricks/labs/remorph/parsers/snowflake/SnowflakeDDLBuilder.scala
+-rw-r--r--   0        0        0    14821 2020-02-02 00:00:00.000000 databricks_labs_remorph-0.2.0/core/src/main/scala/com/databricks/labs/remorph/parsers/snowflake/SnowflakeExpressionBuilder.scala
+-rw-r--r--   0        0        0     8649 2020-02-02 00:00:00.000000 databricks_labs_remorph-0.2.0/core/src/main/scala/com/databricks/labs/remorph/parsers/snowflake/SnowflakeRelationBuilder.scala
+-rw-r--r--   0        0        0      531 2020-02-02 00:00:00.000000 databricks_labs_remorph-0.2.0/core/src/main/scala/com/databricks/labs/remorph/parsers/snowflake/package.scala
+-rw-r--r--   0        0        0     1379 2020-02-02 00:00:00.000000 databricks_labs_remorph-0.2.0/core/src/main/scala/com/databricks/labs/remorph/parsers/tsql/TSqlAstBuilder.scala
+-rw-r--r--   0        0        0    15726 2020-02-02 00:00:00.000000 databricks_labs_remorph-0.2.0/core/src/main/scala/com/databricks/labs/remorph/parsers/tsql/TSqlExpressionBuilder.scala
+-rw-r--r--   0        0        0     3753 2020-02-02 00:00:00.000000 databricks_labs_remorph-0.2.0/core/src/main/scala/com/databricks/labs/remorph/parsers/tsql/TSqlRelationBuilder.scala
+-rw-r--r--   0        0        0      159 2020-02-02 00:00:00.000000 databricks_labs_remorph-0.2.0/core/src/test/scala/com/databricks/labs/remorph/MainTest.scala
+-rw-r--r--   0        0        0     1318 2020-02-02 00:00:00.000000 databricks_labs_remorph-0.2.0/core/src/test/scala/com/databricks/labs/remorph/parsers/ErrorCollectorSpec.scala
+-rw-r--r--   0        0        0     1755 2020-02-02 00:00:00.000000 databricks_labs_remorph-0.2.0/core/src/test/scala/com/databricks/labs/remorph/parsers/ParserTestCommon.scala
+-rw-r--r--   0        0        0    12367 2020-02-02 00:00:00.000000 databricks_labs_remorph-0.2.0/core/src/test/scala/com/databricks/labs/remorph/parsers/common/FunctionBuilderSpec.scala
+-rw-r--r--   0        0        0     1466 2020-02-02 00:00:00.000000 databricks_labs_remorph-0.2.0/core/src/test/scala/com/databricks/labs/remorph/parsers/snowflake/DataTypeBuilderSpec.scala
+-rw-r--r--   0        0        0    15224 2020-02-02 00:00:00.000000 databricks_labs_remorph-0.2.0/core/src/test/scala/com/databricks/labs/remorph/parsers/snowflake/SnowflakeAstBuilderSpec.scala
+-rw-r--r--   0        0        0    16134 2020-02-02 00:00:00.000000 databricks_labs_remorph-0.2.0/core/src/test/scala/com/databricks/labs/remorph/parsers/snowflake/SnowflakeDDLBuilderSpec.scala
+-rw-r--r--   0        0        0     7289 2020-02-02 00:00:00.000000 databricks_labs_remorph-0.2.0/core/src/test/scala/com/databricks/labs/remorph/parsers/snowflake/SnowflakeExprSpec.scala
+-rw-r--r--   0        0        0    11148 2020-02-02 00:00:00.000000 databricks_labs_remorph-0.2.0/core/src/test/scala/com/databricks/labs/remorph/parsers/snowflake/SnowflakeExpressionBuilderSpec.scala
+-rw-r--r--   0        0        0      537 2020-02-02 00:00:00.000000 databricks_labs_remorph-0.2.0/core/src/test/scala/com/databricks/labs/remorph/parsers/snowflake/SnowflakeParserTestCommon.scala
+-rw-r--r--   0        0        0     8596 2020-02-02 00:00:00.000000 databricks_labs_remorph-0.2.0/core/src/test/scala/com/databricks/labs/remorph/parsers/snowflake/SnowflakeRelationBuilderSpec.scala
+-rw-r--r--   0        0        0    15627 2020-02-02 00:00:00.000000 databricks_labs_remorph-0.2.0/core/src/test/scala/com/databricks/labs/remorph/parsers/tsql/TSqlAstBuilderSpec.scala
+-rw-r--r--   0        0        0     6549 2020-02-02 00:00:00.000000 databricks_labs_remorph-0.2.0/core/src/test/scala/com/databricks/labs/remorph/parsers/tsql/TSqlErrorHandlerSpec.scala
+-rw-r--r--   0        0        0    19226 2020-02-02 00:00:00.000000 databricks_labs_remorph-0.2.0/core/src/test/scala/com/databricks/labs/remorph/parsers/tsql/TSqlExpressionBuilderSpec.scala
+-rw-r--r--   0        0        0     8352 2020-02-02 00:00:00.000000 databricks_labs_remorph-0.2.0/core/src/test/scala/com/databricks/labs/remorph/parsers/tsql/TSqlFunctionSpec.scala
+-rw-r--r--   0        0        0      689 2020-02-02 00:00:00.000000 databricks_labs_remorph-0.2.0/core/src/test/scala/com/databricks/labs/remorph/parsers/tsql/TSqlParserTestCommon.scala
+-rw-r--r--   0        0        0      261 2020-02-02 00:00:00.000000 databricks_labs_remorph-0.2.0/databricks/__init__.py
+-rw-r--r--   0        0        0      261 2020-02-02 00:00:00.000000 databricks_labs_remorph-0.2.0/databricks/labs/__init__.py
+-rw-r--r--   0        0        0       48 2020-02-02 00:00:00.000000 databricks_labs_remorph-0.2.0/databricks/labs/remorph/__about__.py
+-rw-r--r--   0        0        0       78 2020-02-02 00:00:00.000000 databricks_labs_remorph-0.2.0/databricks/labs/remorph/__init__.py
+-rw-r--r--   0        0        0     4934 2020-02-02 00:00:00.000000 databricks_labs_remorph-0.2.0/databricks/labs/remorph/cli.py
+-rw-r--r--   0        0        0     2669 2020-02-02 00:00:00.000000 databricks_labs_remorph-0.2.0/databricks/labs/remorph/config.py
+-rw-r--r--   0        0        0     8758 2020-02-02 00:00:00.000000 databricks_labs_remorph-0.2.0/databricks/labs/remorph/install.py
+-rw-r--r--   0        0        0     1701 2020-02-02 00:00:00.000000 databricks_labs_remorph-0.2.0/databricks/labs/remorph/lineage.py
+-rw-r--r--   0        0        0     1965 2020-02-02 00:00:00.000000 databricks_labs_remorph-0.2.0/databricks/labs/remorph/uninstall.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 databricks_labs_remorph-0.2.0/databricks/labs/remorph/coverage/__init__.py
+-rw-r--r--   0        0        0     5787 2020-02-02 00:00:00.000000 databricks_labs_remorph-0.2.0/databricks/labs/remorph/coverage/commons.py
+-rw-r--r--   0        0        0      992 2020-02-02 00:00:00.000000 databricks_labs_remorph-0.2.0/databricks/labs/remorph/coverage/remorph_snow_transpilation_coverage.py
+-rw-r--r--   0        0        0      844 2020-02-02 00:00:00.000000 databricks_labs_remorph-0.2.0/databricks/labs/remorph/coverage/sqlglot_snow_transpilation_coverage.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 databricks_labs_remorph-0.2.0/databricks/labs/remorph/helpers/__init__.py
+-rw-r--r--   0        0        0     1531 2020-02-02 00:00:00.000000 databricks_labs_remorph-0.2.0/databricks/labs/remorph/helpers/db_sql.py
+-rw-r--r--   0        0        0      533 2020-02-02 00:00:00.000000 databricks_labs_remorph-0.2.0/databricks/labs/remorph/helpers/execution_time.py
+-rw-r--r--   0        0        0     3977 2020-02-02 00:00:00.000000 databricks_labs_remorph-0.2.0/databricks/labs/remorph/helpers/file_utils.py
+-rw-r--r--   0        0        0      378 2020-02-02 00:00:00.000000 databricks_labs_remorph-0.2.0/databricks/labs/remorph/helpers/morph_status.py
+-rw-r--r--   0        0        0     7412 2020-02-02 00:00:00.000000 databricks_labs_remorph-0.2.0/databricks/labs/remorph/helpers/recon_config_utils.py
+-rw-r--r--   0        0        0     4280 2020-02-02 00:00:00.000000 databricks_labs_remorph-0.2.0/databricks/labs/remorph/helpers/validation.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 databricks_labs_remorph-0.2.0/databricks/labs/remorph/intermediate/__init__.py
+-rw-r--r--   0        0        0     3165 2020-02-02 00:00:00.000000 databricks_labs_remorph-0.2.0/databricks/labs/remorph/intermediate/dag.py
+-rw-r--r--   0        0        0      913 2020-02-02 00:00:00.000000 databricks_labs_remorph-0.2.0/databricks/labs/remorph/intermediate/engine_adapter.py
+-rw-r--r--   0        0        0     1380 2020-02-02 00:00:00.000000 databricks_labs_remorph-0.2.0/databricks/labs/remorph/intermediate/root_tables.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 databricks_labs_remorph-0.2.0/databricks/labs/remorph/reconcile/__init__.py
+-rw-r--r--   0        0        0     4971 2020-02-02 00:00:00.000000 databricks_labs_remorph-0.2.0/databricks/labs/remorph/reconcile/compare.py
+-rw-r--r--   0        0        0      536 2020-02-02 00:00:00.000000 databricks_labs_remorph-0.2.0/databricks/labs/remorph/reconcile/constants.py
+-rw-r--r--   0        0        0      487 2020-02-02 00:00:00.000000 databricks_labs_remorph-0.2.0/databricks/labs/remorph/reconcile/exception.py
+-rw-r--r--   0        0        0    15760 2020-02-02 00:00:00.000000 databricks_labs_remorph-0.2.0/databricks/labs/remorph/reconcile/execute.py
+-rw-r--r--   0        0        0    13124 2020-02-02 00:00:00.000000 databricks_labs_remorph-0.2.0/databricks/labs/remorph/reconcile/recon_capture.py
+-rw-r--r--   0        0        0     7739 2020-02-02 00:00:00.000000 databricks_labs_remorph-0.2.0/databricks/labs/remorph/reconcile/recon_config.py
+-rw-r--r--   0        0        0     5034 2020-02-02 00:00:00.000000 databricks_labs_remorph-0.2.0/databricks/labs/remorph/reconcile/schema_compare.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 databricks_labs_remorph-0.2.0/databricks/labs/remorph/reconcile/connectors/__init__.py
+-rw-r--r--   0        0        0     2389 2020-02-02 00:00:00.000000 databricks_labs_remorph-0.2.0/databricks/labs/remorph/reconcile/connectors/data_source.py
+-rw-r--r--   0        0        0     2733 2020-02-02 00:00:00.000000 databricks_labs_remorph-0.2.0/databricks/labs/remorph/reconcile/connectors/databricks.py
+-rw-r--r--   0        0        0      804 2020-02-02 00:00:00.000000 databricks_labs_remorph-0.2.0/databricks/labs/remorph/reconcile/connectors/jdbc_reader.py
+-rw-r--r--   0        0        0     4049 2020-02-02 00:00:00.000000 databricks_labs_remorph-0.2.0/databricks/labs/remorph/reconcile/connectors/oracle.py
+-rw-r--r--   0        0        0     1125 2020-02-02 00:00:00.000000 databricks_labs_remorph-0.2.0/databricks/labs/remorph/reconcile/connectors/secrets.py
+-rw-r--r--   0        0        0     3990 2020-02-02 00:00:00.000000 databricks_labs_remorph-0.2.0/databricks/labs/remorph/reconcile/connectors/snowflake.py
+-rw-r--r--   0        0        0     1124 2020-02-02 00:00:00.000000 databricks_labs_remorph-0.2.0/databricks/labs/remorph/reconcile/connectors/source_adapter.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 databricks_labs_remorph-0.2.0/databricks/labs/remorph/reconcile/query_builder/__init__.py
+-rw-r--r--   0        0        0     4590 2020-02-02 00:00:00.000000 databricks_labs_remorph-0.2.0/databricks/labs/remorph/reconcile/query_builder/base.py
+-rw-r--r--   0        0        0     9045 2020-02-02 00:00:00.000000 databricks_labs_remorph-0.2.0/databricks/labs/remorph/reconcile/query_builder/expression_generator.py
+-rw-r--r--   0        0        0     2716 2020-02-02 00:00:00.000000 databricks_labs_remorph-0.2.0/databricks/labs/remorph/reconcile/query_builder/hash_query.py
+-rw-r--r--   0        0        0     2762 2020-02-02 00:00:00.000000 databricks_labs_remorph-0.2.0/databricks/labs/remorph/reconcile/query_builder/sampling_query.py
+-rw-r--r--   0        0        0     9189 2020-02-02 00:00:00.000000 databricks_labs_remorph-0.2.0/databricks/labs/remorph/reconcile/query_builder/threshold_query.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 databricks_labs_remorph-0.2.0/databricks/labs/remorph/snow/__init__.py
+-rw-r--r--   0        0        0    26846 2020-02-02 00:00:00.000000 databricks_labs_remorph-0.2.0/databricks/labs/remorph/snow/databricks.py
+-rw-r--r--   0        0        0      646 2020-02-02 00:00:00.000000 databricks_labs_remorph-0.2.0/databricks/labs/remorph/snow/experimental.py
+-rw-r--r--   0        0        0     5014 2020-02-02 00:00:00.000000 databricks_labs_remorph-0.2.0/databricks/labs/remorph/snow/lca_utils.py
+-rw-r--r--   0        0        0     2983 2020-02-02 00:00:00.000000 databricks_labs_remorph-0.2.0/databricks/labs/remorph/snow/local_expression.py
+-rw-r--r--   0        0        0      711 2020-02-02 00:00:00.000000 databricks_labs_remorph-0.2.0/databricks/labs/remorph/snow/oracle.py
+-rw-r--r--   0        0        0    22129 2020-02-02 00:00:00.000000 databricks_labs_remorph-0.2.0/databricks/labs/remorph/snow/snowflake.py
+-rw-r--r--   0        0        0     2266 2020-02-02 00:00:00.000000 databricks_labs_remorph-0.2.0/databricks/labs/remorph/snow/sql_transpiler.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 databricks_labs_remorph-0.2.0/databricks/labs/remorph/transpiler/__init__.py
+-rw-r--r--   0        0        0     9936 2020-02-02 00:00:00.000000 databricks_labs_remorph-0.2.0/databricks/labs/remorph/transpiler/execute.py
+-rw-r--r--   0        0        0      134 2020-02-02 00:00:00.000000 databricks_labs_remorph-0.2.0/.gitignore
+-rw-r--r--   0        0        0     3862 2020-02-02 00:00:00.000000 databricks_labs_remorph-0.2.0/LICENSE
+-rw-r--r--   0        0        0     2238 2020-02-02 00:00:00.000000 databricks_labs_remorph-0.2.0/NOTICE
+-rw-r--r--   0        0        0     6443 2020-02-02 00:00:00.000000 databricks_labs_remorph-0.2.0/README.md
+-rw-r--r--   0        0        0    26930 2020-02-02 00:00:00.000000 databricks_labs_remorph-0.2.0/pyproject.toml
+-rw-r--r--   0        0        0     7367 2020-02-02 00:00:00.000000 databricks_labs_remorph-0.2.0/PKG-INFO
```

### Comparing `databricks_labs_remorph-0.1.7/core/src/main/antlr4/com/databricks/labs/remorph/parsers/snowflake/SnowflakeLexer.g4` & `databricks_labs_remorph-0.2.0/core/src/main/antlr4/com/databricks/labs/remorph/parsers/snowflake/SnowflakeLexer.g4`

 * *Files 0% similar despite different names*

```diff
@@ -970,14 +970,15 @@
 TIMEZONE                    : 'TIMEZONE';
 TIME_FORMAT                 : 'TIME_FORMAT';
 TIME_INPUT_FORMAT           : 'TIME_INPUT_FORMAT';
 TIME_OUTPUT_FORMAT          : 'TIME_OUTPUT_FORMAT';
 TO                          : 'TO';
 TO_BOOLEAN                  : 'TO_BOOLEAN';
 TO_DATE                     : 'TO_DATE';
+TO_TIME                     : 'TO_TIME';
 TO_TIMESTAMP                : 'TO_TIMESTAMP';
 TOP                         : 'TOP';
 // TRACKING:                                              'TRACKING';
 // TRACK_CAUSALITY:                                       'TRACK_CAUSALITY';
 // TRAN:                                                  'TRAN';
 TRANSACTION                         : 'TRANSACTION';
 TRANSACTIONS                        : 'TRANSACTIONS';
@@ -1183,16 +1184,16 @@
 PIPE_PIPE : '||';
 DOT       : '.';
 // UNDERLINE:           '_';
 AT   : '@';
 AT_Q : '\'@\'';
 //HASH:                '#';
 DOLLAR      : '$';
-LR_BRACKET  : '(';
-RR_BRACKET  : ')';
+L_PAREN     : '(';
+R_PAREN     : ')';
 LSB         : '[';
 RSB         : ']';
 LCB         : '{';
 RCB         : '}';
 COMMA       : ',';
 SEMI        : ';';
 COLON       : ':';
```

### Comparing `databricks_labs_remorph-0.1.7/core/src/main/antlr4/com/databricks/labs/remorph/parsers/snowflake/SnowflakeParser.g4` & `databricks_labs_remorph-0.2.0/core/src/main/antlr4/com/databricks/labs/remorph/parsers/snowflake/SnowflakeParser.g4`

 * *Files 11% similar despite different names*

```diff
@@ -72,19 +72,19 @@
 
 insert_multi_table_statement
     : INSERT OVERWRITE? ALL into_clause2
     | INSERT OVERWRITE? (FIRST | ALL) (WHEN predicate THEN into_clause2+)+ (ELSE into_clause2)? subquery
     ;
 
 into_clause2
-    : INTO object_name ('(' column_list ')')? values_list?
+    : INTO object_name (L_PAREN column_list R_PAREN)? values_list?
     ;
 
 values_list
-    : VALUES '(' value_item (COMMA value_item)* ')'
+    : VALUES L_PAREN value_item (COMMA value_item)* R_PAREN
     ;
 
 value_item
     : column_name
     | DEFAULT
     | NULL_
     ;
@@ -99,41 +99,41 @@
 
 merge_cond
     : (WHEN MATCHED (AND search_condition)? THEN merge_update_delete)+
     | WHEN NOT MATCHED (AND search_condition)? THEN merge_insert
     ;
 
 merge_update_delete
-    : UPDATE SET column_name EQ expr (',' column_name EQ expr)*
+    : UPDATE SET column_name EQ expr (COLON column_name EQ expr)*
     | DELETE
     ;
 
 merge_insert
-    : INSERT ('(' column_list ')')? VALUES '(' expr_list ')'
+    : INSERT (L_PAREN column_list R_PAREN)? VALUES L_PAREN expr_list R_PAREN
     ;
 
 update_statement
     : UPDATE object_name as_alias? SET column_name EQ expr (COMMA column_name EQ expr)* (
         FROM table_sources
     )? (WHERE search_condition)?
     ;
 
 table_or_query
     : object_name as_alias?
-    | '(' subquery ')' as_alias?
+    | L_PAREN subquery R_PAREN as_alias?
     ;
 
 delete_statement
     : DELETE FROM object_name as_alias? (USING table_or_query (COMMA table_or_query)?)? (
         WHERE search_condition
     )?
     ;
 
 values_builder
-    : VALUES '(' expr_list ')' (COMMA '(' expr_list ')')?
+    : VALUES L_PAREN expr_list R_PAREN (COMMA L_PAREN expr_list R_PAREN)?
     ;
 
 other_command
     : copy_into_table
     | copy_into_location
     | comment
     | commit
@@ -167,86 +167,86 @@
 
 copy_into_table
     : COPY INTO object_name FROM (table_stage | user_stage | named_stage | external_location) files? pattern? file_format? copy_options* (
         VALIDATION_MODE EQ (RETURN_N_ROWS | RETURN_ERRORS | RETURN_ALL_ERRORS)
     )?
     //
     /* Data load with transformation */
-    | COPY INTO object_name ('(' column_list ')')? FROM '(' SELECT select_list FROM (
+    | COPY INTO object_name (L_PAREN column_list R_PAREN)? FROM L_PAREN SELECT select_list FROM (
         table_stage
         | user_stage
         | named_stage
-    ) ')' files? pattern? file_format? copy_options*
+    ) R_PAREN files? pattern? file_format? copy_options*
     ;
 
 external_location
     //(for Amazon S3)
     : S3_PATH //'s3://<bucket>[/<path>]'
     //        ( ( STORAGE_INTEGRATION EQ id_ )?
-    //        | ( CREDENTIALS EQ '(' ( AWS_KEY_ID EQ string AWS_SECRET_KEY EQ string ( AWS_TOKEN EQ string )? ) ')' )?
+    //        | ( CREDENTIALS EQ L_PAREN ( AWS_KEY_ID EQ string AWS_SECRET_KEY EQ string ( AWS_TOKEN EQ string )? ) R_PAREN )?
     //        )?
     //        [ ENCRYPTION = ( [ TYPE = 'AWS_CSE' ] [ MASTER_KEY = '<string>' ] |
     //                   [ TYPE = 'AWS_SSE_S3' ] |
     //                   [ TYPE = 'AWS_SSE_KMS' [ KMS_KEY_ID = '<string>' ] ] |
     //                   [ TYPE = 'NONE' ] ) ]
     // (for Google Cloud Storage)
     | GCS_PATH //'gcs://<bucket>[/<path>]'
     //        ( STORAGE_INTEGRATION EQ id_ )?
     //[ ENCRYPTION = ( [ TYPE = 'GCS_SSE_KMS' ] [ KMS_KEY_ID = '<string>' ] | [ TYPE = 'NONE' ] ) ]
     // (for Microsoft Azure)
     | AZURE_PATH //'azure://<account>.blob.core.windows.net/<container>[/<path>]'
     //        (   ( STORAGE_INTEGRATION EQ id_ )?
-    //            | ( CREDENTIALS EQ '(' ( AZURE_SAS_TOKEN EQ string ) ')' )
+    //            | ( CREDENTIALS EQ L_PAREN ( AZURE_SAS_TOKEN EQ string ) R_PAREN )
     //        )?
     //[ ENCRYPTION = ( [ TYPE = { 'AZURE_CSE' | 'NONE' } ] [ MASTER_KEY = '<string>' ] ) ]
     ;
 
 files
-    : FILES EQ '(' string (COMMA string)* ')'
+    : FILES EQ L_PAREN string (COMMA string)* R_PAREN
     ;
 
 file_format
-    : FILE_FORMAT EQ '(' (format_name | format_type) ')'
+    : FILE_FORMAT EQ L_PAREN (format_name | format_type) R_PAREN
     ;
 
 format_name
     : FORMAT_NAME EQ string
     ;
 
 format_type
     : TYPE EQ type_fileformat format_type_options*
     ;
 
 stage_file_format
-    : STAGE_FILE_FORMAT EQ LR_BRACKET FORMAT_NAME EQ string
-    | TYPE EQ type_fileformat format_type_options+ RR_BRACKET
+    : STAGE_FILE_FORMAT EQ L_PAREN FORMAT_NAME EQ string
+    | TYPE EQ type_fileformat format_type_options+ R_PAREN
     ;
 
 copy_into_location
     : COPY INTO (table_stage | user_stage | named_stage | external_location) FROM (
         object_name
-        | '(' query_statement ')'
+        | L_PAREN query_statement R_PAREN
     ) partition_by? file_format? copy_options? (VALIDATION_MODE EQ RETURN_ROWS)? HEADER?
     ;
 
 comment
     : COMMENT if_exists? ON object_type_name object_name function_signature? IS string
     | COMMENT if_exists? ON COLUMN full_column_name IS string
     ;
 
 function_signature
-    : '(' data_type_list? ')'
+    : L_PAREN data_type_list? R_PAREN
     ;
 
 commit
     : COMMIT WORK?
     ;
 
 execute_immediate
-    : EXECUTE IMMEDIATE (string | id_ | ID2) (USING '(' id_ (COMMA id_)* ')')?
+    : EXECUTE IMMEDIATE (string | id_ | ID2) (USING L_PAREN id_ (COMMA id_)* R_PAREN)?
     | EXECUTE IMMEDIATE DBL_DOLLAR
     ;
 
 execute_task
     : EXECUTE TASK object_name
     ;
 
@@ -432,15 +432,15 @@
 //  @~[/<path>]
 user_stage
     : AT TILDA stage_path?
     ;
 
 //  @[<namespace>.]%<table_name>[/<path>]
 table_stage
-    : AT schema_name? '%' id_ stage_path?
+    : AT schema_name? MODULE id_ stage_path?
     ;
 
 //  @[<namespace>.]<ext_stage_name>[/<path>]
 named_stage
     : AT object_name stage_path?
     ;
 
@@ -509,28 +509,28 @@
 
 rollback
     : ROLLBACK WORK?
     ;
 
 set
     : SET id_ EQ expr
-    | SET LR_BRACKET id_ (COMMA id_)* RR_BRACKET EQ LR_BRACKET expr (COMMA expr)* RR_BRACKET
+    | SET L_PAREN id_ (COMMA id_)* R_PAREN EQ L_PAREN expr (COMMA expr)* R_PAREN
     ;
 
 truncate_materialized_view
     : TRUNCATE MATERIALIZED VIEW object_name
     ;
 
 truncate_table
     : TRUNCATE TABLE? if_exists? object_name
     ;
 
 unset
     : UNSET id_
-    | UNSET '(' id_ (COMMA id_)* ')'
+    | UNSET L_PAREN id_ (COMMA id_)* R_PAREN
     ;
 
 // alter commands
 alter_command
     : alter_account
     | alter_alert
     | alter_api_integration
@@ -617,15 +617,15 @@
     | MUST_CHANGE_PASSWORD EQ true_false
     | DISABLED EQ true_false
     | DAYS_TO_EXPIRY EQ num
     | MINS_TO_UNLOCK EQ num
     | DEFAULT_WAREHOUSE EQ string
     | DEFAULT_NAMESPACE EQ string
     | DEFAULT_ROLE EQ string
-    //| DEFAULT_SECONDARY_ROLES EQ '(' 'ALL' ')'
+    //| DEFAULT_SECONDARY_ROLES EQ L_PAREN 'ALL' R_PAREN
     | MINS_TO_BYPASS_MFA EQ num
     | RSA_PUBLIC_KEY EQ string
     | RSA_PUBLIC_KEY_2 EQ string
     | comment_clause
     ;
 
 session_params
@@ -671,15 +671,15 @@
     ;
 
 alter_alert
     : ALTER ALERT if_exists? id_ (
         resume_suspend
         | SET alert_set_clause+
         | UNSET alert_unset_clause+
-        | MODIFY CONDITION EXISTS '(' alert_condition ')'
+        | MODIFY CONDITION EXISTS L_PAREN alert_condition R_PAREN
         | MODIFY ACTION alert_action
     )
     ;
 
 resume_suspend
     : RESUME
     | SUSPEND
@@ -696,16 +696,16 @@
     | SCHEDULE
     | COMMENT
     ;
 
 alter_api_integration
     : ALTER API? INTEGRATION if_exists? id_ SET (API_AWS_ROLE_ARN EQ string)? (
         AZURE_AD_APPLICATION_ID EQ string
-    )? (API_KEY EQ string)? enabled_true_false? (API_ALLOWED_PREFIXES EQ '(' string ')')? (
-        API_BLOCKED_PREFIXES EQ '(' string ')'
+    )? (API_KEY EQ string)? enabled_true_false? (API_ALLOWED_PREFIXES EQ L_PAREN string R_PAREN)? (
+        API_BLOCKED_PREFIXES EQ L_PAREN string R_PAREN
     )? comment_clause?
     | ALTER API? INTEGRATION id_ set_tags
     | ALTER API? INTEGRATION id_ unset_tags
     | ALTER API? INTEGRATION if_exists? id_ UNSET api_integration_property (
         COMMA api_integration_property
     )*
     ;
@@ -752,22 +752,22 @@
 
 alter_dynamic_table
     : ALTER DYNAMIC TABLE id_ (resume_suspend | REFRESH | SET WAREHOUSE EQ id_)
     ;
 
 alter_external_table
     : ALTER EXTERNAL TABLE if_exists? object_name REFRESH string?
-    | ALTER EXTERNAL TABLE if_exists? object_name ADD FILES '(' string_list ')'
-    | ALTER EXTERNAL TABLE if_exists? object_name REMOVE FILES '(' string_list ')'
+    | ALTER EXTERNAL TABLE if_exists? object_name ADD FILES L_PAREN string_list R_PAREN
+    | ALTER EXTERNAL TABLE if_exists? object_name REMOVE FILES L_PAREN string_list R_PAREN
     | ALTER EXTERNAL TABLE if_exists? object_name SET (AUTO_REFRESH EQ true_false)? tag_decl_list?
     | ALTER EXTERNAL TABLE if_exists? object_name unset_tags
     //Partitions added and removed manually
-    | ALTER EXTERNAL TABLE object_name if_exists? ADD PARTITION '(' column_name EQ string (
+    | ALTER EXTERNAL TABLE object_name if_exists? ADD PARTITION L_PAREN column_name EQ string (
         COMMA column_name EQ string
-    )* ')' LOCATION string
+    )* R_PAREN LOCATION string
     | ALTER EXTERNAL TABLE object_name if_exists? DROP PARTITION LOCATION string
     ;
 
 ignore_edition_check
     : IGNORE EDITION CHECK
     ;
 
@@ -814,16 +814,16 @@
 alter_function
     : alter_function_signature RENAME TO id_
     | alter_function_signature SET comment_clause
     | alter_function_signature SET SECURE
     | alter_function_signature UNSET (SECURE | COMMENT)
     // External Functions
     | alter_function_signature SET API_INTEGRATION EQ id_
-    | alter_function_signature SET HEADERS EQ '(' header_decl* ')'
-    | alter_function_signature SET CONTEXT_HEADERS EQ '(' id_* ')'
+    | alter_function_signature SET HEADERS EQ L_PAREN header_decl* R_PAREN
+    | alter_function_signature SET CONTEXT_HEADERS EQ L_PAREN id_* R_PAREN
     | alter_function_signature SET MAX_BATCH_ROWS EQ num
     | alter_function_signature SET COMPRESSION EQ compression_type
     | alter_function_signature SET (REQUEST_TRANSLATOR | RESPONSE_TRANSLATOR) EQ id_
     | alter_function_signature UNSET (
         COMMENT
         | HEADERS
         | CONTEXT_HEADERS
@@ -832,15 +832,15 @@
         | SECURE
         | REQUEST_TRANSLATOR
         | RESPONSE_TRANSLATOR
     )
     ;
 
 alter_function_signature
-    : ALTER FUNCTION if_exists? id_ '(' data_type_list? ')'
+    : ALTER FUNCTION if_exists? id_ L_PAREN data_type_list? R_PAREN
     ;
 
 data_type_list
     : data_type (COMMA data_type)*
     ;
 
 alter_masking_policy
@@ -848,15 +848,15 @@
     | ALTER MASKING POLICY if_exists? id_ RENAME TO id_
     | ALTER MASKING POLICY if_exists? id_ SET comment_clause
     ;
 
 alter_materialized_view
     : ALTER MATERIALIZED VIEW id_ (
         RENAME TO id_
-        | CLUSTER BY '(' expr_list ')'
+        | CLUSTER BY L_PAREN expr_list R_PAREN
         | DROP CLUSTERING KEY
         | resume_suspend RECLUSTER?
         | SET ( SECURE? comment_clause?)
         | UNSET ( SECURE | COMMENT)
     )
     ;
 
@@ -879,18 +879,18 @@
     | ALTER PIPE id_ unset_tags
     | ALTER PIPE if_exists? id_ UNSET PIPE_EXECUTION_PAUSED EQ true_false
     | ALTER PIPE if_exists? id_ UNSET COMMENT
     | ALTER PIPE if_exists? id_ REFRESH (PREFIX EQ string)? (MODIFIED_AFTER EQ string)?
     ;
 
 alter_procedure
-    : ALTER PROCEDURE if_exists? id_ '(' data_type_list? ')' RENAME TO id_
-    | ALTER PROCEDURE if_exists? id_ '(' data_type_list? ')' SET comment_clause
-    | ALTER PROCEDURE if_exists? id_ '(' data_type_list? ')' UNSET COMMENT
-    | ALTER PROCEDURE if_exists? id_ '(' data_type_list? ')' EXECUTE AS caller_owner
+    : ALTER PROCEDURE if_exists? id_ L_PAREN data_type_list? R_PAREN RENAME TO id_
+    | ALTER PROCEDURE if_exists? id_ L_PAREN data_type_list? R_PAREN SET comment_clause
+    | ALTER PROCEDURE if_exists? id_ L_PAREN data_type_list? R_PAREN UNSET COMMENT
+    | ALTER PROCEDURE if_exists? id_ L_PAREN data_type_list? R_PAREN EXECUTE AS caller_owner
     ;
 
 alter_replication_group
     //Source Account
     : ALTER REPLICATION GROUP if_exists? id_ RENAME TO id_
     | ALTER REPLICATION GROUP if_exists? id_ SET (OBJECT_TYPES EQ object_type_list)? (
         REPLICATION_SCHEDULE EQ string
@@ -917,26 +917,26 @@
     ;
 
 frequency
     : FREQUENCY EQ (MONTHLY | DAILY | WEEKLY | YEARLY | NEVER)
     ;
 
 notify_users
-    : NOTIFY_USERS EQ LR_BRACKET id_ (COMMA id_)* RR_BRACKET
+    : NOTIFY_USERS EQ L_PAREN id_ (COMMA id_)* R_PAREN
     ;
 
 triggerDefinition
     : ON num PERCENT DO (SUSPEND | SUSPEND_IMMEDIATE | NOTIFY)
     ;
 
 alter_resource_monitor
     : ALTER RESOURCE MONITOR if_exists? id_ (
         SET credit_quota? frequency? (
-            START_TIMESTAMP EQ LR_BRACKET string
-            | IMMEDIATELY RR_BRACKET
+            START_TIMESTAMP EQ L_PAREN string
+            | IMMEDIATELY R_PAREN
         )? (END_TIMESTAMP EQ string)?
     )? (notify_users ( TRIGGERS triggerDefinition (COMMA triggerDefinition)*)?)?
     ;
 
 alter_role
     : ALTER ROLE if_exists? id_ RENAME TO id_
     | ALTER ROLE if_exists? id_ SET comment_clause
@@ -978,22 +978,22 @@
     ;
 
 alter_security_integration_external_oauth
     : ALTER SECURITY? INTEGRATION if_exists id_ SET (TYPE EQ EXTERNAL_OAUTH)? (
         ENABLED EQ true_false
     )? (EXTERNAL_OAUTH_TYPE EQ ( OKTA | AZURE | PING_FEDERATE | CUSTOM))? (
         EXTERNAL_OAUTH_ISSUER EQ string
-    )? (EXTERNAL_OAUTH_TOKEN_USER_MAPPING_CLAIM EQ (string | '(' string_list ')'))? (
+    )? (EXTERNAL_OAUTH_TOKEN_USER_MAPPING_CLAIM EQ (string | L_PAREN string_list R_PAREN))? (
         EXTERNAL_OAUTH_SNOWFLAKE_USER_MAPPING_ATTRIBUTE EQ string
     )? (EXTERNAL_OAUTH_JWS_KEYS_URL EQ string)?                      // For OKTA | PING_FEDERATE | CUSTOM
-    (EXTERNAL_OAUTH_JWS_KEYS_URL EQ (string | '(' string_list ')'))? // For Azure
+    (EXTERNAL_OAUTH_JWS_KEYS_URL EQ (string | L_PAREN string_list R_PAREN))? // For Azure
     (EXTERNAL_OAUTH_RSA_PUBLIC_KEY EQ string)? (EXTERNAL_OAUTH_RSA_PUBLIC_KEY_2 EQ string)? (
-        EXTERNAL_OAUTH_BLOCKED_ROLES_LIST EQ '(' string_list ')'
-    )? (EXTERNAL_OAUTH_ALLOWED_ROLES_LIST EQ '(' string_list ')')? (
-        EXTERNAL_OAUTH_AUDIENCE_LIST EQ '(' string ')'
+        EXTERNAL_OAUTH_BLOCKED_ROLES_LIST EQ L_PAREN string_list R_PAREN
+    )? (EXTERNAL_OAUTH_ALLOWED_ROLES_LIST EQ L_PAREN string_list R_PAREN)? (
+        EXTERNAL_OAUTH_AUDIENCE_LIST EQ L_PAREN string R_PAREN
     )? (EXTERNAL_OAUTH_ANY_ROLE_MODE EQ (DISABLE | ENABLE | ENABLE_FOR_PRIVILEGE))? (
         EXTERNAL_OAUTH_ANY_ROLE_MODE EQ string
     )? // Only for EXTERNAL_OAUTH_TYPE EQ CUSTOM
     | ALTER SECURITY? INTEGRATION if_exists? id_ UNSET security_integration_external_oauth_property (
         COMMA security_integration_external_oauth_property
     )*
     | ALTER SECURITY? INTEGRATION id_ set_tags
@@ -1009,23 +1009,23 @@
     | COMMENT
     ;
 
 alter_security_integration_snowflake_oauth
     : ALTER SECURITY? INTEGRATION if_exists? id_ SET (TYPE EQ EXTERNAL_OAUTH)? enabled_true_false? (
         EXTERNAL_OAUTH_TYPE EQ ( OKTA | AZURE | PING_FEDERATE | CUSTOM)
     )? (EXTERNAL_OAUTH_ISSUER EQ string)? (
-        EXTERNAL_OAUTH_TOKEN_USER_MAPPING_CLAIM EQ (string | '(' string_list ')')
+        EXTERNAL_OAUTH_TOKEN_USER_MAPPING_CLAIM EQ (string | L_PAREN string_list R_PAREN)
     )? (EXTERNAL_OAUTH_SNOWFLAKE_USER_MAPPING_ATTRIBUTE EQ string)? (
         EXTERNAL_OAUTH_JWS_KEYS_URL EQ string
     )?                                                                // For OKTA | PING_FEDERATE | CUSTOM
-    (EXTERNAL_OAUTH_JWS_KEYS_URL EQ ( string | '(' string_list ')'))? // For Azure
+    (EXTERNAL_OAUTH_JWS_KEYS_URL EQ ( string | L_PAREN string_list R_PAREN))? // For Azure
     (EXTERNAL_OAUTH_RSA_PUBLIC_KEY EQ string)? (EXTERNAL_OAUTH_RSA_PUBLIC_KEY_2 EQ string)? (
-        EXTERNAL_OAUTH_BLOCKED_ROLES_LIST EQ '(' string_list ')'
-    )? (EXTERNAL_OAUTH_ALLOWED_ROLES_LIST EQ '(' string_list ')')? (
-        EXTERNAL_OAUTH_AUDIENCE_LIST EQ '(' string ')'
+        EXTERNAL_OAUTH_BLOCKED_ROLES_LIST EQ L_PAREN string_list R_PAREN
+    )? (EXTERNAL_OAUTH_ALLOWED_ROLES_LIST EQ L_PAREN string_list R_PAREN)? (
+        EXTERNAL_OAUTH_AUDIENCE_LIST EQ L_PAREN string R_PAREN
     )? (EXTERNAL_OAUTH_ANY_ROLE_MODE EQ DISABLE | ENABLE | ENABLE_FOR_PRIVILEGE)? (
         EXTERNAL_OAUTH_SCOPE_DELIMITER EQ string
     ) // Only for EXTERNAL_OAUTH_TYPE EQ CUSTOM
     | ALTER SECURITY? INTEGRATION if_exists? id_ UNSET security_integration_snowflake_oauth_property (
         COMMA security_integration_snowflake_oauth_property
     )*
     | ALTER SECURITY? INTEGRATION id_ set_tags
@@ -1092,16 +1092,16 @@
     | ALTER SHARE if_exists? id_ set_tags
     | ALTER SHARE id_ unset_tags
     | ALTER SHARE if_exists? id_ UNSET COMMENT
     ;
 
 alter_storage_integration
     : ALTER STORAGE? INTEGRATION if_exists? id_ SET cloud_provider_params2? enabled_true_false? (
-        STORAGE_ALLOWED_LOCATIONS EQ '(' string_list ')'
-    )? (STORAGE_BLOCKED_LOCATIONS EQ '(' string_list ')')? comment_clause?
+        STORAGE_ALLOWED_LOCATIONS EQ L_PAREN string_list R_PAREN
+    )? (STORAGE_BLOCKED_LOCATIONS EQ L_PAREN string_list R_PAREN)? comment_clause?
     | ALTER STORAGE? INTEGRATION if_exists? id_ set_tags
     | ALTER STORAGE? INTEGRATION id_ unset_tags
     | ALTER STORAGE? INTEGRATION if_exists? id_ UNSET (
         ENABLED
         | STORAGE_BLOCKED_LOCATIONS
         | COMMENT
     )
@@ -1122,15 +1122,15 @@
         clustering_action
         | table_column_action
         | constraint_action
     )
     | ALTER TABLE if_exists? object_name ext_table_column_action
     | ALTER TABLE if_exists? object_name search_optimization_action
     | ALTER TABLE if_exists? object_name SET stage_file_format? (
-        STAGE_COPY_OPTIONS EQ '(' copy_options ')'
+        STAGE_COPY_OPTIONS EQ L_PAREN copy_options R_PAREN
     )? (DATA_RETENTION_TIME_IN_DAYS EQ num)? (MAX_DATA_EXTENSION_TIME_IN_DAYS EQ num)? (
         CHANGE_TRACKING EQ true_false
     )? default_ddl_collation? comment_clause?
     | ALTER TABLE if_exists? object_name set_tags
     | ALTER TABLE if_exists? object_name unset_tags
     | ALTER TABLE if_exists? object_name UNSET (
         DATA_RETENTION_TIME_IN_DAYS
@@ -1144,29 +1144,29 @@
     | ALTER TABLE if_exists? object_name ADD ROW ACCESS POLICY id_ ON column_list_in_parentheses
     | ALTER TABLE if_exists? object_name DROP ROW ACCESS POLICY id_
     | ALTER TABLE if_exists? object_name DROP ROW ACCESS POLICY id_ COMMA ADD ROW ACCESS POLICY id_ ON column_list_in_parentheses
     | ALTER TABLE if_exists? object_name DROP ALL ROW ACCESS POLICIES
     ;
 
 clustering_action
-    : CLUSTER BY '(' expr_list ')'
+    : CLUSTER BY L_PAREN expr_list R_PAREN
     | RECLUSTER ( MAX_SIZE EQ num)? ( WHERE expr)?
     | resume_suspend RECLUSTER
     | DROP CLUSTERING KEY
     ;
 
 table_column_action
     : ADD COLUMN? if_not_exists? full_col_decl (COMMA full_col_decl)*
     | RENAME COLUMN column_name TO column_name
     | alter_modify (
-        '(' alter_column_clause (',' alter_column_clause)* ')'
-        | alter_column_clause (',' alter_column_clause)*
+        L_PAREN alter_column_clause (COLON alter_column_clause)* R_PAREN
+        | alter_column_clause (COLON alter_column_clause)*
     )
     | alter_modify COLUMN column_name SET MASKING POLICY id_ (
-        USING '(' column_name COMMA column_list ')'
+        USING L_PAREN column_name COMMA column_list R_PAREN
     )? FORCE?
     | alter_modify COLUMN column_name UNSET MASKING POLICY
     | alter_modify column_set_tags (COMMA column_set_tags)*
     | alter_modify column_unset_tags (COMMA column_unset_tags)*
     | DROP COLUMN? if_exists? column_list
     //| DROP DEFAULT
     ;
@@ -1181,15 +1181,15 @@
         | UNSET COMMENT
     )
     ;
 
 inline_constraint
     : (CONSTRAINT id_)? (
         (UNIQUE | primary_key) common_constraint_properties*
-        | foreign_key REFERENCES object_name (LR_BRACKET column_name RR_BRACKET)? constraint_properties
+        | foreign_key REFERENCES object_name (L_PAREN column_name R_PAREN)? constraint_properties
     )
     ;
 
 enforced_not_enforced
     : NOT? ENFORCED
     ;
 
@@ -1234,15 +1234,15 @@
 constraint_properties
     : common_constraint_properties*
     | foreign_key_match
     | foreign_key_match? ( on_update on_delete? | on_delete on_update?)
     ;
 
 ext_table_column_action
-    : ADD COLUMN? column_name data_type AS '(' expr ')'
+    : ADD COLUMN? column_name data_type AS L_PAREN expr R_PAREN
     | RENAME COLUMN column_name TO column_name
     | DROP COLUMN? column_list
     ;
 
 constraint_action
     : ADD out_of_line_constraint
     | RENAME CONSTRAINT id_ TO id_
@@ -1256,24 +1256,24 @@
 
 search_optimization_action
     : ADD SEARCH OPTIMIZATION (ON search_method_with_target (COMMA search_method_with_target)*)?
     | DROP SEARCH OPTIMIZATION (ON search_method_with_target (COMMA search_method_with_target)*)?
     ;
 
 search_method_with_target
-    : (EQUALITY | SUBSTRING | GEO) '(' (STAR | expr) ')'
+    : (EQUALITY | SUBSTRING | GEO) L_PAREN (STAR | expr) R_PAREN
     ;
 
 alter_table_alter_column
     : ALTER TABLE object_name alter_modify (
-        '(' alter_column_decl_list ')'
+        L_PAREN alter_column_decl_list R_PAREN
         | alter_column_decl_list
     )
     | ALTER TABLE object_name alter_modify COLUMN column_name SET MASKING POLICY id_ (
-        USING '(' column_name COMMA column_list ')'
+        USING L_PAREN column_name COMMA column_list R_PAREN
     )? FORCE?
     | ALTER TABLE object_name alter_modify COLUMN column_name UNSET MASKING POLICY
     | ALTER TABLE object_name alter_modify column_set_tags (COMMA column_set_tags)*
     | ALTER TABLE object_name alter_modify column_unset_tags (COMMA column_unset_tags)*
     ;
 
 alter_column_decl_list
@@ -1334,15 +1334,15 @@
     | ALTER VIEW if_exists? object_name set_tags
     | ALTER VIEW if_exists? object_name unset_tags
     | ALTER VIEW if_exists? object_name ADD ROW ACCESS POLICY id_ ON column_list_in_parentheses
     | ALTER VIEW if_exists? object_name DROP ROW ACCESS POLICY id_
     | ALTER VIEW if_exists? object_name ADD ROW ACCESS POLICY id_ ON column_list_in_parentheses COMMA DROP ROW ACCESS POLICY id_
     | ALTER VIEW if_exists? object_name DROP ALL ROW ACCESS POLICIES
     | ALTER VIEW object_name alter_modify COLUMN? id_ SET MASKING POLICY id_ (
-        USING '(' column_name COMMA column_list ')'
+        USING L_PAREN column_name COMMA column_list R_PAREN
     )? FORCE?
     | ALTER VIEW object_name alter_modify COLUMN? id_ UNSET MASKING POLICY
     | ALTER VIEW object_name alter_modify COLUMN? id_ set_tags
     | ALTER VIEW object_name alter_modify COLUMN id_ unset_tags
     ;
 
 alter_modify
@@ -1381,30 +1381,30 @@
     | SET MASKING POLICY id_ (COMMA MASKING POLICY id_)*
     | UNSET MASKING POLICY id_ (COMMA MASKING POLICY id_)*
     | SET comment_clause
     | UNSET COMMENT
     ;
 
 alter_network_policy_opts
-    : if_exists? id_ SET (ALLOWED_IP_LIST EQ '(' string_list ')')? (
-        BLOCKED_IP_LIST EQ '(' string_list ')'
+    : if_exists? id_ SET (ALLOWED_IP_LIST EQ L_PAREN string_list R_PAREN)? (
+        BLOCKED_IP_LIST EQ L_PAREN string_list R_PAREN
     )? comment_clause?
     | if_exists? id_ UNSET COMMENT
     | id_ RENAME TO id_
     ;
 
 alter_warehouse_opts
     : id_fn? (SUSPEND | RESUME if_suspended?)
     | id_fn? ABORT ALL QUERIES
     | id_fn RENAME TO id_
     //    | id_ SET [ objectProperties ]
     | id_fn set_tags
     | id_fn unset_tags
     | id_fn UNSET id_ (COMMA id_)*
-    | id_ SET wh_properties (',' wh_properties)*
+    | id_ SET wh_properties (COLON wh_properties)*
     ;
 
 alter_account_opts
     : SET account_params? object_params? session_params?
     | UNSET param_name (COMMA param_name)?
     | SET RESOURCE_MONITOR EQ id_
     | set_tags
@@ -1481,15 +1481,15 @@
         STANDARD
         | ENTERPRISE
         | BUSINESS_CRITICAL
     ) (REGION_GROUP EQ region_group_id)? (REGION EQ snowflake_region_id)? comment_clause?
     ;
 
 create_alert
-    : CREATE or_replace? ALERT if_not_exists? id_ WAREHOUSE EQ id_ SCHEDULE EQ string IF '(' EXISTS '(' alert_condition ')' ')' THEN alert_action
+    : CREATE or_replace? ALERT if_not_exists? id_ WAREHOUSE EQ id_ SCHEDULE EQ string IF L_PAREN EXISTS L_PAREN alert_condition R_PAREN R_PAREN THEN alert_action
     ;
 
 alert_condition
     : select_statement
     | show_command
     | call
     ;
@@ -1497,28 +1497,28 @@
 alert_action
     : sql_command
     ;
 
 create_api_integration
     : CREATE or_replace? API INTEGRATION if_not_exists? id_ API_PROVIDER EQ (id_) API_AWS_ROLE_ARN EQ string (
         API_KEY EQ string
-    )? API_ALLOWED_PREFIXES EQ LR_BRACKET string RR_BRACKET (
-        API_BLOCKED_PREFIXES EQ LR_BRACKET string RR_BRACKET
+    )? API_ALLOWED_PREFIXES EQ L_PAREN string R_PAREN (
+        API_BLOCKED_PREFIXES EQ L_PAREN string R_PAREN
     )? ENABLED EQ true_false comment_clause?
     | CREATE or_replace? API INTEGRATION if_not_exists? id_ API_PROVIDER EQ id_ AZURE_TENANT_ID EQ string AZURE_AD_APPLICATION_ID EQ string (
         API_KEY EQ string
-    )? API_ALLOWED_PREFIXES EQ '(' string ')' (API_BLOCKED_PREFIXES EQ '(' string ')')? ENABLED EQ true_false comment_clause?
-    | CREATE or_replace API INTEGRATION if_not_exists id_ API_PROVIDER EQ id_ GOOGLE_AUDIENCE EQ string API_ALLOWED_PREFIXES EQ '(' string ')' (
-        API_BLOCKED_PREFIXES EQ '(' string ')'
+    )? API_ALLOWED_PREFIXES EQ L_PAREN string R_PAREN (API_BLOCKED_PREFIXES EQ L_PAREN string R_PAREN)? ENABLED EQ true_false comment_clause?
+    | CREATE or_replace API INTEGRATION if_not_exists id_ API_PROVIDER EQ id_ GOOGLE_AUDIENCE EQ string API_ALLOWED_PREFIXES EQ L_PAREN string R_PAREN (
+        API_BLOCKED_PREFIXES EQ L_PAREN string R_PAREN
     )? ENABLED EQ true_false comment_clause?
     ;
 
 create_object_clone
     : CREATE or_replace? (DATABASE | SCHEMA | TABLE) if_not_exists? id_ CLONE object_name (
-        at_before1 LR_BRACKET (TIMESTAMP ASSOC string | OFFSET ASSOC string | STATEMENT ASSOC id_) RR_BRACKET
+        at_before1 L_PAREN (TIMESTAMP ASSOC string | OFFSET ASSOC string | STATEMENT ASSOC id_) R_PAREN
     )?
     | CREATE or_replace? (STAGE | FILE FORMAT | SEQUENCE | STREAM | TASK) if_not_exists? object_name CLONE object_name
     ;
 
 create_connection
     : CREATE CONNECTION if_not_exists? id_ (
         comment_clause?
@@ -1530,15 +1530,15 @@
     : CREATE or_replace? TRANSIENT? DATABASE if_not_exists? id_ clone_at_before? (
         DATA_RETENTION_TIME_IN_DAYS EQ num
     )? (MAX_DATA_EXTENSION_TIME_IN_DAYS EQ num)? default_ddl_collation? with_tags? comment_clause?
     ;
 
 clone_at_before
     : CLONE id_ (
-        at_before1 LR_BRACKET (TIMESTAMP ASSOC string | OFFSET ASSOC string | STATEMENT ASSOC id_) RR_BRACKET
+        at_before1 L_PAREN (TIMESTAMP ASSOC string | OFFSET ASSOC string | STATEMENT ASSOC id_) R_PAREN
     )?
     ;
 
 at_before1
     : AT_KEYWORD
     | BEFORE
     ;
@@ -1567,37 +1567,37 @@
         DATA_RETENTION_TIME_IN_DAYS EQ num
     )? (MAX_DATA_EXTENSION_TIME_IN_DAYS EQ num)? change_tracking? (
         DEFAULT_DDL_COLLATION_ EQ string
     )? copy_grants? with_row_access_policy? with_tags? (WITH? comment_clause)?
     ;
 
 create_external_function
-    : CREATE or_replace? SECURE? EXTERNAL FUNCTION object_name LR_BRACKET (
+    : CREATE or_replace? SECURE? EXTERNAL FUNCTION object_name L_PAREN (
         arg_name arg_data_type (COMMA arg_name arg_data_type)*
-    )? RR_BRACKET RETURNS data_type null_not_null? (
+    )? R_PAREN RETURNS data_type null_not_null? (
         ( CALLED ON NULL_ INPUT)
         | ((RETURNS NULL_ ON NULL_ INPUT) | STRICT)
     )? (VOLATILE | IMMUTABLE)? comment_clause? API_INTEGRATION EQ id_ (
-        HEADERS EQ LR_BRACKET header_decl (COMMA header_decl)* RR_BRACKET
-    )? (CONTEXT_HEADERS EQ LR_BRACKET id_ (COMMA id_)* RR_BRACKET)? (MAX_BATCH_ROWS EQ num)? compression? (
+        HEADERS EQ L_PAREN header_decl (COMMA header_decl)* R_PAREN
+    )? (CONTEXT_HEADERS EQ L_PAREN id_ (COMMA id_)* R_PAREN)? (MAX_BATCH_ROWS EQ num)? compression? (
         REQUEST_TRANSLATOR EQ id_
     )? (RESPONSE_TRANSLATOR EQ id_)? AS string
     ;
 
 create_external_table
     // Partitions computed from expressions
-    : CREATE or_replace? EXTERNAL TABLE if_not_exists? object_name '(' external_table_column_decl_list ')' cloud_provider_params3? partition_by? WITH?
+    : CREATE or_replace? EXTERNAL TABLE if_not_exists? object_name L_PAREN external_table_column_decl_list R_PAREN cloud_provider_params3? partition_by? WITH?
         LOCATION EQ named_stage (REFRESH_ON_CREATE EQ true_false)? (AUTO_REFRESH EQ true_false)? pattern? file_format (
         AWS_SNS_TOPIC EQ string
     )? copy_grants? with_row_access_policy? with_tags? comment_clause?
     // Partitions added and removed manually
-    | CREATE or_replace? EXTERNAL TABLE if_not_exists? object_name '(' external_table_column_decl_list ')' cloud_provider_params3? partition_by? WITH?
+    | CREATE or_replace? EXTERNAL TABLE if_not_exists? object_name L_PAREN external_table_column_decl_list R_PAREN cloud_provider_params3? partition_by? WITH?
         LOCATION EQ named_stage PARTITION_TYPE EQ USER_SPECIFIED file_format copy_grants? with_row_access_policy? with_tags? comment_clause?
     // Delta Lake
-    | CREATE or_replace? EXTERNAL TABLE if_not_exists? object_name '(' external_table_column_decl_list ')' cloud_provider_params3? partition_by? WITH?
+    | CREATE or_replace? EXTERNAL TABLE if_not_exists? object_name L_PAREN external_table_column_decl_list R_PAREN cloud_provider_params3? partition_by? WITH?
         LOCATION EQ named_stage PARTITION_TYPE EQ USER_SPECIFIED file_format (
         TABLE_FORMAT EQ DELTA
     )? copy_grants? with_row_access_policy? with_tags? comment_clause?
     ;
 
 external_table_column_decl
     : column_name data_type AS (expr | id_) inline_constraint?
@@ -1656,71 +1656,71 @@
     ;
 
 col_decl
     : column_name data_type virtual_column_decl?
     ;
 
 virtual_column_decl
-    : AS '(' function_call ')'
+    : AS L_PAREN function_call R_PAREN
     ;
 
 function_definition
     : string
     | DBL_DOLLAR
     ;
 
 create_function
-    : CREATE or_replace? SECURE? FUNCTION if_not_exists? object_name LR_BRACKET (
+    : CREATE or_replace? SECURE? FUNCTION if_not_exists? object_name L_PAREN (
         arg_decl (COMMA arg_decl)*
-    )? RR_BRACKET RETURNS (data_type | TABLE LR_BRACKET (col_decl (COMMA col_decl)*)? RR_BRACKET) (
+    )? R_PAREN RETURNS (data_type | TABLE L_PAREN (col_decl (COMMA col_decl)*)? R_PAREN) (
         LANGUAGE (JAVA | PYTHON | JAVASCRIPT | SCALA | SQL)
     )? (CALLED ON NULL_ INPUT | RETURNS NULL_ ON NULL_ INPUT | STRICT)? (VOLATILE | IMMUTABLE)? (
-        PACKAGES EQ '(' string_list ')'
-    )? (RUNTIME_VERSION EQ (string | FLOAT))? (IMPORTS EQ '(' string_list ')')? (
-        PACKAGES EQ '(' string_list ')'
+        PACKAGES EQ L_PAREN string_list R_PAREN
+    )? (RUNTIME_VERSION EQ (string | FLOAT))? (IMPORTS EQ L_PAREN string_list R_PAREN)? (
+        PACKAGES EQ L_PAREN string_list R_PAREN
     )? (HANDLER EQ string)? null_not_null? comment_clause? AS function_definition
-    | CREATE or_replace? SECURE? FUNCTION object_name LR_BRACKET (arg_decl (COMMA arg_decl)*)? RR_BRACKET RETURNS (
+    | CREATE or_replace? SECURE? FUNCTION object_name L_PAREN (arg_decl (COMMA arg_decl)*)? R_PAREN RETURNS (
         data_type
-        | TABLE LR_BRACKET (col_decl (COMMA col_decl)*)? RR_BRACKET
+        | TABLE L_PAREN (col_decl (COMMA col_decl)*)? R_PAREN
     ) null_not_null? (CALLED ON NULL_ INPUT | RETURNS NULL_ ON NULL_ INPUT | STRICT)? (
         VOLATILE
         | IMMUTABLE
     )? MEMOIZABLE? comment_clause? AS function_definition
     ;
 
 create_managed_account
     : CREATE MANAGED ACCOUNT id_ ADMIN_NAME EQ id_ COMMA ADMIN_PASSWORD EQ string COMMA TYPE EQ READER (
         COMMA comment_clause
     )?
     ;
 
 create_masking_policy
-    : CREATE or_replace? MASKING POLICY if_not_exists? object_name AS '(' arg_name arg_data_type (
+    : CREATE or_replace? MASKING POLICY if_not_exists? object_name AS L_PAREN arg_name arg_data_type (
         COMMA arg_name arg_data_type
-    )? ')' RETURNS arg_data_type ARROW expr comment_clause?
+    )? R_PAREN RETURNS arg_data_type ARROW expr comment_clause?
     ;
 
 tag_decl
     : object_name EQ string
     ;
 
 column_list_in_parentheses
-    : LR_BRACKET column_list RR_BRACKET
+    : L_PAREN column_list R_PAREN
     ;
 
 create_materialized_view
     : CREATE or_replace? SECURE? MATERIALIZED VIEW if_not_exists? object_name (
-        LR_BRACKET column_list_with_comment RR_BRACKET
+        L_PAREN column_list_with_comment R_PAREN
     )? view_col* with_row_access_policy? with_tags? copy_grants? comment_clause? cluster_by? AS select_statement
     //NOTA MATERIALIZED VIEW accept only simple select statement at this time
     ;
 
 create_network_policy
-    : CREATE or_replace? NETWORK POLICY id_ ALLOWED_IP_LIST EQ '(' string_list? ')' (
-        BLOCKED_IP_LIST EQ '(' string_list? ')'
+    : CREATE or_replace? NETWORK POLICY id_ ALLOWED_IP_LIST EQ L_PAREN string_list? R_PAREN (
+        BLOCKED_IP_LIST EQ L_PAREN string_list? R_PAREN
     )? comment_clause?
     ;
 
 cloud_provider_params_auto
     //(for Google Cloud Storage)
     : NOTIFICATION_PROVIDER EQ GCP_PUBSUB GCP_PUBSUB_SUBSCRIPTION_NAME EQ string
     //(for Microsoft Azure Storage)
@@ -1763,32 +1763,32 @@
     ;
 
 not_null
     : NOT NULL_
     ;
 
 create_procedure
-    : CREATE or_replace? PROCEDURE object_name LR_BRACKET (arg_decl (COMMA arg_decl)*)? RR_BRACKET RETURNS (
+    : CREATE or_replace? PROCEDURE object_name L_PAREN (arg_decl (COMMA arg_decl)*)? R_PAREN RETURNS (
         data_type
-        | TABLE LR_BRACKET (col_decl (COMMA col_decl)*)? RR_BRACKET
+        | TABLE L_PAREN (col_decl (COMMA col_decl)*)? R_PAREN
     ) not_null? LANGUAGE SQL (CALLED ON NULL_ INPUT | RETURNS NULL_ ON NULL_ INPUT | STRICT)? (
         VOLATILE
         | IMMUTABLE
     )? // Note: VOLATILE and IMMUTABLE are deprecated.
     comment_clause? executa_as? AS procedure_definition
-    | CREATE or_replace? SECURE? PROCEDURE object_name LR_BRACKET (arg_decl (COMMA arg_decl)*)? RR_BRACKET RETURNS data_type not_null? LANGUAGE
+    | CREATE or_replace? SECURE? PROCEDURE object_name L_PAREN (arg_decl (COMMA arg_decl)*)? R_PAREN RETURNS data_type not_null? LANGUAGE
         JAVASCRIPT (CALLED ON NULL_ INPUT | RETURNS NULL_ ON NULL_ INPUT | STRICT)? (
         VOLATILE
         | IMMUTABLE
     )? // Note: VOLATILE and IMMUTABLE are deprecated.
     comment_clause? executa_as? AS procedure_definition
-    | CREATE or_replace? SECURE? PROCEDURE object_name LR_BRACKET (arg_decl (COMMA arg_decl)*)? RR_BRACKET RETURNS (
+    | CREATE or_replace? SECURE? PROCEDURE object_name L_PAREN (arg_decl (COMMA arg_decl)*)? R_PAREN RETURNS (
         data_type not_null?
-        | TABLE LR_BRACKET (col_decl (COMMA col_decl)*)? RR_BRACKET
-    ) LANGUAGE PYTHON RUNTIME_VERSION EQ string (IMPORTS EQ '(' string_list ')')? PACKAGES EQ '(' string_list ')' HANDLER EQ string
+        | TABLE L_PAREN (col_decl (COMMA col_decl)*)? R_PAREN
+    ) LANGUAGE PYTHON RUNTIME_VERSION EQ string (IMPORTS EQ L_PAREN string_list R_PAREN)? PACKAGES EQ L_PAREN string_list R_PAREN HANDLER EQ string
     //            ( CALLED ON NULL_ INPUT | RETURNS NULL_ ON NULL_ INPUT | STRICT )?
     //            ( VOLATILE | IMMUTABLE )? // Note: VOLATILE and IMMUTABLE are deprecated.
     comment_clause? executa_as? AS procedure_definition
     ;
 
 create_replication_group
     : CREATE REPLICATION GROUP if_not_exists? id_ OBJECT_TYPES EQ object_type (COMMA object_type)* (
@@ -1809,17 +1809,17 @@
     ;
 
 create_role
     : CREATE or_replace? ROLE if_not_exists? id_ with_tags? comment_clause?
     ;
 
 create_row_access_policy
-    : CREATE or_replace? ROW ACCESS POLICY if_not_exists? id_ AS LR_BRACKET arg_decl (
+    : CREATE or_replace? ROW ACCESS POLICY if_not_exists? id_ AS L_PAREN arg_decl (
         COMMA arg_decl
-    )* RR_BRACKET RETURNS BOOLEAN ARROW expr comment_clause?
+    )* R_PAREN RETURNS BOOLEAN ARROW expr comment_clause?
     ;
 
 create_schema
     : CREATE or_replace? TRANSIENT? SCHEMA if_not_exists? schema_name clone_at_before? (
         WITH MANAGED ACCESS
     )? (DATA_RETENTION_TIME_IN_DAYS EQ num)? (MAX_DATA_EXTENSION_TIME_IN_DAYS EQ num)? default_ddl_collation? with_tags? comment_clause?
     ;
@@ -1828,23 +1828,23 @@
     : CREATE or_replace? SECURITY INTEGRATION if_not_exists? id_ TYPE EQ EXTERNAL_OAUTH ENABLED EQ true_false EXTERNAL_OAUTH_TYPE EQ (
         OKTA
         | AZURE
         | PING_FEDERATE
         | CUSTOM
     ) EXTERNAL_OAUTH_ISSUER EQ string EXTERNAL_OAUTH_TOKEN_USER_MAPPING_CLAIM EQ (
         string
-        | '(' string_list ')'
+        | L_PAREN string_list R_PAREN
     ) EXTERNAL_OAUTH_SNOWFLAKE_USER_MAPPING_ATTRIBUTE EQ string (
         EXTERNAL_OAUTH_JWS_KEYS_URL EQ string
     )?                                                               // For OKTA | PING_FEDERATE | CUSTOM
-    (EXTERNAL_OAUTH_JWS_KEYS_URL EQ (string | '(' string_list ')'))? // For Azure
-    (EXTERNAL_OAUTH_BLOCKED_ROLES_LIST EQ '(' string_list ')')? (
-        EXTERNAL_OAUTH_ALLOWED_ROLES_LIST EQ '(' string_list ')'
+    (EXTERNAL_OAUTH_JWS_KEYS_URL EQ (string | L_PAREN string_list R_PAREN))? // For Azure
+    (EXTERNAL_OAUTH_BLOCKED_ROLES_LIST EQ L_PAREN string_list R_PAREN)? (
+        EXTERNAL_OAUTH_ALLOWED_ROLES_LIST EQ L_PAREN string_list R_PAREN
     )? (EXTERNAL_OAUTH_RSA_PUBLIC_KEY EQ string)? (EXTERNAL_OAUTH_RSA_PUBLIC_KEY_2 EQ string)? (
-        EXTERNAL_OAUTH_AUDIENCE_LIST EQ '(' string ')'
+        EXTERNAL_OAUTH_AUDIENCE_LIST EQ L_PAREN string R_PAREN
     )? (EXTERNAL_OAUTH_ANY_ROLE_MODE EQ (DISABLE | ENABLE | ENABLE_FOR_PRIVILEGE))? (
         EXTERNAL_OAUTH_SCOPE_DELIMITER EQ string
     )? // Only for EXTERNAL_OAUTH_TYPE EQ CUSTOM
     ;
 
 implicit_none
     : IMPLICIT
@@ -1852,23 +1852,23 @@
     ;
 
 create_security_integration_snowflake_oauth
     : CREATE or_replace? SECURITY INTEGRATION if_not_exists? id_ TYPE EQ OAUTH OAUTH_CLIENT EQ partner_application OAUTH_REDIRECT_URI EQ string
     //Required when OAUTH_CLIENTEQLOOKER
     enabled_true_false? (OAUTH_ISSUE_REFRESH_TOKENS EQ true_false)? (
         OAUTH_REFRESH_TOKEN_VALIDITY EQ num
-    )? (OAUTH_USE_SECONDARY_ROLES EQ implicit_none)? (BLOCKED_ROLES_LIST EQ '(' string_list ')')? comment_clause?
+    )? (OAUTH_USE_SECONDARY_ROLES EQ implicit_none)? (BLOCKED_ROLES_LIST EQ L_PAREN string_list R_PAREN)? comment_clause?
     // Snowflake OAuth for custom clients
     | CREATE or_replace? SECURITY INTEGRATION if_not_exists? id_ TYPE EQ OAUTH OAUTH_CLIENT EQ CUSTOM
     //OAUTH_CLIENT_TYPE EQ 'CONFIDENTIAL' | 'PUBLIC'
     OAUTH_REDIRECT_URI EQ string enabled_true_false? (
         OAUTH_ALLOW_NON_TLS_REDIRECT_URI EQ true_false
     )? (OAUTH_ENFORCE_PKCE EQ true_false)? (OAUTH_USE_SECONDARY_ROLES EQ implicit_none)? (
-        PRE_AUTHORIZED_ROLES_LIST EQ '(' string_list ')'
-    )? (BLOCKED_ROLES_LIST EQ '(' string_list ')')? (OAUTH_ISSUE_REFRESH_TOKENS EQ true_false)? (
+        PRE_AUTHORIZED_ROLES_LIST EQ L_PAREN string_list R_PAREN
+    )? (BLOCKED_ROLES_LIST EQ L_PAREN string_list R_PAREN)? (OAUTH_ISSUE_REFRESH_TOKENS EQ true_false)? (
         OAUTH_REFRESH_TOKEN_VALIDITY EQ num
     )? network_policy? (OAUTH_CLIENT_RSA_PUBLIC_KEY EQ string)? (
         OAUTH_CLIENT_RSA_PUBLIC_KEY_2 EQ string
     )? comment_clause?
     ;
 
 create_security_integration_saml2
@@ -1961,15 +1961,15 @@
     | TIME_FORMAT EQ (string | AUTO)
     | TIMESTAMP_FORMAT EQ (string | AUTO)
     | BINARY_FORMAT EQ (HEX | BASE64 | UTF8)
     | ESCAPE EQ (character | NONE | NONE_Q)
     | ESCAPE_UNENCLOSED_FIELD EQ (string | NONE | NONE_Q)
     | TRIM_SPACE EQ true_false
     | FIELD_OPTIONALLY_ENCLOSED_BY EQ (string | NONE | NONE_Q | SINGLE_QUOTE)
-    | NULL_IF EQ LR_BRACKET string_list RR_BRACKET
+    | NULL_IF EQ L_PAREN string_list R_PAREN
     | ERROR_ON_COLUMN_COUNT_MISMATCH EQ true_false
     | REPLACE_INVALID_CHARACTERS EQ true_false
     | EMPTY_FIELD_AS_NULL EQ true_false
     | SKIP_BYTE_ORDER_MARK EQ true_false
     | ENCODING EQ (string | UTF8) //by the way other encoding keyword are valid ie WINDOWS1252
     //-- If TYPE EQ JSON
     //| COMPRESSION EQ (AUTO | GZIP | BZ2 | BROTLI | ZSTD | DEFLATE | RAW_DEFLATE | NONE)
@@ -2030,15 +2030,15 @@
     | NONE
     | ENFORCE_LENGTH EQ true_false
     | TRUNCATECOLUMNS EQ true_false
     | FORCE EQ true_false
     ;
 
 stage_encryption_opts_internal
-    : ENCRYPTION EQ LR_BRACKET TYPE EQ (SNOWFLAKE_FULL | SNOWFLAKE_SSE) RR_BRACKET
+    : ENCRYPTION EQ L_PAREN TYPE EQ (SNOWFLAKE_FULL | SNOWFLAKE_SSE) R_PAREN
     ;
 
 stage_type
     : TYPE EQ string
     ;
 
 stage_master_key
@@ -2046,15 +2046,15 @@
     ;
 
 stage_kms_key
     : KMS_KEY_ID EQ string
     ;
 
 stage_encryption_opts_aws
-    : ENCRYPTION EQ LR_BRACKET (stage_type? stage_master_key | stage_type stage_kms_key?) RR_BRACKET
+    : ENCRYPTION EQ L_PAREN (stage_type? stage_master_key | stage_type stage_kms_key?) R_PAREN
     ;
 
 aws_token
     : AWS_TOKEN EQ string
     ;
 
 aws_key_id
@@ -2072,39 +2072,39 @@
 azure_encryption_value
     : (TYPE EQ AZURE_CSE_Q)? MASTER_KEY EQ string
     | MASTER_KEY EQ string TYPE EQ AZURE_CSE_Q
     | TYPE EQ NONE_Q
     ;
 
 stage_encryption_opts_az
-    : ENCRYPTION EQ LR_BRACKET azure_encryption_value RR_BRACKET
+    : ENCRYPTION EQ L_PAREN azure_encryption_value R_PAREN
     ;
 
 storage_integration_eq_id
     : STORAGE_INTEGRATION EQ id_
     ;
 
 az_credential_or_storage_integration
     : storage_integration_eq_id
-    | CREDENTIALS EQ LR_BRACKET AZURE_SAS_TOKEN EQ string RR_BRACKET
+    | CREDENTIALS EQ L_PAREN AZURE_SAS_TOKEN EQ string R_PAREN
     ;
 
 gcp_encryption_value
     : (TYPE EQ GCS_SSE_KMS_Q)? KMS_KEY_ID EQ string
     | KMS_KEY_ID EQ string TYPE EQ GCS_SSE_KMS_Q
     | TYPE EQ NONE_Q
     ;
 
 stage_encryption_opts_gcp
-    : ENCRYPTION EQ LR_BRACKET gcp_encryption_value RR_BRACKET
+    : ENCRYPTION EQ L_PAREN gcp_encryption_value R_PAREN
     ;
 
 aws_credential_or_storage_integration
     : storage_integration_eq_id
-    | CREDENTIALS EQ LR_BRACKET (aws_key_id aws_secret_key aws_token? | aws_role) RR_BRACKET
+    | CREDENTIALS EQ L_PAREN (aws_key_id aws_secret_key aws_token? | aws_role) R_PAREN
     ;
 
 external_stage_params
     //(for Amazon S3)
     : URL EQ s3_url = (S3_PATH | S3GOV_PATH) (
         aws_credential_or_storage_integration? stage_encryption_opts_aws
         | stage_encryption_opts_aws? aws_credential_or_storage_integration
@@ -2139,52 +2139,52 @@
     ;
 
 notification_integration
     : NOTIFICATION_INTEGRATION EQ string
     ;
 
 directory_table_internal_params
-    : DIRECTORY EQ LR_BRACKET (
+    : DIRECTORY EQ L_PAREN (
         enable refresh_on_create?
         | REFRESH_ON_CREATE EQ FALSE
         | refresh_on_create enable
-    ) RR_BRACKET
+    ) R_PAREN
     ;
 
 directory_table_external_params
     // (for Amazon S3)
-    : DIRECTORY EQ LR_BRACKET enable refresh_on_create? auto_refresh? RR_BRACKET
+    : DIRECTORY EQ L_PAREN enable refresh_on_create? auto_refresh? R_PAREN
     // (for Google Cloud Storage)
-    | DIRECTORY EQ LR_BRACKET enable auto_refresh? refresh_on_create? notification_integration? RR_BRACKET
+    | DIRECTORY EQ L_PAREN enable auto_refresh? refresh_on_create? notification_integration? R_PAREN
     // (for Microsoft Azure)
-    | DIRECTORY EQ LR_BRACKET enable refresh_on_create? auto_refresh? notification_integration? RR_BRACKET
+    | DIRECTORY EQ L_PAREN enable refresh_on_create? auto_refresh? notification_integration? R_PAREN
     ;
 
 /* ===========  Stage DDL section =========== */
 create_stage
     : CREATE or_replace? temporary? STAGE if_not_exists? object_name_or_identifier stage_encryption_opts_internal? directory_table_internal_params? (
-        FILE_FORMAT EQ LR_BRACKET (
+        FILE_FORMAT EQ L_PAREN (
             FORMAT_NAME EQ string
             | TYPE EQ type_fileformat format_type_options*
-        ) RR_BRACKET
-    )? (COPY_OPTIONS_ EQ LR_BRACKET copy_options RR_BRACKET)? with_tags? comment_clause?
+        ) R_PAREN
+    )? (COPY_OPTIONS_ EQ L_PAREN copy_options R_PAREN)? with_tags? comment_clause?
     | CREATE or_replace? temporary? STAGE if_not_exists? object_name_or_identifier external_stage_params directory_table_external_params? (
-        FILE_FORMAT EQ LR_BRACKET (
+        FILE_FORMAT EQ L_PAREN (
             FORMAT_NAME EQ string
             | TYPE EQ type_fileformat format_type_options*
-        ) RR_BRACKET
-    )? (COPY_OPTIONS_ EQ LR_BRACKET copy_options RR_BRACKET)? with_tags? comment_clause?
+        ) R_PAREN
+    )? (COPY_OPTIONS_ EQ L_PAREN copy_options R_PAREN)? with_tags? comment_clause?
     ;
 
 alter_stage
     : ALTER STAGE if_exists? object_name_or_identifier RENAME TO object_name_or_identifier
     | ALTER STAGE if_exists? object_name_or_identifier set_tags
     | ALTER STAGE if_exists? object_name_or_identifier unset_tags
     | ALTER STAGE if_exists? object_name_or_identifier SET external_stage_params? file_format? (
-        COPY_OPTIONS_ EQ LR_BRACKET copy_options RR_BRACKET
+        COPY_OPTIONS_ EQ L_PAREN copy_options R_PAREN
     )? comment_clause?
     ;
 
 drop_stage
     : DROP STAGE if_exists? object_name_or_identifier
     ;
 
@@ -2216,16 +2216,16 @@
 
 cloud_provider_params3
     : INTEGRATION EQ string
     ;
 
 create_storage_integration
     : CREATE or_replace? STORAGE INTEGRATION if_not_exists? id_ TYPE EQ EXTERNAL_STAGE cloud_provider_params ENABLED EQ true_false
-        STORAGE_ALLOWED_LOCATIONS EQ LR_BRACKET string_list RR_BRACKET (
-        STORAGE_BLOCKED_LOCATIONS EQ LR_BRACKET string_list RR_BRACKET
+        STORAGE_ALLOWED_LOCATIONS EQ L_PAREN string_list R_PAREN (
+        STORAGE_BLOCKED_LOCATIONS EQ L_PAREN string_list R_PAREN
     )? comment_clause?
     ;
 
 copy_grants
     : COPY GRANTS
     ;
 
@@ -2238,20 +2238,20 @@
     ;
 
 show_initial_rows
     : SHOW_INITIAL_ROWS EQ true_false
     ;
 
 stream_time
-    : at_before1 LR_BRACKET (
+    : at_before1 L_PAREN (
         TIMESTAMP ASSOC string
         | OFFSET ASSOC string
         | STATEMENT ASSOC id_
         | STREAM ASSOC string
-    ) RR_BRACKET
+    ) R_PAREN
     ;
 
 create_stream
     //-- table
     : CREATE or_replace? STREAM if_not_exists? object_name copy_grants? ON TABLE object_name stream_time? append_only? show_initial_rows?
         comment_clause?
     //-- External table
@@ -2270,19 +2270,19 @@
 
 table_type
     : (( LOCAL | GLOBAL)? temporary | VOLATILE)
     | TRANSIENT
     ;
 
 with_tags
-    : WITH? TAG LR_BRACKET tag_decl (COMMA tag_decl)* RR_BRACKET
+    : WITH? TAG L_PAREN tag_decl (COMMA tag_decl)* R_PAREN
     ;
 
 with_row_access_policy
-    : WITH? ROW ACCESS POLICY id_ ON LR_BRACKET column_name (COMMA column_name)* RR_BRACKET
+    : WITH? ROW ACCESS POLICY id_ ON L_PAREN column_name (COMMA column_name)* R_PAREN
     ;
 
 cluster_by
     : CLUSTER BY LINEAR? expr_list_in_parentheses
     ;
 
 change_tracking
@@ -2301,15 +2301,15 @@
     : ORDER
     | NOORDER
     ;
 
 default_value
     : DEFAULT expr
     | (AUTOINCREMENT | IDENTITY) (
-        LR_BRACKET num COMMA num RR_BRACKET
+        L_PAREN num COMMA num R_PAREN
         | start_with
         | increment_by
         | start_with increment_by
     )? order_noorder?
     ;
 
 foreign_key
@@ -2346,32 +2346,32 @@
     : CREATE or_replace? table_type? TABLE (
         if_not_exists? object_name
         | object_name if_not_exists?
     ) ((comment_clause? create_table_clause) | (create_table_clause comment_clause?))
     ;
 
 column_decl_item_list_paren
-    : '(' column_decl_item_list ')'
+    : L_PAREN column_decl_item_list R_PAREN
     ;
 
 create_table_clause
     : (
         column_decl_item_list_paren cluster_by?
         | cluster_by? comment_clause? column_decl_item_list_paren
-    ) stage_file_format? (STAGE_COPY_OPTIONS EQ LR_BRACKET copy_options RR_BRACKET)? (
+    ) stage_file_format? (STAGE_COPY_OPTIONS EQ L_PAREN copy_options R_PAREN)? (
         DATA_RETENTION_TIME_IN_DAYS EQ num
     )? (MAX_DATA_EXTENSION_TIME_IN_DAYS EQ num)? change_tracking? default_ddl_collation? copy_grants? comment_clause? with_row_access_policy?
         with_tags?
     ;
 
 create_table_as_select
     : CREATE or_replace? table_type? TABLE (
         if_not_exists? object_name
         | object_name if_not_exists?
-    ) ('(' column_decl_item_list ')')? cluster_by? copy_grants? with_row_access_policy? with_tags? comment_clause? AS query_statement
+    ) (L_PAREN column_decl_item_list R_PAREN)? cluster_by? copy_grants? with_row_access_policy? with_tags? comment_clause? AS query_statement
     ;
 
 create_table_like
     : CREATE or_replace? TRANSIENT? TABLE if_not_exists? object_name LIKE object_name cluster_by? copy_grants?
     ;
 
 create_tag
@@ -2518,28 +2518,28 @@
 sql
     : EXECUTE IMMEDIATE DBL_DOLLAR
     | sql_command
     | call
     ;
 
 call
-    : CALL object_name '(' expr_list? ')'
+    : CALL object_name L_PAREN expr_list? R_PAREN
     ;
 
 create_user
     : CREATE or_replace? USER if_not_exists? id_ object_properties? object_params? session_params?
     ;
 
 view_col
     : column_name with_masking_policy with_tags
     ;
 
 create_view
     : CREATE or_replace? SECURE? RECURSIVE? VIEW if_not_exists? object_name (
-        LR_BRACKET column_list_with_comment RR_BRACKET
+        L_PAREN column_list_with_comment R_PAREN
     )? view_col* with_row_access_policy? with_tags? copy_grants? comment_clause? AS query_statement
     ;
 
 create_warehouse
     : CREATE or_replace? WAREHOUSE if_not_exists? id_fn (WITH? wh_properties+)? wh_params*
     ;
 
@@ -2787,15 +2787,15 @@
 
 cascade_restrict
     : CASCADE
     | RESTRICT
     ;
 
 arg_types
-    : LR_BRACKET data_type_list? RR_BRACKET
+    : L_PAREN data_type_list? R_PAREN
     ;
 
 // undrop commands
 undrop_command
     //: undrop_object
     : undrop_database
     | undrop_schema
@@ -2955,15 +2955,15 @@
     ;
 
 describe_procedure
     : describe PROCEDURE object_name arg_types
     ;
 
 describe_result
-    : describe RESULT (STRING | LAST_QUERY_ID LR_BRACKET RR_BRACKET)
+    : describe RESULT (STRING | LAST_QUERY_ID L_PAREN R_PAREN)
     ;
 
 describe_row_access_policy
     : describe ROW ACCESS POLICY id_
     ;
 
 describe_schema
@@ -3405,15 +3405,15 @@
 
 string_list
     : string (COMMA string)*
     ;
 
 id_fn
     : id_
-    | IDENTIFIER '(' id_ ')'
+    | IDENTIFIER L_PAREN id_ R_PAREN
     ;
 
 id_
     //id_ is used for object name. Snowflake is very permissive
     //so we could use nearly all keyword as object name (table, column etc..)
     : ID
     | ID2
@@ -3639,15 +3639,15 @@
     ;
 
 //pattern_assoc
 //    : PATTERN ASSOC string
 //    ;
 
 column_name
-    : (id_ '.')? id_
+    : (id_ DOT)? id_
     ;
 
 column_list
     : column_name (COMMA column_name)*
     ;
 
 column_list_with_comment
@@ -3658,15 +3658,15 @@
     : d = id_ DOT s = id_ DOT o = id_
     | s = id_ DOT o = id_
     | o = id_
     ;
 
 object_name_or_identifier
     : object_name
-    | IDENTIFIER LR_BRACKET string RR_BRACKET
+    | IDENTIFIER L_PAREN string R_PAREN
     ;
 
 num
     : DECIMAL
     ;
 
 /*** expressions ***/
@@ -3675,62 +3675,73 @@
     ;
 
 expr_list_sorted
     : expr asc_desc? (COMMA expr asc_desc?)*
     ;
 
 expr
-    : object_name DOT NEXTVAL
-    | expr LSB expr RSB //array access
-    | expr COLON expr   //json access
-    | expr DOT (VALUE | expr)
-    | expr COLLATE string
-    | case_expression
-    | iff_expr
-    | bracket_expression
-    | op = ( PLUS | MINUS) expr
-    | expr op = (STAR | DIVIDE | MODULE) expr
-    | expr op = (PLUS | MINUS | PIPE_PIPE) expr
-    | expr comparison_operator expr
-    | op = NOT+ expr
-    | expr AND expr //bool operation
-    | expr OR expr  //bool operation
-    | arr_literal
+    : object_name DOT NEXTVAL                       #exprNextval
+    | expr LSB expr RSB                             #exprArrayAccess
+    | expr COLON json_path                          #exprJsonAccess
+    | expr DOT (VALUE | expr)                       #exprDot
+    | expr COLLATE string                           #exprCollate
+    | case_expression                               #exprCase
+    | iff_expr                                      #exprIff
+    | bracket_expression                            #exprBracket
+    | sign expr                                     #exprSign
+    | expr op = (STAR | DIVIDE | MODULE) expr       #exprPrecedence0
+    | expr op = (PLUS | MINUS | PIPE_PIPE) expr     #exprPrecedence1
+    | expr comparison_operator expr                 #exprComparison
+    | op = NOT+ expr                                #exprNot
+    | expr AND expr                                 #exprAnd
+    | expr OR expr                                  #exprOr
+    | arr_literal                                   #exprArrayLit
     //    | expr time_zone
-    | expr over_clause
-    | cast_expr
-    | expr COLON_COLON data_type // Cast also
-    | try_cast_expr
-    | json_literal
-    | trim_expression
-    | function_call
-    | subquery
-    | expr IS null_not_null
-    | expr NOT? IN LR_BRACKET (subquery | expr_list) RR_BRACKET
-    | expr NOT? ( LIKE | ILIKE) expr (ESCAPE expr)?
-    | expr NOT? RLIKE expr
-    | expr NOT? (LIKE | ILIKE) ANY LR_BRACKET expr (COMMA expr)* RR_BRACKET (ESCAPE expr)?
-    | primitive_expression //Should be latest rule as it's nearly a catch all
+    | expr over_clause                              #exprOver
+    | cast_expr                                     #exprCast
+    | expr COLON_COLON data_type                    #exprAscribe
+    | json_literal                                  #exprJsonLit
+    | trim_expression                               #exprTrim
+    | function_call                                 #exprFuncCall
+    // Probably wrong
+    | subquery                                      #exprSubquery
+    | expr predicate_partial                        #exprPredicate
+    //Should be latest rule as it's nearly a catch all
+    | primitive_expression                          #exprPrimitive
+    ;
+
+predicate_partial
+    : IS null_not_null
+    | NOT? IN L_PAREN (subquery | expr_list) R_PAREN
+    | NOT? ( LIKE | ILIKE) expr (ESCAPE expr)?
+    | NOT? RLIKE expr
+    | NOT? (LIKE | ILIKE) ANY L_PAREN expr (COMMA expr)* R_PAREN (ESCAPE expr)?
+    | NOT? BETWEEN expr AND expr
     ;
 
-iff_expr
-    : IFF '(' search_condition ',' expr ',' expr ')'
+json_path
+    : json_path_elem (DOT json_path_elem)*
     ;
 
-trim_expression
-    : (TRIM | LTRIM | RTRIM) LR_BRACKET expr (COMMA string)* RR_BRACKET
+json_path_elem
+    : ID | DOUBLE_QUOTE_ID
+    ;
+
+iff_expr
+    : IFF L_PAREN search_condition COMMA expr COMMA expr R_PAREN
     ;
 
-try_cast_expr
-    : TRY_CAST LR_BRACKET expr AS data_type RR_BRACKET
+trim_expression
+    : (TRIM | LTRIM | RTRIM) L_PAREN expr (COMMA string)* R_PAREN
     ;
 
 cast_expr
-    : CAST LR_BRACKET expr AS data_type RR_BRACKET
-    | (TIMESTAMP | DATE | TIME | INTERVAL) expr
+    : cast_op = (TRY_CAST | CAST) L_PAREN expr AS data_type R_PAREN
+    | conversion = (TO_TIMESTAMP | TO_DATE | DATE | TO_TIME | TIME ) L_PAREN expr R_PAREN
+    | INTERVAL expr
     ;
 
 json_literal
     : LCB kv_pair (COMMA kv_pair)* RCB
     | LCB RCB
     ;
 
@@ -3739,25 +3750,25 @@
     ;
 
 value
     : expr
     ;
 
 arr_literal
-    : LSB value (',' value)* RSB
+    : LSB value (COMMA value)* RSB
     | LSB RSB
     ;
 
 data_type_size
-    : LR_BRACKET num RR_BRACKET
+    : L_PAREN num R_PAREN
     ;
 
 data_type
     : int_alias = (INT | INTEGER | SMALLINT | TINYINT | BYTEINT | BIGINT)
-    | number_alias = (NUMBER | NUMERIC | DECIMAL_) (LR_BRACKET num (COMMA num)? RR_BRACKET)?
+    | number_alias = (NUMBER | NUMERIC | DECIMAL_) (L_PAREN num (COMMA num)? R_PAREN)?
     | float_alias = (FLOAT_ | FLOAT4 | FLOAT8 | DOUBLE | DOUBLE_PRECISION | REAL_)
     | BOOLEAN
     | DATE
     | DATETIME data_type_size?
     | TIME data_type_size?
     | TIMESTAMP data_type_size?
     | TIMESTAMP_LTZ data_type_size?
@@ -3780,15 +3791,15 @@
     | GEOGRAPHY
     | GEOMETRY
     ;
 
 primitive_expression
     : DEFAULT //?
     | NULL_
-    | id_ ('.' id_)* // json field access
+    | id_ (DOT id_)* // json field access
     | full_column_name
     | literal
     | BOTH_Q
     | ARRAY_Q
     | OBJECT_Q
     //| json_literal
     //| arr_literal
@@ -3799,67 +3810,67 @@
     ;
 
 //order_by_expr_list
 //    : ORDER BY expr_list
 //    ;
 
 //over_clause_window
-//    : OVER '(' partition_by? order_by_expr (cumulative_frame | sliding_frame)? ')'
+//    : OVER L_PAREN partition_by? order_by_expr (cumulative_frame | sliding_frame)? R_PAREN
 //    ;
 
 asc_desc
     : ASC
     | DESC
     ;
 
 over_clause
-    : OVER '(' partition_by order_by_expr? ')'
-    | OVER '(' order_by_expr ')'
+    : OVER L_PAREN partition_by order_by_expr? R_PAREN
+    | OVER L_PAREN order_by_expr R_PAREN
     ;
 
 function_call
-    : unary_or_binary_builtin_function LR_BRACKET expr (COMMA expr)* RR_BRACKET
-    | binary_builtin_function LR_BRACKET expr COMMA expr RR_BRACKET
-    | binary_or_ternary_builtin_function LR_BRACKET expr COMMA expr (COMMA expr)* RR_BRACKET
-    | ternary_builtin_function LR_BRACKET expr COMMA expr COMMA expr RR_BRACKET
+    : unary_or_binary_builtin_function L_PAREN expr (COMMA expr)* R_PAREN
+    | binary_builtin_function L_PAREN expr COMMA expr R_PAREN
+    | binary_or_ternary_builtin_function L_PAREN expr COMMA expr (COMMA expr)* R_PAREN
+    | ternary_builtin_function L_PAREN expr COMMA expr COMMA expr R_PAREN
     | ranking_windowed_function
     | aggregate_function
     //    | aggregate_windowed_function
-    | object_name '(' expr_list? ')'
-    | object_name '(' param_assoc_list ')'
-    | list_function LR_BRACKET expr_list RR_BRACKET
-    | to_date = ( TO_DATE | DATE) LR_BRACKET expr RR_BRACKET
-    | length = ( LENGTH | LEN) LR_BRACKET expr RR_BRACKET
-    | TO_BOOLEAN LR_BRACKET expr RR_BRACKET
+    | object_name L_PAREN expr_list? R_PAREN
+    | object_name L_PAREN param_assoc_list R_PAREN
+    | list_function L_PAREN expr_list R_PAREN
+    | to_date = ( TO_DATE | DATE) L_PAREN expr R_PAREN
+    | length = ( LENGTH | LEN) L_PAREN expr R_PAREN
+    | TO_BOOLEAN L_PAREN expr R_PAREN
     ;
 
 param_assoc_list
-    : param_assoc (',' param_assoc)*
+    : param_assoc (COLON param_assoc)*
     ;
 
 param_assoc
     : id_ ASSOC expr
     ;
 
 ignore_or_repect_nulls
     : (IGNORE | RESPECT) NULLS
     ;
 
 ranking_windowed_function
-    : (RANK | DENSE_RANK | ROW_NUMBER) '(' ')' over_clause
-    | NTILE '(' expr ')' over_clause
-    | (LEAD | LAG) LR_BRACKET expr (COMMA expr COMMA expr)? RR_BRACKET ignore_or_repect_nulls? over_clause
-    | (FIRST_VALUE | LAST_VALUE) LR_BRACKET expr RR_BRACKET ignore_or_repect_nulls? over_clause
+    : (RANK | DENSE_RANK | ROW_NUMBER) L_PAREN R_PAREN over_clause
+    | NTILE L_PAREN expr R_PAREN over_clause
+    | (LEAD | LAG) L_PAREN expr (COMMA expr COMMA expr)? R_PAREN ignore_or_repect_nulls? over_clause
+    | (FIRST_VALUE | LAST_VALUE) L_PAREN expr R_PAREN ignore_or_repect_nulls? over_clause
     ;
 
 aggregate_function
-    : id_ '(' DISTINCT? expr_list ')'
-    | id_ '(' STAR ')'
-    | (LISTAGG | ARRAY_AGG) '(' DISTINCT? expr (COMMA string)? ')' (
-        WITHIN GROUP '(' order_by_clause ')'
+    : id_ L_PAREN DISTINCT? expr_list R_PAREN
+    | id_ L_PAREN STAR R_PAREN
+    | (LISTAGG | ARRAY_AGG) L_PAREN DISTINCT? expr (COMMA string)? R_PAREN (
+        WITHIN GROUP L_PAREN order_by_clause R_PAREN
     )?
     ;
 
 //rows_range
 //    : ROWS | RANGE
 //    ;
 
@@ -3896,16 +3907,16 @@
     : db_name = id_? DOT schema = id_? DOT tab_name = id_? DOT col_name = id_
     | schema = id_? DOT tab_name = id_? DOT col_name = id_
     | tab_name = id_? DOT col_name = id_
     | col_name = id_
     ;
 
 bracket_expression
-    : LR_BRACKET expr_list RR_BRACKET
-    | LR_BRACKET subquery RR_BRACKET
+    : L_PAREN expr_list R_PAREN
+    | L_PAREN subquery R_PAREN
     ;
 
 case_expression
     : CASE expr switch_section+ (ELSE expr)? END
     | CASE switch_search_condition_section+ (ELSE expr)? END
     ;
 
@@ -3923,25 +3934,25 @@
     ;
 
 with_expression
     : WITH common_table_expression (COMMA common_table_expression)*
     ;
 
 common_table_expression
-    : id_ ('(' columns = column_list ')')? AS '(' select_statement set_operators* ')'
+    : id_ (L_PAREN columns = column_list R_PAREN)? AS L_PAREN select_statement set_operators* R_PAREN
     ;
 
 select_statement
     : select_clause select_optional_clauses limit_clause?
     | select_top_clause select_optional_clauses //TOP and LIMIT are not allowed together
     ;
 
 set_operators
     : (UNION ALL? | EXCEPT | MINUS_ | INTERSECT) select_statement //EXCEPT and MINUS have same SQL meaning
-    | LR_BRACKET select_statement RR_BRACKET
+    | L_PAREN select_statement R_PAREN
     ;
 
 select_optional_clauses
     : into_clause? from_clause? where_clause? (group_by_clause | having_clause)? qualify_clause? order_by_clause?
     ;
 
 select_clause
@@ -4020,52 +4031,52 @@
     ;
 
 from_clause
     : FROM table_sources // object_ref join_clause*
     ;
 
 table_sources
-    : table_source (',' table_source)*
+    : table_source (COLON table_source)*
     ;
 
 table_source
     : table_source_item_joined
-    //| '(' table_source ')'
+    //| L_PAREN table_source R_PAREN
     ;
 
 table_source_item_joined
     : object_ref join_clause*
-    | '(' table_source_item_joined ')' join_clause*
+    | L_PAREN table_source_item_joined R_PAREN join_clause*
     ;
 
 object_ref
     : object_name at_before? changes? match_recognize? pivot_unpivot? as_alias? column_list_in_parentheses? sample?
     | object_name START WITH predicate CONNECT BY prior_list?
-    | TABLE '(' function_call ')' pivot_unpivot? as_alias? sample?
+    | TABLE L_PAREN function_call R_PAREN pivot_unpivot? as_alias? sample?
     | values_table sample?
-    | LATERAL? '(' subquery ')' pivot_unpivot? as_alias? column_list_in_parentheses?
+    | LATERAL? L_PAREN subquery R_PAREN pivot_unpivot? as_alias? column_list_in_parentheses?
     | LATERAL (flatten_table | splited_table) as_alias?
     //| AT id_ PATH?
-    //    ('(' FILE_FORMAT ASSOC id_ COMMA pattern_assoc ')')?
+    //    (L_PAREN FILE_FORMAT ASSOC id_ COMMA pattern_assoc R_PAREN)?
     //    as_alias?
     ;
 
 flatten_table_option
     : PATH_ ASSOC string
     | OUTER ASSOC true_false
     | RECURSIVE ASSOC true_false
     | MODE ASSOC (ARRAY_Q | OBJECT_Q | BOTH_Q)
     ;
 
 flatten_table
-    : FLATTEN LR_BRACKET (INPUT ASSOC)? expr (COMMA flatten_table_option)* RR_BRACKET
+    : FLATTEN L_PAREN (INPUT ASSOC)? expr (COMMA flatten_table_option)* R_PAREN
     ;
 
 splited_table
-    : SPLIT_TO_TABLE LR_BRACKET expr COMMA expr RR_BRACKET
+    : SPLIT_TO_TABLE L_PAREN expr COMMA expr R_PAREN
     ;
 
 prior_list
     : prior_item (COMMA prior_item)*
     ;
 
 prior_item
@@ -4078,36 +4089,36 @@
 
 join_type
     : INNER
     | outer_join
     ;
 
 join_clause
-    : join_type? JOIN object_ref ((ON search_condition)? | (USING '(' column_list ')')?)
-    //| join_type? JOIN object_ref (USING '(' column_list ')')?
+    : join_type? JOIN object_ref ((ON search_condition)? | (USING L_PAREN column_list R_PAREN)?)
+    //| join_type? JOIN object_ref (USING L_PAREN column_list R_PAREN)?
     | NATURAL outer_join? JOIN object_ref
     | CROSS JOIN object_ref
     ;
 
 at_before
-    : AT_KEYWORD LR_BRACKET (
+    : AT_KEYWORD L_PAREN (
         TIMESTAMP ASSOC expr
         | OFFSET ASSOC expr
         | STATEMENT ASSOC string
         | STREAM ASSOC string
-    ) RR_BRACKET
-    | BEFORE LR_BRACKET STATEMENT ASSOC string RR_BRACKET
+    ) R_PAREN
+    | BEFORE L_PAREN STATEMENT ASSOC string R_PAREN
     ;
 
 end
-    : END LR_BRACKET (TIMESTAMP ASSOC expr | OFFSET ASSOC expr | STATEMENT ASSOC string) RR_BRACKET
+    : END L_PAREN (TIMESTAMP ASSOC expr | OFFSET ASSOC expr | STATEMENT ASSOC string) R_PAREN
     ;
 
 changes
-    : CHANGES LR_BRACKET INFORMATION ASSOC default_append_only RR_BRACKET at_before end?
+    : CHANGES L_PAREN INFORMATION ASSOC default_append_only R_PAREN at_before end?
     ;
 
 default_append_only
     : DEFAULT
     | APPEND_ONLY
     ;
 
@@ -4155,60 +4166,60 @@
     ;
 
 define
     : DEFINE symbol_list
     ;
 
 match_recognize
-    : MATCH_RECOGNIZE LR_BRACKET partition_by? order_by_clause? measures? row_match? after_match? pattern? define? RR_BRACKET
+    : MATCH_RECOGNIZE L_PAREN partition_by? order_by_clause? measures? row_match? after_match? pattern? define? R_PAREN
     ;
 
 pivot_unpivot
-    : PIVOT LR_BRACKET id_ LR_BRACKET id_ RR_BRACKET FOR id_ IN LR_BRACKET literal (COMMA literal)* RR_BRACKET RR_BRACKET (
+    : PIVOT L_PAREN id_ L_PAREN id_ R_PAREN FOR id_ IN L_PAREN literal (COMMA literal)* R_PAREN R_PAREN (
         as_alias column_alias_list_in_brackets?
     )?
-    | UNPIVOT LR_BRACKET id_ FOR column_name IN LR_BRACKET column_list RR_BRACKET RR_BRACKET
+    | UNPIVOT L_PAREN id_ FOR column_name IN L_PAREN column_list R_PAREN R_PAREN
     ;
 
 column_alias_list_in_brackets
-    : LR_BRACKET id_ (COMMA id_)* RR_BRACKET
+    : L_PAREN id_ (COMMA id_)* R_PAREN
     ;
 
 expr_list_in_parentheses
-    : LR_BRACKET expr_list RR_BRACKET
+    : L_PAREN expr_list R_PAREN
     ;
 
 values_table
-    : LR_BRACKET values_table_body RR_BRACKET (as_alias column_alias_list_in_brackets?)?
+    : L_PAREN values_table_body R_PAREN (as_alias column_alias_list_in_brackets?)?
     | values_table_body (as_alias column_alias_list_in_brackets?)?
     ;
 
 values_table_body
     : VALUES expr_list_in_parentheses (COMMA expr_list_in_parentheses)*
     ;
 
 sample_method
     : row_sampling = (BERNOULLI | ROW)
     | block_sampling = ( SYSTEM | BLOCK)
     ;
 
 repeatable_seed
-    : (REPEATABLE | SEED) LR_BRACKET num RR_BRACKET
+    : (REPEATABLE | SEED) L_PAREN num R_PAREN
     ;
 
 sample_opts
-    : LR_BRACKET num ROWS? RR_BRACKET repeatable_seed?
+    : L_PAREN num ROWS? R_PAREN repeatable_seed?
     ;
 
 sample
     : (SAMPLE | TABLESAMPLE) sample_method? sample_opts
     ;
 
 search_condition
-    : NOT* (predicate | '(' search_condition ')')
+    : NOT* (predicate | L_PAREN search_condition R_PAREN)
     | search_condition AND search_condition
     | search_condition OR search_condition
     ;
 
 comparison_operator
     : EQ
     | GT
@@ -4224,22 +4235,17 @@
     ;
 
 subquery
     : query_statement
     ;
 
 predicate
-    : EXISTS LR_BRACKET subquery RR_BRACKET
-    | expr comparison_operator (ALL | SOME | ANY) '(' subquery ')'
-    | expr NOT? BETWEEN expr AND expr
-    | expr NOT? IN '(' (subquery | expr_list) ')'
-    | expr NOT? (LIKE | ILIKE) expr (ESCAPE expr)?
-    | expr NOT? RLIKE expr
-    | expr NOT? (LIKE | ILIKE) ANY LR_BRACKET expr (COMMA expr)* RR_BRACKET (ESCAPE expr)?
-    | expr IS null_not_null
+    : EXISTS L_PAREN subquery R_PAREN
+    | expr comparison_operator (ALL | SOME | ANY) L_PAREN subquery R_PAREN
+    | expr predicate_partial
     | expr
     ;
 
 where_clause
     : WHERE search_condition
     ;
 
@@ -4251,15 +4257,15 @@
 
 group_by_list
     : group_by_elem (COMMA group_by_elem)*
     ;
 
 group_by_clause
     : GROUP BY group_by_list having_clause?
-    | GROUP BY (CUBE | GROUPING SETS | ROLLUP) LR_BRACKET group_by_list RR_BRACKET
+    | GROUP BY (CUBE | GROUPING SETS | ROLLUP) L_PAREN group_by_list R_PAREN
     | GROUP BY ALL
     ;
 
 having_clause
     : HAVING search_condition
     ;
```

### Comparing `databricks_labs_remorph-0.1.7/core/src/main/antlr4/com/databricks/labs/remorph/parsers/tsql/TSqlLexer.g4` & `databricks_labs_remorph-0.2.0/core/src/main/antlr4/com/databricks/labs/remorph/parsers/tsql/TSqlLexer.g4`

 * *Files 10% similar despite different names*

```diff
@@ -82,25 +82,20 @@
 ANSI_NULL_DFLT_ON                           : 'ANSI_NULL_DFLT_ON';
 ANSI_PADDING                                : 'ANSI_PADDING';
 ANSI_WARNINGS                               : 'ANSI_WARNINGS';
 ANY                                         : 'ANY';
 APPEND                                      : 'APPEND';
 APPLICATION                                 : 'APPLICATION';
 APPLICATION_LOG                             : 'APPLICATION_LOG';
-APPLOCK_MODE                                : 'APPLOCK_MODE';
-APPLOCK_TEST                                : 'APPLOCK_TEST';
 APPLY                                       : 'APPLY';
-APP_NAME                                    : 'APP_NAME';
 ARITHABORT                                  : 'ARITHABORT';
 ARITHIGNORE                                 : 'ARITHIGNORE';
 AS                                          : 'AS';
 ASC                                         : 'ASC';
-ASCII                                       : 'ASCII';
 ASSEMBLY                                    : 'ASSEMBLY';
-ASSEMBLYPROPERTY                            : 'ASSEMBLYPROPERTY';
 ASYMMETRIC                                  : 'ASYMMETRIC';
 ASYNCHRONOUS_COMMIT                         : 'ASYNCHRONOUS_COMMIT';
 AT_KEYWORD                                  : 'AT';
 AUDIT                                       : 'AUDIT';
 AUDIT_GUID                                  : 'AUDIT_GUID';
 AUTHENTICATE                                : 'AUTHENTICATE';
 AUTHENTICATION                              : 'AUTHENTICATION';
@@ -115,15 +110,14 @@
 AUTO_CREATE_STATISTICS                      : 'AUTO_CREATE_STATISTICS';
 AUTO_DROP                                   : 'AUTO_DROP';
 AUTO_SHRINK                                 : 'AUTO_SHRINK';
 AUTO_UPDATE_STATISTICS                      : 'AUTO_UPDATE_STATISTICS';
 AUTO_UPDATE_STATISTICS_ASYNC                : 'AUTO_UPDATE_STATISTICS_ASYNC';
 AVAILABILITY                                : 'AVAILABILITY';
 AVAILABILITY_MODE                           : 'AVAILABILITY_MODE';
-AVG                                         : 'AVG';
 BACKSLASH                                   : '\\';
 BACKUP                                      : 'BACKUP';
 BACKUP_CLONEDB                              : 'BACKUP_CLONEDB';
 BACKUP_PRIORITY                             : 'BACKUP_PRIORITY';
 BASE64                                      : 'BASE64';
 BEFORE                                      : 'BEFORE';
 BEGIN                                       : 'BEGIN';
@@ -132,15 +126,14 @@
 BIGINT                                      : 'BIGINT';
 BINARY_CHECKSUM                             : 'BINARY_CHECKSUM';
 BINARY_KEYWORD                              : 'BINARY';
 BINDING                                     : 'BINDING';
 BLOB_STORAGE                                : 'BLOB_STORAGE';
 BLOCK                                       : 'BLOCK';
 BLOCKERS                                    : 'BLOCKERS';
-BLOCKING_HIERARCHY                          : 'BLOCKING_HIERARCHY';
 BLOCKSIZE                                   : 'BLOCKSIZE';
 BREAK                                       : 'BREAK';
 BROKER                                      : 'BROKER';
 BROKER_INSTANCE                             : 'BROKER_INSTANCE';
 BROWSE                                      : 'BROWSE';
 BUFFER                                      : 'BUFFER';
 BUFFERCOUNT                                 : 'BUFFERCOUNT';
@@ -152,160 +145,125 @@
 CALLER                                      : 'CALLER';
 CAP_CPU_PERCENT                             : 'CAP_CPU_PERCENT';
 CASCADE                                     : 'CASCADE';
 CASE                                        : 'CASE';
 CAST                                        : 'CAST';
 CATALOG                                     : 'CATALOG';
 CATCH                                       : 'CATCH';
-CERTENCODED                                 : 'CERTENCODED';
 CERTIFICATE                                 : 'CERTIFICATE';
-CERTPRIVATEKEY                              : 'CERTPRIVATEKEY';
-CERT_ID                                     : 'CERT_ID';
 CHANGE                                      : 'CHANGE';
 CHANGES                                     : 'CHANGES';
 CHANGETABLE                                 : 'CHANGETABLE';
 CHANGE_RETENTION                            : 'CHANGE_RETENTION';
 CHANGE_TRACKING                             : 'CHANGE_TRACKING';
-CHAR                                        : 'CHAR';
-CHARINDEX                                   : 'CHARINDEX';
 CHECK                                       : 'CHECK';
 CHECKALLOC                                  : 'CHECKALLOC';
 CHECKCATALOG                                : 'CHECKCATALOG';
 CHECKCONSTRAINTS                            : 'CHECKCONSTRAINTS';
 CHECKDB                                     : 'CHECKDB';
 CHECKFILEGROUP                              : 'CHECKFILEGROUP';
 CHECKPOINT                                  : 'CHECKPOINT';
 CHECKSUM                                    : 'CHECKSUM';
-CHECKSUM_AGG                                : 'CHECKSUM_AGG';
 CHECKTABLE                                  : 'CHECKTABLE';
 CHECK_EXPIRATION                            : 'CHECK_EXPIRATION';
 CHECK_POLICY                                : 'CHECK_POLICY';
 CLASSIFIER_FUNCTION                         : 'CLASSIFIER_FUNCTION';
 CLEANTABLE                                  : 'CLEANTABLE';
 CLEANUP                                     : 'CLEANUP';
 CLONEDATABASE                               : 'CLONEDATABASE';
 CLOSE                                       : 'CLOSE';
 CLUSTER                                     : 'CLUSTER';
 CLUSTERED                                   : 'CLUSTERED';
-COALESCE                                    : 'COALESCE';
 COLLATE                                     : 'COLLATE';
 COLLECTION                                  : 'COLLECTION';
 COLUMN                                      : 'COLUMN';
-COLUMNPROPERTY                              : 'COLUMNPROPERTY';
 COLUMNS                                     : 'COLUMNS';
 COLUMNSTORE                                 : 'COLUMNSTORE';
 COLUMNSTORE_ARCHIVE                         : 'COLUMNSTORE_ARCHIVE';
 COLUMN_ENCRYPTION_KEY                       : 'COLUMN_ENCRYPTION_KEY';
 COLUMN_MASTER_KEY                           : 'COLUMN_MASTER_KEY';
-COL_LENGTH                                  : 'COL_LENGTH';
-COL_NAME                                    : 'COL_NAME';
 COMMIT                                      : 'COMMIT';
 COMMITTED                                   : 'COMMITTED';
 COMPATIBILITY_LEVEL                         : 'COMPATIBILITY_LEVEL';
-COMPRESS                                    : 'COMPRESS';
 COMPRESSION                                 : 'COMPRESSION';
 COMPRESSION_DELAY                           : 'COMPRESSION_DELAY';
 COMPRESS_ALL_ROW_GROUPS                     : 'COMPRESS_ALL_ROW_GROUPS';
 COMPUTE                                     : 'COMPUTE';
 CONCAT                                      : 'CONCAT';
 CONCAT_NULL_YIELDS_NULL                     : 'CONCAT_NULL_YIELDS_NULL';
-CONCAT_WS                                   : 'CONCAT_WS';
 CONFIGURATION                               : 'CONFIGURATION';
 CONNECT                                     : 'CONNECT';
 CONNECTION                                  : 'CONNECTION';
-CONNECTIONPROPERTY                          : 'CONNECTIONPROPERTY';
 CONSTRAINT                                  : 'CONSTRAINT';
 CONTAINMENT                                 : 'CONTAINMENT';
 CONTAINS                                    : 'CONTAINS';
 CONTAINSTABLE                               : 'CONTAINSTABLE';
 CONTENT                                     : 'CONTENT';
 CONTEXT                                     : 'CONTEXT';
-CONTEXT_INFO                                : 'CONTEXT_INFO';
 CONTINUE                                    : 'CONTINUE';
 CONTINUE_AFTER_ERROR                        : 'CONTINUE_AFTER_ERROR';
 CONTRACT                                    : 'CONTRACT';
 CONTRACT_NAME                               : 'CONTRACT_NAME';
 CONTROL                                     : 'CONTROL';
 CONVERSATION                                : 'CONVERSATION';
-CONVERT                                     : 'TRY_'? 'CONVERT';
 COOKIE                                      : 'COOKIE';
 COPY_ONLY                                   : 'COPY_ONLY';
-COUNT                                       : 'COUNT';
 COUNTER                                     : 'COUNTER';
-COUNT_BIG                                   : 'COUNT_BIG';
 CPU                                         : 'CPU';
 CREATE                                      : 'CREATE';
 CREATE_NEW                                  : 'CREATE_NEW';
 CREATION_DISPOSITION                        : 'CREATION_DISPOSITION';
 CREDENTIAL                                  : 'CREDENTIAL';
 CROSS                                       : 'CROSS';
 CRYPTOGRAPHIC                               : 'CRYPTOGRAPHIC';
 CUME_DIST                                   : 'CUME_DIST';
 CURRENT                                     : 'CURRENT';
-CURRENT_DATE                                : 'CURRENT_DATE';
-CURRENT_REQUEST_ID                          : 'CURRENT_REQUEST_ID';
 CURRENT_TIME                                : 'CURRENT_TIME';
-CURRENT_TIMESTAMP                           : 'CURRENT_TIMESTAMP';
-CURRENT_TRANSACTION_ID                      : 'CURRENT_TRANSACTION_ID';
-CURRENT_USER                                : 'CURRENT_USER';
 CURSOR                                      : 'CURSOR';
 CURSOR_CLOSE_ON_COMMIT                      : 'CURSOR_CLOSE_ON_COMMIT';
 CURSOR_DEFAULT                              : 'CURSOR_DEFAULT';
-CURSOR_STATUS                               : 'CURSOR_STATUS';
 CYCLE                                       : 'CYCLE';
 DATA                                        : 'DATA';
 DATABASE                                    : 'DATABASE';
-DATABASEPROPERTYEX                          : 'DATABASEPROPERTYEX';
 DATABASE_MIRRORING                          : 'DATABASE_MIRRORING';
-DATABASE_PRINCIPAL_ID                       : 'DATABASE_PRINCIPAL_ID';
-DATALENGTH                                  : 'DATALENGTH';
 DATASPACE                                   : 'DATASPACE';
 DATA_COMPRESSION                            : 'DATA_COMPRESSION';
 DATA_PURITY                                 : 'DATA_PURITY';
 DATA_SOURCE                                 : 'DATA_SOURCE';
-DATEADD                                     : 'DATEADD';
-DATEDIFF                                    : 'DATEDIFF';
-DATENAME                                    : 'DATENAME';
-DATEPART                                    : 'DATEPART';
 DATE_CORRELATION_OPTIMIZATION               : 'DATE_CORRELATION_OPTIMIZATION';
 DAYS                                        : 'DAYS';
 DBCC                                        : 'DBCC';
 DBREINDEX                                   : 'DBREINDEX';
 DB_CHAINING                                 : 'DB_CHAINING';
 DB_FAILOVER                                 : 'DB_FAILOVER';
-DB_ID                                       : 'DB_ID';
-DB_NAME                                     : 'DB_NAME';
 DDL                                         : 'DDL';
 DEALLOCATE                                  : 'DEALLOCATE';
 DECLARE                                     : 'DECLARE';
-DECOMPRESS                                  : 'DECOMPRESS';
 DECRYPTION                                  : 'DECRYPTION';
 DEFAULT                                     : 'DEFAULT';
 DEFAULT_DATABASE                            : 'DEFAULT_DATABASE';
 DEFAULT_DOUBLE_QUOTE                        : ["]'DEFAULT' ["];
 DEFAULT_FULLTEXT_LANGUAGE                   : 'DEFAULT_FULLTEXT_LANGUAGE';
 DEFAULT_LANGUAGE                            : 'DEFAULT_LANGUAGE';
 DEFAULT_SCHEMA                              : 'DEFAULT_SCHEMA';
 DEFINITION                                  : 'DEFINITION';
 DELAY                                       : 'DELAY';
 DELAYED_DURABILITY                          : 'DELAYED_DURABILITY';
 DELETE                                      : 'DELETE';
 DELETED                                     : 'DELETED';
-DENSE_RANK                                  : 'DENSE_RANK';
 DENY                                        : 'DENY';
 DEPENDENTS                                  : 'DEPENDENTS';
 DES                                         : 'DES';
 DESC                                        : 'DESC';
 DESCRIPTION                                 : 'DESCRIPTION';
 DESX                                        : 'DESX';
 DETERMINISTIC                               : 'DETERMINISTIC';
 DHCP                                        : 'DHCP';
 DIAGNOSTICS                                 : 'DIAGNOSTICS';
 DIALOG                                      : 'DIALOG';
-DIFFERENCE                                  : 'DIFFERENCE';
 DIFFERENTIAL                                : 'DIFFERENTIAL';
 DIRECTORY_NAME                              : 'DIRECTORY_NAME';
 DISABLE                                     : 'DISABLE';
 DISABLED                                    : 'DISABLED';
 DISABLE_BROKER                              : 'DISABLE_BROKER';
 DISK                                        : 'DISK';
 DISTINCT                                    : 'DISTINCT';
@@ -335,33 +293,25 @@
 ENCRYPTION_TYPE                             : 'ENCRYPTION_TYPE';
 END                                         : 'END';
 ENDPOINT                                    : 'ENDPOINT';
 ENDPOINT_URL                                : 'ENDPOINT_URL';
 ERRLVL                                      : 'ERRLVL';
 ERROR                                       : 'ERROR';
 ERROR_BROKER_CONVERSATIONS                  : 'ERROR_BROKER_CONVERSATIONS';
-ERROR_LINE                                  : 'ERROR_LINE';
-ERROR_MESSAGE                               : 'ERROR_MESSAGE';
-ERROR_NUMBER                                : 'ERROR_NUMBER';
-ERROR_PROCEDURE                             : 'ERROR_PROCEDURE';
-ERROR_SEVERITY                              : 'ERROR_SEVERITY';
-ERROR_STATE                                 : 'ERROR_STATE';
 ESCAPE                                      : 'ESCAPE';
 ESTIMATEONLY                                : 'ESTIMATEONLY';
 EVENT                                       : 'EVENT';
 EVENTDATA                                   : 'EVENTDATA';
 EVENT_RETENTION_MODE                        : 'EVENT_RETENTION_MODE';
 EXCEPT                                      : 'EXCEPT';
 EXCLUSIVE                                   : 'EXCLUSIVE';
 EXECUTABLE                                  : 'EXECUTABLE';
 EXECUTABLE_FILE                             : 'EXECUTABLE_FILE';
 EXECUTE                                     : 'EXEC' 'UTE'?;
-EXIST                                       : 'EXIST';
 EXISTS                                      : 'EXISTS';
-EXIST_SQUARE_BRACKET                        : '[EXIST]';
 EXIT                                        : 'EXIT';
 EXPAND                                      : 'EXPAND';
 EXPIREDATE                                  : 'EXPIREDATE';
 EXPIRY_DATE                                 : 'EXPIRY_DATE';
 EXPLICIT                                    : 'EXPLICIT';
 EXTENDED_LOGICAL_CHECKS                     : 'EXTENDED_LOGICAL_CHECKS';
 EXTENSION                                   : 'EXTENSION';
@@ -375,27 +325,19 @@
 FAIL_OPERATION                              : 'FAIL_OPERATION';
 FAN_IN                                      : 'FAN_IN';
 FAST                                        : 'FAST';
 FAST_FORWARD                                : 'FAST_FORWARD';
 FETCH                                       : 'FETCH';
 FILE                                        : 'FILE';
 FILEGROUP                                   : 'FILEGROUP';
-FILEGROUPPROPERTY                           : 'FILEGROUPPROPERTY';
-FILEGROUP_ID                                : 'FILEGROUP_ID';
-FILEGROUP_NAME                              : 'FILEGROUP_NAME';
 FILEGROWTH                                  : 'FILEGROWTH';
 FILENAME                                    : 'FILENAME';
 FILEPATH                                    : 'FILEPATH';
-FILEPROPERTY                                : 'FILEPROPERTY';
-FILEPROPERTYEX                              : 'FILEPROPERTYEX';
 FILESTREAM                                  : 'FILESTREAM';
 FILESTREAM_ON                               : 'FILESTREAM_ON';
-FILE_ID                                     : 'FILE_ID';
-FILE_IDEX                                   : 'FILE_IDEX';
-FILE_NAME                                   : 'FILE_NAME';
 FILE_SNAPSHOT                               : 'FILE_SNAPSHOT';
 FILLFACTOR                                  : 'FILLFACTOR';
 FILTER                                      : 'FILTER';
 FIRST                                       : 'FIRST';
 FIRST_VALUE                                 : 'FIRST_VALUE';
 FMTONLY                                     : 'FMTONLY';
 FOLLOWING                                   : 'FOLLOWING';
@@ -404,73 +346,53 @@
 FORCED                                      : 'FORCED';
 FORCEPLAN                                   : 'FORCEPLAN';
 FORCESCAN                                   : 'FORCESCAN';
 FORCESEEK                                   : 'FORCESEEK';
 FORCE_FAILOVER_ALLOW_DATA_LOSS              : 'FORCE_FAILOVER_ALLOW_DATA_LOSS';
 FORCE_SERVICE_ALLOW_DATA_LOSS               : 'FORCE_SERVICE_ALLOW_DATA_LOSS';
 FOREIGN                                     : 'FOREIGN';
-FORMAT                                      : 'FORMAT';
-FORMATMESSAGE                               : 'FORMATMESSAGE';
 FORWARD_ONLY                                : 'FORWARD_ONLY';
+FORMAT                                      : 'FORMAT';
 FREE                                        : 'FREE';
 FREETEXT                                    : 'FREETEXT';
 FREETEXTTABLE                               : 'FREETEXTTABLE';
 FROM                                        : 'FROM';
 FULL                                        : 'FULL';
 FULLSCAN                                    : 'FULLSCAN';
 FULLTEXT                                    : 'FULLTEXT';
-FULLTEXTCATALOGPROPERTY                     : 'FULLTEXTCATALOGPROPERTY';
-FULLTEXTSERVICEPROPERTY                     : 'FULLTEXTSERVICEPROPERTY';
 FUNCTION                                    : 'FUNCTION';
 GB                                          : 'GB';
 GENERATED                                   : 'GENERATED';
 GET                                         : 'GET';
-GETANCESTOR                                 : 'GETANCESTOR';
-GETANSINULL                                 : 'GETANSINULL';
-GETDATE                                     : 'GETDATE';
-GETDESCENDANT                               : 'GETDESCENDANT';
-GETLEVEL                                    : 'GETLEVEL';
-GETREPARENTEDVALUE                          : 'GETREPARENTEDVALUE';
 GETROOT                                     : 'GETROOT';
-GETUTCDATE                                  : 'GETUTCDATE';
-GET_FILESTREAM_TRANSACTION_CONTEXT          : 'GET_FILESTREAM_TRANSACTION_CONTEXT';
 GLOBAL                                      : 'GLOBAL';
 GO                                          : 'GO';
 GOTO                                        : 'GOTO';
 GOVERNOR                                    : 'GOVERNOR';
 GRANT                                       : 'GRANT';
-GREATEST                                    : 'GREATEST';
 GROUP                                       : 'GROUP';
 GROUPING                                    : 'GROUPING';
-GROUPING_ID                                 : 'GROUPING_ID';
 GROUP_MAX_REQUESTS                          : 'GROUP_MAX_REQUESTS';
 HADR                                        : 'HADR';
 HASH                                        : 'HASH';
 HASHED                                      : 'HASHED';
-HAS_DBACCESS                                : 'HAS_DBACCESS';
-HAS_PERMS_BY_NAME                           : 'HAS_PERMS_BY_NAME';
 HAVING                                      : 'HAVING';
 HEALTHCHECKTIMEOUT                          : 'HEALTHCHECKTIMEOUT';
 HEALTH_CHECK_TIMEOUT                        : 'HEALTH_CHECK_TIMEOUT';
 HEAP                                        : 'HEAP';
 HIDDEN_KEYWORD                              : 'HIDDEN';
 HIERARCHYID                                 : 'HIERARCHYID';
 HIGH                                        : 'HIGH';
 HOLDLOCK                                    : 'HOLDLOCK';
 HONOR_BROKER_PRIORITY                       : 'HONOR_BROKER_PRIORITY';
-HOST_ID                                     : 'HOST_ID';
-HOST_NAME                                   : 'HOST_NAME';
 HOURS                                       : 'HOURS';
 IDENTITY                                    : 'IDENTITY';
 IDENTITYCOL                                 : 'IDENTITYCOL';
 IDENTITY_INSERT                             : 'IDENTITY_INSERT';
 IDENTITY_VALUE                              : 'IDENTITY_VALUE';
-IDENT_CURRENT                               : 'IDENT_CURRENT';
-IDENT_INCR                                  : 'IDENT_INCR';
-IDENT_SEED                                  : 'IDENT_SEED';
 IF                                          : 'IF';
 IGNORE_CONSTRAINTS                          : 'IGNORE_CONSTRAINTS';
 IGNORE_DUP_KEY                              : 'IGNORE_DUP_KEY';
 IGNORE_NONCLUSTERED_COLUMNSTORE_INDEX       : 'IGNORE_NONCLUSTERED_COLUMNSTORE_INDEX';
 IGNORE_REPLICATED_TABLE_CACHE               : 'IGNORE_REPLICATED_TABLE_CACHE';
 IGNORE_TRIGGERS                             : 'IGNORE_TRIGGERS';
 IIF                                         : 'IIF';
@@ -480,17 +402,14 @@
 IMPORTANCE                                  : 'IMPORTANCE';
 IN                                          : 'IN';
 INCLUDE                                     : 'INCLUDE';
 INCLUDE_NULL_VALUES                         : 'INCLUDE_NULL_VALUES';
 INCREMENT                                   : 'INCREMENT';
 INCREMENTAL                                 : 'INCREMENTAL';
 INDEX                                       : 'INDEX';
-INDEXKEY_PROPERTY                           : 'INDEXKEY_PROPERTY';
-INDEXPROPERTY                               : 'INDEXPROPERTY';
-INDEX_COL                                   : 'INDEX_COL';
 INFINITE                                    : 'INFINITE';
 INIT                                        : 'INIT';
 INITIATOR                                   : 'INITIATOR';
 INNER                                       : 'INNER';
 INPUT                                       : 'INPUT';
 INSENSITIVE                                 : 'INSENSITIVE';
 INSERT                                      : 'INSERT';
@@ -498,31 +417,20 @@
 INSTEAD                                     : 'INSTEAD';
 KWINT                                       : 'INT';
 INTERSECT                                   : 'INTERSECT';
 INTO                                        : 'INTO';
 IO                                          : 'IO';
 IP                                          : 'IP';
 IS                                          : 'IS';
-ISDESCENDANTOF                              : 'ISDESCENDANTOF';
-ISJSON                                      : 'ISJSON';
-ISNULL                                      : 'ISNULL';
-ISNUMERIC                                   : 'ISNUMERIC';
 ISOLATION                                   : 'ISOLATION';
-IS_MEMBER                                   : 'IS_MEMBER';
-IS_ROLEMEMBER                               : 'IS_ROLEMEMBER';
-IS_SRVROLEMEMBER                            : 'IS_SRVROLEMEMBER';
 JOB                                         : 'JOB';
 JOIN                                        : 'JOIN';
 JSON                                        : 'JSON';
 JSON_ARRAY                                  : 'JSON_ARRAY';
-JSON_MODIFY                                 : 'JSON_MODIFY';
 JSON_OBJECT                                 : 'JSON_OBJECT';
-JSON_PATH_EXISTS                            : 'JSON_PATH_EXISTS';
-JSON_QUERY                                  : 'JSON_QUERY';
-JSON_VALUE                                  : 'JSON_VALUE';
 KB                                          : 'KB';
 KEEP                                        : 'KEEP';
 KEEPDEFAULTS                                : 'KEEPDEFAULTS';
 KEEPFIXED                                   : 'KEEPFIXED';
 KEEPIDENTITY                                : 'KEEPIDENTITY';
 KERBEROS                                    : 'KERBEROS';
 KEY                                         : 'KEY';
@@ -533,43 +441,38 @@
 KEY_STORE_PROVIDER_NAME                     : 'KEY_STORE_PROVIDER_NAME';
 KILL                                        : 'KILL';
 LAG                                         : 'LAG';
 LANGUAGE                                    : 'LANGUAGE';
 LAST                                        : 'LAST';
 LAST_VALUE                                  : 'LAST_VALUE';
 LEAD                                        : 'LEAD';
-LEAST                                       : 'LEAST';
 LEFT                                        : 'LEFT';
-LEN                                         : 'LEN';
 LEVEL                                       : 'LEVEL';
 LIBRARY                                     : 'LIBRARY';
 LIFETIME                                    : 'LIFETIME';
 LIKE                                        : 'LIKE';
 LINENO                                      : 'LINENO';
 LINKED                                      : 'LINKED';
 LINUX                                       : 'LINUX';
 LIST                                        : 'LIST';
 LISTENER                                    : 'LISTENER';
 LISTENER_IP                                 : 'LISTENER_IP';
 LISTENER_PORT                               : 'LISTENER_PORT';
 LISTENER_URL                                : 'LISTENER_URL';
+LOG                                         : 'LOG';
 LOAD                                        : 'LOAD';
 LOB_COMPACTION                              : 'LOB_COMPACTION';
 LOCAL                                       : 'LOCAL';
 LOCAL_SERVICE_NAME                          : 'LOCAL_SERVICE_NAME';
 LOCATION                                    : 'LOCATION';
 LOCK                                        : 'LOCK';
 LOCK_ESCALATION                             : 'LOCK_ESCALATION';
-LOG                                         : 'LOG';
 LOGIN                                       : 'LOGIN';
-LOGINPROPERTY                               : 'LOGINPROPERTY';
 LOOP                                        : 'LOOP';
 LOW                                         : 'LOW';
-LOWER                                       : 'LOWER';
-LTRIM                                       : 'LTRIM';
 MANUAL                                      : 'MANUAL';
 MARK                                        : 'MARK';
 MASK                                        : 'MASK';
 MASKED                                      : 'MASKED';
 MASTER                                      : 'MASTER';
 MATCHED                                     : 'MATCHED';
 MATERIALIZED                                : 'MATERIALIZED';
@@ -600,38 +503,32 @@
 MEMBER                                      : 'MEMBER';
 MEMORY_OPTIMIZED_DATA                       : 'MEMORY_OPTIMIZED_DATA';
 MEMORY_PARTITION_MODE                       : 'MEMORY_PARTITION_MODE';
 MERGE                                       : 'MERGE';
 MESSAGE                                     : 'MESSAGE';
 MESSAGE_FORWARDING                          : 'MESSAGE_FORWARDING';
 MESSAGE_FORWARD_SIZE                        : 'MESSAGE_FORWARD_SIZE';
-MIN                                         : 'MIN';
 MINUTES                                     : 'MINUTES';
 MINVALUE                                    : 'MINVALUE';
-MIN_ACTIVE_ROWVERSION                       : 'MIN_ACTIVE_ROWVERSION';
 MIN_CPU_PERCENT                             : 'MIN_CPU_PERCENT';
 MIN_IOPS_PER_VOLUME                         : 'MIN_IOPS_PER_VOLUME';
 MIN_MEMORY_PERCENT                          : 'MIN_MEMORY_PERCENT';
 MIRROR                                      : 'MIRROR';
 MIRROR_ADDRESS                              : 'MIRROR_ADDRESS';
 MIXED_PAGE_ALLOCATION                       : 'MIXED_PAGE_ALLOCATION';
 MODE                                        : 'MODE';
 MODIFY                                      : 'MODIFY';
-MODIFY_SQUARE_BRACKET                       : '[MODIFY]';
 MOVE                                        : 'MOVE';
 MULTI_USER                                  : 'MULTI_USER';
 MUST_CHANGE                                 : 'MUST_CHANGE';
 NAME                                        : 'NAME';
 NATIONAL                                    : 'NATIONAL';
-NCHAR                                       : 'NCHAR';
 NEGOTIATE                                   : 'NEGOTIATE';
 NESTED_TRIGGERS                             : 'NESTED_TRIGGERS';
-NEWID                                       : 'NEWID';
 NEWNAME                                     : 'NEWNAME';
-NEWSEQUENTIALID                             : 'NEWSEQUENTIALID';
 NEW_ACCOUNT                                 : 'NEW_ACCOUNT';
 NEW_BROKER                                  : 'NEW_BROKER';
 NEW_PASSWORD                                : 'NEW_PASSWORD';
 NEXT                                        : 'NEXT';
 NO                                          : 'NO';
 NOCHECK                                     : 'NOCHECK';
 NOCOUNT                                     : 'NOCOUNT';
@@ -661,27 +558,20 @@
 NO_INFOMSGS                                 : 'NO_INFOMSGS';
 NO_QUERYSTORE                               : 'NO_QUERYSTORE';
 NO_STATISTICS                               : 'NO_STATISTICS';
 NO_TRUNCATE                                 : 'NO_TRUNCATE';
 NO_WAIT                                     : 'NO_WAIT';
 NTILE                                       : 'NTILE';
 NTLM                                        : 'NTLM';
-NULLIF                                      : 'NULLIF';
 NULL_                                       : 'NULL';
 NULL_DOUBLE_QUOTE                           : ["]'NULL' ["];
 NUMANODE                                    : 'NUMANODE';
 NUMBER                                      : 'NUMBER';
 NUMERIC_ROUNDABORT                          : 'NUMERIC_ROUNDABORT';
 OBJECT                                      : 'OBJECT';
-OBJECTPROPERTY                              : 'OBJECTPROPERTY';
-OBJECTPROPERTYEX                            : 'OBJECTPROPERTYEX';
-OBJECT_DEFINITION                           : 'OBJECT_DEFINITION';
-OBJECT_ID                                   : 'OBJECT_ID';
-OBJECT_NAME                                 : 'OBJECT_NAME';
-OBJECT_SCHEMA_NAME                          : 'OBJECT_SCHEMA_NAME';
 OF                                          : 'OF';
 OFF                                         : 'OFF';
 OFFLINE                                     : 'OFFLINE';
 OFFSET                                      : 'OFFSET';
 OFFSETS                                     : 'OFFSETS';
 OLD_ACCOUNT                                 : 'OLD_ACCOUNT';
 OLD_PASSWORD                                : 'OLD_PASSWORD';
@@ -699,47 +589,42 @@
 OPERATIONS                                  : 'OPERATIONS';
 OPTIMISTIC                                  : 'OPTIMISTIC';
 OPTIMIZE                                    : 'OPTIMIZE';
 OPTIMIZE_FOR_SEQUENTIAL_KEY                 : 'OPTIMIZE_FOR_SEQUENTIAL_KEY';
 OPTION                                      : 'OPTION';
 OR                                          : 'OR';
 ORDER                                       : 'ORDER';
-ORIGINAL_DB_NAME                            : 'ORIGINAL_DB_NAME';
-ORIGINAL_LOGIN                              : 'ORIGINAL_LOGIN';
 OUT                                         : 'OUT';
 OUTER                                       : 'OUTER';
 OUTPUT                                      : 'OUTPUT';
 OVER                                        : 'OVER';
 OVERRIDE                                    : 'OVERRIDE';
 OWNER                                       : 'OWNER';
 OWNERSHIP                                   : 'OWNERSHIP';
 PAD_INDEX                                   : 'PAD_INDEX';
 PAGE                                        : 'PAGE';
 PAGECOUNT                                   : 'PAGECOUNT';
 PAGE_VERIFY                                 : 'PAGE_VERIFY';
 PAGLOCK                                     : 'PAGLOCK';
 PARAMETERIZATION                            : 'PARAMETERIZATION';
 PARAM_NODE                                  : 'PARAM_NODE';
-PARSE                                       : 'TRY_'? 'PARSE';
-PARSENAME                                   : 'PARSENAME';
+PARSE                                       : 'PARSE';
 PARSEONLY                                   : 'PARSEONLY';
 PARTIAL                                     : 'PARTIAL';
 PARTITION                                   : 'PARTITION';
 PARTITIONS                                  : 'PARTITIONS';
 PARTNER                                     : 'PARTNER';
 PASSWORD                                    : 'PASSWORD';
 PATH                                        : 'PATH';
-PATINDEX                                    : 'PATINDEX';
 PAUSE                                       : 'PAUSE';
 PDW_SHOWSPACEUSED                           : 'PDW_SHOWSPACEUSED';
 PERCENT                                     : 'PERCENT';
 PERCENTILE_CONT                             : 'PERCENTILE_CONT';
 PERCENTILE_DISC                             : 'PERCENTILE_DISC';
 PERCENT_RANK                                : 'PERCENT_RANK';
-PERMISSIONS                                 : 'PERMISSIONS';
 PERMISSION_SET                              : 'PERMISSION_SET';
 PERSISTED                                   : 'PERSISTED';
 PERSIST_SAMPLE_PERCENT                      : 'PERSIST_SAMPLE_PERCENT';
 PER_CPU                                     : 'PER_CPU';
 PER_DB                                      : 'PER_DB';
 PER_NODE                                    : 'PER_NODE';
 PHYSICAL_ONLY                               : 'PHYSICAL_ONLY';
@@ -768,28 +653,23 @@
 PROCEDURE_NAME                              : 'PROCEDURE_NAME';
 PROCESS                                     : 'PROCESS';
 PROFILE                                     : 'PROFILE';
 PROPERTY                                    : 'PROPERTY';
 PROVIDER                                    : 'PROVIDER';
 PROVIDER_KEY_NAME                           : 'PROVIDER_KEY_NAME';
 PUBLIC                                      : 'PUBLIC';
-PWDCOMPARE                                  : 'PWDCOMPARE';
-PWDENCRYPT                                  : 'PWDENCRYPT';
 PYTHON                                      : 'PYTHON';
 QUERY                                       : 'QUERY';
-QUERY_SQUARE_BRACKET                        : '[QUERY]';
 QUEUE                                       : 'QUEUE';
 QUEUE_DELAY                                 : 'QUEUE_DELAY';
 QUOTED_IDENTIFIER                           : 'QUOTED_IDENTIFIER';
-QUOTENAME                                   : 'QUOTENAME';
 R                                           : 'R';
 RAISERROR                                   : 'RAISERROR';
 RANDOMIZED                                  : 'RANDOMIZED';
 RANGE                                       : 'RANGE';
-RANK                                        : 'RANK';
 RAW                                         : 'RAW';
 RC2                                         : 'RC2';
 RC4                                         : 'RC4';
 RC4_128                                     : 'RC4_128';
 READ                                        : 'READ';
 READCOMMITTED                               : 'READCOMMITTED';
 READCOMMITTEDLOCK                           : 'READCOMMITTEDLOCK';
@@ -822,15 +702,14 @@
 REPAIR_ALLOW_DATA_LOSS                      : 'REPAIR_ALLOW_DATA_LOSS';
 REPAIR_FAST                                 : 'REPAIR_FAST';
 REPAIR_REBUILD                              : 'REPAIR_REBUILD';
 REPEATABLE                                  : 'REPEATABLE';
 REPEATABLEREAD                              : 'REPEATABLEREAD';
 REPLACE                                     : 'REPLACE';
 REPLICA                                     : 'REPLICA';
-REPLICATE                                   : 'REPLICATE';
 REPLICATION                                 : 'REPLICATION';
 REQUEST_MAX_CPU_TIME_SEC                    : 'REQUEST_MAX_CPU_TIME_SEC';
 REQUEST_MAX_MEMORY_GRANT_PERCENT            : 'REQUEST_MAX_MEMORY_GRANT_PERCENT';
 REQUEST_MEMORY_GRANT_TIMEOUT_SEC            : 'REQUEST_MEMORY_GRANT_TIMEOUT_SEC';
 REQUIRED                                    : 'REQUIRED';
 REQUIRED_SYNCHRONIZED_SECONDARIES_TO_COMMIT : 'REQUIRED_SYNCHRONIZED_SECONDARIES_TO_COMMIT';
 RESAMPLE                                    : 'RESAMPLE';
@@ -845,52 +724,45 @@
 RESTRICTED_USER                             : 'RESTRICTED_USER';
 RESUMABLE                                   : 'RESUMABLE';
 RESUME                                      : 'RESUME';
 RETAINDAYS                                  : 'RETAINDAYS';
 RETENTION                                   : 'RETENTION';
 RETURN                                      : 'RETURN';
 RETURNS                                     : 'RETURNS';
-REVERSE                                     : 'REVERSE';
 REVERT                                      : 'REVERT';
 REVOKE                                      : 'REVOKE';
 REWIND                                      : 'REWIND';
 RIGHT                                       : 'RIGHT';
 ROBUST                                      : 'ROBUST';
 ROLE                                        : 'ROLE';
 ROLLBACK                                    : 'ROLLBACK';
 ROOT                                        : 'ROOT';
 ROUND_ROBIN                                 : 'ROUND_ROBIN';
 ROUTE                                       : 'ROUTE';
 ROW                                         : 'ROW';
 ROWCOUNT                                    : 'ROWCOUNT';
-ROWCOUNT_BIG                                : 'ROWCOUNT_BIG';
 ROWGUID                                     : 'ROWGUID';
 ROWGUIDCOL                                  : 'ROWGUIDCOL';
 ROWLOCK                                     : 'ROWLOCK';
 ROWS                                        : 'ROWS';
-ROW_NUMBER                                  : 'ROW_NUMBER';
 RSA_1024                                    : 'RSA_1024';
 RSA_2048                                    : 'RSA_2048';
 RSA_3072                                    : 'RSA_3072';
 RSA_4096                                    : 'RSA_4096';
 RSA_512                                     : 'RSA_512';
-RTRIM                                       : 'RTRIM';
 RULE                                        : 'RULE';
 SAFE                                        : 'SAFE';
 SAFETY                                      : 'SAFETY';
 SAMPLE                                      : 'SAMPLE';
 SAVE                                        : 'SAVE';
 SCHEDULER                                   : 'SCHEDULER';
 SCHEMA                                      : 'SCHEMA';
 SCHEMABINDING                               : 'SCHEMABINDING';
-SCHEMA_ID                                   : 'SCHEMA_ID';
-SCHEMA_NAME                                 : 'SCHEMA_NAME';
 SCHEME                                      : 'SCHEME';
 SCOPED                                      : 'SCOPED';
-SCOPE_IDENTITY                              : 'SCOPE_IDENTITY';
 SCRIPT                                      : 'SCRIPT';
 SCROLL                                      : 'SCROLL';
 SCROLL_LOCKS                                : 'SCROLL_LOCKS';
 SEARCH                                      : 'SEARCH';
 SECONDARY                                   : 'SECONDARY';
 SECONDARY_ONLY                              : 'SECONDARY_ONLY';
 SECONDARY_ROLE                              : 'SECONDARY_ROLE';
@@ -909,22 +781,19 @@
 SEMI_SENSITIVE                              : 'SEMI_SENSITIVE';
 SEND                                        : 'SEND';
 SENT                                        : 'SENT';
 SEQUENCE                                    : 'SEQUENCE';
 SEQUENCE_NUMBER                             : 'SEQUENCE_NUMBER';
 SERIALIZABLE                                : 'SERIALIZABLE';
 SERVER                                      : 'SERVER';
-SERVERPROPERTY                              : 'SERVERPROPERTY';
 SERVICE                                     : 'SERVICE';
 SERVICEBROKER                               : 'SERVICEBROKER';
 SERVICE_BROKER                              : 'SERVICE_BROKER';
 SERVICE_NAME                                : 'SERVICE_NAME';
 SESSION                                     : 'SESSION';
-SESSIONPROPERTY                             : 'SESSIONPROPERTY';
-SESSION_CONTEXT                             : 'SESSION_CONTEXT';
 SESSION_TIMEOUT                             : 'SESSION_TIMEOUT';
 SESSION_USER                                : 'SESSION_USER';
 SET                                         : 'SET';
 SETERROR                                    : 'SETERROR';
 SETS                                        : 'SETS';
 SETTINGS                                    : 'SETTINGS';
 SETUSER                                     : 'SETUSER';
@@ -944,61 +813,45 @@
 SIZE                                        : 'SIZE';
 SKIP_KEYWORD                                : 'SKIP';
 SMALLINT                                    : 'SMALLINT';
 SNAPSHOT                                    : 'SNAPSHOT';
 SOFTNUMA                                    : 'SOFTNUMA';
 SOME                                        : 'SOME';
 SORT_IN_TEMPDB                              : 'SORT_IN_TEMPDB';
-SOUNDEX                                     : 'SOUNDEX';
 SOURCE                                      : 'SOURCE';
-SPACE_KEYWORD                               : 'SPACE';
 SPARSE                                      : 'SPARSE';
 SPATIAL_WINDOW_MAX_CELLS                    : 'SPATIAL_WINDOW_MAX_CELLS';
 SPECIFICATION                               : 'SPECIFICATION';
 SPLIT                                       : 'SPLIT';
 SQL                                         : 'SQL';
 SQLDUMPERFLAGS                              : 'SQLDUMPERFLAGS';
 SQLDUMPERPATH                               : 'SQLDUMPERPATH';
 SQLDUMPERTIMEOUT                            : 'SQLDUMPERTIMEOUT';
-SQL_VARIANT_PROPERTY                        : 'SQL_VARIANT_PROPERTY';
 STANDBY                                     : 'STANDBY';
 START                                       : 'START';
 STARTED                                     : 'STARTED';
 STARTUP_STATE                               : 'STARTUP_STATE';
 START_DATE                                  : 'START_DATE';
 STATE                                       : 'STATE';
 STATIC                                      : 'STATIC';
 STATISTICS                                  : 'STATISTICS';
 STATISTICS_INCREMENTAL                      : 'STATISTICS_INCREMENTAL';
 STATISTICS_NORECOMPUTE                      : 'STATISTICS_NORECOMPUTE';
 STATS                                       : 'STATS';
-STATS_DATE                                  : 'STATS_DATE';
 STATS_STREAM                                : 'STATS_STREAM';
 STATUS                                      : 'STATUS';
 STATUSONLY                                  : 'STATUSONLY';
-STDEV                                       : 'STDEV';
-STDEVP                                      : 'STDEVP';
 STOP                                        : 'STOP';
 STOPLIST                                    : 'STOPLIST';
 STOPPED                                     : 'STOPPED';
 STOP_ON_ERROR                               : 'STOP_ON_ERROR';
-STR                                         : 'STR';
-STRING_AGG                                  : 'STRING_AGG';
-STRING_ESCAPE                               : 'STRING_ESCAPE';
-STUFF                                       : 'STUFF';
 SUBJECT                                     : 'SUBJECT';
 SUBSCRIBE                                   : 'SUBSCRIBE';
 SUBSCRIPTION                                : 'SUBSCRIPTION';
-SUBSTRING                                   : 'SUBSTRING';
-SUM                                         : 'SUM';
 SUPPORTED                                   : 'SUPPORTED';
-SUSER_ID                                    : 'SUSER_ID';
-SUSER_NAME                                  : 'SUSER_NAME';
-SUSER_SID                                   : 'SUSER_SID';
-SUSER_SNAME                                 : 'SUSER_SNAME';
 SUSPEND                                     : 'SUSPEND';
 SWITCH                                      : 'SWITCH';
 SYMMETRIC                                   : 'SYMMETRIC';
 SYNCHRONOUS_COMMIT                          : 'SYNCHRONOUS_COMMIT';
 SYNONYM                                     : 'SYNONYM';
 SYSTEM                                      : 'SYSTEM';
 SYSTEM_USER                                 : 'SYSTEM_USER';
@@ -1030,63 +883,52 @@
 TRACKING                                    : 'TRACKING';
 TRACK_CAUSALITY                             : 'TRACK_CAUSALITY';
 TRAN                                        : 'TRAN';
 TRANSACTION                                 : 'TRANSACTION';
 TRANSACTION_ID                              : 'TRANSACTION_ID';
 TRANSFER                                    : 'TRANSFER';
 TRANSFORM_NOISE_WORDS                       : 'TRANSFORM_NOISE_WORDS';
-TRANSLATE                                   : 'TRANSLATE';
 TRIGGER                                     : 'TRIGGER';
-TRIM                                        : 'TRIM';
 TRIPLE_DES                                  : 'TRIPLE_DES';
 TRIPLE_DES_3KEY                             : 'TRIPLE_DES_3KEY';
 TRUNCATE                                    : 'TRUNCATE';
 TRUSTWORTHY                                 : 'TRUSTWORTHY';
 TRY                                         : 'TRY';
 TRY_CAST                                    : 'TRY_CAST';
 TSEQUAL                                     : 'TSEQUAL';
 TSQL                                        : 'TSQL';
 TWO_DIGIT_YEAR_CUTOFF                       : 'TWO_DIGIT_YEAR_CUTOFF';
 TYPE                                        : 'TYPE';
-TYPEPROPERTY                                : 'TYPEPROPERTY';
-TYPE_ID                                     : 'TYPE_ID';
-TYPE_NAME                                   : 'TYPE_NAME';
 TYPE_WARNING                                : 'TYPE_WARNING';
 UNBOUNDED                                   : 'UNBOUNDED';
 UNCHECKED                                   : 'UNCHECKED';
 UNCOMMITTED                                 : 'UNCOMMITTED';
-UNICODE                                     : 'UNICODE';
 UNION                                       : 'UNION';
 UNIQUE                                      : 'UNIQUE';
 UNKNOWN                                     : 'UNKNOWN';
 UNLIMITED                                   : 'UNLIMITED';
 UNLOCK                                      : 'UNLOCK';
 UNMASK                                      : 'UNMASK';
 UNPIVOT                                     : 'UNPIVOT';
 UNSAFE                                      : 'UNSAFE';
 UOW                                         : 'UOW';
 UPDATE                                      : 'UPDATE';
 UPDATETEXT                                  : 'UPDATETEXT';
 UPDLOCK                                     : 'UPDLOCK';
-UPPER                                       : 'UPPER';
 URL                                         : 'URL';
 USE                                         : 'USE';
 USED                                        : 'USED';
 USER                                        : 'USER';
-USER_ID                                     : 'USER_ID';
-USER_NAME                                   : 'USER_NAME';
 USING                                       : 'USING';
 VALIDATION                                  : 'VALIDATION';
 VALID_XML                                   : 'VALID_XML';
 VALUE                                       : 'VALUE';
 VALUES                                      : 'VALUES';
-VALUE_SQUARE_BRACKET                        : '[VALUE]';
 VAR                                         : 'VAR';
 VARBINARY_KEYWORD                           : 'VARBINARY';
-VARP                                        : 'VARP';
 VARYING                                     : 'VARYING';
 VERBOSELOGGING                              : 'VERBOSELOGGING';
 VERIFY_CLONEDB                              : 'VERIFY_CLONEDB';
 VERSION                                     : 'VERSION';
 VIEW                                        : 'VIEW';
 VIEWS                                       : 'VIEWS';
 VIEW_METADATA                               : 'VIEW_METADATA';
@@ -1104,97 +946,23 @@
 WITHOUT                                     : 'WITHOUT';
 WITHOUT_ARRAY_WRAPPER                       : 'WITHOUT_ARRAY_WRAPPER';
 WITNESS                                     : 'WITNESS';
 WORK                                        : 'WORK';
 WORKLOAD                                    : 'WORKLOAD';
 WRITETEXT                                   : 'WRITETEXT';
 XACT_ABORT                                  : 'XACT_ABORT';
-XACT_STATE                                  : 'XACT_STATE';
 XLOCK                                       : 'XLOCK';
 XML                                         : 'XML';
 XMLDATA                                     : 'XMLDATA';
 XMLNAMESPACES                               : 'XMLNAMESPACES';
 XMLSCHEMA                                   : 'XMLSCHEMA';
 XML_COMPRESSION                             : 'XML_COMPRESSION';
 XSINIL                                      : 'XSINIL';
 ZONE                                        : 'ZONE';
 
-ABS     : 'ABS';
-ACOS    : 'ACOS';
-ASIN    : 'ASIN';
-ATAN    : 'ATAN';
-ATN2    : 'ATN2';
-CEILING : 'CEILING';
-COS     : 'COS';
-COT     : 'COT';
-DEGREES : 'DEGREES';
-EXP     : 'EXP';
-FLOOR   : 'FLOOR';
-LOG10   : 'LOG10';
-PI      : 'PI';
-POWER   : 'POWER';
-RADIANS : 'RADIANS';
-RAND    : 'RAND';
-ROUND   : 'ROUND';
-SIGN    : 'SIGN';
-SIN     : 'SIN';
-SQRT    : 'SQRT';
-SQUARE  : 'SQUARE';
-TAN     : 'TAN';
-
-CURRENT_TIMEZONE        : 'CURRENT_TIMEZONE';
-CURRENT_TIMEZONE_ID     : 'CURRENT_TIMEZONE_ID';
-DATE_BUCKET             : 'DATE_BUCKET';
-DATEDIFF_BIG            : 'DATEDIFF_BIG';
-DATEFROMPARTS           : 'DATEFROMPARTS';
-DATETIME2FROMPARTS      : 'DATETIME2FROMPARTS';
-DATETIMEFROMPARTS       : 'DATETIMEFROMPARTS';
-DATETIMEOFFSETFROMPARTS : 'DATETIMEOFFSETFROMPARTS';
-DATETRUNC               : 'DATETRUNC';
-DAY                     : 'DAY';
-EOMONTH                 : 'EOMONTH';
-ISDATE                  : 'ISDATE';
-MONTH                   : 'MONTH';
-SMALLDATETIMEFROMPARTS  : 'SMALLDATETIMEFROMPARTS';
-SWITCHOFFSET            : 'SWITCHOFFSET';
-SYSDATETIME             : 'SYSDATETIME';
-SYSDATETIMEOFFSET       : 'SYSDATETIMEOFFSET';
-SYSUTCDATETIME          : 'SYSUTCDATETIME';
-TIMEFROMPARTS           : 'TIMEFROMPARTS';
-TODATETIMEOFFSET        : 'TODATETIMEOFFSET';
-YEAR                    : 'YEAR';
-
-QUARTER     : 'QUARTER';
-DAYOFYEAR   : 'DAYOFYEAR';
-WEEK        : 'WEEK';
-HOUR        : 'HOUR';
-MINUTE      : 'MINUTE';
-SECOND      : 'SECOND';
-MILLISECOND : 'MILLISECOND';
-MICROSECOND : 'MICROSECOND';
-NANOSECOND  : 'NANOSECOND';
-TZOFFSET    : 'TZOFFSET';
-ISO_WEEK    : 'ISO_WEEK';
-WEEKDAY     : 'WEEKDAY';
-
-YEAR_ABBR        : 'yy' | 'yyyy';
-QUARTER_ABBR     : 'qq' | 'q';
-MONTH_ABBR       : 'mm' | 'm';
-DAYOFYEAR_ABBR   : 'dy' | 'y';
-DAY_ABBR         : 'dd' | 'd';
-WEEK_ABBR        : 'wk' | 'ww';
-HOUR_ABBR        : 'hh';
-MINUTE_ABBR      : 'mi' | 'n';
-SECOND_ABBR      : 'ss' | 's';
-MILLISECOND_ABBR : 'ms';
-MICROSECOND_ABBR : 'mcs';
-NANOSECOND_ABBR  : 'ns';
-TZOFFSET_ABBR    : 'tz';
-ISO_WEEK_ABBR    : 'isowk' | 'isoww';
-WEEKDAY_ABBR     : 'dw';
 
 SP_EXECUTESQL: 'SP_EXECUTESQL';
 
 //Build-ins:
 VARCHAR  : 'VARCHAR';
 NVARCHAR : 'NVARCHAR';
 
@@ -1217,37 +985,40 @@
 // TODO: ID can be not only Latin.
 DOUBLE_QUOTE_ID    : '"' ~'"'+ '"';
 DOUBLE_QUOTE_BLANK : '""';
 SINGLE_QUOTE       : '\'';
 SQUARE_BRACKET_ID  : '[' (~']' | ']' ']')* ']';
 LOCAL_ID           : '@' ([A-Z_$@#0-9] | FullWidthLetter)*;
 TEMP_ID            : '#' ([A-Z_$@#0-9] | FullWidthLetter)*;
-INT            : DEC_DIGIT+;
+
 ID                 : ( [A-Z_#] | FullWidthLetter) ( [A-Z_#$@0-9] | FullWidthLetter)*;
 STRING options {
     caseInsensitive = false;
 }      : 'N'? '\'' (~'\'' | '\'\'')* '\'';
-HEX : '0' 'X' HEX_DIGIT*;
-FLOAT  : DEC_DOT_DEC;
-REAL   : (INT | DEC_DOT_DEC) ('E' [+-]? DEC_DIGIT+);
 
-EQ: '=';
+fragment SIGN: [+-];
 
+INT         : SIGN? DEC_DIGIT+;
+HEX         : SIGN? '0' 'X' HEX_DIGIT*;
+FLOAT       : SIGN? DEC_DOT_DEC;
+REAL        : SIGN? (INT | DEC_DOT_DEC) ('E' [+-]? DEC_DIGIT+);
+MONEY       : SIGN? '$' (INT | FLOAT);
+
+EQ          : '=';
 GT          : '>';
 LT          : '<';
 BANG        : '!';
-
-PE  : '+=';
-ME : '-=';
-SE  : '*=';
-DE   : '/=';
-MEA   : '%=';
-AND_ASSIGN   : '&=';
-XOR_ASSIGN   : '^=';
-OR_ASSIGN    : '|=';
+PE          : '+=';
+ME          : '-=';
+SE          : '*=';
+DE          : '/=';
+MEA         : '%=';
+AND_ASSIGN  : '&=';
+XOR_ASSIGN  : '^=';
+OR_ASSIGN   : '|=';
 
 DOUBLE_BAR   : '||';
 DOT          : '.';
 UNDERLINE    : '_';
 AT           : '@';
 SHARP        : '#';
 DOLLAR       : '$';
@@ -1285,8 +1056,8 @@
     | '\u3040' ..'\u318f'
     | '\u3300' ..'\u337f'
     | '\u3400' ..'\u3fff'
     | '\u4e00' ..'\u9fff'
     | '\ua000' ..'\ud7ff'
     | '\uf900' ..'\ufaff'
     | '\uff00' ..'\ufff0'
-; // | '\u20000'..'\u2FA1F'
+; // | '\u20000'..'\u2FA1F'
```

### Comparing `databricks_labs_remorph-0.1.7/core/src/main/antlr4/com/databricks/labs/remorph/parsers/tsql/TSqlParser.g4` & `databricks_labs_remorph-0.2.0/core/src/main/antlr4/com/databricks/labs/remorph/parsers/tsql/TSqlParser.g4`

 * *Files 17% similar despite different names*

```diff
@@ -28,587 +28,586 @@
 
 parser grammar TSqlParser;
 
 options {
     tokenVocab = TSqlLexer;
 }
 
-tsql_file
-    : batch* EOF
-    | execute_body_batch go_statement* EOF
+tSqlFile
+    : batch? EOF
     ;
 
 batch
-    : go_statement
-    | execute_body_batch? (go_statement | sql_clauses+) go_statement*
-    | batch_level_statement go_statement*
-    ;
-
-batch_level_statement
-    : create_or_alter_function
-    | create_or_alter_procedure
-    | create_or_alter_trigger
-    | create_view
-    ;
-
-sql_clauses
-    : dml_clause SEMI?
-    | cfl_statement SEMI?
-    | another_statement SEMI?
-    | ddl_clause SEMI?
-    | dbcc_clause SEMI?
-    | backup_statement SEMI?
+    : goStatement
+    | executeBodyBatch? (goStatement | sqlClauses+) goStatement*
+    | batchLevelStatement goStatement*
+    ;
+
+batchLevelStatement
+    : createOrAlterFunction
+    | createOrAlterProcedure
+    | createOrAlterTrigger
+    | createView
+    ;
+
+sqlClauses
+    : dmlClause SEMI?
+    | cflStatement SEMI?
+    | anotherStatement SEMI?
+    | ddlClause SEMI?
+    | dbccClause SEMI?
+    | backupStatement SEMI?
     | SEMI
     ;
 
 // Data Manipulation Language: https://msdn.microsoft.com/en-us/library/ff848766(v=sql.120).aspx
-dml_clause
-    : merge_statement
-    | delete_statement
-    | insert_statement
-    | select_statement_standalone
-    | update_statement
+dmlClause
+    : mergeStatement
+    | deleteStatement
+    | insertStatement
+    | selectStatementStandalone
+    | updateStatement
     ;
 
 // Data Definition Language: https://msdn.microsoft.com/en-us/library/ff848799.aspx)
-ddl_clause
-    : alter_application_role
-    | alter_assembly
-    | alter_asymmetric_key
-    | alter_authorization
-    | alter_authorization_for_azure_dw
-    | alter_authorization_for_parallel_dw
-    | alter_authorization_for_sql_database
-    | alter_availability_group
-    | alter_certificate
-    | alter_column_encryption_key
-    | alter_credential
-    | alter_cryptographic_provider
-    | alter_database
-    | alter_database_audit_specification
-    | alter_db_role
-    | alter_endpoint
-    | alter_external_data_source
-    | alter_external_library
-    | alter_external_resource_pool
-    | alter_fulltext_catalog
-    | alter_fulltext_stoplist
-    | alter_index
-    | alter_login_azure_sql
-    | alter_login_azure_sql_dw_and_pdw
-    | alter_login_sql_server
-    | alter_master_key_azure_sql
-    | alter_master_key_sql_server
-    | alter_message_type
-    | alter_partition_function
-    | alter_partition_scheme
-    | alter_remote_service_binding
-    | alter_resource_governor
-    | alter_schema_azure_sql_dw_and_pdw
-    | alter_schema_sql
-    | alter_sequence
-    | alter_server_audit
-    | alter_server_audit_specification
-    | alter_server_configuration
-    | alter_server_role
-    | alter_server_role_pdw
-    | alter_service
-    | alter_service_master_key
-    | alter_symmetric_key
-    | alter_table
-    | alter_user
-    | alter_user_azure_sql
-    | alter_workload_group
-    | alter_xml_schema_collection
-    | create_application_role
-    | create_assembly
-    | create_asymmetric_key
-    | create_column_encryption_key
-    | create_column_master_key
-    | create_columnstore_index
-    | create_credential
-    | create_cryptographic_provider
-    | create_database
-    | create_database_audit_specification
-    | create_db_role
-    | create_endpoint
-    | create_event_notification
-    | create_external_library
-    | create_external_resource_pool
-    | create_fulltext_catalog
-    | create_fulltext_stoplist
-    | create_index
-    | create_login_azure_sql
-    | create_login_pdw
-    | create_login_sql_server
-    | create_master_key_azure_sql
-    | create_master_key_sql_server
-    | create_nonclustered_columnstore_index
-    | create_or_alter_broker_priority
-    | create_or_alter_event_session
-    | create_partition_function
-    | create_partition_scheme
-    | create_remote_service_binding
-    | create_resource_pool
-    | create_route
-    | create_rule
-    | create_schema
-    | create_schema_azure_sql_dw_and_pdw
-    | create_search_property_list
-    | create_security_policy
-    | create_sequence
-    | create_server_audit
-    | create_server_audit_specification
-    | create_server_role
-    | create_service
-    | create_statistics
-    | create_synonym
-    | create_table
-    | create_type
-    | create_user
-    | create_user_azure_sql_dw
-    | create_workload_group
-    | create_xml_index
-    | create_xml_schema_collection
-    | disable_trigger
-    | drop_aggregate
-    | drop_application_role
-    | drop_assembly
-    | drop_asymmetric_key
-    | drop_availability_group
-    | drop_broker_priority
-    | drop_certificate
-    | drop_column_encryption_key
-    | drop_column_master_key
-    | drop_contract
-    | drop_credential
-    | drop_cryptograhic_provider
-    | drop_database
-    | drop_database_audit_specification
-    | drop_database_encryption_key
-    | drop_database_scoped_credential
-    | drop_db_role
-    | drop_default
-    | drop_endpoint
-    | drop_event_notifications
-    | drop_event_session
-    | drop_external_data_source
-    | drop_external_file_format
-    | drop_external_library
-    | drop_external_resource_pool
-    | drop_external_table
-    | drop_fulltext_catalog
-    | drop_fulltext_index
-    | drop_fulltext_stoplist
-    | drop_function
-    | drop_index
-    | drop_login
-    | drop_master_key
-    | drop_message_type
-    | drop_partition_function
-    | drop_partition_scheme
-    | drop_procedure
-    | drop_queue
-    | drop_remote_service_binding
-    | drop_resource_pool
-    | drop_route
-    | drop_rule
-    | drop_schema
-    | drop_search_property_list
-    | drop_security_policy
-    | drop_sequence
-    | drop_server_audit
-    | drop_server_audit_specification
-    | drop_server_role
-    | drop_service
-    | drop_signature
-    | drop_statistics
-    | drop_statistics_name_azure_dw_and_pdw
-    | drop_symmetric_key
-    | drop_synonym
-    | drop_table
-    | drop_trigger
-    | drop_type
-    | drop_user
-    | drop_view
-    | drop_workload_group
-    | drop_xml_schema_collection
-    | enable_trigger
-    | lock_table
-    | truncate_table
-    | update_statistics
-    ;
-
-backup_statement
-    : backup_database
-    | backup_log
-    | backup_certificate
-    | backup_master_key
-    | backup_service_master_key
+ddlClause
+    : alterApplicationRole
+    | alterAssembly
+    | alterAsymmetricKey
+    | alterAuthorization
+    | alterAuthorizationForAzureDw
+    | alterAuthorizationForParallelDw
+    | alterAuthorizationForSqlDatabase
+    | alterAvailabilityGroup
+    | alterCertificate
+    | alterColumnEncryptionKey
+    | alterCredential
+    | alterCryptographicProvider
+    | alterDatabase
+    | alterDatabaseAuditSpecification
+    | alterDbRole
+    | alterEndpoint
+    | alterExternalDataSource
+    | alterExternalLibrary
+    | alterExternalResourcePool
+    | alterFulltextCatalog
+    | alterFulltextStoplist
+    | alterIndex
+    | alterLoginAzureSql
+    | alterLoginAzureSqlDwAndPdw
+    | alterLoginSqlServer
+    | alterMasterKeyAzureSql
+    | alterMasterKeySqlServer
+    | alterMessageType
+    | alterPartitionFunction
+    | alterPartitionScheme
+    | alterRemoteServiceBinding
+    | alterResourceGovernor
+    | alterSchemaAzureSqlDwAndPdw
+    | alterSchemaSql
+    | alterSequence
+    | alterServerAudit
+    | alterServerAuditSpecification
+    | alterServerConfiguration
+    | alterServerRole
+    | alterServerRolePdw
+    | alterService
+    | alterServiceMasterKey
+    | alterSymmetricKey
+    | alterTable
+    | alterUser
+    | alterUserAzureSql
+    | alterWorkloadGroup
+    | alterXmlSchemaCollection
+    | createApplicationRole
+    | createAssembly
+    | createAsymmetricKey
+    | createColumnEncryptionKey
+    | createColumnMasterKey
+    | createColumnstoreIndex
+    | createCredential
+    | createCryptographicProvider
+    | createDatabase
+    | createDatabaseAuditSpecification
+    | createDbRole
+    | createEndpoint
+    | createEventNotification
+    | createExternalLibrary
+    | createExternalResourcePool
+    | createFulltextCatalog
+    | createFulltextStoplist
+    | createIndex
+    | createLoginAzureSql
+    | createLoginPdw
+    | createLoginSqlServer
+    | createMasterKeyAzureSql
+    | createMasterKeySqlServer
+    | createNonclusteredColumnstoreIndex
+    | createOrAlterBrokerPriority
+    | createOrAlterEventSession
+    | createPartitionFunction
+    | createPartitionScheme
+    | createRemoteServiceBinding
+    | createResourcePool
+    | createRoute
+    | createRule
+    | createSchema
+    | createSchemaAzureSqlDwAndPdw
+    | createSearchPropertyList
+    | createSecurityPolicy
+    | createSequence
+    | createServerAudit
+    | createServerAuditSpecification
+    | createServerRole
+    | createService
+    | createStatistics
+    | createSynonym
+    | createTable
+    | createType
+    | createUser
+    | createUserAzureSqlDw
+    | createWorkloadGroup
+    | createXmlIndex
+    | createXmlSchemaCollection
+    | disableTrigger
+    | dropAggregate
+    | dropApplicationRole
+    | dropAssembly
+    | dropAsymmetricKey
+    | dropAvailabilityGroup
+    | dropBrokerPriority
+    | dropCertificate
+    | dropColumnEncryptionKey
+    | dropColumnMasterKey
+    | dropContract
+    | dropCredential
+    | dropCryptograhicProvider
+    | dropDatabase
+    | dropDatabaseAuditSpecification
+    | dropDatabaseEncryptionKey
+    | dropDatabaseScopedCredential
+    | dropDbRole
+    | dropDefault
+    | dropEndpoint
+    | dropEventNotifications
+    | dropEventSession
+    | dropExternalDataSource
+    | dropExternalFileFormat
+    | dropExternalLibrary
+    | dropExternalResourcePool
+    | dropExternalTable
+    | dropFulltextCatalog
+    | dropFulltextIndex
+    | dropFulltextStoplist
+    | dropFunction
+    | dropIndex
+    | dropLogin
+    | dropMasterKey
+    | dropMessageType
+    | dropPartitionFunction
+    | dropPartitionScheme
+    | dropProcedure
+    | dropQueue
+    | dropRemoteServiceBinding
+    | dropResourcePool
+    | dropRoute
+    | dropRule
+    | dropSchema
+    | dropSearchPropertyList
+    | dropSecurityPolicy
+    | dropSequence
+    | dropServerAudit
+    | dropServerAuditSpecification
+    | dropServerRole
+    | dropService
+    | dropSignature
+    | dropStatistics
+    | dropStatisticsNameAzureDwAndPdw
+    | dropSymmetricKey
+    | dropSynonym
+    | dropTable
+    | dropTrigger
+    | dropType
+    | dropUser
+    | dropView
+    | dropWorkloadGroup
+    | dropXmlSchemaCollection
+    | enableTrigger
+    | lockTable
+    | truncateTable
+    | updateStatistics
+    ;
+
+backupStatement
+    : backupDatabase
+    | backupLog
+    | backupCertificate
+    | backupMasterKey
+    | backupServiceMasterKey
     ;
 
 // Control-of-Flow Language: https://docs.microsoft.com/en-us/sql/t-sql/language-elements/control-of-flow
-cfl_statement
-    : block_statement
-    | break_statement
-    | continue_statement
-    | goto_statement
-    | if_statement
-    | print_statement
-    | raiseerror_statement
-    | return_statement
-    | throw_statement
-    | try_catch_statement
-    | waitfor_statement
-    | while_statement
+cflStatement
+    : blockStatement
+    | breakStatement
+    | continueStatement
+    | gotoStatement
+    | ifStatement
+    | printStatement
+    | raiseerrorStatement
+    | returnStatement
+    | throwStatement
+    | tryCatchStatement
+    | waitforStatement
+    | whileStatement
     ;
 
 // https://docs.microsoft.com/en-us/sql/t-sql/language-elements/begin-end-transact-sql
-block_statement
-    : BEGIN SEMI? sql_clauses* END SEMI?
+blockStatement
+    : BEGIN SEMI? sqlClauses* END SEMI?
     ;
 
 // https://docs.microsoft.com/en-us/sql/t-sql/language-elements/break-transact-sql
-break_statement
+breakStatement
     : BREAK SEMI?
     ;
 
 // https://docs.microsoft.com/en-us/sql/t-sql/language-elements/continue-transact-sql
-continue_statement
+continueStatement
     : CONTINUE SEMI?
     ;
 
 // https://docs.microsoft.com/en-us/sql/t-sql/language-elements/goto-transact-sql
-goto_statement
-    : GOTO id_ SEMI?
-    | id_ COLON SEMI?
+gotoStatement
+    : GOTO id SEMI?
+    | id COLON SEMI?
     ;
 
 // https://docs.microsoft.com/en-us/sql/t-sql/language-elements/return-transact-sql
-return_statement
+returnStatement
     : RETURN expression? SEMI?
     ;
 
 // https://docs.microsoft.com/en-us/sql/t-sql/language-elements/if-else-transact-sql
-if_statement
-    : IF search_condition sql_clauses (ELSE sql_clauses)? SEMI?
+ifStatement
+    : IF searchCondition sqlClauses (ELSE sqlClauses)? SEMI?
     ;
 
 // https://docs.microsoft.com/en-us/sql/t-sql/language-elements/throw-transact-sql
-throw_statement
-    : THROW (throw_error_number COMMA throw_message COMMA throw_state)? SEMI?
+throwStatement
+    : THROW (throwErrorNumber COMMA throwMessage COMMA throwState)? SEMI?
     ;
 
-throw_error_number
+throwErrorNumber
     : INT
     | LOCAL_ID
     ;
 
-throw_message
+throwMessage
     : STRING
     | LOCAL_ID
     ;
 
-throw_state
+throwState
     : INT
     | LOCAL_ID
     ;
 
 // https://docs.microsoft.com/en-us/sql/t-sql/language-elements/try-catch-transact-sql
-try_catch_statement
-    : BEGIN TRY SEMI? try_clauses = sql_clauses+ END TRY SEMI? BEGIN CATCH SEMI? catch_clauses = sql_clauses* END CATCH SEMI?
+tryCatchStatement
+    : BEGIN TRY SEMI? tryClauses = sqlClauses+ END TRY SEMI? BEGIN CATCH SEMI? catchClauses = sqlClauses* END CATCH SEMI?
     ;
 
 // https://docs.microsoft.com/en-us/sql/t-sql/language-elements/waitfor-transact-sql
-waitfor_statement
-    : WAITFOR receive_statement? COMMA? ((DELAY | TIME | TIMEOUT) time)? expression? SEMI?
+waitforStatement
+    : WAITFOR receiveStatement? COMMA? ((DELAY | TIME | TIMEOUT) time)? expression? SEMI?
     ;
 
 // https://docs.microsoft.com/en-us/sql/t-sql/language-elements/while-transact-sql
-while_statement
-    : WHILE search_condition (sql_clauses | BREAK SEMI? | CONTINUE SEMI?)
+whileStatement
+    : WHILE searchCondition (sqlClauses | BREAK SEMI? | CONTINUE SEMI?)
     ;
 
 // https://docs.microsoft.com/en-us/sql/t-sql/language-elements/print-transact-sql
-print_statement
+printStatement
     : PRINT (expression | DOUBLE_QUOTE_ID) (COMMA LOCAL_ID)* SEMI?
     ;
 
 // https://docs.microsoft.com/en-us/sql/t-sql/language-elements/raiserror-transact-sql
-raiseerror_statement
+raiseerrorStatement
     : RAISERROR LPAREN msg = (INT | STRING | LOCAL_ID) COMMA severity = constant_LOCAL_ID COMMA state = constant_LOCAL_ID (
         COMMA (constant_LOCAL_ID | NULL_)
     )* RPAREN (WITH (LOG | SETERROR | NOWAIT))? SEMI?
     | RAISERROR INT formatstring = (STRING | LOCAL_ID | DOUBLE_QUOTE_ID) (
         COMMA argument = (INT | STRING | LOCAL_ID)
     )*
     ;
 
-empty_statement
+emptyStatement
     : SEMI
     ;
 
-another_statement
-    : alter_queue
-    | checkpoint_statement
-    | conversation_statement
-    | create_contract
-    | create_queue
-    | cursor_statement
-    | declare_statement
-    | execute_statement
-    | kill_statement
-    | message_statement
-    | reconfigure_statement
-    | security_statement
-    | set_statement
-    | setuser_statement
-    | shutdown_statement
-    | transaction_statement
-    | use_statement
+anotherStatement
+    : alterQueue
+    | checkpointStatement
+    | conversationStatement
+    | createContract
+    | createQueue
+    | cursorStatement
+    | declareStatement
+    | executeStatement
+    | killStatement
+    | messageStatement
+    | reconfigureStatement
+    | securityStatement
+    | setStatement
+    | setuserStatement
+    | shutdownStatement
+    | transactionStatement
+    | useStatement
     ;
 
 // https://docs.microsoft.com/en-us/sql/t-sql/statements/alter-application-role-transact-sql
-alter_application_role
-    : ALTER APPLICATION ROLE appliction_role = id_ WITH (
-        COMMA? NAME EQ new_application_role_name = id_
-    )? (COMMA? PASSWORD EQ application_role_password = STRING)? (
-        COMMA? DEFAULT_SCHEMA EQ app_role_default_schema = id_
+alterApplicationRole
+    : ALTER APPLICATION ROLE applictionRole = id WITH (
+        COMMA? NAME EQ newApplicationRoleName = id
+    )? (COMMA? PASSWORD EQ applicationRolePassword = STRING)? (
+        COMMA? DEFAULT_SCHEMA EQ appRoleDefaultSchema = id
     )?
     ;
 
 // https://learn.microsoft.com/en-us/sql/t-sql/statements/alter-xml-schema-collection-transact-sql?view=sql-server-ver16
-alter_xml_schema_collection
-    : ALTER XML SCHEMA COLLECTION (id_ DOT)? id_ ADD STRING
+alterXmlSchemaCollection
+    : ALTER XML SCHEMA COLLECTION (id DOT)? id ADD STRING
     ;
 
-create_application_role
-    : CREATE APPLICATION ROLE appliction_role = id_ WITH (
-        COMMA? PASSWORD EQ application_role_password = STRING
-    )? (COMMA? DEFAULT_SCHEMA EQ app_role_default_schema = id_)?
+createApplicationRole
+    : CREATE APPLICATION ROLE applictionRole = id WITH (
+        COMMA? PASSWORD EQ applicationRolePassword = STRING
+    )? (COMMA? DEFAULT_SCHEMA EQ appRoleDefaultSchema = id)?
     ;
 
 // https://docs.microsoft.com/en-us/sql/t-sql/statements/drop-aggregate-transact-sql
 
-drop_aggregate
-    : DROP AGGREGATE (IF EXISTS)? (schema_name = id_ DOT)? aggregate_name = id_
+dropAggregate
+    : DROP AGGREGATE (IF EXISTS)? (schemaName = id DOT)? aggregateName = id
     ;
 
 // https://docs.microsoft.com/en-us/sql/t-sql/statements/drop-application-role-transact-sql
-drop_application_role
-    : DROP APPLICATION ROLE rolename = id_
+dropApplicationRole
+    : DROP APPLICATION ROLE rolename = id
     ;
 
-alter_assembly
-    : alter_assembly_start assembly_name = id_ alter_assembly_clause
+alterAssembly
+    : alterAssemblyStart assemblyName = id alterAssemblyClause
     ;
 
-alter_assembly_start
+alterAssemblyStart
     : ALTER ASSEMBLY
     ;
 
-alter_assembly_clause
-    : alter_assembly_from_clause? alter_assembly_with_clause? alter_assembly_drop_clause? alter_assembly_add_clause?
+alterAssemblyClause
+    : alterAssemblyFromClause? alterAssemblyWithClause? alterAssemblyDropClause? alterAssemblyAddClause?
     ;
 
-alter_assembly_from_clause
-    : alter_assembly_from_clause_start (client_assembly_specifier | alter_assembly_file_bits)
+alterAssemblyFromClause
+    : alterAssemblyFromClauseStart (clientAssemblySpecifier | alterAssemblyFileBits)
     ;
 
-alter_assembly_from_clause_start
+alterAssemblyFromClauseStart
     : FROM
     ;
 
-alter_assembly_drop_clause
-    : alter_assembly_drop alter_assembly_drop_multiple_files
+alterAssemblyDropClause
+    : alterAssemblyDrop alterAssemblyDropMultipleFiles
     ;
 
-alter_assembly_drop_multiple_files
+alterAssemblyDropMultipleFiles
     : ALL
-    | multiple_local_files
+    | multipleLocalFiles
     ;
 
-alter_assembly_drop
+alterAssemblyDrop
     : DROP
     ;
 
-alter_assembly_add_clause
-    : alter_asssembly_add_clause_start alter_assembly_client_file_clause
+alterAssemblyAddClause
+    : alterAsssemblyAddClauseStart alterAssemblyClientFileClause
     ;
 
-alter_asssembly_add_clause_start
+alterAsssemblyAddClauseStart
     : ADD FILE FROM
     ;
 
 // need to implement
-alter_assembly_client_file_clause
-    : alter_assembly_file_name (alter_assembly_as id_)?
+alterAssemblyClientFileClause
+    : alterAssemblyFileName (alterAssemblyAs id)?
     ;
 
-alter_assembly_file_name
+alterAssemblyFileName
     : STRING
     ;
 
 //need to implement
-alter_assembly_file_bits
-    : alter_assembly_as id_
+alterAssemblyFileBits
+    : alterAssemblyAs id
     ;
 
-alter_assembly_as
+alterAssemblyAs
     : AS
     ;
 
-alter_assembly_with_clause
-    : alter_assembly_with assembly_option
+alterAssemblyWithClause
+    : alterAssemblyWith assemblyOption
     ;
 
-alter_assembly_with
+alterAssemblyWith
     : WITH
     ;
 
-client_assembly_specifier
-    : network_file_share
-    | local_file
+clientAssemblySpecifier
+    : networkFileShare
+    | localFile
     | STRING
     ;
 
-assembly_option
+assemblyOption
     : PERMISSION_SET EQ (SAFE | EXTERNAL_ACCESS | UNSAFE)
-    | VISIBILITY EQ on_off
+    | VISIBILITY EQ onOff
     | UNCHECKED DATA
-    | assembly_option COMMA
+    | assemblyOption COMMA
     ;
 
-network_file_share
-    : BACKSLASH BACKSLASH network_computer file_path
+networkFileShare
+    : BACKSLASH BACKSLASH networkComputer filePath
     ;
 
-network_computer
-    : computer_name = id_
+networkComputer
+    : computerName = id
     ;
 
-file_path
-    : BACKSLASH file_path
-    | id_
+filePath
+    : BACKSLASH filePath
+    | id
     ;
 
-local_file
-    : local_drive file_path
+localFile
+    : localDrive filePath
     ;
 
-local_drive
+localDrive
     : DISK_DRIVE
     ;
 
-multiple_local_files
-    : multiple_local_file_start local_file SINGLE_QUOTE COMMA
-    | local_file
+multipleLocalFiles
+    : multipleLocalFileStart localFile SINGLE_QUOTE COMMA
+    | localFile
     ;
 
-multiple_local_file_start
+multipleLocalFileStart
     : SINGLE_QUOTE
     ;
 
 // https://docs.microsoft.com/en-us/sql/t-sql/statements/create-assembly-transact-sql
-create_assembly
-    : CREATE ASSEMBLY assembly_name = id_ (AUTHORIZATION owner_name = id_)? FROM (
+createAssembly
+    : CREATE ASSEMBLY assemblyName = id (AUTHORIZATION ownerName = id)? FROM (
         COMMA? (STRING | HEX)
     )+ (WITH PERMISSION_SET EQ (SAFE | EXTERNAL_ACCESS | UNSAFE))?
     ;
 
 // https://docs.microsoft.com/en-us/sql/t-sql/statements/drop-assembly-transact-sql
-drop_assembly
-    : DROP ASSEMBLY (IF EXISTS)? (COMMA? assembly_name = id_)+ (WITH NO DEPENDENTS)?
+dropAssembly
+    : DROP ASSEMBLY (IF EXISTS)? (COMMA? assemblyName = id)+ (WITH NO DEPENDENTS)?
     ;
 
 // https://docs.microsoft.com/en-us/sql/t-sql/statements/alter-asymmetric-key-transact-sql
 
-alter_asymmetric_key
-    : alter_asymmetric_key_start Asym_Key_Name = id_ (asymmetric_key_option | REMOVE PRIVATE KEY)
+alterAsymmetricKey
+    : alterAsymmetricKeyStart Asym_Key_Name = id (asymmetricKeyOption | REMOVE PRIVATE KEY)
     ;
 
-alter_asymmetric_key_start
+alterAsymmetricKeyStart
     : ALTER ASYMMETRIC KEY
     ;
 
-asymmetric_key_option
-    : asymmetric_key_option_start asymmetric_key_password_change_option (
-        COMMA asymmetric_key_password_change_option
+asymmetricKeyOption
+    : asymmetricKeyOptionStart asymmetricKeyPasswordChangeOption (
+        COMMA asymmetricKeyPasswordChangeOption
     )? RPAREN
     ;
 
-asymmetric_key_option_start
+asymmetricKeyOptionStart
     : WITH PRIVATE KEY LPAREN
     ;
 
-asymmetric_key_password_change_option
+asymmetricKeyPasswordChangeOption
     : DECRYPTION BY PASSWORD EQ STRING
     | ENCRYPTION BY PASSWORD EQ STRING
     ;
 
 //https://docs.microsoft.com/en-us/sql/t-sql/statements/create-asymmetric-key-transact-sql
 
-create_asymmetric_key
-    : CREATE ASYMMETRIC KEY Asym_Key_Nam = id_ (AUTHORIZATION database_principal_name = id_)? (
+createAsymmetricKey
+    : CREATE ASYMMETRIC KEY Asym_Key_Nam = id (AUTHORIZATION databasePrincipalName = id)? (
         FROM (
             FILE EQ STRING
             | EXECUTABLE_FILE EQ STRING
-            | ASSEMBLY Assembly_Name = id_
-            | PROVIDER Provider_Name = id_
+            | ASSEMBLY Assembly_Name = id
+            | PROVIDER Provider_Name = id
         )
     )? (
         WITH (
             ALGORITHM EQ (RSA_4096 | RSA_3072 | RSA_2048 | RSA_1024 | RSA_512)
-            | PROVIDER_KEY_NAME EQ provider_key_name = STRING
+            | PROVIDER_KEY_NAME EQ providerKeyName = STRING
             | CREATION_DISPOSITION EQ (CREATE_NEW | OPEN_EXISTING)
         )
-    )? (ENCRYPTION BY PASSWORD EQ asymmetric_key_password = STRING)?
+    )? (ENCRYPTION BY PASSWORD EQ asymmetricKeyPassword = STRING)?
     ;
 
 // https://docs.microsoft.com/en-us/sql/t-sql/statements/drop-asymmetric-key-transact-sql
-drop_asymmetric_key
-    : DROP ASYMMETRIC KEY key_name = id_ (REMOVE PROVIDER KEY)?
+dropAsymmetricKey
+    : DROP ASYMMETRIC KEY keyName = id (REMOVE PROVIDER KEY)?
     ;
 
 // https://docs.microsoft.com/en-us/sql/t-sql/statements/alter-authorization-transact-sql
 
-alter_authorization
-    : alter_authorization_start (class_type colon_colon)? entity = entity_name entity_to authorization_grantee
+alterAuthorization
+    : alterAuthorizationStart (classType colonColon)? entity = entityName entityTo authorizationGrantee
     ;
 
-authorization_grantee
-    : principal_name = id_
+authorizationGrantee
+    : principalName = id
     | SCHEMA OWNER
     ;
 
-entity_to
+entityTo
     : TO
     ;
 
-colon_colon
+colonColon
     : DOUBLE_COLON
     ;
 
-alter_authorization_start
+alterAuthorizationStart
     : ALTER AUTHORIZATION ON
     ;
 
-alter_authorization_for_sql_database
-    : alter_authorization_start (class_type_for_sql_database colon_colon)? entity = entity_name entity_to authorization_grantee
+alterAuthorizationForSqlDatabase
+    : alterAuthorizationStart (classTypeForSqlDatabase colonColon)? entity = entityName entityTo authorizationGrantee
     ;
 
-alter_authorization_for_azure_dw
-    : alter_authorization_start (class_type_for_azure_dw colon_colon)? entity = entity_name_for_azure_dw entity_to authorization_grantee
+alterAuthorizationForAzureDw
+    : alterAuthorizationStart (classTypeForAzureDw colonColon)? entity = entityNameForAzureDw entityTo authorizationGrantee
     ;
 
-alter_authorization_for_parallel_dw
-    : alter_authorization_start (class_type_for_parallel_dw colon_colon)? entity = entity_name_for_parallel_dw entity_to authorization_grantee
+alterAuthorizationForParallelDw
+    : alterAuthorizationStart (classTypeForParallelDw colonColon)? entity = entityNameForParallelDw entityTo authorizationGrantee
     ;
 
-class_type
+classType
     : OBJECT
     | ASSEMBLY
     | ASYMMETRIC KEY
     | AVAILABILITY GROUP
     | CERTIFICATE
     | CONTRACT
     | TYPE
@@ -624,15 +623,15 @@
     | SEARCH PROPERTY LIST
     | SERVER ROLE
     | SERVICE
     | SYMMETRIC KEY
     | XML SCHEMA COLLECTION
     ;
 
-class_type_for_sql_database
+classTypeForSqlDatabase
     : OBJECT
     | ASSEMBLY
     | ASYMMETRIC KEY
     | CERTIFICATE
     | TYPE
     | DATABASE
     | FULLTEXT CATALOG
@@ -640,30 +639,30 @@
     | ROLE
     | SCHEMA
     | SEARCH PROPERTY LIST
     | SYMMETRIC KEY
     | XML SCHEMA COLLECTION
     ;
 
-class_type_for_azure_dw
+classTypeForAzureDw
     : SCHEMA
     | OBJECT
     ;
 
-class_type_for_parallel_dw
+classTypeForParallelDw
     : DATABASE
     | SCHEMA
     | OBJECT
     ;
 
 // https://docs.microsoft.com/en-us/sql/t-sql/statements/grant-transact-sql?view=sql-server-ver15
 // SELECT DISTINCT '| ' + CLASS_DESC
-// FROM sys.dm_audit_actions
+// FROM sys.dmAuditActions
 // ORDER BY 1
-class_type_for_grant
+classTypeForGrant
     : APPLICATION ROLE
     | ASSEMBLY
     | ASYMMETRIC KEY
     | AUDIT
     | AVAILABILITY GROUP
     | BROKER PRIORITY
     | CERTIFICATE
@@ -699,40 +698,40 @@
     | TRIGGER ( DATABASE | SERVER)
     | TYPE
     | USER
     | XML SCHEMA COLLECTION
     ;
 
 // https://docs.microsoft.com/en-us/sql/t-sql/statements/drop-availability-group-transact-sql
-drop_availability_group
-    : DROP AVAILABILITY GROUP group_name = id_
+dropAvailabilityGroup
+    : DROP AVAILABILITY GROUP groupName = id
     ;
 
 // https://docs.microsoft.com/en-us/sql/t-sql/statements/alter-availability-group-transact-sql
-alter_availability_group
-    : alter_availability_group_start alter_availability_group_options
+alterAvailabilityGroup
+    : alterAvailabilityGroupStart alterAvailabilityGroupOptions
     ;
 
-alter_availability_group_start
-    : ALTER AVAILABILITY GROUP group_name = id_
+alterAvailabilityGroupStart
+    : ALTER AVAILABILITY GROUP groupName = id
     ;
 
-alter_availability_group_options
+alterAvailabilityGroupOptions
     : SET LPAREN (
         (
             AUTOMATED_BACKUP_PREFERENCE EQ (PRIMARY | SECONDARY_ONLY | SECONDARY | NONE)
             | FAILURE_CONDITION_LEVEL EQ INT
             | HEALTH_CHECK_TIMEOUT EQ milliseconds = INT
             | DB_FAILOVER EQ ( ON | OFF)
             | REQUIRED_SYNCHRONIZED_SECONDARIES_TO_COMMIT EQ INT
         ) RPAREN
     )
-    | ADD DATABASE database_name = id_
-    | REMOVE DATABASE database_name = id_
-    | ADD REPLICA ON server_instance = STRING (
+    | ADD DATABASE databaseName = id
+    | REMOVE DATABASE databaseName = id
+    | ADD REPLICA ON serverInstance = STRING (
         WITH LPAREN (
             (ENDPOINT_URL EQ STRING)? (
                 COMMA? AVAILABILITY_MODE EQ (SYNCHRONOUS_COMMIT | ASYNCHRONOUS_COMMIT)
             )? (COMMA? FAILOVER_MODE EQ (AUTOMATIC | MANUAL))? (
                 COMMA? SEEDING_MODE EQ (AUTOMATIC | MANUAL)
             )? (COMMA? BACKUP_PRIORITY EQ INT)? (
                 COMMA? PRIMARY_ROLE LPAREN ALLOW_CONNECTIONS EQ (READ_WRITE | ALL) RPAREN
@@ -742,798 +741,798 @@
     | SECONDARY_ROLE LPAREN (
         ALLOW_CONNECTIONS EQ (NO | READ_ONLY | ALL)
         | READ_ONLY_ROUTING_LIST EQ ( LPAREN ( ( STRING)) RPAREN)
     )
     | PRIMARY_ROLE LPAREN (
         ALLOW_CONNECTIONS EQ (NO | READ_ONLY | ALL)
         | READ_ONLY_ROUTING_LIST EQ (LPAREN ( (COMMA? STRING)* | NONE) RPAREN)
-        | SESSION_TIMEOUT EQ session_timeout = INT
+        | SESSION_TIMEOUT EQ sessionTimeout = INT
     )
-    | MODIFY REPLICA ON server_instance = STRING (
+    | MODIFY REPLICA ON serverInstance = STRING (
         WITH LPAREN (
             ENDPOINT_URL EQ STRING
             | AVAILABILITY_MODE EQ (SYNCHRONOUS_COMMIT | ASYNCHRONOUS_COMMIT)
             | FAILOVER_MODE EQ (AUTOMATIC | MANUAL)
             | SEEDING_MODE EQ (AUTOMATIC | MANUAL)
             | BACKUP_PRIORITY EQ INT
         )
         | SECONDARY_ROLE LPAREN (
             ALLOW_CONNECTIONS EQ (NO | READ_ONLY | ALL)
             | READ_ONLY_ROUTING_LIST EQ ( LPAREN ( ( STRING)) RPAREN)
         )
         | PRIMARY_ROLE LPAREN (
             ALLOW_CONNECTIONS EQ (NO | READ_ONLY | ALL)
             | READ_ONLY_ROUTING_LIST EQ (LPAREN ( (COMMA? STRING)* | NONE) RPAREN)
-            | SESSION_TIMEOUT EQ session_timeout = INT
+            | SESSION_TIMEOUT EQ sessionTimeout = INT
         )
     ) RPAREN
     | REMOVE REPLICA ON STRING
     | JOIN
     | JOIN AVAILABILITY GROUP ON (
-        COMMA? ag_name = STRING WITH LPAREN (
+        COMMA? agName = STRING WITH LPAREN (
             LISTENER_URL EQ STRING COMMA AVAILABILITY_MODE EQ (
                 SYNCHRONOUS_COMMIT
                 | ASYNCHRONOUS_COMMIT
             ) COMMA FAILOVER_MODE EQ MANUAL COMMA SEEDING_MODE EQ (AUTOMATIC | MANUAL) RPAREN
         )
     )+
     | MODIFY AVAILABILITY GROUP ON (
-        COMMA? ag_name_modified = STRING WITH LPAREN (
+        COMMA? agNameModified = STRING WITH LPAREN (
             LISTENER_URL EQ STRING (
                 COMMA? AVAILABILITY_MODE EQ (SYNCHRONOUS_COMMIT | ASYNCHRONOUS_COMMIT)
             )? (COMMA? FAILOVER_MODE EQ MANUAL)? (
                 COMMA? SEEDING_MODE EQ (AUTOMATIC | MANUAL)
             )? RPAREN
         )
     )+
     | GRANT CREATE ANY DATABASE
     | DENY CREATE ANY DATABASE
     | FAILOVER
     | FORCE_FAILOVER_ALLOW_DATA_LOSS
-    | ADD LISTENER listener_name = STRING LPAREN (
-        WITH DHCP (ON LPAREN ip_v4_failover ip_v4_failover RPAREN)
+    | ADD LISTENER listenerName = STRING LPAREN (
+        WITH DHCP (ON LPAREN ipV4_failover ipV4_failover RPAREN)
         | WITH IP LPAREN (
-            (COMMA? LPAREN ( ip_v4_failover COMMA ip_v4_failover | ip_v6_failover) RPAREN)+ RPAREN (
+            (COMMA? LPAREN ( ipV4_failover COMMA ipV4_failover | ipV6_failover) RPAREN)+ RPAREN (
                 COMMA PORT EQ INT
             )?
         )
     ) RPAREN
     | MODIFY LISTENER (
-        ADD IP LPAREN (ip_v4_failover ip_v4_failover | ip_v6_failover) RPAREN
+        ADD IP LPAREN (ipV4_failover ipV4_failover | ipV6_failover) RPAREN
         | PORT EQ INT
     )
     | RESTART LISTENER STRING
     | REMOVE LISTENER STRING
     | OFFLINE
     | WITH LPAREN DTC_SUPPORT EQ PER_DB RPAREN
     ;
 
-ip_v4_failover
+ipV4_failover
     : STRING
     ;
 
-ip_v6_failover
+ipV6_failover
     : STRING
     ;
 
 // https://docs.microsoft.com/en-us/sql/t-sql/statements/alter-broker-priority-transact-sql
 // https://docs.microsoft.com/en-us/sql/t-sql/statements/create-broker-priority-transact-sql
-create_or_alter_broker_priority
-    : (CREATE | ALTER) BROKER PRIORITY ConversationPriorityName = id_ FOR CONVERSATION SET LPAREN (
-        CONTRACT_NAME EQ ( ( id_) | ANY) COMMA?
-    )? (LOCAL_SERVICE_NAME EQ (DOUBLE_FORWARD_SLASH? id_ | ANY) COMMA?)? (
+createOrAlterBrokerPriority
+    : (CREATE | ALTER) BROKER PRIORITY ConversationPriorityName = id FOR CONVERSATION SET LPAREN (
+        CONTRACT_NAME EQ ( ( id) | ANY) COMMA?
+    )? (LOCAL_SERVICE_NAME EQ (DOUBLE_FORWARD_SLASH? id | ANY) COMMA?)? (
         REMOTE_SERVICE_NAME EQ (RemoteServiceName = STRING | ANY) COMMA?
     )? (PRIORITY_LEVEL EQ ( PriorityValue = INT | DEFAULT))? RPAREN
     ;
 
 // https://docs.microsoft.com/en-us/sql/t-sql/statements/drop-broker-priority-transact-sql
-drop_broker_priority
-    : DROP BROKER PRIORITY ConversationPriorityName = id_
+dropBrokerPriority
+    : DROP BROKER PRIORITY ConversationPriorityName = id
     ;
 
 // https://docs.microsoft.com/en-us/sql/t-sql/statements/alter-certificate-transact-sql
-alter_certificate
-    : ALTER CERTIFICATE certificate_name = id_ (
+alterCertificate
+    : ALTER CERTIFICATE certificateName = id (
         REMOVE PRIVATE_KEY
         | WITH PRIVATE KEY LPAREN (
             FILE EQ STRING COMMA?
             | DECRYPTION BY PASSWORD EQ STRING COMMA?
             | ENCRYPTION BY PASSWORD EQ STRING COMMA?
         )+ RPAREN
         | WITH ACTIVE FOR BEGIN_DIALOG EQ ( ON | OFF)
     )
     ;
 
 // https://docs.microsoft.com/en-us/sql/t-sql/statements/alter-column-encryption-key-transact-sql
-alter_column_encryption_key
-    : ALTER COLUMN ENCRYPTION KEY column_encryption_key = id_ (ADD | DROP) VALUE LPAREN COLUMN_MASTER_KEY EQ column_master_key_name = id_ (
-        COMMA ALGORITHM EQ algorithm_name = STRING COMMA ENCRYPTED_VALUE EQ HEX
+alterColumnEncryptionKey
+    : ALTER COLUMN ENCRYPTION KEY columnEncryptionKey = id (ADD | DROP) VALUE LPAREN COLUMN_MASTER_KEY EQ columnMasterKeyName = id (
+        COMMA ALGORITHM EQ algorithmName = STRING COMMA ENCRYPTED_VALUE EQ HEX
     )? RPAREN
     ;
 
 // https://docs.microsoft.com/en-us/sql/t-sql/statements/create-column-encryption-key-transact-sql
-create_column_encryption_key
-    : CREATE COLUMN ENCRYPTION KEY column_encryption_key = id_ WITH VALUES (
-        LPAREN COMMA? COLUMN_MASTER_KEY EQ column_master_key_name = id_ COMMA ALGORITHM EQ algorithm_name = STRING COMMA ENCRYPTED_VALUE
-            EQ encrypted_value = HEX RPAREN COMMA?
+createColumnEncryptionKey
+    : CREATE COLUMN ENCRYPTION KEY columnEncryptionKey = id WITH VALUES (
+        LPAREN COMMA? COLUMN_MASTER_KEY EQ columnMasterKeyName = id COMMA ALGORITHM EQ algorithmName = STRING COMMA ENCRYPTED_VALUE
+            EQ encryptedValue = HEX RPAREN COMMA?
     )+
     ;
 
 // https://docs.microsoft.com/en-us/sql/t-sql/statements/drop-certificate-transact-sql
-drop_certificate
-    : DROP CERTIFICATE certificate_name = id_
+dropCertificate
+    : DROP CERTIFICATE certificateName = id
     ;
 
 // https://docs.microsoft.com/en-us/sql/t-sql/statements/drop-column-encryption-key-transact-sql
-drop_column_encryption_key
-    : DROP COLUMN ENCRYPTION KEY key_name = id_
+dropColumnEncryptionKey
+    : DROP COLUMN ENCRYPTION KEY keyName = id
     ;
 
 // https://docs.microsoft.com/en-us/sql/t-sql/statements/drop-column-master-key-transact-sql
-drop_column_master_key
-    : DROP COLUMN MASTER KEY key_name = id_
+dropColumnMasterKey
+    : DROP COLUMN MASTER KEY keyName = id
     ;
 
 // https://docs.microsoft.com/en-us/sql/t-sql/statements/drop-contract-transact-sql
-drop_contract
-    : DROP CONTRACT dropped_contract_name = id_
+dropContract
+    : DROP CONTRACT droppedContractName = id
     ;
 
 // https://docs.microsoft.com/en-us/sql/t-sql/statements/drop-credential-transact-sql
-drop_credential
-    : DROP CREDENTIAL credential_name = id_
+dropCredential
+    : DROP CREDENTIAL credentialName = id
     ;
 
 // https://docs.microsoft.com/en-us/sql/t-sql/statements/drop-cryptographic-provider-transact-sql
-drop_cryptograhic_provider
-    : DROP CRYPTOGRAPHIC PROVIDER provider_name = id_
+dropCryptograhicProvider
+    : DROP CRYPTOGRAPHIC PROVIDER providerName = id
     ;
 
 // https://docs.microsoft.com/en-us/sql/t-sql/statements/drop-database-transact-sql
-drop_database
-    : DROP DATABASE (IF EXISTS)? (COMMA? database_name_or_database_snapshot_name = id_)+
+dropDatabase
+    : DROP DATABASE (IF EXISTS)? (COMMA? databaseNameOrDatabaseSnapshotName = id)+
     ;
 
 // https://docs.microsoft.com/en-us/sql/t-sql/statements/drop-database-audit-specification-transact-sql
-drop_database_audit_specification
-    : DROP DATABASE AUDIT SPECIFICATION audit_specification_name = id_
+dropDatabaseAuditSpecification
+    : DROP DATABASE AUDIT SPECIFICATION auditSpecificationName = id
     ;
 
 // https://docs.microsoft.com/en-us/sql/t-sql/statements/drop-database-encryption-key-transact-sql?view=sql-server-ver15
-drop_database_encryption_key
+dropDatabaseEncryptionKey
     : DROP DATABASE ENCRYPTION KEY
     ;
 
 // https://docs.microsoft.com/en-us/sql/t-sql/statements/drop-database-scoped-credential-transact-sql
-drop_database_scoped_credential
-    : DROP DATABASE SCOPED CREDENTIAL credential_name = id_
+dropDatabaseScopedCredential
+    : DROP DATABASE SCOPED CREDENTIAL credentialName = id
     ;
 
 // https://docs.microsoft.com/en-us/sql/t-sql/statements/drop-default-transact-sql
-drop_default
-    : DROP DEFAULT (IF EXISTS)? (COMMA? (schema_name = id_ DOT)? default_name = id_)
+dropDefault
+    : DROP DEFAULT (IF EXISTS)? (COMMA? (schemaName = id DOT)? defaultName = id)
     ;
 
 // https://docs.microsoft.com/en-us/sql/t-sql/statements/drop-endpoint-transact-sql
-drop_endpoint
-    : DROP ENDPOINT endPointName = id_
+dropEndpoint
+    : DROP ENDPOINT endPointName = id
     ;
 
 // https://docs.microsoft.com/en-us/sql/t-sql/statements/drop-external-data-source-transact-sql
-drop_external_data_source
-    : DROP EXTERNAL DATA SOURCE external_data_source_name = id_
+dropExternalDataSource
+    : DROP EXTERNAL DATA SOURCE externalDataSourceName = id
     ;
 
 // https://docs.microsoft.com/en-us/sql/t-sql/statements/drop-external-file-format-transact-sql
-drop_external_file_format
-    : DROP EXTERNAL FILE FORMAT external_file_format_name = id_
+dropExternalFileFormat
+    : DROP EXTERNAL FILE FORMAT externalFileFormatName = id
     ;
 
 // https://docs.microsoft.com/en-us/sql/t-sql/statements/drop-external-library-transact-sql
-drop_external_library
-    : DROP EXTERNAL LIBRARY library_name = id_ (AUTHORIZATION owner_name = id_)?
+dropExternalLibrary
+    : DROP EXTERNAL LIBRARY libraryName = id (AUTHORIZATION ownerName = id)?
     ;
 
 // https://docs.microsoft.com/en-us/sql/t-sql/statements/drop-external-resource-pool-transact-sql
-drop_external_resource_pool
-    : DROP EXTERNAL RESOURCE POOL pool_name = id_
+dropExternalResourcePool
+    : DROP EXTERNAL RESOURCE POOL poolName = id
     ;
 
 // https://docs.microsoft.com/en-us/sql/t-sql/statements/drop-external-table-transact-sql
-drop_external_table
-    : DROP EXTERNAL TABLE (database_name = id_ DOT)? (schema_name = id_ DOT)? table = id_
+dropExternalTable
+    : DROP EXTERNAL TABLE (databaseName = id DOT)? (schemaName = id DOT)? table = id
     ;
 
 // https://docs.microsoft.com/en-us/sql/t-sql/statements/drop-event-notification-transact-sql
-drop_event_notifications
-    : DROP EVENT NOTIFICATION (COMMA? notification_name = id_)+ ON (
+dropEventNotifications
+    : DROP EVENT NOTIFICATION (COMMA? notificationName = id)+ ON (
         SERVER
         | DATABASE
-        | QUEUE queue_name = id_
+        | QUEUE queueName = id
     )
     ;
 
 // https://docs.microsoft.com/en-us/sql/t-sql/statements/drop-event-session-transact-sql
-drop_event_session
-    : DROP EVENT SESSION event_session_name = id_ ON SERVER
+dropEventSession
+    : DROP EVENT SESSION eventSessionName = id ON SERVER
     ;
 
 // https://docs.microsoft.com/en-us/sql/t-sql/statements/drop-fulltext-catalog-transact-sql
-drop_fulltext_catalog
-    : DROP FULLTEXT CATALOG catalog_name = id_
+dropFulltextCatalog
+    : DROP FULLTEXT CATALOG catalogName = id
     ;
 
 // https://docs.microsoft.com/en-us/sql/t-sql/statements/drop-fulltext-index-transact-sql
-drop_fulltext_index
-    : DROP FULLTEXT INDEX ON (schema = id_ DOT)? table = id_
+dropFulltextIndex
+    : DROP FULLTEXT INDEX ON (schema = id DOT)? table = id
     ;
 
 // https://docs.microsoft.com/en-us/sql/t-sql/statements/drop-fulltext-stoplist-transact-sql
-drop_fulltext_stoplist
-    : DROP FULLTEXT STOPLIST stoplist_name = id_
+dropFulltextStoplist
+    : DROP FULLTEXT STOPLIST stoplistName = id
     ;
 
 // https://docs.microsoft.com/en-us/sql/t-sql/statements/drop-login-transact-sql
-drop_login
-    : DROP LOGIN login_name = id_
+dropLogin
+    : DROP LOGIN loginName = id
     ;
 
 // https://docs.microsoft.com/en-us/sql/t-sql/statements/drop-master-key-transact-sql
-drop_master_key
+dropMasterKey
     : DROP MASTER KEY
     ;
 
 // https://docs.microsoft.com/en-us/sql/t-sql/statements/drop-message-type-transact-sql
-drop_message_type
-    : DROP MESSAGE TYPE message_type_name = id_
+dropMessageType
+    : DROP MESSAGE TYPE messageTypeName = id
     ;
 
 // https://docs.microsoft.com/en-us/sql/t-sql/statements/drop-partition-function-transact-sql
-drop_partition_function
-    : DROP PARTITION FUNCTION partition_function_name = id_
+dropPartitionFunction
+    : DROP PARTITION FUNCTION partitionFunctionName = id
     ;
 
 // https://docs.microsoft.com/en-us/sql/t-sql/statements/drop-partition-scheme-transact-sql
-drop_partition_scheme
-    : DROP PARTITION SCHEME partition_scheme_name = id_
+dropPartitionScheme
+    : DROP PARTITION SCHEME partitionSchemeName = id
     ;
 
 // https://docs.microsoft.com/en-us/sql/t-sql/statements/drop-queue-transact-sql
-drop_queue
-    : DROP QUEUE (database_name = id_ DOT)? (schema_name = id_ DOT)? queue_name = id_
+dropQueue
+    : DROP QUEUE (databaseName = id DOT)? (schemaName = id DOT)? queueName = id
     ;
 
 // https://docs.microsoft.com/en-us/sql/t-sql/statements/drop-remote-service-binding-transact-sql
-drop_remote_service_binding
-    : DROP REMOTE SERVICE BINDING binding_name = id_
+dropRemoteServiceBinding
+    : DROP REMOTE SERVICE BINDING bindingName = id
     ;
 
 // https://docs.microsoft.com/en-us/sql/t-sql/statements/drop-resource-pool-transact-sql
-drop_resource_pool
-    : DROP RESOURCE POOL pool_name = id_
+dropResourcePool
+    : DROP RESOURCE POOL poolName = id
     ;
 
 // https://docs.microsoft.com/en-us/sql/t-sql/statements/drop-role-transact-sql
-drop_db_role
-    : DROP ROLE (IF EXISTS)? role_name = id_
+dropDbRole
+    : DROP ROLE (IF EXISTS)? roleName = id
     ;
 
 // https://docs.microsoft.com/en-us/sql/t-sql/statements/drop-route-transact-sql
-drop_route
-    : DROP ROUTE route_name = id_
+dropRoute
+    : DROP ROUTE routeName = id
     ;
 
 // https://docs.microsoft.com/en-us/sql/t-sql/statements/drop-rule-transact-sql
-drop_rule
-    : DROP RULE (IF EXISTS)? (COMMA? (schema_name = id_ DOT)? rule_name = id_)?
+dropRule
+    : DROP RULE (IF EXISTS)? (COMMA? (schemaName = id DOT)? ruleName = id)?
     ;
 
 // https://docs.microsoft.com/en-us/sql/t-sql/statements/drop-schema-transact-sql
-drop_schema
-    : DROP SCHEMA (IF EXISTS)? schema_name = id_
+dropSchema
+    : DROP SCHEMA (IF EXISTS)? schemaName = id
     ;
 
 // https://docs.microsoft.com/en-us/sql/t-sql/statements/drop-search-property-list-transact-sql
-drop_search_property_list
-    : DROP SEARCH PROPERTY LIST property_list_name = id_
+dropSearchPropertyList
+    : DROP SEARCH PROPERTY LIST propertyListName = id
     ;
 
 // https://docs.microsoft.com/en-us/sql/t-sql/statements/drop-security-policy-transact-sql
-drop_security_policy
-    : DROP SECURITY POLICY (IF EXISTS)? (schema_name = id_ DOT)? security_policy_name = id_
+dropSecurityPolicy
+    : DROP SECURITY POLICY (IF EXISTS)? (schemaName = id DOT)? securityPolicyName = id
     ;
 
 // https://docs.microsoft.com/en-us/sql/t-sql/statements/drop-sequence-transact-sql
-drop_sequence
+dropSequence
     : DROP SEQUENCE (IF EXISTS)? (
-        COMMA? (database_name = id_ DOT)? (schema_name = id_ DOT)? sequence_name = id_
+        COMMA? (databaseName = id DOT)? (schemaName = id DOT)? sequenceName = id
     )?
     ;
 
 // https://docs.microsoft.com/en-us/sql/t-sql/statements/drop-server-audit-transact-sql
-drop_server_audit
-    : DROP SERVER AUDIT audit_name = id_
+dropServerAudit
+    : DROP SERVER AUDIT auditName = id
     ;
 
 // https://docs.microsoft.com/en-us/sql/t-sql/statements/drop-server-audit-specification-transact-sql
-drop_server_audit_specification
-    : DROP SERVER AUDIT SPECIFICATION audit_specification_name = id_
+dropServerAuditSpecification
+    : DROP SERVER AUDIT SPECIFICATION auditSpecificationName = id
     ;
 
 // https://docs.microsoft.com/en-us/sql/t-sql/statements/drop-server-role-transact-sql
-drop_server_role
-    : DROP SERVER ROLE role_name = id_
+dropServerRole
+    : DROP SERVER ROLE roleName = id
     ;
 
 // https://docs.microsoft.com/en-us/sql/t-sql/statements/drop-service-transact-sql
-drop_service
-    : DROP SERVICE dropped_service_name = id_
+dropService
+    : DROP SERVICE droppedServiceName = id
     ;
 
 // https://docs.microsoft.com/en-us/sql/t-sql/statements/drop-signature-transact-sql
-drop_signature
-    : DROP (COUNTER)? SIGNATURE FROM (schema_name = id_ DOT)? module_name = id_ BY (
-        COMMA? CERTIFICATE cert_name = id_
-        | COMMA? ASYMMETRIC KEY Asym_key_name = id_
+dropSignature
+    : DROP (COUNTER)? SIGNATURE FROM (schemaName = id DOT)? moduleName = id BY (
+        COMMA? CERTIFICATE certName = id
+        | COMMA? ASYMMETRIC KEY AsymKeyName = id
     )+
     ;
 
-drop_statistics_name_azure_dw_and_pdw
-    : DROP STATISTICS (schema_name = id_ DOT)? object_name = id_ DOT statistics_name = id_
+dropStatisticsNameAzureDwAndPdw
+    : DROP STATISTICS (schemaName = id DOT)? objectName = id DOT statisticsName = id
     ;
 
 // https://docs.microsoft.com/en-us/sql/t-sql/statements/drop-symmetric-key-transact-sql
-drop_symmetric_key
-    : DROP SYMMETRIC KEY symmetric_key_name = id_ (REMOVE PROVIDER KEY)?
+dropSymmetricKey
+    : DROP SYMMETRIC KEY symmetricKeyName = id (REMOVE PROVIDER KEY)?
     ;
 
 // https://docs.microsoft.com/en-us/sql/t-sql/statements/drop-synonym-transact-sql
-drop_synonym
-    : DROP SYNONYM (IF EXISTS)? (schema = id_ DOT)? synonym_name = id_
+dropSynonym
+    : DROP SYNONYM (IF EXISTS)? (schema = id DOT)? synonymName = id
     ;
 
 // https://docs.microsoft.com/en-us/sql/t-sql/statements/drop-user-transact-sql
-drop_user
-    : DROP USER (IF EXISTS)? user_name = id_
+dropUser
+    : DROP USER (IF EXISTS)? userName = id
     ;
 
 // https://docs.microsoft.com/en-us/sql/t-sql/statements/drop-workload-group-transact-sql
-drop_workload_group
-    : DROP WORKLOAD GROUP group_name = id_
+dropWorkloadGroup
+    : DROP WORKLOAD GROUP groupName = id
     ;
 
 // https://docs.microsoft.com/en-us/sql/t-sql/statements/drop-xml-schema-collection-transact-sql
-drop_xml_schema_collection
-    : DROP XML SCHEMA COLLECTION (relational_schema = id_ DOT)? sql_identifier = id_
+dropXmlSchemaCollection
+    : DROP XML SCHEMA COLLECTION (relationalSchema = id DOT)? sqlIdentifier = id
     ;
 
 // https://docs.microsoft.com/en-us/sql/t-sql/statements/disable-trigger-transact-sql
-disable_trigger
-    : DISABLE TRIGGER (( COMMA? (schema_name = id_ DOT)? trigger_name = id_)+ | ALL) ON (
-        (schema_id = id_ DOT)? object_name = id_
+disableTrigger
+    : DISABLE TRIGGER (( COMMA? (schemaName = id DOT)? triggerName = id)+ | ALL) ON (
+        (schemaId = id DOT)? objectName = id
         | DATABASE
         | ALL SERVER
     )
     ;
 
 // https://docs.microsoft.com/en-us/sql/t-sql/statements/enable-trigger-transact-sql
-enable_trigger
-    : ENABLE TRIGGER (( COMMA? (schema_name = id_ DOT)? trigger_name = id_)+ | ALL) ON (
-        (schema_id = id_ DOT)? object_name = id_
+enableTrigger
+    : ENABLE TRIGGER (( COMMA? (schemaName = id DOT)? triggerName = id)+ | ALL) ON (
+        (schemaId = id DOT)? objectName = id
         | DATABASE
         | ALL SERVER
     )
     ;
 
-lock_table
-    : LOCK TABLE table_name IN (SHARE | EXCLUSIVE) MODE (WAIT seconds = INT | NOWAIT)? SEMI?
+lockTable
+    : LOCK TABLE tableName IN (SHARE | EXCLUSIVE) MODE (WAIT seconds = INT | NOWAIT)? SEMI?
     ;
 
 // https://docs.microsoft.com/en-us/sql/t-sql/statements/truncate-table-transact-sql
-truncate_table
-    : TRUNCATE TABLE table_name (
+truncateTable
+    : TRUNCATE TABLE tableName (
         WITH LPAREN PARTITIONS LPAREN (COMMA? (INT | INT TO INT))+ RPAREN RPAREN
     )?
     ;
 
 // https://docs.microsoft.com/en-us/sql/t-sql/statements/create-column-master-key-transact-sql
-create_column_master_key
-    : CREATE COLUMN MASTER KEY key_name = id_ WITH LPAREN KEY_STORE_PROVIDER_NAME EQ key_store_provider_name = STRING COMMA KEY_PATH EQ
-        key_path = STRING RPAREN
+createColumnMasterKey
+    : CREATE COLUMN MASTER KEY keyName = id WITH LPAREN KEY_STORE_PROVIDER_NAME EQ keyStoreProviderName = STRING COMMA KEY_PATH EQ
+        keyPath = STRING RPAREN
     ;
 
 // https://docs.microsoft.com/en-us/sql/t-sql/statements/alter-credential-transact-sql
-alter_credential
-    : ALTER CREDENTIAL credential_name = id_ WITH IDENTITY EQ identity_name = STRING (
+alterCredential
+    : ALTER CREDENTIAL credentialName = id WITH IDENTITY EQ identityName = STRING (
         COMMA SECRET EQ secret = STRING
     )?
     ;
 
 // https://docs.microsoft.com/en-us/sql/t-sql/statements/create-credential-transact-sql
-create_credential
-    : CREATE CREDENTIAL credential_name = id_ WITH IDENTITY EQ identity_name = STRING (
+createCredential
+    : CREATE CREDENTIAL credentialName = id WITH IDENTITY EQ identityName = STRING (
         COMMA SECRET EQ secret = STRING
-    )? (FOR CRYPTOGRAPHIC PROVIDER cryptographic_provider_name = id_)?
+    )? (FOR CRYPTOGRAPHIC PROVIDER cryptographicProviderName = id)?
     ;
 
 // https://docs.microsoft.com/en-us/sql/t-sql/statements/alter-cryptographic-provider-transact-sql
-alter_cryptographic_provider
-    : ALTER CRYPTOGRAPHIC PROVIDER provider_name = id_ (
-        FROM FILE EQ crypto_provider_ddl_file = STRING
+alterCryptographicProvider
+    : ALTER CRYPTOGRAPHIC PROVIDER providerName = id (
+        FROM FILE EQ cryptoProviderDdlFile = STRING
     )? (ENABLE | DISABLE)?
     ;
 
 // https://docs.microsoft.com/en-us/sql/t-sql/statements/create-cryptographic-provider-transact-sql
-create_cryptographic_provider
-    : CREATE CRYPTOGRAPHIC PROVIDER provider_name = id_ FROM FILE EQ path_of_DLL = STRING
+createCryptographicProvider
+    : CREATE CRYPTOGRAPHIC PROVIDER providerName = id FROM FILE EQ pathOf_DLL = STRING
     ;
 
 // https://learn.microsoft.com/en-us/sql/t-sql/statements/create-endpoint-transact-sql?view=sql-server-ver16
-create_endpoint
-    : CREATE ENDPOINT endpointname = id_ (AUTHORIZATION login = id_)? (
+createEndpoint
+    : CREATE ENDPOINT endpointname = id (AUTHORIZATION login = id)? (
         STATE EQ state = (STARTED | STOPPED | DISABLED)
-    )? AS TCP LPAREN endpoint_listener_clause RPAREN (
+    )? AS TCP LPAREN endpointListenerClause RPAREN (
         FOR TSQL LPAREN RPAREN
-        | FOR SERVICE_BROKER LPAREN endpoint_authentication_clause (
-            COMMA? endpoint_encryption_alogorithm_clause
+        | FOR SERVICE_BROKER LPAREN endpointAuthenticationClause (
+            COMMA? endpointEncryptionAlogorithmClause
         )? (COMMA? MESSAGE_FORWARDING EQ (ENABLED | DISABLED))? (
             COMMA? MESSAGE_FORWARD_SIZE EQ INT
         )? RPAREN
-        | FOR DATABASE_MIRRORING LPAREN endpoint_authentication_clause (
-            COMMA? endpoint_encryption_alogorithm_clause
+        | FOR DATABASE_MIRRORING LPAREN endpointAuthenticationClause (
+            COMMA? endpointEncryptionAlogorithmClause
         )? COMMA? ROLE EQ (WITNESS | PARTNER | ALL) RPAREN
     )
     ;
 
-endpoint_encryption_alogorithm_clause
+endpointEncryptionAlogorithmClause
     : ENCRYPTION EQ (DISABLED | SUPPORTED | REQUIRED) (ALGORITHM (AES RC4? | RC4 AES?))?
     ;
 
-endpoint_authentication_clause
+endpointAuthenticationClause
     : AUTHENTICATION EQ (
-        WINDOWS (NTLM | KERBEROS | NEGOTIATE)? (CERTIFICATE cert_name = id_)?
-        | CERTIFICATE cert_name = id_ WINDOWS? (NTLM | KERBEROS | NEGOTIATE)?
+        WINDOWS (NTLM | KERBEROS | NEGOTIATE)? (CERTIFICATE certName = id)?
+        | CERTIFICATE certName = id WINDOWS? (NTLM | KERBEROS | NEGOTIATE)?
     )
     ;
 
-endpoint_listener_clause
+endpointListenerClause
     : LISTENER_PORT EQ port = INT (
         COMMA LISTENER_IP EQ (ALL | LPAREN (ipv4 = IPV4_ADDR | ipv6 = STRING) RPAREN)
     )?
     ;
 
 // https://docs.microsoft.com/en-us/sql/t-sql/statements/create-event-notification-transact-sql
-create_event_notification
-    : CREATE EVENT NOTIFICATION event_notification_name = id_ ON (
+createEventNotification
+    : CREATE EVENT NOTIFICATION eventNotificationName = id ON (
         SERVER
         | DATABASE
-        | QUEUE queue_name = id_
-    ) (WITH FAN_IN)? FOR (COMMA? event_type_or_group = id_)+ TO SERVICE broker_service = STRING COMMA broker_service_specifier_or_current_database =
+        | QUEUE queueName = id
+    ) (WITH FAN_IN)? FOR (COMMA? eventTypeOrGroup = id)+ TO SERVICE brokerService = STRING COMMA brokerServiceSpecifierOrCurrentDatabase =
         STRING
     ;
 
 // https://docs.microsoft.com/en-us/sql/t-sql/statements/alter-event-session-transact-sql
 // https://docs.microsoft.com/en-us/sql/t-sql/statements/create-event-session-transact-sql
 // todo: not implemented
-create_or_alter_event_session
-    : (CREATE | ALTER) EVENT SESSION event_session_name = id_ ON SERVER (
+createOrAlterEventSession
+    : (CREATE | ALTER) EVENT SESSION eventSessionName = id ON SERVER (
         COMMA? ADD EVENT (
-            (event_module_guid = id_ DOT)? event_package_name = id_ DOT event_name = id_
+            (eventModuleGuid = id DOT)? eventPackageName = id DOT eventName = id
         ) (
-            LPAREN (SET ( COMMA? event_customizable_attributue = id_ EQ (INT | STRING))*)? (
+            LPAREN (SET ( COMMA? eventCustomizableAttributue = id EQ (INT | STRING))*)? (
                 ACTION LPAREN (
-                    COMMA? (event_module_guid = id_ DOT)? event_package_name = id_ DOT action_name = id_
+                    COMMA? (eventModuleGuid = id DOT)? eventPackageName = id DOT actionName = id
                 )+ RPAREN
-            )+ (WHERE event_session_predicate_expression)? RPAREN
+            )+ (WHERE eventSessionPredicateExpression)? RPAREN
         )*
     )* (
-        COMMA? DROP EVENT (event_module_guid = id_ DOT)? event_package_name = id_ DOT event_name = id_
+        COMMA? DROP EVENT (eventModuleGuid = id DOT)? eventPackageName = id DOT eventName = id
     )* (
-        (ADD TARGET (event_module_guid = id_ DOT)? event_package_name = id_ DOT target_name = id_) (
+        (ADD TARGET (eventModuleGuid = id DOT)? eventPackageName = id DOT targetName = id) (
             LPAREN SET (
-                COMMA? target_parameter_name = id_ EQ (LPAREN? INT RPAREN? | STRING)
+                COMMA? targetParameterName = id EQ (LPAREN? INT RPAREN? | STRING)
             )+ RPAREN
         )*
-    )* (DROP TARGET (event_module_guid = id_ DOT)? event_package_name = id_ DOT target_name = id_)* (
-        WITH LPAREN (COMMA? MAX_MEMORY EQ max_memory = INT (KB | MB))? (
+    )* (DROP TARGET (eventModuleGuid = id DOT)? eventPackageName = id DOT targetName = id)* (
+        WITH LPAREN (COMMA? MAX_MEMORY EQ maxMemory = INT (KB | MB))? (
             COMMA? EVENT_RETENTION_MODE EQ (
                 ALLOW_SINGLE_EVENT_LOSS
                 | ALLOW_MULTIPLE_EVENT_LOSS
                 | NO_EVENT_LOSS
             )
         )? (
             COMMA? MAX_DISPATCH_LATENCY EQ (
-                max_dispatch_latency_seconds = INT SECONDS
+                maxDispatchLatencySeconds = INT SECONDS
                 | INFINITE
             )
-        )? (COMMA? MAX_EVENT_SIZE EQ max_event_size = INT (KB | MB))? (
+        )? (COMMA? MAX_EVENT_SIZE EQ maxEventSize = INT (KB | MB))? (
             COMMA? MEMORY_PARTITION_MODE EQ (NONE | PER_NODE | PER_CPU)
         )? (COMMA? TRACK_CAUSALITY EQ (ON | OFF))? (COMMA? STARTUP_STATE EQ (ON | OFF))? RPAREN
     )? (STATE EQ (START | STOP))?
     ;
 
-event_session_predicate_expression
+eventSessionPredicateExpression
     : (
         COMMA? (AND | OR)? NOT? (
-            event_session_predicate_factor
-            | LPAREN event_session_predicate_expression RPAREN
+            eventSessionPredicateFactor
+            | LPAREN eventSessionPredicateExpression RPAREN
         )
     )+
     ;
 
-event_session_predicate_factor
-    : event_session_predicate_leaf
-    | LPAREN event_session_predicate_expression RPAREN
+eventSessionPredicateFactor
+    : eventSessionPredicateLeaf
+    | LPAREN eventSessionPredicateExpression RPAREN
     ;
 
-event_session_predicate_leaf
+eventSessionPredicateLeaf
     : (
-        event_field_name = id_
+        eventFieldName = id
         | (
-            event_field_name = id_
+            eventFieldName = id
             | (
-                (event_module_guid = id_ DOT)? event_package_name = id_ DOT predicate_source_name = id_
+                (eventModuleGuid = id DOT)? eventPackageName = id DOT predicateSourceName = id
             )
         ) (
             EQ
             | (LT GT)
             | (BANG EQ)
             | GT
             | (GT EQ)
             | LT
             | LT EQ
         ) (INT | STRING)
     )
-    | (event_module_guid = id_ DOT)? event_package_name = id_ DOT predicate_compare_name = id_ LPAREN (
-        event_field_name = id_
-        | ((event_module_guid = id_ DOT)? event_package_name = id_ DOT predicate_source_name = id_) COMMA (
+    | (eventModuleGuid = id DOT)? eventPackageName = id DOT predicateCompareName = id LPAREN (
+        eventFieldName = id
+        | ((eventModuleGuid = id DOT)? eventPackageName = id DOT predicateSourceName = id) COMMA (
             INT
             | STRING
         )
     ) RPAREN
     ;
 
 // https://docs.microsoft.com/en-us/sql/t-sql/statements/alter-external-data-source-transact-sql
-alter_external_data_source
-    : ALTER EXTERNAL DATA SOURCE data_source_name = id_ SET (
+alterExternalDataSource
+    : ALTER EXTERNAL DATA SOURCE dataSourceName = id SET (
         LOCATION EQ location = STRING COMMA?
-        | RESOURCE_MANAGER_LOCATION EQ resource_manager_location = STRING COMMA?
-        | CREDENTIAL EQ credential_name = id_
+        | RESOURCE_MANAGER_LOCATION EQ resourceManagerLocation = STRING COMMA?
+        | CREDENTIAL EQ credentialName = id
     )+
-    | ALTER EXTERNAL DATA SOURCE data_source_name = id_ WITH LPAREN TYPE EQ BLOB_STORAGE COMMA LOCATION EQ location = STRING (
-        COMMA CREDENTIAL EQ credential_name = id_
+    | ALTER EXTERNAL DATA SOURCE dataSourceName = id WITH LPAREN TYPE EQ BLOB_STORAGE COMMA LOCATION EQ location = STRING (
+        COMMA CREDENTIAL EQ credentialName = id
     )? RPAREN
     ;
 
 // https://docs.microsoft.com/en-us/sql/t-sql/statements/alter-external-library-transact-sql
-alter_external_library
-    : ALTER EXTERNAL LIBRARY library_name = id_ (AUTHORIZATION owner_name = id_)? (SET | ADD) (
-        LPAREN CONTENT EQ (client_library = STRING | HEX | NONE) (
+alterExternalLibrary
+    : ALTER EXTERNAL LIBRARY libraryName = id (AUTHORIZATION ownerName = id)? (SET | ADD) (
+        LPAREN CONTENT EQ (clientLibrary = STRING | HEX | NONE) (
             COMMA PLATFORM EQ (WINDOWS | LINUX)? RPAREN
         ) WITH (
             COMMA? LANGUAGE EQ (R | PYTHON)
-            | DATA_SOURCE EQ external_data_source_name = id_
+            | DATA_SOURCE EQ externalDataSourceName = id
         )+ RPAREN
     )
     ;
 
 // https://docs.microsoft.com/en-us/sql/t-sql/statements/create-external-library-transact-sql
-create_external_library
-    : CREATE EXTERNAL LIBRARY library_name = id_ (AUTHORIZATION owner_name = id_)? FROM (
-        COMMA? LPAREN? (CONTENT EQ)? (client_library = STRING | HEX | NONE) (
+createExternalLibrary
+    : CREATE EXTERNAL LIBRARY libraryName = id (AUTHORIZATION ownerName = id)? FROM (
+        COMMA? LPAREN? (CONTENT EQ)? (clientLibrary = STRING | HEX | NONE) (
             COMMA PLATFORM EQ (WINDOWS | LINUX)? RPAREN
         )?
     ) (
         WITH (
             COMMA? LANGUAGE EQ (R | PYTHON)
-            | DATA_SOURCE EQ external_data_source_name = id_
+            | DATA_SOURCE EQ externalDataSourceName = id
         )+ RPAREN
     )?
     ;
 
 // https://docs.microsoft.com/en-us/sql/t-sql/statements/alter-external-resource-pool-transact-sql
-alter_external_resource_pool
-    : ALTER EXTERNAL RESOURCE POOL (pool_name = id_ | DEFAULT_DOUBLE_QUOTE) WITH LPAREN MAX_CPU_PERCENT EQ max_cpu_percent = INT (
+alterExternalResourcePool
+    : ALTER EXTERNAL RESOURCE POOL (poolName = id | DEFAULT_DOUBLE_QUOTE) WITH LPAREN MAX_CPU_PERCENT EQ maxCpuPercent = INT (
         COMMA? AFFINITY CPU EQ (AUTO | (COMMA? INT TO INT | COMMA INT)+)
         | NUMANODE EQ (COMMA? INT TO INT | COMMA? INT)+
-    ) (COMMA? MAX_MEMORY_PERCENT EQ max_memory_percent = INT)? (
-        COMMA? MAX_PROCESSES EQ max_processes = INT
+    ) (COMMA? MAX_MEMORY_PERCENT EQ maxMemoryPercent = INT)? (
+        COMMA? MAX_PROCESSES EQ maxProcesses = INT
     )? RPAREN
     ;
 
 // https://docs.microsoft.com/en-us/sql/t-sql/statements/create-external-resource-pool-transact-sql
-create_external_resource_pool
-    : CREATE EXTERNAL RESOURCE POOL pool_name = id_ WITH LPAREN MAX_CPU_PERCENT EQ max_cpu_percent = INT (
+createExternalResourcePool
+    : CREATE EXTERNAL RESOURCE POOL poolName = id WITH LPAREN MAX_CPU_PERCENT EQ maxCpuPercent = INT (
         COMMA? AFFINITY CPU EQ (AUTO | (COMMA? INT TO INT | COMMA INT)+)
         | NUMANODE EQ (COMMA? INT TO INT | COMMA? INT)+
-    ) (COMMA? MAX_MEMORY_PERCENT EQ max_memory_percent = INT)? (
-        COMMA? MAX_PROCESSES EQ max_processes = INT
+    ) (COMMA? MAX_MEMORY_PERCENT EQ maxMemoryPercent = INT)? (
+        COMMA? MAX_PROCESSES EQ maxProcesses = INT
     )? RPAREN
     ;
 
 // https://docs.microsoft.com/en-us/sql/t-sql/statements/alter-fulltext-catalog-transact-sql
-alter_fulltext_catalog
-    : ALTER FULLTEXT CATALOG catalog_name = id_ (
+alterFulltextCatalog
+    : ALTER FULLTEXT CATALOG catalogName = id (
         REBUILD (WITH ACCENT_SENSITIVITY EQ (ON | OFF))?
         | REORGANIZE
         | AS DEFAULT
     )
     ;
 
 // https://docs.microsoft.com/en-us/sql/t-sql/statements/create-fulltext-catalog-transact-sql
-create_fulltext_catalog
-    : CREATE FULLTEXT CATALOG catalog_name = id_ (ON FILEGROUP filegroup = id_)? (
+createFulltextCatalog
+    : CREATE FULLTEXT CATALOG catalogName = id (ON FILEGROUP filegroup = id)? (
         IN PATH rootpath = STRING
-    )? (WITH ACCENT_SENSITIVITY EQ (ON | OFF))? (AS DEFAULT)? (AUTHORIZATION owner_name = id_)?
+    )? (WITH ACCENT_SENSITIVITY EQ (ON | OFF))? (AS DEFAULT)? (AUTHORIZATION ownerName = id)?
     ;
 
 // https://docs.microsoft.com/en-us/sql/t-sql/statements/alter-fulltext-stoplist-transact-sql
-alter_fulltext_stoplist
-    : ALTER FULLTEXT STOPLIST stoplist_name = id_ (
+alterFulltextStoplist
+    : ALTER FULLTEXT STOPLIST stoplistName = id (
         ADD stopword = STRING LANGUAGE (STRING | INT | HEX)
         | DROP (
             stopword = STRING LANGUAGE (STRING | INT | HEX)
             | ALL (STRING | INT | HEX)
             | ALL
         )
     )
     ;
 
 // https://docs.microsoft.com/en-us/sql/t-sql/statements/create-fulltext-stoplist-transact-sql
-create_fulltext_stoplist
-    : CREATE FULLTEXT STOPLIST stoplist_name = id_ (
-        FROM ((database_name = id_ DOT)? source_stoplist_name = id_ | SYSTEM STOPLIST)
-    )? (AUTHORIZATION owner_name = id_)?
+createFulltextStoplist
+    : CREATE FULLTEXT STOPLIST stoplistName = id (
+        FROM ((databaseName = id DOT)? sourceStoplistName = id | SYSTEM STOPLIST)
+    )? (AUTHORIZATION ownerName = id)?
     ;
 
 // https://docs.microsoft.com/en-us/sql/t-sql/statements/alter-login-transact-sql
-alter_login_sql_server
-    : ALTER LOGIN login_name = id_ (
+alterLoginSqlServer
+    : ALTER LOGIN loginName = id (
         (ENABLE | DISABLE)?
         | WITH (
-            (PASSWORD EQ ( password = STRING | password_hash = HEX HASHED)) (
+            (PASSWORD EQ ( password = STRING | passwordHash = HEX HASHED)) (
                 MUST_CHANGE
                 | UNLOCK
             )*
-        )? (OLD_PASSWORD EQ old_password = STRING (MUST_CHANGE | UNLOCK)*)? (
-            DEFAULT_DATABASE EQ default_database = id_
-        )? (DEFAULT_LANGUAGE EQ default_laguage = id_)? (NAME EQ login_name = id_)? (
+        )? (OLD_PASSWORD EQ oldPassword = STRING (MUST_CHANGE | UNLOCK)*)? (
+            DEFAULT_DATABASE EQ defaultDatabase = id
+        )? (DEFAULT_LANGUAGE EQ defaultLaguage = id)? (NAME EQ loginName = id)? (
             CHECK_POLICY EQ (ON | OFF)
-        )? (CHECK_EXPIRATION EQ (ON | OFF))? (CREDENTIAL EQ credential_name = id_)? (
+        )? (CHECK_EXPIRATION EQ (ON | OFF))? (CREDENTIAL EQ credentialName = id)? (
             NO CREDENTIAL
         )?
-        | (ADD | DROP) CREDENTIAL credential_name = id_
+        | (ADD | DROP) CREDENTIAL credentialName = id
     )
     ;
 
 // https://docs.microsoft.com/en-us/sql/t-sql/statements/create-login-transact-sql
-create_login_sql_server
-    : CREATE LOGIN login_name = id_ (
+createLoginSqlServer
+    : CREATE LOGIN loginName = id (
         WITH (
-            (PASSWORD EQ ( password = STRING | password_hash = HEX HASHED)) (
+            (PASSWORD EQ ( password = STRING | passwordHash = HEX HASHED)) (
                 MUST_CHANGE
                 | UNLOCK
             )*
-        )? (COMMA? SID EQ sid = HEX)? (COMMA? DEFAULT_DATABASE EQ default_database = id_)? (
-            COMMA? DEFAULT_LANGUAGE EQ default_laguage = id_
+        )? (COMMA? SID EQ sid = HEX)? (COMMA? DEFAULT_DATABASE EQ defaultDatabase = id)? (
+            COMMA? DEFAULT_LANGUAGE EQ defaultLaguage = id
         )? (COMMA? CHECK_EXPIRATION EQ (ON | OFF))? (COMMA? CHECK_POLICY EQ (ON | OFF))? (
-            COMMA? CREDENTIAL EQ credential_name = id_
+            COMMA? CREDENTIAL EQ credentialName = id
         )?
         | (
             FROM (
                 WINDOWS (
-                    WITH (COMMA? DEFAULT_DATABASE EQ default_database = id_)? (
-                        COMMA? DEFAULT_LANGUAGE EQ default_language = STRING
+                    WITH (COMMA? DEFAULT_DATABASE EQ defaultDatabase = id)? (
+                        COMMA? DEFAULT_LANGUAGE EQ defaultLanguage = STRING
                     )?
                 )
-                | CERTIFICATE certname = id_
-                | ASYMMETRIC KEY asym_key_name = id_
+                | CERTIFICATE certname = id
+                | ASYMMETRIC KEY asymKeyName = id
             )
         )
     )
     ;
 
-alter_login_azure_sql
-    : ALTER LOGIN login_name = id_ (
+alterLoginAzureSql
+    : ALTER LOGIN loginName = id (
         (ENABLE | DISABLE)?
         | WITH (
-            PASSWORD EQ password = STRING (OLD_PASSWORD EQ old_password = STRING)?
-            | NAME EQ login_name = id_
+            PASSWORD EQ password = STRING (OLD_PASSWORD EQ oldPassword = STRING)?
+            | NAME EQ loginName = id
         )
     )
     ;
 
-create_login_azure_sql
-    : CREATE LOGIN login_name = id_ WITH PASSWORD EQ STRING (SID EQ sid = HEX)?
+createLoginAzureSql
+    : CREATE LOGIN loginName = id WITH PASSWORD EQ STRING (SID EQ sid = HEX)?
     ;
 
-alter_login_azure_sql_dw_and_pdw
-    : ALTER LOGIN login_name = id_ (
+alterLoginAzureSqlDwAndPdw
+    : ALTER LOGIN loginName = id (
         (ENABLE | DISABLE)?
         | WITH (
             PASSWORD EQ password = STRING (
-                OLD_PASSWORD EQ old_password = STRING (MUST_CHANGE | UNLOCK)*
+                OLD_PASSWORD EQ oldPassword = STRING (MUST_CHANGE | UNLOCK)*
             )?
-            | NAME EQ login_name = id_
+            | NAME EQ loginName = id
         )
     )
     ;
 
-create_login_pdw
-    : CREATE LOGIN loginName = id_ (
+createLoginPdw
+    : CREATE LOGIN loginName = id (
         WITH (PASSWORD EQ password = STRING (MUST_CHANGE)? (CHECK_POLICY EQ (ON | OFF)?)?)
         | FROM WINDOWS
     )
     ;
 
 // https://docs.microsoft.com/en-us/sql/t-sql/statements/alter-master-key-transact-sql
-alter_master_key_sql_server
+alterMasterKeySqlServer
     : ALTER MASTER KEY (
         (FORCE)? REGENERATE WITH ENCRYPTION BY PASSWORD EQ password = STRING
         | (ADD | DROP) ENCRYPTION BY (
             SERVICE MASTER KEY
-            | PASSWORD EQ encryption_password = STRING
+            | PASSWORD EQ encryptionPassword = STRING
         )
     )
     ;
 
 // https://docs.microsoft.com/en-us/sql/t-sql/statements/create-master-key-transact-sql
-create_master_key_sql_server
+createMasterKeySqlServer
     : CREATE MASTER KEY ENCRYPTION BY PASSWORD EQ password = STRING
     ;
 
-alter_master_key_azure_sql
+alterMasterKeyAzureSql
     : ALTER MASTER KEY (
         (FORCE)? REGENERATE WITH ENCRYPTION BY PASSWORD EQ password = STRING
-        | ADD ENCRYPTION BY (SERVICE MASTER KEY | PASSWORD EQ encryption_password = STRING)
-        | DROP ENCRYPTION BY PASSWORD EQ encryption_password = STRING
+        | ADD ENCRYPTION BY (SERVICE MASTER KEY | PASSWORD EQ encryptionPassword = STRING)
+        | DROP ENCRYPTION BY PASSWORD EQ encryptionPassword = STRING
     )
     ;
 
-create_master_key_azure_sql
+createMasterKeyAzureSql
     : CREATE MASTER KEY (ENCRYPTION BY PASSWORD EQ password = STRING)?
     ;
 
 // https://docs.microsoft.com/en-us/sql/t-sql/statements/alter-message-type-transact-sql
-alter_message_type
-    : ALTER MESSAGE TYPE message_type_name = id_ VALIDATION EQ (
+alterMessageType
+    : ALTER MESSAGE TYPE messageTypeName = id VALIDATION EQ (
         NONE
         | EMPTY
         | WELL_FORMED_XML
-        | VALID_XML WITH SCHEMA COLLECTION schema_collection_name = id_
+        | VALID_XML WITH SCHEMA COLLECTION schemaCollectionName = id
     )
     ;
 
 // https://docs.microsoft.com/en-us/sql/t-sql/statements/alter-partition-function-transact-sql
-alter_partition_function
-    : ALTER PARTITION FUNCTION partition_function_name = id_ LPAREN RPAREN (SPLIT | MERGE) RANGE LPAREN INT RPAREN
+alterPartitionFunction
+    : ALTER PARTITION FUNCTION partitionFunctionName = id LPAREN RPAREN (SPLIT | MERGE) RANGE LPAREN INT RPAREN
     ;
 
 // https://docs.microsoft.com/en-us/sql/t-sql/statements/alter-partition-scheme-transact-sql
-alter_partition_scheme
-    : ALTER PARTITION SCHEME partition_scheme_name = id_ NEXT USED (file_group_name = id_)?
+alterPartitionScheme
+    : ALTER PARTITION SCHEME partitionSchemeName = id NEXT USED (fileGroupName = id)?
     ;
 
 // https://docs.microsoft.com/en-us/sql/t-sql/statements/alter-remote-service-binding-transact-sql
-alter_remote_service_binding
-    : ALTER REMOTE SERVICE BINDING binding_name = id_ WITH (USER EQ user_name = id_)? (
+alterRemoteServiceBinding
+    : ALTER REMOTE SERVICE BINDING bindingName = id WITH (USER EQ userName = id)? (
         COMMA ANONYMOUS EQ (ON | OFF)
     )?
     ;
 
 // https://docs.microsoft.com/en-us/sql/t-sql/statements/create-remote-service-binding-transact-sql
-create_remote_service_binding
-    : CREATE REMOTE SERVICE BINDING binding_name = id_ (AUTHORIZATION owner_name = id_)? TO SERVICE remote_service_name = STRING WITH (
-        USER EQ user_name = id_
+createRemoteServiceBinding
+    : CREATE REMOTE SERVICE BINDING bindingName = id (AUTHORIZATION ownerName = id)? TO SERVICE remoteServiceName = STRING WITH (
+        USER EQ userName = id
     )? (COMMA ANONYMOUS EQ (ON | OFF))?
     ;
 
 // https://docs.microsoft.com/en-us/sql/t-sql/statements/create-resource-pool-transact-sql
-create_resource_pool
-    : CREATE RESOURCE POOL pool_name = id_ (
+createResourcePool
+    : CREATE RESOURCE POOL poolName = id (
         WITH LPAREN (COMMA? MIN_CPU_PERCENT EQ INT)? (
             COMMA? MAX_CPU_PERCENT EQ INT
         )? (COMMA? CAP_CPU_PERCENT EQ INT)? (
             COMMA? AFFINITY SCHEDULER EQ (
                 AUTO
                 | LPAREN (COMMA? (INT | INT TO INT))+ RPAREN
                 | NUMANODE EQ LPAREN (COMMA? (INT | INT TO INT))+ RPAREN
@@ -1541,197 +1540,197 @@
         )? (COMMA? MIN_MEMORY_PERCENT EQ INT)? (COMMA? MAX_MEMORY_PERCENT EQ INT)? (
             COMMA? MIN_IOPS_PER_VOLUME EQ INT
         )? (COMMA? MAX_IOPS_PER_VOLUME EQ INT)? RPAREN
     )?
     ;
 
 // https://docs.microsoft.com/en-us/sql/t-sql/statements/alter-resource-governor-transact-sql
-alter_resource_governor
+alterResourceGovernor
     : ALTER RESOURCE GOVERNOR (
         (DISABLE | RECONFIGURE)
         | WITH LPAREN CLASSIFIER_FUNCTION EQ (
-            schema_name = id_ DOT function_name = id_
+            schemaName = id DOT functionName = id
             | NULL_
         ) RPAREN
         | RESET STATISTICS
-        | WITH LPAREN MAX_OUTSTANDING_IO_PER_VOLUME EQ max_outstanding_io_per_volume = INT RPAREN
+        | WITH LPAREN MAX_OUTSTANDING_IO_PER_VOLUME EQ maxOutstandingIoPerVolume = INT RPAREN
     )
     ;
 
 // https://learn.microsoft.com/en-us/sql/t-sql/statements/alter-database-audit-specification-transact-sql?view=sql-server-ver16
-alter_database_audit_specification
-    : ALTER DATABASE AUDIT SPECIFICATION audit_specification_name = id_ (
-        FOR SERVER AUDIT audit_name = id_
-    )? (audit_action_spec_group (COMMA audit_action_spec_group)*)? (
+alterDatabaseAuditSpecification
+    : ALTER DATABASE AUDIT SPECIFICATION auditSpecificationName = id (
+        FOR SERVER AUDIT auditName = id
+    )? (auditActionSpecGroup (COMMA auditActionSpecGroup)*)? (
         WITH LPAREN STATE EQ (ON | OFF) RPAREN
     )?
     ;
 
-audit_action_spec_group
-    : (ADD | DROP) LPAREN (audit_action_specification | audit_action_group_name = id_) RPAREN
+auditActionSpecGroup
+    : (ADD | DROP) LPAREN (auditActionSpecification | auditActionGroupName = id) RPAREN
     ;
 
-audit_action_specification
-    : action_specification (COMMA action_specification)* ON (audit_class_name COLON COLON)? audit_securable BY principal_id (
-        COMMA principal_id
+auditActionSpecification
+    : actionSpecification (COMMA actionSpecification)* ON (auditClassName COLON COLON)? auditSecurable BY principalId (
+        COMMA principalId
     )*
     ;
 
-action_specification
+actionSpecification
     : SELECT
     | INSERT
     | UPDATE
     | DELETE
     | EXECUTE
     | RECEIVE
     | REFERENCES
     ;
 
-audit_class_name
+auditClassName
     : OBJECT
     | SCHEMA
     | TABLE
     ;
 
-audit_securable
-    : ((id_ DOT)? id_ DOT)? id_
+auditSecurable
+    : ((id DOT)? id DOT)? id
     ;
 
 // https://docs.microsoft.com/en-us/sql/t-sql/statements/alter-role-transact-sql
-alter_db_role
-    : ALTER ROLE role_name = id_ (
-        (ADD | DROP) MEMBER database_principal = id_
-        | WITH NAME EQ new_role_name = id_
+alterDbRole
+    : ALTER ROLE roleName = id (
+        (ADD | DROP) MEMBER databasePrincipal = id
+        | WITH NAME EQ newRoleName = id
     )
     ;
 
 // https://learn.microsoft.com/en-us/sql/t-sql/statements/create-database-audit-specification-transact-sql?view=sql-server-ver16
-create_database_audit_specification
-    : CREATE DATABASE AUDIT SPECIFICATION audit_specification_name = id_ (
-        FOR SERVER AUDIT audit_name = id_
-    )? (audit_action_spec_group (COMMA audit_action_spec_group)*)? (
+createDatabaseAuditSpecification
+    : CREATE DATABASE AUDIT SPECIFICATION auditSpecificationName = id (
+        FOR SERVER AUDIT auditName = id
+    )? (auditActionSpecGroup (COMMA auditActionSpecGroup)*)? (
         WITH LPAREN STATE EQ (ON | OFF) RPAREN
     )?
     ;
 
 // https://docs.microsoft.com/en-us/sql/t-sql/statements/create-role-transact-sql
-create_db_role
-    : CREATE ROLE role_name = id_ (AUTHORIZATION owner_name = id_)?
+createDbRole
+    : CREATE ROLE roleName = id (AUTHORIZATION ownerName = id)?
     ;
 
 // https://docs.microsoft.com/en-us/sql/t-sql/statements/create-route-transact-sql
-create_route
-    : CREATE ROUTE route_name = id_ (AUTHORIZATION owner_name = id_)? WITH (
-        COMMA? SERVICE_NAME EQ route_service_name = STRING
-    )? (COMMA? BROKER_INSTANCE EQ broker_instance_identifier = STRING)? (
+createRoute
+    : CREATE ROUTE routeName = id (AUTHORIZATION ownerName = id)? WITH (
+        COMMA? SERVICE_NAME EQ routeServiceName = STRING
+    )? (COMMA? BROKER_INSTANCE EQ brokerInstanceIdentifier = STRING)? (
         COMMA? LIFETIME EQ INT
     )? COMMA? ADDRESS EQ STRING (COMMA MIRROR_ADDRESS EQ STRING)?
     ;
 
 // https://docs.microsoft.com/en-us/sql/t-sql/statements/create-rule-transact-sql
-create_rule
-    : CREATE RULE (schema_name = id_ DOT)? rule_name = id_ AS search_condition
+createRule
+    : CREATE RULE (schemaName = id DOT)? ruleName = id AS searchCondition
     ;
 
 // https://docs.microsoft.com/en-us/sql/t-sql/statements/alter-schema-transact-sql
-alter_schema_sql
-    : ALTER SCHEMA schema_name = id_ TRANSFER (
+alterSchemaSql
+    : ALTER SCHEMA schemaName = id TRANSFER (
         (OBJECT | TYPE | XML SCHEMA COLLECTION) DOUBLE_COLON
-    )? id_ (DOT id_)?
+    )? id (DOT id)?
     ;
 
 // https://docs.microsoft.com/en-us/sql/t-sql/statements/create-schema-transact-sql
-create_schema
+createSchema
     : CREATE SCHEMA (
-        schema_name = id_
-        | AUTHORIZATION owner_name = id_
-        | schema_name = id_ AUTHORIZATION owner_name = id_
+        schemaName = id
+        | AUTHORIZATION ownerName = id
+        | schemaName = id AUTHORIZATION ownerName = id
     ) (
-        create_table
-        | create_view
-        | (GRANT | DENY) (SELECT | INSERT | DELETE | UPDATE) ON (SCHEMA DOUBLE_COLON)? object_name = id_ TO owner_name = id_
-        | REVOKE (SELECT | INSERT | DELETE | UPDATE) ON (SCHEMA DOUBLE_COLON)? object_name = id_ FROM owner_name = id_
+        createTable
+        | createView
+        | (GRANT | DENY) (SELECT | INSERT | DELETE | UPDATE) ON (SCHEMA DOUBLE_COLON)? objectName = id TO ownerName = id
+        | REVOKE (SELECT | INSERT | DELETE | UPDATE) ON (SCHEMA DOUBLE_COLON)? objectName = id FROM ownerName = id
     )*
     ;
 
-create_schema_azure_sql_dw_and_pdw
-    : CREATE SCHEMA schema_name = id_ (AUTHORIZATION owner_name = id_)?
+createSchemaAzureSqlDwAndPdw
+    : CREATE SCHEMA schemaName = id (AUTHORIZATION ownerName = id)?
     ;
 
-alter_schema_azure_sql_dw_and_pdw
-    : ALTER SCHEMA schema_name = id_ TRANSFER (OBJECT DOUBLE_COLON)? id_ (DOT ID)?
+alterSchemaAzureSqlDwAndPdw
+    : ALTER SCHEMA schemaName = id TRANSFER (OBJECT DOUBLE_COLON)? id (DOT ID)?
     ;
 
 // https://docs.microsoft.com/en-us/sql/t-sql/statements/create-search-property-list-transact-sql
-create_search_property_list
-    : CREATE SEARCH PROPERTY LIST new_list_name = id_ (
-        FROM (database_name = id_ DOT)? source_list_name = id_
-    )? (AUTHORIZATION owner_name = id_)?
+createSearchPropertyList
+    : CREATE SEARCH PROPERTY LIST newListName = id (
+        FROM (databaseName = id DOT)? sourceListName = id
+    )? (AUTHORIZATION ownerName = id)?
     ;
 
 // https://docs.microsoft.com/en-us/sql/t-sql/statements/create-security-policy-transact-sql
-create_security_policy
-    : CREATE SECURITY POLICY (schema_name = id_ DOT)? security_policy_name = id_ (
-        COMMA? ADD (FILTER | BLOCK)? PREDICATE tvf_schema_name = id_ DOT security_predicate_function_name = id_ LPAREN (
-            COMMA? column_name_or_arguments = id_
-        )+ RPAREN ON table_schema_name = id_ DOT name = id_ (
+createSecurityPolicy
+    : CREATE SECURITY POLICY (schemaName = id DOT)? securityPolicyName = id (
+        COMMA? ADD (FILTER | BLOCK)? PREDICATE tvfSchemaName = id DOT securityPredicateFunctionName = id LPAREN (
+            COMMA? columnNameOrArguments = id
+        )+ RPAREN ON tableSchemaName = id DOT name = id (
             COMMA? AFTER (INSERT | UPDATE)
             | COMMA? BEFORE (UPDATE | DELETE)
         )*
     )+ (WITH LPAREN STATE EQ (ON | OFF) (SCHEMABINDING (ON | OFF))? RPAREN)? (
         NOT FOR REPLICATION
     )?
     ;
 
 // https://docs.microsoft.com/en-us/sql/t-sql/statements/alter-sequence-transact-sql
-alter_sequence
-    : ALTER SEQUENCE (schema_name = id_ DOT)? sequence_name = id_ (RESTART (WITH INT)?)? (
-        INCREMENT BY sequnce_increment = INT
+alterSequence
+    : ALTER SEQUENCE (schemaName = id DOT)? sequenceName = id (RESTART (WITH INT)?)? (
+        INCREMENT BY sequnceIncrement = INT
     )? (MINVALUE INT | NO MINVALUE)? (MAXVALUE INT | NO MAXVALUE)? (CYCLE | NO CYCLE)? (
         CACHE INT
         | NO CACHE
     )?
     ;
 
 // https://docs.microsoft.com/en-us/sql/t-sql/statements/create-sequence-transact-sql
-create_sequence
-    : CREATE SEQUENCE (schema_name = id_ DOT)? sequence_name = id_ (AS data_type)? (
+createSequence
+    : CREATE SEQUENCE (schemaName = id DOT)? sequenceName = id (AS dataType)? (
         START WITH INT
     )? (INCREMENT BY MINUS? INT)? (MINVALUE (MINUS? INT)? | NO MINVALUE)? (
         MAXVALUE (MINUS? INT)?
         | NO MAXVALUE
     )? (CYCLE | NO CYCLE)? (CACHE INT? | NO CACHE)?
     ;
 
 // https://docs.microsoft.com/en-us/sql/t-sql/statements/alter-server-audit-transact-sql
-alter_server_audit
-    : ALTER SERVER AUDIT audit_name = id_ (
+alterServerAudit
+    : ALTER SERVER AUDIT auditName = id (
         (
             TO (
                 FILE (
                     LPAREN (
                         COMMA? FILEPATH EQ filepath = STRING
                         | COMMA? MAXSIZE EQ ( INT (MB | GB | TB) | UNLIMITED)
-                        | COMMA? MAX_ROLLOVER_FILES EQ max_rollover_files = (INT | UNLIMITED)
-                        | COMMA? MAX_FILES EQ max_files = INT
+                        | COMMA? MAX_ROLLOVER_FILES EQ maxRolloverFiles = (INT | UNLIMITED)
+                        | COMMA? MAX_FILES EQ maxFiles = INT
                         | COMMA? RESERVE_DISK_SPACE EQ (ON | OFF)
                     )* RPAREN
                 )
                 | APPLICATION_LOG
                 | SECURITY_LOG
             )
         )? (
             WITH LPAREN (
-                COMMA? QUEUE_DELAY EQ queue_delay = INT
+                COMMA? QUEUE_DELAY EQ queueDelay = INT
                 | COMMA? ON_FAILURE EQ (CONTINUE | SHUTDOWN | FAIL_OPERATION)
                 | COMMA? STATE EQ (ON | OFF)
             )* RPAREN
         )? (
             WHERE (
-                COMMA? (NOT?) event_field_name = id_ (
+                COMMA? (NOT?) eventFieldName = id (
                     EQ
                     | (LT GT)
                     | (BANG EQ)
                     | GT
                     | (GT EQ)
                     | LT
                     | LT EQ
@@ -1744,45 +1743,45 @@
                     | (GT EQ)
                     | LT
                     | LT EQ
                 ) (INT | STRING)
             )
         )?
         | REMOVE WHERE
-        | MODIFY NAME EQ new_audit_name = id_
+        | MODIFY NAME EQ newAuditName = id
     )
     ;
 
 // https://docs.microsoft.com/en-us/sql/t-sql/statements/create-server-audit-transact-sql
-create_server_audit
-    : CREATE SERVER AUDIT audit_name = id_ (
+createServerAudit
+    : CREATE SERVER AUDIT auditName = id (
         (
             TO (
                 FILE (
                     LPAREN (
                         COMMA? FILEPATH EQ filepath = STRING
                         | COMMA? MAXSIZE EQ ( INT (MB | GB | TB) | UNLIMITED)
-                        | COMMA? MAX_ROLLOVER_FILES EQ max_rollover_files = (INT | UNLIMITED)
-                        | COMMA? MAX_FILES EQ max_files = INT
+                        | COMMA? MAX_ROLLOVER_FILES EQ maxRolloverFiles = (INT | UNLIMITED)
+                        | COMMA? MAX_FILES EQ maxFiles = INT
                         | COMMA? RESERVE_DISK_SPACE EQ (ON | OFF)
                     )* RPAREN
                 )
                 | APPLICATION_LOG
                 | SECURITY_LOG
             )
         )? (
             WITH LPAREN (
-                COMMA? QUEUE_DELAY EQ queue_delay = INT
+                COMMA? QUEUE_DELAY EQ queueDelay = INT
                 | COMMA? ON_FAILURE EQ (CONTINUE | SHUTDOWN | FAIL_OPERATION)
                 | COMMA? STATE EQ (ON | OFF)
-                | COMMA? AUDIT_GUID EQ audit_guid = id_
+                | COMMA? AUDIT_GUID EQ auditGuid = id
             )* RPAREN
         )? (
             WHERE (
-                COMMA? (NOT?) event_field_name = id_ (
+                COMMA? (NOT?) eventFieldName = id (
                     EQ
                     | (LT GT)
                     | (BANG EQ)
                     | GT
                     | (GT EQ)
                     | LT
                     | LT EQ
@@ -1795,40 +1794,40 @@
                     | (GT EQ)
                     | LT
                     | LT EQ
                 ) (INT | STRING)
             )
         )?
         | REMOVE WHERE
-        | MODIFY NAME EQ new_audit_name = id_
+        | MODIFY NAME EQ newAuditName = id
     )
     ;
 
 // https://docs.microsoft.com/en-us/sql/t-sql/statements/alter-server-audit-specification-transact-sql
 
-alter_server_audit_specification
-    : ALTER SERVER AUDIT SPECIFICATION audit_specification_name = id_ (
-        FOR SERVER AUDIT audit_name = id_
-    )? ((ADD | DROP) LPAREN audit_action_group_name = id_ RPAREN)* (
+alterServerAuditSpecification
+    : ALTER SERVER AUDIT SPECIFICATION auditSpecificationName = id (
+        FOR SERVER AUDIT auditName = id
+    )? ((ADD | DROP) LPAREN auditActionGroupName = id RPAREN)* (
         WITH LPAREN STATE EQ (ON | OFF) RPAREN
     )?
     ;
 
 // https://docs.microsoft.com/en-us/sql/t-sql/statements/create-server-audit-specification-transact-sql
-create_server_audit_specification
-    : CREATE SERVER AUDIT SPECIFICATION audit_specification_name = id_ (
-        FOR SERVER AUDIT audit_name = id_
-    )? (ADD LPAREN audit_action_group_name = id_ RPAREN)* (
+createServerAuditSpecification
+    : CREATE SERVER AUDIT SPECIFICATION auditSpecificationName = id (
+        FOR SERVER AUDIT auditName = id
+    )? (ADD LPAREN auditActionGroupName = id RPAREN)* (
         WITH LPAREN STATE EQ (ON | OFF) RPAREN
     )?
     ;
 
 // https://docs.microsoft.com/en-us/sql/t-sql/statements/alter-server-configuration-transact-sql
 
-alter_server_configuration
+alterServerConfiguration
     : ALTER SERVER CONFIGURATION SET (
         (
             PROCESS AFFINITY (
                 CPU EQ (AUTO | (COMMA? INT | COMMA? INT TO INT)+)
                 | NUMANODE EQ ( COMMA? INT | COMMA? INT TO INT)+
             )
             | DIAGNOSTICS LOG (
@@ -1853,1400 +1852,1400 @@
             )
             | SET SOFTNUMA (ON | OFF)
         )
     )
     ;
 
 // https://docs.microsoft.com/en-us/sql/t-sql/statements/alter-server-role-transact-sql
-alter_server_role
-    : ALTER SERVER ROLE server_role_name = id_ (
-        (ADD | DROP) MEMBER server_principal = id_
-        | WITH NAME EQ new_server_role_name = id_
+alterServerRole
+    : ALTER SERVER ROLE serverRoleName = id (
+        (ADD | DROP) MEMBER serverPrincipal = id
+        | WITH NAME EQ newServerRoleName = id
     )
     ;
 
 // https://docs.microsoft.com/en-us/sql/t-sql/statements/create-server-role-transact-sql
-create_server_role
-    : CREATE SERVER ROLE server_role = id_ (AUTHORIZATION server_principal = id_)?
+createServerRole
+    : CREATE SERVER ROLE serverRole = id (AUTHORIZATION serverPrincipal = id)?
     ;
 
-alter_server_role_pdw
-    : ALTER SERVER ROLE server_role_name = id_ (ADD | DROP) MEMBER login = id_
+alterServerRolePdw
+    : ALTER SERVER ROLE serverRoleName = id (ADD | DROP) MEMBER login = id
     ;
 
 // https://docs.microsoft.com/en-us/sql/t-sql/statements/alter-service-transact-sql
-alter_service
-    : ALTER SERVICE modified_service_name = id_ (
-        ON QUEUE (schema_name = id_ DOT)? queue_name = id_
-    )? (LPAREN opt_arg_clause (COMMA opt_arg_clause)* RPAREN)?
+alterService
+    : ALTER SERVICE modifiedServiceName = id (
+        ON QUEUE (schemaName = id DOT)? queueName = id
+    )? (LPAREN optArgClause (COMMA optArgClause)* RPAREN)?
     ;
 
-opt_arg_clause
-    : (ADD | DROP) CONTRACT modified_contract_name = id_
+optArgClause
+    : (ADD | DROP) CONTRACT modifiedContractName = id
     ;
 
 // https://docs.microsoft.com/en-us/sql/t-sql/statements/create-service-transact-sql
-create_service
-    : CREATE SERVICE create_service_name = id_ (AUTHORIZATION owner_name = id_)? ON QUEUE (
-        schema_name = id_ DOT
-    )? queue_name = id_ (LPAREN (COMMA? (id_ | DEFAULT))+ RPAREN)?
+createService
+    : CREATE SERVICE createServiceName = id (AUTHORIZATION ownerName = id)? ON QUEUE (
+        schemaName = id DOT
+    )? queueName = id (LPAREN (COMMA? (id | DEFAULT))+ RPAREN)?
     ;
 
 // https://docs.microsoft.com/en-us/sql/t-sql/statements/alter-service-master-key-transact-sql
 
-alter_service_master_key
+alterServiceMasterKey
     : ALTER SERVICE MASTER KEY (
         FORCE? REGENERATE
         | (
             WITH (
-                OLD_ACCOUNT EQ acold_account_name = STRING COMMA OLD_PASSWORD EQ old_password = STRING
-                | NEW_ACCOUNT EQ new_account_name = STRING COMMA NEW_PASSWORD EQ new_password = STRING
+                OLD_ACCOUNT EQ acoldAccountName = STRING COMMA OLD_PASSWORD EQ oldPassword = STRING
+                | NEW_ACCOUNT EQ newAccountName = STRING COMMA NEW_PASSWORD EQ newPassword = STRING
             )?
         )
     )
     ;
 
 // https://docs.microsoft.com/en-us/sql/t-sql/statements/alter-symmetric-key-transact-sql
 
-alter_symmetric_key
-    : ALTER SYMMETRIC KEY key_name = id_ (
+alterSymmetricKey
+    : ALTER SYMMETRIC KEY keyName = id (
         (ADD | DROP) ENCRYPTION BY (
-            CERTIFICATE certificate_name = id_
+            CERTIFICATE certificateName = id
             | PASSWORD EQ password = STRING
-            | SYMMETRIC KEY symmetric_key_name = id_
-            | ASYMMETRIC KEY Asym_key_name = id_
+            | SYMMETRIC KEY symmetricKeyName = id
+            | ASYMMETRIC KEY AsymKeyName = id
         )
     )
     ;
 
 // https://docs.microsoft.com/en-us/sql/t-sql/statements/create-synonym-transact-sql
-create_synonym
-    : CREATE SYNONYM (schema_name_1 = id_ DOT)? synonym_name = id_ FOR (
-        (server_name = id_ DOT)? (database_name = id_ DOT)? (schema_name_2 = id_ DOT)? object_name = id_
-        | (database_or_schema2 = id_ DOT)? (schema_id_2_or_object_name = id_ DOT)?
+createSynonym
+    : CREATE SYNONYM (schemaName_1 = id DOT)? synonymName = id FOR (
+        (serverName = id DOT)? (databaseName = id DOT)? (schemaName_2 = id DOT)? objectName = id
+        | (databaseOrSchema2 = id DOT)? (schemaId2_orObjectName = id DOT)?
     )
     ;
 
 // https://docs.microsoft.com/en-us/sql/t-sql/statements/alter-user-transact-sql
-alter_user
-    : ALTER USER username = id_ WITH (
-        COMMA? NAME EQ newusername = id_
-        | COMMA? DEFAULT_SCHEMA EQ ( schema_name = id_ | NULL_)
-        | COMMA? LOGIN EQ loginame = id_
+alterUser
+    : ALTER USER username = id WITH (
+        COMMA? NAME EQ newusername = id
+        | COMMA? DEFAULT_SCHEMA EQ ( schemaName = id | NULL_)
+        | COMMA? LOGIN EQ loginame = id
         | COMMA? PASSWORD EQ STRING (OLD_PASSWORD EQ STRING)+
-        | COMMA? DEFAULT_LANGUAGE EQ (NONE | lcid = INT | language_name_or_alias = id_)
+        | COMMA? DEFAULT_LANGUAGE EQ (NONE | lcid = INT | languageNameOrAlias = id)
         | COMMA? ALLOW_ENCRYPTED_VALUE_MODIFICATIONS EQ (ON | OFF)
     )+
     ;
 
 // https://docs.microsoft.com/en-us/sql/t-sql/statements/create-user-transact-sql
-create_user
-    : CREATE USER user_name = id_ ((FOR | FROM) LOGIN login_name = id_)? (
+createUser
+    : CREATE USER userName = id ((FOR | FROM) LOGIN loginName = id)? (
         WITH (
-            COMMA? DEFAULT_SCHEMA EQ schema_name = id_
+            COMMA? DEFAULT_SCHEMA EQ schemaName = id
             | COMMA? ALLOW_ENCRYPTED_VALUE_MODIFICATIONS EQ (ON | OFF)
         )*
     )?
     | CREATE USER (
-        windows_principal = id_ (
+        windowsPrincipal = id (
             WITH (
-                COMMA? DEFAULT_SCHEMA EQ schema_name = id_
-                | COMMA? DEFAULT_LANGUAGE EQ (NONE | INT | language_name_or_alias = id_)
+                COMMA? DEFAULT_SCHEMA EQ schemaName = id
+                | COMMA? DEFAULT_LANGUAGE EQ (NONE | INT | languageNameOrAlias = id)
                 | COMMA? SID EQ HEX
                 | COMMA? ALLOW_ENCRYPTED_VALUE_MODIFICATIONS EQ (ON | OFF)
             )*
         )?
-        | user_name = id_ WITH PASSWORD EQ password = STRING (
-            COMMA? DEFAULT_SCHEMA EQ schema_name = id_
-            | COMMA? DEFAULT_LANGUAGE EQ (NONE | INT | language_name_or_alias = id_)
+        | userName = id WITH PASSWORD EQ password = STRING (
+            COMMA? DEFAULT_SCHEMA EQ schemaName = id
+            | COMMA? DEFAULT_LANGUAGE EQ (NONE | INT | languageNameOrAlias = id)
             | COMMA? SID EQ HEX
             | COMMA? ALLOW_ENCRYPTED_VALUE_MODIFICATIONS EQ (ON | OFF)
         )*
-        | Azure_Active_Directory_principal = id_ FROM EXTERNAL PROVIDER
+        | Azure_Active_DirectoryPrincipal = id FROM EXTERNAL PROVIDER
     )
-    | CREATE USER user_name = id_ (
+    | CREATE USER userName = id (
         WITHOUT LOGIN (
-            COMMA? DEFAULT_SCHEMA EQ schema_name = id_
+            COMMA? DEFAULT_SCHEMA EQ schemaName = id
             | COMMA? ALLOW_ENCRYPTED_VALUE_MODIFICATIONS EQ (ON | OFF)
         )*
-        | (FOR | FROM) CERTIFICATE cert_name = id_
-        | (FOR | FROM) ASYMMETRIC KEY asym_key_name = id_
+        | (FOR | FROM) CERTIFICATE certName = id
+        | (FOR | FROM) ASYMMETRIC KEY asymKeyName = id
     )
-    | CREATE USER user_name = id_
+    | CREATE USER userName = id
     ;
 
-create_user_azure_sql_dw
-    : CREATE USER user_name = id_ ((FOR | FROM) LOGIN login_name = id_ | WITHOUT LOGIN)? (
-        WITH DEFAULT_SCHEMA EQ schema_name = id_
+createUserAzureSqlDw
+    : CREATE USER userName = id ((FOR | FROM) LOGIN loginName = id | WITHOUT LOGIN)? (
+        WITH DEFAULT_SCHEMA EQ schemaName = id
     )?
-    | CREATE USER Azure_Active_Directory_principal = id_ FROM EXTERNAL PROVIDER (
-        WITH DEFAULT_SCHEMA EQ schema_name = id_
+    | CREATE USER Azure_Active_DirectoryPrincipal = id FROM EXTERNAL PROVIDER (
+        WITH DEFAULT_SCHEMA EQ schemaName = id
     )?
     ;
 
-alter_user_azure_sql
-    : ALTER USER username = id_ WITH (
-        COMMA? NAME EQ newusername = id_
-        | COMMA? DEFAULT_SCHEMA EQ schema_name = id_
-        | COMMA? LOGIN EQ loginame = id_
+alterUserAzureSql
+    : ALTER USER username = id WITH (
+        COMMA? NAME EQ newusername = id
+        | COMMA? DEFAULT_SCHEMA EQ schemaName = id
+        | COMMA? LOGIN EQ loginame = id
         | COMMA? ALLOW_ENCRYPTED_VALUE_MODIFICATIONS EQ (ON | OFF)
     )+
     ;
 
 // https://docs.microsoft.com/en-us/sql/t-sql/statements/alter-workload-group-transact-sql
 
-alter_workload_group
-    : ALTER WORKLOAD GROUP (workload_group_group_name = id_ | DEFAULT_DOUBLE_QUOTE) (
+alterWorkloadGroup
+    : ALTER WORKLOAD GROUP (workloadGroupGroupName = id | DEFAULT_DOUBLE_QUOTE) (
         WITH LPAREN (
             IMPORTANCE EQ (LOW | MEDIUM | HIGH)
-            | COMMA? REQUEST_MAX_MEMORY_GRANT_PERCENT EQ request_max_memory_grant = INT
-            | COMMA? REQUEST_MAX_CPU_TIME_SEC EQ request_max_cpu_time_sec = INT
-            | REQUEST_MEMORY_GRANT_TIMEOUT_SEC EQ request_memory_grant_timeout_sec = INT
-            | MAX_DOP EQ max_dop = INT
-            | GROUP_MAX_REQUESTS EQ group_max_requests = INT
+            | COMMA? REQUEST_MAX_MEMORY_GRANT_PERCENT EQ requestMaxMemoryGrant = INT
+            | COMMA? REQUEST_MAX_CPU_TIME_SEC EQ requestMaxCpuTimeSec = INT
+            | REQUEST_MEMORY_GRANT_TIMEOUT_SEC EQ requestMemoryGrantTimeoutSec = INT
+            | MAX_DOP EQ maxDop = INT
+            | GROUP_MAX_REQUESTS EQ groupMaxRequests = INT
         )+ RPAREN
-    )? (USING (workload_group_pool_name = id_ | DEFAULT_DOUBLE_QUOTE))?
+    )? (USING (workloadGroupPoolName = id | DEFAULT_DOUBLE_QUOTE))?
     ;
 
 // https://docs.microsoft.com/en-us/sql/t-sql/statements/create-workload-group-transact-sql
-create_workload_group
-    : CREATE WORKLOAD GROUP workload_group_group_name = id_ (
+createWorkloadGroup
+    : CREATE WORKLOAD GROUP workloadGroupGroupName = id (
         WITH LPAREN (
             IMPORTANCE EQ (LOW | MEDIUM | HIGH)
-            | COMMA? REQUEST_MAX_MEMORY_GRANT_PERCENT EQ request_max_memory_grant = INT
-            | COMMA? REQUEST_MAX_CPU_TIME_SEC EQ request_max_cpu_time_sec = INT
-            | REQUEST_MEMORY_GRANT_TIMEOUT_SEC EQ request_memory_grant_timeout_sec = INT
-            | MAX_DOP EQ max_dop = INT
-            | GROUP_MAX_REQUESTS EQ group_max_requests = INT
+            | COMMA? REQUEST_MAX_MEMORY_GRANT_PERCENT EQ requestMaxMemoryGrant = INT
+            | COMMA? REQUEST_MAX_CPU_TIME_SEC EQ requestMaxCpuTimeSec = INT
+            | REQUEST_MEMORY_GRANT_TIMEOUT_SEC EQ requestMemoryGrantTimeoutSec = INT
+            | MAX_DOP EQ maxDop = INT
+            | GROUP_MAX_REQUESTS EQ groupMaxRequests = INT
         )+ RPAREN
     )? (
-        USING (workload_group_pool_name = id_ | DEFAULT_DOUBLE_QUOTE)? (
-            COMMA? EXTERNAL external_pool_name = id_
+        USING (workloadGroupPoolName = id | DEFAULT_DOUBLE_QUOTE)? (
+            COMMA? EXTERNAL externalPoolName = id
             | DEFAULT_DOUBLE_QUOTE
         )?
     )?
     ;
 
 // https://docs.microsoft.com/en-us/sql/t-sql/statements/create-xml-schema-collection-transact-sql
-create_xml_schema_collection
-    : CREATE XML SCHEMA COLLECTION (relational_schema = id_ DOT)? sql_identifier = id_ AS (
+createXmlSchemaCollection
+    : CREATE XML SCHEMA COLLECTION (relationalSchema = id DOT)? sqlIdentifier = id AS (
         STRING
-        | id_
+        | id
         | LOCAL_ID
     )
     ;
 
 // https://docs.microsoft.com/en-us/sql/t-sql/statements/create-partition-function-transact-sql?view=sql-server-ver15
-create_partition_function
-    : CREATE PARTITION FUNCTION partition_function_name = id_ LPAREN input_parameter_type = data_type RPAREN AS RANGE (
+createPartitionFunction
+    : CREATE PARTITION FUNCTION partitionFunctionName = id LPAREN inputParameterType = dataType RPAREN AS RANGE (
         LEFT
         | RIGHT
-    )? FOR VALUES LPAREN boundary_values = expression_list_ RPAREN
+    )? FOR VALUES LPAREN boundaryValues = expressionList RPAREN
     ;
 
 // https://docs.microsoft.com/en-us/sql/t-sql/statements/create-partition-scheme-transact-sql?view=sql-server-ver15
-create_partition_scheme
-    : CREATE PARTITION SCHEME partition_scheme_name = id_ AS PARTITION partition_function_name = id_ ALL? TO LPAREN file_group_names += id_ (
-        COMMA file_group_names += id_
+createPartitionScheme
+    : CREATE PARTITION SCHEME partitionSchemeName = id AS PARTITION partitionFunctionName = id ALL? TO LPAREN fileGroupNames += id (
+        COMMA fileGroupNames += id
     )* RPAREN
     ;
 
-create_queue
-    : CREATE QUEUE (full_table_name | queue_name = id_) queue_settings? (
-        ON filegroup = id_
+createQueue
+    : CREATE QUEUE (tableName | queueName = id) queueSettings? (
+        ON filegroup = id
         | DEFAULT
     )?
     ;
 
-queue_settings
-    : WITH (STATUS EQ on_off COMMA?)? (RETENTION EQ on_off COMMA?)? (
+queueSettings
+    : WITH (STATUS EQ onOff COMMA?)? (RETENTION EQ onOff COMMA?)? (
         ACTIVATION LPAREN (
             (
-                (STATUS EQ on_off COMMA?)? (
-                    PROCEDURE_NAME EQ func_proc_name_database_schema COMMA?
-                )? (MAX_QUEUE_READERS EQ max_readers = INT COMMA?)? (
-                    EXECUTE AS (SELF | user_name = STRING | OWNER) COMMA?
+                (STATUS EQ onOff COMMA?)? (
+                    PROCEDURE_NAME EQ funcProcNameDatabaseSchema COMMA?
+                )? (MAX_QUEUE_READERS EQ maxReaders = INT COMMA?)? (
+                    EXECUTE AS (SELF | userName = STRING | OWNER) COMMA?
                 )?
             )
             | DROP
         ) RPAREN COMMA?
-    )? (POISON_MESSAGE_HANDLING LPAREN (STATUS EQ on_off) RPAREN)?
+    )? (POISON_MESSAGE_HANDLING LPAREN (STATUS EQ onOff) RPAREN)?
     ;
 
-alter_queue
-    : ALTER QUEUE (full_table_name | queue_name = id_) (queue_settings | queue_action)
+alterQueue
+    : ALTER QUEUE (tableName | queueName = id) (queueSettings | queueAction)
     ;
 
-queue_action
-    : REBUILD (WITH LPAREN queue_rebuild_options RPAREN)?
-    | REORGANIZE (WITH LOB_COMPACTION EQ on_off)?
-    | MOVE TO (id_ | DEFAULT)
+queueAction
+    : REBUILD (WITH LPAREN queueRebuildOptions RPAREN)?
+    | REORGANIZE (WITH LOB_COMPACTION EQ onOff)?
+    | MOVE TO (id | DEFAULT)
     ;
 
-queue_rebuild_options
+queueRebuildOptions
     : MAXDOP EQ INT
     ;
 
-create_contract
-    : CREATE CONTRACT contract_name (AUTHORIZATION owner_name = id_)? LPAREN (
-        (message_type_name = id_ | DEFAULT) SENT BY (INITIATOR | TARGET | ANY) COMMA?
+createContract
+    : CREATE CONTRACT contractName (AUTHORIZATION ownerName = id)? LPAREN (
+        (messageTypeName = id | DEFAULT) SENT BY (INITIATOR | TARGET | ANY) COMMA?
     )+ RPAREN
     ;
 
-conversation_statement
-    : begin_conversation_timer
-    | begin_conversation_dialog
-    | end_conversation
-    | get_conversation
-    | send_conversation
-    | waitfor_conversation
+conversationStatement
+    : beginConversationTimer
+    | beginConversationDialog
+    | endConversation
+    | getConversation
+    | sendConversation
+    | waitforConversation
     ;
 
-message_statement
-    : CREATE MESSAGE TYPE message_type_name = id_ (AUTHORIZATION owner_name = id_)? (
+messageStatement
+    : CREATE MESSAGE TYPE messageTypeName = id (AUTHORIZATION ownerName = id)? (
         VALIDATION EQ (
             NONE
             | EMPTY
             | WELL_FORMED_XML
-            | VALID_XML WITH SCHEMA COLLECTION schema_collection_name = id_
+            | VALID_XML WITH SCHEMA COLLECTION schemaCollectionName = id
         )
     )
     ;
 
 // DML
 
 // https://docs.microsoft.com/en-us/sql/t-sql/statements/merge-transact-sql
-// note that there's a limit on number of when_matches but it has to be done runtime due to different ordering of statements allowed
-merge_statement
-    : with_expression? MERGE (TOP LPAREN expression RPAREN PERCENT?)? INTO? ddl_object with_table_hints? as_table_alias? USING table_sources ON
-        search_condition when_matches+ output_clause? option_clause? SEMI
+// note that there's a limit on number of whenMatches but it has to be done runtime due to different ordering of statements allowed
+mergeStatement
+    : withExpression? MERGE (TOP LPAREN expression RPAREN PERCENT?)? INTO? ddlObject withTableHints? asTableAlias? USING tableSources ON
+        searchCondition whenMatches+ outputClause? optionClause? SEMI
     ;
 
-when_matches
-    : (WHEN MATCHED (AND search_condition)? THEN merge_matched)+
-    | (WHEN NOT MATCHED (BY TARGET)? (AND search_condition)? THEN merge_not_matched)
-    | (WHEN NOT MATCHED BY SOURCE (AND search_condition)? THEN merge_matched)+
+whenMatches
+    : (WHEN MATCHED (AND searchCondition)? THEN mergeMatched)+
+    | (WHEN NOT MATCHED (BY TARGET)? (AND searchCondition)? THEN mergeNotMatched)
+    | (WHEN NOT MATCHED BY SOURCE (AND searchCondition)? THEN mergeMatched)+
     ;
 
-merge_matched
-    : UPDATE SET update_elem_merge (COMMA update_elem_merge)*
+mergeMatched
+    : UPDATE SET updateElemMerge (COMMA updateElemMerge)*
     | DELETE
     ;
 
-merge_not_matched
-    : INSERT (LPAREN column_name_list RPAREN)? (table_value_constructor | DEFAULT VALUES)
+mergeNotMatched
+    : INSERT (LPAREN columnNameList RPAREN)? (tableValueConstructor | DEFAULT VALUES)
     ;
 
 // https://msdn.microsoft.com/en-us/library/ms189835.aspx
-delete_statement
-    : with_expression? DELETE (TOP LPAREN expression RPAREN PERCENT? | TOP INT)? FROM? delete_statement_from with_table_hints? output_clause? (
-        FROM table_sources
-    )? (WHERE (search_condition | CURRENT OF (GLOBAL? cursor_name | cursor_var = LOCAL_ID)))? for_clause? option_clause? SEMI?
+deleteStatement
+    : withExpression? DELETE (TOP LPAREN expression RPAREN PERCENT? | TOP INT)? FROM? deleteStatementFrom withTableHints? outputClause? (
+        FROM tableSources
+    )? (WHERE (searchCondition | CURRENT OF (GLOBAL? cursorName | cursorVar = LOCAL_ID)))? forClause? optionClause? SEMI?
     ;
 
-delete_statement_from
-    : ddl_object
-    | rowset_function_limited
-    | table_var = LOCAL_ID
+deleteStatementFrom
+    : ddlObject
+    | rowsetFunctionLimited
+    | tableVar = LOCAL_ID
     ;
 
 // https://msdn.microsoft.com/en-us/library/ms174335.aspx
-insert_statement
-    : with_expression? INSERT (TOP LPAREN expression RPAREN PERCENT?)? INTO? (
-        ddl_object
-        | rowset_function_limited
-    ) with_table_hints? (LPAREN insert_column_name_list RPAREN)? output_clause? insert_statement_value for_clause? option_clause? SEMI?
+insertStatement
+    : withExpression? INSERT (TOP LPAREN expression RPAREN PERCENT?)? INTO? (
+        ddlObject
+        | rowsetFunctionLimited
+    ) withTableHints? (LPAREN insertColumnNameList RPAREN)? outputClause? insertStatementValue forClause? optionClause? SEMI?
     ;
 
-insert_statement_value
-    : table_value_constructor
-    | derived_table
-    | execute_statement
+insertStatementValue
+    : tableValueConstructor
+    | derivedTable
+    | executeStatement
     | DEFAULT VALUES
     ;
 
-receive_statement
-    : LPAREN? RECEIVE (ALL | DISTINCT | top_clause | STAR) (LOCAL_ID EQ expression COMMA?)* FROM full_table_name (
-        INTO table_variable = id_ (WHERE where = search_condition)
+receiveStatement
+    : LPAREN? RECEIVE (ALL | DISTINCT | topClause | STAR) (LOCAL_ID EQ expression COMMA?)* FROM tableName (
+        INTO tableVariable = id (WHERE where = searchCondition)
     )? RPAREN?
     ;
 
 // https://msdn.microsoft.com/en-us/library/ms189499.aspx
-select_statement_standalone
-    : with_expression? select_statement
+selectStatementStandalone
+    : withExpression? selectStatement
     ;
 
-select_statement
-    : query_expression select_order_by_clause? for_clause? option_clause? SEMI?
+selectStatement
+    : queryExpression selectOrderByClause? forClause? optionClause? SEMI?
     ;
 
 time
     : (LOCAL_ID | constant)
     ;
 
 // https://msdn.microsoft.com/en-us/library/ms177523.aspx
-update_statement
-    : with_expression? UPDATE (TOP LPAREN expression RPAREN PERCENT?)? (
-        ddl_object
-        | rowset_function_limited
-    ) with_table_hints? SET update_elem (COMMA update_elem)* output_clause? (FROM table_sources)? (
-        WHERE (search_condition | CURRENT OF (GLOBAL? cursor_name | cursor_var = LOCAL_ID))
-    )? for_clause? option_clause? SEMI?
+updateStatement
+    : withExpression? UPDATE (TOP LPAREN expression RPAREN PERCENT?)? (
+        ddlObject
+        | rowsetFunctionLimited
+    ) withTableHints? SET updateElem (COMMA updateElem)* outputClause? (FROM tableSources)? (
+        WHERE (searchCondition | CURRENT OF (GLOBAL? cursorName | cursorVar = LOCAL_ID))
+    )? forClause? optionClause? SEMI?
     ;
 
 // https://msdn.microsoft.com/en-us/library/ms177564.aspx
-output_clause
-    : OUTPUT output_dml_list_elem (COMMA output_dml_list_elem)* (
-        INTO (LOCAL_ID | table_name) (LPAREN column_name_list RPAREN)?
+outputClause
+    : OUTPUT outputDmlListElem (COMMA outputDmlListElem)* (
+        INTO (LOCAL_ID | tableName) (LPAREN columnNameList RPAREN)?
     )?
     ;
 
-output_dml_list_elem
-    : (expression | asterisk) as_column_alias?
+outputDmlListElem
+    : (expression | asterisk) asColumnAlias?
     ;
 
 // DDL
 
 // https://msdn.microsoft.com/en-ie/library/ms176061.aspx
-create_database
-    : CREATE DATABASE (database = id_) (CONTAINMENT EQ ( NONE | PARTIAL))? (
-        ON PRIMARY? database_file_spec ( COMMA database_file_spec)*
-    )? (LOG ON database_file_spec ( COMMA database_file_spec)*)? (COLLATE collation_name = id_)? (
-        WITH create_database_option ( COMMA create_database_option)*
+createDatabase
+    : CREATE DATABASE (database = id) (CONTAINMENT EQ ( NONE | PARTIAL))? (
+        ON PRIMARY? databaseFileSpec ( COMMA databaseFileSpec)*
+    )? (LOG ON databaseFileSpec ( COMMA databaseFileSpec)*)? (COLLATE collationName = id)? (
+        WITH createDatabaseOption ( COMMA createDatabaseOption)*
     )?
     ;
 
 // https://msdn.microsoft.com/en-us/library/ms188783.aspx
-create_index
-    : CREATE UNIQUE? clustered? INDEX id_ ON table_name LPAREN column_name_list_with_order RPAREN (
-        INCLUDE LPAREN column_name_list RPAREN
-    )? (WHERE where = search_condition)? (create_index_options)? (ON id_)? SEMI?
+createIndex
+    : CREATE UNIQUE? clustered? INDEX id ON tableName LPAREN columnNameListWithOrder RPAREN (
+        INCLUDE LPAREN columnNameList RPAREN
+    )? (WHERE where = searchCondition)? (createIndexOptions)? (ON id)? SEMI?
     ;
 
-create_index_options
-    : WITH LPAREN relational_index_option (COMMA relational_index_option)* RPAREN
+createIndexOptions
+    : WITH LPAREN relationalIndexOption (COMMA relationalIndexOption)* RPAREN
     ;
 
-relational_index_option
-    : rebuild_index_option
-    | DROP_EXISTING EQ on_off
-    | OPTIMIZE_FOR_SEQUENTIAL_KEY EQ on_off
+relationalIndexOption
+    : rebuildIndexOption
+    | DROP_EXISTING EQ onOff
+    | OPTIMIZE_FOR_SEQUENTIAL_KEY EQ onOff
     ;
 
 // https://docs.microsoft.com/en-us/sql/t-sql/statements/alter-index-transact-sql
-alter_index
-    : ALTER INDEX (id_ | ALL) ON table_name (
+alterIndex
+    : ALTER INDEX (id | ALL) ON tableName (
         DISABLE
         | PAUSE
         | ABORT
-        | RESUME resumable_index_options?
-        | reorganize_partition
-        | set_index_options
-        | rebuild_partition
+        | RESUME resumableIndexOptions?
+        | reorganizePartition
+        | setIndexOptions
+        | rebuildPartition
     )
     ;
 
-resumable_index_options
-    : WITH LPAREN (resumable_index_option (COMMA resumable_index_option)*) RPAREN
+resumableIndexOptions
+    : WITH LPAREN (resumableIndexOption (COMMA resumableIndexOption)*) RPAREN
     ;
 
-resumable_index_option
-    : MAXDOP EQ max_degree_of_parallelism = INT
-    | MAX_DURATION EQ max_duration = INT MINUTES?
-    | low_priority_lock_wait
+resumableIndexOption
+    : MAXDOP EQ maxDegreeOfParallelism = INT
+    | MAX_DURATION EQ maxDuration = INT MINUTES?
+    | lowPriorityLockWait
     ;
 
-reorganize_partition
-    : REORGANIZE (PARTITION EQ INT)? reorganize_options?
+reorganizePartition
+    : REORGANIZE (PARTITION EQ INT)? reorganizeOptions?
     ;
 
-reorganize_options
-    : WITH LPAREN (reorganize_option (COMMA reorganize_option)*) RPAREN
+reorganizeOptions
+    : WITH LPAREN (reorganizeOption (COMMA reorganizeOption)*) RPAREN
     ;
 
-reorganize_option
-    : LOB_COMPACTION EQ on_off
-    | COMPRESS_ALL_ROW_GROUPS EQ on_off
+reorganizeOption
+    : LOB_COMPACTION EQ onOff
+    | COMPRESS_ALL_ROW_GROUPS EQ onOff
     ;
 
-set_index_options
-    : SET LPAREN set_index_option (COMMA set_index_option)* RPAREN
+setIndexOptions
+    : SET LPAREN setIndexOption (COMMA setIndexOption)* RPAREN
     ;
 
-set_index_option
-    : ALLOW_ROW_LOCKS EQ on_off
-    | ALLOW_PAGE_LOCKS EQ on_off
-    | OPTIMIZE_FOR_SEQUENTIAL_KEY EQ on_off
-    | IGNORE_DUP_KEY EQ on_off
-    | STATISTICS_NORECOMPUTE EQ on_off
+setIndexOption
+    : ALLOW_ROW_LOCKS EQ onOff
+    | ALLOW_PAGE_LOCKS EQ onOff
+    | OPTIMIZE_FOR_SEQUENTIAL_KEY EQ onOff
+    | IGNORE_DUP_KEY EQ onOff
+    | STATISTICS_NORECOMPUTE EQ onOff
     | COMPRESSION_DELAY EQ delay = INT MINUTES?
     ;
 
-rebuild_partition
-    : REBUILD (PARTITION EQ ALL)? rebuild_index_options?
-    | REBUILD PARTITION EQ INT single_partition_rebuild_index_options?
+rebuildPartition
+    : REBUILD (PARTITION EQ ALL)? rebuildIndexOptions?
+    | REBUILD PARTITION EQ INT singlePartitionRebuildIndexOptions?
     ;
 
-rebuild_index_options
-    : WITH LPAREN rebuild_index_option (COMMA rebuild_index_option)* RPAREN
+rebuildIndexOptions
+    : WITH LPAREN rebuildIndexOption (COMMA rebuildIndexOption)* RPAREN
     ;
 
-rebuild_index_option
-    : PAD_INDEX EQ on_off
+rebuildIndexOption
+    : PAD_INDEX EQ onOff
     | FILLFACTOR EQ INT
-    | SORT_IN_TEMPDB EQ on_off
-    | IGNORE_DUP_KEY EQ on_off
-    | STATISTICS_NORECOMPUTE EQ on_off
-    | STATISTICS_INCREMENTAL EQ on_off
-    | ONLINE EQ (ON (LPAREN low_priority_lock_wait RPAREN)? | OFF)
-    | RESUMABLE EQ on_off
+    | SORT_IN_TEMPDB EQ onOff
+    | IGNORE_DUP_KEY EQ onOff
+    | STATISTICS_NORECOMPUTE EQ onOff
+    | STATISTICS_INCREMENTAL EQ onOff
+    | ONLINE EQ (ON (LPAREN lowPriorityLockWait RPAREN)? | OFF)
+    | RESUMABLE EQ onOff
     | MAX_DURATION EQ times = INT MINUTES?
-    | ALLOW_ROW_LOCKS EQ on_off
-    | ALLOW_PAGE_LOCKS EQ on_off
-    | MAXDOP EQ max_degree_of_parallelism = INT
-    | DATA_COMPRESSION EQ (NONE | ROW | PAGE | COLUMNSTORE | COLUMNSTORE_ARCHIVE) on_partitions?
-    | XML_COMPRESSION EQ on_off on_partitions?
+    | ALLOW_ROW_LOCKS EQ onOff
+    | ALLOW_PAGE_LOCKS EQ onOff
+    | MAXDOP EQ maxDegreeOfParallelism = INT
+    | DATA_COMPRESSION EQ (NONE | ROW | PAGE | COLUMNSTORE | COLUMNSTORE_ARCHIVE) onPartitions?
+    | XML_COMPRESSION EQ onOff onPartitions?
     ;
 
-single_partition_rebuild_index_options
-    : WITH LPAREN single_partition_rebuild_index_option (COMMA single_partition_rebuild_index_option)* RPAREN
+singlePartitionRebuildIndexOptions
+    : WITH LPAREN singlePartitionRebuildIndexOption (COMMA singlePartitionRebuildIndexOption)* RPAREN
     ;
 
-single_partition_rebuild_index_option
-    : SORT_IN_TEMPDB EQ on_off
-    | MAXDOP EQ max_degree_of_parallelism = INT
-    | RESUMABLE EQ on_off
-    | DATA_COMPRESSION EQ (NONE | ROW | PAGE | COLUMNSTORE | COLUMNSTORE_ARCHIVE) on_partitions?
-    | XML_COMPRESSION EQ on_off on_partitions?
-    | ONLINE EQ (ON (LPAREN low_priority_lock_wait RPAREN)? | OFF)
+singlePartitionRebuildIndexOption
+    : SORT_IN_TEMPDB EQ onOff
+    | MAXDOP EQ maxDegreeOfParallelism = INT
+    | RESUMABLE EQ onOff
+    | DATA_COMPRESSION EQ (NONE | ROW | PAGE | COLUMNSTORE | COLUMNSTORE_ARCHIVE) onPartitions?
+    | XML_COMPRESSION EQ onOff onPartitions?
+    | ONLINE EQ (ON (LPAREN lowPriorityLockWait RPAREN)? | OFF)
     ;
 
-on_partitions
-    : ON PARTITIONS LPAREN partition_number = INT (TO to_partition_number = INT)? (
-        COMMA partition_number = INT (TO to_partition_number = INT)?
+onPartitions
+    : ON PARTITIONS LPAREN partitionNumber = INT (TO toPartitionNumber = INT)? (
+        COMMA partitionNumber = INT (TO toPartitionNumber = INT)?
     )* RPAREN
     ;
 
 // https://docs.microsoft.com/en-us/sql/t-sql/statements/create-columnstore-index-transact-sql?view=sql-server-ver15
-create_columnstore_index
-    : CREATE CLUSTERED COLUMNSTORE INDEX id_ ON table_name create_columnstore_index_options? (
-        ON id_
+createColumnstoreIndex
+    : CREATE CLUSTERED COLUMNSTORE INDEX id ON tableName createColumnstoreIndexOptions? (
+        ON id
     )? SEMI?
     ;
 
-create_columnstore_index_options
-    : WITH LPAREN columnstore_index_option (COMMA columnstore_index_option)* RPAREN
+createColumnstoreIndexOptions
+    : WITH LPAREN columnstoreIndexOption (COMMA columnstoreIndexOption)* RPAREN
     ;
 
-columnstore_index_option
-    : DROP_EXISTING EQ on_off
-    | MAXDOP EQ max_degree_of_parallelism = INT
-    | ONLINE EQ on_off
+columnstoreIndexOption
+    : DROP_EXISTING EQ onOff
+    | MAXDOP EQ maxDegreeOfParallelism = INT
+    | ONLINE EQ onOff
     | COMPRESSION_DELAY EQ delay = INT MINUTES?
-    | DATA_COMPRESSION EQ (COLUMNSTORE | COLUMNSTORE_ARCHIVE) on_partitions?
+    | DATA_COMPRESSION EQ (COLUMNSTORE | COLUMNSTORE_ARCHIVE) onPartitions?
     ;
 
 // https://docs.microsoft.com/en-us/sql/t-sql/statements/create-columnstore-index-transact-sql?view=sql-server-ver15
-create_nonclustered_columnstore_index
-    : CREATE NONCLUSTERED? COLUMNSTORE INDEX id_ ON table_name LPAREN column_name_list_with_order RPAREN (
-        WHERE search_condition
-    )? create_columnstore_index_options? (ON id_)? SEMI?
+createNonclusteredColumnstoreIndex
+    : CREATE NONCLUSTERED? COLUMNSTORE INDEX id ON tableName LPAREN columnNameListWithOrder RPAREN (
+        WHERE searchCondition
+    )? createColumnstoreIndexOptions? (ON id)? SEMI?
     ;
 
-create_xml_index
-    : CREATE PRIMARY? XML INDEX id_ ON table_name LPAREN id_ RPAREN (
-        USING XML INDEX id_ (FOR (VALUE | PATH | PROPERTY)?)?
-    )? xml_index_options? SEMI?
+createXmlIndex
+    : CREATE PRIMARY? XML INDEX id ON tableName LPAREN id RPAREN (
+        USING XML INDEX id (FOR (VALUE | PATH | PROPERTY)?)?
+    )? xmlIndexOptions? SEMI?
     ;
 
-xml_index_options
-    : WITH LPAREN xml_index_option (COMMA xml_index_option)* RPAREN
+xmlIndexOptions
+    : WITH LPAREN xmlIndexOption (COMMA xmlIndexOption)* RPAREN
     ;
 
-xml_index_option
-    : PAD_INDEX EQ on_off
+xmlIndexOption
+    : PAD_INDEX EQ onOff
     | FILLFACTOR EQ INT
-    | SORT_IN_TEMPDB EQ on_off
-    | IGNORE_DUP_KEY EQ on_off
-    | DROP_EXISTING EQ on_off
-    | ONLINE EQ (ON (LPAREN low_priority_lock_wait RPAREN)? | OFF)
-    | ALLOW_ROW_LOCKS EQ on_off
-    | ALLOW_PAGE_LOCKS EQ on_off
-    | MAXDOP EQ max_degree_of_parallelism = INT
-    | XML_COMPRESSION EQ on_off
+    | SORT_IN_TEMPDB EQ onOff
+    | IGNORE_DUP_KEY EQ onOff
+    | DROP_EXISTING EQ onOff
+    | ONLINE EQ (ON (LPAREN lowPriorityLockWait RPAREN)? | OFF)
+    | ALLOW_ROW_LOCKS EQ onOff
+    | ALLOW_PAGE_LOCKS EQ onOff
+    | MAXDOP EQ maxDegreeOfParallelism = INT
+    | XML_COMPRESSION EQ onOff
     ;
 
 // https://msdn.microsoft.com/en-us/library/ms187926(v=sql.120).aspx
-create_or_alter_procedure
-    : ((CREATE (OR (ALTER | REPLACE))?) | ALTER) proc = (PROC | PROCEDURE) procName = func_proc_name_schema (
+createOrAlterProcedure
+    : ((CREATE (OR (ALTER | REPLACE))?) | ALTER) proc = (PROC | PROCEDURE) procName = funcProcNameSchema (
         SEMI INT
-    )? (LPAREN? procedure_param (COMMA procedure_param)* RPAREN?)? (
-        WITH procedure_option (COMMA procedure_option)*
-    )? (FOR REPLICATION)? AS (as_external_name | sql_clauses*)
+    )? (LPAREN? procedureParam (COMMA procedureParam)* RPAREN?)? (
+        WITH procedureOption (COMMA procedureOption)*
+    )? (FOR REPLICATION)? AS (asExternalName | sqlClauses*)
     ;
 
-as_external_name
-    : EXTERNAL NAME assembly_name = id_ DOT class_name = id_ DOT method_name = id_
+asExternalName
+    : EXTERNAL NAME assemblyName = id DOT className = id DOT methodName = id
     ;
 
 // https://docs.microsoft.com/en-us/sql/t-sql/statements/create-trigger-transact-sql
-create_or_alter_trigger
-    : create_or_alter_dml_trigger
-    | create_or_alter_ddl_trigger
+createOrAlterTrigger
+    : createOrAlterDmlTrigger
+    | createOrAlterDdlTrigger
     ;
 
-create_or_alter_dml_trigger
-    : (CREATE (OR (ALTER | REPLACE))? | ALTER) TRIGGER simple_name ON table_name (
-        WITH dml_trigger_option (COMMA dml_trigger_option)*
-    )? (FOR | AFTER | INSTEAD OF) dml_trigger_operation (COMMA dml_trigger_operation)* (WITH APPEND)? (
+createOrAlterDmlTrigger
+    : (CREATE (OR (ALTER | REPLACE))? | ALTER) TRIGGER simpleName ON tableName (
+        WITH dmlTriggerOption (COMMA dmlTriggerOption)*
+    )? (FOR | AFTER | INSTEAD OF) dmlTriggerOperation (COMMA dmlTriggerOperation)* (WITH APPEND)? (
         NOT FOR REPLICATION
-    )? AS sql_clauses+
+    )? AS sqlClauses+
     ;
 
-dml_trigger_option
+dmlTriggerOption
     : ENCRYPTION
-    | execute_clause
+    | executeClause
     ;
 
-dml_trigger_operation
+dmlTriggerOperation
     : (INSERT | UPDATE | DELETE)
     ;
 
-create_or_alter_ddl_trigger
-    : (CREATE (OR (ALTER | REPLACE))? | ALTER) TRIGGER simple_name ON (ALL SERVER | DATABASE) (
-        WITH dml_trigger_option (COMMA dml_trigger_option)*
-    )? (FOR | AFTER) ddl_trigger_operation (COMMA ddl_trigger_operation)* AS sql_clauses+
+createOrAlterDdlTrigger
+    : (CREATE (OR (ALTER | REPLACE))? | ALTER) TRIGGER simpleName ON (ALL SERVER | DATABASE) (
+        WITH dmlTriggerOption (COMMA dmlTriggerOption)*
+    )? (FOR | AFTER) ddlTriggerOperation (COMMA ddlTriggerOperation)* AS sqlClauses+
     ;
 
-ddl_trigger_operation
-    : simple_id
+ddlTriggerOperation
+    : simpleId
     ;
 
 // https://msdn.microsoft.com/en-us/library/ms186755.aspx
-create_or_alter_function
-    : ((CREATE (OR ALTER)?) | ALTER) FUNCTION funcName = func_proc_name_schema (
-        (LPAREN procedure_param (COMMA procedure_param)* RPAREN)
+createOrAlterFunction
+    : ((CREATE (OR ALTER)?) | ALTER) FUNCTION funcName = funcProcNameSchema (
+        (LPAREN procedureParam (COMMA procedureParam)* RPAREN)
         | LPAREN RPAREN
     ) //must have (), but can be empty
-    (func_body_returns_select | func_body_returns_table | func_body_returns_scalar) SEMI?
+    (funcBodyReturnsSelect | funcBodyReturnsTable | funcBodyReturnsScalar) SEMI?
     ;
 
-func_body_returns_select
-    : RETURNS TABLE (WITH function_option (COMMA function_option)*)? AS? (
-        as_external_name
-        | RETURN (LPAREN select_statement_standalone RPAREN | select_statement_standalone)
+funcBodyReturnsSelect
+    : RETURNS TABLE (WITH functionOption (COMMA functionOption)*)? AS? (
+        asExternalName
+        | RETURN (LPAREN selectStatementStandalone RPAREN | selectStatementStandalone)
     )
     ;
 
-func_body_returns_table
-    : RETURNS LOCAL_ID table_type_definition (WITH function_option (COMMA function_option)*)? AS? (
-        as_external_name
-        | BEGIN sql_clauses* RETURN SEMI? END SEMI?
+funcBodyReturnsTable
+    : RETURNS LOCAL_ID tableTypeDefinition (WITH functionOption (COMMA functionOption)*)? AS? (
+        asExternalName
+        | BEGIN sqlClauses* RETURN SEMI? END SEMI?
     )
     ;
 
-func_body_returns_scalar
-    : RETURNS data_type (WITH function_option (COMMA function_option)*)? AS? (
-        as_external_name
-        | BEGIN sql_clauses* RETURN ret = expression SEMI? END
+funcBodyReturnsScalar
+    : RETURNS dataType (WITH functionOption (COMMA functionOption)*)? AS? (
+        asExternalName
+        | BEGIN sqlClauses* RETURN ret = expression SEMI? END
     )
     ;
 
-procedure_param_default_value
+procedureParamDefaultValue
     : NULL_
     | DEFAULT
     | constant
     | LOCAL_ID
     ;
 
-procedure_param
-    : LOCAL_ID AS? (type_schema = id_ DOT)? data_type VARYING? (
-        EQ default_val = procedure_param_default_value
+procedureParam
+    : LOCAL_ID AS? (typeSchema = id DOT)? dataType VARYING? (
+        EQ defaultVal = procedureParamDefaultValue
     )? (OUT | OUTPUT | READONLY)?
     ;
 
-procedure_option
+procedureOption
     : ENCRYPTION
     | RECOMPILE
-    | execute_clause
+    | executeClause
     ;
 
-function_option
+functionOption
     : ENCRYPTION
     | SCHEMABINDING
     | RETURNS NULL_ ON NULL_ INPUT
     | CALLED ON NULL_ INPUT
-    | execute_clause
+    | executeClause
     ;
 
 // https://msdn.microsoft.com/en-us/library/ms188038.aspx
-create_statistics
-    : CREATE STATISTICS id_ ON table_name LPAREN column_name_list RPAREN (
+createStatistics
+    : CREATE STATISTICS id ON tableName LPAREN columnNameList RPAREN (
         WITH (FULLSCAN | SAMPLE INT (PERCENT | ROWS) | STATS_STREAM) (COMMA NORECOMPUTE)? (
-            COMMA INCREMENTAL EQ on_off
+            COMMA INCREMENTAL EQ onOff
         )?
     )? SEMI?
     ;
 
-update_statistics
-    : UPDATE STATISTICS full_table_name (id_ | LPAREN id_ ( COMMA id_)* RPAREN)? update_statistics_options?
+updateStatistics
+    : UPDATE STATISTICS tableName (id | LPAREN id ( COMMA id)* RPAREN)? updateStatisticsOptions?
     ;
 
-update_statistics_options
-    : WITH update_statistics_option (COMMA update_statistics_option)*
+updateStatisticsOptions
+    : WITH updateStatisticsOption (COMMA updateStatisticsOption)*
     ;
 
-update_statistics_option
-    : (FULLSCAN (COMMA? PERSIST_SAMPLE_PERCENT EQ on_off)?)
-    | (SAMPLE number = INT (PERCENT | ROWS) (COMMA? PERSIST_SAMPLE_PERCENT EQ on_off)?)
-    | RESAMPLE on_partitions?
-    | STATS_STREAM EQ stats_stream_ = expression
+updateStatisticsOption
+    : (FULLSCAN (COMMA? PERSIST_SAMPLE_PERCENT EQ onOff)?)
+    | (SAMPLE number = INT (PERCENT | ROWS) (COMMA? PERSIST_SAMPLE_PERCENT EQ onOff)?)
+    | RESAMPLE onPartitions?
+    | STATS_STREAM EQ statsStream_ = expression
     | ROWCOUNT EQ INT
     | PAGECOUNT EQ INT
     | ALL
     | COLUMNS
     | INDEX
     | NORECOMPUTE
-    | INCREMENTAL EQ on_off
-    | MAXDOP EQ max_dregree_of_parallelism = INT
-    | AUTO_DROP EQ on_off
+    | INCREMENTAL EQ onOff
+    | MAXDOP EQ maxDregreeOfParallelism = INT
+    | AUTO_DROP EQ onOff
     ;
 
 // https://msdn.microsoft.com/en-us/library/ms174979.aspx
-create_table
-    : CREATE TABLE table_name LPAREN column_def_table_constraints (COMMA? table_indices)* COMMA? RPAREN (
-        LOCK simple_id
-    )? table_options* (ON id_ | DEFAULT | on_partition_or_filegroup)? (TEXTIMAGE_ON id_ | DEFAULT)? SEMI?
+createTable
+    : CREATE TABLE tableName LPAREN columnDefTableConstraints (COMMA? tableIndices)* COMMA? RPAREN (
+        LOCK simpleId
+    )? tableOptions* (ON id | DEFAULT | onPartitionOrFilegroup)? (TEXTIMAGE_ON id | DEFAULT)? SEMI?
     ;
 
-table_indices
-    : INDEX id_ UNIQUE? clustered? LPAREN column_name_list_with_order RPAREN
-    | INDEX id_ CLUSTERED COLUMNSTORE
-    | INDEX id_ NONCLUSTERED? COLUMNSTORE LPAREN column_name_list RPAREN create_table_index_options? (
-        ON id_
+tableIndices
+    : INDEX id UNIQUE? clustered? LPAREN columnNameListWithOrder RPAREN
+    | INDEX id CLUSTERED COLUMNSTORE
+    | INDEX id NONCLUSTERED? COLUMNSTORE LPAREN columnNameList RPAREN createTableIndexOptions? (
+        ON id
     )?
     ;
 
-table_options
-    : WITH (LPAREN table_option (COMMA table_option)* RPAREN | table_option (COMMA table_option)*)
+tableOptions
+    : WITH (LPAREN tableOption (COMMA tableOption)* RPAREN | tableOption (COMMA tableOption)*)
     ;
 
-table_option
-    : (simple_id | keyword) EQ (simple_id | keyword | on_off | INT)
+tableOption
+    : (simpleId | keyword) EQ (simpleId | keyword | onOff | INT)
     | CLUSTERED COLUMNSTORE INDEX
     | HEAP
     | FILLFACTOR EQ INT
-    | DISTRIBUTION EQ HASH LPAREN id_ RPAREN
-    | CLUSTERED INDEX LPAREN id_ (ASC | DESC)? (COMMA id_ (ASC | DESC)?)* RPAREN
-    | DATA_COMPRESSION EQ (NONE | ROW | PAGE) on_partitions?
-    | XML_COMPRESSION EQ on_off on_partitions?
+    | DISTRIBUTION EQ HASH LPAREN id RPAREN
+    | CLUSTERED INDEX LPAREN id (ASC | DESC)? (COMMA id (ASC | DESC)?)* RPAREN
+    | DATA_COMPRESSION EQ (NONE | ROW | PAGE) onPartitions?
+    | XML_COMPRESSION EQ onOff onPartitions?
     ;
 
-create_table_index_options
-    : WITH LPAREN create_table_index_option (COMMA create_table_index_option)* RPAREN
+createTableIndexOptions
+    : WITH LPAREN createTableIndexOption (COMMA createTableIndexOption)* RPAREN
     ;
 
-create_table_index_option
-    : PAD_INDEX EQ on_off
+createTableIndexOption
+    : PAD_INDEX EQ onOff
     | FILLFACTOR EQ INT
-    | IGNORE_DUP_KEY EQ on_off
-    | STATISTICS_NORECOMPUTE EQ on_off
-    | STATISTICS_INCREMENTAL EQ on_off
-    | ALLOW_ROW_LOCKS EQ on_off
-    | ALLOW_PAGE_LOCKS EQ on_off
-    | OPTIMIZE_FOR_SEQUENTIAL_KEY EQ on_off
-    | DATA_COMPRESSION EQ (NONE | ROW | PAGE | COLUMNSTORE | COLUMNSTORE_ARCHIVE) on_partitions?
-    | XML_COMPRESSION EQ on_off on_partitions?
+    | IGNORE_DUP_KEY EQ onOff
+    | STATISTICS_NORECOMPUTE EQ onOff
+    | STATISTICS_INCREMENTAL EQ onOff
+    | ALLOW_ROW_LOCKS EQ onOff
+    | ALLOW_PAGE_LOCKS EQ onOff
+    | OPTIMIZE_FOR_SEQUENTIAL_KEY EQ onOff
+    | DATA_COMPRESSION EQ (NONE | ROW | PAGE | COLUMNSTORE | COLUMNSTORE_ARCHIVE) onPartitions?
+    | XML_COMPRESSION EQ onOff onPartitions?
     ;
 
 // https://msdn.microsoft.com/en-us/library/ms187956.aspx
-create_view
-    : (CREATE (OR (ALTER | REPLACE))? | ALTER) VIEW simple_name (LPAREN column_name_list RPAREN)? (
-        WITH view_attribute (COMMA view_attribute)*
-    )? AS select_statement_standalone (WITH CHECK OPTION)? SEMI?
+createView
+    : (CREATE (OR (ALTER | REPLACE))? | ALTER) VIEW simpleName (LPAREN columnNameList RPAREN)? (
+        WITH viewAttribute (COMMA viewAttribute)*
+    )? AS selectStatementStandalone (WITH CHECK OPTION)? SEMI?
     ;
 
-view_attribute
+viewAttribute
     : ENCRYPTION
     | SCHEMABINDING
     | VIEW_METADATA
     ;
 
 // https://msdn.microsoft.com/en-us/library/ms190273.aspx
-alter_table
-    : ALTER TABLE table_name (
+alterTable
+    : ALTER TABLE tableName (
         SET LPAREN LOCK_ESCALATION EQ (AUTO | TABLE | DISABLE) RPAREN
-        | ADD column_def_table_constraints
-        | ALTER COLUMN (column_definition | column_modifier)
-        | DROP COLUMN id_ (COMMA id_)*
-        | DROP CONSTRAINT constraint = id_
-        | WITH (CHECK | NOCHECK) ADD (CONSTRAINT constraint = id_)? (
-            FOREIGN KEY LPAREN fk = column_name_list RPAREN REFERENCES table_name (
-                LPAREN pk = column_name_list RPAREN
-            )? (on_delete | on_update)*
-            | CHECK LPAREN search_condition RPAREN
+        | ADD columnDefTableConstraints
+        | ALTER COLUMN (columnDefinition | columnModifier)
+        | DROP COLUMN id (COMMA id)*
+        | DROP CONSTRAINT constraint = id
+        | WITH (CHECK | NOCHECK) ADD (CONSTRAINT constraint = id)? (
+            FOREIGN KEY LPAREN fk = columnNameList RPAREN REFERENCES tableName (
+                LPAREN pk = columnNameList RPAREN
+            )? (onDelete | onUpdate)*
+            | CHECK LPAREN searchCondition RPAREN
         )
-        | (NOCHECK | CHECK) CONSTRAINT constraint = id_
-        | (ENABLE | DISABLE) TRIGGER id_?
-        | REBUILD table_options
-        | SWITCH switch_partition
+        | (NOCHECK | CHECK) CONSTRAINT constraint = id
+        | (ENABLE | DISABLE) TRIGGER id?
+        | REBUILD tableOptions
+        | SWITCH switchPartition
     ) SEMI?
     ;
 
-switch_partition
-    : (PARTITION? source_partition_number_expression = expression)? TO target_table = table_name (
-        PARTITION target_partition_number_expression = expression
-    )? (WITH low_priority_lock_wait)?
+switchPartition
+    : (PARTITION? sourcePartitionNumberExpression = expression)? TO targetTable = tableName (
+        PARTITION targetPartitionNumberExpression = expression
+    )? (WITH lowPriorityLockWait)?
     ;
 
-low_priority_lock_wait
-    : WAIT_AT_LOW_PRIORITY LPAREN MAX_DURATION EQ max_duration = time MINUTES? COMMA ABORT_AFTER_WAIT EQ abort_after_wait = (
+lowPriorityLockWait
+    : WAIT_AT_LOW_PRIORITY LPAREN MAX_DURATION EQ maxDuration = time MINUTES? COMMA ABORT_AFTER_WAIT EQ abortAfterWait = (
         NONE
         | SELF
         | BLOCKERS
     ) RPAREN
     ;
 
 // https://msdn.microsoft.com/en-us/library/ms174269.aspx
-alter_database
-    : ALTER DATABASE (database = id_ | CURRENT) (
-        MODIFY NAME EQ new_name = id_
-        | COLLATE collation = id_
-        | SET database_optionspec (WITH termination)?
-        | add_or_modify_files
-        | add_or_modify_filegroups
+alterDatabase
+    : ALTER DATABASE (database = id | CURRENT) (
+        MODIFY NAME EQ newName = id
+        | COLLATE collation = id
+        | SET databaseOptionspec (WITH termination)?
+        | addOrModifyFiles
+        | addOrModifyFilegroups
     ) SEMI?
     ;
 
 // https://docs.microsoft.com/en-us/sql/t-sql/statements/alter-database-transact-sql-file-and-filegroup-options?view=sql-server-ver15
-add_or_modify_files
-    : ADD FILE filespec (COMMA filespec)* (TO FILEGROUP filegroup_name = id_)?
-    | ADD LOG FILE filespec (COMMA filespec)*
-    | REMOVE FILE logical_file_name = id_
-    | MODIFY FILE filespec
+addOrModifyFiles
+    : ADD FILE fileSpec (COMMA fileSpec)* (TO FILEGROUP filegroupName = id)?
+    | ADD LOG FILE fileSpec (COMMA fileSpec)*
+    | REMOVE FILE logicalFileName = id
+    | MODIFY FILE fileSpec
     ;
 
-filespec
-    : LPAREN NAME EQ name = id_or_string (COMMA NEWNAME EQ new_name = id_or_string)? (
-        COMMA FILENAME EQ file_name = STRING
-    )? (COMMA SIZE EQ size = file_size)? (COMMA MAXSIZE EQ (max_size = file_size) | UNLIMITED)? (
-        COMMA FILEGROWTH EQ growth_increment = file_size
+fileSpec
+    : LPAREN NAME EQ name = idOrString (COMMA NEWNAME EQ newName = idOrString)? (
+        COMMA FILENAME EQ fileName = STRING
+    )? (COMMA SIZE EQ size = fileSize)? (COMMA MAXSIZE EQ (maxSize = fileSize) | UNLIMITED)? (
+        COMMA FILEGROWTH EQ growthIncrement = fileSize
     )? (COMMA OFFLINE)? RPAREN
     ;
 
-add_or_modify_filegroups
-    : ADD FILEGROUP filegroup_name = id_ (CONTAINS FILESTREAM | CONTAINS MEMORY_OPTIMIZED_DATA)?
-    | REMOVE FILEGROUP filegrou_name = id_
-    | MODIFY FILEGROUP filegrou_name = id_ (
-        filegroup_updatability_option
+addOrModifyFilegroups
+    : ADD FILEGROUP filegroupName = id (CONTAINS FILESTREAM | CONTAINS MEMORY_OPTIMIZED_DATA)?
+    | REMOVE FILEGROUP filegrouName = id
+    | MODIFY FILEGROUP filegrouName = id (
+        filegroupUpdatabilityOption
         | DEFAULT
-        | NAME EQ new_filegroup_name = id_
+        | NAME EQ newFilegroupName = id
         | AUTOGROW_SINGLE_FILE
         | AUTOGROW_ALL_FILES
     )
     ;
 
-filegroup_updatability_option
+filegroupUpdatabilityOption
     : READONLY
     | READWRITE
     | READ_ONLY
     | READ_WRITE
     ;
 
 // https://msdn.microsoft.com/en-us/library/bb522682.aspx
 // Runtime check.
-database_optionspec
-    : auto_option
-    | change_tracking_option
-    | containment_option
-    | cursor_option
-    | database_mirroring_option
-    | date_correlation_optimization_option
-    | db_encryption_option
-    | db_state_option
-    | db_update_option
-    | db_user_access_option
-    | delayed_durability_option
-    | external_access_option
-    | FILESTREAM database_filestream_option
-    | hadr_options
-    | mixed_page_allocation_option
-    | parameterization_option
-    //  | query_store_options
-    | recovery_option
-    //  | remote_data_archive_option
-    | service_broker_option
-    | snapshot_option
-    | sql_option
-    | target_recovery_time_option
+databaseOptionspec
+    : autoOption
+    | changeTrackingOption
+    | containmentOption
+    | cursorOption
+    | databaseMirroringOption
+    | dateCorrelationOptimizationOption
+    | dbEncryptionOption
+    | dbStateOption
+    | dbUpdateOption
+    | dbUserAccessOption
+    | delayedDurabilityOption
+    | externalAccessOption
+    | FILESTREAM databaseFilestreamOption
+    | hadrOptions
+    | mixedPageAllocationOption
+    | parameterizationOption
+    //  | queryStoreOptions
+    | recoveryOption
+    //  | remoteDataArchiveOption
+    | serviceBrokerOption
+    | snapshotOption
+    | sqlOption
+    | targetRecoveryTimeOption
     | termination
     ;
 
-auto_option
-    : AUTO_CLOSE on_off
+autoOption
+    : AUTO_CLOSE onOff
     | AUTO_CREATE_STATISTICS OFF
     | ON ( INCREMENTAL EQ ON | OFF)
-    | AUTO_SHRINK on_off
-    | AUTO_UPDATE_STATISTICS on_off
+    | AUTO_SHRINK onOff
+    | AUTO_UPDATE_STATISTICS onOff
     | AUTO_UPDATE_STATISTICS_ASYNC (ON | OFF)
     ;
 
-change_tracking_option
+changeTrackingOption
     : CHANGE_TRACKING EQ (
         OFF
-        | ON LPAREN (change_tracking_option_list (COMMA change_tracking_option_list)*)* RPAREN
+        | ON LPAREN (changeTrackingOptionList (COMMA changeTrackingOptionList)*)* RPAREN
     )
     ;
 
-change_tracking_option_list
-    : AUTO_CLEANUP EQ on_off
+changeTrackingOptionList
+    : AUTO_CLEANUP EQ onOff
     | CHANGE_RETENTION EQ INT ( DAYS | HOURS | MINUTES)
     ;
 
-containment_option
+containmentOption
     : CONTAINMENT EQ (NONE | PARTIAL)
     ;
 
-cursor_option
-    : CURSOR_CLOSE_ON_COMMIT on_off
+cursorOption
+    : CURSOR_CLOSE_ON_COMMIT onOff
     | CURSOR_DEFAULT ( LOCAL | GLOBAL)
     ;
 
 // https://docs.microsoft.com/en-us/sql/t-sql/statements/alter-endpoint-transact-sql
-alter_endpoint
-    : ALTER ENDPOINT endpointname = id_ (AUTHORIZATION login = id_)? (
+alterEndpoint
+    : ALTER ENDPOINT endpointname = id (AUTHORIZATION login = id)? (
         STATE EQ state = (STARTED | STOPPED | DISABLED)
-    )? AS TCP LPAREN endpoint_listener_clause RPAREN (
+    )? AS TCP LPAREN endpointListenerClause RPAREN (
         FOR TSQL LPAREN RPAREN
-        | FOR SERVICE_BROKER LPAREN endpoint_authentication_clause (
-            COMMA? endpoint_encryption_alogorithm_clause
+        | FOR SERVICE_BROKER LPAREN endpointAuthenticationClause (
+            COMMA? endpointEncryptionAlogorithmClause
         )? (COMMA? MESSAGE_FORWARDING EQ (ENABLED | DISABLED))? (
             COMMA? MESSAGE_FORWARD_SIZE EQ INT
         )? RPAREN
-        | FOR DATABASE_MIRRORING LPAREN endpoint_authentication_clause (
-            COMMA? endpoint_encryption_alogorithm_clause
+        | FOR DATABASE_MIRRORING LPAREN endpointAuthenticationClause (
+            COMMA? endpointEncryptionAlogorithmClause
         )? COMMA? ROLE EQ (WITNESS | PARTNER | ALL) RPAREN
     )
     ;
 
 /* Will visit later
 */
-database_mirroring_option
-    : mirroring_set_option
+databaseMirroringOption
+    : mirroringSetOption
     ;
 
-mirroring_set_option
-    : mirroring_partner partner_option
-    | mirroring_witness witness_option
+mirroringSetOption
+    : mirroringPartner partnerOption
+    | mirroringWitness witnessOption
     ;
 
-mirroring_partner
+mirroringPartner
     : PARTNER
     ;
 
-mirroring_witness
+mirroringWitness
     : WITNESS
     ;
 
-witness_partner_equal
+witnessPartnerEqual
     : EQ
     ;
 
-partner_option
-    : witness_partner_equal partner_server
+partnerOption
+    : witnessPartnerEqual partnerServer
     | FAILOVER
     | FORCE_SERVICE_ALLOW_DATA_LOSS
     | OFF
     | RESUME
     | SAFETY (FULL | OFF)
     | SUSPEND
     | TIMEOUT INT
     ;
 
-witness_option
-    : witness_partner_equal witness_server
+witnessOption
+    : witnessPartnerEqual witnessServer
     | OFF
     ;
 
-witness_server
-    : partner_server
+witnessServer
+    : partnerServer
     ;
 
-partner_server
-    : partner_server_tcp_prefix host mirroring_host_port_seperator port_number
+partnerServer
+    : partnerServerTcpPrefix host mirroringHostPortSeperator portNumber
     ;
 
-mirroring_host_port_seperator
+mirroringHostPortSeperator
     : COLON
     ;
 
-partner_server_tcp_prefix
+partnerServerTcpPrefix
     : TCP COLON DOUBLE_FORWARD_SLASH
     ;
 
-port_number
+portNumber
     : port = INT
     ;
 
 host
-    : id_ DOT host
-    | (id_ DOT | id_)
+    : id DOT host
+    | (id DOT | id)
     ;
 
-date_correlation_optimization_option
-    : DATE_CORRELATION_OPTIMIZATION on_off
+dateCorrelationOptimizationOption
+    : DATE_CORRELATION_OPTIMIZATION onOff
     ;
 
-db_encryption_option
-    : ENCRYPTION on_off
+dbEncryptionOption
+    : ENCRYPTION onOff
     ;
 
-db_state_option
+dbStateOption
     : (ONLINE | OFFLINE | EMERGENCY)
     ;
 
-db_update_option
+dbUpdateOption
     : READ_ONLY
     | READ_WRITE
     ;
 
-db_user_access_option
+dbUserAccessOption
     : SINGLE_USER
     | RESTRICTED_USER
     | MULTI_USER
     ;
 
-delayed_durability_option
+delayedDurabilityOption
     : DELAYED_DURABILITY EQ (DISABLED | ALLOWED | FORCED)
     ;
 
-external_access_option
-    : DB_CHAINING on_off
-    | TRUSTWORTHY on_off
-    | DEFAULT_LANGUAGE EQ ( id_ | STRING)
-    | DEFAULT_FULLTEXT_LANGUAGE EQ ( id_ | STRING)
+externalAccessOption
+    : DB_CHAINING onOff
+    | TRUSTWORTHY onOff
+    | DEFAULT_LANGUAGE EQ ( id | STRING)
+    | DEFAULT_FULLTEXT_LANGUAGE EQ ( id | STRING)
     | NESTED_TRIGGERS EQ ( OFF | ON)
     | TRANSFORM_NOISE_WORDS EQ ( OFF | ON)
     | TWO_DIGIT_YEAR_CUTOFF EQ INT
     ;
 
-hadr_options
-    : HADR (( AVAILABILITY GROUP EQ availability_group_name = id_ | OFF) | (SUSPEND | RESUME))
+hadrOptions
+    : HADR (( AVAILABILITY GROUP EQ availabilityGroupName = id | OFF) | (SUSPEND | RESUME))
     ;
 
-mixed_page_allocation_option
+mixedPageAllocationOption
     : MIXED_PAGE_ALLOCATION (OFF | ON)
     ;
 
-parameterization_option
+parameterizationOption
     : PARAMETERIZATION (SIMPLE | FORCED)
     ;
 
-recovery_option
+recoveryOption
     : RECOVERY (FULL | BULK_LOGGED | SIMPLE)
-    | TORN_PAGE_DETECTION on_off
-    | ACCELERATED_DATABASE_RECOVERY EQ on_off
+    | TORN_PAGE_DETECTION onOff
+    | ACCELERATED_DATABASE_RECOVERY EQ onOff
     | PAGE_VERIFY ( CHECKSUM | TORN_PAGE_DETECTION | NONE)
     ;
 
-service_broker_option
+serviceBrokerOption
     : ENABLE_BROKER
     | DISABLE_BROKER
     | NEW_BROKER
     | ERROR_BROKER_CONVERSATIONS
-    | HONOR_BROKER_PRIORITY on_off
+    | HONOR_BROKER_PRIORITY onOff
     ;
 
-snapshot_option
-    : ALLOW_SNAPSHOT_ISOLATION on_off
+snapshotOption
+    : ALLOW_SNAPSHOT_ISOLATION onOff
     | READ_COMMITTED_SNAPSHOT (ON | OFF)
     | MEMORY_OPTIMIZED_ELEVATE_TO_SNAPSHOT = (ON | OFF)
     ;
 
-sql_option
-    : ANSI_NULL_DEFAULT on_off
-    | ANSI_NULLS on_off
-    | ANSI_PADDING on_off
-    | ANSI_WARNINGS on_off
-    | ARITHABORT on_off
+sqlOption
+    : ANSI_NULL_DEFAULT onOff
+    | ANSI_NULLS onOff
+    | ANSI_PADDING onOff
+    | ANSI_WARNINGS onOff
+    | ARITHABORT onOff
     | COMPATIBILITY_LEVEL EQ INT
-    | CONCAT_NULL_YIELDS_NULL on_off
-    | NUMERIC_ROUNDABORT on_off
-    | QUOTED_IDENTIFIER on_off
-    | RECURSIVE_TRIGGERS on_off
+    | CONCAT_NULL_YIELDS_NULL onOff
+    | NUMERIC_ROUNDABORT onOff
+    | QUOTED_IDENTIFIER onOff
+    | RECURSIVE_TRIGGERS onOff
     ;
 
-target_recovery_time_option
+targetRecoveryTimeOption
     : TARGET_RECOVERY_TIME EQ INT (SECONDS | MINUTES)
     ;
 
 termination
     : ROLLBACK AFTER seconds = INT
     | ROLLBACK IMMEDIATE
     | NO_WAIT
     ;
 
 // https://msdn.microsoft.com/en-us/library/ms176118.aspx
-drop_index
+dropIndex
     : DROP INDEX (IF EXISTS)? (
-        drop_relational_or_xml_or_spatial_index (COMMA drop_relational_or_xml_or_spatial_index)*
-        | drop_backward_compatible_index (COMMA drop_backward_compatible_index)*
+        dropRelationalOrXmlOrSpatialIndex (COMMA dropRelationalOrXmlOrSpatialIndex)*
+        | dropBackwardCompatibleIndex (COMMA dropBackwardCompatibleIndex)*
     ) SEMI?
     ;
 
-drop_relational_or_xml_or_spatial_index
-    : index_name = id_ ON full_table_name
+dropRelationalOrXmlOrSpatialIndex
+    : indexName = id ON tableName
     ;
 
-drop_backward_compatible_index
-    : (owner_name = id_ DOT)? table_or_view_name = id_ DOT index_name = id_
+dropBackwardCompatibleIndex
+    : (ownerName = id DOT)? tableOrViewName = id DOT indexName = id
     ;
 
 // https://msdn.microsoft.com/en-us/library/ms174969.aspx
-drop_procedure
-    : DROP proc = (PROC | PROCEDURE) (IF EXISTS)? func_proc_name_schema (COMMA func_proc_name_schema)* SEMI?
+dropProcedure
+    : DROP proc = (PROC | PROCEDURE) (IF EXISTS)? funcProcNameSchema (COMMA funcProcNameSchema)* SEMI?
     ;
 
 // https://docs.microsoft.com/en-us/sql/t-sql/statements/drop-trigger-transact-sql
-drop_trigger
-    : drop_dml_trigger
-    | drop_ddl_trigger
+dropTrigger
+    : dropDmlTrigger
+    | dropDdlTrigger
     ;
 
-drop_dml_trigger
-    : DROP TRIGGER (IF EXISTS)? simple_name (COMMA simple_name)* SEMI?
+dropDmlTrigger
+    : DROP TRIGGER (IF EXISTS)? simpleName (COMMA simpleName)* SEMI?
     ;
 
-drop_ddl_trigger
-    : DROP TRIGGER (IF EXISTS)? simple_name (COMMA simple_name)* ON (DATABASE | ALL SERVER) SEMI?
+dropDdlTrigger
+    : DROP TRIGGER (IF EXISTS)? simpleName (COMMA simpleName)* ON (DATABASE | ALL SERVER) SEMI?
     ;
 
 // https://msdn.microsoft.com/en-us/library/ms190290.aspx
-drop_function
-    : DROP FUNCTION (IF EXISTS)? func_proc_name_schema (COMMA func_proc_name_schema)* SEMI?
+dropFunction
+    : DROP FUNCTION (IF EXISTS)? funcProcNameSchema (COMMA funcProcNameSchema)* SEMI?
     ;
 
 // https://msdn.microsoft.com/en-us/library/ms175075.aspx
-drop_statistics
-    : DROP STATISTICS (COMMA? (table_name DOT)? name = id_)+ SEMI
+dropStatistics
+    : DROP STATISTICS (COMMA? (tableName DOT)? name = id)+ SEMI
     ;
 
 // https://msdn.microsoft.com/en-us/library/ms173790.aspx
-drop_table
-    : DROP TABLE (IF EXISTS)? table_name (COMMA table_name)* SEMI?
+dropTable
+    : DROP TABLE (IF EXISTS)? tableName (COMMA tableName)* SEMI?
     ;
 
 // https://msdn.microsoft.com/en-us/library/ms173492.aspx
-drop_view
-    : DROP VIEW (IF EXISTS)? simple_name (COMMA simple_name)* SEMI?
+dropView
+    : DROP VIEW (IF EXISTS)? simpleName (COMMA simpleName)* SEMI?
     ;
 
-create_type
-    : CREATE TYPE name = simple_name (FROM data_type null_notnull?)? (
-        AS TABLE LPAREN column_def_table_constraints RPAREN
+createType
+    : CREATE TYPE name = simpleName (FROM dataType nullNotnull?)? (
+        AS TABLE LPAREN columnDefTableConstraints RPAREN
     )?
     ;
 
-drop_type
-    : DROP TYPE (IF EXISTS)? name = simple_name
+dropType
+    : DROP TYPE (IF EXISTS)? name = simpleName
     ;
 
-rowset_function_limited
+rowsetFunctionLimited
     : openquery
     | opendatasource
     ;
 
 // https://msdn.microsoft.com/en-us/library/ms188427(v=sql.120).aspx
 openquery
-    : OPENQUERY LPAREN linked_server = id_ COMMA query = STRING RPAREN
+    : OPENQUERY LPAREN linkedServer = id COMMA query = STRING RPAREN
     ;
 
 // https://msdn.microsoft.com/en-us/library/ms179856.aspx
 opendatasource
-    : OPENDATASOURCE LPAREN provider = STRING COMMA init = STRING RPAREN DOT (database = id_)? DOT (
-        scheme = id_
-    )? DOT (table = id_)
+    : OPENDATASOURCE LPAREN provider = STRING COMMA init = STRING RPAREN DOT (database = id)? DOT (
+        scheme = id
+    )? DOT (table = id)
     ;
 
 // Other statements.
 
 // https://msdn.microsoft.com/en-us/library/ms188927.aspx
-declare_statement
-    : DECLARE LOCAL_ID AS? (data_type | table_type_definition | table_name)
-    | DECLARE loc += declare_local (COMMA loc += declare_local)*
-    | DECLARE LOCAL_ID AS? xml_type_definition
-    | WITH XMLNAMESPACES LPAREN xml_dec += xml_declaration (COMMA xml_dec += xml_declaration)* RPAREN
+declareStatement
+    : DECLARE LOCAL_ID AS? (dataType | tableTypeDefinition | tableName)
+    | DECLARE loc += declareLocal (COMMA loc += declareLocal)*
+    | DECLARE LOCAL_ID AS? xmlTypeDefinition
+    | WITH XMLNAMESPACES LPAREN xmlDec += xmlDeclaration (COMMA xmlDec += xmlDeclaration)* RPAREN
     ;
 
-xml_declaration
-    : xml_namespace_uri = STRING AS id_
+xmlDeclaration
+    : xmlNamespaceUri = STRING AS id
     | DEFAULT STRING
     ;
 
 // https://msdn.microsoft.com/en-us/library/ms181441(v=sql.120).aspx
-cursor_statement
+cursorStatement
     // https://msdn.microsoft.com/en-us/library/ms175035(v=sql.120).aspx
-    : CLOSE GLOBAL? cursor_name SEMI?
+    : CLOSE GLOBAL? cursorName SEMI?
     // https://msdn.microsoft.com/en-us/library/ms188782(v=sql.120).aspx
-    | DEALLOCATE GLOBAL? CURSOR? cursor_name SEMI?
+    | DEALLOCATE GLOBAL? CURSOR? cursorName SEMI?
     // https://msdn.microsoft.com/en-us/library/ms180169(v=sql.120).aspx
-    | declare_cursor
+    | declareCursor
     // https://msdn.microsoft.com/en-us/library/ms180152(v=sql.120).aspx
-    | fetch_cursor
+    | fetchCursor
     // https://msdn.microsoft.com/en-us/library/ms190500(v=sql.120).aspx
-    | OPEN GLOBAL? cursor_name SEMI?
+    | OPEN GLOBAL? cursorName SEMI?
     ;
 
 // https://docs.microsoft.com/en-us/sql/t-sql/statements/backup-transact-sql
-backup_database
-    : BACKUP DATABASE (database_name = id_) (
-        READ_WRITE_FILEGROUPS (COMMA? (FILE | FILEGROUP) EQ file_or_filegroup = STRING)*
-    )? (COMMA? (FILE | FILEGROUP) EQ file_or_filegroup = STRING)* (
-        TO ( COMMA? logical_device_name = id_)+
-        | TO ( COMMA? (DISK | TAPE | URL) EQ (STRING | id_))+
+backupDatabase
+    : BACKUP DATABASE (databaseName = id) (
+        READ_WRITE_FILEGROUPS (COMMA? (FILE | FILEGROUP) EQ fileOrFilegroup = STRING)*
+    )? (COMMA? (FILE | FILEGROUP) EQ fileOrFilegroup = STRING)* (
+        TO ( COMMA? logicalDeviceName = id)+
+        | TO ( COMMA? (DISK | TAPE | URL) EQ (STRING | id))+
     ) (
-        (MIRROR TO ( COMMA? logical_device_name = id_)+)+
-        | ( MIRROR TO ( COMMA? (DISK | TAPE | URL) EQ (STRING | id_))+)+
+        (MIRROR TO ( COMMA? logicalDeviceName = id)+)+
+        | ( MIRROR TO ( COMMA? (DISK | TAPE | URL) EQ (STRING | id))+)+
     )? (
         WITH (
             COMMA? DIFFERENTIAL
             | COMMA? COPY_ONLY
             | COMMA? (COMPRESSION | NO_COMPRESSION)
-            | COMMA? DESCRIPTION EQ (STRING | id_)
-            | COMMA? NAME EQ backup_set_name = id_
+            | COMMA? DESCRIPTION EQ (STRING | id)
+            | COMMA? NAME EQ backupSetName = id
             | COMMA? CREDENTIAL
             | COMMA? FILE_SNAPSHOT
-            | COMMA? (EXPIREDATE EQ (STRING | id_) | RETAINDAYS EQ (INT | id_))
+            | COMMA? (EXPIREDATE EQ (STRING | id) | RETAINDAYS EQ (INT | id))
             | COMMA? (NOINIT | INIT)
             | COMMA? (NOSKIP | SKIP_KEYWORD)
             | COMMA? (NOFORMAT | FORMAT)
-            | COMMA? MEDIADESCRIPTION EQ (STRING | id_)
+            | COMMA? MEDIADESCRIPTION EQ (STRING | id)
             | COMMA? MEDIANAME EQ (medianame = STRING)
-            | COMMA? BLOCKSIZE EQ (INT | id_)
-            | COMMA? BUFFERCOUNT EQ (INT | id_)
-            | COMMA? MAXTRANSFER EQ (INT | id_)
+            | COMMA? BLOCKSIZE EQ (INT | id)
+            | COMMA? BUFFERCOUNT EQ (INT | id)
+            | COMMA? MAXTRANSFER EQ (INT | id)
             | COMMA? (NO_CHECKSUM | CHECKSUM)
             | COMMA? (STOP_ON_ERROR | CONTINUE_AFTER_ERROR)
             | COMMA? RESTART
-            | COMMA? STATS (EQ stats_percent = INT)?
+            | COMMA? STATS (EQ statsPercent = INT)?
             | COMMA? (REWIND | NOREWIND)
             | COMMA? (LOAD | NOUNLOAD)
             | COMMA? ENCRYPTION LPAREN ALGORITHM EQ (
                 AES_128
                 | AES_192
                 | AES_256
                 | TRIPLE_DES_3KEY
             ) COMMA SERVER CERTIFICATE EQ (
-                encryptor_name = id_
-                | SERVER ASYMMETRIC KEY EQ encryptor_name = id_
+                encryptorName = id
+                | SERVER ASYMMETRIC KEY EQ encryptorName = id
             )
         )*
     )?
     ;
 
-backup_log
-    : BACKUP LOG (database_name = id_) (
-        TO ( COMMA? logical_device_name = id_)+
-        | TO ( COMMA? (DISK | TAPE | URL) EQ (STRING | id_))+
+backupLog
+    : BACKUP LOG (databaseName = id) (
+        TO ( COMMA? logicalDeviceName = id)+
+        | TO ( COMMA? (DISK | TAPE | URL) EQ (STRING | id))+
     ) (
-        (MIRROR TO ( COMMA? logical_device_name = id_)+)+
-        | ( MIRROR TO ( COMMA? (DISK | TAPE | URL) EQ (STRING | id_))+)+
+        (MIRROR TO ( COMMA? logicalDeviceName = id)+)+
+        | ( MIRROR TO ( COMMA? (DISK | TAPE | URL) EQ (STRING | id))+)+
     )? (
         WITH (
             COMMA? DIFFERENTIAL
             | COMMA? COPY_ONLY
             | COMMA? (COMPRESSION | NO_COMPRESSION)
-            | COMMA? DESCRIPTION EQ (STRING | id_)
-            | COMMA? NAME EQ backup_set_name = id_
+            | COMMA? DESCRIPTION EQ (STRING | id)
+            | COMMA? NAME EQ backupSetName = id
             | COMMA? CREDENTIAL
             | COMMA? FILE_SNAPSHOT
-            | COMMA? (EXPIREDATE EQ (STRING | id_) | RETAINDAYS EQ (INT | id_))
+            | COMMA? (EXPIREDATE EQ (STRING | id) | RETAINDAYS EQ (INT | id))
             | COMMA? (NOINIT | INIT)
             | COMMA? (NOSKIP | SKIP_KEYWORD)
             | COMMA? (NOFORMAT | FORMAT)
-            | COMMA? MEDIADESCRIPTION EQ (STRING | id_)
+            | COMMA? MEDIADESCRIPTION EQ (STRING | id)
             | COMMA? MEDIANAME EQ (medianame = STRING)
-            | COMMA? BLOCKSIZE EQ (INT | id_)
-            | COMMA? BUFFERCOUNT EQ (INT | id_)
-            | COMMA? MAXTRANSFER EQ (INT | id_)
+            | COMMA? BLOCKSIZE EQ (INT | id)
+            | COMMA? BUFFERCOUNT EQ (INT | id)
+            | COMMA? MAXTRANSFER EQ (INT | id)
             | COMMA? (NO_CHECKSUM | CHECKSUM)
             | COMMA? (STOP_ON_ERROR | CONTINUE_AFTER_ERROR)
             | COMMA? RESTART
-            | COMMA? STATS (EQ stats_percent = INT)?
+            | COMMA? STATS (EQ statsPercent = INT)?
             | COMMA? (REWIND | NOREWIND)
             | COMMA? (LOAD | NOUNLOAD)
-            | COMMA? (NORECOVERY | STANDBY EQ undo_file_name = STRING)
+            | COMMA? (NORECOVERY | STANDBY EQ undoFileName = STRING)
             | COMMA? NO_TRUNCATE
             | COMMA? ENCRYPTION LPAREN ALGORITHM EQ (
                 AES_128
                 | AES_192
                 | AES_256
                 | TRIPLE_DES_3KEY
             ) COMMA SERVER CERTIFICATE EQ (
-                encryptor_name = id_
-                | SERVER ASYMMETRIC KEY EQ encryptor_name = id_
+                encryptorName = id
+                | SERVER ASYMMETRIC KEY EQ encryptorName = id
             )
         )*
     )?
     ;
 
 // https://docs.microsoft.com/en-us/sql/t-sql/statements/backup-certificate-transact-sql
-backup_certificate
-    : BACKUP CERTIFICATE certname = id_ TO FILE EQ cert_file = STRING (
+backupCertificate
+    : BACKUP CERTIFICATE certname = id TO FILE EQ certFile = STRING (
         WITH PRIVATE KEY LPAREN (
-            COMMA? FILE EQ private_key_file = STRING
-            | COMMA? ENCRYPTION BY PASSWORD EQ encryption_password = STRING
-            | COMMA? DECRYPTION BY PASSWORD EQ decryption_pasword = STRING
+            COMMA? FILE EQ privateKeyFile = STRING
+            | COMMA? ENCRYPTION BY PASSWORD EQ encryptionPassword = STRING
+            | COMMA? DECRYPTION BY PASSWORD EQ decryptionPasword = STRING
         )+ RPAREN
     )?
     ;
 
 // https://docs.microsoft.com/en-us/sql/t-sql/statements/backup-master-key-transact-sql
-backup_master_key
-    : BACKUP MASTER KEY TO FILE EQ master_key_backup_file = STRING ENCRYPTION BY PASSWORD EQ encryption_password = STRING
+backupMasterKey
+    : BACKUP MASTER KEY TO FILE EQ masterKeyBackupFile = STRING ENCRYPTION BY PASSWORD EQ encryptionPassword = STRING
     ;
 
 // https://docs.microsoft.com/en-us/sql/t-sql/statements/backup-service-master-key-transact-sql
-backup_service_master_key
-    : BACKUP SERVICE MASTER KEY TO FILE EQ service_master_key_backup_file = STRING ENCRYPTION BY PASSWORD EQ encryption_password = STRING
+backupServiceMasterKey
+    : BACKUP SERVICE MASTER KEY TO FILE EQ serviceMasterKeyBackupFile = STRING ENCRYPTION BY PASSWORD EQ encryptionPassword = STRING
     ;
 
-kill_statement
-    : KILL (kill_process | kill_query_notification | kill_stats_job)
+killStatement
+    : KILL (killProcess | killQueryNotification | killStatsJob)
     ;
 
 // https://docs.microsoft.com/en-us/sql/t-sql/language-elements/kill-transact-sql
-kill_process
-    : (session_id = (INT | STRING) | UOW) (WITH STATUSONLY)?
+killProcess
+    : (sessionId = (INT | STRING) | UOW) (WITH STATUSONLY)?
     ;
 
 // https://docs.microsoft.com/en-us/sql/t-sql/language-elements/kill-query-notification-subscription-transact-sql
-kill_query_notification
-    : QUERY NOTIFICATION SUBSCRIPTION (ALL | subscription_id = INT)
+killQueryNotification
+    : QUERY NOTIFICATION SUBSCRIPTION (ALL | subscriptionId = INT)
     ;
 
 // https://docs.microsoft.com/en-us/sql/t-sql/language-elements/kill-stats-job-transact-sql
-kill_stats_job
-    : STATS JOB job_id = INT
+killStatsJob
+    : STATS JOB jobId = INT
     ;
 
 // https://msdn.microsoft.com/en-us/library/ms188332.aspx
-execute_statement
-    : EXECUTE execute_body SEMI?
+executeStatement
+    : EXECUTE executeBody SEMI?
     ;
 
-execute_body_batch
-    : func_proc_name_server_database_schema (execute_statement_arg (COMMA execute_statement_arg)*)? SEMI?
+executeBodyBatch
+    : funcProcNameServerDatabaseSchema (executeStatementArg (COMMA executeStatementArg)*)? SEMI?
     ;
 
 //https://docs.microsoft.com/it-it/sql/t-sql/language-elements/execute-transact-sql?view=sql-server-ver15
-execute_body
-    : (return_status = LOCAL_ID EQ)? (func_proc_name_server_database_schema | execute_var_string) execute_statement_arg?
-    | LPAREN execute_var_string (COMMA execute_var_string)* RPAREN (AS (LOGIN | USER) EQ STRING)? (
-        AT_KEYWORD linkedServer = id_
+executeBody
+    : (returnStatus = LOCAL_ID EQ)? (funcProcNameServerDatabaseSchema | executeVarString) executeStatementArg?
+    | LPAREN executeVarString (COMMA executeVarString)* RPAREN (AS (LOGIN | USER) EQ STRING)? (
+        AT_KEYWORD linkedServer = id
     )?
     | AS ( (LOGIN | USER) EQ STRING | CALLER)
     ;
 
-execute_statement_arg
-    : execute_statement_arg_unnamed (COMMA execute_statement_arg)*     //Unnamed params can continue unnamed
-    | execute_statement_arg_named (COMMA execute_statement_arg_named)* //Named can only be continued by unnamed
+executeStatementArg
+    : executeStatementArgUnnamed (COMMA executeStatementArg)*     //Unnamed params can continue unnamed
+    | executeStatementArgNamed (COMMA executeStatementArgNamed)* //Named can only be continued by unnamed
     ;
 
-execute_statement_arg_named
-    : name = LOCAL_ID EQ value = execute_parameter
+executeStatementArgNamed
+    : name = LOCAL_ID EQ value = executeParameter
     ;
 
-execute_statement_arg_unnamed
-    : value = execute_parameter
+executeStatementArgUnnamed
+    : value = executeParameter
     ;
 
-execute_parameter
-    : (constant | LOCAL_ID (OUTPUT | OUT)? | id_ | DEFAULT | NULL_)
+executeParameter
+    : (constant | LOCAL_ID (OUTPUT | OUT)? | id | DEFAULT | NULL_)
     ;
 
-execute_var_string
-    : LOCAL_ID (OUTPUT | OUT)? (PLUS LOCAL_ID (PLUS execute_var_string)?)?
-    | STRING (PLUS LOCAL_ID (PLUS execute_var_string)?)?
+executeVarString
+    : LOCAL_ID (OUTPUT | OUT)? (PLUS LOCAL_ID (PLUS executeVarString)?)?
+    | STRING (PLUS LOCAL_ID (PLUS executeVarString)?)?
     ;
 
 // https://msdn.microsoft.com/en-us/library/ff848791.aspx
-security_statement
+securityStatement
     // https://msdn.microsoft.com/en-us/library/ms188354.aspx
-    : execute_clause SEMI?
+    : executeClause SEMI?
     // https://msdn.microsoft.com/en-us/library/ms187965.aspx
-    | GRANT (ALL PRIVILEGES? | grant_permission (LPAREN column_name_list RPAREN)?) (
-        ON (class_type_for_grant COLON COLON)? on_id = table_name
-    )? TO to_principal += principal_id (COMMA to_principal += principal_id)* (WITH GRANT OPTION)? (
-        AS as_principal = principal_id
+    | GRANT (ALL PRIVILEGES? | grantPermission (LPAREN columnNameList RPAREN)?) (
+        ON (classTypeForGrant COLON COLON)? onId = tableName
+    )? TO toPrincipal += principalId (COMMA toPrincipal += principalId)* (WITH GRANT OPTION)? (
+        AS asPrincipal = principalId
     )? SEMI?
     // https://msdn.microsoft.com/en-us/library/ms178632.aspx
     | REVERT (WITH COOKIE EQ LOCAL_ID)? SEMI?
-    | open_key
-    | close_key
-    | create_key
-    | create_certificate
+    | openKey
+    | closeKey
+    | createKey
+    | createCertificate
     ;
 
-principal_id
-    : id_
+principalId
+    : id
     | PUBLIC
     ;
 
-create_certificate
-    : CREATE CERTIFICATE certificate_name = id_ (AUTHORIZATION user_name = id_)? (
-        FROM existing_keys
-        | generate_new_keys
-    ) (ACTIVE FOR BEGIN DIALOG EQ on_off)?
+createCertificate
+    : CREATE CERTIFICATE certificateName = id (AUTHORIZATION userName = id)? (
+        FROM existingKeys
+        | generateNewKeys
+    ) (ACTIVE FOR BEGIN DIALOG EQ onOff)?
     ;
 
-existing_keys
-    : ASSEMBLY assembly_name = id_
-    | EXECUTABLE? FILE EQ path_to_file = STRING (WITH PRIVATE KEY LPAREN private_key_options RPAREN)?
+existingKeys
+    : ASSEMBLY assemblyName = id
+    | EXECUTABLE? FILE EQ pathToFile = STRING (WITH PRIVATE KEY LPAREN privateKeyOptions RPAREN)?
     ;
 
-private_key_options
+privateKeyOptions
     : (FILE | HEX) EQ path = STRING (
         COMMA (DECRYPTION | ENCRYPTION) BY PASSWORD EQ password = STRING
     )?
     ;
 
-generate_new_keys
-    : (ENCRYPTION BY PASSWORD EQ password = STRING)? WITH SUBJECT EQ certificate_subject_name = STRING (
-        COMMA date_options
+generateNewKeys
+    : (ENCRYPTION BY PASSWORD EQ password = STRING)? WITH SUBJECT EQ certificateSubjectName = STRING (
+        COMMA dateOptions
     )*
     ;
 
-date_options
+dateOptions
     : (START_DATE | EXPIRY_DATE) EQ STRING
     ;
 
-open_key
-    : OPEN SYMMETRIC KEY key_name = id_ DECRYPTION BY decryption_mechanism
+openKey
+    : OPEN SYMMETRIC KEY keyName = id DECRYPTION BY decryptionMechanism
     | OPEN MASTER KEY DECRYPTION BY PASSWORD EQ password = STRING
     ;
 
-close_key
-    : CLOSE SYMMETRIC KEY key_name = id_
+closeKey
+    : CLOSE SYMMETRIC KEY keyName = id
     | CLOSE ALL SYMMETRIC KEYS
     | CLOSE MASTER KEY
     ;
 
-create_key
+createKey
     : CREATE MASTER KEY ENCRYPTION BY PASSWORD EQ password = STRING
-    | CREATE SYMMETRIC KEY key_name = id_ (AUTHORIZATION user_name = id_)? (
-        FROM PROVIDER provider_name = id_
-    )? WITH ((key_options | ENCRYPTION BY encryption_mechanism) COMMA?)+
+    | CREATE SYMMETRIC KEY keyName = id (AUTHORIZATION userName = id)? (
+        FROM PROVIDER providerName = id
+    )? WITH ((keyOptions | ENCRYPTION BY encryptionMechanism) COMMA?)+
     ;
 
-key_options
-    : KEY_SOURCE EQ pass_phrase = STRING
+keyOptions
+    : KEY_SOURCE EQ passPhrase = STRING
     | ALGORITHM EQ algorithm
-    | IDENTITY_VALUE EQ identity_phrase = STRING
-    | PROVIDER_KEY_NAME EQ key_name_in_provider = STRING
+    | IDENTITY_VALUE EQ identityPhrase = STRING
+    | PROVIDER_KEY_NAME EQ keyNameInProvider = STRING
     | CREATION_DISPOSITION EQ (CREATE_NEW | OPEN_EXISTING)
     ;
 
 algorithm
     : DES
     | TRIPLE_DES
     | TRIPLE_DES_3KEY
@@ -3255,33 +3254,33 @@
     | RC4_128
     | DESX
     | AES_128
     | AES_192
     | AES_256
     ;
 
-encryption_mechanism
-    : CERTIFICATE certificate_name = id_
-    | ASYMMETRIC KEY asym_key_name = id_
-    | SYMMETRIC KEY decrypting_Key_name = id_
+encryptionMechanism
+    : CERTIFICATE certificateName = id
+    | ASYMMETRIC KEY asymKeyName = id
+    | SYMMETRIC KEY decrypting_KeyName = id
     | PASSWORD EQ STRING
     ;
 
-decryption_mechanism
-    : CERTIFICATE certificate_name = id_ (WITH PASSWORD EQ STRING)?
-    | ASYMMETRIC KEY asym_key_name = id_ (WITH PASSWORD EQ STRING)?
-    | SYMMETRIC KEY decrypting_Key_name = id_
+decryptionMechanism
+    : CERTIFICATE certificateName = id (WITH PASSWORD EQ STRING)?
+    | ASYMMETRIC KEY asymKeyName = id (WITH PASSWORD EQ STRING)?
+    | SYMMETRIC KEY decrypting_KeyName = id
     | PASSWORD EQ STRING
     ;
 
 // https://docs.microsoft.com/en-us/sql/relational-databases/system-functions/sys-fn-builtin-permissions-transact-sql?view=sql-server-ver15
-// SELECT DISTINCT '| ' + permission_name
-// FROM sys.fn_builtin_permissions (DEFAULT)
+// SELECT DISTINCT '| ' + permissionName
+// FROM sys.fnBuiltinPermissions (DEFAULT)
 // ORDER BY 1
-grant_permission
+grantPermission
     : ADMINISTER (BULK OPERATIONS | DATABASE BULK OPERATIONS)
     | ALTER (
         ANY (
             APPLICATION ROLE
             | ASSEMBLY
             | ASYMMETRIC KEY
             | AVAILABILITY GROUP
@@ -3383,484 +3382,484 @@
         | DEFINITION
         | SERVER STATE
     )
     ;
 
 // https://msdn.microsoft.com/en-us/library/ms190356.aspx
 // https://msdn.microsoft.com/en-us/library/ms189484.aspx
-set_statement
-    : SET LOCAL_ID (DOT member_name = id_)? EQ expression
-    | SET LOCAL_ID assignment_operator expression
-    | SET LOCAL_ID EQ CURSOR declare_set_cursor_common (
-        FOR (READ ONLY | UPDATE (OF column_name_list)?)
+setStatement
+    : SET LOCAL_ID (DOT memberName = id)? EQ expression
+    | SET LOCAL_ID assignmentOperator expression
+    | SET LOCAL_ID EQ CURSOR declareSetCursorCommon (
+        FOR (READ ONLY | UPDATE (OF columnNameList)?)
     )?
     // https://msdn.microsoft.com/en-us/library/ms189837.aspx
-    | set_special
+    | setSpecial
     ;
 
 // https://msdn.microsoft.com/en-us/library/ms174377.aspx
-transaction_statement
+transactionStatement
     // https://msdn.microsoft.com/en-us/library/ms188386.aspx
-    : BEGIN DISTRIBUTED (TRAN | TRANSACTION) (id_ | LOCAL_ID)?
+    : BEGIN DISTRIBUTED (TRAN | TRANSACTION) (id | LOCAL_ID)?
     // https://msdn.microsoft.com/en-us/library/ms188929.aspx
-    | BEGIN (TRAN | TRANSACTION) ((id_ | LOCAL_ID) (WITH MARK STRING)?)?
+    | BEGIN (TRAN | TRANSACTION) ((id | LOCAL_ID) (WITH MARK STRING)?)?
     // https://msdn.microsoft.com/en-us/library/ms190295.aspx
     | COMMIT (TRAN | TRANSACTION) (
-        (id_ | LOCAL_ID) (WITH LPAREN DELAYED_DURABILITY EQ (OFF | ON) RPAREN)?
+        (id | LOCAL_ID) (WITH LPAREN DELAYED_DURABILITY EQ (OFF | ON) RPAREN)?
     )?
     // https://msdn.microsoft.com/en-us/library/ms178628.aspx
     | COMMIT WORK?
-    | COMMIT id_
-    | ROLLBACK id_
+    | COMMIT id
+    | ROLLBACK id
     // https://msdn.microsoft.com/en-us/library/ms181299.aspx
-    | ROLLBACK (TRAN | TRANSACTION) (id_ | LOCAL_ID)?
+    | ROLLBACK (TRAN | TRANSACTION) (id | LOCAL_ID)?
     // https://msdn.microsoft.com/en-us/library/ms174973.aspx
     | ROLLBACK WORK?
     // https://msdn.microsoft.com/en-us/library/ms188378.aspx
-    | SAVE (TRAN | TRANSACTION) (id_ | LOCAL_ID)?
+    | SAVE (TRAN | TRANSACTION) (id | LOCAL_ID)?
     ;
 
 // https://msdn.microsoft.com/en-us/library/ms188037.aspx
-go_statement
+goStatement
     : GO (count = INT)?
     ;
 
 // https://msdn.microsoft.com/en-us/library/ms188366.aspx
-use_statement
-    : USE database = id_
+useStatement
+    : USE database = id
     ;
 
-setuser_statement
+setuserStatement
     : SETUSER user = STRING?
     ;
 
 // https://docs.microsoft.com/en-us/sql/t-sql/language-elements/reconfigure-transact-sql
-reconfigure_statement
+reconfigureStatement
     : RECONFIGURE (WITH OVERRIDE)?
     ;
 
 // https://docs.microsoft.com/en-us/sql/t-sql/language-elements/shutdown-transact-sql
-shutdown_statement
+shutdownStatement
     : SHUTDOWN (WITH NOWAIT)?
     ;
 
-checkpoint_statement
+checkpointStatement
     : CHECKPOINT (checkPointDuration = INT)?
     ;
 
-dbcc_checkalloc_option
+dbccCheckallocOption
     : ALL_ERRORMSGS
     | NO_INFOMSGS
     | TABLOCK
     | ESTIMATEONLY
     ;
 
 // https://learn.microsoft.com/en-us/sql/t-sql/database-console-commands/dbcc-checkalloc-transact-sql?view=sql-server-ver16
-dbcc_checkalloc
+dbccCheckalloc
     : name = CHECKALLOC (
-        LPAREN (database = id_ | databaseid = STRING | INT) (
+        LPAREN (database = id | databaseid = STRING | INT) (
             COMMA NOINDEX
             | COMMA ( REPAIR_ALLOW_DATA_LOSS | REPAIR_FAST | REPAIR_REBUILD)
         )? RPAREN (
-            WITH dbcc_option = dbcc_checkalloc_option (COMMA dbcc_option = dbcc_checkalloc_option)*
+            WITH dbccOption = dbccCheckallocOption (COMMA dbccOption = dbccCheckallocOption)*
         )?
     )?
     ;
 
 // https://learn.microsoft.com/en-us/sql/t-sql/database-console-commands/dbcc-checkcatalog-transact-sql?view=sql-server-ver16
-dbcc_checkcatalog
-    : name = CHECKCATALOG (LPAREN ( database = id_ | databasename = STRING | INT) RPAREN)? (
-        WITH dbcc_option = NO_INFOMSGS
+dbccCheckcatalog
+    : name = CHECKCATALOG (LPAREN ( database = id | databasename = STRING | INT) RPAREN)? (
+        WITH dbccOption = NO_INFOMSGS
     )?
     ;
 
-dbcc_checkconstraints_option
+dbccCheckconstraintsOption
     : ALL_CONSTRAINTS
     | ALL_ERRORMSGS
     | NO_INFOMSGS
     ;
 
 // https://learn.microsoft.com/en-us/sql/t-sql/database-console-commands/dbcc-checkconstraints-transact-sql?view=sql-server-ver16
-dbcc_checkconstraints
+dbccCheckconstraints
     : name = CHECKCONSTRAINTS (
-        LPAREN (table_or_constraint = id_ | table_or_constraint_name = STRING) RPAREN
+        LPAREN (tableOrConstraint = id | tableOrConstraintName = STRING) RPAREN
     )? (
-        WITH dbcc_option = dbcc_checkconstraints_option (
-            COMMA dbcc_option = dbcc_checkconstraints_option
+        WITH dbccOption = dbccCheckconstraintsOption (
+            COMMA dbccOption = dbccCheckconstraintsOption
         )*
     )?
     ;
 
-dbcc_checkdb_table_option
+dbccCheckdbTableOption
     : ALL_ERRORMSGS
     | EXTENDED_LOGICAL_CHECKS
     | NO_INFOMSGS
     | TABLOCK
     | ESTIMATEONLY
     | PHYSICAL_ONLY
     | DATA_PURITY
-    | MAXDOP EQ max_dregree_of_parallelism = INT
+    | MAXDOP EQ maxDregreeOfParallelism = INT
     ;
 
 // https://learn.microsoft.com/en-us/sql/t-sql/database-console-commands/dbcc-checkdb-transact-sql?view=sql-server-ver16
-dbcc_checkdb
+dbccCheckdb
     : name = CHECKDB (
-        LPAREN (database = id_ | databasename = STRING | INT) (
+        LPAREN (database = id | databasename = STRING | INT) (
             COMMA (NOINDEX | REPAIR_ALLOW_DATA_LOSS | REPAIR_FAST | REPAIR_REBUILD)
         )? RPAREN
     )? (
-        WITH dbcc_option = dbcc_checkdb_table_option (COMMA dbcc_option = dbcc_checkdb_table_option)*
+        WITH dbccOption = dbccCheckdbTableOption (COMMA dbccOption = dbccCheckdbTableOption)*
     )?
     ;
 
-dbcc_checkfilegroup_option
+dbccCheckfilegroupOption
     : ALL_ERRORMSGS
     | NO_INFOMSGS
     | TABLOCK
     | ESTIMATEONLY
     | PHYSICAL_ONLY
-    | MAXDOP EQ max_dregree_of_parallelism = INT
+    | MAXDOP EQ maxDregreeOfParallelism = INT
     ;
 
 // https://learn.microsoft.com/en-us/sql/t-sql/database-console-commands/dbcc-checkfilegroup-transact-sql?view=sql-server-ver16
 // Additional parameters: https://dbtut.com/index.php/2019/01/01/dbcc-checkfilegroup-command-on-sql-server/
-dbcc_checkfilegroup
+dbccCheckfilegroup
     : name = CHECKFILEGROUP (
-        LPAREN (filegroup_id = INT | filegroup_name = STRING) (
+        LPAREN (filegroupId = INT | filegroupName = STRING) (
             COMMA (NOINDEX | REPAIR_ALLOW_DATA_LOSS | REPAIR_FAST | REPAIR_REBUILD)
         )? RPAREN
     )? (
-        WITH dbcc_option = dbcc_checkfilegroup_option (
-            COMMA dbcc_option = dbcc_checkfilegroup_option
+        WITH dbccOption = dbccCheckfilegroupOption (
+            COMMA dbccOption = dbccCheckfilegroupOption
         )*
     )?
     ;
 
 // https://learn.microsoft.com/en-us/sql/t-sql/database-console-commands/dbcc-checktable-transact-sql?view=sql-server-ver16
-dbcc_checktable
-    : name = CHECKTABLE LPAREN table_or_view_name = STRING (
+dbccChecktable
+    : name = CHECKTABLE LPAREN tableOrViewName = STRING (
         COMMA (
             NOINDEX
-            | index_id = expression
+            | indexId = expression
             | REPAIR_ALLOW_DATA_LOSS
             | REPAIR_FAST
             | REPAIR_REBUILD
         )
     )? RPAREN (
-        WITH dbcc_option = dbcc_checkdb_table_option (COMMA dbcc_option = dbcc_checkdb_table_option)*
+        WITH dbccOption = dbccCheckdbTableOption (COMMA dbccOption = dbccCheckdbTableOption)*
     )?
     ;
 
 // https://learn.microsoft.com/en-us/sql/t-sql/database-console-commands/dbcc-cleantable-transact-sql?view=sql-server-ver16
-dbcc_cleantable
-    : name = CLEANTABLE LPAREN (database = id_ | databasename = STRING | INT) COMMA (
-        table_or_view = id_
-        | table_or_view_name = STRING
-    ) (COMMA batch_size = INT)? RPAREN (WITH dbcc_option = NO_INFOMSGS)?
+dbccCleantable
+    : name = CLEANTABLE LPAREN (database = id | databasename = STRING | INT) COMMA (
+        tableOrView = id
+        | tableOrViewName = STRING
+    ) (COMMA batchSize = INT)? RPAREN (WITH dbccOption = NO_INFOMSGS)?
     ;
 
-dbcc_clonedatabase_option
+dbccClonedatabaseOption
     : NO_STATISTICS
     | NO_QUERYSTORE
     | SERVICEBROKER
     | VERIFY_CLONEDB
     | BACKUP_CLONEDB
     ;
 
 // https://learn.microsoft.com/en-us/sql/t-sql/database-console-commands/dbcc-clonedatabase-transact-sql?view=sql-server-ver16
-dbcc_clonedatabase
-    : name = CLONEDATABASE LPAREN source_database = id_ COMMA target_database = id_ RPAREN (
-        WITH dbcc_option = dbcc_clonedatabase_option (COMMA dbcc_option = dbcc_clonedatabase_option)*
+dbccClonedatabase
+    : name = CLONEDATABASE LPAREN sourceDatabase = id COMMA targetDatabase = id RPAREN (
+        WITH dbccOption = dbccClonedatabaseOption (COMMA dbccOption = dbccClonedatabaseOption)*
     )?
     ;
 
 // https://learn.microsoft.com/en-us/sql/t-sql/database-console-commands/dbcc-pdw-showspaceused-transact-sql?view=aps-pdw-2016-au7
-dbcc_pdw_showspaceused
-    : name = PDW_SHOWSPACEUSED (LPAREN tablename = id_ RPAREN)? (
-        WITH dbcc_option = IGNORE_REPLICATED_TABLE_CACHE
+dbccPdwShowspaceused
+    : name = PDW_SHOWSPACEUSED (LPAREN tablename = id RPAREN)? (
+        WITH dbccOption = IGNORE_REPLICATED_TABLE_CACHE
     )?
     ;
 
 // https://learn.microsoft.com/en-us/sql/t-sql/database-console-commands/dbcc-proccache-transact-sql?view=sql-server-ver16
-dbcc_proccache
-    : name = PROCCACHE (WITH dbcc_option = NO_INFOMSGS)?
+dbccProccache
+    : name = PROCCACHE (WITH dbccOption = NO_INFOMSGS)?
     ;
 
-dbcc_showcontig_option
+dbccShowcontigOption
     : ALL_INDEXES
     | TABLERESULTS
     | FAST
     | ALL_LEVELS
     | NO_INFOMSGS
     ;
 
 // https://learn.microsoft.com/en-us/sql/t-sql/database-console-commands/dbcc-showcontig-transact-sql?view=sql-server-ver16
-dbcc_showcontig
-    : name = SHOWCONTIG (LPAREN table_or_view = expression ( COMMA index = expression)? RPAREN)? (
-        WITH dbcc_option = dbcc_showcontig_option (COMMA dbcc_showcontig_option)*
+dbccShowcontig
+    : name = SHOWCONTIG (LPAREN tableOrView = expression ( COMMA index = expression)? RPAREN)? (
+        WITH dbccOption = dbccShowcontigOption (COMMA dbccShowcontigOption)*
     )?
     ;
 
 // https://learn.microsoft.com/en-us/sql/t-sql/database-console-commands/dbcc-shrinklog-azure-sql-data-warehouse?view=aps-pdw-2016-au7
-dbcc_shrinklog
+dbccShrinklog
     : name = SHRINKLOG (LPAREN SIZE EQ ( (INT ( MB | GB | TB)) | DEFAULT) RPAREN)? (
-        WITH dbcc_option = NO_INFOMSGS
+        WITH dbccOption = NO_INFOMSGS
     )?
     ;
 
 // https://learn.microsoft.com/en-us/sql/t-sql/database-console-commands/dbcc-dbreindex-transact-sql?view=sql-server-ver16
-dbcc_dbreindex
-    : name = DBREINDEX LPAREN table = id_or_string (
-        COMMA index_name = id_or_string ( COMMA fillfactor = expression)?
-    )? RPAREN (WITH dbcc_option = NO_INFOMSGS)?
+dbccDbreindex
+    : name = DBREINDEX LPAREN table = idOrString (
+        COMMA indexName = idOrString ( COMMA fillfactor = expression)?
+    )? RPAREN (WITH dbccOption = NO_INFOMSGS)?
     ;
 
 // https://learn.microsoft.com/en-us/sql/t-sql/database-console-commands/dbcc-dllname-free-transact-sql?view=sql-server-ver16
-dbcc_dll_free
-    : dllname = id_ LPAREN name = FREE RPAREN (WITH dbcc_option = NO_INFOMSGS)?
+dbccDllFree
+    : dllname = id LPAREN name = FREE RPAREN (WITH dbccOption = NO_INFOMSGS)?
     ;
 
 // https://learn.microsoft.com/en-us/sql/t-sql/database-console-commands/dbcc-dropcleanbuffers-transact-sql?view=sql-server-ver16
-dbcc_dropcleanbuffers
-    : name = DROPCLEANBUFFERS (LPAREN COMPUTE | ALL RPAREN)? (WITH dbcc_option = NO_INFOMSGS)?
+dbccDropcleanbuffers
+    : name = DROPCLEANBUFFERS (LPAREN COMPUTE | ALL RPAREN)? (WITH dbccOption = NO_INFOMSGS)?
     ;
 
-dbcc_clause
+dbccClause
     : DBCC (
-        dbcc_checkalloc
-        | dbcc_checkcatalog
-        | dbcc_checkconstraints
-        | dbcc_checkdb
-        | dbcc_checkfilegroup
-        | dbcc_checktable
-        | dbcc_cleantable
-        | dbcc_clonedatabase
-        | dbcc_dbreindex
-        | dbcc_dll_free
-        | dbcc_dropcleanbuffers
-        | dbcc_pdw_showspaceused
-        | dbcc_proccache
-        | dbcc_showcontig
-        | dbcc_shrinklog
+        dbccCheckalloc
+        | dbccCheckcatalog
+        | dbccCheckconstraints
+        | dbccCheckdb
+        | dbccCheckfilegroup
+        | dbccChecktable
+        | dbccCleantable
+        | dbccClonedatabase
+        | dbccDbreindex
+        | dbccDllFree
+        | dbccDropcleanbuffers
+        | dbccPdwShowspaceused
+        | dbccProccache
+        | dbccShowcontig
+        | dbccShrinklog
     )
     ;
 
-execute_clause
+executeClause
     : EXECUTE AS clause = (CALLER | SELF | OWNER | STRING)
     ;
 
-declare_local
-    : LOCAL_ID AS? data_type (EQ expression)?
+declareLocal
+    : LOCAL_ID AS? dataType (EQ expression)?
     ;
 
-table_type_definition
-    : TABLE LPAREN column_def_table_constraints (COMMA? table_type_indices)* RPAREN
+tableTypeDefinition
+    : TABLE LPAREN columnDefTableConstraints (COMMA? tableTypeIndices)* RPAREN
     ;
 
-table_type_indices
-    : (((PRIMARY KEY | INDEX id_) (CLUSTERED | NONCLUSTERED)?) | UNIQUE) LPAREN column_name_list_with_order RPAREN
-    | CHECK LPAREN search_condition RPAREN
+tableTypeIndices
+    : (((PRIMARY KEY | INDEX id) (CLUSTERED | NONCLUSTERED)?) | UNIQUE) LPAREN columnNameListWithOrder RPAREN
+    | CHECK LPAREN searchCondition RPAREN
     ;
 
-xml_type_definition
-    : XML LPAREN (CONTENT | DOCUMENT)? xml_schema_collection RPAREN
+xmlTypeDefinition
+    : XML LPAREN (CONTENT | DOCUMENT)? xmlSchemaCollection RPAREN
     ;
 
-xml_schema_collection
+xmlSchemaCollection
     : ID DOT ID
     ;
 
-column_def_table_constraints
-    : column_def_table_constraint (COMMA? column_def_table_constraint)*
+columnDefTableConstraints
+    : columnDefTableConstraint (COMMA? columnDefTableConstraint)*
     ;
 
-column_def_table_constraint
-    : column_definition
-    | materialized_column_definition
-    | table_constraint
+columnDefTableConstraint
+    : columnDefinition
+    | materializedColumnDefinition
+    | tableConstraint
     ;
 
 // https://msdn.microsoft.com/en-us/library/ms187742.aspx
 // There is a documentation error: column definition elements can be given in
 // any order
-column_definition
-    : id_ (data_type | AS expression PERSISTED?) column_definition_element* column_index?
+columnDefinition
+    : id (dataType | AS expression PERSISTED?) columnDefinitionElement* columnIndex?
     ;
 
-column_definition_element
+columnDefinitionElement
     : FILESTREAM
-    | COLLATE collation_name = id_
+    | COLLATE collationName = id
     | SPARSE
-    | MASKED WITH LPAREN FUNCTION EQ mask_function = STRING RPAREN
-    | (CONSTRAINT constraint = id_)? DEFAULT constant_expr = expression
+    | MASKED WITH LPAREN FUNCTION EQ maskFunction = STRING RPAREN
+    | (CONSTRAINT constraint = id)? DEFAULT constantExpr = expression
     | IDENTITY (LPAREN seed = INT COMMA increment = INT RPAREN)?
     | NOT FOR REPLICATION
     | GENERATED ALWAYS AS (ROW | TRANSACTION_ID | SEQUENCE_NUMBER) (START | END) HIDDEN_KEYWORD?
     // NULL / NOT NULL is a constraint
     | ROWGUIDCOL
-    | ENCRYPTED WITH LPAREN COLUMN_ENCRYPTION_KEY EQ key_name = STRING COMMA ENCRYPTION_TYPE EQ (
+    | ENCRYPTED WITH LPAREN COLUMN_ENCRYPTION_KEY EQ keyName = STRING COMMA ENCRYPTION_TYPE EQ (
         DETERMINISTIC
         | RANDOMIZED
     ) COMMA ALGORITHM EQ algo = STRING RPAREN
-    | column_constraint
+    | columnConstraint
     ;
 
-column_modifier
-    : id_ (ADD | DROP) (
+columnModifier
+    : id (ADD | DROP) (
         ROWGUIDCOL
         | PERSISTED
         | NOT FOR REPLICATION
         | SPARSE
         | HIDDEN_KEYWORD
         | MASKED (WITH (FUNCTION EQ STRING | LPAREN FUNCTION EQ STRING RPAREN))?
     )
     ;
 
-materialized_column_definition
-    : id_ (COMPUTE | AS) expression (MATERIALIZED | NOT MATERIALIZED)?
+materializedColumnDefinition
+    : id (COMPUTE | AS) expression (MATERIALIZED | NOT MATERIALIZED)?
     ;
 
 // https://msdn.microsoft.com/en-us/library/ms186712.aspx
 // There is a documentation error: NOT NULL is a constraint
 // and therefore can be given a name.
-column_constraint
-    : (CONSTRAINT constraint = id_)? (
-        null_notnull
-        | ( (PRIMARY KEY | UNIQUE) clustered? primary_key_options)
-        | ( (FOREIGN KEY)? foreign_key_options)
-        | check_constraint
+columnConstraint
+    : (CONSTRAINT constraint = id)? (
+        nullNotnull
+        | ( (PRIMARY KEY | UNIQUE) clustered? primaryKeyOptions)
+        | ( (FOREIGN KEY)? foreignKeyOptions)
+        | checkConstraint
     )
     ;
 
-column_index
-    : INDEX index_name = id_ clustered? create_table_index_options? on_partition_or_filegroup? (
-        FILESTREAM_ON (filestream_filegroup_or_partition_schema_name = id_ | NULL_DOUBLE_QUOTE)
+columnIndex
+    : INDEX indexName = id clustered? createTableIndexOptions? onPartitionOrFilegroup? (
+        FILESTREAM_ON (filestreamFilegroupOrPartitionSchemaName = id | NULL_DOUBLE_QUOTE)
     )?
     ;
 
-on_partition_or_filegroup
+onPartitionOrFilegroup
     : ON (
-        (partition_scheme_name = id_ LPAREN partition_column_name = id_ RPAREN)
-        | filegroup = id_
+        (partitionSchemeName = id LPAREN partitionColumnName = id RPAREN)
+        | filegroup = id
         | DEFAULT_DOUBLE_QUOTE
     )
     ;
 
 // https://msdn.microsoft.com/en-us/library/ms188066.aspx
-table_constraint
-    : (CONSTRAINT constraint = id_)? (
-        ((PRIMARY KEY | UNIQUE) clustered? LPAREN column_name_list_with_order RPAREN primary_key_options)
-        | ( FOREIGN KEY LPAREN fk = column_name_list RPAREN foreign_key_options)
-        | ( CONNECTION LPAREN connection_node ( COMMA connection_node)* RPAREN)
-        | ( DEFAULT constant_expr = expression FOR column = id_ (WITH VALUES)?)
-        | check_constraint
+tableConstraint
+    : (CONSTRAINT constraint = id)? (
+        ((PRIMARY KEY | UNIQUE) clustered? LPAREN columnNameListWithOrder RPAREN primaryKeyOptions)
+        | ( FOREIGN KEY LPAREN fk = columnNameList RPAREN foreignKeyOptions)
+        | ( CONNECTION LPAREN connectionNode ( COMMA connectionNode)* RPAREN)
+        | ( DEFAULT constantExpr = expression FOR column = id (WITH VALUES)?)
+        | checkConstraint
     )
     ;
 
-connection_node
-    : from_node_table = id_ TO to_node_table = id_
+connectionNode
+    : fromNodeTable = id TO toNodeTable = id
     ;
 
-primary_key_options
-    : (WITH FILLFACTOR EQ INT)? alter_table_index_options? on_partition_or_filegroup?
+primaryKeyOptions
+    : (WITH FILLFACTOR EQ INT)? alterTableIndexOptions? onPartitionOrFilegroup?
     ;
 
-foreign_key_options
-    : REFERENCES table_name LPAREN pk = column_name_list RPAREN (on_delete | on_update)* (
+foreignKeyOptions
+    : REFERENCES tableName LPAREN pk = columnNameList RPAREN (onDelete | onUpdate)* (
         NOT FOR REPLICATION
     )?
     ;
 
-check_constraint
-    : CHECK (NOT FOR REPLICATION)? LPAREN search_condition RPAREN
+checkConstraint
+    : CHECK (NOT FOR REPLICATION)? LPAREN searchCondition RPAREN
     ;
 
-on_delete
+onDelete
     : ON DELETE (NO ACTION | CASCADE | SET NULL_ | SET DEFAULT)
     ;
 
-on_update
+onUpdate
     : ON UPDATE (NO ACTION | CASCADE | SET NULL_ | SET DEFAULT)
     ;
 
-alter_table_index_options
-    : WITH LPAREN alter_table_index_option (COMMA alter_table_index_option)* RPAREN
+alterTableIndexOptions
+    : WITH LPAREN alterTableIndexOption (COMMA alterTableIndexOption)* RPAREN
     ;
 
 // https://msdn.microsoft.com/en-us/library/ms186869.aspx
-alter_table_index_option
-    : PAD_INDEX EQ on_off
+alterTableIndexOption
+    : PAD_INDEX EQ onOff
     | FILLFACTOR EQ INT
-    | IGNORE_DUP_KEY EQ on_off
-    | STATISTICS_NORECOMPUTE EQ on_off
-    | ALLOW_ROW_LOCKS EQ on_off
-    | ALLOW_PAGE_LOCKS EQ on_off
-    | OPTIMIZE_FOR_SEQUENTIAL_KEY EQ on_off
-    | SORT_IN_TEMPDB EQ on_off
-    | MAXDOP EQ max_degree_of_parallelism = INT
-    | DATA_COMPRESSION EQ (NONE | ROW | PAGE | COLUMNSTORE | COLUMNSTORE_ARCHIVE) on_partitions?
-    | XML_COMPRESSION EQ on_off on_partitions?
-    | DISTRIBUTION EQ HASH LPAREN id_ RPAREN
-    | CLUSTERED INDEX LPAREN id_ (ASC | DESC)? (COMMA id_ (ASC | DESC)?)* RPAREN
-    | ONLINE EQ (ON (LPAREN low_priority_lock_wait RPAREN)? | OFF)
-    | RESUMABLE EQ on_off
+    | IGNORE_DUP_KEY EQ onOff
+    | STATISTICS_NORECOMPUTE EQ onOff
+    | ALLOW_ROW_LOCKS EQ onOff
+    | ALLOW_PAGE_LOCKS EQ onOff
+    | OPTIMIZE_FOR_SEQUENTIAL_KEY EQ onOff
+    | SORT_IN_TEMPDB EQ onOff
+    | MAXDOP EQ maxDegreeOfParallelism = INT
+    | DATA_COMPRESSION EQ (NONE | ROW | PAGE | COLUMNSTORE | COLUMNSTORE_ARCHIVE) onPartitions?
+    | XML_COMPRESSION EQ onOff onPartitions?
+    | DISTRIBUTION EQ HASH LPAREN id RPAREN
+    | CLUSTERED INDEX LPAREN id (ASC | DESC)? (COMMA id (ASC | DESC)?)* RPAREN
+    | ONLINE EQ (ON (LPAREN lowPriorityLockWait RPAREN)? | OFF)
+    | RESUMABLE EQ onOff
     | MAX_DURATION EQ times = INT MINUTES?
     ;
 
 // https://msdn.microsoft.com/en-us/library/ms180169.aspx
-declare_cursor
-    : DECLARE cursor_name (
-        CURSOR (declare_set_cursor_common (FOR UPDATE (OF column_name_list)?)?)?
-        | (SEMI_SENSITIVE | INSENSITIVE)? SCROLL? CURSOR FOR select_statement_standalone (
-            FOR (READ ONLY | UPDATE | (OF column_name_list))
+declareCursor
+    : DECLARE cursorName (
+        CURSOR (declareSetCursorCommon (FOR UPDATE (OF columnNameList)?)?)?
+        | (SEMI_SENSITIVE | INSENSITIVE)? SCROLL? CURSOR FOR selectStatementStandalone (
+            FOR (READ ONLY | UPDATE | (OF columnNameList))
         )?
     ) SEMI?
     ;
 
-declare_set_cursor_common
-    : declare_set_cursor_common_partial* FOR select_statement_standalone
+declareSetCursorCommon
+    : declareSetCursorCommonPartial* FOR selectStatementStandalone
     ;
 
-declare_set_cursor_common_partial
+declareSetCursorCommonPartial
     : (LOCAL | GLOBAL)
     | (FORWARD_ONLY | SCROLL)
     | (STATIC | KEYSET | DYNAMIC | FAST_FORWARD)
     | (READ_ONLY | SCROLL_LOCKS | OPTIMISTIC)
     | TYPE_WARNING
     ;
 
-fetch_cursor
-    : FETCH ((NEXT | PRIOR | FIRST | LAST | (ABSOLUTE | RELATIVE) expression)? FROM)? GLOBAL? cursor_name (
+fetchCursor
+    : FETCH ((NEXT | PRIOR | FIRST | LAST | (ABSOLUTE | RELATIVE) expression)? FROM)? GLOBAL? cursorName (
         INTO LOCAL_ID (COMMA LOCAL_ID)*
     )? SEMI?
     ;
 
 // https://msdn.microsoft.com/en-us/library/ms190356.aspx
 // Runtime check.
-set_special
-    : SET id_ (id_ | constant_LOCAL_ID | on_off) SEMI?
-    | SET STATISTICS (IO | TIME | XML | PROFILE) on_off SEMI?
+setSpecial
+    : SET id (id | constant_LOCAL_ID | onOff) SEMI?
+    | SET STATISTICS (IO | TIME | XML | PROFILE) onOff SEMI?
     | SET ROWCOUNT (LOCAL_ID | INT) SEMI?
     | SET TEXTSIZE INT SEMI?
     // https://msdn.microsoft.com/en-us/library/ms173763.aspx
     | SET TRANSACTION ISOLATION LEVEL (
         READ UNCOMMITTED
         | READ COMMITTED
         | REPEATABLE READ
         | SNAPSHOT
         | SERIALIZABLE
         | INT
     ) SEMI?
     // https://msdn.microsoft.com/en-us/library/ms188059.aspx
-    | SET IDENTITY_INSERT table_name on_off SEMI?
-    | SET special_list (COMMA special_list)* on_off
-    | SET modify_method
+    | SET IDENTITY_INSERT tableName onOff SEMI?
+    | SET specialList (COMMA specialList)* onOff
+    // TODO: Rework when it is time to implement SET modifyMethod
     ;
 
-special_list
+specialList
     : ANSI_NULLS
     | QUOTED_IDENTIFIER
     | ANSI_PADDING
     | ANSI_WARNINGS
     | ANSI_DEFAULTS
     | ANSI_NULL_DFLT_OFF
     | ANSI_NULL_DFLT_ON
@@ -3888,1071 +3887,562 @@
     ;
 
 // Expression.
 
 // https://docs.microsoft.com/en-us/sql/t-sql/language-elements/expressions-transact-sql
 // Operator precendence: https://docs.microsoft.com/en-us/sql/t-sql/language-elements/operator-precedence-transact-sql
 expression
-    : LPAREN expression RPAREN #expr_precedence
-    | <assoc=right> op=BIT_NOT expression #expr_bit_not
-    | <assoc=right> op=(PLUS | MINUS) expression #expr_unary
-    | expression op=(STAR | DIV | MOD) expression #expr_op_prec_1
-    | expression op=(PLUS | MINUS) expression #expr_op_prec_2
-    | expression op=(BIT_AND | BIT_XOR | BIT_OR) expression #expr_op_prec_3
-    | expression op=DOUBLE_BAR expression #expr_op_prec_4
-    | primitive_expression #expr_primitive
-    | function_call #expr_func
-    | expression DOT (value_call | query_call | exist_call | modify_call) #expr_dot
-    | expression DOT hierarchyid_call #expr_hierarchyid
-    | expression COLLATE id_ #expr_collate
-    | case_expression #expr_case
-    | full_column_name #expr_full_column
-    | expression time_zone #expr_tz
-    | over_clause #expr_over
-    | DOLLAR_ACTION #expr_dollar
-    | LPAREN subquery RPAREN #expr_subquery
+    : LPAREN expression RPAREN                                  #exprPrecedence
+    | <assoc=right> op=BIT_NOT expression                       #exprBitNot
+    | <assoc=right> op=(PLUS | MINUS) expression                #exprUnary
+    | expression op=(STAR | DIV | MOD) expression               #exprOpPrec1
+    | expression op=(PLUS | MINUS) expression                   #exprOpPrec2
+    | expression op=(BIT_AND | BIT_XOR | BIT_OR) expression     #exprOpPrec3
+    | expression op=DOUBLE_BAR expression                       #exprOpPrec4
+    | primitiveExpression                                       #exprPrimitive
+    | functionCall                                              #exprFunc
+    | expression COLLATE id                                     #exprCollate
+    | caseExpression                                            #exprCase
+    | expression timeZone                                       #exprTz
+    | expression overClause                                     #exprOver
+    | id                                                        #exprId
+    | DOLLAR_ACTION                                             #exprDollar
+    | <assoc=right> expression DOT expression                   #exprDot
+    | LPAREN subquery RPAREN                                    #exprSubquery
+    | ALL expression                                            #exprAll
+    | DISTINCT expression                                       #exprDistinct
+    | STAR                                                      #exprStar
     ;
 
+// TODO: Implement this
 parameter
     : PLACEHOLDER
     ;
 
-time_zone
+timeZone
     : AT_KEYWORD TIME ZONE expression
     ;
 
-primitive_expression
+primitiveExpression
     : DEFAULT
     | NULL_
     | LOCAL_ID
-    | primitive_constant
+    | constant
     ;
 
 // https://docs.microsoft.com/en-us/sql/t-sql/language-elements/case-transact-sql
-case_expression
-    : CASE caseExpr = expression switch_section+ (ELSE elseExpr = expression)? END
-    | CASE switch_search_condition_section+ (ELSE elseExpr = expression)? END
+caseExpression
+    : CASE caseExpr=expression? switchSection+ (ELSE elseExpr = expression)? END
     ;
 
 subquery
-    : select_statement
+    : selectStatement
     ;
 
 // https://msdn.microsoft.com/en-us/library/ms175972.aspx
-with_expression
-    : WITH ctes += common_table_expression (COMMA ctes += common_table_expression)*
+withExpression
+    : WITH ctes += commonTableExpression (COMMA ctes += commonTableExpression)*
     ;
 
-common_table_expression
-    : expression_name = id_ (LPAREN columns = column_name_list RPAREN)? AS LPAREN cte_query = select_statement RPAREN
+commonTableExpression
+    : expressionName = id (LPAREN columns = columnNameList RPAREN)? AS LPAREN cteQuery = selectStatement RPAREN
     ;
 
-update_elem
-    : LOCAL_ID EQ full_column_name (EQ | assignment_operator) expression //Combined variable and column update
-    | (full_column_name | LOCAL_ID) (EQ | assignment_operator) expression
-    | udt_column_name = id_ DOT method_name = id_ LPAREN expression_list_ RPAREN
-    //| full_column_name DOT WRITE (expression, )
+updateElem
+    : LOCAL_ID EQ fullColumnName (EQ | assignmentOperator) expression //Combined variable and column update
+    | (fullColumnName | LOCAL_ID) (EQ | assignmentOperator) expression
+    | udtColumnName = id DOT methodName = id LPAREN expressionList RPAREN
+    //| fullColumnName DOT WRITE (expression, )
     ;
 
-update_elem_merge
-    : (full_column_name | LOCAL_ID) (EQ | assignment_operator) expression
-    | udt_column_name = id_ DOT method_name = id_ LPAREN expression_list_ RPAREN
-    //| full_column_name DOT WRITE (expression, )
+updateElemMerge
+    : (fullColumnName | LOCAL_ID) (EQ | assignmentOperator) expression
+    | udtColumnName = id DOT methodName = id LPAREN expressionList RPAREN
+    //| fullColumnName DOT WRITE (expression, )
     ;
 
 // https://docs.microsoft.com/en-us/sql/t-sql/queries/search-condition-transact-sql
-search_condition
-    : NOT* (predicate | LPAREN search_condition RPAREN)
-    | search_condition AND search_condition // AND takes precedence over OR
-    | search_condition OR search_condition
+searchCondition
+    : LPAREN searchCondition RPAREN         #scPrec
+    | NOT searchCondition                   #scNot
+    | searchCondition AND searchCondition   #scAnd
+    | searchCondition OR searchCondition    #scOr
+    | predicate                             #scPred
     ;
 
 predicate
     : EXISTS LPAREN subquery RPAREN
-    | freetext_predicate
-    | expression comparison_operator expression
+    | freetextPredicate
+    | expression comparisonOperator expression
     | expression ME expression ////SQL-82 syntax for left outer joins; PE. See https://stackoverflow.com/questions/40665/in-sybase-sql
-    | expression comparison_operator (ALL | SOME | ANY) LPAREN subquery RPAREN
+    | expression comparisonOperator (ALL | SOME | ANY) LPAREN subquery RPAREN
     | expression NOT* BETWEEN expression AND expression
-    | expression NOT* IN LPAREN (subquery | expression_list_) RPAREN
+    | expression NOT* IN LPAREN (subquery | expressionList) RPAREN
     | expression NOT* LIKE expression (ESCAPE expression)?
-    | expression IS null_notnull
+    | expression IS nullNotnull
+    | expression
     ;
 
-// Changed union rule to sql_union to avoid union construct with C++ target.  Issue reported by person who generates into C++.  This individual reports change causes generated code to work
-
-query_expression
-    : query_specification select_order_by_clause? unions += sql_union* //if using top, order by can be on the "top" side of union :/
-    | LPAREN query_expression RPAREN (UNION ALL? query_expression)?
+queryExpression
+    : querySpecification selectOrderByClause? unions += sqlUnion* //if using top, order by can be on the "top" side of union :/
+    | LPAREN queryExpression RPAREN (UNION ALL? queryExpression)?
     ;
 
-sql_union
+sqlUnion
     : (UNION ALL? | EXCEPT | INTERSECT) (
-        spec = query_specification
-        | (LPAREN op = query_expression RPAREN)
+        spec = querySpecification
+        | (LPAREN op = queryExpression RPAREN)
     )
     ;
 
 // https://msdn.microsoft.com/en-us/library/ms176104.aspx
-query_specification
-    : SELECT allOrDistinct = (ALL | DISTINCT)? top = top_clause? columns = select_list
+// TODO: This is too much for one rule and it still misses things - rewrite
+querySpecification
+    : SELECT ad=(ALL | DISTINCT)? topClause? selectListElem (COMMA selectListElem)*
     // https://msdn.microsoft.com/en-us/library/ms188029.aspx
-    (INTO into = table_name)? (FROM from = table_sources)? (WHERE where = search_condition)?
+    (INTO into =tableName)? (FROM tableSources)? (WHERE where = searchCondition)?
     // https://msdn.microsoft.com/en-us/library/ms177673.aspx
     (
         GROUP BY (
-            (groupByAll = ALL? groupBys += group_by_item (COMMA groupBys += group_by_item)*)
-            | GROUPING SETS LPAREN groupSets += grouping_sets_item (
-                COMMA groupSets += grouping_sets_item
+            (groupByAll = ALL? groupBys += groupByItem (COMMA groupBys += groupByItem)*)
+            | GROUPING SETS LPAREN groupSets += groupingSetsItem (
+                COMMA groupSets += groupingSetsItem
             )* RPAREN
         )
-    )? (HAVING having = search_condition)?
+    )? (HAVING having = searchCondition)?
     ;
 
 // https://msdn.microsoft.com/en-us/library/ms189463.aspx
-top_clause
-    : TOP (top_percent | top_count) (WITH TIES)?
+topClause
+    : TOP (topPercent | topCount) (WITH TIES)?
     ;
 
-top_percent
-    : percent_constant = (REAL | FLOAT | INT) PERCENT
-    | LPAREN topper_expression = expression RPAREN PERCENT
+topPercent
+    : percentConstant = (REAL | FLOAT | INT) PERCENT
+    | LPAREN topperExpression = expression RPAREN PERCENT
     ;
 
-top_count
-    : count_constant = INT
-    | LPAREN topcount_expression = expression RPAREN
+topCount
+    : countConstant = INT
+    | LPAREN topcountExpression = expression RPAREN
     ;
 
 // https://docs.microsoft.com/en-us/sql/t-sql/queries/select-over-clause-transact-sql?view=sql-server-ver16
-order_by_clause
-    : ORDER BY order_bys += order_by_expression (COMMA order_bys += order_by_expression)*
+orderByClause
+    : ORDER BY orderByExpression (COMMA orderByExpression)*
     ;
 
 // https://msdn.microsoft.com/en-us/library/ms188385.aspx
-select_order_by_clause
-    : order_by_clause (
-        OFFSET offset_exp = expression offset_rows = (ROW | ROWS) (
-            FETCH fetch_offset = (FIRST | NEXT) fetch_exp = expression fetch_rows = (ROW | ROWS) ONLY
+selectOrderByClause
+    : orderByClause (
+        OFFSET offsetExp = expression offsetRows = (ROW | ROWS) (
+            FETCH fetchOffset = (FIRST | NEXT) fetchExp = expression fetchRows = (ROW | ROWS) ONLY
         )?
     )?
     ;
 
 // https://docs.microsoft.com/en-us/sql/t-sql/queries/select-for-clause-transact-sql
-for_clause
+forClause
     : FOR BROWSE
-    | FOR XML (RAW (LPAREN STRING RPAREN)? | AUTO) xml_common_directives* (
+    | FOR XML (RAW (LPAREN STRING RPAREN)? | AUTO) xmlCommonDirectives* (
         COMMA (XMLDATA | XMLSCHEMA (LPAREN STRING RPAREN)?)
     )? (COMMA ELEMENTS (XSINIL | ABSENT)?)?
-    | FOR XML EXPLICIT xml_common_directives* (COMMA XMLDATA)?
-    | FOR XML PATH (LPAREN STRING RPAREN)? xml_common_directives* (COMMA ELEMENTS (XSINIL | ABSENT)?)?
+    | FOR XML EXPLICIT xmlCommonDirectives* (COMMA XMLDATA)?
+    | FOR XML PATH (LPAREN STRING RPAREN)? xmlCommonDirectives* (COMMA ELEMENTS (XSINIL | ABSENT)?)?
     | FOR JSON (AUTO | PATH) (
         COMMA (ROOT (LPAREN STRING RPAREN) | INCLUDE_NULL_VALUES | WITHOUT_ARRAY_WRAPPER)
     )*
     ;
 
-xml_common_directives
+xmlCommonDirectives
     : COMMA (BINARY_KEYWORD BASE64 | TYPE | ROOT (LPAREN STRING RPAREN)?)
     ;
 
-order_by_expression
-    : order_by = expression (ascending = ASC | descending = DESC)?
+orderByExpression
+    : expression (ASC | DESC)?
     ;
 
 // https://docs.microsoft.com/en-us/sql/t-sql/queries/select-group-by-transact-sql?view=sql-server-ver15
-grouping_sets_item
-    : LPAREN? groupSetItems += group_by_item (COMMA groupSetItems += group_by_item)* RPAREN?
+groupingSetsItem
+    : LPAREN? groupSetItems += groupByItem (COMMA groupSetItems += groupByItem)* RPAREN?
     | LPAREN RPAREN
     ;
 
-group_by_item
+groupByItem
     : expression
-    /*| rollup_spec
-    | cube_spec
-    | grouping_sets_spec
-    | grand_total*/
+    /*| rollupSpec
+    | cubeSpec
+    | groupingSetsSpec
+    | grandTotal*/
     ;
 
-option_clause
+optionClause
     // https://msdn.microsoft.com/en-us/library/ms181714.aspx
     : OPTION LPAREN options_ += option (COMMA options_ += option)* RPAREN
     ;
 
 option
-    : FAST number_rows = INT
+    : FAST numberRows = INT
     | (HASH | ORDER) GROUP
     | (MERGE | HASH | CONCAT) UNION
     | (LOOP | MERGE | HASH) JOIN
     | EXPAND VIEWS
     | FORCE ORDER
     | IGNORE_NONCLUSTERED_COLUMNSTORE_INDEX
     | KEEP PLAN
     | KEEPFIXED PLAN
-    | MAXDOP number_of_processors = INT
-    | MAXRECURSION number_recursion = INT
-    | OPTIMIZE FOR LPAREN optimize_for_arg (COMMA optimize_for_arg)* RPAREN
+    | MAXDOP numberOfProcessors = INT
+    | MAXRECURSION numberRecursion = INT
+    | OPTIMIZE FOR LPAREN optimizeForArg (COMMA optimizeForArg)* RPAREN
     | OPTIMIZE FOR UNKNOWN
     | PARAMETERIZATION (SIMPLE | FORCED)
     | RECOMPILE
     | ROBUST PLAN
     | USE PLAN STRING
     ;
 
-optimize_for_arg
+optimizeForArg
     : LOCAL_ID (UNKNOWN | EQ (constant | NULL_))
     ;
 
 // https://msdn.microsoft.com/en-us/library/ms176104.aspx
-select_list
-    : selectElement += select_list_elem (COMMA selectElement += select_list_elem)*
+selectList
+    : selectElement += selectListElem (COMMA selectElement += selectListElem)*
     ;
 
-udt_method_arguments
-    : LPAREN argument += execute_var_string (COMMA argument += execute_var_string)* RPAREN
+udtMethodArguments
+    : LPAREN argument += executeVarString (COMMA argument += executeVarString)* RPAREN
     ;
 
 // https://docs.microsoft.com/ru-ru/sql/t-sql/queries/select-clause-transact-sql
 asterisk
-    : (table_name DOT)? STAR
-    | (INSERTED | DELETED) DOT STAR
+    : (INSERTED | DELETED) DOT STAR
+    | (tableName DOT)? STAR
     ;
 
-udt_elem
-    : udt_column_name = id_ DOT non_static_attr = id_ udt_method_arguments as_column_alias?
-    | udt_column_name = id_ DOUBLE_COLON static_attr = id_ udt_method_arguments? as_column_alias?
+udtElem
+    : udtColumnName = id DOT nonStaticAttr = id udtMethodArguments asColumnAlias?
+    | udtColumnName = id DOUBLE_COLON staticAttr = id udtMethodArguments? asColumnAlias?
     ;
 
-expression_elem
-    : leftAlias = column_alias eq = EQ leftAssignment = expression
-    | expressionAs = expression as_column_alias?
+expressionElem
+    : columnAlias EQ expression
+    | expression asColumnAlias?
     ;
 
-select_list_elem
+selectListElem
     : asterisk
-    | udt_elem
-    | LOCAL_ID (assignment_operator | EQ) expression
-    | expression_elem
+    | LOCAL_ID op=(PE | ME | SE | DE | MEA | AND_ASSIGN | XOR_ASSIGN | OR_ASSIGN | EQ) expression
+    | expressionElem
+    | udtElem  // TODO: May not be needed as expressionElem can handle this?
     ;
 
-table_sources
-    : non_ansi_join
-    | source += table_source (COMMA source += table_source)*
+tableSources
+    : source += tableSource (COMMA source += tableSource)*
     ;
 
 // https://sqlenlight.com/support/help/sa0006/
-non_ansi_join
-    : source += table_source (COMMA source += table_source)+
+// TODO: This is exactly the same as tableSources alt 2 - investigate
+nonAnsiJoin
+    : source += tableSource (COMMA source += tableSource)+
     ;
 
 // https://docs.microsoft.com/en-us/sql/t-sql/queries/from-transact-sql
-table_source
-    : table_source_item joins += join_part*
+tableSource
+    : tableSourceItem joinPart*
     ;
 
-table_source_item
-    : full_table_name deprecated_table_hint as_table_alias // this is currently allowed
-    | full_table_name as_table_alias? (
-        with_table_hints
-        | deprecated_table_hint
-        | sybase_legacy_hints
-    )?
-    | rowset_function as_table_alias?
-    | LPAREN derived_table RPAREN (as_table_alias column_alias_list?)?
-    | change_table as_table_alias?
-    | nodes_method (as_table_alias column_alias_list?)?
-    | function_call (as_table_alias column_alias_list?)?
-    | loc_id = LOCAL_ID as_table_alias?
-    | loc_id_call = LOCAL_ID DOT loc_fcall = function_call (as_table_alias column_alias_list?)?
-    | open_xml
-    | open_json
-    | DOUBLE_COLON oldstyle_fcall = function_call as_table_alias? // Build-in function (old syntax)
-    | LPAREN table_source RPAREN
+tableSourceItem
+    : tableName deprecatedTableHint asTableAlias // this is currently allowed
+    | tableName asTableAlias? (
+        withTableHints
+        | deprecatedTableHint
+        | sybaseLegacyHints
+    )?
+    | rowsetFunction asTableAlias?
+    | LPAREN derivedTable RPAREN (asTableAlias columnAliasList?)?
+    | changeTable asTableAlias?
+    | nodesMethod (asTableAlias columnAliasList?)?
+    | functionCall (asTableAlias columnAliasList?)?
+    | locId = LOCAL_ID asTableAlias?
+    | locIdCall = LOCAL_ID DOT locFcall = functionCall (asTableAlias columnAliasList?)?
+    | openXml
+    | openJson
+    | DOUBLE_COLON oldstyleFcall = functionCall asTableAlias? // Build-in function (old syntax)
+    | LPAREN tableSource RPAREN
     ;
 
 // https://docs.microsoft.com/en-us/sql/t-sql/functions/openxml-transact-sql
-open_xml
-    : OPENXML LPAREN expression COMMA expression (COMMA expression)? RPAREN (WITH LPAREN schema_declaration RPAREN)? as_table_alias?
+openXml
+    : OPENXML LPAREN expression COMMA expression (COMMA expression)? RPAREN (WITH LPAREN schemaDeclaration RPAREN)? asTableAlias?
     ;
 
-open_json
-    : OPENJSON LPAREN expression (COMMA expression)? RPAREN (WITH LPAREN json_declaration RPAREN)? as_table_alias?
+openJson
+    : OPENJSON LPAREN expression (COMMA expression)? RPAREN (WITH LPAREN jsonDeclaration RPAREN)? asTableAlias?
     ;
 
-json_declaration
-    : json_col += json_column_declaration (COMMA json_col += json_column_declaration)*
+jsonDeclaration
+    : jsonCol += jsonColumnDeclaration (COMMA jsonCol += jsonColumnDeclaration)*
     ;
 
-json_column_declaration
-    : column_declaration (AS JSON)?
+jsonColumnDeclaration
+    : columnDeclaration (AS JSON)?
     ;
 
-schema_declaration
-    : xml_col += column_declaration (COMMA xml_col += column_declaration)*
+schemaDeclaration
+    : xmlCol += columnDeclaration (COMMA xmlCol += columnDeclaration)*
     ;
 
-column_declaration
-    : id_ data_type STRING?
+columnDeclaration
+    : id dataType STRING?
     ;
 
-change_table
-    : change_table_changes
-    | change_table_version
+changeTable
+    : changeTableChanges
+    | changeTableVersion
     ;
 
-change_table_changes
-    : CHANGETABLE LPAREN CHANGES changetable = table_name COMMA changesid = (NULL_ | INT | LOCAL_ID) RPAREN
+changeTableChanges
+    : CHANGETABLE LPAREN CHANGES changetable = tableName COMMA changesid = (NULL_ | INT | LOCAL_ID) RPAREN
     ;
 
-change_table_version
-    : CHANGETABLE LPAREN VERSION versiontable = table_name COMMA pk_columns = full_column_name_list COMMA pk_values = select_list RPAREN
+changeTableVersion
+    : CHANGETABLE LPAREN VERSION versiontable = tableName COMMA pkColumns = fullColumnNameList COMMA pkValues = selectList RPAREN
     ;
 
 // https://msdn.microsoft.com/en-us/library/ms191472.aspx
-join_part
+joinPart
     // https://msdn.microsoft.com/en-us/library/ms173815(v=sql.120).aspx
-    : join_on
-    | cross_join
+    : joinOn
+    | crossJoin
     | apply_
     | pivot
     | unpivot
     ;
 
-outer_join
+outerJoin
     : (LEFT | RIGHT | FULL) OUTER?
     ;
 
-join_type
+joinType
     : INNER
-    | outer_join
+    | outerJoin
     ;
 
-join_on
-    : join_type? (
-        join_hint = (LOOP | HASH | MERGE | REMOTE)
-    )? JOIN source = table_source ON cond = search_condition
+joinOn
+    : joinType? (
+        joinHint = (LOOP | HASH | MERGE | REMOTE)
+    )? JOIN source = tableSource ON cond = searchCondition
     ;
 
-cross_join
-    : CROSS JOIN table_source_item
+crossJoin
+    : CROSS JOIN tableSourceItem
     ;
 
 apply_
-    : apply_style = (CROSS | OUTER) APPLY source = table_source_item
+    : applyStyle = (CROSS | OUTER) APPLY source = tableSourceItem
     ;
 
 pivot
-    : PIVOT pivot_clause as_table_alias
+    : PIVOT pivotClause asTableAlias
     ;
 
 unpivot
-    : UNPIVOT unpivot_clause as_table_alias
+    : UNPIVOT unpivotClause asTableAlias
     ;
 
-pivot_clause
-    : LPAREN aggregate_windowed_function FOR full_column_name IN column_alias_list RPAREN
+pivotClause
+    : LPAREN expression FOR fullColumnName IN columnAliasList RPAREN
     ;
 
-unpivot_clause
-    : LPAREN unpivot_exp = expression FOR full_column_name IN LPAREN full_column_name_list RPAREN RPAREN
+unpivotClause
+    : LPAREN unpivotExp = expression FOR fullColumnName IN LPAREN fullColumnNameList RPAREN RPAREN
     ;
 
-full_column_name_list
-    : column += full_column_name (COMMA column += full_column_name)*
+fullColumnNameList
+    : column += fullColumnName (COMMA column += fullColumnName)*
     ;
 
 // https://msdn.microsoft.com/en-us/library/ms190312.aspx
-rowset_function
+rowsetFunction
     : (
-        OPENROWSET LPAREN provider_name = STRING COMMA connectionString = STRING COMMA sql = STRING RPAREN
+        OPENROWSET LPAREN providerName = STRING COMMA connectionString = STRING COMMA sql = STRING RPAREN
     )
-    | (OPENROWSET LPAREN BULK data_file = STRING COMMA (bulk_option (COMMA bulk_option)* | id_) RPAREN)
+    | (OPENROWSET LPAREN BULK dataFile = STRING COMMA (bulkOption (COMMA bulkOption)* | id) RPAREN)
     ;
 
 // runtime check.
-bulk_option
-    : id_ EQ bulk_option_value = (INT | STRING)
+bulkOption
+    : id EQ bulkOptionValue = (INT | STRING)
     ;
 
-derived_table
+derivedTable
     : subquery
     | LPAREN subquery (UNION ALL subquery)* RPAREN
-    | table_value_constructor
-    | LPAREN table_value_constructor RPAREN
+    | tableValueConstructor
+    | LPAREN tableValueConstructor RPAREN
     ;
 
-function_call
-    : ranking_windowed_function                      # RANKING_WINDOWED_FUNC
-    | aggregate_windowed_function                    # AGGREGATE_WINDOWED_FUNC
-    | analytic_windowed_function                     # ANALYTIC_WINDOWED_FUNC
-    | built_in_functions                             # BUILT_IN_FUNC
-    | scalar_function_name LPAREN expression_list_? RPAREN # SCALAR_FUNCTION
-    | freetext_function                              # FREE_TEXT
-    | partition_function                             # PARTITION_FUNC
-    | hierarchyid_static_method                      # HIERARCHYID_METHOD
+functionCall
+    : analyticWindowedFunction
+    | builtInFunctions
+    | standardFunction
+    | freetextFunction
+    | partitionFunction
+    | hierarchyidStaticMethod
+    // TODO: This is broken and highly ambiguous - will need to be reworked so the expression allows the primitives
+    // | scalarFunctionName LPAREN expressionList? RPAREN
     ;
 
-partition_function
-    : (database = id_ DOT)? DOLLAR_PARTITION DOT func_name = id_ LPAREN expression RPAREN
+// Standard functions are built in but take standard syntax, or are
+// some user function etc
+standardFunction
+    : funcId LPAREN (expression (COMMA expression)*)? RPAREN
     ;
 
-freetext_function
-    : (CONTAINSTABLE | FREETEXTTABLE) LPAREN table_name COMMA (
-        full_column_name
-        | LPAREN full_column_name (COMMA full_column_name)* RPAREN
+funcId
+    : id
+    | LOG
+    | FORMAT
+    | LEFT
+    | RIGHT
+    | REPLACE
+    | CONCAT
+    ;
+
+partitionFunction
+    : (database = id DOT)? DOLLAR_PARTITION DOT funcName = id LPAREN expression RPAREN
+    ;
+
+freetextFunction
+    : (CONTAINSTABLE | FREETEXTTABLE) LPAREN tableName COMMA (
+        fullColumnName
+        | LPAREN fullColumnName (COMMA fullColumnName)* RPAREN
         | STAR
     ) COMMA expression (COMMA LANGUAGE expression)? (COMMA expression)? RPAREN
-    | (SEMANTICSIMILARITYTABLE | SEMANTICKEYPHRASETABLE) LPAREN table_name COMMA (
-        full_column_name
-        | LPAREN full_column_name (COMMA full_column_name)* RPAREN
+    | (SEMANTICSIMILARITYTABLE | SEMANTICKEYPHRASETABLE) LPAREN tableName COMMA (
+        fullColumnName
+        | LPAREN fullColumnName (COMMA fullColumnName)* RPAREN
         | STAR
     ) COMMA expression RPAREN
-    | SEMANTICSIMILARITYDETAILSTABLE LPAREN table_name COMMA full_column_name COMMA expression COMMA full_column_name COMMA expression RPAREN
+    | SEMANTICSIMILARITYDETAILSTABLE LPAREN tableName COMMA fullColumnName COMMA expression COMMA fullColumnName COMMA expression RPAREN
     ;
 
-freetext_predicate
+freetextPredicate
     : CONTAINS LPAREN (
-        full_column_name
-        | LPAREN full_column_name (COMMA full_column_name)* RPAREN
+        fullColumnName
+        | LPAREN fullColumnName (COMMA fullColumnName)* RPAREN
         | STAR
-        | PROPERTY LPAREN full_column_name COMMA expression RPAREN
+        | PROPERTY LPAREN fullColumnName COMMA expression RPAREN
     ) COMMA expression RPAREN
-    | FREETEXT LPAREN table_name COMMA (
-        full_column_name
-        | LPAREN full_column_name (COMMA full_column_name)* RPAREN
+    | FREETEXT LPAREN tableName COMMA (
+        fullColumnName
+        | LPAREN fullColumnName (COMMA fullColumnName)* RPAREN
         | STAR
     ) COMMA expression (COMMA LANGUAGE expression)? RPAREN
     ;
 
-json_key_value
-    : json_key_name = expression COLON value_expression = expression
+jsonKeyValue
+    : jsonKeyName = expression COLON valueExpression = expression
     ;
 
-json_null_clause
+jsonNullClause
     : (ABSENT | NULL_) ON NULL_
     ;
 
-built_in_functions
-    // Metadata functions
-    // https://docs.microsoft.com/en-us/sql/t-sql/functions/app-name-transact-sql?view=sql-server-ver16
-    : APP_NAME LPAREN RPAREN # APP_NAME
-    // https://docs.microsoft.com/en-us/sql/t-sql/functions/applock-mode-transact-sql?view=sql-server-ver16
-    | APPLOCK_MODE LPAREN database_principal = expression COMMA resource_name = expression COMMA lock_owner = expression RPAREN # APPLOCK_MODE
-    // https://docs.microsoft.com/en-us/sql/t-sql/functions/applock-test-transact-sql?view=sql-server-ver16
-    | APPLOCK_TEST LPAREN database_principal = expression COMMA resource_name = expression COMMA lock_mode = expression COMMA lock_owner = expression RPAREN #
-        APPLOCK_TEST
-    // https://docs.microsoft.com/en-us/sql/t-sql/functions/assemblyproperty-transact-sql?view=sql-server-ver16
-    | ASSEMBLYPROPERTY LPAREN assembly_name = expression COMMA property_name = expression RPAREN # ASSEMBLYPROPERTY
-    // https://docs.microsoft.com/en-us/sql/t-sql/functions/col-length-transact-sql?view=sql-server-ver16
-    | COL_LENGTH LPAREN table = expression COMMA column = expression RPAREN # COL_LENGTH
-    // https://docs.microsoft.com/en-us/sql/t-sql/functions/col-name-transact-sql?view=sql-server-ver16
-    | COL_NAME LPAREN table_id = expression COMMA column_id = expression RPAREN # COL_NAME
-    // https://docs.microsoft.com/en-us/sql/t-sql/functions/columnproperty-transact-sql?view=sql-server-ver16
-    | COLUMNPROPERTY LPAREN id = expression COMMA column = expression COMMA property = expression RPAREN # COLUMNPROPERTY
-    // https://docs.microsoft.com/en-us/sql/t-sql/functions/databasepropertyex-transact-sql?view=sql-server-ver16
-    | DATABASEPROPERTYEX LPAREN database = expression COMMA property = expression RPAREN # DATABASEPROPERTYEX
-    // https://docs.microsoft.com/en-us/sql/t-sql/functions/db-id-transact-sql?view=sql-server-ver16
-    | DB_ID LPAREN database_name = expression? RPAREN # DB_ID
-    // https://docs.microsoft.com/en-us/sql/t-sql/functions/db-name-transact-sql?view=sql-server-ver16
-    | DB_NAME LPAREN database_id = expression? RPAREN # DB_NAME
-    // https://docs.microsoft.com/en-us/sql/t-sql/functions/file-id-transact-sql?view=sql-server-ver16
-    | FILE_ID LPAREN file_name = expression RPAREN # FILE_ID
-    // https://docs.microsoft.com/en-us/sql/t-sql/functions/file-idex-transact-sql?view=sql-server-ver16
-    | FILE_IDEX LPAREN file_name = expression RPAREN # FILE_IDEX
-    // https://docs.microsoft.com/en-us/sql/t-sql/functions/file-name-transact-sql?view=sql-server-ver16
-    | FILE_NAME LPAREN file_id = expression RPAREN # FILE_NAME
-    // https://docs.microsoft.com/en-us/sql/t-sql/functions/filegroup-id-transact-sql?view=sql-server-ver16
-    | FILEGROUP_ID LPAREN filegroup_name = expression RPAREN # FILEGROUP_ID
-    // https://docs.microsoft.com/en-us/sql/t-sql/functions/filegroup-name-transact-sql?view=sql-server-ver16
-    | FILEGROUP_NAME LPAREN filegroup_id = expression RPAREN # FILEGROUP_NAME
-    // https://docs.microsoft.com/en-us/sql/t-sql/functions/filegroupproperty-transact-sql?view=sql-server-ver16
-    | FILEGROUPPROPERTY LPAREN filegroup_name = expression COMMA property = expression RPAREN # FILEGROUPPROPERTY
-    // https://docs.microsoft.com/en-us/sql/t-sql/functions/fileproperty-transact-sql?view=sql-server-ver16
-    | FILEPROPERTY LPAREN file_name = expression COMMA property = expression RPAREN # FILEPROPERTY
-    // https://docs.microsoft.com/en-us/sql/t-sql/functions/filepropertyex-transact-sql?view=sql-server-ver16
-    | FILEPROPERTYEX LPAREN name = expression COMMA property = expression RPAREN # FILEPROPERTYEX
-    // https://docs.microsoft.com/en-us/sql/t-sql/functions/fulltextcatalogproperty-transact-sql?view=sql-server-ver16
-    | FULLTEXTCATALOGPROPERTY LPAREN catalog_name = expression COMMA property = expression RPAREN # FULLTEXTCATALOGPROPERTY
-    // https://docs.microsoft.com/en-us/sql/t-sql/functions/fulltextserviceproperty-transact-sql?view=sql-server-ver16
-    | FULLTEXTSERVICEPROPERTY LPAREN property = expression RPAREN # FULLTEXTSERVICEPROPERTY
-    // https://docs.microsoft.com/en-us/sql/t-sql/functions/index-col-transact-sql?view=sql-server-ver16
-    | INDEX_COL LPAREN table_or_view_name = expression COMMA index_id = expression COMMA key_id = expression RPAREN # INDEX_COL
-    // https://docs.microsoft.com/en-us/sql/t-sql/functions/indexkey-property-transact-sql?view=sql-server-ver16
-    | INDEXKEY_PROPERTY LPAREN object_id = expression COMMA index_id = expression COMMA key_id = expression COMMA property = expression RPAREN # INDEXKEY_PROPERTY
-    // https://docs.microsoft.com/en-us/sql/t-sql/functions/indexproperty-transact-sql?view=sql-server-ver16
-    | INDEXPROPERTY LPAREN object_id = expression COMMA index_or_statistics_name = expression COMMA property = expression RPAREN # INDEXPROPERTY
-    // https://docs.microsoft.com/en-us/sql/t-sql/functions/next-value-for-transact-sql?view=sql-server-ver16
-    | NEXT VALUE FOR sequence_name = table_name (OVER LPAREN order_by_clause RPAREN)? # NEXT_VALUE_FOR
-    // https://docs.microsoft.com/en-us/sql/t-sql/functions/object-definition-transact-sql?view=sql-server-ver16
-    | OBJECT_DEFINITION LPAREN object_id = expression RPAREN # OBJECT_DEFINITION
-    // https://docs.microsoft.com/en-us/sql/t-sql/functions/object-id-transact-sql?view=sql-server-ver16
-    | OBJECT_ID LPAREN object_name = expression (COMMA object_type = expression)? RPAREN # OBJECT_ID
-    // https://docs.microsoft.com/en-us/sql/t-sql/functions/object-name-transact-sql?view=sql-server-ver16
-    | OBJECT_NAME LPAREN object_id = expression (COMMA database_id = expression)? RPAREN # OBJECT_NAME
-    // https://docs.microsoft.com/en-us/sql/t-sql/functions/object-schema-name-transact-sql?view=sql-server-ver16
-    | OBJECT_SCHEMA_NAME LPAREN object_id = expression (COMMA database_id = expression)? RPAREN # OBJECT_SCHEMA_NAME
-    // https://docs.microsoft.com/en-us/sql/t-sql/functions/objectproperty-transact-sql?view=sql-server-ver16
-    | OBJECTPROPERTY LPAREN id = expression COMMA property = expression RPAREN # OBJECTPROPERTY
-    // https://docs.microsoft.com/en-us/sql/t-sql/functions/objectpropertyex-transact-sql?view=sql-server-ver16
-    | OBJECTPROPERTYEX LPAREN id = expression COMMA property = expression RPAREN # OBJECTPROPERTYEX
-    // https://docs.microsoft.com/en-us/sql/t-sql/functions/original-db-name-transact-sql?view=sql-server-ver16
-    | ORIGINAL_DB_NAME LPAREN RPAREN # ORIGINAL_DB_NAME
-    // https://docs.microsoft.com/en-us/sql/t-sql/functions/parsename-transact-sql?view=sql-server-ver16
-    | PARSENAME LPAREN object_name = expression COMMA object_piece = expression RPAREN # PARSENAME
-    // https://docs.microsoft.com/en-us/sql/t-sql/functions/schema-id-transact-sql?view=sql-server-ver16
-    | SCHEMA_ID LPAREN schema_name = expression? RPAREN # SCHEMA_ID
-    // https://docs.microsoft.com/en-us/sql/t-sql/functions/schema-name-transact-sql?view=sql-server-ver16
-    | SCHEMA_NAME LPAREN schema_id = expression? RPAREN # SCHEMA_NAME
-    // https://docs.microsoft.com/en-us/sql/t-sql/functions/scope-identity-transact-sql?view=sql-server-ver16
-    | SCOPE_IDENTITY LPAREN RPAREN # SCOPE_IDENTITY
-    // https://docs.microsoft.com/en-us/sql/t-sql/functions/serverproperty-transact-sql?view=sql-server-ver16
-    | SERVERPROPERTY LPAREN property = expression RPAREN # SERVERPROPERTY
-    // https://docs.microsoft.com/en-us/sql/t-sql/functions/stats-date-transact-sql?view=sql-server-ver16
-    | STATS_DATE LPAREN object_id = expression COMMA stats_id = expression RPAREN # STATS_DATE
-    // https://docs.microsoft.com/en-us/sql/t-sql/functions/type-id-transact-sql?view=sql-server-ver16
-    | TYPE_ID LPAREN type_name = expression RPAREN # TYPE_ID
-    // https://docs.microsoft.com/en-us/sql/t-sql/functions/type-name-transact-sql?view=sql-server-ver16
-    | TYPE_NAME LPAREN type_id = expression RPAREN # TYPE_NAME
-    // https://docs.microsoft.com/en-us/sql/t-sql/functions/typeproperty-transact-sql?view=sql-server-ver16
-    | TYPEPROPERTY LPAREN type = expression COMMA property = expression RPAREN # TYPEPROPERTY
-    // String functions
-    // https://docs.microsoft.com/en-us/sql/t-sql/functions/ascii-transact-sql?view=sql-server-ver16
-    | ASCII LPAREN character_expression = expression RPAREN # ASCII
-    // https://docs.microsoft.com/en-us/sql/t-sql/functions/char-transact-sql?view=sql-server-ver16
-    | CHAR LPAREN integer_expression = expression RPAREN # CHAR
-    // https://docs.microsoft.com/en-us/sql/t-sql/functions/charindex-transact-sql?view=sql-server-ver16
-    | CHARINDEX LPAREN expressionToFind = expression COMMA expressionToSearch = expression (
-        COMMA start_location = expression
-    )? RPAREN # CHARINDEX
-    // https://docs.microsoft.com/en-us/sql/t-sql/functions/concat-transact-sql?view=sql-server-ver16
-    | CONCAT LPAREN string_value_1 = expression COMMA string_value_2 = expression (
-        COMMA string_value_n += expression
-    )* RPAREN # CONCAT
-    // https://docs.microsoft.com/en-us/sql/t-sql/functions/concat-ws-transact-sql?view=sql-server-ver16
-    | CONCAT_WS LPAREN separator = expression COMMA argument_1 = expression COMMA argument_2 = expression (
-        COMMA argument_n += expression
-    )* RPAREN # CONCAT_WS
-    // https://docs.microsoft.com/en-us/sql/t-sql/functions/difference-transact-sql?view=sql-server-ver16
-    | DIFFERENCE LPAREN character_expression_1 = expression COMMA character_expression_2 = expression RPAREN # DIFFERENCE
-    // https://docs.microsoft.com/en-us/sql/t-sql/functions/format-transact-sql?view=sql-server-ver16
-    | FORMAT LPAREN value = expression COMMA format = expression (COMMA culture = expression)? RPAREN # FORMAT
-    // https://docs.microsoft.com/en-us/sql/t-sql/functions/left-transact-sql?view=sql-server-ver16
-    | LEFT LPAREN character_expression = expression COMMA integer_expression = expression RPAREN # LEFT
-    // https://docs.microsoft.com/en-us/sql/t-sql/functions/len-transact-sql?view=sql-server-ver16
-    | LEN LPAREN string_expression = expression RPAREN # LEN
-    // https://docs.microsoft.com/en-us/sql/t-sql/functions/lower-transact-sql?view=sql-server-ver16
-    | LOWER LPAREN character_expression = expression RPAREN # LOWER
-    // https://docs.microsoft.com/en-us/sql/t-sql/functions/ltrim-transact-sql?view=sql-server-ver16
-    | LTRIM LPAREN character_expression = expression RPAREN # LTRIM
-    // https://docs.microsoft.com/en-us/sql/t-sql/functions/nchar-transact-sql?view=sql-server-ver16
-    | NCHAR LPAREN integer_expression = expression RPAREN # NCHAR
-    // https://docs.microsoft.com/en-us/sql/t-sql/functions/patindex-transact-sql?view=sql-server-ver16
-    | PATINDEX LPAREN pattern = expression COMMA string_expression = expression RPAREN # PATINDEX
-    // https://docs.microsoft.com/en-us/sql/t-sql/functions/quotename-transact-sql?view=sql-server-ver16
-    | QUOTENAME LPAREN character_string = expression (COMMA quote_character = expression)? RPAREN # QUOTENAME
-    // https://docs.microsoft.com/en-us/sql/t-sql/functions/replace-transact-sql?view=sql-server-ver16
-    | REPLACE LPAREN input = expression COMMA replacing = expression COMMA with = expression RPAREN # REPLACE
-    // https://docs.microsoft.com/en-us/sql/t-sql/functions/replicate-transact-sql?view=sql-server-ver16
-    | REPLICATE LPAREN string_expression = expression COMMA integer_expression = expression RPAREN # REPLICATE
-    // https://docs.microsoft.com/en-us/sql/t-sql/functions/reverse-transact-sql?view=sql-server-ver16
-    | REVERSE LPAREN string_expression = expression RPAREN # REVERSE
-    // https://docs.microsoft.com/en-us/sql/t-sql/functions/right-transact-sql?view=sql-server-ver16
-    | RIGHT LPAREN character_expression = expression COMMA integer_expression = expression RPAREN # RIGHT
-    // https://docs.microsoft.com/en-us/sql/t-sql/functions/rtrim-transact-sql?view=sql-server-ver16
-    | RTRIM LPAREN character_expression = expression RPAREN # RTRIM
-    // https://docs.microsoft.com/en-us/sql/t-sql/functions/soundex-transact-sql?view=sql-server-ver16
-    | SOUNDEX LPAREN character_expression = expression RPAREN # SOUNDEX
-    // https://docs.microsoft.com/en-us/sql/t-sql/functions/space-transact-sql?view=sql-server-ver16
-    | SPACE_KEYWORD LPAREN integer_expression = expression RPAREN # SPACE
-    // https://docs.microsoft.com/en-us/sql/t-sql/functions/str-transact-sql?view=sql-server-ver16
-    | STR LPAREN float_expression = expression (
-        COMMA length_expression = expression ( COMMA decimal = expression)?
-    )? RPAREN # STR
-    // https://docs.microsoft.com/en-us/sql/t-sql/functions/string-agg-transact-sql?view=sql-server-ver16
-    | STRING_AGG LPAREN expr = expression COMMA separator = expression RPAREN (
-        WITHIN GROUP LPAREN order_by_clause RPAREN
-    )? # STRINGAGG
-    // https://docs.microsoft.com/en-us/sql/t-sql/functions/string-escape-transact-sql?view=sql-server-ver16
-    | STRING_ESCAPE LPAREN text_ = expression COMMA type_ = expression RPAREN # STRING_ESCAPE
-    // https://msdn.microsoft.com/fr-fr/library/ms188043.aspx
-    | STUFF LPAREN str = expression COMMA from = expression COMMA to = expression COMMA str_with = expression RPAREN # STUFF
-    // https://docs.microsoft.com/en-us/sql/t-sql/functions/substring-transact-sql?view=sql-server-ver16
-    | SUBSTRING LPAREN string_expression = expression COMMA start_ = expression COMMA length = expression RPAREN # SUBSTRING
-    // https://docs.microsoft.com/en-us/sql/t-sql/functions/translate-transact-sql?view=sql-server-ver16
-    | TRANSLATE LPAREN inputString = expression COMMA characters = expression COMMA translations = expression RPAREN # TRANSLATE
-    // https://docs.microsoft.com/en-us/sql/t-sql/functions/trim-transact-sql?view=sql-server-ver16
-    | TRIM LPAREN (characters = expression FROM)? string_ = expression RPAREN # TRIM
-    // https://docs.microsoft.com/en-us/sql/t-sql/functions/unicode-transact-sql?view=sql-server-ver16
-    | UNICODE LPAREN ncharacter_expression = expression RPAREN # UNICODE
-    // https://docs.microsoft.com/en-us/sql/t-sql/functions/upper-transact-sql?view=sql-server-ver16
-    | UPPER LPAREN character_expression = expression RPAREN # UPPER
-    // System functions
-    // https://msdn.microsoft.com/en-us/library/ms173784.aspx
+builtInFunctions
+    : NEXT VALUE FOR sequenceName = tableName (OVER LPAREN orderByClause RPAREN)? # NEXT_VALUE_FOR
+      // https://msdn.microsoft.com/en-us/library/ms173784.aspx
     | BINARY_CHECKSUM LPAREN (star = STAR | expression (COMMA expression)*) RPAREN # BINARY_CHECKSUM
-    // https://msdn.microsoft.com/en-us/library/ms189788.aspx
+      // https://msdn.microsoft.com/en-us/library/ms189788.aspx
     | CHECKSUM LPAREN (star = STAR | expression (COMMA expression)*) RPAREN # CHECKSUM
-    // https://docs.microsoft.com/en-us/sql/t-sql/functions/compress-transact-sql?view=sql-server-ver16
-    | COMPRESS LPAREN expr = expression RPAREN # COMPRESS
-    // https://docs.microsoft.com/en-us/sql/t-sql/functions/connectionproperty-transact-sql?view=sql-server-ver16
-    | CONNECTIONPROPERTY LPAREN property = STRING RPAREN # CONNECTIONPROPERTY
-    // https://docs.microsoft.com/en-us/sql/t-sql/functions/context-info-transact-sql?view=sql-server-ver16
-    | CONTEXT_INFO LPAREN RPAREN # CONTEXT_INFO
-    // https://docs.microsoft.com/en-us/sql/t-sql/functions/current-request-id-transact-sql?view=sql-server-ver16
-    | CURRENT_REQUEST_ID LPAREN RPAREN # CURRENT_REQUEST_ID
-    // https://docs.microsoft.com/en-us/sql/t-sql/functions/current-transaction-id-transact-sql?view=sql-server-ver16
-    | CURRENT_TRANSACTION_ID LPAREN RPAREN # CURRENT_TRANSACTION_ID
-    // https://docs.microsoft.com/en-us/sql/t-sql/functions/decompress-transact-sql?view=sql-server-ver16
-    | DECOMPRESS LPAREN expr = expression RPAREN # DECOMPRESS
-    // https://docs.microsoft.com/en-us/sql/t-sql/functions/error-line-transact-sql?view=sql-server-ver16
-    | ERROR_LINE LPAREN RPAREN # ERROR_LINE
-    // https://docs.microsoft.com/en-us/sql/t-sql/functions/error-message-transact-sql?view=sql-server-ver16
-    | ERROR_MESSAGE LPAREN RPAREN # ERROR_MESSAGE
-    // https://docs.microsoft.com/en-us/sql/t-sql/functions/error-number-transact-sql?view=sql-server-ver16
-    | ERROR_NUMBER LPAREN RPAREN # ERROR_NUMBER
-    // https://docs.microsoft.com/en-us/sql/t-sql/functions/error-procedure-transact-sql?view=sql-server-ver16
-    | ERROR_PROCEDURE LPAREN RPAREN # ERROR_PROCEDURE
-    // https://docs.microsoft.com/en-us/sql/t-sql/functions/error-severity-transact-sql?view=sql-server-ver16
-    | ERROR_SEVERITY LPAREN RPAREN # ERROR_SEVERITY
-    // https://docs.microsoft.com/en-us/sql/t-sql/functions/error-state-transact-sql?view=sql-server-ver16
-    | ERROR_STATE LPAREN RPAREN # ERROR_STATE
-    // https://docs.microsoft.com/en-us/sql/t-sql/functions/formatmessage-transact-sql?view=sql-server-ver16
-    | FORMATMESSAGE LPAREN (msg_number = INT | msg_string = STRING | msg_variable = LOCAL_ID) COMMA expression (
-        COMMA expression
-    )* RPAREN # FORMATMESSAGE
-    // https://docs.microsoft.com/en-us/sql/t-sql/functions/get-filestream-transaction-context-transact-sql?view=sql-server-ver16
-    | GET_FILESTREAM_TRANSACTION_CONTEXT LPAREN RPAREN # GET_FILESTREAM_TRANSACTION_CONTEXT
-    // https://docs.microsoft.com/en-us/sql/t-sql/functions/getansinull-transact-sql?view=sql-server-ver16
-    | GETANSINULL LPAREN (database = STRING)? RPAREN # GETANSINULL
-    // https://docs.microsoft.com/en-us/sql/t-sql/functions/host-id-transact-sql?view=sql-server-ver16
-    | HOST_ID LPAREN RPAREN # HOST_ID
-    // https://docs.microsoft.com/en-us/sql/t-sql/functions/host-name-transact-sql?view=sql-server-ver16
-    | HOST_NAME LPAREN RPAREN # HOST_NAME
-    // https://msdn.microsoft.com/en-us/library/ms184325.aspx
-    | ISNULL LPAREN left = expression COMMA right = expression RPAREN # ISNULL
-    // https://docs.microsoft.com/en-us/sql/t-sql/functions/isnumeric-transact-sql?view=sql-server-ver16
-    | ISNUMERIC LPAREN expression RPAREN # ISNUMERIC
-    // https://docs.microsoft.com/en-us/sql/t-sql/functions/min-active-rowversion-transact-sql?view=sql-server-ver16
-    | MIN_ACTIVE_ROWVERSION LPAREN RPAREN # MIN_ACTIVE_ROWVERSION
-    // https://docs.microsoft.com/en-us/sql/t-sql/functions/newid-transact-sql?view=sql-server-ver16
-    | NEWID LPAREN RPAREN # NEWID
-    // https://docs.microsoft.com/en-us/sql/t-sql/functions/newsequentialid-transact-sql?view=sql-server-ver16
-    | NEWSEQUENTIALID LPAREN RPAREN # NEWSEQUENTIALID
-    // https://docs.microsoft.com/en-us/sql/t-sql/functions/rowcount-big-transact-sql?view=sql-server-ver16
-    | ROWCOUNT_BIG LPAREN RPAREN # ROWCOUNT_BIG
-    // https://docs.microsoft.com/en-us/sql/t-sql/functions/session-context-transact-sql?view=sql-server-ver16
-    | SESSION_CONTEXT LPAREN key = STRING RPAREN # SESSION_CONTEXT
-    // https://docs.microsoft.com/en-us/sql/t-sql/functions/xact-state-transact-sql?view=sql-server-ver16
-    | XACT_STATE LPAREN RPAREN # XACT_STATE
-    // https://msdn.microsoft.com/en-us/library/hh231076.aspx
-    // https://msdn.microsoft.com/en-us/library/ms187928.aspx
-    | CAST LPAREN expression AS data_type RPAREN     # CAST
-    | TRY_CAST LPAREN expression AS data_type RPAREN # TRY_CAST
-    | CONVERT LPAREN convert_data_type = data_type COMMA convert_expression = expression (
-        COMMA style = expression
-    )? RPAREN # CONVERT
-    // https://msdn.microsoft.com/en-us/library/ms190349.aspx
-    | COALESCE LPAREN expression_list_ RPAREN # COALESCE
-    // Cursor functions
-    // https://learn.microsoft.com/en-us/sql/t-sql/functions/cursor-rows-transact-sql?view=sql-server-ver16
+      // https://docs.microsoft.com/en-us/sql/t-sql/functions/compress-transact-sql?view=sql-server-ver16
+    | CAST LPAREN expression AS dataType RPAREN     # CAST
+    | TRY_CAST LPAREN expression AS dataType RPAREN # TRY_CAST
+      // https://learn.microsoft.com/en-us/sql/t-sql/functions/ident-seed-transact-sql?view=sql-server-ver16
+    | IDENTITY LPAREN datatype = dataType (COMMA seed = INT COMMA increment = INT)? RPAREN # IDENTITY
     | CURSOR_ROWS # CURSOR_ROWS
-    // https://learn.microsoft.com/en-us/sql/t-sql/functions/cursor-rows-transact-sql?view=sql-server-ver16
+      // https://learn.microsoft.com/en-us/sql/t-sql/functions/cursor-rows-transact-sql?view=sql-server-ver16
     | FETCH_STATUS # FETCH_STATUS
-    // https://learn.microsoft.com/en-us/sql/t-sql/functions/cursor-status-transact-sql?view=sql-server-ver16
-    | CURSOR_STATUS LPAREN scope = STRING COMMA cursor = expression RPAREN # CURSOR_STATUS
-    // Cryptographic functions
-    // https://learn.microsoft.com/en-us/sql/t-sql/functions/cert-id-transact-sql?view=sql-server-ver16
-    | CERT_ID LPAREN cert_name = expression RPAREN # CERT_ID
-    // Data type functions
-    // https://learn.microsoft.com/en-us/sql/t-sql/functions/datalength-transact-sql?view=sql-server-ver16
-    | DATALENGTH LPAREN expression RPAREN # DATALENGTH
-    // https://learn.microsoft.com/en-us/sql/t-sql/functions/ident-current-transact-sql?view=sql-server-ver16
-    | IDENT_CURRENT LPAREN table_or_view = expression RPAREN # IDENT_CURRENT
-    // https://learn.microsoft.com/en-us/sql/t-sql/functions/ident-incr-transact-sql?view=sql-server-ver16
-    | IDENT_INCR LPAREN table_or_view = expression RPAREN # IDENT_INCR
-    // https://learn.microsoft.com/en-us/sql/t-sql/functions/ident-seed-transact-sql?view=sql-server-ver16
-    | IDENT_SEED LPAREN table_or_view = expression RPAREN # IDENT_SEED
-    // https://learn.microsoft.com/en-us/sql/t-sql/functions/ident-seed-transact-sql?view=sql-server-ver16
-    | IDENTITY LPAREN datatype = data_type (COMMA seed = INT COMMA increment = INT)? RPAREN # IDENTITY
-    // https://learn.microsoft.com/en-us/sql/t-sql/functions/ident-seed-transact-sql?view=sql-server-ver16
-    | SQL_VARIANT_PROPERTY LPAREN expr = expression COMMA property = STRING RPAREN # SQL_VARIANT_PROPERTY
-    // Date functions
-    //https://infocenter.sybase.com/help/index.jsp?topic=/com.sybase.infocenter.dc36271.1572/html/blocks/CJADIDHD.htm
-    | CURRENT_DATE LPAREN RPAREN # CURRENT_DATE
-    // https://msdn.microsoft.com/en-us/library/ms188751.aspx
-    | CURRENT_TIMESTAMP # CURRENT_TIMESTAMP
-    // https://learn.microsoft.com/en-us/sql/t-sql/functions/current-timezone-transact-sql?view=sql-server-ver16
-    | CURRENT_TIMEZONE LPAREN RPAREN # CURRENT_TIMEZONE
-    // https://learn.microsoft.com/en-us/sql/t-sql/functions/current-timezone-id-transact-sql?view=sql-server-ver16
-    | CURRENT_TIMEZONE_ID LPAREN RPAREN # CURRENT_TIMEZONE_ID
-    // https://learn.microsoft.com/en-us/sql/t-sql/functions/date-bucket-transact-sql?view=sql-server-ver16
-    | DATE_BUCKET LPAREN datepart = dateparts_9 COMMA number = expression COMMA date = expression (
-        COMMA origin = expression
-    )? RPAREN # DATE_BUCKET
-    // https://msdn.microsoft.com/en-us/library/ms186819.aspx
-    | DATEADD LPAREN datepart = dateparts_12 COMMA number = expression COMMA date = expression RPAREN # DATEADD
-    // https://msdn.microsoft.com/en-us/library/ms189794.aspx
-    | DATEDIFF LPAREN datepart = dateparts_12 COMMA date_first = expression COMMA date_second = expression RPAREN # DATEDIFF
-    // https://learn.microsoft.com/en-us/sql/t-sql/functions/datediff-big-transact-sql?view=sql-server-ver16
-    | DATEDIFF_BIG LPAREN datepart = dateparts_12 COMMA startdate = expression COMMA enddate = expression RPAREN # DATEDIFF_BIG
-    // https://learn.microsoft.com/en-us/sql/t-sql/functions/datefromparts-transact-sql?view=sql-server-ver16
-    | DATEFROMPARTS LPAREN year = expression COMMA month = expression COMMA day = expression RPAREN # DATEFROMPARTS
-    // https://msdn.microsoft.com/en-us/library/ms174395.aspx
-    | DATENAME LPAREN datepart = dateparts_15 COMMA date = expression RPAREN # DATENAME
-    // https://msdn.microsoft.com/en-us/library/ms174420.aspx
-    | DATEPART LPAREN datepart = dateparts_15 COMMA date = expression RPAREN # DATEPART
-    // https://learn.microsoft.com/en-us/sql/t-sql/functions/datetime2fromparts-transact-sql?view=sql-server-ver16
-    | DATETIME2FROMPARTS LPAREN year = expression COMMA month = expression COMMA day = expression COMMA hour = expression COMMA minute = expression COMMA seconds =
-        expression COMMA fractions = expression COMMA precision = expression RPAREN # DATETIME2FROMPARTS
-    // https://learn.microsoft.com/en-us/sql/t-sql/functions/datetimefromparts-transact-sql?view=sql-server-ver16
-    | DATETIMEFROMPARTS LPAREN year = expression COMMA month = expression COMMA day = expression COMMA hour = expression COMMA minute = expression COMMA seconds =
-        expression COMMA milliseconds = expression RPAREN # DATETIMEFROMPARTS
-    // https://learn.microsoft.com/en-us/sql/t-sql/functions/datetimeoffsetfromparts-transact-sql?view=sql-server-ver16
-    | DATETIMEOFFSETFROMPARTS LPAREN year = expression COMMA month = expression COMMA day = expression COMMA hour = expression COMMA minute = expression COMMA
-        seconds = expression COMMA fractions = expression COMMA hour_offset = expression COMMA minute_offset = expression COMMA precision = INT RPAREN #
-        DATETIMEOFFSETFROMPARTS
-    // https://learn.microsoft.com/en-us/sql/t-sql/functions/datetrunc-transact-sql?view=sql-server-ver16
-    | DATETRUNC LPAREN datepart = dateparts_datetrunc COMMA date = expression RPAREN # DATETRUNC
-    // https://learn.microsoft.com/en-us/sql/t-sql/functions/day-transact-sql?view=sql-server-ver16
-    | DAY LPAREN date = expression RPAREN # DAY
-    // https://learn.microsoft.com/en-us/sql/t-sql/functions/eomonth-transact-sql?view=sql-server-ver16
-    | EOMONTH LPAREN start_date = expression (COMMA month_to_add = expression)? RPAREN # EOMONTH
-    // https://docs.microsoft.com/en-us/sql/t-sql/functions/getdate-transact-sql
-    | GETDATE LPAREN RPAREN # GETDATE
-    // https://docs.microsoft.com/en-us/sql/t-sql/functions/getdate-transact-sql
-    | GETUTCDATE LPAREN RPAREN # GETUTCDATE
-    // https://learn.microsoft.com/en-us/sql/t-sql/functions/isdate-transact-sql?view=sql-server-ver16
-    | ISDATE LPAREN expression RPAREN # ISDATE
-    // https://learn.microsoft.com/en-us/sql/t-sql/functions/month-transact-sql?view=sql-server-ver16
-    | MONTH LPAREN date = expression RPAREN # MONTH
-    // https://learn.microsoft.com/en-us/sql/t-sql/functions/smalldatetimefromparts-transact-sql?view=sql-server-ver16
-    | SMALLDATETIMEFROMPARTS LPAREN year = expression COMMA month = expression COMMA day = expression COMMA hour = expression COMMA minute = expression RPAREN #
-        SMALLDATETIMEFROMPARTS
-    // https://learn.microsoft.com/en-us/sql/t-sql/functions/switchoffset-transact-sql?view=sql-server-ver16
-    | SWITCHOFFSET LPAREN datetimeoffset_expression = expression COMMA timezoneoffset_expression = expression RPAREN # SWITCHOFFSET
-    // https://learn.microsoft.com/en-us/sql/t-sql/functions/sysdatetime-transact-sql?view=sql-server-ver16
-    | SYSDATETIME LPAREN RPAREN # SYSDATETIME
-    // https://learn.microsoft.com/en-us/sql/t-sql/functions/sysdatetimeoffset-transact-sql?view=sql-server-ver16
-    | SYSDATETIMEOFFSET LPAREN RPAREN # SYSDATETIMEOFFSET
-    // https://learn.microsoft.com/en-us/sql/t-sql/functions/sysutcdatetime-transact-sql?view=sql-server-ver16
-    | SYSUTCDATETIME LPAREN RPAREN # SYSUTCDATETIME
-    //https://learn.microsoft.com/en-us/sql/t-sql/functions/timefromparts-transact-sql?view=sql-server-ver16
-    | TIMEFROMPARTS LPAREN hour = expression COMMA minute = expression COMMA seconds = expression COMMA fractions = expression COMMA precision = INT RPAREN #
-        TIMEFROMPARTS
-    // https://learn.microsoft.com/en-us/sql/t-sql/functions/todatetimeoffset-transact-sql?view=sql-server-ver16
-    | TODATETIMEOFFSET LPAREN datetime_expression = expression COMMA timezoneoffset_expression = expression RPAREN # TODATETIMEOFFSET
-    // https://learn.microsoft.com/en-us/sql/t-sql/functions/year-transact-sql?view=sql-server-ver16
-    | YEAR LPAREN date = expression RPAREN # YEAR
-    // https://msdn.microsoft.com/en-us/library/ms189838.aspx
-    | IDENTITY LPAREN data_type (COMMA seed = INT)? (COMMA increment = INT)? RPAREN # IDENTITY
-    // https://msdn.microsoft.com/en-us/library/bb839514.aspx
-    | MIN_ACTIVE_ROWVERSION LPAREN RPAREN # MIN_ACTIVE_ROWVERSION
-    // https://msdn.microsoft.com/en-us/library/ms177562.aspx
-    | NULLIF LPAREN left = expression COMMA right = expression RPAREN # NULLIF
-    // https://docs.microsoft.com/en-us/sql/t-sql/functions/parse-transact-sql
-    // https://docs.microsoft.com/en-us/sql/t-sql/functions/try-parse-transact-sql
-    | PARSE LPAREN str = expression AS data_type (USING culture = expression)? RPAREN # PARSE
-    // https://docs.microsoft.com/en-us/sql/t-sql/xml/xml-data-type-methods
-    | xml_data_type_methods # XML_DATA_TYPE_FUNC
-    // https://docs.microsoft.com/en-us/sql/t-sql/functions/logical-functions-iif-transact-sql
-    | IIF LPAREN cond = search_condition COMMA left = expression COMMA right = expression RPAREN # IIF
-    // JSON functions
-    // https://learn.microsoft.com/en-us/sql/t-sql/functions/isjson-transact-sql?view=azure-sqldw-latest
-    | ISJSON LPAREN json_expr = expression (COMMA json_type_constraint = expression)? RPAREN # ISJSON
-    // https://learn.microsoft.com/en-us/sql/t-sql/functions/json-object-transact-sql?view=azure-sqldw-latest
-    | JSON_OBJECT LPAREN (key_value = json_key_value (COMMA key_value = json_key_value)*)? json_null_clause? RPAREN # JSON_OBJECT
-    // https://learn.microsoft.com/en-us/sql/t-sql/functions/json-array-transact-sql?view=azure-sqldw-latest
-    | JSON_ARRAY LPAREN expression_list_? json_null_clause? RPAREN # JSON_ARRAY
-    // https://learn.microsoft.com/en-us/sql/t-sql/functions/json-value-transact-sql?view=azure-sqldw-latest
-    | JSON_VALUE LPAREN expr = expression COMMA path = expression RPAREN # JSON_VALUE
-    // https://learn.microsoft.com/en-us/sql/t-sql/functions/json-query-transact-sql?view=azure-sqldw-latest
-    | JSON_QUERY LPAREN expr = expression (COMMA path = expression)? RPAREN # JSON_QUERY
-    // https://learn.microsoft.com/en-us/sql/t-sql/functions/json-modify-transact-sql?view=azure-sqldw-latest
-    | JSON_MODIFY LPAREN expr = expression COMMA path = expression COMMA new_value = expression RPAREN # JSON_MODIFY
-    // https://learn.microsoft.com/en-us/sql/t-sql/functions/json-path-exists-transact-sql?view=azure-sqldw-latest
-    | JSON_PATH_EXISTS LPAREN value_expression = expression COMMA sql_json_path = expression RPAREN # JSON_PATH_EXISTS
-    // Math functions
-    // https://learn.microsoft.com/en-us/sql/t-sql/functions/abs-transact-sql?view=sql-server-ver16
-    | ABS LPAREN numeric_expression = expression RPAREN # ABS
-    // https://learn.microsoft.com/en-us/sql/t-sql/functions/acos-transact-sql?view=sql-server-ver16
-    | ACOS LPAREN float_expression = expression RPAREN # ACOS
-    // https://learn.microsoft.com/en-us/sql/t-sql/functions/asin-transact-sql?view=sql-server-ver16
-    | ASIN LPAREN float_expression = expression RPAREN # ASIN
-    // https://learn.microsoft.com/en-us/sql/t-sql/functions/atan-transact-sql?view=sql-server-ver16
-    | ATAN LPAREN float_expression = expression RPAREN # ATAN
-    // https://learn.microsoft.com/en-us/sql/t-sql/functions/atn2-transact-sql?view=sql-server-ver16
-    | ATN2 LPAREN float_expression = expression COMMA float_expression = expression RPAREN # ATN2
-    // https://learn.microsoft.com/en-us/sql/t-sql/functions/ceiling-transact-sql?view=sql-server-ver16
-    | CEILING LPAREN numeric_expression = expression RPAREN # CEILING
-    // https://learn.microsoft.com/en-us/sql/t-sql/functions/cos-transact-sql?view=sql-server-ver16
-    | COS LPAREN float_expression = expression RPAREN # COS
-    // https://learn.microsoft.com/en-us/sql/t-sql/functions/cot-transact-sql?view=sql-server-ver16
-    | COT LPAREN float_expression = expression RPAREN # COT
-    // https://learn.microsoft.com/en-us/sql/t-sql/functions/degrees-transact-sql?view=sql-server-ver16
-    | DEGREES LPAREN numeric_expression = expression RPAREN # DEGREES
-    // https://learn.microsoft.com/en-us/sql/t-sql/functions/exp-transact-sql?view=sql-server-ver16
-    | EXP LPAREN float_expression = expression RPAREN # EXP
-    // https://learn.microsoft.com/en-us/sql/t-sql/functions/floor-transact-sql?view=sql-server-ver16
-    | FLOOR LPAREN numeric_expression = expression RPAREN # FLOOR
-    // https://learn.microsoft.com/en-us/sql/t-sql/functions/log-transact-sql?view=sql-server-ver16
-    | LOG LPAREN float_expression = expression (COMMA base = expression)? RPAREN # LOG
-    // https://learn.microsoft.com/en-us/sql/t-sql/functions/log10-transact-sql?view=sql-server-ver16
-    | LOG10 LPAREN float_expression = expression RPAREN # LOG10
-    // https://learn.microsoft.com/en-us/sql/t-sql/functions/pi-transact-sql?view=sql-server-ver16
-    | PI LPAREN RPAREN # PI
-    // https://learn.microsoft.com/en-us/sql/t-sql/functions/power-transact-sql?view=sql-server-ver16
-    | POWER LPAREN float_expression = expression COMMA y = expression RPAREN # POWER
-    // https://learn.microsoft.com/en-us/sql/t-sql/functions/radians-transact-sql?view=sql-server-ver16
-    | RADIANS LPAREN numeric_expression = expression RPAREN # RADIANS
-    // https://learn.microsoft.com/en-us/sql/t-sql/functions/rand-transact-sql?view=sql-server-ver16
-    | RAND LPAREN (seed = expression)? RPAREN # RAND
-    // https://learn.microsoft.com/en-us/sql/t-sql/functions/round-transact-sql?view=sql-server-ver16
-    | ROUND LPAREN numeric_expression = expression COMMA length = expression (COMMA function = expression)? RPAREN # ROUND
-    // https://learn.microsoft.com/en-us/sql/t-sql/functions/sign-transact-sql?view=sql-server-ver16
-    | SIGN LPAREN numeric_expression = expression RPAREN # MATH_SIGN
-    // https://learn.microsoft.com/en-us/sql/t-sql/functions/sin-transact-sql?view=sql-server-ver16
-    | SIN LPAREN float_expression = expression RPAREN # SIN
-    // https://learn.microsoft.com/en-us/sql/t-sql/functions/sqrt-transact-sql?view=sql-server-ver16
-    | SQRT LPAREN float_expression = expression RPAREN # SQRT
-    // https://learn.microsoft.com/en-us/sql/t-sql/functions/square-transact-sql?view=sql-server-ver16
-    | SQUARE LPAREN float_expression = expression RPAREN # SQUARE
-    // https://learn.microsoft.com/en-us/sql/t-sql/functions/tan-transact-sql?view=sql-server-ver16
-    | TAN LPAREN float_expression = expression RPAREN # TAN
-    // Logical functions
-    // https://learn.microsoft.com/en-us/sql/t-sql/functions/logical-functions-greatest-transact-sql?view=azure-sqldw-latest
-    | GREATEST LPAREN expression_list_ RPAREN # GREATEST
-    // https://learn.microsoft.com/en-us/sql/t-sql/functions/logical-functions-least-transact-sql?view=azure-sqldw-latest
-    | LEAST LPAREN expression_list_ RPAREN # LEAST
-    // Security functions
-    // https://learn.microsoft.com/en-us/sql/t-sql/functions/certencoded-transact-sql?view=sql-server-ver16
-    | CERTENCODED LPAREN certid = expression RPAREN # CERTENCODED
-    // https://learn.microsoft.com/en-us/sql/t-sql/functions/certprivatekey-transact-sql?view=sql-server-ver16
-    | CERTPRIVATEKEY LPAREN certid = expression COMMA encryption_password = expression (
-        COMMA decryption_pasword = expression
-    )? RPAREN # CERTPRIVATEKEY
-    // https://msdn.microsoft.com/en-us/library/ms176050.aspx
-    | CURRENT_USER # CURRENT_USER
-    // https://learn.microsoft.com/en-us/sql/t-sql/functions/database-principal-id-transact-sql?view=sql-server-ver16
-    | DATABASE_PRINCIPAL_ID LPAREN (principal_name = expression)? RPAREN # DATABASE_PRINCIPAL_ID
-    // https://learn.microsoft.com/en-us/sql/t-sql/functions/has-dbaccess-transact-sql?view=sql-server-ver16
-    | HAS_DBACCESS LPAREN database_name = expression RPAREN # HAS_DBACCESS
-    // https://learn.microsoft.com/en-us/sql/t-sql/functions/has-perms-by-name-transact-sql?view=sql-server-ver16
-    | HAS_PERMS_BY_NAME LPAREN securable = expression COMMA securable_class = expression COMMA permission = expression (
-        COMMA sub_securable = expression (COMMA sub_securable_class = expression)?
-    )? RPAREN # HAS_PERMS_BY_NAME
-    // https://learn.microsoft.com/en-us/sql/t-sql/functions/is-member-transact-sql?view=sql-server-ver16
-    | IS_MEMBER LPAREN group_or_role = expression RPAREN # IS_MEMBER
-    // https://learn.microsoft.com/en-us/sql/t-sql/functions/is-rolemember-transact-sql?view=sql-server-ver16
-    | IS_ROLEMEMBER LPAREN role = expression (COMMA database_principal = expression)? RPAREN # IS_ROLEMEMBER
-    // https://learn.microsoft.com/en-us/sql/t-sql/functions/is-srvrolemember-transact-sql?view=sql-server-ver16
-    | IS_SRVROLEMEMBER LPAREN role = expression (COMMA login = expression)? RPAREN # IS_SRVROLEMEMBER
-    // https://learn.microsoft.com/en-us/sql/t-sql/functions/loginproperty-transact-sql?view=sql-server-ver16
-    | LOGINPROPERTY LPAREN login_name = expression COMMA property_name = expression RPAREN # LOGINPROPERTY
-    // https://learn.microsoft.com/en-us/sql/t-sql/functions/original-login-transact-sql?view=sql-server-ver16
-    | ORIGINAL_LOGIN LPAREN RPAREN # ORIGINAL_LOGIN
-    // https://learn.microsoft.com/en-us/sql/t-sql/functions/permissions-transact-sql?view=sql-server-ver16
-    | PERMISSIONS LPAREN (object_id = expression (COMMA column = expression)?)? RPAREN # PERMISSIONS
-    // https://learn.microsoft.com/en-us/sql/t-sql/functions/pwdencrypt-transact-sql?view=sql-server-ver16
-    | PWDENCRYPT LPAREN password = expression RPAREN # PWDENCRYPT
-    // https://learn.microsoft.com/en-us/sql/t-sql/functions/pwdcompare-transact-sql?view=sql-server-ver16
-    | PWDCOMPARE LPAREN clear_text_password = expression COMMA password_hash = expression (
-        COMMA version = expression
-    )? RPAREN # PWDCOMPARE
-    // https://msdn.microsoft.com/en-us/library/ms177587.aspx
+    | PARSE LPAREN str = expression AS dataType (USING culture = expression)? RPAREN # PARSE
+    | JSON_ARRAY LPAREN expressionList? jsonNullClause? RPAREN # JSON_ARRAY
+    | JSON_OBJECT LPAREN (keyValue = jsonKeyValue (COMMA keyValue = jsonKeyValue)*)? jsonNullClause? RPAREN # JSON_OBJECT
+      // https://msdn.microsoft.com/en-us/library/ms177587.aspx
     | SESSION_USER # SESSION_USER
-    // https://learn.microsoft.com/en-us/sql/t-sql/functions/sessionproperty-transact-sql?view=sql-server-ver16
-    | SESSIONPROPERTY LPAREN option_name = expression RPAREN # SESSIONPROPERTY
-    // https://learn.microsoft.com/en-us/sql/t-sql/functions/suser-id-transact-sql?view=sql-server-ver16
-    | SUSER_ID LPAREN (login = expression)? RPAREN # SUSER_ID
-    // https://learn.microsoft.com/en-us/sql/t-sql/functions/suser-name-transact-sql?view=sql-server-ver16
-    | SUSER_NAME LPAREN (server_user_sid = expression)? RPAREN # SUSER_SNAME
-    // https://learn.microsoft.com/en-us/sql/t-sql/functions/suser-sid-transact-sql?view=sql-server-ver16
-    | SUSER_SID LPAREN (login = expression (COMMA param2 = expression)?)? RPAREN # SUSER_SID
-    // https://learn.microsoft.com/en-us/sql/t-sql/functions/suser-sname-transact-sql?view=sql-server-ver16
-    | SUSER_SNAME LPAREN (server_user_sid = expression)? RPAREN # SUSER_SNAME
-    // https://msdn.microsoft.com/en-us/library/ms179930.aspx
+      // https://msdn.microsoft.com/en-us/library/ms179930.aspx
     | SYSTEM_USER # SYSTEM_USER
-    // https://learn.microsoft.com/en-us/sql/t-sql/functions/user-transact-sql?view=sql-server-ver16
+      // https://learn.microsoft.com/en-us/sql/t-sql/functions/user-transact-sql?view=sql-server-ver16
     | USER # USER
-    // https://learn.microsoft.com/en-us/sql/t-sql/functions/user-id-transact-sql?view=sql-server-ver16
-    | USER_ID LPAREN (user = expression)? RPAREN # USER_ID
-    // https://learn.microsoft.com/en-us/sql/t-sql/functions/user-name-transact-sql?view=sql-server-ver16
-    | USER_NAME LPAREN (id = expression)? RPAREN # USER_NAME
-    ;
-
-xml_data_type_methods
-    : value_method
-    | query_method
-    | exist_method
-    | modify_method
-    ;
-
-// https://learn.microsoft.com/en-us/sql/t-sql/functions/date-bucket-transact-sql?view=sql-server-ver16
-dateparts_9
-    : YEAR
-    | YEAR_ABBR
-    | QUARTER
-    | QUARTER_ABBR
-    | MONTH
-    | MONTH_ABBR
-    | DAY
-    | DAY_ABBR
-    | WEEK
-    | WEEK_ABBR
-    | HOUR
-    | HOUR_ABBR
-    | MINUTE
-    | MINUTE_ABBR
-    | SECOND
-    | SECOND_ABBR
-    | MILLISECOND
-    | MILLISECOND_ABBR
-    ;
-
-// https://learn.microsoft.com/en-us/sql/t-sql/functions/dateadd-transact-sql?view=sql-server-ver16
-dateparts_12
-    : dateparts_9
-    | DAYOFYEAR
-    | DAYOFYEAR_ABBR
-    | MICROSECOND
-    | MICROSECOND_ABBR
-    | NANOSECOND
-    | NANOSECOND_ABBR
-    ;
-
-// https://learn.microsoft.com/en-us/sql/t-sql/functions/datename-transact-sql?view=sql-server-ver16
-dateparts_15
-    : dateparts_12
-    | WEEKDAY
-    | WEEKDAY_ABBR
-    | TZOFFSET
-    | TZOFFSET_ABBR
-    | ISO_WEEK
-    | ISO_WEEK_ABBR
-    ;
-
-// https://learn.microsoft.com/en-us/sql/t-sql/functions/datetrunc-transact-sql?view=sql-server-ver16
-dateparts_datetrunc
-    : dateparts_9
-    | DAYOFYEAR
-    | DAYOFYEAR_ABBR
-    | MICROSECOND
-    | MICROSECOND_ABBR
-    | ISO_WEEK
-    | ISO_WEEK_ABBR
     ;
 
-value_method
+valueMethod
     : (
-        loc_id = LOCAL_ID
-        | value_id = full_column_name
+        locId = LOCAL_ID
+        | valueId = fullColumnName
         | eventdata = EVENTDATA LPAREN RPAREN
-        | query = query_method
         | LPAREN subquery RPAREN
-    ) DOT call = value_call
+    ) DOT standardFunction
     ;
 
-value_call
-    : (VALUE | VALUE_SQUARE_BRACKET) LPAREN xquery = STRING COMMA sqltype = STRING RPAREN
-    ;
-
-query_method
-    : (loc_id = LOCAL_ID | value_id = full_column_name | LPAREN subquery RPAREN) DOT call = query_call
-    ;
-
-query_call
-    : (QUERY | QUERY_SQUARE_BRACKET) LPAREN xquery = STRING RPAREN
-    ;
-
-exist_method
-    : (loc_id = LOCAL_ID | value_id = full_column_name | LPAREN subquery RPAREN) DOT call = exist_call
-    ;
-
-exist_call
-    : (EXIST | EXIST_SQUARE_BRACKET) LPAREN xquery = STRING RPAREN
-    ;
-
-modify_method
-    : (loc_id = LOCAL_ID | value_id = full_column_name | LPAREN subquery RPAREN) DOT call = modify_call
-    ;
-
-modify_call
-    : (MODIFY | MODIFY_SQUARE_BRACKET) LPAREN xml_dml = STRING RPAREN
-    ;
-
-hierarchyid_call
-    : GETANCESTOR LPAREN n = expression RPAREN
-    | GETDESCENDANT LPAREN child1 = expression COMMA child2 = expression RPAREN
-    | GETLEVEL LPAREN RPAREN
-    | ISDESCENDANTOF LPAREN parent_ = expression RPAREN
-    | GETREPARENTEDVALUE LPAREN oldroot = expression COMMA newroot = expression RPAREN
-    | TOSTRING LPAREN RPAREN
-    ;
-
-hierarchyid_static_method
+hierarchyidStaticMethod
     : HIERARCHYID DOUBLE_COLON (GETROOT LPAREN RPAREN | PARSE LPAREN input = expression RPAREN)
     ;
 
-nodes_method
-    : (loc_id = LOCAL_ID | value_id = full_column_name | LPAREN subquery RPAREN) DOT NODES LPAREN xquery = STRING RPAREN
+nodesMethod
+    : (locId = LOCAL_ID | valueId = fullColumnName | LPAREN subquery RPAREN) DOT NODES LPAREN xquery = STRING RPAREN
     ;
 
-switch_section
-    : WHEN expression THEN expression
+switchSection
+    // Nore that searchCondition includes an expression only but allows too much for case expression.. on purpose
+    : WHEN searchCondition THEN expression
     ;
 
-switch_search_condition_section
-    : WHEN search_condition THEN expression
+asColumnAlias
+    : AS? columnAlias
     ;
 
-as_column_alias
-    : AS? column_alias
-    ;
-
-as_table_alias
-    : AS? table_alias
-    ;
-
-table_alias
-    : id_
+asTableAlias
+    : AS? (id | DOUBLE_QUOTE_ID)
     ;
 
 // https://msdn.microsoft.com/en-us/library/ms187373.aspx
-with_table_hints
-    : WITH LPAREN hint += table_hint (COMMA? hint += table_hint)* RPAREN
+withTableHints
+    : WITH LPAREN hint += tableHint (COMMA? hint += tableHint)* RPAREN
     ;
 
-deprecated_table_hint
-    : LPAREN table_hint RPAREN
+deprecatedTableHint
+    : LPAREN tableHint RPAREN
     ;
 
 // https://infocenter-archive.sybase.com/help/index.jsp?topic=/com.sybase.infocenter.dc00938.1502/html/locking/locking103.htm
 // https://infocenter-archive.sybase.com/help/index.jsp?topic=/com.sybase.dc32300_1250/html/sqlug/sqlug792.htm
 // https://infocenter-archive.sybase.com/help/index.jsp?topic=/com.sybase.dc36271_36272_36273_36274_1250/html/refman/X35229.htm
 // Legacy hint with no parenthesis and no WITH keyword. Actually conflicts with table alias name except for holdlock which is
 // a reserved keyword in this grammar. We might want a separate sybase grammar variant.
-sybase_legacy_hints
-    : sybase_legacy_hint+
+sybaseLegacyHints
+    : sybaseLegacyHint+
     ;
 
-sybase_legacy_hint
+sybaseLegacyHint
     : HOLDLOCK
     | NOHOLDLOCK
     | READPAST
     | SHARED
     ;
 
 // For simplicity, we don't build subsets for INSERT/UPDATE/DELETE/SELECT/MERGE
 // which means the grammar accept slightly more than the what the specification (documentation) says.
-table_hint
+tableHint
     : NOEXPAND
     | INDEX (
-        LPAREN index_value (COMMA index_value)* RPAREN
-        | EQ LPAREN index_value RPAREN
-        | EQ index_value // examples in the doc include this syntax
+        LPAREN indexValue (COMMA indexValue)* RPAREN
+        | EQ LPAREN indexValue RPAREN
+        | EQ indexValue // examples in the doc include this syntax
     )
-    | FORCESEEK ( LPAREN index_value LPAREN column_name_list RPAREN RPAREN)?
+    | FORCESEEK ( LPAREN indexValue LPAREN columnNameList RPAREN RPAREN)?
     | FORCESCAN
     | HOLDLOCK
     | NOLOCK
     | NOWAIT
     | PAGLOCK
     | READCOMMITTED
     | READCOMMITTEDLOCK
@@ -4969,319 +4459,271 @@
     | XLOCK
     | KEEPIDENTITY
     | KEEPDEFAULTS
     | IGNORE_CONSTRAINTS
     | IGNORE_TRIGGERS
     ;
 
-index_value
-    : id_
+indexValue
+    : id
     | INT
     ;
 
-column_alias_list
-    : LPAREN alias += column_alias (COMMA alias += column_alias)* RPAREN
+columnAliasList
+    : LPAREN columnAlias (COMMA columnAlias)* RPAREN
     ;
 
-column_alias
-    : id_
+columnAlias
+    : id
     | STRING
     ;
 
-table_value_constructor
-    : VALUES LPAREN exps += expression_list_ RPAREN (COMMA LPAREN exps += expression_list_ RPAREN)*
+tableValueConstructor
+    : VALUES LPAREN exps += expressionList RPAREN (COMMA LPAREN exps += expressionList RPAREN)*
     ;
 
-expression_list_
+expressionList
     : exp += expression (COMMA exp += expression)*
     ;
 
-// https://msdn.microsoft.com/en-us/library/ms189798.aspx
-ranking_windowed_function
-    : (RANK | DENSE_RANK | ROW_NUMBER) LPAREN RPAREN over_clause
-    | NTILE LPAREN expression RPAREN over_clause
-    ;
-
-// https://msdn.microsoft.com/en-us/library/ms173454.aspx
-aggregate_windowed_function
-    : agg_func = (AVG | MAX | MIN | SUM | STDEV | STDEVP | VAR | VARP) LPAREN all_distinct_expression RPAREN over_clause?
-    | cnt = (COUNT | COUNT_BIG) LPAREN (STAR | all_distinct_expression) RPAREN over_clause?
-    | CHECKSUM_AGG LPAREN all_distinct_expression RPAREN
-    | GROUPING LPAREN expression RPAREN
-    | GROUPING_ID LPAREN expression_list_ RPAREN
-    ;
-
 // https://docs.microsoft.com/en-us/sql/t-sql/functions/analytic-functions-transact-sql
-analytic_windowed_function
-    : (FIRST_VALUE | LAST_VALUE) LPAREN expression RPAREN over_clause
-    | (LAG | LEAD) LPAREN expression (COMMA expression (COMMA expression)?)? RPAREN over_clause
-    | (CUME_DIST | PERCENT_RANK) LPAREN RPAREN OVER LPAREN (PARTITION BY expression_list_)? order_by_clause RPAREN
-    | (PERCENTILE_CONT | PERCENTILE_DISC) LPAREN expression RPAREN WITHIN GROUP LPAREN order_by_clause RPAREN OVER LPAREN (
-        PARTITION BY expression_list_
+analyticWindowedFunction
+    : (FIRST_VALUE | LAST_VALUE) LPAREN expression RPAREN
+    | (LAG | LEAD) LPAREN expression (COMMA expression (COMMA expression)?)? RPAREN
+    | (CUME_DIST | PERCENT_RANK) LPAREN RPAREN OVER LPAREN (PARTITION BY expressionList)? orderByClause RPAREN
+    | (PERCENTILE_CONT | PERCENTILE_DISC) LPAREN expression RPAREN WITHIN GROUP LPAREN orderByClause RPAREN OVER LPAREN (
+        PARTITION BY expressionList
     )? RPAREN
     ;
 
-all_distinct_expression
-    : (ALL | DISTINCT)? expression
-    ;
-
 // https://msdn.microsoft.com/en-us/library/ms189461.aspx
-over_clause
-    : OVER LPAREN (PARTITION BY expression_list_)? order_by_clause? row_or_range_clause? RPAREN
-    ;
-
-row_or_range_clause
-    : (ROWS | RANGE) window_frame_extent
+overClause
+    : OVER LPAREN (PARTITION BY expression (COMMA expression)*)? orderByClause? rowOrRangeClause? RPAREN
     ;
 
-window_frame_extent
-    : window_frame_preceding
-    | BETWEEN window_frame_bound AND window_frame_bound
+rowOrRangeClause
+    : (ROWS | RANGE) windowFrameExtent
     ;
 
-window_frame_bound
-    : window_frame_preceding
-    | window_frame_following
+windowFrameExtent
+    : windowFrameBound
+    | BETWEEN windowFrameBound AND windowFrameBound
     ;
 
-window_frame_preceding
-    : UNBOUNDED PRECEDING
-    | INT PRECEDING
+windowFrameBound
+    : UNBOUNDED (PRECEDING | FOLLOWING)
+    | INT (PRECEDING | FOLLOWING)
     | CURRENT ROW
     ;
 
-window_frame_following
-    : UNBOUNDED FOLLOWING
-    | INT FOLLOWING
-    ;
-
-create_database_option
-    : FILESTREAM (database_filestream_option (COMMA database_filestream_option)*)
-    | DEFAULT_LANGUAGE EQ ( id_ | STRING)
-    | DEFAULT_FULLTEXT_LANGUAGE EQ ( id_ | STRING)
+createDatabaseOption
+    : FILESTREAM (databaseFilestreamOption (COMMA databaseFilestreamOption)*)
+    | DEFAULT_LANGUAGE EQ ( id | STRING)
+    | DEFAULT_FULLTEXT_LANGUAGE EQ ( id | STRING)
     | NESTED_TRIGGERS EQ ( OFF | ON)
     | TRANSFORM_NOISE_WORDS EQ ( OFF | ON)
     | TWO_DIGIT_YEAR_CUTOFF EQ INT
     | DB_CHAINING ( OFF | ON)
     | TRUSTWORTHY ( OFF | ON)
     ;
 
-database_filestream_option
+databaseFilestreamOption
     : LPAREN (
         ( NON_TRANSACTED_ACCESS EQ ( OFF | READ_ONLY | FULL))
         | ( DIRECTORY_NAME EQ STRING)
     ) RPAREN
     ;
 
-database_file_spec
-    : file_group
-    | file_spec
+databaseFileSpec
+    : fileGroup
+    | fileSpecification
     ;
 
-file_group
-    : FILEGROUP id_ (CONTAINS FILESTREAM)? (DEFAULT)? (CONTAINS MEMORY_OPTIMIZED_DATA)? file_spec (
-        COMMA file_spec
+fileGroup
+    : FILEGROUP id (CONTAINS FILESTREAM)? (DEFAULT)? (CONTAINS MEMORY_OPTIMIZED_DATA)? fileSpecification (
+        COMMA fileSpecification
     )*
     ;
 
-file_spec
-    : LPAREN NAME EQ (id_ | STRING) COMMA? FILENAME EQ file = STRING COMMA? (
-        SIZE EQ file_size COMMA?
-    )? (MAXSIZE EQ (file_size | UNLIMITED) COMMA?)? (FILEGROWTH EQ file_size COMMA?)? RPAREN
+fileSpecification
+    : LPAREN NAME EQ (id | STRING) COMMA? FILENAME EQ file = STRING COMMA? (
+        SIZE EQ fileSize COMMA?
+    )? (MAXSIZE EQ (fileSize | UNLIMITED) COMMA?)? (FILEGROWTH EQ fileSize COMMA?)? RPAREN
     ;
 
 // Primitive.
-entity_name
+entityName
     : (
-        server = id_ DOT database = id_ DOT schema = id_ DOT
-        | database = id_ DOT (schema = id_)? DOT
-        | schema = id_ DOT
-    )? table = id_
-    ;
-
-entity_name_for_azure_dw
-    : schema = id_
-    | schema = id_ DOT object_name = id_
+        server = id DOT database = id DOT schema = id DOT
+        | database = id DOT (schema = id)? DOT
+        | schema = id DOT
+    )? table = id
     ;
 
-entity_name_for_parallel_dw
-    : schema_database = id_
-    | schema = id_ DOT object_name = id_
+entityNameForAzureDw
+    : schema = id
+    | schema = id DOT objectName = id
     ;
 
-full_table_name
-    : (
-        linkedServer = id_ DOT DOT schema = id_ DOT
-        | server = id_ DOT database = id_ DOT schema = id_ DOT
-        | database = id_ DOT schema = id_? DOT
-        | schema = id_ DOT
-    )? table = id_
+entityNameForParallelDw
+    : schemaDatabase = id
+    | schema = id DOT objectName = id
     ;
 
-table_name
-    : (database = id_ DOT schema = id_? DOT | schema = id_ DOT)? (
-        table = id_
-        | blocking_hierarchy = BLOCKING_HIERARCHY
-    )
+tableName
+    : (linkedServer = id DOT DOT)? ids+=id (DOT ids +=id)*
     ;
 
-simple_name
-    : (schema = id_ DOT)? name = id_
+simpleName
+    : (schema = id DOT)? name = id
     ;
 
-func_proc_name_schema
-    : ((schema = id_) DOT)? procedure = id_
+funcProcNameSchema
+    : ((schema = id) DOT)? procedure = id
     ;
 
-func_proc_name_database_schema
-    : database = id_? DOT schema = id_? DOT procedure = id_
-    | func_proc_name_schema
+funcProcNameDatabaseSchema
+    : database = id? DOT schema = id? DOT procedure = id
+    | funcProcNameSchema
     ;
 
-func_proc_name_server_database_schema
-    : server = id_? DOT database = id_? DOT schema = id_? DOT procedure = id_
-    | func_proc_name_database_schema
+funcProcNameServerDatabaseSchema
+    : server = id? DOT database = id? DOT schema = id? DOT procedure = id
+    | funcProcNameDatabaseSchema
     ;
 
-ddl_object
-    : full_table_name
+ddlObject
+    : tableName
     | LOCAL_ID
     ;
 
-full_column_name
-    : ((DELETED | INSERTED | full_table_name) DOT)? (
-        column_name = id_
+fullColumnName
+    : ((DELETED | INSERTED | tableName) DOT)? (
+          id
         | (DOLLAR (IDENTITY | ROWGUID))
     )
     ;
 
-column_name_list_with_order
-    : id_ (ASC | DESC)? (COMMA id_ (ASC | DESC)?)*
+columnNameListWithOrder
+    : id (ASC | DESC)? (COMMA id (ASC | DESC)?)*
     ;
 
 //For some reason, sql server allows any number of prefixes:  Here, h is the column: a.b.c.d.e.f.g.h
-insert_column_name_list
-    : col += insert_column_id (COMMA col += insert_column_id)*
+insertColumnNameList
+    : col += insertColumnId (COMMA col += insertColumnId)*
     ;
 
-insert_column_id
-    : (ignore += id_? DOT)* id_
+insertColumnId
+    : (ignore += id? DOT)* id
     ;
 
-column_name_list
-    : col += id_ (COMMA col += id_)*
+columnNameList
+    : col += id (COMMA col += id)*
     ;
 
-cursor_name
-    : id_
+cursorName
+    : id
     | LOCAL_ID
     ;
 
-on_off
+onOff
     : ON
     | OFF
     ;
 
 clustered
     : CLUSTERED
     | NONCLUSTERED
     ;
 
-null_notnull
+nullNotnull
     : NOT? NULL_
     ;
 
-scalar_function_name
-    : func_proc_name_server_database_schema
+scalarFunctionName
+    : funcProcNameServerDatabaseSchema
     | RIGHT
     | LEFT
     | BINARY_CHECKSUM
     | CHECKSUM
     ;
 
-begin_conversation_timer
+beginConversationTimer
     : BEGIN CONVERSATION TIMER LPAREN LOCAL_ID RPAREN TIMEOUT EQ time SEMI?
     ;
 
-begin_conversation_dialog
-    : BEGIN DIALOG (CONVERSATION)? dialog_handle = LOCAL_ID FROM SERVICE initiator_service_name = service_name TO SERVICE target_service_name =
-        service_name (COMMA service_broker_guid = STRING)? ON CONTRACT contract_name (
+beginConversationDialog
+    : BEGIN DIALOG (CONVERSATION)? dialogHandle = LOCAL_ID FROM SERVICE initiatorServiceName = serviceName TO SERVICE targetServiceName =
+        serviceName (COMMA serviceBrokerGuid = STRING)? ON CONTRACT contractName (
         WITH ((RELATED_CONVERSATION | RELATED_CONVERSATION_GROUP) EQ LOCAL_ID COMMA?)? (
             LIFETIME EQ (INT | LOCAL_ID) COMMA?
-        )? (ENCRYPTION EQ on_off)?
+        )? (ENCRYPTION EQ onOff)?
     )? SEMI?
     ;
 
-contract_name
-    : (id_ | expression)
+contractName
+    : (id | expression)
     ;
 
-service_name
-    : (id_ | expression)
+serviceName
+    : (id | expression)
     ;
 
-end_conversation
-    : END CONVERSATION conversation_handle = LOCAL_ID SEMI? (
+endConversation
+    : END CONVERSATION conversationHandle = LOCAL_ID SEMI? (
         WITH (
-            ERROR EQ faliure_code = (LOCAL_ID | STRING) DESCRIPTION EQ failure_text = (
+            ERROR EQ faliureCode = (LOCAL_ID | STRING) DESCRIPTION EQ failureText = (
                 LOCAL_ID
                 | STRING
             )
         )? CLEANUP?
     )?
     ;
 
-waitfor_conversation
-    : WAITFOR? LPAREN get_conversation RPAREN (COMMA? TIMEOUT timeout = time)? SEMI?
+waitforConversation
+    : WAITFOR? LPAREN getConversation RPAREN (COMMA? TIMEOUT timeout = time)? SEMI?
     ;
 
-get_conversation
-    : GET CONVERSATION GROUP conversation_group_id = (STRING | LOCAL_ID) FROM queue = queue_id SEMI?
+getConversation
+    : GET CONVERSATION GROUP conversationGroupId = (STRING | LOCAL_ID) FROM queue = queueId SEMI?
     ;
 
-queue_id
-    : (database_name = id_ DOT schema_name = id_ DOT name = id_)
-    | id_
+queueId
+    : (databaseName = id DOT schemaName = id DOT name = id)
+    | id
     ;
 
-send_conversation
-    : SEND ON CONVERSATION conversation_handle = (STRING | LOCAL_ID) MESSAGE TYPE message_type_name = expression (
-        LPAREN message_body_expression = (STRING | LOCAL_ID) RPAREN
+sendConversation
+    : SEND ON CONVERSATION conversationHandle = (STRING | LOCAL_ID) MESSAGE TYPE messageTypeName = expression (
+        LPAREN messageBodyExpression = (STRING | LOCAL_ID) RPAREN
     )? SEMI?
     ;
 
 // https://msdn.microsoft.com/en-us/library/ms187752.aspx
 // TODO: implement runtime check or add new tokens.
 
-data_type
+dataType
     : scaled = (VARCHAR | NVARCHAR | BINARY_KEYWORD | VARBINARY_KEYWORD | SQUARE_BRACKET_ID) LPAREN MAX RPAREN
-    | ext_type = id_ LPAREN scale = INT COMMA prec = INT RPAREN
-    | ext_type = id_ LPAREN scale = INT RPAREN
-    | ext_type = id_ IDENTITY (LPAREN seed = INT COMMA inc = INT RPAREN)?
-    | double_prec = DOUBLE PRECISION?
-    | unscaled_type = id_
+    | extType = id LPAREN scale = INT COMMA prec = INT RPAREN
+    | extType = id LPAREN scale = INT RPAREN
+    | extType = id IDENTITY (LPAREN seed = INT COMMA inc = INT RPAREN)?
+    | doublePrec = DOUBLE PRECISION?
+    | unscaledType = id
     ;
 
 // https://msdn.microsoft.com/en-us/library/ms179899.aspx
 constant
-    : STRING // string, datetime or uniqueidentifier
-    | HEX
-    | MINUS? (INT | REAL | FLOAT)                    // float or decimal
-    | MINUS? DOLLAR (MINUS | PLUS)? (INT | FLOAT) // money
-    | parameter
-    ;
-
-// To reduce ambiguity, -X is considered as an application of unary operator
-primitive_constant
-    : STRING // string, datetime or uniqueidentifier
-    | HEX
-    | INT
-    | REAL
-    | FLOAT
-    | DOLLAR (MINUS | PLUS)? (INT | FLOAT) // money
+    : con = (
+          STRING
+        | HEX
+        | INT
+        | REAL
+        | FLOAT
+        | MONEY
+        )
     | parameter
     ;
 
 keyword
     : ABORT
     | ABSOLUTE
     | ACCENT_SENSITIVITY
@@ -5311,39 +4753,33 @@
     | ANSI_DEFAULTS
     | ANSI_NULL_DEFAULT
     | ANSI_NULL_DFLT_OFF
     | ANSI_NULL_DFLT_ON
     | ANSI_NULLS
     | ANSI_PADDING
     | ANSI_WARNINGS
-    | APP_NAME
     | APPLICATION_LOG
-    | APPLOCK_MODE
-    | APPLOCK_TEST
     | APPLY
     | ARITHABORT
     | ARITHIGNORE
-    | ASCII
     | ASSEMBLY
-    | ASSEMBLYPROPERTY
     | AT_KEYWORD
     | AUDIT
     | AUDIT_GUID
     | AUTO
     | AUTO_CLEANUP
     | AUTO_CLOSE
     | AUTO_CREATE_STATISTICS
     | AUTO_DROP
     | AUTO_SHRINK
     | AUTO_UPDATE_STATISTICS
     | AUTO_UPDATE_STATISTICS_ASYNC
     | AUTOGROW_ALL_FILES
     | AUTOGROW_SINGLE_FILE
     | AVAILABILITY
-    | AVG
     | BACKUP_CLONEDB
     | BACKUP_PRIORITY
     | BASE64
     | BEGIN_DIALOG
     | BIGINT
     | BINARY_KEYWORD
     | BINARY_CHECKSUM
@@ -5354,98 +4790,74 @@
     | BULK_LOGGED
     | CALLER
     | CAP_CPU_PERCENT
     | CAST
     | TRY_CAST
     | CATALOG
     | CATCH
-    | CERT_ID
-    | CERTENCODED
-    | CERTPRIVATEKEY
     | CHANGE
     | CHANGE_RETENTION
     | CHANGE_TRACKING
-    | CHAR
-    | CHARINDEX
     | CHECKALLOC
     | CHECKCATALOG
     | CHECKCONSTRAINTS
     | CHECKDB
     | CHECKFILEGROUP
     | CHECKSUM
-    | CHECKSUM_AGG
     | CHECKTABLE
     | CLEANTABLE
     | CLEANUP
     | CLONEDATABASE
-    | COL_LENGTH
-    | COL_NAME
     | COLLECTION
     | COLUMN_ENCRYPTION_KEY
     | COLUMN_MASTER_KEY
-    | COLUMNPROPERTY
     | COLUMNS
     | COLUMNSTORE
     | COLUMNSTORE_ARCHIVE
     | COMMITTED
     | COMPATIBILITY_LEVEL
     | COMPRESS_ALL_ROW_GROUPS
     | COMPRESSION_DELAY
     | CONCAT
-    | CONCAT_WS
     | CONCAT_NULL_YIELDS_NULL
     | CONTENT
     | CONTROL
     | COOKIE
-    | COUNT
-    | COUNT_BIG
     | COUNTER
     | CPU
     | CREATE_NEW
     | CREATION_DISPOSITION
     | CREDENTIAL
     | CRYPTOGRAPHIC
     | CUME_DIST
     | CURSOR_CLOSE_ON_COMMIT
     | CURSOR_DEFAULT
-    | CURSOR_STATUS
     | DATA
     | DATA_PURITY
-    | DATABASE_PRINCIPAL_ID
-    | DATABASEPROPERTYEX
-    | DATALENGTH
     | DATE_CORRELATION_OPTIMIZATION
-    | DATEADD
-    | DATEDIFF
-    | DATENAME
-    | DATEPART
     | DAYS
     | DB_CHAINING
     | DB_FAILOVER
-    | DB_ID
-    | DB_NAME
     | DBCC
     | DBREINDEX
     | DECRYPTION
     | DEFAULT_DOUBLE_QUOTE
     | DEFAULT_FULLTEXT_LANGUAGE
     | DEFAULT_LANGUAGE
     | DEFINITION
     | DELAY
     | DELAYED_DURABILITY
     | DELETED
-    | DENSE_RANK
     | DEPENDENTS
     | DES
     | DESCRIPTION
     | DESX
     | DETERMINISTIC
     | DHCP
     | DIALOG
-    | DIFFERENCE
     | DIRECTORY_NAME
     | DISABLE
     | DISABLE_BROKER
     | DISABLED
     | DOCUMENT
     | DROP_EXISTING
     | DROPCLEANBUFFERS
@@ -5460,38 +4872,28 @@
     | ENCRYPTION
     | ENCRYPTION_TYPE
     | ENDPOINT_URL
     | ERROR_BROKER_CONVERSATIONS
     | ESTIMATEONLY
     | EXCLUSIVE
     | EXECUTABLE
-    | EXIST
-    | EXIST_SQUARE_BRACKET
     | EXPAND
     | EXPIRY_DATE
     | EXPLICIT
     | EXTENDED_LOGICAL_CHECKS
     | FAIL_OPERATION
     | FAILOVER_MODE
     | FAILURE
     | FAILURE_CONDITION_LEVEL
     | FAST
     | FAST_FORWARD
-    | FILE_ID
-    | FILE_IDEX
-    | FILE_NAME
     | FILEGROUP
-    | FILEGROUP_ID
-    | FILEGROUP_NAME
-    | FILEGROUPPROPERTY
     | FILEGROWTH
     | FILENAME
     | FILEPATH
-    | FILEPROPERTY
-    | FILEPROPERTYEX
     | FILESTREAM
     | FILTER
     | FIRST
     | FIRST_VALUE
     | FMTONLY
     | FOLLOWING
     | FORCE
@@ -5500,101 +4902,74 @@
     | FORCEPLAN
     | FORCESCAN
     | FORMAT
     | FORWARD_ONLY
     | FREE
     | FULLSCAN
     | FULLTEXT
-    | FULLTEXTCATALOGPROPERTY
-    | FULLTEXTSERVICEPROPERTY
     | GB
     | GENERATED
-    | GETDATE
-    | GETUTCDATE
     | GLOBAL
     | GO
-    | GREATEST
     | GROUP_MAX_REQUESTS
     | GROUPING
-    | GROUPING_ID
     | HADR
-    | HAS_DBACCESS
-    | HAS_PERMS_BY_NAME
     | HASH
     | HEALTH_CHECK_TIMEOUT
     | HIDDEN_KEYWORD
     | HIGH
     | HONOR_BROKER_PRIORITY
     | HOURS
-    | IDENT_CURRENT
-    | IDENT_INCR
-    | IDENT_SEED
     | IDENTITY_VALUE
     | IGNORE_CONSTRAINTS
     | IGNORE_DUP_KEY
     | IGNORE_NONCLUSTERED_COLUMNSTORE_INDEX
     | IGNORE_REPLICATED_TABLE_CACHE
     | IGNORE_TRIGGERS
     | IMMEDIATE
     | IMPERSONATE
     | IMPLICIT_TRANSACTIONS
     | IMPORTANCE
     | INCLUDE_NULL_VALUES
     | INCREMENTAL
-    | INDEX_COL
-    | INDEXKEY_PROPERTY
-    | INDEXPROPERTY
     | INITIATOR
     | INPUT
     | INSENSITIVE
     | INSERTED
     | KWINT
     | IP
-    | IS_MEMBER
-    | IS_ROLEMEMBER
-    | IS_SRVROLEMEMBER
-    | ISJSON
     | ISOLATION
     | JOB
     | JSON
     | JSON_OBJECT
     | JSON_ARRAY
-    | JSON_VALUE
-    | JSON_QUERY
-    | JSON_MODIFY
-    | JSON_PATH_EXISTS
     | KB
     | KEEP
     | KEEPDEFAULTS
     | KEEPFIXED
     | KEEPIDENTITY
     | KEY_SOURCE
     | KEYS
     | KEYSET
     | LAG
     | LAST
     | LAST_VALUE
     | LEAD
-    | LEAST
-    | LEN
     | LEVEL
     | LIST
     | LISTENER
     | LISTENER_URL
     | LOB_COMPACTION
     | LOCAL
     | LOCATION
     | LOCK
     | LOCK_ESCALATION
     | LOGIN
-    | LOGINPROPERTY
     | LOOP
     | LOW
-    | LOWER
-    | LTRIM
     | MANUAL
     | MARK
     | MASKED
     | MATERIALIZED
     | MAX
     | MAX_CPU_PERCENT
     | MAX_DOP
@@ -5607,29 +4982,25 @@
     | MAXDOP
     | MAXRECURSION
     | MAXSIZE
     | MB
     | MEDIUM
     | MEMORY_OPTIMIZED_DATA
     | MESSAGE
-    | MIN
-    | MIN_ACTIVE_ROWVERSION
     | MIN_CPU_PERCENT
     | MIN_IOPS_PER_VOLUME
     | MIN_MEMORY_PERCENT
     | MINUTES
     | MIRROR_ADDRESS
     | MIXED_PAGE_ALLOCATION
     | MODE
     | MODIFY
-    | MODIFY_SQUARE_BRACKET
     | MOVE
     | MULTI_USER
     | NAME
-    | NCHAR
     | NESTED_TRIGGERS
     | NEW_ACCOUNT
     | NEW_BROKER
     | NEW_PASSWORD
     | NEWNAME
     | NEXT
     | NO
@@ -5651,55 +5022,44 @@
     | NOWAIT
     | NTILE
     | NULL_DOUBLE_QUOTE
     | NUMANODE
     | NUMBER
     | NUMERIC_ROUNDABORT
     | OBJECT
-    | OBJECT_DEFINITION
-    | OBJECT_ID
-    | OBJECT_NAME
-    | OBJECT_SCHEMA_NAME
-    | OBJECTPROPERTY
-    | OBJECTPROPERTYEX
     | OFFLINE
     | OFFSET
     | OLD_ACCOUNT
     | ONLINE
     | ONLY
     | OPEN_EXISTING
     | OPENJSON
     | OPTIMISTIC
     | OPTIMIZE
     | OPTIMIZE_FOR_SEQUENTIAL_KEY
-    | ORIGINAL_DB_NAME
-    | ORIGINAL_LOGIN
     | OUT
     | OUTPUT
     | OVERRIDE
     | OWNER
     | OWNERSHIP
     | PAD_INDEX
     | PAGE_VERIFY
     | PAGECOUNT
     | PAGLOCK
     | PARAMETERIZATION
-    | PARSENAME
     | PARSEONLY
     | PARTITION
     | PARTITIONS
     | PARTNER
     | PATH
-    | PATINDEX
     | PAUSE
     | PDW_SHOWSPACEUSED
     | PERCENT_RANK
     | PERCENTILE_CONT
     | PERCENTILE_DISC
-    | PERMISSIONS
     | PERSIST_SAMPLE_PERCENT
     | PHYSICAL_ONLY
     | POISON_MESSAGE_HANDLING
     | POOL
     | PORT
     | PRECEDING
     | PRIMARY_ROLE
@@ -5710,25 +5070,20 @@
     | PRIVATE_KEY
     | PRIVILEGES
     | PROCCACHE
     | PROCEDURE_NAME
     | PROPERTY
     | PROVIDER
     | PROVIDER_KEY_NAME
-    | PWDCOMPARE
-    | PWDENCRYPT
     | QUERY
-    | QUERY_SQUARE_BRACKET
     | QUEUE
     | QUEUE_DELAY
     | QUOTED_IDENTIFIER
-    | QUOTENAME
     | RANDOMIZED
     | RANGE
-    | RANK
     | RC2
     | RC4
     | RC4_128
     | READ_COMMITTED_SNAPSHOT
     | READ_ONLY
     | READ_ONLY_ROUTING_LIST
     | READ_WRITE
@@ -5752,41 +5107,34 @@
     | REPAIR_ALLOW_DATA_LOSS
     | REPAIR_FAST
     | REPAIR_REBUILD
     | REPEATABLE
     | REPEATABLEREAD
     | REPLACE
     | REPLICA
-    | REPLICATE
     | REQUEST_MAX_CPU_TIME_SEC
     | REQUEST_MAX_MEMORY_GRANT_PERCENT
     | REQUEST_MEMORY_GRANT_TIMEOUT_SEC
     | REQUIRED_SYNCHRONIZED_SECONDARIES_TO_COMMIT
     | RESAMPLE
     | RESERVE_DISK_SPACE
     | RESOURCE
     | RESOURCE_MANAGER_LOCATION
     | RESTRICTED_USER
     | RESUMABLE
     | RETENTION
-    | REVERSE
     | ROBUST
     | ROOT
     | ROUTE
     | ROW
-    | ROW_NUMBER
     | ROWGUID
     | ROWLOCK
     | ROWS
-    | RTRIM
     | SAMPLE
-    | SCHEMA_ID
-    | SCHEMA_NAME
     | SCHEMABINDING
-    | SCOPE_IDENTITY
     | SCOPED
     | SCROLL
     | SCROLL_LOCKS
     | SEARCH
     | SECONDARY
     | SECONDARY_ONLY
     | SECONDARY_ROLE
@@ -5799,17 +5147,15 @@
     | SELF
     | SEMI_SENSITIVE
     | SEND
     | SENT
     | SEQUENCE
     | SEQUENCE_NUMBER
     | SERIALIZABLE
-    | SERVERPROPERTY
     | SERVICEBROKER
-    | SESSIONPROPERTY
     | SESSION_TIMEOUT
     | SETERROR
     | SHARE
     | SHARED
     | SHOWCONTIG
     | SHOWPLAN
     | SHOWPLAN_ALL
@@ -5818,44 +5164,28 @@
     | SIGNATURE
     | SIMPLE
     | SINGLE_USER
     | SIZE
     | SMALLINT
     | SNAPSHOT
     | SORT_IN_TEMPDB
-    | SOUNDEX
-    | SPACE_KEYWORD
     | SPARSE
     | SPATIAL_WINDOW_MAX_CELLS
-    | SQL_VARIANT_PROPERTY
     | STANDBY
     | START_DATE
     | STATIC
     | STATISTICS_INCREMENTAL
     | STATISTICS_NORECOMPUTE
-    | STATS_DATE
     | STATS_STREAM
     | STATUS
     | STATUSONLY
-    | STDEV
-    | STDEVP
     | STOPLIST
-    | STR
-    | STRING_AGG
-    | STRING_ESCAPE
-    | STUFF
     | SUBJECT
     | SUBSCRIBE
     | SUBSCRIPTION
-    | SUBSTRING
-    | SUM
-    | SUSER_ID
-    | SUSER_NAME
-    | SUSER_SID
-    | SUSER_SNAME
     | SUSPEND
     | SYMMETRIC
     | SYNCHRONOUS_COMMIT
     | SYNONYM
     | SYSTEM
     | TABLERESULTS
     | TABLOCK
@@ -5870,46 +5200,35 @@
     | TIMEOUT
     | TIMER
     | TINYINT
     | TORN_PAGE_DETECTION
     | TRACKING
     | TRANSACTION_ID
     | TRANSFORM_NOISE_WORDS
-    | TRANSLATE
-    | TRIM
     | TRIPLE_DES
     | TRIPLE_DES_3KEY
     | TRUSTWORTHY
     | TRY
     | TSQL
     | TWO_DIGIT_YEAR_CUTOFF
     | TYPE
-    | TYPE_ID
-    | TYPE_NAME
     | TYPE_WARNING
-    | TYPEPROPERTY
     | UNBOUNDED
     | UNCOMMITTED
-    | UNICODE
     | UNKNOWN
     | UNLIMITED
     | UNMASK
     | UOW
     | UPDLOCK
-    | UPPER
-    | USER_ID
-    | USER_NAME
     | USING
     | VALID_XML
     | VALIDATION
     | VALUE
-    | VALUE_SQUARE_BRACKET
     | VAR
     | VARBINARY_KEYWORD
-    | VARP
     | VERIFY_CLONEDB
     | VERSION
     | VIEW_METADATA
     | VIEWS
     | WAIT
     | WELL_FORMED_XML
     | WITHOUT_ARRAY_WRAPPER
@@ -5941,103 +5260,78 @@
     | AUTOMATED_BACKUP_PREFERENCE
     | AUTOMATIC
     | AVAILABILITY_MODE
     | BEFORE
     | BLOCK
     | BLOCKERS
     | BLOCKSIZE
-    | BLOCKING_HIERARCHY
     | BUFFER
     | BUFFERCOUNT
     | CACHE
     | CALLED
     | CERTIFICATE
     | CHANGETABLE
     | CHANGES
     | CHECK_POLICY
     | CHECK_EXPIRATION
     | CLASSIFIER_FUNCTION
     | CLUSTER
-    | COMPRESS
     | COMPRESSION
     | CONNECT
     | CONNECTION
     | CONFIGURATION
-    | CONNECTIONPROPERTY
     | CONTAINMENT
     | CONTEXT
-    | CONTEXT_INFO
     | CONTINUE_AFTER_ERROR
     | CONTRACT
     | CONTRACT_NAME
     | CONVERSATION
     | COPY_ONLY
-    | CURRENT_REQUEST_ID
-    | CURRENT_TRANSACTION_ID
     | CYCLE
     | DATA_COMPRESSION
     | DATA_SOURCE
     | DATABASE_MIRRORING
     | DATASPACE
     | DDL
-    | DECOMPRESS
     | DEFAULT_DATABASE
     | DEFAULT_SCHEMA
     | DIAGNOSTICS
     | DIFFERENTIAL
     | DISTRIBUTION
     | DTC_SUPPORT
     | ENABLED
     | ENDPOINT
     | ERROR
-    | ERROR_LINE
-    | ERROR_MESSAGE
-    | ERROR_NUMBER
-    | ERROR_PROCEDURE
-    | ERROR_SEVERITY
-    | ERROR_STATE
     | EVENT
     | EVENTDATA
     | EVENT_RETENTION_MODE
     | EXECUTABLE_FILE
     | EXPIREDATE
     | EXTENSION
     | EXTERNAL_ACCESS
     | FAILOVER
     | FAILURECONDITIONLEVEL
     | FAN_IN
     | FILE_SNAPSHOT
     | FORCESEEK
     | FORCE_SERVICE_ALLOW_DATA_LOSS
-    | FORMATMESSAGE
     | GET
-    | GET_FILESTREAM_TRANSACTION_CONTEXT
-    | GETANCESTOR
-    | GETANSINULL
-    | GETDESCENDANT
-    | GETLEVEL
-    | GETREPARENTEDVALUE
     | GETROOT
     | GOVERNOR
     | HASHED
     | HEALTHCHECKTIMEOUT
     | HEAP
     | HIERARCHYID
-    | HOST_ID
-    | HOST_NAME
     | IIF
     | IO
     | INCLUDE
     | INCREMENT
     | INFINITE
     | INIT
     | INSTEAD
-    | ISDESCENDANTOF
-    | ISNULL
-    | ISNUMERIC
     | KERBEROS
     | KEY_PATH
     | KEY_STORE_PROVIDER_NAME
     | LANGUAGE
     | LIBRARY
     | LIFETIME
     | LINKED
@@ -6062,16 +5356,14 @@
     | MEMBER
     | MEMORY_PARTITION_MODE
     | MESSAGE_FORWARDING
     | MESSAGE_FORWARD_SIZE
     | MINVALUE
     | MIRROR
     | MUST_CHANGE
-    | NEWID
-    | NEWSEQUENTIALID
     | NOFORMAT
     | NOINIT
     | NONE
     | NOREWIND
     | NOSKIP
     | NOUNLOAD
     | NO_CHECKSUM
@@ -6108,15 +5400,14 @@
     | RESTART
     | RESUME
     | RETAINDAYS
     | RETURNS
     | REWIND
     | ROLE
     | ROUND_ROBIN
-    | ROWCOUNT_BIG
     | RSA_512
     | RSA_1024
     | RSA_2048
     | RSA_3072
     | RSA_4096
     | SAFETY
     | SAFE
@@ -6124,15 +5415,14 @@
     | SCHEME
     | SCRIPT
     | SERVER
     | SERVICE
     | SERVICE_BROKER
     | SERVICE_NAME
     | SESSION
-    | SESSION_CONTEXT
     | SETTINGS
     | SHRINKLOG
     | SID
     | SKIP_KEYWORD
     | SOFTNUMA
     | SOURCE
     | SPECIFICATION
@@ -6166,139 +5456,64 @@
     | VERBOSELOGGING
     | VISIBILITY
     | WAIT_AT_LOW_PRIORITY
     | WINDOWS
     | WITHOUT
     | WITNESS
     | XACT_ABORT
-    | XACT_STATE
-    //
-    | ABS
-    | ACOS
-    | ASIN
-    | ATAN
-    | ATN2
-    | CEILING
-    | COS
-    | COT
-    | DEGREES
-    | EXP
-    | FLOOR
-    | LOG10
-    | PI
-    | POWER
-    | RADIANS
-    | RAND
-    | ROUND
-    | SIGN
-    | SIN
-    | SQRT
-    | SQUARE
-    | TAN
-    //
-    | CURRENT_TIMEZONE
-    | CURRENT_TIMEZONE_ID
-    | DATE_BUCKET
-    | DATEDIFF_BIG
-    | DATEFROMPARTS
-    | DATETIME2FROMPARTS
-    | DATETIMEFROMPARTS
-    | DATETIMEOFFSETFROMPARTS
-    | DATETRUNC
-    | DAY
-    | EOMONTH
-    | ISDATE
-    | MONTH
-    | SMALLDATETIMEFROMPARTS
-    | SWITCHOFFSET
-    | SYSDATETIME
-    | SYSDATETIMEOFFSET
-    | SYSUTCDATETIME
-    | TIMEFROMPARTS
-    | TODATETIMEOFFSET
-    | YEAR
-    //
-    | QUARTER
-    | DAYOFYEAR
-    | WEEK
-    | HOUR
-    | MINUTE
-    | SECOND
-    | MILLISECOND
-    | MICROSECOND
-    | NANOSECOND
-    | TZOFFSET
-    | ISO_WEEK
-    | WEEKDAY
-    //
-    | YEAR_ABBR
-    | QUARTER_ABBR
-    | MONTH_ABBR
-    | DAYOFYEAR_ABBR
-    | DAY_ABBR
-    | WEEK_ABBR
-    | HOUR_ABBR
-    | MINUTE_ABBR
-    | SECOND_ABBR
-    | MILLISECOND_ABBR
-    | MICROSECOND_ABBR
-    | NANOSECOND_ABBR
-    | TZOFFSET_ABBR
-    | ISO_WEEK_ABBR
-    | WEEKDAY_ABBR
     //
     | SP_EXECUTESQL
-    //Build-ins:
+    //Built-ins:
     | VARCHAR
     | NVARCHAR
     | PRECISION //For some reason this is possible to use as ID
     | FILESTREAM_ON
     ;
 
 // https://msdn.microsoft.com/en-us/library/ms175874.aspx
-id_
+id
     : ID
     | TEMP_ID
     | DOUBLE_QUOTE_ID
-    | DOUBLE_QUOTE_BLANK
+    | DOUBLE_QUOTE_BLANK // TODO: This is unnecessary I think - remove
     | SQUARE_BRACKET_ID
     | keyword
     | RAW
     ;
 
-simple_id
+simpleId
     : ID
     ;
 
-id_or_string
-    : id_
+idOrString
+    : id
     | STRING
     ;
 
 // https://msdn.microsoft.com/en-us/library/ms188074.aspx
 // Spaces are allowed for comparison operators.
-comparison_operator
+comparisonOperator
     : EQ
     | GT
     | LT
     | LT EQ
     | GT EQ
     | LT GT
     | EQ
     | GT
     | LT
     ;
 
-assignment_operator
+assignmentOperator
     : PE
     | ME
     | SE
     | DE
     | MEA
     | AND_ASSIGN
     | XOR_ASSIGN
     | OR_ASSIGN
     ;
 
-file_size
+fileSize
     : INT (KB | MB | GB | TB | MOD)?
-    ;
+    ;
```

### Comparing `databricks_labs_remorph-0.1.7/core/src/main/scala/com/databricks/labs/remorph/parsers/IncompleteParser.scala` & `databricks_labs_remorph-0.2.0/core/src/main/scala/com/databricks/labs/remorph/parsers/IncompleteParser.scala`

 * *Files identical despite different names*

### Comparing `databricks_labs_remorph-0.1.7/core/src/main/scala/com/databricks/labs/remorph/parsers/intermediate/catalog.scala` & `databricks_labs_remorph-0.2.0/core/src/main/scala/com/databricks/labs/remorph/parsers/intermediate/catalog.scala`

 * *Files identical despite different names*

### Comparing `databricks_labs_remorph-0.1.7/core/src/main/scala/com/databricks/labs/remorph/parsers/intermediate/commands.scala` & `databricks_labs_remorph-0.2.0/core/src/main/scala/com/databricks/labs/remorph/parsers/intermediate/commands.scala`

 * *Files identical despite different names*

### Comparing `databricks_labs_remorph-0.1.7/core/src/main/scala/com/databricks/labs/remorph/parsers/intermediate/expressions.scala` & `databricks_labs_remorph-0.2.0/core/src/main/scala/com/databricks/labs/remorph/parsers/intermediate/expressions.scala`

 * *Files 2% similar despite different names*

```diff
@@ -28,21 +28,22 @@
 abstract class NullOrdering
 case object SortNullsUnspecified extends NullOrdering
 case object SortNullsFirst extends NullOrdering
 case object SortNullsLast extends NullOrdering
 
 case class SortOrder(child: Expression, direction: SortDirection, nullOrdering: NullOrdering) extends Expression {}
 
-case class Cast(expr: Expression, dataType: DataType, type_str: String) extends Expression {}
+case class Cast(expr: Expression, dataType: DataType, type_str: String = "", returnNullOnError: Boolean = false)
+    extends Expression {}
 
 case class Decimal(value: String, precision: Option[Int], scale: Option[Int]) extends Expression {}
 
 case class CalendarInterval(months: Int, days: Int, microseconds: Long) extends Expression {}
 
-case class ArrayExpr(dataType: DataType, elements: Seq[Literal]) extends Expression {}
+case class ArrayExpr(dataType: Option[DataType], elements: Seq[Literal]) extends Expression {}
 
 case class MapExpr(key_type: DataType, value_type: DataType, keys: Seq[Literal], values: Seq[Literal])
     extends Expression {}
 
 case class Struct(struct_type: DataType, elements: Seq[Literal]) extends Expression {}
 
 case class Literal(
@@ -71,15 +72,16 @@
 case class UnresolvedAttribute(unparsed_identifier: String, plan_id: Long, is_metadata_column: Boolean)
     extends Expression {}
 
 case class UnresolvedFunction(
     function_name: String,
     arguments: Seq[Expression],
     is_distinct: Boolean,
-    is_user_defined_function: Boolean)
+    is_user_defined_function: Boolean,
+    has_incorrect_argc: Boolean = false)
     extends Expression {}
 
 case class ExpressionString(expression: String) extends Expression {}
 
 case class UnresolvedStar(unparsed_target: String) extends Expression {}
 
 case class UnresolvedRegex(col_name: String, plan_id: Long) extends Expression {}
```

### Comparing `databricks_labs_remorph-0.1.7/core/src/main/scala/com/databricks/labs/remorph/parsers/intermediate/relations.scala` & `databricks_labs_remorph-0.2.0/core/src/main/scala/com/databricks/labs/remorph/parsers/intermediate/relations.scala`

 * *Files identical despite different names*

### Comparing `databricks_labs_remorph-0.1.7/core/src/main/scala/com/databricks/labs/remorph/parsers/intermediate/types.scala` & `databricks_labs_remorph-0.2.0/core/src/main/scala/com/databricks/labs/remorph/parsers/intermediate/types.scala`

 * *Files 12% similar despite different names*

```diff
@@ -18,18 +18,20 @@
 // String types
 case class StringType() extends DataType
 case class CharType(size: Option[Int]) extends DataType
 case class VarCharType(size: Option[Int]) extends DataType
 
 // Datatime types
 case class DateType() extends DataType
+case class TimeType() extends DataType
 case class TimestampType() extends DataType
 case class TimestampNTZType() extends DataType
 
 // Interval types
+case class IntervalType() extends DataType
 case class CalendarIntervalType() extends DataType
 case class YearMonthIntervalType() extends DataType
 case class DayTimeIntervalType() extends DataType
 
 // Complex types
 case class ArrayType() extends DataType
 case class StructType() extends DataType
```

### Comparing `databricks_labs_remorph-0.1.7/core/src/main/scala/com/databricks/labs/remorph/parsers/snowflake/DataTypeBuilder.scala` & `databricks_labs_remorph-0.2.0/core/src/main/scala/com/databricks/labs/remorph/parsers/snowflake/DataTypeBuilder.scala`

 * *Files identical despite different names*

### Comparing `databricks_labs_remorph-0.1.7/core/src/main/scala/com/databricks/labs/remorph/parsers/snowflake/SnowflakeAstBuilder.scala` & `databricks_labs_remorph-0.2.0/core/src/main/scala/com/databricks/labs/remorph/parsers/snowflake/SnowflakeAstBuilder.scala`

 * *Files identical despite different names*

### Comparing `databricks_labs_remorph-0.1.7/core/src/main/scala/com/databricks/labs/remorph/parsers/snowflake/SnowflakeExpressionBuilder.scala` & `databricks_labs_remorph-0.2.0/core/src/main/scala/com/databricks/labs/remorph/parsers/snowflake/SnowflakeExpressionBuilder.scala`

 * *Files 20% similar despite different names*

```diff
@@ -1,11 +1,12 @@
 package com.databricks.labs.remorph.parsers.snowflake
 
-import com.databricks.labs.remorph.parsers.{ParserCommon, IncompleteParser, intermediate => ir}
+import com.databricks.labs.remorph.parsers.{IncompleteParser, ParserCommon, intermediate => ir}
 import com.databricks.labs.remorph.parsers.snowflake.SnowflakeParser._
+import org.antlr.v4.runtime.Token
 
 import scala.collection.JavaConverters._
 class SnowflakeExpressionBuilder
     extends SnowflakeParserBaseVisitor[ir.Expression]
     with ParserCommon
     with IncompleteParser[ir.Expression] {
 
@@ -29,32 +30,33 @@
 
   private def buildAlias(ctx: As_aliasContext, input: ir.Expression): ir.Expression =
     Option(ctx).fold(input) { c =>
       val alias = c.alias().id_().getText
       ir.Alias(input, Seq(alias), None)
     }
   override def visitColumn_name(ctx: Column_nameContext): ir.Expression = {
+    // TODO: Build table as per TSQl
     ir.Column(ctx.id_(0).getText)
   }
 
   override def visitPrimitive_expression(ctx: Primitive_expressionContext): ir.Expression = {
-    if (ctx.id_(0) != null) {
-      val columnName = ctx.id_(0).getText
+    if (!ctx.id_().isEmpty) {
+      val columnName = ctx.id_().asScala.map(_.getText).mkString(".")
       ir.Column(columnName)
     } else {
       super.visitPrimitive_expression(ctx)
     }
   }
 
   override def visitOrder_item(ctx: Order_itemContext): ir.Expression = {
     val columnName = ctx.id_().getText
     ir.Column(columnName)
   }
 
-  override def visitLiteral(ctx: LiteralContext): ir.Literal = {
+  override def visitLiteral(ctx: LiteralContext): ir.Expression = {
     val sign = Option(ctx.sign()).map(_ => "-").getOrElse("")
     if (ctx.STRING() != null) {
       ir.Literal(string = Some(removeQuotes(ctx.STRING().getText)))
     } else if (ctx.DECIMAL() != null) {
       visitDecimal(sign + ctx.DECIMAL().getText)
     } else if (ctx.FLOAT() != null) {
       visitDecimal(sign + ctx.FLOAT().getText)
@@ -83,35 +85,96 @@
     case d if d.isValidLong => ir.Literal(long = Some(d.toLong))
     case d if d.isValidShort => ir.Literal(short = Some(d.toShort))
     case d if d.isDecimalFloat || d.isExactFloat => ir.Literal(float = Some(d.toFloat))
     case d if d.isDecimalDouble || d.isExactDouble => ir.Literal(double = Some(d.toDouble))
     case _ => ir.Literal(decimal = Some(ir.Decimal(decimal, None, None)))
   }
 
-  override def visitExpr(ctx: ExprContext): ir.Expression = ctx match {
-    case c if c.AND() != null =>
-      val left = ctx.expr(0).accept(this)
-      val right = ctx.expr(1).accept(this)
-      ir.And(left, right)
-    case c if c.OR() != null =>
-      val left = ctx.expr(0).accept(this)
-      val right = ctx.expr(1).accept(this)
-      ir.Or(left, right)
-    case c if c.comparison_operator() != null =>
-      val left = ctx.expr(0).accept(this)
-      val right = ctx.expr(1).accept(this)
-      buildComparisonExpression(ctx.comparison_operator(), left, right)
-    case c if c.over_clause() != null =>
-      val windowFunction = c.expr(0).accept(this)
-      buildWindow(c.over_clause(), windowFunction)
-    case c => visitChildren(c)
+  override def visitExprNextval(ctx: ExprNextvalContext): ir.Expression = {
+    ir.NextValue(ctx.object_name().getText)
+  }
+
+  override def visitExprArrayAccess(ctx: ExprArrayAccessContext): ir.Expression = {
+    ir.ArrayAccess(ctx.expr(0).accept(this), ctx.expr(1).accept(this))
+  }
+
+  override def visitExprJsonAccess(ctx: ExprJsonAccessContext): ir.Expression = {
+    val jsonPath = buildJsonPath(ctx.json_path())
+    ir.JsonAccess(ctx.expr().accept(this), jsonPath)
+  }
+
+  override def visitExprCollate(ctx: ExprCollateContext): ir.Expression = {
+    ir.Collate(ctx.expr().accept(this), removeQuotes(ctx.string().getText))
+  }
+
+  override def visitExprNot(ctx: ExprNotContext): ir.Expression = {
+    ctx.NOT().asScala.foldLeft(ctx.expr().accept(this)) { case (e, _) => ir.Not(e) }
+  }
+
+  override def visitExprAnd(ctx: ExprAndContext): ir.Expression = {
+    val left = ctx.expr(0).accept(this)
+    val right = ctx.expr(1).accept(this)
+    ir.And(left, right)
+  }
+
+  override def visitExprOr(ctx: ExprOrContext): ir.Expression = {
+    val left = ctx.expr(0).accept(this)
+    val right = ctx.expr(1).accept(this)
+    ir.Or(left, right)
+  }
+
+  override def visitExprPredicate(ctx: ExprPredicateContext): ir.Expression = {
+    buildPredicatePartial(ctx.predicate_partial(), ctx.expr().accept(this))
+  }
+
+  override def visitExprComparison(ctx: ExprComparisonContext): ir.Expression = {
+    val left = ctx.expr(0).accept(this)
+    val right = ctx.expr(1).accept(this)
+    buildComparisonExpression(ctx.comparison_operator(), left, right)
+  }
+
+  override def visitExprOver(ctx: ExprOverContext): ir.Expression = {
+    buildWindow(ctx.over_clause(), ctx.expr().accept(this))
+  }
+
+  override def visitExprAscribe(ctx: ExprAscribeContext): ir.Expression = {
+    ir.Cast(ctx.expr().accept(this), DataTypeBuilder.buildDataType(ctx.data_type()))
+  }
 
+  override def visitExprSign(ctx: ExprSignContext): ir.Expression = ctx.sign() match {
+    case c if c.PLUS() != null => ir.UPlus(ctx.expr().accept(this))
+    case c if c.MINUS() != null => ir.UMinus(ctx.expr().accept(this))
   }
 
-  private def buildComparisonExpression(
+  override def visitExprPrecedence0(ctx: ExprPrecedence0Context): ir.Expression = {
+    buildBinaryOperation(ctx.op, ctx.expr(0).accept(this), ctx.expr(1).accept(this))
+  }
+
+  override def visitExprPrecedence1(ctx: ExprPrecedence1Context): ir.Expression = {
+    buildBinaryOperation(ctx.op, ctx.expr(0).accept(this), ctx.expr(1).accept(this))
+  }
+
+  private def buildJsonPath(ctx: Json_pathContext): Seq[String] =
+    ctx.json_path_elem().asScala.map {
+      case elem if elem.ID() != null => elem.ID().getText
+      case elem if elem.DOUBLE_QUOTE_ID() != null =>
+        elem.DOUBLE_QUOTE_ID().getText.stripPrefix("\"").stripSuffix("\"")
+    }
+
+  private def buildBinaryOperation(operator: Token, left: ir.Expression, right: ir.Expression): ir.Expression =
+    operator.getType match {
+      case STAR => ir.Multiply(left, right)
+      case DIVIDE => ir.Divide(left, right)
+      case PLUS => ir.Add(left, right)
+      case MINUS => ir.Subtract(left, right)
+      case MODULE => ir.Mod(left, right)
+      case PIPE_PIPE => ir.Concat(left, right)
+    }
+
+  private[snowflake] def buildComparisonExpression(
       op: Comparison_operatorContext,
       left: ir.Expression,
       right: ir.Expression): ir.Expression = {
     if (op.EQ() != null) {
       ir.Equals(left, right)
     } else if (op.NE() != null || op.LTGT() != null) {
       ir.NotEquals(left, right)
@@ -120,27 +183,62 @@
     } else if (op.LT() != null) {
       ir.LesserThan(left, right)
     } else if (op.GE() != null) {
       ir.GreaterThanOrEqual(left, right)
     } else if (op.LE() != null) {
       ir.LesserThanOrEqual(left, right)
     } else {
-      visitChildren(op)
+      ir.UnresolvedExpression(op.getText)
     }
   }
 
+  override def visitIff_expr(ctx: Iff_exprContext): ir.Expression = {
+    val condition = ctx.search_condition().accept(this)
+    val thenBranch = ctx.expr(0).accept(this)
+    val elseBranch = ctx.expr(1).accept(this)
+    ir.Iff(condition, thenBranch, elseBranch)
+  }
+
   override def visitSearch_condition(ctx: Search_conditionContext): ir.Expression = {
     val pred = ctx.predicate().accept(this)
     if (ctx.NOT().size() % 2 == 1) {
       ir.Not(pred)
     } else {
       pred
     }
   }
 
+  override def visitArr_literal(ctx: Arr_literalContext): ir.Expression = {
+    val elementsExpressions = ctx.value().asScala.map(_.accept(this))
+    val elements = elementsExpressions.collect { case lit: ir.Literal => lit }
+    if (elementsExpressions.size != elements.size) {
+      ir.UnresolvedExpression(ctx.getText)
+    } else {
+      ir.Literal(array = Some(ir.ArrayExpr(dataType = None, elements = elements)))
+    }
+  }
+
+  override def visitCast_expr(ctx: Cast_exprContext): ir.Expression = ctx match {
+    case c if c.cast_op != null =>
+      val expression = c.expr().accept(this)
+      val dataType = DataTypeBuilder.buildDataType(c.data_type())
+      ir.Cast(expression, dataType, returnNullOnError = c.TRY_CAST() != null)
+    case c if c.conversion != null =>
+      ir.Cast(c.expr().accept(this), extractDateTimeType(c.conversion))
+    case c if c.INTERVAL() != null =>
+      ir.Cast(c.expr().accept(this), ir.IntervalType())
+  }
+
+  private def extractDateTimeType(t: Token): ir.DataType = t.getType match {
+    // default timestamp type is TIMESTAMP_NZT
+    case TO_TIMESTAMP => ir.TimestampNTZType()
+    case TO_TIME | TIME => ir.TimeType()
+    case TO_DATE | DATE => ir.DateType()
+  }
+
   override def visitRanking_windowed_function(ctx: Ranking_windowed_functionContext): ir.Expression = {
     val windowFunction = buildWindowFunction(ctx)
     buildWindow(ctx.over_clause(), windowFunction)
   }
 
   private def buildWindow(ctx: Over_clauseContext, windowFunction: ir.Expression): ir.Expression = {
     val overClause = Option(ctx)
@@ -152,23 +250,20 @@
     ir.Window(
       window_function = windowFunction,
       partition_spec = partitionSpec,
       sort_order = sortOrder,
       frame_spec = DummyWindowFrame)
   }
 
-  private def buildWindowFunction(ctx: Ranking_windowed_functionContext): ir.Expression = {
-    if (ctx.ROW_NUMBER() != null) {
-      ir.RowNumber
-    } else if (ctx.NTILE() != null) {
+  private[snowflake] def buildWindowFunction(ctx: Ranking_windowed_functionContext): ir.Expression = ctx match {
+    case c if c.ROW_NUMBER() != null => ir.RowNumber
+    case c if c.NTILE() != null =>
       val parameter = ctx.expr(0).accept(this)
       ir.NTile(parameter)
-    } else {
-      visitChildren(ctx)
-    }
+    case c => ir.UnresolvedExpression(c.getText)
   }
 
   private def buildPartitionSpec(ctx: Partition_byContext): Seq[ir.Expression] = {
     ctx.expr_list().expr().asScala.map(_.accept(this))
   }
 
   private[snowflake] def buildSortOrder(ctx: Order_by_exprContext): Seq[ir.SortOrder] = {
@@ -222,48 +317,52 @@
       case c if c.switch_search_condition_section().size() > 0 =>
         val branches = c.switch_search_condition_section().asScala.map { branch =>
           ir.WhenBranch(branch.search_condition().accept(this), branch.expr().accept(this))
         }
         ir.Case(None, branches, otherwise)
     }
   }
-  override def visitPredicate(ctx: PredicateContext): ir.Expression = {
+  override def visitPredicate(ctx: PredicateContext): ir.Expression = ctx match {
+    case c if c.EXISTS() != null =>
+      ir.Exists(c.subquery().accept(new SnowflakeRelationBuilder))
+    case c if c.predicate_partial() != null =>
+      val expr = c.expr().accept(this)
+      buildPredicatePartial(c.predicate_partial(), expr)
+    case c => visitChildren(c)
+  }
 
+  private def buildPredicatePartial(ctx: Predicate_partialContext, expression: ir.Expression): ir.Expression = {
     val predicate = ctx match {
-      case c if c.EXISTS() != null =>
-        ir.Exists(c.subquery().accept(new SnowflakeRelationBuilder))
+
       case c if c.IN() != null =>
-        ir.IsIn(c.subquery().accept(new SnowflakeRelationBuilder), c.expr(0).accept(this))
+        ir.IsIn(c.subquery().accept(new SnowflakeRelationBuilder), expression)
       case c if c.BETWEEN() != null =>
-        val expression = c.expr(0).accept(this)
-        val lowerBound = c.expr(1).accept(this)
-        val upperBound = c.expr(2).accept(this)
+        val lowerBound = c.expr(0).accept(this)
+        val upperBound = c.expr(1).accept(this)
         ir.And(ir.GreaterThanOrEqual(expression, lowerBound), ir.LesserThanOrEqual(expression, upperBound))
       case c if c.LIKE() != null || c.ILIKE() != null =>
-        val expression = c.expr(0).accept(this)
         val patterns = if (c.ANY() != null) {
           c.expr()
             .asScala
-            .filter(e => occursBefore(c.LR_BRACKET(), e) && occursBefore(e, c.RR_BRACKET()))
-            .map(_.accept(this)) _
+            .filter(e => occursBefore(c.L_PAREN(), e) && occursBefore(e, c.R_PAREN()))
+            .map(_.accept(this))
         } else {
-          Seq(c.expr(1).accept(this))
+          Seq(c.expr(0).accept(this))
         }
         val escape = Option(c.ESCAPE())
           .flatMap(_ =>
             c.expr()
               .asScala
               .find(occursBefore(c.ESCAPE(), _))
               .map(_.accept(this)))
         ir.Like(expression, patterns, escape, c.LIKE() != null)
       case c if c.RLIKE() != null =>
-        val expression = c.expr(0).accept(this)
-        val pattern = c.expr(1).accept(this)
+        val pattern = c.expr(0).accept(this)
         ir.RLike(expression, pattern)
       case c if c.IS() != null =>
-        val isNull: ir.Expression = ir.IsNull(c.expr(0).accept(this))
+        val isNull: ir.Expression = ir.IsNull(expression)
         Option(c.null_not_null().NOT()).fold(isNull)(_ => ir.Not(isNull))
-      case c => visitChildren(c)
     }
     Option(ctx.NOT()).fold(predicate)(_ => ir.Not(predicate))
   }
+
 }
```

### Comparing `databricks_labs_remorph-0.1.7/core/src/main/scala/com/databricks/labs/remorph/parsers/snowflake/SnowflakeRelationBuilder.scala` & `databricks_labs_remorph-0.2.0/core/src/main/scala/com/databricks/labs/remorph/parsers/snowflake/SnowflakeRelationBuilder.scala`

 * *Files 12% similar despite different names*

```diff
@@ -153,30 +153,22 @@
       input = relation,
       ids = unpivotColumns,
       values = None,
       variable_column_name = variableColumnName,
       value_column_name = valueColumnName)
   }
 
-  private def translateAggregateFunction(aggFunc: Id_Context, parameter: Id_Context): ir.Expression = {
+  private[snowflake] def translateAggregateFunction(aggFunc: Id_Context, parameter: Id_Context): ir.Expression = {
     val column = ir.Column(parameter.getText)
-    if (aggFunc.builtin_function() != null) {
-      if (aggFunc.builtin_function().SUM() != null) {
-        ir.Sum(column)
-      } else if (aggFunc.builtin_function().AVG() != null) {
-        ir.Avg(column)
-      } else if (aggFunc.builtin_function().COUNT() != null) {
-        ir.Count(column)
-      } else if (aggFunc.builtin_function().MIN() != null) {
-        ir.Min(column)
-      } else {
-        null
-      }
-    } else {
-      null
+    aggFunc match {
+      case f if f.builtin_function() != null && f.builtin_function().SUM() != null => ir.Sum(column)
+      case f if f.builtin_function() != null && f.builtin_function().AVG() != null => ir.Avg(column)
+      case f if f.builtin_function() != null && f.builtin_function().COUNT() != null => ir.Count(column)
+      case f if f.builtin_function() != null && f.builtin_function().MIN() != null => ir.Min(column)
+      case _ => ir.UnresolvedExpression(aggFunc.getText)
     }
   }
   override def visitTable_source_item_joined(ctx: Table_source_item_joinedContext): ir.Relation = {
 
     def buildJoin(left: ir.Relation, right: Join_clauseContext): ir.Join = {
 
       ir.Join(
@@ -187,15 +179,15 @@
         Seq(),
         ir.JoinDataType(is_left_struct = false, is_right_struct = false))
     }
     val left = ctx.object_ref().accept(this)
     ctx.join_clause().asScala.foldLeft(left)(buildJoin)
   }
 
-  private def translateJoinType(joinType: Join_typeContext): ir.JoinType = {
+  private[snowflake] def translateJoinType(joinType: Join_typeContext): ir.JoinType = {
     if (joinType == null || joinType.outer_join() == null) {
       ir.InnerJoin
     } else if (joinType.outer_join().LEFT() != null) {
       ir.LeftOuterJoin
     } else if (joinType.outer_join().RIGHT() != null) {
       ir.RightOuterJoin
     } else if (joinType.outer_join().FULL() != null) {
```

### Comparing `databricks_labs_remorph-0.1.7/core/src/main/scala/com/databricks/labs/remorph/parsers/snowflake/package.scala` & `databricks_labs_remorph-0.2.0/core/src/main/scala/com/databricks/labs/remorph/parsers/snowflake/package.scala`

 * *Files identical despite different names*

### Comparing `databricks_labs_remorph-0.1.7/core/src/test/scala/com/databricks/labs/remorph/parsers/snowflake/DataTypeBuilderSpec.scala` & `databricks_labs_remorph-0.2.0/core/src/test/scala/com/databricks/labs/remorph/parsers/snowflake/DataTypeBuilderSpec.scala`

 * *Files identical despite different names*

### Comparing `databricks_labs_remorph-0.1.7/core/src/test/scala/com/databricks/labs/remorph/parsers/snowflake/SnowflakeAstBuilderSpec.scala` & `databricks_labs_remorph-0.2.0/core/src/test/scala/com/databricks/labs/remorph/parsers/snowflake/SnowflakeAstBuilderSpec.scala`

 * *Files 1% similar despite different names*

```diff
@@ -216,14 +216,17 @@
     "translate queries with LIMIT and OFFSET" in {
       singleQueryExample(
         query = "SELECT a FROM b LIMIT 5",
         expectedAst = Project(Limit(NamedTable("b", Map.empty, is_streaming = false), 5), Seq(Column("a"))))
       singleQueryExample(
         query = "SELECT a FROM b LIMIT 5 OFFSET 10",
         expectedAst = Project(Offset(Limit(NamedTable("b", Map.empty, is_streaming = false), 5), 10), Seq(Column("a"))))
+      singleQueryExample(
+        query = "SELECT a FROM b OFFSET 10 FETCH FIRST 42",
+        expectedAst = Project(Offset(NamedTable("b", Map.empty, is_streaming = false), 10), Seq(Column("a"))))
     }
     "translate a query with PIVOT" in {
       singleQueryExample(
         query = "SELECT a FROM b PIVOT (SUM(a) FOR c IN ('foo', 'bar'))",
         expectedAst = Project(
           Aggregate(
             input = NamedTable("b", Map.empty, is_streaming = false),
@@ -366,20 +369,20 @@
           by_name = false,
           allow_missing_columns = false))
     }
 
     "translate batches of queries" in {
       example(
         """
-          |SELECT 1 FROM t1;
-          |SELECT 2 FROM t2;
+          |CREATE TABLE t1 (x VARCHAR);
+          |SELECT x FROM t1;
           |SELECT 3 FROM t3;
           |""".stripMargin,
         _.snowflake_file(),
         Batch(
           Seq(
-            Project(namedTable("t1"), Seq(Literal(integer = Some(1)))),
-            Project(namedTable("t2"), Seq(Literal(integer = Some(2)))),
+            CreateTableCommand("t1", Seq(ColumnDeclaration("x", VarCharType(None)))),
+            Project(namedTable("t1"), Seq(Column("x"))),
             Project(namedTable("t3"), Seq(Literal(integer = Some(3)))))))
     }
   }
 }
```

### Comparing `databricks_labs_remorph-0.1.7/core/src/test/scala/com/databricks/labs/remorph/parsers/snowflake/SnowflakeExpressionBuilderSpec.scala` & `databricks_labs_remorph-0.2.0/core/src/test/scala/com/databricks/labs/remorph/parsers/snowflake/SnowflakeExpressionBuilderSpec.scala`

 * *Files 27% similar despite different names*

```diff
@@ -1,16 +1,23 @@
 package com.databricks.labs.remorph.parsers.snowflake
 
 import com.databricks.labs.remorph.parsers.intermediate._
+import com.databricks.labs.remorph.parsers.snowflake.SnowflakeParser.{Comparison_operatorContext, LiteralContext, Ranking_windowed_functionContext}
 import org.scalatest.matchers.should.Matchers
 import org.scalatest.wordspec.AnyWordSpec
+import org.mockito.Mockito._
+import org.scalatestplus.mockito.MockitoSugar
 
-class SnowflakeExpressionBuilderSpec extends AnyWordSpec with SnowflakeParserTestCommon with Matchers {
+class SnowflakeExpressionBuilderSpec
+    extends AnyWordSpec
+    with SnowflakeParserTestCommon
+    with Matchers
+    with MockitoSugar {
 
-  override protected def astBuilder: SnowflakeParserBaseVisitor[_] = new SnowflakeExpressionBuilder
+  override protected def astBuilder: SnowflakeExpressionBuilder = new SnowflakeExpressionBuilder
 
   "SnowflakeExpressionBuilder" should {
     "translate literals" in {
       example("null", _.literal(), Literal(nullType = Some(NullType())))
       example("true", _.literal(), Literal(boolean = Some(true)))
       example("false", _.literal(), Literal(boolean = Some(false)))
       example("1", _.literal(), Literal(integer = Some(1)))
@@ -150,120 +157,14 @@
     }
 
     // see https://github.com/databrickslabs/remorph/issues/273
     "translate NOT EXISTS expressions" ignore {
       example("NOT EXISTS (SELECT * FROM t)", _.expr(), Not(Exists(Project(namedTable("t"), Seq(Star(None))))))
     }
 
-    "translate IN expressions" in {
-      example("col1 IN (SELECT * FROM t)", _.predicate, IsIn(Project(namedTable("t"), Seq(Star(None))), Column("col1")))
-      example(
-        "col1 NOT IN (SELECT * FROM t)",
-        _.predicate,
-        Not(IsIn(Project(namedTable("t"), Seq(Star(None))), Column("col1"))))
-    }
-
-    "translate BETWEEN expressions" in {
-      example(
-        "col1 BETWEEN 3.14 AND 42",
-        _.predicate,
-        And(
-          GreaterThanOrEqual(Column("col1"), Literal(float = Some(3.14f))),
-          LesserThanOrEqual(Column("col1"), Literal(integer = Some(42)))))
-      example(
-        "col1 NOT BETWEEN 3.14 AND 42",
-        _.predicate,
-        Not(
-          And(
-            GreaterThanOrEqual(Column("col1"), Literal(float = Some(3.14f))),
-            LesserThanOrEqual(Column("col1"), Literal(integer = Some(42))))))
-    }
-
-    "translate LIKE expressions" in {
-      example(
-        "col1 LIKE '%foo'",
-        _.predicate,
-        Like(Column("col1"), Seq(Literal(string = Some("%foo"))), None, caseSensitive = true))
-      example(
-        "col1 ILIKE '%foo'",
-        _.predicate,
-        Like(Column("col1"), Seq(Literal(string = Some("%foo"))), None, caseSensitive = false))
-      example(
-        "col1 NOT LIKE '%foo'",
-        _.predicate,
-        Not(Like(Column("col1"), Seq(Literal(string = Some("%foo"))), None, caseSensitive = true)))
-      example(
-        "col1 NOT ILIKE '%foo'",
-        _.predicate,
-        Not(Like(Column("col1"), Seq(Literal(string = Some("%foo"))), None, caseSensitive = false)))
-      example(
-        "col1 LIKE '%foo' ESCAPE '^'",
-        _.predicate,
-        Like(
-          Column("col1"),
-          Seq(Literal(string = Some("%foo"))),
-          Some(Literal(string = Some("^"))),
-          caseSensitive = true))
-      example(
-        "col1 ILIKE '%foo' ESCAPE '^'",
-        _.predicate,
-        Like(
-          Column("col1"),
-          Seq(Literal(string = Some("%foo"))),
-          Some(Literal(string = Some("^"))),
-          caseSensitive = false))
-
-      example(
-        "col1 NOT LIKE '%foo' ESCAPE '^'",
-        _.predicate,
-        Not(
-          Like(
-            Column("col1"),
-            Seq(Literal(string = Some("%foo"))),
-            Some(Literal(string = Some("^"))),
-            caseSensitive = true)))
-      example(
-        "col1 NOT ILIKE '%foo' ESCAPE '^'",
-        _.predicate,
-        Not(
-          Like(
-            Column("col1"),
-            Seq(Literal(string = Some("%foo"))),
-            Some(Literal(string = Some("^"))),
-            caseSensitive = false)))
-
-      example(
-        "col1 LIKE ANY ('%foo', 'bar%', '%qux%')",
-        _.predicate,
-        Like(
-          Column("col1"),
-          Seq(Literal(string = Some("%foo")), Literal(string = Some("bar%")), Literal(string = Some("%qux%"))),
-          None,
-          caseSensitive = true))
-
-      example(
-        "col1 LIKE ANY ('%foo', 'bar%', '%qux%') ESCAPE '^'",
-        _.predicate,
-        Like(
-          Column("col1"),
-          Seq(Literal(string = Some("%foo")), Literal(string = Some("bar%")), Literal(string = Some("%qux%"))),
-          Some(Literal(string = Some("^"))),
-          caseSensitive = true))
-
-      example("col1 RLIKE '[a-z][A-Z]*'", _.predicate, RLike(Column("col1"), Literal(string = Some("[a-z][A-Z]*"))))
-      example(
-        "col1 NOT RLIKE '[a-z][A-Z]*'",
-        _.predicate,
-        Not(RLike(Column("col1"), Literal(string = Some("[a-z][A-Z]*")))))
-    }
-
-    "translate IS [NOT] NULL expressions" in {
-      example("col1 IS NULL", _.predicate, IsNull(Column("col1")))
-      example("col1 IS NOT NULL", _.predicate, Not(IsNull(Column("col1"))))
-    }
   }
 
   "translate CASE expressions" in {
     example(
       "CASE WHEN col1 = 1 THEN 'one' WHEN col2 = 2 THEN 'two' END",
       _.case_expression(),
       Case(
@@ -306,8 +207,54 @@
   }
 
   "Unparsed input" should {
     "be reported as UnresolvedExpression" in {
       example("{'name':'Homer Simpson'}", _.json_literal(), UnresolvedExpression("{'name':'Homer Simpson'}"))
     }
   }
+
+  "SnowflakeExpressionBuilder.visit_Literal" should {
+    "handle unresolved input" in {
+      val literal = mock[LiteralContext]
+      astBuilder.visitLiteral(literal) shouldBe Literal(nullType = Some(NullType()))
+      verify(literal).sign()
+      verify(literal).STRING()
+      verify(literal).DECIMAL()
+      verify(literal).FLOAT()
+      verify(literal).REAL()
+      verify(literal).true_false()
+      verify(literal).NULL_()
+      verifyNoMoreInteractions(literal)
+    }
+  }
+
+  "SnowflakeExpressionBuilder.buildComparisonExpression" should {
+    "handle unresolved input" in {
+      val operator = mock[Comparison_operatorContext]
+      val dummyTextForOperator = "dummy"
+      when(operator.getText).thenReturn(dummyTextForOperator)
+      astBuilder.buildComparisonExpression(operator, null, null) shouldBe UnresolvedExpression(dummyTextForOperator)
+      verify(operator).EQ()
+      verify(operator).NE()
+      verify(operator).LTGT()
+      verify(operator).GT()
+      verify(operator).LT()
+      verify(operator).GE()
+      verify(operator).LE()
+      verify(operator).getText
+      verifyNoMoreInteractions(operator)
+    }
+  }
+
+  "SnowflakeExpressionBuilder.buildWindowFunction" should {
+    "handle unresolved input" in {
+      val windowedFunction = mock[Ranking_windowed_functionContext]
+      val dummyTextForWindowedFunction = "dummy"
+      when(windowedFunction.getText).thenReturn(dummyTextForWindowedFunction)
+      astBuilder.buildWindowFunction(windowedFunction) shouldBe UnresolvedExpression(dummyTextForWindowedFunction)
+      verify(windowedFunction).ROW_NUMBER()
+      verify(windowedFunction).NTILE()
+      verify(windowedFunction).getText
+      verifyNoMoreInteractions(windowedFunction)
+    }
+  }
 }
```

### Comparing `databricks_labs_remorph-0.1.7/core/src/test/scala/com/databricks/labs/remorph/parsers/snowflake/SnowflakeParserTestCommon.scala` & `databricks_labs_remorph-0.2.0/core/src/test/scala/com/databricks/labs/remorph/parsers/snowflake/SnowflakeParserTestCommon.scala`

 * *Files identical despite different names*

### Comparing `databricks_labs_remorph-0.1.7/databricks/labs/remorph/cli.py` & `databricks_labs_remorph-0.2.0/databricks/labs/remorph/cli.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,17 +1,19 @@
 import json
 import os
 
+from pyspark.sql import SparkSession
+
+from databricks.connect import DatabricksSession
 from databricks.labs.blueprint.cli import App
 from databricks.labs.blueprint.entrypoint import get_logger
 from databricks.labs.blueprint.installation import Installation
 from databricks.labs.remorph.config import SQLGLOT_DIALECTS, MorphConfig
 from databricks.labs.remorph.helpers.recon_config_utils import ReconConfigPrompts
 from databricks.labs.remorph.lineage import lineage_generator
-from databricks.labs.remorph.reconcile.execute import recon
 from databricks.labs.remorph.transpiler.execute import morph
 from databricks.sdk import WorkspaceClient
 
 remorph = App(__file__)
 logger = get_logger(__file__)
 
 DIALECTS = {name for name, dialect in SQLGLOT_DIALECTS.items()}
@@ -22,15 +24,15 @@
 
 
 @remorph.command
 def transpile(
     w: WorkspaceClient,
     source: str,
     input_sql: str,
-    output_folder: str,
+    output_folder: str | None,
     skip_validation: str,
     catalog_name: str,
     schema_name: str,
     mode: str,
 ):
     """transpiles source dialect to databricks dialect"""
     logger.info(f"user: {w.current_user.me()}")
@@ -38,15 +40,15 @@
     default_config = installation.load(MorphConfig)
     mode = mode if mode else "current"  # not checking for default config as it will always be current
 
     if source.lower() not in SQLGLOT_DIALECTS:
         raise_validation_exception(f"Error: Invalid value for '--source': '{source}' is not one of {DIALECTS}. ")
     if not os.path.exists(input_sql) or input_sql in {None, ""}:
         raise_validation_exception(f"Error: Invalid value for '--input_sql': Path '{input_sql}' does not exist.")
-    if output_folder == "":
+    if not output_folder:
         output_folder = default_config.output_folder if default_config.output_folder else None
     if skip_validation.lower() not in {"true", "false"}:
         raise_validation_exception(
             f"Error: Invalid value for '--skip_validation': '{skip_validation}' is not one of 'true', 'false'. "
         )
     if mode.lower() not in {"current", "experimental"}:
         raise_validation_exception(
@@ -70,34 +72,37 @@
 
     status = morph(w, config)
 
     print(json.dumps(status))
 
 
 @remorph.command
-def reconcile(w: WorkspaceClient, recon_conf: str, conn_profile: str, source: str, report: str):
-    """reconciles source to databricks datasets"""
+def reconcile(w: WorkspaceClient, source: str, report: str):
+    """[EXPERIMENTAL] reconciles source to databricks datasets"""
     logger.info(f"user: {w.current_user.me()}")
-    if not os.path.exists(recon_conf) or recon_conf in {None, ""}:
-        raise_validation_exception(f"Error: Invalid value for '--recon_conf': Path '{recon_conf}' does not exist.")
-    if not os.path.exists(conn_profile) or conn_profile in {None, ""}:
-        raise_validation_exception(f"Error: Invalid value for '--conn_profile': Path '{conn_profile}' does not exist.")
-    if source.lower() not in "snowflake":
-        raise_validation_exception(f"Error: Invalid value for '--source': '{source}' is not one of 'snowflake'. ")
-    if report.lower() not in {"data", "schema", "all"}:
+
+    if source.lower() not in {"databricks", "snowflake", "oracle"}:
+        raise_validation_exception(
+            f"Error: Invalid value for '--source': '{source}' is not one of 'databricks', 'snowflake', 'oracle'. "
+        )
+    if report.lower() not in {"data", "schema", "all", "row"}:
         raise_validation_exception(
-            f"Error: Invalid value for '--report': '{report}' is not one of 'data', 'schema', 'all' "
+            f"Error: Invalid value for '--report': '{report}' is not one of 'data', 'schema', 'all' , 'row'"
         )
 
-    recon(recon_conf, conn_profile, source, report)
+    raise NotImplementedError
+
+
+def _get_spark_session(ws: WorkspaceClient) -> SparkSession:
+    return DatabricksSession.builder.sdkConfig(ws.config).getOrCreate()
 
 
 @remorph.command
 def generate_lineage(w: WorkspaceClient, source: str, input_sql: str, output_folder: str):
-    """Generates a lineage of source SQL files or folder"""
+    """[Experimental] Generates a lineage of source SQL files or folder"""
     logger.info(f"User: {w.current_user.me()}")
     if source.lower() not in SQLGLOT_DIALECTS:
         raise_validation_exception(f"Error: Invalid value for '--source': '{source}' is not one of {DIALECTS}. ")
     if not os.path.exists(input_sql) or input_sql in {None, ""}:
         raise_validation_exception(f"Error: Invalid value for '--input_sql': Path '{input_sql}' does not exist.")
     if not os.path.exists(output_folder) or output_folder in {None, ""}:
         raise_validation_exception(
```

### Comparing `databricks_labs_remorph-0.1.7/databricks/labs/remorph/config.py` & `databricks_labs_remorph-0.2.0/databricks/labs/remorph/config.py`

 * *Files 11% similar despite different names*

```diff
@@ -1,18 +1,19 @@
 import logging
 from dataclasses import dataclass
 
-from sqlglot.dialects.dialect import Dialect, Dialects
+from sqlglot.dialects.dialect import Dialect, Dialects, DialectType
 
+from databricks.labs.remorph.helpers.morph_status import ParserError
 from databricks.labs.remorph.reconcile.recon_config import Table
 from databricks.labs.remorph.snow import databricks, experimental, oracle, snowflake
 
 logger = logging.getLogger(__name__)
 
-SQLGLOT_DIALECTS = {
+SQLGLOT_DIALECTS: dict[str, DialectType] = {
     "bigquery": Dialects.BIGQUERY,
     "databricks": databricks.Databricks,
     "experimental": experimental.DatabricksExperimental,
     "drill": Dialects.DRILL,
     "mssql": Dialects.TSQL,
     "netezza": Dialects.POSTGRES,
     "oracle": oracle.Oracle,
@@ -23,18 +24,22 @@
     "sqlite": Dialects.SQLITE,
     "teradata": Dialects.TERADATA,
     "trino": Dialects.TRINO,
     "vertica": Dialects.POSTGRES,
 }
 
 
-def _get_dialect(engine: str) -> Dialect:
+def get_dialect(engine: str) -> Dialect:
     return Dialect.get_or_raise(SQLGLOT_DIALECTS.get(engine))
 
 
+def get_key_form_dialect(input_dialect: Dialect) -> str:
+    return [source_key for source_key, dialect in SQLGLOT_DIALECTS.items() if dialect == input_dialect][0]
+
+
 @dataclass
 class MorphConfig:
     __file__ = "config.yml"
     __version__ = 1
 
     source: str
     sdk_config: dict[str, str] | None = None
@@ -42,33 +47,51 @@
     output_folder: str | None = None
     skip_validation: bool = False
     catalog_name: str = "transpiler_test"
     schema_name: str = "convertor_test"
     mode: str = "current"
 
     def get_read_dialect(self):
-        return _get_dialect(self.source)
+        return get_dialect(self.source)
 
     def get_write_dialect(self):
         if self.mode == "experimental":
-            return _get_dialect("experimental")
-        return _get_dialect("databricks")
+            return get_dialect("experimental")
+        return get_dialect("databricks")
 
 
 @dataclass
 class TableRecon:
     __file__ = "recon_config.yml"
     __version__ = 1
 
     source_schema: str
     target_catalog: str
     target_schema: str
     tables: list[Table]
     source_catalog: str | None = None
 
+    def __post_init__(self):
+        self.source_schema = self.source_schema.lower()
+        self.target_schema = self.target_schema.lower()
+        self.target_catalog = self.target_catalog.lower()
+        self.source_catalog = self.source_catalog.lower() if self.source_catalog else self.source_catalog
+
 
 @dataclass
 class DatabaseConfig:
     source_schema: str
     target_catalog: str
     target_schema: str
     source_catalog: str | None = None
+
+
+@dataclass
+class TranspilationResult:
+    transpiled_sql: list[str]
+    parse_error_list: list[ParserError]
+
+
+@dataclass
+class ValidationResult:
+    validated_sql: str
+    exception_msg: str | None
```

### Comparing `databricks_labs_remorph-0.1.7/databricks/labs/remorph/install.py` & `databricks_labs_remorph-0.2.0/databricks/labs/remorph/install.py`

 * *Files 2% similar despite different names*

```diff
@@ -57,15 +57,15 @@
         logger.info("Please answer a couple of questions to configure Remorph")
 
         # default params
         catalog_name = "transpiler_test"
         schema_name = "convertor_test"
         ws_config = None
 
-        source_prompt = self._prompts.choice("Select the source", SQLGLOT_DIALECTS.keys())
+        source_prompt = self._prompts.choice("Select the source", list(SQLGLOT_DIALECTS.keys()))
         source = source_prompt.lower()
 
         skip_validation = self._prompts.confirm("Do you want to Skip Validation")
 
         if not skip_validation:
             ws_config = self._configure_runtime()
             catalog_name = self._prompts.question("Enter catalog_name")
@@ -86,15 +86,16 @@
             skip_validation=skip_validation,
             catalog_name=catalog_name,
             schema_name=schema_name,
             sdk_config=ws_config,
             mode="current",  # mode will not have a prompt as this is hidden flag
         )
 
-        ws_file_url = self._installation.save(config)
+        self._installation.save(config)
+        ws_file_url = self._installation.workspace_link(config.__file__)
         if self._prompts.confirm("Open config file in the browser and continue installing?"):
             webbrowser.open(ws_file_url)
         return config
 
     def _configure_runtime(self) -> dict[str, str]:
         if self._prompts.confirm("Do you want to use SQL Warehouse for validation?"):
             warehouse_id = self._configure_warehouse()
```

### Comparing `databricks_labs_remorph-0.1.7/databricks/labs/remorph/lineage.py` & `databricks_labs_remorph-0.2.0/databricks/labs/remorph/lineage.py`

 * *Files 2% similar despite different names*

```diff
@@ -9,28 +9,28 @@
 
 
 def _generate_dot_file_contents(dag: DAG) -> str:
     _lineage_str = "flowchart TD\n"
     for node_name, node in dag.nodes.items():
         if node.parents:
             for parent in node.parents:
-                _lineage_str += f"    {node_name.capitalize()} --> {parent.name.capitalize()}\n"
+                _lineage_str += f"    {node_name.capitalize()} --> {parent.capitalize()}\n"
         else:
             # Include nodes without parents to ensure they appear in the diagram
             _lineage_str += f"    {node_name.capitalize()}\n"
     return _lineage_str
 
 
 def lineage_generator(source: str, input_sql: str, output_folder: str):
-    input_sql = Path(input_sql)
+    input_sql_path = Path(input_sql)
     output_folder = output_folder if output_folder.endswith('/') else output_folder + '/'
 
-    msg = f"Processing for SQLs at this location: {input_sql}"
+    msg = f"Processing for SQLs at this location: {input_sql_path}"
     logger.info(msg)
-    root_table_identifier = RootTableIdentifier(source, input_sql)
+    root_table_identifier = RootTableIdentifier(source, input_sql_path)
     generated_dag = root_table_identifier.generate_lineage()
     lineage_file_content = _generate_dot_file_contents(generated_dag)
 
     date_str = datetime.datetime.now().strftime("%d%m%y")
 
     output_filename = Path(f"{output_folder}lineage_{date_str}.dot")
     if output_filename.exists():
```

### Comparing `databricks_labs_remorph-0.1.7/databricks/labs/remorph/uninstall.py` & `databricks_labs_remorph-0.2.0/databricks/labs/remorph/uninstall.py`

 * *Files identical despite different names*

### Comparing `databricks_labs_remorph-0.1.7/databricks/labs/remorph/coverage/commons.py` & `databricks_labs_remorph-0.2.0/databricks/labs/remorph/coverage/commons.py`

 * *Files 2% similar despite different names*

```diff
@@ -2,20 +2,20 @@
 import dataclasses
 import json
 import logging
 import os
 import subprocess
 import time
 from collections.abc import Generator
-from datetime import datetime
+from datetime import datetime, timezone
 from pathlib import Path
 from typing import TextIO
 
 import sqlglot
-from sqlglot import Expression
+from sqlglot.expressions import Expression
 from sqlglot.dialects.dialect import Dialect
 from sqlglot.errors import ErrorLevel
 
 logger = logging.getLogger(__name__)
 
 
 @dataclasses.dataclass
@@ -40,15 +40,15 @@
 
 
 def write_json_line(file: TextIO, content: ReportEntry):
     json.dump(dataclasses.asdict(content), file)
     file.write("\n")
 
 
-def get_env_var(env_var: str, *, required: bool = False) -> str:
+def get_env_var(env_var: str, *, required: bool = False) -> str | None:
     """
     Get the value of an environment variable.
 
     :param env_var: The name of the environment variable to get the value of.
     :param required: Indicates if the environment variable is required and raises a ValueError if it's not set.
     :return: Returns the environment variable's value, or None if it's not set and not required.
     """
@@ -71,15 +71,15 @@
         )
     except (subprocess.CalledProcessError, FileNotFoundError) as e:
         logger.warning(f"Could not get the current commit hash. {e!s}")
         return None
 
 
 def get_current_time_utc() -> datetime:
-    return datetime.utcnow()
+    return datetime.now(timezone.utc)
 
 
 def parse_sql(sql: str, dialect: type[Dialect]) -> list[Expression]:
     return [expression for expression in sqlglot.parse(sql, read=dialect, error_level=ErrorLevel.RAISE) if expression]
 
 
 def generate_sql(expressions: list[Expression], dialect: type[Dialect]) -> list[str]:
```

### Comparing `databricks_labs_remorph-0.1.7/databricks/labs/remorph/coverage/remorph_snow_transpilation_coverage.py` & `databricks_labs_remorph-0.2.0/databricks/labs/remorph/coverage/remorph_snow_transpilation_coverage.py`

 * *Files 25% similar despite different names*

```diff
@@ -9,14 +9,19 @@
     input_dir = commons.get_env_var("INPUT_DIR", required=True)
     output_dir = commons.get_env_var("OUTPUT_DIR", required=True)
 
     REMORPH_COMMIT_HASH = commons.get_current_commit_hash() or ""  # C0103 pylint
     product_info = ProductInfo(__file__)
     remorph_version = product_info.unreleased_version()
 
+    if not input_dir:
+        raise ValueError("Environment variable `INPUT_DIR` is required")
+    if not output_dir:
+        raise ValueError("Environment variable `OUTPUT_DIR` is required")
+
     commons.collect_transpilation_stats(
         "Remorph",
         REMORPH_COMMIT_HASH,
         remorph_version,
         Snow,
         Databricks,
         Path(input_dir),
```

### Comparing `databricks_labs_remorph-0.1.7/databricks/labs/remorph/coverage/sqlglot_snow_transpilation_coverage.py` & `databricks_labs_remorph-0.2.0/databricks/labs/remorph/coverage/sqlglot_snow_transpilation_coverage.py`

 * *Files 12% similar despite different names*

```diff
@@ -8,14 +8,19 @@
 
 if __name__ == "__main__":
     input_dir = commons.get_env_var("INPUT_DIR", required=True)
     output_dir = commons.get_env_var("OUTPUT_DIR", required=True)
     sqlglot_version = sqlglot.__version__
     SQLGLOT_COMMIT_HASH = ""  # C0103 pylint
 
+    if not input_dir:
+        raise ValueError("Environment variable `INPUT_DIR` is required")
+    if not output_dir:
+        raise ValueError("Environment variable `OUTPUT_DIR` is required")
+
     commons.collect_transpilation_stats(
         "SQLGlot",
         SQLGLOT_COMMIT_HASH,
         sqlglot_version,
         Snowflake,
         Databricks,
         Path(input_dir),
```

### Comparing `databricks_labs_remorph-0.1.7/databricks/labs/remorph/helpers/db_sql.py` & `databricks_labs_remorph-0.2.0/databricks/labs/remorph/helpers/db_sql.py`

 * *Files 4% similar despite different names*

```diff
@@ -17,15 +17,15 @@
 def get_sql_backend(ws: WorkspaceClient, config: MorphConfig) -> SqlBackend:
     sdk_config = config.sdk_config
     warehouse_id = sdk_config.get("warehouse_id", None) if sdk_config else None
     cluster_id = sdk_config.get("cluster_id", None) if sdk_config else None
     catalog_name = config.catalog_name
     schema_name = config.schema_name
     if warehouse_id:
-        sql_backend = StatementExecutionBackend(ws, warehouse_id, catalog=catalog_name, schema=schema_name)
+        sql_backend: SqlBackend = StatementExecutionBackend(ws, warehouse_id, catalog=catalog_name, schema=schema_name)
     else:
         # assigning cluster id explicitly to the config as user can provide them during installation
         ws.config.cluster_id = cluster_id if cluster_id else ws.config.cluster_id
         sql_backend = RuntimeBackend() if "DATABRICKS_RUNTIME_VERSION" in os.environ else DatabricksConnectBackend(ws)
         try:
             sql_backend.execute(f"use catalog {catalog_name}")
             sql_backend.execute(f"use {schema_name}")
```

### Comparing `databricks_labs_remorph-0.1.7/databricks/labs/remorph/helpers/execution_time.py` & `databricks_labs_remorph-0.2.0/databricks/labs/remorph/helpers/execution_time.py`

 * *Files identical despite different names*

### Comparing `databricks_labs_remorph-0.1.7/databricks/labs/remorph/helpers/file_utils.py` & `databricks_labs_remorph-0.2.0/databricks/labs/remorph/helpers/file_utils.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,9 +1,10 @@
 import codecs
 from pathlib import Path
+from collections.abc import Generator
 
 
 # Optionally check to see if a string begins with a Byte Order Mark
 # such a character will cause the transpiler to fail
 def remove_bom(input_string: str) -> str:
     """
     Removes the Byte Order Mark (BOM) from the given string if it exists.
@@ -63,17 +64,17 @@
     files = [f for f in root.iterdir() if f.is_file()]
     yield root, sub_dirs, files
 
     for each_dir in sub_dirs:
         yield from dir_walk(each_dir)
 
 
-def get_sql_file(input_path: str | Path) -> list:
+def get_sql_file(input_path: str | Path) -> Generator[Path, None, None]:
     """
-    Generator that yields the names of all SQL files in the given directory tree.
+    Returns Generator that yields the names of all SQL files in the given directory.
     :param input_path: Path
     :return: List of SQL files
     """
     for _, _, files in dir_walk(Path(input_path)):
         for filename in files:
             if is_sql_file(filename):
                 yield filename
```

### Comparing `databricks_labs_remorph-0.1.7/databricks/labs/remorph/helpers/recon_config_utils.py` & `databricks_labs_remorph-0.2.0/databricks/labs/remorph/helpers/recon_config_utils.py`

 * *Files identical despite different names*

### Comparing `databricks_labs_remorph-0.1.7/databricks/labs/remorph/helpers/validation.py` & `databricks_labs_remorph-0.2.0/databricks/labs/remorph/helpers/validation.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,26 +1,26 @@
 import logging
 from io import StringIO
 
 from databricks.labs.lsql.backends import SqlBackend
-from databricks.labs.remorph.config import MorphConfig
+from databricks.labs.remorph.config import MorphConfig, ValidationResult
 from databricks.sdk.errors.base import DatabricksError
 
 logger = logging.getLogger(__name__)
 
 
 class Validator:
     """
     The Validator class is used to validate SQL queries.
     """
 
     def __init__(self, sql_backend: SqlBackend):
         self._sql_backend = sql_backend
 
-    def validate_format_result(self, config: MorphConfig, input_sql: str) -> tuple[str, str | None]:
+    def validate_format_result(self, config: MorphConfig, input_sql: str) -> ValidationResult:
         """
         Validates the SQL query and formats the result.
 
         This function validates the SQL query based on the provided configuration. If the query is valid,
         it appends a semicolon to the end of the query. If the query is not valid, it formats the error message.
 
         Parameters:
@@ -34,27 +34,27 @@
         (is_valid, exception_type, exception_msg) = self._query(self._sql_backend, input_sql)
         if is_valid:
             result = input_sql + "\n;\n"
             if exception_type is not None:
                 exception_msg = f"[{exception_type.upper()}]: {exception_msg}"
         else:
             query = ""
-            if "[UNRESOLVED_ROUTINE]" in exception_msg:
+            if "[UNRESOLVED_ROUTINE]" in str(exception_msg):
                 query = input_sql
             buffer = StringIO()
             buffer.write("-------------- Exception Start-------------------\n")
             buffer.write("/* \n")
-            buffer.write(exception_msg)
+            buffer.write(str(exception_msg))
             buffer.write("\n */ \n")
             buffer.write(query)
             buffer.write("\n ---------------Exception End --------------------\n")
 
             result = buffer.getvalue()
 
-        return result, exception_msg
+        return ValidationResult(result, exception_msg)
 
     def _query(self, sql_backend: SqlBackend, query: str) -> tuple[bool, str | None, str | None]:
         """
         Validate a given SQL query using the provided SQL backend
 
         Parameters:
         - query (str): The SQL query to be validated.
@@ -67,16 +67,16 @@
         # When variables is mentioned Explain fails we need way to replace them before explain is executed.
         explain_query = f'EXPLAIN {query.replace("${", "`{").replace("}", "}`").replace("``", "`")}'
         try:
             rows = list(sql_backend.fetch(explain_query))
             if not rows:
                 return False, "error", "No results returned from explain query."
 
-            if "Error occurred during query planning" in rows[0].as_dict().get("plan", ""):
-                error_details = rows[1].as_dict().get("plan", "Unknown error.") if len(rows) > 1 else "Unknown error."
+            if "Error occurred during query planning" in rows[0].asDict().get("plan", ""):
+                error_details = rows[1].asDict().get("plan", "Unknown error.") if len(rows) > 1 else "Unknown error."
                 raise DatabricksError(error_details)
             return True, None, None
         except DatabricksError as dbe:
             err_msg = str(dbe)
             if "[PARSE_SYNTAX_ERROR]" in err_msg:
                 logger.debug(f"Syntax Exception : NOT IGNORED. Flag as syntax error: {err_msg}")
                 return False, "error", err_msg
```

### Comparing `databricks_labs_remorph-0.1.7/databricks/labs/remorph/intermediate/dag.py` & `databricks_labs_remorph-0.2.0/databricks/labs/remorph/intermediate/dag.py`

 * *Files 14% similar despite different names*

```diff
@@ -2,87 +2,87 @@
 
 logger = logging.getLogger(__name__)
 
 
 class Node:
     def __init__(self, name: str):
         self.name = name.lower()
-        self.children = []
-        self.parents = []
+        self.children: list[str] = []
+        self.parents: list[str] = []
 
-    def add_parent(self, node: str):
+    def add_parent(self, node: str) -> None:
         self.parents.append(node)
 
-    def add_child(self, node: str):
+    def add_child(self, node: str) -> None:
         self.children.append(node)
 
-    def __repr__(self):
+    def __repr__(self) -> str:
         return f"Node({self.name}, {self.children})"
 
 
 class DAG:
     def __init__(self):
-        self.nodes = {}
+        self.nodes: dict[str, Node] = {}
 
-    def add_node(self, node_name: str):
+    def add_node(self, node_name: str) -> None:
         if node_name not in self.nodes and node_name not in {None, "none"}:
             self.nodes[node_name.lower()] = Node(node_name.lower())
 
-    def add_edge(self, parent_name: str, child_name: str):
+    def add_edge(self, parent_name: str, child_name: str) -> None:
         parent_name = parent_name.lower() if parent_name is not None else None
         child_name = child_name.lower() if child_name is not None else None
         logger.debug(f"Adding edge: {parent_name} -> {child_name}")
         if parent_name not in self.nodes:
             self.add_node(parent_name)
         if child_name not in self.nodes:
             self.add_node(child_name)
 
         if child_name is not None:
-            self.nodes[parent_name].add_child(self.nodes[child_name])
-            self.nodes[child_name].add_parent(self.nodes[parent_name])
+            self.nodes[parent_name].add_child(child_name)
+            self.nodes[child_name].add_parent(parent_name)
 
-    def identify_immediate_parents(self, table_name: str):
+    def identify_immediate_parents(self, table_name: str) -> list[str]:
         table_name = table_name.lower()  # convert to lower() case
         if table_name not in self.nodes:
             logger.debug(f"Table with the name {table_name} not found in the DAG")
             return []
 
-        return [parent.name for parent in self.nodes[table_name].parents]
+        return list(self.nodes[table_name].parents)
 
-    def identify_immediate_children(self, table_name: str):
+    def identify_immediate_children(self, table_name: str) -> list[str]:
         table_name = table_name.lower()  # convert to lower() case
         if table_name not in self.nodes:
             logger.debug(f"Table with the name {table_name} not found in the DAG")
             return []
 
-        return [child.name for child in self.nodes[table_name].children]
+        return list(self.nodes[table_name].children)
 
     def _is_root_node(self, node_name: str) -> bool:
         return len(self.identify_immediate_parents(node_name)) == 0
 
-    def walk_bfs(self, node: str, level: int) -> set:
+    def walk_bfs(self, node: Node, level: int) -> set:
         tables_at_level = set()
         queue = [(node, 0)]  # The queue for the BFS. Each element is a tuple (node, level).
         while queue:
             current_node, node_level = queue.pop(0)
 
             if node_level == level:
                 tables_at_level.add(current_node.name)
             elif node_level > level:
                 break
 
             for child_name in self.identify_immediate_children(current_node.name):
                 queue.append((self.nodes[child_name], node_level + 1))
         return tables_at_level
 
-    def identify_root_tables(self, level: int):
+    def identify_root_tables(self, level: int) -> set:
         all_nodes = set(self.nodes.values())
         root_tables_at_level = set()
 
         for node in all_nodes:
             if self._is_root_node(node.name):
                 root_tables_at_level.update(self.walk_bfs(node, level))
 
         return root_tables_at_level
 
-    def __repr__(self):
+    def __repr__(self) -> str:
         return str({node_name: str(node) for node_name, node in self.nodes.items()})
```

### Comparing `databricks_labs_remorph-0.1.7/databricks/labs/remorph/intermediate/engine_adapter.py` & `databricks_labs_remorph-0.2.0/databricks/labs/remorph/intermediate/engine_adapter.py`

 * *Files identical despite different names*

### Comparing `databricks_labs_remorph-0.1.7/databricks/labs/remorph/intermediate/root_tables.py` & `databricks_labs_remorph-0.2.0/databricks/labs/remorph/intermediate/root_tables.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 import logging
 from pathlib import Path
 
-from databricks.labs.remorph.config import SQLGLOT_DIALECTS
+from databricks.labs.remorph.config import get_dialect
 from databricks.labs.remorph.helpers.file_utils import (
     get_sql_file,
     is_sql_file,
     read_file,
 )
 from databricks.labs.remorph.intermediate.dag import DAG
 from databricks.labs.remorph.intermediate.engine_adapter import EngineAdapter
@@ -13,15 +13,15 @@
 logger = logging.getLogger(__name__)
 
 
 class RootTableIdentifier:
     def __init__(self, source: str, input_path: str | Path):
         self.source = source
         self.input_path = input_path
-        self.engine_adapter = EngineAdapter(SQLGLOT_DIALECTS.get(source))
+        self.engine_adapter = EngineAdapter(get_dialect(source))
 
     def generate_lineage(self, engine="sqlglot") -> DAG:
         dag = DAG()
 
         # when input is sql file then parse the file
         if is_sql_file(self.input_path):
             filename = self.input_path
```

### Comparing `databricks_labs_remorph-0.1.7/databricks/labs/remorph/reconcile/compare.py` & `databricks_labs_remorph-0.2.0/databricks/labs/remorph/reconcile/compare.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,79 +1,94 @@
 from pyspark.sql import DataFrame
 from pyspark.sql.functions import col, expr, lit
 
-from databricks.labs.remorph.reconcile.constants import Constants
 from databricks.labs.remorph.reconcile.exception import ColumnMismatchException
-from databricks.labs.remorph.reconcile.recon_config import ReconcileOutput
+from databricks.labs.remorph.reconcile.recon_config import (
+    DataReconcileOutput,
+    MismatchOutput,
+)
+
+_HASH_COLUMN_NAME = "hash_value_recon"
 
 
 def raise_column_mismatch_exception(msg: str, source_missing: list[str], target_missing: list[str]) -> Exception:
     error_msg = (
         f"{msg}\n"
         f"columns missing in source: {','.join(source_missing) if source_missing else None}\n"
         f"columns missing in target: {','.join(target_missing) if target_missing else None}\n"
     )
     return ColumnMismatchException(error_msg)
 
 
-def reconcile_data(source: DataFrame, target: DataFrame, key_columns: list[str], report_type: str) -> ReconcileOutput:
+def reconcile_data(
+    source: DataFrame, target: DataFrame, key_columns: list[str], report_type: str
+) -> DataReconcileOutput:
     source_alias = "src"
     target_alias = "tgt"
     if report_type not in {"data", "all"}:
-        key_columns = Constants.hash_column_name
+        key_columns = [_HASH_COLUMN_NAME]
     df = source.alias(source_alias).join(other=target.alias(target_alias), on=key_columns, how="full")
 
     mismatch = (
         _get_mismatch_data(df, source_alias, target_alias, source.columns) if report_type in {"all", "data"} else None
     )
     missing_in_src = (
-        df.filter(col(f"{source_alias}.{Constants.hash_column_name}").isNull())
+        df.filter(col(f"{source_alias}.{_HASH_COLUMN_NAME}").isNull())
         .select((key_columns if report_type == "all" else alias_column_str(target_alias, target.columns)))
-        .drop(Constants.hash_column_name)
+        .drop(_HASH_COLUMN_NAME)
     )
     missing_in_tgt = (
-        df.filter(col(f"{target_alias}.{Constants.hash_column_name}").isNull())
+        df.filter(col(f"{target_alias}.{_HASH_COLUMN_NAME}").isNull())
         .select((key_columns if report_type == "all" else alias_column_str(source_alias, source.columns)))
-        .drop(Constants.hash_column_name)
+        .drop(_HASH_COLUMN_NAME)
+    )
+    mismatch_count = 0
+    if mismatch:
+        mismatch_count = mismatch.count()
+
+    return DataReconcileOutput(
+        mismatch_count=mismatch_count,
+        missing_in_src_count=missing_in_src.count(),
+        missing_in_tgt_count=missing_in_tgt.count(),
+        missing_in_src=missing_in_src,
+        missing_in_tgt=missing_in_tgt,
+        mismatch=MismatchOutput(mismatch_df=mismatch),
     )
-    return ReconcileOutput(missing_in_src=missing_in_src, missing_in_tgt=missing_in_tgt, mismatch=mismatch)
 
 
 def _get_mismatch_data(df: DataFrame, src_alias: str, tgt_alias: str, select_columns) -> DataFrame:
     return (
         df.filter(
-            (col(f"{src_alias}.{Constants.hash_column_name}").isNotNull())
-            & (col(f"{tgt_alias}.{Constants.hash_column_name}").isNotNull())
+            (col(f"{src_alias}.{_HASH_COLUMN_NAME}").isNotNull())
+            & (col(f"{tgt_alias}.{_HASH_COLUMN_NAME}").isNotNull())
         )
         .withColumn(
             "hash_match",
-            col(f"{src_alias}.{Constants.hash_column_name}") == col(f"{tgt_alias}.{Constants.hash_column_name}"),
+            col(f"{src_alias}.{_HASH_COLUMN_NAME}") == col(f"{tgt_alias}.{_HASH_COLUMN_NAME}"),
         )
         .filter(col("hash_match") == lit(False))
         .select(alias_column_str(src_alias, select_columns))
-        .drop(Constants.hash_column_name)
+        .drop(_HASH_COLUMN_NAME)
     )
 
 
-def capture_mismatch_data_and_columns(
-    source: DataFrame, target: DataFrame, key_columns: list[str]
-) -> (DataFrame, list[str]):
+def capture_mismatch_data_and_columns(source: DataFrame, target: DataFrame, key_columns: list[str]) -> MismatchOutput:
     source_columns = source.columns
     target_columns = target.columns
 
     if source_columns != target_columns:
         message = "source and target should have same columns for capturing the mismatch data"
         source_missing = [column for column in target_columns if column not in source_columns]
         target_missing = [column for column in source_columns if column not in target_columns]
         raise raise_column_mismatch_exception(message, source_missing, target_missing)
 
     check_columns = [column for column in source_columns if column not in key_columns]
     mismatch_df = _get_mismatch_df(source, target, key_columns, check_columns)
     mismatch_columns = _get_mismatch_columns(mismatch_df, check_columns)
-    return mismatch_df, mismatch_columns
+    return MismatchOutput(mismatch_df, mismatch_columns)
 
 
 def _get_mismatch_columns(df: DataFrame, columns: list[str]):
     mismatch_columns = []
     for column in columns:
         if df.where(~col(column + "_match")).take(1):
             mismatch_columns.append(column)
@@ -81,23 +96,24 @@
 
 
 def _get_mismatch_df(source: DataFrame, target: DataFrame, key_columns: list[str], column_list: list[str]):
     source_aliased = [col('base.' + column).alias(column + '_base') for column in column_list]
     target_aliased = [col('compare.' + column).alias(column + '_compare') for column in column_list]
 
     match_expr = [expr(f"{column}_base=={column}_compare").alias(column + "_match") for column in column_list]
-    select_expr = key_columns + source_aliased + target_aliased + match_expr
+    key_cols = [col(column) for column in key_columns]
+    select_expr = key_cols + source_aliased + target_aliased + match_expr
 
     filter_columns = " and ".join([column + "_match" for column in column_list])
     filter_expr = ~expr(filter_columns)
 
     mismatch_df = (
         source.alias('base')
         .join(other=target.alias('compare'), on=key_columns, how="inner")
-        .select(select_expr)
+        .select(*select_expr)
         .filter(filter_expr)
     )
     compare_columns = [column for column in mismatch_df.columns if column not in key_columns]
     return mismatch_df.select(*key_columns + sorted(compare_columns))
 
 
 def alias_column_str(alias: str, columns: list[str]) -> list[str]:
```

### Comparing `databricks_labs_remorph-0.1.7/databricks/labs/remorph/reconcile/schema_compare.py` & `databricks_labs_remorph-0.2.0/databricks/labs/remorph/reconcile/schema_compare.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,22 +1,22 @@
 import logging
 from dataclasses import asdict
 
 from pyspark.sql import DataFrame, SparkSession
 from pyspark.sql.types import BooleanType, StringType, StructField, StructType
-from sqlglot import parse_one
+from sqlglot import Dialect, parse_one
 
-from databricks.labs.remorph.config import SQLGLOT_DIALECTS
-from databricks.labs.remorph.reconcile.constants import SourceType
+from databricks.labs.remorph.config import get_dialect
 from databricks.labs.remorph.reconcile.recon_config import (
     Schema,
     SchemaMatchResult,
-    SchemCompareOutput,
+    SchemaReconcileOutput,
     Table,
 )
+from databricks.labs.remorph.snow.databricks import Databricks
 
 logger = logging.getLogger(__name__)
 
 
 class SchemaCompare:
     def __init__(
         self,
@@ -45,15 +45,15 @@
         master_schema = source_schema
         if table_conf.select_columns:
             master_schema = [schema for schema in master_schema if schema.column_name in table_conf.select_columns]
         if table_conf.drop_columns:
             master_schema = [sschema for sschema in master_schema if sschema.column_name not in table_conf.drop_columns]
 
         target_column_map = table_conf.to_src_col_map or {}
-        master_schema = [
+        master_schema_match_res = [
             SchemaMatchResult(
                 source_column=s.column_name,
                 databricks_column=target_column_map.get(s.column_name, s.column_name),
                 source_datatype=s.data_type,
                 databricks_datatype=next(
                     (
                         tgt.data_type
@@ -61,32 +61,32 @@
                         if tgt.column_name == target_column_map.get(s.column_name, s.column_name)
                     ),
                     "",
                 ),
             )
             for s in master_schema
         ]
-        return master_schema
+        return master_schema_match_res
 
     def _create_dataframe(self, data: list, schema: StructType) -> DataFrame:
         """
         :param data: Expectation is list of dataclass
         :param schema: Target schema
         :return: DataFrame
         """
         data = [tuple(asdict(item).values()) for item in data]
         df = self.spark.createDataFrame(data, schema)
 
         return df
 
     @classmethod
-    def _parse(cls, source: str, column: str, data_type: str) -> str:
+    def _parse(cls, source: Dialect, column: str, data_type: str) -> str:
         return (
-            parse_one(f"create table dummy ({column} {data_type})", read=SQLGLOT_DIALECTS.get(source))
-            .sql(dialect=SQLGLOT_DIALECTS.get("databricks"))
+            parse_one(f"create table dummy ({column} {data_type})", read=source)
+            .sql(dialect=get_dialect("databricks"))
             .replace(", ", ",")
         )
 
     @classmethod
     def _table_schema_status(cls, schema_compare_maps: list[SchemaMatchResult]) -> bool:
         return bool(all(x.is_valid for x in schema_compare_maps))
 
@@ -103,28 +103,28 @@
         if parsed_query.lower() != databricks_query.lower():
             master.is_valid = False
 
     def compare(
         self,
         source_schema: list[Schema],
         databricks_schema: list[Schema],
-        source: str,
+        source: Dialect,
         table_conf: Table,
-    ) -> SchemCompareOutput:
+    ) -> SchemaReconcileOutput:
         """
         This method compares the source schema and the Databricks schema. It checks if the data types of the columns in the source schema
         match with the corresponding columns in the Databricks schema by parsing using remorph transpile.
 
         Returns:
-            SchemCompareOutput: A dataclass object containing a boolean indicating the overall result of the comparison and a DataFrame with the comparison details.
+            SchemaReconcileOutput: A dataclass object containing a boolean indicating the overall result of the comparison and a DataFrame with the comparison details.
         """
         master_schema = self._build_master_schema(source_schema, databricks_schema, table_conf)
         for master in master_schema:
-            if source.upper() != str(SourceType.DATABRICKS.value).upper():
+            if not isinstance(source, Databricks):
                 parsed_query = self._parse(source, master.source_column, master.source_datatype)
                 self._validate_parsed_query(master, parsed_query)
             elif master.source_datatype.lower() != master.databricks_datatype.lower():
                 master.is_valid = False
 
         df = self._create_dataframe(master_schema, self._schema_compare_schema)
         final_result = self._table_schema_status(master_schema)
-        return SchemCompareOutput(final_result, df)
+        return SchemaReconcileOutput(final_result, df)
```

### Comparing `databricks_labs_remorph-0.1.7/databricks/labs/remorph/reconcile/connectors/data_source.py` & `databricks_labs_remorph-0.2.0/databricks/labs/remorph/reconcile/connectors/data_source.py`

 * *Files 26% similar despite different names*

```diff
@@ -1,60 +1,72 @@
-import re
+import logging
 from abc import ABC, abstractmethod
 
-from pyspark.sql import DataFrame, SparkSession
+from pyspark.sql import DataFrame
 
+from databricks.labs.remorph.reconcile.exception import DataSourceRuntimeException
 from databricks.labs.remorph.reconcile.recon_config import JdbcReaderOptions, Schema
-from databricks.sdk import WorkspaceClient
+
+logger = logging.getLogger(__name__)
 
 
 class DataSource(ABC):
-    # TODO need to remove connection_params
-    def __init__(
-        self,
-        engine: str,
-        spark: SparkSession,
-        ws: WorkspaceClient,
-        scope: str,
-    ):
-        self.engine = engine
-        self.spark = spark
-        self.ws = ws
-        self.scope = scope
 
     @abstractmethod
-    def read_data(self, catalog: str, schema: str, query: str, options: JdbcReaderOptions) -> DataFrame:
+    def read_data(
+        self,
+        catalog: str | None,
+        schema: str,
+        table: str,
+        query: str,
+        options: JdbcReaderOptions | None,
+    ) -> DataFrame:
         return NotImplemented
 
     @abstractmethod
-    def get_schema(self, catalog: str, schema: str, table: str) -> list[Schema]:
+    def get_schema(
+        self,
+        catalog: str | None,
+        schema: str,
+        table: str,
+    ) -> list[Schema]:
         return NotImplemented
 
-    def _get_jdbc_reader(self, query, jdbc_url, driver):
-        return (
-            self.spark.read.format("jdbc")
-            .option("url", jdbc_url)
-            .option("driver", driver)
-            .option("dbtable", f"({query}) tmp")
-        )
-
-    @staticmethod
-    def _get_jdbc_reader_options(options: JdbcReaderOptions):
-        return {
-            "numPartitions": options.number_partitions,
-            "partitionColumn": options.partition_column,
-            "lowerBound": options.lower_bound,
-            "upperBound": options.upper_bound,
-            "fetchsize": options.fetch_size,
-        }
-
-    def _get_secrets(self, key_name: str):
-        key = self.engine + '_' + key_name
-        return self.ws.secrets.get_secret(self.scope, key)
-
-    @staticmethod
-    def _get_table_or_query(catalog: str, schema: str, query: str) -> str:
-        if re.search('select', query, re.IGNORECASE):
-            return query.format(catalog_name=catalog, schema_name=schema)
-        if catalog and catalog != "hive_metastore":
-            return f"select * from {catalog}.{schema}.{query}"
-        return f"select * from {schema}.{query}"
+    @classmethod
+    def log_and_throw_exception(cls, exception: Exception, fetch_type: str, query: str):
+        error_msg = f"Runtime exception occurred while fetching {fetch_type} using {query} : {exception}"
+        logger.warning(error_msg)
+        raise DataSourceRuntimeException(error_msg)
+
+
+class MockDataSource(DataSource):
+
+    def __init__(
+        self,
+        dataframe_repository: dict[tuple[str, str, str], DataFrame],
+        schema_repository: dict[tuple[str, str, str], list[Schema]],
+        exception: Exception = RuntimeError("Mock Exception"),
+    ):
+        self._dataframe_repository: dict[tuple[str, str, str], DataFrame] = dataframe_repository
+        self._schema_repository: dict[tuple[str, str, str], list[Schema]] = schema_repository
+        self._exception = exception
+
+    def read_data(
+        self,
+        catalog: str | None,
+        schema: str,
+        table: str,
+        query: str,
+        options: JdbcReaderOptions | None,
+    ) -> DataFrame:
+        catalog_str = catalog if catalog else ""
+        mock_df = self._dataframe_repository.get((catalog_str, schema, query))
+        if not mock_df:
+            return self.log_and_throw_exception(self._exception, "data", f"({catalog}, {schema}, {query})")
+        return mock_df
+
+    def get_schema(self, catalog: str | None, schema: str, table: str) -> list[Schema]:
+        catalog_str = catalog if catalog else ""
+        mock_schema = self._schema_repository.get((catalog_str, schema, table))
+        if not mock_schema:
+            return self.log_and_throw_exception(self._exception, "schema", f"({catalog}, {schema}, {table})")
+        return mock_schema
```

### Comparing `databricks_labs_remorph-0.1.7/databricks/labs/remorph/reconcile/connectors/databricks.py` & `databricks_labs_remorph-0.2.0/databricks/labs/remorph/reconcile/connectors/databricks.py`

 * *Files 26% similar despite different names*

```diff
@@ -1,49 +1,72 @@
+import logging
 import re
 
 from pyspark.errors import PySparkException
-from pyspark.sql import DataFrame
+from pyspark.sql import DataFrame, SparkSession
 from pyspark.sql.functions import col
+from sqlglot import Dialect
 
 from databricks.labs.remorph.reconcile.connectors.data_source import DataSource
+from databricks.labs.remorph.reconcile.connectors.secrets import SecretsMixin
 from databricks.labs.remorph.reconcile.recon_config import JdbcReaderOptions, Schema
+from databricks.sdk import WorkspaceClient
 
+logger = logging.getLogger(__name__)
 
-class DatabricksDataSource(DataSource):
-    def read_data(self, catalog: str, schema: str, query: str, options: JdbcReaderOptions) -> DataFrame:
+
+def _get_schema_query(catalog: str, schema: str, table: str):
+    # TODO: Ensure that the target_catalog in the configuration is not set to "hive_metastore". The source_catalog
+    #  can only be set to "hive_metastore" if the source type is "databricks".
+    if catalog == "hive_metastore":
+        return f"describe table {catalog}.{schema}.{table}"
+
+    query = f"""select lower(column_name) as col_name, full_data_type as data_type from 
+                {catalog}.information_schema.columns where lower(table_catalog)='{catalog}' 
+                and lower(table_schema)='{schema}' and lower(table_name) ='{table}' order by 
+                col_name"""
+    return re.sub(r'\s+', ' ', query)
+
+
+class DatabricksDataSource(DataSource, SecretsMixin):
+
+    def __init__(
+        self,
+        engine: Dialect,
+        spark: SparkSession,
+        ws: WorkspaceClient,
+        secret_scope: str,
+    ):
+        self._engine = engine
+        self._spark = spark
+        self._ws = ws
+        self._secret_scope = secret_scope
+
+    def read_data(
+        self,
+        catalog: str | None,
+        schema: str,
+        table: str,
+        query: str,
+        options: JdbcReaderOptions | None,
+    ) -> DataFrame:
+        table_with_namespace = f"{catalog}.{schema}.{table}"
+        table_query = query.replace(":tbl", table_with_namespace)
         try:
-            table_query = self._get_table_or_query(catalog, schema, query)
-            df = self.spark.sql(table_query)
+            df = self._spark.sql(table_query)
             return df.select([col(column).alias(column.lower()) for column in df.columns])
-        except PySparkException as e:
-            error_msg = (
-                f"An error occurred while fetching Databricks Data using the following {table_query} in "
-                f"DatabricksDataSource : {e!s}"
-            )
-            raise PySparkException(error_msg) from e
+        except (RuntimeError, PySparkException) as e:
+            return self.log_and_throw_exception(e, "data", table_query)
 
-    def get_schema(self, catalog: str, schema: str, table: str) -> list[Schema]:
+    def get_schema(
+        self,
+        catalog: str | None,
+        schema: str,
+        table: str,
+    ) -> list[Schema]:
+        catalog_str = catalog if catalog else "hive_metastore"
+        schema_query = _get_schema_query(catalog_str, schema, table)
         try:
-            schema_query = self.get_schema_query(catalog, schema, table)
-            schema_df = self.spark.sql(schema_query).where("col_name not like '#%'").distinct()
+            schema_df = self._spark.sql(schema_query).where("col_name not like '#%'").distinct()
             return [Schema(field.col_name.lower(), field.data_type.lower()) for field in schema_df.collect()]
-        except PySparkException as e:
-            error_msg = (
-                f"An error occurred while fetching Databricks Schema using the following "
-                f"{schema_query} query in DatabricksDataSource: {e!s}"
-            )
-            raise PySparkException(error_msg) from e
-
-    @staticmethod
-    def get_schema_query(catalog: str, schema: str, table: str):
-        # TODO: Ensure that the target_catalog in the configuration is not set to "hive_metastore". The source_catalog
-        #  can only be set to "hive_metastore" if the source type is "databricks".
-        if catalog == "hive_metastore":
-            return f"describe table {schema}.{table}"
-
-        query = f"""select lower(column_name) as col_name, full_data_type as data_type from 
-                    {catalog}.information_schema.columns where lower(table_catalog)='{catalog}' 
-                    and lower(table_schema)='{schema}' and lower(table_name) ='{table}' order by 
-                    col_name"""
-        return re.sub(r'\s+', ' ', query)
-
-    databricks_datatype_mapper = {}
+        except (RuntimeError, PySparkException) as e:
+            return self.log_and_throw_exception(e, "schema", schema_query)
```

### Comparing `databricks_labs_remorph-0.1.7/databricks/labs/remorph/reconcile/connectors/oracle.py` & `databricks_labs_remorph-0.2.0/databricks/labs/remorph/reconcile/connectors/oracle.py`

 * *Files 19% similar despite different names*

```diff
@@ -1,72 +1,93 @@
+import re
+
 from pyspark.errors import PySparkException
-from pyspark.sql import DataFrame, DataFrameReader
+from pyspark.sql import DataFrame, DataFrameReader, SparkSession
+from sqlglot import Dialect
 
 from databricks.labs.remorph.reconcile.connectors.data_source import DataSource
-from databricks.labs.remorph.reconcile.constants import SourceDriver, SourceType
+from databricks.labs.remorph.reconcile.connectors.jdbc_reader import JDBCReaderMixin
+from databricks.labs.remorph.reconcile.connectors.secrets import SecretsMixin
 from databricks.labs.remorph.reconcile.recon_config import JdbcReaderOptions, Schema
+from databricks.sdk import WorkspaceClient
+
+
+class OracleDataSource(DataSource, SecretsMixin, JDBCReaderMixin):
+    _DRIVER = "oracle"
+    _SCHEMA_QUERY = """select column_name, case when (data_precision is not null
+                                              and data_scale <> 0)
+                                              then data_type || '(' || data_precision || ',' || data_scale || ')'
+                                              when (data_precision is not null and data_scale = 0)
+                                              then data_type || '(' || data_precision || ')'
+                                              when data_precision is null and (lower(data_type) in ('date') or
+                                              lower(data_type) like 'timestamp%') then  data_type
+                                              when CHAR_LENGTH == 0 then data_type
+                                              else data_type || '(' || CHAR_LENGTH || ')'
+                                              end data_type
+                                              FROM ALL_TAB_COLUMNS
+                            WHERE lower(TABLE_NAME) = '{table}' and lower(owner) = '{owner}'"""
 
+    def __init__(
+        self,
+        engine: Dialect,
+        spark: SparkSession,
+        ws: WorkspaceClient,
+        secret_scope: str,
+    ):
+        self._engine = engine
+        self._spark = spark
+        self._ws = ws
+        self._secret_scope = secret_scope
 
-class OracleDataSource(DataSource):
     @property
     def get_jdbc_url(self) -> str:
         return (
-            f"jdbc:{SourceType.ORACLE.value}:thin:{self._get_secrets('user')}"
-            f"/{self._get_secrets('password')}@//{self._get_secrets('host')}"
-            f":{self._get_secrets('port')}/{self._get_secrets('database')}"
+            f"jdbc:{OracleDataSource._DRIVER}:thin:{self._get_secret('user')}"
+            f"/{self._get_secret('password')}@//{self._get_secret('host')}"
+            f":{self._get_secret('port')}/{self._get_secret('database')}"
         )
 
-    def read_data(self, catalog: str, schema: str, query: str, options: JdbcReaderOptions) -> DataFrame:
+    def read_data(
+        self,
+        catalog: str | None,
+        schema: str,
+        table: str,
+        query: str,
+        options: JdbcReaderOptions | None,
+    ) -> DataFrame:
+        table_query = query.replace(":tbl", f"{schema}.{table}")
         try:
-            table_query = self._get_table_or_query(catalog, schema, query)
             if options is None:
                 return self.reader(table_query).options(**self._get_timestamp_options()).load()
-            options = self._get_jdbc_reader_options(options) | self._get_timestamp_options()
-            return self.reader(table_query).options(**options).load()
-        except PySparkException as e:
-            error_msg = (
-                f"An error occurred while fetching Oracle Data using the following {query} in OracleDataSource : {e!s}"
-            )
-            raise PySparkException(error_msg) from e
-
-    def get_schema(self, catalog: str, schema: str, table: str) -> list[Schema]:
+            reader_options = self._get_jdbc_reader_options(options) | self._get_timestamp_options()
+            return self.reader(table_query).options(**reader_options).load()
+        except (RuntimeError, PySparkException) as e:
+            return self.log_and_throw_exception(e, "data", table_query)
+
+    def get_schema(
+        self,
+        catalog: str | None,
+        schema: str,
+        table: str,
+    ) -> list[Schema]:
+        schema_query = re.sub(
+            r'\s+',
+            ' ',
+            OracleDataSource._SCHEMA_QUERY.format(table=table, owner=schema),
+        )
         try:
-            schema_query = self._get_schema_query(table, schema)
             schema_df = self.reader(schema_query).load()
             return [Schema(field.column_name.lower(), field.data_type.lower()) for field in schema_df.collect()]
-        except PySparkException as e:
-            error_msg = (
-                f"An error occurred while fetching Oracle Schema using the following {table} in "
-                f"OracleDataSource: {e!s}"
-            )
-            raise PySparkException(error_msg) from e
-
-    oracle_datatype_mapper = {
-        "date": "coalesce(trim(to_char({},'YYYY-MM-DD')),'')",
-    }
+        except (RuntimeError, PySparkException) as e:
+            return self.log_and_throw_exception(e, "schema", schema_query)
 
     @staticmethod
     def _get_timestamp_options() -> dict[str, str]:
         return {
             "oracle.jdbc.mapDateToTimestamp": "False",
-            "sessionInitStatement": """BEGIN dbms_session.set_nls('nls_date_format', '''YYYY-MM-DD''');
-                                 dbms_session.set_nls('nls_timestamp_format', '''YYYY-MM-DD HH24:MI:SS''');
-                           END;""",
+            "sessionInitStatement": "BEGIN dbms_session.set_nls('nls_date_format', "
+            "'''YYYY-MM-DD''');dbms_session.set_nls('nls_timestamp_format', '''YYYY-MM-DD "
+            "HH24:MI:SS''');END;",
         }
 
     def reader(self, query: str) -> DataFrameReader:
-        return self._get_jdbc_reader(query, self.get_jdbc_url, SourceDriver.ORACLE.value)
-
-    @staticmethod
-    def _get_schema_query(table: str, owner: str) -> str:
-        return f"""select column_name, case when (data_precision is not null
-                                              and data_scale <> 0)
-                                              then data_type || '(' || data_precision || ',' || data_scale || ')'
-                                              when (data_precision is not null and data_scale = 0)
-                                              then data_type || '(' || data_precision || ')'
-                                              when data_precision is null and (lower(data_type) in ('date') or
-                                              lower(data_type) like 'timestamp%') then  data_type
-                                              when CHAR_LENGTH == 0 then data_type
-                                              else data_type || '(' || CHAR_LENGTH || ')'
-                                              end data_type
-                                              FROM ALL_TAB_COLUMNS
-                            WHERE lower(TABLE_NAME) = '{table}' and lower(owner) = '{owner}' """
+        return self._get_jdbc_reader(query, self.get_jdbc_url, OracleDataSource._DRIVER)
```

### Comparing `databricks_labs_remorph-0.1.7/databricks/labs/remorph/reconcile/connectors/snowflake.py` & `databricks_labs_remorph-0.2.0/databricks/labs/remorph/reconcile/connectors/snowflake.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,76 +1,97 @@
+import logging
 import re
 
 from pyspark.errors import PySparkException
-from pyspark.sql import DataFrame
+from pyspark.sql import DataFrame, DataFrameReader, SparkSession
 from pyspark.sql.functions import col
+from sqlglot import Dialect
 
 from databricks.labs.remorph.reconcile.connectors.data_source import DataSource
-from databricks.labs.remorph.reconcile.constants import SourceDriver, SourceType
+from databricks.labs.remorph.reconcile.connectors.jdbc_reader import JDBCReaderMixin
+from databricks.labs.remorph.reconcile.connectors.secrets import SecretsMixin
 from databricks.labs.remorph.reconcile.recon_config import JdbcReaderOptions, Schema
+from databricks.sdk import WorkspaceClient
 
+logger = logging.getLogger(__name__)
+
+
+class SnowflakeDataSource(DataSource, SecretsMixin, JDBCReaderMixin):
+    _DRIVER = "snowflake"
+    _SCHEMA_QUERY = """select column_name, case when numeric_precision is not null and numeric_scale is not null then 
+        concat(data_type, '(', numeric_precision, ',' , numeric_scale, ')') when lower(data_type) = 'text' then 
+        concat('varchar', '(', CHARACTER_MAXIMUM_LENGTH, ')')  else data_type end as data_type from 
+        {catalog}.INFORMATION_SCHEMA.COLUMNS where lower(table_name)='{table}' 
+        and lower(table_schema) = '{schema}' order by ordinal_position"""
+
+    def __init__(
+        self,
+        engine: Dialect,
+        spark: SparkSession,
+        ws: WorkspaceClient,
+        secret_scope: str,
+    ):
+        self._engine = engine
+        self._spark = spark
+        self._ws = ws
+        self._secret_scope = secret_scope
 
-class SnowflakeDataSource(DataSource):
     @property
     def get_jdbc_url(self) -> str:
         return (
-            f"jdbc:{SourceType.SNOWFLAKE.value}://{self._get_secrets('account')}.snowflakecomputing.com"
-            f"/?user={self._get_secrets('sfUser')}&password={self._get_secrets('sfPassword')}"
-            f"&db={self._get_secrets('sfDatabase')}&schema={self._get_secrets('sfSchema')}"
-            f"&warehouse={self._get_secrets('sfWarehouse')}&role={self._get_secrets('sfRole')}"
+            f"jdbc:{SnowflakeDataSource._DRIVER}://{self._get_secret('sfAccount')}.snowflakecomputing.com"
+            f"/?user={self._get_secret('sfUser')}&password={self._get_secret('sfPassword')}"
+            f"&db={self._get_secret('sfDatabase')}&schema={self._get_secret('sfSchema')}"
+            f"&warehouse={self._get_secret('sfWarehouse')}&role={self._get_secret('sfRole')}"
         )
 
-    def read_data(self, catalog: str, schema: str, query: str, options: JdbcReaderOptions) -> DataFrame:
+    def read_data(
+        self,
+        catalog: str | None,
+        schema: str,
+        table: str,
+        query: str,
+        options: JdbcReaderOptions | None,
+    ) -> DataFrame:
+        table_query = query.replace(":tbl", f"{catalog}.{schema}.{table}")
         try:
-            table_query = self._get_table_or_query(catalog, schema, query)
-
             if options is None:
-                df = self.reader(table_query)
+                df = self.reader(table_query).load()
             else:
                 options = self._get_jdbc_reader_options(options)
                 df = (
-                    self._get_jdbc_reader(table_query, self.get_jdbc_url, SourceDriver.SNOWFLAKE.value)
+                    self._get_jdbc_reader(table_query, self.get_jdbc_url, SnowflakeDataSource._DRIVER)
                     .options(**options)
                     .load()
                 )
             return df.select([col(column).alias(column.lower()) for column in df.columns])
-        except PySparkException as e:
-            error_msg = (
-                f"An error occurred while fetching Snowflake Data using the following {query} in "
-                f"SnowflakeDataSource : {e!s}"
-            )
-            raise PySparkException(error_msg) from e
+        except (RuntimeError, PySparkException) as e:
+            return self.log_and_throw_exception(e, "data", table_query)
 
-    def get_schema(self, catalog: str, schema: str, table: str) -> list[Schema]:
+    def get_schema(
+        self,
+        catalog: str | None,
+        schema: str,
+        table: str,
+    ) -> list[Schema]:
+        schema_query = re.sub(
+            r'\s+',
+            ' ',
+            SnowflakeDataSource._SCHEMA_QUERY.format(catalog=catalog, schema=schema, table=table),
+        )
         try:
-            schema_query = self.get_schema_query(catalog, schema, table)
             schema_df = self.reader(schema_query).load()
             return [Schema(field.column_name.lower(), field.data_type.lower()) for field in schema_df.collect()]
-        except PySparkException as e:
-            error_msg = (
-                f"An error occurred while fetching Snowflake Schema using the following {table} in "
-                f"SnowflakeDataSource: {e!s}"
-            )
-            raise PySparkException(error_msg) from e
+        except (RuntimeError, PySparkException) as e:
+            return self.log_and_throw_exception(e, "schema", schema_query)
 
-    def reader(self, query: str) -> DataFrame:
+    def reader(self, query: str) -> DataFrameReader:
         options = {
-            "sfUrl": self._get_secrets('sfUrl'),
-            "sfUser": self._get_secrets('sfUser'),
-            "sfPassword": self._get_secrets('sfPassword'),
-            "sfDatabase": self._get_secrets('sfDatabase'),
-            "sfSchema": self._get_secrets('sfSchema'),
-            "sfWarehouse": self._get_secrets('sfWarehouse'),
-            "sfRole": self._get_secrets('sfRole'),
+            "sfUrl": self._get_secret('sfUrl'),
+            "sfUser": self._get_secret('sfUser'),
+            "sfPassword": self._get_secret('sfPassword'),
+            "sfDatabase": self._get_secret('sfDatabase'),
+            "sfSchema": self._get_secret('sfSchema'),
+            "sfWarehouse": self._get_secret('sfWarehouse'),
+            "sfRole": self._get_secret('sfRole'),
         }
-        return self.spark.read.format("snowflake").option("dbtable", f"({query}) as tmp").options(**options).load()
-
-    @staticmethod
-    def get_schema_query(catalog: str, schema: str, table: str):
-        query = f"""select column_name, case when numeric_precision is not null and numeric_scale is not null then 
-        concat(data_type, '(', numeric_precision, ',' , numeric_scale, ')') when lower(data_type) = 'text' then 
-        concat('varchar', '(', CHARACTER_MAXIMUM_LENGTH, ')')  else data_type end as data_type from 
-        {catalog}.INFORMATION_SCHEMA.COLUMNS where lower(table_name)='{table}' 
-        and lower(table_schema) = '{schema}' order by ordinal_position"""
-        return re.sub(r'\s+', ' ', query)
-
-    snowflake_datatype_mapper = {}
+        return self._spark.read.format("snowflake").option("dbtable", f"({query}) as tmp").options(**options)
```

### Comparing `databricks_labs_remorph-0.1.7/databricks/labs/remorph/reconcile/query_builder/base.py` & `databricks_labs_remorph-0.2.0/databricks/labs/remorph/reconcile/query_builder/base.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,28 +1,35 @@
 from abc import ABC
 
 import sqlglot.expressions as exp
-from sqlglot import parse_one
+from sqlglot import Dialect, parse_one
 
+from databricks.labs.remorph.config import SQLGLOT_DIALECTS
 from databricks.labs.remorph.reconcile.query_builder.expression_generator import (
     DataType_transform_mapping,
     transform_expression,
 )
 from databricks.labs.remorph.reconcile.recon_config import Schema, Table
 
 
 class QueryBuilder(ABC):
-    def __init__(self, table_conf: Table, schema: list[Schema], layer: str, source: str):
+    def __init__(
+        self,
+        table_conf: Table,
+        schema: list[Schema],
+        layer: str,
+        source: Dialect,
+    ):
         self._table_conf = table_conf
         self._schema = schema
         self._layer = layer
         self._source = source
 
     @property
-    def source(self) -> str:
+    def source(self) -> Dialect:
         return self._source
 
     @property
     def layer(self) -> str:
         return self._layer
 
     @property
@@ -57,53 +64,61 @@
     def filter(self) -> str | None:
         return self._table_conf.get_filter(self._layer)
 
     @property
     def user_transformations(self) -> dict[str, str]:
         return self._table_conf.get_transformation_dict(self._layer)
 
-    def add_transformations(self, aliases: list[exp.Alias], source: str) -> list[exp.Alias]:
+    def add_transformations(self, aliases: list[exp.Expression], source: Dialect) -> list[exp.Expression]:
         if self.user_transformations:
             alias_with_user_transforms = self._apply_user_transformation(aliases)
             default_transform_schema: list[Schema] = list(
                 filter(lambda sch: sch.column_name not in self.user_transformations.keys(), self.schema)
             )
             return self._apply_default_transformation(alias_with_user_transforms, default_transform_schema, source)
         return self._apply_default_transformation(aliases, self.schema, source)
 
-    def _apply_user_transformation(self, aliases: list[exp.Alias]) -> list[exp.Alias]:
+    def _apply_user_transformation(self, aliases: list[exp.Expression]) -> list[exp.Expression]:
         with_transform = []
         for alias in aliases:
             with_transform.append(alias.transform(self._user_transformer, self.user_transformations))
         return with_transform
 
     @staticmethod
     def _user_transformer(node: exp.Expression, user_transformations: dict[str, str]) -> exp.Expression:
         if isinstance(node, exp.Column) and user_transformations:
             column_name = node.name
             if column_name in user_transformations.keys():
-                return parse_one(user_transformations.get(column_name))
+                return parse_one(user_transformations.get(column_name, column_name))
         return node
 
-    def _apply_default_transformation(self, aliases: list[exp.Alias], schema: list[Schema], source) -> list[exp.Alias]:
+    def _apply_default_transformation(
+        self, aliases: list[exp.Expression], schema: list[Schema], source: Dialect
+    ) -> (list)[exp.Expression]:
         with_transform = []
         for alias in aliases:
             with_transform.append(alias.transform(self._default_transformer, schema, source))
         return with_transform
 
     @staticmethod
-    def _default_transformer(node: exp.Expression, schema: list[Schema], source) -> exp.Expression:
+    def _default_transformer(node: exp.Expression, schema: list[Schema], source: Dialect) -> exp.Expression:
+
         def _get_transform(datatype: str):
-            if DataType_transform_mapping.get(source) is not None:
-                if DataType_transform_mapping.get(source).get(datatype.upper()) is not None:
-                    return DataType_transform_mapping.get(source).get(datatype.upper())
-                if DataType_transform_mapping.get(source).get("default") is not None:
-                    return DataType_transform_mapping.get(source).get("default")
-            return DataType_transform_mapping.get("default")
+            source_dialects = [source_key for source_key, dialect in SQLGLOT_DIALECTS.items() if dialect == source]
+            source_dialect = source_dialects[0] if source_dialects else "universal"
+
+            source_mapping = DataType_transform_mapping.get(source_dialect, {})
+
+            if source_mapping.get(datatype.upper()) is not None:
+                return source_mapping.get(datatype.upper())
+            if source_mapping.get("default") is not None:
+                return source_mapping.get("default")
+
+            return DataType_transform_mapping.get("universal", {}).get("default")
 
         schema_dict = {v.column_name: v.data_type for v in schema}
         if isinstance(node, exp.Column):
             column_name = node.name
             if column_name in schema_dict.keys():
-                transform = _get_transform(schema_dict.get(column_name))
+                transform = _get_transform(schema_dict.get(column_name, column_name))
                 return transform_expression(node, transform)
         return node
```

### Comparing `databricks_labs_remorph-0.1.7/databricks/labs/remorph/reconcile/query_builder/expression_generator.py` & `databricks_labs_remorph-0.2.0/databricks/labs/remorph/reconcile/query_builder/expression_generator.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,12 +1,15 @@
 from collections.abc import Callable
 from functools import partial
 
+from pyspark.sql.types import DataType, NumericType
+from sqlglot import Dialect
 from sqlglot import expressions as exp
 
+from databricks.labs.remorph.config import get_dialect
 from databricks.labs.remorph.reconcile.recon_config import DialectHashConfig
 
 
 def _apply_func_expr(expr: exp.Expression, expr_func: Callable, **kwargs) -> exp.Expression:
     is_terminal = isinstance(expr, exp.Column)
     new_expr = expr.copy()
     for node in new_expr.dfs():
@@ -32,61 +35,61 @@
 
 def lower(expr: exp.Expression, is_expr: bool = False) -> exp.Expression:
     if is_expr:
         return exp.Lower(this=expr)
     return _apply_func_expr(expr, exp.Lower)
 
 
-def coalesce(expr: exp.Expression, default="0", is_string=False) -> exp.Coalesce | exp.Expression:
+def coalesce(expr: exp.Expression, default="0", is_string=False) -> exp.Expression:
     expressions = [exp.Literal(this=default, is_string=is_string)]
     return _apply_func_expr(expr, exp.Coalesce, expressions=expressions)
 
 
 def trim(expr: exp.Expression) -> exp.Trim | exp.Expression:
     return _apply_func_expr(expr, exp.Trim)
 
 
-def json_format(expr: exp.Expression, options: dict[str, str] | None = None) -> exp.JSONFormat | exp.Expression:
+def json_format(expr: exp.Expression, options: dict[str, str] | None = None) -> exp.Expression:
     return _apply_func_expr(expr, exp.JSONFormat, options=options)
 
 
-def sort_array(expr: exp.Expression, asc=True):
+def sort_array(expr: exp.Expression, asc=True) -> exp.Expression:
     return _apply_func_expr(expr, exp.SortArray, asc=exp.Boolean(this=asc))
 
 
-def to_char(expr: exp.Expression, to_format=None, nls_param=None):
+def to_char(expr: exp.Expression, to_format=None, nls_param=None) -> exp.Expression:
     if to_format:
         return _apply_func_expr(
             expr, exp.ToChar, format=exp.Literal(this=to_format, is_string=True), nls_param=nls_param
         )
     return _apply_func_expr(expr, exp.ToChar)
 
 
 def array_to_string(
     expr: exp.Expression,
     delimiter: str = ",",
     is_string=True,
     null_replacement: str | None = None,
     is_null_replace=True,
-):
+) -> exp.Expression:
     if null_replacement:
         return _apply_func_expr(
             expr,
             exp.ArrayToString,
             expression=[exp.Literal(this=delimiter, is_string=is_string)],
             null=exp.Literal(this=null_replacement, is_string=is_null_replace),
         )
     return _apply_func_expr(expr, exp.ArrayToString, expression=[exp.Literal(this=delimiter, is_string=is_string)])
 
 
-def array_sort(expr: exp.Expression, asc=True):
+def array_sort(expr: exp.Expression, asc=True) -> exp.Expression:
     return _apply_func_expr(expr, exp.ArraySort, expression=exp.Boolean(this=asc))
 
 
-def anonymous(expr: exp.Column, func: str, is_expr: bool = False) -> exp.Anonymous | exp.Expression:
+def anonymous(expr: exp.Column, func: str, is_expr: bool = False) -> exp.Expression:
     """
 
     This function used in cases where the sql functions are not available in sqlGlot expressions
     Example:
         >>> from sqlglot import parse_one
         >>> print(repr(parse_one('select unix_timestamp(col1)')))
 
@@ -110,25 +113,25 @@
             anonymous_func = exp.Column(this=func.format(name))
             if is_terminal:
                 return anonymous_func
             node.replace(anonymous_func)
     return new_expr
 
 
-def build_column(this: exp.ExpOrStr, table_name="", quoted=False, alias=None) -> exp.Alias | exp.Column:
+def build_column(this: exp.ExpOrStr, table_name="", quoted=False, alias=None) -> exp.Expression:
     if alias:
         if isinstance(this, str):
             return exp.Alias(
                 this=exp.Column(this=this, table=table_name), alias=exp.Identifier(this=alias, quoted=quoted)
             )
         return exp.Alias(this=this, alias=exp.Identifier(this=alias, quoted=quoted))
     return exp.Column(this=exp.Identifier(this=this, quoted=quoted), table=table_name)
 
 
-def build_literal(this: exp.ExpOrStr, alias=None, quoted=False, is_string=True) -> exp.Alias | exp.Literal:
+def build_literal(this: exp.ExpOrStr, alias=None, quoted=False, is_string=True) -> exp.Expression:
     if alias:
         return exp.Alias(
             this=exp.Literal(this=this, is_string=is_string), alias=exp.Identifier(this=alias, quoted=quoted)
         )
     return exp.Literal(this=this, is_string=is_string)
 
 
@@ -140,15 +143,15 @@
         expr = func(expr)
     assert isinstance(expr, exp.Expression), (
         f"Func returned an instance of type [{type(expr)}], " "should have been Expression."
     )
     return expr
 
 
-def get_hash_transform(source: str):
+def get_hash_transform(source: Dialect):
     dialect_algo = list(filter(lambda dialect: dialect.dialect == source, Dialect_hash_algo_mapping))
     if dialect_algo:
         return dialect_algo[0].algo
     raise ValueError(f"Source {source} is not supported")
 
 
 def build_from_clause(table_name: str, table_alias: str | None = None) -> exp.From:
@@ -167,15 +170,15 @@
         join_condition = exp.NullSafeEQ(
             this=exp.Column(this=column, table=source_table_alias),
             expression=exp.Column(this=column, table=target_table_alias),
         )
         join_conditions.append(join_condition)
 
     # Combine all join conditions with AND
-    on_condition = join_conditions[0]
+    on_condition: exp.NullSafeEQ | exp.And = join_conditions[0]
     for condition in join_conditions[1:]:
         on_condition = exp.And(this=on_condition, expression=condition)
 
     return exp.Join(
         this=exp.Table(this=exp.Identifier(this=table_name), alias=target_table_alias), kind=kind, on=on_condition
     )
 
@@ -188,18 +191,18 @@
 ) -> exp.Sub:
     return exp.Sub(
         this=build_column(left_column_name, left_table_name),
         expression=build_column(right_column_name, right_table_name),
     )
 
 
-def build_where_clause(where_clause=list[exp.Expression], condition_type: str = "or") -> exp.Or:
+def build_where_clause(where_clause: list[exp.Expression], condition_type: str = "or") -> exp.Expression:
     func = exp.Or if condition_type == "or" else exp.And
     # Start with a default
-    combined_expression = exp.Paren(this=func(this='1 = 1', expression='1 = 1'))
+    combined_expression: exp.Expression = exp.Paren(this=func(this='1 = 1', expression='1 = 1'))
 
     # Loop through the expressions and combine them with OR
     for expression in where_clause:
         combined_expression = func(this=combined_expression, expression=expression)
 
     return combined_expression
 
@@ -208,26 +211,33 @@
     return exp.If(this=this, true=true, false=false)
 
 
 def build_between(this: exp.Expression, low: exp.Expression, high: exp.Expression) -> exp.Between:
     return exp.Between(this=this, low=low, high=high)
 
 
-DataType_transform_mapping = {
-    "default": [partial(coalesce, default='', is_string=True), trim],
-    "snowflake": {exp.DataType.Type.ARRAY.value: [array_to_string, array_sort]},
+def _get_is_string(column_types_dict: dict[str, DataType], column_name: str) -> bool:
+    if isinstance(column_types_dict.get(column_name), NumericType):
+        return False
+    return True
+
+
+DataType_transform_mapping: dict[str, dict[str, list[partial[exp.Expression]]]] = {
+    "universal": {"default": [partial(coalesce, default='', is_string=True), partial(trim)]},
+    "snowflake": {exp.DataType.Type.ARRAY.value: [partial(array_to_string), partial(array_sort)]},
     "oracle": {
         exp.DataType.Type.NCHAR.value: [partial(anonymous, func="NVL(TRIM(TO_CHAR({})),'_null_recon_')")],
         exp.DataType.Type.NVARCHAR.value: [partial(anonymous, func="NVL(TRIM(TO_CHAR({})),'_null_recon_')")],
     },
     "databricks": {
         exp.DataType.Type.ARRAY.value: [partial(anonymous, func="CONCAT_WS(',', SORT_ARRAY({}))")],
     },
 }
 
 Dialect_hash_algo_mapping = [
-    DialectHashConfig(dialect="snowflake", algo=[partial(sha2, num_bits="256", is_expr=True)]),
+    DialectHashConfig(dialect=get_dialect("snowflake"), algo=[partial(sha2, num_bits="256", is_expr=True)]),
     DialectHashConfig(
-        dialect="oracle", algo=[partial(anonymous, func="RAWTOHEX(STANDARD_HASH({}, 'SHA256'))", is_expr=True)]
+        dialect=get_dialect("oracle"),
+        algo=[partial(anonymous, func="RAWTOHEX(STANDARD_HASH({}, 'SHA256'))", is_expr=True)],
     ),
-    DialectHashConfig(dialect="databricks", algo=[partial(sha2, num_bits="256", is_expr=True)]),
+    DialectHashConfig(dialect=get_dialect("databricks"), algo=[partial(sha2, num_bits="256", is_expr=True)]),
 ]
```

### Comparing `databricks_labs_remorph-0.1.7/databricks/labs/remorph/reconcile/query_builder/hash_query.py` & `databricks_labs_remorph-0.2.0/databricks/labs/remorph/reconcile/query_builder/hash_query.py`

 * *Files 19% similar despite different names*

```diff
@@ -1,49 +1,77 @@
+import logging
+
 import sqlglot.expressions as exp
+from sqlglot import Dialect
 
-from databricks.labs.remorph.reconcile.constants import Constants
 from databricks.labs.remorph.reconcile.query_builder.base import QueryBuilder
 from databricks.labs.remorph.reconcile.query_builder.expression_generator import (
     build_column,
     concat,
     get_hash_transform,
     lower,
     transform_expression,
 )
 
+logger = logging.getLogger(__name__)
+
+
+def _hash_transform(
+    node: exp.Expression,
+    source: Dialect,
+):
+    transform = get_hash_transform(source)
+    return transform_expression(node, transform)
+
+
+_HASH_COLUMN_NAME = "hash_value_recon"
+
 
 class HashQueryBuilder(QueryBuilder):
-    def build_query(self) -> str:
+
+    def build_query(self, report_type: str) -> str:
         hash_cols = sorted((self.join_columns | self.select_columns) - self.threshold_columns - self.drop_columns)
-        key_cols = sorted(self.join_columns | self.partition_column)
+
+        key_cols = hash_cols if report_type == "row" else sorted(self.join_columns | self.partition_column)
 
         cols_with_alias = [
-            build_column(this=col, alias=self.table_conf.get_tgt_to_src_col_mapping(col, self.layer))
+            build_column(this=col, alias=self.table_conf.get_layer_tgt_to_src_col_mapping(col, self.layer))
             for col in key_cols
         ]
 
-        key_cols_with_transform = self.add_transformations(cols_with_alias, self.source)
-        hash_col_with_transform = [self._generate_hash_algorithm(hash_cols)]
+        # in case if we have column mapping, we need to sort the target columns in the order of source columns to get
+        # same hash value
+        hash_cols_with_alias = [
+            {"this": col, "alias": self.table_conf.get_layer_tgt_to_src_col_mapping(col, self.layer)}
+            for col in hash_cols
+        ]
+        sorted_hash_cols_with_alias = sorted(hash_cols_with_alias, key=lambda column: column["alias"])
+        hashcols_sorted_as_src_seq = [column["this"] for column in sorted_hash_cols_with_alias]
+
+        key_cols_with_transform = (
+            self._apply_user_transformation(cols_with_alias) if self.user_transformations else cols_with_alias
+        )
+        hash_col_with_transform = [self._generate_hash_algorithm(hashcols_sorted_as_src_seq, _HASH_COLUMN_NAME)]
 
         res = (
             exp.select(*hash_col_with_transform + key_cols_with_transform)
             .from_(":tbl")
             .where(self.filter)
             .sql(dialect=self.source)
         )
 
+        logger.info(f"Hash Query for {self.layer}: {res}")
         return res
 
-    def _generate_hash_algorithm(self, cols: list[str]) -> exp.Expression:
+    def _generate_hash_algorithm(
+        self,
+        cols: list[str],
+        column_alias: str,
+    ) -> exp.Expression:
         cols_with_alias = [build_column(this=col, alias=None) for col in cols]
         cols_with_transform = self.add_transformations(cols_with_alias, self.source)
         col_exprs = exp.select(*cols_with_transform).iter_expressions()
         concat_expr = concat(list(col_exprs))
 
-        hash_expr = concat_expr.transform(self._hash_transform, self.source).transform(lower, is_expr=True)
-
-        return build_column(hash_expr, alias=Constants.hash_column_name)
+        hash_expr = concat_expr.transform(_hash_transform, self.source).transform(lower, is_expr=True)
 
-    @staticmethod
-    def _hash_transform(node: exp.Expression, source: str):
-        transform = get_hash_transform(source)
-        return transform_expression(node, transform)
+        return build_column(hash_expr, alias=column_alias)
```

### Comparing `databricks_labs_remorph-0.1.7/databricks/labs/remorph/reconcile/query_builder/sampling_query.py` & `databricks_labs_remorph-0.2.0/databricks/labs/remorph/reconcile/query_builder/sampling_query.py`

 * *Files 9% similar despite different names*

```diff
@@ -1,57 +1,78 @@
+import logging
+
 import sqlglot.expressions as exp
 from pyspark.sql import DataFrame
 from sqlglot import select
 
-from databricks.labs.remorph.reconcile.constants import SampleConfig
 from databricks.labs.remorph.reconcile.query_builder.base import QueryBuilder
 from databricks.labs.remorph.reconcile.query_builder.expression_generator import (
     build_column,
     build_literal,
+    _get_is_string,
 )
 
+_SAMPLE_ROWS = 50
+
+logger = logging.getLogger(__name__)
+
 
-def _union_concat(unions: list[exp.Select], result: exp.Union | exp.Select, cnt=0) -> exp.Select | exp.Union:
+def _union_concat(
+    unions: list[exp.Select],
+    result: exp.Union | exp.Select,
+    cnt=0,
+) -> exp.Select | exp.Union:
     if len(unions) == 1:
         return result
     if cnt == len(unions) - 2:
         return exp.union(result, unions[cnt + 1])
     cnt = cnt + 1
     res = exp.union(result, unions[cnt])
     return _union_concat(unions, res, cnt)
 
 
 class SamplingQueryBuilder(QueryBuilder):
     def build_query(self, df: DataFrame):
         if self.layer == "source":
             key_cols = sorted(self.join_columns)
         else:
-            key_cols = sorted(self.table_conf.get_tgt_to_src_col_mapping(self.join_columns, self.layer))
+            key_cols = sorted(self.table_conf.get_tgt_to_src_col_mapping_list(self.join_columns))
         keys_df = df.select(*key_cols)
         with_clause = self._get_with_clause(keys_df)
 
         cols = sorted((self.join_columns | self.select_columns) - self.threshold_columns - self.drop_columns)
 
         cols_with_alias = [
-            build_column(this=col, alias=self.table_conf.get_tgt_to_src_col_mapping(col, self.layer)) for col in cols
+            build_column(this=col, alias=self.table_conf.get_layer_tgt_to_src_col_mapping(col, self.layer))
+            for col in cols
         ]
 
         sql_with_transforms = self.add_transformations(cols_with_alias, self.source)
         query_sql = select(*sql_with_transforms).from_(":tbl").where(self.filter)
-        with_select = sorted(self.table_conf.get_tgt_to_src_col_mapping(cols, self.layer))
+        if self.layer == "source":
+            with_select = sorted(cols)
+        else:
+            with_select = sorted(self.table_conf.get_tgt_to_src_col_mapping_list(cols))
 
-        return (
+        query = (
             with_clause.with_(alias="src", as_=query_sql)
             .select(*with_select)
             .from_("src")
             .join(expression="recon", join_type="inner", using=key_cols)
             .sql(dialect=self.source)
         )
+        logger.info(f"Sampling Query for {self.layer}: {query}")
+        return query
 
     @staticmethod
     def _get_with_clause(df: DataFrame) -> exp.Select:
         union_res = []
-        for row in df.take(SampleConfig.SAMPLE_ROWS):
-            row_select = [build_literal(this=value, alias=col, is_string=False) for col, value in zip(df.columns, row)]
+        for row in df.take(_SAMPLE_ROWS):
+            column_types = [(str(f.name).lower(), f.dataType) for f in df.schema.fields]
+            column_types_dict = dict(column_types)
+            row_select = [
+                build_literal(this=value, alias=col, is_string=_get_is_string(column_types_dict, col))
+                for col, value in zip(df.columns, row)
+            ]
             union_res.append(select(*row_select))
         union_statements = _union_concat(union_res, union_res[0], 0)
         return exp.Select().with_(alias='recon', as_=union_statements)
```

### Comparing `databricks_labs_remorph-0.1.7/databricks/labs/remorph/reconcile/query_builder/threshold_query.py` & `databricks_labs_remorph-0.2.0/databricks/labs/remorph/reconcile/query_builder/threshold_query.py`

 * *Files 19% similar despite different names*

```diff
@@ -1,13 +1,12 @@
 import logging
 
 from sqlglot import expressions as exp
 from sqlglot import select
 
-from databricks.labs.remorph.reconcile.constants import ThresholdMode
 from databricks.labs.remorph.reconcile.query_builder.base import QueryBuilder
 from databricks.labs.remorph.reconcile.query_builder.expression_generator import (
     anonymous,
     build_between,
     build_column,
     build_from_clause,
     build_if,
@@ -24,21 +23,21 @@
 
 
 class ThresholdQueryBuilder(QueryBuilder):
     # Comparison query
     def build_comparison_query(self) -> str:
         select_clause, where = self._generate_select_where_clause()
         from_clause, join_clause = self._generate_from_and_join_clause()
-        # for threshold comparison query the dialect is always Daabricks
+        # for threshold comparison query the dialect is always Databricks
         query = select(*select_clause).from_(from_clause).join(join_clause).where(where).sql(dialect=Databricks)
         logger.info(f"Threshold Comparison query: {query}")
         return query
 
-    def _generate_select_where_clause(self) -> tuple[list[exp.Alias], exp.Or]:
-        thresholds = self.table_conf.thresholds
+    def _generate_select_where_clause(self) -> tuple[list[exp.Expression], exp.Expression]:
+        thresholds = self.table_conf.thresholds if self.table_conf.thresholds else []
         select_clause = []
         where_clause = []
 
         # threshold columns
         for threshold in thresholds:
             column = threshold.column_name
             base = exp.Paren(
@@ -58,94 +57,106 @@
             select_clause.append(build_column(this=column, alias=f"{column}_source", table_name="source"))
         where = build_where_clause(where_clause)
 
         return select_clause, where
 
     @classmethod
     def _build_expression_alias_components(
-        cls, threshold: Thresholds, base: exp.Expression
-    ) -> tuple[list[exp.Alias], exp.Expression]:
+        cls,
+        threshold: Thresholds,
+        base: exp.Expression,
+    ) -> tuple[list[exp.Expression], exp.Expression]:
         select_clause = []
         column = threshold.column_name
         select_clause.append(
             build_column(this=column, alias=f"{column}_source", table_name="source").transform(coalesce)
         )
         select_clause.append(
             build_column(this=column, alias=f"{column}_databricks", table_name="databricks").transform(coalesce)
         )
         where_clause = exp.NEQ(this=base, expression=exp.Literal(this="0", is_string=False))
         return select_clause, where_clause
 
     def _build_expression_type(
-        self, threshold: Thresholds, base: exp.Expression
-    ) -> tuple[list[exp.Alias], exp.Expression]:
+        self,
+        threshold: Thresholds,
+        base: exp.Expression,
+    ) -> tuple[list[exp.Expression], exp.Expression]:
         column = threshold.column_name
         # default expressions
         select_clause, where_clause = self._build_expression_alias_components(threshold, base)
 
-        if threshold.get_type() in (ThresholdMode.NUMBER_ABSOLUTE.value, ThresholdMode.DATETIME.value):
-            if threshold.get_type() == ThresholdMode.DATETIME.value:
+        if threshold.get_type() in {"number_absolute", "datetime"}:
+            if threshold.get_type() == "datetime":
                 # unix_timestamp expression only if it is datetime
                 select_clause = [expression.transform(anonymous, "unix_timestamp({})") for expression in select_clause]
                 base = base.transform(anonymous, "unix_timestamp({})")
                 where_clause = exp.NEQ(this=base, expression=exp.Literal(this="0", is_string=False))
 
             # absolute threshold
             func = self._build_threshold_absolute_case
-        elif threshold.get_type() == ThresholdMode.NUMBER_PERCENTAGE.value:
+        elif threshold.get_type() == "number_percentage":
             # percentage threshold
             func = self._build_threshold_percentage_case
         else:
             error_message = f"Threshold type {threshold.get_type()} not supported for column {column}"
             logger.error(error_message)
             raise ValueError(error_message)
 
         select_clause.append(build_column(this=func(base=base, threshold=threshold), alias=f"{column}_match"))
 
         return select_clause, where_clause
 
     def _generate_from_and_join_clause(self) -> tuple[exp.From, exp.Join]:
         join_columns = sorted(self.table_conf.get_join_columns("source"))
-        source_view = f"{self.table_conf.source_name}_df_threshold_vw"
-        target_view = f"{self.table_conf.target_name}_df_threshold_vw"
+        source_view = f"source_{self.table_conf.source_name}_df_threshold_vw"
+        target_view = f"target_{self.table_conf.target_name}_df_threshold_vw"
 
         from_clause = build_from_clause(source_view, "source")
         join_clause = build_join_clause(
             table_name=target_view,
             source_table_alias="source",
             target_table_alias="databricks",
             join_columns=join_columns,
         )
 
         return from_clause, join_clause
 
     @classmethod
-    def _build_threshold_absolute_case(cls, base: exp.Expression, threshold: Thresholds) -> exp.Case:
+    def _build_threshold_absolute_case(
+        cls,
+        base: exp.Expression,
+        threshold: Thresholds,
+    ) -> exp.Case:
         eq_if = build_if(
             this=exp.EQ(this=base, expression=build_literal(this="0", is_string=False)),
-            true=exp.Identifier(this="Match", quoted=True),
+            true=exp.Literal(this="Match", is_string=True),
         )
 
         between_base = build_between(
             this=base,
             low=build_literal(threshold.lower_bound.replace("%", ""), is_string=False),
             high=build_literal(threshold.upper_bound.replace("%", ""), is_string=False),
         )
 
         between_if = build_if(
             this=between_base,
-            true=exp.Identifier(this="Warning", quoted=True),
+            true=exp.Literal(this="Warning", is_string=True),
         )
-        return exp.Case(ifs=[eq_if, between_if], default=exp.Identifier(this="Failed", quoted=True))
+        return exp.Case(ifs=[eq_if, between_if], default=exp.Literal(this="Failed", is_string=True))
 
     @classmethod
-    def _build_threshold_percentage_case(cls, base: exp.Expression, threshold: Thresholds) -> exp.Case:
+    def _build_threshold_percentage_case(
+        cls,
+        base: exp.Expression,
+        threshold: Thresholds,
+    ) -> exp.Case:
         eq_if = exp.If(
             this=exp.EQ(this=base, expression=build_literal(this="0", is_string=False)),
-            true=exp.Identifier(this="Match", quoted=True),
+            true=exp.Literal(this="Match", is_string=True),
         )
 
         denominator = build_if(
             this=exp.Or(
                 this=exp.EQ(
                     this=exp.Column(this=threshold.column_name, table="databricks"),
                     expression=exp.Literal(this='0', is_string=False),
@@ -168,10 +179,44 @@
             this=percentage,
             low=build_literal(threshold.lower_bound.replace("%", ""), is_string=False),
             high=build_literal(threshold.upper_bound.replace("%", ""), is_string=False),
         )
 
         between_if = build_if(
             this=between_base,
-            true=exp.Identifier(this="Warning", quoted=True),
+            true=exp.Literal(this="Warning", is_string=True),
         )
-        return exp.Case(ifs=[eq_if, between_if], default=exp.Identifier(this="Failed", quoted=True))
+        return exp.Case(ifs=[eq_if, between_if], default=exp.Literal(this="Failed", is_string=True))
+
+    def build_threshold_query(self) -> str:
+        """
+        This method builds a threshold query based on the configuration of the table and the columns involved.
+
+        The query is constructed by selecting the necessary columns (partition, join, and threshold columns)
+        from a specified table. Any transformations specified in the table configuration are applied to the
+        selected columns. The query also includes a WHERE clause based on the filter defined in the table configuration.
+
+        The resulting query is then converted to a SQL string using the dialect of the source database.
+
+        Returns:
+            str: The SQL string representation of the threshold query.
+        """
+        # key column expression
+        keys: list[str] = sorted(self.partition_column.union(self.join_columns))
+        keys_select_alias = [
+            build_column(this=col, alias=self.table_conf.get_layer_tgt_to_src_col_mapping(col, self.layer))
+            for col in keys
+        ]
+        keys_expr = self.add_transformations(keys_select_alias, self.source)
+
+        # threshold column expression
+        threshold_alias = [
+            build_column(this=col, alias=self.table_conf.get_layer_tgt_to_src_col_mapping(col, self.layer))
+            for col in sorted(self.threshold_columns)
+        ]
+        thresholds_expr = threshold_alias
+        if self.user_transformations:
+            thresholds_expr = self._apply_user_transformation(threshold_alias)
+
+        query = (select(*keys_expr + thresholds_expr).from_(":tbl").where(self.filter)).sql(dialect=self.source)
+        logger.info(f"Threshold Query for {self.layer}: {query}")
+        return query
```

### Comparing `databricks_labs_remorph-0.1.7/databricks/labs/remorph/snow/databricks.py` & `databricks_labs_remorph-0.2.0/databricks/labs/remorph/snow/databricks.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,17 +1,17 @@
 import logging
 import re
-from typing import ClassVar
 
 from sqlglot import expressions as exp
 from sqlglot.dialects import hive
-from sqlglot.dialects.databricks import Databricks
+from sqlglot.dialects import databricks as org_databricks
 from sqlglot.dialects.dialect import rename_func
 from sqlglot.errors import ParseError, UnsupportedError
 from sqlglot.helper import apply_index_offset, csv
+from sqlglot.dialects.dialect import if_sql
 
 from databricks.labs.remorph.snow import lca_utils, local_expression
 
 logger = logging.getLogger(__name__)
 
 VALID_DATABRICKS_TYPES = {
     "BIGINT",
@@ -83,15 +83,15 @@
     for expr in expression.expressions:
         column = expr.unalias() if isinstance(expr, exp.Alias) else expr
         if column.name == "index":
             return True
     return False
 
 
-def _lateral_view(self: Databricks.Generator, expression: exp.Lateral) -> str:
+def _lateral_view(self: org_databricks.Databricks.Generator, expression: exp.Lateral) -> str:
     this = expression.args['this']
     alias = expression.args['alias']
     alias_str = f" AS {alias.name}" if isinstance(alias, exp.TableAlias) else ""
     generator_function_str = self.sql(this)
     is_outer = False
 
     if isinstance(this, exp.Explode):
@@ -158,15 +158,15 @@
         func_expr = self.func(func, expression.this, expression.expression)
     else:
         func_expr = expression.this
 
     return f"CAST({func_expr} AS DECIMAL({precision}, {scale}))"
 
 
-def _to_boolean(self: Databricks.Generator, expression: local_expression.ToBoolean) -> str:
+def _to_boolean(self: org_databricks.Databricks.Generator, expression: local_expression.ToBoolean) -> str:
     this = self.sql(expression, "this")
     logger.debug(f"Converting {this} to Boolean")
     raise_error = self.sql(expression, "raise_error")
     raise_error_str = "RAISE_ERROR('Invalid parameter type for TO_BOOLEAN')" if bool(int(raise_error)) else "NULL"
     transformed = f"""
     CASE
        WHEN {this} IS NULL THEN NULL
@@ -185,55 +185,59 @@
                END
        ELSE {raise_error_str}
        END
     """
     return transformed
 
 
-def _is_integer(self: Databricks.Generator, expression: local_expression.IsInteger) -> str:
+def _is_integer(self: org_databricks.Databricks.Generator, expression: local_expression.IsInteger) -> str:
     this = self.sql(expression, "this")
     transformed = f"""
     CASE
        WHEN {this} IS NULL THEN NULL
        WHEN {this} RLIKE '^-?[0-9]+$' AND TRY_CAST({this} AS INT) IS NOT NULL THEN TRUE
        ELSE FALSE
        END
     """
     return transformed
 
 
-def _parse_json_extract_path_text(self: Databricks.Generator, expression: local_expression.JsonExtractPathText) -> str:
+def _parse_json_extract_path_text(
+    self: org_databricks.Databricks.Generator, expression: local_expression.JsonExtractPathText
+) -> str:
     this = self.sql(expression, "this")
     path_name = expression.args["path_name"]
     if path_name.is_string:
         path = f"{self.dialect.QUOTE_START}$.{expression.text('path_name')}{self.dialect.QUOTE_END}"
     else:
         path = f"CONCAT('$.', {self.sql(expression, 'path_name')})"
     return f"GET_JSON_OBJECT({this}, {path})"
 
 
-def _array_construct_compact(self: Databricks.Generator, expression: local_expression.ArrayConstructCompact) -> str:
+def _array_construct_compact(
+    self: org_databricks.Databricks.Generator, expression: local_expression.ArrayConstructCompact
+) -> str:
     exclude = "ARRAY(NULL)"
     array_expr = f"ARRAY({self.expressions(expression, flat=True)})"
     return f"ARRAY_EXCEPT({array_expr}, {exclude})"
 
 
-def _array_slice(self: Databricks.Generator, expression: local_expression.ArraySlice) -> str:
+def _array_slice(self: org_databricks.Databricks.Generator, expression: local_expression.ArraySlice) -> str:
     from_expr = self.sql(expression, "from")
     # In Databricks: array indices start at 1 in function `slice(array, start, length)`
-    from_expr = 1 if from_expr == "0" else from_expr
+    parsed_from_expr = 1 if from_expr == "0" else from_expr
 
     to_expr = self.sql(expression, "to")
     # Convert string expression to number and check if it is negative number
     if int(to_expr) < 0:
         err_message = "In Databricks: function `slice` length must be greater than or equal to 0"
         raise UnsupportedError(err_message)
 
     func = "SLICE"
-    func_expr = self.func(func, expression.this, exp.Literal.number(from_expr), expression.args["to"])
+    func_expr = self.func(func, expression.this, exp.Literal.number(parsed_from_expr), expression.args["to"])
     return func_expr
 
 
 def _parse_json(self, expr: exp.ParseJSON):
     """
     Converts `PARSE_JSON` function to `FROM_JSON` function.
     Schema is a mandatory argument for Databricks `FROM_JSON` function
@@ -271,26 +275,26 @@
         raise UnsupportedError(exception_msg)
 
     precision = PRECISION_CONST if not precision else precision
     scale = SCALE_CONST if not scale else scale
     return f"CAST({func_expr} AS DECIMAL({precision}, {scale}))"
 
 
-def _uuid(self: Databricks.Generator, expression: local_expression.UUID) -> str:
+def _uuid(self: org_databricks.Databricks.Generator, expression: local_expression.UUID) -> str:
     namespace = self.sql(expression, "this")
     name = self.sql(expression, "name")
 
     if namespace and name:
         logger.warning("UUID version 5 is not supported currently. Needs manual intervention.")
         return f"UUID({namespace}, {name})"
 
     return "UUID()"
 
 
-def _parse_date_trunc(self: Databricks.Generator, expression: local_expression.DateTrunc) -> str:
+def _parse_date_trunc(self: org_databricks.Databricks.Generator, expression: local_expression.DateTrunc) -> str:
     if not expression.args.get("unit"):
         error_message = f"Required keyword: 'unit' missing for {exp.DateTrunc}"
         raise UnsupportedError(error_message)
     return self.func("TRUNC", expression.this, expression.args.get("unit"))
 
 
 def _get_within_group_params(
@@ -324,38 +328,37 @@
             exp.Literal(this="sort_by", is_string=True),
             order_col,
         ],
     )
     return named_struct_func
 
 
-# pylint: disable=function-redefined
-class Databricks(Databricks):  #
+class Databricks(org_databricks.Databricks):  #
     # Instantiate Databricks Dialect
-    databricks = Databricks()
+    databricks = org_databricks.Databricks()
 
-    class Generator(databricks.Generator):
+    class Generator(org_databricks.Databricks.Generator):
         COLLATE_IS_FUNC = True
         # [TODO]: Variant needs to be transformed better, for now parsing to string was deemed as the choice.
-        TYPE_MAPPING: ClassVar[dict] = {
-            **Databricks.Generator.TYPE_MAPPING,
+        TYPE_MAPPING = {
+            **org_databricks.Databricks.Generator.TYPE_MAPPING,
             exp.DataType.Type.TINYINT: "TINYINT",
             exp.DataType.Type.SMALLINT: "SMALLINT",
             exp.DataType.Type.INT: "INT",
             exp.DataType.Type.BIGINT: "BIGINT",
             exp.DataType.Type.DATETIME: "TIMESTAMP",
             exp.DataType.Type.VARCHAR: "STRING",
             exp.DataType.Type.VARIANT: "STRING",
             exp.DataType.Type.FLOAT: "DOUBLE",
             exp.DataType.Type.OBJECT: "STRING",
             exp.DataType.Type.GEOGRAPHY: "STRING",
         }
 
-        TRANSFORMS: ClassVar[dict] = {
-            **Databricks.Generator.TRANSFORMS,
+        TRANSFORMS = {
+            **org_databricks.Databricks.Generator.TRANSFORMS,
             exp.Create: _format_create_sql,
             exp.DataType: _datatype_map,
             exp.CurrentTime: _curr_time(),
             exp.Lateral: _lateral_view,
             exp.FromBase64: rename_func("UNBASE64"),
             local_expression.Parameter: _parm_sfx,
             local_expression.ToBoolean: _to_boolean,
@@ -380,14 +383,15 @@
             local_expression.ToNumber: _to_number,
             local_expression.UUID: _uuid,
             local_expression.DateTrunc: _parse_date_trunc,
             exp.ApproxQuantile: rename_func("APPROX_PERCENTILE"),
             exp.TimestampTrunc: timestamptrunc_sql,
             exp.Mod: rename_func("MOD"),
             exp.NullSafeEQ: lambda self, e: self.binary(e, "<=>"),
+            exp.If: if_sql(false_value="NULL"),
         }
 
         def preprocess(self, expression: exp.Expression) -> exp.Expression:
             fixed_ast = expression.transform(lca_utils.unalias_lca_in_select, copy=False)
             return super().preprocess(fixed_ast)
 
         def join_sql(self, expression: exp.Join) -> str:
@@ -423,21 +427,21 @@
                 return f"\n {this_sql}"
             elif not op_sql:
                 return f", {this_sql}"
 
             op_sql = f"{op_sql} JOIN" if op_sql else "JOIN"
             return f"{self.seg(op_sql)} {this_sql}{on_sql}"
 
-        def arrayagg_sql(self, expr: exp.ArrayAgg) -> str:
-            sql = self.func("ARRAY_AGG", expr.this)
-            within_group = expr.parent if isinstance(expr.parent, exp.WithinGroup) else None
+        def arrayagg_sql(self, expression: exp.ArrayAgg) -> str:
+            sql = self.func("ARRAY_AGG", expression.this)
+            within_group = expression.parent if isinstance(expression.parent, exp.WithinGroup) else None
             if not within_group:
                 return sql
 
-            wg_params = _get_within_group_params(expr, within_group)
+            wg_params = _get_within_group_params(expression, within_group)
             if wg_params.agg_col == wg_params.order_col:
                 return f"SORT_ARRAY({sql}{'' if wg_params.is_order_asc else ', FALSE'})"
 
             named_struct_func = _create_named_struct_for_cmp(wg_params.agg_col, wg_params.order_col)
             array_sort = self.func(
                 "ARRAY_SORT",
                 self.func("ARRAY_AGG", named_struct_func),
@@ -555,31 +559,31 @@
             :return: Converted expression (SPLIT_PART) compatible with Databricks
             """
             expr_name = self.sql(expression.this)
             delimiter = self.sql(expression.expression)
             part_num = self.sql(expression.args["partNum"])
             return f"SPLIT_PART({expr_name}, {delimiter}, {part_num})"
 
-        def transaction_sql(self, expression: exp.Transaction) -> str:  # noqa: ARG002 pylint: disable=unused-argument
+        def transaction_sql(self, expression: exp.Transaction) -> str:
             """
             Skip begin command
             :param expression:
             :return: Empty string for unsupported operation
             """
             return ""
 
-        def rollback_sql(self, expression: exp.Rollback) -> str:  # noqa: ARG002 pylint: disable=unused-argument
+        def rollback_sql(self, expression: exp.Rollback) -> str:
             """
             Skip rollback command
             :param expression:
             :return: Empty string for unsupported operation
             """
             return ""
 
-        def commit_sql(self, expression: exp.Rollback) -> str:  # noqa: ARG002 pylint: disable=unused-argument
+        def commit_sql(self, expression: exp.Commit) -> str:
             """
             Skip commit command
             :param expression:
             :return: Empty string for unsupported operation
             """
             return ""
```

### Comparing `databricks_labs_remorph-0.1.7/databricks/labs/remorph/snow/lca_utils.py` & `databricks_labs_remorph-0.2.0/databricks/labs/remorph/snow/lca_utils.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,48 +1,49 @@
 import logging
+from collections.abc import Iterable
 
-from sqlglot import ErrorLevel, exp, parse
-from sqlglot.errors import ParseError, TokenError, UnsupportedError
+from sqlglot import expressions as exp
+from sqlglot import parse
+from sqlglot.dialects.dialect import DialectType
+from sqlglot.errors import ErrorLevel, ParseError, TokenError, UnsupportedError
 from sqlglot.expressions import Expression, Select
-from sqlglot.optimizer.scope import build_scope
+from sqlglot.optimizer.scope import Scope, build_scope
+
 
 from databricks.labs.remorph.helpers.morph_status import ValidationError
 from databricks.labs.remorph.snow.local_expression import AliasInfo
-from databricks.labs.remorph.snow.snowflake import Snow
 
 logger = logging.getLogger(__name__)
 
 
 def check_for_unsupported_lca(
-    dialect: str,
+    dialect: DialectType,
     sql: str,
     filename: str,
 ) -> ValidationError | None:
     """
     Check for presence of unsupported lateral column aliases in window expressions and where clauses
     :return: An error if found
     """
-    if dialect.upper() == "SNOWFLAKE":
-        dialect = Snow
 
     try:
-        parsed_expr = parse(sql, read=dialect, error_level=ErrorLevel.RAISE)
+        all_parsed_expressions: Iterable[Expression | None] = parse(sql, read=dialect, error_level=ErrorLevel.RAISE)
+        root_expressions: Iterable[Expression] = [pe for pe in all_parsed_expressions if pe is not None]
     except (ParseError, TokenError, UnsupportedError) as e:
         logger.warning(f"Error while preprocessing {filename}: {e}")
         return None
 
     aliases_in_where = set()
     aliases_in_window = set()
 
-    for expr in parsed_expr:
-        if expr:
-            for select in expr.find_all(exp.Select, bfs=False):
-                alias_info = _find_aliases_in_select(select)
-                aliases_in_where.update(_find_invalid_lca_in_where(select, alias_info))
-                aliases_in_window.update(_find_invalid_lca_in_window(select, alias_info))
+    for expr in root_expressions:
+        for select in expr.find_all(exp.Select, bfs=False):
+            alias_info = _find_aliases_in_select(select)
+            aliases_in_where.update(_find_invalid_lca_in_where(select, alias_info))
+            aliases_in_window.update(_find_invalid_lca_in_window(select, alias_info))
 
     if not (aliases_in_where or aliases_in_window):
         return None
 
     err_messages = [f"Unsupported operation found in file {filename}. Needs manual review of transpiled query."]
     if aliases_in_where:
         err_messages.append(f"Lateral column aliases `{', '.join(aliases_in_where)}` found in where clause.")
@@ -52,38 +53,44 @@
 
     return ValidationError(filename, " ".join(err_messages))
 
 
 def unalias_lca_in_select(expr: exp.Expression) -> exp.Expression:
     if not isinstance(expr, exp.Select):
         return expr
-    root_select = build_scope(expr)
+
+    root_select: Scope | None = build_scope(expr)
+    if not root_select:
+        return expr
+
     # We won't search inside nested selects, they will be visited separately
     nested_selects = {*root_select.derived_tables, *root_select.subqueries}
     alias_info = _find_aliases_in_select(expr)
-    where_ast: Expression = expr.args.get("where")
+    where_ast: Expression | None = expr.args.get("where")
     if where_ast:
         for column in where_ast.walk(prune=lambda n: n in nested_selects):
-            if (
-                isinstance(column, exp.Column)
-                and column.name in alias_info
-                and not alias_info[column.name].is_same_name_as_column
-            ):
-                column.replace(alias_info[column.name].expression)
+            _replace_aliases(column, alias_info)
     for window in _find_windows_in_select(expr):
         for column in window.walk():
-            if (
-                isinstance(column, exp.Column)
-                and column.name in alias_info
-                and not alias_info[column.name].is_same_name_as_column
-            ):
-                column.replace(alias_info[column.name].expression)
+            _replace_aliases(column, alias_info)
     return expr
 
 
+def _replace_aliases(column: Expression, alias_info: dict[str, AliasInfo]):
+    if (
+        isinstance(column, exp.Column)
+        and column.name in alias_info
+        and not alias_info[column.name].is_same_name_as_column
+    ):
+        unaliased_expr = alias_info[column.name].expression
+        column.replace(unaliased_expr)
+        for col in unaliased_expr.walk():
+            _replace_aliases(col, alias_info)
+
+
 def _find_windows_in_select(select: Select) -> list[exp.Window]:
     window_expressions = []
     for expr in select.expressions:
         window_expr = expr.find(exp.Window)
         if window_expr:
             window_expressions.append(window_expr)
     return window_expressions
@@ -95,24 +102,24 @@
         if isinstance(expr, exp.Alias):
             alias_name = expr.output_name
             is_same_name_as_column = False
             for column in expr.find_all(exp.Column):
                 if column.name == alias_name:
                     is_same_name_as_column = True
                     break
-            aliases[alias_name] = AliasInfo(alias_name, expr.unalias(), is_same_name_as_column)
+            aliases[alias_name] = AliasInfo(alias_name, expr.unalias().copy(), is_same_name_as_column)
     return aliases
 
 
 def _find_invalid_lca_in_where(
     select_expr: Select,
     aliases: dict[str, AliasInfo],
 ) -> set[str]:
     aliases_in_where = set()
-    where_ast: Expression = select_expr.args.get("where")
+    where_ast: Expression | None = select_expr.args.get("where")
     if where_ast:
         for column in where_ast.find_all(exp.Column):
             if column.name in aliases and not aliases[column.name].is_same_name_as_column:
                 aliases_in_where.add(column.name)
 
     return aliases_in_where
```

### Comparing `databricks_labs_remorph-0.1.7/databricks/labs/remorph/snow/snowflake.py` & `databricks_labs_remorph-0.2.0/databricks/labs/remorph/snow/snowflake.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,15 +1,14 @@
 import copy
 import logging
 import re
-from typing import ClassVar
 
-from sqlglot import exp
-from sqlglot.dialects.dialect import build_date_delta as parse_date_delta
-from sqlglot.dialects.snowflake import Snowflake, build_formatted_time
+from sqlglot import expressions as exp
+from sqlglot.dialects.dialect import build_date_delta as parse_date_delta, build_formatted_time
+from sqlglot.dialects.snowflake import Snowflake
 from sqlglot.errors import ParseError
 from sqlglot.helper import is_int, seq_get
 from sqlglot.optimizer.simplify import simplify_literals
 from sqlglot.parser import build_var_map as parse_var_map
 from sqlglot.tokens import Token, TokenType
 from sqlglot.trie import new_trie
 
@@ -215,26 +214,25 @@
     return local_expression.ToNumber(this=seq_get(args, 0), expression=seq_get(args, 1))
 
 
 class Snow(Snowflake):
     # Instantiate Snowflake Dialect
     snowflake = Snowflake()
 
-    class Tokenizer(snowflake.Tokenizer):
-        IDENTIFIERS: ClassVar[list[str]] = ['"']
+    class Tokenizer(Snowflake.Tokenizer):
 
-        COMMENTS: ClassVar[list[str]] = ["--", "//", ("/*", "*/")]
-        STRING_ESCAPES: ClassVar[list[str]] = ["\\", "'"]
+        COMMENTS = ["--", "//", ("/*", "*/")]
+        STRING_ESCAPES = ["\\", "'"]
 
-        CUSTOM_TOKEN_MAP: ClassVar[dict] = {
+        CUSTOM_TOKEN_MAP = {
             r"(?i)CREATE\s+OR\s+REPLACE\s+PROCEDURE": TokenType.PROCEDURE,
             r"(?i)var\s+\w+\s+=\s+\w+?": TokenType.VAR,
         }
 
-        KEYWORDS: ClassVar[dict] = {**Snowflake.Tokenizer.KEYWORDS}
+        KEYWORDS = {**Snowflake.Tokenizer.KEYWORDS}
         # DEC is not a reserved keyword in Snowflake it can be used as table alias
         KEYWORDS.pop("DEC")
 
         @classmethod
         def update_keywords(cls, new_key_word_dict):
             cls.KEYWORDS = new_key_word_dict | cls.KEYWORDS
 
@@ -296,31 +294,31 @@
             # Update Keyword Trie
             custom_trie = new_trie(self.match_strings_list(sql, self.CUSTOM_TOKEN_MAP))
             logger.debug(
                 f"The New Trie after adding the REF, VAR and IF ELSE blocks "
                 f"based on {self.CUSTOM_TOKEN_MAP}, is \n\n {custom_trie}"
             )
             self.update_keyword_trie(custom_trie)
-            logger.debug(f"Updated New Trie is {self.KEYWORD_TRIE}")
+            logger.debug(f"Updated New Trie is {custom_trie}")
             # Parent Code
             self.size = len(sql)
             try:
                 self._scan()
             except Exception as e:
                 start = self._current - 50
                 end = self._current + 50
                 start = start if start > 0 else 0
                 end = end if end < self.size else self.size - 1
                 context = self.sql[start:end]
                 msg = f"Error tokenizing '{context}'"
                 raise ParseError(msg) from e
             return self.tokens
 
-    class Parser(snowflake.Parser):
-        FUNCTIONS: ClassVar[dict] = {
+    class Parser(Snowflake.Parser):
+        FUNCTIONS = {
             **Snowflake.Parser.FUNCTIONS,
             "ARRAY_AGG": exp.ArrayAgg.from_arg_list,
             "STRTOK_TO_ARRAY": local_expression.Split.from_arg_list,
             "DATE_FROM_PARTS": local_expression.MakeDate.from_arg_list,
             "CONVERT_TIMEZONE": local_expression.ConvertTimeZone.from_arg_list,
             "TRY_TO_DATE": local_expression.TryToDate.from_arg_list,
             "STRTOK": local_expression.StrTok.from_arg_list,
@@ -365,44 +363,42 @@
             "SYSDATE": exp.CurrentTimestamp.from_arg_list,
             "TRUNC": lambda args: local_expression.DateTrunc(unit=seq_get(args, 1), this=seq_get(args, 0)),
             "APPROX_PERCENTILE": exp.ApproxQuantile.from_arg_list,
             "NTH_VALUE": local_expression.NthValue.from_arg_list,
             "MEDIAN": local_expression.Median.from_arg_list,
         }
 
-        FUNCTION_PARSERS: ClassVar[dict] = {
+        FUNCTION_PARSERS = {
             **Snowflake.Parser.FUNCTION_PARSERS,
             "LISTAGG": lambda self: self._parse_list_agg(),
         }
 
-        PLACEHOLDER_PARSERS: ClassVar[dict] = {
+        PLACEHOLDER_PARSERS = {
             **Snowflake.Parser.PLACEHOLDER_PARSERS,
             TokenType.PARAMETER: lambda self: self._parse_parameter(),
         }
 
-        FUNC_TOKENS: ClassVar[dict] = {*Snowflake.Parser.FUNC_TOKENS, TokenType.COLLATE}
+        FUNC_TOKENS = {*Snowflake.Parser.FUNC_TOKENS, TokenType.COLLATE}
 
-        COLUMN_OPERATORS: ClassVar[dict] = {
+        COLUMN_OPERATORS = {
             **Snowflake.Parser.COLUMN_OPERATORS,
             TokenType.COLON: lambda self, this, path: self._json_column_op(this, path),
         }
 
-        TIMESTAMPS: ClassVar[dict] = Snowflake.Parser.TIMESTAMPS.copy() - {TokenType.TIME}
+        TIMESTAMPS: set[TokenType] = Snowflake.Parser.TIMESTAMPS.copy() - {TokenType.TIME}
 
-        RANGE_PARSERS: ClassVar[dict] = {
+        RANGE_PARSERS = {
             **Snowflake.Parser.RANGE_PARSERS,
         }
 
-        ALTER_PARSERS: ClassVar[dict] = {**Snowflake.Parser.ALTER_PARSERS}
+        ALTER_PARSERS = {**Snowflake.Parser.ALTER_PARSERS}
 
         def _parse_list_agg(self) -> exp.GroupConcat:
             if self._match(TokenType.DISTINCT):
-                args: list[exp.Expression | None] = [
-                    self.expression(exp.Distinct, expressions=[self._parse_conjunction()])
-                ]
+                args: list[exp.Expression] = [self.expression(exp.Distinct, expressions=[self._parse_conjunction()])]
                 if self._match(TokenType.COMMA):
                     args.extend(self._parse_csv(self._parse_conjunction))
             else:
                 args = self._parse_csv(self._parse_conjunction)
 
             return self.expression(exp.GroupConcat, this=args[0], separator=seq_get(args, 1))
 
@@ -415,25 +411,25 @@
                 isinstance(this, exp.DataType)
                 and this.is_type("numeric", "decimal", "number", "integer", "int", "smallint", "bigint")
                 and not this.expressions
             ):
                 return exp.DataType.build("DECIMAL(38,0)")
             return this
 
-        def _parse_parameter(self) -> local_expression.Parameter:
+        def _parse_parameter(self):
             wrapped = self._match(TokenType.L_BRACE)
             this = self._parse_var() or self._parse_identifier() or self._parse_primary()
             self._match(TokenType.R_BRACE)
-            suffix = ""
+            suffix: exp.Expression | None = None
             if not self._match(TokenType.SPACE) or self._match(TokenType.DOT):
                 suffix = self._parse_var() or self._parse_identifier() or self._parse_primary()
 
             return self.expression(local_expression.Parameter, this=this, wrapped=wrapped, suffix=suffix)
 
-        def _get_table_alias(self) -> str | None:
+        def _get_table_alias(self) -> exp.TableAlias | None:
             """
             :returns the `table alias` by looping through all the tokens until it finds the `From` token.
             Example:
             * SELECT .... FROM persons p => returns `p`
             * SELECT
                  ....
               FROM
@@ -451,26 +447,26 @@
                     self_copy._advance()  # advance to next token
                     # break the loop when subquery is found after `FROM` For ex: `FROM (select * from another_table)`
                     # instead of table name, For ex: `FROM persons p`
                     if self_copy._match(TokenType.L_PAREN, advance=False):
                         break
                     self_copy._parse_table_parts()  # parse the table parts
                     table_alias = self_copy._parse_table_alias()  # get to table alias
-                    return str(table_alias)
+                    return table_alias
 
             return table_alias
 
         def _json_column_op(self, this, path):
             """
             Get the `table alias` using _get_table_alias() and it is used to check whether
             to remove `.value` from `<COL>.value`. We need to remove `.value` only if it refers
             to `Lateral View` alias.
             :return: the expression based on the alias.
             """
-            table_alias = self._get_table_alias()
+            table_alias = str(self._get_table_alias()) if self._get_table_alias() else None
             is_name_value = this.name.upper() == "VALUE"
             is_path_value = path.alias_or_name.upper() == "VALUE"
 
             if isinstance(this, exp.Column) and this.table:
                 col_table_alias = this.table.upper()
             elif isinstance(this, local_expression.Bracket) and isinstance(this.this, exp.Column) and this.this.table:
                 col_table_alias = this.this.table.upper()
```

### Comparing `databricks_labs_remorph-0.1.7/databricks/labs/remorph/snow/sql_transpiler.py` & `databricks_labs_remorph-0.2.0/databricks/labs/remorph/snow/sql_transpiler.py`

 * *Files 13% similar despite different names*

```diff
@@ -1,37 +1,39 @@
-from sqlglot import ErrorLevel, Expression, exp, parse, transpile
+from sqlglot import expressions as exp, parse, transpile
 from sqlglot.dialects.dialect import Dialect
-from sqlglot.errors import ParseError, TokenError, UnsupportedError
+from sqlglot.errors import ErrorLevel, ParseError, TokenError, UnsupportedError
+from sqlglot.expressions import Expression
 
+from databricks.labs.remorph.config import TranspilationResult
 from databricks.labs.remorph.helpers.file_utils import refactor_hexadecimal_chars
 from databricks.labs.remorph.helpers.morph_status import ParserError
 
 
 class SqlglotEngine:
     def __init__(self, read_dialect: Dialect):
         self.read_dialect = read_dialect
 
     def transpile(
         self, write_dialect: Dialect, sql: str, file_name: str, error_list: list[ParserError]
-    ) -> (list[str], list[ParserError]):
+    ) -> TranspilationResult:
         try:
             transpiled_sql = transpile(sql, read=self.read_dialect, write=write_dialect, pretty=True, error_level=None)
         except (ParseError, TokenError, UnsupportedError) as e:
             transpiled_sql = [""]
             error_list.append(ParserError(file_name, refactor_hexadecimal_chars(str(e))))
 
-        return transpiled_sql, error_list
+        return TranspilationResult(transpiled_sql, error_list)
 
-    def parse(self, sql: str, file_name: str) -> (list[Expression] | None, ParserError | None):
+    def parse(self, sql: str, file_name: str) -> tuple[list[Expression | None] | None, ParserError | None]:
         expression = None
         error = None
         try:
             expression = parse(sql, read=self.read_dialect, error_level=ErrorLevel.IMMEDIATE)
         except (ParseError, TokenError, UnsupportedError) as e:
-            error = ParserError(file_name, e)
+            error = ParserError(file_name, str(e))
 
         return expression, error
 
     def parse_sql_content(self, sql, file_name):
         parsed_expression, _ = self.parse(sql, file_name)
         if parsed_expression is not None:
             for expr in parsed_expression:
@@ -40,10 +42,11 @@
                     for create in expr.find_all(exp.Create, exp.Insert, exp.Merge, bfs=False):
                         child = self._find_root_tables(create)
 
                     for select in expr.find_all(exp.Select, exp.Join, exp.With, bfs=False):
                         yield self._find_root_tables(select), child
 
     @staticmethod
-    def _find_root_tables(expression) -> str:
+    def _find_root_tables(expression) -> str | None:
         for table in expression.find_all(exp.Table, bfs=False):
             return table.name
+        return None
```

### Comparing `databricks_labs_remorph-0.1.7/LICENSE` & `databricks_labs_remorph-0.2.0/LICENSE`

 * *Files identical despite different names*

### Comparing `databricks_labs_remorph-0.1.7/NOTICE` & `databricks_labs_remorph-0.2.0/NOTICE`

 * *Files identical despite different names*

### Comparing `databricks_labs_remorph-0.1.7/README.md` & `databricks_labs_remorph-0.2.0/README.md`

 * *Files identical despite different names*

### Comparing `databricks_labs_remorph-0.1.7/pyproject.toml` & `databricks_labs_remorph-0.2.0/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -12,15 +12,15 @@
   "Programming Language :: Python :: 3.11",
   "Programming Language :: Python :: Implementation :: CPython",
 ]
 dependencies = [
   "databricks-sdk>=0.18.0",
   "sqlglot==23.13.7",
   "databricks-labs-blueprint[yaml]>=0.2.3",
-  "databricks-labs-lsql>=0.2.3",
+  "databricks-labs-lsql>=0.4.3",
 ]
 
 [project.urls]
 Documentation = "https://github.com/databrickslabs/remorph"
 Issues = "https://github.com/databrickslabs/remorph/issues"
 Source = "https://github.com/databrickslabs/remorph"
 
@@ -45,42 +45,41 @@
   "pylint",
   "pylint-pytest==2.0.0a0",
   "coverage[toml]>=6.5",
   "pytest",
   "pytest-cov>=4.0.0,<5.0.0",
   "black>=23.1.0",
   "ruff>=0.0.243",
-  "isort>=2.5.0",
-  "databricks-connect"
+  "databricks-connect",
+  "types-pyYAML",
+  "types-pytz",
+  "databricks-labs-pylint~=0.4.0",
+  "mypy~=1.10.0",
 ]
 
 [tool.hatch.envs.default.scripts]
 test        = "pytest --cov src --cov-report=xml tests/unit"
 coverage    = "pytest --cov src tests/unit --cov-report=html"
 integration = "pytest --cov src tests/integration --durations 20"
-fmt         = ["isort .",
-               "black .",
+fmt         = ["black .",
                "ruff  check . --fix",
+               "mypy --disable-error-code 'annotation-unchecked' .",
                "pylint --output-format=colorized -j 0 src tests"]
 verify      = ["black --check .",
-               "isort . --check-only",
                "ruff check .",
+               "mypy --disable-error-code 'annotation-unchecked' .",
                "pylint --output-format=colorized -j 0 src tests"]
 
 [tool.hatch.envs.sqlglot-latest]
 detached = true
 python="3.10"
 dependencies = [
   "sqlglot",
 ]
 
-[tool.isort]
-skip_glob = ["notebooks/*.py"]
-profile = "black"
-known_first_party = ["databricks"]
 
 [tool.pytest.ini_options]
 addopts = "-s -p no:warnings -vv --cache-clear"
 cache_dir = ".venv/pytest-cache"
 
 [tool.black]
 target-version = ["py310"]
@@ -112,16 +111,14 @@
   "PLR2004",
   "UP038", # Use `X | Y` in `isinstance` call instead of `(X, Y)`
 ]
 extend-exclude = [
   "notebooks/*.py"
 ]
 
-[tool.ruff.lint.isort]
-known-first-party = ["databricks.labs.remorph"]
 
 [tool.ruff.lint.flake8-tidy-imports]
 ban-relative-imports = "all"
 
 [tool.ruff.lint.per-file-ignores]
 
 "tests/**/*" = [
@@ -650,15 +647,15 @@
 
 # Spelling dictionary name. No available dictionaries : You need to install both
 # the python package and the system dependency for enchant to work.
 # spelling-dict =
 
 # List of comma separated words that should be considered directives if they
 # appear at the beginning of a comment and should not be checked.
-spelling-ignore-comment-directives = "fmt: on,fmt: off,noqa:,noqa,nosec,isort:skip,mypy:,pragma:,# noinspection"
+spelling-ignore-comment-directives = "fmt: on,fmt: off,noqa:,noqa,nosec,mypy:,pragma:,# noinspection"
 
 # List of comma separated words that should not be checked.
 # spelling-ignore-words =
 
 # A path to a file that contains the private dictionary; one word per line.
 spelling-private-dict-file = ".pyenchant_pylint_custom_dict.txt"
```

### Comparing `databricks_labs_remorph-0.1.7/PKG-INFO` & `databricks_labs_remorph-0.2.0/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,24 +1,24 @@
 Metadata-Version: 2.3
 Name: databricks-labs-remorph
-Version: 0.1.7
+Version: 0.2.0
 Summary: SQL code converter and data reconcilation tool for accelerating data onboarding to Databricks from EDW, CDW and other ETL sources.
 Project-URL: Documentation, https://github.com/databrickslabs/remorph
 Project-URL: Issues, https://github.com/databrickslabs/remorph/issues
 Project-URL: Source, https://github.com/databrickslabs/remorph
 License-File: LICENSE
 License-File: NOTICE
 Keywords: Databricks
 Classifier: Development Status :: 3 - Alpha
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: Python :: Implementation :: CPython
 Requires-Python: >=3.10
 Requires-Dist: databricks-labs-blueprint[yaml]>=0.2.3
-Requires-Dist: databricks-labs-lsql>=0.2.3
+Requires-Dist: databricks-labs-lsql>=0.4.3
 Requires-Dist: databricks-sdk>=0.18.0
 Requires-Dist: sqlglot==23.13.7
 Description-Content-Type: text/markdown
 
 Databricks Labs Remorph
 ---
 ![Databricks Labs Remorph](docs/remorph-logo.svg)
```

