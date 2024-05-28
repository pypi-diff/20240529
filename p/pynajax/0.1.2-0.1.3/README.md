# Comparing `tmp/pynajax-0.1.2.tar.gz` & `tmp/pynajax-0.1.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pynajax-0.1.2.tar", last modified: Mon May 13 16:58:31 2024, max compression
+gzip compressed data, was "pynajax-0.1.3.tar", last modified: Tue May 28 22:04:33 2024, max compression
```

## Comparing `pynajax-0.1.2.tar` & `pynajax-0.1.3.tar`

### file list

```diff
@@ -1,48 +1,48 @@
-drwxrwxr-x   0 gviejo    (2224) gviejo    (2224)        0 2024-05-13 16:58:31.385098 pynajax-0.1.2/
-drwxrwxr-x   0 gviejo    (2224) gviejo    (2224)        0 2024-05-13 16:58:31.157584 pynajax-0.1.2/.github/
-drwxrwxr-x   0 gviejo    (2224) gviejo    (2224)        0 2024-05-13 16:58:31.204484 pynajax-0.1.2/.github/workflows/
--rw-rw-r--   0 gviejo    (2224) gviejo    (2224)     1416 2024-05-13 16:44:00.000000 pynajax-0.1.2/.github/workflows/ci.yml
--rw-rw-r--   0 gviejo    (2224) gviejo    (2224)     3077 2024-04-03 20:32:36.000000 pynajax-0.1.2/.gitignore
--rw-rw-r--   0 gviejo    (2224) gviejo    (2224)     1069 2024-04-03 20:32:36.000000 pynajax-0.1.2/LICENSE
--rw-r--r--   0 gviejo    (2224) gviejo    (2224)     4537 2024-05-13 16:58:31.380343 pynajax-0.1.2/PKG-INFO
--rw-rw-r--   0 gviejo    (2224) gviejo    (2224)     1988 2024-05-13 16:44:08.000000 pynajax-0.1.2/README.md
-drwxrwxr-x   0 gviejo    (2224) gviejo    (2224)        0 2024-05-13 16:58:31.222247 pynajax-0.1.2/docs/
-drwxrwxr-x   0 gviejo    (2224) gviejo    (2224)        0 2024-05-13 16:58:31.250811 pynajax-0.1.2/docs/examples/
--rw-rw-r--   0 gviejo    (2224) gviejo    (2224)      710 2024-05-08 02:28:34.000000 pynajax-0.1.2/docs/examples/README.md
--rw-rw-r--   0 gviejo    (2224) gviejo    (2224)     1707 2024-05-08 02:28:34.000000 pynajax-0.1.2/docs/examples/plot_benchmark_bin_average.py
--rw-rw-r--   0 gviejo    (2224) gviejo    (2224)     1524 2024-05-08 02:28:34.000000 pynajax-0.1.2/docs/examples/plot_benchmark_convolve.py
--rw-rw-r--   0 gviejo    (2224) gviejo    (2224)     1940 2024-05-08 14:38:55.000000 pynajax-0.1.2/docs/examples/plot_benchmark_event_trigger_average.py
--rw-rw-r--   0 gviejo    (2224) gviejo    (2224)     1610 2024-05-08 02:28:34.000000 pynajax-0.1.2/docs/examples/plot_benchmark_threshold.py
--rw-rw-r--   0 gviejo    (2224) gviejo    (2224)      821 2024-05-08 02:28:34.000000 pynajax-0.1.2/docs/gallery_conf.py
--rw-rw-r--   0 gviejo    (2224) gviejo    (2224)     1762 2024-04-03 20:32:36.000000 pynajax-0.1.2/docs/gen_ref_pages.py
-drwxrwxr-x   0 gviejo    (2224) gviejo    (2224)        0 2024-05-13 16:58:31.256562 pynajax-0.1.2/docs/images/
--rw-rw-r--   0 gviejo    (2224) gviejo    (2224)    38967 2024-05-08 14:38:55.000000 pynajax-0.1.2/docs/images/convolve_benchmark.png
--rw-rw-r--   0 gviejo    (2224) gviejo    (2224)     1977 2024-05-13 16:44:08.000000 pynajax-0.1.2/docs/index.md
-drwxrwxr-x   0 gviejo    (2224) gviejo    (2224)        0 2024-05-13 16:58:31.262682 pynajax-0.1.2/docs/javascripts/
--rw-rw-r--   0 gviejo    (2224) gviejo    (2224)      384 2024-04-03 20:32:36.000000 pynajax-0.1.2/docs/javascripts/katex.js
--rw-rw-r--   0 gviejo    (2224) gviejo    (2224)     2012 2024-05-08 02:28:34.000000 pynajax-0.1.2/mkdocs.yml
--rw-rw-r--   0 gviejo    (2224) gviejo    (2224)     1407 2024-05-08 02:28:34.000000 pynajax-0.1.2/noxfile.py
--rw-rw-r--   0 gviejo    (2224) gviejo    (2224)     3194 2024-05-13 16:58:08.000000 pynajax-0.1.2/pyproject.toml
--rw-rw-r--   0 gviejo    (2224) gviejo    (2224)       38 2024-05-13 16:58:31.386071 pynajax-0.1.2/setup.cfg
-drwxrwxr-x   0 gviejo    (2224) gviejo    (2224)        0 2024-05-13 16:58:31.168317 pynajax-0.1.2/src/
-drwxrwxr-x   0 gviejo    (2224) gviejo    (2224)        0 2024-05-13 16:58:31.295817 pynajax-0.1.2/src/pynajax/
--rw-rw-r--   0 gviejo    (2224) gviejo    (2224)      112 2024-05-13 16:58:08.000000 pynajax-0.1.2/src/pynajax/__init__.py
--rw-rw-r--   0 gviejo    (2224) gviejo    (2224)     5592 2024-05-08 02:28:34.000000 pynajax-0.1.2/src/pynajax/jax_core_bin_average.py
--rw-rw-r--   0 gviejo    (2224) gviejo    (2224)     6148 2024-05-08 02:28:34.000000 pynajax-0.1.2/src/pynajax/jax_core_convolve.py
--rw-rw-r--   0 gviejo    (2224) gviejo    (2224)     1437 2024-05-08 02:28:34.000000 pynajax-0.1.2/src/pynajax/jax_core_threshold.py
--rw-rw-r--   0 gviejo    (2224) gviejo    (2224)     6928 2024-05-13 16:44:00.000000 pynajax-0.1.2/src/pynajax/jax_process_perievent.py
--rw-rw-r--   0 gviejo    (2224) gviejo    (2224)     8469 2024-05-08 02:28:34.000000 pynajax-0.1.2/src/pynajax/utils.py
-drwxrwxr-x   0 gviejo    (2224) gviejo    (2224)        0 2024-05-13 16:58:31.368364 pynajax-0.1.2/src/pynajax.egg-info/
--rw-r--r--   0 gviejo    (2224) gviejo    (2224)     4537 2024-05-13 16:58:31.302780 pynajax-0.1.2/src/pynajax.egg-info/PKG-INFO
--rw-rw-r--   0 gviejo    (2224) gviejo    (2224)      948 2024-05-13 16:58:31.000000 pynajax-0.1.2/src/pynajax.egg-info/SOURCES.txt
--rw-rw-r--   0 gviejo    (2224) gviejo    (2224)        1 2024-05-13 16:58:31.000000 pynajax-0.1.2/src/pynajax.egg-info/dependency_links.txt
--rw-rw-r--   0 gviejo    (2224) gviejo    (2224)      282 2024-05-13 16:58:31.000000 pynajax-0.1.2/src/pynajax.egg-info/requires.txt
--rw-rw-r--   0 gviejo    (2224) gviejo    (2224)        8 2024-05-13 16:58:31.000000 pynajax-0.1.2/src/pynajax.egg-info/top_level.txt
-drwxrwxr-x   0 gviejo    (2224) gviejo    (2224)        0 2024-05-13 16:58:31.362108 pynajax-0.1.2/tests/
--rw-rw-r--   0 gviejo    (2224) gviejo    (2224)       18 2024-05-08 02:28:34.000000 pynajax-0.1.2/tests/__init__.py
--rw-rw-r--   0 gviejo    (2224) gviejo    (2224)      546 2024-05-08 02:28:34.000000 pynajax-0.1.2/tests/conftest.py
--rw-rw-r--   0 gviejo    (2224) gviejo    (2224)     1438 2024-05-08 02:28:34.000000 pynajax-0.1.2/tests/mock.py
--rw-rw-r--   0 gviejo    (2224) gviejo    (2224)     5237 2024-05-08 02:28:34.000000 pynajax-0.1.2/tests/test_jax_core_convolve.py
--rw-rw-r--   0 gviejo    (2224) gviejo    (2224)     5256 2024-05-13 16:44:00.000000 pynajax-0.1.2/tests/test_jax_core_perievent.py
--rw-rw-r--   0 gviejo    (2224) gviejo    (2224)    16141 2024-05-08 02:28:34.000000 pynajax-0.1.2/tests/test_jax_numpy_compatibility.py
--rw-rw-r--   0 gviejo    (2224) gviejo    (2224)      111 2024-05-08 02:28:34.000000 pynajax-0.1.2/tests/test_pynapple.py
+drwxrwxr-x   0 gviejo    (2224) gviejo    (2224)        0 2024-05-28 22:04:33.402620 pynajax-0.1.3/
+drwxrwxr-x   0 gviejo    (2224) gviejo    (2224)        0 2024-05-28 22:04:33.136890 pynajax-0.1.3/.github/
+drwxrwxr-x   0 gviejo    (2224) gviejo    (2224)        0 2024-05-28 22:04:33.188322 pynajax-0.1.3/.github/workflows/
+-rw-rw-r--   0 gviejo    (2224) gviejo    (2224)     1416 2024-05-13 16:44:00.000000 pynajax-0.1.3/.github/workflows/ci.yml
+-rw-rw-r--   0 gviejo    (2224) gviejo    (2224)     3077 2024-04-03 20:32:36.000000 pynajax-0.1.3/.gitignore
+-rw-rw-r--   0 gviejo    (2224) gviejo    (2224)     1069 2024-04-03 20:32:36.000000 pynajax-0.1.3/LICENSE
+-rw-r--r--   0 gviejo    (2224) gviejo    (2224)     4537 2024-05-28 22:04:33.397173 pynajax-0.1.3/PKG-INFO
+-rw-rw-r--   0 gviejo    (2224) gviejo    (2224)     1988 2024-05-13 16:44:08.000000 pynajax-0.1.3/README.md
+drwxrwxr-x   0 gviejo    (2224) gviejo    (2224)        0 2024-05-28 22:04:33.205069 pynajax-0.1.3/docs/
+drwxrwxr-x   0 gviejo    (2224) gviejo    (2224)        0 2024-05-28 22:04:33.262842 pynajax-0.1.3/docs/examples/
+-rw-rw-r--   0 gviejo    (2224) gviejo    (2224)      710 2024-05-08 02:28:34.000000 pynajax-0.1.3/docs/examples/README.md
+-rw-rw-r--   0 gviejo    (2224) gviejo    (2224)     1707 2024-05-08 02:28:34.000000 pynajax-0.1.3/docs/examples/plot_benchmark_bin_average.py
+-rw-rw-r--   0 gviejo    (2224) gviejo    (2224)     1524 2024-05-08 02:28:34.000000 pynajax-0.1.3/docs/examples/plot_benchmark_convolve.py
+-rw-rw-r--   0 gviejo    (2224) gviejo    (2224)     1940 2024-05-08 14:38:55.000000 pynajax-0.1.3/docs/examples/plot_benchmark_event_trigger_average.py
+-rw-rw-r--   0 gviejo    (2224) gviejo    (2224)     1610 2024-05-08 02:28:34.000000 pynajax-0.1.3/docs/examples/plot_benchmark_threshold.py
+-rw-rw-r--   0 gviejo    (2224) gviejo    (2224)      821 2024-05-08 02:28:34.000000 pynajax-0.1.3/docs/gallery_conf.py
+-rw-rw-r--   0 gviejo    (2224) gviejo    (2224)     1762 2024-04-03 20:32:36.000000 pynajax-0.1.3/docs/gen_ref_pages.py
+drwxrwxr-x   0 gviejo    (2224) gviejo    (2224)        0 2024-05-28 22:04:33.268838 pynajax-0.1.3/docs/images/
+-rw-rw-r--   0 gviejo    (2224) gviejo    (2224)    38967 2024-05-08 14:38:55.000000 pynajax-0.1.3/docs/images/convolve_benchmark.png
+-rw-rw-r--   0 gviejo    (2224) gviejo    (2224)     1977 2024-05-13 16:44:08.000000 pynajax-0.1.3/docs/index.md
+drwxrwxr-x   0 gviejo    (2224) gviejo    (2224)        0 2024-05-28 22:04:33.275881 pynajax-0.1.3/docs/javascripts/
+-rw-rw-r--   0 gviejo    (2224) gviejo    (2224)      384 2024-04-03 20:32:36.000000 pynajax-0.1.3/docs/javascripts/katex.js
+-rw-rw-r--   0 gviejo    (2224) gviejo    (2224)     2012 2024-05-08 02:28:34.000000 pynajax-0.1.3/mkdocs.yml
+-rw-rw-r--   0 gviejo    (2224) gviejo    (2224)     1407 2024-05-28 18:50:40.000000 pynajax-0.1.3/noxfile.py
+-rw-rw-r--   0 gviejo    (2224) gviejo    (2224)     3194 2024-05-28 22:04:12.000000 pynajax-0.1.3/pyproject.toml
+-rw-rw-r--   0 gviejo    (2224) gviejo    (2224)       38 2024-05-28 22:04:33.403717 pynajax-0.1.3/setup.cfg
+drwxrwxr-x   0 gviejo    (2224) gviejo    (2224)        0 2024-05-28 22:04:33.148709 pynajax-0.1.3/src/
+drwxrwxr-x   0 gviejo    (2224) gviejo    (2224)        0 2024-05-28 22:04:33.310344 pynajax-0.1.3/src/pynajax/
+-rw-rw-r--   0 gviejo    (2224) gviejo    (2224)      112 2024-05-28 22:04:12.000000 pynajax-0.1.3/src/pynajax/__init__.py
+-rw-rw-r--   0 gviejo    (2224) gviejo    (2224)     5686 2024-05-28 22:04:12.000000 pynajax-0.1.3/src/pynajax/jax_core_bin_average.py
+-rw-rw-r--   0 gviejo    (2224) gviejo    (2224)     6243 2024-05-28 22:04:12.000000 pynajax-0.1.3/src/pynajax/jax_core_convolve.py
+-rw-rw-r--   0 gviejo    (2224) gviejo    (2224)     1531 2024-05-28 22:04:12.000000 pynajax-0.1.3/src/pynajax/jax_core_threshold.py
+-rw-rw-r--   0 gviejo    (2224) gviejo    (2224)     7023 2024-05-28 22:04:12.000000 pynajax-0.1.3/src/pynajax/jax_process_perievent.py
+-rw-rw-r--   0 gviejo    (2224) gviejo    (2224)     8469 2024-05-08 02:28:34.000000 pynajax-0.1.3/src/pynajax/utils.py
+drwxrwxr-x   0 gviejo    (2224) gviejo    (2224)        0 2024-05-28 22:04:33.384726 pynajax-0.1.3/src/pynajax.egg-info/
+-rw-r--r--   0 gviejo    (2224) gviejo    (2224)     4537 2024-05-28 22:04:33.317265 pynajax-0.1.3/src/pynajax.egg-info/PKG-INFO
+-rw-rw-r--   0 gviejo    (2224) gviejo    (2224)      948 2024-05-28 22:04:33.000000 pynajax-0.1.3/src/pynajax.egg-info/SOURCES.txt
+-rw-rw-r--   0 gviejo    (2224) gviejo    (2224)        1 2024-05-28 22:04:33.000000 pynajax-0.1.3/src/pynajax.egg-info/dependency_links.txt
+-rw-rw-r--   0 gviejo    (2224) gviejo    (2224)      282 2024-05-28 22:04:33.000000 pynajax-0.1.3/src/pynajax.egg-info/requires.txt
+-rw-rw-r--   0 gviejo    (2224) gviejo    (2224)        8 2024-05-28 22:04:33.000000 pynajax-0.1.3/src/pynajax.egg-info/top_level.txt
+drwxrwxr-x   0 gviejo    (2224) gviejo    (2224)        0 2024-05-28 22:04:33.378542 pynajax-0.1.3/tests/
+-rw-rw-r--   0 gviejo    (2224) gviejo    (2224)       18 2024-05-08 02:28:34.000000 pynajax-0.1.3/tests/__init__.py
+-rw-rw-r--   0 gviejo    (2224) gviejo    (2224)      546 2024-05-28 18:50:52.000000 pynajax-0.1.3/tests/conftest.py
+-rw-rw-r--   0 gviejo    (2224) gviejo    (2224)     1438 2024-05-08 02:28:34.000000 pynajax-0.1.3/tests/mock.py
+-rw-rw-r--   0 gviejo    (2224) gviejo    (2224)     5237 2024-05-08 02:28:34.000000 pynajax-0.1.3/tests/test_jax_core_convolve.py
+-rw-rw-r--   0 gviejo    (2224) gviejo    (2224)     5256 2024-05-13 16:44:00.000000 pynajax-0.1.3/tests/test_jax_core_perievent.py
+-rw-rw-r--   0 gviejo    (2224) gviejo    (2224)    16141 2024-05-08 02:28:34.000000 pynajax-0.1.3/tests/test_jax_numpy_compatibility.py
+-rw-rw-r--   0 gviejo    (2224) gviejo    (2224)      111 2024-05-08 02:28:34.000000 pynajax-0.1.3/tests/test_pynapple.py
```

### Comparing `pynajax-0.1.2/.github/workflows/ci.yml` & `pynajax-0.1.3/.github/workflows/ci.yml`

 * *Files identical despite different names*

### Comparing `pynajax-0.1.2/.gitignore` & `pynajax-0.1.3/.gitignore`

 * *Files identical despite different names*

### Comparing `pynajax-0.1.2/LICENSE` & `pynajax-0.1.3/LICENSE`

 * *Files identical despite different names*

### Comparing `pynajax-0.1.2/PKG-INFO` & `pynajax-0.1.3/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pynajax
-Version: 0.1.2
+Version: 0.1.3
 Summary: A JAX backend for pynapple.
 Author: pynajax authors
 License: MIT License
         
         Copyright (c) 2024 pynapple-org
         
         Permission is hereby granted, free of charge, to any person obtaining a copy
