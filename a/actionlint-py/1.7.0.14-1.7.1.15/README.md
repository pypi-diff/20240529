# Comparing `tmp/actionlint_py-1.7.0.14.tar.gz` & `tmp/actionlint_py-1.7.1.15.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "actionlint_py-1.7.0.14.tar", last modified: Sun May 19 07:23:12 2024, max compression
+gzip compressed data, was "actionlint_py-1.7.1.15.tar", last modified: Wed May 29 06:24:46 2024, max compression
```

## Comparing `actionlint_py-1.7.0.14.tar` & `actionlint_py-1.7.1.15.tar`

### file list

```diff
@@ -1,30 +1,30 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-19 07:23:12.152948 actionlint_py-1.7.0.14/
--rw-r--r--   0 runner    (1001) docker     (127)     1066 2024-05-19 07:22:59.000000 actionlint_py-1.7.0.14/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)     7054 2024-05-19 07:23:12.148949 actionlint_py-1.7.0.14/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     4637 2024-05-19 07:22:59.000000 actionlint_py-1.7.0.14/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-19 07:23:12.148949 actionlint_py-1.7.0.14/_custom_build/
--rw-r--r--   0 runner    (1001) docker     (127)        5 2024-05-19 07:22:59.000000 actionlint_py-1.7.0.14/_custom_build/VERSION_ACTIONLINT.txt
--rw-r--r--   0 runner    (1001) docker     (127)        3 2024-05-19 07:22:59.000000 actionlint_py-1.7.0.14/_custom_build/VERSION_BUILD_SYSTEM.txt
--rw-r--r--   0 runner    (1001) docker     (127)        2 2024-05-19 07:22:59.000000 actionlint_py-1.7.0.14/_custom_build/VERSION_DEV.txt
--rw-r--r--   0 runner    (1001) docker     (127)       53 2024-05-19 07:22:59.000000 actionlint_py-1.7.0.14/_custom_build/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     5123 2024-05-19 07:22:59.000000 actionlint_py-1.7.0.14/_custom_build/auto_update_main.py
--rw-r--r--   0 runner    (1001) docker     (127)     1698 2024-05-19 07:22:59.000000 actionlint_py-1.7.0.14/_custom_build/checksums.cfg
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-19 07:23:12.148949 actionlint_py-1.7.0.14/_custom_build/commands/
--rw-r--r--   0 runner    (1001) docker     (127)      295 2024-05-19 07:22:59.000000 actionlint_py-1.7.0.14/_custom_build/commands/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      449 2024-05-19 07:22:59.000000 actionlint_py-1.7.0.14/_custom_build/commands/bdist_wheel.py
--rw-r--r--   0 runner    (1001) docker     (127)      308 2024-05-19 07:22:59.000000 actionlint_py-1.7.0.14/_custom_build/commands/build.py
--rw-r--r--   0 runner    (1001) docker     (127)     1069 2024-05-19 07:22:59.000000 actionlint_py-1.7.0.14/_custom_build/commands/fetch_binaries.py
--rw-r--r--   0 runner    (1001) docker     (127)      172 2024-05-19 07:22:59.000000 actionlint_py-1.7.0.14/_custom_build/commands/install.py
--rw-r--r--   0 runner    (1001) docker     (127)      707 2024-05-19 07:22:59.000000 actionlint_py-1.7.0.14/_custom_build/commands/install_actionlint.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-19 07:23:12.148949 actionlint_py-1.7.0.14/_custom_build/utils/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-19 07:22:59.000000 actionlint_py-1.7.0.14/_custom_build/utils/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1668 2024-05-19 07:22:59.000000 actionlint_py-1.7.0.14/_custom_build/utils/file_ops.py
--rw-r--r--   0 runner    (1001) docker     (127)     2913 2024-05-19 07:22:59.000000 actionlint_py-1.7.0.14/_custom_build/version.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-19 07:23:12.148949 actionlint_py-1.7.0.14/actionlint_py.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     7054 2024-05-19 07:23:12.000000 actionlint_py-1.7.0.14/actionlint_py.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      724 2024-05-19 07:23:12.000000 actionlint_py-1.7.0.14/actionlint_py.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-19 07:23:12.000000 actionlint_py-1.7.0.14/actionlint_py.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       75 2024-05-19 07:23:12.000000 actionlint_py-1.7.0.14/actionlint_py.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       14 2024-05-19 07:23:12.000000 actionlint_py-1.7.0.14/actionlint_py.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)     1894 2024-05-19 07:22:59.000000 actionlint_py-1.7.0.14/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-19 07:23:12.152948 actionlint_py-1.7.0.14/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-29 06:24:46.971149 actionlint_py-1.7.1.15/
+-rw-r--r--   0 runner    (1001) docker     (127)     1066 2024-05-29 06:24:36.000000 actionlint_py-1.7.1.15/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)     7054 2024-05-29 06:24:46.971149 actionlint_py-1.7.1.15/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     4637 2024-05-29 06:24:36.000000 actionlint_py-1.7.1.15/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-29 06:24:46.967149 actionlint_py-1.7.1.15/_custom_build/
+-rw-r--r--   0 runner    (1001) docker     (127)        5 2024-05-29 06:24:36.000000 actionlint_py-1.7.1.15/_custom_build/VERSION_ACTIONLINT.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        3 2024-05-29 06:24:36.000000 actionlint_py-1.7.1.15/_custom_build/VERSION_BUILD_SYSTEM.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        2 2024-05-29 06:24:36.000000 actionlint_py-1.7.1.15/_custom_build/VERSION_DEV.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       53 2024-05-29 06:24:36.000000 actionlint_py-1.7.1.15/_custom_build/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5123 2024-05-29 06:24:36.000000 actionlint_py-1.7.1.15/_custom_build/auto_update_main.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1698 2024-05-29 06:24:36.000000 actionlint_py-1.7.1.15/_custom_build/checksums.cfg
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-29 06:24:46.967149 actionlint_py-1.7.1.15/_custom_build/commands/
+-rw-r--r--   0 runner    (1001) docker     (127)      295 2024-05-29 06:24:36.000000 actionlint_py-1.7.1.15/_custom_build/commands/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      449 2024-05-29 06:24:36.000000 actionlint_py-1.7.1.15/_custom_build/commands/bdist_wheel.py
+-rw-r--r--   0 runner    (1001) docker     (127)      308 2024-05-29 06:24:36.000000 actionlint_py-1.7.1.15/_custom_build/commands/build.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1069 2024-05-29 06:24:36.000000 actionlint_py-1.7.1.15/_custom_build/commands/fetch_binaries.py
+-rw-r--r--   0 runner    (1001) docker     (127)      172 2024-05-29 06:24:36.000000 actionlint_py-1.7.1.15/_custom_build/commands/install.py
+-rw-r--r--   0 runner    (1001) docker     (127)      707 2024-05-29 06:24:36.000000 actionlint_py-1.7.1.15/_custom_build/commands/install_actionlint.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-29 06:24:46.967149 actionlint_py-1.7.1.15/_custom_build/utils/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-29 06:24:36.000000 actionlint_py-1.7.1.15/_custom_build/utils/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1668 2024-05-29 06:24:36.000000 actionlint_py-1.7.1.15/_custom_build/utils/file_ops.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2913 2024-05-29 06:24:36.000000 actionlint_py-1.7.1.15/_custom_build/version.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-29 06:24:46.971149 actionlint_py-1.7.1.15/actionlint_py.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     7054 2024-05-29 06:24:46.000000 actionlint_py-1.7.1.15/actionlint_py.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      724 2024-05-29 06:24:46.000000 actionlint_py-1.7.1.15/actionlint_py.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-29 06:24:46.000000 actionlint_py-1.7.1.15/actionlint_py.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       75 2024-05-29 06:24:46.000000 actionlint_py-1.7.1.15/actionlint_py.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       14 2024-05-29 06:24:46.000000 actionlint_py-1.7.1.15/actionlint_py.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)     1894 2024-05-29 06:24:36.000000 actionlint_py-1.7.1.15/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-29 06:24:46.971149 actionlint_py-1.7.1.15/setup.cfg
```

### Comparing `actionlint_py-1.7.0.14/LICENSE` & `actionlint_py-1.7.1.15/LICENSE`

 * *Files identical despite different names*

### Comparing `actionlint_py-1.7.0.14/PKG-INFO` & `actionlint_py-1.7.1.15/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: actionlint_py
-Version: 1.7.0.14
+Version: 1.7.1.15
 Summary: Python wrapper around invoking actionlint (https://github.com/rhysd/actionlint)
 Author-email: Ryan Rhee <pypi@rhee.io>, Mateusz Grzeliński <grzelinskimat@gmail.com>
 Maintainer-email: Mateusz Grzeliński <grzelinskimat@gmail.com>
 License: MIT License
         
         Copyright (c) 2019 Ryan Rhee
         
@@ -75,15 +75,15 @@
 
 Use this repo if you can not use officially supported hooks (docker, golang, system) and you are fine with python `pip` wrapper.
 
 Sample `.pre-commit-config.yaml` using `pip` as package manager:
 
 ```yaml
 - repo: https://github.com/Mateusz-Grzelinski/actionlint-py
-  rev: v1.7.0.14
+  rev: v1.7.1.15
   hooks:
     - id: actionlint
       additional_dependencies: [ pyflakes>=3.0.1, shellcheck-py>=0.9.0.5 ]
       # actionlint has built in support for pyflakes and shellcheck, sadly they will not be auto updated. Check https://pypi.org/project/actionlint-py/ for latest version. Alternatively:
       # args: [-shellcheck=/path/shellcheck -pyflakes=/path/pyflakes]
       # note - invalid path in arguments will fail silently
 ```
@@ -95,17 +95,17 @@
 ```yaml
 - repo: local
   hooks:
     - id: actionlint
       name: actionlint
       description: Lint GitHub workflows with actionlint
       additional_dependencies: [ actionlint-py ]
-      #additional_dependencies: [actionlint-py==1.7.0.14]
+      #additional_dependencies: [actionlint-py==1.7.1.15]
       # safer, but pre-commit autoupdate will not work
-      # note: the pip versioning scheme is different from actionlint binary: not "v1.7.0" but "1.7.0.14" (last number is build system version)
+      # note: the pip versioning scheme is different from actionlint binary: not "v1.7.1" but "1.7.1.15" (last number is build system version)
       entry: actionlint
       #args: [-ignore "*.set-output. was depracated.*"]
       language: python
       types: [ "yaml" ]
       files: "^.github/workflows/"
 ```
 
@@ -117,15 +117,15 @@
 
 ### As pre-commit hooks
 
 See [official docs for pre-commit integration](https://github.com/rhysd/actionlint/blob/main/docs/usage.md#pre-commit)
 
 ```yaml
 - repo: https://github.com/rhysd/actionlint
-  rev: v1.7.0
+  rev: v1.7.1
   hooks:
     - id: actionlint
     # - id: actionlint-docker
     # - id: actionlint-system
 ```
 
 ### Use as github action step
```

### Comparing `actionlint_py-1.7.0.14/README.md` & `actionlint_py-1.7.1.15/README.md`

 * *Files 2% similar despite different names*

```diff
@@ -28,15 +28,15 @@
 
 Use this repo if you can not use officially supported hooks (docker, golang, system) and you are fine with python `pip` wrapper.
 
 Sample `.pre-commit-config.yaml` using `pip` as package manager:
 
 ```yaml
 - repo: https://github.com/Mateusz-Grzelinski/actionlint-py
-  rev: v1.7.0.14
+  rev: v1.7.1.15
   hooks:
     - id: actionlint
       additional_dependencies: [ pyflakes>=3.0.1, shellcheck-py>=0.9.0.5 ]
       # actionlint has built in support for pyflakes and shellcheck, sadly they will not be auto updated. Check https://pypi.org/project/actionlint-py/ for latest version. Alternatively:
       # args: [-shellcheck=/path/shellcheck -pyflakes=/path/pyflakes]
       # note - invalid path in arguments will fail silently
 ```
@@ -48,17 +48,17 @@
 ```yaml
 - repo: local
   hooks:
     - id: actionlint
       name: actionlint
       description: Lint GitHub workflows with actionlint
       additional_dependencies: [ actionlint-py ]
-      #additional_dependencies: [actionlint-py==1.7.0.14]
+      #additional_dependencies: [actionlint-py==1.7.1.15]
       # safer, but pre-commit autoupdate will not work
-      # note: the pip versioning scheme is different from actionlint binary: not "v1.7.0" but "1.7.0.14" (last number is build system version)
+      # note: the pip versioning scheme is different from actionlint binary: not "v1.7.1" but "1.7.1.15" (last number is build system version)
       entry: actionlint
       #args: [-ignore "*.set-output. was depracated.*"]
       language: python
       types: [ "yaml" ]
       files: "^.github/workflows/"
 ```
 
@@ -70,15 +70,15 @@
 
 ### As pre-commit hooks
 
 See [official docs for pre-commit integration](https://github.com/rhysd/actionlint/blob/main/docs/usage.md#pre-commit)
 
 ```yaml
 - repo: https://github.com/rhysd/actionlint
-  rev: v1.7.0
+  rev: v1.7.1
   hooks:
     - id: actionlint
     # - id: actionlint-docker
     # - id: actionlint-system
 ```
 
 ### Use as github action step
```

### Comparing `actionlint_py-1.7.0.14/_custom_build/auto_update_main.py` & `actionlint_py-1.7.1.15/_custom_build/auto_update_main.py`

 * *Files identical despite different names*

### Comparing `actionlint_py-1.7.0.14/_custom_build/checksums.cfg` & `actionlint_py-1.7.1.15/_custom_build/checksums.cfg`

 * *Files 24% similar despite different names*

```diff
@@ -1,35 +1,35 @@
 [linux-x86_64]
-file_name = actionlint_1.7.0_linux_amd64.tar.gz
-checksum = 8aae9148f61952d11a97651852fdc7dffd2b762ed3cdd28b3c2232ae5f55d4db
-url = https://github.com/rhysd/actionlint/releases/download/v1.7.0/actionlint_1.7.0_linux_amd64.tar.gz
+file_name = actionlint_1.7.1_linux_amd64.tar.gz
+checksum = f53c34493657dfea83b657e4b62cc68c25fbc383dff64c8d581613b037aacaa3
+url = https://github.com/rhysd/actionlint/releases/download/v1.7.1/actionlint_1.7.1_linux_amd64.tar.gz
 
 [linux-arm64]
-file_name = actionlint_1.7.0_linux_arm64.tar.gz
-checksum = 8181452246e7e6310b988f83762fc982e03f27eeb53dd4ad33fa4a5f4276b383
-url = https://github.com/rhysd/actionlint/releases/download/v1.7.0/actionlint_1.7.0_linux_arm64.tar.gz
+file_name = actionlint_1.7.1_linux_arm64.tar.gz
+checksum = 21a20f38b19dc962d89e17fe1c6f116199e9e0d343ab33361868def14cc220fc
+url = https://github.com/rhysd/actionlint/releases/download/v1.7.1/actionlint_1.7.1_linux_arm64.tar.gz
 
 [darwin-x86_64]
-file_name = actionlint_1.7.0_darwin_amd64.tar.gz
-checksum = 138aff674f31bd218030d4b00b3024bf0c721b75a7ec8e90b743763f81e3128e
-url = https://github.com/rhysd/actionlint/releases/download/v1.7.0/actionlint_1.7.0_darwin_amd64.tar.gz
+file_name = actionlint_1.7.1_darwin_amd64.tar.gz
+checksum = ee24184e2e7003c19eb739717b34b7c65d096f2ca0df8d571837b4f20112d573
+url = https://github.com/rhysd/actionlint/releases/download/v1.7.1/actionlint_1.7.1_darwin_amd64.tar.gz
 
 [darwin-arm64]
-file_name = actionlint_1.7.0_darwin_arm64.tar.gz
-checksum = 806e73fbafe54b7324d9478798534c5195fb71ea171633d9035b3fca237addd3
-url = https://github.com/rhysd/actionlint/releases/download/v1.7.0/actionlint_1.7.0_darwin_arm64.tar.gz
+file_name = actionlint_1.7.1_darwin_arm64.tar.gz
+checksum = a72f66f28a4cc294670abb7a5e3392033700e00cc6a385c32fb769971b71ec9f
+url = https://github.com/rhysd/actionlint/releases/download/v1.7.1/actionlint_1.7.1_darwin_arm64.tar.gz
 
 [win32-AMD64]
-file_name = actionlint_1.7.0_windows_amd64.zip
-checksum = 2ecb1b4d3b54ee4503a0edeb29bdc910c5ef8826358698078905f485e0bab675
-url = https://github.com/rhysd/actionlint/releases/download/v1.7.0/actionlint_1.7.0_windows_amd64.zip
+file_name = actionlint_1.7.1_windows_amd64.zip
+checksum = 5dbecc21cf2ebe982a1ae5e029ee49f5be8ca3263a936c597323ed9331d896de
+url = https://github.com/rhysd/actionlint/releases/download/v1.7.1/actionlint_1.7.1_windows_amd64.zip
 
 [win32-ARM64]
-file_name = actionlint_1.7.0_windows_arm64.zip
-checksum = c2d9d30c7fdb4808a99a0800b768425b14132d4968ab01926f1bafa44b0f230a
-url = https://github.com/rhysd/actionlint/releases/download/v1.7.0/actionlint_1.7.0_windows_arm64.zip
+file_name = actionlint_1.7.1_windows_arm64.zip
+checksum = 84548356008900caa7aeaed73f60df48253550a5ecf42d6143d3e2690ff75446
+url = https://github.com/rhysd/actionlint/releases/download/v1.7.1/actionlint_1.7.1_windows_arm64.zip
 
 [cygwin-x86_64]
-file_name = actionlint_1.7.0_windows_amd64.zip
-checksum = 2ecb1b4d3b54ee4503a0edeb29bdc910c5ef8826358698078905f485e0bab675
-url = https://github.com/rhysd/actionlint/releases/download/v1.7.0/actionlint_1.7.0_windows_amd64.zip
+file_name = actionlint_1.7.1_windows_amd64.zip
+checksum = 5dbecc21cf2ebe982a1ae5e029ee49f5be8ca3263a936c597323ed9331d896de
+url = https://github.com/rhysd/actionlint/releases/download/v1.7.1/actionlint_1.7.1_windows_amd64.zip
```

### Comparing `actionlint_py-1.7.0.14/_custom_build/commands/fetch_binaries.py` & `actionlint_py-1.7.1.15/_custom_build/commands/fetch_binaries.py`

 * *Files identical despite different names*

### Comparing `actionlint_py-1.7.0.14/_custom_build/commands/install_actionlint.py` & `actionlint_py-1.7.1.15/_custom_build/commands/install_actionlint.py`

 * *Files identical despite different names*

### Comparing `actionlint_py-1.7.0.14/_custom_build/utils/file_ops.py` & `actionlint_py-1.7.1.15/_custom_build/utils/file_ops.py`

 * *Files identical despite different names*

### Comparing `actionlint_py-1.7.0.14/_custom_build/version.py` & `actionlint_py-1.7.1.15/_custom_build/version.py`

 * *Files identical despite different names*

### Comparing `actionlint_py-1.7.0.14/actionlint_py.egg-info/PKG-INFO` & `actionlint_py-1.7.1.15/actionlint_py.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: actionlint_py
-Version: 1.7.0.14
+Version: 1.7.1.15
 Summary: Python wrapper around invoking actionlint (https://github.com/rhysd/actionlint)
 Author-email: Ryan Rhee <pypi@rhee.io>, Mateusz Grzeliński <grzelinskimat@gmail.com>
 Maintainer-email: Mateusz Grzeliński <grzelinskimat@gmail.com>
 License: MIT License
         
         Copyright (c) 2019 Ryan Rhee
         
@@ -75,15 +75,15 @@
 
 Use this repo if you can not use officially supported hooks (docker, golang, system) and you are fine with python `pip` wrapper.
 
 Sample `.pre-commit-config.yaml` using `pip` as package manager:
 
 ```yaml
 - repo: https://github.com/Mateusz-Grzelinski/actionlint-py
-  rev: v1.7.0.14
+  rev: v1.7.1.15
   hooks:
     - id: actionlint
       additional_dependencies: [ pyflakes>=3.0.1, shellcheck-py>=0.9.0.5 ]
       # actionlint has built in support for pyflakes and shellcheck, sadly they will not be auto updated. Check https://pypi.org/project/actionlint-py/ for latest version. Alternatively:
       # args: [-shellcheck=/path/shellcheck -pyflakes=/path/pyflakes]
       # note - invalid path in arguments will fail silently
 ```
@@ -95,17 +95,17 @@
 ```yaml
 - repo: local
   hooks:
     - id: actionlint
       name: actionlint
       description: Lint GitHub workflows with actionlint
       additional_dependencies: [ actionlint-py ]
-      #additional_dependencies: [actionlint-py==1.7.0.14]
+      #additional_dependencies: [actionlint-py==1.7.1.15]
       # safer, but pre-commit autoupdate will not work
-      # note: the pip versioning scheme is different from actionlint binary: not "v1.7.0" but "1.7.0.14" (last number is build system version)
+      # note: the pip versioning scheme is different from actionlint binary: not "v1.7.1" but "1.7.1.15" (last number is build system version)
       entry: actionlint
       #args: [-ignore "*.set-output. was depracated.*"]
       language: python
       types: [ "yaml" ]
       files: "^.github/workflows/"
 ```
 
@@ -117,15 +117,15 @@
 
 ### As pre-commit hooks
 
 See [official docs for pre-commit integration](https://github.com/rhysd/actionlint/blob/main/docs/usage.md#pre-commit)
 
 ```yaml
 - repo: https://github.com/rhysd/actionlint
-  rev: v1.7.0
+  rev: v1.7.1
   hooks:
     - id: actionlint
     # - id: actionlint-docker
     # - id: actionlint-system
 ```
 
 ### Use as github action step
```

### Comparing `actionlint_py-1.7.0.14/actionlint_py.egg-info/SOURCES.txt` & `actionlint_py-1.7.1.15/actionlint_py.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `actionlint_py-1.7.0.14/pyproject.toml` & `actionlint_py-1.7.1.15/pyproject.toml`

 * *Files identical despite different names*

