# Comparing `tmp/brainglobe-segmentation-1.2.3.tar.gz` & `tmp/brainglobe_segmentation-1.2.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "brainglobe-segmentation-1.2.3.tar", last modified: Tue Feb 27 10:55:40 2024, max compression
+gzip compressed data, was "brainglobe_segmentation-1.2.4.tar", last modified: Wed May 29 09:46:04 2024, max compression
```

## Comparing `brainglobe-segmentation-1.2.3.tar` & `brainglobe_segmentation-1.2.4.tar`

### file list

```diff
@@ -1,50 +1,50 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-27 10:55:40.665542 brainglobe-segmentation-1.2.3/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-27 10:55:40.653542 brainglobe-segmentation-1.2.3/.github/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-27 10:55:40.657542 brainglobe-segmentation-1.2.3/.github/workflows/
--rw-r--r--   0 runner    (1001) docker     (127)     1780 2024-02-27 10:55:30.000000 brainglobe-segmentation-1.2.3/.github/workflows/test_and_deploy.yml
--rw-r--r--   0 runner    (1001) docker     (127)      978 2024-02-27 10:55:30.000000 brainglobe-segmentation-1.2.3/.gitignore
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-27 10:55:40.657542 brainglobe-segmentation-1.2.3/.napari/
--rw-r--r--   0 runner    (1001) docker     (127)      172 2024-02-27 10:55:30.000000 brainglobe-segmentation-1.2.3/.napari/config.yml
--rw-r--r--   0 runner    (1001) docker     (127)     1840 2024-02-27 10:55:30.000000 brainglobe-segmentation-1.2.3/CITATION.cff
--rw-r--r--   0 runner    (1001) docker     (127)     1518 2024-02-27 10:55:30.000000 brainglobe-segmentation-1.2.3/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)      180 2024-02-27 10:55:30.000000 brainglobe-segmentation-1.2.3/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (127)     4025 2024-02-27 10:55:40.665542 brainglobe-segmentation-1.2.3/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     2271 2024-02-27 10:55:30.000000 brainglobe-segmentation-1.2.3/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-27 10:55:40.657542 brainglobe-segmentation-1.2.3/brainglobe_segmentation/
--rw-r--r--   0 runner    (1001) docker     (127)      232 2024-02-27 10:55:30.000000 brainglobe-segmentation-1.2.3/brainglobe_segmentation/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-27 10:55:40.661542 brainglobe-segmentation-1.2.3/brainglobe_segmentation/atlas/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-02-27 10:55:30.000000 brainglobe-segmentation-1.2.3/brainglobe_segmentation/atlas/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2800 2024-02-27 10:55:30.000000 brainglobe-segmentation-1.2.3/brainglobe_segmentation/atlas/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-27 10:55:40.661542 brainglobe-segmentation-1.2.3/brainglobe_segmentation/image/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-02-27 10:55:30.000000 brainglobe-segmentation-1.2.3/brainglobe_segmentation/image/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      387 2024-02-27 10:55:30.000000 brainglobe-segmentation-1.2.3/brainglobe_segmentation/image/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-27 10:55:40.661542 brainglobe-segmentation-1.2.3/brainglobe_segmentation/layout/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-02-27 10:55:30.000000 brainglobe-segmentation-1.2.3/brainglobe_segmentation/layout/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      768 2024-02-27 10:55:30.000000 brainglobe-segmentation-1.2.3/brainglobe_segmentation/layout/gui_constants.py
--rw-r--r--   0 runner    (1001) docker     (127)      346 2024-02-27 10:55:30.000000 brainglobe-segmentation-1.2.3/brainglobe_segmentation/napari.yaml
--rw-r--r--   0 runner    (1001) docker     (127)      769 2024-02-27 10:55:30.000000 brainglobe-segmentation-1.2.3/brainglobe_segmentation/paths.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-27 10:55:40.661542 brainglobe-segmentation-1.2.3/brainglobe_segmentation/regions/
--rw-r--r--   0 runner    (1001) docker     (127)     3262 2024-02-27 10:55:30.000000 brainglobe-segmentation-1.2.3/brainglobe_segmentation/regions/IO.py
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-02-27 10:55:30.000000 brainglobe-segmentation-1.2.3/brainglobe_segmentation/regions/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     7481 2024-02-27 10:55:30.000000 brainglobe-segmentation-1.2.3/brainglobe_segmentation/regions/analysis.py
--rw-r--r--   0 runner    (1001) docker     (127)     2811 2024-02-27 10:55:30.000000 brainglobe-segmentation-1.2.3/brainglobe_segmentation/regions/layers.py
--rw-r--r--   0 runner    (1001) docker     (127)    18588 2024-02-27 10:55:30.000000 brainglobe-segmentation-1.2.3/brainglobe_segmentation/segment.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-27 10:55:40.661542 brainglobe-segmentation-1.2.3/brainglobe_segmentation/segmentation_panels/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-02-27 10:55:30.000000 brainglobe-segmentation-1.2.3/brainglobe_segmentation/segmentation_panels/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     9223 2024-02-27 10:55:30.000000 brainglobe-segmentation-1.2.3/brainglobe_segmentation/segmentation_panels/regions.py
--rw-r--r--   0 runner    (1001) docker     (127)    11574 2024-02-27 10:55:30.000000 brainglobe-segmentation-1.2.3/brainglobe_segmentation/segmentation_panels/tracks.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-27 10:55:40.661542 brainglobe-segmentation-1.2.3/brainglobe_segmentation/tracks/
--rw-r--r--   0 runner    (1001) docker     (127)     1306 2024-02-27 10:55:30.000000 brainglobe-segmentation-1.2.3/brainglobe_segmentation/tracks/IO.py
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-02-27 10:55:30.000000 brainglobe-segmentation-1.2.3/brainglobe_segmentation/tracks/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     6064 2024-02-27 10:55:30.000000 brainglobe-segmentation-1.2.3/brainglobe_segmentation/tracks/analysis.py
--rw-r--r--   0 runner    (1001) docker     (127)      977 2024-02-27 10:55:30.000000 brainglobe-segmentation-1.2.3/brainglobe_segmentation/tracks/fit.py
--rw-r--r--   0 runner    (1001) docker     (127)     1023 2024-02-27 10:55:30.000000 brainglobe-segmentation-1.2.3/brainglobe_segmentation/tracks/layers.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-27 10:55:40.661542 brainglobe-segmentation-1.2.3/brainglobe_segmentation.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     4025 2024-02-27 10:55:40.000000 brainglobe-segmentation-1.2.3/brainglobe_segmentation.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     1337 2024-02-27 10:55:40.000000 brainglobe-segmentation-1.2.3/brainglobe_segmentation.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-02-27 10:55:40.000000 brainglobe-segmentation-1.2.3/brainglobe_segmentation.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)      231 2024-02-27 10:55:40.000000 brainglobe-segmentation-1.2.3/brainglobe_segmentation.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (127)      235 2024-02-27 10:55:40.000000 brainglobe-segmentation-1.2.3/brainglobe_segmentation.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       24 2024-02-27 10:55:40.000000 brainglobe-segmentation-1.2.3/brainglobe_segmentation.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)     2959 2024-02-27 10:55:30.000000 brainglobe-segmentation-1.2.3/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-02-27 10:55:40.665542 brainglobe-segmentation-1.2.3/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-29 09:46:04.876744 brainglobe_segmentation-1.2.4/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-29 09:46:04.868744 brainglobe_segmentation-1.2.4/.github/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-29 09:46:04.872744 brainglobe_segmentation-1.2.4/.github/workflows/
+-rw-r--r--   0 runner    (1001) docker     (127)     2033 2024-05-29 09:45:56.000000 brainglobe_segmentation-1.2.4/.github/workflows/test_and_deploy.yml
+-rw-r--r--   0 runner    (1001) docker     (127)      978 2024-05-29 09:45:56.000000 brainglobe_segmentation-1.2.4/.gitignore
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-29 09:46:04.872744 brainglobe_segmentation-1.2.4/.napari/
+-rw-r--r--   0 runner    (1001) docker     (127)      172 2024-05-29 09:45:56.000000 brainglobe_segmentation-1.2.4/.napari/config.yml
+-rw-r--r--   0 runner    (1001) docker     (127)     1840 2024-05-29 09:45:56.000000 brainglobe_segmentation-1.2.4/CITATION.cff
+-rw-r--r--   0 runner    (1001) docker     (127)     1518 2024-05-29 09:45:56.000000 brainglobe_segmentation-1.2.4/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)      180 2024-05-29 09:45:56.000000 brainglobe_segmentation-1.2.4/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (127)     4025 2024-05-29 09:46:04.876744 brainglobe_segmentation-1.2.4/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     2271 2024-05-29 09:45:56.000000 brainglobe_segmentation-1.2.4/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-29 09:46:04.872744 brainglobe_segmentation-1.2.4/brainglobe_segmentation/
+-rw-r--r--   0 runner    (1001) docker     (127)      232 2024-05-29 09:45:56.000000 brainglobe_segmentation-1.2.4/brainglobe_segmentation/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-29 09:46:04.872744 brainglobe_segmentation-1.2.4/brainglobe_segmentation/atlas/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-29 09:45:56.000000 brainglobe_segmentation-1.2.4/brainglobe_segmentation/atlas/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2800 2024-05-29 09:45:56.000000 brainglobe_segmentation-1.2.4/brainglobe_segmentation/atlas/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-29 09:46:04.872744 brainglobe_segmentation-1.2.4/brainglobe_segmentation/image/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-29 09:45:56.000000 brainglobe_segmentation-1.2.4/brainglobe_segmentation/image/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      387 2024-05-29 09:45:56.000000 brainglobe_segmentation-1.2.4/brainglobe_segmentation/image/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-29 09:46:04.872744 brainglobe_segmentation-1.2.4/brainglobe_segmentation/layout/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-29 09:45:56.000000 brainglobe_segmentation-1.2.4/brainglobe_segmentation/layout/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      768 2024-05-29 09:45:56.000000 brainglobe_segmentation-1.2.4/brainglobe_segmentation/layout/gui_constants.py
+-rw-r--r--   0 runner    (1001) docker     (127)      346 2024-05-29 09:45:56.000000 brainglobe_segmentation-1.2.4/brainglobe_segmentation/napari.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)      769 2024-05-29 09:45:56.000000 brainglobe_segmentation-1.2.4/brainglobe_segmentation/paths.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-29 09:46:04.876744 brainglobe_segmentation-1.2.4/brainglobe_segmentation/regions/
+-rw-r--r--   0 runner    (1001) docker     (127)     3267 2024-05-29 09:45:56.000000 brainglobe_segmentation-1.2.4/brainglobe_segmentation/regions/IO.py
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-29 09:45:56.000000 brainglobe_segmentation-1.2.4/brainglobe_segmentation/regions/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7481 2024-05-29 09:45:56.000000 brainglobe_segmentation-1.2.4/brainglobe_segmentation/regions/analysis.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2811 2024-05-29 09:45:56.000000 brainglobe_segmentation-1.2.4/brainglobe_segmentation/regions/layers.py
+-rw-r--r--   0 runner    (1001) docker     (127)    19434 2024-05-29 09:45:56.000000 brainglobe_segmentation-1.2.4/brainglobe_segmentation/segment.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-29 09:46:04.876744 brainglobe_segmentation-1.2.4/brainglobe_segmentation/segmentation_panels/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-29 09:45:56.000000 brainglobe_segmentation-1.2.4/brainglobe_segmentation/segmentation_panels/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9223 2024-05-29 09:45:56.000000 brainglobe_segmentation-1.2.4/brainglobe_segmentation/segmentation_panels/regions.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11574 2024-05-29 09:45:56.000000 brainglobe_segmentation-1.2.4/brainglobe_segmentation/segmentation_panels/tracks.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-29 09:46:04.876744 brainglobe_segmentation-1.2.4/brainglobe_segmentation/tracks/
+-rw-r--r--   0 runner    (1001) docker     (127)     1306 2024-05-29 09:45:56.000000 brainglobe_segmentation-1.2.4/brainglobe_segmentation/tracks/IO.py
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-29 09:45:56.000000 brainglobe_segmentation-1.2.4/brainglobe_segmentation/tracks/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6064 2024-05-29 09:45:56.000000 brainglobe_segmentation-1.2.4/brainglobe_segmentation/tracks/analysis.py
+-rw-r--r--   0 runner    (1001) docker     (127)      977 2024-05-29 09:45:56.000000 brainglobe_segmentation-1.2.4/brainglobe_segmentation/tracks/fit.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1023 2024-05-29 09:45:56.000000 brainglobe_segmentation-1.2.4/brainglobe_segmentation/tracks/layers.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-29 09:46:04.876744 brainglobe_segmentation-1.2.4/brainglobe_segmentation.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     4025 2024-05-29 09:46:04.000000 brainglobe_segmentation-1.2.4/brainglobe_segmentation.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     1337 2024-05-29 09:46:04.000000 brainglobe_segmentation-1.2.4/brainglobe_segmentation.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-29 09:46:04.000000 brainglobe_segmentation-1.2.4/brainglobe_segmentation.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      231 2024-05-29 09:46:04.000000 brainglobe_segmentation-1.2.4/brainglobe_segmentation.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      235 2024-05-29 09:46:04.000000 brainglobe_segmentation-1.2.4/brainglobe_segmentation.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       24 2024-05-29 09:46:04.000000 brainglobe_segmentation-1.2.4/brainglobe_segmentation.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)     2959 2024-05-29 09:45:56.000000 brainglobe_segmentation-1.2.4/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-29 09:46:04.876744 brainglobe_segmentation-1.2.4/setup.cfg
```

### Comparing `brainglobe-segmentation-1.2.3/.github/workflows/test_and_deploy.yml` & `brainglobe_segmentation-1.2.4/.github/workflows/test_and_deploy.yml`

 * *Files 8% similar despite different names*

```diff
@@ -28,33 +28,39 @@
     strategy:
       fail-fast: false
       matrix:
         # Run across a mixture of Python versions and operating systems
         include:
         - os: ubuntu-latest
           python-version: "3.11"
