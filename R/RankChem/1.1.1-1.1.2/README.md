# Comparing `tmp/rankchem-1.1.1.tar.gz` & `tmp/rankchem-1.1.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "rankchem-1.1.1.tar", last modified: Wed May 29 14:34:15 2024, max compression
+gzip compressed data, was "rankchem-1.1.2.tar", last modified: Wed May 29 17:01:08 2024, max compression
```

## Comparing `rankchem-1.1.1.tar` & `rankchem-1.1.2.tar`

### file list

```diff
@@ -1,24 +1,22 @@
-drwxrwxrwx   0 emmaunix  (1000) emmaunix  (1000)        0 2024-05-29 14:34:15.195316 rankchem-1.1.1/
--rwxrwxrwx   0 emmaunix  (1000) emmaunix  (1000)     1164 2024-05-17 18:59:58.000000 rankchem-1.1.1/LICENSE
--rwxrwxrwx   0 emmaunix  (1000) emmaunix  (1000)    10447 2024-05-29 14:34:15.187876 rankchem-1.1.1/PKG-INFO
--rwxrwxrwx   0 emmaunix  (1000) emmaunix  (1000)     7698 2024-05-28 11:58:59.000000 rankchem-1.1.1/README.md
--rwxrwxrwx   0 emmaunix  (1000) emmaunix  (1000)     1619 2024-05-29 14:27:15.000000 rankchem-1.1.1/pyproject.toml
--rwxrwxrwx   0 emmaunix  (1000) emmaunix  (1000)       38 2024-05-29 14:34:15.196702 rankchem-1.1.1/setup.cfg
--rwxrwxrwx   0 emmaunix  (1000) emmaunix  (1000)     1124 2024-05-29 14:27:19.000000 rankchem-1.1.1/setup.py
-drwxrwxrwx   0 emmaunix  (1000) emmaunix  (1000)        0 2024-05-29 14:34:14.270226 rankchem-1.1.1/src/
-drwxrwxrwx   0 emmaunix  (1000) emmaunix  (1000)        0 2024-05-29 14:34:15.173876 rankchem-1.1.1/src/RankChem.egg-info/
--rwxrwxrwx   0 emmaunix  (1000) emmaunix  (1000)    10447 2024-05-29 14:34:13.000000 rankchem-1.1.1/src/RankChem.egg-info/PKG-INFO
--rwxrwxrwx   0 emmaunix  (1000) emmaunix  (1000)      456 2024-05-29 14:34:14.000000 rankchem-1.1.1/src/RankChem.egg-info/SOURCES.txt
--rwxrwxrwx   0 emmaunix  (1000) emmaunix  (1000)        1 2024-05-29 14:34:13.000000 rankchem-1.1.1/src/RankChem.egg-info/dependency_links.txt
--rwxrwxrwx   0 emmaunix  (1000) emmaunix  (1000)      169 2024-05-29 14:34:13.000000 rankchem-1.1.1/src/RankChem.egg-info/requires.txt
--rwxrwxrwx   0 emmaunix  (1000) emmaunix  (1000)        9 2024-05-29 14:34:13.000000 rankchem-1.1.1/src/RankChem.egg-info/top_level.txt
-drwxrwxrwx   0 emmaunix  (1000) emmaunix  (1000)        0 2024-05-29 14:34:14.842744 rankchem-1.1.1/src/Rankchem/
--rwxrwxrwx   0 emmaunix  (1000) emmaunix  (1000)       82 2024-05-17 18:01:00.000000 rankchem-1.1.1/src/Rankchem/__init__.py
-drwxrwxrwx   0 emmaunix  (1000) emmaunix  (1000)        0 2024-05-29 14:34:15.135890 rankchem-1.1.1/tests/
--rwxrwxrwx   0 emmaunix  (1000) emmaunix  (1000)      608 2024-05-26 13:57:31.000000 rankchem-1.1.1/tests/test_average.py
--rwxrwxrwx   0 emmaunix  (1000) emmaunix  (1000)      592 2024-05-26 13:58:59.000000 rankchem-1.1.1/tests/test_calculate_descriptor.py
--rwxrwxrwx   0 emmaunix  (1000) emmaunix  (1000)      749 2024-05-26 12:24:41.000000 rankchem-1.1.1/tests/test_calculate_fukui.py
--rwxrwxrwx   0 emmaunix  (1000) emmaunix  (1000)      483 2024-05-26 12:24:41.000000 rankchem-1.1.1/tests/test_get_max_fukui_avg.py
--rwxrwxrwx   0 emmaunix  (1000) emmaunix  (1000)      665 2024-05-26 14:00:42.000000 rankchem-1.1.1/tests/test_rank_descriptors.py
--rwxrwxrwx   0 emmaunix  (1000) emmaunix  (1000)      617 2024-05-26 12:24:41.000000 rankchem-1.1.1/tests/test_smiles_to_xyz.py
--rwxrwxrwx   0 emmaunix  (1000) emmaunix  (1000)      409 2024-05-26 13:57:17.000000 rankchem-1.1.1/tests/test_visualize_molecule.py
+drwxrwxrwx   0 emmaunix  (1000) emmaunix  (1000)        0 2024-05-29 17:01:08.544939 rankchem-1.1.2/
+-rwxrwxrwx   0 emmaunix  (1000) emmaunix  (1000)     1164 2024-05-17 18:59:58.000000 rankchem-1.1.2/LICENSE
+-rwxrwxrwx   0 emmaunix  (1000) emmaunix  (1000)    10447 2024-05-29 17:01:08.535605 rankchem-1.1.2/PKG-INFO
+-rwxrwxrwx   0 emmaunix  (1000) emmaunix  (1000)     7698 2024-05-29 16:47:22.000000 rankchem-1.1.2/README.md
+-rwxrwxrwx   0 emmaunix  (1000) emmaunix  (1000)     1719 2024-05-29 16:47:22.000000 rankchem-1.1.2/pyproject.toml
+-rwxrwxrwx   0 emmaunix  (1000) emmaunix  (1000)       38 2024-05-29 17:01:08.546160 rankchem-1.1.2/setup.cfg
+-rwxrwxrwx   0 emmaunix  (1000) emmaunix  (1000)     1183 2024-05-29 16:59:54.000000 rankchem-1.1.2/setup.py
+drwxrwxrwx   0 emmaunix  (1000) emmaunix  (1000)        0 2024-05-29 17:01:08.233177 rankchem-1.1.2/src/
+drwxrwxrwx   0 emmaunix  (1000) emmaunix  (1000)        0 2024-05-29 17:01:08.522565 rankchem-1.1.2/src/RankChem.egg-info/
+-rwxrwxrwx   0 emmaunix  (1000) emmaunix  (1000)    10447 2024-05-29 17:01:07.000000 rankchem-1.1.2/src/RankChem.egg-info/PKG-INFO
+-rwxrwxrwx   0 emmaunix  (1000) emmaunix  (1000)      431 2024-05-29 17:01:08.000000 rankchem-1.1.2/src/RankChem.egg-info/SOURCES.txt
+-rwxrwxrwx   0 emmaunix  (1000) emmaunix  (1000)        1 2024-05-29 17:01:07.000000 rankchem-1.1.2/src/RankChem.egg-info/dependency_links.txt
+-rwxrwxrwx   0 emmaunix  (1000) emmaunix  (1000)      169 2024-05-29 17:01:07.000000 rankchem-1.1.2/src/RankChem.egg-info/requires.txt
+-rwxrwxrwx   0 emmaunix  (1000) emmaunix  (1000)        1 2024-05-29 17:01:07.000000 rankchem-1.1.2/src/RankChem.egg-info/top_level.txt
+drwxrwxrwx   0 emmaunix  (1000) emmaunix  (1000)        0 2024-05-29 17:01:08.494829 rankchem-1.1.2/tests/
+-rwxrwxrwx   0 emmaunix  (1000) emmaunix  (1000)      608 2024-05-26 13:57:31.000000 rankchem-1.1.2/tests/test_average.py
+-rwxrwxrwx   0 emmaunix  (1000) emmaunix  (1000)      592 2024-05-26 13:58:59.000000 rankchem-1.1.2/tests/test_calculate_descriptor.py
+-rwxrwxrwx   0 emmaunix  (1000) emmaunix  (1000)      749 2024-05-26 12:24:41.000000 rankchem-1.1.2/tests/test_calculate_fukui.py
+-rwxrwxrwx   0 emmaunix  (1000) emmaunix  (1000)      483 2024-05-26 12:24:41.000000 rankchem-1.1.2/tests/test_get_max_fukui_avg.py
+-rwxrwxrwx   0 emmaunix  (1000) emmaunix  (1000)      665 2024-05-26 14:00:42.000000 rankchem-1.1.2/tests/test_rank_descriptors.py
+-rwxrwxrwx   0 emmaunix  (1000) emmaunix  (1000)      617 2024-05-26 12:24:41.000000 rankchem-1.1.2/tests/test_smiles_to_xyz.py
+-rwxrwxrwx   0 emmaunix  (1000) emmaunix  (1000)      409 2024-05-26 13:57:17.000000 rankchem-1.1.2/tests/test_visualize_molecule.py
```

### Comparing `rankchem-1.1.1/LICENSE` & `rankchem-1.1.2/LICENSE`

 * *Files identical despite different names*

### Comparing `rankchem-1.1.1/PKG-INFO` & `rankchem-1.1.2/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: RankChem
-Version: 1.1.1
+Version: 1.1.2
 Summary: RankChem project
 Home-page: https://github.com/kappelemma/RankChem
 Author: Emma Kappeler, Ludovica Fracassi
 Author-email: Emma Kappeler <emma.kappeler@epfl.ch>, Ludovica Fracassi <ludovica.fracassi@epfl.ch>
 License: MIT License
         
         Copyright (c) 2024 by Emma Kappeler <emma.kappeler@epfl.ch>,
