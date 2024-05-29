# Comparing `tmp/aa-opcalendar-2.4.0.tar.gz` & `tmp/aa_opcalendar-3.0.0b1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "aa-opcalendar-2.4.0.tar", last modified: Sun Apr 16 09:12:25 2023, max compression
+gzip compressed data, was "aa_opcalendar-3.0.0b1.tar", last modified: Wed May 29 14:21:15 2024, max compression
```

## Comparing `aa-opcalendar-2.4.0.tar` & `aa_opcalendar-3.0.0b1.tar`

### file list

```diff
@@ -1,97 +1,112 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-16 09:12:25.591395 aa-opcalendar-2.4.0/
--rwxr-xr-x   0 root         (0) root         (0)     1070 2023-03-23 16:33:31.000000 aa-opcalendar-2.4.0/LICENSE
--rwxr-xr-x   0 root         (0) root         (0)      179 2023-03-23 16:33:31.000000 aa-opcalendar-2.4.0/MANIFEST.in
--rw-r--r--   0 root         (0) root         (0)    10967 2023-04-16 09:12:25.591395 aa-opcalendar-2.4.0/PKG-INFO
--rwxr-xr-x   0 root         (0) root         (0)    10205 2023-03-23 16:33:31.000000 aa-opcalendar-2.4.0/README.md
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-16 09:12:25.567399 aa-opcalendar-2.4.0/aa_opcalendar.egg-info/
--rw-r--r--   0 root         (0) root         (0)    10967 2023-04-16 09:12:25.000000 aa-opcalendar-2.4.0/aa_opcalendar.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)     2904 2023-04-16 09:12:25.000000 aa-opcalendar-2.4.0/aa_opcalendar.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2023-04-16 09:12:25.000000 aa-opcalendar-2.4.0/aa_opcalendar.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)       59 2023-04-16 09:12:25.000000 aa-opcalendar-2.4.0/aa_opcalendar.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)       34 2023-04-16 09:12:25.000000 aa-opcalendar-2.4.0/aa_opcalendar.egg-info/top_level.txt
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-16 09:12:25.567399 aa-opcalendar-2.4.0/eventcalendar/
--rwxr-xr-x   0 root         (0) root         (0)        0 2023-03-23 16:33:31.000000 aa-opcalendar-2.4.0/eventcalendar/__init__.py
--rwxr-xr-x   0 root         (0) root         (0)      403 2023-03-23 16:33:31.000000 aa-opcalendar-2.4.0/eventcalendar/asgi.py
--rwxr-xr-x   0 root         (0) root         (0)      453 2023-03-23 16:33:31.000000 aa-opcalendar-2.4.0/eventcalendar/helper.py
--rwxr-xr-x   0 root         (0) root         (0)     3217 2023-03-23 16:33:31.000000 aa-opcalendar-2.4.0/eventcalendar/settings.py
--rwxr-xr-x   0 root         (0) root         (0)      938 2023-03-23 16:33:31.000000 aa-opcalendar-2.4.0/eventcalendar/urls.py
--rwxr-xr-x   0 root         (0) root         (0)      747 2023-03-23 16:33:31.000000 aa-opcalendar-2.4.0/eventcalendar/views.py
--rwxr-xr-x   0 root         (0) root         (0)      403 2023-03-23 16:33:31.000000 aa-opcalendar-2.4.0/eventcalendar/wsgi.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-16 09:12:25.567399 aa-opcalendar-2.4.0/opcalendar/
--rwxr-xr-x   0 root         (0) root         (0)      104 2023-04-16 09:09:21.000000 aa-opcalendar-2.4.0/opcalendar/__init__.py
--rwxr-xr-x   0 root         (0) root         (0)     3814 2023-03-23 16:33:31.000000 aa-opcalendar-2.4.0/opcalendar/admin.py
--rwxr-xr-x   0 root         (0) root         (0)     3188 2023-03-23 16:33:31.000000 aa-opcalendar-2.4.0/opcalendar/app_settings.py
--rwxr-xr-x   0 root         (0) root         (0)      165 2023-03-23 16:33:31.000000 aa-opcalendar-2.4.0/opcalendar/apps.py
--rwxr-xr-x   0 root         (0) root         (0)     1018 2023-03-23 16:33:31.000000 aa-opcalendar-2.4.0/opcalendar/auth_hooks.py
--rwxr-xr-x   0 root         (0) root         (0)    10322 2023-03-23 16:33:31.000000 aa-opcalendar-2.4.0/opcalendar/calendar.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-16 09:12:25.567399 aa-opcalendar-2.4.0/opcalendar/cogs/
--rwxr-xr-x   0 root         (0) root         (0)     6898 2023-04-16 09:09:21.000000 aa-opcalendar-2.4.0/opcalendar/cogs/ops.py
--rwxr-xr-x   0 root         (0) root         (0)      553 2023-03-23 16:33:31.000000 aa-opcalendar-2.4.0/opcalendar/decorators.py
--rwxr-xr-x   0 root         (0) root         (0)     3320 2023-03-23 16:33:31.000000 aa-opcalendar-2.4.0/opcalendar/forms.py
--rwxr-xr-x   0 root         (0) root         (0)      772 2023-03-23 16:33:31.000000 aa-opcalendar-2.4.0/opcalendar/helpers.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-16 09:12:25.587395 aa-opcalendar-2.4.0/opcalendar/migrations/
--rwxr-xr-x   0 root         (0) root         (0)     7318 2023-03-23 16:33:31.000000 aa-opcalendar-2.4.0/opcalendar/migrations/0001_initial.py
--rwxr-xr-x   0 root         (0) root         (0)      769 2023-03-23 16:33:31.000000 aa-opcalendar-2.4.0/opcalendar/migrations/0002_auto_20201104_1054.py
--rwxr-xr-x   0 root         (0) root         (0)      827 2023-03-23 16:33:31.000000 aa-opcalendar-2.4.0/opcalendar/migrations/0003_eventhost.py
--rwxr-xr-x   0 root         (0) root         (0)      539 2023-03-23 16:33:31.000000 aa-opcalendar-2.4.0/opcalendar/migrations/0004_event_host.py
--rwxr-xr-x   0 root         (0) root         (0)      569 2023-03-23 16:33:31.000000 aa-opcalendar-2.4.0/opcalendar/migrations/0005_auto_20201104_1127.py
--rwxr-xr-x   0 root         (0) root         (0)     1946 2023-03-23 16:33:31.000000 aa-opcalendar-2.4.0/opcalendar/migrations/0006_auto_20201104_1201.py
--rwxr-xr-x   0 root         (0) root         (0)      403 2023-03-23 16:33:31.000000 aa-opcalendar-2.4.0/opcalendar/migrations/0007_eventhost_twitter.py
--rwxr-xr-x   0 root         (0) root         (0)      358 2023-03-23 16:33:31.000000 aa-opcalendar-2.4.0/opcalendar/migrations/0008_auto_20201105_0846.py
--rwxr-xr-x   0 root         (0) root         (0)      913 2023-03-23 16:33:31.000000 aa-opcalendar-2.4.0/opcalendar/migrations/0009_auto_20201105_0859.py
--rwxr-xr-x   0 root         (0) root         (0)      635 2023-03-23 16:33:31.000000 aa-opcalendar-2.4.0/opcalendar/migrations/0010_auto_20201105_1602.py
--rwxr-xr-x   0 root         (0) root         (0)     1568 2023-03-23 16:33:31.000000 aa-opcalendar-2.4.0/opcalendar/migrations/0011_eventimport.py
--rwxr-xr-x   0 root         (0) root         (0)      576 2023-03-23 16:33:31.000000 aa-opcalendar-2.4.0/opcalendar/migrations/0012_auto_20210112_0934.py
--rwxr-xr-x   0 root         (0) root         (0)      661 2023-03-23 16:33:31.000000 aa-opcalendar-2.4.0/opcalendar/migrations/0013_eventimport_creator.py
--rwxr-xr-x   0 root         (0) root         (0)     1957 2023-03-23 16:33:31.000000 aa-opcalendar-2.4.0/opcalendar/migrations/0014_auto_20210113_0836.py
--rwxr-xr-x   0 root         (0) root         (0)      671 2023-03-23 16:33:31.000000 aa-opcalendar-2.4.0/opcalendar/migrations/0015_eventimport_eve_character.py
--rwxr-xr-x   0 root         (0) root         (0)     4088 2023-03-23 16:33:31.000000 aa-opcalendar-2.4.0/opcalendar/migrations/0016_auto_20210119_1545.py
--rwxr-xr-x   0 root         (0) root         (0)     1295 2023-03-23 16:33:31.000000 aa-opcalendar-2.4.0/opcalendar/migrations/0017_auto_20210119_1626.py
--rwxr-xr-x   0 root         (0) root         (0)      684 2023-03-23 16:33:31.000000 aa-opcalendar-2.4.0/opcalendar/migrations/0018_auto_20210119_1701.py
--rwxr-xr-x   0 root         (0) root         (0)      708 2023-03-23 16:33:31.000000 aa-opcalendar-2.4.0/opcalendar/migrations/0019_auto_20210125_1005.py
--rwxr-xr-x   0 root         (0) root         (0)      459 2023-03-23 16:33:31.000000 aa-opcalendar-2.4.0/opcalendar/migrations/0020_auto_20210125_1007.py
--rwxr-xr-x   0 root         (0) root         (0)      404 2023-03-23 16:33:31.000000 aa-opcalendar-2.4.0/opcalendar/migrations/0021_eventhost_logo_url.py
--rwxr-xr-x   0 root         (0) root         (0)     2983 2023-03-23 16:33:31.000000 aa-opcalendar-2.4.0/opcalendar/migrations/0022_auto_20210222_1255.py
--rwxr-xr-x   0 root         (0) root         (0)    13049 2023-03-23 16:33:31.000000 aa-opcalendar-2.4.0/opcalendar/migrations/0023_auto_20210330_0632.py
--rwxr-xr-x   0 root         (0) root         (0)     2617 2023-03-23 16:33:31.000000 aa-opcalendar-2.4.0/opcalendar/migrations/0024_auto_20210429_1111.py
--rw-r--r--   0 root         (0) root         (0)      995 2023-03-23 16:33:31.000000 aa-opcalendar-2.4.0/opcalendar/migrations/0025_auto_20220115_1101.py
--rw-r--r--   0 root         (0) root         (0)      791 2023-03-23 16:33:31.000000 aa-opcalendar-2.4.0/opcalendar/migrations/0026_alter_event_repeat_event.py
--rwxr-xr-x   0 root         (0) root         (0)        0 2023-03-23 16:33:31.000000 aa-opcalendar-2.4.0/opcalendar/migrations/__init__.py
--rwxr-xr-x   0 root         (0) root         (0)    25244 2023-04-16 09:07:24.000000 aa-opcalendar-2.4.0/opcalendar/models.py
--rwxr-xr-x   0 root         (0) root         (0)      374 2023-03-23 16:33:31.000000 aa-opcalendar-2.4.0/opcalendar/providers.py
--rwxr-xr-x   0 root         (0) root         (0)    17736 2023-03-23 16:33:31.000000 aa-opcalendar-2.4.0/opcalendar/signals.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-16 09:12:25.567399 aa-opcalendar-2.4.0/opcalendar/static/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-16 09:12:25.591395 aa-opcalendar-2.4.0/opcalendar/static/opcalendar/
--rwxr-xr-x   0 root         (0) root         (0)     1204 2023-03-23 16:33:31.000000 aa-opcalendar-2.4.0/opcalendar/static/opcalendar/calendar.png
--rwxr-xr-x   0 root         (0) root         (0)     2845 2023-03-23 16:33:31.000000 aa-opcalendar-2.4.0/opcalendar/static/opcalendar/style_dark.css
--rw-r--r--   0 root         (0) root         (0)     2861 2023-03-23 16:33:31.000000 aa-opcalendar-2.4.0/opcalendar/static/opcalendar/style_light.css
--rwxr-xr-x   0 root         (0) root         (0)     1379 2023-03-23 16:33:31.000000 aa-opcalendar-2.4.0/opcalendar/static/opcalendar/terminate.png
--rwxr-xr-x   0 root         (0) root         (0)   947196 2023-03-23 16:33:31.000000 aa-opcalendar-2.4.0/opcalendar/swagger.json
--rwxr-xr-x   0 root         (0) root         (0)    14478 2023-03-23 16:33:31.000000 aa-opcalendar-2.4.0/opcalendar/tasks.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-16 09:12:25.567399 aa-opcalendar-2.4.0/opcalendar/templates/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-16 09:12:25.591395 aa-opcalendar-2.4.0/opcalendar/templates/opcalendar/
--rwxr-xr-x   0 root         (0) root         (0)      448 2023-03-23 16:33:31.000000 aa-opcalendar-2.4.0/opcalendar/templates/opcalendar/add_member.html
--rwxr-xr-x   0 root         (0) root         (0)     1194 2023-03-23 16:33:31.000000 aa-opcalendar-2.4.0/opcalendar/templates/opcalendar/base.html
--rwxr-xr-x   0 root         (0) root         (0)     3745 2023-03-23 16:33:31.000000 aa-opcalendar-2.4.0/opcalendar/templates/opcalendar/calendar.html
--rwxr-xr-x   0 root         (0) root         (0)     1751 2023-03-23 16:33:31.000000 aa-opcalendar-2.4.0/opcalendar/templates/opcalendar/event-add.html
--rwxr-xr-x   0 root         (0) root         (0)    10057 2023-03-23 16:33:31.000000 aa-opcalendar-2.4.0/opcalendar/templates/opcalendar/event-details.html
--rwxr-xr-x   0 root         (0) root         (0)     1219 2023-03-23 16:33:31.000000 aa-opcalendar-2.4.0/opcalendar/templates/opcalendar/event-edit.html
--rwxr-xr-x   0 root         (0) root         (0)      384 2023-03-23 16:33:31.000000 aa-opcalendar-2.4.0/opcalendar/templates/opcalendar/event_delete.html
--rwxr-xr-x   0 root         (0) root         (0)     4780 2023-03-23 16:33:31.000000 aa-opcalendar-2.4.0/opcalendar/templates/opcalendar/ingame-event-details.html
--rwxr-xr-x   0 root         (0) root         (0)      400 2023-03-23 16:33:31.000000 aa-opcalendar-2.4.0/opcalendar/templates/opcalendar/signup.html
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-16 09:12:25.591395 aa-opcalendar-2.4.0/opcalendar/tests/
--rwxr-xr-x   0 root         (0) root         (0)        0 2023-03-23 16:33:31.000000 aa-opcalendar-2.4.0/opcalendar/tests/__init__.py
--rwxr-xr-x   0 root         (0) root         (0)     4316 2023-03-23 16:33:31.000000 aa-opcalendar-2.4.0/opcalendar/tests/test_models.py
--rwxr-xr-x   0 root         (0) root         (0)    20000 2023-03-23 16:33:31.000000 aa-opcalendar-2.4.0/opcalendar/tests/test_tasks.py
--rwxr-xr-x   0 root         (0) root         (0)     2875 2023-03-23 16:33:31.000000 aa-opcalendar-2.4.0/opcalendar/tests/testdata.py
--rwxr-xr-x   0 root         (0) root         (0)     1246 2023-03-23 16:33:31.000000 aa-opcalendar-2.4.0/opcalendar/urls.py
--rwxr-xr-x   0 root         (0) root         (0)    10257 2023-03-23 16:33:31.000000 aa-opcalendar-2.4.0/opcalendar/utils.py
--rwxr-xr-x   0 root         (0) root         (0)    16275 2023-03-23 16:33:31.000000 aa-opcalendar-2.4.0/opcalendar/views.py
--rwxr-xr-x   0 root         (0) root         (0)      187 2023-04-16 09:12:25.591395 aa-opcalendar-2.4.0/setup.cfg
--rwxr-xr-x   0 root         (0) root         (0)     1485 2023-03-23 16:33:31.000000 aa-opcalendar-2.4.0/setup.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-16 09:12:25.591395 aa-opcalendar-2.4.0/testauth/
--rwxr-xr-x   0 root         (0) root         (0)       46 2023-03-23 16:33:31.000000 aa-opcalendar-2.4.0/testauth/__init__.py
--rwxr-xr-x   0 root         (0) root         (0)      611 2023-03-23 16:33:31.000000 aa-opcalendar-2.4.0/testauth/celery.py
--rwxr-xr-x   0 root         (0) root         (0)     9946 2023-03-23 16:33:31.000000 aa-opcalendar-2.4.0/testauth/settings.py
--rwxr-xr-x   0 root         (0) root         (0)      120 2023-03-23 16:33:31.000000 aa-opcalendar-2.4.0/testauth/urls.py
--rwxr-xr-x   0 root         (0) root         (0)      397 2023-03-23 16:33:31.000000 aa-opcalendar-2.4.0/testauth/wsgi.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-29 14:21:15.339625 aa_opcalendar-3.0.0b1/
+-rwxrwxrwx   0 root         (0) root         (0)     1070 2024-05-16 14:14:35.000000 aa_opcalendar-3.0.0b1/LICENSE
+-rwxrwxrwx   0 root         (0) root         (0)      179 2024-05-16 14:14:35.000000 aa_opcalendar-3.0.0b1/MANIFEST.in
+-rw-r--r--   0 root         (0) root         (0)    10083 2024-05-29 14:21:15.339625 aa_opcalendar-3.0.0b1/PKG-INFO
+-rwxrwxrwx   0 root         (0) root         (0)     9185 2024-05-29 12:50:54.000000 aa_opcalendar-3.0.0b1/README.md
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-29 14:21:15.339625 aa_opcalendar-3.0.0b1/aa_opcalendar.egg-info/
+-rw-r--r--   0 root         (0) root         (0)    10083 2024-05-29 14:21:15.000000 aa_opcalendar-3.0.0b1/aa_opcalendar.egg-info/PKG-INFO
+-rwxrwxrwx   0 root         (0) root         (0)     3636 2024-05-29 14:21:15.000000 aa_opcalendar-3.0.0b1/aa_opcalendar.egg-info/SOURCES.txt
+-rwxrwxrwx   0 root         (0) root         (0)        1 2024-05-29 14:21:15.000000 aa_opcalendar-3.0.0b1/aa_opcalendar.egg-info/dependency_links.txt
+-rwxrwxrwx   0 root         (0) root         (0)       59 2024-05-29 14:21:15.000000 aa_opcalendar-3.0.0b1/aa_opcalendar.egg-info/requires.txt
+-rwxrwxrwx   0 root         (0) root         (0)       34 2024-05-29 14:21:15.000000 aa_opcalendar-3.0.0b1/aa_opcalendar.egg-info/top_level.txt
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-29 14:21:15.303625 aa_opcalendar-3.0.0b1/eventcalendar/
+-rwxrwxrwx   0 root         (0) root         (0)        0 2024-05-16 14:14:35.000000 aa_opcalendar-3.0.0b1/eventcalendar/__init__.py
+-rwxrwxrwx   0 root         (0) root         (0)      403 2024-05-16 14:14:35.000000 aa_opcalendar-3.0.0b1/eventcalendar/asgi.py
+-rwxrwxrwx   0 root         (0) root         (0)      453 2024-05-16 14:14:35.000000 aa_opcalendar-3.0.0b1/eventcalendar/helper.py
+-rwxrwxrwx   0 root         (0) root         (0)     3217 2024-05-16 14:14:35.000000 aa_opcalendar-3.0.0b1/eventcalendar/settings.py
+-rwxrwxrwx   0 root         (0) root         (0)      938 2024-05-16 14:14:35.000000 aa_opcalendar-3.0.0b1/eventcalendar/urls.py
+-rwxrwxrwx   0 root         (0) root         (0)      747 2024-05-16 14:14:35.000000 aa_opcalendar-3.0.0b1/eventcalendar/views.py
+-rwxrwxrwx   0 root         (0) root         (0)      403 2024-05-16 14:14:35.000000 aa_opcalendar-3.0.0b1/eventcalendar/wsgi.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-29 14:21:15.307625 aa_opcalendar-3.0.0b1/opcalendar/
+-rwxrwxrwx   0 root         (0) root         (0)      106 2024-05-29 12:56:52.000000 aa_opcalendar-3.0.0b1/opcalendar/__init__.py
+-rwxrwxrwx   0 root         (0) root         (0)     4254 2024-05-19 12:13:34.000000 aa_opcalendar-3.0.0b1/opcalendar/admin.py
+-rwxrwxrwx   0 root         (0) root         (0)     3339 2024-05-20 14:29:05.000000 aa_opcalendar-3.0.0b1/opcalendar/app_settings.py
+-rwxrwxrwx   0 root         (0) root         (0)      165 2024-05-16 14:14:35.000000 aa_opcalendar-3.0.0b1/opcalendar/apps.py
+-rwxrwxrwx   0 root         (0) root         (0)     1104 2024-05-29 12:51:05.000000 aa_opcalendar-3.0.0b1/opcalendar/auth_hooks.py
+-rwxr-xr-x   0 root         (0) root         (0)    11174 2024-05-21 12:42:18.000000 aa_opcalendar-3.0.0b1/opcalendar/calendar.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-29 14:21:15.307625 aa_opcalendar-3.0.0b1/opcalendar/cogs/
+-rwxrwxrwx   0 root         (0) root         (0)     6898 2024-05-16 14:14:35.000000 aa_opcalendar-3.0.0b1/opcalendar/cogs/ops.py
+-rwxrwxrwx   0 root         (0) root         (0)      553 2024-05-16 14:14:35.000000 aa_opcalendar-3.0.0b1/opcalendar/decorators.py
+-rwxrwxrwx   0 root         (0) root         (0)     3984 2024-05-19 12:13:34.000000 aa_opcalendar-3.0.0b1/opcalendar/forms.py
+-rwxrwxrwx   0 root         (0) root         (0)      772 2024-05-16 14:14:35.000000 aa_opcalendar-3.0.0b1/opcalendar/helpers.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-29 14:21:15.319625 aa_opcalendar-3.0.0b1/opcalendar/migrations/
+-rwxrwxrwx   0 root         (0) root         (0)     7318 2024-05-16 14:14:35.000000 aa_opcalendar-3.0.0b1/opcalendar/migrations/0001_initial.py
+-rwxrwxrwx   0 root         (0) root         (0)      769 2024-05-16 14:14:35.000000 aa_opcalendar-3.0.0b1/opcalendar/migrations/0002_auto_20201104_1054.py
+-rwxrwxrwx   0 root         (0) root         (0)      827 2024-05-16 14:14:35.000000 aa_opcalendar-3.0.0b1/opcalendar/migrations/0003_eventhost.py
+-rwxrwxrwx   0 root         (0) root         (0)      539 2024-05-16 14:14:35.000000 aa_opcalendar-3.0.0b1/opcalendar/migrations/0004_event_host.py
+-rwxrwxrwx   0 root         (0) root         (0)      569 2024-05-16 14:14:35.000000 aa_opcalendar-3.0.0b1/opcalendar/migrations/0005_auto_20201104_1127.py
+-rwxrwxrwx   0 root         (0) root         (0)     1946 2024-05-16 14:14:35.000000 aa_opcalendar-3.0.0b1/opcalendar/migrations/0006_auto_20201104_1201.py
+-rwxrwxrwx   0 root         (0) root         (0)      403 2024-05-16 14:14:35.000000 aa_opcalendar-3.0.0b1/opcalendar/migrations/0007_eventhost_twitter.py
+-rwxrwxrwx   0 root         (0) root         (0)      358 2024-05-16 14:14:35.000000 aa_opcalendar-3.0.0b1/opcalendar/migrations/0008_auto_20201105_0846.py
+-rwxrwxrwx   0 root         (0) root         (0)      913 2024-05-16 14:14:35.000000 aa_opcalendar-3.0.0b1/opcalendar/migrations/0009_auto_20201105_0859.py
+-rwxrwxrwx   0 root         (0) root         (0)      635 2024-05-16 14:14:35.000000 aa_opcalendar-3.0.0b1/opcalendar/migrations/0010_auto_20201105_1602.py
+-rwxrwxrwx   0 root         (0) root         (0)     1568 2024-05-16 14:14:35.000000 aa_opcalendar-3.0.0b1/opcalendar/migrations/0011_eventimport.py
+-rwxrwxrwx   0 root         (0) root         (0)      576 2024-05-16 14:14:35.000000 aa_opcalendar-3.0.0b1/opcalendar/migrations/0012_auto_20210112_0934.py
+-rwxrwxrwx   0 root         (0) root         (0)      661 2024-05-16 14:14:35.000000 aa_opcalendar-3.0.0b1/opcalendar/migrations/0013_eventimport_creator.py
+-rwxrwxrwx   0 root         (0) root         (0)     1957 2024-05-16 14:14:35.000000 aa_opcalendar-3.0.0b1/opcalendar/migrations/0014_auto_20210113_0836.py
+-rwxrwxrwx   0 root         (0) root         (0)      671 2024-05-16 14:14:35.000000 aa_opcalendar-3.0.0b1/opcalendar/migrations/0015_eventimport_eve_character.py
+-rwxrwxrwx   0 root         (0) root         (0)     4088 2024-05-16 14:14:35.000000 aa_opcalendar-3.0.0b1/opcalendar/migrations/0016_auto_20210119_1545.py
+-rwxrwxrwx   0 root         (0) root         (0)     1295 2024-05-16 14:14:35.000000 aa_opcalendar-3.0.0b1/opcalendar/migrations/0017_auto_20210119_1626.py
+-rwxrwxrwx   0 root         (0) root         (0)      684 2024-05-16 14:14:35.000000 aa_opcalendar-3.0.0b1/opcalendar/migrations/0018_auto_20210119_1701.py
+-rwxrwxrwx   0 root         (0) root         (0)      708 2024-05-16 14:14:35.000000 aa_opcalendar-3.0.0b1/opcalendar/migrations/0019_auto_20210125_1005.py
+-rwxrwxrwx   0 root         (0) root         (0)      459 2024-05-16 14:14:35.000000 aa_opcalendar-3.0.0b1/opcalendar/migrations/0020_auto_20210125_1007.py
+-rwxrwxrwx   0 root         (0) root         (0)      404 2024-05-16 14:14:35.000000 aa_opcalendar-3.0.0b1/opcalendar/migrations/0021_eventhost_logo_url.py
+-rwxrwxrwx   0 root         (0) root         (0)     2983 2024-05-16 14:14:35.000000 aa_opcalendar-3.0.0b1/opcalendar/migrations/0022_auto_20210222_1255.py
+-rwxrwxrwx   0 root         (0) root         (0)    13049 2024-05-16 14:14:35.000000 aa_opcalendar-3.0.0b1/opcalendar/migrations/0023_auto_20210330_0632.py
+-rwxrwxrwx   0 root         (0) root         (0)     2617 2024-05-16 14:14:35.000000 aa_opcalendar-3.0.0b1/opcalendar/migrations/0024_auto_20210429_1111.py
+-rwxr-xr-x   0 root         (0) root         (0)      995 2024-05-18 03:55:12.000000 aa_opcalendar-3.0.0b1/opcalendar/migrations/0025_auto_20220115_1101.py
+-rwxr-xr-x   0 root         (0) root         (0)      791 2024-05-18 03:55:12.000000 aa_opcalendar-3.0.0b1/opcalendar/migrations/0026_alter_event_repeat_event.py
+-rw-r--r--   0 root         (0) root         (0)     2305 2024-05-29 12:57:47.000000 aa_opcalendar-3.0.0b1/opcalendar/migrations/0027_eventmember_comment_eventmember_status_usersettings.py
+-rwxrwxrwx   0 root         (0) root         (0)        0 2024-05-16 14:14:35.000000 aa_opcalendar-3.0.0b1/opcalendar/migrations/__init__.py
+-rwxr-xr-x   0 root         (0) root         (0)    26776 2024-05-20 12:49:29.000000 aa_opcalendar-3.0.0b1/opcalendar/models.py
+-rwxrwxrwx   0 root         (0) root         (0)      374 2024-05-16 14:14:35.000000 aa_opcalendar-3.0.0b1/opcalendar/providers.py
+-rwxrwxrwx   0 root         (0) root         (0)     7077 2024-05-20 14:43:05.000000 aa_opcalendar-3.0.0b1/opcalendar/signals.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-29 14:21:15.295625 aa_opcalendar-3.0.0b1/opcalendar/static/
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-29 14:21:15.319625 aa_opcalendar-3.0.0b1/opcalendar/static/opcalendar/
+-rwxrwxrwx   0 root         (0) root         (0)     1204 2024-05-16 14:14:35.000000 aa_opcalendar-3.0.0b1/opcalendar/static/opcalendar/calendar.png
+-rwxrwxrwx   0 root         (0) root         (0)     2845 2024-05-16 14:14:35.000000 aa_opcalendar-3.0.0b1/opcalendar/static/opcalendar/style_dark.css
+-rwxr-xr-x   0 root         (0) root         (0)     6988 2024-05-18 11:32:45.000000 aa_opcalendar-3.0.0b1/opcalendar/static/opcalendar/style_light.css
+-rwxrwxrwx   0 root         (0) root         (0)     1379 2024-05-16 14:14:35.000000 aa_opcalendar-3.0.0b1/opcalendar/static/opcalendar/terminate.png
+-rwxrwxrwx   0 root         (0) root         (0)   947196 2024-05-16 14:14:35.000000 aa_opcalendar-3.0.0b1/opcalendar/swagger.json
+-rwxrwxrwx   0 root         (0) root         (0)    14774 2024-05-16 14:14:35.000000 aa_opcalendar-3.0.0b1/opcalendar/tasks.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-29 14:21:15.295625 aa_opcalendar-3.0.0b1/opcalendar/templates/
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-29 14:21:15.327625 aa_opcalendar-3.0.0b1/opcalendar/templates/opcalendar/
+-rwxrwxrwx   0 root         (0) root         (0)      448 2024-05-16 14:14:35.000000 aa_opcalendar-3.0.0b1/opcalendar/templates/opcalendar/add_member.html
+-rwxr-xr-x   0 root         (0) root         (0)     1255 2024-05-18 03:55:12.000000 aa_opcalendar-3.0.0b1/opcalendar/templates/opcalendar/base.html
+-rwxr-xr-x   0 root         (0) root         (0)     2558 2024-05-21 12:42:18.000000 aa_opcalendar-3.0.0b1/opcalendar/templates/opcalendar/calendar.html
+-rwxr-xr-x   0 root         (0) root         (0)     1401 2024-05-18 03:55:12.000000 aa_opcalendar-3.0.0b1/opcalendar/templates/opcalendar/event-add.html
+-rwxr-xr-x   0 root         (0) root         (0)     2392 2024-05-19 08:16:20.000000 aa_opcalendar-3.0.0b1/opcalendar/templates/opcalendar/event-details.html
+-rwxr-xr-x   0 root         (0) root         (0)      900 2024-05-18 03:55:12.000000 aa_opcalendar-3.0.0b1/opcalendar/templates/opcalendar/event-edit.html
+-rwxrwxrwx   0 root         (0) root         (0)      384 2024-05-16 14:14:35.000000 aa_opcalendar-3.0.0b1/opcalendar/templates/opcalendar/event_delete.html
+-rwxrwxrwx   0 root         (0) root         (0)     4607 2024-05-19 06:53:22.000000 aa_opcalendar-3.0.0b1/opcalendar/templates/opcalendar/ingame-event-details.html
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-29 14:21:15.303625 aa_opcalendar-3.0.0b1/opcalendar/templates/opcalendar/partials/
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-29 14:21:15.339625 aa_opcalendar-3.0.0b1/opcalendar/templates/opcalendar/partials/base/
+-rw-r--r--   0 root         (0) root         (0)      943 2024-05-19 12:04:57.000000 aa_opcalendar-3.0.0b1/opcalendar/templates/opcalendar/partials/base/menu.html
+-rw-r--r--   0 root         (0) root         (0)      247 2024-05-18 03:55:12.000000 aa_opcalendar-3.0.0b1/opcalendar/templates/opcalendar/partials/base/stylesheets.html
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-29 14:21:15.339625 aa_opcalendar-3.0.0b1/opcalendar/templates/opcalendar/partials/calendar/
+-rw-r--r--   0 root         (0) root         (0)     1995 2024-05-20 13:01:40.000000 aa_opcalendar-3.0.0b1/opcalendar/templates/opcalendar/partials/calendar/legends.html
+-rw-r--r--   0 root         (0) root         (0)      672 2024-05-19 06:58:32.000000 aa_opcalendar-3.0.0b1/opcalendar/templates/opcalendar/partials/calendar/navigation.html
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-29 14:21:15.339625 aa_opcalendar-3.0.0b1/opcalendar/templates/opcalendar/partials/event_details/
+-rw-r--r--   0 root         (0) root         (0)     1386 2024-05-18 03:55:12.000000 aa_opcalendar-3.0.0b1/opcalendar/templates/opcalendar/partials/event_details/details.html
+-rw-r--r--   0 root         (0) root         (0)     1651 2024-05-18 03:55:12.000000 aa_opcalendar-3.0.0b1/opcalendar/templates/opcalendar/partials/event_details/host.html
+-rw-r--r--   0 root         (0) root         (0)     1215 2024-05-18 08:14:23.000000 aa_opcalendar-3.0.0b1/opcalendar/templates/opcalendar/partials/event_details/navigation.html
+-rw-r--r--   0 root         (0) root         (0)      945 2024-05-18 11:33:31.000000 aa_opcalendar-3.0.0b1/opcalendar/templates/opcalendar/partials/event_details/signups.html
+-rw-r--r--   0 root         (0) root         (0)     1718 2024-05-18 11:34:28.000000 aa_opcalendar-3.0.0b1/opcalendar/templates/opcalendar/partials/event_details/signups_navigation.html
+-rwxrwxrwx   0 root         (0) root         (0)      400 2024-05-16 14:14:35.000000 aa_opcalendar-3.0.0b1/opcalendar/templates/opcalendar/signup.html
+-rw-rw-r--   0 root         (0) root         (0)     1026 2024-05-20 11:48:14.000000 aa_opcalendar-3.0.0b1/opcalendar/templates/opcalendar/user_settings.html
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-29 14:21:15.339625 aa_opcalendar-3.0.0b1/opcalendar/tests/
+-rwxrwxrwx   0 root         (0) root         (0)        0 2024-05-16 14:14:35.000000 aa_opcalendar-3.0.0b1/opcalendar/tests/__init__.py
+-rwxrwxrwx   0 root         (0) root         (0)     4316 2024-05-16 14:14:35.000000 aa_opcalendar-3.0.0b1/opcalendar/tests/test_models.py
+-rwxrwxrwx   0 root         (0) root         (0)    20005 2024-05-16 14:14:35.000000 aa_opcalendar-3.0.0b1/opcalendar/tests/test_tasks.py
+-rwxrwxrwx   0 root         (0) root         (0)     2880 2024-05-16 14:14:35.000000 aa_opcalendar-3.0.0b1/opcalendar/tests/testdata.py
+-rwxrwxrwx   0 root         (0) root         (0)     1909 2024-05-29 12:47:00.000000 aa_opcalendar-3.0.0b1/opcalendar/urls.py
+-rwxrwxrwx   0 root         (0) root         (0)    10257 2024-05-16 14:14:35.000000 aa_opcalendar-3.0.0b1/opcalendar/utils.py
+-rwxr-xr-x   0 root         (0) root         (0)    18850 2024-05-29 12:51:04.000000 aa_opcalendar-3.0.0b1/opcalendar/views.py
+-rwxrwxrwx   0 root         (0) root         (0)      187 2024-05-29 14:21:15.339625 aa_opcalendar-3.0.0b1/setup.cfg
+-rwxrwxrwx   0 root         (0) root         (0)     1485 2024-05-16 14:14:35.000000 aa_opcalendar-3.0.0b1/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-29 14:21:15.339625 aa_opcalendar-3.0.0b1/testauth/
+-rwxrwxrwx   0 root         (0) root         (0)       46 2024-05-16 14:14:35.000000 aa_opcalendar-3.0.0b1/testauth/__init__.py
+-rwxrwxrwx   0 root         (0) root         (0)      611 2024-05-16 14:14:35.000000 aa_opcalendar-3.0.0b1/testauth/celery.py
+-rwxrwxrwx   0 root         (0) root         (0)     9946 2024-05-16 14:14:35.000000 aa_opcalendar-3.0.0b1/testauth/settings.py
+-rwxrwxrwx   0 root         (0) root         (0)      120 2024-05-16 14:14:35.000000 aa_opcalendar-3.0.0b1/testauth/urls.py
+-rwxrwxrwx   0 root         (0) root         (0)      397 2024-05-16 14:14:35.000000 aa_opcalendar-3.0.0b1/testauth/wsgi.py
```

### Comparing `aa-opcalendar-2.4.0/LICENSE` & `aa_opcalendar-3.0.0b1/LICENSE`

 * *Files identical despite different names*

### Comparing `aa-opcalendar-2.4.0/PKG-INFO` & `aa_opcalendar-3.0.0b1/PKG-INFO`

 * *Files 10% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: aa-opcalendar
-Version: 2.4.0
+Version: 3.0.0b1
 Summary: Event calendar plugin app for Alliance Auth
 Home-page: https://gitlab.com/paulipa/allianceauth-opcalendar
 Author: Ikarus Cesaille
 Author-email: contact@eve-linknet.com
 License: MIT
 Classifier: Environment :: Web Environment
 Classifier: Framework :: Django
@@ -14,14 +14,19 @@
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3.5
 Classifier: Topic :: Internet :: WWW/HTTP
 Classifier: Topic :: Internet :: WWW/HTTP :: Dynamic Content
 Description-Content-Type: text/markdown
 License-File: LICENSE
+Requires-Dist: allianceauth>=2.8.0
+Requires-Dist: feedparser
+Requires-Dist: ics>=0.7.2
+Requires-Dist: pytz
+Requires-Dist: django-ical
 
 # Operation Calendar
 
 An operation calendar app for Alliance Auth to display fleet operations and other events.
 
 ![release](https://img.shields.io/pypi/v/aa-opcalendar??label=release) ![python](https://img.shields.io/pypi/pyversions/aa-opcalendar?) ![license](https://img.shields.io/badge/license-MIT-green)
 
@@ -106,14 +111,15 @@
  --- | --- | ---
 OPCALENDAR_NOTIFY_IMPORTS | Wheter to send out discord notifications for ingame and public NPSI events | True
 OPCALENDAR_DISPLAY_STRUCTURETIMERS | whether we should inculde timers from the structuretimers plugin in the calendar. Inherits view permissions from aa-structuretimers | True
 OPCALENDAR_DISPLAY_MOONMINING | whether we should inculde extractions from the aa-moonmining plugin in the calendar. Inherits view permissions from aa-moonmining | True
 OPCALENDAR_DISCORD_OPS_DISPLAY_EXTERNAL | whether we display external hosts such as ingame hosts in the discord ops command filters | False
 OPCALENDAR_DISPLAY_MOONMINING_TAGS | Display the rarity tag of aa-moonmining moons if the moonmining plugin is installed | True
 OPCALENDAR_DISPLAY_MOONMINING_ARRIVAL_TIME | Displays aa-moonmining extraction time based on arrival time. Set to False to display as auto fracture time | True
+OPCALENDAR_NOTIFY_REPEAT_EVENTS | If repeated events should also be created as webhook pings on discord. Can create spam if the event repeat is set to high | True
 
 
 ## Setup
 Before you are able to create new events on the front end you will need to setup the needed categories and visibility filters for your events.
 
 ### 1. Host
 Hosts are for identifying reasons. If you run a single corporation or alliance entity you most likely only want one host. If you want to extend the calendar with other hosts such as NPSI communities you can create a host for each different entity.
@@ -195,49 +201,24 @@
 On default the ingame events you import have no visibility filter and no category. This means they **will be visible for everyone**.
 
 If you wish to add a visibility filter or a category similar to the manual events simply go to the `admin panel -> Ingame event owners` and select a filter and a category for the owner.
 
 After selecing a visibility filter and a category the ingame events will behave similar to the manual events and respect the group and state restrictions set for the visibility filters.
 
 ### Ical feed setup (optional)
-Opcalendar has the ability to generate a standard ical formated feed for pushing out events. To push out evets to the feed without login requirement requires editing the allianceauth url file as on default all pages are locked behind a login requirement.
+Opcalendar has the ability to generate a standard ical formated feed for pushing out events. To push out evets to the feed without login requirement requires editing auth settings file.
 
 #### Feed setup
-1. Open up the event visibility category and check the box to include it in the ical feed.
-2. Open the alliance auth `urls.py` file that is located on default in the following path `/home/allianceserver/myauth/myauth/urls.py`
-3. On default the file looks something like this:
-```
-from django.conf.urls import include, url
-from allianceauth import urls
+1. Open up the event visibility category and check the box to include it in the ical feed. Only categories tagged with this box will show up on the feed.
 
