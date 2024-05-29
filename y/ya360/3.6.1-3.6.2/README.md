# Comparing `tmp/ya360-3.6.1.tar.gz` & `tmp/ya360-3.6.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ya360-3.6.1.tar", last modified: Thu May  2 10:25:36 2024, max compression
+gzip compressed data, was "ya360-3.6.2.tar", last modified: Wed May 29 10:11:20 2024, max compression
```

## Comparing `ya360-3.6.1.tar` & `ya360-3.6.2.tar`

### file list

```diff
@@ -1,63 +1,62 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-02 10:25:36.218502 ya360-3.6.1/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-02 10:25:36.210502 ya360-3.6.1/.github/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-02 10:25:36.210502 ya360-3.6.1/.github/ISSUE_TEMPLATE/
--rw-r--r--   0 runner    (1001) docker     (127)      535 2024-05-02 10:25:31.000000 ya360-3.6.1/.github/ISSUE_TEMPLATE/bug_report.md
--rw-r--r--   0 runner    (1001) docker     (127)      595 2024-05-02 10:25:31.000000 ya360-3.6.1/.github/ISSUE_TEMPLATE/feature_request.md
--rw-r--r--   0 runner    (1001) docker     (127)      502 2024-05-02 10:25:31.000000 ya360-3.6.1/.github/dependabot.yml
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-02 10:25:36.210502 ya360-3.6.1/.github/workflows/
--rw-r--r--   0 runner    (1001) docker     (127)     2740 2024-05-02 10:25:31.000000 ya360-3.6.1/.github/workflows/codeql-analysis.yml
--rw-r--r--   0 runner    (1001) docker     (127)     1091 2024-05-02 10:25:31.000000 ya360-3.6.1/.github/workflows/python-publish.yml
--rw-r--r--   0 runner    (1001) docker     (127)     1900 2024-05-02 10:25:31.000000 ya360-3.6.1/.gitignore
--rw-r--r--   0 runner    (1001) docker     (127)      730 2024-05-02 10:25:31.000000 ya360-3.6.1/.readthedocs.yaml
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-02 10:25:36.210502 ya360-3.6.1/.vscode/
--rw-r--r--   0 runner    (1001) docker     (127)       53 2024-05-02 10:25:31.000000 ya360-3.6.1/.vscode/settings.json
--rw-r--r--   0 runner    (1001) docker     (127)     5208 2024-05-02 10:25:31.000000 ya360-3.6.1/CODE_OF_CONDUCT.md
--rw-r--r--   0 runner    (1001) docker     (127)     1069 2024-05-02 10:25:31.000000 ya360-3.6.1/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)       18 2024-05-02 10:25:31.000000 ya360-3.6.1/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (127)     2255 2024-05-02 10:25:36.218502 ya360-3.6.1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     1374 2024-05-02 10:25:31.000000 ya360-3.6.1/README.md
--rw-r--r--   0 runner    (1001) docker     (127)     1462 2024-05-02 10:25:31.000000 ya360-3.6.1/README.rst
--rw-r--r--   0 runner    (1001) docker     (127)      175 2024-05-02 10:25:31.000000 ya360-3.6.1/SECURITY.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-02 10:25:36.210502 ya360-3.6.1/docs/
--rw-r--r--   0 runner    (1001) docker     (127)      638 2024-05-02 10:25:31.000000 ya360-3.6.1/docs/Makefile
--rw-r--r--   0 runner    (1001) docker     (127)      804 2024-05-02 10:25:31.000000 ya360-3.6.1/docs/make.bat
--rw-r--r--   0 runner    (1001) docker     (127)       82 2024-05-02 10:25:31.000000 ya360-3.6.1/docs/requirements.txt
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-02 10:25:36.210502 ya360-3.6.1/docs/source/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-02 10:25:36.214502 ya360-3.6.1/docs/source/_static/
--rw-r--r--   0 runner    (1001) docker     (127)    38353 2024-05-02 10:25:31.000000 ya360-3.6.1/docs/source/_static/fig1.png
--rw-r--r--   0 runner    (1001) docker     (127)   127538 2024-05-02 10:25:31.000000 ya360-3.6.1/docs/source/_static/fig2.png
--rw-r--r--   0 runner    (1001) docker     (127)    36447 2024-05-02 10:25:31.000000 ya360-3.6.1/docs/source/_static/fig3.png
--rw-r--r--   0 runner    (1001) docker     (127)      116 2024-05-02 10:25:31.000000 ya360-3.6.1/docs/source/_static/robots.txt
--rw-r--r--   0 runner    (1001) docker     (127)      859 2024-05-02 10:25:31.000000 ya360-3.6.1/docs/source/befo.rst
--rw-r--r--   0 runner    (1001) docker     (127)     1134 2024-05-02 10:25:31.000000 ya360-3.6.1/docs/source/cmd.rst
--rw-r--r--   0 runner    (1001) docker     (127)     2583 2024-05-02 10:25:31.000000 ya360-3.6.1/docs/source/conf.py
--rw-r--r--   0 runner    (1001) docker     (127)     1057 2024-05-02 10:25:31.000000 ya360-3.6.1/docs/source/index.rst
--rw-r--r--   0 runner    (1001) docker     (127)     1080 2024-05-02 10:25:31.000000 ya360-3.6.1/docs/source/lic.rst
--rw-r--r--   0 runner    (1001) docker     (127)      413 2024-05-02 10:25:31.000000 ya360-3.6.1/docs/source/routing.rst
--rw-r--r--   0 runner    (1001) docker     (127)     7235 2024-05-02 10:25:31.000000 ya360-3.6.1/docs/source/usage.rst
--rw-r--r--   0 runner    (1001) docker     (127)     1160 2024-05-02 10:25:31.000000 ya360-3.6.1/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-02 10:25:36.218502 ya360-3.6.1/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)      115 2024-05-02 10:25:31.000000 ya360-3.6.1/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-02 10:25:36.214502 ya360-3.6.1/ya360/
--rw-r--r--   0 runner    (1001) docker     (127)      199 2024-05-02 10:25:31.000000 ya360-3.6.1/ya360/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      182 2024-05-02 10:25:31.000000 ya360-3.6.1/ya360/__main__.py
--rw-r--r--   0 runner    (1001) docker     (127)      411 2024-05-02 10:25:36.000000 ya360-3.6.1/ya360/_version.py
--rw-r--r--   0 runner    (1001) docker     (127)     1764 2024-05-02 10:25:31.000000 ya360-3.6.1/ya360/antispam.py
--rw-r--r--   0 runner    (1001) docker     (127)    31096 2024-05-02 10:25:31.000000 ya360-3.6.1/ya360/cmd.py
--rw-r--r--   0 runner    (1001) docker     (127)     3463 2024-05-02 10:25:31.000000 ya360-3.6.1/ya360/configure.py
--rw-r--r--   0 runner    (1001) docker     (127)     6229 2024-05-02 10:25:31.000000 ya360-3.6.1/ya360/departments.py
--rw-r--r--   0 runner    (1001) docker     (127)     6459 2024-05-02 10:25:31.000000 ya360-3.6.1/ya360/groups.py
--rw-r--r--   0 runner    (1001) docker     (127)     2736 2024-05-02 10:25:31.000000 ya360-3.6.1/ya360/logs.py
--rw-r--r--   0 runner    (1001) docker     (127)    13014 2024-05-02 10:25:31.000000 ya360-3.6.1/ya360/mail.py
--rw-r--r--   0 runner    (1001) docker     (127)     1551 2024-05-02 10:25:31.000000 ya360-3.6.1/ya360/routing.py
--rw-r--r--   0 runner    (1001) docker     (127)      514 2024-05-02 10:25:31.000000 ya360-3.6.1/ya360/tid.py
--rw-r--r--   0 runner    (1001) docker     (127)     1336 2024-05-02 10:25:31.000000 ya360-3.6.1/ya360/tools.py
--rw-r--r--   0 runner    (1001) docker     (127)     9423 2024-05-02 10:25:31.000000 ya360-3.6.1/ya360/users.py
--rw-r--r--   0 runner    (1001) docker     (127)     3620 2024-05-02 10:25:31.000000 ya360-3.6.1/ya360/whois.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-02 10:25:36.218502 ya360-3.6.1/ya360.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     2255 2024-05-02 10:25:36.000000 ya360-3.6.1/ya360.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     1060 2024-05-02 10:25:36.000000 ya360-3.6.1/ya360.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-02 10:25:36.000000 ya360-3.6.1/ya360.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       42 2024-05-02 10:25:36.000000 ya360-3.6.1/ya360.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-02 10:25:36.000000 ya360-3.6.1/ya360.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)        6 2024-05-02 10:25:36.000000 ya360-3.6.1/ya360.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-29 10:11:20.216072 ya360-3.6.2/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-29 10:11:20.208073 ya360-3.6.2/.github/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-29 10:11:20.208073 ya360-3.6.2/.github/ISSUE_TEMPLATE/
+-rw-r--r--   0 runner    (1001) docker     (127)      535 2024-05-29 10:11:15.000000 ya360-3.6.2/.github/ISSUE_TEMPLATE/bug_report.md
+-rw-r--r--   0 runner    (1001) docker     (127)      595 2024-05-29 10:11:15.000000 ya360-3.6.2/.github/ISSUE_TEMPLATE/feature_request.md
+-rw-r--r--   0 runner    (1001) docker     (127)      502 2024-05-29 10:11:15.000000 ya360-3.6.2/.github/dependabot.yml
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-29 10:11:20.208073 ya360-3.6.2/.github/workflows/
+-rw-r--r--   0 runner    (1001) docker     (127)     2740 2024-05-29 10:11:15.000000 ya360-3.6.2/.github/workflows/codeql-analysis.yml
+-rw-r--r--   0 runner    (1001) docker     (127)     1091 2024-05-29 10:11:15.000000 ya360-3.6.2/.github/workflows/python-publish.yml
+-rw-r--r--   0 runner    (1001) docker     (127)     1900 2024-05-29 10:11:15.000000 ya360-3.6.2/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (127)      730 2024-05-29 10:11:15.000000 ya360-3.6.2/.readthedocs.yaml
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-29 10:11:20.208073 ya360-3.6.2/.vscode/
+-rw-r--r--   0 runner    (1001) docker     (127)       53 2024-05-29 10:11:15.000000 ya360-3.6.2/.vscode/settings.json
+-rw-r--r--   0 runner    (1001) docker     (127)     5208 2024-05-29 10:11:15.000000 ya360-3.6.2/CODE_OF_CONDUCT.md
+-rw-r--r--   0 runner    (1001) docker     (127)     1069 2024-05-29 10:11:15.000000 ya360-3.6.2/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)       18 2024-05-29 10:11:15.000000 ya360-3.6.2/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (127)     2255 2024-05-29 10:11:20.216072 ya360-3.6.2/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     1374 2024-05-29 10:11:15.000000 ya360-3.6.2/README.md
+-rw-r--r--   0 runner    (1001) docker     (127)     1462 2024-05-29 10:11:15.000000 ya360-3.6.2/README.rst
+-rw-r--r--   0 runner    (1001) docker     (127)      175 2024-05-29 10:11:15.000000 ya360-3.6.2/SECURITY.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-29 10:11:20.208073 ya360-3.6.2/docs/
+-rw-r--r--   0 runner    (1001) docker     (127)      638 2024-05-29 10:11:15.000000 ya360-3.6.2/docs/Makefile
+-rw-r--r--   0 runner    (1001) docker     (127)      804 2024-05-29 10:11:15.000000 ya360-3.6.2/docs/make.bat
+-rw-r--r--   0 runner    (1001) docker     (127)       82 2024-05-29 10:11:15.000000 ya360-3.6.2/docs/requirements.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-29 10:11:20.212072 ya360-3.6.2/docs/source/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-29 10:11:20.212072 ya360-3.6.2/docs/source/_static/
+-rw-r--r--   0 runner    (1001) docker     (127)    38353 2024-05-29 10:11:15.000000 ya360-3.6.2/docs/source/_static/fig1.png
+-rw-r--r--   0 runner    (1001) docker     (127)   127538 2024-05-29 10:11:15.000000 ya360-3.6.2/docs/source/_static/fig2.png
+-rw-r--r--   0 runner    (1001) docker     (127)    36447 2024-05-29 10:11:15.000000 ya360-3.6.2/docs/source/_static/fig3.png
+-rw-r--r--   0 runner    (1001) docker     (127)      116 2024-05-29 10:11:15.000000 ya360-3.6.2/docs/source/_static/robots.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      859 2024-05-29 10:11:15.000000 ya360-3.6.2/docs/source/befo.rst
+-rw-r--r--   0 runner    (1001) docker     (127)     1134 2024-05-29 10:11:15.000000 ya360-3.6.2/docs/source/cmd.rst
+-rw-r--r--   0 runner    (1001) docker     (127)     2583 2024-05-29 10:11:15.000000 ya360-3.6.2/docs/source/conf.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1057 2024-05-29 10:11:15.000000 ya360-3.6.2/docs/source/index.rst
+-rw-r--r--   0 runner    (1001) docker     (127)     1080 2024-05-29 10:11:15.000000 ya360-3.6.2/docs/source/lic.rst
+-rw-r--r--   0 runner    (1001) docker     (127)      413 2024-05-29 10:11:15.000000 ya360-3.6.2/docs/source/routing.rst
+-rw-r--r--   0 runner    (1001) docker     (127)     7235 2024-05-29 10:11:15.000000 ya360-3.6.2/docs/source/usage.rst
+-rw-r--r--   0 runner    (1001) docker     (127)     1132 2024-05-29 10:11:15.000000 ya360-3.6.2/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-29 10:11:20.216072 ya360-3.6.2/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)      115 2024-05-29 10:11:15.000000 ya360-3.6.2/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-29 10:11:20.216072 ya360-3.6.2/ya360/
+-rw-r--r--   0 runner    (1001) docker     (127)      199 2024-05-29 10:11:15.000000 ya360-3.6.2/ya360/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      182 2024-05-29 10:11:15.000000 ya360-3.6.2/ya360/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1764 2024-05-29 10:11:15.000000 ya360-3.6.2/ya360/antispam.py
+-rw-r--r--   0 runner    (1001) docker     (127)    31096 2024-05-29 10:11:15.000000 ya360-3.6.2/ya360/cmd.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3463 2024-05-29 10:11:15.000000 ya360-3.6.2/ya360/configure.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6229 2024-05-29 10:11:15.000000 ya360-3.6.2/ya360/departments.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6459 2024-05-29 10:11:15.000000 ya360-3.6.2/ya360/groups.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2736 2024-05-29 10:11:15.000000 ya360-3.6.2/ya360/logs.py
+-rw-r--r--   0 runner    (1001) docker     (127)    13014 2024-05-29 10:11:15.000000 ya360-3.6.2/ya360/mail.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1551 2024-05-29 10:11:15.000000 ya360-3.6.2/ya360/routing.py
+-rw-r--r--   0 runner    (1001) docker     (127)      514 2024-05-29 10:11:15.000000 ya360-3.6.2/ya360/tid.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1336 2024-05-29 10:11:15.000000 ya360-3.6.2/ya360/tools.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9423 2024-05-29 10:11:15.000000 ya360-3.6.2/ya360/users.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3620 2024-05-29 10:11:15.000000 ya360-3.6.2/ya360/whois.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-29 10:11:20.216072 ya360-3.6.2/ya360.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     2255 2024-05-29 10:11:20.000000 ya360-3.6.2/ya360.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     1042 2024-05-29 10:11:20.000000 ya360-3.6.2/ya360.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-29 10:11:20.000000 ya360-3.6.2/ya360.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       42 2024-05-29 10:11:20.000000 ya360-3.6.2/ya360.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-29 10:11:20.000000 ya360-3.6.2/ya360.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        6 2024-05-29 10:11:20.000000 ya360-3.6.2/ya360.egg-info/top_level.txt
```

### Comparing `ya360-3.6.1/.github/ISSUE_TEMPLATE/bug_report.md` & `ya360-3.6.2/.github/ISSUE_TEMPLATE/bug_report.md`

 * *Files identical despite different names*

### Comparing `ya360-3.6.1/.github/ISSUE_TEMPLATE/feature_request.md` & `ya360-3.6.2/.github/ISSUE_TEMPLATE/feature_request.md`

 * *Files identical despite different names*

### Comparing `ya360-3.6.1/.github/workflows/codeql-analysis.yml` & `ya360-3.6.2/.github/workflows/codeql-analysis.yml`

 * *Files identical despite different names*

### Comparing `ya360-3.6.1/.github/workflows/python-publish.yml` & `ya360-3.6.2/.github/workflows/python-publish.yml`

 * *Files identical despite different names*

### Comparing `ya360-3.6.1/.gitignore` & `ya360-3.6.2/.gitignore`

 * *Files identical despite different names*

### Comparing `ya360-3.6.1/.readthedocs.yaml` & `ya360-3.6.2/.readthedocs.yaml`

 * *Files identical despite different names*

### Comparing `ya360-3.6.1/CODE_OF_CONDUCT.md` & `ya360-3.6.2/CODE_OF_CONDUCT.md`

 * *Files identical despite different names*

### Comparing `ya360-3.6.1/LICENSE` & `ya360-3.6.2/LICENSE`

 * *Files identical despite different names*

### Comparing `ya360-3.6.1/PKG-INFO` & `ya360-3.6.2/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ya360
-Version: 3.6.1
+Version: 3.6.2
 Summary: Утилита командной строки для Yandex 360
 Author-email: Купцов Игорь <ya360@uh.net.ru>
 License: MIT
 Project-URL: Homepage, https://ya360.uh.net.ru
 Project-URL: Bug Tracker, https://github.com/imercury13/ya360/issues
 Project-URL: Documentation, https://ya360.readthedocs.io/
 Project-URL: Download, https://github.com/imercury13/ya360
