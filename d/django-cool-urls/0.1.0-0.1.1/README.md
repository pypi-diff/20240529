# Comparing `tmp/django_cool_urls-0.1.0.tar.gz` & `tmp/django_cool_urls-0.1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "django_cool_urls-0.1.0.tar", max compression
+gzip compressed data, was "django_cool_urls-0.1.1.tar", max compression
```

## Comparing `django_cool_urls-0.1.0.tar` & `django_cool_urls-0.1.1.tar`

### file list

```diff
@@ -1,44 +1,44 @@
--rw-r--r--   0        0        0    35137 2024-05-20 17:39:21.436774 django_cool_urls-0.1.0/LICENSE
--rw-r--r--   0        0        0     2049 2024-05-24 22:30:43.308370 django_cool_urls-0.1.0/README.md
--rw-r--r--   0        0        0        0 2024-05-10 16:27:22.150287 django_cool_urls-0.1.0/cool_urls/__init__.py
--rw-r--r--   0        0        0     1301 2024-05-22 22:21:31.653847 django_cool_urls-0.1.0/cool_urls/admin.py
--rw-r--r--   0        0        0      390 2024-05-22 22:12:24.929492 django_cool_urls-0.1.0/cool_urls/apps.py
--rw-r--r--   0        0        0      205 2024-05-18 20:31:13.504062 django_cool_urls-0.1.0/cool_urls/coolers/__init__.py
--rw-r--r--   0        0        0     2509 2024-05-19 13:38:55.987287 django_cool_urls-0.1.0/cool_urls/coolers/base.py
--rw-r--r--   0        0        0       94 2024-05-10 16:27:22.210288 django_cool_urls-0.1.0/cool_urls/coolers/exceptions.py
--rw-r--r--   0        0        0     1846 2024-05-19 22:26:48.473493 django_cool_urls-0.1.0/cool_urls/coolers/files.py
--rw-r--r--   0        0        0     4162 2024-05-27 22:50:53.337388 django_cool_urls-0.1.0/cool_urls/coolers/pages.py
--rw-r--r--   0        0        0     6633 2024-05-27 22:50:53.337388 django_cool_urls-0.1.0/cool_urls/coolers/videos.py
--rw-r--r--   0        0        0      698 2024-05-14 21:47:23.096123 django_cool_urls-0.1.0/cool_urls/logging.py
--rw-r--r--   0        0        0     1033 2024-05-14 22:14:29.447255 django_cool_urls-0.1.0/cool_urls/management/commands/check_cool_urls.py
--rw-r--r--   0        0        0     1091 2024-05-19 20:51:50.141237 django_cool_urls-0.1.0/cool_urls/management/commands/cool_url.py
--rw-r--r--   0        0        0      398 2024-05-20 17:37:34.605478 django_cool_urls-0.1.0/cool_urls/management/commands/cool_urls.py
--rw-r--r--   0        0        0      699 2024-05-27 22:50:53.337388 django_cool_urls-0.1.0/cool_urls/management/commands/scratch.py
--rw-r--r--   0        0        0     5274 2024-05-24 22:20:53.158262 django_cool_urls-0.1.0/cool_urls/migrations/0001_initial.py
--rw-r--r--   0        0        0        0 2024-05-10 16:27:22.153621 django_cool_urls-0.1.0/cool_urls/migrations/__init__.py
--rw-r--r--   0        0        0     5610 2024-05-24 22:15:48.614829 django_cool_urls-0.1.0/cool_urls/models.py
--rw-r--r--   0        0        0      434 2024-05-13 20:35:59.913282 django_cool_urls-0.1.0/cool_urls/receivers.py
--rw-r--r--   0        0        0      131 2024-05-14 19:53:53.742788 django_cool_urls-0.1.0/cool_urls/signals.py
--rw-r--r--   0        0        0      387 2024-05-27 22:50:53.337388 django_cool_urls-0.1.0/cool_urls/templates/cool_urls/videos/local.html
--rw-r--r--   0        0        0       64 2024-05-27 22:50:53.337388 django_cool_urls-0.1.0/cool_urls/templates/cool_urls/videos/remote/default.html
--rw-r--r--   0        0        0      256 2024-05-27 22:50:53.337388 django_cool_urls-0.1.0/cool_urls/templates/cool_urls/videos/remote/vimeo.html
--rw-r--r--   0        0        0      330 2024-05-27 22:50:53.337388 django_cool_urls-0.1.0/cool_urls/templates/cool_urls/videos/remote/youtube.html
--rw-r--r--   0        0        0        0 2024-05-10 16:27:22.193621 django_cool_urls-0.1.0/cool_urls/templatetags/__init__.py
--rw-r--r--   0        0        0     1705 2024-05-24 23:19:59.585191 django_cool_urls-0.1.0/cool_urls/templatetags/cool_urls.py
--rw-r--r--   0        0        0        0 2024-05-14 19:53:53.742788 django_cool_urls-0.1.0/cool_urls/tests/__init__.py
--rw-r--r--   0        0        0        0 2024-05-14 19:53:53.742788 django_cool_urls-0.1.0/cool_urls/tests/coolers/__init__.py
--rw-r--r--   0        0        0     3134 2024-05-19 13:34:07.072132 django_cool_urls-0.1.0/cool_urls/tests/coolers/test_base.py
--rw-r--r--   0        0        0     2353 2024-05-18 21:19:44.916566 django_cool_urls-0.1.0/cool_urls/tests/coolers/test_files.py
--rw-r--r--   0        0        0     6140 2024-05-19 13:33:59.482028 django_cool_urls-0.1.0/cool_urls/tests/coolers/test_pages.py
--rw-r--r--   0        0        0     8145 2024-05-27 22:50:53.337388 django_cool_urls-0.1.0/cool_urls/tests/coolers/test_videos.py
--rw-r--r--   0        0        0        0 2024-05-14 22:14:51.797637 django_cool_urls-0.1.0/cool_urls/tests/management/__init__.py
--rw-r--r--   0        0        0        0 2024-05-14 22:14:58.677751 django_cool_urls-0.1.0/cool_urls/tests/management/commands/__init__.py
--rw-r--r--   0        0        0     2639 2024-05-18 21:19:44.909899 django_cool_urls-0.1.0/cool_urls/tests/management/commands/test_check_cool_urls.py
--rw-r--r--   0        0        0     1547 2024-05-18 21:19:44.866565 django_cool_urls-0.1.0/cool_urls/tests/management/commands/test_cool_url.py
--rw-r--r--   0        0        0      770 2024-05-22 22:24:36.311281 django_cool_urls-0.1.0/cool_urls/tests/test_admin.py
--rw-r--r--   0        0        0     5817 2024-05-28 01:35:48.025093 django_cool_urls-0.1.0/cool_urls/tests/test_functional.py
--rw-r--r--   0        0        0     4822 2024-05-18 21:19:44.893232 django_cool_urls-0.1.0/cool_urls/tests/test_models.py
--rw-r--r--   0        0        0      364 2024-05-18 21:19:44.959899 django_cool_urls-0.1.0/cool_urls/tests/test_receivers.py
--rw-r--r--   0        0        0     3110 2024-05-24 23:13:59.126859 django_cool_urls-0.1.0/cool_urls/tests/test_templatetags.py
--rw-r--r--   0        0        0     1576 2024-05-28 02:28:26.578013 django_cool_urls-0.1.0/pyproject.toml
--rw-r--r--   0        0        0     2750 1970-01-01 00:00:00.000000 django_cool_urls-0.1.0/PKG-INFO
+-rw-r--r--   0        0        0    35137 2024-05-20 17:39:21.436774 django_cool_urls-0.1.1/LICENSE
+-rw-r--r--   0        0        0     2049 2024-05-24 22:30:43.308370 django_cool_urls-0.1.1/README.md
+-rw-r--r--   0        0        0        0 2024-05-10 16:27:22.150287 django_cool_urls-0.1.1/cool_urls/__init__.py
+-rw-r--r--   0        0        0     1301 2024-05-22 22:21:31.653847 django_cool_urls-0.1.1/cool_urls/admin.py
+-rw-r--r--   0        0        0      390 2024-05-22 22:12:24.929492 django_cool_urls-0.1.1/cool_urls/apps.py
+-rw-r--r--   0        0        0      205 2024-05-18 20:31:13.504062 django_cool_urls-0.1.1/cool_urls/coolers/__init__.py
+-rw-r--r--   0        0        0     2509 2024-05-19 13:38:55.987287 django_cool_urls-0.1.1/cool_urls/coolers/base.py
+-rw-r--r--   0        0        0       94 2024-05-10 16:27:22.210288 django_cool_urls-0.1.1/cool_urls/coolers/exceptions.py
+-rw-r--r--   0        0        0     1846 2024-05-19 22:26:48.473493 django_cool_urls-0.1.1/cool_urls/coolers/files.py
+-rw-r--r--   0        0        0     4162 2024-05-27 22:50:53.337388 django_cool_urls-0.1.1/cool_urls/coolers/pages.py
+-rw-r--r--   0        0        0     6633 2024-05-27 22:50:53.337388 django_cool_urls-0.1.1/cool_urls/coolers/videos.py
+-rw-r--r--   0        0        0      698 2024-05-14 21:47:23.096123 django_cool_urls-0.1.1/cool_urls/logging.py
+-rw-r--r--   0        0        0     1596 2024-05-28 18:42:05.710063 django_cool_urls-0.1.1/cool_urls/management/commands/check_cool_urls.py
+-rw-r--r--   0        0        0     1091 2024-05-19 20:51:50.141237 django_cool_urls-0.1.1/cool_urls/management/commands/cool_url.py
+-rw-r--r--   0        0        0      398 2024-05-20 17:37:34.605478 django_cool_urls-0.1.1/cool_urls/management/commands/cool_urls.py
+-rw-r--r--   0        0        0      699 2024-05-27 22:50:53.337388 django_cool_urls-0.1.1/cool_urls/management/commands/scratch.py
+-rw-r--r--   0        0        0     5274 2024-05-24 22:20:53.158262 django_cool_urls-0.1.1/cool_urls/migrations/0001_initial.py
+-rw-r--r--   0        0        0        0 2024-05-10 16:27:22.153621 django_cool_urls-0.1.1/cool_urls/migrations/__init__.py
+-rw-r--r--   0        0        0     5610 2024-05-24 22:15:48.614829 django_cool_urls-0.1.1/cool_urls/models.py
+-rw-r--r--   0        0        0      434 2024-05-13 20:35:59.913282 django_cool_urls-0.1.1/cool_urls/receivers.py
+-rw-r--r--   0        0        0      131 2024-05-14 19:53:53.742788 django_cool_urls-0.1.1/cool_urls/signals.py
+-rw-r--r--   0        0        0      387 2024-05-27 22:50:53.337388 django_cool_urls-0.1.1/cool_urls/templates/cool_urls/videos/local.html
+-rw-r--r--   0        0        0       64 2024-05-27 22:50:53.337388 django_cool_urls-0.1.1/cool_urls/templates/cool_urls/videos/remote/default.html
+-rw-r--r--   0        0        0      256 2024-05-27 22:50:53.337388 django_cool_urls-0.1.1/cool_urls/templates/cool_urls/videos/remote/vimeo.html
+-rw-r--r--   0        0        0      330 2024-05-27 22:50:53.337388 django_cool_urls-0.1.1/cool_urls/templates/cool_urls/videos/remote/youtube.html
+-rw-r--r--   0        0        0        0 2024-05-10 16:27:22.193621 django_cool_urls-0.1.1/cool_urls/templatetags/__init__.py
+-rw-r--r--   0        0        0     1705 2024-05-24 23:19:59.585191 django_cool_urls-0.1.1/cool_urls/templatetags/cool_urls.py
+-rw-r--r--   0        0        0        0 2024-05-14 19:53:53.742788 django_cool_urls-0.1.1/cool_urls/tests/__init__.py
+-rw-r--r--   0        0        0        0 2024-05-14 19:53:53.742788 django_cool_urls-0.1.1/cool_urls/tests/coolers/__init__.py
+-rw-r--r--   0        0        0     3134 2024-05-19 13:34:07.072132 django_cool_urls-0.1.1/cool_urls/tests/coolers/test_base.py
+-rw-r--r--   0        0        0     2353 2024-05-18 21:19:44.916566 django_cool_urls-0.1.1/cool_urls/tests/coolers/test_files.py
+-rw-r--r--   0        0        0     6140 2024-05-19 13:33:59.482028 django_cool_urls-0.1.1/cool_urls/tests/coolers/test_pages.py
+-rw-r--r--   0        0        0     8145 2024-05-27 22:50:53.337388 django_cool_urls-0.1.1/cool_urls/tests/coolers/test_videos.py
+-rw-r--r--   0        0        0        0 2024-05-14 22:14:51.797637 django_cool_urls-0.1.1/cool_urls/tests/management/__init__.py
+-rw-r--r--   0        0        0        0 2024-05-14 22:14:58.677751 django_cool_urls-0.1.1/cool_urls/tests/management/commands/__init__.py
+-rw-r--r--   0        0        0     6918 2024-05-28 18:47:29.078427 django_cool_urls-0.1.1/cool_urls/tests/management/commands/test_check_cool_urls.py
+-rw-r--r--   0        0        0     1547 2024-05-18 21:19:44.866565 django_cool_urls-0.1.1/cool_urls/tests/management/commands/test_cool_url.py
+-rw-r--r--   0        0        0      770 2024-05-22 22:24:36.311281 django_cool_urls-0.1.1/cool_urls/tests/test_admin.py
+-rw-r--r--   0        0        0     5817 2024-05-28 01:35:48.025093 django_cool_urls-0.1.1/cool_urls/tests/test_functional.py
+-rw-r--r--   0        0        0     4822 2024-05-18 21:19:44.893232 django_cool_urls-0.1.1/cool_urls/tests/test_models.py
+-rw-r--r--   0        0        0      364 2024-05-18 21:19:44.959899 django_cool_urls-0.1.1/cool_urls/tests/test_receivers.py
+-rw-r--r--   0        0        0     3110 2024-05-24 23:13:59.126859 django_cool_urls-0.1.1/cool_urls/tests/test_templatetags.py
+-rw-r--r--   0        0        0     1586 2024-05-28 18:57:02.607252 django_cool_urls-0.1.1/pyproject.toml
+-rw-r--r--   0        0        0     2727 1970-01-01 00:00:00.000000 django_cool_urls-0.1.1/PKG-INFO
```

### Comparing `django_cool_urls-0.1.0/LICENSE` & `django_cool_urls-0.1.1/LICENSE`

 * *Files identical despite different names*

### Comparing `django_cool_urls-0.1.0/README.md` & `django_cool_urls-0.1.1/README.md`

 * *Files identical despite different names*

### Comparing `django_cool_urls-0.1.0/cool_urls/admin.py` & `django_cool_urls-0.1.1/cool_urls/admin.py`

 * *Files identical despite different names*

### Comparing `django_cool_urls-0.1.0/cool_urls/coolers/base.py` & `django_cool_urls-0.1.1/cool_urls/coolers/base.py`

 * *Files identical despite different names*

### Comparing `django_cool_urls-0.1.0/cool_urls/coolers/files.py` & `django_cool_urls-0.1.1/cool_urls/coolers/files.py`

 * *Files identical despite different names*

### Comparing `django_cool_urls-0.1.0/cool_urls/coolers/pages.py` & `django_cool_urls-0.1.1/cool_urls/coolers/pages.py`

 * *Files identical despite different names*

### Comparing `django_cool_urls-0.1.0/cool_urls/coolers/videos.py` & `django_cool_urls-0.1.1/cool_urls/coolers/videos.py`

 * *Files identical despite different names*

### Comparing `django_cool_urls-0.1.0/cool_urls/logging.py` & `django_cool_urls-0.1.1/cool_urls/logging.py`

 * *Files identical despite different names*

### Comparing `django_cool_urls-0.1.0/cool_urls/management/commands/check_cool_urls.py` & `django_cool_urls-0.1.1/cool_urls/management/commands/check_cool_urls.py`

 * *Files 26% similar despite different names*

```diff
@@ -1,8 +1,12 @@
+from datetime import timedelta
+
+from django.conf import settings
 from django.core.management.base import BaseCommand
