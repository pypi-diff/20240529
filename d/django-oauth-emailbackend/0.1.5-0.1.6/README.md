# Comparing `tmp/django_oauth_emailbackend-0.1.5.tar.gz` & `tmp/django_oauth_emailbackend-0.1.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "django_oauth_emailbackend-0.1.5.tar", last modified: Tue May 28 11:17:57 2024, max compression
+gzip compressed data, was "django_oauth_emailbackend-0.1.6.tar", last modified: Wed May 29 00:00:02 2024, max compression
```

## Comparing `django_oauth_emailbackend-0.1.5.tar` & `django_oauth_emailbackend-0.1.6.tar`

### file list

```diff
@@ -1,44 +1,44 @@
-drwxr-xr-x   0 odop       (501) staff       (20)        0 2024-05-28 11:17:57.670231 django_oauth_emailbackend-0.1.5/
--rw-r--r--   0 odop       (501) staff       (20)     1066 2024-05-28 11:17:54.000000 django_oauth_emailbackend-0.1.5/LICENSE
--rw-r--r--   0 odop       (501) staff       (20)      142 2024-05-28 11:17:54.000000 django_oauth_emailbackend-0.1.5/MANIFEST.in
--rw-r--r--   0 odop       (501) staff       (20)     3517 2024-05-28 11:17:57.670044 django_oauth_emailbackend-0.1.5/PKG-INFO
--rw-r--r--   0 odop       (501) staff       (20)     2410 2024-05-28 11:17:54.000000 django_oauth_emailbackend-0.1.5/README.md
--rw-r--r--   0 odop       (501) staff       (20)     1004 2024-05-28 11:17:54.000000 django_oauth_emailbackend-0.1.5/pyproject.toml
--rw-r--r--   0 odop       (501) staff       (20)       38 2024-05-28 11:17:57.670274 django_oauth_emailbackend-0.1.5/setup.cfg
-drwxr-xr-x   0 odop       (501) staff       (20)        0 2024-05-28 11:17:57.664703 django_oauth_emailbackend-0.1.5/src/
-drwxr-xr-x   0 odop       (501) staff       (20)        0 2024-05-28 11:17:57.669807 django_oauth_emailbackend-0.1.5/src/django_oauth_emailbackend.egg-info/
--rw-r--r--   0 odop       (501) staff       (20)     3517 2024-05-28 11:17:57.000000 django_oauth_emailbackend-0.1.5/src/django_oauth_emailbackend.egg-info/PKG-INFO
--rw-r--r--   0 odop       (501) staff       (20)     1135 2024-05-28 11:17:57.000000 django_oauth_emailbackend-0.1.5/src/django_oauth_emailbackend.egg-info/SOURCES.txt
--rw-r--r--   0 odop       (501) staff       (20)        1 2024-05-28 11:17:57.000000 django_oauth_emailbackend-0.1.5/src/django_oauth_emailbackend.egg-info/dependency_links.txt
--rw-r--r--   0 odop       (501) staff       (20)      119 2024-05-28 11:17:57.000000 django_oauth_emailbackend-0.1.5/src/django_oauth_emailbackend.egg-info/requires.txt
--rw-r--r--   0 odop       (501) staff       (20)       19 2024-05-28 11:17:57.000000 django_oauth_emailbackend-0.1.5/src/django_oauth_emailbackend.egg-info/top_level.txt
-drwxr-xr-x   0 odop       (501) staff       (20)        0 2024-05-28 11:17:57.668472 django_oauth_emailbackend-0.1.5/src/oauth_emailbackend/
--rw-r--r--   0 odop       (501) staff       (20)        0 2024-02-27 01:20:37.000000 django_oauth_emailbackend-0.1.5/src/oauth_emailbackend/__init__.py
--rw-r--r--   0 odop       (501) staff       (20)     4930 2024-05-28 11:05:53.000000 django_oauth_emailbackend-0.1.5/src/oauth_emailbackend/admin.py
--rw-r--r--   0 odop       (501) staff       (20)     1693 2024-03-28 12:13:39.000000 django_oauth_emailbackend-0.1.5/src/oauth_emailbackend/apps.py
--rw-r--r--   0 odop       (501) staff       (20)     8389 2024-05-28 00:47:57.000000 django_oauth_emailbackend-0.1.5/src/oauth_emailbackend/backends.py
--rw-r--r--   0 odop       (501) staff       (20)     1945 2024-05-28 11:03:44.000000 django_oauth_emailbackend-0.1.5/src/oauth_emailbackend/forms.py
-drwxr-xr-x   0 odop       (501) staff       (20)        0 2024-05-28 11:17:57.668619 django_oauth_emailbackend-0.1.5/src/oauth_emailbackend/management/
--rw-r--r--   0 odop       (501) staff       (20)        0 2024-05-28 09:55:42.000000 django_oauth_emailbackend-0.1.5/src/oauth_emailbackend/management/__init__.py
-drwxr-xr-x   0 odop       (501) staff       (20)        0 2024-05-28 11:17:57.668734 django_oauth_emailbackend-0.1.5/src/oauth_emailbackend/management/commands/
--rw-r--r--   0 odop       (501) staff       (20)        0 2024-04-04 05:03:10.000000 django_oauth_emailbackend-0.1.5/src/oauth_emailbackend/management/commands/__init__.py
-drwxr-xr-x   0 odop       (501) staff       (20)        0 2024-05-28 11:17:57.669021 django_oauth_emailbackend-0.1.5/src/oauth_emailbackend/migrations/
--rw-r--r--   0 odop       (501) staff       (20)     5913 2024-05-28 05:32:50.000000 django_oauth_emailbackend-0.1.5/src/oauth_emailbackend/migrations/0001_initial.py
--rw-r--r--   0 odop       (501) staff       (20)        0 2024-02-27 01:20:37.000000 django_oauth_emailbackend-0.1.5/src/oauth_emailbackend/migrations/__init__.py
--rw-r--r--   0 odop       (501) staff       (20)     7671 2024-05-28 11:00:07.000000 django_oauth_emailbackend-0.1.5/src/oauth_emailbackend/models.py
-drwxr-xr-x   0 odop       (501) staff       (20)        0 2024-05-28 11:17:57.669280 django_oauth_emailbackend-0.1.5/src/oauth_emailbackend/providers/
--rw-r--r--   0 odop       (501) staff       (20)     3712 2024-04-05 06:16:20.000000 django_oauth_emailbackend-0.1.5/src/oauth_emailbackend/providers/__init__.py
--rw-r--r--   0 odop       (501) staff       (20)     7687 2024-05-28 01:00:07.000000 django_oauth_emailbackend-0.1.5/src/oauth_emailbackend/providers/gmail.py
--rw-r--r--   0 odop       (501) staff       (20)     5066 2024-05-28 00:18:23.000000 django_oauth_emailbackend-0.1.5/src/oauth_emailbackend/tasks.py
-drwxr-xr-x   0 odop       (501) staff       (20)        0 2024-05-28 11:17:57.665326 django_oauth_emailbackend-0.1.5/src/oauth_emailbackend/templates/
-drwxr-xr-x   0 odop       (501) staff       (20)        0 2024-05-28 11:17:57.665192 django_oauth_emailbackend-0.1.5/src/oauth_emailbackend/templates/admin/
-drwxr-xr-x   0 odop       (501) staff       (20)        0 2024-05-28 11:17:57.665248 django_oauth_emailbackend-0.1.5/src/oauth_emailbackend/templates/admin/oauth_emailbackend/
-drwxr-xr-x   0 odop       (501) staff       (20)        0 2024-05-28 11:17:57.669459 django_oauth_emailbackend-0.1.5/src/oauth_emailbackend/templates/admin/oauth_emailbackend/emailclient/
--rw-r--r--   0 odop       (501) staff       (20)     3957 2024-04-05 05:22:12.000000 django_oauth_emailbackend-0.1.5/src/oauth_emailbackend/templates/admin/oauth_emailbackend/emailclient/change_form.html
-drwxr-xr-x   0 odop       (501) staff       (20)        0 2024-05-28 11:17:57.669616 django_oauth_emailbackend-0.1.5/src/oauth_emailbackend/templates/oauth_emailbackend/
--rw-r--r--   0 odop       (501) staff       (20)     3101 2024-04-05 06:19:46.000000 django_oauth_emailbackend-0.1.5/src/oauth_emailbackend/templates/oauth_emailbackend/callback.html
--rw-r--r--   0 odop       (501) staff       (20)        0 2024-05-28 10:06:11.000000 django_oauth_emailbackend-0.1.5/src/oauth_emailbackend/test.html
--rw-r--r--   0 odop       (501) staff       (20)       60 2024-02-27 01:20:37.000000 django_oauth_emailbackend-0.1.5/src/oauth_emailbackend/tests.py
--rw-r--r--   0 odop       (501) staff       (20)      400 2024-03-29 11:43:15.000000 django_oauth_emailbackend-0.1.5/src/oauth_emailbackend/urls.py
--rw-r--r--   0 odop       (501) staff       (20)     8340 2024-05-28 08:00:06.000000 django_oauth_emailbackend-0.1.5/src/oauth_emailbackend/utils.py
--rw-r--r--   0 odop       (501) staff       (20)     1954 2024-04-05 06:28:05.000000 django_oauth_emailbackend-0.1.5/src/oauth_emailbackend/views.py
+drwxr-xr-x   0 odop       (501) staff       (20)        0 2024-05-29 00:00:02.870036 django_oauth_emailbackend-0.1.6/
+-rw-r--r--   0 odop       (501) staff       (20)     1066 2024-05-28 23:59:59.000000 django_oauth_emailbackend-0.1.6/LICENSE
+-rw-r--r--   0 odop       (501) staff       (20)      142 2024-05-28 23:59:59.000000 django_oauth_emailbackend-0.1.6/MANIFEST.in
+-rw-r--r--   0 odop       (501) staff       (20)     3511 2024-05-29 00:00:02.869820 django_oauth_emailbackend-0.1.6/PKG-INFO
+-rw-r--r--   0 odop       (501) staff       (20)     2410 2024-05-28 23:59:59.000000 django_oauth_emailbackend-0.1.6/README.md
+-rw-r--r--   0 odop       (501) staff       (20)      998 2024-05-28 23:59:59.000000 django_oauth_emailbackend-0.1.6/pyproject.toml
+-rw-r--r--   0 odop       (501) staff       (20)       38 2024-05-29 00:00:02.870076 django_oauth_emailbackend-0.1.6/setup.cfg
+drwxr-xr-x   0 odop       (501) staff       (20)        0 2024-05-29 00:00:02.864536 django_oauth_emailbackend-0.1.6/src/
+drwxr-xr-x   0 odop       (501) staff       (20)        0 2024-05-29 00:00:02.869580 django_oauth_emailbackend-0.1.6/src/django_oauth_emailbackend.egg-info/
+-rw-r--r--   0 odop       (501) staff       (20)     3511 2024-05-29 00:00:02.000000 django_oauth_emailbackend-0.1.6/src/django_oauth_emailbackend.egg-info/PKG-INFO
+-rw-r--r--   0 odop       (501) staff       (20)     1135 2024-05-29 00:00:02.000000 django_oauth_emailbackend-0.1.6/src/django_oauth_emailbackend.egg-info/SOURCES.txt
+-rw-r--r--   0 odop       (501) staff       (20)        1 2024-05-29 00:00:02.000000 django_oauth_emailbackend-0.1.6/src/django_oauth_emailbackend.egg-info/dependency_links.txt
+-rw-r--r--   0 odop       (501) staff       (20)      119 2024-05-29 00:00:02.000000 django_oauth_emailbackend-0.1.6/src/django_oauth_emailbackend.egg-info/requires.txt
+-rw-r--r--   0 odop       (501) staff       (20)       19 2024-05-29 00:00:02.000000 django_oauth_emailbackend-0.1.6/src/django_oauth_emailbackend.egg-info/top_level.txt
+drwxr-xr-x   0 odop       (501) staff       (20)        0 2024-05-29 00:00:02.868406 django_oauth_emailbackend-0.1.6/src/oauth_emailbackend/
+-rw-r--r--   0 odop       (501) staff       (20)        0 2024-02-27 01:20:37.000000 django_oauth_emailbackend-0.1.6/src/oauth_emailbackend/__init__.py
+-rw-r--r--   0 odop       (501) staff       (20)     4930 2024-05-28 11:05:53.000000 django_oauth_emailbackend-0.1.6/src/oauth_emailbackend/admin.py
+-rw-r--r--   0 odop       (501) staff       (20)     1693 2024-03-28 12:13:39.000000 django_oauth_emailbackend-0.1.6/src/oauth_emailbackend/apps.py
+-rw-r--r--   0 odop       (501) staff       (20)     8389 2024-05-28 00:47:57.000000 django_oauth_emailbackend-0.1.6/src/oauth_emailbackend/backends.py
+-rw-r--r--   0 odop       (501) staff       (20)     1945 2024-05-28 11:03:44.000000 django_oauth_emailbackend-0.1.6/src/oauth_emailbackend/forms.py
+drwxr-xr-x   0 odop       (501) staff       (20)        0 2024-05-29 00:00:02.868545 django_oauth_emailbackend-0.1.6/src/oauth_emailbackend/management/
+-rw-r--r--   0 odop       (501) staff       (20)        0 2024-05-28 09:55:42.000000 django_oauth_emailbackend-0.1.6/src/oauth_emailbackend/management/__init__.py
+drwxr-xr-x   0 odop       (501) staff       (20)        0 2024-05-29 00:00:02.868662 django_oauth_emailbackend-0.1.6/src/oauth_emailbackend/management/commands/
+-rw-r--r--   0 odop       (501) staff       (20)        0 2024-04-04 05:03:10.000000 django_oauth_emailbackend-0.1.6/src/oauth_emailbackend/management/commands/__init__.py
+drwxr-xr-x   0 odop       (501) staff       (20)        0 2024-05-29 00:00:02.868920 django_oauth_emailbackend-0.1.6/src/oauth_emailbackend/migrations/
+-rw-r--r--   0 odop       (501) staff       (20)     5913 2024-05-28 05:32:50.000000 django_oauth_emailbackend-0.1.6/src/oauth_emailbackend/migrations/0001_initial.py
+-rw-r--r--   0 odop       (501) staff       (20)        0 2024-02-27 01:20:37.000000 django_oauth_emailbackend-0.1.6/src/oauth_emailbackend/migrations/__init__.py
+-rw-r--r--   0 odop       (501) staff       (20)     7671 2024-05-28 11:00:07.000000 django_oauth_emailbackend-0.1.6/src/oauth_emailbackend/models.py
+drwxr-xr-x   0 odop       (501) staff       (20)        0 2024-05-29 00:00:02.869135 django_oauth_emailbackend-0.1.6/src/oauth_emailbackend/providers/
+-rw-r--r--   0 odop       (501) staff       (20)     3712 2024-04-05 06:16:20.000000 django_oauth_emailbackend-0.1.6/src/oauth_emailbackend/providers/__init__.py
+-rw-r--r--   0 odop       (501) staff       (20)     7687 2024-05-28 01:00:07.000000 django_oauth_emailbackend-0.1.6/src/oauth_emailbackend/providers/gmail.py
+-rw-r--r--   0 odop       (501) staff       (20)     5066 2024-05-28 00:18:23.000000 django_oauth_emailbackend-0.1.6/src/oauth_emailbackend/tasks.py
+drwxr-xr-x   0 odop       (501) staff       (20)        0 2024-05-29 00:00:02.865158 django_oauth_emailbackend-0.1.6/src/oauth_emailbackend/templates/
+drwxr-xr-x   0 odop       (501) staff       (20)        0 2024-05-29 00:00:02.865034 django_oauth_emailbackend-0.1.6/src/oauth_emailbackend/templates/admin/
+drwxr-xr-x   0 odop       (501) staff       (20)        0 2024-05-29 00:00:02.865087 django_oauth_emailbackend-0.1.6/src/oauth_emailbackend/templates/admin/oauth_emailbackend/
+drwxr-xr-x   0 odop       (501) staff       (20)        0 2024-05-29 00:00:02.869258 django_oauth_emailbackend-0.1.6/src/oauth_emailbackend/templates/admin/oauth_emailbackend/emailclient/
+-rw-r--r--   0 odop       (501) staff       (20)     3957 2024-04-05 05:22:12.000000 django_oauth_emailbackend-0.1.6/src/oauth_emailbackend/templates/admin/oauth_emailbackend/emailclient/change_form.html
+drwxr-xr-x   0 odop       (501) staff       (20)        0 2024-05-29 00:00:02.869382 django_oauth_emailbackend-0.1.6/src/oauth_emailbackend/templates/oauth_emailbackend/
+-rw-r--r--   0 odop       (501) staff       (20)     3101 2024-04-05 06:19:46.000000 django_oauth_emailbackend-0.1.6/src/oauth_emailbackend/templates/oauth_emailbackend/callback.html
+-rw-r--r--   0 odop       (501) staff       (20)        0 2024-05-28 10:06:11.000000 django_oauth_emailbackend-0.1.6/src/oauth_emailbackend/test.html
+-rw-r--r--   0 odop       (501) staff       (20)       60 2024-02-27 01:20:37.000000 django_oauth_emailbackend-0.1.6/src/oauth_emailbackend/tests.py
+-rw-r--r--   0 odop       (501) staff       (20)      400 2024-03-29 11:43:15.000000 django_oauth_emailbackend-0.1.6/src/oauth_emailbackend/urls.py
+-rw-r--r--   0 odop       (501) staff       (20)     8340 2024-05-28 08:00:06.000000 django_oauth_emailbackend-0.1.6/src/oauth_emailbackend/utils.py
+-rw-r--r--   0 odop       (501) staff       (20)     1954 2024-04-05 06:28:05.000000 django_oauth_emailbackend-0.1.6/src/oauth_emailbackend/views.py
```

### Comparing `django_oauth_emailbackend-0.1.5/LICENSE` & `django_oauth_emailbackend-0.1.6/LICENSE`

 * *Files identical despite different names*

### Comparing `django_oauth_emailbackend-0.1.5/PKG-INFO` & `django_oauth_emailbackend-0.1.6/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 Metadata-Version: 2.1
 Name: django-oauth-emailbackend
