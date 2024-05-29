# Comparing `tmp/spark_expectations-2.0.0.tar.gz` & `tmp/spark_expectations-2.1.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "spark_expectations-2.0.0.tar", max compression
+gzip compressed data, was "spark_expectations-2.1.0.tar", max compression
```

## Comparing `spark_expectations-2.0.0.tar` & `spark_expectations-2.1.0.tar`

### file list

```diff
@@ -1,55 +1,55 @@
--rw-r--r--   0        0        0    11357 2024-05-13 20:26:46.507852 spark_expectations-2.0.0/LICENSE
--rw-r--r--   0        0        0     7558 2024-05-13 20:26:46.507852 spark_expectations-2.0.0/README.md
--rw-r--r--   0        0        0     1972 2024-05-13 20:27:41.516158 spark_expectations-2.0.0/pyproject.toml
--rw-r--r--   0        0        0      788 2024-05-13 20:26:46.563852 spark_expectations-2.0.0/spark_expectations/__init__.py
--rw-r--r--   0        0        0        0 2024-05-13 20:26:46.563852 spark_expectations-2.0.0/spark_expectations/config/__init__.py
--rw-r--r--   0        0        0     3466 2024-05-13 20:26:46.563852 spark_expectations-2.0.0/spark_expectations/config/user_config.py
--rw-r--r--   0        0        0     1477 2024-05-13 20:26:46.563852 spark_expectations-2.0.0/spark_expectations/core/__init__.py
--rw-r--r--   0        0        0    60501 2024-05-13 20:26:46.563852 spark_expectations-2.0.0/spark_expectations/core/context.py
--rw-r--r--   0        0        0     1629 2024-05-13 20:26:46.563852 spark_expectations-2.0.0/spark_expectations/core/exceptions.py
--rw-r--r--   0        0        0    32124 2024-05-13 20:26:46.563852 spark_expectations-2.0.0/spark_expectations/core/expectations.py
--rw-r--r--   0        0        0        0 2024-05-13 20:26:46.563852 spark_expectations-2.0.0/spark_expectations/examples/__init__.py
--rw-r--r--   0        0        0     8635 2024-05-13 20:26:46.563852 spark_expectations-2.0.0/spark_expectations/examples/base_setup.py
--rwxr-xr-x   0        0        0      870 2024-05-13 20:26:46.563852 spark_expectations-2.0.0/spark_expectations/examples/docker_scripts/Dockerfile
--rw-r--r--   0        0        0      966 2024-05-13 20:26:46.563852 spark_expectations-2.0.0/spark_expectations/examples/docker_scripts/create_kafka_topic.sh
--rw-r--r--   0        0        0     1034 2024-05-13 20:26:46.563852 spark_expectations-2.0.0/spark_expectations/examples/docker_scripts/delete_kafka_topic.sh
--rw-r--r--   0        0        0      919 2024-05-13 20:26:46.563852 spark_expectations-2.0.0/spark_expectations/examples/docker_scripts/docker_kafka_start_script.sh
--rw-r--r--   0        0        0      330 2024-05-13 20:26:46.563852 spark_expectations-2.0.0/spark_expectations/examples/docker_scripts/docker_kafka_stop_script.sh
--rwxr-xr-x   0        0        0      218 2024-05-13 20:26:46.563852 spark_expectations-2.0.0/spark_expectations/examples/docker_scripts/kafka_cluster_start.sh
--rwxr-xr-x   0        0        0      141 2024-05-13 20:26:46.563852 spark_expectations-2.0.0/spark_expectations/examples/docker_scripts/kafka_cluster_stop.sh
--rwxr-xr-x   0        0        0      433 2024-05-13 20:26:46.563852 spark_expectations-2.0.0/spark_expectations/examples/docker_scripts/start-kafka.sh
--rw-r--r--   0        0        0     1366 2024-05-13 20:26:46.563852 spark_expectations-2.0.0/spark_expectations/examples/read_example_dataset.py
--rw-r--r--   0        0        0   385487 2024-05-13 20:26:46.563852 spark_expectations-2.0.0/spark_expectations/examples/resources/customer.csv
--rw-r--r--   0        0        0      394 2024-05-13 20:26:46.563852 spark_expectations-2.0.0/spark_expectations/examples/resources/customer_source.csv
--rw-r--r--   0        0        0      474 2024-05-13 20:26:46.563852 spark_expectations-2.0.0/spark_expectations/examples/resources/customer_target.csv
--rw-r--r--   0        0        0   122408 2024-05-13 20:26:46.567852 spark_expectations-2.0.0/spark_expectations/examples/resources/employee.csv
--rw-r--r--   0        0        0   981149 2024-05-13 20:26:46.567852 spark_expectations-2.0.0/spark_expectations/examples/resources/order_1.csv
--rw-r--r--   0        0        0      585 2024-05-13 20:26:46.567852 spark_expectations-2.0.0/spark_expectations/examples/resources/order_s.csv
--rw-r--r--   0        0        0      486 2024-05-13 20:26:46.567852 spark_expectations-2.0.0/spark_expectations/examples/resources/order_t.csv
--rw-r--r--   0        0        0   145357 2024-05-13 20:26:46.571852 spark_expectations-2.0.0/spark_expectations/examples/resources/product.csv
--rw-r--r--   0        0        0  2288625 2024-05-13 20:26:46.579852 spark_expectations-2.0.0/spark_expectations/examples/resources/superstore.csv
--rw-r--r--   0        0        0     4529 2024-05-13 20:26:46.579852 spark_expectations-2.0.0/spark_expectations/examples/sample_dq_bigquery.py
--rw-r--r--   0        0        0     4799 2024-05-13 20:26:46.579852 spark_expectations-2.0.0/spark_expectations/examples/sample_dq_delta.py
--rw-r--r--   0        0        0     5154 2024-05-13 20:26:46.579852 spark_expectations-2.0.0/spark_expectations/examples/sample_dq_iceberg.py
--rw-r--r--   0        0        0     1473 2024-05-13 20:26:46.579852 spark_expectations-2.0.0/spark_expectations/notifications/__init__.py
--rw-r--r--   0        0        0        0 2024-05-13 20:26:46.579852 spark_expectations-2.0.0/spark_expectations/notifications/plugins/__init__.py
--rw-r--r--   0        0        0     1001 2024-05-13 20:26:46.579852 spark_expectations-2.0.0/spark_expectations/notifications/plugins/base_notification.py
--rw-r--r--   0        0        0     2242 2024-05-13 20:26:46.579852 spark_expectations-2.0.0/spark_expectations/notifications/plugins/email.py
--rw-r--r--   0        0        0     1907 2024-05-13 20:26:46.579852 spark_expectations-2.0.0/spark_expectations/notifications/plugins/slack.py
--rw-r--r--   0        0        0     2252 2024-05-13 20:26:46.579852 spark_expectations-2.0.0/spark_expectations/notifications/plugins/teams.py
--rw-r--r--   0        0        0        0 2024-05-13 20:26:46.579852 spark_expectations-2.0.0/spark_expectations/notifications/push/__init__.py
--rw-r--r--   0        0        0    11818 2024-05-13 20:26:46.579852 spark_expectations-2.0.0/spark_expectations/notifications/push/spark_expectations_notify.py
--rw-r--r--   0        0        0     4363 2024-05-13 20:26:46.579852 spark_expectations-2.0.0/spark_expectations/secrets/__init__.py
--rw-r--r--   0        0        0     1000 2024-05-13 20:26:46.579852 spark_expectations-2.0.0/spark_expectations/sinks/__init__.py
--rw-r--r--   0        0        0        0 2024-05-13 20:26:46.579852 spark_expectations-2.0.0/spark_expectations/sinks/plugins/__init__.py
--rw-r--r--   0        0        0      705 2024-05-13 20:26:46.579852 spark_expectations-2.0.0/spark_expectations/sinks/plugins/base_writer.py
--rw-r--r--   0        0        0     1616 2024-05-13 20:26:46.579852 spark_expectations-2.0.0/spark_expectations/sinks/plugins/kafka_writer.py
--rw-r--r--   0        0        0        0 2024-05-13 20:26:46.579852 spark_expectations-2.0.0/spark_expectations/sinks/utils/__init__.py
--rw-r--r--   0        0        0     1686 2024-05-13 20:26:46.579852 spark_expectations-2.0.0/spark_expectations/sinks/utils/collect_statistics.py
--rw-r--r--   0        0        0    40326 2024-05-13 20:26:46.579852 spark_expectations-2.0.0/spark_expectations/sinks/utils/writer.py
--rw-r--r--   0        0        0        0 2024-05-13 20:26:46.579852 spark_expectations-2.0.0/spark_expectations/utils/__init__.py
--rw-r--r--   0        0        0    28072 2024-05-13 20:26:46.579852 spark_expectations-2.0.0/spark_expectations/utils/actions.py
--rw-r--r--   0        0        0    17060 2024-05-13 20:26:46.579852 spark_expectations-2.0.0/spark_expectations/utils/reader.py
--rw-r--r--   0        0        0     6966 2024-05-13 20:26:46.579852 spark_expectations-2.0.0/spark_expectations/utils/regulate_flow.py
--rw-r--r--   0        0        0     1164 2024-05-13 20:26:46.579852 spark_expectations-2.0.0/spark_expectations/utils/udf.py
--rw-r--r--   0        0        0     8222 1970-01-01 00:00:00.000000 spark_expectations-2.0.0/PKG-INFO
+-rw-r--r--   0        0        0    11357 2024-05-29 17:29:49.542251 spark_expectations-2.1.0/LICENSE
+-rw-r--r--   0        0        0     7558 2024-05-29 17:29:49.542251 spark_expectations-2.1.0/README.md
+-rw-r--r--   0        0        0     2014 2024-05-29 17:30:46.002164 spark_expectations-2.1.0/pyproject.toml
+-rw-r--r--   0        0        0      788 2024-05-29 17:29:49.606251 spark_expectations-2.1.0/spark_expectations/__init__.py
+-rw-r--r--   0        0        0        0 2024-05-29 17:29:49.606251 spark_expectations-2.1.0/spark_expectations/config/__init__.py
+-rw-r--r--   0        0        0     3522 2024-05-29 17:29:49.606251 spark_expectations-2.1.0/spark_expectations/config/user_config.py
+-rw-r--r--   0        0        0     1477 2024-05-29 17:29:49.606251 spark_expectations-2.1.0/spark_expectations/core/__init__.py
+-rw-r--r--   0        0        0    61115 2024-05-29 17:29:49.606251 spark_expectations-2.1.0/spark_expectations/core/context.py
+-rw-r--r--   0        0        0     1629 2024-05-29 17:29:49.606251 spark_expectations-2.1.0/spark_expectations/core/exceptions.py
+-rw-r--r--   0        0        0    33085 2024-05-29 17:29:49.606251 spark_expectations-2.1.0/spark_expectations/core/expectations.py
+-rw-r--r--   0        0        0        0 2024-05-29 17:29:49.606251 spark_expectations-2.1.0/spark_expectations/examples/__init__.py
+-rw-r--r--   0        0        0     8626 2024-05-29 17:29:49.606251 spark_expectations-2.1.0/spark_expectations/examples/base_setup.py
+-rwxr-xr-x   0        0        0      870 2024-05-29 17:29:49.606251 spark_expectations-2.1.0/spark_expectations/examples/docker_scripts/Dockerfile
+-rw-r--r--   0        0        0      966 2024-05-29 17:29:49.606251 spark_expectations-2.1.0/spark_expectations/examples/docker_scripts/create_kafka_topic.sh
+-rw-r--r--   0        0        0     1034 2024-05-29 17:29:49.606251 spark_expectations-2.1.0/spark_expectations/examples/docker_scripts/delete_kafka_topic.sh
+-rw-r--r--   0        0        0      919 2024-05-29 17:29:49.606251 spark_expectations-2.1.0/spark_expectations/examples/docker_scripts/docker_kafka_start_script.sh
+-rw-r--r--   0        0        0      330 2024-05-29 17:29:49.606251 spark_expectations-2.1.0/spark_expectations/examples/docker_scripts/docker_kafka_stop_script.sh
+-rwxr-xr-x   0        0        0      218 2024-05-29 17:29:49.606251 spark_expectations-2.1.0/spark_expectations/examples/docker_scripts/kafka_cluster_start.sh
+-rwxr-xr-x   0        0        0      141 2024-05-29 17:29:49.606251 spark_expectations-2.1.0/spark_expectations/examples/docker_scripts/kafka_cluster_stop.sh
+-rwxr-xr-x   0        0        0      433 2024-05-29 17:29:49.606251 spark_expectations-2.1.0/spark_expectations/examples/docker_scripts/start-kafka.sh
+-rw-r--r--   0        0        0     1366 2024-05-29 17:29:49.606251 spark_expectations-2.1.0/spark_expectations/examples/read_example_dataset.py
+-rw-r--r--   0        0        0   385487 2024-05-29 17:29:49.606251 spark_expectations-2.1.0/spark_expectations/examples/resources/customer.csv
+-rw-r--r--   0        0        0      394 2024-05-29 17:29:49.606251 spark_expectations-2.1.0/spark_expectations/examples/resources/customer_source.csv
+-rw-r--r--   0        0        0      474 2024-05-29 17:29:49.606251 spark_expectations-2.1.0/spark_expectations/examples/resources/customer_target.csv
+-rw-r--r--   0        0        0   122408 2024-05-29 17:29:49.606251 spark_expectations-2.1.0/spark_expectations/examples/resources/employee.csv
+-rw-r--r--   0        0        0   981149 2024-05-29 17:29:49.610251 spark_expectations-2.1.0/spark_expectations/examples/resources/order_1.csv
+-rw-r--r--   0        0        0      585 2024-05-29 17:29:49.610251 spark_expectations-2.1.0/spark_expectations/examples/resources/order_s.csv
+-rw-r--r--   0        0        0      486 2024-05-29 17:29:49.610251 spark_expectations-2.1.0/spark_expectations/examples/resources/order_t.csv
+-rw-r--r--   0        0        0   145357 2024-05-29 17:29:49.610251 spark_expectations-2.1.0/spark_expectations/examples/resources/product.csv
+-rw-r--r--   0        0        0  2288625 2024-05-29 17:29:49.622251 spark_expectations-2.1.0/spark_expectations/examples/resources/superstore.csv
+-rw-r--r--   0        0        0     4693 2024-05-29 17:29:49.622251 spark_expectations-2.1.0/spark_expectations/examples/sample_dq_bigquery.py
+-rw-r--r--   0        0        0     4963 2024-05-29 17:29:49.622251 spark_expectations-2.1.0/spark_expectations/examples/sample_dq_delta.py
+-rw-r--r--   0        0        0     5318 2024-05-29 17:29:49.622251 spark_expectations-2.1.0/spark_expectations/examples/sample_dq_iceberg.py
+-rw-r--r--   0        0        0     1473 2024-05-29 17:29:49.622251 spark_expectations-2.1.0/spark_expectations/notifications/__init__.py
+-rw-r--r--   0        0        0        0 2024-05-29 17:29:49.622251 spark_expectations-2.1.0/spark_expectations/notifications/plugins/__init__.py
+-rw-r--r--   0        0        0     1001 2024-05-29 17:29:49.622251 spark_expectations-2.1.0/spark_expectations/notifications/plugins/base_notification.py
+-rw-r--r--   0        0        0     2242 2024-05-29 17:29:49.622251 spark_expectations-2.1.0/spark_expectations/notifications/plugins/email.py
+-rw-r--r--   0        0        0     1907 2024-05-29 17:29:49.622251 spark_expectations-2.1.0/spark_expectations/notifications/plugins/slack.py
+-rw-r--r--   0        0        0     2252 2024-05-29 17:29:49.622251 spark_expectations-2.1.0/spark_expectations/notifications/plugins/teams.py
+-rw-r--r--   0        0        0        0 2024-05-29 17:29:49.622251 spark_expectations-2.1.0/spark_expectations/notifications/push/__init__.py
+-rw-r--r--   0        0        0    11818 2024-05-29 17:29:49.622251 spark_expectations-2.1.0/spark_expectations/notifications/push/spark_expectations_notify.py
+-rw-r--r--   0        0        0     4363 2024-05-29 17:29:49.622251 spark_expectations-2.1.0/spark_expectations/secrets/__init__.py
+-rw-r--r--   0        0        0     1000 2024-05-29 17:29:49.622251 spark_expectations-2.1.0/spark_expectations/sinks/__init__.py
+-rw-r--r--   0        0        0        0 2024-05-29 17:29:49.622251 spark_expectations-2.1.0/spark_expectations/sinks/plugins/__init__.py
+-rw-r--r--   0        0        0      705 2024-05-29 17:29:49.622251 spark_expectations-2.1.0/spark_expectations/sinks/plugins/base_writer.py
+-rw-r--r--   0        0        0     1616 2024-05-29 17:29:49.622251 spark_expectations-2.1.0/spark_expectations/sinks/plugins/kafka_writer.py
+-rw-r--r--   0        0        0        0 2024-05-29 17:29:49.622251 spark_expectations-2.1.0/spark_expectations/sinks/utils/__init__.py
+-rw-r--r--   0        0        0     1686 2024-05-29 17:29:49.622251 spark_expectations-2.1.0/spark_expectations/sinks/utils/collect_statistics.py
+-rw-r--r--   0        0        0    44995 2024-05-29 17:29:49.622251 spark_expectations-2.1.0/spark_expectations/sinks/utils/writer.py
+-rw-r--r--   0        0        0        0 2024-05-29 17:29:49.622251 spark_expectations-2.1.0/spark_expectations/utils/__init__.py
+-rw-r--r--   0        0        0    29164 2024-05-29 17:29:49.622251 spark_expectations-2.1.0/spark_expectations/utils/actions.py
+-rw-r--r--   0        0        0    17067 2024-05-29 17:29:49.622251 spark_expectations-2.1.0/spark_expectations/utils/reader.py
+-rw-r--r--   0        0        0     6966 2024-05-29 17:29:49.622251 spark_expectations-2.1.0/spark_expectations/utils/regulate_flow.py
+-rw-r--r--   0        0        0     1164 2024-05-29 17:29:49.622251 spark_expectations-2.1.0/spark_expectations/utils/udf.py
+-rw-r--r--   0        0        0     8216 1970-01-01 00:00:00.000000 spark_expectations-2.1.0/PKG-INFO
```

### Comparing `spark_expectations-2.0.0/LICENSE` & `spark_expectations-2.1.0/LICENSE`

 * *Files identical despite different names*

### Comparing `spark_expectations-2.0.0/README.md` & `spark_expectations-2.1.0/README.md`

 * *Files identical despite different names*

### Comparing `spark_expectations-2.0.0/pyproject.toml` & `spark_expectations-2.1.0/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,19 +1,19 @@
 [tool.poetry]
 name = "spark-expectations"
