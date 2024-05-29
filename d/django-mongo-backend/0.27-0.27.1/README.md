# Comparing `tmp/django_mongo_backend-0.27.tar.gz` & `tmp/django_mongo_backend-0.27.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "django_mongo_backend-0.27.tar", max compression
+gzip compressed data, was "django_mongo_backend-0.27.1.tar", max compression
```

## Comparing `django_mongo_backend-0.27.tar` & `django_mongo_backend-0.27.1.tar`

### file list

```diff
@@ -1,18 +1,18 @@
--rw-r--r--   0        0        0     4713 2024-05-25 18:05:33.977495 django_mongo_backend-0.27/README.md
--rw-r--r--   0        0        0       21 2024-04-07 12:37:19.975612 django_mongo_backend-0.27/django_mongodb/__init__.py
--rw-r--r--   0        0        0     3913 2024-04-07 12:36:45.620893 django_mongo_backend-0.27/django_mongodb/base.py
--rw-r--r--   0        0        0      237 2024-01-21 16:37:33.480045 django_mongo_backend-0.27/django_mongodb/client.py
--rw-r--r--   0        0        0    12524 2024-05-25 18:13:02.316951 django_mongo_backend-0.27/django_mongodb/compiler.py
--rw-r--r--   0        0        0      805 2024-01-21 16:37:33.480477 django_mongo_backend-0.27/django_mongodb/creation.py
--rw-r--r--   0        0        0     3471 2024-04-07 12:37:01.148887 django_mongo_backend-0.27/django_mongodb/cursor.py
--rw-r--r--   0        0        0      404 2024-01-21 16:37:33.481020 django_mongo_backend-0.27/django_mongodb/database.py
--rw-r--r--   0        0        0      387 2024-04-07 12:36:43.559601 django_mongo_backend-0.27/django_mongodb/expressions.py
--rw-r--r--   0        0        0      260 2024-01-21 16:37:33.481154 django_mongo_backend-0.27/django_mongodb/features.py
--rw-r--r--   0        0        0      446 2024-04-07 12:36:46.197955 django_mongo_backend-0.27/django_mongodb/introspection.py
--rw-r--r--   0        0        0     1726 2024-05-25 18:13:02.301189 django_mongo_backend-0.27/django_mongodb/managers.py
--rw-r--r--   0        0        0     1539 2024-04-07 12:36:46.649359 django_mongo_backend-0.27/django_mongodb/models.py
--rw-r--r--   0        0        0     2117 2024-04-07 12:36:46.976913 django_mongo_backend-0.27/django_mongodb/operations.py
--rw-r--r--   0        0        0    15246 2024-05-25 17:34:05.940230 django_mongo_backend-0.27/django_mongodb/query.py
--rw-r--r--   0        0        0     1410 2024-04-07 12:36:47.930848 django_mongo_backend-0.27/django_mongodb/schema.py
--rw-r--r--   0        0        0     1620 2024-05-25 19:20:25.019184 django_mongo_backend-0.27/pyproject.toml
--rw-r--r--   0        0        0     5629 1970-01-01 00:00:00.000000 django_mongo_backend-0.27/PKG-INFO
+-rw-r--r--   0        0        0     4713 2024-05-25 18:05:33.977495 django_mongo_backend-0.27.1/README.md
+-rw-r--r--   0        0        0       21 2024-04-07 12:37:19.975612 django_mongo_backend-0.27.1/django_mongodb/__init__.py
+-rw-r--r--   0        0        0     3913 2024-04-07 12:36:45.620893 django_mongo_backend-0.27.1/django_mongodb/base.py
+-rw-r--r--   0        0        0      237 2024-01-21 16:37:33.480045 django_mongo_backend-0.27.1/django_mongodb/client.py
+-rw-r--r--   0        0        0    12524 2024-05-25 18:13:02.316951 django_mongo_backend-0.27.1/django_mongodb/compiler.py
+-rw-r--r--   0        0        0      805 2024-01-21 16:37:33.480477 django_mongo_backend-0.27.1/django_mongodb/creation.py
+-rw-r--r--   0        0        0     3471 2024-04-07 12:37:01.148887 django_mongo_backend-0.27.1/django_mongodb/cursor.py
+-rw-r--r--   0        0        0      404 2024-01-21 16:37:33.481020 django_mongo_backend-0.27.1/django_mongodb/database.py
+-rw-r--r--   0        0        0      387 2024-04-07 12:36:43.559601 django_mongo_backend-0.27.1/django_mongodb/expressions.py
+-rw-r--r--   0        0        0      300 2024-05-27 19:49:56.692478 django_mongo_backend-0.27.1/django_mongodb/features.py
+-rw-r--r--   0        0        0      446 2024-04-07 12:36:46.197955 django_mongo_backend-0.27.1/django_mongodb/introspection.py
+-rw-r--r--   0        0        0     1726 2024-05-25 18:13:02.301189 django_mongo_backend-0.27.1/django_mongodb/managers.py
+-rw-r--r--   0        0        0     1784 2024-05-29 09:29:13.456701 django_mongo_backend-0.27.1/django_mongodb/models.py
+-rw-r--r--   0        0        0     2117 2024-04-07 12:36:46.976913 django_mongo_backend-0.27.1/django_mongodb/operations.py
+-rw-r--r--   0        0        0    15246 2024-05-25 17:34:05.940230 django_mongo_backend-0.27.1/django_mongodb/query.py
+-rw-r--r--   0        0        0     1410 2024-04-07 12:36:47.930848 django_mongo_backend-0.27.1/django_mongodb/schema.py
+-rw-r--r--   0        0        0     1622 2024-05-29 09:29:48.787175 django_mongo_backend-0.27.1/pyproject.toml
+-rw-r--r--   0        0        0     5631 1970-01-01 00:00:00.000000 django_mongo_backend-0.27.1/PKG-INFO
```

### Comparing `django_mongo_backend-0.27/README.md` & `django_mongo_backend-0.27.1/README.md`

 * *Files identical despite different names*

### Comparing `django_mongo_backend-0.27/django_mongodb/base.py` & `django_mongo_backend-0.27.1/django_mongodb/base.py`

 * *Files identical despite different names*

### Comparing `django_mongo_backend-0.27/django_mongodb/compiler.py` & `django_mongo_backend-0.27.1/django_mongodb/compiler.py`

 * *Files identical despite different names*

### Comparing `django_mongo_backend-0.27/django_mongodb/creation.py` & `django_mongo_backend-0.27.1/django_mongodb/creation.py`

 * *Files identical despite different names*

### Comparing `django_mongo_backend-0.27/django_mongodb/cursor.py` & `django_mongo_backend-0.27.1/django_mongodb/cursor.py`

 * *Files identical despite different names*

### Comparing `django_mongo_backend-0.27/django_mongodb/managers.py` & `django_mongo_backend-0.27.1/django_mongodb/managers.py`

 * *Files identical despite different names*

### Comparing `django_mongo_backend-0.27/django_mongodb/models.py` & `django_mongo_backend-0.27.1/django_mongodb/models.py`

 * *Files 15% similar despite different names*

```diff
@@ -12,34 +12,40 @@
     }
 
     @cached_property
     def validators(self):
         return self._validators
 
     def db_type(self, connection):
