# Comparing `tmp/rankchem-0.1.1.tar.gz` & `tmp/rankchem-1.1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "rankchem-0.1.1.tar", last modified: Sun May 26 20:06:40 2024, max compression
+gzip compressed data, was "rankchem-1.1.1.tar", last modified: Wed May 29 14:34:15 2024, max compression
```

## Comparing `rankchem-0.1.1.tar` & `rankchem-1.1.1.tar`

### file list

```diff
@@ -1,24 +1,24 @@
-drwxrwxrwx   0 emmaunix  (1000) emmaunix  (1000)        0 2024-05-26 20:06:40.472808 rankchem-0.1.1/
--rwxrwxrwx   0 emmaunix  (1000) emmaunix  (1000)     1164 2024-05-17 18:59:58.000000 rankchem-0.1.1/LICENSE
--rwxrwxrwx   0 emmaunix  (1000) emmaunix  (1000)    10025 2024-05-26 20:06:40.468444 rankchem-0.1.1/PKG-INFO
--rwxrwxrwx   0 emmaunix  (1000) emmaunix  (1000)     7272 2024-05-26 19:58:45.000000 rankchem-0.1.1/README.md
--rwxrwxrwx   0 emmaunix  (1000) emmaunix  (1000)     1619 2024-05-26 20:02:09.000000 rankchem-0.1.1/pyproject.toml
--rwxrwxrwx   0 emmaunix  (1000) emmaunix  (1000)       38 2024-05-26 20:06:40.474065 rankchem-0.1.1/setup.cfg
--rwxrwxrwx   0 emmaunix  (1000) emmaunix  (1000)     1124 2024-05-26 20:02:11.000000 rankchem-0.1.1/setup.py
-drwxrwxrwx   0 emmaunix  (1000) emmaunix  (1000)        0 2024-05-26 20:06:40.299149 rankchem-0.1.1/src/
-drwxrwxrwx   0 emmaunix  (1000) emmaunix  (1000)        0 2024-05-26 20:06:40.461878 rankchem-0.1.1/src/RankChem.egg-info/
--rwxrwxrwx   0 emmaunix  (1000) emmaunix  (1000)    10025 2024-05-26 20:06:40.000000 rankchem-0.1.1/src/RankChem.egg-info/PKG-INFO
--rwxrwxrwx   0 emmaunix  (1000) emmaunix  (1000)      456 2024-05-26 20:06:40.000000 rankchem-0.1.1/src/RankChem.egg-info/SOURCES.txt
--rwxrwxrwx   0 emmaunix  (1000) emmaunix  (1000)        1 2024-05-26 20:06:40.000000 rankchem-0.1.1/src/RankChem.egg-info/dependency_links.txt
--rwxrwxrwx   0 emmaunix  (1000) emmaunix  (1000)      169 2024-05-26 20:06:40.000000 rankchem-0.1.1/src/RankChem.egg-info/requires.txt
--rwxrwxrwx   0 emmaunix  (1000) emmaunix  (1000)        9 2024-05-26 20:06:40.000000 rankchem-0.1.1/src/RankChem.egg-info/top_level.txt
-drwxrwxrwx   0 emmaunix  (1000) emmaunix  (1000)        0 2024-05-26 20:06:40.389203 rankchem-0.1.1/src/Rankchem/
--rwxrwxrwx   0 emmaunix  (1000) emmaunix  (1000)       82 2024-05-17 18:01:00.000000 rankchem-0.1.1/src/Rankchem/__init__.py
-drwxrwxrwx   0 emmaunix  (1000) emmaunix  (1000)        0 2024-05-26 20:06:40.447852 rankchem-0.1.1/tests/
--rwxrwxrwx   0 emmaunix  (1000) emmaunix  (1000)      608 2024-05-26 13:57:31.000000 rankchem-0.1.1/tests/test_average.py
--rwxrwxrwx   0 emmaunix  (1000) emmaunix  (1000)      592 2024-05-26 13:58:59.000000 rankchem-0.1.1/tests/test_calculate_descriptor.py
--rwxrwxrwx   0 emmaunix  (1000) emmaunix  (1000)      749 2024-05-26 12:24:41.000000 rankchem-0.1.1/tests/test_calculate_fukui.py
--rwxrwxrwx   0 emmaunix  (1000) emmaunix  (1000)      483 2024-05-26 12:24:41.000000 rankchem-0.1.1/tests/test_get_max_fukui_avg.py
--rwxrwxrwx   0 emmaunix  (1000) emmaunix  (1000)      665 2024-05-26 14:00:42.000000 rankchem-0.1.1/tests/test_rank_descriptors.py
--rwxrwxrwx   0 emmaunix  (1000) emmaunix  (1000)      617 2024-05-26 12:24:41.000000 rankchem-0.1.1/tests/test_smiles_to_xyz.py
--rwxrwxrwx   0 emmaunix  (1000) emmaunix  (1000)      409 2024-05-26 13:57:17.000000 rankchem-0.1.1/tests/test_visualize_molecule.py
+drwxrwxrwx   0 emmaunix  (1000) emmaunix  (1000)        0 2024-05-29 14:34:15.195316 rankchem-1.1.1/
+-rwxrwxrwx   0 emmaunix  (1000) emmaunix  (1000)     1164 2024-05-17 18:59:58.000000 rankchem-1.1.1/LICENSE
+-rwxrwxrwx   0 emmaunix  (1000) emmaunix  (1000)    10447 2024-05-29 14:34:15.187876 rankchem-1.1.1/PKG-INFO
+-rwxrwxrwx   0 emmaunix  (1000) emmaunix  (1000)     7698 2024-05-28 11:58:59.000000 rankchem-1.1.1/README.md
+-rwxrwxrwx   0 emmaunix  (1000) emmaunix  (1000)     1619 2024-05-29 14:27:15.000000 rankchem-1.1.1/pyproject.toml
+-rwxrwxrwx   0 emmaunix  (1000) emmaunix  (1000)       38 2024-05-29 14:34:15.196702 rankchem-1.1.1/setup.cfg
+-rwxrwxrwx   0 emmaunix  (1000) emmaunix  (1000)     1124 2024-05-29 14:27:19.000000 rankchem-1.1.1/setup.py
+drwxrwxrwx   0 emmaunix  (1000) emmaunix  (1000)        0 2024-05-29 14:34:14.270226 rankchem-1.1.1/src/
+drwxrwxrwx   0 emmaunix  (1000) emmaunix  (1000)        0 2024-05-29 14:34:15.173876 rankchem-1.1.1/src/RankChem.egg-info/
+-rwxrwxrwx   0 emmaunix  (1000) emmaunix  (1000)    10447 2024-05-29 14:34:13.000000 rankchem-1.1.1/src/RankChem.egg-info/PKG-INFO
+-rwxrwxrwx   0 emmaunix  (1000) emmaunix  (1000)      456 2024-05-29 14:34:14.000000 rankchem-1.1.1/src/RankChem.egg-info/SOURCES.txt
+-rwxrwxrwx   0 emmaunix  (1000) emmaunix  (1000)        1 2024-05-29 14:34:13.000000 rankchem-1.1.1/src/RankChem.egg-info/dependency_links.txt
+-rwxrwxrwx   0 emmaunix  (1000) emmaunix  (1000)      169 2024-05-29 14:34:13.000000 rankchem-1.1.1/src/RankChem.egg-info/requires.txt
+-rwxrwxrwx   0 emmaunix  (1000) emmaunix  (1000)        9 2024-05-29 14:34:13.000000 rankchem-1.1.1/src/RankChem.egg-info/top_level.txt
+drwxrwxrwx   0 emmaunix  (1000) emmaunix  (1000)        0 2024-05-29 14:34:14.842744 rankchem-1.1.1/src/Rankchem/
+-rwxrwxrwx   0 emmaunix  (1000) emmaunix  (1000)       82 2024-05-17 18:01:00.000000 rankchem-1.1.1/src/Rankchem/__init__.py
+drwxrwxrwx   0 emmaunix  (1000) emmaunix  (1000)        0 2024-05-29 14:34:15.135890 rankchem-1.1.1/tests/
+-rwxrwxrwx   0 emmaunix  (1000) emmaunix  (1000)      608 2024-05-26 13:57:31.000000 rankchem-1.1.1/tests/test_average.py
+-rwxrwxrwx   0 emmaunix  (1000) emmaunix  (1000)      592 2024-05-26 13:58:59.000000 rankchem-1.1.1/tests/test_calculate_descriptor.py
+-rwxrwxrwx   0 emmaunix  (1000) emmaunix  (1000)      749 2024-05-26 12:24:41.000000 rankchem-1.1.1/tests/test_calculate_fukui.py
+-rwxrwxrwx   0 emmaunix  (1000) emmaunix  (1000)      483 2024-05-26 12:24:41.000000 rankchem-1.1.1/tests/test_get_max_fukui_avg.py
+-rwxrwxrwx   0 emmaunix  (1000) emmaunix  (1000)      665 2024-05-26 14:00:42.000000 rankchem-1.1.1/tests/test_rank_descriptors.py
+-rwxrwxrwx   0 emmaunix  (1000) emmaunix  (1000)      617 2024-05-26 12:24:41.000000 rankchem-1.1.1/tests/test_smiles_to_xyz.py
+-rwxrwxrwx   0 emmaunix  (1000) emmaunix  (1000)      409 2024-05-26 13:57:17.000000 rankchem-1.1.1/tests/test_visualize_molecule.py
```

### Comparing `rankchem-0.1.1/LICENSE` & `rankchem-1.1.1/LICENSE`

 * *Files identical despite different names*

### Comparing `rankchem-0.1.1/PKG-INFO` & `rankchem-1.1.1/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: RankChem
-Version: 0.1.1
+Version: 1.1.1
 Summary: RankChem project
 Home-page: https://github.com/kappelemma/RankChem
 Author: Emma Kappeler, Ludovica Fracassi
 Author-email: Emma Kappeler <emma.kappeler@epfl.ch>, Ludovica Fracassi <ludovica.fracassi@epfl.ch>
 License: MIT License
         
         Copyright (c) 2024 by Emma Kappeler <emma.kappeler@epfl.ch>,