-Version: 0.1.5
-Summary: Django emailbackend with Celery that using IMAP and google OAuth api
+Version: 0.1.6
+Summary: Django emailbackend that using OAuth Gmail API or SMTP server.
 Author-email: Sun-Yeon Lee <odop@youhasoft.com>
 Project-URL: Homepage, https://github.com/youhasoft/django-oauth-emailbackend
 Project-URL: Issues, https://github.com/youhasoft/django-oauth-emailbackend/issues
 Classifier: Development Status :: 3 - Alpha
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
```

### Comparing `django_oauth_emailbackend-0.1.5/README.md` & `django_oauth_emailbackend-0.1.6/README.md`

 * *Files identical despite different names*

### Comparing `django_oauth_emailbackend-0.1.5/pyproject.toml` & `django_oauth_emailbackend-0.1.6/pyproject.toml`

 * *Files 4% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [project]
 name = "django-oauth-emailbackend"
-version = "0.1.5"
+version = "0.1.6"
 authors = [
   { name="Sun-Yeon Lee", email="odop@youhasoft.com" },
 ]
-description = "Django emailbackend with Celery that using IMAP and google OAuth api"
+description = "Django emailbackend that using OAuth Gmail API or SMTP server."
 readme = "README.md"
 requires-python = ">=3.9"
 classifiers = [
     "Development Status :: 3 - Alpha",
     "Programming Language :: Python :: 3",
     "Programming Language :: Python :: 3.9",
     "Programming Language :: Python :: 3.10",
```

