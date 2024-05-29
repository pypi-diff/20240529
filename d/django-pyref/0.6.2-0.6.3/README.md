# Comparing `tmp/django-pyref-0.6.2.tar.gz` & `tmp/django_pyref-0.6.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "django-pyref-0.6.2.tar", last modified: Tue Aug 22 08:22:54 2023, max compression
+gzip compressed data, was "django_pyref-0.6.3.tar", last modified: Wed May 29 13:56:22 2024, max compression
```

## Comparing `django-pyref-0.6.2.tar` & `django_pyref-0.6.3.tar`

### file list

```diff
@@ -1,40 +1,40 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-22 08:22:54.355976 django-pyref-0.6.2/
--rw-r--r--   0 runner    (1001) docker     (123)    10173 2023-08-22 08:22:31.000000 django-pyref-0.6.2/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)     1683 2023-08-22 08:22:54.355976 django-pyref-0.6.2/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      374 2023-08-22 08:22:31.000000 django-pyref-0.6.2/README.rst
--rw-r--r--   0 runner    (1001) docker     (123)       94 2023-08-22 08:22:31.000000 django-pyref-0.6.2/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)       74 2023-08-22 08:22:54.355976 django-pyref-0.6.2/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1913 2023-08-22 08:22:31.000000 django-pyref-0.6.2/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-22 08:22:54.347975 django-pyref-0.6.2/src/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-22 08:22:54.347975 django-pyref-0.6.2/src/django_pyref.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     1683 2023-08-22 08:22:54.000000 django-pyref-0.6.2/src/django_pyref.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      778 2023-08-22 08:22:54.000000 django-pyref-0.6.2/src/django_pyref.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-08-22 08:22:54.000000 django-pyref-0.6.2/src/django_pyref.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)      107 2023-08-22 08:22:54.000000 django-pyref-0.6.2/src/django_pyref.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        5 2023-08-22 08:22:54.000000 django-pyref-0.6.2/src/django_pyref.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-22 08:22:54.355976 django-pyref-0.6.2/src/refs/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-22 08:22:31.000000 django-pyref-0.6.2/src/refs/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      801 2023-08-22 08:22:31.000000 django-pyref-0.6.2/src/refs/admin.py
--rw-r--r--   0 runner    (1001) docker     (123)     1372 2023-08-22 08:22:31.000000 django-pyref-0.6.2/src/refs/api_views.py
--rw-r--r--   0 runner    (1001) docker     (123)       83 2023-08-22 08:22:31.000000 django-pyref-0.6.2/src/refs/apps.py
--rw-r--r--   0 runner    (1001) docker     (123)     1533 2023-08-22 08:22:31.000000 django-pyref-0.6.2/src/refs/export_utils.py
--rw-r--r--   0 runner    (1001) docker     (123)      768 2023-08-22 08:22:31.000000 django-pyref-0.6.2/src/refs/filters.py
--rw-r--r--   0 runner    (1001) docker     (123)     1439 2023-08-22 08:22:31.000000 django-pyref-0.6.2/src/refs/forms.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-22 08:22:54.355976 django-pyref-0.6.2/src/refs/migrations/
--rw-r--r--   0 runner    (1001) docker     (123)     2893 2023-08-22 08:22:31.000000 django-pyref-0.6.2/src/refs/migrations/0001_initial.py
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-22 08:22:31.000000 django-pyref-0.6.2/src/refs/migrations/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    15007 2023-08-22 08:22:31.000000 django-pyref-0.6.2/src/refs/models.py
--rw-r--r--   0 runner    (1001) docker     (123)      468 2023-08-22 08:22:31.000000 django-pyref-0.6.2/src/refs/serializers.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-22 08:22:54.355976 django-pyref-0.6.2/src/refs/templatetags/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-22 08:22:31.000000 django-pyref-0.6.2/src/refs/templatetags/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      861 2023-08-22 08:22:31.000000 django-pyref-0.6.2/src/refs/templatetags/pyref_tags.py
--rw-r--r--   0 runner    (1001) docker     (123)     1088 2023-08-22 08:22:31.000000 django-pyref-0.6.2/src/refs/urls.py
--rw-r--r--   0 runner    (1001) docker     (123)     1303 2023-08-22 08:22:31.000000 django-pyref-0.6.2/src/refs/utils.py
--rw-r--r--   0 runner    (1001) docker     (123)     4064 2023-08-22 08:22:31.000000 django-pyref-0.6.2/src/refs/views.py
--rw-r--r--   0 runner    (1001) docker     (123)     3076 2023-08-22 08:22:31.000000 django-pyref-0.6.2/src/refs/xsams_generators.py
--rw-r--r--   0 runner    (1001) docker     (123)      144 2023-08-22 08:22:31.000000 django-pyref-0.6.2/src/refs/xsams_settings.py
--rw-r--r--   0 runner    (1001) docker     (123)     4139 2023-08-22 08:22:31.000000 django-pyref-0.6.2/src/refs/xsams_utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-22 08:22:54.355976 django-pyref-0.6.2/tests/
--rw-r--r--   0 runner    (1001) docker     (123)      774 2023-08-22 08:22:31.000000 django-pyref-0.6.2/tests/test_ref_model.py
--rw-r--r--   0 runner    (1001) docker     (123)     6186 2023-08-22 08:22:31.000000 django-pyref-0.6.2/tests/test_serialization.py
--rw-r--r--   0 runner    (1001) docker     (123)      418 2023-08-22 08:22:31.000000 django-pyref-0.6.2/tests/test_utils.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-29 13:56:22.434450 django_pyref-0.6.3/
+-rw-r--r--   0 runner    (1001) docker     (127)    10173 2024-05-29 13:56:10.000000 django_pyref-0.6.3/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)     1936 2024-05-29 13:56:22.434450 django_pyref-0.6.3/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      374 2024-05-29 13:56:10.000000 django_pyref-0.6.3/README.rst
+-rw-r--r--   0 runner    (1001) docker     (127)       94 2024-05-29 13:56:10.000000 django_pyref-0.6.3/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)       74 2024-05-29 13:56:22.434450 django_pyref-0.6.3/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)     1944 2024-05-29 13:56:10.000000 django_pyref-0.6.3/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-29 13:56:22.430450 django_pyref-0.6.3/src/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-29 13:56:22.434450 django_pyref-0.6.3/src/django_pyref.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     1936 2024-05-29 13:56:22.000000 django_pyref-0.6.3/src/django_pyref.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      778 2024-05-29 13:56:22.000000 django_pyref-0.6.3/src/django_pyref.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-29 13:56:22.000000 django_pyref-0.6.3/src/django_pyref.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      107 2024-05-29 13:56:22.000000 django_pyref-0.6.3/src/django_pyref.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        5 2024-05-29 13:56:22.000000 django_pyref-0.6.3/src/django_pyref.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-29 13:56:22.434450 django_pyref-0.6.3/src/refs/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-29 13:56:10.000000 django_pyref-0.6.3/src/refs/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      801 2024-05-29 13:56:10.000000 django_pyref-0.6.3/src/refs/admin.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1372 2024-05-29 13:56:10.000000 django_pyref-0.6.3/src/refs/api_views.py
+-rw-r--r--   0 runner    (1001) docker     (127)       83 2024-05-29 13:56:10.000000 django_pyref-0.6.3/src/refs/apps.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1533 2024-05-29 13:56:10.000000 django_pyref-0.6.3/src/refs/export_utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)      768 2024-05-29 13:56:10.000000 django_pyref-0.6.3/src/refs/filters.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1439 2024-05-29 13:56:10.000000 django_pyref-0.6.3/src/refs/forms.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-29 13:56:22.434450 django_pyref-0.6.3/src/refs/migrations/
+-rw-r--r--   0 runner    (1001) docker     (127)     2893 2024-05-29 13:56:10.000000 django_pyref-0.6.3/src/refs/migrations/0001_initial.py
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-29 13:56:10.000000 django_pyref-0.6.3/src/refs/migrations/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    15007 2024-05-29 13:56:10.000000 django_pyref-0.6.3/src/refs/models.py
+-rw-r--r--   0 runner    (1001) docker     (127)      468 2024-05-29 13:56:10.000000 django_pyref-0.6.3/src/refs/serializers.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-29 13:56:22.434450 django_pyref-0.6.3/src/refs/templatetags/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-29 13:56:10.000000 django_pyref-0.6.3/src/refs/templatetags/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      861 2024-05-29 13:56:10.000000 django_pyref-0.6.3/src/refs/templatetags/pyref_tags.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1088 2024-05-29 13:56:10.000000 django_pyref-0.6.3/src/refs/urls.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1303 2024-05-29 13:56:10.000000 django_pyref-0.6.3/src/refs/utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4064 2024-05-29 13:56:10.000000 django_pyref-0.6.3/src/refs/views.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3076 2024-05-29 13:56:10.000000 django_pyref-0.6.3/src/refs/xsams_generators.py
+-rw-r--r--   0 runner    (1001) docker     (127)      144 2024-05-29 13:56:10.000000 django_pyref-0.6.3/src/refs/xsams_settings.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4139 2024-05-29 13:56:10.000000 django_pyref-0.6.3/src/refs/xsams_utils.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-29 13:56:22.434450 django_pyref-0.6.3/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)      774 2024-05-29 13:56:10.000000 django_pyref-0.6.3/tests/test_ref_model.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6186 2024-05-29 13:56:10.000000 django_pyref-0.6.3/tests/test_serialization.py
+-rw-r--r--   0 runner    (1001) docker     (127)      418 2024-05-29 13:56:10.000000 django_pyref-0.6.3/tests/test_utils.py
```

### Comparing `django-pyref-0.6.2/LICENSE` & `django_pyref-0.6.3/LICENSE`

 * *Files identical despite different names*

### Comparing `django-pyref-0.6.2/PKG-INFO` & `django_pyref-0.6.3/PKG-INFO`

 * *Files 18% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 Metadata-Version: 2.1
 Name: django-pyref
-Version: 0.6.2
+Version: 0.6.3
 Summary: A Django app defining data models for managing bibliographic references for scientific databases.
-Home-page: https://github.com/xnx/django-valem
+Home-page: https://github.com/xnx/django-pyref
 Author: Christian Hill, Frances Skinner, Iouli Gordon, Robert Hargreaves, Kelly Lockhart, Dipti
 Author-email: ch.hill@iaea.org
 Project-URL: Bug Reports, https://github.com/xnx/django-pyref/issues
 Keywords: django,database,references,citation
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Science/Research
 Classifier: Topic :: Scientific/Engineering :: Chemistry
@@ -20,16 +20,23 @@
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: Python :: 3 :: Only
 Classifier: Framework :: Django
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.6
 Description-Content-Type: text/x-rst
-Provides-Extra: dev
 License-File: LICENSE
+Requires-Dist: Django>=3.2
+Requires-Dist: requests>=2.28.1
+Requires-Dist: djangorestframework>=3.13.1
+Requires-Dist: django-filter>=22.1
+Provides-Extra: dev
+Requires-Dist: black; extra == "dev"
+Requires-Dist: coverage; extra == "dev"
+Requires-Dist: ipython; extra == "dev"
 
 ============
 django-pyref
 ============
 
 The project, django-pyref, defines a Django app, refs, to create references for
 scientific databases.  The goal of the app is to create a referencing system
```

