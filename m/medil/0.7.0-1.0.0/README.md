# Comparing `tmp/medil-0.7.0.tar.gz` & `tmp/medil-1.0.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "medil-0.7.0.tar", last modified: Thu Oct 27 11:48:05 2022, max compression
+gzip compressed data, was "medil-1.0.0.tar", last modified: Wed May 29 12:19:13 2024, max compression
```

## Comparing `medil-0.7.0.tar` & `medil-1.0.0.tar`

### file list

```diff
@@ -1,23 +1,32 @@
-drwxr-xr-x   0 alex      (1000) alex      (1001)        0 2022-10-27 11:48:05.206721 medil-0.7.0/
--rw-r--r--   0 alex      (1000) alex      (1001)    24909 2022-10-18 13:22:15.000000 medil-0.7.0/LICENSE.txt
--rw-r--r--   0 alex      (1000) alex      (1001)     2575 2022-10-27 11:48:05.206721 medil-0.7.0/PKG-INFO
--rw-r--r--   0 alex      (1000) alex      (1001)     2030 2022-10-18 13:22:15.000000 medil-0.7.0/README.md
-drwxr-xr-x   0 alex      (1000) alex      (1001)        0 2022-10-27 11:48:05.206721 medil-0.7.0/medil/
--rw-r--r--   0 alex      (1000) alex      (1001)      132 2022-06-22 11:59:09.000000 medil-0.7.0/medil/__init__.py
--rw-r--r--   0 alex      (1000) alex      (1001)     3790 2022-10-18 13:16:41.000000 medil-0.7.0/medil/decomposable_score.py
--rw-r--r--   0 alex      (1000) alex      (1001)     5955 2022-06-22 11:59:09.000000 medil-0.7.0/medil/ecc_algorithms.py
--rw-r--r--   0 alex      (1000) alex      (1001)     2424 2022-06-22 11:59:09.000000 medil-0.7.0/medil/examples.py
--rw-r--r--   0 alex      (1000) alex      (1001)    10158 2022-06-22 11:59:09.000000 medil-0.7.0/medil/functional_MCM.py
--rw-r--r--   0 alex      (1000) alex      (1001)     9133 2022-10-18 13:16:41.000000 medil-0.7.0/medil/gauss_obs_l0_pen.py
--rw-r--r--   0 alex      (1000) alex      (1001)    15973 2022-07-14 19:42:15.000000 medil-0.7.0/medil/graph.py
--rw-r--r--   0 alex      (1000) alex      (1001)    20952 2022-10-18 13:16:41.000000 medil-0.7.0/medil/grues.py
--rw-r--r--   0 alex      (1000) alex      (1001)     7626 2022-10-27 11:42:36.000000 medil-0.7.0/medil/independence_testing.py
--rw-r--r--   0 alex      (1000) alex      (1001)     3162 2022-06-22 11:59:09.000000 medil-0.7.0/medil/visualize.py
-drwxr-xr-x   0 alex      (1000) alex      (1001)        0 2022-10-27 11:48:05.206721 medil-0.7.0/medil.egg-info/
--rw-r--r--   0 alex      (1000) alex      (1001)     2575 2022-10-27 11:48:05.000000 medil-0.7.0/medil.egg-info/PKG-INFO
--rw-r--r--   0 alex      (1000) alex      (1001)      391 2022-10-27 11:48:05.000000 medil-0.7.0/medil.egg-info/SOURCES.txt
--rw-r--r--   0 alex      (1000) alex      (1001)        1 2022-10-27 11:48:05.000000 medil-0.7.0/medil.egg-info/dependency_links.txt
--rw-r--r--   0 alex      (1000) alex      (1001)      109 2022-10-27 11:48:05.000000 medil-0.7.0/medil.egg-info/requires.txt
--rw-r--r--   0 alex      (1000) alex      (1001)        6 2022-10-27 11:48:05.000000 medil-0.7.0/medil.egg-info/top_level.txt
--rw-r--r--   0 alex      (1000) alex      (1001)       38 2022-10-27 11:48:05.206721 medil-0.7.0/setup.cfg
--rw-r--r--   0 alex      (1000) alex      (1001)      891 2022-10-18 13:22:15.000000 medil-0.7.0/setup.py
+drwxr-xr-x   0 alex      (1000) alex      (1001)        0 2024-05-29 12:19:13.799611 medil-1.0.0/
+-rw-r--r--   0 alex      (1000) alex      (1001)    34260 2023-10-05 16:01:24.000000 medil-1.0.0/LICENSE.md
+-rw-r--r--   0 alex      (1000) alex      (1001)     2268 2024-05-29 12:19:13.796278 medil-1.0.0/PKG-INFO
+-rw-r--r--   0 alex      (1000) alex      (1001)     1709 2024-05-29 06:42:58.000000 medil-1.0.0/README.md
+-rw-r--r--   0 alex      (1000) alex      (1001)     1781 2023-10-05 19:32:37.000000 medil-1.0.0/README.rst
+drwxr-xr-x   0 alex      (1000) alex      (1001)        0 2024-05-29 12:19:13.796278 medil-1.0.0/medil/
+-rw-r--r--   0 alex      (1000) alex      (1001)      190 2024-04-03 12:37:21.000000 medil-1.0.0/medil/__init__.py
+-rw-r--r--   0 alex      (1000) alex      (1001)     8266 2024-03-27 10:10:04.000000 medil-1.0.0/medil/ecc_algorithms.py
+-rw-r--r--   0 alex      (1000) alex      (1001)     1252 2023-10-05 18:25:44.000000 medil-1.0.0/medil/evaluate.py
+-rw-r--r--   0 alex      (1000) alex      (1001)     3030 2023-06-12 13:07:21.000000 medil-1.0.0/medil/examples.py
+-rw-r--r--   0 alex      (1000) alex      (1001)    16437 2023-10-05 18:15:08.000000 medil-1.0.0/medil/graph.py
+-rw-r--r--   0 alex      (1000) alex      (1001)     9126 2023-10-05 18:15:08.000000 medil-1.0.0/medil/independence_testing.py
+-rw-r--r--   0 alex      (1000) alex      (1001)    15698 2024-05-29 07:24:51.000000 medil-1.0.0/medil/models.py
+-rw-r--r--   0 alex      (1000) alex      (1001)     3607 2024-04-02 13:20:59.000000 medil-1.0.0/medil/sample.py
+-rw-r--r--   0 alex      (1000) alex      (1001)     3735 2024-05-28 09:48:40.000000 medil-1.0.0/medil/vae.py
+-rw-r--r--   0 alex      (1000) alex      (1001)     3155 2023-10-05 18:15:08.000000 medil-1.0.0/medil/visualize.py
+drwxr-xr-x   0 alex      (1000) alex      (1001)        0 2024-05-29 12:19:13.796278 medil-1.0.0/medil.egg-info/
+-rw-r--r--   0 alex      (1000) alex      (1001)     2268 2024-05-29 12:19:13.000000 medil-1.0.0/medil.egg-info/PKG-INFO
+-rw-r--r--   0 alex      (1000) alex      (1001)      529 2024-05-29 12:19:13.000000 medil-1.0.0/medil.egg-info/SOURCES.txt
+-rw-r--r--   0 alex      (1000) alex      (1001)        1 2024-05-29 12:19:13.000000 medil-1.0.0/medil.egg-info/dependency_links.txt
+-rw-r--r--   0 alex      (1000) alex      (1001)       66 2024-05-29 12:19:13.000000 medil-1.0.0/medil.egg-info/requires.txt
+-rw-r--r--   0 alex      (1000) alex      (1001)        6 2024-05-29 12:19:13.000000 medil-1.0.0/medil.egg-info/top_level.txt
+-rw-r--r--   0 alex      (1000) alex      (1001)       38 2024-05-29 12:19:13.799611 medil-1.0.0/setup.cfg
+-rw-r--r--   0 alex      (1000) alex      (1001)      762 2024-05-29 11:50:40.000000 medil-1.0.0/setup.py
+drwxr-xr-x   0 alex      (1000) alex      (1001)        0 2024-05-29 12:19:13.796278 medil-1.0.0/tests/
+-rw-r--r--   0 alex      (1000) alex      (1001)      578 2023-10-05 18:15:08.000000 medil-1.0.0/tests/test_evaluate.py
+-rw-r--r--   0 alex      (1000) alex      (1001)     1139 2023-10-05 18:33:38.000000 medil-1.0.0/tests/test_find_cm.py
+-rw-r--r--   0 alex      (1000) alex      (1001)     6118 2023-10-05 18:15:08.000000 medil-1.0.0/tests/test_graph.py
+-rw-r--r--   0 alex      (1000) alex      (1001)      111 2023-06-12 13:08:23.000000 medil-1.0.0/tests/test_indep_testing.py
+-rw-r--r--   0 alex      (1000) alex      (1001)     6546 2024-05-28 10:03:11.000000 medil-1.0.0/tests/test_models.py
+-rw-r--r--   0 alex      (1000) alex      (1001)     1279 2024-04-02 13:22:23.000000 medil-1.0.0/tests/test_sample.py
+-rw-r--r--   0 alex      (1000) alex      (1001)      236 2023-06-20 15:34:50.000000 medil-1.0.0/tests/test_simulate.py
```

### Comparing `medil-0.7.0/README.md` & `medil-1.0.0/PKG-INFO`

 * *Files 26% similar despite different names*

```diff
@@ -1,23 +1,38 @@
+Metadata-Version: 2.1
+Name: medil
+Version: 1.0.0
+Summary: MeDIL is a Python package for causal factor analysis with the (me)asurement (d)ependence (i)nducing (l)atent causal model framework.
+Author: Alex Markham
+Author-email: alex.markham@causal.dev
+License: GNU Affero General Public License version 3 or later (AGPLv3+)
+Description-Content-Type: text/markdown
+License-File: LICENSE.md
+Requires-Dist: dcor
+Requires-Dist: matplotlib
+Requires-Dist: networkx
+Requires-Dist: seaborn
+Requires-Dist: scikit-learn
+Requires-Dist: torch
+Requires-Dist: xicorrelation
+
 ## MeDIL
