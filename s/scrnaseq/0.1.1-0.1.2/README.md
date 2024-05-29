# Comparing `tmp/scrnaseq-0.1.1.tar.gz` & `tmp/scrnaseq-0.1.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "scrnaseq-0.1.1.tar", last modified: Tue May 28 21:26:02 2024, max compression
+gzip compressed data, was "scrnaseq-0.1.2.tar", last modified: Wed May 29 14:45:17 2024, max compression
```

## Comparing `scrnaseq-0.1.1.tar` & `scrnaseq-0.1.2.tar`

### file list

```diff
@@ -1,58 +1,58 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-28 21:26:02.016818 scrnaseq-0.1.1/
--rw-r--r--   0 runner    (1001) docker     (127)      591 2024-05-28 21:20:48.000000 scrnaseq-0.1.1/.coveragerc
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-28 21:26:02.004818 scrnaseq-0.1.1/.github/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-28 21:26:02.008818 scrnaseq-0.1.1/.github/workflows/
--rw-r--r--   0 runner    (1001) docker     (127)     2431 2024-05-28 21:20:48.000000 scrnaseq-0.1.1/.github/workflows/pypi-publish.yml
--rw-r--r--   0 runner    (1001) docker     (127)     1694 2024-05-28 21:20:48.000000 scrnaseq-0.1.1/.github/workflows/pypi-test.yml
--rw-r--r--   0 runner    (1001) docker     (127)      566 2024-05-28 21:20:48.000000 scrnaseq-0.1.1/.gitignore
--rw-r--r--   0 runner    (1001) docker     (127)     1336 2024-05-28 21:20:48.000000 scrnaseq-0.1.1/.pre-commit-config.yaml
--rw-r--r--   0 runner    (1001) docker     (127)      530 2024-05-28 21:20:48.000000 scrnaseq-0.1.1/.readthedocs.yml
--rw-r--r--   0 runner    (1001) docker     (127)      102 2024-05-28 21:20:48.000000 scrnaseq-0.1.1/AUTHORS.md
--rw-r--r--   0 runner    (1001) docker     (127)      115 2024-05-28 21:20:48.000000 scrnaseq-0.1.1/CHANGELOG.md
--rw-r--r--   0 runner    (1001) docker     (127)    13490 2024-05-28 21:20:48.000000 scrnaseq-0.1.1/CONTRIBUTING.md
--rw-r--r--   0 runner    (1001) docker     (127)     1084 2024-05-28 21:20:48.000000 scrnaseq-0.1.1/LICENSE.txt
--rw-r--r--   0 runner    (1001) docker     (127)    13062 2024-05-28 21:26:02.016818 scrnaseq-0.1.1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)    11937 2024-05-28 21:20:48.000000 scrnaseq-0.1.1/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-28 21:26:02.008818 scrnaseq-0.1.1/docs/
--rw-r--r--   0 runner    (1001) docker     (127)     1154 2024-05-28 21:20:48.000000 scrnaseq-0.1.1/docs/Makefile
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-28 21:26:02.008818 scrnaseq-0.1.1/docs/_static/
--rw-r--r--   0 runner    (1001) docker     (127)       18 2024-05-28 21:20:48.000000 scrnaseq-0.1.1/docs/_static/.gitignore
--rw-r--r--   0 runner    (1001) docker     (127)       71 2024-05-28 21:20:48.000000 scrnaseq-0.1.1/docs/authors.md
--rw-r--r--   0 runner    (1001) docker     (127)       73 2024-05-28 21:20:48.000000 scrnaseq-0.1.1/docs/changelog.md
--rw-r--r--   0 runner    (1001) docker     (127)    10838 2024-05-28 21:20:48.000000 scrnaseq-0.1.1/docs/conf.py
--rw-r--r--   0 runner    (1001) docker     (127)       76 2024-05-28 21:20:48.000000 scrnaseq-0.1.1/docs/contributing.md
--rw-r--r--   0 runner    (1001) docker     (127)     1248 2024-05-28 21:20:48.000000 scrnaseq-0.1.1/docs/index.md
--rw-r--r--   0 runner    (1001) docker     (127)       66 2024-05-28 21:20:48.000000 scrnaseq-0.1.1/docs/license.md
--rw-r--r--   0 runner    (1001) docker     (127)       70 2024-05-28 21:20:48.000000 scrnaseq-0.1.1/docs/readme.md
--rw-r--r--   0 runner    (1001) docker     (127)      284 2024-05-28 21:20:48.000000 scrnaseq-0.1.1/docs/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (127)      589 2024-05-28 21:20:48.000000 scrnaseq-0.1.1/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)     1416 2024-05-28 21:26:02.016818 scrnaseq-0.1.1/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)      683 2024-05-28 21:20:48.000000 scrnaseq-0.1.1/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-28 21:26:02.004818 scrnaseq-0.1.1/src/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-28 21:26:02.012818 scrnaseq-0.1.1/src/scrnaseq/
--rw-r--r--   0 runner    (1001) docker     (127)      909 2024-05-28 21:20:48.000000 scrnaseq-0.1.1/src/scrnaseq/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     4212 2024-05-28 21:20:48.000000 scrnaseq-0.1.1/src/scrnaseq/fetch_dataset.py
--rw-r--r--   0 runner    (1001) docker     (127)     6076 2024-05-28 21:20:48.000000 scrnaseq-0.1.1/src/scrnaseq/list_datasets.py
--rw-r--r--   0 runner    (1001) docker     (127)      863 2024-05-28 21:20:48.000000 scrnaseq-0.1.1/src/scrnaseq/list_versions.py
--rw-r--r--   0 runner    (1001) docker     (127)     4435 2024-05-28 21:20:48.000000 scrnaseq-0.1.1/src/scrnaseq/polish_dataset.py
--rw-r--r--   0 runner    (1001) docker     (127)     3937 2024-05-28 21:20:48.000000 scrnaseq-0.1.1/src/scrnaseq/save_dataset.py
--rw-r--r--   0 runner    (1001) docker     (127)     3492 2024-05-28 21:20:48.000000 scrnaseq-0.1.1/src/scrnaseq/search_datasets.py
--rw-r--r--   0 runner    (1001) docker     (127)     2412 2024-05-28 21:20:48.000000 scrnaseq-0.1.1/src/scrnaseq/upload_dataset.py
--rw-r--r--   0 runner    (1001) docker     (127)     3790 2024-05-28 21:20:48.000000 scrnaseq-0.1.1/src/scrnaseq/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-28 21:26:02.016818 scrnaseq-0.1.1/src/scrnaseq.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)    13062 2024-05-28 21:26:01.000000 scrnaseq-0.1.1/src/scrnaseq.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     1096 2024-05-28 21:26:02.000000 scrnaseq-0.1.1/src/scrnaseq.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-28 21:26:01.000000 scrnaseq-0.1.1/src/scrnaseq.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-28 21:26:01.000000 scrnaseq-0.1.1/src/scrnaseq.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (127)      260 2024-05-28 21:26:01.000000 scrnaseq-0.1.1/src/scrnaseq.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)        9 2024-05-28 21:26:01.000000 scrnaseq-0.1.1/src/scrnaseq.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-28 21:26:02.012818 scrnaseq-0.1.1/tests/
--rw-r--r--   0 runner    (1001) docker     (127)      255 2024-05-28 21:20:48.000000 scrnaseq-0.1.1/tests/conftest.py
--rw-r--r--   0 runner    (1001) docker     (127)     1856 2024-05-28 21:20:48.000000 scrnaseq-0.1.1/tests/test_fetch_dataset.py
--rw-r--r--   0 runner    (1001) docker     (127)      325 2024-05-28 21:20:48.000000 scrnaseq-0.1.1/tests/test_list_dataset.py
--rw-r--r--   0 runner    (1001) docker     (127)      459 2024-05-28 21:20:48.000000 scrnaseq-0.1.1/tests/test_list_version.py
--rw-r--r--   0 runner    (1001) docker     (127)     5786 2024-05-28 21:20:48.000000 scrnaseq-0.1.1/tests/test_polish_dataset.py
--rw-r--r--   0 runner    (1001) docker     (127)     3088 2024-05-28 21:20:48.000000 scrnaseq-0.1.1/tests/test_save_dataset.py
--rw-r--r--   0 runner    (1001) docker     (127)      883 2024-05-28 21:20:48.000000 scrnaseq-0.1.1/tests/test_search_datasets.py
--rw-r--r--   0 runner    (1001) docker     (127)     4705 2024-05-28 21:20:48.000000 scrnaseq-0.1.1/tests/test_upload_dataset.py
--rw-r--r--   0 runner    (1001) docker     (127)     2851 2024-05-28 21:20:48.000000 scrnaseq-0.1.1/tox.ini
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-29 14:45:17.789091 scrnaseq-0.1.2/
+-rw-r--r--   0 runner    (1001) docker     (127)      591 2024-05-29 14:41:12.000000 scrnaseq-0.1.2/.coveragerc
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-29 14:45:17.777091 scrnaseq-0.1.2/.github/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-29 14:45:17.781091 scrnaseq-0.1.2/.github/workflows/
+-rw-r--r--   0 runner    (1001) docker     (127)     2431 2024-05-29 14:41:12.000000 scrnaseq-0.1.2/.github/workflows/pypi-publish.yml
+-rw-r--r--   0 runner    (1001) docker     (127)     1694 2024-05-29 14:41:12.000000 scrnaseq-0.1.2/.github/workflows/pypi-test.yml
+-rw-r--r--   0 runner    (1001) docker     (127)      566 2024-05-29 14:41:12.000000 scrnaseq-0.1.2/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (127)     1336 2024-05-29 14:41:12.000000 scrnaseq-0.1.2/.pre-commit-config.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)      530 2024-05-29 14:41:12.000000 scrnaseq-0.1.2/.readthedocs.yml
+-rw-r--r--   0 runner    (1001) docker     (127)      102 2024-05-29 14:41:12.000000 scrnaseq-0.1.2/AUTHORS.md
+-rw-r--r--   0 runner    (1001) docker     (127)      115 2024-05-29 14:41:12.000000 scrnaseq-0.1.2/CHANGELOG.md
+-rw-r--r--   0 runner    (1001) docker     (127)    13490 2024-05-29 14:41:12.000000 scrnaseq-0.1.2/CONTRIBUTING.md
+-rw-r--r--   0 runner    (1001) docker     (127)     1084 2024-05-29 14:41:12.000000 scrnaseq-0.1.2/LICENSE.txt
+-rw-r--r--   0 runner    (1001) docker     (127)    13062 2024-05-29 14:45:17.789091 scrnaseq-0.1.2/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)    11937 2024-05-29 14:41:12.000000 scrnaseq-0.1.2/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-29 14:45:17.785091 scrnaseq-0.1.2/docs/
+-rw-r--r--   0 runner    (1001) docker     (127)     1154 2024-05-29 14:41:12.000000 scrnaseq-0.1.2/docs/Makefile
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-29 14:45:17.785091 scrnaseq-0.1.2/docs/_static/
+-rw-r--r--   0 runner    (1001) docker     (127)       18 2024-05-29 14:41:12.000000 scrnaseq-0.1.2/docs/_static/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (127)       71 2024-05-29 14:41:12.000000 scrnaseq-0.1.2/docs/authors.md
+-rw-r--r--   0 runner    (1001) docker     (127)       73 2024-05-29 14:41:12.000000 scrnaseq-0.1.2/docs/changelog.md
+-rw-r--r--   0 runner    (1001) docker     (127)    10906 2024-05-29 14:41:12.000000 scrnaseq-0.1.2/docs/conf.py
+-rw-r--r--   0 runner    (1001) docker     (127)       76 2024-05-29 14:41:12.000000 scrnaseq-0.1.2/docs/contributing.md
+-rw-r--r--   0 runner    (1001) docker     (127)     1248 2024-05-29 14:41:12.000000 scrnaseq-0.1.2/docs/index.md
+-rw-r--r--   0 runner    (1001) docker     (127)       66 2024-05-29 14:41:12.000000 scrnaseq-0.1.2/docs/license.md
+-rw-r--r--   0 runner    (1001) docker     (127)       70 2024-05-29 14:41:12.000000 scrnaseq-0.1.2/docs/readme.md
+-rw-r--r--   0 runner    (1001) docker     (127)      284 2024-05-29 14:41:12.000000 scrnaseq-0.1.2/docs/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      589 2024-05-29 14:41:12.000000 scrnaseq-0.1.2/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)     1416 2024-05-29 14:45:17.793091 scrnaseq-0.1.2/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)      683 2024-05-29 14:41:12.000000 scrnaseq-0.1.2/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-29 14:45:17.781091 scrnaseq-0.1.2/src/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-29 14:45:17.785091 scrnaseq-0.1.2/src/scrnaseq/
+-rw-r--r--   0 runner    (1001) docker     (127)      909 2024-05-29 14:41:12.000000 scrnaseq-0.1.2/src/scrnaseq/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4168 2024-05-29 14:41:12.000000 scrnaseq-0.1.2/src/scrnaseq/fetch_dataset.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6076 2024-05-29 14:41:12.000000 scrnaseq-0.1.2/src/scrnaseq/list_datasets.py
+-rw-r--r--   0 runner    (1001) docker     (127)      863 2024-05-29 14:41:12.000000 scrnaseq-0.1.2/src/scrnaseq/list_versions.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4435 2024-05-29 14:41:12.000000 scrnaseq-0.1.2/src/scrnaseq/polish_dataset.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4390 2024-05-29 14:41:12.000000 scrnaseq-0.1.2/src/scrnaseq/save_dataset.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3492 2024-05-29 14:41:12.000000 scrnaseq-0.1.2/src/scrnaseq/search_datasets.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2412 2024-05-29 14:41:12.000000 scrnaseq-0.1.2/src/scrnaseq/upload_dataset.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3790 2024-05-29 14:41:12.000000 scrnaseq-0.1.2/src/scrnaseq/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-29 14:45:17.789091 scrnaseq-0.1.2/src/scrnaseq.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)    13062 2024-05-29 14:45:17.000000 scrnaseq-0.1.2/src/scrnaseq.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     1096 2024-05-29 14:45:17.000000 scrnaseq-0.1.2/src/scrnaseq.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-29 14:45:17.000000 scrnaseq-0.1.2/src/scrnaseq.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-29 14:45:17.000000 scrnaseq-0.1.2/src/scrnaseq.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (127)      260 2024-05-29 14:45:17.000000 scrnaseq-0.1.2/src/scrnaseq.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        9 2024-05-29 14:45:17.000000 scrnaseq-0.1.2/src/scrnaseq.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-29 14:45:17.789091 scrnaseq-0.1.2/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)      255 2024-05-29 14:41:12.000000 scrnaseq-0.1.2/tests/conftest.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1892 2024-05-29 14:41:12.000000 scrnaseq-0.1.2/tests/test_fetch_dataset.py
+-rw-r--r--   0 runner    (1001) docker     (127)      325 2024-05-29 14:41:12.000000 scrnaseq-0.1.2/tests/test_list_dataset.py
+-rw-r--r--   0 runner    (1001) docker     (127)      459 2024-05-29 14:41:12.000000 scrnaseq-0.1.2/tests/test_list_version.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5822 2024-05-29 14:41:12.000000 scrnaseq-0.1.2/tests/test_polish_dataset.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3042 2024-05-29 14:41:12.000000 scrnaseq-0.1.2/tests/test_save_dataset.py
+-rw-r--r--   0 runner    (1001) docker     (127)      883 2024-05-29 14:41:12.000000 scrnaseq-0.1.2/tests/test_search_datasets.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4705 2024-05-29 14:41:12.000000 scrnaseq-0.1.2/tests/test_upload_dataset.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2851 2024-05-29 14:41:12.000000 scrnaseq-0.1.2/tox.ini
```

### Comparing `scrnaseq-0.1.1/.coveragerc` & `scrnaseq-0.1.2/.coveragerc`

 * *Files identical despite different names*

### Comparing `scrnaseq-0.1.1/.github/workflows/pypi-publish.yml` & `scrnaseq-0.1.2/.github/workflows/pypi-publish.yml`

 * *Files identical despite different names*

### Comparing `scrnaseq-0.1.1/.github/workflows/pypi-test.yml` & `scrnaseq-0.1.2/.github/workflows/pypi-test.yml`

 * *Files identical despite different names*

### Comparing `scrnaseq-0.1.1/.gitignore` & `scrnaseq-0.1.2/.gitignore`

 * *Files identical despite different names*

### Comparing `scrnaseq-0.1.1/.pre-commit-config.yaml` & `scrnaseq-0.1.2/.pre-commit-config.yaml`

 * *Files identical despite different names*

### Comparing `scrnaseq-0.1.1/.readthedocs.yml` & `scrnaseq-0.1.2/.readthedocs.yml`

 * *Files identical despite different names*

### Comparing `scrnaseq-0.1.1/CONTRIBUTING.md` & `scrnaseq-0.1.2/CONTRIBUTING.md`

 * *Files identical despite different names*

### Comparing `scrnaseq-0.1.1/LICENSE.txt` & `scrnaseq-0.1.2/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `scrnaseq-0.1.1/PKG-INFO` & `scrnaseq-0.1.2/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: scrnaseq
-Version: 0.1.1
+Version: 0.1.2
 Summary: Collection of Public Single-Cell RNA-Seq Datasets
 Home-page: https://github.com/biocpy/scrnaseq
 Author: Jayaram Kancherla
 Author-email: jayaram.kancherla@gmail.com
 License: MIT
 Project-URL: Documentation, https://github.com/biocpy/scrnaseq
 Platform: any
```

