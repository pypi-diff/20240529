# Comparing `tmp/udata_search_service-2.0.3.dev265.tar.gz` & `tmp/udata_search_service-2.0.3.dev272.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "udata_search_service-2.0.3.dev265.tar", last modified: Fri Jan  1 00:00:00 2016, max compression
+gzip compressed data, was "udata_search_service-2.0.3.dev272.tar", last modified: Fri Jan  1 00:00:00 2016, max compression
```

## Comparing `udata_search_service-2.0.3.dev265.tar` & `udata_search_service-2.0.3.dev272.tar`

### file list

```diff
@@ -1,35 +1,35 @@
--rw-r--r--   0        0        0     2409 2023-11-07 09:34:16.000000 udata_search_service-2.0.3.dev265/.circleci/config.yml
--rw-r--r--   0        0        0      763 2023-11-07 09:34:16.000000 udata_search_service-2.0.3.dev265/.gitignore
--rw-r--r--   0        0        0     1949 2023-11-07 09:34:16.000000 udata_search_service-2.0.3.dev265/CHANGELOG.md
--rw-r--r--   0        0        0      173 2023-11-07 09:34:16.000000 udata_search_service-2.0.3.dev265/Dockerfiles/Dockerfile.app
--rw-r--r--   0        0        0      494 2023-11-07 09:34:16.000000 udata_search_service-2.0.3.dev265/Makefile
--rw-r--r--   0        0        0     3776 2023-11-07 09:34:16.000000 udata_search_service-2.0.3.dev265/README.md
--rw-r--r--   0        0        0      394 2023-11-07 09:34:16.000000 udata_search_service-2.0.3.dev265/bumpr.rc
--rw-r--r--   0        0        0      329 2023-11-07 09:34:16.000000 udata_search_service-2.0.3.dev265/docker-compose.test.yml
--rw-r--r--   0        0        0      560 2023-11-07 09:34:16.000000 udata_search_service-2.0.3.dev265/docker-compose.yml
--rw-r--r--   0        0        0    18532 2023-11-07 09:34:16.000000 udata_search_service-2.0.3.dev265/docs/udata-search-service-schema.png
--rw-r--r--   0        0        0      831 2023-11-07 09:34:16.000000 udata_search_service-2.0.3.dev265/pyproject.toml
--rw-r--r--   0        0        0        0 2023-11-07 09:34:16.000000 udata_search_service-2.0.3.dev265/tests/__init__.py
--rw-r--r--   0        0        0      769 2023-11-07 09:34:16.000000 udata_search_service-2.0.3.dev265/tests/conftest.py
--rw-r--r--   0        0        0    28471 2023-11-07 09:34:16.000000 udata_search_service-2.0.3.dev265/tests/test_api.py
--rw-r--r--   0        0        0     6164 2023-11-07 09:34:16.000000 udata_search_service-2.0.3.dev265/tests/test_consumers.py
--rw-r--r--   0        0        0    13254 2023-11-07 09:34:16.000000 udata_search_service-2.0.3.dev265/tests/test_search_client.py
--rw-r--r--   0        0        0      202 2023-11-07 09:34:16.000000 udata_search_service-2.0.3.dev265/udata_search_service/__init__.py
--rw-r--r--   0        0        0      807 2023-11-07 09:34:16.000000 udata_search_service-2.0.3.dev265/udata_search_service/app.py
--rw-r--r--   0        0        0      703 2023-11-07 09:34:16.000000 udata_search_service-2.0.3.dev265/udata_search_service/config.py
--rw-r--r--   0        0        0      767 2023-11-07 09:34:16.000000 udata_search_service-2.0.3.dev265/udata_search_service/container.py
--rw-r--r--   0        0        0        0 2023-11-07 09:34:16.000000 udata_search_service-2.0.3.dev265/udata_search_service/domain/__init__.py
--rw-r--r--   0        0        0     2695 2023-11-07 09:34:16.000000 udata_search_service-2.0.3.dev265/udata_search_service/domain/entities.py
--rw-r--r--   0        0        0     2529 2023-11-07 09:34:16.000000 udata_search_service-2.0.3.dev265/udata_search_service/domain/factories.py
--rw-r--r--   0        0        0     1343 2023-11-07 09:34:16.000000 udata_search_service-2.0.3.dev265/udata_search_service/domain/interfaces.py
--rw-r--r--   0        0        0        0 2023-11-07 09:34:16.000000 udata_search_service-2.0.3.dev265/udata_search_service/infrastructure/__init__.py
--rw-r--r--   0        0        0     2641 2023-11-07 09:34:16.000000 udata_search_service-2.0.3.dev265/udata_search_service/infrastructure/consumers.py
--rw-r--r--   0        0        0     2063 2023-11-07 09:34:16.000000 udata_search_service-2.0.3.dev265/udata_search_service/infrastructure/migrate.py
--rw-r--r--   0        0        0    15989 2023-11-07 09:34:16.000000 udata_search_service-2.0.3.dev265/udata_search_service/infrastructure/search_clients.py
--rw-r--r--   0        0        0     5781 2023-11-07 09:34:16.000000 udata_search_service-2.0.3.dev265/udata_search_service/infrastructure/services.py
--rw-r--r--   0        0        0     1402 2023-11-07 09:34:16.000000 udata_search_service-2.0.3.dev265/udata_search_service/infrastructure/utils.py
--rw-r--r--   0        0        0        0 2023-11-07 09:34:16.000000 udata_search_service-2.0.3.dev265/udata_search_service/presentation/__init__.py
--rw-r--r--   0        0        0    14316 2023-11-07 09:34:16.000000 udata_search_service-2.0.3.dev265/udata_search_service/presentation/api.py
--rw-r--r--   0        0        0      952 2023-11-07 09:34:16.000000 udata_search_service-2.0.3.dev265/udata_search_service/presentation/commands.py
--rw-r--r--   0        0        0       76 2023-11-07 09:34:16.000000 udata_search_service-2.0.3.dev265/udata_search_service/wsgi.py
--rw-r--r--   0        0        0     4510 1970-01-01 00:00:00.000000 udata_search_service-2.0.3.dev265/PKG-INFO
+-rw-r--r--   0        0        0     2423 2024-05-29 09:27:07.000000 udata_search_service-2.0.3.dev272/.circleci/config.yml
+-rw-r--r--   0        0        0      763 2024-05-29 09:27:07.000000 udata_search_service-2.0.3.dev272/.gitignore
+-rw-r--r--   0        0        0     2042 2024-05-29 09:27:07.000000 udata_search_service-2.0.3.dev272/CHANGELOG.md
+-rw-r--r--   0        0        0      174 2024-05-29 09:27:07.000000 udata_search_service-2.0.3.dev272/Dockerfiles/Dockerfile.app
+-rw-r--r--   0        0        0      494 2024-05-29 09:27:07.000000 udata_search_service-2.0.3.dev272/Makefile
+-rw-r--r--   0        0        0     3776 2024-05-29 09:27:07.000000 udata_search_service-2.0.3.dev272/README.md
+-rw-r--r--   0        0        0      394 2024-05-29 09:27:07.000000 udata_search_service-2.0.3.dev272/bumpr.rc
+-rw-r--r--   0        0        0      329 2024-05-29 09:27:07.000000 udata_search_service-2.0.3.dev272/docker-compose.test.yml
+-rw-r--r--   0        0        0      560 2024-05-29 09:27:07.000000 udata_search_service-2.0.3.dev272/docker-compose.yml
+-rw-r--r--   0        0        0    18532 2024-05-29 09:27:07.000000 udata_search_service-2.0.3.dev272/docs/udata-search-service-schema.png
+-rw-r--r--   0        0        0      831 2024-05-29 09:27:07.000000 udata_search_service-2.0.3.dev272/pyproject.toml
+-rw-r--r--   0        0        0        0 2024-05-29 09:27:07.000000 udata_search_service-2.0.3.dev272/tests/__init__.py
+-rw-r--r--   0        0        0      769 2024-05-29 09:27:07.000000 udata_search_service-2.0.3.dev272/tests/conftest.py
+-rw-r--r--   0        0        0    28471 2024-05-29 09:27:07.000000 udata_search_service-2.0.3.dev272/tests/test_api.py
+-rw-r--r--   0        0        0     6164 2024-05-29 09:27:07.000000 udata_search_service-2.0.3.dev272/tests/test_consumers.py
+-rw-r--r--   0        0        0    13254 2024-05-29 09:27:07.000000 udata_search_service-2.0.3.dev272/tests/test_search_client.py
+-rw-r--r--   0        0        0      202 2024-05-29 09:27:07.000000 udata_search_service-2.0.3.dev272/udata_search_service/__init__.py
+-rw-r--r--   0        0        0      807 2024-05-29 09:27:07.000000 udata_search_service-2.0.3.dev272/udata_search_service/app.py
+-rw-r--r--   0        0        0      703 2024-05-29 09:27:07.000000 udata_search_service-2.0.3.dev272/udata_search_service/config.py
+-rw-r--r--   0        0        0      767 2024-05-29 09:27:07.000000 udata_search_service-2.0.3.dev272/udata_search_service/container.py
+-rw-r--r--   0        0        0        0 2024-05-29 09:27:07.000000 udata_search_service-2.0.3.dev272/udata_search_service/domain/__init__.py
+-rw-r--r--   0        0        0     2695 2024-05-29 09:27:07.000000 udata_search_service-2.0.3.dev272/udata_search_service/domain/entities.py
+-rw-r--r--   0        0        0     2529 2024-05-29 09:27:07.000000 udata_search_service-2.0.3.dev272/udata_search_service/domain/factories.py
+-rw-r--r--   0        0        0     1343 2024-05-29 09:27:07.000000 udata_search_service-2.0.3.dev272/udata_search_service/domain/interfaces.py
+-rw-r--r--   0        0        0        0 2024-05-29 09:27:07.000000 udata_search_service-2.0.3.dev272/udata_search_service/infrastructure/__init__.py
+-rw-r--r--   0        0        0     2641 2024-05-29 09:27:07.000000 udata_search_service-2.0.3.dev272/udata_search_service/infrastructure/consumers.py
+-rw-r--r--   0        0        0     2063 2024-05-29 09:27:07.000000 udata_search_service-2.0.3.dev272/udata_search_service/infrastructure/migrate.py
+-rw-r--r--   0        0        0    15989 2024-05-29 09:27:07.000000 udata_search_service-2.0.3.dev272/udata_search_service/infrastructure/search_clients.py
+-rw-r--r--   0        0        0     5781 2024-05-29 09:27:07.000000 udata_search_service-2.0.3.dev272/udata_search_service/infrastructure/services.py
+-rw-r--r--   0        0        0     1402 2024-05-29 09:27:07.000000 udata_search_service-2.0.3.dev272/udata_search_service/infrastructure/utils.py
+-rw-r--r--   0        0        0        0 2024-05-29 09:27:07.000000 udata_search_service-2.0.3.dev272/udata_search_service/presentation/__init__.py
+-rw-r--r--   0        0        0    14316 2024-05-29 09:27:07.000000 udata_search_service-2.0.3.dev272/udata_search_service/presentation/api.py
+-rw-r--r--   0        0        0      952 2024-05-29 09:27:07.000000 udata_search_service-2.0.3.dev272/udata_search_service/presentation/commands.py
+-rw-r--r--   0        0        0       76 2024-05-29 09:27:07.000000 udata_search_service-2.0.3.dev272/udata_search_service/wsgi.py
+-rw-r--r--   0        0        0     4510 1970-01-01 00:00:00.000000 udata_search_service-2.0.3.dev272/PKG-INFO
```

### Comparing `udata_search_service-2.0.3.dev265/.circleci/config.yml` & `udata_search_service-2.0.3.dev272/.circleci/config.yml`

 * *Files 10% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 ---
 version: 2
 
 jobs:
   build:
     docker:
-      - image: udata/circleci:2-alpine
+      - image: udata/circleci:py3.11-bookworm
       - image: udata/elasticsearch:7.16.2
         environment:
           node.name: es01
           cluster.name: es-docker-cluster
           cluster.initial_master_nodes: es01
     environment:
        BASH_ENV: /root/.bashrc
@@ -57,15 +57,15 @@
       - persist_to_workspace:
           root: .
           paths:
             - .
 
   publish:
     docker:
-      - image: udata/circleci:2-alpine
+      - image: udata/circleci:py3.11-bookworm
     steps:
       - attach_workspace:
           at: .
       - deploy:
           name: Publish on PyPI
           command: |
             source venv/bin/activate
```

