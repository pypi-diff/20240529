# Comparing `tmp/scatcluster-0.0.84.tar.gz` & `tmp/scatcluster-0.0.85.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "scatcluster-0.0.84.tar", last modified: Tue May 28 21:14:06 2024, max compression
+gzip compressed data, was "scatcluster-0.0.85.tar", last modified: Tue May 28 21:18:30 2024, max compression
```

## Comparing `scatcluster-0.0.84.tar` & `scatcluster-0.0.85.tar`

### file list

```diff
@@ -1,30 +1,30 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-28 21:14:06.328552 scatcluster-0.0.84/
--rw-r--r--   0 runner    (1001) docker     (127)     1075 2024-05-28 21:14:03.000000 scatcluster-0.0.84/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)       18 2024-05-28 21:14:03.000000 scatcluster-0.0.84/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (127)     1812 2024-05-28 21:14:06.324551 scatcluster-0.0.84/PKG-INFO
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-28 21:14:06.320551 scatcluster-0.0.84/scatcluster/
--rw-r--r--   0 runner    (1001) docker     (127)       44 2024-05-28 21:14:03.000000 scatcluster-0.0.84/scatcluster/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-28 21:14:06.324551 scatcluster-0.0.84/scatcluster/analysis/
--rw-r--r--   0 runner    (1001) docker     (127)       20 2024-05-28 21:14:03.000000 scatcluster-0.0.84/scatcluster/analysis/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    16133 2024-05-28 21:14:03.000000 scatcluster-0.0.84/scatcluster/analysis/crosstab.py
--rw-r--r--   0 runner    (1001) docker     (127)    27938 2024-05-28 21:14:03.000000 scatcluster-0.0.84/scatcluster/analysis/dendrogram.py
--rw-r--r--   0 runner    (1001) docker     (127)    19119 2024-05-28 21:14:03.000000 scatcluster-0.0.84/scatcluster/analysis/external_correlation.py
--rw-r--r--   0 runner    (1001) docker     (127)     5348 2024-05-28 21:14:03.000000 scatcluster-0.0.84/scatcluster/analysis/predictions.py
--rw-r--r--   0 runner    (1001) docker     (127)     5841 2024-05-28 21:14:03.000000 scatcluster-0.0.84/scatcluster/analysis/processing.py
--rw-r--r--   0 runner    (1001) docker     (127)    19398 2024-05-28 21:14:03.000000 scatcluster-0.0.84/scatcluster/analysis/waveform_correlations.py
--rw-r--r--   0 runner    (1001) docker     (127)    21374 2024-05-28 21:14:03.000000 scatcluster-0.0.84/scatcluster/analysis/waveforms.py
--rw-r--r--   0 runner    (1001) docker     (127)     3452 2024-05-28 21:14:03.000000 scatcluster-0.0.84/scatcluster/helper.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-28 21:14:06.324551 scatcluster-0.0.84/scatcluster/processing/
--rw-r--r--   0 runner    (1001) docker     (127)       22 2024-05-28 21:14:03.000000 scatcluster-0.0.84/scatcluster/processing/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    16143 2024-05-28 21:14:03.000000 scatcluster-0.0.84/scatcluster/processing/ica.py
--rw-r--r--   0 runner    (1001) docker     (127)    28424 2024-05-28 21:14:03.000000 scatcluster-0.0.84/scatcluster/processing/scattering.py
--rw-r--r--   0 runner    (1001) docker     (127)     8253 2024-05-28 21:14:03.000000 scatcluster-0.0.84/scatcluster/scatcluster.py
--rw-r--r--   0 runner    (1001) docker     (127)     6396 2024-05-28 21:14:03.000000 scatcluster-0.0.84/scatcluster/structure.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-28 21:14:06.324551 scatcluster-0.0.84/scatcluster.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     1812 2024-05-28 21:14:06.000000 scatcluster-0.0.84/scatcluster.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      699 2024-05-28 21:14:06.000000 scatcluster-0.0.84/scatcluster.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-28 21:14:06.000000 scatcluster-0.0.84/scatcluster.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)      250 2024-05-28 21:14:06.000000 scatcluster-0.0.84/scatcluster.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       12 2024-05-28 21:14:06.000000 scatcluster-0.0.84/scatcluster.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-28 21:14:06.328552 scatcluster-0.0.84/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)     1659 2024-05-28 21:14:03.000000 scatcluster-0.0.84/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-28 21:18:30.953658 scatcluster-0.0.85/
+-rw-r--r--   0 runner    (1001) docker     (127)     1075 2024-05-28 21:18:27.000000 scatcluster-0.0.85/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)       18 2024-05-28 21:18:27.000000 scatcluster-0.0.85/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (127)     1812 2024-05-28 21:18:30.953658 scatcluster-0.0.85/PKG-INFO
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-28 21:18:30.949658 scatcluster-0.0.85/scatcluster/
+-rw-r--r--   0 runner    (1001) docker     (127)       44 2024-05-28 21:18:27.000000 scatcluster-0.0.85/scatcluster/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-28 21:18:30.953658 scatcluster-0.0.85/scatcluster/analysis/
+-rw-r--r--   0 runner    (1001) docker     (127)       20 2024-05-28 21:18:27.000000 scatcluster-0.0.85/scatcluster/analysis/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    16133 2024-05-28 21:18:27.000000 scatcluster-0.0.85/scatcluster/analysis/crosstab.py
+-rw-r--r--   0 runner    (1001) docker     (127)    27938 2024-05-28 21:18:27.000000 scatcluster-0.0.85/scatcluster/analysis/dendrogram.py
+-rw-r--r--   0 runner    (1001) docker     (127)    19119 2024-05-28 21:18:27.000000 scatcluster-0.0.85/scatcluster/analysis/external_correlation.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5348 2024-05-28 21:18:27.000000 scatcluster-0.0.85/scatcluster/analysis/predictions.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5841 2024-05-28 21:18:27.000000 scatcluster-0.0.85/scatcluster/analysis/processing.py
+-rw-r--r--   0 runner    (1001) docker     (127)    19398 2024-05-28 21:18:27.000000 scatcluster-0.0.85/scatcluster/analysis/waveform_correlations.py
+-rw-r--r--   0 runner    (1001) docker     (127)    21374 2024-05-28 21:18:27.000000 scatcluster-0.0.85/scatcluster/analysis/waveforms.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3452 2024-05-28 21:18:27.000000 scatcluster-0.0.85/scatcluster/helper.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-28 21:18:30.953658 scatcluster-0.0.85/scatcluster/processing/
+-rw-r--r--   0 runner    (1001) docker     (127)       22 2024-05-28 21:18:27.000000 scatcluster-0.0.85/scatcluster/processing/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    16143 2024-05-28 21:18:27.000000 scatcluster-0.0.85/scatcluster/processing/ica.py
+-rw-r--r--   0 runner    (1001) docker     (127)    29497 2024-05-28 21:18:27.000000 scatcluster-0.0.85/scatcluster/processing/scattering.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8253 2024-05-28 21:18:27.000000 scatcluster-0.0.85/scatcluster/scatcluster.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6396 2024-05-28 21:18:27.000000 scatcluster-0.0.85/scatcluster/structure.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-28 21:18:30.953658 scatcluster-0.0.85/scatcluster.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     1812 2024-05-28 21:18:30.000000 scatcluster-0.0.85/scatcluster.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      699 2024-05-28 21:18:30.000000 scatcluster-0.0.85/scatcluster.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-28 21:18:30.000000 scatcluster-0.0.85/scatcluster.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      250 2024-05-28 21:18:30.000000 scatcluster-0.0.85/scatcluster.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       12 2024-05-28 21:18:30.000000 scatcluster-0.0.85/scatcluster.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-28 21:18:30.953658 scatcluster-0.0.85/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)     1659 2024-05-28 21:18:27.000000 scatcluster-0.0.85/setup.py
```

### Comparing `scatcluster-0.0.84/LICENSE` & `scatcluster-0.0.85/LICENSE`

 * *Files identical despite different names*

### Comparing `scatcluster-0.0.84/PKG-INFO` & `scatcluster-0.0.85/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: scatcluster
-Version: 0.0.84
+Version: 0.0.85
 Summary: A workflow for clustering continuous time series with a deep scattering network.
 Home-page: https://github.com/INGV/ScatCluster
 Author: christopher.zerafa@ingv.it
 License: MIT
 Classifier: Intended Audience :: Science/Research
 Classifier: License :: OSI Approved :: GNU General Public License v3 (GPLv3)
 Classifier: Programming Language :: Python
