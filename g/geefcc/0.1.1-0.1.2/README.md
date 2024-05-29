# Comparing `tmp/geefcc-0.1.1.tar.gz` & `tmp/geefcc-0.1.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "geefcc-0.1.1.tar", last modified: Mon May 27 02:24:05 2024, max compression
+gzip compressed data, was "geefcc-0.1.2.tar", last modified: Wed May 29 02:22:03 2024, max compression
```

## Comparing `geefcc-0.1.1.tar` & `geefcc-0.1.2.tar`

### file list

```diff
@@ -1,32 +1,36 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-27 02:24:05.443144 geefcc-0.1.1/
--rw-r--r--   0 runner    (1001) docker     (127)      177 2024-05-27 02:24:03.000000 geefcc-0.1.1/CHANGELOG.rst
--rw-r--r--   0 runner    (1001) docker     (127)    35149 2024-05-27 02:24:03.000000 geefcc-0.1.1/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)       56 2024-05-27 02:24:03.000000 geefcc-0.1.1/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (127)     8661 2024-05-27 02:24:05.443144 geefcc-0.1.1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     7489 2024-05-27 02:24:03.000000 geefcc-0.1.1/README.rst
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-27 02:24:05.443144 geefcc-0.1.1/geefcc/
--rw-r--r--   0 runner    (1001) docker     (127)      551 2024-05-27 02:24:03.000000 geefcc-0.1.1/geefcc/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      640 2024-05-27 02:24:03.000000 geefcc-0.1.1/geefcc/download_gadm.py
--rw-r--r--   0 runner    (1001) docker     (127)     1835 2024-05-27 02:24:03.000000 geefcc-0.1.1/geefcc/ee_gfc.py
--rw-r--r--   0 runner    (1001) docker     (127)     1531 2024-05-27 02:24:03.000000 geefcc-0.1.1/geefcc/ee_initialize.py
--rw-r--r--   0 runner    (1001) docker     (127)     2172 2024-05-27 02:24:03.000000 geefcc-0.1.1/geefcc/ee_tmf.py
--rw-r--r--   0 runner    (1001) docker     (127)      761 2024-05-27 02:24:03.000000 geefcc-0.1.1/geefcc/geefcc.py
--rw-r--r--   0 runner    (1001) docker     (127)     5845 2024-05-27 02:24:03.000000 geefcc-0.1.1/geefcc/geeic2geotiff.py
--rw-r--r--   0 runner    (1001) docker     (127)     1280 2024-05-27 02:24:03.000000 geefcc-0.1.1/geefcc/geotiff_from_tiles.py
--rw-r--r--   0 runner    (1001) docker     (127)     2571 2024-05-27 02:24:03.000000 geefcc-0.1.1/geefcc/get_extent_from_aoi.py
--rw-r--r--   0 runner    (1001) docker     (127)     3970 2024-05-27 02:24:03.000000 geefcc-0.1.1/geefcc/get_fcc.py
--rw-r--r--   0 runner    (1001) docker     (127)      684 2024-05-27 02:24:03.000000 geefcc-0.1.1/geefcc/get_vector_extent.py
--rw-r--r--   0 runner    (1001) docker     (127)     5701 2024-05-27 02:24:03.000000 geefcc-0.1.1/geefcc/make_grid.py
--rw-r--r--   0 runner    (1001) docker     (127)     2399 2024-05-27 02:24:03.000000 geefcc-0.1.1/geefcc/sum_raster_bands.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-27 02:24:05.443144 geefcc-0.1.1/geefcc.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     8661 2024-05-27 02:24:05.000000 geefcc-0.1.1/geefcc.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      589 2024-05-27 02:24:05.000000 geefcc-0.1.1/geefcc.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-27 02:24:05.000000 geefcc-0.1.1/geefcc.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       46 2024-05-27 02:24:05.000000 geefcc-0.1.1/geefcc.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-27 02:24:05.000000 geefcc-0.1.1/geefcc.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (127)       72 2024-05-27 02:24:05.000000 geefcc-0.1.1/geefcc.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)        7 2024-05-27 02:24:05.000000 geefcc-0.1.1/geefcc.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)       67 2024-05-27 02:24:05.447144 geefcc-0.1.1/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)     2402 2024-05-27 02:24:03.000000 geefcc-0.1.1/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-27 02:24:05.443144 geefcc-0.1.1/test/
--rw-r--r--   0 runner    (1001) docker     (127)     1358 2024-05-27 02:24:03.000000 geefcc-0.1.1/test/test_get_fcc.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-29 02:22:03.205837 geefcc-0.1.2/
+-rw-r--r--   0 runner    (1001) docker     (127)      235 2024-05-29 02:22:00.000000 geefcc-0.1.2/CHANGELOG.rst
+-rw-r--r--   0 runner    (1001) docker     (127)    35149 2024-05-29 02:22:00.000000 geefcc-0.1.2/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)       56 2024-05-29 02:22:00.000000 geefcc-0.1.2/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (127)     8667 2024-05-29 02:22:03.205837 geefcc-0.1.2/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     7491 2024-05-29 02:22:00.000000 geefcc-0.1.2/README.rst
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-29 02:22:03.201837 geefcc-0.1.2/geefcc/
+-rw-r--r--   0 runner    (1001) docker     (127)      578 2024-05-29 02:22:00.000000 geefcc-0.1.2/geefcc/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      637 2024-05-29 02:22:00.000000 geefcc-0.1.2/geefcc/download_gadm.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1835 2024-05-29 02:22:00.000000 geefcc-0.1.2/geefcc/ee_gfc.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1531 2024-05-29 02:22:00.000000 geefcc-0.1.2/geefcc/ee_initialize.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2172 2024-05-29 02:22:00.000000 geefcc-0.1.2/geefcc/ee_tmf.py
+-rw-r--r--   0 runner    (1001) docker     (127)      761 2024-05-29 02:22:00.000000 geefcc-0.1.2/geefcc/geefcc.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5845 2024-05-29 02:22:00.000000 geefcc-0.1.2/geefcc/geeic2geotiff.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1280 2024-05-29 02:22:00.000000 geefcc-0.1.2/geefcc/geotiff_from_tiles.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2571 2024-05-29 02:22:00.000000 geefcc-0.1.2/geefcc/get_extent_from_aoi.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4068 2024-05-29 02:22:00.000000 geefcc-0.1.2/geefcc/get_fcc.py
+-rw-r--r--   0 runner    (1001) docker     (127)      684 2024-05-29 02:22:00.000000 geefcc-0.1.2/geefcc/get_vector_extent.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5701 2024-05-29 02:22:00.000000 geefcc-0.1.2/geefcc/make_grid.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-29 02:22:03.201837 geefcc-0.1.2/geefcc/misc/
+-rw-r--r--   0 runner    (1001) docker     (127)      110 2024-05-29 02:22:00.000000 geefcc-0.1.2/geefcc/misc/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3111 2024-05-29 02:22:00.000000 geefcc-0.1.2/geefcc/misc/miscellaneous.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2399 2024-05-29 02:22:00.000000 geefcc-0.1.2/geefcc/sum_raster_bands.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-29 02:22:03.201837 geefcc-0.1.2/geefcc.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     8667 2024-05-29 02:22:03.000000 geefcc-0.1.2/geefcc.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      662 2024-05-29 02:22:03.000000 geefcc-0.1.2/geefcc.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-29 02:22:03.000000 geefcc-0.1.2/geefcc.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       46 2024-05-29 02:22:03.000000 geefcc-0.1.2/geefcc.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-29 02:22:03.000000 geefcc-0.1.2/geefcc.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (127)       76 2024-05-29 02:22:03.000000 geefcc-0.1.2/geefcc.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       19 2024-05-29 02:22:03.000000 geefcc-0.1.2/geefcc.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       67 2024-05-29 02:22:03.205837 geefcc-0.1.2/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)     2444 2024-05-29 02:22:00.000000 geefcc-0.1.2/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-29 02:22:03.201837 geefcc-0.1.2/test/
+-rw-r--r--   0 runner    (1001) docker     (127)     1345 2024-05-29 02:22:00.000000 geefcc-0.1.2/test/test_get_fcc.py
+-rw-r--r--   0 runner    (1001) docker     (127)      596 2024-05-29 02:22:00.000000 geefcc-0.1.2/test/test_import.py
```

### Comparing `geefcc-0.1.1/LICENSE` & `geefcc-0.1.2/LICENSE`

 * *Files identical despite different names*

### Comparing `geefcc-0.1.1/PKG-INFO` & `geefcc-0.1.2/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: geefcc
-Version: 0.1.1
+Version: 0.1.2
 Summary: Forest cover change from Google Earth Engine
 Home-page: https://ecology.ghislainv.fr/geefcc
 Author: Ghislain Vieilledent
 Author-email: ghislain.vieilledent@cirad.fr
 License: GPLv3
 Project-URL: Documentation, https://ecology.ghislainv.fr/geefcc
 Project-URL: Source, https://github.com/ghislainv/geefcc/
