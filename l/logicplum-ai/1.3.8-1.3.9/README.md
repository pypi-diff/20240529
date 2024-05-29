# Comparing `tmp/logicplum-ai-1.3.8.tar.gz` & `tmp/logicplum_ai-1.3.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "C:\WORK\AI CLOUD 4.0\package pYpI\aicloudlp\aicloud-lp-new\dist\.tmp-ez7bt7r7\logicplum-ai-1.3.8.tar", last modified: Tue Apr  2 11:11:03 2024, max compression
+gzip compressed data, was "C:\WORK\AI CLOUD 4.0\package pYpI\aicloudlp\aicloud-lp-new\dist\.tmp-7ihtr4i4\logicplum_ai-1.3.9.tar", last modified: Wed May 29 05:23:37 2024, max compression
```

## Comparing `logicplum-ai-1.3.8.tar` & `logicplum_ai-1.3.9.tar`

### file list

```diff
@@ -1,37 +1,37 @@
-drwxrwxrwx   0        0        0        0 2024-04-02 11:11:03.123609 logicplum-ai-1.3.8/
--rw-rw-rw-   0        0        0     2161 2024-04-02 11:09:11.000000 logicplum-ai-1.3.8/CHANGELOG.md
--rw-rw-rw-   0        0        0     2313 2024-04-02 11:11:03.123609 logicplum-ai-1.3.8/PKG-INFO
-drwxrwxrwx   0        0        0        0 2024-04-02 11:11:03.092364 logicplum-ai-1.3.8/logicplum/
--rw-rw-rw-   0        0        0        0 2023-12-14 07:41:33.000000 logicplum-ai-1.3.8/logicplum/__init__.py
-drwxrwxrwx   0        0        0        0 2024-04-02 11:11:03.092364 logicplum-ai-1.3.8/logicplum/aicloud/
--rw-rw-rw-   0        0        0        0 2023-12-19 05:50:45.000000 logicplum-ai-1.3.8/logicplum/aicloud/__init__.py
--rw-rw-rw-   0        0        0      141 2024-02-15 09:04:54.000000 logicplum-ai-1.3.8/logicplum/aicloud/config.py
-drwxrwxrwx   0        0        0        0 2024-04-02 11:11:03.092364 logicplum-ai-1.3.8/logicplum/aicloud/modeling/
--rw-rw-rw-   0        0        0       97 2023-12-19 05:50:45.000000 logicplum-ai-1.3.8/logicplum/aicloud/modeling/__init__.py
--rw-rw-rw-   0        0        0     5424 2024-03-06 08:02:58.000000 logicplum-ai-1.3.8/logicplum/aicloud/modeling/training.py
-drwxrwxrwx   0        0        0        0 2024-04-02 11:11:03.092364 logicplum-ai-1.3.8/logicplum/aicloud/monitoring/
--rw-rw-rw-   0        0        0       31 2023-12-19 05:50:45.000000 logicplum-ai-1.3.8/logicplum/aicloud/monitoring/__init__.py
--rw-rw-rw-   0        0        0     3552 2024-03-06 08:23:49.000000 logicplum-ai-1.3.8/logicplum/aicloud/monitoring/model_monitoring.py
-drwxrwxrwx   0        0        0        0 2024-04-02 11:11:03.107984 logicplum-ai-1.3.8/logicplum/aicloud/plots/
--rw-rw-rw-   0        0        0       26 2023-12-19 05:50:46.000000 logicplum-ai-1.3.8/logicplum/aicloud/plots/__init__.py
--rw-rw-rw-   0        0        0     3484 2024-03-06 08:24:00.000000 logicplum-ai-1.3.8/logicplum/aicloud/plots/graph_plots.py
-drwxrwxrwx   0        0        0        0 2024-04-02 11:11:03.107984 logicplum-ai-1.3.8/logicplum/aicloud/prediction/
--rw-rw-rw-   0        0        0       29 2023-12-19 05:50:46.000000 logicplum-ai-1.3.8/logicplum/aicloud/prediction/__init__.py
--rw-rw-rw-   0        0        0     2190 2024-03-06 08:32:18.000000 logicplum-ai-1.3.8/logicplum/aicloud/prediction/get_prediction.py
-drwxrwxrwx   0        0        0        0 2024-04-02 11:11:03.107984 logicplum-ai-1.3.8/logicplum/aicloud/reports/
--rw-rw-rw-   0        0        0       25 2023-12-19 05:50:46.000000 logicplum-ai-1.3.8/logicplum/aicloud/reports/__init__.py
--rw-rw-rw-   0        0        0     1482 2024-03-06 08:31:59.000000 logicplum-ai-1.3.8/logicplum/aicloud/reports/get_report.py
-drwxrwxrwx   0        0        0        0 2024-04-02 11:11:03.107984 logicplum-ai-1.3.8/logicplum/aicloud/status/
--rw-rw-rw-   0        0        0       25 2023-12-19 05:50:46.000000 logicplum-ai-1.3.8/logicplum/aicloud/status/__init__.py
--rw-rw-rw-   0        0        0      795 2024-03-06 08:31:52.000000 logicplum-ai-1.3.8/logicplum/aicloud/status/get_status.py
-drwxrwxrwx   0        0        0        0 2024-04-02 11:11:03.107984 logicplum-ai-1.3.8/logicplum/aicloud/users/
--rw-rw-rw-   0        0        0       21 2023-12-19 05:50:46.000000 logicplum-ai-1.3.8/logicplum/aicloud/users/__init__.py
--rw-rw-rw-   0        0        0     1190 2024-03-07 07:29:54.000000 logicplum-ai-1.3.8/logicplum/aicloud/users/client.py
-drwxrwxrwx   0        0        0        0 2024-04-02 11:11:03.123609 logicplum-ai-1.3.8/logicplum_ai.egg-info/
--rw-rw-rw-   0        0        0     2313 2024-04-02 11:11:03.000000 logicplum-ai-1.3.8/logicplum_ai.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      835 2024-04-02 11:11:03.000000 logicplum-ai-1.3.8/logicplum_ai.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-04-02 11:11:03.000000 logicplum-ai-1.3.8/logicplum_ai.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       16 2024-04-02 11:11:03.000000 logicplum-ai-1.3.8/logicplum_ai.egg-info/requires.txt
--rw-rw-rw-   0        0        0       10 2024-04-02 11:11:03.000000 logicplum-ai-1.3.8/logicplum_ai.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2024-04-02 11:11:03.123609 logicplum-ai-1.3.8/setup.cfg
--rw-rw-rw-   0        0        0      561 2024-04-02 11:10:23.000000 logicplum-ai-1.3.8/setup.py
+drwxrwxrwx   0        0        0        0 2024-05-29 05:23:37.286798 logicplum_ai-1.3.9/
+-rw-rw-rw-   0        0        0     2239 2024-05-29 05:23:12.000000 logicplum_ai-1.3.9/CHANGELOG.md
+-rw-rw-rw-   0        0        0     2391 2024-05-29 05:23:37.286798 logicplum_ai-1.3.9/PKG-INFO
+drwxrwxrwx   0        0        0        0 2024-05-29 05:23:37.261654 logicplum_ai-1.3.9/logicplum/
+-rw-rw-rw-   0        0        0        0 2023-12-14 07:41:33.000000 logicplum_ai-1.3.9/logicplum/__init__.py
+drwxrwxrwx   0        0        0        0 2024-05-29 05:23:37.261654 logicplum_ai-1.3.9/logicplum/aicloud/
+-rw-rw-rw-   0        0        0        0 2023-12-19 05:50:45.000000 logicplum_ai-1.3.9/logicplum/aicloud/__init__.py
+-rw-rw-rw-   0        0        0      141 2024-02-15 09:04:54.000000 logicplum_ai-1.3.9/logicplum/aicloud/config.py
+drwxrwxrwx   0        0        0        0 2024-05-29 05:23:37.261654 logicplum_ai-1.3.9/logicplum/aicloud/modeling/
+-rw-rw-rw-   0        0        0       97 2023-12-19 05:50:45.000000 logicplum_ai-1.3.9/logicplum/aicloud/modeling/__init__.py
+-rw-rw-rw-   0        0        0     5704 2024-05-29 05:20:58.000000 logicplum_ai-1.3.9/logicplum/aicloud/modeling/training.py
+drwxrwxrwx   0        0        0        0 2024-05-29 05:23:37.271163 logicplum_ai-1.3.9/logicplum/aicloud/monitoring/
+-rw-rw-rw-   0        0        0       31 2023-12-19 05:50:45.000000 logicplum_ai-1.3.9/logicplum/aicloud/monitoring/__init__.py
+-rw-rw-rw-   0        0        0     3552 2024-03-06 08:23:49.000000 logicplum_ai-1.3.9/logicplum/aicloud/monitoring/model_monitoring.py
+drwxrwxrwx   0        0        0        0 2024-05-29 05:23:37.271163 logicplum_ai-1.3.9/logicplum/aicloud/plots/
+-rw-rw-rw-   0        0        0       26 2023-12-19 05:50:46.000000 logicplum_ai-1.3.9/logicplum/aicloud/plots/__init__.py
+-rw-rw-rw-   0        0        0     3484 2024-03-06 08:24:00.000000 logicplum_ai-1.3.9/logicplum/aicloud/plots/graph_plots.py
+drwxrwxrwx   0        0        0        0 2024-05-29 05:23:37.271163 logicplum_ai-1.3.9/logicplum/aicloud/prediction/
+-rw-rw-rw-   0        0        0       29 2023-12-19 05:50:46.000000 logicplum_ai-1.3.9/logicplum/aicloud/prediction/__init__.py
+-rw-rw-rw-   0        0        0     2628 2024-05-29 05:22:32.000000 logicplum_ai-1.3.9/logicplum/aicloud/prediction/get_prediction.py
+drwxrwxrwx   0        0        0        0 2024-05-29 05:23:37.271163 logicplum_ai-1.3.9/logicplum/aicloud/reports/
+-rw-rw-rw-   0        0        0       25 2023-12-19 05:50:46.000000 logicplum_ai-1.3.9/logicplum/aicloud/reports/__init__.py
+-rw-rw-rw-   0        0        0     1482 2024-03-06 08:31:59.000000 logicplum_ai-1.3.9/logicplum/aicloud/reports/get_report.py
+drwxrwxrwx   0        0        0        0 2024-05-29 05:23:37.271163 logicplum_ai-1.3.9/logicplum/aicloud/status/
+-rw-rw-rw-   0        0        0       25 2023-12-19 05:50:46.000000 logicplum_ai-1.3.9/logicplum/aicloud/status/__init__.py
+-rw-rw-rw-   0        0        0      795 2024-03-06 08:31:52.000000 logicplum_ai-1.3.9/logicplum/aicloud/status/get_status.py
+drwxrwxrwx   0        0        0        0 2024-05-29 05:23:37.271163 logicplum_ai-1.3.9/logicplum/aicloud/users/
+-rw-rw-rw-   0        0        0       21 2023-12-19 05:50:46.000000 logicplum_ai-1.3.9/logicplum/aicloud/users/__init__.py
+-rw-rw-rw-   0        0        0     1190 2024-03-07 07:29:54.000000 logicplum_ai-1.3.9/logicplum/aicloud/users/client.py
+drwxrwxrwx   0        0        0        0 2024-05-29 05:23:37.286798 logicplum_ai-1.3.9/logicplum_ai.egg-info/
+-rw-rw-rw-   0        0        0     2391 2024-05-29 05:23:37.000000 logicplum_ai-1.3.9/logicplum_ai.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      835 2024-05-29 05:23:37.000000 logicplum_ai-1.3.9/logicplum_ai.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-05-29 05:23:37.000000 logicplum_ai-1.3.9/logicplum_ai.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       16 2024-05-29 05:23:37.000000 logicplum_ai-1.3.9/logicplum_ai.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       10 2024-05-29 05:23:37.000000 logicplum_ai-1.3.9/logicplum_ai.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2024-05-29 05:23:37.286798 logicplum_ai-1.3.9/setup.cfg
+-rw-rw-rw-   0        0        0      561 2024-05-29 05:23:18.000000 logicplum_ai-1.3.9/setup.py
```

### Comparing `logicplum-ai-1.3.8/CHANGELOG.md` & `logicplum_ai-1.3.9/CHANGELOG.md`

 * *Files 8% similar despite different names*

```diff
@@ -113,8 +113,11 @@
 ## [1.3.6] - 2023-12-08
 - fixes.
 
 ## [1.3.7] - 2023-12-08
 - fixes.
 
 ## [1.3.8] - 2024-04-02
