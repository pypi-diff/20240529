# Comparing `tmp/haniwers-0.15.1.tar.gz` & `tmp/haniwers-0.15.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "haniwers-0.15.1.tar", max compression
+gzip compressed data, was "haniwers-0.15.2.tar", max compression
```

## Comparing `haniwers-0.15.1.tar` & `haniwers-0.15.2.tar`

### file list

```diff
@@ -1,13 +1,13 @@
--rw-r--r--   0        0        0     1072 2023-05-17 08:20:30.907111 haniwers-0.15.1/LICENSE
--rw-r--r--   0        0        0     6942 2024-05-26 12:45:22.524830 haniwers-0.15.1/README.md
--rw-r--r--   0        0        0       23 2024-05-28 01:21:08.433794 haniwers-0.15.1/haniwers/__init__.py
--rw-r--r--   0        0        0    12494 2024-05-28 01:19:45.569454 haniwers-0.15.1/haniwers/cli.py
--rw-r--r--   0        0        0    16792 2024-05-27 02:58:41.796496 haniwers-0.15.1/haniwers/config.py
--rw-r--r--   0        0        0    22568 2024-05-28 01:19:45.569719 haniwers-0.15.1/haniwers/daq.py
--rw-r--r--   0        0        0     9820 2024-05-27 02:58:41.797488 haniwers-0.15.1/haniwers/dataset.py
--rw-r--r--   0        0        0     2618 2024-05-27 02:58:41.797813 haniwers-0.15.1/haniwers/mimic.py
--rw-r--r--   0        0        0      774 2024-05-22 14:19:28.812968 haniwers-0.15.1/haniwers/postprocess.py
--rw-r--r--   0        0        0    12810 2024-05-23 11:22:23.101251 haniwers-0.15.1/haniwers/preprocess.py
--rw-r--r--   0        0        0     8512 2024-05-27 02:58:41.798249 haniwers-0.15.1/haniwers/threshold.py
--rw-r--r--   0        0        0     1482 2024-05-28 01:21:08.444544 haniwers-0.15.1/pyproject.toml
--rw-r--r--   0        0        0     8398 1970-01-01 00:00:00.000000 haniwers-0.15.1/PKG-INFO
+-rw-r--r--   0        0        0     1072 2023-05-17 08:20:30.907111 haniwers-0.15.2/LICENSE
+-rw-r--r--   0        0        0     6942 2024-05-26 12:45:22.524830 haniwers-0.15.2/README.md
+-rw-r--r--   0        0        0       23 2024-05-28 22:00:03.530327 haniwers-0.15.2/haniwers/__init__.py
+-rw-r--r--   0        0        0    12494 2024-05-28 01:19:45.569454 haniwers-0.15.2/haniwers/cli.py
+-rw-r--r--   0        0        0    16792 2024-05-27 02:58:41.796496 haniwers-0.15.2/haniwers/config.py
+-rw-r--r--   0        0        0    22568 2024-05-28 01:19:45.569719 haniwers-0.15.2/haniwers/daq.py
+-rw-r--r--   0        0        0     9820 2024-05-27 02:58:41.797488 haniwers-0.15.2/haniwers/dataset.py
+-rw-r--r--   0        0        0     2618 2024-05-27 02:58:41.797813 haniwers-0.15.2/haniwers/mimic.py
+-rw-r--r--   0        0        0      774 2024-05-22 14:19:28.812968 haniwers-0.15.2/haniwers/postprocess.py
+-rw-r--r--   0        0        0    12810 2024-05-23 11:22:23.101251 haniwers-0.15.2/haniwers/preprocess.py
+-rw-r--r--   0        0        0     8512 2024-05-27 02:58:41.798249 haniwers-0.15.2/haniwers/threshold.py
+-rw-r--r--   0        0        0     1506 2024-05-28 22:00:03.531977 haniwers-0.15.2/pyproject.toml
+-rw-r--r--   0        0        0     8443 1970-01-01 00:00:00.000000 haniwers-0.15.2/PKG-INFO
```

### Comparing `haniwers-0.15.1/LICENSE` & `haniwers-0.15.2/LICENSE`

 * *Files identical despite different names*

### Comparing `haniwers-0.15.1/README.md` & `haniwers-0.15.2/README.md`

 * *Files identical despite different names*

### Comparing `haniwers-0.15.1/haniwers/cli.py` & `haniwers-0.15.2/haniwers/cli.py`

 * *Files identical despite different names*

### Comparing `haniwers-0.15.1/haniwers/config.py` & `haniwers-0.15.2/haniwers/config.py`

 * *Files identical despite different names*

### Comparing `haniwers-0.15.1/haniwers/daq.py` & `haniwers-0.15.2/haniwers/daq.py`

 * *Files identical despite different names*

### Comparing `haniwers-0.15.1/haniwers/dataset.py` & `haniwers-0.15.2/haniwers/dataset.py`

 * *Files identical despite different names*

### Comparing `haniwers-0.15.1/haniwers/mimic.py` & `haniwers-0.15.2/haniwers/mimic.py`

 * *Files identical despite different names*

### Comparing `haniwers-0.15.1/haniwers/postprocess.py` & `haniwers-0.15.2/haniwers/postprocess.py`

 * *Files identical despite different names*

### Comparing `haniwers-0.15.1/haniwers/preprocess.py` & `haniwers-0.15.2/haniwers/preprocess.py`

 * *Files identical despite different names*

### Comparing `haniwers-0.15.1/haniwers/threshold.py` & `haniwers-0.15.2/haniwers/threshold.py`

 * *Files identical despite different names*

### Comparing `haniwers-0.15.1/pyproject.toml` & `haniwers-0.15.2/pyproject.toml`

 * *Files 5% similar despite different names*

```diff
@@ -1,20 +1,20 @@
 [tool]
 [tool.commitizen]
 name = "cz_conventional_commits"
