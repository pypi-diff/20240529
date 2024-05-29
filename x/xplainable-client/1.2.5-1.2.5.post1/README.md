# Comparing `tmp/xplainable_client-1.2.5.tar.gz` & `tmp/xplainable_client-1.2.5.post1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "xplainable_client-1.2.5.tar", last modified: Tue May 28 05:10:22 2024, max compression
+gzip compressed data, was "xplainable_client-1.2.5.post1.tar", last modified: Wed May 29 08:14:09 2024, max compression
```

## Comparing `xplainable_client-1.2.5.tar` & `xplainable_client-1.2.5.post1.tar`

### file list

```diff
@@ -1,49 +1,49 @@
-drwxrwxrwx   0        0        0        0 2024-05-28 05:10:22.690183 xplainable_client-1.2.5/
--rw-rw-rw-   0        0        0     3325 2024-03-12 06:45:15.000000 xplainable_client-1.2.5/.gitignore
--rw-rw-rw-   0        0        0    35184 2024-03-14 02:05:34.000000 xplainable_client-1.2.5/LICENSE
--rw-rw-rw-   0        0        0    45254 2024-05-28 05:10:22.689186 xplainable_client-1.2.5/PKG-INFO
--rw-rw-rw-   0        0        0     4042 2024-03-09 02:04:58.000000 xplainable_client-1.2.5/README.md
--rw-rw-rw-   0        0        0     3578 2024-05-18 06:05:50.000000 xplainable_client-1.2.5/_build.py
--rw-rw-rw-   0        0        0       23 2024-05-28 05:09:55.000000 xplainable_client-1.2.5/_version.py
--rw-rw-rw-   0        0        0      119 2024-03-09 02:04:58.000000 xplainable_client-1.2.5/config.py
--rw-rw-rw-   0        0        0      392 2024-05-17 05:10:32.000000 xplainable_client-1.2.5/docker-compose.yaml
--rw-rw-rw-   0        0        0      777 2024-05-28 05:09:55.000000 xplainable_client-1.2.5/pyproject.toml
--rw-rw-rw-   0        0        0      123 2024-05-19 00:48:35.000000 xplainable_client-1.2.5/requirements.txt
--rw-rw-rw-   0        0        0       42 2024-05-28 05:10:22.690183 xplainable_client-1.2.5/setup.cfg
--rw-rw-rw-   0        0        0      824 2024-05-28 05:09:55.000000 xplainable_client-1.2.5/setup.py
-drwxrwxrwx   0        0        0        0 2024-05-28 05:10:22.661683 xplainable_client-1.2.5/tests/
--rw-rw-rw-   0        0        0     1337 2024-05-17 05:10:32.000000 xplainable_client-1.2.5/tests/nanoid.sql
--rw-rw-rw-   0        0        0     2856 2024-05-17 05:10:32.000000 xplainable_client-1.2.5/tests/prod-db.sql
--rw-rw-rw-   0        0        0      277 2024-05-17 05:10:32.000000 xplainable_client-1.2.5/tests/test_model.py
--rw-rw-rw-   0        0        0      191 2024-05-17 05:10:32.000000 xplainable_client-1.2.5/tests/test_test.py
-drwxrwxrwx   0        0        0        0 2024-05-28 05:10:22.663683 xplainable_client-1.2.5/thebadboycorner/
--rw-rw-rw-   0        0        0     1596 2024-05-17 07:15:41.000000 xplainable_client-1.2.5/thebadboycorner/clf_model_test_jason.py
--rw-rw-rw-   0        0        0      198 2024-05-17 06:08:34.000000 xplainable_client-1.2.5/thebadboycorner/test.py
-drwxrwxrwx   0        0        0        0 2024-05-28 05:10:22.665184 xplainable_client-1.2.5/xplainable_client/
--rw-rw-rw-   0        0        0       28 2024-05-17 06:02:17.000000 xplainable_client-1.2.5/xplainable_client/__init__.py
-drwxrwxrwx   0        0        0        0 2024-05-28 05:10:22.680683 xplainable_client-1.2.5/xplainable_client/client/
--rw-rw-rw-   0        0        0      975 2024-05-17 06:08:34.000000 xplainable_client-1.2.5/xplainable_client/client/__init__.py
--rw-rw-rw-   0        0        0      129 2024-05-10 01:22:33.000000 xplainable_client-1.2.5/xplainable_client/client/_client_cog_base.py
--rw-rw-rw-   0        0        0     7535 2024-05-17 05:57:53.000000 xplainable_client-1.2.5/xplainable_client/client/_collections.py
--rw-rw-rw-   0        0        0     1295 2024-05-16 08:25:13.000000 xplainable_client-1.2.5/xplainable_client/client/_datasets.py
--rw-rw-rw-   0        0        0    14993 2024-05-17 05:59:23.000000 xplainable_client-1.2.5/xplainable_client/client/_deployments.py
--rw-rw-rw-   0        0        0     1254 2024-05-17 05:10:32.000000 xplainable_client-1.2.5/xplainable_client/client/_gpt.py
--rw-rw-rw-   0        0        0     1266 2024-05-17 05:59:23.000000 xplainable_client-1.2.5/xplainable_client/client/_inference.py
--rw-rw-rw-   0        0        0     8179 2024-05-17 07:08:08.000000 xplainable_client-1.2.5/xplainable_client/client/_misc.py
--rw-rw-rw-   0        0        0    21423 2024-05-17 07:11:19.000000 xplainable_client-1.2.5/xplainable_client/client/_models.py
--rw-rw-rw-   0        0        0    10934 2024-05-28 01:15:50.000000 xplainable_client-1.2.5/xplainable_client/client/_preprocessing.py
--rw-rw-rw-   0        0        0     4135 2024-05-17 06:47:34.000000 xplainable_client-1.2.5/xplainable_client/client/_session.py
-drwxrwxrwx   0        0        0        0 2024-05-28 05:10:22.686685 xplainable_client-1.2.5/xplainable_client/client/utils/
--rw-rw-rw-   0        0        0      127 2024-05-17 07:10:23.000000 xplainable_client-1.2.5/xplainable_client/client/utils/__init__.py
--rw-rw-rw-   0        0        0     1334 2024-03-09 02:04:58.000000 xplainable_client-1.2.5/xplainable_client/client/utils/encoders.py
--rw-rw-rw-   0        0        0      987 2024-05-17 05:57:23.000000 xplainable_client-1.2.5/xplainable_client/client/utils/helpers.py
--rw-rw-rw-   0        0        0     6633 2024-05-17 07:08:08.000000 xplainable_client-1.2.5/xplainable_client/client/utils/metrics.py
--rw-rw-rw-   0        0        0     3122 2024-03-09 02:04:58.000000 xplainable_client-1.2.5/xplainable_client/client/utils/model_parsers.py
--rw-rw-rw-   0        0        0    10818 2024-03-14 02:05:34.000000 xplainable_client-1.2.5/xplainable_client/client/utils/scanner.py
--rw-rw-rw-   0        0        0      125 2024-05-17 05:10:32.000000 xplainable_client-1.2.5/xplainable_client/pytest.ini
-drwxrwxrwx   0        0        0        0 2024-05-28 05:10:22.688185 xplainable_client-1.2.5/xplainable_client.egg-info/
--rw-rw-rw-   0        0        0    45254 2024-05-28 05:10:22.000000 xplainable_client-1.2.5/xplainable_client.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0     1206 2024-05-28 05:10:22.000000 xplainable_client-1.2.5/xplainable_client.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-05-28 05:10:22.000000 xplainable_client-1.2.5/xplainable_client.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0      114 2024-05-28 05:10:22.000000 xplainable_client-1.2.5/xplainable_client.egg-info/requires.txt
--rw-rw-rw-   0        0        0       51 2024-05-28 05:10:22.000000 xplainable_client-1.2.5/xplainable_client.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2024-05-29 08:14:09.330345 xplainable_client-1.2.5.post1/
+-rw-rw-rw-   0        0        0     3325 2024-03-12 06:45:15.000000 xplainable_client-1.2.5.post1/.gitignore
+-rw-rw-rw-   0        0        0    35184 2024-03-14 02:05:34.000000 xplainable_client-1.2.5.post1/LICENSE
+-rw-rw-rw-   0        0        0    45260 2024-05-29 08:14:09.329345 xplainable_client-1.2.5.post1/PKG-INFO
+-rw-rw-rw-   0        0        0     4042 2024-03-09 02:04:58.000000 xplainable_client-1.2.5.post1/README.md
+-rw-rw-rw-   0        0        0     3578 2024-05-18 06:05:50.000000 xplainable_client-1.2.5.post1/_build.py
+-rw-rw-rw-   0        0        0       29 2024-05-29 08:12:16.000000 xplainable_client-1.2.5.post1/_version.py
+-rw-rw-rw-   0        0        0      119 2024-03-09 02:04:58.000000 xplainable_client-1.2.5.post1/config.py
+-rw-rw-rw-   0        0        0      392 2024-05-17 05:10:32.000000 xplainable_client-1.2.5.post1/docker-compose.yaml
+-rw-rw-rw-   0        0        0      783 2024-05-29 08:12:16.000000 xplainable_client-1.2.5.post1/pyproject.toml
+-rw-rw-rw-   0        0        0      123 2024-05-19 00:48:35.000000 xplainable_client-1.2.5.post1/requirements.txt
+-rw-rw-rw-   0        0        0       42 2024-05-29 08:14:09.330345 xplainable_client-1.2.5.post1/setup.cfg
+-rw-rw-rw-   0        0        0      830 2024-05-29 08:12:16.000000 xplainable_client-1.2.5.post1/setup.py
+drwxrwxrwx   0        0        0        0 2024-05-29 08:14:09.304845 xplainable_client-1.2.5.post1/tests/
+-rw-rw-rw-   0        0        0     1337 2024-05-17 05:10:32.000000 xplainable_client-1.2.5.post1/tests/nanoid.sql
+-rw-rw-rw-   0        0        0     2856 2024-05-17 05:10:32.000000 xplainable_client-1.2.5.post1/tests/prod-db.sql
+-rw-rw-rw-   0        0        0      277 2024-05-17 05:10:32.000000 xplainable_client-1.2.5.post1/tests/test_model.py
+-rw-rw-rw-   0        0        0      191 2024-05-17 05:10:32.000000 xplainable_client-1.2.5.post1/tests/test_test.py
+drwxrwxrwx   0        0        0        0 2024-05-29 08:14:09.306345 xplainable_client-1.2.5.post1/thebadboycorner/
+-rw-rw-rw-   0        0        0     1596 2024-05-17 07:15:41.000000 xplainable_client-1.2.5.post1/thebadboycorner/clf_model_test_jason.py
+-rw-rw-rw-   0        0        0      198 2024-05-17 06:08:34.000000 xplainable_client-1.2.5.post1/thebadboycorner/test.py
+drwxrwxrwx   0        0        0        0 2024-05-29 08:14:09.307845 xplainable_client-1.2.5.post1/xplainable_client/
+-rw-rw-rw-   0        0        0       28 2024-05-17 06:02:17.000000 xplainable_client-1.2.5.post1/xplainable_client/__init__.py
+drwxrwxrwx   0        0        0        0 2024-05-29 08:14:09.321846 xplainable_client-1.2.5.post1/xplainable_client/client/
+-rw-rw-rw-   0        0        0      975 2024-05-17 06:08:34.000000 xplainable_client-1.2.5.post1/xplainable_client/client/__init__.py
+-rw-rw-rw-   0        0        0      129 2024-05-10 01:22:33.000000 xplainable_client-1.2.5.post1/xplainable_client/client/_client_cog_base.py
+-rw-rw-rw-   0        0        0     7535 2024-05-17 05:57:53.000000 xplainable_client-1.2.5.post1/xplainable_client/client/_collections.py
+-rw-rw-rw-   0        0        0     1295 2024-05-16 08:25:13.000000 xplainable_client-1.2.5.post1/xplainable_client/client/_datasets.py
+-rw-rw-rw-   0        0        0    14993 2024-05-17 05:59:23.000000 xplainable_client-1.2.5.post1/xplainable_client/client/_deployments.py
+-rw-rw-rw-   0        0        0     1254 2024-05-17 05:10:32.000000 xplainable_client-1.2.5.post1/xplainable_client/client/_gpt.py
+-rw-rw-rw-   0        0        0     1266 2024-05-17 05:59:23.000000 xplainable_client-1.2.5.post1/xplainable_client/client/_inference.py
+-rw-rw-rw-   0        0        0     8179 2024-05-17 07:08:08.000000 xplainable_client-1.2.5.post1/xplainable_client/client/_misc.py
+-rw-rw-rw-   0        0        0    21423 2024-05-17 07:11:19.000000 xplainable_client-1.2.5.post1/xplainable_client/client/_models.py
+-rw-rw-rw-   0        0        0    10934 2024-05-28 01:15:50.000000 xplainable_client-1.2.5.post1/xplainable_client/client/_preprocessing.py
+-rw-rw-rw-   0        0        0     4218 2024-05-29 08:14:03.000000 xplainable_client-1.2.5.post1/xplainable_client/client/_session.py
+drwxrwxrwx   0        0        0        0 2024-05-29 08:14:09.327345 xplainable_client-1.2.5.post1/xplainable_client/client/utils/
+-rw-rw-rw-   0        0        0      127 2024-05-17 07:10:23.000000 xplainable_client-1.2.5.post1/xplainable_client/client/utils/__init__.py
+-rw-rw-rw-   0        0        0     1334 2024-03-09 02:04:58.000000 xplainable_client-1.2.5.post1/xplainable_client/client/utils/encoders.py
+-rw-rw-rw-   0        0        0      987 2024-05-17 05:57:23.000000 xplainable_client-1.2.5.post1/xplainable_client/client/utils/helpers.py
+-rw-rw-rw-   0        0        0     6633 2024-05-17 07:08:08.000000 xplainable_client-1.2.5.post1/xplainable_client/client/utils/metrics.py
+-rw-rw-rw-   0        0        0     3122 2024-03-09 02:04:58.000000 xplainable_client-1.2.5.post1/xplainable_client/client/utils/model_parsers.py
+-rw-rw-rw-   0        0        0    10818 2024-03-14 02:05:34.000000 xplainable_client-1.2.5.post1/xplainable_client/client/utils/scanner.py
+-rw-rw-rw-   0        0        0      125 2024-05-17 05:10:32.000000 xplainable_client-1.2.5.post1/xplainable_client/pytest.ini
+drwxrwxrwx   0        0        0        0 2024-05-29 08:14:09.328345 xplainable_client-1.2.5.post1/xplainable_client.egg-info/
+-rw-rw-rw-   0        0        0    45260 2024-05-29 08:14:08.000000 xplainable_client-1.2.5.post1/xplainable_client.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0     1206 2024-05-29 08:14:09.000000 xplainable_client-1.2.5.post1/xplainable_client.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-05-29 08:14:08.000000 xplainable_client-1.2.5.post1/xplainable_client.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0      114 2024-05-29 08:14:08.000000 xplainable_client-1.2.5.post1/xplainable_client.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       51 2024-05-29 08:14:08.000000 xplainable_client-1.2.5.post1/xplainable_client.egg-info/top_level.txt
```

### Comparing `xplainable_client-1.2.5/.gitignore` & `xplainable_client-1.2.5.post1/.gitignore`

 * *Files identical despite different names*

### Comparing `xplainable_client-1.2.5/LICENSE` & `xplainable_client-1.2.5.post1/LICENSE`

 * *Files identical despite different names*

### Comparing `xplainable_client-1.2.5/PKG-INFO` & `xplainable_client-1.2.5.post1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: xplainable-client
-Version: 1.2.5
+Version: 1.2.5.post1
 Summary: The client for persisting and deploying models to Xplainable cloud.
 Author: xplainable pty ltd
 Author-email: xplainable pty ltd <contact@xplainable.io>
 License:                     GNU AFFERO GENERAL PUBLIC LICENSE
                                Version 3, 19 November 2007
         
          Copyright (C) 2007 Free Software Foundation, Inc. <https://fsf.org/>
