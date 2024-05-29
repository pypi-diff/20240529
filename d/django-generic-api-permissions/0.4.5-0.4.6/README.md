# Comparing `tmp/django_generic_api_permissions-0.4.5.tar.gz` & `tmp/django_generic_api_permissions-0.4.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "django_generic_api_permissions-0.4.5.tar", max compression
+gzip compressed data, was "django_generic_api_permissions-0.4.6.tar", max compression
```

## Comparing `django_generic_api_permissions-0.4.5.tar` & `django_generic_api_permissions-0.4.6.tar`

### file list

```diff
@@ -1,14 +1,14 @@
--rw-r--r--   0        0        0    15276 2024-04-17 11:27:38.601732 django_generic_api_permissions-0.4.5/CHANGELOG.md
--rw-r--r--   0        0        0     7651 2024-04-17 11:27:09.781709 django_generic_api_permissions-0.4.5/LICENSE
--rw-r--r--   0        0        0    11571 2024-04-17 11:27:09.781709 django_generic_api_permissions-0.4.5/README.md
--rw-r--r--   0        0        0        0 2024-04-17 11:27:09.781709 django_generic_api_permissions-0.4.5/generic_permissions/__init__.py
--rw-r--r--   0        0        0     1389 2024-04-17 11:27:09.781709 django_generic_api_permissions-0.4.5/generic_permissions/apps.py
--rw-r--r--   0        0        0     4005 2024-04-17 11:27:09.781709 django_generic_api_permissions-0.4.5/generic_permissions/config.py
--rw-r--r--   0        0        0      746 2024-04-17 11:27:09.781709 django_generic_api_permissions-0.4.5/generic_permissions/models.py
--rw-r--r--   0        0        0     2437 2024-04-17 11:27:09.781709 django_generic_api_permissions-0.4.5/generic_permissions/permissions.py
--rw-r--r--   0        0        0      492 2024-04-17 11:27:09.781709 django_generic_api_permissions-0.4.5/generic_permissions/serializers.py
--rw-r--r--   0        0        0     1439 2024-04-17 11:27:09.781709 django_generic_api_permissions-0.4.5/generic_permissions/validation.py
--rw-r--r--   0        0        0      973 2024-04-17 11:27:09.781709 django_generic_api_permissions-0.4.5/generic_permissions/views.py
--rw-r--r--   0        0        0     6997 2024-04-17 11:27:09.781709 django_generic_api_permissions-0.4.5/generic_permissions/visibilities.py
--rw-r--r--   0        0        0     4069 2024-04-17 11:27:38.645732 django_generic_api_permissions-0.4.5/pyproject.toml
--rw-r--r--   0        0        0    12734 1970-01-01 00:00:00.000000 django_generic_api_permissions-0.4.5/PKG-INFO
+-rw-r--r--   0        0        0    20266 2024-05-29 08:27:02.046006 django_generic_api_permissions-0.4.6/CHANGELOG.md
+-rw-r--r--   0        0        0     7651 2024-05-29 08:26:32.234122 django_generic_api_permissions-0.4.6/LICENSE
+-rw-r--r--   0        0        0    11571 2024-05-29 08:26:32.234122 django_generic_api_permissions-0.4.6/README.md
+-rw-r--r--   0        0        0        0 2024-05-29 08:26:32.234122 django_generic_api_permissions-0.4.6/generic_permissions/__init__.py
+-rw-r--r--   0        0        0     1389 2024-05-29 08:26:32.234122 django_generic_api_permissions-0.4.6/generic_permissions/apps.py
+-rw-r--r--   0        0        0     4005 2024-05-29 08:26:32.234122 django_generic_api_permissions-0.4.6/generic_permissions/config.py
+-rw-r--r--   0        0        0      746 2024-05-29 08:26:32.234122 django_generic_api_permissions-0.4.6/generic_permissions/models.py
+-rw-r--r--   0        0        0     2476 2024-05-29 08:26:32.234122 django_generic_api_permissions-0.4.6/generic_permissions/permissions.py
+-rw-r--r--   0        0        0      492 2024-05-29 08:26:32.234122 django_generic_api_permissions-0.4.6/generic_permissions/serializers.py
+-rw-r--r--   0        0        0     1439 2024-05-29 08:26:32.234122 django_generic_api_permissions-0.4.6/generic_permissions/validation.py
+-rw-r--r--   0        0        0      973 2024-05-29 08:26:32.234122 django_generic_api_permissions-0.4.6/generic_permissions/views.py
+-rw-r--r--   0        0        0     6997 2024-05-29 08:26:32.234122 django_generic_api_permissions-0.4.6/generic_permissions/visibilities.py
+-rw-r--r--   0        0        0     4075 2024-05-29 08:27:02.094005 django_generic_api_permissions-0.4.6/pyproject.toml
+-rw-r--r--   0        0        0    12734 1970-01-01 00:00:00.000000 django_generic_api_permissions-0.4.6/PKG-INFO
```

### Comparing `django_generic_api_permissions-0.4.5/CHANGELOG.md` & `django_generic_api_permissions-0.4.6/CHANGELOG.md`

 * *Files 21% similar despite different names*

```diff
@@ -1,15 +1,131 @@
 # CHANGELOG
 
 
 