+from django.utils import timezone
 
 import httpx
 
 from ...logging import Loggable
 from ...models import CoolUrl
 
 
@@ -11,20 +15,32 @@
     Go through all CoolUrl entries and check if the site is still responding
     properly.  If not, set `show_local` to `True` so we prefer the local copy.
 
     This is the sort of thing you'd probably want to run in a weekly cron or
     something.
     """
 
+    # The time during which you don't want to re-check a URL
+    WINDOW = timedelta(days=getattr(settings, "COOL_URLS_CHECK_WINDOW", 30))
+
     def handle(self, *args, **options):
-        urls = CoolUrl.objects.filter(is_ready=True, show_local=False)
-        for cool_url in urls.iterator():
-            code = httpx.get(cool_url.url).status_code
-            if code != httpx.codes.OK:
+        window = timezone.now() - self.WINDOW
+        urls = CoolUrl.objects.filter(is_ready=True, show_local=False).exclude(
+            last_http_check_time__gt=window
+        )
+
+        for cu in urls.iterator():
+            update_fields = ["last_http_check_state", "last_http_check_time"]
+            cu.last_http_check_state = httpx.get(cu.url).status_code
+            cu.last_http_check_time = timezone.now()
+
+            if cu.last_http_check_state != httpx.codes.OK:
                 self.logger.info(
                     "URL %s had an HTTP response of %s, so we're marking "
                     "it to render the local archived copy.",
-                    cool_url.url,
-                    code,
+                    cu.url,
+                    cu.last_http_check_state,
                 )
-                cool_url.show_local = True
-                cool_url.save(update_fields=("show_local",))
+                cu.show_local = True
+                update_fields.append("show_local")
+
+            cu.save(update_fields=tuple(update_fields))
```

### Comparing `django_cool_urls-0.1.0/cool_urls/management/commands/cool_url.py` & `django_cool_urls-0.1.1/cool_urls/management/commands/cool_url.py`

 * *Files identical despite different names*

### Comparing `django_cool_urls-0.1.0/cool_urls/management/commands/scratch.py` & `django_cool_urls-0.1.1/cool_urls/management/commands/scratch.py`

 * *Files identical despite different names*

### Comparing `django_cool_urls-0.1.0/cool_urls/migrations/0001_initial.py` & `django_cool_urls-0.1.1/cool_urls/migrations/0001_initial.py`

 * *Files identical despite different names*

### Comparing `django_cool_urls-0.1.0/cool_urls/models.py` & `django_cool_urls-0.1.1/cool_urls/models.py`

 * *Files identical despite different names*

### Comparing `django_cool_urls-0.1.0/cool_urls/templatetags/cool_urls.py` & `django_cool_urls-0.1.1/cool_urls/templatetags/cool_urls.py`

 * *Files identical despite different names*

### Comparing `django_cool_urls-0.1.0/cool_urls/tests/coolers/test_base.py` & `django_cool_urls-0.1.1/cool_urls/tests/coolers/test_base.py`

 * *Files identical despite different names*

### Comparing `django_cool_urls-0.1.0/cool_urls/tests/coolers/test_files.py` & `django_cool_urls-0.1.1/cool_urls/tests/coolers/test_files.py`

 * *Files identical despite different names*

### Comparing `django_cool_urls-0.1.0/cool_urls/tests/coolers/test_pages.py` & `django_cool_urls-0.1.1/cool_urls/tests/coolers/test_pages.py`

 * *Files identical despite different names*

### Comparing `django_cool_urls-0.1.0/cool_urls/tests/coolers/test_videos.py` & `django_cool_urls-0.1.1/cool_urls/tests/coolers/test_videos.py`

 * *Files identical despite different names*

### Comparing `django_cool_urls-0.1.0/cool_urls/tests/management/commands/test_cool_url.py` & `django_cool_urls-0.1.1/cool_urls/tests/management/commands/test_cool_url.py`

 * *Files identical despite different names*

### Comparing `django_cool_urls-0.1.0/cool_urls/tests/test_admin.py` & `django_cool_urls-0.1.1/cool_urls/tests/test_admin.py`

 * *Files identical despite different names*

### Comparing `django_cool_urls-0.1.0/cool_urls/tests/test_functional.py` & `django_cool_urls-0.1.1/cool_urls/tests/test_functional.py`

 * *Files identical despite different names*

### Comparing `django_cool_urls-0.1.0/cool_urls/tests/test_models.py` & `django_cool_urls-0.1.1/cool_urls/tests/test_models.py`

 * *Files identical despite different names*

### Comparing `django_cool_urls-0.1.0/cool_urls/tests/test_templatetags.py` & `django_cool_urls-0.1.1/cool_urls/tests/test_templatetags.py`

 * *Files identical despite different names*

### Comparing `django_cool_urls-0.1.0/pyproject.toml` & `django_cool_urls-0.1.1/pyproject.toml`

 * *Files 9% similar despite different names*

```diff
@@ -1,28 +1,29 @@
 [tool.poetry]
 name = "django-cool-urls"
-version = "0.1.0"
+version = "0.1.1"
 description = "Freeze outgoing links in time so that your site never 404s on external pages"
 authors = ["Daniel Quinn <code@danielquinn.org>"]
 license = "AGPL-3.0-or-later"
 readme = "README.md"
 packages = [
     { include = "cool_urls" }
 ]
 
 [tool.poetry.dependencies]
 python = "^3.11"
 Django = ">=3.2"
-yt-dlp = {version = "^2024.4.9", optional = true}
 httpx = "^0.27.0"
+yt-dlp = {version = "*", optional = true}
 
 [tool.poetry.group.dev.dependencies]
-ruff = "^0.4.4"
 coverage = "^7.5.1"
+freezegun = "^1.5.1"
 mkdocs-techdocs-core = "^1.3.5"
+ruff = "^0.4.4"
 
 [tool.poetry.extras]
 embed = ["yt-dlp"]
 
 
 [build-system]
 requires = ["poetry-core"]
@@ -43,15 +44,15 @@
 case-sensitive = true
 lines-after-imports = 2
 lines-between-types = 1
 combine-as-imports = true
 split-on-trailing-comma = true
 known-first-party = [
   "cool_urls",
-  "example",
+  "core",
 ]
 section-order = [
   "future",
   "standard-library",
   "django",
   "third-party",
   "first-party",
```

### Comparing `django_cool_urls-0.1.0/PKG-INFO` & `django_cool_urls-0.1.1/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,23 +1,23 @@
 Metadata-Version: 2.1
 Name: django-cool-urls
-Version: 0.1.0
+Version: 0.1.1
 Summary: Freeze outgoing links in time so that your site never 404s on external pages
 License: AGPL-3.0-or-later
 Author: Daniel Quinn
 Author-email: code@danielquinn.org
 Requires-Python: >=3.11,<4.0
 Classifier: License :: OSI Approved :: GNU Affero General Public License v3 or later (AGPLv3+)
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: Python :: 3.12
 Provides-Extra: embed
 Requires-Dist: Django (>=3.2)
 Requires-Dist: httpx (>=0.27.0,<0.28.0)
-Requires-Dist: yt-dlp (>=2024.4.9,<2025.0.0) ; extra == "embed"
+Requires-Dist: yt-dlp ; extra == "embed"
 Description-Content-Type: text/markdown
 
 ![logo.png](https://gitlab.com/danielquinn/django-cool-urls/-/raw/master/docs/logo.png)
 
 # Django Cool URLs
 
 Tim Berners-Lee is credited with saying that "cool URLs don't change", but
```

#### html2text {}

```diff
@@ -1,33 +1,33 @@
-Metadata-Version: 2.1 Name: django-cool-urls Version: 0.1.0 Summary: Freeze
+Metadata-Version: 2.1 Name: django-cool-urls Version: 0.1.1 Summary: Freeze
 outgoing links in time so that your site never 404s on external pages License:
 AGPL-3.0-or-later Author: Daniel Quinn Author-email: code@danielquinn.org
 Requires-Python: >=3.11,<4.0 Classifier: License :: OSI Approved :: GNU Affero
 General Public License v3 or later (AGPLv3+) Classifier: Programming Language
 :: Python :: 3 Classifier: Programming Language :: Python :: 3.11 Classifier:
 Programming Language :: Python :: 3.12 Provides-Extra: embed Requires-Dist:
-Django (>=3.2) Requires-Dist: httpx (>=0.27.0,<0.28.0) Requires-Dist: yt-dlp
-(>=2024.4.9,<2025.0.0) ; extra == "embed" Description-Content-Type: text/
-markdown ![logo.png](https://gitlab.com/danielquinn/django-cool-urls/-/raw/
-master/docs/logo.png) # Django Cool URLs Tim Berners-Lee is credited with
-saying that "cool URLs don't change", but sadly that's just not the case. Cool
-URLs are changing all the time because the people who run those sites are
-moving stuff around or just deleting whole pages and domains. If you have a
-long-running site full of links like a blog however, this means that over time
-your site can be pointing to a lot of dead links, which is bad for your SEO.
-It's also annoying when you're looking over a post from 10 years ago that says
-something like "[this](.) is some really nice work" and that link 404s. With
-`django-cool-urls`, you can link to whatever you like and the state of that
-page is captured from the moment you linked to it. If the page ever disappears
-from the web, you can automatically switch over to the local copy. All you need
-to do is switch from doing this: ```html _N_i_f_t_y_! ``` to this: ```html _N_i_f_t_y_! ```
-If that page ever 404s, your site will switch to showing the locally cached
-version. Think of it like your own private [archive.org](https://archive.org/).
-Currently, this project supports caching *most* pages (see the [Caveats](https:
-//danielquinn.gitlab.io/django-cool-urls/caveats/) page) as well as embedded
+Django (>=3.2) Requires-Dist: httpx (>=0.27.0,<0.28.0) Requires-Dist: yt-dlp ;
+extra == "embed" Description-Content-Type: text/markdown ![logo.png](https://
+gitlab.com/danielquinn/django-cool-urls/-/raw/master/docs/logo.png) # Django
+Cool URLs Tim Berners-Lee is credited with saying that "cool URLs don't
+change", but sadly that's just not the case. Cool URLs are changing all the
+time because the people who run those sites are moving stuff around or just
+deleting whole pages and domains. If you have a long-running site full of links
+like a blog however, this means that over time your site can be pointing to a
+lot of dead links, which is bad for your SEO. It's also annoying when you're
+looking over a post from 10 years ago that says something like "[this](.) is
+some really nice work" and that link 404s. With `django-cool-urls`, you can
+link to whatever you like and the state of that page is captured from the
+moment you linked to it. If the page ever disappears from the web, you can
+automatically switch over to the local copy. All you need to do is switch from
+doing this: ```html _N_i_f_t_y_! ``` to this: ```html _N_i_f_t_y_! ``` If that page ever
+404s, your site will switch to showing the locally cached version. Think of it
+like your own private [archive.org](https://archive.org/). Currently, this
+project supports caching *most* pages (see the [Caveats](https://
+danielquinn.gitlab.io/django-cool-urls/caveats/) page) as well as embedded
 video from YouTube, Vimeo, and Instagram. * [Official documentation](https://
 danielquinn.gitlab.io/django-cool-urls/) * [Installation](https://
 danielquinn.gitlab.io/django-cool-urls/installation/) * [Configuration](https:/
 /danielquinn.gitlab.io/django-cool-urls/configuration/) * [How to use it]
 (https://danielquinn.gitlab.io/django-cool-urls/how-to-use-it/) * [Caveats &
 troubleshooting](https://danielquinn.gitlab.io/django-cool-urls/caveats/) *
 [Development](https://danielquinn.gitlab.io/django-cool-urls/development/) *
```

