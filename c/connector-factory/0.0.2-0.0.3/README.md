# Comparing `tmp/connector-factory-0.0.2.tar.gz` & `tmp/connector-factory-0.0.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "connector-factory-0.0.2.tar", last modified: Fri Dec 15 11:40:57 2023, max compression
+gzip compressed data, was "connector-factory-0.0.3.tar", last modified: Wed May 29 11:46:43 2024, max compression
```

## Comparing `connector-factory-0.0.2.tar` & `connector-factory-0.0.3.tar`

### file list

```diff
@@ -1,30 +1,34 @@
-drwxrwxr-x   0 ankit     (1001) ankit     (1001)        0 2023-12-15 11:40:57.593176 connector-factory-0.0.2/
--rw-rw-r--   0 ankit     (1001) ankit     (1001)     1074 2023-08-24 05:58:53.000000 connector-factory-0.0.2/LICENSE
--rw-rw-r--   0 ankit     (1001) ankit     (1001)      162 2023-08-24 08:19:39.000000 connector-factory-0.0.2/MANIFEST.in
--rw-rw-r--   0 ankit     (1001) ankit     (1001)    12403 2023-12-15 11:40:57.593176 connector-factory-0.0.2/PKG-INFO
--rw-rw-r--   0 ankit     (1001) ankit     (1001)    10891 2023-08-24 08:19:39.000000 connector-factory-0.0.2/README.md
-drwxrwxr-x   0 ankit     (1001) ankit     (1001)        0 2023-12-15 11:40:57.589176 connector-factory-0.0.2/connector_factory/
--rw-rw-r--   0 ankit     (1001) ankit     (1001)       39 2023-12-15 11:40:57.000000 connector-factory-0.0.2/connector_factory/.version
--rw-rw-r--   0 ankit     (1001) ankit     (1001)       38 2023-08-24 08:19:39.000000 connector-factory-0.0.2/connector_factory/__init__.py
-drwxrwxr-x   0 ankit     (1001) ankit     (1001)        0 2023-12-15 11:40:57.593176 connector-factory-0.0.2/connector_factory/common/
--rw-rw-r--   0 ankit     (1001) ankit     (1001)        0 2023-08-24 08:19:39.000000 connector-factory-0.0.2/connector_factory/common/__init__.py
--rw-rw-r--   0 ankit     (1001) ankit     (1001)     1621 2023-08-24 08:19:39.000000 connector-factory-0.0.2/connector_factory/common/common.py
-drwxrwxr-x   0 ankit     (1001) ankit     (1001)        0 2023-12-15 11:40:57.593176 connector-factory-0.0.2/connector_factory/connectors/
--rw-rw-r--   0 ankit     (1001) ankit     (1001)     1801 2023-08-24 08:19:39.000000 connector-factory-0.0.2/connector_factory/connectors/aws.py
--rw-rw-r--   0 ankit     (1001) ankit     (1001)     2913 2023-08-24 08:19:39.000000 connector-factory-0.0.2/connector_factory/connectors/mysql.py
--rw-rw-r--   0 ankit     (1001) ankit     (1001)     2925 2023-08-24 08:19:39.000000 connector-factory-0.0.2/connector_factory/connectors/postgreSQL.py
--rw-rw-r--   0 ankit     (1001) ankit     (1001)     2854 2023-08-24 08:19:39.000000 connector-factory-0.0.2/connector_factory/connectors/redshift.py
--rw-rw-r--   0 ankit     (1001) ankit     (1001)    11726 2023-08-24 08:19:39.000000 connector-factory-0.0.2/connector_factory/connectors/s3select.py
--rw-rw-r--   0 ankit     (1001) ankit     (1001)     6631 2023-12-15 11:40:01.000000 connector-factory-0.0.2/connector_factory/connectors/salesforce.py
--rw-rw-r--   0 ankit     (1001) ankit     (1001)     5932 2023-08-24 08:19:39.000000 connector-factory-0.0.2/connector_factory/connectors/snowflake.py
--rw-rw-r--   0 ankit     (1001) ankit     (1001)     2879 2023-08-24 08:19:39.000000 connector-factory-0.0.2/connector_factory/connectors/sqlite3.py
--rw-rw-r--   0 ankit     (1001) ankit     (1001)     8408 2023-08-24 08:19:39.000000 connector-factory-0.0.2/connector_factory/decorator.py
--rw-rw-r--   0 ankit     (1001) ankit     (1001)    11079 2023-08-24 08:19:39.000000 connector-factory-0.0.2/connector_factory/factory.py
-drwxrwxr-x   0 ankit     (1001) ankit     (1001)        0 2023-12-15 11:40:57.593176 connector-factory-0.0.2/connector_factory.egg-info/
--rw-rw-r--   0 ankit     (1001) ankit     (1001)    12403 2023-12-15 11:40:57.000000 connector-factory-0.0.2/connector_factory.egg-info/PKG-INFO
--rw-rw-r--   0 ankit     (1001) ankit     (1001)      765 2023-12-15 11:40:57.000000 connector-factory-0.0.2/connector_factory.egg-info/SOURCES.txt
--rw-rw-r--   0 ankit     (1001) ankit     (1001)        1 2023-12-15 11:40:57.000000 connector-factory-0.0.2/connector_factory.egg-info/dependency_links.txt
--rw-rw-r--   0 ankit     (1001) ankit     (1001)     5190 2023-12-15 11:40:57.000000 connector-factory-0.0.2/connector_factory.egg-info/requires.txt
--rw-rw-r--   0 ankit     (1001) ankit     (1001)       18 2023-12-15 11:40:57.000000 connector-factory-0.0.2/connector_factory.egg-info/top_level.txt
--rw-rw-r--   0 ankit     (1001) ankit     (1001)       67 2023-12-15 11:40:57.593176 connector-factory-0.0.2/setup.cfg
--rw-rw-r--   0 ankit     (1001) ankit     (1001)    10030 2023-08-24 08:19:39.000000 connector-factory-0.0.2/setup.py
+drwxrwxr-x   0 ankit     (1000) ankit     (1000)        0 2024-05-29 11:46:43.530319 connector-factory-0.0.3/
+-rw-rw-r--   0 ankit     (1000) ankit     (1000)     1074 2024-05-27 06:59:06.000000 connector-factory-0.0.3/LICENSE
+-rw-rw-r--   0 ankit     (1000) ankit     (1000)      162 2024-05-27 06:59:06.000000 connector-factory-0.0.3/MANIFEST.in
+-rw-rw-r--   0 ankit     (1000) ankit     (1000)    15504 2024-05-29 11:46:43.530319 connector-factory-0.0.3/PKG-INFO
+-rw-rw-r--   0 ankit     (1000) ankit     (1000)    13919 2024-05-29 11:44:19.000000 connector-factory-0.0.3/README.md
+drwxrwxr-x   0 ankit     (1000) ankit     (1000)        0 2024-05-29 11:46:43.530319 connector-factory-0.0.3/connector_factory/
+-rw-rw-r--   0 ankit     (1000) ankit     (1000)       45 2024-05-29 11:46:43.000000 connector-factory-0.0.3/connector_factory/.version
+-rw-rw-r--   0 ankit     (1000) ankit     (1000)       38 2024-05-27 06:59:06.000000 connector-factory-0.0.3/connector_factory/__init__.py
+drwxrwxr-x   0 ankit     (1000) ankit     (1000)        0 2024-05-29 11:46:43.530319 connector-factory-0.0.3/connector_factory/common/
+-rw-rw-r--   0 ankit     (1000) ankit     (1000)        0 2024-05-27 06:59:06.000000 connector-factory-0.0.3/connector_factory/common/__init__.py
+-rw-rw-r--   0 ankit     (1000) ankit     (1000)     1621 2024-05-27 06:59:06.000000 connector-factory-0.0.3/connector_factory/common/common.py
+drwxrwxr-x   0 ankit     (1000) ankit     (1000)        0 2024-05-29 11:46:43.530319 connector-factory-0.0.3/connector_factory/connectors/
+-rw-rw-r--   0 ankit     (1000) ankit     (1000)     1801 2024-05-27 06:59:06.000000 connector-factory-0.0.3/connector_factory/connectors/aws.py
+-rw-rw-r--   0 ankit     (1000) ankit     (1000)     3407 2024-05-29 11:44:19.000000 connector-factory-0.0.3/connector_factory/connectors/databricks.py
+-rw-rw-r--   0 ankit     (1000) ankit     (1000)     3468 2024-05-29 11:44:19.000000 connector-factory-0.0.3/connector_factory/connectors/db2.py
+-rw-rw-r--   0 ankit     (1000) ankit     (1000)     3335 2024-05-29 11:44:19.000000 connector-factory-0.0.3/connector_factory/connectors/dynamodb.py
+-rw-rw-r--   0 ankit     (1000) ankit     (1000)     2913 2024-05-27 06:59:06.000000 connector-factory-0.0.3/connector_factory/connectors/mysql.py
+-rw-rw-r--   0 ankit     (1000) ankit     (1000)     2925 2024-05-27 06:59:06.000000 connector-factory-0.0.3/connector_factory/connectors/postgreSQL.py
+-rw-rw-r--   0 ankit     (1000) ankit     (1000)     2804 2024-05-29 11:44:19.000000 connector-factory-0.0.3/connector_factory/connectors/redshift.py
+-rw-rw-r--   0 ankit     (1000) ankit     (1000)    11915 2024-05-29 11:44:19.000000 connector-factory-0.0.3/connector_factory/connectors/s3select.py
+-rw-rw-r--   0 ankit     (1000) ankit     (1000)     6631 2024-05-27 06:59:06.000000 connector-factory-0.0.3/connector_factory/connectors/salesforce.py
+-rw-rw-r--   0 ankit     (1000) ankit     (1000)     5932 2024-05-27 06:59:06.000000 connector-factory-0.0.3/connector_factory/connectors/snowflake.py
+-rw-rw-r--   0 ankit     (1000) ankit     (1000)     2879 2024-05-27 06:59:06.000000 connector-factory-0.0.3/connector_factory/connectors/sqlite3.py
+-rw-rw-r--   0 ankit     (1000) ankit     (1000)     4713 2024-05-29 11:44:19.000000 connector-factory-0.0.3/connector_factory/connectors/synapse.py
+-rw-rw-r--   0 ankit     (1000) ankit     (1000)     8414 2024-05-29 11:44:19.000000 connector-factory-0.0.3/connector_factory/decorator.py
+-rw-rw-r--   0 ankit     (1000) ankit     (1000)    12291 2024-05-29 11:44:19.000000 connector-factory-0.0.3/connector_factory/factory.py
+drwxrwxr-x   0 ankit     (1000) ankit     (1000)        0 2024-05-29 11:46:43.530319 connector-factory-0.0.3/connector_factory.egg-info/
+-rw-rw-r--   0 ankit     (1000) ankit     (1000)    15504 2024-05-29 11:46:43.000000 connector-factory-0.0.3/connector_factory.egg-info/PKG-INFO
+-rw-rw-r--   0 ankit     (1000) ankit     (1000)      925 2024-05-29 11:46:43.000000 connector-factory-0.0.3/connector_factory.egg-info/SOURCES.txt
+-rw-rw-r--   0 ankit     (1000) ankit     (1000)        1 2024-05-29 11:46:43.000000 connector-factory-0.0.3/connector_factory.egg-info/dependency_links.txt
+-rw-rw-r--   0 ankit     (1000) ankit     (1000)     6017 2024-05-29 11:46:43.000000 connector-factory-0.0.3/connector_factory.egg-info/requires.txt
+-rw-rw-r--   0 ankit     (1000) ankit     (1000)       18 2024-05-29 11:46:43.000000 connector-factory-0.0.3/connector_factory.egg-info/top_level.txt
+-rw-rw-r--   0 ankit     (1000) ankit     (1000)       67 2024-05-29 11:46:43.530319 connector-factory-0.0.3/setup.cfg
+-rw-rw-r--   0 ankit     (1000) ankit     (1000)    11022 2024-05-29 11:44:19.000000 connector-factory-0.0.3/setup.py
```

### Comparing `connector-factory-0.0.2/LICENSE` & `connector-factory-0.0.3/LICENSE`

 * *Files identical despite different names*

### Comparing `connector-factory-0.0.2/PKG-INFO` & `connector-factory-0.0.3/PKG-INFO`

 * *Files 12% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: connector-factory
-Version: 0.0.2
+Version: 0.0.3
 Summary: Connector Factory;
 Home-page: https://github.com/shrivastava-v-ankit/connector-factory
 Author: Ankit Shrivastava
 License: MIT
 Project-URL: Source, https://github.com/shrivastava-v-ankit/connector-factory/
 Project-URL: Tracker, https://github.com/shrivastava-v-ankit/connector-factory/issues
 Keywords: python,os independent,database,sqlalchemy,sqlite3,sqlite,postgres,mysql,maridb,snowflake,bigquery,gcp,aws,s3select,salesforce
@@ -22,23 +22,26 @@
 Classifier: Topic :: Software Development :: Libraries :: Python Modules
 Classifier: Topic :: Software Development :: Version Control :: Git
 Requires-Python: >=3.8, <3.12
 Description-Content-Type: text/markdown
 Provides-Extra: all
 Provides-Extra: aws
 Provides-Extra: bigquery
+Provides-Extra: databricks
+Provides-Extra: db2
+Provides-Extra: dynamodb
 Provides-Extra: gcp
 Provides-Extra: mariadb
 Provides-Extra: mysql
 Provides-Extra: postgres
 Provides-Extra: redshift
 Provides-Extra: s3select
 Provides-Extra: salesforce
 Provides-Extra: snowflake
-Provides-Extra: sqlite
+Provides-Extra: synapse
 License-File: LICENSE
 
 # connector-factory
 
 [![License: MIT](https://img.shields.io/badge/License-MIT-yellow.svg)](https://opensource.org/licenses/MIT)
 [![PyPI](https://img.shields.io/pypi/v/connector-factory.svg)](https://pypi.org/project/connector-factory)
 
@@ -58,18 +61,25 @@
 * BigQuery (Upcomming)
 * Snowflake
 * MariaDB
 * MySQL
 * Redshift
 * Salesforce
 * S3Select
+* Databricks
+* Synapse
+* DynamoDB
+* IBM DB2
 ```
 