### Comparing `udata_search_service-2.0.3.dev265/.gitignore` & `udata_search_service-2.0.3.dev272/.gitignore`

 * *Files identical despite different names*

### Comparing `udata_search_service-2.0.3.dev265/CHANGELOG.md` & `udata_search_service-2.0.3.dev272/CHANGELOG.md`

 * *Files 2% similar despite different names*

```diff
@@ -1,12 +1,13 @@
 # Changelog
 
 ## Current (in progress)
 
 - Upgrade Flask to 2.2.5 [#44](https://github.com/opendatateam/udata-search-service/pull/44)
+- Upgrade to Python 3.11 [#45](https://github.com/opendatateam/udata-search-service/pull/45)
 
 ## 2.0.2 (2023-09-01)
 
 - Add dataset's topics in index [#43](https://github.com/opendatateam/udata-search-service/pull/43)
 
 ## 2.0.1 (2023-05-16)
```

### Comparing `udata_search_service-2.0.3.dev265/README.md` & `udata_search_service-2.0.3.dev272/README.md`

 * *Files identical despite different names*

### Comparing `udata_search_service-2.0.3.dev265/docker-compose.yml` & `udata_search_service-2.0.3.dev272/docker-compose.yml`

 * *Files identical despite different names*

### Comparing `udata_search_service-2.0.3.dev265/docs/udata-search-service-schema.png` & `udata_search_service-2.0.3.dev272/docs/udata-search-service-schema.png`

 * *Files identical despite different names*