### Comparing `scrnaseq-0.1.1/README.md` & `scrnaseq-0.1.2/README.md`

 * *Files identical despite different names*

### Comparing `scrnaseq-0.1.1/docs/Makefile` & `scrnaseq-0.1.2/docs/Makefile`

 * *Files identical despite different names*

### Comparing `scrnaseq-0.1.1/docs/conf.py` & `scrnaseq-0.1.2/docs/conf.py`

 * *Files 2% similar despite different names*

```diff
@@ -312,10 +312,11 @@
     "biocframe": ("https://biocpy.github.io/BiocFrame", None),
     "genomicranges": ("https://biocpy.github.io/GenomicRanges", None),
     "singlecellexperiment": ("https://biocpy.github.io/SingleCellExperiment", None),
     "summarizedexperiment": ("https://biocpy.github.io/SummarizedExperiment", None),
     "gypsum_client": ("https://artifactdb.github.io/gypsum-py", None),
     "delayedarray": ("https://biocpy.github.io/DelayedArray", None),
     "dolomite_base": ("https://artifactdb.github.io/dolomite-base", None),
+    "anndata": ("https://anndata.readthedocs.io/en/latest/", None),
 }
 
 print(f"loading configurations for {project} {version} ...", file=sys.stderr)
```

### Comparing `scrnaseq-0.1.1/docs/index.md` & `scrnaseq-0.1.2/docs/index.md`

 * *Files identical despite different names*

