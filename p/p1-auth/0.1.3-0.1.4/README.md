# Comparing `tmp/p1_auth-0.1.3.tar.gz` & `tmp/p1_auth-0.1.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "p1_auth-0.1.3.tar", last modified: Mon May 20 20:12:16 2024, max compression
+gzip compressed data, was "p1_auth-0.1.4.tar", last modified: Wed May 29 15:20:32 2024, max compression
```

## Comparing `p1_auth-0.1.3.tar` & `p1_auth-0.1.4.tar`

### file list

```diff
@@ -1,23 +1,23 @@
-drwxr-xr-x   0 jametobin   (502) staff       (20)        0 2024-05-20 20:12:16.008617 p1_auth-0.1.3/
--rw-r--r--   0 jametobin   (502) staff       (20)     5620 2024-05-20 20:12:16.008454 p1_auth-0.1.3/PKG-INFO
--rw-r--r--   0 jametobin   (502) staff       (20)     4644 2024-05-20 20:11:59.000000 p1_auth-0.1.3/README.md
-drwxr-xr-x   0 jametobin   (502) staff       (20)        0 2024-05-20 20:12:16.003877 p1_auth-0.1.3/p1_auth/
--rw-r--r--   0 jametobin   (502) staff       (20)        0 2024-05-15 15:17:01.000000 p1_auth-0.1.3/p1_auth/__init__.py
--rw-r--r--   0 jametobin   (502) staff       (20)      849 2024-05-15 15:17:01.000000 p1_auth-0.1.3/p1_auth/admin.py
--rw-r--r--   0 jametobin   (502) staff       (20)      145 2024-05-15 15:17:01.000000 p1_auth-0.1.3/p1_auth/apps.py
--rw-r--r--   0 jametobin   (502) staff       (20)     5708 2024-05-20 20:11:07.000000 p1_auth-0.1.3/p1_auth/backends.py
--rw-r--r--   0 jametobin   (502) staff       (20)      460 2024-05-15 15:17:01.000000 p1_auth-0.1.3/p1_auth/middleware.py
-drwxr-xr-x   0 jametobin   (502) staff       (20)        0 2024-05-20 20:12:16.007542 p1_auth-0.1.3/p1_auth/migrations/
--rw-r--r--   0 jametobin   (502) staff       (20)     1250 2024-05-15 15:17:01.000000 p1_auth-0.1.3/p1_auth/migrations/0001_initial.py
--rw-r--r--   0 jametobin   (502) staff       (20)        0 2024-05-15 15:17:01.000000 p1_auth-0.1.3/p1_auth/migrations/__init__.py
--rw-r--r--   0 jametobin   (502) staff       (20)     3599 2024-05-15 15:17:01.000000 p1_auth-0.1.3/p1_auth/models.py
--rw-r--r--   0 jametobin   (502) staff       (20)       60 2024-05-15 15:17:01.000000 p1_auth-0.1.3/p1_auth/tests.py
--rw-r--r--   0 jametobin   (502) staff       (20)      613 2024-05-15 15:17:01.000000 p1_auth-0.1.3/p1_auth/views.py
-drwxr-xr-x   0 jametobin   (502) staff       (20)        0 2024-05-20 20:12:16.007898 p1_auth-0.1.3/p1_auth.egg-info/
--rw-r--r--   0 jametobin   (502) staff       (20)     5620 2024-05-20 20:12:15.000000 p1_auth-0.1.3/p1_auth.egg-info/PKG-INFO
--rw-r--r--   0 jametobin   (502) staff       (20)      395 2024-05-20 20:12:15.000000 p1_auth-0.1.3/p1_auth.egg-info/SOURCES.txt
--rw-r--r--   0 jametobin   (502) staff       (20)        1 2024-05-20 20:12:15.000000 p1_auth-0.1.3/p1_auth.egg-info/dependency_links.txt
--rw-r--r--   0 jametobin   (502) staff       (20)       41 2024-05-20 20:12:15.000000 p1_auth-0.1.3/p1_auth.egg-info/requires.txt
--rw-r--r--   0 jametobin   (502) staff       (20)        8 2024-05-20 20:12:15.000000 p1_auth-0.1.3/p1_auth.egg-info/top_level.txt
--rw-r--r--   0 jametobin   (502) staff       (20)     1053 2024-05-20 20:12:16.009141 p1_auth-0.1.3/setup.cfg
--rw-r--r--   0 jametobin   (502) staff       (20)       95 2024-05-15 15:17:01.000000 p1_auth-0.1.3/setup.py
+drwxr-xr-x   0 jametobin   (502) staff       (20)        0 2024-05-29 15:20:32.112461 p1_auth-0.1.4/
+-rw-r--r--   0 jametobin   (502) staff       (20)     5823 2024-05-29 15:20:32.112145 p1_auth-0.1.4/PKG-INFO
+-rw-r--r--   0 jametobin   (502) staff       (20)     4847 2024-05-29 15:19:19.000000 p1_auth-0.1.4/README.md
+drwxr-xr-x   0 jametobin   (502) staff       (20)        0 2024-05-29 15:20:32.107555 p1_auth-0.1.4/p1_auth/
+-rw-r--r--   0 jametobin   (502) staff       (20)        0 2024-05-15 15:17:01.000000 p1_auth-0.1.4/p1_auth/__init__.py
+-rw-r--r--   0 jametobin   (502) staff       (20)      849 2024-05-15 15:17:01.000000 p1_auth-0.1.4/p1_auth/admin.py
+-rw-r--r--   0 jametobin   (502) staff       (20)      145 2024-05-15 15:17:01.000000 p1_auth-0.1.4/p1_auth/apps.py
+-rw-r--r--   0 jametobin   (502) staff       (20)     5820 2024-05-29 15:12:15.000000 p1_auth-0.1.4/p1_auth/backends.py
+-rw-r--r--   0 jametobin   (502) staff       (20)      460 2024-05-15 15:17:01.000000 p1_auth-0.1.4/p1_auth/middleware.py
+drwxr-xr-x   0 jametobin   (502) staff       (20)        0 2024-05-29 15:20:32.111340 p1_auth-0.1.4/p1_auth/migrations/
+-rw-r--r--   0 jametobin   (502) staff       (20)     1250 2024-05-15 15:17:01.000000 p1_auth-0.1.4/p1_auth/migrations/0001_initial.py
+-rw-r--r--   0 jametobin   (502) staff       (20)        0 2024-05-15 15:17:01.000000 p1_auth-0.1.4/p1_auth/migrations/__init__.py
+-rw-r--r--   0 jametobin   (502) staff       (20)     3599 2024-05-15 15:17:01.000000 p1_auth-0.1.4/p1_auth/models.py
+-rw-r--r--   0 jametobin   (502) staff       (20)       60 2024-05-15 15:17:01.000000 p1_auth-0.1.4/p1_auth/tests.py
+-rw-r--r--   0 jametobin   (502) staff       (20)      613 2024-05-15 15:17:01.000000 p1_auth-0.1.4/p1_auth/views.py
+drwxr-xr-x   0 jametobin   (502) staff       (20)        0 2024-05-29 15:20:32.111692 p1_auth-0.1.4/p1_auth.egg-info/
+-rw-r--r--   0 jametobin   (502) staff       (20)     5823 2024-05-29 15:20:32.000000 p1_auth-0.1.4/p1_auth.egg-info/PKG-INFO
+-rw-r--r--   0 jametobin   (502) staff       (20)      395 2024-05-29 15:20:32.000000 p1_auth-0.1.4/p1_auth.egg-info/SOURCES.txt
+-rw-r--r--   0 jametobin   (502) staff       (20)        1 2024-05-29 15:20:32.000000 p1_auth-0.1.4/p1_auth.egg-info/dependency_links.txt
+-rw-r--r--   0 jametobin   (502) staff       (20)       41 2024-05-29 15:20:32.000000 p1_auth-0.1.4/p1_auth.egg-info/requires.txt
+-rw-r--r--   0 jametobin   (502) staff       (20)        8 2024-05-29 15:20:32.000000 p1_auth-0.1.4/p1_auth.egg-info/top_level.txt
+-rw-r--r--   0 jametobin   (502) staff       (20)     1053 2024-05-29 15:20:32.112897 p1_auth-0.1.4/setup.cfg
+-rw-r--r--   0 jametobin   (502) staff       (20)       95 2024-05-15 15:17:01.000000 p1_auth-0.1.4/setup.py
```

### Comparing `p1_auth-0.1.3/PKG-INFO` & `p1_auth-0.1.4/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: p1-auth
-Version: 0.1.3
+Version: 0.1.4
 Summary: Installable Django Authentication that adds support for Platform One
 Home-page: https://github.com/OpenLXP/p1-auth/
 Author: OpenLXP
 Author-email: openlxphost@gmail.com
 License: MIT
 Classifier: Development Status :: 4 - Beta
 Classifier: Environment :: Web Environment
