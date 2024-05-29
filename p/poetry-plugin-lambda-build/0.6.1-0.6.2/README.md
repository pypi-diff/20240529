# Comparing `tmp/poetry_plugin_lambda_build-0.6.1.tar.gz` & `tmp/poetry_plugin_lambda_build-0.6.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "poetry_plugin_lambda_build-0.6.1.tar", max compression
+gzip compressed data, was "poetry_plugin_lambda_build-0.6.2.tar", max compression
```

## Comparing `poetry_plugin_lambda_build-0.6.1.tar` & `poetry_plugin_lambda_build-0.6.2.tar`

### file list

```diff
@@ -1,14 +1,14 @@
--rw-r--r--   0        0        0     1073 2024-05-24 14:38:43.667381 poetry_plugin_lambda_build-0.6.1/LICENSE
--rw-r--r--   0        0        0     5414 2024-05-24 14:38:43.667381 poetry_plugin_lambda_build-0.6.1/README.md
--rw-r--r--   0        0        0        0 2024-05-24 14:38:43.671381 poetry_plugin_lambda_build-0.6.1/poetry_plugin_lambda_build/__init__.py
--rw-r--r--   0        0        0      748 2024-05-24 14:38:43.671381 poetry_plugin_lambda_build-0.6.1/poetry_plugin_lambda_build/commands.py
--rw-r--r--   0        0        0     3020 2024-05-24 14:38:43.671381 poetry_plugin_lambda_build-0.6.1/poetry_plugin_lambda_build/docker.py
--rw-r--r--   0        0        0     3942 2024-05-24 14:38:43.671381 poetry_plugin_lambda_build-0.6.1/poetry_plugin_lambda_build/parameters.py
--rw-r--r--   0        0        0     2043 2024-05-24 14:38:43.671381 poetry_plugin_lambda_build-0.6.1/poetry_plugin_lambda_build/plugin.py
--rw-r--r--   0        0        0    12794 2024-05-24 14:38:43.671381 poetry_plugin_lambda_build-0.6.1/poetry_plugin_lambda_build/recipes.py
--rw-r--r--   0        0        0     6727 2024-05-24 14:38:43.671381 poetry_plugin_lambda_build-0.6.1/poetry_plugin_lambda_build/requirements.py
--rw-r--r--   0        0        0     2059 2024-05-24 14:38:43.671381 poetry_plugin_lambda_build-0.6.1/poetry_plugin_lambda_build/utils.py
--rw-r--r--   0        0        0     9831 2024-05-24 14:38:43.671381 poetry_plugin_lambda_build-0.6.1/poetry_plugin_lambda_build/walker.py
--rw-r--r--   0        0        0      767 2024-05-24 14:38:43.671381 poetry_plugin_lambda_build-0.6.1/poetry_plugin_lambda_build/zip.py
--rw-r--r--   0        0        0     1063 2024-05-24 14:38:43.671381 poetry_plugin_lambda_build-0.6.1/pyproject.toml
--rw-r--r--   0        0        0     6158 1970-01-01 00:00:00.000000 poetry_plugin_lambda_build-0.6.1/PKG-INFO
+-rw-r--r--   0        0        0     1073 2024-05-29 13:18:21.878552 poetry_plugin_lambda_build-0.6.2/LICENSE
+-rw-r--r--   0        0        0     5414 2024-05-29 13:18:21.878552 poetry_plugin_lambda_build-0.6.2/README.md
+-rw-r--r--   0        0        0        0 2024-05-29 13:18:21.878552 poetry_plugin_lambda_build-0.6.2/poetry_plugin_lambda_build/__init__.py
+-rw-r--r--   0        0        0      748 2024-05-29 13:18:21.882552 poetry_plugin_lambda_build-0.6.2/poetry_plugin_lambda_build/commands.py
+-rw-r--r--   0        0        0     3020 2024-05-29 13:18:21.882552 poetry_plugin_lambda_build-0.6.2/poetry_plugin_lambda_build/docker.py
+-rw-r--r--   0        0        0     3942 2024-05-29 13:18:21.882552 poetry_plugin_lambda_build-0.6.2/poetry_plugin_lambda_build/parameters.py
+-rw-r--r--   0        0        0     2043 2024-05-29 13:18:21.882552 poetry_plugin_lambda_build-0.6.2/poetry_plugin_lambda_build/plugin.py
+-rw-r--r--   0        0        0    12794 2024-05-29 13:18:21.882552 poetry_plugin_lambda_build-0.6.2/poetry_plugin_lambda_build/recipes.py
+-rw-r--r--   0        0        0     6727 2024-05-29 13:18:21.882552 poetry_plugin_lambda_build-0.6.2/poetry_plugin_lambda_build/requirements.py
+-rw-r--r--   0        0        0     2059 2024-05-29 13:18:21.882552 poetry_plugin_lambda_build-0.6.2/poetry_plugin_lambda_build/utils.py
+-rw-r--r--   0        0        0     9831 2024-05-29 13:18:21.882552 poetry_plugin_lambda_build-0.6.2/poetry_plugin_lambda_build/walker.py
+-rw-r--r--   0        0        0      767 2024-05-29 13:18:21.882552 poetry_plugin_lambda_build-0.6.2/poetry_plugin_lambda_build/zip.py
+-rw-r--r--   0        0        0     1042 2024-05-29 13:18:21.882552 poetry_plugin_lambda_build-0.6.2/pyproject.toml
+-rw-r--r--   0        0        0     6124 1970-01-01 00:00:00.000000 poetry_plugin_lambda_build-0.6.2/PKG-INFO
```

### Comparing `poetry_plugin_lambda_build-0.6.1/LICENSE` & `poetry_plugin_lambda_build-0.6.2/LICENSE`

 * *Files identical despite different names*

### Comparing `poetry_plugin_lambda_build-0.6.1/README.md` & `poetry_plugin_lambda_build-0.6.2/README.md`

 * *Files identical despite different names*

### Comparing `poetry_plugin_lambda_build-0.6.1/poetry_plugin_lambda_build/commands.py` & `poetry_plugin_lambda_build-0.6.2/poetry_plugin_lambda_build/commands.py`

 * *Files identical despite different names*

### Comparing `poetry_plugin_lambda_build-0.6.1/poetry_plugin_lambda_build/docker.py` & `poetry_plugin_lambda_build-0.6.2/poetry_plugin_lambda_build/docker.py`

 * *Files identical despite different names*

### Comparing `poetry_plugin_lambda_build-0.6.1/poetry_plugin_lambda_build/parameters.py` & `poetry_plugin_lambda_build-0.6.2/poetry_plugin_lambda_build/parameters.py`

 * *Files identical despite different names*

### Comparing `poetry_plugin_lambda_build-0.6.1/poetry_plugin_lambda_build/plugin.py` & `poetry_plugin_lambda_build-0.6.2/poetry_plugin_lambda_build/plugin.py`

 * *Files identical despite different names*

### Comparing `poetry_plugin_lambda_build-0.6.1/poetry_plugin_lambda_build/recipes.py` & `poetry_plugin_lambda_build-0.6.2/poetry_plugin_lambda_build/recipes.py`

 * *Files identical despite different names*

### Comparing `poetry_plugin_lambda_build-0.6.1/poetry_plugin_lambda_build/requirements.py` & `poetry_plugin_lambda_build-0.6.2/poetry_plugin_lambda_build/requirements.py`

 * *Files identical despite different names*

### Comparing `poetry_plugin_lambda_build-0.6.1/poetry_plugin_lambda_build/utils.py` & `poetry_plugin_lambda_build-0.6.2/poetry_plugin_lambda_build/utils.py`

 * *Files identical despite different names*

### Comparing `poetry_plugin_lambda_build-0.6.1/poetry_plugin_lambda_build/walker.py` & `poetry_plugin_lambda_build-0.6.2/poetry_plugin_lambda_build/walker.py`

 * *Files identical despite different names*

### Comparing `poetry_plugin_lambda_build-0.6.1/poetry_plugin_lambda_build/zip.py` & `poetry_plugin_lambda_build-0.6.2/poetry_plugin_lambda_build/zip.py`

 * *Files identical despite different names*

### Comparing `poetry_plugin_lambda_build-0.6.1/pyproject.toml` & `poetry_plugin_lambda_build-0.6.2/pyproject.toml`

 * *Files 7% similar despite different names*

```diff
@@ -1,18 +1,17 @@
 [tool.poetry]
 name = "poetry-plugin-lambda-build"
