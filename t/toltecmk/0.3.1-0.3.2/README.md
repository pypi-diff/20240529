# Comparing `tmp/toltecmk-0.3.1.tar.gz` & `tmp/toltecmk-0.3.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "toltecmk-0.3.1.tar", last modified: Mon May 20 19:20:54 2024, max compression
+gzip compressed data, was "toltecmk-0.3.2.tar", last modified: Wed May 29 00:57:28 2024, max compression
```

## Comparing `toltecmk-0.3.1.tar` & `toltecmk-0.3.2.tar`

### file list

```diff
@@ -1,42 +1,42 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-20 19:20:54.916532 toltecmk-0.3.1/
--rw-r--r--   0 runner    (1001) docker     (127)     1080 2024-05-20 19:20:36.000000 toltecmk-0.3.1/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)     6537 2024-05-20 19:20:54.916532 toltecmk-0.3.1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     5500 2024-05-20 19:20:36.000000 toltecmk-0.3.1/README.md
--rw-r--r--   0 runner    (1001) docker     (127)     1479 2024-05-20 19:20:36.000000 toltecmk-0.3.1/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)      136 2024-05-20 19:20:36.000000 toltecmk-0.3.1/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-20 19:20:54.916532 toltecmk-0.3.1/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-20 19:20:54.912532 toltecmk-0.3.1/tests/
--rw-r--r--   0 runner    (1001) docker     (127)     5560 2024-05-20 19:20:36.000000 toltecmk-0.3.1/tests/test_ipk.py
--rw-r--r--   0 runner    (1001) docker     (127)     2890 2024-05-20 19:20:36.000000 toltecmk-0.3.1/tests/test_recipe.py
--rw-r--r--   0 runner    (1001) docker     (127)     3084 2024-05-20 19:20:36.000000 toltecmk-0.3.1/tests/test_strip.py
--rw-r--r--   0 runner    (1001) docker     (127)     6112 2024-05-20 19:20:36.000000 toltecmk-0.3.1/tests/test_toltec.py
--rw-r--r--   0 runner    (1001) docker     (127)     9862 2024-05-20 19:20:36.000000 toltecmk-0.3.1/tests/test_version.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-20 19:20:54.916532 toltecmk-0.3.1/toltec/
--rw-r--r--   0 runner    (1001) docker     (127)      153 2024-05-20 19:20:36.000000 toltecmk-0.3.1/toltec/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     3657 2024-05-20 19:20:36.000000 toltecmk-0.3.1/toltec/__main__.py
--rw-r--r--   0 runner    (1001) docker     (127)    13255 2024-05-20 19:20:36.000000 toltecmk-0.3.1/toltec/bash.py
--rw-r--r--   0 runner    (1001) docker     (127)    16023 2024-05-20 19:20:36.000000 toltecmk-0.3.1/toltec/builder.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-20 19:20:54.916532 toltecmk-0.3.1/toltec/hooks/
--rw-r--r--   0 runner    (1001) docker     (127)      207 2024-05-20 19:20:36.000000 toltecmk-0.3.1/toltec/hooks/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     5202 2024-05-20 19:20:36.000000 toltecmk-0.3.1/toltec/hooks/install_lib.py
--rw-r--r--   0 runner    (1001) docker     (127)     2832 2024-05-20 19:20:36.000000 toltecmk-0.3.1/toltec/hooks/patch_rm2fb.py
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-20 19:20:36.000000 toltecmk-0.3.1/toltec/hooks/py.typed
--rw-r--r--   0 runner    (1001) docker     (127)     1064 2024-05-20 19:20:36.000000 toltecmk-0.3.1/toltec/hooks/reload_oxide_apps.py
--rw-r--r--   0 runner    (1001) docker     (127)     4591 2024-05-20 19:20:36.000000 toltecmk-0.3.1/toltec/hooks/strip.py
--rw-r--r--   0 runner    (1001) docker     (127)     7766 2024-05-20 19:20:36.000000 toltecmk-0.3.1/toltec/ipk.py
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-20 19:20:36.000000 toltecmk-0.3.1/toltec/py.typed
--rw-r--r--   0 runner    (1001) docker     (127)     5505 2024-05-20 19:20:36.000000 toltecmk-0.3.1/toltec/recipe.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-20 19:20:54.916532 toltecmk-0.3.1/toltec/recipe_parsers/
--rw-r--r--   0 runner    (1001) docker     (127)      891 2024-05-20 19:20:36.000000 toltecmk-0.3.1/toltec/recipe_parsers/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    13185 2024-05-20 19:20:36.000000 toltecmk-0.3.1/toltec/recipe_parsers/bash.py
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-20 19:20:36.000000 toltecmk-0.3.1/toltec/recipe_parsers/py.typed
--rw-r--r--   0 runner    (1001) docker     (127)     1764 2024-05-20 19:20:36.000000 toltecmk-0.3.1/toltec/repo.py
--rw-r--r--   0 runner    (1001) docker     (127)    10931 2024-05-20 19:20:36.000000 toltecmk-0.3.1/toltec/util.py
--rw-r--r--   0 runner    (1001) docker     (127)    12758 2024-05-20 19:20:36.000000 toltecmk-0.3.1/toltec/version.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-20 19:20:54.916532 toltecmk-0.3.1/toltecmk.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     6537 2024-05-20 19:20:54.000000 toltecmk-0.3.1/toltecmk.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      765 2024-05-20 19:20:54.000000 toltecmk-0.3.1/toltecmk.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-20 19:20:54.000000 toltecmk-0.3.1/toltecmk.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       50 2024-05-20 19:20:54.000000 toltecmk-0.3.1/toltecmk.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (127)       71 2024-05-20 19:20:54.000000 toltecmk-0.3.1/toltecmk.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)        7 2024-05-20 19:20:54.000000 toltecmk-0.3.1/toltecmk.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-29 00:57:28.085897 toltecmk-0.3.2/
+-rw-r--r--   0 runner    (1001) docker     (127)     1080 2024-05-29 00:57:08.000000 toltecmk-0.3.2/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)     6537 2024-05-29 00:57:28.085897 toltecmk-0.3.2/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     5500 2024-05-29 00:57:08.000000 toltecmk-0.3.2/README.md
+-rw-r--r--   0 runner    (1001) docker     (127)     1479 2024-05-29 00:57:08.000000 toltecmk-0.3.2/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)      136 2024-05-29 00:57:08.000000 toltecmk-0.3.2/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-29 00:57:28.085897 toltecmk-0.3.2/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-29 00:57:28.081897 toltecmk-0.3.2/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)     5560 2024-05-29 00:57:08.000000 toltecmk-0.3.2/tests/test_ipk.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2890 2024-05-29 00:57:08.000000 toltecmk-0.3.2/tests/test_recipe.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3084 2024-05-29 00:57:08.000000 toltecmk-0.3.2/tests/test_strip.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6112 2024-05-29 00:57:08.000000 toltecmk-0.3.2/tests/test_toltec.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9862 2024-05-29 00:57:08.000000 toltecmk-0.3.2/tests/test_version.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-29 00:57:28.081897 toltecmk-0.3.2/toltec/
+-rw-r--r--   0 runner    (1001) docker     (127)      153 2024-05-29 00:57:08.000000 toltecmk-0.3.2/toltec/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3657 2024-05-29 00:57:08.000000 toltecmk-0.3.2/toltec/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    13255 2024-05-29 00:57:08.000000 toltecmk-0.3.2/toltec/bash.py
+-rw-r--r--   0 runner    (1001) docker     (127)    16023 2024-05-29 00:57:08.000000 toltecmk-0.3.2/toltec/builder.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-29 00:57:28.081897 toltecmk-0.3.2/toltec/hooks/
+-rw-r--r--   0 runner    (1001) docker     (127)      207 2024-05-29 00:57:08.000000 toltecmk-0.3.2/toltec/hooks/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5253 2024-05-29 00:57:08.000000 toltecmk-0.3.2/toltec/hooks/install_lib.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2832 2024-05-29 00:57:08.000000 toltecmk-0.3.2/toltec/hooks/patch_rm2fb.py
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-29 00:57:08.000000 toltecmk-0.3.2/toltec/hooks/py.typed
+-rw-r--r--   0 runner    (1001) docker     (127)     1064 2024-05-29 00:57:08.000000 toltecmk-0.3.2/toltec/hooks/reload_oxide_apps.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4591 2024-05-29 00:57:08.000000 toltecmk-0.3.2/toltec/hooks/strip.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7766 2024-05-29 00:57:08.000000 toltecmk-0.3.2/toltec/ipk.py
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-29 00:57:08.000000 toltecmk-0.3.2/toltec/py.typed
+-rw-r--r--   0 runner    (1001) docker     (127)     5505 2024-05-29 00:57:08.000000 toltecmk-0.3.2/toltec/recipe.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-29 00:57:28.081897 toltecmk-0.3.2/toltec/recipe_parsers/
+-rw-r--r--   0 runner    (1001) docker     (127)      891 2024-05-29 00:57:08.000000 toltecmk-0.3.2/toltec/recipe_parsers/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    13185 2024-05-29 00:57:08.000000 toltecmk-0.3.2/toltec/recipe_parsers/bash.py
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-29 00:57:08.000000 toltecmk-0.3.2/toltec/recipe_parsers/py.typed
+-rw-r--r--   0 runner    (1001) docker     (127)     1764 2024-05-29 00:57:08.000000 toltecmk-0.3.2/toltec/repo.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10931 2024-05-29 00:57:08.000000 toltecmk-0.3.2/toltec/util.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12758 2024-05-29 00:57:08.000000 toltecmk-0.3.2/toltec/version.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-29 00:57:28.085897 toltecmk-0.3.2/toltecmk.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     6537 2024-05-29 00:57:28.000000 toltecmk-0.3.2/toltecmk.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      765 2024-05-29 00:57:28.000000 toltecmk-0.3.2/toltecmk.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-29 00:57:28.000000 toltecmk-0.3.2/toltecmk.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       50 2024-05-29 00:57:28.000000 toltecmk-0.3.2/toltecmk.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       71 2024-05-29 00:57:28.000000 toltecmk-0.3.2/toltecmk.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        7 2024-05-29 00:57:28.000000 toltecmk-0.3.2/toltecmk.egg-info/top_level.txt
```

### Comparing `toltecmk-0.3.1/LICENSE` & `toltecmk-0.3.2/LICENSE`

 * *Files identical despite different names*

### Comparing `toltecmk-0.3.1/PKG-INFO` & `toltecmk-0.3.2/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: toltecmk
-Version: 0.3.1
+Version: 0.3.2
 Summary: Build system used for the Toltec community repository
 Author-email: Mattéo Delabre <git.matteo@delab.re>, Eeems <eeems@eeems.email>
 Project-URL: Homepage, https://github.com/toltec-dev/build
 Project-URL: Bug Tracker, https://github.com/toltec-dev/build/issues
 Keywords: build-tooling,packaging,distribution
 Classifier: Development Status :: 4 - Beta
 Classifier: Intended Audience :: Developers
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: toltecmk Version: 0.3.1 Summary: Build system used
+Metadata-Version: 2.1 Name: toltecmk Version: 0.3.2 Summary: Build system used
 for the Toltec community repository Author-email: MattÃ©o Delabre
 delab.re>, Eeems
 eeems.email> Project-URL: Homepage, https://github.com/toltec-dev/build
 Project-URL: Bug Tracker, https://github.com/toltec-dev/build/issues Keywords:
 build-tooling,packaging,distribution Classifier: Development Status :: 4 - Beta
 Classifier: Intended Audience :: Developers Classifier: License :: OSI Approved
 :: MIT License Classifier: Operating System :: POSIX :: Linux Classifier:
