# Comparing `tmp/pdb_numpy-0.0.2.tar.gz` & `tmp/pdb_numpy-0.0.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pdb_numpy-0.0.2.tar", last modified: Mon Nov 20 11:45:25 2023, max compression
+gzip compressed data, was "pdb_numpy-0.0.3.tar", last modified: Wed May 29 08:28:17 2024, max compression
```

## Comparing `pdb_numpy-0.0.2.tar` & `pdb_numpy-0.0.3.tar`

### file list

```diff
@@ -1,39 +1,44 @@
-drwxrwxr-x   0 murail    (1000) murail    (1000)        0 2023-11-20 11:45:25.448087 pdb_numpy-0.0.2/
--rw-rw-r--   0 murail    (1000) murail    (1000)    18092 2023-11-03 13:13:10.000000 pdb_numpy-0.0.2/LICENSE
--rw-rw-r--   0 murail    (1000) murail    (1000)       32 2023-11-03 13:13:10.000000 pdb_numpy-0.0.2/MANIFEST.in
--rw-r--r--   0 murail    (1000) murail    (1000)     4220 2023-11-20 11:45:25.448087 pdb_numpy-0.0.2/PKG-INFO
--rw-rw-r--   0 murail    (1000) murail    (1000)     3021 2023-11-03 15:49:45.000000 pdb_numpy-0.0.2/README.rst
-drwxrwxr-x   0 murail    (1000) murail    (1000)        0 2023-11-20 11:45:25.444087 pdb_numpy-0.0.2/pdb_numpy.egg-info/
--rw-r--r--   0 murail    (1000) murail    (1000)     4220 2023-11-20 11:45:25.000000 pdb_numpy-0.0.2/pdb_numpy.egg-info/PKG-INFO
--rw-rw-r--   0 murail    (1000) murail    (1000)      815 2023-11-20 11:45:25.000000 pdb_numpy-0.0.2/pdb_numpy.egg-info/SOURCES.txt
--rw-rw-r--   0 murail    (1000) murail    (1000)        1 2023-11-20 11:45:25.000000 pdb_numpy-0.0.2/pdb_numpy.egg-info/dependency_links.txt
--rw-rw-r--   0 murail    (1000) murail    (1000)       54 2023-11-20 11:45:25.000000 pdb_numpy-0.0.2/pdb_numpy.egg-info/entry_points.txt
--rw-rw-r--   0 murail    (1000) murail    (1000)        1 2023-11-20 11:45:25.000000 pdb_numpy-0.0.2/pdb_numpy.egg-info/not-zip-safe
--rw-rw-r--   0 murail    (1000) murail    (1000)       22 2023-11-20 11:45:25.000000 pdb_numpy-0.0.2/pdb_numpy.egg-info/requires.txt
--rw-rw-r--   0 murail    (1000) murail    (1000)       10 2023-11-20 11:45:25.000000 pdb_numpy-0.0.2/pdb_numpy.egg-info/top_level.txt
--rw-rw-r--   0 murail    (1000) murail    (1000)      475 2023-11-20 11:45:25.448087 pdb_numpy-0.0.2/setup.cfg
--rw-rw-r--   0 murail    (1000) murail    (1000)     1882 2023-11-20 11:43:58.000000 pdb_numpy-0.0.2/setup.py
-drwxrwxr-x   0 murail    (1000) murail    (1000)        0 2023-11-20 11:45:25.444087 pdb_numpy-0.0.2/src/
-drwxrwxr-x   0 murail    (1000) murail    (1000)        0 2023-11-20 11:45:25.444087 pdb_numpy-0.0.2/src/pdb_numpy/
--rw-rw-r--   0 murail    (1000) murail    (1000)    14047 2023-11-03 13:13:10.000000 pdb_numpy-0.0.2/src/pdb_numpy/DSSP.py
--rw-rw-r--   0 murail    (1000) murail    (1000)      572 2023-11-20 11:43:58.000000 pdb_numpy-0.0.2/src/pdb_numpy/__init__.py
--rw-rw-r--   0 murail    (1000) murail    (1000)    21456 2023-11-03 13:13:10.000000 pdb_numpy-0.0.2/src/pdb_numpy/_align.so
--rw-rw-r--   0 murail    (1000) murail    (1000)    28653 2023-11-07 12:49:22.000000 pdb_numpy-0.0.2/src/pdb_numpy/abinitio.py
--rw-rw-r--   0 murail    (1000) murail    (1000)    20124 2023-11-03 13:13:10.000000 pdb_numpy-0.0.2/src/pdb_numpy/alignement.py
--rw-rw-r--   0 murail    (1000) murail    (1000)    24793 2023-11-20 10:34:56.000000 pdb_numpy-0.0.2/src/pdb_numpy/analysis.py
--rw-rw-r--   0 murail    (1000) murail    (1000)    32678 2023-11-03 13:13:10.000000 pdb_numpy-0.0.2/src/pdb_numpy/coor.py
-drwxrwxr-x   0 murail    (1000) murail    (1000)        0 2023-11-20 11:45:25.444087 pdb_numpy-0.0.2/src/pdb_numpy/data/
--rw-rw-r--   0 murail    (1000) murail    (1000)       40 2023-11-03 13:13:10.000000 pdb_numpy-0.0.2/src/pdb_numpy/data/__init__.py
--rw-rw-r--   0 murail    (1000) murail    (1000)     1036 2023-11-03 13:13:10.000000 pdb_numpy-0.0.2/src/pdb_numpy/data/aa_dict.py
--rw-rw-r--   0 murail    (1000) murail    (1000)      619 2023-11-03 13:13:10.000000 pdb_numpy-0.0.2/src/pdb_numpy/data/blosum.py
--rw-rw-r--   0 murail    (1000) murail    (1000)     2122 2023-11-03 13:13:10.000000 pdb_numpy-0.0.2/src/pdb_numpy/data/blosum62.txt
-drwxrwxr-x   0 murail    (1000) murail    (1000)        0 2023-11-20 11:45:25.448087 pdb_numpy-0.0.2/src/pdb_numpy/format/
--rw-rw-r--   0 murail    (1000) murail    (1000)       43 2023-11-03 13:13:10.000000 pdb_numpy-0.0.2/src/pdb_numpy/format/__init__.py
--rw-rw-r--   0 murail    (1000) murail    (1000)     5883 2023-11-03 13:13:10.000000 pdb_numpy-0.0.2/src/pdb_numpy/format/gro.py
--rw-rw-r--   0 murail    (1000) murail    (1000)    29903 2023-11-07 12:49:22.000000 pdb_numpy-0.0.2/src/pdb_numpy/format/mmcif.py
--rw-rw-r--   0 murail    (1000) murail    (1000)    12605 2023-11-07 12:49:22.000000 pdb_numpy-0.0.2/src/pdb_numpy/format/pdb.py
--rw-rw-r--   0 murail    (1000) murail    (1000)     3729 2023-11-03 13:13:10.000000 pdb_numpy-0.0.2/src/pdb_numpy/format/pqr.py
--rw-rw-r--   0 murail    (1000) murail    (1000)     9479 2023-11-03 13:13:10.000000 pdb_numpy-0.0.2/src/pdb_numpy/geom.py
--rw-rw-r--   0 murail    (1000) murail    (1000)    16619 2023-11-07 12:49:22.000000 pdb_numpy-0.0.2/src/pdb_numpy/model.py
--rw-rw-r--   0 murail    (1000) murail    (1000)     6295 2023-11-03 13:13:10.000000 pdb_numpy-0.0.2/src/pdb_numpy/select.py
--rw-rw-r--   0 murail    (1000) murail    (1000)     6295 2023-11-03 13:13:10.000000 pdb_numpy-0.0.2/src/pdb_numpy/visu.py
+drwxrwxr-x   0 murail    (1000) murail    (1000)        0 2024-05-29 08:28:17.016479 pdb_numpy-0.0.3/
+-rw-rw-r--   0 murail    (1000) murail    (1000)    18092 2023-11-03 13:13:10.000000 pdb_numpy-0.0.3/LICENSE
+-rw-rw-r--   0 murail    (1000) murail    (1000)       32 2023-11-03 13:13:10.000000 pdb_numpy-0.0.3/MANIFEST.in
+-rw-r--r--   0 murail    (1000) murail    (1000)     4501 2024-05-29 08:28:17.016479 pdb_numpy-0.0.3/PKG-INFO
+-rw-rw-r--   0 murail    (1000) murail    (1000)     3301 2024-04-25 07:49:50.000000 pdb_numpy-0.0.3/README.rst
+drwxrwxr-x   0 murail    (1000) murail    (1000)        0 2024-05-29 08:28:17.012479 pdb_numpy-0.0.3/pdb_numpy.egg-info/
+-rw-r--r--   0 murail    (1000) murail    (1000)     4501 2024-05-29 08:28:16.000000 pdb_numpy-0.0.3/pdb_numpy.egg-info/PKG-INFO
+-rw-rw-r--   0 murail    (1000) murail    (1000)      993 2024-05-29 08:28:16.000000 pdb_numpy-0.0.3/pdb_numpy.egg-info/SOURCES.txt
+-rw-rw-r--   0 murail    (1000) murail    (1000)        1 2024-05-29 08:28:16.000000 pdb_numpy-0.0.3/pdb_numpy.egg-info/dependency_links.txt
+-rw-rw-r--   0 murail    (1000) murail    (1000)       54 2024-05-29 08:28:16.000000 pdb_numpy-0.0.3/pdb_numpy.egg-info/entry_points.txt
+-rw-rw-r--   0 murail    (1000) murail    (1000)        1 2024-05-29 08:28:16.000000 pdb_numpy-0.0.3/pdb_numpy.egg-info/not-zip-safe
+-rw-rw-r--   0 murail    (1000) murail    (1000)       23 2024-05-29 08:28:16.000000 pdb_numpy-0.0.3/pdb_numpy.egg-info/requires.txt
+-rw-rw-r--   0 murail    (1000) murail    (1000)       10 2024-05-29 08:28:16.000000 pdb_numpy-0.0.3/pdb_numpy.egg-info/top_level.txt
+-rw-rw-r--   0 murail    (1000) murail    (1000)      478 2024-05-29 08:28:17.016479 pdb_numpy-0.0.3/setup.cfg
+-rw-rw-r--   0 murail    (1000) murail    (1000)     2583 2024-05-29 08:08:34.000000 pdb_numpy-0.0.3/setup.py
+drwxrwxr-x   0 murail    (1000) murail    (1000)        0 2024-05-29 08:28:17.012479 pdb_numpy-0.0.3/src/
+drwxrwxr-x   0 murail    (1000) murail    (1000)        0 2024-05-29 08:28:17.016479 pdb_numpy-0.0.3/src/pdb_numpy/
+-rw-rw-r--   0 murail    (1000) murail    (1000)    14010 2024-03-29 09:26:59.000000 pdb_numpy-0.0.3/src/pdb_numpy/DSSP.py
+-rw-rw-r--   0 murail    (1000) murail    (1000)      792 2024-05-29 08:08:34.000000 pdb_numpy-0.0.3/src/pdb_numpy/__init__.py
+-rw-rw-r--   0 murail    (1000) murail    (1000)    22870 2024-03-22 14:17:41.000000 pdb_numpy-0.0.3/src/pdb_numpy/abinitio.py
+drwxrwxr-x   0 murail    (1000) murail    (1000)        0 2024-05-29 08:28:17.016479 pdb_numpy-0.0.3/src/pdb_numpy/alignement/
+-rw-rw-r--   0 murail    (1000) murail    (1000)    21728 2024-05-29 08:00:38.000000 pdb_numpy-0.0.3/src/pdb_numpy/alignement/__init__.py
+-rw-rw-r--   0 murail    (1000) murail    (1000)     8766 2024-03-29 09:45:03.000000 pdb_numpy-0.0.3/src/pdb_numpy/alignement/align_cython.pyx
+-rw-rw-r--   0 murail    (1000) murail    (1000)      741 2024-03-22 14:17:40.000000 pdb_numpy-0.0.3/src/pdb_numpy/alignement/profile_cython.py
+-rw-rw-r--   0 murail    (1000) murail    (1000)    30170 2024-05-16 07:45:32.000000 pdb_numpy-0.0.3/src/pdb_numpy/analysis.py
+-rw-rw-r--   0 murail    (1000) murail    (1000)    33499 2024-04-20 14:54:34.000000 pdb_numpy-0.0.3/src/pdb_numpy/coor.py
+drwxrwxr-x   0 murail    (1000) murail    (1000)        0 2024-05-29 08:28:17.016479 pdb_numpy-0.0.3/src/pdb_numpy/data/
+-rw-rw-r--   0 murail    (1000) murail    (1000)       40 2023-11-03 13:13:10.000000 pdb_numpy-0.0.3/src/pdb_numpy/data/__init__.py
+-rw-rw-r--   0 murail    (1000) murail    (1000)     1068 2024-03-22 14:17:40.000000 pdb_numpy-0.0.3/src/pdb_numpy/data/aa_dict.py
+-rw-rw-r--   0 murail    (1000) murail    (1000)      619 2023-11-03 13:13:10.000000 pdb_numpy-0.0.3/src/pdb_numpy/data/blosum.py
+-rw-rw-r--   0 murail    (1000) murail    (1000)     2122 2023-11-03 13:13:10.000000 pdb_numpy-0.0.3/src/pdb_numpy/data/blosum62.txt
+drwxrwxr-x   0 murail    (1000) murail    (1000)        0 2024-05-29 08:28:17.016479 pdb_numpy-0.0.3/src/pdb_numpy/format/
+-rw-rw-r--   0 murail    (1000) murail    (1000)       43 2024-03-28 09:37:34.000000 pdb_numpy-0.0.3/src/pdb_numpy/format/__init__.py
+-rw-rw-r--   0 murail    (1000) murail    (1000)     5912 2024-03-22 14:17:40.000000 pdb_numpy-0.0.3/src/pdb_numpy/format/encode.py
+-rw-rw-r--   0 murail    (1000) murail    (1000)     7343 2024-03-28 22:02:39.000000 pdb_numpy-0.0.3/src/pdb_numpy/format/encode_cython.pyx
+-rw-rw-r--   0 murail    (1000) murail    (1000)     5891 2024-03-29 11:06:23.000000 pdb_numpy-0.0.3/src/pdb_numpy/format/gro.py
+-rw-rw-r--   0 murail    (1000) murail    (1000)    31473 2024-04-19 17:02:05.000000 pdb_numpy-0.0.3/src/pdb_numpy/format/mmcif.py
+-rw-rw-r--   0 murail    (1000) murail    (1000)    14336 2024-03-29 12:36:43.000000 pdb_numpy-0.0.3/src/pdb_numpy/format/pdb.py
+-rw-rw-r--   0 murail    (1000) murail    (1000)     3732 2024-01-25 09:35:36.000000 pdb_numpy-0.0.3/src/pdb_numpy/format/pqr.py
+-rw-rw-r--   0 murail    (1000) murail    (1000)     1256 2024-03-29 08:57:14.000000 pdb_numpy-0.0.3/src/pdb_numpy/format/split_cython.pyx
+-rw-rw-r--   0 murail    (1000) murail    (1000)    12556 2024-03-29 09:52:46.000000 pdb_numpy-0.0.3/src/pdb_numpy/geom.py
+-rw-rw-r--   0 murail    (1000) murail    (1000)    16439 2024-04-23 11:49:48.000000 pdb_numpy-0.0.3/src/pdb_numpy/model.py
+-rw-rw-r--   0 murail    (1000) murail    (1000)     6288 2024-04-23 10:12:17.000000 pdb_numpy-0.0.3/src/pdb_numpy/select.py
+-rw-rw-r--   0 murail    (1000) murail    (1000)     7548 2024-03-22 14:17:40.000000 pdb_numpy-0.0.3/src/pdb_numpy/visu.py
```

### Comparing `pdb_numpy-0.0.2/LICENSE` & `pdb_numpy-0.0.3/LICENSE`

 * *Files identical despite different names*

### Comparing `pdb_numpy-0.0.2/PKG-INFO` & `pdb_numpy-0.0.3/PKG-INFO`

 * *Files 11% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pdb_numpy
-Version: 0.0.2
+Version: 0.0.3
 Summary: Pdb_Numpy is a python library allowing simple operations on pdb coor files.
 Home-page: https://github.com/samuelmurail/pdb_numpy
 Author: Samuel Murail
 Author-email: samuel.murail@u-paris.fr
 License: GNUv2.0
 Keywords: pdb_numpy,Python,PDB,Numpy,Coor,Model
 Classifier: Development Status :: 4 - Beta
@@ -22,32 +22,38 @@
 Classifier: Programming Language :: Python :: Implementation :: PyPy
 Classifier: Programming Language :: Python
 Classifier: Topic :: Software Development
 Requires-Python: >=3.7
 Description-Content-Type: text/markdown
 License-File: LICENSE
 Requires-Dist: numpy>=1.2
-Requires-Dist: scipy>=1.5
+Requires-Dist: cython>=3.0
 
 
 .. image:: https://readthedocs.org/projects/pdb-numpy/badge/?version=latest
     :target: https://pdb-numpy.readthedocs.io/en/latest/?badge=latest
     :alt: Documentation Status
 
-.. image:: https://dev.azure.com/samuelmurailRPBS/pdb_numpy/_apis/build/status/samuelmurail.pdb_numpy?branchName=main
+.. image:: https://dev.azure.com/samuelmurailRPBS/pdb_numpy/_apis/build/status%2Fsamuelmurail.pdb_numpy?branchName=main
     :target: https://dev.azure.com/samuelmurailRPBS/pdb_numpy/_build/latest?definitionId=1&branchName=main
     :alt: Build Status
 
 .. image:: https://codecov.io/gh/samuelmurail/pdb_numpy/branch/main/graph/badge.svg?token=MCVDZ7GD0V
     :target: https://codecov.io/gh/samuelmurail/pdb_numpy
     :alt: Code coverage
 
 About PDB-numpy
 ===============
 
+.. image:: https://raw.githubusercontent.com/samuelmurail/pdb_numpy/master/docs/source/logo.jpeg
+  :width: 200
+  :align: center
+  :alt: PDB Numpy Logo
+
+
 ``pdb_numpy`` is a python library designed to facilitate working with PDB files
 in the context of structural bioinformatics. The library builds upon the
 powerful ``numpy`` library to provide efficient and easy-to-use tools for
 reading, manipulating, and analyzing PDB files.
 
 The library includes a number of functions for working with PDB files,
 including functions for parsing PDB files and extracting relevant information,
@@ -93,25 +99,31 @@
 
 Dependencies
 ------------
 
 ``pdb_numpy`` requires the following dependencies:
 
 - ``numpy``
-- ``scipy``
+- ``cython``
 
 
 Contributing
 ------------
 
 ``pdb_numpy`` is an open-source project and contributions are welcome. If
 you find a bug or have a feature request, please open an issue on the GitHub
 repository at https://github.com/samuelmurail/pdb_numpy. If you would like
 to contribute code, please fork the repository and submit a pull request.
 
+To build locally the extension module, you can run the following command:
+
+```bash
+python setup.py build_ext --inplace
+```
+
 Author
 --------------
 
 * `Samuel Murail <https://samuelmurail.github.io/PersonalPage/>`_, Associate Professor - `Université Paris Cité <https://u-paris.fr>`_, `CMPLI <http://bfa.univ-paris-diderot.fr/equipe-8/>`_.
 
 See also the list of `contributors <https://github.com/samuelmurail/pdb_numpy/contributors>`_ who participated in this project.