-urlpatterns = [
-    url(r'', include(urls)),
-]
+2. Add 'opcalendar' to the local settings file settings.py in the APPS_WITH_PUBLIC_VIEWS or create the section if you do not have it:
 
-handler500 = 'allianceauth.views.Generic500Redirect'
-handler404 = 'allianceauth.views.Generic404Redirect'
-handler403 = 'allianceauth.views.Generic403Redirect'
-handler400 = 'allianceauth.views.Generic400Redirect'
-```
-4. Include the following 2 lines in the file:
-	- `from opcalendar.views import EventFeed #Added import for opcalendar ical feed` bellow the imports on top of the file
-	- `url(r'^opcalendar/feed.ics', EventFeed()), #Opcalendar feed url` in the `urlpatterns` **before** the `url(r'', include(urls)),` line
-Your file `urls.py` file should now look like this:
-```
-from django.conf.urls import include, url
-from allianceauth import urls
-from opcalendar.views import EventFeed #Added import for opcalendar ical feed
-
-urlpatterns = [
-    url(r'^opcalendar/feed.ics', EventFeed()), #Opcalendar feed url
-    url(r'', include(urls)),
+```
+APPS_WITH_PUBLIC_VIEWS = [
+    'opcalendar',
 ]
-
-handler500 = 'allianceauth.views.Generic500Redirect'
-handler404 = 'allianceauth.views.Generic404Redirect'
-handler403 = 'allianceauth.views.Generic403Redirect'
-handler400 = 'allianceauth.views.Generic400Redirect'
 ```
-5. You can now access the ical feed at `auth.example.com/opcalendar/feed.ics`
+
+3. You can now access the ical feed at `auth.example.com/opcalendar/feed.ics`
 
 ## Contributing
 Make sure you have signed the [License Agreement](https://developers.eveonline.com/resource/license-agreement) by logging in at https://developers.eveonline.com before submitting any pull requests. All bug fixes or features must not include extra superfluous formatting changes.
```

