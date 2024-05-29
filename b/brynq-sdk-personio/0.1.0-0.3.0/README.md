# Comparing `tmp/brynq_sdk_personio-0.1.0.tar.gz` & `tmp/brynq_sdk_personio-0.3.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/brynq_sdk_personio-0.1.0.tar", last modified: Thu Apr 18 15:18:53 2024, max compression
+gzip compressed data, was "dist/brynq_sdk_personio-0.3.0.tar", last modified: Wed May 29 12:10:46 2024, max compression
```

## Comparing `brynq_sdk_personio-0.1.0.tar` & `brynq_sdk_personio-0.3.0.tar`

### file list

```diff
@@ -1,16 +1,20 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-18 15:18:53.000000 brynq_sdk_personio-0.1.0/
--rw-r--r--   0 root         (0) root         (0)      246 2024-04-18 15:18:53.000000 brynq_sdk_personio-0.1.0/PKG-INFO
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-18 15:18:53.000000 brynq_sdk_personio-0.1.0/brynq_sdk/
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-18 15:18:53.000000 brynq_sdk_personio-0.1.0/brynq_sdk/personio/
--rw-rw-rw-   0 root         (0) root         (0)     1617 2024-04-18 15:18:38.000000 brynq_sdk_personio-0.1.0/brynq_sdk/personio/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)        0 2024-04-18 15:18:38.000000 brynq_sdk_personio-0.1.0/brynq_sdk/personio/attendances.py
--rw-rw-rw-   0 root         (0) root         (0)     1218 2024-04-18 15:18:38.000000 brynq_sdk_personio-0.1.0/brynq_sdk/personio/employees.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-18 15:18:53.000000 brynq_sdk_personio-0.1.0/brynq_sdk_personio.egg-info/
--rw-r--r--   0 root         (0) root         (0)      246 2024-04-18 15:18:53.000000 brynq_sdk_personio-0.1.0/brynq_sdk_personio.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)      355 2024-04-18 15:18:53.000000 brynq_sdk_personio-0.1.0/brynq_sdk_personio.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2024-04-18 15:18:53.000000 brynq_sdk_personio-0.1.0/brynq_sdk_personio.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)        1 2024-04-18 15:18:53.000000 brynq_sdk_personio-0.1.0/brynq_sdk_personio.egg-info/not-zip-safe
--rw-r--r--   0 root         (0) root         (0)       40 2024-04-18 15:18:53.000000 brynq_sdk_personio-0.1.0/brynq_sdk_personio.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)       10 2024-04-18 15:18:53.000000 brynq_sdk_personio-0.1.0/brynq_sdk_personio.egg-info/top_level.txt
--rw-r--r--   0 root         (0) root         (0)       38 2024-04-18 15:18:53.000000 brynq_sdk_personio-0.1.0/setup.cfg
--rw-rw-rw-   0 root         (0) root         (0)      426 2024-04-18 15:18:38.000000 brynq_sdk_personio-0.1.0/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-29 12:10:46.000000 brynq_sdk_personio-0.3.0/
+-rw-r--r--   0 root         (0) root         (0)      246 2024-05-29 12:10:46.000000 brynq_sdk_personio-0.3.0/PKG-INFO
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-29 12:10:46.000000 brynq_sdk_personio-0.3.0/brynq_sdk/
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-29 12:10:46.000000 brynq_sdk_personio-0.3.0/brynq_sdk/personio/
+-rw-rw-rw-   0 root         (0) root         (0)     2989 2024-05-29 12:10:29.000000 brynq_sdk_personio-0.3.0/brynq_sdk/personio/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)        0 2024-05-29 12:10:29.000000 brynq_sdk_personio-0.3.0/brynq_sdk/personio/absences.py
+-rw-rw-rw-   0 root         (0) root         (0)        0 2024-05-29 12:10:29.000000 brynq_sdk_personio-0.3.0/brynq_sdk/personio/attendances.py
+-rw-rw-rw-   0 root         (0) root         (0)     2992 2024-05-29 12:10:29.000000 brynq_sdk_personio-0.3.0/brynq_sdk/personio/compensations.py
+-rw-rw-rw-   0 root         (0) root         (0)     4624 2024-05-29 12:10:29.000000 brynq_sdk_personio-0.3.0/brynq_sdk/personio/custom_reports.py
+-rw-rw-rw-   0 root         (0) root         (0)     2377 2024-05-29 12:10:29.000000 brynq_sdk_personio-0.3.0/brynq_sdk/personio/documents.py
+-rw-rw-rw-   0 root         (0) root         (0)     7687 2024-05-29 12:10:29.000000 brynq_sdk_personio-0.3.0/brynq_sdk/personio/employees.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-29 12:10:46.000000 brynq_sdk_personio-0.3.0/brynq_sdk_personio.egg-info/
+-rw-r--r--   0 root         (0) root         (0)      246 2024-05-29 12:10:46.000000 brynq_sdk_personio-0.3.0/brynq_sdk_personio.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)      491 2024-05-29 12:10:46.000000 brynq_sdk_personio-0.3.0/brynq_sdk_personio.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2024-05-29 12:10:46.000000 brynq_sdk_personio-0.3.0/brynq_sdk_personio.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2024-05-29 12:10:46.000000 brynq_sdk_personio-0.3.0/brynq_sdk_personio.egg-info/not-zip-safe
+-rw-r--r--   0 root         (0) root         (0)       40 2024-05-29 12:10:46.000000 brynq_sdk_personio-0.3.0/brynq_sdk_personio.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)       10 2024-05-29 12:10:46.000000 brynq_sdk_personio-0.3.0/brynq_sdk_personio.egg-info/top_level.txt
+-rw-r--r--   0 root         (0) root         (0)       38 2024-05-29 12:10:46.000000 brynq_sdk_personio-0.3.0/setup.cfg
+-rw-rw-rw-   0 root         (0) root         (0)      426 2024-05-29 12:10:29.000000 brynq_sdk_personio-0.3.0/setup.py
```

### Comparing `brynq_sdk_personio-0.1.0/brynq_sdk/personio/__init__.py` & `brynq_sdk_personio-0.3.0/brynq_sdk/personio/__init__.py`

 * *Files 25% similar despite different names*

```diff
@@ -1,40 +1,68 @@
 import requests
 import json
 from typing import List, Union
 from brynq_sdk.brynq import BrynQ
 from brynq_sdk.personio.employees import Employees