-        return "ObjectId"
+        return "ObjectId" if "ObjectIdField" in connection.data_types else "CHAR(24)"
 
     def to_python(self, value):
         if value is None or isinstance(value, bson.ObjectId):
             return value
         else:
             return bson.ObjectId(value)
 
+    def from_db_value(self, value, expression, connection):
+        return self.to_python(value)
+
     def get_prep_value(self, value):
         if value is None:
             return None
         if isinstance(value, str):
             return bson.ObjectId(value)
         return bson.ObjectId(value)
 
+    def get_db_prep_value(self, value, connection, prepared=False):
+        return (
+            self.get_prep_value(value) if "ObjectIdField" in connection.data_types else str(value)
+        )
+
 
 class ObjectIdField(ObjectIdFieldMixin, models.CharField):
-    def __init__(self, *args, **kwargs):
-        kwargs["max_length"] = 24
-        super().__init__(*args, **kwargs)
+    pass
 
 
 class ObjectIdAutoField(ObjectIdFieldMixin, AutoField, metaclass=AutoFieldMeta):
     description = "MongoDB ObjectIdAutoField"
 
     def __init__(self, *args, **kwargs):
         if "db_column" not in kwargs:
```

### Comparing `django_mongo_backend-0.27/django_mongodb/operations.py` & `django_mongo_backend-0.27.1/django_mongodb/operations.py`

 * *Files identical despite different names*

### Comparing `django_mongo_backend-0.27/django_mongodb/query.py` & `django_mongo_backend-0.27.1/django_mongodb/query.py`

 * *Files identical despite different names*

### Comparing `django_mongo_backend-0.27/django_mongodb/schema.py` & `django_mongo_backend-0.27.1/django_mongodb/schema.py`

 * *Files identical despite different names*

### Comparing `django_mongo_backend-0.27/pyproject.toml` & `django_mongo_backend-0.27.1/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -11,15 +11,15 @@
     "Framework :: Django :: 4.0",
     "Framework :: Django :: 4.1",
     "Framework :: Django :: 4.2",
     "Framework :: Django :: 5.0",
     "Intended Audience :: Developers",
     "Operating System :: OS Independent",
 ]
-version = "0.27"
+version = "0.27.1"
 description = ""
 authors = ["gersmann"]
 readme = "README.md"
 homepage = "https://github.com/gersmann/django-mongo-backend"
 repository = "https://github.com/gersmann/django-mongo-backend"
 
 [tool.poetry.dependencies]
```

### Comparing `django_mongo_backend-0.27/PKG-INFO` & `django_mongo_backend-0.27.1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: django-mongo-backend
-Version: 0.27
+Version: 0.27.1
 Summary: 
 Home-page: https://github.com/gersmann/django-mongo-backend
 Keywords: django,mongodb,backend
 Author: gersmann
 Requires-Python: >=3.11,<4.0
 Classifier: Development Status :: 3 - Alpha
 Classifier: Environment :: Web Environment
```