### Comparing `django_oauth_emailbackend-0.1.5/src/django_oauth_emailbackend.egg-info/PKG-INFO` & `django_oauth_emailbackend-0.1.6/src/django_oauth_emailbackend.egg-info/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 Metadata-Version: 2.1
 Name: django-oauth-emailbackend
-Version: 0.1.5
-Summary: Django emailbackend with Celery that using IMAP and google OAuth api
+Version: 0.1.6
+Summary: Django emailbackend that using OAuth Gmail API or SMTP server.
 Author-email: Sun-Yeon Lee <odop@youhasoft.com>
 Project-URL: Homepage, https://github.com/youhasoft/django-oauth-emailbackend
 Project-URL: Issues, https://github.com/youhasoft/django-oauth-emailbackend/issues
 Classifier: Development Status :: 3 - Alpha
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
```

### Comparing `django_oauth_emailbackend-0.1.5/src/django_oauth_emailbackend.egg-info/SOURCES.txt` & `django_oauth_emailbackend-0.1.6/src/django_oauth_emailbackend.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `django_oauth_emailbackend-0.1.5/src/oauth_emailbackend/admin.py` & `django_oauth_emailbackend-0.1.6/src/oauth_emailbackend/admin.py`

 * *Files identical despite different names*

### Comparing `django_oauth_emailbackend-0.1.5/src/oauth_emailbackend/apps.py` & `django_oauth_emailbackend-0.1.6/src/oauth_emailbackend/apps.py`

 * *Files identical despite different names*

