# Comparing `tmp/dkist_quality-1.0.3.tar.gz` & `tmp/dkist_quality-1.0.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dkist_quality-1.0.3.tar", last modified: Fri May 24 18:16:09 2024, max compression
+gzip compressed data, was "dkist_quality-1.0.4.tar", last modified: Tue May 28 22:40:32 2024, max compression
```

## Comparing `dkist_quality-1.0.3.tar` & `dkist_quality-1.0.4.tar`

### file list

```diff
@@ -1,30 +1,30 @@
-drwxrwxrwx   0 root         (0) root         (0)        0 2024-05-24 18:16:09.416220 dkist_quality-1.0.3/
--rw-rw-rw-   0 root         (0) root         (0)     3104 2024-05-24 18:15:52.000000 dkist_quality-1.0.3/.gitignore
--rw-rw-rw-   0 root         (0) root         (0)      580 2024-05-24 18:15:52.000000 dkist_quality-1.0.3/.pre-commit-config.yaml
--rw-rw-rw-   0 root         (0) root         (0)     1063 2024-05-24 18:15:52.000000 dkist_quality-1.0.3/LICENSE
--rw-rw-rw-   0 root         (0) root         (0)      468 2024-05-24 18:15:52.000000 dkist_quality-1.0.3/MANIFEST.in
--rw-r--r--   0 root         (0) root         (0)     2160 2024-05-24 18:16:09.416220 dkist_quality-1.0.3/PKG-INFO
--rw-rw-rw-   0 root         (0) root         (0)     1229 2024-05-24 18:15:52.000000 dkist_quality-1.0.3/README.rst
--rw-rw-rw-   0 root         (0) root         (0)     2791 2024-05-24 18:15:52.000000 dkist_quality-1.0.3/bitbucket-pipelines.yml
-drwxrwxrwx   0 root         (0) root         (0)        0 2024-05-24 18:16:09.412220 dkist_quality-1.0.3/dkist_quality/
--rw-rw-rw-   0 root         (0) root         (0)        0 2024-05-24 18:15:52.000000 dkist_quality-1.0.3/dkist_quality/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)      411 2024-05-24 18:16:09.000000 dkist_quality-1.0.3/dkist_quality/_version.py
-drwxrwxrwx   0 root         (0) root         (0)        0 2024-05-24 18:16:09.416220 dkist_quality-1.0.3/dkist_quality/fonts/
--rw-rw-rw-   0 root         (0) root         (0)    91676 2024-05-24 18:15:52.000000 dkist_quality-1.0.3/dkist_quality/fonts/Oswald-Bold.ttf
--rw-rw-rw-   0 root         (0) root         (0)    91400 2024-05-24 18:15:52.000000 dkist_quality-1.0.3/dkist_quality/fonts/Oswald-Regular.ttf
--rw-rw-rw-   0 root         (0) root         (0)      871 2024-05-24 18:15:52.000000 dkist_quality-1.0.3/dkist_quality/json_encoder.py
--rw-rw-rw-   0 root         (0) root         (0)    37316 2024-05-24 18:15:52.000000 dkist_quality-1.0.3/dkist_quality/report.py
-drwxrwxrwx   0 root         (0) root         (0)        0 2024-05-24 18:16:09.416220 dkist_quality-1.0.3/dkist_quality/tests/
--rw-rw-rw-   0 root         (0) root         (0)        0 2024-05-24 18:15:52.000000 dkist_quality-1.0.3/dkist_quality/tests/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)    11866 2024-05-24 18:15:52.000000 dkist_quality-1.0.3/dkist_quality/tests/test_report.py
--rw-rw-rw-   0 root         (0) root         (0)      346 2024-05-24 18:15:52.000000 dkist_quality-1.0.3/dkist_quality/version.py
-drwxrwxrwx   0 root         (0) root         (0)        0 2024-05-24 18:16:09.416220 dkist_quality-1.0.3/dkist_quality.egg-info/
--rw-r--r--   0 root         (0) root         (0)     2160 2024-05-24 18:16:09.000000 dkist_quality-1.0.3/dkist_quality.egg-info/PKG-INFO
--rw-rw-rw-   0 root         (0) root         (0)      605 2024-05-24 18:16:09.000000 dkist_quality-1.0.3/dkist_quality.egg-info/SOURCES.txt
--rw-rw-rw-   0 root         (0) root         (0)        1 2024-05-24 18:16:09.000000 dkist_quality-1.0.3/dkist_quality.egg-info/dependency_links.txt
--rw-rw-rw-   0 root         (0) root         (0)        1 2024-05-24 18:16:08.000000 dkist_quality-1.0.3/dkist_quality.egg-info/not-zip-safe
--rw-rw-rw-   0 root         (0) root         (0)      144 2024-05-24 18:16:09.000000 dkist_quality-1.0.3/dkist_quality.egg-info/requires.txt
--rw-rw-rw-   0 root         (0) root         (0)       25 2024-05-24 18:16:09.000000 dkist_quality-1.0.3/dkist_quality.egg-info/top_level.txt
--rw-rw-rw-   0 root         (0) root         (0)     2048 2024-05-24 18:15:52.000000 dkist_quality-1.0.3/pyproject.toml
--rw-rw-rw-   0 root         (0) root         (0)       38 2024-05-24 18:16:09.416220 dkist_quality-1.0.3/setup.cfg
--rw-rw-rw-   0 root         (0) root         (0)     1214 2024-05-24 18:15:52.000000 dkist_quality-1.0.3/tox.ini
+drwxrwxrwx   0 root         (0) root         (0)        0 2024-05-28 22:40:32.481357 dkist_quality-1.0.4/
+-rw-rw-rw-   0 root         (0) root         (0)     3104 2024-05-28 22:40:20.000000 dkist_quality-1.0.4/.gitignore
+-rw-rw-rw-   0 root         (0) root         (0)      580 2024-05-28 22:40:20.000000 dkist_quality-1.0.4/.pre-commit-config.yaml
+-rw-rw-rw-   0 root         (0) root         (0)     1063 2024-05-28 22:40:20.000000 dkist_quality-1.0.4/LICENSE
+-rw-rw-rw-   0 root         (0) root         (0)      468 2024-05-28 22:40:20.000000 dkist_quality-1.0.4/MANIFEST.in
+-rw-r--r--   0 root         (0) root         (0)     2160 2024-05-28 22:40:32.477357 dkist_quality-1.0.4/PKG-INFO
+-rw-rw-rw-   0 root         (0) root         (0)     1229 2024-05-28 22:40:20.000000 dkist_quality-1.0.4/README.rst
+-rw-rw-rw-   0 root         (0) root         (0)     2791 2024-05-28 22:40:20.000000 dkist_quality-1.0.4/bitbucket-pipelines.yml
+drwxrwxrwx   0 root         (0) root         (0)        0 2024-05-28 22:40:32.477357 dkist_quality-1.0.4/dkist_quality/
+-rw-rw-rw-   0 root         (0) root         (0)        0 2024-05-28 22:40:20.000000 dkist_quality-1.0.4/dkist_quality/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)      411 2024-05-28 22:40:32.000000 dkist_quality-1.0.4/dkist_quality/_version.py
+drwxrwxrwx   0 root         (0) root         (0)        0 2024-05-28 22:40:32.477357 dkist_quality-1.0.4/dkist_quality/fonts/
+-rw-rw-rw-   0 root         (0) root         (0)    91676 2024-05-28 22:40:20.000000 dkist_quality-1.0.4/dkist_quality/fonts/Oswald-Bold.ttf
+-rw-rw-rw-   0 root         (0) root         (0)    91400 2024-05-28 22:40:20.000000 dkist_quality-1.0.4/dkist_quality/fonts/Oswald-Regular.ttf
+-rw-rw-rw-   0 root         (0) root         (0)      871 2024-05-28 22:40:20.000000 dkist_quality-1.0.4/dkist_quality/json_encoder.py
+-rw-rw-rw-   0 root         (0) root         (0)    37398 2024-05-28 22:40:20.000000 dkist_quality-1.0.4/dkist_quality/report.py
+drwxrwxrwx   0 root         (0) root         (0)        0 2024-05-28 22:40:32.477357 dkist_quality-1.0.4/dkist_quality/tests/
+-rw-rw-rw-   0 root         (0) root         (0)        0 2024-05-28 22:40:20.000000 dkist_quality-1.0.4/dkist_quality/tests/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)    11866 2024-05-28 22:40:20.000000 dkist_quality-1.0.4/dkist_quality/tests/test_report.py
+-rw-rw-rw-   0 root         (0) root         (0)      346 2024-05-28 22:40:20.000000 dkist_quality-1.0.4/dkist_quality/version.py
+drwxrwxrwx   0 root         (0) root         (0)        0 2024-05-28 22:40:32.477357 dkist_quality-1.0.4/dkist_quality.egg-info/
+-rw-r--r--   0 root         (0) root         (0)     2160 2024-05-28 22:40:32.000000 dkist_quality-1.0.4/dkist_quality.egg-info/PKG-INFO
+-rw-rw-rw-   0 root         (0) root         (0)      605 2024-05-28 22:40:32.000000 dkist_quality-1.0.4/dkist_quality.egg-info/SOURCES.txt
+-rw-rw-rw-   0 root         (0) root         (0)        1 2024-05-28 22:40:32.000000 dkist_quality-1.0.4/dkist_quality.egg-info/dependency_links.txt
+-rw-rw-rw-   0 root         (0) root         (0)        1 2024-05-28 22:40:32.000000 dkist_quality-1.0.4/dkist_quality.egg-info/not-zip-safe
+-rw-rw-rw-   0 root         (0) root         (0)      144 2024-05-28 22:40:32.000000 dkist_quality-1.0.4/dkist_quality.egg-info/requires.txt
+-rw-rw-rw-   0 root         (0) root         (0)       25 2024-05-28 22:40:32.000000 dkist_quality-1.0.4/dkist_quality.egg-info/top_level.txt
+-rw-rw-rw-   0 root         (0) root         (0)     2048 2024-05-28 22:40:20.000000 dkist_quality-1.0.4/pyproject.toml
+-rw-rw-rw-   0 root         (0) root         (0)       38 2024-05-28 22:40:32.481357 dkist_quality-1.0.4/setup.cfg
+-rw-rw-rw-   0 root         (0) root         (0)     1214 2024-05-28 22:40:20.000000 dkist_quality-1.0.4/tox.ini
```

### Comparing `dkist_quality-1.0.3/.gitignore` & `dkist_quality-1.0.4/.gitignore`

 * *Files identical despite different names*

### Comparing `dkist_quality-1.0.3/.pre-commit-config.yaml` & `dkist_quality-1.0.4/.pre-commit-config.yaml`

 * *Files identical despite different names*

### Comparing `dkist_quality-1.0.3/LICENSE` & `dkist_quality-1.0.4/LICENSE`

 * *Files identical despite different names*

### Comparing `dkist_quality-1.0.3/PKG-INFO` & `dkist_quality-1.0.4/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: dkist-quality
-Version: 1.0.3
+Version: 1.0.4
 Summary: DKIST library for generating quality report pdf
 Author-email: NSO / AURA <dkistdc@nso.edu>
 License: MIT
 Project-URL: repository, https://bitbucket.org/dkistdc/dkist-quality
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.10
```

### Comparing `dkist_quality-1.0.3/README.rst` & `dkist_quality-1.0.4/README.rst`

 * *Files identical despite different names*

### Comparing `dkist_quality-1.0.3/bitbucket-pipelines.yml` & `dkist_quality-1.0.4/bitbucket-pipelines.yml`

 * *Files identical despite different names*

### Comparing `dkist_quality-1.0.3/dkist_quality/fonts/Oswald-Bold.ttf` & `dkist_quality-1.0.4/dkist_quality/fonts/Oswald-Bold.ttf`

 * *Files identical despite different names*

### Comparing `dkist_quality-1.0.3/dkist_quality/fonts/Oswald-Regular.ttf` & `dkist_quality-1.0.4/dkist_quality/fonts/Oswald-Regular.ttf`

 * *Files identical despite different names*

### Comparing `dkist_quality-1.0.3/dkist_quality/json_encoder.py` & `dkist_quality-1.0.4/dkist_quality/json_encoder.py`

 * *Files identical despite different names*

### Comparing `dkist_quality-1.0.3/dkist_quality/report.py` & `dkist_quality-1.0.4/dkist_quality/report.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,32 +1,33 @@
 """
 Report Formatting
 """
