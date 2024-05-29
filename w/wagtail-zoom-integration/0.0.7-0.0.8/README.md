# Comparing `tmp/wagtail_zoom_integration-0.0.7.tar.gz` & `tmp/wagtail_zoom_integration-0.0.8.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "wagtail_zoom_integration-0.0.7.tar", last modified: Thu May 23 10:26:49 2024, max compression
+gzip compressed data, was "wagtail_zoom_integration-0.0.8.tar", last modified: Wed May 29 11:46:18 2024, max compression
```

## Comparing `wagtail_zoom_integration-0.0.7.tar` & `wagtail_zoom_integration-0.0.8.tar`

### file list

```diff
@@ -1,58 +1,58 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-23 10:26:49.343329 wagtail_zoom_integration-0.0.7/
--rw-r--r--   0 runner    (1001) docker     (127)      131 2024-05-23 10:26:45.000000 wagtail_zoom_integration-0.0.7/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (127)     7828 2024-05-23 10:26:49.343329 wagtail_zoom_integration-0.0.7/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     6820 2024-05-23 10:26:45.000000 wagtail_zoom_integration-0.0.7/README.md
--rw-r--r--   0 runner    (1001) docker     (127)       80 2024-05-23 10:26:45.000000 wagtail_zoom_integration-0.0.7/pyproject.toml
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-23 10:26:49.335329 wagtail_zoom_integration-0.0.7/sandbox/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-23 10:26:45.000000 wagtail_zoom_integration-0.0.7/sandbox/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-23 10:26:49.335329 wagtail_zoom_integration-0.0.7/sandbox/home/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-23 10:26:45.000000 wagtail_zoom_integration-0.0.7/sandbox/home/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-23 10:26:49.339329 wagtail_zoom_integration-0.0.7/sandbox/home/migrations/
--rw-r--r--   0 runner    (1001) docker     (127)      830 2024-05-23 10:26:45.000000 wagtail_zoom_integration-0.0.7/sandbox/home/migrations/0001_initial.py
--rw-r--r--   0 runner    (1001) docker     (127)     1741 2024-05-23 10:26:45.000000 wagtail_zoom_integration-0.0.7/sandbox/home/migrations/0002_create_homepage.py
--rw-r--r--   0 runner    (1001) docker     (127)     1031 2024-05-23 10:26:45.000000 wagtail_zoom_integration-0.0.7/sandbox/home/migrations/0003_eventregistrationpage.py
--rw-r--r--   0 runner    (1001) docker     (127)     2226 2024-05-23 10:26:45.000000 wagtail_zoom_integration-0.0.7/sandbox/home/migrations/0004_formfield.py
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-23 10:26:45.000000 wagtail_zoom_integration-0.0.7/sandbox/home/migrations/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      825 2024-05-23 10:26:45.000000 wagtail_zoom_integration-0.0.7/sandbox/home/models.py
--rwxr-xr-x   0 runner    (1001) docker     (127)      254 2024-05-23 10:26:45.000000 wagtail_zoom_integration-0.0.7/sandbox/manage.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-23 10:26:49.339329 wagtail_zoom_integration-0.0.7/sandbox/sandbox/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-23 10:26:45.000000 wagtail_zoom_integration-0.0.7/sandbox/sandbox/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-23 10:26:49.339329 wagtail_zoom_integration-0.0.7/sandbox/sandbox/settings/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-23 10:26:45.000000 wagtail_zoom_integration-0.0.7/sandbox/sandbox/settings/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     4541 2024-05-23 10:26:45.000000 wagtail_zoom_integration-0.0.7/sandbox/sandbox/settings/base.py
--rw-r--r--   0 runner    (1001) docker     (127)      460 2024-05-23 10:26:45.000000 wagtail_zoom_integration-0.0.7/sandbox/sandbox/settings/dev.py
--rw-r--r--   0 runner    (1001) docker     (127)       95 2024-05-23 10:26:45.000000 wagtail_zoom_integration-0.0.7/sandbox/sandbox/settings/production.py
--rw-r--r--   0 runner    (1001) docker     (127)     1245 2024-05-23 10:26:45.000000 wagtail_zoom_integration-0.0.7/sandbox/sandbox/urls.py
--rw-r--r--   0 runner    (1001) docker     (127)      395 2024-05-23 10:26:45.000000 wagtail_zoom_integration-0.0.7/sandbox/sandbox/wsgi.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-23 10:26:49.339329 wagtail_zoom_integration-0.0.7/sandbox/search/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-23 10:26:45.000000 wagtail_zoom_integration-0.0.7/sandbox/search/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1019 2024-05-23 10:26:45.000000 wagtail_zoom_integration-0.0.7/sandbox/search/views.py
--rw-r--r--   0 runner    (1001) docker     (127)     1020 2024-05-23 10:26:49.343329 wagtail_zoom_integration-0.0.7/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-23 10:26:49.343329 wagtail_zoom_integration-0.0.7/wagtail_zoom_integration.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     7828 2024-05-23 10:26:49.000000 wagtail_zoom_integration-0.0.7/wagtail_zoom_integration.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     1452 2024-05-23 10:26:49.000000 wagtail_zoom_integration-0.0.7/wagtail_zoom_integration.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-23 10:26:49.000000 wagtail_zoom_integration-0.0.7/wagtail_zoom_integration.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       47 2024-05-23 10:26:49.000000 wagtail_zoom_integration-0.0.7/wagtail_zoom_integration.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       20 2024-05-23 10:26:49.000000 wagtail_zoom_integration-0.0.7/wagtail_zoom_integration.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-23 10:26:49.343329 wagtail_zoom_integration-0.0.7/wagtailzoom/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-23 10:26:45.000000 wagtail_zoom_integration-0.0.7/wagtailzoom/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)       63 2024-05-23 10:26:45.000000 wagtail_zoom_integration-0.0.7/wagtailzoom/admin.py
--rw-r--r--   0 runner    (1001) docker     (127)     5340 2024-05-23 10:26:45.000000 wagtail_zoom_integration-0.0.7/wagtailzoom/api.py
--rw-r--r--   0 runner    (1001) docker     (127)      154 2024-05-23 10:26:45.000000 wagtail_zoom_integration-0.0.7/wagtailzoom/apps.py
--rw-r--r--   0 runner    (1001) docker     (127)      241 2024-05-23 10:26:45.000000 wagtail_zoom_integration-0.0.7/wagtailzoom/errors.py
--rw-r--r--   0 runner    (1001) docker     (127)     3172 2024-05-23 10:26:45.000000 wagtail_zoom_integration-0.0.7/wagtailzoom/forms.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-23 10:26:49.343329 wagtail_zoom_integration-0.0.7/wagtailzoom/migrations/
--rw-r--r--   0 runner    (1001) docker     (127)     1044 2024-05-23 10:26:45.000000 wagtail_zoom_integration-0.0.7/wagtailzoom/migrations/0001_initial.py
--rw-r--r--   0 runner    (1001) docker     (127)     1340 2024-05-23 10:26:45.000000 wagtail_zoom_integration-0.0.7/wagtailzoom/migrations/0002_remove_zoomsettings_api_key_and_more.py
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-23 10:26:45.000000 wagtail_zoom_integration-0.0.7/wagtailzoom/migrations/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     5679 2024-05-23 10:26:45.000000 wagtail_zoom_integration-0.0.7/wagtailzoom/models.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-23 10:26:49.335329 wagtail_zoom_integration-0.0.7/wagtailzoom/templates/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-23 10:26:49.343329 wagtail_zoom_integration-0.0.7/wagtailzoom/templates/wagtailzoom/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-23 10:26:49.343329 wagtail_zoom_integration-0.0.7/wagtailzoom/templates/wagtailzoom/widgets/
--rw-r--r--   0 runner    (1001) docker     (127)     1213 2024-05-23 10:26:45.000000 wagtail_zoom_integration-0.0.7/wagtailzoom/templates/wagtailzoom/widgets/zoom_event_select_widget.html
--rw-r--r--   0 runner    (1001) docker     (127)     1290 2024-05-23 10:26:45.000000 wagtail_zoom_integration-0.0.7/wagtailzoom/templates/wagtailzoom/widgets/zoom_event_select_widget_js.html
--rw-r--r--   0 runner    (1001) docker     (127)     2943 2024-05-23 10:26:45.000000 wagtail_zoom_integration-0.0.7/wagtailzoom/templates/wagtailzoom/zoom_integration_form.html
--rw-r--r--   0 runner    (1001) docker     (127)       60 2024-05-23 10:26:45.000000 wagtail_zoom_integration-0.0.7/wagtailzoom/tests.py
--rw-r--r--   0 runner    (1001) docker     (127)     4648 2024-05-23 10:26:45.000000 wagtail_zoom_integration-0.0.7/wagtailzoom/views.py
--rw-r--r--   0 runner    (1001) docker     (127)     3335 2024-05-23 10:26:45.000000 wagtail_zoom_integration-0.0.7/wagtailzoom/wagtail_hooks.py
--rw-r--r--   0 runner    (1001) docker     (127)     3282 2024-05-23 10:26:45.000000 wagtail_zoom_integration-0.0.7/wagtailzoom/widgets.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-29 11:46:18.217473 wagtail_zoom_integration-0.0.8/
+-rw-r--r--   0 runner    (1001) docker     (127)      131 2024-05-29 11:46:14.000000 wagtail_zoom_integration-0.0.8/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (127)     7828 2024-05-29 11:46:18.213473 wagtail_zoom_integration-0.0.8/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     6820 2024-05-29 11:46:14.000000 wagtail_zoom_integration-0.0.8/README.md
+-rw-r--r--   0 runner    (1001) docker     (127)       80 2024-05-29 11:46:14.000000 wagtail_zoom_integration-0.0.8/pyproject.toml
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-29 11:46:18.209473 wagtail_zoom_integration-0.0.8/sandbox/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-29 11:46:14.000000 wagtail_zoom_integration-0.0.8/sandbox/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-29 11:46:18.209473 wagtail_zoom_integration-0.0.8/sandbox/home/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-29 11:46:14.000000 wagtail_zoom_integration-0.0.8/sandbox/home/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-29 11:46:18.209473 wagtail_zoom_integration-0.0.8/sandbox/home/migrations/
+-rw-r--r--   0 runner    (1001) docker     (127)      830 2024-05-29 11:46:14.000000 wagtail_zoom_integration-0.0.8/sandbox/home/migrations/0001_initial.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1741 2024-05-29 11:46:14.000000 wagtail_zoom_integration-0.0.8/sandbox/home/migrations/0002_create_homepage.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1031 2024-05-29 11:46:14.000000 wagtail_zoom_integration-0.0.8/sandbox/home/migrations/0003_eventregistrationpage.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2226 2024-05-29 11:46:14.000000 wagtail_zoom_integration-0.0.8/sandbox/home/migrations/0004_formfield.py
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-29 11:46:14.000000 wagtail_zoom_integration-0.0.8/sandbox/home/migrations/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      825 2024-05-29 11:46:14.000000 wagtail_zoom_integration-0.0.8/sandbox/home/models.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)      254 2024-05-29 11:46:14.000000 wagtail_zoom_integration-0.0.8/sandbox/manage.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-29 11:46:18.209473 wagtail_zoom_integration-0.0.8/sandbox/sandbox/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-29 11:46:14.000000 wagtail_zoom_integration-0.0.8/sandbox/sandbox/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-29 11:46:18.209473 wagtail_zoom_integration-0.0.8/sandbox/sandbox/settings/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-29 11:46:14.000000 wagtail_zoom_integration-0.0.8/sandbox/sandbox/settings/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4541 2024-05-29 11:46:14.000000 wagtail_zoom_integration-0.0.8/sandbox/sandbox/settings/base.py
+-rw-r--r--   0 runner    (1001) docker     (127)      460 2024-05-29 11:46:14.000000 wagtail_zoom_integration-0.0.8/sandbox/sandbox/settings/dev.py
+-rw-r--r--   0 runner    (1001) docker     (127)       95 2024-05-29 11:46:14.000000 wagtail_zoom_integration-0.0.8/sandbox/sandbox/settings/production.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1245 2024-05-29 11:46:14.000000 wagtail_zoom_integration-0.0.8/sandbox/sandbox/urls.py
+-rw-r--r--   0 runner    (1001) docker     (127)      395 2024-05-29 11:46:14.000000 wagtail_zoom_integration-0.0.8/sandbox/sandbox/wsgi.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-29 11:46:18.209473 wagtail_zoom_integration-0.0.8/sandbox/search/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-29 11:46:14.000000 wagtail_zoom_integration-0.0.8/sandbox/search/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1019 2024-05-29 11:46:14.000000 wagtail_zoom_integration-0.0.8/sandbox/search/views.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1020 2024-05-29 11:46:18.217473 wagtail_zoom_integration-0.0.8/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-29 11:46:18.213473 wagtail_zoom_integration-0.0.8/wagtail_zoom_integration.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     7828 2024-05-29 11:46:18.000000 wagtail_zoom_integration-0.0.8/wagtail_zoom_integration.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     1452 2024-05-29 11:46:18.000000 wagtail_zoom_integration-0.0.8/wagtail_zoom_integration.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-29 11:46:18.000000 wagtail_zoom_integration-0.0.8/wagtail_zoom_integration.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       47 2024-05-29 11:46:18.000000 wagtail_zoom_integration-0.0.8/wagtail_zoom_integration.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       20 2024-05-29 11:46:18.000000 wagtail_zoom_integration-0.0.8/wagtail_zoom_integration.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-29 11:46:18.213473 wagtail_zoom_integration-0.0.8/wagtailzoom/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-29 11:46:14.000000 wagtail_zoom_integration-0.0.8/wagtailzoom/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)       63 2024-05-29 11:46:14.000000 wagtail_zoom_integration-0.0.8/wagtailzoom/admin.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5340 2024-05-29 11:46:14.000000 wagtail_zoom_integration-0.0.8/wagtailzoom/api.py
+-rw-r--r--   0 runner    (1001) docker     (127)      154 2024-05-29 11:46:14.000000 wagtail_zoom_integration-0.0.8/wagtailzoom/apps.py
+-rw-r--r--   0 runner    (1001) docker     (127)      241 2024-05-29 11:46:14.000000 wagtail_zoom_integration-0.0.8/wagtailzoom/errors.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3172 2024-05-29 11:46:14.000000 wagtail_zoom_integration-0.0.8/wagtailzoom/forms.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-29 11:46:18.213473 wagtail_zoom_integration-0.0.8/wagtailzoom/migrations/
+-rw-r--r--   0 runner    (1001) docker     (127)     1044 2024-05-29 11:46:14.000000 wagtail_zoom_integration-0.0.8/wagtailzoom/migrations/0001_initial.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1340 2024-05-29 11:46:14.000000 wagtail_zoom_integration-0.0.8/wagtailzoom/migrations/0002_remove_zoomsettings_api_key_and_more.py
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-29 11:46:14.000000 wagtail_zoom_integration-0.0.8/wagtailzoom/migrations/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6180 2024-05-29 11:46:14.000000 wagtail_zoom_integration-0.0.8/wagtailzoom/models.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-29 11:46:18.205474 wagtail_zoom_integration-0.0.8/wagtailzoom/templates/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-29 11:46:18.213473 wagtail_zoom_integration-0.0.8/wagtailzoom/templates/wagtailzoom/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-29 11:46:18.213473 wagtail_zoom_integration-0.0.8/wagtailzoom/templates/wagtailzoom/widgets/
+-rw-r--r--   0 runner    (1001) docker     (127)     1153 2024-05-29 11:46:14.000000 wagtail_zoom_integration-0.0.8/wagtailzoom/templates/wagtailzoom/widgets/zoom_event_select_widget.html
+-rw-r--r--   0 runner    (1001) docker     (127)     1290 2024-05-29 11:46:14.000000 wagtail_zoom_integration-0.0.8/wagtailzoom/templates/wagtailzoom/widgets/zoom_event_select_widget_js.html
+-rw-r--r--   0 runner    (1001) docker     (127)     2943 2024-05-29 11:46:14.000000 wagtail_zoom_integration-0.0.8/wagtailzoom/templates/wagtailzoom/zoom_integration_form.html
+-rw-r--r--   0 runner    (1001) docker     (127)       60 2024-05-29 11:46:14.000000 wagtail_zoom_integration-0.0.8/wagtailzoom/tests.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4671 2024-05-29 11:46:14.000000 wagtail_zoom_integration-0.0.8/wagtailzoom/views.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3462 2024-05-29 11:46:14.000000 wagtail_zoom_integration-0.0.8/wagtailzoom/wagtail_hooks.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3282 2024-05-29 11:46:14.000000 wagtail_zoom_integration-0.0.8/wagtailzoom/widgets.py
```

### Comparing `wagtail_zoom_integration-0.0.7/PKG-INFO` & `wagtail_zoom_integration-0.0.8/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: wagtail-zoom-integration
-Version: 0.0.7
+Version: 0.0.8
 Summary: Integrate automated Zoom Events registration in Wagtail Form Builder Pages.
 Home-page: https://github.com/erick-otenyo/wagtail-zoom-integration
 Author: Erick Otenyo
 Author-email: otenyo.erick@gmail.com
 License: MIT
 Classifier: Development Status :: 4 - Beta
 Classifier: Environment :: Web Environment