-version = "2.0.0"
+version = "2.1.0"
 description = "This project helps us to run Data Quality Rules in flight while spark job is being run"
 authors = ["Ashok Singamaneni <ashok.singamaneni@nike.com>"]
 readme = "README.md"
 packages = [{ include = "spark_expectations" }]
 
 [tool.poetry.dependencies]
 python = "^3.8.9"
-pluggy = "1.0.0"
-pyspark = "^3.0.0"
+pluggy = ">=1"
+pyspark = "^3.0.0,<3.5"
 requests = "^2.28.1"
 
 [tool.poetry.group.dev.dependencies]
 black = "23.3.0"
 pytest = "7.3.1"
 pytest-mock = "3.10.0"
 coverage = "7.2.5"
@@ -25,18 +25,18 @@
 mkdocstrings = { extras = ["python"], version = "0.20.0" }
 mkdocs-autorefs = "0.4.1"
 mdx-include = ">=1.4.1,<2.0.0"
 mkdocs-markdownextradata-plugin = "0.2.5"
 mkdocs-click = "0.8.0"
 types-requests = "2.28.11.16"
 types-setuptools = "67.7.0.2"
-cerberus-python-client= "2.5.4"
+cerberus-python-client = "2.5.4"
 mike = "1.1.2"
 pre-commit = "3.3.1"