+import importlib.resources
 import os
 from datetime import datetime
 from importlib.metadata import version
 from io import BytesIO
+from io import StringIO
 from typing import Any
 
 import dacite
 import matplotlib.dates as mdates
 import numpy as np
+import packaging
 import pandas
-import pkg_resources
 import seaborn as sns
 from cycler import cycler
 from matplotlib import pyplot as plt
 from matplotlib import rc
 from matplotlib import rcdefaults
 from matplotlib import rcParams
 from matplotlib.ticker import _Edge_integer  # noqa
 from matplotlib.ticker import MaxNLocator
 from matplotlib.ticker import scale_range  # noqa
 from natsort import natsorted
-from pkg_resources import packaging  # noqa
 from pydantic import Field
 from pydantic.dataclasses import dataclass as validating_dataclass
 from reportlab.lib import colors
 from reportlab.lib.styles import ParagraphStyle
 from reportlab.pdfbase import pdfmetrics
 from reportlab.pdfbase.ttfonts import TTFont
 from reportlab.platypus import Flowable
@@ -134,17 +135,18 @@
         return availWidth, height
 
 
 # Default size for a spacer i.e. how to vertically space out  elements
 spacer = ConditionalSpacer(1, 10)
 
 # Register official DKIST fonts
-font_dir = pkg_resources.resource_filename("dkist_quality", "fonts")
-pdfmetrics.registerFont(TTFont("Oswald-Bold", os.path.join(font_dir, "Oswald-Bold.ttf")))
-pdfmetrics.registerFont(TTFont("Oswald-Regular", os.path.join(font_dir, "Oswald-Regular.ttf")))
+font_dir = importlib.resources.files("dkist_quality") / "fonts"
+with importlib.resources.as_file(font_dir) as font_path:
+    pdfmetrics.registerFont(TTFont("Oswald-Bold", os.path.join(font_path, "Oswald-Bold.ttf")))
+    pdfmetrics.registerFont(TTFont("Oswald-Regular", os.path.join(font_path, "Oswald-Regular.ttf")))
 
 style_normal = ParagraphStyle(
     name="Normal", fontSize=10, leading=12, textColor=colors.black, fontName="Times-Roman"
 )
 style_bold = ParagraphStyle(name="Bold", parent=style_normal, fontName="Times-Bold")
 style_warn = ParagraphStyle(
     name="Warning",
@@ -555,24 +557,24 @@
         # Much of this taken from https://towardsdatascience.com/violin-strip-swarm-and-raincloud-plots-in-python-as-better-sometimes-alternatives-to-a-boxplot-15019bdff8f8
         fig_width_in, fig_height_in, legend_width_in, line_alpha = self.setup_plot_style()
 
         # Turn off minor ticks to avoid clutter
         rc("xtick.minor", visible=False)
 
         # Load data into a DataFrame
-        data_frame = pandas.read_json(self.raincloud_data.dataframe_json)
+        data_frame = pandas.read_json(StringIO(self.raincloud_data.dataframe_json))
 
         # Make the violin plot. This shows the KDE's
         ax = sns.violinplot(
             y=self.raincloud_data.distribution_column_name,
             x=self.raincloud_data.categorical_column_name,
             data=data_frame,
             color="lightgrey",
             cut=0,
-            scale="width",
+            density_norm="width",
             inner=None,
             width=1,
             linewidth=0.0,
         )
 
         # Clip the right half of each violin to make room for the strip plot
         for item in ax.collections:
```

### Comparing `dkist_quality-1.0.3/dkist_quality/tests/test_report.py` & `dkist_quality-1.0.4/dkist_quality/tests/test_report.py`

 * *Files identical despite different names*

### Comparing `dkist_quality-1.0.3/dkist_quality.egg-info/PKG-INFO` & `dkist_quality-1.0.4/dkist_quality.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: dkist-quality
-Version: 1.0.3
+Version: 1.0.4
 Summary: DKIST library for generating quality report pdf
 Author-email: NSO / AURA <dkistdc@nso.edu>
 License: MIT
 Project-URL: repository, https://bitbucket.org/dkistdc/dkist-quality
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.10
```

### Comparing `dkist_quality-1.0.3/dkist_quality.egg-info/SOURCES.txt` & `dkist_quality-1.0.4/dkist_quality.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `dkist_quality-1.0.3/pyproject.toml` & `dkist_quality-1.0.4/pyproject.toml`

 * *Files identical despite different names*

### Comparing `dkist_quality-1.0.3/tox.ini` & `dkist_quality-1.0.4/tox.ini`

 * *Files identical despite different names*

