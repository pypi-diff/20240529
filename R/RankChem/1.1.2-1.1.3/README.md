# Comparing `tmp/rankchem-1.1.2.tar.gz` & `tmp/rankchem-1.1.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "rankchem-1.1.2.tar", last modified: Wed May 29 17:01:08 2024, max compression
+gzip compressed data, was "rankchem-1.1.3.tar", last modified: Wed May 29 17:27:12 2024, max compression
```

## Comparing `rankchem-1.1.2.tar` & `rankchem-1.1.3.tar`

### file list

```diff
@@ -1,22 +1,22 @@
-drwxrwxrwx   0 emmaunix  (1000) emmaunix  (1000)        0 2024-05-29 17:01:08.544939 rankchem-1.1.2/
--rwxrwxrwx   0 emmaunix  (1000) emmaunix  (1000)     1164 2024-05-17 18:59:58.000000 rankchem-1.1.2/LICENSE
--rwxrwxrwx   0 emmaunix  (1000) emmaunix  (1000)    10447 2024-05-29 17:01:08.535605 rankchem-1.1.2/PKG-INFO
--rwxrwxrwx   0 emmaunix  (1000) emmaunix  (1000)     7698 2024-05-29 16:47:22.000000 rankchem-1.1.2/README.md
--rwxrwxrwx   0 emmaunix  (1000) emmaunix  (1000)     1719 2024-05-29 16:47:22.000000 rankchem-1.1.2/pyproject.toml
--rwxrwxrwx   0 emmaunix  (1000) emmaunix  (1000)       38 2024-05-29 17:01:08.546160 rankchem-1.1.2/setup.cfg
--rwxrwxrwx   0 emmaunix  (1000) emmaunix  (1000)     1183 2024-05-29 16:59:54.000000 rankchem-1.1.2/setup.py
-drwxrwxrwx   0 emmaunix  (1000) emmaunix  (1000)        0 2024-05-29 17:01:08.233177 rankchem-1.1.2/src/
-drwxrwxrwx   0 emmaunix  (1000) emmaunix  (1000)        0 2024-05-29 17:01:08.522565 rankchem-1.1.2/src/RankChem.egg-info/
--rwxrwxrwx   0 emmaunix  (1000) emmaunix  (1000)    10447 2024-05-29 17:01:07.000000 rankchem-1.1.2/src/RankChem.egg-info/PKG-INFO
--rwxrwxrwx   0 emmaunix  (1000) emmaunix  (1000)      431 2024-05-29 17:01:08.000000 rankchem-1.1.2/src/RankChem.egg-info/SOURCES.txt
--rwxrwxrwx   0 emmaunix  (1000) emmaunix  (1000)        1 2024-05-29 17:01:07.000000 rankchem-1.1.2/src/RankChem.egg-info/dependency_links.txt
--rwxrwxrwx   0 emmaunix  (1000) emmaunix  (1000)      169 2024-05-29 17:01:07.000000 rankchem-1.1.2/src/RankChem.egg-info/requires.txt
--rwxrwxrwx   0 emmaunix  (1000) emmaunix  (1000)        1 2024-05-29 17:01:07.000000 rankchem-1.1.2/src/RankChem.egg-info/top_level.txt
-drwxrwxrwx   0 emmaunix  (1000) emmaunix  (1000)        0 2024-05-29 17:01:08.494829 rankchem-1.1.2/tests/
--rwxrwxrwx   0 emmaunix  (1000) emmaunix  (1000)      608 2024-05-26 13:57:31.000000 rankchem-1.1.2/tests/test_average.py
--rwxrwxrwx   0 emmaunix  (1000) emmaunix  (1000)      592 2024-05-26 13:58:59.000000 rankchem-1.1.2/tests/test_calculate_descriptor.py
--rwxrwxrwx   0 emmaunix  (1000) emmaunix  (1000)      749 2024-05-26 12:24:41.000000 rankchem-1.1.2/tests/test_calculate_fukui.py
--rwxrwxrwx   0 emmaunix  (1000) emmaunix  (1000)      483 2024-05-26 12:24:41.000000 rankchem-1.1.2/tests/test_get_max_fukui_avg.py
--rwxrwxrwx   0 emmaunix  (1000) emmaunix  (1000)      665 2024-05-26 14:00:42.000000 rankchem-1.1.2/tests/test_rank_descriptors.py
--rwxrwxrwx   0 emmaunix  (1000) emmaunix  (1000)      617 2024-05-26 12:24:41.000000 rankchem-1.1.2/tests/test_smiles_to_xyz.py
--rwxrwxrwx   0 emmaunix  (1000) emmaunix  (1000)      409 2024-05-26 13:57:17.000000 rankchem-1.1.2/tests/test_visualize_molecule.py
+drwxrwxrwx   0 emmaunix  (1000) emmaunix  (1000)        0 2024-05-29 17:27:12.541951 rankchem-1.1.3/
+-rwxrwxrwx   0 emmaunix  (1000) emmaunix  (1000)     1164 2024-05-17 18:59:58.000000 rankchem-1.1.3/LICENSE
+-rwxrwxrwx   0 emmaunix  (1000) emmaunix  (1000)    10447 2024-05-29 17:27:12.519823 rankchem-1.1.3/PKG-INFO
+-rwxrwxrwx   0 emmaunix  (1000) emmaunix  (1000)     7698 2024-05-29 16:47:22.000000 rankchem-1.1.3/README.md
+-rwxrwxrwx   0 emmaunix  (1000) emmaunix  (1000)     1719 2024-05-29 16:47:22.000000 rankchem-1.1.3/pyproject.toml
+-rwxrwxrwx   0 emmaunix  (1000) emmaunix  (1000)       38 2024-05-29 17:27:12.544488 rankchem-1.1.3/setup.cfg
+-rwxrwxrwx   0 emmaunix  (1000) emmaunix  (1000)     1289 2024-05-29 17:26:23.000000 rankchem-1.1.3/setup.py
+drwxrwxrwx   0 emmaunix  (1000) emmaunix  (1000)        0 2024-05-29 17:27:11.530072 rankchem-1.1.3/src/
+drwxrwxrwx   0 emmaunix  (1000) emmaunix  (1000)        0 2024-05-29 17:27:12.489808 rankchem-1.1.3/src/RankChem.egg-info/
+-rwxrwxrwx   0 emmaunix  (1000) emmaunix  (1000)    10447 2024-05-29 17:27:11.000000 rankchem-1.1.3/src/RankChem.egg-info/PKG-INFO
+-rwxrwxrwx   0 emmaunix  (1000) emmaunix  (1000)      431 2024-05-29 17:27:11.000000 rankchem-1.1.3/src/RankChem.egg-info/SOURCES.txt
+-rwxrwxrwx   0 emmaunix  (1000) emmaunix  (1000)        1 2024-05-29 17:27:11.000000 rankchem-1.1.3/src/RankChem.egg-info/dependency_links.txt
+-rwxrwxrwx   0 emmaunix  (1000) emmaunix  (1000)      169 2024-05-29 17:27:11.000000 rankchem-1.1.3/src/RankChem.egg-info/requires.txt
+-rwxrwxrwx   0 emmaunix  (1000) emmaunix  (1000)        1 2024-05-29 17:27:11.000000 rankchem-1.1.3/src/RankChem.egg-info/top_level.txt
+drwxrwxrwx   0 emmaunix  (1000) emmaunix  (1000)        0 2024-05-29 17:27:12.401814 rankchem-1.1.3/tests/
+-rwxrwxrwx   0 emmaunix  (1000) emmaunix  (1000)      608 2024-05-26 13:57:31.000000 rankchem-1.1.3/tests/test_average.py
+-rwxrwxrwx   0 emmaunix  (1000) emmaunix  (1000)      592 2024-05-26 13:58:59.000000 rankchem-1.1.3/tests/test_calculate_descriptor.py
+-rwxrwxrwx   0 emmaunix  (1000) emmaunix  (1000)      749 2024-05-26 12:24:41.000000 rankchem-1.1.3/tests/test_calculate_fukui.py
+-rwxrwxrwx   0 emmaunix  (1000) emmaunix  (1000)      483 2024-05-26 12:24:41.000000 rankchem-1.1.3/tests/test_get_max_fukui_avg.py
+-rwxrwxrwx   0 emmaunix  (1000) emmaunix  (1000)      665 2024-05-26 14:00:42.000000 rankchem-1.1.3/tests/test_rank_descriptors.py
+-rwxrwxrwx   0 emmaunix  (1000) emmaunix  (1000)      617 2024-05-26 12:24:41.000000 rankchem-1.1.3/tests/test_smiles_to_xyz.py
+-rwxrwxrwx   0 emmaunix  (1000) emmaunix  (1000)      409 2024-05-26 13:57:17.000000 rankchem-1.1.3/tests/test_visualize_molecule.py
```

### Comparing `rankchem-1.1.2/LICENSE` & `rankchem-1.1.3/LICENSE`

 * *Files identical despite different names*

### Comparing `rankchem-1.1.2/PKG-INFO` & `rankchem-1.1.3/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: RankChem
-Version: 1.1.2
+Version: 1.1.3
 Summary: RankChem project
 Home-page: https://github.com/kappelemma/RankChem
 Author: Emma Kappeler, Ludovica Fracassi
 Author-email: Emma Kappeler <emma.kappeler@epfl.ch>, Ludovica Fracassi <ludovica.fracassi@epfl.ch>
 License: MIT License
         
         Copyright (c) 2024 by Emma Kappeler <emma.kappeler@epfl.ch>,
