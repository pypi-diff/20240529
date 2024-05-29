# Comparing `tmp/django-typomatic-2.5.0.tar.gz` & `tmp/django_typomatic-2.5.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "django-typomatic-2.5.0.tar", last modified: Tue Apr  2 22:44:54 2024, max compression
+gzip compressed data, was "django_typomatic-2.5.1.tar", last modified: Wed May 29 01:53:05 2024, max compression
```

## Comparing `django-typomatic-2.5.0.tar` & `django_typomatic-2.5.1.tar`

### file list

```diff
@@ -1,27 +1,27 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-02 22:44:54.832271 django-typomatic-2.5.0/
--rw-r--r--   0 runner    (1001) docker     (127)     1068 2024-04-02 22:44:45.000000 django-typomatic-2.5.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)     9911 2024-04-02 22:44:54.832271 django-typomatic-2.5.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     9435 2024-04-02 22:44:45.000000 django-typomatic-2.5.0/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-02 22:44:54.832271 django-typomatic-2.5.0/django_typomatic/
--rw-r--r--   0 runner    (1001) docker     (127)    25266 2024-04-02 22:44:45.000000 django-typomatic-2.5.0/django_typomatic/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      651 2024-04-02 22:44:45.000000 django-typomatic-2.5.0/django_typomatic/__init__.pyi
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-02 22:44:54.832271 django-typomatic-2.5.0/django_typomatic/management/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-02 22:44:45.000000 django-typomatic-2.5.0/django_typomatic/management/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      197 2024-04-02 22:44:45.000000 django-typomatic-2.5.0/django_typomatic/management/apps.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-02 22:44:54.832271 django-typomatic-2.5.0/django_typomatic/management/commands/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-02 22:44:45.000000 django-typomatic-2.5.0/django_typomatic/management/commands/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     5398 2024-04-02 22:44:45.000000 django-typomatic-2.5.0/django_typomatic/management/commands/generate_ts.py
--rw-r--r--   0 runner    (1001) docker     (127)     1149 2024-04-02 22:44:45.000000 django-typomatic-2.5.0/django_typomatic/management/models.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-02 22:44:54.832271 django-typomatic-2.5.0/django_typomatic/management/settings/
--rw-r--r--   0 runner    (1001) docker     (127)      136 2024-04-02 22:44:45.000000 django-typomatic-2.5.0/django_typomatic/management/settings/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2230 2024-04-02 22:44:45.000000 django-typomatic-2.5.0/django_typomatic/mappings.py
--rw-r--r--   0 runner    (1001) docker     (127)    12097 2024-04-02 22:44:45.000000 django-typomatic-2.5.0/django_typomatic/test__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-02 22:44:54.832271 django-typomatic-2.5.0/django_typomatic.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     9911 2024-04-02 22:44:54.000000 django-typomatic-2.5.0/django_typomatic.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      649 2024-04-02 22:44:54.000000 django-typomatic-2.5.0/django_typomatic.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-02 22:44:54.000000 django-typomatic-2.5.0/django_typomatic.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-02 22:44:54.000000 django-typomatic-2.5.0/django_typomatic.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (127)       27 2024-04-02 22:44:54.000000 django-typomatic-2.5.0/django_typomatic.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       17 2024-04-02 22:44:54.000000 django-typomatic-2.5.0/django_typomatic.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-02 22:44:54.832271 django-typomatic-2.5.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)      789 2024-04-02 22:44:45.000000 django-typomatic-2.5.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-29 01:53:05.010525 django_typomatic-2.5.1/
+-rw-r--r--   0 runner    (1001) docker     (127)     1068 2024-05-29 01:52:57.000000 django_typomatic-2.5.1/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)     9911 2024-05-29 01:53:05.010525 django_typomatic-2.5.1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     9435 2024-05-29 01:52:57.000000 django_typomatic-2.5.1/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-29 01:53:05.006525 django_typomatic-2.5.1/django_typomatic/
+-rw-r--r--   0 runner    (1001) docker     (127)    25266 2024-05-29 01:52:57.000000 django_typomatic-2.5.1/django_typomatic/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      651 2024-05-29 01:52:57.000000 django_typomatic-2.5.1/django_typomatic/__init__.pyi
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-29 01:53:05.010525 django_typomatic-2.5.1/django_typomatic/management/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-29 01:52:57.000000 django_typomatic-2.5.1/django_typomatic/management/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      197 2024-05-29 01:52:57.000000 django_typomatic-2.5.1/django_typomatic/management/apps.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-29 01:53:05.010525 django_typomatic-2.5.1/django_typomatic/management/commands/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-29 01:52:57.000000 django_typomatic-2.5.1/django_typomatic/management/commands/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5398 2024-05-29 01:52:57.000000 django_typomatic-2.5.1/django_typomatic/management/commands/generate_ts.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1149 2024-05-29 01:52:57.000000 django_typomatic-2.5.1/django_typomatic/management/models.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-29 01:53:05.010525 django_typomatic-2.5.1/django_typomatic/management/settings/
+-rw-r--r--   0 runner    (1001) docker     (127)      136 2024-05-29 01:52:57.000000 django_typomatic-2.5.1/django_typomatic/management/settings/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2393 2024-05-29 01:52:57.000000 django_typomatic-2.5.1/django_typomatic/mappings.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12097 2024-05-29 01:52:57.000000 django_typomatic-2.5.1/django_typomatic/test__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-29 01:53:05.010525 django_typomatic-2.5.1/django_typomatic.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     9911 2024-05-29 01:53:04.000000 django_typomatic-2.5.1/django_typomatic.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      649 2024-05-29 01:53:05.000000 django_typomatic-2.5.1/django_typomatic.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-29 01:53:04.000000 django_typomatic-2.5.1/django_typomatic.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-29 01:53:04.000000 django_typomatic-2.5.1/django_typomatic.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (127)       27 2024-05-29 01:53:04.000000 django_typomatic-2.5.1/django_typomatic.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       17 2024-05-29 01:53:04.000000 django_typomatic-2.5.1/django_typomatic.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-29 01:53:05.010525 django_typomatic-2.5.1/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)      789 2024-05-29 01:52:57.000000 django_typomatic-2.5.1/setup.py
```

### Comparing `django-typomatic-2.5.0/LICENSE` & `django_typomatic-2.5.1/LICENSE`

 * *Files identical despite different names*

### Comparing `django-typomatic-2.5.0/PKG-INFO` & `django_typomatic-2.5.1/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: django-typomatic
-Version: 2.5.0
+Version: 2.5.1
 Summary: A simple solution for generating Typescript interfaces from your Django Rest Framework Serializers.
 Home-page: https://github.com/adenh93/django-typomatic
 Author: Aden Herold
 Author-email: aden.herold1@gmail.com
 Keywords: Django,Django Rest Framework,DRF,Typescript,Python
 Platform: any
 Description-Content-Type: text/markdown
