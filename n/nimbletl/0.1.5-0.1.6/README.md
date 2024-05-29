# Comparing `tmp/nimbletl-0.1.5.tar.gz` & `tmp/nimbletl-0.1.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "nimbletl-0.1.5.tar", last modified: Tue May 28 08:49:04 2024, max compression
+gzip compressed data, was "nimbletl-0.1.6.tar", last modified: Wed May 29 03:05:31 2024, max compression
```

## Comparing `nimbletl-0.1.5.tar` & `nimbletl-0.1.6.tar`

### file list

```diff
@@ -1,18 +1,23 @@
-drwxr-xr-x   0 xiaoqiangma   (501) staff       (20)        0 2024-05-28 08:49:04.431060 nimbletl-0.1.5/
--rw-r--r--   0 xiaoqiangma   (501) staff       (20)      510 2024-05-28 08:49:04.430747 nimbletl-0.1.5/PKG-INFO
--rw-r--r--   0 xiaoqiangma   (501) staff       (20)      217 2024-05-28 06:32:53.000000 nimbletl-0.1.5/README.md
-drwxr-xr-x   0 xiaoqiangma   (501) staff       (20)        0 2024-05-28 08:49:04.427521 nimbletl-0.1.5/log_driver/
--rw-r--r--   0 xiaoqiangma   (501) staff       (20)        0 2024-05-28 03:12:18.000000 nimbletl-0.1.5/log_driver/__init__.py
-drwxr-xr-x   0 xiaoqiangma   (501) staff       (20)        0 2024-05-28 08:49:04.428511 nimbletl-0.1.5/log_driver/init/
--rw-r--r--   0 xiaoqiangma   (501) staff       (20)        0 2024-05-28 03:12:25.000000 nimbletl-0.1.5/log_driver/init/__init__.py
--rw-r--r--   0 xiaoqiangma   (501) staff       (20)      778 2024-05-28 08:46:37.000000 nimbletl-0.1.5/log_driver/init/cli.py
--rw-r--r--   0 xiaoqiangma   (501) staff       (20)     1365 2024-05-28 06:44:00.000000 nimbletl-0.1.5/log_driver/init/db.py
-drwxr-xr-x   0 xiaoqiangma   (501) staff       (20)        0 2024-05-28 08:49:04.430400 nimbletl-0.1.5/nimbletl.egg-info/
--rw-r--r--   0 xiaoqiangma   (501) staff       (20)      510 2024-05-28 08:49:04.000000 nimbletl-0.1.5/nimbletl.egg-info/PKG-INFO
--rw-r--r--   0 xiaoqiangma   (501) staff       (20)      308 2024-05-28 08:49:04.000000 nimbletl-0.1.5/nimbletl.egg-info/SOURCES.txt
--rw-r--r--   0 xiaoqiangma   (501) staff       (20)        1 2024-05-28 08:49:04.000000 nimbletl-0.1.5/nimbletl.egg-info/dependency_links.txt
--rw-r--r--   0 xiaoqiangma   (501) staff       (20)       54 2024-05-28 08:49:04.000000 nimbletl-0.1.5/nimbletl.egg-info/entry_points.txt
--rw-r--r--   0 xiaoqiangma   (501) staff       (20)       57 2024-05-28 08:49:04.000000 nimbletl-0.1.5/nimbletl.egg-info/requires.txt
--rw-r--r--   0 xiaoqiangma   (501) staff       (20)       11 2024-05-28 08:49:04.000000 nimbletl-0.1.5/nimbletl.egg-info/top_level.txt
--rw-r--r--   0 xiaoqiangma   (501) staff       (20)       38 2024-05-28 08:49:04.431128 nimbletl-0.1.5/setup.cfg
--rw-r--r--   0 xiaoqiangma   (501) staff       (20)      742 2024-05-28 08:48:34.000000 nimbletl-0.1.5/setup.py
+drwxr-xr-x   0 xiaoqiangma   (501) staff       (20)        0 2024-05-29 03:05:31.969395 nimbletl-0.1.6/
+-rw-r--r--   0 xiaoqiangma   (501) staff       (20)      742 2024-05-29 03:05:31.969140 nimbletl-0.1.6/PKG-INFO
+-rw-r--r--   0 xiaoqiangma   (501) staff       (20)      217 2024-05-28 06:32:53.000000 nimbletl-0.1.6/README.md
+drwxr-xr-x   0 xiaoqiangma   (501) staff       (20)        0 2024-05-29 03:05:31.966060 nimbletl-0.1.6/common/
+-rw-r--r--   0 xiaoqiangma   (501) staff       (20)        0 2024-05-29 02:16:50.000000 nimbletl-0.1.6/common/__init__.py
+-rw-r--r--   0 xiaoqiangma   (501) staff       (20)     1168 2024-05-29 03:05:20.000000 nimbletl-0.1.6/common/db.py
+drwxr-xr-x   0 xiaoqiangma   (501) staff       (20)        0 2024-05-29 03:05:31.966373 nimbletl-0.1.6/log_driver/
+-rw-r--r--   0 xiaoqiangma   (501) staff       (20)        0 2024-05-28 03:12:18.000000 nimbletl-0.1.6/log_driver/__init__.py
+drwxr-xr-x   0 xiaoqiangma   (501) staff       (20)        0 2024-05-29 03:05:31.967378 nimbletl-0.1.6/log_driver/init/
+-rw-r--r--   0 xiaoqiangma   (501) staff       (20)       98 2024-05-29 02:57:33.000000 nimbletl-0.1.6/log_driver/init/__init__.py
+-rw-r--r--   0 xiaoqiangma   (501) staff       (20)      904 2024-05-29 03:05:20.000000 nimbletl-0.1.6/log_driver/init/cli.py
+-rw-r--r--   0 xiaoqiangma   (501) staff       (20)      136 2024-05-29 03:01:15.000000 nimbletl-0.1.6/log_driver/init/init_drive_db.py
+-rw-r--r--   0 xiaoqiangma   (501) staff       (20)      465 2024-05-29 02:44:32.000000 nimbletl-0.1.6/log_driver/init/load_config_to_env.py
+-rw-r--r--   0 xiaoqiangma   (501) staff       (20)        0 2024-05-29 02:13:14.000000 nimbletl-0.1.6/log_driver/time_windows.py
+drwxr-xr-x   0 xiaoqiangma   (501) staff       (20)        0 2024-05-29 03:05:31.968842 nimbletl-0.1.6/nimbletl.egg-info/
+-rw-r--r--   0 xiaoqiangma   (501) staff       (20)      742 2024-05-29 03:05:31.000000 nimbletl-0.1.6/nimbletl.egg-info/PKG-INFO
+-rw-r--r--   0 xiaoqiangma   (501) staff       (20)      416 2024-05-29 03:05:31.000000 nimbletl-0.1.6/nimbletl.egg-info/SOURCES.txt
+-rw-r--r--   0 xiaoqiangma   (501) staff       (20)        1 2024-05-29 03:05:31.000000 nimbletl-0.1.6/nimbletl.egg-info/dependency_links.txt
+-rw-r--r--   0 xiaoqiangma   (501) staff       (20)       54 2024-05-29 03:05:31.000000 nimbletl-0.1.6/nimbletl.egg-info/entry_points.txt
+-rw-r--r--   0 xiaoqiangma   (501) staff       (20)      184 2024-05-29 03:05:31.000000 nimbletl-0.1.6/nimbletl.egg-info/requires.txt
+-rw-r--r--   0 xiaoqiangma   (501) staff       (20)       18 2024-05-29 03:05:31.000000 nimbletl-0.1.6/nimbletl.egg-info/top_level.txt
+-rw-r--r--   0 xiaoqiangma   (501) staff       (20)       38 2024-05-29 03:05:31.969454 nimbletl-0.1.6/setup.cfg
+-rw-r--r--   0 xiaoqiangma   (501) staff       (20)      742 2024-05-29 03:05:20.000000 nimbletl-0.1.6/setup.py
```

### Comparing `nimbletl-0.1.5/log_driver/init/db.py` & `nimbletl-0.1.6/common/db.py`

 * *Files 24% similar despite different names*

```diff
@@ -1,40 +1,43 @@
-import click
-import mysql.connector
-from mysql.connector import errorcode
+import os
 
