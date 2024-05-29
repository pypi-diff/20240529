# Comparing `tmp/rankchem-1.1.4.tar.gz` & `tmp/rankchem-1.1.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "rankchem-1.1.4.tar", last modified: Wed May 29 18:19:11 2024, max compression
+gzip compressed data, was "rankchem-1.1.5.tar", last modified: Wed May 29 18:35:43 2024, max compression
```

## Comparing `rankchem-1.1.4.tar` & `rankchem-1.1.5.tar`

### file list

```diff
@@ -1,26 +1,26 @@
-drwxrwxrwx   0 emmaunix  (1000) emmaunix  (1000)        0 2024-05-29 18:19:11.764485 rankchem-1.1.4/
--rwxrwxrwx   0 emmaunix  (1000) emmaunix  (1000)     1164 2024-05-17 18:59:58.000000 rankchem-1.1.4/LICENSE
--rwxrwxrwx   0 emmaunix  (1000) emmaunix  (1000)    10192 2024-05-29 18:19:11.755847 rankchem-1.1.4/PKG-INFO
--rwxrwxrwx   0 emmaunix  (1000) emmaunix  (1000)     7698 2024-05-29 16:47:22.000000 rankchem-1.1.4/README.md
--rwxrwxrwx   0 emmaunix  (1000) emmaunix  (1000)     1282 2024-05-29 17:59:34.000000 rankchem-1.1.4/pyproject.toml
--rwxrwxrwx   0 emmaunix  (1000) emmaunix  (1000)       38 2024-05-29 18:19:11.766672 rankchem-1.1.4/setup.cfg
--rwxrwxrwx   0 emmaunix  (1000) emmaunix  (1000)     1289 2024-05-29 18:17:55.000000 rankchem-1.1.4/setup.py
-drwxrwxrwx   0 emmaunix  (1000) emmaunix  (1000)        0 2024-05-29 18:19:11.273246 rankchem-1.1.4/src/
-drwxrwxrwx   0 emmaunix  (1000) emmaunix  (1000)        0 2024-05-29 18:19:11.742397 rankchem-1.1.4/src/RankChem.egg-info/
--rwxrwxrwx   0 emmaunix  (1000) emmaunix  (1000)    10192 2024-05-29 18:19:11.000000 rankchem-1.1.4/src/RankChem.egg-info/PKG-INFO
--rwxrwxrwx   0 emmaunix  (1000) emmaunix  (1000)      509 2024-05-29 18:19:11.000000 rankchem-1.1.4/src/RankChem.egg-info/SOURCES.txt
--rwxrwxrwx   0 emmaunix  (1000) emmaunix  (1000)        1 2024-05-29 18:19:11.000000 rankchem-1.1.4/src/RankChem.egg-info/dependency_links.txt
--rwxrwxrwx   0 emmaunix  (1000) emmaunix  (1000)      117 2024-05-29 18:19:11.000000 rankchem-1.1.4/src/RankChem.egg-info/requires.txt
--rwxrwxrwx   0 emmaunix  (1000) emmaunix  (1000)        9 2024-05-29 18:19:11.000000 rankchem-1.1.4/src/RankChem.egg-info/top_level.txt
-drwxrwxrwx   0 emmaunix  (1000) emmaunix  (1000)        0 2024-05-29 18:19:11.521155 rankchem-1.1.4/src/Rankchem/
--rwxrwxrwx   0 emmaunix  (1000) emmaunix  (1000)     6736 2024-05-29 18:17:55.000000 rankchem-1.1.4/src/Rankchem/Highlighting.py
--rwxrwxrwx   0 emmaunix  (1000) emmaunix  (1000)     4235 2024-05-29 18:17:55.000000 rankchem-1.1.4/src/Rankchem/Ranking.py
--rwxrwxrwx   0 emmaunix  (1000) emmaunix  (1000)       86 2024-05-29 18:17:55.000000 rankchem-1.1.4/src/Rankchem/__init__.py
-drwxrwxrwx   0 emmaunix  (1000) emmaunix  (1000)        0 2024-05-29 18:19:11.708123 rankchem-1.1.4/tests/
--rwxrwxrwx   0 emmaunix  (1000) emmaunix  (1000)      608 2024-05-26 13:57:31.000000 rankchem-1.1.4/tests/test_average.py
--rwxrwxrwx   0 emmaunix  (1000) emmaunix  (1000)      592 2024-05-26 13:58:59.000000 rankchem-1.1.4/tests/test_calculate_descriptor.py
--rwxrwxrwx   0 emmaunix  (1000) emmaunix  (1000)      749 2024-05-26 12:24:41.000000 rankchem-1.1.4/tests/test_calculate_fukui.py
--rwxrwxrwx   0 emmaunix  (1000) emmaunix  (1000)      483 2024-05-26 12:24:41.000000 rankchem-1.1.4/tests/test_get_max_fukui_avg.py
--rwxrwxrwx   0 emmaunix  (1000) emmaunix  (1000)      665 2024-05-26 14:00:42.000000 rankchem-1.1.4/tests/test_rank_descriptors.py
--rwxrwxrwx   0 emmaunix  (1000) emmaunix  (1000)      617 2024-05-26 12:24:41.000000 rankchem-1.1.4/tests/test_smiles_to_xyz.py
--rwxrwxrwx   0 emmaunix  (1000) emmaunix  (1000)      409 2024-05-26 13:57:17.000000 rankchem-1.1.4/tests/test_visualize_molecule.py
+drwxrwxrwx   0 emmaunix  (1000) emmaunix  (1000)        0 2024-05-29 18:35:43.375749 rankchem-1.1.5/
+-rwxrwxrwx   0 emmaunix  (1000) emmaunix  (1000)     1164 2024-05-17 18:59:58.000000 rankchem-1.1.5/LICENSE
+-rwxrwxrwx   0 emmaunix  (1000) emmaunix  (1000)    10190 2024-05-29 18:35:43.352419 rankchem-1.1.5/PKG-INFO
+-rwxrwxrwx   0 emmaunix  (1000) emmaunix  (1000)     7698 2024-05-29 16:47:22.000000 rankchem-1.1.5/README.md
+-rwxrwxrwx   0 emmaunix  (1000) emmaunix  (1000)     1281 2024-05-29 18:34:46.000000 rankchem-1.1.5/pyproject.toml
+-rwxrwxrwx   0 emmaunix  (1000) emmaunix  (1000)       38 2024-05-29 18:35:43.376742 rankchem-1.1.5/setup.cfg
+-rwxrwxrwx   0 emmaunix  (1000) emmaunix  (1000)     1288 2024-05-29 18:34:46.000000 rankchem-1.1.5/setup.py
+drwxrwxrwx   0 emmaunix  (1000) emmaunix  (1000)        0 2024-05-29 18:35:42.214254 rankchem-1.1.5/src/
+drwxrwxrwx   0 emmaunix  (1000) emmaunix  (1000)        0 2024-05-29 18:35:43.323852 rankchem-1.1.5/src/RankChem.egg-info/
+-rwxrwxrwx   0 emmaunix  (1000) emmaunix  (1000)    10190 2024-05-29 18:35:41.000000 rankchem-1.1.5/src/RankChem.egg-info/PKG-INFO
+-rwxrwxrwx   0 emmaunix  (1000) emmaunix  (1000)      509 2024-05-29 18:35:42.000000 rankchem-1.1.5/src/RankChem.egg-info/SOURCES.txt
+-rwxrwxrwx   0 emmaunix  (1000) emmaunix  (1000)        1 2024-05-29 18:35:41.000000 rankchem-1.1.5/src/RankChem.egg-info/dependency_links.txt
+-rwxrwxrwx   0 emmaunix  (1000) emmaunix  (1000)      117 2024-05-29 18:35:41.000000 rankchem-1.1.5/src/RankChem.egg-info/requires.txt
+-rwxrwxrwx   0 emmaunix  (1000) emmaunix  (1000)        9 2024-05-29 18:35:41.000000 rankchem-1.1.5/src/RankChem.egg-info/top_level.txt
+drwxrwxrwx   0 emmaunix  (1000) emmaunix  (1000)        0 2024-05-29 18:35:42.894661 rankchem-1.1.5/src/Rankchem/
+-rwxrwxrwx   0 emmaunix  (1000) emmaunix  (1000)     6736 2024-05-29 18:17:55.000000 rankchem-1.1.5/src/Rankchem/Highlighting.py
+-rwxrwxrwx   0 emmaunix  (1000) emmaunix  (1000)     4235 2024-05-29 18:17:55.000000 rankchem-1.1.5/src/Rankchem/Ranking.py
+-rwxrwxrwx   0 emmaunix  (1000) emmaunix  (1000)       86 2024-05-29 18:34:46.000000 rankchem-1.1.5/src/Rankchem/__init__.py
+drwxrwxrwx   0 emmaunix  (1000) emmaunix  (1000)        0 2024-05-29 18:35:43.245776 rankchem-1.1.5/tests/
+-rwxrwxrwx   0 emmaunix  (1000) emmaunix  (1000)      594 2024-05-29 18:25:32.000000 rankchem-1.1.5/tests/test_average.py
+-rwxrwxrwx   0 emmaunix  (1000) emmaunix  (1000)      578 2024-05-29 18:26:22.000000 rankchem-1.1.5/tests/test_calculate_descriptor.py
+-rwxrwxrwx   0 emmaunix  (1000) emmaunix  (1000)      735 2024-05-29 18:26:20.000000 rankchem-1.1.5/tests/test_calculate_fukui.py
+-rwxrwxrwx   0 emmaunix  (1000) emmaunix  (1000)      469 2024-05-29 18:25:41.000000 rankchem-1.1.5/tests/test_get_max_fukui_avg.py
+-rwxrwxrwx   0 emmaunix  (1000) emmaunix  (1000)      651 2024-05-29 18:25:39.000000 rankchem-1.1.5/tests/test_rank_descriptors.py
+-rwxrwxrwx   0 emmaunix  (1000) emmaunix  (1000)      603 2024-05-29 18:25:38.000000 rankchem-1.1.5/tests/test_smiles_to_xyz.py
+-rwxrwxrwx   0 emmaunix  (1000) emmaunix  (1000)      395 2024-05-29 18:25:36.000000 rankchem-1.1.5/tests/test_visualize_molecule.py
```

### Comparing `rankchem-1.1.4/LICENSE` & `rankchem-1.1.5/LICENSE`

 * *Files identical despite different names*

### Comparing `rankchem-1.1.4/PKG-INFO` & `rankchem-1.1.5/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 Metadata-Version: 2.1
 Name: RankChem