### Comparing `django-pyref-0.6.2/setup.py` & `django_pyref-0.6.3/setup.py`

 * *Files 4% similar despite different names*

```diff
@@ -4,20 +4,20 @@
 root = Path(__file__).parent.resolve()
 
 # Get the long description from the README file
 long_description = (root / "README.rst").read_text(encoding="utf-8")
 
 setup(
     name="django-pyref",
-    version="0.6.2",
+    version="0.6.3",
     description="A Django app defining data models for managing "
     "bibliographic references for scientific databases.",
     long_description=long_description,
     long_description_content_type="text/x-rst",
-    url="https://github.com/xnx/django-valem",
+    url="https://github.com/xnx/django-pyref",
     author="Christian Hill, Frances Skinner, Iouli Gordon, Robert Hargreaves,"
     " Kelly Lockhart, Dipti",
     author_email="ch.hill@iaea.org",
     classifiers=[
         "Development Status :: 3 - Alpha",
         "Intended Audience :: Science/Research",
         "Topic :: Scientific/Engineering :: Chemistry",
@@ -41,11 +41,12 @@
     install_requires=[
         "Django>=3.2",
         "requests>=2.28.1",
         "djangorestframework>=3.13.1",
         "django-filter>=22.1",
     ],
     extras_require={"dev": ["black", "coverage", "ipython"]},
+    include_package_data=True,
     project_urls={
         "Bug Reports": "https://github.com/xnx/django-pyref/issues",
     },
 )
```

