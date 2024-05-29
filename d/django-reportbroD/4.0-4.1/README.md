# Comparing `tmp/django-reportbroD-4.0.tar.gz` & `tmp/django_reportbrod-4.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "django-reportbroD-4.0.tar", last modified: Wed May 22 15:14:56 2024, max compression
+gzip compressed data, was "django_reportbrod-4.1.tar", last modified: Wed May 29 14:03:36 2024, max compression
```

## Comparing `django-reportbroD-4.0.tar` & `django_reportbrod-4.1.tar`

### file list

```diff
@@ -1,185 +1,185 @@
-drwxr-xr-x   0 rider     (1000) rider     (1000)        0 2024-05-22 15:14:56.977805 django-reportbroD-4.0/
--rw-r--r--   0 rider     (1000) rider     (1000)      176 2024-05-22 11:02:56.000000 django-reportbroD-4.0/MANIFEST.in
--rw-r--r--   0 rider     (1000) rider     (1000)     5861 2024-05-22 15:14:56.977805 django-reportbroD-4.0/PKG-INFO
--rw-r--r--   0 rider     (1000) rider     (1000)     4803 2024-05-22 15:12:16.000000 django-reportbroD-4.0/README.md
-drwxr-xr-x   0 rider     (1000) rider     (1000)        0 2024-05-22 15:14:56.894470 django-reportbroD-4.0/django_reportbroD/
--rw-r--r--   0 rider     (1000) rider     (1000)        0 2024-02-16 20:55:14.000000 django-reportbroD-4.0/django_reportbroD/__init__.py
--rw-r--r--   0 rider     (1000) rider     (1000)      164 2024-02-18 03:27:34.000000 django-reportbroD-4.0/django_reportbroD/admin.py
--rw-r--r--   0 rider     (1000) rider     (1000)      189 2024-05-20 13:44:27.000000 django-reportbroD-4.0/django_reportbroD/apps.py
--rw-r--r--   0 rider     (1000) rider     (1000)      803 2024-05-01 16:21:02.000000 django-reportbroD-4.0/django_reportbroD/base.py
--rw-r--r--   0 rider     (1000) rider     (1000)      865 2024-05-17 14:51:48.000000 django-reportbroD-4.0/django_reportbroD/forms.py
-drwxr-xr-x   0 rider     (1000) rider     (1000)        0 2024-05-22 15:14:56.887803 django-reportbroD-4.0/django_reportbroD/locale/
-drwxr-xr-x   0 rider     (1000) rider     (1000)        0 2024-05-22 15:14:56.887803 django-reportbroD-4.0/django_reportbroD/locale/en/
-drwxr-xr-x   0 rider     (1000) rider     (1000)        0 2024-05-22 15:14:56.894470 django-reportbroD-4.0/django_reportbroD/locale/en/LC_MESSAGES/
--rw-r--r--   0 rider     (1000) rider     (1000)     9709 2024-05-22 11:17:28.000000 django-reportbroD-4.0/django_reportbroD/locale/en/LC_MESSAGES/django.mo
--rw-r--r--   0 rider     (1000) rider     (1000)     9997 2024-05-22 11:17:28.000000 django-reportbroD-4.0/django_reportbroD/locale/en/LC_MESSAGES/django.po
-drwxr-xr-x   0 rider     (1000) rider     (1000)        0 2024-05-22 15:14:56.887803 django-reportbroD-4.0/django_reportbroD/locale/es/
-drwxr-xr-x   0 rider     (1000) rider     (1000)        0 2024-05-22 15:14:56.894470 django-reportbroD-4.0/django_reportbroD/locale/es/LC_MESSAGES/
--rw-r--r--   0 rider     (1000) rider     (1000)    10561 2024-05-20 12:40:39.000000 django-reportbroD-4.0/django_reportbroD/locale/es/LC_MESSAGES/django.mo
--rw-r--r--   0 rider     (1000) rider     (1000)    10852 2024-05-19 00:43:40.000000 django-reportbroD-4.0/django_reportbroD/locale/es/LC_MESSAGES/django.po
--rw-r--r--   0 rider     (1000) rider     (1000)     1123 2024-05-19 02:27:08.000000 django-reportbroD-4.0/django_reportbroD/menus.py
-drwxr-xr-x   0 rider     (1000) rider     (1000)        0 2024-05-22 15:14:56.897803 django-reportbroD-4.0/django_reportbroD/migrations/
--rw-r--r--   0 rider     (1000) rider     (1000)     1737 2024-05-15 13:06:40.000000 django-reportbroD-4.0/django_reportbroD/migrations/0001_initial.py
--rw-r--r--   0 rider     (1000) rider     (1000)        0 2024-02-16 20:55:14.000000 django-reportbroD-4.0/django_reportbroD/migrations/__init__.py
--rw-r--r--   0 rider     (1000) rider     (1000)     1883 2024-05-13 14:18:14.000000 django-reportbroD-4.0/django_reportbroD/models.py
--rw-r--r--   0 rider     (1000) rider     (1000)    13459 2024-05-09 20:40:36.000000 django-reportbroD-4.0/django_reportbroD/reportcore.py
-drwxr-xr-x   0 rider     (1000) rider     (1000)        0 2024-05-22 15:14:56.887803 django-reportbroD-4.0/django_reportbroD/static/
-drwxr-xr-x   0 rider     (1000) rider     (1000)        0 2024-05-22 15:14:56.887803 django-reportbroD-4.0/django_reportbroD/static/assets/
-drwxr-xr-x   0 rider     (1000) rider     (1000)        0 2024-05-22 15:14:56.897803 django-reportbroD-4.0/django_reportbroD/static/assets/css/
--rw-r--r--   0 rider     (1000) rider     (1000)     1772 2019-03-30 20:18:02.000000 django-reportbroD-4.0/django_reportbroD/static/assets/css/mCSB_buttons.html
--rw-r--r--   0 rider     (1000) rider     (1000)     1772 2019-03-30 20:18:02.000000 django-reportbroD-4.0/django_reportbroD/static/assets/css/owl.video.play.html
--rw-r--r--   0 rider     (1000) rider     (1000)   509223 2019-03-30 20:18:10.000000 django-reportbroD-4.0/django_reportbroD/static/assets/css/style.css
--rw-r--r--   0 rider     (1000) rider     (1000)   236692 2024-05-05 16:55:58.000000 django-reportbroD-4.0/django_reportbroD/static/assets/css/vendors.css
-drwxr-xr-x   0 rider     (1000) rider     (1000)        0 2024-05-22 15:14:56.931137 django-reportbroD-4.0/django_reportbroD/static/assets/fonts/
--rw-r--r--   0 rider     (1000) rider     (1000)    62984 2019-03-30 20:18:20.000000 django-reportbroD-4.0/django_reportbroD/static/assets/fonts/cryptocurrency-icons.eot
--rw-r--r--   0 rider     (1000) rider     (1000)    24288 2019-03-30 20:18:20.000000 django-reportbroD-4.0/django_reportbroD/static/assets/fonts/cryptocurrency-icons.html
--rw-r--r--   0 rider     (1000) rider     (1000)   351196 2019-03-30 20:18:20.000000 django-reportbroD-4.0/django_reportbroD/static/assets/fonts/cryptocurrency-icons.svg
--rw-r--r--   0 rider     (1000) rider     (1000)    62768 2019-03-30 20:18:20.000000 django-reportbroD-4.0/django_reportbroD/static/assets/fonts/cryptocurrency-icons.ttf
--rw-r--r--   0 rider     (1000) rider     (1000)    31064 2019-03-30 20:18:20.000000 django-reportbroD-4.0/django_reportbroD/static/assets/fonts/cryptocurrency-icons.woff
--rw-r--r--   0 rider     (1000) rider     (1000)    62984 2019-03-30 20:18:20.000000 django-reportbroD-4.0/django_reportbroD/static/assets/fonts/cryptocurrency-iconsd41d.eot
--rw-r--r--   0 rider     (1000) rider     (1000)    41808 2019-03-30 20:18:22.000000 django-reportbroD-4.0/django_reportbroD/static/assets/fonts/dashicons.eot
--rw-r--r--   0 rider     (1000) rider     (1000)    16604 2019-03-30 20:18:22.000000 django-reportbroD-4.0/django_reportbroD/static/assets/fonts/dashicons.html
--rw-r--r--   0 rider     (1000) rider     (1000)   163862 2019-03-30 20:18:22.000000 django-reportbroD-4.0/django_reportbroD/static/assets/fonts/dashicons.svg
--rw-r--r--   0 rider     (1000) rider     (1000)    41636 2019-03-30 20:18:22.000000 django-reportbroD-4.0/django_reportbroD/static/assets/fonts/dashicons.ttf
--rw-r--r--   0 rider     (1000) rider     (1000)    20528 2019-03-30 20:18:22.000000 django-reportbroD-4.0/django_reportbroD/static/assets/fonts/dashicons.woff
--rw-r--r--   0 rider     (1000) rider     (1000)    41808 2019-03-30 20:18:22.000000 django-reportbroD-4.0/django_reportbroD/static/assets/fonts/dashiconsd41d.eot
--rw-r--r--   0 rider     (1000) rider     (1000)    40522 2019-03-30 20:18:22.000000 django-reportbroD-4.0/django_reportbroD/static/assets/fonts/dripicons.eot
--rw-r--r--   0 rider     (1000) rider     (1000)    99368 2019-03-30 20:18:22.000000 django-reportbroD-4.0/django_reportbroD/static/assets/fonts/dripicons.svg
--rw-r--r--   0 rider     (1000) rider     (1000)    40348 2019-03-30 20:18:22.000000 django-reportbroD-4.0/django_reportbroD/static/assets/fonts/dripicons.ttf
--rw-r--r--   0 rider     (1000) rider     (1000)    26004 2019-03-30 20:18:24.000000 django-reportbroD-4.0/django_reportbroD/static/assets/fonts/dripicons.woff
--rw-r--r--   0 rider     (1000) rider     (1000)    40522 2019-03-30 20:18:24.000000 django-reportbroD-4.0/django_reportbroD/static/assets/fonts/dripiconsd41d.eot
--rw-r--r--   0 rider     (1000) rider     (1000)    62084 2019-03-30 20:18:24.000000 django-reportbroD-4.0/django_reportbroD/static/assets/fonts/feather.eot
--rw-r--r--   0 rider     (1000) rider     (1000)   213926 2019-03-30 20:18:26.000000 django-reportbroD-4.0/django_reportbroD/static/assets/fonts/feather.svg
--rw-r--r--   0 rider     (1000) rider     (1000)    61920 2019-03-30 20:18:24.000000 django-reportbroD-4.0/django_reportbroD/static/assets/fonts/feather.ttf
--rw-r--r--   0 rider     (1000) rider     (1000)    29500 2019-03-30 20:18:24.000000 django-reportbroD-4.0/django_reportbroD/static/assets/fonts/feather.woff
--rw-r--r--   0 rider     (1000) rider     (1000)    62084 2019-03-30 20:18:24.000000 django-reportbroD-4.0/django_reportbroD/static/assets/fonts/featherd41d.eot
--rw-r--r--   0 rider     (1000) rider     (1000)   165742 2019-03-30 20:18:26.000000 django-reportbroD-4.0/django_reportbroD/static/assets/fonts/font-awesome.eot
--rw-r--r--   0 rider     (1000) rider     (1000)    77159 2019-03-30 20:18:26.000000 django-reportbroD-4.0/django_reportbroD/static/assets/fonts/font-awesome.html
--rw-r--r--   0 rider     (1000) rider     (1000)   444379 2019-03-30 20:18:28.000000 django-reportbroD-4.0/django_reportbroD/static/assets/fonts/font-awesome.svg
--rw-r--r--   0 rider     (1000) rider     (1000)   165548 2019-03-30 20:18:28.000000 django-reportbroD-4.0/django_reportbroD/static/assets/fonts/font-awesome.ttf
--rw-r--r--   0 rider     (1000) rider     (1000)    98024 2019-03-30 20:18:26.000000 django-reportbroD-4.0/django_reportbroD/static/assets/fonts/font-awesome.woff
--rw-r--r--   0 rider     (1000) rider     (1000)   165742 2019-03-30 20:18:28.000000 django-reportbroD-4.0/django_reportbroD/static/assets/fonts/font-awesomed41d.eot
--rw-r--r--   0 rider     (1000) rider     (1000)   144114 2019-03-30 20:18:28.000000 django-reportbroD-4.0/django_reportbroD/static/assets/fonts/ionicons.eot
--rw-r--r--   0 rider     (1000) rider     (1000)    61020 2019-03-30 20:18:28.000000 django-reportbroD-4.0/django_reportbroD/static/assets/fonts/ionicons.html
--rw-r--r--   0 rider     (1000) rider     (1000)   400219 2019-03-30 20:18:30.000000 django-reportbroD-4.0/django_reportbroD/static/assets/fonts/ionicons.svg
--rw-r--r--   0 rider     (1000) rider     (1000)   143936 2019-03-30 20:18:34.000000 django-reportbroD-4.0/django_reportbroD/static/assets/fonts/ionicons.ttf
--rw-r--r--   0 rider     (1000) rider     (1000)    80356 2019-03-30 20:18:30.000000 django-reportbroD-4.0/django_reportbroD/static/assets/fonts/ionicons.woff
--rw-r--r--   0 rider     (1000) rider     (1000)   144114 2019-03-30 20:18:30.000000 django-reportbroD-4.0/django_reportbroD/static/assets/fonts/ioniconsd41d.eot
--rw-r--r--   0 rider     (1000) rider     (1000)    21514 2019-03-30 20:18:30.000000 django-reportbroD-4.0/django_reportbroD/static/assets/fonts/linea-weather.eot
--rw-r--r--   0 rider     (1000) rider     (1000)    48132 2019-03-30 20:18:30.000000 django-reportbroD-4.0/django_reportbroD/static/assets/fonts/linea-weather.svg
--rw-r--r--   0 rider     (1000) rider     (1000)    21308 2019-03-30 20:18:30.000000 django-reportbroD-4.0/django_reportbroD/static/assets/fonts/linea-weather.ttf
--rw-r--r--   0 rider     (1000) rider     (1000)     7936 2019-03-30 20:18:30.000000 django-reportbroD-4.0/django_reportbroD/static/assets/fonts/linea-weather.woff
--rw-r--r--   0 rider     (1000) rider     (1000)    21514 2019-03-30 20:18:32.000000 django-reportbroD-4.0/django_reportbroD/static/assets/fonts/linea-weatherd41d.eot
--rw-r--r--   0 rider     (1000) rider     (1000)    42495 2019-03-30 20:18:32.000000 django-reportbroD-4.0/django_reportbroD/static/assets/fonts/material-icons.eot
--rw-r--r--   0 rider     (1000) rider     (1000)    38383 2019-03-30 20:18:32.000000 django-reportbroD-4.0/django_reportbroD/static/assets/fonts/material-icons.html
--rw-r--r--   0 rider     (1000) rider     (1000)   238287 2019-03-30 20:18:34.000000 django-reportbroD-4.0/django_reportbroD/static/assets/fonts/material-icons.svg
--rw-r--r--   0 rider     (1000) rider     (1000)    99212 2019-03-30 20:18:32.000000 django-reportbroD-4.0/django_reportbroD/static/assets/fonts/material-icons.ttf
--rw-r--r--   0 rider     (1000) rider     (1000)    50312 2019-03-30 20:18:32.000000 django-reportbroD-4.0/django_reportbroD/static/assets/fonts/material-icons.woff
--rw-r--r--   0 rider     (1000) rider     (1000)    42495 2019-03-30 20:18:34.000000 django-reportbroD-4.0/django_reportbroD/static/assets/fonts/material-iconsd41d.eot
--rw-r--r--   0 rider     (1000) rider     (1000)    16746 2019-03-30 20:18:34.000000 django-reportbroD-4.0/django_reportbroD/static/assets/fonts/summernotec360.eot
--rw-r--r--   0 rider     (1000) rider     (1000)    16560 2019-03-30 20:18:34.000000 django-reportbroD-4.0/django_reportbroD/static/assets/fonts/summernotec360.ttf
--rw-r--r--   0 rider     (1000) rider     (1000)    10324 2019-03-30 20:18:34.000000 django-reportbroD-4.0/django_reportbroD/static/assets/fonts/summernotec360.woff
--rw-r--r--   0 rider     (1000) rider     (1000)    78748 2019-03-30 20:18:34.000000 django-reportbroD-4.0/django_reportbroD/static/assets/fonts/themify-icons.eot
--rw-r--r--   0 rider     (1000) rider     (1000)   234269 2019-03-30 20:18:36.000000 django-reportbroD-4.0/django_reportbroD/static/assets/fonts/themify-icons.svg
--rw-r--r--   0 rider     (1000) rider     (1000)    78584 2019-03-30 20:18:36.000000 django-reportbroD-4.0/django_reportbroD/static/assets/fonts/themify-icons.ttf
--rw-r--r--   0 rider     (1000) rider     (1000)    56108 2019-03-30 20:18:34.000000 django-reportbroD-4.0/django_reportbroD/static/assets/fonts/themify-icons.woff
--rw-r--r--   0 rider     (1000) rider     (1000)    78748 2019-03-30 20:18:36.000000 django-reportbroD-4.0/django_reportbroD/static/assets/fonts/themify-iconsd41d.eot
-drwxr-xr-x   0 rider     (1000) rider     (1000)        0 2024-05-22 15:14:56.931137 django-reportbroD-4.0/django_reportbroD/static/assets/img/
--rw-r--r--   0 rider     (1000) rider     (1000)    39361 2019-03-30 21:07:44.000000 django-reportbroD-4.0/django_reportbroD/static/assets/img/02.jpg
--rw-r--r--   0 rider     (1000) rider     (1000)    29789 2024-05-13 15:49:44.000000 django-reportbroD-4.0/django_reportbroD/static/assets/img/eeuu.png
-drwxr-xr-x   0 rider     (1000) rider     (1000)        0 2024-05-22 15:14:56.934471 django-reportbroD-4.0/django_reportbroD/static/assets/img/export/
--rw-r--r--   0 rider     (1000) rider     (1000)     1876 2019-03-30 21:07:30.000000 django-reportbroD-4.0/django_reportbroD/static/assets/img/export/csv.svg
--rw-r--r--   0 rider     (1000) rider     (1000)     1348 2019-03-30 21:07:30.000000 django-reportbroD-4.0/django_reportbroD/static/assets/img/export/txt.svg
--rw-r--r--   0 rider     (1000) rider     (1000)     2060 2019-03-30 21:07:30.000000 django-reportbroD-4.0/django_reportbroD/static/assets/img/export/xlsx.svg
--rw-r--r--   0 rider     (1000) rider     (1000)    48878 2024-02-21 14:09:26.000000 django-reportbroD-4.0/django_reportbroD/static/assets/img/favicon.ico
-drwxr-xr-x   0 rider     (1000) rider     (1000)        0 2024-05-22 15:14:56.937804 django-reportbroD-4.0/django_reportbroD/static/assets/img/file-icon/
--rw-r--r--   0 rider     (1000) rider     (1000)     1182 2019-03-30 21:07:32.000000 django-reportbroD-4.0/django_reportbroD/static/assets/img/file-icon/ai.png
--rw-r--r--   0 rider     (1000) rider     (1000)     1380 2019-03-30 21:07:32.000000 django-reportbroD-4.0/django_reportbroD/static/assets/img/file-icon/css.png
--rw-r--r--   0 rider     (1000) rider     (1000)      948 2019-03-30 21:07:32.000000 django-reportbroD-4.0/django_reportbroD/static/assets/img/file-icon/dbf.png
--rw-r--r--   0 rider     (1000) rider     (1000)     1383 2019-03-30 21:07:32.000000 django-reportbroD-4.0/django_reportbroD/static/assets/img/file-icon/doc.png
--rw-r--r--   0 rider     (1000) rider     (1000)     1215 2019-03-30 21:07:32.000000 django-reportbroD-4.0/django_reportbroD/static/assets/img/file-icon/dwg.png
--rw-r--r--   0 rider     (1000) rider     (1000)     1269 2019-03-30 21:07:32.000000 django-reportbroD-4.0/django_reportbroD/static/assets/img/file-icon/exe.png
--rw-r--r--   0 rider     (1000) rider     (1000)     1006 2019-03-30 21:07:32.000000 django-reportbroD-4.0/django_reportbroD/static/assets/img/file-icon/html.png
--rw-r--r--   0 rider     (1000) rider     (1000)     1364 2019-03-30 21:07:32.000000 django-reportbroD-4.0/django_reportbroD/static/assets/img/file-icon/jpg.png
--rw-r--r--   0 rider     (1000) rider     (1000)     1399 2019-03-30 21:07:32.000000 django-reportbroD-4.0/django_reportbroD/static/assets/img/file-icon/pdf.png
--rw-r--r--   0 rider     (1000) rider     (1000)     1397 2019-03-30 21:07:32.000000 django-reportbroD-4.0/django_reportbroD/static/assets/img/file-icon/png.png
--rw-r--r--   0 rider     (1000) rider     (1000)     1430 2019-03-30 21:07:32.000000 django-reportbroD-4.0/django_reportbroD/static/assets/img/file-icon/psd.png
--rw-r--r--   0 rider     (1000) rider     (1000)     6359 2024-04-14 18:02:54.000000 django-reportbroD-4.0/django_reportbroD/static/assets/img/file-icon/reporte.png
--rw-r--r--   0 rider     (1000) rider     (1000)     1005 2019-03-30 21:07:32.000000 django-reportbroD-4.0/django_reportbroD/static/assets/img/file-icon/rtf.png
--rw-r--r--   0 rider     (1000) rider     (1000)     1421 2019-03-30 21:07:32.000000 django-reportbroD-4.0/django_reportbroD/static/assets/img/file-icon/svg.png
--rw-r--r--   0 rider     (1000) rider     (1000)      974 2019-03-30 21:07:34.000000 django-reportbroD-4.0/django_reportbroD/static/assets/img/file-icon/xls.png
--rw-r--r--   0 rider     (1000) rider     (1000)     1332 2019-03-30 21:07:34.000000 django-reportbroD-4.0/django_reportbroD/static/assets/img/file-icon/xml.png
--rw-r--r--   0 rider     (1000) rider     (1000)      997 2019-03-30 21:07:34.000000 django-reportbroD-4.0/django_reportbroD/static/assets/img/file-icon/zip.png
--rw-r--r--   0 rider     (1000) rider     (1000)     7446 2024-03-09 16:12:06.000000 django-reportbroD-4.0/django_reportbroD/static/assets/img/lista.png
--rw-r--r--   0 rider     (1000) rider     (1000)     4814 2024-02-21 13:55:04.000000 django-reportbroD-4.0/django_reportbroD/static/assets/img/logo-icon.png
--rw-r--r--   0 rider     (1000) rider     (1000)     2422 2019-03-30 20:18:36.000000 django-reportbroD-4.0/django_reportbroD/static/assets/img/logo-light.png
--rw-r--r--   0 rider     (1000) rider     (1000)    13606 2024-02-21 13:43:58.000000 django-reportbroD-4.0/django_reportbroD/static/assets/img/logo.png
--rw-r--r--   0 rider     (1000) rider     (1000)    28535 2024-05-13 15:49:44.000000 django-reportbroD-4.0/django_reportbroD/static/assets/img/spain.png
-drwxr-xr-x   0 rider     (1000) rider     (1000)        0 2024-05-22 15:14:56.937804 django-reportbroD-4.0/django_reportbroD/static/assets/js/
--rw-r--r--   0 rider     (1000) rider     (1000)   576312 2019-03-30 20:18:44.000000 django-reportbroD-4.0/django_reportbroD/static/assets/js/app.js
--rw-r--r--   0 rider     (1000) rider     (1000)  8320860 2019-03-30 20:19:02.000000 django-reportbroD-4.0/django_reportbroD/static/assets/js/vendors.js
-drwxr-xr-x   0 rider     (1000) rider     (1000)        0 2024-05-22 15:14:56.961138 django-reportbroD-4.0/django_reportbroD/static/reportlib/
-drwxr-xr-x   0 rider     (1000) rider     (1000)        0 2024-05-22 15:14:56.964471 django-reportbroD-4.0/django_reportbroD/static/reportlib/css/
-drwxr-xr-x   0 rider     (1000) rider     (1000)        0 2024-05-22 15:14:56.964471 django-reportbroD-4.0/django_reportbroD/static/reportlib/css/iconfonts/
-drwxr-xr-x   0 rider     (1000) rider     (1000)        0 2024-05-22 15:14:56.964471 django-reportbroD-4.0/django_reportbroD/static/reportlib/css/iconfonts/fonts/
--rw-r--r--   0 rider     (1000) rider     (1000)     1633 2024-02-14 15:51:44.000000 django-reportbroD-4.0/django_reportbroD/static/reportlib/css/iconfonts/fonts/demoapp.svg
--rw-r--r--   0 rider     (1000) rider     (1000)     1384 2024-02-14 15:51:44.000000 django-reportbroD-4.0/django_reportbroD/static/reportlib/css/iconfonts/fonts/demoapp.ttf
--rw-r--r--   0 rider     (1000) rider     (1000)     1460 2024-02-14 15:51:44.000000 django-reportbroD-4.0/django_reportbroD/static/reportlib/css/iconfonts/fonts/demoapp.woff
--rw-r--r--   0 rider     (1000) rider     (1000)      684 2024-02-14 15:51:44.000000 django-reportbroD-4.0/django_reportbroD/static/reportlib/css/iconfonts/fonts/demoapp.woff2
--rw-r--r--   0 rider     (1000) rider     (1000)      855 2024-02-14 15:51:44.000000 django-reportbroD-4.0/django_reportbroD/static/reportlib/css/iconfonts/style.css
--rw-r--r--   0 rider     (1000) rider     (1000)     4509 2024-02-21 21:05:40.000000 django-reportbroD-4.0/django_reportbroD/static/reportlib/css/styles.css
--rw-r--r--   0 rider     (1000) rider     (1000)     2238 2024-02-14 15:51:44.000000 django-reportbroD-4.0/django_reportbroD/static/reportlib/favicon.ico
-drwxr-xr-x   0 rider     (1000) rider     (1000)        0 2024-05-22 15:14:56.964471 django-reportbroD-4.0/django_reportbroD/static/reportlib/js/
--rw-r--r--   0 rider     (1000) rider     (1000)   288580 2024-02-14 15:51:44.000000 django-reportbroD-4.0/django_reportbroD/static/reportlib/js/jquery-3.6.0.js
--rw-r--r--   0 rider     (1000) rider     (1000)    89501 2024-02-14 15:51:44.000000 django-reportbroD-4.0/django_reportbroD/static/reportlib/js/jquery-3.6.0.min.js
--rw-r--r--   0 rider     (1000) rider     (1000)     3121 2024-02-14 15:51:44.000000 django-reportbroD-4.0/django_reportbroD/static/reportlib/js/jquery.cookie.js
--rw-r--r--   0 rider     (1000) rider     (1000)    55398 2024-02-21 20:18:44.000000 django-reportbroD-4.0/django_reportbroD/static/reportlib/reportbro.css
--rw-r--r--   0 rider     (1000) rider     (1000)    77644 2024-02-21 20:18:44.000000 django-reportbroD-4.0/django_reportbroD/static/reportlib/reportbro.css.map
--rw-r--r--   0 rider     (1000) rider     (1000)   733475 2024-05-18 23:36:56.000000 django-reportbroD-4.0/django_reportbroD/static/reportlib/reportbro.js
--rw-r--r--   0 rider     (1000) rider     (1000)      665 2024-02-21 20:18:44.000000 django-reportbroD-4.0/django_reportbroD/static/reportlib/reportbro.js.LICENSE.txt
--rw-r--r--   0 rider     (1000) rider     (1000)  2440768 2024-02-21 20:18:44.000000 django-reportbroD-4.0/django_reportbroD/static/reportlib/reportbro.js.map
--rw-r--r--   0 rider     (1000) rider     (1000)   722287 2024-02-21 20:18:44.000000 django-reportbroD-4.0/django_reportbroD/static/reportlib/reportbro.min.js
--rw-r--r--   0 rider     (1000) rider     (1000)   803864 2024-02-21 20:18:44.000000 django-reportbroD-4.0/django_reportbroD/static/reportlib/reportbro.min.js.map
-drwxr-xr-x   0 rider     (1000) rider     (1000)        0 2024-05-22 15:14:56.967804 django-reportbroD-4.0/django_reportbroD/static/reportlib/src/
--rw-r--r--   0 rider     (1000) rider     (1000)    24374 2024-02-21 20:18:44.000000 django-reportbroD-4.0/django_reportbroD/static/reportlib/src/ajaxload.gif
-drwxr-xr-x   0 rider     (1000) rider     (1000)        0 2024-05-22 15:14:56.971138 django-reportbroD-4.0/django_reportbroD/static/reportlib/src/fonts/
--rw-r--r--   0 rider     (1000) rider     (1000)    20756 2024-02-21 20:18:44.000000 django-reportbroD-4.0/django_reportbroD/static/reportlib/src/fonts/open-sans-v34-latin-300.woff
--rw-r--r--   0 rider     (1000) rider     (1000)    16748 2024-02-21 20:18:44.000000 django-reportbroD-4.0/django_reportbroD/static/reportlib/src/fonts/open-sans-v34-latin-300.woff2
--rw-r--r--   0 rider     (1000) rider     (1000)    20672 2024-02-21 20:18:44.000000 django-reportbroD-4.0/django_reportbroD/static/reportlib/src/fonts/open-sans-v34-latin-600.woff
--rw-r--r--   0 rider     (1000) rider     (1000)    16756 2024-02-21 20:18:44.000000 django-reportbroD-4.0/django_reportbroD/static/reportlib/src/fonts/open-sans-v34-latin-600.woff2
--rw-r--r--   0 rider     (1000) rider     (1000)    20664 2024-02-21 20:18:44.000000 django-reportbroD-4.0/django_reportbroD/static/reportlib/src/fonts/open-sans-v34-latin-800.woff
--rw-r--r--   0 rider     (1000) rider     (1000)    16696 2024-02-21 20:18:44.000000 django-reportbroD-4.0/django_reportbroD/static/reportlib/src/fonts/open-sans-v34-latin-800.woff2
--rw-r--r--   0 rider     (1000) rider     (1000)    20712 2024-02-21 20:18:44.000000 django-reportbroD-4.0/django_reportbroD/static/reportlib/src/fonts/open-sans-v34-latin-regular.woff
--rw-r--r--   0 rider     (1000) rider     (1000)    16740 2024-02-21 20:18:44.000000 django-reportbroD-4.0/django_reportbroD/static/reportlib/src/fonts/open-sans-v34-latin-regular.woff2
-drwxr-xr-x   0 rider     (1000) rider     (1000)        0 2024-05-22 15:14:56.971138 django-reportbroD-4.0/django_reportbroD/static/reportlib/src/iconfonts/
--rw-r--r--   0 rider     (1000) rider     (1000)    37788 2024-02-21 20:18:44.000000 django-reportbroD-4.0/django_reportbroD/static/reportlib/src/iconfonts/reportbro.svg
--rw-r--r--   0 rider     (1000) rider     (1000)    12676 2024-02-21 20:18:44.000000 django-reportbroD-4.0/django_reportbroD/static/reportlib/src/iconfonts/reportbro.ttf
--rw-r--r--   0 rider     (1000) rider     (1000)    12752 2024-02-21 20:18:44.000000 django-reportbroD-4.0/django_reportbroD/static/reportlib/src/iconfonts/reportbro.woff
--rw-r--r--   0 rider     (1000) rider     (1000)     4460 2024-02-21 20:18:44.000000 django-reportbroD-4.0/django_reportbroD/static/reportlib/src/iconfonts/reportbro.woff2
--rw-r--r--   0 rider     (1000) rider     (1000)    12924 2024-02-21 20:18:44.000000 django-reportbroD-4.0/django_reportbroD/static/reportlib/src/rb_logo_dark.png
--rw-r--r--   0 rider     (1000) rider     (1000)    13606 2024-02-21 20:18:44.000000 django-reportbroD-4.0/django_reportbroD/static/reportlib/src/rb_logo_white.png
-drwxr-xr-x   0 rider     (1000) rider     (1000)        0 2024-05-22 15:14:56.974471 django-reportbroD-4.0/django_reportbroD/templates/
-drwxr-xr-x   0 rider     (1000) rider     (1000)        0 2024-05-22 15:14:56.977805 django-reportbroD-4.0/django_reportbroD/templates/bases/
--rw-r--r--   0 rider     (1000) rider     (1000)     1942 2024-05-16 14:15:12.000000 django-reportbroD-4.0/django_reportbroD/templates/bases/base.html
--rw-r--r--   0 rider     (1000) rider     (1000)      352 2024-04-15 00:52:16.000000 django-reportbroD-4.0/django_reportbroD/templates/bases/footer.html
--rw-r--r--   0 rider     (1000) rider     (1000)     3916 2024-05-19 02:26:34.000000 django-reportbroD-4.0/django_reportbroD/templates/bases/header.html
--rw-r--r--   0 rider     (1000) rider     (1000)      677 2024-05-19 00:25:08.000000 django-reportbroD-4.0/django_reportbroD/templates/bases/navigator.html
--rw-r--r--   0 rider     (1000) rider     (1000)     1926 2024-05-17 14:02:34.000000 django-reportbroD-4.0/django_reportbroD/templates/create.html
--rw-r--r--   0 rider     (1000) rider     (1000)    16761 2024-05-16 15:46:40.000000 django-reportbroD-4.0/django_reportbroD/templates/document.html
--rw-r--r--   0 rider     (1000) rider     (1000)     2157 2024-05-17 14:00:38.000000 django-reportbroD-4.0/django_reportbroD/templates/edit.html
--rw-r--r--   0 rider     (1000) rider     (1000)    21051 2024-05-17 13:57:14.000000 django-reportbroD-4.0/django_reportbroD/templates/especif.html
--rw-r--r--   0 rider     (1000) rider     (1000)     1192 2024-05-17 14:18:06.000000 django-reportbroD-4.0/django_reportbroD/templates/formulario.html
--rw-r--r--   0 rider     (1000) rider     (1000)     3102 2024-05-17 14:04:22.000000 django-reportbroD-4.0/django_reportbroD/templates/import.html
--rw-r--r--   0 rider     (1000) rider     (1000)     8884 2024-05-13 14:01:34.000000 django-reportbroD-4.0/django_reportbroD/templates/index.html
--rw-r--r--   0 rider     (1000) rider     (1000)     6199 2024-05-20 13:21:45.000000 django-reportbroD-4.0/django_reportbroD/templates/report.html
--rw-r--r--   0 rider     (1000) rider     (1000)      756 2024-05-20 12:15:37.000000 django-reportbroD-4.0/django_reportbroD/urls.py
--rw-r--r--   0 rider     (1000) rider     (1000)     4621 2024-05-12 18:19:58.000000 django-reportbroD-4.0/django_reportbroD/utils.py
--rw-r--r--   0 rider     (1000) rider     (1000)     3258 2024-05-16 12:47:16.000000 django-reportbroD-4.0/django_reportbroD/views.py
-drwxr-xr-x   0 rider     (1000) rider     (1000)        0 2024-05-22 15:14:56.894470 django-reportbroD-4.0/django_reportbroD.egg-info/
--rw-r--r--   0 rider     (1000) rider     (1000)     5861 2024-05-22 15:14:56.000000 django-reportbroD-4.0/django_reportbroD.egg-info/PKG-INFO
--rw-r--r--   0 rider     (1000) rider     (1000)     8032 2024-05-22 15:14:56.000000 django-reportbroD-4.0/django_reportbroD.egg-info/SOURCES.txt
--rw-r--r--   0 rider     (1000) rider     (1000)        1 2024-05-22 15:14:56.000000 django-reportbroD-4.0/django_reportbroD.egg-info/dependency_links.txt
--rw-r--r--   0 rider     (1000) rider     (1000)       33 2024-05-22 15:14:56.000000 django-reportbroD-4.0/django_reportbroD.egg-info/requires.txt
--rw-r--r--   0 rider     (1000) rider     (1000)       18 2024-05-22 15:14:56.000000 django-reportbroD-4.0/django_reportbroD.egg-info/top_level.txt
--rw-r--r--   0 rider     (1000) rider     (1000)     1177 2024-05-22 15:14:56.977805 django-reportbroD-4.0/setup.cfg
--rw-r--r--   0 rider     (1000) rider     (1000)       37 2024-02-21 17:28:39.000000 django-reportbroD-4.0/setup.py
+drwxr-xr-x   0 rider     (1000) rider     (1000)        0 2024-05-29 14:03:36.344705 django_reportbrod-4.1/
+-rw-r--r--   0 rider     (1000) rider     (1000)      176 2024-05-22 11:02:56.000000 django_reportbrod-4.1/MANIFEST.in
+-rw-r--r--   0 rider     (1000) rider     (1000)     5733 2024-05-29 14:03:36.344705 django_reportbrod-4.1/PKG-INFO
+-rw-r--r--   0 rider     (1000) rider     (1000)     4612 2024-05-29 14:03:09.000000 django_reportbrod-4.1/README.md
+drwxr-xr-x   0 rider     (1000) rider     (1000)        0 2024-05-29 14:03:36.134704 django_reportbrod-4.1/django_reportbroD/
+-rw-r--r--   0 rider     (1000) rider     (1000)        0 2024-02-16 20:55:14.000000 django_reportbrod-4.1/django_reportbroD/__init__.py
+-rw-r--r--   0 rider     (1000) rider     (1000)      166 2024-05-29 12:11:22.000000 django_reportbrod-4.1/django_reportbroD/admin.py
+-rw-r--r--   0 rider     (1000) rider     (1000)      189 2024-05-29 13:34:02.000000 django_reportbrod-4.1/django_reportbroD/apps.py
+-rw-r--r--   0 rider     (1000) rider     (1000)      802 2024-05-29 12:11:51.000000 django_reportbrod-4.1/django_reportbroD/base.py
+-rw-r--r--   0 rider     (1000) rider     (1000)     1164 2024-05-29 12:11:51.000000 django_reportbrod-4.1/django_reportbroD/forms.py
+drwxr-xr-x   0 rider     (1000) rider     (1000)        0 2024-05-29 14:03:36.128037 django_reportbrod-4.1/django_reportbroD/locale/
+drwxr-xr-x   0 rider     (1000) rider     (1000)        0 2024-05-29 14:03:36.128037 django_reportbrod-4.1/django_reportbroD/locale/en/
+drwxr-xr-x   0 rider     (1000) rider     (1000)        0 2024-05-29 14:03:36.138037 django_reportbrod-4.1/django_reportbroD/locale/en/LC_MESSAGES/
+-rw-r--r--   0 rider     (1000) rider     (1000)     9709 2024-05-22 11:16:38.000000 django_reportbrod-4.1/django_reportbroD/locale/en/LC_MESSAGES/django.mo
+-rw-r--r--   0 rider     (1000) rider     (1000)     9997 2024-05-22 11:15:35.000000 django_reportbrod-4.1/django_reportbroD/locale/en/LC_MESSAGES/django.po
+drwxr-xr-x   0 rider     (1000) rider     (1000)        0 2024-05-29 14:03:36.128037 django_reportbrod-4.1/django_reportbroD/locale/es/
+drwxr-xr-x   0 rider     (1000) rider     (1000)        0 2024-05-29 14:03:36.141370 django_reportbrod-4.1/django_reportbroD/locale/es/LC_MESSAGES/
+-rw-r--r--   0 rider     (1000) rider     (1000)    10561 2024-05-20 12:40:39.000000 django_reportbrod-4.1/django_reportbroD/locale/es/LC_MESSAGES/django.mo
+-rw-r--r--   0 rider     (1000) rider     (1000)    10852 2024-05-19 00:43:40.000000 django_reportbrod-4.1/django_reportbroD/locale/es/LC_MESSAGES/django.po
+-rw-r--r--   0 rider     (1000) rider     (1000)     1241 2024-05-29 13:03:22.000000 django_reportbrod-4.1/django_reportbroD/menus.py
+drwxr-xr-x   0 rider     (1000) rider     (1000)        0 2024-05-29 14:03:36.141370 django_reportbrod-4.1/django_reportbroD/migrations/
+-rw-r--r--   0 rider     (1000) rider     (1000)     2358 2024-05-29 12:11:51.000000 django_reportbrod-4.1/django_reportbroD/migrations/0001_initial.py
+-rw-r--r--   0 rider     (1000) rider     (1000)        0 2024-02-16 20:55:14.000000 django_reportbrod-4.1/django_reportbroD/migrations/__init__.py
+-rw-r--r--   0 rider     (1000) rider     (1000)     1894 2024-05-29 12:11:51.000000 django_reportbrod-4.1/django_reportbroD/models.py
+-rw-r--r--   0 rider     (1000) rider     (1000)    14380 2024-05-29 13:32:25.000000 django_reportbrod-4.1/django_reportbroD/reportcore.py
+drwxr-xr-x   0 rider     (1000) rider     (1000)        0 2024-05-29 14:03:36.128037 django_reportbrod-4.1/django_reportbroD/static/
+drwxr-xr-x   0 rider     (1000) rider     (1000)        0 2024-05-29 14:03:36.128037 django_reportbrod-4.1/django_reportbroD/static/assets/
+drwxr-xr-x   0 rider     (1000) rider     (1000)        0 2024-05-29 14:03:36.144704 django_reportbrod-4.1/django_reportbroD/static/assets/css/
+-rw-r--r--   0 rider     (1000) rider     (1000)     1772 2019-03-30 20:18:02.000000 django_reportbrod-4.1/django_reportbroD/static/assets/css/mCSB_buttons.html
+-rw-r--r--   0 rider     (1000) rider     (1000)     1772 2019-03-30 20:18:02.000000 django_reportbrod-4.1/django_reportbroD/static/assets/css/owl.video.play.html
+-rw-r--r--   0 rider     (1000) rider     (1000)   509223 2019-03-30 20:18:10.000000 django_reportbrod-4.1/django_reportbroD/static/assets/css/style.css
+-rw-r--r--   0 rider     (1000) rider     (1000)   236692 2024-05-05 16:55:58.000000 django_reportbrod-4.1/django_reportbroD/static/assets/css/vendors.css
+drwxr-xr-x   0 rider     (1000) rider     (1000)        0 2024-05-29 14:03:36.248037 django_reportbrod-4.1/django_reportbroD/static/assets/fonts/
+-rw-r--r--   0 rider     (1000) rider     (1000)    62984 2019-03-30 20:18:20.000000 django_reportbrod-4.1/django_reportbroD/static/assets/fonts/cryptocurrency-icons.eot
+-rw-r--r--   0 rider     (1000) rider     (1000)    24288 2019-03-30 20:18:20.000000 django_reportbrod-4.1/django_reportbroD/static/assets/fonts/cryptocurrency-icons.html
+-rw-r--r--   0 rider     (1000) rider     (1000)   351196 2019-03-30 20:18:20.000000 django_reportbrod-4.1/django_reportbroD/static/assets/fonts/cryptocurrency-icons.svg
+-rw-r--r--   0 rider     (1000) rider     (1000)    62768 2019-03-30 20:18:20.000000 django_reportbrod-4.1/django_reportbroD/static/assets/fonts/cryptocurrency-icons.ttf
+-rw-r--r--   0 rider     (1000) rider     (1000)    31064 2019-03-30 20:18:20.000000 django_reportbrod-4.1/django_reportbroD/static/assets/fonts/cryptocurrency-icons.woff
+-rw-r--r--   0 rider     (1000) rider     (1000)    62984 2019-03-30 20:18:20.000000 django_reportbrod-4.1/django_reportbroD/static/assets/fonts/cryptocurrency-iconsd41d.eot
+-rw-r--r--   0 rider     (1000) rider     (1000)    41808 2019-03-30 20:18:22.000000 django_reportbrod-4.1/django_reportbroD/static/assets/fonts/dashicons.eot
+-rw-r--r--   0 rider     (1000) rider     (1000)    16604 2019-03-30 20:18:22.000000 django_reportbrod-4.1/django_reportbroD/static/assets/fonts/dashicons.html
+-rw-r--r--   0 rider     (1000) rider     (1000)   163862 2019-03-30 20:18:22.000000 django_reportbrod-4.1/django_reportbroD/static/assets/fonts/dashicons.svg
+-rw-r--r--   0 rider     (1000) rider     (1000)    41636 2019-03-30 20:18:22.000000 django_reportbrod-4.1/django_reportbroD/static/assets/fonts/dashicons.ttf
+-rw-r--r--   0 rider     (1000) rider     (1000)    20528 2019-03-30 20:18:22.000000 django_reportbrod-4.1/django_reportbroD/static/assets/fonts/dashicons.woff
+-rw-r--r--   0 rider     (1000) rider     (1000)    41808 2019-03-30 20:18:22.000000 django_reportbrod-4.1/django_reportbroD/static/assets/fonts/dashiconsd41d.eot
+-rw-r--r--   0 rider     (1000) rider     (1000)    40522 2019-03-30 20:18:22.000000 django_reportbrod-4.1/django_reportbroD/static/assets/fonts/dripicons.eot
+-rw-r--r--   0 rider     (1000) rider     (1000)    99368 2019-03-30 20:18:22.000000 django_reportbrod-4.1/django_reportbroD/static/assets/fonts/dripicons.svg
+-rw-r--r--   0 rider     (1000) rider     (1000)    40348 2019-03-30 20:18:22.000000 django_reportbrod-4.1/django_reportbroD/static/assets/fonts/dripicons.ttf
+-rw-r--r--   0 rider     (1000) rider     (1000)    26004 2019-03-30 20:18:24.000000 django_reportbrod-4.1/django_reportbroD/static/assets/fonts/dripicons.woff
+-rw-r--r--   0 rider     (1000) rider     (1000)    40522 2019-03-30 20:18:24.000000 django_reportbrod-4.1/django_reportbroD/static/assets/fonts/dripiconsd41d.eot
+-rw-r--r--   0 rider     (1000) rider     (1000)    62084 2019-03-30 20:18:24.000000 django_reportbrod-4.1/django_reportbroD/static/assets/fonts/feather.eot
+-rw-r--r--   0 rider     (1000) rider     (1000)   213926 2019-03-30 20:18:26.000000 django_reportbrod-4.1/django_reportbroD/static/assets/fonts/feather.svg
+-rw-r--r--   0 rider     (1000) rider     (1000)    61920 2019-03-30 20:18:24.000000 django_reportbrod-4.1/django_reportbroD/static/assets/fonts/feather.ttf
+-rw-r--r--   0 rider     (1000) rider     (1000)    29500 2019-03-30 20:18:24.000000 django_reportbrod-4.1/django_reportbroD/static/assets/fonts/feather.woff
+-rw-r--r--   0 rider     (1000) rider     (1000)    62084 2019-03-30 20:18:24.000000 django_reportbrod-4.1/django_reportbroD/static/assets/fonts/featherd41d.eot
+-rw-r--r--   0 rider     (1000) rider     (1000)   165742 2019-03-30 20:18:26.000000 django_reportbrod-4.1/django_reportbroD/static/assets/fonts/font-awesome.eot
+-rw-r--r--   0 rider     (1000) rider     (1000)    77159 2019-03-30 20:18:26.000000 django_reportbrod-4.1/django_reportbroD/static/assets/fonts/font-awesome.html
+-rw-r--r--   0 rider     (1000) rider     (1000)   444379 2019-03-30 20:18:28.000000 django_reportbrod-4.1/django_reportbroD/static/assets/fonts/font-awesome.svg
+-rw-r--r--   0 rider     (1000) rider     (1000)   165548 2019-03-30 20:18:28.000000 django_reportbrod-4.1/django_reportbroD/static/assets/fonts/font-awesome.ttf
+-rw-r--r--   0 rider     (1000) rider     (1000)    98024 2019-03-30 20:18:26.000000 django_reportbrod-4.1/django_reportbroD/static/assets/fonts/font-awesome.woff
+-rw-r--r--   0 rider     (1000) rider     (1000)   165742 2019-03-30 20:18:28.000000 django_reportbrod-4.1/django_reportbroD/static/assets/fonts/font-awesomed41d.eot
+-rw-r--r--   0 rider     (1000) rider     (1000)   144114 2019-03-30 20:18:28.000000 django_reportbrod-4.1/django_reportbroD/static/assets/fonts/ionicons.eot
+-rw-r--r--   0 rider     (1000) rider     (1000)    61020 2019-03-30 20:18:28.000000 django_reportbrod-4.1/django_reportbroD/static/assets/fonts/ionicons.html
+-rw-r--r--   0 rider     (1000) rider     (1000)   400219 2019-03-30 20:18:30.000000 django_reportbrod-4.1/django_reportbroD/static/assets/fonts/ionicons.svg
+-rw-r--r--   0 rider     (1000) rider     (1000)   143936 2019-03-30 20:18:34.000000 django_reportbrod-4.1/django_reportbroD/static/assets/fonts/ionicons.ttf
+-rw-r--r--   0 rider     (1000) rider     (1000)    80356 2019-03-30 20:18:30.000000 django_reportbrod-4.1/django_reportbroD/static/assets/fonts/ionicons.woff
+-rw-r--r--   0 rider     (1000) rider     (1000)   144114 2019-03-30 20:18:30.000000 django_reportbrod-4.1/django_reportbroD/static/assets/fonts/ioniconsd41d.eot
+-rw-r--r--   0 rider     (1000) rider     (1000)    21514 2019-03-30 20:18:30.000000 django_reportbrod-4.1/django_reportbroD/static/assets/fonts/linea-weather.eot
+-rw-r--r--   0 rider     (1000) rider     (1000)    48132 2019-03-30 20:18:30.000000 django_reportbrod-4.1/django_reportbroD/static/assets/fonts/linea-weather.svg
+-rw-r--r--   0 rider     (1000) rider     (1000)    21308 2019-03-30 20:18:30.000000 django_reportbrod-4.1/django_reportbroD/static/assets/fonts/linea-weather.ttf
+-rw-r--r--   0 rider     (1000) rider     (1000)     7936 2019-03-30 20:18:30.000000 django_reportbrod-4.1/django_reportbroD/static/assets/fonts/linea-weather.woff
+-rw-r--r--   0 rider     (1000) rider     (1000)    21514 2019-03-30 20:18:32.000000 django_reportbrod-4.1/django_reportbroD/static/assets/fonts/linea-weatherd41d.eot
+-rw-r--r--   0 rider     (1000) rider     (1000)    42495 2019-03-30 20:18:32.000000 django_reportbrod-4.1/django_reportbroD/static/assets/fonts/material-icons.eot
+-rw-r--r--   0 rider     (1000) rider     (1000)    38383 2019-03-30 20:18:32.000000 django_reportbrod-4.1/django_reportbroD/static/assets/fonts/material-icons.html
+-rw-r--r--   0 rider     (1000) rider     (1000)   238287 2019-03-30 20:18:34.000000 django_reportbrod-4.1/django_reportbroD/static/assets/fonts/material-icons.svg
+-rw-r--r--   0 rider     (1000) rider     (1000)    99212 2019-03-30 20:18:32.000000 django_reportbrod-4.1/django_reportbroD/static/assets/fonts/material-icons.ttf
+-rw-r--r--   0 rider     (1000) rider     (1000)    50312 2019-03-30 20:18:32.000000 django_reportbrod-4.1/django_reportbroD/static/assets/fonts/material-icons.woff
+-rw-r--r--   0 rider     (1000) rider     (1000)    42495 2019-03-30 20:18:34.000000 django_reportbrod-4.1/django_reportbroD/static/assets/fonts/material-iconsd41d.eot
+-rw-r--r--   0 rider     (1000) rider     (1000)    16746 2019-03-30 20:18:34.000000 django_reportbrod-4.1/django_reportbroD/static/assets/fonts/summernotec360.eot
+-rw-r--r--   0 rider     (1000) rider     (1000)    16560 2019-03-30 20:18:34.000000 django_reportbrod-4.1/django_reportbroD/static/assets/fonts/summernotec360.ttf
+-rw-r--r--   0 rider     (1000) rider     (1000)    10324 2019-03-30 20:18:34.000000 django_reportbrod-4.1/django_reportbroD/static/assets/fonts/summernotec360.woff
+-rw-r--r--   0 rider     (1000) rider     (1000)    78748 2019-03-30 20:18:34.000000 django_reportbrod-4.1/django_reportbroD/static/assets/fonts/themify-icons.eot
+-rw-r--r--   0 rider     (1000) rider     (1000)   234269 2019-03-30 20:18:36.000000 django_reportbrod-4.1/django_reportbroD/static/assets/fonts/themify-icons.svg
+-rw-r--r--   0 rider     (1000) rider     (1000)    78584 2019-03-30 20:18:36.000000 django_reportbrod-4.1/django_reportbroD/static/assets/fonts/themify-icons.ttf
+-rw-r--r--   0 rider     (1000) rider     (1000)    56108 2019-03-30 20:18:34.000000 django_reportbrod-4.1/django_reportbroD/static/assets/fonts/themify-icons.woff
+-rw-r--r--   0 rider     (1000) rider     (1000)    78748 2019-03-30 20:18:36.000000 django_reportbrod-4.1/django_reportbroD/static/assets/fonts/themify-iconsd41d.eot
+drwxr-xr-x   0 rider     (1000) rider     (1000)        0 2024-05-29 14:03:36.254704 django_reportbrod-4.1/django_reportbroD/static/assets/img/
+-rw-r--r--   0 rider     (1000) rider     (1000)    39361 2019-03-30 21:07:44.000000 django_reportbrod-4.1/django_reportbroD/static/assets/img/02.jpg
+-rw-r--r--   0 rider     (1000) rider     (1000)    29789 2024-05-13 15:49:44.000000 django_reportbrod-4.1/django_reportbroD/static/assets/img/eeuu.png
+drwxr-xr-x   0 rider     (1000) rider     (1000)        0 2024-05-29 14:03:36.258038 django_reportbrod-4.1/django_reportbroD/static/assets/img/export/
+-rw-r--r--   0 rider     (1000) rider     (1000)     1876 2019-03-30 21:07:30.000000 django_reportbrod-4.1/django_reportbroD/static/assets/img/export/csv.svg
+-rw-r--r--   0 rider     (1000) rider     (1000)     1348 2019-03-30 21:07:30.000000 django_reportbrod-4.1/django_reportbroD/static/assets/img/export/txt.svg
+-rw-r--r--   0 rider     (1000) rider     (1000)     2060 2019-03-30 21:07:30.000000 django_reportbrod-4.1/django_reportbroD/static/assets/img/export/xlsx.svg
+-rw-r--r--   0 rider     (1000) rider     (1000)    48878 2024-02-21 14:09:26.000000 django_reportbrod-4.1/django_reportbroD/static/assets/img/favicon.ico
+drwxr-xr-x   0 rider     (1000) rider     (1000)        0 2024-05-29 14:03:36.271371 django_reportbrod-4.1/django_reportbroD/static/assets/img/file-icon/
+-rw-r--r--   0 rider     (1000) rider     (1000)     1182 2019-03-30 21:07:32.000000 django_reportbrod-4.1/django_reportbroD/static/assets/img/file-icon/ai.png
+-rw-r--r--   0 rider     (1000) rider     (1000)     1380 2019-03-30 21:07:32.000000 django_reportbrod-4.1/django_reportbroD/static/assets/img/file-icon/css.png
+-rw-r--r--   0 rider     (1000) rider     (1000)      948 2019-03-30 21:07:32.000000 django_reportbrod-4.1/django_reportbroD/static/assets/img/file-icon/dbf.png
+-rw-r--r--   0 rider     (1000) rider     (1000)     1383 2019-03-30 21:07:32.000000 django_reportbrod-4.1/django_reportbroD/static/assets/img/file-icon/doc.png
+-rw-r--r--   0 rider     (1000) rider     (1000)     1215 2019-03-30 21:07:32.000000 django_reportbrod-4.1/django_reportbroD/static/assets/img/file-icon/dwg.png
+-rw-r--r--   0 rider     (1000) rider     (1000)     1269 2019-03-30 21:07:32.000000 django_reportbrod-4.1/django_reportbroD/static/assets/img/file-icon/exe.png
+-rw-r--r--   0 rider     (1000) rider     (1000)     1006 2019-03-30 21:07:32.000000 django_reportbrod-4.1/django_reportbroD/static/assets/img/file-icon/html.png
+-rw-r--r--   0 rider     (1000) rider     (1000)     1364 2019-03-30 21:07:32.000000 django_reportbrod-4.1/django_reportbroD/static/assets/img/file-icon/jpg.png
+-rw-r--r--   0 rider     (1000) rider     (1000)     1399 2019-03-30 21:07:32.000000 django_reportbrod-4.1/django_reportbroD/static/assets/img/file-icon/pdf.png
+-rw-r--r--   0 rider     (1000) rider     (1000)     1397 2019-03-30 21:07:32.000000 django_reportbrod-4.1/django_reportbroD/static/assets/img/file-icon/png.png
+-rw-r--r--   0 rider     (1000) rider     (1000)     1430 2019-03-30 21:07:32.000000 django_reportbrod-4.1/django_reportbroD/static/assets/img/file-icon/psd.png
+-rw-r--r--   0 rider     (1000) rider     (1000)     6359 2024-04-14 18:02:54.000000 django_reportbrod-4.1/django_reportbroD/static/assets/img/file-icon/reporte.png
+-rw-r--r--   0 rider     (1000) rider     (1000)     1005 2019-03-30 21:07:32.000000 django_reportbrod-4.1/django_reportbroD/static/assets/img/file-icon/rtf.png
+-rw-r--r--   0 rider     (1000) rider     (1000)     1421 2019-03-30 21:07:32.000000 django_reportbrod-4.1/django_reportbroD/static/assets/img/file-icon/svg.png
+-rw-r--r--   0 rider     (1000) rider     (1000)      974 2019-03-30 21:07:34.000000 django_reportbrod-4.1/django_reportbroD/static/assets/img/file-icon/xls.png
+-rw-r--r--   0 rider     (1000) rider     (1000)     1332 2019-03-30 21:07:34.000000 django_reportbrod-4.1/django_reportbroD/static/assets/img/file-icon/xml.png
+-rw-r--r--   0 rider     (1000) rider     (1000)      997 2019-03-30 21:07:34.000000 django_reportbrod-4.1/django_reportbroD/static/assets/img/file-icon/zip.png
+-rw-r--r--   0 rider     (1000) rider     (1000)     7446 2024-03-09 16:12:06.000000 django_reportbrod-4.1/django_reportbroD/static/assets/img/lista.png
+-rw-r--r--   0 rider     (1000) rider     (1000)     4814 2024-02-21 13:55:04.000000 django_reportbrod-4.1/django_reportbroD/static/assets/img/logo-icon.png
+-rw-r--r--   0 rider     (1000) rider     (1000)     2422 2019-03-30 20:18:36.000000 django_reportbrod-4.1/django_reportbroD/static/assets/img/logo-light.png
+-rw-r--r--   0 rider     (1000) rider     (1000)    13606 2024-02-21 13:43:58.000000 django_reportbrod-4.1/django_reportbroD/static/assets/img/logo.png
+-rw-r--r--   0 rider     (1000) rider     (1000)    28535 2024-05-13 15:49:44.000000 django_reportbrod-4.1/django_reportbroD/static/assets/img/spain.png
+drwxr-xr-x   0 rider     (1000) rider     (1000)        0 2024-05-29 14:03:36.274704 django_reportbrod-4.1/django_reportbroD/static/assets/js/
+-rw-r--r--   0 rider     (1000) rider     (1000)   576312 2019-03-30 20:18:44.000000 django_reportbrod-4.1/django_reportbroD/static/assets/js/app.js
+-rw-r--r--   0 rider     (1000) rider     (1000)  8320860 2019-03-30 20:19:02.000000 django_reportbrod-4.1/django_reportbroD/static/assets/js/vendors.js
+drwxr-xr-x   0 rider     (1000) rider     (1000)        0 2024-05-29 14:03:36.318038 django_reportbrod-4.1/django_reportbroD/static/reportlib/
+drwxr-xr-x   0 rider     (1000) rider     (1000)        0 2024-05-29 14:03:36.321371 django_reportbrod-4.1/django_reportbroD/static/reportlib/css/
+drwxr-xr-x   0 rider     (1000) rider     (1000)        0 2024-05-29 14:03:36.321371 django_reportbrod-4.1/django_reportbroD/static/reportlib/css/iconfonts/
+drwxr-xr-x   0 rider     (1000) rider     (1000)        0 2024-05-29 14:03:36.321371 django_reportbrod-4.1/django_reportbroD/static/reportlib/css/iconfonts/fonts/
+-rw-r--r--   0 rider     (1000) rider     (1000)     1633 2024-02-14 15:51:44.000000 django_reportbrod-4.1/django_reportbroD/static/reportlib/css/iconfonts/fonts/demoapp.svg
+-rw-r--r--   0 rider     (1000) rider     (1000)     1384 2024-02-14 15:51:44.000000 django_reportbrod-4.1/django_reportbroD/static/reportlib/css/iconfonts/fonts/demoapp.ttf
+-rw-r--r--   0 rider     (1000) rider     (1000)     1460 2024-02-14 15:51:44.000000 django_reportbrod-4.1/django_reportbroD/static/reportlib/css/iconfonts/fonts/demoapp.woff
+-rw-r--r--   0 rider     (1000) rider     (1000)      684 2024-02-14 15:51:44.000000 django_reportbrod-4.1/django_reportbroD/static/reportlib/css/iconfonts/fonts/demoapp.woff2
+-rw-r--r--   0 rider     (1000) rider     (1000)      855 2024-02-14 15:51:44.000000 django_reportbrod-4.1/django_reportbroD/static/reportlib/css/iconfonts/style.css
+-rw-r--r--   0 rider     (1000) rider     (1000)     4509 2024-02-21 21:05:40.000000 django_reportbrod-4.1/django_reportbroD/static/reportlib/css/styles.css
+-rw-r--r--   0 rider     (1000) rider     (1000)     2238 2024-02-14 15:51:44.000000 django_reportbrod-4.1/django_reportbroD/static/reportlib/favicon.ico
+drwxr-xr-x   0 rider     (1000) rider     (1000)        0 2024-05-29 14:03:36.324705 django_reportbrod-4.1/django_reportbroD/static/reportlib/js/
+-rw-r--r--   0 rider     (1000) rider     (1000)   288580 2024-02-14 15:51:44.000000 django_reportbrod-4.1/django_reportbroD/static/reportlib/js/jquery-3.6.0.js
+-rw-r--r--   0 rider     (1000) rider     (1000)    89501 2024-02-14 15:51:44.000000 django_reportbrod-4.1/django_reportbroD/static/reportlib/js/jquery-3.6.0.min.js
+-rw-r--r--   0 rider     (1000) rider     (1000)     3121 2024-02-14 15:51:44.000000 django_reportbrod-4.1/django_reportbroD/static/reportlib/js/jquery.cookie.js
+-rw-r--r--   0 rider     (1000) rider     (1000)    55398 2024-02-21 20:18:44.000000 django_reportbrod-4.1/django_reportbroD/static/reportlib/reportbro.css
+-rw-r--r--   0 rider     (1000) rider     (1000)    77644 2024-02-21 20:18:44.000000 django_reportbrod-4.1/django_reportbroD/static/reportlib/reportbro.css.map
+-rw-r--r--   0 rider     (1000) rider     (1000)   733475 2024-05-18 23:36:56.000000 django_reportbrod-4.1/django_reportbroD/static/reportlib/reportbro.js
+-rw-r--r--   0 rider     (1000) rider     (1000)      665 2024-02-21 20:18:44.000000 django_reportbrod-4.1/django_reportbroD/static/reportlib/reportbro.js.LICENSE.txt
+-rw-r--r--   0 rider     (1000) rider     (1000)  2440768 2024-02-21 20:18:44.000000 django_reportbrod-4.1/django_reportbroD/static/reportlib/reportbro.js.map
+-rw-r--r--   0 rider     (1000) rider     (1000)   722287 2024-02-21 20:18:44.000000 django_reportbrod-4.1/django_reportbroD/static/reportlib/reportbro.min.js
+-rw-r--r--   0 rider     (1000) rider     (1000)   803864 2024-02-21 20:18:44.000000 django_reportbrod-4.1/django_reportbroD/static/reportlib/reportbro.min.js.map
+drwxr-xr-x   0 rider     (1000) rider     (1000)        0 2024-05-29 14:03:36.324705 django_reportbrod-4.1/django_reportbroD/static/reportlib/src/
+-rw-r--r--   0 rider     (1000) rider     (1000)    24374 2024-02-21 20:18:44.000000 django_reportbrod-4.1/django_reportbroD/static/reportlib/src/ajaxload.gif
+drwxr-xr-x   0 rider     (1000) rider     (1000)        0 2024-05-29 14:03:36.328038 django_reportbrod-4.1/django_reportbroD/static/reportlib/src/fonts/
+-rw-r--r--   0 rider     (1000) rider     (1000)    20756 2024-02-21 20:18:44.000000 django_reportbrod-4.1/django_reportbroD/static/reportlib/src/fonts/open-sans-v34-latin-300.woff
+-rw-r--r--   0 rider     (1000) rider     (1000)    16748 2024-02-21 20:18:44.000000 django_reportbrod-4.1/django_reportbroD/static/reportlib/src/fonts/open-sans-v34-latin-300.woff2
+-rw-r--r--   0 rider     (1000) rider     (1000)    20672 2024-02-21 20:18:44.000000 django_reportbrod-4.1/django_reportbroD/static/reportlib/src/fonts/open-sans-v34-latin-600.woff
+-rw-r--r--   0 rider     (1000) rider     (1000)    16756 2024-02-21 20:18:44.000000 django_reportbrod-4.1/django_reportbroD/static/reportlib/src/fonts/open-sans-v34-latin-600.woff2
+-rw-r--r--   0 rider     (1000) rider     (1000)    20664 2024-02-21 20:18:44.000000 django_reportbrod-4.1/django_reportbroD/static/reportlib/src/fonts/open-sans-v34-latin-800.woff
+-rw-r--r--   0 rider     (1000) rider     (1000)    16696 2024-02-21 20:18:44.000000 django_reportbrod-4.1/django_reportbroD/static/reportlib/src/fonts/open-sans-v34-latin-800.woff2
+-rw-r--r--   0 rider     (1000) rider     (1000)    20712 2024-02-21 20:18:44.000000 django_reportbrod-4.1/django_reportbroD/static/reportlib/src/fonts/open-sans-v34-latin-regular.woff
+-rw-r--r--   0 rider     (1000) rider     (1000)    16740 2024-02-21 20:18:44.000000 django_reportbrod-4.1/django_reportbroD/static/reportlib/src/fonts/open-sans-v34-latin-regular.woff2
+drwxr-xr-x   0 rider     (1000) rider     (1000)        0 2024-05-29 14:03:36.338038 django_reportbrod-4.1/django_reportbroD/static/reportlib/src/iconfonts/
+-rw-r--r--   0 rider     (1000) rider     (1000)    37788 2024-02-21 20:18:44.000000 django_reportbrod-4.1/django_reportbroD/static/reportlib/src/iconfonts/reportbro.svg
+-rw-r--r--   0 rider     (1000) rider     (1000)    12676 2024-02-21 20:18:44.000000 django_reportbrod-4.1/django_reportbroD/static/reportlib/src/iconfonts/reportbro.ttf
+-rw-r--r--   0 rider     (1000) rider     (1000)    12752 2024-02-21 20:18:44.000000 django_reportbrod-4.1/django_reportbroD/static/reportlib/src/iconfonts/reportbro.woff
+-rw-r--r--   0 rider     (1000) rider     (1000)     4460 2024-02-21 20:18:44.000000 django_reportbrod-4.1/django_reportbroD/static/reportlib/src/iconfonts/reportbro.woff2
+-rw-r--r--   0 rider     (1000) rider     (1000)    12924 2024-02-21 20:18:44.000000 django_reportbrod-4.1/django_reportbroD/static/reportlib/src/rb_logo_dark.png
+-rw-r--r--   0 rider     (1000) rider     (1000)    13606 2024-02-21 20:18:44.000000 django_reportbrod-4.1/django_reportbroD/static/reportlib/src/rb_logo_white.png
+drwxr-xr-x   0 rider     (1000) rider     (1000)        0 2024-05-29 14:03:36.341371 django_reportbrod-4.1/django_reportbroD/templates/
+drwxr-xr-x   0 rider     (1000) rider     (1000)        0 2024-05-29 14:03:36.341371 django_reportbrod-4.1/django_reportbroD/templates/bases/
+-rw-r--r--   0 rider     (1000) rider     (1000)     1942 2024-05-16 14:15:12.000000 django_reportbrod-4.1/django_reportbroD/templates/bases/base.html
+-rw-r--r--   0 rider     (1000) rider     (1000)      352 2024-04-15 00:52:16.000000 django_reportbrod-4.1/django_reportbroD/templates/bases/footer.html
+-rw-r--r--   0 rider     (1000) rider     (1000)     4205 2024-05-29 13:25:08.000000 django_reportbrod-4.1/django_reportbroD/templates/bases/header.html
+-rw-r--r--   0 rider     (1000) rider     (1000)      765 2024-05-29 13:28:42.000000 django_reportbrod-4.1/django_reportbroD/templates/bases/navigator.html
+-rw-r--r--   0 rider     (1000) rider     (1000)     1926 2024-05-17 14:02:34.000000 django_reportbrod-4.1/django_reportbroD/templates/create.html
+-rw-r--r--   0 rider     (1000) rider     (1000)    16761 2024-05-16 15:46:40.000000 django_reportbrod-4.1/django_reportbroD/templates/document.html
+-rw-r--r--   0 rider     (1000) rider     (1000)     2157 2024-05-17 14:00:38.000000 django_reportbrod-4.1/django_reportbroD/templates/edit.html
+-rw-r--r--   0 rider     (1000) rider     (1000)    21051 2024-05-17 13:57:14.000000 django_reportbrod-4.1/django_reportbroD/templates/especif.html
+-rw-r--r--   0 rider     (1000) rider     (1000)     1192 2024-05-17 14:18:06.000000 django_reportbrod-4.1/django_reportbroD/templates/formulario.html
+-rw-r--r--   0 rider     (1000) rider     (1000)     3102 2024-05-17 14:04:22.000000 django_reportbrod-4.1/django_reportbroD/templates/import.html
+-rw-r--r--   0 rider     (1000) rider     (1000)     8884 2024-05-13 14:01:34.000000 django_reportbrod-4.1/django_reportbroD/templates/index.html
+-rw-r--r--   0 rider     (1000) rider     (1000)     6454 2024-05-29 13:28:30.000000 django_reportbrod-4.1/django_reportbroD/templates/report.html
+-rw-r--r--   0 rider     (1000) rider     (1000)      751 2024-05-29 12:11:51.000000 django_reportbrod-4.1/django_reportbroD/urls.py
+-rw-r--r--   0 rider     (1000) rider     (1000)     4614 2024-05-29 12:11:51.000000 django_reportbrod-4.1/django_reportbroD/utils.py
+-rw-r--r--   0 rider     (1000) rider     (1000)     4435 2024-05-29 13:17:13.000000 django_reportbrod-4.1/django_reportbroD/views.py
+drwxr-xr-x   0 rider     (1000) rider     (1000)        0 2024-05-29 14:03:36.341371 django_reportbrod-4.1/django_reportbroD.egg-info/
+-rw-r--r--   0 rider     (1000) rider     (1000)     5733 2024-05-29 14:03:36.000000 django_reportbrod-4.1/django_reportbroD.egg-info/PKG-INFO
+-rw-r--r--   0 rider     (1000) rider     (1000)     8032 2024-05-29 14:03:36.000000 django_reportbrod-4.1/django_reportbroD.egg-info/SOURCES.txt
+-rw-r--r--   0 rider     (1000) rider     (1000)        1 2024-05-29 14:03:36.000000 django_reportbrod-4.1/django_reportbroD.egg-info/dependency_links.txt
+-rw-r--r--   0 rider     (1000) rider     (1000)       33 2024-05-29 14:03:36.000000 django_reportbrod-4.1/django_reportbroD.egg-info/requires.txt
+-rw-r--r--   0 rider     (1000) rider     (1000)       18 2024-05-29 14:03:36.000000 django_reportbrod-4.1/django_reportbroD.egg-info/top_level.txt
+-rw-r--r--   0 rider     (1000) rider     (1000)     1177 2024-05-29 14:03:36.344705 django_reportbrod-4.1/setup.cfg
+-rw-r--r--   0 rider     (1000) rider     (1000)       37 2024-02-21 17:28:39.000000 django_reportbrod-4.1/setup.py
```

### Comparing `django-reportbroD-4.0/PKG-INFO` & `django_reportbrod-4.1/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: django-reportbroD
-Version: 4.0
+Version: 4.1
 Summary: A Django app to create and use ReportBro reports with a sample admin. This allows you to generate yours reports using three options: by its code or name from database or JSON template.
 Author: Rider Raul Espinosa Perez
 Author-email: riderraule@gmail.com
 License: MIT
 Classifier: Environment :: Web Environment
 Classifier: Framework :: Django
 Classifier: Framework :: Django :: 5.0
