# Comparing `tmp/django-audit-events-0.3.1.dev0.tar.gz` & `tmp/django-audit-events-0.3.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/django-audit-events-0.3.1.dev0.tar", last modified: Sun May 12 22:25:28 2024, max compression
+gzip compressed data, was "dist/django-audit-events-0.3.2.tar", last modified: Tue May 28 13:34:24 2024, max compression
```

## Comparing `django-audit-events-0.3.1.dev0.tar` & `django-audit-events-0.3.2.tar`

### file list

```diff
@@ -1,70 +1,70 @@
-drwxrwxrwx   0 root         (0) root         (0)        0 2024-05-12 22:25:28.000000 django-audit-events-0.3.1.dev0/
--rw-rw-rw-   0 root         (0) root         (0)      220 2024-05-12 22:25:07.000000 django-audit-events-0.3.1.dev0/.editorconfig
--rw-rw-rw-   0 root         (0) root         (0)      101 2024-05-12 22:25:07.000000 django-audit-events-0.3.1.dev0/.gitignore
--rw-rw-rw-   0 root         (0) root         (0)      113 2024-05-12 22:25:07.000000 django-audit-events-0.3.1.dev0/.isort.cfg
--rw-rw-rw-   0 root         (0) root         (0)       27 2024-05-12 22:25:07.000000 django-audit-events-0.3.1.dev0/CHANGELOG.md
--rw-rw-rw-   0 root         (0) root         (0)     1050 2024-05-12 22:25:07.000000 django-audit-events-0.3.1.dev0/LICENSE.txt
--rw-rw-rw-   0 root         (0) root         (0)     3512 2024-05-12 22:25:28.000000 django-audit-events-0.3.1.dev0/PKG-INFO
--rw-rw-rw-   0 root         (0) root         (0)     1714 2024-05-12 22:25:07.000000 django-audit-events-0.3.1.dev0/README.md
--rw-rw-rw-   0 root         (0) root         (0)     2620 2024-05-12 22:25:07.000000 django-audit-events-0.3.1.dev0/bitbucket-pipelines.yml
-drwxrwxrwx   0 root         (0) root         (0)        0 2024-05-12 22:25:28.000000 django-audit-events-0.3.1.dev0/django_audit_events/
--rw-rw-rw-   0 root         (0) root         (0)      380 2024-05-12 22:25:07.000000 django-audit-events-0.3.1.dev0/django_audit_events/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)      396 2024-05-12 22:25:07.000000 django-audit-events-0.3.1.dev0/django_audit_events/admin.py
--rw-rw-rw-   0 root         (0) root         (0)      447 2024-05-12 22:25:07.000000 django-audit-events-0.3.1.dev0/django_audit_events/apps.py
--rw-rw-rw-   0 root         (0) root         (0)      733 2024-05-12 22:25:07.000000 django-audit-events-0.3.1.dev0/django_audit_events/conf.py
--rw-rw-rw-   0 root         (0) root         (0)     4523 2024-05-12 22:25:07.000000 django-audit-events-0.3.1.dev0/django_audit_events/context.py
--rw-rw-rw-   0 root         (0) root         (0)     1842 2024-05-12 22:25:07.000000 django-audit-events-0.3.1.dev0/django_audit_events/filters.py
-drwxrwxrwx   0 root         (0) root         (0)        0 2024-05-12 22:25:28.000000 django-audit-events-0.3.1.dev0/django_audit_events/locale/
-drwxrwxrwx   0 root         (0) root         (0)        0 2024-05-12 22:25:28.000000 django-audit-events-0.3.1.dev0/django_audit_events/locale/tr/
-drwxrwxrwx   0 root         (0) root         (0)        0 2024-05-12 22:25:28.000000 django-audit-events-0.3.1.dev0/django_audit_events/locale/tr/LC_MESSAGES/
--rw-rw-rw-   0 root         (0) root         (0)     1544 2024-05-12 22:25:07.000000 django-audit-events-0.3.1.dev0/django_audit_events/locale/tr/LC_MESSAGES/django.po
--rw-rw-rw-   0 root         (0) root         (0)      843 2024-05-12 22:25:07.000000 django-audit-events-0.3.1.dev0/django_audit_events/middleware.py
-drwxrwxrwx   0 root         (0) root         (0)        0 2024-05-12 22:25:28.000000 django-audit-events-0.3.1.dev0/django_audit_events/migrations/
--rw-rw-rw-   0 root         (0) root         (0)     1984 2024-05-12 22:25:07.000000 django-audit-events-0.3.1.dev0/django_audit_events/migrations/0001_initial.py
--rw-rw-rw-   0 root         (0) root         (0)     2207 2024-05-12 22:25:07.000000 django-audit-events-0.3.1.dev0/django_audit_events/migrations/0002_archivedauditevent.py
--rw-rw-rw-   0 root         (0) root         (0)      712 2024-05-12 22:25:07.000000 django-audit-events-0.3.1.dev0/django_audit_events/migrations/0003_auto_20201218_1113.py
--rw-rw-rw-   0 root         (0) root         (0)      650 2024-05-12 22:25:07.000000 django-audit-events-0.3.1.dev0/django_audit_events/migrations/0004_auto_20210127_2021.py
--rw-rw-rw-   0 root         (0) root         (0)      768 2024-05-12 22:25:07.000000 django-audit-events-0.3.1.dev0/django_audit_events/migrations/0005_auto_20220215_0756.py
--rw-rw-rw-   0 root         (0) root         (0)      669 2024-05-12 22:25:07.000000 django-audit-events-0.3.1.dev0/django_audit_events/migrations/0006_auto_20220920_1327.py
--rw-rw-rw-   0 root         (0) root         (0)        0 2024-05-12 22:25:07.000000 django-audit-events-0.3.1.dev0/django_audit_events/migrations/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)      857 2024-05-12 22:25:07.000000 django-audit-events-0.3.1.dev0/django_audit_events/mixin.py
--rw-rw-rw-   0 root         (0) root         (0)     4659 2024-05-12 22:25:07.000000 django-audit-events-0.3.1.dev0/django_audit_events/models.py
--rw-rw-rw-   0 root         (0) root         (0)      476 2024-05-12 22:25:07.000000 django-audit-events-0.3.1.dev0/django_audit_events/serializers.py
--rw-rw-rw-   0 root         (0) root         (0)     1675 2024-05-12 22:25:07.000000 django-audit-events-0.3.1.dev0/django_audit_events/tasks.py
-drwxrwxrwx   0 root         (0) root         (0)        0 2024-05-12 22:25:28.000000 django-audit-events-0.3.1.dev0/django_audit_events/tests/
--rw-rw-rw-   0 root         (0) root         (0)        0 2024-05-12 22:25:07.000000 django-audit-events-0.3.1.dev0/django_audit_events/tests/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)      290 2024-05-12 22:25:07.000000 django-audit-events-0.3.1.dev0/django_audit_events/tests/test_conf.py
--rw-rw-rw-   0 root         (0) root         (0)     6001 2024-05-12 22:25:07.000000 django-audit-events-0.3.1.dev0/django_audit_events/tests/test_context.py
--rw-rw-rw-   0 root         (0) root         (0)     1362 2024-05-12 22:25:07.000000 django-audit-events-0.3.1.dev0/django_audit_events/tests/test_middleware.py
--rw-rw-rw-   0 root         (0) root         (0)     1539 2024-05-12 22:25:07.000000 django-audit-events-0.3.1.dev0/django_audit_events/tests/test_mixin.py
--rw-rw-rw-   0 root         (0) root         (0)     2062 2024-05-12 22:25:07.000000 django-audit-events-0.3.1.dev0/django_audit_events/tests/test_models.py
--rw-rw-rw-   0 root         (0) root         (0)     2548 2024-05-12 22:25:07.000000 django-audit-events-0.3.1.dev0/django_audit_events/tests/test_tasks.py
--rw-rw-rw-   0 root         (0) root         (0)       58 2024-05-12 22:25:07.000000 django-audit-events-0.3.1.dev0/django_audit_events/tests/urls.py
-drwxrwxrwx   0 root         (0) root         (0)        0 2024-05-12 22:25:28.000000 django-audit-events-0.3.1.dev0/django_audit_events/tests/utils/
--rw-rw-rw-   0 root         (0) root         (0)       65 2024-05-12 22:25:07.000000 django-audit-events-0.3.1.dev0/django_audit_events/tests/utils/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)      160 2024-05-12 22:25:07.000000 django-audit-events-0.3.1.dev0/django_audit_events/tests/utils/models.py
--rw-rw-rw-   0 root         (0) root         (0)      205 2024-05-12 22:25:07.000000 django-audit-events-0.3.1.dev0/django_audit_events/urls.py
--rw-rw-rw-   0 root         (0) root         (0)      917 2024-05-12 22:25:07.000000 django-audit-events-0.3.1.dev0/django_audit_events/utils.py
--rw-rw-rw-   0 root         (0) root         (0)       27 2024-05-12 22:25:28.000000 django-audit-events-0.3.1.dev0/django_audit_events/version.py
--rw-rw-rw-   0 root         (0) root         (0)     1060 2024-05-12 22:25:07.000000 django-audit-events-0.3.1.dev0/django_audit_events/views.py
-drwxrwxrwx   0 root         (0) root         (0)        0 2024-05-12 22:25:28.000000 django-audit-events-0.3.1.dev0/django_audit_events.egg-info/
--rw-rw-rw-   0 root         (0) root         (0)     3512 2024-05-12 22:25:28.000000 django-audit-events-0.3.1.dev0/django_audit_events.egg-info/PKG-INFO
--rw-rw-rw-   0 root         (0) root         (0)     1798 2024-05-12 22:25:28.000000 django-audit-events-0.3.1.dev0/django_audit_events.egg-info/SOURCES.txt
--rw-rw-rw-   0 root         (0) root         (0)        1 2024-05-12 22:25:28.000000 django-audit-events-0.3.1.dev0/django_audit_events.egg-info/dependency_links.txt
--rw-rw-rw-   0 root         (0) root         (0)        1 2024-05-12 22:25:28.000000 django-audit-events-0.3.1.dev0/django_audit_events.egg-info/not-zip-safe
--rw-rw-rw-   0 root         (0) root         (0)       20 2024-05-12 22:25:28.000000 django-audit-events-0.3.1.dev0/django_audit_events.egg-info/top_level.txt
-drwxrwxrwx   0 root         (0) root         (0)        0 2024-05-12 22:25:28.000000 django-audit-events-0.3.1.dev0/docs/
--rw-rw-rw-   0 root         (0) root         (0)      634 2024-05-12 22:25:07.000000 django-audit-events-0.3.1.dev0/docs/Makefile
--rw-rw-rw-   0 root         (0) root         (0)     1609 2024-05-12 22:25:07.000000 django-audit-events-0.3.1.dev0/docs/advanced.rst
--rw-rw-rw-   0 root         (0) root         (0)     2080 2024-05-12 22:25:07.000000 django-audit-events-0.3.1.dev0/docs/conf.py
--rw-rw-rw-   0 root         (0) root         (0)     1533 2024-05-12 22:25:07.000000 django-audit-events-0.3.1.dev0/docs/configuration.rst
--rw-rw-rw-   0 root         (0) root         (0)      944 2024-05-12 22:25:07.000000 django-audit-events-0.3.1.dev0/docs/index.rst
--rw-rw-rw-   0 root         (0) root         (0)     1252 2024-05-12 22:25:07.000000 django-audit-events-0.3.1.dev0/docs/introduction.rst
--rw-rw-rw-   0 root         (0) root         (0)      795 2024-05-12 22:25:07.000000 django-audit-events-0.3.1.dev0/docs/make.bat
--rw-rw-rw-   0 root         (0) root         (0)     2265 2024-05-12 22:25:07.000000 django-audit-events-0.3.1.dev0/docs/quickstart.rst
--rw-rw-rw-   0 root         (0) root         (0)      310 2024-05-12 22:25:07.000000 django-audit-events-0.3.1.dev0/pyproject.toml
--rw-rw-rw-   0 root         (0) root         (0)      396 2024-05-12 22:25:07.000000 django-audit-events-0.3.1.dev0/requirements.txt
--rw-rw-rw-   0 root         (0) root         (0)     2337 2024-05-12 22:25:07.000000 django-audit-events-0.3.1.dev0/runtests.py
--rw-rw-rw-   0 root         (0) root         (0)       38 2024-05-12 22:25:28.000000 django-audit-events-0.3.1.dev0/setup.cfg
--rw-rw-rw-   0 root         (0) root         (0)     2628 2024-05-12 22:25:07.000000 django-audit-events-0.3.1.dev0/setup.py
--rw-rw-rw-   0 root         (0) root         (0)     1819 2024-05-12 22:25:07.000000 django-audit-events-0.3.1.dev0/tox.ini
+drwxrwxrwx   0 root         (0) root         (0)        0 2024-05-28 13:34:24.000000 django-audit-events-0.3.2/
+-rw-rw-rw-   0 root         (0) root         (0)      220 2024-05-28 13:33:58.000000 django-audit-events-0.3.2/.editorconfig
+-rw-rw-rw-   0 root         (0) root         (0)      101 2024-05-28 13:33:58.000000 django-audit-events-0.3.2/.gitignore
+-rw-rw-rw-   0 root         (0) root         (0)      113 2024-05-28 13:33:58.000000 django-audit-events-0.3.2/.isort.cfg
+-rw-rw-rw-   0 root         (0) root         (0)       27 2024-05-28 13:33:58.000000 django-audit-events-0.3.2/CHANGELOG.md
+-rw-rw-rw-   0 root         (0) root         (0)     1050 2024-05-28 13:33:58.000000 django-audit-events-0.3.2/LICENSE.txt
+-rw-rw-rw-   0 root         (0) root         (0)     3507 2024-05-28 13:34:24.000000 django-audit-events-0.3.2/PKG-INFO
+-rw-rw-rw-   0 root         (0) root         (0)     1714 2024-05-28 13:33:58.000000 django-audit-events-0.3.2/README.md
+-rw-rw-rw-   0 root         (0) root         (0)     2924 2024-05-28 13:33:58.000000 django-audit-events-0.3.2/bitbucket-pipelines.yml
+drwxrwxrwx   0 root         (0) root         (0)        0 2024-05-28 13:34:24.000000 django-audit-events-0.3.2/django_audit_events/
+-rw-rw-rw-   0 root         (0) root         (0)      380 2024-05-28 13:33:58.000000 django-audit-events-0.3.2/django_audit_events/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)      396 2024-05-28 13:33:58.000000 django-audit-events-0.3.2/django_audit_events/admin.py
+-rw-rw-rw-   0 root         (0) root         (0)      447 2024-05-28 13:33:58.000000 django-audit-events-0.3.2/django_audit_events/apps.py
+-rw-rw-rw-   0 root         (0) root         (0)      733 2024-05-28 13:33:58.000000 django-audit-events-0.3.2/django_audit_events/conf.py
+-rw-rw-rw-   0 root         (0) root         (0)     4523 2024-05-28 13:33:58.000000 django-audit-events-0.3.2/django_audit_events/context.py
+-rw-rw-rw-   0 root         (0) root         (0)     1842 2024-05-28 13:33:58.000000 django-audit-events-0.3.2/django_audit_events/filters.py
+drwxrwxrwx   0 root         (0) root         (0)        0 2024-05-28 13:34:24.000000 django-audit-events-0.3.2/django_audit_events/locale/
+drwxrwxrwx   0 root         (0) root         (0)        0 2024-05-28 13:34:24.000000 django-audit-events-0.3.2/django_audit_events/locale/tr/
+drwxrwxrwx   0 root         (0) root         (0)        0 2024-05-28 13:34:24.000000 django-audit-events-0.3.2/django_audit_events/locale/tr/LC_MESSAGES/
+-rw-rw-rw-   0 root         (0) root         (0)     1544 2024-05-28 13:33:58.000000 django-audit-events-0.3.2/django_audit_events/locale/tr/LC_MESSAGES/django.po
+-rw-rw-rw-   0 root         (0) root         (0)      843 2024-05-28 13:33:58.000000 django-audit-events-0.3.2/django_audit_events/middleware.py
+drwxrwxrwx   0 root         (0) root         (0)        0 2024-05-28 13:34:24.000000 django-audit-events-0.3.2/django_audit_events/migrations/
+-rw-rw-rw-   0 root         (0) root         (0)     1984 2024-05-28 13:33:58.000000 django-audit-events-0.3.2/django_audit_events/migrations/0001_initial.py
+-rw-rw-rw-   0 root         (0) root         (0)     2207 2024-05-28 13:33:58.000000 django-audit-events-0.3.2/django_audit_events/migrations/0002_archivedauditevent.py
+-rw-rw-rw-   0 root         (0) root         (0)      712 2024-05-28 13:33:58.000000 django-audit-events-0.3.2/django_audit_events/migrations/0003_auto_20201218_1113.py
+-rw-rw-rw-   0 root         (0) root         (0)      650 2024-05-28 13:33:58.000000 django-audit-events-0.3.2/django_audit_events/migrations/0004_auto_20210127_2021.py
+-rw-rw-rw-   0 root         (0) root         (0)      768 2024-05-28 13:33:58.000000 django-audit-events-0.3.2/django_audit_events/migrations/0005_auto_20220215_0756.py
+-rw-rw-rw-   0 root         (0) root         (0)      669 2024-05-28 13:33:58.000000 django-audit-events-0.3.2/django_audit_events/migrations/0006_auto_20220920_1327.py
+-rw-rw-rw-   0 root         (0) root         (0)        0 2024-05-28 13:33:58.000000 django-audit-events-0.3.2/django_audit_events/migrations/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)      857 2024-05-28 13:33:58.000000 django-audit-events-0.3.2/django_audit_events/mixin.py
+-rw-rw-rw-   0 root         (0) root         (0)     4659 2024-05-28 13:33:58.000000 django-audit-events-0.3.2/django_audit_events/models.py
+-rw-rw-rw-   0 root         (0) root         (0)      476 2024-05-28 13:33:58.000000 django-audit-events-0.3.2/django_audit_events/serializers.py
+-rw-rw-rw-   0 root         (0) root         (0)     1675 2024-05-28 13:33:58.000000 django-audit-events-0.3.2/django_audit_events/tasks.py
+drwxrwxrwx   0 root         (0) root         (0)        0 2024-05-28 13:34:24.000000 django-audit-events-0.3.2/django_audit_events/tests/
+-rw-rw-rw-   0 root         (0) root         (0)        0 2024-05-28 13:33:58.000000 django-audit-events-0.3.2/django_audit_events/tests/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)      290 2024-05-28 13:33:58.000000 django-audit-events-0.3.2/django_audit_events/tests/test_conf.py
+-rw-rw-rw-   0 root         (0) root         (0)     6001 2024-05-28 13:33:58.000000 django-audit-events-0.3.2/django_audit_events/tests/test_context.py
+-rw-rw-rw-   0 root         (0) root         (0)     1362 2024-05-28 13:33:58.000000 django-audit-events-0.3.2/django_audit_events/tests/test_middleware.py
+-rw-rw-rw-   0 root         (0) root         (0)     1539 2024-05-28 13:33:58.000000 django-audit-events-0.3.2/django_audit_events/tests/test_mixin.py
+-rw-rw-rw-   0 root         (0) root         (0)     2062 2024-05-28 13:33:58.000000 django-audit-events-0.3.2/django_audit_events/tests/test_models.py
+-rw-rw-rw-   0 root         (0) root         (0)     2548 2024-05-28 13:33:58.000000 django-audit-events-0.3.2/django_audit_events/tests/test_tasks.py
+-rw-rw-rw-   0 root         (0) root         (0)       58 2024-05-28 13:33:58.000000 django-audit-events-0.3.2/django_audit_events/tests/urls.py
+drwxrwxrwx   0 root         (0) root         (0)        0 2024-05-28 13:34:24.000000 django-audit-events-0.3.2/django_audit_events/tests/utils/
+-rw-rw-rw-   0 root         (0) root         (0)       65 2024-05-28 13:33:58.000000 django-audit-events-0.3.2/django_audit_events/tests/utils/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)      160 2024-05-28 13:33:58.000000 django-audit-events-0.3.2/django_audit_events/tests/utils/models.py
+-rw-rw-rw-   0 root         (0) root         (0)      205 2024-05-28 13:33:58.000000 django-audit-events-0.3.2/django_audit_events/urls.py
+-rw-rw-rw-   0 root         (0) root         (0)      917 2024-05-28 13:33:58.000000 django-audit-events-0.3.2/django_audit_events/utils.py
+-rw-rw-rw-   0 root         (0) root         (0)       22 2024-05-28 13:34:24.000000 django-audit-events-0.3.2/django_audit_events/version.py
+-rw-rw-rw-   0 root         (0) root         (0)     1060 2024-05-28 13:33:58.000000 django-audit-events-0.3.2/django_audit_events/views.py
+drwxrwxrwx   0 root         (0) root         (0)        0 2024-05-28 13:34:24.000000 django-audit-events-0.3.2/django_audit_events.egg-info/
+-rw-rw-rw-   0 root         (0) root         (0)     3507 2024-05-28 13:34:24.000000 django-audit-events-0.3.2/django_audit_events.egg-info/PKG-INFO
+-rw-rw-rw-   0 root         (0) root         (0)     1798 2024-05-28 13:34:24.000000 django-audit-events-0.3.2/django_audit_events.egg-info/SOURCES.txt
+-rw-rw-rw-   0 root         (0) root         (0)        1 2024-05-28 13:34:24.000000 django-audit-events-0.3.2/django_audit_events.egg-info/dependency_links.txt
+-rw-rw-rw-   0 root         (0) root         (0)        1 2024-05-28 13:34:24.000000 django-audit-events-0.3.2/django_audit_events.egg-info/not-zip-safe
+-rw-rw-rw-   0 root         (0) root         (0)       20 2024-05-28 13:34:24.000000 django-audit-events-0.3.2/django_audit_events.egg-info/top_level.txt
+drwxrwxrwx   0 root         (0) root         (0)        0 2024-05-28 13:34:24.000000 django-audit-events-0.3.2/docs/
+-rw-rw-rw-   0 root         (0) root         (0)      634 2024-05-28 13:33:58.000000 django-audit-events-0.3.2/docs/Makefile
+-rw-rw-rw-   0 root         (0) root         (0)     1609 2024-05-28 13:33:58.000000 django-audit-events-0.3.2/docs/advanced.rst
+-rw-rw-rw-   0 root         (0) root         (0)     2080 2024-05-28 13:33:58.000000 django-audit-events-0.3.2/docs/conf.py
+-rw-rw-rw-   0 root         (0) root         (0)     1533 2024-05-28 13:33:58.000000 django-audit-events-0.3.2/docs/configuration.rst
+-rw-rw-rw-   0 root         (0) root         (0)      944 2024-05-28 13:33:58.000000 django-audit-events-0.3.2/docs/index.rst
+-rw-rw-rw-   0 root         (0) root         (0)     1252 2024-05-28 13:33:58.000000 django-audit-events-0.3.2/docs/introduction.rst
+-rw-rw-rw-   0 root         (0) root         (0)      795 2024-05-28 13:33:58.000000 django-audit-events-0.3.2/docs/make.bat
+-rw-rw-rw-   0 root         (0) root         (0)     2265 2024-05-28 13:33:58.000000 django-audit-events-0.3.2/docs/quickstart.rst
+-rw-rw-rw-   0 root         (0) root         (0)      310 2024-05-28 13:33:58.000000 django-audit-events-0.3.2/pyproject.toml
+-rw-rw-rw-   0 root         (0) root         (0)      396 2024-05-28 13:33:58.000000 django-audit-events-0.3.2/requirements.txt
+-rw-rw-rw-   0 root         (0) root         (0)     2337 2024-05-28 13:33:58.000000 django-audit-events-0.3.2/runtests.py
+-rw-rw-rw-   0 root         (0) root         (0)       38 2024-05-28 13:34:24.000000 django-audit-events-0.3.2/setup.cfg
+-rw-rw-rw-   0 root         (0) root         (0)     2628 2024-05-28 13:33:58.000000 django-audit-events-0.3.2/setup.py
+-rw-rw-rw-   0 root         (0) root         (0)     1801 2024-05-28 13:33:58.000000 django-audit-events-0.3.2/tox.ini
```

### Comparing `django-audit-events-0.3.1.dev0/LICENSE.txt` & `django-audit-events-0.3.2/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `django-audit-events-0.3.1.dev0/PKG-INFO` & `django-audit-events-0.3.2/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: django-audit-events
-Version: 0.3.1.dev0
+Version: 0.3.2
 Summary: Log audit events in Django
 Home-page: https://bitbucket.org/akinonteam/django-audit-events
 Author: Onur Güzel
 Author-email: dev@akinon.com
 Maintainer: Akinon
 Maintainer-email: dev@akinon.com
 License: MIT
```