```

### Comparing `wagtail_zoom_integration-0.0.7/README.md` & `wagtail_zoom_integration-0.0.8/README.md`

 * *Files identical despite different names*

### Comparing `wagtail_zoom_integration-0.0.7/sandbox/home/migrations/0001_initial.py` & `wagtail_zoom_integration-0.0.8/sandbox/home/migrations/0001_initial.py`

 * *Files identical despite different names*

### Comparing `wagtail_zoom_integration-0.0.7/sandbox/home/migrations/0002_create_homepage.py` & `wagtail_zoom_integration-0.0.8/sandbox/home/migrations/0002_create_homepage.py`

 * *Files identical despite different names*

### Comparing `wagtail_zoom_integration-0.0.7/sandbox/home/migrations/0003_eventregistrationpage.py` & `wagtail_zoom_integration-0.0.8/sandbox/home/migrations/0003_eventregistrationpage.py`

 * *Files identical despite different names*

### Comparing `wagtail_zoom_integration-0.0.7/sandbox/home/migrations/0004_formfield.py` & `wagtail_zoom_integration-0.0.8/sandbox/home/migrations/0004_formfield.py`

 * *Files identical despite different names*

### Comparing `wagtail_zoom_integration-0.0.7/sandbox/home/models.py` & `wagtail_zoom_integration-0.0.8/sandbox/home/models.py`

 * *Files identical despite different names*

### Comparing `wagtail_zoom_integration-0.0.7/sandbox/sandbox/settings/base.py` & `wagtail_zoom_integration-0.0.8/sandbox/sandbox/settings/base.py`

 * *Files identical despite different names*

### Comparing `wagtail_zoom_integration-0.0.7/sandbox/sandbox/urls.py` & `wagtail_zoom_integration-0.0.8/sandbox/sandbox/urls.py`

 * *Files identical despite different names*

### Comparing `wagtail_zoom_integration-0.0.7/sandbox/search/views.py` & `wagtail_zoom_integration-0.0.8/sandbox/search/views.py`

 * *Files identical despite different names*

### Comparing `wagtail_zoom_integration-0.0.7/setup.cfg` & `wagtail_zoom_integration-0.0.8/setup.cfg`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [metadata]
 name = wagtail-zoom-integration
-version = 0.0.7
+version = 0.0.8
 description = Integrate automated Zoom Events registration in Wagtail Form Builder Pages.
 long_description = file:README.md
 long_description_content_type = text/markdown
 url = https://github.com/erick-otenyo/wagtail-zoom-integration
 author = Erick Otenyo
 author_email = otenyo.erick@gmail.com
 license = MIT
```

