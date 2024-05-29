# Comparing `tmp/dhuodata_lib-0.3.8.tar.gz` & `tmp/dhuodata_lib-0.3.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dhuodata_lib-0.3.8.tar", last modified: Mon May 13 20:02:36 2024, max compression
+gzip compressed data, was "dhuodata_lib-0.3.9.tar", last modified: Wed May 29 16:05:06 2024, max compression
```

## Comparing `dhuodata_lib-0.3.8.tar` & `dhuodata_lib-0.3.9.tar`

### file list

```diff
@@ -1,24 +1,28 @@
-drwxrwxr-x   0 diego     (1000) diego     (1000)        0 2024-05-13 20:02:36.471445 dhuodata_lib-0.3.8/
--rw-r--r--   0 diego     (1000) diego     (1000)     3007 2024-05-13 20:02:36.471445 dhuodata_lib-0.3.8/PKG-INFO
--rw-rw-r--   0 diego     (1000) diego     (1000)     2346 2024-04-16 18:35:41.000000 dhuodata_lib-0.3.8/README.md
--rw-rw-r--   0 diego     (1000) diego     (1000)       38 2024-05-13 20:02:36.471445 dhuodata_lib-0.3.8/setup.cfg
--rw-rw-r--   0 diego     (1000) diego     (1000)      863 2024-05-13 20:02:28.000000 dhuodata_lib-0.3.8/setup.py
-drwxrwxr-x   0 diego     (1000) diego     (1000)        0 2024-05-13 20:02:36.467446 dhuodata_lib-0.3.8/src/
-drwxrwxr-x   0 diego     (1000) diego     (1000)        0 2024-05-13 20:02:36.471445 dhuodata_lib-0.3.8/src/dhuodata_lib.egg-info/
--rw-r--r--   0 diego     (1000) diego     (1000)     3007 2024-05-13 20:02:36.000000 dhuodata_lib-0.3.8/src/dhuodata_lib.egg-info/PKG-INFO
--rw-rw-r--   0 diego     (1000) diego     (1000)      445 2024-05-13 20:02:36.000000 dhuodata_lib-0.3.8/src/dhuodata_lib.egg-info/SOURCES.txt
--rw-rw-r--   0 diego     (1000) diego     (1000)        1 2024-05-13 20:02:36.000000 dhuodata_lib-0.3.8/src/dhuodata_lib.egg-info/dependency_links.txt
--rw-rw-r--   0 diego     (1000) diego     (1000)      152 2024-05-13 20:02:36.000000 dhuodata_lib-0.3.8/src/dhuodata_lib.egg-info/requires.txt
--rw-rw-r--   0 diego     (1000) diego     (1000)        8 2024-05-13 20:02:36.000000 dhuodata_lib-0.3.8/src/dhuodata_lib.egg-info/top_level.txt
-drwxrwxr-x   0 diego     (1000) diego     (1000)        0 2024-05-13 20:02:36.471445 dhuodata_lib-0.3.8/src/dhuolib/
--rw-rw-r--   0 diego     (1000) diego     (1000)        0 2024-05-09 13:16:16.000000 dhuodata_lib-0.3.8/src/dhuolib/__init__.py
--rw-rw-r--   0 diego     (1000) diego     (1000)      261 2024-05-09 13:16:16.000000 dhuodata_lib-0.3.8/src/dhuolib/auth.py
--rw-rw-r--   0 diego     (1000) diego     (1000)     8805 2024-05-13 19:55:08.000000 dhuodata_lib-0.3.8/src/dhuolib/clients.py
--rw-rw-r--   0 diego     (1000) diego     (1000)      348 2024-05-09 13:16:16.000000 dhuodata_lib-0.3.8/src/dhuolib/config.py
--rw-rw-r--   0 diego     (1000) diego     (1000)       95 2024-05-09 16:59:36.000000 dhuodata_lib-0.3.8/src/dhuolib/enums.py
--rw-rw-r--   0 diego     (1000) diego     (1000)      758 2024-05-09 13:16:16.000000 dhuodata_lib-0.3.8/src/dhuolib/predict.py
--rw-rw-r--   0 diego     (1000) diego     (1000)     3393 2024-05-13 18:03:54.000000 dhuodata_lib-0.3.8/src/dhuolib/services.py
--rw-rw-r--   0 diego     (1000) diego     (1000)      790 2024-05-09 13:16:16.000000 dhuodata_lib-0.3.8/src/dhuolib/validations.py
--rw-rw-r--   0 diego     (1000) diego     (1000)      141 2024-05-09 13:16:16.000000 dhuodata_lib-0.3.8/src/dhuolib/worker.py
-drwxrwxr-x   0 diego     (1000) diego     (1000)        0 2024-05-13 20:02:36.471445 dhuodata_lib-0.3.8/tests/
--rw-rw-r--   0 diego     (1000) diego     (1000)     5248 2024-05-13 19:59:14.000000 dhuodata_lib-0.3.8/tests/test_dhuolib.py
+drwxrwxr-x   0 diego     (1000) diego     (1000)        0 2024-05-29 16:05:06.696355 dhuodata_lib-0.3.9/
+-rw-r--r--   0 diego     (1000) diego     (1000)     3560 2024-05-29 16:05:06.696355 dhuodata_lib-0.3.9/PKG-INFO
+-rw-rw-r--   0 diego     (1000) diego     (1000)     2346 2024-04-16 18:35:41.000000 dhuodata_lib-0.3.9/README.md
+-rw-rw-r--   0 diego     (1000) diego     (1000)       38 2024-05-29 16:05:06.696355 dhuodata_lib-0.3.9/setup.cfg
+-rw-rw-r--   0 diego     (1000) diego     (1000)      863 2024-05-29 16:04:24.000000 dhuodata_lib-0.3.9/setup.py
+drwxrwxr-x   0 diego     (1000) diego     (1000)        0 2024-05-29 16:05:06.692355 dhuodata_lib-0.3.9/src/
+drwxrwxr-x   0 diego     (1000) diego     (1000)        0 2024-05-29 16:05:06.696355 dhuodata_lib-0.3.9/src/dhuodata_lib.egg-info/
+-rw-r--r--   0 diego     (1000) diego     (1000)     3560 2024-05-29 16:05:06.000000 dhuodata_lib-0.3.9/src/dhuodata_lib.egg-info/PKG-INFO
+-rw-rw-r--   0 diego     (1000) diego     (1000)      538 2024-05-29 16:05:06.000000 dhuodata_lib-0.3.9/src/dhuodata_lib.egg-info/SOURCES.txt
+-rw-rw-r--   0 diego     (1000) diego     (1000)        1 2024-05-29 16:05:06.000000 dhuodata_lib-0.3.9/src/dhuodata_lib.egg-info/dependency_links.txt
+-rw-rw-r--   0 diego     (1000) diego     (1000)      435 2024-05-29 16:05:06.000000 dhuodata_lib-0.3.9/src/dhuodata_lib.egg-info/requires.txt
+-rw-rw-r--   0 diego     (1000) diego     (1000)        8 2024-05-29 16:05:06.000000 dhuodata_lib-0.3.9/src/dhuodata_lib.egg-info/top_level.txt
+drwxrwxr-x   0 diego     (1000) diego     (1000)        0 2024-05-29 16:05:06.696355 dhuodata_lib-0.3.9/src/dhuolib/
+-rw-rw-r--   0 diego     (1000) diego     (1000)        0 2024-05-09 13:16:16.000000 dhuodata_lib-0.3.9/src/dhuolib/__init__.py
+-rw-rw-r--   0 diego     (1000) diego     (1000)      261 2024-05-09 13:16:16.000000 dhuodata_lib-0.3.9/src/dhuolib/auth.py
+-rw-rw-r--   0 diego     (1000) diego     (1000)      348 2024-05-09 13:16:16.000000 dhuodata_lib-0.3.9/src/dhuolib/config.py
+-rw-rw-r--   0 diego     (1000) diego     (1000)       95 2024-05-09 16:59:36.000000 dhuodata_lib-0.3.9/src/dhuolib/enums.py
+-rw-rw-r--   0 diego     (1000) diego     (1000)     1000 2024-05-27 19:03:08.000000 dhuodata_lib-0.3.9/src/dhuolib/extensions.py
+-rw-rw-r--   0 diego     (1000) diego     (1000)      758 2024-05-09 13:16:16.000000 dhuodata_lib-0.3.9/src/dhuolib/predict.py
+-rw-rw-r--   0 diego     (1000) diego     (1000)     3375 2024-05-28 12:44:44.000000 dhuodata_lib-0.3.9/src/dhuolib/repository.py
+-rw-rw-r--   0 diego     (1000) diego     (1000)     3343 2024-05-17 15:29:34.000000 dhuodata_lib-0.3.9/src/dhuolib/services.py
+-rw-rw-r--   0 diego     (1000) diego     (1000)     1033 2024-05-28 17:55:59.000000 dhuodata_lib-0.3.9/src/dhuolib/utils.py
+-rw-rw-r--   0 diego     (1000) diego     (1000)      790 2024-05-09 13:16:16.000000 dhuodata_lib-0.3.9/src/dhuolib/validations.py
+-rw-rw-r--   0 diego     (1000) diego     (1000)      141 2024-05-09 13:16:16.000000 dhuodata_lib-0.3.9/src/dhuolib/worker.py
+drwxrwxr-x   0 diego     (1000) diego     (1000)        0 2024-05-29 16:05:06.696355 dhuodata_lib-0.3.9/tests/
+-rw-rw-r--   0 diego     (1000) diego     (1000)     4285 2024-05-29 16:05:04.000000 dhuodata_lib-0.3.9/tests/test_database.py
+-rw-rw-r--   0 diego     (1000) diego     (1000)     6219 2024-05-29 16:04:55.000000 dhuodata_lib-0.3.9/tests/test_dhuolib.py
+-rw-rw-r--   0 diego     (1000) diego     (1000)      906 2024-05-28 22:01:05.000000 dhuodata_lib-0.3.9/tests/test_utils.py
```

### Comparing `dhuodata_lib-0.3.8/PKG-INFO` & `dhuodata_lib-0.3.9/PKG-INFO`

 * *Files 22% similar despite different names*

```diff
@@ -1,17 +1,35 @@
 Metadata-Version: 2.1
 Name: dhuodata-lib
