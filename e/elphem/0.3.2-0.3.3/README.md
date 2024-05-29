# Comparing `tmp/elphem-0.3.2.tar.gz` & `tmp/elphem-0.3.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "elphem-0.3.2.tar", last modified: Tue May 28 06:53:03 2024, max compression
+gzip compressed data, was "elphem-0.3.3.tar", last modified: Wed May 29 13:49:27 2024, max compression
```

## Comparing `elphem-0.3.2.tar` & `elphem-0.3.3.tar`

### file list

```diff
@@ -1,60 +1,60 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-28 06:53:03.624229 elphem-0.3.2/
--rw-r--r--   0 runner    (1001) docker     (127)     1068 2024-05-28 06:52:59.000000 elphem-0.3.2/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)     8098 2024-05-28 06:53:03.620229 elphem-0.3.2/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     7433 2024-05-28 06:52:59.000000 elphem-0.3.2/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-28 06:53:03.616228 elphem-0.3.2/elphem/
--rw-r--r--   0 runner    (1001) docker     (127)      110 2024-05-28 06:52:59.000000 elphem-0.3.2/elphem/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-28 06:53:03.616228 elphem-0.3.2/elphem/common/
--rw-r--r--   0 runner    (1001) docker     (127)      147 2024-05-28 06:52:59.000000 elphem-0.3.2/elphem/common/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     3150 2024-05-28 06:52:59.000000 elphem-0.3.2/elphem/common/atomic_weight.py
--rw-r--r--   0 runner    (1001) docker     (127)     3035 2024-05-28 06:52:59.000000 elphem-0.3.2/elphem/common/brillouin.py
--rw-r--r--   0 runner    (1001) docker     (127)     2839 2024-05-28 06:52:59.000000 elphem-0.3.2/elphem/common/distribution.py
--rw-r--r--   0 runner    (1001) docker     (127)     1011 2024-05-28 06:52:59.000000 elphem-0.3.2/elphem/common/function.py
--rw-r--r--   0 runner    (1001) docker     (127)      923 2024-05-28 06:52:59.000000 elphem-0.3.2/elphem/common/stdout.py
--rw-r--r--   0 runner    (1001) docker     (127)     3006 2024-05-28 06:52:59.000000 elphem-0.3.2/elphem/common/unit.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-28 06:53:03.616228 elphem-0.3.2/elphem/electron/
--rw-r--r--   0 runner    (1001) docker     (127)       23 2024-05-28 06:52:59.000000 elphem-0.3.2/elphem/electron/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     8663 2024-05-28 06:52:59.000000 elphem-0.3.2/elphem/electron/electron.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-28 06:53:03.620229 elphem-0.3.2/elphem/elph/
--rw-r--r--   0 runner    (1001) docker     (127)       30 2024-05-28 06:52:59.000000 elphem-0.3.2/elphem/elph/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    10519 2024-05-28 06:52:59.000000 elphem-0.3.2/elphem/elph/electron_phonon.py
--rw-r--r--   0 runner    (1001) docker     (127)     2926 2024-05-28 06:52:59.000000 elphem-0.3.2/elphem/elph/green_function.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-28 06:53:03.620229 elphem-0.3.2/elphem/lattice/
--rw-r--r--   0 runner    (1001) docker     (127)      118 2024-05-28 06:52:59.000000 elphem-0.3.2/elphem/lattice/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1354 2024-05-28 06:52:59.000000 elphem-0.3.2/elphem/lattice/cell.py
--rw-r--r--   0 runner    (1001) docker     (127)     4831 2024-05-28 06:52:59.000000 elphem-0.3.2/elphem/lattice/lattice.py
--rw-r--r--   0 runner    (1001) docker     (127)     1978 2024-05-28 06:52:59.000000 elphem-0.3.2/elphem/lattice/lattice_constant.py
--rw-r--r--   0 runner    (1001) docker     (127)      431 2024-05-28 06:52:59.000000 elphem-0.3.2/elphem/lattice/path.py
--rw-r--r--   0 runner    (1001) docker     (127)     4307 2024-05-28 06:52:59.000000 elphem-0.3.2/elphem/lattice/primitive_cell.py
--rw-r--r--   0 runner    (1001) docker     (127)    12162 2024-05-28 06:52:59.000000 elphem-0.3.2/elphem/lattice/reciprocal_cell.py
--rw-r--r--   0 runner    (1001) docker     (127)     6898 2024-05-28 06:52:59.000000 elphem-0.3.2/elphem/lattice/rotation.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-28 06:53:03.620229 elphem-0.3.2/elphem/phonon/
--rw-r--r--   0 runner    (1001) docker     (127)       21 2024-05-28 06:52:59.000000 elphem-0.3.2/elphem/phonon/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     6254 2024-05-28 06:52:59.000000 elphem-0.3.2/elphem/phonon/phonon.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-28 06:53:03.620229 elphem-0.3.2/elphem.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     8098 2024-05-28 06:53:03.000000 elphem-0.3.2/elphem.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     1156 2024-05-28 06:53:03.000000 elphem-0.3.2/elphem.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-28 06:53:03.000000 elphem-0.3.2/elphem.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       12 2024-05-28 06:53:03.000000 elphem-0.3.2/elphem.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       13 2024-05-28 06:53:03.000000 elphem-0.3.2/elphem.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-28 06:53:03.624229 elphem-0.3.2/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)     1234 2024-05-28 06:52:59.000000 elphem-0.3.2/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-28 06:53:03.620229 elphem-0.3.2/tests/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-28 06:52:59.000000 elphem-0.3.2/tests/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-28 06:53:03.620229 elphem-0.3.2/tests/common/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-28 06:52:59.000000 elphem-0.3.2/tests/common/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      409 2024-05-28 06:52:59.000000 elphem-0.3.2/tests/common/test_atomic_weight.py
--rw-r--r--   0 runner    (1001) docker     (127)      876 2024-05-28 06:52:59.000000 elphem-0.3.2/tests/common/test_brillouin.py
--rw-r--r--   0 runner    (1001) docker     (127)      514 2024-05-28 06:52:59.000000 elphem-0.3.2/tests/common/test_unit.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-28 06:53:03.620229 elphem-0.3.2/tests/electron/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-28 06:52:59.000000 elphem-0.3.2/tests/electron/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1406 2024-05-28 06:52:59.000000 elphem-0.3.2/tests/electron/test_electron.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-28 06:53:03.620229 elphem-0.3.2/tests/elph/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-28 06:52:59.000000 elphem-0.3.2/tests/elph/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2116 2024-05-28 06:52:59.000000 elphem-0.3.2/tests/elph/test_self_energy.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-28 06:53:03.620229 elphem-0.3.2/tests/lattice/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-28 06:52:59.000000 elphem-0.3.2/tests/lattice/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      755 2024-05-28 06:52:59.000000 elphem-0.3.2/tests/lattice/test_lattice.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-28 06:53:03.620229 elphem-0.3.2/tests/phonon/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-28 06:52:59.000000 elphem-0.3.2/tests/phonon/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1392 2024-05-28 06:52:59.000000 elphem-0.3.2/tests/phonon/test_phonon.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-29 13:49:27.963654 elphem-0.3.3/
+-rw-r--r--   0 runner    (1001) docker     (127)     1068 2024-05-29 13:49:23.000000 elphem-0.3.3/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)     8099 2024-05-29 13:49:27.963654 elphem-0.3.3/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     7434 2024-05-29 13:49:23.000000 elphem-0.3.3/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-29 13:49:27.955654 elphem-0.3.3/elphem/
+-rw-r--r--   0 runner    (1001) docker     (127)      110 2024-05-29 13:49:23.000000 elphem-0.3.3/elphem/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-29 13:49:27.959654 elphem-0.3.3/elphem/common/
+-rw-r--r--   0 runner    (1001) docker     (127)      147 2024-05-29 13:49:23.000000 elphem-0.3.3/elphem/common/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3150 2024-05-29 13:49:23.000000 elphem-0.3.3/elphem/common/atomic_weight.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3035 2024-05-29 13:49:23.000000 elphem-0.3.3/elphem/common/brillouin.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2839 2024-05-29 13:49:23.000000 elphem-0.3.3/elphem/common/distribution.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1011 2024-05-29 13:49:23.000000 elphem-0.3.3/elphem/common/function.py
+-rw-r--r--   0 runner    (1001) docker     (127)      923 2024-05-29 13:49:23.000000 elphem-0.3.3/elphem/common/stdout.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3006 2024-05-29 13:49:23.000000 elphem-0.3.3/elphem/common/unit.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-29 13:49:27.959654 elphem-0.3.3/elphem/electron/
+-rw-r--r--   0 runner    (1001) docker     (127)       23 2024-05-29 13:49:23.000000 elphem-0.3.3/elphem/electron/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8663 2024-05-29 13:49:23.000000 elphem-0.3.3/elphem/electron/electron.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-29 13:49:27.959654 elphem-0.3.3/elphem/elph/
+-rw-r--r--   0 runner    (1001) docker     (127)       30 2024-05-29 13:49:23.000000 elphem-0.3.3/elphem/elph/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10519 2024-05-29 13:49:23.000000 elphem-0.3.3/elphem/elph/electron_phonon.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2926 2024-05-29 13:49:23.000000 elphem-0.3.3/elphem/elph/green_function.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-29 13:49:27.963654 elphem-0.3.3/elphem/lattice/
+-rw-r--r--   0 runner    (1001) docker     (127)      118 2024-05-29 13:49:23.000000 elphem-0.3.3/elphem/lattice/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1354 2024-05-29 13:49:23.000000 elphem-0.3.3/elphem/lattice/cell.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4831 2024-05-29 13:49:23.000000 elphem-0.3.3/elphem/lattice/lattice.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1978 2024-05-29 13:49:23.000000 elphem-0.3.3/elphem/lattice/lattice_constant.py
+-rw-r--r--   0 runner    (1001) docker     (127)      431 2024-05-29 13:49:23.000000 elphem-0.3.3/elphem/lattice/path.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4307 2024-05-29 13:49:23.000000 elphem-0.3.3/elphem/lattice/primitive_cell.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12162 2024-05-29 13:49:23.000000 elphem-0.3.3/elphem/lattice/reciprocal_cell.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6898 2024-05-29 13:49:23.000000 elphem-0.3.3/elphem/lattice/rotation.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-29 13:49:27.963654 elphem-0.3.3/elphem/phonon/
+-rw-r--r--   0 runner    (1001) docker     (127)       21 2024-05-29 13:49:23.000000 elphem-0.3.3/elphem/phonon/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6254 2024-05-29 13:49:23.000000 elphem-0.3.3/elphem/phonon/phonon.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-29 13:49:27.963654 elphem-0.3.3/elphem.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     8099 2024-05-29 13:49:27.000000 elphem-0.3.3/elphem.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     1156 2024-05-29 13:49:27.000000 elphem-0.3.3/elphem.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-29 13:49:27.000000 elphem-0.3.3/elphem.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       12 2024-05-29 13:49:27.000000 elphem-0.3.3/elphem.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       13 2024-05-29 13:49:27.000000 elphem-0.3.3/elphem.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-29 13:49:27.963654 elphem-0.3.3/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)     1234 2024-05-29 13:49:23.000000 elphem-0.3.3/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-29 13:49:27.963654 elphem-0.3.3/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-29 13:49:23.000000 elphem-0.3.3/tests/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-29 13:49:27.963654 elphem-0.3.3/tests/common/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-29 13:49:23.000000 elphem-0.3.3/tests/common/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      409 2024-05-29 13:49:23.000000 elphem-0.3.3/tests/common/test_atomic_weight.py
+-rw-r--r--   0 runner    (1001) docker     (127)      876 2024-05-29 13:49:23.000000 elphem-0.3.3/tests/common/test_brillouin.py
+-rw-r--r--   0 runner    (1001) docker     (127)      514 2024-05-29 13:49:23.000000 elphem-0.3.3/tests/common/test_unit.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-29 13:49:27.963654 elphem-0.3.3/tests/electron/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-29 13:49:23.000000 elphem-0.3.3/tests/electron/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1406 2024-05-29 13:49:23.000000 elphem-0.3.3/tests/electron/test_electron.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-29 13:49:27.963654 elphem-0.3.3/tests/elph/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-29 13:49:23.000000 elphem-0.3.3/tests/elph/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2116 2024-05-29 13:49:23.000000 elphem-0.3.3/tests/elph/test_self_energy.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-29 13:49:27.963654 elphem-0.3.3/tests/lattice/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-29 13:49:23.000000 elphem-0.3.3/tests/lattice/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      755 2024-05-29 13:49:23.000000 elphem-0.3.3/tests/lattice/test_lattice.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-29 13:49:27.963654 elphem-0.3.3/tests/phonon/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-29 13:49:23.000000 elphem-0.3.3/tests/phonon/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1392 2024-05-29 13:49:23.000000 elphem-0.3.3/tests/phonon/test_phonon.py
```

### Comparing `elphem-0.3.2/LICENSE` & `elphem-0.3.3/LICENSE`

 * *Files identical despite different names*

### Comparing `elphem-0.3.2/PKG-INFO` & `elphem-0.3.3/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: elphem
-Version: 0.3.2
+Version: 0.3.3
 Summary: Elphem: Calculating electron-phonon interactions with the empty lattice.
 Home-page: https://github.com/cohsh/elphem
 Download-URL: https://github.com/cohsh/elphem
 Author: Kohei Ishii
 Author-email: 
 Maintainer: Kohei Ishii
 Maintainer-email: 
