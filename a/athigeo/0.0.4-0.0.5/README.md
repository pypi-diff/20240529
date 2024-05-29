# Comparing `tmp/athigeo-0.0.4.tar.gz` & `tmp/athigeo-0.0.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "athigeo-0.0.4.tar", last modified: Sat May 11 12:48:39 2024, max compression
+gzip compressed data, was "athigeo-0.0.5.tar", last modified: Tue May 28 13:31:25 2024, max compression
```

## Comparing `athigeo-0.0.4.tar` & `athigeo-0.0.5.tar`

### file list

```diff
@@ -1,56 +1,62 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-11 12:48:39.597303 athigeo-0.0.4/
--rw-r--r--   0 runner    (1001) docker     (127)      292 2024-05-11 12:48:28.000000 athigeo-0.0.4/.editorconfig
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-11 12:48:39.589303 athigeo-0.0.4/.github/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-11 12:48:39.593303 athigeo-0.0.4/.github/ISSUE_TEMPLATE/
--rw-r--r--   0 runner    (1001) docker     (127)      507 2024-05-11 12:48:28.000000 athigeo-0.0.4/.github/ISSUE_TEMPLATE/bug_report.md
--rw-r--r--   0 runner    (1001) docker     (127)      492 2024-05-11 12:48:28.000000 athigeo-0.0.4/.github/ISSUE_TEMPLATE/config.yml
--rw-r--r--   0 runner    (1001) docker     (127)      441 2024-05-11 12:48:28.000000 athigeo-0.0.4/.github/ISSUE_TEMPLATE/feature_request.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-11 12:48:39.593303 athigeo-0.0.4/.github/workflows/
--rw-r--r--   0 runner    (1001) docker     (127)     2005 2024-05-11 12:48:28.000000 athigeo-0.0.4/.github/workflows/docs-build.yml
--rw-r--r--   0 runner    (1001) docker     (127)      915 2024-05-11 12:48:28.000000 athigeo-0.0.4/.github/workflows/docs.yml
--rw-r--r--   0 runner    (1001) docker     (127)      738 2024-05-11 12:48:28.000000 athigeo-0.0.4/.github/workflows/installation.yml
--rw-r--r--   0 runner    (1001) docker     (127)     1082 2024-05-11 12:48:28.000000 athigeo-0.0.4/.github/workflows/macos.yml
--rw-r--r--   0 runner    (1001) docker     (127)      993 2024-05-11 12:48:28.000000 athigeo-0.0.4/.github/workflows/pypi.yml
--rw-r--r--   0 runner    (1001) docker     (127)     1521 2024-05-11 12:48:28.000000 athigeo-0.0.4/.github/workflows/ubuntu.yml
--rw-r--r--   0 runner    (1001) docker     (127)      974 2024-05-11 12:48:28.000000 athigeo-0.0.4/.github/workflows/windows.yml
--rw-r--r--   0 runner    (1001) docker     (127)     1267 2024-05-11 12:48:28.000000 athigeo-0.0.4/.gitignore
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-11 12:48:28.000000 athigeo-0.0.4/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)      122 2024-05-11 12:48:28.000000 athigeo-0.0.4/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (127)     1340 2024-05-11 12:48:39.597303 athigeo-0.0.4/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      435 2024-05-11 12:48:28.000000 athigeo-0.0.4/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-11 12:48:39.593303 athigeo-0.0.4/athigeo/
--rw-r--r--   0 runner    (1001) docker     (127)      159 2024-05-11 12:48:28.000000 athigeo-0.0.4/athigeo/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2469 2024-05-11 12:48:28.000000 athigeo-0.0.4/athigeo/athigeo.py
--rw-r--r--   0 runner    (1001) docker     (127)      360 2024-05-11 12:48:28.000000 athigeo-0.0.4/athigeo/common.py
--rw-r--r--   0 runner    (1001) docker     (127)      354 2024-05-11 12:48:28.000000 athigeo-0.0.4/athigeo/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-11 12:48:39.597303 athigeo-0.0.4/athigeo.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     1340 2024-05-11 12:48:39.000000 athigeo-0.0.4/athigeo.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      973 2024-05-11 12:48:39.000000 athigeo-0.0.4/athigeo.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-11 12:48:39.000000 athigeo-0.0.4/athigeo.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       45 2024-05-11 12:48:39.000000 athigeo-0.0.4/athigeo.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (127)       62 2024-05-11 12:48:39.000000 athigeo-0.0.4/athigeo.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)        8 2024-05-11 12:48:39.000000 athigeo-0.0.4/athigeo.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-11 12:48:39.597303 athigeo-0.0.4/docs/
--rw-r--r--   0 runner    (1001) docker     (127)       12 2024-05-11 12:48:28.000000 athigeo-0.0.4/docs/CNAME
--rw-r--r--   0 runner    (1001) docker     (127)       39 2024-05-11 12:48:28.000000 athigeo-0.0.4/docs/athigeo.md
--rw-r--r--   0 runner    (1001) docker     (127)       85 2024-05-11 12:48:28.000000 athigeo-0.0.4/docs/changelog.md
--rw-r--r--   0 runner    (1001) docker     (127)       35 2024-05-11 12:48:28.000000 athigeo-0.0.4/docs/common.md
--rw-r--r--   0 runner    (1001) docker     (127)     3114 2024-05-11 12:48:28.000000 athigeo-0.0.4/docs/contributing.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-11 12:48:39.597303 athigeo-0.0.4/docs/examples/
--rw-r--r--   0 runner    (1001) docker     (127)    11141 2024-05-11 12:48:28.000000 athigeo-0.0.4/docs/examples/csv.ipynb
--rw-r--r--   0 runner    (1001) docker     (127)      288 2024-05-11 12:48:28.000000 athigeo-0.0.4/docs/examples/intro.ipynb
--rw-r--r--   0 runner    (1001) docker     (127)        6 2024-05-11 12:48:28.000000 athigeo-0.0.4/docs/faq.md
--rw-r--r--   0 runner    (1001) docker     (127)      246 2024-05-11 12:48:28.000000 athigeo-0.0.4/docs/index.md
--rw-r--r--   0 runner    (1001) docker     (127)      560 2024-05-11 12:48:28.000000 athigeo-0.0.4/docs/installation.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-11 12:48:39.597303 athigeo-0.0.4/docs/overrides/
--rw-r--r--   0 runner    (1001) docker     (127)      274 2024-05-11 12:48:28.000000 athigeo-0.0.4/docs/overrides/main.html
--rw-r--r--   0 runner    (1001) docker     (127)       62 2024-05-11 12:48:28.000000 athigeo-0.0.4/docs/usage.md
--rw-r--r--   0 runner    (1001) docker     (127)       33 2024-05-11 12:48:28.000000 athigeo-0.0.4/docs/utils.md
--rw-r--r--   0 runner    (1001) docker     (127)     2147 2024-05-11 12:48:28.000000 athigeo-0.0.4/mkdocs.yml
--rw-r--r--   0 runner    (1001) docker     (127)     1627 2024-05-11 12:48:28.000000 athigeo-0.0.4/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)       23 2024-05-11 12:48:28.000000 athigeo-0.0.4/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (127)      400 2024-05-11 12:48:28.000000 athigeo-0.0.4/requirements_dev.txt
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-11 12:48:39.597303 athigeo-0.0.4/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-11 12:48:39.597303 athigeo-0.0.4/tests/
--rw-r--r--   0 runner    (1001) docker     (127)       37 2024-05-11 12:48:28.000000 athigeo-0.0.4/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      387 2024-05-11 12:48:28.000000 athigeo-0.0.4/tests/test_athigeo.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-28 13:31:25.713899 athigeo-0.0.5/
+-rw-r--r--   0 runner    (1001) docker     (127)      292 2024-05-28 13:31:15.000000 athigeo-0.0.5/.editorconfig
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-28 13:31:25.705899 athigeo-0.0.5/.github/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-28 13:31:25.709899 athigeo-0.0.5/.github/ISSUE_TEMPLATE/
+-rw-r--r--   0 runner    (1001) docker     (127)      507 2024-05-28 13:31:15.000000 athigeo-0.0.5/.github/ISSUE_TEMPLATE/bug_report.md
+-rw-r--r--   0 runner    (1001) docker     (127)      492 2024-05-28 13:31:15.000000 athigeo-0.0.5/.github/ISSUE_TEMPLATE/config.yml
+-rw-r--r--   0 runner    (1001) docker     (127)      441 2024-05-28 13:31:15.000000 athigeo-0.0.5/.github/ISSUE_TEMPLATE/feature_request.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-28 13:31:25.709899 athigeo-0.0.5/.github/workflows/
+-rw-r--r--   0 runner    (1001) docker     (127)     2005 2024-05-28 13:31:15.000000 athigeo-0.0.5/.github/workflows/docs-build.yml
+-rw-r--r--   0 runner    (1001) docker     (127)      911 2024-05-28 13:31:15.000000 athigeo-0.0.5/.github/workflows/docs.yml
+-rw-r--r--   0 runner    (1001) docker     (127)      738 2024-05-28 13:31:15.000000 athigeo-0.0.5/.github/workflows/installation.yml
+-rw-r--r--   0 runner    (1001) docker     (127)     1082 2024-05-28 13:31:15.000000 athigeo-0.0.5/.github/workflows/macos.yml
+-rw-r--r--   0 runner    (1001) docker     (127)      993 2024-05-28 13:31:15.000000 athigeo-0.0.5/.github/workflows/pypi.yml
+-rw-r--r--   0 runner    (1001) docker     (127)     1521 2024-05-28 13:31:15.000000 athigeo-0.0.5/.github/workflows/ubuntu.yml
+-rw-r--r--   0 runner    (1001) docker     (127)      974 2024-05-28 13:31:15.000000 athigeo-0.0.5/.github/workflows/windows.yml
+-rw-r--r--   0 runner    (1001) docker     (127)     1267 2024-05-28 13:31:15.000000 athigeo-0.0.5/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-28 13:31:15.000000 athigeo-0.0.5/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)      122 2024-05-28 13:31:15.000000 athigeo-0.0.5/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (127)     1340 2024-05-28 13:31:25.713899 athigeo-0.0.5/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      435 2024-05-28 13:31:15.000000 athigeo-0.0.5/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-28 13:31:25.709899 athigeo-0.0.5/athigeo/
+-rw-r--r--   0 runner    (1001) docker     (127)      159 2024-05-28 13:31:15.000000 athigeo-0.0.5/athigeo/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7357 2024-05-28 13:31:15.000000 athigeo-0.0.5/athigeo/athigeo.py
+-rw-r--r--   0 runner    (1001) docker     (127)      360 2024-05-28 13:31:15.000000 athigeo-0.0.5/athigeo/common.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2727 2024-05-28 13:31:15.000000 athigeo-0.0.5/athigeo/foliumap.py
+-rw-r--r--   0 runner    (1001) docker     (127)      355 2024-05-28 13:31:15.000000 athigeo-0.0.5/athigeo/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-28 13:31:25.713899 athigeo-0.0.5/athigeo.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     1340 2024-05-28 13:31:25.000000 athigeo-0.0.5/athigeo.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     1133 2024-05-28 13:31:25.000000 athigeo-0.0.5/athigeo.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-28 13:31:25.000000 athigeo-0.0.5/athigeo.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       45 2024-05-28 13:31:25.000000 athigeo-0.0.5/athigeo.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       62 2024-05-28 13:31:25.000000 athigeo-0.0.5/athigeo.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        8 2024-05-28 13:31:25.000000 athigeo-0.0.5/athigeo.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-28 13:31:25.713899 athigeo-0.0.5/docs/
+-rw-r--r--   0 runner    (1001) docker     (127)       12 2024-05-28 13:31:15.000000 athigeo-0.0.5/docs/CNAME
+-rw-r--r--   0 runner    (1001) docker     (127)       39 2024-05-28 13:31:15.000000 athigeo-0.0.5/docs/athigeo.md
+-rw-r--r--   0 runner    (1001) docker     (127)       85 2024-05-28 13:31:15.000000 athigeo-0.0.5/docs/changelog.md
+-rw-r--r--   0 runner    (1001) docker     (127)       35 2024-05-28 13:31:15.000000 athigeo-0.0.5/docs/common.md
+-rw-r--r--   0 runner    (1001) docker     (127)     3114 2024-05-28 13:31:15.000000 athigeo-0.0.5/docs/contributing.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-28 13:31:25.713899 athigeo-0.0.5/docs/examples/
+-rw-r--r--   0 runner    (1001) docker     (127)     1093 2024-05-28 13:31:15.000000 athigeo-0.0.5/docs/examples/csv.ipynb
+-rw-r--r--   0 runner    (1001) docker     (127)     2243 2024-05-28 13:31:15.000000 athigeo-0.0.5/docs/examples/folium.ipynb
+-rw-r--r--   0 runner    (1001) docker     (127)      288 2024-05-28 13:31:15.000000 athigeo-0.0.5/docs/examples/intro.ipynb
+-rw-r--r--   0 runner    (1001) docker     (127)    18947 2024-05-28 13:31:15.000000 athigeo-0.0.5/docs/examples/ipywidgets.ipynb
+-rw-r--r--   0 runner    (1001) docker     (127)     7791 2024-05-28 13:31:15.000000 athigeo-0.0.5/docs/examples/raster.ipynb
+-rw-r--r--   0 runner    (1001) docker     (127)     7356 2024-05-28 13:31:15.000000 athigeo-0.0.5/docs/examples/toolbar.ipynb
+-rw-r--r--   0 runner    (1001) docker     (127)     3268 2024-05-28 13:31:15.000000 athigeo-0.0.5/docs/examples/vector.ipynb
+-rw-r--r--   0 runner    (1001) docker     (127)        6 2024-05-28 13:31:15.000000 athigeo-0.0.5/docs/faq.md
+-rw-r--r--   0 runner    (1001) docker     (127)      321 2024-05-28 13:31:15.000000 athigeo-0.0.5/docs/index.md
+-rw-r--r--   0 runner    (1001) docker     (127)      560 2024-05-28 13:31:15.000000 athigeo-0.0.5/docs/installation.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-28 13:31:25.713899 athigeo-0.0.5/docs/overrides/
+-rw-r--r--   0 runner    (1001) docker     (127)      274 2024-05-28 13:31:15.000000 athigeo-0.0.5/docs/overrides/main.html
+-rw-r--r--   0 runner    (1001) docker     (127)       62 2024-05-28 13:31:15.000000 athigeo-0.0.5/docs/usage.md
+-rw-r--r--   0 runner    (1001) docker     (127)       33 2024-05-28 13:31:15.000000 athigeo-0.0.5/docs/utils.md
+-rw-r--r--   0 runner    (1001) docker     (127)     2498 2024-05-28 13:31:15.000000 athigeo-0.0.5/mkdocs.yml
+-rw-r--r--   0 runner    (1001) docker     (127)     1627 2024-05-28 13:31:15.000000 athigeo-0.0.5/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)       23 2024-05-28 13:31:15.000000 athigeo-0.0.5/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      400 2024-05-28 13:31:15.000000 athigeo-0.0.5/requirements_dev.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-28 13:31:25.713899 athigeo-0.0.5/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-28 13:31:25.713899 athigeo-0.0.5/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)       37 2024-05-28 13:31:15.000000 athigeo-0.0.5/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      387 2024-05-28 13:31:15.000000 athigeo-0.0.5/tests/test_athigeo.py
```

### Comparing `athigeo-0.0.4/.github/workflows/docs-build.yml` & `athigeo-0.0.5/.github/workflows/docs-build.yml`

 * *Files identical despite different names*

### Comparing `athigeo-0.0.4/.github/workflows/docs.yml` & `athigeo-0.0.5/.github/workflows/docs.yml`

 * *Files 4% similar despite different names*

```diff
@@ -1,13 +1,12 @@
 name: docs
 on:
     push:
         branches:
             - main
