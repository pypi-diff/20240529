# Comparing `tmp/ibl_neuropixel-1.0.0.tar.gz` & `tmp/ibl_neuropixel-1.0.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ibl_neuropixel-1.0.0.tar", last modified: Wed Apr 24 15:06:49 2024, max compression
+gzip compressed data, was "ibl_neuropixel-1.0.1.tar", last modified: Wed May 29 18:38:07 2024, max compression
```

## Comparing `ibl_neuropixel-1.0.0.tar` & `ibl_neuropixel-1.0.1.tar`

### file list

```diff
@@ -1,35 +1,35 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 15:06:49.379966 ibl_neuropixel-1.0.0/
--rw-r--r--   0 runner    (1001) docker     (127)     1087 2024-04-24 15:06:46.000000 ibl_neuropixel-1.0.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)       25 2024-04-24 15:06:46.000000 ibl_neuropixel-1.0.0/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (127)     2156 2024-04-24 15:06:49.379966 ibl_neuropixel-1.0.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     1427 2024-04-24 15:06:46.000000 ibl_neuropixel-1.0.0/README.md
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-24 15:06:49.379966 ibl_neuropixel-1.0.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)     1072 2024-04-24 15:06:46.000000 ibl_neuropixel-1.0.0/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 15:06:49.375966 ibl_neuropixel-1.0.0/src/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 15:06:49.379966 ibl_neuropixel-1.0.0/src/ibl_neuropixel.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     2156 2024-04-24 15:06:49.000000 ibl_neuropixel-1.0.0/src/ibl_neuropixel.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      681 2024-04-24 15:06:49.000000 ibl_neuropixel-1.0.0/src/ibl_neuropixel.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-24 15:06:49.000000 ibl_neuropixel-1.0.0/src/ibl_neuropixel.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       68 2024-04-24 15:06:49.000000 ibl_neuropixel-1.0.0/src/ibl_neuropixel.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       51 2024-04-24 15:06:49.000000 ibl_neuropixel-1.0.0/src/ibl_neuropixel.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 15:06:49.375966 ibl_neuropixel-1.0.0/src/ibldsp/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-24 15:06:46.000000 ibl_neuropixel-1.0.0/src/ibldsp/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     5993 2024-04-24 15:06:46.000000 ibl_neuropixel-1.0.0/src/ibldsp/cadzow.py
--rw-r--r--   0 runner    (1001) docker     (127)     2387 2024-04-24 15:06:46.000000 ibl_neuropixel-1.0.0/src/ibldsp/cuda_tools.py
--rw-r--r--   0 runner    (1001) docker     (127)     2824 2024-04-24 15:06:46.000000 ibl_neuropixel-1.0.0/src/ibldsp/destripe_gpu.py
--rw-r--r--   0 runner    (1001) docker     (127)     5789 2024-04-24 15:06:46.000000 ibl_neuropixel-1.0.0/src/ibldsp/filter_gpu.py
--rw-r--r--   0 runner    (1001) docker     (127)    10607 2024-04-24 15:06:46.000000 ibl_neuropixel-1.0.0/src/ibldsp/fourier.py
--rw-r--r--   0 runner    (1001) docker     (127)     5161 2024-04-24 15:06:46.000000 ibl_neuropixel-1.0.0/src/ibldsp/raw_metrics.py
--rw-r--r--   0 runner    (1001) docker     (127)     8030 2024-04-24 15:06:46.000000 ibl_neuropixel-1.0.0/src/ibldsp/smooth.py
--rw-r--r--   0 runner    (1001) docker     (127)     6874 2024-04-24 15:06:46.000000 ibl_neuropixel-1.0.0/src/ibldsp/spiketrains.py
--rw-r--r--   0 runner    (1001) docker     (127)    10073 2024-04-24 15:06:46.000000 ibl_neuropixel-1.0.0/src/ibldsp/utils.py
--rw-r--r--   0 runner    (1001) docker     (127)    37561 2024-04-24 15:06:46.000000 ibl_neuropixel-1.0.0/src/ibldsp/voltage.py
--rw-r--r--   0 runner    (1001) docker     (127)    14015 2024-04-24 15:06:46.000000 ibl_neuropixel-1.0.0/src/ibldsp/waveform_extraction.py
--rw-r--r--   0 runner    (1001) docker     (127)    28777 2024-04-24 15:06:46.000000 ibl_neuropixel-1.0.0/src/ibldsp/waveforms.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 15:06:49.379966 ibl_neuropixel-1.0.0/src/neurodsp/
--rw-r--r--   0 runner    (1001) docker     (127)      201 2024-04-24 15:06:46.000000 ibl_neuropixel-1.0.0/src/neurodsp/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    36748 2024-04-24 15:06:46.000000 ibl_neuropixel-1.0.0/src/neuropixel.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 15:06:49.379966 ibl_neuropixel-1.0.0/src/neurowaveforms/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-24 15:06:46.000000 ibl_neuropixel-1.0.0/src/neurowaveforms/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     6704 2024-04-24 15:06:46.000000 ibl_neuropixel-1.0.0/src/neurowaveforms/model.py
--rw-r--r--   0 runner    (1001) docker     (127)    37250 2024-04-24 15:06:46.000000 ibl_neuropixel-1.0.0/src/spikeglx.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-29 18:38:07.658453 ibl_neuropixel-1.0.1/
+-rw-r--r--   0 runner    (1001) docker     (127)     1087 2024-05-29 18:38:04.000000 ibl_neuropixel-1.0.1/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)       25 2024-05-29 18:38:04.000000 ibl_neuropixel-1.0.1/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (127)     2156 2024-05-29 18:38:07.658453 ibl_neuropixel-1.0.1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     1427 2024-05-29 18:38:04.000000 ibl_neuropixel-1.0.1/README.md
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-29 18:38:07.658453 ibl_neuropixel-1.0.1/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)     1072 2024-05-29 18:38:04.000000 ibl_neuropixel-1.0.1/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-29 18:38:07.654453 ibl_neuropixel-1.0.1/src/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-29 18:38:07.658453 ibl_neuropixel-1.0.1/src/ibl_neuropixel.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     2156 2024-05-29 18:38:07.000000 ibl_neuropixel-1.0.1/src/ibl_neuropixel.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      681 2024-05-29 18:38:07.000000 ibl_neuropixel-1.0.1/src/ibl_neuropixel.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-29 18:38:07.000000 ibl_neuropixel-1.0.1/src/ibl_neuropixel.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       68 2024-05-29 18:38:07.000000 ibl_neuropixel-1.0.1/src/ibl_neuropixel.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       51 2024-05-29 18:38:07.000000 ibl_neuropixel-1.0.1/src/ibl_neuropixel.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-29 18:38:07.658453 ibl_neuropixel-1.0.1/src/ibldsp/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-29 18:38:04.000000 ibl_neuropixel-1.0.1/src/ibldsp/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5993 2024-05-29 18:38:04.000000 ibl_neuropixel-1.0.1/src/ibldsp/cadzow.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2387 2024-05-29 18:38:04.000000 ibl_neuropixel-1.0.1/src/ibldsp/cuda_tools.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2824 2024-05-29 18:38:04.000000 ibl_neuropixel-1.0.1/src/ibldsp/destripe_gpu.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5789 2024-05-29 18:38:04.000000 ibl_neuropixel-1.0.1/src/ibldsp/filter_gpu.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10607 2024-05-29 18:38:04.000000 ibl_neuropixel-1.0.1/src/ibldsp/fourier.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5161 2024-05-29 18:38:04.000000 ibl_neuropixel-1.0.1/src/ibldsp/raw_metrics.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8030 2024-05-29 18:38:04.000000 ibl_neuropixel-1.0.1/src/ibldsp/smooth.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6874 2024-05-29 18:38:04.000000 ibl_neuropixel-1.0.1/src/ibldsp/spiketrains.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10141 2024-05-29 18:38:04.000000 ibl_neuropixel-1.0.1/src/ibldsp/utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)    37561 2024-05-29 18:38:04.000000 ibl_neuropixel-1.0.1/src/ibldsp/voltage.py
+-rw-r--r--   0 runner    (1001) docker     (127)    13983 2024-05-29 18:38:04.000000 ibl_neuropixel-1.0.1/src/ibldsp/waveform_extraction.py
+-rw-r--r--   0 runner    (1001) docker     (127)    28777 2024-05-29 18:38:04.000000 ibl_neuropixel-1.0.1/src/ibldsp/waveforms.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-29 18:38:07.658453 ibl_neuropixel-1.0.1/src/neurodsp/
+-rw-r--r--   0 runner    (1001) docker     (127)      201 2024-05-29 18:38:04.000000 ibl_neuropixel-1.0.1/src/neurodsp/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    36748 2024-05-29 18:38:04.000000 ibl_neuropixel-1.0.1/src/neuropixel.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-29 18:38:07.658453 ibl_neuropixel-1.0.1/src/neurowaveforms/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-29 18:38:04.000000 ibl_neuropixel-1.0.1/src/neurowaveforms/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6704 2024-05-29 18:38:04.000000 ibl_neuropixel-1.0.1/src/neurowaveforms/model.py
+-rw-r--r--   0 runner    (1001) docker     (127)    37753 2024-05-29 18:38:04.000000 ibl_neuropixel-1.0.1/src/spikeglx.py
```

### Comparing `ibl_neuropixel-1.0.0/LICENSE` & `ibl_neuropixel-1.0.1/LICENSE`

 * *Files identical despite different names*

### Comparing `ibl_neuropixel-1.0.0/PKG-INFO` & `ibl_neuropixel-1.0.1/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ibl-neuropixel
-Version: 1.0.0
+Version: 1.0.1
 Summary: Collection of tools for Neuropixel 1.0 and 2.0 probes data
 Home-page: https://github.com/int-brain-lab/ibl-neuropixel
 Author: The International Brain Laboratory
 Project-URL: Bug Tracker, https://github.com/int-brain-lab/ibl-neuropixel/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
