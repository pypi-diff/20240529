# Comparing `tmp/rankchem-1.1.3.tar.gz` & `tmp/rankchem-1.1.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "rankchem-1.1.3.tar", last modified: Wed May 29 17:27:12 2024, max compression
+gzip compressed data, was "rankchem-1.1.4.tar", last modified: Wed May 29 18:19:11 2024, max compression
```

## Comparing `rankchem-1.1.3.tar` & `rankchem-1.1.4.tar`

### file list

```diff
@@ -1,22 +1,26 @@
-drwxrwxrwx   0 emmaunix  (1000) emmaunix  (1000)        0 2024-05-29 17:27:12.541951 rankchem-1.1.3/
--rwxrwxrwx   0 emmaunix  (1000) emmaunix  (1000)     1164 2024-05-17 18:59:58.000000 rankchem-1.1.3/LICENSE
--rwxrwxrwx   0 emmaunix  (1000) emmaunix  (1000)    10447 2024-05-29 17:27:12.519823 rankchem-1.1.3/PKG-INFO
--rwxrwxrwx   0 emmaunix  (1000) emmaunix  (1000)     7698 2024-05-29 16:47:22.000000 rankchem-1.1.3/README.md
--rwxrwxrwx   0 emmaunix  (1000) emmaunix  (1000)     1719 2024-05-29 16:47:22.000000 rankchem-1.1.3/pyproject.toml
--rwxrwxrwx   0 emmaunix  (1000) emmaunix  (1000)       38 2024-05-29 17:27:12.544488 rankchem-1.1.3/setup.cfg
--rwxrwxrwx   0 emmaunix  (1000) emmaunix  (1000)     1289 2024-05-29 17:26:23.000000 rankchem-1.1.3/setup.py
-drwxrwxrwx   0 emmaunix  (1000) emmaunix  (1000)        0 2024-05-29 17:27:11.530072 rankchem-1.1.3/src/
-drwxrwxrwx   0 emmaunix  (1000) emmaunix  (1000)        0 2024-05-29 17:27:12.489808 rankchem-1.1.3/src/RankChem.egg-info/
--rwxrwxrwx   0 emmaunix  (1000) emmaunix  (1000)    10447 2024-05-29 17:27:11.000000 rankchem-1.1.3/src/RankChem.egg-info/PKG-INFO
--rwxrwxrwx   0 emmaunix  (1000) emmaunix  (1000)      431 2024-05-29 17:27:11.000000 rankchem-1.1.3/src/RankChem.egg-info/SOURCES.txt
--rwxrwxrwx   0 emmaunix  (1000) emmaunix  (1000)        1 2024-05-29 17:27:11.000000 rankchem-1.1.3/src/RankChem.egg-info/dependency_links.txt
--rwxrwxrwx   0 emmaunix  (1000) emmaunix  (1000)      169 2024-05-29 17:27:11.000000 rankchem-1.1.3/src/RankChem.egg-info/requires.txt
--rwxrwxrwx   0 emmaunix  (1000) emmaunix  (1000)        1 2024-05-29 17:27:11.000000 rankchem-1.1.3/src/RankChem.egg-info/top_level.txt
-drwxrwxrwx   0 emmaunix  (1000) emmaunix  (1000)        0 2024-05-29 17:27:12.401814 rankchem-1.1.3/tests/
--rwxrwxrwx   0 emmaunix  (1000) emmaunix  (1000)      608 2024-05-26 13:57:31.000000 rankchem-1.1.3/tests/test_average.py
--rwxrwxrwx   0 emmaunix  (1000) emmaunix  (1000)      592 2024-05-26 13:58:59.000000 rankchem-1.1.3/tests/test_calculate_descriptor.py
--rwxrwxrwx   0 emmaunix  (1000) emmaunix  (1000)      749 2024-05-26 12:24:41.000000 rankchem-1.1.3/tests/test_calculate_fukui.py
--rwxrwxrwx   0 emmaunix  (1000) emmaunix  (1000)      483 2024-05-26 12:24:41.000000 rankchem-1.1.3/tests/test_get_max_fukui_avg.py
--rwxrwxrwx   0 emmaunix  (1000) emmaunix  (1000)      665 2024-05-26 14:00:42.000000 rankchem-1.1.3/tests/test_rank_descriptors.py
--rwxrwxrwx   0 emmaunix  (1000) emmaunix  (1000)      617 2024-05-26 12:24:41.000000 rankchem-1.1.3/tests/test_smiles_to_xyz.py
--rwxrwxrwx   0 emmaunix  (1000) emmaunix  (1000)      409 2024-05-26 13:57:17.000000 rankchem-1.1.3/tests/test_visualize_molecule.py
+drwxrwxrwx   0 emmaunix  (1000) emmaunix  (1000)        0 2024-05-29 18:19:11.764485 rankchem-1.1.4/
+-rwxrwxrwx   0 emmaunix  (1000) emmaunix  (1000)     1164 2024-05-17 18:59:58.000000 rankchem-1.1.4/LICENSE
+-rwxrwxrwx   0 emmaunix  (1000) emmaunix  (1000)    10192 2024-05-29 18:19:11.755847 rankchem-1.1.4/PKG-INFO
+-rwxrwxrwx   0 emmaunix  (1000) emmaunix  (1000)     7698 2024-05-29 16:47:22.000000 rankchem-1.1.4/README.md
+-rwxrwxrwx   0 emmaunix  (1000) emmaunix  (1000)     1282 2024-05-29 17:59:34.000000 rankchem-1.1.4/pyproject.toml
+-rwxrwxrwx   0 emmaunix  (1000) emmaunix  (1000)       38 2024-05-29 18:19:11.766672 rankchem-1.1.4/setup.cfg
+-rwxrwxrwx   0 emmaunix  (1000) emmaunix  (1000)     1289 2024-05-29 18:17:55.000000 rankchem-1.1.4/setup.py
+drwxrwxrwx   0 emmaunix  (1000) emmaunix  (1000)        0 2024-05-29 18:19:11.273246 rankchem-1.1.4/src/
+drwxrwxrwx   0 emmaunix  (1000) emmaunix  (1000)        0 2024-05-29 18:19:11.742397 rankchem-1.1.4/src/RankChem.egg-info/
+-rwxrwxrwx   0 emmaunix  (1000) emmaunix  (1000)    10192 2024-05-29 18:19:11.000000 rankchem-1.1.4/src/RankChem.egg-info/PKG-INFO
+-rwxrwxrwx   0 emmaunix  (1000) emmaunix  (1000)      509 2024-05-29 18:19:11.000000 rankchem-1.1.4/src/RankChem.egg-info/SOURCES.txt
+-rwxrwxrwx   0 emmaunix  (1000) emmaunix  (1000)        1 2024-05-29 18:19:11.000000 rankchem-1.1.4/src/RankChem.egg-info/dependency_links.txt
+-rwxrwxrwx   0 emmaunix  (1000) emmaunix  (1000)      117 2024-05-29 18:19:11.000000 rankchem-1.1.4/src/RankChem.egg-info/requires.txt
+-rwxrwxrwx   0 emmaunix  (1000) emmaunix  (1000)        9 2024-05-29 18:19:11.000000 rankchem-1.1.4/src/RankChem.egg-info/top_level.txt
+drwxrwxrwx   0 emmaunix  (1000) emmaunix  (1000)        0 2024-05-29 18:19:11.521155 rankchem-1.1.4/src/Rankchem/
+-rwxrwxrwx   0 emmaunix  (1000) emmaunix  (1000)     6736 2024-05-29 18:17:55.000000 rankchem-1.1.4/src/Rankchem/Highlighting.py
+-rwxrwxrwx   0 emmaunix  (1000) emmaunix  (1000)     4235 2024-05-29 18:17:55.000000 rankchem-1.1.4/src/Rankchem/Ranking.py
+-rwxrwxrwx   0 emmaunix  (1000) emmaunix  (1000)       86 2024-05-29 18:17:55.000000 rankchem-1.1.4/src/Rankchem/__init__.py
+drwxrwxrwx   0 emmaunix  (1000) emmaunix  (1000)        0 2024-05-29 18:19:11.708123 rankchem-1.1.4/tests/
+-rwxrwxrwx   0 emmaunix  (1000) emmaunix  (1000)      608 2024-05-26 13:57:31.000000 rankchem-1.1.4/tests/test_average.py
+-rwxrwxrwx   0 emmaunix  (1000) emmaunix  (1000)      592 2024-05-26 13:58:59.000000 rankchem-1.1.4/tests/test_calculate_descriptor.py
+-rwxrwxrwx   0 emmaunix  (1000) emmaunix  (1000)      749 2024-05-26 12:24:41.000000 rankchem-1.1.4/tests/test_calculate_fukui.py
+-rwxrwxrwx   0 emmaunix  (1000) emmaunix  (1000)      483 2024-05-26 12:24:41.000000 rankchem-1.1.4/tests/test_get_max_fukui_avg.py
+-rwxrwxrwx   0 emmaunix  (1000) emmaunix  (1000)      665 2024-05-26 14:00:42.000000 rankchem-1.1.4/tests/test_rank_descriptors.py
+-rwxrwxrwx   0 emmaunix  (1000) emmaunix  (1000)      617 2024-05-26 12:24:41.000000 rankchem-1.1.4/tests/test_smiles_to_xyz.py
+-rwxrwxrwx   0 emmaunix  (1000) emmaunix  (1000)      409 2024-05-26 13:57:17.000000 rankchem-1.1.4/tests/test_visualize_molecule.py
```

### Comparing `rankchem-1.1.3/LICENSE` & `rankchem-1.1.4/LICENSE`

 * *Files identical despite different names*

### Comparing `rankchem-1.1.3/PKG-INFO` & `rankchem-1.1.4/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: RankChem
-Version: 1.1.3
+Version: 1.1.4
 Summary: RankChem project
 Home-page: https://github.com/kappelemma/RankChem
 Author: Emma Kappeler, Ludovica Fracassi
 Author-email: Emma Kappeler <emma.kappeler@epfl.ch>, Ludovica Fracassi <ludovica.fracassi@epfl.ch>
 License: MIT License
         
         Copyright (c) 2024 by Emma Kappeler <emma.kappeler@epfl.ch>,