### Comparing `django_oauth_emailbackend-0.1.5/src/oauth_emailbackend/backends.py` & `django_oauth_emailbackend-0.1.6/src/oauth_emailbackend/backends.py`

 * *Files identical despite different names*

### Comparing `django_oauth_emailbackend-0.1.5/src/oauth_emailbackend/forms.py` & `django_oauth_emailbackend-0.1.6/src/oauth_emailbackend/forms.py`

 * *Files identical despite different names*

### Comparing `django_oauth_emailbackend-0.1.5/src/oauth_emailbackend/migrations/0001_initial.py` & `django_oauth_emailbackend-0.1.6/src/oauth_emailbackend/migrations/0001_initial.py`

 * *Files identical despite different names*

### Comparing `django_oauth_emailbackend-0.1.5/src/oauth_emailbackend/models.py` & `django_oauth_emailbackend-0.1.6/src/oauth_emailbackend/models.py`

 * *Files identical despite different names*

### Comparing `django_oauth_emailbackend-0.1.5/src/oauth_emailbackend/providers/__init__.py` & `django_oauth_emailbackend-0.1.6/src/oauth_emailbackend/providers/__init__.py`

 * *Files identical despite different names*

### Comparing `django_oauth_emailbackend-0.1.5/src/oauth_emailbackend/providers/gmail.py` & `django_oauth_emailbackend-0.1.6/src/oauth_emailbackend/providers/gmail.py`

 * *Files identical despite different names*

