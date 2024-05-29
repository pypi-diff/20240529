# Comparing `tmp/py-ard-1.1.3.tar.gz` & `tmp/py-ard-1.2.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "py-ard-1.1.3.tar", last modified: Tue May  7 20:57:12 2024, max compression
+gzip compressed data, was "py-ard-1.2.0.tar", last modified: Wed May 29 18:03:21 2024, max compression
```

## Comparing `py-ard-1.1.3.tar` & `py-ard-1.2.0.tar`

### file list

```diff
@@ -1,40 +1,40 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 20:57:12.710717 py-ard-1.1.3/
--rw-r--r--   0 runner    (1001) docker     (127)     3151 2024-05-07 20:57:03.000000 py-ard-1.1.3/CONTRIBUTING.rst
--rw-r--r--   0 runner    (1001) docker     (127)    35147 2024-05-07 20:57:03.000000 py-ard-1.1.3/COPYING
--rw-r--r--   0 runner    (1001) docker     (127)       89 2024-05-07 20:57:03.000000 py-ard-1.1.3/HISTORY.rst
--rw-r--r--   0 runner    (1001) docker     (127)     7652 2024-05-07 20:57:03.000000 py-ard-1.1.3/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)      344 2024-05-07 20:57:03.000000 py-ard-1.1.3/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (127)    20830 2024-05-07 20:57:12.710717 py-ard-1.1.3/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)    15967 2024-05-07 20:57:03.000000 py-ard-1.1.3/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 20:57:12.706717 py-ard-1.1.3/py_ard.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)    20830 2024-05-07 20:57:12.000000 py-ard-1.1.3/py_ard.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      642 2024-05-07 20:57:12.000000 py-ard-1.1.3/py_ard.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-07 20:57:12.000000 py-ard-1.1.3/py_ard.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-07 20:57:12.000000 py-ard-1.1.3/py_ard.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (127)       41 2024-05-07 20:57:12.000000 py-ard-1.1.3/py_ard.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)        6 2024-05-07 20:57:12.000000 py-ard-1.1.3/py_ard.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 20:57:12.710717 py-ard-1.1.3/pyard/
--rw-r--r--   0 runner    (1001) docker     (127)    12706 2024-05-07 20:57:03.000000 py-ard-1.1.3/pyard/CWD2.csv
--rw-r--r--   0 runner    (1001) docker     (127)     1595 2024-05-07 20:57:03.000000 py-ard-1.1.3/pyard/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    38295 2024-05-07 20:57:03.000000 py-ard-1.1.3/pyard/ard.py
--rw-r--r--   0 runner    (1001) docker     (127)     7628 2024-05-07 20:57:03.000000 py-ard-1.1.3/pyard/blender.py
--rw-r--r--   0 runner    (1001) docker     (127)     1593 2024-05-07 20:57:03.000000 py-ard-1.1.3/pyard/constants.py
--rw-r--r--   0 runner    (1001) docker     (127)    17513 2024-05-07 20:57:03.000000 py-ard-1.1.3/pyard/data_repository.py
--rw-r--r--   0 runner    (1001) docker     (127)    22303 2024-05-07 20:57:03.000000 py-ard-1.1.3/pyard/db.py
--rw-r--r--   0 runner    (1001) docker     (127)      316 2024-05-07 20:57:03.000000 py-ard-1.1.3/pyard/dna_relshp.csv
--rw-r--r--   0 runner    (1001) docker     (127)     2477 2024-05-07 20:57:03.000000 py-ard-1.1.3/pyard/drbx.py
--rw-r--r--   0 runner    (1001) docker     (127)     1793 2024-05-07 20:57:03.000000 py-ard-1.1.3/pyard/exceptions.py
--rw-r--r--   0 runner    (1001) docker     (127)    10163 2024-05-07 20:57:03.000000 py-ard-1.1.3/pyard/load.py
--rw-r--r--   0 runner    (1001) docker     (127)     1621 2024-05-07 20:57:03.000000 py-ard-1.1.3/pyard/mappings.py
--rw-r--r--   0 runner    (1001) docker     (127)     4691 2024-05-07 20:57:03.000000 py-ard-1.1.3/pyard/misc.py
--rw-r--r--   0 runner    (1001) docker     (127)     7912 2024-05-07 20:57:03.000000 py-ard-1.1.3/pyard/serology.py
--rw-r--r--   0 runner    (1001) docker     (127)     3758 2024-05-07 20:57:03.000000 py-ard-1.1.3/pyard/smart_sort.py
--rw-r--r--   0 runner    (1001) docker     (127)       46 2024-05-07 20:57:03.000000 py-ard-1.1.3/requirements-tests.txt
--rw-r--r--   0 runner    (1001) docker     (127)       41 2024-05-07 20:57:03.000000 py-ard-1.1.3/requirements.txt
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 20:57:12.710717 py-ard-1.1.3/scripts/
--rwxr-xr-x   0 runner    (1001) docker     (127)     6024 2024-05-07 20:57:03.000000 py-ard-1.1.3/scripts/pyard
--rwxr-xr-x   0 runner    (1001) docker     (127)     5195 2024-05-07 20:57:03.000000 py-ard-1.1.3/scripts/pyard-import
--rwxr-xr-x   0 runner    (1001) docker     (127)    15974 2024-05-07 20:57:03.000000 py-ard-1.1.3/scripts/pyard-reduce-csv
--rwxr-xr-x   0 runner    (1001) docker     (127)     4183 2024-05-07 20:57:03.000000 py-ard-1.1.3/scripts/pyard-status
--rw-r--r--   0 runner    (1001) docker     (127)      634 2024-05-07 20:57:12.710717 py-ard-1.1.3/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)     2535 2024-05-07 20:57:03.000000 py-ard-1.1.3/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-29 18:03:21.204545 py-ard-1.2.0/
+-rw-r--r--   0 runner    (1001) docker     (127)     3151 2024-05-29 18:03:07.000000 py-ard-1.2.0/CONTRIBUTING.rst
+-rw-r--r--   0 runner    (1001) docker     (127)    35147 2024-05-29 18:03:07.000000 py-ard-1.2.0/COPYING
+-rw-r--r--   0 runner    (1001) docker     (127)       89 2024-05-29 18:03:07.000000 py-ard-1.2.0/HISTORY.rst
+-rw-r--r--   0 runner    (1001) docker     (127)     7652 2024-05-29 18:03:07.000000 py-ard-1.2.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)      344 2024-05-29 18:03:07.000000 py-ard-1.2.0/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (127)    21193 2024-05-29 18:03:21.204545 py-ard-1.2.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)    16266 2024-05-29 18:03:07.000000 py-ard-1.2.0/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-29 18:03:21.200545 py-ard-1.2.0/py_ard.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)    21193 2024-05-29 18:03:20.000000 py-ard-1.2.0/py_ard.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      642 2024-05-29 18:03:21.000000 py-ard-1.2.0/py_ard.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-29 18:03:20.000000 py-ard-1.2.0/py_ard.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-29 18:03:20.000000 py-ard-1.2.0/py_ard.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (127)       41 2024-05-29 18:03:20.000000 py-ard-1.2.0/py_ard.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        6 2024-05-29 18:03:20.000000 py-ard-1.2.0/py_ard.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-29 18:03:21.204545 py-ard-1.2.0/pyard/
+-rw-r--r--   0 runner    (1001) docker     (127)    12706 2024-05-29 18:03:07.000000 py-ard-1.2.0/pyard/CWD2.csv
+-rw-r--r--   0 runner    (1001) docker     (127)     1595 2024-05-29 18:03:07.000000 py-ard-1.2.0/pyard/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    39521 2024-05-29 18:03:07.000000 py-ard-1.2.0/pyard/ard.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7628 2024-05-29 18:03:07.000000 py-ard-1.2.0/pyard/blender.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1593 2024-05-29 18:03:07.000000 py-ard-1.2.0/pyard/constants.py
+-rw-r--r--   0 runner    (1001) docker     (127)    17513 2024-05-29 18:03:07.000000 py-ard-1.2.0/pyard/data_repository.py
+-rw-r--r--   0 runner    (1001) docker     (127)    22303 2024-05-29 18:03:07.000000 py-ard-1.2.0/pyard/db.py
+-rw-r--r--   0 runner    (1001) docker     (127)      316 2024-05-29 18:03:07.000000 py-ard-1.2.0/pyard/dna_relshp.csv
+-rw-r--r--   0 runner    (1001) docker     (127)     2477 2024-05-29 18:03:07.000000 py-ard-1.2.0/pyard/drbx.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1793 2024-05-29 18:03:07.000000 py-ard-1.2.0/pyard/exceptions.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10163 2024-05-29 18:03:07.000000 py-ard-1.2.0/pyard/load.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1621 2024-05-29 18:03:07.000000 py-ard-1.2.0/pyard/mappings.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4691 2024-05-29 18:03:07.000000 py-ard-1.2.0/pyard/misc.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7912 2024-05-29 18:03:07.000000 py-ard-1.2.0/pyard/serology.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3758 2024-05-29 18:03:07.000000 py-ard-1.2.0/pyard/smart_sort.py
+-rw-r--r--   0 runner    (1001) docker     (127)       46 2024-05-29 18:03:07.000000 py-ard-1.2.0/requirements-tests.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       41 2024-05-29 18:03:07.000000 py-ard-1.2.0/requirements.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-29 18:03:21.204545 py-ard-1.2.0/scripts/
+-rwxr-xr-x   0 runner    (1001) docker     (127)     6024 2024-05-29 18:03:07.000000 py-ard-1.2.0/scripts/pyard
+-rwxr-xr-x   0 runner    (1001) docker     (127)     5195 2024-05-29 18:03:07.000000 py-ard-1.2.0/scripts/pyard-import
+-rwxr-xr-x   0 runner    (1001) docker     (127)    15974 2024-05-29 18:03:07.000000 py-ard-1.2.0/scripts/pyard-reduce-csv
+-rwxr-xr-x   0 runner    (1001) docker     (127)     4183 2024-05-29 18:03:07.000000 py-ard-1.2.0/scripts/pyard-status
+-rw-r--r--   0 runner    (1001) docker     (127)      634 2024-05-29 18:03:21.204545 py-ard-1.2.0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)     2535 2024-05-29 18:03:07.000000 py-ard-1.2.0/setup.py
```

### Comparing `py-ard-1.1.3/CONTRIBUTING.rst` & `py-ard-1.2.0/CONTRIBUTING.rst`

 * *Files identical despite different names*

### Comparing `py-ard-1.1.3/COPYING` & `py-ard-1.2.0/COPYING`

 * *Files identical despite different names*

### Comparing `py-ard-1.1.3/LICENSE` & `py-ard-1.2.0/LICENSE`

 * *Files identical despite different names*

### Comparing `py-ard-1.1.3/PKG-INFO` & `py-ard-1.2.0/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: py-ard
-Version: 1.1.3
+Version: 1.2.0
 Summary: ARD reduction for HLA with Python
 Home-page: https://github.com/nmdp-bioinformatics/py-ard
 Author: CIBMTR
 Author-email: cibmtr-pypi@nmdp.org
 License: LGPL 3.0
 Description: # py-ard
         