+from brynq_sdk.personio.compensations import Compensations
+from brynq_sdk.personio.custom_reports import CustomReports
+from brynq_sdk.personio.documents import Documents
 
 
 # Set the base class for Persinio. This class will be used to set the credentials and those will be used in all other classes.
 class Personio(BrynQ):
     def __init__(self, label: Union[str, List], debug: bool = False):
         """"
         For the documentation of Personio, see: https://developer.personio.de/reference/auth
         """
         super().__init__()
-        base_url = 'https://api.personio.de/v1/'
-        headers = self._set_credentials(label, base_url)
-        self.employees = Employees(headers, base_url)
+        base_url = 'https://api.personio.de/'
+        access_token_v1 = self._get_credentials(label, base_url, version='v1')
+        access_token_v2 = self._get_credentials(label, base_url, version='v2')
+        headers_v1, headers_v2 = self._set_headers(access_token_v1, access_token_v2)
+        self.employees = Employees(headers_v1, f'{base_url}v1/')
+        self.custom_reports = CustomReports(headers_v1, f'{base_url}v1/')
+        self.documents = Documents(headers_v1, f'{base_url}v1/')
+        self.compensations = Compensations(headers_v2, f'{base_url}v2/')
 
-    def _set_credentials(self, label, base_url):
+
+    def _get_credentials(self, label, base_url, version='v2'):
         """
         Sets the credentials for the SuccessFactors API.
         :param label (str): The label for the system credentials.
         :returns: headers (dict): The headers for the API request, including the access token.
         """
         credentials = self.get_system_credential(system='personio', label=label)
-        payload = json.dumps({
+        payload = {
             "client_id": f"{credentials['client_id']}",
-            "client_secret": f"{credentials['client_secret']}"
-        })
-        headers = {
-            'accept': 'application/json',
-            'content-type': 'application/json'
+            "client_secret": f"{credentials['client_secret']}",
+            "grant_type": "client_credentials"
         }
-        response = requests.post(f'{base_url}auth', headers=headers, data=payload)
-        access_token = response.json()['data']['token']
         headers = {
+            "accept": "application/json",
+            "content-type": "application/x-www-form-urlencoded"
+        }
+        url = f'{base_url}{version}/auth/token'
+        if version == 'v1':
+            url = f'{base_url}{version}/auth'
+            headers["content-type"] = "application/json"
+            payload = json.dumps(payload)
+        response = requests.post(url, headers=headers, data=payload)
+        response.raise_for_status()
+        access_token = response.json()['data']['token'] if version == 'v1' else response.json()['access_token']
+
+        return access_token
+
+    def _set_headers(self, access_token_v1, access_token_v2):
+        headers_v1 = {
+            'Authorization': f'Bearer {access_token_v1}',
             'Content-Type': 'application/json',
-            'Authorization': f'Bearer {access_token}'
+            'X-Personio-Partner-ID': 'BRYNQ',
+            'X-Personio-App-ID': 'BRYNQ_COM'
+        }
+        headers_v2 = {
+            'Authorization': f'Bearer {access_token_v2}',
+            'accept': 'application/json',
+            'X-Personio-Partner-ID': 'BRYNQ',
+            'X-Personio-App-ID': 'BRYNQ_COM'
         }
-        return headers
+        return headers_v1, headers_v2
```