```

### Comparing `ya360-3.6.1/README.md` & `ya360-3.6.2/README.md`

 * *Files identical despite different names*

### Comparing `ya360-3.6.1/README.rst` & `ya360-3.6.2/README.rst`

 * *Files identical despite different names*

### Comparing `ya360-3.6.1/docs/Makefile` & `ya360-3.6.2/docs/Makefile`

 * *Files identical despite different names*

### Comparing `ya360-3.6.1/docs/make.bat` & `ya360-3.6.2/docs/make.bat`

 * *Files identical despite different names*

### Comparing `ya360-3.6.1/docs/source/_static/fig1.png` & `ya360-3.6.2/docs/source/_static/fig1.png`

 * *Files identical despite different names*

### Comparing `ya360-3.6.1/docs/source/_static/fig2.png` & `ya360-3.6.2/docs/source/_static/fig2.png`

 * *Files identical despite different names*

### Comparing `ya360-3.6.1/docs/source/_static/fig3.png` & `ya360-3.6.2/docs/source/_static/fig3.png`

 * *Files identical despite different names*

### Comparing `ya360-3.6.1/docs/source/befo.rst` & `ya360-3.6.2/docs/source/befo.rst`

 * *Files identical despite different names*

### Comparing `ya360-3.6.1/docs/source/cmd.rst` & `ya360-3.6.2/docs/source/cmd.rst`

 * *Files identical despite different names*

### Comparing `ya360-3.6.1/docs/source/conf.py` & `ya360-3.6.2/docs/source/conf.py`

 * *Files identical despite different names*

### Comparing `ya360-3.6.1/docs/source/index.rst` & `ya360-3.6.2/docs/source/index.rst`

 * *Files identical despite different names*

### Comparing `ya360-3.6.1/docs/source/lic.rst` & `ya360-3.6.2/docs/source/lic.rst`

 * *Files identical despite different names*

### Comparing `ya360-3.6.1/docs/source/usage.rst` & `ya360-3.6.2/docs/source/usage.rst`

 * *Files identical despite different names*

### Comparing `ya360-3.6.1/pyproject.toml` & `ya360-3.6.2/pyproject.toml`

 * *Files 7% similar despite different names*

```diff
@@ -23,18 +23,18 @@
 ]
 authors = [
     {name = "Купцов Игорь", email = "ya360@uh.net.ru"},
 ]
 dynamic = ["version"]
 
 [tool.setuptools_scm]
