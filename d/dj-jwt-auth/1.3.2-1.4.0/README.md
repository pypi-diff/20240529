# Comparing `tmp/dj-jwt-auth-1.3.2.tar.gz` & `tmp/dj-jwt-auth-1.4.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dj-jwt-auth-1.3.2.tar", last modified: Thu May 23 16:46:55 2024, max compression
+gzip compressed data, was "dj-jwt-auth-1.4.0.tar", last modified: Wed May 29 17:24:03 2024, max compression
```

## Comparing `dj-jwt-auth-1.3.2.tar` & `dj-jwt-auth-1.4.0.tar`

### file list

```diff
@@ -1,29 +1,29 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-23 16:46:55.135604 dj-jwt-auth-1.3.2/
--rw-r--r--   0 runner    (1001) docker     (127)     3867 2024-05-23 16:46:55.135604 dj-jwt-auth-1.3.2/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     2926 2024-05-23 16:46:41.000000 dj-jwt-auth-1.3.2/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-23 16:46:55.131604 dj-jwt-auth-1.3.2/dj_jwt_auth.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     3867 2024-05-23 16:46:55.000000 dj-jwt-auth-1.3.2/dj_jwt_auth.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      513 2024-05-23 16:46:55.000000 dj-jwt-auth-1.3.2/dj_jwt_auth.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-23 16:46:55.000000 dj-jwt-auth-1.3.2/dj_jwt_auth.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       63 2024-05-23 16:46:55.000000 dj-jwt-auth-1.3.2/dj_jwt_auth.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       17 2024-05-23 16:46:55.000000 dj-jwt-auth-1.3.2/dj_jwt_auth.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-23 16:46:55.135604 dj-jwt-auth-1.3.2/django_jwt/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-23 16:46:41.000000 dj-jwt-auth-1.3.2/django_jwt/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1301 2024-05-23 16:46:41.000000 dj-jwt-auth-1.3.2/django_jwt/config.py
--rw-r--r--   0 runner    (1001) docker     (127)      198 2024-05-23 16:46:41.000000 dj-jwt-auth-1.3.2/django_jwt/exceptions.py
--rw-r--r--   0 runner    (1001) docker     (127)     1176 2024-05-23 16:46:41.000000 dj-jwt-auth-1.3.2/django_jwt/middleware.py
--rw-r--r--   0 runner    (1001) docker     (127)      711 2024-05-23 16:46:41.000000 dj-jwt-auth-1.3.2/django_jwt/pkce.py
--rw-r--r--   0 runner    (1001) docker     (127)      143 2024-05-23 16:46:41.000000 dj-jwt-auth-1.3.2/django_jwt/roles.py
--rw-r--r--   0 runner    (1001) docker     (127)     1482 2024-05-23 16:46:41.000000 dj-jwt-auth-1.3.2/django_jwt/settings.py
--rw-r--r--   0 runner    (1001) docker     (127)      251 2024-05-23 16:46:41.000000 dj-jwt-auth-1.3.2/django_jwt/urls.py
--rw-r--r--   0 runner    (1001) docker     (127)     5021 2024-05-23 16:46:41.000000 dj-jwt-auth-1.3.2/django_jwt/user.py
--rw-r--r--   0 runner    (1001) docker     (127)     1485 2024-05-23 16:46:41.000000 dj-jwt-auth-1.3.2/django_jwt/utils.py
--rw-r--r--   0 runner    (1001) docker     (127)     3705 2024-05-23 16:46:41.000000 dj-jwt-auth-1.3.2/django_jwt/views.py
--rw-r--r--   0 runner    (1001) docker     (127)      221 2024-05-23 16:46:41.000000 dj-jwt-auth-1.3.2/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)      991 2024-05-23 16:46:55.135604 dj-jwt-auth-1.3.2/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)       90 2024-05-23 16:46:41.000000 dj-jwt-auth-1.3.2/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-23 16:46:55.135604 dj-jwt-auth-1.3.2/tests/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-23 16:46:41.000000 dj-jwt-auth-1.3.2/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      251 2024-05-23 16:46:41.000000 dj-jwt-auth-1.3.2/tests/models.py
--rw-r--r--   0 runner    (1001) docker     (127)     7460 2024-05-23 16:46:41.000000 dj-jwt-auth-1.3.2/tests/test.py
--rw-r--r--   0 runner    (1001) docker     (127)      212 2024-05-23 16:46:41.000000 dj-jwt-auth-1.3.2/tests/urls.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-29 17:24:02.998390 dj-jwt-auth-1.4.0/
+-rw-r--r--   0 runner    (1001) docker     (127)     3946 2024-05-29 17:24:02.998390 dj-jwt-auth-1.4.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     3005 2024-05-29 17:23:52.000000 dj-jwt-auth-1.4.0/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-29 17:24:02.998390 dj-jwt-auth-1.4.0/dj_jwt_auth.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     3946 2024-05-29 17:24:02.000000 dj-jwt-auth-1.4.0/dj_jwt_auth.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      513 2024-05-29 17:24:02.000000 dj-jwt-auth-1.4.0/dj_jwt_auth.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-29 17:24:02.000000 dj-jwt-auth-1.4.0/dj_jwt_auth.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       63 2024-05-29 17:24:02.000000 dj-jwt-auth-1.4.0/dj_jwt_auth.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       17 2024-05-29 17:24:02.000000 dj-jwt-auth-1.4.0/dj_jwt_auth.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-29 17:24:02.998390 dj-jwt-auth-1.4.0/django_jwt/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-29 17:23:52.000000 dj-jwt-auth-1.4.0/django_jwt/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1301 2024-05-29 17:23:52.000000 dj-jwt-auth-1.4.0/django_jwt/config.py
+-rw-r--r--   0 runner    (1001) docker     (127)      198 2024-05-29 17:23:52.000000 dj-jwt-auth-1.4.0/django_jwt/exceptions.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1176 2024-05-29 17:23:52.000000 dj-jwt-auth-1.4.0/django_jwt/middleware.py
+-rw-r--r--   0 runner    (1001) docker     (127)      711 2024-05-29 17:23:52.000000 dj-jwt-auth-1.4.0/django_jwt/pkce.py
+-rw-r--r--   0 runner    (1001) docker     (127)      143 2024-05-29 17:23:52.000000 dj-jwt-auth-1.4.0/django_jwt/roles.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1552 2024-05-29 17:23:52.000000 dj-jwt-auth-1.4.0/django_jwt/settings.py
+-rw-r--r--   0 runner    (1001) docker     (127)      251 2024-05-29 17:23:52.000000 dj-jwt-auth-1.4.0/django_jwt/urls.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4930 2024-05-29 17:23:52.000000 dj-jwt-auth-1.4.0/django_jwt/user.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1485 2024-05-29 17:23:52.000000 dj-jwt-auth-1.4.0/django_jwt/utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3705 2024-05-29 17:23:52.000000 dj-jwt-auth-1.4.0/django_jwt/views.py
+-rw-r--r--   0 runner    (1001) docker     (127)      221 2024-05-29 17:23:52.000000 dj-jwt-auth-1.4.0/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)      991 2024-05-29 17:24:02.998390 dj-jwt-auth-1.4.0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)       90 2024-05-29 17:23:52.000000 dj-jwt-auth-1.4.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-29 17:24:02.998390 dj-jwt-auth-1.4.0/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-29 17:23:52.000000 dj-jwt-auth-1.4.0/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      251 2024-05-29 17:23:52.000000 dj-jwt-auth-1.4.0/tests/models.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7405 2024-05-29 17:23:52.000000 dj-jwt-auth-1.4.0/tests/test.py
+-rw-r--r--   0 runner    (1001) docker     (127)      212 2024-05-29 17:23:52.000000 dj-jwt-auth-1.4.0/tests/urls.py
```

### Comparing `dj-jwt-auth-1.3.2/PKG-INFO` & `dj-jwt-auth-1.4.0/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: dj-jwt-auth
-Version: 1.3.2
+Version: 1.4.0
 Summary: A Django package for JSON Web Token validation and verification. Using PyJWT.
 Home-page: https://www.example.com/
 Author: Konstantin Seleznev
 Author-email: k.seleznev@elsevier.com
 License: MIT
 Classifier: Environment :: Web Environment
 Classifier: Framework :: Django
