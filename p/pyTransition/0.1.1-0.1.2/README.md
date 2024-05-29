# Comparing `tmp/pytransition-0.1.1.tar.gz` & `tmp/pytransition-0.1.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pytransition-0.1.1.tar", last modified: Thu May 23 13:34:09 2024, max compression
+gzip compressed data, was "pytransition-0.1.2.tar", last modified: Wed May 29 20:30:16 2024, max compression
```

## Comparing `pytransition-0.1.1.tar` & `pytransition-0.1.2.tar`

### file list

```diff
@@ -1,18 +1,18 @@
-drwxrwxr-x   0 scientist  (1000) scientist  (1000)        0 2024-05-23 13:34:09.898708 pytransition-0.1.1/
--rw-rw-r--   0 scientist  (1000) scientist  (1000)     1080 2024-05-06 12:29:32.000000 pytransition-0.1.1/LICENSE
--rw-r--r--   0 scientist  (1000) scientist  (1000)    18908 2024-05-23 13:34:09.898708 pytransition-0.1.1/PKG-INFO
--rw-rw-r--   0 scientist  (1000) scientist  (1000)    18480 2024-05-06 12:29:32.000000 pytransition-0.1.1/README.md
-drwxrwxr-x   0 scientist  (1000) scientist  (1000)        0 2024-05-23 13:34:09.894708 pytransition-0.1.1/pyTransition/
--rw-rw-r--   0 scientist  (1000) scientist  (1000)      198 2024-05-06 12:29:32.000000 pytransition-0.1.1/pyTransition/__init__.py
--rw-rw-r--   0 scientist  (1000) scientist  (1000)    14241 2024-05-22 21:47:02.000000 pytransition-0.1.1/pyTransition/transition.py
-drwxrwxr-x   0 scientist  (1000) scientist  (1000)        0 2024-05-23 13:34:09.894708 pytransition-0.1.1/pyTransition.egg-info/
--rw-r--r--   0 scientist  (1000) scientist  (1000)    18908 2024-05-23 13:34:09.000000 pytransition-0.1.1/pyTransition.egg-info/PKG-INFO
--rw-rw-r--   0 scientist  (1000) scientist  (1000)      300 2024-05-23 13:34:09.000000 pytransition-0.1.1/pyTransition.egg-info/SOURCES.txt
--rw-rw-r--   0 scientist  (1000) scientist  (1000)        1 2024-05-23 13:34:09.000000 pytransition-0.1.1/pyTransition.egg-info/dependency_links.txt
--rw-rw-r--   0 scientist  (1000) scientist  (1000)       23 2024-05-23 13:34:09.000000 pytransition-0.1.1/pyTransition.egg-info/requires.txt
--rw-rw-r--   0 scientist  (1000) scientist  (1000)       19 2024-05-23 13:34:09.000000 pytransition-0.1.1/pyTransition.egg-info/top_level.txt
--rw-rw-r--   0 scientist  (1000) scientist  (1000)       38 2024-05-23 13:34:09.898708 pytransition-0.1.1/setup.cfg
--rw-rw-r--   0 scientist  (1000) scientist  (1000)     1720 2024-05-23 13:33:51.000000 pytransition-0.1.1/setup.py
-drwxrwxr-x   0 scientist  (1000) scientist  (1000)        0 2024-05-23 13:34:09.894708 pytransition-0.1.1/tests/
--rw-rw-r--   0 scientist  (1000) scientist  (1000)        0 2024-05-06 12:29:32.000000 pytransition-0.1.1/tests/__init__.py
--rw-rw-r--   0 scientist  (1000) scientist  (1000)    12251 2024-05-22 21:47:02.000000 pytransition-0.1.1/tests/test_transition.py
+drwxrwxr-x   0 scientist  (1000) scientist  (1000)        0 2024-05-29 20:30:16.581109 pytransition-0.1.2/
+-rw-rw-r--   0 scientist  (1000) scientist  (1000)     1080 2024-05-06 12:29:32.000000 pytransition-0.1.2/LICENSE
+-rw-r--r--   0 scientist  (1000) scientist  (1000)    18908 2024-05-29 20:30:16.581109 pytransition-0.1.2/PKG-INFO
+-rw-rw-r--   0 scientist  (1000) scientist  (1000)    18480 2024-05-06 12:29:32.000000 pytransition-0.1.2/README.md
+drwxrwxr-x   0 scientist  (1000) scientist  (1000)        0 2024-05-29 20:30:16.581109 pytransition-0.1.2/pyTransition/
+-rw-rw-r--   0 scientist  (1000) scientist  (1000)      198 2024-05-06 12:29:32.000000 pytransition-0.1.2/pyTransition/__init__.py
+-rw-rw-r--   0 scientist  (1000) scientist  (1000)    14787 2024-05-29 20:29:16.000000 pytransition-0.1.2/pyTransition/transition.py
+drwxrwxr-x   0 scientist  (1000) scientist  (1000)        0 2024-05-29 20:30:16.581109 pytransition-0.1.2/pyTransition.egg-info/
+-rw-r--r--   0 scientist  (1000) scientist  (1000)    18908 2024-05-29 20:30:16.000000 pytransition-0.1.2/pyTransition.egg-info/PKG-INFO
+-rw-rw-r--   0 scientist  (1000) scientist  (1000)      300 2024-05-29 20:30:16.000000 pytransition-0.1.2/pyTransition.egg-info/SOURCES.txt
+-rw-rw-r--   0 scientist  (1000) scientist  (1000)        1 2024-05-29 20:30:16.000000 pytransition-0.1.2/pyTransition.egg-info/dependency_links.txt
+-rw-rw-r--   0 scientist  (1000) scientist  (1000)       23 2024-05-29 20:30:16.000000 pytransition-0.1.2/pyTransition.egg-info/requires.txt
+-rw-rw-r--   0 scientist  (1000) scientist  (1000)       19 2024-05-29 20:30:16.000000 pytransition-0.1.2/pyTransition.egg-info/top_level.txt
+-rw-rw-r--   0 scientist  (1000) scientist  (1000)       38 2024-05-29 20:30:16.581109 pytransition-0.1.2/setup.cfg
+-rw-rw-r--   0 scientist  (1000) scientist  (1000)     1720 2024-05-29 20:29:16.000000 pytransition-0.1.2/setup.py
+drwxrwxr-x   0 scientist  (1000) scientist  (1000)        0 2024-05-29 20:30:16.581109 pytransition-0.1.2/tests/
+-rw-rw-r--   0 scientist  (1000) scientist  (1000)        0 2024-05-06 12:29:32.000000 pytransition-0.1.2/tests/__init__.py
+-rw-rw-r--   0 scientist  (1000) scientist  (1000)    13236 2024-05-29 20:29:16.000000 pytransition-0.1.2/tests/test_transition.py
```

### Comparing `pytransition-0.1.1/LICENSE` & `pytransition-0.1.2/LICENSE`

 * *Files identical despite different names*

### Comparing `pytransition-0.1.1/PKG-INFO` & `pytransition-0.1.2/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pyTransition
-Version: 0.1.1
+Version: 0.1.2
 Summary: A Python package to interact with the Transition API.
 Author: Transition City
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python :: 3
 Requires-Python: >=3.6
 Description-Content-Type: text/markdown