### Comparing `scrnaseq-0.1.1/pyproject.toml` & `scrnaseq-0.1.2/pyproject.toml`

 * *Files identical despite different names*

### Comparing `scrnaseq-0.1.1/setup.cfg` & `scrnaseq-0.1.2/setup.cfg`

 * *Files identical despite different names*

### Comparing `scrnaseq-0.1.1/setup.py` & `scrnaseq-0.1.2/setup.py`

 * *Files identical despite different names*

### Comparing `scrnaseq-0.1.1/src/scrnaseq/__init__.py` & `scrnaseq-0.1.2/src/scrnaseq/__init__.py`

 * *Files identical despite different names*

### Comparing `scrnaseq-0.1.1/src/scrnaseq/fetch_dataset.py` & `scrnaseq-0.1.2/src/scrnaseq/fetch_dataset.py`

 * *Files 2% similar despite different names*

```diff
@@ -79,16 +79,14 @@
 
     Returns:
         The dataset as a
         :py:class:`~summarizedexperiment.SummarizedExperiment.SummarizedExperiment`
         or one of its subclasses.
     """
 
-    cache_dir = cache_directory(cache_dir)
-
     version_path = save_version(
         package, name, version, cache_dir=cache_dir, overwrite=overwrite
     )
     obj_path = (
         version_path if path is None else os.path.join(version_path, path.rstrip("/"))
     )
```

