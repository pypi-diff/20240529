# Comparing `tmp/libcoveweb-0.30.2.tar.gz` & `tmp/libcoveweb-0.30.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "libcoveweb-0.30.2.tar", last modified: Tue Jan 30 15:39:56 2024, max compression
+gzip compressed data, was "libcoveweb-0.30.3.tar", last modified: Wed May 29 21:51:26 2024, max compression
```

## Comparing `libcoveweb-0.30.2.tar` & `libcoveweb-0.30.3.tar`

### file list

```diff
@@ -1,200 +1,201 @@
-drwxr-xr-x   0 odscjames  (1000) odscjames  (1000)        0 2024-01-30 15:39:56.178465 libcoveweb-0.30.2/
--rw-r--r--   0 odscjames  (1000) odscjames  (1000)      395 2024-01-30 15:39:56.178465 libcoveweb-0.30.2/PKG-INFO
--rw-r--r--   0 odscjames  (1000) odscjames  (1000)     3492 2024-01-30 15:33:17.000000 libcoveweb-0.30.2/README.md
-drwxr-xr-x   0 odscjames  (1000) odscjames  (1000)        0 2024-01-30 15:39:56.150464 libcoveweb-0.30.2/cove/
--rw-r--r--   0 odscjames  (1000) odscjames  (1000)        0 2023-08-16 07:10:06.000000 libcoveweb-0.30.2/cove/__init__.py
--rw-r--r--   0 odscjames  (1000) odscjames  (1000)      544 2023-08-16 07:10:06.000000 libcoveweb-0.30.2/cove/context_processors.py
-drwxr-xr-x   0 odscjames  (1000) odscjames  (1000)        0 2024-01-30 15:39:56.150464 libcoveweb-0.30.2/cove/fixtures/
--rw-r--r--   0 odscjames  (1000) odscjames  (1000)        0 2023-08-16 07:10:06.000000 libcoveweb-0.30.2/cove/fixtures/bad.xlsx
--rw-r--r--   0 odscjames  (1000) odscjames  (1000)    25816 2023-08-16 07:10:06.000000 libcoveweb-0.30.2/cove/fixtures/badfile.json
--rw-r--r--   0 odscjames  (1000) odscjames  (1000)     5771 2023-08-16 07:10:06.000000 libcoveweb-0.30.2/cove/fixtures/basic.xlsx
--rw-r--r--   0 odscjames  (1000) odscjames  (1000)       65 2023-08-16 07:10:06.000000 libcoveweb-0.30.2/cove/fixtures/utf8.json
--rw-r--r--   0 odscjames  (1000) odscjames  (1000)     9398 2023-10-20 15:24:41.000000 libcoveweb-0.30.2/cove/html_error_msg.py
-drwxr-xr-x   0 odscjames  (1000) odscjames  (1000)        0 2024-01-30 15:39:56.150464 libcoveweb-0.30.2/cove/input/
--rw-r--r--   0 odscjames  (1000) odscjames  (1000)        0 2023-08-16 07:10:06.000000 libcoveweb-0.30.2/cove/input/__init__.py
-drwxr-xr-x   0 odscjames  (1000) odscjames  (1000)        0 2024-01-30 15:39:56.150464 libcoveweb-0.30.2/cove/input/migrations/
--rw-r--r--   0 odscjames  (1000) odscjames  (1000)      565 2023-08-16 07:10:06.000000 libcoveweb-0.30.2/cove/input/migrations/0001_initial.py
--rw-r--r--   0 odscjames  (1000) odscjames  (1000)      455 2023-08-16 07:10:06.000000 libcoveweb-0.30.2/cove/input/migrations/0002_supplieddata_current_app.py
--rw-r--r--   0 odscjames  (1000) odscjames  (1000)      893 2023-08-16 07:10:06.000000 libcoveweb-0.30.2/cove/input/migrations/0003_auto_20150506_1649.py
--rw-r--r--   0 odscjames  (1000) odscjames  (1000)      462 2023-08-16 07:10:06.000000 libcoveweb-0.30.2/cove/input/migrations/0004_auto_20150908_1533.py
--rw-r--r--   0 odscjames  (1000) odscjames  (1000)      422 2023-08-16 07:10:06.000000 libcoveweb-0.30.2/cove/input/migrations/0005_auto_20160104_1208.py
--rw-r--r--   0 odscjames  (1000) odscjames  (1000)      444 2023-08-16 07:10:06.000000 libcoveweb-0.30.2/cove/input/migrations/0006_supplieddata_rendered.py
--rw-r--r--   0 odscjames  (1000) odscjames  (1000)      591 2023-08-16 07:10:06.000000 libcoveweb-0.30.2/cove/input/migrations/0007_supplied_data_schema_version.py
--rw-r--r--   0 odscjames  (1000) odscjames  (1000)      488 2023-08-16 07:10:06.000000 libcoveweb-0.30.2/cove/input/migrations/0008_supplieddata_data_schema_version.py
--rw-r--r--   0 odscjames  (1000) odscjames  (1000)      415 2023-08-16 07:10:06.000000 libcoveweb-0.30.2/cove/input/migrations/0009_supplieddata_parameters.py
--rw-r--r--   0 odscjames  (1000) odscjames  (1000)      468 2023-08-16 07:10:06.000000 libcoveweb-0.30.2/cove/input/migrations/0010_alter_supplieddata_original_file.py
--rw-r--r--   0 odscjames  (1000) odscjames  (1000)        0 2023-08-16 07:10:06.000000 libcoveweb-0.30.2/cove/input/migrations/__init__.py
--rw-r--r--   0 odscjames  (1000) odscjames  (1000)     3863 2023-08-16 07:10:06.000000 libcoveweb-0.30.2/cove/input/models.py
--rw-r--r--   0 odscjames  (1000) odscjames  (1000)     3913 2024-01-30 15:29:06.000000 libcoveweb-0.30.2/cove/input/views.py
-drwxr-xr-x   0 odscjames  (1000) odscjames  (1000)        0 2024-01-30 15:39:56.150464 libcoveweb-0.30.2/cove/lib/
--rw-r--r--   0 odscjames  (1000) odscjames  (1000)        0 2023-08-16 07:10:06.000000 libcoveweb-0.30.2/cove/lib/__init__.py
--rw-r--r--   0 odscjames  (1000) odscjames  (1000)     1992 2023-08-16 07:10:06.000000 libcoveweb-0.30.2/cove/lib/common.py
-drwxr-xr-x   0 odscjames  (1000) odscjames  (1000)        0 2024-01-30 15:39:56.146464 libcoveweb-0.30.2/cove/locale/
-drwxr-xr-x   0 odscjames  (1000) odscjames  (1000)        0 2024-01-30 15:39:56.146464 libcoveweb-0.30.2/cove/locale/en/
-drwxr-xr-x   0 odscjames  (1000) odscjames  (1000)        0 2024-01-30 15:39:56.150464 libcoveweb-0.30.2/cove/locale/en/LC_MESSAGES/
--rw-r--r--   0 odscjames  (1000) odscjames  (1000)      337 2023-08-16 07:10:06.000000 libcoveweb-0.30.2/cove/locale/en/LC_MESSAGES/django.mo
--rw-r--r--   0 odscjames  (1000) odscjames  (1000)    13391 2023-08-16 07:10:06.000000 libcoveweb-0.30.2/cove/locale/en/LC_MESSAGES/django.po
-drwxr-xr-x   0 odscjames  (1000) odscjames  (1000)        0 2024-01-30 15:39:56.146464 libcoveweb-0.30.2/cove/locale/es/
-drwxr-xr-x   0 odscjames  (1000) odscjames  (1000)        0 2024-01-30 15:39:56.154464 libcoveweb-0.30.2/cove/locale/es/LC_MESSAGES/
--rw-r--r--   0 odscjames  (1000) odscjames  (1000)    13345 2023-12-05 14:55:03.000000 libcoveweb-0.30.2/cove/locale/es/LC_MESSAGES/django.mo
--rw-r--r--   0 odscjames  (1000) odscjames  (1000)    19517 2023-12-05 14:55:03.000000 libcoveweb-0.30.2/cove/locale/es/LC_MESSAGES/django.po
-drwxr-xr-x   0 odscjames  (1000) odscjames  (1000)        0 2024-01-30 15:39:56.154464 libcoveweb-0.30.2/cove/management/
--rw-r--r--   0 odscjames  (1000) odscjames  (1000)        0 2023-08-16 07:10:06.000000 libcoveweb-0.30.2/cove/management/__init__.py
-drwxr-xr-x   0 odscjames  (1000) odscjames  (1000)        0 2024-01-30 15:39:56.154464 libcoveweb-0.30.2/cove/management/commands/
--rw-r--r--   0 odscjames  (1000) odscjames  (1000)        0 2023-08-16 07:10:06.000000 libcoveweb-0.30.2/cove/management/commands/__init__.py
--rw-r--r--   0 odscjames  (1000) odscjames  (1000)     1594 2023-08-16 07:10:06.000000 libcoveweb-0.30.2/cove/management/commands/base_command.py
--rw-r--r--   0 odscjames  (1000) odscjames  (1000)      649 2023-08-16 07:10:06.000000 libcoveweb-0.30.2/cove/management/commands/expire_files.py
--rw-r--r--   0 odscjames  (1000) odscjames  (1000)     1370 2023-08-16 07:10:06.000000 libcoveweb-0.30.2/cove/management/commands/tests.py
--rw-r--r--   0 odscjames  (1000) odscjames  (1000)      592 2023-08-16 07:10:06.000000 libcoveweb-0.30.2/cove/management/commands/upload.py
--rw-r--r--   0 odscjames  (1000) odscjames  (1000)      354 2023-08-16 07:10:06.000000 libcoveweb-0.30.2/cove/middleware.py
-drwxr-xr-x   0 odscjames  (1000) odscjames  (1000)        0 2024-01-30 15:39:56.146464 libcoveweb-0.30.2/cove/sass/
-drwxr-xr-x   0 odscjames  (1000) odscjames  (1000)        0 2024-01-30 15:39:56.154464 libcoveweb-0.30.2/cove/sass/bootstrap/
--rw-r--r--   0 odscjames  (1000) odscjames  (1000)      178 2023-08-16 07:10:06.000000 libcoveweb-0.30.2/cove/sass/bootstrap/_bootstrap-compass.scss
--rw-r--r--   0 odscjames  (1000) odscjames  (1000)      757 2023-08-16 07:10:06.000000 libcoveweb-0.30.2/cove/sass/bootstrap/_bootstrap-mincer.scss
--rw-r--r--   0 odscjames  (1000) odscjames  (1000)      168 2023-08-16 07:10:06.000000 libcoveweb-0.30.2/cove/sass/bootstrap/_bootstrap-sprockets.scss
--rw-r--r--   0 odscjames  (1000) odscjames  (1000)     1486 2023-08-16 07:10:06.000000 libcoveweb-0.30.2/cove/sass/bootstrap/_bootstrap.scss
-drwxr-xr-x   0 odscjames  (1000) odscjames  (1000)        0 2024-01-30 15:39:56.162464 libcoveweb-0.30.2/cove/sass/bootstrap/bootstrap/
--rw-r--r--   0 odscjames  (1000) odscjames  (1000)     1550 2023-08-16 07:10:06.000000 libcoveweb-0.30.2/cove/sass/bootstrap/bootstrap/_alerts.scss
--rw-r--r--   0 odscjames  (1000) odscjames  (1000)     1228 2023-08-16 07:10:06.000000 libcoveweb-0.30.2/cove/sass/bootstrap/bootstrap/_badges.scss
--rw-r--r--   0 odscjames  (1000) odscjames  (1000)      700 2023-08-16 07:10:06.000000 libcoveweb-0.30.2/cove/sass/bootstrap/bootstrap/_breadcrumbs.scss
--rw-r--r--   0 odscjames  (1000) odscjames  (1000)     5758 2023-08-16 07:10:06.000000 libcoveweb-0.30.2/cove/sass/bootstrap/bootstrap/_button-groups.scss
--rw-r--r--   0 odscjames  (1000) odscjames  (1000)     3819 2023-08-16 07:10:06.000000 libcoveweb-0.30.2/cove/sass/bootstrap/bootstrap/_buttons.scss
--rw-r--r--   0 odscjames  (1000) odscjames  (1000)     5725 2023-08-16 07:10:06.000000 libcoveweb-0.30.2/cove/sass/bootstrap/bootstrap/_carousel.scss
--rw-r--r--   0 odscjames  (1000) odscjames  (1000)      815 2023-08-16 07:10:06.000000 libcoveweb-0.30.2/cove/sass/bootstrap/bootstrap/_close.scss
--rw-r--r--   0 odscjames  (1000) odscjames  (1000)     1401 2023-08-16 07:10:06.000000 libcoveweb-0.30.2/cove/sass/bootstrap/bootstrap/_code.scss
--rw-r--r--   0 odscjames  (1000) odscjames  (1000)      819 2023-08-16 07:10:06.000000 libcoveweb-0.30.2/cove/sass/bootstrap/bootstrap/_component-animations.scss
--rw-r--r--   0 odscjames  (1000) odscjames  (1000)     4889 2023-08-16 07:10:06.000000 libcoveweb-0.30.2/cove/sass/bootstrap/bootstrap/_dropdowns.scss
--rw-r--r--   0 odscjames  (1000) odscjames  (1000)    16162 2023-08-16 07:10:06.000000 libcoveweb-0.30.2/cove/sass/bootstrap/bootstrap/_forms.scss
--rw-r--r--   0 odscjames  (1000) odscjames  (1000)    20448 2023-08-16 07:10:06.000000 libcoveweb-0.30.2/cove/sass/bootstrap/bootstrap/_glyphicons.scss
--rw-r--r--   0 odscjames  (1000) odscjames  (1000)     1443 2023-08-16 07:10:06.000000 libcoveweb-0.30.2/cove/sass/bootstrap/bootstrap/_grid.scss
--rw-r--r--   0 odscjames  (1000) odscjames  (1000)     4313 2023-08-16 07:10:06.000000 libcoveweb-0.30.2/cove/sass/bootstrap/bootstrap/_input-groups.scss
--rw-r--r--   0 odscjames  (1000) odscjames  (1000)     1152 2023-08-16 07:10:06.000000 libcoveweb-0.30.2/cove/sass/bootstrap/bootstrap/_jumbotron.scss
--rw-r--r--   0 odscjames  (1000) odscjames  (1000)     1156 2023-08-16 07:10:06.000000 libcoveweb-0.30.2/cove/sass/bootstrap/bootstrap/_labels.scss
--rw-r--r--   0 odscjames  (1000) odscjames  (1000)     3172 2023-08-16 07:10:06.000000 libcoveweb-0.30.2/cove/sass/bootstrap/bootstrap/_list-group.scss
--rw-r--r--   0 odscjames  (1000) odscjames  (1000)      900 2023-08-16 07:10:06.000000 libcoveweb-0.30.2/cove/sass/bootstrap/bootstrap/_media.scss
--rw-r--r--   0 odscjames  (1000) odscjames  (1000)      986 2023-08-16 07:10:06.000000 libcoveweb-0.30.2/cove/sass/bootstrap/bootstrap/_mixins.scss
--rw-r--r--   0 odscjames  (1000) odscjames  (1000)     3568 2023-08-16 07:10:06.000000 libcoveweb-0.30.2/cove/sass/bootstrap/bootstrap/_modals.scss
--rw-r--r--   0 odscjames  (1000) odscjames  (1000)    14729 2023-08-16 07:10:06.000000 libcoveweb-0.30.2/cove/sass/bootstrap/bootstrap/_navbar.scss
--rw-r--r--   0 odscjames  (1000) odscjames  (1000)     4950 2023-08-16 07:10:06.000000 libcoveweb-0.30.2/cove/sass/bootstrap/bootstrap/_navs.scss
--rw-r--r--   0 odscjames  (1000) odscjames  (1000)     7559 2023-08-16 07:10:06.000000 libcoveweb-0.30.2/cove/sass/bootstrap/bootstrap/_normalize.scss
--rw-r--r--   0 odscjames  (1000) odscjames  (1000)      855 2023-08-16 07:10:06.000000 libcoveweb-0.30.2/cove/sass/bootstrap/bootstrap/_pager.scss
--rw-r--r--   0 odscjames  (1000) odscjames  (1000)     2091 2023-08-16 07:10:06.000000 libcoveweb-0.30.2/cove/sass/bootstrap/bootstrap/_pagination.scss
--rw-r--r--   0 odscjames  (1000) odscjames  (1000)     6385 2023-08-16 07:10:06.000000 libcoveweb-0.30.2/cove/sass/bootstrap/bootstrap/_panels.scss
--rw-r--r--   0 odscjames  (1000) odscjames  (1000)     3502 2023-08-16 07:10:06.000000 libcoveweb-0.30.2/cove/sass/bootstrap/bootstrap/_popovers.scss
--rw-r--r--   0 odscjames  (1000) odscjames  (1000)     1939 2023-08-16 07:10:06.000000 libcoveweb-0.30.2/cove/sass/bootstrap/bootstrap/_print.scss
--rw-r--r--   0 odscjames  (1000) odscjames  (1000)     1992 2023-08-16 07:10:06.000000 libcoveweb-0.30.2/cove/sass/bootstrap/bootstrap/_progress-bars.scss
--rw-r--r--   0 odscjames  (1000) odscjames  (1000)      546 2023-08-16 07:10:06.000000 libcoveweb-0.30.2/cove/sass/bootstrap/bootstrap/_responsive-embed.scss
--rw-r--r--   0 odscjames  (1000) odscjames  (1000)     4409 2023-08-16 07:10:06.000000 libcoveweb-0.30.2/cove/sass/bootstrap/bootstrap/_responsive-utilities.scss
--rw-r--r--   0 odscjames  (1000) odscjames  (1000)     3031 2023-08-16 07:10:06.000000 libcoveweb-0.30.2/cove/sass/bootstrap/bootstrap/_scaffolding.scss
--rw-r--r--   0 odscjames  (1000) odscjames  (1000)     4662 2023-08-16 07:10:06.000000 libcoveweb-0.30.2/cove/sass/bootstrap/bootstrap/_tables.scss
--rw-r--r--   0 odscjames  (1000) odscjames  (1000)     8558 2023-08-16 07:10:06.000000 libcoveweb-0.30.2/cove/sass/bootstrap/bootstrap/_theme.scss
--rw-r--r--   0 odscjames  (1000) odscjames  (1000)      892 2023-08-16 07:10:06.000000 libcoveweb-0.30.2/cove/sass/bootstrap/bootstrap/_thumbnails.scss
--rw-r--r--   0 odscjames  (1000) odscjames  (1000)     3007 2023-08-16 07:10:06.000000 libcoveweb-0.30.2/cove/sass/bootstrap/bootstrap/_tooltip.scss
--rw-r--r--   0 odscjames  (1000) odscjames  (1000)     6149 2023-08-16 07:10:06.000000 libcoveweb-0.30.2/cove/sass/bootstrap/bootstrap/_type.scss
--rw-r--r--   0 odscjames  (1000) odscjames  (1000)      765 2023-08-16 07:10:06.000000 libcoveweb-0.30.2/cove/sass/bootstrap/bootstrap/_utilities.scss
--rw-r--r--   0 odscjames  (1000) odscjames  (1000)    31290 2023-08-16 07:10:06.000000 libcoveweb-0.30.2/cove/sass/bootstrap/bootstrap/_variables.scss
--rw-r--r--   0 odscjames  (1000) odscjames  (1000)      535 2023-08-16 07:10:06.000000 libcoveweb-0.30.2/cove/sass/bootstrap/bootstrap/_wells.scss
-drwxr-xr-x   0 odscjames  (1000) odscjames  (1000)        0 2024-01-30 15:39:56.166464 libcoveweb-0.30.2/cove/sass/bootstrap/bootstrap/mixins/
--rw-r--r--   0 odscjames  (1000) odscjames  (1000)      263 2023-08-16 07:10:06.000000 libcoveweb-0.30.2/cove/sass/bootstrap/bootstrap/mixins/_alerts.scss
--rw-r--r--   0 odscjames  (1000) odscjames  (1000)      233 2023-08-16 07:10:06.000000 libcoveweb-0.30.2/cove/sass/bootstrap/bootstrap/mixins/_background-variant.scss
--rw-r--r--   0 odscjames  (1000) odscjames  (1000)      492 2023-08-16 07:10:06.000000 libcoveweb-0.30.2/cove/sass/bootstrap/bootstrap/mixins/_border-radius.scss
--rw-r--r--   0 odscjames  (1000) odscjames  (1000)     1453 2023-08-16 07:10:06.000000 libcoveweb-0.30.2/cove/sass/bootstrap/bootstrap/mixins/_buttons.scss
--rw-r--r--   0 odscjames  (1000) odscjames  (1000)      126 2023-08-16 07:10:06.000000 libcoveweb-0.30.2/cove/sass/bootstrap/bootstrap/mixins/_center-block.scss
--rw-r--r--   0 odscjames  (1000) odscjames  (1000)      611 2023-08-16 07:10:06.000000 libcoveweb-0.30.2/cove/sass/bootstrap/bootstrap/mixins/_clearfix.scss
--rw-r--r--   0 odscjames  (1000) odscjames  (1000)     2771 2023-08-16 07:10:06.000000 libcoveweb-0.30.2/cove/sass/bootstrap/bootstrap/mixins/_forms.scss
--rw-r--r--   0 odscjames  (1000) odscjames  (1000)     4392 2023-08-16 07:10:06.000000 libcoveweb-0.30.2/cove/sass/bootstrap/bootstrap/mixins/_gradients.scss
--rw-r--r--   0 odscjames  (1000) odscjames  (1000)     2360 2023-08-16 07:10:06.000000 libcoveweb-0.30.2/cove/sass/bootstrap/bootstrap/mixins/_grid-framework.scss
--rw-r--r--   0 odscjames  (1000) odscjames  (1000)     3216 2023-08-16 07:10:06.000000 libcoveweb-0.30.2/cove/sass/bootstrap/bootstrap/mixins/_grid.scss
--rw-r--r--   0 odscjames  (1000) odscjames  (1000)      590 2023-08-16 07:10:06.000000 libcoveweb-0.30.2/cove/sass/bootstrap/bootstrap/mixins/_hide-text.scss
--rw-r--r--   0 odscjames  (1000) odscjames  (1000)     1208 2023-08-16 07:10:06.000000 libcoveweb-0.30.2/cove/sass/bootstrap/bootstrap/mixins/_image.scss
--rw-r--r--   0 odscjames  (1000) odscjames  (1000)      167 2023-08-16 07:10:06.000000 libcoveweb-0.30.2/cove/sass/bootstrap/bootstrap/mixins/_labels.scss
--rw-r--r--   0 odscjames  (1000) odscjames  (1000)      672 2023-08-16 07:10:06.000000 libcoveweb-0.30.2/cove/sass/bootstrap/bootstrap/mixins/_list-group.scss
--rw-r--r--   0 odscjames  (1000) odscjames  (1000)      238 2023-08-16 07:10:06.000000 libcoveweb-0.30.2/cove/sass/bootstrap/bootstrap/mixins/_nav-divider.scss
--rw-r--r--   0 odscjames  (1000) odscjames  (1000)      370 2023-08-16 07:10:06.000000 libcoveweb-0.30.2/cove/sass/bootstrap/bootstrap/mixins/_nav-vertical-align.scss
--rw-r--r--   0 odscjames  (1000) odscjames  (1000)      149 2023-08-16 07:10:06.000000 libcoveweb-0.30.2/cove/sass/bootstrap/bootstrap/mixins/_opacity.scss
--rw-r--r--   0 odscjames  (1000) odscjames  (1000)      507 2023-08-16 07:10:06.000000 libcoveweb-0.30.2/cove/sass/bootstrap/bootstrap/mixins/_pagination.scss
--rw-r--r--   0 odscjames  (1000) odscjames  (1000)      543 2023-08-16 07:10:06.000000 libcoveweb-0.30.2/cove/sass/bootstrap/bootstrap/mixins/_panels.scss
--rw-r--r--   0 odscjames  (1000) odscjames  (1000)      200 2023-08-16 07:10:06.000000 libcoveweb-0.30.2/cove/sass/bootstrap/bootstrap/mixins/_progress-bar.scss
--rw-r--r--   0 odscjames  (1000) odscjames  (1000)      246 2023-08-16 07:10:06.000000 libcoveweb-0.30.2/cove/sass/bootstrap/bootstrap/mixins/_reset-filter.scss
--rw-r--r--   0 odscjames  (1000) odscjames  (1000)      476 2023-08-16 07:10:06.000000 libcoveweb-0.30.2/cove/sass/bootstrap/bootstrap/mixins/_reset-text.scss
--rw-r--r--   0 odscjames  (1000) odscjames  (1000)      202 2023-08-16 07:10:06.000000 libcoveweb-0.30.2/cove/sass/bootstrap/bootstrap/mixins/_resize.scss
--rw-r--r--   0 odscjames  (1000) odscjames  (1000)      514 2023-08-16 07:10:06.000000 libcoveweb-0.30.2/cove/sass/bootstrap/bootstrap/mixins/_responsive-visibility.scss
--rw-r--r--   0 odscjames  (1000) odscjames  (1000)      147 2023-08-16 07:10:06.000000 libcoveweb-0.30.2/cove/sass/bootstrap/bootstrap/mixins/_size.scss
--rw-r--r--   0 odscjames  (1000) odscjames  (1000)      338 2023-08-16 07:10:06.000000 libcoveweb-0.30.2/cove/sass/bootstrap/bootstrap/mixins/_tab-focus.scss
--rw-r--r--   0 odscjames  (1000) odscjames  (1000)      715 2023-08-16 07:10:06.000000 libcoveweb-0.30.2/cove/sass/bootstrap/bootstrap/mixins/_table-row.scss
--rw-r--r--   0 odscjames  (1000) odscjames  (1000)      210 2023-08-16 07:10:06.000000 libcoveweb-0.30.2/cove/sass/bootstrap/bootstrap/mixins/_text-emphasis.scss
--rw-r--r--   0 odscjames  (1000) odscjames  (1000)      168 2023-08-16 07:10:06.000000 libcoveweb-0.30.2/cove/sass/bootstrap/bootstrap/mixins/_text-overflow.scss
--rw-r--r--   0 odscjames  (1000) odscjames  (1000)     6645 2023-08-16 07:10:06.000000 libcoveweb-0.30.2/cove/sass/bootstrap/bootstrap/mixins/_vendor-prefixes.scss
--rw-r--r--   0 odscjames  (1000) odscjames  (1000)     4771 2024-01-30 15:29:06.000000 libcoveweb-0.30.2/cove/settings.py
-drwxr-xr-x   0 odscjames  (1000) odscjames  (1000)        0 2024-01-30 15:39:56.146464 libcoveweb-0.30.2/cove/static/
-drwxr-xr-x   0 odscjames  (1000) odscjames  (1000)        0 2024-01-30 15:39:56.146464 libcoveweb-0.30.2/cove/static/dataexplore/
-drwxr-xr-x   0 odscjames  (1000) odscjames  (1000)        0 2024-01-30 15:39:56.166464 libcoveweb-0.30.2/cove/static/dataexplore/css/
--rw-r--r--   0 odscjames  (1000) odscjames  (1000)     1833 2023-08-16 07:10:06.000000 libcoveweb-0.30.2/cove/static/dataexplore/css/style.css
-drwxr-xr-x   0 odscjames  (1000) odscjames  (1000)        0 2024-01-30 15:39:56.146464 libcoveweb-0.30.2/cove/static/dataexplore/fonts/
-drwxr-xr-x   0 odscjames  (1000) odscjames  (1000)        0 2024-01-30 15:39:56.170464 libcoveweb-0.30.2/cove/static/dataexplore/fonts/bootstrap/
--rw-r--r--   0 odscjames  (1000) odscjames  (1000)    20127 2023-08-16 07:10:06.000000 libcoveweb-0.30.2/cove/static/dataexplore/fonts/bootstrap/glyphicons-halflings-regular.eot
--rw-r--r--   0 odscjames  (1000) odscjames  (1000)   108738 2023-08-16 07:10:06.000000 libcoveweb-0.30.2/cove/static/dataexplore/fonts/bootstrap/glyphicons-halflings-regular.svg
--rw-r--r--   0 odscjames  (1000) odscjames  (1000)    45404 2023-08-16 07:10:06.000000 libcoveweb-0.30.2/cove/static/dataexplore/fonts/bootstrap/glyphicons-halflings-regular.ttf
--rw-r--r--   0 odscjames  (1000) odscjames  (1000)    23424 2023-08-16 07:10:06.000000 libcoveweb-0.30.2/cove/static/dataexplore/fonts/bootstrap/glyphicons-halflings-regular.woff
--rw-r--r--   0 odscjames  (1000) odscjames  (1000)    18028 2023-08-16 07:10:06.000000 libcoveweb-0.30.2/cove/static/dataexplore/fonts/bootstrap/glyphicons-halflings-regular.woff2
-drwxr-xr-x   0 odscjames  (1000) odscjames  (1000)        0 2024-01-30 15:39:56.170464 libcoveweb-0.30.2/cove/static/dataexplore/fonts/tick/
--rw-r--r--   0 odscjames  (1000) odscjames  (1000)      408 2023-08-16 07:10:06.000000 libcoveweb-0.30.2/cove/static/dataexplore/fonts/tick/tick.css
--rw-r--r--   0 odscjames  (1000) odscjames  (1000)     2328 2023-08-16 07:10:06.000000 libcoveweb-0.30.2/cove/static/dataexplore/fonts/tick/tick.eot
--rw-r--r--   0 odscjames  (1000) odscjames  (1000)     3063 2023-08-16 07:10:06.000000 libcoveweb-0.30.2/cove/static/dataexplore/fonts/tick/tick.svg
--rw-r--r--   0 odscjames  (1000) odscjames  (1000)     2168 2023-08-16 07:10:06.000000 libcoveweb-0.30.2/cove/static/dataexplore/fonts/tick/tick.ttf
--rw-r--r--   0 odscjames  (1000) odscjames  (1000)     1604 2023-08-16 07:10:06.000000 libcoveweb-0.30.2/cove/static/dataexplore/fonts/tick/tick.woff
--rw-r--r--   0 odscjames  (1000) odscjames  (1000)     1064 2023-08-16 07:10:06.000000 libcoveweb-0.30.2/cove/static/dataexplore/fonts/tick/tick.woff2
-drwxr-xr-x   0 odscjames  (1000) odscjames  (1000)        0 2024-01-30 15:39:56.178465 libcoveweb-0.30.2/cove/templates/
--rw-r--r--   0 odscjames  (1000) odscjames  (1000)     1114 2023-08-16 07:10:06.000000 libcoveweb-0.30.2/cove/templates/500.html
--rw-r--r--   0 odscjames  (1000) odscjames  (1000)      849 2023-12-01 09:23:46.000000 libcoveweb-0.30.2/cove/templates/additional_codelist_values.html
--rw-r--r--   0 odscjames  (1000) odscjames  (1000)      405 2023-08-16 07:10:06.000000 libcoveweb-0.30.2/cove/templates/additional_fields_table.html
--rw-r--r--   0 odscjames  (1000) odscjames  (1000)     2722 2023-08-16 07:10:06.000000 libcoveweb-0.30.2/cove/templates/additional_fields_table_all.html
--rw-r--r--   0 odscjames  (1000) odscjames  (1000)     4938 2023-08-16 07:10:06.000000 libcoveweb-0.30.2/cove/templates/base.html
--rw-r--r--   0 odscjames  (1000) odscjames  (1000)      748 2023-08-16 07:10:06.000000 libcoveweb-0.30.2/cove/templates/error.html
--rw-r--r--   0 odscjames  (1000) odscjames  (1000)      405 2023-08-16 07:10:06.000000 libcoveweb-0.30.2/cove/templates/error_extra.html
--rw-r--r--   0 odscjames  (1000) odscjames  (1000)     2431 2023-08-16 07:10:06.000000 libcoveweb-0.30.2/cove/templates/explore.html
--rw-r--r--   0 odscjames  (1000) odscjames  (1000)      479 2023-08-16 07:10:06.000000 libcoveweb-0.30.2/cove/templates/google_analytics.html
--rw-r--r--   0 odscjames  (1000) odscjames  (1000)     3845 2023-08-16 07:10:06.000000 libcoveweb-0.30.2/cove/templates/input.html
--rw-r--r--   0 odscjames  (1000) odscjames  (1000)     3004 2023-08-16 07:10:06.000000 libcoveweb-0.30.2/cove/templates/modal_errors.html
--rw-r--r--   0 odscjames  (1000) odscjames  (1000)      534 2023-08-16 07:10:06.000000 libcoveweb-0.30.2/cove/templates/modal_list.html
--rw-r--r--   0 odscjames  (1000) odscjames  (1000)     1647 2023-08-16 07:10:06.000000 libcoveweb-0.30.2/cove/templates/page_header.html
--rw-r--r--   0 odscjames  (1000) odscjames  (1000)     1157 2023-08-16 07:10:06.000000 libcoveweb-0.30.2/cove/templates/piwik.html
--rw-r--r--   0 odscjames  (1000) odscjames  (1000)     1092 2023-08-16 07:10:06.000000 libcoveweb-0.30.2/cove/templates/stats.html
--rw-r--r--   0 odscjames  (1000) odscjames  (1000)     1034 2023-08-16 07:10:06.000000 libcoveweb-0.30.2/cove/templates/terms.html
--rw-r--r--   0 odscjames  (1000) odscjames  (1000)     1954 2023-08-16 07:10:06.000000 libcoveweb-0.30.2/cove/templates/terms_conditions.html
--rw-r--r--   0 odscjames  (1000) odscjames  (1000)     2351 2023-08-16 07:10:06.000000 libcoveweb-0.30.2/cove/templates/terms_conditions_intro.html
--rw-r--r--   0 odscjames  (1000) odscjames  (1000)     2043 2023-08-16 07:10:06.000000 libcoveweb-0.30.2/cove/templates/terms_cookies.html
--rw-r--r--   0 odscjames  (1000) odscjames  (1000)      195 2023-08-16 07:10:06.000000 libcoveweb-0.30.2/cove/templates/terms_cookies_link_google_analytics.html
--rw-r--r--   0 odscjames  (1000) odscjames  (1000)      124 2023-08-16 07:10:06.000000 libcoveweb-0.30.2/cove/templates/terms_cookies_link_matmo.html
--rw-r--r--   0 odscjames  (1000) odscjames  (1000)      105 2023-08-16 07:10:06.000000 libcoveweb-0.30.2/cove/templates/terms_cookies_links.html
--rw-r--r--   0 odscjames  (1000) odscjames  (1000)      484 2023-08-16 07:10:06.000000 libcoveweb-0.30.2/cove/templates/terms_cookies_we_use.html
--rw-r--r--   0 odscjames  (1000) odscjames  (1000)      830 2023-08-16 07:10:06.000000 libcoveweb-0.30.2/cove/templates/terms_data_deleting.html
--rw-r--r--   0 odscjames  (1000) odscjames  (1000)      764 2023-08-16 07:10:06.000000 libcoveweb-0.30.2/cove/templates/terms_data_uploaded.html
--rw-r--r--   0 odscjames  (1000) odscjames  (1000)     1357 2023-08-16 07:10:06.000000 libcoveweb-0.30.2/cove/templates/terms_disclaimer.html
--rw-r--r--   0 odscjames  (1000) odscjames  (1000)      525 2023-08-16 07:10:06.000000 libcoveweb-0.30.2/cove/templates/terms_links.html
--rw-r--r--   0 odscjames  (1000) odscjames  (1000)     1448 2023-08-16 07:10:06.000000 libcoveweb-0.30.2/cove/templates/terms_privacy.html
--rw-r--r--   0 odscjames  (1000) odscjames  (1000)     1165 2023-08-16 07:10:06.000000 libcoveweb-0.30.2/cove/templates/terms_privacy_intro.html
--rw-r--r--   0 odscjames  (1000) odscjames  (1000)      279 2023-08-16 07:10:06.000000 libcoveweb-0.30.2/cove/templates/terms_security.html
--rw-r--r--   0 odscjames  (1000) odscjames  (1000)        0 2023-08-16 07:10:06.000000 libcoveweb-0.30.2/cove/templates/terms_tracker_data_controller_international.html
--rw-r--r--   0 odscjames  (1000) odscjames  (1000)      804 2023-08-16 07:10:06.000000 libcoveweb-0.30.2/cove/templates/terms_tracker_google_analytics.html
--rw-r--r--   0 odscjames  (1000) odscjames  (1000)     1197 2023-08-16 07:10:06.000000 libcoveweb-0.30.2/cove/templates/terms_tracker_matmo.html
--rw-r--r--   0 odscjames  (1000) odscjames  (1000)       81 2023-08-16 07:10:06.000000 libcoveweb-0.30.2/cove/templates/terms_tracker_no_international.html
--rw-r--r--   0 odscjames  (1000) odscjames  (1000)      969 2023-08-16 07:10:06.000000 libcoveweb-0.30.2/cove/templates/terms_tracker_sentry.html
--rw-r--r--   0 odscjames  (1000) odscjames  (1000)      856 2023-08-16 07:10:06.000000 libcoveweb-0.30.2/cove/templates/terms_tracker_server.html
--rw-r--r--   0 odscjames  (1000) odscjames  (1000)      427 2023-08-16 07:10:06.000000 libcoveweb-0.30.2/cove/templates/terms_trackers.html
--rw-r--r--   0 odscjames  (1000) odscjames  (1000)     2506 2023-08-16 07:10:06.000000 libcoveweb-0.30.2/cove/templates/validation_table.html
-drwxr-xr-x   0 odscjames  (1000) odscjames  (1000)        0 2024-01-30 15:39:56.178465 libcoveweb-0.30.2/cove/templatetags/
--rw-r--r--   0 odscjames  (1000) odscjames  (1000)        0 2023-08-16 07:10:06.000000 libcoveweb-0.30.2/cove/templatetags/__init__.py
--rw-r--r--   0 odscjames  (1000) odscjames  (1000)     1690 2023-08-16 07:10:06.000000 libcoveweb-0.30.2/cove/templatetags/cove_tags.py
--rw-r--r--   0 odscjames  (1000) odscjames  (1000)     9021 2023-08-16 07:10:06.000000 libcoveweb-0.30.2/cove/tests.py
--rw-r--r--   0 odscjames  (1000) odscjames  (1000)      983 2023-08-16 07:10:06.000000 libcoveweb-0.30.2/cove/urls.py
--rw-r--r--   0 odscjames  (1000) odscjames  (1000)     5438 2024-01-30 15:29:06.000000 libcoveweb-0.30.2/cove/views.py
-drwxr-xr-x   0 odscjames  (1000) odscjames  (1000)        0 2024-01-30 15:39:56.178465 libcoveweb-0.30.2/libcoveweb.egg-info/
--rw-r--r--   0 odscjames  (1000) odscjames  (1000)      395 2024-01-30 15:39:56.000000 libcoveweb-0.30.2/libcoveweb.egg-info/PKG-INFO
--rw-r--r--   0 odscjames  (1000) odscjames  (1000)     7243 2024-01-30 15:39:56.000000 libcoveweb-0.30.2/libcoveweb.egg-info/SOURCES.txt
--rw-r--r--   0 odscjames  (1000) odscjames  (1000)        1 2024-01-30 15:39:56.000000 libcoveweb-0.30.2/libcoveweb.egg-info/dependency_links.txt
--rw-r--r--   0 odscjames  (1000) odscjames  (1000)      215 2024-01-30 15:39:56.000000 libcoveweb-0.30.2/libcoveweb.egg-info/requires.txt
--rw-r--r--   0 odscjames  (1000) odscjames  (1000)        5 2024-01-30 15:39:56.000000 libcoveweb-0.30.2/libcoveweb.egg-info/top_level.txt
--rwxr-xr-x   0 odscjames  (1000) odscjames  (1000)      247 2023-08-16 07:10:06.000000 libcoveweb-0.30.2/manage.py
--rw-r--r--   0 odscjames  (1000) odscjames  (1000)      147 2024-01-30 15:39:56.178465 libcoveweb-0.30.2/setup.cfg
--rw-r--r--   0 odscjames  (1000) odscjames  (1000)     1341 2024-01-30 15:39:16.000000 libcoveweb-0.30.2/setup.py
+drwxrwxr-x   0 bjwebb    (1000) bjwebb    (1000)        0 2024-05-29 21:51:26.777771 libcoveweb-0.30.3/
+-rw-rw-r--   0 bjwebb    (1000) bjwebb    (1000)     2141 2023-01-12 10:32:22.000000 libcoveweb-0.30.3/LICENCE.rst
+-rw-rw-r--   0 bjwebb    (1000) bjwebb    (1000)      410 2024-05-29 21:51:26.777771 libcoveweb-0.30.3/PKG-INFO
+-rw-rw-r--   0 bjwebb    (1000) bjwebb    (1000)     3492 2024-05-29 15:42:53.000000 libcoveweb-0.30.3/README.md
+drwxrwxr-x   0 bjwebb    (1000) bjwebb    (1000)        0 2024-05-29 21:51:26.717763 libcoveweb-0.30.3/cove/
+-rw-rw-r--   0 bjwebb    (1000) bjwebb    (1000)        0 2023-01-12 10:32:22.000000 libcoveweb-0.30.3/cove/__init__.py
+-rw-rw-r--   0 bjwebb    (1000) bjwebb    (1000)      544 2023-01-12 10:32:22.000000 libcoveweb-0.30.3/cove/context_processors.py
+drwxrwxr-x   0 bjwebb    (1000) bjwebb    (1000)        0 2024-05-29 21:51:26.721764 libcoveweb-0.30.3/cove/fixtures/
+-rw-rw-r--   0 bjwebb    (1000) bjwebb    (1000)        0 2023-01-12 10:32:22.000000 libcoveweb-0.30.3/cove/fixtures/bad.xlsx
+-rw-rw-r--   0 bjwebb    (1000) bjwebb    (1000)    25816 2023-01-12 10:32:22.000000 libcoveweb-0.30.3/cove/fixtures/badfile.json
+-rw-rw-r--   0 bjwebb    (1000) bjwebb    (1000)     5771 2023-01-12 10:32:22.000000 libcoveweb-0.30.3/cove/fixtures/basic.xlsx
+-rw-rw-r--   0 bjwebb    (1000) bjwebb    (1000)       65 2023-01-12 10:32:22.000000 libcoveweb-0.30.3/cove/fixtures/utf8.json
+-rw-rw-r--   0 bjwebb    (1000) bjwebb    (1000)     9398 2024-05-29 15:42:53.000000 libcoveweb-0.30.3/cove/html_error_msg.py
+drwxrwxr-x   0 bjwebb    (1000) bjwebb    (1000)        0 2024-05-29 21:51:26.721764 libcoveweb-0.30.3/cove/input/
+-rw-rw-r--   0 bjwebb    (1000) bjwebb    (1000)        0 2023-01-12 10:32:22.000000 libcoveweb-0.30.3/cove/input/__init__.py
+drwxrwxr-x   0 bjwebb    (1000) bjwebb    (1000)        0 2024-05-29 21:51:26.725764 libcoveweb-0.30.3/cove/input/migrations/
+-rw-rw-r--   0 bjwebb    (1000) bjwebb    (1000)      565 2023-01-12 10:32:22.000000 libcoveweb-0.30.3/cove/input/migrations/0001_initial.py
+-rw-rw-r--   0 bjwebb    (1000) bjwebb    (1000)      455 2023-01-12 10:32:22.000000 libcoveweb-0.30.3/cove/input/migrations/0002_supplieddata_current_app.py
+-rw-rw-r--   0 bjwebb    (1000) bjwebb    (1000)      893 2023-01-12 10:32:22.000000 libcoveweb-0.30.3/cove/input/migrations/0003_auto_20150506_1649.py
+-rw-rw-r--   0 bjwebb    (1000) bjwebb    (1000)      462 2023-01-12 10:32:22.000000 libcoveweb-0.30.3/cove/input/migrations/0004_auto_20150908_1533.py
+-rw-rw-r--   0 bjwebb    (1000) bjwebb    (1000)      422 2023-01-12 10:32:22.000000 libcoveweb-0.30.3/cove/input/migrations/0005_auto_20160104_1208.py
+-rw-rw-r--   0 bjwebb    (1000) bjwebb    (1000)      444 2023-01-12 10:32:22.000000 libcoveweb-0.30.3/cove/input/migrations/0006_supplieddata_rendered.py
+-rw-rw-r--   0 bjwebb    (1000) bjwebb    (1000)      591 2023-01-12 10:32:22.000000 libcoveweb-0.30.3/cove/input/migrations/0007_supplied_data_schema_version.py
+-rw-rw-r--   0 bjwebb    (1000) bjwebb    (1000)      488 2023-01-12 10:32:22.000000 libcoveweb-0.30.3/cove/input/migrations/0008_supplieddata_data_schema_version.py
+-rw-rw-r--   0 bjwebb    (1000) bjwebb    (1000)      415 2023-01-12 10:32:22.000000 libcoveweb-0.30.3/cove/input/migrations/0009_supplieddata_parameters.py
+-rw-rw-r--   0 bjwebb    (1000) bjwebb    (1000)      468 2024-05-29 15:42:53.000000 libcoveweb-0.30.3/cove/input/migrations/0010_alter_supplieddata_original_file.py
+-rw-rw-r--   0 bjwebb    (1000) bjwebb    (1000)        0 2023-01-12 10:32:22.000000 libcoveweb-0.30.3/cove/input/migrations/__init__.py
+-rw-rw-r--   0 bjwebb    (1000) bjwebb    (1000)     3863 2023-03-06 16:25:33.000000 libcoveweb-0.30.3/cove/input/models.py
+-rw-rw-r--   0 bjwebb    (1000) bjwebb    (1000)     4251 2024-05-29 15:42:53.000000 libcoveweb-0.30.3/cove/input/views.py
+drwxrwxr-x   0 bjwebb    (1000) bjwebb    (1000)        0 2024-05-29 21:51:26.725764 libcoveweb-0.30.3/cove/lib/
+-rw-rw-r--   0 bjwebb    (1000) bjwebb    (1000)        0 2023-01-12 10:32:22.000000 libcoveweb-0.30.3/cove/lib/__init__.py
+-rw-rw-r--   0 bjwebb    (1000) bjwebb    (1000)     1992 2023-01-12 10:32:22.000000 libcoveweb-0.30.3/cove/lib/common.py
+drwxrwxr-x   0 bjwebb    (1000) bjwebb    (1000)        0 2024-05-29 21:51:26.713763 libcoveweb-0.30.3/cove/locale/
+drwxrwxr-x   0 bjwebb    (1000) bjwebb    (1000)        0 2024-05-29 21:51:26.713763 libcoveweb-0.30.3/cove/locale/en/
+drwxrwxr-x   0 bjwebb    (1000) bjwebb    (1000)        0 2024-05-29 21:51:26.729765 libcoveweb-0.30.3/cove/locale/en/LC_MESSAGES/
+-rw-rw-r--   0 bjwebb    (1000) bjwebb    (1000)      337 2023-01-12 10:32:22.000000 libcoveweb-0.30.3/cove/locale/en/LC_MESSAGES/django.mo
+-rw-rw-r--   0 bjwebb    (1000) bjwebb    (1000)    13479 2024-05-29 15:42:53.000000 libcoveweb-0.30.3/cove/locale/en/LC_MESSAGES/django.po
+drwxrwxr-x   0 bjwebb    (1000) bjwebb    (1000)        0 2024-05-29 21:51:26.713763 libcoveweb-0.30.3/cove/locale/es/
+drwxrwxr-x   0 bjwebb    (1000) bjwebb    (1000)        0 2024-05-29 21:51:26.729765 libcoveweb-0.30.3/cove/locale/es/LC_MESSAGES/
+-rw-rw-r--   0 bjwebb    (1000) bjwebb    (1000)    13403 2024-05-29 15:42:53.000000 libcoveweb-0.30.3/cove/locale/es/LC_MESSAGES/django.mo
+-rw-rw-r--   0 bjwebb    (1000) bjwebb    (1000)    19627 2024-05-29 15:42:53.000000 libcoveweb-0.30.3/cove/locale/es/LC_MESSAGES/django.po
+drwxrwxr-x   0 bjwebb    (1000) bjwebb    (1000)        0 2024-05-29 21:51:26.729765 libcoveweb-0.30.3/cove/management/
+-rw-rw-r--   0 bjwebb    (1000) bjwebb    (1000)        0 2023-01-12 10:32:22.000000 libcoveweb-0.30.3/cove/management/__init__.py
+drwxrwxr-x   0 bjwebb    (1000) bjwebb    (1000)        0 2024-05-29 21:51:26.729765 libcoveweb-0.30.3/cove/management/commands/
+-rw-rw-r--   0 bjwebb    (1000) bjwebb    (1000)        0 2023-01-12 10:32:22.000000 libcoveweb-0.30.3/cove/management/commands/__init__.py
+-rw-rw-r--   0 bjwebb    (1000) bjwebb    (1000)     1594 2023-01-12 10:32:22.000000 libcoveweb-0.30.3/cove/management/commands/base_command.py
+-rw-rw-r--   0 bjwebb    (1000) bjwebb    (1000)      649 2023-01-12 10:32:22.000000 libcoveweb-0.30.3/cove/management/commands/expire_files.py
+-rw-rw-r--   0 bjwebb    (1000) bjwebb    (1000)     1370 2023-01-12 10:32:22.000000 libcoveweb-0.30.3/cove/management/commands/tests.py
+-rw-rw-r--   0 bjwebb    (1000) bjwebb    (1000)      592 2023-01-12 10:32:22.000000 libcoveweb-0.30.3/cove/management/commands/upload.py
+-rw-rw-r--   0 bjwebb    (1000) bjwebb    (1000)      354 2023-01-12 10:32:22.000000 libcoveweb-0.30.3/cove/middleware.py
+drwxrwxr-x   0 bjwebb    (1000) bjwebb    (1000)        0 2024-05-29 21:51:26.713763 libcoveweb-0.30.3/cove/sass/
+drwxrwxr-x   0 bjwebb    (1000) bjwebb    (1000)        0 2024-05-29 21:51:26.729765 libcoveweb-0.30.3/cove/sass/bootstrap/
+-rw-rw-r--   0 bjwebb    (1000) bjwebb    (1000)      178 2023-01-12 10:32:22.000000 libcoveweb-0.30.3/cove/sass/bootstrap/_bootstrap-compass.scss
+-rw-rw-r--   0 bjwebb    (1000) bjwebb    (1000)      757 2023-01-12 10:32:22.000000 libcoveweb-0.30.3/cove/sass/bootstrap/_bootstrap-mincer.scss
+-rw-rw-r--   0 bjwebb    (1000) bjwebb    (1000)      168 2023-01-12 10:32:22.000000 libcoveweb-0.30.3/cove/sass/bootstrap/_bootstrap-sprockets.scss
+-rw-rw-r--   0 bjwebb    (1000) bjwebb    (1000)     1486 2023-01-12 10:32:22.000000 libcoveweb-0.30.3/cove/sass/bootstrap/_bootstrap.scss
+drwxrwxr-x   0 bjwebb    (1000) bjwebb    (1000)        0 2024-05-29 21:51:26.749767 libcoveweb-0.30.3/cove/sass/bootstrap/bootstrap/
+-rw-rw-r--   0 bjwebb    (1000) bjwebb    (1000)     1550 2023-01-12 10:32:22.000000 libcoveweb-0.30.3/cove/sass/bootstrap/bootstrap/_alerts.scss
+-rw-rw-r--   0 bjwebb    (1000) bjwebb    (1000)     1228 2023-01-12 10:32:22.000000 libcoveweb-0.30.3/cove/sass/bootstrap/bootstrap/_badges.scss
+-rw-rw-r--   0 bjwebb    (1000) bjwebb    (1000)      700 2023-01-12 10:32:22.000000 libcoveweb-0.30.3/cove/sass/bootstrap/bootstrap/_breadcrumbs.scss
+-rw-rw-r--   0 bjwebb    (1000) bjwebb    (1000)     5758 2023-01-12 10:32:22.000000 libcoveweb-0.30.3/cove/sass/bootstrap/bootstrap/_button-groups.scss
+-rw-rw-r--   0 bjwebb    (1000) bjwebb    (1000)     3819 2023-01-12 10:32:22.000000 libcoveweb-0.30.3/cove/sass/bootstrap/bootstrap/_buttons.scss
+-rw-rw-r--   0 bjwebb    (1000) bjwebb    (1000)     5725 2023-01-12 10:32:22.000000 libcoveweb-0.30.3/cove/sass/bootstrap/bootstrap/_carousel.scss
+-rw-rw-r--   0 bjwebb    (1000) bjwebb    (1000)      815 2023-01-12 10:32:22.000000 libcoveweb-0.30.3/cove/sass/bootstrap/bootstrap/_close.scss
+-rw-rw-r--   0 bjwebb    (1000) bjwebb    (1000)     1401 2023-01-12 10:32:22.000000 libcoveweb-0.30.3/cove/sass/bootstrap/bootstrap/_code.scss
+-rw-rw-r--   0 bjwebb    (1000) bjwebb    (1000)      819 2023-01-12 10:32:22.000000 libcoveweb-0.30.3/cove/sass/bootstrap/bootstrap/_component-animations.scss
+-rw-rw-r--   0 bjwebb    (1000) bjwebb    (1000)     4889 2023-01-12 10:32:22.000000 libcoveweb-0.30.3/cove/sass/bootstrap/bootstrap/_dropdowns.scss
+-rw-rw-r--   0 bjwebb    (1000) bjwebb    (1000)    16162 2023-01-12 10:32:22.000000 libcoveweb-0.30.3/cove/sass/bootstrap/bootstrap/_forms.scss
+-rw-rw-r--   0 bjwebb    (1000) bjwebb    (1000)    20448 2023-01-12 10:32:22.000000 libcoveweb-0.30.3/cove/sass/bootstrap/bootstrap/_glyphicons.scss
+-rw-rw-r--   0 bjwebb    (1000) bjwebb    (1000)     1443 2023-01-12 10:32:22.000000 libcoveweb-0.30.3/cove/sass/bootstrap/bootstrap/_grid.scss
+-rw-rw-r--   0 bjwebb    (1000) bjwebb    (1000)     4313 2023-01-12 10:32:22.000000 libcoveweb-0.30.3/cove/sass/bootstrap/bootstrap/_input-groups.scss
+-rw-rw-r--   0 bjwebb    (1000) bjwebb    (1000)     1152 2023-01-12 10:32:22.000000 libcoveweb-0.30.3/cove/sass/bootstrap/bootstrap/_jumbotron.scss
+-rw-rw-r--   0 bjwebb    (1000) bjwebb    (1000)     1156 2023-01-12 10:32:22.000000 libcoveweb-0.30.3/cove/sass/bootstrap/bootstrap/_labels.scss
+-rw-rw-r--   0 bjwebb    (1000) bjwebb    (1000)     3172 2023-01-12 10:32:22.000000 libcoveweb-0.30.3/cove/sass/bootstrap/bootstrap/_list-group.scss
+-rw-rw-r--   0 bjwebb    (1000) bjwebb    (1000)      900 2023-01-12 10:32:22.000000 libcoveweb-0.30.3/cove/sass/bootstrap/bootstrap/_media.scss
+-rw-rw-r--   0 bjwebb    (1000) bjwebb    (1000)      986 2023-01-12 10:32:22.000000 libcoveweb-0.30.3/cove/sass/bootstrap/bootstrap/_mixins.scss
+-rw-rw-r--   0 bjwebb    (1000) bjwebb    (1000)     3568 2023-01-12 10:32:22.000000 libcoveweb-0.30.3/cove/sass/bootstrap/bootstrap/_modals.scss
+-rw-rw-r--   0 bjwebb    (1000) bjwebb    (1000)    14729 2023-01-12 10:32:22.000000 libcoveweb-0.30.3/cove/sass/bootstrap/bootstrap/_navbar.scss
+-rw-rw-r--   0 bjwebb    (1000) bjwebb    (1000)     4950 2023-01-12 10:32:22.000000 libcoveweb-0.30.3/cove/sass/bootstrap/bootstrap/_navs.scss
+-rw-rw-r--   0 bjwebb    (1000) bjwebb    (1000)     7559 2023-01-12 10:32:22.000000 libcoveweb-0.30.3/cove/sass/bootstrap/bootstrap/_normalize.scss
+-rw-rw-r--   0 bjwebb    (1000) bjwebb    (1000)      855 2023-01-12 10:32:22.000000 libcoveweb-0.30.3/cove/sass/bootstrap/bootstrap/_pager.scss
+-rw-rw-r--   0 bjwebb    (1000) bjwebb    (1000)     2091 2023-01-12 10:32:22.000000 libcoveweb-0.30.3/cove/sass/bootstrap/bootstrap/_pagination.scss
+-rw-rw-r--   0 bjwebb    (1000) bjwebb    (1000)     6385 2023-01-12 10:32:22.000000 libcoveweb-0.30.3/cove/sass/bootstrap/bootstrap/_panels.scss
+-rw-rw-r--   0 bjwebb    (1000) bjwebb    (1000)     3502 2023-01-12 10:32:22.000000 libcoveweb-0.30.3/cove/sass/bootstrap/bootstrap/_popovers.scss
+-rw-rw-r--   0 bjwebb    (1000) bjwebb    (1000)     1939 2023-01-12 10:32:22.000000 libcoveweb-0.30.3/cove/sass/bootstrap/bootstrap/_print.scss
+-rw-rw-r--   0 bjwebb    (1000) bjwebb    (1000)     1992 2023-01-12 10:32:22.000000 libcoveweb-0.30.3/cove/sass/bootstrap/bootstrap/_progress-bars.scss
+-rw-rw-r--   0 bjwebb    (1000) bjwebb    (1000)      546 2023-01-12 10:32:22.000000 libcoveweb-0.30.3/cove/sass/bootstrap/bootstrap/_responsive-embed.scss
+-rw-rw-r--   0 bjwebb    (1000) bjwebb    (1000)     4409 2023-01-12 10:32:22.000000 libcoveweb-0.30.3/cove/sass/bootstrap/bootstrap/_responsive-utilities.scss
+-rw-rw-r--   0 bjwebb    (1000) bjwebb    (1000)     3031 2023-01-12 10:32:22.000000 libcoveweb-0.30.3/cove/sass/bootstrap/bootstrap/_scaffolding.scss
+-rw-rw-r--   0 bjwebb    (1000) bjwebb    (1000)     4662 2023-01-12 10:32:22.000000 libcoveweb-0.30.3/cove/sass/bootstrap/bootstrap/_tables.scss
+-rw-rw-r--   0 bjwebb    (1000) bjwebb    (1000)     8558 2023-01-12 10:32:22.000000 libcoveweb-0.30.3/cove/sass/bootstrap/bootstrap/_theme.scss
+-rw-rw-r--   0 bjwebb    (1000) bjwebb    (1000)      892 2023-01-12 10:32:22.000000 libcoveweb-0.30.3/cove/sass/bootstrap/bootstrap/_thumbnails.scss
+-rw-rw-r--   0 bjwebb    (1000) bjwebb    (1000)     3007 2023-01-12 10:32:22.000000 libcoveweb-0.30.3/cove/sass/bootstrap/bootstrap/_tooltip.scss
+-rw-rw-r--   0 bjwebb    (1000) bjwebb    (1000)     6149 2023-01-12 10:32:22.000000 libcoveweb-0.30.3/cove/sass/bootstrap/bootstrap/_type.scss
+-rw-rw-r--   0 bjwebb    (1000) bjwebb    (1000)      765 2023-01-12 10:32:22.000000 libcoveweb-0.30.3/cove/sass/bootstrap/bootstrap/_utilities.scss
+-rw-rw-r--   0 bjwebb    (1000) bjwebb    (1000)    31290 2023-01-12 10:32:22.000000 libcoveweb-0.30.3/cove/sass/bootstrap/bootstrap/_variables.scss
+-rw-rw-r--   0 bjwebb    (1000) bjwebb    (1000)      535 2023-01-12 10:32:22.000000 libcoveweb-0.30.3/cove/sass/bootstrap/bootstrap/_wells.scss
+drwxrwxr-x   0 bjwebb    (1000) bjwebb    (1000)        0 2024-05-29 21:51:26.757768 libcoveweb-0.30.3/cove/sass/bootstrap/bootstrap/mixins/
+-rw-rw-r--   0 bjwebb    (1000) bjwebb    (1000)      263 2023-01-12 10:32:22.000000 libcoveweb-0.30.3/cove/sass/bootstrap/bootstrap/mixins/_alerts.scss
+-rw-rw-r--   0 bjwebb    (1000) bjwebb    (1000)      233 2023-01-12 10:32:22.000000 libcoveweb-0.30.3/cove/sass/bootstrap/bootstrap/mixins/_background-variant.scss
+-rw-rw-r--   0 bjwebb    (1000) bjwebb    (1000)      492 2023-01-12 10:32:22.000000 libcoveweb-0.30.3/cove/sass/bootstrap/bootstrap/mixins/_border-radius.scss
+-rw-rw-r--   0 bjwebb    (1000) bjwebb    (1000)     1453 2023-01-12 10:32:22.000000 libcoveweb-0.30.3/cove/sass/bootstrap/bootstrap/mixins/_buttons.scss
+-rw-rw-r--   0 bjwebb    (1000) bjwebb    (1000)      126 2023-01-12 10:32:22.000000 libcoveweb-0.30.3/cove/sass/bootstrap/bootstrap/mixins/_center-block.scss
+-rw-rw-r--   0 bjwebb    (1000) bjwebb    (1000)      611 2023-01-12 10:32:22.000000 libcoveweb-0.30.3/cove/sass/bootstrap/bootstrap/mixins/_clearfix.scss
+-rw-rw-r--   0 bjwebb    (1000) bjwebb    (1000)     2771 2023-01-12 10:32:22.000000 libcoveweb-0.30.3/cove/sass/bootstrap/bootstrap/mixins/_forms.scss
+-rw-rw-r--   0 bjwebb    (1000) bjwebb    (1000)     4392 2023-01-12 10:32:22.000000 libcoveweb-0.30.3/cove/sass/bootstrap/bootstrap/mixins/_gradients.scss
+-rw-rw-r--   0 bjwebb    (1000) bjwebb    (1000)     2360 2023-01-12 10:32:22.000000 libcoveweb-0.30.3/cove/sass/bootstrap/bootstrap/mixins/_grid-framework.scss
+-rw-rw-r--   0 bjwebb    (1000) bjwebb    (1000)     3216 2023-01-12 10:32:22.000000 libcoveweb-0.30.3/cove/sass/bootstrap/bootstrap/mixins/_grid.scss
+-rw-rw-r--   0 bjwebb    (1000) bjwebb    (1000)      590 2023-01-12 10:32:22.000000 libcoveweb-0.30.3/cove/sass/bootstrap/bootstrap/mixins/_hide-text.scss
+-rw-rw-r--   0 bjwebb    (1000) bjwebb    (1000)     1208 2023-01-12 10:32:22.000000 libcoveweb-0.30.3/cove/sass/bootstrap/bootstrap/mixins/_image.scss
+-rw-rw-r--   0 bjwebb    (1000) bjwebb    (1000)      167 2023-01-12 10:32:22.000000 libcoveweb-0.30.3/cove/sass/bootstrap/bootstrap/mixins/_labels.scss
+-rw-rw-r--   0 bjwebb    (1000) bjwebb    (1000)      672 2023-01-12 10:32:22.000000 libcoveweb-0.30.3/cove/sass/bootstrap/bootstrap/mixins/_list-group.scss
+-rw-rw-r--   0 bjwebb    (1000) bjwebb    (1000)      238 2023-01-12 10:32:22.000000 libcoveweb-0.30.3/cove/sass/bootstrap/bootstrap/mixins/_nav-divider.scss
+-rw-rw-r--   0 bjwebb    (1000) bjwebb    (1000)      370 2023-01-12 10:32:22.000000 libcoveweb-0.30.3/cove/sass/bootstrap/bootstrap/mixins/_nav-vertical-align.scss
+-rw-rw-r--   0 bjwebb    (1000) bjwebb    (1000)      149 2023-01-12 10:32:22.000000 libcoveweb-0.30.3/cove/sass/bootstrap/bootstrap/mixins/_opacity.scss
+-rw-rw-r--   0 bjwebb    (1000) bjwebb    (1000)      507 2023-01-12 10:32:22.000000 libcoveweb-0.30.3/cove/sass/bootstrap/bootstrap/mixins/_pagination.scss
+-rw-rw-r--   0 bjwebb    (1000) bjwebb    (1000)      543 2023-01-12 10:32:22.000000 libcoveweb-0.30.3/cove/sass/bootstrap/bootstrap/mixins/_panels.scss
+-rw-rw-r--   0 bjwebb    (1000) bjwebb    (1000)      200 2023-01-12 10:32:22.000000 libcoveweb-0.30.3/cove/sass/bootstrap/bootstrap/mixins/_progress-bar.scss
+-rw-rw-r--   0 bjwebb    (1000) bjwebb    (1000)      246 2023-01-12 10:32:22.000000 libcoveweb-0.30.3/cove/sass/bootstrap/bootstrap/mixins/_reset-filter.scss
+-rw-rw-r--   0 bjwebb    (1000) bjwebb    (1000)      476 2023-01-12 10:32:22.000000 libcoveweb-0.30.3/cove/sass/bootstrap/bootstrap/mixins/_reset-text.scss
+-rw-rw-r--   0 bjwebb    (1000) bjwebb    (1000)      202 2023-01-12 10:32:22.000000 libcoveweb-0.30.3/cove/sass/bootstrap/bootstrap/mixins/_resize.scss
+-rw-rw-r--   0 bjwebb    (1000) bjwebb    (1000)      514 2023-01-12 10:32:22.000000 libcoveweb-0.30.3/cove/sass/bootstrap/bootstrap/mixins/_responsive-visibility.scss
+-rw-rw-r--   0 bjwebb    (1000) bjwebb    (1000)      147 2023-01-12 10:32:22.000000 libcoveweb-0.30.3/cove/sass/bootstrap/bootstrap/mixins/_size.scss
+-rw-rw-r--   0 bjwebb    (1000) bjwebb    (1000)      338 2023-01-12 10:32:22.000000 libcoveweb-0.30.3/cove/sass/bootstrap/bootstrap/mixins/_tab-focus.scss
+-rw-rw-r--   0 bjwebb    (1000) bjwebb    (1000)      715 2023-01-12 10:32:22.000000 libcoveweb-0.30.3/cove/sass/bootstrap/bootstrap/mixins/_table-row.scss
+-rw-rw-r--   0 bjwebb    (1000) bjwebb    (1000)      210 2023-01-12 10:32:22.000000 libcoveweb-0.30.3/cove/sass/bootstrap/bootstrap/mixins/_text-emphasis.scss
+-rw-rw-r--   0 bjwebb    (1000) bjwebb    (1000)      168 2023-01-12 10:32:22.000000 libcoveweb-0.30.3/cove/sass/bootstrap/bootstrap/mixins/_text-overflow.scss
+-rw-rw-r--   0 bjwebb    (1000) bjwebb    (1000)     6645 2023-01-12 10:32:22.000000 libcoveweb-0.30.3/cove/sass/bootstrap/bootstrap/mixins/_vendor-prefixes.scss
+-rw-rw-r--   0 bjwebb    (1000) bjwebb    (1000)     4771 2024-05-29 15:42:53.000000 libcoveweb-0.30.3/cove/settings.py
+drwxrwxr-x   0 bjwebb    (1000) bjwebb    (1000)        0 2024-05-29 21:51:26.713763 libcoveweb-0.30.3/cove/static/
+drwxrwxr-x   0 bjwebb    (1000) bjwebb    (1000)        0 2024-05-29 21:51:26.713763 libcoveweb-0.30.3/cove/static/dataexplore/
+drwxrwxr-x   0 bjwebb    (1000) bjwebb    (1000)        0 2024-05-29 21:51:26.757768 libcoveweb-0.30.3/cove/static/dataexplore/css/
+-rw-rw-r--   0 bjwebb    (1000) bjwebb    (1000)     1833 2023-01-12 10:32:22.000000 libcoveweb-0.30.3/cove/static/dataexplore/css/style.css
+drwxrwxr-x   0 bjwebb    (1000) bjwebb    (1000)        0 2024-05-29 21:51:26.713763 libcoveweb-0.30.3/cove/static/dataexplore/fonts/
+drwxrwxr-x   0 bjwebb    (1000) bjwebb    (1000)        0 2024-05-29 21:51:26.761769 libcoveweb-0.30.3/cove/static/dataexplore/fonts/bootstrap/
+-rw-rw-r--   0 bjwebb    (1000) bjwebb    (1000)    20127 2023-01-12 10:32:22.000000 libcoveweb-0.30.3/cove/static/dataexplore/fonts/bootstrap/glyphicons-halflings-regular.eot
+-rw-rw-r--   0 bjwebb    (1000) bjwebb    (1000)   108738 2023-01-12 10:32:22.000000 libcoveweb-0.30.3/cove/static/dataexplore/fonts/bootstrap/glyphicons-halflings-regular.svg
+-rw-rw-r--   0 bjwebb    (1000) bjwebb    (1000)    45404 2023-01-12 10:32:22.000000 libcoveweb-0.30.3/cove/static/dataexplore/fonts/bootstrap/glyphicons-halflings-regular.ttf
+-rw-rw-r--   0 bjwebb    (1000) bjwebb    (1000)    23424 2023-01-12 10:32:22.000000 libcoveweb-0.30.3/cove/static/dataexplore/fonts/bootstrap/glyphicons-halflings-regular.woff
+-rw-rw-r--   0 bjwebb    (1000) bjwebb    (1000)    18028 2023-01-12 10:32:22.000000 libcoveweb-0.30.3/cove/static/dataexplore/fonts/bootstrap/glyphicons-halflings-regular.woff2
+drwxrwxr-x   0 bjwebb    (1000) bjwebb    (1000)        0 2024-05-29 21:51:26.765769 libcoveweb-0.30.3/cove/static/dataexplore/fonts/tick/
+-rw-rw-r--   0 bjwebb    (1000) bjwebb    (1000)      408 2023-01-12 10:32:22.000000 libcoveweb-0.30.3/cove/static/dataexplore/fonts/tick/tick.css
+-rw-rw-r--   0 bjwebb    (1000) bjwebb    (1000)     2328 2023-01-12 10:32:22.000000 libcoveweb-0.30.3/cove/static/dataexplore/fonts/tick/tick.eot
+-rw-rw-r--   0 bjwebb    (1000) bjwebb    (1000)     3063 2023-01-12 10:32:22.000000 libcoveweb-0.30.3/cove/static/dataexplore/fonts/tick/tick.svg
+-rw-rw-r--   0 bjwebb    (1000) bjwebb    (1000)     2168 2023-01-12 10:32:22.000000 libcoveweb-0.30.3/cove/static/dataexplore/fonts/tick/tick.ttf
+-rw-rw-r--   0 bjwebb    (1000) bjwebb    (1000)     1604 2023-01-12 10:32:22.000000 libcoveweb-0.30.3/cove/static/dataexplore/fonts/tick/tick.woff
+-rw-rw-r--   0 bjwebb    (1000) bjwebb    (1000)     1064 2023-01-12 10:32:22.000000 libcoveweb-0.30.3/cove/static/dataexplore/fonts/tick/tick.woff2
+drwxrwxr-x   0 bjwebb    (1000) bjwebb    (1000)        0 2024-05-29 21:51:26.777771 libcoveweb-0.30.3/cove/templates/
+-rw-rw-r--   0 bjwebb    (1000) bjwebb    (1000)     1114 2023-01-12 10:32:22.000000 libcoveweb-0.30.3/cove/templates/500.html
+-rw-rw-r--   0 bjwebb    (1000) bjwebb    (1000)      849 2024-05-29 15:42:53.000000 libcoveweb-0.30.3/cove/templates/additional_codelist_values.html
+-rw-rw-r--   0 bjwebb    (1000) bjwebb    (1000)      405 2023-01-12 10:32:22.000000 libcoveweb-0.30.3/cove/templates/additional_fields_table.html
+-rw-rw-r--   0 bjwebb    (1000) bjwebb    (1000)     2722 2023-01-12 10:32:22.000000 libcoveweb-0.30.3/cove/templates/additional_fields_table_all.html
+-rw-rw-r--   0 bjwebb    (1000) bjwebb    (1000)     4938 2023-01-12 10:32:22.000000 libcoveweb-0.30.3/cove/templates/base.html
+-rw-rw-r--   0 bjwebb    (1000) bjwebb    (1000)      748 2023-01-12 10:32:22.000000 libcoveweb-0.30.3/cove/templates/error.html
+-rw-rw-r--   0 bjwebb    (1000) bjwebb    (1000)      405 2023-01-12 10:32:22.000000 libcoveweb-0.30.3/cove/templates/error_extra.html
+-rw-rw-r--   0 bjwebb    (1000) bjwebb    (1000)     2431 2023-01-12 10:32:22.000000 libcoveweb-0.30.3/cove/templates/explore.html
+-rw-rw-r--   0 bjwebb    (1000) bjwebb    (1000)      479 2023-01-12 10:32:22.000000 libcoveweb-0.30.3/cove/templates/google_analytics.html
+-rw-rw-r--   0 bjwebb    (1000) bjwebb    (1000)     3845 2023-01-12 10:32:22.000000 libcoveweb-0.30.3/cove/templates/input.html
+-rw-rw-r--   0 bjwebb    (1000) bjwebb    (1000)     3004 2023-01-12 10:32:22.000000 libcoveweb-0.30.3/cove/templates/modal_errors.html
+-rw-rw-r--   0 bjwebb    (1000) bjwebb    (1000)      534 2023-01-12 10:32:22.000000 libcoveweb-0.30.3/cove/templates/modal_list.html
+-rw-rw-r--   0 bjwebb    (1000) bjwebb    (1000)     1647 2023-01-12 10:32:22.000000 libcoveweb-0.30.3/cove/templates/page_header.html
+-rw-rw-r--   0 bjwebb    (1000) bjwebb    (1000)     1157 2023-01-12 10:32:22.000000 libcoveweb-0.30.3/cove/templates/piwik.html
+-rw-rw-r--   0 bjwebb    (1000) bjwebb    (1000)     1092 2023-01-12 10:32:22.000000 libcoveweb-0.30.3/cove/templates/stats.html
+-rw-rw-r--   0 bjwebb    (1000) bjwebb    (1000)     1034 2023-01-12 10:32:22.000000 libcoveweb-0.30.3/cove/templates/terms.html
+-rw-rw-r--   0 bjwebb    (1000) bjwebb    (1000)     1954 2023-01-12 10:32:22.000000 libcoveweb-0.30.3/cove/templates/terms_conditions.html
+-rw-rw-r--   0 bjwebb    (1000) bjwebb    (1000)     2351 2023-01-12 10:32:22.000000 libcoveweb-0.30.3/cove/templates/terms_conditions_intro.html
+-rw-rw-r--   0 bjwebb    (1000) bjwebb    (1000)     2043 2023-01-12 10:32:22.000000 libcoveweb-0.30.3/cove/templates/terms_cookies.html
+-rw-rw-r--   0 bjwebb    (1000) bjwebb    (1000)      195 2023-01-12 10:32:22.000000 libcoveweb-0.30.3/cove/templates/terms_cookies_link_google_analytics.html
+-rw-rw-r--   0 bjwebb    (1000) bjwebb    (1000)      124 2023-01-12 10:32:22.000000 libcoveweb-0.30.3/cove/templates/terms_cookies_link_matmo.html
+-rw-rw-r--   0 bjwebb    (1000) bjwebb    (1000)      105 2023-01-12 10:32:22.000000 libcoveweb-0.30.3/cove/templates/terms_cookies_links.html
+-rw-rw-r--   0 bjwebb    (1000) bjwebb    (1000)      484 2023-01-12 10:32:22.000000 libcoveweb-0.30.3/cove/templates/terms_cookies_we_use.html
+-rw-rw-r--   0 bjwebb    (1000) bjwebb    (1000)      830 2023-01-12 10:32:22.000000 libcoveweb-0.30.3/cove/templates/terms_data_deleting.html
+-rw-rw-r--   0 bjwebb    (1000) bjwebb    (1000)      764 2023-01-12 10:32:22.000000 libcoveweb-0.30.3/cove/templates/terms_data_uploaded.html
+-rw-rw-r--   0 bjwebb    (1000) bjwebb    (1000)     1357 2023-01-12 10:32:22.000000 libcoveweb-0.30.3/cove/templates/terms_disclaimer.html
+-rw-rw-r--   0 bjwebb    (1000) bjwebb    (1000)      525 2023-01-12 10:32:22.000000 libcoveweb-0.30.3/cove/templates/terms_links.html
+-rw-rw-r--   0 bjwebb    (1000) bjwebb    (1000)     1448 2023-01-12 10:32:22.000000 libcoveweb-0.30.3/cove/templates/terms_privacy.html
+-rw-rw-r--   0 bjwebb    (1000) bjwebb    (1000)     1165 2023-01-12 10:32:22.000000 libcoveweb-0.30.3/cove/templates/terms_privacy_intro.html
+-rw-rw-r--   0 bjwebb    (1000) bjwebb    (1000)      279 2023-01-12 10:32:22.000000 libcoveweb-0.30.3/cove/templates/terms_security.html
+-rw-rw-r--   0 bjwebb    (1000) bjwebb    (1000)        0 2023-01-12 10:32:22.000000 libcoveweb-0.30.3/cove/templates/terms_tracker_data_controller_international.html
+-rw-rw-r--   0 bjwebb    (1000) bjwebb    (1000)      804 2023-01-12 10:32:22.000000 libcoveweb-0.30.3/cove/templates/terms_tracker_google_analytics.html
+-rw-rw-r--   0 bjwebb    (1000) bjwebb    (1000)     1197 2023-01-12 10:32:22.000000 libcoveweb-0.30.3/cove/templates/terms_tracker_matmo.html
+-rw-rw-r--   0 bjwebb    (1000) bjwebb    (1000)       81 2023-01-12 10:32:22.000000 libcoveweb-0.30.3/cove/templates/terms_tracker_no_international.html
+-rw-rw-r--   0 bjwebb    (1000) bjwebb    (1000)      969 2023-01-12 10:32:22.000000 libcoveweb-0.30.3/cove/templates/terms_tracker_sentry.html
+-rw-rw-r--   0 bjwebb    (1000) bjwebb    (1000)      856 2023-01-12 10:32:22.000000 libcoveweb-0.30.3/cove/templates/terms_tracker_server.html
+-rw-rw-r--   0 bjwebb    (1000) bjwebb    (1000)      427 2023-01-12 10:32:22.000000 libcoveweb-0.30.3/cove/templates/terms_trackers.html
+-rw-rw-r--   0 bjwebb    (1000) bjwebb    (1000)     2506 2023-01-12 10:32:22.000000 libcoveweb-0.30.3/cove/templates/validation_table.html
+drwxrwxr-x   0 bjwebb    (1000) bjwebb    (1000)        0 2024-05-29 21:51:26.777771 libcoveweb-0.30.3/cove/templatetags/
+-rw-rw-r--   0 bjwebb    (1000) bjwebb    (1000)        0 2023-01-12 10:32:22.000000 libcoveweb-0.30.3/cove/templatetags/__init__.py
+-rw-rw-r--   0 bjwebb    (1000) bjwebb    (1000)     1690 2023-01-12 10:32:22.000000 libcoveweb-0.30.3/cove/templatetags/cove_tags.py
+-rw-rw-r--   0 bjwebb    (1000) bjwebb    (1000)     9021 2023-01-12 10:32:22.000000 libcoveweb-0.30.3/cove/tests.py
+-rw-rw-r--   0 bjwebb    (1000) bjwebb    (1000)      983 2023-01-12 10:32:22.000000 libcoveweb-0.30.3/cove/urls.py
+-rw-rw-r--   0 bjwebb    (1000) bjwebb    (1000)     5438 2024-05-29 15:42:53.000000 libcoveweb-0.30.3/cove/views.py
+drwxrwxr-x   0 bjwebb    (1000) bjwebb    (1000)        0 2024-05-29 21:51:26.777771 libcoveweb-0.30.3/libcoveweb.egg-info/
+-rw-rw-r--   0 bjwebb    (1000) bjwebb    (1000)      410 2024-05-29 21:51:26.000000 libcoveweb-0.30.3/libcoveweb.egg-info/PKG-INFO
+-rw-rw-r--   0 bjwebb    (1000) bjwebb    (1000)     7255 2024-05-29 21:51:26.000000 libcoveweb-0.30.3/libcoveweb.egg-info/SOURCES.txt
+-rw-rw-r--   0 bjwebb    (1000) bjwebb    (1000)        1 2024-05-29 21:51:26.000000 libcoveweb-0.30.3/libcoveweb.egg-info/dependency_links.txt
+-rw-rw-r--   0 bjwebb    (1000) bjwebb    (1000)      215 2024-05-29 21:51:26.000000 libcoveweb-0.30.3/libcoveweb.egg-info/requires.txt
+-rw-rw-r--   0 bjwebb    (1000) bjwebb    (1000)        5 2024-05-29 21:51:26.000000 libcoveweb-0.30.3/libcoveweb.egg-info/top_level.txt
+-rwxrwxr-x   0 bjwebb    (1000) bjwebb    (1000)      247 2024-05-29 15:42:53.000000 libcoveweb-0.30.3/manage.py
+-rw-rw-r--   0 bjwebb    (1000) bjwebb    (1000)      147 2024-05-29 21:51:26.777771 libcoveweb-0.30.3/setup.cfg
+-rw-rw-r--   0 bjwebb    (1000) bjwebb    (1000)     1341 2024-05-29 15:43:16.000000 libcoveweb-0.30.3/setup.py
```

### Comparing `libcoveweb-0.30.2/README.md` & `libcoveweb-0.30.3/README.md`

 * *Files identical despite different names*

### Comparing `libcoveweb-0.30.2/cove/context_processors.py` & `libcoveweb-0.30.3/cove/context_processors.py`

 * *Files identical despite different names*

### Comparing `libcoveweb-0.30.2/cove/fixtures/badfile.json` & `libcoveweb-0.30.3/cove/fixtures/badfile.json`

 * *Files identical despite different names*

### Comparing `libcoveweb-0.30.2/cove/fixtures/basic.xlsx` & `libcoveweb-0.30.3/cove/fixtures/basic.xlsx`

 * *Files identical despite different names*

### Comparing `libcoveweb-0.30.2/cove/html_error_msg.py` & `libcoveweb-0.30.3/cove/html_error_msg.py`

 * *Files identical despite different names*

### Comparing `libcoveweb-0.30.2/cove/input/migrations/0001_initial.py` & `libcoveweb-0.30.3/cove/input/migrations/0001_initial.py`

 * *Files identical despite different names*

### Comparing `libcoveweb-0.30.2/cove/input/migrations/0003_auto_20150506_1649.py` & `libcoveweb-0.30.3/cove/input/migrations/0003_auto_20150506_1649.py`

 * *Files identical despite different names*

### Comparing `libcoveweb-0.30.2/cove/input/migrations/0007_supplied_data_schema_version.py` & `libcoveweb-0.30.3/cove/input/migrations/0007_supplied_data_schema_version.py`

 * *Files identical despite different names*

### Comparing `libcoveweb-0.30.2/cove/input/models.py` & `libcoveweb-0.30.3/cove/input/models.py`

 * *Files identical despite different names*

### Comparing `libcoveweb-0.30.2/cove/input/views.py` & `libcoveweb-0.30.3/cove/input/views.py`

 * *Files 2% similar despite different names*

```diff
@@ -72,14 +72,21 @@
             except TypeError:
                 pass
 
             data.save()
             if form_name == 'url_form':
                 try:
                     data.download()