### Comparing `django-audit-events-0.3.1.dev0/README.md` & `django-audit-events-0.3.2/README.md`

 * *Files identical despite different names*

### Comparing `django-audit-events-0.3.1.dev0/bitbucket-pipelines.yml` & `django-audit-events-0.3.2/bitbucket-pipelines.yml`

 * *Files 5% similar despite different names*

```diff
@@ -58,14 +58,23 @@
           image: python:3.8-alpine
           script:
             - apk add postgresql-dev gcc git python3-dev musl-dev
             - pip install tox
             - tox -e py38-django22,py38-django30,py38-django31,py38-django32,py38-django40,py38-django41,py38-django42
           services:
             - postgres
+      - step:
+          name: py39
+          image: python:3.9-alpine
+          script:
+            - apk add postgresql-dev gcc git python3-dev musl-dev
+            - pip install tox
+            - tox -e py39-django32,py39-django40,py39-django41,py39-django42
+          services:
+            - postgres
   tags:
     '*':
       - step:
           name: Publish to PyPI
           image: python:3.7-alpine
           script:
             - apk add gcc git libffi-dev musl-dev openssl-dev python3-dev
```

### Comparing `django-audit-events-0.3.1.dev0/django_audit_events/conf.py` & `django-audit-events-0.3.2/django_audit_events/conf.py`

 * *Files identical despite different names*