@@ -19,18 +19,18 @@
 Description-Content-Type: text/x-rst
 License-File: LICENSE
 Requires-Dist: numpy
 Requires-Dist: gdal
 Requires-Dist: xarray
 Requires-Dist: xee
 Provides-Extra: interactive
-Requires-Dist: jupyter; extra == "interactive"
+Requires-Dist: cartopy; extra == "interactive"
+Requires-Dist: rioxarray; extra == "interactive"
+Requires-Dist: matplotlib; extra == "interactive"
 Requires-Dist: geopandas; extra == "interactive"
-Requires-Dist: descartes; extra == "interactive"
-Requires-Dist: folium; extra == "interactive"
 
 ..
    # ==============================================================================
    # author          :Ghislain Vieilledent
    # email           :ghislain.vieilledent@cirad.fr
    # web             :https://ecology.ghislainv.fr
    # license         :GPLv3
@@ -104,15 +104,15 @@
 The ``geefcc`` package downloads country administrative borders from the `GADM <https://gadm.org/data.html>`_ website. From time to time, their server is not responding. In case of problem with downloading country borders, check directly on the GADM website that data can be downloaded manually to be sure that the problem is coming from ``geefcc``.
 
 Installation
 ============
 
 The easiest way to install the ``geefcc`` Python package is via `pip <https://pip.pypa.io/en/stable/>`_ in the *OSGeo4W Shell* for Windows or in a virtual environment for Linux.
 