@@ -17,68 +17,69 @@
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: Python :: 3.12
 Classifier: Topic :: Internet :: WWW/HTTP
 Classifier: Topic :: Internet :: WWW/HTTP :: Dynamic Content
 Requires-Python: >=3.8
 Description-Content-Type: text/markdown
+Requires-Dist: Django>=4.2
+Requires-Dist: reportbro-lib>=3.7.0
 
 # django-reportbroD
 A Django app to create, use and export ReportBro reports (free version) with a admin. 
 
 ![Django](https://img.shields.io/badge/django-%23092E20.svg?style=for-the-badge&logo=django&logoColor=white) ![lib](https://badgen.net/badge/Export/PDF-XLSX/red?) ![JS](https://badgen.net/badge/Js/Reportbro_Designer/blue?icon=doc)  ![lib](https://badgen.net/badge/Package/Reportbro-lib/red?icon=doc)
 
 Quick start
 -----------
 
 1. Add "django_reportbroD" to your INSTALLED_APPS setting like this:
 ```
-    INSTALLED_APPS = [
-   
-                ... ,
-   'django_reportbroD.apps.ReportbrodConfig',
-
+INSTALLED_APPS = [
+... ,
+'django_reportbroD.apps.ReportbrodConfig',
    ]
 
 ```
-2. Add LocaleMiddleware to your MIDDLEWARE list in your settings. This allows the reporting app to have translation in Spanish and English. 
+
+2. Include the reportbroD URLconf in your project urls.py like this:
+
+```
+   path("reportbroD/", include("django_reportbroD.urls", namespace="reportbroD")),  
+```
+
+
+3.  Run ``python manage.py migrate`` to create the models and to migrating to data base.
+
+4. Start the development server.
+
+5. Visit the ``/reportbroD/`` URL to create/update/edit/duplicate/remove reports.
+
+
+
+
+> **Traslations** 
+>
+>The next step is optional if you want to use in Spanish and English, otherwise it isn't necessary.
+
+1. Add LocaleMiddleware to your MIDDLEWARE list in your settings. This allows the reporting app to have translation in Spanish and English. 
  ```
         MIDDLEWARE = [
     'django.middleware.locale.LocaleMiddleware',
     ...
-            ],
-            
-        
+            ],  
 ```
 
-3. Add 'django_reportbroD.menus.get_menu_items' to your OPTIONS.context_processors in your TEMPLATES settings. This enables the use of menu for the installed report app. 
- ```
-        'OPTIONS': {
-   
-            'context_processors': [...,
-'django_reportbroD.menus.get_menu_items'
-   
-            ],
-            
-        }
-```
-
-4. Include the reportbroD URLconf in your project urls.py and the i18n urls like this:
+1. Include the i18N URLconf in your project urls.py like this:
 
 ```
-   path("reportbroD/", include("django_reportbroD.urls" namespace="reportbroD")),  
-   path('i18n/', include('django.conf.urls.i18n')),
+   path("i18n/", include("django.conf.urls.i18n")),  
 ```
 
 
-5.  Run ``python manage.py migrate`` to create the models and to migrating to data base.
-
-6. Start the development server.
-
-7. Visit the ``/reportbroD/`` URL to create/update/edit/duplicate/remove reports.
 
 
 Using report
 -----------
 
 1. Create a app to using the view file or other file .py for defining the view function to show/export selected report
  ```
```

### Comparing `django-reportbroD-4.0/README.md` & `django_reportbrod-4.1/README.md`

 * *Files 7% similar despite different names*

```diff
@@ -4,57 +4,56 @@
 ![Django](https://img.shields.io/badge/django-%23092E20.svg?style=for-the-badge&logo=django&logoColor=white) ![lib](https://badgen.net/badge/Export/PDF-XLSX/red?) ![JS](https://badgen.net/badge/Js/Reportbro_Designer/blue?icon=doc)  ![lib](https://badgen.net/badge/Package/Reportbro-lib/red?icon=doc)
 
 Quick start
 -----------
 
 1. Add "django_reportbroD" to your INSTALLED_APPS setting like this:
 ```
-    INSTALLED_APPS = [
-   
-                ... ,
-   'django_reportbroD.apps.ReportbrodConfig',
-
+INSTALLED_APPS = [
+... ,
+'django_reportbroD.apps.ReportbrodConfig',
    ]
 
 ```
-2. Add LocaleMiddleware to your MIDDLEWARE list in your settings. This allows the reporting app to have translation in Spanish and English. 
+
+2. Include the reportbroD URLconf in your project urls.py like this:
+
+```
+   path("reportbroD/", include("django_reportbroD.urls", namespace="reportbroD")),  
+```
+
+
+3.  Run ``python manage.py migrate`` to create the models and to migrating to data base.
+
+4. Start the development server.
+
+5. Visit the ``/reportbroD/`` URL to create/update/edit/duplicate/remove reports.
+
+
+
+
+> **Traslations** 
+>
+>The next step is optional if you want to use in Spanish and English, otherwise it isn't necessary.
+
+1. Add LocaleMiddleware to your MIDDLEWARE list in your settings. This allows the reporting app to have translation in Spanish and English. 
  ```
         MIDDLEWARE = [
     'django.middleware.locale.LocaleMiddleware',
     ...
-            ],
-            
-        
+            ],  
 ```
 
-3. Add 'django_reportbroD.menus.get_menu_items' to your OPTIONS.context_processors in your TEMPLATES settings. This enables the use of menu for the installed report app. 
- ```
-        'OPTIONS': {
-   
-            'context_processors': [...,
-'django_reportbroD.menus.get_menu_items'
-   
-            ],
-            
-        }
-```
-
-4. Include the reportbroD URLconf in your project urls.py and the i18n urls like this:
+1. Include the i18N URLconf in your project urls.py like this:
 
 ```
-   path("reportbroD/", include("django_reportbroD.urls" namespace="reportbroD")),  
-   path('i18n/', include('django.conf.urls.i18n')),
+   path("i18n/", include("django.conf.urls.i18n")),  
 ```
 
 
-5.  Run ``python manage.py migrate`` to create the models and to migrating to data base.
-
-6. Start the development server.
-
-7. Visit the ``/reportbroD/`` URL to create/update/edit/duplicate/remove reports.
 
 
 Using report
 -----------
 
 1. Create a app to using the view file or other file .py for defining the view function to show/export selected report
  ```
```

### Comparing `django-reportbroD-4.0/django_reportbroD/base.py` & `django_reportbrod-4.1/django_reportbroD/base.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,30 +1,27 @@
 import datetime
 import decimal
 import json
-from .models import ReportDefinition
 
+from .models import ReportDefinition
 
 
 def create_base_report_template(name):
     # use a predefined report definition so you don't have to start from scratch in this demo app,
     # for a real world app you would probably start with an empty report if nothing was saved previously
 
     report_definition = ""
 
     ReportDefinition.objects.create(
         name=name,
         report_definition=json.dumps(report_definition),
-        last_modified_at=datetime.datetime.now())
-
-
+        last_modified_at=datetime.datetime.now(),
+    )
 
 
 def json_default(obj):
     """Serializes decimal and date values, can be used for json encoder."""
     if isinstance(obj, decimal.Decimal):
         return float(obj)
     if isinstance(obj, datetime.date):
         return str(obj)
     raise TypeError
