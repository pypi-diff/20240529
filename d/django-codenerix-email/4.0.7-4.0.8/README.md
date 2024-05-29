# Comparing `tmp/django-codenerix-email-4.0.7.tar.gz` & `tmp/django-codenerix-email-4.0.8.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "django-codenerix-email-4.0.7.tar", last modified: Thu May 23 05:51:57 2024, max compression
+gzip compressed data, was "django-codenerix-email-4.0.8.tar", last modified: Wed May 29 05:46:30 2024, max compression
```

## Comparing `django-codenerix-email-4.0.7.tar` & `django-codenerix-email-4.0.8.tar`

### file list

```diff
@@ -1,89 +1,89 @@
-drwxrwxr-x   0 br0th3r   (1001) br0th3r   (1001)        0 2024-05-23 05:51:57.226019 django-codenerix-email-4.0.7/
--rw-r--r--   0 br0th3r   (1001) br0th3r   (1001)    11339 2024-03-27 07:06:52.000000 django-codenerix-email-4.0.7/LICENSE
--rw-r--r--   0 br0th3r   (1001) br0th3r   (1001)      247 2020-05-15 23:36:43.000000 django-codenerix-email-4.0.7/MANIFEST.in
--rw-rw-r--   0 br0th3r   (1001) br0th3r   (1001)     2543 2024-05-23 05:51:57.226019 django-codenerix-email-4.0.7/PKG-INFO
--rw-r--r--   0 br0th3r   (1001) br0th3r   (1001)     1344 2022-08-14 19:56:23.000000 django-codenerix-email-4.0.7/README.rst
-drwxrwxr-x   0 br0th3r   (1001) br0th3r   (1001)        0 2024-05-23 05:51:57.222019 django-codenerix-email-4.0.7/codenerix_email/
--rw-rw-r--   0 br0th3r   (1001) br0th3r   (1001)      148 2024-05-23 05:51:56.000000 django-codenerix-email-4.0.7/codenerix_email/__init__.py
--rw-r--r--   0 br0th3r   (1001) br0th3r   (1001)     1208 2022-08-14 19:56:23.000000 django-codenerix-email-4.0.7/codenerix_email/admin.py
--rw-r--r--   0 br0th3r   (1001) br0th3r   (1001)      149 2022-08-14 19:56:23.000000 django-codenerix-email-4.0.7/codenerix_email/apps.py
--rw-r--r--   0 br0th3r   (1001) br0th3r   (1001)     3706 2024-05-22 12:29:39.000000 django-codenerix-email-4.0.7/codenerix_email/forms.py
-drwxrwxr-x   0 br0th3r   (1001) br0th3r   (1001)        0 2024-05-23 05:51:57.222019 django-codenerix-email-4.0.7/codenerix_email/management/
--rw-r--r--   0 br0th3r   (1001) br0th3r   (1001)        0 2020-05-15 23:36:43.000000 django-codenerix-email-4.0.7/codenerix_email/management/__init__.py
-drwxrwxr-x   0 br0th3r   (1001) br0th3r   (1001)        0 2024-05-23 05:51:57.222019 django-codenerix-email-4.0.7/codenerix_email/management/__pycache__/
--rw-r--r--   0 br0th3r   (1001) br0th3r   (1001)      179 2023-10-27 11:25:38.000000 django-codenerix-email-4.0.7/codenerix_email/management/__pycache__/__init__.cpython-310.pyc
--rw-r--r--   0 br0th3r   (1001) br0th3r   (1001)      195 2024-02-26 06:56:17.000000 django-codenerix-email-4.0.7/codenerix_email/management/__pycache__/__init__.cpython-311.pyc
--rw-r--r--   0 br0th3r   (1001) br0th3r   (1001)      160 2020-05-15 23:36:43.000000 django-codenerix-email-4.0.7/codenerix_email/management/__pycache__/__init__.cpython-35.pyc
--rw-r--r--   0 br0th3r   (1001) br0th3r   (1001)      168 2022-08-14 19:56:23.000000 django-codenerix-email-4.0.7/codenerix_email/management/__pycache__/__init__.cpython-39.pyc
-drwxrwxr-x   0 br0th3r   (1001) br0th3r   (1001)        0 2024-05-23 05:51:57.222019 django-codenerix-email-4.0.7/codenerix_email/management/commands/
--rw-r--r--   0 br0th3r   (1001) br0th3r   (1001)        0 2020-05-15 23:36:43.000000 django-codenerix-email-4.0.7/codenerix_email/management/commands/__init__.py
--rw-r--r--   0 br0th3r   (1001) br0th3r   (1001)     6290 2024-04-09 05:53:51.000000 django-codenerix-email-4.0.7/codenerix_email/management/commands/send_emails.py
--rw-r--r--   0 br0th3r   (1001) br0th3r   (1001)     1655 2024-04-09 05:53:42.000000 django-codenerix-email-4.0.7/codenerix_email/management/commands/test_email.py
-drwxrwxr-x   0 br0th3r   (1001) br0th3r   (1001)        0 2024-05-23 05:51:57.222019 django-codenerix-email-4.0.7/codenerix_email/migrations/
--rw-r--r--   0 br0th3r   (1001) br0th3r   (1001)     3511 2020-05-15 23:36:43.000000 django-codenerix-email-4.0.7/codenerix_email/migrations/0001_initial.py
--rw-r--r--   0 br0th3r   (1001) br0th3r   (1001)     2369 2020-05-15 23:36:43.000000 django-codenerix-email-4.0.7/codenerix_email/migrations/0002_auto_20170502_1043.py
--rw-r--r--   0 br0th3r   (1001) br0th3r   (1001)      656 2020-05-15 23:36:43.000000 django-codenerix-email-4.0.7/codenerix_email/migrations/0003_auto_20170921_1206.py
--rw-r--r--   0 br0th3r   (1001) br0th3r   (1001)      486 2020-05-15 23:36:43.000000 django-codenerix-email-4.0.7/codenerix_email/migrations/0004_auto_20171108_1628.py
--rw-r--r--   0 br0th3r   (1001) br0th3r   (1001)      495 2020-05-15 23:36:43.000000 django-codenerix-email-4.0.7/codenerix_email/migrations/0005_emailmessage_retries.py
--rw-r--r--   0 br0th3r   (1001) br0th3r   (1001)      489 2020-05-15 23:36:43.000000 django-codenerix-email-4.0.7/codenerix_email/migrations/0006_emailmessage_error.py
--rw-r--r--   0 br0th3r   (1001) br0th3r   (1001)      602 2020-05-15 23:36:43.000000 django-codenerix-email-4.0.7/codenerix_email/migrations/0007_emailmessage_next_retry.py
--rw-r--r--   0 br0th3r   (1001) br0th3r   (1001)      731 2020-05-15 23:36:43.000000 django-codenerix-email-4.0.7/codenerix_email/migrations/0008_auto_20171201_0928.py
--rw-rw-r--   0 br0th3r   (1001) br0th3r   (1001)     1219 2024-05-22 11:42:23.000000 django-codenerix-email-4.0.7/codenerix_email/migrations/0009_emailmessage_opened_emailmessage_uuid.py
--rw-r--r--   0 br0th3r   (1001) br0th3r   (1001)        0 2020-05-15 23:36:43.000000 django-codenerix-email-4.0.7/codenerix_email/migrations/__init__.py
-drwxrwxr-x   0 br0th3r   (1001) br0th3r   (1001)        0 2024-05-23 05:51:57.226019 django-codenerix-email-4.0.7/codenerix_email/migrations/__pycache__/
--rw-r--r--   0 br0th3r   (1001) br0th3r   (1001)     2005 2023-01-29 13:03:07.000000 django-codenerix-email-4.0.7/codenerix_email/migrations/__pycache__/0001_initial.cpython-310.pyc
--rw-r--r--   0 br0th3r   (1001) br0th3r   (1001)     3682 2024-02-14 12:11:39.000000 django-codenerix-email-4.0.7/codenerix_email/migrations/__pycache__/0001_initial.cpython-311.pyc
--rw-r--r--   0 br0th3r   (1001) br0th3r   (1001)     2373 2020-05-15 23:36:43.000000 django-codenerix-email-4.0.7/codenerix_email/migrations/__pycache__/0001_initial.cpython-35.pyc
--rw-r--r--   0 br0th3r   (1001) br0th3r   (1001)     2020 2022-08-14 19:56:23.000000 django-codenerix-email-4.0.7/codenerix_email/migrations/__pycache__/0001_initial.cpython-39.pyc
--rw-r--r--   0 br0th3r   (1001) br0th3r   (1001)     1500 2023-01-29 13:03:07.000000 django-codenerix-email-4.0.7/codenerix_email/migrations/__pycache__/0002_auto_20170502_1043.cpython-310.pyc
--rw-r--r--   0 br0th3r   (1001) br0th3r   (1001)     2664 2024-02-14 12:11:39.000000 django-codenerix-email-4.0.7/codenerix_email/migrations/__pycache__/0002_auto_20170502_1043.cpython-311.pyc
--rw-r--r--   0 br0th3r   (1001) br0th3r   (1001)     1692 2020-05-15 23:36:43.000000 django-codenerix-email-4.0.7/codenerix_email/migrations/__pycache__/0002_auto_20170502_1043.cpython-35.pyc
--rw-r--r--   0 br0th3r   (1001) br0th3r   (1001)     1515 2022-08-14 19:56:23.000000 django-codenerix-email-4.0.7/codenerix_email/migrations/__pycache__/0002_auto_20170502_1043.cpython-39.pyc
--rw-r--r--   0 br0th3r   (1001) br0th3r   (1001)      694 2023-01-29 13:03:07.000000 django-codenerix-email-4.0.7/codenerix_email/migrations/__pycache__/0003_auto_20170921_1206.cpython-310.pyc
--rw-r--r--   0 br0th3r   (1001) br0th3r   (1001)      967 2024-02-14 12:11:39.000000 django-codenerix-email-4.0.7/codenerix_email/migrations/__pycache__/0003_auto_20170921_1206.cpython-311.pyc
--rw-r--r--   0 br0th3r   (1001) br0th3r   (1001)      782 2020-05-15 23:36:43.000000 django-codenerix-email-4.0.7/codenerix_email/migrations/__pycache__/0003_auto_20170921_1206.cpython-35.pyc
--rw-r--r--   0 br0th3r   (1001) br0th3r   (1001)      709 2022-08-14 19:56:23.000000 django-codenerix-email-4.0.7/codenerix_email/migrations/__pycache__/0003_auto_20170921_1206.cpython-39.pyc
--rw-r--r--   0 br0th3r   (1001) br0th3r   (1001)      676 2023-01-29 13:03:07.000000 django-codenerix-email-4.0.7/codenerix_email/migrations/__pycache__/0004_auto_20171108_1628.cpython-310.pyc
--rw-r--r--   0 br0th3r   (1001) br0th3r   (1001)      939 2024-02-14 12:11:39.000000 django-codenerix-email-4.0.7/codenerix_email/migrations/__pycache__/0004_auto_20171108_1628.cpython-311.pyc
--rw-r--r--   0 br0th3r   (1001) br0th3r   (1001)      713 2020-05-15 23:36:43.000000 django-codenerix-email-4.0.7/codenerix_email/migrations/__pycache__/0004_auto_20171108_1628.cpython-35.pyc
--rw-r--r--   0 br0th3r   (1001) br0th3r   (1001)      691 2022-08-14 19:56:23.000000 django-codenerix-email-4.0.7/codenerix_email/migrations/__pycache__/0004_auto_20171108_1628.cpython-39.pyc
--rw-r--r--   0 br0th3r   (1001) br0th3r   (1001)      691 2023-01-29 13:03:07.000000 django-codenerix-email-4.0.7/codenerix_email/migrations/__pycache__/0005_emailmessage_retries.cpython-310.pyc
--rw-r--r--   0 br0th3r   (1001) br0th3r   (1001)      954 2024-02-14 12:11:39.000000 django-codenerix-email-4.0.7/codenerix_email/migrations/__pycache__/0005_emailmessage_retries.cpython-311.pyc
--rw-r--r--   0 br0th3r   (1001) br0th3r   (1001)      728 2020-05-15 23:36:43.000000 django-codenerix-email-4.0.7/codenerix_email/migrations/__pycache__/0005_emailmessage_retries.cpython-35.pyc
--rw-r--r--   0 br0th3r   (1001) br0th3r   (1001)      706 2022-08-14 19:56:23.000000 django-codenerix-email-4.0.7/codenerix_email/migrations/__pycache__/0005_emailmessage_retries.cpython-39.pyc
--rw-r--r--   0 br0th3r   (1001) br0th3r   (1001)      675 2023-01-29 13:03:07.000000 django-codenerix-email-4.0.7/codenerix_email/migrations/__pycache__/0006_emailmessage_error.cpython-310.pyc
--rw-r--r--   0 br0th3r   (1001) br0th3r   (1001)      938 2024-02-14 12:11:39.000000 django-codenerix-email-4.0.7/codenerix_email/migrations/__pycache__/0006_emailmessage_error.cpython-311.pyc
--rw-r--r--   0 br0th3r   (1001) br0th3r   (1001)      712 2020-05-15 23:36:43.000000 django-codenerix-email-4.0.7/codenerix_email/migrations/__pycache__/0006_emailmessage_error.cpython-35.pyc
--rw-r--r--   0 br0th3r   (1001) br0th3r   (1001)      690 2022-08-14 19:56:23.000000 django-codenerix-email-4.0.7/codenerix_email/migrations/__pycache__/0006_emailmessage_error.cpython-39.pyc
--rw-r--r--   0 br0th3r   (1001) br0th3r   (1001)      802 2023-01-29 13:03:07.000000 django-codenerix-email-4.0.7/codenerix_email/migrations/__pycache__/0007_emailmessage_next_retry.cpython-310.pyc
--rw-r--r--   0 br0th3r   (1001) br0th3r   (1001)     1111 2024-02-14 12:11:39.000000 django-codenerix-email-4.0.7/codenerix_email/migrations/__pycache__/0007_emailmessage_next_retry.cpython-311.pyc
--rw-r--r--   0 br0th3r   (1001) br0th3r   (1001)      854 2020-05-15 23:36:43.000000 django-codenerix-email-4.0.7/codenerix_email/migrations/__pycache__/0007_emailmessage_next_retry.cpython-35.pyc
--rw-r--r--   0 br0th3r   (1001) br0th3r   (1001)      817 2022-08-14 19:56:23.000000 django-codenerix-email-4.0.7/codenerix_email/migrations/__pycache__/0007_emailmessage_next_retry.cpython-39.pyc
--rw-r--r--   0 br0th3r   (1001) br0th3r   (1001)      779 2023-01-29 13:03:07.000000 django-codenerix-email-4.0.7/codenerix_email/migrations/__pycache__/0008_auto_20171201_0928.cpython-310.pyc
--rw-r--r--   0 br0th3r   (1001) br0th3r   (1001)     1178 2024-02-14 12:11:39.000000 django-codenerix-email-4.0.7/codenerix_email/migrations/__pycache__/0008_auto_20171201_0928.cpython-311.pyc
--rw-r--r--   0 br0th3r   (1001) br0th3r   (1001)      839 2020-05-15 23:36:43.000000 django-codenerix-email-4.0.7/codenerix_email/migrations/__pycache__/0008_auto_20171201_0928.cpython-35.pyc
--rw-r--r--   0 br0th3r   (1001) br0th3r   (1001)      794 2022-08-14 19:56:23.000000 django-codenerix-email-4.0.7/codenerix_email/migrations/__pycache__/0008_auto_20171201_0928.cpython-39.pyc
--rw-rw-r--   0 br0th3r   (1001) br0th3r   (1001)      733 2024-05-21 07:57:54.000000 django-codenerix-email-4.0.7/codenerix_email/migrations/__pycache__/0009_delete_emailtemplatetexten.cpython-311.pyc
--rw-rw-r--   0 br0th3r   (1001) br0th3r   (1001)     1860 2024-05-22 11:44:13.000000 django-codenerix-email-4.0.7/codenerix_email/migrations/__pycache__/0009_emailmessage_opened_emailmessage_uuid.cpython-311.pyc
--rw-rw-r--   0 br0th3r   (1001) br0th3r   (1001)     3104 2024-05-22 11:40:40.000000 django-codenerix-email-4.0.7/codenerix_email/migrations/__pycache__/0010_emailmessage_opened_emailmessage_uuid_and_more.cpython-311.pyc
--rw-r--r--   0 br0th3r   (1001) br0th3r   (1001)      151 2023-01-29 13:03:07.000000 django-codenerix-email-4.0.7/codenerix_email/migrations/__pycache__/__init__.cpython-310.pyc
--rw-r--r--   0 br0th3r   (1001) br0th3r   (1001)      195 2024-02-14 12:11:39.000000 django-codenerix-email-4.0.7/codenerix_email/migrations/__pycache__/__init__.cpython-311.pyc
--rw-r--r--   0 br0th3r   (1001) br0th3r   (1001)      147 2020-05-15 23:36:43.000000 django-codenerix-email-4.0.7/codenerix_email/migrations/__pycache__/__init__.cpython-35.pyc
--rw-r--r--   0 br0th3r   (1001) br0th3r   (1001)      168 2022-08-14 19:56:23.000000 django-codenerix-email-4.0.7/codenerix_email/migrations/__pycache__/__init__.cpython-39.pyc
--rw-r--r--   0 br0th3r   (1001) br0th3r   (1001)    13280 2024-05-23 05:50:45.000000 django-codenerix-email-4.0.7/codenerix_email/models.py
-drwxrwxr-x   0 br0th3r   (1001) br0th3r   (1001)        0 2024-05-23 05:51:57.218019 django-codenerix-email-4.0.7/codenerix_email/static/
-drwxrwxr-x   0 br0th3r   (1001) br0th3r   (1001)        0 2024-05-23 05:51:57.218019 django-codenerix-email-4.0.7/codenerix_email/static/codenerix_email/
-drwxrwxr-x   0 br0th3r   (1001) br0th3r   (1001)        0 2024-05-23 05:51:57.226019 django-codenerix-email-4.0.7/codenerix_email/static/codenerix_email/partials/
--rw-r--r--   0 br0th3r   (1001) br0th3r   (1001)     1060 2024-05-22 11:47:17.000000 django-codenerix-email-4.0.7/codenerix_email/static/codenerix_email/partials/emailmessages_rows.html
--rw-r--r--   0 br0th3r   (1001) br0th3r   (1001)     2595 2022-08-14 19:56:23.000000 django-codenerix-email-4.0.7/codenerix_email/urls.py
--rw-r--r--   0 br0th3r   (1001) br0th3r   (1001)      873 2024-05-22 12:21:01.000000 django-codenerix-email-4.0.7/codenerix_email/urls_frontend.py
--rw-r--r--   0 br0th3r   (1001) br0th3r   (1001)     4736 2024-05-23 05:50:34.000000 django-codenerix-email-4.0.7/codenerix_email/views.py
-drwxrwxr-x   0 br0th3r   (1001) br0th3r   (1001)        0 2024-05-23 05:51:57.226019 django-codenerix-email-4.0.7/django_codenerix_email.egg-info/
--rw-r--r--   0 br0th3r   (1001) br0th3r   (1001)     2543 2024-05-23 05:51:57.000000 django-codenerix-email-4.0.7/django_codenerix_email.egg-info/PKG-INFO
--rw-r--r--   0 br0th3r   (1001) br0th3r   (1001)     4619 2024-05-23 05:51:57.000000 django-codenerix-email-4.0.7/django_codenerix_email.egg-info/SOURCES.txt
--rw-r--r--   0 br0th3r   (1001) br0th3r   (1001)        1 2024-05-23 05:51:57.000000 django-codenerix-email-4.0.7/django_codenerix_email.egg-info/dependency_links.txt
--rw-r--r--   0 br0th3r   (1001) br0th3r   (1001)        1 2020-05-15 23:36:43.000000 django-codenerix-email-4.0.7/django_codenerix_email.egg-info/not-zip-safe
--rw-r--r--   0 br0th3r   (1001) br0th3r   (1001)       53 2024-05-23 05:51:57.000000 django-codenerix-email-4.0.7/django_codenerix_email.egg-info/requires.txt
--rw-r--r--   0 br0th3r   (1001) br0th3r   (1001)       16 2024-05-23 05:51:57.000000 django-codenerix-email-4.0.7/django_codenerix_email.egg-info/top_level.txt
--rw-rw-r--   0 br0th3r   (1001) br0th3r   (1001)       38 2024-05-23 05:51:57.226019 django-codenerix-email-4.0.7/setup.cfg
--rw-r--r--   0 br0th3r   (1001) br0th3r   (1001)     1707 2024-04-08 11:04:22.000000 django-codenerix-email-4.0.7/setup.py
+drwxrwxr-x   0 br0th3r   (1001) br0th3r   (1001)        0 2024-05-29 05:46:30.960630 django-codenerix-email-4.0.8/
+-rw-r--r--   0 br0th3r   (1001) br0th3r   (1001)    11339 2024-03-27 07:06:52.000000 django-codenerix-email-4.0.8/LICENSE
+-rw-r--r--   0 br0th3r   (1001) br0th3r   (1001)      247 2020-05-15 23:36:43.000000 django-codenerix-email-4.0.8/MANIFEST.in
+-rw-rw-r--   0 br0th3r   (1001) br0th3r   (1001)     2543 2024-05-29 05:46:30.960630 django-codenerix-email-4.0.8/PKG-INFO
+-rw-r--r--   0 br0th3r   (1001) br0th3r   (1001)     1344 2022-08-14 19:56:23.000000 django-codenerix-email-4.0.8/README.rst
+drwxrwxr-x   0 br0th3r   (1001) br0th3r   (1001)        0 2024-05-29 05:46:30.948630 django-codenerix-email-4.0.8/codenerix_email/
+-rw-rw-r--   0 br0th3r   (1001) br0th3r   (1001)      148 2024-05-29 05:46:30.000000 django-codenerix-email-4.0.8/codenerix_email/__init__.py
+-rw-r--r--   0 br0th3r   (1001) br0th3r   (1001)     1208 2022-08-14 19:56:23.000000 django-codenerix-email-4.0.8/codenerix_email/admin.py
+-rw-r--r--   0 br0th3r   (1001) br0th3r   (1001)      149 2022-08-14 19:56:23.000000 django-codenerix-email-4.0.8/codenerix_email/apps.py
+-rw-r--r--   0 br0th3r   (1001) br0th3r   (1001)     3706 2024-05-27 06:59:45.000000 django-codenerix-email-4.0.8/codenerix_email/forms.py
+drwxrwxr-x   0 br0th3r   (1001) br0th3r   (1001)        0 2024-05-29 05:46:30.948630 django-codenerix-email-4.0.8/codenerix_email/management/
+-rw-r--r--   0 br0th3r   (1001) br0th3r   (1001)        0 2020-05-15 23:36:43.000000 django-codenerix-email-4.0.8/codenerix_email/management/__init__.py
+drwxrwxr-x   0 br0th3r   (1001) br0th3r   (1001)        0 2024-05-29 05:46:30.948630 django-codenerix-email-4.0.8/codenerix_email/management/__pycache__/
+-rw-r--r--   0 br0th3r   (1001) br0th3r   (1001)      179 2023-10-27 11:25:38.000000 django-codenerix-email-4.0.8/codenerix_email/management/__pycache__/__init__.cpython-310.pyc
+-rw-r--r--   0 br0th3r   (1001) br0th3r   (1001)      195 2024-02-26 06:56:17.000000 django-codenerix-email-4.0.8/codenerix_email/management/__pycache__/__init__.cpython-311.pyc
+-rw-r--r--   0 br0th3r   (1001) br0th3r   (1001)      160 2020-05-15 23:36:43.000000 django-codenerix-email-4.0.8/codenerix_email/management/__pycache__/__init__.cpython-35.pyc
+-rw-r--r--   0 br0th3r   (1001) br0th3r   (1001)      168 2022-08-14 19:56:23.000000 django-codenerix-email-4.0.8/codenerix_email/management/__pycache__/__init__.cpython-39.pyc
+drwxrwxr-x   0 br0th3r   (1001) br0th3r   (1001)        0 2024-05-29 05:46:30.952630 django-codenerix-email-4.0.8/codenerix_email/management/commands/
+-rw-r--r--   0 br0th3r   (1001) br0th3r   (1001)        0 2020-05-15 23:36:43.000000 django-codenerix-email-4.0.8/codenerix_email/management/commands/__init__.py
+-rw-r--r--   0 br0th3r   (1001) br0th3r   (1001)     6290 2024-04-09 05:53:51.000000 django-codenerix-email-4.0.8/codenerix_email/management/commands/send_emails.py
+-rw-r--r--   0 br0th3r   (1001) br0th3r   (1001)     1655 2024-04-09 05:53:42.000000 django-codenerix-email-4.0.8/codenerix_email/management/commands/test_email.py
+drwxrwxr-x   0 br0th3r   (1001) br0th3r   (1001)        0 2024-05-29 05:46:30.952630 django-codenerix-email-4.0.8/codenerix_email/migrations/
+-rw-r--r--   0 br0th3r   (1001) br0th3r   (1001)     3511 2020-05-15 23:36:43.000000 django-codenerix-email-4.0.8/codenerix_email/migrations/0001_initial.py
+-rw-r--r--   0 br0th3r   (1001) br0th3r   (1001)     2369 2020-05-15 23:36:43.000000 django-codenerix-email-4.0.8/codenerix_email/migrations/0002_auto_20170502_1043.py
+-rw-r--r--   0 br0th3r   (1001) br0th3r   (1001)      656 2020-05-15 23:36:43.000000 django-codenerix-email-4.0.8/codenerix_email/migrations/0003_auto_20170921_1206.py
+-rw-r--r--   0 br0th3r   (1001) br0th3r   (1001)      486 2020-05-15 23:36:43.000000 django-codenerix-email-4.0.8/codenerix_email/migrations/0004_auto_20171108_1628.py
+-rw-r--r--   0 br0th3r   (1001) br0th3r   (1001)      495 2020-05-15 23:36:43.000000 django-codenerix-email-4.0.8/codenerix_email/migrations/0005_emailmessage_retries.py
+-rw-r--r--   0 br0th3r   (1001) br0th3r   (1001)      489 2020-05-15 23:36:43.000000 django-codenerix-email-4.0.8/codenerix_email/migrations/0006_emailmessage_error.py
+-rw-r--r--   0 br0th3r   (1001) br0th3r   (1001)      602 2020-05-15 23:36:43.000000 django-codenerix-email-4.0.8/codenerix_email/migrations/0007_emailmessage_next_retry.py
+-rw-r--r--   0 br0th3r   (1001) br0th3r   (1001)      731 2020-05-15 23:36:43.000000 django-codenerix-email-4.0.8/codenerix_email/migrations/0008_auto_20171201_0928.py
+-rw-rw-r--   0 br0th3r   (1001) br0th3r   (1001)     1219 2024-05-22 11:42:23.000000 django-codenerix-email-4.0.8/codenerix_email/migrations/0009_emailmessage_opened_emailmessage_uuid.py
+-rw-r--r--   0 br0th3r   (1001) br0th3r   (1001)        0 2020-05-15 23:36:43.000000 django-codenerix-email-4.0.8/codenerix_email/migrations/__init__.py
+drwxrwxr-x   0 br0th3r   (1001) br0th3r   (1001)        0 2024-05-29 05:46:30.960630 django-codenerix-email-4.0.8/codenerix_email/migrations/__pycache__/
+-rw-r--r--   0 br0th3r   (1001) br0th3r   (1001)     2005 2023-01-29 13:03:07.000000 django-codenerix-email-4.0.8/codenerix_email/migrations/__pycache__/0001_initial.cpython-310.pyc
+-rw-r--r--   0 br0th3r   (1001) br0th3r   (1001)     3682 2024-02-14 12:11:39.000000 django-codenerix-email-4.0.8/codenerix_email/migrations/__pycache__/0001_initial.cpython-311.pyc
+-rw-r--r--   0 br0th3r   (1001) br0th3r   (1001)     2373 2020-05-15 23:36:43.000000 django-codenerix-email-4.0.8/codenerix_email/migrations/__pycache__/0001_initial.cpython-35.pyc
+-rw-r--r--   0 br0th3r   (1001) br0th3r   (1001)     2020 2022-08-14 19:56:23.000000 django-codenerix-email-4.0.8/codenerix_email/migrations/__pycache__/0001_initial.cpython-39.pyc
+-rw-r--r--   0 br0th3r   (1001) br0th3r   (1001)     1500 2023-01-29 13:03:07.000000 django-codenerix-email-4.0.8/codenerix_email/migrations/__pycache__/0002_auto_20170502_1043.cpython-310.pyc
+-rw-r--r--   0 br0th3r   (1001) br0th3r   (1001)     2664 2024-02-14 12:11:39.000000 django-codenerix-email-4.0.8/codenerix_email/migrations/__pycache__/0002_auto_20170502_1043.cpython-311.pyc
+-rw-r--r--   0 br0th3r   (1001) br0th3r   (1001)     1692 2020-05-15 23:36:43.000000 django-codenerix-email-4.0.8/codenerix_email/migrations/__pycache__/0002_auto_20170502_1043.cpython-35.pyc
+-rw-r--r--   0 br0th3r   (1001) br0th3r   (1001)     1515 2022-08-14 19:56:23.000000 django-codenerix-email-4.0.8/codenerix_email/migrations/__pycache__/0002_auto_20170502_1043.cpython-39.pyc
+-rw-r--r--   0 br0th3r   (1001) br0th3r   (1001)      694 2023-01-29 13:03:07.000000 django-codenerix-email-4.0.8/codenerix_email/migrations/__pycache__/0003_auto_20170921_1206.cpython-310.pyc
+-rw-r--r--   0 br0th3r   (1001) br0th3r   (1001)      967 2024-02-14 12:11:39.000000 django-codenerix-email-4.0.8/codenerix_email/migrations/__pycache__/0003_auto_20170921_1206.cpython-311.pyc
+-rw-r--r--   0 br0th3r   (1001) br0th3r   (1001)      782 2020-05-15 23:36:43.000000 django-codenerix-email-4.0.8/codenerix_email/migrations/__pycache__/0003_auto_20170921_1206.cpython-35.pyc
+-rw-r--r--   0 br0th3r   (1001) br0th3r   (1001)      709 2022-08-14 19:56:23.000000 django-codenerix-email-4.0.8/codenerix_email/migrations/__pycache__/0003_auto_20170921_1206.cpython-39.pyc
+-rw-r--r--   0 br0th3r   (1001) br0th3r   (1001)      676 2023-01-29 13:03:07.000000 django-codenerix-email-4.0.8/codenerix_email/migrations/__pycache__/0004_auto_20171108_1628.cpython-310.pyc
+-rw-r--r--   0 br0th3r   (1001) br0th3r   (1001)      939 2024-02-14 12:11:39.000000 django-codenerix-email-4.0.8/codenerix_email/migrations/__pycache__/0004_auto_20171108_1628.cpython-311.pyc
+-rw-r--r--   0 br0th3r   (1001) br0th3r   (1001)      713 2020-05-15 23:36:43.000000 django-codenerix-email-4.0.8/codenerix_email/migrations/__pycache__/0004_auto_20171108_1628.cpython-35.pyc
+-rw-r--r--   0 br0th3r   (1001) br0th3r   (1001)      691 2022-08-14 19:56:23.000000 django-codenerix-email-4.0.8/codenerix_email/migrations/__pycache__/0004_auto_20171108_1628.cpython-39.pyc
+-rw-r--r--   0 br0th3r   (1001) br0th3r   (1001)      691 2023-01-29 13:03:07.000000 django-codenerix-email-4.0.8/codenerix_email/migrations/__pycache__/0005_emailmessage_retries.cpython-310.pyc
+-rw-r--r--   0 br0th3r   (1001) br0th3r   (1001)      954 2024-02-14 12:11:39.000000 django-codenerix-email-4.0.8/codenerix_email/migrations/__pycache__/0005_emailmessage_retries.cpython-311.pyc
+-rw-r--r--   0 br0th3r   (1001) br0th3r   (1001)      728 2020-05-15 23:36:43.000000 django-codenerix-email-4.0.8/codenerix_email/migrations/__pycache__/0005_emailmessage_retries.cpython-35.pyc
+-rw-r--r--   0 br0th3r   (1001) br0th3r   (1001)      706 2022-08-14 19:56:23.000000 django-codenerix-email-4.0.8/codenerix_email/migrations/__pycache__/0005_emailmessage_retries.cpython-39.pyc
+-rw-r--r--   0 br0th3r   (1001) br0th3r   (1001)      675 2023-01-29 13:03:07.000000 django-codenerix-email-4.0.8/codenerix_email/migrations/__pycache__/0006_emailmessage_error.cpython-310.pyc
+-rw-r--r--   0 br0th3r   (1001) br0th3r   (1001)      938 2024-02-14 12:11:39.000000 django-codenerix-email-4.0.8/codenerix_email/migrations/__pycache__/0006_emailmessage_error.cpython-311.pyc
+-rw-r--r--   0 br0th3r   (1001) br0th3r   (1001)      712 2020-05-15 23:36:43.000000 django-codenerix-email-4.0.8/codenerix_email/migrations/__pycache__/0006_emailmessage_error.cpython-35.pyc
+-rw-r--r--   0 br0th3r   (1001) br0th3r   (1001)      690 2022-08-14 19:56:23.000000 django-codenerix-email-4.0.8/codenerix_email/migrations/__pycache__/0006_emailmessage_error.cpython-39.pyc
+-rw-r--r--   0 br0th3r   (1001) br0th3r   (1001)      802 2023-01-29 13:03:07.000000 django-codenerix-email-4.0.8/codenerix_email/migrations/__pycache__/0007_emailmessage_next_retry.cpython-310.pyc
+-rw-r--r--   0 br0th3r   (1001) br0th3r   (1001)     1111 2024-02-14 12:11:39.000000 django-codenerix-email-4.0.8/codenerix_email/migrations/__pycache__/0007_emailmessage_next_retry.cpython-311.pyc
+-rw-r--r--   0 br0th3r   (1001) br0th3r   (1001)      854 2020-05-15 23:36:43.000000 django-codenerix-email-4.0.8/codenerix_email/migrations/__pycache__/0007_emailmessage_next_retry.cpython-35.pyc
+-rw-r--r--   0 br0th3r   (1001) br0th3r   (1001)      817 2022-08-14 19:56:23.000000 django-codenerix-email-4.0.8/codenerix_email/migrations/__pycache__/0007_emailmessage_next_retry.cpython-39.pyc
+-rw-r--r--   0 br0th3r   (1001) br0th3r   (1001)      779 2023-01-29 13:03:07.000000 django-codenerix-email-4.0.8/codenerix_email/migrations/__pycache__/0008_auto_20171201_0928.cpython-310.pyc
+-rw-r--r--   0 br0th3r   (1001) br0th3r   (1001)     1178 2024-02-14 12:11:39.000000 django-codenerix-email-4.0.8/codenerix_email/migrations/__pycache__/0008_auto_20171201_0928.cpython-311.pyc
+-rw-r--r--   0 br0th3r   (1001) br0th3r   (1001)      839 2020-05-15 23:36:43.000000 django-codenerix-email-4.0.8/codenerix_email/migrations/__pycache__/0008_auto_20171201_0928.cpython-35.pyc
+-rw-r--r--   0 br0th3r   (1001) br0th3r   (1001)      794 2022-08-14 19:56:23.000000 django-codenerix-email-4.0.8/codenerix_email/migrations/__pycache__/0008_auto_20171201_0928.cpython-39.pyc
+-rw-rw-r--   0 br0th3r   (1001) br0th3r   (1001)      733 2024-05-21 07:57:54.000000 django-codenerix-email-4.0.8/codenerix_email/migrations/__pycache__/0009_delete_emailtemplatetexten.cpython-311.pyc
+-rw-rw-r--   0 br0th3r   (1001) br0th3r   (1001)     1860 2024-05-22 11:44:13.000000 django-codenerix-email-4.0.8/codenerix_email/migrations/__pycache__/0009_emailmessage_opened_emailmessage_uuid.cpython-311.pyc
+-rw-rw-r--   0 br0th3r   (1001) br0th3r   (1001)     3104 2024-05-22 11:40:40.000000 django-codenerix-email-4.0.8/codenerix_email/migrations/__pycache__/0010_emailmessage_opened_emailmessage_uuid_and_more.cpython-311.pyc
+-rw-r--r--   0 br0th3r   (1001) br0th3r   (1001)      151 2023-01-29 13:03:07.000000 django-codenerix-email-4.0.8/codenerix_email/migrations/__pycache__/__init__.cpython-310.pyc
+-rw-r--r--   0 br0th3r   (1001) br0th3r   (1001)      195 2024-02-14 12:11:39.000000 django-codenerix-email-4.0.8/codenerix_email/migrations/__pycache__/__init__.cpython-311.pyc
+-rw-r--r--   0 br0th3r   (1001) br0th3r   (1001)      147 2020-05-15 23:36:43.000000 django-codenerix-email-4.0.8/codenerix_email/migrations/__pycache__/__init__.cpython-35.pyc
+-rw-r--r--   0 br0th3r   (1001) br0th3r   (1001)      168 2022-08-14 19:56:23.000000 django-codenerix-email-4.0.8/codenerix_email/migrations/__pycache__/__init__.cpython-39.pyc
+-rw-r--r--   0 br0th3r   (1001) br0th3r   (1001)    13280 2024-05-27 07:00:20.000000 django-codenerix-email-4.0.8/codenerix_email/models.py
+drwxrwxr-x   0 br0th3r   (1001) br0th3r   (1001)        0 2024-05-29 05:46:30.948630 django-codenerix-email-4.0.8/codenerix_email/static/
+drwxrwxr-x   0 br0th3r   (1001) br0th3r   (1001)        0 2024-05-29 05:46:30.948630 django-codenerix-email-4.0.8/codenerix_email/static/codenerix_email/
+drwxrwxr-x   0 br0th3r   (1001) br0th3r   (1001)        0 2024-05-29 05:46:30.960630 django-codenerix-email-4.0.8/codenerix_email/static/codenerix_email/partials/
+-rw-r--r--   0 br0th3r   (1001) br0th3r   (1001)     1060 2024-05-22 11:47:17.000000 django-codenerix-email-4.0.8/codenerix_email/static/codenerix_email/partials/emailmessages_rows.html
+-rw-r--r--   0 br0th3r   (1001) br0th3r   (1001)     2595 2022-08-14 19:56:23.000000 django-codenerix-email-4.0.8/codenerix_email/urls.py
+-rw-r--r--   0 br0th3r   (1001) br0th3r   (1001)      873 2024-05-22 12:21:01.000000 django-codenerix-email-4.0.8/codenerix_email/urls_frontend.py
+-rw-r--r--   0 br0th3r   (1001) br0th3r   (1001)     4758 2024-05-29 05:40:38.000000 django-codenerix-email-4.0.8/codenerix_email/views.py
+drwxrwxr-x   0 br0th3r   (1001) br0th3r   (1001)        0 2024-05-29 05:46:30.960630 django-codenerix-email-4.0.8/django_codenerix_email.egg-info/
+-rw-r--r--   0 br0th3r   (1001) br0th3r   (1001)     2543 2024-05-29 05:46:30.000000 django-codenerix-email-4.0.8/django_codenerix_email.egg-info/PKG-INFO
+-rw-r--r--   0 br0th3r   (1001) br0th3r   (1001)     4619 2024-05-29 05:46:30.000000 django-codenerix-email-4.0.8/django_codenerix_email.egg-info/SOURCES.txt
+-rw-r--r--   0 br0th3r   (1001) br0th3r   (1001)        1 2024-05-29 05:46:30.000000 django-codenerix-email-4.0.8/django_codenerix_email.egg-info/dependency_links.txt
+-rw-r--r--   0 br0th3r   (1001) br0th3r   (1001)        1 2020-05-15 23:36:43.000000 django-codenerix-email-4.0.8/django_codenerix_email.egg-info/not-zip-safe
+-rw-r--r--   0 br0th3r   (1001) br0th3r   (1001)       53 2024-05-29 05:46:30.000000 django-codenerix-email-4.0.8/django_codenerix_email.egg-info/requires.txt
+-rw-r--r--   0 br0th3r   (1001) br0th3r   (1001)       16 2024-05-29 05:46:30.000000 django-codenerix-email-4.0.8/django_codenerix_email.egg-info/top_level.txt
+-rw-rw-r--   0 br0th3r   (1001) br0th3r   (1001)       38 2024-05-29 05:46:30.960630 django-codenerix-email-4.0.8/setup.cfg
+-rw-r--r--   0 br0th3r   (1001) br0th3r   (1001)     1707 2024-04-08 11:04:22.000000 django-codenerix-email-4.0.8/setup.py
```

### Comparing `django-codenerix-email-4.0.7/LICENSE` & `django-codenerix-email-4.0.8/LICENSE`

 * *Files identical despite different names*

### Comparing `django-codenerix-email-4.0.7/PKG-INFO` & `django-codenerix-email-4.0.8/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: django-codenerix-email
-Version: 4.0.7
+Version: 4.0.8
 Summary: Codenerix Email is a module that enables CODENERIX to set send emails in a general manner.
 Home-page: https://github.com/codenerix/django-codenerix-email
 Author: Juan Miguel Taboada Godoy <juanmi@juanmitaboada.com>, Juan Soler Ruiz <soleronline@gmail.com>
 License: Apache License Version 2.0
 Keywords: django,codenerix,management,erp,crm,send email
 Platform: OS Independent
 Classifier: Environment :: Web Environment