-Version: 1.1.4
+Version: 1.1.5
 Summary: RankChem project
-Home-page: https://github.com/kappelemma/RankChem
+Home-page: https://github.com/fracaludo/RankChem
 Author: Emma Kappeler, Ludovica Fracassi
 Author-email: Emma Kappeler <emma.kappeler@epfl.ch>, Ludovica Fracassi <ludovica.fracassi@epfl.ch>
 License: MIT License
         
         Copyright (c) 2024 by Emma Kappeler <emma.kappeler@epfl.ch>,
                             Ludovica Fracassi <ludovica.fracassi@epfl.ch>
         
@@ -24,15 +24,15 @@
         IMPLIED, INCLUDING BUT NOT LIMITED TO THE WARRANTIES OF MERCHANTABILITY,
         FITNESS FOR A PARTICULAR PURPOSE AND NONINFRINGEMENT. IN NO EVENT SHALL THE
         AUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER
         LIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING FROM,
         OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN THE
         SOFTWARE.
         
-Project-URL: Homepage, https://github.com/kappelemma/RankChem
+Project-URL: Homepage, https://github.com/fracaludo/RankChem
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.8
```

### Comparing `rankchem-1.1.4/README.md` & `rankchem-1.1.5/README.md`

 * *Files identical despite different names*

### Comparing `rankchem-1.1.4/pyproject.toml` & `rankchem-1.1.5/pyproject.toml`

 * *Files 6% similar despite different names*

```diff
@@ -1,19 +1,19 @@
 [build-system] 
 requires = ["hatchling"]
 build-backend = "hatchling.build"
 
 
 [tool.hatchling.build.targets.wheel]