-
-
```

### Comparing `django-reportbroD-4.0/django_reportbroD/forms.py` & `django_reportbrod-4.1/django_reportbroD/forms.py`

 * *Files 26% similar despite different names*

```diff
@@ -1,32 +1,44 @@
 from django import forms
+from django.utils.translation import gettext_lazy as _
+
 from .models import ReportDefinition
-from django.utils.translation import gettext_lazy  as _
+
 
 class ReportForm(forms.ModelForm):
 
     class Meta:
-        model=ReportDefinition
-        fields=['name', 'remark']
-        labels={
-            
-             'name':'Nombre',
-            'remark':'Descripcion'
-
+        model = ReportDefinition
+        fields = ["name", "remark"]
+        labels = {"name": "Nombre", "remark": "Descripcion"}
+
+        widgets = {
+            "name": forms.TextInput(
+                attrs={
+                    "class": "form-control",
+                    "id": "nombre",
+                    "placeholder": _("holdern"),
+                }
+            ),
+            "remark": forms.Textarea(
+                attrs={
+                    "class": "form-control",
+                    "rows": "3",
+                    "id": "desc",
+                    "placeholder": _("holderd"),
+                }
+            ),
         }
 
-        widgets={
-           'name':forms.TextInput(attrs={"class":"form-control", "id":"nombre" , "placeholder": _("holdern")}),
-            'remark':forms.Textarea(attrs={"class":"form-control", "rows":"3" ,"id":"desc" ,"placeholder": _("holderd")}),
-            
-            }  
-
-
 
 class ReportImpForm(forms.Form):
 
-    template= forms.FileField(label="Plantilla",widget=forms.FileInput(attrs={"class":"form-control-file","id":"filetemplate", "placeholder": _("holderf")}))
-
-    
-
-
-      
+    template = forms.FileField(
+        label="Plantilla",
+        widget=forms.FileInput(
+            attrs={
+                "class": "form-control-file",
+                "id": "filetemplate",
+                "placeholder": _("holderf"),
+            }
+        ),
+    )
```

### Comparing `django-reportbroD-4.0/django_reportbroD/locale/en/LC_MESSAGES/django.mo` & `django_reportbrod-4.1/django_reportbroD/locale/en/LC_MESSAGES/django.mo`

 * *Files identical despite different names*

### Comparing `django-reportbroD-4.0/django_reportbroD/locale/en/LC_MESSAGES/django.po` & `django_reportbrod-4.1/django_reportbroD/locale/en/LC_MESSAGES/django.po`

 * *Files identical despite different names*

### Comparing `django-reportbroD-4.0/django_reportbroD/locale/es/LC_MESSAGES/django.mo` & `django_reportbrod-4.1/django_reportbroD/locale/es/LC_MESSAGES/django.mo`

 * *Files identical despite different names*

### Comparing `django-reportbroD-4.0/django_reportbroD/locale/es/LC_MESSAGES/django.po` & `django_reportbrod-4.1/django_reportbroD/locale/es/LC_MESSAGES/django.po`

 * *Files identical despite different names*

### Comparing `django-reportbroD-4.0/django_reportbroD/migrations/0001_initial.py` & `django_reportbrod-4.1/django_reportbroD/migrations/0001_initial.py`

 * *Files 19% similar despite different names*

```diff
@@ -1,46 +1,75 @@
 # Generated by Django 5.0.2 on 2024-05-15 13:06
 
 import datetime
+
 from django.db import migrations, models
 
 
 class Migration(migrations.Migration):
 
     initial = True
 
-    dependencies = [
-    ]
+    dependencies = []
 
     operations = [
         migrations.CreateModel(
-            name='ReportDefinition',
+            name="ReportDefinition",
             fields=[
-                ('id', models.BigAutoField(auto_created=True, primary_key=True, serialize=False, verbose_name='ID')),
-                ('report_definition', models.TextField(default='""')),
-                ('name', models.CharField(max_length=200, unique=True, verbose_name='Nombre')),
-                ('remark', models.TextField(blank=True, null=True, verbose_name='Descripción')),
-                ('last_modified_at', models.DateTimeField(default=datetime.datetime(2024, 5, 15, 13, 6, 41, 537274))),
+                (
+                    "id",
+                    models.BigAutoField(
+                        auto_created=True,
+                        primary_key=True,
+                        serialize=False,
+                        verbose_name="ID",
+                    ),
+                ),
+                ("report_definition", models.TextField(default='""')),
+                (
+                    "name",
+                    models.CharField(
+                        max_length=200, unique=True, verbose_name="Nombre"
+                    ),
+                ),
+                (
+                    "remark",
+                    models.TextField(blank=True, null=True, verbose_name="Descripción"),
+                ),
+                (
+                    "last_modified_at",
+                    models.DateTimeField(
+                        default=datetime.datetime(2024, 5, 15, 13, 6, 41, 537274)
+                    ),
+                ),
             ],
             options={
-                'verbose_name': 'Reporte',
-                'verbose_name_plural': 'Reportes',
-                'db_table': 'report_definition',
+                "verbose_name": "Reporte",
+                "verbose_name_plural": "Reportes",
+                "db_table": "report_definition",
             },
         ),
         migrations.CreateModel(
-            name='ReportRequest',
+            name="ReportRequest",
             fields=[
-                ('id', models.BigAutoField(auto_created=True, primary_key=True, serialize=False, verbose_name='ID')),
-                ('key', models.CharField(max_length=36)),
-                ('report_definition', models.TextField()),
-                ('data', models.TextField()),
-                ('is_test_data', models.BooleanField()),
-                ('pdf_file', models.BinaryField(null=True)),
-                ('pdf_file_size', models.IntegerField(null=True)),
-                ('created_on', models.DateTimeField()),
+                (
+                    "id",
+                    models.BigAutoField(
+                        auto_created=True,
+                        primary_key=True,
+                        serialize=False,
+                        verbose_name="ID",
+                    ),
+                ),
+                ("key", models.CharField(max_length=36)),
+                ("report_definition", models.TextField()),
+                ("data", models.TextField()),
+                ("is_test_data", models.BooleanField()),
+                ("pdf_file", models.BinaryField(null=True)),
+                ("pdf_file_size", models.IntegerField(null=True)),
+                ("created_on", models.DateTimeField()),
             ],
             options={
-                'db_table': 'report_request',
+                "db_table": "report_request",
             },
         ),
     ]
```

### Comparing `django-reportbroD-4.0/django_reportbroD/models.py` & `django_reportbrod-4.1/django_reportbroD/models.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,28 +1,27 @@
-from django.db import models
-from datetime import datetime
 import json
-from django.utils.translation import gettext as _
-
+from datetime import datetime
 
+from django.db import models
+from django.utils.translation import gettext as _
 
 
 # store report requests for testing, used by ReportBro Designer
 # for preview of pdf and xlsx
 class ReportRequest(models.Model):
     key = models.CharField(max_length=36)
     report_definition = models.TextField()
     data = models.TextField()
     is_test_data = models.BooleanField()
     pdf_file = models.BinaryField(null=True)
     pdf_file_size = models.IntegerField(null=True)
     created_on = models.DateTimeField()
 
     class Meta:
-        db_table = 'report_request'
+        db_table = "report_request"
 
 
 # report definition for our album report which is used for printing
 # the pdf with the album list. When the report is saved
 # in ReportBro Designer it will be stored in this table.
 class ReportDefinition(models.Model):
     report_definition = models.TextField(default=json.dumps(""))
@@ -30,28 +29,27 @@
     remark = models.TextField(null=True, blank=True, verbose_name="Descripción")
     last_modified_at = models.DateTimeField(default=datetime.now())
 
     def unique_error_message(self, model_class, unique_check):
         if model_class == type(self) and unique_check == ("name",):
             return _("unique")
         else:
-            return super(ReportDefinition, self).unique_error_message(model_class, unique_check)
+            return super(ReportDefinition, self).unique_error_message(
+                model_class, unique_check
+            )
 
     class Meta:
-        db_table = 'report_definition'
-        verbose_name='Reporte'
-        verbose_name_plural='Reportes'
-        
+        db_table = "report_definition"
+        verbose_name = "Reporte"
+        verbose_name_plural = "Reportes"
 
     def __str__(self):
-        
+
         return self.name
-    
+
     def to_dict(self):
         return {
-            "report_definition":self.report_definition,
-            "name":self.name,
-            "remark":self.remark,
-            "last_modified_at":self.last_modified_at.isoformat()
-
+            "report_definition": self.report_definition,
+            "name": self.name,
+            "remark": self.remark,
+            "last_modified_at": self.last_modified_at.isoformat(),
         }
-
```

### Comparing `django-reportbroD-4.0/django_reportbroD/reportcore.py` & `django_reportbrod-4.1/django_reportbroD/reportcore.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,23 +1,23 @@
 import datetime
 import json
 import uuid
+from timeit import default_timer as timer
 
 from django.db.models import Sum
-from django.http import HttpResponseBadRequest, HttpResponse, HttpResponseServerError
+from django.http import (HttpResponse, HttpResponseBadRequest,HttpResponseServerError)
 from django.shortcuts import render
 from django.utils.safestring import SafeString
 from django.views.decorators.clickjacking import xframe_options_exempt
 from django.views.decorators.csrf import csrf_exempt, ensure_csrf_cookie
 from reportbro import Report, ReportBroError
-from timeit import default_timer as timer
-from .models import ReportDefinition, ReportRequest
-from .base import json_default, create_base_report_template
-
 
+from .base import create_base_report_template, json_default
+from .models import ReportDefinition, ReportRequest
+from .menus import get_menu_items, reportbro_langs 
 
 MAX_CACHE_SIZE = 1000 * 1024 * 1024  # keep max. 1000 MB of generated pdf files in db
 
 
 @ensure_csrf_cookie
 def edit(request, pk):
     """Shows a page with ReportBro Designer to edit our report template.
@@ -30,248 +30,301 @@
     """
     context = dict()
     if ReportDefinition.objects.filter(pk=pk).count() == 0:
         create_base_report_template(pk)
 
     # load ReportBro report definition stored in our report_definition table
     row = ReportDefinition.objects.get(pk=pk)
-    context['report_definition'] = SafeString(row.report_definition)
-    context['name'] = row.name
-    context['pk'] = pk
-    return render(request, 'report.html', context)
+    context["report_definition"] = SafeString(row.report_definition)
+    context["name"] = row.name
+    context["pk"] = pk
+    context["active_page"] = "reportlist"
+    context["menu"]=get_menu_items()
+    context["reportbro_langs"]=reportbro_langs()
+    return render(request, "report.html", context)
 
 
 @xframe_options_exempt
 @csrf_exempt
 def run(request):
     """Generates a report for preview.
 
     This method is called by ReportBro Designer when the Preview button is clicked,
     the url is defined when initializing the Designer, see *reportServerUrl*
     in templates/albums/report/edit.html
     """
     now = datetime.datetime.now()
 
-    response = HttpResponse('')
-    response['Access-Control-Allow-Origin'] = '*'
-    response['Access-Control-Allow-Methods'] = 'GET, PUT, OPTIONS'
-    response['Access-Control-Allow-Headers'] =\
-        'Origin, X-Requested-With, X-HTTP-Method-Override, Content-Type, Accept, Authorization, Z-Key'
-    if request.method == 'OPTIONS':
+    response = HttpResponse("")
+    response["Access-Control-Allow-Origin"] = "*"
+    response["Access-Control-Allow-Methods"] = "GET, PUT, OPTIONS"
+    response["Access-Control-Allow-Headers"] = (
+        "Origin, X-Requested-With, X-HTTP-Method-Override, Content-Type, Accept, Authorization, Z-Key"
+    )
+    if request.method == "OPTIONS":
         # options request is usually sent by browser for a cross-site request, we only need to set the
         # Access-Control-Allow headers in the response so the browser sends the following get/put request
         return response
 
     additional_fonts = []
     # add additional fonts here if additional fonts are used in ReportBro Designer
 
-    if request.method == 'PUT':
+    if request.method == "PUT":
         # all data needed for report preview is sent in the initial PUT request, it contains
         # the format (pdf or xlsx), the report itself (report_definition), the data (test data
         # defined within parameters in the Designer) and is_test_data flag (always True
         # when request is sent from Designer)
-        json_data = json.loads(request.body.decode('utf-8'))
-        if not isinstance(json_data, dict) or not isinstance(json_data.get('report'), dict) or\
-                not isinstance(json_data.get('data'), dict) or not isinstance(json_data.get('isTestData'), bool):
-            return HttpResponseBadRequest('invalid report values')
-
-        output_format = json_data.get('outputFormat')
-        if output_format not in ('pdf', 'xlsx'):
-            return HttpResponseBadRequest('outputFormat parameter missing or invalid')
-
-        report_definition = json_data.get('report')
-        data = json_data.get('data')
-        is_test_data = json_data.get('isTestData')
+        json_data = json.loads(request.body.decode("utf-8"))
+        if (
+            not isinstance(json_data, dict)
+            or not isinstance(json_data.get("report"), dict)
+            or not isinstance(json_data.get("data"), dict)
+            or not isinstance(json_data.get("isTestData"), bool)
+        ):
+            return HttpResponseBadRequest("invalid report values")
+
+        output_format = json_data.get("outputFormat")
+        if output_format not in ("pdf", "xlsx"):
+            return HttpResponseBadRequest("outputFormat parameter missing or invalid")
+
+        report_definition = json_data.get("report")
+        data = json_data.get("data")
+        is_test_data = json_data.get("isTestData")
         try:
-            report = Report(report_definition, data, is_test_data, additional_fonts=additional_fonts)
+            report = Report(
+                report_definition, data, is_test_data, additional_fonts=additional_fonts
+            )
         except Exception as e:
-            return HttpResponseBadRequest('failed to initialize report: ' + str(e))
+            return HttpResponseBadRequest("failed to initialize report: " + str(e))
 
         if report.errors:
             # return list of errors in case report contains errors, e.g. duplicate parameters.
             # with this information ReportBro Designer can select object containing errors,
             # highlight erroneous fields and display error messages
             return HttpResponse(json.dumps(dict(errors=report.errors)))
         try:
             # delete old reports (older than 3 minutes) to avoid table getting too big
-            ReportRequest.objects.filter(created_on__lt=(now - datetime.timedelta(minutes=3))).delete()
-
-            total_size = ReportRequest.objects.aggregate(Sum('pdf_file_size'))
-            if total_size['pdf_file_size__sum'] and total_size['pdf_file_size__sum'] > MAX_CACHE_SIZE:
+            ReportRequest.objects.filter(
+                created_on__lt=(now - datetime.timedelta(minutes=3))
+            ).delete()
+
+            total_size = ReportRequest.objects.aggregate(Sum("pdf_file_size"))
+            if (
+                total_size["pdf_file_size__sum"]
+                and total_size["pdf_file_size__sum"] > MAX_CACHE_SIZE
+            ):
                 # delete all reports older than 10 seconds to reduce db size for cached pdf files
-                ReportRequest.objects.filter(created_on__lt=(now - datetime.timedelta(seconds=10))).delete()
+                ReportRequest.objects.filter(
+                    created_on__lt=(now - datetime.timedelta(seconds=10))
+                ).delete()
 
             start = timer()
             report_file = report.generate_pdf()
             end = timer()
-            print('pdf generated in %.3f seconds' % (end-start))
+            print("pdf generated in %.3f seconds" % (end - start))
 
             key = str(uuid.uuid4())
             # add report request into sqlite db, this enables downloading the report by url
             # (the report is identified by the key) without any post parameters.
             # This is needed for pdf and xlsx preview.
             ReportRequest.objects.create(
-                key=key, report_definition=json.dumps(report_definition, default=json_default),
-                data=json.dumps(data, default=json_default), is_test_data=is_test_data,
-                pdf_file=report_file, pdf_file_size=len(report_file), created_on=now)
+                key=key,
+                report_definition=json.dumps(report_definition, default=json_default),
+                data=json.dumps(data, default=json_default),
+                is_test_data=is_test_data,
+                pdf_file=report_file,
+                pdf_file_size=len(report_file),
+                created_on=now,
+            )
 