```

### Comparing `django-codenerix-email-4.0.7/README.rst` & `django-codenerix-email-4.0.8/README.rst`

 * *Files identical despite different names*

### Comparing `django-codenerix-email-4.0.7/codenerix_email/admin.py` & `django-codenerix-email-4.0.8/codenerix_email/admin.py`

 * *Files identical despite different names*

### Comparing `django-codenerix-email-4.0.7/codenerix_email/forms.py` & `django-codenerix-email-4.0.8/codenerix_email/forms.py`

 * *Files identical despite different names*

### Comparing `django-codenerix-email-4.0.7/codenerix_email/management/commands/send_emails.py` & `django-codenerix-email-4.0.8/codenerix_email/management/commands/send_emails.py`

 * *Files identical despite different names*

### Comparing `django-codenerix-email-4.0.7/codenerix_email/management/commands/test_email.py` & `django-codenerix-email-4.0.8/codenerix_email/management/commands/test_email.py`

 * *Files identical despite different names*

### Comparing `django-codenerix-email-4.0.7/codenerix_email/migrations/0001_initial.py` & `django-codenerix-email-4.0.8/codenerix_email/migrations/0001_initial.py`

 * *Files identical despite different names*

### Comparing `django-codenerix-email-4.0.7/codenerix_email/migrations/0002_auto_20170502_1043.py` & `django-codenerix-email-4.0.8/codenerix_email/migrations/0002_auto_20170502_1043.py`

 * *Files identical despite different names*

### Comparing `django-codenerix-email-4.0.7/codenerix_email/migrations/0003_auto_20170921_1206.py` & `django-codenerix-email-4.0.8/codenerix_email/migrations/0003_auto_20170921_1206.py`

 * *Files identical despite different names*

### Comparing `django-codenerix-email-4.0.7/codenerix_email/migrations/0007_emailmessage_next_retry.py` & `django-codenerix-email-4.0.8/codenerix_email/migrations/0007_emailmessage_next_retry.py`

 * *Files identical despite different names*

### Comparing `django-codenerix-email-4.0.7/codenerix_email/migrations/0008_auto_20171201_0928.py` & `django-codenerix-email-4.0.8/codenerix_email/migrations/0008_auto_20171201_0928.py`

 * *Files identical despite different names*

### Comparing `django-codenerix-email-4.0.7/codenerix_email/migrations/0009_emailmessage_opened_emailmessage_uuid.py` & `django-codenerix-email-4.0.8/codenerix_email/migrations/0009_emailmessage_opened_emailmessage_uuid.py`

 * *Files identical despite different names*

### Comparing `django-codenerix-email-4.0.7/codenerix_email/migrations/__pycache__/0001_initial.cpython-310.pyc` & `django-codenerix-email-4.0.8/codenerix_email/migrations/__pycache__/0001_initial.cpython-310.pyc`

 * *Files identical despite different names*

### Comparing `django-codenerix-email-4.0.7/codenerix_email/migrations/__pycache__/0001_initial.cpython-311.pyc` & `django-codenerix-email-4.0.8/codenerix_email/migrations/__pycache__/0001_initial.cpython-311.pyc`

 * *Files identical despite different names*

### Comparing `django-codenerix-email-4.0.7/codenerix_email/migrations/__pycache__/0001_initial.cpython-35.pyc` & `django-codenerix-email-4.0.8/codenerix_email/migrations/__pycache__/0001_initial.cpython-35.pyc`

 * *Files identical despite different names*

### Comparing `django-codenerix-email-4.0.7/codenerix_email/migrations/__pycache__/0001_initial.cpython-39.pyc` & `django-codenerix-email-4.0.8/codenerix_email/migrations/__pycache__/0001_initial.cpython-39.pyc`

 * *Files identical despite different names*

### Comparing `django-codenerix-email-4.0.7/codenerix_email/migrations/__pycache__/0002_auto_20170502_1043.cpython-310.pyc` & `django-codenerix-email-4.0.8/codenerix_email/migrations/__pycache__/0002_auto_20170502_1043.cpython-310.pyc`

 * *Files identical despite different names*

### Comparing `django-codenerix-email-4.0.7/codenerix_email/migrations/__pycache__/0002_auto_20170502_1043.cpython-311.pyc` & `django-codenerix-email-4.0.8/codenerix_email/migrations/__pycache__/0002_auto_20170502_1043.cpython-311.pyc`

 * *Files identical despite different names*

### Comparing `django-codenerix-email-4.0.7/codenerix_email/migrations/__pycache__/0002_auto_20170502_1043.cpython-35.pyc` & `django-codenerix-email-4.0.8/codenerix_email/migrations/__pycache__/0002_auto_20170502_1043.cpython-35.pyc`

 * *Files identical despite different names*

### Comparing `django-codenerix-email-4.0.7/codenerix_email/migrations/__pycache__/0002_auto_20170502_1043.cpython-39.pyc` & `django-codenerix-email-4.0.8/codenerix_email/migrations/__pycache__/0002_auto_20170502_1043.cpython-39.pyc`

 * *Files identical despite different names*

### Comparing `django-codenerix-email-4.0.7/codenerix_email/migrations/__pycache__/0003_auto_20170921_1206.cpython-310.pyc` & `django-codenerix-email-4.0.8/codenerix_email/migrations/__pycache__/0003_auto_20170921_1206.cpython-310.pyc`

 * *Files identical despite different names*

### Comparing `django-codenerix-email-4.0.7/codenerix_email/migrations/__pycache__/0003_auto_20170921_1206.cpython-311.pyc` & `django-codenerix-email-4.0.8/codenerix_email/migrations/__pycache__/0003_auto_20170921_1206.cpython-311.pyc`

 * *Files identical despite different names*

### Comparing `django-codenerix-email-4.0.7/codenerix_email/migrations/__pycache__/0003_auto_20170921_1206.cpython-35.pyc` & `django-codenerix-email-4.0.8/codenerix_email/migrations/__pycache__/0003_auto_20170921_1206.cpython-35.pyc`

 * *Files identical despite different names*

### Comparing `django-codenerix-email-4.0.7/codenerix_email/migrations/__pycache__/0003_auto_20170921_1206.cpython-39.pyc` & `django-codenerix-email-4.0.8/codenerix_email/migrations/__pycache__/0003_auto_20170921_1206.cpython-39.pyc`

 * *Files identical despite different names*

### Comparing `django-codenerix-email-4.0.7/codenerix_email/migrations/__pycache__/0004_auto_20171108_1628.cpython-310.pyc` & `django-codenerix-email-4.0.8/codenerix_email/migrations/__pycache__/0004_auto_20171108_1628.cpython-310.pyc`

 * *Files identical despite different names*

### Comparing `django-codenerix-email-4.0.7/codenerix_email/migrations/__pycache__/0004_auto_20171108_1628.cpython-311.pyc` & `django-codenerix-email-4.0.8/codenerix_email/migrations/__pycache__/0004_auto_20171108_1628.cpython-311.pyc`

 * *Files identical despite different names*

### Comparing `django-codenerix-email-4.0.7/codenerix_email/migrations/__pycache__/0004_auto_20171108_1628.cpython-35.pyc` & `django-codenerix-email-4.0.8/codenerix_email/migrations/__pycache__/0004_auto_20171108_1628.cpython-35.pyc`

 * *Files identical despite different names*

### Comparing `django-codenerix-email-4.0.7/codenerix_email/migrations/__pycache__/0004_auto_20171108_1628.cpython-39.pyc` & `django-codenerix-email-4.0.8/codenerix_email/migrations/__pycache__/0004_auto_20171108_1628.cpython-39.pyc`

 * *Files identical despite different names*

### Comparing `django-codenerix-email-4.0.7/codenerix_email/migrations/__pycache__/0005_emailmessage_retries.cpython-310.pyc` & `django-codenerix-email-4.0.8/codenerix_email/migrations/__pycache__/0005_emailmessage_retries.cpython-310.pyc`

 * *Files identical despite different names*

### Comparing `django-codenerix-email-4.0.7/codenerix_email/migrations/__pycache__/0005_emailmessage_retries.cpython-311.pyc` & `django-codenerix-email-4.0.8/codenerix_email/migrations/__pycache__/0005_emailmessage_retries.cpython-311.pyc`

 * *Files identical despite different names*

### Comparing `django-codenerix-email-4.0.7/codenerix_email/migrations/__pycache__/0005_emailmessage_retries.cpython-35.pyc` & `django-codenerix-email-4.0.8/codenerix_email/migrations/__pycache__/0005_emailmessage_retries.cpython-35.pyc`

 * *Files identical despite different names*

### Comparing `django-codenerix-email-4.0.7/codenerix_email/migrations/__pycache__/0005_emailmessage_retries.cpython-39.pyc` & `django-codenerix-email-4.0.8/codenerix_email/migrations/__pycache__/0005_emailmessage_retries.cpython-39.pyc`

 * *Files identical despite different names*

### Comparing `django-codenerix-email-4.0.7/codenerix_email/migrations/__pycache__/0006_emailmessage_error.cpython-310.pyc` & `django-codenerix-email-4.0.8/codenerix_email/migrations/__pycache__/0006_emailmessage_error.cpython-310.pyc`

 * *Files identical despite different names*

### Comparing `django-codenerix-email-4.0.7/codenerix_email/migrations/__pycache__/0006_emailmessage_error.cpython-311.pyc` & `django-codenerix-email-4.0.8/codenerix_email/migrations/__pycache__/0006_emailmessage_error.cpython-311.pyc`

 * *Files identical despite different names*

### Comparing `django-codenerix-email-4.0.7/codenerix_email/migrations/__pycache__/0006_emailmessage_error.cpython-35.pyc` & `django-codenerix-email-4.0.8/codenerix_email/migrations/__pycache__/0006_emailmessage_error.cpython-35.pyc`

 * *Files identical despite different names*

### Comparing `django-codenerix-email-4.0.7/codenerix_email/migrations/__pycache__/0006_emailmessage_error.cpython-39.pyc` & `django-codenerix-email-4.0.8/codenerix_email/migrations/__pycache__/0006_emailmessage_error.cpython-39.pyc`

 * *Files identical despite different names*

### Comparing `django-codenerix-email-4.0.7/codenerix_email/migrations/__pycache__/0007_emailmessage_next_retry.cpython-310.pyc` & `django-codenerix-email-4.0.8/codenerix_email/migrations/__pycache__/0007_emailmessage_next_retry.cpython-310.pyc`

 * *Files identical despite different names*

### Comparing `django-codenerix-email-4.0.7/codenerix_email/migrations/__pycache__/0007_emailmessage_next_retry.cpython-311.pyc` & `django-codenerix-email-4.0.8/codenerix_email/migrations/__pycache__/0007_emailmessage_next_retry.cpython-311.pyc`

 * *Files identical despite different names*

### Comparing `django-codenerix-email-4.0.7/codenerix_email/migrations/__pycache__/0007_emailmessage_next_retry.cpython-35.pyc` & `django-codenerix-email-4.0.8/codenerix_email/migrations/__pycache__/0007_emailmessage_next_retry.cpython-35.pyc`

 * *Files identical despite different names*

### Comparing `django-codenerix-email-4.0.7/codenerix_email/migrations/__pycache__/0007_emailmessage_next_retry.cpython-39.pyc` & `django-codenerix-email-4.0.8/codenerix_email/migrations/__pycache__/0007_emailmessage_next_retry.cpython-39.pyc`

 * *Files identical despite different names*

### Comparing `django-codenerix-email-4.0.7/codenerix_email/migrations/__pycache__/0008_auto_20171201_0928.cpython-310.pyc` & `django-codenerix-email-4.0.8/codenerix_email/migrations/__pycache__/0008_auto_20171201_0928.cpython-310.pyc`

 * *Files identical despite different names*

### Comparing `django-codenerix-email-4.0.7/codenerix_email/migrations/__pycache__/0008_auto_20171201_0928.cpython-311.pyc` & `django-codenerix-email-4.0.8/codenerix_email/migrations/__pycache__/0008_auto_20171201_0928.cpython-311.pyc`

 * *Files identical despite different names*

### Comparing `django-codenerix-email-4.0.7/codenerix_email/migrations/__pycache__/0008_auto_20171201_0928.cpython-35.pyc` & `django-codenerix-email-4.0.8/codenerix_email/migrations/__pycache__/0008_auto_20171201_0928.cpython-35.pyc`

 * *Files identical despite different names*

### Comparing `django-codenerix-email-4.0.7/codenerix_email/migrations/__pycache__/0008_auto_20171201_0928.cpython-39.pyc` & `django-codenerix-email-4.0.8/codenerix_email/migrations/__pycache__/0008_auto_20171201_0928.cpython-39.pyc`

 * *Files identical despite different names*

### Comparing `django-codenerix-email-4.0.7/codenerix_email/migrations/__pycache__/0009_delete_emailtemplatetexten.cpython-311.pyc` & `django-codenerix-email-4.0.8/codenerix_email/migrations/__pycache__/0009_delete_emailtemplatetexten.cpython-311.pyc`

 * *Files identical despite different names*

### Comparing `django-codenerix-email-4.0.7/codenerix_email/migrations/__pycache__/0009_emailmessage_opened_emailmessage_uuid.cpython-311.pyc` & `django-codenerix-email-4.0.8/codenerix_email/migrations/__pycache__/0009_emailmessage_opened_emailmessage_uuid.cpython-311.pyc`

 * *Files identical despite different names*

### Comparing `django-codenerix-email-4.0.7/codenerix_email/migrations/__pycache__/0010_emailmessage_opened_emailmessage_uuid_and_more.cpython-311.pyc` & `django-codenerix-email-4.0.8/codenerix_email/migrations/__pycache__/0010_emailmessage_opened_emailmessage_uuid_and_more.cpython-311.pyc`

 * *Files identical despite different names*

### Comparing `django-codenerix-email-4.0.7/codenerix_email/models.py` & `django-codenerix-email-4.0.8/codenerix_email/models.py`

 * *Files identical despite different names*

### Comparing `django-codenerix-email-4.0.7/codenerix_email/static/codenerix_email/partials/emailmessages_rows.html` & `django-codenerix-email-4.0.8/codenerix_email/static/codenerix_email/partials/emailmessages_rows.html`

 * *Files identical despite different names*

### Comparing `django-codenerix-email-4.0.7/codenerix_email/urls.py` & `django-codenerix-email-4.0.8/codenerix_email/urls.py`

 * *Files identical despite different names*

### Comparing `django-codenerix-email-4.0.7/codenerix_email/urls_frontend.py` & `django-codenerix-email-4.0.8/codenerix_email/urls_frontend.py`

 * *Files identical despite different names*

### Comparing `django-codenerix-email-4.0.7/codenerix_email/views.py` & `django-codenerix-email-4.0.8/codenerix_email/views.py`

 * *Files 2% similar despite different names*

```diff
@@ -106,16 +106,16 @@
 
 
 # ############################################
 # EmailTemplate
 class EmailTemplateList(GenList):
     model = EmailTemplate
     extra_context = {
-        "menu": ["EmailTemplate", "people"],
-        "bread": [_("EmailTemplate"), _("People")],
+        "menu": ["codenerix_email", "emailtemplate"],
+        "bread": [_("Emails"), _("Email Template")],
     }
 
 
 class EmailTemplateCreate(MultiForm, GenCreate):
     model = EmailTemplate
     form_class = EmailTemplateForm
     forms = formsfull["EmailTemplate"]
