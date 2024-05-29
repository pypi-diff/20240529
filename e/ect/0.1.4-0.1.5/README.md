# Comparing `tmp/ect-0.1.4.tar.gz` & `tmp/ect-0.1.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ect-0.1.4.tar", last modified: Tue May 28 00:24:57 2024, max compression
+gzip compressed data, was "ect-0.1.5.tar", last modified: Wed May 29 02:54:57 2024, max compression
```

## Comparing `ect-0.1.4.tar` & `ect-0.1.5.tar`

### file list

```diff
@@ -1,22 +1,22 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-28 00:24:57.625856 ect-0.1.4/
--rw-r--r--   0 runner    (1001) docker     (127)    35149 2024-05-28 00:24:53.000000 ect-0.1.4/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)     2252 2024-05-28 00:24:57.625856 ect-0.1.4/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     1545 2024-05-28 00:24:53.000000 ect-0.1.4/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-28 00:24:57.621855 ect-0.1.4/ect/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-28 00:24:57.625856 ect-0.1.4/ect/ect.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     2252 2024-05-28 00:24:57.000000 ect-0.1.4/ect/ect.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      383 2024-05-28 00:24:57.000000 ect-0.1.4/ect/ect.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-28 00:24:57.000000 ect-0.1.4/ect/ect.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-28 00:24:57.000000 ect-0.1.4/ect/ect.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       14 2024-05-28 00:24:57.000000 ect-0.1.4/ect/ect.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-28 00:24:57.625856 ect-0.1.4/ect/ect_on_graphs/
--rw-r--r--   0 runner    (1001) docker     (127)      206 2024-05-28 00:24:53.000000 ect-0.1.4/ect/ect_on_graphs/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    14412 2024-05-28 00:24:53.000000 ect-0.1.4/ect/ect_on_graphs/ect_graph.py
--rw-r--r--   0 runner    (1001) docker     (127)     7352 2024-05-28 00:24:53.000000 ect-0.1.4/ect/ect_on_graphs/embed_cw.py
--rw-r--r--   0 runner    (1001) docker     (127)    11747 2024-05-28 00:24:53.000000 ect-0.1.4/ect/ect_on_graphs/embed_graph.py
--rw-r--r--   0 runner    (1001) docker     (127)      745 2024-05-28 00:24:53.000000 ect-0.1.4/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-28 00:24:57.625856 ect-0.1.4/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-28 00:24:57.625856 ect-0.1.4/tests/
--rw-r--r--   0 runner    (1001) docker     (127)     1761 2024-05-28 00:24:53.000000 ect-0.1.4/tests/test_ect_graph.py
--rw-r--r--   0 runner    (1001) docker     (127)     1225 2024-05-28 00:24:53.000000 ect-0.1.4/tests/test_embed_cw.py
--rw-r--r--   0 runner    (1001) docker     (127)     1768 2024-05-28 00:24:53.000000 ect-0.1.4/tests/test_embed_graph.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-29 02:54:57.589631 ect-0.1.5/
+-rw-r--r--   0 runner    (1001) docker     (127)    35149 2024-05-29 02:54:53.000000 ect-0.1.5/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)     2252 2024-05-29 02:54:57.585631 ect-0.1.5/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     1545 2024-05-29 02:54:53.000000 ect-0.1.5/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-29 02:54:57.585631 ect-0.1.5/ect/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-29 02:54:57.585631 ect-0.1.5/ect/ect/
+-rw-r--r--   0 runner    (1001) docker     (127)      225 2024-05-29 02:54:53.000000 ect-0.1.5/ect/ect/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    14398 2024-05-29 02:54:53.000000 ect-0.1.5/ect/ect/ect_graph.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7338 2024-05-29 02:54:53.000000 ect-0.1.5/ect/ect/embed_cw.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11747 2024-05-29 02:54:53.000000 ect-0.1.5/ect/ect/embed_graph.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-29 02:54:57.585631 ect-0.1.5/ect/ect.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     2252 2024-05-29 02:54:57.000000 ect-0.1.5/ect/ect.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      343 2024-05-29 02:54:57.000000 ect-0.1.5/ect/ect.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-29 02:54:57.000000 ect-0.1.5/ect/ect.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-29 02:54:57.000000 ect-0.1.5/ect/ect.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        4 2024-05-29 02:54:57.000000 ect-0.1.5/ect/ect.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      745 2024-05-29 02:54:53.000000 ect-0.1.5/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-29 02:54:57.589631 ect-0.1.5/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-29 02:54:57.585631 ect-0.1.5/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)     1747 2024-05-29 02:54:53.000000 ect-0.1.5/tests/test_ect_graph.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1225 2024-05-29 02:54:53.000000 ect-0.1.5/tests/test_embed_cw.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1754 2024-05-29 02:54:53.000000 ect-0.1.5/tests/test_embed_graph.py
```

### Comparing `ect-0.1.4/LICENSE` & `ect-0.1.5/LICENSE`

 * *Files identical despite different names*

### Comparing `ect-0.1.4/PKG-INFO` & `ect-0.1.5/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ect
-Version: 0.1.4
+Version: 0.1.5
 Summary: A python package for computing the Euler Characteristic Transform
 Author-email: Liz Munch <muncheli@msu.edu>
 Project-URL: Homepage, https://munchlab.github.io/ect
 Project-URL: Repository, https://github.com/MunchLab/ect
 Project-URL: Issues, https://github.com/MunchLab/ect/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: GNU General Public License v3 (GPLv3)