+                except requests.InvalidURL as err:
+                    return render(request, 'error.html', context={
+                        'sub_title': _("That URL is invalid"),
+                        'link': 'index',
+                        'link_text': _('Try Again'),
+                        'msg': str(err)
+                    })
                 except requests.ConnectionError as err:
                     return render(request, 'error.html', context={
                         'sub_title': _("Sorry we got a ConnectionError whilst trying to download that file"),
                         'link': 'index',
                         'link_text': _('Try Again'),
                         'support_email': settings.COVE_CONFIG.get('support_email'),
                         'msg': str(err) + '\n\n' + str(_('Common reasons for this error include supplying a local '
```

### Comparing `libcoveweb-0.30.2/cove/lib/common.py` & `libcoveweb-0.30.3/cove/lib/common.py`

 * *Files identical despite different names*

### Comparing `libcoveweb-0.30.2/cove/locale/en/LC_MESSAGES/django.po` & `libcoveweb-0.30.3/cove/locale/en/LC_MESSAGES/django.po`

 * *Files 2% similar despite different names*

```diff
@@ -4,15 +4,15 @@
 # FIRST AUTHOR <EMAIL@ADDRESS>, YEAR.
 #
 #, fuzzy
 msgid ""
 msgstr ""
 "Project-Id-Version: PACKAGE VERSION\n"
 "Report-Msgid-Bugs-To: \n"
-"POT-Creation-Date: 2021-05-21 15:36+0000\n"
+"POT-Creation-Date: 2024-05-04 04:28+0000\n"
 "PO-Revision-Date: YEAR-MO-DA HO:MI+ZONE\n"
 "Last-Translator: FULL NAME <EMAIL@ADDRESS>\n"
 "Language-Team: LANGUAGE <LL@li.org>\n"
 "Language: \n"
 "MIME-Version: 1.0\n"
 "Content-Type: text/plain; charset=UTF-8\n"
 "Content-Transfer-Encoding: 8bit\n"
@@ -189,46 +189,50 @@
 #: cove/html_error_msg.py:225
 #, python-format
 msgid "%(extras)s does not match any of the regexes: %(patterns)s"
 msgid_plural "%(extras)s do not match any of the regexes: %(patterns)s"
 msgstr[0] ""
 msgstr[1] ""
 
-#: cove/input/views.py:18
+#: cove/input/views.py:19
 msgid "Upload a file (.json, .csv, .xlsx, .ods)"
 msgstr ""
 
-#: cove/input/views.py:27
+#: cove/input/views.py:28
 msgid "Supply a URL"
 msgstr ""
 
-#: cove/input/views.py:32
+#: cove/input/views.py:33
 msgid "Paste (JSON only)"
 msgstr ""
 
-#: cove/input/views.py:72
-msgid "Sorry we got a ConnectionError whilst trying to download that file"
+#: cove/input/views.py:81
+msgid "That URL is invalid"
 msgstr ""
 
-#: cove/input/views.py:74 cove/input/views.py:82 cove/views.py:28
-#: cove/views.py:39 cove/views.py:49
+#: cove/input/views.py:83 cove/input/views.py:90 cove/input/views.py:98
+#: cove/views.py:28 cove/views.py:39 cove/views.py:49
 msgid "Try Again"
 msgstr ""
 
-#: cove/input/views.py:75
+#: cove/input/views.py:88
+msgid "Sorry we got a ConnectionError whilst trying to download that file"
+msgstr ""
+
+#: cove/input/views.py:91
 msgid ""
 "Common reasons for this error include supplying a local development url that "
 "our servers can't access, or misconfigured SSL certificates."
 msgstr ""
 
-#: cove/input/views.py:80
+#: cove/input/views.py:96
 msgid "Sorry we got a HTTP Error whilst trying to download that file"
 msgstr ""
 
-#: cove/input/views.py:83
+#: cove/input/views.py:99
 msgid ""
 "If you can access the file through a browser then the problem may be related "
 "to permissions, or you may be blocking certain user agents."
 msgstr ""
 
 #: cove/templates/500.html:8
 msgid "Internal Server Error"
@@ -296,63 +300,63 @@
 
 #: cove/templates/additional_fields_table_all.html:46
 #, python-format
 msgid "Child fields of %(parent_full_path)s"
 msgstr ""
 
 #. Translators: Label of a button that triggers search
-#: cove/templates/base.html:55 cove/templates/page_header.html:27
+#: cove/templates/base.html:54 cove/templates/page_header.html:27
 msgid "Go"
 msgstr ""
 
-#: cove/templates/base.html:115
+#: cove/templates/base.html:114
 msgid "About"
 msgstr ""
 
-#: cove/templates/base.html:118
+#: cove/templates/base.html:117
 msgid "Built by"
 msgstr ""
 
-#: cove/templates/base.html:118
+#: cove/templates/base.html:117
 msgid "Open Data Services Co-operative"
 msgstr ""
 
-#: cove/templates/base.html:119
+#: cove/templates/base.html:118
 msgid "The code for this site is available on"
 msgstr ""
 
-#: cove/templates/base.html:119
+#: cove/templates/base.html:118
 msgid "GitHub"
 msgstr ""
 
-#: cove/templates/base.html:119
+#: cove/templates/base.html:118
 msgid "Cove - COnvert Validate & Explore"
 msgstr ""
 
-#: cove/templates/base.html:119
+#: cove/templates/base.html:118
 msgid "Licence"
 msgstr ""
 
-#: cove/templates/base.html:119
+#: cove/templates/base.html:118
 msgid "AGPLv3"
 msgstr ""
 
-#: cove/templates/base.html:119
+#: cove/templates/base.html:118
 msgid "Report/View issues"
 msgstr ""
 
-#: cove/templates/base.html:119
+#: cove/templates/base.html:118
 msgid "Cove Issues"
 msgstr ""
 
-#: cove/templates/base.html:124
+#: cove/templates/base.html:123
 msgid "Terms &amp; Conditions"
 msgstr ""
 
-#: cove/templates/base.html:133
+#: cove/templates/base.html:132
 msgid "Links"
 msgstr ""
 
 #: cove/templates/error_extra.html:2
 msgid ""
 "If you think this is a bug, you can <a href=\"https://github.com/"
 "OpenDataServices/cove/issues\">file an issue publicly on GitHub</a> or "
```

### Comparing `libcoveweb-0.30.2/cove/locale/es/LC_MESSAGES/django.mo` & `libcoveweb-0.30.3/cove/locale/es/LC_MESSAGES/django.mo`

 * *Files 5% similar despite different names*

#### msgunfmt {}

```diff
@@ -2,18 +2,18 @@
 msgstr ""
 "Project-Id-Version: PACKAGE VERSION\n"
 "Report-Msgid-Bugs-To: \n"
 "PO-Revision-Date: 2018-11-30 11:12+0000\n"
 "Last-Translator: Bibiana Cristòfol <bcristofol@gmail.com>, 2021\n"
 "Language-Team: Spanish (https://www.transifex.com/OpenDataServices/"
 "teams/59127/es/)\n"
+"Language: es\n"
 "MIME-Version: 1.0\n"
 "Content-Type: text/plain; charset=UTF-8\n"
 "Content-Transfer-Encoding: 8bit\n"
-"Language: es\n"
 "Plural-Forms: nplurals=2; plural=(n != 1);\n"
 
 msgid "%(each)s is a dependency of %(property)s"
 msgstr "%(each)s es una dependencia de %(property)s"
 
 msgid "%(extras)s does not match any of the regexes: %(patterns)s"
 msgid_plural "%(extras)s do not match any of the regexes: %(patterns)s"
@@ -324,14 +324,17 @@
 
 msgid "Supply a URL"
 msgstr "Proporcionar una dirección URL"
 
 msgid "Terms &amp; Conditions"
 msgstr "Términos y condiciones"
 
+msgid "That URL is invalid"
+msgstr "Esa URL no es válida"
+
 msgid "The code for this site is available on"
 msgstr "El código de este sitio está disponible en "
 
 msgid ""
 "The data you were hoping to explore no longer exists.\n"
 "\n"
 "This is because all data supplied to this website is automatically deleted "
```

### Comparing `libcoveweb-0.30.2/cove/locale/es/LC_MESSAGES/django.po` & `libcoveweb-0.30.3/cove/locale/es/LC_MESSAGES/django.po`

 * *Files 3% similar despite different names*

```diff
@@ -1,68 +1,69 @@
 # SOME DESCRIPTIVE TITLE.
 # Copyright (C) YEAR THE PACKAGE'S COPYRIGHT HOLDER
 # This file is distributed under the same license as the PACKAGE package.
 # FIRST AUTHOR <EMAIL@ADDRESS>, YEAR.
-# 
+#
 # Translators:
 # Eduardo Gomez <eduardo.gomez@hotmail.co.uk>, 2018
 # David Raznick <david.raznick@opendataservices.coop>, 2019
 # Yohanna Lisnichuk <ylisnichuk@open-contracting.org>, 2019
 # Cecilia Casco <ceciliacasco@cds.com.py>, 2021
 # Maria Esther Cervantes <mcervantes@cds.com.py>, 2021
 # Ben Webb <ben.webb@opendataservices.coop>, 2021
 # Bibiana Cristòfol <bcristofol@gmail.com>, 2021
-# 
+#
 #, fuzzy
 msgid ""
 msgstr ""
 "Project-Id-Version: PACKAGE VERSION\n"
 "Report-Msgid-Bugs-To: \n"
-"POT-Creation-Date: 2021-05-21 15:36+0000\n"
+"POT-Creation-Date: 2024-05-04 04:28+0000\n"
 "PO-Revision-Date: 2018-11-30 11:12+0000\n"
 "Last-Translator: Bibiana Cristòfol <bcristofol@gmail.com>, 2021\n"
-"Language-Team: Spanish (https://www.transifex.com/OpenDataServices/teams/59127/es/)\n"
+"Language-Team: Spanish (https://www.transifex.com/OpenDataServices/"
+"teams/59127/es/)\n"
+"Language: es\n"
 "MIME-Version: 1.0\n"
 "Content-Type: text/plain; charset=UTF-8\n"
 "Content-Transfer-Encoding: 8bit\n"
-"Language: es\n"
 "Plural-Forms: nplurals=2; plural=(n != 1);\n"
 
 #: cove/html_error_msg.py:22
 msgid "Date is not in the correct format"
 msgstr "El formato de la fecha es incorrecto"
 
 #: cove/html_error_msg.py:23
 msgid "Invalid 'uri' found"
 msgstr "Se ha encontrado una 'uri' inválida"
 
 #: cove/html_error_msg.py:24
 msgid ""
-"{}<code>{}</code> is not a string. Check that the value {} has quotes at the"
-" start and end. Escape any quotes in the value with <code>\\</code>"
+"{}<code>{}</code> is not a string. Check that the value {} has quotes at the "
+"start and end. Escape any quotes in the value with <code>\\</code>"
 msgstr ""
 "{}<code>{}</code> no es un hilo. Revise que el valor {} tenga comillas al "
-"principio y al final. Escapa de cualquier comillas con el valor "
-"<code>\\</code>"
+"principio y al final. Escapa de cualquier comillas con el valor <code>\\</"
+"code>"
 
 #: cove/html_error_msg.py:25
 msgid ""
 "{}<code>{}</code> is not a integer. Check that the value {} doesn’t contain "
 "decimal points or any characters other than 0-9. Integer values should not "
 "be in quotes. "
 msgstr ""
 "{}<code>{}</code> no es un entero. Compruebe que el valor {} no contenga "
-"puntos decimales ni ningún otro carácter que no sea 0-9. Los valores enteros"
-" no deben estar entre comillas."
+"puntos decimales ni ningún otro carácter que no sea 0-9. Los valores enteros "
+"no deben estar entre comillas."
 
 #: cove/html_error_msg.py:26
 msgid ""
 "{}<code>{}</code> is not a number. Check that the value {} doesn’t contain "
-"any characters other than 0-9 and dot (<code>.</code>). Number values should"
-" not be in quotes. "
+"any characters other than 0-9 and dot (<code>.</code>). Number values should "
+"not be in quotes. "
 msgstr ""
 "{}<code>{}</code> no es un número. Compruebe que el valor {} no contenga "
 "ningún carácter más que 0-9 y el punto (.). Los valores numéricos no deben "
 "estar entre comillas"
 
 #: cove/html_error_msg.py:27
 msgid "{}<code>{}</code> is not a JSON object"
@@ -203,70 +204,71 @@
 msgstr "Valores {} no únicos"
 
 #: cove/html_error_msg.py:217
 #, python-format
 msgid "Additional properties are not allowed (%s was unexpected)"
 msgid_plural "Additional properties are not allowed (%s were unexpected)"
 msgstr[0] "Propiedades adicionales no están permitidas (%s fue inesperado)"
-msgstr[1] ""
-"Propiedades adicionales no están permitidas (%s fueron inesperados)"
+msgstr[1] "Propiedades adicionales no están permitidas (%s fueron inesperados)"
 
 #: cove/html_error_msg.py:225
 #, python-format
 msgid "%(extras)s does not match any of the regexes: %(patterns)s"
 msgid_plural "%(extras)s do not match any of the regexes: %(patterns)s"
 msgstr[0] ""
-"%(extras)s no coincide con ninguna de las expresiones regulares: "
-"%(patterns)s"
+"%(extras)s no coincide con ninguna de las expresiones regulares: %(patterns)s"
 msgstr[1] ""
 "%(extras)s no coinciden con ninguna de las expresiones regulares: "
 "%(patterns)s"
 
-#: cove/input/views.py:18
+#: cove/input/views.py:19
 msgid "Upload a file (.json, .csv, .xlsx, .ods)"
 msgstr "Subir un archivo (.json, .csv, .xlsx, .ods)"
 
-#: cove/input/views.py:27
+#: cove/input/views.py:28
 msgid "Supply a URL"
 msgstr "Proporcionar una dirección URL"
 
-#: cove/input/views.py:32
+#: cove/input/views.py:33
 msgid "Paste (JSON only)"
 msgstr "Pegar (sólo JSON)"
 
-#: cove/input/views.py:72
+#: cove/input/views.py:81
+msgid "That URL is invalid"
+msgstr "Esa URL no es válida"
+
+#: cove/input/views.py:83 cove/input/views.py:90 cove/input/views.py:98
+#: cove/views.py:28 cove/views.py:39 cove/views.py:49
+msgid "Try Again"
+msgstr "Inténtelo de nuevo"
+
+#: cove/input/views.py:88
 msgid "Sorry we got a ConnectionError whilst trying to download that file"
 msgstr ""
 "Lo sentimos, al tratar de descargar el archivo hemos encontrado un "
 "ConnectionError"
 
-#: cove/input/views.py:74 cove/input/views.py:82 cove/views.py:28
-#: cove/views.py:39 cove/views.py:49
-msgid "Try Again"
-msgstr "Inténtelo de nuevo"
-
-#: cove/input/views.py:75
+#: cove/input/views.py:91
 msgid ""
-"Common reasons for this error include supplying a local development url that"
-" our servers can't access, or misconfigured SSL certificates."
+"Common reasons for this error include supplying a local development url that "
+"our servers can't access, or misconfigured SSL certificates."
 msgstr ""
 "Las razones comunes de este error incluyen el suministro de una URL de "
 "desarrollo local a la que nuestros servidores no pueden acceder o "
 "certificados SSL mal configurados."
 
-#: cove/input/views.py:80
+#: cove/input/views.py:96
 msgid "Sorry we got a HTTP Error whilst trying to download that file"
 msgstr ""
-"Lo sentimos, al tratar de descargar el archivo hemos encontrado un HTTP "
-"Error"
+"Lo sentimos, al tratar de descargar el archivo hemos encontrado un HTTP Error"
 
-#: cove/input/views.py:83
+#: cove/input/views.py:99
 msgid ""
-"If you can access the file through a browser then the problem may be related"
-" to permissions, or you may be blocking certain user agents."
+"If you can access the file through a browser then the problem may be related "
+"to permissions, or you may be blocking certain user agents."
 msgstr ""
 "Si no puede acceder al archivo a través del navegador entonces el problema "
 "puede esta relacionado con los permisos, o puede que este bloqueando a "
 "ciertos usuarios"
 
 #: cove/templates/500.html:8
 msgid "Internal Server Error"
@@ -338,75 +340,74 @@
 
 #: cove/templates/additional_fields_table_all.html:46
 #, python-format
 msgid "Child fields of %(parent_full_path)s"
 msgstr "Campos hijos de %(parent_full_path)s"
 
 #. Translators: Label of a button that triggers search
-#: cove/templates/base.html:55 cove/templates/page_header.html:27
+#: cove/templates/base.html:54 cove/templates/page_header.html:27
 msgid "Go"
 msgstr "Ir"
 
-#: cove/templates/base.html:115
+#: cove/templates/base.html:114
 msgid "About"
 msgstr "Acerca de"
 
-#: cove/templates/base.html:118
+#: cove/templates/base.html:117
 msgid "Built by"
 msgstr "Construido por "
 
-#: cove/templates/base.html:118
+#: cove/templates/base.html:117
 msgid "Open Data Services Co-operative"
 msgstr "Open Data Services Co-operative"
 
-#: cove/templates/base.html:119
+#: cove/templates/base.html:118
 msgid "The code for this site is available on"
 msgstr "El código de este sitio está disponible en "
 
-#: cove/templates/base.html:119
+#: cove/templates/base.html:118
 msgid "GitHub"
 msgstr "GitHub"
 
-#: cove/templates/base.html:119
+#: cove/templates/base.html:118
 msgid "Cove - COnvert Validate & Explore"
 msgstr "Cove - COnvert Validate & Explore"
 
-#: cove/templates/base.html:119
+#: cove/templates/base.html:118
 msgid "Licence"
 msgstr "Licencia"
 
-#: cove/templates/base.html:119
+#: cove/templates/base.html:118
 msgid "AGPLv3"
 msgstr "AGPLv3"
 
-#: cove/templates/base.html:119
+#: cove/templates/base.html:118
 msgid "Report/View issues"
 msgstr "Reportar / Ver issues"
 
-#: cove/templates/base.html:119
+#: cove/templates/base.html:118
 msgid "Cove Issues"
 msgstr "Issues del Cove"
 
-#: cove/templates/base.html:124
+#: cove/templates/base.html:123
 msgid "Terms &amp; Conditions"
 msgstr "Términos y condiciones"
 
-#: cove/templates/base.html:133
+#: cove/templates/base.html:132
 msgid "Links"
 msgstr "Enlaces"
 
 #: cove/templates/error_extra.html:2
 msgid ""
-"If you think this is a bug, you can <a "
-"href=\"https://github.com/OpenDataServices/cove/issues\">file an issue "
-"publicly on GitHub</a> or "
-msgstr ""
-"Si cree que esto es un error, puede <a "
-"href=\"https://github.com/OpenDataServices/cove/issues\">presentar un issue "
-"públicamente en GitHub</a> o"
+"If you think this is a bug, you can <a href=\"https://github.com/"
+"OpenDataServices/cove/issues\">file an issue publicly on GitHub</a> or "
+msgstr ""
+"Si cree que esto es un error, puede <a href=\"https://github.com/"
+"OpenDataServices/cove/issues\">presentar un issue públicamente en GitHub</a> "
+"o"
 
 #: cove/templates/error_extra.html:2
 msgid "get in touch via email"
 msgstr "póngase en contacto a través de correo electrónico "
 
 #: cove/templates/error_extra.html:2
 msgid "referencing this error as "
@@ -440,16 +441,15 @@
 msgid "Excel Spreadsheet (.xlsx) with titles"
 msgstr "Hoja de cálculo de Excel (.xlsx) con títulos"
 
 #: cove/templates/explore.html:17
 msgid "OpenDocument Spreadsheet (.ods) with titles"
 msgstr "Hoja de cálculo de OpenDocument (.ods) con títulos"
 
-#. Translators: JSON probably does not need a transalation:
-#. http://www.json.org/
+#. Translators: JSON probably does not need a transalation: http://www.json.org/
 #: cove/templates/explore.html:19
 msgid "JSON"
 msgstr "JSON"
 
 #: cove/templates/explore.html:20
 msgid "XML"
 msgstr "XML"
@@ -581,15 +581,16 @@
 
 #: cove/views.py:30
 msgid ""
 "We think you tried to upload a JSON file, but it is not well formed JSON.\n"
 "\n"
 "Error message: {}"
 msgstr ""
-"Creemos que ha intentado subir un archivo JSON, pero el archivo no es JSON bien formado.\n"
+"Creemos que ha intentado subir un archivo JSON, pero el archivo no es JSON "
+"bien formado.\n"
 "\n"
 "Mensaje del error: {}"
 
 #: cove/views.py:41
 msgid ""
 "We did not recognise the file type.\n"
 "\n"
@@ -601,15 +602,16 @@
 
 #: cove/views.py:51
 msgid ""
 "We think you tried to supply a spreadsheet, but we failed to convert it.\n"
 "\n"
 "Error message: {}"
 msgstr ""
-"Creemos que ha tratado de suministrar una hoja de cálculo, pero no hemos podido convertirla.\n"
+"Creemos que ha tratado de suministrar una hoja de cálculo, pero no hemos "
+"podido convertirla.\n"
 "\n"
 "Mensaje del error: {}"
 
 #: cove/views.py:75 cove/views.py:87
 msgid "Sorry, the page you are looking for is not available"
 msgstr "Lo sentimos, la página que está buscando no está disponible"
 
@@ -621,12 +623,15 @@
 msgid "We don't seem to be able to find the data you requested."
 msgstr "Parece que no podemos encontrar los datos que usted solicitó."
 
 #: cove/views.py:90
 msgid ""
 "The data you were hoping to explore no longer exists.\n"
 "\n"
-"This is because all data supplied to this website is automatically deleted after 7 days, and therefore the analysis of that data is no longer available."
+"This is because all data supplied to this website is automatically deleted "
+"after 7 days, and therefore the analysis of that data is no longer available."
 msgstr ""
 "Los datos que usted quería explorar ya no existen.\n"
 "\n"
-"Esto se debe a que todos los datos suministrados a este sitio web se borran automáticamente después de 7 días, y por lo tanto el análisis de esos datos ya no está disponible."
+"Esto se debe a que todos los datos suministrados a este sitio web se borran "
+"automáticamente después de 7 días, y por lo tanto el análisis de esos datos "
+"ya no está disponible."
```

### Comparing `libcoveweb-0.30.2/cove/management/commands/base_command.py` & `libcoveweb-0.30.3/cove/management/commands/base_command.py`

 * *Files identical despite different names*

### Comparing `libcoveweb-0.30.2/cove/management/commands/expire_files.py` & `libcoveweb-0.30.3/cove/management/commands/expire_files.py`

 * *Files identical despite different names*

### Comparing `libcoveweb-0.30.2/cove/management/commands/tests.py` & `libcoveweb-0.30.3/cove/management/commands/tests.py`

 * *Files identical despite different names*

### Comparing `libcoveweb-0.30.2/cove/management/commands/upload.py` & `libcoveweb-0.30.3/cove/management/commands/upload.py`

 * *Files identical despite different names*

### Comparing `libcoveweb-0.30.2/cove/sass/bootstrap/_bootstrap-mincer.scss` & `libcoveweb-0.30.3/cove/sass/bootstrap/_bootstrap-mincer.scss`

 * *Files identical despite different names*

### Comparing `libcoveweb-0.30.2/cove/sass/bootstrap/_bootstrap.scss` & `libcoveweb-0.30.3/cove/sass/bootstrap/_bootstrap.scss`

 * *Files identical despite different names*

### Comparing `libcoveweb-0.30.2/cove/sass/bootstrap/bootstrap/_alerts.scss` & `libcoveweb-0.30.3/cove/sass/bootstrap/bootstrap/_alerts.scss`

 * *Files identical despite different names*

### Comparing `libcoveweb-0.30.2/cove/sass/bootstrap/bootstrap/_badges.scss` & `libcoveweb-0.30.3/cove/sass/bootstrap/bootstrap/_badges.scss`

 * *Files identical despite different names*

### Comparing `libcoveweb-0.30.2/cove/sass/bootstrap/bootstrap/_breadcrumbs.scss` & `libcoveweb-0.30.3/cove/sass/bootstrap/bootstrap/_breadcrumbs.scss`

 * *Files identical despite different names*

### Comparing `libcoveweb-0.30.2/cove/sass/bootstrap/bootstrap/_button-groups.scss` & `libcoveweb-0.30.3/cove/sass/bootstrap/bootstrap/_button-groups.scss`

 * *Files identical despite different names*

### Comparing `libcoveweb-0.30.2/cove/sass/bootstrap/bootstrap/_buttons.scss` & `libcoveweb-0.30.3/cove/sass/bootstrap/bootstrap/_buttons.scss`

 * *Files identical despite different names*

### Comparing `libcoveweb-0.30.2/cove/sass/bootstrap/bootstrap/_carousel.scss` & `libcoveweb-0.30.3/cove/sass/bootstrap/bootstrap/_carousel.scss`

 * *Files identical despite different names*

### Comparing `libcoveweb-0.30.2/cove/sass/bootstrap/bootstrap/_close.scss` & `libcoveweb-0.30.3/cove/sass/bootstrap/bootstrap/_close.scss`

 * *Files identical despite different names*

### Comparing `libcoveweb-0.30.2/cove/sass/bootstrap/bootstrap/_code.scss` & `libcoveweb-0.30.3/cove/sass/bootstrap/bootstrap/_code.scss`

 * *Files identical despite different names*

### Comparing `libcoveweb-0.30.2/cove/sass/bootstrap/bootstrap/_component-animations.scss` & `libcoveweb-0.30.3/cove/sass/bootstrap/bootstrap/_component-animations.scss`

 * *Files identical despite different names*

### Comparing `libcoveweb-0.30.2/cove/sass/bootstrap/bootstrap/_dropdowns.scss` & `libcoveweb-0.30.3/cove/sass/bootstrap/bootstrap/_dropdowns.scss`

 * *Files identical despite different names*

### Comparing `libcoveweb-0.30.2/cove/sass/bootstrap/bootstrap/_forms.scss` & `libcoveweb-0.30.3/cove/sass/bootstrap/bootstrap/_forms.scss`

 * *Files identical despite different names*

### Comparing `libcoveweb-0.30.2/cove/sass/bootstrap/bootstrap/_glyphicons.scss` & `libcoveweb-0.30.3/cove/sass/bootstrap/bootstrap/_glyphicons.scss`

 * *Files identical despite different names*

### Comparing `libcoveweb-0.30.2/cove/sass/bootstrap/bootstrap/_grid.scss` & `libcoveweb-0.30.3/cove/sass/bootstrap/bootstrap/_grid.scss`

 * *Files identical despite different names*

### Comparing `libcoveweb-0.30.2/cove/sass/bootstrap/bootstrap/_input-groups.scss` & `libcoveweb-0.30.3/cove/sass/bootstrap/bootstrap/_input-groups.scss`

 * *Files identical despite different names*

### Comparing `libcoveweb-0.30.2/cove/sass/bootstrap/bootstrap/_jumbotron.scss` & `libcoveweb-0.30.3/cove/sass/bootstrap/bootstrap/_jumbotron.scss`

 * *Files identical despite different names*

### Comparing `libcoveweb-0.30.2/cove/sass/bootstrap/bootstrap/_labels.scss` & `libcoveweb-0.30.3/cove/sass/bootstrap/bootstrap/_labels.scss`

 * *Files identical despite different names*

### Comparing `libcoveweb-0.30.2/cove/sass/bootstrap/bootstrap/_list-group.scss` & `libcoveweb-0.30.3/cove/sass/bootstrap/bootstrap/_list-group.scss`

 * *Files identical despite different names*

### Comparing `libcoveweb-0.30.2/cove/sass/bootstrap/bootstrap/_media.scss` & `libcoveweb-0.30.3/cove/sass/bootstrap/bootstrap/_media.scss`

 * *Files identical despite different names*

### Comparing `libcoveweb-0.30.2/cove/sass/bootstrap/bootstrap/_mixins.scss` & `libcoveweb-0.30.3/cove/sass/bootstrap/bootstrap/_mixins.scss`

 * *Files identical despite different names*

### Comparing `libcoveweb-0.30.2/cove/sass/bootstrap/bootstrap/_modals.scss` & `libcoveweb-0.30.3/cove/sass/bootstrap/bootstrap/_modals.scss`

 * *Files identical despite different names*

### Comparing `libcoveweb-0.30.2/cove/sass/bootstrap/bootstrap/_navbar.scss` & `libcoveweb-0.30.3/cove/sass/bootstrap/bootstrap/_navbar.scss`

 * *Files identical despite different names*

### Comparing `libcoveweb-0.30.2/cove/sass/bootstrap/bootstrap/_navs.scss` & `libcoveweb-0.30.3/cove/sass/bootstrap/bootstrap/_navs.scss`

 * *Files identical despite different names*

### Comparing `libcoveweb-0.30.2/cove/sass/bootstrap/bootstrap/_normalize.scss` & `libcoveweb-0.30.3/cove/sass/bootstrap/bootstrap/_normalize.scss`

 * *Files identical despite different names*

### Comparing `libcoveweb-0.30.2/cove/sass/bootstrap/bootstrap/_pager.scss` & `libcoveweb-0.30.3/cove/sass/bootstrap/bootstrap/_pager.scss`

 * *Files identical despite different names*

### Comparing `libcoveweb-0.30.2/cove/sass/bootstrap/bootstrap/_pagination.scss` & `libcoveweb-0.30.3/cove/sass/bootstrap/bootstrap/_pagination.scss`

 * *Files identical despite different names*

### Comparing `libcoveweb-0.30.2/cove/sass/bootstrap/bootstrap/_panels.scss` & `libcoveweb-0.30.3/cove/sass/bootstrap/bootstrap/_panels.scss`

 * *Files identical despite different names*

### Comparing `libcoveweb-0.30.2/cove/sass/bootstrap/bootstrap/_popovers.scss` & `libcoveweb-0.30.3/cove/sass/bootstrap/bootstrap/_popovers.scss`

 * *Files identical despite different names*

### Comparing `libcoveweb-0.30.2/cove/sass/bootstrap/bootstrap/_print.scss` & `libcoveweb-0.30.3/cove/sass/bootstrap/bootstrap/_print.scss`

 * *Files identical despite different names*

### Comparing `libcoveweb-0.30.2/cove/sass/bootstrap/bootstrap/_progress-bars.scss` & `libcoveweb-0.30.3/cove/sass/bootstrap/bootstrap/_progress-bars.scss`

 * *Files identical despite different names*

### Comparing `libcoveweb-0.30.2/cove/sass/bootstrap/bootstrap/_responsive-embed.scss` & `libcoveweb-0.30.3/cove/sass/bootstrap/bootstrap/_responsive-embed.scss`

 * *Files identical despite different names*

### Comparing `libcoveweb-0.30.2/cove/sass/bootstrap/bootstrap/_responsive-utilities.scss` & `libcoveweb-0.30.3/cove/sass/bootstrap/bootstrap/_responsive-utilities.scss`

 * *Files identical despite different names*

### Comparing `libcoveweb-0.30.2/cove/sass/bootstrap/bootstrap/_scaffolding.scss` & `libcoveweb-0.30.3/cove/sass/bootstrap/bootstrap/_scaffolding.scss`

 * *Files identical despite different names*

### Comparing `libcoveweb-0.30.2/cove/sass/bootstrap/bootstrap/_tables.scss` & `libcoveweb-0.30.3/cove/sass/bootstrap/bootstrap/_tables.scss`

 * *Files identical despite different names*

### Comparing `libcoveweb-0.30.2/cove/sass/bootstrap/bootstrap/_theme.scss` & `libcoveweb-0.30.3/cove/sass/bootstrap/bootstrap/_theme.scss`

 * *Files identical despite different names*

### Comparing `libcoveweb-0.30.2/cove/sass/bootstrap/bootstrap/_thumbnails.scss` & `libcoveweb-0.30.3/cove/sass/bootstrap/bootstrap/_thumbnails.scss`

 * *Files identical despite different names*

### Comparing `libcoveweb-0.30.2/cove/sass/bootstrap/bootstrap/_tooltip.scss` & `libcoveweb-0.30.3/cove/sass/bootstrap/bootstrap/_tooltip.scss`

 * *Files identical despite different names*

### Comparing `libcoveweb-0.30.2/cove/sass/bootstrap/bootstrap/_type.scss` & `libcoveweb-0.30.3/cove/sass/bootstrap/bootstrap/_type.scss`

 * *Files identical despite different names*

### Comparing `libcoveweb-0.30.2/cove/sass/bootstrap/bootstrap/_utilities.scss` & `libcoveweb-0.30.3/cove/sass/bootstrap/bootstrap/_utilities.scss`

 * *Files identical despite different names*

### Comparing `libcoveweb-0.30.2/cove/sass/bootstrap/bootstrap/_variables.scss` & `libcoveweb-0.30.3/cove/sass/bootstrap/bootstrap/_variables.scss`

 * *Files identical despite different names*

### Comparing `libcoveweb-0.30.2/cove/sass/bootstrap/bootstrap/_wells.scss` & `libcoveweb-0.30.3/cove/sass/bootstrap/bootstrap/_wells.scss`

 * *Files identical despite different names*

### Comparing `libcoveweb-0.30.2/cove/sass/bootstrap/bootstrap/mixins/_buttons.scss` & `libcoveweb-0.30.3/cove/sass/bootstrap/bootstrap/mixins/_buttons.scss`

 * *Files identical despite different names*

### Comparing `libcoveweb-0.30.2/cove/sass/bootstrap/bootstrap/mixins/_clearfix.scss` & `libcoveweb-0.30.3/cove/sass/bootstrap/bootstrap/mixins/_clearfix.scss`

 * *Files identical despite different names*

### Comparing `libcoveweb-0.30.2/cove/sass/bootstrap/bootstrap/mixins/_forms.scss` & `libcoveweb-0.30.3/cove/sass/bootstrap/bootstrap/mixins/_forms.scss`

 * *Files identical despite different names*

### Comparing `libcoveweb-0.30.2/cove/sass/bootstrap/bootstrap/mixins/_gradients.scss` & `libcoveweb-0.30.3/cove/sass/bootstrap/bootstrap/mixins/_gradients.scss`

 * *Files identical despite different names*

### Comparing `libcoveweb-0.30.2/cove/sass/bootstrap/bootstrap/mixins/_grid-framework.scss` & `libcoveweb-0.30.3/cove/sass/bootstrap/bootstrap/mixins/_grid-framework.scss`

 * *Files identical despite different names*

### Comparing `libcoveweb-0.30.2/cove/sass/bootstrap/bootstrap/mixins/_grid.scss` & `libcoveweb-0.30.3/cove/sass/bootstrap/bootstrap/mixins/_grid.scss`

 * *Files identical despite different names*

### Comparing `libcoveweb-0.30.2/cove/sass/bootstrap/bootstrap/mixins/_hide-text.scss` & `libcoveweb-0.30.3/cove/sass/bootstrap/bootstrap/mixins/_hide-text.scss`

 * *Files identical despite different names*

### Comparing `libcoveweb-0.30.2/cove/sass/bootstrap/bootstrap/mixins/_image.scss` & `libcoveweb-0.30.3/cove/sass/bootstrap/bootstrap/mixins/_image.scss`

 * *Files identical despite different names*

### Comparing `libcoveweb-0.30.2/cove/sass/bootstrap/bootstrap/mixins/_list-group.scss` & `libcoveweb-0.30.3/cove/sass/bootstrap/bootstrap/mixins/_list-group.scss`

 * *Files identical despite different names*

### Comparing `libcoveweb-0.30.2/cove/sass/bootstrap/bootstrap/mixins/_panels.scss` & `libcoveweb-0.30.3/cove/sass/bootstrap/bootstrap/mixins/_panels.scss`

 * *Files identical despite different names*

### Comparing `libcoveweb-0.30.2/cove/sass/bootstrap/bootstrap/mixins/_responsive-visibility.scss` & `libcoveweb-0.30.3/cove/sass/bootstrap/bootstrap/mixins/_responsive-visibility.scss`

 * *Files identical despite different names*

### Comparing `libcoveweb-0.30.2/cove/sass/bootstrap/bootstrap/mixins/_table-row.scss` & `libcoveweb-0.30.3/cove/sass/bootstrap/bootstrap/mixins/_table-row.scss`

 * *Files identical despite different names*

### Comparing `libcoveweb-0.30.2/cove/sass/bootstrap/bootstrap/mixins/_vendor-prefixes.scss` & `libcoveweb-0.30.3/cove/sass/bootstrap/bootstrap/mixins/_vendor-prefixes.scss`

 * *Files identical despite different names*

### Comparing `libcoveweb-0.30.2/cove/settings.py` & `libcoveweb-0.30.3/cove/settings.py`

 * *Files identical despite different names*

### Comparing `libcoveweb-0.30.2/cove/static/dataexplore/css/style.css` & `libcoveweb-0.30.3/cove/static/dataexplore/css/style.css`

 * *Files identical despite different names*

### Comparing `libcoveweb-0.30.2/cove/static/dataexplore/fonts/bootstrap/glyphicons-halflings-regular.eot` & `libcoveweb-0.30.3/cove/static/dataexplore/fonts/bootstrap/glyphicons-halflings-regular.eot`

 * *Files identical despite different names*

### Comparing `libcoveweb-0.30.2/cove/static/dataexplore/fonts/bootstrap/glyphicons-halflings-regular.svg` & `libcoveweb-0.30.3/cove/static/dataexplore/fonts/bootstrap/glyphicons-halflings-regular.svg`

 * *Files identical despite different names*

### Comparing `libcoveweb-0.30.2/cove/static/dataexplore/fonts/bootstrap/glyphicons-halflings-regular.ttf` & `libcoveweb-0.30.3/cove/static/dataexplore/fonts/bootstrap/glyphicons-halflings-regular.ttf`

 * *Files identical despite different names*

### Comparing `libcoveweb-0.30.2/cove/static/dataexplore/fonts/bootstrap/glyphicons-halflings-regular.woff` & `libcoveweb-0.30.3/cove/static/dataexplore/fonts/bootstrap/glyphicons-halflings-regular.woff`

 * *Files identical despite different names*

### Comparing `libcoveweb-0.30.2/cove/static/dataexplore/fonts/bootstrap/glyphicons-halflings-regular.woff2` & `libcoveweb-0.30.3/cove/static/dataexplore/fonts/bootstrap/glyphicons-halflings-regular.woff2`

 * *Files identical despite different names*

### Comparing `libcoveweb-0.30.2/cove/static/dataexplore/fonts/tick/tick.eot` & `libcoveweb-0.30.3/cove/static/dataexplore/fonts/tick/tick.eot`

 * *Files identical despite different names*

### Comparing `libcoveweb-0.30.2/cove/static/dataexplore/fonts/tick/tick.svg` & `libcoveweb-0.30.3/cove/static/dataexplore/fonts/tick/tick.svg`

 * *Files identical despite different names*

### Comparing `libcoveweb-0.30.2/cove/static/dataexplore/fonts/tick/tick.ttf` & `libcoveweb-0.30.3/cove/static/dataexplore/fonts/tick/tick.ttf`

 * *Files identical despite different names*

### Comparing `libcoveweb-0.30.2/cove/static/dataexplore/fonts/tick/tick.woff` & `libcoveweb-0.30.3/cove/static/dataexplore/fonts/tick/tick.woff`

 * *Files identical despite different names*

### Comparing `libcoveweb-0.30.2/cove/static/dataexplore/fonts/tick/tick.woff2` & `libcoveweb-0.30.3/cove/static/dataexplore/fonts/tick/tick.woff2`

 * *Files identical despite different names*

### Comparing `libcoveweb-0.30.2/cove/templates/500.html` & `libcoveweb-0.30.3/cove/templates/500.html`

 * *Files identical despite different names*

### Comparing `libcoveweb-0.30.2/cove/templates/additional_codelist_values.html` & `libcoveweb-0.30.3/cove/templates/additional_codelist_values.html`

 * *Files identical despite different names*

### Comparing `libcoveweb-0.30.2/cove/templates/additional_fields_table_all.html` & `libcoveweb-0.30.3/cove/templates/additional_fields_table_all.html`

 * *Files identical despite different names*

### Comparing `libcoveweb-0.30.2/cove/templates/base.html` & `libcoveweb-0.30.3/cove/templates/base.html`

 * *Files identical despite different names*

### Comparing `libcoveweb-0.30.2/cove/templates/error.html` & `libcoveweb-0.30.3/cove/templates/error.html`

 * *Files identical despite different names*

### Comparing `libcoveweb-0.30.2/cove/templates/explore.html` & `libcoveweb-0.30.3/cove/templates/explore.html`

 * *Files identical despite different names*

### Comparing `libcoveweb-0.30.2/cove/templates/input.html` & `libcoveweb-0.30.3/cove/templates/input.html`

 * *Files identical despite different names*

### Comparing `libcoveweb-0.30.2/cove/templates/modal_errors.html` & `libcoveweb-0.30.3/cove/templates/modal_errors.html`

 * *Files identical despite different names*

### Comparing `libcoveweb-0.30.2/cove/templates/modal_list.html` & `libcoveweb-0.30.3/cove/templates/modal_list.html`

 * *Files identical despite different names*

### Comparing `libcoveweb-0.30.2/cove/templates/page_header.html` & `libcoveweb-0.30.3/cove/templates/page_header.html`

 * *Files identical despite different names*

### Comparing `libcoveweb-0.30.2/cove/templates/piwik.html` & `libcoveweb-0.30.3/cove/templates/piwik.html`

 * *Files identical despite different names*

### Comparing `libcoveweb-0.30.2/cove/templates/stats.html` & `libcoveweb-0.30.3/cove/templates/stats.html`

 * *Files identical despite different names*

### Comparing `libcoveweb-0.30.2/cove/templates/terms.html` & `libcoveweb-0.30.3/cove/templates/terms.html`

 * *Files identical despite different names*

### Comparing `libcoveweb-0.30.2/cove/templates/terms_conditions.html` & `libcoveweb-0.30.3/cove/templates/terms_conditions.html`

 * *Files identical despite different names*

### Comparing `libcoveweb-0.30.2/cove/templates/terms_conditions_intro.html` & `libcoveweb-0.30.3/cove/templates/terms_conditions_intro.html`

 * *Files identical despite different names*

### Comparing `libcoveweb-0.30.2/cove/templates/terms_cookies.html` & `libcoveweb-0.30.3/cove/templates/terms_cookies.html`

 * *Files identical despite different names*

### Comparing `libcoveweb-0.30.2/cove/templates/terms_data_deleting.html` & `libcoveweb-0.30.3/cove/templates/terms_data_deleting.html`

 * *Files identical despite different names*

### Comparing `libcoveweb-0.30.2/cove/templates/terms_data_uploaded.html` & `libcoveweb-0.30.3/cove/templates/terms_data_uploaded.html`

 * *Files identical despite different names*

### Comparing `libcoveweb-0.30.2/cove/templates/terms_disclaimer.html` & `libcoveweb-0.30.3/cove/templates/terms_disclaimer.html`

 * *Files identical despite different names*

### Comparing `libcoveweb-0.30.2/cove/templates/terms_links.html` & `libcoveweb-0.30.3/cove/templates/terms_links.html`

 * *Files identical despite different names*

### Comparing `libcoveweb-0.30.2/cove/templates/terms_privacy.html` & `libcoveweb-0.30.3/cove/templates/terms_privacy.html`

 * *Files identical despite different names*

### Comparing `libcoveweb-0.30.2/cove/templates/terms_privacy_intro.html` & `libcoveweb-0.30.3/cove/templates/terms_privacy_intro.html`

 * *Files identical despite different names*

### Comparing `libcoveweb-0.30.2/cove/templates/terms_tracker_google_analytics.html` & `libcoveweb-0.30.3/cove/templates/terms_tracker_google_analytics.html`

 * *Files identical despite different names*

### Comparing `libcoveweb-0.30.2/cove/templates/terms_tracker_matmo.html` & `libcoveweb-0.30.3/cove/templates/terms_tracker_matmo.html`

 * *Files identical despite different names*

### Comparing `libcoveweb-0.30.2/cove/templates/terms_tracker_sentry.html` & `libcoveweb-0.30.3/cove/templates/terms_tracker_sentry.html`

 * *Files identical despite different names*

### Comparing `libcoveweb-0.30.2/cove/templates/terms_tracker_server.html` & `libcoveweb-0.30.3/cove/templates/terms_tracker_server.html`

 * *Files identical despite different names*

### Comparing `libcoveweb-0.30.2/cove/templates/validation_table.html` & `libcoveweb-0.30.3/cove/templates/validation_table.html`

 * *Files identical despite different names*

### Comparing `libcoveweb-0.30.2/cove/templatetags/cove_tags.py` & `libcoveweb-0.30.3/cove/templatetags/cove_tags.py`

 * *Files identical despite different names*

### Comparing `libcoveweb-0.30.2/cove/tests.py` & `libcoveweb-0.30.3/cove/tests.py`

 * *Files identical despite different names*

### Comparing `libcoveweb-0.30.2/cove/urls.py` & `libcoveweb-0.30.3/cove/urls.py`

 * *Files identical despite different names*

### Comparing `libcoveweb-0.30.2/cove/views.py` & `libcoveweb-0.30.3/cove/views.py`

 * *Files identical despite different names*

### Comparing `libcoveweb-0.30.2/libcoveweb.egg-info/SOURCES.txt` & `libcoveweb-0.30.3/libcoveweb.egg-info/SOURCES.txt`

 * *Files 0% similar despite different names*

```diff
@@ -1,7 +1,8 @@
+LICENCE.rst
 README.md
 manage.py
 setup.cfg
 setup.py
 cove/__init__.py
 cove/context_processors.py
 cove/html_error_msg.py
```

### Comparing `libcoveweb-0.30.2/setup.py` & `libcoveweb-0.30.3/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 from setuptools import setup, find_packages
 
 install_requires = []
 
 setup(
     name='libcoveweb',
-    version='0.30.2',
+    version='0.30.3',
     author='Open Data Services',
     author_email='code@opendataservices.coop',
     packages=find_packages(),
     package_data={
         'cove': [
             'fixtures/*',
             'locale/*/*/*.po',
```

