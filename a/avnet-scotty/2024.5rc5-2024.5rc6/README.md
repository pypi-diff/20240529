# Comparing `tmp/avnet_scotty-2024.5rc5.tar.gz` & `tmp/avnet_scotty-2024.5rc6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "avnet_scotty-2024.5rc5.tar", last modified: Thu May 23 15:55:57 2024, max compression
+gzip compressed data, was "avnet_scotty-2024.5rc6.tar", last modified: Fri May 24 09:21:54 2024, max compression
```

## Comparing `avnet_scotty-2024.5rc5.tar` & `avnet_scotty-2024.5rc6.tar`

### file list

```diff
@@ -1,35 +1,35 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-23 15:55:57.670289 avnet_scotty-2024.5rc5/
--rw-r--r--   0 root         (0) root         (0)    32879 2024-05-23 15:55:54.000000 avnet_scotty-2024.5rc5/LICENSE
--rw-r--r--   0 root         (0) root         (0)       48 2024-05-23 15:55:54.000000 avnet_scotty-2024.5rc5/MANIFEST.in
--rw-r--r--   0 root         (0) root         (0)     1433 2024-05-23 15:55:57.670289 avnet_scotty-2024.5rc5/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)    23984 2024-05-23 15:55:54.000000 avnet_scotty-2024.5rc5/README.rst
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-23 15:55:57.670289 avnet_scotty-2024.5rc5/avnet_scotty.egg-info/
--rw-r--r--   0 root         (0) root         (0)     1433 2024-05-23 15:55:57.000000 avnet_scotty-2024.5rc5/avnet_scotty.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)      564 2024-05-23 15:55:57.000000 avnet_scotty-2024.5rc5/avnet_scotty.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2024-05-23 15:55:57.000000 avnet_scotty-2024.5rc5/avnet_scotty.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)       88 2024-05-23 15:55:57.000000 avnet_scotty-2024.5rc5/avnet_scotty.egg-info/entry_points.txt
--rw-r--r--   0 root         (0) root         (0)       99 2024-05-23 15:55:57.000000 avnet_scotty-2024.5rc5/avnet_scotty.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)       19 2024-05-23 15:55:57.000000 avnet_scotty-2024.5rc5/avnet_scotty.egg-info/top_level.txt
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-23 15:55:57.666288 avnet_scotty-2024.5rc5/bumper/
--rw-r--r--   0 root         (0) root         (0)      110 2024-05-23 15:55:54.000000 avnet_scotty-2024.5rc5/bumper/__init__.py
--rwxr-xr-x   0 root         (0) root         (0)     4006 2024-05-23 15:55:54.000000 avnet_scotty-2024.5rc5/bumper/__main__.py
--rw-r--r--   0 root         (0) root         (0)      206 2024-05-23 15:55:54.000000 avnet_scotty-2024.5rc5/requirements.txt
--rwxr-xr-x   0 root         (0) root         (0)     6902 2024-05-23 15:55:54.000000 avnet_scotty-2024.5rc5/scotty
--rwxr-xr-x   0 root         (0) root         (0)     2370 2024-05-23 15:55:54.000000 avnet_scotty-2024.5rc5/scotty-runqemu
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-23 15:55:57.666288 avnet_scotty-2024.5rc5/scotty_test/
--rw-r--r--   0 root         (0) root         (0)     4424 2024-05-23 15:55:54.000000 avnet_scotty-2024.5rc5/scotty_test/__main__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-23 15:55:57.666288 avnet_scotty-2024.5rc5/scotty_test/menu/
--rw-r--r--   0 root         (0) root         (0)     2746 2024-05-23 15:55:54.000000 avnet_scotty-2024.5rc5/scotty_test/menu/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-23 15:55:57.666288 avnet_scotty-2024.5rc5/scotty_test/reporter/
--rw-r--r--   0 root         (0) root         (0)     3101 2024-05-23 15:55:54.000000 avnet_scotty-2024.5rc5/scotty_test/reporter/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-23 15:55:57.666288 avnet_scotty-2024.5rc5/scotty_test/runner/
--rw-r--r--   0 root         (0) root         (0)     9890 2024-05-23 15:55:54.000000 avnet_scotty-2024.5rc5/scotty_test/runner/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-23 15:55:57.670289 avnet_scotty-2024.5rc5/scotty_test/storage/
--rw-r--r--   0 root         (0) root         (0)     2481 2024-05-23 15:55:54.000000 avnet_scotty-2024.5rc5/scotty_test/storage/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-23 15:55:57.670289 avnet_scotty-2024.5rc5/scotty_test/utils/
--rw-r--r--   0 root         (0) root         (0)     1526 2024-05-23 15:55:54.000000 avnet_scotty-2024.5rc5/scotty_test/utils/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-23 15:55:57.670289 avnet_scotty-2024.5rc5/scripts/
--rwxr-xr-x   0 root         (0) root         (0)      811 2024-05-23 15:55:54.000000 avnet_scotty-2024.5rc5/scripts/vm_bundle.sh
--rw-r--r--   0 root         (0) root         (0)     1137 2024-05-23 15:55:54.000000 avnet_scotty-2024.5rc5/scripts/vm_create.sh.template
--rw-r--r--   0 root         (0) root         (0)       38 2024-05-23 15:55:57.670289 avnet_scotty-2024.5rc5/setup.cfg
--rw-r--r--   0 root         (0) root         (0)     2338 2024-05-23 15:55:54.000000 avnet_scotty-2024.5rc5/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-24 09:21:54.508935 avnet_scotty-2024.5rc6/
+-rw-r--r--   0 root         (0) root         (0)    32879 2024-05-24 09:21:50.000000 avnet_scotty-2024.5rc6/LICENSE
+-rw-r--r--   0 root         (0) root         (0)       48 2024-05-24 09:21:50.000000 avnet_scotty-2024.5rc6/MANIFEST.in
+-rw-r--r--   0 root         (0) root         (0)     1433 2024-05-24 09:21:54.508935 avnet_scotty-2024.5rc6/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)    23984 2024-05-24 09:21:50.000000 avnet_scotty-2024.5rc6/README.rst
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-24 09:21:54.508935 avnet_scotty-2024.5rc6/avnet_scotty.egg-info/
+-rw-r--r--   0 root         (0) root         (0)     1433 2024-05-24 09:21:54.000000 avnet_scotty-2024.5rc6/avnet_scotty.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)      564 2024-05-24 09:21:54.000000 avnet_scotty-2024.5rc6/avnet_scotty.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2024-05-24 09:21:54.000000 avnet_scotty-2024.5rc6/avnet_scotty.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)       88 2024-05-24 09:21:54.000000 avnet_scotty-2024.5rc6/avnet_scotty.egg-info/entry_points.txt
+-rw-r--r--   0 root         (0) root         (0)       99 2024-05-24 09:21:54.000000 avnet_scotty-2024.5rc6/avnet_scotty.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)       19 2024-05-24 09:21:54.000000 avnet_scotty-2024.5rc6/avnet_scotty.egg-info/top_level.txt
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-24 09:21:54.504935 avnet_scotty-2024.5rc6/bumper/
+-rw-r--r--   0 root         (0) root         (0)      110 2024-05-24 09:21:50.000000 avnet_scotty-2024.5rc6/bumper/__init__.py
+-rwxr-xr-x   0 root         (0) root         (0)     4006 2024-05-24 09:21:50.000000 avnet_scotty-2024.5rc6/bumper/__main__.py
+-rw-r--r--   0 root         (0) root         (0)      206 2024-05-24 09:21:50.000000 avnet_scotty-2024.5rc6/requirements.txt
+-rwxr-xr-x   0 root         (0) root         (0)     6902 2024-05-24 09:21:51.000000 avnet_scotty-2024.5rc6/scotty
+-rwxr-xr-x   0 root         (0) root         (0)     2370 2024-05-24 09:21:50.000000 avnet_scotty-2024.5rc6/scotty-runqemu
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-24 09:21:54.504935 avnet_scotty-2024.5rc6/scotty_test/
+-rw-r--r--   0 root         (0) root         (0)     4424 2024-05-24 09:21:50.000000 avnet_scotty-2024.5rc6/scotty_test/__main__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-24 09:21:54.504935 avnet_scotty-2024.5rc6/scotty_test/menu/
+-rw-r--r--   0 root         (0) root         (0)     2746 2024-05-24 09:21:50.000000 avnet_scotty-2024.5rc6/scotty_test/menu/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-24 09:21:54.504935 avnet_scotty-2024.5rc6/scotty_test/reporter/
+-rw-r--r--   0 root         (0) root         (0)     3101 2024-05-24 09:21:50.000000 avnet_scotty-2024.5rc6/scotty_test/reporter/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-24 09:21:54.504935 avnet_scotty-2024.5rc6/scotty_test/runner/
+-rw-r--r--   0 root         (0) root         (0)     9890 2024-05-24 09:21:50.000000 avnet_scotty-2024.5rc6/scotty_test/runner/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-24 09:21:54.504935 avnet_scotty-2024.5rc6/scotty_test/storage/
+-rw-r--r--   0 root         (0) root         (0)     2481 2024-05-24 09:21:50.000000 avnet_scotty-2024.5rc6/scotty_test/storage/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-24 09:21:54.504935 avnet_scotty-2024.5rc6/scotty_test/utils/
+-rw-r--r--   0 root         (0) root         (0)     1526 2024-05-24 09:21:50.000000 avnet_scotty-2024.5rc6/scotty_test/utils/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-24 09:21:54.504935 avnet_scotty-2024.5rc6/scripts/
+-rwxr-xr-x   0 root         (0) root         (0)      811 2024-05-24 09:21:50.000000 avnet_scotty-2024.5rc6/scripts/vm_bundle.sh
+-rw-r--r--   0 root         (0) root         (0)     1137 2024-05-24 09:21:50.000000 avnet_scotty-2024.5rc6/scripts/vm_create.sh.template
+-rw-r--r--   0 root         (0) root         (0)       38 2024-05-24 09:21:54.508935 avnet_scotty-2024.5rc6/setup.cfg
+-rw-r--r--   0 root         (0) root         (0)     2338 2024-05-24 09:21:50.000000 avnet_scotty-2024.5rc6/setup.py
```

### Comparing `avnet_scotty-2024.5rc5/LICENSE` & `avnet_scotty-2024.5rc6/LICENSE`

 * *Files identical despite different names*

### Comparing `avnet_scotty-2024.5rc5/PKG-INFO` & `avnet_scotty-2024.5rc6/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: avnet-scotty
-Version: 2024.5rc5
+Version: 2024.5rc6
 Summary: scotty: S(imple)C(ore) O(pen) T(echnology) T(ool for) Y(ou)
 Author: Avnet Embedded GmbH
 License: GPL-3.0-only
 Project-URL: Documentation, https://simple.embedded.avnet.com/?link=tools/scotty/README.html
 Project-URL: SimpleCore Documentation, https://simple.embedded.avnet.com/
 Project-URL: Source Code, https://github.com/avnet-embedded/simplecore-tools/tree/kirkstone/scotty
 Description-Content-Type: text/markdown