### Comparing `aa-opcalendar-2.4.0/README.md` & `aa_opcalendar-3.0.0b1/aa_opcalendar.egg-info/PKG-INFO`

 * *Files 12% similar despite different names*

```diff
@@ -1,7 +1,33 @@
+Metadata-Version: 2.1
+Name: aa-opcalendar
+Version: 3.0.0b1
+Summary: Event calendar plugin app for Alliance Auth
+Home-page: https://gitlab.com/paulipa/allianceauth-opcalendar
+Author: Ikarus Cesaille
+Author-email: contact@eve-linknet.com
+License: MIT
+Classifier: Environment :: Web Environment
+Classifier: Framework :: Django
+Classifier: Framework :: Django :: 2.2
+Classifier: Intended Audience :: Developers
+Classifier: License :: OSI Approved :: MIT License
+Classifier: Operating System :: OS Independent
+Classifier: Programming Language :: Python
+Classifier: Programming Language :: Python :: 3.5
+Classifier: Topic :: Internet :: WWW/HTTP
+Classifier: Topic :: Internet :: WWW/HTTP :: Dynamic Content
+Description-Content-Type: text/markdown
+License-File: LICENSE
+Requires-Dist: allianceauth>=2.8.0
+Requires-Dist: feedparser
+Requires-Dist: ics>=0.7.2
+Requires-Dist: pytz
+Requires-Dist: django-ical
+
 # Operation Calendar
 
 An operation calendar app for Alliance Auth to display fleet operations and other events.
 
 ![release](https://img.shields.io/pypi/v/aa-opcalendar??label=release) ![python](https://img.shields.io/pypi/pyversions/aa-opcalendar?) ![license](https://img.shields.io/badge/license-MIT-green)
 
 ## Includes:
@@ -85,14 +111,15 @@
  --- | --- | ---
 OPCALENDAR_NOTIFY_IMPORTS | Wheter to send out discord notifications for ingame and public NPSI events | True
 OPCALENDAR_DISPLAY_STRUCTURETIMERS | whether we should inculde timers from the structuretimers plugin in the calendar. Inherits view permissions from aa-structuretimers | True
 OPCALENDAR_DISPLAY_MOONMINING | whether we should inculde extractions from the aa-moonmining plugin in the calendar. Inherits view permissions from aa-moonmining | True
 OPCALENDAR_DISCORD_OPS_DISPLAY_EXTERNAL | whether we display external hosts such as ingame hosts in the discord ops command filters | False
 OPCALENDAR_DISPLAY_MOONMINING_TAGS | Display the rarity tag of aa-moonmining moons if the moonmining plugin is installed | True
 OPCALENDAR_DISPLAY_MOONMINING_ARRIVAL_TIME | Displays aa-moonmining extraction time based on arrival time. Set to False to display as auto fracture time | True
+OPCALENDAR_NOTIFY_REPEAT_EVENTS | If repeated events should also be created as webhook pings on discord. Can create spam if the event repeat is set to high | True
 
 
 ## Setup
 Before you are able to create new events on the front end you will need to setup the needed categories and visibility filters for your events.
 
 ### 1. Host
 Hosts are for identifying reasons. If you run a single corporation or alliance entity you most likely only want one host. If you want to extend the calendar with other hosts such as NPSI communities you can create a host for each different entity.
@@ -174,49 +201,24 @@
 On default the ingame events you import have no visibility filter and no category. This means they **will be visible for everyone**.
 
 If you wish to add a visibility filter or a category similar to the manual events simply go to the `admin panel -> Ingame event owners` and select a filter and a category for the owner.
 
 After selecing a visibility filter and a category the ingame events will behave similar to the manual events and respect the group and state restrictions set for the visibility filters.
 
 ### Ical feed setup (optional)
-Opcalendar has the ability to generate a standard ical formated feed for pushing out events. To push out evets to the feed without login requirement requires editing the allianceauth url file as on default all pages are locked behind a login requirement.
+Opcalendar has the ability to generate a standard ical formated feed for pushing out events. To push out evets to the feed without login requirement requires editing auth settings file.
 
 #### Feed setup
-1. Open up the event visibility category and check the box to include it in the ical feed.
-2. Open the alliance auth `urls.py` file that is located on default in the following path `/home/allianceserver/myauth/myauth/urls.py`
-3. On default the file looks something like this:
-```
-from django.conf.urls import include, url
-from allianceauth import urls
+1. Open up the event visibility category and check the box to include it in the ical feed. Only categories tagged with this box will show up on the feed.
 
