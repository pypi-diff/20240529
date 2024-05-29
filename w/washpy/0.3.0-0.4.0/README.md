# Comparing `tmp/washpy-0.3.0.tar.gz` & `tmp/washpy-0.4.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "washpy-0.3.0.tar", max compression
+gzip compressed data, was "washpy-0.4.0.tar", max compression
```

## Comparing `washpy-0.3.0.tar` & `washpy-0.4.0.tar`

### file list

```diff
@@ -1,14 +1,14 @@
--rw-r--r--   0        0        0    42028 2024-05-14 21:13:05.974878 washpy-0.3.0/LICENSE
--rw-r--r--   0        0        0     3296 2024-05-15 18:58:32.047829 washpy-0.3.0/README.md
--rw-r--r--   0        0        0      612 2024-05-14 23:15:44.787766 washpy-0.3.0/pyproject.toml
--rw-r--r--   0        0        0      596 2024-05-14 21:13:05.974878 washpy-0.3.0/washpy/__init__.py
--rw-r--r--   0        0        0     2185 2024-05-14 21:13:05.978211 washpy-0.3.0/washpy/authenticate.py
--rw-r--r--   0        0        0     9687 2024-05-15 18:36:09.024907 washpy-0.3.0/washpy/device_user.py
--rw-r--r--   0        0        0     1224 2024-05-14 21:13:05.978211 washpy-0.3.0/washpy/pExtended.py
--rw-r--r--   0        0        0     2585 2024-05-14 23:09:17.713438 washpy-0.3.0/washpy/permission.py
--rw-r--r--   0        0        0      827 2024-05-15 11:13:09.808240 washpy-0.3.0/washpy/post_new_password.py
--rw-r--r--   0        0        0      865 2024-05-15 17:42:51.893287 washpy-0.3.0/washpy/role.py
--rw-r--r--   0        0        0     6215 2024-05-14 21:13:05.978211 washpy-0.3.0/washpy/state.py
--rw-r--r--   0        0        0     6133 2024-05-14 23:13:12.557401 washpy-0.3.0/washpy/status.py
--rw-r--r--   0        0        0     1077 2024-05-15 18:51:39.295645 washpy-0.3.0/washpy/user.py
--rw-r--r--   0        0        0     4164 1970-01-01 00:00:00.000000 washpy-0.3.0/PKG-INFO
+-rw-r--r--   0        0        0    42028 2024-05-14 21:13:05.974878 washpy-0.4.0/LICENSE
+-rw-r--r--   0        0        0     3296 2024-05-15 18:58:32.047829 washpy-0.4.0/README.md
+-rw-r--r--   0        0        0      640 2024-05-29 20:25:23.073078 washpy-0.4.0/pyproject.toml
+-rw-r--r--   0        0        0      596 2024-05-14 21:13:05.974878 washpy-0.4.0/washpy/__init__.py
+-rw-r--r--   0        0        0     3800 2024-05-29 20:46:29.588200 washpy-0.4.0/washpy/authenticate.py
+-rw-r--r--   0        0        0    10579 2024-05-29 20:50:39.142420 washpy-0.4.0/washpy/device_user.py
+-rw-r--r--   0        0        0     1224 2024-05-14 21:13:05.978211 washpy-0.4.0/washpy/pExtended.py
+-rw-r--r--   0        0        0     2585 2024-05-14 23:09:17.713438 washpy-0.4.0/washpy/permission.py
+-rw-r--r--   0        0        0      960 2024-05-29 20:47:27.364756 washpy-0.4.0/washpy/post_new_password.py
+-rw-r--r--   0        0        0      865 2024-05-15 17:42:51.893287 washpy-0.4.0/washpy/role.py
+-rw-r--r--   0        0        0     6215 2024-05-14 21:13:05.978211 washpy-0.4.0/washpy/state.py
+-rw-r--r--   0        0        0     6133 2024-05-14 23:13:12.557401 washpy-0.4.0/washpy/status.py
+-rw-r--r--   0        0        0     1077 2024-05-15 18:51:39.295645 washpy-0.4.0/washpy/user.py
+-rw-r--r--   0        0        0     4207 1970-01-01 00:00:00.000000 washpy-0.4.0/PKG-INFO
```

### Comparing `washpy-0.3.0/LICENSE` & `washpy-0.4.0/LICENSE`

 * *Files identical despite different names*

### Comparing `washpy-0.3.0/README.md` & `washpy-0.4.0/README.md`

 * *Files identical despite different names*

### Comparing `washpy-0.3.0/pyproject.toml` & `washpy-0.4.0/pyproject.toml`

 * *Files 16% similar despite different names*

```diff
@@ -1,20 +1,21 @@
 [tool.poetry]
 name = "washpy"