-            return HttpResponse('key:' + key)
+            return HttpResponse("key:" + key)
         except ReportBroError as err:
             # in case an error occurs during report generation a ReportBroError exception is thrown
             # to stop processing. We return this error within a list so the error can be
             # processed by ReportBro Designer.
             return HttpResponse(json.dumps(dict(errors=[err.error])))
 
-    elif request.method == 'GET':
-        output_format = request.GET.get('outputFormat')
-        if output_format not in ('pdf', 'xlsx'):
-            return HttpResponseBadRequest('outputFormat parameter missing or invalid')
-        key = request.GET.get('key')
+    elif request.method == "GET":
+        output_format = request.GET.get("outputFormat")
+        if output_format not in ("pdf", "xlsx"):
+            return HttpResponseBadRequest("outputFormat parameter missing or invalid")
+        key = request.GET.get("key")
 
         report = None
         report_file = None
         if key and len(key) == 36:
             # the report is identified by a key which was saved
             # in a table during report preview with a PUT request
             try:
                 report_request = ReportRequest.objects.get(key=key)
             except ReportRequest.DoesNotExist:
                 return HttpResponseBadRequest(
-                    'report not found (preview probably too old), update report preview and try again')
-            if output_format == 'pdf' and report_request.pdf_file:
+                    "report not found (preview probably too old), update report preview and try again"
+                )
+            if output_format == "pdf" and report_request.pdf_file:
                 report_file = report_request.pdf_file
             else:
                 report_definition = json.loads(report_request.report_definition)
                 data = json.loads(report_request.data)
                 is_test_data = report_request.is_test_data