-* Note: Only select operations are supported for Salesforce and S3Select.
-Connector factory can be enhanced for all the sqlalchemy supported database.
+* Note: Only select operations are supported for Salesforce and S3Select and limited functionality. These are not managed by the usage of sqlalchemy.
+
+* Note: Connector factory can be enhanced for all the sqlalchemy supported database.
+
+* Note: DynamoDB is supported via PyDynao. Please check the features and limitations at [PyDynamoDB](https://github.com/passren/PyDynamoDB/wiki).
 
 Connector factory also provide the facility to create the connections for Salesforce
 using simple-saleforce python package. Only Select query is supported in Salesforce. For advance usage it exposes the Salesforce object (simple-saleforce python package) which can be used as per the requirements. Refer [simple-saleforce](https://pypi.org/project/simple-salesforce/) for more detail.
 
 ## Getting Started
 
 ```bash
@@ -80,14 +90,18 @@
 * postgres
 * redshift
 * snowflake
 * mysql
 * mariadb
 * salesforce
 * s3select
+* databricks
+* synapse
+* db2
+* dynamodb
 * bigquery (upcomming)
 * all (For all supported types)
 
 
 ### Using connector-factory
 -----
 ```python
@@ -96,15 +110,14 @@
 
 temp_dir = tempfile.gettempdir()
 config = {
   "path": temp_dir,
   "database": "site.db"
   }
 db = ConnectorFactory(connector_type="sqlite", config=config)
-db.create_session()
 
 db.execute_sql(sql="create table test (id int PRIMARY KEY)")
 db.execute_sql(sql="insert into test values (1)")
 db.execute_sql(sql="insert into test values (2)")
 
 rows = db.execute_sql(sql="select * from test")
 if rows:
@@ -130,14 +143,18 @@
 *   postgres
 *   mysql
 *   mariadb
 *   snowflake
 *   redshift
 *   salesforce
 *   s3select
+*   databricks
+*   synapse
+*   db2
+*   dynamodb
 ```
 
 ### Configuration parameters for sqlite:
 -----
 -----
 ```python
 * connector_type: sqlite
@@ -307,14 +324,104 @@
 * type: (Required)=> Supported types is one of csv, json or parquet.
 * file (Required)=> Full file path without bucket or prefix key to serach for similar files as per the type of files provided. First line is considered as header of file for csv. Example: if only prefix is provided like mypath/mydatafile and type is csv then all files named as mypath/mydatafile*.csv will be read.
 * limit: (Optional)=> Commulative number of records to read from the file (multiple files).
 * compression: (Optional)=> Supported types is one of GZIP, BZIP2 or NONE.
 -----
 
 
+### Connection parameters for Synapse:
+-----
+-----
+```python
+* connector_type: synapse
+* config = {
+    "username": "<synapse_user>",
+    "password": "<user_password>",
+    "host": "<hostname_of_synapse_service>",
+    "port": "<port_of_synapse_service>",
+    "database": "<database_name>",
+    "driver": "<driver_to_connect_synapse_service>",
+    "trust_certificate": "<trust_the_synapse_connection>",
+    "authentication_with": "<authentication_type_of_synapse_service>",
+    "connection_timeout": "<connection_timeout_to_synapse_service>"
+}
+```
+
+**Details:**
+* username: (Required)=> Name of user for connection.
+* password (Required)=> Password of user.
+* host: (Required)=> Host of Synapse service.
+* port: (Optional)=> Port of Synapse service. Default to 1433
+* database: (Required)=> Database name.
+* driver: (Optional)=> Name of driver to use. Default to ODBC Driver 17 for SQL Server.
+* trust_certificate: (Optional)=> Trust the connection with certificate. Default to no.
+* authentication_with: (Optional)=> Default to None and not in use to authenticate with. If service principal or AD authenitication is used then pass appropriate value.
+* connection_timeout: (Optional)=> Connection timeout. Default to 30.
+-----
+
+
+### Connection parameters for Databricks:
+-----
+-----
+```python
+* connector_type: databricks
+* config = {
+    "hostname": "<hostname_of_databricks_service>",
+    "token": "<pat_token_of_databricks_as_password>",
+    "http_path": "<path_of_warehouse_or_cluster>",
+    "catalog": "<catalog_name_of_databricks>",
+    "schema": "<schema_name_of_databricks>",
+}
+```
+
+**Details:**
+* hostname: (Required)=> Databricks hostname.
+* token (Required)=> Pat token of user.
+* http_path: (Required)=> Path of warehouse or cluster.
+* catalog: (Required)=> Unity catalog name
+* schema: (Required)=> Schema name under catalog.
+-----
+
+
+### Connection parameters for IBM DB2:
+-----
+-----
+```python
+* connector_type: db2
+* config = {
+    "username": "<hostname_of_databricks_service>",
+    "password": "<pat_token_of_databricks_as_password>",
+    "host": "<path_of_warehouse_or_cluster>",
+    "port": "<catalog_name_of_databricks>",
+    "database": "<schema_name_of_databricks>",
+}
+```
+
+**Details:**
+* username: (Required)=> Name of user for connection.
+* password (Required)=> Password of user.
+* host: (Required)=> Host of IBM DB2 Server.
+* port: (Optional)=> Port of IBM DB2 Server. Default to 50000
+* database: (Required)=> Database name.
+-----
+
+
+### Connection parameters for DynamoDB:
+-----
+-----
+```python
+* connector_type: dynamodb
+* config = {
+    "region": "<aws_region_of_dynamodb>"
+}
+```
+
+**Details:**
+* region: (Optional)=> AWS Region. Default is us-east-1
+-----
 
 
 ### Development Setup
 
 #### Using virtualenv
 
 ```bash
```

### Comparing `connector-factory-0.0.2/README.md` & `connector-factory-0.0.3/README.md`

 * *Files 18% similar despite different names*

```diff
@@ -19,18 +19,25 @@
 * BigQuery (Upcomming)
 * Snowflake
 * MariaDB
 * MySQL
 * Redshift
 * Salesforce
 * S3Select
+* Databricks
+* Synapse
+* DynamoDB
+* IBM DB2
 ```
 
-* Note: Only select operations are supported for Salesforce and S3Select.
-Connector factory can be enhanced for all the sqlalchemy supported database.
+* Note: Only select operations are supported for Salesforce and S3Select and limited functionality. These are not managed by the usage of sqlalchemy.
+
+* Note: Connector factory can be enhanced for all the sqlalchemy supported database.
+
+* Note: DynamoDB is supported via PyDynao. Please check the features and limitations at [PyDynamoDB](https://github.com/passren/PyDynamoDB/wiki).
 
 Connector factory also provide the facility to create the connections for Salesforce
 using simple-saleforce python package. Only Select query is supported in Salesforce. For advance usage it exposes the Salesforce object (simple-saleforce python package) which can be used as per the requirements. Refer [simple-saleforce](https://pypi.org/project/simple-salesforce/) for more detail.
 
 ## Getting Started
 
 ```bash
@@ -41,14 +48,18 @@
 * postgres
 * redshift
 * snowflake
 * mysql
 * mariadb
 * salesforce
 * s3select
+* databricks
+* synapse
+* db2
+* dynamodb
 * bigquery (upcomming)
 * all (For all supported types)
 
 
 ### Using connector-factory
 -----
 ```python
@@ -57,15 +68,14 @@
 
 temp_dir = tempfile.gettempdir()
 config = {
   "path": temp_dir,
   "database": "site.db"
   }
 db = ConnectorFactory(connector_type="sqlite", config=config)
-db.create_session()
 
 db.execute_sql(sql="create table test (id int PRIMARY KEY)")
 db.execute_sql(sql="insert into test values (1)")
 db.execute_sql(sql="insert into test values (2)")
 
 rows = db.execute_sql(sql="select * from test")
 if rows:
@@ -91,14 +101,18 @@
 *   postgres
 *   mysql
 *   mariadb
 *   snowflake
 *   redshift
 *   salesforce
 *   s3select
+*   databricks
+*   synapse
+*   db2
+*   dynamodb
 ```
 
 ### Configuration parameters for sqlite:
 -----
 -----
 ```python
 * connector_type: sqlite
@@ -268,14 +282,104 @@
 * type: (Required)=> Supported types is one of csv, json or parquet.
 * file (Required)=> Full file path without bucket or prefix key to serach for similar files as per the type of files provided. First line is considered as header of file for csv. Example: if only prefix is provided like mypath/mydatafile and type is csv then all files named as mypath/mydatafile*.csv will be read.
 * limit: (Optional)=> Commulative number of records to read from the file (multiple files).
 * compression: (Optional)=> Supported types is one of GZIP, BZIP2 or NONE.
 -----
 
 
+### Connection parameters for Synapse:
+-----
+-----
+```python
+* connector_type: synapse
+* config = {
+    "username": "<synapse_user>",
+    "password": "<user_password>",
+    "host": "<hostname_of_synapse_service>",
+    "port": "<port_of_synapse_service>",
+    "database": "<database_name>",
+    "driver": "<driver_to_connect_synapse_service>",
+    "trust_certificate": "<trust_the_synapse_connection>",
+    "authentication_with": "<authentication_type_of_synapse_service>",
+    "connection_timeout": "<connection_timeout_to_synapse_service>"
+}
+```
+
+**Details:**
+* username: (Required)=> Name of user for connection.
+* password (Required)=> Password of user.
+* host: (Required)=> Host of Synapse service.
+* port: (Optional)=> Port of Synapse service. Default to 1433
+* database: (Required)=> Database name.
+* driver: (Optional)=> Name of driver to use. Default to ODBC Driver 17 for SQL Server.
+* trust_certificate: (Optional)=> Trust the connection with certificate. Default to no.
+* authentication_with: (Optional)=> Default to None and not in use to authenticate with. If service principal or AD authenitication is used then pass appropriate value.
+* connection_timeout: (Optional)=> Connection timeout. Default to 30.
+-----
+
+
+### Connection parameters for Databricks:
+-----
+-----
+```python
+* connector_type: databricks
+* config = {
+    "hostname": "<hostname_of_databricks_service>",
+    "token": "<pat_token_of_databricks_as_password>",
+    "http_path": "<path_of_warehouse_or_cluster>",
+    "catalog": "<catalog_name_of_databricks>",
+    "schema": "<schema_name_of_databricks>",
+}
+```
+
+**Details:**
+* hostname: (Required)=> Databricks hostname.
+* token (Required)=> Pat token of user.
+* http_path: (Required)=> Path of warehouse or cluster.
+* catalog: (Required)=> Unity catalog name
+* schema: (Required)=> Schema name under catalog.
+-----
+
+
+### Connection parameters for IBM DB2:
+-----
+-----
+```python
+* connector_type: db2
+* config = {
+    "username": "<hostname_of_databricks_service>",
+    "password": "<pat_token_of_databricks_as_password>",
+    "host": "<path_of_warehouse_or_cluster>",
+    "port": "<catalog_name_of_databricks>",
+    "database": "<schema_name_of_databricks>",
+}
+```
+
+**Details:**
+* username: (Required)=> Name of user for connection.
+* password (Required)=> Password of user.
+* host: (Required)=> Host of IBM DB2 Server.
+* port: (Optional)=> Port of IBM DB2 Server. Default to 50000
+* database: (Required)=> Database name.
+-----
+
+
+### Connection parameters for DynamoDB:
+-----
+-----
+```python
+* connector_type: dynamodb
+* config = {
+    "region": "<aws_region_of_dynamodb>"
+}
+```
+
+**Details:**
+* region: (Optional)=> AWS Region. Default is us-east-1
+-----
 
 
 ### Development Setup
 
 #### Using virtualenv
 
 ```bash
```

### Comparing `connector-factory-0.0.2/connector_factory/common/common.py` & `connector-factory-0.0.3/connector_factory/common/common.py`

 * *Files identical despite different names*

### Comparing `connector-factory-0.0.2/connector_factory/connectors/aws.py` & `connector-factory-0.0.3/connector_factory/connectors/aws.py`

 * *Files identical despite different names*

### Comparing `connector-factory-0.0.2/connector_factory/connectors/mysql.py` & `connector-factory-0.0.3/connector_factory/connectors/mysql.py`

 * *Files identical despite different names*

### Comparing `connector-factory-0.0.2/connector_factory/connectors/postgreSQL.py` & `connector-factory-0.0.3/connector_factory/connectors/postgreSQL.py`

 * *Files identical despite different names*

### Comparing `connector-factory-0.0.2/connector_factory/connectors/redshift.py` & `connector-factory-0.0.3/connector_factory/connectors/redshift.py`

 * *Files 8% similar despite different names*

```diff
@@ -48,16 +48,14 @@
     def create_uri(self):
         super().create_uri()
         logger.info("Call for creating the URI for Redshift")
 
         is_valid, message = self.validate_config()
         uri = None
         if is_valid:
-            from snowflake.sqlalchemy import URL
-
             username = self.config.get("username", None)
             password = self.config.get("password", None)
             host = self.config.get("host", None)
             port = self.config.get("port", 5439)
             database = self.config.get("database", "")
 
             if password:
```

### Comparing `connector-factory-0.0.2/connector_factory/connectors/s3select.py` & `connector-factory-0.0.3/connector_factory/connectors/s3select.py`

 * *Files 2% similar despite different names*

```diff
@@ -19,26 +19,27 @@
         self.is_valid = False
         self.aws = None
         self.aws_session = None
         self.files = []
 
     def validate_config(self):
         super().validate_config()
-        logger.info("Validating the paylod for the Redshift connection")
+        logger.info("Validating the paylod for the S3select connection")
         message = ""
 
         if not self.is_valid:
             import botocore
 
             bucket = self.config.get("bucket", None)
             file = self.config.get("file", None)
             file_type = self.config.get("type", None)
             compression = self.config.get("compression", None)
             record_delimiter = self.config.get("record_delimiter", None)
             field_delimiter = self.config.get("field_delimiter", None)
+            region = self.config.get("region", None)
 
             if not bucket or not file or not file_type:
                 message = f"Invalid connection details. file, password and file_type are required.{os.linesep}"
                 self.is_valid = False
                 logger.error(message)
             else:
                 self.is_valid = True
@@ -60,14 +61,17 @@
 
             if not record_delimiter:
                 message = f"{message}Record delimiter is not provided. Default '\n' will be used.{os.linesep}"
 
             if not field_delimiter:
                 message = f"{message}Field_delimiter is not provided. Default ',' will be used.{os.linesep}"
 
+            if not region:
+                message = f"{message}Region is not provided. Default 'us-east-1' will be used.{os.linesep}"
+
             if self.is_valid:
                 logger.info("Connection is valid")
 
                 if message:
                     logger.info(message)
 
         return self.is_valid, message
```

### Comparing `connector-factory-0.0.2/connector_factory/connectors/salesforce.py` & `connector-factory-0.0.3/connector_factory/connectors/salesforce.py`

 * *Files identical despite different names*

### Comparing `connector-factory-0.0.2/connector_factory/connectors/snowflake.py` & `connector-factory-0.0.3/connector_factory/connectors/snowflake.py`

 * *Files identical despite different names*

### Comparing `connector-factory-0.0.2/connector_factory/connectors/sqlite3.py` & `connector-factory-0.0.3/connector_factory/connectors/sqlite3.py`

 * *Files identical despite different names*

### Comparing `connector-factory-0.0.2/connector_factory/decorator.py` & `connector-factory-0.0.3/connector_factory/decorator.py`

 * *Files 2% similar despite different names*

```diff
@@ -35,14 +35,15 @@
         and create the URI depending upon the database signature.
         """
         pass
 
     def destroy(self):
         try:
             if (self.session):
+                self.session.close()
                 self.session.remove()
                 self.engine.dispose(close=True)
                 self.session = None
                 self.engine = None
                 logger.info("Successfully dispose the connection")
         except Exception as err:
             message = f"Failed to close connection"
@@ -147,15 +148,14 @@
                             or fail.
         *******
         Return:
         -------
 
             rows:           If rows in case of DDL queries else none.
         """
-        print("*************")
         logger.info(
             "Got pandas dataframe to insert/update in table {table_name}")
         message = None
 
         if not self.session:
             _, _, message = self.get_session(None)
```

### Comparing `connector-factory-0.0.2/connector_factory/factory.py` & `connector-factory-0.0.3/connector_factory/factory.py`

 * *Files 4% similar despite different names*

```diff
@@ -17,15 +17,20 @@
                     "mysql",
                     "mariadb",
                     "snowflake",
                     "redshift",
                     "sqlite",
                     "salesforce",
                     "s3select"
-                    "aws"]
+                    "aws",
+                    "databricks",
+                    "synapse",
+                    "db2",
+                    "dynamodb"
+                    ]
 
 SUPPORTED_SECRET_MANAGER_CLOUD = ["aws", "gcp"]
 
 
 class ConnectorFactory(object):
     """Class handle the Database Manager using SQLAlchemy Dialects or specific
     object of supported python libraries which don't supports SQLAlchemy.
@@ -76,14 +81,18 @@
                                     * mysql
                                     * mariadb
                                     * snowflake
                                     * s3select
                                     * sqlite
                                     * redshift
                                     * salesforce
+                                    * databricks
+                                    * synapse
+                                    * db2
+                                    * dynamodb
             config (dict):  (Required) => Dictonary of connection details like username, password, host, port etc.
             debug (bool, optional): (Optional) => Detailed logs for debugging.. Defaults to False.
         """
 
         self.engine_type = connector_type
         self.config = config
         self.debug = debug
@@ -114,14 +123,26 @@
             self.is_connector = True
         elif self.engine_type in ["s3select"]:
             from .connectors.s3select import S3Select as Connector
             self.is_connector = True
         elif self.engine_type in ["aws"]:
             from .connectors.aws import Aws as Connector
             self.is_connector = True
+        elif self.engine_type in ["databricks"]:
+            from .connectors.databricks import Databricks as Connector
+            self.is_connector = True
+        elif self.engine_type in ["synapse"]:
+            from .connectors.synapse import Synapse as Connector
+            self.is_connector = True
+        elif self.engine_type in ["db2"]:
+            from .connectors.db2 import Db2 as Connector
+            self.is_connector = True
+        elif self.engine_type in ["dynamodb"]:
+            from .connectors.dynamodb import DynamoDb as Connector
+            self.is_connector = True
 
         if self.is_connector:
             self.connection = Connector(self.config)
 
     def create_session(self):
         """Method to create the SQLAlchemy session for the initalized the engine type.
         Use the class variables and update to hold the sessions.
@@ -277,7 +298,17 @@
             rows:           If rows in case of DDL queries else none.
         """
 
         if self.is_connector:
             return self.connection.get_df(sql=sql, chunk_size=chunk_size)
         else:
             return f"Invalid connection type : {self.engine_type}. Valid type is anyone from {SUPPORTED_ENGINE}"
+
+    def destroy(self):
+        """
+        Function to close the sessions.
+        """
+
+        if self.is_connector:
+            return self.connection.destroy()
+        else:
+            return f"Invalid connection type : {self.engine_type}. Valid type is anyone from {SUPPORTED_ENGINE}"
```

### Comparing `connector-factory-0.0.2/connector_factory.egg-info/PKG-INFO` & `connector-factory-0.0.3/connector_factory.egg-info/PKG-INFO`

 * *Files 12% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: connector-factory
-Version: 0.0.2
+Version: 0.0.3
 Summary: Connector Factory;
 Home-page: https://github.com/shrivastava-v-ankit/connector-factory
 Author: Ankit Shrivastava
 License: MIT
 Project-URL: Source, https://github.com/shrivastava-v-ankit/connector-factory/
 Project-URL: Tracker, https://github.com/shrivastava-v-ankit/connector-factory/issues
 Keywords: python,os independent,database,sqlalchemy,sqlite3,sqlite,postgres,mysql,maridb,snowflake,bigquery,gcp,aws,s3select,salesforce
@@ -22,23 +22,26 @@
 Classifier: Topic :: Software Development :: Libraries :: Python Modules
 Classifier: Topic :: Software Development :: Version Control :: Git
 Requires-Python: >=3.8, <3.12
 Description-Content-Type: text/markdown
 Provides-Extra: all
 Provides-Extra: aws
 Provides-Extra: bigquery
+Provides-Extra: databricks
+Provides-Extra: db2
+Provides-Extra: dynamodb
 Provides-Extra: gcp
 Provides-Extra: mariadb
 Provides-Extra: mysql
 Provides-Extra: postgres
 Provides-Extra: redshift
 Provides-Extra: s3select
 Provides-Extra: salesforce
 Provides-Extra: snowflake
-Provides-Extra: sqlite
+Provides-Extra: synapse
 License-File: LICENSE
 
 # connector-factory
 
 [![License: MIT](https://img.shields.io/badge/License-MIT-yellow.svg)](https://opensource.org/licenses/MIT)
 [![PyPI](https://img.shields.io/pypi/v/connector-factory.svg)](https://pypi.org/project/connector-factory)
 
@@ -58,18 +61,25 @@
 * BigQuery (Upcomming)
 * Snowflake
 * MariaDB
 * MySQL
 * Redshift
 * Salesforce
 * S3Select
+* Databricks
+* Synapse
+* DynamoDB
+* IBM DB2
 ```
 
-* Note: Only select operations are supported for Salesforce and S3Select.
-Connector factory can be enhanced for all the sqlalchemy supported database.
+* Note: Only select operations are supported for Salesforce and S3Select and limited functionality. These are not managed by the usage of sqlalchemy.
+
+* Note: Connector factory can be enhanced for all the sqlalchemy supported database.
+
+* Note: DynamoDB is supported via PyDynao. Please check the features and limitations at [PyDynamoDB](https://github.com/passren/PyDynamoDB/wiki).
 
 Connector factory also provide the facility to create the connections for Salesforce
 using simple-saleforce python package. Only Select query is supported in Salesforce. For advance usage it exposes the Salesforce object (simple-saleforce python package) which can be used as per the requirements. Refer [simple-saleforce](https://pypi.org/project/simple-salesforce/) for more detail.
 
 ## Getting Started
 
 ```bash
@@ -80,14 +90,18 @@
 * postgres
 * redshift
 * snowflake
 * mysql
 * mariadb
 * salesforce
 * s3select
+* databricks
+* synapse
+* db2
+* dynamodb
 * bigquery (upcomming)
 * all (For all supported types)
 
 
 ### Using connector-factory
 -----
 ```python
@@ -96,15 +110,14 @@
 
 temp_dir = tempfile.gettempdir()
 config = {
   "path": temp_dir,
   "database": "site.db"
   }
 db = ConnectorFactory(connector_type="sqlite", config=config)
-db.create_session()
 
 db.execute_sql(sql="create table test (id int PRIMARY KEY)")
 db.execute_sql(sql="insert into test values (1)")
 db.execute_sql(sql="insert into test values (2)")
 
 rows = db.execute_sql(sql="select * from test")
 if rows:
@@ -130,14 +143,18 @@
 *   postgres
 *   mysql
 *   mariadb
 *   snowflake
 *   redshift
 *   salesforce
 *   s3select
+*   databricks
+*   synapse
+*   db2
+*   dynamodb
 ```
 
 ### Configuration parameters for sqlite:
 -----
 -----
 ```python
 * connector_type: sqlite
@@ -307,14 +324,104 @@
 * type: (Required)=> Supported types is one of csv, json or parquet.
 * file (Required)=> Full file path without bucket or prefix key to serach for similar files as per the type of files provided. First line is considered as header of file for csv. Example: if only prefix is provided like mypath/mydatafile and type is csv then all files named as mypath/mydatafile*.csv will be read.
 * limit: (Optional)=> Commulative number of records to read from the file (multiple files).
 * compression: (Optional)=> Supported types is one of GZIP, BZIP2 or NONE.
 -----
 
 
+### Connection parameters for Synapse:
+-----
+-----
+```python
+* connector_type: synapse
+* config = {
+    "username": "<synapse_user>",
+    "password": "<user_password>",
+    "host": "<hostname_of_synapse_service>",
+    "port": "<port_of_synapse_service>",
+    "database": "<database_name>",
+    "driver": "<driver_to_connect_synapse_service>",
+    "trust_certificate": "<trust_the_synapse_connection>",
+    "authentication_with": "<authentication_type_of_synapse_service>",
+    "connection_timeout": "<connection_timeout_to_synapse_service>"
+}
+```
+
+**Details:**
+* username: (Required)=> Name of user for connection.
+* password (Required)=> Password of user.
+* host: (Required)=> Host of Synapse service.
+* port: (Optional)=> Port of Synapse service. Default to 1433
+* database: (Required)=> Database name.
+* driver: (Optional)=> Name of driver to use. Default to ODBC Driver 17 for SQL Server.
+* trust_certificate: (Optional)=> Trust the connection with certificate. Default to no.
+* authentication_with: (Optional)=> Default to None and not in use to authenticate with. If service principal or AD authenitication is used then pass appropriate value.
+* connection_timeout: (Optional)=> Connection timeout. Default to 30.
+-----
+
+
+### Connection parameters for Databricks:
+-----
+-----
+```python
+* connector_type: databricks
+* config = {
+    "hostname": "<hostname_of_databricks_service>",
+    "token": "<pat_token_of_databricks_as_password>",
+    "http_path": "<path_of_warehouse_or_cluster>",
+    "catalog": "<catalog_name_of_databricks>",
+    "schema": "<schema_name_of_databricks>",
+}
+```
+
+**Details:**
+* hostname: (Required)=> Databricks hostname.
+* token (Required)=> Pat token of user.
+* http_path: (Required)=> Path of warehouse or cluster.
+* catalog: (Required)=> Unity catalog name
+* schema: (Required)=> Schema name under catalog.
+-----
+
+
+### Connection parameters for IBM DB2:
+-----
+-----
+```python
+* connector_type: db2
+* config = {
+    "username": "<hostname_of_databricks_service>",
+    "password": "<pat_token_of_databricks_as_password>",
+    "host": "<path_of_warehouse_or_cluster>",
+    "port": "<catalog_name_of_databricks>",
+    "database": "<schema_name_of_databricks>",
+}
+```
+
+**Details:**
+* username: (Required)=> Name of user for connection.
+* password (Required)=> Password of user.
+* host: (Required)=> Host of IBM DB2 Server.
+* port: (Optional)=> Port of IBM DB2 Server. Default to 50000
+* database: (Required)=> Database name.
+-----
+
+
+### Connection parameters for DynamoDB:
+-----
+-----
+```python
+* connector_type: dynamodb
+* config = {
+    "region": "<aws_region_of_dynamodb>"
+}
+```
+
+**Details:**
+* region: (Optional)=> AWS Region. Default is us-east-1
+-----
 
 
 ### Development Setup
 
 #### Using virtualenv
 
 ```bash
```

### Comparing `connector-factory-0.0.2/connector_factory.egg-info/SOURCES.txt` & `connector-factory-0.0.3/connector_factory.egg-info/SOURCES.txt`

 * *Files 16% similar despite different names*

```diff
@@ -11,14 +11,18 @@
 connector_factory.egg-info/SOURCES.txt
 connector_factory.egg-info/dependency_links.txt
 connector_factory.egg-info/requires.txt
 connector_factory.egg-info/top_level.txt
 connector_factory/common/__init__.py
 connector_factory/common/common.py
 connector_factory/connectors/aws.py
+connector_factory/connectors/databricks.py
+connector_factory/connectors/db2.py
+connector_factory/connectors/dynamodb.py
 connector_factory/connectors/mysql.py
 connector_factory/connectors/postgreSQL.py
 connector_factory/connectors/redshift.py
 connector_factory/connectors/s3select.py
 connector_factory/connectors/salesforce.py
 connector_factory/connectors/snowflake.py
-connector_factory/connectors/sqlite3.py
+connector_factory/connectors/sqlite3.py
+connector_factory/connectors/synapse.py
```

### Comparing `connector-factory-0.0.2/connector_factory.egg-info/requires.txt` & `connector-factory-0.0.3/connector_factory.egg-info/requires.txt`

 * *Files 9% similar despite different names*

```diff
@@ -14,250 +14,305 @@
 botocore==1.31.22
 cachetools==5.3.1
 cachetools==5.3.1
 certifi==2023.7.22
 certifi==2023.7.22
 certifi==2023.7.22
 certifi==2023.7.22
+certifi==2023.7.22
 cffi==1.15.1
 cffi==1.15.1
 charset-normalizer==3.2.0
 charset-normalizer==3.2.0
 charset-normalizer==3.2.0
 charset-normalizer==3.2.0
+charset-normalizer==3.2.0
 cryptography==41.0.3
 cryptography==41.0.3
+databricks-sql-connector==2.9.6
+et-xmlfile==1.1.0
 filelock==3.12.2
 future==0.18.3
-future==0.18.3
 google-api-core==2.11.1
 google-api-core==2.11.1
 google-api-python-client==2.96.0
 google-auth-httplib2==0.1.0
 google-auth==2.22.0
 google-auth==2.22.0
 google-cloud-bigquery==3.11.4
 google-cloud-core==2.3.3
-google-cloud-core==2.3.3
 google-cloud-secret-manager==2.16.3
 google-crc32c==1.5.0
 google-resumable-media==2.5.0
-google-resumable-media==2.5.0
 googleapis-common-protos==1.60.0
 googleapis-common-protos==1.60.0
 greenlet==2.0.2
 greenlet==2.0.2
+greenlet==2.0.2
+greenlet==2.0.2
 grpc-google-iam-v1==0.12.6
 grpcio-status==1.56.2
 grpcio-status==1.56.2
 grpcio==1.56.2
 grpcio==1.56.2
 httplib2==0.22.0
+ibm-db-sa==0.4.0
+ibm_db==3.2.3
+idna==3.4
 idna==3.4
 idna==3.4
 idna==3.4
 idna==3.4
 isodate==0.6.1
 jmespath==1.0.1
 lxml==4.9.3
+lz4==4.3.3
+numpy==1.25.2
+oauthlib==3.2.2
+openpyxl==3.1.2
 oscrypto==1.3.0
 packaging==23.1
 packaging==23.1
-packaging==23.1
+pandas==2.0.3
 platformdirs==3.8.1
 platformdirs==3.8.1
 proto-plus==1.22.3
 proto-plus==1.22.3
 protobuf==4.24.0
 protobuf==4.24.0
 psycopg2-binary==2.9.7
 psycopg2-binary==2.9.7
 pyOpenSSL==23.2.0
+pyarrow==14.0.2
 pyasn1-modules==0.3.0
 pyasn1-modules==0.3.0
 pyasn1==0.5.0
 pyasn1==0.5.0
 pybigquery==0.5.0
 pycparser==2.21
+pycparser==2.21
 pycryptodomex==3.18.0
 pyjwt==2.8.0
 pyjwt==2.8.0
+pyjwt==2.8.0
 pymysql==1.1.0
+pyodbc==5.1.0
 pyparsing==3.1.1
 python-dateutil==2.8.2
 python-dateutil==2.8.2
+python-dateutil==2.8.2
+pytz==2023.3
+pytz==2023.3
 requests-file==1.5.1
 requests-toolbelt==1.0.0
 requests==2.31.0
 requests==2.31.0
 requests==2.31.0
 requests==2.31.0
 requests==2.31.0
 rsa==4.9
 rsa==4.9
 s3transfer==0.6.1
 simple-salesforce==1.12.4
 six==1.16.0
 six==1.16.0
 six==1.16.0
+six==1.16.0
+six==1.16.0
 snowflake-connector-python==3.1.0
 snowflake-sqlalchemy==1.4.7
 sortedcontainers==2.4.0
 sqlalchemy==1.4.49
+sqlalchemy==1.4.49
+sqlalchemy==1.4.49
+sqlalchemy==1.4.49
+thrift==0.16.0
 tomlkit==0.12.1
 typing-extensions==4.7.1
+typing-extensions==4.7.1
+typing-extensions==4.7.1
+typing-extensions==4.7.1
+tzdata==2023.3
 uritemplate==4.1.1
 urllib3==1.26.16
 urllib3==1.26.16
 urllib3==1.26.16
 urllib3==1.26.16
 urllib3==1.26.16
+urllib3==1.26.16
 zeep==4.2.1
 
 [aws]
 boto3==1.28.22
 botocore==1.31.22
 jmespath==1.0.1
+python-dateutil==2.8.2
 s3transfer==0.6.1
+six==1.16.0
 urllib3==1.26.16
 
 [bigquery]
 cachetools==5.3.1
 cachetools==5.3.1
 certifi==2023.7.22
 certifi==2023.7.22
 charset-normalizer==3.2.0
 charset-normalizer==3.2.0
 future==0.18.3
-future==0.18.3
 google-api-core==2.11.1
 google-api-core==2.11.1
 google-api-python-client==2.96.0
 google-auth-httplib2==0.1.0
 google-auth==2.22.0
 google-auth==2.22.0
 google-cloud-bigquery==3.11.4
 google-cloud-core==2.3.3
-google-cloud-core==2.3.3
 google-cloud-secret-manager==2.16.3
 google-crc32c==1.5.0
 google-resumable-media==2.5.0
-google-resumable-media==2.5.0
 googleapis-common-protos==1.60.0
 googleapis-common-protos==1.60.0
 greenlet==2.0.2
-greenlet==2.0.2
 grpc-google-iam-v1==0.12.6
 grpcio-status==1.56.2
 grpcio-status==1.56.2
 grpcio==1.56.2
 grpcio==1.56.2
 httplib2==0.22.0
 idna==3.4
 idna==3.4
 packaging==23.1
-packaging==23.1
 proto-plus==1.22.3
 proto-plus==1.22.3
 protobuf==4.24.0
 protobuf==4.24.0
 pyasn1-modules==0.3.0
 pyasn1-modules==0.3.0
 pyasn1==0.5.0
 pyasn1==0.5.0
 pybigquery==0.5.0
 pyparsing==3.1.1
 python-dateutil==2.8.2
-python-dateutil==2.8.2
 requests==2.31.0
 requests==2.31.0
 rsa==4.9
 rsa==4.9
 six==1.16.0
 six==1.16.0
 sqlalchemy==1.4.49
+typing-extensions==4.7.1
 uritemplate==4.1.1
 urllib3==1.26.16
 urllib3==1.26.16
 
+[databricks]
+certifi==2023.7.22
+charset-normalizer==3.2.0
+databricks-sql-connector==2.9.6
+et-xmlfile==1.1.0
+greenlet==2.0.2
+idna==3.4
+lz4==4.3.3
+numpy==1.25.2
+oauthlib==3.2.2
+openpyxl==3.1.2
+pandas==2.0.3
+pyarrow==14.0.2
+python-dateutil==2.8.2
+pytz==2023.3
+requests==2.31.0
+six==1.16.0
+sqlalchemy==1.4.49
+thrift==0.16.0
+typing-extensions==4.7.1
+tzdata==2023.3
+urllib3==1.26.16
+
+[db2]
+greenlet==2.0.2
+ibm-db-sa==0.4.0
+ibm_db==3.2.3
+sqlalchemy==1.4.49
+typing-extensions==4.7.1
+
+[dynamodb]
+PyDynamoDB==0.5.7
+boto3==1.28.22
+botocore==1.31.22
+jmespath==1.0.1
+pyparsing==3.1.1
+python-dateutil==2.8.2
+s3transfer==0.6.1
+six==1.16.0
+tenacity==8.3.0
+urllib3==1.26.16
+
 [gcp]
 cachetools==5.3.1
 certifi==2023.7.22
 charset-normalizer==3.2.0
-future==0.18.3
 google-api-core==2.11.1
 google-api-python-client==2.96.0
 google-auth-httplib2==0.1.0
 google-auth==2.22.0
-google-cloud-core==2.3.3
 google-cloud-secret-manager==2.16.3
-google-crc32c==1.5.0
-google-resumable-media==2.5.0
 googleapis-common-protos==1.60.0
 grpc-google-iam-v1==0.12.6
 grpcio-status==1.56.2
 grpcio==1.56.2
 httplib2==0.22.0
 idna==3.4
-packaging==23.1
 proto-plus==1.22.3
 protobuf==4.24.0
 pyasn1-modules==0.3.0
 pyasn1==0.5.0
 pyparsing==3.1.1
-python-dateutil==2.8.2
 requests==2.31.0
 rsa==4.9
 six==1.16.0
 uritemplate==4.1.1
 urllib3==1.26.16
 
 [mariadb]
-greenlet==2.0.2
 pymysql==1.1.0
-sqlalchemy==1.4.49
 
 [mysql]
-greenlet==2.0.2
 pymysql==1.1.0
-sqlalchemy==1.4.49
 
 [postgres]
-greenlet==2.0.2
 psycopg2-binary==2.9.7
-sqlalchemy==1.4.49
 
 [redshift]
-greenlet==2.0.2
 psycopg2-binary==2.9.7
-sqlalchemy==1.4.49
 
 [s3select]
 boto3==1.28.22
 botocore==1.31.22
 jmespath==1.0.1
+python-dateutil==2.8.2
 s3transfer==0.6.1
+six==1.16.0
 urllib3==1.26.16
 
 [salesforce]
 attrs==23.1.0
 certifi==2023.7.22
 cffi==1.15.1
 charset-normalizer==3.2.0
 cryptography==41.0.3
 idna==3.4
 isodate==0.6.1
 lxml==4.9.3
 platformdirs==3.8.1
 pycparser==2.21
 pyjwt==2.8.0
+pytz==2023.3
 requests-file==1.5.1
 requests-toolbelt==1.0.0
 requests==2.31.0
-requests==2.31.0
 simple-salesforce==1.12.4
 six==1.16.0
 urllib3==1.26.16
 zeep==4.2.1
 
 [snowflake]
 asn1crypto==1.5.1
@@ -268,21 +323,22 @@
 filelock==3.12.2
 greenlet==2.0.2
 idna==3.4
 oscrypto==1.3.0
 packaging==23.1
 platformdirs==3.8.1
 pyOpenSSL==23.2.0
+pycparser==2.21
 pycryptodomex==3.18.0
 pyjwt==2.8.0
+pyjwt==2.8.0
 requests==2.31.0
 snowflake-connector-python==3.1.0
 snowflake-sqlalchemy==1.4.7
 sortedcontainers==2.4.0
 sqlalchemy==1.4.49
 tomlkit==0.12.1
 typing-extensions==4.7.1
 urllib3==1.26.16
 
-[sqlite]
-greenlet==2.0.2
-sqlalchemy==1.4.49
+[synapse]
+pyodbc==5.1.0
```

### Comparing `connector-factory-0.0.2/setup.py` & `connector-factory-0.0.3/setup.py`

 * *Files 23% similar despite different names*

```diff
@@ -1,13 +1,14 @@
 #!/usr/bin/env python
 
 """
 Prerequesites -
   Python Packages:
     * setuptools
+    * wheel
     * GitPython
   System Packages:
     * make
     * Python 3
 Commands: python setup.py [bdist_wheel / [sdist [--format=[gztar][,tar]]]
 Ex:
   * python setup.py bdist_wheel
@@ -20,227 +21,261 @@
 """
 
 """
 distutils/setuptools install script.
 """
 
 
-from setuptools import setup, find_packages
+from setuptools import setup
+from setuptools import find_packages
+from setuptools import Command
+from textwrap import wrap
 import traceback
 import shutil
 import re
 import os
 import sys
 __NAME__ = "connector-factory"
 
 ROOT = os.path.dirname(os.path.abspath(__file__))
 VERSION_FILE = os.path.join(ROOT, __NAME__.replace("-", "_"), ".version")
 VERSION_RE = re.compile(r'''__version__ = ['"]([0-9.]+)['"]''')
 python_version = f"{sys.version_info[0]}.{sys.version_info[1]}"
 
 base = [
     # Powerful data structures for data analysis, time series, and statistics
-    "pandas==2.0.3"
-]
-
-dependencies_base = [
-    "pytz==2023.3",
-    "python-dateutil==2.8.2",
-    "tzdata==2023.3",
+    "pandas==2.0.3",
+    # Database Abstraction Library
+    "sqlalchemy==1.4.49",
+    "greenlet==2.0.2",
     "numpy==1.24.4" if python_version in [
         "3.8"] else "numpy==1.25.2" if python_version in [
             "3.9", "3.10", "3.11"] else "numpy",
-    "six==1.16.0"
-]
-
-rds_type = [
-    # Database Abstraction Library
-    "sqlalchemy==1.4.49"
-]
-
-dependencies_rds_type = [
-    "greenlet==2.0.2"
+    "python-dateutil==2.8.2",
+    "pytz==2023.3",
+    "six==1.16.0",
+    "tzdata==2023.3"
 ]
 
 aws = s3select = [
     # The AWS SDK for Python
-    "boto3==1.28.22"
-]
-
-dependencies_aws = [
+    "boto3==1.28.22",
     "botocore==1.31.22",
     "jmespath==1.0.1",
+    "python-dateutil==2.8.2",
     "s3transfer==0.6.1",
-    "urllib3==1.26.16",
+    "six==1.16.0",
+    "urllib3==1.26.16"
 ]
 
 gcp = [
     # This library simplifies using Google’s various server-to-server authentication mechanisms to access Google APIs.
     "google-auth==2.22.0",
     # This library provides an httplib2 transport for google-auth.
     "google-auth-httplib2==0.1.0",
     # Google API Client Library for Python
     "google-api-python-client==2.96.0",
     # Google Secret Manager API API client library
-    "google-cloud-secret-manager==2.16.3"
-]
-
-
-dependencies_gcp = [
+    "google-cloud-secret-manager==2.16.3",
     "cachetools==5.3.1",
+    "certifi==2023.7.22",
+    "charset-normalizer==3.2.0",
+    "google-api-core==2.11.1",
+    "googleapis-common-protos==1.60.0",
+    "grpc-google-iam-v1==0.12.6",
+    "grpcio==1.56.2",
+    "grpcio-status==1.56.2",
+    "httplib2==0.22.0",
+    "idna==3.4",
+    "proto-plus==1.22.3",
+    "protobuf==4.24.0",
     "pyasn1==0.5.0",
     "pyasn1-modules==0.3.0",
-    "rsa==4.9",
-    "urllib3==1.26.16",
-    "six==1.16.0",
-    "httplib2==0.22.0",
     "pyparsing==3.1.1",
-    "python-dateutil==2.8.2",
-    "protobuf==4.24.0",
-    "packaging==23.1",
-    "idna==3.4",
-    "grpcio==1.56.2",
-    "google-crc32c==1.5.0",
-    "charset-normalizer==3.2.0",
-    "certifi==2023.7.22",
     "requests==2.31.0",
-    "proto-plus==1.22.3",
-    "googleapis-common-protos==1.60.0",
-    "google-resumable-media==2.5.0",
-    "grpcio-status==1.56.2",
-    "google-api-core==2.11.1",
-    "google-cloud-core==2.3.3",
+    "rsa==4.9",
+    "six==1.16.0",
     "uritemplate==4.1.1",
-    "grpc-google-iam-v1==0.12.6",
-    "future==0.18.3"
+    "urllib3==1.26.16"
 ]
 
 bigquery = [
     # SQLAlchemy dialect for BigQuery
     "pybigquery==0.10.2" if python_version in [
         "3.8", "3.9"] else "pybigquery==0.5.0" if python_version in [
-            "3.10", "3.11"] else "pybigquery"
-]
-
-dependencies_bigquery = [
+            "3.10", "3.11"] else "pybigquery",
+    "sqlalchemy==1.4.49",
+    "cachetools==5.3.1",
+    "certifi==2023.7.22",
+    "charset-normalizer==3.2.0",
     "future==0.18.3",
-    "google-cloud-bigquery==3.11.4",
     "google-api-core==2.11.1",
-    "python-dateutil==2.8.2",
-    "google-resumable-media==2.5.0",
-    "grpcio==1.56.2",
-    "proto-plus==1.22.3",
-    "protobuf==4.24.0",
-    "google-cloud-core==2.3.3",
-    "packaging==23.1",
-    "requests==2.31.0",
-    "greenlet==2.0.2",
     "google-auth==2.22.0",
+    "google-cloud-bigquery==3.11.4",
+    "google-cloud-core==2.3.3",
+    "google-resumable-media==2.5.0",
     "googleapis-common-protos==1.60.0",
+    "google-crc32c==1.5.0",
+    "greenlet==2.0.2",
+    "grpcio==1.56.2",
     "grpcio-status==1.56.2",
-    "six==1.16.0",
-    "certifi==2023.7.22",
     "idna==3.4",
-    "urllib3==1.26.16",
-    "charset-normalizer==3.2.0",
+    "packaging==23.1",
+    "proto-plus==1.22.3",
+    "protobuf==4.24.0",
+    "pyasn1==0.5.0",
     "pyasn1-modules==0.3.0",
-    "cachetools==5.3.1",
+    "python-dateutil==2.8.2",
+    "requests==2.31.0",
     "rsa==4.9",
-    "pyasn1==0.5.0",
+    "six==1.16.0",
+    "typing-extensions==4.7.1",
+    "urllib3==1.26.16"
 ]
 
 snowflake = [
     # Snowflake Connector Library
     "snowflake-connector-python==3.1.0",
     # Snowflake SQLAlchemy Dialect
     "snowflake-sqlalchemy==1.4.7",
-    # cryptography is a package which provides cryptographic recipes and primitives.
-    "cryptography==41.0.3"
-]
-
-dependencies_snowflake = [
     "pyjwt==2.8.0",
-    "packaging==23.1",
+    "sqlalchemy==1.4.49",
+    "asn1crypto==1.5.1",
+    "certifi==2023.7.22",
+    "cffi==1.15.1",
+    "charset-normalizer==3.2.0",
+    "cryptography==41.0.3",
     "filelock==3.12.2",
+    "greenlet==2.0.2",
+    "idna==3.4",
+    "oscrypto==1.3.0",
+    "packaging==23.1",
     "platformdirs==3.8.1",
-    "urllib3==1.26.16",
+    "pyOpenSSL==23.2.0",
+    "pycparser==2.21",
     "pycryptodomex==3.18.0",
-    "certifi==2023.7.22",
+    "pyjwt==2.8.0",
+    "requests==2.31.0",
     "sortedcontainers==2.4.0",
-    "charset-normalizer==3.2.0",
-    "asn1crypto==1.5.1",
-    "pyOpenSSL==23.2.0",
     "tomlkit==0.12.1",
-    "idna==3.4",
-    "requests==2.31.0",
-    "oscrypto==1.3.0",
     "typing-extensions==4.7.1",
-    "cffi==1.15.1"
+    "urllib3==1.26.16"
 ]
 
 redshift = postgres = [
     # PostgreSQL interface library.
     "psycopg2-binary==2.9.7"
 ]
 
-
 mysql = [
     # Pure Python MySQL Driver
     "pymysql==1.1.0"
 ]
 
-
 salesforce = [
     # A basic Salesforce.com REST API client.
     "simple-salesforce==1.12.4",
-    # Python HTTP for Humans.
-    "requests==2.31.0"
-]
-
-dependencies_salesforce = [
     "pyjwt==2.8.0",
+    "attrs==23.1.0",
+    "certifi==2023.7.22",
+    "cffi==1.15.1",
+    "charset-normalizer==3.2.0",
     "cryptography==41.0.3",
-    "zeep==4.2.1",
+    "idna==3.4",
+    "isodate==0.6.1",
+    "lxml==4.9.3",
+    "platformdirs==3.8.1",
+    "pycparser==2.21",
+    "pytz==2023.3",
     "requests==2.31.0",
-    "charset-normalizer==3.2.0",
+    "requests-file==1.5.1",
+    "requests-toolbelt==1.0.0",
+    "six==1.16.0",
     "urllib3==1.26.16",
+    "zeep==4.2.1"
+]
+
+databricks = [
+    "databricks-sql-connector==2.9.6",
     "certifi==2023.7.22",
+    "sqlalchemy==1.4.49",
+    "charset-normalizer==3.2.0",
+    "et-xmlfile==1.1.0",
+    "greenlet==2.0.2",
     "idna==3.4",
-    "cffi==1.15.1",
-    "platformdirs==3.8.1",
-    "lxml==4.9.3",
-    "requests-toolbelt==1.0.0",
-    "requests-file==1.5.1",
-    "isodate==0.6.1",
-    "attrs==23.1.0",
-    "pycparser==2.21",
-    "six==1.16.0"
+    "lz4==4.3.3",
+    "numpy==1.24.4" if python_version in [
+        "3.8"] else "numpy==1.25.2" if python_version in [
+            "3.9", "3.10", "3.11"] else "numpy",
+    "oauthlib==3.2.2",
+    "openpyxl==3.1.2",
+    "pandas==2.0.3",
+    "pyarrow==14.0.2",
+    "python-dateutil==2.8.2",
+    "pytz==2023.3",
+    "six==1.16.0",
+    "requests==2.31.0",
+    "typing-extensions==4.7.1",
+    "tzdata==2023.3",
+    "urllib3==1.26.16",
+    "thrift==0.16.0"
 ]
 
+synapse = [
+    "pyodbc==5.1.0"
+]
 
-setups = []
+db2 = [
+    "ibm-db-sa==0.4.0",
+    "ibm_db==3.2.3",
+    "sqlalchemy==1.4.49",
+    "greenlet==2.0.2",
+    "typing-extensions==4.7.1",
+]
+
+dynamodb = [
+    "PyDynamoDB==0.5.7",
+    "boto3==1.28.22",
+    "botocore==1.31.22",
+    "jmespath==1.0.1",
+    "pyparsing==3.1.1",
+    "python-dateutil==2.8.2",
+    "s3transfer==0.6.1",
+    "six==1.16.0",
+    "tenacity==8.3.0",
+    "urllib3==1.26.16"
+]
+
+
+setups = [
+    'gitpython',
+    'setuptools',
+    'wheel'
+]
 
 
-extra_dependencies = {
-    "sqlite": (rds_type + dependencies_rds_type),
-    "snowflake": (rds_type + dependencies_rds_type + snowflake + dependencies_snowflake),
-    "aws": (aws + dependencies_aws),
-    "s3select": (aws + dependencies_aws),
-    "postgres": (rds_type + dependencies_rds_type + postgres),
-    "redshift": (rds_type + dependencies_rds_type + redshift),
-    "mysql": (rds_type + dependencies_rds_type + mysql),
-    "mariadb": (rds_type + dependencies_rds_type + mysql),
-    "salesforce": (salesforce + dependencies_salesforce),
-    "gcp": (gcp + dependencies_gcp),
-    "bigquery": (gcp + dependencies_gcp + bigquery + dependencies_bigquery + rds_type + dependencies_rds_type),
-    "all": (rds_type + dependencies_rds_type + snowflake + dependencies_snowflake + aws + dependencies_aws + postgres + redshift + mysql + salesforce + dependencies_salesforce + gcp + dependencies_gcp + bigquery + dependencies_bigquery)
+extras = {
+    "snowflake": snowflake,
+    "aws": aws,
+    "s3select": aws,
+    "postgres": postgres,
+    "redshift": redshift,
+    "mysql": mysql,
+    "mariadb": mysql,
+    "salesforce": salesforce,
+    "databricks": databricks,
+    "gcp": gcp,
+    "bigquery": (gcp + bigquery),
+    "synapse": synapse,
+    "db2": db2,
+    "dynamodb": dynamodb,
+    "all": (snowflake + aws + postgres + redshift + mysql + salesforce + gcp + bigquery + databricks + synapse + db2)
 }
 
-ir = (base + dependencies_base + extra_dependencies["sqlite"])
-install_requires = ir
+install_requires = base
 
 
 def delete(path):
     if os.path.exists(path=path):
         try:
             if os.path.isfile(path=path):
                 os.remove(path=path)
@@ -290,14 +325,34 @@
     return version
 
 
 with open("README.md", "r") as f:
     long_description = f.read()
 
 
+class List_Extras(Command):
+    """
+    List all available extras
+    Registered as cmdclass in setup() so it can be called with ``python setup.py list_extras``.
+    """
+
+    description = "List available extras"
+    user_options = []
+
+    def initialize_options(self):
+        """Set default values for options."""
+
+    def finalize_options(self):
+        """Set final values for options."""
+
+    def run(self):
+        """List extras."""
+        print("\n".join(wrap(", ".join(extras.keys()), 100)))
+
+
 def do_setup():
     setup(
         name=__NAME__,
         version=get_version(filename=VERSION_FILE),
         description="Connector Factory;",
         long_description=long_description,
         long_description_content_type="text/markdown",
@@ -306,18 +361,21 @@
                   "snowflake", "bigquery", "gcp", "aws", "s3select", "salesforce"],
         author="Ankit Shrivastava",
         url="https://github.com/shrivastava-v-ankit/connector-factory",
         packages=find_packages(include=[__NAME__.replace("-", "_")]),
         include_package_data=True,
         setup_requires=setups,
         install_requires=install_requires,
-        extras_require=extra_dependencies,
+        extras_require=extras,
         license="MIT",
         python_requires=">=3.8, <3.12",
         platforms="any",
+        cmdclass={
+            'list_extras': List_Extras,
+        },
         project_urls={
             "Source": "https://github.com/shrivastava-v-ankit/connector-factory/",
             "Tracker": "https://github.com/shrivastava-v-ankit/connector-factory/issues",
         },
         classifiers=[
             "Development Status :: 5 - Production/Stable",
             "Environment :: Web Environment",
```