-Version: 0.3.8
+Version: 0.3.9
 Home-page: https://gitlab.engdb.com.br/dhuo-plat/dhuo-data/data-science/dhuolib
 Author: DHuO Data Team
 Author-email: diego.salles@engdb.com.br
 Platform: any
 Description-Content-Type: text/markdown
 Requires-Dist: oci==2.125.3
 Requires-Dist: pydantic==1.8.2
+Requires-Dist: SQLAlchemy==2.0.30
+Requires-Dist: pandas
+Requires-Dist: oracledb
+Requires-Dist: cffi==1.16.0
+Requires-Dist: cryptography==42.0.7
+Requires-Dist: joblib==1.4.2
+Requires-Dist: lightgbm==4.3.0
+Requires-Dist: numpy==1.26.4
+Requires-Dist: oracledb==2.2.0
+Requires-Dist: pandas==2.2.2
+Requires-Dist: pycparser==2.22
+Requires-Dist: python-dateutil==2.9.0.post0
+Requires-Dist: pytz==2024.1
+Requires-Dist: scikit-learn==1.4.2
+Requires-Dist: scipy==1.13.0
+Requires-Dist: six==1.16.0
+Requires-Dist: threadpoolctl==3.5.0
+Requires-Dist: tzdata==2024.1
 Provides-Extra: interactive
 Requires-Dist: mypy==1.5.1; extra == "interactive"
 Requires-Dist: flake8==6.1.0; extra == "interactive"
 Requires-Dist: black==22.3.0; extra == "interactive"
 Requires-Dist: pytest-cov~=4.0; extra == "interactive"
 Requires-Dist: pytest~=7.0; extra == "interactive"
 Requires-Dist: twine==3.4.2; extra == "interactive"
