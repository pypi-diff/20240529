# Comparing `tmp/distancerasters-0.3.2.tar.gz` & `tmp/distancerasters-0.3.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "distancerasters-0.3.2.tar", last modified: Mon Feb 13 14:11:40 2023, max compression
+gzip compressed data, was "distancerasters-0.3.3.tar", last modified: Wed May 29 18:01:26 2024, max compression
```

## Comparing `distancerasters-0.3.2.tar` & `distancerasters-0.3.3.tar`

### file list

```diff
@@ -1,20 +1,20 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-13 14:11:40.707761 distancerasters-0.3.2/
--rw-r--r--   0 runner    (1001) docker     (123)     1481 2023-02-13 14:11:25.000000 distancerasters-0.3.2/LICENSE.txt
--rw-r--r--   0 runner    (1001) docker     (123)     7269 2023-02-13 14:11:40.707761 distancerasters-0.3.2/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     6753 2023-02-13 14:11:25.000000 distancerasters-0.3.2/README.md
--rw-r--r--   0 runner    (1001) docker     (123)      104 2023-02-13 14:11:25.000000 distancerasters-0.3.2/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)      740 2023-02-13 14:11:40.707761 distancerasters-0.3.2/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-13 14:11:40.703761 distancerasters-0.3.2/src/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-13 14:11:40.707761 distancerasters-0.3.2/src/distancerasters/
--rw-r--r--   0 runner    (1001) docker     (123)      101 2023-02-13 14:11:25.000000 distancerasters-0.3.2/src/distancerasters/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3928 2023-02-13 14:11:25.000000 distancerasters-0.3.2/src/distancerasters/main.py
--rw-r--r--   0 runner    (1001) docker     (123)     7239 2023-02-13 14:11:25.000000 distancerasters-0.3.2/src/distancerasters/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-13 14:11:40.707761 distancerasters-0.3.2/src/distancerasters.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     7269 2023-02-13 14:11:40.000000 distancerasters-0.3.2/src/distancerasters.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      388 2023-02-13 14:11:40.000000 distancerasters-0.3.2/src/distancerasters.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-02-13 14:11:40.000000 distancerasters-0.3.2/src/distancerasters.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       53 2023-02-13 14:11:40.000000 distancerasters-0.3.2/src/distancerasters.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       16 2023-02-13 14:11:40.000000 distancerasters-0.3.2/src/distancerasters.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-13 14:11:40.707761 distancerasters-0.3.2/tests/
--rw-r--r--   0 runner    (1001) docker     (123)     2843 2023-02-13 14:11:25.000000 distancerasters-0.3.2/tests/test_main.py
--rw-r--r--   0 runner    (1001) docker     (123)     6579 2023-02-13 14:11:25.000000 distancerasters-0.3.2/tests/test_utils.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-29 18:01:26.968737 distancerasters-0.3.3/
+-rw-r--r--   0 runner    (1001) docker     (127)     1481 2024-05-29 18:01:22.000000 distancerasters-0.3.3/LICENSE.txt
+-rw-r--r--   0 runner    (1001) docker     (127)     7414 2024-05-29 18:01:26.968737 distancerasters-0.3.3/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     6735 2024-05-29 18:01:22.000000 distancerasters-0.3.3/README.md
+-rw-r--r--   0 runner    (1001) docker     (127)      104 2024-05-29 18:01:22.000000 distancerasters-0.3.3/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)      746 2024-05-29 18:01:26.968737 distancerasters-0.3.3/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-29 18:01:26.964738 distancerasters-0.3.3/src/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-29 18:01:26.964738 distancerasters-0.3.3/src/distancerasters/
+-rw-r--r--   0 runner    (1001) docker     (127)      101 2024-05-29 18:01:22.000000 distancerasters-0.3.3/src/distancerasters/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4081 2024-05-29 18:01:22.000000 distancerasters-0.3.3/src/distancerasters/main.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7239 2024-05-29 18:01:22.000000 distancerasters-0.3.3/src/distancerasters/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-29 18:01:26.968737 distancerasters-0.3.3/src/distancerasters.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     7414 2024-05-29 18:01:26.000000 distancerasters-0.3.3/src/distancerasters.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      388 2024-05-29 18:01:26.000000 distancerasters-0.3.3/src/distancerasters.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-29 18:01:26.000000 distancerasters-0.3.3/src/distancerasters.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       58 2024-05-29 18:01:26.000000 distancerasters-0.3.3/src/distancerasters.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       16 2024-05-29 18:01:26.000000 distancerasters-0.3.3/src/distancerasters.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-29 18:01:26.968737 distancerasters-0.3.3/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)     2843 2024-05-29 18:01:22.000000 distancerasters-0.3.3/tests/test_main.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6579 2024-05-29 18:01:22.000000 distancerasters-0.3.3/tests/test_utils.py
```

### Comparing `distancerasters-0.3.2/LICENSE.txt` & `distancerasters-0.3.3/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `distancerasters-0.3.2/PKG-INFO` & `distancerasters-0.3.3/README.md`

 * *Files 3% similar despite different names*

