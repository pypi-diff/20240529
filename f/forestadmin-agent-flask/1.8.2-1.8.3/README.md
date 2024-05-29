# Comparing `tmp/forestadmin_agent_flask-1.8.2.tar.gz` & `tmp/forestadmin_agent_flask-1.8.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "forestadmin_agent_flask-1.8.2.tar", max compression
+gzip compressed data, was "forestadmin_agent_flask-1.8.3.tar", max compression
```

## Comparing `forestadmin_agent_flask-1.8.2.tar` & `forestadmin_agent_flask-1.8.3.tar`

### file list

```diff
@@ -1,9 +1,9 @@
--rw-r--r--   0        0        0        0 2024-05-23 09:47:37.395526 forestadmin_agent_flask-1.8.2/README.md
--rw-r--r--   0        0        0        0 2024-05-23 09:47:37.395526 forestadmin_agent_flask-1.8.2/forestadmin/flask_agent/__init__.py
--rw-r--r--   0        0        0     9640 2024-05-23 09:47:37.395526 forestadmin_agent_flask-1.8.2/forestadmin/flask_agent/agent.py
--rw-r--r--   0        0        0      125 2024-05-23 09:47:37.395526 forestadmin_agent_flask-1.8.2/forestadmin/flask_agent/exception.py
--rw-r--r--   0        0        0        0 2024-05-23 09:47:37.395526 forestadmin_agent_flask-1.8.2/forestadmin/flask_agent/utils/__init__.py
--rw-r--r--   0        0        0      581 2024-05-23 09:47:37.395526 forestadmin_agent_flask-1.8.2/forestadmin/flask_agent/utils/dispatcher.py
--rw-r--r--   0        0        0     1630 2024-05-23 09:47:37.395526 forestadmin_agent_flask-1.8.2/forestadmin/flask_agent/utils/requests.py
--rw-r--r--   0        0        0     1950 2024-05-23 09:47:52.967828 forestadmin_agent_flask-1.8.2/pyproject.toml
--rw-r--r--   0        0        0     1060 1970-01-01 00:00:00.000000 forestadmin_agent_flask-1.8.2/PKG-INFO
+-rw-r--r--   0        0        0        0 2024-05-29 07:53:14.663486 forestadmin_agent_flask-1.8.3/README.md
+-rw-r--r--   0        0        0        0 2024-05-29 07:53:14.663486 forestadmin_agent_flask-1.8.3/forestadmin/flask_agent/__init__.py
+-rw-r--r--   0        0        0     9640 2024-05-29 07:53:14.663486 forestadmin_agent_flask-1.8.3/forestadmin/flask_agent/agent.py
+-rw-r--r--   0        0        0      125 2024-05-29 07:53:14.663486 forestadmin_agent_flask-1.8.3/forestadmin/flask_agent/exception.py
+-rw-r--r--   0        0        0        0 2024-05-29 07:53:14.663486 forestadmin_agent_flask-1.8.3/forestadmin/flask_agent/utils/__init__.py
+-rw-r--r--   0        0        0      581 2024-05-29 07:53:14.663486 forestadmin_agent_flask-1.8.3/forestadmin/flask_agent/utils/dispatcher.py
+-rw-r--r--   0        0        0     1630 2024-05-29 07:53:14.663486 forestadmin_agent_flask-1.8.3/forestadmin/flask_agent/utils/requests.py
+-rw-r--r--   0        0        0     1950 2024-05-29 07:53:29.663693 forestadmin_agent_flask-1.8.3/pyproject.toml
+-rw-r--r--   0        0        0     1060 1970-01-01 00:00:00.000000 forestadmin_agent_flask-1.8.3/PKG-INFO
```

### Comparing `forestadmin_agent_flask-1.8.2/forestadmin/flask_agent/agent.py` & `forestadmin_agent_flask-1.8.3/forestadmin/flask_agent/agent.py`

 * *Files identical despite different names*

### Comparing `forestadmin_agent_flask-1.8.2/forestadmin/flask_agent/utils/dispatcher.py` & `forestadmin_agent_flask-1.8.3/forestadmin/flask_agent/utils/dispatcher.py`

 * *Files identical despite different names*

### Comparing `forestadmin_agent_flask-1.8.2/forestadmin/flask_agent/utils/requests.py` & `forestadmin_agent_flask-1.8.3/forestadmin/flask_agent/utils/requests.py`

 * *Files identical despite different names*

### Comparing `forestadmin_agent_flask-1.8.2/pyproject.toml` & `forestadmin_agent_flask-1.8.3/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,28 +1,28 @@
 [build-system]
 requires = [ "poetry-core",]
 build-backend = "poetry.core.masonry.api"
 
 [tool.poetry]
 name = "forestadmin-agent-flask"
 description = "flask agent for forestadmin python agent"
-version = "1.8.2"
+version = "1.8.3"
 authors = [ "Valentin Monté <valentinm@forestadmin.com>", "Julien Barreau <julien.barreau@forestadmin.com>",]
 readme = "README.md"
 repository = "https://github.com/ForestAdmin/agent-python"
 documentation = "https://docs.forestadmin.com/developer-guide-agents-python/"
 homepage = "https://www.forestadmin.com"
 [[tool.poetry.packages]]
 include = "forestadmin"
 
 [tool.poetry.dependencies]
 python = ">=3.8,<3.13"
 typing-extensions = "~=4.2"
-forestadmin-agent-toolkit = "1.8.2"
-forestadmin-datasource-toolkit = "1.8.2"
+forestadmin-agent-toolkit = "1.8.3"
+forestadmin-datasource-toolkit = "1.8.3"
 flask-cors = ">=3.0.0"
 
 [tool.poetry.dependencies.flask]
 extras = [ "async",]
 version = ">=2.0.0"
 
 [tool.poetry.dependencies."backports.zoneinfo"]
```

### Comparing `forestadmin_agent_flask-1.8.2/PKG-INFO` & `forestadmin_agent_flask-1.8.3/PKG-INFO`

 * *Files 9% similar despite different names*

```diff
@@ -1,25 +1,25 @@
 Metadata-Version: 2.1
 Name: forestadmin-agent-flask
-Version: 1.8.2
+Version: 1.8.3
 Summary: flask agent for forestadmin python agent
 Home-page: https://www.forestadmin.com
 Author: Valentin Monté
 Author-email: valentinm@forestadmin.com
 Requires-Python: >=3.8,<3.13
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: Python :: 3.12
 Requires-Dist: backports.zoneinfo[tzdata] (>=0.2.1,<0.3.0) ; python_version < "3.9"
 Requires-Dist: flask-cors (>=3.0.0)
 Requires-Dist: flask[async] (>=2.0.0)
-Requires-Dist: forestadmin-agent-toolkit (==1.8.2)
-Requires-Dist: forestadmin-datasource-toolkit (==1.8.2)
+Requires-Dist: forestadmin-agent-toolkit (==1.8.3)
+Requires-Dist: forestadmin-datasource-toolkit (==1.8.3)
 Requires-Dist: typing-extensions (>=4.2,<5.0)
 Project-URL: Documentation, https://docs.forestadmin.com/developer-guide-agents-python/
 Project-URL: Repository, https://github.com/ForestAdmin/agent-python
 Description-Content-Type: text/markdown
```