-                report = Report(report_definition, data, is_test_data, additional_fonts=additional_fonts)
+                report = Report(
+                    report_definition,
+                    data,
+                    is_test_data,
+                    additional_fonts=additional_fonts,
+                )
                 if report.errors:
-                    return HttpResponseBadRequest(reason='error generating report')
+                    return HttpResponseBadRequest(reason="error generating report")
         else:
             # in case there is a GET request without a key we expect all report data to be available.
             # this is NOT used by ReportBro Designer and only added for the sake of completeness.
-            json_data = json.loads(request.body.decode('utf-8'))
-            if not isinstance(json_data, dict) or not isinstance(json_data.get('report'), dict) or\
-                    not isinstance(json_data.get('data'), dict) or not isinstance(json_data.get('isTestData'), bool):
-                return HttpResponseBadRequest('invalid report values')
-            report_definition = json_data.get('report')
-            data = json_data.get('data')
-            is_test_data = json_data.get('isTestData')
+            json_data = json.loads(request.body.decode("utf-8"))
+            if (
+                not isinstance(json_data, dict)
+                or not isinstance(json_data.get("report"), dict)
+                or not isinstance(json_data.get("data"), dict)
+                or not isinstance(json_data.get("isTestData"), bool)
+            ):
+                return HttpResponseBadRequest("invalid report values")
+            report_definition = json_data.get("report")
+            data = json_data.get("data")
+            is_test_data = json_data.get("isTestData")
             if not isinstance(report_definition, dict) or not isinstance(data, dict):