### Comparing `wagtail_zoom_integration-0.0.7/wagtail_zoom_integration.egg-info/PKG-INFO` & `wagtail_zoom_integration-0.0.8/wagtail_zoom_integration.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: wagtail-zoom-integration
-Version: 0.0.7
+Version: 0.0.8
 Summary: Integrate automated Zoom Events registration in Wagtail Form Builder Pages.
 Home-page: https://github.com/erick-otenyo/wagtail-zoom-integration
 Author: Erick Otenyo
 Author-email: otenyo.erick@gmail.com
 License: MIT
 Classifier: Development Status :: 4 - Beta
 Classifier: Environment :: Web Environment
```

### Comparing `wagtail_zoom_integration-0.0.7/wagtail_zoom_integration.egg-info/SOURCES.txt` & `wagtail_zoom_integration-0.0.8/wagtail_zoom_integration.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `wagtail_zoom_integration-0.0.7/wagtailzoom/api.py` & `wagtail_zoom_integration-0.0.8/wagtailzoom/api.py`

 * *Files identical despite different names*

### Comparing `wagtail_zoom_integration-0.0.7/wagtailzoom/forms.py` & `wagtail_zoom_integration-0.0.8/wagtailzoom/forms.py`

 * *Files identical despite different names*

### Comparing `wagtail_zoom_integration-0.0.7/wagtailzoom/migrations/0001_initial.py` & `wagtail_zoom_integration-0.0.8/wagtailzoom/migrations/0001_initial.py`

 * *Files identical despite different names*

