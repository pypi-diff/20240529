# Comparing `tmp/deinterf-0.1.0.tar.gz` & `tmp/deinterf-1.0.0.tar.gz`

## Comparing `deinterf-0.1.0.tar` & `deinterf-1.0.0.tar`

### file list

```diff
@@ -1,10 +1,26 @@
--rw-r--r--   0        0        0       44 2020-02-02 00:00:00.000000 deinterf-0.1.0/requirements.txt
--rw-r--r--   0        0        0       50 2020-02-02 00:00:00.000000 deinterf-0.1.0/deinterf/__init__.py
--rw-r--r--   0        0        0     6059 2020-02-02 00:00:00.000000 deinterf-0.1.0/deinterf/compensator.py
--rw-r--r--   0        0        0      946 2020-02-02 00:00:00.000000 deinterf-0.1.0/example/main_compensator.py
--rw-r--r--   0        0        0  1570834 2020-02-02 00:00:00.000000 deinterf-0.1.0/example/test_data.csv
--rw-r--r--   0        0        0     3238 2020-02-02 00:00:00.000000 deinterf-0.1.0/.gitignore
--rw-r--r--   0        0        0     1087 2020-02-02 00:00:00.000000 deinterf-0.1.0/LICENSE
--rw-r--r--   0        0        0     1108 2020-02-02 00:00:00.000000 deinterf-0.1.0/README.md
--rw-r--r--   0        0        0      708 2020-02-02 00:00:00.000000 deinterf-0.1.0/pyproject.toml
--rw-r--r--   0        0        0     1627 2020-02-02 00:00:00.000000 deinterf-0.1.0/PKG-INFO
+-rw-r--r--   0        0        0       74 2020-02-02 00:00:00.000000 deinterf-1.0.0/requirements.txt
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 deinterf-1.0.0/deinterf/__init__.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 deinterf-1.0.0/deinterf/compensator/__init__.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 deinterf-1.0.0/deinterf/compensator/tmi/__init__.py
+-rw-r--r--   0        0        0       65 2020-02-02 00:00:00.000000 deinterf-1.0.0/deinterf/compensator/tmi/linear/__init__.py
+-rw-r--r--   0        0        0     2244 2020-02-02 00:00:00.000000 deinterf-1.0.0/deinterf/compensator/tmi/linear/_term.py
+-rw-r--r--   0        0        0      486 2020-02-02 00:00:00.000000 deinterf-1.0.0/deinterf/compensator/tmi/linear/terms.py
+-rw-r--r--   0        0        0     3689 2020-02-02 00:00:00.000000 deinterf-1.0.0/deinterf/compensator/tmi/linear/tolles_lawson.py
+-rw-r--r--   0        0        0       48 2020-02-02 00:00:00.000000 deinterf-1.0.0/deinterf/foundation/__init__.py
+-rw-r--r--   0        0        0     1185 2020-02-02 00:00:00.000000 deinterf-1.0.0/deinterf/foundation/_term.py
+-rw-r--r--   0        0        0     1684 2020-02-02 00:00:00.000000 deinterf-1.0.0/deinterf/foundation/sensors.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 deinterf-1.0.0/deinterf/metrics/__init__.py
+-rw-r--r--   0        0        0     2086 2020-02-02 00:00:00.000000 deinterf-1.0.0/deinterf/metrics/fom.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 deinterf-1.0.0/deinterf/utils/__init__.py
+-rw-r--r--   0        0        0     1244 2020-02-02 00:00:00.000000 deinterf-1.0.0/deinterf/utils/filter.py
+-rw-r--r--   0        0        0     1714 2020-02-02 00:00:00.000000 deinterf-1.0.0/deinterf/utils/transform.py
+-rw-r--r--   0        0        0      126 2020-02-02 00:00:00.000000 deinterf-1.0.0/deinterf/utils/data_ioc/__init__.py
+-rw-r--r--   0        0        0    20030 2020-02-02 00:00:00.000000 deinterf-1.0.0/deinterf/utils/data_ioc/_data.py
+-rw-r--r--   0        0        0     1946 2020-02-02 00:00:00.000000 deinterf-1.0.0/deinterf/utils/data_ioc/_data_ndarray.py
+-rw-r--r--   0        0        0     1570 2020-02-02 00:00:00.000000 deinterf-1.0.0/examples/compensate_tmi.py
+-rw-r--r--   0        0        0     3902 2020-02-02 00:00:00.000000 deinterf-1.0.0/examples/compensate_tmi_extended.py
+-rw-r--r--   0        0        0     3255 2020-02-02 00:00:00.000000 deinterf-1.0.0/.gitignore
+-rw-r--r--   0        0        0     1087 2020-02-02 00:00:00.000000 deinterf-1.0.0/LICENSE
+-rw-r--r--   0        0        0     6750 2020-02-02 00:00:00.000000 deinterf-1.0.0/README.md
+-rw-r--r--   0        0        0      767 2020-02-02 00:00:00.000000 deinterf-1.0.0/pyproject.toml
+-rw-r--r--   0        0        0     7166 2020-02-02 00:00:00.000000 deinterf-1.0.0/PKG-INFO
```

### Comparing `deinterf-0.1.0/.gitignore` & `deinterf-1.0.0/.gitignore`

 * *Files 1% similar despite different names*

```diff
@@ -1,7 +1,9 @@
+.cenv
+.vscode/
 # Byte-compiled / optimized / DLL files
 __pycache__/
 *.py[cod]
 *$py.class
 
 # C extensions
 *.so
```

### Comparing `deinterf-0.1.0/LICENSE` & `deinterf-1.0.0/LICENSE`

 * *Files identical despite different names*

### Comparing `deinterf-0.1.0/pyproject.toml` & `deinterf-1.0.0/pyproject.toml`

 * *Files 12% similar despite different names*

```diff
@@ -1,22 +1,24 @@
 # Project Metadata
 [project]
 name = "deinterf"
-version = "0.1.0"
+version = "1.0.0"
 description = "Aeromagnetic Data Compensation for Magnetic Interference"
 readme = "README.md"
 
 # Requirements
 requires-python = ">=3.9"
 dependencies = [
-    "numpy>=1.24.4", 
-    "scipy>=1.11.1", 
-    "pandas>=2.0.3", 
-    "loguru>=0.7.0", 
-    "scikit-learn>=1.3.0"
+    "numpy>=1.26.4", 
+    "scipy>=1.12.0", 
+    "scikit-learn>=1.4.0",
+    "typing-extensions>=4.10.0",
+    "sgl2020>=0.1.1",
+    "matplotlib>=3.8.3",
+    "ppigrf>=1.0.2"
 ]
 
 # Author Info
 authors = [ { name = "dorian", email = "dorian.li@outlook.com" } ]
 
 # Project Classifiers
 classifiers = [
```