-                return HttpResponseBadRequest('report_definition or data missing')
-            report = Report(report_definition, data, is_test_data, additional_fonts=additional_fonts)
+                return HttpResponseBadRequest("report_definition or data missing")
+            report = Report(
+                report_definition, data, is_test_data, additional_fonts=additional_fonts
+            )
             if report.errors:
-                return HttpResponseBadRequest(reason='error generating report')
+                return HttpResponseBadRequest(reason="error generating report")
 
         try:
             # once we have the reportbro.Report instance we can generate
             # the report (pdf or xlsx) and return it
-            if output_format == 'pdf':
+            if output_format == "pdf":
                 if report_file is None:
                     # as it is currently implemented the pdf file is always stored in the
                     # report_request table along the other report data. Therefor report_file
                     # will always be set. The generate_pdf call here is only needed in case
                     # the code is changed to clear report_request.pdf_file column when the
                     # data in this table gets too big (currently whole table rows are deleted)
                     report_file = report.generate_pdf()
-                response = HttpResponse(
-                    report_file, content_type='application/pdf')
-                response['Content-Disposition'] = 'inline; filename="{filename}"'.format(
-                    filename='report-' + str(now) + '.pdf')
+                response = HttpResponse(report_file, content_type="application/pdf")
+                response["Content-Disposition"] = (
+                    'inline; filename="{filename}"'.format(
+                        filename="report-" + str(now) + ".pdf"
+                    )
+                )
             else:
                 report_file = report.generate_xlsx()
                 response = HttpResponse(
-                    report_file, content_type='application/vnd.openxmlformats-officedocument.spreadsheetml.sheet')
-                response['Content-Disposition'] = 'inline; filename="{filename}"'.format(
-                    filename='report-' + str(now) + '.xlsx')
+                    report_file,
+                    content_type="application/vnd.openxmlformats-officedocument.spreadsheetml.sheet",
+                )
+                response["Content-Disposition"] = (
+                    'inline; filename="{filename}"'.format(
+                        filename="report-" + str(now) + ".xlsx"
+                    )
+                )
             return response
         except ReportBroError:
-            return HttpResponseBadRequest('error generating report')
+            return HttpResponseBadRequest("error generating report")
     return None
 
 
 def save(request, pk):
     """Save report_definition in our db table.
 
     This method is called by save button in ReportBro Designer.
     The url is called in *saveReport* callback from the Designer,
     see *saveCallback* in templates/albums/report/edit.html
     """
 
-    json_data = json.loads(request.body.decode('utf-8'))
+    json_data = json.loads(request.body.decode("utf-8"))
 
     # perform some basic checks if all necessary fields for report_definition are present
-    if not isinstance(json_data, dict) or not isinstance(json_data.get('docElements'), list) or\
-            not isinstance(json_data.get('styles'), list) or not isinstance(json_data.get('parameters'), list) or\
-            not isinstance(json_data.get('documentProperties'), dict) or not isinstance(json_data.get('version'), int):
-        return HttpResponseBadRequest('invalid values')
-
-    report_definition = json.dumps(dict(
-        docElements=json_data.get('docElements'), styles=json_data.get('styles'),
-        parameters=json_data.get('parameters'),
-        documentProperties=json_data.get('documentProperties'), version=json_data.get('version')))
+    if (
+        not isinstance(json_data, dict)
+        or not isinstance(json_data.get("docElements"), list)
+        or not isinstance(json_data.get("styles"), list)
+        or not isinstance(json_data.get("parameters"), list)
+        or not isinstance(json_data.get("documentProperties"), dict)
+        or not isinstance(json_data.get("version"), int)
+    ):
+        return HttpResponseBadRequest("invalid values")
+
+    report_definition = json.dumps(
+        dict(
+            docElements=json_data.get("docElements"),
+            styles=json_data.get("styles"),
+            parameters=json_data.get("parameters"),
+            documentProperties=json_data.get("documentProperties"),
+            version=json_data.get("version"),
+        )
+    )
 
     now = datetime.datetime.now()
-    if ReportDefinition.objects.filter(pk=pk).update(
-            report_definition=report_definition, last_modified_at=now) == 0:
+    if (
+        ReportDefinition.objects.filter(pk=pk).update(
+            report_definition=report_definition, last_modified_at=now
+        )
+        == 0
+    ):
         ReportDefinition.objects.create(
-            name=str(pk)+" reporte",
-            report_definition=report_definition, 
-            last_modified_at=now)
-    return HttpResponse('ok')
-
-
+            name=str(pk) + " reporte",
+            report_definition=report_definition,
+            last_modified_at=now,
+        )
+    return HttpResponse("ok")
 
 
 def reportPDF(report_definition, data, file="reporte", download=False):
-    """Prints a pdf file with the available data. 
-
-    """
+    """Prints a pdf file with the available data."""
     # if ReportDefinition.objects.filter(pk=code)== None:
     #     create_base_report_template(code)
-    
-#attachment
-    view_mode="attachment" if download else "inline"
+
+    # attachment
+    view_mode = "attachment" if download else "inline"
     try:
         report_inst = Report(json.loads(report_definition), data)
-        
+
         if report_inst.errors:
             # report definition should never contain any errors,
             # unless you saved an invalid report and didn't test in ReportBro Designer
             raise ReportBroError(report_inst.errors[0])
-        
+
         pdf_report = report_inst.generate_pdf()
 
-        response = HttpResponse(bytes(pdf_report), content_type='application/pdf')
-        response['Content-Disposition'] = '{view_mode}; filename="{filename}"'.format(filename=f"{file}.pdf", view_mode=view_mode)
-        
+        response = HttpResponse(bytes(pdf_report), content_type="application/pdf")
+        response["Content-Disposition"] = '{view_mode}; filename="{filename}"'.format(
+            filename=f"{file}.pdf", view_mode=view_mode
+        )
+
         return response
     except ReportBroError as ex:
-        return HttpResponseServerError('report error: ' + str(ex.error))
+        return HttpResponseServerError("report error: " + str(ex.error))
     except Exception as ex:
-        return HttpResponseServerError('report exception: ' + str(ex))
-    
+        return HttpResponseServerError("report exception: " + str(ex))
 
 
 def reportXLSX(report_definition, data, file="reporte"):
-    """Prints a xlsx file with the available data. 
-
-    """
+    """Prints a xlsx file with the available data."""
     # if ReportDefinition.objects.filter(pk=code)== None:
     #     create_base_report_template(code)
     try:
         report_inst = Report(json.loads(report_definition), data)
-        
+
         if report_inst.errors:
             # report definition should never contain any errors,
             # unless you saved an invalid report and didn't test in ReportBro Designer
             raise ReportBroError(report_inst.errors[0])
-        
+
         pdf_report = report_inst.generate_xlsx()
-        
-        response = HttpResponse(bytes(pdf_report), content_type='application/xlsx')
-        response['Content-Disposition'] = 'inline ; filename="{filename}"'.format(filename=f"{file}.xlsx")
+
+        response = HttpResponse(bytes(pdf_report), content_type="application/xlsx")
+        response["Content-Disposition"] = 'inline ; filename="{filename}"'.format(
+            filename=f"{file}.xlsx"
+        )
         return response
     except ReportBroError as ex:
-        return HttpResponseServerError('report error: ' + str(ex.error))
+        return HttpResponseServerError("report error: " + str(ex.error))
     except Exception as ex:
-        return HttpResponseServerError('report exception: ' + str(ex))
+        return HttpResponseServerError("report exception: " + str(ex))
```

### Comparing `django-reportbroD-4.0/django_reportbroD/static/assets/css/mCSB_buttons.html` & `django_reportbrod-4.1/django_reportbroD/static/assets/css/mCSB_buttons.html`

 * *Files identical despite different names*

### Comparing `django-reportbroD-4.0/django_reportbroD/static/assets/css/owl.video.play.html` & `django_reportbrod-4.1/django_reportbroD/static/assets/css/owl.video.play.html`

 * *Files identical despite different names*

### Comparing `django-reportbroD-4.0/django_reportbroD/static/assets/css/style.css` & `django_reportbrod-4.1/django_reportbroD/static/assets/css/style.css`

 * *Files identical despite different names*

### Comparing `django-reportbroD-4.0/django_reportbroD/static/assets/css/vendors.css` & `django_reportbrod-4.1/django_reportbroD/static/assets/css/vendors.css`

 * *Files identical despite different names*

### Comparing `django-reportbroD-4.0/django_reportbroD/static/assets/fonts/cryptocurrency-icons.eot` & `django_reportbrod-4.1/django_reportbroD/static/assets/fonts/cryptocurrency-icons.eot`

 * *Files identical despite different names*

### Comparing `django-reportbroD-4.0/django_reportbroD/static/assets/fonts/cryptocurrency-icons.html` & `django_reportbrod-4.1/django_reportbroD/static/assets/fonts/cryptocurrency-icons.html`

 * *Files identical despite different names*

### Comparing `django-reportbroD-4.0/django_reportbroD/static/assets/fonts/cryptocurrency-icons.svg` & `django_reportbrod-4.1/django_reportbroD/static/assets/fonts/cryptocurrency-icons.svg`

 * *Files identical despite different names*

### Comparing `django-reportbroD-4.0/django_reportbroD/static/assets/fonts/cryptocurrency-icons.ttf` & `django_reportbrod-4.1/django_reportbroD/static/assets/fonts/cryptocurrency-icons.ttf`

 * *Files identical despite different names*

### Comparing `django-reportbroD-4.0/django_reportbroD/static/assets/fonts/cryptocurrency-icons.woff` & `django_reportbrod-4.1/django_reportbroD/static/assets/fonts/cryptocurrency-icons.woff`

 * *Files identical despite different names*

### Comparing `django-reportbroD-4.0/django_reportbroD/static/assets/fonts/cryptocurrency-iconsd41d.eot` & `django_reportbrod-4.1/django_reportbroD/static/assets/fonts/cryptocurrency-iconsd41d.eot`

 * *Files identical despite different names*

### Comparing `django-reportbroD-4.0/django_reportbroD/static/assets/fonts/dashicons.eot` & `django_reportbrod-4.1/django_reportbroD/static/assets/fonts/dashicons.eot`

 * *Files identical despite different names*

### Comparing `django-reportbroD-4.0/django_reportbroD/static/assets/fonts/dashicons.html` & `django_reportbrod-4.1/django_reportbroD/static/assets/fonts/dashicons.html`

 * *Files identical despite different names*

### Comparing `django-reportbroD-4.0/django_reportbroD/static/assets/fonts/dashicons.svg` & `django_reportbrod-4.1/django_reportbroD/static/assets/fonts/dashicons.svg`

 * *Files identical despite different names*

### Comparing `django-reportbroD-4.0/django_reportbroD/static/assets/fonts/dashicons.ttf` & `django_reportbrod-4.1/django_reportbroD/static/assets/fonts/dashicons.ttf`

 * *Files identical despite different names*

### Comparing `django-reportbroD-4.0/django_reportbroD/static/assets/fonts/dashicons.woff` & `django_reportbrod-4.1/django_reportbroD/static/assets/fonts/dashicons.woff`

 * *Files identical despite different names*

### Comparing `django-reportbroD-4.0/django_reportbroD/static/assets/fonts/dashiconsd41d.eot` & `django_reportbrod-4.1/django_reportbroD/static/assets/fonts/dashiconsd41d.eot`

 * *Files identical despite different names*

### Comparing `django-reportbroD-4.0/django_reportbroD/static/assets/fonts/dripicons.eot` & `django_reportbrod-4.1/django_reportbroD/static/assets/fonts/dripicons.eot`

 * *Files identical despite different names*

### Comparing `django-reportbroD-4.0/django_reportbroD/static/assets/fonts/dripicons.svg` & `django_reportbrod-4.1/django_reportbroD/static/assets/fonts/dripicons.svg`

 * *Files identical despite different names*

### Comparing `django-reportbroD-4.0/django_reportbroD/static/assets/fonts/dripicons.ttf` & `django_reportbrod-4.1/django_reportbroD/static/assets/fonts/dripicons.ttf`

 * *Files identical despite different names*

### Comparing `django-reportbroD-4.0/django_reportbroD/static/assets/fonts/dripicons.woff` & `django_reportbrod-4.1/django_reportbroD/static/assets/fonts/dripicons.woff`

 * *Files identical despite different names*

### Comparing `django-reportbroD-4.0/django_reportbroD/static/assets/fonts/dripiconsd41d.eot` & `django_reportbrod-4.1/django_reportbroD/static/assets/fonts/dripiconsd41d.eot`

 * *Files identical despite different names*

### Comparing `django-reportbroD-4.0/django_reportbroD/static/assets/fonts/feather.eot` & `django_reportbrod-4.1/django_reportbroD/static/assets/fonts/feather.eot`

 * *Files identical despite different names*

### Comparing `django-reportbroD-4.0/django_reportbroD/static/assets/fonts/feather.svg` & `django_reportbrod-4.1/django_reportbroD/static/assets/fonts/feather.svg`

 * *Files identical despite different names*

### Comparing `django-reportbroD-4.0/django_reportbroD/static/assets/fonts/feather.ttf` & `django_reportbrod-4.1/django_reportbroD/static/assets/fonts/feather.ttf`

 * *Files identical despite different names*

### Comparing `django-reportbroD-4.0/django_reportbroD/static/assets/fonts/feather.woff` & `django_reportbrod-4.1/django_reportbroD/static/assets/fonts/feather.woff`

 * *Files identical despite different names*

### Comparing `django-reportbroD-4.0/django_reportbroD/static/assets/fonts/featherd41d.eot` & `django_reportbrod-4.1/django_reportbroD/static/assets/fonts/featherd41d.eot`

 * *Files identical despite different names*

### Comparing `django-reportbroD-4.0/django_reportbroD/static/assets/fonts/font-awesome.eot` & `django_reportbrod-4.1/django_reportbroD/static/assets/fonts/font-awesome.eot`

 * *Files identical despite different names*

### Comparing `django-reportbroD-4.0/django_reportbroD/static/assets/fonts/font-awesome.html` & `django_reportbrod-4.1/django_reportbroD/static/assets/fonts/font-awesome.html`

 * *Files identical despite different names*

### Comparing `django-reportbroD-4.0/django_reportbroD/static/assets/fonts/font-awesome.svg` & `django_reportbrod-4.1/django_reportbroD/static/assets/fonts/font-awesome.svg`

 * *Files identical despite different names*

### Comparing `django-reportbroD-4.0/django_reportbroD/static/assets/fonts/font-awesome.ttf` & `django_reportbrod-4.1/django_reportbroD/static/assets/fonts/font-awesome.ttf`

 * *Files identical despite different names*

### Comparing `django-reportbroD-4.0/django_reportbroD/static/assets/fonts/font-awesome.woff` & `django_reportbrod-4.1/django_reportbroD/static/assets/fonts/font-awesome.woff`

 * *Files identical despite different names*

### Comparing `django-reportbroD-4.0/django_reportbroD/static/assets/fonts/font-awesomed41d.eot` & `django_reportbrod-4.1/django_reportbroD/static/assets/fonts/font-awesomed41d.eot`

 * *Files identical despite different names*

### Comparing `django-reportbroD-4.0/django_reportbroD/static/assets/fonts/ionicons.eot` & `django_reportbrod-4.1/django_reportbroD/static/assets/fonts/ionicons.eot`

 * *Files identical despite different names*

### Comparing `django-reportbroD-4.0/django_reportbroD/static/assets/fonts/ionicons.html` & `django_reportbrod-4.1/django_reportbroD/static/assets/fonts/ionicons.html`

 * *Files identical despite different names*

### Comparing `django-reportbroD-4.0/django_reportbroD/static/assets/fonts/ionicons.svg` & `django_reportbrod-4.1/django_reportbroD/static/assets/fonts/ionicons.svg`

 * *Files identical despite different names*

### Comparing `django-reportbroD-4.0/django_reportbroD/static/assets/fonts/ionicons.ttf` & `django_reportbrod-4.1/django_reportbroD/static/assets/fonts/ionicons.ttf`

 * *Files identical despite different names*

### Comparing `django-reportbroD-4.0/django_reportbroD/static/assets/fonts/ionicons.woff` & `django_reportbrod-4.1/django_reportbroD/static/assets/fonts/ionicons.woff`

 * *Files identical despite different names*

### Comparing `django-reportbroD-4.0/django_reportbroD/static/assets/fonts/ioniconsd41d.eot` & `django_reportbrod-4.1/django_reportbroD/static/assets/fonts/ioniconsd41d.eot`

 * *Files identical despite different names*

### Comparing `django-reportbroD-4.0/django_reportbroD/static/assets/fonts/linea-weather.eot` & `django_reportbrod-4.1/django_reportbroD/static/assets/fonts/linea-weather.eot`

 * *Files identical despite different names*

### Comparing `django-reportbroD-4.0/django_reportbroD/static/assets/fonts/linea-weather.svg` & `django_reportbrod-4.1/django_reportbroD/static/assets/fonts/linea-weather.svg`

 * *Files identical despite different names*

### Comparing `django-reportbroD-4.0/django_reportbroD/static/assets/fonts/linea-weather.ttf` & `django_reportbrod-4.1/django_reportbroD/static/assets/fonts/linea-weather.ttf`

 * *Files identical despite different names*

### Comparing `django-reportbroD-4.0/django_reportbroD/static/assets/fonts/linea-weather.woff` & `django_reportbrod-4.1/django_reportbroD/static/assets/fonts/linea-weather.woff`

 * *Files identical despite different names*

### Comparing `django-reportbroD-4.0/django_reportbroD/static/assets/fonts/linea-weatherd41d.eot` & `django_reportbrod-4.1/django_reportbroD/static/assets/fonts/linea-weatherd41d.eot`

 * *Files identical despite different names*

### Comparing `django-reportbroD-4.0/django_reportbroD/static/assets/fonts/material-icons.eot` & `django_reportbrod-4.1/django_reportbroD/static/assets/fonts/material-icons.eot`

 * *Files identical despite different names*

### Comparing `django-reportbroD-4.0/django_reportbroD/static/assets/fonts/material-icons.html` & `django_reportbrod-4.1/django_reportbroD/static/assets/fonts/material-icons.html`

 * *Files identical despite different names*

### Comparing `django-reportbroD-4.0/django_reportbroD/static/assets/fonts/material-icons.svg` & `django_reportbrod-4.1/django_reportbroD/static/assets/fonts/material-icons.svg`

 * *Files identical despite different names*

### Comparing `django-reportbroD-4.0/django_reportbroD/static/assets/fonts/material-icons.ttf` & `django_reportbrod-4.1/django_reportbroD/static/assets/fonts/material-icons.ttf`

 * *Files identical despite different names*

### Comparing `django-reportbroD-4.0/django_reportbroD/static/assets/fonts/material-icons.woff` & `django_reportbrod-4.1/django_reportbroD/static/assets/fonts/material-icons.woff`

 * *Files identical despite different names*

### Comparing `django-reportbroD-4.0/django_reportbroD/static/assets/fonts/material-iconsd41d.eot` & `django_reportbrod-4.1/django_reportbroD/static/assets/fonts/material-iconsd41d.eot`

 * *Files identical despite different names*

### Comparing `django-reportbroD-4.0/django_reportbroD/static/assets/fonts/summernotec360.eot` & `django_reportbrod-4.1/django_reportbroD/static/assets/fonts/summernotec360.eot`

 * *Files identical despite different names*

### Comparing `django-reportbroD-4.0/django_reportbroD/static/assets/fonts/summernotec360.ttf` & `django_reportbrod-4.1/django_reportbroD/static/assets/fonts/summernotec360.ttf`

 * *Files identical despite different names*

### Comparing `django-reportbroD-4.0/django_reportbroD/static/assets/fonts/summernotec360.woff` & `django_reportbrod-4.1/django_reportbroD/static/assets/fonts/summernotec360.woff`

 * *Files identical despite different names*

### Comparing `django-reportbroD-4.0/django_reportbroD/static/assets/fonts/themify-icons.eot` & `django_reportbrod-4.1/django_reportbroD/static/assets/fonts/themify-icons.eot`

 * *Files identical despite different names*

### Comparing `django-reportbroD-4.0/django_reportbroD/static/assets/fonts/themify-icons.svg` & `django_reportbrod-4.1/django_reportbroD/static/assets/fonts/themify-icons.svg`

 * *Files identical despite different names*

### Comparing `django-reportbroD-4.0/django_reportbroD/static/assets/fonts/themify-icons.ttf` & `django_reportbrod-4.1/django_reportbroD/static/assets/fonts/themify-icons.ttf`

 * *Files identical despite different names*

### Comparing `django-reportbroD-4.0/django_reportbroD/static/assets/fonts/themify-icons.woff` & `django_reportbrod-4.1/django_reportbroD/static/assets/fonts/themify-icons.woff`

 * *Files identical despite different names*

### Comparing `django-reportbroD-4.0/django_reportbroD/static/assets/fonts/themify-iconsd41d.eot` & `django_reportbrod-4.1/django_reportbroD/static/assets/fonts/themify-iconsd41d.eot`

 * *Files identical despite different names*

### Comparing `django-reportbroD-4.0/django_reportbroD/static/assets/img/02.jpg` & `django_reportbrod-4.1/django_reportbroD/static/assets/img/02.jpg`

 * *Files identical despite different names*

### Comparing `django-reportbroD-4.0/django_reportbroD/static/assets/img/eeuu.png` & `django_reportbrod-4.1/django_reportbroD/static/assets/img/eeuu.png`

 * *Files identical despite different names*

### Comparing `django-reportbroD-4.0/django_reportbroD/static/assets/img/export/csv.svg` & `django_reportbrod-4.1/django_reportbroD/static/assets/img/export/csv.svg`

 * *Files identical despite different names*

### Comparing `django-reportbroD-4.0/django_reportbroD/static/assets/img/export/txt.svg` & `django_reportbrod-4.1/django_reportbroD/static/assets/img/export/txt.svg`

 * *Files identical despite different names*

### Comparing `django-reportbroD-4.0/django_reportbroD/static/assets/img/export/xlsx.svg` & `django_reportbrod-4.1/django_reportbroD/static/assets/img/export/xlsx.svg`

 * *Files identical despite different names*

### Comparing `django-reportbroD-4.0/django_reportbroD/static/assets/img/favicon.ico` & `django_reportbrod-4.1/django_reportbroD/static/assets/img/favicon.ico`

 * *Files identical despite different names*

### Comparing `django-reportbroD-4.0/django_reportbroD/static/assets/img/file-icon/ai.png` & `django_reportbrod-4.1/django_reportbroD/static/assets/img/file-icon/ai.png`

 * *Files identical despite different names*

### Comparing `django-reportbroD-4.0/django_reportbroD/static/assets/img/file-icon/css.png` & `django_reportbrod-4.1/django_reportbroD/static/assets/img/file-icon/css.png`

 * *Files identical despite different names*

### Comparing `django-reportbroD-4.0/django_reportbroD/static/assets/img/file-icon/dbf.png` & `django_reportbrod-4.1/django_reportbroD/static/assets/img/file-icon/dbf.png`

 * *Files identical despite different names*

### Comparing `django-reportbroD-4.0/django_reportbroD/static/assets/img/file-icon/doc.png` & `django_reportbrod-4.1/django_reportbroD/static/assets/img/file-icon/doc.png`

 * *Files identical despite different names*

### Comparing `django-reportbroD-4.0/django_reportbroD/static/assets/img/file-icon/dwg.png` & `django_reportbrod-4.1/django_reportbroD/static/assets/img/file-icon/dwg.png`

 * *Files identical despite different names*

### Comparing `django-reportbroD-4.0/django_reportbroD/static/assets/img/file-icon/exe.png` & `django_reportbrod-4.1/django_reportbroD/static/assets/img/file-icon/exe.png`

 * *Files identical despite different names*

### Comparing `django-reportbroD-4.0/django_reportbroD/static/assets/img/file-icon/html.png` & `django_reportbrod-4.1/django_reportbroD/static/assets/img/file-icon/html.png`

 * *Files identical despite different names*

### Comparing `django-reportbroD-4.0/django_reportbroD/static/assets/img/file-icon/jpg.png` & `django_reportbrod-4.1/django_reportbroD/static/assets/img/file-icon/jpg.png`

 * *Files identical despite different names*

### Comparing `django-reportbroD-4.0/django_reportbroD/static/assets/img/file-icon/pdf.png` & `django_reportbrod-4.1/django_reportbroD/static/assets/img/file-icon/pdf.png`

 * *Files identical despite different names*

### Comparing `django-reportbroD-4.0/django_reportbroD/static/assets/img/file-icon/png.png` & `django_reportbrod-4.1/django_reportbroD/static/assets/img/file-icon/png.png`

 * *Files identical despite different names*

### Comparing `django-reportbroD-4.0/django_reportbroD/static/assets/img/file-icon/psd.png` & `django_reportbrod-4.1/django_reportbroD/static/assets/img/file-icon/psd.png`

 * *Files identical despite different names*

### Comparing `django-reportbroD-4.0/django_reportbroD/static/assets/img/file-icon/reporte.png` & `django_reportbrod-4.1/django_reportbroD/static/assets/img/file-icon/reporte.png`

 * *Files identical despite different names*

### Comparing `django-reportbroD-4.0/django_reportbroD/static/assets/img/file-icon/rtf.png` & `django_reportbrod-4.1/django_reportbroD/static/assets/img/file-icon/rtf.png`

 * *Files identical despite different names*

### Comparing `django-reportbroD-4.0/django_reportbroD/static/assets/img/file-icon/svg.png` & `django_reportbrod-4.1/django_reportbroD/static/assets/img/file-icon/svg.png`

 * *Files identical despite different names*

### Comparing `django-reportbroD-4.0/django_reportbroD/static/assets/img/file-icon/xls.png` & `django_reportbrod-4.1/django_reportbroD/static/assets/img/file-icon/xls.png`

 * *Files identical despite different names*

### Comparing `django-reportbroD-4.0/django_reportbroD/static/assets/img/file-icon/xml.png` & `django_reportbrod-4.1/django_reportbroD/static/assets/img/file-icon/xml.png`

 * *Files identical despite different names*

### Comparing `django-reportbroD-4.0/django_reportbroD/static/assets/img/file-icon/zip.png` & `django_reportbrod-4.1/django_reportbroD/static/assets/img/file-icon/zip.png`

 * *Files identical despite different names*

### Comparing `django-reportbroD-4.0/django_reportbroD/static/assets/img/lista.png` & `django_reportbrod-4.1/django_reportbroD/static/assets/img/lista.png`

 * *Files identical despite different names*

### Comparing `django-reportbroD-4.0/django_reportbroD/static/assets/img/logo-icon.png` & `django_reportbrod-4.1/django_reportbroD/static/assets/img/logo-icon.png`

 * *Files identical despite different names*

### Comparing `django-reportbroD-4.0/django_reportbroD/static/assets/img/logo-light.png` & `django_reportbrod-4.1/django_reportbroD/static/assets/img/logo-light.png`

 * *Files identical despite different names*

### Comparing `django-reportbroD-4.0/django_reportbroD/static/assets/img/logo.png` & `django_reportbrod-4.1/django_reportbroD/static/assets/img/logo.png`

 * *Files identical despite different names*

### Comparing `django-reportbroD-4.0/django_reportbroD/static/assets/img/spain.png` & `django_reportbrod-4.1/django_reportbroD/static/assets/img/spain.png`

 * *Files identical despite different names*

### Comparing `django-reportbroD-4.0/django_reportbroD/static/assets/js/app.js` & `django_reportbrod-4.1/django_reportbroD/static/assets/js/app.js`

 * *Files identical despite different names*

### Comparing `django-reportbroD-4.0/django_reportbroD/static/assets/js/vendors.js` & `django_reportbrod-4.1/django_reportbroD/static/assets/js/vendors.js`

 * *Files identical despite different names*

### Comparing `django-reportbroD-4.0/django_reportbroD/static/reportlib/css/iconfonts/fonts/demoapp.svg` & `django_reportbrod-4.1/django_reportbroD/static/reportlib/css/iconfonts/fonts/demoapp.svg`

 * *Files identical despite different names*

### Comparing `django-reportbroD-4.0/django_reportbroD/static/reportlib/css/iconfonts/fonts/demoapp.ttf` & `django_reportbrod-4.1/django_reportbroD/static/reportlib/css/iconfonts/fonts/demoapp.ttf`

 * *Files identical despite different names*

### Comparing `django-reportbroD-4.0/django_reportbroD/static/reportlib/css/iconfonts/fonts/demoapp.woff` & `django_reportbrod-4.1/django_reportbroD/static/reportlib/css/iconfonts/fonts/demoapp.woff`

 * *Files identical despite different names*

### Comparing `django-reportbroD-4.0/django_reportbroD/static/reportlib/css/iconfonts/fonts/demoapp.woff2` & `django_reportbrod-4.1/django_reportbroD/static/reportlib/css/iconfonts/fonts/demoapp.woff2`

 * *Files identical despite different names*

### Comparing `django-reportbroD-4.0/django_reportbroD/static/reportlib/css/iconfonts/style.css` & `django_reportbrod-4.1/django_reportbroD/static/reportlib/css/iconfonts/style.css`

 * *Files identical despite different names*

### Comparing `django-reportbroD-4.0/django_reportbroD/static/reportlib/css/styles.css` & `django_reportbrod-4.1/django_reportbroD/static/reportlib/css/styles.css`

 * *Files identical despite different names*

### Comparing `django-reportbroD-4.0/django_reportbroD/static/reportlib/favicon.ico` & `django_reportbrod-4.1/django_reportbroD/static/reportlib/favicon.ico`

 * *Files identical despite different names*

### Comparing `django-reportbroD-4.0/django_reportbroD/static/reportlib/js/jquery-3.6.0.js` & `django_reportbrod-4.1/django_reportbroD/static/reportlib/js/jquery-3.6.0.js`

 * *Files identical despite different names*

### Comparing `django-reportbroD-4.0/django_reportbroD/static/reportlib/js/jquery-3.6.0.min.js` & `django_reportbrod-4.1/django_reportbroD/static/reportlib/js/jquery-3.6.0.min.js`

 * *Files identical despite different names*

### Comparing `django-reportbroD-4.0/django_reportbroD/static/reportlib/js/jquery.cookie.js` & `django_reportbrod-4.1/django_reportbroD/static/reportlib/js/jquery.cookie.js`

 * *Files identical despite different names*

### Comparing `django-reportbroD-4.0/django_reportbroD/static/reportlib/reportbro.css` & `django_reportbrod-4.1/django_reportbroD/static/reportlib/reportbro.css`

 * *Files identical despite different names*

### Comparing `django-reportbroD-4.0/django_reportbroD/static/reportlib/reportbro.css.map` & `django_reportbrod-4.1/django_reportbroD/static/reportlib/reportbro.css.map`

 * *Files identical despite different names*

### Comparing `django-reportbroD-4.0/django_reportbroD/static/reportlib/reportbro.js` & `django_reportbrod-4.1/django_reportbroD/static/reportlib/reportbro.js`

 * *Files identical despite different names*

### Comparing `django-reportbroD-4.0/django_reportbroD/static/reportlib/reportbro.js.LICENSE.txt` & `django_reportbrod-4.1/django_reportbroD/static/reportlib/reportbro.js.LICENSE.txt`

 * *Files identical despite different names*

### Comparing `django-reportbroD-4.0/django_reportbroD/static/reportlib/reportbro.js.map` & `django_reportbrod-4.1/django_reportbroD/static/reportlib/reportbro.js.map`

 * *Files identical despite different names*

### Comparing `django-reportbroD-4.0/django_reportbroD/static/reportlib/reportbro.min.js` & `django_reportbrod-4.1/django_reportbroD/static/reportlib/reportbro.min.js`

 * *Files identical despite different names*

### Comparing `django-reportbroD-4.0/django_reportbroD/static/reportlib/reportbro.min.js.map` & `django_reportbrod-4.1/django_reportbroD/static/reportlib/reportbro.min.js.map`

 * *Files identical despite different names*

### Comparing `django-reportbroD-4.0/django_reportbroD/static/reportlib/src/ajaxload.gif` & `django_reportbrod-4.1/django_reportbroD/static/reportlib/src/ajaxload.gif`

 * *Files identical despite different names*

### Comparing `django-reportbroD-4.0/django_reportbroD/static/reportlib/src/fonts/open-sans-v34-latin-300.woff` & `django_reportbrod-4.1/django_reportbroD/static/reportlib/src/fonts/open-sans-v34-latin-300.woff`

 * *Files identical despite different names*

### Comparing `django-reportbroD-4.0/django_reportbroD/static/reportlib/src/fonts/open-sans-v34-latin-300.woff2` & `django_reportbrod-4.1/django_reportbroD/static/reportlib/src/fonts/open-sans-v34-latin-300.woff2`

 * *Files identical despite different names*

### Comparing `django-reportbroD-4.0/django_reportbroD/static/reportlib/src/fonts/open-sans-v34-latin-600.woff` & `django_reportbrod-4.1/django_reportbroD/static/reportlib/src/fonts/open-sans-v34-latin-600.woff`

 * *Files identical despite different names*

### Comparing `django-reportbroD-4.0/django_reportbroD/static/reportlib/src/fonts/open-sans-v34-latin-600.woff2` & `django_reportbrod-4.1/django_reportbroD/static/reportlib/src/fonts/open-sans-v34-latin-600.woff2`

 * *Files identical despite different names*

### Comparing `django-reportbroD-4.0/django_reportbroD/static/reportlib/src/fonts/open-sans-v34-latin-800.woff` & `django_reportbrod-4.1/django_reportbroD/static/reportlib/src/fonts/open-sans-v34-latin-800.woff`

 * *Files identical despite different names*

### Comparing `django-reportbroD-4.0/django_reportbroD/static/reportlib/src/fonts/open-sans-v34-latin-800.woff2` & `django_reportbrod-4.1/django_reportbroD/static/reportlib/src/fonts/open-sans-v34-latin-800.woff2`

 * *Files identical despite different names*

### Comparing `django-reportbroD-4.0/django_reportbroD/static/reportlib/src/fonts/open-sans-v34-latin-regular.woff` & `django_reportbrod-4.1/django_reportbroD/static/reportlib/src/fonts/open-sans-v34-latin-regular.woff`

 * *Files identical despite different names*

### Comparing `django-reportbroD-4.0/django_reportbroD/static/reportlib/src/fonts/open-sans-v34-latin-regular.woff2` & `django_reportbrod-4.1/django_reportbroD/static/reportlib/src/fonts/open-sans-v34-latin-regular.woff2`

 * *Files identical despite different names*

### Comparing `django-reportbroD-4.0/django_reportbroD/static/reportlib/src/iconfonts/reportbro.svg` & `django_reportbrod-4.1/django_reportbroD/static/reportlib/src/iconfonts/reportbro.svg`

 * *Files identical despite different names*

### Comparing `django-reportbroD-4.0/django_reportbroD/static/reportlib/src/iconfonts/reportbro.ttf` & `django_reportbrod-4.1/django_reportbroD/static/reportlib/src/iconfonts/reportbro.ttf`

 * *Files identical despite different names*

### Comparing `django-reportbroD-4.0/django_reportbroD/static/reportlib/src/iconfonts/reportbro.woff` & `django_reportbrod-4.1/django_reportbroD/static/reportlib/src/iconfonts/reportbro.woff`

 * *Files identical despite different names*

### Comparing `django-reportbroD-4.0/django_reportbroD/static/reportlib/src/iconfonts/reportbro.woff2` & `django_reportbrod-4.1/django_reportbroD/static/reportlib/src/iconfonts/reportbro.woff2`

 * *Files identical despite different names*

### Comparing `django-reportbroD-4.0/django_reportbroD/static/reportlib/src/rb_logo_dark.png` & `django_reportbrod-4.1/django_reportbroD/static/reportlib/src/rb_logo_dark.png`

 * *Files identical despite different names*

### Comparing `django-reportbroD-4.0/django_reportbroD/static/reportlib/src/rb_logo_white.png` & `django_reportbrod-4.1/django_reportbroD/static/reportlib/src/rb_logo_white.png`

 * *Files identical despite different names*

### Comparing `django-reportbroD-4.0/django_reportbroD/templates/bases/base.html` & `django_reportbrod-4.1/django_reportbroD/templates/bases/base.html`

 * *Files identical despite different names*

### Comparing `django-reportbroD-4.0/django_reportbroD/templates/bases/header.html` & `django_reportbrod-4.1/django_reportbroD/templates/bases/header.html`

 * *Files 4% similar despite different names*

```diff
@@ -36,15 +36,20 @@
                     
                 </ul>
 
                 <ul class="navbar-nav nav-right ml-auto menuhidden">
                     
                     {% for elem in menu %}
                     <li class="nav-item dropdown">
