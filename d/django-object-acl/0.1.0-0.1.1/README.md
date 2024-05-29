# Comparing `tmp/django-object-acl-0.1.0.tar.gz` & `tmp/django-object-acl-0.1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "django-object-acl-0.1.0.tar", max compression
+gzip compressed data, was "django-object-acl-0.1.1.tar", max compression
```

## Comparing `django-object-acl-0.1.0.tar` & `django-object-acl-0.1.1.tar`

### file list

```diff
@@ -1,10 +1,11 @@
--rw-r--r--   0        0        0        0 2024-05-28 07:29:16.425270 django-object-acl-0.1.0/django_object_acl/__init__.py
--rw-r--r--   0        0        0      107 2024-05-28 07:29:16.425414 django-object-acl-0.1.0/django_object_acl/apps.py
--rw-r--r--   0        0        0     5349 2024-05-29 09:34:04.849021 django-object-acl-0.1.0/django_object_acl/managers.py
--rw-r--r--   0        0        0     3195 2024-05-28 17:44:54.399861 django-object-acl-0.1.0/django_object_acl/migrations/0001_initial.py
--rw-r--r--   0        0        0        0 2024-05-28 07:29:16.425753 django-object-acl-0.1.0/django_object_acl/migrations/__init__.py
--rw-r--r--   0        0        0     2908 2024-05-28 17:46:27.297581 django-object-acl-0.1.0/django_object_acl/mixins.py
--rw-r--r--   0        0        0     2074 2024-05-28 17:47:31.137910 django-object-acl-0.1.0/django_object_acl/models.py
--rw-r--r--   0        0        0      593 2024-05-28 10:35:48.478592 django-object-acl-0.1.0/pyproject.toml
--rw-r--r--   0        0        0      696 2024-05-29 12:32:34.529677 django-object-acl-0.1.0/setup.py
--rw-r--r--   0        0        0      353 2024-05-29 12:32:34.529872 django-object-acl-0.1.0/PKG-INFO
+-rw-r--r--   0        0        0    10757 2024-05-29 12:31:23.353710 django-object-acl-0.1.1/README.md
+-rw-r--r--   0        0        0        0 2024-05-28 07:29:16.425270 django-object-acl-0.1.1/django_object_acl/__init__.py
+-rw-r--r--   0        0        0      107 2024-05-28 07:29:16.425414 django-object-acl-0.1.1/django_object_acl/apps.py
+-rw-r--r--   0        0        0     5349 2024-05-29 09:34:04.849021 django-object-acl-0.1.1/django_object_acl/managers.py
+-rw-r--r--   0        0        0     3195 2024-05-28 17:44:54.399861 django-object-acl-0.1.1/django_object_acl/migrations/0001_initial.py
+-rw-r--r--   0        0        0        0 2024-05-28 07:29:16.425753 django-object-acl-0.1.1/django_object_acl/migrations/__init__.py
+-rw-r--r--   0        0        0     2908 2024-05-28 17:46:27.297581 django-object-acl-0.1.1/django_object_acl/mixins.py
+-rw-r--r--   0        0        0     2074 2024-05-28 17:47:31.137910 django-object-acl-0.1.1/django_object_acl/models.py
+-rw-r--r--   0        0        0      614 2024-05-29 13:11:07.431998 django-object-acl-0.1.1/pyproject.toml
+-rw-r--r--   0        0        0    11714 2024-05-29 13:11:17.299613 django-object-acl-0.1.1/setup.py
+-rw-r--r--   0        0        0    11152 2024-05-29 13:11:17.300243 django-object-acl-0.1.1/PKG-INFO
```

### Comparing `django-object-acl-0.1.0/django_object_acl/managers.py` & `django-object-acl-0.1.1/django_object_acl/managers.py`

 * *Files identical despite different names*

### Comparing `django-object-acl-0.1.0/django_object_acl/migrations/0001_initial.py` & `django-object-acl-0.1.1/django_object_acl/migrations/0001_initial.py`

 * *Files identical despite different names*

### Comparing `django-object-acl-0.1.0/django_object_acl/mixins.py` & `django-object-acl-0.1.1/django_object_acl/mixins.py`

 * *Files identical despite different names*

### Comparing `django-object-acl-0.1.0/django_object_acl/models.py` & `django-object-acl-0.1.1/django_object_acl/models.py`

 * *Files identical despite different names*

### Comparing `django-object-acl-0.1.0/pyproject.toml` & `django-object-acl-0.1.1/pyproject.toml`

 * *Files 24% similar despite different names*

```diff
@@ -1,11 +1,12 @@
 [tool.poetry]
 name = "django-object-acl"
-version = "0.1.0"
+version = "0.1.1"
 description = "Adds object level permission for your models"
+readme = "README.md"
 authors = [
     "Noam Ben-Yechiel <nbenyechiel@twistbioscience.com>",
     "Simon Nizov <simon.nizov@gmail.com>",
 ]
 
 [tool.poetry.dependencies]
 python = "^3.10"
```