```

### Comparing `toltecmk-0.3.1/README.md` & `toltecmk-0.3.2/README.md`

 * *Files identical despite different names*

### Comparing `toltecmk-0.3.1/pyproject.toml` & `toltecmk-0.3.2/pyproject.toml`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [project]
 name = "toltecmk"
-version = "0.3.1"
+version = "0.3.2"
 authors = [
   { name="Mattéo Delabre", email="git.matteo@delab.re" },
   { name="Eeems", email="eeems@eeems.email" },
 ]
 description = "Build system used for the Toltec community repository"
 requires-python = ">=3.11"
 classifiers = [
```

### Comparing `toltecmk-0.3.1/tests/test_ipk.py` & `toltecmk-0.3.2/tests/test_ipk.py`

 * *Files identical despite different names*

### Comparing `toltecmk-0.3.1/tests/test_recipe.py` & `toltecmk-0.3.2/tests/test_recipe.py`

 * *Files identical despite different names*

### Comparing `toltecmk-0.3.1/tests/test_strip.py` & `toltecmk-0.3.2/tests/test_strip.py`

 * *Files identical despite different names*

### Comparing `toltecmk-0.3.1/tests/test_toltec.py` & `toltecmk-0.3.2/tests/test_toltec.py`

 * *Files identical despite different names*