### Comparing `wagtail_zoom_integration-0.0.7/wagtailzoom/migrations/0002_remove_zoomsettings_api_key_and_more.py` & `wagtail_zoom_integration-0.0.8/wagtailzoom/migrations/0002_remove_zoomsettings_api_key_and_more.py`

 * *Files identical despite different names*

### Comparing `wagtail_zoom_integration-0.0.7/wagtailzoom/models.py` & `wagtail_zoom_integration-0.0.8/wagtailzoom/models.py`

 * *Files 14% similar despite different names*

```diff
@@ -87,18 +87,27 @@
                         "event_topic": event.get("event_topic")
                     })
             except Exception:
                 pass
 
         return data
 
+    def should_perform_zoom_integration_operation(self, request, form):
+        # override this method to add custom logic to determine if the zoom integration operation should be performed
+        return True
+
+    def show_page_listing_zoom_integration_button(self):
+        # override this method to add custom logic to determine if the
+        # zoom integration button should be shown in the page listing
+        return True
+
     def process_form_submission(self, form):
         form_submission = super(AbstractZoomIntegrationForm, self).process_form_submission(form)
 
-        if self.request:
+        if self.request and self.should_perform_zoom_integration_operation(self.request, form):
             self.zoom_integration_operation(self, form=form, request=self.request)
 
         return form_submission
 
     def serve(self, request, *args, **kwargs):
         # We need to access the request later on in integration operation
         self.request = request
```

