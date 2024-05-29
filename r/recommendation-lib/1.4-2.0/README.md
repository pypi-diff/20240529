# Comparing `tmp/recommendation_lib-1.4.tar.gz` & `tmp/recommendation_lib-2.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "recommendation_lib-1.4.tar", last modified: Wed May 29 08:27:10 2024, max compression
+gzip compressed data, was "recommendation_lib-2.0.tar", last modified: Wed May 29 09:21:02 2024, max compression
```

## Comparing `recommendation_lib-1.4.tar` & `recommendation_lib-2.0.tar`

### file list

```diff
@@ -1,36 +1,36 @@
-drwxrwxrwx   0        0        0        0 2024-05-29 08:27:10.165128 recommendation_lib-1.4/
--rw-rw-rw-   0        0        0      930 2024-05-29 08:26:36.000000 recommendation_lib-1.4/Dockerfile
--rw-rw-rw-   0        0        0       97 2024-05-29 08:10:19.000000 recommendation_lib-1.4/MANIFEST.in
--rw-rw-rw-   0        0        0      302 2024-05-29 08:27:10.161163 recommendation_lib-1.4/PKG-INFO
--rw-rw-rw-   0        0        0        0 2024-05-29 08:09:33.000000 recommendation_lib-1.4/README.md
-drwxrwxrwx   0        0        0        0 2024-05-29 08:27:10.013910 recommendation_lib-1.4/app/
--rw-rw-rw-   0        0        0        0 2024-05-29 00:52:06.000000 recommendation_lib-1.4/app/__init__.py
-drwxrwxrwx   0        0        0        0 2024-05-29 08:27:10.024910 recommendation_lib-1.4/app/core/
--rw-rw-rw-   0        0        0        0 2024-05-29 07:59:28.000000 recommendation_lib-1.4/app/core/__init__.py
--rw-rw-rw-   0        0        0     2974 2024-05-29 08:05:28.000000 recommendation_lib-1.4/app/core/main.py
-drwxrwxrwx   0        0        0        0 2024-05-29 08:27:10.063466 recommendation_lib-1.4/app/data/
--rw-rw-rw-   0        0        0        0 2024-05-29 07:54:55.000000 recommendation_lib-1.4/app/data/__init__.py
--rw-rw-rw-   0        0        0  4540272 2024-05-29 00:57:54.000000 recommendation_lib-1.4/app/data/content_owns.csv
--rw-rw-rw-   0        0        0  4715753 2024-05-26 12:29:21.000000 recommendation_lib-1.4/app/data/machine_ratings.csv
--rw-rw-rw-   0        0        0   422045 2024-05-26 12:29:25.000000 recommendation_lib-1.4/app/data/machines.csv
-drwxrwxrwx   0        0        0        0 2024-05-29 08:27:10.076877 recommendation_lib-1.4/app/general_tools/
--rw-rw-rw-   0        0        0        0 2024-05-27 22:28:14.000000 recommendation_lib-1.4/app/general_tools/__init__.py
--rw-rw-rw-   0        0        0      785 2024-05-26 13:37:53.000000 recommendation_lib-1.4/app/general_tools/logger.py
-drwxrwxrwx   0        0        0        0 2024-05-29 08:27:10.093127 recommendation_lib-1.4/app/postgres/
--rw-rw-rw-   0        0        0        0 2024-05-27 22:28:25.000000 recommendation_lib-1.4/app/postgres/__init__.py
--rw-rw-rw-   0        0        0     3805 2024-05-29 08:04:57.000000 recommendation_lib-1.4/app/postgres/functions.py
--rw-rw-rw-   0        0        0     1436 2024-05-28 17:21:25.000000 recommendation_lib-1.4/app/postgres/table_class.py
-drwxrwxrwx   0        0        0        0 2024-05-29 08:27:10.101127 recommendation_lib-1.4/app/preprocessing/
--rw-rw-rw-   0        0        0        0 2024-05-27 22:28:34.000000 recommendation_lib-1.4/app/preprocessing/__init__.py
--rw-rw-rw-   0        0        0     2941 2024-05-28 22:05:36.000000 recommendation_lib-1.4/app/preprocessing/preprocess.py
-drwxrwxrwx   0        0        0        0 2024-05-29 08:27:10.112176 recommendation_lib-1.4/app/recommendation/
--rw-rw-rw-   0        0        0        0 2024-05-27 22:33:29.000000 recommendation_lib-1.4/app/recommendation/__init__.py
--rw-rw-rw-   0        0        0     1520 2024-05-28 23:44:52.000000 recommendation_lib-1.4/app/recommendation/recommendation.py
-drwxrwxrwx   0        0        0        0 2024-05-29 08:27:10.156135 recommendation_lib-1.4/recommendation_lib.egg-info/
--rw-rw-rw-   0        0        0      302 2024-05-29 08:27:09.000000 recommendation_lib-1.4/recommendation_lib.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      645 2024-05-29 08:27:09.000000 recommendation_lib-1.4/recommendation_lib.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-05-29 08:27:09.000000 recommendation_lib-1.4/recommendation_lib.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0        4 2024-05-29 08:27:09.000000 recommendation_lib-1.4/recommendation_lib.egg-info/top_level.txt
--rw-rw-rw-   0        0        0      155 2024-05-29 08:21:27.000000 recommendation_lib-1.4/requirements.txt
--rw-rw-rw-   0        0        0       42 2024-05-29 08:27:10.166218 recommendation_lib-1.4/setup.cfg
--rw-rw-rw-   0        0        0      546 2024-05-29 08:26:53.000000 recommendation_lib-1.4/setup.py
+drwxrwxrwx   0        0        0        0 2024-05-29 09:21:02.849852 recommendation_lib-2.0/
+-rw-rw-rw-   0        0        0     1521 2024-05-29 09:16:44.000000 recommendation_lib-2.0/Dockerfile
+-rw-rw-rw-   0        0        0       97 2024-05-29 08:10:19.000000 recommendation_lib-2.0/MANIFEST.in
+-rw-rw-rw-   0        0        0      302 2024-05-29 09:21:02.845836 recommendation_lib-2.0/PKG-INFO
+-rw-rw-rw-   0        0        0        0 2024-05-29 08:09:33.000000 recommendation_lib-2.0/README.md
+drwxrwxrwx   0        0        0        0 2024-05-29 09:21:02.664404 recommendation_lib-2.0/app/
+-rw-rw-rw-   0        0        0        0 2024-05-29 00:52:06.000000 recommendation_lib-2.0/app/__init__.py
+drwxrwxrwx   0        0        0        0 2024-05-29 09:21:02.679948 recommendation_lib-2.0/app/core/
+-rw-rw-rw-   0        0        0        0 2024-05-29 07:59:28.000000 recommendation_lib-2.0/app/core/__init__.py
+-rw-rw-rw-   0        0        0     2969 2024-05-29 09:17:38.000000 recommendation_lib-2.0/app/core/main.py
+drwxrwxrwx   0        0        0        0 2024-05-29 09:21:02.736665 recommendation_lib-2.0/app/data/
+-rw-rw-rw-   0        0        0        0 2024-05-29 07:54:55.000000 recommendation_lib-2.0/app/data/__init__.py
+-rw-rw-rw-   0        0        0  4540272 2024-05-29 00:57:54.000000 recommendation_lib-2.0/app/data/content_owns.csv
+-rw-rw-rw-   0        0        0  4715753 2024-05-26 12:29:21.000000 recommendation_lib-2.0/app/data/machine_ratings.csv
+-rw-rw-rw-   0        0        0   422045 2024-05-26 12:29:25.000000 recommendation_lib-2.0/app/data/machines.csv
+drwxrwxrwx   0        0        0        0 2024-05-29 09:21:02.748705 recommendation_lib-2.0/app/general_tools/
+-rw-rw-rw-   0        0        0        0 2024-05-27 22:28:14.000000 recommendation_lib-2.0/app/general_tools/__init__.py
+-rw-rw-rw-   0        0        0      785 2024-05-26 13:37:53.000000 recommendation_lib-2.0/app/general_tools/logger.py
+drwxrwxrwx   0        0        0        0 2024-05-29 09:21:02.767614 recommendation_lib-2.0/app/postgres/
+-rw-rw-rw-   0        0        0        0 2024-05-27 22:28:25.000000 recommendation_lib-2.0/app/postgres/__init__.py
+-rw-rw-rw-   0        0        0     3800 2024-05-29 09:18:13.000000 recommendation_lib-2.0/app/postgres/functions.py
+-rw-rw-rw-   0        0        0     1436 2024-05-28 17:21:25.000000 recommendation_lib-2.0/app/postgres/table_class.py
+drwxrwxrwx   0        0        0        0 2024-05-29 09:21:02.779480 recommendation_lib-2.0/app/preprocessing/
+-rw-rw-rw-   0        0        0        0 2024-05-27 22:28:34.000000 recommendation_lib-2.0/app/preprocessing/__init__.py
+-rw-rw-rw-   0        0        0     2941 2024-05-28 22:05:36.000000 recommendation_lib-2.0/app/preprocessing/preprocess.py
+drwxrwxrwx   0        0        0        0 2024-05-29 09:21:02.802595 recommendation_lib-2.0/app/recommendation/
+-rw-rw-rw-   0        0        0        0 2024-05-27 22:33:29.000000 recommendation_lib-2.0/app/recommendation/__init__.py
+-rw-rw-rw-   0        0        0     1520 2024-05-28 23:44:52.000000 recommendation_lib-2.0/app/recommendation/recommendation.py
+drwxrwxrwx   0        0        0        0 2024-05-29 09:21:02.841215 recommendation_lib-2.0/recommendation_lib.egg-info/
+-rw-rw-rw-   0        0        0      302 2024-05-29 09:21:02.000000 recommendation_lib-2.0/recommendation_lib.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      645 2024-05-29 09:21:02.000000 recommendation_lib-2.0/recommendation_lib.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-05-29 09:21:02.000000 recommendation_lib-2.0/recommendation_lib.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0        4 2024-05-29 09:21:02.000000 recommendation_lib-2.0/recommendation_lib.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0      155 2024-05-29 09:20:57.000000 recommendation_lib-2.0/requirements.txt
+-rw-rw-rw-   0        0        0       42 2024-05-29 09:21:02.849852 recommendation_lib-2.0/setup.cfg
+-rw-rw-rw-   0        0        0      546 2024-05-29 09:20:40.000000 recommendation_lib-2.0/setup.py
```

### Comparing `recommendation_lib-1.4/app/core/main.py` & `recommendation_lib-2.0/app/core/main.py`

 * *Files 1% similar despite different names*

```diff
@@ -6,15 +6,15 @@
 from sqlalchemy import create_engine
 from sqlalchemy.orm import sessionmaker
 from app.postgres.table_class import Base
 import uvicorn
 from contextlib import asynccontextmanager
 
 # Global engine and session maker