-urlpatterns = [
-    url(r'', include(urls)),
-]
+2. Add 'opcalendar' to the local settings file settings.py in the APPS_WITH_PUBLIC_VIEWS or create the section if you do not have it:
 
-handler500 = 'allianceauth.views.Generic500Redirect'
-handler404 = 'allianceauth.views.Generic404Redirect'
-handler403 = 'allianceauth.views.Generic403Redirect'
-handler400 = 'allianceauth.views.Generic400Redirect'
-```
-4. Include the following 2 lines in the file:
-	- `from opcalendar.views import EventFeed #Added import for opcalendar ical feed` bellow the imports on top of the file
-	- `url(r'^opcalendar/feed.ics', EventFeed()), #Opcalendar feed url` in the `urlpatterns` **before** the `url(r'', include(urls)),` line
-Your file `urls.py` file should now look like this:
-```
-from django.conf.urls import include, url
-from allianceauth import urls
-from opcalendar.views import EventFeed #Added import for opcalendar ical feed
-
-urlpatterns = [
-    url(r'^opcalendar/feed.ics', EventFeed()), #Opcalendar feed url
-    url(r'', include(urls)),
+```
+APPS_WITH_PUBLIC_VIEWS = [
+    'opcalendar',
 ]
-
-handler500 = 'allianceauth.views.Generic500Redirect'
-handler404 = 'allianceauth.views.Generic404Redirect'
-handler403 = 'allianceauth.views.Generic403Redirect'
-handler400 = 'allianceauth.views.Generic400Redirect'
 ```
-5. You can now access the ical feed at `auth.example.com/opcalendar/feed.ics`
+
+3. You can now access the ical feed at `auth.example.com/opcalendar/feed.ics`
 
 ## Contributing
 Make sure you have signed the [License Agreement](https://developers.eveonline.com/resource/license-agreement) by logging in at https://developers.eveonline.com before submitting any pull requests. All bug fixes or features must not include extra superfluous formatting changes.
```

### Comparing `aa-opcalendar-2.4.0/aa_opcalendar.egg-info/PKG-INFO` & `aa_opcalendar-3.0.0b1/README.md`

 * *Files 22% similar despite different names*

```diff
@@ -1,28 +1,7 @@
-Metadata-Version: 2.1
-Name: aa-opcalendar
-Version: 2.4.0
-Summary: Event calendar plugin app for Alliance Auth
-Home-page: https://gitlab.com/paulipa/allianceauth-opcalendar
-Author: Ikarus Cesaille
-Author-email: contact@eve-linknet.com
-License: MIT
-Classifier: Environment :: Web Environment
-Classifier: Framework :: Django
-Classifier: Framework :: Django :: 2.2
-Classifier: Intended Audience :: Developers
-Classifier: License :: OSI Approved :: MIT License
-Classifier: Operating System :: OS Independent
-Classifier: Programming Language :: Python
-Classifier: Programming Language :: Python :: 3.5
-Classifier: Topic :: Internet :: WWW/HTTP
-Classifier: Topic :: Internet :: WWW/HTTP :: Dynamic Content
-Description-Content-Type: text/markdown
-License-File: LICENSE
-
 # Operation Calendar
 
 An operation calendar app for Alliance Auth to display fleet operations and other events.
 
 ![release](https://img.shields.io/pypi/v/aa-opcalendar??label=release) ![python](https://img.shields.io/pypi/pyversions/aa-opcalendar?) ![license](https://img.shields.io/badge/license-MIT-green)
 
 ## Includes:
@@ -106,14 +85,15 @@
  --- | --- | ---
 OPCALENDAR_NOTIFY_IMPORTS | Wheter to send out discord notifications for ingame and public NPSI events | True
 OPCALENDAR_DISPLAY_STRUCTURETIMERS | whether we should inculde timers from the structuretimers plugin in the calendar. Inherits view permissions from aa-structuretimers | True
 OPCALENDAR_DISPLAY_MOONMINING | whether we should inculde extractions from the aa-moonmining plugin in the calendar. Inherits view permissions from aa-moonmining | True
 OPCALENDAR_DISCORD_OPS_DISPLAY_EXTERNAL | whether we display external hosts such as ingame hosts in the discord ops command filters | False
 OPCALENDAR_DISPLAY_MOONMINING_TAGS | Display the rarity tag of aa-moonmining moons if the moonmining plugin is installed | True
 OPCALENDAR_DISPLAY_MOONMINING_ARRIVAL_TIME | Displays aa-moonmining extraction time based on arrival time. Set to False to display as auto fracture time | True
+OPCALENDAR_NOTIFY_REPEAT_EVENTS | If repeated events should also be created as webhook pings on discord. Can create spam if the event repeat is set to high | True
 
 
 ## Setup
 Before you are able to create new events on the front end you will need to setup the needed categories and visibility filters for your events.
 
 ### 1. Host
 Hosts are for identifying reasons. If you run a single corporation or alliance entity you most likely only want one host. If you want to extend the calendar with other hosts such as NPSI communities you can create a host for each different entity.
@@ -195,49 +175,24 @@
 On default the ingame events you import have no visibility filter and no category. This means they **will be visible for everyone**.
 
 If you wish to add a visibility filter or a category similar to the manual events simply go to the `admin panel -> Ingame event owners` and select a filter and a category for the owner.
 
 After selecing a visibility filter and a category the ingame events will behave similar to the manual events and respect the group and state restrictions set for the visibility filters.
 
 ### Ical feed setup (optional)
-Opcalendar has the ability to generate a standard ical formated feed for pushing out events. To push out evets to the feed without login requirement requires editing the allianceauth url file as on default all pages are locked behind a login requirement.
+Opcalendar has the ability to generate a standard ical formated feed for pushing out events. To push out evets to the feed without login requirement requires editing auth settings file.
 
 #### Feed setup
-1. Open up the event visibility category and check the box to include it in the ical feed.
-2. Open the alliance auth `urls.py` file that is located on default in the following path `/home/allianceserver/myauth/myauth/urls.py`
-3. On default the file looks something like this:
-```
-from django.conf.urls import include, url
-from allianceauth import urls
+1. Open up the event visibility category and check the box to include it in the ical feed. Only categories tagged with this box will show up on the feed.
 