-botocore = "1.29.133" # This is just for fixing the dependency resolution version on cerberus-python-client
+botocore = "1.29.133"                                      # This is just for fixing the dependency resolution version on cerberus-python-client
 ipykernel = "^6.29.2"
 
 [tool.poetry-dynamic-versioning]
 enable = false
 vcs = "git"
 bump = true
 style = "semver"
@@ -72,8 +72,8 @@
 #[tool.poetry_bumpversion.file."spark_expectations/__init__.py"]
 #search = '__version__ = "{current_version}"'
 #replace = '__version__ = "{new_version}"'
 
 [tool.mypy]
 disallow_untyped_defs = true
 ignore_missing_imports = true
-follow_imports = "skip"
+follow_imports = "skip"
```

### Comparing `spark_expectations-2.0.0/spark_expectations/__init__.py` & `spark_expectations-2.1.0/spark_expectations/__init__.py`

 * *Files identical despite different names*

### Comparing `spark_expectations-2.0.0/spark_expectations/config/user_config.py` & `spark_expectations-2.1.0/spark_expectations/config/user_config.py`

 * *Files 2% similar despite different names*

```diff
@@ -60,14 +60,15 @@
     dbx_secret_app_name = "se.streaming.dbx.secret.app.name"
     dbx_secret_token = "se.streaming.dbx.secret.token"
     dbx_topic_name = "se.streaming.dbx.topic.name"
 
     # declare const user config variables for agg query dq detailed stats
     se_enable_agg_dq_detailed_result = "spark.expectations.agg.dq.detailed.stats"
     se_enable_query_dq_detailed_result = "spark.expectations.query.dq.detailed.stats"
+    se_job_metadata = "spark.expectations.job.metadata"
 
     querydq_output_custom_table_name = "spark.expectations.query.dq.custom.table_name"
 
     # declare const variable for agg query dq detailed stats
 
     se_agg_dq_expectation_regex_pattern = (
         r"(\(.+?\)|\w+\(.+?\))(\s*[<>!=]+\s*.+|\s*between\s*.+)$"
```

### Comparing `spark_expectations-2.0.0/spark_expectations/core/__init__.py` & `spark_expectations-2.1.0/spark_expectations/core/__init__.py`

 * *Files identical despite different names*

### Comparing `spark_expectations-2.0.0/spark_expectations/core/context.py` & `spark_expectations-2.1.0/spark_expectations/core/context.py`

 * *Files 1% similar despite different names*

```diff
@@ -71,14 +71,15 @@
             "dq-sparkexpectations-row-dq-results"
         )
 
         self._source_agg_dq_result: Optional[List[Dict[str, str]]] = None
         self._final_agg_dq_result: Optional[List[Dict[str, str]]] = None
         self._source_query_dq_result: Optional[List[Dict[str, str]]] = None
         self._final_query_dq_result: Optional[List[Dict[str, str]]] = None
+        self._job_metadata: Optional[str] = None
 
         self._source_agg_dq_detailed_stats: Optional[List[Tuple]] = None
         self._source_query_dq_detailed_stats: Optional[List[Tuple]] = None
 
         self._target_agg_dq_detailed_stats: Optional[List[Tuple]] = None
         self._target_query_dq_detailed_stats: Optional[List[Tuple]] = None
 
@@ -1907,7 +1908,30 @@
     def get_dq_rules_params(self) -> dict:
         """
         This function returns params which are mapping in dq rules
         Returns: _dq_rules_params(dict)
 
         """
         return self._dq_rules_params
+
+    def set_job_metadata(self, job_metadata: Optional[str] = None) -> None:
+        """
+        This function is used to set the job_metadata
+
+        Returns:
+            None
+
+        """
+        self._job_metadata = job_metadata
+
+    @property
+    def get_job_metadata(self) -> Optional[str]:
+        """
+        This function is used to get row data quality rule type name
+
+        Returns:
+             str: Returns _row_dq_rule_type_name"
+
+        """
+        if self._job_metadata is not None:
+            return str(self._job_metadata)
+        return None
```

### Comparing `spark_expectations-2.0.0/spark_expectations/core/exceptions.py` & `spark_expectations-2.1.0/spark_expectations/core/exceptions.py`

 * *Files identical despite different names*

### Comparing `spark_expectations-2.0.0/spark_expectations/core/expectations.py` & `spark_expectations-2.1.0/spark_expectations/core/expectations.py`

 * *Files 5% similar despite different names*

```diff
@@ -42,15 +42,23 @@
     target_and_error_table_writer: "WrappedDataFrameWriter"
     stats_table_writer: "WrappedDataFrameWriter"
     debugger: bool = False
     stats_streaming_options: Optional[Dict[str, Union[str, bool]]] = None
 
     def __post_init__(self) -> None:
         if isinstance(self.rules_df, DataFrame):