-write_to = "ya360/_version.py"
 
-[tool.setuptools.dynamic]
-version = {attr = "ya360/_version.__version__"}
+
+#[tool.setuptools.dynamic]
+#version = {attr = "ya360/_version.__version__"}
 
 [project.urls]
 "Homepage" = "https://ya360.uh.net.ru"
 "Bug Tracker" = "https://github.com/imercury13/ya360/issues"
 "Documentation" = "https://ya360.readthedocs.io/"
 "Download" = "https://github.com/imercury13/ya360"
```

### Comparing `ya360-3.6.1/ya360/antispam.py` & `ya360-3.6.2/ya360/antispam.py`

 * *Files identical despite different names*

### Comparing `ya360-3.6.1/ya360/cmd.py` & `ya360-3.6.2/ya360/cmd.py`

 * *Files identical despite different names*

### Comparing `ya360-3.6.1/ya360/configure.py` & `ya360-3.6.2/ya360/configure.py`

 * *Files identical despite different names*

### Comparing `ya360-3.6.1/ya360/departments.py` & `ya360-3.6.2/ya360/departments.py`

 * *Files identical despite different names*

### Comparing `ya360-3.6.1/ya360/groups.py` & `ya360-3.6.2/ya360/groups.py`

 * *Files identical despite different names*

### Comparing `ya360-3.6.1/ya360/logs.py` & `ya360-3.6.2/ya360/logs.py`

 * *Files identical despite different names*

### Comparing `ya360-3.6.1/ya360/mail.py` & `ya360-3.6.2/ya360/mail.py`

 * *Files identical despite different names*

### Comparing `ya360-3.6.1/ya360/routing.py` & `ya360-3.6.2/ya360/routing.py`

 * *Files identical despite different names*

### Comparing `ya360-3.6.1/ya360/tid.py` & `ya360-3.6.2/ya360/tid.py`

 * *Files identical despite different names*

### Comparing `ya360-3.6.1/ya360/tools.py` & `ya360-3.6.2/ya360/tools.py`

 * *Files identical despite different names*

### Comparing `ya360-3.6.1/ya360/users.py` & `ya360-3.6.2/ya360/users.py`

 * *Files 0% similar despite different names*

```diff
@@ -157,15 +157,15 @@
 		if args.passwordChangeRequired == 'true':
 			body.update({'passwordChangeRequired': True})
 		else:
 			body.update({'passwordChangeRequired': False})
 
 	uid = check_request(tools.get_id_user_by_nickname(args.nickname, __token__, __orgid__))['id']
 