### Comparing `django-audit-events-0.3.1.dev0/django_audit_events/context.py` & `django-audit-events-0.3.2/django_audit_events/context.py`

 * *Files identical despite different names*

### Comparing `django-audit-events-0.3.1.dev0/django_audit_events/filters.py` & `django-audit-events-0.3.2/django_audit_events/filters.py`

 * *Files identical despite different names*

### Comparing `django-audit-events-0.3.1.dev0/django_audit_events/locale/tr/LC_MESSAGES/django.po` & `django-audit-events-0.3.2/django_audit_events/locale/tr/LC_MESSAGES/django.po`

 * *Files identical despite different names*

### Comparing `django-audit-events-0.3.1.dev0/django_audit_events/middleware.py` & `django-audit-events-0.3.2/django_audit_events/middleware.py`

 * *Files identical despite different names*

### Comparing `django-audit-events-0.3.1.dev0/django_audit_events/migrations/0001_initial.py` & `django-audit-events-0.3.2/django_audit_events/migrations/0001_initial.py`

 * *Files identical despite different names*

### Comparing `django-audit-events-0.3.1.dev0/django_audit_events/migrations/0002_archivedauditevent.py` & `django-audit-events-0.3.2/django_audit_events/migrations/0002_archivedauditevent.py`

 * *Files identical despite different names*