```

### Comparing `scatcluster-0.0.84/scatcluster/analysis/crosstab.py` & `scatcluster-0.0.85/scatcluster/analysis/crosstab.py`

 * *Files identical despite different names*

### Comparing `scatcluster-0.0.84/scatcluster/analysis/dendrogram.py` & `scatcluster-0.0.85/scatcluster/analysis/dendrogram.py`

 * *Files identical despite different names*

### Comparing `scatcluster-0.0.84/scatcluster/analysis/external_correlation.py` & `scatcluster-0.0.85/scatcluster/analysis/external_correlation.py`

 * *Files identical despite different names*

### Comparing `scatcluster-0.0.84/scatcluster/analysis/predictions.py` & `scatcluster-0.0.85/scatcluster/analysis/predictions.py`

 * *Files identical despite different names*

### Comparing `scatcluster-0.0.84/scatcluster/analysis/processing.py` & `scatcluster-0.0.85/scatcluster/analysis/processing.py`

 * *Files identical despite different names*

### Comparing `scatcluster-0.0.84/scatcluster/analysis/waveform_correlations.py` & `scatcluster-0.0.85/scatcluster/analysis/waveform_correlations.py`

 * *Files identical despite different names*

### Comparing `scatcluster-0.0.84/scatcluster/analysis/waveforms.py` & `scatcluster-0.0.85/scatcluster/analysis/waveforms.py`

 * *Files identical despite different names*

### Comparing `scatcluster-0.0.84/scatcluster/helper.py` & `scatcluster-0.0.85/scatcluster/helper.py`

 * *Files identical despite different names*

### Comparing `scatcluster-0.0.84/scatcluster/processing/ica.py` & `scatcluster-0.0.85/scatcluster/processing/ica.py`

 * *Files identical despite different names*

### Comparing `scatcluster-0.0.84/scatcluster/processing/scattering.py` & `scatcluster-0.0.85/scatcluster/processing/scattering.py`

 * *Files 1% similar despite different names*

```diff
@@ -617,14 +617,39 @@
         """
         scat_coeff_xr = xr.open_dataset(
             f'{self.data_savepath}data/{self.data_network}_{self.data_station}_{self.data_location}_'
             f'{self.network_name}_scat_coef_xarray.nc')
         self.scattering_coefficients_xarray = scat_coeff_xr
         return scat_coeff_xr
 
+    
+    def plot_scattering_coefficients_normalisation(self):
+        """
+        Plot the normalization of scattering coefficients. 
+        This function loads the scattering coefficients from an xarray dataset file and plots the normalization of the coefficients. The plot is saved as a PNG file in the specified directory.
+
+        Parameters:
+            self (object): The instance of the class.
+
+        Returns:
+            None
+        """
+        scat_vec = self.vectorize_scattering_coefficients_xarray(self.load_scattering_coefficients_xarray())
+        _, axs = plt.subplots(1, 1, figsize=(10, 7))
+        for col in range(scat_vec.shape[1]):
+            axs.plot(scat_vec[col], 'b', alpha=0.1)
+        plt.title(f'{self.data_network}_{self.data_station}_{self.data_location}_{self.network_name}\n'
+                'Scattering Coefficients Normalization')
+        
+        plt.savefig(
+                f'{self.data_network}_{self.data_station}_{self.data_location}_{self.network_name}_Scattering_Coefficients_Normalization.png')
+
+        plt.show()
+    
+    
     def preload_times(self):
         """
         Preloads the times data from a numpy file and assigns it to the `data_times` attribute of the class.
 
         """
         data_times = np.load(f'{self.data_savepath}data/{self.data_network}_{self.data_station}_{self.data_location}_'
                              f'{self.network_name}_times.npy')
```

### Comparing `scatcluster-0.0.84/scatcluster/scatcluster.py` & `scatcluster-0.0.85/scatcluster/scatcluster.py`

 * *Files identical despite different names*

### Comparing `scatcluster-0.0.84/scatcluster/structure.py` & `scatcluster-0.0.85/scatcluster/structure.py`

 * *Files identical despite different names*

### Comparing `scatcluster-0.0.84/scatcluster.egg-info/PKG-INFO` & `scatcluster-0.0.85/scatcluster.egg-info/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: scatcluster
-Version: 0.0.84
+Version: 0.0.85
 Summary: A workflow for clustering continuous time series with a deep scattering network.
 Home-page: https://github.com/INGV/ScatCluster
 Author: christopher.zerafa@ingv.it
 License: MIT
 Classifier: Intended Audience :: Science/Research
 Classifier: License :: OSI Approved :: GNU General Public License v3 (GPLv3)
 Classifier: Programming Language :: Python
```

### Comparing `scatcluster-0.0.84/scatcluster.egg-info/SOURCES.txt` & `scatcluster-0.0.85/scatcluster.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `scatcluster-0.0.84/setup.py` & `scatcluster-0.0.85/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -18,15 +18,15 @@
 REQUIRED_GPU = [
     'cupy>=11.3.0',
 ]
 
 setup(
     name=NAME,
     author=AUTHOR,
-    version='0.0.84',
+    version='0.0.85',
     description=DESCRIPTION,
     long_description=DESCRIPTION,
     long_description_content_type='text/markdown',
     python_requires=REQUIRES_PYTHON,
     url=URL,
     packages=find_packages(where='.'),
     package_data={NAME: ['scatcluster/*.py']},
```