### Comparing `udata_search_service-2.0.3.dev265/pyproject.toml` & `udata_search_service-2.0.3.dev272/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -4,15 +4,15 @@
 
 [project]
 name = "udata-search-service"
 authors = [{name = "Opendata Team", email = "opendatateam@data.gouv.fr"}]
 readme = "README.md"
 dynamic = ["version", "description"]
 dependencies = [
-    "dependency-injector==4.36.0",
+    "dependency-injector==4.41.0",
     "elasticsearch==7.15.0",
     "elasticsearch_dsl==7.4.0",
     "factory-boy==3.2.1",
     "Faker==11.3.0",
     "flake8==4.0.1",
     "Flask==2.2.5",
     "flit==3.6.0",
```

### Comparing `udata_search_service-2.0.3.dev265/tests/conftest.py` & `udata_search_service-2.0.3.dev272/tests/conftest.py`

 * *Files identical despite different names*

### Comparing `udata_search_service-2.0.3.dev265/tests/test_api.py` & `udata_search_service-2.0.3.dev272/tests/test_api.py`

 * *Files identical despite different names*

### Comparing `udata_search_service-2.0.3.dev265/tests/test_consumers.py` & `udata_search_service-2.0.3.dev272/tests/test_consumers.py`

 * *Files identical despite different names*

### Comparing `udata_search_service-2.0.3.dev265/tests/test_search_client.py` & `udata_search_service-2.0.3.dev272/tests/test_search_client.py`

 * *Files identical despite different names*

### Comparing `udata_search_service-2.0.3.dev265/udata_search_service/app.py` & `udata_search_service-2.0.3.dev272/udata_search_service/app.py`

 * *Files identical despite different names*

### Comparing `udata_search_service-2.0.3.dev265/udata_search_service/config.py` & `udata_search_service-2.0.3.dev272/udata_search_service/config.py`

 * *Files identical despite different names*

### Comparing `udata_search_service-2.0.3.dev265/udata_search_service/container.py` & `udata_search_service-2.0.3.dev272/udata_search_service/container.py`

 * *Files identical despite different names*

### Comparing `udata_search_service-2.0.3.dev265/udata_search_service/domain/entities.py` & `udata_search_service-2.0.3.dev272/udata_search_service/domain/entities.py`

 * *Files identical despite different names*

### Comparing `udata_search_service-2.0.3.dev265/udata_search_service/domain/factories.py` & `udata_search_service-2.0.3.dev272/udata_search_service/domain/factories.py`

 * *Files identical despite different names*

### Comparing `udata_search_service-2.0.3.dev265/udata_search_service/domain/interfaces.py` & `udata_search_service-2.0.3.dev272/udata_search_service/domain/interfaces.py`

 * *Files identical despite different names*

### Comparing `udata_search_service-2.0.3.dev265/udata_search_service/infrastructure/consumers.py` & `udata_search_service-2.0.3.dev272/udata_search_service/infrastructure/consumers.py`

 * *Files identical despite different names*

### Comparing `udata_search_service-2.0.3.dev265/udata_search_service/infrastructure/migrate.py` & `udata_search_service-2.0.3.dev272/udata_search_service/infrastructure/migrate.py`

 * *Files identical despite different names*

### Comparing `udata_search_service-2.0.3.dev265/udata_search_service/infrastructure/search_clients.py` & `udata_search_service-2.0.3.dev272/udata_search_service/infrastructure/search_clients.py`

 * *Files identical despite different names*

### Comparing `udata_search_service-2.0.3.dev265/udata_search_service/infrastructure/services.py` & `udata_search_service-2.0.3.dev272/udata_search_service/infrastructure/services.py`

 * *Files identical despite different names*

### Comparing `udata_search_service-2.0.3.dev265/udata_search_service/infrastructure/utils.py` & `udata_search_service-2.0.3.dev272/udata_search_service/infrastructure/utils.py`

 * *Files identical despite different names*

### Comparing `udata_search_service-2.0.3.dev265/udata_search_service/presentation/api.py` & `udata_search_service-2.0.3.dev272/udata_search_service/presentation/api.py`

 * *Files identical despite different names*

### Comparing `udata_search_service-2.0.3.dev265/udata_search_service/presentation/commands.py` & `udata_search_service-2.0.3.dev272/udata_search_service/presentation/commands.py`

 * *Files identical despite different names*

### Comparing `udata_search_service-2.0.3.dev265/PKG-INFO` & `udata_search_service-2.0.3.dev272/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 Metadata-Version: 2.1
 Name: udata-search-service
-Version: 2.0.3.dev265
+Version: 2.0.3.dev272
 Summary: udata search service
 Author-email: Opendata Team <opendatateam@data.gouv.fr>
 Description-Content-Type: text/markdown
-Requires-Dist: dependency-injector==4.36.0
+Requires-Dist: dependency-injector==4.41.0
 Requires-Dist: elasticsearch==7.15.0
 Requires-Dist: elasticsearch_dsl==7.4.0
 Requires-Dist: factory-boy==3.2.1
 Requires-Dist: Faker==11.3.0
 Requires-Dist: flake8==4.0.1
 Requires-Dist: Flask==2.2.5
 Requires-Dist: flit==3.6.0
```