-version = "0.3.0"
+version = "0.4.0"
 description = "A partial implementation of the Miele Professional IP Profile API"
 authors = ["Johann Carl Meyer <info@johannc.de>"]
 license = "LGPL-3.0-only"
 readme = "README.md"
 repository = "https://codeberg.org/johann-cm/washpy"
 documentation = "https://johann-cm.codeberg.page/washpy/washpy.html"
 
 [tool.poetry.dependencies]
 python = "^3.10"
 requests = "2.29.0"
+types-requests = "2.29.0.0"
 isodate = "^0.6.1"
 pydantic = "^2.7.1"
 
 
 [tool.poetry.group.dev.dependencies]
 pytest = "^8.2.0"
 pdoc = "^14.4.0"
```

### Comparing `washpy-0.3.0/washpy/__init__.py` & `washpy-0.4.0/washpy/__init__.py`

 * *Files identical despite different names*

### Comparing `washpy-0.3.0/washpy/device_user.py` & `washpy-0.4.0/washpy/device_user.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,13 +1,15 @@
-from typing import Any, Dict, Final, List, Optional, Union
+from typing import Any, Dict, Final, List
 import requests
-
 import datetime
-
-from washpy.authenticate import authenticate
+from washpy.authenticate import (
+    DeviceUrl,
+    authenticate,
+    parse_and_validate_device_url_to_str,
+)
 from washpy.post_new_password import post_new_password
 from washpy.state import State
 from washpy.status import *
 from washpy.role import Role
 from washpy.user import User
 
 
@@ -16,15 +18,21 @@
     Represents a user on a device.
 
     This class is used to interface with the actual machine,
     most of the methods of this class perform HTTP requests.
     """
 
     device_url: Final[str]
-    """e.g. `'https://192.168.1.251/Devices/000116343328'`"""
+    """
+    must be a valid `DeviceUrl` and follow this scheme:
+
+    `https://<device_address>/Devices/<device_id>`
+
+    e.g. `'https://192.168.1.251/Devices/000116343328'`
+    """
 
     user: Final[str]
     """username"""
 
     password: str
 
     token: str
@@ -35,32 +43,49 @@
     timedelta. From the date when the `token` was last used,
     the `token` stays valid for the duration of `timeout`
     """
 
     last_used: datetime.datetime
     """date when the `token` was last used"""
 
-    def __init__(self, device_url: str, user: str, password: str) -> None:
+    verify_https: Final[bool | str]
+    """is passed to the `requests.request` `verify` argument"""
+
+    def __init__(
+        self,
+        device_url: str | DeviceUrl,
+        user: str,
+        password: str,
+        verify_https: bool | str = False,
+    ) -> None:
         """
         `device_url`: e.g. `'https://192.168.1.251/Devices/000116343328'`
 
         `user`: a username
 
         `password`: the password of user
 
+        `validate`: is passed to the `requests.request` `validate` argument.
+            Default value: `False`. Miele XKM modules produce self-signed SSL certificates per default.
+            These self-signed certificates cannot be verified.
+            It is possible to upload custom SSL certificates to the modules, in this case you can switch HTTPS validation on.
+
         Authenticates the user at the specified machine
 
         **raises**: see `washpy.authenticate`
         """
         self.user = user
         self.password = password