-                        <a class="nav-link " href="{{elem.url}}" id="navbarDropdown2" role="button"  aria-haspopup="true" aria-expanded="false" title="{{elem.label}}">
+                        <a class="nav-link " href="{{elem.url}}" id="navbarDropdown2" role="button"  aria-haspopup="true" aria-expanded="false" title="{{elem.label}}"
+                        {% if elem.target %}
+                        target="__blank"
+                            
+                        {% endif %}
+                        >
                             <i class="{{elem.icon}}"></i>
 
                             {% if active_page == elem.id %}
                         <span class="notify">
                             <span class="blink"></span>
                 <span class="dot"></span>
                 </span>
@@ -55,16 +60,20 @@
 
 
                     {% endfor %}
                 </ul>
              
 
                 
+{% url 'set_language' as language_url %}
+{% if language_url %}
                 <ul class="navbar-nav nav-right ml-auto ">
-        
+                   
+                  
+
 <form  action="{% url 'set_language' %}" method="post" style="display: inline;">
     {% csrf_token %}
     <input name="next" type="hidden" value="{{ redirect_to }}">
   
     {% get_current_language as LANGUAGE_CODE %}
    
     {% if LANGUAGE_CODE == 'es' %}
@@ -87,15 +96,18 @@
         
                 {{ language.name_local |lower|capfirst}} ({{ language.code }})
             </option>
         {% endfor %}
     </select>
     
 </form>
+
+
 </ul>
-        
+{% endif %} 
+
         </div>
         <!-- end navigation -->
     </nav>
     <!-- end navbar -->
 </header>
```

#### html2text {}

```diff
@@ -1,11 +1,14 @@
 {% load static %} {% load i18n %}
 _[_l_o_g_o_]_[_l_o_g_o_]
     * _{_%_ _t_r_a_n_s_ _"_a_p_p_"_ _%_}
     * {% for elem in menu %}
-    * _{_%_ _i_f_ _a_c_t_i_v_e___p_a_g_e_ _=_=_ _e_l_e_m_._i_d_ _%_}_ _{_%_ _e_n_d_i_f_ _%_}
-    * {% endfor %}
+    * % if elem.target %} target="__blank" {% endif %} > {% if active_page ==
+      elem.id %} {% endif %}
+{% endfor %}
+{% url 'set_language' as language_url %} {% if language_url %}
       {% for language in reportbro_langs %}
       % if language.code == LANGUAGE_CODE %} selected {% endif %}> [{% static
       'assets/img/spain.png' %}]{{ language.name_local |lower|capfirst}} ({
       { language.code }})
       {% endfor %}
+{% endif %}
```

### Comparing `django-reportbroD-4.0/django_reportbroD/templates/bases/navigator.html` & `django_reportbrod-4.1/django_reportbroD/templates/bases/navigator.html`

 * *Files 13% similar despite different names*

```diff
@@ -11,15 +11,21 @@
     {% if active_page == elem.id %}
     class="active"
   
     {% endif %}
 
     >
 
-    <a class=" has-arrow "  href="{{elem.url}}" aria-expanded="false" >
+    <a class=" has-arrow "  href="{{elem.url}}" aria-expanded="false"  
+    
+    {% if elem.target %}
+    target="__blank"
+        
+    {% endif %}
+    >
 
     <i class="{{elem.icon}}"></i>
         <span class="nav-title">{{elem.label}}</span>
 
     </a>
 
 </li>
```

### Comparing `django-reportbroD-4.0/django_reportbroD/templates/create.html` & `django_reportbrod-4.1/django_reportbroD/templates/create.html`

 * *Files identical despite different names*

### Comparing `django-reportbroD-4.0/django_reportbroD/templates/document.html` & `django_reportbrod-4.1/django_reportbroD/templates/document.html`

 * *Files identical despite different names*

### Comparing `django-reportbroD-4.0/django_reportbroD/templates/edit.html` & `django_reportbrod-4.1/django_reportbroD/templates/edit.html`

 * *Files identical despite different names*

### Comparing `django-reportbroD-4.0/django_reportbroD/templates/especif.html` & `django_reportbrod-4.1/django_reportbroD/templates/especif.html`

 * *Files identical despite different names*

### Comparing `django-reportbroD-4.0/django_reportbroD/templates/formulario.html` & `django_reportbrod-4.1/django_reportbroD/templates/formulario.html`

 * *Files identical despite different names*

### Comparing `django-reportbroD-4.0/django_reportbroD/templates/import.html` & `django_reportbrod-4.1/django_reportbroD/templates/import.html`

 * *Files identical despite different names*

### Comparing `django-reportbroD-4.0/django_reportbroD/templates/index.html` & `django_reportbrod-4.1/django_reportbroD/templates/index.html`

 * *Files identical despite different names*

### Comparing `django-reportbroD-4.0/django_reportbroD/templates/report.html` & `django_reportbrod-4.1/django_reportbroD/templates/report.html`

 * *Files 4% similar despite different names*

```diff
@@ -80,26 +80,32 @@
                                             <i class="ti ti-align-right"></i>
                                         </a>
                                     </li>
                                     <li class="nav-item">
                                         <a class="nav-link "   role="button"  aria-haspopup="true" aria-expanded="false">
                                             
                                             <i class="fa fa-edit"></i> {{name}}
-                                          
+
                                         </a>
                                     </li>
                                     
                                     
                                 </ul>
                 
                                 <ul class="navbar-nav nav-right ml-auto">
                                     
                                     {% for elem in menu %}
                                     <li class="nav-item dropdown">
-                                        <a class="nav-link " href="{{elem.url}}" id="navbarDropdown2" role="button"  aria-haspopup="true" aria-expanded="false" title="{{elem.label}}">
+                                        <a class="nav-link " href="{{elem.url}}" id="navbarDropdown2" role="button"  aria-haspopup="true" aria-expanded="false" title="{{elem.label}}"
+                                        
+                                        {% if elem.target %}
+                                        target="__blank"
+                                            
+                                        {% endif %}
+                                        >
                                             <i class="{{elem.icon}}"></i>
                 
                                             {% if active_page == elem.id %}
                                         <span class="notify">
                                             <span class="blink"></span>
                                 <span class="dot"></span>
                                 </span>
```

#### html2text {}

```diff
@@ -1,5 +1,6 @@
 {% load static %} {% load i18n %}
     * {{name}}
     * {% for elem in menu %}
-    * _{_%_ _i_f_ _a_c_t_i_v_e___p_a_g_e_ _=_=_ _e_l_e_m_._i_d_ _%_}_ _{_%_ _e_n_d_i_f_ _%_}
-    * {% endfor %}
+    * % if elem.target %} target="__blank" {% endif %} > {% if active_page ==
+      elem.id %} {% endif %}
+{% endfor %}
```

### Comparing `django-reportbroD-4.0/django_reportbroD/urls.py` & `django_reportbrod-4.1/django_reportbroD/urls.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,21 +1,19 @@
-from django.urls import path, include
+from django.urls import include, path
+
+from .reportcore import *
 from .views import *
-from  .reportcore import *
 
-app_name="reportbroD"
+app_name = "reportbroD"
 urlpatterns = [
- 
     path("", ReportList.as_view(), name="list"),
     path("create/", CreateReport.as_view(), name="create"),
-     path("import/", importreport, name="import"),
- path("edit/<int:pk>", EditReport.as_view(), name="edit"),
+    path("import/", importreport, name="import"),
+    path("edit/<int:pk>", EditReport.as_view(), name="edit"),
     path("delete/<int:id>", deletereport, name="delete"),
-     path("duplicate/<int:id>", duplicatereport, name="duplicate"),
-     path("export/<int:id>", exportreport, name="exportation"),
+    path("duplicate/<int:id>", duplicatereport, name="duplicate"),
+    path("export/<int:id>", exportreport, name="exportation"),
     path("docs/", docs_view, name="docs"),
     path("template/<int:pk>/", edit, name="template"),
     path("run/", run, name="report_run"),
     path("save/<int:pk>/", save, name="report_save"),
-
-
-] 
+]
```

### Comparing `django-reportbroD-4.0/django_reportbroD/utils.py` & `django_reportbrod-4.1/django_reportbroD/utils.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,17 +1,16 @@
-
 import json
-from .models import ReportDefinition
-from django.db import models
 from itertools import chain
+
+from django.db import models
 from django.http import HttpResponseServerError
-from .reportcore import reportPDF, reportXLSX
 from PIL import Image, ImageDraw, ImageOps
 
-
+from .models import ReportDefinition
+from .reportcore import reportPDF, reportXLSX
 
 
 def to_dict(instance):
     """Esta función permite convertir un objeto de tipo Model a un diccionario
     para que su información pueda ser pasada como parámetro a ReportBro"""
     opts = instance._meta
     data = {}
@@ -19,99 +18,101 @@
         if isinstance(f, models.DateTimeField):
             if f.value_from_object(instance) is not None:
                 data[f.name] = f.value_from_object(instance).isoformat()
             else:
                 data[f.name] = None
         elif isinstance(f, models.ImageField):
             if f.value_from_object(instance) is not None:
-                formato= f.value_from_object(instance).url.split(".")[-1]
-                data[f.name] = convert_to_base64(f.value_from_object(instance).url, formato)
+                formato = f.value_from_object(instance).url.split(".")[-1]
+                data[f.name] = convert_to_base64(
+                    f.value_from_object(instance).url, formato
+                )
             else:
                 data[f.name] = None
         else:
             data[f.name] = f.value_from_object(instance)
     return data
 
 
 def convert_list_to_dict(listado):
-    """Convierte una query o lista de elementos de la clase Model en un 
+    """Convierte una query o lista de elementos de la clase Model en un
     diccionario entendible para ReportBro"""
 
-    lista=[to_dict(elem) for elem in listado ]
+    lista = [to_dict(elem) for elem in listado]
     return lista
 
 
 def convert_to_base64(path, format_image):
     """
     Nota: path se refiere a la ruta de la imagen y  format_image se refiere al fomato de la imagen (jpg, png, jpeg, etc)
-    Este método permite convertir una imagen jpg o png a una imagen en base 64 
-      para que ReportBro pueda renderizarla como parte de sus parámetros  """
+    Este método permite convertir una imagen jpg o png a una imagen en base 64
+      para que ReportBro pueda renderizarla como parte de sus parámetros"""
     import base64
+
     from django.conf import settings
-    
-    with open(str(settings.BASE_DIR)+path, "rb") as image_file:
+
+    with open(str(settings.BASE_DIR) + path, "rb") as image_file:
         return f"data:image/{format_image};base64,{base64.b64encode(image_file.read()).decode('utf-8')}"
-    
 
 
-def export_report_by_code(template_code, data, extension="pdf", file="reporte", download=False):
-    """ Export a report using its code
+def export_report_by_code(
+    template_code, data, extension="pdf", file="reporte", download=False
+):
+    """Export a report using its code
     view_mode: Its the way in the report pdf is going to download through the navegator. Two options:
     1. download =False, (inline) >the pdf report is showed in the navegator and the user can download it handly or making print, etc.
     2. download =True (attachment) >the pdf report is downloaded directly into pc
-    
+
     """
-    
+
     report = ReportDefinition.objects.filter(pk=template_code).first()
-    
+
     if not report:
-        return HttpResponseServerError('Este reporte no se encuentra disponible')
-    
+        return HttpResponseServerError("Este reporte no se encuentra disponible")
 
-    if extension.lower() =="xlsx":
-        return reportXLSX( report.report_definition, data, file)
-    
-    return reportPDF( report.report_definition, data, file, download)
+    if extension.lower() == "xlsx":
+        return reportXLSX(report.report_definition, data, file)
 
+    return reportPDF(report.report_definition, data, file, download)
 
 
-def export_report_by_name(template_name, data, extension="pdf", file="reporte", download=False):
-    """ Export a report using its name
+def export_report_by_name(
+    template_name, data, extension="pdf", file="reporte", download=False
+):
+    """Export a report using its name
     view_mode: Its the way in the report pdf is going to download through the navegator. Two options:
     1. download =False, (inline) >the pdf report is showed in the navegator and the user can download it handly or making print, etc.
     2. download =True (attachment) >the pdf report is downloaded directly into pc
     """
 
     report = ReportDefinition.objects.filter(name=template_name).first()
-    
-    if not report:
-        return HttpResponseServerError('Este reporte no se encuentra disponible')
 
+    if not report:
+        return HttpResponseServerError("Este reporte no se encuentra disponible")
 
-    if extension.lower() =="xlsx":
+    if extension.lower() == "xlsx":
         return reportXLSX(report.report_definition, data, file)
-    
-    return reportPDF(report.report_definition, data, file, download)
 
+    return reportPDF(report.report_definition, data, file, download)
 
 
-def export_report_from_JSON(path_json, data, extension="pdf", file="reporte", download=False):
-    """ Export a report using a JSON template report.
+def export_report_from_JSON(
+    path_json, data, extension="pdf", file="reporte", download=False
+):
+    """Export a report using a JSON template report.
     view_mode: Its the way in the report pdf is going to download through the navegator. Two options:
     1. download =False, (inline) >the pdf report is showed in the navegator and the user can download it handly or making print, etc.
     2. download =True (attachment) >the pdf report is downloaded directly into pc
     """
-    
+
     try:
         with open(path_json) as json_file:
             report = json.load(json_file)
-    except FileNotFoundError :
-        return HttpResponseServerError('La ruta especificada no contiene la plantilla.')
+    except FileNotFoundError:
+        return HttpResponseServerError("La ruta especificada no contiene la plantilla.")
     except json.JSONDecodeError:
-        return HttpResponseServerError('El fichero no tiene un formato adecuado.')
-        
+        return HttpResponseServerError("El fichero no tiene un formato adecuado.")
 
-    if extension.lower() =="xlsx":
-        return reportXLSX(report["report_definition"], data, file )
-    
-    return reportPDF(report["report_definition"], data, file, download)
+    if extension.lower() == "xlsx":
+        return reportXLSX(report["report_definition"], data, file)
 
+    return reportPDF(report["report_definition"], data, file, download)
```

### Comparing `django-reportbroD-4.0/django_reportbroD.egg-info/PKG-INFO` & `django_reportbrod-4.1/django_reportbroD.egg-info/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: django-reportbroD
-Version: 4.0
+Version: 4.1
 Summary: A Django app to create and use ReportBro reports with a sample admin. This allows you to generate yours reports using three options: by its code or name from database or JSON template.
 Author: Rider Raul Espinosa Perez
 Author-email: riderraule@gmail.com
 License: MIT
 Classifier: Environment :: Web Environment
 Classifier: Framework :: Django
 Classifier: Framework :: Django :: 5.0
@@ -17,68 +17,69 @@
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: Python :: 3.12
 Classifier: Topic :: Internet :: WWW/HTTP
 Classifier: Topic :: Internet :: WWW/HTTP :: Dynamic Content
 Requires-Python: >=3.8
 Description-Content-Type: text/markdown
+Requires-Dist: Django>=4.2
+Requires-Dist: reportbro-lib>=3.7.0
 
 # django-reportbroD
 A Django app to create, use and export ReportBro reports (free version) with a admin. 
 
 ![Django](https://img.shields.io/badge/django-%23092E20.svg?style=for-the-badge&logo=django&logoColor=white) ![lib](https://badgen.net/badge/Export/PDF-XLSX/red?) ![JS](https://badgen.net/badge/Js/Reportbro_Designer/blue?icon=doc)  ![lib](https://badgen.net/badge/Package/Reportbro-lib/red?icon=doc)
 
 Quick start
 -----------
 
 1. Add "django_reportbroD" to your INSTALLED_APPS setting like this:
 ```
-    INSTALLED_APPS = [
-   
-                ... ,
-   'django_reportbroD.apps.ReportbrodConfig',
-
+INSTALLED_APPS = [
+... ,
+'django_reportbroD.apps.ReportbrodConfig',
    ]
 
 ```
-2. Add LocaleMiddleware to your MIDDLEWARE list in your settings. This allows the reporting app to have translation in Spanish and English. 
+
+2. Include the reportbroD URLconf in your project urls.py like this:
+
+```
+   path("reportbroD/", include("django_reportbroD.urls", namespace="reportbroD")),  
+```
+
+
+3.  Run ``python manage.py migrate`` to create the models and to migrating to data base.
+
+4. Start the development server.
+
+5. Visit the ``/reportbroD/`` URL to create/update/edit/duplicate/remove reports.
+
+
+
+
+> **Traslations** 
+>
+>The next step is optional if you want to use in Spanish and English, otherwise it isn't necessary.
+
+1. Add LocaleMiddleware to your MIDDLEWARE list in your settings. This allows the reporting app to have translation in Spanish and English. 
  ```
         MIDDLEWARE = [
     'django.middleware.locale.LocaleMiddleware',
     ...
-            ],
-            
-        
+            ],  
 ```
 
-3. Add 'django_reportbroD.menus.get_menu_items' to your OPTIONS.context_processors in your TEMPLATES settings. This enables the use of menu for the installed report app. 
- ```
-        'OPTIONS': {
-   
-            'context_processors': [...,
-'django_reportbroD.menus.get_menu_items'
-   
-            ],
-            
-        }
-```
-
-4. Include the reportbroD URLconf in your project urls.py and the i18n urls like this:
+1. Include the i18N URLconf in your project urls.py like this:
 
 ```
-   path("reportbroD/", include("django_reportbroD.urls" namespace="reportbroD")),  
-   path('i18n/', include('django.conf.urls.i18n')),
+   path("i18n/", include("django.conf.urls.i18n")),  
 ```
 
 
-5.  Run ``python manage.py migrate`` to create the models and to migrating to data base.
-
-6. Start the development server.
-
-7. Visit the ``/reportbroD/`` URL to create/update/edit/duplicate/remove reports.
 
 
 Using report
 -----------
 
 1. Create a app to using the view file or other file .py for defining the view function to show/export selected report
  ```
```

### Comparing `django-reportbroD-4.0/django_reportbroD.egg-info/SOURCES.txt` & `django_reportbrod-4.1/django_reportbroD.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `django-reportbroD-4.0/setup.cfg` & `django_reportbrod-4.1/setup.cfg`

 * *Files 9% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [metadata]
 name = django-reportbroD
-version = 4.0
+version = 4.1
 description = A Django app to create and use ReportBro reports with a sample admin. This allows you to generate yours reports using three options: by its code or name from database or JSON template.
 long_description = file: README.md
 long_description_content_type = text/markdown
 author = Rider Raul Espinosa Perez
 author_email = riderraule@gmail.com
 license = MIT
 classifiers =
```