### Comparing `scrnaseq-0.1.1/src/scrnaseq/list_datasets.py` & `scrnaseq-0.1.2/src/scrnaseq/list_datasets.py`

 * *Files identical despite different names*

### Comparing `scrnaseq-0.1.1/src/scrnaseq/list_versions.py` & `scrnaseq-0.1.2/src/scrnaseq/list_versions.py`

 * *Files identical despite different names*

### Comparing `scrnaseq-0.1.1/src/scrnaseq/polish_dataset.py` & `scrnaseq-0.1.2/src/scrnaseq/polish_dataset.py`

 * *Files identical despite different names*

### Comparing `scrnaseq-0.1.1/src/scrnaseq/save_dataset.py` & `scrnaseq-0.1.2/src/scrnaseq/save_dataset.py`

 * *Files 7% similar despite different names*

```diff
@@ -3,14 +3,15 @@
 import shutil
 from functools import singledispatch
 from typing import Any
 
 import dolomite_base as dl
 from gypsum_client import fetch_metadata_schema, validate_metadata
 from singlecellexperiment import SingleCellExperiment
+from summarizedexperiment import SummarizedExperiment
 
 from .utils import format_object_metadata
 
 __author__ = "Jayaram Kancherla"
 __copyright__ = "Jayaram Kancherla"
 __license__ = "MIT"
 
@@ -18,15 +19,17 @@
 @singledispatch
 def save_dataset(x: Any, path, metadata):
     """Save a dataset to disk.
 
     Args:
         x:
             An object containing single-cell data.
-            May be a derivative of SummarizedExperiment or AnnData.
+            May be a derivative of
+            :py:class:`~summarizedexperiment.SummarizedExperiment.SummarizedExperiment`
+            or :py:class:`~anndata.AnnData`.
 
         path:
             Path to a new directory to save the dataset.
 
         metadata:
             Dictionary containing the metadata for this dataset.
             see the schema returned by
@@ -76,21 +79,19 @@
             scrnaseq.save_dataset(sce, cache_dir, meta)
     """
     raise NotImplementedError(
         f"'save_dataset' is not supported for objects of class: {type(x)}"
     )
 
 
-@save_dataset.register
-def save_dataset_sce(x: SingleCellExperiment, path: str, metadata: dict):
-    """Save :py:class:`~singlecellexperiment.SingleCellExperiment.SingleCellExperiment` to disk."""
+def _save_se(x, path, metadata):
     schema = fetch_metadata_schema()
 
     if "bioconductor_version" not in metadata:
-        metadata["bioconductor_version"] = "3.14"  # current release
+        metadata["bioconductor_version"] = "3.19"  # current release
 
     validate_metadata(metadata, schema)
 
     if os.path.exists(path):
         shutil.rmtree(path)
 
     dl.save_object(x, path, reloaded_array_reuse_mode="symlink")
@@ -105,15 +106,25 @@
 
     # Second validation with the takane metadata.
     contents = json.dumps(metadata, indent=4)
     validate_metadata(json.loads(contents), schema=schema)
     with open(os.path.join(path, "_bioconductor.json"), "w") as f:
         f.write(contents)
 
-    return
+
+@save_dataset.register
+def save_dataset_sce(x: SingleCellExperiment, path: str, metadata: dict):
+    """Save :py:class:`~singlecellexperiment.SingleCellExperiment.SingleCellExperiment` to disk."""
+    return _save_se(x, path, metadata)
+
+
+@save_dataset.register
+def save_dataset_se(x: SummarizedExperiment, path: str, metadata: dict):
+    """Save :py:class:`~summarizedexperiment.SummarizedExperiment.SummarizedExperiment` to disk."""
+    return _save_se(x, path, metadata)
 
 
 has_anndata = False
 try:
     import anndata
 
     has_anndata = True
```