```

### Comparing `avnet_scotty-2024.5rc5/README.rst` & `avnet_scotty-2024.5rc6/README.rst`

 * *Files identical despite different names*

### Comparing `avnet_scotty-2024.5rc5/avnet_scotty.egg-info/PKG-INFO` & `avnet_scotty-2024.5rc6/avnet_scotty.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: avnet-scotty
-Version: 2024.5rc5
+Version: 2024.5rc6
 Summary: scotty: S(imple)C(ore) O(pen) T(echnology) T(ool for) Y(ou)
 Author: Avnet Embedded GmbH
 License: GPL-3.0-only
 Project-URL: Documentation, https://simple.embedded.avnet.com/?link=tools/scotty/README.html
 Project-URL: SimpleCore Documentation, https://simple.embedded.avnet.com/
 Project-URL: Source Code, https://github.com/avnet-embedded/simplecore-tools/tree/kirkstone/scotty
 Description-Content-Type: text/markdown
```

### Comparing `avnet_scotty-2024.5rc5/avnet_scotty.egg-info/SOURCES.txt` & `avnet_scotty-2024.5rc6/avnet_scotty.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `avnet_scotty-2024.5rc5/bumper/__main__.py` & `avnet_scotty-2024.5rc6/bumper/__main__.py`

 * *Files identical despite different names*