-packages = ["src/RankChem"]
+packages = ["src/Rankchem"]
 
 
 [project]
 name = "RankChem"
-version = "1.1.4"
+version = "1.1.5"
 readme = "README.md"
 requires-python = ">=3.8"
 license = {file = "LICENSE"}
 description = "RankChem project"
 dependencies = [
      "rdkit",
      "morfeus-ml",
@@ -40,15 +40,15 @@
     "Programming Language :: Python :: 3.9",
     "Programming Language :: Python :: 3.10",
     "Programming Language :: Python :: 3.11",
 ]
 
 
 [project.urls]
-Homepage = "https://github.com/kappelemma/RankChem"
+Homepage = "https://github.com/fracaludo/RankChem"
 
 [project.optional-dependencies]
 test = [
     "hypothesis",
     "pytest",
     "pytest-cov",
     "tox",
```

### Comparing `rankchem-1.1.4/setup.py` & `rankchem-1.1.5/setup.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 from setuptools import setup, find_packages
 
 with open('README.md', 'r', encoding='utf-8') as fh:
     long_description = fh.read()
 
 setup(
     name='rankchem',
-    version='1.1.4',
+    version='1.1.5',
     packages=find_packages(where='src'),
     package_dir={'': 'src'},
     install_requires=[
         'rdkit',
         'morfeus-ml',
         'pyvistaqt',
         'numpy',
@@ -19,15 +19,15 @@
     ],
     python_requires='>=3.8',
     author='Emma Kappeler, Ludovica Fracassi',
     author_email='emma.kappeler@epfl.ch,ludovica.fracassi@epfl.ch',
     description='RankChem project',
     long_description=long_description,
     long_description_content_type='text/markdown',
-    url='https://github.com/kappelemma/RankChem',
+    url='https://github.com/fracaludo/RankChem',
     classifiers=[
         'Development Status :: 3 - Alpha',
         'Intended Audience :: Developers',
         'License :: OSI Approved :: MIT License',
         'Operating System :: OS Independent',
         'Programming Language :: Python',
         'Programming Language :: Python :: 3',
```

### Comparing `rankchem-1.1.4/src/RankChem.egg-info/PKG-INFO` & `rankchem-1.1.5/src/RankChem.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 Metadata-Version: 2.1
 Name: RankChem
-Version: 1.1.4
+Version: 1.1.5
 Summary: RankChem project
-Home-page: https://github.com/kappelemma/RankChem
+Home-page: https://github.com/fracaludo/RankChem
 Author: Emma Kappeler, Ludovica Fracassi
 Author-email: Emma Kappeler <emma.kappeler@epfl.ch>, Ludovica Fracassi <ludovica.fracassi@epfl.ch>
 License: MIT License
         
         Copyright (c) 2024 by Emma Kappeler <emma.kappeler@epfl.ch>,
                             Ludovica Fracassi <ludovica.fracassi@epfl.ch>
         
@@ -24,15 +24,15 @@
         IMPLIED, INCLUDING BUT NOT LIMITED TO THE WARRANTIES OF MERCHANTABILITY,
         FITNESS FOR A PARTICULAR PURPOSE AND NONINFRINGEMENT. IN NO EVENT SHALL THE
         AUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER
         LIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING FROM,
         OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN THE
         SOFTWARE.
         
-Project-URL: Homepage, https://github.com/kappelemma/RankChem
+Project-URL: Homepage, https://github.com/fracaludo/RankChem
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.8
```

### Comparing `rankchem-1.1.4/src/Rankchem/Highlighting.py` & `rankchem-1.1.5/src/Rankchem/Highlighting.py`

 * *Files identical despite different names*

### Comparing `rankchem-1.1.4/src/Rankchem/Ranking.py` & `rankchem-1.1.5/src/Rankchem/Ranking.py`

 * *Files identical despite different names*

### Comparing `rankchem-1.1.4/tests/test_average.py` & `rankchem-1.1.5/tests/test_average.py`

 * *Files 24% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 import sys
 import os
 import pytest
 
 sys.path.insert(0, os.path.abspath(os.path.join(os.path.dirname(__file__), '..', 'src')))
 
-from Rankchem.for_streamlit.Highlighting import average
+from Rankchem.Highlighting import average
 
 def test_average():
     fukui_dicts = [{0: 0.1, 1: 0.2}, {0: 0.2, 1: 0.1}]
     avg_fukui = average(fukui_dicts)
     assert isinstance(avg_fukui, dict), "Test failed: Result is not a dictionary"
     assert avg_fukui[0] == pytest.approx(0.15, rel=1e-9), "Test failed: Incorrect average value for atom 0"
     assert avg_fukui[1] == pytest.approx(0.15, rel=1e-9), "Test failed: Incorrect average value for atom 1"
```

### Comparing `rankchem-1.1.4/tests/test_calculate_descriptor.py` & `rankchem-1.1.5/tests/test_calculate_descriptor.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 import sys
 import os
 import pytest
 
 sys.path.insert(0, os.path.abspath(os.path.join(os.path.dirname(__file__), '..', 'src')))
 
-from Rankchem.for_streamlit.Ranking import calculate_descriptor
+from Rankchem.Ranking import calculate_descriptor
 
 def test_calculate_descriptor():
     smiles_list = ["CC=O", "CC(=O)C"]
     descriptor_type = "N"
     iterations = 10
     descriptors = calculate_descriptor(smiles_list, descriptor_type, iterations)
     assert isinstance(descriptors, list), "Test failed: Result is not a list"
```

### Comparing `rankchem-1.1.4/tests/test_calculate_fukui.py` & `rankchem-1.1.5/tests/test_calculate_fukui.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 import sys
 import os
 import pytest
 
 sys.path.insert(0, os.path.abspath(os.path.join(os.path.dirname(__file__), '..', 'src')))
 
-from Rankchem.for_streamlit.Highlighting import calculate_fukui
+from Rankchem.Highlighting import calculate_fukui
 
 def test_calculate_fukui():
     elements = ['C', 'O', 'H', 'H']
     coordinates = [[0.0, 0.0, 0.0], [1.0, 0.0, 0.0], [0.0, 1.0, 0.0], [0.0, 0.0, 1.0]]
     fukui_type = 'nucleophilicity'
     fukui_values = calculate_fukui(elements, coordinates, fukui_type)
     assert isinstance(fukui_values, dict), "Test failed: Result is not a dictionary"
```

### Comparing `rankchem-1.1.4/tests/test_rank_descriptors.py` & `rankchem-1.1.5/tests/test_rank_descriptors.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 import sys
 import os
 import pytest
 
 sys.path.insert(0, os.path.abspath(os.path.join(os.path.dirname(__file__), '..', 'src')))
 
-from Rankchem.for_streamlit.Ranking import rank_descriptors
+from Rankchem.Ranking import rank_descriptors
 
 def test_rank_descriptors():
     descriptors = [('SMILES1', 0.5), ('SMILES2', 0.3), ('SMILES3', 0.7)]
     ranked_descriptors = rank_descriptors(descriptors)
     assert isinstance(ranked_descriptors, list), "Test failed: Result is not a list"
     assert len(ranked_descriptors) == len(descriptors), "Test failed: Number of elements in result is incorrect"
     assert ranked_descriptors == [('SMILES3', 0.7), ('SMILES1', 0.5), ('SMILES2', 0.3)], "Test failed: Incorrect ranking"
```

### Comparing `rankchem-1.1.4/tests/test_smiles_to_xyz.py` & `rankchem-1.1.5/tests/test_smiles_to_xyz.py`

 * *Files 19% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 import sys
 import os
 sys.path.insert(0, os.path.abspath(os.path.join(os.path.dirname(__file__), '..', 'src')))
 
-from Rankchem.for_streamlit.Highlighting import smiles_to_xyz
+from Rankchem.Highlighting import smiles_to_xyz
 import os
 
 def test_smiles_to_xyz():
     filename = "test_molecule.xyz"
     result = smiles_to_xyz("C(=O)O", filename)
     assert result == filename, "Test failed: Incorrect filename returned"
     assert os.path.exists(filename), "Test failed: File not created"
```