-            - master
 jobs:
     deploy:
         runs-on: ubuntu-latest
         steps:
             - uses: actions/checkout@v4
             - uses: actions/setup-python@v5
               with:
@@ -17,13 +16,12 @@
               run: |
                   python -m pip install --upgrade pip
                   pip install --user --no-cache-dir Cython
                   pip install --user -r requirements.txt -r requirements_dev.txt
                   pip install .
             - name: Discover typos with codespell
               run: |
-                  codespell --skip="*.csv,*.geojson,*.json,*.js,*.html,*cff,./.git" --ignore-words-list="aci,hist"
+                  codespell --skip="*.geojson,*.json,*.js,*.html,*cff,./.git,*.txt,*data_types.ipynb" --ignore-words-list="aci,hist"
             - name: PKG-TEST
               run: |
                   python -m unittest discover tests/
             - run: mkdocs gh-deploy --force
-
```

### Comparing `athigeo-0.0.4/.github/workflows/installation.yml` & `athigeo-0.0.5/.github/workflows/installation.yml`

 * *Files identical despite different names*

### Comparing `athigeo-0.0.4/.github/workflows/macos.yml` & `athigeo-0.0.5/.github/workflows/macos.yml`

 * *Files identical despite different names*

### Comparing `athigeo-0.0.4/.github/workflows/pypi.yml` & `athigeo-0.0.5/.github/workflows/pypi.yml`

 * *Files identical despite different names*

### Comparing `athigeo-0.0.4/.github/workflows/ubuntu.yml` & `athigeo-0.0.5/.github/workflows/ubuntu.yml`

 * *Files identical despite different names*

### Comparing `athigeo-0.0.4/.github/workflows/windows.yml` & `athigeo-0.0.5/.github/workflows/windows.yml`

 * *Files identical despite different names*

### Comparing `athigeo-0.0.4/.gitignore` & `athigeo-0.0.5/.gitignore`

 * *Files identical despite different names*

### Comparing `athigeo-0.0.4/PKG-INFO` & `athigeo-0.0.5/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: athigeo
-Version: 0.0.4
+Version: 0.0.5
 Summary: A python package intro
 Author-email: Dennis Mutai <dennis.mutaigeo@gmail.com>
 License: MIT License
 Project-URL: Homepage, https://github.com/Dmutai/athigeo
 Keywords: athigeo
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: MIT License
```

### Comparing `athigeo-0.0.4/athigeo/athigeo.py` & `athigeo-0.0.5/athigeo/foliumap.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,78 +1,88 @@
-"""Main module."""
+import folium
+from ipyleaflet import basemaps
 
 
-import ipyleaflet
-from ipyleaflet import basemaps
+class Map(folium.Map):
 
