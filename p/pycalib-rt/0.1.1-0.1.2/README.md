# Comparing `tmp/pycalib_rt-0.1.1.tar.gz` & `tmp/pycalib_rt-0.1.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pycalib_rt-0.1.1.tar", last modified: Tue May 28 15:56:49 2024, max compression
+gzip compressed data, was "pycalib_rt-0.1.2.tar", last modified: Wed May 29 10:49:45 2024, max compression
```

## Comparing `pycalib_rt-0.1.1.tar` & `pycalib_rt-0.1.2.tar`

### file list

```diff
@@ -1,30 +1,30 @@
-drwxrwxrwx   0        0        0        0 2024-05-28 15:56:49.429202 pycalib_rt-0.1.1/
--rw-rw-rw-   0        0        0     1088 2023-10-25 16:04:22.000000 pycalib_rt-0.1.1/LICENSE
--rw-rw-rw-   0        0        0     3074 2024-05-28 15:56:49.426202 pycalib_rt-0.1.1/PKG-INFO
--rw-rw-rw-   0        0        0     2437 2024-05-28 15:54:17.000000 pycalib_rt-0.1.1/README.md
-drwxrwxrwx   0        0        0        0 2024-05-28 15:56:49.357295 pycalib_rt-0.1.1/calib_rt/
--rw-rw-rw-   0        0        0      286 2024-05-28 08:32:19.000000 pycalib_rt-0.1.1/calib_rt/__init__.py
--rw-rw-rw-   0        0        0     3170 2024-05-28 03:25:49.000000 pycalib_rt-0.1.1/calib_rt/calib_rt.py
-drwxrwxrwx   0        0        0        0 2024-05-28 15:56:49.399311 pycalib_rt-0.1.1/calib_rt/data/
--rw-rw-rw-   0        0        0   737338 2023-10-25 16:04:22.000000 pycalib_rt-0.1.1/calib_rt/data/20200505_Evosep_100SPD_SG06-16_MLHeLa_100ng_py8_S2-C1_1_2731.d.npz
--rw-rw-rw-   0        0        0   472346 2023-10-25 16:04:22.000000 pycalib_rt-0.1.1/calib_rt/data/20200505_Evosep_200SPD_SG06-16_MLHeLa_200ng_py8_S3-A1_1_2737.d.npz
--rw-rw-rw-   0        0        0    72650 2023-10-25 16:04:22.000000 pycalib_rt-0.1.1/calib_rt/data/20211101_PRO2_LS_04_MA_HeLaSCS_0.2_ngHS_GE2_1_1408.d.npz
--rw-rw-rw-   0        0        0  1958218 2023-10-25 16:04:22.000000 pycalib_rt-0.1.1/calib_rt/data/20211103_PRO2_LS_01_MA_HeLa_200_SDC_NS_RE2_1_1418.d.npz
--rw-rw-rw-   0        0        0    59146 2023-10-25 16:04:22.000000 pycalib_rt-0.1.1/calib_rt/data/20220714_10ngK562_ZI_500ul60C3cm5min_P1-C1_1_9675.d.npz
--rw-rw-rw-   0        0        0   142762 2023-10-25 16:04:22.000000 pycalib_rt-0.1.1/calib_rt/data/CMs_Subject3_Lvmid_G10_BG11_1_7560.d.npz
--rw-rw-rw-   0        0        0    50234 2023-10-25 16:04:22.000000 pycalib_rt-0.1.1/calib_rt/data/SC_HeLa_10min1_Slot1-9_1_807.d.npz
--rw-rw-rw-   0        0        0    29994 2023-10-25 16:04:22.000000 pycalib_rt-0.1.1/calib_rt/data/SC_HeLa_15min1_Slot1-7_1_805.d.npz
--rw-rw-rw-   0        0        0   855754 2023-10-25 16:04:22.000000 pycalib_rt-0.1.1/calib_rt/data/fmeierab_T190525_CLL_diaPASEF_04_1979.d.npz
--rw-rw-rw-   0        0        0   761146 2023-10-25 16:04:22.000000 pycalib_rt-0.1.1/calib_rt/data/fmeierab_T190525_CLL_diaPASEF_40_1965.d.npz
--rw-rw-rw-   0        0        0     4662 2024-05-28 03:25:49.000000 pycalib_rt-0.1.1/calib_rt/datasets.py
--rw-rw-rw-   0        0        0     2554 2024-05-28 07:40:19.000000 pycalib_rt-0.1.1/calib_rt/regression.py
--rw-rw-rw-   0        0        0     3200 2024-05-28 03:25:49.000000 pycalib_rt-0.1.1/calib_rt/screen.py
--rw-rw-rw-   0        0        0     1113 2024-05-28 07:40:14.000000 pycalib_rt-0.1.1/calib_rt/utils.py
-drwxrwxrwx   0        0        0        0 2024-05-28 15:56:49.423694 pycalib_rt-0.1.1/pycalib_rt.egg-info/
--rw-rw-rw-   0        0        0     3074 2024-05-28 15:56:49.000000 pycalib_rt-0.1.1/pycalib_rt.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      960 2024-05-28 15:56:49.000000 pycalib_rt-0.1.1/pycalib_rt.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-05-28 15:56:49.000000 pycalib_rt-0.1.1/pycalib_rt.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       76 2024-05-28 15:56:49.000000 pycalib_rt-0.1.1/pycalib_rt.egg-info/requires.txt
--rw-rw-rw-   0        0        0        9 2024-05-28 15:56:49.000000 pycalib_rt-0.1.1/pycalib_rt.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2024-05-28 15:56:49.430202 pycalib_rt-0.1.1/setup.cfg
--rw-rw-rw-   0        0        0     1119 2024-05-28 15:54:25.000000 pycalib_rt-0.1.1/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-29 10:49:45.175917 pycalib_rt-0.1.2/
+-rw-r--r--   0 runner    (1001) docker     (127)     1067 2024-05-29 10:49:42.000000 pycalib_rt-0.1.2/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)     2835 2024-05-29 10:49:45.175917 pycalib_rt-0.1.2/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     2368 2024-05-29 10:49:42.000000 pycalib_rt-0.1.2/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-29 10:49:45.167917 pycalib_rt-0.1.2/calib_rt/
+-rw-r--r--   0 runner    (1001) docker     (127)      273 2024-05-29 10:49:42.000000 pycalib_rt-0.1.2/calib_rt/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3069 2024-05-29 10:49:42.000000 pycalib_rt-0.1.2/calib_rt/calib_rt.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-29 10:49:45.171918 pycalib_rt-0.1.2/calib_rt/data/
+-rw-r--r--   0 runner    (1001) docker     (127)   737338 2024-05-29 10:49:42.000000 pycalib_rt-0.1.2/calib_rt/data/20200505_Evosep_100SPD_SG06-16_MLHeLa_100ng_py8_S2-C1_1_2731.d.npz
+-rw-r--r--   0 runner    (1001) docker     (127)   472346 2024-05-29 10:49:42.000000 pycalib_rt-0.1.2/calib_rt/data/20200505_Evosep_200SPD_SG06-16_MLHeLa_200ng_py8_S3-A1_1_2737.d.npz
+-rw-r--r--   0 runner    (1001) docker     (127)    72650 2024-05-29 10:49:42.000000 pycalib_rt-0.1.2/calib_rt/data/20211101_PRO2_LS_04_MA_HeLaSCS_0.2_ngHS_GE2_1_1408.d.npz
+-rw-r--r--   0 runner    (1001) docker     (127)  1958218 2024-05-29 10:49:42.000000 pycalib_rt-0.1.2/calib_rt/data/20211103_PRO2_LS_01_MA_HeLa_200_SDC_NS_RE2_1_1418.d.npz
+-rw-r--r--   0 runner    (1001) docker     (127)    59146 2024-05-29 10:49:42.000000 pycalib_rt-0.1.2/calib_rt/data/20220714_10ngK562_ZI_500ul60C3cm5min_P1-C1_1_9675.d.npz
+-rw-r--r--   0 runner    (1001) docker     (127)   142762 2024-05-29 10:49:42.000000 pycalib_rt-0.1.2/calib_rt/data/CMs_Subject3_Lvmid_G10_BG11_1_7560.d.npz
+-rw-r--r--   0 runner    (1001) docker     (127)    50234 2024-05-29 10:49:42.000000 pycalib_rt-0.1.2/calib_rt/data/SC_HeLa_10min1_Slot1-9_1_807.d.npz
+-rw-r--r--   0 runner    (1001) docker     (127)    29994 2024-05-29 10:49:42.000000 pycalib_rt-0.1.2/calib_rt/data/SC_HeLa_15min1_Slot1-7_1_805.d.npz
+-rw-r--r--   0 runner    (1001) docker     (127)   855754 2024-05-29 10:49:42.000000 pycalib_rt-0.1.2/calib_rt/data/fmeierab_T190525_CLL_diaPASEF_04_1979.d.npz
+-rw-r--r--   0 runner    (1001) docker     (127)   761146 2024-05-29 10:49:42.000000 pycalib_rt-0.1.2/calib_rt/data/fmeierab_T190525_CLL_diaPASEF_40_1965.d.npz
+-rw-r--r--   0 runner    (1001) docker     (127)     4524 2024-05-29 10:49:42.000000 pycalib_rt-0.1.2/calib_rt/datasets.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2475 2024-05-29 10:49:42.000000 pycalib_rt-0.1.2/calib_rt/regression.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3115 2024-05-29 10:49:42.000000 pycalib_rt-0.1.2/calib_rt/screen.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1075 2024-05-29 10:49:42.000000 pycalib_rt-0.1.2/calib_rt/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-29 10:49:45.175917 pycalib_rt-0.1.2/pycalib_rt.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     2835 2024-05-29 10:49:45.000000 pycalib_rt-0.1.2/pycalib_rt.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      960 2024-05-29 10:49:45.000000 pycalib_rt-0.1.2/pycalib_rt.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-29 10:49:45.000000 pycalib_rt-0.1.2/pycalib_rt.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       76 2024-05-29 10:49:45.000000 pycalib_rt-0.1.2/pycalib_rt.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        9 2024-05-29 10:49:45.000000 pycalib_rt-0.1.2/pycalib_rt.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-29 10:49:45.175917 pycalib_rt-0.1.2/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)      954 2024-05-29 10:49:42.000000 pycalib_rt-0.1.2/setup.py
```

### Comparing `pycalib_rt-0.1.1/LICENSE` & `pycalib_rt-0.1.2/LICENSE`

 * *Ordering differences only*

 * *Files 20% similar despite different names*

```diff
@@ -1,21 +1,21 @@
-MIT License
-
-Copyright (c) 2023 chenghui03
-
-Permission is hereby granted, free of charge, to any person obtaining a copy
-of this software and associated documentation files (the "Software"), to deal
-in the Software without restriction, including without limitation the rights
-to use, copy, modify, merge, publish, distribute, sublicense, and/or sell
-copies of the Software, and to permit persons to whom the Software is
-furnished to do so, subject to the following conditions:
-
-The above copyright notice and this permission notice shall be included in all
-copies or substantial portions of the Software.
-
-THE SOFTWARE IS PROVIDED "AS IS", WITHOUT WARRANTY OF ANY KIND, EXPRESS OR
-IMPLIED, INCLUDING BUT NOT LIMITED TO THE WARRANTIES OF MERCHANTABILITY,
-FITNESS FOR A PARTICULAR PURPOSE AND NONINFRINGEMENT. IN NO EVENT SHALL THE
-AUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER
-LIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING FROM,
-OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN THE
-SOFTWARE.
+MIT License
+
+Copyright (c) 2023 chenghui03
+
+Permission is hereby granted, free of charge, to any person obtaining a copy
+of this software and associated documentation files (the "Software"), to deal
+in the Software without restriction, including without limitation the rights
+to use, copy, modify, merge, publish, distribute, sublicense, and/or sell
+copies of the Software, and to permit persons to whom the Software is
+furnished to do so, subject to the following conditions:
+
+The above copyright notice and this permission notice shall be included in all
+copies or substantial portions of the Software.
+
+THE SOFTWARE IS PROVIDED "AS IS", WITHOUT WARRANTY OF ANY KIND, EXPRESS OR
+IMPLIED, INCLUDING BUT NOT LIMITED TO THE WARRANTIES OF MERCHANTABILITY,
+FITNESS FOR A PARTICULAR PURPOSE AND NONINFRINGEMENT. IN NO EVENT SHALL THE
+AUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER
+LIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING FROM,
+OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN THE
+SOFTWARE.
```

### Comparing `pycalib_rt-0.1.1/PKG-INFO` & `pycalib_rt-0.1.2/README.md`

 * *Files 26% similar despite different names*

```diff
@@ -1,90 +1,71 @@
-Metadata-Version: 2.1
-Name: pycalib_rt
-Version: 0.1.1
-Summary: Calib-RT is designed for RT (retention time) calibration.
-Home-page: https://github.com/chenghui03/Calib_RT/tree/main/
-Author: yichi zhang
-Author-email: kszyc1001@163.com
-Classifier: Programming Language :: Python :: 3
-Classifier: License :: OSI Approved :: MIT License
-Classifier: Operating System :: OS Independent
-Requires-Python: >=3.10
-Description-Content-Type: text/markdown
-License-File: LICENSE
-Requires-Dist: numpy>=1.26.0
-Requires-Dist: pandas>=2.1.1
-Requires-Dist: networkx>=3.1
-Requires-Dist: statsmodels>=0.14.0
-Requires-Dist: scipy>=1.11.3
-
-# Calib-RT
-<p align="left">
-    <img alt="PyPI - Version" src="https://img.shields.io/pypi/v/pycalib_rt?style=flat&label=Calib-RT&color=green">
-    <img title="python version" src="https://img.shields.io/badge/python-3.10-blue" alt="">
-</p>
-
-## Overview
-Calib-RT is an open-source Python software package designed for RT (retention time) calibration. 
-This package provides a flexible and robust solution for achieving accurate RT calibration across various data scales while handling a certain level of noise interference. 
-
-The workflow diagram is below, providing an overview of the process. For a comprehensive and in-depth explanation, please refer to the associated paper for detailed insights and analysis.
-
-<div align=center>
-<img src="https://raw.githubusercontent.com/chenghui03/Calib_RT/93750fced36ee36786e61817d71d6ec5e2c5fdd3/img/workflow.svg" alt="Your Image" width="500">
-</div>
-
-## Installation
-To use `calib_rt`, make sure you have the following dependencies installed:
-- Python (>= 3.10)
-- numpy (>= 1.26.0)
-- pandas (>= 2.1.1)
-- networkx (>= 3.1)
-- statsmodels (>= 0.14.0)
-- scipy (>= 1.11.3)
-
-You can install the `calib_rt` package using pip:
-```bash
-pip install pycalib_rt 
-```
-
-## Usage
-Here is an example of how to use `calib_rt` for RT calibration:
-
-```python
-import calib_rt
-
-# basic information of all built-in datasets 
-calib_rt.RTdatasets.get_datasets_list()  
-         sample_type  datasets_num
-   0   distort_left             2
-   1  distort_right             2
-   2            exp             2
-   3         linear             2
-   4              S             2
-
-# use first of "S" type datasets
-datasets = calib_rt.RTdatasets.get_pandas(sample_type="S",index_in_group=1)
-x = datasets["Spectral library RT"]
-y = datasets["Measured RT"]
-
-# fit and predict
-model = calib_rt.Calib_RT() 
-model.fit(x,y)
-y_pred = model.predict(x)         
-```
-
-## Performance test
-
-<div align=center>
-<img src="https://raw.githubusercontent.com/chenghui03/Calib_RT/main/img/performance-test-1.jpg" alt="Your Image" width="500">
-</div>
-
-Code for performance test is available in the [analysis](https://github.com/chenghui03/Calib_RT/tree/main/analyses).
-For a detailed analysis of the test conclusion, please refer to our paper.
-
-## References
-
-[link of paper]()
-
-## License
-This project is licensed under the MIT License. See the LICENSE file for details.
+# Calib-RT
+<p align="left">
+    <img alt="PyPI - Version" src="https://img.shields.io/pypi/v/pycalib_rt?style=flat&label=pycalib_rt&color=green">
+    <img title="python version" src="https://img.shields.io/badge/python-3.10-blue" alt="">
+</p>
+
+## Overview
+Calib-RT is an open-source Python software package designed for RT (retention time) calibration. 
+This package provides a flexible and robust solution for achieving accurate RT calibration across various data scales while handling a certain level of noise interference. 
+
+The workflow diagram is below, providing an overview of the process. For a comprehensive and in-depth explanation, please refer to the associated paper for detailed insights and analysis.
+
+<div align=center>
+<img src="https://raw.githubusercontent.com/chenghui03/Calib_RT/93750fced36ee36786e61817d71d6ec5e2c5fdd3/img/workflow.svg" alt="Your Image" width="500">
+</div>
+
+## Installation
+To use `calib_rt`, make sure you have the following dependencies installed:
+- Python (>= 3.10)
+- numpy (>= 1.26.0)
+- pandas (>= 2.1.1)
+- networkx (>= 3.1)
+- statsmodels (>= 0.14.0)
+- scipy (>= 1.11.3)
+
+You can install the `calib_rt` package using pip:
+```bash
+pip install pycalib_rt 
+```
+
+## Usage
+Here is an example of how to use `calib_rt` for RT calibration:
+
+```python
+import calib_rt
+
+# basic information of all built-in datasets 
+calib_rt.RTdatasets.get_datasets_list()  
+         sample_type  datasets_num
+   0   distort_left             2
+   1  distort_right             2
+   2            exp             2
+   3         linear             2
+   4              S             2
+
+# use first of "S" type datasets
+datasets = calib_rt.RTdatasets.get_pandas(sample_type="S",index_in_group=1)
+x = datasets["Spectral library RT"]
+y = datasets["Measured RT"]
+
+# fit and predict
+model = calib_rt.Calib_RT() 
+model.fit(x,y)
+y_pred = model.predict(x)         
+```
+
+## Performance test
+
+<div align=center>
+<img src="https://raw.githubusercontent.com/chenghui03/Calib_RT/main/img/performance-test-1.jpg" alt="Your Image" width="500">
+</div>
+
+Code for performance test is available in the [analysis](https://github.com/chenghui03/Calib_RT/tree/main/analyses).
+For a detailed analysis of the test conclusion, please refer to our paper.
+
+## References
+
+[link of paper]()
+
+## License
+This project is licensed under the MIT License. See the LICENSE file for details.
```

### Comparing `pycalib_rt-0.1.1/README.md` & `pycalib_rt-0.1.2/PKG-INFO`

 * *Files 15% similar despite different names*

```diff
@@ -1,71 +1,85 @@
-# Calib-RT
-<p align="left">
-    <img alt="PyPI - Version" src="https://img.shields.io/pypi/v/pycalib_rt?style=flat&label=Calib-RT&color=green">
-    <img title="python version" src="https://img.shields.io/badge/python-3.10-blue" alt="">
-</p>
-
-## Overview
-Calib-RT is an open-source Python software package designed for RT (retention time) calibration. 
-This package provides a flexible and robust solution for achieving accurate RT calibration across various data scales while handling a certain level of noise interference. 
-
-The workflow diagram is below, providing an overview of the process. For a comprehensive and in-depth explanation, please refer to the associated paper for detailed insights and analysis.
-
-<div align=center>
-<img src="https://raw.githubusercontent.com/chenghui03/Calib_RT/93750fced36ee36786e61817d71d6ec5e2c5fdd3/img/workflow.svg" alt="Your Image" width="500">
-</div>
-
-## Installation
-To use `calib_rt`, make sure you have the following dependencies installed:
-- Python (>= 3.10)
-- numpy (>= 1.26.0)
-- pandas (>= 2.1.1)
-- networkx (>= 3.1)
-- statsmodels (>= 0.14.0)
-- scipy (>= 1.11.3)
-
-You can install the `calib_rt` package using pip:
-```bash
-pip install pycalib_rt 
-```
-
-## Usage
-Here is an example of how to use `calib_rt` for RT calibration:
-
-```python
-import calib_rt
-
-# basic information of all built-in datasets 
-calib_rt.RTdatasets.get_datasets_list()  
-         sample_type  datasets_num
-   0   distort_left             2
-   1  distort_right             2
-   2            exp             2
-   3         linear             2
-   4              S             2
-
-# use first of "S" type datasets
-datasets = calib_rt.RTdatasets.get_pandas(sample_type="S",index_in_group=1)
-x = datasets["Spectral library RT"]
-y = datasets["Measured RT"]
-
-# fit and predict
-model = calib_rt.Calib_RT() 
-model.fit(x,y)
-y_pred = model.predict(x)         
-```
-
-## Performance test
-
-<div align=center>
-<img src="https://raw.githubusercontent.com/chenghui03/Calib_RT/main/img/performance-test-1.jpg" alt="Your Image" width="500">
-</div>
-
-Code for performance test is available in the [analysis](https://github.com/chenghui03/Calib_RT/tree/main/analyses).
-For a detailed analysis of the test conclusion, please refer to our paper.
-
-## References
-
-[link of paper]()
-
-## License
-This project is licensed under the MIT License. See the LICENSE file for details.
+Metadata-Version: 2.1
+Name: pycalib_rt
+Version: 0.1.2
+Summary: Calib-RT is designed for RT (retention time) calibration.
+Home-page: https://github.com/chenghui03/Calib_RT/tree/main/
+Author: yichi zhang
+Author-email: kszyc1001@163.com
+Classifier: Programming Language :: Python :: 3
+Classifier: License :: OSI Approved :: MIT License
+Classifier: Operating System :: OS Independent
+Requires-Python: >=3.10
+Description-Content-Type: text/markdown
+License-File: LICENSE
+
+# Calib-RT
+<p align="left">
+    <img alt="PyPI - Version" src="https://img.shields.io/pypi/v/pycalib_rt?style=flat&label=pycalib_rt&color=green">
+    <img title="python version" src="https://img.shields.io/badge/python-3.10-blue" alt="">
+</p>
+
+## Overview
+Calib-RT is an open-source Python software package designed for RT (retention time) calibration. 
+This package provides a flexible and robust solution for achieving accurate RT calibration across various data scales while handling a certain level of noise interference. 
+
+The workflow diagram is below, providing an overview of the process. For a comprehensive and in-depth explanation, please refer to the associated paper for detailed insights and analysis.
+
+<div align=center>
+<img src="https://raw.githubusercontent.com/chenghui03/Calib_RT/93750fced36ee36786e61817d71d6ec5e2c5fdd3/img/workflow.svg" alt="Your Image" width="500">
+</div>
+
+## Installation
+To use `calib_rt`, make sure you have the following dependencies installed:
+- Python (>= 3.10)
+- numpy (>= 1.26.0)
+- pandas (>= 2.1.1)
+- networkx (>= 3.1)
+- statsmodels (>= 0.14.0)
+- scipy (>= 1.11.3)
+
+You can install the `calib_rt` package using pip:
+```bash
+pip install pycalib_rt 
+```
+
+## Usage
+Here is an example of how to use `calib_rt` for RT calibration:
+
+```python
+import calib_rt
+
+# basic information of all built-in datasets 
+calib_rt.RTdatasets.get_datasets_list()  
+         sample_type  datasets_num
+   0   distort_left             2
+   1  distort_right             2
+   2            exp             2
+   3         linear             2
+   4              S             2
+
+# use first of "S" type datasets
+datasets = calib_rt.RTdatasets.get_pandas(sample_type="S",index_in_group=1)
+x = datasets["Spectral library RT"]
+y = datasets["Measured RT"]
+
+# fit and predict
+model = calib_rt.Calib_RT() 
+model.fit(x,y)
+y_pred = model.predict(x)         
+```
+
+## Performance test
+
+<div align=center>
+<img src="https://raw.githubusercontent.com/chenghui03/Calib_RT/main/img/performance-test-1.jpg" alt="Your Image" width="500">
+</div>
+
+Code for performance test is available in the [analysis](https://github.com/chenghui03/Calib_RT/tree/main/analyses).
+For a detailed analysis of the test conclusion, please refer to our paper.
+
+## References
+
+[link of paper]()
+
+## License
+This project is licensed under the MIT License. See the LICENSE file for details.
```

### Comparing `pycalib_rt-0.1.1/calib_rt/data/20200505_Evosep_100SPD_SG06-16_MLHeLa_100ng_py8_S2-C1_1_2731.d.npz` & `pycalib_rt-0.1.2/calib_rt/data/20200505_Evosep_100SPD_SG06-16_MLHeLa_100ng_py8_S2-C1_1_2731.d.npz`

 * *Files identical despite different names*

### Comparing `pycalib_rt-0.1.1/calib_rt/data/20200505_Evosep_200SPD_SG06-16_MLHeLa_200ng_py8_S3-A1_1_2737.d.npz` & `pycalib_rt-0.1.2/calib_rt/data/20200505_Evosep_200SPD_SG06-16_MLHeLa_200ng_py8_S3-A1_1_2737.d.npz`

 * *Files identical despite different names*

### Comparing `pycalib_rt-0.1.1/calib_rt/data/20211101_PRO2_LS_04_MA_HeLaSCS_0.2_ngHS_GE2_1_1408.d.npz` & `pycalib_rt-0.1.2/calib_rt/data/20211101_PRO2_LS_04_MA_HeLaSCS_0.2_ngHS_GE2_1_1408.d.npz`

 * *Files identical despite different names*

### Comparing `pycalib_rt-0.1.1/calib_rt/data/20211103_PRO2_LS_01_MA_HeLa_200_SDC_NS_RE2_1_1418.d.npz` & `pycalib_rt-0.1.2/calib_rt/data/20211103_PRO2_LS_01_MA_HeLa_200_SDC_NS_RE2_1_1418.d.npz`

 * *Files identical despite different names*

### Comparing `pycalib_rt-0.1.1/calib_rt/data/20220714_10ngK562_ZI_500ul60C3cm5min_P1-C1_1_9675.d.npz` & `pycalib_rt-0.1.2/calib_rt/data/20220714_10ngK562_ZI_500ul60C3cm5min_P1-C1_1_9675.d.npz`

 * *Files identical despite different names*

### Comparing `pycalib_rt-0.1.1/calib_rt/data/CMs_Subject3_Lvmid_G10_BG11_1_7560.d.npz` & `pycalib_rt-0.1.2/calib_rt/data/CMs_Subject3_Lvmid_G10_BG11_1_7560.d.npz`

 * *Files identical despite different names*

### Comparing `pycalib_rt-0.1.1/calib_rt/data/SC_HeLa_10min1_Slot1-9_1_807.d.npz` & `pycalib_rt-0.1.2/calib_rt/data/SC_HeLa_10min1_Slot1-9_1_807.d.npz`

 * *Files identical despite different names*

### Comparing `pycalib_rt-0.1.1/calib_rt/data/SC_HeLa_15min1_Slot1-7_1_805.d.npz` & `pycalib_rt-0.1.2/calib_rt/data/SC_HeLa_15min1_Slot1-7_1_805.d.npz`

 * *Files identical despite different names*

### Comparing `pycalib_rt-0.1.1/calib_rt/data/fmeierab_T190525_CLL_diaPASEF_04_1979.d.npz` & `pycalib_rt-0.1.2/calib_rt/data/fmeierab_T190525_CLL_diaPASEF_04_1979.d.npz`

 * *Files identical despite different names*

### Comparing `pycalib_rt-0.1.1/calib_rt/data/fmeierab_T190525_CLL_diaPASEF_40_1965.d.npz` & `pycalib_rt-0.1.2/calib_rt/data/fmeierab_T190525_CLL_diaPASEF_40_1965.d.npz`

 * *Files identical despite different names*

### Comparing `pycalib_rt-0.1.1/calib_rt/datasets.py` & `pycalib_rt-0.1.2/calib_rt/datasets.py`

 * *Ordering differences only*

 * *Files 18% similar despite different names*

```diff
@@ -1,139 +1,139 @@
-# -*- coding:utf-8 -*-
-
-import pandas as pd
-import numpy as np
-import os
-
-
-class RTdatasets(object):
-    """
-    RTdatasets include some commonly used datasets
-    
-    Properties:
-        info: a dict store of all information
-        sample_types: a list of available sample type
-
-    Attributes:
-        get_datasets_list(): get basis information of all datasets
-        get_sample_type_info(): get detail information of all datasets in one sample group
-        get_dict(): get data of datasets in a dict
-        get_pandas(): get data of datasets in a DataFrame type
-    """
-
-    info = {
-        "distort_left":('fmeierab_T190525_CLL_diaPASEF_04_1979',
-                        'fmeierab_T190525_CLL_diaPASEF_40_1965'),
-        "distort_right":('20200505_Evosep_100SPD_SG06-16_MLHeLa_100ng_py8_S2-C1_1_2731',
-                         '20211103_PRO2_LS_01_MA_HeLa_200_SDC_NS_RE2_1_1418'),
-        "exp":('SC_HeLa_10min1_Slot1-9_1_807',
-               'SC_HeLa_15min1_Slot1-7_1_805'),
-        "linear":('20211101_PRO2_LS_04_MA_HeLaSCS_0.2_ngHS_GE2_1_1408',
-                  '20220714_10ngK562_ZI_500ul60C3cm5min_P1-C1_1_9675'),
-        "S":('20200505_Evosep_200SPD_SG06-16_MLHeLa_200ng_py8_S3-A1_1_2737',
-             'CMs_Subject3_Lvmid_G10_BG11_1_7560')
-    }
-    sample_types = ["distort_left","distort_right","exp","linear","S"]
-
-    __library_root = os.path.dirname(__file__)
-    __file_path = os.path.join(__library_root, "data")
-
-    def get_datasets_list() -> pd.DataFrame:
-        """
-        get basis information of all datasets
-        
-        Results:
-            a DataFrame of all datasets
-        
-        Examples:
-            >>> from calib_rt import RTdatasets
-            >>> RTdatasets.get_datasets_list()
-                 sample_type  datasets_num
-            0   distort_left             2
-            1  distort_right             2
-            2            exp             2
-            3         linear             2
-            4              S             2
-        
-        References:
-            url
-        """
-        result = [len(RTdatasets.info[sample_type])
-                  for sample_type in RTdatasets.sample_types]
-        df = pd.DataFrame({"sample_type":RTdatasets.sample_types,
-                           "datasets_num":result})
-        return df
-    
-    def get_sample_type_info(sample_type:str) -> dict:
-        """
-        get detail information of all datasets in one sample group
-
-        Args:
-            sample_type(str): a str which in RTdatasets.sample_types is OK
-
-        Results:
-            a dict of detail of datasets in is sample group
-        
-        Examples:
-            >>> from calib_rt import RTdatasets
-            >>> RTdatasets.get_sample_type_info("S")
-        
-        References:
-            url
-        """
-        result = RTdatasets.info[sample_type]
-        return {sample_type:result}
-
-    
-    def get_dict(sample_type:str,index_in_group:int) -> dict[str:np.ndarray]:
-        """
-        get data of datasets in a dict
-
-        Args:
-            sample_type(str): a str which in RTdatasets.sample_types is OK
-
-            index_in_group(int): the index of datasets in it's group
-
-        Results:
-            dict of RT data
-
-            like: {"Spectral library RT":ndarray,"Measured RT":ndarray}
-        
-        Examples:
-            >>> from calib_rt import RTdatasets
-            >>> RTdatasets.get_dict("linear",0)
-        
-        References:
-            url
-        """
-        info = RTdatasets.info[sample_type][index_in_group]
-        df_path = os.path.join(RTdatasets.__file_path,f"{info}.d.npz")
-        data = np.load(df_path)
-        df_dict = {"Spectral library RT":data["x"],
-                   "Measured RT":data["y"]}
-        return df_dict
-    
-    def get_pandas(sample_type:str,index_in_group:int) -> pd.DataFrame:
-        """
-        get data of datasets in a DataFrame type
-
-        Args:
-            sample_type(str): a str which in RTdatasets.sample_types is OK
-
-            index_in_group(int): the index of datasets in it's group
-
-        Results:
-            DataFrame of RT data 
-            
-            The detail information can get from Name 
-        
-        Examples:
-            >>> from calib_rt import RTdatasets
-            >>> RTdatasets.get_pandas("linear",0)
-        
-        References:
-            url
-        """
-        df_dict = RTdatasets.get_dict(sample_type,index_in_group)
-        df = pd.DataFrame(df_dict)
-        df.Name = RTdatasets.info[sample_type][index_in_group]
+# -*- coding:utf-8 -*-
+
+import pandas as pd
+import numpy as np
+import os
+
+
+class RTdatasets(object):
+    """
+    RTdatasets include some commonly used datasets
+    
+    Properties:
+        info: a dict store of all information
+        sample_types: a list of available sample type
+
+    Attributes:
+        get_datasets_list(): get basis information of all datasets
+        get_sample_type_info(): get detail information of all datasets in one sample group
+        get_dict(): get data of datasets in a dict
+        get_pandas(): get data of datasets in a DataFrame type
+    """
+
+    info = {
+        "distort_left":('fmeierab_T190525_CLL_diaPASEF_04_1979',
+                        'fmeierab_T190525_CLL_diaPASEF_40_1965'),
+        "distort_right":('20200505_Evosep_100SPD_SG06-16_MLHeLa_100ng_py8_S2-C1_1_2731',
+                         '20211103_PRO2_LS_01_MA_HeLa_200_SDC_NS_RE2_1_1418'),
+        "exp":('SC_HeLa_10min1_Slot1-9_1_807',
+               'SC_HeLa_15min1_Slot1-7_1_805'),
+        "linear":('20211101_PRO2_LS_04_MA_HeLaSCS_0.2_ngHS_GE2_1_1408',
+                  '20220714_10ngK562_ZI_500ul60C3cm5min_P1-C1_1_9675'),
+        "S":('20200505_Evosep_200SPD_SG06-16_MLHeLa_200ng_py8_S3-A1_1_2737',
+             'CMs_Subject3_Lvmid_G10_BG11_1_7560')
+    }
+    sample_types = ["distort_left","distort_right","exp","linear","S"]
+
+    __library_root = os.path.dirname(__file__)
+    __file_path = os.path.join(__library_root, "data")
+
+    def get_datasets_list() -> pd.DataFrame:
+        """
+        get basis information of all datasets
+        
+        Results:
+            a DataFrame of all datasets
+        
+        Examples:
+            >>> from calib_rt import RTdatasets
+            >>> RTdatasets.get_datasets_list()
+                 sample_type  datasets_num
+            0   distort_left             2
+            1  distort_right             2
+            2            exp             2
+            3         linear             2
+            4              S             2
+        
+        References:
+            url
+        """
+        result = [len(RTdatasets.info[sample_type])
+                  for sample_type in RTdatasets.sample_types]
+        df = pd.DataFrame({"sample_type":RTdatasets.sample_types,
+                           "datasets_num":result})
+        return df
+    
+    def get_sample_type_info(sample_type:str) -> dict:
+        """
+        get detail information of all datasets in one sample group
+
+        Args:
+            sample_type(str): a str which in RTdatasets.sample_types is OK
+
+        Results:
+            a dict of detail of datasets in is sample group
+        
+        Examples:
+            >>> from calib_rt import RTdatasets
+            >>> RTdatasets.get_sample_type_info("S")
+        
+        References:
+            url
+        """
+        result = RTdatasets.info[sample_type]
+        return {sample_type:result}
+
+    
+    def get_dict(sample_type:str,index_in_group:int) -> dict[str:np.ndarray]:
+        """
+        get data of datasets in a dict
+
+        Args:
+            sample_type(str): a str which in RTdatasets.sample_types is OK
+
+            index_in_group(int): the index of datasets in it's group
+
+        Results:
+            dict of RT data
+
+            like: {"Spectral library RT":ndarray,"Measured RT":ndarray}
+        
+        Examples:
+            >>> from calib_rt import RTdatasets
+            >>> RTdatasets.get_dict("linear",0)
+        
+        References:
+            url
+        """
+        info = RTdatasets.info[sample_type][index_in_group]
+        df_path = os.path.join(RTdatasets.__file_path,f"{info}.d.npz")
+        data = np.load(df_path)
+        df_dict = {"Spectral library RT":data["x"],
+                   "Measured RT":data["y"]}
+        return df_dict
+    
+    def get_pandas(sample_type:str,index_in_group:int) -> pd.DataFrame:
+        """
+        get data of datasets in a DataFrame type
+
+        Args:
+            sample_type(str): a str which in RTdatasets.sample_types is OK
+
+            index_in_group(int): the index of datasets in it's group
+
+        Results:
+            DataFrame of RT data 
+            
+            The detail information can get from Name 
+        
+        Examples:
+            >>> from calib_rt import RTdatasets
+            >>> RTdatasets.get_pandas("linear",0)
+        
+        References:
+            url
+        """
+        df_dict = RTdatasets.get_dict(sample_type,index_in_group)
+        df = pd.DataFrame(df_dict)
+        df.Name = RTdatasets.info[sample_type][index_in_group]
         return df
```

### Comparing `pycalib_rt-0.1.1/calib_rt/regression.py` & `pycalib_rt-0.1.2/calib_rt/regression.py`

 * *Ordering differences only*

 * *Files 13% similar despite different names*

```diff
@@ -1,80 +1,80 @@
-# -*- coding:utf-8 -*-
-
-import statsmodels.api as sm
-import numpy as np
-from scipy.interpolate import interp1d
-
-class InputDataError(Exception):
-    def __init__(self, message) -> None:
-        super().__init__(message)
-
-
-def fit_by_lowess(x, y, manual_frac=-1):
-    data=np.column_stack((x,y))
-    data = data[data[:, 0] != 0]
-    x,y=data[:,0],data[:,1]
-
-    if manual_frac == -1:
-        frac=choose_frac(x,y)
-        print(f"Choose lowess frac: {frac:.2f}")
-    else:
-        frac=manual_frac
-
-    # by lowess
-    lowess = sm.nonparametric.lowess
-    y_lowess = lowess(y, x, frac)
-    x_fit, y_fit = zip(*y_lowess)
-    x_fit, y_fit = np.array(x_fit), np.array(y_fit)
-    return x_fit, y_fit
-
-def choose_frac(x, y):
-    frac_v = [0.05, 0.1, 0.15, 0.2, 0.25, 0.3]
-    mape_v = []
-    for frac in frac_v:
-        y_pred = sm.nonparametric.lowess(y, x, frac, return_sorted=False)
-        mape = np.nanmean(np.abs(y - y_pred) / y)
-        mape_v.append(mape)
-    return frac_v[np.argmin(mape_v)]
-
-
-class Predictor:
-    def __init__(self,x_fit,y_fit) -> None:
-        
-        data=self.__make_x_unique(x_fit,y_fit)
-        x_fit,y_fit=data[:,0],data[:,1]
-        self.f_in = interp1d(x_fit, y_fit, kind ='linear')
-
-        # extrapolate for start
-        idx_start = np.argsort(x_fit)[:5]
-        coefficients = np.polyfit(x_fit[idx_start], y_fit[idx_start], 1)
-        self.f_start = np.poly1d(coefficients)
-
-        # extrapolate for end
-        idx_end = np.argsort(x_fit)[::-1][:5]
-        coefficients = np.polyfit(x_fit[idx_end], y_fit[idx_end], 1)
-        self.f_end = np.poly1d(coefficients)
-
-    def __make_x_unique(self,x_fit,y_fit):
-        data=np.column_stack((x_fit,y_fit))
-        unique_data=dict()
-        for x,y in data:
-            if not unique_data.get(x):
-                unique_data[x]=y
-        return np.array(list(unique_data.items()))
-
-    def predict(self,x_interp):
-        x_max, x_min = self.f_in.x.max(), self.f_in.x.min()
-        is_inner = (x_interp <= x_max) & (x_interp >= x_min)
-        is_start = x_interp < x_min
-        is_end = x_interp > x_max
-        x_in = x_interp[is_inner]
-        x_start = x_interp[is_start]
-        x_end = x_interp[is_end]
-        x_in_pred = self.f_in(x_in)
-        x_start_pred = self.f_start(x_start)
-        x_end_pred = self.f_end(x_end)
-        pred = np.empty_like(x_interp)
-        pred[is_inner] = x_in_pred
-        pred[is_start] = x_start_pred
-        pred[is_end] = x_end_pred
+# -*- coding:utf-8 -*-
+
+import statsmodels.api as sm
+import numpy as np
+from scipy.interpolate import interp1d
+
+class InputDataError(Exception):
+    def __init__(self, message) -> None:
+        super().__init__(message)
+
+
+def fit_by_lowess(x, y, manual_frac=-1):
+    data=np.column_stack((x,y))
+    data = data[data[:, 0] != 0]
+    x,y=data[:,0],data[:,1]
+
+    if manual_frac == -1:
+        frac=choose_frac(x,y)
+        print(f"Choose lowess frac: {frac:.2f}")
+    else:
+        frac=manual_frac
+
+    # by lowess
+    lowess = sm.nonparametric.lowess
+    y_lowess = lowess(y, x, frac)
+    x_fit, y_fit = zip(*y_lowess)
+    x_fit, y_fit = np.array(x_fit), np.array(y_fit)
+    return x_fit, y_fit
+
+def choose_frac(x, y):
+    frac_v = [0.05, 0.1, 0.15, 0.2, 0.25, 0.3]
+    mape_v = []
+    for frac in frac_v:
+        y_pred = sm.nonparametric.lowess(y, x, frac, return_sorted=False)
+        mape = np.nanmean(np.abs(y - y_pred) / y)
+        mape_v.append(mape)
+    return frac_v[np.argmin(mape_v)]
+
+
+class Predictor:
+    def __init__(self,x_fit,y_fit) -> None:
+        
+        data=self.__make_x_unique(x_fit,y_fit)
+        x_fit,y_fit=data[:,0],data[:,1]
+        self.f_in = interp1d(x_fit, y_fit, kind ='linear')
+
+        # extrapolate for start
+        idx_start = np.argsort(x_fit)[:5]
+        coefficients = np.polyfit(x_fit[idx_start], y_fit[idx_start], 1)
+        self.f_start = np.poly1d(coefficients)
+
+        # extrapolate for end
+        idx_end = np.argsort(x_fit)[::-1][:5]
+        coefficients = np.polyfit(x_fit[idx_end], y_fit[idx_end], 1)
+        self.f_end = np.poly1d(coefficients)
+
+    def __make_x_unique(self,x_fit,y_fit):
+        data=np.column_stack((x_fit,y_fit))
+        unique_data=dict()
+        for x,y in data:
+            if not unique_data.get(x):
+                unique_data[x]=y
+        return np.array(list(unique_data.items()))
+
+    def predict(self,x_interp):
+        x_max, x_min = self.f_in.x.max(), self.f_in.x.min()
+        is_inner = (x_interp <= x_max) & (x_interp >= x_min)
+        is_start = x_interp < x_min
+        is_end = x_interp > x_max
+        x_in = x_interp[is_inner]
+        x_start = x_interp[is_start]
+        x_end = x_interp[is_end]
+        x_in_pred = self.f_in(x_in)
+        x_start_pred = self.f_start(x_start)
+        x_end_pred = self.f_end(x_end)
+        pred = np.empty_like(x_interp)
+        pred[is_inner] = x_in_pred
+        pred[is_start] = x_start_pred
+        pred[is_end] = x_end_pred
         return pred
```

### Comparing `pycalib_rt-0.1.1/calib_rt/screen.py` & `pycalib_rt-0.1.2/calib_rt/screen.py`

 * *Ordering differences only*

 * *Files 16% similar despite different names*

```diff
@@ -1,86 +1,86 @@
-# -*- coding:utf-8 -*-
-
-import numpy as np
-import networkx as nx
-
-def screen_by_hist(x_data, y_data, bins):
-    extenti = (x_data.min()-0.1, x_data.max()+0.1)
-    extentj = (y_data.min()-0.1, y_data.max()+0.1)
-    hist, edges_x, edges_y = np.histogram2d(
-        x_data, y_data, bins=bins,range=(extenti, extentj)
-    )
-    edges_x = (edges_x[:-1] + edges_x[1:]) / 2
-    edges_y = (edges_y[:-1] + edges_y[1:]) / 2
-    
-    cell_idXy = np.stack((np.arange(hist.shape[0]),hist.argmax(axis=1)),axis=-1)
-    cell_idYx = np.stack((hist.argmax(axis=0),np.arange(hist.shape[1])),axis=-1)
-    cell_idxy = np.vstack((cell_idXy,cell_idYx))
-    cell_idxy = np.unique(cell_idxy,axis=0)
-    cell_idxy = cell_idxy[~(cell_idxy == 0).any(axis=1)]
-    
-    x_hist = edges_x[cell_idxy[:,0]]
-    y_hist = edges_y[cell_idxy[:,1]]
-    cell_counts = hist[tuple(cell_idxy.T)]
-
-    rho=cell_counts
-    if np.max(rho)-np.min(rho)!=0:
-        rho = (rho - np.min(rho))/(np.max(rho)-np.min(rho))+1
-    return x_hist, y_hist, rho
-
-def screen_by_graph(x_screen1, y_screen1, rho):
-    G = nx.DiGraph()
-    for i in range(len(x_screen1)):
-        x_curr, y_curr = x_screen1[i], y_screen1[i]
-        candidates_idx = (x_screen1 >= x_curr) & (y_screen1 >= y_curr)
-        candidates_idx[i] = False
-        
-        x_candidates = x_screen1[candidates_idx]
-        y_candidates = y_screen1[candidates_idx]
-        rho_candidates = rho[candidates_idx]
-
-        candidates = [((x_curr, y_curr), (x, y),{"edge":rho[i]*r/((x_curr-x)**2+(y_curr-y)**2)**0.5}) 
-                      for x, y ,r in zip(x_candidates, y_candidates, rho_candidates)]
-        G.add_edges_from(candidates)
-
-    longest_path = nx.dag_longest_path(G,weight="edge")
-    x_screen2, y_screen2 = zip(*longest_path)
-    x_screen2, y_screen2 = np.array(x_screen2), np.array(y_screen2)
-
-    return x_screen2, y_screen2
-
-def polish_ends(x_screen2, y_screen2, tol_bins):
-    center_idx = int(len(x_screen2) / 4)
-
-    x, y = x_screen2[:center_idx], y_screen2[:center_idx]
-    stepx = x[1:] - x[:-1]
-    good_x = (stepx / stepx[stepx > 0].min()) < tol_bins
-    stepy = y[1:] - y[:-1]
-    good_y = (stepy / stepy[stepy > 0].min()) < tol_bins
-    good_xy = good_x & good_y
-    breaks_idx = np.where(good_xy == False)[0]
-    
-    break_idx = 0
-    if len(breaks_idx) > 0:
-        idx = np.where(breaks_idx < len(x) * 0.25)[0]
-        if len(idx) > 0:
-            break_idx = breaks_idx[idx][-1] + 1
-    x_left, y_left = x[break_idx:], y[break_idx:]
-
-    x, y = x_screen2[center_idx:], y_screen2[center_idx:]
-    stepx = x[1:] - x[:-1]
-    good_x = (stepx / stepx[stepx > 0].min()) < tol_bins
-    stepy = y[1:] - y[:-1]
-    good_y = (stepy / stepy[stepy > 0].min()) < tol_bins
-    good_xy = good_x & good_y
-    breaks_idx = np.where(good_xy == False)[0]
-    
-    break_idx = len(x)
-    if len(breaks_idx) > 0:
-        idx = np.where(breaks_idx > len(x) * 0.75)[0] 
-        if len(idx) > 0:
-            break_idx = breaks_idx[idx][0] + 1 
-    x_right, y_right = x[:break_idx], y[:break_idx]
-    
-    x = np.concatenate([x_left, x_right])
-    y = np.concatenate([y_left, y_right])
+# -*- coding:utf-8 -*-
+
+import numpy as np
+import networkx as nx
+
+def screen_by_hist(x_data, y_data, bins):
+    extenti = (x_data.min()-0.1, x_data.max()+0.1)
+    extentj = (y_data.min()-0.1, y_data.max()+0.1)
+    hist, edges_x, edges_y = np.histogram2d(
+        x_data, y_data, bins=bins,range=(extenti, extentj)
+    )
+    edges_x = (edges_x[:-1] + edges_x[1:]) / 2
+    edges_y = (edges_y[:-1] + edges_y[1:]) / 2
+    
+    cell_idXy = np.stack((np.arange(hist.shape[0]),hist.argmax(axis=1)),axis=-1)
+    cell_idYx = np.stack((hist.argmax(axis=0),np.arange(hist.shape[1])),axis=-1)
+    cell_idxy = np.vstack((cell_idXy,cell_idYx))
+    cell_idxy = np.unique(cell_idxy,axis=0)
+    cell_idxy = cell_idxy[~(cell_idxy == 0).any(axis=1)]
+    
+    x_hist = edges_x[cell_idxy[:,0]]
+    y_hist = edges_y[cell_idxy[:,1]]
+    cell_counts = hist[tuple(cell_idxy.T)]
+
+    rho=cell_counts
+    if np.max(rho)-np.min(rho)!=0:
+        rho = (rho - np.min(rho))/(np.max(rho)-np.min(rho))+1
+    return x_hist, y_hist, rho
+
+def screen_by_graph(x_screen1, y_screen1, rho):
+    G = nx.DiGraph()
+    for i in range(len(x_screen1)):
+        x_curr, y_curr = x_screen1[i], y_screen1[i]
+        candidates_idx = (x_screen1 >= x_curr) & (y_screen1 >= y_curr)
+        candidates_idx[i] = False
+        
+        x_candidates = x_screen1[candidates_idx]
+        y_candidates = y_screen1[candidates_idx]
+        rho_candidates = rho[candidates_idx]
+
+        candidates = [((x_curr, y_curr), (x, y),{"edge":rho[i]*r/((x_curr-x)**2+(y_curr-y)**2)**0.5}) 
+                      for x, y ,r in zip(x_candidates, y_candidates, rho_candidates)]
+        G.add_edges_from(candidates)
+
+    longest_path = nx.dag_longest_path(G,weight="edge")
+    x_screen2, y_screen2 = zip(*longest_path)
+    x_screen2, y_screen2 = np.array(x_screen2), np.array(y_screen2)
+
+    return x_screen2, y_screen2
+
+def polish_ends(x_screen2, y_screen2, tol_bins):
+    center_idx = int(len(x_screen2) / 4)
+
+    x, y = x_screen2[:center_idx], y_screen2[:center_idx]
+    stepx = x[1:] - x[:-1]
+    good_x = (stepx / stepx[stepx > 0].min()) < tol_bins
+    stepy = y[1:] - y[:-1]
+    good_y = (stepy / stepy[stepy > 0].min()) < tol_bins
+    good_xy = good_x & good_y
+    breaks_idx = np.where(good_xy == False)[0]
+    
+    break_idx = 0
+    if len(breaks_idx) > 0:
+        idx = np.where(breaks_idx < len(x) * 0.25)[0]
+        if len(idx) > 0:
+            break_idx = breaks_idx[idx][-1] + 1
+    x_left, y_left = x[break_idx:], y[break_idx:]
+
+    x, y = x_screen2[center_idx:], y_screen2[center_idx:]
+    stepx = x[1:] - x[:-1]
+    good_x = (stepx / stepx[stepx > 0].min()) < tol_bins
+    stepy = y[1:] - y[:-1]
+    good_y = (stepy / stepy[stepy > 0].min()) < tol_bins
+    good_xy = good_x & good_y
+    breaks_idx = np.where(good_xy == False)[0]
+    
+    break_idx = len(x)
+    if len(breaks_idx) > 0:
+        idx = np.where(breaks_idx > len(x) * 0.75)[0] 
+        if len(idx) > 0:
+            break_idx = breaks_idx[idx][0] + 1 
+    x_right, y_right = x[:break_idx], y[:break_idx]
+    
+    x = np.concatenate([x_left, x_right])
+    y = np.concatenate([y_left, y_right])
     return x, y
```

### Comparing `pycalib_rt-0.1.1/pycalib_rt.egg-info/SOURCES.txt` & `pycalib_rt-0.1.2/pycalib_rt.egg-info/SOURCES.txt`

 * *Files identical despite different names*

