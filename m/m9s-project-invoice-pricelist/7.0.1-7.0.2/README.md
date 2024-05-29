# Comparing `tmp/m9s_project_invoice_pricelist-7.0.1.tar.gz` & `tmp/m9s_project_invoice_pricelist-7.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "m9s_project_invoice_pricelist-7.0.1.tar", last modified: Sat Mar 16 11:18:24 2024, max compression
+gzip compressed data, was "m9s_project_invoice_pricelist-7.0.2.tar", last modified: Wed May 29 16:04:01 2024, max compression
```

## Comparing `m9s_project_invoice_pricelist-7.0.1.tar` & `m9s_project_invoice_pricelist-7.0.2.tar`

### file list

```diff
@@ -1,46 +1,46 @@
-drwxr-xr-x   0 mathiasb  (1000) mathiasb  (1000)        0 2024-03-16 11:18:24.037492 m9s_project_invoice_pricelist-7.0.1/
--rw-r--r--   0 mathiasb  (1000) mathiasb  (1000)       95 2023-12-21 15:13:58.000000 m9s_project_invoice_pricelist-7.0.1/.coveragerc
--rw-r--r--   0 mathiasb  (1000) mathiasb  (1000)     1875 2022-02-13 19:23:18.000000 m9s_project_invoice_pricelist-7.0.1/.drone.yml
--rw-r--r--   0 mathiasb  (1000) mathiasb  (1000)       46 2023-12-21 15:13:58.000000 m9s_project_invoice_pricelist-7.0.1/.flake8
--rw-r--r--   0 mathiasb  (1000) mathiasb  (1000)       92 2023-12-21 15:13:58.000000 m9s_project_invoice_pricelist-7.0.1/.gitlab-ci-m9s.yml
--rw-r--r--   0 mathiasb  (1000) mathiasb  (1000)     1892 2023-12-21 15:13:58.000000 m9s_project_invoice_pricelist-7.0.1/.gitlab-ci.yml
--rw-r--r--   0 mathiasb  (1000) mathiasb  (1000)      173 2023-12-21 15:13:58.000000 m9s_project_invoice_pricelist-7.0.1/.isort.cfg
-drwxr-xr-x   0 mathiasb  (1000) mathiasb  (1000)        0 2024-03-16 11:18:24.037492 m9s_project_invoice_pricelist-7.0.1/.woodpecker/
--rwxrwxr-x   0 mathiasb  (1000) mathiasb  (1000)     1367 2023-12-21 15:13:58.000000 m9s_project_invoice_pricelist-7.0.1/.woodpecker/mail_curl.sh
--rw-r--r--   0 mathiasb  (1000) mathiasb  (1000)      645 2023-12-21 15:13:58.000000 m9s_project_invoice_pricelist-7.0.1/.woodpecker/report.yml
--rw-r--r--   0 mathiasb  (1000) mathiasb  (1000)     1302 2023-12-21 15:13:58.000000 m9s_project_invoice_pricelist-7.0.1/.woodpecker/test.yml
--rw-r--r--   0 mathiasb  (1000) mathiasb  (1000)      690 2023-12-21 15:13:58.000000 m9s_project_invoice_pricelist-7.0.1/COPYRIGHT
--rw-r--r--   0 mathiasb  (1000) mathiasb  (1000)      700 2023-12-21 15:13:58.000000 m9s_project_invoice_pricelist-7.0.1/INSTALL
--rw-r--r--   0 mathiasb  (1000) mathiasb  (1000)    35147 2023-12-21 15:13:58.000000 m9s_project_invoice_pricelist-7.0.1/LICENSE
--rw-r--r--   0 mathiasb  (1000) mathiasb  (1000)      121 2023-12-21 15:13:58.000000 m9s_project_invoice_pricelist-7.0.1/MANIFEST.in
--rw-r--r--   0 mathiasb  (1000) mathiasb  (1000)     3540 2024-03-16 11:18:24.037492 m9s_project_invoice_pricelist-7.0.1/PKG-INFO
--rw-r--r--   0 mathiasb  (1000) mathiasb  (1000)     1322 2023-12-21 15:13:58.000000 m9s_project_invoice_pricelist-7.0.1/README.md
--rw-r--r--   0 mathiasb  (1000) mathiasb  (1000)       66 2023-12-21 15:13:58.000000 m9s_project_invoice_pricelist-7.0.1/README.rst
--rw-r--r--   0 mathiasb  (1000) mathiasb  (1000)      303 2023-12-21 15:13:58.000000 m9s_project_invoice_pricelist-7.0.1/__init__.py
--rw-r--r--   0 mathiasb  (1000) mathiasb  (1000)       92 2023-12-21 15:13:58.000000 m9s_project_invoice_pricelist-7.0.1/dev_requirements.txt
-drwxr-xr-x   0 mathiasb  (1000) mathiasb  (1000)        0 2024-03-16 11:18:24.037492 m9s_project_invoice_pricelist-7.0.1/doc/
-drwxr-xr-x   0 mathiasb  (1000) mathiasb  (1000)        0 2024-03-16 11:18:24.037492 m9s_project_invoice_pricelist-7.0.1/doc/de/
--rw-r--r--   0 mathiasb  (1000) mathiasb  (1000)       65 2023-12-21 15:13:58.000000 m9s_project_invoice_pricelist-7.0.1/doc/de/index.rst
--rw-r--r--   0 mathiasb  (1000) mathiasb  (1000)       66 2023-12-21 15:13:58.000000 m9s_project_invoice_pricelist-7.0.1/doc/index.rst
-drwxr-xr-x   0 mathiasb  (1000) mathiasb  (1000)        0 2024-03-16 11:18:24.033492 m9s_project_invoice_pricelist-7.0.1/locale/
--rw-r--r--   0 mathiasb  (1000) mathiasb  (1000)      610 2022-11-10 15:09:53.000000 m9s_project_invoice_pricelist-7.0.1/locale/de.po
-drwxr-xr-x   0 mathiasb  (1000) mathiasb  (1000)        0 2024-03-16 11:18:24.037492 m9s_project_invoice_pricelist-7.0.1/m9s_project_invoice_pricelist.egg-info/
--rw-r--r--   0 mathiasb  (1000) mathiasb  (1000)     3540 2024-03-16 11:18:23.000000 m9s_project_invoice_pricelist-7.0.1/m9s_project_invoice_pricelist.egg-info/PKG-INFO
--rw-r--r--   0 mathiasb  (1000) mathiasb  (1000)      899 2024-03-16 11:18:23.000000 m9s_project_invoice_pricelist-7.0.1/m9s_project_invoice_pricelist.egg-info/SOURCES.txt
--rw-r--r--   0 mathiasb  (1000) mathiasb  (1000)        1 2024-03-16 11:18:23.000000 m9s_project_invoice_pricelist-7.0.1/m9s_project_invoice_pricelist.egg-info/dependency_links.txt
--rw-r--r--   0 mathiasb  (1000) mathiasb  (1000)       88 2024-03-16 11:18:23.000000 m9s_project_invoice_pricelist-7.0.1/m9s_project_invoice_pricelist.egg-info/entry_points.txt
--rw-r--r--   0 mathiasb  (1000) mathiasb  (1000)        1 2021-04-04 19:01:02.000000 m9s_project_invoice_pricelist-7.0.1/m9s_project_invoice_pricelist.egg-info/not-zip-safe
--rw-r--r--   0 mathiasb  (1000) mathiasb  (1000)       98 2024-03-16 11:18:23.000000 m9s_project_invoice_pricelist-7.0.1/m9s_project_invoice_pricelist.egg-info/requires.txt
--rw-r--r--   0 mathiasb  (1000) mathiasb  (1000)        8 2024-03-16 11:18:23.000000 m9s_project_invoice_pricelist-7.0.1/m9s_project_invoice_pricelist.egg-info/top_level.txt
--rw-r--r--   0 mathiasb  (1000) mathiasb  (1000)      106 2023-12-21 15:13:58.000000 m9s_project_invoice_pricelist-7.0.1/requirements.txt
--rw-r--r--   0 mathiasb  (1000) mathiasb  (1000)       38 2024-03-16 11:18:24.037492 m9s_project_invoice_pricelist-7.0.1/setup.cfg
--rwxr-xr-x   0 mathiasb  (1000) mathiasb  (1000)     4504 2023-12-21 15:13:58.000000 m9s_project_invoice_pricelist-7.0.1/setup.py
-drwxr-xr-x   0 mathiasb  (1000) mathiasb  (1000)        0 2024-03-16 11:18:24.037492 m9s_project_invoice_pricelist-7.0.1/tests/
--rw-r--r--   0 mathiasb  (1000) mathiasb  (1000)      115 2023-12-21 15:13:58.000000 m9s_project_invoice_pricelist-7.0.1/tests/__init__.py
--rw-r--r--   0 mathiasb  (1000) mathiasb  (1000)      331 2023-12-21 15:13:58.000000 m9s_project_invoice_pricelist-7.0.1/tests/test_module.py
--rw-r--r--   0 mathiasb  (1000) mathiasb  (1000)      595 2023-12-21 15:13:58.000000 m9s_project_invoice_pricelist-7.0.1/tox.ini
--rw-r--r--   0 mathiasb  (1000) mathiasb  (1000)      131 2024-01-21 12:01:53.000000 m9s_project_invoice_pricelist-7.0.1/tryton.cfg
-drwxr-xr-x   0 mathiasb  (1000) mathiasb  (1000)        0 2024-03-16 11:18:24.037492 m9s_project_invoice_pricelist-7.0.1/view/
--rw-r--r--   0 mathiasb  (1000) mathiasb  (1000)      429 2022-11-10 15:09:53.000000 m9s_project_invoice_pricelist-7.0.1/view/work_form.xml
--rw-r--r--   0 mathiasb  (1000) mathiasb  (1000)     3200 2024-03-16 11:18:17.000000 m9s_project_invoice_pricelist-7.0.1/work.py
--rw-r--r--   0 mathiasb  (1000) mathiasb  (1000)      424 2020-10-02 08:16:00.000000 m9s_project_invoice_pricelist-7.0.1/work.xml
+drwxrwxr-x   0 mathiasb  (1000) mathiasb  (1000)        0 2024-05-29 16:04:01.266717 m9s_project_invoice_pricelist-7.0.2/
+-rw-r--r--   0 mathiasb  (1000) mathiasb  (1000)       95 2024-04-25 09:53:46.000000 m9s_project_invoice_pricelist-7.0.2/.coveragerc
+-rw-r--r--   0 mathiasb  (1000) mathiasb  (1000)     1875 2022-02-13 19:23:18.000000 m9s_project_invoice_pricelist-7.0.2/.drone.yml
+-rw-r--r--   0 mathiasb  (1000) mathiasb  (1000)       46 2024-04-25 09:53:46.000000 m9s_project_invoice_pricelist-7.0.2/.flake8
+-rw-r--r--   0 mathiasb  (1000) mathiasb  (1000)       92 2024-04-25 09:53:46.000000 m9s_project_invoice_pricelist-7.0.2/.gitlab-ci-m9s.yml
+-rw-r--r--   0 mathiasb  (1000) mathiasb  (1000)     2204 2024-04-25 09:53:46.000000 m9s_project_invoice_pricelist-7.0.2/.gitlab-ci.yml
+-rw-r--r--   0 mathiasb  (1000) mathiasb  (1000)      173 2024-04-25 09:53:46.000000 m9s_project_invoice_pricelist-7.0.2/.isort.cfg
+drwxrwxr-x   0 mathiasb  (1000) mathiasb  (1000)        0 2024-05-29 16:04:01.266717 m9s_project_invoice_pricelist-7.0.2/.woodpecker/
+-rwxrwxr-x   0 mathiasb  (1000) mathiasb  (1000)     1367 2024-04-25 09:53:46.000000 m9s_project_invoice_pricelist-7.0.2/.woodpecker/mail_curl.sh
+-rw-r--r--   0 mathiasb  (1000) mathiasb  (1000)      645 2024-04-25 09:53:46.000000 m9s_project_invoice_pricelist-7.0.2/.woodpecker/report.yml
+-rw-r--r--   0 mathiasb  (1000) mathiasb  (1000)     1302 2024-04-25 09:53:46.000000 m9s_project_invoice_pricelist-7.0.2/.woodpecker/test.yml
+-rw-rw-r--   0 mathiasb  (1000) mathiasb  (1000)      690 2024-04-25 09:53:46.000000 m9s_project_invoice_pricelist-7.0.2/COPYRIGHT
+-rw-r--r--   0 mathiasb  (1000) mathiasb  (1000)      700 2024-04-25 09:53:46.000000 m9s_project_invoice_pricelist-7.0.2/INSTALL
+-rw-r--r--   0 mathiasb  (1000) mathiasb  (1000)    35147 2024-04-25 09:53:46.000000 m9s_project_invoice_pricelist-7.0.2/LICENSE
+-rw-r--r--   0 mathiasb  (1000) mathiasb  (1000)      121 2024-04-25 09:53:46.000000 m9s_project_invoice_pricelist-7.0.2/MANIFEST.in
+-rw-rw-r--   0 mathiasb  (1000) mathiasb  (1000)     3330 2024-05-29 16:04:01.266717 m9s_project_invoice_pricelist-7.0.2/PKG-INFO
+-rw-r--r--   0 mathiasb  (1000) mathiasb  (1000)     1112 2024-04-25 09:53:46.000000 m9s_project_invoice_pricelist-7.0.2/README.md
+-rw-r--r--   0 mathiasb  (1000) mathiasb  (1000)       66 2024-04-25 09:53:46.000000 m9s_project_invoice_pricelist-7.0.2/README.rst
+-rw-rw-r--   0 mathiasb  (1000) mathiasb  (1000)      303 2024-04-25 09:53:46.000000 m9s_project_invoice_pricelist-7.0.2/__init__.py
+-rw-r--r--   0 mathiasb  (1000) mathiasb  (1000)       86 2024-04-25 09:53:46.000000 m9s_project_invoice_pricelist-7.0.2/dev_requirements.txt
+drwxrwxr-x   0 mathiasb  (1000) mathiasb  (1000)        0 2024-05-29 16:04:01.266717 m9s_project_invoice_pricelist-7.0.2/doc/
+drwxrwxr-x   0 mathiasb  (1000) mathiasb  (1000)        0 2024-05-29 16:04:01.266717 m9s_project_invoice_pricelist-7.0.2/doc/de/
+-rw-r--r--   0 mathiasb  (1000) mathiasb  (1000)       65 2024-04-25 09:53:46.000000 m9s_project_invoice_pricelist-7.0.2/doc/de/index.rst
+-rw-r--r--   0 mathiasb  (1000) mathiasb  (1000)       66 2024-04-25 09:53:46.000000 m9s_project_invoice_pricelist-7.0.2/doc/index.rst
+drwxrwxr-x   0 mathiasb  (1000) mathiasb  (1000)        0 2024-05-29 16:04:01.266717 m9s_project_invoice_pricelist-7.0.2/locale/
+-rw-rw-r--   0 mathiasb  (1000) mathiasb  (1000)      691 2024-05-29 16:03:48.000000 m9s_project_invoice_pricelist-7.0.2/locale/de.po
+drwxrwxr-x   0 mathiasb  (1000) mathiasb  (1000)        0 2024-05-29 16:04:01.266717 m9s_project_invoice_pricelist-7.0.2/m9s_project_invoice_pricelist.egg-info/
+-rw-r--r--   0 mathiasb  (1000) mathiasb  (1000)     3330 2024-05-29 16:04:00.000000 m9s_project_invoice_pricelist-7.0.2/m9s_project_invoice_pricelist.egg-info/PKG-INFO
+-rw-r--r--   0 mathiasb  (1000) mathiasb  (1000)      899 2024-05-29 16:04:01.000000 m9s_project_invoice_pricelist-7.0.2/m9s_project_invoice_pricelist.egg-info/SOURCES.txt
+-rw-r--r--   0 mathiasb  (1000) mathiasb  (1000)        1 2024-05-29 16:04:00.000000 m9s_project_invoice_pricelist-7.0.2/m9s_project_invoice_pricelist.egg-info/dependency_links.txt
+-rw-r--r--   0 mathiasb  (1000) mathiasb  (1000)       88 2024-05-29 16:04:00.000000 m9s_project_invoice_pricelist-7.0.2/m9s_project_invoice_pricelist.egg-info/entry_points.txt
+-rw-r--r--   0 mathiasb  (1000) mathiasb  (1000)        1 2021-04-04 19:01:02.000000 m9s_project_invoice_pricelist-7.0.2/m9s_project_invoice_pricelist.egg-info/not-zip-safe
+-rw-r--r--   0 mathiasb  (1000) mathiasb  (1000)       98 2024-05-29 16:04:00.000000 m9s_project_invoice_pricelist-7.0.2/m9s_project_invoice_pricelist.egg-info/requires.txt
+-rw-r--r--   0 mathiasb  (1000) mathiasb  (1000)        8 2024-05-29 16:04:00.000000 m9s_project_invoice_pricelist-7.0.2/m9s_project_invoice_pricelist.egg-info/top_level.txt
+-rw-r--r--   0 mathiasb  (1000) mathiasb  (1000)      106 2024-04-25 09:53:46.000000 m9s_project_invoice_pricelist-7.0.2/requirements.txt
+-rw-rw-r--   0 mathiasb  (1000) mathiasb  (1000)       38 2024-05-29 16:04:01.266717 m9s_project_invoice_pricelist-7.0.2/setup.cfg
+-rwxr-xr-x   0 mathiasb  (1000) mathiasb  (1000)     4504 2024-04-25 09:53:46.000000 m9s_project_invoice_pricelist-7.0.2/setup.py
+drwxrwxr-x   0 mathiasb  (1000) mathiasb  (1000)        0 2024-05-29 16:04:01.266717 m9s_project_invoice_pricelist-7.0.2/tests/
+-rw-r--r--   0 mathiasb  (1000) mathiasb  (1000)      115 2024-04-25 09:53:46.000000 m9s_project_invoice_pricelist-7.0.2/tests/__init__.py
+-rw-r--r--   0 mathiasb  (1000) mathiasb  (1000)      331 2024-04-25 09:53:46.000000 m9s_project_invoice_pricelist-7.0.2/tests/test_module.py
+-rw-r--r--   0 mathiasb  (1000) mathiasb  (1000)      595 2024-04-25 09:53:46.000000 m9s_project_invoice_pricelist-7.0.2/tox.ini
+-rw-rw-r--   0 mathiasb  (1000) mathiasb  (1000)      131 2024-04-25 09:53:46.000000 m9s_project_invoice_pricelist-7.0.2/tryton.cfg
+drwxrwxr-x   0 mathiasb  (1000) mathiasb  (1000)        0 2024-05-29 16:04:01.266717 m9s_project_invoice_pricelist-7.0.2/view/
+-rw-r--r--   0 mathiasb  (1000) mathiasb  (1000)      429 2022-11-10 15:09:53.000000 m9s_project_invoice_pricelist-7.0.2/view/work_form.xml
+-rw-rw-r--   0 mathiasb  (1000) mathiasb  (1000)     3573 2024-05-29 16:03:48.000000 m9s_project_invoice_pricelist-7.0.2/work.py
+-rw-r--r--   0 mathiasb  (1000) mathiasb  (1000)      424 2020-10-02 08:16:00.000000 m9s_project_invoice_pricelist-7.0.2/work.xml
```

### Comparing `m9s_project_invoice_pricelist-7.0.1/.drone.yml` & `m9s_project_invoice_pricelist-7.0.2/.drone.yml`

 * *Files identical despite different names*

### Comparing `m9s_project_invoice_pricelist-7.0.1/.gitlab-ci.yml` & `m9s_project_invoice_pricelist-7.0.2/.gitlab-ci.yml`

 * *Files 14% similar despite different names*

```diff
@@ -47,37 +47,43 @@
     - tox -e py311-postgresql -vv -- -v
   tags:
     - postgres
 
 test-sqlite:
   <<: *test_base
   script:
-    - tox -e py311-sqlite -vv -- -v
+    - tox -e py311-sqlite -vv -- -v --output-file junit.xml
+    - coverage xml
     - coverage html
     - coverage report -m
-    # 20131213: coverage-badge not Python 3.12 ready
-    - coverage-badge
-
-  coverage: '/TOTAL.+ ([0-9]{1,3}%)/'
-      
+    - genbadge tests -i - < junit.xml -o reports/junit/junit-badge.svg
+    - genbadge coverage -i - < coverage.xml -o reports/coverage/coverage-badge.svg
+  coverage: '/(?i)total.*? (100(?:\.0+)?\%|[1-9]?\d(?:\.\d+)?\%)$/'
   artifacts:
     when: always
+    reports:
+      junit: junit.xml
+      coverage_report:
+        coverage_format: cobertura
+        path: coverage.xml
     paths:
       - htmlcov
+      - reports
     expire_in: 30 days
 
 pages:
   stage: pages
   #dependencies:
   #   - test-sqlite
   script:
     # delete everything in the current public folder
     # and replace with code coverage HTML report
     - mkdir -p public
     - rm -rf public/*
     - cp -r htmlcov/* public/
+    - cp -r reports/* public/
   artifacts:
     paths:
       - public
     expire_in: 30 days
   only:
     - develop
```

### Comparing `m9s_project_invoice_pricelist-7.0.1/.woodpecker/mail_curl.sh` & `m9s_project_invoice_pricelist-7.0.2/.woodpecker/mail_curl.sh`

 * *Files identical despite different names*

### Comparing `m9s_project_invoice_pricelist-7.0.1/.woodpecker/report.yml` & `m9s_project_invoice_pricelist-7.0.2/.woodpecker/report.yml`

 * *Files identical despite different names*

### Comparing `m9s_project_invoice_pricelist-7.0.1/.woodpecker/test.yml` & `m9s_project_invoice_pricelist-7.0.2/.woodpecker/test.yml`

 * *Files identical despite different names*

### Comparing `m9s_project_invoice_pricelist-7.0.1/COPYRIGHT` & `m9s_project_invoice_pricelist-7.0.2/COPYRIGHT`

 * *Files identical despite different names*

### Comparing `m9s_project_invoice_pricelist-7.0.1/INSTALL` & `m9s_project_invoice_pricelist-7.0.2/INSTALL`

 * *Files identical despite different names*

### Comparing `m9s_project_invoice_pricelist-7.0.1/LICENSE` & `m9s_project_invoice_pricelist-7.0.2/LICENSE`

 * *Files identical despite different names*

### Comparing `m9s_project_invoice_pricelist-7.0.1/PKG-INFO` & `m9s_project_invoice_pricelist-7.0.2/m9s_project_invoice_pricelist.egg-info/PKG-INFO`

 * *Files 17% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
-Name: m9s_project_invoice_pricelist
-Version: 7.0.1
+Name: m9s-project-invoice-pricelist
+Version: 7.0.2
 Summary: Tryton Project Invoice Pricelist Module
 Home-page: https://www.m9s.biz/
 Download-URL: https://gitlab.com/m9s/project_invoice_pricelist.git
 Author: MBSolutions
 Author-email: info@m9s.biz
 License: GPL-3
 Project-URL: Bug Tracker, https://support.m9s.biz/
@@ -47,25 +47,17 @@
 Classifier: Programming Language :: Python :: Implementation :: CPython
 Classifier: Topic :: Office/Business
 Requires-Python: >=3.8
 Description-Content-Type: text/markdown
 Provides-Extra: test
 License-File: LICENSE
 
-Master
-
-[![Pipeline status](https://gitlab.com/m9s/project_invoice_pricelist/badges/master/pipeline.svg)](https://gitlab.com/m9s/project_invoice_pricelist/commits/master)
-
-Develop
-
-[![Pipeline status](https://gitlab.com/m9s/project_invoice_pricelist/badges/develop/pipeline.svg)](https://gitlab.com/m9s/project_invoice_pricelist/commits/develop)
-
-[![Coverage report](https://gitlab.com/m9s/project_invoice_pricelist/badges/develop/coverage.svg)](http://m9s.gitlab.io/project_invoice_pricelist)
-
+[![Tests Status](https://m9s.gitlab.io/project_invoice_pricelist/junit/junit-badge.svg)](https://m9s.gitlab.io/project_invoice_pricelist)
 
+[![Coverage Status](https://m9s.gitlab.io/project_invoice_pricelist/coverage/coverage-badge.svg)](https://m9s.gitlab.io/project_invoice_pricelist)
 
 This module runs with the Tryton application platform.
 
 Installing
 ----------
 
 See INSTALL
```

### Comparing `m9s_project_invoice_pricelist-7.0.1/README.md` & `m9s_project_invoice_pricelist-7.0.2/README.md`

 * *Files 22% similar despite different names*

```diff
@@ -1,18 +1,10 @@
-Master
-
-[![Pipeline status](https://gitlab.com/m9s/project_invoice_pricelist/badges/master/pipeline.svg)](https://gitlab.com/m9s/project_invoice_pricelist/commits/master)
-
-Develop
-
-[![Pipeline status](https://gitlab.com/m9s/project_invoice_pricelist/badges/develop/pipeline.svg)](https://gitlab.com/m9s/project_invoice_pricelist/commits/develop)
-
-[![Coverage report](https://gitlab.com/m9s/project_invoice_pricelist/badges/develop/coverage.svg)](http://m9s.gitlab.io/project_invoice_pricelist)
-
+[![Tests Status](https://m9s.gitlab.io/project_invoice_pricelist/junit/junit-badge.svg)](https://m9s.gitlab.io/project_invoice_pricelist)
 
+[![Coverage Status](https://m9s.gitlab.io/project_invoice_pricelist/coverage/coverage-badge.svg)](https://m9s.gitlab.io/project_invoice_pricelist)
 
 This module runs with the Tryton application platform.
 
 Installing
 ----------
 
 See INSTALL
```

### Comparing `m9s_project_invoice_pricelist-7.0.1/locale/de.po` & `m9s_project_invoice_pricelist-7.0.2/locale/de.po`

 * *Files 23% similar despite different names*

```diff
@@ -12,14 +12,16 @@
 
 msgctxt "help:project.work,price_list:"
 msgid ""
 "Use the first pricelist found in following precedence:\n"
 "\n"
 "- Pricelist of the task\n"
 "- Pricelist of the parent project\n"
-"- Pricelist of the party"
+"- Pricelist of the party\n"
+"- Pricelist of sale configuration"
 msgstr ""
 "Preislisten kommen in folgender Reihenfolge zum Zuge:\n"
 "\n"
 "- Preisliste der Aufgabe\n"
 "- Preisliste des Projekts\n"
-"- Preisliste der Partei"
+"- Preisliste der Partei\n"
+"- Preisliste aus Einstellungen Verkauf"
```

### Comparing `m9s_project_invoice_pricelist-7.0.1/m9s_project_invoice_pricelist.egg-info/PKG-INFO` & `m9s_project_invoice_pricelist-7.0.2/PKG-INFO`

 * *Files 20% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
-Name: m9s-project-invoice-pricelist
-Version: 7.0.1
+Name: m9s_project_invoice_pricelist
+Version: 7.0.2
 Summary: Tryton Project Invoice Pricelist Module
 Home-page: https://www.m9s.biz/
 Download-URL: https://gitlab.com/m9s/project_invoice_pricelist.git
 Author: MBSolutions
 Author-email: info@m9s.biz
 License: GPL-3
 Project-URL: Bug Tracker, https://support.m9s.biz/
@@ -47,25 +47,17 @@
 Classifier: Programming Language :: Python :: Implementation :: CPython
 Classifier: Topic :: Office/Business
 Requires-Python: >=3.8
 Description-Content-Type: text/markdown
 Provides-Extra: test
 License-File: LICENSE
 
-Master
-
-[![Pipeline status](https://gitlab.com/m9s/project_invoice_pricelist/badges/master/pipeline.svg)](https://gitlab.com/m9s/project_invoice_pricelist/commits/master)
-
-Develop
-
-[![Pipeline status](https://gitlab.com/m9s/project_invoice_pricelist/badges/develop/pipeline.svg)](https://gitlab.com/m9s/project_invoice_pricelist/commits/develop)
-
-[![Coverage report](https://gitlab.com/m9s/project_invoice_pricelist/badges/develop/coverage.svg)](http://m9s.gitlab.io/project_invoice_pricelist)
-
+[![Tests Status](https://m9s.gitlab.io/project_invoice_pricelist/junit/junit-badge.svg)](https://m9s.gitlab.io/project_invoice_pricelist)
 
+[![Coverage Status](https://m9s.gitlab.io/project_invoice_pricelist/coverage/coverage-badge.svg)](https://m9s.gitlab.io/project_invoice_pricelist)
 
 This module runs with the Tryton application platform.
 
 Installing
 ----------
 
 See INSTALL
```

### Comparing `m9s_project_invoice_pricelist-7.0.1/m9s_project_invoice_pricelist.egg-info/SOURCES.txt` & `m9s_project_invoice_pricelist-7.0.2/m9s_project_invoice_pricelist.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `m9s_project_invoice_pricelist-7.0.1/setup.py` & `m9s_project_invoice_pricelist-7.0.2/setup.py`

 * *Files identical despite different names*

### Comparing `m9s_project_invoice_pricelist-7.0.1/tox.ini` & `m9s_project_invoice_pricelist-7.0.2/tox.ini`

 * *Files identical despite different names*

### Comparing `m9s_project_invoice_pricelist-7.0.1/work.py` & `m9s_project_invoice_pricelist-7.0.2/work.py`

 * *Files 4% similar despite different names*

```diff
@@ -9,34 +9,43 @@
 class Work(metaclass=PoolMeta):
     __name__ = 'project.work'
     price_list = fields.Many2One('product.price_list', 'Price List',
         domain=[('company', '=', Eval('company'))],
         help='Use the first pricelist found in following precedence:\n\n'
         '- Pricelist of the task\n'
         '- Pricelist of the parent project\n'
-        '- Pricelist of the party')
+        '- Pricelist of the party\n'
+        '- Pricelist of sale configuration')
     price_list_used = fields.Function(fields.Many2One('product.price_list',
             'Price List Used'), 'on_change_with_price_list_used')
 
     @fields.depends('price_list', 'parent', '_parent_parent.parent', 'party')
     def on_change_with_price_list_used(self, name=None):
+        pool = Pool()
+        Configuration = pool.get('sale.configuration')
         if self.price_list:
             return self.price_list.id
         parent_project = self.__class__.search([
                 ('parent', 'parent_of', [self.id]),
                 ('parent', '=', None),
                 ])
         if parent_project:
             project = parent_project[0]
             if project.price_list:
                 return project.price_list.id
             elif project.party and project.party.sale_price_list:
                 return project.party.sale_price_list.id
         elif self.party and self.party.sale_price_list:
             return self.party.sale_price_list.id
+        else:
+            config = Configuration(1)
+            price_list = config.get_multivalue(
+                'sale_price_list',
+                company=self.company.id if self.company else None)
+            return price_list and price_list.id
 
     @fields.depends('party')
     def on_change_party(self):
         self.price_list = None
         if self.party and self.party.sale_price_list:
             self.price_list = self.party.sale_price_list
```