### Comparing `wagtail_zoom_integration-0.0.7/wagtailzoom/templates/wagtailzoom/widgets/zoom_event_select_widget.html` & `wagtail_zoom_integration-0.0.8/wagtailzoom/templates/wagtailzoom/widgets/zoom_event_select_widget.html`

 * *Files 18% similar despite different names*

```diff
@@ -8,21 +8,19 @@
         {% if event.id == widget.stored_event_id %} selected{% endif %}
         <option value="{{ event.id }}" {% if event.id|stringformat:"i" == widget.stored_event_id %} selected{% endif %}>
             {{ event.event_type_label }} - {{ event.topic }}
         </option>
     {% endfor %}
 </select>
 {% if widget.zoom_error %}
-    <div class="error">
-        <div class="help-block help-critical">
-            <svg class="icon icon-warning icon" aria-hidden="true">
-                <use href="#icon-warning"></use>
-            </svg>
-            {{ widget.zoom_error }}
-        </div>
+    <div class="help-block help-warning">
+        <svg class="icon icon-warning icon" aria-hidden="true">
+            <use href="#icon-warning"></use>
+        </svg>
+        {{ widget.zoom_error }}
     </div>
 {% elif not widget.selectable_events %}
     <div class="help-block help-warning">
         <svg class="icon icon-warning icon" aria-hidden="true">
             <use href="#icon-warning"></use>
         </svg>
         {{ widget.no_events_message }}
```