@@ -68,19 +68,19 @@
 
 def main():
     # Parameters of lattice
     a = 2.98 * Length.ANGSTROM['->']
 
     # Parameters of electron
     n_electrons = 1
-    n_bands_electron = 4
+    n_bands_electron = 10
 
     # Parameters of phonon
     debye_temperature = 344.0
-    n_q = [6, 6, 6]
+    n_q = [8, 8, 8]
     
     # Parameters of k-path
     k_names = ["G", "H", "N", "G", "P", "H"]
     n_split = 50
     
     # Parameters of electron-phonon
     temperature = 300.0
@@ -173,15 +173,15 @@
     # Generate an electron.
     electron = Electron.create_from_path(lattice, n_electrons, n_bands_electron, k_path)
 
     # Generate a phonon.
     phonon = Phonon.create_from_n(lattice, debye_temperature, n_q)
 
     # Generate electron-phonon
-    electron_phonon = ElectronPhonon(electron, phonon, temperature, n_bands_elph, eta=0.05)
+    electron_phonon = ElectronPhonon(electron, phonon, temperature, n_bands_elph, eta=0.03)
     
     # Calculate electron-phonon renormalization
     epr = electron_phonon.calculate_electron_phonon_renormalization()
     
     fig = plt.figure()
     ax = fig.add_subplot(111)
