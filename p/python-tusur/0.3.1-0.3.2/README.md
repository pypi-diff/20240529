# Comparing `tmp/python-tusur-0.3.1.tar.gz` & `tmp/python-tusur-0.3.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "python-tusur-0.3.1.tar", last modified: Thu Aug 24 14:59:59 2023, max compression
+gzip compressed data, was "python-tusur-0.3.2.tar", last modified: Wed May 29 18:49:06 2024, max compression
```

## Comparing `python-tusur-0.3.1.tar` & `python-tusur-0.3.2.tar`

### file list

```diff
@@ -1,27 +1,27 @@
-drwxrwxrwx   0        0        0        0 2023-08-24 14:59:59.751325 python-tusur-0.3.1/
--rw-rw-rw-   0        0        0     1088 2023-08-18 18:44:16.000000 python-tusur-0.3.1/LICENSE
--rw-rw-rw-   0        0        0     1843 2023-08-24 14:59:59.751325 python-tusur-0.3.1/PKG-INFO
--rw-rw-rw-   0        0        0     1338 2023-08-24 14:58:24.000000 python-tusur-0.3.1/README.md
--rw-rw-rw-   0        0        0      468 2023-08-24 14:58:24.000000 python-tusur-0.3.1/pyproject.toml
-drwxrwxrwx   0        0        0        0 2023-08-24 14:59:59.733326 python-tusur-0.3.1/python_tusur.egg-info/
--rw-rw-rw-   0        0        0     1843 2023-08-24 14:59:59.000000 python-tusur-0.3.1/python_tusur.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      468 2023-08-24 14:59:59.000000 python-tusur-0.3.1/python_tusur.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-08-24 14:59:59.000000 python-tusur-0.3.1/python_tusur.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       40 2023-08-24 14:59:59.000000 python-tusur-0.3.1/python_tusur.egg-info/requires.txt
--rw-rw-rw-   0        0        0       12 2023-08-24 14:59:59.000000 python-tusur-0.3.1/python_tusur.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2023-08-24 14:59:59.753326 python-tusur-0.3.1/setup.cfg
--rw-rw-rw-   0        0        0      812 2023-08-24 14:59:47.000000 python-tusur-0.3.1/setup.py
-drwxrwxrwx   0        0        0        0 2023-08-24 14:59:59.739327 python-tusur-0.3.1/tests/
--rw-rw-rw-   0        0        0        0 2023-08-24 14:58:24.000000 python-tusur-0.3.1/tests/__init__.py
--rw-rw-rw-   0        0        0      538 2023-08-24 14:58:24.000000 python-tusur-0.3.1/tests/test_messages.py
--rw-rw-rw-   0        0        0      578 2023-08-24 14:58:24.000000 python-tusur-0.3.1/tests/test_notifications.py
--rw-rw-rw-   0        0        0     1103 2023-08-24 14:58:24.000000 python-tusur-0.3.1/tests/test_ocenka.py
--rw-rw-rw-   0        0        0      369 2023-08-24 14:58:24.000000 python-tusur-0.3.1/tests/test_timetable.py
-drwxrwxrwx   0        0        0        0 2023-08-24 14:59:59.750326 python-tusur-0.3.1/tusur/
--rw-rw-rw-   0        0        0      304 2023-08-24 14:58:24.000000 python-tusur-0.3.1/tusur/__init__.py
--rw-rw-rw-   0        0        0     1405 2023-08-24 14:58:24.000000 python-tusur-0.3.1/tusur/ajax.py
--rw-rw-rw-   0        0        0     2553 2023-08-24 14:58:24.000000 python-tusur-0.3.1/tusur/authorization.py
--rw-rw-rw-   0        0        0      621 2023-08-24 14:58:24.000000 python-tusur-0.3.1/tusur/constants.py
--rw-rw-rw-   0        0        0      587 2023-08-24 14:58:24.000000 python-tusur-0.3.1/tusur/exceptions.py
--rw-rw-rw-   0        0        0     3148 2023-08-24 14:58:24.000000 python-tusur-0.3.1/tusur/sdo.py
--rw-rw-rw-   0        0        0     9880 2023-08-24 14:58:24.000000 python-tusur-0.3.1/tusur/session.py
+drwxrwxrwx   0        0        0        0 2024-05-29 18:49:06.767390 python-tusur-0.3.2/
+-rw-rw-rw-   0        0        0     1088 2024-01-10 08:03:29.000000 python-tusur-0.3.2/LICENSE
+-rw-rw-rw-   0        0        0     1922 2024-05-29 18:49:06.766389 python-tusur-0.3.2/PKG-INFO
+-rw-rw-rw-   0        0        0     1338 2024-01-10 08:03:29.000000 python-tusur-0.3.2/README.md
+-rw-rw-rw-   0        0        0      468 2024-05-29 18:14:21.000000 python-tusur-0.3.2/pyproject.toml
+drwxrwxrwx   0        0        0        0 2024-05-29 18:49:06.739392 python-tusur-0.3.2/python_tusur.egg-info/
+-rw-rw-rw-   0        0        0     1922 2024-05-29 18:49:06.000000 python-tusur-0.3.2/python_tusur.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      468 2024-05-29 18:49:06.000000 python-tusur-0.3.2/python_tusur.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-05-29 18:49:06.000000 python-tusur-0.3.2/python_tusur.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       40 2024-05-29 18:49:06.000000 python-tusur-0.3.2/python_tusur.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       12 2024-05-29 18:49:06.000000 python-tusur-0.3.2/python_tusur.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2024-05-29 18:49:06.776587 python-tusur-0.3.2/setup.cfg
+-rw-rw-rw-   0        0        0      819 2024-05-29 18:45:50.000000 python-tusur-0.3.2/setup.py
+drwxrwxrwx   0        0        0        0 2024-05-29 18:49:06.750392 python-tusur-0.3.2/tests/
+-rw-rw-rw-   0        0        0        0 2024-01-10 08:03:29.000000 python-tusur-0.3.2/tests/__init__.py
+-rw-rw-rw-   0        0        0      538 2024-01-10 08:03:29.000000 python-tusur-0.3.2/tests/test_messages.py
+-rw-rw-rw-   0        0        0      578 2024-01-10 08:03:29.000000 python-tusur-0.3.2/tests/test_notifications.py
+-rw-rw-rw-   0        0        0     1103 2024-01-10 08:03:29.000000 python-tusur-0.3.2/tests/test_ocenka.py
+-rw-rw-rw-   0        0        0      369 2024-01-10 08:03:29.000000 python-tusur-0.3.2/tests/test_timetable.py
+drwxrwxrwx   0        0        0        0 2024-05-29 18:49:06.765389 python-tusur-0.3.2/tusur/
+-rw-rw-rw-   0        0        0      304 2024-01-10 08:03:29.000000 python-tusur-0.3.2/tusur/__init__.py
+-rw-rw-rw-   0        0        0     1521 2024-01-10 08:03:29.000000 python-tusur-0.3.2/tusur/ajax.py
+-rw-rw-rw-   0        0        0     2549 2024-01-10 08:03:29.000000 python-tusur-0.3.2/tusur/authorization.py
+-rw-rw-rw-   0        0        0      621 2024-05-29 18:13:56.000000 python-tusur-0.3.2/tusur/constants.py
+-rw-rw-rw-   0        0        0      587 2024-01-10 08:03:29.000000 python-tusur-0.3.2/tusur/exceptions.py
+-rw-rw-rw-   0        0        0     3168 2024-05-29 18:13:47.000000 python-tusur-0.3.2/tusur/sdo.py
+-rw-rw-rw-   0        0        0    10394 2024-05-29 18:12:33.000000 python-tusur-0.3.2/tusur/session.py
```

### Comparing `python-tusur-0.3.1/LICENSE` & `python-tusur-0.3.2/LICENSE`

 * *Files identical despite different names*

### Comparing `python-tusur-0.3.1/PKG-INFO` & `python-tusur-0.3.2/PKG-INFO`

 * *Files 13% similar despite different names*

```diff
@@ -1,21 +1,23 @@
 Metadata-Version: 2.1
 Name: python-tusur