```

### Comparing `rankchem-1.1.2/README.md` & `rankchem-1.1.3/README.md`

 * *Files identical despite different names*

### Comparing `rankchem-1.1.2/pyproject.toml` & `rankchem-1.1.3/pyproject.toml`

 * *Files identical despite different names*

### Comparing `rankchem-1.1.2/setup.py` & `rankchem-1.1.3/setup.py`

 * *Files 17% similar despite different names*

```diff
@@ -1,27 +1,31 @@
 from setuptools import setup, find_packages
 
+with open('README.md', 'r', encoding='utf-8') as fh:
+    long_description = fh.read()
+
 setup(
     name='rankchem',
-    version='1.1.2',
-    packages=find_packages(where='src/RankChem/for_streamlit'),
+    version='1.1.3',
+    packages=find_packages(where='src'),
     package_dir={'': 'src'},
     install_requires=[
         'rdkit',
         'morfeus-ml',
         'pyvistaqt',
         'numpy',
         'py3Dmol',
         'streamlit',
         'stmol'
     ],
     python_requires='>=3.8',
     author='Emma Kappeler, Ludovica Fracassi',
-    author_email='emma.kappeler@epfl.ch, ludovica.fracassi@epfl.ch',
+    author_email='emma.kappeler@epfl.ch,ludovica.fracassi@epfl.ch',
     description='RankChem project',
+    long_description=long_description,
     long_description_content_type='text/markdown',
     url='https://github.com/kappelemma/RankChem',
     classifiers=[
         'Development Status :: 3 - Alpha',
         'Intended Audience :: Developers',
         'License :: OSI Approved :: MIT License',
         'Operating System :: OS Independent',
```

### Comparing `rankchem-1.1.2/src/RankChem.egg-info/PKG-INFO` & `rankchem-1.1.3/src/RankChem.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: RankChem
-Version: 1.1.2
+Version: 1.1.3
 Summary: RankChem project
 Home-page: https://github.com/kappelemma/RankChem
 Author: Emma Kappeler, Ludovica Fracassi
 Author-email: Emma Kappeler <emma.kappeler@epfl.ch>, Ludovica Fracassi <ludovica.fracassi@epfl.ch>
 License: MIT License
         
         Copyright (c) 2024 by Emma Kappeler <emma.kappeler@epfl.ch>,
```

### Comparing `rankchem-1.1.2/tests/test_average.py` & `rankchem-1.1.3/tests/test_average.py`

 * *Files identical despite different names*

### Comparing `rankchem-1.1.2/tests/test_calculate_descriptor.py` & `rankchem-1.1.3/tests/test_calculate_descriptor.py`

 * *Files identical despite different names*

### Comparing `rankchem-1.1.2/tests/test_calculate_fukui.py` & `rankchem-1.1.3/tests/test_calculate_fukui.py`

 * *Files identical despite different names*

### Comparing `rankchem-1.1.2/tests/test_rank_descriptors.py` & `rankchem-1.1.3/tests/test_rank_descriptors.py`

 * *Files identical despite different names*

### Comparing `rankchem-1.1.2/tests/test_smiles_to_xyz.py` & `rankchem-1.1.3/tests/test_smiles_to_xyz.py`

 * *Files identical despite different names*