### Comparing `toltecmk-0.3.1/tests/test_version.py` & `toltecmk-0.3.2/tests/test_version.py`

 * *Files identical despite different names*

### Comparing `toltecmk-0.3.1/toltec/__main__.py` & `toltecmk-0.3.2/toltec/__main__.py`

 * *Files identical despite different names*

### Comparing `toltecmk-0.3.1/toltec/bash.py` & `toltecmk-0.3.2/toltec/bash.py`

 * *Files identical despite different names*

### Comparing `toltecmk-0.3.1/toltec/builder.py` & `toltecmk-0.3.2/toltec/builder.py`

 * *Files identical despite different names*

### Comparing `toltecmk-0.3.1/toltec/hooks/install_lib.py` & `toltecmk-0.3.2/toltec/hooks/install_lib.py`

 * *Files 2% similar despite different names*

```diff
@@ -176,15 +176,15 @@
     systemctl stop "$unit_name"
     rm "$unit_path"
     systemctl daemon-reload
     """,
     )
     add_method(
         "unit-exists",
-        '[ "$(systemctl --quiet list-unit-files "${1}" | grep -c "${1}")" -eq 1 ]',
+        '[ "$(systemctl --quiet list-unit-files "${1}" | /bin/grep -c "${1}" 2> /dev/null)" -eq 1 ]',  # pylint: disable=line-too-long
     )
     add_method(
         "disable-unit",
         """
     if ! unit-exists "${1}"; then
         return
     fi
```

