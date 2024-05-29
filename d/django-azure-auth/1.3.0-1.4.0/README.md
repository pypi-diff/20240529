# Comparing `tmp/django_azure_auth-1.3.0.tar.gz` & `tmp/django_azure_auth-1.4.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "django_azure_auth-1.3.0.tar", max compression
+gzip compressed data, was "django_azure_auth-1.4.0.tar", max compression
```

## Comparing `django_azure_auth-1.3.0.tar` & `django_azure_auth-1.4.0.tar`

### file list

```diff
@@ -1,20 +1,20 @@
--rw-r--r--   0        0        0     1064 2024-04-27 16:50:15.543754 django_azure_auth-1.3.0/LICENSE
--rw-r--r--   0        0        0     5957 2024-04-27 16:50:15.543754 django_azure_auth-1.3.0/README.md
--rw-r--r--   0        0        0        0 2024-04-27 16:50:15.543754 django_azure_auth-1.3.0/azure_auth/__init__.py
--rw-r--r--   0        0        0      151 2024-04-27 16:50:15.543754 django_azure_auth-1.3.0/azure_auth/apps.py
--rw-r--r--   0        0        0      415 2024-04-27 16:50:15.543754 django_azure_auth-1.3.0/azure_auth/backends.py
--rw-r--r--   0        0        0      529 2024-04-27 16:50:15.543754 django_azure_auth-1.3.0/azure_auth/decorators.py
--rw-r--r--   0        0        0      333 2024-04-27 16:50:15.547754 django_azure_auth-1.3.0/azure_auth/exceptions.py
--rw-r--r--   0        0        0     6773 2024-04-27 16:50:15.547754 django_azure_auth-1.3.0/azure_auth/handlers.py
--rw-r--r--   0        0        0     1148 2024-04-27 16:50:15.547754 django_azure_auth-1.3.0/azure_auth/middleware.py
--rw-r--r--   0        0        0        0 2024-04-27 16:50:15.547754 django_azure_auth-1.3.0/azure_auth/tests/__init__.py
--rw-r--r--   0        0        0     2091 2024-04-27 16:50:15.547754 django_azure_auth-1.3.0/azure_auth/tests/conftest.py
--rw-r--r--   0        0        0     3943 2024-04-27 16:50:15.547754 django_azure_auth-1.3.0/azure_auth/tests/settings.py
--rw-r--r--   0        0        0     1409 2024-04-27 16:50:15.547754 django_azure_auth-1.3.0/azure_auth/tests/test_decorators.py
--rw-r--r--   0        0        0     1885 2024-04-27 16:50:15.547754 django_azure_auth-1.3.0/azure_auth/tests/test_middleware.py
--rw-r--r--   0        0        0    11869 2024-04-27 16:50:15.547754 django_azure_auth-1.3.0/azure_auth/tests/test_views.py
--rw-r--r--   0        0        0     1017 2024-04-27 16:50:15.547754 django_azure_auth-1.3.0/azure_auth/tests/urls.py
--rw-r--r--   0        0        0      324 2024-04-27 16:50:15.547754 django_azure_auth-1.3.0/azure_auth/urls.py
--rw-r--r--   0        0        0      869 2024-04-27 16:50:15.547754 django_azure_auth-1.3.0/azure_auth/views.py
--rw-r--r--   0        0        0     1464 2024-04-27 16:50:15.547754 django_azure_auth-1.3.0/pyproject.toml
--rw-r--r--   0        0        0     6938 1970-01-01 00:00:00.000000 django_azure_auth-1.3.0/PKG-INFO
+-rw-r--r--   0        0        0     1064 2024-05-28 16:20:29.815346 django_azure_auth-1.4.0/LICENSE
+-rw-r--r--   0        0        0     6081 2024-05-28 16:20:29.815346 django_azure_auth-1.4.0/README.md
+-rw-r--r--   0        0        0        0 2024-05-28 16:20:29.815346 django_azure_auth-1.4.0/azure_auth/__init__.py
+-rw-r--r--   0        0        0      151 2024-05-28 16:20:29.815346 django_azure_auth-1.4.0/azure_auth/apps.py
+-rw-r--r--   0        0        0      415 2024-05-28 16:20:29.815346 django_azure_auth-1.4.0/azure_auth/backends.py
+-rw-r--r--   0        0        0      529 2024-05-28 16:20:29.815346 django_azure_auth-1.4.0/azure_auth/decorators.py
+-rw-r--r--   0        0        0      333 2024-05-28 16:20:29.815346 django_azure_auth-1.4.0/azure_auth/exceptions.py
+-rw-r--r--   0        0        0     6704 2024-05-28 16:20:29.815346 django_azure_auth-1.4.0/azure_auth/handlers.py
+-rw-r--r--   0        0        0     1327 2024-05-28 16:20:29.815346 django_azure_auth-1.4.0/azure_auth/middleware.py
+-rw-r--r--   0        0        0        0 2024-05-28 16:20:29.815346 django_azure_auth-1.4.0/azure_auth/tests/__init__.py
+-rw-r--r--   0        0        0     2091 2024-05-28 16:20:29.815346 django_azure_auth-1.4.0/azure_auth/tests/conftest.py
+-rw-r--r--   0        0        0     3943 2024-05-28 16:20:29.815346 django_azure_auth-1.4.0/azure_auth/tests/settings.py
+-rw-r--r--   0        0        0     1409 2024-05-28 16:20:29.815346 django_azure_auth-1.4.0/azure_auth/tests/test_decorators.py
+-rw-r--r--   0        0        0     2019 2024-05-28 16:20:29.815346 django_azure_auth-1.4.0/azure_auth/tests/test_middleware.py
+-rw-r--r--   0        0        0    13037 2024-05-28 16:20:29.815346 django_azure_auth-1.4.0/azure_auth/tests/test_views.py
+-rw-r--r--   0        0        0     1017 2024-05-28 16:20:29.815346 django_azure_auth-1.4.0/azure_auth/tests/urls.py
+-rw-r--r--   0        0        0      324 2024-05-28 16:20:29.819346 django_azure_auth-1.4.0/azure_auth/urls.py
+-rw-r--r--   0        0        0     1045 2024-05-28 16:20:29.819346 django_azure_auth-1.4.0/azure_auth/views.py
+-rw-r--r--   0        0        0     1464 2024-05-28 16:20:29.819346 django_azure_auth-1.4.0/pyproject.toml
+-rw-r--r--   0        0        0     7062 1970-01-01 00:00:00.000000 django_azure_auth-1.4.0/PKG-INFO
```

### Comparing `django_azure_auth-1.3.0/LICENSE` & `django_azure_auth-1.4.0/LICENSE`

 * *Files identical despite different names*

### Comparing `django_azure_auth-1.3.0/README.md` & `django_azure_auth-1.4.0/README.md`

 * *Files 2% similar despite different names*

```diff
@@ -1,9 +1,10 @@
 ![Build](https://github.com/Weird-Sheep-Labs/django-azure-auth/actions/workflows/ci.yml/badge.svg)
 ![Coverage Status](./reports/coverage/coverage-badge.svg?dummy=8484744)
+[![PyPI downloads](https://img.shields.io/pypi/dm/django-azure-auth.svg)](https://pypistats.org/packages/django-azure-auth)
 
 # django-azure-auth
 
 ### A simple Django app for user authentication with Azure Active Directory/Entra ID.
 
 by [Weird Sheep Labs](https://weirdsheeplabs.com)
```

### Comparing `django_azure_auth-1.3.0/azure_auth/decorators.py` & `django_azure_auth-1.4.0/azure_auth/decorators.py`

 * *Files identical despite different names*

### Comparing `django_azure_auth-1.3.0/azure_auth/handlers.py` & `django_azure_auth-1.4.0/azure_auth/handlers.py`

 * *Files 2% similar despite different names*

```diff
@@ -36,15 +36,14 @@
     def get_auth_uri(self) -> str:
         """
         Requests the auth flow dictionary and stores it on the session to be
         queried later in the auth process.
 
         :return: Authentication redirect URI
         """
-        # TODO: Handle if user has put incorrect details in settings
         flow = self.msal_app.initiate_auth_code_flow(
             scopes=settings.AZURE_AUTH["SCOPES"],
             redirect_uri=settings.AZURE_AUTH["REDIRECT_URI"],
         )
         self.request.session[self.auth_flow_session_key] = flow
         return flow["auth_uri"]
```

### Comparing `django_azure_auth-1.3.0/azure_auth/middleware.py` & `django_azure_auth-1.4.0/azure_auth/middleware.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,19 +1,20 @@
 from django.conf import settings
+from django.http import HttpRequest
 from django.shortcuts import redirect
 from django.urls import reverse
 
 from .handlers import AuthHandler
 
 
 class AzureMiddleware:
     def __init__(self, get_response):
         self.get_response = get_response
 
-    def __call__(self, request):
+    def __call__(self, request: HttpRequest):
         public_views = ["azure_auth:login", "azure_auth:logout", "azure_auth:callback"]
         public_views.extend(settings.AZURE_AUTH.get("PUBLIC_URLS", []))
         public_urls = [reverse(view_name) for view_name in public_views]
         public_paths = settings.AZURE_AUTH.get(
             "PUBLIC_PATHS", []
         )  # added to resolve paths
 
@@ -25,8 +26,11 @@
             if request.path_info.startswith(path):
                 return self.get_response(request)
 
         if AuthHandler(request).get_token_from_cache():
             # If the user is authenticated
             if request.user.is_authenticated:
                 return self.get_response(request)
+
+        # Save the intended path on the session to be redirected there upon login
+        request.session["next"] = request.path
         return redirect("azure_auth:login")
```

### Comparing `django_azure_auth-1.3.0/azure_auth/tests/conftest.py` & `django_azure_auth-1.4.0/azure_auth/tests/conftest.py`

 * *Files identical despite different names*

### Comparing `django_azure_auth-1.3.0/azure_auth/tests/settings.py` & `django_azure_auth-1.4.0/azure_auth/tests/settings.py`

 * *Files identical despite different names*

### Comparing `django_azure_auth-1.3.0/azure_auth/tests/test_decorators.py` & `django_azure_auth-1.4.0/azure_auth/tests/test_decorators.py`

 * *Files identical despite different names*

### Comparing `django_azure_auth-1.3.0/azure_auth/tests/test_middleware.py` & `django_azure_auth-1.4.0/azure_auth/tests/test_middleware.py`

 * *Files 6% similar despite different names*

```diff
@@ -11,23 +11,25 @@
 @pytest.mark.usefixtures("token")
 @patch.object(msal, "ConfidentialClientApplication")
 class TestAzureAuthMiddleware(TransactionTestCase):
     def test_invalid_token(self, mocked_msal_app):
         mocked_msal_app.return_value.acquire_token_silent.return_value = None
         resp = self.client.get(reverse("middleware_protected"))
         assert resp.status_code == HTTPStatus.FOUND
-        assert resp.url == reverse("azure_auth:login")  # type: ignore
+        assert resp.url == "/azure_auth/login"  # type: ignore
+        assert self.client.session.get("next") == "/middleware_protected/"
 
     def test_valid_token_unauthenticated_user(self, mocked_msal_app):
         # Not sure how this situation could arise but test anyway...
 
         mocked_msal_app.return_value.acquire_token_silent.return_value = self.token  # type: ignore
         resp = self.client.get(reverse("middleware_protected"))
         assert resp.status_code == HTTPStatus.FOUND
-        assert resp.url == reverse("azure_auth:login")  # type: ignore
+        assert resp.url == "/azure_auth/login"  # type: ignore
+        assert self.client.session.get("next") == "/middleware_protected/"
 
     def test_valid_token_authenticated_user(self, mocked_msal_app):
         mocked_msal_app.return_value.acquire_token_silent.return_value = self.token  # type: ignore
         self.client.force_login(self.user)  # type: ignore
 
         resp = self.client.get(reverse("middleware_protected"))
         assert resp.status_code == HTTPStatus.OK
```

### Comparing `django_azure_auth-1.3.0/azure_auth/tests/test_views.py` & `django_azure_auth-1.4.0/azure_auth/tests/test_views.py`

 * *Files 4% similar despite different names*

```diff
@@ -235,14 +235,41 @@
         # Make user inactive
         self.user.is_active = False  # type: ignore
         self.user.save()  # type: ignore
         resp = self.client.get(reverse("azure_auth:callback"))
         assert resp.status_code == HTTPStatus.FORBIDDEN
         assert resp.content.decode() == "Invalid email for this app."
 
+    def test_callback_redirect(self, mocked_msal_app, mocked_requests, mocked_cache):
+        mocked_msal_app.return_value.acquire_token_by_auth_code_flow.return_value = (
+            self.token  # type: ignore
+        )
+        mocked_cache.has_state_changed = True
+        mocked_cache.serialize = msal.SerializableTokenCache().serialize
+        mocked_cache.deserialize = msal.SerializableTokenCache().deserialize
+
+        # Graph API response
+        expected_response_json = self._get_graph_response(self.user)  # type: ignore
+        mocked_requests.get.side_effect = [
+            self._mocked_response(HTTPStatus.OK, expected_response_json)
+        ]
+
+        # `next` should be on the session
+        session = self.client.session
+        session["next"] = "/middleware_protected/"  # type: ignore
+        session.save()
+
+        resp = self.client.get(reverse("azure_auth:callback"))
+        assert resp.status_code == HTTPStatus.FOUND
+        assert resp.url == reverse("middleware_protected")  # type: ignore
+        assert "id_token_claims" in self.client.session
+
+        self._msal_asserts(mocked_msal_app)
+        self._graph_asserts(mocked_requests)
+
 
 @pytest.mark.usefixtures("token")
 class TestLogoutView(TestCase):
     # No redirect logout
     no_logout_query_params_settings = copy.deepcopy(settings.AZURE_AUTH)
     del no_logout_query_params_settings["LOGOUT_URI"]
```

### Comparing `django_azure_auth-1.3.0/azure_auth/tests/urls.py` & `django_azure_auth-1.4.0/azure_auth/tests/urls.py`

 * *Files identical despite different names*

### Comparing `django_azure_auth-1.3.0/azure_auth/views.py` & `django_azure_auth-1.4.0/azure_auth/views.py`

 * *Files 9% similar despite different names*

```diff
@@ -1,27 +1,29 @@
 from django.conf import settings
 from django.contrib.auth import authenticate, login, logout
-from django.http import HttpResponseForbidden, HttpResponseRedirect
+from django.http import HttpRequest, HttpResponseForbidden, HttpResponseRedirect
 
 from .handlers import AuthHandler
 
 
-def azure_auth_login(request):
+def azure_auth_login(request: HttpRequest):
     return HttpResponseRedirect(AuthHandler(request).get_auth_uri())
 
 
-def azure_auth_logout(request):
+def azure_auth_logout(request: HttpRequest):
     # Auth handler has to be initialized before `logout()` to load the claims from the session
     auth_handler = AuthHandler(request)
 
     logout(request)
     return HttpResponseRedirect(auth_handler.get_logout_uri())
 
 
-def azure_auth_callback(request):
+def azure_auth_callback(request: HttpRequest):
     token = AuthHandler(request).get_token_from_flow()
     user = authenticate(request, token=token)
     if user:
+        # Get the `next` URL from the anonymous session before login
+        next = request.session.get("next", "")
         login(request, user)
     else:
         return HttpResponseForbidden("Invalid email for this app.")
-    return HttpResponseRedirect(settings.LOGIN_REDIRECT_URL)
+    return HttpResponseRedirect(next or settings.LOGIN_REDIRECT_URL)
```

### Comparing `django_azure_auth-1.3.0/pyproject.toml` & `django_azure_auth-1.4.0/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "django-azure-auth"
-version = "1.3.0"
+version = "1.4.0"
 description = "A simple Django app for user authentication with Azure Active Directory/Entra ID."
 authors = ["Weird Sheep Labs <info@weirdsheeplabs.com>"]
 license = "MIT"
 readme = "README.md"
 homepage = "https://github.com/Weird-Sheep-Labs/django-azure-auth"
 keywords = ['django', 'azure', 'authentication', 'microsoft', 'entra']
 classifiers = [
```

### Comparing `django_azure_auth-1.3.0/PKG-INFO` & `django_azure_auth-1.4.0/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: django-azure-auth
-Version: 1.3.0
+Version: 1.4.0
 Summary: A simple Django app for user authentication with Azure Active Directory/Entra ID.
 Home-page: https://github.com/Weird-Sheep-Labs/django-azure-auth
 License: MIT
 Keywords: django,azure,authentication,microsoft,entra
 Author: Weird Sheep Labs
 Author-email: info@weirdsheeplabs.com
 Requires-Python: >=3.8,<4.0
@@ -20,14 +20,15 @@
 Classifier: Programming Language :: Python :: 3.12
 Requires-Dist: Django (>=3.2)
 Requires-Dist: msal (>=1.18.0,<2.0.0)
 Description-Content-Type: text/markdown
 
 ![Build](https://github.com/Weird-Sheep-Labs/django-azure-auth/actions/workflows/ci.yml/badge.svg)
 ![Coverage Status](./reports/coverage/coverage-badge.svg?dummy=8484744)
+[![PyPI downloads](https://img.shields.io/pypi/dm/django-azure-auth.svg)](https://pypistats.org/packages/django-azure-auth)
 
 # django-azure-auth
 
 ### A simple Django app for user authentication with Azure Active Directory/Entra ID.
 
 by [Weird Sheep Labs](https://weirdsheeplabs.com)
```