```

### Comparing `elphem-0.3.2/README.md` & `elphem-0.3.3/README.md`

 * *Files 1% similar despite different names*

```diff
@@ -47,19 +47,19 @@
 
 def main():
     # Parameters of lattice
     a = 2.98 * Length.ANGSTROM['->']
 
     # Parameters of electron
     n_electrons = 1
-    n_bands_electron = 4
+    n_bands_electron = 10
 
     # Parameters of phonon
     debye_temperature = 344.0
-    n_q = [6, 6, 6]
+    n_q = [8, 8, 8]
     
     # Parameters of k-path
     k_names = ["G", "H", "N", "G", "P", "H"]
     n_split = 50
     
     # Parameters of electron-phonon
     temperature = 300.0
@@ -152,15 +152,15 @@
     # Generate an electron.
     electron = Electron.create_from_path(lattice, n_electrons, n_bands_electron, k_path)
 
     # Generate a phonon.
     phonon = Phonon.create_from_n(lattice, debye_temperature, n_q)
 
     # Generate electron-phonon
-    electron_phonon = ElectronPhonon(electron, phonon, temperature, n_bands_elph, eta=0.05)
+    electron_phonon = ElectronPhonon(electron, phonon, temperature, n_bands_elph, eta=0.03)
     
     # Calculate electron-phonon renormalization
     epr = electron_phonon.calculate_electron_phonon_renormalization()
     
     fig = plt.figure()
     ax = fig.add_subplot(111)
