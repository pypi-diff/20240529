# Comparing `tmp/logos_sdk-0.0.23.tar.gz` & `tmp/logos_sdk-0.0.24.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "logos_sdk-0.0.23.tar", last modified: Mon May 20 08:10:54 2024, max compression
+gzip compressed data, was "logos_sdk-0.0.24.tar", last modified: Wed May 29 10:00:31 2024, max compression
```

## Comparing `logos_sdk-0.0.23.tar` & `logos_sdk-0.0.24.tar`

### file list

```diff
@@ -1,32 +1,32 @@
-drwxr-xr-x   0 W          (501) staff       (20)        0 2024-05-20 08:10:54.024999 logos_sdk-0.0.23/
--rw-r--r--   0 W          (501) staff       (20)     1061 2024-05-16 14:39:43.000000 logos_sdk-0.0.23/LICENSE
--rw-r--r--   0 W          (501) staff       (20)     9876 2024-05-20 08:10:54.024904 logos_sdk-0.0.23/PKG-INFO
--rw-r--r--   0 W          (501) staff       (20)     9230 2024-05-19 08:08:40.000000 logos_sdk-0.0.23/README.md
-drwxr-xr-x   0 W          (501) staff       (20)        0 2024-05-20 08:10:54.021544 logos_sdk-0.0.23/logos_sdk/
--rw-r--r--   0 W          (501) staff       (20)      116 2024-05-16 14:06:44.000000 logos_sdk-0.0.23/logos_sdk/__init__.py
-drwxr-xr-x   0 W          (501) staff       (20)        0 2024-05-20 08:10:54.022412 logos_sdk-0.0.23/logos_sdk/big_query/
--rw-r--r--   0 W          (501) staff       (20)     5498 2024-05-20 07:25:33.000000 logos_sdk-0.0.23/logos_sdk/big_query/BigQuery.py
--rw-r--r--   0 W          (501) staff       (20)      745 2024-01-08 11:17:31.000000 logos_sdk-0.0.23/logos_sdk/big_query/__init__.py
-drwxr-xr-x   0 W          (501) staff       (20)        0 2024-05-20 08:10:54.022683 logos_sdk-0.0.23/logos_sdk/logging/
--rw-r--r--   0 W          (501) staff       (20)     2557 2024-05-16 14:06:44.000000 logos_sdk-0.0.23/logos_sdk/logging/LogosLogger.py
--rw-r--r--   0 W          (501) staff       (20)     2818 2023-09-13 09:34:42.000000 logos_sdk-0.0.23/logos_sdk/logging/__init__.py
-drwxr-xr-x   0 W          (501) staff       (20)        0 2024-05-20 08:10:54.024506 logos_sdk-0.0.23/logos_sdk/services/
--rw-r--r--   0 W          (501) staff       (20)    14319 2024-05-16 14:19:15.000000 logos_sdk-0.0.23/logos_sdk/services/CampaignManager.py
--rw-r--r--   0 W          (501) staff       (20)     7036 2024-05-16 14:06:44.000000 logos_sdk-0.0.23/logos_sdk/services/Collabim.py
--rw-r--r--   0 W          (501) staff       (20)     9572 2024-05-16 14:06:44.000000 logos_sdk-0.0.23/logos_sdk/services/DV360.py
--rw-r--r--   0 W          (501) staff       (20)    15646 2024-05-16 13:55:20.000000 logos_sdk-0.0.23/logos_sdk/services/Facebook.py
--rw-r--r--   0 W          (501) staff       (20)     5600 2024-05-16 13:55:20.000000 logos_sdk-0.0.23/logos_sdk/services/GoogleAds.py
--rw-r--r--   0 W          (501) staff       (20)    12483 2024-05-16 13:55:20.000000 logos_sdk-0.0.23/logos_sdk/services/GoogleSheets.py
--rw-r--r--   0 W          (501) staff       (20)     1151 2024-05-16 13:55:20.000000 logos_sdk-0.0.23/logos_sdk/services/MarketMiner.py
--rw-r--r--   0 W          (501) staff       (20)     6129 2024-05-16 13:55:20.000000 logos_sdk-0.0.23/logos_sdk/services/MerchantCenter.py
--rw-r--r--   0 W          (501) staff       (20)     6899 2024-05-16 13:55:20.000000 logos_sdk-0.0.23/logos_sdk/services/MicrosoftAdvertising.py
--rw-r--r--   0 W          (501) staff       (20)    11621 2024-05-16 13:55:20.000000 logos_sdk-0.0.23/logos_sdk/services/Sklik.py
--rw-r--r--   0 W          (501) staff       (20)     1110 2024-05-16 14:19:15.000000 logos_sdk-0.0.23/logos_sdk/services/__init__.py
-drwxr-xr-x   0 W          (501) staff       (20)        0 2024-05-20 08:10:54.024684 logos_sdk-0.0.23/logos_sdk.egg-info/
--rw-r--r--   0 W          (501) staff       (20)     9876 2024-05-20 08:10:54.000000 logos_sdk-0.0.23/logos_sdk.egg-info/PKG-INFO
--rw-r--r--   0 W          (501) staff       (20)      717 2024-05-20 08:10:54.000000 logos_sdk-0.0.23/logos_sdk.egg-info/SOURCES.txt
--rw-r--r--   0 W          (501) staff       (20)        1 2024-05-20 08:10:54.000000 logos_sdk-0.0.23/logos_sdk.egg-info/dependency_links.txt
--rw-r--r--   0 W          (501) staff       (20)      135 2024-05-20 08:10:54.000000 logos_sdk-0.0.23/logos_sdk.egg-info/requires.txt
--rw-r--r--   0 W          (501) staff       (20)       10 2024-05-20 08:10:54.000000 logos_sdk-0.0.23/logos_sdk.egg-info/top_level.txt
--rw-r--r--   0 W          (501) staff       (20)       79 2024-05-20 08:10:54.025179 logos_sdk-0.0.23/setup.cfg
--rw-r--r--   0 W          (501) staff       (20)     1187 2024-05-16 14:38:17.000000 logos_sdk-0.0.23/setup.py
+drwxrwxrwx   0 root         (0) root         (0)        0 2024-05-29 10:00:31.777952 logos_sdk-0.0.24/
+-rw-rw-rw-   0 root         (0) root         (0)     1061 2024-05-29 10:00:07.000000 logos_sdk-0.0.24/LICENSE
+-rw-r--r--   0 root         (0) root         (0)     9070 2024-05-29 10:00:31.777952 logos_sdk-0.0.24/PKG-INFO
+-rw-rw-rw-   0 root         (0) root         (0)     8425 2024-05-29 10:00:07.000000 logos_sdk-0.0.24/README.md
+drwxrwxrwx   0 root         (0) root         (0)        0 2024-05-29 10:00:31.769952 logos_sdk-0.0.24/logos_sdk/
+-rw-rw-rw-   0 root         (0) root         (0)      113 2024-05-29 10:00:07.000000 logos_sdk-0.0.24/logos_sdk/__init__.py
+drwxrwxrwx   0 root         (0) root         (0)        0 2024-05-29 10:00:31.769952 logos_sdk-0.0.24/logos_sdk/big_query/
+-rw-rw-rw-   0 root         (0) root         (0)     5498 2024-05-29 10:00:07.000000 logos_sdk-0.0.24/logos_sdk/big_query/BigQuery.py
+-rw-rw-rw-   0 root         (0) root         (0)      723 2024-05-29 10:00:07.000000 logos_sdk-0.0.24/logos_sdk/big_query/__init__.py
+drwxrwxrwx   0 root         (0) root         (0)        0 2024-05-29 10:00:31.769952 logos_sdk-0.0.24/logos_sdk/logging/
+-rw-rw-rw-   0 root         (0) root         (0)     2557 2024-05-29 10:00:07.000000 logos_sdk-0.0.24/logos_sdk/logging/LogosLogger.py
+-rw-rw-rw-   0 root         (0) root         (0)     2818 2024-05-29 10:00:07.000000 logos_sdk-0.0.24/logos_sdk/logging/__init__.py
+drwxrwxrwx   0 root         (0) root         (0)        0 2024-05-29 10:00:31.777952 logos_sdk-0.0.24/logos_sdk/services/
+-rw-rw-rw-   0 root         (0) root         (0)    14319 2024-05-29 10:00:07.000000 logos_sdk-0.0.24/logos_sdk/services/CampaignManager.py
+-rw-rw-rw-   0 root         (0) root         (0)     7036 2024-05-29 10:00:07.000000 logos_sdk-0.0.24/logos_sdk/services/Collabim.py
+-rw-rw-rw-   0 root         (0) root         (0)    15566 2024-05-29 10:00:07.000000 logos_sdk-0.0.24/logos_sdk/services/DV360.py
+-rw-rw-rw-   0 root         (0) root         (0)    15233 2024-05-29 10:00:07.000000 logos_sdk-0.0.24/logos_sdk/services/Facebook.py
+-rw-rw-rw-   0 root         (0) root         (0)     5450 2024-05-29 10:00:07.000000 logos_sdk-0.0.24/logos_sdk/services/GoogleAds.py
+-rw-rw-rw-   0 root         (0) root         (0)    12190 2024-05-29 10:00:07.000000 logos_sdk-0.0.24/logos_sdk/services/GoogleSheets.py
+-rw-rw-rw-   0 root         (0) root         (0)     1151 2024-05-29 10:00:07.000000 logos_sdk-0.0.24/logos_sdk/services/MarketMiner.py
+-rw-rw-rw-   0 root         (0) root         (0)     6129 2024-05-29 10:00:07.000000 logos_sdk-0.0.24/logos_sdk/services/MerchantCenter.py
+-rw-rw-rw-   0 root         (0) root         (0)     6721 2024-05-29 10:00:07.000000 logos_sdk-0.0.24/logos_sdk/services/MicrosoftAdvertising.py
+-rw-rw-rw-   0 root         (0) root         (0)    11621 2024-05-29 10:00:07.000000 logos_sdk-0.0.24/logos_sdk/services/Sklik.py
+-rw-rw-rw-   0 root         (0) root         (0)     1110 2024-05-29 10:00:07.000000 logos_sdk-0.0.24/logos_sdk/services/__init__.py
+drwxrwxrwx   0 root         (0) root         (0)        0 2024-05-29 10:00:31.777952 logos_sdk-0.0.24/logos_sdk.egg-info/
+-rw-r--r--   0 root         (0) root         (0)     9070 2024-05-29 10:00:31.000000 logos_sdk-0.0.24/logos_sdk.egg-info/PKG-INFO
+-rw-rw-rw-   0 root         (0) root         (0)      717 2024-05-29 10:00:31.000000 logos_sdk-0.0.24/logos_sdk.egg-info/SOURCES.txt
+-rw-rw-rw-   0 root         (0) root         (0)        1 2024-05-29 10:00:31.000000 logos_sdk-0.0.24/logos_sdk.egg-info/dependency_links.txt
+-rw-rw-rw-   0 root         (0) root         (0)      135 2024-05-29 10:00:31.000000 logos_sdk-0.0.24/logos_sdk.egg-info/requires.txt
+-rw-rw-rw-   0 root         (0) root         (0)       10 2024-05-29 10:00:31.000000 logos_sdk-0.0.24/logos_sdk.egg-info/top_level.txt
+-rw-rw-rw-   0 root         (0) root         (0)       79 2024-05-29 10:00:31.777952 logos_sdk-0.0.24/setup.cfg
+-rw-rw-rw-   0 root         (0) root         (0)     1187 2024-05-29 10:00:07.000000 logos_sdk-0.0.24/setup.py
```

### Comparing `logos_sdk-0.0.23/LICENSE` & `logos_sdk-0.0.24/LICENSE`

 * *Files identical despite different names*

### Comparing `logos_sdk-0.0.23/PKG-INFO` & `logos_sdk-0.0.24/PKG-INFO`

 * *Files 13% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: logos-sdk
-Version: 0.0.23
+Version: 0.0.24
 Summary: SDK for Logos platform
 Home-page: https://bitbucket.org/databy/logos-sdk-pip/src/master/
 Author: Databy.io
 Author-email: admin@proficio.cz
 Classifier: Programming Language :: Python :: 3
 Classifier: Operating System :: OS Independent
 Description-Content-Type: text/markdown
@@ -162,55 +162,56 @@
   
 the URLs of development services (bound to the development branches in BitBucket) are used. On the other hand, if none of these is set, production URLs are called (used in the Cloud production environment).  
   
 # Installation as a dependency to Logos Scripts  
   
 ## Local environment  
   
-This library is hosted as a private package in Google Artifact Registry, only accessible to authorised users - to be able to include it as a pip dependency in a Logos Script requirements.txt file, one must ensure that `google-auth`, `keyring` and `keyrings.google-artifactregistry-auth` packages were pre-installed. These libraries are able to read the contents of `GOOGLE_APPLICATION_CREDENTIALS` environment variable and pull the information necessary for authenticating to Google Artifact Registry when fetching the `logos-sdk` package from the extra index URL.  
-  
-To sum it up, the required steps for installing `logos-sdk` as a dependency are:  
-  
-1. In a Logos Script requirements.txt, put the following:  
-```bash  
---extra-index-url https://europe-west1-python.pkg.dev/logos-382010/logos-sdk/simple logos-sdk  
-  
-logos-sdk=[desired version]  
+This library is hosted as on Pypi.  
+
+logos-sdk=[desired version]/latest
 ```  
 2. Then in your terminal with the venv active, run following:  
 ```bash