### Comparing `django-audit-events-0.3.1.dev0/django_audit_events/migrations/0003_auto_20201218_1113.py` & `django-audit-events-0.3.2/django_audit_events/migrations/0003_auto_20201218_1113.py`

 * *Files identical despite different names*

### Comparing `django-audit-events-0.3.1.dev0/django_audit_events/migrations/0004_auto_20210127_2021.py` & `django-audit-events-0.3.2/django_audit_events/migrations/0004_auto_20210127_2021.py`

 * *Files identical despite different names*

### Comparing `django-audit-events-0.3.1.dev0/django_audit_events/migrations/0005_auto_20220215_0756.py` & `django-audit-events-0.3.2/django_audit_events/migrations/0005_auto_20220215_0756.py`

 * *Files identical despite different names*

### Comparing `django-audit-events-0.3.1.dev0/django_audit_events/migrations/0006_auto_20220920_1327.py` & `django-audit-events-0.3.2/django_audit_events/migrations/0006_auto_20220920_1327.py`

 * *Files identical despite different names*

### Comparing `django-audit-events-0.3.1.dev0/django_audit_events/mixin.py` & `django-audit-events-0.3.2/django_audit_events/mixin.py`

 * *Files identical despite different names*

### Comparing `django-audit-events-0.3.1.dev0/django_audit_events/models.py` & `django-audit-events-0.3.2/django_audit_events/models.py`

 * *Files identical despite different names*