-engine = create_engine('postgresql://postgres:my_secret_password@localhost:5432/postgres')
+engine = create_engine('postgresql://gpanagou:my_secret_password@localhost:5432/htb')
 Session = sessionmaker(bind=engine)
 
 @asynccontextmanager
 async def lifespan(app: FastAPI):
 
     Base.metadata.create_all(engine)
     session = Session()
```

### Comparing `recommendation_lib-1.4/app/data/content_owns.csv` & `recommendation_lib-2.0/app/data/content_owns.csv`

 * *Files identical despite different names*

### Comparing `recommendation_lib-1.4/app/data/machine_ratings.csv` & `recommendation_lib-2.0/app/data/machine_ratings.csv`

 * *Files identical despite different names*

### Comparing `recommendation_lib-1.4/app/data/machines.csv` & `recommendation_lib-2.0/app/data/machines.csv`

 * *Files identical despite different names*

### Comparing `recommendation_lib-1.4/app/general_tools/logger.py` & `recommendation_lib-2.0/app/general_tools/logger.py`

 * *Files identical despite different names*

### Comparing `recommendation_lib-1.4/app/postgres/functions.py` & `recommendation_lib-2.0/app/postgres/functions.py`

 * *Files 1% similar despite different names*

```diff
@@ -12,16 +12,16 @@
 '''
 def connect_to_db():
     try:
         logger.info("Trying to connect to Postgres database...")
         connection = psycopg2.connect(
             host="localhost",
             port=5432,
-            database="postgres",
-            user="postgres",
+            database="htb",
+            user="gpanagou",
             password="my_secret_password"
         )
         return connection
     except psycopg2.DatabaseError as error:
         logger.error(f"Error while connecting to PostgreSQL: {error}")
         return None
```

### Comparing `recommendation_lib-1.4/app/postgres/table_class.py` & `recommendation_lib-2.0/app/postgres/table_class.py`

 * *Files identical despite different names*

### Comparing `recommendation_lib-1.4/app/preprocessing/preprocess.py` & `recommendation_lib-2.0/app/preprocessing/preprocess.py`

 * *Files identical despite different names*

### Comparing `recommendation_lib-1.4/app/recommendation/recommendation.py` & `recommendation_lib-2.0/app/recommendation/recommendation.py`

 * *Files identical despite different names*

### Comparing `recommendation_lib-1.4/recommendation_lib.egg-info/SOURCES.txt` & `recommendation_lib-2.0/recommendation_lib.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `recommendation_lib-1.4/setup.py` & `recommendation_lib-2.0/setup.py`

 * *Files 22% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 import setuptools
 
 
 setuptools.setup(
     name="recommendation_lib",
-    version="1.4",
+    version="2.0",
     author="Giorgos Panagou",
     author_email="g.panagou94@gmail.com",
     description="Package containining recommendation algorithm",
     packages= setuptools.find_packages(include=['app', 'app.*']),
     classifiers=[
         "Programming Language :: Python :: 3",
         "Operating System :: OS Independent",
```

