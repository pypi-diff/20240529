# Comparing `tmp/punkweb_bb-0.2.0.tar.gz` & `tmp/punkweb_bb-0.2.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "punkweb_bb-0.2.0.tar", last modified: Tue May 28 23:00:59 2024, max compression
+gzip compressed data, was "punkweb_bb-0.2.1.tar", last modified: Wed May 29 04:58:56 2024, max compression
```

## Comparing `punkweb_bb-0.2.0.tar` & `punkweb_bb-0.2.1.tar`

### file list

```diff
@@ -1,280 +1,282 @@
-drwxr-xr-x   0 pork      (1000) pork      (1000)        0 2024-05-28 23:00:59.976560 punkweb_bb-0.2.0/
--rw-r--r--   0 pork      (1000) pork      (1000)     1507 2024-04-09 06:08:41.000000 punkweb_bb-0.2.0/LICENSE
--rw-r--r--   0 pork      (1000) pork      (1000)       64 2024-04-09 05:47:19.000000 punkweb_bb-0.2.0/MANIFEST.in
--rw-r--r--   0 pork      (1000) pork      (1000)     5023 2024-05-28 23:00:59.976560 punkweb_bb-0.2.0/PKG-INFO
--rw-r--r--   0 pork      (1000) pork      (1000)     4369 2024-05-09 06:47:11.000000 punkweb_bb-0.2.0/README.md
-drwxr-xr-x   0 pork      (1000) pork      (1000)        0 2024-05-28 23:00:59.964560 punkweb_bb-0.2.0/punkweb_bb/
--rw-r--r--   0 pork      (1000) pork      (1000)        0 2023-08-20 16:04:51.000000 punkweb_bb-0.2.0/punkweb_bb/__init__.py
-drwxr-xr-x   0 pork      (1000) pork      (1000)        0 2024-05-28 23:00:59.964560 punkweb_bb-0.2.0/punkweb_bb/__pycache__/
--rw-r--r--   0 pork      (1000) pork      (1000)      161 2024-04-09 05:48:25.000000 punkweb_bb-0.2.0/punkweb_bb/__pycache__/__init__.cpython-311.pyc
--rw-r--r--   0 pork      (1000) pork      (1000)     3679 2024-04-09 05:48:25.000000 punkweb_bb-0.2.0/punkweb_bb/__pycache__/admin.cpython-311.pyc
--rw-r--r--   0 pork      (1000) pork      (1000)     2980 2024-04-09 05:48:25.000000 punkweb_bb-0.2.0/punkweb_bb/__pycache__/admin_forms.cpython-311.pyc
--rw-r--r--   0 pork      (1000) pork      (1000)      730 2024-04-09 06:55:15.000000 punkweb_bb-0.2.0/punkweb_bb/__pycache__/apps.cpython-311.pyc
--rw-r--r--   0 pork      (1000) pork      (1000)     8534 2024-04-09 06:32:38.000000 punkweb_bb-0.2.0/punkweb_bb/__pycache__/bbcode_tags.cpython-311.pyc
--rw-r--r--   0 pork      (1000) pork      (1000)      392 2024-04-09 06:44:27.000000 punkweb_bb-0.2.0/punkweb_bb/__pycache__/context_processors.cpython-311.pyc
--rw-r--r--   0 pork      (1000) pork      (1000)     6194 2024-05-28 21:39:20.000000 punkweb_bb-0.2.0/punkweb_bb/__pycache__/forms.cpython-311.pyc
--rw-r--r--   0 pork      (1000) pork      (1000)     1581 2024-05-09 05:36:59.000000 punkweb_bb-0.2.0/punkweb_bb/__pycache__/guests.cpython-311.pyc
--rw-r--r--   0 pork      (1000) pork      (1000)     1560 2024-05-09 05:37:45.000000 punkweb_bb-0.2.0/punkweb_bb/__pycache__/middleware.cpython-311.pyc
--rw-r--r--   0 pork      (1000) pork      (1000)     1478 2024-04-09 05:48:25.000000 punkweb_bb-0.2.0/punkweb_bb/__pycache__/mixins.cpython-311.pyc
--rw-r--r--   0 pork      (1000) pork      (1000)    13824 2024-05-28 22:54:03.000000 punkweb_bb-0.2.0/punkweb_bb/__pycache__/models.cpython-311.pyc
--rw-r--r--   0 pork      (1000) pork      (1000)      990 2024-04-09 05:48:25.000000 punkweb_bb-0.2.0/punkweb_bb/__pycache__/pagination.cpython-311.pyc
--rw-r--r--   0 pork      (1000) pork      (1000)     5335 2024-04-09 07:07:59.000000 punkweb_bb-0.2.0/punkweb_bb/__pycache__/parsers.cpython-311.pyc
--rw-r--r--   0 pork      (1000) pork      (1000)      448 2024-04-09 05:48:25.000000 punkweb_bb-0.2.0/punkweb_bb/__pycache__/response.cpython-311.pyc
--rw-r--r--   0 pork      (1000) pork      (1000)      947 2024-05-09 05:27:51.000000 punkweb_bb-0.2.0/punkweb_bb/__pycache__/settings.cpython-311.pyc
--rw-r--r--   0 pork      (1000) pork      (1000)      864 2024-04-09 05:48:25.000000 punkweb_bb-0.2.0/punkweb_bb/__pycache__/signals.cpython-311.pyc
--rw-r--r--   0 pork      (1000) pork      (1000)    51768 2024-05-28 21:35:15.000000 punkweb_bb-0.2.0/punkweb_bb/__pycache__/tests.cpython-311.pyc
--rw-r--r--   0 pork      (1000) pork      (1000)     3322 2024-05-28 20:10:30.000000 punkweb_bb-0.2.0/punkweb_bb/__pycache__/urls.cpython-311.pyc
--rw-r--r--   0 pork      (1000) pork      (1000)      748 2024-05-28 21:07:24.000000 punkweb_bb-0.2.0/punkweb_bb/__pycache__/utils.cpython-311.pyc
--rw-r--r--   0 pork      (1000) pork      (1000)    23918 2024-05-28 22:09:45.000000 punkweb_bb-0.2.0/punkweb_bb/__pycache__/views.cpython-311.pyc
--rw-r--r--   0 pork      (1000) pork      (1000)     1552 2024-04-09 05:48:25.000000 punkweb_bb-0.2.0/punkweb_bb/__pycache__/widgets.cpython-311.pyc
--rw-r--r--   0 pork      (1000) pork      (1000)     2493 2024-04-05 21:20:18.000000 punkweb_bb-0.2.0/punkweb_bb/admin.py
--rw-r--r--   0 pork      (1000) pork      (1000)     1128 2024-04-03 19:18:44.000000 punkweb_bb-0.2.0/punkweb_bb/admin_forms.py
--rw-r--r--   0 pork      (1000) pork      (1000)      207 2024-04-09 06:52:38.000000 punkweb_bb-0.2.0/punkweb_bb/apps.py
--rw-r--r--   0 pork      (1000) pork      (1000)     4419 2024-04-09 06:31:31.000000 punkweb_bb-0.2.0/punkweb_bb/bbcode_tags.py
--rw-r--r--   0 pork      (1000) pork      (1000)      146 2024-04-09 04:54:41.000000 punkweb_bb-0.2.0/punkweb_bb/context_processors.py
--rw-r--r--   0 pork      (1000) pork      (1000)     2907 2024-05-28 21:39:19.000000 punkweb_bb-0.2.0/punkweb_bb/forms.py
--rw-r--r--   0 pork      (1000) pork      (1000)      467 2024-05-09 05:36:58.000000 punkweb_bb-0.2.0/punkweb_bb/guests.py
--rw-r--r--   0 pork      (1000) pork      (1000)      628 2024-05-09 05:37:44.000000 punkweb_bb-0.2.0/punkweb_bb/middleware.py
-drwxr-xr-x   0 pork      (1000) pork      (1000)        0 2024-05-28 23:00:59.964560 punkweb_bb-0.2.0/punkweb_bb/migrations/
--rw-r--r--   0 pork      (1000) pork      (1000)     8950 2024-04-09 07:09:02.000000 punkweb_bb-0.2.0/punkweb_bb/migrations/0001_initial.py
--rw-r--r--   0 pork      (1000) pork      (1000)      388 2024-05-07 04:24:13.000000 punkweb_bb-0.2.0/punkweb_bb/migrations/0002_thread_view_count.py
--rw-r--r--   0 pork      (1000) pork      (1000)        0 2023-08-20 16:04:51.000000 punkweb_bb-0.2.0/punkweb_bb/migrations/__init__.py
-drwxr-xr-x   0 pork      (1000) pork      (1000)        0 2024-05-28 23:00:59.964560 punkweb_bb-0.2.0/punkweb_bb/migrations/__pycache__/
--rw-r--r--   0 pork      (1000) pork      (1000)     6456 2024-04-09 07:09:10.000000 punkweb_bb-0.2.0/punkweb_bb/migrations/__pycache__/0001_initial.cpython-311.pyc
--rw-r--r--   0 pork      (1000) pork      (1000)      815 2024-05-07 04:24:16.000000 punkweb_bb-0.2.0/punkweb_bb/migrations/__pycache__/0002_thread_view_count.cpython-311.pyc
--rw-r--r--   0 pork      (1000) pork      (1000)      172 2024-04-09 05:48:25.000000 punkweb_bb-0.2.0/punkweb_bb/migrations/__pycache__/__init__.cpython-311.pyc
--rw-r--r--   0 pork      (1000) pork      (1000)      395 2024-04-03 19:16:01.000000 punkweb_bb-0.2.0/punkweb_bb/mixins.py
--rw-r--r--   0 pork      (1000) pork      (1000)     6218 2024-05-28 22:54:01.000000 punkweb_bb-0.2.0/punkweb_bb/models.py
--rw-r--r--   0 pork      (1000) pork      (1000)      409 2024-04-06 08:06:22.000000 punkweb_bb-0.2.0/punkweb_bb/pagination.py
--rw-r--r--   0 pork      (1000) pork      (1000)     2732 2024-04-09 07:07:58.000000 punkweb_bb-0.2.0/punkweb_bb/parsers.py
--rw-r--r--   0 pork      (1000) pork      (1000)      130 2024-04-03 19:15:29.000000 punkweb_bb-0.2.0/punkweb_bb/response.py
--rw-r--r--   0 pork      (1000) pork      (1000)      517 2024-05-09 05:27:49.000000 punkweb_bb-0.2.0/punkweb_bb/settings.py
--rw-r--r--   0 pork      (1000) pork      (1000)      365 2024-04-03 19:18:44.000000 punkweb_bb-0.2.0/punkweb_bb/signals.py
-drwxr-xr-x   0 pork      (1000) pork      (1000)        0 2024-05-28 23:00:59.964560 punkweb_bb-0.2.0/punkweb_bb/static/
-drwxr-xr-x   0 pork      (1000) pork      (1000)        0 2024-05-28 23:00:59.964560 punkweb_bb-0.2.0/punkweb_bb/static/punkweb_bb/
-drwxr-xr-x   0 pork      (1000) pork      (1000)        0 2024-05-28 23:00:59.968560 punkweb_bb-0.2.0/punkweb_bb/static/punkweb_bb/css/
--rw-r--r--   0 pork      (1000) pork      (1000)      359 2024-05-28 20:15:52.000000 punkweb_bb-0.2.0/punkweb_bb/static/punkweb_bb/css/category-form.css
--rw-r--r--   0 pork      (1000) pork      (1000)     1455 2024-04-06 07:32:15.000000 punkweb_bb-0.2.0/punkweb_bb/static/punkweb_bb/css/defaults.css
--rw-r--r--   0 pork      (1000) pork      (1000)     1418 2024-05-28 22:37:20.000000 punkweb_bb-0.2.0/punkweb_bb/static/punkweb_bb/css/index.css
--rw-r--r--   0 pork      (1000) pork      (1000)      234 2024-04-03 22:23:23.000000 punkweb_bb-0.2.0/punkweb_bb/static/punkweb_bb/css/login.css
--rw-r--r--   0 pork      (1000) pork      (1000)      395 2024-04-08 22:57:27.000000 punkweb_bb-0.2.0/punkweb_bb/static/punkweb_bb/css/members.css
--rw-r--r--   0 pork      (1000) pork      (1000)      321 2024-04-03 21:47:53.000000 punkweb_bb-0.2.0/punkweb_bb/static/punkweb_bb/css/post-form.css
--rw-r--r--   0 pork      (1000) pork      (1000)      916 2024-05-07 01:46:57.000000 punkweb_bb-0.2.0/punkweb_bb/static/punkweb_bb/css/profile.css
--rw-r--r--   0 pork      (1000) pork      (1000)     1296 2024-04-05 22:11:56.000000 punkweb_bb-0.2.0/punkweb_bb/static/punkweb_bb/css/punkweb-modal.css
--rw-r--r--   0 pork      (1000) pork      (1000)    12678 2024-05-28 22:41:43.000000 punkweb_bb-0.2.0/punkweb_bb/static/punkweb_bb/css/punkweb.css
--rw-r--r--   0 pork      (1000) pork      (1000)      308 2024-04-06 07:53:29.000000 punkweb_bb-0.2.0/punkweb_bb/static/punkweb_bb/css/settings.css
--rw-r--r--   0 pork      (1000) pork      (1000)      536 2024-05-28 21:51:42.000000 punkweb_bb-0.2.0/punkweb_bb/static/punkweb_bb/css/shoutbox.css
--rw-r--r--   0 pork      (1000) pork      (1000)      371 2024-05-28 20:14:48.000000 punkweb_bb-0.2.0/punkweb_bb/static/punkweb_bb/css/subcategory-form.css
--rw-r--r--   0 pork      (1000) pork      (1000)      711 2024-05-28 20:02:41.000000 punkweb_bb-0.2.0/punkweb_bb/static/punkweb_bb/css/subcategory.css
--rw-r--r--   0 pork      (1000) pork      (1000)      329 2024-04-03 19:20:08.000000 punkweb_bb-0.2.0/punkweb_bb/static/punkweb_bb/css/thread-form.css
--rw-r--r--   0 pork      (1000) pork      (1000)     1870 2024-05-28 22:52:41.000000 punkweb_bb-0.2.0/punkweb_bb/static/punkweb_bb/css/thread.css
--rw-r--r--   0 pork      (1000) pork      (1000)      448 2024-04-05 15:05:58.000000 punkweb_bb-0.2.0/punkweb_bb/static/punkweb_bb/css/typography.css
--rw-r--r--   0 pork      (1000) pork      (1000)     1193 2024-05-28 22:52:14.000000 punkweb_bb-0.2.0/punkweb_bb/static/punkweb_bb/css/variables.css
-drwxr-xr-x   0 pork      (1000) pork      (1000)        0 2024-05-28 23:00:59.968560 punkweb_bb-0.2.0/punkweb_bb/static/punkweb_bb/editor/
--rw-r--r--   0 pork      (1000) pork      (1000)     1466 2024-04-06 07:32:28.000000 punkweb_bb-0.2.0/punkweb_bb/static/punkweb_bb/editor/bbcode-editor-content.css
--rw-r--r--   0 pork      (1000) pork      (1000)     1624 2024-04-03 19:20:08.000000 punkweb_bb-0.2.0/punkweb_bb/static/punkweb_bb/editor/bbcode-editor-tags.js
--rw-r--r--   0 pork      (1000) pork      (1000)        0 2024-04-03 19:20:08.000000 punkweb_bb-0.2.0/punkweb_bb/static/punkweb_bb/editor/bbcode-editor.css
--rw-r--r--   0 pork      (1000) pork      (1000)      606 2024-04-08 22:10:44.000000 punkweb_bb-0.2.0/punkweb_bb/static/punkweb_bb/editor/bbcode-editor.js
--rw-r--r--   0 pork      (1000) pork      (1000)      318 2024-04-03 19:11:51.000000 punkweb_bb-0.2.0/punkweb_bb/static/punkweb_bb/favicon.ico
-drwxr-xr-x   0 pork      (1000) pork      (1000)        0 2024-05-28 23:00:59.968560 punkweb_bb-0.2.0/punkweb_bb/static/punkweb_bb/img/
--rw-r--r--   0 pork      (1000) pork      (1000)    60475 2024-04-03 19:20:08.000000 punkweb_bb-0.2.0/punkweb_bb/static/punkweb_bb/img/default-profile-image.png
-drwxr-xr-x   0 pork      (1000) pork      (1000)        0 2024-05-28 23:00:59.968560 punkweb_bb-0.2.0/punkweb_bb/static/punkweb_bb/js/
--rw-r--r--   0 pork      (1000) pork      (1000)      179 2024-04-03 19:20:08.000000 punkweb_bb-0.2.0/punkweb_bb/static/punkweb_bb/js/punkweb-modal.js
--rw-r--r--   0 pork      (1000) pork      (1000)      142 2024-04-08 20:20:47.000000 punkweb_bb-0.2.0/punkweb_bb/static/punkweb_bb/js/shoutbox.js
-drwxr-xr-x   0 pork      (1000) pork      (1000)        0 2024-05-28 23:00:59.968560 punkweb_bb-0.2.0/punkweb_bb/static/punkweb_bb/vendor/
--rw-r--r--   0 pork      (1000) pork      (1000)    44307 2024-04-03 19:17:23.000000 punkweb_bb-0.2.0/punkweb_bb/static/punkweb_bb/vendor/htmx-1.9.4.min.js
--rw-r--r--   0 pork      (1000) pork      (1000)    87461 2024-04-03 19:11:51.000000 punkweb_bb-0.2.0/punkweb_bb/static/punkweb_bb/vendor/jquery-3.7.0.min.js
--rw-r--r--   0 pork      (1000) pork      (1000)    10331 2024-04-03 19:11:51.000000 punkweb_bb-0.2.0/punkweb_bb/static/punkweb_bb/vendor/open-color.css
--rw-r--r--   0 pork      (1000) pork      (1000)     3948 2024-04-03 19:11:51.000000 punkweb_bb-0.2.0/punkweb_bb/static/punkweb_bb/vendor/prism.css
--rw-r--r--   0 pork      (1000) pork      (1000)   576492 2024-04-03 19:11:51.000000 punkweb_bb-0.2.0/punkweb_bb/static/punkweb_bb/vendor/prism.js
-drwxr-xr-x   0 pork      (1000) pork      (1000)        0 2024-05-28 23:00:59.968560 punkweb_bb-0.2.0/punkweb_bb/static/punkweb_bb/vendor/sceditor-3.2.0/
--rw-r--r--   0 pork      (1000) pork      (1000)     4129 2024-04-03 19:11:51.000000 punkweb_bb-0.2.0/punkweb_bb/static/punkweb_bb/vendor/sceditor-3.2.0/README.md
-drwxr-xr-x   0 pork      (1000) pork      (1000)        0 2024-05-28 23:00:59.968560 punkweb_bb-0.2.0/punkweb_bb/static/punkweb_bb/vendor/sceditor-3.2.0/development/
-drwxr-xr-x   0 pork      (1000) pork      (1000)        0 2024-05-28 23:00:59.968560 punkweb_bb-0.2.0/punkweb_bb/static/punkweb_bb/vendor/sceditor-3.2.0/development/formats/
--rw-r--r--   0 pork      (1000) pork      (1000)    61679 2024-04-03 19:11:51.000000 punkweb_bb-0.2.0/punkweb_bb/static/punkweb_bb/vendor/sceditor-3.2.0/development/formats/bbcode.js
--rw-r--r--   0 pork      (1000) pork      (1000)    26086 2024-04-03 19:11:51.000000 punkweb_bb-0.2.0/punkweb_bb/static/punkweb_bb/vendor/sceditor-3.2.0/development/formats/xhtml.js
-drwxr-xr-x   0 pork      (1000) pork      (1000)        0 2024-05-28 23:00:59.968560 punkweb_bb-0.2.0/punkweb_bb/static/punkweb_bb/vendor/sceditor-3.2.0/development/icons/
--rw-r--r--   0 pork      (1000) pork      (1000)    11260 2024-04-03 19:11:51.000000 punkweb_bb-0.2.0/punkweb_bb/static/punkweb_bb/vendor/sceditor-3.2.0/development/icons/material.js
--rw-r--r--   0 pork      (1000) pork      (1000)    15873 2024-04-03 19:11:51.000000 punkweb_bb-0.2.0/punkweb_bb/static/punkweb_bb/vendor/sceditor-3.2.0/development/icons/monocons.js
--rw-r--r--   0 pork      (1000) pork      (1000)   312959 2024-04-03 19:11:51.000000 punkweb_bb-0.2.0/punkweb_bb/static/punkweb_bb/vendor/sceditor-3.2.0/development/jquery.sceditor.bbcode.js
--rw-r--r--   0 pork      (1000) pork      (1000)   251279 2024-04-03 19:11:51.000000 punkweb_bb-0.2.0/punkweb_bb/static/punkweb_bb/vendor/sceditor-3.2.0/development/jquery.sceditor.js
--rw-r--r--   0 pork      (1000) pork      (1000)   277366 2024-04-03 19:11:51.000000 punkweb_bb-0.2.0/punkweb_bb/static/punkweb_bb/vendor/sceditor-3.2.0/development/jquery.sceditor.xhtml.js
-drwxr-xr-x   0 pork      (1000) pork      (1000)        0 2024-05-28 23:00:59.968560 punkweb_bb-0.2.0/punkweb_bb/static/punkweb_bb/vendor/sceditor-3.2.0/development/plugins/
--rw-r--r--   0 pork      (1000) pork      (1000)     3446 2024-04-03 19:11:51.000000 punkweb_bb-0.2.0/punkweb_bb/static/punkweb_bb/vendor/sceditor-3.2.0/development/plugins/alternative-lists.js
--rw-r--r--   0 pork      (1000) pork      (1000)     2571 2024-04-03 19:11:51.000000 punkweb_bb-0.2.0/punkweb_bb/static/punkweb_bb/vendor/sceditor-3.2.0/development/plugins/autosave.js
--rw-r--r--   0 pork      (1000) pork      (1000)     2791 2024-04-03 19:11:51.000000 punkweb_bb-0.2.0/punkweb_bb/static/punkweb_bb/vendor/sceditor-3.2.0/development/plugins/autoyoutube.js
--rw-r--r--   0 pork      (1000) pork      (1000)     6306 2024-04-03 19:11:51.000000 punkweb_bb-0.2.0/punkweb_bb/static/punkweb_bb/vendor/sceditor-3.2.0/development/plugins/dragdrop.js
--rw-r--r--   0 pork      (1000) pork      (1000)     2528 2024-04-03 19:11:51.000000 punkweb_bb-0.2.0/punkweb_bb/static/punkweb_bb/vendor/sceditor-3.2.0/development/plugins/format.js
--rw-r--r--   0 pork      (1000) pork      (1000)     2059 2024-04-03 19:11:51.000000 punkweb_bb-0.2.0/punkweb_bb/static/punkweb_bb/vendor/sceditor-3.2.0/development/plugins/plaintext.js
--rw-r--r--   0 pork      (1000) pork      (1000)     9375 2024-04-03 19:11:51.000000 punkweb_bb-0.2.0/punkweb_bb/static/punkweb_bb/vendor/sceditor-3.2.0/development/plugins/undo.js
--rw-r--r--   0 pork      (1000) pork      (1000)     2067 2024-04-03 19:11:51.000000 punkweb_bb-0.2.0/punkweb_bb/static/punkweb_bb/vendor/sceditor-3.2.0/development/plugins/v1compat.js
--rw-r--r--   0 pork      (1000) pork      (1000)   249123 2024-04-03 19:11:51.000000 punkweb_bb-0.2.0/punkweb_bb/static/punkweb_bb/vendor/sceditor-3.2.0/development/sceditor.js
-drwxr-xr-x   0 pork      (1000) pork      (1000)        0 2024-05-28 23:00:59.968560 punkweb_bb-0.2.0/punkweb_bb/static/punkweb_bb/vendor/sceditor-3.2.0/development/themes/
-drwxr-xr-x   0 pork      (1000) pork      (1000)        0 2024-05-28 23:00:59.968560 punkweb_bb-0.2.0/punkweb_bb/static/punkweb_bb/vendor/sceditor-3.2.0/development/themes/content/
--rw-r--r--   0 pork      (1000) pork      (1000)     1476 2024-04-03 19:11:51.000000 punkweb_bb-0.2.0/punkweb_bb/static/punkweb_bb/vendor/sceditor-3.2.0/development/themes/content/default.css
--rw-r--r--   0 pork      (1000) pork      (1000)    11194 2024-04-03 19:11:51.000000 punkweb_bb-0.2.0/punkweb_bb/static/punkweb_bb/vendor/sceditor-3.2.0/development/themes/default.css
--rw-r--r--   0 pork      (1000) pork      (1000)    11500 2024-04-03 19:11:51.000000 punkweb_bb-0.2.0/punkweb_bb/static/punkweb_bb/vendor/sceditor-3.2.0/development/themes/defaultdark.css
--rw-r--r--   0 pork      (1000) pork      (1000)     4583 2024-04-03 19:11:51.000000 punkweb_bb-0.2.0/punkweb_bb/static/punkweb_bb/vendor/sceditor-3.2.0/development/themes/famfamfam.png
--rw-r--r--   0 pork      (1000) pork      (1000)    12943 2024-04-03 19:11:51.000000 punkweb_bb-0.2.0/punkweb_bb/static/punkweb_bb/vendor/sceditor-3.2.0/development/themes/modern.css
--rw-r--r--   0 pork      (1000) pork      (1000)    13431 2024-04-03 19:11:51.000000 punkweb_bb-0.2.0/punkweb_bb/static/punkweb_bb/vendor/sceditor-3.2.0/development/themes/office-toolbar.css
--rw-r--r--   0 pork      (1000) pork      (1000)    14124 2024-04-03 19:11:51.000000 punkweb_bb-0.2.0/punkweb_bb/static/punkweb_bb/vendor/sceditor-3.2.0/development/themes/office.css
--rw-r--r--   0 pork      (1000) pork      (1000)    13183 2024-04-03 19:11:51.000000 punkweb_bb-0.2.0/punkweb_bb/static/punkweb_bb/vendor/sceditor-3.2.0/development/themes/square.css
-drwxr-xr-x   0 pork      (1000) pork      (1000)        0 2024-05-28 23:00:59.972560 punkweb_bb-0.2.0/punkweb_bb/static/punkweb_bb/vendor/sceditor-3.2.0/emoticons/
--rw-r--r--   0 pork      (1000) pork      (1000)      756 2024-04-03 19:11:51.000000 punkweb_bb-0.2.0/punkweb_bb/static/punkweb_bb/vendor/sceditor-3.2.0/emoticons/alien.png
--rw-r--r--   0 pork      (1000) pork      (1000)     1182 2024-04-03 19:11:51.000000 punkweb_bb-0.2.0/punkweb_bb/static/punkweb_bb/vendor/sceditor-3.2.0/emoticons/angel.png
--rw-r--r--   0 pork      (1000) pork      (1000)      781 2024-04-03 19:11:51.000000 punkweb_bb-0.2.0/punkweb_bb/static/punkweb_bb/vendor/sceditor-3.2.0/emoticons/angry.png
--rw-r--r--   0 pork      (1000) pork      (1000)      972 2024-04-03 19:11:51.000000 punkweb_bb-0.2.0/punkweb_bb/static/punkweb_bb/vendor/sceditor-3.2.0/emoticons/blink.png
--rw-r--r--   0 pork      (1000) pork      (1000)      865 2024-04-03 19:11:51.000000 punkweb_bb-0.2.0/punkweb_bb/static/punkweb_bb/vendor/sceditor-3.2.0/emoticons/blush.png
--rw-r--r--   0 pork      (1000) pork      (1000)      753 2024-04-03 19:11:51.000000 punkweb_bb-0.2.0/punkweb_bb/static/punkweb_bb/vendor/sceditor-3.2.0/emoticons/cheerful.png
--rw-r--r--   0 pork      (1000) pork      (1000)      965 2024-04-03 19:11:51.000000 punkweb_bb-0.2.0/punkweb_bb/static/punkweb_bb/vendor/sceditor-3.2.0/emoticons/cool.png
--rw-r--r--   0 pork      (1000) pork      (1000)      421 2024-04-03 19:11:51.000000 punkweb_bb-0.2.0/punkweb_bb/static/punkweb_bb/vendor/sceditor-3.2.0/emoticons/credits.txt
--rw-r--r--   0 pork      (1000) pork      (1000)      877 2024-04-03 19:11:51.000000 punkweb_bb-0.2.0/punkweb_bb/static/punkweb_bb/vendor/sceditor-3.2.0/emoticons/cwy.png
--rw-r--r--   0 pork      (1000) pork      (1000)     1012 2024-04-03 19:11:51.000000 punkweb_bb-0.2.0/punkweb_bb/static/punkweb_bb/vendor/sceditor-3.2.0/emoticons/devil.png
--rw-r--r--   0 pork      (1000) pork      (1000)      991 2024-04-03 19:11:51.000000 punkweb_bb-0.2.0/punkweb_bb/static/punkweb_bb/vendor/sceditor-3.2.0/emoticons/dizzy.png
--rw-r--r--   0 pork      (1000) pork      (1000)      983 2024-04-03 19:11:51.000000 punkweb_bb-0.2.0/punkweb_bb/static/punkweb_bb/vendor/sceditor-3.2.0/emoticons/ermm.png
--rw-r--r--   0 pork      (1000) pork      (1000)      793 2024-04-03 19:11:51.000000 punkweb_bb-0.2.0/punkweb_bb/static/punkweb_bb/vendor/sceditor-3.2.0/emoticons/face.png
--rw-r--r--   0 pork      (1000) pork      (1000)      792 2024-04-03 19:11:51.000000 punkweb_bb-0.2.0/punkweb_bb/static/punkweb_bb/vendor/sceditor-3.2.0/emoticons/getlost.png
--rw-r--r--   0 pork      (1000) pork      (1000)      867 2024-04-03 19:11:51.000000 punkweb_bb-0.2.0/punkweb_bb/static/punkweb_bb/vendor/sceditor-3.2.0/emoticons/grin.png
--rw-r--r--   0 pork      (1000) pork      (1000)      792 2024-04-03 19:11:51.000000 punkweb_bb-0.2.0/punkweb_bb/static/punkweb_bb/vendor/sceditor-3.2.0/emoticons/happy.png
--rw-r--r--   0 pork      (1000) pork      (1000)      572 2024-04-03 19:11:51.000000 punkweb_bb-0.2.0/punkweb_bb/static/punkweb_bb/vendor/sceditor-3.2.0/emoticons/heart.png
--rw-r--r--   0 pork      (1000) pork      (1000)      793 2024-04-03 19:11:51.000000 punkweb_bb-0.2.0/punkweb_bb/static/punkweb_bb/vendor/sceditor-3.2.0/emoticons/kissing.png
--rw-r--r--   0 pork      (1000) pork      (1000)      912 2024-04-03 19:11:51.000000 punkweb_bb-0.2.0/punkweb_bb/static/punkweb_bb/vendor/sceditor-3.2.0/emoticons/laughing.png
--rw-r--r--   0 pork      (1000) pork      (1000)      694 2024-04-03 19:11:51.000000 punkweb_bb-0.2.0/punkweb_bb/static/punkweb_bb/vendor/sceditor-3.2.0/emoticons/ninja.png
--rw-r--r--   0 pork      (1000) pork      (1000)      804 2024-04-03 19:11:51.000000 punkweb_bb-0.2.0/punkweb_bb/static/punkweb_bb/vendor/sceditor-3.2.0/emoticons/pinch.png
--rw-r--r--   0 pork      (1000) pork      (1000)      799 2024-04-03 19:11:51.000000 punkweb_bb-0.2.0/punkweb_bb/static/punkweb_bb/vendor/sceditor-3.2.0/emoticons/pouty.png
--rw-r--r--   0 pork      (1000) pork      (1000)      789 2024-04-03 19:11:51.000000 punkweb_bb-0.2.0/punkweb_bb/static/punkweb_bb/vendor/sceditor-3.2.0/emoticons/sad.png
--rw-r--r--   0 pork      (1000) pork      (1000)      780 2024-04-03 19:11:51.000000 punkweb_bb-0.2.0/punkweb_bb/static/punkweb_bb/vendor/sceditor-3.2.0/emoticons/shocked.png
--rw-r--r--   0 pork      (1000) pork      (1000)      783 2024-04-03 19:11:51.000000 punkweb_bb-0.2.0/punkweb_bb/static/punkweb_bb/vendor/sceditor-3.2.0/emoticons/sick.png
--rw-r--r--   0 pork      (1000) pork      (1000)      788 2024-04-03 19:11:51.000000 punkweb_bb-0.2.0/punkweb_bb/static/punkweb_bb/vendor/sceditor-3.2.0/emoticons/sideways.png
--rw-r--r--   0 pork      (1000) pork      (1000)      930 2024-04-03 19:11:51.000000 punkweb_bb-0.2.0/punkweb_bb/static/punkweb_bb/vendor/sceditor-3.2.0/emoticons/silly.png
--rw-r--r--   0 pork      (1000) pork      (1000)     1039 2024-04-03 19:11:51.000000 punkweb_bb-0.2.0/punkweb_bb/static/punkweb_bb/vendor/sceditor-3.2.0/emoticons/sleeping.png
--rw-r--r--   0 pork      (1000) pork      (1000)      983 2024-04-03 19:11:51.000000 punkweb_bb-0.2.0/punkweb_bb/static/punkweb_bb/vendor/sceditor-3.2.0/emoticons/smile.png
--rw-r--r--   0 pork      (1000) pork      (1000)      981 2024-04-03 19:11:51.000000 punkweb_bb-0.2.0/punkweb_bb/static/punkweb_bb/vendor/sceditor-3.2.0/emoticons/tongue.png
--rw-r--r--   0 pork      (1000) pork      (1000)      763 2024-04-03 19:11:51.000000 punkweb_bb-0.2.0/punkweb_bb/static/punkweb_bb/vendor/sceditor-3.2.0/emoticons/unsure.png
--rw-r--r--   0 pork      (1000) pork      (1000)      718 2024-04-03 19:11:51.000000 punkweb_bb-0.2.0/punkweb_bb/static/punkweb_bb/vendor/sceditor-3.2.0/emoticons/w00t.png
--rw-r--r--   0 pork      (1000) pork      (1000)      810 2024-04-03 19:11:51.000000 punkweb_bb-0.2.0/punkweb_bb/static/punkweb_bb/vendor/sceditor-3.2.0/emoticons/wassat.png
--rw-r--r--   0 pork      (1000) pork      (1000)     1072 2024-04-03 19:11:51.000000 punkweb_bb-0.2.0/punkweb_bb/static/punkweb_bb/vendor/sceditor-3.2.0/emoticons/whistling.png
--rw-r--r--   0 pork      (1000) pork      (1000)      791 2024-04-03 19:11:51.000000 punkweb_bb-0.2.0/punkweb_bb/static/punkweb_bb/vendor/sceditor-3.2.0/emoticons/wink.png
--rw-r--r--   0 pork      (1000) pork      (1000)     1010 2024-04-03 19:11:51.000000 punkweb_bb-0.2.0/punkweb_bb/static/punkweb_bb/vendor/sceditor-3.2.0/emoticons/wub.png
--rw-r--r--   0 pork      (1000) pork      (1000)     2237 2024-04-03 19:11:51.000000 punkweb_bb-0.2.0/punkweb_bb/static/punkweb_bb/vendor/sceditor-3.2.0/example.html
-drwxr-xr-x   0 pork      (1000) pork      (1000)        0 2024-05-28 23:00:59.972560 punkweb_bb-0.2.0/punkweb_bb/static/punkweb_bb/vendor/sceditor-3.2.0/languages/
--rw-r--r--   0 pork      (1000) pork      (1000)     3235 2024-04-03 19:11:51.000000 punkweb_bb-0.2.0/punkweb_bb/static/punkweb_bb/vendor/sceditor-3.2.0/languages/ar.js
--rw-r--r--   0 pork      (1000) pork      (1000)     2803 2024-04-03 19:11:51.000000 punkweb_bb-0.2.0/punkweb_bb/static/punkweb_bb/vendor/sceditor-3.2.0/languages/ca.js
--rw-r--r--   0 pork      (1000) pork      (1000)     2543 2024-04-03 19:11:51.000000 punkweb_bb-0.2.0/punkweb_bb/static/punkweb_bb/vendor/sceditor-3.2.0/languages/cn.js
--rw-r--r--   0 pork      (1000) pork      (1000)     2879 2024-04-03 19:11:51.000000 punkweb_bb-0.2.0/punkweb_bb/static/punkweb_bb/vendor/sceditor-3.2.0/languages/cs.js
--rw-r--r--   0 pork      (1000) pork      (1000)     2504 2024-04-03 19:11:51.000000 punkweb_bb-0.2.0/punkweb_bb/static/punkweb_bb/vendor/sceditor-3.2.0/languages/de.js
--rw-r--r--   0 pork      (1000) pork      (1000)     4020 2024-04-03 19:11:51.000000 punkweb_bb-0.2.0/punkweb_bb/static/punkweb_bb/vendor/sceditor-3.2.0/languages/el.js
--rw-r--r--   0 pork      (1000) pork      (1000)      102 2024-04-03 19:11:51.000000 punkweb_bb-0.2.0/punkweb_bb/static/punkweb_bb/vendor/sceditor-3.2.0/languages/en-US.js
--rw-r--r--   0 pork      (1000) pork      (1000)      250 2024-04-03 19:11:51.000000 punkweb_bb-0.2.0/punkweb_bb/static/punkweb_bb/vendor/sceditor-3.2.0/languages/en.js
--rw-r--r--   0 pork      (1000) pork      (1000)     2831 2024-04-03 19:11:51.000000 punkweb_bb-0.2.0/punkweb_bb/static/punkweb_bb/vendor/sceditor-3.2.0/languages/es.js
--rw-r--r--   0 pork      (1000) pork      (1000)     2018 2024-04-03 19:11:51.000000 punkweb_bb-0.2.0/punkweb_bb/static/punkweb_bb/vendor/sceditor-3.2.0/languages/et.js
--rw-r--r--   0 pork      (1000) pork      (1000)     3577 2024-04-03 19:11:51.000000 punkweb_bb-0.2.0/punkweb_bb/static/punkweb_bb/vendor/sceditor-3.2.0/languages/fa.js
--rw-r--r--   0 pork      (1000) pork      (1000)     2813 2024-04-03 19:11:51.000000 punkweb_bb-0.2.0/punkweb_bb/static/punkweb_bb/vendor/sceditor-3.2.0/languages/fi.js
--rw-r--r--   0 pork      (1000) pork      (1000)     2906 2024-04-03 19:11:51.000000 punkweb_bb-0.2.0/punkweb_bb/static/punkweb_bb/vendor/sceditor-3.2.0/languages/fr.js
--rw-r--r--   0 pork      (1000) pork      (1000)     2802 2024-04-03 19:11:51.000000 punkweb_bb-0.2.0/punkweb_bb/static/punkweb_bb/vendor/sceditor-3.2.0/languages/gl.js
--rw-r--r--   0 pork      (1000) pork      (1000)     2956 2024-04-03 19:11:51.000000 punkweb_bb-0.2.0/punkweb_bb/static/punkweb_bb/vendor/sceditor-3.2.0/languages/hu.js
--rw-r--r--   0 pork      (1000) pork      (1000)     2718 2024-04-03 19:11:51.000000 punkweb_bb-0.2.0/punkweb_bb/static/punkweb_bb/vendor/sceditor-3.2.0/languages/id.js
--rw-r--r--   0 pork      (1000) pork      (1000)     2981 2024-04-03 19:11:51.000000 punkweb_bb-0.2.0/punkweb_bb/static/punkweb_bb/vendor/sceditor-3.2.0/languages/it.js
--rw-r--r--   0 pork      (1000) pork      (1000)     3259 2024-04-03 19:11:51.000000 punkweb_bb-0.2.0/punkweb_bb/static/punkweb_bb/vendor/sceditor-3.2.0/languages/ja.js
--rw-r--r--   0 pork      (1000) pork      (1000)     3141 2024-04-03 19:11:51.000000 punkweb_bb-0.2.0/punkweb_bb/static/punkweb_bb/vendor/sceditor-3.2.0/languages/lt.js
--rw-r--r--   0 pork      (1000) pork      (1000)     2797 2024-04-03 19:11:51.000000 punkweb_bb-0.2.0/punkweb_bb/static/punkweb_bb/vendor/sceditor-3.2.0/languages/nb.js
--rw-r--r--   0 pork      (1000) pork      (1000)     2903 2024-04-03 19:11:51.000000 punkweb_bb-0.2.0/punkweb_bb/static/punkweb_bb/vendor/sceditor-3.2.0/languages/nl.js
--rw-r--r--   0 pork      (1000) pork      (1000)     2745 2024-04-03 19:11:51.000000 punkweb_bb-0.2.0/punkweb_bb/static/punkweb_bb/vendor/sceditor-3.2.0/languages/pl.js
--rw-r--r--   0 pork      (1000) pork      (1000)     2739 2024-04-03 19:11:51.000000 punkweb_bb-0.2.0/punkweb_bb/static/punkweb_bb/vendor/sceditor-3.2.0/languages/pt-BR.js
--rw-r--r--   0 pork      (1000) pork      (1000)     2810 2024-04-03 19:11:51.000000 punkweb_bb-0.2.0/punkweb_bb/static/punkweb_bb/vendor/sceditor-3.2.0/languages/pt.js
--rw-r--r--   0 pork      (1000) pork      (1000)     3192 2024-04-03 19:11:51.000000 punkweb_bb-0.2.0/punkweb_bb/static/punkweb_bb/vendor/sceditor-3.2.0/languages/ru.js
--rw-r--r--   0 pork      (1000) pork      (1000)     3017 2024-04-03 19:11:51.000000 punkweb_bb-0.2.0/punkweb_bb/static/punkweb_bb/vendor/sceditor-3.2.0/languages/sk.js
--rw-r--r--   0 pork      (1000) pork      (1000)     2210 2024-04-03 19:11:51.000000 punkweb_bb-0.2.0/punkweb_bb/static/punkweb_bb/vendor/sceditor-3.2.0/languages/sv.js
--rw-r--r--   0 pork      (1000) pork      (1000)     2122 2024-04-03 19:11:51.000000 punkweb_bb-0.2.0/punkweb_bb/static/punkweb_bb/vendor/sceditor-3.2.0/languages/template.js
--rw-r--r--   0 pork      (1000) pork      (1000)     2772 2024-04-03 19:11:51.000000 punkweb_bb-0.2.0/punkweb_bb/static/punkweb_bb/vendor/sceditor-3.2.0/languages/tr.js
--rw-r--r--   0 pork      (1000) pork      (1000)     2557 2024-04-03 19:11:51.000000 punkweb_bb-0.2.0/punkweb_bb/static/punkweb_bb/vendor/sceditor-3.2.0/languages/tw.js
--rw-r--r--   0 pork      (1000) pork      (1000)     3102 2024-04-03 19:11:51.000000 punkweb_bb-0.2.0/punkweb_bb/static/punkweb_bb/vendor/sceditor-3.2.0/languages/uk.js
--rw-r--r--   0 pork      (1000) pork      (1000)     2913 2024-04-03 19:11:51.000000 punkweb_bb-0.2.0/punkweb_bb/static/punkweb_bb/vendor/sceditor-3.2.0/languages/vi.js
-drwxr-xr-x   0 pork      (1000) pork      (1000)        0 2024-05-28 23:00:59.972560 punkweb_bb-0.2.0/punkweb_bb/static/punkweb_bb/vendor/sceditor-3.2.0/minified/
-drwxr-xr-x   0 pork      (1000) pork      (1000)        0 2024-05-28 23:00:59.972560 punkweb_bb-0.2.0/punkweb_bb/static/punkweb_bb/vendor/sceditor-3.2.0/minified/formats/
--rw-r--r--   0 pork      (1000) pork      (1000)    17567 2024-04-03 19:11:51.000000 punkweb_bb-0.2.0/punkweb_bb/static/punkweb_bb/vendor/sceditor-3.2.0/minified/formats/bbcode.js
--rw-r--r--   0 pork      (1000) pork      (1000)     8873 2024-04-03 19:11:51.000000 punkweb_bb-0.2.0/punkweb_bb/static/punkweb_bb/vendor/sceditor-3.2.0/minified/formats/xhtml.js
-drwxr-xr-x   0 pork      (1000) pork      (1000)        0 2024-05-28 23:00:59.972560 punkweb_bb-0.2.0/punkweb_bb/static/punkweb_bb/vendor/sceditor-3.2.0/minified/icons/
--rw-r--r--   0 pork      (1000) pork      (1000)     9203 2024-04-03 19:11:51.000000 punkweb_bb-0.2.0/punkweb_bb/static/punkweb_bb/vendor/sceditor-3.2.0/minified/icons/material.js
--rw-r--r--   0 pork      (1000) pork      (1000)    14779 2024-04-03 19:11:51.000000 punkweb_bb-0.2.0/punkweb_bb/static/punkweb_bb/vendor/sceditor-3.2.0/minified/icons/monocons.js
--rw-r--r--   0 pork      (1000) pork      (1000)    91043 2024-04-03 19:11:51.000000 punkweb_bb-0.2.0/punkweb_bb/static/punkweb_bb/vendor/sceditor-3.2.0/minified/jquery.sceditor.bbcode.min.js
--rw-r--r--   0 pork      (1000) pork      (1000)    73632 2024-04-03 19:11:51.000000 punkweb_bb-0.2.0/punkweb_bb/static/punkweb_bb/vendor/sceditor-3.2.0/minified/jquery.sceditor.min.js
--rw-r--r--   0 pork      (1000) pork      (1000)    82349 2024-04-03 19:11:51.000000 punkweb_bb-0.2.0/punkweb_bb/static/punkweb_bb/vendor/sceditor-3.2.0/minified/jquery.sceditor.xhtml.min.js
-drwxr-xr-x   0 pork      (1000) pork      (1000)        0 2024-05-28 23:00:59.972560 punkweb_bb-0.2.0/punkweb_bb/static/punkweb_bb/vendor/sceditor-3.2.0/minified/plugins/
--rw-r--r--   0 pork      (1000) pork      (1000)     1417 2024-04-03 19:11:51.000000 punkweb_bb-0.2.0/punkweb_bb/static/punkweb_bb/vendor/sceditor-3.2.0/minified/plugins/alternative-lists.js
--rw-r--r--   0 pork      (1000) pork      (1000)     1259 2024-04-03 19:11:51.000000 punkweb_bb-0.2.0/punkweb_bb/static/punkweb_bb/vendor/sceditor-3.2.0/minified/plugins/autosave.js
--rw-r--r--   0 pork      (1000) pork      (1000)     1107 2024-04-03 19:11:51.000000 punkweb_bb-0.2.0/punkweb_bb/static/punkweb_bb/vendor/sceditor-3.2.0/minified/plugins/autoyoutube.js
--rw-r--r--   0 pork      (1000) pork      (1000)     3667 2024-04-03 19:11:51.000000 punkweb_bb-0.2.0/punkweb_bb/static/punkweb_bb/vendor/sceditor-3.2.0/minified/plugins/dragdrop.js
--rw-r--r--   0 pork      (1000) pork      (1000)     1088 2024-04-03 19:11:51.000000 punkweb_bb-0.2.0/punkweb_bb/static/punkweb_bb/vendor/sceditor-3.2.0/minified/plugins/format.js
--rw-r--r--   0 pork      (1000) pork      (1000)      775 2024-04-03 19:11:51.000000 punkweb_bb-0.2.0/punkweb_bb/static/punkweb_bb/vendor/sceditor-3.2.0/minified/plugins/plaintext.js
--rw-r--r--   0 pork      (1000) pork      (1000)     2760 2024-04-03 19:11:51.000000 punkweb_bb-0.2.0/punkweb_bb/static/punkweb_bb/vendor/sceditor-3.2.0/minified/plugins/undo.js
--rw-r--r--   0 pork      (1000) pork      (1000)      934 2024-04-03 19:11:51.000000 punkweb_bb-0.2.0/punkweb_bb/static/punkweb_bb/vendor/sceditor-3.2.0/minified/plugins/v1compat.js
--rw-r--r--   0 pork      (1000) pork      (1000)    73296 2024-04-03 19:11:51.000000 punkweb_bb-0.2.0/punkweb_bb/static/punkweb_bb/vendor/sceditor-3.2.0/minified/sceditor.min.js
-drwxr-xr-x   0 pork      (1000) pork      (1000)        0 2024-05-28 23:00:59.972560 punkweb_bb-0.2.0/punkweb_bb/static/punkweb_bb/vendor/sceditor-3.2.0/minified/themes/
-drwxr-xr-x   0 pork      (1000) pork      (1000)        0 2024-05-28 23:00:59.976560 punkweb_bb-0.2.0/punkweb_bb/static/punkweb_bb/vendor/sceditor-3.2.0/minified/themes/content/
--rw-r--r--   0 pork      (1000) pork      (1000)     1016 2024-04-03 19:11:51.000000 punkweb_bb-0.2.0/punkweb_bb/static/punkweb_bb/vendor/sceditor-3.2.0/minified/themes/content/default.min.css
--rw-r--r--   0 pork      (1000) pork      (1000)     9307 2024-04-03 19:11:51.000000 punkweb_bb-0.2.0/punkweb_bb/static/punkweb_bb/vendor/sceditor-3.2.0/minified/themes/default.min.css
--rw-r--r--   0 pork      (1000) pork      (1000)     9570 2024-04-03 19:11:51.000000 punkweb_bb-0.2.0/punkweb_bb/static/punkweb_bb/vendor/sceditor-3.2.0/minified/themes/defaultdark.min.css
--rw-r--r--   0 pork      (1000) pork      (1000)     4583 2024-04-03 19:11:51.000000 punkweb_bb-0.2.0/punkweb_bb/static/punkweb_bb/vendor/sceditor-3.2.0/minified/themes/famfamfam.png
--rw-r--r--   0 pork      (1000) pork      (1000)    10656 2024-04-03 19:11:51.000000 punkweb_bb-0.2.0/punkweb_bb/static/punkweb_bb/vendor/sceditor-3.2.0/minified/themes/modern.min.css
--rw-r--r--   0 pork      (1000) pork      (1000)    12604 2024-04-03 19:11:51.000000 punkweb_bb-0.2.0/punkweb_bb/static/punkweb_bb/vendor/sceditor-3.2.0/minified/themes/office-toolbar.min.css
--rw-r--r--   0 pork      (1000) pork      (1000)    13148 2024-04-03 19:11:51.000000 punkweb_bb-0.2.0/punkweb_bb/static/punkweb_bb/vendor/sceditor-3.2.0/minified/themes/office.min.css
--rw-r--r--   0 pork      (1000) pork      (1000)    10710 2024-04-03 19:11:51.000000 punkweb_bb-0.2.0/punkweb_bb/static/punkweb_bb/vendor/sceditor-3.2.0/minified/themes/square.min.css
-drwxr-xr-x   0 pork      (1000) pork      (1000)        0 2024-05-28 23:00:59.964560 punkweb_bb-0.2.0/punkweb_bb/templates/
-drwxr-xr-x   0 pork      (1000) pork      (1000)        0 2024-05-28 23:00:59.976560 punkweb_bb-0.2.0/punkweb_bb/templates/punkweb_bb/
--rw-r--r--   0 pork      (1000) pork      (1000)     4037 2024-05-07 02:13:59.000000 punkweb_bb-0.2.0/punkweb_bb/templates/punkweb_bb/base.html
--rw-r--r--   0 pork      (1000) pork      (1000)      460 2024-04-05 19:59:05.000000 punkweb_bb-0.2.0/punkweb_bb/templates/punkweb_bb/base_modal.html
--rw-r--r--   0 pork      (1000) pork      (1000)      396 2024-04-06 07:23:56.000000 punkweb_bb-0.2.0/punkweb_bb/templates/punkweb_bb/bbcode.html
--rw-r--r--   0 pork      (1000) pork      (1000)     1369 2024-05-28 22:31:26.000000 punkweb_bb-0.2.0/punkweb_bb/templates/punkweb_bb/category_create.html
--rw-r--r--   0 pork      (1000) pork      (1000)     1467 2024-05-28 19:26:46.000000 punkweb_bb-0.2.0/punkweb_bb/templates/punkweb_bb/category_update.html
--rw-r--r--   0 pork      (1000) pork      (1000)    10032 2024-05-28 22:56:48.000000 punkweb_bb-0.2.0/punkweb_bb/templates/punkweb_bb/index.html
--rw-r--r--   0 pork      (1000) pork      (1000)     1087 2024-04-06 02:06:29.000000 punkweb_bb-0.2.0/punkweb_bb/templates/punkweb_bb/login.html
--rw-r--r--   0 pork      (1000) pork      (1000)     2729 2024-04-08 23:13:19.000000 punkweb_bb-0.2.0/punkweb_bb/templates/punkweb_bb/members.html
-drwxr-xr-x   0 pork      (1000) pork      (1000)        0 2024-05-28 23:00:59.976560 punkweb_bb-0.2.0/punkweb_bb/templates/punkweb_bb/partials/
--rw-r--r--   0 pork      (1000) pork      (1000)      435 2024-05-28 20:05:18.000000 punkweb_bb-0.2.0/punkweb_bb/templates/punkweb_bb/partials/category_delete.html
--rw-r--r--   0 pork      (1000) pork      (1000)      417 2024-04-06 02:06:29.000000 punkweb_bb-0.2.0/punkweb_bb/templates/punkweb_bb/partials/post_delete.html
--rw-r--r--   0 pork      (1000) pork      (1000)      565 2024-04-06 02:06:29.000000 punkweb_bb-0.2.0/punkweb_bb/templates/punkweb_bb/partials/post_update.html
--rw-r--r--   0 pork      (1000) pork      (1000)      421 2024-05-28 20:24:22.000000 punkweb_bb-0.2.0/punkweb_bb/templates/punkweb_bb/partials/shout_delete.html
--rw-r--r--   0 pork      (1000) pork      (1000)      447 2024-05-28 20:05:14.000000 punkweb_bb-0.2.0/punkweb_bb/templates/punkweb_bb/partials/subcategory_delete.html
--rw-r--r--   0 pork      (1000) pork      (1000)      425 2024-04-06 02:06:29.000000 punkweb_bb-0.2.0/punkweb_bb/templates/punkweb_bb/partials/thread_delete.html
--rw-r--r--   0 pork      (1000) pork      (1000)     2948 2024-04-08 23:26:38.000000 punkweb_bb-0.2.0/punkweb_bb/templates/punkweb_bb/profile.html
--rw-r--r--   0 pork      (1000) pork      (1000)     1994 2024-04-07 22:46:43.000000 punkweb_bb-0.2.0/punkweb_bb/templates/punkweb_bb/settings.html
-drwxr-xr-x   0 pork      (1000) pork      (1000)        0 2024-05-28 23:00:59.976560 punkweb_bb-0.2.0/punkweb_bb/templates/punkweb_bb/shoutbox/
--rw-r--r--   0 pork      (1000) pork      (1000)      689 2024-05-28 21:28:48.000000 punkweb_bb-0.2.0/punkweb_bb/templates/punkweb_bb/shoutbox/shout_list.html
--rw-r--r--   0 pork      (1000) pork      (1000)      672 2024-05-28 22:12:45.000000 punkweb_bb-0.2.0/punkweb_bb/templates/punkweb_bb/shoutbox/shoutbox.html
--rw-r--r--   0 pork      (1000) pork      (1000)     1167 2024-04-06 02:06:29.000000 punkweb_bb-0.2.0/punkweb_bb/templates/punkweb_bb/signup.html
--rw-r--r--   0 pork      (1000) pork      (1000)     5543 2024-05-28 22:58:20.000000 punkweb_bb-0.2.0/punkweb_bb/templates/punkweb_bb/subcategory.html
--rw-r--r--   0 pork      (1000) pork      (1000)     1521 2024-05-28 22:31:18.000000 punkweb_bb-0.2.0/punkweb_bb/templates/punkweb_bb/subcategory_create.html
--rw-r--r--   0 pork      (1000) pork      (1000)     1638 2024-05-28 19:43:47.000000 punkweb_bb-0.2.0/punkweb_bb/templates/punkweb_bb/subcategory_update.html
--rw-r--r--   0 pork      (1000) pork      (1000)     8417 2024-05-28 22:53:06.000000 punkweb_bb-0.2.0/punkweb_bb/templates/punkweb_bb/thread.html
--rw-r--r--   0 pork      (1000) pork      (1000)     1639 2024-05-28 22:43:05.000000 punkweb_bb-0.2.0/punkweb_bb/templates/punkweb_bb/thread_create.html
--rw-r--r--   0 pork      (1000) pork      (1000)     1730 2024-05-07 04:35:30.000000 punkweb_bb-0.2.0/punkweb_bb/templates/punkweb_bb/thread_update.html
-drwxr-xr-x   0 pork      (1000) pork      (1000)        0 2024-05-28 23:00:59.976560 punkweb_bb-0.2.0/punkweb_bb/templatetags/
--rw-r--r--   0 pork      (1000) pork      (1000)        0 2024-05-07 04:31:09.000000 punkweb_bb-0.2.0/punkweb_bb/templatetags/__init__.py
-drwxr-xr-x   0 pork      (1000) pork      (1000)        0 2024-05-28 23:00:59.976560 punkweb_bb-0.2.0/punkweb_bb/templatetags/__pycache__/
--rw-r--r--   0 pork      (1000) pork      (1000)      174 2024-05-07 04:31:10.000000 punkweb_bb-0.2.0/punkweb_bb/templatetags/__pycache__/__init__.cpython-311.pyc
--rw-r--r--   0 pork      (1000) pork      (1000)      528 2024-05-28 21:22:24.000000 punkweb_bb-0.2.0/punkweb_bb/templatetags/__pycache__/can_delete.cpython-311.pyc
--rw-r--r--   0 pork      (1000) pork      (1000)      524 2024-05-28 21:22:32.000000 punkweb_bb-0.2.0/punkweb_bb/templatetags/__pycache__/can_edit.cpython-311.pyc
--rw-r--r--   0 pork      (1000) pork      (1000)      524 2024-05-28 21:25:13.000000 punkweb_bb-0.2.0/punkweb_bb/templatetags/__pycache__/can_post.cpython-311.pyc
--rw-r--r--   0 pork      (1000) pork      (1000)      621 2024-05-07 04:30:58.000000 punkweb_bb-0.2.0/punkweb_bb/templatetags/__pycache__/humanize_count.cpython-311.pyc
--rw-r--r--   0 pork      (1000) pork      (1000)      619 2024-05-07 04:31:10.000000 punkweb_bb-0.2.0/punkweb_bb/templatetags/__pycache__/humanize_int.cpython-311.pyc
--rw-r--r--   0 pork      (1000) pork      (1000)      833 2024-04-09 07:07:10.000000 punkweb_bb-0.2.0/punkweb_bb/templatetags/__pycache__/shoutbox_bbcode.cpython-311.pyc
--rw-r--r--   0 pork      (1000) pork      (1000)      137 2024-05-28 21:20:55.000000 punkweb_bb-0.2.0/punkweb_bb/templatetags/can_delete.py
--rw-r--r--   0 pork      (1000) pork      (1000)      133 2024-05-28 21:22:30.000000 punkweb_bb-0.2.0/punkweb_bb/templatetags/can_edit.py
--rw-r--r--   0 pork      (1000) pork      (1000)      133 2024-05-28 21:24:47.000000 punkweb_bb-0.2.0/punkweb_bb/templatetags/can_post.py
--rw-r--r--   0 pork      (1000) pork      (1000)      248 2024-05-07 04:31:08.000000 punkweb_bb-0.2.0/punkweb_bb/templatetags/humanize_int.py
--rw-r--r--   0 pork      (1000) pork      (1000)      310 2024-04-09 07:07:08.000000 punkweb_bb-0.2.0/punkweb_bb/templatetags/shoutbox_bbcode.py
--rw-r--r--   0 pork      (1000) pork      (1000)    26338 2024-05-28 21:35:13.000000 punkweb_bb-0.2.0/punkweb_bb/tests.py
--rw-r--r--   0 pork      (1000) pork      (1000)     2415 2024-05-28 20:10:29.000000 punkweb_bb-0.2.0/punkweb_bb/urls.py
--rw-r--r--   0 pork      (1000) pork      (1000)      396 2024-05-28 21:06:17.000000 punkweb_bb-0.2.0/punkweb_bb/utils.py
--rw-r--r--   0 pork      (1000) pork      (1000)    16610 2024-05-28 22:09:44.000000 punkweb_bb-0.2.0/punkweb_bb/views.py
--rw-r--r--   0 pork      (1000) pork      (1000)      840 2024-04-03 19:20:08.000000 punkweb_bb-0.2.0/punkweb_bb/widgets.py
-drwxr-xr-x   0 pork      (1000) pork      (1000)        0 2024-05-28 23:00:59.964560 punkweb_bb-0.2.0/punkweb_bb.egg-info/
--rw-r--r--   0 pork      (1000) pork      (1000)     5023 2024-05-28 23:00:59.000000 punkweb_bb-0.2.0/punkweb_bb.egg-info/PKG-INFO
--rw-r--r--   0 pork      (1000) pork      (1000)    14282 2024-05-28 23:00:59.000000 punkweb_bb-0.2.0/punkweb_bb.egg-info/SOURCES.txt
--rw-r--r--   0 pork      (1000) pork      (1000)        1 2024-05-28 23:00:59.000000 punkweb_bb-0.2.0/punkweb_bb.egg-info/dependency_links.txt
--rw-r--r--   0 pork      (1000) pork      (1000)        1 2024-04-09 07:09:59.000000 punkweb_bb-0.2.0/punkweb_bb.egg-info/not-zip-safe
--rw-r--r--   0 pork      (1000) pork      (1000)       54 2024-05-28 23:00:59.000000 punkweb_bb-0.2.0/punkweb_bb.egg-info/requires.txt
--rw-r--r--   0 pork      (1000) pork      (1000)       11 2024-05-28 23:00:59.000000 punkweb_bb-0.2.0/punkweb_bb.egg-info/top_level.txt
--rw-r--r--   0 pork      (1000) pork      (1000)       38 2024-05-28 23:00:59.976560 punkweb_bb-0.2.0/setup.cfg
--rw-r--r--   0 pork      (1000) pork      (1000)     1010 2024-05-28 23:00:40.000000 punkweb_bb-0.2.0/setup.py
+drwxr-xr-x   0 pork      (1000) pork      (1000)        0 2024-05-29 04:58:56.305215 punkweb_bb-0.2.1/
+-rw-r--r--   0 pork      (1000) pork      (1000)     1507 2024-04-09 06:08:41.000000 punkweb_bb-0.2.1/LICENSE
+-rw-r--r--   0 pork      (1000) pork      (1000)       64 2024-04-09 05:47:19.000000 punkweb_bb-0.2.1/MANIFEST.in
+-rw-r--r--   0 pork      (1000) pork      (1000)     5023 2024-05-29 04:58:56.305215 punkweb_bb-0.2.1/PKG-INFO
+-rw-r--r--   0 pork      (1000) pork      (1000)     4369 2024-05-09 06:47:11.000000 punkweb_bb-0.2.1/README.md
+drwxr-xr-x   0 pork      (1000) pork      (1000)        0 2024-05-29 04:58:56.293215 punkweb_bb-0.2.1/punkweb_bb/
+-rw-r--r--   0 pork      (1000) pork      (1000)        0 2023-08-20 16:04:51.000000 punkweb_bb-0.2.1/punkweb_bb/__init__.py
+drwxr-xr-x   0 pork      (1000) pork      (1000)        0 2024-05-29 04:58:56.297215 punkweb_bb-0.2.1/punkweb_bb/__pycache__/
+-rw-r--r--   0 pork      (1000) pork      (1000)      161 2024-04-09 05:48:25.000000 punkweb_bb-0.2.1/punkweb_bb/__pycache__/__init__.cpython-311.pyc
+-rw-r--r--   0 pork      (1000) pork      (1000)     3679 2024-04-09 05:48:25.000000 punkweb_bb-0.2.1/punkweb_bb/__pycache__/admin.cpython-311.pyc
+-rw-r--r--   0 pork      (1000) pork      (1000)     2980 2024-04-09 05:48:25.000000 punkweb_bb-0.2.1/punkweb_bb/__pycache__/admin_forms.cpython-311.pyc
+-rw-r--r--   0 pork      (1000) pork      (1000)      730 2024-04-09 06:55:15.000000 punkweb_bb-0.2.1/punkweb_bb/__pycache__/apps.cpython-311.pyc
+-rw-r--r--   0 pork      (1000) pork      (1000)     8534 2024-04-09 06:32:38.000000 punkweb_bb-0.2.1/punkweb_bb/__pycache__/bbcode_tags.cpython-311.pyc
+-rw-r--r--   0 pork      (1000) pork      (1000)      392 2024-04-09 06:44:27.000000 punkweb_bb-0.2.1/punkweb_bb/__pycache__/context_processors.cpython-311.pyc
+-rw-r--r--   0 pork      (1000) pork      (1000)     6194 2024-05-28 21:39:20.000000 punkweb_bb-0.2.1/punkweb_bb/__pycache__/forms.cpython-311.pyc
+-rw-r--r--   0 pork      (1000) pork      (1000)     1581 2024-05-09 05:36:59.000000 punkweb_bb-0.2.1/punkweb_bb/__pycache__/guests.cpython-311.pyc
+-rw-r--r--   0 pork      (1000) pork      (1000)     1560 2024-05-09 05:37:45.000000 punkweb_bb-0.2.1/punkweb_bb/__pycache__/middleware.cpython-311.pyc
+-rw-r--r--   0 pork      (1000) pork      (1000)     1478 2024-04-09 05:48:25.000000 punkweb_bb-0.2.1/punkweb_bb/__pycache__/mixins.cpython-311.pyc
+-rw-r--r--   0 pork      (1000) pork      (1000)    13931 2024-05-29 01:02:42.000000 punkweb_bb-0.2.1/punkweb_bb/__pycache__/models.cpython-311.pyc
+-rw-r--r--   0 pork      (1000) pork      (1000)      990 2024-04-09 05:48:25.000000 punkweb_bb-0.2.1/punkweb_bb/__pycache__/pagination.cpython-311.pyc
+-rw-r--r--   0 pork      (1000) pork      (1000)     5335 2024-04-09 07:07:59.000000 punkweb_bb-0.2.1/punkweb_bb/__pycache__/parsers.cpython-311.pyc
+-rw-r--r--   0 pork      (1000) pork      (1000)      448 2024-04-09 05:48:25.000000 punkweb_bb-0.2.1/punkweb_bb/__pycache__/response.cpython-311.pyc
+-rw-r--r--   0 pork      (1000) pork      (1000)     1025 2024-05-29 04:36:57.000000 punkweb_bb-0.2.1/punkweb_bb/__pycache__/settings.cpython-311.pyc
+-rw-r--r--   0 pork      (1000) pork      (1000)      864 2024-04-09 05:48:25.000000 punkweb_bb-0.2.1/punkweb_bb/__pycache__/signals.cpython-311.pyc
+-rw-r--r--   0 pork      (1000) pork      (1000)    51768 2024-05-28 21:35:15.000000 punkweb_bb-0.2.1/punkweb_bb/__pycache__/tests.cpython-311.pyc
+-rw-r--r--   0 pork      (1000) pork      (1000)     3565 2024-05-29 01:15:02.000000 punkweb_bb-0.2.1/punkweb_bb/__pycache__/urls.cpython-311.pyc
+-rw-r--r--   0 pork      (1000) pork      (1000)      748 2024-05-28 21:07:24.000000 punkweb_bb-0.2.1/punkweb_bb/__pycache__/utils.cpython-311.pyc
+-rw-r--r--   0 pork      (1000) pork      (1000)    25276 2024-05-29 01:17:40.000000 punkweb_bb-0.2.1/punkweb_bb/__pycache__/views.cpython-311.pyc
+-rw-r--r--   0 pork      (1000) pork      (1000)     1552 2024-04-09 05:48:25.000000 punkweb_bb-0.2.1/punkweb_bb/__pycache__/widgets.cpython-311.pyc
+-rw-r--r--   0 pork      (1000) pork      (1000)     2493 2024-04-05 21:20:18.000000 punkweb_bb-0.2.1/punkweb_bb/admin.py
+-rw-r--r--   0 pork      (1000) pork      (1000)     1128 2024-04-03 19:18:44.000000 punkweb_bb-0.2.1/punkweb_bb/admin_forms.py
+-rw-r--r--   0 pork      (1000) pork      (1000)      207 2024-04-09 06:52:38.000000 punkweb_bb-0.2.1/punkweb_bb/apps.py
+-rw-r--r--   0 pork      (1000) pork      (1000)     4419 2024-04-09 06:31:31.000000 punkweb_bb-0.2.1/punkweb_bb/bbcode_tags.py
+-rw-r--r--   0 pork      (1000) pork      (1000)      146 2024-04-09 04:54:41.000000 punkweb_bb-0.2.1/punkweb_bb/context_processors.py
+-rw-r--r--   0 pork      (1000) pork      (1000)     2907 2024-05-28 21:39:19.000000 punkweb_bb-0.2.1/punkweb_bb/forms.py
+-rw-r--r--   0 pork      (1000) pork      (1000)      467 2024-05-09 05:36:58.000000 punkweb_bb-0.2.1/punkweb_bb/guests.py
+-rw-r--r--   0 pork      (1000) pork      (1000)      628 2024-05-09 05:37:44.000000 punkweb_bb-0.2.1/punkweb_bb/middleware.py
+drwxr-xr-x   0 pork      (1000) pork      (1000)        0 2024-05-29 04:58:56.297215 punkweb_bb-0.2.1/punkweb_bb/migrations/
+-rw-r--r--   0 pork      (1000) pork      (1000)     8950 2024-04-09 07:09:02.000000 punkweb_bb-0.2.1/punkweb_bb/migrations/0001_initial.py
+-rw-r--r--   0 pork      (1000) pork      (1000)      388 2024-05-07 04:24:13.000000 punkweb_bb-0.2.1/punkweb_bb/migrations/0002_thread_view_count.py
+-rw-r--r--   0 pork      (1000) pork      (1000)      589 2024-05-29 01:03:10.000000 punkweb_bb-0.2.1/punkweb_bb/migrations/0003_alter_thread_options.py
+-rw-r--r--   0 pork      (1000) pork      (1000)        0 2023-08-20 16:04:51.000000 punkweb_bb-0.2.1/punkweb_bb/migrations/__init__.py
+drwxr-xr-x   0 pork      (1000) pork      (1000)        0 2024-05-29 04:58:56.297215 punkweb_bb-0.2.1/punkweb_bb/migrations/__pycache__/
+-rw-r--r--   0 pork      (1000) pork      (1000)     6456 2024-04-09 07:09:10.000000 punkweb_bb-0.2.1/punkweb_bb/migrations/__pycache__/0001_initial.cpython-311.pyc
+-rw-r--r--   0 pork      (1000) pork      (1000)      815 2024-05-07 04:24:16.000000 punkweb_bb-0.2.1/punkweb_bb/migrations/__pycache__/0002_thread_view_count.cpython-311.pyc
+-rw-r--r--   0 pork      (1000) pork      (1000)      860 2024-05-29 01:03:13.000000 punkweb_bb-0.2.1/punkweb_bb/migrations/__pycache__/0003_alter_thread_options.cpython-311.pyc
+-rw-r--r--   0 pork      (1000) pork      (1000)      172 2024-04-09 05:48:25.000000 punkweb_bb-0.2.1/punkweb_bb/migrations/__pycache__/__init__.cpython-311.pyc
+-rw-r--r--   0 pork      (1000) pork      (1000)      395 2024-04-03 19:16:01.000000 punkweb_bb-0.2.1/punkweb_bb/mixins.py
+-rw-r--r--   0 pork      (1000) pork      (1000)     6348 2024-05-29 01:02:41.000000 punkweb_bb-0.2.1/punkweb_bb/models.py
+-rw-r--r--   0 pork      (1000) pork      (1000)      409 2024-04-06 08:06:22.000000 punkweb_bb-0.2.1/punkweb_bb/pagination.py
+-rw-r--r--   0 pork      (1000) pork      (1000)     2732 2024-04-09 07:07:58.000000 punkweb_bb-0.2.1/punkweb_bb/parsers.py
+-rw-r--r--   0 pork      (1000) pork      (1000)      130 2024-04-03 19:15:29.000000 punkweb_bb-0.2.1/punkweb_bb/response.py
+-rw-r--r--   0 pork      (1000) pork      (1000)      561 2024-05-29 04:36:54.000000 punkweb_bb-0.2.1/punkweb_bb/settings.py
+-rw-r--r--   0 pork      (1000) pork      (1000)      365 2024-04-03 19:18:44.000000 punkweb_bb-0.2.1/punkweb_bb/signals.py
+drwxr-xr-x   0 pork      (1000) pork      (1000)        0 2024-05-29 04:58:56.293215 punkweb_bb-0.2.1/punkweb_bb/static/
+drwxr-xr-x   0 pork      (1000) pork      (1000)        0 2024-05-29 04:58:56.297215 punkweb_bb-0.2.1/punkweb_bb/static/punkweb_bb/
+drwxr-xr-x   0 pork      (1000) pork      (1000)        0 2024-05-29 04:58:56.297215 punkweb_bb-0.2.1/punkweb_bb/static/punkweb_bb/css/
+-rw-r--r--   0 pork      (1000) pork      (1000)      359 2024-05-28 20:15:52.000000 punkweb_bb-0.2.1/punkweb_bb/static/punkweb_bb/css/category-form.css
+-rw-r--r--   0 pork      (1000) pork      (1000)     1455 2024-04-06 07:32:15.000000 punkweb_bb-0.2.1/punkweb_bb/static/punkweb_bb/css/defaults.css
+-rw-r--r--   0 pork      (1000) pork      (1000)     1415 2024-05-29 04:56:43.000000 punkweb_bb-0.2.1/punkweb_bb/static/punkweb_bb/css/index.css
+-rw-r--r--   0 pork      (1000) pork      (1000)      234 2024-04-03 22:23:23.000000 punkweb_bb-0.2.1/punkweb_bb/static/punkweb_bb/css/login.css
+-rw-r--r--   0 pork      (1000) pork      (1000)      395 2024-04-08 22:57:27.000000 punkweb_bb-0.2.1/punkweb_bb/static/punkweb_bb/css/members.css
+-rw-r--r--   0 pork      (1000) pork      (1000)      321 2024-04-03 21:47:53.000000 punkweb_bb-0.2.1/punkweb_bb/static/punkweb_bb/css/post-form.css
+-rw-r--r--   0 pork      (1000) pork      (1000)      916 2024-05-07 01:46:57.000000 punkweb_bb-0.2.1/punkweb_bb/static/punkweb_bb/css/profile.css
+-rw-r--r--   0 pork      (1000) pork      (1000)     1296 2024-04-05 22:11:56.000000 punkweb_bb-0.2.1/punkweb_bb/static/punkweb_bb/css/punkweb-modal.css
+-rw-r--r--   0 pork      (1000) pork      (1000)    14557 2024-05-29 04:06:18.000000 punkweb_bb-0.2.1/punkweb_bb/static/punkweb_bb/css/punkweb.css
+-rw-r--r--   0 pork      (1000) pork      (1000)      308 2024-04-06 07:53:29.000000 punkweb_bb-0.2.1/punkweb_bb/static/punkweb_bb/css/settings.css
+-rw-r--r--   0 pork      (1000) pork      (1000)      536 2024-05-28 21:51:42.000000 punkweb_bb-0.2.1/punkweb_bb/static/punkweb_bb/css/shoutbox.css
+-rw-r--r--   0 pork      (1000) pork      (1000)      371 2024-05-28 20:14:48.000000 punkweb_bb-0.2.1/punkweb_bb/static/punkweb_bb/css/subcategory-form.css
+-rw-r--r--   0 pork      (1000) pork      (1000)      711 2024-05-28 20:02:41.000000 punkweb_bb-0.2.1/punkweb_bb/static/punkweb_bb/css/subcategory.css
+-rw-r--r--   0 pork      (1000) pork      (1000)      329 2024-04-03 19:20:08.000000 punkweb_bb-0.2.1/punkweb_bb/static/punkweb_bb/css/thread-form.css
+-rw-r--r--   0 pork      (1000) pork      (1000)     1873 2024-05-29 01:04:59.000000 punkweb_bb-0.2.1/punkweb_bb/static/punkweb_bb/css/thread.css
+-rw-r--r--   0 pork      (1000) pork      (1000)      448 2024-04-05 15:05:58.000000 punkweb_bb-0.2.1/punkweb_bb/static/punkweb_bb/css/typography.css
+-rw-r--r--   0 pork      (1000) pork      (1000)     1193 2024-05-28 22:52:14.000000 punkweb_bb-0.2.1/punkweb_bb/static/punkweb_bb/css/variables.css
+drwxr-xr-x   0 pork      (1000) pork      (1000)        0 2024-05-29 04:58:56.297215 punkweb_bb-0.2.1/punkweb_bb/static/punkweb_bb/editor/
+-rw-r--r--   0 pork      (1000) pork      (1000)     1466 2024-04-06 07:32:28.000000 punkweb_bb-0.2.1/punkweb_bb/static/punkweb_bb/editor/bbcode-editor-content.css
+-rw-r--r--   0 pork      (1000) pork      (1000)     1624 2024-04-03 19:20:08.000000 punkweb_bb-0.2.1/punkweb_bb/static/punkweb_bb/editor/bbcode-editor-tags.js
+-rw-r--r--   0 pork      (1000) pork      (1000)        0 2024-04-03 19:20:08.000000 punkweb_bb-0.2.1/punkweb_bb/static/punkweb_bb/editor/bbcode-editor.css
+-rw-r--r--   0 pork      (1000) pork      (1000)      607 2024-05-29 03:55:47.000000 punkweb_bb-0.2.1/punkweb_bb/static/punkweb_bb/editor/bbcode-editor.js
+-rw-r--r--   0 pork      (1000) pork      (1000)      318 2024-04-03 19:11:51.000000 punkweb_bb-0.2.1/punkweb_bb/static/punkweb_bb/favicon.ico
+drwxr-xr-x   0 pork      (1000) pork      (1000)        0 2024-05-29 04:58:56.297215 punkweb_bb-0.2.1/punkweb_bb/static/punkweb_bb/img/
+-rw-r--r--   0 pork      (1000) pork      (1000)    60475 2024-04-03 19:20:08.000000 punkweb_bb-0.2.1/punkweb_bb/static/punkweb_bb/img/default-profile-image.png
+drwxr-xr-x   0 pork      (1000) pork      (1000)        0 2024-05-29 04:58:56.297215 punkweb_bb-0.2.1/punkweb_bb/static/punkweb_bb/js/
+-rw-r--r--   0 pork      (1000) pork      (1000)      179 2024-04-03 19:20:08.000000 punkweb_bb-0.2.1/punkweb_bb/static/punkweb_bb/js/punkweb-modal.js
+-rw-r--r--   0 pork      (1000) pork      (1000)      142 2024-04-08 20:20:47.000000 punkweb_bb-0.2.1/punkweb_bb/static/punkweb_bb/js/shoutbox.js
+drwxr-xr-x   0 pork      (1000) pork      (1000)        0 2024-05-29 04:58:56.297215 punkweb_bb-0.2.1/punkweb_bb/static/punkweb_bb/vendor/
+-rw-r--r--   0 pork      (1000) pork      (1000)    44307 2024-04-03 19:17:23.000000 punkweb_bb-0.2.1/punkweb_bb/static/punkweb_bb/vendor/htmx-1.9.4.min.js
+-rw-r--r--   0 pork      (1000) pork      (1000)    87461 2024-04-03 19:11:51.000000 punkweb_bb-0.2.1/punkweb_bb/static/punkweb_bb/vendor/jquery-3.7.0.min.js
+-rw-r--r--   0 pork      (1000) pork      (1000)    10331 2024-04-03 19:11:51.000000 punkweb_bb-0.2.1/punkweb_bb/static/punkweb_bb/vendor/open-color.css
+-rw-r--r--   0 pork      (1000) pork      (1000)     3948 2024-04-03 19:11:51.000000 punkweb_bb-0.2.1/punkweb_bb/static/punkweb_bb/vendor/prism.css
+-rw-r--r--   0 pork      (1000) pork      (1000)   576492 2024-04-03 19:11:51.000000 punkweb_bb-0.2.1/punkweb_bb/static/punkweb_bb/vendor/prism.js
+drwxr-xr-x   0 pork      (1000) pork      (1000)        0 2024-05-29 04:58:56.297215 punkweb_bb-0.2.1/punkweb_bb/static/punkweb_bb/vendor/sceditor-3.2.0/
+-rw-r--r--   0 pork      (1000) pork      (1000)     4129 2024-04-03 19:11:51.000000 punkweb_bb-0.2.1/punkweb_bb/static/punkweb_bb/vendor/sceditor-3.2.0/README.md
+drwxr-xr-x   0 pork      (1000) pork      (1000)        0 2024-05-29 04:58:56.297215 punkweb_bb-0.2.1/punkweb_bb/static/punkweb_bb/vendor/sceditor-3.2.0/development/
+drwxr-xr-x   0 pork      (1000) pork      (1000)        0 2024-05-29 04:58:56.297215 punkweb_bb-0.2.1/punkweb_bb/static/punkweb_bb/vendor/sceditor-3.2.0/development/formats/
+-rw-r--r--   0 pork      (1000) pork      (1000)    61679 2024-04-03 19:11:51.000000 punkweb_bb-0.2.1/punkweb_bb/static/punkweb_bb/vendor/sceditor-3.2.0/development/formats/bbcode.js
+-rw-r--r--   0 pork      (1000) pork      (1000)    26086 2024-04-03 19:11:51.000000 punkweb_bb-0.2.1/punkweb_bb/static/punkweb_bb/vendor/sceditor-3.2.0/development/formats/xhtml.js
+drwxr-xr-x   0 pork      (1000) pork      (1000)        0 2024-05-29 04:58:56.297215 punkweb_bb-0.2.1/punkweb_bb/static/punkweb_bb/vendor/sceditor-3.2.0/development/icons/
+-rw-r--r--   0 pork      (1000) pork      (1000)    11260 2024-04-03 19:11:51.000000 punkweb_bb-0.2.1/punkweb_bb/static/punkweb_bb/vendor/sceditor-3.2.0/development/icons/material.js
+-rw-r--r--   0 pork      (1000) pork      (1000)    15873 2024-04-03 19:11:51.000000 punkweb_bb-0.2.1/punkweb_bb/static/punkweb_bb/vendor/sceditor-3.2.0/development/icons/monocons.js
+-rw-r--r--   0 pork      (1000) pork      (1000)   312959 2024-04-03 19:11:51.000000 punkweb_bb-0.2.1/punkweb_bb/static/punkweb_bb/vendor/sceditor-3.2.0/development/jquery.sceditor.bbcode.js
+-rw-r--r--   0 pork      (1000) pork      (1000)   251279 2024-04-03 19:11:51.000000 punkweb_bb-0.2.1/punkweb_bb/static/punkweb_bb/vendor/sceditor-3.2.0/development/jquery.sceditor.js
+-rw-r--r--   0 pork      (1000) pork      (1000)   277366 2024-04-03 19:11:51.000000 punkweb_bb-0.2.1/punkweb_bb/static/punkweb_bb/vendor/sceditor-3.2.0/development/jquery.sceditor.xhtml.js
+drwxr-xr-x   0 pork      (1000) pork      (1000)        0 2024-05-29 04:58:56.301216 punkweb_bb-0.2.1/punkweb_bb/static/punkweb_bb/vendor/sceditor-3.2.0/development/plugins/
+-rw-r--r--   0 pork      (1000) pork      (1000)     3446 2024-04-03 19:11:51.000000 punkweb_bb-0.2.1/punkweb_bb/static/punkweb_bb/vendor/sceditor-3.2.0/development/plugins/alternative-lists.js
+-rw-r--r--   0 pork      (1000) pork      (1000)     2571 2024-04-03 19:11:51.000000 punkweb_bb-0.2.1/punkweb_bb/static/punkweb_bb/vendor/sceditor-3.2.0/development/plugins/autosave.js
+-rw-r--r--   0 pork      (1000) pork      (1000)     2791 2024-04-03 19:11:51.000000 punkweb_bb-0.2.1/punkweb_bb/static/punkweb_bb/vendor/sceditor-3.2.0/development/plugins/autoyoutube.js
+-rw-r--r--   0 pork      (1000) pork      (1000)     6306 2024-04-03 19:11:51.000000 punkweb_bb-0.2.1/punkweb_bb/static/punkweb_bb/vendor/sceditor-3.2.0/development/plugins/dragdrop.js
+-rw-r--r--   0 pork      (1000) pork      (1000)     2528 2024-04-03 19:11:51.000000 punkweb_bb-0.2.1/punkweb_bb/static/punkweb_bb/vendor/sceditor-3.2.0/development/plugins/format.js
+-rw-r--r--   0 pork      (1000) pork      (1000)     2059 2024-04-03 19:11:51.000000 punkweb_bb-0.2.1/punkweb_bb/static/punkweb_bb/vendor/sceditor-3.2.0/development/plugins/plaintext.js
+-rw-r--r--   0 pork      (1000) pork      (1000)     9375 2024-04-03 19:11:51.000000 punkweb_bb-0.2.1/punkweb_bb/static/punkweb_bb/vendor/sceditor-3.2.0/development/plugins/undo.js
+-rw-r--r--   0 pork      (1000) pork      (1000)     2067 2024-04-03 19:11:51.000000 punkweb_bb-0.2.1/punkweb_bb/static/punkweb_bb/vendor/sceditor-3.2.0/development/plugins/v1compat.js
+-rw-r--r--   0 pork      (1000) pork      (1000)   249123 2024-04-03 19:11:51.000000 punkweb_bb-0.2.1/punkweb_bb/static/punkweb_bb/vendor/sceditor-3.2.0/development/sceditor.js
+drwxr-xr-x   0 pork      (1000) pork      (1000)        0 2024-05-29 04:58:56.301216 punkweb_bb-0.2.1/punkweb_bb/static/punkweb_bb/vendor/sceditor-3.2.0/development/themes/
+drwxr-xr-x   0 pork      (1000) pork      (1000)        0 2024-05-29 04:58:56.301216 punkweb_bb-0.2.1/punkweb_bb/static/punkweb_bb/vendor/sceditor-3.2.0/development/themes/content/
+-rw-r--r--   0 pork      (1000) pork      (1000)     1476 2024-04-03 19:11:51.000000 punkweb_bb-0.2.1/punkweb_bb/static/punkweb_bb/vendor/sceditor-3.2.0/development/themes/content/default.css
+-rw-r--r--   0 pork      (1000) pork      (1000)    11194 2024-04-03 19:11:51.000000 punkweb_bb-0.2.1/punkweb_bb/static/punkweb_bb/vendor/sceditor-3.2.0/development/themes/default.css
+-rw-r--r--   0 pork      (1000) pork      (1000)    11500 2024-04-03 19:11:51.000000 punkweb_bb-0.2.1/punkweb_bb/static/punkweb_bb/vendor/sceditor-3.2.0/development/themes/defaultdark.css
+-rw-r--r--   0 pork      (1000) pork      (1000)     4583 2024-04-03 19:11:51.000000 punkweb_bb-0.2.1/punkweb_bb/static/punkweb_bb/vendor/sceditor-3.2.0/development/themes/famfamfam.png
+-rw-r--r--   0 pork      (1000) pork      (1000)    12943 2024-04-03 19:11:51.000000 punkweb_bb-0.2.1/punkweb_bb/static/punkweb_bb/vendor/sceditor-3.2.0/development/themes/modern.css
+-rw-r--r--   0 pork      (1000) pork      (1000)    13431 2024-04-03 19:11:51.000000 punkweb_bb-0.2.1/punkweb_bb/static/punkweb_bb/vendor/sceditor-3.2.0/development/themes/office-toolbar.css
+-rw-r--r--   0 pork      (1000) pork      (1000)    14124 2024-04-03 19:11:51.000000 punkweb_bb-0.2.1/punkweb_bb/static/punkweb_bb/vendor/sceditor-3.2.0/development/themes/office.css
+-rw-r--r--   0 pork      (1000) pork      (1000)    13183 2024-04-03 19:11:51.000000 punkweb_bb-0.2.1/punkweb_bb/static/punkweb_bb/vendor/sceditor-3.2.0/development/themes/square.css
+drwxr-xr-x   0 pork      (1000) pork      (1000)        0 2024-05-29 04:58:56.301216 punkweb_bb-0.2.1/punkweb_bb/static/punkweb_bb/vendor/sceditor-3.2.0/emoticons/
+-rw-r--r--   0 pork      (1000) pork      (1000)      756 2024-04-03 19:11:51.000000 punkweb_bb-0.2.1/punkweb_bb/static/punkweb_bb/vendor/sceditor-3.2.0/emoticons/alien.png
+-rw-r--r--   0 pork      (1000) pork      (1000)     1182 2024-04-03 19:11:51.000000 punkweb_bb-0.2.1/punkweb_bb/static/punkweb_bb/vendor/sceditor-3.2.0/emoticons/angel.png
+-rw-r--r--   0 pork      (1000) pork      (1000)      781 2024-04-03 19:11:51.000000 punkweb_bb-0.2.1/punkweb_bb/static/punkweb_bb/vendor/sceditor-3.2.0/emoticons/angry.png
+-rw-r--r--   0 pork      (1000) pork      (1000)      972 2024-04-03 19:11:51.000000 punkweb_bb-0.2.1/punkweb_bb/static/punkweb_bb/vendor/sceditor-3.2.0/emoticons/blink.png
+-rw-r--r--   0 pork      (1000) pork      (1000)      865 2024-04-03 19:11:51.000000 punkweb_bb-0.2.1/punkweb_bb/static/punkweb_bb/vendor/sceditor-3.2.0/emoticons/blush.png
+-rw-r--r--   0 pork      (1000) pork      (1000)      753 2024-04-03 19:11:51.000000 punkweb_bb-0.2.1/punkweb_bb/static/punkweb_bb/vendor/sceditor-3.2.0/emoticons/cheerful.png
+-rw-r--r--   0 pork      (1000) pork      (1000)      965 2024-04-03 19:11:51.000000 punkweb_bb-0.2.1/punkweb_bb/static/punkweb_bb/vendor/sceditor-3.2.0/emoticons/cool.png
+-rw-r--r--   0 pork      (1000) pork      (1000)      421 2024-04-03 19:11:51.000000 punkweb_bb-0.2.1/punkweb_bb/static/punkweb_bb/vendor/sceditor-3.2.0/emoticons/credits.txt
+-rw-r--r--   0 pork      (1000) pork      (1000)      877 2024-04-03 19:11:51.000000 punkweb_bb-0.2.1/punkweb_bb/static/punkweb_bb/vendor/sceditor-3.2.0/emoticons/cwy.png
+-rw-r--r--   0 pork      (1000) pork      (1000)     1012 2024-04-03 19:11:51.000000 punkweb_bb-0.2.1/punkweb_bb/static/punkweb_bb/vendor/sceditor-3.2.0/emoticons/devil.png
+-rw-r--r--   0 pork      (1000) pork      (1000)      991 2024-04-03 19:11:51.000000 punkweb_bb-0.2.1/punkweb_bb/static/punkweb_bb/vendor/sceditor-3.2.0/emoticons/dizzy.png
+-rw-r--r--   0 pork      (1000) pork      (1000)      983 2024-04-03 19:11:51.000000 punkweb_bb-0.2.1/punkweb_bb/static/punkweb_bb/vendor/sceditor-3.2.0/emoticons/ermm.png
+-rw-r--r--   0 pork      (1000) pork      (1000)      793 2024-04-03 19:11:51.000000 punkweb_bb-0.2.1/punkweb_bb/static/punkweb_bb/vendor/sceditor-3.2.0/emoticons/face.png
+-rw-r--r--   0 pork      (1000) pork      (1000)      792 2024-04-03 19:11:51.000000 punkweb_bb-0.2.1/punkweb_bb/static/punkweb_bb/vendor/sceditor-3.2.0/emoticons/getlost.png
+-rw-r--r--   0 pork      (1000) pork      (1000)      867 2024-04-03 19:11:51.000000 punkweb_bb-0.2.1/punkweb_bb/static/punkweb_bb/vendor/sceditor-3.2.0/emoticons/grin.png
+-rw-r--r--   0 pork      (1000) pork      (1000)      792 2024-04-03 19:11:51.000000 punkweb_bb-0.2.1/punkweb_bb/static/punkweb_bb/vendor/sceditor-3.2.0/emoticons/happy.png
+-rw-r--r--   0 pork      (1000) pork      (1000)      572 2024-04-03 19:11:51.000000 punkweb_bb-0.2.1/punkweb_bb/static/punkweb_bb/vendor/sceditor-3.2.0/emoticons/heart.png
+-rw-r--r--   0 pork      (1000) pork      (1000)      793 2024-04-03 19:11:51.000000 punkweb_bb-0.2.1/punkweb_bb/static/punkweb_bb/vendor/sceditor-3.2.0/emoticons/kissing.png
+-rw-r--r--   0 pork      (1000) pork      (1000)      912 2024-04-03 19:11:51.000000 punkweb_bb-0.2.1/punkweb_bb/static/punkweb_bb/vendor/sceditor-3.2.0/emoticons/laughing.png
+-rw-r--r--   0 pork      (1000) pork      (1000)      694 2024-04-03 19:11:51.000000 punkweb_bb-0.2.1/punkweb_bb/static/punkweb_bb/vendor/sceditor-3.2.0/emoticons/ninja.png
+-rw-r--r--   0 pork      (1000) pork      (1000)      804 2024-04-03 19:11:51.000000 punkweb_bb-0.2.1/punkweb_bb/static/punkweb_bb/vendor/sceditor-3.2.0/emoticons/pinch.png
+-rw-r--r--   0 pork      (1000) pork      (1000)      799 2024-04-03 19:11:51.000000 punkweb_bb-0.2.1/punkweb_bb/static/punkweb_bb/vendor/sceditor-3.2.0/emoticons/pouty.png
+-rw-r--r--   0 pork      (1000) pork      (1000)      789 2024-04-03 19:11:51.000000 punkweb_bb-0.2.1/punkweb_bb/static/punkweb_bb/vendor/sceditor-3.2.0/emoticons/sad.png
+-rw-r--r--   0 pork      (1000) pork      (1000)      780 2024-04-03 19:11:51.000000 punkweb_bb-0.2.1/punkweb_bb/static/punkweb_bb/vendor/sceditor-3.2.0/emoticons/shocked.png
+-rw-r--r--   0 pork      (1000) pork      (1000)      783 2024-04-03 19:11:51.000000 punkweb_bb-0.2.1/punkweb_bb/static/punkweb_bb/vendor/sceditor-3.2.0/emoticons/sick.png
+-rw-r--r--   0 pork      (1000) pork      (1000)      788 2024-04-03 19:11:51.000000 punkweb_bb-0.2.1/punkweb_bb/static/punkweb_bb/vendor/sceditor-3.2.0/emoticons/sideways.png
+-rw-r--r--   0 pork      (1000) pork      (1000)      930 2024-04-03 19:11:51.000000 punkweb_bb-0.2.1/punkweb_bb/static/punkweb_bb/vendor/sceditor-3.2.0/emoticons/silly.png
+-rw-r--r--   0 pork      (1000) pork      (1000)     1039 2024-04-03 19:11:51.000000 punkweb_bb-0.2.1/punkweb_bb/static/punkweb_bb/vendor/sceditor-3.2.0/emoticons/sleeping.png
+-rw-r--r--   0 pork      (1000) pork      (1000)      983 2024-04-03 19:11:51.000000 punkweb_bb-0.2.1/punkweb_bb/static/punkweb_bb/vendor/sceditor-3.2.0/emoticons/smile.png
+-rw-r--r--   0 pork      (1000) pork      (1000)      981 2024-04-03 19:11:51.000000 punkweb_bb-0.2.1/punkweb_bb/static/punkweb_bb/vendor/sceditor-3.2.0/emoticons/tongue.png
+-rw-r--r--   0 pork      (1000) pork      (1000)      763 2024-04-03 19:11:51.000000 punkweb_bb-0.2.1/punkweb_bb/static/punkweb_bb/vendor/sceditor-3.2.0/emoticons/unsure.png
+-rw-r--r--   0 pork      (1000) pork      (1000)      718 2024-04-03 19:11:51.000000 punkweb_bb-0.2.1/punkweb_bb/static/punkweb_bb/vendor/sceditor-3.2.0/emoticons/w00t.png
+-rw-r--r--   0 pork      (1000) pork      (1000)      810 2024-04-03 19:11:51.000000 punkweb_bb-0.2.1/punkweb_bb/static/punkweb_bb/vendor/sceditor-3.2.0/emoticons/wassat.png
+-rw-r--r--   0 pork      (1000) pork      (1000)     1072 2024-04-03 19:11:51.000000 punkweb_bb-0.2.1/punkweb_bb/static/punkweb_bb/vendor/sceditor-3.2.0/emoticons/whistling.png
+-rw-r--r--   0 pork      (1000) pork      (1000)      791 2024-04-03 19:11:51.000000 punkweb_bb-0.2.1/punkweb_bb/static/punkweb_bb/vendor/sceditor-3.2.0/emoticons/wink.png
+-rw-r--r--   0 pork      (1000) pork      (1000)     1010 2024-04-03 19:11:51.000000 punkweb_bb-0.2.1/punkweb_bb/static/punkweb_bb/vendor/sceditor-3.2.0/emoticons/wub.png
+-rw-r--r--   0 pork      (1000) pork      (1000)     2237 2024-04-03 19:11:51.000000 punkweb_bb-0.2.1/punkweb_bb/static/punkweb_bb/vendor/sceditor-3.2.0/example.html
+drwxr-xr-x   0 pork      (1000) pork      (1000)        0 2024-05-29 04:58:56.301216 punkweb_bb-0.2.1/punkweb_bb/static/punkweb_bb/vendor/sceditor-3.2.0/languages/
+-rw-r--r--   0 pork      (1000) pork      (1000)     3235 2024-04-03 19:11:51.000000 punkweb_bb-0.2.1/punkweb_bb/static/punkweb_bb/vendor/sceditor-3.2.0/languages/ar.js
+-rw-r--r--   0 pork      (1000) pork      (1000)     2803 2024-04-03 19:11:51.000000 punkweb_bb-0.2.1/punkweb_bb/static/punkweb_bb/vendor/sceditor-3.2.0/languages/ca.js
+-rw-r--r--   0 pork      (1000) pork      (1000)     2543 2024-04-03 19:11:51.000000 punkweb_bb-0.2.1/punkweb_bb/static/punkweb_bb/vendor/sceditor-3.2.0/languages/cn.js
+-rw-r--r--   0 pork      (1000) pork      (1000)     2879 2024-04-03 19:11:51.000000 punkweb_bb-0.2.1/punkweb_bb/static/punkweb_bb/vendor/sceditor-3.2.0/languages/cs.js
+-rw-r--r--   0 pork      (1000) pork      (1000)     2504 2024-04-03 19:11:51.000000 punkweb_bb-0.2.1/punkweb_bb/static/punkweb_bb/vendor/sceditor-3.2.0/languages/de.js
+-rw-r--r--   0 pork      (1000) pork      (1000)     4020 2024-04-03 19:11:51.000000 punkweb_bb-0.2.1/punkweb_bb/static/punkweb_bb/vendor/sceditor-3.2.0/languages/el.js
+-rw-r--r--   0 pork      (1000) pork      (1000)      102 2024-04-03 19:11:51.000000 punkweb_bb-0.2.1/punkweb_bb/static/punkweb_bb/vendor/sceditor-3.2.0/languages/en-US.js
+-rw-r--r--   0 pork      (1000) pork      (1000)      250 2024-04-03 19:11:51.000000 punkweb_bb-0.2.1/punkweb_bb/static/punkweb_bb/vendor/sceditor-3.2.0/languages/en.js
+-rw-r--r--   0 pork      (1000) pork      (1000)     2831 2024-04-03 19:11:51.000000 punkweb_bb-0.2.1/punkweb_bb/static/punkweb_bb/vendor/sceditor-3.2.0/languages/es.js
+-rw-r--r--   0 pork      (1000) pork      (1000)     2018 2024-04-03 19:11:51.000000 punkweb_bb-0.2.1/punkweb_bb/static/punkweb_bb/vendor/sceditor-3.2.0/languages/et.js
+-rw-r--r--   0 pork      (1000) pork      (1000)     3577 2024-04-03 19:11:51.000000 punkweb_bb-0.2.1/punkweb_bb/static/punkweb_bb/vendor/sceditor-3.2.0/languages/fa.js
+-rw-r--r--   0 pork      (1000) pork      (1000)     2813 2024-04-03 19:11:51.000000 punkweb_bb-0.2.1/punkweb_bb/static/punkweb_bb/vendor/sceditor-3.2.0/languages/fi.js
+-rw-r--r--   0 pork      (1000) pork      (1000)     2906 2024-04-03 19:11:51.000000 punkweb_bb-0.2.1/punkweb_bb/static/punkweb_bb/vendor/sceditor-3.2.0/languages/fr.js
+-rw-r--r--   0 pork      (1000) pork      (1000)     2802 2024-04-03 19:11:51.000000 punkweb_bb-0.2.1/punkweb_bb/static/punkweb_bb/vendor/sceditor-3.2.0/languages/gl.js
+-rw-r--r--   0 pork      (1000) pork      (1000)     2956 2024-04-03 19:11:51.000000 punkweb_bb-0.2.1/punkweb_bb/static/punkweb_bb/vendor/sceditor-3.2.0/languages/hu.js
+-rw-r--r--   0 pork      (1000) pork      (1000)     2718 2024-04-03 19:11:51.000000 punkweb_bb-0.2.1/punkweb_bb/static/punkweb_bb/vendor/sceditor-3.2.0/languages/id.js
+-rw-r--r--   0 pork      (1000) pork      (1000)     2981 2024-04-03 19:11:51.000000 punkweb_bb-0.2.1/punkweb_bb/static/punkweb_bb/vendor/sceditor-3.2.0/languages/it.js
+-rw-r--r--   0 pork      (1000) pork      (1000)     3259 2024-04-03 19:11:51.000000 punkweb_bb-0.2.1/punkweb_bb/static/punkweb_bb/vendor/sceditor-3.2.0/languages/ja.js
+-rw-r--r--   0 pork      (1000) pork      (1000)     3141 2024-04-03 19:11:51.000000 punkweb_bb-0.2.1/punkweb_bb/static/punkweb_bb/vendor/sceditor-3.2.0/languages/lt.js
+-rw-r--r--   0 pork      (1000) pork      (1000)     2797 2024-04-03 19:11:51.000000 punkweb_bb-0.2.1/punkweb_bb/static/punkweb_bb/vendor/sceditor-3.2.0/languages/nb.js
+-rw-r--r--   0 pork      (1000) pork      (1000)     2903 2024-04-03 19:11:51.000000 punkweb_bb-0.2.1/punkweb_bb/static/punkweb_bb/vendor/sceditor-3.2.0/languages/nl.js
+-rw-r--r--   0 pork      (1000) pork      (1000)     2745 2024-04-03 19:11:51.000000 punkweb_bb-0.2.1/punkweb_bb/static/punkweb_bb/vendor/sceditor-3.2.0/languages/pl.js
+-rw-r--r--   0 pork      (1000) pork      (1000)     2739 2024-04-03 19:11:51.000000 punkweb_bb-0.2.1/punkweb_bb/static/punkweb_bb/vendor/sceditor-3.2.0/languages/pt-BR.js
+-rw-r--r--   0 pork      (1000) pork      (1000)     2810 2024-04-03 19:11:51.000000 punkweb_bb-0.2.1/punkweb_bb/static/punkweb_bb/vendor/sceditor-3.2.0/languages/pt.js
+-rw-r--r--   0 pork      (1000) pork      (1000)     3192 2024-04-03 19:11:51.000000 punkweb_bb-0.2.1/punkweb_bb/static/punkweb_bb/vendor/sceditor-3.2.0/languages/ru.js
+-rw-r--r--   0 pork      (1000) pork      (1000)     3017 2024-04-03 19:11:51.000000 punkweb_bb-0.2.1/punkweb_bb/static/punkweb_bb/vendor/sceditor-3.2.0/languages/sk.js
+-rw-r--r--   0 pork      (1000) pork      (1000)     2210 2024-04-03 19:11:51.000000 punkweb_bb-0.2.1/punkweb_bb/static/punkweb_bb/vendor/sceditor-3.2.0/languages/sv.js
+-rw-r--r--   0 pork      (1000) pork      (1000)     2122 2024-04-03 19:11:51.000000 punkweb_bb-0.2.1/punkweb_bb/static/punkweb_bb/vendor/sceditor-3.2.0/languages/template.js
+-rw-r--r--   0 pork      (1000) pork      (1000)     2772 2024-04-03 19:11:51.000000 punkweb_bb-0.2.1/punkweb_bb/static/punkweb_bb/vendor/sceditor-3.2.0/languages/tr.js
+-rw-r--r--   0 pork      (1000) pork      (1000)     2557 2024-04-03 19:11:51.000000 punkweb_bb-0.2.1/punkweb_bb/static/punkweb_bb/vendor/sceditor-3.2.0/languages/tw.js
+-rw-r--r--   0 pork      (1000) pork      (1000)     3102 2024-04-03 19:11:51.000000 punkweb_bb-0.2.1/punkweb_bb/static/punkweb_bb/vendor/sceditor-3.2.0/languages/uk.js
+-rw-r--r--   0 pork      (1000) pork      (1000)     2913 2024-04-03 19:11:51.000000 punkweb_bb-0.2.1/punkweb_bb/static/punkweb_bb/vendor/sceditor-3.2.0/languages/vi.js
+drwxr-xr-x   0 pork      (1000) pork      (1000)        0 2024-05-29 04:58:56.301216 punkweb_bb-0.2.1/punkweb_bb/static/punkweb_bb/vendor/sceditor-3.2.0/minified/
+drwxr-xr-x   0 pork      (1000) pork      (1000)        0 2024-05-29 04:58:56.301216 punkweb_bb-0.2.1/punkweb_bb/static/punkweb_bb/vendor/sceditor-3.2.0/minified/formats/
+-rw-r--r--   0 pork      (1000) pork      (1000)    17567 2024-04-03 19:11:51.000000 punkweb_bb-0.2.1/punkweb_bb/static/punkweb_bb/vendor/sceditor-3.2.0/minified/formats/bbcode.js
+-rw-r--r--   0 pork      (1000) pork      (1000)     8873 2024-04-03 19:11:51.000000 punkweb_bb-0.2.1/punkweb_bb/static/punkweb_bb/vendor/sceditor-3.2.0/minified/formats/xhtml.js
+drwxr-xr-x   0 pork      (1000) pork      (1000)        0 2024-05-29 04:58:56.305215 punkweb_bb-0.2.1/punkweb_bb/static/punkweb_bb/vendor/sceditor-3.2.0/minified/icons/
+-rw-r--r--   0 pork      (1000) pork      (1000)     9203 2024-04-03 19:11:51.000000 punkweb_bb-0.2.1/punkweb_bb/static/punkweb_bb/vendor/sceditor-3.2.0/minified/icons/material.js
+-rw-r--r--   0 pork      (1000) pork      (1000)    14779 2024-04-03 19:11:51.000000 punkweb_bb-0.2.1/punkweb_bb/static/punkweb_bb/vendor/sceditor-3.2.0/minified/icons/monocons.js
+-rw-r--r--   0 pork      (1000) pork      (1000)    91043 2024-04-03 19:11:51.000000 punkweb_bb-0.2.1/punkweb_bb/static/punkweb_bb/vendor/sceditor-3.2.0/minified/jquery.sceditor.bbcode.min.js
+-rw-r--r--   0 pork      (1000) pork      (1000)    73632 2024-04-03 19:11:51.000000 punkweb_bb-0.2.1/punkweb_bb/static/punkweb_bb/vendor/sceditor-3.2.0/minified/jquery.sceditor.min.js
+-rw-r--r--   0 pork      (1000) pork      (1000)    82349 2024-04-03 19:11:51.000000 punkweb_bb-0.2.1/punkweb_bb/static/punkweb_bb/vendor/sceditor-3.2.0/minified/jquery.sceditor.xhtml.min.js
+drwxr-xr-x   0 pork      (1000) pork      (1000)        0 2024-05-29 04:58:56.305215 punkweb_bb-0.2.1/punkweb_bb/static/punkweb_bb/vendor/sceditor-3.2.0/minified/plugins/
+-rw-r--r--   0 pork      (1000) pork      (1000)     1417 2024-04-03 19:11:51.000000 punkweb_bb-0.2.1/punkweb_bb/static/punkweb_bb/vendor/sceditor-3.2.0/minified/plugins/alternative-lists.js
+-rw-r--r--   0 pork      (1000) pork      (1000)     1259 2024-04-03 19:11:51.000000 punkweb_bb-0.2.1/punkweb_bb/static/punkweb_bb/vendor/sceditor-3.2.0/minified/plugins/autosave.js
+-rw-r--r--   0 pork      (1000) pork      (1000)     1107 2024-04-03 19:11:51.000000 punkweb_bb-0.2.1/punkweb_bb/static/punkweb_bb/vendor/sceditor-3.2.0/minified/plugins/autoyoutube.js
+-rw-r--r--   0 pork      (1000) pork      (1000)     3667 2024-04-03 19:11:51.000000 punkweb_bb-0.2.1/punkweb_bb/static/punkweb_bb/vendor/sceditor-3.2.0/minified/plugins/dragdrop.js
+-rw-r--r--   0 pork      (1000) pork      (1000)     1088 2024-04-03 19:11:51.000000 punkweb_bb-0.2.1/punkweb_bb/static/punkweb_bb/vendor/sceditor-3.2.0/minified/plugins/format.js
+-rw-r--r--   0 pork      (1000) pork      (1000)      775 2024-04-03 19:11:51.000000 punkweb_bb-0.2.1/punkweb_bb/static/punkweb_bb/vendor/sceditor-3.2.0/minified/plugins/plaintext.js
+-rw-r--r--   0 pork      (1000) pork      (1000)     2760 2024-04-03 19:11:51.000000 punkweb_bb-0.2.1/punkweb_bb/static/punkweb_bb/vendor/sceditor-3.2.0/minified/plugins/undo.js
+-rw-r--r--   0 pork      (1000) pork      (1000)      934 2024-04-03 19:11:51.000000 punkweb_bb-0.2.1/punkweb_bb/static/punkweb_bb/vendor/sceditor-3.2.0/minified/plugins/v1compat.js
+-rw-r--r--   0 pork      (1000) pork      (1000)    73296 2024-04-03 19:11:51.000000 punkweb_bb-0.2.1/punkweb_bb/static/punkweb_bb/vendor/sceditor-3.2.0/minified/sceditor.min.js
+drwxr-xr-x   0 pork      (1000) pork      (1000)        0 2024-05-29 04:58:56.305215 punkweb_bb-0.2.1/punkweb_bb/static/punkweb_bb/vendor/sceditor-3.2.0/minified/themes/
+drwxr-xr-x   0 pork      (1000) pork      (1000)        0 2024-05-29 04:58:56.305215 punkweb_bb-0.2.1/punkweb_bb/static/punkweb_bb/vendor/sceditor-3.2.0/minified/themes/content/
+-rw-r--r--   0 pork      (1000) pork      (1000)     1016 2024-04-03 19:11:51.000000 punkweb_bb-0.2.1/punkweb_bb/static/punkweb_bb/vendor/sceditor-3.2.0/minified/themes/content/default.min.css
+-rw-r--r--   0 pork      (1000) pork      (1000)     9307 2024-04-03 19:11:51.000000 punkweb_bb-0.2.1/punkweb_bb/static/punkweb_bb/vendor/sceditor-3.2.0/minified/themes/default.min.css
+-rw-r--r--   0 pork      (1000) pork      (1000)     9570 2024-04-03 19:11:51.000000 punkweb_bb-0.2.1/punkweb_bb/static/punkweb_bb/vendor/sceditor-3.2.0/minified/themes/defaultdark.min.css
+-rw-r--r--   0 pork      (1000) pork      (1000)     4583 2024-04-03 19:11:51.000000 punkweb_bb-0.2.1/punkweb_bb/static/punkweb_bb/vendor/sceditor-3.2.0/minified/themes/famfamfam.png
+-rw-r--r--   0 pork      (1000) pork      (1000)    10656 2024-04-03 19:11:51.000000 punkweb_bb-0.2.1/punkweb_bb/static/punkweb_bb/vendor/sceditor-3.2.0/minified/themes/modern.min.css
+-rw-r--r--   0 pork      (1000) pork      (1000)    12604 2024-04-03 19:11:51.000000 punkweb_bb-0.2.1/punkweb_bb/static/punkweb_bb/vendor/sceditor-3.2.0/minified/themes/office-toolbar.min.css
+-rw-r--r--   0 pork      (1000) pork      (1000)    13148 2024-04-03 19:11:51.000000 punkweb_bb-0.2.1/punkweb_bb/static/punkweb_bb/vendor/sceditor-3.2.0/minified/themes/office.min.css
+-rw-r--r--   0 pork      (1000) pork      (1000)    10710 2024-04-03 19:11:51.000000 punkweb_bb-0.2.1/punkweb_bb/static/punkweb_bb/vendor/sceditor-3.2.0/minified/themes/square.min.css
+drwxr-xr-x   0 pork      (1000) pork      (1000)        0 2024-05-29 04:58:56.293215 punkweb_bb-0.2.1/punkweb_bb/templates/
+drwxr-xr-x   0 pork      (1000) pork      (1000)        0 2024-05-29 04:58:56.305215 punkweb_bb-0.2.1/punkweb_bb/templates/punkweb_bb/
+-rw-r--r--   0 pork      (1000) pork      (1000)     4426 2024-05-29 04:37:00.000000 punkweb_bb-0.2.1/punkweb_bb/templates/punkweb_bb/base.html
+-rw-r--r--   0 pork      (1000) pork      (1000)      460 2024-04-05 19:59:05.000000 punkweb_bb-0.2.1/punkweb_bb/templates/punkweb_bb/base_modal.html
+-rw-r--r--   0 pork      (1000) pork      (1000)      396 2024-04-06 07:23:56.000000 punkweb_bb-0.2.1/punkweb_bb/templates/punkweb_bb/bbcode.html
+-rw-r--r--   0 pork      (1000) pork      (1000)     1369 2024-05-29 04:29:25.000000 punkweb_bb-0.2.1/punkweb_bb/templates/punkweb_bb/category_create.html
+-rw-r--r--   0 pork      (1000) pork      (1000)     1467 2024-05-28 19:26:46.000000 punkweb_bb-0.2.1/punkweb_bb/templates/punkweb_bb/category_update.html
+-rw-r--r--   0 pork      (1000) pork      (1000)    10470 2024-05-29 04:55:52.000000 punkweb_bb-0.2.1/punkweb_bb/templates/punkweb_bb/index.html
+-rw-r--r--   0 pork      (1000) pork      (1000)     1137 2024-05-29 04:29:31.000000 punkweb_bb-0.2.1/punkweb_bb/templates/punkweb_bb/login.html
+-rw-r--r--   0 pork      (1000) pork      (1000)     2781 2024-05-29 04:30:06.000000 punkweb_bb-0.2.1/punkweb_bb/templates/punkweb_bb/members.html
+drwxr-xr-x   0 pork      (1000) pork      (1000)        0 2024-05-29 04:58:56.305215 punkweb_bb-0.2.1/punkweb_bb/templates/punkweb_bb/partials/
+-rw-r--r--   0 pork      (1000) pork      (1000)      435 2024-05-28 20:05:18.000000 punkweb_bb-0.2.1/punkweb_bb/templates/punkweb_bb/partials/category_delete.html
+-rw-r--r--   0 pork      (1000) pork      (1000)      417 2024-04-06 02:06:29.000000 punkweb_bb-0.2.1/punkweb_bb/templates/punkweb_bb/partials/post_delete.html
+-rw-r--r--   0 pork      (1000) pork      (1000)      565 2024-04-06 02:06:29.000000 punkweb_bb-0.2.1/punkweb_bb/templates/punkweb_bb/partials/post_update.html
+-rw-r--r--   0 pork      (1000) pork      (1000)      421 2024-05-28 20:24:22.000000 punkweb_bb-0.2.1/punkweb_bb/templates/punkweb_bb/partials/shout_delete.html
+-rw-r--r--   0 pork      (1000) pork      (1000)      447 2024-05-28 20:05:14.000000 punkweb_bb-0.2.1/punkweb_bb/templates/punkweb_bb/partials/subcategory_delete.html
+-rw-r--r--   0 pork      (1000) pork      (1000)      425 2024-04-06 02:06:29.000000 punkweb_bb-0.2.1/punkweb_bb/templates/punkweb_bb/partials/thread_delete.html
+-rw-r--r--   0 pork      (1000) pork      (1000)     3012 2024-05-29 04:30:15.000000 punkweb_bb-0.2.1/punkweb_bb/templates/punkweb_bb/profile.html
+-rw-r--r--   0 pork      (1000) pork      (1000)     2047 2024-05-29 04:30:22.000000 punkweb_bb-0.2.1/punkweb_bb/templates/punkweb_bb/settings.html
+drwxr-xr-x   0 pork      (1000) pork      (1000)        0 2024-05-29 04:58:56.305215 punkweb_bb-0.2.1/punkweb_bb/templates/punkweb_bb/shoutbox/
+-rw-r--r--   0 pork      (1000) pork      (1000)      736 2024-05-29 04:44:03.000000 punkweb_bb-0.2.1/punkweb_bb/templates/punkweb_bb/shoutbox/shout_list.html
+-rw-r--r--   0 pork      (1000) pork      (1000)      672 2024-05-28 22:12:45.000000 punkweb_bb-0.2.1/punkweb_bb/templates/punkweb_bb/shoutbox/shoutbox.html
+-rw-r--r--   0 pork      (1000) pork      (1000)     1219 2024-05-29 04:30:30.000000 punkweb_bb-0.2.1/punkweb_bb/templates/punkweb_bb/signup.html
+-rw-r--r--   0 pork      (1000) pork      (1000)     5848 2024-05-29 04:30:44.000000 punkweb_bb-0.2.1/punkweb_bb/templates/punkweb_bb/subcategory.html
+-rw-r--r--   0 pork      (1000) pork      (1000)     1521 2024-05-28 22:31:18.000000 punkweb_bb-0.2.1/punkweb_bb/templates/punkweb_bb/subcategory_create.html
+-rw-r--r--   0 pork      (1000) pork      (1000)     1638 2024-05-28 19:43:47.000000 punkweb_bb-0.2.1/punkweb_bb/templates/punkweb_bb/subcategory_update.html
+-rw-r--r--   0 pork      (1000) pork      (1000)    10276 2024-05-29 04:43:11.000000 punkweb_bb-0.2.1/punkweb_bb/templates/punkweb_bb/thread.html
+-rw-r--r--   0 pork      (1000) pork      (1000)     1697 2024-05-29 04:30:51.000000 punkweb_bb-0.2.1/punkweb_bb/templates/punkweb_bb/thread_create.html
+-rw-r--r--   0 pork      (1000) pork      (1000)     1730 2024-05-07 04:35:30.000000 punkweb_bb-0.2.1/punkweb_bb/templates/punkweb_bb/thread_update.html
+drwxr-xr-x   0 pork      (1000) pork      (1000)        0 2024-05-29 04:58:56.305215 punkweb_bb-0.2.1/punkweb_bb/templatetags/
+-rw-r--r--   0 pork      (1000) pork      (1000)        0 2024-05-07 04:31:09.000000 punkweb_bb-0.2.1/punkweb_bb/templatetags/__init__.py
+drwxr-xr-x   0 pork      (1000) pork      (1000)        0 2024-05-29 04:58:56.305215 punkweb_bb-0.2.1/punkweb_bb/templatetags/__pycache__/
+-rw-r--r--   0 pork      (1000) pork      (1000)      174 2024-05-07 04:31:10.000000 punkweb_bb-0.2.1/punkweb_bb/templatetags/__pycache__/__init__.cpython-311.pyc
+-rw-r--r--   0 pork      (1000) pork      (1000)      528 2024-05-28 21:22:24.000000 punkweb_bb-0.2.1/punkweb_bb/templatetags/__pycache__/can_delete.cpython-311.pyc
+-rw-r--r--   0 pork      (1000) pork      (1000)      524 2024-05-28 21:22:32.000000 punkweb_bb-0.2.1/punkweb_bb/templatetags/__pycache__/can_edit.cpython-311.pyc
+-rw-r--r--   0 pork      (1000) pork      (1000)      524 2024-05-28 21:25:13.000000 punkweb_bb-0.2.1/punkweb_bb/templatetags/__pycache__/can_post.cpython-311.pyc
+-rw-r--r--   0 pork      (1000) pork      (1000)      621 2024-05-07 04:30:58.000000 punkweb_bb-0.2.1/punkweb_bb/templatetags/__pycache__/humanize_count.cpython-311.pyc
+-rw-r--r--   0 pork      (1000) pork      (1000)      619 2024-05-07 04:31:10.000000 punkweb_bb-0.2.1/punkweb_bb/templatetags/__pycache__/humanize_int.cpython-311.pyc
+-rw-r--r--   0 pork      (1000) pork      (1000)      833 2024-04-09 07:07:10.000000 punkweb_bb-0.2.1/punkweb_bb/templatetags/__pycache__/shoutbox_bbcode.cpython-311.pyc
+-rw-r--r--   0 pork      (1000) pork      (1000)      137 2024-05-28 21:20:55.000000 punkweb_bb-0.2.1/punkweb_bb/templatetags/can_delete.py
+-rw-r--r--   0 pork      (1000) pork      (1000)      133 2024-05-28 21:22:30.000000 punkweb_bb-0.2.1/punkweb_bb/templatetags/can_edit.py
+-rw-r--r--   0 pork      (1000) pork      (1000)      133 2024-05-28 21:24:47.000000 punkweb_bb-0.2.1/punkweb_bb/templatetags/can_post.py
+-rw-r--r--   0 pork      (1000) pork      (1000)      248 2024-05-07 04:31:08.000000 punkweb_bb-0.2.1/punkweb_bb/templatetags/humanize_int.py
+-rw-r--r--   0 pork      (1000) pork      (1000)      310 2024-04-09 07:07:08.000000 punkweb_bb-0.2.1/punkweb_bb/templatetags/shoutbox_bbcode.py
+-rw-r--r--   0 pork      (1000) pork      (1000)    26338 2024-05-28 21:35:13.000000 punkweb_bb-0.2.1/punkweb_bb/tests.py
+-rw-r--r--   0 pork      (1000) pork      (1000)     2587 2024-05-29 01:15:01.000000 punkweb_bb-0.2.1/punkweb_bb/urls.py
+-rw-r--r--   0 pork      (1000) pork      (1000)      396 2024-05-28 21:06:17.000000 punkweb_bb-0.2.1/punkweb_bb/utils.py
+-rw-r--r--   0 pork      (1000) pork      (1000)    17400 2024-05-29 01:17:40.000000 punkweb_bb-0.2.1/punkweb_bb/views.py
+-rw-r--r--   0 pork      (1000) pork      (1000)      840 2024-04-03 19:20:08.000000 punkweb_bb-0.2.1/punkweb_bb/widgets.py
+drwxr-xr-x   0 pork      (1000) pork      (1000)        0 2024-05-29 04:58:56.293215 punkweb_bb-0.2.1/punkweb_bb.egg-info/
+-rw-r--r--   0 pork      (1000) pork      (1000)     5023 2024-05-29 04:58:56.000000 punkweb_bb-0.2.1/punkweb_bb.egg-info/PKG-INFO
+-rw-r--r--   0 pork      (1000) pork      (1000)    14409 2024-05-29 04:58:56.000000 punkweb_bb-0.2.1/punkweb_bb.egg-info/SOURCES.txt
+-rw-r--r--   0 pork      (1000) pork      (1000)        1 2024-05-29 04:58:56.000000 punkweb_bb-0.2.1/punkweb_bb.egg-info/dependency_links.txt
+-rw-r--r--   0 pork      (1000) pork      (1000)        1 2024-04-09 07:09:59.000000 punkweb_bb-0.2.1/punkweb_bb.egg-info/not-zip-safe
+-rw-r--r--   0 pork      (1000) pork      (1000)       54 2024-05-29 04:58:56.000000 punkweb_bb-0.2.1/punkweb_bb.egg-info/requires.txt
+-rw-r--r--   0 pork      (1000) pork      (1000)       11 2024-05-29 04:58:56.000000 punkweb_bb-0.2.1/punkweb_bb.egg-info/top_level.txt
+-rw-r--r--   0 pork      (1000) pork      (1000)       38 2024-05-29 04:58:56.305215 punkweb_bb-0.2.1/setup.cfg
+-rw-r--r--   0 pork      (1000) pork      (1000)     1010 2024-05-29 04:58:04.000000 punkweb_bb-0.2.1/setup.py
```

### Comparing `punkweb_bb-0.2.0/LICENSE` & `punkweb_bb-0.2.1/LICENSE`

 * *Files identical despite different names*

### Comparing `punkweb_bb-0.2.0/PKG-INFO` & `punkweb_bb-0.2.1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: punkweb_bb
-Version: 0.2.0
+Version: 0.2.1
 Summary: Django application that provides a simple and modern forum board software for your Django website.
 Home-page: https://github.com/Punkweb/PunkwebBB
 Author: Punkweb
 Author-email: punkwebnet@gmail.com
 License: BSD-3-Clause
 Classifier: Environment :: Web Environment
 Classifier: Framework :: Django
```

### Comparing `punkweb_bb-0.2.0/README.md` & `punkweb_bb-0.2.1/README.md`

 * *Files identical despite different names*

### Comparing `punkweb_bb-0.2.0/punkweb_bb/__pycache__/admin.cpython-311.pyc` & `punkweb_bb-0.2.1/punkweb_bb/__pycache__/admin.cpython-311.pyc`

 * *Files identical despite different names*

### Comparing `punkweb_bb-0.2.0/punkweb_bb/__pycache__/admin_forms.cpython-311.pyc` & `punkweb_bb-0.2.1/punkweb_bb/__pycache__/admin_forms.cpython-311.pyc`

 * *Files identical despite different names*

### Comparing `punkweb_bb-0.2.0/punkweb_bb/__pycache__/apps.cpython-311.pyc` & `punkweb_bb-0.2.1/punkweb_bb/__pycache__/apps.cpython-311.pyc`

 * *Files identical despite different names*

### Comparing `punkweb_bb-0.2.0/punkweb_bb/__pycache__/bbcode_tags.cpython-311.pyc` & `punkweb_bb-0.2.1/punkweb_bb/__pycache__/bbcode_tags.cpython-311.pyc`

 * *Files identical despite different names*

### Comparing `punkweb_bb-0.2.0/punkweb_bb/__pycache__/forms.cpython-311.pyc` & `punkweb_bb-0.2.1/punkweb_bb/__pycache__/forms.cpython-311.pyc`

 * *Files identical despite different names*

### Comparing `punkweb_bb-0.2.0/punkweb_bb/__pycache__/guests.cpython-311.pyc` & `punkweb_bb-0.2.1/punkweb_bb/__pycache__/guests.cpython-311.pyc`

 * *Files identical despite different names*

### Comparing `punkweb_bb-0.2.0/punkweb_bb/__pycache__/middleware.cpython-311.pyc` & `punkweb_bb-0.2.1/punkweb_bb/__pycache__/middleware.cpython-311.pyc`

 * *Files identical despite different names*

### Comparing `punkweb_bb-0.2.0/punkweb_bb/__pycache__/mixins.cpython-311.pyc` & `punkweb_bb-0.2.1/punkweb_bb/__pycache__/mixins.cpython-311.pyc`

 * *Files identical despite different names*

### Comparing `punkweb_bb-0.2.0/punkweb_bb/__pycache__/models.cpython-311.pyc` & `punkweb_bb-0.2.1/punkweb_bb/__pycache__/models.cpython-311.pyc`

 * *Files 4% similar despite different names*

#### Python bytecode

```diff
@@ -1,10 +1,10 @@
 magic:    0xa70d0d0a
-moddate:  0x89605666 (Tue May 28 22:54:01 2024 UTC)
-files sz: 6218
+moddate:  0xb17e5666 (Wed May 29 01:02:41 2024 UTC)
+files sz: 6348
 code
    argcount  : 0
    nlocals   : 0
    stacksize : 6
    flags     : 0
    code
       0x9700640064016c005a00640064016c015a01640064016c025a02640064
@@ -144,28 +144,28 @@
                250 LOAD_CONST              18 ('Thread')
                252 LOAD_NAME               19 (UUIDPrimaryKeyMixin)
                254 LOAD_NAME               18 (TimestampMixin)
                256 PRECALL                  4
                260 CALL                     4
                270 STORE_NAME              25 (Thread)
    
-   147         272 PUSH_NULL
+   151         272 PUSH_NULL
                274 LOAD_BUILD_CLASS
-               276 LOAD_CONST              19 (<code object Post, file "/home/pork/Punkweb/punkweb-bb/punkweb_bb/models.py", line 147>)
+               276 LOAD_CONST              19 (<code object Post, file "/home/pork/Punkweb/punkweb-bb/punkweb_bb/models.py", line 151>)
                278 MAKE_FUNCTION            0
                280 LOAD_CONST              20 ('Post')
                282 LOAD_NAME               19 (UUIDPrimaryKeyMixin)
                284 LOAD_NAME               18 (TimestampMixin)
                286 PRECALL                  4
                290 CALL                     4
                300 STORE_NAME              26 (Post)
    
-   192         302 PUSH_NULL
+   196         302 PUSH_NULL
                304 LOAD_BUILD_CLASS
-               306 LOAD_CONST              21 (<code object Shout, file "/home/pork/Punkweb/punkweb-bb/punkweb_bb/models.py", line 192>)
+               306 LOAD_CONST              21 (<code object Shout, file "/home/pork/Punkweb/punkweb-bb/punkweb_bb/models.py", line 196>)
                308 MAKE_FUNCTION            0
                310 LOAD_CONST              22 ('Shout')
                312 LOAD_NAME               19 (UUIDPrimaryKeyMixin)
                314 LOAD_NAME               18 (TimestampMixin)
                316 PRECALL                  4
                320 CALL                     4
                330 STORE_NAME              27 (Shout)
@@ -1189,51 +1189,51 @@
                      300 LOAD_CONST              10 (<code object Meta, file "/home/pork/Punkweb/punkweb-bb/punkweb_bb/models.py", line 116>)
                      302 MAKE_FUNCTION            0
                      304 LOAD_CONST              11 ('Meta')
                      306 PRECALL                  2
                      310 CALL                     2
                      320 STORE_NAME              21 (Meta)
          
-         123         322 LOAD_CONST              12 (<code object __str__, file "/home/pork/Punkweb/punkweb-bb/punkweb_bb/models.py", line 123>)
+         127         322 LOAD_CONST              12 (<code object __str__, file "/home/pork/Punkweb/punkweb-bb/punkweb_bb/models.py", line 127>)
                      324 MAKE_FUNCTION            0
                      326 STORE_NAME              22 (__str__)
          
-         126         328 LOAD_CONST              13 (<code object can_edit, file "/home/pork/Punkweb/punkweb-bb/punkweb_bb/models.py", line 126>)
+         130         328 LOAD_CONST              13 (<code object can_edit, file "/home/pork/Punkweb/punkweb-bb/punkweb_bb/models.py", line 130>)
                      330 MAKE_FUNCTION            0
                      332 STORE_NAME              23 (can_edit)
          
-         129         334 LOAD_CONST              14 (<code object can_delete, file "/home/pork/Punkweb/punkweb-bb/punkweb_bb/models.py", line 129>)
+         133         334 LOAD_CONST              14 (<code object can_delete, file "/home/pork/Punkweb/punkweb-bb/punkweb_bb/models.py", line 133>)
                      336 MAKE_FUNCTION            0
                      338 STORE_NAME              24 (can_delete)
          
-         132         340 LOAD_CONST              15 (<code object can_post, file "/home/pork/Punkweb/punkweb-bb/punkweb_bb/models.py", line 132>)
+         136         340 LOAD_CONST              15 (<code object can_post, file "/home/pork/Punkweb/punkweb-bb/punkweb_bb/models.py", line 136>)
                      342 MAKE_FUNCTION            0
                      344 STORE_NAME              25 (can_post)
          
-         135         346 LOAD_NAME               26 (property)
+         139         346 LOAD_NAME               26 (property)
          
-         136         348 LOAD_CONST              16 (<code object post_count, file "/home/pork/Punkweb/punkweb-bb/punkweb_bb/models.py", line 135>)
+         140         348 LOAD_CONST              16 (<code object post_count, file "/home/pork/Punkweb/punkweb-bb/punkweb_bb/models.py", line 139>)
                      350 MAKE_FUNCTION            0
          
-         135         352 PRECALL                  0
+         139         352 PRECALL                  0
                      356 CALL                     0
          
-         136         366 STORE_NAME              27 (post_count)
+         140         366 STORE_NAME              27 (post_count)
          
-         139         368 LOAD_NAME               26 (property)
+         143         368 LOAD_NAME               26 (property)
          
-         140         370 LOAD_CONST              17 (<code object latest_post, file "/home/pork/Punkweb/punkweb-bb/punkweb_bb/models.py", line 139>)
+         144         370 LOAD_CONST              17 (<code object latest_post, file "/home/pork/Punkweb/punkweb-bb/punkweb_bb/models.py", line 143>)
                      372 MAKE_FUNCTION            0
          
-         139         374 PRECALL                  0
+         143         374 PRECALL                  0
                      378 CALL                     0
          
-         140         388 STORE_NAME              28 (latest_post)
+         144         388 STORE_NAME              28 (latest_post)
          
-         143         390 LOAD_CONST              18 (<code object get_absolute_url, file "/home/pork/Punkweb/punkweb-bb/punkweb_bb/models.py", line 143>)
+         147         390 LOAD_CONST              18 (<code object get_absolute_url, file "/home/pork/Punkweb/punkweb-bb/punkweb_bb/models.py", line 147>)
                      392 MAKE_FUNCTION            0
                      394 STORE_NAME              29 (get_absolute_url)
                      396 LOAD_CONST              19 (None)
                      398 RETURN_VALUE
          consts
             'Thread'
             'threads'
@@ -1246,72 +1246,76 @@
             ('auto_now_add',)
             0
             code
                argcount  : 0
                nlocals   : 0
                stacksize : 1
                flags     : 0
-               code 0x970065005a0164005a0264015a0364025300
+               code 0x970065005a0164005a0264015a0364025a0464035300
                116           0 RESUME                   0
                              2 LOAD_NAME                0 (__name__)
                              4 STORE_NAME               1 (__module__)
                              6 LOAD_CONST               0 ('Thread.Meta')
                              8 STORE_NAME               2 (__qualname__)
                
                117          10 LOAD_CONST               1 (('subcategory', '-is_pinned', '-last_post_created_at'))
                             12 STORE_NAME               3 (ordering)
-                            14 LOAD_CONST               2 (None)
-                            16 RETURN_VALUE
+               
+               122          14 LOAD_CONST               2 ((('pin_thread', 'Can pin thread'), ('close_thread', 'Can close thread')))
+                            16 STORE_NAME               4 (permissions)
+                            18 LOAD_CONST               3 (None)
+                            20 RETURN_VALUE
                consts
                   'Thread.Meta'
                   ('subcategory', '-is_pinned', '-last_post_created_at')
+                  (('pin_thread', 'Can pin thread'), ('close_thread', 'Can close thread'))
                   None
-               names      ('__name__', '__module__', '__qualname__', 'ordering')
+               names      ('__name__', '__module__', '__qualname__', 'ordering', 'permissions')
                varnames   ()
                freevars   ()
                cellvars   ()
                filename   '/home/pork/Punkweb/punkweb-bb/punkweb_bb/models.py'
                name       'Meta'
                firstlineno 116
-               lnotab 0x0a01
+               lnotab 0x0a010405
             'Meta'
             code
                argcount  : 1
                nlocals   : 1
                stacksize : 1
                flags     : 3
                code 0x97007c006a0000000000000000009b005300
-               123           0 RESUME                   0
+               127           0 RESUME                   0
                
-               124           2 LOAD_FAST                0 (self)
+               128           2 LOAD_FAST                0 (self)
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
-               firstlineno 123
+               firstlineno 127
                lnotab 0x0201
             code
                argcount  : 2
                nlocals   : 2
                stacksize : 3
                flags     : 3
                code
                   0x97007c017c006a0000000000000000006b020000000070147c01a00100
                   000000000000000000000000000000000000006401a6010000ab01000000
                   00000000005300
-               126           0 RESUME                   0
+               130           0 RESUME                   0
                
-               127           2 LOAD_FAST                1 (user)
+               131           2 LOAD_FAST                1 (user)
                              4 LOAD_FAST                0 (self)
                              6 LOAD_ATTR                0 (user)
                             16 COMPARE_OP               2 (==)
                             22 JUMP_IF_TRUE_OR_POP     20 (to 64)
                             24 LOAD_FAST                1 (user)
                             26 LOAD_METHOD              1 (has_perm)
                             48 LOAD_CONST               1 ('punkweb_bb.change_thread')
@@ -1323,28 +1327,28 @@
                   'punkweb_bb.change_thread'
                names      ('user', 'has_perm')
                varnames   ('self', 'user')
                freevars   ()
                cellvars   ()
                filename   '/home/pork/Punkweb/punkweb-bb/punkweb_bb/models.py'
                name       'can_edit'
-               firstlineno 126
+               firstlineno 130
                lnotab 0x0201
             code
                argcount  : 2
                nlocals   : 2
                stacksize : 3
                flags     : 3
                code
                   0x97007c017c006a0000000000000000006b020000000070147c01a00100
                   000000000000000000000000000000000000006401a6010000ab01000000
                   00000000005300
-               129           0 RESUME                   0
+               133           0 RESUME                   0
                
-               130           2 LOAD_FAST                1 (user)
+               134           2 LOAD_FAST                1 (user)
                              4 LOAD_FAST                0 (self)
                              6 LOAD_ATTR                0 (user)
                             16 COMPARE_OP               2 (==)
                             22 JUMP_IF_TRUE_OR_POP     20 (to 64)
                             24 LOAD_FAST                1 (user)
                             26 LOAD_METHOD              1 (has_perm)
                             48 LOAD_CONST               1 ('punkweb_bb.delete_thread')
@@ -1356,77 +1360,77 @@
                   'punkweb_bb.delete_thread'
                names      ('user', 'has_perm')
                varnames   ('self', 'user')
                freevars   ()
                cellvars   ()
                filename   '/home/pork/Punkweb/punkweb-bb/punkweb_bb/models.py'
                name       'can_delete'
-               firstlineno 129
+               firstlineno 133
                lnotab 0x0201
             code
                argcount  : 2
                nlocals   : 2
                stacksize : 1
                flags     : 3
                code 0x97007c006a0000000000000000000c005300
-               132           0 RESUME                   0
+               136           0 RESUME                   0
                
-               133           2 LOAD_FAST                0 (self)
+               137           2 LOAD_FAST                0 (self)
                              4 LOAD_ATTR                0 (is_closed)
                             14 UNARY_NOT
                             16 RETURN_VALUE
                consts
                   None
                names      ('is_closed',)
                varnames   ('self', 'user')
                freevars   ()
                cellvars   ()
                filename   '/home/pork/Punkweb/punkweb-bb/punkweb_bb/models.py'
                name       'can_post'
-               firstlineno 132
+               firstlineno 136
                lnotab 0x0201
             code
                argcount  : 1
                nlocals   : 1
                stacksize : 2
                flags     : 3
                code
                   0x97007c006a000000000000000000a00100000000000000000000000000
                   00000000000000a6000000ab0000000000000000005300
-               135           0 RESUME                   0
+               139           0 RESUME                   0
                
-               137           2 LOAD_FAST                0 (self)
+               141           2 LOAD_FAST                0 (self)
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
-               firstlineno 135
+               firstlineno 139
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
-               139           0 RESUME                   0
+               143           0 RESUME                   0
                
-               141           2 LOAD_FAST                0 (self)
+               145           2 LOAD_FAST                0 (self)
                              4 LOAD_ATTR                0 (posts)
                             14 LOAD_METHOD              1 (order_by)
                             36 LOAD_CONST               1 ('-created_at')
                             38 PRECALL                  1
                             42 CALL                     1
                             52 LOAD_METHOD              2 (first)
                             74 PRECALL                  0
@@ -1437,27 +1441,27 @@
                   '-created_at'
                names      ('posts', 'order_by', 'first')
                varnames   ('self',)
                freevars   ()
                cellvars   ()
                filename   '/home/pork/Punkweb/punkweb-bb/punkweb_bb/models.py'
                name       'latest_post'
-               firstlineno 139
+               firstlineno 143
                lnotab 0x0202
             code
                argcount  : 1
                nlocals   : 1
                stacksize : 4
                flags     : 3
                code
                   0x970074010000000000000000000064017c006a01000000000000000067
                   01ac02a6020000ab0200000000000000005300
-               143           0 RESUME                   0
+               147           0 RESUME                   0
                
-               144           2 LOAD_GLOBAL              1 (NULL + reverse)
+               148           2 LOAD_GLOBAL              1 (NULL + reverse)
                             14 LOAD_CONST               1 ('punkweb_bb:thread')
                             16 LOAD_FAST                0 (self)
                             18 LOAD_ATTR                1 (id)
                             28 BUILD_LIST               1
                             30 KW_NAMES                 2
                             32 PRECALL                  2
                             36 CALL                     2
@@ -1468,26 +1472,26 @@
                   ('args',)
                names      ('reverse', 'id')
                varnames   ('self',)
                freevars   ()
                cellvars   ()
                filename   '/home/pork/Punkweb/punkweb-bb/punkweb_bb/models.py'
                name       'get_absolute_url'
-               firstlineno 143
+               firstlineno 147
                lnotab 0x0201
             None
          names      ('__name__', '__module__', '__qualname__', 'models', 'ForeignKey', 'Subcategory', 'CASCADE', 'subcategory', 'User', 'user', 'CharField', 'title', 'BBCodeTextField', 'content', 'BooleanField', 'is_pinned', 'is_closed', 'DateTimeField', 'last_post_created_at', 'PositiveIntegerField', 'view_count', 'Meta', '__str__', 'can_edit', 'can_delete', 'can_post', 'property', 'post_count', 'latest_post', 'get_absolute_url')
          varnames   ()
          freevars   ()
          cellvars   ()
          filename   '/home/pork/Punkweb/punkweb-bb/punkweb_bb/models.py'
          name       'Thread'
          firstlineno 104
          lnotab
-            0x0a010e0110ff120330012201140122012201220122021a070603060306
+            0x0a010e0110ff120330012201140122012201220122021a0b0603060306
             030603020104ff0e010203020104ff0e010203
       'Thread'
       code
          argcount  : 0
          nlocals   : 0
          stacksize : 5
          flags     : 0
@@ -1499,98 +1503,98 @@
             000000000000005a0b02004700640384006404a6020000ab020000000000
             0000005a0c640584005a0d640684005a0e640784005a0f651064088400a6
             000000ab0000000000000000005a11651064098400a6000000ab00000000
             00000000005a12640a84005a1388006601640b84085a14880078015a1553
             00
                        0 MAKE_CELL                0 (__class__)
          
-         147           2 RESUME                   0
+         151           2 RESUME                   0
                        4 LOAD_NAME                0 (__name__)
                        6 STORE_NAME               1 (__module__)
                        8 LOAD_CONST               0 ('Post')
                       10 STORE_NAME               2 (__qualname__)
          
-         148          12 PUSH_NULL
+         152          12 PUSH_NULL
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
          
-         149          60 PUSH_NULL
+         153          60 PUSH_NULL
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
          
-         150         108 PUSH_NULL
+         154         108 PUSH_NULL
                      110 LOAD_NAME               10 (BBCodeTextField)
                      112 PRECALL                  0
                      116 CALL                     0
                      126 STORE_NAME              11 (content)
          
-         152         128 PUSH_NULL
+         156         128 PUSH_NULL
                      130 LOAD_BUILD_CLASS
-                     132 LOAD_CONST               3 (<code object Meta, file "/home/pork/Punkweb/punkweb-bb/punkweb_bb/models.py", line 152>)
+                     132 LOAD_CONST               3 (<code object Meta, file "/home/pork/Punkweb/punkweb-bb/punkweb_bb/models.py", line 156>)
                      134 MAKE_FUNCTION            0
                      136 LOAD_CONST               4 ('Meta')
                      138 PRECALL                  2
                      142 CALL                     2
                      152 STORE_NAME              12 (Meta)
          
-         155         154 LOAD_CONST               5 (<code object __str__, file "/home/pork/Punkweb/punkweb-bb/punkweb_bb/models.py", line 155>)
+         159         154 LOAD_CONST               5 (<code object __str__, file "/home/pork/Punkweb/punkweb-bb/punkweb_bb/models.py", line 159>)
                      156 MAKE_FUNCTION            0
                      158 STORE_NAME              13 (__str__)
          
-         158         160 LOAD_CONST               6 (<code object can_edit, file "/home/pork/Punkweb/punkweb-bb/punkweb_bb/models.py", line 158>)
+         162         160 LOAD_CONST               6 (<code object can_edit, file "/home/pork/Punkweb/punkweb-bb/punkweb_bb/models.py", line 162>)
                      162 MAKE_FUNCTION            0
                      164 STORE_NAME              14 (can_edit)
          
-         161         166 LOAD_CONST               7 (<code object can_delete, file "/home/pork/Punkweb/punkweb-bb/punkweb_bb/models.py", line 161>)
+         165         166 LOAD_CONST               7 (<code object can_delete, file "/home/pork/Punkweb/punkweb-bb/punkweb_bb/models.py", line 165>)
                      168 MAKE_FUNCTION            0
                      170 STORE_NAME              15 (can_delete)
          
-         164         172 LOAD_NAME               16 (property)
+         168         172 LOAD_NAME               16 (property)
          
-         165         174 LOAD_CONST               8 (<code object index, file "/home/pork/Punkweb/punkweb-bb/punkweb_bb/models.py", line 164>)
+         169         174 LOAD_CONST               8 (<code object index, file "/home/pork/Punkweb/punkweb-bb/punkweb_bb/models.py", line 168>)
                      176 MAKE_FUNCTION            0
          
-         164         178 PRECALL                  0
+         168         178 PRECALL                  0
                      182 CALL                     0
          
-         165         192 STORE_NAME              17 (index)
+         169         192 STORE_NAME              17 (index)
          
-         172         194 LOAD_NAME               16 (property)
+         176         194 LOAD_NAME               16 (property)
          
-         173         196 LOAD_CONST               9 (<code object page_number, file "/home/pork/Punkweb/punkweb-bb/punkweb_bb/models.py", line 172>)
+         177         196 LOAD_CONST               9 (<code object page_number, file "/home/pork/Punkweb/punkweb-bb/punkweb_bb/models.py", line 176>)
                      198 MAKE_FUNCTION            0
          
-         172         200 PRECALL                  0
+         176         200 PRECALL                  0
                      204 CALL                     0
          
-         173         214 STORE_NAME              18 (page_number)
+         177         214 STORE_NAME              18 (page_number)
          
-         176         216 LOAD_CONST              10 (<code object get_absolute_url, file "/home/pork/Punkweb/punkweb-bb/punkweb_bb/models.py", line 176>)
+         180         216 LOAD_CONST              10 (<code object get_absolute_url, file "/home/pork/Punkweb/punkweb-bb/punkweb_bb/models.py", line 180>)
                      218 MAKE_FUNCTION            0
                      220 STORE_NAME              19 (get_absolute_url)
          
-         183         222 LOAD_CLOSURE             0 (__class__)
+         187         222 LOAD_CLOSURE             0 (__class__)
                      224 BUILD_TUPLE              1
-                     226 LOAD_CONST              11 (<code object save, file "/home/pork/Punkweb/punkweb-bb/punkweb_bb/models.py", line 183>)
+                     226 LOAD_CONST              11 (<code object save, file "/home/pork/Punkweb/punkweb-bb/punkweb_bb/models.py", line 187>)
                      228 MAKE_FUNCTION            8 (closure)
                      230 STORE_NAME              20 (save)
                      232 LOAD_CLOSURE             0 (__class__)
                      234 COPY                     1
                      236 STORE_NAME              21 (__classcell__)
                      238 RETURN_VALUE
          consts
@@ -1599,48 +1603,48 @@
             ('related_name', 'on_delete')
             code
                argcount  : 0
                nlocals   : 0
                stacksize : 1
                flags     : 0
                code 0x970065005a0164005a0264015a0364025300
-               152           0 RESUME                   0
+               156           0 RESUME                   0
                              2 LOAD_NAME                0 (__name__)
                              4 STORE_NAME               1 (__module__)
                              6 LOAD_CONST               0 ('Post.Meta')
                              8 STORE_NAME               2 (__qualname__)
                
-               153          10 LOAD_CONST               1 (('created_at',))
+               157          10 LOAD_CONST               1 (('created_at',))
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
-               firstlineno 152
+               firstlineno 156
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
-               155           0 RESUME                   0
+               159           0 RESUME                   0
                
-               156           2 LOAD_FAST                0 (self)
+               160           2 LOAD_FAST                0 (self)
                              4 LOAD_ATTR                0 (thread)
                             14 FORMAT_VALUE             0
                             16 LOAD_CONST               1 (' > ')
                             18 LOAD_FAST                0 (self)
                             20 LOAD_ATTR                1 (user)
                             30 FORMAT_VALUE             0
                             32 LOAD_CONST               1 (' > ')
@@ -1654,28 +1658,28 @@
                   ' > '
                names      ('thread', 'user', 'created_at')
                varnames   ('self',)
                freevars   ()
                cellvars   ()
                filename   '/home/pork/Punkweb/punkweb-bb/punkweb_bb/models.py'
                name       '__str__'
-               firstlineno 155
+               firstlineno 159
                lnotab 0x0201
             code
                argcount  : 2
                nlocals   : 2
                stacksize : 3
                flags     : 3
                code
                   0x97007c017c006a0000000000000000006b020000000070147c01a00100
                   000000000000000000000000000000000000006401a6010000ab01000000
                   00000000005300
-               158           0 RESUME                   0
+               162           0 RESUME                   0
                
-               159           2 LOAD_FAST                1 (user)
+               163           2 LOAD_FAST                1 (user)
                              4 LOAD_FAST                0 (self)
                              6 LOAD_ATTR                0 (user)
                             16 COMPARE_OP               2 (==)
                             22 JUMP_IF_TRUE_OR_POP     20 (to 64)
                             24 LOAD_FAST                1 (user)
                             26 LOAD_METHOD              1 (has_perm)
                             48 LOAD_CONST               1 ('punkweb_bb.change_post')
@@ -1687,28 +1691,28 @@
                   'punkweb_bb.change_post'
                names      ('user', 'has_perm')
                varnames   ('self', 'user')
                freevars   ()
                cellvars   ()
                filename   '/home/pork/Punkweb/punkweb-bb/punkweb_bb/models.py'
                name       'can_edit'
-               firstlineno 158
+               firstlineno 162
                lnotab 0x0201
             code
                argcount  : 2
                nlocals   : 2
                stacksize : 3
                flags     : 3
                code
                   0x97007c017c006a0000000000000000006b020000000070147c01a00100
                   000000000000000000000000000000000000006401a6010000ab01000000
                   00000000005300
-               161           0 RESUME                   0
+               165           0 RESUME                   0
                
-               162           2 LOAD_FAST                1 (user)
+               166           2 LOAD_FAST                1 (user)
                              4 LOAD_FAST                0 (self)
                              6 LOAD_ATTR                0 (user)
                             16 COMPARE_OP               2 (==)
                             22 JUMP_IF_TRUE_OR_POP     20 (to 64)
                             24 LOAD_FAST                1 (user)
                             26 LOAD_METHOD              1 (has_perm)
                             48 LOAD_CONST               1 ('punkweb_bb.delete_post')
@@ -1720,41 +1724,41 @@
                   'punkweb_bb.delete_post'
                names      ('user', 'has_perm')
                varnames   ('self', 'user')
                freevars   ()
                cellvars   ()
                filename   '/home/pork/Punkweb/punkweb-bb/punkweb_bb/models.py'
                name       'can_delete'
-               firstlineno 161
+               firstlineno 165
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
-               164           0 RESUME                   0
+               168           0 RESUME                   0
                
-               168           2 LOAD_FAST                0 (self)
+               172           2 LOAD_FAST                0 (self)
                              4 LOAD_ATTR                0 (thread)
                             14 LOAD_ATTR                1 (posts)
                             24 LOAD_METHOD              2 (order_by)
                             46 LOAD_CONST               1 ('created_at')
                             48 PRECALL                  1
                             52 CALL                     1
                             62 STORE_FAST               1 (qs)
                
-               169          64 LOAD_GLOBAL              7 (NULL + list)
+               173          64 LOAD_GLOBAL              7 (NULL + list)
                             76 LOAD_FAST                1 (qs)
                             78 LOAD_METHOD              4 (values_list)
                            100 LOAD_CONST               2 ('id')
                            102 LOAD_CONST               3 (True)
                            104 KW_NAMES                 4
                            106 PRECALL                  2
                            110 CALL                     2
@@ -1763,15 +1767,15 @@
                            134 LOAD_METHOD              5 (index)
                            156 LOAD_FAST                0 (self)
                            158 LOAD_ATTR                6 (id)
                            168 PRECALL                  1
                            172 CALL                     1
                            182 STORE_FAST               2 (index)
                
-               170         184 LOAD_FAST                2 (index)
+               174         184 LOAD_FAST                2 (index)
                            186 LOAD_CONST               5 (1)
                            188 BINARY_OP                0 (+)
                            192 RETURN_VALUE
                consts
                   None
                   'created_at'
                   'id'
@@ -1780,27 +1784,27 @@
                   1
                names      ('thread', 'posts', 'order_by', 'list', 'values_list', 'index', 'id')
                varnames   ('self', 'qs', 'index')
                freevars   ()
                cellvars   ()
                filename   '/home/pork/Punkweb/punkweb-bb/punkweb_bb/models.py'
                name       'index'
-               firstlineno 164
+               firstlineno 168
                lnotab 0x02043e017801
             code
                argcount  : 1
                nlocals   : 1
                stacksize : 4
                flags     : 3
                code
                   0x97007401000000000000000000006a0100000000000000007c006a0200
                   0000000000000064017a0b0000a6010000ab0100000000000000005300
-               172           0 RESUME                   0
+               176           0 RESUME                   0
                
-               174           2 LOAD_GLOBAL              1 (NULL + math)
+               178           2 LOAD_GLOBAL              1 (NULL + math)
                             14 LOAD_ATTR                1 (ceil)
                             24 LOAD_FAST                0 (self)
                             26 LOAD_ATTR                2 (index)
                             36 LOAD_CONST               1 (10)
                             38 BINARY_OP               11 (/)
                             42 PRECALL                  1
                             46 CALL                     1
@@ -1810,67 +1814,67 @@
                   10
                names      ('math', 'ceil', 'index')
                varnames   ('self',)
                freevars   ()
                cellvars   ()
                filename   '/home/pork/Punkweb/punkweb-bb/punkweb_bb/models.py'
                name       'page_number'
-               firstlineno 172
+               firstlineno 176
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
-               176           0 RESUME                   0
+               180           0 RESUME                   0
                
-               177           2 LOAD_GLOBAL              1 (NULL + reverse)
+               181           2 LOAD_GLOBAL              1 (NULL + reverse)
                             14 LOAD_CONST               1 ('punkweb_bb:thread')
                             16 LOAD_FAST                0 (self)
                             18 LOAD_ATTR                1 (thread)
                             28 LOAD_ATTR                2 (id)
                             38 BUILD_LIST               1
                             40 KW_NAMES                 2
                             42 PRECALL                  2
                             46 CALL                     2
                             56 STORE_FAST               1 (thread_url)
                
-               179          58 LOAD_FAST                1 (thread_url)
+               183          58 LOAD_FAST                1 (thread_url)
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
                
-               181         100 LOAD_FAST                1 (thread_url)
+               185         100 LOAD_FAST                1 (thread_url)
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
-               firstlineno 176
+               firstlineno 180
                lnotab 0x020138022a02
             code
                argcount  : 1
                nlocals   : 3
                stacksize : 5
                flags     : 15
                code
@@ -1881,48 +1885,48 @@
                   006a0000000000000000005f0700000000000000007c006a000000000000
                   000000a0080000000000000000000000000000000000000000a6000000ab
                   00000000000000000001000200741300000000000000000000a6000000ab
                   0000000000000000006a0800000000000000007c0169007c02a4018e0101
                   0064005300
                              0 COPY_FREE_VARS           1
                
-               183           2 RESUME                   0
+               187           2 RESUME                   0
                
-               184           4 LOAD_FAST                0 (self)
+               188           4 LOAD_FAST                0 (self)
                              6 LOAD_ATTR                0 (thread)
                             16 LOAD_ATTR                1 (is_closed)
                             26 POP_JUMP_FORWARD_IF_FALSE    15 (to 58)
                
-               185          28 LOAD_GLOBAL              5 (NULL + ValidationError)
+               189          28 LOAD_GLOBAL              5 (NULL + ValidationError)
                             40 LOAD_CONST               1 ('Cannot add posts to a closed thread.')
                             42 PRECALL                  1
                             46 CALL                     1
                             56 RAISE_VARARGS            1
                
-               186     >>   58 LOAD_FAST                0 (self)
+               190     >>   58 LOAD_FAST                0 (self)
                             60 LOAD_ATTR                3 (_state)
                             70 LOAD_ATTR                4 (adding)
                             80 POP_JUMP_FORWARD_IF_FALSE    54 (to 190)
                
-               187          82 LOAD_GLOBAL             11 (NULL + timezone)
+               191          82 LOAD_GLOBAL             11 (NULL + timezone)
                             94 LOAD_ATTR                6 (now)
                            104 PRECALL                  0
                            108 CALL                     0
                            118 LOAD_FAST                0 (self)
                            120 LOAD_ATTR                0 (thread)
                            130 STORE_ATTR               7 (last_post_created_at)
                
-               188         140 LOAD_FAST                0 (self)
+               192         140 LOAD_FAST                0 (self)
                            142 LOAD_ATTR                0 (thread)
                            152 LOAD_METHOD              8 (save)
                            174 PRECALL                  0
                            178 CALL                     0
                            188 POP_TOP
                
-               189     >>  190 PUSH_NULL
+               193     >>  190 PUSH_NULL
                            192 LOAD_GLOBAL             19 (NULL + super)
                            204 PRECALL                  0
                            208 CALL                     0
                            218 LOAD_ATTR                8 (save)
                            228 LOAD_FAST                1 (args)
                            230 BUILD_MAP                0
                            232 LOAD_FAST                2 (kwargs)
@@ -1936,23 +1940,23 @@
                   'Cannot add posts to a closed thread.'
                names      ('thread', 'is_closed', 'ValidationError', '_state', 'adding', 'timezone', 'now', 'last_post_created_at', 'save', 'super')
                varnames   ('self', 'args', 'kwargs')
                freevars   ('__class__',)
                cellvars   ()
                filename   '/home/pork/Punkweb/punkweb-bb/punkweb_bb/models.py'
                name       'save'
-               firstlineno 183
+               firstlineno 187
                lnotab 0x040118011e0118013a013201
          names      ('__name__', '__module__', '__qualname__', 'models', 'ForeignKey', 'Thread', 'CASCADE', 'thread', 'User', 'user', 'BBCodeTextField', 'content', 'Meta', '__str__', 'can_edit', 'can_delete', 'property', 'index', 'page_number', 'get_absolute_url', 'save', '__classcell__')
          varnames   ()
          freevars   ()
          cellvars   ('__class__',)
          filename   '/home/pork/Punkweb/punkweb-bb/punkweb_bb/models.py'
          name       'Post'
-         firstlineno 147
+         firstlineno 151
          lnotab
             0x0c013001300114021a03060306030603020104ff0e010207020104ff0e
             0102030607
       'Post'
       code
          argcount  : 0
          nlocals   : 0
@@ -1960,101 +1964,101 @@
          flags     : 0
          code
             0x970065005a0164005a02020065036a0400000000000000006505640165
             036a060000000000000000ac02a6030000ab0300000000000000005a0702
             0065036a080000000000000000a6000000ab0000000000000000005a0902
             004700640384006404a6020000ab0200000000000000005a0a640584005a
             0b640684005a0c64075300
-         192           0 RESUME                   0
+         196           0 RESUME                   0
                        2 LOAD_NAME                0 (__name__)
                        4 STORE_NAME               1 (__module__)
                        6 LOAD_CONST               0 ('Shout')
                        8 STORE_NAME               2 (__qualname__)
          
-         193          10 PUSH_NULL
+         197          10 PUSH_NULL
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
          
-         194          58 PUSH_NULL
+         198          58 PUSH_NULL
                       60 LOAD_NAME                3 (models)
                       62 LOAD_ATTR                8 (TextField)
                       72 PRECALL                  0
                       76 CALL                     0
                       86 STORE_NAME               9 (content)
          
-         196          88 PUSH_NULL
+         200          88 PUSH_NULL
                       90 LOAD_BUILD_CLASS
-                      92 LOAD_CONST               3 (<code object Meta, file "/home/pork/Punkweb/punkweb-bb/punkweb_bb/models.py", line 196>)
+                      92 LOAD_CONST               3 (<code object Meta, file "/home/pork/Punkweb/punkweb-bb/punkweb_bb/models.py", line 200>)
                       94 MAKE_FUNCTION            0
                       96 LOAD_CONST               4 ('Meta')
                       98 PRECALL                  2
                      102 CALL                     2
                      112 STORE_NAME              10 (Meta)
          
-         199         114 LOAD_CONST               5 (<code object __str__, file "/home/pork/Punkweb/punkweb-bb/punkweb_bb/models.py", line 199>)
+         203         114 LOAD_CONST               5 (<code object __str__, file "/home/pork/Punkweb/punkweb-bb/punkweb_bb/models.py", line 203>)
                      116 MAKE_FUNCTION            0
                      118 STORE_NAME              11 (__str__)
          
-         202         120 LOAD_CONST               6 (<code object can_delete, file "/home/pork/Punkweb/punkweb-bb/punkweb_bb/models.py", line 202>)
+         206         120 LOAD_CONST               6 (<code object can_delete, file "/home/pork/Punkweb/punkweb-bb/punkweb_bb/models.py", line 206>)
                      122 MAKE_FUNCTION            0
                      124 STORE_NAME              12 (can_delete)
                      126 LOAD_CONST               7 (None)
                      128 RETURN_VALUE
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
-               196           0 RESUME                   0
+               200           0 RESUME                   0
                              2 LOAD_NAME                0 (__name__)
                              4 STORE_NAME               1 (__module__)
                              6 LOAD_CONST               0 ('Shout.Meta')
                              8 STORE_NAME               2 (__qualname__)
                
-               197          10 LOAD_CONST               1 (('-created_at',))
+               201          10 LOAD_CONST               1 (('-created_at',))
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
-               firstlineno 196
+               firstlineno 200
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
-               199           0 RESUME                   0
+               203           0 RESUME                   0
                
-               200           2 LOAD_FAST                0 (self)
+               204           2 LOAD_FAST                0 (self)
                              4 LOAD_ATTR                0 (user)
                             14 FORMAT_VALUE             0
                             16 LOAD_CONST               1 (' > ')
                             18 LOAD_FAST                0 (self)
                             20 LOAD_ATTR                1 (created_at)
                             30 FORMAT_VALUE             0
                             32 BUILD_STRING             3
@@ -2064,28 +2068,28 @@
                   ' > '
                names      ('user', 'created_at')
                varnames   ('self',)
                freevars   ()
                cellvars   ()
                filename   '/home/pork/Punkweb/punkweb-bb/punkweb_bb/models.py'
                name       '__str__'
-               firstlineno 199
+               firstlineno 203
                lnotab 0x0201
             code
                argcount  : 2
                nlocals   : 2
                stacksize : 3
                flags     : 3
                code
                   0x97007c017c006a0000000000000000006b020000000070147c01a00100
                   000000000000000000000000000000000000006401a6010000ab01000000
                   00000000005300
-               202           0 RESUME                   0
+               206           0 RESUME                   0
                
-               203           2 LOAD_FAST                1 (user)
+               207           2 LOAD_FAST                1 (user)
                              4 LOAD_FAST                0 (self)
                              6 LOAD_ATTR                0 (user)
                             16 COMPARE_OP               2 (==)
                             22 JUMP_IF_TRUE_OR_POP     20 (to 64)
                             24 LOAD_FAST                1 (user)
                             26 LOAD_METHOD              1 (has_perm)
                             48 LOAD_CONST               1 ('punkweb_bb.delete_shout')
@@ -2097,29 +2101,29 @@
                   'punkweb_bb.delete_shout'
                names      ('user', 'has_perm')
                varnames   ('self', 'user')
                freevars   ()
                cellvars   ()
                filename   '/home/pork/Punkweb/punkweb-bb/punkweb_bb/models.py'
                name       'can_delete'
-               firstlineno 202
+               firstlineno 206
                lnotab 0x0201
             None
          names      ('__name__', '__module__', '__qualname__', 'models', 'ForeignKey', 'User', 'CASCADE', 'user', 'TextField', 'content', 'Meta', '__str__', 'can_delete')
          varnames   ()
          freevars   ()
          cellvars   ()
          filename   '/home/pork/Punkweb/punkweb-bb/punkweb_bb/models.py'
          name       'Shout'
-         firstlineno 192
+         firstlineno 196
          lnotab 0x0a0130011e021a030603
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
-      051e171e121e281e2b1e2d
+      051e171e121e281e2f1e2d
```

### Comparing `punkweb_bb-0.2.0/punkweb_bb/__pycache__/pagination.cpython-311.pyc` & `punkweb_bb-0.2.1/punkweb_bb/__pycache__/pagination.cpython-311.pyc`

 * *Files identical despite different names*

### Comparing `punkweb_bb-0.2.0/punkweb_bb/__pycache__/parsers.cpython-311.pyc` & `punkweb_bb-0.2.1/punkweb_bb/__pycache__/parsers.cpython-311.pyc`

 * *Files identical despite different names*

### Comparing `punkweb_bb-0.2.0/punkweb_bb/__pycache__/settings.cpython-311.pyc` & `punkweb_bb-0.2.1/punkweb_bb/__pycache__/settings.cpython-311.pyc`

 * *Files 10% similar despite different names*

#### Python bytecode

```diff
@@ -1,10 +1,10 @@
 magic:    0xa70d0d0a
-moddate:  0xd55e3c66 (Thu May  9 05:27:49 2024 UTC)
-files sz: 517
+moddate:  0xe6b05666 (Wed May 29 04:36:54 2024 UTC)
+files sz: 561
 code
    argcount  : 0
    nlocals   : 0
    stacksize : 5
    flags     : 0
    code
       0x9700640064016c006d015a01010002006502650164026900a6030000ab
@@ -14,15 +14,17 @@
       000000000000005a066503a0040000000000000000000000000000000000
       00000064076408a6020000ab0200000000000000005a076503a004000000
       00000000000000000000000000000000006409640aa6020000ab02000000
       00000000005a086503a00400000000000000000000000000000000000000
       00640b640ca6020000ab0200000000000000005a096503a0040000000000
       000000000000000000000000000000640d640ea6020000ab020000000000
       0000005a0a6503a004000000000000000000000000000000000000000064
-      0f6410a6020000ab0200000000000000005a0b64105300
+      0f6410a6020000ab0200000000000000005a0b6503a00400000000000000
+      000000000000000000000000006411640aa6020000ab0200000000000000
+      005a0c640a5300
      0           0 RESUME                   0
    
      1           2 LOAD_CONST               0 (0)
                  4 LOAD_CONST               1 (('settings',))
                  6 IMPORT_NAME              0 (django.conf)
                  8 IMPORT_FROM              1 (settings)
                 10 STORE_NAME               1 (settings)
@@ -59,64 +61,73 @@
                154 LOAD_CONST               8 ('punkweb_bb/favicon.ico')
                156 PRECALL                  2
                160 CALL                     2
                170 STORE_NAME               7 (FAVICON)
    
      8         172 LOAD_NAME                3 (PUNKWEB_BB)
                174 LOAD_METHOD              4 (get)
-               196 LOAD_CONST               9 ('SHOUTBOX_ENABLED')
-               198 LOAD_CONST              10 (True)
+               196 LOAD_CONST               9 ('OG_IMAGE')
+               198 LOAD_CONST              10 (None)
                200 PRECALL                  2
                204 CALL                     2
-               214 STORE_NAME               8 (SHOUTBOX_ENABLED)
+               214 STORE_NAME               8 (OG_IMAGE)
    
      9         216 LOAD_NAME                3 (PUNKWEB_BB)
                218 LOAD_METHOD              4 (get)
-               240 LOAD_CONST              11 ('DISCORD_WIDGET_ENABLED')
-               242 LOAD_CONST              12 (False)
+               240 LOAD_CONST              11 ('SHOUTBOX_ENABLED')
+               242 LOAD_CONST              12 (True)
                244 PRECALL                  2
                248 CALL                     2
-               258 STORE_NAME               9 (DISCORD_WIDGET_ENABLED)
+               258 STORE_NAME               9 (SHOUTBOX_ENABLED)
    
     10         260 LOAD_NAME                3 (PUNKWEB_BB)
                262 LOAD_METHOD              4 (get)
-               284 LOAD_CONST              13 ('DISCORD_WIDGET_THEME')
-               286 LOAD_CONST              14 ('dark')
+               284 LOAD_CONST              13 ('DISCORD_WIDGET_ENABLED')
+               286 LOAD_CONST              14 (False)
                288 PRECALL                  2
                292 CALL                     2
-               302 STORE_NAME              10 (DISCORD_WIDGET_THEME)
+               302 STORE_NAME              10 (DISCORD_WIDGET_ENABLED)
    
     11         304 LOAD_NAME                3 (PUNKWEB_BB)
                306 LOAD_METHOD              4 (get)
-               328 LOAD_CONST              15 ('DISCORD_SERVER_ID')
-               330 LOAD_CONST              16 (None)
+               328 LOAD_CONST              15 ('DISCORD_WIDGET_THEME')
+               330 LOAD_CONST              16 ('dark')
                332 PRECALL                  2
                336 CALL                     2
-               346 STORE_NAME              11 (DISCORD_SERVER_ID)
-               348 LOAD_CONST              16 (None)
-               350 RETURN_VALUE
+               346 STORE_NAME              11 (DISCORD_WIDGET_THEME)
+   
+    12         348 LOAD_NAME                3 (PUNKWEB_BB)
+               350 LOAD_METHOD              4 (get)
+               372 LOAD_CONST              17 ('DISCORD_SERVER_ID')
+               374 LOAD_CONST              10 (None)
+               376 PRECALL                  2
+               380 CALL                     2
+               390 STORE_NAME              12 (DISCORD_SERVER_ID)
+               392 LOAD_CONST              10 (None)
+               394 RETURN_VALUE
    consts
       0
       ('settings',)
       'PUNKWEB_BB'
       'SITE_NAME'
       'PUNKWEB'
       'SITE_TITLE'
       'PunkwebBB'
       'FAVICON'
       'punkweb_bb/favicon.ico'
+      'OG_IMAGE'
+      None
       'SHOUTBOX_ENABLED'
       True
       'DISCORD_WIDGET_ENABLED'
       False
       'DISCORD_WIDGET_THEME'
       'dark'
       'DISCORD_SERVER_ID'
-      None
-   names      ('django.conf', 'settings', 'getattr', 'PUNKWEB_BB', 'get', 'SITE_NAME', 'SITE_TITLE', 'FAVICON', 'SHOUTBOX_ENABLED', 'DISCORD_WIDGET_ENABLED', 'DISCORD_WIDGET_THEME', 'DISCORD_SERVER_ID')
+   names      ('django.conf', 'settings', 'getattr', 'PUNKWEB_BB', 'get', 'SITE_NAME', 'SITE_TITLE', 'FAVICON', 'OG_IMAGE', 'SHOUTBOX_ENABLED', 'DISCORD_WIDGET_ENABLED', 'DISCORD_WIDGET_THEME', 'DISCORD_SERVER_ID')
    varnames   ()
    freevars   ()
    cellvars   ()
    filename   '/home/pork/Punkweb/punkweb-bb/punkweb_bb/settings.py'
    name       '<module>'
    firstlineno 1
-   lnotab 0x00ff02010c021a022c012c012c012c012c012c01
+   lnotab 0x00ff02010c021a022c012c012c012c012c012c012c01
```

### Comparing `punkweb_bb-0.2.0/punkweb_bb/__pycache__/signals.cpython-311.pyc` & `punkweb_bb-0.2.1/punkweb_bb/__pycache__/signals.cpython-311.pyc`

 * *Files identical despite different names*

### Comparing `punkweb_bb-0.2.0/punkweb_bb/__pycache__/tests.cpython-311.pyc` & `punkweb_bb-0.2.1/punkweb_bb/__pycache__/tests.cpython-311.pyc`

 * *Files identical despite different names*

### Comparing `punkweb_bb-0.2.0/punkweb_bb/__pycache__/urls.cpython-311.pyc` & `punkweb_bb-0.2.1/punkweb_bb/__pycache__/urls.cpython-311.pyc`

 * *Files 7% similar despite different names*

#### Python bytecode

```diff
@@ -1,14 +1,14 @@
 magic:    0xa70d0d0a
-moddate:  0x353a5666 (Tue May 28 20:10:29 2024 UTC)
-files sz: 2415
+moddate:  0x95815666 (Wed May 29 01:15:01 2024 UTC)
+files sz: 2587
 code
    argcount  : 0
    nlocals   : 0
-   stacksize : 29
+   stacksize : 31
    flags     : 0
    code
       0x9700640064016c006d015a010100640064026c026d035a03010064035a
       0402006501640465036a0500000000000000006405ac06a6030000ab0300
       0000000000000002006501640765036a0600000000000000006408ac06a6
       030000ab03000000000000000002006501640965036a0700000000000000
       00640aac06a6030000ab03000000000000000002006501640b65036a0800
@@ -34,15 +34,17 @@
       2b65036a180000000000000000642cac06a6030000ab0300000000000000
       0002006501642d65036a190000000000000000642eac06a6030000ab0300
       0000000000000002006501642f65036a1a00000000000000006430ac06a6
       030000ab03000000000000000002006501643165036a1b00000000000000
       006432ac06a6030000ab03000000000000000002006501643365036a1c00
       000000000000006434ac06a6030000ab0300000000000000000200650164
       3565036a1d00000000000000006436ac06a6030000ab0300000000000000
-      0067195a1e64375300
+      0002006501643765036a1e00000000000000006438ac06a6030000ab0300
+      0000000000000002006501643965036a1f0000000000000000643aac06a6
+      030000ab030000000000000000671b5a20643b5300
      0           0 RESUME                   0
    
      1           2 LOAD_CONST               0 (0)
                  4 LOAD_CONST               1 (('path',))
                  6 IMPORT_NAME              0 (django.urls)
                  8 IMPORT_FROM              1 (path)
                 10 STORE_NAME               1 (path)
@@ -282,76 +284,96 @@
    
     57         698 KW_NAMES                 6
                700 PRECALL                  3
                704 CALL                     3
    
     62         714 PUSH_NULL
                716 LOAD_NAME                1 (path)
-               718 LOAD_CONST              43 ('post/<str:post_id>/delete/')
+               718 LOAD_CONST              43 ('thread/<str:thread_id>/pin/')
                720 LOAD_NAME                3 (views)
-               722 LOAD_ATTR               24 (post_delete_view)
-               732 LOAD_CONST              44 ('post_delete')
+               722 LOAD_ATTR               24 (thread_pin_view)
+               732 LOAD_CONST              44 ('thread_pin')
                734 KW_NAMES                 6
                736 PRECALL                  3
                740 CALL                     3
    
     63         750 PUSH_NULL
                752 LOAD_NAME                1 (path)
-               754 LOAD_CONST              45 ('post/<str:post_id>/update/')
+               754 LOAD_CONST              45 ('thread/<str:thread_id>/close/')
                756 LOAD_NAME                3 (views)
-               758 LOAD_ATTR               25 (post_update_view)
-               768 LOAD_CONST              46 ('post_update')
+               758 LOAD_ATTR               25 (thread_close_view)
+               768 LOAD_CONST              46 ('thread_close')
                770 KW_NAMES                 6
                772 PRECALL                  3
                776 CALL                     3
    
     64         786 PUSH_NULL
                788 LOAD_NAME                1 (path)
-               790 LOAD_CONST              47 ('shout-list/')
+               790 LOAD_CONST              47 ('post/<str:post_id>/delete/')
                792 LOAD_NAME                3 (views)
-               794 LOAD_ATTR               26 (shout_list_view)
-               804 LOAD_CONST              48 ('shout_list')
+               794 LOAD_ATTR               26 (post_delete_view)
+               804 LOAD_CONST              48 ('post_delete')
                806 KW_NAMES                 6
                808 PRECALL                  3
                812 CALL                     3
    
     65         822 PUSH_NULL
                824 LOAD_NAME                1 (path)
-               826 LOAD_CONST              49 ('shout-create/')
+               826 LOAD_CONST              49 ('post/<str:post_id>/update/')
                828 LOAD_NAME                3 (views)
-               830 LOAD_ATTR               27 (shout_create_view)
-               840 LOAD_CONST              50 ('shout_create')
+               830 LOAD_ATTR               27 (post_update_view)
+               840 LOAD_CONST              50 ('post_update')
                842 KW_NAMES                 6
                844 PRECALL                  3
                848 CALL                     3
    
     66         858 PUSH_NULL
                860 LOAD_NAME                1 (path)
-               862 LOAD_CONST              51 ('shout/<str:shout_id>/delete/')
+               862 LOAD_CONST              51 ('shout-list/')
                864 LOAD_NAME                3 (views)
-               866 LOAD_ATTR               28 (shout_delete_view)
-               876 LOAD_CONST              52 ('shout_delete')
+               866 LOAD_ATTR               28 (shout_list_view)
+               876 LOAD_CONST              52 ('shout_list')
                878 KW_NAMES                 6
                880 PRECALL                  3
                884 CALL                     3
    
     67         894 PUSH_NULL
                896 LOAD_NAME                1 (path)
-               898 LOAD_CONST              53 ('bbcode/')
+               898 LOAD_CONST              53 ('shout-create/')
                900 LOAD_NAME                3 (views)
-               902 LOAD_ATTR               29 (bbcode_view)
-               912 LOAD_CONST              54 ('bbcode')
+               902 LOAD_ATTR               29 (shout_create_view)
+               912 LOAD_CONST              54 ('shout_create')
                914 KW_NAMES                 6
                916 PRECALL                  3
                920 CALL                     3
    
-     6         930 BUILD_LIST              25
-               932 STORE_NAME              30 (urlpatterns)
-               934 LOAD_CONST              55 (None)
-               936 RETURN_VALUE
+    68         930 PUSH_NULL
+               932 LOAD_NAME                1 (path)
+               934 LOAD_CONST              55 ('shout/<str:shout_id>/delete/')
+               936 LOAD_NAME                3 (views)
+               938 LOAD_ATTR               30 (shout_delete_view)
+               948 LOAD_CONST              56 ('shout_delete')
+               950 KW_NAMES                 6
+               952 PRECALL                  3
+               956 CALL                     3
+   
+    69         966 PUSH_NULL
+               968 LOAD_NAME                1 (path)
+               970 LOAD_CONST              57 ('bbcode/')
+               972 LOAD_NAME                3 (views)
+               974 LOAD_ATTR               31 (bbcode_view)
+               984 LOAD_CONST              58 ('bbcode')
+               986 KW_NAMES                 6
+               988 PRECALL                  3
+               992 CALL                     3
+   
+     6        1002 BUILD_LIST              27
+              1004 STORE_NAME              32 (urlpatterns)
+              1006 LOAD_CONST              59 (None)
+              1008 RETURN_VALUE
    consts
       0
       ('path',)
       ('views',)
       'punkweb_bb'
       ''
       'index'
@@ -388,33 +410,37 @@
       'thread'
       'thread/<str:thread_id>/delete/'
       'thread_delete'
       'thread/<str:thread_id>/update/'
       'thread_update'
       'thread/<str:thread_id>/create-post/'
       'post_create'
+      'thread/<str:thread_id>/pin/'
+      'thread_pin'
+      'thread/<str:thread_id>/close/'
+      'thread_close'
       'post/<str:post_id>/delete/'
       'post_delete'
       'post/<str:post_id>/update/'
       'post_update'
       'shout-list/'
       'shout_list'
       'shout-create/'
       'shout_create'
       'shout/<str:shout_id>/delete/'
       'shout_delete'
       'bbcode/'
       'bbcode'
       None
-   names      ('django.urls', 'path', 'punkweb_bb', 'views', 'app_name', 'index_view', 'signup_view', 'login_view', 'logout_view', 'settings_view', 'members_view', 'profile_view', 'category_create_view', 'category_update_view', 'category_delete_view', 'subcategory_view', 'subcategory_create_view', 'subcategory_update_view', 'subcategory_delete_view', 'thread_create_view', 'thread_view', 'thread_delete_view', 'thread_update_view', 'post_create_view', 'post_delete_view', 'post_update_view', 'shout_list_view', 'shout_create_view', 'shout_delete_view', 'bbcode_view', 'urlpatterns')
+   names      ('django.urls', 'path', 'punkweb_bb', 'views', 'app_name', 'index_view', 'signup_view', 'login_view', 'logout_view', 'settings_view', 'members_view', 'profile_view', 'category_create_view', 'category_update_view', 'category_delete_view', 'subcategory_view', 'subcategory_create_view', 'subcategory_update_view', 'subcategory_delete_view', 'thread_create_view', 'thread_view', 'thread_delete_view', 'thread_update_view', 'post_create_view', 'thread_pin_view', 'thread_close_view', 'post_delete_view', 'post_update_view', 'shout_list_view', 'shout_create_view', 'shout_delete_view', 'bbcode_view', 'urlpatterns')
    varnames   ()
    freevars   ()
    cellvars   ()
    filename   '/home/pork/Punkweb/punkweb-bb/punkweb_bb/urls.py'
    name       '<module>'
    firstlineno 1
    lnotab
       0x00ff02010c020c02040224012401240124012401240124012401040102
       010c0102fd1005040102010c0102fd1005040102010c0102fd1005040102
       010c0102fd1005040102010c0102fd1005040102010c0102fd1005040102
       010c0102fd10052401040110ff1003040110ff1003040102010c0102fd10
-      052401240124012401240124c3
+      05240124012401240124012401240124c1
```

### Comparing `punkweb_bb-0.2.0/punkweb_bb/__pycache__/utils.cpython-311.pyc` & `punkweb_bb-0.2.1/punkweb_bb/__pycache__/utils.cpython-311.pyc`

 * *Files identical despite different names*

### Comparing `punkweb_bb-0.2.0/punkweb_bb/__pycache__/views.cpython-311.pyc` & `punkweb_bb-0.2.1/punkweb_bb/__pycache__/views.cpython-311.pyc`

 * *Files 4% similar despite different names*

#### Python bytecode

```diff
@@ -1,10 +1,10 @@
 magic:    0xa70d0d0a
-moddate:  0x28565666 (Tue May 28 22:09:44 2024 UTC)
-files sz: 16610
+moddate:  0x34825666 (Wed May 29 01:17:40 2024 UTC)
+files sz: 17400
 code
    argcount  : 0
    nlocals   : 0
    stacksize : 3
    flags     : 0
    code
       0x9700640064016c005a00640064026c016d025a026d035a036d045a046d
@@ -30,18 +30,20 @@
       00a6000000ab0000000000000000005a38641f84005a39020065076414ac
       15a6010000ab01000000000000000064208400a6000000ab000000000000
       0000005a3a020065076414ac15a6010000ab010000000000000000642184
       00a6000000ab0000000000000000005a3b020065076414ac15a6010000ab
       01000000000000000064228400a6000000ab0000000000000000005a3c02
       0065076414ac15a6010000ab01000000000000000064238400a6000000ab
       0000000000000000005a3d020065076414ac15a6010000ab010000000000
-      00000064248400a6000000ab0000000000000000005a3e642584005a3f64
-      2684005a40642784005a41020065076414ac15a6010000ab010000000000
-      00000064288400a6000000ab0000000000000000005a42642984005a4364
-      015300
+      00000064248400a6000000ab0000000000000000005a3e020065076414ac
+      15a6010000ab01000000000000000064258400a6000000ab000000000000
+      0000005a3f020065076414ac15a6010000ab010000000000000000642684
+      00a6000000ab0000000000000000005a40642784005a41642884005a4264
+      2984005a43020065076414ac15a6010000ab010000000000000000642a84
+      00a6000000ab0000000000000000005a44642b84005a4564015300
      0           0 RESUME                   0
    
      1           2 LOAD_CONST               0 (0)
                  4 LOAD_CONST               1 (None)
                  6 IMPORT_NAME              0 (datetime)
                  8 STORE_NAME               0 (datetime)
    
@@ -352,84 +354,114 @@
    409         706 PUSH_NULL
                708 LOAD_NAME                7 (login_required)
                710 LOAD_CONST              20 ('/login/')
                712 KW_NAMES                21
                714 PRECALL                  1
                718 CALL                     1
    
-   410         728 LOAD_CONST              34 (<code object post_create_view, file "/home/pork/Punkweb/punkweb-bb/punkweb_bb/views.py", line 409>)
+   410         728 LOAD_CONST              34 (<code object thread_pin_view, file "/home/pork/Punkweb/punkweb-bb/punkweb_bb/views.py", line 409>)
                730 MAKE_FUNCTION            0
    
    409         732 PRECALL                  0
                736 CALL                     0
    
-   410         746 STORE_NAME              60 (post_create_view)
+   410         746 STORE_NAME              60 (thread_pin_view)
    
-   429         748 PUSH_NULL
+   422         748 PUSH_NULL
                750 LOAD_NAME                7 (login_required)
                752 LOAD_CONST              20 ('/login/')
                754 KW_NAMES                21
                756 PRECALL                  1
                760 CALL                     1
    
-   430         770 LOAD_CONST              35 (<code object post_update_view, file "/home/pork/Punkweb/punkweb-bb/punkweb_bb/views.py", line 429>)
+   423         770 LOAD_CONST              35 (<code object thread_close_view, file "/home/pork/Punkweb/punkweb-bb/punkweb_bb/views.py", line 422>)
                772 MAKE_FUNCTION            0
    
-   429         774 PRECALL                  0
+   422         774 PRECALL                  0
                778 CALL                     0
    
-   430         788 STORE_NAME              61 (post_update_view)
+   423         788 STORE_NAME              61 (thread_close_view)
    
-   454         790 PUSH_NULL
+   435         790 PUSH_NULL
                792 LOAD_NAME                7 (login_required)
                794 LOAD_CONST              20 ('/login/')
                796 KW_NAMES                21
                798 PRECALL                  1
                802 CALL                     1
    
-   455         812 LOAD_CONST              36 (<code object post_delete_view, file "/home/pork/Punkweb/punkweb-bb/punkweb_bb/views.py", line 454>)
+   436         812 LOAD_CONST              36 (<code object post_create_view, file "/home/pork/Punkweb/punkweb-bb/punkweb_bb/views.py", line 435>)
                814 MAKE_FUNCTION            0
    
-   454         816 PRECALL                  0
+   435         816 PRECALL                  0
                820 CALL                     0
    
-   455         830 STORE_NAME              62 (post_delete_view)
+   436         830 STORE_NAME              62 (post_create_view)
    
-   473         832 LOAD_CONST              37 (<code object current_shouts, file "/home/pork/Punkweb/punkweb-bb/punkweb_bb/views.py", line 473>)
-               834 MAKE_FUNCTION            0
-               836 STORE_NAME              63 (current_shouts)
-   
-   479         838 LOAD_CONST              38 (<code object shout_list_view, file "/home/pork/Punkweb/punkweb-bb/punkweb_bb/views.py", line 479>)
-               840 MAKE_FUNCTION            0
-               842 STORE_NAME              64 (shout_list_view)
-   
-   488         844 LOAD_CONST              39 (<code object shout_create_view, file "/home/pork/Punkweb/punkweb-bb/punkweb_bb/views.py", line 488>)
-               846 MAKE_FUNCTION            0
-               848 STORE_NAME              65 (shout_create_view)
-   
-   511         850 PUSH_NULL
-               852 LOAD_NAME                7 (login_required)
-               854 LOAD_CONST              20 ('/login/')
-               856 KW_NAMES                21
-               858 PRECALL                  1
-               862 CALL                     1
-   
-   512         872 LOAD_CONST              40 (<code object shout_delete_view, file "/home/pork/Punkweb/punkweb-bb/punkweb_bb/views.py", line 511>)
-               874 MAKE_FUNCTION            0
-   
-   511         876 PRECALL                  0
-               880 CALL                     0
-   
-   512         890 STORE_NAME              66 (shout_delete_view)
-   
-   530         892 LOAD_CONST              41 (<code object bbcode_view, file "/home/pork/Punkweb/punkweb-bb/punkweb_bb/views.py", line 530>)
-               894 MAKE_FUNCTION            0
-               896 STORE_NAME              67 (bbcode_view)
-               898 LOAD_CONST               1 (None)
-               900 RETURN_VALUE
+   455         832 PUSH_NULL
+               834 LOAD_NAME                7 (login_required)
+               836 LOAD_CONST              20 ('/login/')
+               838 KW_NAMES                21
+               840 PRECALL                  1
+               844 CALL                     1
+   
+   456         854 LOAD_CONST              37 (<code object post_update_view, file "/home/pork/Punkweb/punkweb-bb/punkweb_bb/views.py", line 455>)
+               856 MAKE_FUNCTION            0
+   
+   455         858 PRECALL                  0
+               862 CALL                     0
+   
+   456         872 STORE_NAME              63 (post_update_view)
+   
+   480         874 PUSH_NULL
+               876 LOAD_NAME                7 (login_required)
+               878 LOAD_CONST              20 ('/login/')
+               880 KW_NAMES                21
+               882 PRECALL                  1
+               886 CALL                     1
+   
+   481         896 LOAD_CONST              38 (<code object post_delete_view, file "/home/pork/Punkweb/punkweb-bb/punkweb_bb/views.py", line 480>)
+               898 MAKE_FUNCTION            0
+   
+   480         900 PRECALL                  0
+               904 CALL                     0
+   
+   481         914 STORE_NAME              64 (post_delete_view)
+   
+   499         916 LOAD_CONST              39 (<code object current_shouts, file "/home/pork/Punkweb/punkweb-bb/punkweb_bb/views.py", line 499>)
+               918 MAKE_FUNCTION            0
+               920 STORE_NAME              65 (current_shouts)
+   
+   505         922 LOAD_CONST              40 (<code object shout_list_view, file "/home/pork/Punkweb/punkweb-bb/punkweb_bb/views.py", line 505>)
+               924 MAKE_FUNCTION            0
+               926 STORE_NAME              66 (shout_list_view)
+   
+   514         928 LOAD_CONST              41 (<code object shout_create_view, file "/home/pork/Punkweb/punkweb-bb/punkweb_bb/views.py", line 514>)
+               930 MAKE_FUNCTION            0
+               932 STORE_NAME              67 (shout_create_view)
+   
+   537         934 PUSH_NULL
+               936 LOAD_NAME                7 (login_required)
+               938 LOAD_CONST              20 ('/login/')
+               940 KW_NAMES                21
+               942 PRECALL                  1
+               946 CALL                     1
+   
+   538         956 LOAD_CONST              42 (<code object shout_delete_view, file "/home/pork/Punkweb/punkweb-bb/punkweb_bb/views.py", line 537>)
+               958 MAKE_FUNCTION            0
+   
+   537         960 PRECALL                  0
+               964 CALL                     0
+   
+   538         974 STORE_NAME              68 (shout_delete_view)
+   
+   556         976 LOAD_CONST              43 (<code object bbcode_view, file "/home/pork/Punkweb/punkweb-bb/punkweb_bb/views.py", line 556>)
+               978 MAKE_FUNCTION            0
+               980 STORE_NAME              69 (bbcode_view)
+               982 LOAD_CONST               1 (None)
+               984 RETURN_VALUE
    consts
       0
       None
       ('authenticate', 'get_user_model', 'login', 'logout')
       ('login_required',)
       ('HttpResponseForbidden',)
       ('get_object_or_404', 'redirect', 'render')
@@ -2423,14 +2455,158 @@
          cellvars   ()
          filename   '/home/pork/Punkweb/punkweb-bb/punkweb_bb/views.py'
          name       'thread_delete_view'
          firstlineno 388
          lnotab 0x02022c0234010c0102ff1004160128024c0304ff0404
       code
          argcount  : 2
+         nlocals   : 3
+         stacksize : 4
+         flags     : 3
+         code
+            0x97007401000000000000000000007402000000000000000000007c01ac
+            01a6020000ab0200000000000000007d027c006a020000000000000000a0
+            0300000000000000000000000000000000000000006402a6010000ab0100
+            00000000000000730f7409000000000000000000006403a6010000ab0100
+            0000000000000053007c026a0500000000000000000c007c025f05000000
+            00000000007c02a0060000000000000000000000000000000000000000a6
+            000000ab0000000000000000000100740f000000000000000000007c02a0
+            080000000000000000000000000000000000000000a6000000ab00000000
+            0000000000a6010000ab0100000000000000005300
+         409           0 RESUME                   0
+         
+         411           2 LOAD_GLOBAL              1 (NULL + get_object_or_404)
+                      14 LOAD_GLOBAL              2 (Thread)
+                      26 LOAD_FAST                1 (thread_id)
+                      28 KW_NAMES                 1
+                      30 PRECALL                  2
+                      34 CALL                     2
+                      44 STORE_FAST               2 (thread)
+         
+         413          46 LOAD_FAST                0 (request)
+                      48 LOAD_ATTR                2 (user)
+                      58 LOAD_METHOD              3 (has_perm)
+                      80 LOAD_CONST               2 ('punkweb_bb.pin_thread')
+                      82 PRECALL                  1
+                      86 CALL                     1
+                      96 POP_JUMP_FORWARD_IF_TRUE    15 (to 128)
+         
+         414          98 LOAD_GLOBAL              9 (NULL + HttpResponseForbidden)
+                     110 LOAD_CONST               3 ('You do not have permission to pin threads.')
+                     112 PRECALL                  1
+                     116 CALL                     1
+                     126 RETURN_VALUE
+         
+         416     >>  128 LOAD_FAST                2 (thread)
+                     130 LOAD_ATTR                5 (is_pinned)
+                     140 UNARY_NOT
+                     142 LOAD_FAST                2 (thread)
+                     144 STORE_ATTR               5 (is_pinned)
+         
+         417         154 LOAD_FAST                2 (thread)
+                     156 LOAD_METHOD              6 (save)
+                     178 PRECALL                  0
+                     182 CALL                     0
+                     192 POP_TOP
+         
+         419         194 LOAD_GLOBAL             15 (NULL + htmx_redirect)
+                     206 LOAD_FAST                2 (thread)
+                     208 LOAD_METHOD              8 (get_absolute_url)
+                     230 PRECALL                  0
+                     234 CALL                     0
+                     244 PRECALL                  1
+                     248 CALL                     1
+                     258 RETURN_VALUE
+         consts
+            None
+            ('pk',)
+            'punkweb_bb.pin_thread'
+            'You do not have permission to pin threads.'
+         names      ('get_object_or_404', 'Thread', 'user', 'has_perm', 'HttpResponseForbidden', 'is_pinned', 'save', 'htmx_redirect', 'get_absolute_url')
+         varnames   ('request', 'thread_id', 'thread')
+         freevars   ()
+         cellvars   ()
+         filename   '/home/pork/Punkweb/punkweb-bb/punkweb_bb/views.py'
+         name       'thread_pin_view'
+         firstlineno 409
+         lnotab 0x02022c0234011e021a012802
+      code
+         argcount  : 2
+         nlocals   : 3
+         stacksize : 4
+         flags     : 3
+         code
+            0x97007401000000000000000000007402000000000000000000007c01ac
+            01a6020000ab0200000000000000007d027c006a020000000000000000a0
+            0300000000000000000000000000000000000000006402a6010000ab0100
+            00000000000000730f7409000000000000000000006403a6010000ab0100
+            0000000000000053007c026a0500000000000000000c007c025f05000000
+            00000000007c02a0060000000000000000000000000000000000000000a6
+            000000ab0000000000000000000100740f000000000000000000007c02a0
+            080000000000000000000000000000000000000000a6000000ab00000000
+            0000000000a6010000ab0100000000000000005300
+         422           0 RESUME                   0
+         
+         424           2 LOAD_GLOBAL              1 (NULL + get_object_or_404)
+                      14 LOAD_GLOBAL              2 (Thread)
+                      26 LOAD_FAST                1 (thread_id)
+                      28 KW_NAMES                 1
+                      30 PRECALL                  2
+                      34 CALL                     2
+                      44 STORE_FAST               2 (thread)
+         
+         426          46 LOAD_FAST                0 (request)
+                      48 LOAD_ATTR                2 (user)
+                      58 LOAD_METHOD              3 (has_perm)
+                      80 LOAD_CONST               2 ('punkweb_bb.close_thread')
+                      82 PRECALL                  1
+                      86 CALL                     1
+                      96 POP_JUMP_FORWARD_IF_TRUE    15 (to 128)
+         
+         427          98 LOAD_GLOBAL              9 (NULL + HttpResponseForbidden)
+                     110 LOAD_CONST               3 ('You do not have permission to close threads.')
+                     112 PRECALL                  1
+                     116 CALL                     1
+                     126 RETURN_VALUE
+         
+         429     >>  128 LOAD_FAST                2 (thread)
+                     130 LOAD_ATTR                5 (is_closed)
+                     140 UNARY_NOT
+                     142 LOAD_FAST                2 (thread)
+                     144 STORE_ATTR               5 (is_closed)
+         
+         430         154 LOAD_FAST                2 (thread)
+                     156 LOAD_METHOD              6 (save)
+                     178 PRECALL                  0
+                     182 CALL                     0
+                     192 POP_TOP
+         
+         432         194 LOAD_GLOBAL             15 (NULL + htmx_redirect)
+                     206 LOAD_FAST                2 (thread)
+                     208 LOAD_METHOD              8 (get_absolute_url)
+                     230 PRECALL                  0
+                     234 CALL                     0
+                     244 PRECALL                  1
+                     248 CALL                     1
+                     258 RETURN_VALUE
+         consts
+            None
+            ('pk',)
+            'punkweb_bb.close_thread'
+            'You do not have permission to close threads.'
+         names      ('get_object_or_404', 'Thread', 'user', 'has_perm', 'HttpResponseForbidden', 'is_closed', 'save', 'htmx_redirect', 'get_absolute_url')
+         varnames   ('request', 'thread_id', 'thread')
+         freevars   ()
+         cellvars   ()
+         filename   '/home/pork/Punkweb/punkweb-bb/punkweb_bb/views.py'
+         name       'thread_close_view'
+         firstlineno 422
+         lnotab 0x02022c0234011e021a012802
+      code
+         argcount  : 2
          nlocals   : 5
          stacksize : 4
          flags     : 3
          code
             0x97007401000000000000000000007402000000000000000000007c01ac
             01a6020000ab0200000000000000007d027c02a002000000000000000000
             00000000000000000000007c006a030000000000000000a6010000ab0100
@@ -2440,97 +2616,97 @@
             00000000000000000000000000a6000000ab000000000000000000724c7c
             03a00800000000000000000000000000000000000000006403ac04a60100
             00ab0100000000000000007d047c027c045f0900000000000000007c006a
             0300000000000000007c045f0300000000000000007c04a0080000000000
             000000000000000000000000000000a6000000ab00000000000000000001
             007415000000000000000000007c04a6010000ab01000000000000000053
             0064005300
-         409           0 RESUME                   0
+         435           0 RESUME                   0
          
-         411           2 LOAD_GLOBAL              1 (NULL + get_object_or_404)
+         437           2 LOAD_GLOBAL              1 (NULL + get_object_or_404)
                       14 LOAD_GLOBAL              2 (Thread)
                       26 LOAD_FAST                1 (thread_id)
                       28 KW_NAMES                 1
                       30 PRECALL                  2
                       34 CALL                     2
                       44 STORE_FAST               2 (thread)
          
-         413          46 LOAD_FAST                2 (thread)
+         439          46 LOAD_FAST                2 (thread)
                       48 LOAD_METHOD              2 (can_post)
                       70 LOAD_FAST                0 (request)
                       72 LOAD_ATTR                3 (user)
                       82 PRECALL                  1
                       86 CALL                     1
                       96 POP_JUMP_FORWARD_IF_TRUE    15 (to 128)
          
-         414          98 LOAD_GLOBAL              9 (NULL + HttpResponseForbidden)
+         440          98 LOAD_GLOBAL              9 (NULL + HttpResponseForbidden)
          
-         415         110 LOAD_CONST               2 ('You do not have permission to post in this thread.')
+         441         110 LOAD_CONST               2 ('You do not have permission to post in this thread.')
          
-         414         112 PRECALL                  1
+         440         112 PRECALL                  1
                      116 CALL                     1
                      126 RETURN_VALUE
          
-         418     >>  128 LOAD_GLOBAL             11 (NULL + PostModelForm)
+         444     >>  128 LOAD_GLOBAL             11 (NULL + PostModelForm)
                      140 LOAD_FAST                0 (request)
                      142 LOAD_ATTR                6 (POST)
                      152 PRECALL                  1
                      156 CALL                     1
                      166 STORE_FAST               3 (form)
          
-         420         168 LOAD_FAST                3 (form)
+         446         168 LOAD_FAST                3 (form)
                      170 LOAD_METHOD              7 (is_valid)
                      192 PRECALL                  0
                      196 CALL                     0
                      206 POP_JUMP_FORWARD_IF_FALSE    76 (to 360)
          
-         421         208 LOAD_FAST                3 (form)
+         447         208 LOAD_FAST                3 (form)
                      210 LOAD_METHOD              8 (save)
                      232 LOAD_CONST               3 (False)
                      234 KW_NAMES                 4
                      236 PRECALL                  1
                      240 CALL                     1
                      250 STORE_FAST               4 (post)
          
-         422         252 LOAD_FAST                2 (thread)
+         448         252 LOAD_FAST                2 (thread)
                      254 LOAD_FAST                4 (post)
                      256 STORE_ATTR               9 (thread)
          
-         423         266 LOAD_FAST                0 (request)
+         449         266 LOAD_FAST                0 (request)
                      268 LOAD_ATTR                3 (user)
                      278 LOAD_FAST                4 (post)
                      280 STORE_ATTR               3 (user)
          
-         424         290 LOAD_FAST                4 (post)
+         450         290 LOAD_FAST                4 (post)
                      292 LOAD_METHOD              8 (save)
                      314 PRECALL                  0
                      318 CALL                     0
                      328 POP_TOP
          
-         426         330 LOAD_GLOBAL             21 (NULL + redirect)
+         452         330 LOAD_GLOBAL             21 (NULL + redirect)
                      342 LOAD_FAST                4 (post)
                      344 PRECALL                  1
                      348 CALL                     1
                      358 RETURN_VALUE
          
-         420     >>  360 LOAD_CONST               0 (None)
+         446     >>  360 LOAD_CONST               0 (None)
                      362 RETURN_VALUE
          consts
             None
             ('pk',)
             'You do not have permission to post in this thread.'
             False
             ('commit',)
          names      ('get_object_or_404', 'Thread', 'can_post', 'user', 'HttpResponseForbidden', 'PostModelForm', 'POST', 'is_valid', 'save', 'thread', 'redirect')
          varnames   ('request', 'thread_id', 'thread', 'form', 'post')
          freevars   ()
          cellvars   ()
          filename   '/home/pork/Punkweb/punkweb-bb/punkweb_bb/views.py'
          name       'post_create_view'
-         firstlineno 409
+         firstlineno 435
          lnotab 0x02022c0234010c0102ff1004280228012c010e01180128021efa
       code
          argcount  : 2
          nlocals   : 5
          stacksize : 5
          flags     : 3
          code
@@ -2543,87 +2719,87 @@
             020000ab0200000000000000007d037c03a0080000000000000000000000
             000000000000000000a6000000ab00000000000000000072237c03a00900
             00000000000000000000000000000000000000a6000000ab000000000000
             0000007d027415000000000000000000007c02a6010000ab010000000000
             0000005300740d000000000000000000007c02ac04a6010000ab01000000
             00000000007d037c027c0364059c027d047417000000000000000000007c
             0064067c04ac07a6030000ab0300000000000000005300
-         429           0 RESUME                   0
+         455           0 RESUME                   0
          
-         431           2 LOAD_GLOBAL              1 (NULL + get_object_or_404)
+         457           2 LOAD_GLOBAL              1 (NULL + get_object_or_404)
                       14 LOAD_GLOBAL              2 (Post)
                       26 LOAD_FAST                1 (post_id)
                       28 KW_NAMES                 1
                       30 PRECALL                  2
                       34 CALL                     2
                       44 STORE_FAST               2 (post)
          
-         433          46 LOAD_FAST                2 (post)
+         459          46 LOAD_FAST                2 (post)
                       48 LOAD_METHOD              2 (can_edit)
                       70 LOAD_FAST                0 (request)
                       72 LOAD_ATTR                3 (user)
                       82 PRECALL                  1
                       86 CALL                     1
                       96 POP_JUMP_FORWARD_IF_TRUE    15 (to 128)
          
-         434          98 LOAD_GLOBAL              9 (NULL + HttpResponseForbidden)
+         460          98 LOAD_GLOBAL              9 (NULL + HttpResponseForbidden)
                      110 LOAD_CONST               2 ('You do not have permission to change this post.')
                      112 PRECALL                  1
                      116 CALL                     1
                      126 RETURN_VALUE
          
-         436     >>  128 LOAD_FAST                0 (request)
+         462     >>  128 LOAD_FAST                0 (request)
                      130 LOAD_ATTR                5 (method)
                      140 LOAD_CONST               3 ('POST')
                      142 COMPARE_OP               2 (==)
                      148 POP_JUMP_FORWARD_IF_FALSE    77 (to 304)
          
-         437         150 LOAD_GLOBAL             13 (NULL + PostModelForm)
+         463         150 LOAD_GLOBAL             13 (NULL + PostModelForm)
                      162 LOAD_FAST                0 (request)
                      164 LOAD_ATTR                7 (POST)
                      174 LOAD_FAST                2 (post)
                      176 KW_NAMES                 4
                      178 PRECALL                  2
                      182 CALL                     2
                      192 STORE_FAST               3 (form)
          
-         439         194 LOAD_FAST                3 (form)
+         465         194 LOAD_FAST                3 (form)
                      196 LOAD_METHOD              8 (is_valid)
                      218 PRECALL                  0
                      222 CALL                     0
                      232 POP_JUMP_FORWARD_IF_FALSE    35 (to 304)
          
-         440         234 LOAD_FAST                3 (form)
+         466         234 LOAD_FAST                3 (form)
                      236 LOAD_METHOD              9 (save)
                      258 PRECALL                  0
                      262 CALL                     0
                      272 STORE_FAST               2 (post)
          
-         442         274 LOAD_GLOBAL             21 (NULL + redirect)
+         468         274 LOAD_GLOBAL             21 (NULL + redirect)
                      286 LOAD_FAST                2 (post)
                      288 PRECALL                  1
                      292 CALL                     1
                      302 RETURN_VALUE
          
-         444     >>  304 LOAD_GLOBAL             13 (NULL + PostModelForm)
+         470     >>  304 LOAD_GLOBAL             13 (NULL + PostModelForm)
                      316 LOAD_FAST                2 (post)
                      318 KW_NAMES                 4
                      320 PRECALL                  1
                      324 CALL                     1
                      334 STORE_FAST               3 (form)
          
-         447         336 LOAD_FAST                2 (post)
+         473         336 LOAD_FAST                2 (post)
          
-         448         338 LOAD_FAST                3 (form)
+         474         338 LOAD_FAST                3 (form)
          
-         446         340 LOAD_CONST               5 (('post', 'form'))
+         472         340 LOAD_CONST               5 (('post', 'form'))
                      342 BUILD_CONST_KEY_MAP      2
                      344 STORE_FAST               4 (context)
          
-         451         346 LOAD_GLOBAL             23 (NULL + render)
+         477         346 LOAD_GLOBAL             23 (NULL + render)
                      358 LOAD_FAST                0 (request)
                      360 LOAD_CONST               6 ('punkweb_bb/partials/post_update.html')
                      362 LOAD_FAST                4 (context)
                      364 KW_NAMES                 7
                      366 PRECALL                  3
                      370 CALL                     3
                      380 RETURN_VALUE
@@ -2638,15 +2814,15 @@
             ('context',)
          names      ('get_object_or_404', 'Post', 'can_edit', 'user', 'HttpResponseForbidden', 'method', 'PostModelForm', 'POST', 'is_valid', 'save', 'redirect', 'render')
          varnames   ('request', 'post_id', 'post', 'form', 'context')
          freevars   ()
          cellvars   ()
          filename   '/home/pork/Punkweb/punkweb-bb/punkweb_bb/views.py'
          name       'post_update_view'
-         firstlineno 429
+         firstlineno 455
          lnotab 0x02022c0234011e0216012c02280128021e022003020102fe0605
       code
          argcount  : 2
          nlocals   : 4
          stacksize : 5
          flags     : 3
          code
@@ -2657,67 +2833,67 @@
             0000000000000053007c006a05000000000000000064036b020000000072
             3a7c02a0060000000000000000000000000000000000000000a6000000ab
             0000000000000000000100740f000000000000000000007c026a08000000
             0000000000a0090000000000000000000000000000000000000000a60000
             00ab000000000000000000a6010000ab010000000000000000530064047c
             0269017d037415000000000000000000007c0064057c03ac06a6030000ab
             0300000000000000005300
-         454           0 RESUME                   0
+         480           0 RESUME                   0
          
-         456           2 LOAD_GLOBAL              1 (NULL + get_object_or_404)
+         482           2 LOAD_GLOBAL              1 (NULL + get_object_or_404)
                       14 LOAD_GLOBAL              2 (Post)
                       26 LOAD_FAST                1 (post_id)
                       28 KW_NAMES                 1
                       30 PRECALL                  2
                       34 CALL                     2
                       44 STORE_FAST               2 (post)
          
-         458          46 LOAD_FAST                2 (post)
+         484          46 LOAD_FAST                2 (post)
                       48 LOAD_METHOD              2 (can_delete)
                       70 LOAD_FAST                0 (request)
                       72 LOAD_ATTR                3 (user)
                       82 PRECALL                  1
                       86 CALL                     1
                       96 POP_JUMP_FORWARD_IF_TRUE    15 (to 128)
          
-         459          98 LOAD_GLOBAL              9 (NULL + HttpResponseForbidden)
+         485          98 LOAD_GLOBAL              9 (NULL + HttpResponseForbidden)
                      110 LOAD_CONST               2 ('You do not have permission to delete this post.')
                      112 PRECALL                  1
                      116 CALL                     1
                      126 RETURN_VALUE
          
-         461     >>  128 LOAD_FAST                0 (request)
+         487     >>  128 LOAD_FAST                0 (request)
                      130 LOAD_ATTR                5 (method)
                      140 LOAD_CONST               3 ('DELETE')
                      142 COMPARE_OP               2 (==)
                      148 POP_JUMP_FORWARD_IF_FALSE    58 (to 266)
          
-         462         150 LOAD_FAST                2 (post)
+         488         150 LOAD_FAST                2 (post)
                      152 LOAD_METHOD              6 (delete)
                      174 PRECALL                  0
                      178 CALL                     0
                      188 POP_TOP
          
-         464         190 LOAD_GLOBAL             15 (NULL + htmx_redirect)
+         490         190 LOAD_GLOBAL             15 (NULL + htmx_redirect)
                      202 LOAD_FAST                2 (post)
                      204 LOAD_ATTR                8 (thread)
                      214 LOAD_METHOD              9 (get_absolute_url)
                      236 PRECALL                  0
                      240 CALL                     0
                      250 PRECALL                  1
                      254 CALL                     1
                      264 RETURN_VALUE
          
-         467     >>  266 LOAD_CONST               4 ('post')
+         493     >>  266 LOAD_CONST               4 ('post')
                      268 LOAD_FAST                2 (post)
          
-         466         270 BUILD_MAP                1
+         492         270 BUILD_MAP                1
                      272 STORE_FAST               3 (context)
          
-         470         274 LOAD_GLOBAL             21 (NULL + render)
+         496         274 LOAD_GLOBAL             21 (NULL + render)
                      286 LOAD_FAST                0 (request)
                      288 LOAD_CONST               5 ('punkweb_bb/partials/post_delete.html')
                      290 LOAD_FAST                3 (context)
                      292 KW_NAMES                 6
                      294 PRECALL                  3
                      298 CALL                     3
                      308 RETURN_VALUE
@@ -2731,94 +2907,94 @@
             ('context',)
          names      ('get_object_or_404', 'Post', 'can_delete', 'user', 'HttpResponseForbidden', 'method', 'delete', 'htmx_redirect', 'thread', 'get_absolute_url', 'render')
          varnames   ('request', 'post_id', 'post', 'context')
          freevars   ()
          cellvars   ()
          filename   '/home/pork/Punkweb/punkweb-bb/punkweb_bb/views.py'
          name       'post_delete_view'
-         firstlineno 454
+         firstlineno 480
          lnotab 0x02022c0234011e02160128024c0304ff0404
       code
          argcount  : 0
          nlocals   : 0
          stacksize : 6
          flags     : 3
          code
             0x97007400000000000000000000006a010000000000000000a002000000
             00000000000000000000000000000000007407000000000000000000006a
             040000000000000000a6000000ab000000000000000000740b0000000000
             00000000006a0600000000000000006401ac02a6010000ab010000000000
             0000007a0a0000ac03a6010000ab010000000000000000a0070000000000
             0000000000000000000000000000006404a6010000ab0100000000000000
             005300
-         473           0 RESUME                   0
+         499           0 RESUME                   0
          
-         474           2 LOAD_GLOBAL              0 (Shout)
+         500           2 LOAD_GLOBAL              0 (Shout)
                       14 LOAD_ATTR                1 (objects)
                       24 LOAD_METHOD              2 (filter)
          
-         475          46 LOAD_GLOBAL              7 (NULL + timezone)
+         501          46 LOAD_GLOBAL              7 (NULL + timezone)
                       58 LOAD_ATTR                4 (now)
                       68 PRECALL                  0
                       72 CALL                     0
                       82 LOAD_GLOBAL             11 (NULL + datetime)
                       94 LOAD_ATTR                6 (timedelta)
                      104 LOAD_CONST               1 (12)
                      106 KW_NAMES                 2
                      108 PRECALL                  1
                      112 CALL                     1
                      122 BINARY_OP               10 (-)
          
-         474         126 KW_NAMES                 3
+         500         126 KW_NAMES                 3
                      128 PRECALL                  1
                      132 CALL                     1
          
-         476         142 LOAD_METHOD              7 (order_by)
+         502         142 LOAD_METHOD              7 (order_by)
                      164 LOAD_CONST               4 ('created_at')
                      166 PRECALL                  1
                      170 CALL                     1
          
-         474         180 RETURN_VALUE
+         500         180 RETURN_VALUE
          consts
             None
             12
             ('hours',)
             ('created_at__gt',)
             'created_at'
          names      ('Shout', 'objects', 'filter', 'timezone', 'now', 'datetime', 'timedelta', 'order_by')
          varnames   ()
          freevars   ()
          cellvars   ()
          filename   '/home/pork/Punkweb/punkweb-bb/punkweb_bb/views.py'
          name       'current_shouts'
-         firstlineno 473
+         firstlineno 499
          lnotab 0x02012c0150ff100226fe
       code
          argcount  : 1
          nlocals   : 3
          stacksize : 5
          flags     : 3
          code
             0x9700740100000000000000000000a6000000ab0000000000000000007d
             0164017c0169017d027403000000000000000000007c0064027c02ac03a6
             030000ab0300000000000000005300
-         479           0 RESUME                   0
+         505           0 RESUME                   0
          
-         480           2 LOAD_GLOBAL              1 (NULL + current_shouts)
+         506           2 LOAD_GLOBAL              1 (NULL + current_shouts)
                       14 PRECALL                  0
                       18 CALL                     0
                       28 STORE_FAST               1 (shouts)
          
-         483          30 LOAD_CONST               1 ('shouts')
+         509          30 LOAD_CONST               1 ('shouts')
                       32 LOAD_FAST                1 (shouts)
          
-         482          34 BUILD_MAP                1
+         508          34 BUILD_MAP                1
                       36 STORE_FAST               2 (context)
          
-         485          38 LOAD_GLOBAL              3 (NULL + render)
+         511          38 LOAD_GLOBAL              3 (NULL + render)
                       50 LOAD_FAST                0 (request)
                       52 LOAD_CONST               2 ('punkweb_bb/shoutbox/shout_list.html')
                       54 LOAD_FAST                2 (context)
                       56 KW_NAMES                 3
                       58 PRECALL                  3
                       62 CALL                     3
                       72 RETURN_VALUE
@@ -2829,15 +3005,15 @@
             ('context',)
          names      ('current_shouts', 'render')
          varnames   ('request', 'shouts', 'context')
          freevars   ()
          cellvars   ()
          filename   '/home/pork/Punkweb/punkweb-bb/punkweb_bb/views.py'
          name       'shout_list_view'
-         firstlineno 479
+         firstlineno 505
          lnotab 0x02011c0304ff0403
       code
          argcount  : 1
          nlocals   : 4
          stacksize : 5
          flags     : 3
          code
@@ -2850,99 +3026,99 @@
             00a6000000ab000000000000000000725a7c02a008000000000000000000
             00000000000000000000006405ac06a6010000ab0100000000000000007d
             037c006a0000000000000000007c035f0000000000000000007c03a00800
             00000000000000000000000000000000000000a6000000ab000000000000
             00000001006401740500000000000000000000a6000000ab000000000000
             00000069017d017407000000000000000000007c0064027c01ac03a60300
             00ab03000000000000000053006400530064005300
-         488           0 RESUME                   0
+         514           0 RESUME                   0
          
-         489           2 LOAD_FAST                0 (request)
+         515           2 LOAD_FAST                0 (request)
                        4 LOAD_ATTR                0 (user)
                       14 LOAD_ATTR                1 (is_authenticated)
                       24 POP_JUMP_FORWARD_IF_TRUE    34 (to 94)
          
-         491          26 LOAD_CONST               1 ('shouts')
+         517          26 LOAD_CONST               1 ('shouts')
                       28 LOAD_GLOBAL              5 (NULL + current_shouts)
                       40 PRECALL                  0
                       44 CALL                     0
          
-         490          54 BUILD_MAP                1
+         516          54 BUILD_MAP                1
                       56 STORE_FAST               1 (context)
          
-         493          58 LOAD_GLOBAL              7 (NULL + render)
+         519          58 LOAD_GLOBAL              7 (NULL + render)
                       70 LOAD_FAST                0 (request)
                       72 LOAD_CONST               2 ('punkweb_bb/shoutbox/shout_list.html')
                       74 LOAD_FAST                1 (context)
                       76 KW_NAMES                 3
                       78 PRECALL                  3
                       82 CALL                     3
                       92 RETURN_VALUE
          
-         495     >>   94 LOAD_FAST                0 (request)
+         521     >>   94 LOAD_FAST                0 (request)
                       96 LOAD_ATTR                4 (method)
                      106 LOAD_CONST               4 ('POST')
                      108 COMPARE_OP               2 (==)
                      114 POP_JUMP_FORWARD_IF_FALSE   128 (to 372)
          
-         496         116 LOAD_GLOBAL             11 (NULL + ShoutModelForm)
+         522         116 LOAD_GLOBAL             11 (NULL + ShoutModelForm)
                      128 LOAD_FAST                0 (request)
                      130 LOAD_ATTR                6 (POST)
                      140 PRECALL                  1
                      144 CALL                     1
                      154 STORE_FAST               2 (form)
          
-         498         156 LOAD_FAST                2 (form)
+         524         156 LOAD_FAST                2 (form)
                      158 LOAD_METHOD              7 (is_valid)
                      180 PRECALL                  0
                      184 CALL                     0
                      194 POP_JUMP_FORWARD_IF_FALSE    90 (to 376)
          
-         499         196 LOAD_FAST                2 (form)
+         525         196 LOAD_FAST                2 (form)
                      198 LOAD_METHOD              8 (save)
                      220 LOAD_CONST               5 (False)
                      222 KW_NAMES                 6
                      224 PRECALL                  1
                      228 CALL                     1
                      238 STORE_FAST               3 (shout)
          
-         500         240 LOAD_FAST                0 (request)
+         526         240 LOAD_FAST                0 (request)
                      242 LOAD_ATTR                0 (user)
                      252 LOAD_FAST                3 (shout)
                      254 STORE_ATTR               0 (user)
          
-         501         264 LOAD_FAST                3 (shout)
+         527         264 LOAD_FAST                3 (shout)
                      266 LOAD_METHOD              8 (save)
                      288 PRECALL                  0
                      292 CALL                     0
                      302 POP_TOP
          
-         504         304 LOAD_CONST               1 ('shouts')
+         530         304 LOAD_CONST               1 ('shouts')
                      306 LOAD_GLOBAL              5 (NULL + current_shouts)
                      318 PRECALL                  0
                      322 CALL                     0
          
-         503         332 BUILD_MAP                1
+         529         332 BUILD_MAP                1
                      334 STORE_FAST               1 (context)
          
-         506         336 LOAD_GLOBAL              7 (NULL + render)
+         532         336 LOAD_GLOBAL              7 (NULL + render)
          
-         507         348 LOAD_FAST                0 (request)
+         533         348 LOAD_FAST                0 (request)
                      350 LOAD_CONST               2 ('punkweb_bb/shoutbox/shout_list.html')
                      352 LOAD_FAST                1 (context)
          
-         506         354 KW_NAMES                 3
+         532         354 KW_NAMES                 3
                      356 PRECALL                  3
                      360 CALL                     3
                      370 RETURN_VALUE
          
-         495     >>  372 LOAD_CONST               0 (None)
+         521     >>  372 LOAD_CONST               0 (None)
                      374 RETURN_VALUE
          
-         498     >>  376 LOAD_CONST               0 (None)
+         524     >>  376 LOAD_CONST               0 (None)
                      378 RETURN_VALUE
          consts
             None
             'shouts'
             'punkweb_bb/shoutbox/shout_list.html'
             ('context',)
             'POST'
@@ -2950,15 +3126,15 @@
             ('commit',)
          names      ('user', 'is_authenticated', 'current_shouts', 'render', 'method', 'ShoutModelForm', 'POST', 'is_valid', 'save')
          varnames   ('request', 'context', 'form', 'shout')
          freevars   ()
          cellvars   ()
          filename   '/home/pork/Punkweb/punkweb-bb/punkweb_bb/views.py'
          name       'shout_create_view'
-         firstlineno 488
+         firstlineno 514
          lnotab
             0x020118021cff040324021601280228012c01180128031cff04030c0106
             ff12f50403
       code
          argcount  : 2
          nlocals   : 4
          stacksize : 5
@@ -2970,66 +3146,66 @@
             00000000000000730f7409000000000000000000006402a6010000ab0100
             0000000000000053007c006a05000000000000000064036b020000000072
             307c02a0060000000000000000000000000000000000000000a6000000ab
             0000000000000000000100740f0000000000000000000074110000000000
             00000000006404a6010000ab010000000000000000a6010000ab01000000
             0000000000530064057c0269017d037413000000000000000000007c0064
             067c03ac07a6030000ab0300000000000000005300
-         511           0 RESUME                   0
+         537           0 RESUME                   0
          
-         513           2 LOAD_GLOBAL              1 (NULL + get_object_or_404)
+         539           2 LOAD_GLOBAL              1 (NULL + get_object_or_404)
                       14 LOAD_GLOBAL              2 (Shout)
                       26 LOAD_FAST                1 (shout_id)
                       28 KW_NAMES                 1
                       30 PRECALL                  2
                       34 CALL                     2
                       44 STORE_FAST               2 (shout)
          
-         515          46 LOAD_FAST                2 (shout)
+         541          46 LOAD_FAST                2 (shout)
                       48 LOAD_METHOD              2 (can_delete)
                       70 LOAD_FAST                0 (request)
                       72 LOAD_ATTR                3 (user)
                       82 PRECALL                  1
                       86 CALL                     1
                       96 POP_JUMP_FORWARD_IF_TRUE    15 (to 128)
          
-         516          98 LOAD_GLOBAL              9 (NULL + HttpResponseForbidden)
+         542          98 LOAD_GLOBAL              9 (NULL + HttpResponseForbidden)
                      110 LOAD_CONST               2 ('You do not have permission to delete this shout.')
                      112 PRECALL                  1
                      116 CALL                     1
                      126 RETURN_VALUE
          
-         518     >>  128 LOAD_FAST                0 (request)
+         544     >>  128 LOAD_FAST                0 (request)
                      130 LOAD_ATTR                5 (method)
                      140 LOAD_CONST               3 ('DELETE')
                      142 COMPARE_OP               2 (==)
                      148 POP_JUMP_FORWARD_IF_FALSE    48 (to 246)
          
-         519         150 LOAD_FAST                2 (shout)
+         545         150 LOAD_FAST                2 (shout)
                      152 LOAD_METHOD              6 (delete)
                      174 PRECALL                  0
                      178 CALL                     0
                      188 POP_TOP
          
-         521         190 LOAD_GLOBAL             15 (NULL + htmx_redirect)
+         547         190 LOAD_GLOBAL             15 (NULL + htmx_redirect)
                      202 LOAD_GLOBAL             17 (NULL + reverse)
                      214 LOAD_CONST               4 ('punkweb_bb:index')
                      216 PRECALL                  1
                      220 CALL                     1
                      230 PRECALL                  1
                      234 CALL                     1
                      244 RETURN_VALUE
          
-         524     >>  246 LOAD_CONST               5 ('shout')
+         550     >>  246 LOAD_CONST               5 ('shout')
                      248 LOAD_FAST                2 (shout)
          
-         523         250 BUILD_MAP                1
+         549         250 BUILD_MAP                1
                      252 STORE_FAST               3 (context)
          
-         527         254 LOAD_GLOBAL             19 (NULL + render)
+         553         254 LOAD_GLOBAL             19 (NULL + render)
                      266 LOAD_FAST                0 (request)
                      268 LOAD_CONST               6 ('punkweb_bb/partials/shout_delete.html')
                      270 LOAD_FAST                3 (context)
                      272 KW_NAMES                 7
                      274 PRECALL                  3
                      278 CALL                     3
                      288 RETURN_VALUE
@@ -3044,36 +3220,36 @@
             ('context',)
          names      ('get_object_or_404', 'Shout', 'can_delete', 'user', 'HttpResponseForbidden', 'method', 'delete', 'htmx_redirect', 'reverse', 'render')
          varnames   ('request', 'shout_id', 'shout', 'context')
          freevars   ()
          cellvars   ()
          filename   '/home/pork/Punkweb/punkweb-bb/punkweb_bb/views.py'
          name       'shout_delete_view'
-         firstlineno 511
+         firstlineno 537
          lnotab 0x02022c0234011e0216012802380304ff0404
       code
          argcount  : 1
          nlocals   : 3
          stacksize : 5
          flags     : 3
          code
             0x970064017d0164027c0169017d027401000000000000000000007c0064
             037c02ac04a6030000ab0300000000000000005300
-         530           0 RESUME                   0
+         556           0 RESUME                   0
          
-         531           2 LOAD_CONST               1 ((('Bold', '[b]Bold Text[/b]'), ('Italic', '[i]Italic Text[/i]'), ('Underline', '[u]Underlined Text[/u]'), ('Strikethrough', '[s]Strikethrough Text[/s]'), ('Quote', '[quote=Example]Quoted Text[/quote]'), ('Center', '[center]Centered Text[/center]'), ('Color', '[color=red]Red Text[/color]'), ('Url', '[url=https://google.com]Link Text[/url]'), ('Image', '[img]https://placehold.co/400[/img]'), ('Horizontal Rule', '[hr]'), ('Code', '\n[code=python]\nclass ThreadModelForm(forms.ModelForm):\n    class Meta:\n        model = Thread\n        fields = (\n            "title",\n            "content",\n        )\n        widgets = {\n            "title": forms.TextInput(attrs={"autofocus": True, "class": "pw-input"}),\n            "content": BBCodeEditorWidget(),\n        }\n[/code]\n'), ('Email', '[email=test@example.com]Example[/email]'), ('Font', '[font=serif]Serif Text[/font]'), ('Ordered List', '[ol][li]Item 1[/li][li]Item 2[/li][/ol]'), ('Unordered List', '[ul][li]Item 1[/li][li]Item 2[/li][/ul]'), ('Shadow', '[shadow=red]Red Shadow Text[/shadow]'), ('Size', '[size=7]Size 7 Text[/size]'), ('Checkbox', '\n[n]Unchecked\n[y]Checked\n            '), ('Superscript', 'Sup [sup]Superscript Text[/sup]'), ('Subscript', 'Sub [sub]Subscript Text[/sub]'), ('Left', '[left]Left Text[/left]'), ('Right', '[right]Right Text[/right]'), ('Escape', '[escape][b]Escaped bbcode[/b][/escape]')))
+         557           2 LOAD_CONST               1 ((('Bold', '[b]Bold Text[/b]'), ('Italic', '[i]Italic Text[/i]'), ('Underline', '[u]Underlined Text[/u]'), ('Strikethrough', '[s]Strikethrough Text[/s]'), ('Quote', '[quote=Example]Quoted Text[/quote]'), ('Center', '[center]Centered Text[/center]'), ('Color', '[color=red]Red Text[/color]'), ('Url', '[url=https://google.com]Link Text[/url]'), ('Image', '[img]https://placehold.co/400[/img]'), ('Horizontal Rule', '[hr]'), ('Code', '\n[code=python]\nclass ThreadModelForm(forms.ModelForm):\n    class Meta:\n        model = Thread\n        fields = (\n            "title",\n            "content",\n        )\n        widgets = {\n            "title": forms.TextInput(attrs={"autofocus": True, "class": "pw-input"}),\n            "content": BBCodeEditorWidget(),\n        }\n[/code]\n'), ('Email', '[email=test@example.com]Example[/email]'), ('Font', '[font=serif]Serif Text[/font]'), ('Ordered List', '[ol][li]Item 1[/li][li]Item 2[/li][/ol]'), ('Unordered List', '[ul][li]Item 1[/li][li]Item 2[/li][/ul]'), ('Shadow', '[shadow=red]Red Shadow Text[/shadow]'), ('Size', '[size=7]Size 7 Text[/size]'), ('Checkbox', '\n[n]Unchecked\n[y]Checked\n            '), ('Superscript', 'Sup [sup]Superscript Text[/sup]'), ('Subscript', 'Sub [sub]Subscript Text[/sub]'), ('Left', '[left]Left Text[/left]'), ('Right', '[right]Right Text[/right]'), ('Escape', '[escape][b]Escaped bbcode[/b][/escape]')))
                        4 STORE_FAST               1 (codes)
          
-         585           6 LOAD_CONST               2 ('codes')
+         611           6 LOAD_CONST               2 ('codes')
                        8 LOAD_FAST                1 (codes)
          
-         584          10 BUILD_MAP                1
+         610          10 BUILD_MAP                1
                       12 STORE_FAST               2 (context)
          
-         588          14 LOAD_GLOBAL              1 (NULL + render)
+         614          14 LOAD_GLOBAL              1 (NULL + render)
                       26 LOAD_FAST                0 (request)
                       28 LOAD_CONST               3 ('punkweb_bb/bbcode.html')
                       30 LOAD_FAST                2 (context)
                       32 KW_NAMES                 4
                       34 PRECALL                  3
                       38 CALL                     3
                       48 RETURN_VALUE
@@ -3085,23 +3261,24 @@
             ('context',)
          names      ('render',)
          varnames   ('request', 'codes', 'context')
          freevars   ()
          cellvars   ()
          filename   '/home/pork/Punkweb/punkweb-bb/punkweb_bb/views.py'
          name       'bbcode_view'
-         firstlineno 530
+         firstlineno 556
          lnotab 0x0201043604ff0404
-   names      ('datetime', 'django.contrib.auth', 'authenticate', 'get_user_model', 'login', 'logout', 'django.contrib.auth.decorators', 'login_required', 'django.http', 'HttpResponseForbidden', 'django.shortcuts', 'get_object_or_404', 'redirect', 'render', 'django.urls', 'reverse', 'django.utils', 'timezone', 'punkweb_bb.forms', 'BoardProfileModelForm', 'CategoryModelForm', 'LoginForm', 'PostModelForm', 'ShoutModelForm', 'SignUpForm', 'SubcategoryModelForm', 'ThreadModelForm', 'punkweb_bb.guests', 'guest_list', 'punkweb_bb.models', 'Category', 'Post', 'Shout', 'Subcategory', 'Thread', 'punkweb_bb.pagination', 'paginate_qs', 'punkweb_bb.response', 'htmx_redirect', 'punkweb_bb.utils', 'get_unique_slug', 'User', 'signup_view', 'login_view', 'logout_view', 'index_view', 'profile_view', 'members_view', 'settings_view', 'category_create_view', 'category_update_view', 'category_delete_view', 'subcategory_view', 'subcategory_create_view', 'subcategory_update_view', 'subcategory_delete_view', 'thread_create_view', 'thread_view', 'thread_update_view', 'thread_delete_view', 'post_create_view', 'post_update_view', 'post_delete_view', 'current_shouts', 'shout_list_view', 'shout_create_view', 'shout_delete_view', 'bbcode_view')
+   names      ('datetime', 'django.contrib.auth', 'authenticate', 'get_user_model', 'login', 'logout', 'django.contrib.auth.decorators', 'login_required', 'django.http', 'HttpResponseForbidden', 'django.shortcuts', 'get_object_or_404', 'redirect', 'render', 'django.urls', 'reverse', 'django.utils', 'timezone', 'punkweb_bb.forms', 'BoardProfileModelForm', 'CategoryModelForm', 'LoginForm', 'PostModelForm', 'ShoutModelForm', 'SignUpForm', 'SubcategoryModelForm', 'ThreadModelForm', 'punkweb_bb.guests', 'guest_list', 'punkweb_bb.models', 'Category', 'Post', 'Shout', 'Subcategory', 'Thread', 'punkweb_bb.pagination', 'paginate_qs', 'punkweb_bb.response', 'htmx_redirect', 'punkweb_bb.utils', 'get_unique_slug', 'User', 'signup_view', 'login_view', 'logout_view', 'index_view', 'profile_view', 'members_view', 'settings_view', 'category_create_view', 'category_update_view', 'category_delete_view', 'subcategory_view', 'subcategory_create_view', 'subcategory_update_view', 'subcategory_delete_view', 'thread_create_view', 'thread_view', 'thread_update_view', 'thread_delete_view', 'thread_pin_view', 'thread_close_view', 'post_create_view', 'post_update_view', 'post_delete_view', 'current_shouts', 'shout_list_view', 'shout_create_view', 'shout_delete_view', 'bbcode_view')
    varnames   ()
    freevars   ()
    cellvars   ()
    filename   '/home/pork/Punkweb/punkweb-bb/punkweb_bb/views.py'
    name       '<module>'
    firstlineno 1
    lnotab
       0x00ff0201080218010c010c0114010c010c02280a0c011c010c010c010c
       0214030614061a060506200609060b160104ff0e010216160104ff0e0102
       16160104ff0e010217160104ff0e010212060c160104ff0e01021c160104
       ff0e010219160104ff0e010216160104ff0e01021c0616160104ff0e0102
-      19160104ff0e010214160104ff0e010213160104ff0e010218160104ff0e
-      010212060606090617160104ff0e010212
+      19160104ff0e010214160104ff0e01020c160104ff0e01020c160104ff0e
+      010213160104ff0e010218160104ff0e010212060606090617160104ff0e
+      010212
```

### Comparing `punkweb_bb-0.2.0/punkweb_bb/__pycache__/widgets.cpython-311.pyc` & `punkweb_bb-0.2.1/punkweb_bb/__pycache__/widgets.cpython-311.pyc`

 * *Files identical despite different names*

### Comparing `punkweb_bb-0.2.0/punkweb_bb/admin.py` & `punkweb_bb-0.2.1/punkweb_bb/admin.py`

 * *Files identical despite different names*

### Comparing `punkweb_bb-0.2.0/punkweb_bb/admin_forms.py` & `punkweb_bb-0.2.1/punkweb_bb/admin_forms.py`

 * *Files identical despite different names*

### Comparing `punkweb_bb-0.2.0/punkweb_bb/bbcode_tags.py` & `punkweb_bb-0.2.1/punkweb_bb/bbcode_tags.py`

 * *Files identical despite different names*

### Comparing `punkweb_bb-0.2.0/punkweb_bb/forms.py` & `punkweb_bb-0.2.1/punkweb_bb/forms.py`

 * *Files identical despite different names*

### Comparing `punkweb_bb-0.2.0/punkweb_bb/middleware.py` & `punkweb_bb-0.2.1/punkweb_bb/middleware.py`

 * *Files identical despite different names*

### Comparing `punkweb_bb-0.2.0/punkweb_bb/migrations/0001_initial.py` & `punkweb_bb-0.2.1/punkweb_bb/migrations/0001_initial.py`

 * *Files identical despite different names*

### Comparing `punkweb_bb-0.2.0/punkweb_bb/migrations/__pycache__/0001_initial.cpython-311.pyc` & `punkweb_bb-0.2.1/punkweb_bb/migrations/__pycache__/0001_initial.cpython-311.pyc`

 * *Files identical despite different names*

### Comparing `punkweb_bb-0.2.0/punkweb_bb/migrations/__pycache__/0002_thread_view_count.cpython-311.pyc` & `punkweb_bb-0.2.1/punkweb_bb/migrations/__pycache__/0002_thread_view_count.cpython-311.pyc`

 * *Files identical despite different names*

### Comparing `punkweb_bb-0.2.0/punkweb_bb/models.py` & `punkweb_bb-0.2.1/punkweb_bb/models.py`

 * *Files 9% similar despite different names*

```diff
@@ -115,14 +115,18 @@
 
     class Meta:
         ordering = (
             "subcategory",
             "-is_pinned",
             "-last_post_created_at",
         )
+        permissions = (
+            ("pin_thread", "Can pin thread"),
+            ("close_thread", "Can close thread"),
+        )
 
     def __str__(self):
         return f"{self.title}"
 
     def can_edit(self, user):
         return user == self.user or user.has_perm("punkweb_bb.change_thread")
```

### Comparing `punkweb_bb-0.2.0/punkweb_bb/parsers.py` & `punkweb_bb-0.2.1/punkweb_bb/parsers.py`

 * *Files identical despite different names*

### Comparing `punkweb_bb-0.2.0/punkweb_bb/settings.py` & `punkweb_bb-0.2.1/punkweb_bb/settings.py`

 * *Files 13% similar despite different names*

```diff
@@ -1,11 +1,12 @@
 from django.conf import settings
 
 PUNKWEB_BB = getattr(settings, "PUNKWEB_BB", {})
 
 SITE_NAME = PUNKWEB_BB.get("SITE_NAME", "PUNKWEB")
 SITE_TITLE = PUNKWEB_BB.get("SITE_TITLE", "PunkwebBB")
 FAVICON = PUNKWEB_BB.get("FAVICON", "punkweb_bb/favicon.ico")
+OG_IMAGE = PUNKWEB_BB.get("OG_IMAGE", None)
 SHOUTBOX_ENABLED = PUNKWEB_BB.get("SHOUTBOX_ENABLED", True)
 DISCORD_WIDGET_ENABLED = PUNKWEB_BB.get("DISCORD_WIDGET_ENABLED", False)
 DISCORD_WIDGET_THEME = PUNKWEB_BB.get("DISCORD_WIDGET_THEME", "dark")
 DISCORD_SERVER_ID = PUNKWEB_BB.get("DISCORD_SERVER_ID", None)
```

### Comparing `punkweb_bb-0.2.0/punkweb_bb/static/punkweb_bb/css/defaults.css` & `punkweb_bb-0.2.1/punkweb_bb/static/punkweb_bb/css/defaults.css`

 * *Files identical despite different names*

### Comparing `punkweb_bb-0.2.0/punkweb_bb/static/punkweb_bb/css/index.css` & `punkweb_bb-0.2.1/punkweb_bb/static/punkweb_bb/css/index.css`

 * *Files 6% similar despite different names*

```diff
@@ -3,18 +3,18 @@
   gap: 1rem;
 }
 
 .index__categories {
   flex: 1;
 }
 
-.index__category__actions {
+.index__category__title {
   align-items: center;
   display: flex;
-  gap: 0.25rem;
+  gap: 0.5rem;
 }
 
 .index__sidebar {
   flex: 0 0 20rem;
 }
 
 .index__recentThreads__content {
```

### Comparing `punkweb_bb-0.2.0/punkweb_bb/static/punkweb_bb/css/profile.css` & `punkweb_bb-0.2.1/punkweb_bb/static/punkweb_bb/css/profile.css`

 * *Files identical despite different names*

### Comparing `punkweb_bb-0.2.0/punkweb_bb/static/punkweb_bb/css/punkweb-modal.css` & `punkweb_bb-0.2.1/punkweb_bb/static/punkweb_bb/css/punkweb-modal.css`

 * *Files identical despite different names*

### Comparing `punkweb_bb-0.2.0/punkweb_bb/static/punkweb_bb/css/punkweb.css` & `punkweb_bb-0.2.1/punkweb_bb/static/punkweb_bb/css/punkweb.css`

 * *Files 14% similar despite different names*

```diff
@@ -386,20 +386,21 @@
 .pw-button.raised:not(:disabled):active {
   box-shadow: 0 0.25rem 0.5rem 0 rgba(0, 0, 0, 0.25);
 }
 
 /** Icon Button **/
 
 .pw-icon-button {
+  align-items: center;
   border-radius: 0.25rem;
   cursor: pointer;
-  display: inline-block;
+  display: flex;
+  justify-content: center;
   font-weight: 500;
   transition: all 0.15s ease;
-  text-align: center;
 
   height: 2rem;
   line-height: 2rem;
   max-height: 2rem;
   max-width: 2rem;
   min-height: 2rem;
   min-width: 2rem;
@@ -459,15 +460,15 @@
   max-height: 3rem;
   max-width: 3rem;
   min-height: 3rem;
   min-width: 3rem;
   width: 3rem;
 }
 
-.pw-icon-button.sl .material-symbols-outlined {
+.pw-icon-button.xl .material-symbols-outlined {
   font-size: 1.5rem;
 }
 
 .pw-icon-button:disabled {
   background-color: var(--oc-gray-5) !important;
   border-color: var(--oc-gray-5) !important;
   color: var(--oc-gray-5) !important;
@@ -488,14 +489,38 @@
   background-color: var(--oc-gray-0);
 }
 
 .pw-icon-button.default:not(:disabled):active {
   background-color: var(--oc-gray-1);
 }
 
+.pw-icon-button.default.primary {
+  color: var(--primary-9);
+}
+
+.pw-icon-button.default.primary:hover {
+  background-color: var(--primary-0);
+}
+
+.pw-icon-button.default.primary:active {
+  background-color: var(--primary-1);
+}
+
+.pw-icon-button.default.danger {
+  color: var(--oc-red-9);
+}
+
+.pw-icon-button.default.danger:hover {
+  background-color: var(--oc-red-0);
+}
+
+.pw-icon-button.default.danger:active {
+  background-color: var(--oc-red-1);
+}
+
 /* Outlined */
 
 .pw-icon-button.outlined {
   border: 1px solid var(--oc-gray-9);
   color: var(--oc-gray-9);
 }
 
@@ -503,15 +528,41 @@
   background-color: var(--oc-gray-0);
 }
 
 .pw-icon-button.outlined:not(:disabled):active {
   background-color: var(--oc-gray-1);
 }
 
-/* Outlined */
+.pw-icon-button.outlined.primary {
+  border-color: var(--primary-9);
+  color: var(--primary-9);
+}
+
+.pw-icon-button.outlined.primary:hover {
+  background-color: var(--primary-0);
+}
+
+.pw-icon-button.outlined.primary:active {
+  background-color: var(--primary-1);
+}
+
+.pw-icon-button.outlined.danger {
+  border-color: var(--oc-red-9);
+  color: var(--oc-red-9);
+}
+
+.pw-icon-button.outlined.danger:hover {
+  background-color: var(--oc-red-0);
+}
+
+.pw-icon-button.outlined.danger:active {
+  background-color: var(--oc-red-1);
+}
+
+/* Ghost */
 
 .pw-icon-button.ghost {
   border: 1px solid var(--oc-gray-9);
   color: var(--oc-gray-9);
 }
 
 .pw-icon-button.ghost:not(:disabled):hover {
@@ -521,22 +572,62 @@
 
 .pw-icon-button.ghost:not(:disabled):active {
   background-color: var(--oc-gray-9);
   box-shadow: 0 0.125rem 0.25rem 0 rgba(0, 0, 0, 0.25);
   color: white;
 }
 
+.pw-icon-button.ghost.primary {
+  border: 1px solid var(--primary-9);
+  color: var(--primary-9);
+}
+
+.pw-icon-button.ghost.primary:not(:disabled):hover {
+  background-color: var(--primary-9);
+  color: white;
+}
+
+.pw-icon-button.ghost.primary:not(:disabled):active {
+  background-color: var(--primary-9);
+  box-shadow: 0 0.125rem 0.25rem 0 rgba(0, 0, 0, 0.25);
+  color: white;
+}
+
+.pw-icon-button.ghost.danger {
+  border: 1px solid var(--oc-red-9);
+  color: var(--oc-red-9);
+}
+
+.pw-icon-button.ghost.danger:not(:disabled):hover {
+  background-color: var(--oc-red-9);
+  color: white;
+}
+
+.pw-icon-button.ghost.danger:not(:disabled):active {
+  background-color: var(--oc-red-9);
+  box-shadow: 0 0.125rem 0.25rem 0 rgba(0, 0, 0, 0.25);
+  color: white;
+}
+
 /* Raised */
 
 .pw-icon-button.raised {
   background-color: var(--oc-gray-9);
   box-shadow: 0 0.0625rem 0.125rem 0 rgba(0, 0, 0, 0.25);
   color: white;
 }
 
+.pw-icon-button.raised.primary {
+  background-color: var(--primary-9);
+}
+
+.pw-icon-button.raised.danger {
+  background-color: var(--oc-red-9);
+}
+
 .pw-icon-button.raised:not(:disabled):hover {
   box-shadow: 0 0.125rem 0.25rem 0 rgba(0, 0, 0, 0.25);
 }
 
 .pw-icon-button.raised:not(:disabled):active {
   box-shadow: 0 0.25rem 0.5rem 0 rgba(0, 0, 0, 0.25);
 }
```

### Comparing `punkweb_bb-0.2.0/punkweb_bb/static/punkweb_bb/css/shoutbox.css` & `punkweb_bb-0.2.1/punkweb_bb/static/punkweb_bb/css/shoutbox.css`

 * *Files identical despite different names*

### Comparing `punkweb_bb-0.2.0/punkweb_bb/static/punkweb_bb/css/subcategory.css` & `punkweb_bb-0.2.1/punkweb_bb/static/punkweb_bb/css/subcategory.css`

 * *Files identical despite different names*

### Comparing `punkweb_bb-0.2.0/punkweb_bb/static/punkweb_bb/css/thread.css` & `punkweb_bb-0.2.1/punkweb_bb/static/punkweb_bb/css/thread.css`

 * *Files 0% similar despite different names*

```diff
@@ -90,15 +90,15 @@
   padding: 1rem;
 }
 
 .thread__actions {
   align-items: center;
   display: flex;
   justify-content: flex-end;
-  gap: 1rem;
+  gap: 0.25rem;
   padding: 1rem;
 }
 
 .thread__reply__content {
   display: flex;
   flex-direction: column;
   gap: 1rem;
```

### Comparing `punkweb_bb-0.2.0/punkweb_bb/static/punkweb_bb/css/variables.css` & `punkweb_bb-0.2.1/punkweb_bb/static/punkweb_bb/css/variables.css`

 * *Files identical despite different names*

### Comparing `punkweb_bb-0.2.0/punkweb_bb/static/punkweb_bb/editor/bbcode-editor-content.css` & `punkweb_bb-0.2.1/punkweb_bb/static/punkweb_bb/editor/bbcode-editor-content.css`

 * *Files identical despite different names*

### Comparing `punkweb_bb-0.2.0/punkweb_bb/static/punkweb_bb/editor/bbcode-editor-tags.js` & `punkweb_bb-0.2.1/punkweb_bb/static/punkweb_bb/editor/bbcode-editor-tags.js`

 * *Files identical despite different names*

### Comparing `punkweb_bb-0.2.0/punkweb_bb/static/punkweb_bb/editor/bbcode-editor.js` & `punkweb_bb-0.2.1/punkweb_bb/static/punkweb_bb/editor/bbcode-editor.js`

 * *Files 3% similar despite different names*

#### js-beautify {}

```diff
@@ -1,12 +1,12 @@
 $(function() {
     $(document).ready(function() {
         $(".bbcode-editor").sceditor({
             emoticonsCompat: true,
-            emoticonsEnabled: true,
+            emoticonsEnabled: false,
             emoticonsRoot: "/media/precise_bbcode/smilies/",
             emoticons: {
                 dropdown: {},
             },
             format: "bbcode",
             icons: "material",
             style: "/static/punkweb_bb/editor/bbcode-editor-content.css",
```

### Comparing `punkweb_bb-0.2.0/punkweb_bb/static/punkweb_bb/img/default-profile-image.png` & `punkweb_bb-0.2.1/punkweb_bb/static/punkweb_bb/img/default-profile-image.png`

 * *Files identical despite different names*

### Comparing `punkweb_bb-0.2.0/punkweb_bb/static/punkweb_bb/vendor/htmx-1.9.4.min.js` & `punkweb_bb-0.2.1/punkweb_bb/static/punkweb_bb/vendor/htmx-1.9.4.min.js`

 * *Files identical despite different names*

### Comparing `punkweb_bb-0.2.0/punkweb_bb/static/punkweb_bb/vendor/jquery-3.7.0.min.js` & `punkweb_bb-0.2.1/punkweb_bb/static/punkweb_bb/vendor/jquery-3.7.0.min.js`

 * *Files identical despite different names*

### Comparing `punkweb_bb-0.2.0/punkweb_bb/static/punkweb_bb/vendor/open-color.css` & `punkweb_bb-0.2.1/punkweb_bb/static/punkweb_bb/vendor/open-color.css`

 * *Files identical despite different names*

### Comparing `punkweb_bb-0.2.0/punkweb_bb/static/punkweb_bb/vendor/prism.css` & `punkweb_bb-0.2.1/punkweb_bb/static/punkweb_bb/vendor/prism.css`

 * *Files identical despite different names*

### Comparing `punkweb_bb-0.2.0/punkweb_bb/static/punkweb_bb/vendor/prism.js` & `punkweb_bb-0.2.1/punkweb_bb/static/punkweb_bb/vendor/prism.js`

 * *Files identical despite different names*

### Comparing `punkweb_bb-0.2.0/punkweb_bb/static/punkweb_bb/vendor/sceditor-3.2.0/README.md` & `punkweb_bb-0.2.1/punkweb_bb/static/punkweb_bb/vendor/sceditor-3.2.0/README.md`

 * *Files identical despite different names*

### Comparing `punkweb_bb-0.2.0/punkweb_bb/static/punkweb_bb/vendor/sceditor-3.2.0/development/formats/bbcode.js` & `punkweb_bb-0.2.1/punkweb_bb/static/punkweb_bb/vendor/sceditor-3.2.0/development/formats/bbcode.js`

 * *Files identical despite different names*

### Comparing `punkweb_bb-0.2.0/punkweb_bb/static/punkweb_bb/vendor/sceditor-3.2.0/development/formats/xhtml.js` & `punkweb_bb-0.2.1/punkweb_bb/static/punkweb_bb/vendor/sceditor-3.2.0/development/formats/xhtml.js`

 * *Files identical despite different names*

### Comparing `punkweb_bb-0.2.0/punkweb_bb/static/punkweb_bb/vendor/sceditor-3.2.0/development/icons/material.js` & `punkweb_bb-0.2.1/punkweb_bb/static/punkweb_bb/vendor/sceditor-3.2.0/development/icons/material.js`

 * *Files identical despite different names*

### Comparing `punkweb_bb-0.2.0/punkweb_bb/static/punkweb_bb/vendor/sceditor-3.2.0/development/icons/monocons.js` & `punkweb_bb-0.2.1/punkweb_bb/static/punkweb_bb/vendor/sceditor-3.2.0/development/icons/monocons.js`

 * *Files identical despite different names*

### Comparing `punkweb_bb-0.2.0/punkweb_bb/static/punkweb_bb/vendor/sceditor-3.2.0/development/jquery.sceditor.bbcode.js` & `punkweb_bb-0.2.1/punkweb_bb/static/punkweb_bb/vendor/sceditor-3.2.0/development/jquery.sceditor.bbcode.js`

 * *Files identical despite different names*

### Comparing `punkweb_bb-0.2.0/punkweb_bb/static/punkweb_bb/vendor/sceditor-3.2.0/development/jquery.sceditor.js` & `punkweb_bb-0.2.1/punkweb_bb/static/punkweb_bb/vendor/sceditor-3.2.0/development/jquery.sceditor.js`

 * *Files identical despite different names*

### Comparing `punkweb_bb-0.2.0/punkweb_bb/static/punkweb_bb/vendor/sceditor-3.2.0/development/jquery.sceditor.xhtml.js` & `punkweb_bb-0.2.1/punkweb_bb/static/punkweb_bb/vendor/sceditor-3.2.0/development/jquery.sceditor.xhtml.js`

 * *Files identical despite different names*

### Comparing `punkweb_bb-0.2.0/punkweb_bb/static/punkweb_bb/vendor/sceditor-3.2.0/development/plugins/alternative-lists.js` & `punkweb_bb-0.2.1/punkweb_bb/static/punkweb_bb/vendor/sceditor-3.2.0/development/plugins/alternative-lists.js`

 * *Files identical despite different names*

### Comparing `punkweb_bb-0.2.0/punkweb_bb/static/punkweb_bb/vendor/sceditor-3.2.0/development/plugins/autosave.js` & `punkweb_bb-0.2.1/punkweb_bb/static/punkweb_bb/vendor/sceditor-3.2.0/development/plugins/autosave.js`

 * *Files identical despite different names*

### Comparing `punkweb_bb-0.2.0/punkweb_bb/static/punkweb_bb/vendor/sceditor-3.2.0/development/plugins/autoyoutube.js` & `punkweb_bb-0.2.1/punkweb_bb/static/punkweb_bb/vendor/sceditor-3.2.0/development/plugins/autoyoutube.js`

 * *Files identical despite different names*

### Comparing `punkweb_bb-0.2.0/punkweb_bb/static/punkweb_bb/vendor/sceditor-3.2.0/development/plugins/dragdrop.js` & `punkweb_bb-0.2.1/punkweb_bb/static/punkweb_bb/vendor/sceditor-3.2.0/development/plugins/dragdrop.js`

 * *Files identical despite different names*

### Comparing `punkweb_bb-0.2.0/punkweb_bb/static/punkweb_bb/vendor/sceditor-3.2.0/development/plugins/format.js` & `punkweb_bb-0.2.1/punkweb_bb/static/punkweb_bb/vendor/sceditor-3.2.0/development/plugins/format.js`

 * *Files identical despite different names*

### Comparing `punkweb_bb-0.2.0/punkweb_bb/static/punkweb_bb/vendor/sceditor-3.2.0/development/plugins/plaintext.js` & `punkweb_bb-0.2.1/punkweb_bb/static/punkweb_bb/vendor/sceditor-3.2.0/development/plugins/plaintext.js`

 * *Files identical despite different names*

### Comparing `punkweb_bb-0.2.0/punkweb_bb/static/punkweb_bb/vendor/sceditor-3.2.0/development/plugins/undo.js` & `punkweb_bb-0.2.1/punkweb_bb/static/punkweb_bb/vendor/sceditor-3.2.0/development/plugins/undo.js`

 * *Files identical despite different names*

### Comparing `punkweb_bb-0.2.0/punkweb_bb/static/punkweb_bb/vendor/sceditor-3.2.0/development/plugins/v1compat.js` & `punkweb_bb-0.2.1/punkweb_bb/static/punkweb_bb/vendor/sceditor-3.2.0/development/plugins/v1compat.js`

 * *Files identical despite different names*

### Comparing `punkweb_bb-0.2.0/punkweb_bb/static/punkweb_bb/vendor/sceditor-3.2.0/development/sceditor.js` & `punkweb_bb-0.2.1/punkweb_bb/static/punkweb_bb/vendor/sceditor-3.2.0/development/sceditor.js`

 * *Files identical despite different names*

### Comparing `punkweb_bb-0.2.0/punkweb_bb/static/punkweb_bb/vendor/sceditor-3.2.0/development/themes/content/default.css` & `punkweb_bb-0.2.1/punkweb_bb/static/punkweb_bb/vendor/sceditor-3.2.0/development/themes/content/default.css`

 * *Files identical despite different names*

### Comparing `punkweb_bb-0.2.0/punkweb_bb/static/punkweb_bb/vendor/sceditor-3.2.0/development/themes/default.css` & `punkweb_bb-0.2.1/punkweb_bb/static/punkweb_bb/vendor/sceditor-3.2.0/development/themes/default.css`

 * *Files identical despite different names*

### Comparing `punkweb_bb-0.2.0/punkweb_bb/static/punkweb_bb/vendor/sceditor-3.2.0/development/themes/defaultdark.css` & `punkweb_bb-0.2.1/punkweb_bb/static/punkweb_bb/vendor/sceditor-3.2.0/development/themes/defaultdark.css`

 * *Files identical despite different names*

### Comparing `punkweb_bb-0.2.0/punkweb_bb/static/punkweb_bb/vendor/sceditor-3.2.0/development/themes/famfamfam.png` & `punkweb_bb-0.2.1/punkweb_bb/static/punkweb_bb/vendor/sceditor-3.2.0/development/themes/famfamfam.png`

 * *Files identical despite different names*

### Comparing `punkweb_bb-0.2.0/punkweb_bb/static/punkweb_bb/vendor/sceditor-3.2.0/development/themes/modern.css` & `punkweb_bb-0.2.1/punkweb_bb/static/punkweb_bb/vendor/sceditor-3.2.0/development/themes/modern.css`

 * *Files identical despite different names*

### Comparing `punkweb_bb-0.2.0/punkweb_bb/static/punkweb_bb/vendor/sceditor-3.2.0/development/themes/office-toolbar.css` & `punkweb_bb-0.2.1/punkweb_bb/static/punkweb_bb/vendor/sceditor-3.2.0/development/themes/office-toolbar.css`

 * *Files identical despite different names*

### Comparing `punkweb_bb-0.2.0/punkweb_bb/static/punkweb_bb/vendor/sceditor-3.2.0/development/themes/office.css` & `punkweb_bb-0.2.1/punkweb_bb/static/punkweb_bb/vendor/sceditor-3.2.0/development/themes/office.css`

 * *Files identical despite different names*

### Comparing `punkweb_bb-0.2.0/punkweb_bb/static/punkweb_bb/vendor/sceditor-3.2.0/development/themes/square.css` & `punkweb_bb-0.2.1/punkweb_bb/static/punkweb_bb/vendor/sceditor-3.2.0/development/themes/square.css`

 * *Files identical despite different names*

### Comparing `punkweb_bb-0.2.0/punkweb_bb/static/punkweb_bb/vendor/sceditor-3.2.0/emoticons/alien.png` & `punkweb_bb-0.2.1/punkweb_bb/static/punkweb_bb/vendor/sceditor-3.2.0/emoticons/alien.png`

 * *Files identical despite different names*

### Comparing `punkweb_bb-0.2.0/punkweb_bb/static/punkweb_bb/vendor/sceditor-3.2.0/emoticons/angel.png` & `punkweb_bb-0.2.1/punkweb_bb/static/punkweb_bb/vendor/sceditor-3.2.0/emoticons/angel.png`

 * *Files identical despite different names*

### Comparing `punkweb_bb-0.2.0/punkweb_bb/static/punkweb_bb/vendor/sceditor-3.2.0/emoticons/angry.png` & `punkweb_bb-0.2.1/punkweb_bb/static/punkweb_bb/vendor/sceditor-3.2.0/emoticons/angry.png`

 * *Files identical despite different names*

### Comparing `punkweb_bb-0.2.0/punkweb_bb/static/punkweb_bb/vendor/sceditor-3.2.0/emoticons/blink.png` & `punkweb_bb-0.2.1/punkweb_bb/static/punkweb_bb/vendor/sceditor-3.2.0/emoticons/blink.png`

 * *Files identical despite different names*

### Comparing `punkweb_bb-0.2.0/punkweb_bb/static/punkweb_bb/vendor/sceditor-3.2.0/emoticons/blush.png` & `punkweb_bb-0.2.1/punkweb_bb/static/punkweb_bb/vendor/sceditor-3.2.0/emoticons/blush.png`

 * *Files identical despite different names*

### Comparing `punkweb_bb-0.2.0/punkweb_bb/static/punkweb_bb/vendor/sceditor-3.2.0/emoticons/cheerful.png` & `punkweb_bb-0.2.1/punkweb_bb/static/punkweb_bb/vendor/sceditor-3.2.0/emoticons/cheerful.png`

 * *Files identical despite different names*

### Comparing `punkweb_bb-0.2.0/punkweb_bb/static/punkweb_bb/vendor/sceditor-3.2.0/emoticons/cool.png` & `punkweb_bb-0.2.1/punkweb_bb/static/punkweb_bb/vendor/sceditor-3.2.0/emoticons/cool.png`

 * *Files identical despite different names*

### Comparing `punkweb_bb-0.2.0/punkweb_bb/static/punkweb_bb/vendor/sceditor-3.2.0/emoticons/cwy.png` & `punkweb_bb-0.2.1/punkweb_bb/static/punkweb_bb/vendor/sceditor-3.2.0/emoticons/cwy.png`

 * *Files identical despite different names*

### Comparing `punkweb_bb-0.2.0/punkweb_bb/static/punkweb_bb/vendor/sceditor-3.2.0/emoticons/devil.png` & `punkweb_bb-0.2.1/punkweb_bb/static/punkweb_bb/vendor/sceditor-3.2.0/emoticons/devil.png`

 * *Files identical despite different names*

### Comparing `punkweb_bb-0.2.0/punkweb_bb/static/punkweb_bb/vendor/sceditor-3.2.0/emoticons/dizzy.png` & `punkweb_bb-0.2.1/punkweb_bb/static/punkweb_bb/vendor/sceditor-3.2.0/emoticons/dizzy.png`

 * *Files identical despite different names*

### Comparing `punkweb_bb-0.2.0/punkweb_bb/static/punkweb_bb/vendor/sceditor-3.2.0/emoticons/ermm.png` & `punkweb_bb-0.2.1/punkweb_bb/static/punkweb_bb/vendor/sceditor-3.2.0/emoticons/ermm.png`

 * *Files identical despite different names*

### Comparing `punkweb_bb-0.2.0/punkweb_bb/static/punkweb_bb/vendor/sceditor-3.2.0/emoticons/face.png` & `punkweb_bb-0.2.1/punkweb_bb/static/punkweb_bb/vendor/sceditor-3.2.0/emoticons/face.png`

 * *Files identical despite different names*

### Comparing `punkweb_bb-0.2.0/punkweb_bb/static/punkweb_bb/vendor/sceditor-3.2.0/emoticons/getlost.png` & `punkweb_bb-0.2.1/punkweb_bb/static/punkweb_bb/vendor/sceditor-3.2.0/emoticons/getlost.png`

 * *Files identical despite different names*

### Comparing `punkweb_bb-0.2.0/punkweb_bb/static/punkweb_bb/vendor/sceditor-3.2.0/emoticons/grin.png` & `punkweb_bb-0.2.1/punkweb_bb/static/punkweb_bb/vendor/sceditor-3.2.0/emoticons/grin.png`

 * *Files identical despite different names*

### Comparing `punkweb_bb-0.2.0/punkweb_bb/static/punkweb_bb/vendor/sceditor-3.2.0/emoticons/happy.png` & `punkweb_bb-0.2.1/punkweb_bb/static/punkweb_bb/vendor/sceditor-3.2.0/emoticons/happy.png`

 * *Files identical despite different names*

### Comparing `punkweb_bb-0.2.0/punkweb_bb/static/punkweb_bb/vendor/sceditor-3.2.0/emoticons/heart.png` & `punkweb_bb-0.2.1/punkweb_bb/static/punkweb_bb/vendor/sceditor-3.2.0/emoticons/heart.png`

 * *Files identical despite different names*

### Comparing `punkweb_bb-0.2.0/punkweb_bb/static/punkweb_bb/vendor/sceditor-3.2.0/emoticons/kissing.png` & `punkweb_bb-0.2.1/punkweb_bb/static/punkweb_bb/vendor/sceditor-3.2.0/emoticons/kissing.png`

 * *Files identical despite different names*

### Comparing `punkweb_bb-0.2.0/punkweb_bb/static/punkweb_bb/vendor/sceditor-3.2.0/emoticons/laughing.png` & `punkweb_bb-0.2.1/punkweb_bb/static/punkweb_bb/vendor/sceditor-3.2.0/emoticons/laughing.png`

 * *Files identical despite different names*

### Comparing `punkweb_bb-0.2.0/punkweb_bb/static/punkweb_bb/vendor/sceditor-3.2.0/emoticons/ninja.png` & `punkweb_bb-0.2.1/punkweb_bb/static/punkweb_bb/vendor/sceditor-3.2.0/emoticons/ninja.png`

 * *Files identical despite different names*

### Comparing `punkweb_bb-0.2.0/punkweb_bb/static/punkweb_bb/vendor/sceditor-3.2.0/emoticons/pinch.png` & `punkweb_bb-0.2.1/punkweb_bb/static/punkweb_bb/vendor/sceditor-3.2.0/emoticons/pinch.png`

 * *Files identical despite different names*

### Comparing `punkweb_bb-0.2.0/punkweb_bb/static/punkweb_bb/vendor/sceditor-3.2.0/emoticons/pouty.png` & `punkweb_bb-0.2.1/punkweb_bb/static/punkweb_bb/vendor/sceditor-3.2.0/emoticons/pouty.png`

 * *Files identical despite different names*

### Comparing `punkweb_bb-0.2.0/punkweb_bb/static/punkweb_bb/vendor/sceditor-3.2.0/emoticons/sad.png` & `punkweb_bb-0.2.1/punkweb_bb/static/punkweb_bb/vendor/sceditor-3.2.0/emoticons/sad.png`

 * *Files identical despite different names*

### Comparing `punkweb_bb-0.2.0/punkweb_bb/static/punkweb_bb/vendor/sceditor-3.2.0/emoticons/shocked.png` & `punkweb_bb-0.2.1/punkweb_bb/static/punkweb_bb/vendor/sceditor-3.2.0/emoticons/shocked.png`

 * *Files identical despite different names*

### Comparing `punkweb_bb-0.2.0/punkweb_bb/static/punkweb_bb/vendor/sceditor-3.2.0/emoticons/sick.png` & `punkweb_bb-0.2.1/punkweb_bb/static/punkweb_bb/vendor/sceditor-3.2.0/emoticons/sick.png`

 * *Files identical despite different names*

### Comparing `punkweb_bb-0.2.0/punkweb_bb/static/punkweb_bb/vendor/sceditor-3.2.0/emoticons/sideways.png` & `punkweb_bb-0.2.1/punkweb_bb/static/punkweb_bb/vendor/sceditor-3.2.0/emoticons/sideways.png`

 * *Files identical despite different names*

### Comparing `punkweb_bb-0.2.0/punkweb_bb/static/punkweb_bb/vendor/sceditor-3.2.0/emoticons/silly.png` & `punkweb_bb-0.2.1/punkweb_bb/static/punkweb_bb/vendor/sceditor-3.2.0/emoticons/silly.png`

 * *Files identical despite different names*

### Comparing `punkweb_bb-0.2.0/punkweb_bb/static/punkweb_bb/vendor/sceditor-3.2.0/emoticons/sleeping.png` & `punkweb_bb-0.2.1/punkweb_bb/static/punkweb_bb/vendor/sceditor-3.2.0/emoticons/sleeping.png`

 * *Files identical despite different names*

### Comparing `punkweb_bb-0.2.0/punkweb_bb/static/punkweb_bb/vendor/sceditor-3.2.0/emoticons/smile.png` & `punkweb_bb-0.2.1/punkweb_bb/static/punkweb_bb/vendor/sceditor-3.2.0/emoticons/smile.png`

 * *Files identical despite different names*

### Comparing `punkweb_bb-0.2.0/punkweb_bb/static/punkweb_bb/vendor/sceditor-3.2.0/emoticons/tongue.png` & `punkweb_bb-0.2.1/punkweb_bb/static/punkweb_bb/vendor/sceditor-3.2.0/emoticons/tongue.png`

 * *Files identical despite different names*

### Comparing `punkweb_bb-0.2.0/punkweb_bb/static/punkweb_bb/vendor/sceditor-3.2.0/emoticons/unsure.png` & `punkweb_bb-0.2.1/punkweb_bb/static/punkweb_bb/vendor/sceditor-3.2.0/emoticons/unsure.png`

 * *Files identical despite different names*

### Comparing `punkweb_bb-0.2.0/punkweb_bb/static/punkweb_bb/vendor/sceditor-3.2.0/emoticons/w00t.png` & `punkweb_bb-0.2.1/punkweb_bb/static/punkweb_bb/vendor/sceditor-3.2.0/emoticons/w00t.png`

 * *Files identical despite different names*

### Comparing `punkweb_bb-0.2.0/punkweb_bb/static/punkweb_bb/vendor/sceditor-3.2.0/emoticons/wassat.png` & `punkweb_bb-0.2.1/punkweb_bb/static/punkweb_bb/vendor/sceditor-3.2.0/emoticons/wassat.png`

 * *Files identical despite different names*

### Comparing `punkweb_bb-0.2.0/punkweb_bb/static/punkweb_bb/vendor/sceditor-3.2.0/emoticons/whistling.png` & `punkweb_bb-0.2.1/punkweb_bb/static/punkweb_bb/vendor/sceditor-3.2.0/emoticons/whistling.png`

 * *Files identical despite different names*

### Comparing `punkweb_bb-0.2.0/punkweb_bb/static/punkweb_bb/vendor/sceditor-3.2.0/emoticons/wink.png` & `punkweb_bb-0.2.1/punkweb_bb/static/punkweb_bb/vendor/sceditor-3.2.0/emoticons/wink.png`

 * *Files identical despite different names*

### Comparing `punkweb_bb-0.2.0/punkweb_bb/static/punkweb_bb/vendor/sceditor-3.2.0/emoticons/wub.png` & `punkweb_bb-0.2.1/punkweb_bb/static/punkweb_bb/vendor/sceditor-3.2.0/emoticons/wub.png`

 * *Files identical despite different names*

### Comparing `punkweb_bb-0.2.0/punkweb_bb/static/punkweb_bb/vendor/sceditor-3.2.0/example.html` & `punkweb_bb-0.2.1/punkweb_bb/static/punkweb_bb/vendor/sceditor-3.2.0/example.html`

 * *Files identical despite different names*

### Comparing `punkweb_bb-0.2.0/punkweb_bb/static/punkweb_bb/vendor/sceditor-3.2.0/languages/ar.js` & `punkweb_bb-0.2.1/punkweb_bb/static/punkweb_bb/vendor/sceditor-3.2.0/languages/ar.js`

 * *Files identical despite different names*

### Comparing `punkweb_bb-0.2.0/punkweb_bb/static/punkweb_bb/vendor/sceditor-3.2.0/languages/ca.js` & `punkweb_bb-0.2.1/punkweb_bb/static/punkweb_bb/vendor/sceditor-3.2.0/languages/ca.js`

 * *Files identical despite different names*

### Comparing `punkweb_bb-0.2.0/punkweb_bb/static/punkweb_bb/vendor/sceditor-3.2.0/languages/cn.js` & `punkweb_bb-0.2.1/punkweb_bb/static/punkweb_bb/vendor/sceditor-3.2.0/languages/cn.js`

 * *Files identical despite different names*

### Comparing `punkweb_bb-0.2.0/punkweb_bb/static/punkweb_bb/vendor/sceditor-3.2.0/languages/cs.js` & `punkweb_bb-0.2.1/punkweb_bb/static/punkweb_bb/vendor/sceditor-3.2.0/languages/cs.js`

 * *Files identical despite different names*

### Comparing `punkweb_bb-0.2.0/punkweb_bb/static/punkweb_bb/vendor/sceditor-3.2.0/languages/de.js` & `punkweb_bb-0.2.1/punkweb_bb/static/punkweb_bb/vendor/sceditor-3.2.0/languages/de.js`

 * *Files identical despite different names*

### Comparing `punkweb_bb-0.2.0/punkweb_bb/static/punkweb_bb/vendor/sceditor-3.2.0/languages/el.js` & `punkweb_bb-0.2.1/punkweb_bb/static/punkweb_bb/vendor/sceditor-3.2.0/languages/el.js`

 * *Files identical despite different names*

### Comparing `punkweb_bb-0.2.0/punkweb_bb/static/punkweb_bb/vendor/sceditor-3.2.0/languages/es.js` & `punkweb_bb-0.2.1/punkweb_bb/static/punkweb_bb/vendor/sceditor-3.2.0/languages/es.js`

 * *Files identical despite different names*

### Comparing `punkweb_bb-0.2.0/punkweb_bb/static/punkweb_bb/vendor/sceditor-3.2.0/languages/et.js` & `punkweb_bb-0.2.1/punkweb_bb/static/punkweb_bb/vendor/sceditor-3.2.0/languages/et.js`

 * *Files identical despite different names*

### Comparing `punkweb_bb-0.2.0/punkweb_bb/static/punkweb_bb/vendor/sceditor-3.2.0/languages/fa.js` & `punkweb_bb-0.2.1/punkweb_bb/static/punkweb_bb/vendor/sceditor-3.2.0/languages/fa.js`

 * *Files identical despite different names*

### Comparing `punkweb_bb-0.2.0/punkweb_bb/static/punkweb_bb/vendor/sceditor-3.2.0/languages/fi.js` & `punkweb_bb-0.2.1/punkweb_bb/static/punkweb_bb/vendor/sceditor-3.2.0/languages/fi.js`

 * *Files identical despite different names*

### Comparing `punkweb_bb-0.2.0/punkweb_bb/static/punkweb_bb/vendor/sceditor-3.2.0/languages/fr.js` & `punkweb_bb-0.2.1/punkweb_bb/static/punkweb_bb/vendor/sceditor-3.2.0/languages/fr.js`

 * *Files identical despite different names*

### Comparing `punkweb_bb-0.2.0/punkweb_bb/static/punkweb_bb/vendor/sceditor-3.2.0/languages/gl.js` & `punkweb_bb-0.2.1/punkweb_bb/static/punkweb_bb/vendor/sceditor-3.2.0/languages/gl.js`

 * *Files identical despite different names*

### Comparing `punkweb_bb-0.2.0/punkweb_bb/static/punkweb_bb/vendor/sceditor-3.2.0/languages/hu.js` & `punkweb_bb-0.2.1/punkweb_bb/static/punkweb_bb/vendor/sceditor-3.2.0/languages/hu.js`

 * *Files identical despite different names*

### Comparing `punkweb_bb-0.2.0/punkweb_bb/static/punkweb_bb/vendor/sceditor-3.2.0/languages/id.js` & `punkweb_bb-0.2.1/punkweb_bb/static/punkweb_bb/vendor/sceditor-3.2.0/languages/id.js`

 * *Files identical despite different names*

### Comparing `punkweb_bb-0.2.0/punkweb_bb/static/punkweb_bb/vendor/sceditor-3.2.0/languages/it.js` & `punkweb_bb-0.2.1/punkweb_bb/static/punkweb_bb/vendor/sceditor-3.2.0/languages/it.js`

 * *Files identical despite different names*

### Comparing `punkweb_bb-0.2.0/punkweb_bb/static/punkweb_bb/vendor/sceditor-3.2.0/languages/ja.js` & `punkweb_bb-0.2.1/punkweb_bb/static/punkweb_bb/vendor/sceditor-3.2.0/languages/ja.js`

 * *Files identical despite different names*

### Comparing `punkweb_bb-0.2.0/punkweb_bb/static/punkweb_bb/vendor/sceditor-3.2.0/languages/lt.js` & `punkweb_bb-0.2.1/punkweb_bb/static/punkweb_bb/vendor/sceditor-3.2.0/languages/lt.js`

 * *Files identical despite different names*

### Comparing `punkweb_bb-0.2.0/punkweb_bb/static/punkweb_bb/vendor/sceditor-3.2.0/languages/nb.js` & `punkweb_bb-0.2.1/punkweb_bb/static/punkweb_bb/vendor/sceditor-3.2.0/languages/nb.js`

 * *Files identical despite different names*

### Comparing `punkweb_bb-0.2.0/punkweb_bb/static/punkweb_bb/vendor/sceditor-3.2.0/languages/nl.js` & `punkweb_bb-0.2.1/punkweb_bb/static/punkweb_bb/vendor/sceditor-3.2.0/languages/nl.js`

 * *Files identical despite different names*

### Comparing `punkweb_bb-0.2.0/punkweb_bb/static/punkweb_bb/vendor/sceditor-3.2.0/languages/pl.js` & `punkweb_bb-0.2.1/punkweb_bb/static/punkweb_bb/vendor/sceditor-3.2.0/languages/pl.js`

 * *Files identical despite different names*

### Comparing `punkweb_bb-0.2.0/punkweb_bb/static/punkweb_bb/vendor/sceditor-3.2.0/languages/pt-BR.js` & `punkweb_bb-0.2.1/punkweb_bb/static/punkweb_bb/vendor/sceditor-3.2.0/languages/pt-BR.js`

 * *Files identical despite different names*

### Comparing `punkweb_bb-0.2.0/punkweb_bb/static/punkweb_bb/vendor/sceditor-3.2.0/languages/pt.js` & `punkweb_bb-0.2.1/punkweb_bb/static/punkweb_bb/vendor/sceditor-3.2.0/languages/pt.js`

 * *Files identical despite different names*

### Comparing `punkweb_bb-0.2.0/punkweb_bb/static/punkweb_bb/vendor/sceditor-3.2.0/languages/ru.js` & `punkweb_bb-0.2.1/punkweb_bb/static/punkweb_bb/vendor/sceditor-3.2.0/languages/ru.js`

 * *Files identical despite different names*

### Comparing `punkweb_bb-0.2.0/punkweb_bb/static/punkweb_bb/vendor/sceditor-3.2.0/languages/sk.js` & `punkweb_bb-0.2.1/punkweb_bb/static/punkweb_bb/vendor/sceditor-3.2.0/languages/sk.js`

 * *Files identical despite different names*

### Comparing `punkweb_bb-0.2.0/punkweb_bb/static/punkweb_bb/vendor/sceditor-3.2.0/languages/sv.js` & `punkweb_bb-0.2.1/punkweb_bb/static/punkweb_bb/vendor/sceditor-3.2.0/languages/sv.js`

 * *Files identical despite different names*

### Comparing `punkweb_bb-0.2.0/punkweb_bb/static/punkweb_bb/vendor/sceditor-3.2.0/languages/template.js` & `punkweb_bb-0.2.1/punkweb_bb/static/punkweb_bb/vendor/sceditor-3.2.0/languages/template.js`

 * *Files identical despite different names*

### Comparing `punkweb_bb-0.2.0/punkweb_bb/static/punkweb_bb/vendor/sceditor-3.2.0/languages/tr.js` & `punkweb_bb-0.2.1/punkweb_bb/static/punkweb_bb/vendor/sceditor-3.2.0/languages/tr.js`

 * *Files identical despite different names*

### Comparing `punkweb_bb-0.2.0/punkweb_bb/static/punkweb_bb/vendor/sceditor-3.2.0/languages/tw.js` & `punkweb_bb-0.2.1/punkweb_bb/static/punkweb_bb/vendor/sceditor-3.2.0/languages/tw.js`

 * *Files identical despite different names*

### Comparing `punkweb_bb-0.2.0/punkweb_bb/static/punkweb_bb/vendor/sceditor-3.2.0/languages/uk.js` & `punkweb_bb-0.2.1/punkweb_bb/static/punkweb_bb/vendor/sceditor-3.2.0/languages/uk.js`

 * *Files identical despite different names*

### Comparing `punkweb_bb-0.2.0/punkweb_bb/static/punkweb_bb/vendor/sceditor-3.2.0/languages/vi.js` & `punkweb_bb-0.2.1/punkweb_bb/static/punkweb_bb/vendor/sceditor-3.2.0/languages/vi.js`

 * *Files identical despite different names*

### Comparing `punkweb_bb-0.2.0/punkweb_bb/static/punkweb_bb/vendor/sceditor-3.2.0/minified/formats/bbcode.js` & `punkweb_bb-0.2.1/punkweb_bb/static/punkweb_bb/vendor/sceditor-3.2.0/minified/formats/bbcode.js`

 * *Files identical despite different names*

### Comparing `punkweb_bb-0.2.0/punkweb_bb/static/punkweb_bb/vendor/sceditor-3.2.0/minified/formats/xhtml.js` & `punkweb_bb-0.2.1/punkweb_bb/static/punkweb_bb/vendor/sceditor-3.2.0/minified/formats/xhtml.js`

 * *Files identical despite different names*

### Comparing `punkweb_bb-0.2.0/punkweb_bb/static/punkweb_bb/vendor/sceditor-3.2.0/minified/icons/material.js` & `punkweb_bb-0.2.1/punkweb_bb/static/punkweb_bb/vendor/sceditor-3.2.0/minified/icons/material.js`

 * *Files identical despite different names*

### Comparing `punkweb_bb-0.2.0/punkweb_bb/static/punkweb_bb/vendor/sceditor-3.2.0/minified/icons/monocons.js` & `punkweb_bb-0.2.1/punkweb_bb/static/punkweb_bb/vendor/sceditor-3.2.0/minified/icons/monocons.js`

 * *Files identical despite different names*

### Comparing `punkweb_bb-0.2.0/punkweb_bb/static/punkweb_bb/vendor/sceditor-3.2.0/minified/jquery.sceditor.bbcode.min.js` & `punkweb_bb-0.2.1/punkweb_bb/static/punkweb_bb/vendor/sceditor-3.2.0/minified/jquery.sceditor.bbcode.min.js`

 * *Files identical despite different names*

### Comparing `punkweb_bb-0.2.0/punkweb_bb/static/punkweb_bb/vendor/sceditor-3.2.0/minified/jquery.sceditor.min.js` & `punkweb_bb-0.2.1/punkweb_bb/static/punkweb_bb/vendor/sceditor-3.2.0/minified/jquery.sceditor.min.js`

 * *Files identical despite different names*

### Comparing `punkweb_bb-0.2.0/punkweb_bb/static/punkweb_bb/vendor/sceditor-3.2.0/minified/jquery.sceditor.xhtml.min.js` & `punkweb_bb-0.2.1/punkweb_bb/static/punkweb_bb/vendor/sceditor-3.2.0/minified/jquery.sceditor.xhtml.min.js`

 * *Files identical despite different names*

### Comparing `punkweb_bb-0.2.0/punkweb_bb/static/punkweb_bb/vendor/sceditor-3.2.0/minified/plugins/alternative-lists.js` & `punkweb_bb-0.2.1/punkweb_bb/static/punkweb_bb/vendor/sceditor-3.2.0/minified/plugins/alternative-lists.js`

 * *Files identical despite different names*

### Comparing `punkweb_bb-0.2.0/punkweb_bb/static/punkweb_bb/vendor/sceditor-3.2.0/minified/plugins/autosave.js` & `punkweb_bb-0.2.1/punkweb_bb/static/punkweb_bb/vendor/sceditor-3.2.0/minified/plugins/autosave.js`

 * *Files identical despite different names*

### Comparing `punkweb_bb-0.2.0/punkweb_bb/static/punkweb_bb/vendor/sceditor-3.2.0/minified/plugins/autoyoutube.js` & `punkweb_bb-0.2.1/punkweb_bb/static/punkweb_bb/vendor/sceditor-3.2.0/minified/plugins/autoyoutube.js`

 * *Files identical despite different names*

### Comparing `punkweb_bb-0.2.0/punkweb_bb/static/punkweb_bb/vendor/sceditor-3.2.0/minified/plugins/dragdrop.js` & `punkweb_bb-0.2.1/punkweb_bb/static/punkweb_bb/vendor/sceditor-3.2.0/minified/plugins/dragdrop.js`

 * *Files identical despite different names*

### Comparing `punkweb_bb-0.2.0/punkweb_bb/static/punkweb_bb/vendor/sceditor-3.2.0/minified/plugins/format.js` & `punkweb_bb-0.2.1/punkweb_bb/static/punkweb_bb/vendor/sceditor-3.2.0/minified/plugins/format.js`

 * *Files identical despite different names*

### Comparing `punkweb_bb-0.2.0/punkweb_bb/static/punkweb_bb/vendor/sceditor-3.2.0/minified/plugins/plaintext.js` & `punkweb_bb-0.2.1/punkweb_bb/static/punkweb_bb/vendor/sceditor-3.2.0/minified/plugins/plaintext.js`

 * *Files identical despite different names*

### Comparing `punkweb_bb-0.2.0/punkweb_bb/static/punkweb_bb/vendor/sceditor-3.2.0/minified/plugins/undo.js` & `punkweb_bb-0.2.1/punkweb_bb/static/punkweb_bb/vendor/sceditor-3.2.0/minified/plugins/undo.js`

 * *Files identical despite different names*

### Comparing `punkweb_bb-0.2.0/punkweb_bb/static/punkweb_bb/vendor/sceditor-3.2.0/minified/plugins/v1compat.js` & `punkweb_bb-0.2.1/punkweb_bb/static/punkweb_bb/vendor/sceditor-3.2.0/minified/plugins/v1compat.js`

 * *Files identical despite different names*

### Comparing `punkweb_bb-0.2.0/punkweb_bb/static/punkweb_bb/vendor/sceditor-3.2.0/minified/sceditor.min.js` & `punkweb_bb-0.2.1/punkweb_bb/static/punkweb_bb/vendor/sceditor-3.2.0/minified/sceditor.min.js`

 * *Files identical despite different names*

### Comparing `punkweb_bb-0.2.0/punkweb_bb/static/punkweb_bb/vendor/sceditor-3.2.0/minified/themes/content/default.min.css` & `punkweb_bb-0.2.1/punkweb_bb/static/punkweb_bb/vendor/sceditor-3.2.0/minified/themes/content/default.min.css`

 * *Files identical despite different names*

### Comparing `punkweb_bb-0.2.0/punkweb_bb/static/punkweb_bb/vendor/sceditor-3.2.0/minified/themes/default.min.css` & `punkweb_bb-0.2.1/punkweb_bb/static/punkweb_bb/vendor/sceditor-3.2.0/minified/themes/default.min.css`

 * *Files identical despite different names*

### Comparing `punkweb_bb-0.2.0/punkweb_bb/static/punkweb_bb/vendor/sceditor-3.2.0/minified/themes/defaultdark.min.css` & `punkweb_bb-0.2.1/punkweb_bb/static/punkweb_bb/vendor/sceditor-3.2.0/minified/themes/defaultdark.min.css`

 * *Files identical despite different names*

### Comparing `punkweb_bb-0.2.0/punkweb_bb/static/punkweb_bb/vendor/sceditor-3.2.0/minified/themes/famfamfam.png` & `punkweb_bb-0.2.1/punkweb_bb/static/punkweb_bb/vendor/sceditor-3.2.0/minified/themes/famfamfam.png`

 * *Files identical despite different names*

### Comparing `punkweb_bb-0.2.0/punkweb_bb/static/punkweb_bb/vendor/sceditor-3.2.0/minified/themes/modern.min.css` & `punkweb_bb-0.2.1/punkweb_bb/static/punkweb_bb/vendor/sceditor-3.2.0/minified/themes/modern.min.css`

 * *Files identical despite different names*

### Comparing `punkweb_bb-0.2.0/punkweb_bb/static/punkweb_bb/vendor/sceditor-3.2.0/minified/themes/office-toolbar.min.css` & `punkweb_bb-0.2.1/punkweb_bb/static/punkweb_bb/vendor/sceditor-3.2.0/minified/themes/office-toolbar.min.css`

 * *Files identical despite different names*

### Comparing `punkweb_bb-0.2.0/punkweb_bb/static/punkweb_bb/vendor/sceditor-3.2.0/minified/themes/office.min.css` & `punkweb_bb-0.2.1/punkweb_bb/static/punkweb_bb/vendor/sceditor-3.2.0/minified/themes/office.min.css`

 * *Files identical despite different names*

### Comparing `punkweb_bb-0.2.0/punkweb_bb/static/punkweb_bb/vendor/sceditor-3.2.0/minified/themes/square.min.css` & `punkweb_bb-0.2.1/punkweb_bb/static/punkweb_bb/vendor/sceditor-3.2.0/minified/themes/square.min.css`

 * *Files identical despite different names*

### Comparing `punkweb_bb-0.2.0/punkweb_bb/templates/punkweb_bb/base.html` & `punkweb_bb-0.2.1/punkweb_bb/templates/punkweb_bb/base.html`

 * *Files 10% similar despite different names*

```diff
@@ -2,14 +2,20 @@
 
 <!DOCTYPE html>
 <html lang="en">
 <head>
   <meta charset="UTF-8" />
   <meta name="viewport" content="width=device-width, initial-scale=1.0" />
   <title>{% block title_prefix %}{% endblock %}{{ punkweb_bb.settings.SITE_TITLE|default:"PunkwebBB" }}</title>
+  <meta property="og:title" content="{% block og_title_prefix %}{% endblock %}{{ punkweb_bb.settings.SITE_TITLE|default:"PunkwebBB" }}" />
+  <meta property="og:type" content="website" />
+  <meta property="og:url" content="{{ request.build_absolute_uri }}" />
+  {% if punkweb_bb.settings.OG_IMAGE %}
+  <meta property="og:image" content="{{ punkweb_bb.settings.OG_IMAGE }}" />
+  {% endif %}
   <link rel="icon" href="{% static punkweb_bb.settings.FAVICON %}" />
   <link rel="stylesheet" href="{% static 'punkweb_bb/vendor/open-color.css' %}" />
   <link rel="stylesheet" href="{% static 'punkweb_bb/vendor/prism.css' %}" />
   <link rel="stylesheet" href="{% static 'punkweb_bb/css/defaults.css' %}" />
   <link rel="stylesheet" href="{% static 'punkweb_bb/css/variables.css' %}" />
   <link rel="stylesheet" href="{% static 'punkweb_bb/css/typography.css' %}" />
   <link rel="stylesheet" href="{% static 'punkweb_bb/css/punkweb.css' %}" />
```

#### html2text {}

```diff
@@ -1,8 +1,11 @@
 {% load static %}
+}" />
+{% if punkweb_bb.settings.OG_IMAGE %}
+{% endif %}
 {% block extra_head %}{% endblock %}
 {% if request.user.is_staff %}
 _A_d_m_i_n
 {% endif %}
 {% if request.user.is_authenticated %}
 _P_r_o_f_i_l_e_ _S_e_t_t_i_n_g_s_ _L_o_g_o_u_t
 {% else %}
```

### Comparing `punkweb_bb-0.2.0/punkweb_bb/templates/punkweb_bb/category_create.html` & `punkweb_bb-0.2.1/punkweb_bb/templates/punkweb_bb/category_create.html`

 * *Files identical despite different names*

### Comparing `punkweb_bb-0.2.0/punkweb_bb/templates/punkweb_bb/category_update.html` & `punkweb_bb-0.2.1/punkweb_bb/templates/punkweb_bb/category_update.html`

 * *Files identical despite different names*

### Comparing `punkweb_bb-0.2.0/punkweb_bb/templates/punkweb_bb/index.html` & `punkweb_bb-0.2.1/punkweb_bb/templates/punkweb_bb/index.html`

 * *Files 4% similar despite different names*

```diff
@@ -27,44 +27,53 @@
               <col span="1">
               <col span="1" width="96px">
               <col span="1" width="96px">
               <col span="1" width="320px">
             </colgroup>
             <thead>
               <tr>
-                <th><a href="{{category.get_absolute_url}}">{{category.name}}</a></th>
-                <th>Threads</th>
-                <th>Posts</th>
-                <th></th>
-              </tr>
-            </thead>
-            <tbody>
-              {% if perms.punkweb_bb.add_subcategory or perms.punkweb_bb.change_category or perms.punkweb_bb.delete_category %}
-              <tr>
-                <td colspan="4">
-                  <div class="index__category__actions">
+                <th>
+                  <div class="index__category__title">
+                    <a href="{{category.get_absolute_url}}">{{category.name}}</a>
                     {% if perms.punkweb_bb.add_subcategory %}
-                    <a class="pw-button ghost xs" href="{% url 'punkweb_bb:subcategory_create' category.slug %}">
-                      Create Subcategory
+                    <a
+                      class="pw-icon-button default rounded sm"
+                      href="{% url 'punkweb_bb:subcategory_create' category.slug %}"
+                      title="Create subcategory"
+                    >
+                      <span class="material-symbols-outlined">add</span>
                     </a>
                     {% endif %}
                     {% if perms.punkweb_bb.change_category %}
-                    <a class="pw-button ghost xs" href="{% url 'punkweb_bb:category_update' category.slug %}">
-                      Edit
+                    <a
+                      class="pw-icon-button default rounded sm"
+                      href="{% url 'punkweb_bb:category_update' category.slug %}"
+                      title="Edit category"
+                    >
+                      <span class="material-symbols-outlined">edit</span>
                     </a>
                     {% endif %}
                     {% if perms.punkweb_bb.delete_category %}
-                    <a class="pw-button ghost danger xs" hx-get="{% url 'punkweb_bb:category_delete' category.slug %}" hx-target="#modal-portal">
-                      Delete
+                    <a
+                      class="pw-icon-button default danger rounded sm"
+                      title="Delete category"
+                      hx-get="{% url 'punkweb_bb:category_delete' category.slug %}"
+                      hx-target="#modal-portal"
+                    >
+                    <span class="material-symbols-outlined">delete</span>
                     </a>
                     {% endif %}
                   </div>
-                </td>
+                </th>
+                <th>Threads</th>
+                <th>Posts</th>
+                <th></th>
               </tr>
-              {% endif %}
+            </thead>
+            <tbody>
               {% for subcategory in category.subcategories.all %}
               <tr>
                 <td>
                   <a href="{{subcategory.get_absolute_url}}" title="{{subcategory.name}}">{{subcategory.name}}</a>
                   <div>
                     {{subcategory.description.rendered}}
                   </div>
@@ -130,15 +139,21 @@
               {% endfor %}
             </tbody>
           </table>
         </div>
       </div>
       {% endfor %}
       {% if perms.punkweb_bb.add_category %}
-      <a class="pw-button ghost xs" href="{% url 'punkweb_bb:category_create' %}">Create Category</a>
+      <a
+        class="pw-icon-button raised primary rounded"
+        href="{% url 'punkweb_bb:category_create' %}"
+        title="Create category"
+      >
+        <span class="material-symbols-outlined">add</span>
+      </a>
       {% endif %}
     </div>
     <div class="index__sidebar">
       <div class="pw-card fluid">
         <div class="pw-card-header">Recent threads</div>
         <div class="index__recentThreads__content">
           {% for thread in recent_threads %}
```

#### html2text {}

```diff
@@ -1,16 +1,20 @@
 {% extends 'punkweb_bb/base.html' %} {% load static %} {% block extra_head %}
 {% endblock %} {% block extra_script %}
 {% endblock %} {% block content %}
 {% if punkweb_bb.settings.SHOUTBOX_ENABLED|default:True %} {% include
 'punkweb_bb/shoutbox/shoutbox.html' %} {% endif %} {% for category in
 categories %}
-_{{_{{_cc_aa_tt_ee_gg_oo_rr_yy_.._nn_aa_mm_ee_}}_}}                   TThhrreeaaddss                     PPoossttss
-{% if perms.punkweb_bb.add_subcategory %} _C_r_e_a_t_e_ _S_u_b_c_a_t_e_g_o_r_y_ {% endif %} {% if perms.punkweb_bb.change_category %} _E_d_i_t_ {% endif %} {% if
-perms.punkweb_bb.delete_category %} Delete {% endif %}
+_{{_{{_cc_aa_tt_ee_gg_oo_rr_yy_.._nn_aa_mm_ee_}}_}} {{%% iiff
+ppeerrmmss..ppuunnkkwweebb__bbbb..aadddd__ssuubbccaatteeggoorryy %%}}
+_aa_dd_dd_ {{%% eennddiiff %%}} {{%% iiff
+ppeerrmmss..ppuunnkkwweebb__bbbb..cchhaannggee__ccaatteeggoorryy %%}} TThhrreeaaddss                     PPoossttss
+_ee_dd_ii_tt_ {{%% eennddiiff %%}} {{%% iiff
+ppeerrmmss..ppuunnkkwweebb__bbbb..ddeelleettee__ccaatteeggoorryy %%}}
+ddeelleettee {{%% eennddiiff %%}}
                                                                                           {% if subcategory.latest_thread %} {% if
                                                                                           subcategory.latest_thread.latest_post %}
                                                                                           {% if subcategory.latest_thread.latest_post.user.profile.image
                                                                                           %} [{
                                                                                           {subcategory.latest_thread.latest_post.user.profile.image.url}}]
                                                                                           {% else%} [{% static 'punkweb_bb/img/default-profile-image.png'
                                                                                           %}]{% endif %}
@@ -25,15 +29,15 @@
                                                                                           {% static 'punkweb_bb/img/default-profile-image.png' %}]{% endif
                                                                                           %}
                                                                                           _{_{_s_u_b_c_a_t_e_g_o_r_y_._l_a_t_e_s_t___t_h_r_e_a_d_._t_i_t_l_e_}_}
                                                                                           {{subcategory.latest_thread.created_at|date:'M j, Y'}} at {
                                                                                           {subcategory.latest_thread.created_at|date:'g:i A'}} â¢ _{
                                                                                           _{_s_u_b_c_a_t_e_g_o_r_y_._l_a_t_e_s_t___t_h_r_e_a_d_._u_s_e_r_._u_s_e_r_n_a_m_e_}_}
                                                                                           {% endif %} {% else %} No threads {% endif %}
-{% endfor %} {% if perms.punkweb_bb.add_category %} _C_r_e_a_t_e_ _C_a_t_e_g_o_r_y {% endif %}
+{% endfor %} {% if perms.punkweb_bb.add_category %} _a_d_d_ {% endif %}
 Recent threads
 {% for thread in recent_threads %}
 {% if thread.user.profile.image %} [{{thread.user.profile.image.url}}]{% else%}
 [{% static 'punkweb_bb/img/default-profile-image.png' %}]{% endif %}
 _{_{_t_h_r_e_a_d_._t_i_t_l_e_}_}
 {{thread.created_at|date:'M j, Y'}} at {{thread.created_at|date:'g:i A'}} â¢ _{
 _{_t_h_r_e_a_d_._u_s_e_r_._u_s_e_r_n_a_m_e_}_}
```

### Comparing `punkweb_bb-0.2.0/punkweb_bb/templates/punkweb_bb/login.html` & `punkweb_bb-0.2.1/punkweb_bb/templates/punkweb_bb/login.html`

 * *Files 10% similar despite different names*

```diff
@@ -1,11 +1,12 @@
 {% extends 'punkweb_bb/base.html' %}
 {% load static %}
 
 {% block title_prefix %}Login | {% endblock%}
+{% block og_title_prefix %}Login | {% endblock %}
 
 {% block extra_head %}
 <link rel="stylesheet" href="{% static 'punkweb_bb/css/login.css' %}" />
 {% endblock %}
 
 {% block content %}
```

#### html2text {}

```diff
@@ -1,9 +1,10 @@
 {% extends 'punkweb_bb/base.html' %} {% load static %} {% block title_prefix
-%}Login | {% endblock%} {% block extra_head %}
+%}Login | {% endblock%} {% block og_title_prefix %}Login | {% endblock %} {%
+block extra_head %}
 {% endblock %} {% block content %}
     * _H_o_m_e
     * Login
 Login
 {% csrf_token %} {% for field in form %}
 {{ field.label }} {{ field }}
 {% endfor %} {% if form.non_field_errors %} {{ form.non_field_errors }} {%
```

### Comparing `punkweb_bb-0.2.0/punkweb_bb/templates/punkweb_bb/members.html` & `punkweb_bb-0.2.1/punkweb_bb/templates/punkweb_bb/members.html`

 * *Files 7% similar despite different names*

```diff
@@ -1,11 +1,12 @@
 {% extends "punkweb_bb/base.html" %}
 {% load static %}
 
 {% block title_prefix %}Members | {% endblock%}
+{% block og_title_prefix %}Members | {% endblock %}
 
 {% block extra_head %}
 <link rel="stylesheet" href="{% static 'punkweb_bb/css/members.css' %}" />
 {% endblock %}
 
 {% block content %}
```

#### html2text {}

```diff
@@ -1,9 +1,10 @@
 {% extends "punkweb_bb/base.html" %} {% load static %} {% block title_prefix
-%}Members | {% endblock%} {% block extra_head %}
+%}Members | {% endblock%} {% block og_title_prefix %}Members | {% endblock %}
+{% block extra_head %}
 {% endblock %} {% block content %}
     * _H_o_m_e
     * Members
     * {% for user in users %}
     * {% if user.profile.image %} [{{user.profile.image.url}}]{% else %} [{%
       static 'punkweb_bb/img/default-profile-image.png' %}]{% endif %}
       _{_{_ _u_s_e_r_._u_s_e_r_n_a_m_e_ _}_}
```

### Comparing `punkweb_bb-0.2.0/punkweb_bb/templates/punkweb_bb/partials/post_update.html` & `punkweb_bb-0.2.1/punkweb_bb/templates/punkweb_bb/partials/post_update.html`

 * *Files identical despite different names*

### Comparing `punkweb_bb-0.2.0/punkweb_bb/templates/punkweb_bb/profile.html` & `punkweb_bb-0.2.1/punkweb_bb/templates/punkweb_bb/profile.html`

 * *Files 4% similar despite different names*

```diff
@@ -1,11 +1,12 @@
 {% extends 'punkweb_bb/base.html' %}
 {% load static %}
 
 {% block title_prefix %}{{ user.username }} | {% endblock%}
+{% block og_title_prefix %}{{ user.username }} | {% endblock %}
 
 {% block extra_head %}
 <link rel="stylesheet" href="{% static 'punkweb_bb/css/profile.css' %}">
 {% endblock %}
 
 {% block content %}
```

#### html2text {}

```diff
@@ -1,9 +1,10 @@
 {% extends 'punkweb_bb/base.html' %} {% load static %} {% block title_prefix %}
-{{ user.username }} | {% endblock%} {% block extra_head %}
+{{ user.username }} | {% endblock%} {% block og_title_prefix %}{{ user.username
+}} | {% endblock %} {% block extra_head %}
 {% endblock %} {% block content %}
     * _H_o_m_e
     * _M_e_m_b_e_r_s
     * {{ user.username }}
 {% if user.profile.image %} [{{user.profile.image.url}}]{% else %} [{% static
 'punkweb_bb/img/default-profile-image.png' %}]{% endif %}
 {{user.username}}
```

### Comparing `punkweb_bb-0.2.0/punkweb_bb/templates/punkweb_bb/settings.html` & `punkweb_bb-0.2.1/punkweb_bb/templates/punkweb_bb/settings.html`

 * *Files 2% similar despite different names*

```diff
@@ -1,11 +1,12 @@
 {% extends 'punkweb_bb/base.html' %}
 {% load static %}
 
 {% block title_prefix %}Settings | {% endblock %}
+{% block og_title_prefix %}Settings | {% endblock %}
 
 {% block extra_head %}
 {{form.media.css}}
 <link rel="stylesheet" href="{% static 'punkweb_bb/css/settings.css' %}" />
 {% endblock %}
 
 {% block content %}
```

#### html2text {}

```diff
@@ -1,9 +1,10 @@
 {% extends 'punkweb_bb/base.html' %} {% load static %} {% block title_prefix
-%}Settings | {% endblock %} {% block extra_head %} {{form.media.css}}
+%}Settings | {% endblock %} {% block og_title_prefix %}Settings | {% endblock
+%} {% block extra_head %} {{form.media.css}}
 {% endblock %} {% block content %}
     * _H_o_m_e
     * Settings
 Settings
 {% csrf_token %} {% for field in form %} {% if field.name == "image" %}
 {{ field.label }} {% if field.value %} [{{ field.label }}]??Remove {% endif %}
 [File]
```

### Comparing `punkweb_bb-0.2.0/punkweb_bb/templates/punkweb_bb/shoutbox/shout_list.html` & `punkweb_bb-0.2.1/punkweb_bb/templates/punkweb_bb/shoutbox/shout_list.html`

 * *Files 9% similar despite different names*

```diff
@@ -5,15 +5,19 @@
   <div class="shoutbox__shout__content">
     <span>{{shout.created_at|date:'g:i A'}}</span>
     <span><a href="{% url 'punkweb_bb:profile' shout.user.id %}">{{shout.user.username}}</a>: </span>
     <span>{{ shout.content | safe | shoutbox_bbcode }}</span>
   </div>
   {% if shout|can_delete:request.user %}
   <div class="shoutbox__shout__actions">
-    <button class="pw-icon-button danger xs" hx-get="{% url 'punkweb_bb:shout_delete' shout.id %}"
-      hx-target="#modal-portal">
-      <span class="material-symbols-outlined">close</span>
+    <button
+      class="pw-icon-button default danger sm"
+      title="Delete"
+      hx-get="{% url 'punkweb_bb:shout_delete' shout.id %}"
+      hx-target="#modal-portal"
+    >
+      <span class="material-symbols-outlined">delete</span>
     </button>
   </div>
   {% endif %}
 </div>
 {% endfor %}
```

#### html2text {}

```diff
@@ -1,7 +1,7 @@
 {% load shoutbox_bbcode can_delete %} {% for shout in shouts %}
 {{shout.created_at|date:'g:i A'}} _{_{_s_h_o_u_t_._u_s_e_r_._u_s_e_r_n_a_m_e_}_}: {{ shout.content |
 safe | shoutbox_bbcode }}
 {% if shout|can_delete:request.user %}
-close
+delete
 {% endif %}
 {% endfor %}
```

### Comparing `punkweb_bb-0.2.0/punkweb_bb/templates/punkweb_bb/shoutbox/shoutbox.html` & `punkweb_bb-0.2.1/punkweb_bb/templates/punkweb_bb/shoutbox/shoutbox.html`

 * *Files identical despite different names*

### Comparing `punkweb_bb-0.2.0/punkweb_bb/templates/punkweb_bb/signup.html` & `punkweb_bb-0.2.1/punkweb_bb/templates/punkweb_bb/signup.html`

 * *Files 4% similar despite different names*

```diff
@@ -1,11 +1,12 @@
 {% extends 'punkweb_bb/base.html' %}
 {% load static %}
 
 {% block title_prefix %}Sign Up | {% endblock%}
+{% block og_title_prefix %}Sign Up | {% endblock %}
 
 {% block extra_head %}
 <link rel="stylesheet" href="{% static 'punkweb_bb/css/login.css' %}" />
 {% endblock %}
 
 {% block content %}
```

#### html2text {}

```diff
@@ -1,9 +1,10 @@
 {% extends 'punkweb_bb/base.html' %} {% load static %} {% block title_prefix
-%}Sign Up | {% endblock%} {% block extra_head %}
+%}Sign Up | {% endblock%} {% block og_title_prefix %}Sign Up | {% endblock %}
+{% block extra_head %}
 {% endblock %} {% block content %}
     * _H_o_m_e
     * Sign Up
 Sign Up
 {% csrf_token %} {% for field in form %}
 {{ field.label }} {{ field }}
 {% if field.errors %} {{ field.errors }} {% endif %} {% endfor %} {% if
```

### Comparing `punkweb_bb-0.2.0/punkweb_bb/templates/punkweb_bb/subcategory.html` & `punkweb_bb-0.2.1/punkweb_bb/templates/punkweb_bb/subcategory.html`

 * *Files 4% similar despite different names*

```diff
@@ -1,11 +1,12 @@
 {% extends 'punkweb_bb/base.html' %}
 {% load static humanize_int can_post %}
 
 {% block title_prefix %}{{subcategory.name}} | {% endblock%}
+{% block og_title_prefix %}{{subcategory.name}} | {% endblock %}
 
 {% block extra_head %}
 <link rel="stylesheet" href="{% static 'punkweb_bb/css/subcategory.css' %}" />
 {% endblock %}
 
 {% block content %}
 
@@ -25,21 +26,30 @@
 
 <div class="subcategory__header">
   <div class="subcategory__header__name">
     <h1>{{subcategory.name}}</h1>
     {% if perms.punkweb_bb.change_subcategory or perms.punkweb_bb.delete_subcategory %}
     <div class="subcategory__header__actions">
       {% if perms.punkweb_bb.change_subcategory %}
-      <a class="pw-button ghost xs" href="{% url 'punkweb_bb:subcategory_update' subcategory.slug %}">
-        Edit
+      <a
+        class="pw-icon-button default rounded"
+        href="{% url 'punkweb_bb:subcategory_update' subcategory.slug %}"
+        title="Edit subcategory"
+      >
+        <span class="material-symbols-outlined">edit</span>
       </a>
       {% endif %}
       {% if perms.punkweb_bb.delete_subcategory %}
-      <a class="pw-button ghost danger xs" hx-get="{% url 'punkweb_bb:subcategory_delete' subcategory.slug %}" hx-target="#modal-portal">
-        Delete
+      <a
+        class="pw-icon-button default rounded danger"
+        title="Delete subcategory"
+        hx-get="{% url 'punkweb_bb:subcategory_delete' subcategory.slug %}"
+        hx-target="#modal-portal"
+      >
+        <span class="material-symbols-outlined">delete</span>
       </a>
       {% endif %}
     </div>
     {% endif %}
   </div>
 
   {% if subcategory|can_post:request.user %}
```

#### html2text {}

```diff
@@ -1,19 +1,19 @@
 {% extends 'punkweb_bb/base.html' %} {% load static humanize_int can_post %} {%
-block title_prefix %}{{subcategory.name}} | {% endblock%} {% block extra_head
-%}
+block title_prefix %}{{subcategory.name}} | {% endblock%} {% block
+og_title_prefix %}{{subcategory.name}} | {% endblock %} {% block extra_head %}
 {% endblock %} {% block content %}
     * _H_o_m_e
     * _{_{_s_u_b_c_a_t_e_g_o_r_y_._c_a_t_e_g_o_r_y_._n_a_m_e_}_}
     * {{subcategory.name}}
 ************ {{{{ssuubbccaatteeggoorryy..nnaammee}}}} ************
 {% if perms.punkweb_bb.change_subcategory or
 perms.punkweb_bb.delete_subcategory %}
-{% if perms.punkweb_bb.change_subcategory %} _E_d_i_t_ {% endif %} {% if
-perms.punkweb_bb.delete_subcategory %} Delete {% endif %}
+{% if perms.punkweb_bb.change_subcategory %} _e_d_i_t_ {% endif %} {% if
+perms.punkweb_bb.delete_subcategory %} delete {% endif %}
 {% endif %}
 {% if subcategory|can_post:request.user %} _C_r_e_a_t_e_ _T_h_r_e_a_d {% else %} Create
 Thread {% endif %}
 TTiittllee                    PPoossttss                VViieewwss
 _{_{_t_h_r_e_a_d_._t_i_t_l_e_}_} {% if                                           {% if thread.latest_post %}
 thread.is_pinned %} keep                                         _{_{_t_h_r_e_a_d_._l_a_t_e_s_t___p_o_s_t_._c_r_e_a_t_e_d___a_t_|_d_a_t_e_:_'_M_ _j_,
 {% endif %} {% if                                                _Y_'_}_}
```

### Comparing `punkweb_bb-0.2.0/punkweb_bb/templates/punkweb_bb/subcategory_create.html` & `punkweb_bb-0.2.1/punkweb_bb/templates/punkweb_bb/subcategory_create.html`

 * *Files identical despite different names*

### Comparing `punkweb_bb-0.2.0/punkweb_bb/templates/punkweb_bb/subcategory_update.html` & `punkweb_bb-0.2.1/punkweb_bb/templates/punkweb_bb/subcategory_update.html`

 * *Files identical despite different names*

### Comparing `punkweb_bb-0.2.0/punkweb_bb/templates/punkweb_bb/thread.html` & `punkweb_bb-0.2.1/punkweb_bb/templates/punkweb_bb/thread.html`

 * *Files 26% similar despite different names*

```diff
@@ -1,13 +1,16 @@
 {% extends 'punkweb_bb/base.html' %}
 {% load static can_delete can_edit can_post %}
 
 {% block title_prefix %}{{thread.title}} | {% endblock %}
+{% block og_title_prefix %}{{thread.title}} | {% endblock %}
 
 {% block extra_head %}
+<meta name="description" content="{{thread.content.rendered|striptags|truncatechars:120}}" />
+<meta property="og:description" content="{{thread.content.rendered|striptags|truncatechars:120}}" />
 <link rel="stylesheet" href="{% static 'punkweb_bb/css/post-form.css' %}" />
 <link rel="stylesheet" href="{% static 'punkweb_bb/css/thread.css' %}" />
 <link rel="stylesheet" href="{% static 'punkweb_bb/css/thread-form.css' %}" />
 {{post_form.media.css}}
 {% endblock %}
 
 {% block extra_script %}
@@ -75,32 +78,70 @@
       </div>
       {% endif %}
     </div>
     <div class="thread__main">
       <div class="thread__content">
         {{thread.content.rendered}}
       </div>
-      {% if thread.user.profile.signature.rendered %}
-      <div class="thread__signature">
-        {{thread.user.profile.signature.rendered}}
-      </div>
-      {% endif %}
-      {% if thread|can_delete:request.user or thread|can_edit:request.user %}
+      {% if thread|can_delete:request.user or thread|can_edit:request.user or perms.punkweb_bb.pin_thread or perms.punkweb_bb.close_thread %}
       <div class="thread__actions">
+        {% if perms.punkweb_bb.pin_thread %}
+        <a 
+          class="pw-icon-button default rounded"
+          title="{% if thread.is_pinned %}Unpin{% else %}Pin{% endif %}"
+          hx-get="{% url 'punkweb_bb:thread_pin' thread.id %}"
+          hx-swap="none"
+        >
+          {% if thread.is_pinned %}
+          <span class="material-symbols-outlined">keep_off</span>
+          {% else %}
+          <span class="material-symbols-outlined">keep</span>
+          {% endif %}
+        </a>
+        {% endif %}
+        {% if perms.punkweb_bb.close_thread %}
+        <a
+          class="pw-icon-button default rounded"
+          title="{% if thread.is_closed %}Reopen{% else %}Close{% endif %}"
+          hx-get="{% url 'punkweb_bb:thread_close' thread.id %}"
+          hx-swap="none"
+        >
+          {% if thread.is_closed %}
+          <span class="material-symbols-outlined">lock_open</span>
+          {% else %}
+          <span class="material-symbols-outlined">lock</span>
+          {% endif %}
+        </a>
+        {% endif %}
         {% if thread|can_edit:request.user %}
-        <a class="pw-button ghost sm" href="{% url 'punkweb_bb:thread_update' thread.id %}">Edit</a>
+        <a
+          class="pw-icon-button default rounded"
+          href="{% url 'punkweb_bb:thread_update' thread.id %}"
+          title="Edit"
+        >
+          <span class="material-symbols-outlined">edit</span>
+        </a>
         {% endif %}
         {% if thread|can_delete:request.user %}
-        <a class="pw-button ghost danger sm" hx-get="{% url 'punkweb_bb:thread_delete' thread.id %}"
-          hx-target="#modal-portal">
-          Delete
+        <a
+          class="pw-icon-button default rounded danger"
+          title="Delete"
+          hx-get="{% url 'punkweb_bb:thread_delete' thread.id %}"
+          hx-target="#modal-portal"
+        >
+          <span class="material-symbols-outlined">delete</span>
         </a>
         {% endif %}
       </div>
       {% endif %}
+      {% if thread.user.profile.signature.rendered %}
+      <div class="thread__signature">
+        {{thread.user.profile.signature.rendered}}
+      </div>
+      {% endif %}
     </div>
   </div>
 </div>
 {% endif %}
 
 {% for post in posts %}
 <div id="post-{{post.id}}" class="pw-card fluid margin">
@@ -147,32 +188,43 @@
       </div>
       {% endif %}
     </div>
     <div class="thread__main">
       <div class="thread__content">
         {{post.content.rendered}}
       </div>
-      {% if post.user.profile.signature.rendered %}
-      <div class="thread__signature">
-        {{post.user.profile.signature.rendered}}
-      </div>
-      {% endif %}
       {% if post|can_delete:request.user or post|can_edit:request.user %}
       <div class="thread__actions">
         {% if post|can_edit:request.user %}
-        <a class="pw-button ghost sm" hx-get="{% url 'punkweb_bb:post_update' post.id %}" hx-target="#modal-portal">Edit</a>
+        <a
+          class="pw-icon-button default rounded"
+          title="Edit"
+          hx-get="{% url 'punkweb_bb:post_update' post.id %}"
+          hx-target="#modal-portal"
+        >
+          <span class="material-symbols-outlined">edit</span>
+        </a>
         {% endif %}
         {% if post|can_delete:request.user %}
-        <a class="pw-button ghost danger sm" hx-get="{% url 'punkweb_bb:post_delete' post.id %}"
-          hx-target="#modal-portal">
-          Delete
+        <a
+          class="pw-icon-button default rounded danger"
+          title="Delete"
+          hx-get="{% url 'punkweb_bb:post_delete' post.id %}"
+          hx-target="#modal-portal"
+        >
+          <span class="material-symbols-outlined">delete</span>
         </a>
         {% endif %}
       </div>
       {% endif %}
+      {% if post.user.profile.signature.rendered %}
+      <div class="thread__signature">
+        {{post.user.profile.signature.rendered}}
+      </div>
+      {% endif %}
     </div>
   </div>
 </div>
 {% endfor %}
 
 {% if posts.has_other_pages %}
 <nav>
```

#### html2text {}

```diff
@@ -1,10 +1,10 @@
 {% extends 'punkweb_bb/base.html' %} {% load static can_delete can_edit
 can_post %} {% block title_prefix %}{{thread.title}} | {% endblock %} {% block
-extra_head %}
+og_title_prefix %}{{thread.title}} | {% endblock %} {% block extra_head %}
 {{post_form.media.css}} {% endblock %} {% block extra_script %} {
 {post_form.media.js}} {% endblock %} {% block content %}
     * _H_o_m_e
     * _{_{_t_h_r_e_a_d_._s_u_b_c_a_t_e_g_o_r_y_._c_a_t_e_g_o_r_y_._n_a_m_e_}_}
     * _{_{_t_h_r_e_a_d_._s_u_b_c_a_t_e_g_o_r_y_._n_a_m_e_}_}
     * {{thread.title}}
 {% if posts.number == 1 %}
@@ -20,20 +20,23 @@
 {{thread.user.profile.post_count}}
 {% if thread.user.groups.all|length > 0 %}
 {% for group in thread.user.groups.all %}
 {{group.name}}
 {% endfor %}
 {% endif %}
 {{thread.content.rendered}}
-{% if thread.user.profile.signature.rendered %}
+{% if thread|can_delete:request.user or thread|can_edit:request.user or
+perms.punkweb_bb.pin_thread or perms.punkweb_bb.close_thread %}
+{% if perms.punkweb_bb.pin_thread %} {% if thread.is_pinned %} keep_off {% else
+%} keep {% endif %} {% endif %} {% if perms.punkweb_bb.close_thread %} {% if
+thread.is_closed %} lock_open {% else %} lock {% endif %} {% endif %} {% if
+thread|can_edit:request.user %} _e_d_i_t_ {% endif %} {% if thread|can_delete:
+request.user %} delete {% endif %}
+{% endif %} {% if thread.user.profile.signature.rendered %}
 {{thread.user.profile.signature.rendered}}
-{% endif %} {% if thread|can_delete:request.user or thread|can_edit:
-request.user %}
-{% if thread|can_edit:request.user %} _E_d_i_t {% endif %} {% if thread|can_delete:
-request.user %} Delete {% endif %}
 {% endif %}
 {% endif %} {% for post in posts %}
 {{post.created_at|date:'M d, Y'}}
 _#_{_{_p_o_s_t_._i_n_d_e_x_}_}
 {% if post.user.profile.image %}
 [{{post.user.username}}]
 {% else %}
@@ -47,19 +50,19 @@
 {{post.user.profile.post_count}}
 {% if post.user.groups.all|length > 0 %}
 {% for group in post.user.groups.all %}
 {{group.name}}
 {% endfor %}
 {% endif %}
 {{post.content.rendered}}
-{% if post.user.profile.signature.rendered %}
+{% if post|can_delete:request.user or post|can_edit:request.user %}
+{% if post|can_edit:request.user %} edit {% endif %} {% if post|can_delete:
+request.user %} delete {% endif %}
+{% endif %} {% if post.user.profile.signature.rendered %}
 {{post.user.profile.signature.rendered}}
-{% endif %} {% if post|can_delete:request.user or post|can_edit:request.user %}
-{% if post|can_edit:request.user %} Edit {% endif %} {% if post|can_delete:
-request.user %} Delete {% endif %}
 {% endif %}
 {% endfor %} {% if posts.has_other_pages %}
     * {% if posts.has_previous %}
     * _P_r_e_v
     * {% else %}
     * _P_r_e_v
     * {% endif %} {% for i in posts.paginator.page_range %} {% if posts.number
```

### Comparing `punkweb_bb-0.2.0/punkweb_bb/templates/punkweb_bb/thread_create.html` & `punkweb_bb-0.2.1/punkweb_bb/templates/punkweb_bb/thread_create.html`

 * *Files 2% similar despite different names*

```diff
@@ -1,11 +1,12 @@
 {% extends 'punkweb_bb/base.html' %}
 {% load static %}
 
 {% block title_prefix %}Create Thread | {% endblock %}
+{% block og_title_prefix %}Create Thread | {% endblock %}
 
 {% block extra_head %}
 {{form.media.css}}
 <link rel="stylesheet" href="{% static 'punkweb_bb/css/thread-form.css' %}" />
 {% endblock %}
 
 {% block content %}
```

#### html2text {}

```diff
@@ -1,9 +1,10 @@
 {% extends 'punkweb_bb/base.html' %} {% load static %} {% block title_prefix
-%}Create Thread | {% endblock %} {% block extra_head %} {{form.media.css}}
+%}Create Thread | {% endblock %} {% block og_title_prefix %}Create Thread | {%
+endblock %} {% block extra_head %} {{form.media.css}}
 {% endblock %} {% block content %}
     * _H_o_m_e
     * _{_{_s_u_b_c_a_t_e_g_o_r_y_._c_a_t_e_g_o_r_y_._n_a_m_e_}_}
     * _{_{_s_u_b_c_a_t_e_g_o_r_y_._n_a_m_e_}_}
     * Create Thread
 Create Thread
 {% csrf_token %} {% for field in form %}
```

### Comparing `punkweb_bb-0.2.0/punkweb_bb/templates/punkweb_bb/thread_update.html` & `punkweb_bb-0.2.1/punkweb_bb/templates/punkweb_bb/thread_update.html`

 * *Files identical despite different names*

### Comparing `punkweb_bb-0.2.0/punkweb_bb/templatetags/__pycache__/can_delete.cpython-311.pyc` & `punkweb_bb-0.2.1/punkweb_bb/templatetags/__pycache__/can_delete.cpython-311.pyc`

 * *Files identical despite different names*

### Comparing `punkweb_bb-0.2.0/punkweb_bb/templatetags/__pycache__/can_edit.cpython-311.pyc` & `punkweb_bb-0.2.1/punkweb_bb/templatetags/__pycache__/can_edit.cpython-311.pyc`

 * *Files identical despite different names*

### Comparing `punkweb_bb-0.2.0/punkweb_bb/templatetags/__pycache__/can_post.cpython-311.pyc` & `punkweb_bb-0.2.1/punkweb_bb/templatetags/__pycache__/can_post.cpython-311.pyc`

 * *Files identical despite different names*

### Comparing `punkweb_bb-0.2.0/punkweb_bb/templatetags/__pycache__/humanize_count.cpython-311.pyc` & `punkweb_bb-0.2.1/punkweb_bb/templatetags/__pycache__/humanize_count.cpython-311.pyc`

 * *Files identical despite different names*

### Comparing `punkweb_bb-0.2.0/punkweb_bb/templatetags/__pycache__/humanize_int.cpython-311.pyc` & `punkweb_bb-0.2.1/punkweb_bb/templatetags/__pycache__/humanize_int.cpython-311.pyc`

 * *Files identical despite different names*

### Comparing `punkweb_bb-0.2.0/punkweb_bb/templatetags/__pycache__/shoutbox_bbcode.cpython-311.pyc` & `punkweb_bb-0.2.1/punkweb_bb/templatetags/__pycache__/shoutbox_bbcode.cpython-311.pyc`

 * *Files identical despite different names*

### Comparing `punkweb_bb-0.2.0/punkweb_bb/tests.py` & `punkweb_bb-0.2.1/punkweb_bb/tests.py`

 * *Files identical despite different names*

### Comparing `punkweb_bb-0.2.0/punkweb_bb/urls.py` & `punkweb_bb-0.2.1/punkweb_bb/urls.py`

 * *Files 12% similar despite different names*

```diff
@@ -55,14 +55,16 @@
         "thread/<str:thread_id>/update/", views.thread_update_view, name="thread_update"
     ),
     path(
         "thread/<str:thread_id>/create-post/",
         views.post_create_view,
         name="post_create",
     ),
+    path("thread/<str:thread_id>/pin/", views.thread_pin_view, name="thread_pin"),
+    path("thread/<str:thread_id>/close/", views.thread_close_view, name="thread_close"),
     path("post/<str:post_id>/delete/", views.post_delete_view, name="post_delete"),
     path("post/<str:post_id>/update/", views.post_update_view, name="post_update"),
     path("shout-list/", views.shout_list_view, name="shout_list"),
     path("shout-create/", views.shout_create_view, name="shout_create"),
     path("shout/<str:shout_id>/delete/", views.shout_delete_view, name="shout_delete"),
     path("bbcode/", views.bbcode_view, name="bbcode"),
 ]
```

### Comparing `punkweb_bb-0.2.0/punkweb_bb/views.py` & `punkweb_bb-0.2.1/punkweb_bb/views.py`

 * *Files 23% similar despite different names*

```diff
@@ -403,14 +403,40 @@
         "thread": thread,
     }
 
     return render(request, "punkweb_bb/partials/thread_delete.html", context=context)
 
 
 @login_required(login_url="/login/")
+def thread_pin_view(request, thread_id):
+    thread = get_object_or_404(Thread, pk=thread_id)
+
+    if not request.user.has_perm("punkweb_bb.pin_thread"):
+        return HttpResponseForbidden("You do not have permission to pin threads.")
+
+    thread.is_pinned = not thread.is_pinned
+    thread.save()
+
+    return htmx_redirect(thread.get_absolute_url())
+
+
+@login_required(login_url="/login/")
+def thread_close_view(request, thread_id):
+    thread = get_object_or_404(Thread, pk=thread_id)
+
+    if not request.user.has_perm("punkweb_bb.close_thread"):
+        return HttpResponseForbidden("You do not have permission to close threads.")
+
+    thread.is_closed = not thread.is_closed
+    thread.save()
+
+    return htmx_redirect(thread.get_absolute_url())
+
+
+@login_required(login_url="/login/")
 def post_create_view(request, thread_id):
     thread = get_object_or_404(Thread, pk=thread_id)
 
     if not thread.can_post(request.user):
         return HttpResponseForbidden(
             "You do not have permission to post in this thread."
         )
```

### Comparing `punkweb_bb-0.2.0/punkweb_bb/widgets.py` & `punkweb_bb-0.2.1/punkweb_bb/widgets.py`

 * *Files identical despite different names*

### Comparing `punkweb_bb-0.2.0/punkweb_bb.egg-info/PKG-INFO` & `punkweb_bb-0.2.1/punkweb_bb.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: punkweb-bb
-Version: 0.2.0
+Version: 0.2.1
 Summary: Django application that provides a simple and modern forum board software for your Django website.
 Home-page: https://github.com/Punkweb/PunkwebBB
 Author: Punkweb
 Author-email: punkwebnet@gmail.com
 License: BSD-3-Clause
 Classifier: Environment :: Web Environment
 Classifier: Framework :: Django
```

### Comparing `punkweb_bb-0.2.0/punkweb_bb.egg-info/SOURCES.txt` & `punkweb_bb-0.2.1/punkweb_bb.egg-info/SOURCES.txt`

 * *Files 1% similar despite different names*

```diff
@@ -48,17 +48,19 @@
 punkweb_bb/__pycache__/tests.cpython-311.pyc
 punkweb_bb/__pycache__/urls.cpython-311.pyc
 punkweb_bb/__pycache__/utils.cpython-311.pyc
 punkweb_bb/__pycache__/views.cpython-311.pyc
 punkweb_bb/__pycache__/widgets.cpython-311.pyc
 punkweb_bb/migrations/0001_initial.py
 punkweb_bb/migrations/0002_thread_view_count.py
+punkweb_bb/migrations/0003_alter_thread_options.py
 punkweb_bb/migrations/__init__.py
 punkweb_bb/migrations/__pycache__/0001_initial.cpython-311.pyc
 punkweb_bb/migrations/__pycache__/0002_thread_view_count.cpython-311.pyc
+punkweb_bb/migrations/__pycache__/0003_alter_thread_options.cpython-311.pyc
 punkweb_bb/migrations/__pycache__/__init__.cpython-311.pyc
 punkweb_bb/static/punkweb_bb/favicon.ico
 punkweb_bb/static/punkweb_bb/css/category-form.css
 punkweb_bb/static/punkweb_bb/css/defaults.css
 punkweb_bb/static/punkweb_bb/css/index.css
 punkweb_bb/static/punkweb_bb/css/login.css
 punkweb_bb/static/punkweb_bb/css/members.css
```

### Comparing `punkweb_bb-0.2.0/setup.py` & `punkweb_bb-0.2.1/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from setuptools import setup
 
 setup(
     name="punkweb_bb",
-    version="0.2.0",
+    version="0.2.1",
     author="Punkweb",
     author_email="punkwebnet@gmail.com",
     packages=["punkweb_bb"],
     url="https://github.com/Punkweb/PunkwebBB",
     license="BSD-3-Clause",
     description="Django application that provides a simple and modern forum board software for your Django website.",
     long_description=open("README.md").read(),
```

