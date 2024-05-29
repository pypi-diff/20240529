# Comparing `tmp/sciqlopplots-0.7.0-cp39-cp39-win_amd64.whl.zip` & `tmp/sciqlopplots-0.7.1-cp39-cp39-win_amd64.whl.zip`

## zipinfo {}

```diff
@@ -1,8 +1,8 @@
-Zip file size: 973239 bytes, number of entries: 6
-?rw-rw-r--  2.0 fat     3166 b- defN 24-Apr-15 21:00 sciqlopplots-0.7.0.dist-info/METADATA
-?rw-rw-r--  2.0 fat       83 b- defN 24-Apr-15 21:00 sciqlopplots-0.7.0.dist-info/WHEEL
--rw-rw-rw-  2.0 fat     1585 b- defN 24-Apr-15 20:47 sciqlopplots-0.7.0.dist-info/COPYING
--rw-rw-rw-  2.0 fat  2752000 b- defN 24-Apr-15 21:00 SciQLopPlots/SciQLopPlotsBindings.cp39-win_amd64.pyd
--rw-rw-rw-  2.0 fat      204 b- defN 24-Apr-15 20:47 SciQLopPlots/__init__.py
-?rw-rw-r--  2.0 fat      506 b- defN 24-Apr-15 21:00 sciqlopplots-0.7.0.dist-info/RECORD
-6 files, 2757544 bytes uncompressed, 972325 bytes compressed:  64.8%
+Zip file size: 970646 bytes, number of entries: 6
+?rw-rw-r--  2.0 fat     3166 b- defN 24-May-29 16:13 sciqlopplots-0.7.1.dist-info/METADATA
+?rw-rw-r--  2.0 fat       83 b- defN 24-May-29 16:13 sciqlopplots-0.7.1.dist-info/WHEEL
+-rw-rw-rw-  2.0 fat     1585 b- defN 24-May-29 16:05 sciqlopplots-0.7.1.dist-info/COPYING
+-rw-rw-rw-  2.0 fat  2775040 b- defN 24-May-29 16:13 SciQLopPlots/SciQLopPlotsBindings.cp39-win_amd64.pyd
+-rw-rw-rw-  2.0 fat      204 b- defN 24-May-29 16:05 SciQLopPlots/__init__.py
+?rw-rw-r--  2.0 fat      506 b- defN 24-May-29 16:13 sciqlopplots-0.7.1.dist-info/RECORD
+6 files, 2780584 bytes uncompressed, 969732 bytes compressed:  65.1%
```

## zipnote {}

```diff
@@ -1,19 +1,19 @@
-Filename: sciqlopplots-0.7.0.dist-info/METADATA
+Filename: sciqlopplots-0.7.1.dist-info/METADATA
 Comment: 
 
-Filename: sciqlopplots-0.7.0.dist-info/WHEEL
+Filename: sciqlopplots-0.7.1.dist-info/WHEEL
 Comment: 
 
-Filename: sciqlopplots-0.7.0.dist-info/COPYING
+Filename: sciqlopplots-0.7.1.dist-info/COPYING
 Comment: 
 
 Filename: SciQLopPlots/SciQLopPlotsBindings.cp39-win_amd64.pyd
 Comment: 
 
 Filename: SciQLopPlots/__init__.py
 Comment: 
 
-Filename: sciqlopplots-0.7.0.dist-info/RECORD
+Filename: sciqlopplots-0.7.1.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## SciQLopPlots/__init__.py

```diff
@@ -1,5 +1,5 @@
 from PySide6 import QtCore, QtGui, QtWidgets, QtOpenGL, QtPrintSupport, QtSvg
 from .SciQLopPlotsBindings import *
 from .SciQLopPlotsBindings import _QCustomPlot as QCustomPlot
 
-__version__ = '0.7.0'
+__version__ = '0.7.1'
```

## Comparing `sciqlopplots-0.7.0.dist-info/METADATA` & `sciqlopplots-0.7.1.dist-info/METADATA`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: SciQLopPlots
-Version: 0.7.0
+Version: 0.7.1
 Summary: SciQLop plot API based on QCustomPlot
 Home-page: https://github.com/SciQLop/SciQLopPlots
 Author-Email: Alexis Jeandet <alexis.jeandet@member.fsf.org>
 License: GNU GENERAL PUBLIC LICENSE
                               Version 3, 29 June 2007
         
             An easy to use ISTP loader package.
@@ -45,16 +45,16 @@
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: Python :: 3.12
 Project-URL: Homepage, https://github.com/SciQLop/SciQLopPlots
 Requires-Python: >=3.8
 Requires-Dist: numpy
-Requires-Dist: pyside6==6.6.2
-Requires-Dist: shiboken6==6.6.2
+Requires-Dist: pyside6==6.7.1
+Requires-Dist: shiboken6==6.7.1
 Description-Content-Type: text/markdown
 
 [![License: GPL v3](https://img.shields.io/badge/License-GPLv3-blue.svg)](https://www.gnu.org/licenses/gpl-3.0)
 [![CPP17](https://img.shields.io/badge/Language-C++17-blue.svg)]()
 [![PyPi](https://img.shields.io/pypi/v/sciqlopplots.svg)](https://pypi.python.org/pypi/sciqlopplots)
 [![Coverage](https://codecov.io/gh/SciQLop/CDFpp/coverage.svg?branch=main)](https://codecov.io/gh/SciQLop/SciQLopPlots/branch/main)
```

## Comparing `sciqlopplots-0.7.0.dist-info/COPYING` & `sciqlopplots-0.7.1.dist-info/COPYING`

 * *Files identical despite different names*