-            self.spark: SparkSession = self.rules_df.sparkSession
+            try:
+                self.spark: Optional[SparkSession] = self.rules_df.sparkSession
+            except AttributeError:
+                self.spark = SparkSession.getActiveSession()
+
+            if self.spark is None:
+                raise SparkExpectationsMiscException(
+                    "Spark session is not available, please initialize a spark session before calling SE"
+                )
         else:
             raise SparkExpectationsMiscException(
                 "Input rules_df is not of dataframe type"
             )
         self.actions: SparkExpectationsActions = SparkExpectationsActions()
         self._context: SparkExpectationsContext = SparkExpectationsContext(
             product_id=self.product_id, spark=self.spark
@@ -108,27 +116,30 @@
             Any: Returns a function which applied the expectations on dataset
         """
 
         def _except(func: Any) -> Any:
             # variable used for enabling notification at different level
 
             _default_notification_dict: Dict[
-                str, Union[str, int, bool, Dict[str, str]]
+                str, Union[str, int, bool, Dict[str, str], None]
             ] = {
                 user_config.se_notifications_on_start: False,
                 user_config.se_notifications_on_completion: False,
                 user_config.se_notifications_on_fail: True,
                 user_config.se_notifications_on_error_drop_exceeds_threshold_breach: False,
                 user_config.se_notifications_on_error_drop_threshold: 100,
                 user_config.se_enable_agg_dq_detailed_result: False,
                 user_config.se_enable_query_dq_detailed_result: False,
+                user_config.se_job_metadata: None,
                 user_config.querydq_output_custom_table_name: f"{self.stats_table}_querydq_output",
             }
 
-            _notification_dict: Dict[str, Union[str, int, bool, Dict[str, str]]] = (
+            _notification_dict: Dict[
+                str, Union[str, int, bool, Dict[str, str], None]
+            ] = (
                 {**_default_notification_dict, **user_conf}
                 if user_conf
                 else _default_notification_dict
             )
             _default_stats_streaming_dict: Dict[str, Union[bool, str]] = {
                 user_config.se_enable_streaming: True,
                 user_config.secret_type: "databricks",
@@ -258,14 +269,16 @@
                         user_config.se_notifications_on_error_drop_exceeds_threshold_breach
                     ],
                     bool,
                 )
                 else False
             )
 
+            _job_metadata: str = user_config.se_job_metadata
+
             notifications_on_error_drop_threshold = _notification_dict.get(
                 user_config.se_notifications_on_error_drop_threshold, 100
             )
             _error_drop_threshold: int = (
                 notifications_on_error_drop_threshold
                 if isinstance(notifications_on_error_drop_threshold, int)
                 else 100
@@ -276,26 +289,28 @@
             self._context.set_notification_on_completion(_notification_on_completion)
             self._context.set_notification_on_fail(_notification_on_fail)
 
             self._context.set_se_streaming_stats_dict(_se_stats_streaming_dict)
             self._context.set_dq_expectations(expectations)
             self._context.set_rules_execution_settings_config(rules_execution_settings)
             self._context.set_querydq_secondary_queries(dq_queries_dict)
+            self._context.set_job_metadata(_job_metadata)
 
             @self._notification.send_notification_decorator
             @self._statistics_decorator.collect_stats_decorator
             @functools.wraps(func)
             def wrapper(*args: tuple, **kwargs: dict) -> DataFrame:
                 try:
                     _log.info("The function dataframe is getting created")
                     # _df: DataFrame = func(*args, **kwargs)
                     _df: DataFrame = func(*args, **kwargs)
                     table_name: str = self._context.get_table_name
 
                     _input_count = _df.count()
+                    _log.info("data frame input record count: %s", _input_count)
                     _output_count: int = 0
                     _error_count: int = 0
                     _source_dq_df: Optional[DataFrame] = None
                     _source_query_dq_df: Optional[DataFrame] = None
                     _row_dq_df: DataFrame = _df
                     _final_dq_df: Optional[DataFrame] = None
                     _final_query_dq_df: Optional[DataFrame] = None
@@ -329,29 +344,36 @@
                     self._context._source_query_dq_end_time = None
                     self._context._final_query_dq_end_time = None
                     self._context._row_dq_end_time = None
 
                     self._context.set_input_count(_input_count)
                     self._context.set_error_drop_threshold(_error_drop_threshold)
 
+                    _log.info(
+                        "Spark Expectations run id for this run: %s",
+                        self._context.get_run_id,
+                    )
+
                     if isinstance(_df, DataFrame):
                         _log.info("The function dataframe is created")
                         self._context.set_table_name(table_name)
                         if write_to_temp_table:
                             _log.info("Dropping to temp table started")
-                            self.spark.sql(f"drop table if exists {table_name}_temp")
+                            self.spark.sql(f"drop table if exists {table_name}_temp")  # type: ignore
                             _log.info("Dropping to temp table completed")
                             _log.info("Writing to temp table started")
+                            source_columns = _df.columns
                             self._writer.save_df_as_table(
                                 _df,
                                 f"{table_name}_temp",
                                 self._context.get_target_and_error_table_writer_config,
                             )
                             _log.info("Read from temp table started")
-                            _df = self.spark.sql(f"select * from {table_name}_temp")
+                            _df = self.spark.sql(f"select * from {table_name}_temp")  # type: ignore
+                            _df = _df.select(source_columns)
                             _log.info("Read from temp table completed")
 
                         func_process = self._process.execute_dq_process(
                             _context=self._context,
                             _actions=self.actions,
                             _writer=self._writer,
                             _notification=self._notification,
@@ -540,15 +562,15 @@
                             _log.info("Writing into the final table ended")
 
                     else:
                         raise SparkExpectationsDataframeNotReturnedException(
                             "error occurred while processing spark "
                             "expectations due to given dataframe is not type of dataframe"
                         )
-                    self.spark.catalog.clearCache()
+                    # self.spark.catalog.clearCache()
 
                     return _row_dq_df
 
                 except Exception as e:
                     raise SparkExpectationsMiscException(
                         f"error occurred while processing spark expectations {e}"
                     )
```

### Comparing `spark_expectations-2.0.0/spark_expectations/examples/base_setup.py` & `spark_expectations-2.1.0/spark_expectations/examples/base_setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -21,15 +21,15 @@
     error_drop_threshold INT ,
     query_dq_delimiter STRING,
     enable_querydq_custom_output BOOLEAN
     )
 """
 
 
-RULES_DATA = """ 
+RULES_DATA = """
 
      ("your_product", "dq_spark_dev.customer_order", "row_dq", "sales_greater_than_zero", "sales", "sales > 2", "ignore", "accuracy", "sales value should be greater than zero", false, true, true, false, 0,null, null)
     ,("your_product", "dq_spark_{env}.customer_order", "row_dq", "discount_threshold", "discount", "discount*100 < 60","drop", "validity", "discount should be less than 40", true, true, true, false, 0,null, null)
     ,("your_product", "dq_spark_{env}.customer_order", "row_dq", "ship_mode_in_set", "ship_mode", "lower(trim(ship_mode)) in('second class', 'standard class', 'standard class')", "drop", "validity", "ship_mode mode belongs in the sets", true, true, true, false, 0,null, null)
     ,("your_product", "dq_spark_{env}.customer_order", "row_dq", "profit_threshold", "profit", "profit>0", "ignore", "validity", "profit threshold should be greater tahn 0", false, true, false, true, 0,null, null)
     ,("your_product", "dq_spark_dev.customer_order", "agg_dq", "sum_of_sales_range type 1", "sales", "sum(sales)>99 and sum(sales)<99999", "ignore", "validity", "regex format validation for quantity",  true, true, true, false, 0, null, true)
     ,("your_product", "dq_spark_dev.customer_order", "agg_dq", "sum_of_sales_range type 2", "sales", "sum(sales) between 100 and 10000 ", "ignore", "validity", "regex format validation for quantity", true, true, true, false, 0, null, true)
@@ -37,16 +37,16 @@
     ,("your_product", "dq_spark_dev.customer_order", "agg_dq", "sum_of_quantity", "quantity", "sum(quantity)>10000", "ignore", "validity", "regex format validation for quantity", true, true, true, false, 0,null, null)
     ,("your_product", "dq_spark_dev.customer_order", "query_dq", "product_missing_count_threshold", "*", "((select count(*) from ({source_f1}) a) - (select count(*) from ({target_f1}) b) ) < 3@source_f1@select distinct product_id,order_id from order_source@target_f1@select distinct product_id,order_id from order_target", "ignore", "validity", "row count threshold", true, true, true, false, 0,null, true)
     ,("your_product", "dq_spark_dev.customer_order", "query_dq", "customer_missing_count_threshold","*", "((select count(*) from ({source_f1}) a join ({source_f2}) b on a.customer_id = b.customer_id) - (select count(*) from ({target_f1}) a join ({target_f2}) b on a.customer_id = b.customer_id)) > ({target_f3})@source_f1@select customer_id, count(*) from customer_source group by customer_id@source_f2@select customer_id, count(*) from order_source group by customer_id@target_f1@select customer_id, count(*) from customer_target group by customer_id@target_f2@select customer_id, count(*) from order_target group by customer_id@target_f3@select count(*) from order_source", "ignore", "validity", "customer count threshold", true, true, true, false, 0,null, true)
     ,("your_product", "dq_spark_dev.customer_order", "query_dq", "order_count_validity", "*", "({source_f1}) > 10@source_f1@select count(*) from order_source", "ignore", "validity", "row count threshold", true, true, true, false, 0, "@", true)
     ,("your_product", "dq_spark_dev.customer_order", "query_dq", "order_count_validity_check", "*", "(select count(*) from order_source) > 10", "ignore", "validity", "row count threshold", true, true, true, false, 0, null, true)
     ,("your_product", "dq_spark_{env}.customer_order", "query_dq", "product_category", "*", "(select count(distinct category) from {table}) < 5", "ignore", "validity", "distinct product category", true, true, true, false, 0,null, true)
     ,("your_product", "dq_spark_{env}.customer_order", "agg_dq", "distinct_of_ship_mode", "ship_mode", "count(distinct ship_mode) <= 3", "ignore", "validity", "regex format validation for quantity", true, true, true, false, 0,null, null)
-    
-    
+
+
     """
 
 
 def set_up_kafka() -> None:
     print("create or run if exist docker container")
     os.system(f"sh {CURRENT_DIR}/docker_scripts/docker_kafka_start_script.sh")
```

### Comparing `spark_expectations-2.0.0/spark_expectations/examples/docker_scripts/Dockerfile` & `spark_expectations-2.1.0/spark_expectations/examples/docker_scripts/Dockerfile`

 * *Files identical despite different names*

### Comparing `spark_expectations-2.0.0/spark_expectations/examples/docker_scripts/create_kafka_topic.sh` & `spark_expectations-2.1.0/spark_expectations/examples/docker_scripts/create_kafka_topic.sh`

 * *Files identical despite different names*

### Comparing `spark_expectations-2.0.0/spark_expectations/examples/docker_scripts/delete_kafka_topic.sh` & `spark_expectations-2.1.0/spark_expectations/examples/docker_scripts/delete_kafka_topic.sh`

 * *Files identical despite different names*

### Comparing `spark_expectations-2.0.0/spark_expectations/examples/docker_scripts/docker_kafka_start_script.sh` & `spark_expectations-2.1.0/spark_expectations/examples/docker_scripts/docker_kafka_start_script.sh`

 * *Files identical despite different names*

### Comparing `spark_expectations-2.0.0/spark_expectations/examples/read_example_dataset.py` & `spark_expectations-2.1.0/spark_expectations/examples/read_example_dataset.py`

 * *Files identical despite different names*

### Comparing `spark_expectations-2.0.0/spark_expectations/examples/resources/customer.csv` & `spark_expectations-2.1.0/spark_expectations/examples/resources/customer.csv`

 * *Files identical despite different names*

### Comparing `spark_expectations-2.0.0/spark_expectations/examples/resources/employee.csv` & `spark_expectations-2.1.0/spark_expectations/examples/resources/employee.csv`

 * *Files identical despite different names*

### Comparing `spark_expectations-2.0.0/spark_expectations/examples/resources/order_1.csv` & `spark_expectations-2.1.0/spark_expectations/examples/resources/order_1.csv`

 * *Files identical despite different names*

### Comparing `spark_expectations-2.0.0/spark_expectations/examples/resources/order_s.csv` & `spark_expectations-2.1.0/spark_expectations/examples/resources/order_s.csv`

 * *Files identical despite different names*

### Comparing `spark_expectations-2.0.0/spark_expectations/examples/resources/product.csv` & `spark_expectations-2.1.0/spark_expectations/examples/resources/product.csv`

 * *Files identical despite different names*

### Comparing `spark_expectations-2.0.0/spark_expectations/examples/resources/superstore.csv` & `spark_expectations-2.1.0/spark_expectations/examples/resources/superstore.csv`

 * *Files identical despite different names*

### Comparing `spark_expectations-2.0.0/spark_expectations/examples/sample_dq_bigquery.py` & `spark_expectations-2.1.0/spark_expectations/examples/sample_dq_bigquery.py`

 * *Files 4% similar despite different names*

```diff
@@ -15,14 +15,20 @@
 writer = (
     WrappedDataFrameWriter()
     .mode("overwrite")
     .format("bigquery")
     .option("createDisposition", "CREATE_IF_NEEDED")
     .option("writeMethod", "direct")
 )
+dic_job_info = {
+    "job": "job_name",
+    "Region": "NA",
+    "Snapshot": "2024-04-15",
+}
+job_info = str(dic_job_info)
 
 # if wanted to use indirect method use below setting and spark session
 # writer = WrappedDataFrameWriter().mode("overwrite").format("bigquery").\
 #     option("createDisposition", "CREATE_IF_NEEDED")\
 #     .option("writeMethod", "indirect")\
 #     .option("intermediateFormat", "AVRO")\
 #     .option("temporaryGcsBucket", "<temporaryGCSBucket>")
@@ -59,14 +65,15 @@
     user_config.se_enable_query_dq_detailed_result: True,
     user_config.se_enable_agg_dq_detailed_result: True,
     user_config.se_enable_error_table: True,
     user_config.se_dq_rules_params: {
         "env": "local",
         "table": "product",
     },
+    user_config.se_job_metadata: job_info,
 }
 
 
 @se.with_expectations(
     target_table="<project_id>.<dataset_id>.<target_table_name>",
     write_to_table=True,
     user_conf=user_conf,
```

### Comparing `spark_expectations-2.0.0/spark_expectations/examples/sample_dq_delta.py` & `spark_expectations-2.1.0/spark_expectations/examples/sample_dq_delta.py`

 * *Files 3% similar despite different names*

```diff
@@ -10,14 +10,20 @@
 )
 from spark_expectations.config.user_config import Constants as user_config
 
 
 writer = WrappedDataFrameWriter().mode("append").format("delta")
 
 spark = set_up_delta()
+dic_job_info = {
+    "job": "job_name",
+    "Region": "NA",
+    "Snapshot": "2024-04-15",
+}
+job_info = str(dic_job_info)
 
 se: SparkExpectations = SparkExpectations(
     product_id="your_product",
     rules_df=spark.table("dq_spark_dev.dq_rules"),
     stats_table="dq_spark_dev.dq_stats",
     stats_table_writer=writer,
     target_and_error_table_writer=writer,
@@ -43,14 +49,15 @@
     user_config.se_enable_agg_dq_detailed_result: True,
     # user_config.querydq_output_custom_table_name: "dq_spark_local.dq_stats_detailed_outputt",
     user_config.se_enable_error_table: True,
     user_config.se_dq_rules_params: {
         "env": "dev",
         "table": "product",
     },
+    user_config.se_job_metadata: job_info,
 }
 
 
 @se.with_expectations(
     target_table="dq_spark_dev.customer_order",
     write_to_table=True,
     user_conf=user_conf,
```

### Comparing `spark_expectations-2.0.0/spark_expectations/examples/sample_dq_iceberg.py` & `spark_expectations-2.1.0/spark_expectations/examples/sample_dq_iceberg.py`

 * *Files 2% similar despite different names*

```diff
@@ -7,14 +7,20 @@
 from spark_expectations.core.expectations import (
     SparkExpectations,
     WrappedDataFrameWriter,
 )
 from spark_expectations.config.user_config import Constants as user_config
 
 writer = WrappedDataFrameWriter().mode("append").format("iceberg")
+dic_job_info = {
+    "job": "job_name",
+    "Region": "NA",
+    "Snapshot": "2024-04-15",
+}
+job_info = str(dic_job_info)
 
 spark = set_up_iceberg()
 
 print(spark.sparkContext.getConf().getAll())
 se: SparkExpectations = SparkExpectations(
     product_id="your_product",
     rules_df=spark.sql("select * from dq_spark_local.dq_rules"),
@@ -44,14 +50,15 @@
     user_config.se_enable_error_table: True,
     user_config.enable_query_dq_detailed_result: True,
     user_config.enable_agg_dq_detailed_result: True,
     user_config.se_dq_rules_params: {
         "env": "local",
         "table": "product",
     },
+    user_config.se_job_metadata: job_info,
 }
 
 
 @se.with_expectations(
     target_table="dq_spark_local.customer_order",
     write_to_table=True,
     user_conf=user_conf,
```

### Comparing `spark_expectations-2.0.0/spark_expectations/notifications/__init__.py` & `spark_expectations-2.1.0/spark_expectations/notifications/__init__.py`

 * *Files identical despite different names*

### Comparing `spark_expectations-2.0.0/spark_expectations/notifications/plugins/base_notification.py` & `spark_expectations-2.1.0/spark_expectations/notifications/plugins/base_notification.py`

 * *Files identical despite different names*

### Comparing `spark_expectations-2.0.0/spark_expectations/notifications/plugins/email.py` & `spark_expectations-2.1.0/spark_expectations/notifications/plugins/email.py`

 * *Files identical despite different names*

### Comparing `spark_expectations-2.0.0/spark_expectations/notifications/plugins/slack.py` & `spark_expectations-2.1.0/spark_expectations/notifications/plugins/slack.py`

 * *Files identical despite different names*

### Comparing `spark_expectations-2.0.0/spark_expectations/notifications/plugins/teams.py` & `spark_expectations-2.1.0/spark_expectations/notifications/plugins/teams.py`

 * *Files identical despite different names*

### Comparing `spark_expectations-2.0.0/spark_expectations/notifications/push/spark_expectations_notify.py` & `spark_expectations-2.1.0/spark_expectations/notifications/push/spark_expectations_notify.py`

 * *Files identical despite different names*

### Comparing `spark_expectations-2.0.0/spark_expectations/secrets/__init__.py` & `spark_expectations-2.1.0/spark_expectations/secrets/__init__.py`

 * *Files identical despite different names*

### Comparing `spark_expectations-2.0.0/spark_expectations/sinks/__init__.py` & `spark_expectations-2.1.0/spark_expectations/sinks/__init__.py`

 * *Files identical despite different names*

### Comparing `spark_expectations-2.0.0/spark_expectations/sinks/plugins/base_writer.py` & `spark_expectations-2.1.0/spark_expectations/sinks/plugins/base_writer.py`

 * *Files identical despite different names*

### Comparing `spark_expectations-2.0.0/spark_expectations/sinks/plugins/kafka_writer.py` & `spark_expectations-2.1.0/spark_expectations/sinks/plugins/kafka_writer.py`

 * *Files identical despite different names*

### Comparing `spark_expectations-2.0.0/spark_expectations/sinks/utils/collect_statistics.py` & `spark_expectations-2.1.0/spark_expectations/sinks/utils/collect_statistics.py`

 * *Files identical despite different names*

### Comparing `spark_expectations-2.0.0/spark_expectations/sinks/utils/writer.py` & `spark_expectations-2.1.0/spark_expectations/sinks/utils/writer.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,24 +1,26 @@
 from dataclasses import dataclass
 from typing import Dict, Optional, Tuple, List
-from datetime import datetime
+from datetime import datetime, timezone
 from pyspark.sql import DataFrame
 from pyspark.sql.functions import (
     lit,
     expr,
     when,
     array,
     to_timestamp,
     round as sql_round,
     create_map,
     explode,
     to_json,
     col,
     split,
     current_date,
+    monotonically_increasing_id,
+    coalesce,
 )
 from pyspark.sql.types import StructType
 from spark_expectations import _log
 from spark_expectations.core.exceptions import (
     SparkExpectationsUserInputOrConfigInvalidException,
     SparkExpectationsMiscException,
 )
@@ -121,15 +123,32 @@
             raise SparkExpectationsUserInputOrConfigInvalidException(
                 f"error occurred while writing data in to the table - {table_name}: {e}"
             )
 
     def get_row_dq_detailed_stats(
         self,
     ) -> List[
-        Tuple[str, str, str, str, str, str, str, str, str, None, None, int, str, int]
+        Tuple[
+            str,
+            str,
+            str,
+            str,
+            str,
+            str,
+            str,
+            str,
+            str,
+            None,
+            None,
+            int,
+            str,
+            int,
+            str,
+            str,
+        ]
     ]:
         """
         This function writes the detailed stats for row dq into the detailed stats table
 
         Args:
             df: Provide the dataframe which need to be written as a table
             rule_type: Provide the rule type for which the detailed stats need to be written
@@ -141,52 +160,87 @@
         try:
             _run_id = self._context.get_run_id
             _product_id = self._context.product_id
             _table_name = self._context.get_table_name
             _input_count = self._context.get_input_count
 
             _row_dq_result = []
-            _rowdq_rule_dict = {}
+
+            _rowdq_expectations = self._context.get_dq_expectations
+            _row_dq_expectations = _rowdq_expectations["row_dq_rules"]
+
             if (
                 self._context.get_summarized_row_dq_res is not None
                 and len(self._context.get_summarized_row_dq_res) > 0
             ):
-                _rowdq_expectations = self._context.get_dq_expectations
-                for _rowdq_rule in _rowdq_expectations["row_dq_rules"]:
-                    _rowdq_rule_dict[_rowdq_rule["rule"]] = (
-                        _rowdq_rule["expectation"]
-                        + "|"
-                        + _rowdq_rule["tag"]
-                        + "|"
-                        + _rowdq_rule["description"]
-                    )
+                _row_dq_res = self._context.get_summarized_row_dq_res
+                _dq_res = {d["rule"]: d["failed_row_count"] for d in _row_dq_res}
 
-                for _dq_res in self._context.get_summarized_row_dq_res:
-                    _rowdq_rules = str(_rowdq_rule_dict[_dq_res["rule"]]).split("|")
-                    _rule_expectations = _rowdq_rules[0]
-                    _rule_tag = _rowdq_rules[1]
-                    _rule_desc = _rowdq_rules[2]
-                    _row_dq_result.append(
-                        (
-                            _run_id,
-                            _product_id,
-                            _table_name,
-                            _dq_res["rule_type"],
-                            _dq_res["rule"],
-                            _rule_expectations,
-                            _rule_tag,
-                            _rule_desc,
-                            "pass" if int(_dq_res["failed_row_count"]) == 0 else "fail",
-                            None,
-                            None,
-                            (_input_count - int(_dq_res["failed_row_count"])),
-                            _dq_res["failed_row_count"],
-                            _input_count,
+                for _rowdq_rule in _row_dq_expectations:
+                    if _rowdq_rule["rule"] in _dq_res:
+                        failed_row_count = _dq_res[_rowdq_rule["rule"]]
+                        _row_dq_result.append(
+                            (
+                                _run_id,
+                                _product_id,
+                                _table_name,
+                                _rowdq_rule["rule_type"],
+                                _rowdq_rule["rule"],
+                                _rowdq_rule["expectation"],
+                                _rowdq_rule["tag"],
+                                _rowdq_rule["description"],
+                                "pass" if int(failed_row_count) == 0 else "fail",
+                                None,
+                                None,
+                                (_input_count - int(failed_row_count)),
+                                failed_row_count,
+                                _input_count,
+                                self._context.get_row_dq_start_time.replace(
+                                    tzinfo=timezone.utc
+                                ).strftime("%Y-%m-%d %H:%M:%S")
+                                if self._context.get_row_dq_start_time
+                                else "1900-01-01 00:00:00",
+                                self._context.get_row_dq_end_time.replace(
+                                    tzinfo=timezone.utc
+                                ).strftime("%Y-%m-%d %H:%M:%S")
+                                if self._context.get_row_dq_end_time
+                                else "1900-01-01 00:00:00",
+                            )
                         )
+                        _row_dq_expectations.remove(_rowdq_rule)
+
+            for _rowdq_rule in _row_dq_expectations:
+                _row_dq_result.append(
+                    (
+                        _run_id,
+                        _product_id,
+                        _table_name,
+                        _rowdq_rule["rule_type"],
+                        _rowdq_rule["rule"],
+                        _rowdq_rule["expectation"],
+                        _rowdq_rule["tag"],
+                        _rowdq_rule["description"],
+                        "pass",
+                        None,
+                        None,
+                        _input_count,
+                        "0",
+                        _input_count,
+                        self._context.get_row_dq_start_time.replace(
+                            tzinfo=timezone.utc
+                        ).strftime("%Y-%m-%d %H:%M:%S")
+                        if self._context.get_row_dq_start_time
+                        else "1900-01-01 00:00:00",
+                        self._context.get_row_dq_end_time.replace(
+                            tzinfo=timezone.utc
+                        ).strftime("%Y-%m-%d %H:%M:%S")
+                        if self._context.get_row_dq_end_time
+                        else "1900-01-01 00:00:00",
                     )
+                )
 
             return _row_dq_result
 
         except Exception as e:
             raise SparkExpectationsMiscException(
                 f"error occurred while fetching the stats from get_row_dq_detailed_stats {e}"
             )
@@ -262,14 +316,16 @@
             - dq_type
             - source_dq
             - run_date
             - compare
             - alias_comp
             - target_output
             - dq_time
+            - dq_start_time
+            - dq_end_time
         """
         _querydq_secondary_query_source_output = (
             self._context.get_source_query_dq_output
             if self._context.get_source_query_dq_output is not None
             and self._context.get_query_dq_detailed_stats_status
             else []
         )
@@ -370,14 +426,16 @@
                 "description",
                 "source_dq_status",
                 "source_dq_actual_outcome",
                 "source_dq_expected_outcome",
                 "source_dq_actual_row_count",
                 "source_dq_error_row_count",
                 "source_dq_row_count",
+                "source_dq_start_time",
+                "source_dq_end_time",
             ]
         )
         _detailed_stats_target_dq_schema = self._create_schema(
             [
                 "run_id",
                 "product_id",
                 "table_name",
@@ -388,14 +446,16 @@
                 "description",
                 "target_dq_status",
                 "target_dq_actual_outcome",
                 "target_dq_expected_outcome",
                 "target_dq_actual_row_count",
                 "target_dq_error_row_count",
                 "target_dq_row_count",
+                "target_dq_start_time",
+                "target_dq_end_time",
             ]
         )
         rules_execution_settings = self._context.get_rules_execution_settings_config
         _row_dq: bool = rules_execution_settings.get("row_dq", False)
         _target_agg_dq: bool = rules_execution_settings.get("target_agg_dq", False)
 
         _target_query_dq: bool = rules_execution_settings.get("target_query_dq", False)
@@ -404,19 +464,15 @@
             _source_aggdq_detailed_stats_result is not None
             and _source_querydq_detailed_stats_result is not None
         ):
             _source_aggdq_detailed_stats_result.extend(
                 _source_querydq_detailed_stats_result
             )
 
-        if (
-            self._context.get_row_dq_status != "Skipped"
-            and self._context.get_summarized_row_dq_res is not None
-            and len(self._context.get_summarized_row_dq_res) > 0
-        ):
+        if self._context.get_row_dq_status != "Skipped" and _row_dq:
             _rowdq_detailed_stats_result = self.get_row_dq_detailed_stats()
 
         else:
             _rowdq_detailed_stats_result = []
 
         if _source_aggdq_detailed_stats_result is not None:
             _source_aggdq_detailed_stats_result.extend(_rowdq_detailed_stats_result)
@@ -457,14 +513,18 @@
             "full_outer",
         )
 
         _df_detailed_stats = _df_detailed_stats.withColumn(
             "dq_date", current_date()
         ).withColumn("dq_time", lit(datetime.now().strftime("%Y-%m-%d %H:%M:%S")))
 
+        _df_detailed_stats = _df_detailed_stats.withColumn(
+            "dq_job_metadata_info", lit(self._context.get_job_metadata).cast("string")
+        )
+
         return _df_detailed_stats
 
     def write_detailed_stats(self) -> None:
         """
         This functions writes the detailed stats for all rule type into the detailed stats table
 
         Args:
@@ -519,27 +579,38 @@
                 _df_detailed_stats,
                 self._context.get_dq_detailed_stats_table_name,
                 config=self._context.get_detailed_stats_table_writer_config,
                 stats_table=True,
             )
 
             _log.info(
-                "Writing metrics to the querydq custom output table: %s, ended",
-                self._context.get_query_dq_output_custom_table_name,
+                "Writing metrics to the detailed stats table: %s, ended",
+                self._context.get_dq_detailed_stats_table_name,
             )
 
+            # TODO Create a separate function for writing the custom query dq stats
             _df_custom_detailed_stats_source = self._prep_secondary_query_output()
 
+            _log.info(
+                "Writing metrics to the output custom table: %s, started",
+                self._context.get_query_dq_output_custom_table_name,
+            )
+
             self.save_df_as_table(
                 _df_custom_detailed_stats_source,
                 self._context.get_query_dq_output_custom_table_name,
                 config=self._context.get_detailed_stats_table_writer_config,
                 stats_table=True,
             )
 
+            _log.info(
+                "Writing metrics to the output custom table: %s, ended",
+                self._context.get_query_dq_output_custom_table_name,
+            )
+
         except Exception as e:
             raise SparkExpectationsMiscException(
                 f"error occurred while saving the data into the stats table {e}"
             )
 
     def write_error_stats(self) -> None:
         """
@@ -725,24 +796,28 @@
             self.save_df_as_table(
                 df,
                 self._context.get_dq_stats_table_name,
                 config=self._context.get_stats_table_writer_config,
                 stats_table=True,
             )
 
+            _log.info(
+                "Writing metrics to the stats table: %s, ended",
+                self._context.get_dq_stats_table_name,
+            )
+
             if (
                 self._context.get_agg_dq_detailed_stats_status is True
                 or self._context.get_query_dq_detailed_stats_status is True
             ):
                 self.write_detailed_stats()
 
-            _log.info(
-                "Writing metrics to the stats table: %s, ended",
-                self._context.get_dq_stats_table_name,
-            )
+                # TODO Implement the below function for writing the custom query dq stats
+                # if self._context.get_query_dq_detailed_stats_status is True:
+                #     self.write_query_dq_custom_output()
 
             # TODO check if streaming_stats is set to off, if it's enabled only then this should run
 
             _se_stats_dict = self._context.get_se_streaming_stats_dict
             if _se_stats_dict["se.enable.streaming"]:
                 secret_handler = SparkExpectationsSecretsBackend(
                     secret_dict=_se_stats_dict
@@ -800,14 +875,27 @@
             )
 
     def write_error_records_final(
         self, df: DataFrame, error_table: str, rule_type: str
     ) -> Tuple[int, DataFrame]:
         try:
             _log.info("_write_error_records_final started")
+            df = df.withColumn("sequence_number", monotonically_increasing_id())
+
+            df_seq = df
+
+            df = df.select(
+                "sequence_number",
+                *[
+                    dq_column
+                    for dq_column in df.columns
+                    if dq_column.startswith(f"{rule_type}")
+                ],
+            )
+            df.cache()
 
             failed_records = [
                 f"size({dq_column}) != 0"
                 for dq_column in df.columns
                 if dq_column.startswith(f"{rule_type}")
             ]
 
@@ -837,15 +925,34 @@
                     self._context.get_run_id_name, lit(self._context.get_run_id)
                 )
                 .withColumn(
                     self._context.get_run_date_time_name,
                     lit(self._context.get_run_date),
                 )
             )
-            error_df = df.filter(f"size(meta_{rule_type}_results) != 0")
+            error_df_seq = df.filter(f"size(meta_{rule_type}_results) != 0")
+
+            error_df = df_seq.join(
+                error_df_seq,
+                df_seq.sequence_number == error_df_seq.sequence_number,
+                "inner",
+            )
+
+            # sequence number column removing from the data frame
+            error_df_columns = [
+                dq_column
+                for dq_column in error_df.columns
+                if (
+                    dq_column.startswith("sequence_number")
+                    or dq_column.startswith(rule_type)
+                )
+                is False
+            ]
+
+            error_df = error_df.select(error_df_columns)
             self._context.print_dataframe_with_debugger(error_df)
 
             print(
                 f"self._context.get_se_enable_error_table : {self._context.get_se_enable_error_table}"
             )
             if self._context.get_se_enable_error_table:
                 self.save_df_as_table(
@@ -854,14 +961,35 @@
                     self._context.get_target_and_error_table_writer_config,
                 )
 
             _error_count = error_df.count()
             # if _error_count > 0:
             self.generate_summarized_row_dq_res(error_df, rule_type)
 
+            # sequence number adding to dataframe for passing to action function
+            df = df_seq.join(
+                error_df_seq,
+                df_seq.sequence_number == error_df_seq.sequence_number,
+                "left",
+            ).withColumn(
+                f"meta_{rule_type}_results",
+                coalesce(col(f"meta_{rule_type}_results"), array()),
+            )
+
+            df = (
+                df.select(error_df_columns)
+                .withColumn(
+                    self._context.get_run_id_name, lit(self._context.get_run_id)
+                )
+                .withColumn(
+                    self._context.get_run_date_time_name,
+                    lit(self._context.get_run_date),
+                )
+            )
+
             _log.info("_write_error_records_final ended")
             return _error_count, df
 
         except Exception as e:
             raise SparkExpectationsMiscException(
                 f"error occurred while saving data into the final error table {e}"
             )
```

### Comparing `spark_expectations-2.0.0/spark_expectations/utils/actions.py` & `spark_expectations-2.1.0/spark_expectations/utils/actions.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,9 +1,10 @@
 from typing import Dict, List, Any, Optional, Tuple
 import re
+from datetime import datetime
 from pyspark.sql import DataFrame
 
 
 from pyspark.sql.functions import (
     create_map,
     expr,
     when,
@@ -116,15 +117,26 @@
         )  # return True if no unmatched left parentheses remain
 
     @staticmethod
     def agg_query_dq_detailed_result(
         _context: SparkExpectationsContext,
         _dq_rule: Dict[str, str],
         df: DataFrame,
-        querydq_output: List[Tuple[str, str, str, str, Any, str, dict, str]],
+        querydq_output: List[
+            Tuple[
+                str,
+                str,
+                str,
+                str,
+                Any,
+                str,
+                dict,
+                str,
+            ]
+        ],
         _source_dq_status: bool = False,
         _target_dq_status: bool = False,
     ) -> Any:
         """
         Executes detailed result aggregation for query-based data quality rules.
 
         Args:
@@ -524,26 +536,37 @@
                             _context.get_agg_dq_rule_type_name,
                             _context.get_query_dq_rule_type_name,
                         )
                     ) and (
                         _context.get_agg_dq_detailed_stats_status is True
                         or _context.get_query_dq_detailed_stats_status is True
                     ):