@@ -98,15 +98,15 @@
 ```
 Where myenv is the name of your environment.
 
 The package runs on python 3.10 but supports python 3.8 through 3.10.
 RankChem can be installed using pip as followed:
 
 ```bash
-pip install Rankchem
+pip install RankChem
 ```
 
 The package can also be installed from source by running the following commands:
 
 First, clone the repository from Github and go in the RankChem folder.
 
 ```bash
```

### Comparing `rankchem-1.1.1/README.md` & `rankchem-1.1.2/README.md`

 * *Files 0% similar despite different names*

```diff
@@ -34,15 +34,15 @@
 ```
 Where myenv is the name of your environment.
 
 The package runs on python 3.10 but supports python 3.8 through 3.10.
 RankChem can be installed using pip as followed:
 
 ```bash
-pip install Rankchem
+pip install RankChem
 ```
 
 The package can also be installed from source by running the following commands:
 
 First, clone the repository from Github and go in the RankChem folder.
 
 ```bash
```

### Comparing `rankchem-1.1.1/pyproject.toml` & `rankchem-1.1.2/pyproject.toml`

 * *Files 27% similar despite different names*

```diff
@@ -1,79 +1,78 @@
-[build-system] 
-requires = ["hatchling"]
-build-backend = "hatchling.build"
-
-[tool.hatch.build.targets.wheel]
-packages = ["src/Rankchem"]
-
-[project]
-name = "RankChem"
-readme = "README.md"
-requires-python = ">=3.8"
-license = {file = "LICENSE"}
-description = "RankChem project"
-dependencies = [
-     "rdkit",
-     "morfeus-ml",
-     "pyvistaqt",
-     "numpy",
-     "py3Dmol",
-     "streamlit",
-     "stmol"
-]
-
-
-authors = [
-    {name = "Emma Kappeler", email = "emma.kappeler@epfl.ch"},
-    {name = "Ludovica Fracassi", email = "ludovica.fracassi@epfl.ch"}
-]
-classifiers = [
-    "Development Status :: 3 - Alpha",
-    "Intended Audience :: Developers",
-    "License :: OSI Approved :: MIT License",
-    "Operating System :: OS Independent",
-    "Programming Language :: Python",
-    "Programming Language :: Python :: 3",
-    "Programming Language :: Python :: 3.8",
-    "Programming Language :: Python :: 3.9",
-    "Programming Language :: Python :: 3.10",
-    "Programming Language :: Python :: 3.11",
-]
-dynamic = ["version"]
-
-[project.urls]
-source = "https://github.com/kappelemma/RankChem"
-tracker = "https://github.com/kappelemma/RankChem/issues"
-
-[project.optional-dependencies]
-test = [
-    "hypothesis",
-    "pytest",
-    "pytest-cov",
-    "tox",
-    "genbadge[coverage]",
-]
-doc = [
-    "furo",
-    "myst-parser",
-    "sphinx>=5",
-    "sphinx-copybutton",
-]
-
-[tool.hatch.version]
-path = "src/Rankchem/__init__.py"
-version = "1.1.1"
-
-[tool.pytest.ini_options]
-testpaths = [
-    "tests",
-]
-
-[tool.coverage.run]
-omit = [
-    '__init__.py'
-]
-
-[tool.coverage.report]
-exclude_also = [
-    "if __name__ == .__main__.:",
-]
+[build-system] 
+requires = ["hatchling"]
+build-backend = "hatchling.build"
+
+[tool.hatch.build.targets.wheel]
+packages = ["src/Rankchem/for_streamlit/__init__.py"]
+
+[project]
+name = "RankChem"
+readme = "README.md"
+requires-python = ">=3.8"
+license = {file = "LICENSE"}
+description = "RankChem project"
+dependencies = [
+     "rdkit",
+     "morfeus-ml",
+     "pyvistaqt",
+     "numpy",
+     "py3Dmol",
+     "streamlit",
+     "stmol"
+]
+
+
+authors = [
+    {name = "Emma Kappeler", email = "emma.kappeler@epfl.ch"},
+    {name = "Ludovica Fracassi", email = "ludovica.fracassi@epfl.ch"}
+]
+classifiers = [
+    "Development Status :: 3 - Alpha",
+    "Intended Audience :: Developers",
+    "License :: OSI Approved :: MIT License",
+    "Operating System :: OS Independent",
+    "Programming Language :: Python",
+    "Programming Language :: Python :: 3",
+    "Programming Language :: Python :: 3.8",
+    "Programming Language :: Python :: 3.9",
+    "Programming Language :: Python :: 3.10",
+    "Programming Language :: Python :: 3.11",
+]
+dynamic = ["version"]
+
+[project.urls]
+source = "https://github.com/kappelemma/RankChem"
+tracker = "https://github.com/kappelemma/RankChem/issues"
+
+[project.optional-dependencies]
+test = [
+    "hypothesis",
+    "pytest",
+    "pytest-cov",
+    "tox",
+    "genbadge[coverage]",
+]
+doc = [
+    "furo",
+    "myst-parser",
+    "sphinx>=5",
+    "sphinx-copybutton",
+]
+
+[tool.hatch.version]
+path = "src/Rankchem/for_streamlit/__init__.py"
+
+[tool.pytest.ini_options]
+testpaths = [
+    "tests",
+]
+
+[tool.coverage.run]
+omit = [
+    '__init__.py'
+]
+
+[tool.coverage.report]
+exclude_also = [
+    "if __name__ == .__main__.:",
+]
```

### Comparing `rankchem-1.1.1/src/RankChem.egg-info/PKG-INFO` & `rankchem-1.1.2/src/RankChem.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: RankChem
-Version: 1.1.1
+Version: 1.1.2
 Summary: RankChem project
 Home-page: https://github.com/kappelemma/RankChem
 Author: Emma Kappeler, Ludovica Fracassi
 Author-email: Emma Kappeler <emma.kappeler@epfl.ch>, Ludovica Fracassi <ludovica.fracassi@epfl.ch>
 License: MIT License
         
         Copyright (c) 2024 by Emma Kappeler <emma.kappeler@epfl.ch>,