```

### Comparing `django-typomatic-2.5.0/README.md` & `django_typomatic-2.5.1/README.md`

 * *Files identical despite different names*

### Comparing `django-typomatic-2.5.0/django_typomatic/__init__.py` & `django_typomatic-2.5.1/django_typomatic/__init__.py`

 * *Files identical despite different names*

### Comparing `django-typomatic-2.5.0/django_typomatic/__init__.pyi` & `django_typomatic-2.5.1/django_typomatic/__init__.pyi`

 * *Files identical despite different names*

### Comparing `django-typomatic-2.5.0/django_typomatic/management/commands/generate_ts.py` & `django_typomatic-2.5.1/django_typomatic/management/commands/generate_ts.py`

 * *Files identical despite different names*

### Comparing `django-typomatic-2.5.0/django_typomatic/management/models.py` & `django_typomatic-2.5.1/django_typomatic/management/models.py`

 * *Files identical despite different names*

### Comparing `django-typomatic-2.5.0/django_typomatic/mappings.py` & `django_typomatic-2.5.1/django_typomatic/mappings.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,9 +1,11 @@
+import django
 from django.db.models import fields
 from rest_framework import serializers
+from packaging.version import Version
 
 mappings = {
     fields.AutoField: 'number',
     fields.BigAutoField: 'number',
     fields.BigIntegerField : 'number',
     fields.BinaryField: 'string',
     fields.BooleanField: 'boolean',
@@ -15,15 +17,14 @@
     fields.DurationField: 'string',
     fields.EmailField: 'string',
     fields.FilePathField: 'string',
     fields.FloatField: 'number',
     fields.GenericIPAddressField: 'string',
     fields.IPAddressField: 'string',
     fields.IntegerField: 'number',
-    fields.PositiveBigIntegerField: 'number',
     fields.PositiveIntegerField: 'number',
     fields.PositiveSmallIntegerField: 'number',
     fields.SlugField: 'string',
     fields.SmallAutoField: 'number',
     fields.SmallIntegerField: 'number',
     fields.TextField: 'string',
     fields.TimeField: 'string',
@@ -46,14 +47,18 @@
     serializers.DecimalField: 'number',
     serializers.DateTimeField: 'string',
     serializers.DateField: 'string',
     serializers.TimeField: 'string',
     serializers.DurationField: 'string',
 }
 
+# PositiveBigIntegerField was added in Django 3.1
+if Version(django.__version__) >= Version('3.1'):
+    mappings[fields.PositiveBigIntegerField] = 'number'
+
 format_mappings = {
     serializers.EmailField: 'email',
     serializers.URLField: 'url',
     serializers.UUIDField: 'uuid',
     serializers.DateTimeField: 'date-time',
     serializers.DateField: 'date',
     serializers.TimeField: 'time',
```

### Comparing `django-typomatic-2.5.0/django_typomatic/test__init__.py` & `django_typomatic-2.5.1/django_typomatic/test__init__.py`

 * *Files identical despite different names*

### Comparing `django-typomatic-2.5.0/django_typomatic.egg-info/PKG-INFO` & `django_typomatic-2.5.1/django_typomatic.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: django-typomatic
-Version: 2.5.0
+Version: 2.5.1
 Summary: A simple solution for generating Typescript interfaces from your Django Rest Framework Serializers.
 Home-page: https://github.com/adenh93/django-typomatic
 Author: Aden Herold
 Author-email: aden.herold1@gmail.com
 Keywords: Django,Django Rest Framework,DRF,Typescript,Python
 Platform: any
 Description-Content-Type: text/markdown
```

### Comparing `django-typomatic-2.5.0/django_typomatic.egg-info/SOURCES.txt` & `django_typomatic-2.5.1/django_typomatic.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `django-typomatic-2.5.0/setup.py` & `django_typomatic-2.5.1/setup.py`

 * *Files 13% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 import setuptools
 
 with open('README.md') as file:
     long_description = file.read()
 
 setuptools.setup(
     name="django-typomatic",
-    version="2.5.0",
+    version="2.5.1",
     url="https://github.com/adenh93/django-typomatic",
 
     author="Aden Herold",
     author_email="aden.herold1@gmail.com",
 
     description="A simple solution for generating Typescript interfaces from your Django Rest Framework Serializers.",
     long_description=long_description,
```

