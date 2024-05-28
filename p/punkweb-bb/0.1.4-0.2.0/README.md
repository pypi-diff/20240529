# Comparing `tmp/punkweb_bb-0.1.4.tar.gz` & `tmp/punkweb_bb-0.2.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "punkweb_bb-0.1.4.tar", last modified: Thu May  9 06:04:30 2024, max compression
+gzip compressed data, was "punkweb_bb-0.2.0.tar", last modified: Tue May 28 23:00:59 2024, max compression
```

## Comparing `punkweb_bb-0.1.4.tar` & `punkweb_bb-0.2.0.tar`

### file list

```diff
@@ -1,263 +1,280 @@
-drwxr-xr-x   0 pork      (1000) pork      (1000)        0 2024-05-09 06:04:30.064355 punkweb_bb-0.1.4/
--rw-r--r--   0 pork      (1000) pork      (1000)     1507 2024-04-09 06:08:41.000000 punkweb_bb-0.1.4/LICENSE
--rw-r--r--   0 pork      (1000) pork      (1000)       64 2024-04-09 05:47:19.000000 punkweb_bb-0.1.4/MANIFEST.in
--rw-r--r--   0 pork      (1000) pork      (1000)     4992 2024-05-09 06:04:30.064355 punkweb_bb-0.1.4/PKG-INFO
--rw-r--r--   0 pork      (1000) pork      (1000)     4338 2024-05-09 05:30:29.000000 punkweb_bb-0.1.4/README.md
-drwxr-xr-x   0 pork      (1000) pork      (1000)        0 2024-05-09 06:04:30.048355 punkweb_bb-0.1.4/punkweb_bb/
--rw-r--r--   0 pork      (1000) pork      (1000)        0 2023-08-20 16:04:51.000000 punkweb_bb-0.1.4/punkweb_bb/__init__.py
-drwxr-xr-x   0 pork      (1000) pork      (1000)        0 2024-05-09 06:04:30.048355 punkweb_bb-0.1.4/punkweb_bb/__pycache__/
--rw-r--r--   0 pork      (1000) pork      (1000)      161 2024-04-09 05:48:25.000000 punkweb_bb-0.1.4/punkweb_bb/__pycache__/__init__.cpython-311.pyc
--rw-r--r--   0 pork      (1000) pork      (1000)     3679 2024-04-09 05:48:25.000000 punkweb_bb-0.1.4/punkweb_bb/__pycache__/admin.cpython-311.pyc
--rw-r--r--   0 pork      (1000) pork      (1000)     2980 2024-04-09 05:48:25.000000 punkweb_bb-0.1.4/punkweb_bb/__pycache__/admin_forms.cpython-311.pyc
--rw-r--r--   0 pork      (1000) pork      (1000)      730 2024-04-09 06:55:15.000000 punkweb_bb-0.1.4/punkweb_bb/__pycache__/apps.cpython-311.pyc
--rw-r--r--   0 pork      (1000) pork      (1000)     8534 2024-04-09 06:32:38.000000 punkweb_bb-0.1.4/punkweb_bb/__pycache__/bbcode_tags.cpython-311.pyc
--rw-r--r--   0 pork      (1000) pork      (1000)      392 2024-04-09 06:44:27.000000 punkweb_bb-0.1.4/punkweb_bb/__pycache__/context_processors.cpython-311.pyc
--rw-r--r--   0 pork      (1000) pork      (1000)     4680 2024-04-09 05:48:25.000000 punkweb_bb-0.1.4/punkweb_bb/__pycache__/forms.cpython-311.pyc
--rw-r--r--   0 pork      (1000) pork      (1000)     1581 2024-05-09 05:36:59.000000 punkweb_bb-0.1.4/punkweb_bb/__pycache__/guests.cpython-311.pyc
--rw-r--r--   0 pork      (1000) pork      (1000)     1560 2024-05-09 05:37:45.000000 punkweb_bb-0.1.4/punkweb_bb/__pycache__/middleware.cpython-311.pyc
--rw-r--r--   0 pork      (1000) pork      (1000)     1478 2024-04-09 05:48:25.000000 punkweb_bb-0.1.4/punkweb_bb/__pycache__/mixins.cpython-311.pyc
--rw-r--r--   0 pork      (1000) pork      (1000)    12308 2024-05-07 05:16:02.000000 punkweb_bb-0.1.4/punkweb_bb/__pycache__/models.cpython-311.pyc
--rw-r--r--   0 pork      (1000) pork      (1000)      990 2024-04-09 05:48:25.000000 punkweb_bb-0.1.4/punkweb_bb/__pycache__/pagination.cpython-311.pyc
--rw-r--r--   0 pork      (1000) pork      (1000)     5335 2024-04-09 07:07:59.000000 punkweb_bb-0.1.4/punkweb_bb/__pycache__/parsers.cpython-311.pyc
--rw-r--r--   0 pork      (1000) pork      (1000)      448 2024-04-09 05:48:25.000000 punkweb_bb-0.1.4/punkweb_bb/__pycache__/response.cpython-311.pyc
--rw-r--r--   0 pork      (1000) pork      (1000)      947 2024-05-09 05:27:51.000000 punkweb_bb-0.1.4/punkweb_bb/__pycache__/settings.cpython-311.pyc
--rw-r--r--   0 pork      (1000) pork      (1000)      864 2024-04-09 05:48:25.000000 punkweb_bb-0.1.4/punkweb_bb/__pycache__/signals.cpython-311.pyc
--rw-r--r--   0 pork      (1000) pork      (1000)    51829 2024-05-09 05:55:07.000000 punkweb_bb-0.1.4/punkweb_bb/__pycache__/tests.cpython-311.pyc
--rw-r--r--   0 pork      (1000) pork      (1000)     2304 2024-04-09 05:48:25.000000 punkweb_bb-0.1.4/punkweb_bb/__pycache__/urls.cpython-311.pyc
--rw-r--r--   0 pork      (1000) pork      (1000)    16108 2024-05-09 05:54:18.000000 punkweb_bb-0.1.4/punkweb_bb/__pycache__/views.cpython-311.pyc
--rw-r--r--   0 pork      (1000) pork      (1000)     1552 2024-04-09 05:48:25.000000 punkweb_bb-0.1.4/punkweb_bb/__pycache__/widgets.cpython-311.pyc
--rw-r--r--   0 pork      (1000) pork      (1000)     2493 2024-04-05 21:20:18.000000 punkweb_bb-0.1.4/punkweb_bb/admin.py
--rw-r--r--   0 pork      (1000) pork      (1000)     1128 2024-04-03 19:18:44.000000 punkweb_bb-0.1.4/punkweb_bb/admin_forms.py
--rw-r--r--   0 pork      (1000) pork      (1000)      207 2024-04-09 06:52:38.000000 punkweb_bb-0.1.4/punkweb_bb/apps.py
--rw-r--r--   0 pork      (1000) pork      (1000)     4419 2024-04-09 06:31:31.000000 punkweb_bb-0.1.4/punkweb_bb/bbcode_tags.py
--rw-r--r--   0 pork      (1000) pork      (1000)      146 2024-04-09 04:54:41.000000 punkweb_bb-0.1.4/punkweb_bb/context_processors.py
--rw-r--r--   0 pork      (1000) pork      (1000)     1977 2024-04-03 19:20:08.000000 punkweb_bb-0.1.4/punkweb_bb/forms.py
--rw-r--r--   0 pork      (1000) pork      (1000)      467 2024-05-09 05:36:58.000000 punkweb_bb-0.1.4/punkweb_bb/guests.py
--rw-r--r--   0 pork      (1000) pork      (1000)      628 2024-05-09 05:37:44.000000 punkweb_bb-0.1.4/punkweb_bb/middleware.py
-drwxr-xr-x   0 pork      (1000) pork      (1000)        0 2024-05-09 06:04:30.048355 punkweb_bb-0.1.4/punkweb_bb/migrations/
--rw-r--r--   0 pork      (1000) pork      (1000)     8950 2024-04-09 07:09:02.000000 punkweb_bb-0.1.4/punkweb_bb/migrations/0001_initial.py
--rw-r--r--   0 pork      (1000) pork      (1000)      388 2024-05-07 04:24:13.000000 punkweb_bb-0.1.4/punkweb_bb/migrations/0002_thread_view_count.py
--rw-r--r--   0 pork      (1000) pork      (1000)        0 2023-08-20 16:04:51.000000 punkweb_bb-0.1.4/punkweb_bb/migrations/__init__.py
-drwxr-xr-x   0 pork      (1000) pork      (1000)        0 2024-05-09 06:04:30.052355 punkweb_bb-0.1.4/punkweb_bb/migrations/__pycache__/
--rw-r--r--   0 pork      (1000) pork      (1000)     6456 2024-04-09 07:09:10.000000 punkweb_bb-0.1.4/punkweb_bb/migrations/__pycache__/0001_initial.cpython-311.pyc
--rw-r--r--   0 pork      (1000) pork      (1000)      815 2024-05-07 04:24:16.000000 punkweb_bb-0.1.4/punkweb_bb/migrations/__pycache__/0002_thread_view_count.cpython-311.pyc
--rw-r--r--   0 pork      (1000) pork      (1000)      172 2024-04-09 05:48:25.000000 punkweb_bb-0.1.4/punkweb_bb/migrations/__pycache__/__init__.cpython-311.pyc
--rw-r--r--   0 pork      (1000) pork      (1000)      395 2024-04-03 19:16:01.000000 punkweb_bb-0.1.4/punkweb_bb/mixins.py
--rw-r--r--   0 pork      (1000) pork      (1000)     5519 2024-05-07 05:16:01.000000 punkweb_bb-0.1.4/punkweb_bb/models.py
--rw-r--r--   0 pork      (1000) pork      (1000)      409 2024-04-06 08:06:22.000000 punkweb_bb-0.1.4/punkweb_bb/pagination.py
--rw-r--r--   0 pork      (1000) pork      (1000)     2732 2024-04-09 07:07:58.000000 punkweb_bb-0.1.4/punkweb_bb/parsers.py
--rw-r--r--   0 pork      (1000) pork      (1000)      130 2024-04-03 19:15:29.000000 punkweb_bb-0.1.4/punkweb_bb/response.py
--rw-r--r--   0 pork      (1000) pork      (1000)      517 2024-05-09 05:27:49.000000 punkweb_bb-0.1.4/punkweb_bb/settings.py
--rw-r--r--   0 pork      (1000) pork      (1000)      365 2024-04-03 19:18:44.000000 punkweb_bb-0.1.4/punkweb_bb/signals.py
-drwxr-xr-x   0 pork      (1000) pork      (1000)        0 2024-05-09 06:04:30.048355 punkweb_bb-0.1.4/punkweb_bb/static/
-drwxr-xr-x   0 pork      (1000) pork      (1000)        0 2024-05-09 06:04:30.052355 punkweb_bb-0.1.4/punkweb_bb/static/punkweb_bb/
-drwxr-xr-x   0 pork      (1000) pork      (1000)        0 2024-05-09 06:04:30.052355 punkweb_bb-0.1.4/punkweb_bb/static/punkweb_bb/css/
--rw-r--r--   0 pork      (1000) pork      (1000)     1455 2024-04-06 07:32:15.000000 punkweb_bb-0.1.4/punkweb_bb/static/punkweb_bb/css/defaults.css
--rw-r--r--   0 pork      (1000) pork      (1000)     1331 2024-04-06 07:48:47.000000 punkweb_bb-0.1.4/punkweb_bb/static/punkweb_bb/css/index.css
--rw-r--r--   0 pork      (1000) pork      (1000)      234 2024-04-03 22:23:23.000000 punkweb_bb-0.1.4/punkweb_bb/static/punkweb_bb/css/login.css
--rw-r--r--   0 pork      (1000) pork      (1000)      395 2024-04-08 22:57:27.000000 punkweb_bb-0.1.4/punkweb_bb/static/punkweb_bb/css/members.css
--rw-r--r--   0 pork      (1000) pork      (1000)      321 2024-04-03 21:47:53.000000 punkweb_bb-0.1.4/punkweb_bb/static/punkweb_bb/css/post-form.css
--rw-r--r--   0 pork      (1000) pork      (1000)      916 2024-05-07 01:46:57.000000 punkweb_bb-0.1.4/punkweb_bb/static/punkweb_bb/css/profile.css
--rw-r--r--   0 pork      (1000) pork      (1000)     1296 2024-04-05 22:11:56.000000 punkweb_bb-0.1.4/punkweb_bb/static/punkweb_bb/css/punkweb-modal.css
--rw-r--r--   0 pork      (1000) pork      (1000)    11745 2024-05-09 05:20:26.000000 punkweb_bb-0.1.4/punkweb_bb/static/punkweb_bb/css/punkweb.css
--rw-r--r--   0 pork      (1000) pork      (1000)      308 2024-04-06 07:53:29.000000 punkweb_bb-0.1.4/punkweb_bb/static/punkweb_bb/css/settings.css
--rw-r--r--   0 pork      (1000) pork      (1000)      333 2024-04-08 23:25:45.000000 punkweb_bb-0.1.4/punkweb_bb/static/punkweb_bb/css/shoutbox.css
--rw-r--r--   0 pork      (1000) pork      (1000)      536 2024-04-06 07:48:52.000000 punkweb_bb-0.1.4/punkweb_bb/static/punkweb_bb/css/subcategory.css
--rw-r--r--   0 pork      (1000) pork      (1000)      329 2024-04-03 19:20:08.000000 punkweb_bb-0.1.4/punkweb_bb/static/punkweb_bb/css/thread-form.css
--rw-r--r--   0 pork      (1000) pork      (1000)     1508 2024-04-06 07:53:50.000000 punkweb_bb-0.1.4/punkweb_bb/static/punkweb_bb/css/thread.css
--rw-r--r--   0 pork      (1000) pork      (1000)      448 2024-04-05 15:05:58.000000 punkweb_bb-0.1.4/punkweb_bb/static/punkweb_bb/css/typography.css
--rw-r--r--   0 pork      (1000) pork      (1000)     1154 2024-04-05 19:38:35.000000 punkweb_bb-0.1.4/punkweb_bb/static/punkweb_bb/css/variables.css
-drwxr-xr-x   0 pork      (1000) pork      (1000)        0 2024-05-09 06:04:30.052355 punkweb_bb-0.1.4/punkweb_bb/static/punkweb_bb/editor/
--rw-r--r--   0 pork      (1000) pork      (1000)     1466 2024-04-06 07:32:28.000000 punkweb_bb-0.1.4/punkweb_bb/static/punkweb_bb/editor/bbcode-editor-content.css
--rw-r--r--   0 pork      (1000) pork      (1000)     1624 2024-04-03 19:20:08.000000 punkweb_bb-0.1.4/punkweb_bb/static/punkweb_bb/editor/bbcode-editor-tags.js
--rw-r--r--   0 pork      (1000) pork      (1000)        0 2024-04-03 19:20:08.000000 punkweb_bb-0.1.4/punkweb_bb/static/punkweb_bb/editor/bbcode-editor.css
--rw-r--r--   0 pork      (1000) pork      (1000)      606 2024-04-08 22:10:44.000000 punkweb_bb-0.1.4/punkweb_bb/static/punkweb_bb/editor/bbcode-editor.js
--rw-r--r--   0 pork      (1000) pork      (1000)      318 2024-04-03 19:11:51.000000 punkweb_bb-0.1.4/punkweb_bb/static/punkweb_bb/favicon.ico
-drwxr-xr-x   0 pork      (1000) pork      (1000)        0 2024-05-09 06:04:30.052355 punkweb_bb-0.1.4/punkweb_bb/static/punkweb_bb/img/
--rw-r--r--   0 pork      (1000) pork      (1000)    60475 2024-04-03 19:20:08.000000 punkweb_bb-0.1.4/punkweb_bb/static/punkweb_bb/img/default-profile-image.png
-drwxr-xr-x   0 pork      (1000) pork      (1000)        0 2024-05-09 06:04:30.052355 punkweb_bb-0.1.4/punkweb_bb/static/punkweb_bb/js/
--rw-r--r--   0 pork      (1000) pork      (1000)      179 2024-04-03 19:20:08.000000 punkweb_bb-0.1.4/punkweb_bb/static/punkweb_bb/js/punkweb-modal.js
--rw-r--r--   0 pork      (1000) pork      (1000)      142 2024-04-08 20:20:47.000000 punkweb_bb-0.1.4/punkweb_bb/static/punkweb_bb/js/shoutbox.js
-drwxr-xr-x   0 pork      (1000) pork      (1000)        0 2024-05-09 06:04:30.052355 punkweb_bb-0.1.4/punkweb_bb/static/punkweb_bb/vendor/
--rw-r--r--   0 pork      (1000) pork      (1000)    44307 2024-04-03 19:17:23.000000 punkweb_bb-0.1.4/punkweb_bb/static/punkweb_bb/vendor/htmx-1.9.4.min.js
--rw-r--r--   0 pork      (1000) pork      (1000)    87461 2024-04-03 19:11:51.000000 punkweb_bb-0.1.4/punkweb_bb/static/punkweb_bb/vendor/jquery-3.7.0.min.js
--rw-r--r--   0 pork      (1000) pork      (1000)    10331 2024-04-03 19:11:51.000000 punkweb_bb-0.1.4/punkweb_bb/static/punkweb_bb/vendor/open-color.css
--rw-r--r--   0 pork      (1000) pork      (1000)     3948 2024-04-03 19:11:51.000000 punkweb_bb-0.1.4/punkweb_bb/static/punkweb_bb/vendor/prism.css
--rw-r--r--   0 pork      (1000) pork      (1000)   576492 2024-04-03 19:11:51.000000 punkweb_bb-0.1.4/punkweb_bb/static/punkweb_bb/vendor/prism.js
-drwxr-xr-x   0 pork      (1000) pork      (1000)        0 2024-05-09 06:04:30.052355 punkweb_bb-0.1.4/punkweb_bb/static/punkweb_bb/vendor/sceditor-3.2.0/
--rw-r--r--   0 pork      (1000) pork      (1000)     4129 2024-04-03 19:11:51.000000 punkweb_bb-0.1.4/punkweb_bb/static/punkweb_bb/vendor/sceditor-3.2.0/README.md
-drwxr-xr-x   0 pork      (1000) pork      (1000)        0 2024-05-09 06:04:30.052355 punkweb_bb-0.1.4/punkweb_bb/static/punkweb_bb/vendor/sceditor-3.2.0/development/
-drwxr-xr-x   0 pork      (1000) pork      (1000)        0 2024-05-09 06:04:30.052355 punkweb_bb-0.1.4/punkweb_bb/static/punkweb_bb/vendor/sceditor-3.2.0/development/formats/
--rw-r--r--   0 pork      (1000) pork      (1000)    61679 2024-04-03 19:11:51.000000 punkweb_bb-0.1.4/punkweb_bb/static/punkweb_bb/vendor/sceditor-3.2.0/development/formats/bbcode.js
--rw-r--r--   0 pork      (1000) pork      (1000)    26086 2024-04-03 19:11:51.000000 punkweb_bb-0.1.4/punkweb_bb/static/punkweb_bb/vendor/sceditor-3.2.0/development/formats/xhtml.js
-drwxr-xr-x   0 pork      (1000) pork      (1000)        0 2024-05-09 06:04:30.052355 punkweb_bb-0.1.4/punkweb_bb/static/punkweb_bb/vendor/sceditor-3.2.0/development/icons/
--rw-r--r--   0 pork      (1000) pork      (1000)    11260 2024-04-03 19:11:51.000000 punkweb_bb-0.1.4/punkweb_bb/static/punkweb_bb/vendor/sceditor-3.2.0/development/icons/material.js
--rw-r--r--   0 pork      (1000) pork      (1000)    15873 2024-04-03 19:11:51.000000 punkweb_bb-0.1.4/punkweb_bb/static/punkweb_bb/vendor/sceditor-3.2.0/development/icons/monocons.js
--rw-r--r--   0 pork      (1000) pork      (1000)   312959 2024-04-03 19:11:51.000000 punkweb_bb-0.1.4/punkweb_bb/static/punkweb_bb/vendor/sceditor-3.2.0/development/jquery.sceditor.bbcode.js
--rw-r--r--   0 pork      (1000) pork      (1000)   251279 2024-04-03 19:11:51.000000 punkweb_bb-0.1.4/punkweb_bb/static/punkweb_bb/vendor/sceditor-3.2.0/development/jquery.sceditor.js
--rw-r--r--   0 pork      (1000) pork      (1000)   277366 2024-04-03 19:11:51.000000 punkweb_bb-0.1.4/punkweb_bb/static/punkweb_bb/vendor/sceditor-3.2.0/development/jquery.sceditor.xhtml.js
-drwxr-xr-x   0 pork      (1000) pork      (1000)        0 2024-05-09 06:04:30.056355 punkweb_bb-0.1.4/punkweb_bb/static/punkweb_bb/vendor/sceditor-3.2.0/development/plugins/
--rw-r--r--   0 pork      (1000) pork      (1000)     3446 2024-04-03 19:11:51.000000 punkweb_bb-0.1.4/punkweb_bb/static/punkweb_bb/vendor/sceditor-3.2.0/development/plugins/alternative-lists.js
--rw-r--r--   0 pork      (1000) pork      (1000)     2571 2024-04-03 19:11:51.000000 punkweb_bb-0.1.4/punkweb_bb/static/punkweb_bb/vendor/sceditor-3.2.0/development/plugins/autosave.js
--rw-r--r--   0 pork      (1000) pork      (1000)     2791 2024-04-03 19:11:51.000000 punkweb_bb-0.1.4/punkweb_bb/static/punkweb_bb/vendor/sceditor-3.2.0/development/plugins/autoyoutube.js
--rw-r--r--   0 pork      (1000) pork      (1000)     6306 2024-04-03 19:11:51.000000 punkweb_bb-0.1.4/punkweb_bb/static/punkweb_bb/vendor/sceditor-3.2.0/development/plugins/dragdrop.js
--rw-r--r--   0 pork      (1000) pork      (1000)     2528 2024-04-03 19:11:51.000000 punkweb_bb-0.1.4/punkweb_bb/static/punkweb_bb/vendor/sceditor-3.2.0/development/plugins/format.js
--rw-r--r--   0 pork      (1000) pork      (1000)     2059 2024-04-03 19:11:51.000000 punkweb_bb-0.1.4/punkweb_bb/static/punkweb_bb/vendor/sceditor-3.2.0/development/plugins/plaintext.js
--rw-r--r--   0 pork      (1000) pork      (1000)     9375 2024-04-03 19:11:51.000000 punkweb_bb-0.1.4/punkweb_bb/static/punkweb_bb/vendor/sceditor-3.2.0/development/plugins/undo.js
--rw-r--r--   0 pork      (1000) pork      (1000)     2067 2024-04-03 19:11:51.000000 punkweb_bb-0.1.4/punkweb_bb/static/punkweb_bb/vendor/sceditor-3.2.0/development/plugins/v1compat.js
--rw-r--r--   0 pork      (1000) pork      (1000)   249123 2024-04-03 19:11:51.000000 punkweb_bb-0.1.4/punkweb_bb/static/punkweb_bb/vendor/sceditor-3.2.0/development/sceditor.js
-drwxr-xr-x   0 pork      (1000) pork      (1000)        0 2024-05-09 06:04:30.056355 punkweb_bb-0.1.4/punkweb_bb/static/punkweb_bb/vendor/sceditor-3.2.0/development/themes/
-drwxr-xr-x   0 pork      (1000) pork      (1000)        0 2024-05-09 06:04:30.056355 punkweb_bb-0.1.4/punkweb_bb/static/punkweb_bb/vendor/sceditor-3.2.0/development/themes/content/
--rw-r--r--   0 pork      (1000) pork      (1000)     1476 2024-04-03 19:11:51.000000 punkweb_bb-0.1.4/punkweb_bb/static/punkweb_bb/vendor/sceditor-3.2.0/development/themes/content/default.css
--rw-r--r--   0 pork      (1000) pork      (1000)    11194 2024-04-03 19:11:51.000000 punkweb_bb-0.1.4/punkweb_bb/static/punkweb_bb/vendor/sceditor-3.2.0/development/themes/default.css
--rw-r--r--   0 pork      (1000) pork      (1000)    11500 2024-04-03 19:11:51.000000 punkweb_bb-0.1.4/punkweb_bb/static/punkweb_bb/vendor/sceditor-3.2.0/development/themes/defaultdark.css
--rw-r--r--   0 pork      (1000) pork      (1000)     4583 2024-04-03 19:11:51.000000 punkweb_bb-0.1.4/punkweb_bb/static/punkweb_bb/vendor/sceditor-3.2.0/development/themes/famfamfam.png
--rw-r--r--   0 pork      (1000) pork      (1000)    12943 2024-04-03 19:11:51.000000 punkweb_bb-0.1.4/punkweb_bb/static/punkweb_bb/vendor/sceditor-3.2.0/development/themes/modern.css
--rw-r--r--   0 pork      (1000) pork      (1000)    13431 2024-04-03 19:11:51.000000 punkweb_bb-0.1.4/punkweb_bb/static/punkweb_bb/vendor/sceditor-3.2.0/development/themes/office-toolbar.css
--rw-r--r--   0 pork      (1000) pork      (1000)    14124 2024-04-03 19:11:51.000000 punkweb_bb-0.1.4/punkweb_bb/static/punkweb_bb/vendor/sceditor-3.2.0/development/themes/office.css
--rw-r--r--   0 pork      (1000) pork      (1000)    13183 2024-04-03 19:11:51.000000 punkweb_bb-0.1.4/punkweb_bb/static/punkweb_bb/vendor/sceditor-3.2.0/development/themes/square.css
-drwxr-xr-x   0 pork      (1000) pork      (1000)        0 2024-05-09 06:04:30.056355 punkweb_bb-0.1.4/punkweb_bb/static/punkweb_bb/vendor/sceditor-3.2.0/emoticons/
--rw-r--r--   0 pork      (1000) pork      (1000)      756 2024-04-03 19:11:51.000000 punkweb_bb-0.1.4/punkweb_bb/static/punkweb_bb/vendor/sceditor-3.2.0/emoticons/alien.png
--rw-r--r--   0 pork      (1000) pork      (1000)     1182 2024-04-03 19:11:51.000000 punkweb_bb-0.1.4/punkweb_bb/static/punkweb_bb/vendor/sceditor-3.2.0/emoticons/angel.png
--rw-r--r--   0 pork      (1000) pork      (1000)      781 2024-04-03 19:11:51.000000 punkweb_bb-0.1.4/punkweb_bb/static/punkweb_bb/vendor/sceditor-3.2.0/emoticons/angry.png
--rw-r--r--   0 pork      (1000) pork      (1000)      972 2024-04-03 19:11:51.000000 punkweb_bb-0.1.4/punkweb_bb/static/punkweb_bb/vendor/sceditor-3.2.0/emoticons/blink.png
--rw-r--r--   0 pork      (1000) pork      (1000)      865 2024-04-03 19:11:51.000000 punkweb_bb-0.1.4/punkweb_bb/static/punkweb_bb/vendor/sceditor-3.2.0/emoticons/blush.png
--rw-r--r--   0 pork      (1000) pork      (1000)      753 2024-04-03 19:11:51.000000 punkweb_bb-0.1.4/punkweb_bb/static/punkweb_bb/vendor/sceditor-3.2.0/emoticons/cheerful.png
--rw-r--r--   0 pork      (1000) pork      (1000)      965 2024-04-03 19:11:51.000000 punkweb_bb-0.1.4/punkweb_bb/static/punkweb_bb/vendor/sceditor-3.2.0/emoticons/cool.png
--rw-r--r--   0 pork      (1000) pork      (1000)      421 2024-04-03 19:11:51.000000 punkweb_bb-0.1.4/punkweb_bb/static/punkweb_bb/vendor/sceditor-3.2.0/emoticons/credits.txt
--rw-r--r--   0 pork      (1000) pork      (1000)      877 2024-04-03 19:11:51.000000 punkweb_bb-0.1.4/punkweb_bb/static/punkweb_bb/vendor/sceditor-3.2.0/emoticons/cwy.png
--rw-r--r--   0 pork      (1000) pork      (1000)     1012 2024-04-03 19:11:51.000000 punkweb_bb-0.1.4/punkweb_bb/static/punkweb_bb/vendor/sceditor-3.2.0/emoticons/devil.png
--rw-r--r--   0 pork      (1000) pork      (1000)      991 2024-04-03 19:11:51.000000 punkweb_bb-0.1.4/punkweb_bb/static/punkweb_bb/vendor/sceditor-3.2.0/emoticons/dizzy.png
--rw-r--r--   0 pork      (1000) pork      (1000)      983 2024-04-03 19:11:51.000000 punkweb_bb-0.1.4/punkweb_bb/static/punkweb_bb/vendor/sceditor-3.2.0/emoticons/ermm.png
--rw-r--r--   0 pork      (1000) pork      (1000)      793 2024-04-03 19:11:51.000000 punkweb_bb-0.1.4/punkweb_bb/static/punkweb_bb/vendor/sceditor-3.2.0/emoticons/face.png
--rw-r--r--   0 pork      (1000) pork      (1000)      792 2024-04-03 19:11:51.000000 punkweb_bb-0.1.4/punkweb_bb/static/punkweb_bb/vendor/sceditor-3.2.0/emoticons/getlost.png
--rw-r--r--   0 pork      (1000) pork      (1000)      867 2024-04-03 19:11:51.000000 punkweb_bb-0.1.4/punkweb_bb/static/punkweb_bb/vendor/sceditor-3.2.0/emoticons/grin.png
--rw-r--r--   0 pork      (1000) pork      (1000)      792 2024-04-03 19:11:51.000000 punkweb_bb-0.1.4/punkweb_bb/static/punkweb_bb/vendor/sceditor-3.2.0/emoticons/happy.png
--rw-r--r--   0 pork      (1000) pork      (1000)      572 2024-04-03 19:11:51.000000 punkweb_bb-0.1.4/punkweb_bb/static/punkweb_bb/vendor/sceditor-3.2.0/emoticons/heart.png
--rw-r--r--   0 pork      (1000) pork      (1000)      793 2024-04-03 19:11:51.000000 punkweb_bb-0.1.4/punkweb_bb/static/punkweb_bb/vendor/sceditor-3.2.0/emoticons/kissing.png
--rw-r--r--   0 pork      (1000) pork      (1000)      912 2024-04-03 19:11:51.000000 punkweb_bb-0.1.4/punkweb_bb/static/punkweb_bb/vendor/sceditor-3.2.0/emoticons/laughing.png
--rw-r--r--   0 pork      (1000) pork      (1000)      694 2024-04-03 19:11:51.000000 punkweb_bb-0.1.4/punkweb_bb/static/punkweb_bb/vendor/sceditor-3.2.0/emoticons/ninja.png
--rw-r--r--   0 pork      (1000) pork      (1000)      804 2024-04-03 19:11:51.000000 punkweb_bb-0.1.4/punkweb_bb/static/punkweb_bb/vendor/sceditor-3.2.0/emoticons/pinch.png
--rw-r--r--   0 pork      (1000) pork      (1000)      799 2024-04-03 19:11:51.000000 punkweb_bb-0.1.4/punkweb_bb/static/punkweb_bb/vendor/sceditor-3.2.0/emoticons/pouty.png
--rw-r--r--   0 pork      (1000) pork      (1000)      789 2024-04-03 19:11:51.000000 punkweb_bb-0.1.4/punkweb_bb/static/punkweb_bb/vendor/sceditor-3.2.0/emoticons/sad.png
--rw-r--r--   0 pork      (1000) pork      (1000)      780 2024-04-03 19:11:51.000000 punkweb_bb-0.1.4/punkweb_bb/static/punkweb_bb/vendor/sceditor-3.2.0/emoticons/shocked.png
--rw-r--r--   0 pork      (1000) pork      (1000)      783 2024-04-03 19:11:51.000000 punkweb_bb-0.1.4/punkweb_bb/static/punkweb_bb/vendor/sceditor-3.2.0/emoticons/sick.png
--rw-r--r--   0 pork      (1000) pork      (1000)      788 2024-04-03 19:11:51.000000 punkweb_bb-0.1.4/punkweb_bb/static/punkweb_bb/vendor/sceditor-3.2.0/emoticons/sideways.png
--rw-r--r--   0 pork      (1000) pork      (1000)      930 2024-04-03 19:11:51.000000 punkweb_bb-0.1.4/punkweb_bb/static/punkweb_bb/vendor/sceditor-3.2.0/emoticons/silly.png
--rw-r--r--   0 pork      (1000) pork      (1000)     1039 2024-04-03 19:11:51.000000 punkweb_bb-0.1.4/punkweb_bb/static/punkweb_bb/vendor/sceditor-3.2.0/emoticons/sleeping.png
--rw-r--r--   0 pork      (1000) pork      (1000)      983 2024-04-03 19:11:51.000000 punkweb_bb-0.1.4/punkweb_bb/static/punkweb_bb/vendor/sceditor-3.2.0/emoticons/smile.png
--rw-r--r--   0 pork      (1000) pork      (1000)      981 2024-04-03 19:11:51.000000 punkweb_bb-0.1.4/punkweb_bb/static/punkweb_bb/vendor/sceditor-3.2.0/emoticons/tongue.png
--rw-r--r--   0 pork      (1000) pork      (1000)      763 2024-04-03 19:11:51.000000 punkweb_bb-0.1.4/punkweb_bb/static/punkweb_bb/vendor/sceditor-3.2.0/emoticons/unsure.png
--rw-r--r--   0 pork      (1000) pork      (1000)      718 2024-04-03 19:11:51.000000 punkweb_bb-0.1.4/punkweb_bb/static/punkweb_bb/vendor/sceditor-3.2.0/emoticons/w00t.png
--rw-r--r--   0 pork      (1000) pork      (1000)      810 2024-04-03 19:11:51.000000 punkweb_bb-0.1.4/punkweb_bb/static/punkweb_bb/vendor/sceditor-3.2.0/emoticons/wassat.png
--rw-r--r--   0 pork      (1000) pork      (1000)     1072 2024-04-03 19:11:51.000000 punkweb_bb-0.1.4/punkweb_bb/static/punkweb_bb/vendor/sceditor-3.2.0/emoticons/whistling.png
--rw-r--r--   0 pork      (1000) pork      (1000)      791 2024-04-03 19:11:51.000000 punkweb_bb-0.1.4/punkweb_bb/static/punkweb_bb/vendor/sceditor-3.2.0/emoticons/wink.png
--rw-r--r--   0 pork      (1000) pork      (1000)     1010 2024-04-03 19:11:51.000000 punkweb_bb-0.1.4/punkweb_bb/static/punkweb_bb/vendor/sceditor-3.2.0/emoticons/wub.png
--rw-r--r--   0 pork      (1000) pork      (1000)     2237 2024-04-03 19:11:51.000000 punkweb_bb-0.1.4/punkweb_bb/static/punkweb_bb/vendor/sceditor-3.2.0/example.html
-drwxr-xr-x   0 pork      (1000) pork      (1000)        0 2024-05-09 06:04:30.060355 punkweb_bb-0.1.4/punkweb_bb/static/punkweb_bb/vendor/sceditor-3.2.0/languages/
--rw-r--r--   0 pork      (1000) pork      (1000)     3235 2024-04-03 19:11:51.000000 punkweb_bb-0.1.4/punkweb_bb/static/punkweb_bb/vendor/sceditor-3.2.0/languages/ar.js
--rw-r--r--   0 pork      (1000) pork      (1000)     2803 2024-04-03 19:11:51.000000 punkweb_bb-0.1.4/punkweb_bb/static/punkweb_bb/vendor/sceditor-3.2.0/languages/ca.js
--rw-r--r--   0 pork      (1000) pork      (1000)     2543 2024-04-03 19:11:51.000000 punkweb_bb-0.1.4/punkweb_bb/static/punkweb_bb/vendor/sceditor-3.2.0/languages/cn.js
--rw-r--r--   0 pork      (1000) pork      (1000)     2879 2024-04-03 19:11:51.000000 punkweb_bb-0.1.4/punkweb_bb/static/punkweb_bb/vendor/sceditor-3.2.0/languages/cs.js
--rw-r--r--   0 pork      (1000) pork      (1000)     2504 2024-04-03 19:11:51.000000 punkweb_bb-0.1.4/punkweb_bb/static/punkweb_bb/vendor/sceditor-3.2.0/languages/de.js
--rw-r--r--   0 pork      (1000) pork      (1000)     4020 2024-04-03 19:11:51.000000 punkweb_bb-0.1.4/punkweb_bb/static/punkweb_bb/vendor/sceditor-3.2.0/languages/el.js
--rw-r--r--   0 pork      (1000) pork      (1000)      102 2024-04-03 19:11:51.000000 punkweb_bb-0.1.4/punkweb_bb/static/punkweb_bb/vendor/sceditor-3.2.0/languages/en-US.js
--rw-r--r--   0 pork      (1000) pork      (1000)      250 2024-04-03 19:11:51.000000 punkweb_bb-0.1.4/punkweb_bb/static/punkweb_bb/vendor/sceditor-3.2.0/languages/en.js
--rw-r--r--   0 pork      (1000) pork      (1000)     2831 2024-04-03 19:11:51.000000 punkweb_bb-0.1.4/punkweb_bb/static/punkweb_bb/vendor/sceditor-3.2.0/languages/es.js
--rw-r--r--   0 pork      (1000) pork      (1000)     2018 2024-04-03 19:11:51.000000 punkweb_bb-0.1.4/punkweb_bb/static/punkweb_bb/vendor/sceditor-3.2.0/languages/et.js
--rw-r--r--   0 pork      (1000) pork      (1000)     3577 2024-04-03 19:11:51.000000 punkweb_bb-0.1.4/punkweb_bb/static/punkweb_bb/vendor/sceditor-3.2.0/languages/fa.js
--rw-r--r--   0 pork      (1000) pork      (1000)     2813 2024-04-03 19:11:51.000000 punkweb_bb-0.1.4/punkweb_bb/static/punkweb_bb/vendor/sceditor-3.2.0/languages/fi.js
--rw-r--r--   0 pork      (1000) pork      (1000)     2906 2024-04-03 19:11:51.000000 punkweb_bb-0.1.4/punkweb_bb/static/punkweb_bb/vendor/sceditor-3.2.0/languages/fr.js
--rw-r--r--   0 pork      (1000) pork      (1000)     2802 2024-04-03 19:11:51.000000 punkweb_bb-0.1.4/punkweb_bb/static/punkweb_bb/vendor/sceditor-3.2.0/languages/gl.js
--rw-r--r--   0 pork      (1000) pork      (1000)     2956 2024-04-03 19:11:51.000000 punkweb_bb-0.1.4/punkweb_bb/static/punkweb_bb/vendor/sceditor-3.2.0/languages/hu.js
--rw-r--r--   0 pork      (1000) pork      (1000)     2718 2024-04-03 19:11:51.000000 punkweb_bb-0.1.4/punkweb_bb/static/punkweb_bb/vendor/sceditor-3.2.0/languages/id.js
--rw-r--r--   0 pork      (1000) pork      (1000)     2981 2024-04-03 19:11:51.000000 punkweb_bb-0.1.4/punkweb_bb/static/punkweb_bb/vendor/sceditor-3.2.0/languages/it.js
--rw-r--r--   0 pork      (1000) pork      (1000)     3259 2024-04-03 19:11:51.000000 punkweb_bb-0.1.4/punkweb_bb/static/punkweb_bb/vendor/sceditor-3.2.0/languages/ja.js
--rw-r--r--   0 pork      (1000) pork      (1000)     3141 2024-04-03 19:11:51.000000 punkweb_bb-0.1.4/punkweb_bb/static/punkweb_bb/vendor/sceditor-3.2.0/languages/lt.js
--rw-r--r--   0 pork      (1000) pork      (1000)     2797 2024-04-03 19:11:51.000000 punkweb_bb-0.1.4/punkweb_bb/static/punkweb_bb/vendor/sceditor-3.2.0/languages/nb.js
--rw-r--r--   0 pork      (1000) pork      (1000)     2903 2024-04-03 19:11:51.000000 punkweb_bb-0.1.4/punkweb_bb/static/punkweb_bb/vendor/sceditor-3.2.0/languages/nl.js
--rw-r--r--   0 pork      (1000) pork      (1000)     2745 2024-04-03 19:11:51.000000 punkweb_bb-0.1.4/punkweb_bb/static/punkweb_bb/vendor/sceditor-3.2.0/languages/pl.js
--rw-r--r--   0 pork      (1000) pork      (1000)     2739 2024-04-03 19:11:51.000000 punkweb_bb-0.1.4/punkweb_bb/static/punkweb_bb/vendor/sceditor-3.2.0/languages/pt-BR.js
--rw-r--r--   0 pork      (1000) pork      (1000)     2810 2024-04-03 19:11:51.000000 punkweb_bb-0.1.4/punkweb_bb/static/punkweb_bb/vendor/sceditor-3.2.0/languages/pt.js
--rw-r--r--   0 pork      (1000) pork      (1000)     3192 2024-04-03 19:11:51.000000 punkweb_bb-0.1.4/punkweb_bb/static/punkweb_bb/vendor/sceditor-3.2.0/languages/ru.js
--rw-r--r--   0 pork      (1000) pork      (1000)     3017 2024-04-03 19:11:51.000000 punkweb_bb-0.1.4/punkweb_bb/static/punkweb_bb/vendor/sceditor-3.2.0/languages/sk.js
--rw-r--r--   0 pork      (1000) pork      (1000)     2210 2024-04-03 19:11:51.000000 punkweb_bb-0.1.4/punkweb_bb/static/punkweb_bb/vendor/sceditor-3.2.0/languages/sv.js
--rw-r--r--   0 pork      (1000) pork      (1000)     2122 2024-04-03 19:11:51.000000 punkweb_bb-0.1.4/punkweb_bb/static/punkweb_bb/vendor/sceditor-3.2.0/languages/template.js
--rw-r--r--   0 pork      (1000) pork      (1000)     2772 2024-04-03 19:11:51.000000 punkweb_bb-0.1.4/punkweb_bb/static/punkweb_bb/vendor/sceditor-3.2.0/languages/tr.js
--rw-r--r--   0 pork      (1000) pork      (1000)     2557 2024-04-03 19:11:51.000000 punkweb_bb-0.1.4/punkweb_bb/static/punkweb_bb/vendor/sceditor-3.2.0/languages/tw.js
--rw-r--r--   0 pork      (1000) pork      (1000)     3102 2024-04-03 19:11:51.000000 punkweb_bb-0.1.4/punkweb_bb/static/punkweb_bb/vendor/sceditor-3.2.0/languages/uk.js
--rw-r--r--   0 pork      (1000) pork      (1000)     2913 2024-04-03 19:11:51.000000 punkweb_bb-0.1.4/punkweb_bb/static/punkweb_bb/vendor/sceditor-3.2.0/languages/vi.js
-drwxr-xr-x   0 pork      (1000) pork      (1000)        0 2024-05-09 06:04:30.060355 punkweb_bb-0.1.4/punkweb_bb/static/punkweb_bb/vendor/sceditor-3.2.0/minified/
-drwxr-xr-x   0 pork      (1000) pork      (1000)        0 2024-05-09 06:04:30.060355 punkweb_bb-0.1.4/punkweb_bb/static/punkweb_bb/vendor/sceditor-3.2.0/minified/formats/
--rw-r--r--   0 pork      (1000) pork      (1000)    17567 2024-04-03 19:11:51.000000 punkweb_bb-0.1.4/punkweb_bb/static/punkweb_bb/vendor/sceditor-3.2.0/minified/formats/bbcode.js
--rw-r--r--   0 pork      (1000) pork      (1000)     8873 2024-04-03 19:11:51.000000 punkweb_bb-0.1.4/punkweb_bb/static/punkweb_bb/vendor/sceditor-3.2.0/minified/formats/xhtml.js
-drwxr-xr-x   0 pork      (1000) pork      (1000)        0 2024-05-09 06:04:30.060355 punkweb_bb-0.1.4/punkweb_bb/static/punkweb_bb/vendor/sceditor-3.2.0/minified/icons/
--rw-r--r--   0 pork      (1000) pork      (1000)     9203 2024-04-03 19:11:51.000000 punkweb_bb-0.1.4/punkweb_bb/static/punkweb_bb/vendor/sceditor-3.2.0/minified/icons/material.js
--rw-r--r--   0 pork      (1000) pork      (1000)    14779 2024-04-03 19:11:51.000000 punkweb_bb-0.1.4/punkweb_bb/static/punkweb_bb/vendor/sceditor-3.2.0/minified/icons/monocons.js
--rw-r--r--   0 pork      (1000) pork      (1000)    91043 2024-04-03 19:11:51.000000 punkweb_bb-0.1.4/punkweb_bb/static/punkweb_bb/vendor/sceditor-3.2.0/minified/jquery.sceditor.bbcode.min.js
--rw-r--r--   0 pork      (1000) pork      (1000)    73632 2024-04-03 19:11:51.000000 punkweb_bb-0.1.4/punkweb_bb/static/punkweb_bb/vendor/sceditor-3.2.0/minified/jquery.sceditor.min.js
--rw-r--r--   0 pork      (1000) pork      (1000)    82349 2024-04-03 19:11:51.000000 punkweb_bb-0.1.4/punkweb_bb/static/punkweb_bb/vendor/sceditor-3.2.0/minified/jquery.sceditor.xhtml.min.js
-drwxr-xr-x   0 pork      (1000) pork      (1000)        0 2024-05-09 06:04:30.060355 punkweb_bb-0.1.4/punkweb_bb/static/punkweb_bb/vendor/sceditor-3.2.0/minified/plugins/
--rw-r--r--   0 pork      (1000) pork      (1000)     1417 2024-04-03 19:11:51.000000 punkweb_bb-0.1.4/punkweb_bb/static/punkweb_bb/vendor/sceditor-3.2.0/minified/plugins/alternative-lists.js
--rw-r--r--   0 pork      (1000) pork      (1000)     1259 2024-04-03 19:11:51.000000 punkweb_bb-0.1.4/punkweb_bb/static/punkweb_bb/vendor/sceditor-3.2.0/minified/plugins/autosave.js
--rw-r--r--   0 pork      (1000) pork      (1000)     1107 2024-04-03 19:11:51.000000 punkweb_bb-0.1.4/punkweb_bb/static/punkweb_bb/vendor/sceditor-3.2.0/minified/plugins/autoyoutube.js
--rw-r--r--   0 pork      (1000) pork      (1000)     3667 2024-04-03 19:11:51.000000 punkweb_bb-0.1.4/punkweb_bb/static/punkweb_bb/vendor/sceditor-3.2.0/minified/plugins/dragdrop.js
--rw-r--r--   0 pork      (1000) pork      (1000)     1088 2024-04-03 19:11:51.000000 punkweb_bb-0.1.4/punkweb_bb/static/punkweb_bb/vendor/sceditor-3.2.0/minified/plugins/format.js
--rw-r--r--   0 pork      (1000) pork      (1000)      775 2024-04-03 19:11:51.000000 punkweb_bb-0.1.4/punkweb_bb/static/punkweb_bb/vendor/sceditor-3.2.0/minified/plugins/plaintext.js
--rw-r--r--   0 pork      (1000) pork      (1000)     2760 2024-04-03 19:11:51.000000 punkweb_bb-0.1.4/punkweb_bb/static/punkweb_bb/vendor/sceditor-3.2.0/minified/plugins/undo.js
--rw-r--r--   0 pork      (1000) pork      (1000)      934 2024-04-03 19:11:51.000000 punkweb_bb-0.1.4/punkweb_bb/static/punkweb_bb/vendor/sceditor-3.2.0/minified/plugins/v1compat.js
--rw-r--r--   0 pork      (1000) pork      (1000)    73296 2024-04-03 19:11:51.000000 punkweb_bb-0.1.4/punkweb_bb/static/punkweb_bb/vendor/sceditor-3.2.0/minified/sceditor.min.js
-drwxr-xr-x   0 pork      (1000) pork      (1000)        0 2024-05-09 06:04:30.060355 punkweb_bb-0.1.4/punkweb_bb/static/punkweb_bb/vendor/sceditor-3.2.0/minified/themes/
-drwxr-xr-x   0 pork      (1000) pork      (1000)        0 2024-05-09 06:04:30.060355 punkweb_bb-0.1.4/punkweb_bb/static/punkweb_bb/vendor/sceditor-3.2.0/minified/themes/content/
--rw-r--r--   0 pork      (1000) pork      (1000)     1016 2024-04-03 19:11:51.000000 punkweb_bb-0.1.4/punkweb_bb/static/punkweb_bb/vendor/sceditor-3.2.0/minified/themes/content/default.min.css
--rw-r--r--   0 pork      (1000) pork      (1000)     9307 2024-04-03 19:11:51.000000 punkweb_bb-0.1.4/punkweb_bb/static/punkweb_bb/vendor/sceditor-3.2.0/minified/themes/default.min.css
--rw-r--r--   0 pork      (1000) pork      (1000)     9570 2024-04-03 19:11:51.000000 punkweb_bb-0.1.4/punkweb_bb/static/punkweb_bb/vendor/sceditor-3.2.0/minified/themes/defaultdark.min.css
--rw-r--r--   0 pork      (1000) pork      (1000)     4583 2024-04-03 19:11:51.000000 punkweb_bb-0.1.4/punkweb_bb/static/punkweb_bb/vendor/sceditor-3.2.0/minified/themes/famfamfam.png
--rw-r--r--   0 pork      (1000) pork      (1000)    10656 2024-04-03 19:11:51.000000 punkweb_bb-0.1.4/punkweb_bb/static/punkweb_bb/vendor/sceditor-3.2.0/minified/themes/modern.min.css
--rw-r--r--   0 pork      (1000) pork      (1000)    12604 2024-04-03 19:11:51.000000 punkweb_bb-0.1.4/punkweb_bb/static/punkweb_bb/vendor/sceditor-3.2.0/minified/themes/office-toolbar.min.css
--rw-r--r--   0 pork      (1000) pork      (1000)    13148 2024-04-03 19:11:51.000000 punkweb_bb-0.1.4/punkweb_bb/static/punkweb_bb/vendor/sceditor-3.2.0/minified/themes/office.min.css
--rw-r--r--   0 pork      (1000) pork      (1000)    10710 2024-04-03 19:11:51.000000 punkweb_bb-0.1.4/punkweb_bb/static/punkweb_bb/vendor/sceditor-3.2.0/minified/themes/square.min.css
-drwxr-xr-x   0 pork      (1000) pork      (1000)        0 2024-05-09 06:04:30.048355 punkweb_bb-0.1.4/punkweb_bb/templates/
-drwxr-xr-x   0 pork      (1000) pork      (1000)        0 2024-05-09 06:04:30.064355 punkweb_bb-0.1.4/punkweb_bb/templates/punkweb_bb/
--rw-r--r--   0 pork      (1000) pork      (1000)     4037 2024-05-07 02:13:59.000000 punkweb_bb-0.1.4/punkweb_bb/templates/punkweb_bb/base.html
--rw-r--r--   0 pork      (1000) pork      (1000)      460 2024-04-05 19:59:05.000000 punkweb_bb-0.1.4/punkweb_bb/templates/punkweb_bb/base_modal.html
--rw-r--r--   0 pork      (1000) pork      (1000)      396 2024-04-06 07:23:56.000000 punkweb_bb-0.1.4/punkweb_bb/templates/punkweb_bb/bbcode.html
--rw-r--r--   0 pork      (1000) pork      (1000)     8703 2024-05-09 05:55:01.000000 punkweb_bb-0.1.4/punkweb_bb/templates/punkweb_bb/index.html
--rw-r--r--   0 pork      (1000) pork      (1000)     1087 2024-04-06 02:06:29.000000 punkweb_bb-0.1.4/punkweb_bb/templates/punkweb_bb/login.html
--rw-r--r--   0 pork      (1000) pork      (1000)     2729 2024-04-08 23:13:19.000000 punkweb_bb-0.1.4/punkweb_bb/templates/punkweb_bb/members.html
-drwxr-xr-x   0 pork      (1000) pork      (1000)        0 2024-05-09 06:04:30.064355 punkweb_bb-0.1.4/punkweb_bb/templates/punkweb_bb/partials/
--rw-r--r--   0 pork      (1000) pork      (1000)      417 2024-04-06 02:06:29.000000 punkweb_bb-0.1.4/punkweb_bb/templates/punkweb_bb/partials/post_delete.html
--rw-r--r--   0 pork      (1000) pork      (1000)      565 2024-04-06 02:06:29.000000 punkweb_bb-0.1.4/punkweb_bb/templates/punkweb_bb/partials/post_update.html
--rw-r--r--   0 pork      (1000) pork      (1000)      425 2024-04-06 02:06:29.000000 punkweb_bb-0.1.4/punkweb_bb/templates/punkweb_bb/partials/thread_delete.html
--rw-r--r--   0 pork      (1000) pork      (1000)     2948 2024-04-08 23:26:38.000000 punkweb_bb-0.1.4/punkweb_bb/templates/punkweb_bb/profile.html
--rw-r--r--   0 pork      (1000) pork      (1000)     1994 2024-04-07 22:46:43.000000 punkweb_bb-0.1.4/punkweb_bb/templates/punkweb_bb/settings.html
-drwxr-xr-x   0 pork      (1000) pork      (1000)        0 2024-05-09 06:04:30.064355 punkweb_bb-0.1.4/punkweb_bb/templates/punkweb_bb/shoutbox/
--rw-r--r--   0 pork      (1000) pork      (1000)      312 2024-04-08 23:26:13.000000 punkweb_bb-0.1.4/punkweb_bb/templates/punkweb_bb/shoutbox/shout_list.html
--rw-r--r--   0 pork      (1000) pork      (1000)      672 2024-04-08 23:49:26.000000 punkweb_bb-0.1.4/punkweb_bb/templates/punkweb_bb/shoutbox/shoutbox.html
--rw-r--r--   0 pork      (1000) pork      (1000)     1167 2024-04-06 02:06:29.000000 punkweb_bb-0.1.4/punkweb_bb/templates/punkweb_bb/signup.html
--rw-r--r--   0 pork      (1000) pork      (1000)     4950 2024-05-07 04:34:46.000000 punkweb_bb-0.1.4/punkweb_bb/templates/punkweb_bb/subcategory.html
--rw-r--r--   0 pork      (1000) pork      (1000)     7595 2024-05-07 04:36:10.000000 punkweb_bb-0.1.4/punkweb_bb/templates/punkweb_bb/thread.html
--rw-r--r--   0 pork      (1000) pork      (1000)     1537 2024-05-07 04:34:23.000000 punkweb_bb-0.1.4/punkweb_bb/templates/punkweb_bb/thread_create.html
--rw-r--r--   0 pork      (1000) pork      (1000)     1730 2024-05-07 04:35:30.000000 punkweb_bb-0.1.4/punkweb_bb/templates/punkweb_bb/thread_update.html
-drwxr-xr-x   0 pork      (1000) pork      (1000)        0 2024-05-09 06:04:30.064355 punkweb_bb-0.1.4/punkweb_bb/templatetags/
--rw-r--r--   0 pork      (1000) pork      (1000)        0 2024-05-07 04:31:09.000000 punkweb_bb-0.1.4/punkweb_bb/templatetags/__init__.py
-drwxr-xr-x   0 pork      (1000) pork      (1000)        0 2024-05-09 06:04:30.064355 punkweb_bb-0.1.4/punkweb_bb/templatetags/__pycache__/
--rw-r--r--   0 pork      (1000) pork      (1000)      174 2024-05-07 04:31:10.000000 punkweb_bb-0.1.4/punkweb_bb/templatetags/__pycache__/__init__.cpython-311.pyc
--rw-r--r--   0 pork      (1000) pork      (1000)      621 2024-05-07 04:30:58.000000 punkweb_bb-0.1.4/punkweb_bb/templatetags/__pycache__/humanize_count.cpython-311.pyc
--rw-r--r--   0 pork      (1000) pork      (1000)      619 2024-05-07 04:31:10.000000 punkweb_bb-0.1.4/punkweb_bb/templatetags/__pycache__/humanize_int.cpython-311.pyc
--rw-r--r--   0 pork      (1000) pork      (1000)      833 2024-04-09 07:07:10.000000 punkweb_bb-0.1.4/punkweb_bb/templatetags/__pycache__/shoutbox_bbcode.cpython-311.pyc
--rw-r--r--   0 pork      (1000) pork      (1000)      248 2024-05-07 04:31:08.000000 punkweb_bb-0.1.4/punkweb_bb/templatetags/humanize_int.py
--rw-r--r--   0 pork      (1000) pork      (1000)      310 2024-04-09 07:07:08.000000 punkweb_bb-0.1.4/punkweb_bb/templatetags/shoutbox_bbcode.py
--rw-r--r--   0 pork      (1000) pork      (1000)    26368 2024-05-09 05:54:51.000000 punkweb_bb-0.1.4/punkweb_bb/tests.py
--rw-r--r--   0 pork      (1000) pork      (1000)     1538 2024-04-08 22:43:34.000000 punkweb_bb-0.1.4/punkweb_bb/urls.py
--rw-r--r--   0 pork      (1000) pork      (1000)    11036 2024-05-09 05:54:18.000000 punkweb_bb-0.1.4/punkweb_bb/views.py
--rw-r--r--   0 pork      (1000) pork      (1000)      840 2024-04-03 19:20:08.000000 punkweb_bb-0.1.4/punkweb_bb/widgets.py
-drwxr-xr-x   0 pork      (1000) pork      (1000)        0 2024-05-09 06:04:30.048355 punkweb_bb-0.1.4/punkweb_bb.egg-info/
--rw-r--r--   0 pork      (1000) pork      (1000)     4992 2024-05-09 06:04:30.000000 punkweb_bb-0.1.4/punkweb_bb.egg-info/PKG-INFO
--rw-r--r--   0 pork      (1000) pork      (1000)    13413 2024-05-09 06:04:30.000000 punkweb_bb-0.1.4/punkweb_bb.egg-info/SOURCES.txt
--rw-r--r--   0 pork      (1000) pork      (1000)        1 2024-05-09 06:04:30.000000 punkweb_bb-0.1.4/punkweb_bb.egg-info/dependency_links.txt
--rw-r--r--   0 pork      (1000) pork      (1000)        1 2024-04-09 07:09:59.000000 punkweb_bb-0.1.4/punkweb_bb.egg-info/not-zip-safe
--rw-r--r--   0 pork      (1000) pork      (1000)       54 2024-05-09 06:04:30.000000 punkweb_bb-0.1.4/punkweb_bb.egg-info/requires.txt
--rw-r--r--   0 pork      (1000) pork      (1000)       11 2024-05-09 06:04:30.000000 punkweb_bb-0.1.4/punkweb_bb.egg-info/top_level.txt
--rw-r--r--   0 pork      (1000) pork      (1000)       38 2024-05-09 06:04:30.064355 punkweb_bb-0.1.4/setup.cfg
--rw-r--r--   0 pork      (1000) pork      (1000)     1010 2024-05-09 06:02:08.000000 punkweb_bb-0.1.4/setup.py
+drwxr-xr-x   0 pork      (1000) pork      (1000)        0 2024-05-28 23:00:59.976560 punkweb_bb-0.2.0/
+-rw-r--r--   0 pork      (1000) pork      (1000)     1507 2024-04-09 06:08:41.000000 punkweb_bb-0.2.0/LICENSE
+-rw-r--r--   0 pork      (1000) pork      (1000)       64 2024-04-09 05:47:19.000000 punkweb_bb-0.2.0/MANIFEST.in
+-rw-r--r--   0 pork      (1000) pork      (1000)     5023 2024-05-28 23:00:59.976560 punkweb_bb-0.2.0/PKG-INFO
+-rw-r--r--   0 pork      (1000) pork      (1000)     4369 2024-05-09 06:47:11.000000 punkweb_bb-0.2.0/README.md
+drwxr-xr-x   0 pork      (1000) pork      (1000)        0 2024-05-28 23:00:59.964560 punkweb_bb-0.2.0/punkweb_bb/
+-rw-r--r--   0 pork      (1000) pork      (1000)        0 2023-08-20 16:04:51.000000 punkweb_bb-0.2.0/punkweb_bb/__init__.py
+drwxr-xr-x   0 pork      (1000) pork      (1000)        0 2024-05-28 23:00:59.964560 punkweb_bb-0.2.0/punkweb_bb/__pycache__/
+-rw-r--r--   0 pork      (1000) pork      (1000)      161 2024-04-09 05:48:25.000000 punkweb_bb-0.2.0/punkweb_bb/__pycache__/__init__.cpython-311.pyc
+-rw-r--r--   0 pork      (1000) pork      (1000)     3679 2024-04-09 05:48:25.000000 punkweb_bb-0.2.0/punkweb_bb/__pycache__/admin.cpython-311.pyc
+-rw-r--r--   0 pork      (1000) pork      (1000)     2980 2024-04-09 05:48:25.000000 punkweb_bb-0.2.0/punkweb_bb/__pycache__/admin_forms.cpython-311.pyc
+-rw-r--r--   0 pork      (1000) pork      (1000)      730 2024-04-09 06:55:15.000000 punkweb_bb-0.2.0/punkweb_bb/__pycache__/apps.cpython-311.pyc
+-rw-r--r--   0 pork      (1000) pork      (1000)     8534 2024-04-09 06:32:38.000000 punkweb_bb-0.2.0/punkweb_bb/__pycache__/bbcode_tags.cpython-311.pyc
+-rw-r--r--   0 pork      (1000) pork      (1000)      392 2024-04-09 06:44:27.000000 punkweb_bb-0.2.0/punkweb_bb/__pycache__/context_processors.cpython-311.pyc
+-rw-r--r--   0 pork      (1000) pork      (1000)     6194 2024-05-28 21:39:20.000000 punkweb_bb-0.2.0/punkweb_bb/__pycache__/forms.cpython-311.pyc
+-rw-r--r--   0 pork      (1000) pork      (1000)     1581 2024-05-09 05:36:59.000000 punkweb_bb-0.2.0/punkweb_bb/__pycache__/guests.cpython-311.pyc
+-rw-r--r--   0 pork      (1000) pork      (1000)     1560 2024-05-09 05:37:45.000000 punkweb_bb-0.2.0/punkweb_bb/__pycache__/middleware.cpython-311.pyc
+-rw-r--r--   0 pork      (1000) pork      (1000)     1478 2024-04-09 05:48:25.000000 punkweb_bb-0.2.0/punkweb_bb/__pycache__/mixins.cpython-311.pyc
+-rw-r--r--   0 pork      (1000) pork      (1000)    13824 2024-05-28 22:54:03.000000 punkweb_bb-0.2.0/punkweb_bb/__pycache__/models.cpython-311.pyc
+-rw-r--r--   0 pork      (1000) pork      (1000)      990 2024-04-09 05:48:25.000000 punkweb_bb-0.2.0/punkweb_bb/__pycache__/pagination.cpython-311.pyc
+-rw-r--r--   0 pork      (1000) pork      (1000)     5335 2024-04-09 07:07:59.000000 punkweb_bb-0.2.0/punkweb_bb/__pycache__/parsers.cpython-311.pyc
+-rw-r--r--   0 pork      (1000) pork      (1000)      448 2024-04-09 05:48:25.000000 punkweb_bb-0.2.0/punkweb_bb/__pycache__/response.cpython-311.pyc
+-rw-r--r--   0 pork      (1000) pork      (1000)      947 2024-05-09 05:27:51.000000 punkweb_bb-0.2.0/punkweb_bb/__pycache__/settings.cpython-311.pyc
+-rw-r--r--   0 pork      (1000) pork      (1000)      864 2024-04-09 05:48:25.000000 punkweb_bb-0.2.0/punkweb_bb/__pycache__/signals.cpython-311.pyc
+-rw-r--r--   0 pork      (1000) pork      (1000)    51768 2024-05-28 21:35:15.000000 punkweb_bb-0.2.0/punkweb_bb/__pycache__/tests.cpython-311.pyc
+-rw-r--r--   0 pork      (1000) pork      (1000)     3322 2024-05-28 20:10:30.000000 punkweb_bb-0.2.0/punkweb_bb/__pycache__/urls.cpython-311.pyc
+-rw-r--r--   0 pork      (1000) pork      (1000)      748 2024-05-28 21:07:24.000000 punkweb_bb-0.2.0/punkweb_bb/__pycache__/utils.cpython-311.pyc
+-rw-r--r--   0 pork      (1000) pork      (1000)    23918 2024-05-28 22:09:45.000000 punkweb_bb-0.2.0/punkweb_bb/__pycache__/views.cpython-311.pyc
+-rw-r--r--   0 pork      (1000) pork      (1000)     1552 2024-04-09 05:48:25.000000 punkweb_bb-0.2.0/punkweb_bb/__pycache__/widgets.cpython-311.pyc
+-rw-r--r--   0 pork      (1000) pork      (1000)     2493 2024-04-05 21:20:18.000000 punkweb_bb-0.2.0/punkweb_bb/admin.py
+-rw-r--r--   0 pork      (1000) pork      (1000)     1128 2024-04-03 19:18:44.000000 punkweb_bb-0.2.0/punkweb_bb/admin_forms.py
+-rw-r--r--   0 pork      (1000) pork      (1000)      207 2024-04-09 06:52:38.000000 punkweb_bb-0.2.0/punkweb_bb/apps.py
+-rw-r--r--   0 pork      (1000) pork      (1000)     4419 2024-04-09 06:31:31.000000 punkweb_bb-0.2.0/punkweb_bb/bbcode_tags.py
+-rw-r--r--   0 pork      (1000) pork      (1000)      146 2024-04-09 04:54:41.000000 punkweb_bb-0.2.0/punkweb_bb/context_processors.py
+-rw-r--r--   0 pork      (1000) pork      (1000)     2907 2024-05-28 21:39:19.000000 punkweb_bb-0.2.0/punkweb_bb/forms.py
+-rw-r--r--   0 pork      (1000) pork      (1000)      467 2024-05-09 05:36:58.000000 punkweb_bb-0.2.0/punkweb_bb/guests.py
+-rw-r--r--   0 pork      (1000) pork      (1000)      628 2024-05-09 05:37:44.000000 punkweb_bb-0.2.0/punkweb_bb/middleware.py
+drwxr-xr-x   0 pork      (1000) pork      (1000)        0 2024-05-28 23:00:59.964560 punkweb_bb-0.2.0/punkweb_bb/migrations/
+-rw-r--r--   0 pork      (1000) pork      (1000)     8950 2024-04-09 07:09:02.000000 punkweb_bb-0.2.0/punkweb_bb/migrations/0001_initial.py
+-rw-r--r--   0 pork      (1000) pork      (1000)      388 2024-05-07 04:24:13.000000 punkweb_bb-0.2.0/punkweb_bb/migrations/0002_thread_view_count.py
+-rw-r--r--   0 pork      (1000) pork      (1000)        0 2023-08-20 16:04:51.000000 punkweb_bb-0.2.0/punkweb_bb/migrations/__init__.py
+drwxr-xr-x   0 pork      (1000) pork      (1000)        0 2024-05-28 23:00:59.964560 punkweb_bb-0.2.0/punkweb_bb/migrations/__pycache__/
+-rw-r--r--   0 pork      (1000) pork      (1000)     6456 2024-04-09 07:09:10.000000 punkweb_bb-0.2.0/punkweb_bb/migrations/__pycache__/0001_initial.cpython-311.pyc
+-rw-r--r--   0 pork      (1000) pork      (1000)      815 2024-05-07 04:24:16.000000 punkweb_bb-0.2.0/punkweb_bb/migrations/__pycache__/0002_thread_view_count.cpython-311.pyc
+-rw-r--r--   0 pork      (1000) pork      (1000)      172 2024-04-09 05:48:25.000000 punkweb_bb-0.2.0/punkweb_bb/migrations/__pycache__/__init__.cpython-311.pyc
+-rw-r--r--   0 pork      (1000) pork      (1000)      395 2024-04-03 19:16:01.000000 punkweb_bb-0.2.0/punkweb_bb/mixins.py
+-rw-r--r--   0 pork      (1000) pork      (1000)     6218 2024-05-28 22:54:01.000000 punkweb_bb-0.2.0/punkweb_bb/models.py
+-rw-r--r--   0 pork      (1000) pork      (1000)      409 2024-04-06 08:06:22.000000 punkweb_bb-0.2.0/punkweb_bb/pagination.py
+-rw-r--r--   0 pork      (1000) pork      (1000)     2732 2024-04-09 07:07:58.000000 punkweb_bb-0.2.0/punkweb_bb/parsers.py
+-rw-r--r--   0 pork      (1000) pork      (1000)      130 2024-04-03 19:15:29.000000 punkweb_bb-0.2.0/punkweb_bb/response.py
+-rw-r--r--   0 pork      (1000) pork      (1000)      517 2024-05-09 05:27:49.000000 punkweb_bb-0.2.0/punkweb_bb/settings.py
+-rw-r--r--   0 pork      (1000) pork      (1000)      365 2024-04-03 19:18:44.000000 punkweb_bb-0.2.0/punkweb_bb/signals.py
+drwxr-xr-x   0 pork      (1000) pork      (1000)        0 2024-05-28 23:00:59.964560 punkweb_bb-0.2.0/punkweb_bb/static/
+drwxr-xr-x   0 pork      (1000) pork      (1000)        0 2024-05-28 23:00:59.964560 punkweb_bb-0.2.0/punkweb_bb/static/punkweb_bb/
+drwxr-xr-x   0 pork      (1000) pork      (1000)        0 2024-05-28 23:00:59.968560 punkweb_bb-0.2.0/punkweb_bb/static/punkweb_bb/css/
+-rw-r--r--   0 pork      (1000) pork      (1000)      359 2024-05-28 20:15:52.000000 punkweb_bb-0.2.0/punkweb_bb/static/punkweb_bb/css/category-form.css
+-rw-r--r--   0 pork      (1000) pork      (1000)     1455 2024-04-06 07:32:15.000000 punkweb_bb-0.2.0/punkweb_bb/static/punkweb_bb/css/defaults.css
+-rw-r--r--   0 pork      (1000) pork      (1000)     1418 2024-05-28 22:37:20.000000 punkweb_bb-0.2.0/punkweb_bb/static/punkweb_bb/css/index.css
+-rw-r--r--   0 pork      (1000) pork      (1000)      234 2024-04-03 22:23:23.000000 punkweb_bb-0.2.0/punkweb_bb/static/punkweb_bb/css/login.css
+-rw-r--r--   0 pork      (1000) pork      (1000)      395 2024-04-08 22:57:27.000000 punkweb_bb-0.2.0/punkweb_bb/static/punkweb_bb/css/members.css
+-rw-r--r--   0 pork      (1000) pork      (1000)      321 2024-04-03 21:47:53.000000 punkweb_bb-0.2.0/punkweb_bb/static/punkweb_bb/css/post-form.css
+-rw-r--r--   0 pork      (1000) pork      (1000)      916 2024-05-07 01:46:57.000000 punkweb_bb-0.2.0/punkweb_bb/static/punkweb_bb/css/profile.css
+-rw-r--r--   0 pork      (1000) pork      (1000)     1296 2024-04-05 22:11:56.000000 punkweb_bb-0.2.0/punkweb_bb/static/punkweb_bb/css/punkweb-modal.css
+-rw-r--r--   0 pork      (1000) pork      (1000)    12678 2024-05-28 22:41:43.000000 punkweb_bb-0.2.0/punkweb_bb/static/punkweb_bb/css/punkweb.css
+-rw-r--r--   0 pork      (1000) pork      (1000)      308 2024-04-06 07:53:29.000000 punkweb_bb-0.2.0/punkweb_bb/static/punkweb_bb/css/settings.css
+-rw-r--r--   0 pork      (1000) pork      (1000)      536 2024-05-28 21:51:42.000000 punkweb_bb-0.2.0/punkweb_bb/static/punkweb_bb/css/shoutbox.css
+-rw-r--r--   0 pork      (1000) pork      (1000)      371 2024-05-28 20:14:48.000000 punkweb_bb-0.2.0/punkweb_bb/static/punkweb_bb/css/subcategory-form.css
+-rw-r--r--   0 pork      (1000) pork      (1000)      711 2024-05-28 20:02:41.000000 punkweb_bb-0.2.0/punkweb_bb/static/punkweb_bb/css/subcategory.css
+-rw-r--r--   0 pork      (1000) pork      (1000)      329 2024-04-03 19:20:08.000000 punkweb_bb-0.2.0/punkweb_bb/static/punkweb_bb/css/thread-form.css
+-rw-r--r--   0 pork      (1000) pork      (1000)     1870 2024-05-28 22:52:41.000000 punkweb_bb-0.2.0/punkweb_bb/static/punkweb_bb/css/thread.css
+-rw-r--r--   0 pork      (1000) pork      (1000)      448 2024-04-05 15:05:58.000000 punkweb_bb-0.2.0/punkweb_bb/static/punkweb_bb/css/typography.css
+-rw-r--r--   0 pork      (1000) pork      (1000)     1193 2024-05-28 22:52:14.000000 punkweb_bb-0.2.0/punkweb_bb/static/punkweb_bb/css/variables.css
+drwxr-xr-x   0 pork      (1000) pork      (1000)        0 2024-05-28 23:00:59.968560 punkweb_bb-0.2.0/punkweb_bb/static/punkweb_bb/editor/
+-rw-r--r--   0 pork      (1000) pork      (1000)     1466 2024-04-06 07:32:28.000000 punkweb_bb-0.2.0/punkweb_bb/static/punkweb_bb/editor/bbcode-editor-content.css
+-rw-r--r--   0 pork      (1000) pork      (1000)     1624 2024-04-03 19:20:08.000000 punkweb_bb-0.2.0/punkweb_bb/static/punkweb_bb/editor/bbcode-editor-tags.js
+-rw-r--r--   0 pork      (1000) pork      (1000)        0 2024-04-03 19:20:08.000000 punkweb_bb-0.2.0/punkweb_bb/static/punkweb_bb/editor/bbcode-editor.css
+-rw-r--r--   0 pork      (1000) pork      (1000)      606 2024-04-08 22:10:44.000000 punkweb_bb-0.2.0/punkweb_bb/static/punkweb_bb/editor/bbcode-editor.js
+-rw-r--r--   0 pork      (1000) pork      (1000)      318 2024-04-03 19:11:51.000000 punkweb_bb-0.2.0/punkweb_bb/static/punkweb_bb/favicon.ico
+drwxr-xr-x   0 pork      (1000) pork      (1000)        0 2024-05-28 23:00:59.968560 punkweb_bb-0.2.0/punkweb_bb/static/punkweb_bb/img/
+-rw-r--r--   0 pork      (1000) pork      (1000)    60475 2024-04-03 19:20:08.000000 punkweb_bb-0.2.0/punkweb_bb/static/punkweb_bb/img/default-profile-image.png
+drwxr-xr-x   0 pork      (1000) pork      (1000)        0 2024-05-28 23:00:59.968560 punkweb_bb-0.2.0/punkweb_bb/static/punkweb_bb/js/
+-rw-r--r--   0 pork      (1000) pork      (1000)      179 2024-04-03 19:20:08.000000 punkweb_bb-0.2.0/punkweb_bb/static/punkweb_bb/js/punkweb-modal.js
+-rw-r--r--   0 pork      (1000) pork      (1000)      142 2024-04-08 20:20:47.000000 punkweb_bb-0.2.0/punkweb_bb/static/punkweb_bb/js/shoutbox.js
+drwxr-xr-x   0 pork      (1000) pork      (1000)        0 2024-05-28 23:00:59.968560 punkweb_bb-0.2.0/punkweb_bb/static/punkweb_bb/vendor/
+-rw-r--r--   0 pork      (1000) pork      (1000)    44307 2024-04-03 19:17:23.000000 punkweb_bb-0.2.0/punkweb_bb/static/punkweb_bb/vendor/htmx-1.9.4.min.js
+-rw-r--r--   0 pork      (1000) pork      (1000)    87461 2024-04-03 19:11:51.000000 punkweb_bb-0.2.0/punkweb_bb/static/punkweb_bb/vendor/jquery-3.7.0.min.js
+-rw-r--r--   0 pork      (1000) pork      (1000)    10331 2024-04-03 19:11:51.000000 punkweb_bb-0.2.0/punkweb_bb/static/punkweb_bb/vendor/open-color.css
+-rw-r--r--   0 pork      (1000) pork      (1000)     3948 2024-04-03 19:11:51.000000 punkweb_bb-0.2.0/punkweb_bb/static/punkweb_bb/vendor/prism.css
+-rw-r--r--   0 pork      (1000) pork      (1000)   576492 2024-04-03 19:11:51.000000 punkweb_bb-0.2.0/punkweb_bb/static/punkweb_bb/vendor/prism.js
+drwxr-xr-x   0 pork      (1000) pork      (1000)        0 2024-05-28 23:00:59.968560 punkweb_bb-0.2.0/punkweb_bb/static/punkweb_bb/vendor/sceditor-3.2.0/
+-rw-r--r--   0 pork      (1000) pork      (1000)     4129 2024-04-03 19:11:51.000000 punkweb_bb-0.2.0/punkweb_bb/static/punkweb_bb/vendor/sceditor-3.2.0/README.md
+drwxr-xr-x   0 pork      (1000) pork      (1000)        0 2024-05-28 23:00:59.968560 punkweb_bb-0.2.0/punkweb_bb/static/punkweb_bb/vendor/sceditor-3.2.0/development/
+drwxr-xr-x   0 pork      (1000) pork      (1000)        0 2024-05-28 23:00:59.968560 punkweb_bb-0.2.0/punkweb_bb/static/punkweb_bb/vendor/sceditor-3.2.0/development/formats/
+-rw-r--r--   0 pork      (1000) pork      (1000)    61679 2024-04-03 19:11:51.000000 punkweb_bb-0.2.0/punkweb_bb/static/punkweb_bb/vendor/sceditor-3.2.0/development/formats/bbcode.js
+-rw-r--r--   0 pork      (1000) pork      (1000)    26086 2024-04-03 19:11:51.000000 punkweb_bb-0.2.0/punkweb_bb/static/punkweb_bb/vendor/sceditor-3.2.0/development/formats/xhtml.js
+drwxr-xr-x   0 pork      (1000) pork      (1000)        0 2024-05-28 23:00:59.968560 punkweb_bb-0.2.0/punkweb_bb/static/punkweb_bb/vendor/sceditor-3.2.0/development/icons/
+-rw-r--r--   0 pork      (1000) pork      (1000)    11260 2024-04-03 19:11:51.000000 punkweb_bb-0.2.0/punkweb_bb/static/punkweb_bb/vendor/sceditor-3.2.0/development/icons/material.js
+-rw-r--r--   0 pork      (1000) pork      (1000)    15873 2024-04-03 19:11:51.000000 punkweb_bb-0.2.0/punkweb_bb/static/punkweb_bb/vendor/sceditor-3.2.0/development/icons/monocons.js
+-rw-r--r--   0 pork      (1000) pork      (1000)   312959 2024-04-03 19:11:51.000000 punkweb_bb-0.2.0/punkweb_bb/static/punkweb_bb/vendor/sceditor-3.2.0/development/jquery.sceditor.bbcode.js
+-rw-r--r--   0 pork      (1000) pork      (1000)   251279 2024-04-03 19:11:51.000000 punkweb_bb-0.2.0/punkweb_bb/static/punkweb_bb/vendor/sceditor-3.2.0/development/jquery.sceditor.js
+-rw-r--r--   0 pork      (1000) pork      (1000)   277366 2024-04-03 19:11:51.000000 punkweb_bb-0.2.0/punkweb_bb/static/punkweb_bb/vendor/sceditor-3.2.0/development/jquery.sceditor.xhtml.js
+drwxr-xr-x   0 pork      (1000) pork      (1000)        0 2024-05-28 23:00:59.968560 punkweb_bb-0.2.0/punkweb_bb/static/punkweb_bb/vendor/sceditor-3.2.0/development/plugins/
+-rw-r--r--   0 pork      (1000) pork      (1000)     3446 2024-04-03 19:11:51.000000 punkweb_bb-0.2.0/punkweb_bb/static/punkweb_bb/vendor/sceditor-3.2.0/development/plugins/alternative-lists.js
+-rw-r--r--   0 pork      (1000) pork      (1000)     2571 2024-04-03 19:11:51.000000 punkweb_bb-0.2.0/punkweb_bb/static/punkweb_bb/vendor/sceditor-3.2.0/development/plugins/autosave.js
+-rw-r--r--   0 pork      (1000) pork      (1000)     2791 2024-04-03 19:11:51.000000 punkweb_bb-0.2.0/punkweb_bb/static/punkweb_bb/vendor/sceditor-3.2.0/development/plugins/autoyoutube.js
+-rw-r--r--   0 pork      (1000) pork      (1000)     6306 2024-04-03 19:11:51.000000 punkweb_bb-0.2.0/punkweb_bb/static/punkweb_bb/vendor/sceditor-3.2.0/development/plugins/dragdrop.js
+-rw-r--r--   0 pork      (1000) pork      (1000)     2528 2024-04-03 19:11:51.000000 punkweb_bb-0.2.0/punkweb_bb/static/punkweb_bb/vendor/sceditor-3.2.0/development/plugins/format.js
+-rw-r--r--   0 pork      (1000) pork      (1000)     2059 2024-04-03 19:11:51.000000 punkweb_bb-0.2.0/punkweb_bb/static/punkweb_bb/vendor/sceditor-3.2.0/development/plugins/plaintext.js
+-rw-r--r--   0 pork      (1000) pork      (1000)     9375 2024-04-03 19:11:51.000000 punkweb_bb-0.2.0/punkweb_bb/static/punkweb_bb/vendor/sceditor-3.2.0/development/plugins/undo.js
+-rw-r--r--   0 pork      (1000) pork      (1000)     2067 2024-04-03 19:11:51.000000 punkweb_bb-0.2.0/punkweb_bb/static/punkweb_bb/vendor/sceditor-3.2.0/development/plugins/v1compat.js
+-rw-r--r--   0 pork      (1000) pork      (1000)   249123 2024-04-03 19:11:51.000000 punkweb_bb-0.2.0/punkweb_bb/static/punkweb_bb/vendor/sceditor-3.2.0/development/sceditor.js
+drwxr-xr-x   0 pork      (1000) pork      (1000)        0 2024-05-28 23:00:59.968560 punkweb_bb-0.2.0/punkweb_bb/static/punkweb_bb/vendor/sceditor-3.2.0/development/themes/
+drwxr-xr-x   0 pork      (1000) pork      (1000)        0 2024-05-28 23:00:59.968560 punkweb_bb-0.2.0/punkweb_bb/static/punkweb_bb/vendor/sceditor-3.2.0/development/themes/content/
+-rw-r--r--   0 pork      (1000) pork      (1000)     1476 2024-04-03 19:11:51.000000 punkweb_bb-0.2.0/punkweb_bb/static/punkweb_bb/vendor/sceditor-3.2.0/development/themes/content/default.css
+-rw-r--r--   0 pork      (1000) pork      (1000)    11194 2024-04-03 19:11:51.000000 punkweb_bb-0.2.0/punkweb_bb/static/punkweb_bb/vendor/sceditor-3.2.0/development/themes/default.css
+-rw-r--r--   0 pork      (1000) pork      (1000)    11500 2024-04-03 19:11:51.000000 punkweb_bb-0.2.0/punkweb_bb/static/punkweb_bb/vendor/sceditor-3.2.0/development/themes/defaultdark.css
+-rw-r--r--   0 pork      (1000) pork      (1000)     4583 2024-04-03 19:11:51.000000 punkweb_bb-0.2.0/punkweb_bb/static/punkweb_bb/vendor/sceditor-3.2.0/development/themes/famfamfam.png
+-rw-r--r--   0 pork      (1000) pork      (1000)    12943 2024-04-03 19:11:51.000000 punkweb_bb-0.2.0/punkweb_bb/static/punkweb_bb/vendor/sceditor-3.2.0/development/themes/modern.css
+-rw-r--r--   0 pork      (1000) pork      (1000)    13431 2024-04-03 19:11:51.000000 punkweb_bb-0.2.0/punkweb_bb/static/punkweb_bb/vendor/sceditor-3.2.0/development/themes/office-toolbar.css
+-rw-r--r--   0 pork      (1000) pork      (1000)    14124 2024-04-03 19:11:51.000000 punkweb_bb-0.2.0/punkweb_bb/static/punkweb_bb/vendor/sceditor-3.2.0/development/themes/office.css
+-rw-r--r--   0 pork      (1000) pork      (1000)    13183 2024-04-03 19:11:51.000000 punkweb_bb-0.2.0/punkweb_bb/static/punkweb_bb/vendor/sceditor-3.2.0/development/themes/square.css
+drwxr-xr-x   0 pork      (1000) pork      (1000)        0 2024-05-28 23:00:59.972560 punkweb_bb-0.2.0/punkweb_bb/static/punkweb_bb/vendor/sceditor-3.2.0/emoticons/
+-rw-r--r--   0 pork      (1000) pork      (1000)      756 2024-04-03 19:11:51.000000 punkweb_bb-0.2.0/punkweb_bb/static/punkweb_bb/vendor/sceditor-3.2.0/emoticons/alien.png
+-rw-r--r--   0 pork      (1000) pork      (1000)     1182 2024-04-03 19:11:51.000000 punkweb_bb-0.2.0/punkweb_bb/static/punkweb_bb/vendor/sceditor-3.2.0/emoticons/angel.png
+-rw-r--r--   0 pork      (1000) pork      (1000)      781 2024-04-03 19:11:51.000000 punkweb_bb-0.2.0/punkweb_bb/static/punkweb_bb/vendor/sceditor-3.2.0/emoticons/angry.png
+-rw-r--r--   0 pork      (1000) pork      (1000)      972 2024-04-03 19:11:51.000000 punkweb_bb-0.2.0/punkweb_bb/static/punkweb_bb/vendor/sceditor-3.2.0/emoticons/blink.png
+-rw-r--r--   0 pork      (1000) pork      (1000)      865 2024-04-03 19:11:51.000000 punkweb_bb-0.2.0/punkweb_bb/static/punkweb_bb/vendor/sceditor-3.2.0/emoticons/blush.png
+-rw-r--r--   0 pork      (1000) pork      (1000)      753 2024-04-03 19:11:51.000000 punkweb_bb-0.2.0/punkweb_bb/static/punkweb_bb/vendor/sceditor-3.2.0/emoticons/cheerful.png
+-rw-r--r--   0 pork      (1000) pork      (1000)      965 2024-04-03 19:11:51.000000 punkweb_bb-0.2.0/punkweb_bb/static/punkweb_bb/vendor/sceditor-3.2.0/emoticons/cool.png
+-rw-r--r--   0 pork      (1000) pork      (1000)      421 2024-04-03 19:11:51.000000 punkweb_bb-0.2.0/punkweb_bb/static/punkweb_bb/vendor/sceditor-3.2.0/emoticons/credits.txt
+-rw-r--r--   0 pork      (1000) pork      (1000)      877 2024-04-03 19:11:51.000000 punkweb_bb-0.2.0/punkweb_bb/static/punkweb_bb/vendor/sceditor-3.2.0/emoticons/cwy.png
+-rw-r--r--   0 pork      (1000) pork      (1000)     1012 2024-04-03 19:11:51.000000 punkweb_bb-0.2.0/punkweb_bb/static/punkweb_bb/vendor/sceditor-3.2.0/emoticons/devil.png
+-rw-r--r--   0 pork      (1000) pork      (1000)      991 2024-04-03 19:11:51.000000 punkweb_bb-0.2.0/punkweb_bb/static/punkweb_bb/vendor/sceditor-3.2.0/emoticons/dizzy.png
+-rw-r--r--   0 pork      (1000) pork      (1000)      983 2024-04-03 19:11:51.000000 punkweb_bb-0.2.0/punkweb_bb/static/punkweb_bb/vendor/sceditor-3.2.0/emoticons/ermm.png
+-rw-r--r--   0 pork      (1000) pork      (1000)      793 2024-04-03 19:11:51.000000 punkweb_bb-0.2.0/punkweb_bb/static/punkweb_bb/vendor/sceditor-3.2.0/emoticons/face.png
+-rw-r--r--   0 pork      (1000) pork      (1000)      792 2024-04-03 19:11:51.000000 punkweb_bb-0.2.0/punkweb_bb/static/punkweb_bb/vendor/sceditor-3.2.0/emoticons/getlost.png
+-rw-r--r--   0 pork      (1000) pork      (1000)      867 2024-04-03 19:11:51.000000 punkweb_bb-0.2.0/punkweb_bb/static/punkweb_bb/vendor/sceditor-3.2.0/emoticons/grin.png
+-rw-r--r--   0 pork      (1000) pork      (1000)      792 2024-04-03 19:11:51.000000 punkweb_bb-0.2.0/punkweb_bb/static/punkweb_bb/vendor/sceditor-3.2.0/emoticons/happy.png
+-rw-r--r--   0 pork      (1000) pork      (1000)      572 2024-04-03 19:11:51.000000 punkweb_bb-0.2.0/punkweb_bb/static/punkweb_bb/vendor/sceditor-3.2.0/emoticons/heart.png
+-rw-r--r--   0 pork      (1000) pork      (1000)      793 2024-04-03 19:11:51.000000 punkweb_bb-0.2.0/punkweb_bb/static/punkweb_bb/vendor/sceditor-3.2.0/emoticons/kissing.png
+-rw-r--r--   0 pork      (1000) pork      (1000)      912 2024-04-03 19:11:51.000000 punkweb_bb-0.2.0/punkweb_bb/static/punkweb_bb/vendor/sceditor-3.2.0/emoticons/laughing.png
+-rw-r--r--   0 pork      (1000) pork      (1000)      694 2024-04-03 19:11:51.000000 punkweb_bb-0.2.0/punkweb_bb/static/punkweb_bb/vendor/sceditor-3.2.0/emoticons/ninja.png
+-rw-r--r--   0 pork      (1000) pork      (1000)      804 2024-04-03 19:11:51.000000 punkweb_bb-0.2.0/punkweb_bb/static/punkweb_bb/vendor/sceditor-3.2.0/emoticons/pinch.png
+-rw-r--r--   0 pork      (1000) pork      (1000)      799 2024-04-03 19:11:51.000000 punkweb_bb-0.2.0/punkweb_bb/static/punkweb_bb/vendor/sceditor-3.2.0/emoticons/pouty.png
+-rw-r--r--   0 pork      (1000) pork      (1000)      789 2024-04-03 19:11:51.000000 punkweb_bb-0.2.0/punkweb_bb/static/punkweb_bb/vendor/sceditor-3.2.0/emoticons/sad.png
+-rw-r--r--   0 pork      (1000) pork      (1000)      780 2024-04-03 19:11:51.000000 punkweb_bb-0.2.0/punkweb_bb/static/punkweb_bb/vendor/sceditor-3.2.0/emoticons/shocked.png
+-rw-r--r--   0 pork      (1000) pork      (1000)      783 2024-04-03 19:11:51.000000 punkweb_bb-0.2.0/punkweb_bb/static/punkweb_bb/vendor/sceditor-3.2.0/emoticons/sick.png
+-rw-r--r--   0 pork      (1000) pork      (1000)      788 2024-04-03 19:11:51.000000 punkweb_bb-0.2.0/punkweb_bb/static/punkweb_bb/vendor/sceditor-3.2.0/emoticons/sideways.png
+-rw-r--r--   0 pork      (1000) pork      (1000)      930 2024-04-03 19:11:51.000000 punkweb_bb-0.2.0/punkweb_bb/static/punkweb_bb/vendor/sceditor-3.2.0/emoticons/silly.png
+-rw-r--r--   0 pork      (1000) pork      (1000)     1039 2024-04-03 19:11:51.000000 punkweb_bb-0.2.0/punkweb_bb/static/punkweb_bb/vendor/sceditor-3.2.0/emoticons/sleeping.png
+-rw-r--r--   0 pork      (1000) pork      (1000)      983 2024-04-03 19:11:51.000000 punkweb_bb-0.2.0/punkweb_bb/static/punkweb_bb/vendor/sceditor-3.2.0/emoticons/smile.png
+-rw-r--r--   0 pork      (1000) pork      (1000)      981 2024-04-03 19:11:51.000000 punkweb_bb-0.2.0/punkweb_bb/static/punkweb_bb/vendor/sceditor-3.2.0/emoticons/tongue.png
+-rw-r--r--   0 pork      (1000) pork      (1000)      763 2024-04-03 19:11:51.000000 punkweb_bb-0.2.0/punkweb_bb/static/punkweb_bb/vendor/sceditor-3.2.0/emoticons/unsure.png
+-rw-r--r--   0 pork      (1000) pork      (1000)      718 2024-04-03 19:11:51.000000 punkweb_bb-0.2.0/punkweb_bb/static/punkweb_bb/vendor/sceditor-3.2.0/emoticons/w00t.png
+-rw-r--r--   0 pork      (1000) pork      (1000)      810 2024-04-03 19:11:51.000000 punkweb_bb-0.2.0/punkweb_bb/static/punkweb_bb/vendor/sceditor-3.2.0/emoticons/wassat.png
+-rw-r--r--   0 pork      (1000) pork      (1000)     1072 2024-04-03 19:11:51.000000 punkweb_bb-0.2.0/punkweb_bb/static/punkweb_bb/vendor/sceditor-3.2.0/emoticons/whistling.png
+-rw-r--r--   0 pork      (1000) pork      (1000)      791 2024-04-03 19:11:51.000000 punkweb_bb-0.2.0/punkweb_bb/static/punkweb_bb/vendor/sceditor-3.2.0/emoticons/wink.png
+-rw-r--r--   0 pork      (1000) pork      (1000)     1010 2024-04-03 19:11:51.000000 punkweb_bb-0.2.0/punkweb_bb/static/punkweb_bb/vendor/sceditor-3.2.0/emoticons/wub.png
+-rw-r--r--   0 pork      (1000) pork      (1000)     2237 2024-04-03 19:11:51.000000 punkweb_bb-0.2.0/punkweb_bb/static/punkweb_bb/vendor/sceditor-3.2.0/example.html
+drwxr-xr-x   0 pork      (1000) pork      (1000)        0 2024-05-28 23:00:59.972560 punkweb_bb-0.2.0/punkweb_bb/static/punkweb_bb/vendor/sceditor-3.2.0/languages/
+-rw-r--r--   0 pork      (1000) pork      (1000)     3235 2024-04-03 19:11:51.000000 punkweb_bb-0.2.0/punkweb_bb/static/punkweb_bb/vendor/sceditor-3.2.0/languages/ar.js
+-rw-r--r--   0 pork      (1000) pork      (1000)     2803 2024-04-03 19:11:51.000000 punkweb_bb-0.2.0/punkweb_bb/static/punkweb_bb/vendor/sceditor-3.2.0/languages/ca.js
+-rw-r--r--   0 pork      (1000) pork      (1000)     2543 2024-04-03 19:11:51.000000 punkweb_bb-0.2.0/punkweb_bb/static/punkweb_bb/vendor/sceditor-3.2.0/languages/cn.js
+-rw-r--r--   0 pork      (1000) pork      (1000)     2879 2024-04-03 19:11:51.000000 punkweb_bb-0.2.0/punkweb_bb/static/punkweb_bb/vendor/sceditor-3.2.0/languages/cs.js
+-rw-r--r--   0 pork      (1000) pork      (1000)     2504 2024-04-03 19:11:51.000000 punkweb_bb-0.2.0/punkweb_bb/static/punkweb_bb/vendor/sceditor-3.2.0/languages/de.js
+-rw-r--r--   0 pork      (1000) pork      (1000)     4020 2024-04-03 19:11:51.000000 punkweb_bb-0.2.0/punkweb_bb/static/punkweb_bb/vendor/sceditor-3.2.0/languages/el.js
+-rw-r--r--   0 pork      (1000) pork      (1000)      102 2024-04-03 19:11:51.000000 punkweb_bb-0.2.0/punkweb_bb/static/punkweb_bb/vendor/sceditor-3.2.0/languages/en-US.js
+-rw-r--r--   0 pork      (1000) pork      (1000)      250 2024-04-03 19:11:51.000000 punkweb_bb-0.2.0/punkweb_bb/static/punkweb_bb/vendor/sceditor-3.2.0/languages/en.js
+-rw-r--r--   0 pork      (1000) pork      (1000)     2831 2024-04-03 19:11:51.000000 punkweb_bb-0.2.0/punkweb_bb/static/punkweb_bb/vendor/sceditor-3.2.0/languages/es.js
+-rw-r--r--   0 pork      (1000) pork      (1000)     2018 2024-04-03 19:11:51.000000 punkweb_bb-0.2.0/punkweb_bb/static/punkweb_bb/vendor/sceditor-3.2.0/languages/et.js
+-rw-r--r--   0 pork      (1000) pork      (1000)     3577 2024-04-03 19:11:51.000000 punkweb_bb-0.2.0/punkweb_bb/static/punkweb_bb/vendor/sceditor-3.2.0/languages/fa.js
+-rw-r--r--   0 pork      (1000) pork      (1000)     2813 2024-04-03 19:11:51.000000 punkweb_bb-0.2.0/punkweb_bb/static/punkweb_bb/vendor/sceditor-3.2.0/languages/fi.js
+-rw-r--r--   0 pork      (1000) pork      (1000)     2906 2024-04-03 19:11:51.000000 punkweb_bb-0.2.0/punkweb_bb/static/punkweb_bb/vendor/sceditor-3.2.0/languages/fr.js
+-rw-r--r--   0 pork      (1000) pork      (1000)     2802 2024-04-03 19:11:51.000000 punkweb_bb-0.2.0/punkweb_bb/static/punkweb_bb/vendor/sceditor-3.2.0/languages/gl.js
+-rw-r--r--   0 pork      (1000) pork      (1000)     2956 2024-04-03 19:11:51.000000 punkweb_bb-0.2.0/punkweb_bb/static/punkweb_bb/vendor/sceditor-3.2.0/languages/hu.js
+-rw-r--r--   0 pork      (1000) pork      (1000)     2718 2024-04-03 19:11:51.000000 punkweb_bb-0.2.0/punkweb_bb/static/punkweb_bb/vendor/sceditor-3.2.0/languages/id.js
+-rw-r--r--   0 pork      (1000) pork      (1000)     2981 2024-04-03 19:11:51.000000 punkweb_bb-0.2.0/punkweb_bb/static/punkweb_bb/vendor/sceditor-3.2.0/languages/it.js
+-rw-r--r--   0 pork      (1000) pork      (1000)     3259 2024-04-03 19:11:51.000000 punkweb_bb-0.2.0/punkweb_bb/static/punkweb_bb/vendor/sceditor-3.2.0/languages/ja.js
+-rw-r--r--   0 pork      (1000) pork      (1000)     3141 2024-04-03 19:11:51.000000 punkweb_bb-0.2.0/punkweb_bb/static/punkweb_bb/vendor/sceditor-3.2.0/languages/lt.js
+-rw-r--r--   0 pork      (1000) pork      (1000)     2797 2024-04-03 19:11:51.000000 punkweb_bb-0.2.0/punkweb_bb/static/punkweb_bb/vendor/sceditor-3.2.0/languages/nb.js
+-rw-r--r--   0 pork      (1000) pork      (1000)     2903 2024-04-03 19:11:51.000000 punkweb_bb-0.2.0/punkweb_bb/static/punkweb_bb/vendor/sceditor-3.2.0/languages/nl.js
+-rw-r--r--   0 pork      (1000) pork      (1000)     2745 2024-04-03 19:11:51.000000 punkweb_bb-0.2.0/punkweb_bb/static/punkweb_bb/vendor/sceditor-3.2.0/languages/pl.js
+-rw-r--r--   0 pork      (1000) pork      (1000)     2739 2024-04-03 19:11:51.000000 punkweb_bb-0.2.0/punkweb_bb/static/punkweb_bb/vendor/sceditor-3.2.0/languages/pt-BR.js
+-rw-r--r--   0 pork      (1000) pork      (1000)     2810 2024-04-03 19:11:51.000000 punkweb_bb-0.2.0/punkweb_bb/static/punkweb_bb/vendor/sceditor-3.2.0/languages/pt.js
+-rw-r--r--   0 pork      (1000) pork      (1000)     3192 2024-04-03 19:11:51.000000 punkweb_bb-0.2.0/punkweb_bb/static/punkweb_bb/vendor/sceditor-3.2.0/languages/ru.js
+-rw-r--r--   0 pork      (1000) pork      (1000)     3017 2024-04-03 19:11:51.000000 punkweb_bb-0.2.0/punkweb_bb/static/punkweb_bb/vendor/sceditor-3.2.0/languages/sk.js
+-rw-r--r--   0 pork      (1000) pork      (1000)     2210 2024-04-03 19:11:51.000000 punkweb_bb-0.2.0/punkweb_bb/static/punkweb_bb/vendor/sceditor-3.2.0/languages/sv.js
+-rw-r--r--   0 pork      (1000) pork      (1000)     2122 2024-04-03 19:11:51.000000 punkweb_bb-0.2.0/punkweb_bb/static/punkweb_bb/vendor/sceditor-3.2.0/languages/template.js
+-rw-r--r--   0 pork      (1000) pork      (1000)     2772 2024-04-03 19:11:51.000000 punkweb_bb-0.2.0/punkweb_bb/static/punkweb_bb/vendor/sceditor-3.2.0/languages/tr.js
+-rw-r--r--   0 pork      (1000) pork      (1000)     2557 2024-04-03 19:11:51.000000 punkweb_bb-0.2.0/punkweb_bb/static/punkweb_bb/vendor/sceditor-3.2.0/languages/tw.js
+-rw-r--r--   0 pork      (1000) pork      (1000)     3102 2024-04-03 19:11:51.000000 punkweb_bb-0.2.0/punkweb_bb/static/punkweb_bb/vendor/sceditor-3.2.0/languages/uk.js
+-rw-r--r--   0 pork      (1000) pork      (1000)     2913 2024-04-03 19:11:51.000000 punkweb_bb-0.2.0/punkweb_bb/static/punkweb_bb/vendor/sceditor-3.2.0/languages/vi.js
+drwxr-xr-x   0 pork      (1000) pork      (1000)        0 2024-05-28 23:00:59.972560 punkweb_bb-0.2.0/punkweb_bb/static/punkweb_bb/vendor/sceditor-3.2.0/minified/
+drwxr-xr-x   0 pork      (1000) pork      (1000)        0 2024-05-28 23:00:59.972560 punkweb_bb-0.2.0/punkweb_bb/static/punkweb_bb/vendor/sceditor-3.2.0/minified/formats/
+-rw-r--r--   0 pork      (1000) pork      (1000)    17567 2024-04-03 19:11:51.000000 punkweb_bb-0.2.0/punkweb_bb/static/punkweb_bb/vendor/sceditor-3.2.0/minified/formats/bbcode.js
+-rw-r--r--   0 pork      (1000) pork      (1000)     8873 2024-04-03 19:11:51.000000 punkweb_bb-0.2.0/punkweb_bb/static/punkweb_bb/vendor/sceditor-3.2.0/minified/formats/xhtml.js
+drwxr-xr-x   0 pork      (1000) pork      (1000)        0 2024-05-28 23:00:59.972560 punkweb_bb-0.2.0/punkweb_bb/static/punkweb_bb/vendor/sceditor-3.2.0/minified/icons/
+-rw-r--r--   0 pork      (1000) pork      (1000)     9203 2024-04-03 19:11:51.000000 punkweb_bb-0.2.0/punkweb_bb/static/punkweb_bb/vendor/sceditor-3.2.0/minified/icons/material.js
+-rw-r--r--   0 pork      (1000) pork      (1000)    14779 2024-04-03 19:11:51.000000 punkweb_bb-0.2.0/punkweb_bb/static/punkweb_bb/vendor/sceditor-3.2.0/minified/icons/monocons.js
+-rw-r--r--   0 pork      (1000) pork      (1000)    91043 2024-04-03 19:11:51.000000 punkweb_bb-0.2.0/punkweb_bb/static/punkweb_bb/vendor/sceditor-3.2.0/minified/jquery.sceditor.bbcode.min.js
+-rw-r--r--   0 pork      (1000) pork      (1000)    73632 2024-04-03 19:11:51.000000 punkweb_bb-0.2.0/punkweb_bb/static/punkweb_bb/vendor/sceditor-3.2.0/minified/jquery.sceditor.min.js
+-rw-r--r--   0 pork      (1000) pork      (1000)    82349 2024-04-03 19:11:51.000000 punkweb_bb-0.2.0/punkweb_bb/static/punkweb_bb/vendor/sceditor-3.2.0/minified/jquery.sceditor.xhtml.min.js
+drwxr-xr-x   0 pork      (1000) pork      (1000)        0 2024-05-28 23:00:59.972560 punkweb_bb-0.2.0/punkweb_bb/static/punkweb_bb/vendor/sceditor-3.2.0/minified/plugins/
+-rw-r--r--   0 pork      (1000) pork      (1000)     1417 2024-04-03 19:11:51.000000 punkweb_bb-0.2.0/punkweb_bb/static/punkweb_bb/vendor/sceditor-3.2.0/minified/plugins/alternative-lists.js
+-rw-r--r--   0 pork      (1000) pork      (1000)     1259 2024-04-03 19:11:51.000000 punkweb_bb-0.2.0/punkweb_bb/static/punkweb_bb/vendor/sceditor-3.2.0/minified/plugins/autosave.js
+-rw-r--r--   0 pork      (1000) pork      (1000)     1107 2024-04-03 19:11:51.000000 punkweb_bb-0.2.0/punkweb_bb/static/punkweb_bb/vendor/sceditor-3.2.0/minified/plugins/autoyoutube.js
+-rw-r--r--   0 pork      (1000) pork      (1000)     3667 2024-04-03 19:11:51.000000 punkweb_bb-0.2.0/punkweb_bb/static/punkweb_bb/vendor/sceditor-3.2.0/minified/plugins/dragdrop.js
+-rw-r--r--   0 pork      (1000) pork      (1000)     1088 2024-04-03 19:11:51.000000 punkweb_bb-0.2.0/punkweb_bb/static/punkweb_bb/vendor/sceditor-3.2.0/minified/plugins/format.js
+-rw-r--r--   0 pork      (1000) pork      (1000)      775 2024-04-03 19:11:51.000000 punkweb_bb-0.2.0/punkweb_bb/static/punkweb_bb/vendor/sceditor-3.2.0/minified/plugins/plaintext.js
+-rw-r--r--   0 pork      (1000) pork      (1000)     2760 2024-04-03 19:11:51.000000 punkweb_bb-0.2.0/punkweb_bb/static/punkweb_bb/vendor/sceditor-3.2.0/minified/plugins/undo.js
+-rw-r--r--   0 pork      (1000) pork      (1000)      934 2024-04-03 19:11:51.000000 punkweb_bb-0.2.0/punkweb_bb/static/punkweb_bb/vendor/sceditor-3.2.0/minified/plugins/v1compat.js
+-rw-r--r--   0 pork      (1000) pork      (1000)    73296 2024-04-03 19:11:51.000000 punkweb_bb-0.2.0/punkweb_bb/static/punkweb_bb/vendor/sceditor-3.2.0/minified/sceditor.min.js
+drwxr-xr-x   0 pork      (1000) pork      (1000)        0 2024-05-28 23:00:59.972560 punkweb_bb-0.2.0/punkweb_bb/static/punkweb_bb/vendor/sceditor-3.2.0/minified/themes/
+drwxr-xr-x   0 pork      (1000) pork      (1000)        0 2024-05-28 23:00:59.976560 punkweb_bb-0.2.0/punkweb_bb/static/punkweb_bb/vendor/sceditor-3.2.0/minified/themes/content/
+-rw-r--r--   0 pork      (1000) pork      (1000)     1016 2024-04-03 19:11:51.000000 punkweb_bb-0.2.0/punkweb_bb/static/punkweb_bb/vendor/sceditor-3.2.0/minified/themes/content/default.min.css
+-rw-r--r--   0 pork      (1000) pork      (1000)     9307 2024-04-03 19:11:51.000000 punkweb_bb-0.2.0/punkweb_bb/static/punkweb_bb/vendor/sceditor-3.2.0/minified/themes/default.min.css
+-rw-r--r--   0 pork      (1000) pork      (1000)     9570 2024-04-03 19:11:51.000000 punkweb_bb-0.2.0/punkweb_bb/static/punkweb_bb/vendor/sceditor-3.2.0/minified/themes/defaultdark.min.css
+-rw-r--r--   0 pork      (1000) pork      (1000)     4583 2024-04-03 19:11:51.000000 punkweb_bb-0.2.0/punkweb_bb/static/punkweb_bb/vendor/sceditor-3.2.0/minified/themes/famfamfam.png
+-rw-r--r--   0 pork      (1000) pork      (1000)    10656 2024-04-03 19:11:51.000000 punkweb_bb-0.2.0/punkweb_bb/static/punkweb_bb/vendor/sceditor-3.2.0/minified/themes/modern.min.css
+-rw-r--r--   0 pork      (1000) pork      (1000)    12604 2024-04-03 19:11:51.000000 punkweb_bb-0.2.0/punkweb_bb/static/punkweb_bb/vendor/sceditor-3.2.0/minified/themes/office-toolbar.min.css
+-rw-r--r--   0 pork      (1000) pork      (1000)    13148 2024-04-03 19:11:51.000000 punkweb_bb-0.2.0/punkweb_bb/static/punkweb_bb/vendor/sceditor-3.2.0/minified/themes/office.min.css
+-rw-r--r--   0 pork      (1000) pork      (1000)    10710 2024-04-03 19:11:51.000000 punkweb_bb-0.2.0/punkweb_bb/static/punkweb_bb/vendor/sceditor-3.2.0/minified/themes/square.min.css
+drwxr-xr-x   0 pork      (1000) pork      (1000)        0 2024-05-28 23:00:59.964560 punkweb_bb-0.2.0/punkweb_bb/templates/
+drwxr-xr-x   0 pork      (1000) pork      (1000)        0 2024-05-28 23:00:59.976560 punkweb_bb-0.2.0/punkweb_bb/templates/punkweb_bb/
+-rw-r--r--   0 pork      (1000) pork      (1000)     4037 2024-05-07 02:13:59.000000 punkweb_bb-0.2.0/punkweb_bb/templates/punkweb_bb/base.html
+-rw-r--r--   0 pork      (1000) pork      (1000)      460 2024-04-05 19:59:05.000000 punkweb_bb-0.2.0/punkweb_bb/templates/punkweb_bb/base_modal.html
+-rw-r--r--   0 pork      (1000) pork      (1000)      396 2024-04-06 07:23:56.000000 punkweb_bb-0.2.0/punkweb_bb/templates/punkweb_bb/bbcode.html
+-rw-r--r--   0 pork      (1000) pork      (1000)     1369 2024-05-28 22:31:26.000000 punkweb_bb-0.2.0/punkweb_bb/templates/punkweb_bb/category_create.html
+-rw-r--r--   0 pork      (1000) pork      (1000)     1467 2024-05-28 19:26:46.000000 punkweb_bb-0.2.0/punkweb_bb/templates/punkweb_bb/category_update.html
+-rw-r--r--   0 pork      (1000) pork      (1000)    10032 2024-05-28 22:56:48.000000 punkweb_bb-0.2.0/punkweb_bb/templates/punkweb_bb/index.html
+-rw-r--r--   0 pork      (1000) pork      (1000)     1087 2024-04-06 02:06:29.000000 punkweb_bb-0.2.0/punkweb_bb/templates/punkweb_bb/login.html
+-rw-r--r--   0 pork      (1000) pork      (1000)     2729 2024-04-08 23:13:19.000000 punkweb_bb-0.2.0/punkweb_bb/templates/punkweb_bb/members.html
+drwxr-xr-x   0 pork      (1000) pork      (1000)        0 2024-05-28 23:00:59.976560 punkweb_bb-0.2.0/punkweb_bb/templates/punkweb_bb/partials/
+-rw-r--r--   0 pork      (1000) pork      (1000)      435 2024-05-28 20:05:18.000000 punkweb_bb-0.2.0/punkweb_bb/templates/punkweb_bb/partials/category_delete.html
+-rw-r--r--   0 pork      (1000) pork      (1000)      417 2024-04-06 02:06:29.000000 punkweb_bb-0.2.0/punkweb_bb/templates/punkweb_bb/partials/post_delete.html
+-rw-r--r--   0 pork      (1000) pork      (1000)      565 2024-04-06 02:06:29.000000 punkweb_bb-0.2.0/punkweb_bb/templates/punkweb_bb/partials/post_update.html
+-rw-r--r--   0 pork      (1000) pork      (1000)      421 2024-05-28 20:24:22.000000 punkweb_bb-0.2.0/punkweb_bb/templates/punkweb_bb/partials/shout_delete.html
+-rw-r--r--   0 pork      (1000) pork      (1000)      447 2024-05-28 20:05:14.000000 punkweb_bb-0.2.0/punkweb_bb/templates/punkweb_bb/partials/subcategory_delete.html
+-rw-r--r--   0 pork      (1000) pork      (1000)      425 2024-04-06 02:06:29.000000 punkweb_bb-0.2.0/punkweb_bb/templates/punkweb_bb/partials/thread_delete.html
+-rw-r--r--   0 pork      (1000) pork      (1000)     2948 2024-04-08 23:26:38.000000 punkweb_bb-0.2.0/punkweb_bb/templates/punkweb_bb/profile.html
+-rw-r--r--   0 pork      (1000) pork      (1000)     1994 2024-04-07 22:46:43.000000 punkweb_bb-0.2.0/punkweb_bb/templates/punkweb_bb/settings.html
+drwxr-xr-x   0 pork      (1000) pork      (1000)        0 2024-05-28 23:00:59.976560 punkweb_bb-0.2.0/punkweb_bb/templates/punkweb_bb/shoutbox/
+-rw-r--r--   0 pork      (1000) pork      (1000)      689 2024-05-28 21:28:48.000000 punkweb_bb-0.2.0/punkweb_bb/templates/punkweb_bb/shoutbox/shout_list.html
+-rw-r--r--   0 pork      (1000) pork      (1000)      672 2024-05-28 22:12:45.000000 punkweb_bb-0.2.0/punkweb_bb/templates/punkweb_bb/shoutbox/shoutbox.html
+-rw-r--r--   0 pork      (1000) pork      (1000)     1167 2024-04-06 02:06:29.000000 punkweb_bb-0.2.0/punkweb_bb/templates/punkweb_bb/signup.html
+-rw-r--r--   0 pork      (1000) pork      (1000)     5543 2024-05-28 22:58:20.000000 punkweb_bb-0.2.0/punkweb_bb/templates/punkweb_bb/subcategory.html
+-rw-r--r--   0 pork      (1000) pork      (1000)     1521 2024-05-28 22:31:18.000000 punkweb_bb-0.2.0/punkweb_bb/templates/punkweb_bb/subcategory_create.html
+-rw-r--r--   0 pork      (1000) pork      (1000)     1638 2024-05-28 19:43:47.000000 punkweb_bb-0.2.0/punkweb_bb/templates/punkweb_bb/subcategory_update.html
+-rw-r--r--   0 pork      (1000) pork      (1000)     8417 2024-05-28 22:53:06.000000 punkweb_bb-0.2.0/punkweb_bb/templates/punkweb_bb/thread.html
+-rw-r--r--   0 pork      (1000) pork      (1000)     1639 2024-05-28 22:43:05.000000 punkweb_bb-0.2.0/punkweb_bb/templates/punkweb_bb/thread_create.html
+-rw-r--r--   0 pork      (1000) pork      (1000)     1730 2024-05-07 04:35:30.000000 punkweb_bb-0.2.0/punkweb_bb/templates/punkweb_bb/thread_update.html
+drwxr-xr-x   0 pork      (1000) pork      (1000)        0 2024-05-28 23:00:59.976560 punkweb_bb-0.2.0/punkweb_bb/templatetags/
+-rw-r--r--   0 pork      (1000) pork      (1000)        0 2024-05-07 04:31:09.000000 punkweb_bb-0.2.0/punkweb_bb/templatetags/__init__.py
+drwxr-xr-x   0 pork      (1000) pork      (1000)        0 2024-05-28 23:00:59.976560 punkweb_bb-0.2.0/punkweb_bb/templatetags/__pycache__/
+-rw-r--r--   0 pork      (1000) pork      (1000)      174 2024-05-07 04:31:10.000000 punkweb_bb-0.2.0/punkweb_bb/templatetags/__pycache__/__init__.cpython-311.pyc
+-rw-r--r--   0 pork      (1000) pork      (1000)      528 2024-05-28 21:22:24.000000 punkweb_bb-0.2.0/punkweb_bb/templatetags/__pycache__/can_delete.cpython-311.pyc
+-rw-r--r--   0 pork      (1000) pork      (1000)      524 2024-05-28 21:22:32.000000 punkweb_bb-0.2.0/punkweb_bb/templatetags/__pycache__/can_edit.cpython-311.pyc
+-rw-r--r--   0 pork      (1000) pork      (1000)      524 2024-05-28 21:25:13.000000 punkweb_bb-0.2.0/punkweb_bb/templatetags/__pycache__/can_post.cpython-311.pyc
+-rw-r--r--   0 pork      (1000) pork      (1000)      621 2024-05-07 04:30:58.000000 punkweb_bb-0.2.0/punkweb_bb/templatetags/__pycache__/humanize_count.cpython-311.pyc
+-rw-r--r--   0 pork      (1000) pork      (1000)      619 2024-05-07 04:31:10.000000 punkweb_bb-0.2.0/punkweb_bb/templatetags/__pycache__/humanize_int.cpython-311.pyc
+-rw-r--r--   0 pork      (1000) pork      (1000)      833 2024-04-09 07:07:10.000000 punkweb_bb-0.2.0/punkweb_bb/templatetags/__pycache__/shoutbox_bbcode.cpython-311.pyc
+-rw-r--r--   0 pork      (1000) pork      (1000)      137 2024-05-28 21:20:55.000000 punkweb_bb-0.2.0/punkweb_bb/templatetags/can_delete.py
+-rw-r--r--   0 pork      (1000) pork      (1000)      133 2024-05-28 21:22:30.000000 punkweb_bb-0.2.0/punkweb_bb/templatetags/can_edit.py
+-rw-r--r--   0 pork      (1000) pork      (1000)      133 2024-05-28 21:24:47.000000 punkweb_bb-0.2.0/punkweb_bb/templatetags/can_post.py
+-rw-r--r--   0 pork      (1000) pork      (1000)      248 2024-05-07 04:31:08.000000 punkweb_bb-0.2.0/punkweb_bb/templatetags/humanize_int.py
+-rw-r--r--   0 pork      (1000) pork      (1000)      310 2024-04-09 07:07:08.000000 punkweb_bb-0.2.0/punkweb_bb/templatetags/shoutbox_bbcode.py
+-rw-r--r--   0 pork      (1000) pork      (1000)    26338 2024-05-28 21:35:13.000000 punkweb_bb-0.2.0/punkweb_bb/tests.py
+-rw-r--r--   0 pork      (1000) pork      (1000)     2415 2024-05-28 20:10:29.000000 punkweb_bb-0.2.0/punkweb_bb/urls.py
+-rw-r--r--   0 pork      (1000) pork      (1000)      396 2024-05-28 21:06:17.000000 punkweb_bb-0.2.0/punkweb_bb/utils.py
+-rw-r--r--   0 pork      (1000) pork      (1000)    16610 2024-05-28 22:09:44.000000 punkweb_bb-0.2.0/punkweb_bb/views.py
+-rw-r--r--   0 pork      (1000) pork      (1000)      840 2024-04-03 19:20:08.000000 punkweb_bb-0.2.0/punkweb_bb/widgets.py
+drwxr-xr-x   0 pork      (1000) pork      (1000)        0 2024-05-28 23:00:59.964560 punkweb_bb-0.2.0/punkweb_bb.egg-info/
+-rw-r--r--   0 pork      (1000) pork      (1000)     5023 2024-05-28 23:00:59.000000 punkweb_bb-0.2.0/punkweb_bb.egg-info/PKG-INFO
+-rw-r--r--   0 pork      (1000) pork      (1000)    14282 2024-05-28 23:00:59.000000 punkweb_bb-0.2.0/punkweb_bb.egg-info/SOURCES.txt
+-rw-r--r--   0 pork      (1000) pork      (1000)        1 2024-05-28 23:00:59.000000 punkweb_bb-0.2.0/punkweb_bb.egg-info/dependency_links.txt
+-rw-r--r--   0 pork      (1000) pork      (1000)        1 2024-04-09 07:09:59.000000 punkweb_bb-0.2.0/punkweb_bb.egg-info/not-zip-safe
+-rw-r--r--   0 pork      (1000) pork      (1000)       54 2024-05-28 23:00:59.000000 punkweb_bb-0.2.0/punkweb_bb.egg-info/requires.txt
+-rw-r--r--   0 pork      (1000) pork      (1000)       11 2024-05-28 23:00:59.000000 punkweb_bb-0.2.0/punkweb_bb.egg-info/top_level.txt
+-rw-r--r--   0 pork      (1000) pork      (1000)       38 2024-05-28 23:00:59.976560 punkweb_bb-0.2.0/setup.cfg
+-rw-r--r--   0 pork      (1000) pork      (1000)     1010 2024-05-28 23:00:40.000000 punkweb_bb-0.2.0/setup.py
```

### Comparing `punkweb_bb-0.1.4/LICENSE` & `punkweb_bb-0.2.0/LICENSE`

 * *Files identical despite different names*

### Comparing `punkweb_bb-0.1.4/PKG-INFO` & `punkweb_bb-0.2.0/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: punkweb_bb
-Version: 0.1.4
+Version: 0.2.0
 Summary: Django application that provides a simple and modern forum board software for your Django website.
 Home-page: https://github.com/Punkweb/PunkwebBB
 Author: Punkweb
 Author-email: punkwebnet@gmail.com
 License: BSD-3-Clause
 Classifier: Environment :: Web Environment
 Classifier: Framework :: Django
