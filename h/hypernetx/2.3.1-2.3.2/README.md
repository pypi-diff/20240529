# Comparing `tmp/hypernetx-2.3.1.tar.gz` & `tmp/hypernetx-2.3.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "hypernetx-2.3.1.tar", max compression
+gzip compressed data, was "hypernetx-2.3.2.tar", max compression
```

## Comparing `hypernetx-2.3.1.tar` & `hypernetx-2.3.2.tar`

### file list

```diff
@@ -1,40 +1,40 @@
--rw-r--r--   0        0        0     1531 2024-05-17 22:55:30.575081 hypernetx-2.3.1/LICENSE.rst
--rw-r--r--   0        0        0    14282 2024-05-17 22:55:30.575081 hypernetx-2.3.1/README.md
--rw-r--r--   0        0        0      394 2024-05-17 22:55:30.583081 hypernetx-2.3.1/hypernetx/__init__.py
--rw-r--r--   0        0        0     2539 2024-05-17 22:55:30.583081 hypernetx-2.3.1/hypernetx/algorithms/__init__.py
--rw-r--r--   0        0        0    39968 2024-05-17 22:55:30.583081 hypernetx-2.3.1/hypernetx/algorithms/contagion.py
--rw-r--r--   0        0        0     8678 2024-05-17 22:55:30.583081 hypernetx-2.3.1/hypernetx/algorithms/generative_models.py
--rw-r--r--   0        0        0    24278 2024-05-17 22:55:30.583081 hypernetx-2.3.1/hypernetx/algorithms/homology_mod2.py
--rw-r--r--   0        0        0    18956 2024-05-17 22:55:30.583081 hypernetx-2.3.1/hypernetx/algorithms/hypergraph_modularity.py
--rw-r--r--   0        0        0     7821 2024-05-17 22:55:30.583081 hypernetx-2.3.1/hypernetx/algorithms/laplacians_clustering.py
--rw-r--r--   0        0        0     9964 2024-05-17 22:55:30.583081 hypernetx-2.3.1/hypernetx/algorithms/s_centrality_measures.py
--rw-r--r--   0        0        0      237 2024-05-17 22:55:30.583081 hypernetx-2.3.1/hypernetx/classes/__init__.py
--rw-r--r--   0        0        0    13259 2024-05-17 22:55:30.583081 hypernetx-2.3.1/hypernetx/classes/factory.py
--rw-r--r--   0        0        0     9852 2024-05-17 22:55:30.583081 hypernetx-2.3.1/hypernetx/classes/hyp_view.py
--rw-r--r--   0        0        0    98452 2024-05-17 22:55:30.583081 hypernetx-2.3.1/hypernetx/classes/hypergraph.py
--rw-r--r--   0        0        0     7443 2024-05-17 22:55:30.583081 hypernetx-2.3.1/hypernetx/classes/incidence_store.py
--rw-r--r--   0        0        0    10028 2024-05-17 22:55:30.583081 hypernetx-2.3.1/hypernetx/classes/property_store.py
--rw-r--r--   0        0        0      151 2024-05-17 22:55:30.583081 hypernetx-2.3.1/hypernetx/drawing/__init__.py
--rw-r--r--   0        0        0    16790 2024-05-17 22:55:30.583081 hypernetx-2.3.1/hypernetx/drawing/rubber_band.py
--rw-r--r--   0        0        0     5612 2024-05-17 22:55:30.583081 hypernetx-2.3.1/hypernetx/drawing/two_column.py
--rw-r--r--   0        0        0     3406 2024-05-17 22:55:30.583081 hypernetx-2.3.1/hypernetx/drawing/util.py
--rw-r--r--   0        0        0      426 2024-05-17 22:55:30.583081 hypernetx-2.3.1/hypernetx/exception.py
--rw-r--r--   0        0        0      379 2024-05-17 22:55:30.583081 hypernetx-2.3.1/hypernetx/read_write.py
--rw-r--r--   0        0        0      491 2024-05-17 22:55:30.583081 hypernetx-2.3.1/hypernetx/reports/__init__.py
--rw-r--r--   0        0        0    11393 2024-05-17 22:55:30.583081 hypernetx-2.3.1/hypernetx/reports/descriptive_stats.py
--rw-r--r--   0        0        0      720 2024-05-17 22:55:30.583081 hypernetx-2.3.1/hypernetx/utils/__init__.py
--rw-r--r--   0        0        0     2430 2024-05-17 22:55:30.583081 hypernetx-2.3.1/hypernetx/utils/decorators.py
--rw-r--r--   0        0        0     5122 2024-05-17 22:55:30.583081 hypernetx-2.3.1/hypernetx/utils/extras.py
--rw-r--r--   0        0        0     1423 2024-05-17 22:55:30.583081 hypernetx-2.3.1/hypernetx/utils/log.py
--rw-r--r--   0        0        0   165566 2024-05-17 22:55:30.587081 hypernetx-2.3.1/hypernetx/utils/toys/ChungLuTransmissionData.csv
--rw-r--r--   0        0        0   116969 2024-05-17 22:55:30.587081 hypernetx-2.3.1/hypernetx/utils/toys/GoT.pkl
--rw-r--r--   0        0        0     7925 2024-05-17 22:55:30.587081 hypernetx-2.3.1/hypernetx/utils/toys/HarryPotterHypergraph.p
--rw-r--r--   0        0        0    26129 2024-05-17 22:55:30.587081 hypernetx-2.3.1/hypernetx/utils/toys/HarryPotter_Characters.csv
--rw-r--r--   0        0        0      409 2024-05-17 22:55:30.587081 hypernetx-2.3.1/hypernetx/utils/toys/__init__.py
--rw-r--r--   0        0        0  1736336 2024-05-17 22:55:30.591081 hypernetx-2.3.1/hypernetx/utils/toys/disGene.txt
--rw-r--r--   0        0        0      353 2024-05-17 22:55:30.591081 hypernetx-2.3.1/hypernetx/utils/toys/gene_data.py
--rw-r--r--   0        0        0     3809 2024-05-17 22:55:30.591081 hypernetx-2.3.1/hypernetx/utils/toys/harrypotter.py
--rw-r--r--   0        0        0    14357 2024-05-17 22:55:30.591081 hypernetx-2.3.1/hypernetx/utils/toys/lesmis.py
--rw-r--r--   0        0        0      552 2024-05-17 22:55:30.591081 hypernetx-2.3.1/hypernetx/utils/toys/transmission_problem.py
--rw-r--r--   0        0        0     2429 2024-05-17 22:55:30.595081 hypernetx-2.3.1/pyproject.toml
--rw-r--r--   0        0        0    15251 1970-01-01 00:00:00.000000 hypernetx-2.3.1/PKG-INFO
+-rw-r--r--   0        0        0     1531 2024-05-29 21:03:46.934074 hypernetx-2.3.2/LICENSE.rst
+-rw-r--r--   0        0        0    13922 2024-05-29 21:03:46.934074 hypernetx-2.3.2/README.md
+-rw-r--r--   0        0        0      394 2024-05-29 21:03:46.942074 hypernetx-2.3.2/hypernetx/__init__.py
+-rw-r--r--   0        0        0     2539 2024-05-29 21:03:46.942074 hypernetx-2.3.2/hypernetx/algorithms/__init__.py
+-rw-r--r--   0        0        0    39968 2024-05-29 21:03:46.942074 hypernetx-2.3.2/hypernetx/algorithms/contagion.py
+-rw-r--r--   0        0        0     8678 2024-05-29 21:03:46.942074 hypernetx-2.3.2/hypernetx/algorithms/generative_models.py
+-rw-r--r--   0        0        0    24278 2024-05-29 21:03:46.942074 hypernetx-2.3.2/hypernetx/algorithms/homology_mod2.py
+-rw-r--r--   0        0        0    18956 2024-05-29 21:03:46.942074 hypernetx-2.3.2/hypernetx/algorithms/hypergraph_modularity.py
+-rw-r--r--   0        0        0     7821 2024-05-29 21:03:46.942074 hypernetx-2.3.2/hypernetx/algorithms/laplacians_clustering.py
+-rw-r--r--   0        0        0     9964 2024-05-29 21:03:46.942074 hypernetx-2.3.2/hypernetx/algorithms/s_centrality_measures.py
+-rw-r--r--   0        0        0      237 2024-05-29 21:03:46.942074 hypernetx-2.3.2/hypernetx/classes/__init__.py
+-rw-r--r--   0        0        0    13259 2024-05-29 21:03:46.942074 hypernetx-2.3.2/hypernetx/classes/factory.py
+-rw-r--r--   0        0        0     9852 2024-05-29 21:03:46.942074 hypernetx-2.3.2/hypernetx/classes/hyp_view.py
+-rw-r--r--   0        0        0    98452 2024-05-29 21:03:46.942074 hypernetx-2.3.2/hypernetx/classes/hypergraph.py
+-rw-r--r--   0        0        0     7443 2024-05-29 21:03:46.942074 hypernetx-2.3.2/hypernetx/classes/incidence_store.py
+-rw-r--r--   0        0        0    10028 2024-05-29 21:03:46.942074 hypernetx-2.3.2/hypernetx/classes/property_store.py
+-rw-r--r--   0        0        0      151 2024-05-29 21:03:46.942074 hypernetx-2.3.2/hypernetx/drawing/__init__.py
+-rw-r--r--   0        0        0    16790 2024-05-29 21:03:46.942074 hypernetx-2.3.2/hypernetx/drawing/rubber_band.py
+-rw-r--r--   0        0        0     5612 2024-05-29 21:03:46.942074 hypernetx-2.3.2/hypernetx/drawing/two_column.py
+-rw-r--r--   0        0        0     3406 2024-05-29 21:03:46.942074 hypernetx-2.3.2/hypernetx/drawing/util.py
+-rw-r--r--   0        0        0      426 2024-05-29 21:03:46.942074 hypernetx-2.3.2/hypernetx/exception.py
+-rw-r--r--   0        0        0      379 2024-05-29 21:03:46.942074 hypernetx-2.3.2/hypernetx/read_write.py
+-rw-r--r--   0        0        0      491 2024-05-29 21:03:46.942074 hypernetx-2.3.2/hypernetx/reports/__init__.py
+-rw-r--r--   0        0        0    11393 2024-05-29 21:03:46.942074 hypernetx-2.3.2/hypernetx/reports/descriptive_stats.py
+-rw-r--r--   0        0        0      720 2024-05-29 21:03:46.942074 hypernetx-2.3.2/hypernetx/utils/__init__.py
+-rw-r--r--   0        0        0     2430 2024-05-29 21:03:46.942074 hypernetx-2.3.2/hypernetx/utils/decorators.py
+-rw-r--r--   0        0        0     5122 2024-05-29 21:03:46.942074 hypernetx-2.3.2/hypernetx/utils/extras.py
+-rw-r--r--   0        0        0     1423 2024-05-29 21:03:46.942074 hypernetx-2.3.2/hypernetx/utils/log.py
+-rw-r--r--   0        0        0   165566 2024-05-29 21:03:46.946075 hypernetx-2.3.2/hypernetx/utils/toys/ChungLuTransmissionData.csv
+-rw-r--r--   0        0        0   116969 2024-05-29 21:03:46.946075 hypernetx-2.3.2/hypernetx/utils/toys/GoT.pkl
+-rw-r--r--   0        0        0     7925 2024-05-29 21:03:46.946075 hypernetx-2.3.2/hypernetx/utils/toys/HarryPotterHypergraph.p
+-rw-r--r--   0        0        0    26129 2024-05-29 21:03:46.946075 hypernetx-2.3.2/hypernetx/utils/toys/HarryPotter_Characters.csv
+-rw-r--r--   0        0        0      409 2024-05-29 21:03:46.946075 hypernetx-2.3.2/hypernetx/utils/toys/__init__.py
+-rw-r--r--   0        0        0  1736336 2024-05-29 21:03:46.950075 hypernetx-2.3.2/hypernetx/utils/toys/disGene.txt
+-rw-r--r--   0        0        0      353 2024-05-29 21:03:46.950075 hypernetx-2.3.2/hypernetx/utils/toys/gene_data.py
+-rw-r--r--   0        0        0     3809 2024-05-29 21:03:46.950075 hypernetx-2.3.2/hypernetx/utils/toys/harrypotter.py
+-rw-r--r--   0        0        0    14357 2024-05-29 21:03:46.950075 hypernetx-2.3.2/hypernetx/utils/toys/lesmis.py
+-rw-r--r--   0        0        0      552 2024-05-29 21:03:46.950075 hypernetx-2.3.2/hypernetx/utils/toys/transmission_problem.py
+-rw-r--r--   0        0        0     2429 2024-05-29 21:03:46.950075 hypernetx-2.3.2/pyproject.toml
+-rw-r--r--   0        0        0    14882 1970-01-01 00:00:00.000000 hypernetx-2.3.2/PKG-INFO
```

### Comparing `hypernetx-2.3.1/LICENSE.rst` & `hypernetx-2.3.2/LICENSE.rst`

 * *Files identical despite different names*

### Comparing `hypernetx-2.3.1/README.md` & `hypernetx-2.3.2/README.md`

 * *Files 6% similar despite different names*

```diff
@@ -68,58 +68,58 @@
 ------------
 
 
 <a href="https://colab.research.google.com/github/pnnl/HyperNetX/blob/master/tutorials/basic/Basic%201%20-%20HNX%20Basics.ipynb" target="_blank">
   <img src="https://colab.research.google.com/assets/colab-badge.svg" alt="Open In Colab"/>
     <span >Basic 1 - HNX Basics</span>
 </a>