-- removed unwanted modules.
+- removed unwanted modules.
+
+## [1.3.9] - 2024-04-02
+- added training & prediction cancelling modules.
```

### Comparing `logicplum-ai-1.3.8/PKG-INFO` & `logicplum_ai-1.3.9/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: logicplum-ai
-Version: 1.3.8
+Version: 1.3.9
 Description-Content-Type: text/markdown
 Requires-Dist: requests
 Requires-Dist: Pillow
 
 # Changelog
 
 All notable changes to this project will be documented in this file.
@@ -121,7 +121,10 @@
 - fixes.
 
 ## [1.3.7] - 2023-12-08
 - fixes.
 
 ## [1.3.8] - 2024-04-02
 - removed unwanted modules.
+
+## [1.3.9] - 2024-04-02
+- added training & prediction cancelling modules.
```

### Comparing `logicplum-ai-1.3.8/logicplum/aicloud/modeling/training.py` & `logicplum_ai-1.3.9/logicplum/aicloud/modeling/training.py`

 * *Files 2% similar despite different names*

```diff
@@ -133,8 +133,16 @@
     else:
         return "Something went wrong on service"
 
 def json_check(response):
     if response.status_code != 500 and response.status_code != 400:
         return response.json()
     else:
-        return f"Request failed with status code: {response.status_code}"
+        return f"Request failed with status code: {response.status_code}"
+    
+
+def cancel_training_task(project_id, token):
+    url = f"{base_url}/training/cancel-job/{project_id}"
+    access_token = 'Bearer '+ token
+    headers = {"Authorization": access_token}
+    response = requests.get(url, headers=headers)
+    return json_check(response)
```

### Comparing `logicplum-ai-1.3.8/logicplum/aicloud/monitoring/model_monitoring.py` & `logicplum_ai-1.3.9/logicplum/aicloud/monitoring/model_monitoring.py`

 * *Files identical despite different names*

### Comparing `logicplum-ai-1.3.8/logicplum/aicloud/plots/graph_plots.py` & `logicplum_ai-1.3.9/logicplum/aicloud/plots/graph_plots.py`

 * *Files identical despite different names*

### Comparing `logicplum-ai-1.3.8/logicplum/aicloud/prediction/get_prediction.py` & `logicplum_ai-1.3.9/logicplum/aicloud/prediction/get_prediction.py`

 * *Files 19% similar despite different names*

```diff
@@ -45,7 +45,18 @@
 
 def get_prediction_result(deployment_or_project_id, token, mode):
     if mode.lower() == "quick":
         url = f"{base_url}/prediction/get-prediction-score/{deployment_or_project_id}"
     else:
         url = f"{base_url}/prediction/get-prediction-score/{deployment_or_project_id}"
     return make_request(url, token)
