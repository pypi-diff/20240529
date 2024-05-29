# Comparing `tmp/forestadmin_agent_django-1.8.2.tar.gz` & `tmp/forestadmin_agent_django-1.8.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "forestadmin_agent_django-1.8.2.tar", max compression
+gzip compressed data, was "forestadmin_agent_django-1.8.3.tar", max compression
```

## Comparing `forestadmin_agent_django-1.8.2.tar` & `forestadmin_agent_django-1.8.3.tar`

### file list

```diff
@@ -1,18 +1,18 @@
--rw-r--r--   0        0        0        0 2024-05-23 09:47:37.940073 forestadmin_agent_django-1.8.2/README.md
--rw-r--r--   0        0        0        0 2024-05-23 09:47:37.940073 forestadmin_agent_django-1.8.2/forestadmin/django_agent/__init__.py
--rw-r--r--   0        0        0     2757 2024-05-23 09:47:37.940073 forestadmin_agent_django-1.8.2/forestadmin/django_agent/agent.py
--rw-r--r--   0        0        0     3735 2024-05-23 09:47:37.940073 forestadmin_agent_django-1.8.2/forestadmin/django_agent/apps.py
--rw-r--r--   0        0        0     2740 2024-05-23 09:47:37.940073 forestadmin_agent_django-1.8.2/forestadmin/django_agent/urls.py
--rw-r--r--   0        0        0        0 2024-05-23 09:47:37.940073 forestadmin_agent_django-1.8.2/forestadmin/django_agent/utils/__init__.py
--rw-r--r--   0        0        0     1488 2024-05-23 09:47:37.944073 forestadmin_agent_django-1.8.2/forestadmin/django_agent/utils/converter.py
--rw-r--r--   0        0        0      612 2024-05-23 09:47:37.944073 forestadmin_agent_django-1.8.2/forestadmin/django_agent/utils/dispatcher.py
--rw-r--r--   0        0        0        0 2024-05-23 09:47:37.944073 forestadmin_agent_django-1.8.2/forestadmin/django_agent/views/__init__.py
--rw-r--r--   0        0        0      887 2024-05-23 09:47:37.944073 forestadmin_agent_django-1.8.2/forestadmin/django_agent/views/actions.py
--rw-r--r--   0        0        0      899 2024-05-23 09:47:37.944073 forestadmin_agent_django-1.8.2/forestadmin/django_agent/views/authentication.py
--rw-r--r--   0        0        0      975 2024-05-23 09:47:37.944073 forestadmin_agent_django-1.8.2/forestadmin/django_agent/views/charts.py
--rw-r--r--   0        0        0     1655 2024-05-23 09:47:37.944073 forestadmin_agent_django-1.8.2/forestadmin/django_agent/views/crud.py
--rw-r--r--   0        0        0     1336 2024-05-23 09:47:37.944073 forestadmin_agent_django-1.8.2/forestadmin/django_agent/views/crud_related.py
--rw-r--r--   0        0        0      465 2024-05-23 09:47:37.944073 forestadmin_agent_django-1.8.2/forestadmin/django_agent/views/index.py
--rw-r--r--   0        0        0      598 2024-05-23 09:47:37.944073 forestadmin_agent_django-1.8.2/forestadmin/django_agent/views/stats.py
--rw-r--r--   0        0        0     1949 2024-05-23 09:47:55.296298 forestadmin_agent_django-1.8.2/pyproject.toml
--rw-r--r--   0        0        0     1069 1970-01-01 00:00:00.000000 forestadmin_agent_django-1.8.2/PKG-INFO
+-rw-r--r--   0        0        0        0 2024-05-29 07:53:13.926919 forestadmin_agent_django-1.8.3/README.md
+-rw-r--r--   0        0        0        0 2024-05-29 07:53:13.926919 forestadmin_agent_django-1.8.3/forestadmin/django_agent/__init__.py
+-rw-r--r--   0        0        0     2757 2024-05-29 07:53:13.926919 forestadmin_agent_django-1.8.3/forestadmin/django_agent/agent.py
+-rw-r--r--   0        0        0     3735 2024-05-29 07:53:13.926919 forestadmin_agent_django-1.8.3/forestadmin/django_agent/apps.py
+-rw-r--r--   0        0        0     2740 2024-05-29 07:53:13.926919 forestadmin_agent_django-1.8.3/forestadmin/django_agent/urls.py
+-rw-r--r--   0        0        0        0 2024-05-29 07:53:13.926919 forestadmin_agent_django-1.8.3/forestadmin/django_agent/utils/__init__.py
+-rw-r--r--   0        0        0     1488 2024-05-29 07:53:13.926919 forestadmin_agent_django-1.8.3/forestadmin/django_agent/utils/converter.py
+-rw-r--r--   0        0        0      612 2024-05-29 07:53:13.926919 forestadmin_agent_django-1.8.3/forestadmin/django_agent/utils/dispatcher.py
+-rw-r--r--   0        0        0        0 2024-05-29 07:53:13.926919 forestadmin_agent_django-1.8.3/forestadmin/django_agent/views/__init__.py
+-rw-r--r--   0        0        0      887 2024-05-29 07:53:13.926919 forestadmin_agent_django-1.8.3/forestadmin/django_agent/views/actions.py
+-rw-r--r--   0        0        0      899 2024-05-29 07:53:13.926919 forestadmin_agent_django-1.8.3/forestadmin/django_agent/views/authentication.py
+-rw-r--r--   0        0        0      975 2024-05-29 07:53:13.930919 forestadmin_agent_django-1.8.3/forestadmin/django_agent/views/charts.py
+-rw-r--r--   0        0        0     1655 2024-05-29 07:53:13.930919 forestadmin_agent_django-1.8.3/forestadmin/django_agent/views/crud.py
+-rw-r--r--   0        0        0     1336 2024-05-29 07:53:13.930919 forestadmin_agent_django-1.8.3/forestadmin/django_agent/views/crud_related.py
+-rw-r--r--   0        0        0      465 2024-05-29 07:53:13.930919 forestadmin_agent_django-1.8.3/forestadmin/django_agent/views/index.py
+-rw-r--r--   0        0        0      598 2024-05-29 07:53:13.930919 forestadmin_agent_django-1.8.3/forestadmin/django_agent/views/stats.py
+-rw-r--r--   0        0        0     1949 2024-05-29 07:53:27.822915 forestadmin_agent_django-1.8.3/pyproject.toml
+-rw-r--r--   0        0        0     1069 1970-01-01 00:00:00.000000 forestadmin_agent_django-1.8.3/PKG-INFO
```

### Comparing `forestadmin_agent_django-1.8.2/forestadmin/django_agent/agent.py` & `forestadmin_agent_django-1.8.3/forestadmin/django_agent/agent.py`

 * *Files identical despite different names*

### Comparing `forestadmin_agent_django-1.8.2/forestadmin/django_agent/apps.py` & `forestadmin_agent_django-1.8.3/forestadmin/django_agent/apps.py`

 * *Files identical despite different names*

### Comparing `forestadmin_agent_django-1.8.2/forestadmin/django_agent/urls.py` & `forestadmin_agent_django-1.8.3/forestadmin/django_agent/urls.py`

 * *Files identical despite different names*

### Comparing `forestadmin_agent_django-1.8.2/forestadmin/django_agent/utils/converter.py` & `forestadmin_agent_django-1.8.3/forestadmin/django_agent/utils/converter.py`

 * *Files identical despite different names*

### Comparing `forestadmin_agent_django-1.8.2/forestadmin/django_agent/utils/dispatcher.py` & `forestadmin_agent_django-1.8.3/forestadmin/django_agent/utils/dispatcher.py`

 * *Files identical despite different names*

### Comparing `forestadmin_agent_django-1.8.2/forestadmin/django_agent/views/actions.py` & `forestadmin_agent_django-1.8.3/forestadmin/django_agent/views/actions.py`

 * *Files identical despite different names*

### Comparing `forestadmin_agent_django-1.8.2/forestadmin/django_agent/views/authentication.py` & `forestadmin_agent_django-1.8.3/forestadmin/django_agent/views/authentication.py`

 * *Files identical despite different names*

### Comparing `forestadmin_agent_django-1.8.2/forestadmin/django_agent/views/charts.py` & `forestadmin_agent_django-1.8.3/forestadmin/django_agent/views/charts.py`

 * *Files identical despite different names*

### Comparing `forestadmin_agent_django-1.8.2/forestadmin/django_agent/views/crud.py` & `forestadmin_agent_django-1.8.3/forestadmin/django_agent/views/crud.py`

 * *Files identical despite different names*

### Comparing `forestadmin_agent_django-1.8.2/forestadmin/django_agent/views/crud_related.py` & `forestadmin_agent_django-1.8.3/forestadmin/django_agent/views/crud_related.py`

 * *Files identical despite different names*

### Comparing `forestadmin_agent_django-1.8.2/forestadmin/django_agent/views/stats.py` & `forestadmin_agent_django-1.8.3/forestadmin/django_agent/views/stats.py`

 * *Files identical despite different names*

### Comparing `forestadmin_agent_django-1.8.2/pyproject.toml` & `forestadmin_agent_django-1.8.3/pyproject.toml`

 * *Files 5% similar despite different names*

```diff
@@ -1,28 +1,28 @@
 [build-system]
 requires = [ "poetry-core",]
 build-backend = "poetry.core.masonry.api"
 
 [tool.poetry]
 name = "forestadmin-agent-django"
