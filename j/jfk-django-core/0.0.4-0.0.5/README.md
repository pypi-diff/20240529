# Comparing `tmp/jfk_django_core-0.0.4.tar.gz` & `tmp/jfk_django_core-0.0.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "jfk_django_core-0.0.4.tar", last modified: Fri May 24 12:22:20 2024, max compression
+gzip compressed data, was "jfk_django_core-0.0.5.tar", last modified: Wed May 29 18:21:37 2024, max compression
```

## Comparing `jfk_django_core-0.0.4.tar` & `jfk_django_core-0.0.5.tar`

### file list

```diff
@@ -1,33 +1,33 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-24 12:22:20.212600 jfk_django_core-0.0.4/
--rw-rw-rw-   0 root         (0) root         (0)       47 2024-05-24 12:22:12.000000 jfk_django_core-0.0.4/.gitignore
--rw-rw-rw-   0 root         (0) root         (0)      300 2024-05-24 12:22:12.000000 jfk_django_core-0.0.4/.gitlab-ci.yml
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-24 12:22:20.208600 jfk_django_core-0.0.4/.vscode/
--rw-rw-rw-   0 root         (0) root         (0)      496 2024-05-24 12:22:12.000000 jfk_django_core-0.0.4/.vscode/launch.json
--rw-rw-rw-   0 root         (0) root         (0)     1091 2024-05-24 12:22:12.000000 jfk_django_core-0.0.4/LICENSE
--rw-r--r--   0 root         (0) root         (0)      790 2024-05-24 12:22:20.212600 jfk_django_core-0.0.4/PKG-INFO
--rw-rw-rw-   0 root         (0) root         (0)       13 2024-05-24 12:22:12.000000 jfk_django_core-0.0.4/README.md
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-24 12:22:20.209600 jfk_django_core-0.0.4/jfk_django_core/
--rw-rw-rw-   0 root         (0) root         (0)        0 2024-05-24 12:22:12.000000 jfk_django_core-0.0.4/jfk_django_core/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-24 12:22:20.210600 jfk_django_core-0.0.4/jfk_django_core/admin/
--rw-rw-rw-   0 root         (0) root         (0)        0 2024-05-24 12:22:12.000000 jfk_django_core-0.0.4/jfk_django_core/admin/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-24 12:22:20.211600 jfk_django_core-0.0.4/jfk_django_core/apis/
--rw-rw-rw-   0 root         (0) root         (0)       33 2024-05-24 12:22:12.000000 jfk_django_core-0.0.4/jfk_django_core/apis/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)      590 2024-05-24 12:22:12.000000 jfk_django_core-0.0.4/jfk_django_core/apis/jfk_authentication.py
--rw-rw-rw-   0 root         (0) root         (0)      197 2024-05-24 12:22:12.000000 jfk_django_core-0.0.4/jfk_django_core/apps.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-24 12:22:20.211600 jfk_django_core-0.0.4/jfk_django_core/migrations/
--rw-rw-rw-   0 root         (0) root         (0)        0 2024-05-24 12:22:12.000000 jfk_django_core-0.0.4/jfk_django_core/migrations/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-24 12:22:20.211600 jfk_django_core-0.0.4/jfk_django_core/models/
--rw-rw-rw-   0 root         (0) root         (0)        0 2024-05-24 12:22:12.000000 jfk_django_core-0.0.4/jfk_django_core/models/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)      394 2024-05-24 12:22:12.000000 jfk_django_core-0.0.4/jfk_django_core/serializers.py
--rw-rw-rw-   0 root         (0) root         (0)     7168 2024-05-24 12:22:12.000000 jfk_django_core-0.0.4/jfk_django_core/settings.py
--rw-rw-rw-   0 root         (0) root         (0)      862 2024-05-24 12:22:12.000000 jfk_django_core-0.0.4/jfk_django_core/urls.py
--rw-rw-rw-   0 root         (0) root         (0)      503 2024-05-24 12:22:12.000000 jfk_django_core-0.0.4/jfk_django_core/viewsets.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-24 12:22:20.211600 jfk_django_core-0.0.4/jfk_django_core.egg-info/
--rw-r--r--   0 root         (0) root         (0)      790 2024-05-24 12:22:20.000000 jfk_django_core-0.0.4/jfk_django_core.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)      628 2024-05-24 12:22:20.000000 jfk_django_core-0.0.4/jfk_django_core.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2024-05-24 12:22:20.000000 jfk_django_core-0.0.4/jfk_django_core.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)      337 2024-05-24 12:22:20.000000 jfk_django_core-0.0.4/jfk_django_core.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)       16 2024-05-24 12:22:20.000000 jfk_django_core-0.0.4/jfk_django_core.egg-info/top_level.txt
--rw-rw-rw-   0 root         (0) root         (0)      916 2024-05-24 12:22:12.000000 jfk_django_core-0.0.4/pyproject.toml
--rw-r--r--   0 root         (0) root         (0)       38 2024-05-24 12:22:20.212600 jfk_django_core-0.0.4/setup.cfg
--rw-rw-rw-   0 root         (0) root         (0)      143 2024-05-24 12:22:12.000000 jfk_django_core-0.0.4/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-29 18:21:37.009555 jfk_django_core-0.0.5/
+-rw-rw-rw-   0 root         (0) root         (0)       47 2024-05-29 18:21:29.000000 jfk_django_core-0.0.5/.gitignore
+-rw-rw-rw-   0 root         (0) root         (0)      300 2024-05-29 18:21:29.000000 jfk_django_core-0.0.5/.gitlab-ci.yml
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-29 18:21:37.005555 jfk_django_core-0.0.5/.vscode/
+-rw-rw-rw-   0 root         (0) root         (0)      496 2024-05-29 18:21:29.000000 jfk_django_core-0.0.5/.vscode/launch.json
+-rw-rw-rw-   0 root         (0) root         (0)     1091 2024-05-29 18:21:29.000000 jfk_django_core-0.0.5/LICENSE
+-rw-r--r--   0 root         (0) root         (0)      874 2024-05-29 18:21:37.009555 jfk_django_core-0.0.5/PKG-INFO
+-rw-rw-rw-   0 root         (0) root         (0)       13 2024-05-29 18:21:29.000000 jfk_django_core-0.0.5/README.md
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-29 18:21:37.006555 jfk_django_core-0.0.5/jfk_django_core/
+-rw-rw-rw-   0 root         (0) root         (0)        0 2024-05-29 18:21:29.000000 jfk_django_core-0.0.5/jfk_django_core/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-29 18:21:37.008556 jfk_django_core-0.0.5/jfk_django_core/admin/
+-rw-rw-rw-   0 root         (0) root         (0)        0 2024-05-29 18:21:29.000000 jfk_django_core-0.0.5/jfk_django_core/admin/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-29 18:21:37.008556 jfk_django_core-0.0.5/jfk_django_core/apis/
+-rw-rw-rw-   0 root         (0) root         (0)       33 2024-05-29 18:21:29.000000 jfk_django_core-0.0.5/jfk_django_core/apis/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)      590 2024-05-29 18:21:29.000000 jfk_django_core-0.0.5/jfk_django_core/apis/jfk_authentication.py
+-rw-rw-rw-   0 root         (0) root         (0)      197 2024-05-29 18:21:29.000000 jfk_django_core-0.0.5/jfk_django_core/apps.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-29 18:21:37.008556 jfk_django_core-0.0.5/jfk_django_core/migrations/
+-rw-rw-rw-   0 root         (0) root         (0)        0 2024-05-29 18:21:29.000000 jfk_django_core-0.0.5/jfk_django_core/migrations/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-29 18:21:37.008556 jfk_django_core-0.0.5/jfk_django_core/models/
+-rw-rw-rw-   0 root         (0) root         (0)        0 2024-05-29 18:21:29.000000 jfk_django_core-0.0.5/jfk_django_core/models/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)      394 2024-05-29 18:21:29.000000 jfk_django_core-0.0.5/jfk_django_core/serializers.py
+-rw-rw-rw-   0 root         (0) root         (0)     7209 2024-05-29 18:21:29.000000 jfk_django_core-0.0.5/jfk_django_core/settings.py
+-rw-rw-rw-   0 root         (0) root         (0)      862 2024-05-29 18:21:29.000000 jfk_django_core-0.0.5/jfk_django_core/urls.py
+-rw-rw-rw-   0 root         (0) root         (0)      503 2024-05-29 18:21:29.000000 jfk_django_core-0.0.5/jfk_django_core/viewsets.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-29 18:21:37.009555 jfk_django_core-0.0.5/jfk_django_core.egg-info/
+-rw-r--r--   0 root         (0) root         (0)      874 2024-05-29 18:21:36.000000 jfk_django_core-0.0.5/jfk_django_core.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)      628 2024-05-29 18:21:36.000000 jfk_django_core-0.0.5/jfk_django_core.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2024-05-29 18:21:36.000000 jfk_django_core-0.0.5/jfk_django_core.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)      391 2024-05-29 18:21:36.000000 jfk_django_core-0.0.5/jfk_django_core.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)       16 2024-05-29 18:21:36.000000 jfk_django_core-0.0.5/jfk_django_core.egg-info/top_level.txt
+-rw-rw-rw-   0 root         (0) root         (0)      985 2024-05-29 18:21:29.000000 jfk_django_core-0.0.5/pyproject.toml
+-rw-r--r--   0 root         (0) root         (0)       38 2024-05-29 18:21:37.009555 jfk_django_core-0.0.5/setup.cfg
+-rw-rw-rw-   0 root         (0) root         (0)      143 2024-05-29 18:21:29.000000 jfk_django_core-0.0.5/setup.py
```

### Comparing `jfk_django_core-0.0.4/LICENSE` & `jfk_django_core-0.0.5/LICENSE`

 * *Files identical despite different names*

### Comparing `jfk_django_core-0.0.4/PKG-INFO` & `jfk_django_core-0.0.5/PKG-INFO`

 * *Files 20% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: jfk-django-core
-Version: 0.0.4
+Version: 0.0.5
 Summary: JFK Django Core
 Author: JFK344
 License: All-Rights-Reserved
 Requires-Python: >=3.8
 Description-Content-Type: text/markdown
 License-File: LICENSE
 Requires-Dist: Django>=5.0.0
@@ -18,9 +18,11 @@
 Requires-Dist: psycopg2-binary==2.9.9
 Requires-Dist: uvicorn>=0.29.0
 Requires-Dist: websockets>=12.0
 Requires-Dist: whitenoise>=6.6.0
 Requires-Dist: daphne>=4.1.2
 Requires-Dist: drf-spectacular-sidecar>=2024.5.1
 Requires-Dist: drf-spectacular>=0.27.2
+Requires-Dist: django-mass-edit>=3.5.0
+Requires-Dist: django-extra-settings>=0.12.0
 
 # Django Core
```