-For Linux, create and activate a virtual environment before install ``geefcc`` with ``pip``:
+For Linux, create and activate a virtual environment before installing ``geefcc`` with ``pip``:
 
 .. code-block:: shell
 
    cd ~
    # Create a directory for virtual environments
    mkdir venvs
    # Create the virtual environment with venv
@@ -146,15 +146,15 @@
    deactivate
    rm -R ~/venvs/venv-geefcc # Just remove the repository
 
 In case of problem while installing GDAL Python bindings, try the following command:
 
 .. code-block:: shell
 		
-   python3 -m pip install  --no-cache-dir --force-reinstall gdal==$(gdal-config --version)
+   python3 -m pip install --no-cache-dir --force-reinstall gdal==$(gdal-config --version)
    
 Contributing
 ============
 
 The ``geefcc`` Python package is Open Source and released under
 the `GNU GPL version 3 license
 <https://ecology.ghislainv.fr/geefcc/license.html>`__. Anybody
```

### Comparing `geefcc-0.1.1/README.rst` & `geefcc-0.1.2/README.rst`

 * *Files 0% similar despite different names*

```diff
@@ -74,15 +74,15 @@
 The ``geefcc`` package downloads country administrative borders from the `GADM <https://gadm.org/data.html>`_ website. From time to time, their server is not responding. In case of problem with downloading country borders, check directly on the GADM website that data can be downloaded manually to be sure that the problem is coming from ``geefcc``.
 
 Installation
 ============
 
 The easiest way to install the ``geefcc`` Python package is via `pip <https://pip.pypa.io/en/stable/>`_ in the *OSGeo4W Shell* for Windows or in a virtual environment for Linux.
 