-class Map(ipyleaflet.Map):
-    """This is the map class that inherits from ipyleaflet.Map.
+    def __init__(self, center=[20, 0], zoom=2, **kwargs):
+        super().__init__(location=center, zoom_start=zoom, **kwargs)
 
-    Args:
-        ipyleaflet (Map): The ipyleaflet.Map class.
-    """
-    def __init__(self, center = [20, 0], zoom = 2, **kwargs):
-        """Initialize the map.
+    def add_raster(self, data, name="raster", **kwargs):
+        """Adds a raster layer to the map.
 
         Args:
-            center (list, optional): Set the center of the map. Defaults to [20, 0].
-            zoom (int, optional): Set the zoom level of the map. Defaults to 2.
+            data (str): The path to the raster file.
+            name (str, optional): The name of the layer. Defaults to "raster".
+        """
+
+        try:
+            from localtileserver import TileClient, get_folium_tile_layer
+        except ImportError:
+            raise ImportError("Please install the localtileserver package.")
+
+        client = TileClient(data)
+        layer = get_folium_tile_layer(client, name=name, **kwargs)
+        layer.add_to(self)
+
+    def add_tile_layer(self, url, name, attribution="Custom Tile", **kwargs):
         """
-        super().__init__(center = center, zoom = zoom, **kwargs)
-        self.add_control(ipyleaflet.LayersControl())
+        Adds a tile layer to the current map.
 