@@ -98,15 +98,15 @@
 ```
 Where myenv is the name of your environment.
 
 The package runs on python 3.10 but supports python 3.8 through 3.10.
 RankChem can be installed using pip as followed:
 
 ```bash
-pip install Rankchem
+pip install RankChem
 ```
 
 The package can also be installed from source by running the following commands:
 
 First, clone the repository from Github and go in the RankChem folder.
 
 ```bash
```

### Comparing `rankchem-1.1.1/tests/test_average.py` & `rankchem-1.1.2/tests/test_average.py`

 * *Files identical despite different names*

### Comparing `rankchem-1.1.1/tests/test_calculate_descriptor.py` & `rankchem-1.1.2/tests/test_calculate_descriptor.py`

 * *Files identical despite different names*

### Comparing `rankchem-1.1.1/tests/test_calculate_fukui.py` & `rankchem-1.1.2/tests/test_calculate_fukui.py`

 * *Files identical despite different names*

### Comparing `rankchem-1.1.1/tests/test_rank_descriptors.py` & `rankchem-1.1.2/tests/test_rank_descriptors.py`

 * *Files identical despite different names*

### Comparing `rankchem-1.1.1/tests/test_smiles_to_xyz.py` & `rankchem-1.1.2/tests/test_smiles_to_xyz.py`

 * *Files identical despite different names*