+import pandas as pd
+from sqlalchemy import create_engine
+from sqlalchemy.exc import SQLAlchemyError
 
-def initialize_database(config):
-    click.echo("""Log table creation...""")
-    db_config = config.get('database', {})
+
+def _get_drive_db_url():
+    db_user = os.getenv('LOG_DRIVE_DB_USER', 'root')
+    db_password = os.getenv('LOG_DRIVE_DB_PASSWORD', '')
+    db_host = os.getenv('LOG_DRIVE_DB_HOST', 'localhost')
+    db_port = os.getenv('LOG_DRIVE_DB_PORT', '3306')
+    db_name = os.getenv('LOG_DRIVE_DB_NAME', 'nimbletl')
+
+    return f'mysql+mysqldb://{db_user}:{db_password}@{db_host}:{db_port}/{db_name}?charset=utf8'
+
+
+def _get_engine():
+    return create_engine(_get_drive_db_url())
+
+
+def get_dataframe(sql_str):
+    try:
+        connection = _get_engine().connect()
+        df = pd.read_sql(sql_str, connection)
+        return df
+    except SQLAlchemyError as e:
+        print(f"Error occurred: {e}")
+    finally:
+        if connection:
+            connection.close()
+
+
+def execute_sql(sql_str):
     try:
-        connection = mysql.connector.connect(
-            host=db_config.get('host', 'localhost'),
-            user=db_config.get('user', 'root'),
-            password=db_config.get('password', ''),
-            database=db_config.get('database', '')
-        )
-        cursor = connection.cursor()
-
-        # Example: Create a sample table
-        cursor.execute("""
-            CREATE TABLE IF NOT EXISTS example_table (
-                id INT AUTO_INCREMENT PRIMARY KEY,
-                name VARCHAR(100) NOT NULL,
-                created_at TIMESTAMP DEFAULT CURRENT_TIMESTAMP
-            );
-        """)
-
-        connection.commit()
-        cursor.close()
-        connection.close()
-        print("Database initialized successfully.")
-    except mysql.connector.Error as err:
-        if err.errno == errorcode.ER_ACCESS_DENIED_ERROR:
-            print("Error: Something is wrong with your user name or password")
-        elif err.errno == errorcode.ER_BAD_DB_ERROR:
-            print("Error: Database does not exist")
-        else:
-            print(err)
-    else:
-        connection.close()
-        click.echo("""The log table is created successfully.""")
+        connection = _get_engine().connect()
+        connection.execute(sql_str)
+        print("Table created successfully.")
+    except SQLAlchemyError as e:
+        print(f"Error occurred: {e}")
+    finally:
+        if connection:
+            connection.close()
```

### Comparing `nimbletl-0.1.5/setup.py` & `nimbletl-0.1.6/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -8,15 +8,15 @@
         lock_data = json.load(f)
     dependencies = lock_data['default']
     return [f"{pkg}{info.get('version', '')}" for pkg, info in dependencies.items()]
 
 
 setuptools.setup(
     name='nimbletl',
-    version='0.1.5',
+    version='0.1.6',
     packages=setuptools.find_packages(),
     install_requires=parse_pipfile_lock(),
     entry_points={
         'console_scripts': [
             'nimbletl=log_driver.init.cli:main',
         ],
     },
```

