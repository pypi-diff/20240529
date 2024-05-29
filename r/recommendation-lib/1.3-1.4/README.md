# Comparing `tmp/recommendation_lib-1.3.tar.gz` & `tmp/recommendation_lib-1.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "recommendation_lib-1.3.tar", last modified: Wed May 29 08:18:46 2024, max compression
+gzip compressed data, was "recommendation_lib-1.4.tar", last modified: Wed May 29 08:27:10 2024, max compression
```

## Comparing `recommendation_lib-1.3.tar` & `recommendation_lib-1.4.tar`

### file list

```diff
@@ -1,36 +1,36 @@
-drwxrwxrwx   0        0        0        0 2024-05-29 08:18:46.248245 recommendation_lib-1.3/
--rw-rw-rw-   0        0        0      883 2024-05-29 01:06:20.000000 recommendation_lib-1.3/Dockerfile
--rw-rw-rw-   0        0        0       97 2024-05-29 08:10:19.000000 recommendation_lib-1.3/MANIFEST.in
--rw-rw-rw-   0        0        0      302 2024-05-29 08:18:46.244244 recommendation_lib-1.3/PKG-INFO
--rw-rw-rw-   0        0        0        0 2024-05-29 08:09:33.000000 recommendation_lib-1.3/README.md
-drwxrwxrwx   0        0        0        0 2024-05-29 08:18:46.093855 recommendation_lib-1.3/app/
--rw-rw-rw-   0        0        0        0 2024-05-29 00:52:06.000000 recommendation_lib-1.3/app/__init__.py
-drwxrwxrwx   0        0        0        0 2024-05-29 08:18:46.103235 recommendation_lib-1.3/app/core/
--rw-rw-rw-   0        0        0        0 2024-05-29 07:59:28.000000 recommendation_lib-1.3/app/core/__init__.py
--rw-rw-rw-   0        0        0     2974 2024-05-29 08:05:28.000000 recommendation_lib-1.3/app/core/main.py
-drwxrwxrwx   0        0        0        0 2024-05-29 08:18:46.145289 recommendation_lib-1.3/app/data/
--rw-rw-rw-   0        0        0        0 2024-05-29 07:54:55.000000 recommendation_lib-1.3/app/data/__init__.py
--rw-rw-rw-   0        0        0  4540272 2024-05-29 00:57:54.000000 recommendation_lib-1.3/app/data/content_owns.csv
--rw-rw-rw-   0        0        0  4715753 2024-05-26 12:29:21.000000 recommendation_lib-1.3/app/data/machine_ratings.csv
--rw-rw-rw-   0        0        0   422045 2024-05-26 12:29:25.000000 recommendation_lib-1.3/app/data/machines.csv
-drwxrwxrwx   0        0        0        0 2024-05-29 08:18:46.156798 recommendation_lib-1.3/app/general_tools/
--rw-rw-rw-   0        0        0        0 2024-05-27 22:28:14.000000 recommendation_lib-1.3/app/general_tools/__init__.py
--rw-rw-rw-   0        0        0      785 2024-05-26 13:37:53.000000 recommendation_lib-1.3/app/general_tools/logger.py
-drwxrwxrwx   0        0        0        0 2024-05-29 08:18:46.171291 recommendation_lib-1.3/app/postgres/
--rw-rw-rw-   0        0        0        0 2024-05-27 22:28:25.000000 recommendation_lib-1.3/app/postgres/__init__.py
--rw-rw-rw-   0        0        0     3805 2024-05-29 08:04:57.000000 recommendation_lib-1.3/app/postgres/functions.py
--rw-rw-rw-   0        0        0     1436 2024-05-28 17:21:25.000000 recommendation_lib-1.3/app/postgres/table_class.py
-drwxrwxrwx   0        0        0        0 2024-05-29 08:18:46.182125 recommendation_lib-1.3/app/preprocessing/
--rw-rw-rw-   0        0        0        0 2024-05-27 22:28:34.000000 recommendation_lib-1.3/app/preprocessing/__init__.py
--rw-rw-rw-   0        0        0     2941 2024-05-28 22:05:36.000000 recommendation_lib-1.3/app/preprocessing/preprocess.py
-drwxrwxrwx   0        0        0        0 2024-05-29 08:18:46.193640 recommendation_lib-1.3/app/recommendation/
--rw-rw-rw-   0        0        0        0 2024-05-27 22:33:29.000000 recommendation_lib-1.3/app/recommendation/__init__.py
--rw-rw-rw-   0        0        0     1520 2024-05-28 23:44:52.000000 recommendation_lib-1.3/app/recommendation/recommendation.py
-drwxrwxrwx   0        0        0        0 2024-05-29 08:18:46.239220 recommendation_lib-1.3/recommendation_lib.egg-info/
--rw-rw-rw-   0        0        0      302 2024-05-29 08:18:45.000000 recommendation_lib-1.3/recommendation_lib.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      645 2024-05-29 08:18:45.000000 recommendation_lib-1.3/recommendation_lib.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-05-29 08:18:45.000000 recommendation_lib-1.3/recommendation_lib.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0        4 2024-05-29 08:18:45.000000 recommendation_lib-1.3/recommendation_lib.egg-info/top_level.txt
--rw-rw-rw-   0        0        0      155 2024-05-29 08:17:23.000000 recommendation_lib-1.3/requirements.txt
--rw-rw-rw-   0        0        0       42 2024-05-29 08:18:46.248245 recommendation_lib-1.3/setup.cfg
--rw-rw-rw-   0        0        0      546 2024-05-29 08:18:40.000000 recommendation_lib-1.3/setup.py
+drwxrwxrwx   0        0        0        0 2024-05-29 08:27:10.165128 recommendation_lib-1.4/
+-rw-rw-rw-   0        0        0      930 2024-05-29 08:26:36.000000 recommendation_lib-1.4/Dockerfile
+-rw-rw-rw-   0        0        0       97 2024-05-29 08:10:19.000000 recommendation_lib-1.4/MANIFEST.in
+-rw-rw-rw-   0        0        0      302 2024-05-29 08:27:10.161163 recommendation_lib-1.4/PKG-INFO
+-rw-rw-rw-   0        0        0        0 2024-05-29 08:09:33.000000 recommendation_lib-1.4/README.md
+drwxrwxrwx   0        0        0        0 2024-05-29 08:27:10.013910 recommendation_lib-1.4/app/
+-rw-rw-rw-   0        0        0        0 2024-05-29 00:52:06.000000 recommendation_lib-1.4/app/__init__.py
+drwxrwxrwx   0        0        0        0 2024-05-29 08:27:10.024910 recommendation_lib-1.4/app/core/
+-rw-rw-rw-   0        0        0        0 2024-05-29 07:59:28.000000 recommendation_lib-1.4/app/core/__init__.py
+-rw-rw-rw-   0        0        0     2974 2024-05-29 08:05:28.000000 recommendation_lib-1.4/app/core/main.py
+drwxrwxrwx   0        0        0        0 2024-05-29 08:27:10.063466 recommendation_lib-1.4/app/data/
+-rw-rw-rw-   0        0        0        0 2024-05-29 07:54:55.000000 recommendation_lib-1.4/app/data/__init__.py
+-rw-rw-rw-   0        0        0  4540272 2024-05-29 00:57:54.000000 recommendation_lib-1.4/app/data/content_owns.csv
+-rw-rw-rw-   0        0        0  4715753 2024-05-26 12:29:21.000000 recommendation_lib-1.4/app/data/machine_ratings.csv
+-rw-rw-rw-   0        0        0   422045 2024-05-26 12:29:25.000000 recommendation_lib-1.4/app/data/machines.csv
+drwxrwxrwx   0        0        0        0 2024-05-29 08:27:10.076877 recommendation_lib-1.4/app/general_tools/
+-rw-rw-rw-   0        0        0        0 2024-05-27 22:28:14.000000 recommendation_lib-1.4/app/general_tools/__init__.py
+-rw-rw-rw-   0        0        0      785 2024-05-26 13:37:53.000000 recommendation_lib-1.4/app/general_tools/logger.py
+drwxrwxrwx   0        0        0        0 2024-05-29 08:27:10.093127 recommendation_lib-1.4/app/postgres/
+-rw-rw-rw-   0        0        0        0 2024-05-27 22:28:25.000000 recommendation_lib-1.4/app/postgres/__init__.py
+-rw-rw-rw-   0        0        0     3805 2024-05-29 08:04:57.000000 recommendation_lib-1.4/app/postgres/functions.py
+-rw-rw-rw-   0        0        0     1436 2024-05-28 17:21:25.000000 recommendation_lib-1.4/app/postgres/table_class.py
+drwxrwxrwx   0        0        0        0 2024-05-29 08:27:10.101127 recommendation_lib-1.4/app/preprocessing/
+-rw-rw-rw-   0        0        0        0 2024-05-27 22:28:34.000000 recommendation_lib-1.4/app/preprocessing/__init__.py
+-rw-rw-rw-   0        0        0     2941 2024-05-28 22:05:36.000000 recommendation_lib-1.4/app/preprocessing/preprocess.py
+drwxrwxrwx   0        0        0        0 2024-05-29 08:27:10.112176 recommendation_lib-1.4/app/recommendation/
+-rw-rw-rw-   0        0        0        0 2024-05-27 22:33:29.000000 recommendation_lib-1.4/app/recommendation/__init__.py
+-rw-rw-rw-   0        0        0     1520 2024-05-28 23:44:52.000000 recommendation_lib-1.4/app/recommendation/recommendation.py
+drwxrwxrwx   0        0        0        0 2024-05-29 08:27:10.156135 recommendation_lib-1.4/recommendation_lib.egg-info/
+-rw-rw-rw-   0        0        0      302 2024-05-29 08:27:09.000000 recommendation_lib-1.4/recommendation_lib.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      645 2024-05-29 08:27:09.000000 recommendation_lib-1.4/recommendation_lib.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-05-29 08:27:09.000000 recommendation_lib-1.4/recommendation_lib.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0        4 2024-05-29 08:27:09.000000 recommendation_lib-1.4/recommendation_lib.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0      155 2024-05-29 08:21:27.000000 recommendation_lib-1.4/requirements.txt
+-rw-rw-rw-   0        0        0       42 2024-05-29 08:27:10.166218 recommendation_lib-1.4/setup.cfg
+-rw-rw-rw-   0        0        0      546 2024-05-29 08:26:53.000000 recommendation_lib-1.4/setup.py
```

### Comparing `recommendation_lib-1.3/Dockerfile` & `recommendation_lib-1.4/Dockerfile`

 * *Files 19% similar despite different names*

```diff
@@ -1,32 +1,31 @@
-# Dockerfile
-
 # Use an official Python runtime as a parent image
 FROM python:3.9-slim
 
 # Set the working directory in the container
 WORKDIR /app
 
 # Install dependencies