### Comparing `jfk_django_core-0.0.4/jfk_django_core/apis/jfk_authentication.py` & `jfk_django_core-0.0.5/jfk_django_core/apis/jfk_authentication.py`

 * *Files identical despite different names*

### Comparing `jfk_django_core-0.0.4/jfk_django_core/settings.py` & `jfk_django_core-0.0.5/jfk_django_core/settings.py`

 * *Files 3% similar despite different names*

```diff
@@ -66,14 +66,18 @@
     'django.middleware.common.CommonMiddleware',
     'django.middleware.csrf.CsrfViewMiddleware',
     'django.contrib.auth.middleware.AuthenticationMiddleware',
     'django.contrib.messages.middleware.MessageMiddleware',
     'django.middleware.clickjacking.XFrameOptionsMiddleware',
     # 3rd party
     "whitenoise.middleware.WhiteNoiseMiddleware",
+    "massadmin",
+    "extra_settings",
+
+
 ]
 
 # Application Templates
 TEMPLATES = [
     {
         'BACKEND': 'django.template.backends.django.DjangoTemplates',
         'DIRS': [],
```

### Comparing `jfk_django_core-0.0.4/jfk_django_core/urls.py` & `jfk_django_core-0.0.5/jfk_django_core/urls.py`

 * *Files identical despite different names*