### Comparing `toltecmk-0.3.1/toltec/hooks/patch_rm2fb.py` & `toltecmk-0.3.2/toltec/hooks/patch_rm2fb.py`

 * *Files identical despite different names*

### Comparing `toltecmk-0.3.1/toltec/hooks/reload_oxide_apps.py` & `toltecmk-0.3.2/toltec/hooks/reload_oxide_apps.py`

 * *Files identical despite different names*

### Comparing `toltecmk-0.3.1/toltec/hooks/strip.py` & `toltecmk-0.3.2/toltec/hooks/strip.py`

 * *Files identical despite different names*

### Comparing `toltecmk-0.3.1/toltec/ipk.py` & `toltecmk-0.3.2/toltec/ipk.py`

 * *Files identical despite different names*

### Comparing `toltecmk-0.3.1/toltec/recipe.py` & `toltecmk-0.3.2/toltec/recipe.py`

 * *Files identical despite different names*

### Comparing `toltecmk-0.3.1/toltec/recipe_parsers/__init__.py` & `toltecmk-0.3.2/toltec/recipe_parsers/__init__.py`

 * *Files identical despite different names*

### Comparing `toltecmk-0.3.1/toltec/recipe_parsers/bash.py` & `toltecmk-0.3.2/toltec/recipe_parsers/bash.py`

 * *Files identical despite different names*

### Comparing `toltecmk-0.3.1/toltec/repo.py` & `toltecmk-0.3.2/toltec/repo.py`

 * *Files identical despite different names*

### Comparing `toltecmk-0.3.1/toltec/util.py` & `toltecmk-0.3.2/toltec/util.py`

 * *Files identical despite different names*

### Comparing `toltecmk-0.3.1/toltec/version.py` & `toltecmk-0.3.2/toltec/version.py`

 * *Files identical despite different names*

### Comparing `toltecmk-0.3.1/toltecmk.egg-info/PKG-INFO` & `toltecmk-0.3.2/toltecmk.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: toltecmk
-Version: 0.3.1
+Version: 0.3.2
 Summary: Build system used for the Toltec community repository
 Author-email: Mattéo Delabre <git.matteo@delab.re>, Eeems <eeems@eeems.email>
 Project-URL: Homepage, https://github.com/toltec-dev/build
 Project-URL: Bug Tracker, https://github.com/toltec-dev/build/issues
 Keywords: build-tooling,packaging,distribution
 Classifier: Development Status :: 4 - Beta
 Classifier: Intended Audience :: Developers
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: toltecmk Version: 0.3.1 Summary: Build system used
+Metadata-Version: 2.1 Name: toltecmk Version: 0.3.2 Summary: Build system used
 for the Toltec community repository Author-email: MattÃ©o Delabre
 delab.re>, Eeems
 eeems.email> Project-URL: Homepage, https://github.com/toltec-dev/build
 Project-URL: Bug Tracker, https://github.com/toltec-dev/build/issues Keywords:
 build-tooling,packaging,distribution Classifier: Development Status :: 4 - Beta
 Classifier: Intended Audience :: Developers Classifier: License :: OSI Approved
 :: MIT License Classifier: Operating System :: POSIX :: Linux Classifier:
```

### Comparing `toltecmk-0.3.1/toltecmk.egg-info/SOURCES.txt` & `toltecmk-0.3.2/toltecmk.egg-info/SOURCES.txt`

 * *Files identical despite different names*