-COPY requirements.txt .
+# Install gcc and other dependencies for building psycopg2
 RUN apt-get update && \
-    apt-get install -y --no-install-recommends \
-        postgresql-client \
-        libpq-dev && \
-    pip install --no-cache-dir -r requirements.txt
+    apt-get install -y build-essential libpq-dev gcc && \
+    rm -rf /var/lib/apt/lists/*
+
+# Copy requirements.txt to the container
+COPY requirements.txt .
+
+# Install Python dependencies
+RUN pip install --no-cache-dir -r requirements.txt
 
 # Copy the current directory contents into the container at /app
 COPY . /app
 
 # Install PostgreSQL client for database operations
 RUN apt-get update && apt-get install -y postgresql-client
 
-# Set environment variables
+# Set environment variables for PostgreSQL
 ENV POSTGRES_USER=postgres
 ENV POSTGRES_PASSWORD=my_secret_password
 ENV POSTGRES_DB=postgres
 
-# Copy initialization script
-# COPY init.sql /docker-entrypoint-initdb.d/
-
 # Run the FastAPI application
 CMD ["uvicorn", "main:app", "--host", "0.0.0.0", "--port", "8000"]
```

### Comparing `recommendation_lib-1.3/app/core/main.py` & `recommendation_lib-1.4/app/core/main.py`

 * *Files identical despite different names*

### Comparing `recommendation_lib-1.3/app/data/content_owns.csv` & `recommendation_lib-1.4/app/data/content_owns.csv`

 * *Files identical despite different names*

### Comparing `recommendation_lib-1.3/app/data/machine_ratings.csv` & `recommendation_lib-1.4/app/data/machine_ratings.csv`

 * *Files identical despite different names*

### Comparing `recommendation_lib-1.3/app/data/machines.csv` & `recommendation_lib-1.4/app/data/machines.csv`

 * *Files identical despite different names*

### Comparing `recommendation_lib-1.3/app/general_tools/logger.py` & `recommendation_lib-1.4/app/general_tools/logger.py`

 * *Files identical despite different names*

### Comparing `recommendation_lib-1.3/app/postgres/functions.py` & `recommendation_lib-1.4/app/postgres/functions.py`

 * *Files identical despite different names*

### Comparing `recommendation_lib-1.3/app/postgres/table_class.py` & `recommendation_lib-1.4/app/postgres/table_class.py`

 * *Files identical despite different names*

### Comparing `recommendation_lib-1.3/app/preprocessing/preprocess.py` & `recommendation_lib-1.4/app/preprocessing/preprocess.py`

 * *Files identical despite different names*

### Comparing `recommendation_lib-1.3/app/recommendation/recommendation.py` & `recommendation_lib-1.4/app/recommendation/recommendation.py`

 * *Files identical despite different names*

### Comparing `recommendation_lib-1.3/recommendation_lib.egg-info/SOURCES.txt` & `recommendation_lib-1.4/recommendation_lib.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `recommendation_lib-1.3/setup.py` & `recommendation_lib-1.4/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 import setuptools
 
 
 setuptools.setup(
     name="recommendation_lib",
-    version="1.3",
+    version="1.4",
     author="Giorgos Panagou",
     author_email="g.panagou94@gmail.com",
     description="Package containining recommendation algorithm",
     packages= setuptools.find_packages(include=['app', 'app.*']),
     classifiers=[
         "Programming Language :: Python :: 3",
         "Operating System :: OS Independent",
```

