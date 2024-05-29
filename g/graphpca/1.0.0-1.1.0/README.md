# Comparing `tmp/graphpca-1.0.0.tar.gz` & `tmp/graphpca-1.1.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/graphpca-1.0.0.tar", last modified: Sat Jun 27 00:55:21 2020, max compression
+gzip compressed data, was "graphpca-1.1.0.tar", last modified: Wed May 29 03:11:05 2024, max compression
```

## Comparing `graphpca-1.0.0.tar` & `graphpca-1.1.0.tar`

### file list

```diff
@@ -1,17 +1,17 @@
-drwxrwxr-x   0 brandon   (1000) brandon   (1000)        0 2020-06-27 00:55:21.000000 graphpca-1.0.0/
--rw-rw-r--   0 brandon   (1000) brandon   (1000)     1274 2020-06-18 16:00:59.000000 graphpca-1.0.0/README.rst
--rw-rw-r--   0 brandon   (1000) brandon   (1000)      641 2020-06-18 16:00:59.000000 graphpca-1.0.0/LICENSE
--rw-rw-r--   0 brandon   (1000) brandon   (1000)      959 2020-06-27 00:52:10.000000 graphpca-1.0.0/setup.py
--rw-rw-r--   0 brandon   (1000) brandon   (1000)      103 2020-06-27 00:55:21.000000 graphpca-1.0.0/setup.cfg
-drwxrwxr-x   0 brandon   (1000) brandon   (1000)        0 2020-06-27 00:55:21.000000 graphpca-1.0.0/graphpca.egg-info/
--rw-rw-r--   0 brandon   (1000) brandon   (1000)      251 2020-06-27 00:55:21.000000 graphpca-1.0.0/graphpca.egg-info/SOURCES.txt
--rw-rw-r--   0 brandon   (1000) brandon   (1000)     2227 2020-06-27 00:55:21.000000 graphpca-1.0.0/graphpca.egg-info/PKG-INFO
--rw-rw-r--   0 brandon   (1000) brandon   (1000)        9 2020-06-27 00:55:21.000000 graphpca-1.0.0/graphpca.egg-info/top_level.txt
--rw-rw-r--   0 brandon   (1000) brandon   (1000)        1 2020-06-27 00:55:21.000000 graphpca-1.0.0/graphpca.egg-info/dependency_links.txt
--rw-rw-r--   0 brandon   (1000) brandon   (1000)       21 2020-06-27 00:55:21.000000 graphpca-1.0.0/graphpca.egg-info/requires.txt
-drwxrwxr-x   0 brandon   (1000) brandon   (1000)        0 2020-06-27 00:55:21.000000 graphpca-1.0.0/test/
--rw-rw-r--   0 brandon   (1000) brandon   (1000)     5132 2020-06-27 00:20:36.000000 graphpca-1.0.0/test/test_graphpca.py
-drwxrwxr-x   0 brandon   (1000) brandon   (1000)        0 2020-06-27 00:55:21.000000 graphpca-1.0.0/graphpca/
--rw-rw-r--   0 brandon   (1000) brandon   (1000)    12561 2020-06-27 00:45:14.000000 graphpca-1.0.0/graphpca/__init__.py
--rw-rw-r--   0 brandon   (1000) brandon   (1000)     2227 2020-06-27 00:55:21.000000 graphpca-1.0.0/PKG-INFO
--rw-rw-r--   0 brandon   (1000) brandon   (1000)       21 2020-06-18 16:00:59.000000 graphpca-1.0.0/MANIFEST.in
+drwxrwxr-x   0 brandon   (1000) brandon   (1000)        0 2024-05-29 03:11:05.504213 graphpca-1.1.0/
+-rw-rw-r--   0 brandon   (1000) brandon   (1000)      641 2020-06-18 16:00:59.000000 graphpca-1.1.0/LICENSE
+-rw-rw-r--   0 brandon   (1000) brandon   (1000)       21 2020-06-18 16:00:59.000000 graphpca-1.1.0/MANIFEST.in
+-rw-rw-r--   0 brandon   (1000) brandon   (1000)     1855 2024-05-29 03:11:05.504213 graphpca-1.1.0/PKG-INFO
+-rw-rw-r--   0 brandon   (1000) brandon   (1000)     1303 2024-05-20 12:22:47.000000 graphpca-1.1.0/README.rst
+drwxrwxr-x   0 brandon   (1000) brandon   (1000)        0 2024-05-29 03:11:05.504213 graphpca-1.1.0/graphpca/
+-rw-rw-r--   0 brandon   (1000) brandon   (1000)    12541 2024-05-20 12:14:46.000000 graphpca-1.1.0/graphpca/__init__.py
+drwxrwxr-x   0 brandon   (1000) brandon   (1000)        0 2024-05-29 03:11:05.504213 graphpca-1.1.0/graphpca.egg-info/
+-rw-r--r--   0 brandon   (1000) brandon   (1000)     1855 2024-05-29 03:11:05.000000 graphpca-1.1.0/graphpca.egg-info/PKG-INFO
+-rw-rw-r--   0 brandon   (1000) brandon   (1000)      251 2024-05-29 03:11:05.000000 graphpca-1.1.0/graphpca.egg-info/SOURCES.txt
+-rw-rw-r--   0 brandon   (1000) brandon   (1000)        1 2024-05-29 03:11:05.000000 graphpca-1.1.0/graphpca.egg-info/dependency_links.txt
+-rw-rw-r--   0 brandon   (1000) brandon   (1000)       21 2024-05-29 03:11:05.000000 graphpca-1.1.0/graphpca.egg-info/requires.txt
+-rw-rw-r--   0 brandon   (1000) brandon   (1000)        9 2024-05-29 03:11:05.000000 graphpca-1.1.0/graphpca.egg-info/top_level.txt
+-rw-rw-r--   0 brandon   (1000) brandon   (1000)      103 2024-05-29 03:11:05.504213 graphpca-1.1.0/setup.cfg
+-rw-rw-r--   0 brandon   (1000) brandon   (1000)      959 2024-05-20 12:23:04.000000 graphpca-1.1.0/setup.py
+drwxrwxr-x   0 brandon   (1000) brandon   (1000)        0 2024-05-29 03:11:05.504213 graphpca-1.1.0/test/
+-rw-rw-r--   0 brandon   (1000) brandon   (1000)     5130 2024-05-20 12:16:55.000000 graphpca-1.1.0/test/test_graphpca.py
```

### filetype from file(1)

```diff
@@ -1 +1 @@
-POSIX tar archive (GNU)
+POSIX tar archive
```

### Comparing `graphpca-1.0.0/README.rst` & `graphpca-1.1.0/README.rst`

 * *Files 9% similar despite different names*

```diff
@@ -1,33 +1,35 @@
-graphpca
-===========
+GraphPCA
+========
 
 Produces a low-dimensional representation of the input graph.
 
 Calculates the ECTD [1]_ of the graph and reduces its dimension using PCA. The
 result is an embedding of the graph nodes as vectors in a low-dimensional
 space.
 