-urlpatterns = [
-    url(r'', include(urls)),
-]
+2. Add 'opcalendar' to the local settings file settings.py in the APPS_WITH_PUBLIC_VIEWS or create the section if you do not have it:
 
-handler500 = 'allianceauth.views.Generic500Redirect'
-handler404 = 'allianceauth.views.Generic404Redirect'
-handler403 = 'allianceauth.views.Generic403Redirect'
-handler400 = 'allianceauth.views.Generic400Redirect'
-```
-4. Include the following 2 lines in the file:
-	- `from opcalendar.views import EventFeed #Added import for opcalendar ical feed` bellow the imports on top of the file
-	- `url(r'^opcalendar/feed.ics', EventFeed()), #Opcalendar feed url` in the `urlpatterns` **before** the `url(r'', include(urls)),` line
-Your file `urls.py` file should now look like this:
-```
-from django.conf.urls import include, url
-from allianceauth import urls
-from opcalendar.views import EventFeed #Added import for opcalendar ical feed
-
-urlpatterns = [
-    url(r'^opcalendar/feed.ics', EventFeed()), #Opcalendar feed url
-    url(r'', include(urls)),
+```
+APPS_WITH_PUBLIC_VIEWS = [
+    'opcalendar',
 ]
-
-handler500 = 'allianceauth.views.Generic500Redirect'
-handler404 = 'allianceauth.views.Generic404Redirect'
-handler403 = 'allianceauth.views.Generic403Redirect'
-handler400 = 'allianceauth.views.Generic400Redirect'
 ```
-5. You can now access the ical feed at `auth.example.com/opcalendar/feed.ics`
+
+3. You can now access the ical feed at `auth.example.com/opcalendar/feed.ics`
 
 ## Contributing
 Make sure you have signed the [License Agreement](https://developers.eveonline.com/resource/license-agreement) by logging in at https://developers.eveonline.com before submitting any pull requests. All bug fixes or features must not include extra superfluous formatting changes.
```

### Comparing `aa-opcalendar-2.4.0/aa_opcalendar.egg-info/SOURCES.txt` & `aa_opcalendar-3.0.0b1/aa_opcalendar.egg-info/SOURCES.txt`

 * *Files 18% similar despite different names*

```diff
@@ -55,28 +55,39 @@
 opcalendar/migrations/0020_auto_20210125_1007.py
 opcalendar/migrations/0021_eventhost_logo_url.py
 opcalendar/migrations/0022_auto_20210222_1255.py
 opcalendar/migrations/0023_auto_20210330_0632.py
 opcalendar/migrations/0024_auto_20210429_1111.py
 opcalendar/migrations/0025_auto_20220115_1101.py
 opcalendar/migrations/0026_alter_event_repeat_event.py
+opcalendar/migrations/0027_eventmember_comment_eventmember_status_usersettings.py
 opcalendar/migrations/__init__.py
 opcalendar/static/opcalendar/calendar.png
 opcalendar/static/opcalendar/style_dark.css
 opcalendar/static/opcalendar/style_light.css
 opcalendar/static/opcalendar/terminate.png
 opcalendar/templates/opcalendar/add_member.html
 opcalendar/templates/opcalendar/base.html
 opcalendar/templates/opcalendar/calendar.html
 opcalendar/templates/opcalendar/event-add.html
 opcalendar/templates/opcalendar/event-details.html
 opcalendar/templates/opcalendar/event-edit.html
 opcalendar/templates/opcalendar/event_delete.html
 opcalendar/templates/opcalendar/ingame-event-details.html
 opcalendar/templates/opcalendar/signup.html
+opcalendar/templates/opcalendar/user_settings.html
+opcalendar/templates/opcalendar/partials/base/menu.html
+opcalendar/templates/opcalendar/partials/base/stylesheets.html
+opcalendar/templates/opcalendar/partials/calendar/legends.html
+opcalendar/templates/opcalendar/partials/calendar/navigation.html
+opcalendar/templates/opcalendar/partials/event_details/details.html
+opcalendar/templates/opcalendar/partials/event_details/host.html
+opcalendar/templates/opcalendar/partials/event_details/navigation.html
+opcalendar/templates/opcalendar/partials/event_details/signups.html
+opcalendar/templates/opcalendar/partials/event_details/signups_navigation.html
 opcalendar/tests/__init__.py
 opcalendar/tests/test_models.py
 opcalendar/tests/test_tasks.py
 opcalendar/tests/testdata.py
 testauth/__init__.py
 testauth/celery.py
 testauth/settings.py
```

### Comparing `aa-opcalendar-2.4.0/eventcalendar/settings.py` & `aa_opcalendar-3.0.0b1/eventcalendar/settings.py`

 * *Files identical despite different names*

### Comparing `aa-opcalendar-2.4.0/eventcalendar/urls.py` & `aa_opcalendar-3.0.0b1/eventcalendar/urls.py`

 * *Files identical despite different names*

### Comparing `aa-opcalendar-2.4.0/eventcalendar/views.py` & `aa_opcalendar-3.0.0b1/eventcalendar/views.py`

 * *Files identical despite different names*

### Comparing `aa-opcalendar-2.4.0/opcalendar/admin.py` & `aa_opcalendar-3.0.0b1/opcalendar/admin.py`

 * *Files 18% similar despite different names*

```diff
@@ -5,14 +5,16 @@
     EventCategory,
     WebHook,
     EventHost,
     EventImport,
     Owner,
     IngameEvents,
     EventVisibility,
+    EventMember,
+    UserSettings,
 )
 from .forms import EventVisibilityAdminForm, EventCategoryAdminForm
 
 
 def custom_filter(title):
     """
     custom filter for model properties
@@ -171,7 +173,20 @@
     list_display = (
         "title",
         "host",
         "operation_type",
         "event_visibility",
         "external",
     )
+
+
+@admin.register(EventMember)
+class EventMemberAdmin(admin.ModelAdmin):
+    list_display = ("event", "character", "status")
+    list_filter = ("status",)
+    search_fields = ("character__name", "event__name")
+
+
+@admin.register(UserSettings)
+class UserSettingsAdmin(admin.ModelAdmin):
+    list_display = ("user", "disable_discord_notifications", "use_local_times")
+    search_fields = ("user__username",)
```

### Comparing `aa-opcalendar-2.4.0/opcalendar/app_settings.py` & `aa_opcalendar-3.0.0b1/opcalendar/app_settings.py`

 * *Files 8% similar despite different names*

```diff
@@ -44,14 +44,17 @@
 )
 
 # whether we display external hosts in the discord ops command filters
 OPCALENDAR_DISCORD_OPS_DISPLAY_EXTERNAL = clean_setting(
     "OPCALENDAR_DISCORD_OPS_DISPLAY_EXTERNAL", False
 )
 
+# whether events with repeat should be sent over the webhook
+OPCALENDAR_NOTIFY_REPEAT_EVENTS = clean_setting("OPCALENDAR_NOTIFY_REPEAT_EVENTS", True)
+
 OPCALENDAR_EVE_UNI_URL = "https://portal.eveuniversity.org/api/getcalendar"
 OPCALENDAR_SPECTRE_URL = "https://www.spectre-fleet.space/engagement/events/rss"
 OPCALENDAR_FUNINC_URL = "https://calendar.google.com/calendar/ical/og3uh76l8ul3dfgbie03fbbgs8%40group.calendar.google.com/private-f466889b44741fd7249e99e21ac171ff/basic.ics"
 OPCALENDAR_FRIDAY_YARRRR_URL = "https://calendar.google.com/calendar/ical/vl43scrg7olk01fv7g79hsbe74%40group.calendar.google.com/public/basic.ics"
 OPCALENDAR_REDEMPTION_ROAD_URL = "https://calendar.google.com/calendar/ical/5o3gpum6ek2irk12f0hnhfdtrs%40group.calendar.google.com/public/basic.ics"
 OPCALENDAR_CAS_URL = "https://calendar.google.com/calendar/ical/0sqru3js6pb1p71e7n1ko91rqs%40group.calendar.google.com/public/basic.ics"
 OPCALENDAR_FWAMING_DWAGONS_URL = "https://calendar.google.com/calendar/ical/l0mnjo7ormaq9gomap0cke4kqk%40group.calendar.google.com/public/basic.ics"
```

### Comparing `aa-opcalendar-2.4.0/opcalendar/auth_hooks.py` & `aa_opcalendar-3.0.0b1/opcalendar/auth_hooks.py`

 * *Files 8% similar despite different names*

```diff
@@ -27,13 +27,18 @@
 @hooks.register("menu_item_hook")
 def register_menu():
     return OpcalendarMenuItem()
 
 
 @hooks.register("url_hook")
 def register_urls():
-    return UrlHook(urls, "opcalendar", r"^opcalendar/")
+    return UrlHook(
+        urls,
+        "opcalendar",
+        r"^opcalendar/",
+        excluded_views=["opcalendar.views.EventFeed"],
+    )
 
 
 @hooks.register("discord_cogs_hook")
 def register_cogs():
     return ["opcalendar.cogs.ops"]
```

### Comparing `aa-opcalendar-2.4.0/opcalendar/cogs/ops.py` & `aa_opcalendar-3.0.0b1/opcalendar/cogs/ops.py`

 * *Files identical despite different names*

### Comparing `aa-opcalendar-2.4.0/opcalendar/decorators.py` & `aa_opcalendar-3.0.0b1/opcalendar/decorators.py`

 * *Files identical despite different names*

### Comparing `aa-opcalendar-2.4.0/opcalendar/forms.py` & `aa_opcalendar-3.0.0b1/opcalendar/forms.py`

 * *Files 15% similar despite different names*

```diff
@@ -1,14 +1,15 @@
 from django.forms import ModelForm
 from opcalendar.models import (
     Event,
     EventMember,
     EventCategory,
     EventHost,
     EventVisibility,
+    UserSettings,
 )
 from django.forms.widgets import TextInput
 from django import forms
 from allianceauth.services.hooks import get_extension_logger
 
 logger = get_extension_logger(__name__)
 
@@ -79,15 +80,24 @@
         )
     )
 
 
 class AddMemberForm(forms.ModelForm):
     class Meta:
         model = EventMember
-        fields = ["character"]
+        fields = ["character", "status", "comment"]
+        widgets = {
+            "comment": forms.TextInput(
+                attrs={
+                    "class": "form-control",
+                    "maxlength": 100,
+                    "placeholder": "Optional comment",
+                }
+            ),
+        }
 
 
 class AddCategoryForm(forms.ModelForm):
     class Meta:
         model = EventCategory
         fields = "__all__"
 
@@ -104,7 +114,17 @@
 class EventCategoryAdminForm(forms.ModelForm):
     class Meta:
         model = EventCategory
         fields = "__all__"
         widgets = {
             "color": TextInput(attrs={"type": "color"}),
         }
+
+
+class UserSettingsForm(forms.ModelForm):
+    class Meta:
+        model = UserSettings
+        fields = ["disable_discord_notifications", "use_local_times"]
+        labels = {
+            "disable_discord_notifications": "Disable all direct discord notifications",
+            "use_local_times": "Show all events in local time instead of EVE time",
+        }
```