-        - os: macos-latest
+        - os: macos-13 # Intel Mac
+          python-version: "3.10"
+        - os: macos-latest # ARM Mac
           python-version: "3.10"
         - os: windows-latest
           python-version: "3.9"
 
     steps:
       - name: Cache atlases
         uses: actions/cache@v3
         with:
           path: ~/.brainglobe
           key: bg-atlases
+      - name: install HDF5 libs on ARM Mac
+        if: matrix.os == 'macos-latest'
+        run: brew install hdf5
       # Setup pyqt libraries
       - uses: tlambert03/setup-qt-libs@v1
       # Helps set up VTK with a headless display
       - uses: pyvista/setup-headless-display-action@v2
       # Run tests
       - uses: neuroinformatics-unit/actions/test@v2
         with:
           python-version: ${{ matrix.python-version }}
+          secret-codecov-token: ${{ secrets.CODECOV_TOKEN }}
           use-xvfb: true
 
   build_sdist_wheels:
     name: Build source distribution
     needs: [test]
     if: github.event_name == 'push' && github.ref_type == 'tag'
     runs-on: ubuntu-latest
```

### Comparing `brainglobe-segmentation-1.2.3/.gitignore` & `brainglobe_segmentation-1.2.4/.gitignore`

 * *Files identical despite different names*

### Comparing `brainglobe-segmentation-1.2.3/CITATION.cff` & `brainglobe_segmentation-1.2.4/CITATION.cff`

 * *Files identical despite different names*

### Comparing `brainglobe-segmentation-1.2.3/LICENSE` & `brainglobe_segmentation-1.2.4/LICENSE`

 * *Files identical despite different names*

### Comparing `brainglobe-segmentation-1.2.3/PKG-INFO` & `brainglobe_segmentation-1.2.4/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: brainglobe-segmentation
-Version: 1.2.3
+Version: 1.2.4
 Summary: Segmentation of anatomical structures in a common coordinate space
 Author-email: "Adam Tyson, Horst Obenhaus" <code@adamltyson.com>
 License: BSD-3-Clause
 Project-URL: Homepage, https://brainglobe.info/
 Project-URL: Source Code, https://github.com/brainglobe/brainglobe-segmentation
 Project-URL: Bug Tracker, https://github.com/brainglobe/brainglobe-segmentation/issues
 Project-URL: Documentation, https://brainglobe.info/documentation/brainglobe-segmentation/index.html