```

### Comparing `pynajax-0.1.2/README.md` & `pynajax-0.1.3/README.md`

 * *Files identical despite different names*

### Comparing `pynajax-0.1.2/docs/examples/README.md` & `pynajax-0.1.3/docs/examples/README.md`

 * *Files identical despite different names*

### Comparing `pynajax-0.1.2/docs/examples/plot_benchmark_bin_average.py` & `pynajax-0.1.3/docs/examples/plot_benchmark_bin_average.py`

 * *Files identical despite different names*

### Comparing `pynajax-0.1.2/docs/examples/plot_benchmark_convolve.py` & `pynajax-0.1.3/docs/examples/plot_benchmark_convolve.py`

 * *Files identical despite different names*

### Comparing `pynajax-0.1.2/docs/examples/plot_benchmark_event_trigger_average.py` & `pynajax-0.1.3/docs/examples/plot_benchmark_event_trigger_average.py`

 * *Files identical despite different names*

### Comparing `pynajax-0.1.2/docs/examples/plot_benchmark_threshold.py` & `pynajax-0.1.3/docs/examples/plot_benchmark_threshold.py`

 * *Files identical despite different names*

### Comparing `pynajax-0.1.2/docs/gallery_conf.py` & `pynajax-0.1.3/docs/gallery_conf.py`

 * *Files identical despite different names*

### Comparing `pynajax-0.1.2/docs/gen_ref_pages.py` & `pynajax-0.1.3/docs/gen_ref_pages.py`

 * *Files identical despite different names*

### Comparing `pynajax-0.1.2/docs/images/convolve_benchmark.png` & `pynajax-0.1.3/docs/images/convolve_benchmark.png`

 * *Files identical despite different names*

### Comparing `pynajax-0.1.2/docs/index.md` & `pynajax-0.1.3/docs/index.md`

 * *Files identical despite different names*

### Comparing `pynajax-0.1.2/mkdocs.yml` & `pynajax-0.1.3/mkdocs.yml`

 * *Files identical despite different names*

### Comparing `pynajax-0.1.2/noxfile.py` & `pynajax-0.1.3/noxfile.py`

 * *Files identical despite different names*

### Comparing `pynajax-0.1.2/pyproject.toml` & `pynajax-0.1.3/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 [build-system]
 requires      = ["setuptools>=61.0.0", "setuptools-scm", "wheel"]
 build-backend = "setuptools.build_meta"
 
 
 [project]
 name = "pynajax"