### Comparing `django-pyref-0.6.2/src/django_pyref.egg-info/PKG-INFO` & `django_pyref-0.6.3/src/django_pyref.egg-info/PKG-INFO`

 * *Files 18% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 Metadata-Version: 2.1
 Name: django-pyref
-Version: 0.6.2
+Version: 0.6.3
 Summary: A Django app defining data models for managing bibliographic references for scientific databases.
-Home-page: https://github.com/xnx/django-valem
+Home-page: https://github.com/xnx/django-pyref
 Author: Christian Hill, Frances Skinner, Iouli Gordon, Robert Hargreaves, Kelly Lockhart, Dipti
 Author-email: ch.hill@iaea.org
 Project-URL: Bug Reports, https://github.com/xnx/django-pyref/issues
 Keywords: django,database,references,citation
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Science/Research
 Classifier: Topic :: Scientific/Engineering :: Chemistry
@@ -20,16 +20,23 @@
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: Python :: 3 :: Only
 Classifier: Framework :: Django
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.6
 Description-Content-Type: text/x-rst
-Provides-Extra: dev
 License-File: LICENSE
+Requires-Dist: Django>=3.2
+Requires-Dist: requests>=2.28.1
+Requires-Dist: djangorestframework>=3.13.1
+Requires-Dist: django-filter>=22.1
+Provides-Extra: dev
+Requires-Dist: black; extra == "dev"
+Requires-Dist: coverage; extra == "dev"
+Requires-Dist: ipython; extra == "dev"
 
 ============
 django-pyref
 ============
 
 The project, django-pyref, defines a Django app, refs, to create references for
 scientific databases.  The goal of the app is to create a referencing system