### Comparing `aa-opcalendar-2.4.0/opcalendar/helpers.py` & `aa_opcalendar-3.0.0b1/opcalendar/helpers.py`

 * *Files identical despite different names*

### Comparing `aa-opcalendar-2.4.0/opcalendar/migrations/0001_initial.py` & `aa_opcalendar-3.0.0b1/opcalendar/migrations/0001_initial.py`

 * *Files identical despite different names*

### Comparing `aa-opcalendar-2.4.0/opcalendar/migrations/0002_auto_20201104_1054.py` & `aa_opcalendar-3.0.0b1/opcalendar/migrations/0002_auto_20201104_1054.py`

 * *Files identical despite different names*

### Comparing `aa-opcalendar-2.4.0/opcalendar/migrations/0003_eventhost.py` & `aa_opcalendar-3.0.0b1/opcalendar/migrations/0003_eventhost.py`

 * *Files identical despite different names*

### Comparing `aa-opcalendar-2.4.0/opcalendar/migrations/0004_event_host.py` & `aa_opcalendar-3.0.0b1/opcalendar/migrations/0004_event_host.py`

 * *Files identical despite different names*

### Comparing `aa-opcalendar-2.4.0/opcalendar/migrations/0005_auto_20201104_1127.py` & `aa_opcalendar-3.0.0b1/opcalendar/migrations/0005_auto_20201104_1127.py`

 * *Files identical despite different names*

### Comparing `aa-opcalendar-2.4.0/opcalendar/migrations/0006_auto_20201104_1201.py` & `aa_opcalendar-3.0.0b1/opcalendar/migrations/0006_auto_20201104_1201.py`

 * *Files identical despite different names*

### Comparing `aa-opcalendar-2.4.0/opcalendar/migrations/0009_auto_20201105_0859.py` & `aa_opcalendar-3.0.0b1/opcalendar/migrations/0009_auto_20201105_0859.py`

 * *Files identical despite different names*

### Comparing `aa-opcalendar-2.4.0/opcalendar/migrations/0010_auto_20201105_1602.py` & `aa_opcalendar-3.0.0b1/opcalendar/migrations/0010_auto_20201105_1602.py`

 * *Files identical despite different names*

### Comparing `aa-opcalendar-2.4.0/opcalendar/migrations/0011_eventimport.py` & `aa_opcalendar-3.0.0b1/opcalendar/migrations/0011_eventimport.py`

 * *Files identical despite different names*

### Comparing `aa-opcalendar-2.4.0/opcalendar/migrations/0012_auto_20210112_0934.py` & `aa_opcalendar-3.0.0b1/opcalendar/migrations/0012_auto_20210112_0934.py`

 * *Files identical despite different names*

### Comparing `aa-opcalendar-2.4.0/opcalendar/migrations/0013_eventimport_creator.py` & `aa_opcalendar-3.0.0b1/opcalendar/migrations/0013_eventimport_creator.py`

 * *Files identical despite different names*

### Comparing `aa-opcalendar-2.4.0/opcalendar/migrations/0014_auto_20210113_0836.py` & `aa_opcalendar-3.0.0b1/opcalendar/migrations/0014_auto_20210113_0836.py`

 * *Files identical despite different names*

### Comparing `aa-opcalendar-2.4.0/opcalendar/migrations/0015_eventimport_eve_character.py` & `aa_opcalendar-3.0.0b1/opcalendar/migrations/0015_eventimport_eve_character.py`

 * *Files identical despite different names*

### Comparing `aa-opcalendar-2.4.0/opcalendar/migrations/0016_auto_20210119_1545.py` & `aa_opcalendar-3.0.0b1/opcalendar/migrations/0016_auto_20210119_1545.py`

 * *Files identical despite different names*

### Comparing `aa-opcalendar-2.4.0/opcalendar/migrations/0017_auto_20210119_1626.py` & `aa_opcalendar-3.0.0b1/opcalendar/migrations/0017_auto_20210119_1626.py`

 * *Files identical despite different names*

### Comparing `aa-opcalendar-2.4.0/opcalendar/migrations/0018_auto_20210119_1701.py` & `aa_opcalendar-3.0.0b1/opcalendar/migrations/0018_auto_20210119_1701.py`

 * *Files identical despite different names*

### Comparing `aa-opcalendar-2.4.0/opcalendar/migrations/0019_auto_20210125_1005.py` & `aa_opcalendar-3.0.0b1/opcalendar/migrations/0019_auto_20210125_1005.py`

 * *Files identical despite different names*

### Comparing `aa-opcalendar-2.4.0/opcalendar/migrations/0022_auto_20210222_1255.py` & `aa_opcalendar-3.0.0b1/opcalendar/migrations/0022_auto_20210222_1255.py`

 * *Files identical despite different names*

### Comparing `aa-opcalendar-2.4.0/opcalendar/migrations/0023_auto_20210330_0632.py` & `aa_opcalendar-3.0.0b1/opcalendar/migrations/0023_auto_20210330_0632.py`

 * *Files identical despite different names*

### Comparing `aa-opcalendar-2.4.0/opcalendar/migrations/0024_auto_20210429_1111.py` & `aa_opcalendar-3.0.0b1/opcalendar/migrations/0024_auto_20210429_1111.py`

 * *Files identical despite different names*

### Comparing `aa-opcalendar-2.4.0/opcalendar/migrations/0025_auto_20220115_1101.py` & `aa_opcalendar-3.0.0b1/opcalendar/migrations/0025_auto_20220115_1101.py`

 * *Files identical despite different names*

### Comparing `aa-opcalendar-2.4.0/opcalendar/migrations/0026_alter_event_repeat_event.py` & `aa_opcalendar-3.0.0b1/opcalendar/migrations/0026_alter_event_repeat_event.py`

 * *Files identical despite different names*

### Comparing `aa-opcalendar-2.4.0/opcalendar/models.py` & `aa_opcalendar-3.0.0b1/opcalendar/models.py`

 * *Files 3% similar despite different names*

```diff
@@ -436,21 +436,28 @@
     def get_date_status(self):
         if datetime.now(timezone.utc) > self.start_time:
             return "past-event"
         else:
             return "future-event"
 
     @property
+    def external_tag(self):
+        if self.external:
+            return "external"
+        else:
+            return False
+
+    @property
     def get_html_url(self):
         url = reverse("opcalendar:event-detail", args=(self.id,))
         return f"{url}"
 
     @property
     def get_html_title(self):
-        return f'<span>{self.start_time.strftime("%H:%M")} - {self.end_time.strftime("%H:%M")} <i>{self.host.community}</i></span><span><b>{self.operation_type.ticker} {self.title}</b></span>'
+        return f'<span id="event-time-{self.id}">{self.start_time.strftime("%H:%M")}</span><span><b>{self.operation_type.ticker} {self.title}</b></span><span><i>{self.host.community}</i></span>'
 
     def user_can_edit(self, user: user) -> bool:
         """Checks if the given user can edit this timer. Returns True or False"""
         return user.has_perm("opcalendar.manage_event") or (
             self.user == user and user.has_perm("opcalendar.create_event")
         )
 
@@ -734,21 +741,84 @@
     @property
     def get_html_url(self):
         url = reverse("opcalendar:ingame-event-detail", args=(self.event_id,))
         return f"{url}"
 
     @property
     def get_html_title(self):
-        return f'<span>{self.event_start_date.strftime("%H:%M")} - {self.event_end_date.strftime("%H:%M")}<i> {self.owner_name}</i></span><span><b>{self.title}</b></span>'
+        return f'<span id="event-time-{self.unique_id}">{self.event_start_date.strftime("%H:%M")}</span><span><b>{self.title}</b></span><span><i>{self.owner_name}</i></span>'
+
+    @property
+    def external_tag(self):
+        return False
 
 
 class EventMember(models.Model):
+    class Status(models.TextChoices):
+        ATTENDING = "A", _("Attending")
+        MAYBE = "M", _("Maybe")
+        DECLINED = "D", _("Declined")
+
     event = models.ForeignKey(Event, on_delete=models.CASCADE)
     character = models.ForeignKey(
         EveCharacter,
         null=True,
         on_delete=models.SET_NULL,
         help_text="Event creator main character",
     )
+    status = models.CharField(
+        max_length=1,
+        choices=Status.choices,
+        default=Status.ATTENDING,
+    )
+    comment = models.CharField(
+        max_length=100, blank=True, help_text="Optional comment about the event"
+    )
 
     class Meta:
         unique_together = ["event", "character"]
+
+    def __str__(self):
+        return f"{self.character} - {self.get_status_display()}"
+
+
+def get_sentinel_user():
+    """
+    get user or create one
+    :return:
+    """
+
+    return User.objects.get_or_create(username="deleted")[0]
+
+
+class UserSettings(models.Model):
+    """
+    User settings
+    """
+
+    user = models.ForeignKey(
+        User,
+        related_name="+",
+        null=True,
+        blank=True,
+        default=None,
+        on_delete=models.SET(get_sentinel_user),
+    )
+
+    disable_discord_notifications = models.BooleanField(
+        default=True,
+        verbose_name=_("Discord Notifications"),
+    )
+
+    use_local_times = models.BooleanField(
+        default=True,
+        verbose_name=_("Use Local Times"),
+    )
+
+    class Meta:
+        """
+        Meta definitions
+        """
+
+        default_permissions = ()
+        verbose_name = _("User Settings")
+        verbose_name_plural = _("User Settings")
```

### Comparing `aa-opcalendar-2.4.0/opcalendar/static/opcalendar/calendar.png` & `aa_opcalendar-3.0.0b1/opcalendar/static/opcalendar/calendar.png`

 * *Files identical despite different names*

### Comparing `aa-opcalendar-2.4.0/opcalendar/static/opcalendar/style_dark.css` & `aa_opcalendar-3.0.0b1/opcalendar/static/opcalendar/style_dark.css`

 * *Files identical despite different names*

### Comparing `aa-opcalendar-2.4.0/opcalendar/static/opcalendar/terminate.png` & `aa_opcalendar-3.0.0b1/opcalendar/static/opcalendar/terminate.png`

 * *Files identical despite different names*

### Comparing `aa-opcalendar-2.4.0/opcalendar/swagger.json` & `aa_opcalendar-3.0.0b1/opcalendar/swagger.json`

 * *Files identical despite different names*

### Comparing `aa-opcalendar-2.4.0/opcalendar/tasks.py` & `aa_opcalendar-3.0.0b1/opcalendar/tasks.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,35 +1,35 @@
-from datetime import datetime
 import re
+from datetime import datetime
 
-from bravado.exception import HTTPBadGateway, HTTPGatewayTimeout, HTTPServiceUnavailable
-from celery import shared_task
 import feedparser
-from ics import Calendar
-import requests
 import pytz
-from django.utils.html import strip_tags
+import requests
 from allianceauth.services.hooks import get_extension_logger
 from allianceauth.services.tasks import QueueOnce
+from bravado.exception import HTTPBadGateway, HTTPGatewayTimeout, HTTPServiceUnavailable
+from celery import shared_task
+from django.utils.html import strip_tags
+from ics import Calendar
+from requests.exceptions import RequestException
 
 from .app_settings import (
+    OPCALENDAR_CAS_URL,
+    OPCALENDAR_EVE_LINKNET_URL,
     OPCALENDAR_EVE_UNI_URL,
-    OPCALENDAR_SPECTRE_URL,
-    OPCALENDAR_FUNINC_URL,
+    OPCALENDAR_FREE_RANGE_CHIKUNS_URL,
     OPCALENDAR_FRIDAY_YARRRR_URL,
-    OPCALENDAR_REDEMPTION_ROAD_URL,
-    OPCALENDAR_CAS_URL,
+    OPCALENDAR_FUNINC_URL,
     OPCALENDAR_FWAMING_DWAGONS_URL,
-    OPCALENDAR_FREE_RANGE_CHIKUNS_URL,
-    OPCALENDAR_EVE_LINKNET_URL,
+    OPCALENDAR_REDEMPTION_ROAD_URL,
+    OPCALENDAR_SPECTRE_URL,
+    OPCALENDAR_TASKS_TIME_LIMIT,
 )
-from .app_settings import OPCALENDAR_TASKS_TIME_LIMIT
 from .models import Event, EventImport, Owner
 
-
 DEFAULT_TASK_PRIORITY = 6
 
 logger = get_extension_logger(__name__)
 
 # Create your tasks here
 TASK_DEFAULT_KWARGS = {
     "time_limit": OPCALENDAR_TASKS_TIME_LIMIT,
@@ -182,15 +182,15 @@
 
                         logger.debug(
                             "%s: Saved new event in database: %s",
                             feed,
                             entry.title,
                         )
 
-    except Exception:
+    except (NotImplementedError, RequestException):
         logger.error("%s: Error in fetching fleets", feed, exc_info=True)
         return True
 
     return False
 
 
 def _import_fun_inc(feed, event_ids_to_remove):
@@ -199,26 +199,28 @@
         feed,
         OPCALENDAR_FUNINC_URL,
     )
 
     try:
         # Get FUN Inc fleets from google ical
         r = requests.get(OPCALENDAR_FUNINC_URL)