-version = "1.8.2"
+version = "1.8.3"
 description = "django agent for forestadmin python agent"
 authors = [ "Julien Barreau <julien.barreau@forestadmin.com>",]
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
-forestadmin-datasource-django = "1.8.2"
+forestadmin-agent-toolkit = "1.8.3"
+forestadmin-datasource-django = "1.8.3"
 django = ">=3.2,<6.0"
 django-cors-headers = ">=3.8"
 
 [tool.pytest.ini_options]
 DJANGO_SETTINGS_MODULE = "test_project_agent.settings"
 pythonpath = "tests/test_project_agent"
```

### Comparing `forestadmin_agent_django-1.8.2/PKG-INFO` & `forestadmin_agent_django-1.8.3/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,25 +1,25 @@
 Metadata-Version: 2.1
 Name: forestadmin-agent-django
-Version: 1.8.2
+Version: 1.8.3
 Summary: django agent for forestadmin python agent
 Home-page: https://www.forestadmin.com
 Author: Julien Barreau
 Author-email: julien.barreau@forestadmin.com
 Requires-Python: >=3.8,<3.13
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: Python :: 3.12
 Requires-Dist: backports.zoneinfo[tzdata] (>=0.2.1,<0.3.0) ; python_version < "3.9"
 Requires-Dist: django (>=3.2,<6.0)
 Requires-Dist: django-cors-headers (>=3.8)
-Requires-Dist: forestadmin-agent-toolkit (==1.8.2)
-Requires-Dist: forestadmin-datasource-django (==1.8.2)
+Requires-Dist: forestadmin-agent-toolkit (==1.8.3)
+Requires-Dist: forestadmin-datasource-django (==1.8.3)
 Requires-Dist: typing-extensions (>=4.2,<5.0)
 Project-URL: Documentation, https://docs.forestadmin.com/developer-guide-agents-python/
 Project-URL: Repository, https://github.com/ForestAdmin/agent-python
 Description-Content-Type: text/markdown
```