-For Linux, create and activate a virtual environment before install ``geefcc`` with ``pip``:
+For Linux, create and activate a virtual environment before installing ``geefcc`` with ``pip``:
 
 .. code-block:: shell
 
    cd ~
    # Create a directory for virtual environments
    mkdir venvs
    # Create the virtual environment with venv
@@ -116,15 +116,15 @@
    deactivate
    rm -R ~/venvs/venv-geefcc # Just remove the repository
 
 In case of problem while installing GDAL Python bindings, try the following command:
 
 .. code-block:: shell
 		
-   python3 -m pip install  --no-cache-dir --force-reinstall gdal==$(gdal-config --version)
+   python3 -m pip install --no-cache-dir --force-reinstall gdal==$(gdal-config --version)
    
 Contributing
 ============
 
 The ``geefcc`` Python package is Open Source and released under
 the `GNU GPL version 3 license
 <https://ecology.ghislainv.fr/geefcc/license.html>`__. Anybody
```

### Comparing `geefcc-0.1.1/geefcc/__init__.py` & `geefcc-0.1.2/geefcc/__init__.py`

 * *Files 4% similar despite different names*

```diff
@@ -3,20 +3,21 @@
 https://ecology.ghislainv.fr/geefcc/
 """
 
 # Define double undescore variables
 # https://peps.python.org/pep-0008/#module-level-dunder-names
 __author__ = "Ghislain Vieilledent and Thomas Arsouze"
 __email__ = "ghislain.vieilledent@cirad.fr, thomas.arsouze@cirad.fr"
-__version__ = "0.1.1"
+__version__ = "0.1.2"
 
 # GDAL exceptions
 from osgeo import gdal
 
 from .ee_initialize import ee_initialize
 from .get_fcc import get_fcc
 from .sum_raster_bands import sum_raster_bands
+from .misc import make_dir
 
 # GDAL exceptions
 gdal.UseExceptions()
 
 # End
```

### Comparing `geefcc-0.1.1/geefcc/download_gadm.py` & `geefcc-0.1.2/geefcc/download_gadm.py`

 * *Files 18% similar despite different names*

```diff
@@ -15,14 +15,14 @@
     :param output_file: Path to output GPKG file.
 
     """
 
     # Check for existing file
     if not os.path.isfile(output_file):
 
-        # Download the zipfile from gadm.org
+        # Download the file from gadm.org
         url = ("https://geodata.ucdavis.edu/gadm/gadm4.1/"
                f"gpkg/gadm41_{iso3}.gpkg")
         urlretrieve(url, output_file)
 
 
 # End
```

### Comparing `geefcc-0.1.1/geefcc/ee_gfc.py` & `geefcc-0.1.2/geefcc/ee_gfc.py`

 * *Files identical despite different names*

### Comparing `geefcc-0.1.1/geefcc/ee_initialize.py` & `geefcc-0.1.2/geefcc/ee_initialize.py`

 * *Files identical despite different names*

### Comparing `geefcc-0.1.1/geefcc/ee_tmf.py` & `geefcc-0.1.2/geefcc/ee_tmf.py`

 * *Files identical despite different names*

### Comparing `geefcc-0.1.1/geefcc/geefcc.py` & `geefcc-0.1.2/geefcc/geefcc.py`

 * *Files identical despite different names*

### Comparing `geefcc-0.1.1/geefcc/geeic2geotiff.py` & `geefcc-0.1.2/geefcc/geeic2geotiff.py`

 * *Files identical despite different names*

### Comparing `geefcc-0.1.1/geefcc/geotiff_from_tiles.py` & `geefcc-0.1.2/geefcc/geotiff_from_tiles.py`

 * *Files identical despite different names*

### Comparing `geefcc-0.1.1/geefcc/get_extent_from_aoi.py` & `geefcc-0.1.2/geefcc/get_extent_from_aoi.py`

 * *Files identical despite different names*

### Comparing `geefcc-0.1.1/geefcc/get_fcc.py` & `geefcc-0.1.2/geefcc/get_fcc.py`

 * *Files 5% similar despite different names*

```diff
@@ -47,21 +47,24 @@
         defining the forest must be specified with parameter ``perc``.
 
     :param perc: Tree cover threshold defining the forest for GFC
         product.
 
     :param tile_size: Tile size for parallel computing.
 