```

### Comparing `pdb_numpy-0.0.2/README.rst` & `pdb_numpy-0.0.3/README.rst`

 * *Files 10% similar despite different names*

```diff
@@ -1,23 +1,29 @@
 
 .. image:: https://readthedocs.org/projects/pdb-numpy/badge/?version=latest
     :target: https://pdb-numpy.readthedocs.io/en/latest/?badge=latest
     :alt: Documentation Status
 
-.. image:: https://dev.azure.com/samuelmurailRPBS/pdb_numpy/_apis/build/status/samuelmurail.pdb_numpy?branchName=main
+.. image:: https://dev.azure.com/samuelmurailRPBS/pdb_numpy/_apis/build/status%2Fsamuelmurail.pdb_numpy?branchName=main
     :target: https://dev.azure.com/samuelmurailRPBS/pdb_numpy/_build/latest?definitionId=1&branchName=main
     :alt: Build Status
 
 .. image:: https://codecov.io/gh/samuelmurail/pdb_numpy/branch/main/graph/badge.svg?token=MCVDZ7GD0V
     :target: https://codecov.io/gh/samuelmurail/pdb_numpy
     :alt: Code coverage
 
 About PDB-numpy
 ===============
 
+.. image:: https://raw.githubusercontent.com/samuelmurail/pdb_numpy/master/docs/source/logo.jpeg
+  :width: 200
+  :align: center
+  :alt: PDB Numpy Logo
+
+
 ``pdb_numpy`` is a python library designed to facilitate working with PDB files
 in the context of structural bioinformatics. The library builds upon the
 powerful ``numpy`` library to provide efficient and easy-to-use tools for
 reading, manipulating, and analyzing PDB files.
 
 The library includes a number of functions for working with PDB files,
 including functions for parsing PDB files and extracting relevant information,
@@ -63,25 +69,31 @@
 
 Dependencies
 ------------
 
 ``pdb_numpy`` requires the following dependencies:
 
 - ``numpy``
-- ``scipy``
+- ``cython``
 
 
 Contributing
 ------------
 
 ``pdb_numpy`` is an open-source project and contributions are welcome. If
 you find a bug or have a feature request, please open an issue on the GitHub
 repository at https://github.com/samuelmurail/pdb_numpy. If you would like
 to contribute code, please fork the repository and submit a pull request.
 
+To build locally the extension module, you can run the following command:
+
+```bash
+python setup.py build_ext --inplace
+```
+
 Author
 --------------
 
 * `Samuel Murail <https://samuelmurail.github.io/PersonalPage/>`_, Associate Professor - `Université Paris Cité <https://u-paris.fr>`_, `CMPLI <http://bfa.univ-paris-diderot.fr/equipe-8/>`_.
 
 See also the list of `contributors <https://github.com/samuelmurail/pdb_numpy/contributors>`_ who participated in this project.
```

### Comparing `pdb_numpy-0.0.2/pdb_numpy.egg-info/PKG-INFO` & `pdb_numpy-0.0.3/pdb_numpy.egg-info/PKG-INFO`

 * *Files 11% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pdb-numpy
-Version: 0.0.2
+Version: 0.0.3
 Summary: Pdb_Numpy is a python library allowing simple operations on pdb coor files.
 Home-page: https://github.com/samuelmurail/pdb_numpy
 Author: Samuel Murail
 Author-email: samuel.murail@u-paris.fr
 License: GNUv2.0
 Keywords: pdb_numpy,Python,PDB,Numpy,Coor,Model
 Classifier: Development Status :: 4 - Beta
@@ -22,32 +22,38 @@
 Classifier: Programming Language :: Python :: Implementation :: PyPy
 Classifier: Programming Language :: Python
 Classifier: Topic :: Software Development
 Requires-Python: >=3.7
 Description-Content-Type: text/markdown
 License-File: LICENSE
 Requires-Dist: numpy>=1.2
-Requires-Dist: scipy>=1.5
+Requires-Dist: cython>=3.0
 
 
 .. image:: https://readthedocs.org/projects/pdb-numpy/badge/?version=latest
     :target: https://pdb-numpy.readthedocs.io/en/latest/?badge=latest
     :alt: Documentation Status
 
-.. image:: https://dev.azure.com/samuelmurailRPBS/pdb_numpy/_apis/build/status/samuelmurail.pdb_numpy?branchName=main
+.. image:: https://dev.azure.com/samuelmurailRPBS/pdb_numpy/_apis/build/status%2Fsamuelmurail.pdb_numpy?branchName=main
     :target: https://dev.azure.com/samuelmurailRPBS/pdb_numpy/_build/latest?definitionId=1&branchName=main
     :alt: Build Status
 
 .. image:: https://codecov.io/gh/samuelmurail/pdb_numpy/branch/main/graph/badge.svg?token=MCVDZ7GD0V
     :target: https://codecov.io/gh/samuelmurail/pdb_numpy
     :alt: Code coverage
 
 About PDB-numpy
 ===============
 
+.. image:: https://raw.githubusercontent.com/samuelmurail/pdb_numpy/master/docs/source/logo.jpeg
+  :width: 200
+  :align: center
+  :alt: PDB Numpy Logo
+
+
 ``pdb_numpy`` is a python library designed to facilitate working with PDB files
 in the context of structural bioinformatics. The library builds upon the
 powerful ``numpy`` library to provide efficient and easy-to-use tools for
 reading, manipulating, and analyzing PDB files.
 
 The library includes a number of functions for working with PDB files,
 including functions for parsing PDB files and extracting relevant information,
@@ -93,25 +99,31 @@
 
 Dependencies
 ------------
 
 ``pdb_numpy`` requires the following dependencies:
 
 - ``numpy``
-- ``scipy``
+- ``cython``
 
 
 Contributing
 ------------
 
 ``pdb_numpy`` is an open-source project and contributions are welcome. If
 you find a bug or have a feature request, please open an issue on the GitHub
 repository at https://github.com/samuelmurail/pdb_numpy. If you would like
 to contribute code, please fork the repository and submit a pull request.
 
+To build locally the extension module, you can run the following command:
+
+```bash
+python setup.py build_ext --inplace
+```
+
 Author
 --------------
 
 * `Samuel Murail <https://samuelmurail.github.io/PersonalPage/>`_, Associate Professor - `Université Paris Cité <https://u-paris.fr>`_, `CMPLI <http://bfa.univ-paris-diderot.fr/equipe-8/>`_.
 
 See also the list of `contributors <https://github.com/samuelmurail/pdb_numpy/contributors>`_ who participated in this project.
```

### Comparing `pdb_numpy-0.0.2/pdb_numpy.egg-info/SOURCES.txt` & `pdb_numpy-0.0.3/pdb_numpy.egg-info/SOURCES.txt`

 * *Files 16% similar despite different names*

```diff
@@ -8,25 +8,29 @@
 pdb_numpy.egg-info/dependency_links.txt
 pdb_numpy.egg-info/entry_points.txt
 pdb_numpy.egg-info/not-zip-safe
 pdb_numpy.egg-info/requires.txt
 pdb_numpy.egg-info/top_level.txt
 src/pdb_numpy/DSSP.py
 src/pdb_numpy/__init__.py
-src/pdb_numpy/_align.so
 src/pdb_numpy/abinitio.py
-src/pdb_numpy/alignement.py
 src/pdb_numpy/analysis.py
 src/pdb_numpy/coor.py
 src/pdb_numpy/geom.py
 src/pdb_numpy/model.py
 src/pdb_numpy/select.py
 src/pdb_numpy/visu.py
+src/pdb_numpy/alignement/__init__.py
+src/pdb_numpy/alignement/align_cython.pyx
+src/pdb_numpy/alignement/profile_cython.py
 src/pdb_numpy/data/__init__.py
 src/pdb_numpy/data/aa_dict.py
 src/pdb_numpy/data/blosum.py
 src/pdb_numpy/data/blosum62.txt
 src/pdb_numpy/format/__init__.py
+src/pdb_numpy/format/encode.py
+src/pdb_numpy/format/encode_cython.pyx
 src/pdb_numpy/format/gro.py
 src/pdb_numpy/format/mmcif.py
 src/pdb_numpy/format/pdb.py
-src/pdb_numpy/format/pqr.py
+src/pdb_numpy/format/pqr.py
+src/pdb_numpy/format/split_cython.pyx
```

### Comparing `pdb_numpy-0.0.2/setup.py` & `pdb_numpy-0.0.3/setup.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,42 +1,65 @@
-from setuptools import setup, find_packages
+import numpy as np
 
-version="0.0.2"
+from setuptools import setup
+from distutils.extension import Extension
+
+version="0.0.3"
 
 with open('README.rst', encoding='utf-8') as readme_file:
     readme = readme_file.read()
 