### Comparing `django-audit-events-0.3.1.dev0/django_audit_events/tasks.py` & `django-audit-events-0.3.2/django_audit_events/tasks.py`

 * *Files identical despite different names*

### Comparing `django-audit-events-0.3.1.dev0/django_audit_events/tests/test_context.py` & `django-audit-events-0.3.2/django_audit_events/tests/test_context.py`

 * *Files identical despite different names*

### Comparing `django-audit-events-0.3.1.dev0/django_audit_events/tests/test_middleware.py` & `django-audit-events-0.3.2/django_audit_events/tests/test_middleware.py`

 * *Files identical despite different names*

### Comparing `django-audit-events-0.3.1.dev0/django_audit_events/tests/test_mixin.py` & `django-audit-events-0.3.2/django_audit_events/tests/test_mixin.py`

 * *Files identical despite different names*

### Comparing `django-audit-events-0.3.1.dev0/django_audit_events/tests/test_models.py` & `django-audit-events-0.3.2/django_audit_events/tests/test_models.py`

 * *Files identical despite different names*

### Comparing `django-audit-events-0.3.1.dev0/django_audit_events/tests/test_tasks.py` & `django-audit-events-0.3.2/django_audit_events/tests/test_tasks.py`

 * *Files identical despite different names*

### Comparing `django-audit-events-0.3.1.dev0/django_audit_events/utils.py` & `django-audit-events-0.3.2/django_audit_events/utils.py`

 * *Files identical despite different names*