@@ -24,16 +24,15 @@
         IMPLIED, INCLUDING BUT NOT LIMITED TO THE WARRANTIES OF MERCHANTABILITY,
         FITNESS FOR A PARTICULAR PURPOSE AND NONINFRINGEMENT. IN NO EVENT SHALL THE
         AUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER
         LIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING FROM,
         OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN THE
         SOFTWARE.
         
-Project-URL: source, https://github.com/kappelemma/RankChem
-Project-URL: tracker, https://github.com/kappelemma/RankChem/issues
+Project-URL: Homepage, https://github.com/kappelemma/RankChem
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.8
@@ -52,19 +51,14 @@
 Requires-Dist: stmol
 Provides-Extra: test
 Requires-Dist: hypothesis; extra == "test"
 Requires-Dist: pytest; extra == "test"
 Requires-Dist: pytest-cov; extra == "test"
 Requires-Dist: tox; extra == "test"
 Requires-Dist: genbadge[coverage]; extra == "test"
-Provides-Extra: doc
-Requires-Dist: furo; extra == "doc"
-Requires-Dist: myst-parser; extra == "doc"
-Requires-Dist: sphinx>=5; extra == "doc"
-Requires-Dist: sphinx-copybutton; extra == "doc"
 
 ![project logo](assets/nkChem.png)
 
 # ChemInterface for Reactivity Analysis
 ### Project in the *Practical programming in chemistry* course EPFL CH-200
 [![python](https://img.shields.io/badge/Python-14354C?style=for-the-badge&logo=python&logoColor=white)](https://www.python.org)
 ![GitHub](https://img.shields.io/badge/github-%23121011.svg?style=for-the-badge&logo=github&logoColor=white)
```

### Comparing `rankchem-1.1.3/README.md` & `rankchem-1.1.4/README.md`

 * *Files identical despite different names*

### Comparing `rankchem-1.1.3/pyproject.toml` & `rankchem-1.1.4/pyproject.toml`

 * *Files 21% similar despite different names*

```diff
@@ -1,78 +1,56 @@
 [build-system] 
 requires = ["hatchling"]
 build-backend = "hatchling.build"
 
-[tool.hatch.build.targets.wheel]
-packages = ["src/Rankchem/for_streamlit/__init__.py"]
+
+[tool.hatchling.build.targets.wheel]
+packages = ["src/RankChem"]
+
 
 [project]
 name = "RankChem"
+version = "1.1.4"
 readme = "README.md"
 requires-python = ">=3.8"
 license = {file = "LICENSE"}
 description = "RankChem project"
 dependencies = [
      "rdkit",
      "morfeus-ml",
      "pyvistaqt",
      "numpy",
      "py3Dmol",
      "streamlit",
      "stmol"
 ]
 
-
 authors = [
     {name = "Emma Kappeler", email = "emma.kappeler@epfl.ch"},
     {name = "Ludovica Fracassi", email = "ludovica.fracassi@epfl.ch"}
 ]
+
 classifiers = [
     "Development Status :: 3 - Alpha",
     "Intended Audience :: Developers",
     "License :: OSI Approved :: MIT License",
     "Operating System :: OS Independent",
     "Programming Language :: Python",
     "Programming Language :: Python :: 3",
     "Programming Language :: Python :: 3.8",
     "Programming Language :: Python :: 3.9",
     "Programming Language :: Python :: 3.10",
     "Programming Language :: Python :: 3.11",
 ]
-dynamic = ["version"]
+
 
 [project.urls]
-source = "https://github.com/kappelemma/RankChem"
-tracker = "https://github.com/kappelemma/RankChem/issues"
+Homepage = "https://github.com/kappelemma/RankChem"
 
 [project.optional-dependencies]
 test = [
     "hypothesis",
     "pytest",
     "pytest-cov",
     "tox",
     "genbadge[coverage]",
 ]
-doc = [
-    "furo",
-    "myst-parser",
-    "sphinx>=5",
-    "sphinx-copybutton",
-]
-
-[tool.hatch.version]
-path = "src/Rankchem/for_streamlit/__init__.py"
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
```

### Comparing `rankchem-1.1.3/setup.py` & `rankchem-1.1.4/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 from setuptools import setup, find_packages
 
 with open('README.md', 'r', encoding='utf-8') as fh:
     long_description = fh.read()
 
 setup(
     name='rankchem',
-    version='1.1.3',
+    version='1.1.4',
     packages=find_packages(where='src'),
     package_dir={'': 'src'},
     install_requires=[
         'rdkit',
         'morfeus-ml',
         'pyvistaqt',
         'numpy',
```

### Comparing `rankchem-1.1.3/src/RankChem.egg-info/PKG-INFO` & `rankchem-1.1.4/src/RankChem.egg-info/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: RankChem
-Version: 1.1.3
+Version: 1.1.4
 Summary: RankChem project
 Home-page: https://github.com/kappelemma/RankChem
 Author: Emma Kappeler, Ludovica Fracassi
 Author-email: Emma Kappeler <emma.kappeler@epfl.ch>, Ludovica Fracassi <ludovica.fracassi@epfl.ch>
 License: MIT License
         
         Copyright (c) 2024 by Emma Kappeler <emma.kappeler@epfl.ch>,
@@ -24,16 +24,15 @@
         IMPLIED, INCLUDING BUT NOT LIMITED TO THE WARRANTIES OF MERCHANTABILITY,
         FITNESS FOR A PARTICULAR PURPOSE AND NONINFRINGEMENT. IN NO EVENT SHALL THE
         AUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER
         LIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING FROM,
         OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN THE
         SOFTWARE.
         
-Project-URL: source, https://github.com/kappelemma/RankChem
-Project-URL: tracker, https://github.com/kappelemma/RankChem/issues
+Project-URL: Homepage, https://github.com/kappelemma/RankChem
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.8
@@ -52,19 +51,14 @@
 Requires-Dist: stmol
 Provides-Extra: test
 Requires-Dist: hypothesis; extra == "test"
 Requires-Dist: pytest; extra == "test"
 Requires-Dist: pytest-cov; extra == "test"
 Requires-Dist: tox; extra == "test"
 Requires-Dist: genbadge[coverage]; extra == "test"
-Provides-Extra: doc
-Requires-Dist: furo; extra == "doc"
-Requires-Dist: myst-parser; extra == "doc"
-Requires-Dist: sphinx>=5; extra == "doc"
-Requires-Dist: sphinx-copybutton; extra == "doc"
 
 ![project logo](assets/nkChem.png)
 
 # ChemInterface for Reactivity Analysis
 ### Project in the *Practical programming in chemistry* course EPFL CH-200
 [![python](https://img.shields.io/badge/Python-14354C?style=for-the-badge&logo=python&logoColor=white)](https://www.python.org)
 ![GitHub](https://img.shields.io/badge/github-%23121011.svg?style=for-the-badge&logo=github&logoColor=white)
```

### Comparing `rankchem-1.1.3/tests/test_average.py` & `rankchem-1.1.4/tests/test_average.py`

 * *Files identical despite different names*

### Comparing `rankchem-1.1.3/tests/test_calculate_descriptor.py` & `rankchem-1.1.4/tests/test_calculate_descriptor.py`

 * *Files identical despite different names*

### Comparing `rankchem-1.1.3/tests/test_calculate_fukui.py` & `rankchem-1.1.4/tests/test_calculate_fukui.py`

 * *Files identical despite different names*

### Comparing `rankchem-1.1.3/tests/test_rank_descriptors.py` & `rankchem-1.1.4/tests/test_rank_descriptors.py`

 * *Files identical despite different names*

### Comparing `rankchem-1.1.3/tests/test_smiles_to_xyz.py` & `rankchem-1.1.4/tests/test_smiles_to_xyz.py`

 * *Files identical despite different names*