### Comparing `django_oauth_emailbackend-0.1.5/src/oauth_emailbackend/tasks.py` & `django_oauth_emailbackend-0.1.6/src/oauth_emailbackend/tasks.py`

 * *Files identical despite different names*

### Comparing `django_oauth_emailbackend-0.1.5/src/oauth_emailbackend/templates/admin/oauth_emailbackend/emailclient/change_form.html` & `django_oauth_emailbackend-0.1.6/src/oauth_emailbackend/templates/admin/oauth_emailbackend/emailclient/change_form.html`

 * *Files identical despite different names*

### Comparing `django_oauth_emailbackend-0.1.5/src/oauth_emailbackend/templates/oauth_emailbackend/callback.html` & `django_oauth_emailbackend-0.1.6/src/oauth_emailbackend/templates/oauth_emailbackend/callback.html`

 * *Files identical despite different names*

### Comparing `django_oauth_emailbackend-0.1.5/src/oauth_emailbackend/utils.py` & `django_oauth_emailbackend-0.1.6/src/oauth_emailbackend/utils.py`

 * *Files identical despite different names*

### Comparing `django_oauth_emailbackend-0.1.5/src/oauth_emailbackend/views.py` & `django_oauth_emailbackend-0.1.6/src/oauth_emailbackend/views.py`

 * *Files identical despite different names*