@@ -149,16 +149,16 @@
     gentranslate = {
         "sending": _("Sending"),
         "sent": _("Sent"),
         "notsent": _("Not sent!"),
         "waiting": _("Waiting"),
     }
     extra_context = {
-        "menu": ["EmailMessage", "people"],
-        "bread": [_("EmailMessage"), _("People")],
+        "menu": ["codenerix_email", "emailmessages"],
+        "bread": [_("Emails"), _("Email Messages")],
     }
 
 
 class EmailMessageCreate(GenCreate):
     model = EmailMessage
     form_class = EmailMessageForm
```

### Comparing `django-codenerix-email-4.0.7/django_codenerix_email.egg-info/PKG-INFO` & `django-codenerix-email-4.0.8/django_codenerix_email.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: django-codenerix-email
-Version: 4.0.7
+Version: 4.0.8
 Summary: Codenerix Email is a module that enables CODENERIX to set send emails in a general manner.
 Home-page: https://github.com/codenerix/django-codenerix-email
 Author: Juan Miguel Taboada Godoy <juanmi@juanmitaboada.com>, Juan Soler Ruiz <soleronline@gmail.com>
 License: Apache License Version 2.0
 Keywords: django,codenerix,management,erp,crm,send email
 Platform: OS Independent
 Classifier: Environment :: Web Environment
```

### Comparing `django-codenerix-email-4.0.7/django_codenerix_email.egg-info/SOURCES.txt` & `django-codenerix-email-4.0.8/django_codenerix_email.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `django-codenerix-email-4.0.7/setup.py` & `django-codenerix-email-4.0.8/setup.py`

 * *Files identical despite different names*