### Comparing `avnet_scotty-2024.5rc5/scotty` & `avnet_scotty-2024.5rc6/scotty`

 * *Files 2% similar despite different names*

```diff
@@ -31,20 +31,20 @@
 	TERM \
 	UBOOT_ENV_VARS \
 	"
 # SCOTTY_FEATURES_LAYERS REPO_URL SCOTTY_MACHINE_DIR BUILDDIR
 declare -r scotty_whitelist=${SCOTTY_WHITELIST:-${scotty_whitelist_default}}
 
 if [ "${SCOTTY_DOCKER_IMAGE:-1}" == "1" ]; then
-    declare -r docker_default_image="ghcr.io/avnet-embedded/scotty:2024.5rc5"
+    declare -r docker_default_image="ghcr.io/avnet-embedded/scotty:2024.5rc6"
 else
     declare -r docker_default_image="${SCOTTY_DOCKER_IMAGE}"
 fi
 
-export SCOTTY_DEFAULT_MANIFEST_BRANCH="refs/tags/2024.5rc5"
+export SCOTTY_DEFAULT_MANIFEST_BRANCH="refs/tags/2024.5rc6"
 export SCOTTY_DEFAULT_MANIFEST_NAME="default-release.xml"
 
 debug() {
 	if [ "${SCOTTY_DEBUG:-0}" == "1" ]; then
 		echo -e "\033[1;38m${*}\033[0m"
 	fi
 }
```