-export GOOGLE_APPLICATION_CREDENTIALS=logos-382010-ee0fd6995649.json  
 pip3 install -r requirements.txt  
 export DEVELOPMENT=True  
 ```  
   
 To verify that the library was successfully installed, you can view the installed package information via:  
   
 ```bash  
 pip3 show -f logos-sdk  
 ```  
   
 ## BitBucket pipelines environment  
   
-Firstly, read the local environment setting. If "been there, done that", the setting for BitBucket pipeline testing is very similar. At first, go to pipeline variables in BitBucket UI and create a variable `GOOGLE_CREDENTIALS`, pasting the contents of the `logos-accessor` service account credentials file into it. Then your bitbucket-pipelines.yml testing step should looks like this:  
+Firstly, read the local environment setting. If "been there, done that", the setting for BitBucket pipeline testing is very similar. At first, go to pipeline variables in BitBucket UI and create a variable `GOOGLE_CREDENTIALS`, pasting the contents of the `logos-accessor` service account credentials file into it. Then create `PYPI_CREDENTIALS` and paste this into the secret:
+You also need set the `SERVICES_PATH` for each service.
+```
+[pypi]
+username = __token__
+password = pypi-[api token]
+```
+
+Then your bitbucket-pipelines.yml testing step should look like this:  
   
 ```  
 pipelines:  
 	default:  
 		- step:  
 			name: Test  
 			caches:  
 				- pip  
 			script:  