@@ -58,17 +58,17 @@
 ### White Paper
 The following describes the methods implemented in this repository.
 https://doi.org/10.6084/m9.figshare.19705522
 
 ## Contribution
 
 Pypi Release checklist:
-Edit the version number in `setup.py`, and add release notes in `release_notes.md`
+- Edit the version number in `setup.py`, and add release notes in `release_notes.md`
 
 ```shell
 flake8
-tag=vX.Y.Z
+tag=X.Y.Z
 git tag -a $tag 
 git push origin %tag
 ```
 
-Create new release with tag vX.Y.Z (will automatically publish to PyPI)
+Create new release with tag X.Y.Z (will automatically publish to PyPI)
```

### Comparing `ibl_neuropixel-1.0.0/README.md` & `ibl_neuropixel-1.0.1/README.md`

 * *Files 2% similar despite different names*

```diff
@@ -36,17 +36,17 @@
 ### White Paper
 The following describes the methods implemented in this repository.
 https://doi.org/10.6084/m9.figshare.19705522
 
 ## Contribution
 
 Pypi Release checklist:
-Edit the version number in `setup.py`, and add release notes in `release_notes.md`
+- Edit the version number in `setup.py`, and add release notes in `release_notes.md`
 
 ```shell
 flake8
-tag=vX.Y.Z
+tag=X.Y.Z
 git tag -a $tag 
 git push origin %tag
 ```
 