+## v0.4.6 (2024-05-29)
+
+### Chore
+
+* chore(deps): bump python-semantic-release/python-semantic-release
+
+Bumps [python-semantic-release/python-semantic-release](https://github.com/python-semantic-release/python-semantic-release) from 8.3.0 to 9.7.3.
+- [Release notes](https://github.com/python-semantic-release/python-semantic-release/releases)
+- [Changelog](https://github.com/python-semantic-release/python-semantic-release/blob/master/CHANGELOG.md)
+- [Commits](https://github.com/python-semantic-release/python-semantic-release/compare/v8.3.0...v9.7.3)
+
+---
+updated-dependencies:
+- dependency-name: python-semantic-release/python-semantic-release
+  dependency-type: direct:production
+  update-type: version-update:semver-major
+...
+
+Signed-off-by: dependabot[bot] &lt;support@github.com&gt; ([`d9655f1`](https://github.com/adfinis/django-generic-api-permissions/commit/d9655f17afc86e4c3d58858d639654ebf5495293))
+
+* chore(deps-dev): bump ruff from 0.3.5 to 0.4.6
+
+Bumps [ruff](https://github.com/astral-sh/ruff) from 0.3.5 to 0.4.6.
+- [Release notes](https://github.com/astral-sh/ruff/releases)
+- [Changelog](https://github.com/astral-sh/ruff/blob/main/CHANGELOG.md)
+- [Commits](https://github.com/astral-sh/ruff/compare/v0.3.5...v0.4.6)
+
+---
+updated-dependencies:
+- dependency-name: ruff
+  dependency-type: direct:development
+  update-type: version-update:semver-minor
+...
+
+Signed-off-by: dependabot[bot] &lt;support@github.com&gt; ([`c614700`](https://github.com/adfinis/django-generic-api-permissions/commit/c6147003d33376bb06aa27b408a00ff1ad8d5894))
+
+* chore(deps-dev): bump djangorestframework-jsonapi from 6.1.0 to 7.0.0
+
+Bumps [djangorestframework-jsonapi](https://github.com/django-json-api/django-rest-framework-json-api) from 6.1.0 to 7.0.0.
+- [Release notes](https://github.com/django-json-api/django-rest-framework-json-api/releases)
+- [Changelog](https://github.com/django-json-api/django-rest-framework-json-api/blob/main/CHANGELOG.md)
+- [Commits](https://github.com/django-json-api/django-rest-framework-json-api/compare/v6.1.0...v7.0.0)
+
+---
+updated-dependencies:
+- dependency-name: djangorestframework-jsonapi
+  dependency-type: direct:development
+  update-type: version-update:semver-major
+...
+
+Signed-off-by: dependabot[bot] &lt;support@github.com&gt; ([`abe4798`](https://github.com/adfinis/django-generic-api-permissions/commit/abe4798e6d81f1549d1caf6ff9e14dff5b682805))
+
+* chore(deps): bump django from 4.2.11 to 4.2.13
+
+Bumps [django](https://github.com/django/django) from 4.2.11 to 4.2.13.
+- [Commits](https://github.com/django/django/compare/4.2.11...4.2.13)
+
+---
+updated-dependencies:
+- dependency-name: django
+  dependency-type: direct:production
+  update-type: version-update:semver-patch
+...
+
+Signed-off-by: dependabot[bot] &lt;support@github.com&gt; ([`33362de`](https://github.com/adfinis/django-generic-api-permissions/commit/33362dec0465739b5506145a8d6ba7dad7970d10))
+
+* chore(deps-dev): bump pytest from 8.2.0 to 8.2.1
+
+Bumps [pytest](https://github.com/pytest-dev/pytest) from 8.2.0 to 8.2.1.
+- [Release notes](https://github.com/pytest-dev/pytest/releases)
+- [Changelog](https://github.com/pytest-dev/pytest/blob/main/CHANGELOG.rst)
+- [Commits](https://github.com/pytest-dev/pytest/compare/8.2.0...8.2.1)
+
+---
+updated-dependencies:
+- dependency-name: pytest
+  dependency-type: direct:development
+  update-type: version-update:semver-patch
+...
+
+Signed-off-by: dependabot[bot] &lt;support@github.com&gt; ([`90762a1`](https://github.com/adfinis/django-generic-api-permissions/commit/90762a161bf0de2d38c67c0e7f4882605f1b5742))
+
+* chore(deps-dev): bump pytest from 8.1.1 to 8.2.0
+
+Bumps [pytest](https://github.com/pytest-dev/pytest) from 8.1.1 to 8.2.0.
+- [Release notes](https://github.com/pytest-dev/pytest/releases)
+- [Changelog](https://github.com/pytest-dev/pytest/blob/main/CHANGELOG.rst)
+- [Commits](https://github.com/pytest-dev/pytest/compare/8.1.1...8.2.0)
+
+---
+updated-dependencies:
+- dependency-name: pytest
+  dependency-type: direct:development
+  update-type: version-update:semver-minor
+...
+
+Signed-off-by: dependabot[bot] &lt;support@github.com&gt; ([`aaae000`](https://github.com/adfinis/django-generic-api-permissions/commit/aaae0005de84ca778974d192b178705e86aee4cf))
+
+### Fix
+
+* fix(permissions): extend drf permission methods
+
+instead of calling permission in each specific method (create, etc.)
+call super in check_object_permission ([`00580d8`](https://github.com/adfinis/django-generic-api-permissions/commit/00580d83c4681df17e366e54942b00b9971ef945))
+
+### Unknown
+
+* Revert &#34;chore(deps): bump python-semantic-release/python-semantic-release&#34;
+
+This reverts commit d9655f17afc86e4c3d58858d639654ebf5495293. ([`18e447a`](https://github.com/adfinis/django-generic-api-permissions/commit/18e447a2fcc1e417270f9d16b5607f5b0ce7d675))
+
+
 ## v0.4.5 (2024-04-17)
 
 ### Chore
 
+* chore(release): 0.4.5
+
+Automatically generated by python-semantic-release ([`dc7e8e5`](https://github.com/adfinis/django-generic-api-permissions/commit/dc7e8e540c2f1318392f984a8d77c56bd8a99f7f))
+
 * chore: fix maintenance docs (#39) ([`9947377`](https://github.com/adfinis/django-generic-api-permissions/commit/99473779dca83ea5c4affe02f3625683e1b9e1c5))
 
 * chore: add CONTRIBUTING.md, allow running pytest directly in dev (#50)
 
 Co-authored-by: Fabio Ambauen &lt;1833932+open-dynaMIX@users.noreply.github.com&gt; ([`4fd4a34`](https://github.com/adfinis/django-generic-api-permissions/commit/4fd4a34b2e7982048f1a4db695a598d214667dcb))
 
 * chore(deps): bump django from 4.2.9 to 4.2.11
```

### Comparing `django_generic_api_permissions-0.4.5/LICENSE` & `django_generic_api_permissions-0.4.6/LICENSE`

 * *Files identical despite different names*

### Comparing `django_generic_api_permissions-0.4.5/README.md` & `django_generic_api_permissions-0.4.6/README.md`

 * *Files identical despite different names*

### Comparing `django_generic_api_permissions-0.4.5/generic_permissions/apps.py` & `django_generic_api_permissions-0.4.6/generic_permissions/apps.py`

 * *Files identical despite different names*

### Comparing `django_generic_api_permissions-0.4.5/generic_permissions/config.py` & `django_generic_api_permissions-0.4.6/generic_permissions/config.py`

 * *Files identical despite different names*

### Comparing `django_generic_api_permissions-0.4.5/generic_permissions/models.py` & `django_generic_api_permissions-0.4.6/generic_permissions/models.py`

 * *Files identical despite different names*

### Comparing `django_generic_api_permissions-0.4.5/generic_permissions/permissions.py` & `django_generic_api_permissions-0.4.6/generic_permissions/permissions.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,57 +1,56 @@
 from warnings import warn
 
 from django.core.exceptions import PermissionDenied
-from django.http import HttpResponse
 
 from .config import ObjectPermissionsConfig, PermissionsConfig
 
 permission_for = PermissionsConfig.decorator
 object_permission_for = ObjectPermissionsConfig.decorator
 
 
 class PermissionViewMixin:
-    def destroy(self, request, *args, **kwargs):
-        self._check_permissions(request)
-        instance = self.get_object()
-
-        # we do not call `super()` in order to not fetch the object twice.
-        self.perform_destroy(instance)
-        return HttpResponse(status=204)
-
-    def create(self, request, *args, **kwargs):
-        self._check_permissions(request)
-        return super().create(request, *args, **kwargs)
-
-    def update(self, request, *args, **kwargs):
-        self._check_permissions(request)
-        return super().update(request, *args, **kwargs)
-
     def _check_permissions(self, request):
+        """
+        Check if access to model is granted.
+
+        Raise PermissionDenied if configured permissions do not allow accesss to the model.
+        """
         for handler in PermissionsConfig.get_handlers(self.get_serializer().Meta.model):
             if not handler(request):
                 raise PermissionDenied()
 
-    def check_object_permissions(self, request, instance):
-        """Check if access to given object is granted.
-
-        Raise PermissionDenied if configured permissions do not allow
-        accesss to the object.
+    def check_permissions(self, request):
+        """
+        Overwrite default implementation to check DGAP permissions.
+        """
+        if request.method != "GET":
+            self._check_permissions(request)
+        super().check_permissions(request)
 
-        Called by get_object().
+    def _check_object_permissions(self, request, instance):
         """
-        if request.method == "GET":
-            return
+        Check if access to given object is granted.
 
+        Raise PermissionDenied if configured permissions do not allow accesss to the object.
+        """
         for handler in ObjectPermissionsConfig.get_handlers(
             self.get_serializer().Meta.model
         ):
             if not handler(request, instance):
                 raise PermissionDenied()
 
+    def check_object_permissions(self, request, instance):
+        """
+        Overwrite default implementation to check DGAP object permissions.
+        """
+        if request.method != "GET":
+            self._check_object_permissions(request, instance)
+        super().check_object_permissions(request, instance)
+
 
 class BasePermission:
     def __init__(self, *args, **kwargs):  # pragma: no cover
         super().__init__(*args, **kwargs)
         warn(
             DeprecationWarning(
                 "BasePermission is not required anymore. Just use "
```

### Comparing `django_generic_api_permissions-0.4.5/generic_permissions/validation.py` & `django_generic_api_permissions-0.4.6/generic_permissions/validation.py`

 * *Files identical despite different names*

### Comparing `django_generic_api_permissions-0.4.5/generic_permissions/views.py` & `django_generic_api_permissions-0.4.6/generic_permissions/views.py`

 * *Files identical despite different names*

### Comparing `django_generic_api_permissions-0.4.5/generic_permissions/visibilities.py` & `django_generic_api_permissions-0.4.6/generic_permissions/visibilities.py`

 * *Files identical despite different names*

### Comparing `django_generic_api_permissions-0.4.5/pyproject.toml` & `django_generic_api_permissions-0.4.6/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "django-generic-api-permissions"
-version = "0.4.5"
+version = "0.4.6"
 description="Generic API permissions and visibilities for Django"
 authors = ["Adfinis <indo@adfinis.com>"]
 readme = "README.md"
 repository = "https://github.com/adfinis/django-generic-api-permissions"
 classifiers = [
     "Development Status :: 4 - Beta",
     "Intended Audience :: Developers",
@@ -31,21 +31,21 @@
 [tool.poetry.dependencies]
 python = ">=3.8.1"
 django = ">=3.2"
 djangorestframework = "^3.14"
 
 [tool.poetry.dev-dependencies]
 black = "^23.12.1"
-ruff = "^0.3.5"
+ruff = "^0.4.6"
 
 [tool.poetry.group.djangorestframework-jsonapi]
 optional = true
 
 [tool.poetry.group.djangorestframework-jsonapi.dependencies]
-djangorestframework-jsonapi= "^6.1"
+djangorestframework-jsonapi= ">=6.1,<8.0"
 
 
 
 [tool.poetry.group.dev.dependencies]
 pytest = "^8.1.1"
 pytest-cov = "^5.0.0"
 pytest-mock = "^3.14.0"
```

### Comparing `django_generic_api_permissions-0.4.5/PKG-INFO` & `django_generic_api_permissions-0.4.6/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: django-generic-api-permissions
-Version: 0.4.5
+Version: 0.4.6
 Summary: Generic API permissions and visibilities for Django
 Home-page: https://github.com/adfinis/django-generic-api-permissions
 Author: Adfinis
 Author-email: indo@adfinis.com
 Requires-Python: >=3.8.1
 Classifier: Development Status :: 4 - Beta
 Classifier: Environment :: Web Environment
```