```

### Comparing `xplainable_client-1.2.5/README.md` & `xplainable_client-1.2.5.post1/README.md`

 * *Files identical despite different names*

### Comparing `xplainable_client-1.2.5/_build.py` & `xplainable_client-1.2.5.post1/_build.py`

 * *Files identical despite different names*

### Comparing `xplainable_client-1.2.5/pyproject.toml` & `xplainable_client-1.2.5.post1/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -3,15 +3,15 @@
 build-backend = "setuptools.build_meta"
 
 [tool.setuptools.packages]
 find = {} 
 
 [project]
 name = "xplainable-client"
-version = "1.2.5"
+version = "1.2.5.post1"
 authors = [
   { name="xplainable pty ltd", email="contact@xplainable.io" },
 ]
 description = "The client for persisting and deploying models to Xplainable cloud."
 readme = "README.md"
 license = { file="LICENSE" }
 requires-python = ">=3.10"
```

### Comparing `xplainable_client-1.2.5/setup.py` & `xplainable_client-1.2.5.post1/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -4,15 +4,15 @@
     description = f.read()
 
 with open("LICENSE", "r") as f:
     license = f.read()
 
 setuptools.setup(
     name="xplainable-client",
-    version="1.2.5",
+    version="1.2.5.post1",
     author="xplainable pty ltd",
     author_email="contact@xplainable.io",
     packages=["xplainable_client"],
     description="The client for persisting and deploying models to Xplainable cloud.",
     long_description=description,
     long_description_content_type="text/markdown",
     license=license,
```

### Comparing `xplainable_client-1.2.5/tests/nanoid.sql` & `xplainable_client-1.2.5.post1/tests/nanoid.sql`

 * *Files identical despite different names*

### Comparing `xplainable_client-1.2.5/tests/prod-db.sql` & `xplainable_client-1.2.5.post1/tests/prod-db.sql`

 * *Files identical despite different names*

### Comparing `xplainable_client-1.2.5/thebadboycorner/clf_model_test_jason.py` & `xplainable_client-1.2.5.post1/thebadboycorner/clf_model_test_jason.py`

 * *Files identical despite different names*

### Comparing `xplainable_client-1.2.5/xplainable_client/client/__init__.py` & `xplainable_client-1.2.5.post1/xplainable_client/client/__init__.py`

 * *Files identical despite different names*

### Comparing `xplainable_client-1.2.5/xplainable_client/client/_collections.py` & `xplainable_client-1.2.5.post1/xplainable_client/client/_collections.py`

 * *Files identical despite different names*

### Comparing `xplainable_client-1.2.5/xplainable_client/client/_datasets.py` & `xplainable_client-1.2.5.post1/xplainable_client/client/_datasets.py`

 * *Files identical despite different names*

### Comparing `xplainable_client-1.2.5/xplainable_client/client/_deployments.py` & `xplainable_client-1.2.5.post1/xplainable_client/client/_deployments.py`

 * *Files identical despite different names*

### Comparing `xplainable_client-1.2.5/xplainable_client/client/_gpt.py` & `xplainable_client-1.2.5.post1/xplainable_client/client/_gpt.py`

 * *Files identical despite different names*

### Comparing `xplainable_client-1.2.5/xplainable_client/client/_inference.py` & `xplainable_client-1.2.5.post1/xplainable_client/client/_inference.py`

 * *Files identical despite different names*

### Comparing `xplainable_client-1.2.5/xplainable_client/client/_misc.py` & `xplainable_client-1.2.5.post1/xplainable_client/client/_misc.py`

 * *Files identical despite different names*

### Comparing `xplainable_client-1.2.5/xplainable_client/client/_models.py` & `xplainable_client-1.2.5.post1/xplainable_client/client/_models.py`

 * *Files identical despite different names*

### Comparing `xplainable_client-1.2.5/xplainable_client/client/_preprocessing.py` & `xplainable_client-1.2.5.post1/xplainable_client/client/_preprocessing.py`

 * *Files identical despite different names*

### Comparing `xplainable_client-1.2.5/xplainable_client/client/_session.py` & `xplainable_client-1.2.5.post1/xplainable_client/client/_session.py`

 * *Files 6% similar despite different names*

```diff
@@ -16,31 +16,30 @@
     Access models, preprocessors and user data from xplainable cloud. API keys
     can be generated at https://beta.xplainable.io.
 
     Args:
         api_key (str): A valid api key.
     """
 
-    def __init__(self, api_key=None, hostname='https://api.xplainable.io'):
+    def __init__(self, api_key=None, hostname='https://api.xplainable.io', org_id=None, team_id=None):
         if not api_key:
             raise ValueError('A valid API Key is required. Generate one from the xplainable app.')
 
         self.api_key = api_key
         self.hostname = hostname
         self._setup_session()  # Set up the session and other initialization steps
 
-
-        self._ext = f"organisations/{self.user_data['organisation_id']}/teams/{self.user_data['team_id']}"
-
-        # You can still use the _render_init_table here if you want to display it,
-        # or you can return the data dict for a more script-friendly approach.
-        data = self._gather_initialization_data()
-        # if not silent_mode:
-        #
-        #     self._render_init_table(data)
+        if org_id is None or team_id is None:
+            self._ext = f"organisations/{self.user_data['organisation_id']}/teams/{self.user_data['team_id']}"
+        else:
+            self._ext = f"organisations/{org_id}/teams/{team_id}"
+
+            # You can still use the _render_init_table here if you want to display it,
+            # or you can return the data dict for a more script-friendly approach.
+            data = self._gather_initialization_data()
 
     @cached_property
     def user_data(self):
         """ Retrieves the user data for the active user.
         Returns:
             dict: User data
         """
```

### Comparing `xplainable_client-1.2.5/xplainable_client/client/utils/encoders.py` & `xplainable_client-1.2.5.post1/xplainable_client/client/utils/encoders.py`

 * *Files identical despite different names*

### Comparing `xplainable_client-1.2.5/xplainable_client/client/utils/helpers.py` & `xplainable_client-1.2.5.post1/xplainable_client/client/utils/helpers.py`

 * *Files identical despite different names*

### Comparing `xplainable_client-1.2.5/xplainable_client/client/utils/metrics.py` & `xplainable_client-1.2.5.post1/xplainable_client/client/utils/metrics.py`

 * *Files identical despite different names*

### Comparing `xplainable_client-1.2.5/xplainable_client/client/utils/model_parsers.py` & `xplainable_client-1.2.5.post1/xplainable_client/client/utils/model_parsers.py`

 * *Files identical despite different names*

### Comparing `xplainable_client-1.2.5/xplainable_client/client/utils/scanner.py` & `xplainable_client-1.2.5.post1/xplainable_client/client/utils/scanner.py`

 * *Files identical despite different names*

### Comparing `xplainable_client-1.2.5/xplainable_client.egg-info/PKG-INFO` & `xplainable_client-1.2.5.post1/xplainable_client.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: xplainable-client
-Version: 1.2.5
+Version: 1.2.5.post1
 Summary: The client for persisting and deploying models to Xplainable cloud.
 Author: xplainable pty ltd
 Author-email: xplainable pty ltd <contact@xplainable.io>
 License:                     GNU AFFERO GENERAL PUBLIC LICENSE
                                Version 3, 19 November 2007
         
          Copyright (C) 2007 Free Software Foundation, Inc. <https://fsf.org/>
```

### Comparing `xplainable_client-1.2.5/xplainable_client.egg-info/SOURCES.txt` & `xplainable_client-1.2.5.post1/xplainable_client.egg-info/SOURCES.txt`

 * *Files identical despite different names*