```diff
@@ -1,21 +1,7 @@
-Metadata-Version: 2.1
-Name: distancerasters
-Version: 0.3.2
-Summary: Generate distance raster using arbitrary sets of spatial features
-Home-page: https://github.com/sgoodm/python-distance-rasters
-Author: Seth Goodman
-Author-email: sgoodman@aiddata.wm.edu
-License: BSD 3-Clause License
-Project-URL: Bug Tracker, https://github.com/sgoodm/python-distance-rasters/issues
-Keywords: raster,distance,spatial
-Classifier: Programming Language :: Python :: 3
-Description-Content-Type: text/markdown
-License-File: LICENSE.txt
-
 # distance-rasters
 
 Generate distance raster using arbitrary sets of spatial features
 
 [![build badge](https://github.com/sgoodm/python-distance-rasters/actions/workflows/test-with-coverage.yml/badge.svg)](https://github.com/sgoodm/python-distance-rasters/actions/workflows/test-and-coverage.yml)
 [![Coverage Status](https://coveralls.io/repos/github/sgoodm/python-distance-rasters/badge.svg)](https://coveralls.io/github/sgoodm/python-distance-rasters)
 [![Downloads](https://static.pepy.tech/personalized-badge/distancerasters?period=total&units=international_system&left_color=lightgrey&right_color=brightgreen&left_text=Downloads)](https://pepy.tech/project/distancerasters)
@@ -131,15 +117,15 @@
 We use Pytest and Coveralls to run unit tests and track code coverage of tests. If you submit code, please make sure it passes existing tests and adds relevant testing coverage for new features.
 
 You can run tests and coverage checks locally, or you can fork the repository and utilize GitHub actions and Coveralls. To use GitHub actions and Coveralls, you'll need to add your forked repo to your own Coverall accounts and add you Coveralls token to your repository as a GitHub Secret (see below).
 
 
 To run tests and coverage checks locally, you can use the following commands:
 ```sh
-pip install pytest coverage shapely geopandas
+pip install pytest coverage
 coverage run -m pytest ./
 coverage html
 ```
 
 ### GitHub Secrets
 
 There are three GitHub Secrets required to enable all of our GitHub Actions:
```