-	check_request(users.update_user(__token__, __orgid__, body, uid))
+	check_request(users.update_user(__token__, __orgid__, uid, body))
 	print('Обновлено')
 
 
 def create_user(args):
 	"""Функция создания пользователя
 	
 	:param args: словарь аргументов командной строки
```

### Comparing `ya360-3.6.1/ya360/whois.py` & `ya360-3.6.2/ya360/whois.py`

 * *Files identical despite different names*

### Comparing `ya360-3.6.1/ya360.egg-info/PKG-INFO` & `ya360-3.6.2/ya360.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ya360
-Version: 3.6.1
+Version: 3.6.2
 Summary: Утилита командной строки для Yandex 360
 Author-email: Купцов Игорь <ya360@uh.net.ru>
 License: MIT
 Project-URL: Homepage, https://ya360.uh.net.ru
 Project-URL: Bug Tracker, https://github.com/imercury13/ya360/issues
 Project-URL: Documentation, https://ya360.readthedocs.io/
 Project-URL: Download, https://github.com/imercury13/ya360
```

### Comparing `ya360-3.6.1/ya360.egg-info/SOURCES.txt` & `ya360-3.6.2/ya360.egg-info/SOURCES.txt`

 * *Files 11% similar despite different names*

```diff
@@ -26,15 +26,14 @@
 docs/source/usage.rst
 docs/source/_static/fig1.png
 docs/source/_static/fig2.png
 docs/source/_static/fig3.png
 docs/source/_static/robots.txt
 ya360/__init__.py
 ya360/__main__.py
-ya360/_version.py
 ya360/antispam.py
 ya360/cmd.py
 ya360/configure.py
 ya360/departments.py
 ya360/groups.py
 ya360/logs.py
 ya360/mail.py
```