### Comparing `django-audit-events-0.3.1.dev0/django_audit_events/views.py` & `django-audit-events-0.3.2/django_audit_events/views.py`

 * *Files identical despite different names*

### Comparing `django-audit-events-0.3.1.dev0/django_audit_events.egg-info/PKG-INFO` & `django-audit-events-0.3.2/django_audit_events.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: django-audit-events
-Version: 0.3.1.dev0
+Version: 0.3.2
 Summary: Log audit events in Django
 Home-page: https://bitbucket.org/akinonteam/django-audit-events
 Author: Onur Güzel
 Author-email: dev@akinon.com
 Maintainer: Akinon
 Maintainer-email: dev@akinon.com
 License: MIT
```

### Comparing `django-audit-events-0.3.1.dev0/django_audit_events.egg-info/SOURCES.txt` & `django-audit-events-0.3.2/django_audit_events.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `django-audit-events-0.3.1.dev0/docs/Makefile` & `django-audit-events-0.3.2/docs/Makefile`

 * *Files identical despite different names*

### Comparing `django-audit-events-0.3.1.dev0/docs/advanced.rst` & `django-audit-events-0.3.2/docs/advanced.rst`

 * *Files identical despite different names*

### Comparing `django-audit-events-0.3.1.dev0/docs/conf.py` & `django-audit-events-0.3.2/docs/conf.py`

 * *Files identical despite different names*