```

### Comparing `pytransition-0.1.1/README.md` & `pytransition-0.1.2/README.md`

 * *Files identical despite different names*

### Comparing `pytransition-0.1.1/pyTransition/transition.py` & `pytransition-0.1.2/pyTransition/transition.py`

 * *Files 2% similar despite different names*

```diff
@@ -131,14 +131,30 @@
             string: the user's authentication token
         """
         body = self.__build_authentication_body(username, password)
         response = requests.post(self.build_url('/token'), json=body)
         response.raise_for_status()
         return response.text
 
+    def is_token_valid(self):
+        """Check if we can connect to the server with the currently stored access information.
+
+        Returns:
+            boolean: Can we access the server with the current token
+
+        """
+        try:
+            # Currently use the simplest call which is get_routing_modes
+            # Could be changed to something simpler is we add one
+            self.get_routing_modes()
+        except:
+            # Return false if we got an exception why doing the query
+            return False
+        return True
+
     def get_paths(self):
         """Gets all paths currently loaded in the Transition application
 
         Returns:
             geojson: Transition paths as a GeoJSON LineString FeatureCollection object
         """
         headers = self.__build_headers()
```

### Comparing `pytransition-0.1.1/pyTransition.egg-info/PKG-INFO` & `pytransition-0.1.2/pyTransition.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pyTransition
-Version: 0.1.1
+Version: 0.1.2
 Summary: A Python package to interact with the Transition API.
 Author: Transition City
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python :: 3
 Requires-Python: >=3.6
 Description-Content-Type: text/markdown
```

### Comparing `pytransition-0.1.1/setup.py` & `pytransition-0.1.2/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -21,15 +21,15 @@
 # SOFTWARE.
 
 from setuptools import setup, find_packages
 from pathlib import Path
 
 setup(
     name="pyTransition",
-    version="0.1.1",
+    version="0.1.2",
     description="A Python package to interact with the Transition API.",
     long_description=open("README.md").read(),
     long_description_content_type="text/markdown",
     author="Transition City",
     packages=find_packages(),
     install_requires=["requests", "requests_mock"],
     python_requires=">=3.6",
```

### Comparing `pytransition-0.1.1/tests/test_transition.py` & `pytransition-0.1.2/tests/test_transition.py`

 * *Files 4% similar despite different names*

```diff
@@ -120,14 +120,35 @@
                 requests.exceptions.HTTPError,
                 self.test_transition_instance._Transition__request_token,
                 self.test_username,
                 self.test_password,
             )
             self.assertTrue(m.called_once)
 
+    def test_is_token_valid_true(self):
+         with requests_mock.Mocker() as m:
+            m.get(f"{self.test_url}/api/v1/routing-modes", text='["mode1","mode2"]', status_code=200)
+            valid = self.test_transition_instance.is_token_valid()
+            self.assertTrue(m.called_once)
+            self.assertTrue(valid)
+
+    def test_is_token_valid_false(self):
+         with requests_mock.Mocker() as m:
+            m.get(f"{self.test_url}/api/v1/routing-modes", text='', status_code=400)
+            valid = self.test_transition_instance.is_token_valid()
+            self.assertTrue(m.called_once)
+            self.assertFalse(valid)
+
+    def test_is_token_valid_no_connection(self):
+         with requests_mock.Mocker() as m:
+            m.get(f"{self.test_url}/api/v1/routing-modes", exc=requests.exceptions.ConnectTimeout)
+            valid = self.test_transition_instance.is_token_valid()
+            self.assertTrue(m.called_once)
+            self.assertFalse(valid)
+
     def test_get_paths(self):
         with requests_mock.Mocker() as m:
             m.get(f"{self.test_url}/api/v1/paths", json={"key": "value"}, status_code=200)
             res = self.test_transition_instance.get_paths()
             self.assertTrue(m.called_once)
             self.assertEqual(res, {"key": "value"})
```