+
+
+def cancel_prediction_task(deployment_id, token):
+    url = f"{base_url}/prediction/cancel-job/{deployment_id}"
+    access_token = 'Bearer '+ token
+    headers = {"Authorization": access_token}
+    response = requests.get(url, headers=headers)
+    if response.status_code != 500 and response.status_code != 400:
+        return response.json()
+    else:
+        return f"Request failed with status code: {response.status_code}"
```

### Comparing `logicplum-ai-1.3.8/logicplum/aicloud/reports/get_report.py` & `logicplum_ai-1.3.9/logicplum/aicloud/reports/get_report.py`

 * *Files identical despite different names*

### Comparing `logicplum-ai-1.3.8/logicplum/aicloud/status/get_status.py` & `logicplum_ai-1.3.9/logicplum/aicloud/status/get_status.py`

 * *Files identical despite different names*

### Comparing `logicplum-ai-1.3.8/logicplum/aicloud/users/client.py` & `logicplum_ai-1.3.9/logicplum/aicloud/users/client.py`

 * *Files identical despite different names*

### Comparing `logicplum-ai-1.3.8/logicplum_ai.egg-info/PKG-INFO` & `logicplum_ai-1.3.9/logicplum_ai.egg-info/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: logicplum-ai
-Version: 1.3.8
+Version: 1.3.9
 Description-Content-Type: text/markdown
 Requires-Dist: requests
 Requires-Dist: Pillow
 
 # Changelog
 
 All notable changes to this project will be documented in this file.
@@ -121,7 +121,10 @@
 - fixes.
 
 ## [1.3.7] - 2023-12-08
 - fixes.
 
 ## [1.3.8] - 2024-04-02
 - removed unwanted modules.
+
+## [1.3.9] - 2024-04-02
+- added training & prediction cancelling modules.
```

### Comparing `logicplum-ai-1.3.8/logicplum_ai.egg-info/SOURCES.txt` & `logicplum_ai-1.3.9/logicplum_ai.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `logicplum-ai-1.3.8/setup.py` & `logicplum_ai-1.3.9/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -4,15 +4,15 @@
 current_dir = os.path.abspath(os.path.dirname(__file__))
 
 with open(os.path.join(current_dir, "CHANGELOG.md"), "r", encoding="utf-8") as f:
     long_description = f.read()
 
 setup(
     name='logicplum-ai',
-    version='1.3.8',  # Update the version number
+    version='1.3.9',  # Update the version number
     packages=find_packages(),
     install_requires=[
         'requests',
         'Pillow'
     ],
     long_description=long_description,
     long_description_content_type="text/markdown",
```