@@ -155,14 +155,22 @@
 
 A flag to require JWTs on every request.
 
 ```python
 REQUIRE_JWT = True
 ```
 
+### JWT_PREFERRED_USERNAME_FIELD
+
+The field to use to populate the Username Field of the Django User model.  This defaults to `preferred_username`.
+
+```python
+JWT_PREFERRED_USERNAME_FIELD = "email"
+```
+
 ## Django Admin
 
 This section covers configurations that can be set in the Django Admin.
 
 ### RelatedAssignment
 
 RelatedAssignment allows selecting a Model (object_model) and instance (object_pk) that a user should be assigned to if all related AttributeChecks pass.
```

### Comparing `p1_auth-0.1.3/README.md` & `p1_auth-0.1.4/README.md`

 * *Files 2% similar despite different names*

```diff
@@ -131,14 +131,22 @@
 
 A flag to require JWTs on every request.
 
 ```python
 REQUIRE_JWT = True
 ```
 
+### JWT_PREFERRED_USERNAME_FIELD
+
+The field to use to populate the Username Field of the Django User model.  This defaults to `preferred_username`.
+
+```python
+JWT_PREFERRED_USERNAME_FIELD = "email"
+```
+
 ## Django Admin
 
 This section covers configurations that can be set in the Django Admin.
 
 ### RelatedAssignment
 
 RelatedAssignment allows selecting a Model (object_model) and instance (object_pk) that a user should be assigned to if all related AttributeChecks pass.