-version = "0.15.1"
+version = "0.15.2"
 tag_format = "$version"
 version_files = [
     "pyproject.toml:version",
     "haniwers/__init__.py:__version__",
 ]
 
 [tool.poetry]
 name = "haniwers"
-version = "0.15.1"
+version = "0.15.2"
 description = "Analysis tool for TanQ/FunQ project"
 authors = ["Shota Takahashi (KMI) <shotakaha@kmi.nagoya-u.ac.jp>"]
 license = "MIT"
 readme = "README.md"
 homepage = "https://qumasan.gitlab.io/haniwers/docs/"
 repository = "https://gitlab.com/qumasan/haniwers/"
 keywords = ["muon"]
@@ -39,14 +39,15 @@
 polars = "^0.20.4"
 altair = "^5.2.0"
 vl-convert-python = "^1.1.0"
 typer = "^0.12.0"
 pydantic = "^2.7.1"
 matplotlib = "^3.8.4"
 hvplot = "^0.10.0"
+platformdirs = "^4.2.2"
 
 [tool.poetry.group.docs.dependencies]
 sphinx-book-theme = "^1.0.1"
 sphinx-copybutton = "^0.5.2"
 myst-parser = "^2.0.0"
 jupyterlab-myst = "^2.0.2"
 mystmd = "^1.2.3"
```

### Comparing `haniwers-0.15.1/PKG-INFO` & `haniwers-0.15.2/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: haniwers
-Version: 0.15.1
+Version: 0.15.2
 Summary: Analysis tool for TanQ/FunQ project
 Home-page: https://qumasan.gitlab.io/haniwers/docs/
 License: MIT
 Keywords: muon
 Author: Shota Takahashi (KMI)
 Author-email: shotakaha@kmi.nagoya-u.ac.jp
 Requires-Python: >=3.9,<3.13
@@ -19,14 +19,15 @@
 Requires-Dist: deprecated (>=1.2.14,<2.0.0)
 Requires-Dist: hvplot (>=0.10.0,<0.11.0)
 Requires-Dist: icecream (>=2.1.2,<3.0.0)
 Requires-Dist: loguru (>=0.7.0,<0.8.0)
 Requires-Dist: matplotlib (>=3.8.4,<4.0.0)
 Requires-Dist: pandas (>=2.0.3,<3.0.0)
 Requires-Dist: pendulum (>=3.0.0,<4.0.0)
+Requires-Dist: platformdirs (>=4.2.2,<5.0.0)
 Requires-Dist: plotly (>=5.7.0,<6.0.0)
 Requires-Dist: polars (>=0.20.4,<0.21.0)
 Requires-Dist: pyarrow (>=15.0.2,<16.0.0)
 Requires-Dist: pydantic (>=2.7.1,<3.0.0)
 Requires-Dist: pyserial (>=3.5,<4.0)
 Requires-Dist: scipy (>=1.11.1,<2.0.0)
 Requires-Dist: tomli (>=2.0.1,<3.0.0)
```