+        r.raise_for_status()
+
         c = Calendar(r.text)
 
         # Parse each entry we got
         for entry in c.events:
             # Format datetime
             start_date = datetime.utcfromtimestamp(entry.begin.float_timestamp).replace(
                 tzinfo=pytz.utc
             )
             end_date = datetime.utcfromtimestamp(entry.end.float_timestamp).replace(
                 tzinfo=pytz.utc
             )
-            title = entry.name
+            title = entry.name if entry.name else ""
 
             logger.debug("%s: Import even found: %s", feed, title)
 
             # Check if we already have the event stored
             original = Event.objects.filter(start_time=start_date, title=title).first()
 
             # If we get the event from API it should not be removed
@@ -246,15 +248,15 @@
                     eve_character=feed.eve_character,
                 )
 
                 logger.debug("%s: Saved new EVE UNI event in database: %s", feed, title)
 
                 event.save()
 
-    except Exception:
+    except (NotImplementedError, RequestException):
         logger.error("%s: Error in fetching fleets", feed, exc_info=True)
         return True
 
     return False
 
 
 def _import_eve_uni(feed, event_ids_to_remove):
@@ -263,18 +265,20 @@
         feed,
         OPCALENDAR_EVE_UNI_URL,
     )
 
     try:
         # Get EVE Uni events from their API feed (ical)
         r = requests.get(OPCALENDAR_EVE_UNI_URL)
+        r.raise_for_status()
+
         c = Calendar(r.text)
         for entry in c.events:
             # Filter only class events as they are the only public events in eveuni
-            if "class" in entry.name.lower():
+            if entry.name and "class" in entry.name.lower():
                 # Format datetime
                 start_date = datetime.utcfromtimestamp(
                     entry.begin.float_timestamp
                 ).replace(tzinfo=pytz.utc)
                 end_date = datetime.utcfromtimestamp(entry.end.float_timestamp).replace(
                     tzinfo=pytz.utc
                 )
@@ -317,15 +321,15 @@
                     logger.debug(
                         "%s: Saved new EVE UNI event in database: %s",
                         feed,
                         title,
                     )
                     event.save()
 
-    except Exception:
+    except (NotImplementedError, RequestException):
         logger.error("%s: Error in fetching fleets", feed, exc_info=True)
         return True
 
     return False
 
 
 def _import_ical(feed, event_ids_to_remove, url):
@@ -334,24 +338,26 @@
         feed,
         url,
     )
 
     try:
         # Get EVE Uni events from their API feed (ical)
         r = requests.get(url)
+        r.raise_for_status()
+
         c = Calendar(r.text)
         for entry in c.events:
             # Format datetime
             start_date = datetime.utcfromtimestamp(entry.begin.float_timestamp).replace(
                 tzinfo=pytz.utc
             )
             end_date = datetime.utcfromtimestamp(entry.end.float_timestamp).replace(
                 tzinfo=pytz.utc
             )
-            title = re.sub(r"[\(\[].*?[\)\]]", "", entry.name)
+            title = re.sub(r"[\(\[].*?[\)\]]", "", entry.name) if entry.name else ""
 
             logger.debug("%s: Import even found: %s", feed, title)
 
             # Check if we already have the event stored
             original = Event.objects.filter(start_time=start_date, title=title).first()
 
             # If we get the event from API it should not be removed
@@ -380,15 +386,15 @@
                 logger.debug(
                     "%s: Saved new EVE UNI event in database: %s",
                     feed,
                     title,
                 )
                 event.save()
 