```

### Comparing `elphem-0.3.2/elphem/common/atomic_weight.py` & `elphem-0.3.3/elphem/common/atomic_weight.py`

 * *Files identical despite different names*

### Comparing `elphem-0.3.2/elphem/common/brillouin.py` & `elphem-0.3.3/elphem/common/brillouin.py`

 * *Files identical despite different names*

### Comparing `elphem-0.3.2/elphem/common/distribution.py` & `elphem-0.3.3/elphem/common/distribution.py`

 * *Files identical despite different names*

### Comparing `elphem-0.3.2/elphem/common/function.py` & `elphem-0.3.3/elphem/common/function.py`

 * *Files identical despite different names*

### Comparing `elphem-0.3.2/elphem/common/stdout.py` & `elphem-0.3.3/elphem/common/stdout.py`

 * *Files identical despite different names*

### Comparing `elphem-0.3.2/elphem/common/unit.py` & `elphem-0.3.3/elphem/common/unit.py`

 * *Files identical despite different names*

### Comparing `elphem-0.3.2/elphem/electron/electron.py` & `elphem-0.3.3/elphem/electron/electron.py`

 * *Files identical despite different names*

### Comparing `elphem-0.3.2/elphem/elph/electron_phonon.py` & `elphem-0.3.3/elphem/elph/electron_phonon.py`

 * *Files 4% similar despite different names*

```diff
@@ -80,38 +80,38 @@
         """Calculate the Bloch (1929) electron-phonon coupling constants.
 
         Returns:
             np.ndarray: The lowest-order electron-phonon coupling constants
         """
         potential = 1.0 / 16.0
         