@@ -61,14 +61,15 @@
 - OIDC_AUDIENCE - by default ["account", "broker"]
 
 User retated variables:
 - OIDC_USER_UPDATE - if True, user model will be updated from userinfo endpoint if MODIFIED date has changed, by default True
 - OIDC_USER_MODIFIED_FIELD - user model field to store last modified date, by default `modified_timestamp`
 - OIDC_TOKEN_MODIFIED_FIELD - access token field to store last modified date, by default `updated_at`
 - OIDC_USER_UID - User model" unique identifier, by default `kc_id`
+- OIDC_TOKEN_USER_UID - access token field to store user UID, by default `sub`
 - OIDC_USER_MAPPING - mapping between JWT claims and user model fields, by default:
 ```
     OIDC_USER_MAPPING = {
         "first_name": "first_name",
         "last_name": "last_name",
         "username": "username",
     }
```

### Comparing `dj-jwt-auth-1.3.2/README.md` & `dj-jwt-auth-1.4.0/README.md`

 * *Files 3% similar despite different names*

```diff
@@ -37,14 +37,15 @@
 - OIDC_AUDIENCE - by default ["account", "broker"]
 
 User retated variables:
 - OIDC_USER_UPDATE - if True, user model will be updated from userinfo endpoint if MODIFIED date has changed, by default True
 - OIDC_USER_MODIFIED_FIELD - user model field to store last modified date, by default `modified_timestamp`
 - OIDC_TOKEN_MODIFIED_FIELD - access token field to store last modified date, by default `updated_at`
 - OIDC_USER_UID - User model" unique identifier, by default `kc_id`
+- OIDC_TOKEN_USER_UID - access token field to store user UID, by default `sub`
 - OIDC_USER_MAPPING - mapping between JWT claims and user model fields, by default:
 ```
     OIDC_USER_MAPPING = {
         "first_name": "first_name",
         "last_name": "last_name",
         "username": "username",
     }