### Comparing `django-audit-events-0.3.1.dev0/docs/configuration.rst` & `django-audit-events-0.3.2/docs/configuration.rst`

 * *Files identical despite different names*

### Comparing `django-audit-events-0.3.1.dev0/docs/index.rst` & `django-audit-events-0.3.2/docs/index.rst`

 * *Files identical despite different names*

### Comparing `django-audit-events-0.3.1.dev0/docs/introduction.rst` & `django-audit-events-0.3.2/docs/introduction.rst`

 * *Files identical despite different names*

### Comparing `django-audit-events-0.3.1.dev0/docs/make.bat` & `django-audit-events-0.3.2/docs/make.bat`

 * *Files identical despite different names*

### Comparing `django-audit-events-0.3.1.dev0/docs/quickstart.rst` & `django-audit-events-0.3.2/docs/quickstart.rst`

 * *Files identical despite different names*

### Comparing `django-audit-events-0.3.1.dev0/runtests.py` & `django-audit-events-0.3.2/runtests.py`

 * *Files identical despite different names*

### Comparing `django-audit-events-0.3.1.dev0/setup.py` & `django-audit-events-0.3.2/setup.py`

 * *Files identical despite different names*

### Comparing `django-audit-events-0.3.1.dev0/tox.ini` & `django-audit-events-0.3.2/tox.ini`

 * *Files 1% similar despite different names*

```diff
@@ -7,15 +7,15 @@
 isolated_build = True
 skip_missing_interpreters = True
 envlist = py27-{django110,django111}
           py34-{django110,django111,django20}
           py35-{django110,django111,django20,django21,django22}
           {py36,py37}-{django111,django20,django21,django22,django30,django31}
           py38-{django22,django30,django31,django32,django40,django41,django42}
-          py39-{django22,django30,django31,django40,django41}
+          py39-{django32,django40,django41}
           py310-{django22,django30,django31,django40,django41}
           py311-{django22,django30,django31,django40,django41}
           linting
 
 [testenv]
 deps = celery>=4.3.0,<=5.2.7
        django110: Django>=1.10,<1.11.1
```

