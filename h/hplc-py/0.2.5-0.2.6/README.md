# Comparing `tmp/hplc-py-0.2.5.tar.gz` & `tmp/hplc_py-0.2.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "hplc-py-0.2.5.tar", last modified: Fri Feb  9 23:27:27 2024, max compression
+gzip compressed data, was "hplc_py-0.2.6.tar", last modified: Wed May 29 01:11:16 2024, max compression
```

## Comparing `hplc-py-0.2.5.tar` & `hplc_py-0.2.6.tar`

### file list

```diff
@@ -1,19 +1,19 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-09 23:27:27.035414 hplc-py-0.2.5/
--rw-r--r--   0 runner    (1001) docker     (127)    34666 2024-02-09 23:27:19.000000 hplc-py-0.2.5/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)     6724 2024-02-09 23:27:27.035414 hplc-py-0.2.5/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     6002 2024-02-09 23:27:19.000000 hplc-py-0.2.5/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-09 23:27:27.031414 hplc-py-0.2.5/hplc/
--rw-r--r--   0 runner    (1001) docker     (127)      150 2024-02-09 23:27:19.000000 hplc-py-0.2.5/hplc/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2115 2024-02-09 23:27:19.000000 hplc-py-0.2.5/hplc/io.py
--rw-r--r--   0 runner    (1001) docker     (127)    61437 2024-02-09 23:27:19.000000 hplc-py-0.2.5/hplc/quant.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-09 23:27:27.035414 hplc-py-0.2.5/hplc_py.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     6724 2024-02-09 23:27:27.000000 hplc-py-0.2.5/hplc_py.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      266 2024-02-09 23:27:27.000000 hplc-py-0.2.5/hplc_py.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-02-09 23:27:27.000000 hplc-py-0.2.5/hplc_py.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)      106 2024-02-09 23:27:27.000000 hplc-py-0.2.5/hplc_py.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)        5 2024-02-09 23:27:27.000000 hplc-py-0.2.5/hplc_py.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-02-09 23:27:27.035414 hplc-py-0.2.5/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)     1152 2024-02-09 23:27:19.000000 hplc-py-0.2.5/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-09 23:27:27.031414 hplc-py-0.2.5/tests/
--rw-r--r--   0 runner    (1001) docker     (127)    18670 2024-02-09 23:27:19.000000 hplc-py-0.2.5/tests/test_chromatogram.py
--rw-r--r--   0 runner    (1001) docker     (127)     1752 2024-02-09 23:27:19.000000 hplc-py-0.2.5/tests/test_io.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-29 01:11:16.091792 hplc_py-0.2.6/
+-rw-r--r--   0 runner    (1001) docker     (127)    34666 2024-05-29 01:11:00.000000 hplc_py-0.2.6/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)     7316 2024-05-29 01:11:16.091792 hplc_py-0.2.6/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     6594 2024-05-29 01:11:00.000000 hplc_py-0.2.6/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-29 01:11:16.087792 hplc_py-0.2.6/hplc/
+-rw-r--r--   0 runner    (1001) docker     (127)      150 2024-05-29 01:11:00.000000 hplc_py-0.2.6/hplc/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2115 2024-05-29 01:11:00.000000 hplc_py-0.2.6/hplc/io.py
+-rw-r--r--   0 runner    (1001) docker     (127)    61594 2024-05-29 01:11:00.000000 hplc_py-0.2.6/hplc/quant.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-29 01:11:16.091792 hplc_py-0.2.6/hplc_py.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     7316 2024-05-29 01:11:16.000000 hplc_py-0.2.6/hplc_py.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      266 2024-05-29 01:11:16.000000 hplc_py-0.2.6/hplc_py.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-29 01:11:16.000000 hplc_py-0.2.6/hplc_py.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      106 2024-05-29 01:11:16.000000 hplc_py-0.2.6/hplc_py.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        5 2024-05-29 01:11:16.000000 hplc_py-0.2.6/hplc_py.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-29 01:11:16.091792 hplc_py-0.2.6/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)     1152 2024-05-29 01:11:00.000000 hplc_py-0.2.6/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-29 01:11:16.091792 hplc_py-0.2.6/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)    18701 2024-05-29 01:11:00.000000 hplc_py-0.2.6/tests/test_chromatogram.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1752 2024-05-29 01:11:01.000000 hplc_py-0.2.6/tests/test_io.py
```

### Comparing `hplc-py-0.2.5/LICENSE` & `hplc_py-0.2.6/LICENSE`

 * *Files identical despite different names*

### Comparing `hplc-py-0.2.5/PKG-INFO` & `hplc_py-0.2.6/PKG-INFO`

 * *Files 12% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: hplc-py
-Version: 0.2.5
+Version: 0.2.6
 Summary: Python utilities for the processing and quantification of chromatograms from High Performance Liquid Chromatography (HPLC).
 Home-page: https://github.com/cremerlab/hplc-py
 Author: Griffin Chure
 Author-email: griffinchure@gmail.com
 License: GPLv3
 Classifier: Development Status :: 4 - Beta
 Classifier: Intended Audience :: Science/Research
@@ -21,16 +21,15 @@
 
 ![](docs/source/_static/homepage_logo.png)
 
 [![License: GPL v3](https://img.shields.io/badge/License-GPLv3-blue.svg)](https://www.gnu.org/licenses/gpl-3.0)
 [![Run tests](https://github.com/cremerlab/hplc-py/actions/workflows/pytest.yaml/badge.svg)](https://github.com/cremerlab/hplc-py/actions/workflows/pytest.yaml)
 [![codecov](https://codecov.io/gh/cremerlab/hplc-py/branch/main/graph/badge.svg?token=WXL50JVR6C)](https://codecov.io/gh/cremerlab/hplc-py)
 [![PyPI version](https://badge.fury.io/py/hplc-py.svg)](https://badge.fury.io/py/hplc-py)
-[![DOI](https://zenodo.org/badge/667610900.svg)](https://zenodo.org/badge/latestdoi/667610900)
-
+[![DOI](https://joss.theoj.org/papers/10.21105/joss.06270/status.svg)](https://doi.org/10.21105/joss.06270)
 
 # About
 
 **H**igh-**P**erformance **L**iquid **C**hromatography (HPLC) is an analytical
 technique which allows for quantitative characterization of the chemical
 components of a mixture. While many of the technical details of HPLC are now
 automated, the programmatic cleaning and processing of the resulting data often requires extensive manual labor. This package was
@@ -107,32 +106,50 @@
 ```python 
 In[6]: peaks = chrom.fit_peaks()
 Performing baseline correction: 100%|████████| 299/299 [00:01<00:00, 167.06it/s]
 Deconvolving mixture: 100%|███████████████████████| 3/3 [00:13<00:00,  4.66s/it]
 
 In[7]: peaks.head()
 Out[7]:   