+ext_modules = [
+    Extension(
+        name="pdb_numpy.alignement.align_cython",
+        sources=["src/pdb_numpy/alignement/align_cython.pyx"],
+        include_dirs=[np.get_include()]),
+    Extension(
+        name="pdb_numpy.format.split_cython",
+        sources=["src/pdb_numpy/format/split_cython.pyx"]),
+    Extension(
+        name="pdb_numpy.format.encode_cython",
+        sources=["src/pdb_numpy/format/encode_cython.pyx"]),
+]
+
 requirements = [
     'numpy>=1.2',
-    'scipy>=1.5',
+    'cython>=3.0',
 ]
 
 setup(
     name='pdb_numpy',
     version=version,
     description=(
         'Pdb_Numpy is a python library allowing simple operations on pdb coor files.'
     ),
     long_description=readme,
     long_description_content_type='text/markdown',
     author='Samuel Murail',
     author_email="samuel.murail@u-paris.fr",
     url='https://github.com/samuelmurail/pdb_numpy',
-    packages=['pdb_numpy', 'pdb_numpy.data', 'pdb_numpy.format'],
+    packages=['pdb_numpy', 'pdb_numpy.data', 'pdb_numpy.format', 'pdb_numpy.alignement'],
     package_dir={'pdb_numpy': 'src/pdb_numpy'},
     entry_points={'console_scripts': ['pdb_numpy = pdb_numpy.__main__:main']},
     include_package_data=True,
     python_requires='>=3.7',
     install_requires=requirements,
+    setup_requires=['pytest-runner'],
+    tests_require=['pytest'],
     license='GNUv2.0',
     zip_safe=False,
+    ext_modules = ext_modules,
     package_data={
         'pdb_numpy.data': [
             'blosum62.txt',
         ],
+        'pdb_numpy.alignement': [
+            '_align.so',
+            '_align.dylib'
+        ],
     },
     classifiers=[
         "Development Status :: 4 - Beta",
         "Environment :: Console",
         "Intended Audience :: Developers",
         "Natural Language :: English",
         "License :: OSI Approved :: BSD License",
```

### Comparing `pdb_numpy-0.0.2/src/pdb_numpy/DSSP.py` & `pdb_numpy-0.0.3/src/pdb_numpy/DSSP.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,13 +1,12 @@
 #!/usr/bin/env python3
 # coding: utf-8
 
 import numpy as np
 from . import geom
-from scipy.spatial import distance_matrix
 import logging
 
 # Logging
 logger = logging.getLogger(__name__)
 
 
 def add_NH(coor):
@@ -255,15 +254,15 @@
 
     """
     cutoff = 8.0
 
     CA_array = model.select_atoms("protein and name CA and not altloc B C D E").xyz
     n_res = len(CA_array)
 
-    dist_mat = distance_matrix(CA_array, CA_array)
+    dist_mat = geom.distance_matrix(CA_array, CA_array)
     Hbond_mat = np.zeros_like(dist_mat, dtype=bool)
 
     O_array = model.select_atoms("protein and name O and not altloc B C D E").xyz
     N_array = model.select_atoms("protein and name N and not altloc B C D E").xyz
     C_array = model.select_atoms("protein and name C and not altloc B C D E").xyz
     H_array = get_NH_xyz(model)
```

### Comparing `pdb_numpy-0.0.2/src/pdb_numpy/alignement.py` & `pdb_numpy-0.0.3/src/pdb_numpy/alignement/__init__.py`

 * *Files 3% similar despite different names*

```diff
@@ -2,69 +2,117 @@
 # coding: utf-8
 
 import os
 import numpy as np
 from itertools import permutations
 import logging
 
-from . import analysis
-from . import geom
-from .data.blosum import BLOSUM62
+from . import align_cython
 
-# Logging
-logger = logging.getLogger(__name__)
-
-
-def align_seq_C(seq_1, seq_2, gap_cost=-11, gap_extension=-1):
-    import ctypes
-
-    dir_path = os.path.dirname(os.path.abspath(__file__))
-    so_file = os.path.join(dir_path, "_align.so")
-
-    my_functions = ctypes.CDLL(so_file)
+from .. import analysis
+from .. import geom
+from ..data.blosum import BLOSUM62
 
-    class test(ctypes.Structure):
-        _fields_ = [
-            ("seq1", ctypes.c_char_p),
-            ("seq2", ctypes.c_char_p),
-            ("score", ctypes.c_int),
-        ]
 
-    align = my_functions.align
-    align.restype = ctypes.POINTER(test)
-    align.argtypes = [
-        ctypes.c_char_p,
-        ctypes.c_char_p,
-        ctypes.c_char_p,
-        ctypes.c_int,
-        ctypes.c_int,
-    ]
+# Logging
+logger = logging.getLogger(__name__)
 
-    seq_1_bytes = seq_1.encode("ascii")
-    seq_2_bytes = seq_2.encode("ascii")
-    blosum_file = os.path.join(dir_path, "data/blosum62.txt")
-
-    alignement_res = align(
-        ctypes.c_char_p(seq_1_bytes),
-        ctypes.c_char_p(seq_2_bytes),
-        ctypes.c_char_p(blosum_file.encode("ascii")),
-        ctypes.c_int(gap_cost),
-        ctypes.c_int(gap_extension),
-    )
 
-    seq_1_aligned = alignement_res.contents.seq1
-    seq_2_aligned = alignement_res.contents.seq2
+#def align_seq_C(seq_1, seq_2, gap_cost=-11, gap_extension=-1):
+#    """Align two amino acid sequences using the Waterman - Smith Algorithm.
+#
+#    Parameters
+#    ----------
+#    seq_1 : str
+#        First sequence to align
+#    seq_2 : str
+#        Second sequence to align
+#    gap_cost : int, optional
+#        Cost of gap, by default -8
+#    gap_extension : int, optional
+#        Cost of gap extension, by default -2
+#
+#    Returns
+#    -------
+#    str
+#        Aligned sequence 1
+#    str
+#        Aligned sequence 2
+#
+#    .note:: This function is based on the C implementation of the Waterman - Smith Algorithm.
+#
+#        To compile the C code, run the following command in the src/pdb_numpy/alignement folder:
+#
+#        in Linux:
+#        ```
+#        gcc -shared -o _align.so -fPIC _align.c
+#        ```
+#
+#        in OSX:
+#        ```
+#        gcc -shared -o _align.dylib -fPIC _align.c
+#        ```
+#
+#    """
+#    import platform
+#    import ctypes
+#
+#    dir_path = os.path.dirname(os.path.abspath(__file__))
+#    if platform.uname()[0] == "Darwin":
+#        so_file = os.path.join(dir_path, "_align.dylib")
+#    else:
+#        so_file = os.path.join(dir_path, "_align.so")
+#
+#    my_functions = ctypes.CDLL(so_file)
+#
+#    class test(ctypes.Structure):
+#        _fields_ = [
+#            ("seq1", ctypes.c_char_p),
+#            ("seq2", ctypes.c_char_p),
+#            ("score", ctypes.c_int),
+#        ]
+#
+#    align = my_functions.align
+#    align.restype = ctypes.POINTER(test)
+#    align.argtypes = [
+#        ctypes.c_char_p,
+#        ctypes.c_char_p,
+#        ctypes.c_char_p,
+#        ctypes.c_int,
+#        ctypes.c_int,
+#    ]
+#
+#    seq_1_bytes = seq_1.encode("ascii")
+#    seq_2_bytes = seq_2.encode("ascii")
+#    blosum_file = os.path.join(dir_path, "../data/blosum62.txt")
+#
+#    alignement_res = align(
+#        ctypes.c_char_p(seq_1_bytes),
+#        ctypes.c_char_p(seq_2_bytes),
+#        ctypes.c_char_p(blosum_file.encode("ascii")),
+#        ctypes.c_int(gap_cost),
+#        ctypes.c_int(gap_extension),
+#    )
+#
+#    seq_1_aligned = alignement_res.contents.seq1
+#    seq_2_aligned = alignement_res.contents.seq2
+#
+#    # print(seq_1_aligned)
+#
+#    free_align = my_functions.free_align
+#    free_align.argtypes = [ctypes.POINTER(test)]
+#    free_align(alignement_res)
+#
+#    # print(f"Max score: {alignement_res.contents.score}")
+#    return seq_1_aligned.decode("ascii"), seq_2_aligned.decode("ascii")
 
-    # print(seq_1_aligned)
 
-    free_align = my_functions.free_align
-    free_align.argtypes = [ctypes.POINTER(test)]
-    free_align(alignement_res)
+def align_seq_cython(seq_1, seq_2, gap_cost=-11, gap_extension=-1):
 
-    return seq_1_aligned.decode("ascii"), seq_2_aligned.decode("ascii")
+    return align_cython.align_seq(seq_1, seq_2, gap_cost, gap_extension)
 
 
 def align_seq(seq_1, seq_2, gap_cost=-11, gap_extension=-1):
     """Align two amino acid sequences using the Waterman - Smith Algorithm.
 
     Parameters
     ----------
@@ -138,14 +186,15 @@
             index_list.append([max_index[0][i], max_index[1][i]])
 
     # if len(index_list) > 1:
     #    logger.warning(f"Ambigous alignement, {len(index_list)} solutions exists")
 
     i = index_list[0][0]
     j = index_list[0][1]
+    # print(i,j)
 
     # Traceback and compute the alignment
     align_1 = ""
     align_2 = ""
 
     if i != len_1:
         align_2 = (len_1 - i) * "-"
@@ -188,19 +237,20 @@
 
     if i != 0:
         align_2 = i * "-" + align_2
     elif j != 0:
         align_1 = j * "-" + align_1
 
     assert len(align_1) == len(align_2)
+    # print(f"Max score: {max_score}")
 
     return align_1, align_2
 
 
-def align_seq_WS(seq_1, seq_2, gap_cost=-8):
+def align_seq_WS(seq_1, seq_2, gap_cost=-8, gap_extension=-1):
     """Align two amino acid sequences using the Waterman - Smith Algorithm.
     without gap extensions.
 
     Parameters
     ----------
     seq_1 : str
         First sequence to align
@@ -340,43 +390,43 @@
         if seq_1[i] == seq_2[i]:
             sim_seq += "*"
             continue
         elif seq_1[i] != "-" and seq_2[i] != "-":
             if (seq_1[i], seq_2[i]) in BLOSUM62:
                 mut_score = BLOSUM62[seq_1[i], seq_2[i]]
             else:
-                print(seq_1[i], seq_2[i])
+                # print(seq_1[i], seq_2[i])
                 mut_score = BLOSUM62[seq_2[i], seq_1[i]]
             if mut_score >= 0:
                 sim_seq += "|"
                 continue
         sim_seq += " "
 
     for i in range(1 + len(seq_1) // line_len):
-        logger.info(seq_1[i * line_len : (i + 1) * line_len])
-        logger.info(sim_seq[i * line_len : (i + 1) * line_len])
-        logger.info(seq_2[i * line_len : (i + 1) * line_len])
-        logger.info("\n")
+        print(seq_1[i * line_len : (i + 1) * line_len])
+        print(sim_seq[i * line_len : (i + 1) * line_len])
+        print(seq_2[i * line_len : (i + 1) * line_len])
+        print("\n")
 
     identity = 0
     similarity = 0
     for char in sim_seq:
         if char == "*":
             identity += 1
         if char in ["|", "*"]:
             similarity += 1
 
     len_1 = len(seq_1.replace("-", ""))
     len_2 = len(seq_2.replace("-", ""))
 
-    logger.info(f"Identity seq1: {identity / len_1 * 100:.2f}%")
-    logger.info(f"Identity seq2: {identity / len_2 * 100:.2f}%")
+    print(f"Identity seq1: {identity / len_1 * 100:.2f}%")
+    print(f"Identity seq2: {identity / len_2 * 100:.2f}%")
 
-    logger.info(f"Similarity seq1: {similarity / len_1 * 100:.2f}%")
-    logger.info(f"Similarity seq2: {similarity / len_2 * 100:.2f}%")
+    print(f"Similarity seq1: {similarity / len_1 * 100:.2f}%")
+    print(f"Similarity seq2: {similarity / len_2 * 100:.2f}%")
 
     return
 
 
 def get_common_atoms(
     coor_1, coor_2, chain_1=["A"], chain_2=["A"], back_names=["C", "N", "O", "CA"]
 ):
@@ -431,15 +481,15 @@
     assert len(sel_index_1) == len(seq_1) * len(
         back_names
     ), "Incomplete backbone atoms for first Coor object, you might consider using the remove_incomplete_residues method before."
     assert len(sel_index_2) == len(seq_2) * len(
         back_names
     ), "Incomplete backbone atoms for second Coor object, you might consider using the remove_incomplete_residues method before."
 
-    align_seq_1, align_seq_2 = align_seq_C(seq_1, seq_2)
+    align_seq_1, align_seq_2 = align_seq_cython(seq_1, seq_2)
     # print_align_seq(align_seq_1, align_seq_2)
 
     align_sel_1 = []
     align_sel_2 = []
     index_sel_1 = 0
     index_sel_2 = 0
     back_num = len(back_names)
@@ -479,15 +529,14 @@
         Frame to use as reference for coor_2, by default 0
 
     Returns
     -------
     None
     """
 
-    from scipy.spatial.transform import Rotation as R
 
     assert len(index_1) != 0, "No atom selected in the first structure"
     assert len(index_1) == len(index_2), "Two structure don't have the same atom number"
     assert (
         0 <= frame_ref < len(coor_2.models)
     ), "Reference frame index is larger than the number of frame in the reference structure"
 
@@ -501,15 +550,17 @@
     ref_coor = coor_2.models[frame_ref].xyz[index_2]
 
     for i, model in enumerate(coor_1.models):
         centroid_1 = model.xyz[index_1].mean(axis=0)
         if not (self_align and (i == frame_ref)):
             model.xyz -= centroid_1
 
-        rot_mat = R.align_vectors(model.xyz[index_1], ref_coor)[0].as_matrix()
+        rot_mat = geom.quaternion_rotate(model.xyz[index_1], ref_coor)
+        # from scipy.spatial.transform import Rotation as R
+        # rot_mat = R.align_vectors(model.xyz[index_1], ref_coor)[0].as_matrix()
 
         model.xyz = np.dot(model.xyz, rot_mat)
         if not (self_align and (i == frame_ref)):
             model.xyz += centroid_2
 
     coor_2.models[frame_ref].xyz += centroid_2
 
@@ -655,14 +706,15 @@
         for chain_j in chain_2:
             logger.info(f"compute  common atoms for {chain_i} and {chain_j}")
             index_1, index_2 = get_common_atoms(
                 coor_1, coor_2, chain_i, chain_j, back_names=back_names
             )
             index_common[chain_i, chain_j] = [index_1, index_2]
 
+    # Compute RMSD for all chains permutation
     rmsd_perm = []
     index_perm = []
     for perm_1, perm_2 in zip(chain_1_perm, chain_2_perm):
         logger.info(
             f'Trying chains permutation: {" ".join(perm_1)} with {" ".join(perm_2)}'
         )
         index_all_1 = []
@@ -683,11 +735,15 @@
     min_rmsd = rmsd_perm[0][0]
     for i, rmsds in enumerate(rmsd_perm):
         for rmsd in rmsds:
             if rmsd < min_rmsd:
                 min_index = i
                 min_rmsd = rmsd
 
+    # Do the alignement with the best permutation
+    min_index_perm = index_perm[min_index]
+    coor_align(coor_1, coor_2, min_index_perm[0], min_index_perm[1])
+
     return (
         rmsd_perm[min_index],
         index_perm[min_index],
     )
```

### Comparing `pdb_numpy-0.0.2/src/pdb_numpy/analysis.py` & `pdb_numpy-0.0.3/src/pdb_numpy/analysis.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,19 +1,19 @@
 #!/usr/bin/env python3
 # coding: utf-8
 
 import numpy as np
 import logging
-from scipy.spatial import distance_matrix
 
 # Logging
 logger = logging.getLogger(__name__)
 
 from . import alignement
-from . import select as select
+from .select import remove_incomplete_backbone_residues
+from .geom import distance_matrix
 
 
 def rmsd(coor_1, coor_2, selection="name CA", index_list=None, frame_ref=0):
     r"""Compute RMSD between two sets of coordinates.
 
     The RMSD (Root Mean Square Deviation) measures the similarity between two sets of coordinates by calculating the
     average distance between the corresponding atoms. It is given by the formula:
@@ -63,31 +63,31 @@
         diff = model.xyz[index_1] - coor_2.models[frame_ref].xyz[index_2]
         rmsd_list.append(np.sqrt((diff * diff).sum() / len(index_1)))
 
     return rmsd_list
 
 
 def interface_rmsd(
-    coor_1, coor_2, rec_chain, lig_chain, cutoff=10.0, back_atom=["CA", "N", "C", "O"]
+    coor, coor_native, rec_chain_native, lig_chain_native, cutoff=10.0, back_atom=["CA", "N", "C", "O"]
 ):
     """Compute the interface RMSD between two models.
     The interface is defined as the distance between the ligand and the receptor
     below the cutoff distance. The RMSD is computed between the ligand and the
     receptor of the two models.
 
 
     Parameters
     ----------
-    coor_1 : Coor
+    coor : Coor
         First coordinates
-    coor_2 : Coor
+    coor_native : Coor
         Second coordinates
-    rec_chain : list
+    rec_chain_native : list
         List of receptor chain
-    lig_chain : list
+    lig_chain_native : list
         List of ligand chain
     cutoff : float, default=10.0
         Cutoff distance for the interface
     back_atom : list, default=['CA', 'N', 'C', 'O']
         List of backbone atoms to use for the RMSD calculation
 
     Returns
@@ -98,38 +98,51 @@
     Notes
     -----
     Both coor object must have equivalent residues number in both chains.
     Chain order must also be equivalent.
 
     """
 
-    lig_interface = coor_2.select_atoms(
-        f'chain {" ".join(lig_chain)} and within {cutoff} of chain {" ".join(rec_chain)}'
+
+    lig_interface = coor_native.select_atoms(
+        f'chain {" ".join(lig_chain_native)} and within {cutoff} of chain {" ".join(rec_chain_native)}'
     )
-    rec_interface = coor_2.select_atoms(
-        f'chain {" ".join(rec_chain)} and within {cutoff} of chain {" ".join(lig_chain)}'
+    rec_interface = coor_native.select_atoms(
+        f'chain {" ".join(rec_chain_native)} and within {cutoff} of chain {" ".join(lig_chain_native)}'
     )
 
-    interface_rmsd = np.concatenate(
+    lig_interface_residues = np.unique(lig_interface.models[0].residue)
+    rec_interface_residues = np.unique(rec_interface.models[0].residue)
+
+    interface_residues = np.concatenate(
         (
-            np.unique(lig_interface.models[0].resid),
-            np.unique(rec_interface.models[0].resid),
+            lig_interface_residues,
+            rec_interface_residues,
         )
     )
 
-    index_1 = coor_1.get_index_select(
-        f'resid {" ".join([str(i) for i in interface_rmsd])} and name {" ".join(back_atom)}'
+    if len(interface_residues) == 0:
+        logger.warning("No interface residues found")
+        return [None] * len(coor.models)
+    
+    # print(f"lig_interface_resids= {lig_interface_residues} rec_interface_resids= {rec_interface_residues}")
+    index = coor.get_index_select(
+        f'residue {" ".join([str(i) for i in interface_residues])} and name {" ".join(back_atom)}'
     )
-    index_2 = coor_2.get_index_select(
-        f'resid {" ".join([str(i) for i in interface_rmsd])} and name {" ".join(back_atom)}'
+    index_native = coor_native.get_index_select(
+        f'residue {" ".join([str(i) for i in interface_residues])} and name {" ".join(back_atom)}'
     )
 
-    alignement.coor_align(coor_1, coor_2, index_1, index_2, frame_ref=0)
+    # print(f"index= {index} index_native= {index_native}")
+    # print(f"index= {len(index)} index_native= {len(index_native)}")
+    assert len(index) == len(index_native), "The number of atoms in the interface is not the same in the two models"
 
-    return rmsd(coor_1, coor_2, index_list=[index_1, index_2])
+    alignement.coor_align(coor, coor_native, index, index_native, frame_ref=0)
+    
+    return rmsd(coor, coor_native, index_list=[index, index_native])
 
 
 def native_contact(
     coor,
     native_coor,
     rec_chain,
     lig_chain,
@@ -176,54 +189,60 @@
 
     Returns
     -------
     float
         Native contact score
     """
 
-    native_rec_interface = native_coor.select_atoms(
-        f'chain {" ".join(native_rec_chain)} and within {cutoff} of chain {" ".join(native_lig_chain)}'
-    )
-
     native_rec_lig_interface = native_coor.select_atoms(
         f'(chain {" ".join(native_rec_chain)} and within {cutoff} of chain {" ".join(native_lig_chain)}) or'
         f'(chain {" ".join(native_lig_chain)} and within {cutoff} of chain {" ".join(native_rec_chain)})'
     )
+    native_rec_interface = native_rec_lig_interface.select_atoms(
+        f'chain {" ".join(native_rec_chain)} and within {cutoff} of chain {" ".join(native_lig_chain)}'
+    )
 
     native_contact_list = []
     native_rec_resid = native_rec_interface.models[0].resid
+
+    # print("native_rec_resid", native_rec_resid)
+
     for residue in np.unique(native_rec_resid):
         res_lig = native_rec_lig_interface.select_atoms(
             f'chain {" ".join(native_lig_chain)} and within {cutoff} of (resid {residue} and chain {" ".join(native_rec_chain)})'
         )
         native_contact_list += [
             [residue, lig_res] for lig_res in np.unique(res_lig.models[0].resid)
         ]
 
+    # print("native_contact_list", native_contact_list)
+
     fnat_list = []
     fnonnat_list = []
     for model in coor.models:
         rec_lig_interface = model.select_atoms(
             f'(chain {" ".join(rec_chain)} and within {cutoff} of chain {" ".join(lig_chain)}) or '
             f'(chain {" ".join(lig_chain)} and within {cutoff} of chain {" ".join(rec_chain)})'
         )
-        rec_interface = model.select_atoms(
+        rec_interface = rec_lig_interface.select_atoms(
             f'(chain {" ".join(rec_chain)} and within {cutoff} of chain {" ".join(lig_chain)})'
         )
 
         model_rec_resid = np.unique(rec_interface.resid)
 
         native_contact_num = 0
         non_native_contact_num = 0
         model_contact_list = []
+
+        # print("model_rec_resid", model_rec_resid)
         for residue in model_rec_resid:
             res_lig = rec_lig_interface.select_atoms(
                 f'chain {" ".join(lig_chain)} and within {cutoff} of (resid {residue} and chain {" ".join(rec_chain)})'
             )
-
+            # print("res_lig", res_lig.resid)
             for lig_res in np.unique(res_lig.resid):
                 if [residue, lig_res] in native_contact_list:
                     native_contact_num += 1
                 else:
                     non_native_contact_num += 1
 
                 model_contact_list.append([residue, lig_res])
@@ -344,21 +363,25 @@
     clean_coor = coor.select_atoms(
         f"protein and not altloc B C D and chain {' '.join(rec_chain + lig_chain)}"
     )
     clean_native_coor = native_coor.select_atoms(
         f"protein and not altloc B C D and chain {' '.join(native_rec_chain + native_lig_chain)}"
     )
 
+    # print("1:", clean_native_coor.models[0].resid[:10])
+
     # Remove incomplete backbone residue:
-    clean_coor = select.remove_incomplete_backbone_residues(clean_coor)
-    clean_native_coor = select.remove_incomplete_backbone_residues(clean_native_coor)
+    clean_coor = remove_incomplete_backbone_residues(clean_coor)
+    clean_native_coor = remove_incomplete_backbone_residues(clean_native_coor)
+    # print("2:", clean_native_coor.models[0].resid[:10])
 
     # Put lig chain at the end of the dict:
     clean_coor.change_order("chain", rec_chain + lig_chain)
     clean_native_coor.change_order("chain", native_rec_chain + native_lig_chain)
+    # print("3:", clean_native_coor.models[0].resid[:10])
 
     # Align model on native structure using model back atoms:
     rmsd_prot_list, [
         align_rec_index,
         align_rec_native_index,
     ] = alignement.align_seq_based(
         clean_coor,
@@ -367,14 +390,15 @@
         chain_2=native_rec_chain,
         back_names=back_atom,
     )
     logger.info(f"Receptor RMSD: {rmsd_prot_list[0]:.3f} A")
     logger.info(
         f"Found {len(align_rec_index)//len(back_atom):d} residues in common (receptor)"
     )
+    # print("4:", clean_native_coor.models[0].resid[:10])
 
     ########################
     # Compute ligand RMSD: #
     ########################
 
     lrmsd_list, [align_lig_index, align_lig_native_index] = alignement.rmsd_seq_based(
         clean_coor,
@@ -383,14 +407,15 @@
         chain_2=native_lig_chain,
         back_names=back_atom,
     )
     logger.info(f"Ligand   RMSD: {lrmsd_list[0]:.3f} A")
     logger.info(
         f"Found {len(align_lig_index)//len(back_atom):d} residues in common (ligand)"
     )
+    # print("5:", clean_native_coor.models[0].resid[:10])
 
     #############################
     # Set same resid in common: #
     #############################
 
     coor_residue = clean_coor.models[0].residue[align_rec_index + align_lig_index]
 
@@ -410,41 +435,46 @@
     interface_coor = clean_coor.select_atoms(
         f'residue {" ".join([str(i) for i in coor_residue_unique])}'
     )
     interface_native_coor = clean_native_coor.select_atoms(
         f'residue {" ".join([str(i) for i in native_residue_unique])}'
     )
 
-    for model in interface_coor.models:
-        model.resid[:] = -1
-        for res, nat_res in zip(coor_residue_unique, native_resid_unique):
-            model.resid[model.residue == res] = nat_res
+    #for model in interface_coor.models:
+    #    model.resid[:] = -1
+    #    for res, nat_res in zip(coor_residue_unique, native_resid_unique):
+    #        model.resid[model.residue == res] = nat_res
+
+    interface_coor.reset_residue_index()
+    interface_native_coor.reset_residue_index()
 
     irmsd_list = interface_rmsd(
         interface_coor,
         interface_native_coor,
         native_rec_chain,
         native_lig_chain,
         cutoff=10.0,
         back_atom=back_atom,
     )
-    logger.info(f"Interface   RMSD: {irmsd_list[0]:.3f} A")
+    logger.info(f"Interface   RMSD: {irmsd_list[0]} A")
 
     fnat_list, fnonnat_list = native_contact(
         clean_coor,
         clean_native_coor,
         rec_chain,
         lig_chain,
         native_rec_chain,
         native_lig_chain,
         cutoff=5.0,
     )
     logger.info(f"Fnat: {fnat_list[0]:.3f}      Fnonnat: {fnonnat_list[0]:.3f}")
 
     def scale_rms(rms, d):
+        if rms is None:
+            return 0.0
         return 1.0 / (1 + (rms / d) ** 2)
 
     d1 = 8.5
     d2 = 1.5
 
     dockq_list = [
         (fnat + scale_rms(lrmsd, d1) + scale_rms(irmsd, d2)) / 3
@@ -464,54 +494,79 @@
 
 
 def compute_pdockQ(
     coor,
     rec_chain=None,
     lig_chain=None,
     cutoff=8.0,
+    L=0.724,
+    x0=152.611,
+    k=0.052,
+    b=0.018,
 ):
     r"""Compute the pdockQ score as define in [1]_.
 
+    pDockQ is computed using this equation [1]_:
+
     .. math::
         pDockQ = \frac{L}{1 + e^{-k (x-x_{0})}} + b
 
     where
 
     .. math::
         x = \overline{plDDT_{interface}} \cdot log(number \: of \: interface \: contacts)
 
     :math:`L = 0.724` is the maximum value of the sigmoid,
     :math:`k = 0.052` is the slope of the sigmoid, :math:`x_{0} = 152.611`
     is the midpoint of the sigmoid, and :math:`b = 0.018` is the y-intercept
     of the sigmoid.
 
+    For the *multiple* pdockQ or `mpDockQ` [2]_ you should use this values:
+
+    :math:`L = 0.728`, :math:`x0 = 309.375`, :math:`k = 0.098` and :math:`b = 0.262`.
+
     Implementation was inspired from https://gitlab.com/ElofssonLab/FoldDock/-/blob/main/src/pdockq.py
 
     Parameters
     ----------
     coor : Coor
         object containing the coordinates of the model
     rec_chain : list
         list of receptor chain
     lig_chain : list
         list of ligand chain
     cutoff : float
         cutoff for native contacts, default is 8.0 A
+    L : float
+        maximum value of the sigmoid, default is 0.728
+    x0 : float
+        midpoint of the sigmoid, default is 309.375
+    k : float
+        slope of the sigmoid, default is 0.098
+    b : float
+        y-intercept of the sigmoid, default is 0.262
+
 
     Returns
     -------
     list
         pdockQ scores
 
+
     References
     ----------
     .. [1] Bryant P, Pozzati G and Elofsson A. Improved prediction of
         protein-protein interactions using AlphaFold2. *Nature Communications*.
         vol. 13, 1265 (2022)
         https://www.nature.com/articles/s41467-022-28865-w
+    .. [2] Bryant P, Pozzati G, Zhu W, Shenoy A, Kundrotas P & Elofsson A. Predicting
+        the structure of large protein complexes using AlphaFold and Monte Carlo
+        tree search. *Nature Communications*.
+        vol. 13, 6028 (2022)
+        https://www.nature.com/articles/s41467-022-33729-4
     """
 
     coor_CA_CB = coor.select_atoms("name CB or (resname GLY and name CA)")
 
     model_seq = coor.get_aa_seq()
 
     if lig_chain is None:
@@ -541,69 +596,93 @@
             pdockq = 0.0
             pdockq_list.append(pdockq)
             continue
 
         avg_plddt = rec_in_contact.len * np.average(
             rec_in_contact.beta
         ) + lig_in_contact.len * np.average(lig_in_contact.beta)
-        avg_plddt /= (rec_in_contact.len + lig_in_contact.len)
+        avg_plddt /= rec_in_contact.len + lig_in_contact.len
 
         x = avg_plddt * np.log10(contact_num)
-        pdockq = 0.724 / (1 + np.exp(-0.052 * (x - 152.611))) + 0.018
+        pdockq = L / (1 + np.exp(-k * (x - x0))) + b
 
         pdockq_list.append(pdockq)
 
     return pdockq_list
 
 
 def compute_pdockQ_sel(
     coor,
     rec_sel,
     lig_sel,
     cutoff=8.0,
+    L=0.724,
+    x0=152.611,
+    k=0.052,
+    b=0.018,
 ):
     r"""Compute the pdockQ score as define in [1]_. Using two selection strings.
+    pDockQ is computed using this equation [1]_:
 
     .. math::
         pDockQ = \frac{L}{1 + e^{-k (x-x_{0})}} + b
 
     where
 
     .. math::
         x = \overline{plDDT_{interface}} \cdot log(number \: of \: interface \: contacts)
 
     :math:`L = 0.724` is the maximum value of the sigmoid,
     :math:`k = 0.052` is the slope of the sigmoid, :math:`x_{0} = 152.611`
     is the midpoint of the sigmoid, and :math:`b = 0.018` is the y-intercept
     of the sigmoid.
 
+    For the *multiple* pdockQ or `mpDockQ` [2]_ you should use this values:
+
+    :math:`L = 0.728`, :math:`x0 = 309.375`, :math:`k = 0.098` and :math:`b = 0.262`.
+
     Implementation was inspired from https://gitlab.com/ElofssonLab/FoldDock/-/blob/main/src/pdockq.py
 
     Parameters
     ----------
     coor : Coor
         object containing the coordinates of the model
     rec_sel : str
         selection string for receptor
     lig_sel : str
         selection string for ligand
     cutoff : float
         cutoff for native contacts, default is 8.0 A
+    L : float
+        maximum value of the sigmoid, default is 0.728
+    x0 : float
+        midpoint of the sigmoid, default is 309.375
+    k : float
+        slope of the sigmoid, default is 0.098
+    b : float
+        y-intercept of the sigmoid, default is 0.262
 
     Returns
     -------
     float
         pdockQ score
 
+
+
     References
     ----------
     .. [1] Bryant P, Pozzati G and Elofsson A. Improved prediction of
         protein-protein interactions using AlphaFold2. *Nature Communications*.
         vol. 13, 1265 (2022)
         https://www.nature.com/articles/s41467-022-28865-w
+    .. [2] Bryant P, Pozzati G, Zhu W, Shenoy A, Kundrotas P & Elofsson A. Predicting
+        the structure of large protein complexes using AlphaFold and Monte Carlo
+        tree search. *Nature Communications*.
+        vol. 13, 6028 (2022)
+        https://www.nature.com/articles/s41467-022-33729-4
     """
 
     coor_CA_CB = coor.select_atoms("name CB or (resname GLY and name CA)")
 
     pdockq_list = []
 
     for model in coor_CA_CB.models:
@@ -622,37 +701,40 @@
             pdockq = 0.0
             pdockq_list.append(pdockq)
             continue
 
         avg_plddt = rec_in_contact.len * np.average(
             rec_in_contact.beta
         ) + lig_in_contact.len * np.average(lig_in_contact.beta)
-        avg_plddt /= (rec_in_contact.len + lig_in_contact.len)
+        avg_plddt /= rec_in_contact.len + lig_in_contact.len
 
         x = avg_plddt * np.log10(contact_num)
-        pdockq = 0.724 / (1 + np.exp(-0.052 * (x - 152.611))) + 0.018
+        pdockq = L / (1 + np.exp(-k * (x - x0))) + b
 
         pdockq_list.append(pdockq)
 
     return pdockq_list
 
 
 def compute_pdockQ2(
     coor,
     pae_array,
-    rec_chain=None,
-    lig_chain=None,
     cutoff=8.0,
+    L=1.31034849e00,
+    x0=8.47326239e01,
+    k=7.47157696e-02,
+    b=5.01886443e-03,
+    d0=10.0,
 ):
     r"""Compute the pdockQ2 score as define in [1]_.
 
     .. math::
         pDockQ_2 = \frac{L}{1 + exp [-k*(X_i-X_0)]} + b
 
-    whith:
+    with:
 
     .. math::
         X_i = \langle \frac{1}{1+(\frac{PAE_{int}}{d_0})^2} \rangle - \langle pLDDT \rangle_{int}
 
     :math:`L = 0.724` is the maximum value of the sigmoid,
     :math:`k = 0.052` is the slope of the sigmoid, :math:`x_{0} = 152.611`
     is the midpoint of the sigmoid, and :math:`b = 0.018` is the y-intercept
@@ -680,98 +762,152 @@
     ----------
     .. [1] Zhu W, Shenoy A, Kundrotras P and Elofsson A. Evaluation of AlphaFold-Multimer prediction
         on multi-chain protein complexes. *Bioinformatics*.
         vol. 39, 7 (2023) btad424
         https://academic.oup.com/bioinformatics/article/39/7/btad424/7219714
     """
 
-    cutoff = 8.0
-    L ,x0, k, b = 1.31034849e+00, 8.47326239e+01, 7.47157696e-02, 5.01886443e-03
-    d0 = 10.0
-
-    models_CA = coor.select_atoms('name CA')
+    models_CA = coor.select_atoms("name CA")
     models_chains = np.unique(models_CA.chain)
 
+    assert pae_array.shape == (models_CA.len, models_CA.len), "PAE array shape mismatch with CA atoms number"
+
     pdockq2_list = []
     for chain in models_chains:
         pdockq2_list.append([])
 
     for model in models_CA.models:
-
         for i, chain in enumerate(models_chains):
+            chain_sel = model.select_atoms(
+                f"(chain {chain} and within {cutoff} of not chain {chain})"
+            )
+            inter_chain_sel = model.select_atoms(
+                f"(not chain {chain} {chain} and within {cutoff} of chain {chain})"
+            )
 
-            chain_sel = model.select_atoms(f"(chain {chain} and within {cutoff} of not chain {chain})")
-            inter_chain_sel = model.select_atoms(f"(not chain {chain} {chain} and within {cutoff} of chain {chain})")
+            if chain_sel.len == 0 or inter_chain_sel.len == 0:
+                pdockq2_list[i].append(0.0)
+                logger.warning("No interface residues found for pdockq2 calculation, 0 value return.")
+                continue
 
             dist_mat = distance_matrix(chain_sel.xyz, inter_chain_sel.xyz)
-            
+
             indexes = np.where(dist_mat < cutoff)
             x_indexes = chain_sel.uniq_resid[indexes[0]]
             y_indexes = inter_chain_sel.uniq_resid[indexes[1]]
             pae_sel = pae_array[x_indexes, y_indexes]
-            
-            norm_if_interpae = np.mean(1/(1+(pae_sel/d0)**2))
+
+            norm_if_interpae = np.mean(1 / (1 + (pae_sel / d0) ** 2))
 
             plddt_avg = np.mean(model.beta[x_indexes])
 
             x = norm_if_interpae * plddt_avg
-            y = L / (1 + np.exp(-k*(x-x0)))+b
+            y = L / (1 + np.exp(-k * (x - x0))) + b
             pdockq2_list[i].append(y)
 
     return pdockq2_list
 
 
+def compute_piTM(
+    coor,
+    pae_array,
+    cutoff=8.0,
+):
+    r"""Compute the piTM score as define in [2]_.
 
+    .. math::
+        piTM = \max_{i \in \mathcal{I}} \frac{1}{I} \sum_{j \in \mathcal{I}}  \frac{1}{1 + [\langle e_{ij} \rangle / d_0 (I)]^2}
 
+    with:
 
+    .. math::
+        d_0(I) = \begin{cases} 1.25 \sqrt[3]{I -15} -1.8\text{,} & \text{if } I \geq 22 \\ 0.02 I \text{,} & \text{if } I < 22  \end{cases}
+    
 
+    Implementation was inspired from `predicted_tm_score_v1()` in https://github.com/FreshAirTonight/af2complex/blob/main/src/alphafold/common/confidence.py
 
+    Parameters
+    ----------
+    coor : Coor
+        object containing the coordinates of the model
+    pae_array : np.array
+        array of predicted PAE
+    cutoff : float
+        cutoff for native contacts, default is 8.0 A
 
+    Returns
+    -------
+    list
+        piTM scores
 
+    References
+    ----------
+    .. [2] Mu Gao, Davi Nakajima An, Jerry M. Parks & Jeffrey Skolnick. 
+        AF2Complex predicts direct physical interactions in multimeric proteins with deep learning
+        *Nature Communications*. volume 13, Article number: 1744 (2022).
+        https://www.nature.com/articles/s41467-022-29394-2
 
+    """
 
+    models_CA = coor.select_atoms("name CA")
+    models_chains = np.unique(models_CA.chain)
 
+    # print(models_chains, pae_array.shape, models_CA.len)
 
+    assert pae_array.shape == (models_CA.len, models_CA.len), "PAE array shape mismatch with CA atoms number"
 
-    coor_CA_CB = coor.select_atoms("name CB or (resname GLY and name CA)")
-
-    model_seq = coor.get_aa_seq()
-
-    if lig_chain is None:
-        lig_chain = [
-            min(model_seq.items(), key=lambda x: len(x[1].replace("-", "")))[0]
-        ]
-    logger.info(f'Model ligand chain : {" ".join(lig_chain)}')
-    if rec_chain is None:
-        rec_chain = [chain for chain in model_seq if chain not in lig_chain]
-    logger.info(f'Model receptor chain : {" ".join(rec_chain)}')
-
-    pdockq_list = []
+    piTM_list = []
 
-    for model in coor_CA_CB.models:
-        rec_in_contact = model.select_atoms(
-            f"chain {' '.join(rec_chain)} and within {cutoff} of chain {' '.join(lig_chain)}"
-        )
+    piTM_Score_list = []
+    for chain in models_chains:
+        piTM_Score_list.append([])
 
-        lig_in_contact = model.select_atoms(
-            f"chain {' '.join(lig_chain)} and within {cutoff} of chain {' '.join(rec_chain)}"
-        )
+    for model in models_CA.models:
 
-        dist_mat = distance_matrix(rec_in_contact.xyz, lig_in_contact.xyz)
-        contact_num = np.sum(dist_mat < cutoff)
+        # Compute I and d0
+        interface_index = []
+        for i, chain in enumerate(models_chains):
+            sel_ndx = model.get_index_select(
+                f"(within {cutoff} of chain {chain}) and (within {cutoff} of not chain {chain})"
+            )
+            interface_index += list(sel_ndx)
+        interface_index = set(interface_index)
 
-        if contact_num == 0:
-            pdockq = 0.0
-            pdockq_list.append(pdockq)
+        I = len(interface_index)
+        if I == 0:
+            piTM_list.append(0)
+            for i in range(len(models_chains)):
+                piTM_Score_list[i].append(0)
             continue
+        d0 = 1.25 * (I -15 ) ** (1 / 3) - 1.8 if I >= 22 else 0.02 * I
 
-        avg_plddt = rec_in_contact.len * np.average(
-            rec_in_contact.beta
-        ) + lig_in_contact.len * np.average(lig_in_contact.beta)
-        avg_plddt /= (rec_in_contact.len + lig_in_contact.len)
+        # Add 0 in case there is no interface residues
+        piTM_local = [0]
+        for i in interface_index:
+            #print(pae_array[:10, :10])
+            local_score = 0
+            for j in interface_index:
+                if i!= j:
+                    local_score += 1 / (1 + (pae_array[i, j] / d0) ** 2)
+            piTM_local.append(local_score)
+        piTM_list.append(max(piTM_local)/I)
 
-        x = avg_plddt * np.log10(contact_num)
-        pdockq = 0.724 / (1 + np.exp(-0.052 * (x - 152.611))) + 0.018
+        for i, chain in enumerate(models_chains):
 
-        pdockq_list.append(pdockq)
+            chain_sel_ndx = model.get_index_select(
+                f"(chain {chain} and within {cutoff} of not chain {chain})"
+            )
+            inter_chain_ndx = model.get_index_select(
+                f"(not chain {chain} {chain} and within {cutoff} of chain {chain})"
+            )
+            # Add 0 in case there is no interface residues
+            chain_score = [0]
+            for j in inter_chain_ndx:
+                local_score = 0
+                for k in chain_sel_ndx:
+                    local_score += 1 / (1 + (pae_array[k, j].mean() / d0) ** 2)
+                chain_score.append(local_score)
 
-    return pdockq_list
+            piTM_Score_list[i].append(max(chain_score)/I)
+            #piTM_Score_list[i].append(max(chain_score)/len(chain_sel_ndx))
+
+    return piTM_list, piTM_Score_list
```

### Comparing `pdb_numpy-0.0.2/src/pdb_numpy/coor.py` & `pdb_numpy-0.0.3/src/pdb_numpy/coor.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,19 +1,19 @@
 #!/usr/bin/env python3
 # coding: utf-8
 
 import logging
 import os
 import copy
 import numpy as np
-from scipy.spatial import distance_matrix
 
 from .data.aa_dict import AA_DICT
 from . import geom
 from .format import mmcif, pdb, pqr, gro
+from .geom import distance_matrix
 
 
 # Logging
 logger = logging.getLogger(__name__)
 
 
 class Coor:
@@ -269,15 +269,15 @@
             pqr.write(self, file_out, overwrite)
         elif str(file_out).endswith(".cif"):
             mmcif.write(self, file_out, overwrite)
         elif str(file_out).endswith(".gro"):
             gro.write(self, file_out, overwrite)
         else:
             logger.warning(
-                "File name doesn't finish with .pdb" " read it as .pdb anyway"
+                "File name doesn't finish with pdb/pqr/cif/gro read it as ``.pdb``."
             )
             pdb.write(self, file_out, overwrite)
 
     def change_order(self, field, order_list):
         """Change the order of the atoms in the model. The `change_order()`
         function takes in two arguments, `field` and `order_list`, which are
         used to change the order of the atoms in the model. The `field` argument
@@ -378,15 +378,16 @@
         residue = -1
         last_residue = self.models[0].atom_dict["num_resid_uniqresid"][0, 2]
         for model in self.models:
             for i in range(model.atom_dict["num_resid_uniqresid"].shape[0]):
                 if model.atom_dict["num_resid_uniqresid"][i, 2] != last_residue:
                     residue += 1
                     last_residue = model.atom_dict["num_resid_uniqresid"][i, 2]
-                model.atom_dict["num_resid_uniqresid"][i, 1] = residue
+                #model.atom_dict["num_resid_uniqresid"][i, 1] = residue
+                model.atom_dict["num_resid_uniqresid"][i, 2] = residue
 
         return
 
     def select_index(self, indexes):
         """The `select_index()` function selects atoms from a Coor object based
         on the provided `indexes` and returns a new `Coor` object with the
         selected atoms.
@@ -402,17 +403,26 @@
 
         Returns
         -------
         Coor
             a new Coor object with the selected atoms
         """
 
-        new_coor = copy.deepcopy(self)
-        for i in range(len(new_coor.models)):
-            new_coor.models[i] = new_coor.models[i].select_index(indexes)
+        #new_coor = copy.deepcopy(self)
+        #for i in range(len(new_coor.models)):
+        #    new_coor.models[i] = new_coor.models[i].select_index(indexes)
+
+        new_coor = Coor()
+        new_coor.models = [model.select_index(indexes) for model in self.models]
+        new_coor.active_model = self.active_model
+        new_coor.crystal_pack = self.crystal_pack
+        new_coor.data_mmCIF = self.data_mmCIF
+        new_coor.symmetry = self.symmetry
+        new_coor.transformation = self.transformation
+        new_coor.data_mmCIF = self.data_mmCIF
 
         return new_coor
 
     def get_index_select(self, selection, frame=0):
         """Return index from the `Coor` object based on the selection string.
 
         Parameters
@@ -509,27 +519,19 @@
 
         # Get CA atoms
         CA_sel = self.select_atoms("name CA", frame=frame)
 
         seq_dict = {}
         aa_num_dict = {}
 
-        for i in range(CA_sel.len):
-            chain = (
-                CA_sel.models[frame]
-                .atom_dict["alterloc_chain_insertres"][i, 1]
-                .astype(np.str_)
-            )
-            res_name = (
-                CA_sel.models[frame]
-                .atom_dict["name_resname_elem"][i, 1]
-                .astype(np.str_)
-            )
-            resid = CA_sel.models[frame].atom_dict["num_resid_uniqresid"][i, 1]
-
+        for chain, res_name, resid in zip(
+            CA_sel.models[frame].atom_dict["alterloc_chain_insertres"][:, 1],
+            CA_sel.models[frame].atom_dict["name_resname_elem"][:, 1],
+            CA_sel.models[frame].atom_dict["num_resid_uniqresid"][:, 1],
+        ):
             if chain not in seq_dict:
                 seq_dict[chain] = ""
                 aa_num_dict[chain] = resid
 
             if res_name in AA_DICT:
                 if resid != aa_num_dict[chain] + 1 and len(seq_dict[chain]) != 0:
                     logger.info(
@@ -538,15 +540,15 @@
                         f"residues"
                     )
                     if gap_in_seq:
                         seq_dict[chain] += "-" * (resid - aa_num_dict[chain] - 1)
                 seq_dict[chain] += AA_DICT[res_name]
                 aa_num_dict[chain] = resid
             else:
-                logger.warning(f"Residue {res_name} in chain {chain} not " "recognized")
+                logger.warning(f"Residue {res_name} in chain {chain} not recognized")
 
         return seq_dict
 
     def get_aa_DL_seq(self, gap_in_seq=True, frame=0):
         """Get the amino acid sequence from a coor object.
         The function calculates the amino acid sequence based
         on the CA atoms in the structure.
@@ -591,30 +593,41 @@
             If atom chains are not arranged sequentially (A,A,A,B,B,A,A,A ...),
             the first atom seq will be overwritten by the last one.
 
         """
 
         # Get CA atoms
         CA_index = self.get_index_select("name CA and not altloc B C D", frame=frame)
+        CA_sel = self.select_atoms("name CA", frame=frame)
+
         N_C_CB_sel = self.select_atoms("name N C CB and not altloc B C D", frame=frame)
 
         seq_dict = {}
         aa_num_dict = {}
 
-        for i in CA_index:
+        for i, chain, res_name, resid, uniq_resid in zip(
+            CA_index,
+            CA_sel.models[frame].atom_dict["alterloc_chain_insertres"][:, 1],
+            CA_sel.models[frame].atom_dict["name_resname_elem"][:, 1],
+            CA_sel.models[frame].atom_dict["num_resid_uniqresid"][:, 1],
+            CA_sel.models[frame].atom_dict["num_resid_uniqresid"][:, 2]
+        ):
+            """"
+            for i in CA_index:
             chain = (
                 self.models[frame]
                 .atom_dict["alterloc_chain_insertres"][i, 1]
                 .astype(np.str_)
             )
             res_name = (
                 self.models[frame].atom_dict["name_resname_elem"][i, 1].astype(np.str_)
             )
             resid = self.models[frame].atom_dict["num_resid_uniqresid"][i, 1]
             uniq_resid = self.models[frame].atom_dict["num_resid_uniqresid"][i, 2]
+            """
 
             if chain not in seq_dict:
                 seq_dict[chain] = ""
                 aa_num_dict[chain] = resid
 
             if res_name in AA_DICT:
                 if resid != aa_num_dict[chain] + 1 and len(seq_dict[chain]) != 0:
@@ -875,14 +888,15 @@
         center_list = []
         for chain in chain_list:
             # print(f'chain {chain}')
             chain_sel = self.models[frame].select_atoms(f"protein and chain {chain}")
             avg = np.average(chain_sel.xyz, axis=0)
             center_list.append(avg)
 
+        center_list = np.array(center_list)
         dist_matrix = distance_matrix(center_list, center_list)
         mask = dist_matrix < cutoff
         # Remove lower triangle and i, (k=0)
         mask[np.tril_indices_from(mask, k=0)] = False
         indices = np.argwhere(mask)
 
         remove_chains = []
```

### Comparing `pdb_numpy-0.0.2/src/pdb_numpy/data/aa_dict.py` & `pdb_numpy-0.0.3/src/pdb_numpy/data/aa_dict.py`

 * *Files 5% similar despite different names*

```diff
@@ -10,16 +10,18 @@
     "HIP": "H",
     "HIE": "H",
     "HID": "H",
     "ARG": "R",
     "LYS": "K",
     "ASP": "D",
     "ASPP": "D",
+    "ASH": "D",
     "GLU": "E",
     "GLUP": "E",
+    "GLH": "E",
     "SER": "S",
     "THR": "T",
     "ASN": "N",
     "GLN": "Q",
     "CYS": "C",
     "SEC": "U",
     "PRO": "P",
```

### Comparing `pdb_numpy-0.0.2/src/pdb_numpy/data/blosum.py` & `pdb_numpy-0.0.3/src/pdb_numpy/data/blosum.py`

 * *Files identical despite different names*

### Comparing `pdb_numpy-0.0.2/src/pdb_numpy/data/blosum62.txt` & `pdb_numpy-0.0.3/src/pdb_numpy/data/blosum62.txt`

 * *Files identical despite different names*

### Comparing `pdb_numpy-0.0.2/src/pdb_numpy/format/gro.py` & `pdb_numpy-0.0.3/src/pdb_numpy/format/gro.py`

 * *Files 2% similar despite different names*

```diff
@@ -38,18 +38,18 @@
     uniq_resid = -1
     old_resid = -1
 
     # Default values
     occ = 0.0
     beta = 0.0
     field = "A"
-    alter_loc = ""
-    chain = ""
-    insert_res = ""
-    elem_symbol = ""
+    alter_loc = "."
+    chain = "?"
+    insert_res = "?"
+    elem_symbol = "?"
 
     index_list = []
     field_list = []  # 6 char
     num_resid_uniqresid_list = []  # int 5 digits (+1 with Chimera)
     alter_chain_insert_list = []  # 1 char
     name_resname_elem_list = []  # 4 / 3 char (+1 with Chimera) = 4
     xyz_list = []  # real (8.3)
@@ -113,15 +113,15 @@
                 ]
             )
 
             if resid != old_resid:
                 uniq_resid += 1
                 old_resid = resid
 
-            field_list.append("A")
+            field_list.append(field)
             num_resid_uniqresid_list.append([atom_num, resid, uniq_resid])
             index_list.append(atom_index)
             name_resname_elem_list.append([atom_name, res_name, elem_symbol])
             alter_chain_insert_list.append([alter_loc, chain, insert_res])
             xyz_list.append(xyz)
             occ_beta_list.append([occ, beta])
 
@@ -148,15 +148,14 @@
     str_out = ""
 
     for model_index, model in enumerate(gro_coor.models):
         str_out += "Create with pdb_numpy\n"
         str_out += f"{model.len:6}\n"
 
         for i in range(model.len):
-
             # Note : Here we use 4 letter residue name.
             str_out += "{:5d}{:5s}{:>5s}{:5d}" "{:8.3f}{:8.3f}{:8.3f}\n".format(
                 model.atom_dict["num_resid_uniqresid"][i, 1],
                 model.atom_dict["name_resname_elem"][i, 1].astype(np.str_),
                 model.atom_dict["name_resname_elem"][i, 0].astype(np.str_),
                 model.atom_dict["num_resid_uniqresid"][i, 0],
                 model.atom_dict["xyz"][i, 0] / 10.0,
@@ -189,15 +188,15 @@
     --------
     >>> prot_coor = Coor(os.path.join(TEST_PATH, '1y0m.pdb'))
     >>> prot_coor.write(os.path.join(TEST_OUT, 'tmp.gro'))
     Succeed to save file tmp.gro
     """
 
     if not overwrite and os.path.exists(gro_out):
-        logger.info(f"GRO file {gro_out} already exist, file not saved")
+        logger.warning(f"GRO file {gro_out} already exist, file not saved")
         return
 
     filout = open(gro_out, "w")
     filout.write(get_gro_string(coor))
     filout.close()
     logger.info(f"Succeed to save file {os.path.relpath(gro_out)}")
     return
```

### Comparing `pdb_numpy-0.0.2/src/pdb_numpy/format/mmcif.py` & `pdb_numpy-0.0.3/src/pdb_numpy/format/mmcif.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,23 +1,24 @@
 #!/usr/bin/env python3
 # coding: utf-8
 
 import os
-import shlex
 from collections import OrderedDict
 import urllib.request
 import logging
 import numpy as np
 import gzip
 
 
 from .. import geom
 from ..model import Model
 from .. import coor
 
+from . import split_cython
+
 # Logging
 logger = logging.getLogger(__name__)
 
 FIELD_DICT = {"A": "ATOM  ", "H": "HETATM"}
 
 MMCIF_ATOM_SITE = (
     "# \n"
@@ -41,14 +42,32 @@
     "_atom_site.auth_seq_id \n"
     "_atom_site.auth_comp_id \n"
     "_atom_site.auth_asym_id \n"
     "_atom_site.auth_atom_id \n"
     "_atom_site.pdbx_PDB_model_num \n"
 )
 
+def remove_double_quote(string):
+    """Remove double quote from a string
+
+    Parameters
+    ----------
+    string : str
+        string with double quote
+
+    Returns
+    -------
+    str
+        string without double quote
+
+    """
+
+    if string[0] == '"':
+        string = string[1:-1]
+    return string
 
 def parse(mmcif_lines):
     """Parse the mmcif lines and return atom information as a dictionary
 
     Parameters
     ----------
 
@@ -77,17 +96,16 @@
         dtype="|U1",
     )
 
     # "num_resid_uniqresid"
     col_index = data_mmCIF["_atom_site"]["col_names"].index("id")
     num_array = np.array(data_mmCIF["_atom_site"]["value"][col_index]).astype(np.int32)
     # check that num_array is consecutive (Maybe useless)
-    assert np.array_equal(
-        num_array, np.arange(1, len(num_array) + 1)
-    ), "Atom numbering is not consecutive"
+    if not np.array_equal(num_array, np.arange(1, len(num_array) + 1)):
+        logger.warning("WARNING: Atom numbering is not consecutive")
 
     col_index = data_mmCIF["_atom_site"]["col_names"].index("auth_seq_id")
     resid_array = np.array(data_mmCIF["_atom_site"]["value"][col_index]).astype(
         np.int32
     )
     uniq_resid_list = []
     uniq_resid = 0
@@ -110,15 +128,15 @@
     num_resid_uniqresid_array = np.column_stack(
         (num_array, resid_array, uniq_resid_array)
     )
 
     # "name_resname"
     col_index = data_mmCIF["_atom_site"]["col_names"].index("label_atom_id")
     # dtype set to U5 to avoid truncation of long atom names like "O5\'"
-    name_array = np.array(data_mmCIF["_atom_site"]["value"][col_index], dtype="|U4")
+    name_array = np.array([remove_double_quote(name) for name in data_mmCIF["_atom_site"]["value"][col_index]], dtype="|U4")
     col_index = data_mmCIF["_atom_site"]["col_names"].index("label_comp_id")
     resname_array = np.array(data_mmCIF["_atom_site"]["value"][col_index], dtype="|U4")
     col_index = data_mmCIF["_atom_site"]["col_names"].index("type_symbol")
     ele_array = np.array(data_mmCIF["_atom_site"]["value"][col_index], dtype="|U4")
 
     name_resname_array = np.column_stack((name_array, resname_array, ele_array))
 
@@ -215,17 +233,23 @@
 
     a = float(data_mmCIF["_cell"]["length_a"])
     b = float(data_mmCIF["_cell"]["length_b"])
     c = float(data_mmCIF["_cell"]["length_c"])
     alpha = float(data_mmCIF["_cell"]["angle_alpha"])
     beta = float(data_mmCIF["_cell"]["angle_beta"])
     gamma = float(data_mmCIF["_cell"]["angle_gamma"])
-    z = int(data_mmCIF["_cell"]["Z_PDB"])
+    if "Z_PDB" in data_mmCIF["_cell"]:
+        z = int(data_mmCIF["_cell"]["Z_PDB"])
+    else:
+        z = 1
 
-    sGroup = data_mmCIF["_symmetry"]["space_group_name_H-M"].replace("'", "")
+    if "_symmetry" in data_mmCIF:
+        sGroup = data_mmCIF["_symmetry"]["space_group_name_H-M"].replace("'", "")
+    else:
+        sGroup = "P 1"
 
     crystal_pack = f"CRYST1{a:9.3f}{b:9.3f}{c:9.3f}{alpha:7.2f}{beta:7.2f}{gamma:7.2f} {sGroup:9} {z:3d}\n"
     return crystal_pack
 
 
 def parse_transformation(data_mmCIF):
     """Parse information from a mmcif file.
@@ -266,15 +290,14 @@
             )
         ]
 
         transformation_dict[1] = {"chains": chain_list, "matrix": []}
 
         if "value" in data_mmCIF["_pdbx_struct_oper_list"]:
             for i in range(len(data_mmCIF["_pdbx_struct_oper_list"]["value"][0])):
-
                 for matrix_index in matrix_indexes:
                     local_matrix = []
                     for index in matrix_index:
                         local_index = data_mmCIF["_pdbx_struct_oper_list"][
                             "col_names"
                         ].index(index)
                         local_matrix.append(
@@ -319,30 +342,42 @@
                 for chain in data_mmCIF["_pdbx_struct_assembly_gen"]["value"][
                     local_matrix_index
                 ][i].split(",")
             ]
             transformation_dict[i + 1] = {"chains": chain_list, "matrix": []}
 
             # Extract matrix value
-            for j in range(len(data_mmCIF["_pdbx_struct_oper_list"]["value"][0])):
-                matrix_id = data_mmCIF["_pdbx_struct_oper_list"]["value"][0][j]
-
+            # print(data_mmCIF["_pdbx_struct_oper_list"])
+            if "value" in data_mmCIF["_pdbx_struct_oper_list"]:
+                for j in range(len(data_mmCIF["_pdbx_struct_oper_list"]["value"][0])):
+                    matrix_id = data_mmCIF["_pdbx_struct_oper_list"]["value"][0][j]
+
+                    if matrix_id in matrix_index_list:
+                        for matrix_index in matrix_indexes:
+                            local_matrix = []
+                            for index in matrix_index:
+                                local_index = data_mmCIF["_pdbx_struct_oper_list"][
+                                    "col_names"
+                                ].index(index)
+                                local_matrix.append(
+                                    float(
+                                        data_mmCIF["_pdbx_struct_oper_list"]["value"][
+                                            local_index
+                                        ][j]
+                                    )
+                                )
+                            transformation_dict[i + 1]["matrix"].append(local_matrix)
+            else:
+                matrix_id = data_mmCIF["_pdbx_struct_oper_list"]["id"]
                 if matrix_id in matrix_index_list:
                     for matrix_index in matrix_indexes:
                         local_matrix = []
                         for index in matrix_index:
-                            local_index = data_mmCIF["_pdbx_struct_oper_list"][
-                                "col_names"
-                            ].index(index)
                             local_matrix.append(
-                                float(
-                                    data_mmCIF["_pdbx_struct_oper_list"]["value"][
-                                        local_index
-                                    ][j]
-                                )
+                                float(data_mmCIF["_pdbx_struct_oper_list"][index])
                             )
                         transformation_dict[i + 1]["matrix"].append(local_matrix)
 
     return transformation_dict
 
 
 def parse_symmetry(data_mmCIF):
@@ -443,15 +478,14 @@
     mmcif_lines : list
         list of pdb lines
 
     Returns
     -------
     dict
         dictionary with atom information
-
     """
 
     data_mmCIF = OrderedDict()
     tabular = False
     mutli_line = ""
 
     category = "title"
@@ -464,15 +498,16 @@
             tabular = False
 
         elif line.startswith("loop_"):
             tabular = True
             col_names = []
 
         elif line.startswith("_"):
-            token = shlex.split(line, posix=False)
+            #token = shlex.split(line, posix=False)
+            token = split_cython.string_split(line[:-1])
             category, attribute = token[0].split(".")
 
             if tabular:
                 if category not in data_mmCIF:
                     data_mmCIF[category] = {"col_names": [], "value": []}
                 data_mmCIF[category]["col_names"].append(attribute)
                 data_mmCIF[category]["value"].append([])
@@ -506,17 +541,24 @@
                 data_mmCIF[category][attribute] = mutli_line
             mutli_line = ""
 
         elif mutli_line:
             mutli_line += line
 
         elif tabular:
-            token = shlex.split(line, posix=False)
+            #token = shlex.split(line, posix=False)
+            token = split_cython.string_split(line[:-1])
+
+            #new_token = line.split()
+            #if set(token) != set(new_token):
+            #    print(line)
+            #    print("shlex:", token)
+            #    print("new  :", new_token)
             token_complete = True
-            # print(final_token, len(final_token), token, len(token), len(data_mmCIF[category]['col_names']))
+            #print(final_token, len(final_token), token, len(token), len(data_mmCIF[category]['col_names']))
 
             # TO FIX !!
             if len(token) != len(data_mmCIF[category]["col_names"]):
                 if len(final_token) == len(data_mmCIF[category]["col_names"]):
                     token = final_token
                 elif len(final_token) + len(token) == len(
                     data_mmCIF[category]["col_names"]
@@ -529,15 +571,17 @@
 
             if token_complete:
                 # print("token complete")
                 for i in range(len(data_mmCIF[category]["col_names"])):
                     data_mmCIF[category]["value"][i].append(token[i])
                 final_token = []
         else:
-            token = shlex.split(line, posix=False)
+            #token = shlex.split(line, posix=False)
+            token = split_cython.string_split(line[:-1])
+
             if category not in data_mmCIF:
                 data_mmCIF[category] = OrderedDict()
             data_mmCIF[category][attribute] = token[0]
 
     return data_mmCIF
 
 
@@ -602,18 +646,15 @@
 
     str_out = ""
 
     line_max_len = 135
     old_category = ""
 
     if len(coor.data_mmCIF) == 0:
-        coor.data_mmCIF = {
-            "title" : {"title": "untitled"},
-            "_entry": {"id": "XXXX"}
-        }
+        coor.data_mmCIF = {"title": {"title": "untitled"}, "_entry": {"id": "XXXX"}}
 
         if coor.crystal_pack.startswith("CRYST1"):
             line = coor.crystal_pack
             a = float(line[6:15])
             b = float(line[15:24])
             c = float(line[24:33])
             alpha = float(line[33:40])
@@ -650,32 +691,31 @@
                 )
                 v3 = np.array(
                     [float(line_split[7]), float(line_split[8]), float(line_split[2])]
                 )
             a = sum(v1**2) ** 0.5 * 10
             b = sum(v2**2) ** 0.5 * 10
             c = sum(v3**2) ** 0.5 * 10
-            alpha = np.rad2deg(angle_vec(v2, v3))
-            beta = np.rad2deg(angle_vec(v1, v3))
-            gamma = np.rad2deg(angle_vec(v1, v2))
-            # Following is wrong, to check !!!
+            alpha = np.rad2deg(geom.angle_vec(v2, v3))
+            beta = np.rad2deg(geom.angle_vec(v1, v3))
+            gamma = np.rad2deg(geom.angle_vec(v1, v2))
+            # Following is probably wrong, to check !!!
             sGroup = "1"
             z = 1
             coor.data_mmCIF["_cell"] = {
                 "length_a": str(a),
                 "length_b": str(b),
                 "length_c": str(c),
                 "angle_alpha": str(alpha),
                 "angle_beta": str(beta),
                 "angle_gamma": str(gamma),
                 "Z_PDB": str(z),
             }
         coor.data_mmCIF["_atom_site"] = None
 
-
     for category in coor.data_mmCIF:
         if category == "title":
             str_out += f"{coor.data_mmCIF[category]['title']}\n"
         elif category == "_atom_site":
             atom_num = coor.total_len
             model_num = 1
             str_out += MMCIF_ATOM_SITE
@@ -704,36 +744,39 @@
             x_size = _get_float_format_size(coor.models[0].atom_dict["xyz"][:, 0])
             y_size = _get_float_format_size(coor.models[0].atom_dict["xyz"][:, 1])
             z_size = _get_float_format_size(coor.models[0].atom_dict["xyz"][:, 2])
             beta_size = _get_float_format_size(
                 coor.models[0].atom_dict["occ_beta"][:, 1], dec_num=2
             )
             for model in coor.models:
+                atom_num = 1
                 for i in range(model.len):
                     alt_pos = (
                         "."
-                        if model.atom_dict["alterloc_chain_insertres"][i, 0] == b""
+                        if model.atom_dict["alterloc_chain_insertres"][i, 0]
+                        in [b"", ""]
                         else model.atom_dict["alterloc_chain_insertres"][i, 0].astype(
                             np.str_
                         )
                     )
                     insert_res = (
                         "?"
-                        if model.atom_dict["alterloc_chain_insertres"][i, 2] == b""
+                        if model.atom_dict["alterloc_chain_insertres"][i, 2]
+                        in [b"", ""]
                         else model.atom_dict["alterloc_chain_insertres"][i, 2].astype(
                             np.str_
                         )
                     )
                     str_out += (
                         "{:6s} {:<{atom_num_size}d} {:{elem_size}s} {:{name_size}s} {:1s} {:{resname_size}s} "
                         "{:{chain_size}s} 1 {:<{resnum_size}d} {:1s} {:<{x_size}.3f} {:<{y_size}.3f} "
                         "{:<{z_size}.3f} {:<4.2f} {:<{beta_size}.2f} {:1s} {:<{resid_size}d}"
                         " {:{resname_size}s} {:{chain_size}s} {:{name_size}s} {:1d}\n".format(
                             FIELD_DICT[model.atom_dict["field"][i]],
-                            model.atom_dict["num_resid_uniqresid"][i, 0],
+                            atom_num,
                             model.atom_dict["name_resname_elem"][i, 2].astype(np.str_),
                             model.atom_dict["name_resname_elem"][i, 0].astype(np.str_),
                             alt_pos,
                             model.atom_dict["name_resname_elem"][i, 1].astype(np.str_),
                             model.atom_dict["alterloc_chain_insertres"][i, 1].astype(
                                 np.str_
                             ),
@@ -761,14 +804,15 @@
                             elem_size=elem_size,
                             resnum_size=resnum_size,
                             resid_size=resid_size,
                             beta_size=beta_size,
                             chain_size=chain_size,
                         )
                     )
+                    atom_num += 1
                 model_num += 1
         else:
             # Add a # for each new category
             if category != old_category:
                 str_out += "# \n"
                 old_category = category
             # Write the loop
@@ -814,23 +858,19 @@
             # Write the data
             else:
                 max_len = (
                     len(max(coor.data_mmCIF[category], key=len)) + len(category) + 3
                 )
                 for attribute in coor.data_mmCIF[category]:
                     if coor.data_mmCIF[category][attribute].startswith(";"):
-                        str_out += (
-                            f"{'.'.join([category, attribute]):{max_len}} \n{coor.data_mmCIF[category][attribute]}"
-                        )
+                        str_out += f"{'.'.join([category, attribute]):{max_len}} \n{coor.data_mmCIF[category][attribute]}"
                     else:
                         local_str = f"{'.'.join([category, attribute]):{max_len}} {coor.data_mmCIF[category][attribute]} \n"
                         if len(local_str) > line_max_len:
-                            str_out += (
-                                f"{'.'.join([category, attribute]):{max_len}} \n{coor.data_mmCIF[category][attribute]} \n"
-                            )
+                            str_out += f"{'.'.join([category, attribute]):{max_len}} \n{coor.data_mmCIF[category][attribute]} \n"
                         else:
                             str_out += local_str
     str_out += "#\n"
 
     return str_out
 
 
@@ -849,15 +889,15 @@
     Returns
     -------
     None
 
     """
 
     if not overwrite and os.path.exists(mmcif_out):
-        logger.info(f"MMCIF file {mmcif_out} already exist, file not saved")
+        logger.warning(f"MMCIF file {mmcif_out} already exist, file not saved")
         return
 
     filout = open(mmcif_out, "w")
     filout.write(get_mmcif_string(coor))
     filout.close()
     logger.info(f"Succeed to save file {os.path.relpath(mmcif_out)}")
     return
```

### Comparing `pdb_numpy-0.0.2/src/pdb_numpy/format/pdb.py` & `pdb_numpy-0.0.3/src/pdb_numpy/format/pdb.py`

 * *Files 14% similar despite different names*

```diff
@@ -7,21 +7,23 @@
 import numpy as np
 import gzip
 
 
 from .. import geom as geom
 from ..model import Model
 from .. import coor
-
+from . import encode_cython as encode
+#from . import encode
 
 # Logging
 logger = logging.getLogger(__name__)
 
 FIELD_DICT = {"A": "ATOM  ", "H": "HETATM"}
 
+CHAIN_LIST = [chr(i) for i in list(range(65, 91)) + list(range(48, 58)) + list(range(97, 123)) + list(range(192, 500))]
 
 def parse(pdb_lines, pqr_format=False):
     """Parse the pdb lines and return atom information's as a dictionary
 
     Parameters
     ----------
     pdb_lines : list
@@ -103,20 +105,20 @@
                 num_resid_uniqresid_list = []  # int 5 digits (+1 with Chimera)
                 alter_chain_insert_list = []  # 1 char
                 name_resname_elem_list = []  # 4 / 3 char (+1 with Chimera) = 4
                 xyz_list = []  # real (8.3)
                 occ_beta_list = []  # real (6.2)
         elif line.startswith("ATOM") or line.startswith("HETATM"):
             field = line[:6].strip()
-            atom_num = int(line[6:11])
+            atom_num = encode.hy36decode(5, line[6:11])
             atom_name = line[12:16].strip()
             res_name = line[17:20].strip()
             chain = line[21]
             # To parse hexadecimal resid:
-            resid = int(line[22:26], base=resid_base)
+            resid = encode.hy36decode(4, line[22:26])
             # If resid is hexadecimal, resid_base is set to 16
             if resid >= 9999:
                 resid_base = 16
             insert_res = line[26:27].strip()
             xyz = [float(line[30:38]), float(line[38:46]), float(line[46:54])]
             if pqr_format:
                 alter_loc = ""
@@ -289,14 +291,39 @@
     req.add_header("Accept-Encoding", "gzip")
 
     with urllib.request.urlopen(req) as response:
         pdb_lines = gzip.decompress(response.read()).decode("utf-8").splitlines(True)
 
     return parse(pdb_lines)
 
+def convert_chain_2_letter(chain: str) -> str:
+    """ For Coor coming from `.mmcif` format,
+    chain ID can be 2 letters long.
+    It has to converted to one letter long in `.pdb` format.
+
+    Parameters
+    ----------
+    chain : str
+        chain ID
+
+    Returns
+    -------
+    str
+        chain ID in one letter long
+    """
+    count = 0
+    base = 65
+    for i, letter in enumerate(chain):
+        if i > 0:
+            base = 64
+        count += 26**i * (ord(letter) - base)
+    if count < len(CHAIN_LIST):
+        return CHAIN_LIST[count]
+    else:
+        return "0"
 
 def get_pdb_string(pdb_coor):
     """Return a coor object as a pdb string.
 
     Parameters
     ----------
     pdb_coor : Coor
@@ -323,49 +350,71 @@
     if pdb_coor.crystal_pack != "":
         str_out += geom.cryst_convert(pdb_coor.crystal_pack, format_out="pdb")
     elif pdb_coor.data_mmCIF is not None:
         str_out += geom.cryst_convert_mmCIF(pdb_coor.data_mmCIF, format_out="pdb")
 
     for model_index, model in enumerate(pdb_coor.models):
         str_out += f"MODEL    {model_index:4d}\n"
+        old_chain = ""
+
+        # Replace mmcif `.` altloc by `''` and `?` insertres by `''`
+        alterloc = ['' if altloc == '.' else altloc for altloc in model.atom_dict["alterloc_chain_insertres"][:, 0]]
+        insertres = ['' if insert == '?' else insert for insert in model.atom_dict["alterloc_chain_insertres"][:, 2]]
+        chain_list = ['' if chain == '?' else chain for chain in model.atom_dict["alterloc_chain_insertres"][:, 1]]
+        elem_symbol = ['' if elem == '?' else elem for elem in model.atom_dict["name_resname_elem"][:, 2]]
+
+        # If resname in 3 letters or less, we add a space at the end
+        mylen = np.vectorize(len)
+        if max(mylen(model.atom_dict["name_resname_elem"][:, 1])) <= 3:
+            resname = np.char.add(model.atom_dict["name_resname_elem"][:, 1], " ")
 
         for i in range(model.len):
-            # Atom name should start a column 14, with the type of atom ex:
+            # Atom name should start at column 14, with the type of atom ex:
             #   - with atom type 'C': ' CH3'
-            # for 2 letters atom type, it should start at coulumn 13 ex:
+            # for 2 letters atom type, it should start at column 13 ex:
             #   - with atom type 'FE': 'FE1'
             name = model.atom_dict["name_resname_elem"][i, 0].astype(np.str_)
             if len(name) <= 3 and name[0] in ["C", "H", "O", "N", "S", "P"]:
                 name = " " + name
-            # To use resid > 9999, we need to convert the resid in hexa
+            # To use resid > 9999, we need to convert the resid in hexadecimal format 
             resid = model.atom_dict["num_resid_uniqresid"][i, 1]
             if resid > 9999:
-                resid = hex(resid).lstrip("0x")
+                resid = encode.hy36encode(4, resid)
             else:
                 resid = str(resid)
+            
+            #chain = model.atom_dict["alterloc_chain_insertres"][i, 1].astype(np.str_)
+
+            if chain_list[i] != old_chain:
+                old_chain = chain_list[i]
+                if len(old_chain) > 1:
+                    out_chain = convert_chain_2_letter(old_chain)
+                else:
+                    out_chain = old_chain
+
 
             # Note : Here we use 4 letter residue name.
             str_out += (
-                "{:6s}{:5d} {:4s}{:1s}{:4s}{:1s}{:>4s}{:1s}"
+                "{:6s}{:5s} {:4s}{:1s}{:>4s}{:1s}{:>4s}{:1s}"
                 "   {:8.3f}{:8.3f}{:8.3f}{:6.2f}{:6.2f}"
-                "          {:2s}\n".format(
+                "          {:>2s}\n".format(
                     FIELD_DICT[model.atom_dict["field"][i]],
-                    i + 1,
+                    encode.hy36encode(5, i + 1),
                     name,
-                    model.atom_dict["alterloc_chain_insertres"][i, 0].astype(np.str_),
-                    model.atom_dict["name_resname_elem"][i, 1].astype(np.str_),
-                    model.atom_dict["alterloc_chain_insertres"][i, 1].astype(np.str_),
+                    alterloc[i],
+                    resname[i],
+                    out_chain,
                     resid,
-                    model.atom_dict["alterloc_chain_insertres"][i, 2].astype(np.str_),
+                    insertres[i],
                     model.atom_dict["xyz"][i, 0],
                     model.atom_dict["xyz"][i, 1],
                     model.atom_dict["xyz"][i, 2],
                     model.atom_dict["occ_beta"][i, 0],
                     model.atom_dict["occ_beta"][i, 1],
-                    model.atom_dict["name_resname_elem"][i, 2].astype(np.str_),
+                    elem_symbol[i],
                 )
             )
         str_out += "ENDMDL\n"
     str_out += "END\n"
     return str_out
 
 
@@ -389,15 +438,15 @@
     --------
     >>> prot_coor = Coor(os.path.join(TEST_PATH, '1y0m.pdb'))
     >>> prot_coor.write_pdb(os.path.join(TEST_OUT, 'tmp.pdb'))
     Succeed to save file tmp.pdb
     """
 
     if not overwrite and os.path.exists(pdb_out):
-        logger.info(f"PDB file {pdb_out} already exist, file not saved")
+        logger.warning(f"PDB file {pdb_out} already exist, file not saved")
         return
 
     filout = open(pdb_out, "w")
     filout.write(get_pdb_string(coor))
     filout.close()
     logger.info(f"Succeed to save file {os.path.relpath(pdb_out)}")
     return
```

### Comparing `pdb_numpy-0.0.2/src/pdb_numpy/format/pqr.py` & `pdb_numpy-0.0.3/src/pdb_numpy/format/pqr.py`

 * *Files 8% similar despite different names*

```diff
@@ -126,13 +126,13 @@
     >>> prot_coor.write_pdb(os.path.join(TEST_OUT, 'tmp.pdb'))\
     #doctest: +ELLIPSIS
     Succeed to save file ...tmp.pdb
 
     """
 
     if not overwrite and os.path.exists(pqr_out):
-        logger.info("PQR file {} already exist, file not saved".format(pqr_out))
+        logger.warning("PQR file {} already exist, file not saved".format(pqr_out))
         return
 
     filout = open(pqr_out, "w")
     filout.write(get_pqr_string(coor))
     filout.close()
```

### Comparing `pdb_numpy-0.0.2/src/pdb_numpy/geom.py` & `pdb_numpy-0.0.3/src/pdb_numpy/geom.py`

 * *Files 24% similar despite different names*

```diff
@@ -322,7 +322,112 @@
     v1_x_v2 = np.cross(v1, v2)
 
     y = np.dot(v1_x_v2, bc) * (1.0 / np.linalg.norm(bc))
     x = np.dot(v1, v2)
     angle = np.arctan2(y, x)
 
     return np.degrees(angle)
+
+
+def distance_matrix(x, y):
+    """Compute the minkowski distance 2th power of the L**p distance
+    between two arrays.
+
+    Taken from:
+    https://github.com/scipy/scipy/blob/main/scipy/spatial/_kdtree.py
+
+    Parameters
+    ----------
+    x : (..., K) array_like
+        Input array.
+    y : (..., K) array_like
+        Input array.
+    p : float, 1 <= p <= infinity
+        Which Minkowski p-norm to use.
+
+    Returns
+    -------
+    dist : ndarray
+        pth power of the distance between the input arrays.
+    """
+    x = np.asarray(x[:,np.newaxis,:])
+    y = np.asarray(y[np.newaxis,:,:])
+    p = 2
+
+    # Find smallest common datatype with float64 (return type of this
+    # function) - addresses #10262.
+    # Don't just cast to float64 for complex input case.
+    common_datatype = np.promote_types(np.promote_types(x.dtype, y.dtype),
+                                       'float64')
+
+    # Make sure x and y are NumPy arrays of correct datatype.
+    x = x.astype(common_datatype)
+    y = y.astype(common_datatype)
+
+    return np.sum(np.abs(y-x)**p, axis=-1)**(1./p)
+
+def makeW(r1, r2, r3, r4=0):
+    """
+    Source: https://github.com/charnley/rmsd/blob/master/rmsd/\
+    calculate_rmsd.py
+    matrix involved in quaternion rotation
+    """
+    W = np.asarray([
+        [r4, r3, -r2, r1],
+        [-r3, r4, r1, r2],
+        [r2, -r1, r4, r3],
+        [-r1, -r2, -r3, r4]])
+    return W
+
+def makeQ(r1, r2, r3, r4=0):
+    """
+    Source: https://github.com/charnley/rmsd/blob/master/rmsd/\
+    calculate_rmsd.py
+    matrix involved in quaternion rotation
+    """
+    Q = np.asarray([
+        [r4, -r3, r2, r1],
+        [r3, r4, -r1, r2],
+        [-r2, r1, r4, r3],
+        [-r1, -r2, -r3, r4]])
+    return Q
+
+def quaternion_transform(r):
+    """
+    Source: https://github.com/charnley/rmsd/blob/master/rmsd/\
+    calculate_rmsd.py
+    Get optimal rotation
+    note: translation will be zero when the centroids of each
+    molecule are the same.
+    """
+    Wt_r = makeW(*r).T
+    Q_r = makeQ(*r)
+    rot = Wt_r.dot(Q_r)[:3, :3]
+    return rot
+    
+def quaternion_rotate(X, Y):
+        """
+        Source: https://github.com/charnley/rmsd/blob/master/rmsd/\
+        calculate_rmsd.py
+        Calculate the rotation matrix between 2 vectors.
+
+        :param coor_1: coordinates array of size (N, D),\
+            where N is points and D is dimension.
+        :type coor_1: np.array
+
+        :param coor_2: coordinates array of size (N, D),\
+            where N is points and D is dimension.
+        :type coor_2: np.array
+
+        :return: rotation matrix
+        :rtype: np.array of size (D, D)
+        """
+        N = X.shape[0]
+        W = np.asarray([makeW(*Y[k]) for k in range(N)])
+        Q = np.asarray([makeQ(*X[k]) for k in range(N)])
+        Qt_dot_W = np.asarray([np.dot(Q[k].T, W[k]) for k in range(N)])
+        # NOTE UNUSED W_minus_Q = np.asarray([W[k] - Q[k] for k in range(N)])
+        A = np.sum(Qt_dot_W, axis=0)
+        eigen = np.linalg.eigh(A)
+        r = eigen[1][:, eigen[0].argmax()]
+        rot = quaternion_transform(r)
+        return rot
```

### Comparing `pdb_numpy-0.0.2/src/pdb_numpy/model.py` & `pdb_numpy-0.0.3/src/pdb_numpy/model.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,22 +1,37 @@
 #!/usr/bin/env python3
 # coding: utf-8
 
 import logging
 import os
 import copy
 import numpy as np
-from scipy.spatial import distance_matrix
 
 from . import select
+from .geom import distance_matrix
 
 # Logging
 logger = logging.getLogger(__name__)
 
 
+KEYWORD_DICT = {
+    "num": ["num_resid_uniqresid", 0],
+    "resname": ["name_resname_elem", 1],
+    "chain": ["alterloc_chain_insertres", 1],
+    "name": ["name_resname_elem", 0],
+    "altloc": ["alterloc_chain_insertres", 0],
+    "resid": ["num_resid_uniqresid", 1],
+    "residue": ["num_resid_uniqresid", 2],
+    "beta": ["occ_beta", 1],
+    "occupancy": ["occ_beta", 0],
+    "x": ["xyz", 0],
+    "y": ["xyz", 1],
+    "z": ["xyz", 2],
+}
+
 class Model:
     """Model class for pdb_numpy
 
     Attributes
     ----------
     atom_dict : dict
         Dictionary containing the atom information
@@ -249,32 +264,17 @@
 
         Returns
         -------
         list
             a list of boolean values for each atom in the PDB file
         """
 
-        keyword_dict = {
-            "num": ["num_resid_uniqresid", 0],
-            "resname": ["name_resname_elem", 1],
-            "chain": ["alterloc_chain_insertres", 1],
-            "name": ["name_resname_elem", 0],
-            "altloc": ["alterloc_chain_insertres", 0],
-            "resid": ["num_resid_uniqresid", 1],
-            "residue": ["num_resid_uniqresid", 2],
-            "beta": ["occ_beta", 1],
-            "occupancy": ["occ_beta", 0],
-            "x": ["xyz", 0],
-            "y": ["xyz", 1],
-            "z": ["xyz", 2],
-        }
-
-        if column in keyword_dict:
-            col = keyword_dict[column][0]
-            index = keyword_dict[column][1]
+        if column in KEYWORD_DICT:
+            col = KEYWORD_DICT[column][0]
+            index = KEYWORD_DICT[column][1]
         else:
             raise ValueError(f"Column {column} not recognized")
 
         if isinstance(values, list):
             if column in ["resname", "chain", "name", "altloc"]:
                 values = np.array(values, dtype="U")
                 # deal with case with "name H*"
@@ -338,16 +338,14 @@
 
         Parameters
         ----------
         self : Model
             Model object
         tokens : list
             List of nested tokens
-        frame : int
-            Frame number for the selection, default is 0
 
         Returns
         -------
         list
             a list of boolean values for each atom in the PDB file
         """
         bool_list = []
@@ -416,18 +414,18 @@
             Frame number for the selection, default is 0
 
         Returns
         -------
         Coor
             a new Coor object with the selected atoms
         """
-
-        new_model = copy.deepcopy(self)
-
-        for key in new_model.atom_dict:
+        
+        new_model = Model()
+        new_model.atom_dict = {}
+        for key in self.atom_dict:
             new_model.atom_dict[key] = self.atom_dict[key][indexes]
 
         return new_model
 
     def get_index_select(self, selection):
         """Return index from the PDB file based on the selection string.
 
@@ -497,15 +495,15 @@
         # Compute distance matrix
         if self.xyz.shape[0] == 0:
             return np.array([])
         elif sel_2.xyz.shape[0] == 0:
             return np.array([False] * self.xyz.shape[0])
         dist_mat = distance_matrix(self.xyz, sel_2.xyz)
 
-        # Retrun column under cutoff_max:
+        # Return column under cutoff_max:
         return dist_mat.min(1) < cutoff
 
     def add_atom(
         self,
         index,
         name,
         resname,
@@ -526,15 +524,15 @@
         ----------
         self : Model
             Model object
         atom : Atom
             Atom object
 
         """
-        
+
         self.atom_dict["field"] = np.insert(
             self.atom_dict["field"], index, ["ATOM"], axis=0
         )
 
         self.atom_dict["num_resid_uniqresid"] = np.insert(
             self.atom_dict["num_resid_uniqresid"],
             index,
@@ -553,21 +551,21 @@
         self.atom_dict["occ_beta"] = np.insert(
             self.atom_dict["occ_beta"], index, [bfactor, occupancy], axis=0
         )
         self.atom_dict["xyz"] = np.insert(self.atom_dict["xyz"], index, xyz, axis=0)
 
         if len(self.atom_dict["field"]) == 1:
             atom_num = 1
-            #self.atom_dict["field"] = self.atom_dict["field"].reshape((atom_num, 1))
+            # self.atom_dict["field"] = self.atom_dict["field"].reshape((atom_num, 1))
             self.atom_dict["num_resid_uniqresid"] = self.atom_dict[
                 "num_resid_uniqresid"
             ].reshape((atom_num, 3))
             self.atom_dict["name_resname_elem"] = self.atom_dict[
                 "name_resname_elem"
             ].reshape((atom_num, 3))
             self.atom_dict["alterloc_chain_insertres"] = self.atom_dict[
                 "alterloc_chain_insertres"
             ].reshape((atom_num, 3))
             self.atom_dict["occ_beta"] = self.atom_dict["occ_beta"].reshape(
                 (atom_num, 2)
             )
-            self.atom_dict["xyz"] = self.atom_dict["xyz"].reshape((atom_num, 3))
+            self.atom_dict["xyz"] = self.atom_dict["xyz"].reshape((atom_num, 3))
```

### Comparing `pdb_numpy-0.0.2/src/pdb_numpy/select.py` & `pdb_numpy-0.0.3/src/pdb_numpy/select.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,12 +1,11 @@
 #!/usr/bin/env python3
 # coding: utf-8
 
 import logging
-import copy
 import numpy as np
 
 from .data.aa_dict import AA_DICT
 
 # Logging
 logger = logging.getLogger(__name__)
 
@@ -228,15 +227,15 @@
 
     if len(uniq_res_num) * len(back_atom) == backbone.len:
         return no_alter_loc
 
     uniq_res_to_remove = []
     for uniq_res in uniq_res_num:
         if sum(backbone.models[0].uniq_resid == uniq_res) != len(back_atom):
-            uniq_res_to_remove.append(uniq_res)
+            uniq_res_to_remove.append(str(uniq_res))
             logger.warning(f"Removing residue {uniq_res} has incomplete backbone atoms")
 
     return no_alter_loc.select_atoms(f'not residue {" ".join(uniq_res_to_remove)}')
 
 
 def remove_hydrogens(coor):
     """Remove hydrogens atoms from the Coor object
```

### Comparing `pdb_numpy-0.0.2/src/pdb_numpy/visu.py` & `pdb_numpy-0.0.3/src/pdb_numpy/visu.py`

 * *Files 20% similar despite different names*

```diff
@@ -5,15 +5,15 @@
 from .format import pdb
 import logging
 
 # Logging
 logger = logging.getLogger(__name__)
 
 
-def get_view(
+def get_nglview(
     coor,
     ref=None,
     cartoon=True,
     licorice=False,
     unitcell=False,
     color="chainid",
     **kwargs
@@ -39,15 +39,15 @@
         nglview object
 
     Examples
     --------
     >>> import pdb_numpy
     >>> from pdb_numpy import visu
     >>> coor = pdb_numpy.Coor('test.pdb')
-    >>> visu.get_view(coor)
+    >>> visu.get_nglview(coor)
 
     """
 
     try:
         import nglview as nv
     except ImportError:
         logger.warning("nglview is not installed\n Use `pip install nglview`")
@@ -62,20 +62,77 @@
         view.add_licorice()
     if unitcell:
         view.add_unitcell()
 
     if ref is not None:
         ref_str = nv.TextStructure(pdb.get_pdb_string(ref))
         view.add_component(ref_str, default=False)
-        view[1].add_cartoon(selection="protein", color='red')
+        view[1].add_cartoon(selection="protein", color="red")
         view[1].add_representation("licorice", selection="ligand", color="red")
 
     return view
 
 
+def get_py3dmolview(
+    coor,
+    ref=None,
+    cartoon=True,
+    licorice=False,
+    unitcell=False,
+    color="chainid",
+    **kwargs
+):
+    """Return a `py3dmol` object to be view in
+    a jupyter notebook.
+
+    Parameters
+    ----------
+    coor : Coor
+        Coor object
+    ref : Coor
+        Reference Coor object
+    licorice : bool, optional
+        Add a licorice representation of the ligand, by default False
+    color : str, optional
+        Color representation, by default 'chain'
+
+
+    Returns
+    -------
+    py3dmol.Widget
+        py3dmol object
+
+    Examples
+    --------
+    >>> import pdb_numpy
+    >>> from pdb_numpy import visu
+    >>> coor = pdb_numpy.Coor('test.pdb')
+    >>> visu.get_py3dmolview(coor)
+
+    """
+
+    try:
+        import py3Dmol
+    except ImportError:
+        logger.warning("py3dmol is not installed\n Use `pip install py3dmol`")
+        return
+
+    view = py3Dmol.view(width=400, height=400)
+    view.addModelsAsFrames(pdb.get_pdb_string(coor))
+    view.setStyle({"model": -1}, {"cartoon": {"color": "spectrum"}})
+
+    if ref is not None:
+        view.addModelsAsFrames(pdb.get_pdb_string(ref))
+        view.setStyle({"model": -1}, {"cartoon": {"color": "red"}})
+
+    view.zoomTo()
+
+    return view
+
+
 def plot_pseudo_3D(
     coor,
     c_field="index",
     cmap="gist_rainbow",
     line_w=1.5,
     chainbreak=5.0,
     sel="name CA",
```

