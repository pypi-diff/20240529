# Comparing `tmp/transparent_classroom-0.0.1.tar.gz` & `tmp/transparent_classroom-0.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/transparent_classroom-0.0.1.tar", last modified: Sun May 19 05:54:52 2024, max compression
+gzip compressed data, was "dist/transparent_classroom-0.0.2.tar", last modified: Wed May 29 03:46:45 2024, max compression
```

## Comparing `transparent_classroom-0.0.1.tar` & `transparent_classroom-0.0.2.tar`

### file list

```diff
@@ -1,50 +1,50 @@
-drwxr-xr-x   0 dpozorski   (501) staff       (20)        0 2024-05-19 05:54:52.000000 transparent_classroom-0.0.1/
--rw-r--r--   0 dpozorski   (501) staff       (20)      486 2024-05-19 05:54:52.000000 transparent_classroom-0.0.1/PKG-INFO
--rw-r--r--   0 dpozorski   (501) staff       (20)     9689 2024-05-19 04:29:43.000000 transparent_classroom-0.0.1/README.md
--rw-r--r--   0 dpozorski   (501) staff       (20)       38 2024-05-19 05:54:52.000000 transparent_classroom-0.0.1/setup.cfg
--rw-r--r--   0 dpozorski   (501) staff       (20)      657 2024-05-19 05:41:08.000000 transparent_classroom-0.0.1/setup.py
-drwxr-xr-x   0 dpozorski   (501) staff       (20)        0 2024-05-19 05:54:52.000000 transparent_classroom-0.0.1/transparent_classroom/
--rw-r--r--   0 dpozorski   (501) staff       (20)        0 2024-01-07 22:51:24.000000 transparent_classroom-0.0.1/transparent_classroom/__init__.py
-drwxr-xr-x   0 dpozorski   (501) staff       (20)        0 2024-05-19 05:54:52.000000 transparent_classroom-0.0.1/transparent_classroom/api/
--rw-r--r--   0 dpozorski   (501) staff       (20)     3719 2024-05-18 18:31:58.000000 transparent_classroom-0.0.1/transparent_classroom/api/__init__.py
-drwxr-xr-x   0 dpozorski   (501) staff       (20)        0 2024-05-19 05:54:52.000000 transparent_classroom-0.0.1/transparent_classroom/api/entry_points/
--rw-r--r--   0 dpozorski   (501) staff       (20)     2460 2024-01-15 22:49:46.000000 transparent_classroom-0.0.1/transparent_classroom/api/entry_points/__init__.py
-drwxr-xr-x   0 dpozorski   (501) staff       (20)        0 2024-05-19 05:54:52.000000 transparent_classroom-0.0.1/transparent_classroom/api/enums/
--rw-r--r--   0 dpozorski   (501) staff       (20)     5327 2024-05-18 18:31:58.000000 transparent_classroom-0.0.1/transparent_classroom/api/enums/__init__.py
-drwxr-xr-x   0 dpozorski   (501) staff       (20)        0 2024-05-19 05:54:52.000000 transparent_classroom-0.0.1/transparent_classroom/api/exceptions/
--rw-r--r--   0 dpozorski   (501) staff       (20)     1268 2024-05-18 18:31:58.000000 transparent_classroom-0.0.1/transparent_classroom/api/exceptions/__init__.py
-drwxr-xr-x   0 dpozorski   (501) staff       (20)        0 2024-05-19 05:54:52.000000 transparent_classroom-0.0.1/transparent_classroom/api/interfaces/
--rw-r--r--   0 dpozorski   (501) staff       (20)     5365 2024-05-18 18:31:58.000000 transparent_classroom-0.0.1/transparent_classroom/api/interfaces/__init__.py
-drwxr-xr-x   0 dpozorski   (501) staff       (20)        0 2024-05-19 05:54:52.000000 transparent_classroom-0.0.1/transparent_classroom/api/interfaces/fields/
--rw-r--r--   0 dpozorski   (501) staff       (20)    23792 2024-05-18 18:31:58.000000 transparent_classroom-0.0.1/transparent_classroom/api/interfaces/fields/__init__.py
-drwxr-xr-x   0 dpozorski   (501) staff       (20)        0 2024-05-19 05:54:52.000000 transparent_classroom-0.0.1/transparent_classroom/api/interfaces/fields/exceptions/
--rw-r--r--   0 dpozorski   (501) staff       (20)      577 2024-01-15 21:55:58.000000 transparent_classroom-0.0.1/transparent_classroom/api/interfaces/fields/exceptions/__init__.py
-drwxr-xr-x   0 dpozorski   (501) staff       (20)        0 2024-05-19 05:54:52.000000 transparent_classroom-0.0.1/transparent_classroom/api/interfaces/validators/
--rw-r--r--   0 dpozorski   (501) staff       (20)     5740 2024-05-18 18:31:58.000000 transparent_classroom-0.0.1/transparent_classroom/api/interfaces/validators/__init__.py
-drwxr-xr-x   0 dpozorski   (501) staff       (20)        0 2024-05-19 05:54:52.000000 transparent_classroom-0.0.1/transparent_classroom/api/interfaces/validators/constraints/
--rw-r--r--   0 dpozorski   (501) staff       (20)    24085 2024-05-18 18:31:58.000000 transparent_classroom-0.0.1/transparent_classroom/api/interfaces/validators/constraints/__init__.py
-drwxr-xr-x   0 dpozorski   (501) staff       (20)        0 2024-05-19 05:54:52.000000 transparent_classroom-0.0.1/transparent_classroom/api/interfaces/validators/exceptions/
--rw-r--r--   0 dpozorski   (501) staff       (20)     5674 2024-05-18 18:31:58.000000 transparent_classroom-0.0.1/transparent_classroom/api/interfaces/validators/exceptions/__init__.py
-drwxr-xr-x   0 dpozorski   (501) staff       (20)        0 2024-05-19 05:54:52.000000 transparent_classroom-0.0.1/transparent_classroom/api/routing/
--rw-r--r--   0 dpozorski   (501) staff       (20)        0 2024-01-09 05:59:42.000000 transparent_classroom-0.0.1/transparent_classroom/api/routing/__init__.py
-drwxr-xr-x   0 dpozorski   (501) staff       (20)        0 2024-05-19 05:54:52.000000 transparent_classroom-0.0.1/transparent_classroom/api/routing/routes/
--rw-r--r--   0 dpozorski   (501) staff       (20)     5869 2024-05-18 18:31:58.000000 transparent_classroom-0.0.1/transparent_classroom/api/routing/routes/__init__.py
--rw-r--r--   0 dpozorski   (501) staff       (20)     1220 2024-01-11 06:19:09.000000 transparent_classroom-0.0.1/transparent_classroom/apis.py
--rw-r--r--   0 dpozorski   (501) staff       (20)    30267 2024-05-19 04:02:37.000000 transparent_classroom-0.0.1/transparent_classroom/clients.py
--rw-r--r--   0 dpozorski   (501) staff       (20)     4798 2024-05-18 18:31:58.000000 transparent_classroom-0.0.1/transparent_classroom/entry_points.py
--rw-r--r--   0 dpozorski   (501) staff       (20)     9510 2024-05-18 18:31:58.000000 transparent_classroom-0.0.1/transparent_classroom/interfaces.py
-drwxr-xr-x   0 dpozorski   (501) staff       (20)        0 2024-05-19 05:54:52.000000 transparent_classroom-0.0.1/transparent_classroom/models/
--rw-r--r--   0 dpozorski   (501) staff       (20)    99532 2024-05-18 18:31:58.000000 transparent_classroom-0.0.1/transparent_classroom/models/__init__.py
-drwxr-xr-x   0 dpozorski   (501) staff       (20)        0 2024-05-19 05:54:52.000000 transparent_classroom-0.0.1/transparent_classroom/models/deserializers/
--rw-r--r--   0 dpozorski   (501) staff       (20)    14177 2024-05-18 18:31:58.000000 transparent_classroom-0.0.1/transparent_classroom/models/deserializers/__init__.py
-drwxr-xr-x   0 dpozorski   (501) staff       (20)        0 2024-05-19 05:54:52.000000 transparent_classroom-0.0.1/transparent_classroom/models/serializers/
--rw-r--r--   0 dpozorski   (501) staff       (20)     4645 2024-05-18 18:31:58.000000 transparent_classroom-0.0.1/transparent_classroom/models/serializers/__init__.py
--rw-r--r--   0 dpozorski   (501) staff       (20)     4077 2024-05-18 18:31:58.000000 transparent_classroom-0.0.1/transparent_classroom/models/utilities.py
--rw-r--r--   0 dpozorski   (501) staff       (20)      669 2024-01-15 07:33:12.000000 transparent_classroom-0.0.1/transparent_classroom/route_components.py
--rw-r--r--   0 dpozorski   (501) staff       (20)     3646 2024-05-18 18:31:58.000000 transparent_classroom-0.0.1/transparent_classroom/routes.py
-drwxr-xr-x   0 dpozorski   (501) staff       (20)        0 2024-05-19 05:54:52.000000 transparent_classroom-0.0.1/transparent_classroom.egg-info/
--rw-r--r--   0 dpozorski   (501) staff       (20)      486 2024-05-19 05:54:52.000000 transparent_classroom-0.0.1/transparent_classroom.egg-info/PKG-INFO
--rw-r--r--   0 dpozorski   (501) staff       (20)     1334 2024-05-19 05:54:52.000000 transparent_classroom-0.0.1/transparent_classroom.egg-info/SOURCES.txt
--rw-r--r--   0 dpozorski   (501) staff       (20)        1 2024-05-19 05:54:52.000000 transparent_classroom-0.0.1/transparent_classroom.egg-info/dependency_links.txt
--rw-r--r--   0 dpozorski   (501) staff       (20)       25 2024-05-19 05:54:52.000000 transparent_classroom-0.0.1/transparent_classroom.egg-info/requires.txt
--rw-r--r--   0 dpozorski   (501) staff       (20)       22 2024-05-19 05:54:52.000000 transparent_classroom-0.0.1/transparent_classroom.egg-info/top_level.txt
+drwxr-xr-x   0 dpozorski   (501) staff       (20)        0 2024-05-29 03:46:45.000000 transparent_classroom-0.0.2/
+-rw-r--r--   0 dpozorski   (501) staff       (20)      486 2024-05-29 03:46:45.000000 transparent_classroom-0.0.2/PKG-INFO
+-rw-r--r--   0 dpozorski   (501) staff       (20)     9689 2024-05-19 04:29:43.000000 transparent_classroom-0.0.2/README.md
+-rw-r--r--   0 dpozorski   (501) staff       (20)       38 2024-05-29 03:46:45.000000 transparent_classroom-0.0.2/setup.cfg
+-rw-r--r--   0 dpozorski   (501) staff       (20)      657 2024-05-29 03:43:07.000000 transparent_classroom-0.0.2/setup.py
+drwxr-xr-x   0 dpozorski   (501) staff       (20)        0 2024-05-29 03:46:45.000000 transparent_classroom-0.0.2/transparent_classroom/
+-rw-r--r--   0 dpozorski   (501) staff       (20)        0 2024-01-07 22:51:24.000000 transparent_classroom-0.0.2/transparent_classroom/__init__.py
+drwxr-xr-x   0 dpozorski   (501) staff       (20)        0 2024-05-29 03:46:45.000000 transparent_classroom-0.0.2/transparent_classroom/api/
+-rw-r--r--   0 dpozorski   (501) staff       (20)     3719 2024-05-18 18:31:58.000000 transparent_classroom-0.0.2/transparent_classroom/api/__init__.py
+drwxr-xr-x   0 dpozorski   (501) staff       (20)        0 2024-05-29 03:46:45.000000 transparent_classroom-0.0.2/transparent_classroom/api/entry_points/
+-rw-r--r--   0 dpozorski   (501) staff       (20)     2460 2024-01-15 22:49:46.000000 transparent_classroom-0.0.2/transparent_classroom/api/entry_points/__init__.py
+drwxr-xr-x   0 dpozorski   (501) staff       (20)        0 2024-05-29 03:46:45.000000 transparent_classroom-0.0.2/transparent_classroom/api/enums/
+-rw-r--r--   0 dpozorski   (501) staff       (20)     5327 2024-05-18 18:31:58.000000 transparent_classroom-0.0.2/transparent_classroom/api/enums/__init__.py
+drwxr-xr-x   0 dpozorski   (501) staff       (20)        0 2024-05-29 03:46:45.000000 transparent_classroom-0.0.2/transparent_classroom/api/exceptions/
+-rw-r--r--   0 dpozorski   (501) staff       (20)     1268 2024-05-18 18:31:58.000000 transparent_classroom-0.0.2/transparent_classroom/api/exceptions/__init__.py
+drwxr-xr-x   0 dpozorski   (501) staff       (20)        0 2024-05-29 03:46:45.000000 transparent_classroom-0.0.2/transparent_classroom/api/interfaces/
+-rw-r--r--   0 dpozorski   (501) staff       (20)     5365 2024-05-18 18:31:58.000000 transparent_classroom-0.0.2/transparent_classroom/api/interfaces/__init__.py
+drwxr-xr-x   0 dpozorski   (501) staff       (20)        0 2024-05-29 03:46:45.000000 transparent_classroom-0.0.2/transparent_classroom/api/interfaces/fields/
+-rw-r--r--   0 dpozorski   (501) staff       (20)    23792 2024-05-18 18:31:58.000000 transparent_classroom-0.0.2/transparent_classroom/api/interfaces/fields/__init__.py
+drwxr-xr-x   0 dpozorski   (501) staff       (20)        0 2024-05-29 03:46:45.000000 transparent_classroom-0.0.2/transparent_classroom/api/interfaces/fields/exceptions/
+-rw-r--r--   0 dpozorski   (501) staff       (20)      577 2024-01-15 21:55:58.000000 transparent_classroom-0.0.2/transparent_classroom/api/interfaces/fields/exceptions/__init__.py
+drwxr-xr-x   0 dpozorski   (501) staff       (20)        0 2024-05-29 03:46:45.000000 transparent_classroom-0.0.2/transparent_classroom/api/interfaces/validators/
+-rw-r--r--   0 dpozorski   (501) staff       (20)     5740 2024-05-18 18:31:58.000000 transparent_classroom-0.0.2/transparent_classroom/api/interfaces/validators/__init__.py
+drwxr-xr-x   0 dpozorski   (501) staff       (20)        0 2024-05-29 03:46:45.000000 transparent_classroom-0.0.2/transparent_classroom/api/interfaces/validators/constraints/
+-rw-r--r--   0 dpozorski   (501) staff       (20)    24085 2024-05-18 18:31:58.000000 transparent_classroom-0.0.2/transparent_classroom/api/interfaces/validators/constraints/__init__.py
+drwxr-xr-x   0 dpozorski   (501) staff       (20)        0 2024-05-29 03:46:45.000000 transparent_classroom-0.0.2/transparent_classroom/api/interfaces/validators/exceptions/
+-rw-r--r--   0 dpozorski   (501) staff       (20)     5674 2024-05-18 18:31:58.000000 transparent_classroom-0.0.2/transparent_classroom/api/interfaces/validators/exceptions/__init__.py
+drwxr-xr-x   0 dpozorski   (501) staff       (20)        0 2024-05-29 03:46:45.000000 transparent_classroom-0.0.2/transparent_classroom/api/routing/
+-rw-r--r--   0 dpozorski   (501) staff       (20)        0 2024-01-09 05:59:42.000000 transparent_classroom-0.0.2/transparent_classroom/api/routing/__init__.py
+drwxr-xr-x   0 dpozorski   (501) staff       (20)        0 2024-05-29 03:46:45.000000 transparent_classroom-0.0.2/transparent_classroom/api/routing/routes/
+-rw-r--r--   0 dpozorski   (501) staff       (20)     5869 2024-05-18 18:31:58.000000 transparent_classroom-0.0.2/transparent_classroom/api/routing/routes/__init__.py
+-rw-r--r--   0 dpozorski   (501) staff       (20)     1220 2024-01-11 06:19:09.000000 transparent_classroom-0.0.2/transparent_classroom/apis.py
+-rw-r--r--   0 dpozorski   (501) staff       (20)    30266 2024-05-29 03:43:07.000000 transparent_classroom-0.0.2/transparent_classroom/clients.py
+-rw-r--r--   0 dpozorski   (501) staff       (20)     4798 2024-05-18 18:31:58.000000 transparent_classroom-0.0.2/transparent_classroom/entry_points.py
+-rw-r--r--   0 dpozorski   (501) staff       (20)     9510 2024-05-18 18:31:58.000000 transparent_classroom-0.0.2/transparent_classroom/interfaces.py
+drwxr-xr-x   0 dpozorski   (501) staff       (20)        0 2024-05-29 03:46:45.000000 transparent_classroom-0.0.2/transparent_classroom/models/
+-rw-r--r--   0 dpozorski   (501) staff       (20)    99532 2024-05-18 18:31:58.000000 transparent_classroom-0.0.2/transparent_classroom/models/__init__.py
+drwxr-xr-x   0 dpozorski   (501) staff       (20)        0 2024-05-29 03:46:45.000000 transparent_classroom-0.0.2/transparent_classroom/models/deserializers/
+-rw-r--r--   0 dpozorski   (501) staff       (20)    14177 2024-05-18 18:31:58.000000 transparent_classroom-0.0.2/transparent_classroom/models/deserializers/__init__.py
+drwxr-xr-x   0 dpozorski   (501) staff       (20)        0 2024-05-29 03:46:45.000000 transparent_classroom-0.0.2/transparent_classroom/models/serializers/
+-rw-r--r--   0 dpozorski   (501) staff       (20)     4645 2024-05-18 18:31:58.000000 transparent_classroom-0.0.2/transparent_classroom/models/serializers/__init__.py
+-rw-r--r--   0 dpozorski   (501) staff       (20)     4077 2024-05-18 18:31:58.000000 transparent_classroom-0.0.2/transparent_classroom/models/utilities.py
+-rw-r--r--   0 dpozorski   (501) staff       (20)      669 2024-01-15 07:33:12.000000 transparent_classroom-0.0.2/transparent_classroom/route_components.py
+-rw-r--r--   0 dpozorski   (501) staff       (20)     3646 2024-05-18 18:31:58.000000 transparent_classroom-0.0.2/transparent_classroom/routes.py
+drwxr-xr-x   0 dpozorski   (501) staff       (20)        0 2024-05-29 03:46:45.000000 transparent_classroom-0.0.2/transparent_classroom.egg-info/
+-rw-r--r--   0 dpozorski   (501) staff       (20)      486 2024-05-29 03:46:45.000000 transparent_classroom-0.0.2/transparent_classroom.egg-info/PKG-INFO
+-rw-r--r--   0 dpozorski   (501) staff       (20)     1334 2024-05-29 03:46:45.000000 transparent_classroom-0.0.2/transparent_classroom.egg-info/SOURCES.txt
+-rw-r--r--   0 dpozorski   (501) staff       (20)        1 2024-05-29 03:46:45.000000 transparent_classroom-0.0.2/transparent_classroom.egg-info/dependency_links.txt
+-rw-r--r--   0 dpozorski   (501) staff       (20)       25 2024-05-29 03:46:45.000000 transparent_classroom-0.0.2/transparent_classroom.egg-info/requires.txt
+-rw-r--r--   0 dpozorski   (501) staff       (20)       22 2024-05-29 03:46:45.000000 transparent_classroom-0.0.2/transparent_classroom.egg-info/top_level.txt
```

### Comparing `transparent_classroom-0.0.1/README.md` & `transparent_classroom-0.0.2/README.md`

 * *Files identical despite different names*

### Comparing `transparent_classroom-0.0.1/setup.py` & `transparent_classroom-0.0.2/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from setuptools import setup, find_packages
 
 setup(
     name='transparent_classroom',
-    version='0.0.1',
+    version='0.0.2',
     author='Dylan Pozorski',
     author_email='dylanpozorski@gmail.com',
     url='https://github.com/dpozorski/transparent-classroom',
     description="Python Client for accessing Transparent Classroom's data model.",
     packages=find_packages(exclude=['tests']),
     classifiers=[
         'Programming Language :: Python :: 3',
```

### Comparing `transparent_classroom-0.0.1/transparent_classroom/api/__init__.py` & `transparent_classroom-0.0.2/transparent_classroom/api/__init__.py`

 * *Files identical despite different names*

### Comparing `transparent_classroom-0.0.1/transparent_classroom/api/entry_points/__init__.py` & `transparent_classroom-0.0.2/transparent_classroom/api/entry_points/__init__.py`

 * *Files identical despite different names*

### Comparing `transparent_classroom-0.0.1/transparent_classroom/api/enums/__init__.py` & `transparent_classroom-0.0.2/transparent_classroom/api/enums/__init__.py`

 * *Files identical despite different names*

### Comparing `transparent_classroom-0.0.1/transparent_classroom/api/exceptions/__init__.py` & `transparent_classroom-0.0.2/transparent_classroom/api/exceptions/__init__.py`

 * *Files identical despite different names*

### Comparing `transparent_classroom-0.0.1/transparent_classroom/api/interfaces/__init__.py` & `transparent_classroom-0.0.2/transparent_classroom/api/interfaces/__init__.py`

 * *Files identical despite different names*

### Comparing `transparent_classroom-0.0.1/transparent_classroom/api/interfaces/fields/__init__.py` & `transparent_classroom-0.0.2/transparent_classroom/api/interfaces/fields/__init__.py`

 * *Files identical despite different names*

### Comparing `transparent_classroom-0.0.1/transparent_classroom/api/interfaces/fields/exceptions/__init__.py` & `transparent_classroom-0.0.2/transparent_classroom/api/interfaces/fields/exceptions/__init__.py`

 * *Files identical despite different names*

### Comparing `transparent_classroom-0.0.1/transparent_classroom/api/interfaces/validators/__init__.py` & `transparent_classroom-0.0.2/transparent_classroom/api/interfaces/validators/__init__.py`

 * *Files identical despite different names*

### Comparing `transparent_classroom-0.0.1/transparent_classroom/api/interfaces/validators/constraints/__init__.py` & `transparent_classroom-0.0.2/transparent_classroom/api/interfaces/validators/constraints/__init__.py`

 * *Files identical despite different names*

### Comparing `transparent_classroom-0.0.1/transparent_classroom/api/interfaces/validators/exceptions/__init__.py` & `transparent_classroom-0.0.2/transparent_classroom/api/interfaces/validators/exceptions/__init__.py`

 * *Files identical despite different names*

### Comparing `transparent_classroom-0.0.1/transparent_classroom/api/routing/routes/__init__.py` & `transparent_classroom-0.0.2/transparent_classroom/api/routing/routes/__init__.py`

 * *Files identical despite different names*

### Comparing `transparent_classroom-0.0.1/transparent_classroom/apis.py` & `transparent_classroom-0.0.2/transparent_classroom/apis.py`

 * *Files identical despite different names*

### Comparing `transparent_classroom-0.0.1/transparent_classroom/clients.py` & `transparent_classroom-0.0.2/transparent_classroom/clients.py`

 * *Files 1% similar despite different names*

```diff
@@ -427,15 +427,15 @@
                     "child_id": child_id,
                     "date_start": convert_date(date_str=start_date),
                     "date_end": convert_date(date_str=end_date)
                 },
                 "route_parameters": {}
             },
             deserializer=deserializers.EventDeserializer(),
