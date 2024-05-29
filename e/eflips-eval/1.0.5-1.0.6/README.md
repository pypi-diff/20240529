# Comparing `tmp/eflips_eval-1.0.5.tar.gz` & `tmp/eflips_eval-1.0.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "eflips_eval-1.0.5.tar", max compression
+gzip compressed data, was "eflips_eval-1.0.6.tar", max compression
```

## Comparing `eflips_eval-1.0.5.tar` & `eflips_eval-1.0.6.tar`

### file list

```diff
@@ -1,10 +1,10 @@
--rw-r--r--   0        0        0    34260 2024-04-22 15:21:44.474064 eflips_eval-1.0.5/LICENSE.md
--rw-r--r--   0        0        0     4656 2024-04-22 15:21:44.474064 eflips_eval-1.0.5/README.md
--rw-r--r--   0        0        0        0 2024-04-22 15:21:44.474064 eflips_eval-1.0.5/eflips/eval/input/__init__.py
--rw-r--r--   0        0        0     3291 2024-04-22 15:21:44.474064 eflips_eval-1.0.5/eflips/eval/input/prepare.py
--rw-r--r--   0        0        0     1321 2024-04-22 15:21:44.478064 eflips_eval-1.0.5/eflips/eval/input/visualize.py
--rw-r--r--   0        0        0        0 2024-04-22 15:21:44.478064 eflips_eval-1.0.5/eflips/eval/output/__init__.py
--rw-r--r--   0        0        0    16194 2024-04-22 15:21:44.478064 eflips_eval-1.0.5/eflips/eval/output/prepare.py
--rw-r--r--   0        0        0    10506 2024-04-22 15:21:44.478064 eflips_eval-1.0.5/eflips/eval/output/visualize.py
--rw-r--r--   0        0        0      781 2024-04-22 15:21:44.498064 eflips_eval-1.0.5/pyproject.toml
--rw-r--r--   0        0        0     5132 1970-01-01 00:00:00.000000 eflips_eval-1.0.5/PKG-INFO
+-rw-r--r--   0        0        0    34260 2024-05-29 13:52:34.479555 eflips_eval-1.0.6/LICENSE.md
+-rw-r--r--   0        0        0     4656 2024-05-29 13:52:34.479555 eflips_eval-1.0.6/README.md
+-rw-r--r--   0        0        0        0 2024-05-29 13:52:34.479555 eflips_eval-1.0.6/eflips/eval/input/__init__.py
+-rw-r--r--   0        0        0     3291 2024-05-29 13:52:34.479555 eflips_eval-1.0.6/eflips/eval/input/prepare.py
+-rw-r--r--   0        0        0     1321 2024-05-29 13:52:34.479555 eflips_eval-1.0.6/eflips/eval/input/visualize.py
+-rw-r--r--   0        0        0        0 2024-05-29 13:52:34.479555 eflips_eval-1.0.6/eflips/eval/output/__init__.py
+-rw-r--r--   0        0        0    16194 2024-05-29 13:52:34.479555 eflips_eval-1.0.6/eflips/eval/output/prepare.py
+-rw-r--r--   0        0        0    10459 2024-05-29 13:52:34.479555 eflips_eval-1.0.6/eflips/eval/output/visualize.py
+-rw-r--r--   0        0        0      781 2024-05-29 13:52:34.499555 eflips_eval-1.0.6/pyproject.toml
+-rw-r--r--   0        0        0     5183 1970-01-01 00:00:00.000000 eflips_eval-1.0.6/PKG-INFO
```

### Comparing `eflips_eval-1.0.5/LICENSE.md` & `eflips_eval-1.0.6/LICENSE.md`

 * *Files identical despite different names*

### Comparing `eflips_eval-1.0.5/README.md` & `eflips_eval-1.0.6/README.md`

 * *Files identical despite different names*

### Comparing `eflips_eval-1.0.5/eflips/eval/input/prepare.py` & `eflips_eval-1.0.6/eflips/eval/input/prepare.py`

 * *Files identical despite different names*

### Comparing `eflips_eval-1.0.5/eflips/eval/input/visualize.py` & `eflips_eval-1.0.6/eflips/eval/input/visualize.py`

 * *Files identical despite different names*

### Comparing `eflips_eval-1.0.5/eflips/eval/output/prepare.py` & `eflips_eval-1.0.6/eflips/eval/output/prepare.py`

 * *Files identical despite different names*

### Comparing `eflips_eval-1.0.5/eflips/eval/output/visualize.py` & `eflips_eval-1.0.6/eflips/eval/output/visualize.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,19 +1,19 @@
 from datetime import datetime
-from typing import Dict, List, Optional, Tuple
+from typing import Dict, List, Tuple
 
 import pandas as pd
 import plotly.express as px  # type: ignore
 import plotly.graph_objs as go  # type: ignore
 from plotly.subplots import make_subplots  # type: ignore
 
 
 def get_color_scheme(
     color_scheme: str,
-) -> Dict[str, str | Dict[str, str] | str | px.colors.sequential]:
+) -> Dict[str, str | dict[str, str] | None]:
     """
     This function returns a dictionary with the color scheme to be used in the gantt chart
     :param color_scheme: A string representing the color scheme to be used in the gantt chart. It can be one of the following:
     - "event_type"
     - "soc"
     - "location"
     :return: A dictionary with the color scheme
@@ -233,15 +233,14 @@
     fig.update_layout(
         barmode="overlay",
         xaxis_title="Specific Energy Consumption (kWh/km)",
         yaxis_title="Count",
     )
     # Reduce opacity to see both histograms
     fig.update_traces(opacity=0.75)
-    fig.show()
     return fig
 
 
 def vehicle_soc(
     prepared_data: pd.DataFrame,
     descriptions: Dict[str, List[Tuple[str, datetime, datetime]]],
 ) -> go.Figure:
```

### Comparing `eflips_eval-1.0.5/pyproject.toml` & `eflips_eval-1.0.6/pyproject.toml`

 * *Files 15% similar despite different names*

```diff
@@ -1,22 +1,22 @@
 [tool.poetry]
 name = "eflips-eval"
-version = "1.0.5"
+version = "1.0.6"
 description = ""
 authors = [
     "Ludger Heide <ludger.heide@lhtechnologies.de>",
 	"Shuyao Guo <shuyao.guo@tu-berlin.de>"
 ]
 readme = "README.md"
 packages = [{ include = "eflips/eval" }]
 include= ["LICENSE.md"]
 
 
 [tool.poetry.dependencies]
-python = "^3.11"
+python = "^3.10"
 eflips-model = ">=2.3.0,<4.0.0"
 pandas = "^2.1.4"
 plotly = "^5.19.0"
 
 [tool.poetry.group.dev.dependencies]
 mypy = "^1.7.1"
 black = "^24.2.0"
```

### Comparing `eflips_eval-1.0.5/PKG-INFO` & `eflips_eval-1.0.6/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,15 +1,16 @@
 Metadata-Version: 2.1
 Name: eflips-eval
-Version: 1.0.5
+Version: 1.0.6
 Summary: 
 Author: Ludger Heide
 Author-email: ludger.heide@lhtechnologies.de
-Requires-Python: >=3.11,<4.0
+Requires-Python: >=3.10,<4.0
 Classifier: Programming Language :: Python :: 3
+Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: Python :: 3.12
 Requires-Dist: eflips-model (>=2.3.0,<4.0.0)
 Requires-Dist: pandas (>=2.1.4,<3.0.0)
 Requires-Dist: plotly (>=5.19.0,<6.0.0)
 Description-Content-Type: text/markdown
```