-Graph data in this repository is courtesy of the mind-blowingly cool
+Graph data in this repository is courtesy of
 `University of Florida Sparse Matrix Collection <https://www.cise.ufl.edu/research/sparse/matrices/>`_.
 
 Python 3.x and 2.6+.
 
+See the API docs: https://brandones.github.io/graphpca/
+
 Usage
 -----
 
 Draw a graph, including edges, from a mat file
 ::
 
     >>> import scipy.io
     >>> import networkx as nx
     >>> import graphpca
     >>> mat = scipy.io.loadmat('test/bcspwr01.mat')
     >>> A = mat['Problem'][0][0][1].todense()  # that's just how the file came
-    >>> G = nx.from_numpy_matrix(A)
+    >>> G = nx.from_numpy_array(A)
     >>> graphpca.draw_graph(G)
 
 .. image:: output/bcspwr01-drawing.png
 
 Get a 2D PCA of a high-dimensional graph and plot it.
 ::
```

### Comparing `graphpca-1.0.0/LICENSE` & `graphpca-1.1.0/LICENSE`

 * *Files identical despite different names*

### Comparing `graphpca-1.0.0/setup.py` & `graphpca-1.1.0/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -9,15 +9,15 @@
     """Build a file path from *paths* and return the contents."""
     with open(os.path.join(*paths), 'r') as f:
         return f.read()
 
 setup(
   name = 'graphpca',
   packages = ['graphpca'],
-  version = '1.0.0',
+  version = '1.1.0',
   license = 'Apache License 2.0',
   description = 'Produces a low-dimensional representation of the input graph',
   long_description=(read('README.rst')),
   long_description_content_type='text/x-rst',
   author = 'Brandon Istenes',
   author_email = 'brandonesbox@gmail.com',
   install_requires=[
```

### Comparing `graphpca-1.0.0/graphpca.egg-info/PKG-INFO` & `graphpca-1.1.0/PKG-INFO`

 * *Files 22% similar despite different names*

```diff
@@ -1,64 +1,66 @@
 Metadata-Version: 2.1
 Name: graphpca
-Version: 1.0.0
+Version: 1.1.0
 Summary: Produces a low-dimensional representation of the input graph
 Home-page: https://github.com/brandones/graphpca
+Download-URL: https://github.com/brandones/graphpca/tarball/0.5
 Author: Brandon Istenes
 Author-email: brandonesbox@gmail.com
 License: Apache License 2.0
-Download-URL: https://github.com/brandones/graphpca/tarball/0.5
-Description: graphpca
-        ===========
-        
-        Produces a low-dimensional representation of the input graph.
-        
-        Calculates the ECTD [1]_ of the graph and reduces its dimension using PCA. The
-        result is an embedding of the graph nodes as vectors in a low-dimensional
-        space.
-        
-        Graph data in this repository is courtesy of the mind-blowingly cool
-        `University of Florida Sparse Matrix Collection <https://www.cise.ufl.edu/research/sparse/matrices/>`_.
-        
-        Python 3.x and 2.6+.
-        
-        Usage
-        -----
-        
-        Draw a graph, including edges, from a mat file
-        ::
-        
-            >>> import scipy.io
-            >>> import networkx as nx
-            >>> import graphpca
-            >>> mat = scipy.io.loadmat('test/bcspwr01.mat')
-            >>> A = mat['Problem'][0][0][1].todense()  # that's just how the file came
-            >>> G = nx.from_numpy_matrix(A)
-            >>> graphpca.draw_graph(G)
-        
-        .. image:: output/bcspwr01-drawing.png
-        
-        Get a 2D PCA of a high-dimensional graph and plot it.
-        ::
-        
-            >>> import networkx as nx
-            >>> import graphpca
-            >>> g = nx.erdos_renyi_graph(1000, 0.2)
-            >>> g_2 = graphpca.reduce_graph(g, 2)
-            >>> graphca.plot_2d(g_2)
-        
-        .. image:: output/erg-1000.png
-        
-        
-        Contributing
-        ------------
-        
-        Issues and Pull requests are very welcome! [On GitHub](https://github.com/brandones/graphpca).
-        
-        .. [1] https://www.info.ucl.ac.be/~pdupont/pdupont/pdf/ecml04.pdf
-        
-        
 Keywords: graph,draw,pca,data,reduction,dimension,compression
-Platform: UNKNOWN
 Classifier: Development Status :: 4 - Beta
 Classifier: License :: OSI Approved :: Apache Software License
 Description-Content-Type: text/x-rst
+License-File: LICENSE
+
+GraphPCA
+========
+
+Produces a low-dimensional representation of the input graph.
+
+Calculates the ECTD [1]_ of the graph and reduces its dimension using PCA. The
+result is an embedding of the graph nodes as vectors in a low-dimensional
+space.
+
+Graph data in this repository is courtesy of
+`University of Florida Sparse Matrix Collection <https://www.cise.ufl.edu/research/sparse/matrices/>`_.
+
+Python 3.x and 2.6+.
+
+See the API docs: https://brandones.github.io/graphpca/
+
+Usage
+-----
+
+Draw a graph, including edges, from a mat file
+::
+
+    >>> import scipy.io
+    >>> import networkx as nx
+    >>> import graphpca
+    >>> mat = scipy.io.loadmat('test/bcspwr01.mat')
+    >>> A = mat['Problem'][0][0][1].todense()  # that's just how the file came
+    >>> G = nx.from_numpy_array(A)
+    >>> graphpca.draw_graph(G)
+
+.. image:: output/bcspwr01-drawing.png
+
+Get a 2D PCA of a high-dimensional graph and plot it.
+::
+
+    >>> import networkx as nx
+    >>> import graphpca
+    >>> g = nx.erdos_renyi_graph(1000, 0.2)
+    >>> g_2 = graphpca.reduce_graph(g, 2)
+    >>> graphca.plot_2d(g_2)
+
+.. image:: output/erg-1000.png
+
+
+Contributing
+------------
+
+Issues and Pull requests are very welcome! [On GitHub](https://github.com/brandones/graphpca).
+
+.. [1] https://www.info.ucl.ac.be/~pdupont/pdupont/pdf/ecml04.pdf
+
```

### Comparing `graphpca-1.0.0/test/test_graphpca.py` & `graphpca-1.1.0/test/test_graphpca.py`

 * *Files 2% similar despite different names*

```diff
@@ -61,15 +61,15 @@
         )
 
     def test_similar_output_to_naive_mat_3(self):
         mat = get_fixture_mat("bcspwr01.mat")
         # I love the UFSMC (https://www.cise.ufl.edu/research/sparse/matrices/)
         # but wow they really buried the matrix in this .mat
         A = mat["Problem"][0][0][1].todense()
-        G = nx.from_numpy_matrix(A)
+        G = nx.from_numpy_array(A)
         G3 = graphpca.reduce_graph_efficiently(G, 3)
         G3n = graphpca.reduce_graph_naively(G, 3)
         self.assertTrue(
             np.allclose(G3, G3n, rtol=1e-04, atol=1e-06),
             "Regular result:\n{}\nNaive result:\n{}\n".format(G3, G3n),
         )
 
@@ -90,15 +90,15 @@
             np.allclose(G2, G2n, rtol=1e-02, atol=1e-06),
             "Regular result:\n{}\nNaive result:\n{}\n".format(G2, G2n),
         )
 
     def test_add_supernode_similar_output_to_naive_mat_3(self):
         mat = get_fixture_mat("bcspwr01.mat")
         A = mat["Problem"][0][0][1].todense()
-        G = nx.from_numpy_matrix(A)
+        G = nx.from_numpy_array(A)
         G3 = graphpca.reduce_graph_efficiently(G, 3, add_supernode=True)
         G3n = graphpca.reduce_graph_naively(G, 3)
         self.assertTrue(
             np.allclose(G3, G3n, rtol=1e-02, atol=1e-06),
             "Regular result:\n{}\nNaive result:\n{}\n".format(G3, G3n),
         )
```

### Comparing `graphpca-1.0.0/graphpca/__init__.py` & `graphpca-1.1.0/graphpca/__init__.py`

 * *Files 0% similar despite different names*

```diff
@@ -4,15 +4,15 @@
 import logging
 
 import networkx as nx
 import numpy as np
 import scipy.io
 import scipy.linalg
 import scipy.sparse.linalg
-from scipy.sparse.linalg.eigen.arpack.arpack import ArpackNoConvergence
+from scipy.sparse.linalg import ArpackNoConvergence
 
 logging.basicConfig(level=logging.WARNING)
 LOG = logging.getLogger(__name__)
 
 
 def reduce_graph(nx_graph, output_dim):
     """
```

### Comparing `graphpca-1.0.0/PKG-INFO` & `graphpca-1.1.0/graphpca.egg-info/PKG-INFO`

 * *Files 22% similar despite different names*

```diff
@@ -1,64 +1,66 @@
 Metadata-Version: 2.1
 Name: graphpca
-Version: 1.0.0
+Version: 1.1.0
 Summary: Produces a low-dimensional representation of the input graph
 Home-page: https://github.com/brandones/graphpca
+Download-URL: https://github.com/brandones/graphpca/tarball/0.5
 Author: Brandon Istenes
 Author-email: brandonesbox@gmail.com
 License: Apache License 2.0
-Download-URL: https://github.com/brandones/graphpca/tarball/0.5
-Description: graphpca
-        ===========
-        
-        Produces a low-dimensional representation of the input graph.
-        
-        Calculates the ECTD [1]_ of the graph and reduces its dimension using PCA. The
-        result is an embedding of the graph nodes as vectors in a low-dimensional
-        space.
-        
-        Graph data in this repository is courtesy of the mind-blowingly cool
-        `University of Florida Sparse Matrix Collection <https://www.cise.ufl.edu/research/sparse/matrices/>`_.
-        
-        Python 3.x and 2.6+.
-        
-        Usage
-        -----
-        
-        Draw a graph, including edges, from a mat file
-        ::
-        
-            >>> import scipy.io
-            >>> import networkx as nx
-            >>> import graphpca
-            >>> mat = scipy.io.loadmat('test/bcspwr01.mat')
-            >>> A = mat['Problem'][0][0][1].todense()  # that's just how the file came
-            >>> G = nx.from_numpy_matrix(A)
-            >>> graphpca.draw_graph(G)
-        
-        .. image:: output/bcspwr01-drawing.png
-        
-        Get a 2D PCA of a high-dimensional graph and plot it.
-        ::
-        
-            >>> import networkx as nx
-            >>> import graphpca
-            >>> g = nx.erdos_renyi_graph(1000, 0.2)
-            >>> g_2 = graphpca.reduce_graph(g, 2)
-            >>> graphca.plot_2d(g_2)
-        
-        .. image:: output/erg-1000.png
-        
-        
-        Contributing
-        ------------
-        
-        Issues and Pull requests are very welcome! [On GitHub](https://github.com/brandones/graphpca).
-        
-        .. [1] https://www.info.ucl.ac.be/~pdupont/pdupont/pdf/ecml04.pdf
-        
-        
 Keywords: graph,draw,pca,data,reduction,dimension,compression
-Platform: UNKNOWN
 Classifier: Development Status :: 4 - Beta
 Classifier: License :: OSI Approved :: Apache Software License
 Description-Content-Type: text/x-rst
+License-File: LICENSE
+
+GraphPCA
+========
+
+Produces a low-dimensional representation of the input graph.
+
+Calculates the ECTD [1]_ of the graph and reduces its dimension using PCA. The
+result is an embedding of the graph nodes as vectors in a low-dimensional
+space.
+
+Graph data in this repository is courtesy of
+`University of Florida Sparse Matrix Collection <https://www.cise.ufl.edu/research/sparse/matrices/>`_.
+
+Python 3.x and 2.6+.
+
+See the API docs: https://brandones.github.io/graphpca/
+
+Usage
+-----
+
+Draw a graph, including edges, from a mat file
+::
+
+    >>> import scipy.io
+    >>> import networkx as nx
+    >>> import graphpca
+    >>> mat = scipy.io.loadmat('test/bcspwr01.mat')
+    >>> A = mat['Problem'][0][0][1].todense()  # that's just how the file came
+    >>> G = nx.from_numpy_array(A)
+    >>> graphpca.draw_graph(G)
+
+.. image:: output/bcspwr01-drawing.png
+
+Get a 2D PCA of a high-dimensional graph and plot it.
+::
+
+    >>> import networkx as nx
+    >>> import graphpca
+    >>> g = nx.erdos_renyi_graph(1000, 0.2)
+    >>> g_2 = graphpca.reduce_graph(g, 2)
+    >>> graphca.plot_2d(g_2)
+
+.. image:: output/erg-1000.png
+
+
+Contributing
+------------
+
+Issues and Pull requests are very welcome! [On GitHub](https://github.com/brandones/graphpca).
+
+.. [1] https://www.info.ucl.ac.be/~pdupont/pdupont/pdf/ecml04.pdf
+
```