-   retention_time     scale      skew     amplitude          area  peak_id
-0           10.90  0.157450  0.674286  23250.349387  2.790042e+06        1
-0           13.17  0.582866  3.839860  42250.783974  5.070094e+06        2
-0           14.45  0.353036 -3.019153  35229.583555  4.227550e+06        3
-0           15.53  0.312563  1.630787  14891.041452  1.786925e+06        4
-0           16.52  0.344266  1.984167  10770.656732  1.292479e+06        5
+	retention_time	   scale	    skew	   amplitude	        area	signal_maximum	peak_id
+0			 10.90	0.158768	0.691961	23380.386403	2.805646e+06	66064.361454	1
+0			 13.17	0.592828	3.889788	43048.461053	5.165815e+06	50331.167860	2
+0			 14.45	0.350139   -2.997977	34791.996875	4.175040e+06	65352.588796	3
+0			 15.53	0.308900	1.567356	14938.309504	1.792597e+06	26723.707626	4
+0			 16.55	0.272283	1.261303	9512.727882	    1.141527e+06	18121.299375	5
 ```
 
 The resulting chromatogram reconstruction can be seen by again calling the `show()` 
 method, this time restricting the plotted time region between 10 and 20 minutes.
 
 ```python
 In[8]: chrom.show()
 Out[8]:[<Figure size 640x480 with 1 Axes>,
  <Axes: xlabel='time', ylabel='signal (baseline corrected)'>]
 ```
 ![](example/reconstructed_chromatogram.png)
 
+# Citation
+If you use `hplc-py` in your research please cite the version of the software
+you use along with our [descriptive paper in JOSS](https://joss.theoj.org/papers/10.21105/joss.06270):
+
+```
+@article{chure2024,
+	author = {Chure, Griffin and Cremer, Jonas},
+	title = {hplc-py: A Python Utility For Rapid Quantification of Complex Chemical Chromatograms},
+	volume = 9,
+    number = 94,
+	url = {https://joss.theoj.org/papers/10.21105/joss.06270},
+	doi = {10.21105/joss.06270},
+	number = {94},
+	urldate = {2024-02-16},
+	journal = {Journal of Open Source Software},
+	year = {2024}
+   }
+```
 
 # Contributing
 Development of hplc-py occurs on various feature branches which are merged and released upon approval by Griffin Chure (@gchure), the primary maintainer of the software.
 
 Please submit issues and bug reports using the issue tracker. When filing an
 issue, provide a reproducible example that demonstrates the bug or problem.
 Feature requests can also be made through the issue tracker, though it is up to
```

### Comparing `hplc-py-0.2.5/README.md` & `hplc_py-0.2.6/README.md`

 * *Files 10% similar despite different names*

```diff
@@ -1,15 +1,14 @@
 ![](docs/source/_static/homepage_logo.png)
 
 [![License: GPL v3](https://img.shields.io/badge/License-GPLv3-blue.svg)](https://www.gnu.org/licenses/gpl-3.0)
 [![Run tests](https://github.com/cremerlab/hplc-py/actions/workflows/pytest.yaml/badge.svg)](https://github.com/cremerlab/hplc-py/actions/workflows/pytest.yaml)
 [![codecov](https://codecov.io/gh/cremerlab/hplc-py/branch/main/graph/badge.svg?token=WXL50JVR6C)](https://codecov.io/gh/cremerlab/hplc-py)
 [![PyPI version](https://badge.fury.io/py/hplc-py.svg)](https://badge.fury.io/py/hplc-py)
-[![DOI](https://zenodo.org/badge/667610900.svg)](https://zenodo.org/badge/latestdoi/667610900)
-
+[![DOI](https://joss.theoj.org/papers/10.21105/joss.06270/status.svg)](https://doi.org/10.21105/joss.06270)
 
 # About
 
 **H**igh-**P**erformance **L**iquid **C**hromatography (HPLC) is an analytical
 technique which allows for quantitative characterization of the chemical
 components of a mixture. While many of the technical details of HPLC are now
 automated, the programmatic cleaning and processing of the resulting data often requires extensive manual labor. This package was
@@ -86,32 +85,50 @@
 ```python 
 In[6]: peaks = chrom.fit_peaks()
 Performing baseline correction: 100%|████████| 299/299 [00:01<00:00, 167.06it/s]
 Deconvolving mixture: 100%|███████████████████████| 3/3 [00:13<00:00,  4.66s/it]
 
 In[7]: peaks.head()
 Out[7]:   
-   retention_time     scale      skew     amplitude          area  peak_id
-0           10.90  0.157450  0.674286  23250.349387  2.790042e+06        1
-0           13.17  0.582866  3.839860  42250.783974  5.070094e+06        2
-0           14.45  0.353036 -3.019153  35229.583555  4.227550e+06        3
-0           15.53  0.312563  1.630787  14891.041452  1.786925e+06        4
-0           16.52  0.344266  1.984167  10770.656732  1.292479e+06        5
+	retention_time	   scale	    skew	   amplitude	        area	signal_maximum	peak_id
+0			 10.90	0.158768	0.691961	23380.386403	2.805646e+06	66064.361454	1
+0			 13.17	0.592828	3.889788	43048.461053	5.165815e+06	50331.167860	2
+0			 14.45	0.350139   -2.997977	34791.996875	4.175040e+06	65352.588796	3
+0			 15.53	0.308900	1.567356	14938.309504	1.792597e+06	26723.707626	4
+0			 16.55	0.272283	1.261303	9512.727882	    1.141527e+06	18121.299375	5
 ```
 
 The resulting chromatogram reconstruction can be seen by again calling the `show()` 
 method, this time restricting the plotted time region between 10 and 20 minutes.
 
 ```python
 In[8]: chrom.show()
 Out[8]:[<Figure size 640x480 with 1 Axes>,
  <Axes: xlabel='time', ylabel='signal (baseline corrected)'>]
 ```
 ![](example/reconstructed_chromatogram.png)
 
+# Citation
+If you use `hplc-py` in your research please cite the version of the software
+you use along with our [descriptive paper in JOSS](https://joss.theoj.org/papers/10.21105/joss.06270):
+
+```
+@article{chure2024,
+	author = {Chure, Griffin and Cremer, Jonas},
+	title = {hplc-py: A Python Utility For Rapid Quantification of Complex Chemical Chromatograms},
+	volume = 9,
+    number = 94,
+	url = {https://joss.theoj.org/papers/10.21105/joss.06270},
+	doi = {10.21105/joss.06270},
+	number = {94},
+	urldate = {2024-02-16},
+	journal = {Journal of Open Source Software},
+	year = {2024}
+   }
+```
 
 # Contributing
 Development of hplc-py occurs on various feature branches which are merged and released upon approval by Griffin Chure (@gchure), the primary maintainer of the software.
 
 Please submit issues and bug reports using the issue tracker. When filing an
 issue, provide a reproducible example that demonstrates the bug or problem.
 Feature requests can also be made through the issue tracker, though it is up to
```

### Comparing `hplc-py-0.2.5/hplc/io.py` & `hplc_py-0.2.6/hplc/io.py`

 * *Files identical despite different names*

### Comparing `hplc-py-0.2.5/hplc/quant.py` & `hplc_py-0.2.6/hplc/quant.py`

 * *Files 1% similar despite different names*

```diff
@@ -637,21 +637,23 @@
 
             # Assemble the dictionary of output
             if v['num_peaks'] > 1:
                 popt = np.reshape(popt, (v['num_peaks'], 4))
             else:
                 popt = [popt]
             for i, p in enumerate(popt):
+                recon_signal = self._compute_skewnorm(t_range, *p)
                 window_dict[f'peak_{i + 1}'] = {
                     'amplitude': p[0],
                     'retention_time': np.round(p[1], decimals=self._time_precision),
                     'scale': p[2],
                     'alpha': p[3],
                     'area': self._compute_skewnorm(t_range, *p).sum(),
-                    'reconstructed_signal': self._compute_skewnorm(v['time_range'], *p)}
+                    'reconstructed_signal': recon_signal,
+                    'signal_max': np.max(recon_signal)}
             peak_props[k] = window_dict
 
         self._peak_props = peak_props
         return peak_props
 
     def fit_peaks(self,
                   known_peaks=[],
@@ -772,15 +774,16 @@
         iter = 0
         for _, peaks in peak_props.items():
             for _, params in peaks.items():
                 _dict = {'retention_time': params['retention_time'],
                          'scale': params['scale'],
                          'skew': params['alpha'],
                          'amplitude': params['amplitude'],
-                         'area': params['area']}
+                         'area': params['area'],
+                         'signal_maximum': params['signal_max']}
                 iter += 1
                 peak_df = pd.concat([peak_df, pd.DataFrame(_dict, index=[0])])
 
         peak_df.sort_values(by='retention_time', inplace=True)
         peak_df['peak_id'] = np.arange(len(peak_df)) + 1
         peak_df['peak_id'] = peak_df['peak_id'].astype(int)
         self.peaks = peak_df
```

### Comparing `hplc-py-0.2.5/hplc_py.egg-info/PKG-INFO` & `hplc_py-0.2.6/hplc_py.egg-info/PKG-INFO`

 * *Files 12% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: hplc-py
-Version: 0.2.5
+Version: 0.2.6
 Summary: Python utilities for the processing and quantification of chromatograms from High Performance Liquid Chromatography (HPLC).
 Home-page: https://github.com/cremerlab/hplc-py
 Author: Griffin Chure
 Author-email: griffinchure@gmail.com
 License: GPLv3
 Classifier: Development Status :: 4 - Beta
 Classifier: Intended Audience :: Science/Research
@@ -21,16 +21,15 @@
 
 ![](docs/source/_static/homepage_logo.png)
 
 [![License: GPL v3](https://img.shields.io/badge/License-GPLv3-blue.svg)](https://www.gnu.org/licenses/gpl-3.0)
 [![Run tests](https://github.com/cremerlab/hplc-py/actions/workflows/pytest.yaml/badge.svg)](https://github.com/cremerlab/hplc-py/actions/workflows/pytest.yaml)
 [![codecov](https://codecov.io/gh/cremerlab/hplc-py/branch/main/graph/badge.svg?token=WXL50JVR6C)](https://codecov.io/gh/cremerlab/hplc-py)
 [![PyPI version](https://badge.fury.io/py/hplc-py.svg)](https://badge.fury.io/py/hplc-py)
-[![DOI](https://zenodo.org/badge/667610900.svg)](https://zenodo.org/badge/latestdoi/667610900)
-
+[![DOI](https://joss.theoj.org/papers/10.21105/joss.06270/status.svg)](https://doi.org/10.21105/joss.06270)
 
 # About
 
 **H**igh-**P**erformance **L**iquid **C**hromatography (HPLC) is an analytical
 technique which allows for quantitative characterization of the chemical
 components of a mixture. While many of the technical details of HPLC are now
 automated, the programmatic cleaning and processing of the resulting data often requires extensive manual labor. This package was
@@ -107,32 +106,50 @@
 ```python 
 In[6]: peaks = chrom.fit_peaks()
 Performing baseline correction: 100%|████████| 299/299 [00:01<00:00, 167.06it/s]
 Deconvolving mixture: 100%|███████████████████████| 3/3 [00:13<00:00,  4.66s/it]
 
 In[7]: peaks.head()
 Out[7]:   
-   retention_time     scale      skew     amplitude          area  peak_id
-0           10.90  0.157450  0.674286  23250.349387  2.790042e+06        1
-0           13.17  0.582866  3.839860  42250.783974  5.070094e+06        2
-0           14.45  0.353036 -3.019153  35229.583555  4.227550e+06        3
-0           15.53  0.312563  1.630787  14891.041452  1.786925e+06        4
-0           16.52  0.344266  1.984167  10770.656732  1.292479e+06        5
+	retention_time	   scale	    skew	   amplitude	        area	signal_maximum	peak_id
+0			 10.90	0.158768	0.691961	23380.386403	2.805646e+06	66064.361454	1
+0			 13.17	0.592828	3.889788	43048.461053	5.165815e+06	50331.167860	2
+0			 14.45	0.350139   -2.997977	34791.996875	4.175040e+06	65352.588796	3
+0			 15.53	0.308900	1.567356	14938.309504	1.792597e+06	26723.707626	4
+0			 16.55	0.272283	1.261303	9512.727882	    1.141527e+06	18121.299375	5
 ```
 
 The resulting chromatogram reconstruction can be seen by again calling the `show()` 
 method, this time restricting the plotted time region between 10 and 20 minutes.
 
 ```python
 In[8]: chrom.show()
 Out[8]:[<Figure size 640x480 with 1 Axes>,
  <Axes: xlabel='time', ylabel='signal (baseline corrected)'>]
 ```
 ![](example/reconstructed_chromatogram.png)
 
+# Citation
+If you use `hplc-py` in your research please cite the version of the software
+you use along with our [descriptive paper in JOSS](https://joss.theoj.org/papers/10.21105/joss.06270):
+
+```
+@article{chure2024,
+	author = {Chure, Griffin and Cremer, Jonas},
+	title = {hplc-py: A Python Utility For Rapid Quantification of Complex Chemical Chromatograms},
+	volume = 9,
+    number = 94,
+	url = {https://joss.theoj.org/papers/10.21105/joss.06270},
+	doi = {10.21105/joss.06270},
+	number = {94},
+	urldate = {2024-02-16},
+	journal = {Journal of Open Source Software},
+	year = {2024}
+   }
+```
 
 # Contributing
 Development of hplc-py occurs on various feature branches which are merged and released upon approval by Griffin Chure (@gchure), the primary maintainer of the software.
 
 Please submit issues and bug reports using the issue tracker. When filing an
 issue, provide a reproducible example that demonstrates the bug or problem.
 Feature requests can also be made through the issue tracker, though it is up to
```

### Comparing `hplc-py-0.2.5/setup.py` & `hplc_py-0.2.6/setup.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 from setuptools import setup, find_packages
 import pathlib
 
-__version__ = "0.2.5"
+__version__ = "0.2.6"
 
 # The directory containing this file
 HERE = pathlib.Path(__file__).parent
 
 # The text of the README file
 README = (HERE / "README.md").read_text()
```

### Comparing `hplc-py-0.2.5/tests/test_chromatogram.py` & `hplc_py-0.2.6/tests/test_chromatogram.py`

 * *Files 0% similar despite different names*

```diff
@@ -21,15 +21,16 @@
 
 def fit_peaks(test_data, truth, colnames={'time': 'x', 'signal': 'y'}, tol=1.5E-2):
     """
     Uses the `hplc.quant.Chromatogram.quantify` method to fit peaks in a chromatogram
     and compares the value with the ground truth.
     """
     # Define constants
-    props = ['retention_time', 'amplitude', 'area', 'scale', 'skew']
+    props = ['retention_time', 'amplitude',
+             'area', 'scale', 'skew', 'signal_maximum']
 
     # Execute analysis
     chrom = hplc.quant.Chromatogram(test_data, cols=colnames)
     peaks = chrom.fit_peaks(correct_baseline=False, prominence=1E-3)
     assert chrom._fitting_progress_state == 1
 
     # Ensure that proper representation is applied.
```

### Comparing `hplc-py-0.2.5/tests/test_io.py` & `hplc_py-0.2.6/tests/test_io.py`

 * *Files identical despite different names*