-Version: 0.3.1
+Version: 0.3.2
 Summary: A project that allows you to work with tusur.ru via python
-Home-page: https://github.com/Weebp-Team/tusur
+Home-page: https://github.com/Weebp-Team/python-tusur
 Author: Tarodictrl
 Author-email: vudi600@gmail.com
 Keywords: python python3.7 tusur
 Classifier: Programming Language :: Python :: 3.11
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.7
 Description-Content-Type: text/markdown
 License-File: LICENSE
+Requires-Dist: requests>=2.31.0
+Requires-Dist: beautifulsoup4>=4.12.2
 
 # Tusur API
 ![PyPI](https://img.shields.io/pypi/v/python-tusur?color=orange) ![GitHub Pull Requests](https://img.shields.io/github/issues-pr/Weebp-Team/python-tusur?color=blueviolet) ![License](https://img.shields.io/pypi/l/python-tusur?color=blueviolet) ![Forks](https://img.shields.io/github/forks/Weebp-team/python-tusur?style=social)
 
 Python library for working with site TUSUR
 
 ## Installation
```

### Comparing `python-tusur-0.3.1/README.md` & `python-tusur-0.3.2/README.md`

 * *Files identical despite different names*

### Comparing `python-tusur-0.3.1/python_tusur.egg-info/PKG-INFO` & `python-tusur-0.3.2/python_tusur.egg-info/PKG-INFO`

 * *Files 13% similar despite different names*

```diff
@@ -1,21 +1,23 @@
 Metadata-Version: 2.1
 Name: python-tusur
-Version: 0.3.1
+Version: 0.3.2
 Summary: A project that allows you to work with tusur.ru via python
-Home-page: https://github.com/Weebp-Team/tusur
+Home-page: https://github.com/Weebp-Team/python-tusur
 Author: Tarodictrl
 Author-email: vudi600@gmail.com
 Keywords: python python3.7 tusur
 Classifier: Programming Language :: Python :: 3.11
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.7
 Description-Content-Type: text/markdown
 License-File: LICENSE
+Requires-Dist: requests>=2.31.0
+Requires-Dist: beautifulsoup4>=4.12.2
 
 # Tusur API
 ![PyPI](https://img.shields.io/pypi/v/python-tusur?color=orange) ![GitHub Pull Requests](https://img.shields.io/github/issues-pr/Weebp-Team/python-tusur?color=blueviolet) ![License](https://img.shields.io/pypi/l/python-tusur?color=blueviolet) ![Forks](https://img.shields.io/github/forks/Weebp-team/python-tusur?style=social)
 
 Python library for working with site TUSUR
 
 ## Installation
```

### Comparing `python-tusur-0.3.1/setup.py` & `python-tusur-0.3.2/setup.py`

 * *Files 7% similar despite different names*

```diff
@@ -4,21 +4,21 @@
 def readme():
     with open('README.md', 'r') as f:
         return f.read()
 
 
 setup(
     name='python-tusur',
-    version='0.3.1',
+    version='0.3.2',
     author='Tarodictrl',
     author_email='vudi600@gmail.com',
     description='A project that allows you to work with tusur.ru via python',
     long_description=readme(),
     long_description_content_type='text/markdown',
-    url='https://github.com/Weebp-Team/tusur',
+    url='https://github.com/Weebp-Team/python-tusur',
     packages=find_packages(),
     install_requires=['requests>=2.31.0', 'beautifulsoup4>=4.12.2'],
     classifiers=[
         'Programming Language :: Python :: 3.11',
         'License :: OSI Approved :: MIT License',
         'Operating System :: OS Independent'
     ],
```

### Comparing `python-tusur-0.3.1/tests/test_messages.py` & `python-tusur-0.3.2/tests/test_messages.py`

 * *Files identical despite different names*

### Comparing `python-tusur-0.3.1/tests/test_notifications.py` & `python-tusur-0.3.2/tests/test_notifications.py`

 * *Files identical despite different names*

### Comparing `python-tusur-0.3.1/tests/test_ocenka.py` & `python-tusur-0.3.2/tests/test_ocenka.py`

 * *Files identical despite different names*

### Comparing `python-tusur-0.3.1/tusur/ajax.py` & `python-tusur-0.3.2/tusur/ajax.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,13 +1,17 @@
 from .exceptions import TusurError
 from .constants import AJAX_SERVICE_URL
+from requests import Session
 
 
 class Ajax:
-    def _ajax_send(self, params: dict, data: dict) -> dict:
+    def __init__(self, session: Session) -> None:
+        self.__session = session
+
+    def _send(self, params: dict, data: dict) -> dict:
         """
         Send an AJAX request to a specified URL
         with the provided parameters and data.
 
         Args:
             params (dict): Query parameters to be included in the request URL.
             data (dict): JSON data payload to be sent in the request body.
@@ -16,21 +20,21 @@
             dict: A dictionary containing the JSON response
             received from the AJAX request.
 
         Raises:
             TusurError: If an error is encountered in the JSON response.
 
         Example:
-            ajax_instance = Ajax()
+            ajax_instance = Ajax(session)
             params = {'key': 'value'}
             data = {'data_key': 'data_value'}
-            response = ajax_instance._ajax_send(params, data)
+            response = ajax_instance._send(params, data)
         """
-        response = self._session.post(AJAX_SERVICE_URL,
-                                      params=params, json=data)
+        response = self.__session.post(AJAX_SERVICE_URL,
+                                       params=params, json=data)
 
         if response.status_code == 200:
             json_response = response.json()
 
             if type(json_response) is list:
                 if json_response[0]["error"]:
                     raise TusurError(json_response[0]["error"])
```

### Comparing `python-tusur-0.3.1/tusur/authorization.py` & `python-tusur-0.3.2/tusur/authorization.py`

 * *Files 2% similar despite different names*

```diff
@@ -17,15 +17,15 @@
         self.__password = password
         self._session = session()
         self.__auth()
         self.__sdo_auth()
 
     def __auth(self):
         """
-        Perform user authentication.
+        Perform tusur.ru authentication.
 
         Raises:
             AuthorizationFailed: If authentication is unsuccessful.
         """
         form = {
             "utf8": "✓",
             "user[email]": self.__login,
@@ -33,15 +33,15 @@
         }
         response = self._session.post(AUTH_URL, data=form)
         if not response.url.endswith("dashboard"):
             raise AuthorizationFailed()
 
     def __sdo_auth(self):
         """
-        Perform SDO (Single Sign-On) authentication.
+        Perform sdo.tusur.ru authentication.
         """
         self._session.get(AUTH_URL,
                           params={
                               "redirect_url": SDO_AUTH_REDIRECT_URL
                           })
 
     def _get_sesskey(self, response: Response) -> str:
```

### Comparing `python-tusur-0.3.1/tusur/constants.py` & `python-tusur-0.3.2/tusur/constants.py`

 * *Files identical despite different names*

### Comparing `python-tusur-0.3.1/tusur/exceptions.py` & `python-tusur-0.3.2/tusur/exceptions.py`

 * *Files identical despite different names*

### Comparing `python-tusur-0.3.1/tusur/sdo.py` & `python-tusur-0.3.2/tusur/sdo.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,24 +1,24 @@
 from typing import List
 from .authorization import Auth
 from .ajax import Ajax
 from .constants import NOTIFICATIONS_URL, MESSAGES_URL
 
 
-class Notifications(Auth, Ajax):
+class Notifications(Auth):
     def __init__(self, login: str, password: str) -> None:
         """
         Initialize an instance of the Notifications class.
 
         Args:
             login (str): The user's login/email.
             password (str): The user's password.
         """
         Auth.__init__(self, login, password)
-        Ajax.__init__(self)
+        self.__ajax = Ajax(self._session)
 
     def get_notifications(self, limit: int = 1000,
                           offset: int = 0) -> List[dict]:
         """
         Get notifications for the authenticated user.
 
         Args:
@@ -47,29 +47,29 @@
                 "useridto": contextInstanceId
             }
         }]
         params = {
             "sesskey": sesskey,
             "info": "message_popup_get_popup_notifications"
         }
-        notifications = self._ajax_send(params=params, data=data)
+        notifications = self.__ajax._send(params=params, data=data)
         return notifications
 
 
-class Messages(Auth, Ajax):
+class Messages(Auth):
     def __init__(self, login: str, password: str) -> None:
         """
         Initialize an instance of the Notifications class.
 
         Args:
             login (str): The user's login/email.
             password (str): The user's password.
         """
         Auth.__init__(self, login, password)
-        Ajax.__init__(self)
+        self.__ajax = Ajax(self._session)
 
     def get_messages(self, favourites: bool = False) -> list:
         response = self._session.get(MESSAGES_URL)
         sesskey = self._get_sesskey(response)
         contextInstanceId = self._get_contextInstanceId(response)
         data = [{
             "index": 0,
@@ -82,9 +82,9 @@
                 "userid": contextInstanceId
             }
         }]
         params = {
             "sesskey": sesskey,
             "info": "core_message_get_conversations"
         }
-        messages = self._ajax_send(params=params, data=data)
+        messages = self.__ajax._send(params=params, data=data)
         return messages
```

### Comparing `python-tusur-0.3.1/tusur/session.py` & `python-tusur-0.3.2/tusur/session.py`

 * *Files 5% similar despite different names*

```diff
@@ -35,15 +35,18 @@
             "utf8": "✓",
             "search[common]": search_data,
             "commit": ""
         }
         response = self.__session.get(url=COMMON_SEARCH_URL,
                                       params=params)
         if len(response.history) == 0:
-            raise TimetableNotFound(search_data)
+            group_url = self.__parse_group(response.content, search_data)
+            if group_url is None:
+                raise TimetableNotFound(search_data)
+            return group_url
         return response.url
 
     @staticmethod
     def __normalize_text(text: str) -> str | None:
         """
         Normalize the provided text by removing extra spaces and newlines.
 
@@ -53,15 +56,23 @@
         Returns:
             str | None: The normalized text, or None if the input was None.
         """
         if text is not None:
             striped_text = text.strip()
             replaced_text = striped_text.replace("  ", "")
             return replaced_text.replace("\n", " ")
-        return None
+    
+    @staticmethod
+    def __parse_group(response: str, group: str) -> str | None:
+        soup = BeautifulSoup(response, "html.parser")
+        ul = soup.find("ul", class_="list-inline")
+        for a in ul.find_all("a"):
+            href: str = a.get("href")
+            if href.endswith(group) and "groups" in href:
+                return "https://timetable.tusur.ru" + href
 
     def __parse_timetable(self, response: Response) -> list:
         """
         Parse the timetable information from the provided response.
 
         Args:
             response (Response): The response containing timetable information.
```