-</br>
+<br>
 
 <a href="https://colab.research.google.com/github/pnnl/HyperNetX/blob/master/tutorials/basic/Basic%202%20-%20Visualization%20Methods.ipynb" target="_blank">
   <img src="https://colab.research.google.com/assets/colab-badge.svg" alt="Open In Colab"/>
     <span >Basic 2 - Visualization Methods</span>
 </a>
-</br>
+<br>
 
 <a href="https://colab.research.google.com/github/pnnl/HyperNetX/blob/master/tutorials/basic/Basic%203%20-%20LesMis%20Case%20Study.ipynb" target="_blank">
   <img src="https://colab.research.google.com/assets/colab-badge.svg" alt="Open In Colab"/>
     <span >Basic 3 - LesMis Case Study</span>
 </a>
-</br>
+<br>
 
 <a href="https://colab.research.google.com/github/pnnl/HyperNetX/blob/master/tutorials/basic/Basic%204%20-%20LesMis%20Visualizations-BookTour.ipynb" target="_blank">
   <img src="https://colab.research.google.com/assets/colab-badge.svg" alt="Open In Colab"/>
     <span >Basic 4 - LesMis Visualizations-Book Tour</span>
 </a>
-</br>
+<br>
 
 <a href="https://colab.research.google.com/github/pnnl/HyperNetX/blob/master/tutorials/basic/Basic%205%20-%20HNX%20attributed%20hypergraph.ipynb" target="_blank">
   <img src="https://colab.research.google.com/assets/colab-badge.svg" alt="Open In Colab"/>
     <span >Basic 5 - HNX attributed hypergraph</span>
 </a>