### Comparing `scrnaseq-0.1.1/src/scrnaseq/search_datasets.py` & `scrnaseq-0.1.2/src/scrnaseq/search_datasets.py`

 * *Files identical despite different names*

### Comparing `scrnaseq-0.1.1/src/scrnaseq/upload_dataset.py` & `scrnaseq-0.1.2/src/scrnaseq/upload_dataset.py`

 * *Files identical despite different names*

### Comparing `scrnaseq-0.1.1/src/scrnaseq/utils.py` & `scrnaseq-0.1.2/src/scrnaseq/utils.py`

 * *Files identical despite different names*

### Comparing `scrnaseq-0.1.1/src/scrnaseq.egg-info/PKG-INFO` & `scrnaseq-0.1.2/src/scrnaseq.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: scrnaseq
-Version: 0.1.1
+Version: 0.1.2
 Summary: Collection of Public Single-Cell RNA-Seq Datasets
 Home-page: https://github.com/biocpy/scrnaseq
 Author: Jayaram Kancherla
 Author-email: jayaram.kancherla@gmail.com
 License: MIT
 Project-URL: Documentation, https://github.com/biocpy/scrnaseq
 Platform: any
```

### Comparing `scrnaseq-0.1.1/src/scrnaseq.egg-info/SOURCES.txt` & `scrnaseq-0.1.2/src/scrnaseq.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `scrnaseq-0.1.1/tests/test_fetch_dataset.py` & `scrnaseq-0.1.2/tests/test_fetch_dataset.py`

 * *Files 14% similar despite different names*

