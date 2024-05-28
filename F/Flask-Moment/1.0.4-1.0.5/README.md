# Comparing `tmp/Flask-Moment-1.0.4.tar.gz` & `tmp/Flask-Moment-1.0.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "Flask-Moment-1.0.4.tar", last modified: Sun Jul 17 22:32:47 2022, max compression
+gzip compressed data, was "Flask-Moment-1.0.5.tar", last modified: Wed Oct  5 13:33:23 2022, max compression
```

## Comparing `Flask-Moment-1.0.4.tar` & `Flask-Moment-1.0.5.tar`

### file list

```diff
@@ -1,18 +1,18 @@
-drwxr-xr-x   0 mgrinberg   (502) staff       (20)        0 2022-07-17 22:32:47.155643 Flask-Moment-1.0.4/
--rw-r--r--   0 mgrinberg   (502) staff       (20)     1082 2019-11-11 09:55:06.000000 Flask-Moment-1.0.4/LICENSE
--rwxr-xr-x   0 mgrinberg   (502) staff       (20)       25 2019-11-11 09:55:06.000000 Flask-Moment-1.0.4/MANIFEST.in
--rw-r--r--   0 mgrinberg   (502) staff       (20)     1272 2022-07-17 22:32:47.155864 Flask-Moment-1.0.4/PKG-INFO
--rw-r--r--   0 mgrinberg   (502) staff       (20)      663 2021-06-10 23:07:45.000000 Flask-Moment-1.0.4/README.md
--rw-r--r--   0 mgrinberg   (502) staff       (20)      104 2021-06-09 22:08:09.000000 Flask-Moment-1.0.4/pyproject.toml
--rw-r--r--   0 mgrinberg   (502) staff       (20)      813 2022-07-17 22:32:47.156711 Flask-Moment-1.0.4/setup.cfg
--rw-r--r--   0 mgrinberg   (502) staff       (20)       38 2021-06-09 22:08:09.000000 Flask-Moment-1.0.4/setup.py
-drwxr-xr-x   0 mgrinberg   (502) staff       (20)        0 2022-07-17 22:32:47.148403 Flask-Moment-1.0.4/src/
-drwxr-xr-x   0 mgrinberg   (502) staff       (20)        0 2022-07-17 22:32:47.154220 Flask-Moment-1.0.4/src/Flask_Moment.egg-info/
--rw-r--r--   0 mgrinberg   (502) staff       (20)     1272 2022-07-17 22:32:47.000000 Flask-Moment-1.0.4/src/Flask_Moment.egg-info/PKG-INFO
--rw-r--r--   0 mgrinberg   (502) staff       (20)      330 2022-07-17 22:32:47.000000 Flask-Moment-1.0.4/src/Flask_Moment.egg-info/SOURCES.txt
--rw-r--r--   0 mgrinberg   (502) staff       (20)        1 2022-07-17 22:32:47.000000 Flask-Moment-1.0.4/src/Flask_Moment.egg-info/dependency_links.txt
--rw-r--r--   0 mgrinberg   (502) staff       (20)        1 2021-06-10 22:39:15.000000 Flask-Moment-1.0.4/src/Flask_Moment.egg-info/not-zip-safe
--rw-r--r--   0 mgrinberg   (502) staff       (20)       22 2022-07-17 22:32:47.000000 Flask-Moment-1.0.4/src/Flask_Moment.egg-info/requires.txt
--rw-r--r--   0 mgrinberg   (502) staff       (20)       13 2022-07-17 22:32:47.000000 Flask-Moment-1.0.4/src/Flask_Moment.egg-info/top_level.txt
-drwxr-xr-x   0 mgrinberg   (502) staff       (20)        0 2022-07-17 22:32:47.154747 Flask-Moment-1.0.4/src/flask_moment/
--rw-r--r--   0 mgrinberg   (502) staff       (20)    15799 2022-07-16 15:24:13.000000 Flask-Moment-1.0.4/src/flask_moment/__init__.py
+drwxr-xr-x   0 mgrinberg   (502) staff       (20)        0 2022-10-05 13:33:23.176222 Flask-Moment-1.0.5/
+-rw-r--r--   0 mgrinberg   (502) staff       (20)     1082 2019-11-11 09:55:06.000000 Flask-Moment-1.0.5/LICENSE
+-rwxr-xr-x   0 mgrinberg   (502) staff       (20)       25 2019-11-11 09:55:06.000000 Flask-Moment-1.0.5/MANIFEST.in
+-rw-r--r--   0 mgrinberg   (502) staff       (20)     1272 2022-10-05 13:33:23.176447 Flask-Moment-1.0.5/PKG-INFO
+-rw-r--r--   0 mgrinberg   (502) staff       (20)      663 2021-06-10 23:07:45.000000 Flask-Moment-1.0.5/README.md
+-rw-r--r--   0 mgrinberg   (502) staff       (20)      104 2021-06-09 22:08:09.000000 Flask-Moment-1.0.5/pyproject.toml
+-rw-r--r--   0 mgrinberg   (502) staff       (20)      813 2022-10-05 13:33:23.177264 Flask-Moment-1.0.5/setup.cfg
+-rw-r--r--   0 mgrinberg   (502) staff       (20)       38 2021-06-09 22:08:09.000000 Flask-Moment-1.0.5/setup.py
+drwxr-xr-x   0 mgrinberg   (502) staff       (20)        0 2022-10-05 13:33:23.169129 Flask-Moment-1.0.5/src/
+drwxr-xr-x   0 mgrinberg   (502) staff       (20)        0 2022-10-05 13:33:23.175313 Flask-Moment-1.0.5/src/Flask_Moment.egg-info/
+-rw-r--r--   0 mgrinberg   (502) staff       (20)     1272 2022-10-05 13:33:23.000000 Flask-Moment-1.0.5/src/Flask_Moment.egg-info/PKG-INFO
+-rw-r--r--   0 mgrinberg   (502) staff       (20)      330 2022-10-05 13:33:23.000000 Flask-Moment-1.0.5/src/Flask_Moment.egg-info/SOURCES.txt
+-rw-r--r--   0 mgrinberg   (502) staff       (20)        1 2022-10-05 13:33:23.000000 Flask-Moment-1.0.5/src/Flask_Moment.egg-info/dependency_links.txt
+-rw-r--r--   0 mgrinberg   (502) staff       (20)        1 2021-06-10 22:39:15.000000 Flask-Moment-1.0.5/src/Flask_Moment.egg-info/not-zip-safe
+-rw-r--r--   0 mgrinberg   (502) staff       (20)       22 2022-10-05 13:33:23.000000 Flask-Moment-1.0.5/src/Flask_Moment.egg-info/requires.txt
+-rw-r--r--   0 mgrinberg   (502) staff       (20)       13 2022-10-05 13:33:23.000000 Flask-Moment-1.0.5/src/Flask_Moment.egg-info/top_level.txt
+drwxr-xr-x   0 mgrinberg   (502) staff       (20)        0 2022-10-05 13:33:23.175873 Flask-Moment-1.0.5/src/flask_moment/
+-rw-r--r--   0 mgrinberg   (502) staff       (20)    15799 2022-10-05 13:32:32.000000 Flask-Moment-1.0.5/src/flask_moment/__init__.py
```

### Comparing `Flask-Moment-1.0.4/LICENSE` & `Flask-Moment-1.0.5/LICENSE`

 * *Files identical despite different names*

### Comparing `Flask-Moment-1.0.4/PKG-INFO` & `Flask-Moment-1.0.5/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: Flask-Moment
-Version: 1.0.4
+Version: 1.0.5
 Summary: Formatting of dates and times in Flask templates using moment.js.
 Home-page: https://github.com/miguelgrinberg/flask-moment
 Author: Miguel Grinberg
 Author-email: miguel.grinberg@gmail.com
 Project-URL: Bug Tracker, https://github.com/miguelgrinberg/flask-moment/issues
 Classifier: Intended Audience :: Developers
 Classifier: Programming Language :: Python :: 3