### Comparing `avnet_scotty-2024.5rc5/scotty-runqemu` & `avnet_scotty-2024.5rc6/scotty-runqemu`

 * *Files identical despite different names*

### Comparing `avnet_scotty-2024.5rc5/scotty_test/__main__.py` & `avnet_scotty-2024.5rc6/scotty_test/__main__.py`

 * *Files identical despite different names*

### Comparing `avnet_scotty-2024.5rc5/scotty_test/menu/__init__.py` & `avnet_scotty-2024.5rc6/scotty_test/menu/__init__.py`

 * *Files identical despite different names*

### Comparing `avnet_scotty-2024.5rc5/scotty_test/reporter/__init__.py` & `avnet_scotty-2024.5rc6/scotty_test/reporter/__init__.py`

 * *Files identical despite different names*

### Comparing `avnet_scotty-2024.5rc5/scotty_test/runner/__init__.py` & `avnet_scotty-2024.5rc6/scotty_test/runner/__init__.py`

 * *Files identical despite different names*

### Comparing `avnet_scotty-2024.5rc5/scotty_test/storage/__init__.py` & `avnet_scotty-2024.5rc6/scotty_test/storage/__init__.py`

 * *Files identical despite different names*

### Comparing `avnet_scotty-2024.5rc5/scotty_test/utils/__init__.py` & `avnet_scotty-2024.5rc6/scotty_test/utils/__init__.py`

 * *Files identical despite different names*

### Comparing `avnet_scotty-2024.5rc5/scripts/vm_bundle.sh` & `avnet_scotty-2024.5rc6/scripts/vm_bundle.sh`

 * *Files identical despite different names*

### Comparing `avnet_scotty-2024.5rc5/scripts/vm_create.sh.template` & `avnet_scotty-2024.5rc6/scripts/vm_create.sh.template`

 * *Files identical despite different names*

### Comparing `avnet_scotty-2024.5rc5/setup.py` & `avnet_scotty-2024.5rc6/setup.py`

 * *Files identical despite different names*