### Comparing `wagtail_zoom_integration-0.0.7/wagtailzoom/templates/wagtailzoom/widgets/zoom_event_select_widget_js.html` & `wagtail_zoom_integration-0.0.8/wagtailzoom/templates/wagtailzoom/widgets/zoom_event_select_widget_js.html`

 * *Files identical despite different names*

### Comparing `wagtail_zoom_integration-0.0.7/wagtailzoom/templates/wagtailzoom/zoom_integration_form.html` & `wagtail_zoom_integration-0.0.8/wagtailzoom/templates/wagtailzoom/zoom_integration_form.html`

 * *Files identical despite different names*

### Comparing `wagtail_zoom_integration-0.0.7/wagtailzoom/views.py` & `wagtail_zoom_integration-0.0.8/wagtailzoom/views.py`

 * *Files 2% similar despite different names*

```diff
@@ -13,15 +13,15 @@
 from .errors import ZoomApiCredentialsError
 from .forms import ZoomIntegrationForm
 from .models import ZoomSettings
 
 
 def zoom_integration_view(request, page_id):
     page = Page.objects.get(pk=page_id)
-    form_page = page.specific
+    form_page = page.get_latest_revision_as_object()
     edit_url = reverse("wagtailadmin_pages:edit", args=[form_page.pk])
     context = {"page": form_page, "page_edit_url": edit_url}
     template_name = "wagtailzoom/zoom_integration_form.html"
 
     parent_page = form_page.get_parent()
     explore_url = reverse("wagtailadmin_explore", args=[parent_page.id])
```