@@ -12,17 +12,19 @@
         
         [![PyPi Version](https://img.shields.io/pypi/v/py-ard.svg)](https://pypi.python.org/pypi/py-ard)
         
         ![py-ard-logo.png](images/py-ard-logo.png)
         
         **Note:**
         
-        Release `1.1.1` has extensive Serolgy related updates and affects Serology related data. Please rebuild the cache database if there's a missing Serology error.
+        - `ping` mode is default. When in `ping` mode, alleles that do not have a G group, their corresponding P group is used.
+        
+        - Release `1.1.1` has extensive Serolgy related updates and affects Serology related data. Please rebuild the cache database if there's a missing Serology error.
         ```
-        pyard-import --re-install
+           pyard-import --re-install
         ```
         
         Or set `py-ard` requirements to be `py-ard<=1.1.1` for your dependency.
         
         
         ---
         
@@ -89,39 +91,52 @@
         brew install py-ard
         ```
         
         Homebrew will notify you as new versions of `py-ard` are released.
         
         ### Install from source
         
+        Checkout the `py-ard` source code.
+        
         ```shell
-        python3 -m venv venv
+        git clone https://github.com/nmdp-bioinformatics/py-ard.git
+        cd py-ard
+        ```
+        
+        Create and activate virtual environment. Install the py-ard dependencies.
+        
+        ```shell
+        make venv
+        
         source venv/bin/activate
         
-        python setup.py install
+        make install
         ```
         
         See [Our Contribution Guide](CONTRIBUTING.rst) for open source contribution to `py-ard`.
         
         ## Using `py-ard`
         
         ### Using `py-ard` from Python code
         
         `py-ard` can be used in a program to reduce/expand HLA GL String representation. If pyard discovers an invalid Allele,
         it'll throw an Invalid Exception, not silently return an empty result.
         
         #### Initialize `py-ard`
         
-        Import `pyard` package.
+        Import and initialize `pyard` package.
+        The default initialization is to use the latest version of IPD-IMGT/HLA database.
         
         ```python
         import pyard
+        
+        ard = pyard.init()
         ```
         
-        Initialize `ARD` object with a version of IMGT HLA database
+        Initialize `py-ard` with a particular version of IPD/IMGT-HLA database.
         
         ```python
         import pyard
         
         ard = pyard.init('3510')
         ```
         
@@ -148,21 +163,14 @@
         
         As MAC data changes frequently, you can choose to refresh the MAC code for current IMGT HLA database version.
         
         ```python
         ard.refresh_mac_codes()
         ```
         
-        The default initialization is to use the latest version of IPD-IMGT/HLA database.
-        
-        ```python
-        import pyard
-        
-        ard = pyard.init()
-        ```
         
         You can check the current version of IPD-IMGT/HLA database.
         
         ```python
         ard.get_db_version()
         ```
```

### Comparing `py-ard-1.1.3/README.md` & `py-ard-1.2.0/README.md`

 * *Files 2% similar despite different names*

```diff
@@ -4,17 +4,19 @@
 
 [![PyPi Version](https://img.shields.io/pypi/v/py-ard.svg)](https://pypi.python.org/pypi/py-ard)
 
 ![py-ard-logo.png](images/py-ard-logo.png)
 
 **Note:**
 
-Release `1.1.1` has extensive Serolgy related updates and affects Serology related data. Please rebuild the cache database if there's a missing Serology error.
+- `ping` mode is default. When in `ping` mode, alleles that do not have a G group, their corresponding P group is used.
+
+- Release `1.1.1` has extensive Serolgy related updates and affects Serology related data. Please rebuild the cache database if there's a missing Serology error.
 ```
-pyard-import --re-install
+   pyard-import --re-install
 ```
 
 Or set `py-ard` requirements to be `py-ard<=1.1.1` for your dependency.
 
 
 ---
 
@@ -81,39 +83,52 @@
 brew install py-ard
 ```
 
 Homebrew will notify you as new versions of `py-ard` are released.
 
 ### Install from source
 
+Checkout the `py-ard` source code.
+
 ```shell
-python3 -m venv venv
+git clone https://github.com/nmdp-bioinformatics/py-ard.git
+cd py-ard
+```
+
+Create and activate virtual environment. Install the py-ard dependencies.
+
+```shell
+make venv
+
 source venv/bin/activate
 
-python setup.py install
+make install
 ```
 
 See [Our Contribution Guide](CONTRIBUTING.rst) for open source contribution to `py-ard`.
 
 ## Using `py-ard`
 
 ### Using `py-ard` from Python code
 
 `py-ard` can be used in a program to reduce/expand HLA GL String representation. If pyard discovers an invalid Allele,
 it'll throw an Invalid Exception, not silently return an empty result.
 
 #### Initialize `py-ard`
 
-Import `pyard` package.
+Import and initialize `pyard` package.
+The default initialization is to use the latest version of IPD-IMGT/HLA database.
 
 ```python
 import pyard
+
+ard = pyard.init()
 ```
 
-Initialize `ARD` object with a version of IMGT HLA database
+Initialize `py-ard` with a particular version of IPD/IMGT-HLA database.
 
 ```python
 import pyard
 
 ard = pyard.init('3510')
 ```
 
@@ -140,21 +155,14 @@
 
 As MAC data changes frequently, you can choose to refresh the MAC code for current IMGT HLA database version.
 
 ```python
 ard.refresh_mac_codes()
 ```
 
-The default initialization is to use the latest version of IPD-IMGT/HLA database.
-
-```python
-import pyard
-
-ard = pyard.init()
-```
 
 You can check the current version of IPD-IMGT/HLA database.
 
 ```python
 ard.get_db_version()
 ```
```

### Comparing `py-ard-1.1.3/py_ard.egg-info/PKG-INFO` & `py-ard-1.2.0/py_ard.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: py-ard
-Version: 1.1.3
+Version: 1.2.0
 Summary: ARD reduction for HLA with Python
 Home-page: https://github.com/nmdp-bioinformatics/py-ard
 Author: CIBMTR
 Author-email: cibmtr-pypi@nmdp.org
 License: LGPL 3.0
 Description: # py-ard
         
@@ -12,17 +12,19 @@
         
         [![PyPi Version](https://img.shields.io/pypi/v/py-ard.svg)](https://pypi.python.org/pypi/py-ard)
         
         ![py-ard-logo.png](images/py-ard-logo.png)
         
         **Note:**
         
-        Release `1.1.1` has extensive Serolgy related updates and affects Serology related data. Please rebuild the cache database if there's a missing Serology error.
+        - `ping` mode is default. When in `ping` mode, alleles that do not have a G group, their corresponding P group is used.
+        
+        - Release `1.1.1` has extensive Serolgy related updates and affects Serology related data. Please rebuild the cache database if there's a missing Serology error.
         ```
-        pyard-import --re-install
+           pyard-import --re-install
         ```
         
         Or set `py-ard` requirements to be `py-ard<=1.1.1` for your dependency.
         
         
         ---
         
@@ -89,39 +91,52 @@
         brew install py-ard
         ```
         
         Homebrew will notify you as new versions of `py-ard` are released.
         
         ### Install from source
         
+        Checkout the `py-ard` source code.
+        
         ```shell
-        python3 -m venv venv
+        git clone https://github.com/nmdp-bioinformatics/py-ard.git
+        cd py-ard
+        ```
+        
+        Create and activate virtual environment. Install the py-ard dependencies.
+        
+        ```shell
+        make venv
+        
         source venv/bin/activate
         
-        python setup.py install
+        make install
         ```
         
         See [Our Contribution Guide](CONTRIBUTING.rst) for open source contribution to `py-ard`.
         
         ## Using `py-ard`
         
         ### Using `py-ard` from Python code
         
         `py-ard` can be used in a program to reduce/expand HLA GL String representation. If pyard discovers an invalid Allele,
         it'll throw an Invalid Exception, not silently return an empty result.
         
         #### Initialize `py-ard`
         
-        Import `pyard` package.
+        Import and initialize `pyard` package.
+        The default initialization is to use the latest version of IPD-IMGT/HLA database.
         
         ```python
         import pyard
+        
+        ard = pyard.init()
         ```
         
-        Initialize `ARD` object with a version of IMGT HLA database
+        Initialize `py-ard` with a particular version of IPD/IMGT-HLA database.
         
         ```python
         import pyard
         
         ard = pyard.init('3510')
         ```
         
@@ -148,21 +163,14 @@
         
         As MAC data changes frequently, you can choose to refresh the MAC code for current IMGT HLA database version.
         
         ```python
         ard.refresh_mac_codes()
         ```
         
-        The default initialization is to use the latest version of IPD-IMGT/HLA database.
-        
-        ```python
-        import pyard
-        
-        ard = pyard.init()
-        ```
         
         You can check the current version of IPD-IMGT/HLA database.
         
         ```python
         ard.get_db_version()
         ```
```

### Comparing `py-ard-1.1.3/py_ard.egg-info/SOURCES.txt` & `py-ard-1.2.0/py_ard.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `py-ard-1.1.3/pyard/CWD2.csv` & `py-ard-1.2.0/pyard/CWD2.csv`

 * *Files identical despite different names*

### Comparing `py-ard-1.1.3/pyard/__init__.py` & `py-ard-1.2.0/pyard/__init__.py`

 * *Files 0% similar despite different names*

```diff
@@ -22,15 +22,15 @@
 #    > http://www.opensource.org/licenses/lgpl-license.php
 #
 from .blender import blender as dr_blender
 from .constants import DEFAULT_CACHE_SIZE
 from .misc import get_imgt_db_versions as db_versions
 
 __author__ = """NMDP Bioinformatics"""
-__version__ = "1.1.3"
+__version__ = "1.2.0"
 
 
 def init(
     imgt_version: str = "Latest",
     data_dir: str = None,
     load_mac: bool = True,
     cache_size: int = DEFAULT_CACHE_SIZE,
```

### Comparing `py-ard-1.1.3/pyard/ard.py` & `py-ard-1.2.0/pyard/ard.py`

 * *Files 1% similar despite different names*

```diff
@@ -52,15 +52,15 @@
     "reduce_serology": True,
     "reduce_v2": True,
     "reduce_3field": True,
     "reduce_P": True,
     "reduce_XX": True,
     "reduce_MAC": True,
     "reduce_shortnull": True,
-    "ping": False,
+    "ping": True,
     "map_drb345_to_drbx": True,
     "verbose_log": False,
     "ARS_as_lg": False,
     "strict": True,
 }
 
 
@@ -202,19 +202,41 @@
         # C*12:02:02    => C*12:02:01G
         # C*12:02       => C*12:02:01G
 
         if allele.endswith(("P", "G")):
             if redux_type in ["lg", "lgx", "G"]:
                 allele = allele[:-1]
         if self._config["ping"] and re_ping:
+            # ping: alleles that are in P group but not in G groups are defined
+            # for 2-field alleles. If not already in 2-field form, reduce it to
+            # 2-field version first then re-reduce it to P group.
             if redux_type in ("lg", "lgx", "U2"):
                 if allele in self.ars_mappings.p_not_g:
-                    return self.ars_mappings.p_not_g[allele]
+                    not_g_allele = self.ars_mappings.p_not_g[allele]
+                    if redux_type == "lg":
+                        return self._add_lg_suffix(not_g_allele)
+                    return not_g_allele
                 else:
-                    return self._redux_allele(allele, redux_type, False)
+                    redux_allele = self._redux_allele(allele, redux_type, False)
+                    if redux_allele.endswith("g"):
+                        no_suffix_allele = redux_allele[:-1]
+                    elif redux_allele.endswith("ARS"):
+                        no_suffix_allele = redux_allele[:-3]
+                    else:
+                        no_suffix_allele = redux_allele
+                    if (
+                        no_suffix_allele == allele
+                        or no_suffix_allele in self.ars_mappings.p_not_g.values()
+                    ):
+                        return redux_allele
+                    redux_allele = self._redux_allele(
+                        no_suffix_allele, redux_type, True
+                    )
+                    if self._is_valid_allele(redux_allele):
+                        return redux_allele
 
         if redux_type == "G" and allele in self.ars_mappings.g_group:
             if allele in self.ars_mappings.dup_g:
                 return self.ars_mappings.dup_g[allele]
             else:
                 return self.ars_mappings.g_group[allele]
         elif redux_type == "P" and allele in self.ars_mappings.p_group:
@@ -225,19 +247,15 @@
             elif allele in self.ars_mappings.lgx_group:
                 redux_allele = self.ars_mappings.lgx_group[allele]
             else:
                 # for 'lgx' or 'lg' mode when allele is not in G group,
                 # return allele with only first 2 field
                 redux_allele = ":".join(allele.split(":")[0:2])
             if redux_type == "lg":
-                # ARS suffix maybe used instead of g
-                if self._config["ARS_as_lg"]:
-                    return redux_allele + "ARS"
-                # lg mode has g appended with lgx reduction
-                return redux_allele + "g"
+                return self._add_lg_suffix(redux_allele)
             return redux_allele
         elif redux_type == "W":
             # new redux_type which is full WHO expansion
             if self._is_who_allele(allele):
                 return allele
             if allele in self.code_mappings.who_group:
                 return self.redux(
@@ -315,14 +333,21 @@
                     return allele
 
             if self._is_allele_in_db(allele):
                 return allele
             else:
                 raise InvalidAlleleError(f"{allele} is an invalid allele.")
 
+    def _add_lg_suffix(self, redux_allele):
+        # ARS suffix maybe used instead of g
+        if self._config["ARS_as_lg"]:
+            return redux_allele + "ARS"
+        # lg mode has g appended with lgx reduction
+        return redux_allele + "g"
+
     def _get_non_strict_allele(self, allele):
         """
         In non-strict mode, if the allele is not valid,
         try it with expression characters suffixed
 
         @param allele: allele that might have non-strict version
         @return: non-strict version of the allele if it exists
```

### Comparing `py-ard-1.1.3/pyard/blender.py` & `py-ard-1.2.0/pyard/blender.py`

 * *Files identical despite different names*

### Comparing `py-ard-1.1.3/pyard/constants.py` & `py-ard-1.2.0/pyard/constants.py`

 * *Files identical despite different names*

### Comparing `py-ard-1.1.3/pyard/data_repository.py` & `py-ard-1.2.0/pyard/data_repository.py`

 * *Files identical despite different names*

### Comparing `py-ard-1.1.3/pyard/db.py` & `py-ard-1.2.0/pyard/db.py`

 * *Files identical despite different names*

### Comparing `py-ard-1.1.3/pyard/drbx.py` & `py-ard-1.2.0/pyard/drbx.py`

 * *Files identical despite different names*

### Comparing `py-ard-1.1.3/pyard/exceptions.py` & `py-ard-1.2.0/pyard/exceptions.py`

 * *Files identical despite different names*

### Comparing `py-ard-1.1.3/pyard/load.py` & `py-ard-1.2.0/pyard/load.py`

 * *Files identical despite different names*

### Comparing `py-ard-1.1.3/pyard/mappings.py` & `py-ard-1.2.0/pyard/mappings.py`

 * *Files identical despite different names*

### Comparing `py-ard-1.1.3/pyard/misc.py` & `py-ard-1.2.0/pyard/misc.py`

 * *Files identical despite different names*

### Comparing `py-ard-1.1.3/pyard/serology.py` & `py-ard-1.2.0/pyard/serology.py`

 * *Files identical despite different names*

### Comparing `py-ard-1.1.3/pyard/smart_sort.py` & `py-ard-1.2.0/pyard/smart_sort.py`

 * *Files identical despite different names*

### Comparing `py-ard-1.1.3/scripts/pyard` & `py-ard-1.2.0/scripts/pyard`

 * *Files identical despite different names*

### Comparing `py-ard-1.1.3/scripts/pyard-import` & `py-ard-1.2.0/scripts/pyard-import`

 * *Files identical despite different names*

### Comparing `py-ard-1.1.3/scripts/pyard-reduce-csv` & `py-ard-1.2.0/scripts/pyard-reduce-csv`

 * *Files identical despite different names*

### Comparing `py-ard-1.1.3/scripts/pyard-status` & `py-ard-1.2.0/scripts/pyard-status`

 * *Files identical despite different names*

### Comparing `py-ard-1.1.3/setup.cfg` & `py-ard-1.2.0/setup.cfg`

 * *Files 2% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 [bumpversion]
-current_version = 1.1.3
+current_version = 1.2.0
 commit = True
 tag = True
 
 [bumpversion:file:setup.py]
 search = version="{current_version}"
 replace = version="{new_version}"
```

### Comparing `py-ard-1.1.3/setup.py` & `py-ard-1.2.0/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -32,15 +32,15 @@
     requirements = requirements_file.read().split("\n")
 
 with open("requirements-tests.txt") as requirements_file:
     test_requirements = requirements_file.read().split("\n")
 
 setup(
     name="py-ard",
-    version="1.1.3",
+    version="1.2.0",
     description="ARD reduction for HLA with Python",
     long_description=readme,
     long_description_content_type="text/markdown",
     author="CIBMTR",
     author_email="cibmtr-pypi@nmdp.org",
     url="https://github.com/nmdp-bioinformatics/py-ard",
     packages=[
```