+        Args:
+            url (str): The URL of the tile layer.
+            name (str): The name of the layer.
+            attribution (str, optional): The attribution text to be displayed for the layer. Defaults to "Custom Tile".
+            **kwargs: Arbitrary keyword arguments for additional layer options.
 
-    def add_tile_layer(self, url, name, **kwargs):
-        layer = ipyleaflet.TileLayer(url=url, name=name, **kwargs)
-        self.add_layer(layer)
+        Returns:
+            None
+        """
+        layer = folium.TileLayer(tiles=url, name=name, attr=attribution, **kwargs)
+        layer.add_to(self)
 
-    def add_basemap(self, name):
-        """Adds a basemap to the map.
+    def add_basemap(self, name, overlay=True):
+        """
+        Adds a basemap to the current map.
 
         Args:
-            name (str): The name of the basemap to add to the map. Check ipyleaflet website for possible names
+            name (str or object): The name of the basemap as a string, or an object representing the basemap.
+            overlay (bool, optional): Whether the basemap is an overlay. Defaults to True.
+
+        Raises:
+            TypeError: If the name is neither a string nor an object representing a basemap.
+
+        Returns:
+            None
         """
+
         if isinstance(name, str):
             url = eval(f"basemaps.{name}").build_url()
-            self.add_tile_layer(url, name)
+            self.add_tile_layer(url, name, overlay=overlay)
         else:
-            self.add(name)
+            name.add_to(self)
 
-    def add_geojson(self, data, name = "geojson", **kwargs):
-        """Adds a GeoJSON layer to the map.
+    def to_streamlit(self, width=700, height=500):
+        """
+        Converts the map to a streamlit component.
 
         Args:
-            data (str | dict): The GeoJSON data as a string or a dictionary.
-            name (str, optional): The name of the layer. Defaults to "geojson".
+            width (int, optional): The width of the map. Defaults to 700.
+            height (int, optional): The height of the map. Defaults to 500.
+
+        Returns:
+            object: The streamlit component representing the map.
         """
-        import json
-        
-        if isinstance(data, str):
-                with open(data) as f:
-                    data = json.load(f)
-
-
-        if "style" not in kwargs:
-            kwargs["style"] = {"color": "blue", "weight": 1, "fillOpacity": 0}
-        
-        if "hover_style" not in kwargs:
-            kwargs["hover_style"] = {"fillColor": "red", "fillOpacity": 0.3}
 
-        layer = ipyleaflet.GeoJSON(data=data, name=name, **kwargs)
-        self.add(layer)
+        from streamlit_folium import folium_static
 
-    def add_shp(self, data, name = "shp", **kwargs):
-        """Adds a shapefile to the current map.
+        return folium_static(self, width=width, height=height)
 