-MeDIL is a Python package for causal modeling, originally focusing on the measurement dependence inducing latent (MeDIL) causal model framework[<sup>1</sup>](#uai_paper), but now including more general methods for causal discovery and inference.
+MeDIL is a Python package for causal factor analysis, using the measurement dependence inducing latent (MeDIL) causal model framework[<sup>1</sup>](#medil_paper).
+In addition to simple linear Gaussian models, MeDIL also supports deep generative models[<sup>2</sup>](#ncfa_paper).
 
 More information can be found in the [documentation](https://medil.causal.dev).
 
 ### Support, Bugs, and Contributing
 If you have any questions, suggestions, feedback, or bugs to report, please [open an issue on Gitlab](https://gitlab.com/alex-markham/medil/issues/new) or [on Github](https://github.com/Alex-Markham/medil/issues/new) or [contact me](https://causal.dev/#contact).
-Additionally, if you would like to use this package or any of its code in your research, or to contribute to this package, feel free (but not obliged) to [contact me](https://causal.dev/#contact).
-
-### License
-See [LICENSE](https://gitlab.com/alex-markham/medil/blob/master/LICENSE.txt), which is the Cooperative Non-Violent Public License v7 or later (CNPLv7+).
 
-#### Brief License Summary (For Lay-People)
+Thanks to contributors [Aditya Chivukula](https://github.com/adityachivu/) and [Mingyu Liu](https://github.com/JerryLiuMY)!
 
-The Nonviolent Public License aims to ensure basic protections against forms of violence, coercion, and discrimination.
-This license covers several formats of creative work but has extra terms for software given the power it has as a tool outside of its creative capacities.
-The Cooperative Nonviolent Public License goes further to only allow commercial use of the copyrighted work for individuals and worker-owned organizations. 
+### License
+See [LICENSE](https://gitlab.com/alex-markham/medil/blob/master/LICENSE.md), which is the GNU Affero General Public License version 3 or later (AGPLv3+).
 
 ### Changelog
 See [CHANGELOG](https://gitlab.com/alex-markham/medil/blob/master/CHANGELOG.md) for a history of the already implemented features, works in progress, and future feature ideas.
 
 ### References
-<a name="uai_paper"> 1.</a> Markham, Alex & Grosse-Wentrup, Moritz. (2020). Measurement Dependence Inducing Latent Causal Models. In *Conference on Uncertainty in Artificial Intelligence (UAI)* PMLR 124:590&ndash;599. URL: [http://proceedings.mlr.press/v124/markham20a/markham20a.pdf](http://proceedings.mlr.press/v124/markham20a/markham20a.pdf)
+<a name="medil_paper"> 1.</a> Alex Markham & Moritz Grosse-Wentrup (2020). Measurement Dependence Inducing Latent Causal Models. In *Conference on Uncertainty in Artificial Intelligence (UAI)* PMLR 124:590&ndash;599. URL: [http://proceedings.mlr.press/v124/markham20a/markham20a.pdf](http://proceedings.mlr.press/v124/markham20a/markham20a.pdf).
+
+<a name="ncfa_paper"> 2.</a> Alex Markham, Mingyu Liu, Bryon Aragam, Liam Solus (2023). Neuro-Causal Factor Analysis. *prepint*. [arXiv:2305.19802](https://arxiv.org/abs/2305.19802) [stat.ML].
```

### Comparing `medil-0.7.0/medil/ecc_algorithms.py` & `medil-1.0.0/medil/ecc_algorithms.py`

 * *Files 26% similar despite different names*

```diff
@@ -1,151 +1,185 @@
 """Implementations of edge clique clover finding algorithms."""
-from .graph import UndirectedDependenceGraph
+import subprocess, os, shutil
+from collections import deque
+
 import numpy as np
 
+from .graph import UndirectedDependenceGraph
+
 
 def find_clique_min_cover(graph, verbose=False):
     """Returns the clique-minimum edge clique cover.
 
     Parameters
     ----------
-    graph : 2d numpy array 
+    graph : np.array
             Adjacency matrix for undirected graph.
 
     verbose : bool, optional
               Wether or not to print verbose output.
 
     Returns
     -------
-    the_cover : 2d numpy array
-                Biadjacency matrix representing edge clique cover.
+    the_cover: np.array
+               Biadjacency matrix representing edge clique cover.
 
     See Also
     --------
-    graph.UndirectedDependenceGraph : Defines auxilliary data structure 
+    graph.UndirectedDependenceGraph : Defines auxilliary data structure
                                       and reduction rules used by this
                                       algorithm.
 
     Notes
     -----
-    This is an implementation of the algorithm described in 
+    This is an implementation of the algorithm described in
     :cite:`Gramm_2009`.
 
     """
     graph = UndirectedDependenceGraph(graph, verbose)
     try:
         graph.make_aux()
     except ValueError:
         print("The input graph doesn't appear to have any edges!")
         return graph.adj_matrix
 
     num_cliques = 1
     the_cover = None
-    if True:# verbose:
+    if True:  # verbose:
         # find bound for cliques in solution
-        max_intersect_num = graph.num_vertices ** 2 // 4
+        max_intersect_num = graph.num_vertices**2 // 4
         if max_intersect_num < graph.num_edges:
             p = graph.n_choose_2(graph.num_vertices) - graph.num_edges
             t = int(np.sqrt(p))
             max_intersect_num = p + t if p > 0 else 1
         print("solution has at most {} cliques.".format(max_intersect_num))
     while the_cover is None:
-        if True:                # verbose:
-            print("\ntesting for solutions with {}/{} cliques".format(num_cliques, max_intersect_num))
-        the_cover = branch(graph, num_cliques, the_cover)
+        if True:  # verbose:
+            print(
+                "\ntesting for solutions with {}/{} cliques".format(
+                    num_cliques, max_intersect_num
+                )
+            )
+        the_cover = branch(graph, num_cliques, the_cover, iteration=0, iteration_max=3)
         num_cliques += 1
 
-    return the_cover
+    return add_isolated_verts(the_cover)
 
 
-def branch(graph, k_num_cliques, the_cover):
+def branch(graph, k_num_cliques, the_cover, iteration, iteration_max):
     """Helper function for `find_clique_min_cover()`.
 
-    Describing the solution search space as a tree, this function tests whether the given node is a solution, and it branches if not,
+    Describing the solution search space as a tree.
+    This function tests whether the given node is a solution, and it branches if not.
 
     Parameters
     ----------
     graph : UndirectedDependenceGraph()
             Class for representing undirected graph and auxilliary data used in edge clique cover algorithm.
 
     k_num_cliques : int
                     Current depth of search; number of cliques in cover being testet for solution.
 
-    the_cover : 2d numpy array
+    the_cover : np.array
                 Biadjacency matrix representing (possibly partial) edge clique cover.
 
+    iteration: current iteration
+
+    iteration_max: maximum number of iteration_max
+
     Returns
     -------
     2d numpy array or None
         Biadjacency matrix representing (complete) edge clique cover or None if cover is only partial.
 
     """
+
+    iteration = iteration + 1
     branch_graph = graph.reducible_copy()
     # if the_cover is not None:
     #     print(the_cover)
     #     for clique in the_cover:  # this might not be necessary, since the_cover_prime is only +1 clique
     #         print('clique: {}'.format(clique))
     #         branch_graph.the_cover = [clique]
     #         branch_graph.cover_edges()  # only works one clique at a time, or on a list of edges
     branch_graph.the_cover = the_cover
     branch_graph.cover_edges()
-    
+
     if branch_graph.num_edges == 0:
         return branch_graph.reconstruct_cover(the_cover)
 
     # branch_graph.the_cover = the_cover
 
     branch_graph.reduzieren(k_num_cliques)
     k_num_cliques = branch_graph.k_num_cliques
-    
+
     if k_num_cliques < 0:
         return None
 
     if branch_graph.num_edges == 0:  # equiv to len(branch_graph.extant_edges_idx)==0
-        return branch_graph.the_cover  # not in paper, but speeds it up slightly; or rather return None?
-    
+        return (
+            branch_graph.the_cover
+        )  # not in paper, but speeds it up slightly; or rather return None?
+
     chosen_nbrhood = branch_graph.choose_nbrhood()
     # print("num cliques: {}".format(len([x for x in max_cliques(chosen_nbrhood)])))
     for clique_nodes in max_cliques(chosen_nbrhood):
         if len(clique_nodes) == 1:  # then this vert has been rmed; quirk of max_cliques
             continue
         clique = np.zeros(branch_graph.unreduced.num_vertices, dtype=int)
         clique[clique_nodes] = 1
-        union = clique.reshape(1, -1) if branch_graph.the_cover is None else np.vstack((branch_graph.the_cover, clique))
-
-        the_cover_prime = branch(branch_graph, k_num_cliques-1, union)
+        union = (
+            clique.reshape(1, -1)
+            if branch_graph.the_cover is None
+            else np.vstack((branch_graph.the_cover, clique))
+        )
+
+        # print(iteration)
+        if iteration > iteration_max:
+            return branch_graph.the_cover
+
+        the_cover_prime = branch(
+            branch_graph,
+            k_num_cliques - 1,
+            union,
+            iteration,
+            iteration_max=iteration_max,
+        )
         if the_cover_prime is not None:
             return the_cover_prime
     return None
 
 
 def max_cliques(nbrhood):
     """Adaptation of NetworkX code for finding all maximal cliques.
 
     Parameters
     ----------
-    nbrhood : 2d numpy array
+    nbrhood : np.array
             Adjacency matrix for undirected (sub)graph.
 
     Returns
     -------
     generator
         set of all maximal cliques
 
     Notes
     -----
     Pieced together from nx.from_numpy_array and nx.find_cliques, which
     is output sensitive.
 
-    """    
+    """
+
     if len(nbrhood) == 0:
         return
-    
+
     # convert adjacency matrix to nx style graph
-    adj = {u: {v for v in np.nonzero(nbrhood[u])[0] if v != u} for u in range(len(nbrhood))}
+    adj = {
+        u: {v for v in np.nonzero(nbrhood[u])[0] if v != u} for u in range(len(nbrhood))
+    }
     Q = [None]
 
     subg = set(range(len(nbrhood)))
     cand = set(range(len(nbrhood)))
     u = max(subg, key=lambda u: len(cand & adj[u]))
     ext_u = cand - adj[u]
     stack = []
@@ -169,10 +203,66 @@
                         cand = cand_q
                         u = max(subg, key=lambda u: len(cand & adj[u]))
                         ext_u = cand - adj[u]
             else:
                 Q.pop()
                 subg, cand, ext_u = stack.pop()
     except IndexError:
-        pass    
+        pass
     # note: max_cliques is a generator, so it's consumed after being
     # looped through once
+
+
+def add_isolated_verts(cover):
+    cover = cover.astype(bool)
+    iso_vert_idx = np.flatnonzero(cover.sum(0) == 0)
+    num_rows = len(iso_vert_idx)
+    num_cols = cover.shape[1]
+    iso_vert_cover = np.zeros((num_rows, num_cols), bool)
+    iso_vert_cover[np.arange(num_rows), iso_vert_idx] = True
+    return np.vstack((cover, iso_vert_cover))
+
+
+def find_heuristic_1pc(graph):
+    num_meas = len(graph)
+
+    # nx_graph = nx.from_numpy_array(graph)
+    # indep_set =
+    # list(nx.approximation.maximum_independent_set(nx_graph))
+
+    indep_sets = max_cliques(np.logical_not(graph))
+    max_indep_set = next(indep_sets)
+    for indep_set in indep_sets:
+        if len(indep_set) > len(max_indep_set):
+            max_indep_set = indep_set
+
+    num_latents = len(max_indep_set)
+
+    the_cover = np.zeros((num_latents, num_meas), bool)
+    the_cover[np.arange(num_latents), max_indep_set] = True
+
+    for idx, node in enumerate(max_indep_set):
+        nbrs = np.flatnonzero(graph[node])
+        the_cover[idx, nbrs] = True
+
+    uncovered_edges = deque(
+        {
+            edge
+            for edge in np.argwhere(np.triu(graph, 1))
+            if not np.logical_and(the_cover[:, edge[0]], the_cover[:, edge[1]]).any()
+        }
+    )
+
+    while bool(uncovered_edges):
+        u, v = uncovered_edges.popleft()
+        if the_cover[:, u].any():
+            the_cover[np.argmax(the_cover[:, u]), v] = True
+        elif the_cover[:, v].any():
+            the_cover[np.argmax(the_cover[:, v]), u] = True
+        else:
+            uncovered_edges.append((u, v))
+
+    recon = the_cover.T @ the_cover
+    if np.logical_not(graph <= recon).any():
+        raise Exception(f"Problem with `find_hueristic_1pc()` for input {graph}")
+
+    return the_cover
```

### Comparing `medil-0.7.0/medil/examples.py` & `medil-1.0.0/medil/examples.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,60 +1,48 @@
 """Example graphs and data, for use in testing and tutorials."""
 import numpy as np
 
 
 class ExampleUDGAndMCM(object):
     r"""Example consisting of a description, UDG, and MCM"""
+
     def __init__(self, description):
         self.description = description
         self.UDG = None
         self.MCM = None
 
     def add_udg(self, udg):
         self.UDG = np.array(udg)
 
     def add_mcm(self, mcm):
         self.MCM = np.array(mcm)
 
 
 simple_M = ExampleUDGAndMCM("M-shaped mcm, with 2 latent- and 3 measurement-variables")
-simple_M.add_udg(
-    [
-        [1, 1, 0],
-        [1, 1, 1],
-        [0, 1, 1]
-    ]
-)
-simple_M.add_mcm(
-    [
-        [0, 1, 1],
-        [1, 1, 0]
-    ]
-)
+simple_M.add_udg([[1, 1, 0], [1, 1, 1], [0, 1, 1]])
+simple_M.add_mcm([[0, 1, 1], [1, 1, 0]])
 
-triangle = ExampleUDGAndMCM("triangle example, where minECC differs from set of all maximal cliques")
+triangle = ExampleUDGAndMCM(
+    "triangle example, where minECC differs from set of all maximal cliques"
+)
 triangle.add_udg(
     [
         [1, 1, 1, 0, 0, 0],
         [1, 1, 1, 1, 1, 0],
         [1, 1, 1, 0, 1, 1],
         [0, 1, 0, 1, 1, 0],
         [0, 1, 1, 1, 1, 1],
         [0, 0, 1, 0, 1, 1],
     ]
 )
-triangle.add_mcm(
-    [
-        [0, 0, 1, 0, 1, 1],
-        [0, 1, 0, 1, 1, 0],
-        [1, 1, 1, 0, 0, 0]
-    ]
-)
+triangle.add_mcm([[0, 0, 1, 0, 1, 1], [0, 1, 0, 1, 1, 0], [1, 1, 1, 0, 0, 0]])
 
-more_latents = ExampleUDGAndMCM("example where number of latent variables is larger than number of measurement variables")
+more_latents = ExampleUDGAndMCM(
+    "example where number of latent variables is larger than number of measurement variables"
+)
 more_latents.add_udg(
     [
         [1, 1, 0, 1, 0, 1],
         [1, 1, 1, 0, 1, 0],
         [0, 1, 1, 1, 0, 0],
         [1, 0, 1, 1, 1, 0],
         [0, 1, 0, 1, 1, 1],
@@ -70,15 +58,17 @@
         [0, 0, 0, 0, 1, 1],
         [1, 0, 0, 0, 0, 1],
         [1, 0, 0, 1, 0, 0],
         [0, 1, 0, 0, 1, 0],
     ]
 )
 
-am_cm_diff = ExampleUDGAndMCM("example where multiple ECCs are possible depending on edge minimal vs vertex minimal")
+am_cm_diff = ExampleUDGAndMCM(
+    "example where multiple ECCs are possible depending on edge minimal vs vertex minimal"
+)
 am_cm_diff.add_udg(
     [
         [1, 1, 1, 1, 1, 0, 1, 0],
         [1, 1, 1, 0, 1, 1, 1, 1],
         [1, 1, 1, 0, 1, 1, 1, 1],
         [1, 0, 0, 1, 0, 1, 1, 1],
         [1, 1, 1, 0, 1, 1, 0, 1],
@@ -93,12 +83,38 @@
         [1, 0, 0, 1, 0, 0, 1, 0],
         [0, 1, 1, 0, 1, 1, 0, 1],
         [0, 0, 0, 1, 0, 1, 0, 1],
         [0, 1, 1, 0, 0, 0, 1, 1],
     ]
 )
 
-examples = (simple_M, triangle, more_latents, am_cm_diff)
+max_assignment_num = ExampleUDGAndMCM(
+    "example where an edge has maximum assignment number, n - 2"
+)
+max_assignment_num.add_udg(
+    [
+        [1, 1, 1, 1, 1, 1, 1, 1],
+        [1, 1, 1, 1, 1, 1, 1, 1],
+        [1, 1, 1, 0, 0, 0, 0, 0],
+        [1, 1, 0, 1, 0, 0, 0, 0],
+        [1, 1, 0, 0, 1, 0, 0, 0],
+        [1, 1, 0, 0, 0, 1, 0, 0],
+        [1, 1, 0, 0, 0, 0, 1, 0],
+        [1, 1, 0, 0, 0, 0, 0, 1],
+    ]
+)
+max_assignment_num.add_mcm(
+    [
+        [1, 1, 1, 0, 0, 0, 0, 0],
+        [1, 1, 0, 1, 0, 0, 0, 0],
+        [1, 1, 0, 0, 1, 0, 0, 0],
+        [1, 1, 0, 0, 0, 1, 0, 0],
+        [1, 1, 0, 0, 0, 0, 1, 0],
+        [1, 1, 0, 0, 0, 0, 0, 1],
+    ]
+)
+
+examples = (simple_M, triangle, more_latents, am_cm_diff, max_assignment_num)
 
 
 ## Data
 # TODO: add linear and nonlinear data example
```

### Comparing `medil-0.7.0/medil/graph.py` & `medil-1.0.0/medil/graph.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,9 +1,10 @@
 """Various types and representations of graphs."""
 import numpy as np
+from numpy.random import default_rng
 
 
 class UndirectedDependenceGraph(object):
     r"""Adjacency matrix representation using a 2d numpy array.
 
     Upon initialization, this class is fairly standard implementation
     of an undirected graph. However, upon calling the :meth:`make_aux`
@@ -18,14 +19,18 @@
 
     Notes
     -----
     The algorithms for finding the minMCM via ECC contain many
     algebraic operations, so adjacency matrix representation (via
     NumPy) is most covenient.
 
+    The diag is used to store information when the graph is reduced,
+    not to indicate self loops, so it is important that diag = 1 at
+    init.
+
     """
 
     def __init__(self, adj_matrix, verbose=False):
         # doesn't behave well unless input is nparray
         self.adj_matrix = adj_matrix
         self.num_vertices = np.trace(adj_matrix)
         self.max_num_verts = len(adj_matrix)
@@ -119,14 +124,22 @@
     @staticmethod
     def n_choose_2(n):
         return n * (n - 1) // 2
 
     def reducible_copy(self):
         return ReducibleUndDepGraph(self)
 
+    def convert_to_nde(self, name="temp"):
+        with open(name + ".nde", "w") as f:
+            f.write(str(self.max_num_verts) + "\n")
+            for idx, node in enumerate(self.adj_matrix):
+                f.write(str(idx) + " " + str(node.sum()) + "\n")
+            for v1, v2 in np.argwhere(np.triu(self.adj_matrix)):
+                f.write(str(v1) + " " + str(v2) + "\n")
+
 
 class ReducibleUndDepGraph(UndirectedDependenceGraph):
     def __init__(self, udg):
         self.unreduced = udg.unreduced if hasattr(udg, "unreduced") else udg
         self.adj_matrix = udg.adj_matrix.copy()
         self.num_vertices = udg.num_vertices
         self.num_edges = udg.num_edges
@@ -379,13 +392,9 @@
                 np.logical_and(tiled_prisoners, the_cover).sum(1).astype(bool)
             )
             the_cover[cliques_to_update_mask, vert] = 1
 
         return the_cover
 
 
-# class minMCM(object):
-# TODO: implement as a bigraph with biadjacency matrix with rows M and cols L
-
-
 # class MCM(object):
 # TODO: implement as large DAG adj matrix over L and M, or smaller bigraph for L-M connections and DAG adj matirx for L->L connections
```

### Comparing `medil-0.7.0/medil/independence_testing.py` & `medil-1.0.0/medil/independence_testing.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,21 +1,24 @@
 """Independence testing on samples of random variables."""
 import numpy as np
-from scipy.spatial.distance import pdist, squareform, cdist
-from multiprocessing import Pool
+from scipy.spatial.distance import pdist, squareform
+from multiprocessing import Pool, cpu_count
+
 
 from numpy import linalg as LA
 from scipy.stats import chi2
 
 try:
+    from dcor.independence import distance_correlation_t_test
     from dcor import pairwise, distance_correlation as dist_corr
 
     default_measure = "dcor"
 except ImportError:
     default_measure = "pearson"
+from xicorrelation import xicorr
 
 
 def hypothesis_test(samples, num_resamples, measure=default_measure, alpha=0.05):
     r"""Performs random permutation tests to estimate independence and
     returns the estimated Undirected Dependency Graph in the form of an
     adjacency matrix.
 
@@ -96,15 +99,15 @@
     deps = p_values <= alpha  # reject null hypothesis of independence
 
     return p_values, sample_corr, deps
 
 
 def distance_correlation(samples, perm=False):
     r"""Compute distance correlation on samples set (or on permuted samples
-    set, if ``perm`` is ``True).
+    set, if ``perm`` is ``True``
 
     Parameters
     ----------
     samples : 2d numpy array of floats or ints
               A :math:`M \times N` matrix with :math:`N` samples of
               :math:`M` random variables.
 
@@ -136,15 +139,15 @@
         with Pool() as pool:
             corr = pairwise(dist_corr, samples_permed, samples_permed_2, pool=pool)
     return corr
 
 
 def pearson_correlation(samples, perm=False):
     r"""Computes Pearson product-moment correlation coefficient on samples
-    set (or on permuted samples set, if ``perm`` is ``True).
+    set (or on permuted samples set, if ``perm`` is ``True``).
 
     Parameters
     ----------
     samples : 2d numpy array of floats or ints
               A :math:`M \times N` matrix with :math:`N` samples of
               :math:`M` random variables.
 
@@ -191,36 +194,79 @@
 
     # apply the permutaton matrix to permute x
     return x[row_idx, col_idx]
 
 
 def dcov(samples):
     r"""Compute sample distance covariance matrix.
-
     Parameters
     ----------
     samples : 2d numpy array of floats
               A :math:`N \times M` matrix with :math:`N` samples of
               :math:`M` random variables.
-
     Returns
     -------
     2d numpy array
         A square matrix :math:`C`, where :math:`C_{i,j}` is the sample
         distance covariance between random variables :math:`R_i` and
         :math:`R_j`.
-
     """
     num_samps, num_feats = samples.shape
     num_pairs = num_samps * (num_samps - 1) // 2
     dists = np.zeros((num_feats, num_pairs))
+    d_bars = np.zeros(num_feats)
     # compute doubly centered distance matrix for every feature:
     for feat_idx in range(num_feats):
         n = num_samps
         t = np.tile
         # raw distance matrix:
         d = squareform(pdist(samples[:, feat_idx].reshape(-1, 1), "cityblock"))
         # doubly centered:
-        d -= t(d.mean(0), (n, 1)) + t(d.mean(1), (n, 1)).T - t(d.mean(), (n, n))
+        d_bar = d.mean()
+        d -= t(d.mean(0), (n, 1)) + t(d.mean(1), (n, 1)).T - t(d_bar, (n, n))
         d = squareform(d, checks=False)  # ignore assymmetry due to numerical error
         dists[feat_idx] = d
-    return dists @ dists.T / num_samps**2
+        d_bars[feat_idx] = d_bar
+    return dists @ dists.T / num_samps**2, d_bars
+
+
+def estimate_UDG(sample, method="dcov_fast", significance_level=0.05):
+    samp_size, num_feats = sample.shape
+
+    if isinstance(method, np.ndarray):
+        p_vals = method
+        udg = p_vals < significance_level
+    elif method == "dcov_fast":
+        cov, d_bars = dcov(sample)
+        crit_val = chi2(1).ppf(1 - significance_level)
+        test_val = samp_size * cov / np.outer(d_bars, d_bars)
+        udg = test_val >= crit_val
+        p_vals = None
+    elif method == "g-test":
+        pass
+    else:
+        p_vals = np.zeros((num_feats, num_feats), float)
+        idxs, jdxs = np.triu_indices(num_feats, 1)
+        zipped = zip(idxs, jdxs)
+        sample_iter = (sample[:, i_j].T for i_j in zipped)
+        if method == "dcov_big":
+            test = dcor_test
+        elif method == "xicor":
+            test = xicor_test
+        with Pool(max(1, int(0.75 * cpu_count()))) as p:
+            p_vals[idxs, jdxs] = p_vals[jdxs, idxs] = np.fromiter(
+                p.imap(test, sample_iter, 100), float
+            )
+            udg = p_vals < significance_level
+    np.fill_diagonal(udg, False)
+    return udg, p_vals
+
+
+def dcor_test(x_y):
+    x, y = x_y
+    return distance_correlation_t_test(x, y).pvalue
+
+
+def xicor_test(x_y):
+    x, y = x_y
+    xi, pvalue = xicorr(x, y)
+    return pvalue
```

### Comparing `medil-0.7.0/medil/visualize.py` & `medil-1.0.0/medil/visualize.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,17 +1,14 @@
 """ Create and display various graphs, plots, and visualizations."""
 import numpy as np
 import matplotlib.pyplot as plt
 import seaborn as sns
-
 import networkx as nx
 
 
-
-# %%
 def show_obs_adj_mat(incidence_mat):
 
     fig, ax = plt.subplots()
 
     adj_mat = get_adj_from_incidence(incidence_mat)
     plt.imshow(adj_mat)
```