```

### Comparing `ect-0.1.4/README.md` & `ect-0.1.5/README.md`

 * *Files identical despite different names*

### Comparing `ect-0.1.4/ect/ect.egg-info/PKG-INFO` & `ect-0.1.5/ect/ect.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ect
-Version: 0.1.4
+Version: 0.1.5
 Summary: A python package for computing the Euler Characteristic Transform
 Author-email: Liz Munch <muncheli@msu.edu>
 Project-URL: Homepage, https://munchlab.github.io/ect
 Project-URL: Repository, https://github.com/MunchLab/ect
 Project-URL: Issues, https://github.com/MunchLab/ect/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: GNU General Public License v3 (GPLv3)
```

### Comparing `ect-0.1.4/ect/ect_on_graphs/ect_graph.py` & `ect-0.1.5/ect/ect/ect_graph.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 import numpy as np
 from itertools import compress, combinations
 from numba import jit
 import matplotlib.pyplot as plt
-from ect.ect_on_graphs.embed_cw import EmbeddedCW
+from ect.embed_cw import EmbeddedCW
 
 
 class ECT:
     """A class to calculate the Euler Characteristic Transform (ECT) from an input :any:`EmbeddedGraph` or :any:`EmbeddedCW`.
 
     The result is a matrix where entry ``M[i,j]`` is :math:`\chi(K_{a_i})` for the direction :math:`\omega_j` where :math:`a_i` is the ith entry in ``self.threshes``, and :math:`\omega_j` is the ith entry in ``self.thetas``.
```

### Comparing `ect-0.1.4/ect/ect_on_graphs/embed_cw.py` & `ect-0.1.5/ect/ect/embed_cw.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 import numpy as np
 from itertools import compress, combinations
 import matplotlib.pyplot as plt
 import networkx as nx
-from ect.ect_on_graphs.embed_graph import EmbeddedGraph, create_example_graph
+from ect.embed_graph import EmbeddedGraph, create_example_graph
 from scipy.optimize import linprog
 
 
 class EmbeddedCW(EmbeddedGraph):
     """
     A class to represent a straight-line-embedded CW complex. We assume that the coordinates for the embedding of the vertices are given, the 1-skeleton is in fact a graph (so not as general as a full CW complex) with straight line embeddings, and 2-Cells are the interior of the shape outlined by its boundary edges.
```

### Comparing `ect-0.1.4/ect/ect_on_graphs/embed_graph.py` & `ect-0.1.5/ect/ect/embed_graph.py`

 * *Files identical despite different names*

### Comparing `ect-0.1.4/pyproject.toml` & `ect-0.1.5/pyproject.toml`

 * *Files 15% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [project]
 name = "ect"
-version = "0.1.4"
+version = "0.1.5"
 authors = [
   { name="Liz Munch", email="muncheli@msu.edu" },
 ]
 description = "A python package for computing the Euler Characteristic Transform"
 readme = "README.md"
 requires-python = ">=3.8"
 classifiers = [
```

### Comparing `ect-0.1.4/tests/test_ect_graph.py` & `ect-0.1.5/tests/test_ect_graph.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 import unittest
-from ect.ect_on_graphs import embed_graph, ect_graph
+from ect import embed_graph, ect_graph
 
 
 
 class TestECT(unittest.TestCase):
     def test_example_graph_ect(self):
         G = embed_graph.create_example_graph()
         num_dirs = 8
```

### Comparing `ect-0.1.4/tests/test_embed_cw.py` & `ect-0.1.5/tests/test_embed_cw.py`

 * *Files identical despite different names*

### Comparing `ect-0.1.4/tests/test_embed_graph.py` & `ect-0.1.5/tests/test_embed_graph.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 import unittest
-from ect.ect_on_graphs import embed_graph
+from ect import embed_graph
 import numpy as np
 
 
 class TestEmbeddedGraph(unittest.TestCase):
     def test_example_graph(self):
         # Make sure we can build a grpah in the first place
         G = embed_graph.create_example_graph()
```