-        Args:
-            data (str or dict): The path to the shapefile as a string or a dictionary representing a shapefile.
-            name (str, optional): Name of the layer. Defaults to "shp".
+    def add_layer_control(self):
         """
+        Adds a layer control to the map.
 
-        import shapefile
-        import json
-
-        if isinstance(data, str):
-            with shapefile.Reader(data) as shp:
-                data = shp.__geo_interface__
-        self.add_geojson(data, name, **kwargs)
+        Returns:
+            None
+        """
 
+        folium.LayerControl().add_to(self)
```

### Comparing `athigeo-0.0.4/athigeo.egg-info/PKG-INFO` & `athigeo-0.0.5/athigeo.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: athigeo
-Version: 0.0.4
+Version: 0.0.5
 Summary: A python package intro
 Author-email: Dennis Mutai <dennis.mutaigeo@gmail.com>
 License: MIT License
 Project-URL: Homepage, https://github.com/Dmutai/athigeo
 Keywords: athigeo
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: MIT License
```

### Comparing `athigeo-0.0.4/docs/contributing.md` & `athigeo-0.0.5/docs/contributing.md`

 * *Files identical despite different names*

### Comparing `athigeo-0.0.4/docs/installation.md` & `athigeo-0.0.5/docs/installation.md`

 * *Files identical despite different names*

### Comparing `athigeo-0.0.4/mkdocs.yml` & `athigeo-0.0.5/mkdocs.yml`

 * *Files 18% similar despite different names*

```diff
@@ -46,15 +46,21 @@
     # - pdf-export
     - mkdocs-jupyter:
           include_source: True
           ignore_h1_titles: True
           execute: True
           allow_errors: false
           ignore: ["conf.py"]
-          execute_ignore: ["*ignore.ipynb"]
+          execute_ignore: 
+              [
+                  "*ignore.ipynb",
+                  "raster.ipynb",
+                  "vector.ipynb",
+                  "folium.ipynb",                 
+              ]
           
 markdown_extensions:
     - admonition
     - abbr
     - attr_list
     - def_list
     - footnotes
@@ -78,11 +84,17 @@
     - Contributing: contributing.md
     - FAQ: faq.md
     - Changelog: changelog.md
     - Report Issues: https://github.com/Dmutai/athigeo/issues
     - Examples:
         - examples/intro.ipynb
         - examples/csv.ipynb
+        - examples/ipywidgets.ipynb
+        - examples/toolbar.ipynb
+        - examples/raster.ipynb
+        - examples/vector.ipynb
+        - examples/folium.ipynb
+                
     - API Reference:
           - athigeo module: athigeo.md
           - common module: common.md
           - utils module: utils.md
```

### Comparing `athigeo-0.0.4/pyproject.toml` & `athigeo-0.0.5/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [project]
 name = "athigeo"
-version = "0.0.4"
+version = "0.0.5"
 dynamic = [
     "dependencies",
 ]
 description = "A python package intro"
 readme = "README.md"
 requires-python = ">=3.8"
 keywords = [
@@ -48,15 +48,15 @@
 
 
 [tool.distutils.bdist_wheel]
 universal = true
 
 
 [tool.bumpversion]
-current_version = "0.0.4"
+current_version = "0.0.5"
 commit = true
 tag = true
 
 [[tool.bumpversion.files]]
 filename = "pyproject.toml"
 search = 'version = "{current_version}"'
 replace = 'version = "{new_version}"'
```