### Comparing `jfk_django_core-0.0.4/jfk_django_core.egg-info/PKG-INFO` & `jfk_django_core-0.0.5/jfk_django_core.egg-info/PKG-INFO`

 * *Files 20% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: jfk-django-core
-Version: 0.0.4
+Version: 0.0.5
 Summary: JFK Django Core
 Author: JFK344
 License: All-Rights-Reserved
 Requires-Python: >=3.8
 Description-Content-Type: text/markdown
 License-File: LICENSE
 Requires-Dist: Django>=5.0.0
@@ -18,9 +18,11 @@
 Requires-Dist: psycopg2-binary==2.9.9
 Requires-Dist: uvicorn>=0.29.0
 Requires-Dist: websockets>=12.0
 Requires-Dist: whitenoise>=6.6.0
 Requires-Dist: daphne>=4.1.2
 Requires-Dist: drf-spectacular-sidecar>=2024.5.1
 Requires-Dist: drf-spectacular>=0.27.2
+Requires-Dist: django-mass-edit>=3.5.0
+Requires-Dist: django-extra-settings>=0.12.0
 
 # Django Core
```

### Comparing `jfk_django_core-0.0.4/jfk_django_core.egg-info/SOURCES.txt` & `jfk_django_core-0.0.5/jfk_django_core.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `jfk_django_core-0.0.4/pyproject.toml` & `jfk_django_core-0.0.5/pyproject.toml`

 * *Files 6% similar despite different names*

```diff
@@ -26,13 +26,15 @@
     "gunicorn==22.0.0",
     "psycopg2-binary==2.9.9",
     "uvicorn>=0.29.0",
     "websockets>=12.0",
     "whitenoise>=6.6.0",
     "daphne>=4.1.2",
     "drf-spectacular-sidecar>=2024.5.1",
-    "drf-spectacular>=0.27.2"
+    "drf-spectacular>=0.27.2",
+    "django-mass-edit>=3.5.0",
+    "django-extra-settings>=0.12.0",
 ]
 
 [tool.setuptools_scm]
 version_scheme = "guess-next-dev"
 local_scheme = "dirty-tag"
```

