# Comparing `tmp/star-chart-spherical-projection-1.5.0.tar.gz` & `tmp/star-chart-spherical-projection-1.6.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/star-chart-spherical-projection-1.5.0.tar", last modified: Fri Jun 30 06:30:59 2023, max compression
+gzip compressed data, was "star-chart-spherical-projection-1.6.0.tar", last modified: Wed May 29 06:09:40 2024, max compression
```

## Comparing `star-chart-spherical-projection-1.5.0.tar` & `star-chart-spherical-projection-1.6.0.tar`

### file list

```diff
@@ -1,27 +1,30 @@
-drwxrwxr-x   0 user      (1000) user      (1000)        0 2023-06-30 06:30:59.947280 star-chart-spherical-projection-1.5.0/
--rw-rw-r--   0 user      (1000) user      (1000)      102 2022-11-20 23:38:29.000000 star-chart-spherical-projection-1.5.0/MANIFEST.in
--rw-rw-r--   0 user      (1000) user      (1000)    30585 2023-06-30 06:30:59.947280 star-chart-spherical-projection-1.5.0/PKG-INFO
--rw-rw-r--   0 user      (1000) user      (1000)    25948 2023-06-30 06:04:37.000000 star-chart-spherical-projection-1.5.0/README.md
--rw-rw-r--   0 user      (1000) user      (1000)       38 2023-06-30 06:30:59.947280 star-chart-spherical-projection-1.5.0/setup.cfg
--rw-rw-r--   0 user      (1000) user      (1000)     1944 2023-06-30 06:04:27.000000 star-chart-spherical-projection-1.5.0/setup.py
-drwxrwxr-x   0 user      (1000) user      (1000)        0 2023-06-30 06:30:59.947280 star-chart-spherical-projection-1.5.0/star_chart_spherical_projection/
--rw-rw-r--   0 user      (1000) user      (1000)      577 2023-06-29 06:41:41.000000 star-chart-spherical-projection-1.5.0/star_chart_spherical_projection/__init__.py
--rw-rw-r--   0 user      (1000) user      (1000)      149 2022-11-20 04:40:07.000000 star-chart-spherical-projection-1.5.0/star_chart_spherical_projection/config.ini
-drwxrwxr-x   0 user      (1000) user      (1000)        0 2023-06-30 06:30:59.947280 star-chart-spherical-projection-1.5.0/star_chart_spherical_projection/data/
--rw-rw-r--   0 user      (1000) user      (1000)    11181 2023-06-28 21:07:57.000000 star-chart-spherical-projection-1.5.0/star_chart_spherical_projection/data/convert_lst_to_csv_data.py
--rw-rw-r--   0 user      (1000) user      (1000)     4355 2023-06-28 19:03:19.000000 star-chart-spherical-projection-1.5.0/star_chart_spherical_projection/data/star_data.csv
--rw-rw-r--   0 user      (1000) user      (1000)     2513 2022-11-20 22:32:39.000000 star-chart-spherical-projection-1.5.0/star_chart_spherical_projection/declination_r_axis.py
--rw-rw-r--   0 user      (1000) user      (1000)    15413 2023-06-30 05:28:45.000000 star-chart-spherical-projection-1.5.0/star_chart_spherical_projection/error_handling.py
--rw-rw-r--   0 user      (1000) user      (1000)    23976 2023-06-30 05:23:55.000000 star-chart-spherical-projection-1.5.0/star_chart_spherical_projection/generate_star_chart.py
-drwxrwxr-x   0 user      (1000) user      (1000)        0 2023-06-30 06:30:59.947280 star-chart-spherical-projection-1.5.0/star_chart_spherical_projection/pytests/
--rw-rw-r--   0 user      (1000) user      (1000)     8339 2023-06-30 05:24:28.000000 star-chart-spherical-projection-1.5.0/star_chart_spherical_projection/pytests/test_finalPositionOfStars.py
--rw-rw-r--   0 user      (1000) user      (1000)    13338 2023-06-30 01:22:42.000000 star-chart-spherical-projection-1.5.0/star_chart_spherical_projection/pytests/test_plotStereographicProjection.py
--rw-rw-r--   0 user      (1000) user      (1000)    13614 2023-06-29 21:04:47.000000 star-chart-spherical-projection-1.5.0/star_chart_spherical_projection/pytests/test_starClass.py
--rw-rw-r--   0 user      (1000) user      (1000)     9126 2022-11-27 07:09:03.000000 star-chart-spherical-projection-1.5.0/star_chart_spherical_projection/ra_dec_precession_vondrak.py
--rw-rw-r--   0 user      (1000) user      (1000)     1605 2023-06-29 09:03:11.000000 star-chart-spherical-projection-1.5.0/star_chart_spherical_projection/starClass.py
-drwxrwxr-x   0 user      (1000) user      (1000)        0 2023-06-30 06:30:59.947280 star-chart-spherical-projection-1.5.0/star_chart_spherical_projection.egg-info/
--rw-rw-r--   0 user      (1000) user      (1000)    30585 2023-06-30 06:30:59.000000 star-chart-spherical-projection-1.5.0/star_chart_spherical_projection.egg-info/PKG-INFO
--rw-rw-r--   0 user      (1000) user      (1000)      974 2023-06-30 06:30:59.000000 star-chart-spherical-projection-1.5.0/star_chart_spherical_projection.egg-info/SOURCES.txt
--rw-rw-r--   0 user      (1000) user      (1000)        1 2023-06-30 06:30:59.000000 star-chart-spherical-projection-1.5.0/star_chart_spherical_projection.egg-info/dependency_links.txt
--rw-rw-r--   0 user      (1000) user      (1000)       80 2023-06-30 06:30:59.000000 star-chart-spherical-projection-1.5.0/star_chart_spherical_projection.egg-info/requires.txt
--rw-rw-r--   0 user      (1000) user      (1000)       32 2023-06-30 06:30:59.000000 star-chart-spherical-projection-1.5.0/star_chart_spherical_projection.egg-info/top_level.txt
+drwxrwxr-x   0 user      (1000) user      (1000)        0 2024-05-29 06:09:40.245323 star-chart-spherical-projection-1.6.0/
+-rw-rw-r--   0 user      (1000) user      (1000)     1066 2024-03-07 02:08:18.000000 star-chart-spherical-projection-1.6.0/LICENSE
+-rw-rw-r--   0 user      (1000) user      (1000)       51 2024-03-07 07:25:25.000000 star-chart-spherical-projection-1.6.0/MANIFEST.in
+-rw-r--r--   0 user      (1000) user      (1000)    37468 2024-05-29 06:09:40.245323 star-chart-spherical-projection-1.6.0/PKG-INFO
+-rw-rw-r--   0 user      (1000) user      (1000)    35842 2024-03-19 07:07:25.000000 star-chart-spherical-projection-1.6.0/README.md
+-rw-rw-r--   0 user      (1000) user      (1000)       38 2024-05-29 06:09:40.245323 star-chart-spherical-projection-1.6.0/setup.cfg
+-rw-rw-r--   0 user      (1000) user      (1000)     1956 2024-05-29 05:57:36.000000 star-chart-spherical-projection-1.6.0/setup.py
+drwxrwxr-x   0 user      (1000) user      (1000)        0 2024-05-29 06:09:40.233323 star-chart-spherical-projection-1.6.0/star_chart_spherical_projection/
+-rw-rw-r--   0 user      (1000) user      (1000)     1086 2024-03-07 02:08:18.000000 star-chart-spherical-projection-1.6.0/star_chart_spherical_projection/__init__.py
+drwxrwxr-x   0 user      (1000) user      (1000)        0 2024-05-29 06:09:40.237323 star-chart-spherical-projection-1.6.0/star_chart_spherical_projection/data/
+-rw-rw-r--   0 user      (1000) user      (1000)    14667 2024-03-15 05:09:41.000000 star-chart-spherical-projection-1.6.0/star_chart_spherical_projection/data/convert_lst_to_csv_data.py
+-rw-rw-r--   0 user      (1000) user      (1000)     5698 2024-03-15 05:10:01.000000 star-chart-spherical-projection-1.6.0/star_chart_spherical_projection/data/star_data.csv
+-rw-rw-r--   0 user      (1000) user      (1000)     2878 2024-03-13 07:32:16.000000 star-chart-spherical-projection-1.6.0/star_chart_spherical_projection/data/web_scrap_iau_catolog.py
+-rw-rw-r--   0 user      (1000) user      (1000)     2513 2024-03-07 02:08:18.000000 star-chart-spherical-projection-1.6.0/star_chart_spherical_projection/declination_r_axis.py
+-rw-rw-r--   0 user      (1000) user      (1000)    14121 2024-03-19 07:26:10.000000 star-chart-spherical-projection-1.6.0/star_chart_spherical_projection/error_handling.py
+-rw-rw-r--   0 user      (1000) user      (1000)    21079 2024-03-19 07:27:56.000000 star-chart-spherical-projection-1.6.0/star_chart_spherical_projection/generate_star_chart.py
+-rw-rw-r--   0 user      (1000) user      (1000)     9784 2024-03-19 07:26:31.000000 star-chart-spherical-projection-1.6.0/star_chart_spherical_projection/position_of_stars.py
+drwxrwxr-x   0 user      (1000) user      (1000)        0 2024-05-29 06:09:40.241323 star-chart-spherical-projection-1.6.0/star_chart_spherical_projection/pytests/
+-rw-rw-r--   0 user      (1000) user      (1000)     6517 2024-03-08 07:21:11.000000 star-chart-spherical-projection-1.6.0/star_chart_spherical_projection/pytests/test_errorFinalPositionOfStars.py
+-rw-rw-r--   0 user      (1000) user      (1000)     9679 2024-03-08 07:30:15.000000 star-chart-spherical-projection-1.6.0/star_chart_spherical_projection/pytests/test_errorPlotStereographicProjection.py
+-rw-rw-r--   0 user      (1000) user      (1000)     1748 2024-03-07 22:58:56.000000 star-chart-spherical-projection-1.6.0/star_chart_spherical_projection/pytests/test_errorPredictPoleStar.py
+-rw-rw-r--   0 user      (1000) user      (1000)    11075 2024-03-08 07:41:54.000000 star-chart-spherical-projection-1.6.0/star_chart_spherical_projection/pytests/test_errorStarClass.py
+-rw-rw-r--   0 user      (1000) user      (1000)     9126 2024-03-07 02:08:18.000000 star-chart-spherical-projection-1.6.0/star_chart_spherical_projection/ra_dec_precession_vondrak.py
+-rw-rw-r--   0 user      (1000) user      (1000)     1605 2024-03-07 02:08:18.000000 star-chart-spherical-projection-1.6.0/star_chart_spherical_projection/starClass.py
+drwxrwxr-x   0 user      (1000) user      (1000)        0 2024-05-29 06:09:40.241323 star-chart-spherical-projection-1.6.0/star_chart_spherical_projection.egg-info/
+-rw-r--r--   0 user      (1000) user      (1000)    37468 2024-05-29 06:09:39.000000 star-chart-spherical-projection-1.6.0/star_chart_spherical_projection.egg-info/PKG-INFO
+-rw-rw-r--   0 user      (1000) user      (1000)     1138 2024-05-29 06:09:40.000000 star-chart-spherical-projection-1.6.0/star_chart_spherical_projection.egg-info/SOURCES.txt
+-rw-rw-r--   0 user      (1000) user      (1000)        1 2024-05-29 06:09:39.000000 star-chart-spherical-projection-1.6.0/star_chart_spherical_projection.egg-info/dependency_links.txt
+-rw-rw-r--   0 user      (1000) user      (1000)       46 2024-05-29 06:09:39.000000 star-chart-spherical-projection-1.6.0/star_chart_spherical_projection.egg-info/requires.txt
+-rw-rw-r--   0 user      (1000) user      (1000)       32 2024-05-29 06:09:39.000000 star-chart-spherical-projection-1.6.0/star_chart_spherical_projection.egg-info/top_level.txt
```

### Comparing `star-chart-spherical-projection-1.5.0/README.md` & `star-chart-spherical-projection-1.6.0/PKG-INFO`

 * *Files 20% similar despite different names*

```diff
@@ -1,44 +1,68 @@
+Metadata-Version: 2.1
+Name: star-chart-spherical-projection
+Version: 1.6.0
+Summary: A Python package to generate circular astronomy star charts (past, present, and future) with spherical projection to correct for distortions with more than a hundred named stars accurate over 400,000 years with proper motion and precession of the equinoxes
+Home-page: https://github.com/cyschneck/Star-Chart-Spherical-Projection
+Download-URL: https://github.com/cyschneck/Star-Chart-Spherical-Projection/archive/refs/tags/v1.6.0.tar.gz
+Author: Cora Schneck (cyschneck)
+License: MIT
+Keywords: astronomy,python,star charts,precession,proper motion,spherical projection,stereographic projection
+Classifier: Development Status :: 4 - Beta
+Classifier: Intended Audience :: Developers
+Classifier: Intended Audience :: Education
+Classifier: Intended Audience :: Science/Research
+Classifier: License :: OSI Approved :: MIT License
+Classifier: Programming Language :: Python
+Classifier: Programming Language :: Python :: 3.9
+Classifier: Programming Language :: Python :: 3.10
+Classifier: Programming Language :: Python :: 3.11
+Classifier: Programming Language :: Python :: 3.12
+Classifier: Intended Audience :: Education
+Classifier: Intended Audience :: Science/Research
+Classifier: Topic :: Scientific/Engineering :: Physics
+Classifier: Topic :: Scientific/Engineering :: Visualization
+Classifier: Topic :: Scientific/Engineering :: Astronomy
+Requires-Python: >=3.9
+Description-Content-Type: text/markdown
+License-File: LICENSE
+Requires-Dist: beautifulsoup4
+Requires-Dist: matplotlib
+Requires-Dist: numpy
+Requires-Dist: pandas
+Requires-Dist: pytest
+
 # Star-Chart-Spherical-Projection
 
 ![PyPi](https://img.shields.io/pypi/v/star-chart-spherical-projection)
 ![license](https://img.shields.io/github/license/cyschneck/Star-Chart-Spherical-Projection)
+[![repo-status](https://www.repostatus.org/badges/latest/active.svg)](https://www.repostatus.org/#active)
 [![pytests](https://github.com/cyschneck/Star-Chart-Spherical-Projection/actions/workflows/pytests.yml/badge.svg?branch=main)](https://github.com/cyschneck/Star-Chart-Spherical-Projection/actions/workflows/pytests.yml)
 
-A Python package to generate circular astronomy star charts (past, present, and future) with spherical projection to correct for distortions with more than a hundred named stars accurate over 400,000 years with proper motion and precession of the equinoxes
+A Python package to generate circular astronomy star charts (past, present, and future) with spherical projection to correct for distortions with all IAU named stars accurate over 400,000 years with proper motion and precession of the equinoxes
 
 * **Plot Stars on a Polar Chart**
 	* plotStereographicProjection()
 * **Return Final Position of Stars**
 	* finalPositionOfStars()
+	* starPositionOverTime()
+	* predictPoleStar()
 * **Add a New Star to Plot**
 	* newStar()
 
-The first step to plot the celestial sphere onto a 2D plot is to map the star's right ascension as hours along the plot (matplotlib polar plot's theta value) and declination as the distance from the center of the circle (matplotlib polar plot's radius value). However, attempting to map the right ascension and declination directly will cause distortion since the angles between the stars along the declination are no longer conserved. On the left, the constellation of the Big Dipper is stretched into an unfamiliar shape due to this distortion. By accounting for the spherical transformation, the star chart can be corrected as seen on the right.
-
-| Without Correction | With Correction |
-| ------------- | ------------- |
-| ![without_correction](https://user-images.githubusercontent.com/22159116/202333014-a53f1176-182f-43c7-ab92-266d15d8c563.jpg) | ![with_correction](https://user-images.githubusercontent.com/22159116/202333015-493619f4-a5b8-4614-8b32-54225d7fad02.png) |
-
-The sphere is projected from the South Pole (via [Stereographic projection](https://gisgeography.com/azimuthal-projection-orthographic-stereographic-gnomonic/)):
- <p align="center">
-  <img src="https://gisgeography.com/wp-content/uploads/2016/12/Stereographic-Projection-768x421.png" />
-</p>
-
-
 ## Quickstart: Star-Chart-Spherical-Projection
-Plot stars in the Southern Hemisphere for the year 2023 (without stars labels)
+Plot stars in the Southern Hemisphere for the year 2024 (without stars labels)
 ```python
 import star_chart_spherical_projection as scsp
 
 scsp.plotStereographicProjection(northOrSouth="South",
 				displayStarNamesLabels=False,
-				yearSince2000=23)
+				yearSince2000=24)
 ```
-![quickstart_star_chart+png](https://raw.githubusercontent.com/cyschneck/Star-Chart-Spherical-Projection/main/examples/quickstart_south_2023.png) 
+![quickstart_star_chart+png](https://raw.githubusercontent.com/cyschneck/Star-Chart-Spherical-Projection/main/examples/quickstart_south_years.png) 
 
 Plot a few built-in stars as well as two new user defined stars in the Northern Hemisphere for the year 1961 (2000-39) (with stars labels and in red). This uses both methods to define the proper motion for new stars: with a given proper motion and angle and with the proper motion speed in the declination and right ascension
 ```python
 import star_chart_spherical_projection as scsp
 
 exalibur_star = scsp.newStar(starName="Exalibur",
 				ra="14.04.23",
@@ -62,37 +86,43 @@
 ![quickstart_star_chart+png](https://raw.githubusercontent.com/cyschneck/Star-Chart-Spherical-Projection/main/examples/quickstart_newstar_example.png) 
 
 
 Return the final position of a Vega (can be a single star or a list of stars) after 11,500 years when Vega is the new North Pole Star (star closest to +90°)
 ```python
 import star_chart_spherical_projection as scsp
 
-star_final_pos_dict = scsp.finalPositionOfStars(builtInStars=["Vega"], yearSince2000=11500, save_to_csv="final_star_positions.csv")
+star_final_pos_dict = scsp.finalPositionOfStars(builtInStars=["Vega"],
+						yearSince2000=11500,
+						save_to_csv="final_star_positions.csv")
 ```
 Returns a dictionary with a star and its declination and right ascension: `{'Vega': {'Declination': 83.6899118156341, 'RA': '05.38.21'}}`
 
 The final position of the stars are saved in `final_star_positions.csv` with the headers ["Star Name", "Right Ascension (HH.MM.SS)", "Declination (DD.SS)"]
 
 ## Install
 
 PyPi pip install at [pypi.org/project/star-chart-spherical-projection/](https://pypi.org/project/star-chart-spherical-projection/)
 
 ```
 pip install star-chart-spherical-projection
 ```
 
-## Requirements
+## Overview
 
-Python 3.7+
-```
-pip install -r requirements.txt
-```
-Requirements will also be downloaded as part of the pip download
+The first step to plot the celestial sphere onto a 2D plot is to map the star's right ascension as hours along the plot (matplotlib polar plot's theta value) and declination as the distance from the center of the circle (matplotlib polar plot's radius value). However, attempting to map the right ascension and declination directly will cause distortion since the angles between the stars along the declination are no longer conserved. On the left, the constellation of the Big Dipper is stretched into an unfamiliar shape due to this distortion. By accounting for the spherical transformation, the star chart can be corrected as seen on the right.
+
+| Without Correction | With Correction |
+| ------------- | ------------- |
+| ![without_correction](https://user-images.githubusercontent.com/22159116/202333014-a53f1176-182f-43c7-ab92-266d15d8c563.jpg) | ![with_correction](https://user-images.githubusercontent.com/22159116/202333015-493619f4-a5b8-4614-8b32-54225d7fad02.png) |
+
+The sphere is projected from the South Pole (via [Stereographic projection](https://gisgeography.com/azimuthal-projection-orthographic-stereographic-gnomonic/)):
+ <p align="center">
+  <img src="https://gisgeography.com/wp-content/uploads/2016/12/Stereographic-Projection-768x421.png" />
+</p>
 
-## Overview
 
 From the perspective of an observer on the Earth's surface, the stars appear to sit along the surface of the celestial sphere--an imaginary sphere of arbitrary radius with the Earth at its center. All objects in the sky will appear projected on the celestial sphere regardless of their true distance from Earth. Each star's position is given by two values. Declination is the angular distance from the celestial equator and right ascension is the distance from the position of the vernal equinox. During the course of a full 24-hour day, stars will appear to rotate across the sky as a result of the Earth's rotation, but their position is fixed. A star’s actual position does change over time as the combined result of the star’s small movement (proper motion) as well as the changing rotational axis of the Earth (precession).
  
  <p align="center">
   <img src="https://upload.wikimedia.org/wikipedia/commons/1/12/Earth_within_celestial_sphere.gif" />
 </p>
 
@@ -122,56 +152,46 @@
 star_chart_spherical_projection.newStar(starName=None,
 					ra=None,
 					dec=None,
 					properMotionSpeed=None,
 					properMotionAngle=None,
 					magnitudeVisual=None)
 ```
-* **[REQUIRED]** starName (string): A star name to be displayed as a label
-* **[REQUIRED]** ra (string): Right Ascension of star as a string with three parts 'HH.MM.SS' (Hours, Minutes, Seconds)
-* **[REQUIRED]** dec (int/float): Declination of star (a positive or negative value)
-* **[REQUIRED]** properMotionSpeed (int/float): Proper motion speed as a single value (in mas/year)
-* **[REQUIRED]** properMotionAngle (int/float): Proper motion positive angle (between 0° and 360°)
-* **[REQUIRED]** magnitudeVisual (int/float): Absolute Visual Magnitude
+* **[REQUIRED]** starName: (string) A star name to be displayed as a label
+* **[REQUIRED]** ra: (string) Right Ascension of star as a string with three parts 'HH.MM.SS' (Hours, Minutes, Seconds)
+* **[REQUIRED]** dec: (int/float) Declination of star (a positive or negative value)
+* **[REQUIRED]** properMotionSpeed: (int/float) Proper motion speed as a single value (in mas/year)
+* **[REQUIRED]** properMotionAngle: (int/float) Proper motion positive angle (between 0° and 360°)
+* **[REQUIRED]** magnitudeVisual: (int/float) Absolute Visual Magnitude
 
 **With the Proper Motion speed along the Right Ascension and Declination**
 
 As seen in [wikipeida.og for Pollux](https://en.wikipedia.org/wiki/Pollux_(star))
 
 ```
 star_chart_spherical_projection.newStar(starName=None,
 					ra=None,
 					dec=None,
 					properMotionSpeedRA=None,
 					properMotionSpeedDec=None,
 					magnitudeVisual=None)
 ```
-* **[REQUIRED]** starName (string): A star name to be displayed as a label
-* **[REQUIRED]** ra (string): Right Ascension of star as a string with three parts 'HH.MM.SS' (Hours, Minutes, Seconds)
-* **[REQUIRED]** dec (int/float): Declination of star (a positive or negative value)
-* **[REQUIRED]** properMotionSpeedRA (int/float): Speed of Proper Motion along the Right Ascension
-* **[REQUIRED]** properMotionSpeedDec (int/float): Speed of Proper Motion along the Declination
-* **[REQUIRED]** magnitudeVisual (int/float):
+* **[REQUIRED]** starName: (string) A star name to be displayed as a label
+* **[REQUIRED]** ra: (string) Right Ascension of star as a string with three parts 'HH.MM.SS' (Hours, Minutes, Seconds)
+* **[REQUIRED]** dec: (int/float) Declination of star (a positive or negative value)
+* **[REQUIRED]** properMotionSpeedRA: (int/float) Speed of Proper Motion along the Right Ascension
+* **[REQUIRED]** properMotionSpeedDec: (int/float) Speed of Proper Motion along the Declination
+* **[REQUIRED]** magnitudeVisual: (int/float) Absolute Visual Magnitude
 
 Important Note: RA/Dec proper motion will be converted from speed along the right ascension and declination to a proper motion speed (`properMotionSpeed`) and an angle (`properMotionAngle`) for further calculations
 
 <details closed>
 <summary>Stars Built-in (Click to view all)</summary>
 <br>
-['Acamar', 'Achernar', 'Acrab', 'Acrux', 'Adhara', 'Aldebaran', 'Alderamin', 'Algieba', 'Algol', 'Alhena', 
-'Alioth', 'Alkaid', 'Almach', 'Alnilam', 'Alnitak', 'Alphard', 'Alphecca', 'Alpheratz', 'Altair', 'Aludra', 
-'Ankaa', 'Antares', 'Arcturus', 'Arneb', 'Ascella', 'Aspidiske', 'Atria', 'Avior', 'Bellatrix', 'Beta Hydri', 
-'Beta Phoenicis', 'Betelgeuse', 'Canopus', 'Capella', 'Caph', 'Castor', 'Cebalrai', 'Celaeno', 'Chara', 
-'Cor-Caroli', 'Cursa', 'Delta Crucis', 'Deneb', 'Denebola', 'Diphda', 'Dschubba', 'Dubhe', 'Elnath', 'Eltanin', 
-'Enif', 'Formalhaut', 'Gacrux', 'Gamma Phoenicis', 'Gienah', 'Hadar', 'Hamal', 'Kochab', 'Kornephoros', 'Lesath', 
-'Markab', 'Megrez', 'Meissa', 'Menkalinan', 'Menkar', 'Menkent', 'Merak', 'Miaplacidus', 'Mimosa', 'Mintaka', 
-'Mirach', 'Mirfak', 'Mirzam', 'Mizar', 'Muphrid', 'Naos', 'Navi', 'Nunki', 'Peacock', 'Phact', 'Phecda', 'Polaris', 
-'Pollux', 'Procyon', 'Rasalhague', 'Rastaban', 'Regulus', 'Rigel', 'Ruchbah', 'Sabik', 'Sadr', 'Saiph', 'Sargas', 
-'Scheat', 'Schedar', 'Segin', 'Seginus', 'Shaula', 'Sheratan', 'Sirius', 'Spica', 'Suhail', 'Tarazed', 'Thuban', 
-'Unukalhai', 'Vega', 'Wezen', 'Zosma', 'Zubeneschamali']
+['Acamar', 'Achernar', 'Acrab', 'Acrux', 'Adhara', 'Aldebaran', 'Alderamin', 'Algieba', 'Algol', 'Alhena', 'Alioth', 'Alkaid', 'Almach', 'Alnair', 'Alnilam', 'Alnitak', 'Alphard', 'Alphecca', 'Alpheratz', 'Altair', 'Aludra', 'Ankaa', 'Antares', 'Arcturus', 'Arneb', 'Ascella', 'Aspidiske', 'Atria', 'Avior', 'Bellatrix', 'Beta Hydri', 'Beta Phoenicis', 'Betelgeuse', 'Canopus', 'Capella', 'Caph', 'Castor', 'Cebalrai', 'Celaeno', 'Chara', 'Cor-Caroli', 'Cursa', 'Delta Crucis', 'Delta Velorum', 'Deneb', 'Denebola', 'Diphda', 'Dschubba', 'Dubhe', 'Elnath', 'Eltanin', 'Enif', 'Formalhaut', 'Gacrux', 'Gamma Phoenicis', 'Gienah', 'Hadar', 'Hamal', 'Kaus Australis', 'Kochab', 'Kornephoros', 'Lesath', 'Markab', 'Megrez', 'Meissa', 'Menkalinan', 'Menkar', 'Menkent', 'Merak', 'Miaplacidus', 'Mimosa', 'Mintaka', 'Mirach', 'Mirfak', 'Mirzam', 'Mizar', 'Muphrid', 'Naos', 'Navi', 'Nunki', 'Peacock', 'Phact', 'Phecda', 'Polaris', 'Pollux', 'Procyon', 'Rasalhague', 'Rastaban', 'Regulus', 'Rigel', 'Ruchbah', 'Sabik', 'Sadr', 'Saiph', 'Sargas', 'Scheat', 'Schedar', 'Segin', 'Seginus', 'Shaula', 'Sheratan', 'Sirius', 'Spica', 'Suhail', 'Tarazed', 'Thuban', 'Tureis', 'Unukalhai', 'Vega', 'Wezen', 'Zosma', 'Zubeneschamali']
 </details>
 
 ## Plot Stars on a Polar Chart
 **plotStereographicProjection()**
 
 Plot stars on a Stereographic Polar Plot
 ```
@@ -200,86 +220,234 @@
 - *[OPTIONAL]* displayStarNamesLabels: (boolean) display the star name labels, defaults to True
 - *[OPTIONAL]* displayDeclinationNumbers: (boolean) display declination values, defaults to True
 - *[OPTIONAL]* incrementBy: (int) increment values for declination (either 1, 5, 10), defaults to 10
 - *[OPTIONAL]* isPrecessionIncluded: (boolean) when calculating star positions include predictions for precession, defaults to True
 - *[OPTIONAL]* maxMagnitudeFilter: (int/float) filter existing stars by magnitude by setting the max magnitude for the chart to include, defaults to None (shows all stars)
 - *[OPTIONAL]* userDefinedStars: (list) List of newStar objects of stars the user has added
 - *[OPTIONAL]* onlyDisplayUserStars: (bool) Only display the stars defined by the users (userDefinedStars)
-- *[OPTIONAL]* showPlot: (boolean) show plot (triggers plt.show()) when finished running, defaults to True
+- *[OPTIONAL]* showPlot: (boolean) show plot (triggers plt.show()), useful when generating multiple plots at once in the background, defaults to True
 - *[OPTIONAL]* fig_plot_title: (string) figure title, defaults to "<North/South>ern Hemisphere [<YEAR NUMBERS> Years Since 2000 (YYYY)]: +/-90° to <DECLINATION MIN>°"
 - *[OPTIONAL]* fig_plot_color: (string) scatter plot star color, defaults to C0
 - *[OPTIONAL]* figsize_n: (int/float) figure size, default to 12
 - *[OPTIONAL]* figsize_dpi: (int/float) figure DPI, default to 100
 - *[OPTIONAL]* save_plot_name: (string) save plot with a string name, defaults to not saving
 
 <details closed>
 <summary>Stars that will be included by default when builtInStars = [] (Click to view all)</summary>
 <br>
-['Acamar', 'Achernar', 'Acrab', 'Acrux', 'Adhara', 'Aldebaran', 'Alderamin', 'Algieba', 'Algol', 'Alhena', 
-'Alioth', 'Alkaid', 'Almach', 'Alnilam', 'Alnitak', 'Alphard', 'Alphecca', 'Alpheratz', 'Altair', 'Aludra', 
-'Ankaa', 'Antares', 'Arcturus', 'Arneb', 'Ascella', 'Aspidiske', 'Atria', 'Avior', 'Bellatrix', 'Beta Hydri', 
-'Beta Phoenicis', 'Betelgeuse', 'Canopus', 'Capella', 'Caph', 'Castor', 'Cebalrai', 'Celaeno', 'Chara', 
-'Cor-Caroli', 'Cursa', 'Delta Crucis', 'Deneb', 'Denebola', 'Diphda', 'Dschubba', 'Dubhe', 'Elnath', 'Eltanin', 
-'Enif', 'Formalhaut', 'Gacrux', 'Gamma Phoenicis', 'Gienah', 'Hadar', 'Hamal', 'Kochab', 'Kornephoros', 'Lesath', 
-'Markab', 'Megrez', 'Meissa', 'Menkalinan', 'Menkar', 'Menkent', 'Merak', 'Miaplacidus', 'Mimosa', 'Mintaka', 
-'Mirach', 'Mirfak', 'Mirzam', 'Mizar', 'Muphrid', 'Naos', 'Navi', 'Nunki', 'Peacock', 'Phact', 'Phecda', 'Polaris', 
-'Pollux', 'Procyon', 'Rasalhague', 'Rastaban', 'Regulus', 'Rigel', 'Ruchbah', 'Sabik', 'Sadr', 'Saiph', 'Sargas', 
-'Scheat', 'Schedar', 'Segin', 'Seginus', 'Shaula', 'Sheratan', 'Sirius', 'Spica', 'Suhail', 'Tarazed', 'Thuban', 
-'Unukalhai', 'Vega', 'Wezen', 'Zosma', 'Zubeneschamali']
+['Acamar', 'Achernar', 'Acrab', 'Acrux', 'Adhara', 'Aldebaran', 'Alderamin', 'Algieba', 'Algol', 'Alhena', 'Alioth', 'Alkaid', 'Almach', 'Alnair', 'Alnilam', 'Alnitak', 'Alphard', 'Alphecca', 'Alpheratz', 'Altair', 'Aludra', 'Ankaa', 'Antares', 'Arcturus', 'Arneb', 'Ascella', 'Aspidiske', 'Atria', 'Avior', 'Bellatrix', 'Beta Hydri', 'Beta Phoenicis', 'Betelgeuse', 'Canopus', 'Capella', 'Caph', 'Castor', 'Cebalrai', 'Celaeno', 'Chara', 'Cor-Caroli', 'Cursa', 'Delta Crucis', 'Delta Velorum', 'Deneb', 'Denebola', 'Diphda', 'Dschubba', 'Dubhe', 'Elnath', 'Eltanin', 'Enif', 'Formalhaut', 'Gacrux', 'Gamma Phoenicis', 'Gienah', 'Hadar', 'Hamal', 'Kaus Australis', 'Kochab', 'Kornephoros', 'Lesath', 'Markab', 'Megrez', 'Meissa', 'Menkalinan', 'Menkar', 'Menkent', 'Merak', 'Miaplacidus', 'Mimosa', 'Mintaka', 'Mirach', 'Mirfak', 'Mirzam', 'Mizar', 'Muphrid', 'Naos', 'Navi', 'Nunki', 'Peacock', 'Phact', 'Phecda', 'Polaris', 'Pollux', 'Procyon', 'Rasalhague', 'Rastaban', 'Regulus', 'Rigel', 'Ruchbah', 'Sabik', 'Sadr', 'Saiph', 'Sargas', 'Scheat', 'Schedar', 'Segin', 'Seginus', 'Shaula', 'Sheratan', 'Sirius', 'Spica', 'Suhail', 'Tarazed', 'Thuban', 'Tureis', 'Unukalhai', 'Vega', 'Wezen', 'Zosma', 'Zubeneschamali']
 </details>
 
 | northOrSouth="North" (-30° to 90°) (without star labels) | northOrSouth="South" (30° to -90°) (without star labels) |
 | ------------- | ------------- |
 | ![northOrSouth+png](https://raw.githubusercontent.com/cyschneck/Star-Chart-Spherical-Projection/main/examples/northOrSouth_north.png) |  ![northOrSouth+png](https://raw.githubusercontent.com/cyschneck/Star-Chart-Spherical-Projection/main/examples/northOrSouth_south.png) |
 
 | builtInStars=[] (Includes all stars, default) | builtInStars=["Vega", "Arcturus", "Enif", "Caph", "Mimosa"]|
 | ------------- | ------------- |
-| ![builtInStars+png](https://raw.githubusercontent.com/cyschneck/Star-Chart-Spherical-Projection/main/examples/declination_min_default.png) | ![builtInStars+png](https://raw.githubusercontent.com/cyschneck/Star-Chart-Spherical-Projection/main/examples/builtInStars_subset.png) |
+| ![builtInStars+png](https://raw.githubusercontent.com/cyschneck/Star-Chart-Spherical-Projection/main/examples/builtInStars_default.png) | ![builtInStars+png](https://raw.githubusercontent.com/cyschneck/Star-Chart-Spherical-Projection/main/examples/builtInStars_subset.png) |
 
 | declination_min=-30° (default) | declination_min=10° |
 | ------------- | ------------- |
-| ![declination_min+png](https://raw.githubusercontent.com/cyschneck/Star-Chart-Spherical-Projection/main/examples/declination_min_default.png) | ![declination_min+png](https://raw.githubusercontent.com/cyschneck/Star-Chart-Spherical-Projection/main/examples/declination_min_20.png) |
+| ![declination_min+png](https://raw.githubusercontent.com/cyschneck/Star-Chart-Spherical-Projection/main/examples/declination_min_default.png) | ![declination_min+png](https://raw.githubusercontent.com/cyschneck/Star-Chart-Spherical-Projection/main/examples/declination_min_10.png) |
 
 | yearSince2000=0 (default) | yearSince2000=-3100 |
 | ------------- | ------------- |
-| ![declination_min+png](https://raw.githubusercontent.com/cyschneck/Star-Chart-Spherical-Projection/main/examples/declination_min_default.png) | ![declination_min+png](https://raw.githubusercontent.com/cyschneck/Star-Chart-Spherical-Projection/main/examples/yearSince2000_1100.png) |
+| ![declination_min+png](https://raw.githubusercontent.com/cyschneck/Star-Chart-Spherical-Projection/main/examples/yearSince2000_default.png) | ![declination_min+png](https://raw.githubusercontent.com/cyschneck/Star-Chart-Spherical-Projection/main/examples/yearSince2000_negative_3100.png) |
 
 | displayStarNamesLabels=True (default) | displayStarNamesLabels=False |
 | ------------- | ------------- |
 | ![displayStarNamesLabels+png](https://raw.githubusercontent.com/cyschneck/Star-Chart-Spherical-Projection/main/examples/displayStarNamesLabels_default.png)  | ![displayStarNamesLabels+png](https://raw.githubusercontent.com/cyschneck/Star-Chart-Spherical-Projection/main/examples/displayStarNamesLabels_false.png) |
 
 | displayDeclinationNumbers=True (default) (without star labels) | displayDeclinationNumbers=False (without star labels) |
 | ------------- | ------------- |
 | ![displayDeclinationNumbers+png](https://raw.githubusercontent.com/cyschneck/Star-Chart-Spherical-Projection/main/examples/displayDeclinationNumbers_default.png)  | ![displayDeclinationNumbers+png](https://raw.githubusercontent.com/cyschneck/Star-Chart-Spherical-Projection/main/examples/displayDeclinationNumbers_false.png) |
 
 | incrementBy=10 (default) (without star labels) | incrementBy=5 (without star labels) |
 | ------------- | ------------- |
 | ![incrementBy_default+png](https://raw.githubusercontent.com/cyschneck/Star-Chart-Spherical-Projection/main/examples/incrementBy_default.png) | ![incrementBy_5+png](https://raw.githubusercontent.com/cyschneck/Star-Chart-Spherical-Projection/main/examples/incrementBy_5.png) |
 
-| isPrecessionIncluded=True (default) | isPrecessionIncluded=False |
+| isPrecessionIncluded=True (default) (yearSince2000=11500) | isPrecessionIncluded=False (yearSince2000=11500) |
 | ------------- | ------------- |
 | ![isPrecessionIncluded_default+png](https://raw.githubusercontent.com/cyschneck/Star-Chart-Spherical-Projection/main/examples/isPrecessionIncluded_default.png) | ![isPrecessionIncluded_false+png](https://raw.githubusercontent.com/cyschneck/Star-Chart-Spherical-Projection/main/examples/isPrecessionIncluded_false.png) |
 
 | maxMagnitudeFilter=None (default) | maxMagnitudeFilter=1 |
 | ------------- | ------------- |
 | ![maxMagnitudeFilter_default+png](https://raw.githubusercontent.com/cyschneck/Star-Chart-Spherical-Projection/main/examples/maxMagnitudeFilter_default.png) | ![maxMagnitudeFilter+png](https://raw.githubusercontent.com/cyschneck/Star-Chart-Spherical-Projection/main/examples/maxMagnitudeFilter_1.png) |
 
-| onlyDisplayUserStars=False (default) with userDefinedStars | onlyDisplayUserStars=True with userDefined Stars |
+| userDefinedStars=[] (default) (with just "Vega") | userDefinedStars=[exalibur_star, karaboudjan_star] (from Quickstart with "Vega") |
+| ------------- | ------------- |
+| ![userDefinedStars_default+png](https://raw.githubusercontent.com/cyschneck/Star-Chart-Spherical-Projection/main/examples/userDefinedStars_none.png) | ![userDefinedStars+png](https://raw.githubusercontent.com/cyschneck/Star-Chart-Spherical-Projection/main/examples/userDefinedStars_included.png) |
+
+| onlyDisplayUserStars=False (default) with userDefinedStars | onlyDisplayUserStars=True with userDefinedStars=[exalibur_star, karaboudjan_star] (from Quickstart) |
 | ------------- | ------------- |
 | ![onlyDisplayUserStars_default+png](https://raw.githubusercontent.com/cyschneck/Star-Chart-Spherical-Projection/main/examples/onlyDisplayUserStars_default.png) | ![onlyDisplayUserStars+png](https://raw.githubusercontent.com/cyschneck/Star-Chart-Spherical-Projection/main/examples/onlyDisplayUserStars_true.png) |
 
 | fig_plot_title=(default) | fig_plot_title="This is a Example Title for a Star Chart" |
 | ------------- | ------------- |
 | ![fig_plot_title_default+png](https://raw.githubusercontent.com/cyschneck/Star-Chart-Spherical-Projection/main/examples/fig_plot_title_default.png) | ![fig_plot_title+png](https://raw.githubusercontent.com/cyschneck/Star-Chart-Spherical-Projection/main/examples/fig_plot_title_example.png) |
 
 | fig_plot_color="C0" (default) (without star labels) | fig_plot_color="darkorchid" (without star labels) |
 | ------------- | ------------- |
 | ![fig_plot_color_default+png](https://raw.githubusercontent.com/cyschneck/Star-Chart-Spherical-Projection/main/examples/fig_plot_color_default.png) | ![fig_plot_color_dark_orchid+png](https://raw.githubusercontent.com/cyschneck/Star-Chart-Spherical-Projection/main/examples/fig_plot_color_darkorchid.png) |
 
-### Star Chart Examples:
+## Return Final Position of Stars
+**finalPositionOfStars()**
+
+Returns a dictionary for the final positions of the stars for a specific year in the format: {'Star Name': {"Declination" : Declination (int), "RA": RA (str)}
+```
+finalPositionOfStars(builtInStars=[],
+		yearSince2000=0, 
+		isPrecessionIncluded=True,
+		userDefinedStars=[],
+		onlyDisplayUserStars=False,
+		declination_min=None,
+		declination_max=None,
+		save_to_csv=None)
+```
+- *[OPTIONAL]* builtInStars: (list) a list of star names to include from built-in list, by default = [] includes all stars (in star_data.csv). Example: ["Vega", "Merak", "Dubhe"]
+- *[OPTIONAL]* yearSince2000: (int/float) years since 2000 (-50 = 1950 and +50 = 2050) to calculate proper motion and precession, defaults = 0 years
+- *[OPTIONAL]* isPrecessionIncluded: (boolean) when calculating star positions include predictions for precession, defaults to True
+- *[OPTIONAL]* userDefinedStars: (list): List of newStar objects of stars the user has added
+- *[OPTIONAL]* onlyDisplayUserStars: (bool) Only include the stars defined by the users (userDefinedStars)
+- *[OPTIONAL]* declination_min: (int/float) set minimum declination value, defaults to -30° in Northern hemisphere and 30° in Southern hemisphere
+- *[OPTIONAL]* declination_max: (int/float) set maximum declination value, defaults to 90° in Northern hemisphere and -90° in Southern hemisphere
+- *[OPTIONAL]* save_to_csv: (string) CSV filename and location to save final star positions with headers ["Star Name", "Right Ascension (HH.MM.SS)", "Declination (DD.SS)"]
+
+<details closed>
+<summary>Stars that will be included by default when builtInStars = [] (Click to view all)</summary>
+<br>
+['Acamar', 'Achernar', 'Acrab', 'Acrux', 'Adhara', 'Aldebaran', 'Alderamin', 'Algieba', 'Algol', 'Alhena', 'Alioth', 'Alkaid', 'Almach', 'Alnair', 'Alnilam', 'Alnitak', 'Alphard', 'Alphecca', 'Alpheratz', 'Altair', 'Aludra', 'Ankaa', 'Antares', 'Arcturus', 'Arneb', 'Ascella', 'Aspidiske', 'Atria', 'Avior', 'Bellatrix', 'Beta Hydri', 'Beta Phoenicis', 'Betelgeuse', 'Canopus', 'Capella', 'Caph', 'Castor', 'Cebalrai', 'Celaeno', 'Chara', 'Cor-Caroli', 'Cursa', 'Delta Crucis', 'Delta Velorum', 'Deneb', 'Denebola', 'Diphda', 'Dschubba', 'Dubhe', 'Elnath', 'Eltanin', 'Enif', 'Formalhaut', 'Gacrux', 'Gamma Phoenicis', 'Gienah', 'Hadar', 'Hamal', 'Kaus Australis', 'Kochab', 'Kornephoros', 'Lesath', 'Markab', 'Megrez', 'Meissa', 'Menkalinan', 'Menkar', 'Menkent', 'Merak', 'Miaplacidus', 'Mimosa', 'Mintaka', 'Mirach', 'Mirfak', 'Mirzam', 'Mizar', 'Muphrid', 'Naos', 'Navi', 'Nunki', 'Peacock', 'Phact', 'Phecda', 'Polaris', 'Pollux', 'Procyon', 'Rasalhague', 'Rastaban', 'Regulus', 'Rigel', 'Ruchbah', 'Sabik', 'Sadr', 'Saiph', 'Sargas', 'Scheat', 'Schedar', 'Segin', 'Seginus', 'Shaula', 'Sheratan', 'Sirius', 'Spica', 'Suhail', 'Tarazed', 'Thuban', 'Tureis', 'Unukalhai', 'Vega', 'Wezen', 'Zosma', 'Zubeneschamali']
+</details>
+
+## Return A Star's Position over Time
+**starPositionOverTime()**
+
+Returns a single star's position over time
+
+```
+starPositionOverTime(builtInStarName=None,
+			newStar=None,
+			startYearSince2000=None,
+			endYearSince2000=None,
+			incrementYear=5,
+			isPrecessionIncluded=True,
+			save_to_csv=None)
+```
+- **[REQUIRED]** builtInStarName: (string) a star name from the built-in list, example: `Vega`
+- **[REQUIRED]** newStar: (newStar object) a new star included created from a newStar objct
+- **[REQUIRED]** startYearSince2000: (float/int) start year since 2000 (-50 = 1950 and +50 = 2050) to calculate proper motion and precession, defaults = 0 years
+- **[REQUIRED]** endYearSince2000: (float/int) end year since 2000 (-50 = 1950 and +50 = 2050) to calculate proper motion and precession, defaults = 0 years
+- **[REQUIRED]** incrementYear: (float/int) number of year to increment from start to end by, defaults to `5` years
+- *[OPTIONAL]* isPrecessionIncluded: (boolean) when calculating star positions include predictions for precession, defaults to True
+- *[OPTIONAL]* save_to_csv: (string) CSV filename and location to save star's position over time with headers ["Year", "Declination (DD.SS)", "Right Ascension (HH.MM.SS)", "Right Ascension (radians)"]
+
+<details closed>
+<summary>Stars Built-in (Click to view all)</summary>
+<br>
+['Acamar', 'Achernar', 'Acrab', 'Acrux', 'Adhara', 'Aldebaran', 'Alderamin', 'Algieba', 'Algol', 'Alhena', 'Alioth', 'Alkaid', 'Almach', 'Alnair', 'Alnilam', 'Alnitak', 'Alphard', 'Alphecca', 'Alpheratz', 'Altair', 'Aludra', 'Ankaa', 'Antares', 'Arcturus', 'Arneb', 'Ascella', 'Aspidiske', 'Atria', 'Avior', 'Bellatrix', 'Beta Hydri', 'Beta Phoenicis', 'Betelgeuse', 'Canopus', 'Capella', 'Caph', 'Castor', 'Cebalrai', 'Celaeno', 'Chara', 'Cor-Caroli', 'Cursa', 'Delta Crucis', 'Delta Velorum', 'Deneb', 'Denebola', 'Diphda', 'Dschubba', 'Dubhe', 'Elnath', 'Eltanin', 'Enif', 'Formalhaut', 'Gacrux', 'Gamma Phoenicis', 'Gienah', 'Hadar', 'Hamal', 'Kaus Australis', 'Kochab', 'Kornephoros', 'Lesath', 'Markab', 'Megrez', 'Meissa', 'Menkalinan', 'Menkar', 'Menkent', 'Merak', 'Miaplacidus', 'Mimosa', 'Mintaka', 'Mirach', 'Mirfak', 'Mirzam', 'Mizar', 'Muphrid', 'Naos', 'Navi', 'Nunki', 'Peacock', 'Phact', 'Phecda', 'Polaris', 'Pollux', 'Procyon', 'Rasalhague', 'Rastaban', 'Regulus', 'Rigel', 'Ruchbah', 'Sabik', 'Sadr', 'Saiph', 'Sargas', 'Scheat', 'Schedar', 'Segin', 'Seginus', 'Shaula', 'Sheratan', 'Sirius', 'Spica', 'Suhail', 'Tarazed', 'Thuban', 'Tureis', 'Unukalhai', 'Vega', 'Wezen', 'Zosma', 'Zubeneschamali']
+</details>
+
+## Predict Past and Future Pole Stars
+**predictPoleStar**
+
+Return the North/South Pole star for a given year since 2000
+```
+predictPoleStar(yearSince2000=0, northOrSouth="North")
+```
+- **[REQUIRED]** yearSince2000 (int/float): ear since 2000 (-50 = 1950 and +50 = 2050) to calculate proper motion and precession, defaults = 0 years
+- *[OPTIONAL]* northOrSouth (string): North or South Pole where `North` = 90° and `South` = -90°, defaults to `North`
+
+## Plot a Star's Position over Time
+**plotStarPositionOverTime()**
+
+Plot a star's declination and right ascension position over time
+
+```
+plotStarPositionOverTime(builtInStarName=None, 
+			newStar=None,
+			startYearSince2000=None,
+			endYearSince2000=None,
+			incrementYear=10,
+			isPrecessionIncluded=True,
+			DecOrRA="D",
+			showPlot=True,
+			showYearMarker=True,
+			fig_plot_title=None,
+			fig_plot_color="C0",
+			figsize_n=12,
+			figsize_dpi=100,
+			save_plot_name=None)
+```
+- **[REQUIRED]** builtInStarName: (string) a star name from the built-in list, example: `Vega`
+- **[REQUIRED]** newStar: (newStar object) a new star included created from a newStar objct
+- **[REQUIRED]** startYearSince2000: (float/int) start year since 2000 (-50 = 1950 and +50 = 2050) to calculate proper motion and precession, defaults = 0 years
+- **[REQUIRED]** endYearSince2000: (float/int) end year since 2000 (-50 = 1950 and +50 = 2050) to calculate proper motion and precession, defaults = 0 years
+- **[REQUIRED]** DecOrRA: (string) Plot the Declination `D` or Right Ascension `RA`, defaults to `D`
+- **[REQUIRED]** incrementYear: (float/int)  number of year to increment from start to end by, defaults to `10` years
+- *[OPTIONAL]* isPrecessionIncluded: (boolean)  when calculating star positions include predictions for precession, defaults to True
+- *[OPTIONAL]* showPlot: (boolean) show plot (triggers plt.show()), useful when generating multiple plots at once in the background, defaults to True
+- *[OPTIONAL]* showYearMarker: (boolean) show dotted line for current year
+- *[OPTIONAL]* fig_plot_title: (string) figure plot title, defaults to `<STAR NAME> <DECLINATION/RA> (<With/Without> Precession) from <START BCE/CE> to <END BCE/CE>, every <YEAR INCREMENT> Years`
+- *[OPTIONAL]* fig_plot_color: (string) figure plot color, defaults to blue `C0`
+- *[OPTIONAL]* figsize_n: (float/int) figure plot size NxN, `12`
+- *[OPTIONAL]* figsize_dpi: (float/int) figure dpi, defaults to `100`
+- *[OPTIONAL]* save_plot_name: (string) save plot name and location
+
+<details closed>
+<summary>Stars Built-in (Click to view all)</summary>
+<br>
+['Acamar', 'Achernar', 'Acrab', 'Acrux', 'Adhara', 'Aldebaran', 'Alderamin', 'Algieba', 'Algol', 'Alhena', 'Alioth', 'Alkaid', 'Almach', 'Alnair', 'Alnilam', 'Alnitak', 'Alphard', 'Alphecca', 'Alpheratz', 'Altair', 'Aludra', 'Ankaa', 'Antares', 'Arcturus', 'Arneb', 'Ascella', 'Aspidiske', 'Atria', 'Avior', 'Bellatrix', 'Beta Hydri', 'Beta Phoenicis', 'Betelgeuse', 'Canopus', 'Capella', 'Caph', 'Castor', 'Cebalrai', 'Celaeno', 'Chara', 'Cor-Caroli', 'Cursa', 'Delta Crucis', 'Delta Velorum', 'Deneb', 'Denebola', 'Diphda', 'Dschubba', 'Dubhe', 'Elnath', 'Eltanin', 'Enif', 'Formalhaut', 'Gacrux', 'Gamma Phoenicis', 'Gienah', 'Hadar', 'Hamal', 'Kaus Australis', 'Kochab', 'Kornephoros', 'Lesath', 'Markab', 'Megrez', 'Meissa', 'Menkalinan', 'Menkar', 'Menkent', 'Merak', 'Miaplacidus', 'Mimosa', 'Mintaka', 'Mirach', 'Mirfak', 'Mirzam', 'Mizar', 'Muphrid', 'Naos', 'Navi', 'Nunki', 'Peacock', 'Phact', 'Phecda', 'Polaris', 'Pollux', 'Procyon', 'Rasalhague', 'Rastaban', 'Regulus', 'Rigel', 'Ruchbah', 'Sabik', 'Sadr', 'Saiph', 'Sargas', 'Scheat', 'Schedar', 'Segin', 'Seginus', 'Shaula', 'Sheratan', 'Sirius', 'Spica', 'Suhail', 'Tarazed', 'Thuban', 'Tureis', 'Unukalhai', 'Vega', 'Wezen', 'Zosma', 'Zubeneschamali']
+</details>
+
+**Declination with Precession:**
+```python
+star_chart_spherical_projection.plotStarPositionOverTime(builtInStarName="Vega",
+							newStar=None,
+							startYearSince2000=-15000,
+							endYearSince2000=15000,
+							isPrecessionIncluded=True,
+							incrementYear=5,
+							DecOrRA="D")
+```
+![plot_star_declination_precession+png](https://raw.githubusercontent.com/cyschneck/Star-Chart-Spherical-Projection/main/examples/plot_star_vega_declination_with_precession.png) 
+**Declination without Precession:**
+```python
+star_chart_spherical_projection.plotStarPositionOverTime(builtInStarName="Vega",
+							newStar=None,
+							startYearSince2000=-15000,
+							endYearSince2000=15000,
+							isPrecessionIncluded=False,
+							incrementYear=5,
+							DecOrRA="D")
+```
+![plot_star_declination_without_prcession+png](https://raw.githubusercontent.com/cyschneck/Star-Chart-Spherical-Projection/main/examples/plot_star_vega_declination_without_precession.png) 
+**Right Ascension with Precession:**
+```python
+star_chart_spherical_projection.plotStarPositionOverTime(builtInStarName="Vega",
+							newStar=None,
+							startYearSince2000=-15000,
+							endYearSince2000=15000,
+							isPrecessionIncluded=True,
+							incrementYear=5,
+							DecOrRA="R")
+```
+![plot_star_RA_with_precession+png](https://raw.githubusercontent.com/cyschneck/Star-Chart-Spherical-Projection/main/examples/plot_star_vega_right_ascension_with_precession.png) 
+**Right Ascension without Precession:**
+```python
+star_chart_spherical_projection.plotStarPositionOverTime(builtInStarName="Vega",
+							newStar=None,
+							startYearSince2000=-15000,
+							endYearSince2000=15000,
+							isPrecessionIncluded=False,
+							incrementYear=5,
+							DecOrRA="R")
+```
+![plot_star_RA_without_precession+png](https://raw.githubusercontent.com/cyschneck/Star-Chart-Spherical-Projection/main/examples/plot_star_vega_right_ascension_without_precession.png) 
+
+# Star Chart Examples:
 __Star Chart in the Northern Hemisphere (centered on 90°) without Precession__
 ```
 star_chart_spherical_projection.plotStereographicProjection(northOrSouth="North",
 							displayStarNamesLabels=False,
 							yearSince2000=11500,
 							isPrecessionIncluded=False,
 							fig_plot_color="red")
@@ -341,57 +509,37 @@
 							displayStarNamesLabels=True,
 							yearSince2000=11500,
 							isPrecessionIncluded=True,
 							fig_plot_color="cornflowerblue")
 ```
 ![south_star_chart_with_labels_with_precession+png](https://raw.githubusercontent.com/cyschneck/Star-Chart-Spherical-Projection/main/examples/south_with_labels_with_precession.png) 
 
-## Return Final Position of Stars
-**finalPositionOfStars()**
+## Development Environment
+To run or test against `star-chart-spherical-projection` github repo/fork, a development environment can be created via conda/miniconda
+
+First, [install Miniconda](https://docs.conda.io/projects/miniconda/en/latest/miniconda-install.html)
+
+Then, using the existing `environment.yml`, a new conda environment can be create to run/test scripts against
 
-Returns a dictionary for the final positions of the stars in the format: {'Star Name': {"Declination" : Declination (int), "RA": RA (str)}
 ```
-finalPositionOfStars(builtInStars=[],
-		yearSince2000=0, 
-		isPrecessionIncluded=True,
-		userDefinedStars=[],
-		onlyDisplayUserStars=False,
-		declination_min=None,
-		declination_max=None,
-		save_to_csv=None)
+conda env create --file environment.yml
+```
+Once the environment has been built, activate the environment:
+```
+conda activate star_chart
+```
+To run existing and new tests from the root directory:
+```
+python -m pytest
 ```
-- *[OPTIONAL]* builtInStars: (list) a list of star names to include from built-in list, by default = [] includes all stars (in star_data.csv). Example: ["Vega", "Merak", "Dubhe"]
-- *[OPTIONAL]* yearSince2000: (int/float) years since 2000 (-50 = 1950 and +50 = 2050) to calculate proper motion and precession, defaults = 0 years
-- *[OPTIONAL]* isPrecessionIncluded: (boolean) when calculating star positions include predictions for precession, defaults to True
-- *[OPTIONAL]* userDefinedStars: (list) List of newStar objects of stars the user has added
-- *[OPTIONAL]* onlyDisplayUserStars: (bool) Only include the stars defined by the users (userDefinedStars)
-- *[OPTIONAL]* declination_min: (int/float) set minimum declination value, defaults to -30° in Northern hemisphere and 30° in Southern hemisphere
-- *[OPTIONAL]* declination_max: (int/float) set maximum declination value, defaults to 90° in Northern hemisphere and -90° in Southern hemisphere
-- *[OPTIONAL]* save_to_csv: (string) CSV filename and location to save final star positions with headers ["Star Name", "Right Ascension (HH.MM.SS)", "Declination (DD.SS)"]
-
-<details closed>
-<summary>Stars that will be included by default when builtInStars = [] (Click to view all)</summary>
-<br>
-['Acamar', 'Achernar', 'Acrab', 'Acrux', 'Adhara', 'Aldebaran', 'Alderamin', 'Algieba', 'Algol', 'Alhena', 
-'Alioth', 'Alkaid', 'Almach', 'Alnilam', 'Alnitak', 'Alphard', 'Alphecca', 'Alpheratz', 'Altair', 'Aludra', 
-'Ankaa', 'Antares', 'Arcturus', 'Arneb', 'Ascella', 'Aspidiske', 'Atria', 'Avior', 'Bellatrix', 'Beta Hydri', 
-'Beta Phoenicis', 'Betelgeuse', 'Canopus', 'Capella', 'Caph', 'Castor', 'Cebalrai', 'Celaeno', 'Chara', 
-'Cor-Caroli', 'Cursa', 'Delta Crucis', 'Deneb', 'Denebola', 'Diphda', 'Dschubba', 'Dubhe', 'Elnath', 'Eltanin', 
-'Enif', 'Formalhaut', 'Gacrux', 'Gamma Phoenicis', 'Gienah', 'Hadar', 'Hamal', 'Kochab', 'Kornephoros', 'Lesath', 
-'Markab', 'Megrez', 'Meissa', 'Menkalinan', 'Menkar', 'Menkent', 'Merak', 'Miaplacidus', 'Mimosa', 'Mintaka', 
-'Mirach', 'Mirfak', 'Mirzam', 'Mizar', 'Muphrid', 'Naos', 'Navi', 'Nunki', 'Peacock', 'Phact', 'Phecda', 'Polaris', 
-'Pollux', 'Procyon', 'Rasalhague', 'Rastaban', 'Regulus', 'Rigel', 'Ruchbah', 'Sabik', 'Sadr', 'Saiph', 'Sargas', 
-'Scheat', 'Schedar', 'Segin', 'Seginus', 'Shaula', 'Sheratan', 'Sirius', 'Spica', 'Suhail', 'Tarazed', 'Thuban', 
-'Unukalhai', 'Vega', 'Wezen', 'Zosma', 'Zubeneschamali']
-</details>
 
 ## Bibliography
 
-Star position (right ascension and declination) as well as the angle and speed of proper motion from [in-the-sky.org](https://in-the-sky.org/)
+Named stars specified by ["IAU Catalog of Star Names"](https://www.pas.rochester.edu/~emamajek/WGSN/IAU-CSN.txt) with the star position (right ascension and declination) as well as the angle and speed of proper motion from [in-the-sky.org](https://in-the-sky.org/) and Wikipedia where indicated
 
 Precession model: [Vondrák, J., et al. “New Precession Expressions, Valid for Long Time Intervals.” Astronomy &amp; Astrophysics, vol. 534, 2011](https://www.aanda.org/articles/aa/pdf/2011/10/aa17274-11.pdf)
 
-Preecession code adapted to Python 3+ from [Github Repo: vondrak](https://github.com/dreamalligator/vondrak)
+Precession code adapted to Python 3+ from [the Vondrak long term precession model Github repo 'vondrak')](https://github.com/dreamalligator/vondrak)
 
 ## Bug and Feature Request
 
 Submit a bug fix, question, or feature request as a [Github Issue](https://github.com/cyschneck/Star-Chart-Spherical-Projection/issues) or to cyschneck@gmail.com
```

### Comparing `star-chart-spherical-projection-1.5.0/setup.py` & `star-chart-spherical-projection-1.6.0/setup.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 # -*- coding: utf-8 -*-
 
 # Python Package Setup
 from setuptools import setup, find_namespace_packages
 
-VERSION="1.5.0"
+VERSION="1.6.0"
 DESCRIPTION="A Python package to generate circular astronomy star charts (past, present, and future) with spherical projection to correct for distortions with more than a hundred named stars accurate over 400,000 years with proper motion and precession of the equinoxes"
 
 with open("README.md", "r") as f:
 	long_description_readme = f.read()
 
 setup(
 	name="star-chart-spherical-projection",
@@ -23,28 +23,29 @@
 	classifiers=[
 		"Development Status :: 4 - Beta",
 		"Intended Audience :: Developers",
 		"Intended Audience :: Education",
 		"Intended Audience :: Science/Research",
 		"License :: OSI Approved :: MIT License",
 		"Programming Language :: Python",
-		"Programming Language :: Python :: 3.7",
-		"Programming Language :: Python :: 3.8",
 		"Programming Language :: Python :: 3.9",
+		"Programming Language :: Python :: 3.10",
+		"Programming Language :: Python :: 3.11",
+		"Programming Language :: Python :: 3.12",
 		"Intended Audience :: Education",
 		"Intended Audience :: Science/Research",
 		"Topic :: Scientific/Engineering :: Physics",
 		"Topic :: Scientific/Engineering :: Visualization",
 		"Topic :: Scientific/Engineering :: Astronomy"
 	],
 	packages=find_namespace_packages(include=['star_chart_spherical_projection',
 											'star_chart_spherical_projection.*']),
 	include_package_data=True,
 	install_requires=[
-		"configparser>=5.3.0",
-		"matplotlib>=3.1.0",
-		"numpy>=1.24.3",
-		"pandas>=1.3.5",
-		"pytest>=7.2.2"
+		"beautifulsoup4",
+		"matplotlib",
+		"numpy",
+		"pandas",
+		"pytest"
 	],
-	python_requires='>=3.7'
+	python_requires='>=3.9'
 )
```

### Comparing `star-chart-spherical-projection-1.5.0/star_chart_spherical_projection/data/convert_lst_to_csv_data.py` & `star-chart-spherical-projection-1.6.0/star_chart_spherical_projection/data/convert_lst_to_csv_data.py`

 * *Files 16% similar despite different names*

```diff
@@ -6,21 +6,40 @@
 logger.setLevel(logging.INFO)
 stream_handler = logging.StreamHandler()
 logger.addHandler(stream_handler)
 
 if __name__ == '__main__':
 	# stars: ["name", "RA: HH.MM.SS", Declination DD.SS, Proper Motion Speed (mas/yr), Proper Motion Angle (DD.SS), Magnitude (V, Visual)]
 	# Northern stars (+ declination)
+	absolutno_star = ["Absolutno", "07.46.51", 39.05, 32.17, 42.0, 12.13] #  Wiki: XO-5
+	achird_star = ["Achird", "00.49.06", 57.48, 1237.30, 292.31, 3.44] #  Wiki: Eta Cassiopeiae
+	acubens_star = ["Acubens", "08.58.29", 11.51, 52.44, 306.45, 4.20] #  Wiki: Acubens
+	adhafera_star = ["Adhafera", "10.16.41", 23.25, 19.62, 290.40, 3.33] #  Wiki: Zeta Leonis
+	adhil_star = ["Adhil", "01.22.20", 45.31, 32.94, 74.10, 4.90] #  Wiki: Xi Andromedae
+	ain_star = ["Ain", "04.28.37", 19.10, 113.46, 288.61, 3.53] #  Wiki: Epsilon Tauri
+	aladfar_star = ["Aladfar", "19.13.45", 39.09, 1.4, 25.46, -3.71] # Wiki: Eta Lyrae
+	albireo_star = ["Albireo", "19.30.45", 27.58, 6.24, 9.94, 5.11] # Wiki: Albireo B
+	alcor_star = ["Alcor", "13.25.13", 54.59, 121.3, 97.6, 3.99]
+	alcyone_star = ["Alcyone", "03.47.29", 24.06, 47.8, 156.1, 2.88]
 	aldebaran_star = ["Aldebaran", "04.35.55", 16.30, 199.3, 161.4, 0.99]
 	alderamin_star = ["Alderamin", "21.18.34", 62.35, 158.4, 71.9, 2.47]
+	aldhibah_star = ["Aldhibah", "17.08.47", 65.43, 28.32, 313.83, 3.17] # Wiki: Zeta Draconis
+	aldulfin_star = ["Aldulfin", "20.33.13", 11.18, 34.32, 337.57, 4.03] # Wiki: Epsilon Delphini
+	alfirk_star = ["Alfirk", "21.28.39", 70.33, 151.1, 56.2, 3.23]
 	algieba_star = ["Algieba", "10.19.58", 19.50, 341.2, 116.9, 2.23]
+	algenib_star = ["Algenib", "00.13.14", 15.11, 10.7, 177.4, 2.84]
 	algol_star = ["Algol", "03.08.10", 40.57, 3.4, 119.0, 2.11]
 	alhena_star = ["Alhena", "06.37.42", 16.24, 56.7, 165.9, 1.93]
 	alioth_star = ["Alioth", "12.54.01", 55.57, 112.2, 94.2, 1.76] # Big Dipper
+	aljanah_star = ["Aljanah", "20.46.13", 33.58, 485.58, 47.09, 2.48] # Wiki: Epsilon Cygni
 	alkaid_star = ["Alkaid", "13.47.32", 49.18, 122.1, 263.0, 1.86] # Big Dipper
+	alkalurops_star = ["Alkalurops", "15.24.29", 37.23, 174.65, 300.86, 4.31] # Wiki: Mu Bootis A
+	alkaphrah_star = ["Alkaphrah", "09.03.37", 47.09, 66.17, 33.15, 3.56] # Wiki: Kappa Ursae Majoris
+	alkarab_star = ["Alkarab", "24.25.23", 23.24, 195.55, 79.36, 4.4] # Wiki: Upsilon Pegasi
+	almaaz_star = ["Almaaz", "05.01.58", 43.49, 2.8, 17.92, 2.92] # Wiki: Epsilon Aurigae
 	almach_star = ["Almach", "02.03.53", 42.19, 65.0, 139.4, 2.17]
 	alphecca_star = ["Alphecca", "15.34.41", 26.42, 147.8, 126.4, 2.22]
 	alpheratz_star = ["Alpheratz", "00.08.23", 29.05, 213.6, 139.9, 2.06]
 	altair_star = ["Altair", "19.50.46", 8.52, 660.3, 54.3, 0.93]
 	arcturus_star = ["Arcturus", "14.15.39", 19.10, 2279.4, 208.7, 0.16]
 	barnards_star = ["Barnard's Star", "17.57.47", 4.44, 10393.3, 355.6, 9.6]
 	bellatrix_star = ["Bellatrix", "05.25.07", 6.20, 15.2, 212.2, 1.66]
@@ -75,15 +94,26 @@
 	#Southern stars (- declination)
 	# stars: ["name", "RA: HH.MM.SS", Declination, PM Speed, PM Angle, Magnitude (V, Visual)]
 	achernar_star = ["Achernar", "01.37.42", -57.14, 95.0, 113.7, 0.54]
 	acamar_star = ["Acamar", "02.58.15", -40.18, 57.1, 293.8, 3.22]
 	acrab_star = ["Acrab", "16.05.26", -19.48, 24.6, 192.2, 2.62]
 	acrux_star = ["Acrux", "12.26.35", -63.05, 38.8, 247.5, 1.28] # Southern Cross
 	adhara_star = ["Adhara", "06.58.37", -28.58, 3.5, 67.7, 1.53]
+	ainalrami_star = ["Ainalrami", "18.54.10", -22.44, 8.89, 331.14, 4.86] #  Wiki: Nu1 Sagittarii
+	alasia_star = ["Alasia", "18.21.49", -11.55, 17.15, 18.56, 4.78] # Wiki: HD 168746
+	albaldah_star = ["Albaldah", "19.09.45", -21.01, 36.48, 2.14, 2.89] # Wiki: Pi Sagittarii
+	albali_star = ["Albali", "20.47.40", -9.29, 48.62, 315.66, 2.89] # Wiki: Epsilon Aquarii
+	alchiba_star = ["Alchiba", "12.08.24", -24.43, 106.96, 291.49, 4.03] # Wiki: Alpha Corvi
+	aldhanab_star = ["Aldhanab", "21.53.55", -37.22, 98.96, 277.68, 3.003] # Wiki: Gamma Gruis
+	algedi_star = ["Algedi", "20.18.03", -12.32, 61.3, 87.7, 3.58]
+	algorab_star = ["Algorab", "12.29.51", -16.31, 251.3, 236.4, 2.97]
+	alkes_star = ["Alkes", "10.59.46", -18.18, 480.05, 285.65, 4.07] # Wiki: Alpha Crateris
 	alphard_star = ["Alphard", "09.27.35", -8.39, 37.6, 336.1, 1.98]
+	alnair_star = ["Alnair", "22.08.13", -46.57, 194.4, 139.3, -0.68]
+	alnasl_star = ["Alnasl", "18.05.48", -30.25, 188.8, 196.6, 2.96]
 	alnilam_star = ["Alnilam", "05.36.12", -1.12, 1.6, 118.4, 1.72]
 	alnitak_star = ["Alnitak", "05.40.45", -1.56, 3.8, 57.5, 1.90]
 	aludra_star = ["Aludra", "07.24.05", -29.18, 7.1, 324.5, 2.46]
 	ankaa_star = ["Ankaa", "00.26.17", -42.18, 425.7, 146.8, 2.38]
 	arneb_star = ["Arneb", "05.32.43", -17.49, 3.7, 66.2, 2.59]
 	ascella_star = ["Ascella", "19.02.36", -29.52, 23.7, 27.1, 2.61]
 	aspidiske_star = ["Aspidiske", "09.17.05", -59.16, 22.3, 302.4, 2.25]
@@ -91,21 +121,23 @@
 	avior_star = ["Avior", "08.22.30", -59.30, 33.7, 310.8, 1.95]
 	antares_star = ["Antares", "16.29.24", -26.25, 26.3, 207.5, 1.07]
 	beta_hydri_star = ["Beta Hydri", "00.25.45", -77.15, 2242.9, 81.6, 2.79]
 	beta_phoenicis_star = ["Beta Phoenicis", "01.06.05", -46.43, 88.1, 293.4, 3.37]
 	canopus_star = ["Canopus", "06.23.57", -51.41, 30.6, 40.6, -0.63]
 	cursa_star = ["Cursa", "05.07.51", -5.05, 112.0, 227.7, 2.79]
 	delta_crucis_star = ["Delta Crucis", "12.15.08", -58.44, 38.6, 253.0, 2.74] # Southern Cross
+	delta_velorum_star = ["Delta Velorum", "08.44.42", -54.42, 107.3, 164.3, -0.02]
 	diphda_star = ["Diphda", "00.43.35", -17.59, 234.7, 82.2, 2.05]
 	dschubba_star = ["Dschubba", "16.00.20", -22.37, 36.9, 196.1, 2.30]
 	formalhaut_star = ["Formalhaut", "22.57.38", -29.37, 367.9, 116.6, 1.23]
 	gacrux_star = ["Gacrux", "12.31.09", -57.06, 266.6, 173.9, 1.65] # Southern Cross
 	gamma_phoenicis_star = ["Gamma Phoenicis", "01.28.21", -43.19, 207.6, 184.9, 3.44]
 	gienah_star = ["Gienah", "12.15.48", -17.32, 160.1, 277.8, 2.59]
 	hadar_star = ["Hadar", "14.03.49", -60.22, 40.5, 235.2, 0.64]
+	kaus_australis_star = ["Kaus Australis", "18.24.10", -34.23, 130.3, 197.6, -1.40]
 	lesath_star = ["Lesath", "17.20.45", -37.17, 30.2, 184.5, 2.64]
 	meissa_star = ["Meissa", "05.35.08", -9.56, 3.0, 186.6, 3.53]
 	menkent_star = ["Menkent", "14.06.40", -36.22, 734.4, 225.1, 2.05]
 	miaplacidus_star = ["Miaplacidus", "09.13.12", -69.43, 190.7, 304.8, 1.67]
 	mintaka_star = ["Mintaka", "05.32.00", -0.18, 0.9, 137.2, 2.23]
 	mimosa_star = ["Mimosa", "12.47.43", -59.41, 45.9, 249.4, 1.31] # Southern Cross
 	mirzam_star = ["Mirzam", "06.22.41", -17.57, 3.3, 256.4, 1.96]
@@ -117,25 +149,45 @@
 	sabik_star = ["Sabik", "17.10.22", -15.43, 107.0, 22.0, 2.43]
 	sadalmelik_star = ["Sadalmelik", "22.05.47", -0.19, 21.3, 119.3, 2.93]
 	saiph_star = ["Saiph", "05.47.45", -9.4, 1.9, 131.2, 2.06]
 	sargas_star = ["Sargas", "17.37.19", -42.59, 6.4, 119.4, 1.86]
 	shaula_star = ["Shaula", "17.33.36", -37.06, 32.0, 195.5, 1.63]
 	sirius_star = ["Sirius", "06.45.08", -16.42, 1339.4, 204.1, -1.44]
 	suhail_star = ["Suhail", "09.07.59", -43.26, 27.6, 299.4, 2.20]
+	tureis_star = ["Tureis", "08.07.32", -24.18, 95.2, 299.5, 1.38]
 	wezen_star = ["Wezen", "07.08.23", -26.23, 4.5, 316.7, 1.84]
 	zubeneschamali_star = ["Zubeneschamali", "15.17.00", -9.22, 100.0, 258.7, 2.61]
 
 	# add stars to total star list
-	northern_star_chart_list = [aldebaran_star,
+	northern_star_chart_list = [absolutno_star,
+								achird_star,
+								acubens_star,
+								adhafera_star,
+								adhil_star,
+								ain_star,
+								aladfar_star,
+								albireo_star,
+								alcor_star,
+								alcyone_star,
+								aldebaran_star,
 								alderamin_star,
+								aldhibah_star,
+								aldulfin_star,
+								alfirk_star,
 								algieba_star,
+								algenib_star,
 								algol_star,
 								alhena_star,
 								alioth_star,
+								aljanah_star,
 								alkaid_star,
+								alkalurops_star,
+								alkaphrah_star,
+								alkarab_star,
+								almaaz_star,
 								almach_star,
 								alphecca_star,
 								alpheratz_star,
 								altair_star,
 								arcturus_star,
 								#barnards_star,
 								bellatrix_star,
@@ -189,15 +241,26 @@
 								]
 
 	southern_star_chart_list = [achernar_star,
 								acamar_star,
 								acrab_star,
 								acrux_star,
 								adhara_star,
+								ainalrami_star,
+								alasia_star,
+								albaldah_star,
+								albali_star,
+								alchiba_star,
+								aldhanab_star,
+								algedi_star,
+								algorab_star,
+								alkes_star,
 								alphard_star,
+								alnair_star,
+								alnasl_star,
 								alnilam_star,
 								alnitak_star,
 								aludra_star,
 								ankaa_star,
 								arneb_star,
 								ascella_star,
 								aspidiske_star,
@@ -205,21 +268,23 @@
 								avior_star,
 								antares_star,
 								beta_hydri_star,
 								beta_phoenicis_star,
 								canopus_star,
 								cursa_star,
 								delta_crucis_star,
+								delta_velorum_star,
 								diphda_star,
 								dschubba_star,
 								formalhaut_star,
 								gacrux_star,
 								gamma_phoenicis_star,
 								gienah_star,
 								hadar_star,
+								kaus_australis_star,
 								lesath_star,
 								meissa_star,
 								menkent_star,
 								miaplacidus_star,
 								mintaka_star,
 								mimosa_star,
 								mirzam_star,
@@ -230,22 +295,28 @@
 								rigel_star,
 								sabik_star,
 								saiph_star,
 								sargas_star,
 								shaula_star,
 								sirius_star,
 								suhail_star,
+								tureis_star,
 								wezen_star,
 								zubeneschamali_star
 								]
 
 	star_chart_list = northern_star_chart_list + southern_star_chart_list
-	logger.info("Total stars = {0}".format(len(star_chart_list)))
+	logger.info(f"Total stars = {len(star_chart_list)}")
 	for star in star_chart_list:
 		if len(star) != 6:
-			logger.info("ERROR: MISSING A VALUE = {0}".format(star[0])) # ensure that all stars have features
+			logger.info(f"ERROR: MISSING A VALUE = {star[0]}") # ensure that all stars have features
 			exit()
-	header_options = ["Star Name", "Right Ascension (HH.MM.SS)", "Declination (DD.SS)", "Proper Motion Speed (mas/yr)", "Proper Motion Angle (DD.SS)", "Magnitude (V, Visual)"]
+	header_options = ["Star Name",
+					"Right Ascension (HH.MM.SS)",
+					"Declination (DD.SS)",
+					"Proper Motion Speed (mas/yr)",
+					"Proper Motion Angle (DD.SS)",
+					"Magnitude (V, Visual)"]
 	df = pd.DataFrame(star_chart_list, columns=header_options)
 	df = df.sort_values(by=["Star Name"])
-	print(df)
+	print(df["Star Name"].tolist())
 	df.to_csv("star_data.csv", header=header_options, index=False)
```

### Comparing `star-chart-spherical-projection-1.5.0/star_chart_spherical_projection/data/star_data.csv` & `star-chart-spherical-projection-1.6.0/star_chart_spherical_projection/data/star_data.csv`

 * *Files 26% similar despite different names*

```diff
@@ -1,21 +1,51 @@
 Star Name,Right Ascension (HH.MM.SS),Declination (DD.SS),Proper Motion Speed (mas/yr),Proper Motion Angle (DD.SS),"Magnitude (V, Visual)"
+Absolutno,07.46.51,39.05,32.17,42.0,12.13
 Acamar,02.58.15,-40.18,57.1,293.8,3.22
 Achernar,01.37.42,-57.14,95.0,113.7,0.54
+Achird,00.49.06,57.48,1237.3,292.31,3.44
 Acrab,16.05.26,-19.48,24.6,192.2,2.62
 Acrux,12.26.35,-63.05,38.8,247.5,1.28
+Acubens,08.58.29,11.51,52.44,306.45,4.2
+Adhafera,10.16.41,23.25,19.62,290.4,3.33
 Adhara,06.58.37,-28.58,3.5,67.7,1.53
+Adhil,01.22.20,45.31,32.94,74.1,4.9
+Ain,04.28.37,19.1,113.46,288.61,3.53
+Ainalrami,18.54.10,-22.44,8.89,331.14,4.86
+Aladfar,19.13.45,39.09,1.4,25.46,-3.71
+Alasia,18.21.49,-11.55,17.15,18.56,4.78
+Albaldah,19.09.45,-21.01,36.48,2.14,2.89
+Albali,20.47.40,-9.29,48.62,315.66,2.89
+Albireo,19.30.45,27.58,6.24,9.94,5.11
+Alchiba,12.08.24,-24.43,106.96,291.49,4.03
+Alcor,13.25.13,54.59,121.3,97.6,3.99
+Alcyone,03.47.29,24.06,47.8,156.1,2.88
 Aldebaran,04.35.55,16.3,199.3,161.4,0.99
 Alderamin,21.18.34,62.35,158.4,71.9,2.47
+Aldhanab,21.53.55,-37.22,98.96,277.68,3.003
+Aldhibah,17.08.47,65.43,28.32,313.83,3.17
+Aldulfin,20.33.13,11.18,34.32,337.57,4.03
+Alfirk,21.28.39,70.33,151.1,56.2,3.23
+Algedi,20.18.03,-12.32,61.3,87.7,3.58
+Algenib,00.13.14,15.11,10.7,177.4,2.84
 Algieba,10.19.58,19.5,341.2,116.9,2.23
 Algol,03.08.10,40.57,3.4,119.0,2.11
+Algorab,12.29.51,-16.31,251.3,236.4,2.97
 Alhena,06.37.42,16.24,56.7,165.9,1.93
 Alioth,12.54.01,55.57,112.2,94.2,1.76
+Aljanah,20.46.13,33.58,485.58,47.09,2.48
 Alkaid,13.47.32,49.18,122.1,263.0,1.86
+Alkalurops,15.24.29,37.23,174.65,300.86,4.31
+Alkaphrah,09.03.37,47.09,66.17,33.15,3.56
+Alkarab,24.25.23,23.24,195.55,79.36,4.4
+Alkes,10.59.46,-18.18,480.05,285.65,4.07
+Almaaz,05.01.58,43.49,2.8,17.92,2.92
 Almach,02.03.53,42.19,65.0,139.4,2.17
+Alnair,22.08.13,-46.57,194.4,139.3,-0.68
+Alnasl,18.05.48,-30.25,188.8,196.6,2.96
 Alnilam,05.36.12,-1.12,1.6,118.4,1.72
 Alnitak,05.40.45,-1.56,3.8,57.5,1.9
 Alphard,09.27.35,-8.39,37.6,336.1,1.98
 Alphecca,15.34.41,26.42,147.8,126.4,2.22
 Alpheratz,00.08.23,29.05,213.6,139.9,2.06
 Altair,19.50.46,8.52,660.3,54.3,0.93
 Aludra,07.24.05,-29.18,7.1,324.5,2.46
@@ -37,28 +67,30 @@
 Castor,07.34.35,31.53,240.3,232.8,1.58
 Cebalrai,17.43.28,4.34,164.8,345.3,2.75
 Celaeno,03.44.48,24.17,49.2,156.2,5.45
 Chara,12.33.43,41.21,762.9,292.5,4.25
 Cor-Caroli,12.56.01,38.19,240.2,283.2,2.89
 Cursa,05.07.51,-5.05,112.0,227.7,2.79
 Delta Crucis,12.15.08,-58.44,38.6,253.0,2.74
+Delta Velorum,08.44.42,-54.42,107.3,164.3,-0.02
 Deneb,20.41.25,45.16,2.7,47.4,1.33
 Denebola,11.49.03,14.34,510.7,257.0,2.13
 Diphda,00.43.35,-17.59,234.7,82.2,2.05
 Dschubba,16.00.20,-22.37,36.9,196.1,2.3
 Dubhe,11.03.43,61.45,138.5,255.5,1.82
 Elnath,28.36.28,28.36,175.1,172.5,1.68
 Eltanin,17.56.36,51.29,24.3,200.4,2.23
 Enif,21.44.11,9.52,26.9,89.1,2.39
 Formalhaut,22.57.38,-29.37,367.9,116.6,1.23
 Gacrux,12.31.09,-57.06,266.6,173.9,1.65
 Gamma Phoenicis,01.28.21,-43.19,207.6,184.9,3.44
 Gienah,12.15.48,-17.32,160.1,277.8,2.59
 Hadar,14.03.49,-60.22,40.5,235.2,0.64
 Hamal,02.07.10,23.27,239.7,128.1,2.02
+Kaus Australis,18.24.10,-34.23,130.3,197.6,-1.4
 Kochab,14.50.42,74.09,34.6,289.3,2.06
 Kornephoros,16.30.13,21.29,99.9,261.4,2.78
 Lesath,17.20.45,-37.17,30.2,184.5,2.64
 Markab,23.04.45,15.12,73.2,124.4,2.49
 Megrez,12.15.25,57.01,104.3,85.5,3.3
 Meissa,05.35.08,-9.56,3.0,186.6,3.53
 Menkalinan,05.59.31,44.57,56.4,269.0,1.9
@@ -98,12 +130,13 @@
 Shaula,17.33.36,-37.06,32.0,195.5,1.63
 Sheratan,01.54.38,20.48,148.1,138.2,2.66
 Sirius,06.45.08,-16.42,1339.4,204.1,-1.44
 Spica,13.25.11,-11.09,52.3,234.1,1.06
 Suhail,09.07.59,-43.26,27.6,299.4,2.2
 Tarazed,19.46.15,10.36,16.3,94.8,2.69
 Thuban,14.04.23,64.22,58.9,287.0,3.65
+Tureis,08.07.32,-24.18,95.2,299.5,1.38
 Unukalhai,15.44.16,6.25,141.5,71.2,2.63
 Vega,18.36.56,38.47,349.7,35.1,0.03
 Wezen,07.08.23,-26.23,4.5,316.7,1.84
 Zosma,11.14.06,20.31,193.5,132.2,2.56
 Zubeneschamali,15.17.00,-9.22,100.0,258.7,2.61
```

### Comparing `star-chart-spherical-projection-1.5.0/star_chart_spherical_projection/declination_r_axis.py` & `star-chart-spherical-projection-1.6.0/star_chart_spherical_projection/declination_r_axis.py`

 * *Files identical despite different names*

### Comparing `star-chart-spherical-projection-1.5.0/star_chart_spherical_projection/generate_star_chart.py` & `star-chart-spherical-projection-1.6.0/star_chart_spherical_projection/generate_star_chart.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,13 +1,12 @@
 ########################################################################
 # Generate a star chart centered on the poles:
 #		Northern Hemsiphere = 90°
 #		Southern Hemsiphere = -90°
 ########################################################################
-import configparser
 import csv
 import logging
 import math
 import matplotlib.pyplot as plt
 import numpy as np
 import os
 import pandas as pd
@@ -17,16 +16,18 @@
 ## Logging set up
 logger = logging.getLogger(__name__)
 logger.setLevel(logging.INFO)
 stream_handler = logging.StreamHandler()
 logger.addHandler(stream_handler)
 
 ## Constants
-config = configparser.ConfigParser()
-config.read(os.path.join(os.path.dirname(__file__), 'config.ini'))
+northern_declination_min = -30
+northern_declination_max = 90
+southern_declination_min = 30
+southern_declination_max = -90
 
 # Start Year (JP2000)
 j2000 = 2000 # start year of the star catalogue (jan 1 2000 via IAU)
 
 def getStarList(selectStars=[]):
 	# generate a star object
 	# selectStars only returns a subset of all the stars saved, empty will return all in the star_data.csv file
@@ -58,15 +59,15 @@
 		star[1] = ra_in_radians
 	return star_list
 
 def convertRadianstoRAhr(ra_in_radians):
 	# change star in radians to RA in hours
 	ra_in_degree = np.rad2deg(ra_in_radians)
 
-	if ra_in_degree > 360 or ra_in_degree < 0: # lock degrees between 0 and 360, if negative, re-write as a postive degree
+	if ra_in_degree > 360 or ra_in_degree < 0: # lock degrees between 0 and 360, if negative, re-write as a positive degree
 		ra_in_degree %= 360
 
 	hours = int(ra_in_degree / 15)
 	minutes = int(((ra_in_degree / 15) - hours) * 60) # measured in minutes
 	seconds = round(((((ra_in_degree / 15) - hours) * 60) - minutes) * 60) # measured in seconds
 
 	# RA in hours 'HH.MM.SS'
@@ -93,43 +94,43 @@
 	logger.debug("(RA)  x Difference = {0} (rad) = {1} degrees".format(ra_x_difference_component, np.rad2deg(ra_x_difference_component)))
 	logger.debug("(DEC) y Difference = {0} (rad) = {1} degrees".format(dec_y_difference_component, np.rad2deg(dec_y_difference_component)))
 
 	star_adjusted_ra = star_ra + ra_x_difference_component # in radians with proper motion (potentionally will be flipped 180 based on new declination)
 	star_adjusted_declination = star_dec + np.rad2deg(dec_y_difference_component) # in degrees new with proper motion
 
 	dec_x = star_adjusted_declination
-	# remap within -90 and 90 for postive declinations
-	if star_adjusted_declination > 0: # Postive declinations
+	# remap within -90 and 90 for positive declinations
+	if star_adjusted_declination > 0: # Positive declinations
 		dec_x = star_adjusted_declination % 360
-		# map from 0 to 90 (postive declinations)
+		# map from 0 to 90 (positive declinations)
 		if dec_x > 90 and dec_x <= 180: 
 			dec_x = 90 + (90 - dec_x)
 		# map from 0 to -90 (negative declinations)
 		if dec_x <= 270 and dec_x > 180:
 			dec_x = 180 - dec_x
 		if dec_x < 360 and dec_x > 270:
 			dec_x = -90 + (dec_x - 270)
 	if star_adjusted_declination < -0: # Negative declinations
 		dec_x = star_adjusted_declination % -360
 		# map from 0 to -90 (negative declinations)
 		if dec_x < -90 and dec_x >= -180: 
 			dec_x = -90 - (90 + dec_x)
-		# map from 0 to 90 (postive declinations)
+		# map from 0 to 90 (positive declinations)
 		if dec_x >= -270 and dec_x <= -180:
 			dec_x = 180 + dec_x
 			dec_x = abs(dec_x)
 		if dec_x > -360 and dec_x < -270:
 			dec_x = 90 + (dec_x + 270)
 	logger.debug("New mapped dec = {0}".format(dec_x))
 	logger.debug("Original Dec = {0}, New Dec = {1}".format(star_dec, star_adjusted_declination))
 
 	# flip over RA by rotating 180
 	is_flipped_across_pole = False
 	star_over_ninety_ra = star_adjusted_declination
-	if star_over_ninety_ra >= 0: # postive declinations
+	if star_over_ninety_ra >= 0: # positive declinations
 		while (star_over_ninety_ra > 90):
 			star_over_ninety_ra -= 90
 			is_flipped_across_pole = not is_flipped_across_pole # flip across the center by 180
 	if star_over_ninety_ra < 0: # negative declinations
 		while (star_over_ninety_ra < -90):
 			star_over_ninety_ra += 90
 			is_flipped_across_pole = not is_flipped_across_pole # flip across the center by 180
@@ -160,101 +161,39 @@
 	final_ra_due_to_precession = original_ra + change_in_ra
 
 	logger.debug("Dec: {0} + {1} = {2}".format(original_declination, change_in_declination, final_declination_due_to_precession))
 	logger.debug("RA:  {0} + {1} = {2}".format(original_ra, change_in_ra, final_ra_due_to_precession))
 	return final_ra_due_to_precession, final_declination_due_to_precession
 
 def vondrakDreamalligator(star_name, star_ra_rad, star_dec_rad, year_to_calculate):
-	# Modified code from github.com/dreamalligator/vondrak
+	# Modified code from github.com/dreamalligator/vondrak to calculate precession
 	def position_matrix(ra=None, dec=None):
 		x = math.cos(dec) * math.cos(ra)
 		y = math.cos(dec) * math.sin(ra)
 		z = math.sin(dec)
 		return np.array([[x], [y], [z]])
 
 	def compute_star(compute_ra, compute_dec):
-		return position_matrix(ra = compute_ra, dec = compute_dec)
+		return position_matrix(ra=compute_ra, dec=compute_dec)
 
-	P = star_chart_spherical_projection.ltp_pbmat(year_to_calculate) # Precession matrix for the given year
+	precession_matrix = star_chart_spherical_projection.ltp_pbmat(year_to_calculate) # Precession matrix for the given year
 	p_1 = compute_star(star_ra_rad, star_dec_rad) # compute star's position matrix for given year
-	p_1 = star_chart_spherical_projection.pdp(P, p_1) # apply precession matrix for given year
+	p_1 = star_chart_spherical_projection.pdp(precession_matrix, p_1) # apply precession matrix for given year
 	(ra_as_rad, dec_as_rad) = star_chart_spherical_projection.ra_dec(p_1)
+
 	return dec_as_rad, ra_as_rad # new declination and right ascension
 
 def precessionVondrak(star_name, star_ra, star_dec, year_YYYY_since_2000):
 	# Temporary fix for vondrak plugin (will only find a smaller subsections of the stars)
 	logger.debug("INCLUDING PRECESSION VIA VONDRAK")
 	vondrak_dec, vondrak_ra = vondrakDreamalligator(star_name, star_ra, np.deg2rad(star_dec), 2000 + year_YYYY_since_2000)
 	vondrak_dec = np.rad2deg(vondrak_dec)
 	logger.debug("Precession for Star = {0}, Declination = {1}, RA = {2}".format(star_name, vondrak_dec, vondrak_ra))
 	return vondrak_dec, vondrak_ra
 
-def finalPositionOfStars(builtInStars=[], 
-						yearSince2000=0,
-						isPrecessionIncluded=True,
-						userDefinedStars=[],
-						onlyDisplayUserStars=False,
-						declination_min=None,
-						declination_max=None,
-						save_to_csv=None):
-	# return the final position of the stars as a dictionary
-
-	star_chart_spherical_projection.errorHandling(isPlotFunction=False,
-												builtInStars=builtInStars,
-												yearSince2000=yearSince2000,
-												isPrecessionIncluded=isPrecessionIncluded,
-												userDefinedStars=userDefinedStars,
-												onlyDisplayUserStars=onlyDisplayUserStars,
-												declination_min=declination_min,
-												declination_max=declination_max,
-												save_to_csv=save_to_csv)
-	if not onlyDisplayUserStars:
-		builtInStars = [x.title() for x in builtInStars] # convert all names to capitalized
-		listOfStars = getStarList(builtInStars)
-		for star_object in userDefinedStars:
-			star_row = [star_object.starName,
-						star_object.ra,
-						star_object.dec,
-						star_object.properMotionSpeed,
-						star_object.properMotionAngle,
-						star_object.magnitudeVisual]
-			listOfStars.append(star_row)
-	else:
-		listOfStars = []
-		for star_object in userDefinedStars:
-			star_row = [star_object.starName,
-						star_object.ra,
-						star_object.dec,
-						star_object.properMotionSpeed,
-						star_object.properMotionAngle,
-						star_object.magnitudeVisual]
-			listOfStars.append(star_row)
-	
-	# Set declination min values when using the generateStereographicProjection() to capture all stars if not set
-	declination_min = -90
-	declination_max = 90
-
-	x_star_labels, x_ra_values, y_dec_values, finalPositionOfStarsDict = generateStereographicProjection(starList=listOfStars, 
-																										northOrSouth="North", 
-																										declination_min=declination_min,
-																										yearSince2000=yearSince2000,
-																										isPrecessionIncluded=isPrecessionIncluded,
-																										maxMagnitudeFilter=None,
-																										declination_max=declination_max)
-	# Generate a .csv file with final positions of stars
-	if save_to_csv is not None:
-		header_options = ["Star Name", "Right Ascension (HH.MM.SS)", "Declination (DD.SS)"]
-		star_chart_list = []
-		for star_name, star_position in finalPositionOfStarsDict.items():
-			star_chart_list.append([star_name, star_position["RA"], star_position["Declination"]])
-		df = pd.DataFrame(star_chart_list, columns=header_options)
-		df = df.sort_values(by=["Star Name"])
-		df.to_csv(save_to_csv, header=header_options, index=False)
-	return finalPositionOfStarsDict
-
 def generateStereographicProjection(starList=None, 
 									northOrSouth=None, 
 									yearSince2000=None,
 									isPrecessionIncluded=None,
 									maxMagnitudeFilter=None,
 									declination_min=None,
 									declination_max=None):
@@ -380,22 +319,23 @@
 			star_row = [star_object.starName,
 						star_object.ra,
 						star_object.dec,
 						star_object.properMotionSpeed,
 						star_object.properMotionAngle,
 						star_object.magnitudeVisual]
 			listOfStars.append(star_row)
+
 	# plot star chart as a circular graph
 
 	# Set declination based on hemisphere selected
 	if declination_min is None:
-		if northOrSouth == "North": declination_min = int(config["declinationDefaultValues"]["northern_declination_min"])
-		if northOrSouth == "South": declination_min = int(config["declinationDefaultValues"]["southern_declination_min"])
-	if northOrSouth == "North": declination_max = int(config["declinationDefaultValues"]["northern_declination_max"])
-	if northOrSouth == "South": declination_max = int(config["declinationDefaultValues"]["southern_declination_max"])
+		if northOrSouth == "North": declination_min = northern_declination_min
+		if northOrSouth == "South": declination_min = southern_declination_min
+	if northOrSouth == "North": declination_max = northern_declination_max
+	if northOrSouth == "South": declination_max = southern_declination_max
 
 	# Polar plot figure
 	fig = plt.figure(figsize=(figsize_n,figsize_n), dpi=figsize_dpi)
 	ax = fig.subplots(subplot_kw={'projection': 'polar'})
 
 	# Set Declination (astronomical 'latitude') as Y (radius of polar plot)
 
@@ -425,17 +365,17 @@
 		else:
 			plt.yticks(ruler_declination_position, fontsize=0) # do not display axis
 			ax.set_yticklabels(ruler_declination_labels)
 			ax.set_rlabel_position(120) # declination labels position
 
 	# Display declination lines based on hemisphere
 	if northOrSouth == "North":
-		displayDeclinationMarksOnAxis(declination_values, int(config["declinationDefaultValues"]["northern_declination_min"]), int(config["declinationDefaultValues"]["northern_declination_max"]), False)
+		displayDeclinationMarksOnAxis(declination_values, northern_declination_min, northern_declination_max, False)
 	if northOrSouth == "South":
-		displayDeclinationMarksOnAxis(declination_values, int(config["declinationDefaultValues"]["southern_declination_min"]), int(config["declinationDefaultValues"]["southern_declination_max"]), True)
+		displayDeclinationMarksOnAxis(declination_values, southern_declination_min, southern_declination_max, True)
 
 	logger.debug("\n{0}ern Range of Declination: {1} to {2}".format(northOrSouth, declination_min, declination_max))
 
 	# convert to x and y values for stars
 	x_star_labels, x_ra_values, y_dec_values, star_dict = generateStereographicProjection(starList=listOfStars, 
 																						northOrSouth=northOrSouth, 
 																						yearSince2000=yearSince2000,
@@ -452,15 +392,15 @@
 	labels_ra = np.array(['$0^h$','$1^h$','$2^h$','$3^h$', '$4^h$','$5^h$',
 						'$6^h$','$7^h$', '$8^h$','$9^h$', '$10^h$',
 						'$11^h$','$12^h$','$13^h$','$14^h$','$15^h$',
 						'$16^h$','$17^h$','$18^h$','$19^h$','$20^h$', 
 						'$21^h$', '$22^h$','$23^h$'])
 	ax.set_xticklabels(labels_ra, fontsize=10)
 
-	# Optiona: Label the stars with names
+	# Optional: Label the stars with names
 	if displayStarNamesLabels:
 		for i, txt in enumerate(x_star_labels):
 			ax.annotate(txt, (x_ra_values[i], y_dec_values[i]), 
 						horizontalalignment='center', verticalalignment='bottom', 
 						fontsize=8)
 	for i, txt in enumerate(x_star_labels):
 		logger.debug("{0}: {1:05f} RA (degrees) and {2:05f} Declination (ruler)".format(txt, np.rad2deg(x_ra_values[i]), y_dec_values[i]))
@@ -474,15 +414,15 @@
 	suffix = ""
 	if 1000 <  abs(years_for_title) and abs(years_for_title) < 1000000:
 		years_for_title = years_for_title / 1000
 		suffix = "K"
 	if abs(years_for_title) > 1000000:
 		years_for_title = years_for_title / 1000000
 		suffix = "M"
-	if yearSince2000 >= -2000: year_bce_ce = "{0} C.E".format(yearSince2000 + 2000) # postive years for C.E
+	if yearSince2000 >= -2000: year_bce_ce = "{0} C.E".format(yearSince2000 + 2000) # positive years for C.E
 	if yearSince2000 < -2000: year_bce_ce = "{0} B.C.E".format(abs(yearSince2000 + 2000)) # negative years for B.C.E
 	figure_has_precession_extra_string = "with Precession" if isPrecessionIncluded else "without Precession"
 
 	if fig_plot_title is None: # by default sets title of plot
 		ax.set_title("{0}ern Hemisphere [{1}{2} Years Since 2000 ({3})]: {4}° to {5}° {6}".format(northOrSouth,
 																								years_for_title,
 																								suffix,
```

### Comparing `star-chart-spherical-projection-1.5.0/star_chart_spherical_projection/pytests/test_finalPositionOfStars.py` & `star-chart-spherical-projection-1.6.0/star_chart_spherical_projection/pytests/test_errorPlotStereographicProjection.py`

 * *Files 27% similar despite different names*

```diff
@@ -1,13 +1,15 @@
-# Pytest for finalPositionOfStars()
-# centerline-width/: python3 -m pytest -v
-import logging
+# Pytest for plotStereographicProjection()
+# star_chart_spherical_projection/: python3 -m pytest -v
+import re
+import os
 
 # External Python libraries (installed via pip install)
 import pytest
+import pandas as pd
 
 # Internal star_chart_spherical_projection reference to access functions, global variables, and error handling
 import star_chart_spherical_projection as scsp
 
 invalid_non_str_options = [(1961, "<class 'int'>"),
 						(3.1415, "<class 'float'>"),
 						([], "<class 'list'>"),
@@ -28,118 +30,117 @@
 						(3.1415, "<class 'float'>"),
 						(False, "<class 'bool'>")]
 
 invalid_non_num_options = [([], "<class 'list'>"),
 						("string", "<class 'str'>"),
 						(False, "<class 'bool'>")]
 
+filepath_one_level_above = os.path.dirname(os.path.dirname(__file__))
+star_csv_file = os.path.join(filepath_one_level_above, 'data', 'star_data.csv')  # get file's directory, up one level, /data/star_data.csv
+star_dataframe = pd.read_csv(star_csv_file)
+star_dataframe = star_dataframe.sort_values(by=["Star Name"])
+lst_of_current_stars = star_dataframe["Star Name"].tolist()
+
+def test_plotStereographicProjection_northOrSouthInvalidOptions():
+	with pytest.raises(ValueError, match=re.escape("[northOrSouth]: Hemisphere options are ['North', 'South'], current option = 'Invalid'")):
+		scsp.plotStereographicProjection(northOrSouth="Invalid")
+
+@pytest.mark.parametrize("invalid_input, error_output", invalid_non_str_options)
+def test_plotStereographicProjection_northOrSouthInvalidTypes(invalid_input, error_output):
+	with pytest.raises(ValueError, match=re.escape(f"[northOrSouth]: Must be a str, current type = '{error_output}'")):
+		scsp.plotStereographicProjection(northOrSouth=invalid_input)
+
 @pytest.mark.parametrize("invalid_input, error_output", invalid_non_list_options)
-def test_finalPositionOfStars_builtInStarsInvalidTypes(caplog, invalid_input, error_output):
-	# Test:
-	with pytest.raises(SystemExit):
-		scsp.finalPositionOfStars(builtInStars=invalid_input)
-	log_record = caplog.records[0]
-	assert log_record.levelno == logging.CRITICAL
-	assert log_record.message == "\nCRITICAL ERROR, [builtInStars]: Must be a list, current type = '{0}'".format(error_output)
-
-def test_finalPositionOfStars_builtInStarsInvalidStar(caplog):
-	# Test:
-	with pytest.raises(SystemExit):
-		scsp.finalPositionOfStars(builtInStars=["Fake star", "VEga"])
-	log_record = caplog.records[0]
-	assert log_record.levelno == logging.CRITICAL
-	assert log_record.message == "\nCRITICAL ERROR, [builtInStars]: 'Fake Star' not a star in current list of stars, please select one of the following: ['Acamar', 'Achernar', 'Acrab', 'Acrux', 'Adhara', 'Aldebaran', 'Alderamin', 'Algieba', 'Algol', 'Alhena', 'Alioth', 'Alkaid', 'Almach', 'Alnilam', 'Alnitak', 'Alphard', 'Alphecca', 'Alpheratz', 'Altair', 'Aludra', 'Ankaa', 'Antares', 'Arcturus', 'Arneb', 'Ascella', 'Aspidiske', 'Atria', 'Avior', 'Bellatrix', 'Beta Hydri', 'Beta Phoenicis', 'Betelgeuse', 'Canopus', 'Capella', 'Caph', 'Castor', 'Cebalrai', 'Celaeno', 'Chara', 'Cor-Caroli', 'Cursa', 'Delta Crucis', 'Deneb', 'Denebola', 'Diphda', 'Dschubba', 'Dubhe', 'Elnath', 'Eltanin', 'Enif', 'Formalhaut', 'Gacrux', 'Gamma Phoenicis', 'Gienah', 'Hadar', 'Hamal', 'Kochab', 'Kornephoros', 'Lesath', 'Markab', 'Megrez', 'Meissa', 'Menkalinan', 'Menkar', 'Menkent', 'Merak', 'Miaplacidus', 'Mimosa', 'Mintaka', 'Mirach', 'Mirfak', 'Mirzam', 'Mizar', 'Muphrid', 'Naos', 'Navi', 'Nunki', 'Peacock', 'Phact', 'Phecda', 'Polaris', 'Pollux', 'Procyon', 'Rasalhague', 'Rastaban', 'Regulus', 'Rigel', 'Ruchbah', 'Sabik', 'Sadr', 'Saiph', 'Sargas', 'Scheat', 'Schedar', 'Segin', 'Seginus', 'Shaula', 'Sheratan', 'Sirius', 'Spica', 'Suhail', 'Tarazed', 'Thuban', 'Unukalhai', 'Vega', 'Wezen', 'Zosma', 'Zubeneschamali']"
-
-@pytest.mark.parametrize("invalid_input, error_output", invalid_non_num_options)
-def test_finalPositionOfStars_declinationMinInvalidTypes(caplog, invalid_input, error_output):
-	# Test:
-	with pytest.raises(SystemExit):
-		scsp.finalPositionOfStars(declination_min=invalid_input)
-	log_record = caplog.records[0]
-	assert log_record.levelno == logging.CRITICAL
-	assert log_record.message == "\nCRITICAL ERROR, [declination_min]: Must be a int or float, current type = '{0}'".format(error_output)
-
-def test_finalPositionOfStars_declinationMinInvalidRangeMin(caplog):
-	# Test:
-	with pytest.raises(SystemExit):
-		scsp.finalPositionOfStars(declination_min=-90)
-	log_record = caplog.records[0]
-	assert log_record.levelno == logging.CRITICAL
-	assert log_record.message == "\nCRITICAL ERROR, [declination_min]: Minimum declination must lie between -90 and +90 (-89 to 89) [recommended by default: north=-30, south=30], current minimum = '-90'"
-
-def test_finalPositionOfStars_declinationMinInvalidRangeMax(caplog):
-	# Test:
-	with pytest.raises(SystemExit):
-		scsp.finalPositionOfStars(declination_min=90)
-	log_record = caplog.records[0]
-	assert log_record.levelno == logging.CRITICAL
-	assert log_record.message == "\nCRITICAL ERROR, [declination_min]: Minimum declination must lie between -90 and +90 (-89 to 89) [recommended by default: north=-30, south=30], current minimum = '90'"
-
-@pytest.mark.parametrize("invalid_input, error_output", invalid_non_num_options)
-def test_finalPositionOfStars_declinationMaxInvalidTypes(caplog, invalid_input, error_output):
-	# Test:
-	with pytest.raises(SystemExit):
-		scsp.finalPositionOfStars(declination_max=invalid_input)
-	log_record = caplog.records[0]
-	assert log_record.levelno == logging.CRITICAL
-	assert log_record.message == "\nCRITICAL ERROR, [declination_max]: Must be a int or float, current type = '{0}'".format(error_output)
-
-def test_finalPositionOfStars_declinationMaxInvalidRangeMin(caplog):
-	# Test:
-	with pytest.raises(SystemExit):
-		scsp.finalPositionOfStars(declination_max=-90)
-	log_record = caplog.records[0]
-	assert log_record.levelno == logging.CRITICAL
-	assert log_record.message == "\nCRITICAL ERROR, [declination_max]: Maximum declination must lie between -90 and +90 (-89 to 89) [recommended by default: north=-30, south=30], current minimum = '-90'"
-
-def test_finalPositionOfStars_declinationMaxInvalidRangeMax(caplog):
-	# Test:
-	with pytest.raises(SystemExit):
-		scsp.finalPositionOfStars(declination_max=90)
-	log_record = caplog.records[0]
-	assert log_record.levelno == logging.CRITICAL
-	assert log_record.message == "\nCRITICAL ERROR, [declination_max]: Maximum declination must lie between -90 and +90 (-89 to 89) [recommended by default: north=-30, south=30], current minimum = '90'"
-
-@pytest.mark.parametrize("invalid_input, error_output", invalid_non_num_options)
-def test_finalPositionOfStars_yearSince2000InvalidTypes(caplog, invalid_input, error_output):
-	# Test:
-	with pytest.raises(SystemExit):
-		scsp.finalPositionOfStars(yearSince2000=invalid_input)
-	log_record = caplog.records[0]
-	assert log_record.levelno == logging.CRITICAL
-	assert log_record.message == "\nCRITICAL ERROR, [yearSince2000]: Must be a int or float, current type = '{0}'".format(error_output)
+def test_plotStereographicProjection_builtInStarsInvalidTypes(invalid_input, error_output):
+	with pytest.raises(ValueError, match=re.escape(f"[builtInStars]: Must be a list, current type = '{error_output}'")):
+		scsp.plotStereographicProjection(northOrSouth="North", builtInStars=invalid_input)
+
+def test_plotStereographicProjection_builtInStarsInvalidStar():
+	with pytest.raises(ValueError, match=re.escape(f"[builtInStars]: 'Fake Star' not a star in current list of stars, please select one of the following: {lst_of_current_stars}")):
+		scsp.plotStereographicProjection(northOrSouth="North", builtInStars=["Fake star", "VEga"])
+
+@pytest.mark.parametrize("invalid_input, error_output", invalid_non_num_options)
+def test_plotStereographicProjection_declinationMinInvalidTypes(invalid_input, error_output):
+	with pytest.raises(ValueError, match=re.escape(f"[declination_min]: Must be a int or float, current type = '{error_output}'")):
+		scsp.plotStereographicProjection(northOrSouth="North", declination_min=invalid_input)
+
+def test_plotStereographicProjection_declinationMinInvalidRangeMin():
+	with pytest.raises(ValueError, match=re.escape("[declination_min]: Minimum declination must lie between -90 and +90 (-89 to 89) [recommended by default: north=-30, south=30], current minimum = '-90'")):
+		scsp.plotStereographicProjection(northOrSouth="North", declination_min=-90)
+
+def test_plotStereographicProjection_declinationMinInvalidRangeMax():
+	with pytest.raises(ValueError, match=re.escape("[declination_min]: Minimum declination must lie between -90 and +90 (-89 to 89) [recommended by default: north=-30, south=30], current minimum = '90'")):
+		scsp.plotStereographicProjection(northOrSouth="North", declination_min=90)
+
+@pytest.mark.parametrize("invalid_input, error_output", invalid_non_num_options)
+def test_plotStereographicProjection_yearSince2000InvalidTypes(invalid_input, error_output):
+	with pytest.raises(ValueError, match=re.escape(f"[yearSince2000]: Must be a int or float, current type = '{error_output}'")):
+		scsp.plotStereographicProjection(northOrSouth="North", yearSince2000=invalid_input)
 
 @pytest.mark.parametrize("invalid_input, error_output", invalid_non_bool_options)
-def test_finalPositionOfStars_isPrecessionIncludedInvalidTypes(caplog, invalid_input, error_output):
-	# Test:
-	with pytest.raises(SystemExit):
-		scsp.finalPositionOfStars(isPrecessionIncluded=invalid_input)
-	log_record = caplog.records[0]
-	assert log_record.levelno == logging.CRITICAL
-	assert log_record.message == "\nCRITICAL ERROR, [isPrecessionIncluded]: Must be a bool, current type = '{0}'".format(error_output)
-
-@pytest.mark.parametrize("invalid_input, error_output", invalid_non_num_options)
-def test_finalPositionOfStars_userDefinedStarsInvalidTypes(caplog, invalid_input, error_output):
-	# Test:
-	with pytest.raises(SystemExit):
-		scsp.finalPositionOfStars(userDefinedStars=[invalid_input])
-	log_record = caplog.records[0]
-	assert log_record.levelno == logging.CRITICAL
-	assert log_record.message == "\nCRITICAL ERROR, [userDefinedStars]: {0} is not a valid newStar object (see: star_chart_spherical_projection.newStar)".format(error_output)
+def test_plotStereographicProjection_displayStarNamesLabelsInvalidTypes(invalid_input, error_output):
+	with pytest.raises(ValueError, match=re.escape(f"[displayStarNamesLabels]: Must be a bool, current type = '{error_output}'")):
+		scsp.plotStereographicProjection(northOrSouth="North", displayStarNamesLabels=invalid_input)
+
+@pytest.mark.parametrize("invalid_input, error_output", invalid_non_bool_options)
+def test_plotStereographicProjection_displayDeclinationNumbersInvalidTypes(invalid_input, error_output):
+	with pytest.raises(ValueError, match=re.escape(f"[displayDeclinationNumbers]: Must be a bool, current type = '{error_output}'")):
+		scsp.plotStereographicProjection(northOrSouth="North", displayDeclinationNumbers=invalid_input)
+
+def test_plotStereographicProjection_incrementByInvalidOptions():
+	with pytest.raises(ValueError, match=re.escape("[incrementBy]: Must be one of the options [1, 5, 10], current value = '2'")):
+		scsp.plotStereographicProjection(northOrSouth="North", incrementBy=2)
+
+@pytest.mark.parametrize("invalid_input, error_output", invalid_non_int_options)
+def test_plotStereographicProjection_incrementByInvalidTypes(invalid_input, error_output):
+	with pytest.raises(ValueError, match=re.escape(f"[incrementBy]: Must be a int, current type = '{error_output}'")):
+		scsp.plotStereographicProjection(northOrSouth="North", incrementBy=invalid_input)
+
+@pytest.mark.parametrize("invalid_input, error_output", invalid_non_bool_options)
+def test_plotStereographicProjection_isPrecessionIncludedInvalidTypes(invalid_input, error_output):
+	with pytest.raises(ValueError, match=re.escape(f"[isPrecessionIncluded]: Must be a bool, current type = '{error_output}'")):
+		scsp.plotStereographicProjection(northOrSouth="North", isPrecessionIncluded=invalid_input)
+
+@pytest.mark.parametrize("invalid_input, error_output", invalid_non_num_options)
+def test_plotStereographicProjection_maxMagnitudeFilterInvalidTypes(invalid_input, error_output):
+	with pytest.raises(ValueError, match=re.escape(f"[maxMagnitudeFilter]: Must be a int or float, current type = '{error_output}'")):
+		scsp.plotStereographicProjection(northOrSouth="North", maxMagnitudeFilter=invalid_input)
 
 @pytest.mark.parametrize("invalid_input, error_output", invalid_non_bool_options)
-def test_finalPositionOfStars_onlyDisplayUserStarsInvalidTypes(caplog, invalid_input, error_output):
-	# Test:
-	with pytest.raises(SystemExit):
-		scsp.finalPositionOfStars(onlyDisplayUserStars=invalid_input)
-	log_record = caplog.records[0]
-	assert log_record.levelno == logging.CRITICAL
-	assert log_record.message == "\nCRITICAL ERROR, [onlyDisplayUserStars]: Must be a bool, current type = '{0}'".format(error_output)
+def test_plotStereographicProjection_showPlotInvalidTypes(invalid_input, error_output):
+	with pytest.raises(ValueError, match=re.escape(f"[showPlot]: Must be a bool, current type = '{error_output}'")):
+		scsp.plotStereographicProjection(northOrSouth="North", showPlot=invalid_input)
 
 @pytest.mark.parametrize("invalid_input, error_output", invalid_non_str_options)
-def test_finalPositionOfStars_saveToCsvInvalidTypes(caplog, invalid_input, error_output):
-	# Test:
-	with pytest.raises(SystemExit):
-		scsp.finalPositionOfStars(save_to_csv=invalid_input)
-	log_record = caplog.records[0]
-	assert log_record.levelno == logging.CRITICAL
-	assert log_record.message == "\nCRITICAL ERROR, [save_to_csv]: Must be a str, current type = '{0}'".format(error_output)
+def test_plotStereographicProjection_figPlotTitleInvalidTypes(invalid_input, error_output):
+	with pytest.raises(ValueError, match=re.escape(f"[fig_plot_title]: Must be a string, current type = '{error_output}'")):
+		scsp.plotStereographicProjection(northOrSouth="North", fig_plot_title=invalid_input)
+
+@pytest.mark.parametrize("invalid_input, error_output", invalid_non_str_options)
+def test_plotStereographicProjection_figPlotColorInvalidTypes(invalid_input, error_output):
+	with pytest.raises(ValueError, match=re.escape(f"[fig_plot_color]: Must be a string, current type = '{error_output}'")):
+		scsp.plotStereographicProjection(northOrSouth="North", fig_plot_color=invalid_input)
+
+@pytest.mark.parametrize("invalid_input, error_output", invalid_non_num_options)
+def test_plotStereographicProjection_figsizeNInvalidTypes(invalid_input, error_output):
+	with pytest.raises(ValueError, match=re.escape(f"[figsize_n]: Must be a int or float, current type = '{error_output}'")):
+		scsp.plotStereographicProjection(northOrSouth="North", figsize_n=invalid_input)
+
+@pytest.mark.parametrize("invalid_input, error_output", invalid_non_num_options)
+def test_plotStereographicProjection_figsizeDPIInvalidTypes(invalid_input, error_output):
+	with pytest.raises(ValueError, match=re.escape(f"[figsize_dpi]: Must be a int or float, current type = '{error_output}'")):
+		scsp.plotStereographicProjection(northOrSouth="North", figsize_dpi=invalid_input)
+
+@pytest.mark.parametrize("invalid_input, error_output", invalid_non_str_options)
+def test_plotStereographicProjection_savePlotNameInvalidTypes(invalid_input, error_output):
+	with pytest.raises(ValueError, match=re.escape(f"[save_plot_name]: Must be a string, current type = '{error_output}'")):
+		scsp.plotStereographicProjection(northOrSouth="North", save_plot_name=invalid_input)
+
+@pytest.mark.parametrize("invalid_input, error_output", invalid_non_num_options)
+def test_plotStereographicProjection_userDefinedStarsInvalidTypes(invalid_input, error_output):
+	with pytest.raises(ValueError, match=re.escape(f"[userDefinedStars]: {error_output} is not a valid newStar object (see: star_chart_spherical_projection.newStar)")):
+		scsp.plotStereographicProjection(northOrSouth="North", userDefinedStars=[invalid_input])
+
+@pytest.mark.parametrize("invalid_input, error_output", invalid_non_bool_options)
+def test_plotStereographicProjection_onlyDisplayUserStarsInvalidTypes(invalid_input, error_output):
+	with pytest.raises(ValueError, match=re.escape(f"[onlyDisplayUserStars]: Must be a bool, current type = '{error_output}'")):
+		scsp.plotStereographicProjection(northOrSouth="North", onlyDisplayUserStars=invalid_input)
```

### Comparing `star-chart-spherical-projection-1.5.0/star_chart_spherical_projection/pytests/test_starClass.py` & `star-chart-spherical-projection-1.6.0/star_chart_spherical_projection/pytests/test_errorStarClass.py`

 * *Files 26% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 # Pytest for starClass()
-# centerline-width/: python3 -m pytest -v
-import logging
+# star_chart_spherical_projection/: python -m pytest -v
+import re
 
 # External Python libraries (installed via pip install)
 import pytest
 
 # Internal star_chart_spherical_projection reference to access functions, global variables, and error handling
 import star_chart_spherical_projection as scsp
 
@@ -13,341 +13,255 @@
 						([], "<class 'list'>"),
 						(False, "<class 'bool'>")]
 
 invalid_non_num_options = [([], "<class 'list'>"),
 						("string", "<class 'str'>"),
 						(False, "<class 'bool'>")]
 
-def test_starClass_starNameRequired(caplog):
-	# Test:
-	with pytest.raises(SystemExit):
+def test_starClass_starNameRequired():
+	with pytest.raises(ValueError, match=re.escape("[starName]: starName is required")):
 		scsp.newStar(starName=None)
-	log_record = caplog.records[0]
-	assert log_record.levelno == logging.CRITICAL
-	assert log_record.message == "\nCRITICAL ERROR, [starName]: starName is required"
 
 @pytest.mark.parametrize("invalid_input, error_output", invalid_non_str_options)
-def test_starClass_starNameInvalidTypes(caplog, invalid_input, error_output):
-	# Test:
-	with pytest.raises(SystemExit):
+def test_starClass_starNameInvalidTypes(invalid_input, error_output):
+	with pytest.raises(ValueError, match=re.escape(f"[starName]: Must be a str, current type = '{error_output}'")):
 		scsp.newStar(starName=invalid_input)
-	log_record = caplog.records[0]
-	assert log_record.levelno == logging.CRITICAL
-	assert log_record.message == "\nCRITICAL ERROR, [starName]: Must be a str, current type = '{0}'".format(error_output)
-
-def test_starClass_RARequired(caplog):
-	# Test:
-	with pytest.raises(SystemExit):
+
+def test_starClass_RARequired():
+	with pytest.raises(ValueError, match=re.escape("[ra]: Right Ascension is required")):
 		scsp.newStar(starName="testing Star",
 					ra=None)
-	log_record = caplog.records[0]
-	assert log_record.levelno == logging.CRITICAL
-	assert log_record.message == "\nCRITICAL ERROR, [ra]: Right Ascension is required"
 
 @pytest.mark.parametrize("invalid_input, error_output", invalid_non_str_options)
-def test_starClass_RAInvalidTypes(caplog, invalid_input, error_output):
-	# Test:
-	with pytest.raises(SystemExit):
+def test_starClass_RAInvalidTypes(invalid_input, error_output):
+	with pytest.raises(ValueError, match=re.escape(f"[ra]: Must be a str, current type = '{error_output}'")):
 		scsp.newStar(starName="Testing Star",
 					ra=invalid_input)
-	log_record = caplog.records[0]
-	assert log_record.levelno == logging.CRITICAL
-	assert log_record.message == "\nCRITICAL ERROR, [ra]: Must be a str, current type = '{0}'".format(error_output)
-
-def test_starClass_RAInvalidFormat(caplog):
-	# Test:
-	with pytest.raises(SystemExit):
+
+def test_starClass_RAInvalidFormat():
+	with pytest.raises(ValueError, match=re.escape("[ra]: Right Ascension must be three parts '[HH, MM, SS]' (Hours, Minutes, Seconds), currently  = '['1', '2', '3', '4']'")):
 		scsp.newStar(starName="Testing Star",
 					ra="1.2.3.4")
-	log_record = caplog.records[0]
-	assert log_record.levelno == logging.CRITICAL
-	assert log_record.message == "\nCRITICAL ERROR, [ra]: Right Ascension must be three parts '[HH, MM, SS]' (Hours, Minutes, Seconds), currently  = '['1', '2', '3', '4']'"
-
-def test_starClass_RAInvalidTimeFormat(caplog):
-	# Test:
-	with pytest.raises(SystemExit):
+
+def test_starClass_RAInvalidTimeFormat():
+	with pytest.raises(ValueError, match=re.escape("[ra]: Each part of the Right Ascension must be an integar, 'a' current type = <class 'str'>")):
 		scsp.newStar(starName="Testing Star",
 					ra="1.2.a")
-	log_record = caplog.records[0]
-	assert log_record.levelno == logging.CRITICAL
-	assert log_record.message == "\nCRITICAL ERROR, [ra]: Each part of the Right Ascension must be an integar, 'a' current type = <class 'str'>"
-
 
-def test_starClass_DecRequired(caplog):
-	# Test:
-	with pytest.raises(SystemExit):
+def test_starClass_DecRequired():
+	with pytest.raises(ValueError, match=re.escape("[dec]: Declination is required")):
 		scsp.newStar(starName="testing Star",
 					ra="1.2.3",
 					dec=None)
-	log_record = caplog.records[0]
-	assert log_record.levelno == logging.CRITICAL
-	assert log_record.message == "\nCRITICAL ERROR, [dec]: Declination is required"
 
 @pytest.mark.parametrize("invalid_input, error_output", invalid_non_num_options)
-def test_starClass_DECInvalidTypes(caplog, invalid_input, error_output):
-	# Test:
-	with pytest.raises(SystemExit):
+def test_starClass_DECInvalidTypes(invalid_input, error_output):
+	with pytest.raises(ValueError, match=re.escape(f"[dec]: Must be a int or float, current type = '{error_output}'")):
 		scsp.newStar(starName="Testing Star",
 					ra="1.2.3",
 					dec=invalid_input)
-	log_record = caplog.records[0]
-	assert log_record.levelno == logging.CRITICAL
-	assert log_record.message == "\nCRITICAL ERROR, [dec]: Must be a int or float, current type = '{0}'".format(error_output)
 
 @pytest.mark.parametrize("invalid_input, error_output", invalid_non_num_options)
-def test_starClass_properMotionSpeedInvalidTypes(caplog, invalid_input, error_output):
-	# Test:
-	with pytest.raises(SystemExit):
+def test_starClass_properMotionSpeedInvalidTypes(invalid_input, error_output):
+	with pytest.raises(ValueError, match=re.escape(f"[properMotionSpeed]: Must be a int or float, current type = '{error_output}'")):
 		scsp.newStar(starName="Testing Star",
 					ra="1.2.3",
 					dec=12.3,
 					properMotionSpeed=invalid_input)
-	log_record = caplog.records[0]
-	assert log_record.levelno == logging.CRITICAL
-	assert log_record.message == "\nCRITICAL ERROR, [properMotionSpeed]: Must be a int or float, current type = '{0}'".format(error_output)
 
 @pytest.mark.parametrize("invalid_input, error_output", invalid_non_num_options)
-def test_starClass_properMotionAngleInvalidTypes(caplog, invalid_input, error_output):
-	# Test:
-	with pytest.raises(SystemExit):
+def test_starClass_properMotionAngleInvalidTypes(invalid_input, error_output):
+	with pytest.raises(ValueError, match=re.escape(f"[properMotionAngle]: Must be a int or float, current type = '{error_output}'")):
 		scsp.newStar(starName="Testing Star",
 					ra="1.2.3",
 					dec=12.3,
 					properMotionSpeed=123.4,
 					properMotionAngle=invalid_input)
-	log_record = caplog.records[0]
-	assert log_record.levelno == logging.CRITICAL
-	assert log_record.message == "\nCRITICAL ERROR, [properMotionAngle]: Must be a int or float, current type = '{0}'".format(error_output)
 
 @pytest.mark.parametrize("invalid_input, error_output", invalid_non_num_options)
-def test_starClass_properMotionSpeedRAInvalidTypes(caplog, invalid_input, error_output):
-	# Test:
-	with pytest.raises(SystemExit):
+def test_starClass_properMotionSpeedRAInvalidTypes(invalid_input, error_output):
+	with pytest.raises(ValueError, match=re.escape(f"[properMotionSpeedRA]: Must be a int or float, current type = '{error_output}'")):
 		scsp.newStar(starName="Testing Star",
 					ra="1.2.3",
 					dec=12.3,
 					properMotionSpeedRA=invalid_input)
-	log_record = caplog.records[0]
-	assert log_record.levelno == logging.CRITICAL
-	assert log_record.message == "\nCRITICAL ERROR, [properMotionSpeedRA]: Must be a int or float, current type = '{0}'".format(error_output)
 
 @pytest.mark.parametrize("invalid_input, error_output", invalid_non_num_options)
-def test_starClass_properMotionSpeedDecInvalidTypes(caplog, invalid_input, error_output):
-	# Test:
-	with pytest.raises(SystemExit):
+def test_starClass_properMotionSpeedDecInvalidTypes(invalid_input, error_output):
+	with pytest.raises(ValueError, match=re.escape(f"[properMotionSpeedDec]: Must be a int or float, current type = '{error_output}'")):
 		scsp.newStar(starName="Testing Star",
 					ra="1.2.3",
 					dec=12.3,
 					properMotionSpeedDec=invalid_input)
-	log_record = caplog.records[0]
-	assert log_record.levelno == logging.CRITICAL
-	assert log_record.message == "\nCRITICAL ERROR, [properMotionSpeedDec]: Must be a int or float, current type = '{0}'".format(error_output)
-
-def test_starClass_properMotionSpeedAngleOrRADecRequired(caplog):
-	# Test:
-	with pytest.raises(SystemExit):
+
+def test_starClass_properMotionSpeedAngleOrRADecRequired():
+	with pytest.raises(ValueError, match=re.escape("Either properMotionSpeedRA/properMotionSpeedDec or properMotionSpeed/properMotionAngle is required")):
 		scsp.newStar(starName="Testing Star",
 					ra="1.2.3",
 					dec=12.3,
 					magnitudeVisual=1.2,
 					properMotionSpeed=None,
 					properMotionAngle=None,
 					properMotionSpeedDec=None,
 					properMotionSpeedRA=None)
-	log_record = caplog.records[0]
-	assert log_record.levelno == logging.CRITICAL
-	assert log_record.message == "\nCRITICAL ERROR, Either properMotionSpeedRA/properMotionSpeedDec or properMotionSpeed/properMotionAngle is required"
-
-def test_starClass_properMotionSpeedAngleOrRADecOnlyOneRequired(caplog):
-	# Test:
-	with pytest.raises(SystemExit):
+
+def test_starClass_properMotionSpeedAngleOrRADecOnlyOneRequired():
+	with pytest.raises(ValueError, match=re.escape("Either properMotionSpeedRA/properMotionSpeedDec or properMotionSpeed/properMotionAngle is required, not both")):
 		scsp.newStar(starName="Testing Star",
 					ra="1.2.3",
 					dec=12.3,
 					magnitudeVisual=1.2,
 					properMotionSpeed=12.3,
 					properMotionAngle=32.1,
 					properMotionSpeedDec=45.6,
 					properMotionSpeedRA=65.4)
-	log_record = caplog.records[0]
-	assert log_record.levelno == logging.CRITICAL
-	assert log_record.message == "\nCRITICAL ERROR, Either properMotionSpeedRA/properMotionSpeedDec or properMotionSpeed/properMotionAngle is required, not both"
-
-def test_starClass_properMotionSpeedDecExtra(caplog):
-	# Test:
-	with pytest.raises(SystemExit):
+
+def test_starClass_properMotionSpeedDecExtra():
+	with pytest.raises(ValueError, match=re.escape("[properMotionSpeedDec]: With properMotionSpeed/properMotionAngle set, properMotionSpeedDec should be None")):
 		scsp.newStar(starName="Testing Star",
 					ra="1.2.3",
 					dec=12.3,
 					magnitudeVisual=1.2,
 					properMotionSpeed=12.3,
 					properMotionAngle=32.1,
 					properMotionSpeedDec=45.6,
 					properMotionSpeedRA=None)
-	log_record = caplog.records[0]
-	assert log_record.levelno == logging.CRITICAL
-	assert log_record.message == "\nCRITICAL ERROR, [properMotionSpeedDec]: With properMotionSpeed/properMotionAngle set, properMotionSpeedDec should be None"
-
-def test_starClass_properMotionSpeedRAExtra(caplog):
-	# Test:
-	with pytest.raises(SystemExit):
+
+def test_starClass_properMotionSpeedRAExtra():
+	with pytest.raises(ValueError, match=re.escape("[properMotionSpeedRA]: With properMotionSpeed/properMotionAngle set, properMotionSpeedRA should be None")):
 		scsp.newStar(starName="Testing Star",
 					ra="1.2.3",
 					dec=12.3,
 					magnitudeVisual=1.2,
 					properMotionSpeed=12.3,
 					properMotionAngle=32.1,
 					properMotionSpeedDec=None,
 					properMotionSpeedRA=65.4)
-	log_record = caplog.records[0]
-	assert log_record.levelno == logging.CRITICAL
-	assert log_record.message == "\nCRITICAL ERROR, [properMotionSpeedRA]: With properMotionSpeed/properMotionAngle set, properMotionSpeedRA should be None"
-
-def test_starClass_properMotionSpeedExtra(caplog):
-	# Test:
-	with pytest.raises(SystemExit):
+
+def test_starClass_properMotionSpeedExtra():
+	with pytest.raises(ValueError, match=re.escape("[properMotionSpeed]: With properMotionSpeedRA/properMotionSpeedDec set, properMotionSpeed should be None")):
 		scsp.newStar(starName="Testing Star",
 					ra="1.2.3",
 					dec=12.3,
 					magnitudeVisual=1.2,
 					properMotionSpeed=12.3,
 					properMotionAngle=None,
 					properMotionSpeedDec=45.6,
 					properMotionSpeedRA=65.4)
-	log_record = caplog.records[0]
-	assert log_record.levelno == logging.CRITICAL
-	assert log_record.message == "\nCRITICAL ERROR, [properMotionSpeed]: With properMotionSpeedRA/properMotionSpeedDec set, properMotionSpeed should be None"
-
-def test_starClass_properMotionAngleExtra(caplog):
-	# Test:
-	with pytest.raises(SystemExit):
+
+def test_starClass_properMotionAngleExtra():
+	with pytest.raises(ValueError, match=re.escape("[properMotionAngle]: With properMotionSpeedRA/properMotionSpeedDec set, properMotionAngle should be None")):
 		scsp.newStar(starName="Testing Star",
 					ra="1.2.3",
 					dec=12.3,
 					magnitudeVisual=1.2,
 					properMotionSpeed=None,
 					properMotionAngle=32.1,
 					properMotionSpeedDec=45.6,
 					properMotionSpeedRA=65.4)
-	log_record = caplog.records[0]
-	assert log_record.levelno == logging.CRITICAL
-	assert log_record.message == "\nCRITICAL ERROR, [properMotionAngle]: With properMotionSpeedRA/properMotionSpeedDec set, properMotionAngle should be None"
-
-def test_starClass_properMotionSpeedDecRequiredWithRA(caplog):
-	# Test:
-	with pytest.raises(SystemExit):
+
+def test_starClass_properMotionSpeedDecRequiredWithRA():
+	with pytest.raises(ValueError, match=re.escape("[properMotionSpeedDec]: With properMotionSpeedRA set, properMotionSpeedDec is required")):
 		scsp.newStar(starName="Testing Star",
 					ra="1.2.3",
 					dec=12.3,
 					magnitudeVisual=1.2,
 					properMotionSpeed=None,
 					properMotionAngle=None,
 					properMotionSpeedDec=None,
 					properMotionSpeedRA=65.4)
-	log_record = caplog.records[0]
-	assert log_record.levelno == logging.CRITICAL
-	assert log_record.message == "\nCRITICAL ERROR, [properMotionSpeedDec]: With properMotionSpeedRA set, properMotionSpeedDec is required"
-
-def test_starClass_properMotionSpeedDecRequiredWithRA(caplog):
-	# Test:
-	with pytest.raises(SystemExit):
+
+def test_starClass_properMotionSpeedDecRequiredWithRA():
+	with pytest.raises(ValueError, match=re.escape("[properMotionSpeedRA]: With properMotionSpeedDec set, properMotionSpeedRA is required")):
 		scsp.newStar(starName="Testing Star",
 					ra="1.2.3",
 					dec=12.3,
 					magnitudeVisual=1.2,
 					properMotionSpeed=None,
 					properMotionAngle=None,
 					properMotionSpeedDec=45.6,
 					properMotionSpeedRA=None)
-	log_record = caplog.records[0]
-	assert log_record.levelno == logging.CRITICAL
-	assert log_record.message == "\nCRITICAL ERROR, [properMotionSpeedRA]: With properMotionSpeedDec set, properMotionSpeedRA is required"
-
-def test_starClass_properMotionAngleRequiredWithSpeed(caplog):
-	# Test:
-	with pytest.raises(SystemExit):
+
+def test_starClass_properMotionAngleRequiredWithSpeed():
+	with pytest.raises(ValueError, match=re.escape("[properMotionAngle]: With properMotionSpeed set, properMotionAngle is required")):
 		scsp.newStar(starName="Testing Star",
 					ra="1.2.3",
 					dec=12.3,
 					magnitudeVisual=1.2,
 					properMotionSpeed=12.3,
 					properMotionAngle=None,
 					properMotionSpeedDec=None,
 					properMotionSpeedRA=None)
-	log_record = caplog.records[0]
-	assert log_record.levelno == logging.CRITICAL
-	assert log_record.message == "\nCRITICAL ERROR, [properMotionAngle]: With properMotionSpeed set, properMotionAngle is required"
-
-def test_starClass_properMotionSpeedRequiredWithAngle(caplog):
-	# Test:
-	with pytest.raises(SystemExit):
+
+def test_starClass_properMotionSpeedRequiredWithAngle():
+	with pytest.raises(ValueError, match=re.escape("[properMotionSpeed]: With properMotionAngle set, properMotionSpeed is required")):
 		scsp.newStar(starName="Testing Star",
 					ra="1.2.3",
 					dec=12.3,
 					magnitudeVisual=1.2,
 					properMotionSpeed=None,
 					properMotionAngle=32.1,
 					properMotionSpeedDec=None,
 					properMotionSpeedRA=None)
-	log_record = caplog.records[0]
-	assert log_record.levelno == logging.CRITICAL
-	assert log_record.message == "\nCRITICAL ERROR, [properMotionSpeed]: With properMotionAngle set, properMotionSpeed is required"
-
-def test_starClass_properMotionSpeedvsDec(caplog):
-	# Test:
-	with pytest.raises(SystemExit):
+
+def test_starClass_properMotionSpeedvsDec():
+	with pytest.raises(ValueError, match=re.escape("Should be a pair of properMotionSpeedRA/properMotionSpeedDec or properMotionSpeed/properMotionAngle, not properMotionSpeed/properMotionSpeedDec")):
 		scsp.newStar(starName="Testing Star",
 					ra="1.2.3",
 					dec=12.3,
 					magnitudeVisual=1.2,
 					properMotionSpeed=12.3,
 					properMotionAngle=None,
 					properMotionSpeedDec=34.5,
 					properMotionSpeedRA=None)
-	log_record = caplog.records[0]
-	assert log_record.levelno == logging.CRITICAL
-	assert log_record.message == "\nCRITICAL ERROR, Should be a pair of properMotionSpeedRA/properMotionSpeedDec or properMotionSpeed/properMotionAngle, not properMotionSpeed/properMotionSpeedDec"
-
-def test_starClass_properMotionSpeedvsRA(caplog):
-	# Test:
-	with pytest.raises(SystemExit):
+
+def test_starClass_properMotionSpeedvsRA():
+	with pytest.raises(ValueError, match=re.escape("Should be a pair of properMotionSpeedRA/properMotionSpeedDec or properMotionSpeed/properMotionAngle, not properMotionSpeed/properMotionSpeedRA")):
 		scsp.newStar(starName="Testing Star",
 					ra="1.2.3",
 					dec=12.3,
 					magnitudeVisual=1.2,
 					properMotionSpeed=12.3,
 					properMotionAngle=None,
 					properMotionSpeedDec=None,
 					properMotionSpeedRA=34.5)
-	log_record = caplog.records[0]
-	assert log_record.levelno == logging.CRITICAL
-	assert log_record.message == "\nCRITICAL ERROR, Should be a pair of properMotionSpeedRA/properMotionSpeedDec or properMotionSpeed/properMotionAngle, not properMotionSpeed/properMotionSpeedRA"
-
-def test_starClass_properMotionAnglevsDec(caplog):
-	# Test:
-	with pytest.raises(SystemExit):
+
+def test_starClass_properMotionAnglevsDec():
+	with pytest.raises(ValueError, match=re.escape("Should be a pair of properMotionSpeedRA/properMotionSpeedDec or properMotionSpeed/properMotionAngle, not properMotionAngle/properMotionSpeedDec")):
 		scsp.newStar(starName="Testing Star",
 					ra="1.2.3",
 					dec=12.3,
 					magnitudeVisual=1.2,
 					properMotionSpeed=None,
 					properMotionAngle=12.3,
 					properMotionSpeedDec=34.5,
 					properMotionSpeedRA=None)
-	log_record = caplog.records[0]
-	assert log_record.levelno == logging.CRITICAL
-	assert log_record.message == "\nCRITICAL ERROR, Should be a pair of properMotionSpeedRA/properMotionSpeedDec or properMotionSpeed/properMotionAngle, not properMotionAngle/properMotionSpeedDec"
-
-def test_starClass_properMotionAnglevsRA(caplog):
-	# Test:
-	with pytest.raises(SystemExit):
+
+def test_starClass_properMotionAnglevsRA():
+	with pytest.raises(ValueError, match=re.escape("Should be a pair of properMotionSpeedRA/properMotionSpeedDec or properMotionSpeed/properMotionAngle, not properMotionAngle/properMotionSpeedRA")):
 		scsp.newStar(starName="Testing Star",
 					ra="1.2.3",
 					dec=12.3,
 					magnitudeVisual=1.2,
 					properMotionSpeed=None,
 					properMotionAngle=12.3,
 					properMotionSpeedDec=None,
 					properMotionSpeedRA=34.5)
-	log_record = caplog.records[0]
-	assert log_record.levelno == logging.CRITICAL
-	assert log_record.message == "\nCRITICAL ERROR, Should be a pair of properMotionSpeedRA/properMotionSpeedDec or properMotionSpeed/properMotionAngle, not properMotionAngle/properMotionSpeedRA"
+
+def test_starClass_magnitudeVisualRequired():
+	with pytest.raises(ValueError, match=re.escape("[magnitudeVisual]: magnitudeVisual is required")):
+		scsp.newStar(starName="Testing Star",
+					ra="1.2.3",
+					dec=12.3,
+					magnitudeVisual=None,
+					properMotionSpeed=12.3,
+					properMotionAngle=32.1)
+
+@pytest.mark.parametrize("invalid_input, error_output", invalid_non_num_options)
+def test_starClass_magnitudeVisualRequired(invalid_input, error_output):
+	with pytest.raises(ValueError, match=re.escape(f"[magnitudeVisual]: Must be a int or float, current type = '{error_output}'")):
+		scsp.newStar(starName="Testing Star",
+					ra="1.2.3",
+					dec=12.3,
+					magnitudeVisual=invalid_input,
+					properMotionSpeed=12.3,
+					properMotionAngle=32.1)
```

### Comparing `star-chart-spherical-projection-1.5.0/star_chart_spherical_projection/ra_dec_precession_vondrak.py` & `star-chart-spherical-projection-1.6.0/star_chart_spherical_projection/ra_dec_precession_vondrak.py`

 * *Files identical despite different names*

### Comparing `star-chart-spherical-projection-1.5.0/star_chart_spherical_projection/starClass.py` & `star-chart-spherical-projection-1.6.0/star_chart_spherical_projection/starClass.py`

 * *Files identical despite different names*

### Comparing `star-chart-spherical-projection-1.5.0/star_chart_spherical_projection.egg-info/SOURCES.txt` & `star-chart-spherical-projection-1.6.0/star_chart_spherical_projection.egg-info/SOURCES.txt`

 * *Files 6% similar despite different names*

```diff
@@ -1,20 +1,23 @@
+LICENSE
 MANIFEST.in
 README.md
 setup.py
 star_chart_spherical_projection/__init__.py
-star_chart_spherical_projection/config.ini
 star_chart_spherical_projection/declination_r_axis.py
 star_chart_spherical_projection/error_handling.py
 star_chart_spherical_projection/generate_star_chart.py
+star_chart_spherical_projection/position_of_stars.py
 star_chart_spherical_projection/ra_dec_precession_vondrak.py
 star_chart_spherical_projection/starClass.py
 star_chart_spherical_projection.egg-info/PKG-INFO
 star_chart_spherical_projection.egg-info/SOURCES.txt
 star_chart_spherical_projection.egg-info/dependency_links.txt
 star_chart_spherical_projection.egg-info/requires.txt
 star_chart_spherical_projection.egg-info/top_level.txt
 star_chart_spherical_projection/data/convert_lst_to_csv_data.py
 star_chart_spherical_projection/data/star_data.csv
-star_chart_spherical_projection/pytests/test_finalPositionOfStars.py
-star_chart_spherical_projection/pytests/test_plotStereographicProjection.py
-star_chart_spherical_projection/pytests/test_starClass.py
+star_chart_spherical_projection/data/web_scrap_iau_catolog.py
+star_chart_spherical_projection/pytests/test_errorFinalPositionOfStars.py
+star_chart_spherical_projection/pytests/test_errorPlotStereographicProjection.py
+star_chart_spherical_projection/pytests/test_errorPredictPoleStar.py
+star_chart_spherical_projection/pytests/test_errorStarClass.py
```