```

### Comparing `p1_auth-0.1.3/p1_auth/admin.py` & `p1_auth-0.1.4/p1_auth/admin.py`

 * *Files identical despite different names*

### Comparing `p1_auth-0.1.3/p1_auth/backends.py` & `p1_auth-0.1.4/p1_auth/backends.py`

 * *Files 3% similar despite different names*

```diff
@@ -25,15 +25,18 @@
         if hasattr(request, 'headers') and "Authorization" in request.headers:
             # decode JWT
             jwt_decoded = decode_jwt(request)
 
             # determine username and username field
             username = {
                 auth.get_user_model().USERNAME_FIELD:
-                jwt_decoded["preferred_username"]
+                jwt_decoded[getattr(
+                    settings,
+                    "JWT_PREFERRED_USERNAME_FIELD",
+                    "preferred_username")]
             }
 
             # retrieve or create user based on username
             user = auth.get_user_model().objects.get_or_create(**username)[0]
 
             if isinstance(user, AbstractBaseUser) and\
                     user.has_usable_password():
```

### Comparing `p1_auth-0.1.3/p1_auth/migrations/0001_initial.py` & `p1_auth-0.1.4/p1_auth/migrations/0001_initial.py`

 * *Files identical despite different names*

### Comparing `p1_auth-0.1.3/p1_auth/models.py` & `p1_auth-0.1.4/p1_auth/models.py`

 * *Files identical despite different names*

### Comparing `p1_auth-0.1.3/p1_auth/views.py` & `p1_auth-0.1.4/p1_auth/views.py`

 * *Files identical despite different names*

### Comparing `p1_auth-0.1.3/p1_auth.egg-info/PKG-INFO` & `p1_auth-0.1.4/p1_auth.egg-info/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: p1-auth
-Version: 0.1.3
+Version: 0.1.4
 Summary: Installable Django Authentication that adds support for Platform One
 Home-page: https://github.com/OpenLXP/p1-auth/
 Author: OpenLXP
 Author-email: openlxphost@gmail.com
 License: MIT
 Classifier: Development Status :: 4 - Beta
 Classifier: Environment :: Web Environment
@@ -155,14 +155,22 @@
 
 A flag to require JWTs on every request.
 
 ```python
 REQUIRE_JWT = True
 ```
 
+### JWT_PREFERRED_USERNAME_FIELD
+
+The field to use to populate the Username Field of the Django User model.  This defaults to `preferred_username`.
+
+```python
+JWT_PREFERRED_USERNAME_FIELD = "email"
+```
+
 ## Django Admin
 
 This section covers configurations that can be set in the Django Admin.
 
 ### RelatedAssignment
 
 RelatedAssignment allows selecting a Model (object_model) and instance (object_pk) that a user should be assigned to if all related AttributeChecks pass.
```

### Comparing `p1_auth-0.1.3/setup.cfg` & `p1_auth-0.1.4/setup.cfg`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [metadata]
 name = p1-auth
-version = 0.1.3
+version = 0.1.4
 description = Installable Django Authentication that adds support for Platform One
 long_description = file:README.md
 long_description_content_type = text/markdown
 url = https://github.com/OpenLXP/p1-auth/
 author = OpenLXP
 author_email = openlxphost@gmail.com
 license = MIT
```