```diff
@@ -31,14 +31,15 @@
 
     alt_exps = sce.get_alternative_experiments()
     for altname, alt in alt_exps.items():
         alt_exp_ass = alt.get_assays()
         assert all(isinstance(a, (np.ndarray)) for _, a in alt_exp_ass.items())
 
 
+@pytest.mark.skip("takes too long")
 def test_fetch_dataset_realizes_reduced_dimensions():
     sce = fetch_dataset("aztekin-tail-2019", "2023-12-14", realize_reduced_dims=False)
     red_dim = sce.get_reduced_dims()
     assert all(isinstance(a, ReloadedArray) for _, a in red_dim.items())
 
     sce = fetch_dataset("aztekin-tail-2019", "2023-12-14", realize_reduced_dims=True)
     red_dim = sce.get_reduced_dims()
```

### Comparing `scrnaseq-0.1.1/tests/test_polish_dataset.py` & `scrnaseq-0.1.2/tests/test_polish_dataset.py`

 * *Files 2% similar despite different names*

```diff
@@ -164,14 +164,15 @@
 
     y = polish_dataset(sce0, forbid_nested_altexp=False)
     assert (
         y.get_alternative_experiment_names() == sce0.get_alternative_experiment_names()
     )
 
 
+@pytest.mark.skip("takes too long")
 def test_polish_existing_dataset():
     sce = fetch_dataset("zeisel-brain-2015", "2023-12-14")
 
     y = polish_dataset(sce)
 
     assert y.shape == sce.shape
     assert type(y.assays["counts"]) != type(sce.assays["counts"])
```