@@ -19,15 +19,15 @@
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Requires-Python: >=3.9
 Description-Content-Type: text/markdown
 License-File: LICENSE
 Requires-Dist: brainglobe-atlasapi>=2.0.1
 Requires-Dist: brainglobe-napari-io>=0.3.0
-Requires-Dist: brainglobe-utils>=0.4.0
+Requires-Dist: brainglobe-utils>=0.5.0
 Requires-Dist: napari>=0.4.5
 Requires-Dist: numpy
 Requires-Dist: pandas[hdf5]
 Requires-Dist: qtpy
 Requires-Dist: scikit-image
 Requires-Dist: scipy
 Requires-Dist: tifffile
```

### Comparing `brainglobe-segmentation-1.2.3/README.md` & `brainglobe_segmentation-1.2.4/README.md`

 * *Files identical despite different names*

### Comparing `brainglobe-segmentation-1.2.3/brainglobe_segmentation/atlas/utils.py` & `brainglobe_segmentation-1.2.4/brainglobe_segmentation/atlas/utils.py`

 * *Files identical despite different names*

### Comparing `brainglobe-segmentation-1.2.3/brainglobe_segmentation/layout/gui_constants.py` & `brainglobe_segmentation-1.2.4/brainglobe_segmentation/layout/gui_constants.py`

 * *Files identical despite different names*

### Comparing `brainglobe-segmentation-1.2.3/brainglobe_segmentation/paths.py` & `brainglobe_segmentation-1.2.4/brainglobe_segmentation/paths.py`

 * *Files identical despite different names*

### Comparing `brainglobe-segmentation-1.2.3/brainglobe_segmentation/regions/IO.py` & `brainglobe_segmentation-1.2.4/brainglobe_segmentation/regions/IO.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from pathlib import Path
 
 import numpy as np
 from brainglobe_utils.general.pathlib import append_to_pathlib_stem