-version = "0.6.1"
+version = "0.6.2"
 description = "The plugin for poetry that allows you to build zip packages suited for serverless deployment like AWS Lambda, Google App Engine, Azure App Service, and more..."
 authors = ["Michal Murawski <mmurawski777@gmail.com>"]
 readme = "README.md"
 
 [tool.poetry.dependencies]
 python = "^3.8"
-docker = "^7.0.0"
-requests = ">2.32.0"
+docker = "^7.1.0"
 
 [tool.poetry.group.test.dependencies]
 pytest = "^8.0.1"
 poetry = "^1.7.1"
 pytest-cov = "^5.0.0"
 
 [build-system]
```

### Comparing `poetry_plugin_lambda_build-0.6.1/PKG-INFO` & `poetry_plugin_lambda_build-0.6.2/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,22 +1,21 @@
 Metadata-Version: 2.1
 Name: poetry-plugin-lambda-build
-Version: 0.6.1
+Version: 0.6.2
 Summary: The plugin for poetry that allows you to build zip packages suited for serverless deployment like AWS Lambda, Google App Engine, Azure App Service, and more...
 Author: Michal Murawski
 Author-email: mmurawski777@gmail.com
 Requires-Python: >=3.8,<4.0
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: Python :: 3.12
-Requires-Dist: docker (>=7.0.0,<8.0.0)
-Requires-Dist: requests (>2.32.0)
+Requires-Dist: docker (>=7.1.0,<8.0.0)
 Description-Content-Type: text/markdown
 
 # Poetry Plugin Lambda Build
 
 The plugin for poetry that allows you to build zip packages suited for serverless deployment like AWS Lambda, Google App Engine, Azure App Service, and more...
 
 Additionally it provides docker container support for build inside container
```