-</br>
+<br>
 
 <a href="https://colab.research.google.com/github/pnnl/HyperNetX/blob/master/tutorials/basic/Basic%206%20-%20Hypergraph%20Arithmetic.ipynb" target="_blank">
   <img src="https://colab.research.google.com/assets/colab-badge.svg" alt="Open In Colab"/>
     <span >Basic 6 - Hypergraph Arithmetic.ipynb</span>
 </a>
-</br>
+<br>
 
 
 Jupyter Notebooks
 -----------------
 
 Additional tutorials that can be run as Jupyter Notebooks are found under [tutorials](./tutorials).
 
 Installation
 ====================
 
 The recommended installation method for most users is to create a virtual environment and install HyperNetX from PyPi.
 
-HyperNetX may be cloned or forked from [Github](https://github.com/pnnl/HyperNetX).
+HyperNetX may be cloned or forked from [GitHub](https://github.com/pnnl/HyperNetX).
 
 Prerequisites
 -------------
 HyperNetX officially supports Python 3.8, 3.9, 3.10 and 3.11.
 
 Create a virtual environment
 ----------------------------
@@ -164,15 +164,15 @@
 ```shell
 .\env-hnx\Scripts\deactivate
 ```
 
 Installing HyperNetX
 ====================
 
-Regardless of how you install HyperNetX, ensure that your environment is activated and that you are running Python >=3.8.
+Regardless of how you install HyperNetX, ensure that your environment is activated and that you are running Python >=3.10.
 
 
 Installing from PyPi
 --------------------
 
 ```shell
 pip install hypernetx
@@ -257,46 +257,54 @@
 -----------------------------
 
 > ℹ️ **NOTE:** This project has a pytest configuration file named 'pytest.ini'. By default, pytest will use those configuration settings to run tests.
 
 ```shell
 poetry install --with test
 
+# activate your virtual environment created by poetry
+poetry shell
+
 # run tests
 python -m pytest
 
 # run tests and show coverage report
 python -m pytest --cov=hypernetx
 
 # Generate an HTML code coverage report and view it on a browser
 coverage html
 open htmlcov/index.html
 ```
 
 Install support for tutorials
 -----------------------------
 
-```
+```shell
 poetry install --with tutorials
 
+# activate your virtual environment created by poetry
+poetry shell
+
 # open Jupyter notebooks in a browser
 make tutorials
 ```
 
 Code Quality
 ------------
 HyperNetX uses a number of tools to maintain code quality:
 
 * Pylint
 * Black
 
 Before using these tools, ensure that you install Pylint in your environment:
 
-```
+```shell
 poetry install --with lint
+# activate your virtual environment created by poetry
+poetry shell
 ```
 
 Pylint
 ------
 
 [Pylint](https://pylint.pycqa.org/en/latest/index.html) is a static code analyzer for Python-based projects. From the [Pylint docs](https://pylint.pycqa.org/en/latest/index.html#what-is-pylint):
 
@@ -321,30 +329,47 @@
 [Black](https://black.readthedocs.io/en/stable/) is a PEP 8 compliant formatter for Python-based project. This tool is highly opinionated about how Python should be formatted and will automagically reformat your code.
 
 
 ```shell
 black hypernetx
 ```
 
+Pre-commit
+---------
+
+Use the [pre-commit framework](https://pre-commit.com/) to automatically point out issues and resolve those issues before code review.
+It is highly recommended to install pre-commit in your development environment so that issues with your code can be found before you submit a
+pull request. More importantly, using pre-commit will automatically format your code changes so that they pass the CI build. For example, pre-commit will
+automatically run the formatter Black on your code changes.
+
+```shell
+pre-commit install
+
+# Once installed, pre-commit will be triggered every time you make a commit in your environment
+```
+
 Documentation
 -------------
 
 Build and view documentation locally:
 
-```
+```shell
 poetry install --with docs
+# activate your virtual environment created by poetry
+poetry shell
+
 cd docs
 make html
 open docs/build/html/index.html
 ```
 
 When editing documentation, you can auto-rebuild the documentation locally so that you can view your document changes
 live on the browser without having to rebuild every time you have a change.
 
-```
+```shell
 cd docs
 make livehtml
 ```
 
 This make script will run in the foreground on your terminal. You should see the following:
 
 ```shell
@@ -356,57 +381,20 @@
 [I 230324 09:51:02 handlers:135] Browser Connected: http://127.0.0.1:8000/
 ```
 
 Click on `http://127.0.0.1:8000/install.html` to open the docs on your browser. Since this will auto-rebuild, every time
 you change a document file, it will automatically render on your browser, allowing you to verify your document changes.
 
 
-Continuous Integration
-======================
-
-This project runs Continuous Integration (CI) using GitHub Actions. Normally, CI runs
-on pull requests, pushes to certain branches, and other events.
-
-Maintainers of the GitHub repository can manually trigger CI using [GitHub CLI](https://cli.github.com/). See instructions below on how to manually trigger CI on GitHub Actions:
-
-```commandline
-# login to Github
-gh auth login --with-token <  ~/.ssh/tokens/<path to my personal access token>
-
-# Trigger CI
-gh workflow run ci.yml --repo pnnl/HyperNetX --ref <name of branch that you want CI to run on> --field triggeredBy="<Your name>"
-
-# Get the status of the workflow
-gh run list --workflow=ci.yml --repo pnnl/HyperNetX
-```
-
-
-Versioning
-==========
-
-This project uses [`commitizen`](https://github.com/commitizen-tools/commitizen) to manage versioning.
-The files where "version" will be updated are listed in the '.cz.toml' file. To create a new version and the associated tag,
-run the following commands:
-
-```shell
-# Install commitizen tool to environment
-pip install commitizen
-
-# Updates version; values for '--increment' can be MAJOR, MINOR, or PATCH
-# Autocreates a tag and commit for the updated version
-cz bump  --increment MAJOR  --dry-run
-cz bump  --increment MAJOR
-```
-
 Notice
 ======
 This material was prepared as an account of work sponsored by an agency of the United States Government.  Neither the United States Government nor the United States Department of Energy, nor Battelle, nor any of their employees, nor any jurisdiction or organization that has cooperated in the development of these materials, makes any warranty, express or implied, or assumes any legal liability or responsibility for the accuracy, completeness, or usefulness or any information, apparatus, product, software, or process disclosed, or represents that its use would not infringe privately owned rights.
 Reference herein to any specific commercial product, process, or service by trade name, trademark, manufacturer, or otherwise does not necessarily constitute or imply its endorsement, recommendation, or favoring by the United States Government or any agency thereof, or Battelle Memorial Institute. The views and opinions of authors expressed herein do not necessarily state or reflect those of the United States Government or any agency thereof.
 
-   <div align=center>
+   <div>
    <pre style="align-text:center;font-size:10pt">
    PACIFIC NORTHWEST NATIONAL LABORATORY
    operated by
    BATTELLE
    for the
    UNITED STATES DEPARTMENT OF ENERGY
    under Contract DE-AC05-76RL01830
```

#### html2text {}

```diff
@@ -41,127 +41,126 @@
 and `dynamic` distinctions no longer exist. All hypergraphs use the same
 underlying data structure, supported by Pandas dataFrames. All hypergraphs
 maintain a `state_dict` to avoid repeating computations. 1. Methods for adding
 nodes and hyperedges are currently not supported. 1. The `nwhy` optimizations
 are no longer supported. 1. Entity and EntitySet classes are being moved to the
 background. The Hypergraph constructor does not accept either. Tutorials
 Available for Colab ============================= Google Colab ------------
-_[_O_p_e_n_ _I_n_ _C_o_l_a_b_]_B_a_s_i_c_ _1_ _-_ _H_N_X_ _B_a_s_i_c_s_ _[_O_p_e_n_ _I_n_ _C_o_l_a_b_]_B_a_s_i_c_ _2_ _-_ _V_i_s_u_a_l_i_z_a_t_i_o_n
-_M_e_t_h_o_d_s_ _[_O_p_e_n_ _I_n_ _C_o_l_a_b_]_B_a_s_i_c_ _3_ _-_ _L_e_s_M_i_s_ _C_a_s_e_ _S_t_u_d_y_ _[_O_p_e_n_ _I_n_ _C_o_l_a_b_]_B_a_s_i_c_ _4_ _-
-_L_e_s_M_i_s_ _V_i_s_u_a_l_i_z_a_t_i_o_n_s_-_B_o_o_k_ _T_o_u_r_ _[_O_p_e_n_ _I_n_ _C_o_l_a_b_]_B_a_s_i_c_ _5_ _-_ _H_N_X_ _a_t_t_r_i_b_u_t_e_d
-_h_y_p_e_r_g_r_a_p_h_ _[_O_p_e_n_ _I_n_ _C_o_l_a_b_]_B_a_s_i_c_ _6_ _-_ _H_y_p_e_r_g_r_a_p_h_ _A_r_i_t_h_m_e_t_i_c_._i_p_y_n_b_ Jupyter
-Notebooks ----------------- Additional tutorials that can be run as Jupyter
-Notebooks are found under [tutorials](./tutorials). Installation
+_[_O_p_e_n_ _I_n_ _C_o_l_a_b_]_B_a_s_i_c_ _1_ _-_ _H_N_X_ _B_a_s_i_c_s_ 
+_[_O_p_e_n_ _I_n_ _C_o_l_a_b_]_B_a_s_i_c_ _2_ _-_ _V_i_s_u_a_l_i_z_a_t_i_o_n_ _M_e_t_h_o_d_s_ 
+_[_O_p_e_n_ _I_n_ _C_o_l_a_b_]_B_a_s_i_c_ _3_ _-_ _L_e_s_M_i_s_ _C_a_s_e_ _S_t_u_d_y_ 
+_[_O_p_e_n_ _I_n_ _C_o_l_a_b_]_B_a_s_i_c_ _4_ _-_ _L_e_s_M_i_s_ _V_i_s_u_a_l_i_z_a_t_i_o_n_s_-_B_o_o_k_ _T_o_u_r_ 
+_[_O_p_e_n_ _I_n_ _C_o_l_a_b_]_B_a_s_i_c_ _5_ _-_ _H_N_X_ _a_t_t_r_i_b_u_t_e_d_ _h_y_p_e_r_g_r_a_p_h_ 
+_[_O_p_e_n_ _I_n_ _C_o_l_a_b_]_B_a_s_i_c_ _6_ _-_ _H_y_p_e_r_g_r_a_p_h_ _A_r_i_t_h_m_e_t_i_c_._i_p_y_n_b_ 
+Jupyter Notebooks ----------------- Additional tutorials that can be run as
+Jupyter Notebooks are found under [tutorials](./tutorials). Installation
 ==================== The recommended installation method for most users is to
 create a virtual environment and install HyperNetX from PyPi. HyperNetX may be
-cloned or forked from [Github](https://github.com/pnnl/HyperNetX).
+cloned or forked from [GitHub](https://github.com/pnnl/HyperNetX).
 Prerequisites ------------- HyperNetX officially supports Python 3.8, 3.9, 3.10
 and 3.11. Create a virtual environment ---------------------------- ### Using
 venv ```shell python -m venv venv-hnx source venv-hnx/bin/activate ``` ###
 Using Anaconda ```shell conda create -n venv-hnx python=3.11 -y conda activate
 venv-hnx ``` ### Using virtualenv ```shell virtualenv venv-hnx source venv-hnx/
 bin/activate ``` ### For Windows Users On both Windows PowerShell or Command
 Prompt, you can use the following command to activate your virtual environment:
 ```shell .\env-hnx\Scripts\activate ``` To deactivate your environment, use:
 ```shell .\env-hnx\Scripts\deactivate ``` Installing HyperNetX
 ==================== Regardless of how you install HyperNetX, ensure that your
-environment is activated and that you are running Python >=3.8. Installing from
-PyPi -------------------- ```shell pip install hypernetx ``` Installing from
-Source ---------------------- Ensure that you have [git](https://git-scm.com/
-book/en/v2/Getting-Started-Installing-Git) installed. ```shell git clone https:
-//github.com/pnnl/HyperNetX.git cd HyperNetX # Create a virtual environment
-make venv source venv-hnx/bin/activate # install required dependencies make
-install ``` Development =========== Install an editable version ``` pip install
--e . ``` Install additional dependencies to support testing and jupyter
-notebooks: ``` pip install -r requirements.txt ``` You can also install all
-these requirements in one Make target: ``` make install ``` Poetry ====== This
-library uses [Poetry](https://python-poetry.org/docs/) to manage dependencies
-and packaging. Poetry can also be used to manage your environment for
-development. Prerequisites ------------- * [Install Poetry](https://python-
-poetry.org/docs/#installation) Configure Poetry ---------------- [Configure
-your Poetry](https://python-poetry.org/docs/configuration/) to create the
-virtual environment in your project directory: ``` poetry config
+environment is activated and that you are running Python >=3.10. Installing
+from PyPi -------------------- ```shell pip install hypernetx ``` Installing
+from Source ---------------------- Ensure that you have [git](https://git-
+scm.com/book/en/v2/Getting-Started-Installing-Git) installed. ```shell git
+clone https://github.com/pnnl/HyperNetX.git cd HyperNetX # Create a virtual
+environment make venv source venv-hnx/bin/activate # install required
+dependencies make install ``` Development =========== Install an editable
+version ``` pip install -e . ``` Install additional dependencies to support
+testing and jupyter notebooks: ``` pip install -r requirements.txt ``` You can
+also install all these requirements in one Make target: ``` make install ```
+Poetry ====== This library uses [Poetry](https://python-poetry.org/docs/) to
+manage dependencies and packaging. Poetry can also be used to manage your
+environment for development. Prerequisites ------------- * [Install Poetry]
+(https://python-poetry.org/docs/#installation) Configure Poetry ---------------
+- [Configure your Poetry](https://python-poetry.org/docs/configuration/) to
+create the virtual environment in your project directory: ``` poetry config
 virtualenvs.in-project true # check the poetry configuration poetry config --
 list ``` Set up virtual environment ---------------------------- Create and
 activate a virtual environment. ``` poetry shell ``` NOTE: If you plan to use
 Poetry to manage your virtual environment, you can activate the virtual
 environment using poerty: `poetry shell`. Another option is to directly Install
 required dependencies and HyperNetX in editable mode. ``` poetry install ```
 Install support for testing ----------------------------- > â¹ï¸ **NOTE:**
 This project has a pytest configuration file named 'pytest.ini'. By default,
 pytest will use those configuration settings to run tests. ```shell poetry
-install --with test # run tests python -m pytest # run tests and show coverage
-report python -m pytest --cov=hypernetx # Generate an HTML code coverage report
-and view it on a browser coverage html open htmlcov/index.html ``` Install
-support for tutorials ----------------------------- ``` poetry install --with
-tutorials # open Jupyter notebooks in a browser make tutorials ``` Code Quality
------------- HyperNetX uses a number of tools to maintain code quality: *
-Pylint * Black Before using these tools, ensure that you install Pylint in your
-environment: ``` poetry install --with lint ``` Pylint ------ [Pylint](https://
-pylint.pycqa.org/en/latest/index.html) is a static code analyzer for Python-
-based projects. From the [Pylint docs](https://pylint.pycqa.org/en/latest/
-index.html#what-is-pylint): > Pylint analyses your code without actually
-running it. It checks for errors, enforces a coding standard, looks for code
-smells, and can make suggestions about how the code could be refactored. Pylint
-can infer actual values from your code using its internal code representation
-(astroid). If your code is import logging as argparse, Pylint will know that
-argparse.error(...) is in fact a logging call and not an argparse call. To run
-Pylint and view the results of Pylint, run the following command: ```shell
-pylint hypernetx ``` You can also run Pylint on the command line to generate a
-report on the quality of the codebase and save it to a file named "pylint-
-results.txt": ```shell pylint hypernetx --output=pylint-results.txt ``` For
-more information on configuration, see https://pylint.pycqa.org/en/latest/
-user_guide/configuration/index.html Black ----- [Black](https://
-black.readthedocs.io/en/stable/) is a PEP 8 compliant formatter for Python-
-based project. This tool is highly opinionated about how Python should be
-formatted and will automagically reformat your code. ```shell black hypernetx
-``` Documentation ------------- Build and view documentation locally: ```
-poetry install --with docs cd docs make html open docs/build/html/index.html
-``` When editing documentation, you can auto-rebuild the documentation locally
-so that you can view your document changes live on the browser without having
-to rebuild every time you have a change. ``` cd docs make livehtml ``` This
+install --with test # activate your virtual environment created by poetry
+poetry shell # run tests python -m pytest # run tests and show coverage report
+python -m pytest --cov=hypernetx # Generate an HTML code coverage report and
+view it on a browser coverage html open htmlcov/index.html ``` Install support
+for tutorials ----------------------------- ```shell poetry install --with
+tutorials # activate your virtual environment created by poetry poetry shell #
+open Jupyter notebooks in a browser make tutorials ``` Code Quality -----------
+- HyperNetX uses a number of tools to maintain code quality: * Pylint * Black
+Before using these tools, ensure that you install Pylint in your environment:
+```shell poetry install --with lint # activate your virtual environment created
+by poetry poetry shell ``` Pylint ------ [Pylint](https://pylint.pycqa.org/en/
+latest/index.html) is a static code analyzer for Python-based projects. From
+the [Pylint docs](https://pylint.pycqa.org/en/latest/index.html#what-is-
+pylint): > Pylint analyses your code without actually running it. It checks for
+errors, enforces a coding standard, looks for code smells, and can make
+suggestions about how the code could be refactored. Pylint can infer actual
+values from your code using its internal code representation (astroid). If your
+code is import logging as argparse, Pylint will know that argparse.error(...)
+is in fact a logging call and not an argparse call. To run Pylint and view the
+results of Pylint, run the following command: ```shell pylint hypernetx ``` You
+can also run Pylint on the command line to generate a report on the quality of
+the codebase and save it to a file named "pylint-results.txt": ```shell pylint
+hypernetx --output=pylint-results.txt ``` For more information on
+configuration, see https://pylint.pycqa.org/en/latest/user_guide/configuration/
+index.html Black ----- [Black](https://black.readthedocs.io/en/stable/) is a
+PEP 8 compliant formatter for Python-based project. This tool is highly
+opinionated about how Python should be formatted and will automagically
+reformat your code. ```shell black hypernetx ``` Pre-commit --------- Use the
+[pre-commit framework](https://pre-commit.com/) to automatically point out
+issues and resolve those issues before code review. It is highly recommended to
+install pre-commit in your development environment so that issues with your
+code can be found before you submit a pull request. More importantly, using
+pre-commit will automatically format your code changes so that they pass the CI
+build. For example, pre-commit will automatically run the formatter Black on
+your code changes. ```shell pre-commit install # Once installed, pre-commit
+will be triggered every time you make a commit in your environment ```
+Documentation ------------- Build and view documentation locally: ```shell
+poetry install --with docs # activate your virtual environment created by
+poetry poetry shell cd docs make html open docs/build/html/index.html ``` When
+editing documentation, you can auto-rebuild the documentation locally so that
+you can view your document changes live on the browser without having to
+rebuild every time you have a change. ```shell cd docs make livehtml ``` This
 make script will run in the foreground on your terminal. You should see the
 following: ```shell The HTML pages are in docs/html. [I 230324 09:50:48 server:
 335] Serving on http://127.0.0.1:8000 [I 230324 09:50:48 handlers:62] Start
 watching changes [I 230324 09:50:48 handlers:64] Start detecting changes [I
 230324 09:50:54 handlers:135] Browser Connected: http://127.0.0.1:8000/
 install.html [I 230324 09:51:02 handlers:135] Browser Connected: http://
 127.0.0.1:8000/ ``` Click on `http://127.0.0.1:8000/install.html` to open the
 docs on your browser. Since this will auto-rebuild, every time you change a
 document file, it will automatically render on your browser, allowing you to
-verify your document changes. Continuous Integration ======================
-This project runs Continuous Integration (CI) using GitHub Actions. Normally,
-CI runs on pull requests, pushes to certain branches, and other events.
-Maintainers of the GitHub repository can manually trigger CI using [GitHub CLI]
-(https://cli.github.com/). See instructions below on how to manually trigger CI
-on GitHub Actions: ```commandline # login to Github gh auth login --with-token
-< ~/.ssh/tokens/ # Trigger CI gh workflow run ci.yml --repo pnnl/HyperNetX --
-ref --field triggeredBy="" # Get the status of the workflow gh run list --
-workflow=ci.yml --repo pnnl/HyperNetX ``` Versioning ========== This project
-uses [`commitizen`](https://github.com/commitizen-tools/commitizen) to manage
-versioning. The files where "version" will be updated are listed in the
-'.cz.toml' file. To create a new version and the associated tag, run the
-following commands: ```shell # Install commitizen tool to environment pip
-install commitizen # Updates version; values for '--increment' can be MAJOR,
-MINOR, or PATCH # Autocreates a tag and commit for the updated version cz bump
---increment MAJOR --dry-run cz bump --increment MAJOR ``` Notice ====== This
-material was prepared as an account of work sponsored by an agency of the
-United States Government. Neither the United States Government nor the United
-States Department of Energy, nor Battelle, nor any of their employees, nor any
-jurisdiction or organization that has cooperated in the development of these
-materials, makes any warranty, express or implied, or assumes any legal
-liability or responsibility for the accuracy, completeness, or usefulness or
-any information, apparatus, product, software, or process disclosed, or
-represents that its use would not infringe privately owned rights. Reference
-herein to any specific commercial product, process, or service by trade name,
-trademark, manufacturer, or otherwise does not necessarily constitute or imply
-its endorsement, recommendation, or favoring by the United States Government or
-any agency thereof, or Battelle Memorial Institute. The views and opinions of
-authors expressed herein do not necessarily state or reflect those of the
-United States Government or any agency thereof.
-                      PACIFIC NORTHWEST NATIONAL LABORATORY
-                                   operated by
-                                     BATTELLE
-                                     for the
-                        UNITED STATES DEPARTMENT OF ENERGY
-                         under Contract DE-AC05-76RL01830
+verify your document changes. Notice ====== This material was prepared as an
+account of work sponsored by an agency of the United States Government. Neither
+the United States Government nor the United States Department of Energy, nor
+Battelle, nor any of their employees, nor any jurisdiction or organization that
+has cooperated in the development of these materials, makes any warranty,
+express or implied, or assumes any legal liability or responsibility for the
+accuracy, completeness, or usefulness or any information, apparatus, product,
+software, or process disclosed, or represents that its use would not infringe
+privately owned rights. Reference herein to any specific commercial product,
+process, or service by trade name, trademark, manufacturer, or otherwise does
+not necessarily constitute or imply its endorsement, recommendation, or
+favoring by the United States Government or any agency thereof, or Battelle
+Memorial Institute. The views and opinions of authors expressed herein do not
+necessarily state or reflect those of the United States Government or any
+agency thereof.
+   PACIFIC NORTHWEST NATIONAL LABORATORY
+   operated by
+   BATTELLE
+   for the
+   UNITED STATES DEPARTMENT OF ENERGY
+   under Contract DE-AC05-76RL01830
 License ======= Released under the 3-Clause BSD license (see License.rst)
```

### Comparing `hypernetx-2.3.1/hypernetx/algorithms/__init__.py` & `hypernetx-2.3.2/hypernetx/algorithms/__init__.py`

 * *Files identical despite different names*

### Comparing `hypernetx-2.3.1/hypernetx/algorithms/contagion.py` & `hypernetx-2.3.2/hypernetx/algorithms/contagion.py`

 * *Files identical despite different names*

### Comparing `hypernetx-2.3.1/hypernetx/algorithms/generative_models.py` & `hypernetx-2.3.2/hypernetx/algorithms/generative_models.py`

 * *Files identical despite different names*

### Comparing `hypernetx-2.3.1/hypernetx/algorithms/homology_mod2.py` & `hypernetx-2.3.2/hypernetx/algorithms/homology_mod2.py`

 * *Files identical despite different names*

### Comparing `hypernetx-2.3.1/hypernetx/algorithms/hypergraph_modularity.py` & `hypernetx-2.3.2/hypernetx/algorithms/hypergraph_modularity.py`

 * *Files identical despite different names*

### Comparing `hypernetx-2.3.1/hypernetx/algorithms/laplacians_clustering.py` & `hypernetx-2.3.2/hypernetx/algorithms/laplacians_clustering.py`

 * *Files identical despite different names*

### Comparing `hypernetx-2.3.1/hypernetx/algorithms/s_centrality_measures.py` & `hypernetx-2.3.2/hypernetx/algorithms/s_centrality_measures.py`

 * *Files identical despite different names*

### Comparing `hypernetx-2.3.1/hypernetx/classes/factory.py` & `hypernetx-2.3.2/hypernetx/classes/factory.py`

 * *Files identical despite different names*

### Comparing `hypernetx-2.3.1/hypernetx/classes/hyp_view.py` & `hypernetx-2.3.2/hypernetx/classes/hyp_view.py`

 * *Files identical despite different names*

### Comparing `hypernetx-2.3.1/hypernetx/classes/hypergraph.py` & `hypernetx-2.3.2/hypernetx/classes/hypergraph.py`

 * *Files identical despite different names*

### Comparing `hypernetx-2.3.1/hypernetx/classes/incidence_store.py` & `hypernetx-2.3.2/hypernetx/classes/incidence_store.py`

 * *Files identical despite different names*

### Comparing `hypernetx-2.3.1/hypernetx/classes/property_store.py` & `hypernetx-2.3.2/hypernetx/classes/property_store.py`

 * *Files identical despite different names*

### Comparing `hypernetx-2.3.1/hypernetx/drawing/rubber_band.py` & `hypernetx-2.3.2/hypernetx/drawing/rubber_band.py`

 * *Files identical despite different names*

### Comparing `hypernetx-2.3.1/hypernetx/drawing/two_column.py` & `hypernetx-2.3.2/hypernetx/drawing/two_column.py`

 * *Files identical despite different names*

### Comparing `hypernetx-2.3.1/hypernetx/drawing/util.py` & `hypernetx-2.3.2/hypernetx/drawing/util.py`

 * *Files identical despite different names*

### Comparing `hypernetx-2.3.1/hypernetx/reports/descriptive_stats.py` & `hypernetx-2.3.2/hypernetx/reports/descriptive_stats.py`

 * *Files identical despite different names*

### Comparing `hypernetx-2.3.1/hypernetx/utils/__init__.py` & `hypernetx-2.3.2/hypernetx/utils/__init__.py`

 * *Files identical despite different names*

### Comparing `hypernetx-2.3.1/hypernetx/utils/decorators.py` & `hypernetx-2.3.2/hypernetx/utils/decorators.py`

 * *Files identical despite different names*

### Comparing `hypernetx-2.3.1/hypernetx/utils/extras.py` & `hypernetx-2.3.2/hypernetx/utils/extras.py`

 * *Files identical despite different names*

### Comparing `hypernetx-2.3.1/hypernetx/utils/log.py` & `hypernetx-2.3.2/hypernetx/utils/log.py`

 * *Files identical despite different names*

### Comparing `hypernetx-2.3.1/hypernetx/utils/toys/ChungLuTransmissionData.csv` & `hypernetx-2.3.2/hypernetx/utils/toys/ChungLuTransmissionData.csv`

 * *Files identical despite different names*

### Comparing `hypernetx-2.3.1/hypernetx/utils/toys/GoT.pkl` & `hypernetx-2.3.2/hypernetx/utils/toys/GoT.pkl`

 * *Files identical despite different names*

### Comparing `hypernetx-2.3.1/hypernetx/utils/toys/HarryPotterHypergraph.p` & `hypernetx-2.3.2/hypernetx/utils/toys/HarryPotterHypergraph.p`

 * *Files identical despite different names*

### Comparing `hypernetx-2.3.1/hypernetx/utils/toys/HarryPotter_Characters.csv` & `hypernetx-2.3.2/hypernetx/utils/toys/HarryPotter_Characters.csv`

 * *Files identical despite different names*

### Comparing `hypernetx-2.3.1/hypernetx/utils/toys/disGene.txt` & `hypernetx-2.3.2/hypernetx/utils/toys/disGene.txt`

 * *Files identical despite different names*

### Comparing `hypernetx-2.3.1/hypernetx/utils/toys/harrypotter.py` & `hypernetx-2.3.2/hypernetx/utils/toys/harrypotter.py`

 * *Files identical despite different names*

### Comparing `hypernetx-2.3.1/hypernetx/utils/toys/lesmis.py` & `hypernetx-2.3.2/hypernetx/utils/toys/lesmis.py`

 * *Files identical despite different names*

### Comparing `hypernetx-2.3.1/hypernetx/utils/toys/transmission_problem.py` & `hypernetx-2.3.2/hypernetx/utils/toys/transmission_problem.py`

 * *Files identical despite different names*

### Comparing `hypernetx-2.3.1/pyproject.toml` & `hypernetx-2.3.2/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "hypernetx"
-version = "2.3.1"
+version = "2.3.2"
 description = "HyperNetX is a Python library for the creation and study of hypergraphs."
 authors = ["Brenda Praggastis <Brenda.Praggastis@pnnl.gov>", "Dustin Arendt <dustin.arendt@pnnl.gov>",
     "Sinan Aksoy <sinan.aksoy@pnnl.gov>", "Emilie Purvine <Emilie.Purvine@pnnl.gov>",
     "Cliff Joslyn <Cliff.Joslyn@pnnl.gov>"]
 license = "3-Clause BSD license"
 readme = "README.md"
 homepage = "https://pypi.org/project/hypernetx/"
@@ -18,21 +18,21 @@
     {include = "hypernetx/drawing"},
     {include = "hypernetx/reports"},
     {include = "hypernetx/utils"},
     {include = "hypernetx/utils/toys"},
 ]
 
 [tool.poetry.dependencies]
-python = "^3.10,<=3.12.3"
+python = ">=3.10,<4.0.0"
 networkx = ">=3.3"
 pandas = ">=2.2.2"
 scikit-learn = ">=1.4.2"
 celluloid = ">=0.2.0"
 igraph = ">=0.11.4"
-decorator = "^5.1.1"
+decorator = ">=5.1.1"
 
 [tool.poetry.group.widget]
 optional = true
 [tool.poetry.group.widget.dependencies]
 jupyter-contrib-nbextensions = "^0.7.0"
 ipywidgets = "7.7.5"
 notebook = "6.4.12"
```

### Comparing `hypernetx-2.3.1/PKG-INFO` & `hypernetx-2.3.2/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,24 +1,24 @@
 Metadata-Version: 2.1
 Name: hypernetx
-Version: 2.3.1
+Version: 2.3.2
 Summary: HyperNetX is a Python library for the creation and study of hypergraphs.
 Home-page: https://pypi.org/project/hypernetx/
 License: 3-Clause BSD license
 Keywords: hypergraphs
 Author: Brenda Praggastis
 Author-email: Brenda.Praggastis@pnnl.gov
-Requires-Python: >=3.10,<=3.12.3
+Requires-Python: >=3.10,<4.0.0
 Classifier: License :: Other/Proprietary License
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: Python :: 3.12
 Requires-Dist: celluloid (>=0.2.0)
-Requires-Dist: decorator (>=5.1.1,<6.0.0)
+Requires-Dist: decorator (>=5.1.1)
 Requires-Dist: igraph (>=0.11.4)
 Requires-Dist: networkx (>=3.3)
 Requires-Dist: pandas (>=2.2.2)
 Requires-Dist: scikit-learn (>=1.4.2)
 Project-URL: Documentation, https://hypernetx.readthedocs.io/en/latest/
 Project-URL: Repository, https://github.com/pnnl/HyperNetX
 Description-Content-Type: text/markdown
@@ -93,58 +93,58 @@
 ------------
 
 
 <a href="https://colab.research.google.com/github/pnnl/HyperNetX/blob/master/tutorials/basic/Basic%201%20-%20HNX%20Basics.ipynb" target="_blank">
   <img src="https://colab.research.google.com/assets/colab-badge.svg" alt="Open In Colab"/>
     <span >Basic 1 - HNX Basics</span>
 </a>
-</br>
+<br>
 
 <a href="https://colab.research.google.com/github/pnnl/HyperNetX/blob/master/tutorials/basic/Basic%202%20-%20Visualization%20Methods.ipynb" target="_blank">
   <img src="https://colab.research.google.com/assets/colab-badge.svg" alt="Open In Colab"/>
     <span >Basic 2 - Visualization Methods</span>
 </a>
-</br>
+<br>
 
 <a href="https://colab.research.google.com/github/pnnl/HyperNetX/blob/master/tutorials/basic/Basic%203%20-%20LesMis%20Case%20Study.ipynb" target="_blank">
   <img src="https://colab.research.google.com/assets/colab-badge.svg" alt="Open In Colab"/>
     <span >Basic 3 - LesMis Case Study</span>
 </a>
-</br>
+<br>
 
 <a href="https://colab.research.google.com/github/pnnl/HyperNetX/blob/master/tutorials/basic/Basic%204%20-%20LesMis%20Visualizations-BookTour.ipynb" target="_blank">
   <img src="https://colab.research.google.com/assets/colab-badge.svg" alt="Open In Colab"/>
     <span >Basic 4 - LesMis Visualizations-Book Tour</span>
 </a>
-</br>
+<br>
 
 <a href="https://colab.research.google.com/github/pnnl/HyperNetX/blob/master/tutorials/basic/Basic%205%20-%20HNX%20attributed%20hypergraph.ipynb" target="_blank">
   <img src="https://colab.research.google.com/assets/colab-badge.svg" alt="Open In Colab"/>
     <span >Basic 5 - HNX attributed hypergraph</span>
 </a>
-</br>
+<br>
 
 <a href="https://colab.research.google.com/github/pnnl/HyperNetX/blob/master/tutorials/basic/Basic%206%20-%20Hypergraph%20Arithmetic.ipynb" target="_blank">
   <img src="https://colab.research.google.com/assets/colab-badge.svg" alt="Open In Colab"/>
     <span >Basic 6 - Hypergraph Arithmetic.ipynb</span>
 </a>
-</br>
+<br>
 
 
 Jupyter Notebooks
 -----------------
 
 Additional tutorials that can be run as Jupyter Notebooks are found under [tutorials](./tutorials).
 
 Installation
 ====================
 
 The recommended installation method for most users is to create a virtual environment and install HyperNetX from PyPi.
 
-HyperNetX may be cloned or forked from [Github](https://github.com/pnnl/HyperNetX).
+HyperNetX may be cloned or forked from [GitHub](https://github.com/pnnl/HyperNetX).
 
 Prerequisites
 -------------
 HyperNetX officially supports Python 3.8, 3.9, 3.10 and 3.11.
 
 Create a virtual environment
 ----------------------------
@@ -189,15 +189,15 @@
 ```shell
 .\env-hnx\Scripts\deactivate
 ```
 
 Installing HyperNetX
 ====================
 
-Regardless of how you install HyperNetX, ensure that your environment is activated and that you are running Python >=3.8.
+Regardless of how you install HyperNetX, ensure that your environment is activated and that you are running Python >=3.10.
 
 
 Installing from PyPi
 --------------------
 
 ```shell
 pip install hypernetx
@@ -282,46 +282,54 @@
 -----------------------------
 
 > ℹ️ **NOTE:** This project has a pytest configuration file named 'pytest.ini'. By default, pytest will use those configuration settings to run tests.
 
 ```shell
 poetry install --with test
 
+# activate your virtual environment created by poetry
+poetry shell
+
 # run tests
 python -m pytest
 
 # run tests and show coverage report
 python -m pytest --cov=hypernetx
 
 # Generate an HTML code coverage report and view it on a browser
 coverage html
 open htmlcov/index.html
 ```
 
 Install support for tutorials
 -----------------------------
 
-```
+```shell
 poetry install --with tutorials
 
+# activate your virtual environment created by poetry
+poetry shell
+
 # open Jupyter notebooks in a browser
 make tutorials
 ```
 
 Code Quality
 ------------
 HyperNetX uses a number of tools to maintain code quality:
 
 * Pylint
 * Black
 
 Before using these tools, ensure that you install Pylint in your environment:
 
-```
+```shell
 poetry install --with lint
+# activate your virtual environment created by poetry
+poetry shell
 ```
 
 Pylint
 ------
 
 [Pylint](https://pylint.pycqa.org/en/latest/index.html) is a static code analyzer for Python-based projects. From the [Pylint docs](https://pylint.pycqa.org/en/latest/index.html#what-is-pylint):
 
@@ -346,30 +354,47 @@
 [Black](https://black.readthedocs.io/en/stable/) is a PEP 8 compliant formatter for Python-based project. This tool is highly opinionated about how Python should be formatted and will automagically reformat your code.
 
 
 ```shell
 black hypernetx
 ```
 
+Pre-commit
+---------
+
+Use the [pre-commit framework](https://pre-commit.com/) to automatically point out issues and resolve those issues before code review.
+It is highly recommended to install pre-commit in your development environment so that issues with your code can be found before you submit a
+pull request. More importantly, using pre-commit will automatically format your code changes so that they pass the CI build. For example, pre-commit will
+automatically run the formatter Black on your code changes.
+
+```shell
+pre-commit install
+
+# Once installed, pre-commit will be triggered every time you make a commit in your environment
+```
+
 Documentation
 -------------
 
 Build and view documentation locally:
 
-```
+```shell
 poetry install --with docs
+# activate your virtual environment created by poetry
+poetry shell
+
 cd docs
 make html
 open docs/build/html/index.html
 ```
 
 When editing documentation, you can auto-rebuild the documentation locally so that you can view your document changes
 live on the browser without having to rebuild every time you have a change.
 
-```
+```shell
 cd docs
 make livehtml
 ```
 
 This make script will run in the foreground on your terminal. You should see the following:
 
 ```shell
@@ -381,57 +406,20 @@
 [I 230324 09:51:02 handlers:135] Browser Connected: http://127.0.0.1:8000/
 ```
 
 Click on `http://127.0.0.1:8000/install.html` to open the docs on your browser. Since this will auto-rebuild, every time
 you change a document file, it will automatically render on your browser, allowing you to verify your document changes.
 
 
-Continuous Integration
-======================
-
-This project runs Continuous Integration (CI) using GitHub Actions. Normally, CI runs
-on pull requests, pushes to certain branches, and other events.
-
-Maintainers of the GitHub repository can manually trigger CI using [GitHub CLI](https://cli.github.com/). See instructions below on how to manually trigger CI on GitHub Actions:
-
-```commandline
-# login to Github
-gh auth login --with-token <  ~/.ssh/tokens/<path to my personal access token>
-
-# Trigger CI
-gh workflow run ci.yml --repo pnnl/HyperNetX --ref <name of branch that you want CI to run on> --field triggeredBy="<Your name>"
-
-# Get the status of the workflow
-gh run list --workflow=ci.yml --repo pnnl/HyperNetX
-```
-
-
-Versioning
-==========
-
-This project uses [`commitizen`](https://github.com/commitizen-tools/commitizen) to manage versioning.
-The files where "version" will be updated are listed in the '.cz.toml' file. To create a new version and the associated tag,
-run the following commands:
-
-```shell
-# Install commitizen tool to environment
-pip install commitizen
-
-# Updates version; values for '--increment' can be MAJOR, MINOR, or PATCH
-# Autocreates a tag and commit for the updated version
-cz bump  --increment MAJOR  --dry-run
-cz bump  --increment MAJOR
-```
-
 Notice
 ======
 This material was prepared as an account of work sponsored by an agency of the United States Government.  Neither the United States Government nor the United States Department of Energy, nor Battelle, nor any of their employees, nor any jurisdiction or organization that has cooperated in the development of these materials, makes any warranty, express or implied, or assumes any legal liability or responsibility for the accuracy, completeness, or usefulness or any information, apparatus, product, software, or process disclosed, or represents that its use would not infringe privately owned rights.
 Reference herein to any specific commercial product, process, or service by trade name, trademark, manufacturer, or otherwise does not necessarily constitute or imply its endorsement, recommendation, or favoring by the United States Government or any agency thereof, or Battelle Memorial Institute. The views and opinions of authors expressed herein do not necessarily state or reflect those of the United States Government or any agency thereof.
 
-   <div align=center>
+   <div>
    <pre style="align-text:center;font-size:10pt">
    PACIFIC NORTHWEST NATIONAL LABORATORY
    operated by
    BATTELLE
    for the
    UNITED STATES DEPARTMENT OF ENERGY
    under Contract DE-AC05-76RL01830
```