```

### Comparing `dj-jwt-auth-1.3.2/dj_jwt_auth.egg-info/PKG-INFO` & `dj-jwt-auth-1.4.0/dj_jwt_auth.egg-info/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: dj-jwt-auth
-Version: 1.3.2
+Version: 1.4.0
 Summary: A Django package for JSON Web Token validation and verification. Using PyJWT.
 Home-page: https://www.example.com/
 Author: Konstantin Seleznev
 Author-email: k.seleznev@elsevier.com
 License: MIT
 Classifier: Environment :: Web Environment
 Classifier: Framework :: Django
@@ -61,14 +61,15 @@
 - OIDC_AUDIENCE - by default ["account", "broker"]
 
 User retated variables:
 - OIDC_USER_UPDATE - if True, user model will be updated from userinfo endpoint if MODIFIED date has changed, by default True
 - OIDC_USER_MODIFIED_FIELD - user model field to store last modified date, by default `modified_timestamp`
 - OIDC_TOKEN_MODIFIED_FIELD - access token field to store last modified date, by default `updated_at`
 - OIDC_USER_UID - User model" unique identifier, by default `kc_id`
+- OIDC_TOKEN_USER_UID - access token field to store user UID, by default `sub`
 - OIDC_USER_MAPPING - mapping between JWT claims and user model fields, by default:
 ```
     OIDC_USER_MAPPING = {
         "first_name": "first_name",
         "last_name": "last_name",
         "username": "username",
     }
```

### Comparing `dj-jwt-auth-1.3.2/dj_jwt_auth.egg-info/SOURCES.txt` & `dj-jwt-auth-1.4.0/dj_jwt_auth.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `dj-jwt-auth-1.3.2/django_jwt/config.py` & `dj-jwt-auth-1.4.0/django_jwt/config.py`

 * *Files identical despite different names*

### Comparing `dj-jwt-auth-1.3.2/django_jwt/middleware.py` & `dj-jwt-auth-1.4.0/django_jwt/middleware.py`

 * *Files identical despite different names*

### Comparing `dj-jwt-auth-1.3.2/django_jwt/pkce.py` & `dj-jwt-auth-1.4.0/django_jwt/pkce.py`

 * *Files identical despite different names*

### Comparing `dj-jwt-auth-1.3.2/django_jwt/settings.py` & `dj-jwt-auth-1.4.0/django_jwt/settings.py`

 * *Files 2% similar despite different names*