-            paginated=False
+            paginated=True
         )
 
     def get_form(self, form_id: int) -> models.Form:
         """
         Get the specified form instance's response data (i.e. an individual response
         to a form template).
```

### Comparing `transparent_classroom-0.0.1/transparent_classroom/entry_points.py` & `transparent_classroom-0.0.2/transparent_classroom/entry_points.py`

 * *Files identical despite different names*

### Comparing `transparent_classroom-0.0.1/transparent_classroom/interfaces.py` & `transparent_classroom-0.0.2/transparent_classroom/interfaces.py`

 * *Files identical despite different names*

### Comparing `transparent_classroom-0.0.1/transparent_classroom/models/__init__.py` & `transparent_classroom-0.0.2/transparent_classroom/models/__init__.py`

 * *Files identical despite different names*

### Comparing `transparent_classroom-0.0.1/transparent_classroom/models/deserializers/__init__.py` & `transparent_classroom-0.0.2/transparent_classroom/models/deserializers/__init__.py`

 * *Files identical despite different names*

### Comparing `transparent_classroom-0.0.1/transparent_classroom/models/serializers/__init__.py` & `transparent_classroom-0.0.2/transparent_classroom/models/serializers/__init__.py`

 * *Files identical despite different names*

### Comparing `transparent_classroom-0.0.1/transparent_classroom/models/utilities.py` & `transparent_classroom-0.0.2/transparent_classroom/models/utilities.py`

 * *Files identical despite different names*

### Comparing `transparent_classroom-0.0.1/transparent_classroom/route_components.py` & `transparent_classroom-0.0.2/transparent_classroom/route_components.py`

 * *Files identical despite different names*

### Comparing `transparent_classroom-0.0.1/transparent_classroom/routes.py` & `transparent_classroom-0.0.2/transparent_classroom/routes.py`

 * *Files identical despite different names*

### Comparing `transparent_classroom-0.0.1/transparent_classroom.egg-info/SOURCES.txt` & `transparent_classroom-0.0.2/transparent_classroom.egg-info/SOURCES.txt`

 * *Files identical despite different names*