@@ -67,15 +67,15 @@
 # ChemInterface for Reactivity Analysis
 ### Project in the *Practical programming in chemistry* course EPFL CH-200
 [![python](https://img.shields.io/badge/Python-14354C?style=for-the-badge&logo=python&logoColor=white)](https://www.python.org)
 ![GitHub](https://img.shields.io/badge/github-%23121011.svg?style=for-the-badge&logo=github&logoColor=white)
 [![jupyter](https://img.shields.io/badge/Jupyter-F37626.svg?&style=for-the-badge&logo=Jupyter&logoColor=purple)](https://jupyter.org/)
 ![license](https://img.shields.io/badge/License-MIT-ac8b11.svg?style=for-the-badge&labelColor=green)
 
-## 🔥 Usage
+## 🔥 What is Rankchem about?
 
 This repository provides the user with a package which will display an interactive interface where the user will be able to analyse the reactivity of meolecules based on their electrophilicity or nucleophilicity. The package leads the user to a streamlit hompage. Two features are available. The first one enables the user to visulaize a molecule in 3D with the reactive site highlighted. The second feature ranks multiple molecule in the order of decreasing reactivity based on descriptors. Both these feature were made using XTB calculations.
 
 The developpers of this package are:
 - Ludovica Fracassi, 2nd year Bachelor student in Chemistry and Chemical engeneering at EPFL [![jhc github](https://img.shields.io/badge/GitHub-fracaludo-181717.svg?style=flat&logo=github)](https://github.com/fracaludo)
 - Emma Kappeler, 2nd year Bachelor student in Chemistry and Chemical engeneering at EPFL [![jhc github](https://img.shields.io/badge/GitHub-kappelemma-181717.svg?style=flat&logo=github)](https://github.com/kappelemma)
 
@@ -86,15 +86,15 @@
 
 Electrophilicity and nucleophilicity are fundamental concepts in organic chemistry that describe the reactivity of molecules. Electrophilicity refers to the ability of a molecule or ion to accept an electron pair, making it an electron-loving species (electrophile). Electrophiles typically have a positive charge, partial positive charge, or an electron-deficient atom, making them attracted to electron-rich regions. On the other hand, nucleophilicity describes the ability of a molecule or ion to donate an electron pair, making it an electron-rich species (nucleophile). Nucleophiles are usually negatively charged or have lone pairs of electrons, such as anions, amines, and alcohols. The interaction between nucleophiles and electrophiles drives many chemical reactions, particularly in organic synthesis, where nucleophiles attack electrophiles to form new bonds.
 
 Now let's go through the steps required to use this package.
 
 ## 👩‍💻 Installation
 
-❗ Before installing the package and all the dependencies, do not forget to create a new conda environment to prevent dependency conflicts and to keep the project isolated. This can be done by executing the folowing command:
+❗ Before installing the package and all the dependencies, do not forget to create a new conda environment to prevent dependency conflicts and to keep the project isolated. This can be done by executing the following command:
 
 ```bash
 conda create --name myenv python=3.10
 conda activate myenv
 ```
 Where myenv is the name of your environment.
 
@@ -106,15 +106,15 @@
 ```
 
 The package can also be installed from source by running the following commands:
 
 First, clone the repository from Github and go in the RankChem folder.
 
 ```bash
-git clone [https://github.com/fracaludo/RankChem.git]
+git clone https://github.com/fracaludo/RankChem.git
 cd RankChem
 ```
 
 Then, install the package using :
 
 ```bash
 pip install -e .
@@ -180,24 +180,28 @@
 
 ![highlight](assets/highlightexample.png)
 
 Lastly, the Ranking feature enable the user to input multiple smiles and again choose if nucleophilicity or electrophilicity is analysed. The interface will then return the moelcules with highest: the most electrophile/nucleophile molecule and lowest the least electrophile/nucleophile molecule. Their corresponding descriptors values are also displayed. An example is shown below:
 
 ![ranking](assets/rankingexample.png)
 
-More information on the usage and limitations of the package can be found in our [jupyter notebook based report]https://github.com/fracaludo/RankChem/blob/main/notebooks/project_report.ipynb 📓
+More information on the usage and limitations of the package can be found in our [jupyter notebook based report](https://github.com/fracaludo/RankChem/blob/main/notebooks/project_report.ipynb) 📓
 
 ## 🚥 Let's get started!
 
-The streamlit interface can now finally be used!!
+The streamlit interface can now finally be used!! ⚠️ currently not working due to conda environment.yml problems. In order to open the working interface, follow the steps descibed previously in your terminal.
 
 Just click on the logo below ;)
 
 [![Streamlit App](https://static.streamlit.io/badges/streamlit_badge_black_white.svg)](https://rankchem.streamlit.app/)
 
+
+## ❗❗ Important
+The package displays the wrong active sites and the ranking is often wrong. This is due to fukui dictionnaries/global descriptors inconsistencies from morfeus-ml or xtb-python. This issue is out of our reach. Sorry :(
+
 ## 🔎 References an documentation
 
 Here is some useful reading on the packages that we used to create this project.
 
 https://digital-chemistry-laboratory.github.io/morfeus/
 https://github.com/digital-chemistry-laboratory/morfeus
 https://github.com/napoles-uach/stmol
```

### Comparing `rankchem-0.1.1/README.md` & `rankchem-1.1.1/README.md`

 * *Files 4% similar despite different names*

```diff
@@ -3,15 +3,15 @@
 # ChemInterface for Reactivity Analysis
 ### Project in the *Practical programming in chemistry* course EPFL CH-200
 [![python](https://img.shields.io/badge/Python-14354C?style=for-the-badge&logo=python&logoColor=white)](https://www.python.org)
 ![GitHub](https://img.shields.io/badge/github-%23121011.svg?style=for-the-badge&logo=github&logoColor=white)
 [![jupyter](https://img.shields.io/badge/Jupyter-F37626.svg?&style=for-the-badge&logo=Jupyter&logoColor=purple)](https://jupyter.org/)
 ![license](https://img.shields.io/badge/License-MIT-ac8b11.svg?style=for-the-badge&labelColor=green)
 
-## 🔥 Usage
+## 🔥 What is Rankchem about?
 
 This repository provides the user with a package which will display an interactive interface where the user will be able to analyse the reactivity of meolecules based on their electrophilicity or nucleophilicity. The package leads the user to a streamlit hompage. Two features are available. The first one enables the user to visulaize a molecule in 3D with the reactive site highlighted. The second feature ranks multiple molecule in the order of decreasing reactivity based on descriptors. Both these feature were made using XTB calculations.
 
 The developpers of this package are:
 - Ludovica Fracassi, 2nd year Bachelor student in Chemistry and Chemical engeneering at EPFL [![jhc github](https://img.shields.io/badge/GitHub-fracaludo-181717.svg?style=flat&logo=github)](https://github.com/fracaludo)
 - Emma Kappeler, 2nd year Bachelor student in Chemistry and Chemical engeneering at EPFL [![jhc github](https://img.shields.io/badge/GitHub-kappelemma-181717.svg?style=flat&logo=github)](https://github.com/kappelemma)
 
@@ -22,15 +22,15 @@
 
 Electrophilicity and nucleophilicity are fundamental concepts in organic chemistry that describe the reactivity of molecules. Electrophilicity refers to the ability of a molecule or ion to accept an electron pair, making it an electron-loving species (electrophile). Electrophiles typically have a positive charge, partial positive charge, or an electron-deficient atom, making them attracted to electron-rich regions. On the other hand, nucleophilicity describes the ability of a molecule or ion to donate an electron pair, making it an electron-rich species (nucleophile). Nucleophiles are usually negatively charged or have lone pairs of electrons, such as anions, amines, and alcohols. The interaction between nucleophiles and electrophiles drives many chemical reactions, particularly in organic synthesis, where nucleophiles attack electrophiles to form new bonds.
 
 Now let's go through the steps required to use this package.
 
 ## 👩‍💻 Installation
 
-❗ Before installing the package and all the dependencies, do not forget to create a new conda environment to prevent dependency conflicts and to keep the project isolated. This can be done by executing the folowing command:
+❗ Before installing the package and all the dependencies, do not forget to create a new conda environment to prevent dependency conflicts and to keep the project isolated. This can be done by executing the following command:
 
 ```bash
 conda create --name myenv python=3.10
 conda activate myenv
 ```
 Where myenv is the name of your environment.
 
@@ -42,15 +42,15 @@
 ```
 
 The package can also be installed from source by running the following commands:
 
 First, clone the repository from Github and go in the RankChem folder.
 
 ```bash
-git clone [https://github.com/fracaludo/RankChem.git]
+git clone https://github.com/fracaludo/RankChem.git
 cd RankChem
 ```
 
 Then, install the package using :
 
 ```bash
 pip install -e .
@@ -116,24 +116,28 @@
 
 ![highlight](assets/highlightexample.png)
 
 Lastly, the Ranking feature enable the user to input multiple smiles and again choose if nucleophilicity or electrophilicity is analysed. The interface will then return the moelcules with highest: the most electrophile/nucleophile molecule and lowest the least electrophile/nucleophile molecule. Their corresponding descriptors values are also displayed. An example is shown below:
 
 ![ranking](assets/rankingexample.png)
 
-More information on the usage and limitations of the package can be found in our [jupyter notebook based report]https://github.com/fracaludo/RankChem/blob/main/notebooks/project_report.ipynb 📓
+More information on the usage and limitations of the package can be found in our [jupyter notebook based report](https://github.com/fracaludo/RankChem/blob/main/notebooks/project_report.ipynb) 📓
 
 ## 🚥 Let's get started!
 
-The streamlit interface can now finally be used!!
+The streamlit interface can now finally be used!! ⚠️ currently not working due to conda environment.yml problems. In order to open the working interface, follow the steps descibed previously in your terminal.
 
 Just click on the logo below ;)
 
 [![Streamlit App](https://static.streamlit.io/badges/streamlit_badge_black_white.svg)](https://rankchem.streamlit.app/)
 
+
+## ❗❗ Important
+The package displays the wrong active sites and the ranking is often wrong. This is due to fukui dictionnaries/global descriptors inconsistencies from morfeus-ml or xtb-python. This issue is out of our reach. Sorry :(
+
 ## 🔎 References an documentation
 
 Here is some useful reading on the packages that we used to create this project.
 
 https://digital-chemistry-laboratory.github.io/morfeus/
 https://github.com/digital-chemistry-laboratory/morfeus
 https://github.com/napoles-uach/stmol
```

### Comparing `rankchem-0.1.1/pyproject.toml` & `rankchem-1.1.1/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -57,15 +57,15 @@
     "myst-parser",
     "sphinx>=5",
     "sphinx-copybutton",
 ]
 
 [tool.hatch.version]
 path = "src/Rankchem/__init__.py"
-version = "0.1.1"
+version = "1.1.1"
 
 [tool.pytest.ini_options]
 testpaths = [
     "tests",
 ]
 
 [tool.coverage.run]
```

### Comparing `rankchem-0.1.1/setup.py` & `rankchem-1.1.1/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from setuptools import setup, find_packages
 
 setup(
     name='rankchem',
-    version='0.1.1',
+    version='1.1.1',
     packages=find_packages(where='src'),
     package_dir={'': 'src'},
     install_requires=[
         'rdkit',
         'morfeus-ml',
         'pyvistaqt',
         'numpy',
```

### Comparing `rankchem-0.1.1/src/RankChem.egg-info/PKG-INFO` & `rankchem-1.1.1/src/RankChem.egg-info/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: RankChem
-Version: 0.1.1
+Version: 1.1.1
 Summary: RankChem project
 Home-page: https://github.com/kappelemma/RankChem
 Author: Emma Kappeler, Ludovica Fracassi
 Author-email: Emma Kappeler <emma.kappeler@epfl.ch>, Ludovica Fracassi <ludovica.fracassi@epfl.ch>
 License: MIT License
         
         Copyright (c) 2024 by Emma Kappeler <emma.kappeler@epfl.ch>,
@@ -67,15 +67,15 @@
 # ChemInterface for Reactivity Analysis
 ### Project in the *Practical programming in chemistry* course EPFL CH-200
 [![python](https://img.shields.io/badge/Python-14354C?style=for-the-badge&logo=python&logoColor=white)](https://www.python.org)
 ![GitHub](https://img.shields.io/badge/github-%23121011.svg?style=for-the-badge&logo=github&logoColor=white)
 [![jupyter](https://img.shields.io/badge/Jupyter-F37626.svg?&style=for-the-badge&logo=Jupyter&logoColor=purple)](https://jupyter.org/)
 ![license](https://img.shields.io/badge/License-MIT-ac8b11.svg?style=for-the-badge&labelColor=green)
 
-## 🔥 Usage
+## 🔥 What is Rankchem about?
 
 This repository provides the user with a package which will display an interactive interface where the user will be able to analyse the reactivity of meolecules based on their electrophilicity or nucleophilicity. The package leads the user to a streamlit hompage. Two features are available. The first one enables the user to visulaize a molecule in 3D with the reactive site highlighted. The second feature ranks multiple molecule in the order of decreasing reactivity based on descriptors. Both these feature were made using XTB calculations.
 
 The developpers of this package are:
 - Ludovica Fracassi, 2nd year Bachelor student in Chemistry and Chemical engeneering at EPFL [![jhc github](https://img.shields.io/badge/GitHub-fracaludo-181717.svg?style=flat&logo=github)](https://github.com/fracaludo)
 - Emma Kappeler, 2nd year Bachelor student in Chemistry and Chemical engeneering at EPFL [![jhc github](https://img.shields.io/badge/GitHub-kappelemma-181717.svg?style=flat&logo=github)](https://github.com/kappelemma)
 
@@ -86,15 +86,15 @@
 
 Electrophilicity and nucleophilicity are fundamental concepts in organic chemistry that describe the reactivity of molecules. Electrophilicity refers to the ability of a molecule or ion to accept an electron pair, making it an electron-loving species (electrophile). Electrophiles typically have a positive charge, partial positive charge, or an electron-deficient atom, making them attracted to electron-rich regions. On the other hand, nucleophilicity describes the ability of a molecule or ion to donate an electron pair, making it an electron-rich species (nucleophile). Nucleophiles are usually negatively charged or have lone pairs of electrons, such as anions, amines, and alcohols. The interaction between nucleophiles and electrophiles drives many chemical reactions, particularly in organic synthesis, where nucleophiles attack electrophiles to form new bonds.
 
 Now let's go through the steps required to use this package.
 
 ## 👩‍💻 Installation
 
-❗ Before installing the package and all the dependencies, do not forget to create a new conda environment to prevent dependency conflicts and to keep the project isolated. This can be done by executing the folowing command:
+❗ Before installing the package and all the dependencies, do not forget to create a new conda environment to prevent dependency conflicts and to keep the project isolated. This can be done by executing the following command:
 
 ```bash
 conda create --name myenv python=3.10
 conda activate myenv
 ```
 Where myenv is the name of your environment.
 
@@ -106,15 +106,15 @@
 ```
 
 The package can also be installed from source by running the following commands:
 
 First, clone the repository from Github and go in the RankChem folder.
 
 ```bash
-git clone [https://github.com/fracaludo/RankChem.git]
+git clone https://github.com/fracaludo/RankChem.git
 cd RankChem
 ```
 
 Then, install the package using :
 
 ```bash
 pip install -e .
@@ -180,24 +180,28 @@
 
 ![highlight](assets/highlightexample.png)
 
 Lastly, the Ranking feature enable the user to input multiple smiles and again choose if nucleophilicity or electrophilicity is analysed. The interface will then return the moelcules with highest: the most electrophile/nucleophile molecule and lowest the least electrophile/nucleophile molecule. Their corresponding descriptors values are also displayed. An example is shown below:
 
 ![ranking](assets/rankingexample.png)
 
-More information on the usage and limitations of the package can be found in our [jupyter notebook based report]https://github.com/fracaludo/RankChem/blob/main/notebooks/project_report.ipynb 📓
+More information on the usage and limitations of the package can be found in our [jupyter notebook based report](https://github.com/fracaludo/RankChem/blob/main/notebooks/project_report.ipynb) 📓
 
 ## 🚥 Let's get started!
 
-The streamlit interface can now finally be used!!
+The streamlit interface can now finally be used!! ⚠️ currently not working due to conda environment.yml problems. In order to open the working interface, follow the steps descibed previously in your terminal.
 
 Just click on the logo below ;)
 
 [![Streamlit App](https://static.streamlit.io/badges/streamlit_badge_black_white.svg)](https://rankchem.streamlit.app/)
 
+
+## ❗❗ Important
+The package displays the wrong active sites and the ranking is often wrong. This is due to fukui dictionnaries/global descriptors inconsistencies from morfeus-ml or xtb-python. This issue is out of our reach. Sorry :(
+
 ## 🔎 References an documentation
 
 Here is some useful reading on the packages that we used to create this project.
 
 https://digital-chemistry-laboratory.github.io/morfeus/
 https://github.com/digital-chemistry-laboratory/morfeus
 https://github.com/napoles-uach/stmol
```

### Comparing `rankchem-0.1.1/tests/test_average.py` & `rankchem-1.1.1/tests/test_average.py`

 * *Files identical despite different names*

### Comparing `rankchem-0.1.1/tests/test_calculate_descriptor.py` & `rankchem-1.1.1/tests/test_calculate_descriptor.py`

 * *Files identical despite different names*

### Comparing `rankchem-0.1.1/tests/test_calculate_fukui.py` & `rankchem-1.1.1/tests/test_calculate_fukui.py`

 * *Files identical despite different names*

### Comparing `rankchem-0.1.1/tests/test_rank_descriptors.py` & `rankchem-1.1.1/tests/test_rank_descriptors.py`

 * *Files identical despite different names*

### Comparing `rankchem-0.1.1/tests/test_smiles_to_xyz.py` & `rankchem-1.1.1/tests/test_smiles_to_xyz.py`

 * *Files identical despite different names*