-    :param ncpu: Number of CPU to use for parallel computing.
+    :param ncpu: Number of CPU to use for parallel computing. If None,
+        it will be set to the number of cores on the computer minus
+        one.
 
     :param crop_to_aoi: Crop the raster GeoTIFF file to aoi. If False,
-        the output file will match the grid covering the aoi with buffer.
+        the output file will match the grid covering the aoi with
+        buffer.
 
-    :param output_file: Path to output GeoTIFF file. If directories in path
-        do not exist they will be created.
+    :param output_file: Path to output GeoTIFF file. If directories in
+        path do not exist they will be created.
 
     """
 
     # Output dir
     out_dir = opd(output_file)
     make_dir(out_dir)
```

### Comparing `geefcc-0.1.1/geefcc/get_vector_extent.py` & `geefcc-0.1.2/geefcc/get_vector_extent.py`

 * *Files identical despite different names*

### Comparing `geefcc-0.1.1/geefcc/make_grid.py` & `geefcc-0.1.2/geefcc/make_grid.py`

 * *Files identical despite different names*

### Comparing `geefcc-0.1.1/geefcc/sum_raster_bands.py` & `geefcc-0.1.2/geefcc/sum_raster_bands.py`

 * *Files identical despite different names*

### Comparing `geefcc-0.1.1/geefcc.egg-info/PKG-INFO` & `geefcc-0.1.2/geefcc.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: geefcc
-Version: 0.1.1
+Version: 0.1.2
 Summary: Forest cover change from Google Earth Engine
 Home-page: https://ecology.ghislainv.fr/geefcc
 Author: Ghislain Vieilledent
 Author-email: ghislain.vieilledent@cirad.fr
 License: GPLv3
 Project-URL: Documentation, https://ecology.ghislainv.fr/geefcc
 Project-URL: Source, https://github.com/ghislainv/geefcc/
@@ -19,18 +19,18 @@
 Description-Content-Type: text/x-rst
 License-File: LICENSE
 Requires-Dist: numpy
 Requires-Dist: gdal
 Requires-Dist: xarray
 Requires-Dist: xee
 Provides-Extra: interactive
-Requires-Dist: jupyter; extra == "interactive"
+Requires-Dist: cartopy; extra == "interactive"
+Requires-Dist: rioxarray; extra == "interactive"
+Requires-Dist: matplotlib; extra == "interactive"
 Requires-Dist: geopandas; extra == "interactive"
-Requires-Dist: descartes; extra == "interactive"
-Requires-Dist: folium; extra == "interactive"
 
 ..
    # ==============================================================================
    # author          :Ghislain Vieilledent
    # email           :ghislain.vieilledent@cirad.fr
    # web             :https://ecology.ghislainv.fr
    # license         :GPLv3
@@ -104,15 +104,15 @@
 The ``geefcc`` package downloads country administrative borders from the `GADM <https://gadm.org/data.html>`_ website. From time to time, their server is not responding. In case of problem with downloading country borders, check directly on the GADM website that data can be downloaded manually to be sure that the problem is coming from ``geefcc``.
 
 Installation
 ============
 
 The easiest way to install the ``geefcc`` Python package is via `pip <https://pip.pypa.io/en/stable/>`_ in the *OSGeo4W Shell* for Windows or in a virtual environment for Linux.
 
-For Linux, create and activate a virtual environment before install ``geefcc`` with ``pip``:
+For Linux, create and activate a virtual environment before installing ``geefcc`` with ``pip``:
 
 .. code-block:: shell
 
    cd ~
    # Create a directory for virtual environments
    mkdir venvs
    # Create the virtual environment with venv
@@ -146,15 +146,15 @@
    deactivate
    rm -R ~/venvs/venv-geefcc # Just remove the repository
 
 In case of problem while installing GDAL Python bindings, try the following command:
 
 .. code-block:: shell
 		
-   python3 -m pip install  --no-cache-dir --force-reinstall gdal==$(gdal-config --version)
+   python3 -m pip install --no-cache-dir --force-reinstall gdal==$(gdal-config --version)
    
 Contributing
 ============
 
 The ``geefcc`` Python package is Open Source and released under
 the `GNU GPL version 3 license
 <https://ecology.ghislainv.fr/geefcc/license.html>`__. Anybody
```

### Comparing `geefcc-0.1.1/geefcc.egg-info/SOURCES.txt` & `geefcc-0.1.2/geefcc.egg-info/SOURCES.txt`

 * *Files 19% similar despite different names*

```diff
@@ -20,8 +20,11 @@
 geefcc.egg-info/PKG-INFO
 geefcc.egg-info/SOURCES.txt
 geefcc.egg-info/dependency_links.txt
 geefcc.egg-info/entry_points.txt
 geefcc.egg-info/not-zip-safe
 geefcc.egg-info/requires.txt
 geefcc.egg-info/top_level.txt
-test/test_get_fcc.py
+geefcc/misc/__init__.py
+geefcc/misc/miscellaneous.py
+test/test_get_fcc.py
+test/test_import.py
```

### Comparing `geefcc-0.1.1/setup.py` & `geefcc-0.1.2/setup.py`

 * *Files 8% similar despite different names*

```diff
@@ -56,17 +56,17 @@
                    "(GPLv3)",
                    "Programming Language :: Python :: 3",
                    "Operating System :: OS Independent",
                    "Topic :: Scientific/Engineering :: Bio-Informatics"],
       keywords=("deforestation tropical forests forest "
                 "cover change map google earth engine"),
       python_requires=">=3.6",
-      packages=["geefcc"],
-      package_dir={"geefcc": "geefcc"},
+      packages=["geefcc", "geefcc/misc"],
+      package_dir={"geefcc": "geefcc", "misc": "geefcc/misc"},
       entry_points={"console_scripts": ["geefcc = geefcc.geefcc:main"]},
       install_requires=["numpy", "gdal", "xarray", "xee"],
       extras_require={
-          "interactive": ["jupyter", "geopandas",
-                          "descartes", "folium"]},
+          "interactive": ["cartopy", "rioxarray",
+                          "matplotlib", "geopandas"]},
       zip_safe=False)
 
 # End
```

### Comparing `geefcc-0.1.1/test/test_get_fcc.py` & `geefcc-0.1.2/test/test_get_fcc.py`

 * *Files 17% similar despite different names*

```diff
@@ -1,45 +1,45 @@
 """Test for gee_fcc()."""
 
 # Import
 import os
 
-from geefcc import get_fcc, ee_initialize
+import geefcc as gf
 
 # "EARTHENGINE_TOKEN" for GitHub actions
 # https://github.com/gee-community/geemap/discussions/1341
 # Find the Earth Engine credentials file on your computer.
 # Open the credentials file and copy its content.
 # On the GitHub Actions page, create a new secret
 # with the name EARTHENGINE_TOKEN.
 
 # Initialize GEE
-ee_initialize(
+gf.ee_initialize(
     token_name="EARTHENGINE_TOKEN",
     project="forestatrisk",
     opt_url="https://earthengine-highvolume.googleapis.com")
 
 
 def test_get_fcc_extent_tmf():
     """Testing get_fcc()."""
-    get_fcc(
+    gf.get_fcc(
         # Extent for Reunion Island
         aoi=(55.21625137, -21.38986015, 55.83736038, -20.87180519),
         buff=0.08983152841195216,
         years=[2000, 2010, 2020],
         source="tmf",
         tile_size=0.5,
         output_file="out_tmf/fcc_tmf.tif",
     )
     assert os.path.isfile("out_tmf/fcc_tmf.tif")
 
 
 def test_get_fcc_extent_gfc():
     """Testing get_fcc()."""
-    get_fcc(
+    gf.get_fcc(
         # Extent for Reunion Island
         aoi=(55.21625137, -21.38986015, 55.83736038, -20.87180519),
         buff=0.08983152841195216,
         years=[2001, 2010, 2020],
         source="gfc",
         perc=50,
         tile_size=0.5,
```