-        return -1.0j * potential * np.nansum((self.phonon.q + self.electron.g - self.electron_inter.g) * self.phonon.eigenvectors, axis=-1) * self.phonon.zero_point_lengths
+        return -1.0j * potential * np.nansum((self.phonon.q + self.electron_inter.g - self.electron.g) * self.phonon.eigenvectors, axis=-1) * self.phonon.zero_point_lengths
 
     def calculate_couplings_nordheim(self) -> np.ndarray:
         """Calculate the Nordheim (1931) electron-phonon coupling constants.
 
         Returns:
             np.ndarray: The lowest-order electron-phonon coupling constants
         """
-        potential = 4.0 / self.electron.lattice.primitive.volume * self.electron.n_electrons * np.pi / ( np.nansum(self.phonon.q + self.electron.g - self.electron_inter.g, axis=-1) ** 2)
+        potential = 4.0 / self.electron.lattice.primitive.volume * self.electron.n_electrons * np.pi / ( np.nansum(self.phonon.q + self.electron_inter.g - self.electron.g, axis=-1) ** 2)
         
-        return -1.0j * potential * np.nansum((self.phonon.q + self.electron.g - self.electron_inter.g) * self.phonon.eigenvectors, axis=-1) * self.phonon.zero_point_lengths
+        return -1.0j * potential * np.nansum((self.phonon.q + self.electron_inter.g - self.electron.g) * self.phonon.eigenvectors, axis=-1) * self.phonon.zero_point_lengths
 
     def calculate_couplings_bardeen(self) -> np.ndarray:
         """Calculate the Bardeen (1937) electron-phonon coupling constants.
 
         Returns:
             np.ndarray: The lowest-order electron-phonon coupling constants
         """
-        wave_number = np.nansum(self.phonon.q + self.electron.g - self.electron_inter.g, axis=-1)
+        wave_number = np.nansum(self.phonon.q + self.electron_inter.g - self.electron.g, axis=-1)
 
         numerator = 4.0 * self.electron.n_electrons * np.pi
         denominator = wave_number ** 2 + self.electron.thomas_fermi_wave_number ** 2 * self.calculate_lindhard_function(wave_number / (2.0 * self.electron.fermi_wave_number))
         