```

### Comparing `Flask-Moment-1.0.4/README.md` & `Flask-Moment-1.0.5/README.md`

 * *Files identical despite different names*

### Comparing `Flask-Moment-1.0.4/setup.cfg` & `Flask-Moment-1.0.5/setup.cfg`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [metadata]
 name = Flask-Moment
-version = 1.0.4
+version = 1.0.5
 author = Miguel Grinberg
 author_email = miguel.grinberg@gmail.com
 description = Formatting of dates and times in Flask templates using moment.js.
 long_description = file: README.md
 long_description_content_type = text/markdown
 url = https://github.com/miguelgrinberg/flask-moment
 project_urls =
```

### Comparing `Flask-Moment-1.0.4/src/Flask_Moment.egg-info/PKG-INFO` & `Flask-Moment-1.0.5/src/Flask_Moment.egg-info/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: Flask-Moment
-Version: 1.0.4
+Version: 1.0.5
 Summary: Formatting of dates and times in Flask templates using moment.js.
 Home-page: https://github.com/miguelgrinberg/flask-moment
 Author: Miguel Grinberg
 Author-email: miguel.grinberg@gmail.com
 Project-URL: Bug Tracker, https://github.com/miguelgrinberg/flask-moment/issues
 Classifier: Intended Audience :: Developers
 Classifier: Programming Language :: Python :: 3
```

### Comparing `Flask-Moment-1.0.4/src/flask_moment/__init__.py` & `Flask-Moment-1.0.5/src/flask_moment/__init__.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,16 +1,16 @@
 from datetime import datetime
 from packaging.version import parse as version_parse
 from markupsafe import Markup
 from flask import current_app
 
-# //cdnjs.cloudflare.com/ajax/libs/moment.js/2.27.0/moment-with-locales.min.js
-default_moment_version = '2.29.1'
-default_moment_sri = ('sha512-LGXaggshOkD/at6PFNcp2V2unf9LzFq6LE+sChH7ceMTDP0'
-                      'g2kn6Vxwgg7wkPP7AAtX+lmPqPdxB47A0Nz0cMQ==')
+# //cdnjs.cloudflare.com/ajax/libs/moment.js/2.29.4/moment-with-locales.min.js
+default_moment_version = '2.29.4'
+default_moment_sri = ('sha512-42PE0rd+wZ2hNXftlM78BSehIGzezNeQuzihiBCvUEB3CVx'
+                      'HvsShF86wBWwQORNxNINlBPuq7rG4WWhNiTVHFg==')
 
 js_code = '''function flask_moment_render(elem) {{
     const timestamp = moment(elem.dataset.timestamp);
     const func = elem.dataset.function;
     const format = elem.dataset.format;
     const timestamp2 = elem.dataset.timestamp2;
     const no_suffix = elem.dataset.nosuffix;
```