-    except Exception:
+    except (NotImplementedError, RequestException):
         logger.error("%s: Error in fetching fleets", feed, exc_info=True)
         return True
 
     return False
 
 
 @shared_task(
```

### Comparing `aa-opcalendar-2.4.0/opcalendar/templates/opcalendar/base.html` & `aa_opcalendar-3.0.0b1/opcalendar/templates/opcalendar/base.html`

 * *Files 10% similar despite different names*

```diff
@@ -1,20 +1,29 @@
-{% extends 'allianceauth/base.html' %}
+{% extends 'allianceauth/base-bs5.html' %}
 {% load i18n %}
 {% load static %}
+v
 
 {% block extra_css %}
     {% include 'bundles/jquery-datetimepicker-css.html' %}
-    {% if NIGHT_MODE %}
-    <link rel="stylesheet" type="text/css" href="{% static 'opcalendar/style_dark.css' %}">
-    {% else %}
-    <link rel="stylesheet" type="text/css" href="{% static 'opcalendar/style_light.css' %}">
-    {% endif %}
+    {% include "opcalendar/partials/base/stylesheets.html" %}
 {% endblock extra_css %}
-{% block page_title %}{% trans title %}{% endblock %}
+
+{% block page_title %}
+    {% translate "Operation Calendar" %}
+{% endblock page_title %}
+
+{% block header_nav_collapse_right %}
+    {% include "opcalendar/partials/base/menu.html" %}
+{% endblock %}
+
+{% block header_nav_brand %}
+    {% translate "Operation Calendar" %}
+{% endblock %}
+
 
 {% block content %}
     <h2 class="text-center">{{ title }}</h2>
     <div class="col-lg-14 container">
         {% block details %}{% endblock %}
     </div>
 {% endblock %}
```

### Comparing `aa-opcalendar-2.4.0/opcalendar/templates/opcalendar/event-add.html` & `aa_opcalendar-3.0.0b1/opcalendar/templates/opcalendar/event-add.html`

 * *Files 17% similar despite different names*

```diff
@@ -6,32 +6,25 @@
 
 {% block page_title %}{% trans "Create Operation" %}{% endblock page_title %}
 {% block extra_css %}
     {% include 'bundles/jquery-datetimepicker-css.html' %}
 {% endblock extra_css %}
 
 {% block content %}
-    <div class="col-lg-12">
-        <h1 class="page-header text-center">{% trans "Create New Event" %}</h1>
-
-        <div class="container-fluid">
-            <div class="col-md-4 col-md-offset-4">
-                <div class="row">
-                    <div class="allianceauth-opcalendar">
-                        <form class="form-signin" role="form" action="" method="POST">
-                            {% csrf_token %}
-                            {{ form|bootstrap }}
-                            <br/>
-                            <button class="btn btn-lg btn-primary btn-block" type="submit">{% trans "Create New Event" %}</button>
-                        </form>
-                    </div>
-                </div>
-            </div>
-        </div>
+<div class="card">
+    <div class="card-header">{% trans "Create New Event" %}</div>
+    <div class="card-body">
+        <form class="form-signin" role="form" action="" method="POST">
+            {% csrf_token %}
+            {{ form|bootstrap }}
+            <br/>
+            <button class="btn btn-lg btn-primary btn-block" type="submit">{% trans "Create New Event" %}</button>
+        </form>
     </div>
+</div>
 
 {% endblock content %}
 
 {% block extra_javascript %}
   <script>
     $("#id_operation_type").change(function () {
       var id = $(this).val();
```

### Comparing `aa-opcalendar-2.4.0/opcalendar/templates/opcalendar/event-edit.html` & `aa_opcalendar-3.0.0b1/opcalendar/templates/opcalendar/user_settings.html`

 * *Files 22% similar despite different names*

```diff
@@ -1,35 +1,30 @@
 {% extends 'opcalendar/base.html' %}
-{% load bootstrap %}
-{% load static %}
 {% load i18n %}
-{% get_current_language as LANGUAGE_CODE %}
 
-{% block page_title %}{% trans "Create Operation" %}{% endblock page_title %}
-{% block extra_css %}
-    {% include 'bundles/jquery-datetimepicker-css.html' %}
-{% endblock extra_css %}
+{% block page_title %}{% trans "User Settings" %}{% endblock page_title %}
 
 {% block content %}
-    <div class="col-lg-12">
-        <h1 class="page-header text-center">{% trans "Edit Event" %}</h1>
-        <div class="container-fluid">
-            <div class="col-md-4 col-md-offset-4">
-                <div class="row">
-                    <div class="allianceauth-opcalendar">
-                        <form class="form-signin" role="form" action="" method="POST">
-                            {% csrf_token %}
-                            {{ form|bootstrap }}
-                            <br/>
-                            <button class="btn btn-lg btn-primary btn-block" type="submit">{% trans "Edit Event" %}</button>
-                        </form>
-                    </div>
+<div class="container mt-4">
+    <div class="card">
+        <div class="card-header">
+            <h4 class="card-title">{% trans "User Settings" %}</h4>
+        </div>
+        <div class="card-body">
+            {% if messages %}
+                <div class="mb-3">
+                    {% for message in messages %}
+                        <div class="alert {% if message.tags %}alert-{{ message.tags }}{% else %}alert-info{% endif %}" role="alert">
+                            {{ message }}
+                        </div>
+                    {% endfor %}
                 </div>
-            </div>
+            {% endif %}
+            <form method="post">
+                {% csrf_token %}
+                {{ form.as_p }}
+                <button type="submit" class="btn btn-primary">{% trans "Save Settings" %}</button>
+            </form>
         </div>
     </div>
-
+</div>
 {% endblock content %}
-
-{% block extra_javascript %}
-    {% include 'bundles/jquery-datetimepicker-js.html' %}
-{% endblock %}
```

### Comparing `aa-opcalendar-2.4.0/opcalendar/templates/opcalendar/ingame-event-details.html` & `aa_opcalendar-3.0.0b1/opcalendar/templates/opcalendar/ingame-event-details.html`

 * *Files 12% similar despite different names*

```diff
@@ -48,82 +48,84 @@
                         <td>{{ event.duration }} minutes</td>
                     </tr>
                 </table>
                 <p style="padding-top:40px">{{ event.text|striptags|urlize}}</p>
             </div>
         </div>
     </div>
-{% include 'bundles/moment-js.html' with locale=True %}
-    <script src="{% static 'js/timers.js' %}"></script>
-    <script type="application/javascript">
-        // Data
-        var timers = [
-            {
-                'id': {{ event.event_id }},
-                'start': moment("{{ event.event_start_date | date:"c" }}"),
-                'expired': false
-            },
+{% endblock %}
+
+{% block extra_javascript %}
+    {% include "bundles/moment-js.html" with locale=True %}
+    {% include "bundles/timers-js.html" %}
+
+    <script>
+        const timers = [
+                {
+                    'id': {{ event.event_id }},
+                    'targetDate': moment("{{ event.event_start_date | date:"c" }}"),
+                    'expired': false
+                },
         ];
-    </script>
-    <script type="application/javascript">
 
-        timedUpdate();
-        setAllLocalTimes();
+        /**
+         * Update a timer
+         * @param timer Timer information
+         */
+        const updateTimer = (timer) => {
+            if (timer.targetDate.isAfter(Date.now())) {
+                const duration = moment.duration(event.event_start_date - moment(), 'milliseconds');
 
-        // Start timed updates
-        setInterval(timedUpdate, 1000);
+                document.getElementById("localtime" + timer.id).innerHTML = getDurationString(duration);
+            } else {
+                timer.expired = true;
 
-        function timedUpdate() {
-            updateClock();
-            updateAllTimers();
-        }
+                document.getElementById("localtime" + timer.id).innerHTML = "";
+            }
+        };
 
-        function updateAllTimers () {
-            var l = timers.length;
-            for (var i=0; i < l; ++i) {
+        const updateAllTimers = () => {
+            const l = timers.length;
+
+            for (let i=0; i < l; ++i) {
                 if (timers[i].expired) continue;
+
                 updateTimer(timers[i]);
             }
-        }
+        };
 
         /**
-         * Update a timer
+         * Set the local time info for the timer
          * @param timer Timer information
-         * @param timer.start Date of the timer
-         * @param timer.id Id number of the timer
-         * @param timer.expired
          */
-        function updateTimer(timer) {
-            if (timer.start.isAfter(Date.now())) {
-                var duration = moment.duration(timer.start - moment(), 'milliseconds');
-                document.getElementById("countdown" + timer.id).innerHTML = getDurationString(duration);
-            } else {
-                timer.expired = true;
-                document.getElementById("countdown" + timer.id).innerHTML = "";
-            }
-        }
+        const setLocalTime = (timer) => {
+            document.getElementById("localtime" + timer.id).innerHTML = timer.targetDate.format("ddd @ LT");
+        };
 
         /**
          * Set all local time fields
          */
-        function setAllLocalTimes() {
-            var l = timers.length;
-            for (var i=0; i < l; ++i) {
+        const setAllLocalTimes = () => {
+            const l = timers.length;
+
+            for (let i=0; i < l; ++i) {
                 setLocalTime(timers[i]);
             }
-        }
-
-        /**
-         * Set the local time info for the timer
-         * @param timer Timer information
-         * @param timer.start Date of the timer
-         * @param timer.id Id number of the timer
-         */
-        function setLocalTime(timer) {
-            document.getElementById("localtime" + timer.id).innerHTML = timer.start.format("ddd MM-DD HH:mm");
-        }
+        };
 
-        function updateClock() {
+        const updateClock = () => {
             document.getElementById("current-time").innerHTML = getCurrentEveTimeString();
+        };
+
+        const timedUpdate = () => {
+            updateClock();
+            updateAllTimers();
         }
+
+        // Set initial values
+        setAllLocalTimes();
+        timedUpdate();
+
+        // Start timed updates
+        setInterval(timedUpdate, 1000);
     </script>
-{% endblock %}
+{% endblock extra_javascript %}
```

#### html2text {}

```diff
@@ -10,9 +10,10 @@
 ****** EEvveenntt ddeettaaiillss ******
 TTyyppee::          Ingame calendar feed
 AAvvaaiillaabbiilliittyy::  {{ event.owner_name }}
 SSttaarrtt ttiimmee::    {{ event.event_start_date|date:"D Y-m-d H:i" }} (EVE) / (Local)
 EEsstt.. eenndd ttiimmee:: {{ event.event_end_date|date:"D Y-m-d H:i" }}
 DDuurraattiioonn::      {{ event.duration }} minutes
 {{ event.text|striptags|urlize}}
-{% include 'bundles/moment-js.html' with locale=True %}
-{% endblock %}
+{% endblock %} {% block extra_javascript %} {% include "bundles/moment-js.html"
+with locale=True %} {% include "bundles/timers-js.html" %}
+{% endblock extra_javascript %}
```

### Comparing `aa-opcalendar-2.4.0/opcalendar/tests/test_models.py` & `aa_opcalendar-3.0.0b1/opcalendar/tests/test_models.py`

 * *Files identical despite different names*

### Comparing `aa-opcalendar-2.4.0/opcalendar/tests/test_tasks.py` & `aa_opcalendar-3.0.0b1/opcalendar/tests/test_tasks.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,14 +1,15 @@
 import datetime as dt
 from unittest.mock import patch
 
 import requests
 import requests_mock
 from allianceauth.tests.auth_utils import AuthUtils
 from pytz import utc
+from requests.exceptions import HTTPError
 
 from .. import tasks
 from ..models import Event, EventCategory, EventHost, EventImport
 from ..utils import NoSocketsTestCase
 from .testdata import COLOR_PURPLE, feedparser_parse, generate_ical_string
 
 MODULE_PATH = "opcalendar.tasks"
@@ -141,15 +142,15 @@
         # then
         self.assertEqual(Event.objects.count(), 0)
 
     def test_should_report_when_spectre_fleet_has_error(
         self, mock_feedparser, requests_mocker
     ):
         # given
-        mock_feedparser.parse.side_effect = RuntimeError
+        mock_feedparser.parse.side_effect = HTTPError
         EventImport.objects.create(
             source=EventImport.SPECTRE_FLEET,
             host=self.host,
             operation_type=self.category,
             creator=self.user,
             eve_character=self.eve_character,
         )
@@ -175,18 +176,17 @@
             operation_type=self.category,
             creator=self.user,
             eve_character=self.eve_character,
         )
         # when
         tasks.import_all_npsi_fleets()
         # then
-        self.assertEqual(Event.objects.count(), 1)
-        obj = Event.objects.first()
+        self.assertEqual(Event.objects.count(), 2)
+        obj = Event.objects.get(title="Fun Fleet 1")
         self.assertEqual(obj.operation_type, self.category)
-        self.assertEqual(obj.title, "Fun Fleet 1")
         self.assertEqual(obj.host, self.host)
         self.assertEqual(obj.doctrine, "see details")
         self.assertEqual(obj.formup_system, EventImport.FUN_INC)
         self.assertEqual(obj.description, "Testing Fun Fleet 1")
         self.assertEqual(obj.start_time, utc.localize(dt.datetime(2021, 2, 5, 22, 0)))
         self.assertEqual(obj.end_time, utc.localize(dt.datetime(2021, 2, 5, 23, 0)))
         self.assertEqual(obj.fc, EventImport.FUN_INC)
@@ -242,15 +242,15 @@
             external=True,
             user=self.user,
             eve_character=self.eve_character,
         )
         # when
         tasks.import_all_npsi_fleets()
         # then
-        self.assertEqual(Event.objects.count(), 1)
+        self.assertEqual(Event.objects.count(), 2)
         self.assertTrue(Event.objects.filter(pk=original_event.pk).exists())
 
     def test_should_delete_outdated_fun_inc_event(
         self, mock_feedparser, requests_mocker
     ):
         # given
         requests_mocker.register_uri(
@@ -531,11 +531,11 @@
             operation_type=self.category,
             creator=self.user,
             eve_character=self.eve_character,
         )
         # when
         tasks.import_all_npsi_fleets()
         # then
-        self.assertEqual(Event.objects.count(), 3)
+        self.assertEqual(Event.objects.count(), 4)
         self.assertTrue(Event.objects.filter(title="Spectre Fleet 1").exists())
         self.assertTrue(Event.objects.filter(title="Fun Fleet 1").exists())
         self.assertTrue(Event.objects.filter(title="Eve Uni class 1").exists())
```

### Comparing `aa-opcalendar-2.4.0/opcalendar/tests/testdata.py` & `aa_opcalendar-3.0.0b1/opcalendar/tests/testdata.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,14 +1,15 @@
 import json
 from pathlib import Path
 
 from bravado.exception import HTTPNotFound
-from django.utils.dateparse import parse_datetime
 from ics import Calendar, Event
 
+from django.utils.dateparse import parse_datetime
+
 from ..utils import BravadoOperationStub, BravadoResponseStub
 
 COLOR_PURPLE = "#8e44ad"
 
 
 def _load_testdata() -> dict:
     testdata_path = Path(__file__).parent / "testdata.json"
@@ -21,15 +22,15 @@
 
 def generate_ical_string(key: str) -> str:
     """generates iCalendar string from testdata and returns it"""
     c = Calendar()
     for row in _testdata["iCalendar"].get(key, []):
         c.events.add(
             Event(
-                name=row["name"],
+                name=row.get("name"),
                 begin=row["begin"],
                 end=row["end"],
                 description=row["description"],
             )
         )
     return c.serialize()
```

### Comparing `aa-opcalendar-2.4.0/opcalendar/urls.py` & `aa_opcalendar-3.0.0b1/opcalendar/urls.py`

 * *Files 23% similar despite different names*

```diff
@@ -29,8 +29,29 @@
     path("feed.ics", views.EventFeed()),
     path(
         "event/<int:event_id>/details/feed.ics",
         views.EventIcalView(),
         name="event-ical-view",
     ),
     path("event/new/ajax/get_category/", views.get_category, name="get_category"),
+    path(
+        "event/<int:event_id>/signup/attending/",
+        views.event_member_signup_attending,
+        name="event_member_signup_attending",
+    ),
+    path(
+        "event/<int:event_id>/signup/maybe/",
+        views.event_member_signup_maybe,
+        name="event_member_signup_maybe",
+    ),
+    path(
+        "event/<int:event_id>/signup/declined/",
+        views.event_member_signup_declined,
+        name="event_member_signup_declined",
+    ),
+    path(
+        "event/<int:event_id>/remove/",
+        views.event_member_remove,
+        name="event_member_remove",
+    ),
+    path("user/settings/", views.user_settings_view, name="user_settings"),
 ]
```

### Comparing `aa-opcalendar-2.4.0/opcalendar/utils.py` & `aa_opcalendar-3.0.0b1/opcalendar/utils.py`

 * *Files identical despite different names*

### Comparing `aa-opcalendar-2.4.0/opcalendar/views.py` & `aa_opcalendar-3.0.0b1/opcalendar/views.py`

 * *Files 5% similar despite different names*

```diff
@@ -26,20 +26,26 @@
 from opcalendar.models import (
     Event,
     EventCategory,
     EventMember,
     EventVisibility,
     IngameEvents,
     Owner,
+    UserSettings,
 )
 
 from . import tasks
-from .app_settings import get_site_url, moonmining_active, structuretimers_active
+from .app_settings import (
+    get_site_url,
+    moonmining_active,
+    structuretimers_active,
+    OPCALENDAR_DISPLAY_MOONMINING_ARRIVAL_TIME,
+)
 from .calendar import Calendar
-from .forms import EventEditForm, EventForm
+from .forms import EventEditForm, EventForm, UserSettingsForm
 from .utils import messages_plus
 
 logger = get_extension_logger(__name__)
 
 
 @login_required(login_url="signup")
 def index(request):
@@ -126,34 +132,80 @@
     days_in_month = calendar.monthrange(d.year, d.month)[1]
     last = d.replace(day=days_in_month)
     next_month = last + timedelta(days=1)
     month = "month=" + str(next_month.year) + "-" + str(next_month.month)
     return month
 
 
+def event_member_signup_attending(request, event_id):
+    return handle_event_member_signup(request, event_id, EventMember.Status.ATTENDING)
+
+
+def event_member_signup_maybe(request, event_id):
+    return handle_event_member_signup(request, event_id, EventMember.Status.MAYBE)
+
+
+def event_member_signup_declined(request, event_id):
+    return handle_event_member_signup(request, event_id, EventMember.Status.DECLINED)
+
+
+def handle_event_member_signup(request, event_id, status):
+    event = get_object_or_404(Event, id=event_id)
+    character = request.user.profile.main_character
+
+    if request.method == "POST":
+        comment = request.POST.get("comment", "")
+        EventMember.objects.update_or_create(
+            event=event,
+            character=character,
+            defaults={"status": status, "comment": comment},
+        )
+        return redirect("opcalendar:event-detail", event_id=event.id)
+
+    return redirect("opcalendar:event-detail", event_id=event.id)
+
+
+def event_member_remove(request, event_id):
+    event = get_object_or_404(Event, id=event_id)
+    character = request.user.profile.main_character
+    EventMember.objects.filter(event=event, character=character).delete()
+    return redirect("opcalendar:event-detail", event_id=event.id)
+
+
 class CalendarView(LoginRequiredMixin, PermissionRequiredMixin, ListView):
     permission_required = "opcalendar.basic_access"
     login_url = "signup"
     model = Event
     template_name = "opcalendar/calendar.html"
 
     def get_context_data(self, **kwargs):
         user = self.request.user
-        # user_permissions = self.request.user.has_perm('app.get_main_view')
         context = super().get_context_data(**kwargs)
         d = get_date(self.request.GET.get("month", None))
         cal = Calendar(d.year, d.month, user)
-        html_cal = cal.formatmonth(withyear=True)
+
+        user_settings, created = UserSettings.objects.get_or_create(
+            user=user,
+            defaults={"discord_notifications": False, "use_local_times": False},
+        )
+
+        html_cal, all_events_per_month = cal.formatmonth(withyear=True)
         context["moonmining_active"] = moonmining_active()
         context["structuretimers_active"] = structuretimers_active()
         context["category"] = EventCategory.objects.all()
         context["visibility"] = EventVisibility.objects.all()
         context["calendar"] = mark_safe(html_cal)
         context["prev_month"] = prev_month(d)
         context["next_month"] = next_month(d)
+        context["all_events_per_month"] = all_events_per_month
+        context["user_settings"] = user_settings
+        context[
+            "OPCALENDAR_DISPLAY_MOONMINING_ARRIVAL_TIME"
+        ] = OPCALENDAR_DISPLAY_MOONMINING_ARRIVAL_TIME
+
         return context
 
 
 @login_required
 @permission_required("opcalendar.create_event")
 def create_event(request):
     form = EventForm(request.POST or None)
@@ -493,7 +545,30 @@
         return item.end_time
 
     def item_organizer(self, item):
         return item.host
 
     def item_link(self, item):
         return "{0}/opcalendar/event/{1}/details/".format(get_site_url(), item.id)
+
+
+@login_required
+def user_settings_view(request):
+    try:
+        user_settings = UserSettings.objects.get(user=request.user)
+    except UserSettings.DoesNotExist:
+        user_settings = UserSettings(user=request.user)
+
+    if request.method == "POST":
+        form = UserSettingsForm(request.POST, instance=user_settings)
+        if form.is_valid():
+            form.save()
+            messages.success(request, "Your settings have been updated successfully.")
+            return redirect("opcalendar:calendar")  # Redirect to the calendar page
+        else:
+            messages.error(
+                request, "There was an error updating your settings. Please try again."
+            )
+    else:
+        form = UserSettingsForm(instance=user_settings)
+
+    return render(request, "opcalendar/user_settings.html", {"form": form})
```

### Comparing `aa-opcalendar-2.4.0/setup.py` & `aa_opcalendar-3.0.0b1/setup.py`

 * *Files identical despite different names*

### Comparing `aa-opcalendar-2.4.0/testauth/celery.py` & `aa_opcalendar-3.0.0b1/testauth/celery.py`

 * *Files identical despite different names*

### Comparing `aa-opcalendar-2.4.0/testauth/settings.py` & `aa_opcalendar-3.0.0b1/testauth/settings.py`

 * *Files identical despite different names*