+                        current_date = datetime.now()
+                        dq_start_time = datetime.strftime(
+                            current_date, "%Y-%m-%d %H:%M:%S"
+                        )
+
                         (
                             _querydq_output_list,
                             _agg_query_dq_output_tuple,
                         ) = SparkExpectationsActions.agg_query_dq_detailed_result(
                             _context,
                             rule,
                             df,
                             querydq_output,
                             _source_dq_status=_source_dq_enabled,
                             _target_dq_status=_target_dq_enabled,
                         )
-
+                        current_date = datetime.now()
+                        dq_end_time = datetime.strftime(
+                            current_date, "%Y-%m-%d %H:%M:%S"
+                        )
+                        _agg_query_dq_output_list = list(_agg_query_dq_output_tuple)
+                        _agg_query_dq_output_list.extend([dq_start_time, dq_end_time])
+                        _agg_query_dq_output_tuple = tuple(_agg_query_dq_output_list)
                         _agg_query_dq_results.append(_agg_query_dq_output_tuple)
 
             if (
                 rule_type == _context.get_agg_dq_rule_type_name
                 and _context.get_agg_dq_detailed_stats_status is True
                 and _source_dq_enabled
             ):
@@ -650,17 +673,23 @@
             _source_query_dq_flag: Mark it as True when dq running for query level expectations on source dataframe
             _final_query_dq_flag: Mark it as True when dq running for query level expectations on final dataframe
         Returns:
                 DataFrame: Returns a dataframe after dropping the error from the dataset
 
         """
         try:
+            _df_dq_columns = [
+                dq_column
+                for dq_column in _df_dq.columns
+                if (dq_column.startswith(f"meta_{_rule_type}_results")) is False
+            ]
+            _df_dq_columns.append("action_if_failed")
             _df_dq = _df_dq.withColumn(
                 "action_if_failed", get_actions_list(col(f"meta_{_rule_type}_results"))
-            ).drop(f"meta_{_rule_type}_results")
+            ).select(_df_dq_columns)
 
             if (
                 not _df_dq.filter(
                     array_contains(_df_dq.action_if_failed, "fail")
                 ).count()
                 > 0
             ):
@@ -678,14 +707,13 @@
                     _context.set_final_query_dq_status("Failed")
 
                 raise SparkExpectOrFailException(
                     f"Job failed, as there is a data quality issue at {_rule_type} "
                     f"expectations and the action_if_failed "
                     "suggested to fail"
                 )
-
-            return _df_dq.drop(_df_dq.action_if_failed)
+            return _df_dq.select(_df_dq_columns[:-1])
 
         except Exception as e:
             raise SparkExpectationsMiscException(
                 f"error occurred while taking action on given rules {e}"
             )
```

### Comparing `spark_expectations-2.0.0/spark_expectations/utils/reader.py` & `spark_expectations-2.1.0/spark_expectations/utils/reader.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 import os
-from typing import Optional, Union, Dict
+from typing import Optional, Union, Dict, Tuple
 from dataclasses import dataclass
 from functools import reduce
 from pyspark.sql import DataFrame
 from pyspark.sql.functions import expr, when, max
 from spark_expectations import _log
 from spark_expectations.core.context import SparkExpectationsContext
 from spark_expectations.config.user_config import Constants as user_config
@@ -242,15 +242,15 @@
     def get_rules_from_df(
         self,
         rules_df: DataFrame,
         target_table: str,
         is_dlt: bool = False,
         tag: Optional[str] = None,
         params: Optional[dict] = None,
-    ) -> tuple[dict, dict, dict]:
+    ) -> Tuple[Dict, Dict, Dict]:
         """
         This function fetches the data quality rules from the table and return it as a dictionary
 
         Args:
             rules_df: DataFrame which has your data quality rules
             target_table: Provide the full table name for which the data quality rules are being run
             is_dlt: True if this for fetching the rules for dlt job