### Comparing `scrnaseq-0.1.1/tests/test_save_dataset.py` & `scrnaseq-0.1.2/tests/test_save_dataset.py`

 * *Files 8% similar despite different names*

```diff
@@ -40,15 +40,15 @@
     assert isinstance(roundtrip.get_assays()["counts"], ReloadedArray)
     assert isinstance(sce.get_assays()["counts"], ReloadedArray)
 
     # Load and check the metadata
     with open(os.path.join(tmp, "_bioconductor.json")) as f:
         saved_meta = json.load(f)
 
-    assert saved_meta["bioconductor_version"] == "3.14"  # Placeholder version
+    assert saved_meta["bioconductor_version"] == "3.19"
 
     # Test validation failure
     meta["title"] = 1234
     with pytest.raises(Exception):
         save_dataset(sce, tmp, meta)
 
     shutil.rmtree(tmp)
@@ -86,15 +86,15 @@
         adata.layers["counts"],
     )
 
     # Load and check the metadata
     with open(os.path.join(tmp, "_bioconductor.json")) as f:
         saved_meta = json.load(f)
 
-    assert saved_meta["bioconductor_version"] == "3.14"  # Placeholder version
+    assert saved_meta["bioconductor_version"] == "3.19"
 
     # Test validation failure
     meta["title"] = 1234
     with pytest.raises(Exception):
         save_dataset(adata, tmp, meta)
 
     shutil.rmtree(tmp)
```

### Comparing `scrnaseq-0.1.1/tests/test_search_datasets.py` & `scrnaseq-0.1.2/tests/test_search_datasets.py`

 * *Files identical despite different names*

### Comparing `scrnaseq-0.1.1/tests/test_upload_dataset.py` & `scrnaseq-0.1.2/tests/test_upload_dataset.py`

 * *Files identical despite different names*

### Comparing `scrnaseq-0.1.1/tox.ini` & `scrnaseq-0.1.2/tox.ini`

 * *Files identical despite different names*