-version = "0.1.2"
+version = "0.1.3"
 authors = [{name = "pynajax authors"}]
 description = "A JAX backend for pynapple."
 readme = "README.md"
 requires-python = ">=3.8"
 keywords = ["neuroscience", "jax-backend", "pynapple"]
 license = { file = "LICENSE" }
 classifiers = [
```

### Comparing `pynajax-0.1.2/src/pynajax/jax_core_bin_average.py` & `pynajax-0.1.3/src/pynajax/jax_core_bin_average.py`

 * *Files 2% similar despite different names*

```diff
@@ -170,14 +170,17 @@
     Returns
     -------
     time_array_new : jax.numpy.ndarray
         New time array corresponding to the bin centers.
     data_array_new : jax.numpy.ndarray
         New data array containing the averaged values.
     """
+    if not isinstance(data_array, jnp.ndarray):
+        data_array = jnp.asarray(data_array)
+
     # Calculate bin edges and identify time points within epochs for averaging.
     ix, edges, in_epoch = _get_bin_edges(time_array, starts, ends, binsize=binsize)
 
     # Digitize time points to find corresponding bins, adjusting indices to be 0-based.
     bins = np.digitize(time_array[ix], edges) - 1
     average = jit_average(bins, data_array[ix], edges)
```

### Comparing `pynajax-0.1.2/src/pynajax/jax_core_convolve.py` & `pynajax-0.1.3/src/pynajax/jax_core_convolve.py`

 * *Files 2% similar despite different names*

```diff
@@ -183,14 +183,18 @@
         convolved_data = _jit_tree_convolve_2d_kernel(tree, kernel)
 
     return convolved_data[idx]
 
 
 def convolve(time_array, data_array, starts, ends, kernel, trim="both"):
     """One-dimensional convolution."""
+
+    if not isinstance(data_array, jnp.ndarray):
+        data_array = jnp.asarray(data_array)
+
     # Perform convolution
     if kernel.ndim == 0:
         raise IOError(
             "Provide a kernel with at least 1 dimension, current kernel has 0 dimensions"
         )
 
     if len(starts) == 1 and len(ends) == 1:
```

### Comparing `pynajax-0.1.2/src/pynajax/jax_core_threshold.py` & `pynajax-0.1.3/src/pynajax/jax_core_threshold.py`

 * *Files 6% similar despite different names*

```diff
@@ -22,14 +22,17 @@
 
 
     Returns
     -------
     tuple of ArrayLike
         Description
     """
+    if not isinstance(data_array, jnp.ndarray):
+        data_array = jnp.asarray(data_array)
+
     idx_start, idx_end = _get_idxs(time_array, starts, ends)
     idx_slicing = _get_slicing(idx_start, idx_end)
 
     data_array = data_array[idx_slicing]
     time_array = time_array[idx_slicing]
 
     if method == "above":
```

### Comparing `pynajax-0.1.2/src/pynajax/jax_process_perievent.py` & `pynajax-0.1.3/src/pynajax/jax_process_perievent.py`

 * *Files 2% similar despite different names*

```diff
@@ -170,14 +170,18 @@
     N_target : int
         Number of reference time points
     slice_idx : ArrayLike
         2-d numpy array of size (N_target, 2). Each row is the start and end of the slice
     w_starts : ArrayLike
         1-d numpy array of size (N_target,). Whether to trim the window on the left when slicing
     """
+
+    if not isinstance(data_array, jnp.ndarray):
+        data_array = jnp.asarray(data_array)
+
     new_data_array = jnp.full((N_w, N_target, *data_array.shape[1:]), jnp.nan)
 
     w_sizes = slice_idx[:, 1] - slice_idx[:, 0]  # Different sizes
 
     all_w_sizes = np.unique(w_sizes)
     all_w_start = np.unique(w_starts)
```

### Comparing `pynajax-0.1.2/src/pynajax/utils.py` & `pynajax-0.1.3/src/pynajax/utils.py`

 * *Files identical despite different names*

### Comparing `pynajax-0.1.2/src/pynajax.egg-info/PKG-INFO` & `pynajax-0.1.3/src/pynajax.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pynajax
-Version: 0.1.2
+Version: 0.1.3
 Summary: A JAX backend for pynapple.
 Author: pynajax authors
 License: MIT License
         
         Copyright (c) 2024 pynapple-org
         
         Permission is hereby granted, free of charge, to any person obtaining a copy
```

### Comparing `pynajax-0.1.2/src/pynajax.egg-info/SOURCES.txt` & `pynajax-0.1.3/src/pynajax.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `pynajax-0.1.2/tests/conftest.py` & `pynajax-0.1.3/tests/conftest.py`

 * *Files identical despite different names*

### Comparing `pynajax-0.1.2/tests/mock.py` & `pynajax-0.1.3/tests/mock.py`

 * *Files identical despite different names*

### Comparing `pynajax-0.1.2/tests/test_jax_core_convolve.py` & `pynajax-0.1.3/tests/test_jax_core_convolve.py`

 * *Files identical despite different names*

### Comparing `pynajax-0.1.2/tests/test_jax_core_perievent.py` & `pynajax-0.1.3/tests/test_jax_core_perievent.py`

 * *Files identical despite different names*

### Comparing `pynajax-0.1.2/tests/test_jax_numpy_compatibility.py` & `pynajax-0.1.3/tests/test_jax_numpy_compatibility.py`

 * *Files identical despite different names*