-        self.device_url = device_url
+        self.verify_https = verify_https
+
+        self.device_url = parse_and_validate_device_url_to_str(device_url)
+
         self.last_used = datetime.datetime.now()
         (self.token, self.timeout) = authenticate(
-            self.device_url, self.user, self.password
+            self.device_url, self.user, self.password, verify_https=self.verify_https
         )
 
     def __repr__(self) -> str:
         return (
             f"DeviceUser(device_url='{self.device_url}', "
             f"user='{self.user}', "
             f"password='~~ HIDDEN ~~', "
@@ -82,15 +107,15 @@
         url = self.device_url + api_endpoint
 
         payload = {}
         headers = {"Authorization": f"Bearer {self.token}"}
 
         now = self.refresh_authentication()
         response = requests.request(
-            "GET", url, headers=headers, data=payload, verify=False
+            "GET", url, headers=headers, data=payload, verify=self.verify_https
         )
 
         if response.status_code != 200:
             raise ValueError(f"Unable to GET: got HTTP response {response}")
         self.last_used = now
         return response.json()
 
@@ -102,15 +127,15 @@
         """
         url = self.device_url + api_endpoint
 
         headers = {"Authorization": f"Bearer {self.token}"}
 
         now = self.refresh_authentication()
         response = requests.request(
-            "POST", url, headers=headers, data=payload, verify=False
+            "POST", url, headers=headers, data=payload, verify=self.verify_https
         )
 
         if response.status_code != 201:
             raise ValueError(f"Unable to POST: got HTTP response {response}")
         self.last_used = now
 
     def _do_put_request(self, api_endpoint: str, payload: str) -> None:
@@ -121,15 +146,15 @@
         """
         url = self.device_url + api_endpoint
 
         headers = {"Authorization": f"Bearer {self.token}"}
 
         now = self.refresh_authentication()
         response = requests.request(
-            "PUT", url, headers=headers, data=payload, verify=False
+            "PUT", url, headers=headers, data=payload, verify=self.verify_https
         )
 
         if response.status_code != 200:
             raise ValueError(f"Unable to PUT: got HTTP response {response}")
         self.last_used = now
 
     def _do_delete_request(self, api_endpoint: str) -> None:
@@ -141,15 +166,15 @@
         url = self.device_url + api_endpoint
 
         headers = {"Authorization": f"Bearer {self.token}"}
 
         payload = {}
         now = self.refresh_authentication()
         response = requests.request(
-            "DELETE", url, headers=headers, data=payload, verify=False
+            "DELETE", url, headers=headers, data=payload, verify=self.verify_https
         )
 
         if response.status_code != 204:
             raise ValueError(f"Unable to DELETE: got HTTP response {response}")
         self.last_used = now
 
     # ~~~ basic management section ~~~
```

### Comparing `washpy-0.3.0/washpy/pExtended.py` & `washpy-0.4.0/washpy/pExtended.py`

 * *Files identical despite different names*

### Comparing `washpy-0.3.0/washpy/permission.py` & `washpy-0.4.0/washpy/permission.py`

 * *Files identical despite different names*

### Comparing `washpy-0.3.0/washpy/post_new_password.py` & `washpy-0.4.0/washpy/post_new_password.py`

 * *Files 19% similar despite different names*

```diff
@@ -1,29 +1,35 @@
 import requests
 import json
 
 
 def post_new_password(
-    device_url: str, user: str, password_old: str, password_new: str
+    device_url: str,
+    user: str,
+    password_old: str,
+    password_new: str,
+    verify_https: bool | str = False,
 ) -> None:
     """
     `device_url`: e.g. `'https://192.168.1.251/Devices/000116343328'`
 
     `user`: e.g. `'MYUSER'`
 
     `password_old`: old password
 
     `password_new`: the new password to be set
 
+    `verify_https`: is passed to the `requests.request` `verify` argument
+
     **raises**: `ValueError`, if the password change was unsuccessfull
     """
     payload = json.dumps(
         {"LoginName": user, "Password": password_old, "PasswordNew": password_new}
     )
     headers = {"Content-Type": "application/json"}
 
     url = device_url + "/profSession"
     response = requests.request(
-        "POST", url, headers=headers, data=payload, verify=False
+        "POST", url, headers=headers, data=payload, verify=verify_https
     )
     if response.status_code != 204:
         raise ValueError(f"something went wrong: got HTTP response {response}")
```

### Comparing `washpy-0.3.0/washpy/role.py` & `washpy-0.4.0/washpy/role.py`

 * *Files identical despite different names*

### Comparing `washpy-0.3.0/washpy/state.py` & `washpy-0.4.0/washpy/state.py`

 * *Files identical despite different names*

### Comparing `washpy-0.3.0/washpy/status.py` & `washpy-0.4.0/washpy/status.py`

 * *Files identical despite different names*

### Comparing `washpy-0.3.0/washpy/user.py` & `washpy-0.4.0/washpy/user.py`

 * *Files identical despite different names*

### Comparing `washpy-0.3.0/PKG-INFO` & `washpy-0.4.0/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,24 +1,25 @@
 Metadata-Version: 2.1
 Name: washpy
-Version: 0.3.0
+Version: 0.4.0
 Summary: A partial implementation of the Miele Professional IP Profile API
 Home-page: https://codeberg.org/johann-cm/washpy
 License: LGPL-3.0-only
 Author: Johann Carl Meyer
 Author-email: info@johannc.de
 Requires-Python: >=3.10,<4.0
 Classifier: License :: OSI Approved :: GNU Lesser General Public License v3 (LGPLv3)
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: Python :: 3.12
 Requires-Dist: isodate (>=0.6.1,<0.7.0)
 Requires-Dist: pydantic (>=2.7.1,<3.0.0)
 Requires-Dist: requests (==2.29.0)
+Requires-Dist: types-requests (==2.29.0.0)
 Project-URL: Documentation, https://johann-cm.codeberg.page/washpy/washpy.html
 Project-URL: Repository, https://codeberg.org/johann-cm/washpy
 Description-Content-Type: text/markdown
 
 # washpy
 
 [![PyPI](https://img.shields.io/pypi/v/washpy.svg)](https://pypi.org/project/washpy/)
```