@@ -18,15 +18,15 @@
 
 # PunkwebBB
 
 PunkwebBB is a Django application that provides a simple and modern forum board software for your Django website.
 
 This is the successor to [punkweb-boards](https://github.com/Punkweb/punkweb-boards).
 
-Check out [punkweb.net](https://punkweb.net/board/) for a live demo and more information!
+Check out [punkweb.net](https://punkweb.net/board/) for documentation, support and a live demonstration of the software.
 
 ## Built with
 
 - [Django](https://www.djangoproject.com/)
 - [django-precise-bbcode](https://github.com/ellmetha/django-precise-bbcode)
 - [HTMX](https://htmx.org/)
 - [jQuery](https://jquery.com/)
```

### Comparing `punkweb_bb-0.1.4/README.md` & `punkweb_bb-0.2.0/README.md`

 * *Files 2% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 # PunkwebBB
 
 PunkwebBB is a Django application that provides a simple and modern forum board software for your Django website.
 
 This is the successor to [punkweb-boards](https://github.com/Punkweb/punkweb-boards).
 
-Check out [punkweb.net](https://punkweb.net/board/) for a live demo and more information!
+Check out [punkweb.net](https://punkweb.net/board/) for documentation, support and a live demonstration of the software.
 
 ## Built with
 
 - [Django](https://www.djangoproject.com/)
 - [django-precise-bbcode](https://github.com/ellmetha/django-precise-bbcode)
 - [HTMX](https://htmx.org/)
 - [jQuery](https://jquery.com/)
```

### Comparing `punkweb_bb-0.1.4/punkweb_bb/__pycache__/admin.cpython-311.pyc` & `punkweb_bb-0.2.0/punkweb_bb/__pycache__/admin.cpython-311.pyc`

 * *Files identical despite different names*

### Comparing `punkweb_bb-0.1.4/punkweb_bb/__pycache__/admin_forms.cpython-311.pyc` & `punkweb_bb-0.2.0/punkweb_bb/__pycache__/admin_forms.cpython-311.pyc`

 * *Files identical despite different names*

### Comparing `punkweb_bb-0.1.4/punkweb_bb/__pycache__/apps.cpython-311.pyc` & `punkweb_bb-0.2.0/punkweb_bb/__pycache__/apps.cpython-311.pyc`

 * *Files identical despite different names*

### Comparing `punkweb_bb-0.1.4/punkweb_bb/__pycache__/bbcode_tags.cpython-311.pyc` & `punkweb_bb-0.2.0/punkweb_bb/__pycache__/bbcode_tags.cpython-311.pyc`

 * *Files identical despite different names*

### Comparing `punkweb_bb-0.1.4/punkweb_bb/__pycache__/guests.cpython-311.pyc` & `punkweb_bb-0.2.0/punkweb_bb/__pycache__/guests.cpython-311.pyc`

 * *Files identical despite different names*

### Comparing `punkweb_bb-0.1.4/punkweb_bb/__pycache__/middleware.cpython-311.pyc` & `punkweb_bb-0.2.0/punkweb_bb/__pycache__/middleware.cpython-311.pyc`

 * *Files identical despite different names*

### Comparing `punkweb_bb-0.1.4/punkweb_bb/__pycache__/mixins.cpython-311.pyc` & `punkweb_bb-0.2.0/punkweb_bb/__pycache__/mixins.cpython-311.pyc`

 * *Files identical despite different names*

### Comparing `punkweb_bb-0.1.4/punkweb_bb/__pycache__/models.cpython-311.pyc` & `punkweb_bb-0.2.0/punkweb_bb/__pycache__/models.cpython-311.pyc`

 * *Files 10% similar despite different names*

#### Python bytecode

```diff
@@ -1,10 +1,10 @@
 magic:    0xa70d0d0a
-moddate:  0x11b93966 (Tue May  7 05:16:01 2024 UTC)
-files sz: 5519
+moddate:  0x89605666 (Tue May 28 22:54:01 2024 UTC)
+files sz: 6218
 code
    argcount  : 0
    nlocals   : 0
    stacksize : 6
    flags     : 0
    code
       0x9700640064016c005a00640064016c015a01640064016c025a02640064
@@ -133,39 +133,39 @@
                220 LOAD_CONST              16 ('Subcategory')
                222 LOAD_NAME               19 (UUIDPrimaryKeyMixin)
                224 LOAD_NAME               18 (TimestampMixin)
                226 PRECALL                  4
                230 CALL                     4
                240 STORE_NAME              24 (Subcategory)
    
-   101         242 PUSH_NULL
+   104         242 PUSH_NULL
                244 LOAD_BUILD_CLASS
-               246 LOAD_CONST              17 (<code object Thread, file "/home/pork/Punkweb/punkweb-bb/punkweb_bb/models.py", line 101>)
+               246 LOAD_CONST              17 (<code object Thread, file "/home/pork/Punkweb/punkweb-bb/punkweb_bb/models.py", line 104>)
                248 MAKE_FUNCTION            0
                250 LOAD_CONST              18 ('Thread')
                252 LOAD_NAME               19 (UUIDPrimaryKeyMixin)
                254 LOAD_NAME               18 (TimestampMixin)
                256 PRECALL                  4
                260 CALL                     4
                270 STORE_NAME              25 (Thread)
    
-   135         272 PUSH_NULL
+   147         272 PUSH_NULL
                274 LOAD_BUILD_CLASS
-               276 LOAD_CONST              19 (<code object Post, file "/home/pork/Punkweb/punkweb-bb/punkweb_bb/models.py", line 135>)
+               276 LOAD_CONST              19 (<code object Post, file "/home/pork/Punkweb/punkweb-bb/punkweb_bb/models.py", line 147>)
                278 MAKE_FUNCTION            0
                280 LOAD_CONST              20 ('Post')
                282 LOAD_NAME               19 (UUIDPrimaryKeyMixin)
                284 LOAD_NAME               18 (TimestampMixin)
                286 PRECALL                  4
                290 CALL                     4
                300 STORE_NAME              26 (Post)
    
-   174         302 PUSH_NULL
+   192         302 PUSH_NULL
                304 LOAD_BUILD_CLASS
-               306 LOAD_CONST              21 (<code object Shout, file "/home/pork/Punkweb/punkweb-bb/punkweb_bb/models.py", line 174>)
+               306 LOAD_CONST              21 (<code object Shout, file "/home/pork/Punkweb/punkweb-bb/punkweb_bb/models.py", line 192>)
                308 MAKE_FUNCTION            0
                310 LOAD_CONST              22 ('Shout')
                312 LOAD_NAME               19 (UUIDPrimaryKeyMixin)
                314 LOAD_NAME               18 (TimestampMixin)
                316 PRECALL                  4
                320 CALL                     4
                330 STORE_NAME              27 (Shout)
@@ -680,18 +680,18 @@
             036a060000000000000000ac02a6030000ab0300000000000000005a0702
             0065036a0800000000000000006403ac04a6010000ab0100000000000000
             005a09020065036a0a000000000000000064056406ac07a6020000ab0200
             000000000000005a0b0200650c64066406ac08a6020000ab020000000000
             0000005a0d020065036a0e00000000000000006409ac0aa6010000ab0100
             000000000000005a0f020065036a100000000000000000640bac0aa60100
             00ab0100000000000000005a1102004700640c8400640da6020000ab0200
-            000000000000005a126513640e8400a6000000ab0000000000000000005a
-            146513640f8400a6000000ab0000000000000000005a15651364108400a6
-            000000ab0000000000000000005a16641184005a17641284005a18641353
-            00
+            000000000000005a12640e84005a136514640f8400a6000000ab00000000
+            00000000005a15651464108400a6000000ab0000000000000000005a1665
+            1464118400a6000000ab0000000000000000005a17641284005a18641384
+            005a1964145300
           64           0 RESUME                   0
                        2 LOAD_NAME                0 (__name__)
                        4 STORE_NAME               1 (__module__)
                        6 LOAD_CONST               0 ('Subcategory')
                        8 STORE_NAME               2 (__qualname__)
          
           65          10 PUSH_NULL
@@ -759,53 +759,57 @@
                      226 LOAD_CONST              12 (<code object Meta, file "/home/pork/Punkweb/punkweb-bb/punkweb_bb/models.py", line 74>)
                      228 MAKE_FUNCTION            0
                      230 LOAD_CONST              13 ('Meta')
                      232 PRECALL                  2
                      236 CALL                     2
                      246 STORE_NAME              18 (Meta)
          
-          82         248 LOAD_NAME               19 (property)
+          82         248 LOAD_CONST              14 (<code object can_post, file "/home/pork/Punkweb/punkweb-bb/punkweb_bb/models.py", line 82>)
+                     250 MAKE_FUNCTION            0
+                     252 STORE_NAME              19 (can_post)
          
-          83         250 LOAD_CONST              14 (<code object thread_count, file "/home/pork/Punkweb/punkweb-bb/punkweb_bb/models.py", line 82>)
-                     252 MAKE_FUNCTION            0
+          85         254 LOAD_NAME               20 (property)
          
-          82         254 PRECALL                  0
-                     258 CALL                     0
+          86         256 LOAD_CONST              15 (<code object thread_count, file "/home/pork/Punkweb/punkweb-bb/punkweb_bb/models.py", line 85>)
+                     258 MAKE_FUNCTION            0
          
-          83         268 STORE_NAME              20 (thread_count)
+          85         260 PRECALL                  0
+                     264 CALL                     0
          
-          86         270 LOAD_NAME               19 (property)
+          86         274 STORE_NAME              21 (thread_count)
          
-          87         272 LOAD_CONST              15 (<code object post_count, file "/home/pork/Punkweb/punkweb-bb/punkweb_bb/models.py", line 86>)
-                     274 MAKE_FUNCTION            0
+          89         276 LOAD_NAME               20 (property)
          
-          86         276 PRECALL                  0
-                     280 CALL                     0
+          90         278 LOAD_CONST              16 (<code object post_count, file "/home/pork/Punkweb/punkweb-bb/punkweb_bb/models.py", line 89>)
+                     280 MAKE_FUNCTION            0
          
-          87         290 STORE_NAME              21 (post_count)
+          89         282 PRECALL                  0
+                     286 CALL                     0
          
-          90         292 LOAD_NAME               19 (property)
+          90         296 STORE_NAME              22 (post_count)
          
-          91         294 LOAD_CONST              16 (<code object latest_thread, file "/home/pork/Punkweb/punkweb-bb/punkweb_bb/models.py", line 90>)
-                     296 MAKE_FUNCTION            0
+          93         298 LOAD_NAME               20 (property)
          
-          90         298 PRECALL                  0
-                     302 CALL                     0
+          94         300 LOAD_CONST              17 (<code object latest_thread, file "/home/pork/Punkweb/punkweb-bb/punkweb_bb/models.py", line 93>)
+                     302 MAKE_FUNCTION            0
          
-          91         312 STORE_NAME              22 (latest_thread)
+          93         304 PRECALL                  0
+                     308 CALL                     0
          
-          94         314 LOAD_CONST              17 (<code object __str__, file "/home/pork/Punkweb/punkweb-bb/punkweb_bb/models.py", line 94>)
-                     316 MAKE_FUNCTION            0
-                     318 STORE_NAME              23 (__str__)
+          94         318 STORE_NAME              23 (latest_thread)
          
-          97         320 LOAD_CONST              18 (<code object get_absolute_url, file "/home/pork/Punkweb/punkweb-bb/punkweb_bb/models.py", line 97>)
+          97         320 LOAD_CONST              18 (<code object __str__, file "/home/pork/Punkweb/punkweb-bb/punkweb_bb/models.py", line 97>)
                      322 MAKE_FUNCTION            0
-                     324 STORE_NAME              24 (get_absolute_url)
-                     326 LOAD_CONST              19 (None)
-                     328 RETURN_VALUE
+                     324 STORE_NAME              24 (__str__)
+         
+         100         326 LOAD_CONST              19 (<code object get_absolute_url, file "/home/pork/Punkweb/punkweb-bb/punkweb_bb/models.py", line 100>)
+                     328 MAKE_FUNCTION            0
+                     330 STORE_NAME              25 (get_absolute_url)
+                     332 LOAD_CONST              20 (None)
+                     334 RETURN_VALUE
          consts
             'Subcategory'
             'subcategories'
             ('related_name', 'on_delete')
             255
             ('max_length',)
             1024
@@ -849,53 +853,80 @@
                cellvars   ()
                filename   '/home/pork/Punkweb/punkweb-bb/punkweb_bb/models.py'
                name       'Meta'
                firstlineno 74
                lnotab 0x0a0104010401
             'Meta'
             code
+               argcount  : 2
+               nlocals   : 2
+               stacksize : 1
+               flags     : 3
+               code
+                  0x97007c006a0000000000000000000c0070067c016a0100000000000000
+                  005300
+                82           0 RESUME                   0
+               
+                83           2 LOAD_FAST                0 (self)
+                             4 LOAD_ATTR                0 (staff_post_only)
+                            14 UNARY_NOT
+                            16 JUMP_IF_TRUE_OR_POP      6 (to 30)
+                            18 LOAD_FAST                1 (user)
+                            20 LOAD_ATTR                1 (is_staff)
+                       >>   30 RETURN_VALUE
+               consts
+                  None
+               names      ('staff_post_only', 'is_staff')
+               varnames   ('self', 'user')
+               freevars   ()
+               cellvars   ()
+               filename   '/home/pork/Punkweb/punkweb-bb/punkweb_bb/models.py'
+               name       'can_post'
+               firstlineno 82
+               lnotab 0x0201
+            code
                argcount  : 1
                nlocals   : 1
                stacksize : 2
                flags     : 3
                code
                   0x97007c006a000000000000000000a00100000000000000000000000000
                   00000000000000a6000000ab0000000000000000005300
-                82           0 RESUME                   0
+                85           0 RESUME                   0
                
-                84           2 LOAD_FAST                0 (self)
+                87           2 LOAD_FAST                0 (self)
                              4 LOAD_ATTR                0 (threads)
                             14 LOAD_METHOD              1 (count)
                             36 PRECALL                  0
                             40 CALL                     0
                             50 RETURN_VALUE
                consts
                   None
                names      ('threads', 'count')
                varnames   ('self',)
                freevars   ()
                cellvars   ()
                filename   '/home/pork/Punkweb/punkweb-bb/punkweb_bb/models.py'
                name       'thread_count'
-               firstlineno 82
+               firstlineno 85
                lnotab 0x0202
             code
                argcount  : 1
                nlocals   : 1
                stacksize : 5
                flags     : 3
                code
                   0x9700740100000000000000000000640184007c006a0100000000000000
                   00a0020000000000000000000000000000000000000000a6000000ab0000
                   000000000000004400a6000000ab000000000000000000a6010000ab0100
                   000000000000005300
-                86           0 RESUME                   0
+                89           0 RESUME                   0
                
-                88           2 LOAD_GLOBAL              1 (NULL + sum)
-                            14 LOAD_CONST               1 (<code object <listcomp>, file "/home/pork/Punkweb/punkweb-bb/punkweb_bb/models.py", line 88>)
+                91           2 LOAD_GLOBAL              1 (NULL + sum)
+                            14 LOAD_CONST               1 (<code object <listcomp>, file "/home/pork/Punkweb/punkweb-bb/punkweb_bb/models.py", line 91>)
                             16 MAKE_FUNCTION            0
                             18 LOAD_FAST                0 (self)
                             20 LOAD_ATTR                1 (threads)
                             30 LOAD_METHOD              2 (all)
                             52 PRECALL                  0
                             56 CALL                     0
                             66 GET_ITER
@@ -908,15 +939,15 @@
                   None
                   code
                      argcount  : 1
                      nlocals   : 2
                      stacksize : 3
                      flags     : 19
                      code 0x970067007c005d097d017c016a00000000000000000091028c0a5300
-                      88           0 RESUME                   0
+                      91           0 RESUME                   0
                                    2 BUILD_LIST               0
                                    4 LOAD_FAST                0 (.0)
                              >>    6 FOR_ITER                 9 (to 26)
                                    8 STORE_FAST               1 (thread)
                                   10 LOAD_FAST                1 (thread)
                                   12 LOAD_ATTR                0 (post_count)
                                   22 LIST_APPEND              2
@@ -925,37 +956,37 @@
                      consts
                      names      ('post_count',)
                      varnames   ('.0', 'thread')
                      freevars   ()
                      cellvars   ()
                      filename   '/home/pork/Punkweb/punkweb-bb/punkweb_bb/models.py'
                      name       '<listcomp>'
-                     firstlineno 88
+                     firstlineno 91
                      lnotab 0x
                names      ('sum', 'threads', 'all')
                varnames   ('self',)
                freevars   ()
                cellvars   ()
                filename   '/home/pork/Punkweb/punkweb-bb/punkweb_bb/models.py'
                name       'post_count'
-               firstlineno 86
+               firstlineno 89
                lnotab 0x0202
             code
                argcount  : 1
                nlocals   : 1
                stacksize : 3
                flags     : 3
                code
                   0x97007c006a000000000000000000a00100000000000000000000000000
                   000000000000006401a6010000ab010000000000000000a0020000000000
                   000000000000000000000000000000a6000000ab00000000000000000053
                   00
-                90           0 RESUME                   0
+                93           0 RESUME                   0
                
-                92           2 LOAD_FAST                0 (self)
+                95           2 LOAD_FAST                0 (self)
                              4 LOAD_ATTR                0 (threads)
                             14 LOAD_METHOD              1 (order_by)
                             36 LOAD_CONST               1 ('-last_post_created_at')
                             38 PRECALL                  1
                             42 CALL                     1
                             52 LOAD_METHOD              2 (first)
                             74 PRECALL                  0
@@ -966,27 +997,27 @@
                   '-last_post_created_at'
                names      ('threads', 'order_by', 'first')
                varnames   ('self',)
                freevars   ()
                cellvars   ()
                filename   '/home/pork/Punkweb/punkweb-bb/punkweb_bb/models.py'
                name       'latest_thread'
-               firstlineno 90
+               firstlineno 93
                lnotab 0x0202
             code
                argcount  : 1
                nlocals   : 1
                stacksize : 5
                flags     : 3
                code
                   0x97007c006a0000000000000000009b0064017c006a0100000000000000
                   009b0064027c006a0200000000000000009b009d055300
-                94           0 RESUME                   0
+                97           0 RESUME                   0
                
-                95           2 LOAD_FAST                0 (self)
+                98           2 LOAD_FAST                0 (self)
                              4 LOAD_ATTR                0 (category)
                             14 FORMAT_VALUE             0
                             16 LOAD_CONST               1 (' > ')
                             18 LOAD_FAST                0 (self)
                             20 LOAD_ATTR                1 (order)
                             30 FORMAT_VALUE             0
                             32 LOAD_CONST               2 ('. ')
@@ -1001,27 +1032,27 @@
                   '. '
                names      ('category', 'order', 'name')
                varnames   ('self',)
                freevars   ()
                cellvars   ()
                filename   '/home/pork/Punkweb/punkweb-bb/punkweb_bb/models.py'
                name       '__str__'
-               firstlineno 94
+               firstlineno 97
                lnotab 0x0201
             code
                argcount  : 1
                nlocals   : 1
                stacksize : 4
                flags     : 3
                code
                   0x970074010000000000000000000064017c006a01000000000000000067
                   01ac02a6020000ab0200000000000000005300
-                97           0 RESUME                   0
+               100           0 RESUME                   0
                
-                98           2 LOAD_GLOBAL              1 (NULL + reverse)
+               101           2 LOAD_GLOBAL              1 (NULL + reverse)
                             14 LOAD_CONST               1 ('punkweb_bb:subcategory')
                             16 LOAD_FAST                0 (self)
                             18 LOAD_ATTR                1 (slug)
                             28 BUILD_LIST               1
                             30 KW_NAMES                 2
                             32 PRECALL                  2
                             36 CALL                     2
@@ -1032,27 +1063,27 @@
                   ('args',)
                names      ('reverse', 'slug')
                varnames   ('self',)
                freevars   ()
                cellvars   ()
                filename   '/home/pork/Punkweb/punkweb-bb/punkweb_bb/models.py'
                name       'get_absolute_url'
-               firstlineno 97
+               firstlineno 100
                lnotab 0x0201
             None
-         names      ('__name__', '__module__', '__qualname__', 'models', 'ForeignKey', 'Category', 'CASCADE', 'category', 'CharField', 'name', 'SlugField', 'slug', 'BBCodeTextField', 'description', 'PositiveIntegerField', 'order', 'BooleanField', 'staff_post_only', 'Meta', 'property', 'thread_count', 'post_count', 'latest_thread', '__str__', 'get_absolute_url')
+         names      ('__name__', '__module__', '__qualname__', 'models', 'ForeignKey', 'Category', 'CASCADE', 'category', 'CharField', 'name', 'SlugField', 'slug', 'BBCodeTextField', 'description', 'PositiveIntegerField', 'order', 'BooleanField', 'staff_post_only', 'Meta', 'can_post', 'property', 'thread_count', 'post_count', 'latest_thread', '__str__', 'get_absolute_url')
          varnames   ()
          freevars   ()
          cellvars   ()
          filename   '/home/pork/Punkweb/punkweb-bb/punkweb_bb/models.py'
          name       'Subcategory'
          firstlineno 64
          lnotab
-            0x0a010e0110ff1203220124011a01220122021a08020104ff0e01020302
-            0104ff0e010203020104ff0e0102030603
+            0x0a010e0110ff1203220124011a01220122021a080603020104ff0e0102
+            03020104ff0e010203020104ff0e0102030603
       'Subcategory'
       code
          argcount  : 0
          nlocals   : 0
          stacksize : 5
          flags     : 0
          code
@@ -1062,138 +1093,151 @@
             02a6030000ab0300000000000000005a09020065036a0a00000000000000
             006403ac04a6010000ab0100000000000000005a0b0200650ca6000000ab
             0000000000000000005a0d020065036a0e00000000000000006405ac06a6
             010000ab0100000000000000005a0f020065036a0e000000000000000064
             05ac06a6010000ab0100000000000000005a10020065036a110000000000
             0000006407ac08a6010000ab0100000000000000005a12020065036a1300
             000000000000006409ac06a6010000ab0100000000000000005a14020047
-            00640a8400640ba6020000ab0200000000000000005a15640c84005a1665
-            17640d8400a6000000ab0000000000000000005a186517640e8400a60000
-            00ab0000000000000000005a19640f84005a1a64105300
-         101           0 RESUME                   0
+            00640a8400640ba6020000ab0200000000000000005a15640c84005a1664
+            0d84005a17640e84005a18640f84005a19651a64108400a6000000ab0000
+            000000000000005a1b651a64118400a6000000ab0000000000000000005a
+            1c641284005a1d64135300
+         104           0 RESUME                   0
                        2 LOAD_NAME                0 (__name__)
                        4 STORE_NAME               1 (__module__)
                        6 LOAD_CONST               0 ('Thread')
                        8 STORE_NAME               2 (__qualname__)
          
-         102          10 PUSH_NULL
+         105          10 PUSH_NULL
                       12 LOAD_NAME                3 (models)
                       14 LOAD_ATTR                4 (ForeignKey)
          
-         103          24 LOAD_NAME                5 (Subcategory)
+         106          24 LOAD_NAME                5 (Subcategory)
                       26 LOAD_CONST               1 ('threads')
                       28 LOAD_NAME                3 (models)
                       30 LOAD_ATTR                6 (CASCADE)
          
-         102          40 KW_NAMES                 2
+         105          40 KW_NAMES                 2
                       42 PRECALL                  3
                       46 CALL                     3
                       56 STORE_NAME               7 (subcategory)
          
-         105          58 PUSH_NULL
+         108          58 PUSH_NULL
                       60 LOAD_NAME                3 (models)
                       62 LOAD_ATTR                4 (ForeignKey)
                       72 LOAD_NAME                8 (User)
                       74 LOAD_CONST               1 ('threads')
                       76 LOAD_NAME                3 (models)
                       78 LOAD_ATTR                6 (CASCADE)
                       88 KW_NAMES                 2
                       90 PRECALL                  3
                       94 CALL                     3
                      104 STORE_NAME               9 (user)
          
-         106         106 PUSH_NULL
+         109         106 PUSH_NULL
                      108 LOAD_NAME                3 (models)
                      110 LOAD_ATTR               10 (CharField)
                      120 LOAD_CONST               3 (255)
                      122 KW_NAMES                 4
                      124 PRECALL                  1
                      128 CALL                     1
                      138 STORE_NAME              11 (title)
          
-         107         140 PUSH_NULL
+         110         140 PUSH_NULL
                      142 LOAD_NAME               12 (BBCodeTextField)
                      144 PRECALL                  0
                      148 CALL                     0
                      158 STORE_NAME              13 (content)
          
-         108         160 PUSH_NULL
+         111         160 PUSH_NULL
                      162 LOAD_NAME                3 (models)
                      164 LOAD_ATTR               14 (BooleanField)
                      174 LOAD_CONST               5 (False)
                      176 KW_NAMES                 6
                      178 PRECALL                  1
                      182 CALL                     1
                      192 STORE_NAME              15 (is_pinned)
          
-         109         194 PUSH_NULL
+         112         194 PUSH_NULL
                      196 LOAD_NAME                3 (models)
                      198 LOAD_ATTR               14 (BooleanField)
                      208 LOAD_CONST               5 (False)
                      210 KW_NAMES                 6
                      212 PRECALL                  1
                      216 CALL                     1
                      226 STORE_NAME              16 (is_closed)
          
-         110         228 PUSH_NULL
+         113         228 PUSH_NULL
                      230 LOAD_NAME                3 (models)
                      232 LOAD_ATTR               17 (DateTimeField)
                      242 LOAD_CONST               7 (True)
                      244 KW_NAMES                 8
                      246 PRECALL                  1
                      250 CALL                     1
                      260 STORE_NAME              18 (last_post_created_at)
          
-         111         262 PUSH_NULL
+         114         262 PUSH_NULL
                      264 LOAD_NAME                3 (models)
                      266 LOAD_ATTR               19 (PositiveIntegerField)
                      276 LOAD_CONST               9 (0)
                      278 KW_NAMES                 6
                      280 PRECALL                  1
                      284 CALL                     1
                      294 STORE_NAME              20 (view_count)
          
-         113         296 PUSH_NULL
+         116         296 PUSH_NULL
                      298 LOAD_BUILD_CLASS
-                     300 LOAD_CONST              10 (<code object Meta, file "/home/pork/Punkweb/punkweb-bb/punkweb_bb/models.py", line 113>)
+                     300 LOAD_CONST              10 (<code object Meta, file "/home/pork/Punkweb/punkweb-bb/punkweb_bb/models.py", line 116>)
                      302 MAKE_FUNCTION            0
                      304 LOAD_CONST              11 ('Meta')
                      306 PRECALL                  2
                      310 CALL                     2
                      320 STORE_NAME              21 (Meta)
          
-         120         322 LOAD_CONST              12 (<code object __str__, file "/home/pork/Punkweb/punkweb-bb/punkweb_bb/models.py", line 120>)
+         123         322 LOAD_CONST              12 (<code object __str__, file "/home/pork/Punkweb/punkweb-bb/punkweb_bb/models.py", line 123>)
                      324 MAKE_FUNCTION            0
                      326 STORE_NAME              22 (__str__)
          
-         123         328 LOAD_NAME               23 (property)
+         126         328 LOAD_CONST              13 (<code object can_edit, file "/home/pork/Punkweb/punkweb-bb/punkweb_bb/models.py", line 126>)
+                     330 MAKE_FUNCTION            0
+                     332 STORE_NAME              23 (can_edit)
+         
+         129         334 LOAD_CONST              14 (<code object can_delete, file "/home/pork/Punkweb/punkweb-bb/punkweb_bb/models.py", line 129>)
+                     336 MAKE_FUNCTION            0
+                     338 STORE_NAME              24 (can_delete)
          
-         124         330 LOAD_CONST              13 (<code object post_count, file "/home/pork/Punkweb/punkweb-bb/punkweb_bb/models.py", line 123>)
-                     332 MAKE_FUNCTION            0
+         132         340 LOAD_CONST              15 (<code object can_post, file "/home/pork/Punkweb/punkweb-bb/punkweb_bb/models.py", line 132>)
+                     342 MAKE_FUNCTION            0
+                     344 STORE_NAME              25 (can_post)
          
-         123         334 PRECALL                  0
-                     338 CALL                     0
+         135         346 LOAD_NAME               26 (property)
          
-         124         348 STORE_NAME              24 (post_count)
+         136         348 LOAD_CONST              16 (<code object post_count, file "/home/pork/Punkweb/punkweb-bb/punkweb_bb/models.py", line 135>)
+                     350 MAKE_FUNCTION            0
          
-         127         350 LOAD_NAME               23 (property)
+         135         352 PRECALL                  0
+                     356 CALL                     0
          
-         128         352 LOAD_CONST              14 (<code object latest_post, file "/home/pork/Punkweb/punkweb-bb/punkweb_bb/models.py", line 127>)
-                     354 MAKE_FUNCTION            0
+         136         366 STORE_NAME              27 (post_count)
          
-         127         356 PRECALL                  0
-                     360 CALL                     0
+         139         368 LOAD_NAME               26 (property)
          
-         128         370 STORE_NAME              25 (latest_post)
+         140         370 LOAD_CONST              17 (<code object latest_post, file "/home/pork/Punkweb/punkweb-bb/punkweb_bb/models.py", line 139>)
+                     372 MAKE_FUNCTION            0
          
-         131         372 LOAD_CONST              15 (<code object get_absolute_url, file "/home/pork/Punkweb/punkweb-bb/punkweb_bb/models.py", line 131>)
-                     374 MAKE_FUNCTION            0
-                     376 STORE_NAME              26 (get_absolute_url)
-                     378 LOAD_CONST              16 (None)
-                     380 RETURN_VALUE
+         139         374 PRECALL                  0
+                     378 CALL                     0
+         
+         140         388 STORE_NAME              28 (latest_post)
+         
+         143         390 LOAD_CONST              18 (<code object get_absolute_url, file "/home/pork/Punkweb/punkweb-bb/punkweb_bb/models.py", line 143>)
+                     392 MAKE_FUNCTION            0
+                     394 STORE_NAME              29 (get_absolute_url)
+                     396 LOAD_CONST              19 (None)
+                     398 RETURN_VALUE
          consts
             'Thread'
             'threads'
             ('related_name', 'on_delete')
             255
             ('max_length',)
             False
@@ -1203,98 +1247,186 @@
             0
             code
                argcount  : 0
                nlocals   : 0
                stacksize : 1
                flags     : 0
                code 0x970065005a0164005a0264015a0364025300
-               113           0 RESUME                   0
+               116           0 RESUME                   0
                              2 LOAD_NAME                0 (__name__)
                              4 STORE_NAME               1 (__module__)
                              6 LOAD_CONST               0 ('Thread.Meta')
                              8 STORE_NAME               2 (__qualname__)
                
-               114          10 LOAD_CONST               1 (('subcategory', '-is_pinned', '-last_post_created_at'))
+               117          10 LOAD_CONST               1 (('subcategory', '-is_pinned', '-last_post_created_at'))
                             12 STORE_NAME               3 (ordering)
                             14 LOAD_CONST               2 (None)
                             16 RETURN_VALUE
                consts
                   'Thread.Meta'
                   ('subcategory', '-is_pinned', '-last_post_created_at')
                   None
                names      ('__name__', '__module__', '__qualname__', 'ordering')
                varnames   ()
                freevars   ()
                cellvars   ()
                filename   '/home/pork/Punkweb/punkweb-bb/punkweb_bb/models.py'
                name       'Meta'
-               firstlineno 113
+               firstlineno 116
                lnotab 0x0a01
             'Meta'
             code
                argcount  : 1
                nlocals   : 1
                stacksize : 1
                flags     : 3
                code 0x97007c006a0000000000000000009b005300
-               120           0 RESUME                   0
+               123           0 RESUME                   0
                
-               121           2 LOAD_FAST                0 (self)
+               124           2 LOAD_FAST                0 (self)
                              4 LOAD_ATTR                0 (title)
                             14 FORMAT_VALUE             0
                             16 RETURN_VALUE
                consts
                   None
                names      ('title',)
                varnames   ('self',)
                freevars   ()
                cellvars   ()
                filename   '/home/pork/Punkweb/punkweb-bb/punkweb_bb/models.py'
                name       '__str__'
-               firstlineno 120
+               firstlineno 123
+               lnotab 0x0201
+            code
+               argcount  : 2
+               nlocals   : 2
+               stacksize : 3
+               flags     : 3
+               code
+                  0x97007c017c006a0000000000000000006b020000000070147c01a00100
+                  000000000000000000000000000000000000006401a6010000ab01000000
+                  00000000005300
+               126           0 RESUME                   0
+               
+               127           2 LOAD_FAST                1 (user)
+                             4 LOAD_FAST                0 (self)
+                             6 LOAD_ATTR                0 (user)
+                            16 COMPARE_OP               2 (==)
+                            22 JUMP_IF_TRUE_OR_POP     20 (to 64)
+                            24 LOAD_FAST                1 (user)
+                            26 LOAD_METHOD              1 (has_perm)
+                            48 LOAD_CONST               1 ('punkweb_bb.change_thread')
+                            50 PRECALL                  1
+                            54 CALL                     1
+                       >>   64 RETURN_VALUE
+               consts
+                  None
+                  'punkweb_bb.change_thread'
+               names      ('user', 'has_perm')
+               varnames   ('self', 'user')
+               freevars   ()
+               cellvars   ()
+               filename   '/home/pork/Punkweb/punkweb-bb/punkweb_bb/models.py'
+               name       'can_edit'
+               firstlineno 126
+               lnotab 0x0201
+            code
+               argcount  : 2
+               nlocals   : 2
+               stacksize : 3
+               flags     : 3
+               code
+                  0x97007c017c006a0000000000000000006b020000000070147c01a00100
+                  000000000000000000000000000000000000006401a6010000ab01000000
+                  00000000005300
+               129           0 RESUME                   0
+               
+               130           2 LOAD_FAST                1 (user)
+                             4 LOAD_FAST                0 (self)
+                             6 LOAD_ATTR                0 (user)
+                            16 COMPARE_OP               2 (==)
+                            22 JUMP_IF_TRUE_OR_POP     20 (to 64)
+                            24 LOAD_FAST                1 (user)
+                            26 LOAD_METHOD              1 (has_perm)
+                            48 LOAD_CONST               1 ('punkweb_bb.delete_thread')
+                            50 PRECALL                  1
+                            54 CALL                     1
+                       >>   64 RETURN_VALUE
+               consts
+                  None
+                  'punkweb_bb.delete_thread'
+               names      ('user', 'has_perm')
+               varnames   ('self', 'user')
+               freevars   ()
+               cellvars   ()
+               filename   '/home/pork/Punkweb/punkweb-bb/punkweb_bb/models.py'
+               name       'can_delete'
+               firstlineno 129
+               lnotab 0x0201
+            code
+               argcount  : 2
+               nlocals   : 2
+               stacksize : 1
+               flags     : 3
+               code 0x97007c006a0000000000000000000c005300
+               132           0 RESUME                   0
+               
+               133           2 LOAD_FAST                0 (self)
+                             4 LOAD_ATTR                0 (is_closed)
+                            14 UNARY_NOT
+                            16 RETURN_VALUE
+               consts
+                  None
+               names      ('is_closed',)
+               varnames   ('self', 'user')
+               freevars   ()
+               cellvars   ()
+               filename   '/home/pork/Punkweb/punkweb-bb/punkweb_bb/models.py'
+               name       'can_post'
+               firstlineno 132
                lnotab 0x0201
             code
                argcount  : 1
                nlocals   : 1
                stacksize : 2
                flags     : 3
                code
                   0x97007c006a000000000000000000a00100000000000000000000000000
                   00000000000000a6000000ab0000000000000000005300
-               123           0 RESUME                   0
+               135           0 RESUME                   0
                
-               125           2 LOAD_FAST                0 (self)
+               137           2 LOAD_FAST                0 (self)
                              4 LOAD_ATTR                0 (posts)
                             14 LOAD_METHOD              1 (count)
                             36 PRECALL                  0
                             40 CALL                     0
                             50 RETURN_VALUE
                consts
                   None
                names      ('posts', 'count')
                varnames   ('self',)
                freevars   ()
                cellvars   ()
                filename   '/home/pork/Punkweb/punkweb-bb/punkweb_bb/models.py'
                name       'post_count'
-               firstlineno 123
+               firstlineno 135
                lnotab 0x0202
             code
                argcount  : 1
                nlocals   : 1
                stacksize : 3
                flags     : 3
                code
                   0x97007c006a000000000000000000a00100000000000000000000000000
                   000000000000006401a6010000ab010000000000000000a0020000000000
                   000000000000000000000000000000a6000000ab00000000000000000053
                   00
-               127           0 RESUME                   0
+               139           0 RESUME                   0
                
-               129           2 LOAD_FAST                0 (self)
+               141           2 LOAD_FAST                0 (self)
                              4 LOAD_ATTR                0 (posts)
                             14 LOAD_METHOD              1 (order_by)
                             36 LOAD_CONST               1 ('-created_at')
                             38 PRECALL                  1
                             42 CALL                     1
                             52 LOAD_METHOD              2 (first)
                             74 PRECALL                  0
@@ -1305,27 +1437,27 @@
                   '-created_at'
                names      ('posts', 'order_by', 'first')
                varnames   ('self',)
                freevars   ()
                cellvars   ()
                filename   '/home/pork/Punkweb/punkweb-bb/punkweb_bb/models.py'
                name       'latest_post'
-               firstlineno 127
+               firstlineno 139
                lnotab 0x0202
             code
                argcount  : 1
                nlocals   : 1
                stacksize : 4
                flags     : 3
                code
                   0x970074010000000000000000000064017c006a01000000000000000067
                   01ac02a6020000ab0200000000000000005300
-               131           0 RESUME                   0
+               143           0 RESUME                   0
                
-               132           2 LOAD_GLOBAL              1 (NULL + reverse)
+               144           2 LOAD_GLOBAL              1 (NULL + reverse)
                             14 LOAD_CONST               1 ('punkweb_bb:thread')
                             16 LOAD_FAST                0 (self)
                             18 LOAD_ATTR                1 (id)
                             28 BUILD_LIST               1
                             30 KW_NAMES                 2
                             32 PRECALL                  2
                             36 CALL                     2
@@ -1336,170 +1468,179 @@
                   ('args',)
                names      ('reverse', 'id')
                varnames   ('self',)
                freevars   ()
                cellvars   ()
                filename   '/home/pork/Punkweb/punkweb-bb/punkweb_bb/models.py'
                name       'get_absolute_url'
-               firstlineno 131
+               firstlineno 143
                lnotab 0x0201
             None
-         names      ('__name__', '__module__', '__qualname__', 'models', 'ForeignKey', 'Subcategory', 'CASCADE', 'subcategory', 'User', 'user', 'CharField', 'title', 'BBCodeTextField', 'content', 'BooleanField', 'is_pinned', 'is_closed', 'DateTimeField', 'last_post_created_at', 'PositiveIntegerField', 'view_count', 'Meta', '__str__', 'property', 'post_count', 'latest_post', 'get_absolute_url')
+         names      ('__name__', '__module__', '__qualname__', 'models', 'ForeignKey', 'Subcategory', 'CASCADE', 'subcategory', 'User', 'user', 'CharField', 'title', 'BBCodeTextField', 'content', 'BooleanField', 'is_pinned', 'is_closed', 'DateTimeField', 'last_post_created_at', 'PositiveIntegerField', 'view_count', 'Meta', '__str__', 'can_edit', 'can_delete', 'can_post', 'property', 'post_count', 'latest_post', 'get_absolute_url')
          varnames   ()
          freevars   ()
          cellvars   ()
          filename   '/home/pork/Punkweb/punkweb-bb/punkweb_bb/models.py'
          name       'Thread'
-         firstlineno 101
+         firstlineno 104
          lnotab
-            0x0a010e0110ff120330012201140122012201220122021a070603020104
-            ff0e010203020104ff0e010203
+            0x0a010e0110ff120330012201140122012201220122021a070603060306
+            030603020104ff0e010203020104ff0e010203
       'Thread'
       code
          argcount  : 0
          nlocals   : 0
          stacksize : 5
          flags     : 0
          code
             0x8700970065005a0164005a02020065036a040000000000000000650564
             0165036a060000000000000000ac02a6030000ab0300000000000000005a
             07020065036a0400000000000000006508640165036a0600000000000000
             00ac02a6030000ab0300000000000000005a090200650aa6000000ab0000
             000000000000005a0b02004700640384006404a6020000ab020000000000
-            0000005a0c640584005a0d650e64068400a6000000ab0000000000000000
-            005a0f650e64078400a6000000ab0000000000000000005a10640884005a
-            1188006601640984085a12880078015a135300
+            0000005a0c640584005a0d640684005a0e640784005a0f651064088400a6
+            000000ab0000000000000000005a11651064098400a6000000ab00000000
+            00000000005a12640a84005a1388006601640b84085a14880078015a1553
+            00
                        0 MAKE_CELL                0 (__class__)
          
-         135           2 RESUME                   0
+         147           2 RESUME                   0
                        4 LOAD_NAME                0 (__name__)
                        6 STORE_NAME               1 (__module__)
                        8 LOAD_CONST               0 ('Post')
                       10 STORE_NAME               2 (__qualname__)
          
-         136          12 PUSH_NULL
+         148          12 PUSH_NULL
                       14 LOAD_NAME                3 (models)
                       16 LOAD_ATTR                4 (ForeignKey)
                       26 LOAD_NAME                5 (Thread)
                       28 LOAD_CONST               1 ('posts')
                       30 LOAD_NAME                3 (models)
                       32 LOAD_ATTR                6 (CASCADE)
                       42 KW_NAMES                 2
                       44 PRECALL                  3
                       48 CALL                     3
                       58 STORE_NAME               7 (thread)
          
-         137          60 PUSH_NULL
+         149          60 PUSH_NULL
                       62 LOAD_NAME                3 (models)
                       64 LOAD_ATTR                4 (ForeignKey)
                       74 LOAD_NAME                8 (User)
                       76 LOAD_CONST               1 ('posts')
                       78 LOAD_NAME                3 (models)
                       80 LOAD_ATTR                6 (CASCADE)
                       90 KW_NAMES                 2
                       92 PRECALL                  3
                       96 CALL                     3
                      106 STORE_NAME               9 (user)
          
-         138         108 PUSH_NULL
+         150         108 PUSH_NULL
                      110 LOAD_NAME               10 (BBCodeTextField)
                      112 PRECALL                  0
                      116 CALL                     0
                      126 STORE_NAME              11 (content)
          
-         140         128 PUSH_NULL
+         152         128 PUSH_NULL
                      130 LOAD_BUILD_CLASS
-                     132 LOAD_CONST               3 (<code object Meta, file "/home/pork/Punkweb/punkweb-bb/punkweb_bb/models.py", line 140>)
+                     132 LOAD_CONST               3 (<code object Meta, file "/home/pork/Punkweb/punkweb-bb/punkweb_bb/models.py", line 152>)
                      134 MAKE_FUNCTION            0
                      136 LOAD_CONST               4 ('Meta')
                      138 PRECALL                  2
                      142 CALL                     2
                      152 STORE_NAME              12 (Meta)
          
-         143         154 LOAD_CONST               5 (<code object __str__, file "/home/pork/Punkweb/punkweb-bb/punkweb_bb/models.py", line 143>)
+         155         154 LOAD_CONST               5 (<code object __str__, file "/home/pork/Punkweb/punkweb-bb/punkweb_bb/models.py", line 155>)
                      156 MAKE_FUNCTION            0
                      158 STORE_NAME              13 (__str__)
          
-         146         160 LOAD_NAME               14 (property)
+         158         160 LOAD_CONST               6 (<code object can_edit, file "/home/pork/Punkweb/punkweb-bb/punkweb_bb/models.py", line 158>)
+                     162 MAKE_FUNCTION            0
+                     164 STORE_NAME              14 (can_edit)
          
-         147         162 LOAD_CONST               6 (<code object index, file "/home/pork/Punkweb/punkweb-bb/punkweb_bb/models.py", line 146>)
-                     164 MAKE_FUNCTION            0
+         161         166 LOAD_CONST               7 (<code object can_delete, file "/home/pork/Punkweb/punkweb-bb/punkweb_bb/models.py", line 161>)
+                     168 MAKE_FUNCTION            0
+                     170 STORE_NAME              15 (can_delete)
          
-         146         166 PRECALL                  0
-                     170 CALL                     0
+         164         172 LOAD_NAME               16 (property)
          
-         147         180 STORE_NAME              15 (index)
-         
-         154         182 LOAD_NAME               14 (property)
+         165         174 LOAD_CONST               8 (<code object index, file "/home/pork/Punkweb/punkweb-bb/punkweb_bb/models.py", line 164>)
+                     176 MAKE_FUNCTION            0
          
-         155         184 LOAD_CONST               7 (<code object page_number, file "/home/pork/Punkweb/punkweb-bb/punkweb_bb/models.py", line 154>)
-                     186 MAKE_FUNCTION            0
+         164         178 PRECALL                  0
+                     182 CALL                     0
          
-         154         188 PRECALL                  0
-                     192 CALL                     0
+         165         192 STORE_NAME              17 (index)
          
-         155         202 STORE_NAME              16 (page_number)
+         172         194 LOAD_NAME               16 (property)
          
-         158         204 LOAD_CONST               8 (<code object get_absolute_url, file "/home/pork/Punkweb/punkweb-bb/punkweb_bb/models.py", line 158>)
-                     206 MAKE_FUNCTION            0
-                     208 STORE_NAME              17 (get_absolute_url)
+         173         196 LOAD_CONST               9 (<code object page_number, file "/home/pork/Punkweb/punkweb-bb/punkweb_bb/models.py", line 172>)
+                     198 MAKE_FUNCTION            0
          
-         165         210 LOAD_CLOSURE             0 (__class__)
-                     212 BUILD_TUPLE              1
-                     214 LOAD_CONST               9 (<code object save, file "/home/pork/Punkweb/punkweb-bb/punkweb_bb/models.py", line 165>)
-                     216 MAKE_FUNCTION            8 (closure)
-                     218 STORE_NAME              18 (save)
-                     220 LOAD_CLOSURE             0 (__class__)
-                     222 COPY                     1
-                     224 STORE_NAME              19 (__classcell__)
-                     226 RETURN_VALUE
+         172         200 PRECALL                  0
+                     204 CALL                     0
+         
+         173         214 STORE_NAME              18 (page_number)
+         
+         176         216 LOAD_CONST              10 (<code object get_absolute_url, file "/home/pork/Punkweb/punkweb-bb/punkweb_bb/models.py", line 176>)
+                     218 MAKE_FUNCTION            0
+                     220 STORE_NAME              19 (get_absolute_url)
+         
+         183         222 LOAD_CLOSURE             0 (__class__)
+                     224 BUILD_TUPLE              1
+                     226 LOAD_CONST              11 (<code object save, file "/home/pork/Punkweb/punkweb-bb/punkweb_bb/models.py", line 183>)
+                     228 MAKE_FUNCTION            8 (closure)
+                     230 STORE_NAME              20 (save)
+                     232 LOAD_CLOSURE             0 (__class__)
+                     234 COPY                     1
+                     236 STORE_NAME              21 (__classcell__)
+                     238 RETURN_VALUE
          consts
             'Post'
             'posts'
             ('related_name', 'on_delete')
             code
                argcount  : 0
                nlocals   : 0
                stacksize : 1
                flags     : 0
                code 0x970065005a0164005a0264015a0364025300
-               140           0 RESUME                   0
+               152           0 RESUME                   0
                              2 LOAD_NAME                0 (__name__)
                              4 STORE_NAME               1 (__module__)
                              6 LOAD_CONST               0 ('Post.Meta')
                              8 STORE_NAME               2 (__qualname__)
                
-               141          10 LOAD_CONST               1 (('created_at',))
+               153          10 LOAD_CONST               1 (('created_at',))
                             12 STORE_NAME               3 (ordering)
                             14 LOAD_CONST               2 (None)
                             16 RETURN_VALUE
                consts
                   'Post.Meta'
                   ('created_at',)
                   None
                names      ('__name__', '__module__', '__qualname__', 'ordering')
                varnames   ()
                freevars   ()
                cellvars   ()
                filename   '/home/pork/Punkweb/punkweb-bb/punkweb_bb/models.py'
                name       'Meta'
-               firstlineno 140
+               firstlineno 152
                lnotab 0x0a01
             'Meta'
             code
                argcount  : 1
                nlocals   : 1
                stacksize : 5
                flags     : 3
                code
                   0x97007c006a0000000000000000009b0064017c006a0100000000000000
                   009b0064017c006a0200000000000000009b009d055300
-               143           0 RESUME                   0
+               155           0 RESUME                   0
                
-               144           2 LOAD_FAST                0 (self)
+               156           2 LOAD_FAST                0 (self)
                              4 LOAD_ATTR                0 (thread)
                             14 FORMAT_VALUE             0
                             16 LOAD_CONST               1 (' > ')
                             18 LOAD_FAST                0 (self)
                             20 LOAD_ATTR                1 (user)
                             30 FORMAT_VALUE             0
                             32 LOAD_CONST               1 (' > ')
@@ -1513,41 +1654,107 @@
                   ' > '
                names      ('thread', 'user', 'created_at')
                varnames   ('self',)
                freevars   ()
                cellvars   ()
                filename   '/home/pork/Punkweb/punkweb-bb/punkweb_bb/models.py'
                name       '__str__'
-               firstlineno 143
+               firstlineno 155
+               lnotab 0x0201
+            code
+               argcount  : 2
+               nlocals   : 2
+               stacksize : 3
+               flags     : 3
+               code
+                  0x97007c017c006a0000000000000000006b020000000070147c01a00100
+                  000000000000000000000000000000000000006401a6010000ab01000000
+                  00000000005300
+               158           0 RESUME                   0
+               
+               159           2 LOAD_FAST                1 (user)
+                             4 LOAD_FAST                0 (self)
+                             6 LOAD_ATTR                0 (user)
+                            16 COMPARE_OP               2 (==)
+                            22 JUMP_IF_TRUE_OR_POP     20 (to 64)
+                            24 LOAD_FAST                1 (user)
+                            26 LOAD_METHOD              1 (has_perm)
+                            48 LOAD_CONST               1 ('punkweb_bb.change_post')
+                            50 PRECALL                  1
+                            54 CALL                     1
+                       >>   64 RETURN_VALUE
+               consts
+                  None
+                  'punkweb_bb.change_post'
+               names      ('user', 'has_perm')
+               varnames   ('self', 'user')
+               freevars   ()
+               cellvars   ()
+               filename   '/home/pork/Punkweb/punkweb-bb/punkweb_bb/models.py'
+               name       'can_edit'
+               firstlineno 158
+               lnotab 0x0201
+            code
+               argcount  : 2
+               nlocals   : 2
+               stacksize : 3
+               flags     : 3
+               code
+                  0x97007c017c006a0000000000000000006b020000000070147c01a00100
+                  000000000000000000000000000000000000006401a6010000ab01000000
+                  00000000005300
+               161           0 RESUME                   0
+               
+               162           2 LOAD_FAST                1 (user)
+                             4 LOAD_FAST                0 (self)
+                             6 LOAD_ATTR                0 (user)
+                            16 COMPARE_OP               2 (==)
+                            22 JUMP_IF_TRUE_OR_POP     20 (to 64)
+                            24 LOAD_FAST                1 (user)
+                            26 LOAD_METHOD              1 (has_perm)
+                            48 LOAD_CONST               1 ('punkweb_bb.delete_post')
+                            50 PRECALL                  1
+                            54 CALL                     1
+                       >>   64 RETURN_VALUE
+               consts
+                  None
+                  'punkweb_bb.delete_post'
+               names      ('user', 'has_perm')
+               varnames   ('self', 'user')
+               freevars   ()
+               cellvars   ()
+               filename   '/home/pork/Punkweb/punkweb-bb/punkweb_bb/models.py'
+               name       'can_delete'
+               firstlineno 161
                lnotab 0x0201
             code
                argcount  : 1
                nlocals   : 3
                stacksize : 6
                flags     : 3
                code
                   0x97007c006a0000000000000000006a010000000000000000a002000000
                   00000000000000000000000000000000006401a6010000ab010000000000
                   0000007d017407000000000000000000007c01a004000000000000000000
                   000000000000000000000064026403ac04a6020000ab0200000000000000
                   00a6010000ab010000000000000000a00500000000000000000000000000
                   000000000000007c006a060000000000000000a6010000ab010000000000
                   0000007d027c0264057a0000005300
-               146           0 RESUME                   0
+               164           0 RESUME                   0
                
-               150           2 LOAD_FAST                0 (self)
+               168           2 LOAD_FAST                0 (self)
                              4 LOAD_ATTR                0 (thread)
                             14 LOAD_ATTR                1 (posts)
                             24 LOAD_METHOD              2 (order_by)
                             46 LOAD_CONST               1 ('created_at')
                             48 PRECALL                  1
                             52 CALL                     1
                             62 STORE_FAST               1 (qs)
                
-               151          64 LOAD_GLOBAL              7 (NULL + list)
+               169          64 LOAD_GLOBAL              7 (NULL + list)
                             76 LOAD_FAST                1 (qs)
                             78 LOAD_METHOD              4 (values_list)
                            100 LOAD_CONST               2 ('id')
                            102 LOAD_CONST               3 (True)
                            104 KW_NAMES                 4
                            106 PRECALL                  2
                            110 CALL                     2
@@ -1556,15 +1763,15 @@
                            134 LOAD_METHOD              5 (index)
                            156 LOAD_FAST                0 (self)
                            158 LOAD_ATTR                6 (id)
                            168 PRECALL                  1
                            172 CALL                     1
                            182 STORE_FAST               2 (index)
                
-               152         184 LOAD_FAST                2 (index)
+               170         184 LOAD_FAST                2 (index)
                            186 LOAD_CONST               5 (1)
                            188 BINARY_OP                0 (+)
                            192 RETURN_VALUE
                consts
                   None
                   'created_at'
                   'id'
@@ -1573,27 +1780,27 @@
                   1
                names      ('thread', 'posts', 'order_by', 'list', 'values_list', 'index', 'id')
                varnames   ('self', 'qs', 'index')
                freevars   ()
                cellvars   ()
                filename   '/home/pork/Punkweb/punkweb-bb/punkweb_bb/models.py'
                name       'index'
-               firstlineno 146
+               firstlineno 164
                lnotab 0x02043e017801
             code
                argcount  : 1
                nlocals   : 1
                stacksize : 4
                flags     : 3
                code
                   0x97007401000000000000000000006a0100000000000000007c006a0200
                   0000000000000064017a0b0000a6010000ab0100000000000000005300
-               154           0 RESUME                   0
+               172           0 RESUME                   0
                
-               156           2 LOAD_GLOBAL              1 (NULL + math)
+               174           2 LOAD_GLOBAL              1 (NULL + math)
                             14 LOAD_ATTR                1 (ceil)
                             24 LOAD_FAST                0 (self)
                             26 LOAD_ATTR                2 (index)
                             36 LOAD_CONST               1 (10)
                             38 BINARY_OP               11 (/)
                             42 PRECALL                  1
                             46 CALL                     1
@@ -1603,67 +1810,67 @@
                   10
                names      ('math', 'ceil', 'index')
                varnames   ('self',)
                freevars   ()
                cellvars   ()
                filename   '/home/pork/Punkweb/punkweb-bb/punkweb_bb/models.py'
                name       'page_number'
-               firstlineno 154
+               firstlineno 172
                lnotab 0x0202
             code
                argcount  : 1
                nlocals   : 2
                stacksize : 5
                flags     : 3
                code
                   0x970074010000000000000000000064017c006a0100000000000000006a
                   0200000000000000006701ac02a6020000ab0200000000000000007d017c
                   0164037c006a0300000000000000009b0064047c006a0200000000000000
                   009b009d047a0d00007d017c015300
-               158           0 RESUME                   0
+               176           0 RESUME                   0
                
-               159           2 LOAD_GLOBAL              1 (NULL + reverse)
+               177           2 LOAD_GLOBAL              1 (NULL + reverse)
                             14 LOAD_CONST               1 ('punkweb_bb:thread')
                             16 LOAD_FAST                0 (self)
                             18 LOAD_ATTR                1 (thread)
                             28 LOAD_ATTR                2 (id)
                             38 BUILD_LIST               1
                             40 KW_NAMES                 2
                             42 PRECALL                  2
                             46 CALL                     2
                             56 STORE_FAST               1 (thread_url)
                
-               161          58 LOAD_FAST                1 (thread_url)
+               179          58 LOAD_FAST                1 (thread_url)
                             60 LOAD_CONST               3 ('?page=')
                             62 LOAD_FAST                0 (self)
                             64 LOAD_ATTR                3 (page_number)
                             74 FORMAT_VALUE             0
                             76 LOAD_CONST               4 ('#post-')
                             78 LOAD_FAST                0 (self)
                             80 LOAD_ATTR                2 (id)
                             90 FORMAT_VALUE             0
                             92 BUILD_STRING             4
                             94 BINARY_OP               13 (+=)
                             98 STORE_FAST               1 (thread_url)
                
-               163         100 LOAD_FAST                1 (thread_url)
+               181         100 LOAD_FAST                1 (thread_url)
                            102 RETURN_VALUE
                consts
                   None
                   'punkweb_bb:thread'
                   ('args',)
                   '?page='
                   '#post-'
                names      ('reverse', 'thread', 'id', 'page_number')
                varnames   ('self', 'thread_url')
                freevars   ()
                cellvars   ()
                filename   '/home/pork/Punkweb/punkweb-bb/punkweb_bb/models.py'
                name       'get_absolute_url'
-               firstlineno 158
+               firstlineno 176
                lnotab 0x020138022a02
             code
                argcount  : 1
                nlocals   : 3
                stacksize : 5
                flags     : 15
                code
@@ -1674,48 +1881,48 @@
                   006a0000000000000000005f0700000000000000007c006a000000000000
                   000000a0080000000000000000000000000000000000000000a6000000ab
                   00000000000000000001000200741300000000000000000000a6000000ab
                   0000000000000000006a0800000000000000007c0169007c02a4018e0101
                   0064005300
                              0 COPY_FREE_VARS           1
                
-               165           2 RESUME                   0
+               183           2 RESUME                   0
                
-               166           4 LOAD_FAST                0 (self)
+               184           4 LOAD_FAST                0 (self)
                              6 LOAD_ATTR                0 (thread)
                             16 LOAD_ATTR                1 (is_closed)
                             26 POP_JUMP_FORWARD_IF_FALSE    15 (to 58)
                
-               167          28 LOAD_GLOBAL              5 (NULL + ValidationError)
+               185          28 LOAD_GLOBAL              5 (NULL + ValidationError)
                             40 LOAD_CONST               1 ('Cannot add posts to a closed thread.')
                             42 PRECALL                  1
                             46 CALL                     1
                             56 RAISE_VARARGS            1
                
-               168     >>   58 LOAD_FAST                0 (self)
+               186     >>   58 LOAD_FAST                0 (self)
                             60 LOAD_ATTR                3 (_state)
                             70 LOAD_ATTR                4 (adding)
                             80 POP_JUMP_FORWARD_IF_FALSE    54 (to 190)
                
-               169          82 LOAD_GLOBAL             11 (NULL + timezone)
+               187          82 LOAD_GLOBAL             11 (NULL + timezone)
                             94 LOAD_ATTR                6 (now)
                            104 PRECALL                  0
                            108 CALL                     0
                            118 LOAD_FAST                0 (self)
                            120 LOAD_ATTR                0 (thread)
                            130 STORE_ATTR               7 (last_post_created_at)
                
-               170         140 LOAD_FAST                0 (self)
+               188         140 LOAD_FAST                0 (self)
                            142 LOAD_ATTR                0 (thread)
                            152 LOAD_METHOD              8 (save)
                            174 PRECALL                  0
                            178 CALL                     0
                            188 POP_TOP
                
-               171     >>  190 PUSH_NULL
+               189     >>  190 PUSH_NULL
                            192 LOAD_GLOBAL             19 (NULL + super)
                            204 PRECALL                  0
                            208 CALL                     0
                            218 LOAD_ATTR                8 (save)
                            228 LOAD_FAST                1 (args)
                            230 BUILD_MAP                0
                            232 LOAD_FAST                2 (kwargs)
@@ -1729,121 +1936,125 @@
                   'Cannot add posts to a closed thread.'
                names      ('thread', 'is_closed', 'ValidationError', '_state', 'adding', 'timezone', 'now', 'last_post_created_at', 'save', 'super')
                varnames   ('self', 'args', 'kwargs')
                freevars   ('__class__',)
                cellvars   ()
                filename   '/home/pork/Punkweb/punkweb-bb/punkweb_bb/models.py'
                name       'save'
-               firstlineno 165
+               firstlineno 183
                lnotab 0x040118011e0118013a013201
-         names      ('__name__', '__module__', '__qualname__', 'models', 'ForeignKey', 'Thread', 'CASCADE', 'thread', 'User', 'user', 'BBCodeTextField', 'content', 'Meta', '__str__', 'property', 'index', 'page_number', 'get_absolute_url', 'save', '__classcell__')
+         names      ('__name__', '__module__', '__qualname__', 'models', 'ForeignKey', 'Thread', 'CASCADE', 'thread', 'User', 'user', 'BBCodeTextField', 'content', 'Meta', '__str__', 'can_edit', 'can_delete', 'property', 'index', 'page_number', 'get_absolute_url', 'save', '__classcell__')
          varnames   ()
          freevars   ()
          cellvars   ('__class__',)
          filename   '/home/pork/Punkweb/punkweb-bb/punkweb_bb/models.py'
          name       'Post'
-         firstlineno 135
+         firstlineno 147
          lnotab
-            0x0c013001300114021a030603020104ff0e010207020104ff0e01020306
-            07
+            0x0c013001300114021a03060306030603020104ff0e010207020104ff0e
+            0102030607
       'Post'
       code
          argcount  : 0
          nlocals   : 0
          stacksize : 5
          flags     : 0
          code
             0x970065005a0164005a02020065036a0400000000000000006505640165
             036a060000000000000000ac02a6030000ab0300000000000000005a0702
             0065036a080000000000000000a6000000ab0000000000000000005a0902
             004700640384006404a6020000ab0200000000000000005a0a640584005a
-            0b64065300
-         174           0 RESUME                   0
+            0b640684005a0c64075300
+         192           0 RESUME                   0
                        2 LOAD_NAME                0 (__name__)
                        4 STORE_NAME               1 (__module__)
                        6 LOAD_CONST               0 ('Shout')
                        8 STORE_NAME               2 (__qualname__)
          
-         175          10 PUSH_NULL
+         193          10 PUSH_NULL
                       12 LOAD_NAME                3 (models)
                       14 LOAD_ATTR                4 (ForeignKey)
                       24 LOAD_NAME                5 (User)
                       26 LOAD_CONST               1 ('shouts')
                       28 LOAD_NAME                3 (models)
                       30 LOAD_ATTR                6 (CASCADE)
                       40 KW_NAMES                 2
                       42 PRECALL                  3
                       46 CALL                     3
                       56 STORE_NAME               7 (user)
          
-         176          58 PUSH_NULL
+         194          58 PUSH_NULL
                       60 LOAD_NAME                3 (models)
                       62 LOAD_ATTR                8 (TextField)
                       72 PRECALL                  0
                       76 CALL                     0
                       86 STORE_NAME               9 (content)
          
-         178          88 PUSH_NULL
+         196          88 PUSH_NULL
                       90 LOAD_BUILD_CLASS
-                      92 LOAD_CONST               3 (<code object Meta, file "/home/pork/Punkweb/punkweb-bb/punkweb_bb/models.py", line 178>)
+                      92 LOAD_CONST               3 (<code object Meta, file "/home/pork/Punkweb/punkweb-bb/punkweb_bb/models.py", line 196>)
                       94 MAKE_FUNCTION            0
                       96 LOAD_CONST               4 ('Meta')
                       98 PRECALL                  2
                      102 CALL                     2
                      112 STORE_NAME              10 (Meta)
          
-         181         114 LOAD_CONST               5 (<code object __str__, file "/home/pork/Punkweb/punkweb-bb/punkweb_bb/models.py", line 181>)
+         199         114 LOAD_CONST               5 (<code object __str__, file "/home/pork/Punkweb/punkweb-bb/punkweb_bb/models.py", line 199>)
                      116 MAKE_FUNCTION            0
                      118 STORE_NAME              11 (__str__)
-                     120 LOAD_CONST               6 (None)
-                     122 RETURN_VALUE
+         
+         202         120 LOAD_CONST               6 (<code object can_delete, file "/home/pork/Punkweb/punkweb-bb/punkweb_bb/models.py", line 202>)
+                     122 MAKE_FUNCTION            0
+                     124 STORE_NAME              12 (can_delete)
+                     126 LOAD_CONST               7 (None)
+                     128 RETURN_VALUE
          consts
             'Shout'
             'shouts'
             ('related_name', 'on_delete')
             code
                argcount  : 0
                nlocals   : 0
                stacksize : 1
                flags     : 0
                code 0x970065005a0164005a0264015a0364025300
-               178           0 RESUME                   0
+               196           0 RESUME                   0
                              2 LOAD_NAME                0 (__name__)
                              4 STORE_NAME               1 (__module__)
                              6 LOAD_CONST               0 ('Shout.Meta')
                              8 STORE_NAME               2 (__qualname__)
                
-               179          10 LOAD_CONST               1 (('-created_at',))
+               197          10 LOAD_CONST               1 (('-created_at',))
                             12 STORE_NAME               3 (ordering)
                             14 LOAD_CONST               2 (None)
                             16 RETURN_VALUE
                consts
                   'Shout.Meta'
                   ('-created_at',)
                   None
                names      ('__name__', '__module__', '__qualname__', 'ordering')
                varnames   ()
                freevars   ()
                cellvars   ()
                filename   '/home/pork/Punkweb/punkweb-bb/punkweb_bb/models.py'
                name       'Meta'
-               firstlineno 178
+               firstlineno 196
                lnotab 0x0a01
             'Meta'
             code
                argcount  : 1
                nlocals   : 1
                stacksize : 3
                flags     : 3
                code
                   0x97007c006a0000000000000000009b0064017c006a0100000000000000
                   009b009d035300
-               181           0 RESUME                   0
+               199           0 RESUME                   0
                
-               182           2 LOAD_FAST                0 (self)
+               200           2 LOAD_FAST                0 (self)
                              4 LOAD_ATTR                0 (user)
                             14 FORMAT_VALUE             0
                             16 LOAD_CONST               1 (' > ')
                             18 LOAD_FAST                0 (self)
                             20 LOAD_ATTR                1 (created_at)
                             30 FORMAT_VALUE             0
                             32 BUILD_STRING             3
@@ -1853,29 +2064,62 @@
                   ' > '
                names      ('user', 'created_at')
                varnames   ('self',)
                freevars   ()
                cellvars   ()
                filename   '/home/pork/Punkweb/punkweb-bb/punkweb_bb/models.py'
                name       '__str__'
-               firstlineno 181
+               firstlineno 199
+               lnotab 0x0201
+            code
+               argcount  : 2
+               nlocals   : 2
+               stacksize : 3
+               flags     : 3
+               code
+                  0x97007c017c006a0000000000000000006b020000000070147c01a00100
+                  000000000000000000000000000000000000006401a6010000ab01000000
+                  00000000005300
+               202           0 RESUME                   0
+               
+               203           2 LOAD_FAST                1 (user)
+                             4 LOAD_FAST                0 (self)
+                             6 LOAD_ATTR                0 (user)
+                            16 COMPARE_OP               2 (==)
+                            22 JUMP_IF_TRUE_OR_POP     20 (to 64)
+                            24 LOAD_FAST                1 (user)
+                            26 LOAD_METHOD              1 (has_perm)
+                            48 LOAD_CONST               1 ('punkweb_bb.delete_shout')
+                            50 PRECALL                  1
+                            54 CALL                     1
+                       >>   64 RETURN_VALUE
+               consts
+                  None
+                  'punkweb_bb.delete_shout'
+               names      ('user', 'has_perm')
+               varnames   ('self', 'user')
+               freevars   ()
+               cellvars   ()
+               filename   '/home/pork/Punkweb/punkweb-bb/punkweb_bb/models.py'
+               name       'can_delete'
+               firstlineno 202
                lnotab 0x0201
             None
-         names      ('__name__', '__module__', '__qualname__', 'models', 'ForeignKey', 'User', 'CASCADE', 'user', 'TextField', 'content', 'Meta', '__str__')
+         names      ('__name__', '__module__', '__qualname__', 'models', 'ForeignKey', 'User', 'CASCADE', 'user', 'TextField', 'content', 'Meta', '__str__', 'can_delete')
          varnames   ()
          freevars   ()
          cellvars   ()
          filename   '/home/pork/Punkweb/punkweb-bb/punkweb_bb/models.py'
          name       'Shout'
-         firstlineno 174
-         lnotab 0x0a0130011e021a03
+         firstlineno 192
+         lnotab 0x0a0130011e021a030603
       'Shout'
    names      ('datetime', 'math', 'os', 'django.contrib.auth', 'get_user_model', 'django.core.cache', 'cache', 'django.db', 'models', 'django.forms', 'ValidationError', 'django.urls', 'reverse', 'django.utils', 'timezone', 'precise_bbcode.fields', 'BBCodeTextField', 'punkweb_bb.mixins', 'TimestampMixin', 'UUIDPrimaryKeyMixin', 'User', 'profile_image_upload_to', 'BoardProfile', 'Category', 'Subcategory', 'Thread', 'Post', 'Shout')
    varnames   ()
    freevars   ()
    cellvars   ()
    filename   '/home/pork/Punkweb/punkweb-bb/punkweb_bb/models.py'
    name       '<module>'
    firstlineno 1
    lnotab
       0x00ff02010801080108020c010c010c010c010c010c010c021002140306
-      051e171e121e251e221e27
+      051e171e121e281e2b1e2d
```

### Comparing `punkweb_bb-0.1.4/punkweb_bb/__pycache__/pagination.cpython-311.pyc` & `punkweb_bb-0.2.0/punkweb_bb/__pycache__/pagination.cpython-311.pyc`

 * *Files identical despite different names*

### Comparing `punkweb_bb-0.1.4/punkweb_bb/__pycache__/parsers.cpython-311.pyc` & `punkweb_bb-0.2.0/punkweb_bb/__pycache__/parsers.cpython-311.pyc`

 * *Files identical despite different names*

### Comparing `punkweb_bb-0.1.4/punkweb_bb/__pycache__/settings.cpython-311.pyc` & `punkweb_bb-0.2.0/punkweb_bb/__pycache__/settings.cpython-311.pyc`

 * *Files identical despite different names*

### Comparing `punkweb_bb-0.1.4/punkweb_bb/__pycache__/signals.cpython-311.pyc` & `punkweb_bb-0.2.0/punkweb_bb/__pycache__/signals.cpython-311.pyc`

 * *Files identical despite different names*

### Comparing `punkweb_bb-0.1.4/punkweb_bb/__pycache__/tests.cpython-311.pyc` & `punkweb_bb-0.2.0/punkweb_bb/__pycache__/tests.cpython-311.pyc`

 * *Files 1% similar despite different names*

#### Python bytecode

```diff
@@ -1,10 +1,10 @@
 magic:    0xa70d0d0a
-moddate:  0x2b653c66 (Thu May  9 05:54:51 2024 UTC)
-files sz: 26368
+moddate:  0x114e5666 (Tue May 28 21:35:13 2024 UTC)
+files sz: 26338
 code
    argcount  : 0
    nlocals   : 0
    stacksize : 5
    flags     : 0
    code
       0x9700640064016c005a00640064026c016d025a020100640064036c036d
@@ -4544,25 +4544,24 @@
                firstlineno 451
                lnotab
                   0x02013e013e02360222010c02020102fe040402fa12093c025001640140
                   01
             code
                argcount  : 1
                nlocals   : 2
-               stacksize : 5
+               stacksize : 4
                flags     : 3
                code
                   0x97007c006a000000000000000000a00100000000000000000000000000
                   000000000000007c006a020000000000000000a6010000ab010000000000
                   00000001007c006a000000000000000000a0030000000000000000000000
                   0000000000000000007c006a040000000000000000a6010000ab01000000
                   00000000007d017c00a00500000000000000000000000000000000000000
-                  007c017c006a060000000000000000a00700000000000000000000000000
-                  00000000000000a6000000ab000000000000000000a6020000ab02000000
-                  0000000000010064005300
+                  007c016a0600000000000000006401a6020000ab02000000000000000001
+                  0064005300
                473           0 RESUME                   0
                
                474           2 LOAD_FAST                0 (self)
                              4 LOAD_ATTR                0 (client)
                             14 LOAD_METHOD              1 (force_login)
                             36 LOAD_FAST                0 (self)
                             38 LOAD_ATTR                2 (user)
@@ -4576,29 +4575,27 @@
                             98 LOAD_FAST                0 (self)
                            100 LOAD_ATTR                4 (staff_only_url)
                            110 PRECALL                  1
                            114 CALL                     1
                            124 STORE_FAST               1 (response)
                
                477         126 LOAD_FAST                0 (self)
-                           128 LOAD_METHOD              5 (assertRedirects)
+                           128 LOAD_METHOD              5 (assertEqual)
                            150 LOAD_FAST                1 (response)
-                           152 LOAD_FAST                0 (self)
-                           154 LOAD_ATTR                6 (staff_subcategory)
-                           164 LOAD_METHOD              7 (get_absolute_url)
-                           186 PRECALL                  0
-                           190 CALL                     0
-                           200 PRECALL                  2
-                           204 CALL                     2
-                           214 POP_TOP
-                           216 LOAD_CONST               0 (None)
-                           218 RETURN_VALUE
+                           152 LOAD_ATTR                6 (status_code)
+                           162 LOAD_CONST               1 (403)
+                           164 PRECALL                  2
+                           168 CALL                     2
+                           178 POP_TOP
+                           180 LOAD_CONST               0 (None)
+                           182 RETURN_VALUE
                consts
                   None
-               names      ('client', 'force_login', 'user', 'get', 'staff_only_url', 'assertRedirects', 'staff_subcategory', 'get_absolute_url')
+                  403
+               names      ('client', 'force_login', 'user', 'get', 'staff_only_url', 'assertEqual', 'status_code')
                varnames   ('self', 'response')
                freevars   ()
                cellvars   ()
                filename   '/home/pork/Punkweb/punkweb-bb/punkweb_bb/tests.py'
                name       'test_thread_create_staff_post_only'
                firstlineno 473
                lnotab 0x02013e013e02
@@ -5082,15 +5079,15 @@
                            114 CALL                     1
                            124 STORE_FAST               1 (response)
                
                525         126 LOAD_FAST                0 (self)
                            128 LOAD_METHOD              5 (assertEqual)
                            150 LOAD_FAST                1 (response)
                            152 LOAD_ATTR                6 (status_code)
-                           162 LOAD_CONST               1 (404)
+                           162 LOAD_CONST               1 (403)
                            164 PRECALL                  2
                            168 CALL                     2
                            178 POP_TOP
                
                527         180 LOAD_FAST                0 (self)
                            182 LOAD_ATTR                0 (client)
                            192 LOAD_METHOD              1 (force_login)
@@ -5117,15 +5114,15 @@
                            342 PRECALL                  2
                            346 CALL                     2
                            356 POP_TOP
                            358 LOAD_CONST               0 (None)
                            360 RETURN_VALUE
                consts
                   None
-                  404
+                  403
                   200
                names      ('client', 'force_login', 'other_user', 'get', 'url', 'assertEqual', 'status_code', 'user')
                varnames   ('self', 'response')
                freevars   ()
                cellvars   ()
                filename   '/home/pork/Punkweb/punkweb-bb/punkweb_bb/tests.py'
                name       'test_is_author'
@@ -5522,15 +5519,15 @@
                            114 CALL                     1
                            124 STORE_FAST               1 (response)
                
                574         126 LOAD_FAST                0 (self)
                            128 LOAD_METHOD              5 (assertEqual)
                            150 LOAD_FAST                1 (response)
                            152 LOAD_ATTR                6 (status_code)
-                           162 LOAD_CONST               1 (404)
+                           162 LOAD_CONST               1 (403)
                            164 PRECALL                  2
                            168 CALL                     2
                            178 POP_TOP
                
                576         180 LOAD_FAST                0 (self)
                            182 LOAD_ATTR                0 (client)
                            192 LOAD_METHOD              1 (force_login)
@@ -5557,15 +5554,15 @@
                            342 PRECALL                  2
                            346 CALL                     2
                            356 POP_TOP
                            358 LOAD_CONST               0 (None)
                            360 RETURN_VALUE
                consts
                   None
-                  404
+                  403
                   200
                names      ('client', 'force_login', 'other_user', 'get', 'url', 'assertEqual', 'status_code', 'user')
                varnames   ('self', 'response')
                freevars   ()
                cellvars   ()
                filename   '/home/pork/Punkweb/punkweb-bb/punkweb_bb/tests.py'
                name       'test_is_author'
@@ -6283,15 +6280,15 @@
                            114 CALL                     1
                            124 STORE_FAST               1 (response)
                
                656         126 LOAD_FAST                0 (self)
                            128 LOAD_METHOD              5 (assertEqual)
                            150 LOAD_FAST                1 (response)
                            152 LOAD_ATTR                6 (status_code)
-                           162 LOAD_CONST               1 (404)
+                           162 LOAD_CONST               1 (403)
                            164 PRECALL                  2
                            168 CALL                     2
                            178 POP_TOP
                
                658         180 LOAD_FAST                0 (self)
                            182 LOAD_ATTR                0 (client)
                            192 LOAD_METHOD              1 (force_login)
@@ -6318,15 +6315,15 @@
                            342 PRECALL                  2
                            346 CALL                     2
                            356 POP_TOP
                            358 LOAD_CONST               0 (None)
                            360 RETURN_VALUE
                consts
                   None
-                  404
+                  403
                   200
                names      ('client', 'force_login', 'other_user', 'get', 'url', 'assertEqual', 'status_code', 'user')
                varnames   ('self', 'response')
                freevars   ()
                cellvars   ()
                filename   '/home/pork/Punkweb/punkweb-bb/punkweb_bb/tests.py'
                name       'test_is_author'
@@ -6729,15 +6726,15 @@
                            114 CALL                     1
                            124 STORE_FAST               1 (response)
                
                706         126 LOAD_FAST                0 (self)
                            128 LOAD_METHOD              5 (assertEqual)
                            150 LOAD_FAST                1 (response)
                            152 LOAD_ATTR                6 (status_code)
-                           162 LOAD_CONST               1 (404)
+                           162 LOAD_CONST               1 (403)
                            164 PRECALL                  2
                            168 CALL                     2
                            178 POP_TOP
                
                708         180 LOAD_FAST                0 (self)
                            182 LOAD_ATTR                0 (client)
                            192 LOAD_METHOD              1 (force_login)
@@ -6764,15 +6761,15 @@
                            342 PRECALL                  2
                            346 CALL                     2
                            356 POP_TOP
                            358 LOAD_CONST               0 (None)
                            360 RETURN_VALUE
                consts
                   None
-                  404
+                  403
                   200
                names      ('client', 'force_login', 'other_user', 'get', 'url', 'assertEqual', 'status_code', 'user')
                varnames   ('self', 'response')
                freevars   ()
                cellvars   ()
                filename   '/home/pork/Punkweb/punkweb-bb/punkweb_bb/tests.py'
                name       'test_is_author'
```

### Comparing `punkweb_bb-0.1.4/punkweb_bb/__pycache__/widgets.cpython-311.pyc` & `punkweb_bb-0.2.0/punkweb_bb/__pycache__/widgets.cpython-311.pyc`

 * *Files identical despite different names*

### Comparing `punkweb_bb-0.1.4/punkweb_bb/admin.py` & `punkweb_bb-0.2.0/punkweb_bb/admin.py`

 * *Files identical despite different names*

### Comparing `punkweb_bb-0.1.4/punkweb_bb/admin_forms.py` & `punkweb_bb-0.2.0/punkweb_bb/admin_forms.py`

 * *Files identical despite different names*

### Comparing `punkweb_bb-0.1.4/punkweb_bb/bbcode_tags.py` & `punkweb_bb-0.2.0/punkweb_bb/bbcode_tags.py`

 * *Files identical despite different names*

### Comparing `punkweb_bb-0.1.4/punkweb_bb/middleware.py` & `punkweb_bb-0.2.0/punkweb_bb/middleware.py`

 * *Files identical despite different names*

### Comparing `punkweb_bb-0.1.4/punkweb_bb/migrations/0001_initial.py` & `punkweb_bb-0.2.0/punkweb_bb/migrations/0001_initial.py`

 * *Files identical despite different names*

### Comparing `punkweb_bb-0.1.4/punkweb_bb/migrations/__pycache__/0001_initial.cpython-311.pyc` & `punkweb_bb-0.2.0/punkweb_bb/migrations/__pycache__/0001_initial.cpython-311.pyc`

 * *Files identical despite different names*

### Comparing `punkweb_bb-0.1.4/punkweb_bb/migrations/__pycache__/0002_thread_view_count.cpython-311.pyc` & `punkweb_bb-0.2.0/punkweb_bb/migrations/__pycache__/0002_thread_view_count.cpython-311.pyc`

 * *Files identical despite different names*

### Comparing `punkweb_bb-0.1.4/punkweb_bb/models.py` & `punkweb_bb-0.2.0/punkweb_bb/models.py`

 * *Files 11% similar despite different names*

```diff
@@ -75,14 +75,17 @@
         verbose_name = "subcategory"
         verbose_name_plural = "subcategories"
         ordering = (
             "category__order",
             "order",
         )
 
+    def can_post(self, user):
+        return not self.staff_post_only or user.is_staff
+
     @property
     def thread_count(self):
         return self.threads.count()
 
     @property
     def post_count(self):
         return sum([thread.post_count for thread in self.threads.all()])
@@ -116,14 +119,23 @@
             "-is_pinned",
             "-last_post_created_at",
         )
 
     def __str__(self):
         return f"{self.title}"
 
+    def can_edit(self, user):
+        return user == self.user or user.has_perm("punkweb_bb.change_thread")
+
+    def can_delete(self, user):
+        return user == self.user or user.has_perm("punkweb_bb.delete_thread")
+
+    def can_post(self, user):
+        return not self.is_closed
+
     @property
     def post_count(self):
         return self.posts.count()
 
     @property
     def latest_post(self):
         return self.posts.order_by("-created_at").first()
@@ -139,14 +151,20 @@
 
     class Meta:
         ordering = ("created_at",)
 
     def __str__(self):
         return f"{self.thread} > {self.user} > {self.created_at}"
 
+    def can_edit(self, user):
+        return user == self.user or user.has_perm("punkweb_bb.change_post")
+
+    def can_delete(self, user):
+        return user == self.user or user.has_perm("punkweb_bb.delete_post")
+
     @property
     def index(self):
         # Returns the index of the post in the thread, starting with 1
 
         qs = self.thread.posts.order_by("created_at")
         index = list(qs.values_list("id", flat=True)).index(self.id)
         return index + 1
@@ -176,7 +194,10 @@
     content = models.TextField()
 
     class Meta:
         ordering = ("-created_at",)
 
     def __str__(self):
         return f"{self.user} > {self.created_at}"
+
+    def can_delete(self, user):
+        return user == self.user or user.has_perm("punkweb_bb.delete_shout")
```

### Comparing `punkweb_bb-0.1.4/punkweb_bb/parsers.py` & `punkweb_bb-0.2.0/punkweb_bb/parsers.py`

 * *Files identical despite different names*

### Comparing `punkweb_bb-0.1.4/punkweb_bb/settings.py` & `punkweb_bb-0.2.0/punkweb_bb/settings.py`

 * *Files identical despite different names*

### Comparing `punkweb_bb-0.1.4/punkweb_bb/static/punkweb_bb/css/defaults.css` & `punkweb_bb-0.2.0/punkweb_bb/static/punkweb_bb/css/defaults.css`

 * *Files identical despite different names*

### Comparing `punkweb_bb-0.1.4/punkweb_bb/static/punkweb_bb/css/index.css` & `punkweb_bb-0.2.0/punkweb_bb/static/punkweb_bb/css/index.css`

 * *Files 8% similar despite different names*

```diff
@@ -3,14 +3,20 @@
   gap: 1rem;
 }
 
 .index__categories {
   flex: 1;
 }
 
+.index__category__actions {
+  align-items: center;
+  display: flex;
+  gap: 0.25rem;
+}
+
 .index__sidebar {
   flex: 0 0 20rem;
 }
 
 .index__recentThreads__content {
   display: flex;
   flex-direction: column;
```

### Comparing `punkweb_bb-0.1.4/punkweb_bb/static/punkweb_bb/css/profile.css` & `punkweb_bb-0.2.0/punkweb_bb/static/punkweb_bb/css/profile.css`

 * *Files identical despite different names*

### Comparing `punkweb_bb-0.1.4/punkweb_bb/static/punkweb_bb/css/punkweb-modal.css` & `punkweb_bb-0.2.0/punkweb_bb/static/punkweb_bb/css/punkweb-modal.css`

 * *Files identical despite different names*

### Comparing `punkweb_bb-0.1.4/punkweb_bb/static/punkweb_bb/css/punkweb.css` & `punkweb_bb-0.2.0/punkweb_bb/static/punkweb_bb/css/punkweb.css`

 * *Files 10% similar despite different names*

```diff
@@ -402,26 +402,82 @@
   max-height: 2rem;
   max-width: 2rem;
   min-height: 2rem;
   min-width: 2rem;
   width: 2rem;
 }
 
+.pw-icon-button .material-symbols-outlined {
+  display: block;
+  font-size: 1.125rem;
+}
+
+.pw-icon-button.xs {
+  height: 1rem;
+  line-height: 1rem;
+  max-height: 1rem;
+  max-width: 1rem;
+  min-height: 1rem;
+  min-width: 1rem;
+  width: 1rem;
+}
+
+.pw-icon-button.xs .material-symbols-outlined {
+  font-size: 0.875rem;
+}
+
+.pw-icon-button.sm {
+  height: 1.5rem;
+  line-height: 1.5rem;
+  max-height: 1.5rem;
+  max-width: 1.5rem;
+  min-height: 1.5rem;
+  min-width: 1.5rem;
+  width: 1.5rem;
+}
+
+.pw-icon-button.sm .material-symbols-outlined {
+  font-size: 1rem;
+}
+
+.pw-icon-button.lg {
+  height: 2.5rem;
+  line-height: 2.5rem;
+  max-height: 2.5rem;
+  max-width: 2.5rem;
+  min-height: 2.5rem;
+  min-width: 2.5rem;
+  width: 2.5rem;
+}
+
+.pw-icon-button.lg .material-symbols-outlined {
+  font-size: 1.25rem;
+}
+
+.pw-icon-button.xl {
+  height: 3rem;
+  line-height: 3rem;
+  max-height: 3rem;
+  max-width: 3rem;
+  min-height: 3rem;
+  min-width: 3rem;
+  width: 3rem;
+}
+
+.pw-icon-button.sl .material-symbols-outlined {
+  font-size: 1.5rem;
+}
+
 .pw-icon-button:disabled {
   background-color: var(--oc-gray-5) !important;
   border-color: var(--oc-gray-5) !important;
   color: var(--oc-gray-5) !important;
   cursor: not-allowed;
 }
 
-.pw-icon-button .material-symbols-outlined {
-  display: block;
-  font-size: 1.125rem;
-}
-
 .pw-icon-button.rounded {
   border-radius: 100%;
 }
 
 /* Default */
 
 .pw-icon-button.default {
```

### Comparing `punkweb_bb-0.1.4/punkweb_bb/static/punkweb_bb/css/thread.css` & `punkweb_bb-0.2.0/punkweb_bb/static/punkweb_bb/css/thread.css`

 * *Files 19% similar despite different names*

```diff
@@ -51,14 +51,33 @@
   justify-content: space-between;
 }
 
 .thread__user__info__label {
   color: var(--body-fg);
 }
 
+.thread__user__groups {
+  display: flex;
+  flex-direction: column;
+  gap: 0.5rem;
+  width: 100%;
+}
+
+.thread__user__group {
+  background-color: var(--primary-8);
+  border: 1px solid var(--primary-9);
+  border-radius: 0.25rem;
+  color: var(--text-on-primary);
+  display: flex;
+  font-size: 0.875rem;
+  justify-content: center;
+  padding: 0.5rem;
+  width: 100%;
+}
+
 .thread__main {
   display: flex;
   flex-direction: column;
   width: 100%;
 }
 
 .thread__content {
```

### Comparing `punkweb_bb-0.1.4/punkweb_bb/static/punkweb_bb/css/variables.css` & `punkweb_bb-0.2.0/punkweb_bb/static/punkweb_bb/css/variables.css`

 * *Files 2% similar despite different names*

```diff
@@ -8,14 +8,15 @@
   --primary-6: var(--oc-indigo-6);
   --primary-7: var(--oc-indigo-7);
   --primary-8: var(--oc-indigo-8);
   --primary-9: var(--oc-indigo-9);
 
   --text-dark: var(--oc-gray-9);
   --text-light: var(--oc-gray-0);
+  --text-on-primary: var(--oc-gray-0);
 
   --body-bg: var(--oc-white);
   --body-fg: var(--text-dark);
 
   --border: var(--oc-gray-4);
 
   --link: var(--primary-9);
```

### Comparing `punkweb_bb-0.1.4/punkweb_bb/static/punkweb_bb/editor/bbcode-editor-content.css` & `punkweb_bb-0.2.0/punkweb_bb/static/punkweb_bb/editor/bbcode-editor-content.css`

 * *Files identical despite different names*

### Comparing `punkweb_bb-0.1.4/punkweb_bb/static/punkweb_bb/editor/bbcode-editor-tags.js` & `punkweb_bb-0.2.0/punkweb_bb/static/punkweb_bb/editor/bbcode-editor-tags.js`

 * *Files identical despite different names*

### Comparing `punkweb_bb-0.1.4/punkweb_bb/static/punkweb_bb/editor/bbcode-editor.js` & `punkweb_bb-0.2.0/punkweb_bb/static/punkweb_bb/editor/bbcode-editor.js`

 * *Files identical despite different names*

### Comparing `punkweb_bb-0.1.4/punkweb_bb/static/punkweb_bb/img/default-profile-image.png` & `punkweb_bb-0.2.0/punkweb_bb/static/punkweb_bb/img/default-profile-image.png`

 * *Files identical despite different names*

### Comparing `punkweb_bb-0.1.4/punkweb_bb/static/punkweb_bb/vendor/htmx-1.9.4.min.js` & `punkweb_bb-0.2.0/punkweb_bb/static/punkweb_bb/vendor/htmx-1.9.4.min.js`

 * *Files identical despite different names*

### Comparing `punkweb_bb-0.1.4/punkweb_bb/static/punkweb_bb/vendor/jquery-3.7.0.min.js` & `punkweb_bb-0.2.0/punkweb_bb/static/punkweb_bb/vendor/jquery-3.7.0.min.js`

 * *Files identical despite different names*

### Comparing `punkweb_bb-0.1.4/punkweb_bb/static/punkweb_bb/vendor/open-color.css` & `punkweb_bb-0.2.0/punkweb_bb/static/punkweb_bb/vendor/open-color.css`

 * *Files identical despite different names*

### Comparing `punkweb_bb-0.1.4/punkweb_bb/static/punkweb_bb/vendor/prism.css` & `punkweb_bb-0.2.0/punkweb_bb/static/punkweb_bb/vendor/prism.css`

 * *Files identical despite different names*

### Comparing `punkweb_bb-0.1.4/punkweb_bb/static/punkweb_bb/vendor/prism.js` & `punkweb_bb-0.2.0/punkweb_bb/static/punkweb_bb/vendor/prism.js`

 * *Files identical despite different names*

### Comparing `punkweb_bb-0.1.4/punkweb_bb/static/punkweb_bb/vendor/sceditor-3.2.0/README.md` & `punkweb_bb-0.2.0/punkweb_bb/static/punkweb_bb/vendor/sceditor-3.2.0/README.md`

 * *Files identical despite different names*

### Comparing `punkweb_bb-0.1.4/punkweb_bb/static/punkweb_bb/vendor/sceditor-3.2.0/development/formats/bbcode.js` & `punkweb_bb-0.2.0/punkweb_bb/static/punkweb_bb/vendor/sceditor-3.2.0/development/formats/bbcode.js`

 * *Files identical despite different names*

### Comparing `punkweb_bb-0.1.4/punkweb_bb/static/punkweb_bb/vendor/sceditor-3.2.0/development/formats/xhtml.js` & `punkweb_bb-0.2.0/punkweb_bb/static/punkweb_bb/vendor/sceditor-3.2.0/development/formats/xhtml.js`

 * *Files identical despite different names*

### Comparing `punkweb_bb-0.1.4/punkweb_bb/static/punkweb_bb/vendor/sceditor-3.2.0/development/icons/material.js` & `punkweb_bb-0.2.0/punkweb_bb/static/punkweb_bb/vendor/sceditor-3.2.0/development/icons/material.js`

 * *Files identical despite different names*

### Comparing `punkweb_bb-0.1.4/punkweb_bb/static/punkweb_bb/vendor/sceditor-3.2.0/development/icons/monocons.js` & `punkweb_bb-0.2.0/punkweb_bb/static/punkweb_bb/vendor/sceditor-3.2.0/development/icons/monocons.js`

 * *Files identical despite different names*

### Comparing `punkweb_bb-0.1.4/punkweb_bb/static/punkweb_bb/vendor/sceditor-3.2.0/development/jquery.sceditor.bbcode.js` & `punkweb_bb-0.2.0/punkweb_bb/static/punkweb_bb/vendor/sceditor-3.2.0/development/jquery.sceditor.bbcode.js`

 * *Files identical despite different names*

### Comparing `punkweb_bb-0.1.4/punkweb_bb/static/punkweb_bb/vendor/sceditor-3.2.0/development/jquery.sceditor.js` & `punkweb_bb-0.2.0/punkweb_bb/static/punkweb_bb/vendor/sceditor-3.2.0/development/jquery.sceditor.js`

 * *Files identical despite different names*

### Comparing `punkweb_bb-0.1.4/punkweb_bb/static/punkweb_bb/vendor/sceditor-3.2.0/development/jquery.sceditor.xhtml.js` & `punkweb_bb-0.2.0/punkweb_bb/static/punkweb_bb/vendor/sceditor-3.2.0/development/jquery.sceditor.xhtml.js`

 * *Files identical despite different names*

### Comparing `punkweb_bb-0.1.4/punkweb_bb/static/punkweb_bb/vendor/sceditor-3.2.0/development/plugins/alternative-lists.js` & `punkweb_bb-0.2.0/punkweb_bb/static/punkweb_bb/vendor/sceditor-3.2.0/development/plugins/alternative-lists.js`

 * *Files identical despite different names*

### Comparing `punkweb_bb-0.1.4/punkweb_bb/static/punkweb_bb/vendor/sceditor-3.2.0/development/plugins/autosave.js` & `punkweb_bb-0.2.0/punkweb_bb/static/punkweb_bb/vendor/sceditor-3.2.0/development/plugins/autosave.js`

 * *Files identical despite different names*

### Comparing `punkweb_bb-0.1.4/punkweb_bb/static/punkweb_bb/vendor/sceditor-3.2.0/development/plugins/autoyoutube.js` & `punkweb_bb-0.2.0/punkweb_bb/static/punkweb_bb/vendor/sceditor-3.2.0/development/plugins/autoyoutube.js`

 * *Files identical despite different names*

### Comparing `punkweb_bb-0.1.4/punkweb_bb/static/punkweb_bb/vendor/sceditor-3.2.0/development/plugins/dragdrop.js` & `punkweb_bb-0.2.0/punkweb_bb/static/punkweb_bb/vendor/sceditor-3.2.0/development/plugins/dragdrop.js`

 * *Files identical despite different names*

### Comparing `punkweb_bb-0.1.4/punkweb_bb/static/punkweb_bb/vendor/sceditor-3.2.0/development/plugins/format.js` & `punkweb_bb-0.2.0/punkweb_bb/static/punkweb_bb/vendor/sceditor-3.2.0/development/plugins/format.js`

 * *Files identical despite different names*

### Comparing `punkweb_bb-0.1.4/punkweb_bb/static/punkweb_bb/vendor/sceditor-3.2.0/development/plugins/plaintext.js` & `punkweb_bb-0.2.0/punkweb_bb/static/punkweb_bb/vendor/sceditor-3.2.0/development/plugins/plaintext.js`

 * *Files identical despite different names*

### Comparing `punkweb_bb-0.1.4/punkweb_bb/static/punkweb_bb/vendor/sceditor-3.2.0/development/plugins/undo.js` & `punkweb_bb-0.2.0/punkweb_bb/static/punkweb_bb/vendor/sceditor-3.2.0/development/plugins/undo.js`

 * *Files identical despite different names*

### Comparing `punkweb_bb-0.1.4/punkweb_bb/static/punkweb_bb/vendor/sceditor-3.2.0/development/plugins/v1compat.js` & `punkweb_bb-0.2.0/punkweb_bb/static/punkweb_bb/vendor/sceditor-3.2.0/development/plugins/v1compat.js`

 * *Files identical despite different names*

### Comparing `punkweb_bb-0.1.4/punkweb_bb/static/punkweb_bb/vendor/sceditor-3.2.0/development/sceditor.js` & `punkweb_bb-0.2.0/punkweb_bb/static/punkweb_bb/vendor/sceditor-3.2.0/development/sceditor.js`

 * *Files identical despite different names*

### Comparing `punkweb_bb-0.1.4/punkweb_bb/static/punkweb_bb/vendor/sceditor-3.2.0/development/themes/content/default.css` & `punkweb_bb-0.2.0/punkweb_bb/static/punkweb_bb/vendor/sceditor-3.2.0/development/themes/content/default.css`

 * *Files identical despite different names*

### Comparing `punkweb_bb-0.1.4/punkweb_bb/static/punkweb_bb/vendor/sceditor-3.2.0/development/themes/default.css` & `punkweb_bb-0.2.0/punkweb_bb/static/punkweb_bb/vendor/sceditor-3.2.0/development/themes/default.css`

 * *Files identical despite different names*

### Comparing `punkweb_bb-0.1.4/punkweb_bb/static/punkweb_bb/vendor/sceditor-3.2.0/development/themes/defaultdark.css` & `punkweb_bb-0.2.0/punkweb_bb/static/punkweb_bb/vendor/sceditor-3.2.0/development/themes/defaultdark.css`

 * *Files identical despite different names*

### Comparing `punkweb_bb-0.1.4/punkweb_bb/static/punkweb_bb/vendor/sceditor-3.2.0/development/themes/famfamfam.png` & `punkweb_bb-0.2.0/punkweb_bb/static/punkweb_bb/vendor/sceditor-3.2.0/development/themes/famfamfam.png`

 * *Files identical despite different names*

### Comparing `punkweb_bb-0.1.4/punkweb_bb/static/punkweb_bb/vendor/sceditor-3.2.0/development/themes/modern.css` & `punkweb_bb-0.2.0/punkweb_bb/static/punkweb_bb/vendor/sceditor-3.2.0/development/themes/modern.css`

 * *Files identical despite different names*

### Comparing `punkweb_bb-0.1.4/punkweb_bb/static/punkweb_bb/vendor/sceditor-3.2.0/development/themes/office-toolbar.css` & `punkweb_bb-0.2.0/punkweb_bb/static/punkweb_bb/vendor/sceditor-3.2.0/development/themes/office-toolbar.css`

 * *Files identical despite different names*

### Comparing `punkweb_bb-0.1.4/punkweb_bb/static/punkweb_bb/vendor/sceditor-3.2.0/development/themes/office.css` & `punkweb_bb-0.2.0/punkweb_bb/static/punkweb_bb/vendor/sceditor-3.2.0/development/themes/office.css`

 * *Files identical despite different names*

### Comparing `punkweb_bb-0.1.4/punkweb_bb/static/punkweb_bb/vendor/sceditor-3.2.0/development/themes/square.css` & `punkweb_bb-0.2.0/punkweb_bb/static/punkweb_bb/vendor/sceditor-3.2.0/development/themes/square.css`

 * *Files identical despite different names*

### Comparing `punkweb_bb-0.1.4/punkweb_bb/static/punkweb_bb/vendor/sceditor-3.2.0/emoticons/alien.png` & `punkweb_bb-0.2.0/punkweb_bb/static/punkweb_bb/vendor/sceditor-3.2.0/emoticons/alien.png`

 * *Files identical despite different names*

### Comparing `punkweb_bb-0.1.4/punkweb_bb/static/punkweb_bb/vendor/sceditor-3.2.0/emoticons/angel.png` & `punkweb_bb-0.2.0/punkweb_bb/static/punkweb_bb/vendor/sceditor-3.2.0/emoticons/angel.png`

 * *Files identical despite different names*

### Comparing `punkweb_bb-0.1.4/punkweb_bb/static/punkweb_bb/vendor/sceditor-3.2.0/emoticons/angry.png` & `punkweb_bb-0.2.0/punkweb_bb/static/punkweb_bb/vendor/sceditor-3.2.0/emoticons/angry.png`

 * *Files identical despite different names*

### Comparing `punkweb_bb-0.1.4/punkweb_bb/static/punkweb_bb/vendor/sceditor-3.2.0/emoticons/blink.png` & `punkweb_bb-0.2.0/punkweb_bb/static/punkweb_bb/vendor/sceditor-3.2.0/emoticons/blink.png`

 * *Files identical despite different names*

### Comparing `punkweb_bb-0.1.4/punkweb_bb/static/punkweb_bb/vendor/sceditor-3.2.0/emoticons/blush.png` & `punkweb_bb-0.2.0/punkweb_bb/static/punkweb_bb/vendor/sceditor-3.2.0/emoticons/blush.png`

 * *Files identical despite different names*

### Comparing `punkweb_bb-0.1.4/punkweb_bb/static/punkweb_bb/vendor/sceditor-3.2.0/emoticons/cheerful.png` & `punkweb_bb-0.2.0/punkweb_bb/static/punkweb_bb/vendor/sceditor-3.2.0/emoticons/cheerful.png`

 * *Files identical despite different names*

### Comparing `punkweb_bb-0.1.4/punkweb_bb/static/punkweb_bb/vendor/sceditor-3.2.0/emoticons/cool.png` & `punkweb_bb-0.2.0/punkweb_bb/static/punkweb_bb/vendor/sceditor-3.2.0/emoticons/cool.png`

 * *Files identical despite different names*

### Comparing `punkweb_bb-0.1.4/punkweb_bb/static/punkweb_bb/vendor/sceditor-3.2.0/emoticons/cwy.png` & `punkweb_bb-0.2.0/punkweb_bb/static/punkweb_bb/vendor/sceditor-3.2.0/emoticons/cwy.png`

 * *Files identical despite different names*

### Comparing `punkweb_bb-0.1.4/punkweb_bb/static/punkweb_bb/vendor/sceditor-3.2.0/emoticons/devil.png` & `punkweb_bb-0.2.0/punkweb_bb/static/punkweb_bb/vendor/sceditor-3.2.0/emoticons/devil.png`

 * *Files identical despite different names*

### Comparing `punkweb_bb-0.1.4/punkweb_bb/static/punkweb_bb/vendor/sceditor-3.2.0/emoticons/dizzy.png` & `punkweb_bb-0.2.0/punkweb_bb/static/punkweb_bb/vendor/sceditor-3.2.0/emoticons/dizzy.png`

 * *Files identical despite different names*

### Comparing `punkweb_bb-0.1.4/punkweb_bb/static/punkweb_bb/vendor/sceditor-3.2.0/emoticons/ermm.png` & `punkweb_bb-0.2.0/punkweb_bb/static/punkweb_bb/vendor/sceditor-3.2.0/emoticons/ermm.png`

 * *Files identical despite different names*

### Comparing `punkweb_bb-0.1.4/punkweb_bb/static/punkweb_bb/vendor/sceditor-3.2.0/emoticons/face.png` & `punkweb_bb-0.2.0/punkweb_bb/static/punkweb_bb/vendor/sceditor-3.2.0/emoticons/face.png`

 * *Files identical despite different names*

### Comparing `punkweb_bb-0.1.4/punkweb_bb/static/punkweb_bb/vendor/sceditor-3.2.0/emoticons/getlost.png` & `punkweb_bb-0.2.0/punkweb_bb/static/punkweb_bb/vendor/sceditor-3.2.0/emoticons/getlost.png`

 * *Files identical despite different names*

### Comparing `punkweb_bb-0.1.4/punkweb_bb/static/punkweb_bb/vendor/sceditor-3.2.0/emoticons/grin.png` & `punkweb_bb-0.2.0/punkweb_bb/static/punkweb_bb/vendor/sceditor-3.2.0/emoticons/grin.png`

 * *Files identical despite different names*

### Comparing `punkweb_bb-0.1.4/punkweb_bb/static/punkweb_bb/vendor/sceditor-3.2.0/emoticons/happy.png` & `punkweb_bb-0.2.0/punkweb_bb/static/punkweb_bb/vendor/sceditor-3.2.0/emoticons/happy.png`

 * *Files identical despite different names*

### Comparing `punkweb_bb-0.1.4/punkweb_bb/static/punkweb_bb/vendor/sceditor-3.2.0/emoticons/heart.png` & `punkweb_bb-0.2.0/punkweb_bb/static/punkweb_bb/vendor/sceditor-3.2.0/emoticons/heart.png`

 * *Files identical despite different names*

### Comparing `punkweb_bb-0.1.4/punkweb_bb/static/punkweb_bb/vendor/sceditor-3.2.0/emoticons/kissing.png` & `punkweb_bb-0.2.0/punkweb_bb/static/punkweb_bb/vendor/sceditor-3.2.0/emoticons/kissing.png`

 * *Files identical despite different names*

### Comparing `punkweb_bb-0.1.4/punkweb_bb/static/punkweb_bb/vendor/sceditor-3.2.0/emoticons/laughing.png` & `punkweb_bb-0.2.0/punkweb_bb/static/punkweb_bb/vendor/sceditor-3.2.0/emoticons/laughing.png`

 * *Files identical despite different names*

### Comparing `punkweb_bb-0.1.4/punkweb_bb/static/punkweb_bb/vendor/sceditor-3.2.0/emoticons/ninja.png` & `punkweb_bb-0.2.0/punkweb_bb/static/punkweb_bb/vendor/sceditor-3.2.0/emoticons/ninja.png`

 * *Files identical despite different names*

### Comparing `punkweb_bb-0.1.4/punkweb_bb/static/punkweb_bb/vendor/sceditor-3.2.0/emoticons/pinch.png` & `punkweb_bb-0.2.0/punkweb_bb/static/punkweb_bb/vendor/sceditor-3.2.0/emoticons/pinch.png`

 * *Files identical despite different names*

### Comparing `punkweb_bb-0.1.4/punkweb_bb/static/punkweb_bb/vendor/sceditor-3.2.0/emoticons/pouty.png` & `punkweb_bb-0.2.0/punkweb_bb/static/punkweb_bb/vendor/sceditor-3.2.0/emoticons/pouty.png`

 * *Files identical despite different names*

### Comparing `punkweb_bb-0.1.4/punkweb_bb/static/punkweb_bb/vendor/sceditor-3.2.0/emoticons/sad.png` & `punkweb_bb-0.2.0/punkweb_bb/static/punkweb_bb/vendor/sceditor-3.2.0/emoticons/sad.png`

 * *Files identical despite different names*

### Comparing `punkweb_bb-0.1.4/punkweb_bb/static/punkweb_bb/vendor/sceditor-3.2.0/emoticons/shocked.png` & `punkweb_bb-0.2.0/punkweb_bb/static/punkweb_bb/vendor/sceditor-3.2.0/emoticons/shocked.png`

 * *Files identical despite different names*

### Comparing `punkweb_bb-0.1.4/punkweb_bb/static/punkweb_bb/vendor/sceditor-3.2.0/emoticons/sick.png` & `punkweb_bb-0.2.0/punkweb_bb/static/punkweb_bb/vendor/sceditor-3.2.0/emoticons/sick.png`

 * *Files identical despite different names*

### Comparing `punkweb_bb-0.1.4/punkweb_bb/static/punkweb_bb/vendor/sceditor-3.2.0/emoticons/sideways.png` & `punkweb_bb-0.2.0/punkweb_bb/static/punkweb_bb/vendor/sceditor-3.2.0/emoticons/sideways.png`

 * *Files identical despite different names*

### Comparing `punkweb_bb-0.1.4/punkweb_bb/static/punkweb_bb/vendor/sceditor-3.2.0/emoticons/silly.png` & `punkweb_bb-0.2.0/punkweb_bb/static/punkweb_bb/vendor/sceditor-3.2.0/emoticons/silly.png`

 * *Files identical despite different names*

### Comparing `punkweb_bb-0.1.4/punkweb_bb/static/punkweb_bb/vendor/sceditor-3.2.0/emoticons/sleeping.png` & `punkweb_bb-0.2.0/punkweb_bb/static/punkweb_bb/vendor/sceditor-3.2.0/emoticons/sleeping.png`

 * *Files identical despite different names*

### Comparing `punkweb_bb-0.1.4/punkweb_bb/static/punkweb_bb/vendor/sceditor-3.2.0/emoticons/smile.png` & `punkweb_bb-0.2.0/punkweb_bb/static/punkweb_bb/vendor/sceditor-3.2.0/emoticons/smile.png`

 * *Files identical despite different names*

### Comparing `punkweb_bb-0.1.4/punkweb_bb/static/punkweb_bb/vendor/sceditor-3.2.0/emoticons/tongue.png` & `punkweb_bb-0.2.0/punkweb_bb/static/punkweb_bb/vendor/sceditor-3.2.0/emoticons/tongue.png`

 * *Files identical despite different names*

### Comparing `punkweb_bb-0.1.4/punkweb_bb/static/punkweb_bb/vendor/sceditor-3.2.0/emoticons/unsure.png` & `punkweb_bb-0.2.0/punkweb_bb/static/punkweb_bb/vendor/sceditor-3.2.0/emoticons/unsure.png`

 * *Files identical despite different names*

### Comparing `punkweb_bb-0.1.4/punkweb_bb/static/punkweb_bb/vendor/sceditor-3.2.0/emoticons/w00t.png` & `punkweb_bb-0.2.0/punkweb_bb/static/punkweb_bb/vendor/sceditor-3.2.0/emoticons/w00t.png`

 * *Files identical despite different names*

### Comparing `punkweb_bb-0.1.4/punkweb_bb/static/punkweb_bb/vendor/sceditor-3.2.0/emoticons/wassat.png` & `punkweb_bb-0.2.0/punkweb_bb/static/punkweb_bb/vendor/sceditor-3.2.0/emoticons/wassat.png`

 * *Files identical despite different names*

### Comparing `punkweb_bb-0.1.4/punkweb_bb/static/punkweb_bb/vendor/sceditor-3.2.0/emoticons/whistling.png` & `punkweb_bb-0.2.0/punkweb_bb/static/punkweb_bb/vendor/sceditor-3.2.0/emoticons/whistling.png`

 * *Files identical despite different names*

### Comparing `punkweb_bb-0.1.4/punkweb_bb/static/punkweb_bb/vendor/sceditor-3.2.0/emoticons/wink.png` & `punkweb_bb-0.2.0/punkweb_bb/static/punkweb_bb/vendor/sceditor-3.2.0/emoticons/wink.png`

 * *Files identical despite different names*

### Comparing `punkweb_bb-0.1.4/punkweb_bb/static/punkweb_bb/vendor/sceditor-3.2.0/emoticons/wub.png` & `punkweb_bb-0.2.0/punkweb_bb/static/punkweb_bb/vendor/sceditor-3.2.0/emoticons/wub.png`

 * *Files identical despite different names*

### Comparing `punkweb_bb-0.1.4/punkweb_bb/static/punkweb_bb/vendor/sceditor-3.2.0/example.html` & `punkweb_bb-0.2.0/punkweb_bb/static/punkweb_bb/vendor/sceditor-3.2.0/example.html`

 * *Files identical despite different names*

### Comparing `punkweb_bb-0.1.4/punkweb_bb/static/punkweb_bb/vendor/sceditor-3.2.0/languages/ar.js` & `punkweb_bb-0.2.0/punkweb_bb/static/punkweb_bb/vendor/sceditor-3.2.0/languages/ar.js`

 * *Files identical despite different names*

### Comparing `punkweb_bb-0.1.4/punkweb_bb/static/punkweb_bb/vendor/sceditor-3.2.0/languages/ca.js` & `punkweb_bb-0.2.0/punkweb_bb/static/punkweb_bb/vendor/sceditor-3.2.0/languages/ca.js`

 * *Files identical despite different names*

### Comparing `punkweb_bb-0.1.4/punkweb_bb/static/punkweb_bb/vendor/sceditor-3.2.0/languages/cn.js` & `punkweb_bb-0.2.0/punkweb_bb/static/punkweb_bb/vendor/sceditor-3.2.0/languages/cn.js`

 * *Files identical despite different names*

### Comparing `punkweb_bb-0.1.4/punkweb_bb/static/punkweb_bb/vendor/sceditor-3.2.0/languages/cs.js` & `punkweb_bb-0.2.0/punkweb_bb/static/punkweb_bb/vendor/sceditor-3.2.0/languages/cs.js`

 * *Files identical despite different names*

### Comparing `punkweb_bb-0.1.4/punkweb_bb/static/punkweb_bb/vendor/sceditor-3.2.0/languages/de.js` & `punkweb_bb-0.2.0/punkweb_bb/static/punkweb_bb/vendor/sceditor-3.2.0/languages/de.js`

 * *Files identical despite different names*

### Comparing `punkweb_bb-0.1.4/punkweb_bb/static/punkweb_bb/vendor/sceditor-3.2.0/languages/el.js` & `punkweb_bb-0.2.0/punkweb_bb/static/punkweb_bb/vendor/sceditor-3.2.0/languages/el.js`

 * *Files identical despite different names*

### Comparing `punkweb_bb-0.1.4/punkweb_bb/static/punkweb_bb/vendor/sceditor-3.2.0/languages/es.js` & `punkweb_bb-0.2.0/punkweb_bb/static/punkweb_bb/vendor/sceditor-3.2.0/languages/es.js`

 * *Files identical despite different names*

### Comparing `punkweb_bb-0.1.4/punkweb_bb/static/punkweb_bb/vendor/sceditor-3.2.0/languages/et.js` & `punkweb_bb-0.2.0/punkweb_bb/static/punkweb_bb/vendor/sceditor-3.2.0/languages/et.js`

 * *Files identical despite different names*

### Comparing `punkweb_bb-0.1.4/punkweb_bb/static/punkweb_bb/vendor/sceditor-3.2.0/languages/fa.js` & `punkweb_bb-0.2.0/punkweb_bb/static/punkweb_bb/vendor/sceditor-3.2.0/languages/fa.js`

 * *Files identical despite different names*

### Comparing `punkweb_bb-0.1.4/punkweb_bb/static/punkweb_bb/vendor/sceditor-3.2.0/languages/fi.js` & `punkweb_bb-0.2.0/punkweb_bb/static/punkweb_bb/vendor/sceditor-3.2.0/languages/fi.js`

 * *Files identical despite different names*

### Comparing `punkweb_bb-0.1.4/punkweb_bb/static/punkweb_bb/vendor/sceditor-3.2.0/languages/fr.js` & `punkweb_bb-0.2.0/punkweb_bb/static/punkweb_bb/vendor/sceditor-3.2.0/languages/fr.js`

 * *Files identical despite different names*

### Comparing `punkweb_bb-0.1.4/punkweb_bb/static/punkweb_bb/vendor/sceditor-3.2.0/languages/gl.js` & `punkweb_bb-0.2.0/punkweb_bb/static/punkweb_bb/vendor/sceditor-3.2.0/languages/gl.js`

 * *Files identical despite different names*

### Comparing `punkweb_bb-0.1.4/punkweb_bb/static/punkweb_bb/vendor/sceditor-3.2.0/languages/hu.js` & `punkweb_bb-0.2.0/punkweb_bb/static/punkweb_bb/vendor/sceditor-3.2.0/languages/hu.js`

 * *Files identical despite different names*

### Comparing `punkweb_bb-0.1.4/punkweb_bb/static/punkweb_bb/vendor/sceditor-3.2.0/languages/id.js` & `punkweb_bb-0.2.0/punkweb_bb/static/punkweb_bb/vendor/sceditor-3.2.0/languages/id.js`

 * *Files identical despite different names*

### Comparing `punkweb_bb-0.1.4/punkweb_bb/static/punkweb_bb/vendor/sceditor-3.2.0/languages/it.js` & `punkweb_bb-0.2.0/punkweb_bb/static/punkweb_bb/vendor/sceditor-3.2.0/languages/it.js`

 * *Files identical despite different names*

### Comparing `punkweb_bb-0.1.4/punkweb_bb/static/punkweb_bb/vendor/sceditor-3.2.0/languages/ja.js` & `punkweb_bb-0.2.0/punkweb_bb/static/punkweb_bb/vendor/sceditor-3.2.0/languages/ja.js`

 * *Files identical despite different names*

### Comparing `punkweb_bb-0.1.4/punkweb_bb/static/punkweb_bb/vendor/sceditor-3.2.0/languages/lt.js` & `punkweb_bb-0.2.0/punkweb_bb/static/punkweb_bb/vendor/sceditor-3.2.0/languages/lt.js`

 * *Files identical despite different names*

### Comparing `punkweb_bb-0.1.4/punkweb_bb/static/punkweb_bb/vendor/sceditor-3.2.0/languages/nb.js` & `punkweb_bb-0.2.0/punkweb_bb/static/punkweb_bb/vendor/sceditor-3.2.0/languages/nb.js`

 * *Files identical despite different names*

### Comparing `punkweb_bb-0.1.4/punkweb_bb/static/punkweb_bb/vendor/sceditor-3.2.0/languages/nl.js` & `punkweb_bb-0.2.0/punkweb_bb/static/punkweb_bb/vendor/sceditor-3.2.0/languages/nl.js`

 * *Files identical despite different names*

### Comparing `punkweb_bb-0.1.4/punkweb_bb/static/punkweb_bb/vendor/sceditor-3.2.0/languages/pl.js` & `punkweb_bb-0.2.0/punkweb_bb/static/punkweb_bb/vendor/sceditor-3.2.0/languages/pl.js`

 * *Files identical despite different names*

### Comparing `punkweb_bb-0.1.4/punkweb_bb/static/punkweb_bb/vendor/sceditor-3.2.0/languages/pt-BR.js` & `punkweb_bb-0.2.0/punkweb_bb/static/punkweb_bb/vendor/sceditor-3.2.0/languages/pt-BR.js`

 * *Files identical despite different names*

### Comparing `punkweb_bb-0.1.4/punkweb_bb/static/punkweb_bb/vendor/sceditor-3.2.0/languages/pt.js` & `punkweb_bb-0.2.0/punkweb_bb/static/punkweb_bb/vendor/sceditor-3.2.0/languages/pt.js`

 * *Files identical despite different names*

### Comparing `punkweb_bb-0.1.4/punkweb_bb/static/punkweb_bb/vendor/sceditor-3.2.0/languages/ru.js` & `punkweb_bb-0.2.0/punkweb_bb/static/punkweb_bb/vendor/sceditor-3.2.0/languages/ru.js`

 * *Files identical despite different names*

### Comparing `punkweb_bb-0.1.4/punkweb_bb/static/punkweb_bb/vendor/sceditor-3.2.0/languages/sk.js` & `punkweb_bb-0.2.0/punkweb_bb/static/punkweb_bb/vendor/sceditor-3.2.0/languages/sk.js`

 * *Files identical despite different names*

### Comparing `punkweb_bb-0.1.4/punkweb_bb/static/punkweb_bb/vendor/sceditor-3.2.0/languages/sv.js` & `punkweb_bb-0.2.0/punkweb_bb/static/punkweb_bb/vendor/sceditor-3.2.0/languages/sv.js`

 * *Files identical despite different names*

### Comparing `punkweb_bb-0.1.4/punkweb_bb/static/punkweb_bb/vendor/sceditor-3.2.0/languages/template.js` & `punkweb_bb-0.2.0/punkweb_bb/static/punkweb_bb/vendor/sceditor-3.2.0/languages/template.js`

 * *Files identical despite different names*

### Comparing `punkweb_bb-0.1.4/punkweb_bb/static/punkweb_bb/vendor/sceditor-3.2.0/languages/tr.js` & `punkweb_bb-0.2.0/punkweb_bb/static/punkweb_bb/vendor/sceditor-3.2.0/languages/tr.js`

 * *Files identical despite different names*

### Comparing `punkweb_bb-0.1.4/punkweb_bb/static/punkweb_bb/vendor/sceditor-3.2.0/languages/tw.js` & `punkweb_bb-0.2.0/punkweb_bb/static/punkweb_bb/vendor/sceditor-3.2.0/languages/tw.js`

 * *Files identical despite different names*

### Comparing `punkweb_bb-0.1.4/punkweb_bb/static/punkweb_bb/vendor/sceditor-3.2.0/languages/uk.js` & `punkweb_bb-0.2.0/punkweb_bb/static/punkweb_bb/vendor/sceditor-3.2.0/languages/uk.js`

 * *Files identical despite different names*

### Comparing `punkweb_bb-0.1.4/punkweb_bb/static/punkweb_bb/vendor/sceditor-3.2.0/languages/vi.js` & `punkweb_bb-0.2.0/punkweb_bb/static/punkweb_bb/vendor/sceditor-3.2.0/languages/vi.js`

 * *Files identical despite different names*

### Comparing `punkweb_bb-0.1.4/punkweb_bb/static/punkweb_bb/vendor/sceditor-3.2.0/minified/formats/bbcode.js` & `punkweb_bb-0.2.0/punkweb_bb/static/punkweb_bb/vendor/sceditor-3.2.0/minified/formats/bbcode.js`

 * *Files identical despite different names*

### Comparing `punkweb_bb-0.1.4/punkweb_bb/static/punkweb_bb/vendor/sceditor-3.2.0/minified/formats/xhtml.js` & `punkweb_bb-0.2.0/punkweb_bb/static/punkweb_bb/vendor/sceditor-3.2.0/minified/formats/xhtml.js`

 * *Files identical despite different names*

### Comparing `punkweb_bb-0.1.4/punkweb_bb/static/punkweb_bb/vendor/sceditor-3.2.0/minified/icons/material.js` & `punkweb_bb-0.2.0/punkweb_bb/static/punkweb_bb/vendor/sceditor-3.2.0/minified/icons/material.js`

 * *Files identical despite different names*

### Comparing `punkweb_bb-0.1.4/punkweb_bb/static/punkweb_bb/vendor/sceditor-3.2.0/minified/icons/monocons.js` & `punkweb_bb-0.2.0/punkweb_bb/static/punkweb_bb/vendor/sceditor-3.2.0/minified/icons/monocons.js`

 * *Files identical despite different names*

### Comparing `punkweb_bb-0.1.4/punkweb_bb/static/punkweb_bb/vendor/sceditor-3.2.0/minified/jquery.sceditor.bbcode.min.js` & `punkweb_bb-0.2.0/punkweb_bb/static/punkweb_bb/vendor/sceditor-3.2.0/minified/jquery.sceditor.bbcode.min.js`

 * *Files identical despite different names*

### Comparing `punkweb_bb-0.1.4/punkweb_bb/static/punkweb_bb/vendor/sceditor-3.2.0/minified/jquery.sceditor.min.js` & `punkweb_bb-0.2.0/punkweb_bb/static/punkweb_bb/vendor/sceditor-3.2.0/minified/jquery.sceditor.min.js`

 * *Files identical despite different names*

### Comparing `punkweb_bb-0.1.4/punkweb_bb/static/punkweb_bb/vendor/sceditor-3.2.0/minified/jquery.sceditor.xhtml.min.js` & `punkweb_bb-0.2.0/punkweb_bb/static/punkweb_bb/vendor/sceditor-3.2.0/minified/jquery.sceditor.xhtml.min.js`

 * *Files identical despite different names*

### Comparing `punkweb_bb-0.1.4/punkweb_bb/static/punkweb_bb/vendor/sceditor-3.2.0/minified/plugins/alternative-lists.js` & `punkweb_bb-0.2.0/punkweb_bb/static/punkweb_bb/vendor/sceditor-3.2.0/minified/plugins/alternative-lists.js`

 * *Files identical despite different names*

### Comparing `punkweb_bb-0.1.4/punkweb_bb/static/punkweb_bb/vendor/sceditor-3.2.0/minified/plugins/autosave.js` & `punkweb_bb-0.2.0/punkweb_bb/static/punkweb_bb/vendor/sceditor-3.2.0/minified/plugins/autosave.js`

 * *Files identical despite different names*

### Comparing `punkweb_bb-0.1.4/punkweb_bb/static/punkweb_bb/vendor/sceditor-3.2.0/minified/plugins/autoyoutube.js` & `punkweb_bb-0.2.0/punkweb_bb/static/punkweb_bb/vendor/sceditor-3.2.0/minified/plugins/autoyoutube.js`

 * *Files identical despite different names*

### Comparing `punkweb_bb-0.1.4/punkweb_bb/static/punkweb_bb/vendor/sceditor-3.2.0/minified/plugins/dragdrop.js` & `punkweb_bb-0.2.0/punkweb_bb/static/punkweb_bb/vendor/sceditor-3.2.0/minified/plugins/dragdrop.js`

 * *Files identical despite different names*

### Comparing `punkweb_bb-0.1.4/punkweb_bb/static/punkweb_bb/vendor/sceditor-3.2.0/minified/plugins/format.js` & `punkweb_bb-0.2.0/punkweb_bb/static/punkweb_bb/vendor/sceditor-3.2.0/minified/plugins/format.js`

 * *Files identical despite different names*

### Comparing `punkweb_bb-0.1.4/punkweb_bb/static/punkweb_bb/vendor/sceditor-3.2.0/minified/plugins/plaintext.js` & `punkweb_bb-0.2.0/punkweb_bb/static/punkweb_bb/vendor/sceditor-3.2.0/minified/plugins/plaintext.js`

 * *Files identical despite different names*

### Comparing `punkweb_bb-0.1.4/punkweb_bb/static/punkweb_bb/vendor/sceditor-3.2.0/minified/plugins/undo.js` & `punkweb_bb-0.2.0/punkweb_bb/static/punkweb_bb/vendor/sceditor-3.2.0/minified/plugins/undo.js`

 * *Files identical despite different names*

### Comparing `punkweb_bb-0.1.4/punkweb_bb/static/punkweb_bb/vendor/sceditor-3.2.0/minified/plugins/v1compat.js` & `punkweb_bb-0.2.0/punkweb_bb/static/punkweb_bb/vendor/sceditor-3.2.0/minified/plugins/v1compat.js`

 * *Files identical despite different names*

### Comparing `punkweb_bb-0.1.4/punkweb_bb/static/punkweb_bb/vendor/sceditor-3.2.0/minified/sceditor.min.js` & `punkweb_bb-0.2.0/punkweb_bb/static/punkweb_bb/vendor/sceditor-3.2.0/minified/sceditor.min.js`

 * *Files identical despite different names*

### Comparing `punkweb_bb-0.1.4/punkweb_bb/static/punkweb_bb/vendor/sceditor-3.2.0/minified/themes/content/default.min.css` & `punkweb_bb-0.2.0/punkweb_bb/static/punkweb_bb/vendor/sceditor-3.2.0/minified/themes/content/default.min.css`

 * *Files identical despite different names*

### Comparing `punkweb_bb-0.1.4/punkweb_bb/static/punkweb_bb/vendor/sceditor-3.2.0/minified/themes/default.min.css` & `punkweb_bb-0.2.0/punkweb_bb/static/punkweb_bb/vendor/sceditor-3.2.0/minified/themes/default.min.css`

 * *Files identical despite different names*

### Comparing `punkweb_bb-0.1.4/punkweb_bb/static/punkweb_bb/vendor/sceditor-3.2.0/minified/themes/defaultdark.min.css` & `punkweb_bb-0.2.0/punkweb_bb/static/punkweb_bb/vendor/sceditor-3.2.0/minified/themes/defaultdark.min.css`

 * *Files identical despite different names*

### Comparing `punkweb_bb-0.1.4/punkweb_bb/static/punkweb_bb/vendor/sceditor-3.2.0/minified/themes/famfamfam.png` & `punkweb_bb-0.2.0/punkweb_bb/static/punkweb_bb/vendor/sceditor-3.2.0/minified/themes/famfamfam.png`

 * *Files identical despite different names*

### Comparing `punkweb_bb-0.1.4/punkweb_bb/static/punkweb_bb/vendor/sceditor-3.2.0/minified/themes/modern.min.css` & `punkweb_bb-0.2.0/punkweb_bb/static/punkweb_bb/vendor/sceditor-3.2.0/minified/themes/modern.min.css`

 * *Files identical despite different names*

### Comparing `punkweb_bb-0.1.4/punkweb_bb/static/punkweb_bb/vendor/sceditor-3.2.0/minified/themes/office-toolbar.min.css` & `punkweb_bb-0.2.0/punkweb_bb/static/punkweb_bb/vendor/sceditor-3.2.0/minified/themes/office-toolbar.min.css`

 * *Files identical despite different names*

### Comparing `punkweb_bb-0.1.4/punkweb_bb/static/punkweb_bb/vendor/sceditor-3.2.0/minified/themes/office.min.css` & `punkweb_bb-0.2.0/punkweb_bb/static/punkweb_bb/vendor/sceditor-3.2.0/minified/themes/office.min.css`

 * *Files identical despite different names*

### Comparing `punkweb_bb-0.1.4/punkweb_bb/static/punkweb_bb/vendor/sceditor-3.2.0/minified/themes/square.min.css` & `punkweb_bb-0.2.0/punkweb_bb/static/punkweb_bb/vendor/sceditor-3.2.0/minified/themes/square.min.css`

 * *Files identical despite different names*

### Comparing `punkweb_bb-0.1.4/punkweb_bb/templates/punkweb_bb/base.html` & `punkweb_bb-0.2.0/punkweb_bb/templates/punkweb_bb/base.html`

 * *Files identical despite different names*

### Comparing `punkweb_bb-0.1.4/punkweb_bb/templates/punkweb_bb/index.html` & `punkweb_bb-0.2.0/punkweb_bb/templates/punkweb_bb/index.html`

 * *Files 12% similar despite different names*

```diff
@@ -34,20 +34,43 @@
                 <th><a href="{{category.get_absolute_url}}">{{category.name}}</a></th>
                 <th>Threads</th>
                 <th>Posts</th>
                 <th></th>
               </tr>
             </thead>
             <tbody>
+              {% if perms.punkweb_bb.add_subcategory or perms.punkweb_bb.change_category or perms.punkweb_bb.delete_category %}
+              <tr>
+                <td colspan="4">
+                  <div class="index__category__actions">
+                    {% if perms.punkweb_bb.add_subcategory %}
+                    <a class="pw-button ghost xs" href="{% url 'punkweb_bb:subcategory_create' category.slug %}">
+                      Create Subcategory
+                    </a>
+                    {% endif %}
+                    {% if perms.punkweb_bb.change_category %}
+                    <a class="pw-button ghost xs" href="{% url 'punkweb_bb:category_update' category.slug %}">
+                      Edit
+                    </a>
+                    {% endif %}
+                    {% if perms.punkweb_bb.delete_category %}
+                    <a class="pw-button ghost danger xs" hx-get="{% url 'punkweb_bb:category_delete' category.slug %}" hx-target="#modal-portal">
+                      Delete
+                    </a>
+                    {% endif %}
+                  </div>
+                </td>
+              </tr>
+              {% endif %}
               {% for subcategory in category.subcategories.all %}
               <tr>
                 <td>
                   <a href="{{subcategory.get_absolute_url}}" title="{{subcategory.name}}">{{subcategory.name}}</a>
                   <div>
-                    {{subcategory.description}}
+                    {{subcategory.description.rendered}}
                   </div>
                 </td>
                 <td>{{subcategory.thread_count}}</td>
                 <td>{{subcategory.post_count}}</td>
                 <td>
                   {% if subcategory.latest_thread %}
                   {% if subcategory.latest_thread.latest_post %}
@@ -106,14 +129,17 @@
               </tr>
               {% endfor %}
             </tbody>
           </table>
         </div>
       </div>
       {% endfor %}
+      {% if perms.punkweb_bb.add_category %}
+      <a class="pw-button ghost xs" href="{% url 'punkweb_bb:category_create' %}">Create Category</a>
+      {% endif %}
     </div>
     <div class="index__sidebar">
       <div class="pw-card fluid">
         <div class="pw-card-header">Recent threads</div>
         <div class="index__recentThreads__content">
           {% for thread in recent_threads %}
           <div class="index__recentThreads__thread">
```

#### html2text {}

```diff
@@ -1,37 +1,39 @@
 {% extends 'punkweb_bb/base.html' %} {% load static %} {% block extra_head %}
 {% endblock %} {% block extra_script %}
 {% endblock %} {% block content %}
 {% if punkweb_bb.settings.SHOUTBOX_ENABLED|default:True %} {% include
 'punkweb_bb/shoutbox/shoutbox.html' %} {% endif %} {% for category in
 categories %}
-_{{_{{_cc_aa_tt_ee_gg_oo_rr_yy_.._nn_aa_mm_ee_}}_}}          TThhrreeaaddss                     PPoossttss
-                                                                                 {% if subcategory.latest_thread %} {% if
-                                                                                 subcategory.latest_thread.latest_post %}
-                                                                                 {% if subcategory.latest_thread.latest_post.user.profile.image
-                                                                                 %} [{
-                                                                                 {subcategory.latest_thread.latest_post.user.profile.image.url}}]
-                                                                                 {% else%} [{% static 'punkweb_bb/img/default-profile-image.png'
-                                                                                 %}]{% endif %}
-                                                                                 _{_{_s_u_b_c_a_t_e_g_o_r_y_._l_a_t_e_s_t___t_h_r_e_a_d_._t_i_t_l_e_}_}
-                                                                                 {{subcategory.latest_thread.latest_post.created_at|date:'M j,
-_{_{_s_u_b_c_a_t_e_g_o_r_y_._n_a_m_e_}_}                                                             Y'}} at {{subcategory.latest_thread.latest_post.created_at|date:
-{                          {                           {                         'g:i A'}} â¢ _{
-{subcategory.description}} {subcategory.thread_count}} {subcategory.post_count}} _{_s_u_b_c_a_t_e_g_o_r_y_._l_a_t_e_s_t___t_h_r_e_a_d_._l_a_t_e_s_t___p_o_s_t_._u_s_e_r_._u_s_e_r_n_a_m_e_}_}
-                                                                                 {% else %}
-                                                                                 {% if subcategory.latest_thread.user.profile.image %} [{
-                                                                                 {subcategory.latest_thread.user.profile.image.url}}]{% else%} [
-                                                                                 {% static 'punkweb_bb/img/default-profile-image.png' %}]{% endif
-                                                                                 %}
-                                                                                 _{_{_s_u_b_c_a_t_e_g_o_r_y_._l_a_t_e_s_t___t_h_r_e_a_d_._t_i_t_l_e_}_}
-                                                                                 {{subcategory.latest_thread.created_at|date:'M j, Y'}} at {
-                                                                                 {subcategory.latest_thread.created_at|date:'g:i A'}} â¢ _{
-                                                                                 _{_s_u_b_c_a_t_e_g_o_r_y_._l_a_t_e_s_t___t_h_r_e_a_d_._u_s_e_r_._u_s_e_r_n_a_m_e_}_}
-                                                                                 {% endif %} {% else %} No threads {% endif %}
-{% endfor %}
+_{{_{{_cc_aa_tt_ee_gg_oo_rr_yy_.._nn_aa_mm_ee_}}_}}                   TThhrreeaaddss                     PPoossttss
+{% if perms.punkweb_bb.add_subcategory %} _C_r_e_a_t_e_ _S_u_b_c_a_t_e_g_o_r_y_ {% endif %} {% if perms.punkweb_bb.change_category %} _E_d_i_t_ {% endif %} {% if
+perms.punkweb_bb.delete_category %} Delete {% endif %}
+                                                                                          {% if subcategory.latest_thread %} {% if
+                                                                                          subcategory.latest_thread.latest_post %}
+                                                                                          {% if subcategory.latest_thread.latest_post.user.profile.image
+                                                                                          %} [{
+                                                                                          {subcategory.latest_thread.latest_post.user.profile.image.url}}]
+                                                                                          {% else%} [{% static 'punkweb_bb/img/default-profile-image.png'
+                                                                                          %}]{% endif %}
+                                                                                          _{_{_s_u_b_c_a_t_e_g_o_r_y_._l_a_t_e_s_t___t_h_r_e_a_d_._t_i_t_l_e_}_}
+                                                                                          {{subcategory.latest_thread.latest_post.created_at|date:'M j,
+_{_{_s_u_b_c_a_t_e_g_o_r_y_._n_a_m_e_}_}                                                                      Y'}} at {{subcategory.latest_thread.latest_post.created_at|date:
+{                                   {                           {                         'g:i A'}} â¢ _{
+{subcategory.description.rendered}} {subcategory.thread_count}} {subcategory.post_count}} _{_s_u_b_c_a_t_e_g_o_r_y_._l_a_t_e_s_t___t_h_r_e_a_d_._l_a_t_e_s_t___p_o_s_t_._u_s_e_r_._u_s_e_r_n_a_m_e_}_}
+                                                                                          {% else %}
+                                                                                          {% if subcategory.latest_thread.user.profile.image %} [{
+                                                                                          {subcategory.latest_thread.user.profile.image.url}}]{% else%} [
+                                                                                          {% static 'punkweb_bb/img/default-profile-image.png' %}]{% endif
+                                                                                          %}
+                                                                                          _{_{_s_u_b_c_a_t_e_g_o_r_y_._l_a_t_e_s_t___t_h_r_e_a_d_._t_i_t_l_e_}_}
+                                                                                          {{subcategory.latest_thread.created_at|date:'M j, Y'}} at {
+                                                                                          {subcategory.latest_thread.created_at|date:'g:i A'}} â¢ _{
+                                                                                          _{_s_u_b_c_a_t_e_g_o_r_y_._l_a_t_e_s_t___t_h_r_e_a_d_._u_s_e_r_._u_s_e_r_n_a_m_e_}_}
+                                                                                          {% endif %} {% else %} No threads {% endif %}
+{% endfor %} {% if perms.punkweb_bb.add_category %} _C_r_e_a_t_e_ _C_a_t_e_g_o_r_y {% endif %}
 Recent threads
 {% for thread in recent_threads %}
 {% if thread.user.profile.image %} [{{thread.user.profile.image.url}}]{% else%}
 [{% static 'punkweb_bb/img/default-profile-image.png' %}]{% endif %}
 _{_{_t_h_r_e_a_d_._t_i_t_l_e_}_}
 {{thread.created_at|date:'M j, Y'}} at {{thread.created_at|date:'g:i A'}} â¢ _{
 _{_t_h_r_e_a_d_._u_s_e_r_._u_s_e_r_n_a_m_e_}_}
```

### Comparing `punkweb_bb-0.1.4/punkweb_bb/templates/punkweb_bb/login.html` & `punkweb_bb-0.2.0/punkweb_bb/templates/punkweb_bb/login.html`

 * *Files identical despite different names*

### Comparing `punkweb_bb-0.1.4/punkweb_bb/templates/punkweb_bb/members.html` & `punkweb_bb-0.2.0/punkweb_bb/templates/punkweb_bb/members.html`

 * *Files identical despite different names*

### Comparing `punkweb_bb-0.1.4/punkweb_bb/templates/punkweb_bb/partials/post_update.html` & `punkweb_bb-0.2.0/punkweb_bb/templates/punkweb_bb/partials/post_update.html`

 * *Files identical despite different names*

### Comparing `punkweb_bb-0.1.4/punkweb_bb/templates/punkweb_bb/profile.html` & `punkweb_bb-0.2.0/punkweb_bb/templates/punkweb_bb/profile.html`

 * *Files identical despite different names*

### Comparing `punkweb_bb-0.1.4/punkweb_bb/templates/punkweb_bb/settings.html` & `punkweb_bb-0.2.0/punkweb_bb/templates/punkweb_bb/settings.html`

 * *Files identical despite different names*

### Comparing `punkweb_bb-0.1.4/punkweb_bb/templates/punkweb_bb/shoutbox/shoutbox.html` & `punkweb_bb-0.2.0/punkweb_bb/templates/punkweb_bb/shoutbox/shoutbox.html`

 * *Files identical despite different names*

### Comparing `punkweb_bb-0.1.4/punkweb_bb/templates/punkweb_bb/signup.html` & `punkweb_bb-0.2.0/punkweb_bb/templates/punkweb_bb/signup.html`

 * *Files identical despite different names*

### Comparing `punkweb_bb-0.1.4/punkweb_bb/templates/punkweb_bb/subcategory.html` & `punkweb_bb-0.2.0/punkweb_bb/templates/punkweb_bb/subcategory.html`

 * *Files 8% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 {% extends 'punkweb_bb/base.html' %}
-{% load static humanize_int %}
+{% load static humanize_int can_post %}
 
 {% block title_prefix %}{{subcategory.name}} | {% endblock%}
 
 {% block extra_head %}
 <link rel="stylesheet" href="{% static 'punkweb_bb/css/subcategory.css' %}" />
 {% endblock %}
 
@@ -20,29 +20,44 @@
     <li class="pw-breadcrumb-item active">
       {{subcategory.name}}
     </li>
   </ul>
 </nav>
 
 <div class="subcategory__header">
-  <h1>{{subcategory.name}}</h1>
-  {% if request.user.is_authenticated %}
-  {% if not subcategory.staff_post_only or request.user.is_staff %}
+  <div class="subcategory__header__name">
+    <h1>{{subcategory.name}}</h1>
+    {% if perms.punkweb_bb.change_subcategory or perms.punkweb_bb.delete_subcategory %}
+    <div class="subcategory__header__actions">
+      {% if perms.punkweb_bb.change_subcategory %}
+      <a class="pw-button ghost xs" href="{% url 'punkweb_bb:subcategory_update' subcategory.slug %}">
+        Edit
+      </a>
+      {% endif %}
+      {% if perms.punkweb_bb.delete_subcategory %}
+      <a class="pw-button ghost danger xs" hx-get="{% url 'punkweb_bb:subcategory_delete' subcategory.slug %}" hx-target="#modal-portal">
+        Delete
+      </a>
+      {% endif %}
+    </div>
+    {% endif %}
+  </div>
+
+  {% if subcategory|can_post:request.user %}
   <a class="pw-button ghost primary" href="{% url 'punkweb_bb:thread_create' subcategory.slug %}">Create Thread</a>
   {% else %}
   <button
     class="pw-button ghost primary"
     disabled
     href="{% url 'punkweb_bb:thread_create' subcategory.slug %}"
-    title="Only staff can create threads in this subcategory"
+    title="You do not have permission to create a thread in this subcategory."
   >
     Create Thread
   </button>
   {% endif %}
-  {% endif %}
 </div>
 
 <div class="pw-card fluid margin">
   <div class="pw-table-container">
     <table class="pw-table">
       <colgroup>
         <col span="1">
```

#### html2text {}

```diff
@@ -1,17 +1,22 @@
-{% extends 'punkweb_bb/base.html' %} {% load static humanize_int %} {% block
-title_prefix %}{{subcategory.name}} | {% endblock%} {% block extra_head %}
+{% extends 'punkweb_bb/base.html' %} {% load static humanize_int can_post %} {%
+block title_prefix %}{{subcategory.name}} | {% endblock%} {% block extra_head
+%}
 {% endblock %} {% block content %}
     * _H_o_m_e
     * _{_{_s_u_b_c_a_t_e_g_o_r_y_._c_a_t_e_g_o_r_y_._n_a_m_e_}_}
     * {{subcategory.name}}
 ************ {{{{ssuubbccaatteeggoorryy..nnaammee}}}} ************
-{% if request.user.is_authenticated %} {% if not subcategory.staff_post_only or
-request.user.is_staff %} _C_r_e_a_t_e_ _T_h_r_e_a_d {% else %} Create Thread {% endif %} {%
-endif %}
+{% if perms.punkweb_bb.change_subcategory or
+perms.punkweb_bb.delete_subcategory %}
+{% if perms.punkweb_bb.change_subcategory %} _E_d_i_t_ {% endif %} {% if
+perms.punkweb_bb.delete_subcategory %} Delete {% endif %}
+{% endif %}
+{% if subcategory|can_post:request.user %} _C_r_e_a_t_e_ _T_h_r_e_a_d {% else %} Create
+Thread {% endif %}
 TTiittllee                    PPoossttss                VViieewwss
 _{_{_t_h_r_e_a_d_._t_i_t_l_e_}_} {% if                                           {% if thread.latest_post %}
 thread.is_pinned %} keep                                         _{_{_t_h_r_e_a_d_._l_a_t_e_s_t___p_o_s_t_._c_r_e_a_t_e_d___a_t_|_d_a_t_e_:_'_M_ _j_,
 {% endif %} {% if                                                _Y_'_}_}
 thread.is_closed %} lock                      {                  _{_{_t_h_r_e_a_d_._l_a_t_e_s_t___p_o_s_t_._u_s_e_r_._u_s_e_r_n_a_m_e_}_}
 {% endif %}              {                    {thread.view_count {% if thread.latest_post.user.profile.image
 _{_{_t_h_r_e_a_d_._u_s_e_r_._u_s_e_r_n_a_m_e_}_} {thread.post_count}} | humanize_int}}   %} [{
```

### Comparing `punkweb_bb-0.1.4/punkweb_bb/templates/punkweb_bb/thread.html` & `punkweb_bb-0.2.0/punkweb_bb/templates/punkweb_bb/thread.html`

 * *Files 10% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 {% extends 'punkweb_bb/base.html' %}
-{% load static %}
+{% load static can_delete can_edit can_post %}
 
 {% block title_prefix %}{{thread.title}} | {% endblock %}
 
 {% block extra_head %}
 <link rel="stylesheet" href="{% static 'punkweb_bb/css/post-form.css' %}" />
 <link rel="stylesheet" href="{% static 'punkweb_bb/css/thread.css' %}" />
 <link rel="stylesheet" href="{% static 'punkweb_bb/css/thread-form.css' %}" />
@@ -63,31 +63,42 @@
           </div>
         </div>
         <div class="thread__user__info__row">
           <div class="thread__user__info__label">Posts:</div>
           <div class="thread__user__info__value">{{thread.user.profile.post_count}}</div>
         </div>
       </div>
+      {% if thread.user.groups.all|length > 0 %}
+      <div class="thread__user__groups">
+        {% for group in thread.user.groups.all %}
+        <div class="thread__user__group">{{group.name}}</div>
+        {% endfor %}
+      </div>
+      {% endif %}
     </div>
     <div class="thread__main">
       <div class="thread__content">
         {{thread.content.rendered}}
       </div>
       {% if thread.user.profile.signature.rendered %}
       <div class="thread__signature">
         {{thread.user.profile.signature.rendered}}
       </div>
       {% endif %}
-      {% if thread.user == request.user %}
+      {% if thread|can_delete:request.user or thread|can_edit:request.user %}
       <div class="thread__actions">
+        {% if thread|can_edit:request.user %}
         <a class="pw-button ghost sm" href="{% url 'punkweb_bb:thread_update' thread.id %}">Edit</a>
+        {% endif %}
+        {% if thread|can_delete:request.user %}
         <a class="pw-button ghost danger sm" hx-get="{% url 'punkweb_bb:thread_delete' thread.id %}"
           hx-target="#modal-portal">
           Delete
         </a>
+        {% endif %}
       </div>
       {% endif %}
     </div>
   </div>
 </div>
 {% endif %}
 
@@ -124,31 +135,42 @@
           </div>
         </div>
         <div class="thread__user__info__row">
           <div class="thread__user__info__label">Posts:</div>
           <div class="thread__user__info__value">{{post.user.profile.post_count}}</div>
         </div>
       </div>
+      {% if post.user.groups.all|length > 0 %}
+      <div class="thread__user__groups">
+        {% for group in post.user.groups.all %}
+        <div class="thread__user__group">{{group.name}}</div>
+        {% endfor %}
+      </div>
+      {% endif %}
     </div>
     <div class="thread__main">
       <div class="thread__content">
         {{post.content.rendered}}
       </div>
       {% if post.user.profile.signature.rendered %}
       <div class="thread__signature">
         {{post.user.profile.signature.rendered}}
       </div>
       {% endif %}
-      {% if post.user == request.user %}
+      {% if post|can_delete:request.user or post|can_edit:request.user %}
       <div class="thread__actions">
+        {% if post|can_edit:request.user %}
         <a class="pw-button ghost sm" hx-get="{% url 'punkweb_bb:post_update' post.id %}" hx-target="#modal-portal">Edit</a>
+        {% endif %}
+        {% if post|can_delete:request.user %}
         <a class="pw-button ghost danger sm" hx-get="{% url 'punkweb_bb:post_delete' post.id %}"
           hx-target="#modal-portal">
           Delete
         </a>
+        {% endif %}
       </div>
       {% endif %}
     </div>
   </div>
 </div>
 {% endfor %}
 
@@ -194,16 +216,15 @@
       <a class="pw-pagination-link" href="#">Next</a>
     </li>
     {% endif %}
   </ul>
 </nav>
 {% endif %}
 
-{% if request.user.is_authenticated %}
-{% if not thread.is_closed %}
+{% if thread|can_post:request.user %}
 <div class="pw-card fluid margin">
   <div class="pw-card-header">Reply to thread</div>
   <div class="pw-card-content">
     <div class="thread__reply__content">
       <form class="postForm" action="{% url 'punkweb_bb:post_create' thread.id %}" method="post">
         {% csrf_token %}
         {% for field in post_form %}
@@ -225,10 +246,9 @@
 <div class="pw-card fluid margin">
   <div class="pw-card-header">Thread closed</div>
   <div class="pw-card-content">
     <p>This thread is closed and you cannot reply to it.</p>
   </div>
 </div>
 {% endif %}
-{% endif %}
 
 {% endblock %}
```

#### html2text {}

```diff
@@ -1,9 +1,10 @@
-{% extends 'punkweb_bb/base.html' %} {% load static %} {% block title_prefix %}
-{{thread.title}} | {% endblock %} {% block extra_head %}
+{% extends 'punkweb_bb/base.html' %} {% load static can_delete can_edit
+can_post %} {% block title_prefix %}{{thread.title}} | {% endblock %} {% block
+extra_head %}
 {{post_form.media.css}} {% endblock %} {% block extra_script %} {
 {post_form.media.js}} {% endblock %} {% block content %}
     * _H_o_m_e
     * _{_{_t_h_r_e_a_d_._s_u_b_c_a_t_e_g_o_r_y_._c_a_t_e_g_o_r_y_._n_a_m_e_}_}
     * _{_{_t_h_r_e_a_d_._s_u_b_c_a_t_e_g_o_r_y_._n_a_m_e_}_}
     * {{thread.title}}
 {% if posts.number == 1 %}
@@ -13,19 +14,26 @@
 {thread.user.username}}]{% endif %}
 {% if thread.user.profile.is_online %}
 {% endif %} _{_{_t_h_r_e_a_d_._u_s_e_r_._u_s_e_r_n_a_m_e_}_}
 Joined:
 {{thread.user.date_joined|date:"M d, Y"}}
 Posts:
 {{thread.user.profile.post_count}}
+{% if thread.user.groups.all|length > 0 %}
+{% for group in thread.user.groups.all %}
+{{group.name}}
+{% endfor %}
+{% endif %}
 {{thread.content.rendered}}
 {% if thread.user.profile.signature.rendered %}
 {{thread.user.profile.signature.rendered}}
-{% endif %} {% if thread.user == request.user %}
-_E_d_i_t Delete
+{% endif %} {% if thread|can_delete:request.user or thread|can_edit:
+request.user %}
+{% if thread|can_edit:request.user %} _E_d_i_t {% endif %} {% if thread|can_delete:
+request.user %} Delete {% endif %}
 {% endif %}
 {% endif %} {% for post in posts %}
 {{post.created_at|date:'M d, Y'}}
 _#_{_{_p_o_s_t_._i_n_d_e_x_}_}
 {% if post.user.profile.image %}
 [{{post.user.username}}]
 {% else %}
@@ -33,19 +41,25 @@
 {% endif %}
 {% if post.user.profile.is_online %}
 {% endif %} _{_{_p_o_s_t_._u_s_e_r_._u_s_e_r_n_a_m_e_}_}
 Joined:
 {{post.user.date_joined|date:"M d, Y"}}
 Posts:
 {{post.user.profile.post_count}}
+{% if post.user.groups.all|length > 0 %}
+{% for group in post.user.groups.all %}
+{{group.name}}
+{% endfor %}
+{% endif %}
 {{post.content.rendered}}
 {% if post.user.profile.signature.rendered %}
 {{post.user.profile.signature.rendered}}
-{% endif %} {% if post.user == request.user %}
-Edit Delete
+{% endif %} {% if post|can_delete:request.user or post|can_edit:request.user %}
+{% if post|can_edit:request.user %} Edit {% endif %} {% if post|can_delete:
+request.user %} Delete {% endif %}
 {% endif %}
 {% endfor %} {% if posts.has_other_pages %}
     * {% if posts.has_previous %}
     * _P_r_e_v
     * {% else %}
     * _P_r_e_v
     * {% endif %} {% for i in posts.paginator.page_range %} {% if posts.number
@@ -54,19 +68,18 @@
     * {% else %}
     * _{_{_i_}_}
     * {% endif %} {% endfor %} {% if posts.has_next %}
     * _N_e_x_t
     * {% else %}
     * _N_e_x_t
     * {% endif %}
-{% endif %} {% if request.user.is_authenticated %} {% if not thread.is_closed
-%}
+{% endif %} {% if thread|can_post:request.user %}
 Reply to thread
 {% csrf_token %} {% for field in post_form %}
 {{ field }}
 {% endfor %} {% if post_form.non_field_errors %} {{ post_form.non_field_errors
 }} {% endif %}
 Post reply
 {% else %}
 Thread closed
 This thread is closed and you cannot reply to it.
-{% endif %} {% endif %} {% endblock %}
+{% endif %} {% endblock %}
```

### Comparing `punkweb_bb-0.1.4/punkweb_bb/templates/punkweb_bb/thread_create.html` & `punkweb_bb-0.2.0/punkweb_bb/templates/punkweb_bb/thread_create.html`

 * *Files 3% similar despite different names*

```diff
@@ -38,14 +38,15 @@
         {{ field }}
       </div>
       {% endfor %}
       {% if form.non_field_errors %}
       {{ form.non_field_errors }}
       {% endif %}
       <div class="threadForm__actions">
+        <a class="pw-button default" href="{{subcategory.get_absolute_url}}" type="submit">Cancel</a>
         <button class="pw-button raised primary" type="submit">Create Thread</button>
       </div>
     </form>
   </div>
 </div>
 
 {% endblock %}
```

#### html2text {}

```diff
@@ -6,9 +6,9 @@
     * _{_{_s_u_b_c_a_t_e_g_o_r_y_._n_a_m_e_}_}
     * Create Thread
 Create Thread
 {% csrf_token %} {% for field in form %}
 {{ field.label }} {{ field }}
 {% endfor %} {% if form.non_field_errors %} {{ form.non_field_errors }} {%
 endif %}
-Create Thread
+_C_a_n_c_e_l Create Thread
 {% endblock %} {% block extra_script %} {{form.media.js}} {% endblock %}
```

### Comparing `punkweb_bb-0.1.4/punkweb_bb/templates/punkweb_bb/thread_update.html` & `punkweb_bb-0.2.0/punkweb_bb/templates/punkweb_bb/thread_update.html`

 * *Files identical despite different names*

### Comparing `punkweb_bb-0.1.4/punkweb_bb/templatetags/__pycache__/humanize_count.cpython-311.pyc` & `punkweb_bb-0.2.0/punkweb_bb/templatetags/__pycache__/humanize_count.cpython-311.pyc`

 * *Files identical despite different names*

### Comparing `punkweb_bb-0.1.4/punkweb_bb/templatetags/__pycache__/humanize_int.cpython-311.pyc` & `punkweb_bb-0.2.0/punkweb_bb/templatetags/__pycache__/humanize_int.cpython-311.pyc`

 * *Files identical despite different names*

### Comparing `punkweb_bb-0.1.4/punkweb_bb/templatetags/__pycache__/shoutbox_bbcode.cpython-311.pyc` & `punkweb_bb-0.2.0/punkweb_bb/templatetags/__pycache__/shoutbox_bbcode.cpython-311.pyc`

 * *Files identical despite different names*

### Comparing `punkweb_bb-0.1.4/punkweb_bb/tests.py` & `punkweb_bb-0.2.0/punkweb_bb/tests.py`

 * *Files 1% similar despite different names*

```diff
@@ -470,15 +470,15 @@
         self.assertEqual(new_thread.user, self.user)
         self.assertEqual(new_thread.subcategory, self.subcategory)
 
     def test_thread_create_staff_post_only(self):
         self.client.force_login(self.user)
         response = self.client.get(self.staff_only_url)
 
-        self.assertRedirects(response, self.staff_subcategory.get_absolute_url())
+        self.assertEqual(response.status_code, 403)
 
 
 class ThreadViewTestCase(TestCase):
     def setUp(self):
         self.client = Client()
         self.user = User.objects.create_user(username="test", password="test")
         self.category = Category.objects.create(name="test")
@@ -518,15 +518,15 @@
         response = self.client.get(self.url)
 
         self.assertRedirects(response, f"{reverse('punkweb_bb:login')}?next={self.url}")
 
     def test_is_author(self):
         self.client.force_login(self.other_user)
         response = self.client.get(self.url)
-        self.assertEqual(response.status_code, 404)
+        self.assertEqual(response.status_code, 403)
 
         self.client.force_login(self.user)
         response = self.client.get(self.url)
         self.assertEqual(response.status_code, 200)
 
     def test_thread_update(self):
         self.client.force_login(self.user)
@@ -567,15 +567,15 @@
         response = self.client.get(self.url)
 
         self.assertRedirects(response, f"{reverse('punkweb_bb:login')}?next={self.url}")
 
     def test_is_author(self):
         self.client.force_login(self.other_user)
         response = self.client.get(self.url)
-        self.assertEqual(response.status_code, 404)
+        self.assertEqual(response.status_code, 403)
 
         self.client.force_login(self.user)
         response = self.client.get(self.url)
         self.assertEqual(response.status_code, 200)
 
     def test_thread_delete(self):
         self.client.force_login(self.user)
@@ -649,15 +649,15 @@
         response = self.client.get(self.url)
 
         self.assertRedirects(response, f"{reverse('punkweb_bb:login')}?next={self.url}")
 
     def test_is_author(self):
         self.client.force_login(self.other_user)
         response = self.client.get(self.url)
-        self.assertEqual(response.status_code, 404)
+        self.assertEqual(response.status_code, 403)
 
         self.client.force_login(self.user)
         response = self.client.get(self.url)
         self.assertEqual(response.status_code, 200)
 
     def test_post_update(self):
         self.client.force_login(self.user)
@@ -699,15 +699,15 @@
         response = self.client.get(self.url)
 
         self.assertRedirects(response, f"{reverse('punkweb_bb:login')}?next={self.url}")
 
     def test_is_author(self):
         self.client.force_login(self.other_user)
         response = self.client.get(self.url)
-        self.assertEqual(response.status_code, 404)
+        self.assertEqual(response.status_code, 403)
 
         self.client.force_login(self.user)
         response = self.client.get(self.url)
         self.assertEqual(response.status_code, 200)
 
     def test_post_delete(self):
         self.client.force_login(self.user)
```

### Comparing `punkweb_bb-0.1.4/punkweb_bb/urls.py` & `punkweb_bb-0.2.0/punkweb_bb/urls.py`

 * *Files 15% similar despite different names*

```diff
@@ -7,20 +7,46 @@
     path("", views.index_view, name="index"),
     path("signup/", views.signup_view, name="signup"),
     path("login/", views.login_view, name="login"),
     path("logout/", views.logout_view, name="logout"),
     path("settings/", views.settings_view, name="settings"),
     path("members/", views.members_view, name="members"),
     path("members/<path:user_id>/", views.profile_view, name="profile"),
+    path("create-category/", views.category_create_view, name="category_create"),
+    path(
+        "category/<str:category_slug>/update/",
+        views.category_update_view,
+        name="category_update",
+    ),
+    path(
+        "category/<str:category_slug>/delete/",
+        views.category_delete_view,
+        name="category_delete",
+    ),
     path(
         "subcategory/<str:subcategory_slug>/",
         views.subcategory_view,
         name="subcategory",
     ),
     path(
+        "category/<str:category_slug>/create-subcategory/",
+        views.subcategory_create_view,
+        name="subcategory_create",
+    ),
+    path(
+        "subcategory/<str:subcategory_slug>/update/",
+        views.subcategory_update_view,
+        name="subcategory_update",
+    ),
+    path(
+        "subcategory/<str:subcategory_slug>/delete/",
+        views.subcategory_delete_view,
+        name="subcategory_delete",
+    ),
+    path(
         "subcategory/<str:subcategory_slug>/create-thread/",
         views.thread_create_view,
         name="thread_create",
     ),
     path("thread/<str:thread_id>/", views.thread_view, name="thread"),
     path(
         "thread/<str:thread_id>/delete/", views.thread_delete_view, name="thread_delete"
@@ -33,9 +59,10 @@
         views.post_create_view,
         name="post_create",
     ),
     path("post/<str:post_id>/delete/", views.post_delete_view, name="post_delete"),
     path("post/<str:post_id>/update/", views.post_update_view, name="post_update"),
     path("shout-list/", views.shout_list_view, name="shout_list"),
     path("shout-create/", views.shout_create_view, name="shout_create"),
+    path("shout/<str:shout_id>/delete/", views.shout_delete_view, name="shout_delete"),
     path("bbcode/", views.bbcode_view, name="bbcode"),
 ]
```

### Comparing `punkweb_bb-0.1.4/punkweb_bb/widgets.py` & `punkweb_bb-0.2.0/punkweb_bb/widgets.py`

 * *Files identical despite different names*

### Comparing `punkweb_bb-0.1.4/punkweb_bb.egg-info/PKG-INFO` & `punkweb_bb-0.2.0/punkweb_bb.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: punkweb-bb
-Version: 0.1.4
+Version: 0.2.0
 Summary: Django application that provides a simple and modern forum board software for your Django website.
 Home-page: https://github.com/Punkweb/PunkwebBB
 Author: Punkweb
 Author-email: punkwebnet@gmail.com
 License: BSD-3-Clause
 Classifier: Environment :: Web Environment
 Classifier: Framework :: Django
@@ -18,15 +18,15 @@
 
 # PunkwebBB
 
 PunkwebBB is a Django application that provides a simple and modern forum board software for your Django website.
 
 This is the successor to [punkweb-boards](https://github.com/Punkweb/punkweb-boards).
 
-Check out [punkweb.net](https://punkweb.net/board/) for a live demo and more information!
+Check out [punkweb.net](https://punkweb.net/board/) for documentation, support and a live demonstration of the software.
 
 ## Built with
 
 - [Django](https://www.djangoproject.com/)
 - [django-precise-bbcode](https://github.com/ellmetha/django-precise-bbcode)
 - [HTMX](https://htmx.org/)
 - [jQuery](https://jquery.com/)
```

### Comparing `punkweb_bb-0.1.4/punkweb_bb.egg-info/SOURCES.txt` & `punkweb_bb-0.2.0/punkweb_bb.egg-info/SOURCES.txt`

 * *Files 6% similar despite different names*

```diff
@@ -16,14 +16,15 @@
 punkweb_bb/pagination.py
 punkweb_bb/parsers.py
 punkweb_bb/response.py
 punkweb_bb/settings.py
 punkweb_bb/signals.py
 punkweb_bb/tests.py
 punkweb_bb/urls.py
+punkweb_bb/utils.py
 punkweb_bb/views.py
 punkweb_bb/widgets.py
 punkweb_bb.egg-info/PKG-INFO
 punkweb_bb.egg-info/SOURCES.txt
 punkweb_bb.egg-info/dependency_links.txt
 punkweb_bb.egg-info/not-zip-safe
 punkweb_bb.egg-info/requires.txt
@@ -42,33 +43,36 @@
 punkweb_bb/__pycache__/pagination.cpython-311.pyc
 punkweb_bb/__pycache__/parsers.cpython-311.pyc
 punkweb_bb/__pycache__/response.cpython-311.pyc
 punkweb_bb/__pycache__/settings.cpython-311.pyc
 punkweb_bb/__pycache__/signals.cpython-311.pyc
 punkweb_bb/__pycache__/tests.cpython-311.pyc
 punkweb_bb/__pycache__/urls.cpython-311.pyc
+punkweb_bb/__pycache__/utils.cpython-311.pyc
 punkweb_bb/__pycache__/views.cpython-311.pyc
 punkweb_bb/__pycache__/widgets.cpython-311.pyc
 punkweb_bb/migrations/0001_initial.py
 punkweb_bb/migrations/0002_thread_view_count.py
 punkweb_bb/migrations/__init__.py
 punkweb_bb/migrations/__pycache__/0001_initial.cpython-311.pyc
 punkweb_bb/migrations/__pycache__/0002_thread_view_count.cpython-311.pyc
 punkweb_bb/migrations/__pycache__/__init__.cpython-311.pyc
 punkweb_bb/static/punkweb_bb/favicon.ico
+punkweb_bb/static/punkweb_bb/css/category-form.css
 punkweb_bb/static/punkweb_bb/css/defaults.css
 punkweb_bb/static/punkweb_bb/css/index.css
 punkweb_bb/static/punkweb_bb/css/login.css
 punkweb_bb/static/punkweb_bb/css/members.css
 punkweb_bb/static/punkweb_bb/css/post-form.css
 punkweb_bb/static/punkweb_bb/css/profile.css
 punkweb_bb/static/punkweb_bb/css/punkweb-modal.css
 punkweb_bb/static/punkweb_bb/css/punkweb.css
 punkweb_bb/static/punkweb_bb/css/settings.css
 punkweb_bb/static/punkweb_bb/css/shoutbox.css
+punkweb_bb/static/punkweb_bb/css/subcategory-form.css
 punkweb_bb/static/punkweb_bb/css/subcategory.css
 punkweb_bb/static/punkweb_bb/css/thread-form.css
 punkweb_bb/static/punkweb_bb/css/thread.css
 punkweb_bb/static/punkweb_bb/css/typography.css
 punkweb_bb/static/punkweb_bb/css/variables.css
 punkweb_bb/static/punkweb_bb/editor/bbcode-editor-content.css
 punkweb_bb/static/punkweb_bb/editor/bbcode-editor-tags.js
@@ -199,29 +203,42 @@
 punkweb_bb/static/punkweb_bb/vendor/sceditor-3.2.0/minified/themes/office-toolbar.min.css
 punkweb_bb/static/punkweb_bb/vendor/sceditor-3.2.0/minified/themes/office.min.css
 punkweb_bb/static/punkweb_bb/vendor/sceditor-3.2.0/minified/themes/square.min.css
 punkweb_bb/static/punkweb_bb/vendor/sceditor-3.2.0/minified/themes/content/default.min.css
 punkweb_bb/templates/punkweb_bb/base.html
 punkweb_bb/templates/punkweb_bb/base_modal.html
 punkweb_bb/templates/punkweb_bb/bbcode.html
+punkweb_bb/templates/punkweb_bb/category_create.html
+punkweb_bb/templates/punkweb_bb/category_update.html
 punkweb_bb/templates/punkweb_bb/index.html
 punkweb_bb/templates/punkweb_bb/login.html
 punkweb_bb/templates/punkweb_bb/members.html
 punkweb_bb/templates/punkweb_bb/profile.html
 punkweb_bb/templates/punkweb_bb/settings.html
 punkweb_bb/templates/punkweb_bb/signup.html
 punkweb_bb/templates/punkweb_bb/subcategory.html
+punkweb_bb/templates/punkweb_bb/subcategory_create.html
+punkweb_bb/templates/punkweb_bb/subcategory_update.html
 punkweb_bb/templates/punkweb_bb/thread.html
 punkweb_bb/templates/punkweb_bb/thread_create.html
 punkweb_bb/templates/punkweb_bb/thread_update.html
+punkweb_bb/templates/punkweb_bb/partials/category_delete.html
 punkweb_bb/templates/punkweb_bb/partials/post_delete.html
 punkweb_bb/templates/punkweb_bb/partials/post_update.html
+punkweb_bb/templates/punkweb_bb/partials/shout_delete.html
+punkweb_bb/templates/punkweb_bb/partials/subcategory_delete.html
 punkweb_bb/templates/punkweb_bb/partials/thread_delete.html
 punkweb_bb/templates/punkweb_bb/shoutbox/shout_list.html
 punkweb_bb/templates/punkweb_bb/shoutbox/shoutbox.html
 punkweb_bb/templatetags/__init__.py
+punkweb_bb/templatetags/can_delete.py
+punkweb_bb/templatetags/can_edit.py
+punkweb_bb/templatetags/can_post.py
 punkweb_bb/templatetags/humanize_int.py
 punkweb_bb/templatetags/shoutbox_bbcode.py
 punkweb_bb/templatetags/__pycache__/__init__.cpython-311.pyc
+punkweb_bb/templatetags/__pycache__/can_delete.cpython-311.pyc
+punkweb_bb/templatetags/__pycache__/can_edit.cpython-311.pyc
+punkweb_bb/templatetags/__pycache__/can_post.cpython-311.pyc
 punkweb_bb/templatetags/__pycache__/humanize_count.cpython-311.pyc
 punkweb_bb/templatetags/__pycache__/humanize_int.cpython-311.pyc
 punkweb_bb/templatetags/__pycache__/shoutbox_bbcode.cpython-311.pyc
```

### Comparing `punkweb_bb-0.1.4/setup.py` & `punkweb_bb-0.2.0/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from setuptools import setup
 
 setup(
     name="punkweb_bb",
-    version="0.1.4",
+    version="0.2.0",
     author="Punkweb",
     author_email="punkwebnet@gmail.com",
     packages=["punkweb_bb"],
     url="https://github.com/Punkweb/PunkwebBB",
     license="BSD-3-Clause",
     description="Django application that provides a simple and modern forum board software for your Django website.",
     long_description=open("README.md").read(),
```