```

### Comparing `django-pyref-0.6.2/src/django_pyref.egg-info/SOURCES.txt` & `django_pyref-0.6.3/src/django_pyref.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `django-pyref-0.6.2/src/refs/admin.py` & `django_pyref-0.6.3/src/refs/admin.py`

 * *Files identical despite different names*

### Comparing `django-pyref-0.6.2/src/refs/api_views.py` & `django_pyref-0.6.3/src/refs/api_views.py`

 * *Files identical despite different names*

### Comparing `django-pyref-0.6.2/src/refs/export_utils.py` & `django_pyref-0.6.3/src/refs/export_utils.py`

 * *Files identical despite different names*

### Comparing `django-pyref-0.6.2/src/refs/filters.py` & `django_pyref-0.6.3/src/refs/filters.py`

 * *Files identical despite different names*

### Comparing `django-pyref-0.6.2/src/refs/forms.py` & `django_pyref-0.6.3/src/refs/forms.py`

 * *Files identical despite different names*

### Comparing `django-pyref-0.6.2/src/refs/migrations/0001_initial.py` & `django_pyref-0.6.3/src/refs/migrations/0001_initial.py`

 * *Files identical despite different names*

### Comparing `django-pyref-0.6.2/src/refs/models.py` & `django_pyref-0.6.3/src/refs/models.py`

 * *Files identical despite different names*

### Comparing `django-pyref-0.6.2/src/refs/templatetags/pyref_tags.py` & `django_pyref-0.6.3/src/refs/templatetags/pyref_tags.py`

 * *Files identical despite different names*

### Comparing `django-pyref-0.6.2/src/refs/urls.py` & `django_pyref-0.6.3/src/refs/urls.py`

 * *Files identical despite different names*

### Comparing `django-pyref-0.6.2/src/refs/utils.py` & `django_pyref-0.6.3/src/refs/utils.py`

 * *Files identical despite different names*

### Comparing `django-pyref-0.6.2/src/refs/views.py` & `django_pyref-0.6.3/src/refs/views.py`

 * *Files identical despite different names*

### Comparing `django-pyref-0.6.2/src/refs/xsams_generators.py` & `django_pyref-0.6.3/src/refs/xsams_generators.py`

 * *Files identical despite different names*

### Comparing `django-pyref-0.6.2/src/refs/xsams_utils.py` & `django_pyref-0.6.3/src/refs/xsams_utils.py`

 * *Files identical despite different names*

### Comparing `django-pyref-0.6.2/tests/test_ref_model.py` & `django_pyref-0.6.3/tests/test_ref_model.py`

 * *Files identical despite different names*

### Comparing `django-pyref-0.6.2/tests/test_serialization.py` & `django_pyref-0.6.3/tests/test_serialization.py`

 * *Files identical despite different names*