### Comparing `wagtail_zoom_integration-0.0.7/wagtailzoom/wagtail_hooks.py` & `wagtail_zoom_integration-0.0.8/wagtailzoom/wagtail_hooks.py`

 * *Files 5% similar despite different names*

```diff
@@ -15,20 +15,21 @@
         path('zoom-integration/<int:page_id>', zoom_integration_view, name="zoom_integration_view"),
     ]
 
 
 @hooks.register('register_page_listing_buttons')
 def page_listing_buttons(page, page_perms, next_url=None):
     if hasattr(page, "is_zoom_integration") and hasattr(page, "zoom_event"):
-        if page.zoom_event_id:
+        latest_revision = page.get_latest_revision_as_object()
+        if latest_revision.zoom_event_id and page.show_page_listing_zoom_integration_button():
             url = reverse("zoom_integration_view", args=[page.pk, ])
             yield wagtail_admin_widgets.PageListingButton(
                 "Zoom Integration",
                 url,
-                priority=40
+                priority=50
             )
 
 
 @hooks.register('after_publish_page')
 def show_zoom_integration_fields_warning(request, page):
     if hasattr(page, "is_zoom_integration") and hasattr(page, "zoom_event"):
         form_fields_changed = False
```

### Comparing `wagtail_zoom_integration-0.0.7/wagtailzoom/widgets.py` & `wagtail_zoom_integration-0.0.8/wagtailzoom/widgets.py`

 * *Files identical despite different names*