```diff
@@ -4,14 +4,15 @@
 OIDC_AUDIENCE = getattr(settings, "OIDC_AUDIENCE", ["account", "broker"])
 OIDC_CONFIG_URL = getattr(settings, "OIDC_CONFIG_URL", None)
 
 # key from KeyCloak; value is user model
 OIDC_USER_UPDATE = getattr(settings, "OIDC_USER_UPDATE", True)
 OIDC_USER_MODIFIED_FIELD = getattr(settings, "OIDC_USER_MODIFIED_FIELD", "modified_timestamp")
 OIDC_TOKEN_MODIFIED_FIELD = getattr(settings, "OIDC_TOKEN_MODIFIED_FIELD", "updated_at")
+OIDC_TOKEN_USER_UID = getattr(settings, "OIDC_TOKEN_USER_UID", "sub")
 OIDC_USER_UID = getattr(settings, "OIDC_USER_UID", "kc_id")
 OIDC_USER_MAPPING = getattr(
     settings,
     "OIDC_USER_MAPPING",
     {
         "given_name": "first_name",
         "family_name": "last_name",
```

### Comparing `dj-jwt-auth-1.3.2/django_jwt/user.py` & `dj-jwt-auth-1.4.0/django_jwt/user.py`

 * *Files 4% similar despite different names*

```diff
@@ -17,17 +17,16 @@
 
 
 class UserHandler:
     modified_at = None
 
     def __init__(self, payload: dict, request: HttpRequest, access_token: str):
         # payload of access token without user info
-        # auth0_id should be available if auth0 added in Client Scopes in KeyCloak admin
         self.kwargs = settings.OIDC_USER_DEFAULTS.copy()
-        self.kwargs[settings.OIDC_USER_UID] = payload.get("auth0_id", payload["sub"])
+        self.kwargs[settings.OIDC_USER_UID] = payload[settings.OIDC_TOKEN_USER_UID]
 
         modified_at = payload.get(settings.OIDC_TOKEN_MODIFIED_FIELD, None)
         if modified_at and isinstance(modified_at, int):
             self.modified_at = utc.localize(datetime.fromtimestamp(modified_at))
 
         self.on_create = settings.OIDC_USER_ON_CREATE
         self.on_update = settings.OIDC_USER_ON_UPDATE
```

### Comparing `dj-jwt-auth-1.3.2/django_jwt/utils.py` & `dj-jwt-auth-1.4.0/django_jwt/utils.py`

 * *Files identical despite different names*

### Comparing `dj-jwt-auth-1.3.2/django_jwt/views.py` & `dj-jwt-auth-1.4.0/django_jwt/views.py`

 * *Files identical despite different names*

### Comparing `dj-jwt-auth-1.3.2/setup.cfg` & `dj-jwt-auth-1.4.0/setup.cfg`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [metadata]
 name = dj-jwt-auth
-version = 1.3.2
+version = 1.4.0
 description = A Django package for JSON Web Token validation and verification. Using PyJWT.
 long_description = file: README.md
 url = https://www.example.com/
 author = Konstantin Seleznev
 author_email = k.seleznev@elsevier.com
 license = MIT
 classifiers =
```

### Comparing `dj-jwt-auth-1.3.2/tests/test.py` & `dj-jwt-auth-1.4.0/tests/test.py`

 * *Files 8% similar despite different names*

```diff
@@ -9,21 +9,19 @@
 
 from django_jwt import settings
 from django_jwt.middleware import JWTAuthMiddleware
 from django_jwt.user import role_handler
 from django_jwt.roles import ROLE
 
 access_token_payload = {
-    "sub": "12345",
-    "auth0_id": "1234",
+    "sub": "1234",
     "updated_at": 2687276498,
 }
 user_info_payload = {
-    "sub": "12345",
-    "auth0_id": "1234",
+    "sub": "1234",
     "email": "example@bk.com",
     "name": "UserName",
     "given_name": "1st name",
     "family_name": "LastName",
 }
 User = get_user_model()
 
@@ -47,15 +45,15 @@
         self.request.META = {"HTTP_AUTHORIZATION": "Bearer 1234"}
 
     def assertUserWithPayload(self):
         self.assertEqual(self.request.user.first_name, user_info_payload["given_name"])
         self.assertEqual(self.request.user.last_name, user_info_payload["family_name"])
         self.assertEqual(self.request.user.username, user_info_payload["name"])
         self.assertEqual(self.request.user.email, user_info_payload["email"])
-        self.assertEqual(self.request.user.kc_id, user_info_payload["auth0_id"])
+        self.assertEqual(self.request.user.kc_id, user_info_payload["sub"])
 
     def test_keycloak_new_user(self, *_):
         """User is created if it doesn't exist in database"""
         self.middleware.process_request(self.request)
         self.assertUserWithPayload()
 
     def test_exists_kc_id_user(self, *_):
```