```

### Comparing `dhuodata_lib-0.3.8/README.md` & `dhuodata_lib-0.3.9/README.md`

 * *Files identical despite different names*

### Comparing `dhuodata_lib-0.3.8/setup.py` & `dhuodata_lib-0.3.9/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -11,15 +11,15 @@
 
 README = ""
 if os.path.exists("README.md"):
     README = open("README.md").read()
 
 setup(
     name="dhuodata-lib",
-    version="0.3.8",
+    version="0.3.9",
     long_description=README,
     long_description_content_type="text/markdown",
     author="DHuO Data Team",
     author_email="diego.salles@engdb.com.br",
     url="https://gitlab.engdb.com.br/dhuo-plat/dhuo-data/data-science/dhuolib",
     install_requires=REQUIRED_PACKAGES,
     extras_require={"interactive": DEV_PACKAGES},
```

### Comparing `dhuodata_lib-0.3.8/src/dhuodata_lib.egg-info/PKG-INFO` & `dhuodata_lib-0.3.9/src/dhuodata_lib.egg-info/PKG-INFO`

 * *Files 22% similar despite different names*

```diff
@@ -1,17 +1,35 @@
 Metadata-Version: 2.1
 Name: dhuodata-lib
-Version: 0.3.8
+Version: 0.3.9
 Home-page: https://gitlab.engdb.com.br/dhuo-plat/dhuo-data/data-science/dhuolib
 Author: DHuO Data Team
 Author-email: diego.salles@engdb.com.br
 Platform: any
 Description-Content-Type: text/markdown
 Requires-Dist: oci==2.125.3
 Requires-Dist: pydantic==1.8.2
+Requires-Dist: SQLAlchemy==2.0.30
+Requires-Dist: pandas
+Requires-Dist: oracledb
+Requires-Dist: cffi==1.16.0
+Requires-Dist: cryptography==42.0.7
+Requires-Dist: joblib==1.4.2
+Requires-Dist: lightgbm==4.3.0
+Requires-Dist: numpy==1.26.4
+Requires-Dist: oracledb==2.2.0
+Requires-Dist: pandas==2.2.2
+Requires-Dist: pycparser==2.22
+Requires-Dist: python-dateutil==2.9.0.post0
+Requires-Dist: pytz==2024.1
+Requires-Dist: scikit-learn==1.4.2
+Requires-Dist: scipy==1.13.0
+Requires-Dist: six==1.16.0
+Requires-Dist: threadpoolctl==3.5.0
+Requires-Dist: tzdata==2024.1
 Provides-Extra: interactive
 Requires-Dist: mypy==1.5.1; extra == "interactive"
 Requires-Dist: flake8==6.1.0; extra == "interactive"
 Requires-Dist: black==22.3.0; extra == "interactive"
 Requires-Dist: pytest-cov~=4.0; extra == "interactive"
 Requires-Dist: pytest~=7.0; extra == "interactive"
 Requires-Dist: twine==3.4.2; extra == "interactive"
```

### Comparing `dhuodata_lib-0.3.8/src/dhuolib/predict.py` & `dhuodata_lib-0.3.9/src/dhuolib/predict.py`

 * *Files identical despite different names*

### Comparing `dhuodata_lib-0.3.8/src/dhuolib/services.py` & `dhuodata_lib-0.3.9/src/dhuolib/services.py`

 * *Files 12% similar despite different names*

```diff
@@ -8,23 +8,23 @@
 
         if not isinstance(service_endpoint, str):
             raise ValueError("service_endpoint must be a string")
 
         self.service_endpoint = f"{service_endpoint}/api"
         self.headers = {"Content-Type": "application/json"}
 
-    def create_experiment_by_conf_json(self, experiment_params='', files=None):
+    def create_experiment_by_conf_json(self, experiment_params="", files=None):
         if experiment_params is None and isinstance(experiment_params, dict):
             raise ValueError("json_data must be a dict")
 
         if files:
             return requests.post(
                 f"{self.service_endpoint}/experiment/save",
                 data=experiment_params,
-                files=files
+                files=files,
             )
 
         response = requests.post(
             f"{self.service_endpoint}/experiment/save",
             data=json.dumps(experiment_params),
             headers=self.headers,
         )
@@ -49,52 +49,48 @@
         )
         return response.json()
 
     def predict_online(self, params={}, files=None):
         if params is None and not isinstance(params, dict):
             raise ValueError("json_data must be a dict")
         response = requests.post(
-            f"{self.service_endpoint}/experiment/predict_online", data=params, files=files
+            f"{self.service_endpoint}/experiment/predict_online",
+            data=params,
+            files=files,
         )
         return response.json()
 
     def create_project(self, project_name):