-				- echo $GOOGLE_CREDENTIALS > logos-382010-ee0fd6995649.json  
-				- export GOOGLE_APPLICATION_CREDENTIALS=$PWD/logos-382010-ee0fd6995649.json  
-				- export TESTING=True  
-				- pip3 install pytest google-auth keyring keyrings.google-artifactregistry-auth  
-				- if [ -f requirements.txt ]; then pip3 install -r requirements.txt; fi  
-				- python3 -m pytest -v tests/* --junitxml=test-reports/report.xml  
+				- echo $GOOGLE_CREDENTIALS > logos-382010-ee0fd6995649.json
+                - echo $PIPY_CREDENTIALS > .pypirc
+                - export GOOGLE_APPLICATION_CREDENTIALS=logos-382010-ee0fd6995649.json
+                - pip3 install -U setuptools wheel twine
+                - python setup.py sdist bdist_wheel
+                - twine upload --config-file .pypirc --verbose dist/* 
 ```  
   
 ## Google Cloud environment  
 Firstly, read the local environment setting. If "been there, done that", your Dockerfile should contain the following steps:  
   
 ```  
 RUN apt-get update && apt-get install -y git  
@@ -228,16 +229,16 @@
 If you are deploying a development cloud instance, in Cloud Run settings, `CLOUD_DEVELOPMENT`needs to be set:
 
 ```bash  
 export CLOUD_DEVELOPMENT=True
 ``` 
 
   
-# Development & versioning  
-This is a versioned package and a version number can only be pushed once into Google Artifact Registry. Development of new features/refactor/debug follow the naming convention of:  
+# Development & versioning
+Development of new features/refactor/debug follow the naming convention of:  
   
 ```  
 "feature/[short name]"  
 "refactor/[short name]"  
 "debug/[short name]"  
 ```
```

### Comparing `logos_sdk-0.0.23/README.md` & `logos_sdk-0.0.24/logos_sdk.egg-info/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,7 +1,29 @@
+Metadata-Version: 2.1
+Name: logos-sdk
+Version: 0.0.24
+Summary: SDK for Logos platform
+Home-page: https://bitbucket.org/databy/logos-sdk-pip/src/master/
+Author: Databy.io
+Author-email: admin@proficio.cz
+Classifier: Programming Language :: Python :: 3
+Classifier: Operating System :: OS Independent
+Description-Content-Type: text/markdown
+License-File: LICENSE
+Requires-Dist: requests
+Requires-Dist: google-auth
+Requires-Dist: google-cloud-logging
+Requires-Dist: google-cloud-bigquery
+Requires-Dist: python-dotenv
+Requires-Dist: google-api-python-client
+Requires-Dist: httplib2
+Requires-Dist: pandas
+Requires-Dist: db-dtypes
+Requires-Dist: numpy
+
 # Logos Software Development Kit  
   
 Logos Software Development Kit (Logos SDK) is a private library encapsulating functionality shared by Logos Scripts - configurable scripts running as Cloud Functions, triggered by Cloud Scheduler, which are controlled and monitored via the Logos UI, as a part of the Logos Ecosystem.  
   
 # Functionality modules  
   
 ## Logging  
@@ -140,55 +162,56 @@
   
 the URLs of development services (bound to the development branches in BitBucket) are used. On the other hand, if none of these is set, production URLs are called (used in the Cloud production environment).  
   
 # Installation as a dependency to Logos Scripts  
   
 ## Local environment  
   
-This library is hosted as a private package in Google Artifact Registry, only accessible to authorised users - to be able to include it as a pip dependency in a Logos Script requirements.txt file, one must ensure that `google-auth`, `keyring` and `keyrings.google-artifactregistry-auth` packages were pre-installed. These libraries are able to read the contents of `GOOGLE_APPLICATION_CREDENTIALS` environment variable and pull the information necessary for authenticating to Google Artifact Registry when fetching the `logos-sdk` package from the extra index URL.  
-  
-To sum it up, the required steps for installing `logos-sdk` as a dependency are:  
-  
-1. In a Logos Script requirements.txt, put the following:  
-```bash  
---extra-index-url https://europe-west1-python.pkg.dev/logos-382010/logos-sdk/simple logos-sdk  
-  
-logos-sdk=[desired version]  
+This library is hosted as on Pypi.  
+
+logos-sdk=[desired version]/latest
 ```  
 2. Then in your terminal with the venv active, run following:  
 ```bash
-export GOOGLE_APPLICATION_CREDENTIALS=logos-382010-ee0fd6995649.json  
 pip3 install -r requirements.txt  
 export DEVELOPMENT=True  
 ```  
   
 To verify that the library was successfully installed, you can view the installed package information via:  
   
 ```bash  
 pip3 show -f logos-sdk  
 ```  
   
 ## BitBucket pipelines environment  
   
-Firstly, read the local environment setting. If "been there, done that", the setting for BitBucket pipeline testing is very similar. At first, go to pipeline variables in BitBucket UI and create a variable `GOOGLE_CREDENTIALS`, pasting the contents of the `logos-accessor` service account credentials file into it. Then your bitbucket-pipelines.yml testing step should looks like this:  
+Firstly, read the local environment setting. If "been there, done that", the setting for BitBucket pipeline testing is very similar. At first, go to pipeline variables in BitBucket UI and create a variable `GOOGLE_CREDENTIALS`, pasting the contents of the `logos-accessor` service account credentials file into it. Then create `PYPI_CREDENTIALS` and paste this into the secret:
+You also need set the `SERVICES_PATH` for each service.
+```
+[pypi]
+username = __token__
+password = pypi-[api token]
+```
+
+Then your bitbucket-pipelines.yml testing step should look like this:  
   
 ```  
 pipelines:  
 	default:  
 		- step:  
 			name: Test  
 			caches:  
 				- pip  
 			script:  
-				- echo $GOOGLE_CREDENTIALS > logos-382010-ee0fd6995649.json  
-				- export GOOGLE_APPLICATION_CREDENTIALS=$PWD/logos-382010-ee0fd6995649.json  
-				- export TESTING=True  
-				- pip3 install pytest google-auth keyring keyrings.google-artifactregistry-auth  
-				- if [ -f requirements.txt ]; then pip3 install -r requirements.txt; fi  
-				- python3 -m pytest -v tests/* --junitxml=test-reports/report.xml  
+				- echo $GOOGLE_CREDENTIALS > logos-382010-ee0fd6995649.json
+                - echo $PIPY_CREDENTIALS > .pypirc
+                - export GOOGLE_APPLICATION_CREDENTIALS=logos-382010-ee0fd6995649.json
+                - pip3 install -U setuptools wheel twine
+                - python setup.py sdist bdist_wheel
+                - twine upload --config-file .pypirc --verbose dist/* 
 ```  
   
 ## Google Cloud environment  
 Firstly, read the local environment setting. If "been there, done that", your Dockerfile should contain the following steps:  
   
 ```  
 RUN apt-get update && apt-get install -y git  
@@ -206,17 +229,17 @@
 If you are deploying a development cloud instance, in Cloud Run settings, `CLOUD_DEVELOPMENT`needs to be set:
 
 ```bash  
 export CLOUD_DEVELOPMENT=True
 ``` 
 
   
-# Development & versioning  
-This is a versioned package and a version number can only be pushed once into Google Artifact Registry. Development of new features/refactor/debug follow the naming convention of:  
+# Development & versioning
+Development of new features/refactor/debug follow the naming convention of:  
   
 ```  
 "feature/[short name]"  
 "refactor/[short name]"  
 "debug/[short name]"  
 ```  
   
-Pull requests are directed do the current development branch, which always bears the number of the newest version, for example `development-0.0.2`.  After adding a major feature, or a number of less significant refactors and hot-fixes, the current development branch is merged into master and deployed into Google Artifact Registry. The old development branch is then deleted and a  new branch with the following version `development-0.0.3` will be created, and the first commit must include changing of  the version in the `setup.py` file.
+Pull requests are directed do the current development branch, which always bears the number of the newest version, for example `development-0.0.2`.  After adding a major feature, or a number of less significant refactors and hot-fixes, the current development branch is merged into master and deployed into Google Artifact Registry. The old development branch is then deleted and a  new branch with the following version `development-0.0.3` will be created, and the first commit must include changing of  the version in the `setup.py` file.
```

### Comparing `logos_sdk-0.0.23/logos_sdk/big_query/BigQuery.py` & `logos_sdk-0.0.24/logos_sdk/big_query/BigQuery.py`

 * *Files identical despite different names*

### Comparing `logos_sdk-0.0.23/logos_sdk/big_query/__init__.py` & `logos_sdk-0.0.24/logos_sdk/big_query/__init__.py`

 * *Ordering differences only*

 * *Files 26% similar despite different names*

```diff
@@ -1,22 +1,22 @@
-from functools import wraps
-from google.api_core.exceptions import NotFound
-import time
-
-MAX_NUMBER_OF_ATTEMPTS = 2
-
-
-def retry_on_not_found(wrapped_function):
-    """This decorator retry call when table is not found. Insert into newly created table often fails with error
-    because API probably needs few seconds to see new created table"""
-
-    @wraps(wrapped_function)
-    def inner(*args, **kwargs):
-        for i in range(1, MAX_NUMBER_OF_ATTEMPTS + 1):
-            try:
-                kwargs["attempts"] = i
-                return wrapped_function(*args, **kwargs)
-                # this is because all request share same service
-            except NotFound as err:
-                time.sleep(2)
-
-    return inner
+from functools import wraps
+from google.api_core.exceptions import NotFound
+import time
+
+MAX_NUMBER_OF_ATTEMPTS = 2
+
+
+def retry_on_not_found(wrapped_function):
+    """This decorator retry call when table is not found. Insert into newly created table often fails with error
+    because API probably needs few seconds to see new created table"""
+
+    @wraps(wrapped_function)
+    def inner(*args, **kwargs):
+        for i in range(1, MAX_NUMBER_OF_ATTEMPTS + 1):
+            try:
+                kwargs["attempts"] = i
+                return wrapped_function(*args, **kwargs)
+                # this is because all request share same service
+            except NotFound as err:
+                time.sleep(2)
+
+    return inner
```

### Comparing `logos_sdk-0.0.23/logos_sdk/logging/LogosLogger.py` & `logos_sdk-0.0.24/logos_sdk/logging/LogosLogger.py`

 * *Files identical despite different names*

### Comparing `logos_sdk-0.0.23/logos_sdk/logging/__init__.py` & `logos_sdk-0.0.24/logos_sdk/logging/__init__.py`

 * *Files identical despite different names*

### Comparing `logos_sdk-0.0.23/logos_sdk/services/CampaignManager.py` & `logos_sdk-0.0.24/logos_sdk/services/CampaignManager.py`

 * *Files identical despite different names*

### Comparing `logos_sdk-0.0.23/logos_sdk/services/Collabim.py` & `logos_sdk-0.0.24/logos_sdk/services/Collabim.py`

 * *Files identical despite different names*

### Comparing `logos_sdk-0.0.23/logos_sdk/services/Facebook.py` & `logos_sdk-0.0.24/logos_sdk/services/Facebook.py`

 * *Ordering differences only*

 * *Files 21% similar despite different names*

```diff
@@ -1,413 +1,413 @@
-from requests import request
-from typing import List, Dict, Optional
-from logos_sdk.services import get_headers
-from http import HTTPStatus
-from random import randint
-from dotenv import load_dotenv
-import os
-import time
-
-
-class FacebookServiceException(Exception):
-    pass
-
-
-class FacebookService:
-    def __init__(self, url=None):
-        load_dotenv()
-        self._URL = url or os.environ.get("FACEBOOK_SERVICE_PATH")
-        self._ACCESSIBLE_ACCOUNTS = self._URL + "/accessible-accounts"
-        self._INSIGHTS = self._URL + "/insights"
-        self._LINK_URLS = self._URL + "/link-urls"
-        self._ACCESSIBLE_BUSINESSES = self._URL + "/accessible-businesses"
-        self._PRODUCT_CATALOGS = self._URL + "/product-catalogs"
-        self._PRODUCT_CATALOG = self._URL + "/product-catalog"
-        self._PRODUCTS = self._URL + "/products"
-        self._FEEDS = self._URL + "/feeds"
-        self._FEED_ERRORS = self._URL + "/feed-errors"
-        self._FEED_ERRORS_REPORT_STATUS = self._URL + "/feed-errors-report-status"
-        self._FEED_ERRORS_REPORT = self._URL + "/feed-errors-report"
-
-    def get_accessible_accounts(
-        self, secret_id: str, timeout: int = None
-    ) -> List[Dict]:
-        """
-        Get all accessible accounts
-        :param secret_id The ID of the secret in secret manager
-        :param timeout Cut the request if it takes too long
-        :return: all accessible accounts List(Dict)
-        """
-
-        body = {"secret_id": secret_id}
-
-        header = get_headers(self._ACCESSIBLE_ACCOUNTS)
-
-        response = request(
-            "post",
-            url=self._ACCESSIBLE_ACCOUNTS,
-            json=body,
-            headers=header,
-            timeout=timeout,
-        )
-
-        if response.status_code == HTTPStatus.OK:
-            service_response = response.json()
-            return service_response["data"]
-        else:
-            raise FacebookServiceException(response.content)
-
-    def get_insights(
-        self,
-        account_id: str,
-        secret_id: str,
-        date_from: str,
-        date_to: str,
-        report_columns: List[str],
-        breakdowns: List[str],
-        filter_columns: List[Dict],
-        level: str = None,
-        timeout: int = None,
-    ) -> List[Dict]:
-        """
-        Get Facebook Ads Insights according to configuration
-        :param account_id The id of the ad account
-        :param secret_id The ID of the secret in secret manager
-        :param date_from The date from
-        :param date_to The date to
-        :param report_columns Required and available fields for report
-        :param breakdowns Group the Insights API results into different sets using breakdowns
-        :param filter_columns Option for filtering results according to specified conditions
-        :param level Set the entity level for insights report
-        :param timeout Cut the request if it takes too long
-        :return Facebook Ads Insights List(Dict)
-        """
-        body = {
-            "account_id": account_id,
-            "date_from": date_from,
-            "secret_id": secret_id,
-            "date_to": date_to,
-            "report_columns": report_columns,
-            "breakdowns": breakdowns,
-            "filter": filter_columns,
-        }
-        if level is not None:
-            body["level"] = level
-        header = get_headers(self._INSIGHTS)
-
-        response = request(
-            "post", url=self._INSIGHTS, json=body, headers=header, timeout=timeout
-        )
-        if response.status_code == HTTPStatus.OK:
-            service_response = response.json()
-            return service_response["data"]
-        else:
-            raise FacebookServiceException(response.content)
-
-    def get_link_urls(
-        self,
-        account_id: str,
-        secret_id: str,
-        date_from: str,
-        date_to: str,
-        report_columns: List[str],
-        filter_columns: List[Dict],
-        timeout: int = None,
-    ) -> List[Dict]:
-        """
-        Get Facebook Ads Insights according to configuration together with ad link urls
-        :param account_id The id of the ad account
-        :param secret_id The ID of the secret in secret manager
-        :param date_from The date from
-        :param date_to The date to
-        :param report_columns Required and available fields for report
-        :param filter_columns Option for filtering results according to specified conditions
-        :param timeout Cut the request if it takes too long
-        :return Facebook Ads Insights with ad link urls List(Dict)
-        """
-        body = {
-            "account_id": account_id,
-            "date_from": date_from,
-            "secret_id": secret_id,
-            "date_to": date_to,
-            "report_columns": report_columns,
-            "filter": filter_columns,
-        }
-
-        header = get_headers(self._LINK_URLS)
-
-        response = request(
-            "post", url=self._LINK_URLS, json=body, headers=header, timeout=timeout
-        )
-
-        if response.status_code == HTTPStatus.OK:
-            service_response = response.json()
-            return service_response["data"]
-        else:
-            raise FacebookServiceException(response.content)
-
-    def get_accessible_businesses(
-        self, secret_id: str, report_columns: List[str], timeout: int = None
-    ) -> List[Dict]:
-        """
-        Get all accessible business entities for the user. Business id is required parameter for requesting connected
-        product catalogs
-        :param secret_id The ID of the secret in secret manager
-        :param report_columns Required and available fields for report
-        :param timeout Cut the request if it takes too long
-        :return: all accessible business entities for the user List(Dict)
-        """
-        body = {"secret_id": secret_id, "report_columns": report_columns}
-
-        header = get_headers(self._ACCESSIBLE_BUSINESSES)
-
-        response = request(
-            "post",
-            url=self._ACCESSIBLE_BUSINESSES,
-            json=body,
-            headers=header,
-            timeout=timeout,
-        )
-        if response.status_code == HTTPStatus.OK:
-            service_response = response.json()
-            return service_response["data"]
-        else:
-            raise FacebookServiceException(response.content)
-
-    def get_product_catalogs(
-        self,
-        secret_id: str,
-        business_id: str,
-        report_columns: List[str],
-        filter_columns: List[Dict],
-        timeout: int = None,
-    ) -> List[Dict]:
-        """
-        Get product catalogs for the selected business
-        :param secret_id The ID of the secret in secret manager
-        :param business_id Business id is required parameter for requesting connected product catalogs
-        :param report_columns Required and available fields for report
-        :param filter_columns Option for filtering results according to specified conditions
-        :param timeout Cut the request if it takes too long
-        :return: product catalogs for the selected business List(Dict)
-        """
-        body = {
-            "secret_id": secret_id,
-            "report_columns": report_columns,
-            "filter": filter_columns,
-            "business_id": business_id,
-        }
-
-        header = get_headers(self._PRODUCT_CATALOGS)
-
-        response = request(
-            "post",
-            url=self._PRODUCT_CATALOGS,
-            json=body,
-            headers=header,
-            timeout=timeout,
-        )
-        if response.status_code == HTTPStatus.OK:
-            service_response = response.json()
-            return service_response["data"]
-        else:
-            raise FacebookServiceException(response.content)
-
-    def get_product_catalog(
-        self,
-        secret_id: str,
-        catalog_id: str,
-        report_columns: List[str],
-        timeout: int = None,
-    ) -> List[Dict]:
-        """
-        Retrieves product catalog by catalog ID
-        :param secret_id The ID of the secret in secret manager
-        :param catalog_id Catalog id of catalog to retrieve
-        :param report_columns Required and available fields for report
-        :param timeout Cut the request if it takes too long
-        :return: product catalog List(Dict)
-        """
-        body = {
-            "secret_id": secret_id,
-            "report_columns": report_columns,
-            "catalog_id": catalog_id,
-        }
-
-        header = get_headers(self._PRODUCT_CATALOG)
-
-        response = request(
-            "post",
-            url=self._PRODUCT_CATALOG,
-            json=body,
-            headers=header,
-            timeout=timeout,
-        )
-        if response.status_code == HTTPStatus.OK:
-            service_response = response.json()
-            return service_response["data"]
-        else:
-            raise FacebookServiceException(response.content)
-
-    def products(
-        self,
-        secret_id: str,
-        catalog_id: str,
-        report_columns: List[str],
-        filter_columns: Optional[Dict[str, Dict]],
-        error_priority: Optional[str] = None,
-        timeout: int = None,
-    ) -> List[Dict]:
-        """
-        Returns products for the selected product catalog
-        :param secret_id: The ID of the secret in secret manager
-        :param catalog_id: Catalog id is required parameter for requesting connected products
-        :param report_columns: Required and available fields for report
-        :param filter_columns: Option for filtering results according to specified conditions
-        :param error_priority: Use for filtering product with issues. Possible values: "HIGH", "MEDIUM", "LOW"
-        :param timeout Cut the request if it takes too long
-        :return: List(Dict)
-        """
-        body = {
-            "secret_id": secret_id,
-            "report_columns": report_columns,
-            "filter": filter_columns,
-            "catalog_id": catalog_id,
-            "error_priority": error_priority,
-        }
-
-        header = get_headers(self._PRODUCTS)
-
-        response = request(
-            "post", url=self._PRODUCTS, json=body, headers=header, timeout=timeout
-        )
-        if response.status_code == HTTPStatus.OK:
-            service_response = response.json()
-            return service_response["data"]
-        else:
-            raise FacebookServiceException(response.content)
-
-    def get_feeds(
-        self, secret_id: str, catalog_id: str, timeout: int = None
-    ) -> List[Dict]:
-        """
-        Returns available feeds for selected product catalog.
-        :param secret_id The ID of the secret in secret manager
-        :param catalog_id Catalog id is required parameter for requesting connected products
-        :param timeout Cut the request if it takes too long
-        """
-        body = {"secret_id": secret_id, "catalog_id": catalog_id}
-
-        header = get_headers(self._FEEDS)
-        response = request(
-            "post", url=self._FEEDS, json=body, headers=header, timeout=timeout
-        )
-
-        if response.status_code == HTTPStatus.OK:
-            service_response = response.json()
-            return service_response["data"]
-        else:
-            raise FacebookServiceException(response.content)
-
-    def get_feed_errors(
-        self, secret_id: str, feed_id: str, timeout: int = None
-    ) -> Dict:
-        """
-        Returns count of errors and status for detailed error report for the newest run of feed upload for selected feed.
-        If the error count is greater than 0 this endpoint initiates creation of the detailed error report.
-        :param secret_id The ID of the secret in secret manager
-        :param feed_id ID of the selected feed
-        :param timeout Cut the request if it takes too long
-        """
-        body = {"secret_id": secret_id, "feed_id": feed_id}
-
-        header = get_headers(self._FEED_ERRORS)
-        response = request(
-            "post", url=self._FEED_ERRORS, json=body, headers=header, timeout=timeout
-        )
-
-        if response.status_code == HTTPStatus.OK:
-            service_response = response.json()
-            return service_response["data"]
-        else:
-            raise FacebookServiceException(response.content)
-
-    def get_feed_errors_report_status(
-        self, secret_id: str, feed_id: str, timeout: int = None
-    ) -> Dict:
-        """
-        Returns status for detailed error report for the newest run of feed upload for selected feed.
-        :param secret_id The ID of the secret in secret manager
-        :param feed_id ID of the selected feed
-        :param timeout Cut the request if it takes too long
-        """
-        body = {"secret_id": secret_id, "feed_id": feed_id}
-
-        header = get_headers(self._FEED_ERRORS_REPORT_STATUS)
-        response = request(
-            "post",
-            url=self._FEED_ERRORS_REPORT_STATUS,
-            json=body,
-            headers=header,
-            timeout=timeout,
-        )
-
-        if response.status_code == HTTPStatus.OK:
-            service_response = response.json()
-            return service_response["data"]
-        else:
-            raise FacebookServiceException(response.content)
-
-    def get_feed_errors_report(
-        self, secret_id: str, feed_id: str, timeout: int = None
-    ) -> List[Dict]:
-        """
-        When status of the feed error report is 'WRITE_FINISHED' or 'PARTIAL_WRITE_FINISHED' returns detailed list
-        of possible feed upload errors with description and hints for correction.
-        Otherwise, it returns just the count of errors with the current error report status.
-        :param secret_id The ID of the secret in secret manager
-        :param feed_id ID of the selected feed
-        :param timeout Cut the request if it takes too long
-        """
-        body = {"secret_id": secret_id, "feed_id": feed_id}
-
-        header = get_headers(self._FEED_ERRORS_REPORT)
-        response = request(
-            "post",
-            url=self._FEED_ERRORS_REPORT,
-            json=body,
-            headers=header,
-            timeout=timeout,
-        )
-
-        if response.status_code == HTTPStatus.OK:
-            service_response = response.json()
-            return service_response["data"]
-        else:
-            raise FacebookServiceException(response.content)
-
-    def check_feed_errors_report_ready_with_exponential_backoff(
-        self,
-        secret_id: str,
-        feed_id: str,
-        backoff_attempts: int = 10,
-        timeout: int = None,
-    ) -> Dict:
-        """
-        Implements exponential backoff for pooling the API for readiness of the report, suggested in
-        algorithm suggested by https://developers.google.com/doubleclick-advertisers/upload#exp-backoff
-        :param secret_id: The ID of the secret in secret manager
-        :param feed_id: ID of the selected feed
-        :param backoff_attempts: Number of attempts in checking the report status
-        :param timeout Cut the request if it takes too long
-        :return Bool
-        """
-        for attempt in range(0, backoff_attempts):
-            if (
-                self.get_feed_errors_report_status(secret_id, feed_id, timeout=timeout)
-                == "WRITE_FINISHED"
-            ):
-                return True
-            else:
-                time.sleep((2**attempt) + randint(1, 20))
-
-        return False
+from requests import request
+from typing import List, Dict, Optional
+from logos_sdk.services import get_headers
+from http import HTTPStatus
+from random import randint
+from dotenv import load_dotenv
+import os
+import time
+
+
+class FacebookServiceException(Exception):
+    pass
+
+
+class FacebookService:
+    def __init__(self, url=None):
+        load_dotenv()
+        self._URL = url or os.environ.get("FACEBOOK_SERVICE_PATH")
+        self._ACCESSIBLE_ACCOUNTS = self._URL + "/accessible-accounts"
+        self._INSIGHTS = self._URL + "/insights"
+        self._LINK_URLS = self._URL + "/link-urls"
+        self._ACCESSIBLE_BUSINESSES = self._URL + "/accessible-businesses"
+        self._PRODUCT_CATALOGS = self._URL + "/product-catalogs"
+        self._PRODUCT_CATALOG = self._URL + "/product-catalog"
+        self._PRODUCTS = self._URL + "/products"
+        self._FEEDS = self._URL + "/feeds"
+        self._FEED_ERRORS = self._URL + "/feed-errors"
+        self._FEED_ERRORS_REPORT_STATUS = self._URL + "/feed-errors-report-status"
+        self._FEED_ERRORS_REPORT = self._URL + "/feed-errors-report"
+
+    def get_accessible_accounts(
+        self, secret_id: str, timeout: int = None
+    ) -> List[Dict]:
+        """
+        Get all accessible accounts
+        :param secret_id The ID of the secret in secret manager
+        :param timeout Cut the request if it takes too long
+        :return: all accessible accounts List(Dict)
+        """
+
+        body = {"secret_id": secret_id}
+
+        header = get_headers(self._ACCESSIBLE_ACCOUNTS)
+
+        response = request(
+            "post",
+            url=self._ACCESSIBLE_ACCOUNTS,
+            json=body,
+            headers=header,
+            timeout=timeout,
+        )
+
+        if response.status_code == HTTPStatus.OK:
+            service_response = response.json()
+            return service_response["data"]
+        else:
+            raise FacebookServiceException(response.content)
+
+    def get_insights(
+        self,
+        account_id: str,
+        secret_id: str,
+        date_from: str,
+        date_to: str,
+        report_columns: List[str],
+        breakdowns: List[str],
+        filter_columns: List[Dict],
+        level: str = None,
+        timeout: int = None,
+    ) -> List[Dict]:
+        """
+        Get Facebook Ads Insights according to configuration
+        :param account_id The id of the ad account
+        :param secret_id The ID of the secret in secret manager
+        :param date_from The date from
+        :param date_to The date to
+        :param report_columns Required and available fields for report
+        :param breakdowns Group the Insights API results into different sets using breakdowns
+        :param filter_columns Option for filtering results according to specified conditions
+        :param level Set the entity level for insights report
+        :param timeout Cut the request if it takes too long
+        :return Facebook Ads Insights List(Dict)
+        """
+        body = {
+            "account_id": account_id,
+            "date_from": date_from,
+            "secret_id": secret_id,
+            "date_to": date_to,
+            "report_columns": report_columns,
+            "breakdowns": breakdowns,
+            "filter": filter_columns,
+        }
+        if level is not None:
+            body["level"] = level
+        header = get_headers(self._INSIGHTS)
+
+        response = request(
+            "post", url=self._INSIGHTS, json=body, headers=header, timeout=timeout
+        )
+        if response.status_code == HTTPStatus.OK:
+            service_response = response.json()
+            return service_response["data"]
+        else:
+            raise FacebookServiceException(response.content)
+
+    def get_link_urls(
+        self,
+        account_id: str,
+        secret_id: str,
+        date_from: str,
+        date_to: str,
+        report_columns: List[str],
+        filter_columns: List[Dict],
+        timeout: int = None,
+    ) -> List[Dict]:
+        """
+        Get Facebook Ads Insights according to configuration together with ad link urls
+        :param account_id The id of the ad account
+        :param secret_id The ID of the secret in secret manager
+        :param date_from The date from
+        :param date_to The date to
+        :param report_columns Required and available fields for report
+        :param filter_columns Option for filtering results according to specified conditions
+        :param timeout Cut the request if it takes too long
+        :return Facebook Ads Insights with ad link urls List(Dict)
+        """
+        body = {
+            "account_id": account_id,
+            "date_from": date_from,
+            "secret_id": secret_id,
+            "date_to": date_to,
+            "report_columns": report_columns,
+            "filter": filter_columns,
+        }
+
+        header = get_headers(self._LINK_URLS)
+
+        response = request(
+            "post", url=self._LINK_URLS, json=body, headers=header, timeout=timeout
+        )
+
+        if response.status_code == HTTPStatus.OK:
+            service_response = response.json()
+            return service_response["data"]
+        else:
+            raise FacebookServiceException(response.content)
+
+    def get_accessible_businesses(
+        self, secret_id: str, report_columns: List[str], timeout: int = None
+    ) -> List[Dict]:
+        """
+        Get all accessible business entities for the user. Business id is required parameter for requesting connected
+        product catalogs
+        :param secret_id The ID of the secret in secret manager
+        :param report_columns Required and available fields for report
+        :param timeout Cut the request if it takes too long
+        :return: all accessible business entities for the user List(Dict)
+        """
+        body = {"secret_id": secret_id, "report_columns": report_columns}
+
+        header = get_headers(self._ACCESSIBLE_BUSINESSES)
+
+        response = request(
+            "post",
+            url=self._ACCESSIBLE_BUSINESSES,
+            json=body,
+            headers=header,
+            timeout=timeout,
+        )
+        if response.status_code == HTTPStatus.OK:
+            service_response = response.json()
+            return service_response["data"]
+        else:
+            raise FacebookServiceException(response.content)
+
+    def get_product_catalogs(
+        self,
+        secret_id: str,
+        business_id: str,
+        report_columns: List[str],
+        filter_columns: List[Dict],
+        timeout: int = None,
+    ) -> List[Dict]:
+        """
+        Get product catalogs for the selected business
+        :param secret_id The ID of the secret in secret manager
+        :param business_id Business id is required parameter for requesting connected product catalogs
+        :param report_columns Required and available fields for report
+        :param filter_columns Option for filtering results according to specified conditions
+        :param timeout Cut the request if it takes too long
+        :return: product catalogs for the selected business List(Dict)
+        """
+        body = {
+            "secret_id": secret_id,
+            "report_columns": report_columns,
+            "filter": filter_columns,
+            "business_id": business_id,
+        }
+
+        header = get_headers(self._PRODUCT_CATALOGS)
+
+        response = request(
+            "post",
+            url=self._PRODUCT_CATALOGS,
+            json=body,
+            headers=header,
+            timeout=timeout,
+        )
+        if response.status_code == HTTPStatus.OK:
+            service_response = response.json()
+            return service_response["data"]
+        else:
+            raise FacebookServiceException(response.content)
+
+    def get_product_catalog(
+        self,
+        secret_id: str,
+        catalog_id: str,
+        report_columns: List[str],
+        timeout: int = None,
+    ) -> List[Dict]:
+        """
+        Retrieves product catalog by catalog ID
+        :param secret_id The ID of the secret in secret manager
+        :param catalog_id Catalog id of catalog to retrieve
+        :param report_columns Required and available fields for report
+        :param timeout Cut the request if it takes too long
+        :return: product catalog List(Dict)
+        """
+        body = {
+            "secret_id": secret_id,
+            "report_columns": report_columns,
+            "catalog_id": catalog_id,
+        }
+
+        header = get_headers(self._PRODUCT_CATALOG)
+
+        response = request(
+            "post",
+            url=self._PRODUCT_CATALOG,
+            json=body,
+            headers=header,
+            timeout=timeout,
+        )
+        if response.status_code == HTTPStatus.OK:
+            service_response = response.json()
+            return service_response["data"]
+        else:
+            raise FacebookServiceException(response.content)
+
+    def products(
+        self,
+        secret_id: str,
+        catalog_id: str,
+        report_columns: List[str],
+        filter_columns: Optional[Dict[str, Dict]],
+        error_priority: Optional[str] = None,
+        timeout: int = None,
+    ) -> List[Dict]:
+        """
+        Returns products for the selected product catalog
+        :param secret_id: The ID of the secret in secret manager
+        :param catalog_id: Catalog id is required parameter for requesting connected products
+        :param report_columns: Required and available fields for report
+        :param filter_columns: Option for filtering results according to specified conditions
+        :param error_priority: Use for filtering product with issues. Possible values: "HIGH", "MEDIUM", "LOW"
+        :param timeout Cut the request if it takes too long
+        :return: List(Dict)
+        """
+        body = {
+            "secret_id": secret_id,
+            "report_columns": report_columns,
+            "filter": filter_columns,
+            "catalog_id": catalog_id,
+            "error_priority": error_priority,
+        }
+
+        header = get_headers(self._PRODUCTS)
+
+        response = request(
+            "post", url=self._PRODUCTS, json=body, headers=header, timeout=timeout
+        )
+        if response.status_code == HTTPStatus.OK:
+            service_response = response.json()
+            return service_response["data"]
+        else:
+            raise FacebookServiceException(response.content)
+
+    def get_feeds(
+        self, secret_id: str, catalog_id: str, timeout: int = None
+    ) -> List[Dict]:
+        """
+        Returns available feeds for selected product catalog.
+        :param secret_id The ID of the secret in secret manager
+        :param catalog_id Catalog id is required parameter for requesting connected products
+        :param timeout Cut the request if it takes too long
+        """
+        body = {"secret_id": secret_id, "catalog_id": catalog_id}
+
+        header = get_headers(self._FEEDS)
+        response = request(
+            "post", url=self._FEEDS, json=body, headers=header, timeout=timeout
+        )
+
+        if response.status_code == HTTPStatus.OK:
+            service_response = response.json()
+            return service_response["data"]
+        else:
+            raise FacebookServiceException(response.content)
+
+    def get_feed_errors(
+        self, secret_id: str, feed_id: str, timeout: int = None
+    ) -> Dict:
+        """
+        Returns count of errors and status for detailed error report for the newest run of feed upload for selected feed.
+        If the error count is greater than 0 this endpoint initiates creation of the detailed error report.
+        :param secret_id The ID of the secret in secret manager
+        :param feed_id ID of the selected feed
+        :param timeout Cut the request if it takes too long
+        """
+        body = {"secret_id": secret_id, "feed_id": feed_id}
+
+        header = get_headers(self._FEED_ERRORS)
+        response = request(
+            "post", url=self._FEED_ERRORS, json=body, headers=header, timeout=timeout
+        )
+
+        if response.status_code == HTTPStatus.OK:
+            service_response = response.json()
+            return service_response["data"]
+        else:
+            raise FacebookServiceException(response.content)
+
+    def get_feed_errors_report_status(
+        self, secret_id: str, feed_id: str, timeout: int = None
+    ) -> Dict:
+        """
+        Returns status for detailed error report for the newest run of feed upload for selected feed.
+        :param secret_id The ID of the secret in secret manager
+        :param feed_id ID of the selected feed
+        :param timeout Cut the request if it takes too long
+        """
+        body = {"secret_id": secret_id, "feed_id": feed_id}
+
+        header = get_headers(self._FEED_ERRORS_REPORT_STATUS)
+        response = request(
+            "post",
+            url=self._FEED_ERRORS_REPORT_STATUS,
+            json=body,
+            headers=header,
+            timeout=timeout,
+        )
+
+        if response.status_code == HTTPStatus.OK:
+            service_response = response.json()
+            return service_response["data"]
+        else:
+            raise FacebookServiceException(response.content)
+
+    def get_feed_errors_report(
+        self, secret_id: str, feed_id: str, timeout: int = None
+    ) -> List[Dict]:
+        """
+        When status of the feed error report is 'WRITE_FINISHED' or 'PARTIAL_WRITE_FINISHED' returns detailed list
+        of possible feed upload errors with description and hints for correction.
+        Otherwise, it returns just the count of errors with the current error report status.
+        :param secret_id The ID of the secret in secret manager
+        :param feed_id ID of the selected feed
+        :param timeout Cut the request if it takes too long
+        """
+        body = {"secret_id": secret_id, "feed_id": feed_id}
+
+        header = get_headers(self._FEED_ERRORS_REPORT)
+        response = request(
+            "post",
+            url=self._FEED_ERRORS_REPORT,
+            json=body,
+            headers=header,
+            timeout=timeout,
+        )
+
+        if response.status_code == HTTPStatus.OK:
+            service_response = response.json()
+            return service_response["data"]
+        else:
+            raise FacebookServiceException(response.content)
+
+    def check_feed_errors_report_ready_with_exponential_backoff(
+        self,
+        secret_id: str,
+        feed_id: str,
+        backoff_attempts: int = 10,
+        timeout: int = None,
+    ) -> Dict:
+        """
+        Implements exponential backoff for pooling the API for readiness of the report, suggested in
+        algorithm suggested by https://developers.google.com/doubleclick-advertisers/upload#exp-backoff
+        :param secret_id: The ID of the secret in secret manager
+        :param feed_id: ID of the selected feed
+        :param backoff_attempts: Number of attempts in checking the report status
+        :param timeout Cut the request if it takes too long
+        :return Bool
+        """
+        for attempt in range(0, backoff_attempts):
+            if (
+                self.get_feed_errors_report_status(secret_id, feed_id, timeout=timeout)
+                == "WRITE_FINISHED"
+            ):
+                return True
+            else:
+                time.sleep((2**attempt) + randint(1, 20))
+
+        return False
```

### Comparing `logos_sdk-0.0.23/logos_sdk/services/GoogleAds.py` & `logos_sdk-0.0.24/logos_sdk/services/GoogleAds.py`

 * *Ordering differences only*

 * *Files 22% similar despite different names*

```diff
@@ -1,150 +1,150 @@
-from requests import request
-from typing import List, Union, Dict
-from logos_sdk.services import get_headers
-from http import HTTPStatus
-from dotenv import load_dotenv
-import os
-
-
-class GoogleAdsServiceException(Exception):
-    pass
-
-
-class GoogleAdsService:
-    def __init__(self, url=None):
-        load_dotenv()
-        self._URL = url or os.environ.get("GOOGLE_ADS_SERVICE_PATH")
-        self._SEARCH_STREAM = self._URL + "/search-stream"
-        self._SEARCH = self._URL + "/search"
-        self._EXCLUDE_FOR_ACCOUNT = self._URL + "/exclude-for-account"
-        self._EXCLUDE_FOR_AD_GROUP = self._URL + "/exclude-for-ad-group"
-
-    def search_stream(
-        self,
-        query: str,
-        queried_account_id: str,
-        secret_id: str,
-    ) -> List[Union[List, Dict]]:
-        """
-        :param query Sql query for google ads. Best way to build it is https://developers.google.com/google-ads/api/fields/v14/accessible_bidding_strategy_query_builder
-        :param queried_account_id Google ads id of queried account
-        :param secret_id The ID of the secret in secret manager
-        :return: List(List)
-        """
-        body = {
-            "query": query,
-            "queried_account_id": queried_account_id,
-            "secret_id": secret_id,
-        }
-
-        header = get_headers(self._SEARCH_STREAM)
-        response = request("post", url=self._SEARCH_STREAM, json=body, headers=header)
-
-        if response.status_code == HTTPStatus.OK:
-            service_response = response.json()
-            return service_response["data"]
-        else:
-            raise GoogleAdsServiceException(response.content)
-
-    def search(
-        self,
-        query: str,
-        queried_account_id: str,
-        secret_id: str,
-        page_size: int,
-    ) -> List[Dict]:
-        """
-        :param query Sql query for google ads. Best way to build it is https://developers.google.com/google-ads/api/fields/v14/accessible_bidding_strategy_query_builder
-        :param queried_account_id Google ads id of queried account
-        :param secret_id The ID of the secret in secret manager
-        :param page_size Size of page for results
-        :return {"next_page_token": token, results: list of dict where key for each dict is "metrics" and then metric type from query}
-        """
-        body = {
-            "query": query,
-            "queried_account_id": queried_account_id,
-            "secret_id": secret_id,
-            "page_token": None,
-            "page_size": page_size,
-        }
-
-        header = get_headers(self._SEARCH)
-        response = request("post", url=self._SEARCH, json=body, headers=header)
-
-        if response.status_code != HTTPStatus.OK:
-            raise GoogleAdsServiceException(response.content)
-
-        service_response = response.json()
-        yield service_response["data"]["results"]
-
-        # if there was a last page response is empty string
-        while service_response["data"]["next_page_token"]:
-            body["page_token"] = service_response["data"]["next_page_token"]
-            response = request("post", url=self._SEARCH, json=body, headers=header)
-
-            if response.status_code != HTTPStatus.OK:
-                raise GoogleAdsServiceException(response.content)
-
-            service_response = response.json()
-            yield service_response["data"]["results"]
-
-    def exclude_criterion_for_account(
-        self, client_id: str, exclusion_raw: List[str], mode: str, secret_id: str = None
-    ) -> None:
-        """
-        Excludes list of unwanted urls/YouTube channels for account with client_id
-        :param client_id: Google Ads id without -
-        :param exclusion_raw: list of negative urls/YouTube channels
-        :param mode: Union(placement, youtube)
-        :param secret_id: id of the secret
-        :return: None
-        """
-        body = {
-            "client_id": client_id,
-            "exclusion_raw": exclusion_raw,
-            "mode": mode,
-            "secret_id": secret_id,
-        }
-
-        header = get_headers(self._EXCLUDE_FOR_ACCOUNT)
-        response = request(
-            "post", url=self._EXCLUDE_FOR_ACCOUNT, json=body, headers=header
-        )
-
-        if response.status_code == HTTPStatus.OK:
-            service_response = response.json()
-            return service_response["data"]
-        else:
-            raise GoogleAdsServiceException(response.content)
-
-    def exclude_criterion_for_ad_group(
-        self,
-        client_id: str,
-        ad_group_id: str,
-        exclusion_raw: List[str],
-        secret_id: str = None,
-    ) -> None:
-        """
-        Excludes list of unwanted urls/YouTube channels for given ad_group with client_id
-        :param client_id: Google Ads id without -
-        :param ad_group_id: given ad group id for which urls should be excluded
-        :param exclusion_raw: list of negative urls/YouTube channels
-        :param secret_id: id of the secret
-        :return:None
-        """
-        body = {
-            "client_id": client_id,
-            "exclusion_raw": exclusion_raw,
-            "ad_group_id": ad_group_id,
-            "secret_id": secret_id,
-        }
-
-        header = get_headers(self._EXCLUDE_FOR_AD_GROUP)
-        response = request(
-            "post", url=self._EXCLUDE_FOR_AD_GROUP, json=body, headers=header
-        )
-
-        if response.status_code == HTTPStatus.OK:
-            return
-        else:
-            raise GoogleAdsServiceException(response.content)
+from requests import request
+from typing import List, Union, Dict
+from logos_sdk.services import get_headers
+from http import HTTPStatus
+from dotenv import load_dotenv
+import os
+
+
+class GoogleAdsServiceException(Exception):
+    pass
+
+
+class GoogleAdsService:
+    def __init__(self, url=None):
+        load_dotenv()
+        self._URL = url or os.environ.get("GOOGLE_ADS_SERVICE_PATH")
+        self._SEARCH_STREAM = self._URL + "/search-stream"
+        self._SEARCH = self._URL + "/search"
+        self._EXCLUDE_FOR_ACCOUNT = self._URL + "/exclude-for-account"
+        self._EXCLUDE_FOR_AD_GROUP = self._URL + "/exclude-for-ad-group"
+
+    def search_stream(
+        self,
+        query: str,
+        queried_account_id: str,
+        secret_id: str,
+    ) -> List[Union[List, Dict]]:
+        """
+        :param query Sql query for google ads. Best way to build it is https://developers.google.com/google-ads/api/fields/v14/accessible_bidding_strategy_query_builder
+        :param queried_account_id Google ads id of queried account
+        :param secret_id The ID of the secret in secret manager
+        :return: List(List)
+        """
+        body = {
+            "query": query,
+            "queried_account_id": queried_account_id,
+            "secret_id": secret_id,
+        }
+
+        header = get_headers(self._SEARCH_STREAM)
+        response = request("post", url=self._SEARCH_STREAM, json=body, headers=header)
+
+        if response.status_code == HTTPStatus.OK:
+            service_response = response.json()
+            return service_response["data"]
+        else:
+            raise GoogleAdsServiceException(response.content)
+
+    def search(
+        self,
+        query: str,
+        queried_account_id: str,
+        secret_id: str,
+        page_size: int,
+    ) -> List[Dict]:
+        """
+        :param query Sql query for google ads. Best way to build it is https://developers.google.com/google-ads/api/fields/v14/accessible_bidding_strategy_query_builder
+        :param queried_account_id Google ads id of queried account
+        :param secret_id The ID of the secret in secret manager
+        :param page_size Size of page for results
+        :return {"next_page_token": token, results: list of dict where key for each dict is "metrics" and then metric type from query}
+        """
+        body = {
+            "query": query,
+            "queried_account_id": queried_account_id,
+            "secret_id": secret_id,
+            "page_token": None,
+            "page_size": page_size,
+        }
+
+        header = get_headers(self._SEARCH)
+        response = request("post", url=self._SEARCH, json=body, headers=header)
+
+        if response.status_code != HTTPStatus.OK:
+            raise GoogleAdsServiceException(response.content)
+
+        service_response = response.json()
+        yield service_response["data"]["results"]
+
+        # if there was a last page response is empty string
+        while service_response["data"]["next_page_token"]:
+            body["page_token"] = service_response["data"]["next_page_token"]
+            response = request("post", url=self._SEARCH, json=body, headers=header)
+
+            if response.status_code != HTTPStatus.OK:
+                raise GoogleAdsServiceException(response.content)
+
+            service_response = response.json()
+            yield service_response["data"]["results"]
+
+    def exclude_criterion_for_account(
+        self, client_id: str, exclusion_raw: List[str], mode: str, secret_id: str = None
+    ) -> None:
+        """
+        Excludes list of unwanted urls/YouTube channels for account with client_id
+        :param client_id: Google Ads id without -
+        :param exclusion_raw: list of negative urls/YouTube channels
+        :param mode: Union(placement, youtube)
+        :param secret_id: id of the secret
+        :return: None
+        """
+        body = {
+            "client_id": client_id,
+            "exclusion_raw": exclusion_raw,
+            "mode": mode,
+            "secret_id": secret_id,
+        }
+
+        header = get_headers(self._EXCLUDE_FOR_ACCOUNT)
+        response = request(
+            "post", url=self._EXCLUDE_FOR_ACCOUNT, json=body, headers=header
+        )
+
+        if response.status_code == HTTPStatus.OK:
+            service_response = response.json()
+            return service_response["data"]
+        else:
+            raise GoogleAdsServiceException(response.content)
+
+    def exclude_criterion_for_ad_group(
+        self,
+        client_id: str,
+        ad_group_id: str,
+        exclusion_raw: List[str],
+        secret_id: str = None,
+    ) -> None:
+        """
+        Excludes list of unwanted urls/YouTube channels for given ad_group with client_id
+        :param client_id: Google Ads id without -
+        :param ad_group_id: given ad group id for which urls should be excluded
+        :param exclusion_raw: list of negative urls/YouTube channels
+        :param secret_id: id of the secret
+        :return:None
+        """
+        body = {
+            "client_id": client_id,
+            "exclusion_raw": exclusion_raw,
+            "ad_group_id": ad_group_id,
+            "secret_id": secret_id,
+        }
+
+        header = get_headers(self._EXCLUDE_FOR_AD_GROUP)
+        response = request(
+            "post", url=self._EXCLUDE_FOR_AD_GROUP, json=body, headers=header
+        )
+
+        if response.status_code == HTTPStatus.OK:
+            return
+        else:
+            raise GoogleAdsServiceException(response.content)
```

### Comparing `logos_sdk-0.0.23/logos_sdk/services/GoogleSheets.py` & `logos_sdk-0.0.24/logos_sdk/services/GoogleSheets.py`

 * *Ordering differences only*

 * *Files 15% similar despite different names*

```diff
@@ -1,293 +1,293 @@
-from requests import request
-from typing import List, Dict, Tuple, Union
-from logos_sdk.services import get_headers
-from http import HTTPStatus
-from dotenv import load_dotenv
-import os
-
-
-class SheetServiceException(Exception):
-    pass
-
-
-class SheetService:
-
-    def __init__(self, sheet_link=None, url=None):
-        load_dotenv()
-        self._URL = url or os.environ.get("GOOGLE_SHEETS_SERVICE_PATH")
-        self.sheet_link = sheet_link
-        self._UPDATE = self._URL + "/update"
-        self._BATCH_UPDATE = self._URL + "/batch-update"
-        self._GET_RECORDS = self._URL + "/get-records"
-        self._GET_VALUES = self._URL + "/get-values"
-        self._CLEAR = self._URL + "/clear"
-        self._DELETE = self._URL + "/delete"
-        self._FORMAT = self._URL + "/format"
-        self._SORT = self._URL + "/sort"
-        self._RESIZE_CLEAR = self._URL + "/resize-clear"
-        self._GET_COL_VALUES = self._URL + "/get-column-values"
-
-    def update(self, update: List[List], worksheet_name: str, a1_notation: str = None,
-               create_if_not_exist: bool = False, clear: bool = False, sheet_link: str = None) -> None:
-        """
-        Function to call SheetService with update route
-        :param update: List of lists of values to be added to worksheet
-        :param worksheet_name: Name of worksheet in spreadsheet
-        :param a1_notation: Range which is updated
-        :param create_if_not_exist: If true new worksheet is created if the worksheet name did not exist in spreadsheet
-        :param sheet_link: Url link for spreadsheet
-        :param clear If true whole worksheet is cleaned before update.
-        Parameters rules and ranges are only applied when new sheet is created. If you want to apply new changes
-        please use set_rules/format.
-        :return: None
-        """
-        body = {
-            "sheet_link": self.sheet_link if sheet_link is None else sheet_link,
-            "update": update,
-            "worksheet_name": worksheet_name,
-            "range": "A1" if a1_notation is None else a1_notation,
-            "create_if_not_exist": create_if_not_exist,
-            "clear": clear
-        }
-
-        header = get_headers(self._UPDATE)
-
-        response = request("post", url=self._UPDATE, json=body, headers=header)
-        service_response = response.json()
-        if response.status_code == HTTPStatus.OK:
-            return
-        
-        raise SheetServiceException(service_response)
-
-    def batch_update(self, batch_updates: List[Dict[str, Union[str, Dict[str, List[List]]]]],
-                     create_if_not_exist: bool = False, sheet_link: str = None) -> None:
-        """
-        Function to call SheetService with batch-update route.
-        :param batch_updates: List(Dict("worksheet_name": str,
-                                        "batch_update": Dict("range": "a1_notation", "values": List(List(Any)))))
-        :param create_if_not_exist: If true, creates every non-existing worksheet in batch updates
-        :param sheet_link: Url link for spreadsheet
-        :return: None
-        """
-        body = {
-            "sheet_link": self.sheet_link if sheet_link is None else sheet_link,
-            "batch_updates": batch_updates,
-            "create_if_not_exist": create_if_not_exist
-        }
-
-        header = get_headers(self._BATCH_UPDATE)
-
-        response = request("post", url=self._BATCH_UPDATE, json=body, headers=header)
-        service_response = response.json()
-        if response.status_code == HTTPStatus.OK:
-            return
-        
-        raise SheetServiceException(service_response)
-
-    def get_records(self, worksheet_name: str, sheet_link: str = None) -> List[Dict]:
-        """
-        Function to call SheetService with get-records route
-        :param worksheet_name:
-        :param sheet_link: Url link for spreadsheet.
-        :return: Dict(List(Int/Str/Float))
-        """
-        body = {
-            "sheet_link": self.sheet_link if sheet_link is None else sheet_link,
-            "worksheet_name": worksheet_name
-        }
-
-        header = get_headers(self._GET_RECORDS)
-
-        response = request("post", url=self._GET_RECORDS, json=body, headers=header)
-        service_response = response.json()
-        if response.status_code == HTTPStatus.OK:
-            return service_response["data"]
-        
-        raise SheetServiceException(service_response)
-
-    def get_values(self, worksheet_name: str, a1_range: str = None, row_start: int = None, col_start: int = None,
-                   row_end: int = None, col_end: int = None, sheet_link: str = None) -> List[List]:
-        """
-        Function to call SheetService with get-values route. You can specify a1_range which you want to get. Or you can
-        specify which rows/cols should be retrieved. If none of the parameters are fulfilled whole
-        worksheet will be retrieved. A1_range cannot be combined with row/col start/end.
-        :param worksheet_name:
-        :param a1_range: A1 range to get data
-        :param row_start: Row start
-        :param col_start: Colum start
-        :param row_end: Row end
-        :param col_end: Colum end
-        :param sheet_link: Url link for spreadsheet
-        :return: List(List(Int/Str/Float))
-        """
-        body = {
-            "sheet_link": self.sheet_link if sheet_link is None else sheet_link,
-            "worksheet_name": worksheet_name
-        }
-
-        if row_start is not None and col_start is not None and col_end is not None and row_end is not None:
-            body = {**body, **{"row_start": row_start, "col_start": col_start, "row_end": row_end,
-                               "col_end": col_end}}
-        elif a1_range is not None:
-            body["a1_range"] = a1_range
-
-        header = get_headers(self._GET_VALUES)
-
-        response = request("post", url=self._GET_VALUES, json=body, headers=header)
-        service_response = response.json()
-        if response.status_code == HTTPStatus.OK:
-            return service_response["data"]
-        
-        raise SheetServiceException(service_response)
-
-    def clear(self, worksheet_name: str, a1_range: str = None, row_clear_start: int = None,
-              row_clear_end: int = None, sheet_link: str = None) -> None:
-        """
-         Function to call SheetService with clear route. You can specify cells which should be cleaned  with a1_range or
-         starting and ending row. If none of them are filled whole worksheet will be cleaned.
-         A1 range cannot be combined with row start/end
-        :param worksheet_name: Name of the cleared worksheet
-        :param a1_range: Range which should be cleared
-        :param row_clear_start: Starting clearing row
-        :param row_clear_end: Ending clearing row
-        :param sheet_link: Url link for spreadsheet
-        :return: None
-        """
-        body = {
-            "sheet_link": self.sheet_link if sheet_link is None else sheet_link,
-            "worksheet_name": worksheet_name
-        }
-
-        if row_clear_start is not None and row_clear_end is not None:
-            body = {**body, **{"row_clear_start": row_clear_start,
-                               "row_clear_end": row_clear_end}}
-        elif a1_range is not None:
-            body["a1_range"] = a1_range
-
-        header = get_headers(self._CLEAR)
-
-        response = request("post", url=self._CLEAR, json=body, headers=header)
-        service_response = response.json()
-        if response.status_code == HTTPStatus.OK:
-            return service_response["data"]
-        
-        raise SheetServiceException(service_response)
-
-    def delete(self, worksheet_name: str, sheet_link: str = None) -> None:
-        """
-        Function to call SheetService with delete route
-        :param worksheet_name: Name of the worksheet to be deleted
-        :param sheet_link: Url link for spreadsheet
-        :return: None
-        """
-        body = {
-            "sheet_link": self.sheet_link if sheet_link is None else sheet_link,
-            "worksheet_name": worksheet_name
-        }
-
-        header = get_headers(self._DELETE)
-
-        response = request("post", url=self._DELETE, json=body, headers=header)
-        service_response = response.json()
-        if response.status_code == HTTPStatus.OK:
-            return
-        
-        raise SheetServiceException(service_response)
-
-    def format(self, worksheet_name: str, cells_format: List[Dict], sheet_link: str = None, freeze: int = None) -> None:
-        """
-        Set formats for given worksheet
-        :param worksheet_name: Name of the worksheet
-        :param sheet_link: Url link for spreadsheet
-        :param cells_format: An iterable whose elements are dict {color: hex, bold: bool}
-        notation, e.g. 'A1:A5', and a ``CellFormat`` object)
-        :param freeze num of rows to be frozen
-        :return:
-        """
-        body = {
-            "sheet_link": self.sheet_link if sheet_link is None else sheet_link,
-            "worksheet_name": worksheet_name,
-            "cells_format": cells_format,
-            "freeze": freeze
-        }
-
-        header = get_headers(self._FORMAT)
-
-        response = request("post", url=self._FORMAT, json=body, headers=header)
-        service_response = response.json()
-        if response.status_code == HTTPStatus.OK:
-            return
-        
-        raise SheetServiceException(service_response)
-
-    def sort(self, worksheet_name: str, sort: Tuple[int, str], sheet_link: str = None, a1_range: str = None) -> None:
-        """
-        Sort given worksheet according to sort parameter. asc/des according to column number
-        :param worksheet_name: Name of given worksheet
-        :param sort: tuple (Union(asc, des), col_number)
-        :param sheet_link: Url link for spreadsheet
-        :param a1_range: Range which should be sorted
-        :return: None
-        """
-        body = {
-            "sheet_link": self.sheet_link if sheet_link is None else sheet_link,
-            "worksheet_name": worksheet_name,
-            "sort": sort,
-            "range": a1_range
-        }
-
-        header = get_headers(self._SORT)
-
-        response = request("post", url=self._SORT, json=body, headers=header)
-        service_response = response.json()
-        if response.status_code == HTTPStatus.OK:
-            return
-        
-        raise SheetServiceException(service_response)
-
-    def resize_clear(self, worksheet_name: str, row_num: int, sheet_link: str = None) -> None:
-        """
-        This endpoint takes worksheet, resizes it to minimum (1, or num_of_frozen_rows + 1) which deletes data with
-        formatting and then resizes it back to row_num.
-        :param worksheet_name: Name of given worksheet
-        :param row_num: new number of rows.
-        :param sheet_link: Url link for spreadsheet
-        :return:
-        """
-        body = {
-            "sheet_link": self.sheet_link if sheet_link is None else sheet_link,
-            "worksheet_name": worksheet_name,
-            "row_num": row_num
-        }
-
-        header = get_headers(self._RESIZE_CLEAR)
-
-        response = request("post", url=self._RESIZE_CLEAR, json=body, headers=header)
-        service_response = response.json()
-        if response.status_code == HTTPStatus.OK:
-            return
-        
-        raise SheetServiceException(service_response)
-
-    def get_column_values(self, worksheet_name: str, col_num: int, sheet_link: str = None) -> List:
-        """
-        Returns a list of all values in column `col_num`
-        :param worksheet_name: Name of given worksheet
-        :param col_num: Number of column for which you want the date
-        :param sheet_link: Url link for spreadsheet
-        :return:
-        """
-        body = {
-            "sheet_link": self.sheet_link if sheet_link is None else sheet_link,
-            "worksheet_name": worksheet_name,
-            "column": col_num
-        }
-
-        header = get_headers(self._GET_COL_VALUES)
-
-        response = request("post", url=self._GET_COL_VALUES, json=body, headers=header)
-        service_response = response.json()
-        if response.status_code == HTTPStatus.OK:
-            return service_response["data"]
-        
-        raise SheetServiceException(service_response)
+from requests import request
+from typing import List, Dict, Tuple, Union
+from logos_sdk.services import get_headers
+from http import HTTPStatus
+from dotenv import load_dotenv
+import os
+
+
+class SheetServiceException(Exception):
+    pass
+
+
+class SheetService:
+
+    def __init__(self, sheet_link=None, url=None):
+        load_dotenv()
+        self._URL = url or os.environ.get("GOOGLE_SHEETS_SERVICE_PATH")
+        self.sheet_link = sheet_link
+        self._UPDATE = self._URL + "/update"
+        self._BATCH_UPDATE = self._URL + "/batch-update"
+        self._GET_RECORDS = self._URL + "/get-records"
+        self._GET_VALUES = self._URL + "/get-values"
+        self._CLEAR = self._URL + "/clear"
+        self._DELETE = self._URL + "/delete"
+        self._FORMAT = self._URL + "/format"
+        self._SORT = self._URL + "/sort"
+        self._RESIZE_CLEAR = self._URL + "/resize-clear"
+        self._GET_COL_VALUES = self._URL + "/get-column-values"
+
+    def update(self, update: List[List], worksheet_name: str, a1_notation: str = None,
+               create_if_not_exist: bool = False, clear: bool = False, sheet_link: str = None) -> None:
+        """
+        Function to call SheetService with update route
+        :param update: List of lists of values to be added to worksheet
+        :param worksheet_name: Name of worksheet in spreadsheet
+        :param a1_notation: Range which is updated
+        :param create_if_not_exist: If true new worksheet is created if the worksheet name did not exist in spreadsheet
+        :param sheet_link: Url link for spreadsheet
+        :param clear If true whole worksheet is cleaned before update.
+        Parameters rules and ranges are only applied when new sheet is created. If you want to apply new changes
+        please use set_rules/format.
+        :return: None
+        """
+        body = {
+            "sheet_link": self.sheet_link if sheet_link is None else sheet_link,
+            "update": update,
+            "worksheet_name": worksheet_name,
+            "range": "A1" if a1_notation is None else a1_notation,
+            "create_if_not_exist": create_if_not_exist,
+            "clear": clear
+        }
+
+        header = get_headers(self._UPDATE)
+
+        response = request("post", url=self._UPDATE, json=body, headers=header)
+        service_response = response.json()
+        if response.status_code == HTTPStatus.OK:
+            return
+        
+        raise SheetServiceException(service_response)
+
+    def batch_update(self, batch_updates: List[Dict[str, Union[str, Dict[str, List[List]]]]],
+                     create_if_not_exist: bool = False, sheet_link: str = None) -> None:
+        """
+        Function to call SheetService with batch-update route.
+        :param batch_updates: List(Dict("worksheet_name": str,
+                                        "batch_update": Dict("range": "a1_notation", "values": List(List(Any)))))
+        :param create_if_not_exist: If true, creates every non-existing worksheet in batch updates
+        :param sheet_link: Url link for spreadsheet
+        :return: None
+        """
+        body = {
+            "sheet_link": self.sheet_link if sheet_link is None else sheet_link,
+            "batch_updates": batch_updates,
+            "create_if_not_exist": create_if_not_exist
+        }
+
+        header = get_headers(self._BATCH_UPDATE)
+
+        response = request("post", url=self._BATCH_UPDATE, json=body, headers=header)
+        service_response = response.json()
+        if response.status_code == HTTPStatus.OK:
+            return
+        
+        raise SheetServiceException(service_response)
+
+    def get_records(self, worksheet_name: str, sheet_link: str = None) -> List[Dict]:
+        """
+        Function to call SheetService with get-records route
+        :param worksheet_name:
+        :param sheet_link: Url link for spreadsheet.
+        :return: Dict(List(Int/Str/Float))
+        """
+        body = {
+            "sheet_link": self.sheet_link if sheet_link is None else sheet_link,
+            "worksheet_name": worksheet_name
+        }
+
+        header = get_headers(self._GET_RECORDS)
+
+        response = request("post", url=self._GET_RECORDS, json=body, headers=header)
+        service_response = response.json()
+        if response.status_code == HTTPStatus.OK:
+            return service_response["data"]
+        
+        raise SheetServiceException(service_response)
+
+    def get_values(self, worksheet_name: str, a1_range: str = None, row_start: int = None, col_start: int = None,
+                   row_end: int = None, col_end: int = None, sheet_link: str = None) -> List[List]:
+        """
+        Function to call SheetService with get-values route. You can specify a1_range which you want to get. Or you can
+        specify which rows/cols should be retrieved. If none of the parameters are fulfilled whole
+        worksheet will be retrieved. A1_range cannot be combined with row/col start/end.
+        :param worksheet_name:
+        :param a1_range: A1 range to get data
+        :param row_start: Row start
+        :param col_start: Colum start
+        :param row_end: Row end
+        :param col_end: Colum end
+        :param sheet_link: Url link for spreadsheet
+        :return: List(List(Int/Str/Float))
+        """
+        body = {
+            "sheet_link": self.sheet_link if sheet_link is None else sheet_link,
+            "worksheet_name": worksheet_name
+        }
+
+        if row_start is not None and col_start is not None and col_end is not None and row_end is not None:
+            body = {**body, **{"row_start": row_start, "col_start": col_start, "row_end": row_end,
+                               "col_end": col_end}}
+        elif a1_range is not None:
+            body["a1_range"] = a1_range
+
+        header = get_headers(self._GET_VALUES)
+
+        response = request("post", url=self._GET_VALUES, json=body, headers=header)
+        service_response = response.json()
+        if response.status_code == HTTPStatus.OK:
+            return service_response["data"]
+        
+        raise SheetServiceException(service_response)
+
+    def clear(self, worksheet_name: str, a1_range: str = None, row_clear_start: int = None,
+              row_clear_end: int = None, sheet_link: str = None) -> None:
+        """
+         Function to call SheetService with clear route. You can specify cells which should be cleaned  with a1_range or
+         starting and ending row. If none of them are filled whole worksheet will be cleaned.
+         A1 range cannot be combined with row start/end
+        :param worksheet_name: Name of the cleared worksheet
+        :param a1_range: Range which should be cleared
+        :param row_clear_start: Starting clearing row
+        :param row_clear_end: Ending clearing row
+        :param sheet_link: Url link for spreadsheet
+        :return: None
+        """
+        body = {
+            "sheet_link": self.sheet_link if sheet_link is None else sheet_link,
+            "worksheet_name": worksheet_name
+        }
+
+        if row_clear_start is not None and row_clear_end is not None:
+            body = {**body, **{"row_clear_start": row_clear_start,
+                               "row_clear_end": row_clear_end}}
+        elif a1_range is not None:
+            body["a1_range"] = a1_range
+
+        header = get_headers(self._CLEAR)
+
+        response = request("post", url=self._CLEAR, json=body, headers=header)
+        service_response = response.json()
+        if response.status_code == HTTPStatus.OK:
+            return service_response["data"]
+        
+        raise SheetServiceException(service_response)
+
+    def delete(self, worksheet_name: str, sheet_link: str = None) -> None:
+        """
+        Function to call SheetService with delete route
+        :param worksheet_name: Name of the worksheet to be deleted
+        :param sheet_link: Url link for spreadsheet
+        :return: None
+        """
+        body = {
+            "sheet_link": self.sheet_link if sheet_link is None else sheet_link,
+            "worksheet_name": worksheet_name
+        }
+
+        header = get_headers(self._DELETE)
+
+        response = request("post", url=self._DELETE, json=body, headers=header)
+        service_response = response.json()
+        if response.status_code == HTTPStatus.OK:
+            return
+        
+        raise SheetServiceException(service_response)
+
+    def format(self, worksheet_name: str, cells_format: List[Dict], sheet_link: str = None, freeze: int = None) -> None:
+        """
+        Set formats for given worksheet
+        :param worksheet_name: Name of the worksheet
+        :param sheet_link: Url link for spreadsheet
+        :param cells_format: An iterable whose elements are dict {color: hex, bold: bool}
+        notation, e.g. 'A1:A5', and a ``CellFormat`` object)
+        :param freeze num of rows to be frozen
+        :return:
+        """
+        body = {
+            "sheet_link": self.sheet_link if sheet_link is None else sheet_link,
+            "worksheet_name": worksheet_name,
+            "cells_format": cells_format,
+            "freeze": freeze
+        }
+
+        header = get_headers(self._FORMAT)
+
+        response = request("post", url=self._FORMAT, json=body, headers=header)
+        service_response = response.json()
+        if response.status_code == HTTPStatus.OK:
+            return
+        
+        raise SheetServiceException(service_response)
+
+    def sort(self, worksheet_name: str, sort: Tuple[int, str], sheet_link: str = None, a1_range: str = None) -> None:
+        """
+        Sort given worksheet according to sort parameter. asc/des according to column number
+        :param worksheet_name: Name of given worksheet
+        :param sort: tuple (Union(asc, des), col_number)
+        :param sheet_link: Url link for spreadsheet
+        :param a1_range: Range which should be sorted
+        :return: None
+        """
+        body = {
+            "sheet_link": self.sheet_link if sheet_link is None else sheet_link,
+            "worksheet_name": worksheet_name,
+            "sort": sort,
+            "range": a1_range
+        }
+
+        header = get_headers(self._SORT)
+
+        response = request("post", url=self._SORT, json=body, headers=header)
+        service_response = response.json()
+        if response.status_code == HTTPStatus.OK:
+            return
+        
+        raise SheetServiceException(service_response)
+
+    def resize_clear(self, worksheet_name: str, row_num: int, sheet_link: str = None) -> None:
+        """
+        This endpoint takes worksheet, resizes it to minimum (1, or num_of_frozen_rows + 1) which deletes data with
+        formatting and then resizes it back to row_num.
+        :param worksheet_name: Name of given worksheet
+        :param row_num: new number of rows.
+        :param sheet_link: Url link for spreadsheet
+        :return:
+        """
+        body = {
+            "sheet_link": self.sheet_link if sheet_link is None else sheet_link,
+            "worksheet_name": worksheet_name,
+            "row_num": row_num
+        }
+
+        header = get_headers(self._RESIZE_CLEAR)
+
+        response = request("post", url=self._RESIZE_CLEAR, json=body, headers=header)
+        service_response = response.json()
+        if response.status_code == HTTPStatus.OK:
+            return
+        
+        raise SheetServiceException(service_response)
+
+    def get_column_values(self, worksheet_name: str, col_num: int, sheet_link: str = None) -> List:
+        """
+        Returns a list of all values in column `col_num`
+        :param worksheet_name: Name of given worksheet
+        :param col_num: Number of column for which you want the date
+        :param sheet_link: Url link for spreadsheet
+        :return:
+        """
+        body = {
+            "sheet_link": self.sheet_link if sheet_link is None else sheet_link,
+            "worksheet_name": worksheet_name,
+            "column": col_num
+        }
+
+        header = get_headers(self._GET_COL_VALUES)
+
+        response = request("post", url=self._GET_COL_VALUES, json=body, headers=header)
+        service_response = response.json()
+        if response.status_code == HTTPStatus.OK:
+            return service_response["data"]
+        
+        raise SheetServiceException(service_response)
```

### Comparing `logos_sdk-0.0.23/logos_sdk/services/MarketMiner.py` & `logos_sdk-0.0.24/logos_sdk/services/MarketMiner.py`

 * *Files identical despite different names*

### Comparing `logos_sdk-0.0.23/logos_sdk/services/MerchantCenter.py` & `logos_sdk-0.0.24/logos_sdk/services/MerchantCenter.py`

 * *Files identical despite different names*

### Comparing `logos_sdk-0.0.23/logos_sdk/services/MicrosoftAdvertising.py` & `logos_sdk-0.0.24/logos_sdk/services/MicrosoftAdvertising.py`

 * *Ordering differences only*

 * *Files 22% similar despite different names*

```diff
@@ -1,178 +1,178 @@
-from http import HTTPStatus
-from requests import request
-from logos_sdk.services import get_headers
-from typing import List
-from dotenv import load_dotenv
-import os
-
-
-class MicrosoftAdvertisingException(Exception):
-    pass
-
-
-# https://learn.microsoft.com/en-us/advertising/reporting-service/adgroupstatusreportfilter?view=bingads-13
-class EntityStatus:
-    ACTIVE = "Active"
-    DELETED = "Deleted"
-    EXPIRED = "Expired"
-    PAUSED = "Paused"
-
-
-class MicrosoftAdvertising:
-    def __init__(self, url=None):
-        load_dotenv()
-        self._URL = url or os.environ.get("MICROSOFT_ADVERTISING_PATH")
-        self._GET_ACCESSIBLE_ACCOUNTS = self._URL + "/accessible-accounts"
-        self._GET_DESTINATION_URL_REPORT = self._URL + "/destination-url-report"
-        self._GET_CAMPAIGN_PERFORMANCE_REPORT = self._URL + "/campaign-performance-report"
-        self._GET_BUDGET_SUMMARY_REPORT = self._URL + "/budget-summary-report"
-
-    def get_destination_url_report(
-        self,
-        account_id: str,
-        secret_id: str,
-        date_from: str,
-        date_to: str,
-        report_columns: List[str],
-        entity_statuses: dict = None,
-    ) -> List:
-        """
-        Calls endpoint for getting destination URL stats
-        https://learn.microsoft.com/en-us/advertising/reporting-service/destinationurlperformancereportrequest?view=bingads-13
-        :param account_id: The ID of the account in Microsoft Advertising
-        :param secret_id: The ID of the secret in secret manager
-        :param date_from: The date we want the report to start from. Must be before date to
-        :param date_to: The date we want the report to end at
-        :param report_columns: stats we want included in the report
-        :param entity_statuses: dict containing status ad_status, ad_group_status, campaign_status and account_status
-        :return: List of urls and their stats
-        """
-        if entity_statuses is None:
-            entity_statuses = {
-                "ad_status": EntityStatus.ACTIVE,
-                "ad_group_status": EntityStatus.ACTIVE,
-                "campaign_status": EntityStatus.ACTIVE,
-                "account_status": EntityStatus.ACTIVE,
-            }
-
-        body = {
-            "account_id": account_id,
-            "secret_id": secret_id,
-            "date_from": date_from,
-            "date_to": date_to,
-            "report_columns": report_columns,
-        } | entity_statuses
-
-        header = get_headers(self._GET_DESTINATION_URL_REPORT)
-        response = request(
-            "post", url=self._GET_DESTINATION_URL_REPORT, json=body, headers=header
-        )
-
-        if response.status_code == HTTPStatus.OK:
-            service_response = response.json()
-            return service_response["data"]
-        else:
-            raise MicrosoftAdvertisingException(response.content)
-
-    def get_campaign_performance_report(
-        self,
-        account_id: str,
-        secret_id: str,
-        date_from: str,
-        date_to: str,
-        report_columns: List[str],
-        entity_statuses: dict = None,
-    ) -> List:
-        """
-        Calls endpoint for getting campaign performance stats
-        https://learn.microsoft.com/en-us/advertising/reporting-service/campaignperformancereportrequest?view=bingads-13
-        :param account_id: The ID of the account in Microsoft Advertising
-        :param secret_id: The ID of the secret in secret manager
-        :param date_from: The date we want the report to start from. Must be before date to
-        :param date_to: The date we want the report to end at
-        :param report_columns: stats we want included in the report
-        :param entity_statuses: dict containing status of status and account_status
-        :return: List of campaigns and their stats
-        """
-        if entity_statuses is None:
-            entity_statuses = {
-                "status": EntityStatus.ACTIVE,
-                "account_status": EntityStatus.ACTIVE,
-            }
-
-        body = {
-            "account_id": account_id,
-            "secret_id": secret_id,
-            "date_from": date_from,
-            "date_to": date_to,
-            "report_columns": report_columns,
-        } | entity_statuses
-
-        header = get_headers(self._GET_CAMPAIGN_PERFORMANCE_REPORT)
-        response = request(
-            "post", url=self._GET_CAMPAIGN_PERFORMANCE_REPORT, json=body, headers=header
-        )
-
-        if response.status_code == HTTPStatus.OK:
-            service_response = response.json()
-            return service_response["data"]
-        else:
-            raise MicrosoftAdvertisingException(response.content)
-
-    def get_budget_summary_report(
-        self,
-        account_id: str,
-        secret_id: str,
-        date_from: str,
-        date_to: str,
-        report_columns: List[str]
-    ):
-        """
-        Calls endpoint for getting budget summary
-        https://learn.microsoft.com/en-us/advertising/reporting-service/budgetsummaryreportcolumn?view=bingads-13
-        :param account_id: The ID of the account in Microsoft Advertising
-        :param secret_id: The ID of the secret in secret manager
-        :param date_from: The date we want the report to start from. Must be before date to
-        :param date_to: The date we want the report to end at
-        :param report_columns: stats we want included in the report
-        :return: List of campaigns and their stats
-        """
-
-        body = {
-            "account_id": account_id,
-            "secret_id": secret_id,
-            "date_from": date_from,
-            "date_to": date_to,
-            "report_columns": report_columns,
-        }
-
-        header = get_headers(self._GET_BUDGET_SUMMARY_REPORT)
-        response = request(
-            "post", url=self._GET_BUDGET_SUMMARY_REPORT, json=body, headers=header
-        )
-
-        if response.status_code == HTTPStatus.OK:
-            service_response = response.json()
-            return service_response["data"]
-        else:
-            raise MicrosoftAdvertisingException(response.content)
-
-    def get_accessible_accounts(self, secret_id: str) -> List[dict]:
-        """
-        Gets
-        :param secret_id: The ID of the secret in secret manager
-        :return: List of dicts with account_id and name keys
-        """
-        body = {
-            "secret_id": secret_id,
-        }
-        header = get_headers(self._GET_ACCESSIBLE_ACCOUNTS)
-        response = request(
-            "post", url=self._GET_ACCESSIBLE_ACCOUNTS, json=body, headers=header
-        )
-
-        if response.status_code == HTTPStatus.OK:
-            service_response = response.json()
-            return service_response["data"]
-        else:
-            raise MicrosoftAdvertisingException(response.content)
+from http import HTTPStatus
+from requests import request
+from logos_sdk.services import get_headers
+from typing import List
+from dotenv import load_dotenv
+import os
+
+
+class MicrosoftAdvertisingException(Exception):
+    pass
+
+
+# https://learn.microsoft.com/en-us/advertising/reporting-service/adgroupstatusreportfilter?view=bingads-13
+class EntityStatus:
+    ACTIVE = "Active"
+    DELETED = "Deleted"
+    EXPIRED = "Expired"
+    PAUSED = "Paused"
+
+
+class MicrosoftAdvertising:
+    def __init__(self, url=None):
+        load_dotenv()
+        self._URL = url or os.environ.get("MICROSOFT_ADVERTISING_PATH")
+        self._GET_ACCESSIBLE_ACCOUNTS = self._URL + "/accessible-accounts"
+        self._GET_DESTINATION_URL_REPORT = self._URL + "/destination-url-report"
+        self._GET_CAMPAIGN_PERFORMANCE_REPORT = self._URL + "/campaign-performance-report"
+        self._GET_BUDGET_SUMMARY_REPORT = self._URL + "/budget-summary-report"
+
+    def get_destination_url_report(
+        self,
+        account_id: str,
+        secret_id: str,
+        date_from: str,
+        date_to: str,
+        report_columns: List[str],
+        entity_statuses: dict = None,
+    ) -> List:
+        """
+        Calls endpoint for getting destination URL stats
+        https://learn.microsoft.com/en-us/advertising/reporting-service/destinationurlperformancereportrequest?view=bingads-13
+        :param account_id: The ID of the account in Microsoft Advertising
+        :param secret_id: The ID of the secret in secret manager
+        :param date_from: The date we want the report to start from. Must be before date to
+        :param date_to: The date we want the report to end at
+        :param report_columns: stats we want included in the report
+        :param entity_statuses: dict containing status ad_status, ad_group_status, campaign_status and account_status
+        :return: List of urls and their stats
+        """
+        if entity_statuses is None:
+            entity_statuses = {
+                "ad_status": EntityStatus.ACTIVE,
+                "ad_group_status": EntityStatus.ACTIVE,
+                "campaign_status": EntityStatus.ACTIVE,
+                "account_status": EntityStatus.ACTIVE,
+            }
+
+        body = {
+            "account_id": account_id,
+            "secret_id": secret_id,
+            "date_from": date_from,
+            "date_to": date_to,
+            "report_columns": report_columns,
+        } | entity_statuses
+
+        header = get_headers(self._GET_DESTINATION_URL_REPORT)
+        response = request(
+            "post", url=self._GET_DESTINATION_URL_REPORT, json=body, headers=header
+        )
+
+        if response.status_code == HTTPStatus.OK:
+            service_response = response.json()
+            return service_response["data"]
+        else:
+            raise MicrosoftAdvertisingException(response.content)
+
+    def get_campaign_performance_report(
+        self,
+        account_id: str,
+        secret_id: str,
+        date_from: str,
+        date_to: str,
+        report_columns: List[str],
+        entity_statuses: dict = None,
+    ) -> List:
+        """
+        Calls endpoint for getting campaign performance stats
+        https://learn.microsoft.com/en-us/advertising/reporting-service/campaignperformancereportrequest?view=bingads-13
+        :param account_id: The ID of the account in Microsoft Advertising
+        :param secret_id: The ID of the secret in secret manager
+        :param date_from: The date we want the report to start from. Must be before date to
+        :param date_to: The date we want the report to end at
+        :param report_columns: stats we want included in the report
+        :param entity_statuses: dict containing status of status and account_status
+        :return: List of campaigns and their stats
+        """
+        if entity_statuses is None:
+            entity_statuses = {
+                "status": EntityStatus.ACTIVE,
+                "account_status": EntityStatus.ACTIVE,
+            }
+
+        body = {
+            "account_id": account_id,
+            "secret_id": secret_id,
+            "date_from": date_from,
+            "date_to": date_to,
+            "report_columns": report_columns,
+        } | entity_statuses
+
+        header = get_headers(self._GET_CAMPAIGN_PERFORMANCE_REPORT)
+        response = request(
+            "post", url=self._GET_CAMPAIGN_PERFORMANCE_REPORT, json=body, headers=header
+        )
+
+        if response.status_code == HTTPStatus.OK:
+            service_response = response.json()
+            return service_response["data"]
+        else:
+            raise MicrosoftAdvertisingException(response.content)
+
+    def get_budget_summary_report(
+        self,
+        account_id: str,
+        secret_id: str,
+        date_from: str,
+        date_to: str,
+        report_columns: List[str]
+    ):
+        """
+        Calls endpoint for getting budget summary
+        https://learn.microsoft.com/en-us/advertising/reporting-service/budgetsummaryreportcolumn?view=bingads-13
+        :param account_id: The ID of the account in Microsoft Advertising
+        :param secret_id: The ID of the secret in secret manager
+        :param date_from: The date we want the report to start from. Must be before date to
+        :param date_to: The date we want the report to end at
+        :param report_columns: stats we want included in the report
+        :return: List of campaigns and their stats
+        """
+
+        body = {
+            "account_id": account_id,
+            "secret_id": secret_id,
+            "date_from": date_from,
+            "date_to": date_to,
+            "report_columns": report_columns,
+        }
+
+        header = get_headers(self._GET_BUDGET_SUMMARY_REPORT)
+        response = request(
+            "post", url=self._GET_BUDGET_SUMMARY_REPORT, json=body, headers=header
+        )
+
+        if response.status_code == HTTPStatus.OK:
+            service_response = response.json()
+            return service_response["data"]
+        else:
+            raise MicrosoftAdvertisingException(response.content)
+
+    def get_accessible_accounts(self, secret_id: str) -> List[dict]:
+        """
+        Gets
+        :param secret_id: The ID of the secret in secret manager
+        :return: List of dicts with account_id and name keys
+        """
+        body = {
+            "secret_id": secret_id,
+        }
+        header = get_headers(self._GET_ACCESSIBLE_ACCOUNTS)
+        response = request(
+            "post", url=self._GET_ACCESSIBLE_ACCOUNTS, json=body, headers=header
+        )
+
+        if response.status_code == HTTPStatus.OK:
+            service_response = response.json()
+            return service_response["data"]
+        else:
+            raise MicrosoftAdvertisingException(response.content)
```

### Comparing `logos_sdk-0.0.23/logos_sdk/services/Sklik.py` & `logos_sdk-0.0.24/logos_sdk/services/Sklik.py`

 * *Files identical despite different names*

### Comparing `logos_sdk-0.0.23/logos_sdk/services/__init__.py` & `logos_sdk-0.0.24/logos_sdk/services/__init__.py`

 * *Files identical despite different names*

### Comparing `logos_sdk-0.0.23/logos_sdk.egg-info/SOURCES.txt` & `logos_sdk-0.0.24/logos_sdk.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `logos_sdk-0.0.23/setup.py` & `logos_sdk-0.0.24/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 
 # I AM MASTER!
 with open("README.md", "r") as fh:
     long_description = fh.read()
 
 setuptools.setup(
     name="logos-sdk",
-    version="0.0.23",
+    version="0.0.24",
     author="Databy.io",
     author_email="admin@proficio.cz",
     description="SDK for Logos platform",
     include_package_data=True,
     long_description=long_description,
     long_description_content_type="text/markdown",
     url="https://bitbucket.org/databy/logos-sdk-pip/src/master/",
```