-        return -1.0j / self.electron.lattice.primitive.volume * numerator / denominator * np.nansum((self.phonon.q + self.electron.g - self.electron_inter.g) * self.phonon.eigenvectors, axis=-1) * self.phonon.zero_point_lengths
+        return -1.0j / self.electron.lattice.primitive.volume * numerator / denominator * np.nansum((self.phonon.q + self.electron_inter.g - self.electron.g) * self.phonon.eigenvectors, axis=-1) * self.phonon.zero_point_lengths
     
     @staticmethod
     def calculate_lindhard_function(x: np.ndarray) -> np.ndarray:
         return 0.5 + (1.0 - x ** 2) / (4.0 * x) * np.log(np.abs(1.0 + x) / np.abs(1.0 - x))
 
     def calculate_self_energies(self, omega: float) -> np.ndarray:
         """Calculate Fan self-energies.
```

### Comparing `elphem-0.3.2/elphem/elph/green_function.py` & `elphem-0.3.3/elphem/elph/green_function.py`

 * *Files identical despite different names*

### Comparing `elphem-0.3.2/elphem/lattice/cell.py` & `elphem-0.3.3/elphem/lattice/cell.py`

 * *Files identical despite different names*

### Comparing `elphem-0.3.2/elphem/lattice/lattice.py` & `elphem-0.3.3/elphem/lattice/lattice.py`

 * *Files identical despite different names*

### Comparing `elphem-0.3.2/elphem/lattice/lattice_constant.py` & `elphem-0.3.3/elphem/lattice/lattice_constant.py`

 * *Files identical despite different names*

### Comparing `elphem-0.3.2/elphem/lattice/primitive_cell.py` & `elphem-0.3.3/elphem/lattice/primitive_cell.py`

 * *Files identical despite different names*

### Comparing `elphem-0.3.2/elphem/lattice/reciprocal_cell.py` & `elphem-0.3.3/elphem/lattice/reciprocal_cell.py`

 * *Files identical despite different names*

### Comparing `elphem-0.3.2/elphem/lattice/rotation.py` & `elphem-0.3.3/elphem/lattice/rotation.py`

 * *Files identical despite different names*

### Comparing `elphem-0.3.2/elphem/phonon/phonon.py` & `elphem-0.3.3/elphem/phonon/phonon.py`

 * *Files identical despite different names*

### Comparing `elphem-0.3.2/elphem.egg-info/PKG-INFO` & `elphem-0.3.3/elphem.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: elphem
-Version: 0.3.2
+Version: 0.3.3
 Summary: Elphem: Calculating electron-phonon interactions with the empty lattice.
 Home-page: https://github.com/cohsh/elphem
 Download-URL: https://github.com/cohsh/elphem
 Author: Kohei Ishii
 Author-email: 
 Maintainer: Kohei Ishii
 Maintainer-email: 
@@ -68,19 +68,19 @@
 
 def main():
     # Parameters of lattice
     a = 2.98 * Length.ANGSTROM['->']
 
     # Parameters of electron
     n_electrons = 1
-    n_bands_electron = 4
+    n_bands_electron = 10
 
     # Parameters of phonon
     debye_temperature = 344.0
-    n_q = [6, 6, 6]
+    n_q = [8, 8, 8]
     
     # Parameters of k-path
     k_names = ["G", "H", "N", "G", "P", "H"]
     n_split = 50
     
     # Parameters of electron-phonon
     temperature = 300.0
@@ -173,15 +173,15 @@
     # Generate an electron.
     electron = Electron.create_from_path(lattice, n_electrons, n_bands_electron, k_path)
 
     # Generate a phonon.
     phonon = Phonon.create_from_n(lattice, debye_temperature, n_q)
 
     # Generate electron-phonon
-    electron_phonon = ElectronPhonon(electron, phonon, temperature, n_bands_elph, eta=0.05)
+    electron_phonon = ElectronPhonon(electron, phonon, temperature, n_bands_elph, eta=0.03)
     
     # Calculate electron-phonon renormalization
     epr = electron_phonon.calculate_electron_phonon_renormalization()
     
     fig = plt.figure()
     ax = fig.add_subplot(111)
```

### Comparing `elphem-0.3.2/elphem.egg-info/SOURCES.txt` & `elphem-0.3.3/elphem.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `elphem-0.3.2/setup.py` & `elphem-0.3.3/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -3,15 +3,15 @@
 DESCRIPTION = 'Elphem: Calculating electron-phonon interactions with the empty lattice.'
 NAME = 'elphem'
 AUTHOR = 'Kohei Ishii'
 AUTHOR_EMAIL = ''
 URL = 'https://github.com/cohsh/elphem'
 LICENSE = 'MIT'
 DOWNLOAD_URL = URL
-VERSION = '0.3.2'
+VERSION = '0.3.3'
 PYTHON_REQUIRES = '>=3.10'
 INSTALL_REQUIRES = ['numpy', 'scipy']
 
 CLASSIFIERS=[
     'License :: OSI Approved :: MIT License',
     'Programming Language :: Python',
     'Programming Language :: Python :: 3.10',
```

### Comparing `elphem-0.3.2/tests/common/test_brillouin.py` & `elphem-0.3.3/tests/common/test_brillouin.py`

 * *Files identical despite different names*

### Comparing `elphem-0.3.2/tests/common/test_unit.py` & `elphem-0.3.3/tests/common/test_unit.py`

 * *Files identical despite different names*

### Comparing `elphem-0.3.2/tests/electron/test_electron.py` & `elphem-0.3.3/tests/electron/test_electron.py`

 * *Files identical despite different names*

### Comparing `elphem-0.3.2/tests/elph/test_self_energy.py` & `elphem-0.3.3/tests/elph/test_self_energy.py`

 * *Files identical despite different names*

### Comparing `elphem-0.3.2/tests/lattice/test_lattice.py` & `elphem-0.3.3/tests/lattice/test_lattice.py`

 * *Files identical despite different names*

### Comparing `elphem-0.3.2/tests/phonon/test_phonon.py` & `elphem-0.3.3/tests/phonon/test_phonon.py`

 * *Files identical despite different names*