-        body = {
-            'project_name': project_name
-        }
-        response = requests.post(
-            f"{self.service_endpoint}/project", json=body)
+        body = {"project_name": project_name}
+        response = requests.post(f"{self.service_endpoint}/project", json=body)
 
         return response.json()
 
-    def deploy_script(self, project_name: str, script_file_encode: str, requirements_file_enconde: str):
+    def deploy_script(
+        self, project_name: str, script_file_encode: str, requirements_file_enconde: str
+    ):
         body = {
             "project_name": project_name,
             "requirements_content": requirements_file_enconde.decode("utf-8"),
-            "run_script_content": script_file_encode.decode("utf-8")
+            "run_script_content": script_file_encode.decode("utf-8"),
         }
         response = requests.post(f"{self.service_endpoint}/deploy", json=body)
 
         return response.json()
 
     def get_pipeline_status(self, project_name: str):
         route = "deploy/{}".format(project_name)
         response = requests.get(f"{self.service_endpoint}/{route}")
 
         return response.json()
 
     def create_cluster(self, project_name: str, cluster_size: int):
-        body = {
-            "project_name": project_name,
-            "cluster_size": cluster_size
-        }
+        body = {"project_name": project_name, "cluster_size": cluster_size}
         response = requests.post(f"{self.service_endpoint}/cluster", json=body)
 
         return response.json()
 
     def run_pipeline(self, project_name: str):
-        body = {
-            "project_name": project_name
-        }
+        body = {"project_name": project_name}
         response = requests.post(f"{self.service_endpoint}/cluster/run", json=body)
 
         return response.json()
```

### Comparing `dhuodata_lib-0.3.8/src/dhuolib/validations.py` & `dhuodata_lib-0.3.9/src/dhuolib/validations.py`

 * *Files identical despite different names*