```

### Comparing `spark_expectations-2.0.0/spark_expectations/utils/regulate_flow.py` & `spark_expectations-2.1.0/spark_expectations/utils/regulate_flow.py`

 * *Files identical despite different names*

### Comparing `spark_expectations-2.0.0/spark_expectations/utils/udf.py` & `spark_expectations-2.1.0/spark_expectations/utils/udf.py`

 * *Files identical despite different names*

### Comparing `spark_expectations-2.0.0/PKG-INFO` & `spark_expectations-2.1.0/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,21 +1,21 @@
 Metadata-Version: 2.1
 Name: spark-expectations
-Version: 2.0.0
+Version: 2.1.0
 Summary: This project helps us to run Data Quality Rules in flight while spark job is being run
 Author: Ashok Singamaneni
 Author-email: ashok.singamaneni@nike.com
 Requires-Python: >=3.8.9,<4.0.0
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: Python :: 3.12
-Requires-Dist: pluggy (==1.0.0)
-Requires-Dist: pyspark (>=3.0.0,<4.0.0)
+Requires-Dist: pluggy (>=1)
+Requires-Dist: pyspark (>=3.0.0,<3.5)
 Requires-Dist: requests (>=2.28.1,<3.0.0)
 Description-Content-Type: text/markdown
 
 # Spark-Expectations
 
 [![CodeQL](https://github.com/Nike-Inc/spark-expectations/actions/workflows/codeql-analysis.yml/badge.svg)](https://github.com/Nike-Inc/spark-expectations/actions/workflows/codeql-analysis.yml)
 [![build](https://github.com/Nike-Inc/spark-expectations/actions/workflows/onpush.yml/badge.svg)](https://github.com/Nike-Inc/spark-expectations/actions/workflows/onpush.yml)
```