### Comparing `distancerasters-0.3.2/README.md` & `distancerasters-0.3.3/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,7 +1,28 @@
+Metadata-Version: 2.1
+Name: distancerasters
+Version: 0.3.3
+Summary: Generate distance raster using arbitrary sets of spatial features
+Home-page: https://github.com/sgoodm/python-distance-rasters
+Author: Seth Goodman
+Author-email: sgoodman@aiddata.wm.edu
+License: BSD 3-Clause License
+Project-URL: Bug Tracker, https://github.com/sgoodm/python-distance-rasters/issues
+Keywords: raster,distance,spatial
+Classifier: Programming Language :: Python :: 3
+Description-Content-Type: text/markdown
+License-File: LICENSE.txt
+Requires-Dist: numpy
+Requires-Dist: rasterio
+Requires-Dist: fiona
+Requires-Dist: affine
+Requires-Dist: scipy>=1.6.0
+Requires-Dist: rasterstats
+Requires-Dist: tqdm
+
 # distance-rasters
 
 Generate distance raster using arbitrary sets of spatial features
 
 [![build badge](https://github.com/sgoodm/python-distance-rasters/actions/workflows/test-with-coverage.yml/badge.svg)](https://github.com/sgoodm/python-distance-rasters/actions/workflows/test-and-coverage.yml)
 [![Coverage Status](https://coveralls.io/repos/github/sgoodm/python-distance-rasters/badge.svg)](https://coveralls.io/github/sgoodm/python-distance-rasters)
 [![Downloads](https://static.pepy.tech/personalized-badge/distancerasters?period=total&units=international_system&left_color=lightgrey&right_color=brightgreen&left_text=Downloads)](https://pepy.tech/project/distancerasters)
@@ -117,15 +138,15 @@
 We use Pytest and Coveralls to run unit tests and track code coverage of tests. If you submit code, please make sure it passes existing tests and adds relevant testing coverage for new features.
 
 You can run tests and coverage checks locally, or you can fork the repository and utilize GitHub actions and Coveralls. To use GitHub actions and Coveralls, you'll need to add your forked repo to your own Coverall accounts and add you Coveralls token to your repository as a GitHub Secret (see below).
 
 
 To run tests and coverage checks locally, you can use the following commands:
 ```sh
-pip install pytest coverage shapely geopandas
+pip install pytest coverage
 coverage run -m pytest ./
 coverage html
 ```
 
 ### GitHub Secrets
 
 There are three GitHub Secrets required to enable all of our GitHub Actions:
```

### Comparing `distancerasters-0.3.2/setup.cfg` & `distancerasters-0.3.3/setup.cfg`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [metadata]
 name = distancerasters
-version = 0.3.2
+version = 0.3.3
 description = Generate distance raster using arbitrary sets of spatial features
 long_description = file:README.md
 long_description_content_type = text/markdown
 author = Seth Goodman
 author_email = sgoodman@aiddata.wm.edu
 url = https://github.com/sgoodm/python-distance-rasters
 project_urls = 
@@ -21,14 +21,15 @@
 install_requires = 
 	numpy
 	rasterio
 	fiona
 	affine
 	scipy>=1.6.0
 	rasterstats
+	tqdm
 
 [options.packages.find]
 where = src
 
 [egg_info]
 tag_build = 
 tag_date = 0
```

### Comparing `distancerasters-0.3.2/src/distancerasters/main.py` & `distancerasters-0.3.3/src/distancerasters/main.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,17 +1,22 @@
 import time
+from itertools import product
+
 import numpy as np
 from affine import Affine
 from scipy.spatial import KDTree
-from .utils import export_raster, convert_index_to_coords, calc_haversine_distance
+from tqdm import tqdm
+
+from .utils import (calc_haversine_distance, convert_index_to_coords,
+                    export_raster)
 
 
 class DistanceRaster(object):
 
-    def __init__(self, raster_array, affine=None, conditional=None, output_path=None):
+    def __init__(self, raster_array, affine=None, conditional=None, output_path=None, progress_bar=False):
         """build distance array from raster array
 
         Args
             raster_array (np array):
                 array to use for distance calculations
             affine (Affine): [optional]
                 affine transformation defining spatial raster data
@@ -42,14 +47,15 @@
             raise Exception("Conditional must be function")
 
 
         self.conditional = conditional
         self.raster_array = raster_array
         self.pixel_size = pixel_size
         self.affine = affine
+        self.progress_bar = progress_bar
 
         self.tree = None
         self.dist_array = None
 
         self._build_tree()
         self._calculate_distance()
 
@@ -73,41 +79,40 @@
     def _calculate_distance(self):
 
         nrows, ncols = self.raster_array.shape
         self.dist_array = np.empty(self.raster_array.shape, dtype=float)
 
         t_start = time.time()
 
-        for r in range(nrows):
+        row_col_iterable = product(range(nrows), range(ncols))
 
-            for c in range(ncols):
+        for r, c in tqdm(row_col_iterable, total=nrows*ncols, disable=(not self.progress_bar)):
+            cur_index = (r, c)
+            min_dist, min_index = self.tree.query([cur_index])
+            min_dist = min_dist[0]
+            min_index = self.tree.data[min_index[0]]
+
+            if self.affine is not None:
+                if cur_index[1] == min_index[1]:
+                    # columns are same meaning nearest is either vertical or self.
+                    # no correction needed, just convert to km
+                    dd_min_dist = min_dist * self.pixel_size
+                    km_min_dist = dd_min_dist * 111.321
 
-                cur_index = (r, c)
-                min_dist, min_index = self.tree.query([cur_index])
-                min_dist = min_dist[0]
-                min_index = self.tree.data[min_index[0]]
-
-                if self.affine is not None:
-                    if cur_index[1] == min_index[1]:
-                        # columns are same meaning nearest is either vertical or self.
-                        # no correction needed, just convert to km
-                        dd_min_dist = min_dist * self.pixel_size
-                        km_min_dist = dd_min_dist * 111.321
-
-                    else:
-                        km_min_dist = calc_haversine_distance(
-                            convert_index_to_coords(cur_index, self.affine),
-                            convert_index_to_coords(min_index, self.affine),
-                        )
+                else:
+                    km_min_dist = calc_haversine_distance(
+                        convert_index_to_coords(cur_index, self.affine),
+                        convert_index_to_coords(min_index, self.affine),
+                    )
 
-                    val = km_min_dist * 1000
+                val = km_min_dist * 1000
 
-                else:
-                    val = min_dist
+            else:
+                val = min_dist
 
-                self.dist_array[r][c] = val
+            self.dist_array[r][c] = val
 
         print("Distance calc run time: {0} seconds".format(round(time.time() - t_start, 4)))
 
 
     def output_raster(self, output_path):
         export_raster(self.dist_array, self.affine, output_path)
```

### Comparing `distancerasters-0.3.2/src/distancerasters/utils.py` & `distancerasters-0.3.3/src/distancerasters/utils.py`

 * *Files identical despite different names*

### Comparing `distancerasters-0.3.2/src/distancerasters.egg-info/PKG-INFO` & `distancerasters-0.3.3/src/distancerasters.egg-info/PKG-INFO`

 * *Files 9% similar despite different names*

```diff
@@ -1,20 +1,27 @@
 Metadata-Version: 2.1
 Name: distancerasters
-Version: 0.3.2
+Version: 0.3.3
 Summary: Generate distance raster using arbitrary sets of spatial features
 Home-page: https://github.com/sgoodm/python-distance-rasters
 Author: Seth Goodman
 Author-email: sgoodman@aiddata.wm.edu
 License: BSD 3-Clause License
 Project-URL: Bug Tracker, https://github.com/sgoodm/python-distance-rasters/issues
 Keywords: raster,distance,spatial
 Classifier: Programming Language :: Python :: 3
 Description-Content-Type: text/markdown
 License-File: LICENSE.txt
+Requires-Dist: numpy
+Requires-Dist: rasterio
+Requires-Dist: fiona
+Requires-Dist: affine
+Requires-Dist: scipy>=1.6.0
+Requires-Dist: rasterstats
+Requires-Dist: tqdm
 
 # distance-rasters
 
 Generate distance raster using arbitrary sets of spatial features
 
 [![build badge](https://github.com/sgoodm/python-distance-rasters/actions/workflows/test-with-coverage.yml/badge.svg)](https://github.com/sgoodm/python-distance-rasters/actions/workflows/test-and-coverage.yml)
 [![Coverage Status](https://coveralls.io/repos/github/sgoodm/python-distance-rasters/badge.svg)](https://coveralls.io/github/sgoodm/python-distance-rasters)
@@ -131,15 +138,15 @@
 We use Pytest and Coveralls to run unit tests and track code coverage of tests. If you submit code, please make sure it passes existing tests and adds relevant testing coverage for new features.
 
 You can run tests and coverage checks locally, or you can fork the repository and utilize GitHub actions and Coveralls. To use GitHub actions and Coveralls, you'll need to add your forked repo to your own Coverall accounts and add you Coveralls token to your repository as a GitHub Secret (see below).
 
 
 To run tests and coverage checks locally, you can use the following commands:
 ```sh
-pip install pytest coverage shapely geopandas
+pip install pytest coverage
 coverage run -m pytest ./
 coverage html
 ```
 
 ### GitHub Secrets
 
 There are three GitHub Secrets required to enable all of our GitHub Actions:
```

### Comparing `distancerasters-0.3.2/tests/test_main.py` & `distancerasters-0.3.3/tests/test_main.py`

 * *Files identical despite different names*

### Comparing `distancerasters-0.3.2/tests/test_utils.py` & `distancerasters-0.3.3/tests/test_utils.py`

 * *Files identical despite different names*