-from brainglobe_utils.image_io import to_tiff
+from brainglobe_utils.IO.image.save import to_tiff
 from brainglobe_utils.IO.surfaces import marching_cubes_to_obj
 from skimage import measure
 
 
 def convert_obj_to_br(verts, faces, voxel_size):
     if voxel_size != 1:
         verts = verts * voxel_size
```

### Comparing `brainglobe-segmentation-1.2.3/brainglobe_segmentation/regions/analysis.py` & `brainglobe_segmentation-1.2.4/brainglobe_segmentation/regions/analysis.py`

 * *Files identical despite different names*

### Comparing `brainglobe-segmentation-1.2.3/brainglobe_segmentation/regions/layers.py` & `brainglobe_segmentation-1.2.4/brainglobe_segmentation/regions/layers.py`

 * *Files identical despite different names*

### Comparing `brainglobe-segmentation-1.2.3/brainglobe_segmentation/segment.py` & `brainglobe_segmentation-1.2.4/brainglobe_segmentation/segment.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,14 +1,15 @@
 from pathlib import Path
 from typing import List, Optional
 
 import napari
 import numpy as np
 from brainglobe_utils.qtpy.dialog import display_warning
 from brainglobe_utils.qtpy.interaction import add_button
+from brainglobe_utils.qtpy.logo import header_widget
 from napari.qt.threading import thread_worker
 from qtpy import QtCore
 from qtpy.QtWidgets import QFileDialog, QGridLayout, QGroupBox, QLabel, QWidget
 
 from brainglobe_segmentation.atlas.utils import structure_from_viewer
 from brainglobe_segmentation.layout.gui_constants import (
     BOUNDARIES_STRING,
@@ -108,20 +109,21 @@
         Construct main layout of widget
         """
         self.layout = QGridLayout()
         self.layout.setContentsMargins(10, 10, 10, 10)
         self.layout.setAlignment(QtCore.Qt.AlignTop)
         self.layout.setSpacing(4)
 
-        # 3 Steps:
+        # 4 Steps:
+        # - header
         # - Loading panel
         # - Segmentation methods panel
         # -> Individual segmentation methods (which are invisible at first)
         # - Saving panel
-
+        self.add_header()
         self.add_loading_panel(1)
         self.add_segmentation_methods_panel(1)
         self.track_seg.add_track_panel(2)  # Track segmentation subpanel
         self.region_seg.add_region_panel(3)  # Region segmentation subpanel
         self.add_saving_panel(4)
 
         # Take care of status label
@@ -129,14 +131,30 @@
         self.status_label.setText("Ready")
         self.layout.addWidget(self.status_label, 5, 0)
 
         self.setLayout(self.layout)
 
     # PANELS ###############################################################
 
+    def add_header(self):
+        """
+        Header including brainglobe logo and documentation links.
+        """
+        # <br> is included in the package_name to make the label under the logo
+        # more compact, by splitting it onto two lines
+        header = header_widget(
+            package_name="brainglobe-<br>segmentation",
+            package_tagline="Segmentation of anatomical structures",
+            documentation_path="brainglobe-segmentation/user-guide/index.html",
+            github_repo_name="brainglobe-segmentation",
+            citation_doi="https://doi.org/10.1038/s41598-021-04676-9",
+            help_text="For help, hover the cursor over each parameter.",
+        )
+        self.layout.addWidget(header, 0, 0, 1, 2)
+
     def add_segmentation_methods_panel(self, row, column=1):
         """
         Segmentation methods chooser panel:
             Toggle visibility of segmentation
             methods
         """
         self.toggle_methods_panel = QGroupBox("Segmentation")
```

### Comparing `brainglobe-segmentation-1.2.3/brainglobe_segmentation/segmentation_panels/regions.py` & `brainglobe_segmentation-1.2.4/brainglobe_segmentation/segmentation_panels/regions.py`

 * *Files identical despite different names*

### Comparing `brainglobe-segmentation-1.2.3/brainglobe_segmentation/segmentation_panels/tracks.py` & `brainglobe_segmentation-1.2.4/brainglobe_segmentation/segmentation_panels/tracks.py`

 * *Files identical despite different names*

### Comparing `brainglobe-segmentation-1.2.3/brainglobe_segmentation/tracks/IO.py` & `brainglobe_segmentation-1.2.4/brainglobe_segmentation/tracks/IO.py`

 * *Files identical despite different names*

### Comparing `brainglobe-segmentation-1.2.3/brainglobe_segmentation/tracks/analysis.py` & `brainglobe_segmentation-1.2.4/brainglobe_segmentation/tracks/analysis.py`

 * *Files identical despite different names*

### Comparing `brainglobe-segmentation-1.2.3/brainglobe_segmentation/tracks/fit.py` & `brainglobe_segmentation-1.2.4/brainglobe_segmentation/tracks/fit.py`

 * *Files identical despite different names*

### Comparing `brainglobe-segmentation-1.2.3/brainglobe_segmentation/tracks/layers.py` & `brainglobe_segmentation-1.2.4/brainglobe_segmentation/tracks/layers.py`

 * *Files identical despite different names*

### Comparing `brainglobe-segmentation-1.2.3/brainglobe_segmentation.egg-info/PKG-INFO` & `brainglobe_segmentation-1.2.4/brainglobe_segmentation.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: brainglobe-segmentation
-Version: 1.2.3
+Version: 1.2.4
 Summary: Segmentation of anatomical structures in a common coordinate space
 Author-email: "Adam Tyson, Horst Obenhaus" <code@adamltyson.com>
 License: BSD-3-Clause
 Project-URL: Homepage, https://brainglobe.info/
 Project-URL: Source Code, https://github.com/brainglobe/brainglobe-segmentation
 Project-URL: Bug Tracker, https://github.com/brainglobe/brainglobe-segmentation/issues
 Project-URL: Documentation, https://brainglobe.info/documentation/brainglobe-segmentation/index.html
@@ -19,15 +19,15 @@
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Requires-Python: >=3.9
 Description-Content-Type: text/markdown
 License-File: LICENSE
 Requires-Dist: brainglobe-atlasapi>=2.0.1
 Requires-Dist: brainglobe-napari-io>=0.3.0
-Requires-Dist: brainglobe-utils>=0.4.0
+Requires-Dist: brainglobe-utils>=0.5.0
 Requires-Dist: napari>=0.4.5
 Requires-Dist: numpy
 Requires-Dist: pandas[hdf5]
 Requires-Dist: qtpy
 Requires-Dist: scikit-image
 Requires-Dist: scipy
 Requires-Dist: tifffile
```

### Comparing `brainglobe-segmentation-1.2.3/brainglobe_segmentation.egg-info/SOURCES.txt` & `brainglobe_segmentation-1.2.4/brainglobe_segmentation.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `brainglobe-segmentation-1.2.3/pyproject.toml` & `brainglobe_segmentation-1.2.4/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -16,15 +16,15 @@
     "Programming Language :: Python :: 3.10",
     "Programming Language :: Python :: 3.11",
 ]
 requires-python = ">=3.9"
 dependencies = [
     "brainglobe-atlasapi >=2.0.1",
     "brainglobe-napari-io >=0.3.0",
-    "brainglobe-utils >=0.4.0",
+    "brainglobe-utils >=0.5.0",
     "napari >=0.4.5",
     "numpy",
     "pandas[hdf5]",
     "qtpy",
     "scikit-image",
     "scipy",
     "tifffile",
```