-Create new release with tag vX.Y.Z (will automatically publish to PyPI)
+Create new release with tag X.Y.Z (will automatically publish to PyPI)
```

### Comparing `ibl_neuropixel-1.0.0/setup.py` & `ibl_neuropixel-1.0.1/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -4,15 +4,15 @@
     long_description = fh.read()
 
 with open("requirements.txt") as f:
     require = [x.strip() for x in f.readlines() if not x.startswith("git+")]
 
 setuptools.setup(
     name="ibl-neuropixel",
-    version="1.0.0",
+    version="1.0.1",
     author="The International Brain Laboratory",
     description="Collection of tools for Neuropixel 1.0 and 2.0 probes data",
     long_description=long_description,
     long_description_content_type="text/markdown",
     url="https://github.com/int-brain-lab/ibl-neuropixel",
     project_urls={
         "Bug Tracker": "https://github.com/int-brain-lab/ibl-neuropixel/issues",
```

### Comparing `ibl_neuropixel-1.0.0/src/ibl_neuropixel.egg-info/PKG-INFO` & `ibl_neuropixel-1.0.1/src/ibl_neuropixel.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ibl-neuropixel
-Version: 1.0.0
+Version: 1.0.1
 Summary: Collection of tools for Neuropixel 1.0 and 2.0 probes data
 Home-page: https://github.com/int-brain-lab/ibl-neuropixel
 Author: The International Brain Laboratory
 Project-URL: Bug Tracker, https://github.com/int-brain-lab/ibl-neuropixel/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
@@ -58,17 +58,17 @@
 ### White Paper
 The following describes the methods implemented in this repository.
 https://doi.org/10.6084/m9.figshare.19705522
 
 ## Contribution
 
 Pypi Release checklist:
-Edit the version number in `setup.py`, and add release notes in `release_notes.md`
+- Edit the version number in `setup.py`, and add release notes in `release_notes.md`
 
 ```shell
 flake8
-tag=vX.Y.Z
+tag=X.Y.Z
 git tag -a $tag 
 git push origin %tag
 ```
 
-Create new release with tag vX.Y.Z (will automatically publish to PyPI)
+Create new release with tag X.Y.Z (will automatically publish to PyPI)
```

### Comparing `ibl_neuropixel-1.0.0/src/ibl_neuropixel.egg-info/SOURCES.txt` & `ibl_neuropixel-1.0.1/src/ibl_neuropixel.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `ibl_neuropixel-1.0.0/src/ibldsp/cadzow.py` & `ibl_neuropixel-1.0.1/src/ibldsp/cadzow.py`

 * *Files identical despite different names*

### Comparing `ibl_neuropixel-1.0.0/src/ibldsp/cuda_tools.py` & `ibl_neuropixel-1.0.1/src/ibldsp/cuda_tools.py`

 * *Files identical despite different names*

### Comparing `ibl_neuropixel-1.0.0/src/ibldsp/destripe_gpu.py` & `ibl_neuropixel-1.0.1/src/ibldsp/destripe_gpu.py`

 * *Files identical despite different names*

### Comparing `ibl_neuropixel-1.0.0/src/ibldsp/filter_gpu.py` & `ibl_neuropixel-1.0.1/src/ibldsp/filter_gpu.py`

 * *Files identical despite different names*

### Comparing `ibl_neuropixel-1.0.0/src/ibldsp/fourier.py` & `ibl_neuropixel-1.0.1/src/ibldsp/fourier.py`

 * *Files identical despite different names*

### Comparing `ibl_neuropixel-1.0.0/src/ibldsp/raw_metrics.py` & `ibl_neuropixel-1.0.1/src/ibldsp/raw_metrics.py`

 * *Files identical despite different names*

### Comparing `ibl_neuropixel-1.0.0/src/ibldsp/smooth.py` & `ibl_neuropixel-1.0.1/src/ibldsp/smooth.py`

 * *Files identical despite different names*

### Comparing `ibl_neuropixel-1.0.0/src/ibldsp/spiketrains.py` & `ibl_neuropixel-1.0.1/src/ibldsp/spiketrains.py`

 * *Files identical despite different names*

### Comparing `ibl_neuropixel-1.0.0/src/ibldsp/utils.py` & `ibl_neuropixel-1.0.1/src/ibldsp/utils.py`

 * *Files 2% similar despite different names*

```diff
@@ -210,23 +210,24 @@
     :param x: array on which to compute RMS
     :param axis: (optional, -1)
     :return: numpy array
     """
     return np.sqrt(np.mean(x**2, axis=axis))
 
 
-def make_channel_index(geom, radius=200.0, pad_val=384):
+def make_channel_index(geom, radius=200.0, pad_val=None):
     """
     Given a neuropixels geometry dict `geom`, returns an array with nc rows
     where the i'th row contains the channel ids that fall within `radius` um
     of channel i. The number of columns is the maximum number of neighbors a
     channel can have and will depend on the geometry and the radius chosen.
 
     For channels at the edges of the probe which have less than the maximum possible
-    number of neighbors, the remaining indices in the row are filled with `pad_val`.
+    number of neighbors, the remaining indices in the row are filled with `pad_val`,
+    which defaults to the number of channels (ie. last index + 1).
     """
     neighbors = (
         scipy.spatial.distance.squareform(scipy.spatial.distance.pdist(geom)) <= radius
     )
     n_nbors = np.max(np.sum(neighbors, 0))
 
     nc = geom.shape[0]
```

### Comparing `ibl_neuropixel-1.0.0/src/ibldsp/voltage.py` & `ibl_neuropixel-1.0.1/src/ibldsp/voltage.py`

 * *Files identical despite different names*

### Comparing `ibl_neuropixel-1.0.0/src/ibldsp/waveform_extraction.py` & `ibl_neuropixel-1.0.1/src/ibldsp/waveform_extraction.py`

 * *Files 1% similar despite different names*

```diff
@@ -2,15 +2,14 @@
 
 import scipy
 import pandas as pd
 import numpy as np
 from numpy.lib.format import open_memmap
 from joblib import Parallel, delayed, cpu_count
 
-import neuropixel
 import spikeglx
 from ibldsp.voltage import detect_bad_channels, interpolate_bad_channels, car
 from ibldsp.fourier import fshift
 from ibldsp.utils import make_channel_index
 
 logger = logging.getLogger(__name__)
 
@@ -267,20 +266,20 @@
 
     - waveforms.table.pqt: `num_units * max_wf` rows
         For each waveform, gives the absolute sample number from the recording (i.e.
         where to find it in `spikes.samples`), peak channel, cluster, and linear index.
         A row of -1s implies that the waveform is missing because the unit is was supposed
         to come from has less than `max_wf` spikes total.
     """
-    if h is None:
-        h = neuropixel.trace_header()
-
     n_jobs = n_jobs or int(cpu_count() / 2)
 
     sr = spikeglx.Reader(cbin_file)
+    if h is None:
+        h = sr.geometry
+
     s0_arr = np.arange(0, sr.ns, chunksize_samples)
     s1_arr = s0_arr + chunksize_samples
     s1_arr[-1] = sr.ns
 
     # selects spikes from throughout the recording for each unit
     wf_flat, unit_ids = _make_wfs_table(
         sr,
```

### Comparing `ibl_neuropixel-1.0.0/src/ibldsp/waveforms.py` & `ibl_neuropixel-1.0.1/src/ibldsp/waveforms.py`

 * *Files identical despite different names*

### Comparing `ibl_neuropixel-1.0.0/src/neuropixel.py` & `ibl_neuropixel-1.0.1/src/neuropixel.py`

 * *Files identical despite different names*

### Comparing `ibl_neuropixel-1.0.0/src/neurowaveforms/model.py` & `ibl_neuropixel-1.0.1/src/neurowaveforms/model.py`

 * *Files identical despite different names*

### Comparing `ibl_neuropixel-1.0.0/src/spikeglx.py` & `ibl_neuropixel-1.0.1/src/spikeglx.py`

 * *Files 0% similar despite different names*

```diff
@@ -4,22 +4,33 @@
 import re
 
 import numpy as np
 
 import mtscomp
 from iblutil.io import hashfile
 from iblutil.util import Bunch
+import one.alf.files
 
 import neuropixel
 
 SAMPLE_SIZE = 2  # int16
 DEFAULT_BATCH_SIZE = 1e6
 _logger = logging.getLogger("ibllib")
 
 
+def _get_companion_file(sglx_file, pattern='.meta'):
+    # on SDSC there is a possibility that there is an UUID string in the filename
+    sglx_file = Path(sglx_file)
+    companion_file = sglx_file.with_suffix(pattern)
+    if not companion_file.exists():
+        search_pattern = f"{one.alf.files.remove_uuid_string(sglx_file).stem}*{pattern}"
+        companion_file = next(sglx_file.parent.glob(search_pattern), companion_file)
+    return companion_file
+
+
 class Reader:
     """
     Class for SpikeGLX reading purposes
     Some format description was found looking at the Matlab SDK here
     https://github.com/billkarsh/SpikeGLX/blob/master/MATLAB-SDK/DemoReadSGLXData.m
 
     To open a spikeglx file that has an associated meta-data file:
@@ -55,15 +66,15 @@
         """
         An interface for reading data from a SpikeGLX file
         :param sglx_file: Path to a SpikeGLX file (compressed or otherwise), or to a meta-data file
         :param open: when True the file is opened
         """
         self.ignore_warnings = ignore_warnings
         sglx_file = Path(sglx_file)
-        meta_file = meta_file or sglx_file.with_suffix(".meta")
+        meta_file = meta_file or _get_companion_file(sglx_file, '.meta')
         # only used if MTSCOMP compressed
         self.ch_file = ch_file
 
         if meta_file == sglx_file:
             # if a meta-data file is provided, try to get the binary file
             self.file_bin = (
                 sglx_file.with_suffix(".cbin")
@@ -116,15 +127,15 @@
             self.open()
 
     def open(self):
         # if we are not looking at a compressed file, use a memmap, otherwise instantiate mtscomp
         sglx_file = str(self.file_bin)
         if self.is_mtscomp:
             self._raw = mtscomp.Reader()
-            ch_file = self.ch_file or self.file_bin.with_suffix(".ch")
+            ch_file = self.ch_file or _get_companion_file(sglx_file, '.ch')
             self._raw.open(self.file_bin, ch_file)
             if self._raw.shape != (self.ns, self.nc):
                 ftsec = self._raw.shape[0] / self.fs
                 if not self.ignore_warnings:  # avoid the checks for streaming data
                     _logger.warning(
                         f"{sglx_file} : meta data and compressed chunks dont checkout\n"
                         f"File duration: expected {self.meta['fileTimeSecs']},"
```

