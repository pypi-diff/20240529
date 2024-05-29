# Comparing `tmp/cgt-0.3.1.tar.gz` & `tmp/cgt-0.4.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "cgt-0.3.1.tar", last modified: Sun Jun 25 12:21:18 2023, max compression
+gzip compressed data, was "cgt-0.4.0.tar", last modified: Wed May 29 03:10:07 2024, max compression
```

## Comparing `cgt-0.3.1.tar` & `cgt-0.4.0.tar`

### file list

```diff
@@ -1,34 +1,38 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-25 12:21:18.023588 cgt-0.3.1/
--rw-r--r--   0 runner    (1001) docker     (123)      828 2023-06-25 12:20:58.000000 cgt-0.3.1/CONTRIBUTING.md
--rw-r--r--   0 runner    (1001) docker     (123)     1689 2023-06-25 12:20:58.000000 cgt-0.3.1/INSTALL.md
--rw-r--r--   0 runner    (1001) docker     (123)    35149 2023-06-25 12:20:58.000000 cgt-0.3.1/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)       85 2023-06-25 12:20:58.000000 cgt-0.3.1/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)     1520 2023-06-25 12:21:18.023588 cgt-0.3.1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1070 2023-06-25 12:20:58.000000 cgt-0.3.1/README.md
--rw-r--r--   0 runner    (1001) docker     (123)        6 2023-06-25 12:20:58.000000 cgt-0.3.1/VERSION
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-25 12:21:18.023588 cgt-0.3.1/cgt/
--rw-r--r--   0 runner    (1001) docker     (123)      585 2023-06-25 12:20:58.000000 cgt-0.3.1/cgt/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    13338 2023-06-25 12:20:58.000000 cgt-0.3.1/cgt/distances.py
--rw-r--r--   0 runner    (1001) docker     (123)     1537 2023-06-25 12:20:58.000000 cgt-0.3.1/cgt/enums.py
--rw-r--r--   0 runner    (1001) docker     (123)      397 2023-06-25 12:20:58.000000 cgt-0.3.1/cgt/examples.py
--rw-r--r--   0 runner    (1001) docker     (123)      437 2023-06-25 12:20:58.000000 cgt-0.3.1/cgt/genome.py
--rw-r--r--   0 runner    (1001) docker     (123)    10024 2023-06-25 12:20:58.000000 cgt-0.3.1/cgt/hyperoctahedral.py
--rw-r--r--   0 runner    (1001) docker     (123)     4920 2023-06-25 12:20:58.000000 cgt-0.3.1/cgt/models.py
--rw-r--r--   0 runner    (1001) docker     (123)     3400 2023-06-25 12:20:58.000000 cgt-0.3.1/cgt/parsers.py
--rw-r--r--   0 runner    (1001) docker     (123)    20398 2023-06-25 12:20:58.000000 cgt-0.3.1/cgt/position_paradigm.py
--rw-r--r--   0 runner    (1001) docker     (123)     6267 2023-06-25 12:20:58.000000 cgt-0.3.1/cgt/rearrangements.py
--rw-r--r--   0 runner    (1001) docker     (123)     4865 2023-06-25 12:20:58.000000 cgt-0.3.1/cgt/simulations.py
--rw-r--r--   0 runner    (1001) docker     (123)      611 2023-06-25 12:20:58.000000 cgt-0.3.1/cgt/structures.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-25 12:21:18.023588 cgt-0.3.1/cgt/tests/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-25 12:20:58.000000 cgt-0.3.1/cgt/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      458 2023-06-25 12:20:58.000000 cgt-0.3.1/cgt/tests/test_conversions.py
--rw-r--r--   0 runner    (1001) docker     (123)     2735 2023-06-25 12:20:58.000000 cgt-0.3.1/cgt/visualisation.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-25 12:21:18.023588 cgt-0.3.1/cgt.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     1520 2023-06-25 12:21:17.000000 cgt-0.3.1/cgt.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      496 2023-06-25 12:21:18.000000 cgt-0.3.1/cgt.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-25 12:21:17.000000 cgt-0.3.1/cgt.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)        4 2023-06-25 12:21:17.000000 cgt-0.3.1/cgt.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)     2073 2023-06-25 12:20:58.000000 cgt-0.3.1/playground.py
--rw-r--r--   0 runner    (1001) docker     (123)     1291 2023-06-25 12:20:58.000000 cgt-0.3.1/playground_2.py
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-25 12:21:18.023588 cgt-0.3.1/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)      766 2023-06-25 12:20:58.000000 cgt-0.3.1/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-29 03:10:07.981596 cgt-0.4.0/
+-rw-r--r--   0 runner    (1001) docker     (127)      828 2024-05-29 03:10:02.000000 cgt-0.4.0/CONTRIBUTING.md
+-rw-r--r--   0 runner    (1001) docker     (127)     1689 2024-05-29 03:10:02.000000 cgt-0.4.0/INSTALL.md
+-rw-r--r--   0 runner    (1001) docker     (127)    35149 2024-05-29 03:10:02.000000 cgt-0.4.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)      101 2024-05-29 03:10:02.000000 cgt-0.4.0/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (127)     1520 2024-05-29 03:10:07.981596 cgt-0.4.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     1070 2024-05-29 03:10:02.000000 cgt-0.4.0/README.md
+-rw-r--r--   0 runner    (1001) docker     (127)        5 2024-05-29 03:10:02.000000 cgt-0.4.0/VERSION
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-29 03:10:07.981596 cgt-0.4.0/cgt/
+-rw-r--r--   0 runner    (1001) docker     (127)      685 2024-05-29 03:10:02.000000 cgt-0.4.0/cgt/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)       96 2024-05-29 03:10:02.000000 cgt-0.4.0/cgt/constants.py
+-rw-r--r--   0 runner    (1001) docker     (127)    23526 2024-05-29 03:10:02.000000 cgt-0.4.0/cgt/distances.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2889 2024-05-29 03:10:02.000000 cgt-0.4.0/cgt/enums.py
+-rw-r--r--   0 runner    (1001) docker     (127)      397 2024-05-29 03:10:02.000000 cgt-0.4.0/cgt/examples.py
+-rw-r--r--   0 runner    (1001) docker     (127)      442 2024-05-29 03:10:02.000000 cgt-0.4.0/cgt/genome.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11595 2024-05-29 03:10:02.000000 cgt-0.4.0/cgt/hyperoctahedral.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7342 2024-05-29 03:10:02.000000 cgt-0.4.0/cgt/models.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3400 2024-05-29 03:10:02.000000 cgt-0.4.0/cgt/parsers.py
+-rw-r--r--   0 runner    (1001) docker     (127)      466 2024-05-29 03:10:02.000000 cgt-0.4.0/cgt/pickle_manager.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3000 2024-05-29 03:10:02.000000 cgt-0.4.0/cgt/plotting.py
+-rw-r--r--   0 runner    (1001) docker     (127)    24864 2024-05-29 03:10:02.000000 cgt-0.4.0/cgt/position_paradigm.py
+-rw-r--r--   0 runner    (1001) docker     (127)    15821 2024-05-29 03:10:02.000000 cgt-0.4.0/cgt/rearrangements.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5305 2024-05-29 03:10:02.000000 cgt-0.4.0/cgt/simulations.py
+-rw-r--r--   0 runner    (1001) docker     (127)       49 2024-05-29 03:10:02.000000 cgt-0.4.0/cgt/sorting.py
+-rw-r--r--   0 runner    (1001) docker     (127)      636 2024-05-29 03:10:02.000000 cgt-0.4.0/cgt/structures.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-29 03:10:07.981596 cgt-0.4.0/cgt/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-29 03:10:02.000000 cgt-0.4.0/cgt/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      595 2024-05-29 03:10:02.000000 cgt-0.4.0/cgt/tests/test_conversions.py
+-rw-r--r--   0 runner    (1001) docker     (127)      737 2024-05-29 03:10:02.000000 cgt-0.4.0/cgt/tests/test_hyperoctahedral.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1367 2024-05-29 03:10:02.000000 cgt-0.4.0/cgt/tests/test_min_distances.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3081 2024-05-29 03:10:02.000000 cgt-0.4.0/cgt/visualisation.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-29 03:10:07.981596 cgt-0.4.0/cgt.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     1520 2024-05-29 03:10:07.000000 cgt-0.4.0/cgt.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      602 2024-05-29 03:10:07.000000 cgt-0.4.0/cgt.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-29 03:10:07.000000 cgt-0.4.0/cgt.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        4 2024-05-29 03:10:07.000000 cgt-0.4.0/cgt.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-29 03:10:07.981596 cgt-0.4.0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)      837 2024-05-29 03:10:02.000000 cgt-0.4.0/setup.py
```

### Comparing `cgt-0.3.1/CONTRIBUTING.md` & `cgt-0.4.0/CONTRIBUTING.md`

 * *Files identical despite different names*

### Comparing `cgt-0.3.1/INSTALL.md` & `cgt-0.4.0/INSTALL.md`

 * *Files identical despite different names*

### Comparing `cgt-0.3.1/LICENSE` & `cgt-0.4.0/LICENSE`

 * *Files identical despite different names*

### Comparing `cgt-0.3.1/PKG-INFO` & `cgt-0.4.0/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: cgt
-Version: 0.3.1
+Version: 0.4.0
 Summary: Tools for representing genomes in sage
 Home-page: https://github.com/js51/Circular-genome-tools
 Author: Joshua Stevenson
 Author-email: joshua.stevenson@utas.edu.au
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

### Comparing `cgt-0.3.1/README.md` & `cgt-0.4.0/README.md`

 * *Files identical despite different names*

### Comparing `cgt-0.3.1/cgt/__init__.py` & `cgt-0.4.0/cgt/__init__.py`

 * *Files 25% similar despite different names*

```diff
@@ -10,9 +10,12 @@
     gap._Expect__command = gap._Expect__command.replace(gap._Expect__command[s:e], f'-o {gigs}G')
 except ValueError:
     s = old_command.index('-b ')
     e = old_command.index(' -', s)
     gap._Expect__command = gap._Expect__command.replace(gap._Expect__command[s:e], f'-b -o {gigs}G')
 from .examples import *
 from .enums import *
-from .position_paradigm import PositionParadigmFramework
-from .models import Model
+from .constants import *
+from .position_paradigm import GenomeFramework, PositionParadigmFramework, Framework
+from .models import Model
+from . import distances
+from . import plotting
```

### Comparing `cgt-0.3.1/cgt/hyperoctahedral.py` & `cgt-0.4.0/cgt/hyperoctahedral.py`

 * *Files 13% similar despite different names*

```diff
@@ -1,92 +1,104 @@
 """
 This file contains the class for the hyperoctahedral group.
 """
+
 # %%
 from cgt import structures
+import sage
+import numpy as np
 from sage.all_cmdline import (
     SymmetricGroup,
     cartesian_product,
     GroupSemidirectProduct,
     SymmetricGroupRepresentation,
     SignedPermutations,
     matrix,
     block_matrix,
     Partitions,
-    Permutation
+    Permutation,
 )
 
 
 def HyperoctahedralGroupRepresentations(n):
     """
     This function returns the irreducible representations of the hyperoctahedral group of order 2^n * n!, indexed by pairs of partitions of l and m, where l + m = n.
 
     Args:
         n (int): The order of the hyperoctahedral group.
-    
+
     Returns:
         dict: A dictionary of the irreducible representations of the hyperoctahedral group of order 2^n * n!
     """
     irreps = {}
-    Hn = hyperoctahedral_group(n)
+    Hn = HyperoctahedralGroup(n)
     for little_subgroup_pair in Hn.little_subgroup_pairs():
         for partition_left in Partitions(little_subgroup_pair[0]):
             for partition_right in Partitions(little_subgroup_pair[1]):
                 partition_pair = (partition_left, partition_right)
                 irrep = Hn.irrep(partition_pair)
+
                 def wrapped_irrep(elt, _irrep=irrep):
-                    return _irrep(Hn.Phi_inv(elt))
+                    return _irrep(Hn.Phi(elt))
+
                 irreps[partition_pair] = wrapped_irrep
     return irreps
 
-class hyperoctahedral_group:
+
+class HyperoctahedralGroup:
     """
     This class represents the hyperoctahedral group of order 2^n * n!. It stores the group as a number of different isomorphic structures, as well as a number of other things that are helpful to keep track of in the context of genome rearrangements. It implements functions to compute the irreducible representations of the hyperoctahedral group.
     """
-    _n = None
-    _sage_signed_perms = None
-    _signed_perms = None
-    _subgroup_of_s2n = None
-    _semidirect_product = None
-    _Sn = None
-    _C2 = None
-    _C2n = None
-    _twist = None
 
     def __init__(self, n, default_element_type="signed_permutation"):
         """
         Args:
             n (int): The order of the hyperoctahedral group.
             default_element_type (str, optional): The type of element to use when generating random elements. Defaults to "signed_permutation".
         """
         self._n = n
-        self._singned_perms = structures.HyperoctahedralGroup(self._n)
+        self._signed_perms = structures.HyperoctahedralGroup(self._n)
         self._sage_signed_perms = SignedPermutations(self._n)
         self._Sn = SymmetricGroup(self._n)
         self._C2 = SymmetricGroup(2)
+        self._N = self._signed_perms.subgroup(
+            [self._signed_perms((i, -i)) for i in range(1, self._n + 1)]
+        )
+        self._Sn_in_Hn = self._signed_perms.subgroup(
+            [
+                self._signed_perms(
+                    f'({",".join(str(x) for x in range(1,n+1))})({",".join(str(-x) for x in range(1,n+1))})'
+                ),
+                self._signed_perms(f"(1,2)(-1,-2)"),
+            ]
+        )
+        self._Sn_wr_N = GroupSemidirectProduct(self._Sn_in_Hn, self._N)
         self._C2n = cartesian_product(tuple(SymmetricGroup(2) for _ in range(self._n)))
-        self._semidirect_product = self.semidirect_product_with_hyperoctahedral_twist(self._C2n, self._Sn)
+        self._semidirect_product = self.semidirect_product_with_hyperoctahedral_twist(
+            self._Sn, self._C2n
+        )
 
     def hyperoctahedral_twist(self, s, c):
         """
         This function implements the twist of the hyperoctahedral group, which is the action of S_n on (C_2)^n by permuting the factors.
 
         Args:
             s (Permutation): A permutation in S_n.
             c (tuple): A tuple of elements of C_2.
-        
+
         Returns:
             an element of (C_2)^n: The tuple of elements of C_2 obtained by applying s to the tuple c.
         """
         try:
             _ = len(s)  # works if it is a "tuple"
         except:
-            pass
-        else:
-            s = self._Sn(s[0]) * self._Sn(s[1])
+            pass  # We have the usual hyperoctahedral group
+        else:  # We have a wreath product of a little subgroup (as a direct product)
+            #s = self._Sn(s[0]) * self._Sn(s[1])
+            raise ValueError("This is not implemented yet")
         return self._C2n((c[s(k) - 1] for k in range(1, self._n + 1)))
 
     def orbit_representative(self, l, m):
         return self._C2n(tuple(() for _ in range(l)) + tuple((1, 2) for _ in range(m)))
 
     def little_subgroup_pairs(self):
         return tuple((l, self._n - l) for l in range(self._n + 1))
@@ -106,78 +118,91 @@
     def little_subgroup_pairs(self):
         return [(l, self._n - l) for l in range(self._n + 1)]
 
     def little_subgroups(self):
         return [
             self.little_subgroup(l, m) for l, m in self.little_subgroup_pairs(self._n)
         ]
-    
+
     def orbit_representative(self, l, m):
         return self._C2n(tuple(() for _ in range(l)) + tuple((1, 2) for _ in range(m)))
-    
+
     def character_for_tuple(self, c):
         return tuple(
-            (lambda x: 1) if entry == self._C2(()) else (lambda x: x.sign()) for entry in c
+            (lambda x: 1) if entry == self._C2(()) else (lambda x: x.sign())
+            for entry in c
         )
 
     def representation_little_subgroup(self, partition_pair):
         rep_left = SymmetricGroupRepresentation(partition_pair[0])
         rep_right = SymmetricGroupRepresentation(partition_pair[1])
         l, m = sum([0] + list(partition_pair[0])), sum([0] + list(partition_pair[1]))
         n = l + m
         left_group = SymmetricGroup(l)
         right_group = SymmetricGroup(m)
         c = self.orbit_representative(l, m)
         x = self.character_for_tuple(c)
 
         def rep(g):
             try:
-                _ = len(g[1])  # works if it is a "tuple"
-            except:  # g[1] is not a "tuple" of permutations
-                g = (g[0], self.element_in_little_subgroup(g[1], l, m))
-            prod = rep_left(g[1][0]).tensor_product(rep_right(g[1][1]))
-            character = (x[i](ci) for i, ci in enumerate(g[0]))
+                _ = len(g[0])  # works if it is a "tuple"
+            except:  # g[0] is not a "tuple" of permutations
+                g = (self.element_in_little_subgroup(g[0], l, m), g[1])
+            prod = rep_left(g[0][0]).tensor_product(rep_right(g[0][1]))
+            character = (x[i](ci) for i, ci in enumerate(g[1]))
             coeff = 1
             for char in character:
                 coeff *= char
             return coeff * prod
 
         return rep
 
+
+    def _elt_in_subgroup(self, elt, l):
+        return all(
+            (
+                all(int(x) <= l for x in str(cycle).strip("()").split(","))
+                or all(int(x) > l for x in str(cycle).strip("()").split(","))
+            )
+            for cycle in elt
+        )
+
     def irrep(self, partition_pair):
         """
         Returns the irreducible representation of the hyperoctahedral group of order 2^n * n! indexed by the pair of partitions of l and m where l + m = n. The representation is given as a function that takes an element of the hyperoctahedral group as input and returns the corresponding matrix.
 
         Args:
             partition_pair (tuple): A pair of partitions of l and m where l + m = n.
-        
+
         Returns:
             function (group element -> real matrix): A function that takes an element of the hyperoctahedral group as input and returns the corresponding matrix.
         """
         rep = self.representation_little_subgroup(partition_pair)
         l, m = sum([0] + list(partition_pair[0])), sum([0] + list(partition_pair[1]))
         subgroup = self.little_subgroup(l, m)
         C2n_wr_SlxSm = self.semidirect_product_with_hyperoctahedral_twist(
-            self._C2n, subgroup
+            subgroup, self._C2n
         )
-        tv = self.right_transversal(self._semidirect_product, C2n_wr_SlxSm)
+        tv = self.right_transversal_of_little_subgroup(l)
+        id_rep = rep(C2n_wr_SlxSm.one())
+        rep_dimension = (id_rep.nrows(), id_rep.ncols())
 
         def _irrep(g):
-            id_rep = rep(C2n_wr_SlxSm.one())
-            rep_dimension = (id_rep.nrows(), id_rep.ncols())
             Y = [[None for _ in range(len(tv))] for _ in range(len(tv))]
-            for r in range(len(tv)):
-                for l in range(len(tv)):
-                    element = tv[l] * g * tv[r].inverse()
-                    if element in C2n_wr_SlxSm:
-                        Y[r][l] = rep(element)
+            for row in range(len(tv)):
+                element_part = g * tv[row].inverse()
+                for col in range(len(tv)):
+                    element = tv[col] * element_part
+                    if self._elt_in_subgroup(element[0], l):
+                        Y[row][col] = np.array(rep(element), dtype=object)
                     else:  # A matrix of zeros
-                        Y[r][l] = matrix(*rep_dimension)
-            return block_matrix(Y, subdivide=False)
-        
+                        Y[row][col] = np.zeros(rep_dimension, dtype=sage.rings.rational.Rational)
+
+            return matrix(np.block(Y))
+
         return _irrep
 
     def element_in_little_subgroup(self, elt, l, m):
         """
         Takes elt as an element of the little subgroup of Sn of order l!m! and returns an element of the direct product of S_l and S_m.
         """
         Sl = SymmetricGroup(l)
@@ -192,38 +217,38 @@
             else:
                 string = str(cycle)
                 for new, old in enumerate(range(l + 1, self._n + 1)):
                     string = string.replace(str(old), str(new + 1))
                 right *= Sm(string)
         return SlxSm((left, right))
 
-    def semidirect_product_with_hyperoctahedral_twist(self, H, G):
+    def semidirect_product_with_hyperoctahedral_twist(self, G, N):
         """
         Compute a semi-direct product of H and G with the hyperoctahedral twist (G acts on H^n by permuting factors). The group returned is a group of pairs (c, s) where c is an element of H^n and s is an element of G. The group operation is given by (c1, s1) * (c2, s2) = (c1 * s1(c2), s1 * s2).
 
         Args:
             H (group): the direct product of n copies of some group.
             G (group): A group.
-        
+
         Returns:
             group: The wreath product of H and G with the hyperoctahedral twist.
         """
         semidirect_product = GroupSemidirectProduct(
-            H, G, act_to_right=False, twist=lambda s, c: self.hyperoctahedral_twist(s, c)
+            G, N, act_to_right=True, twist=lambda s, c: self.hyperoctahedral_twist(s, c)
         )
 
         def random_element():
-            C, Sn = semidirect_product.cartesian_factors()
-            return semidirect_product((C.random_element(), Sn.random_element()))
+            Sn, C = semidirect_product.cartesian_factors()
+            return semidirect_product((Sn.random_element(), C.random_element()))
 
         def order():
-            return H.order() * G.order()
+            return G.order() * N.order()
 
         def elements():
-            return [semidirect_product((c, s)) for c in H for s in G]
+            return [semidirect_product((s, c)) for c in N for s in G]
 
         semidirect_product.random_element = random_element
         semidirect_product.action = self.hyperoctahedral_twist
         semidirect_product.order = order
         semidirect_product.elements = elements
         return semidirect_product
 
@@ -231,13 +256,34 @@
         transversal = [subgroup.one()]
         num_cosets = group.order() / subgroup.order()
         while len(transversal) < num_cosets:
             elt = group.random_element()
             if all(t * elt.inverse() not in subgroup for t in transversal):
                 transversal.append(elt)
         return transversal
-    
-    def Phi_inv(self, elt):
-        c = tuple(self._C2(() if elt(k) > 0 else (1, 2)) for k in range(1, self._n + 1))
+
+    def right_transversal_of_little_subgroup(self, k):
+        from itertools import combinations
+
+        n = self._n
+        H = self
+        combs = list(combinations(tuple((i for i in range(1, n + 1))), k))
+        t_new = []
+        for comb in combs:
+            sets = ((i for i in range(1, k + 1)), (i for i in range(k + 1, n + 1)))
+            elt = Permutation(
+                [next(sets[0]) if i in comb else next(sets[1]) for i in range(1, n + 1)]
+            )
+            t_new.append(
+                H._semidirect_product(
+                    (H._Sn(elt.cycle_string()), (() for _ in range(n)))
+                ).inverse()
+            )
+        return t_new
+
+    def Phi(self, elt):
+        c = tuple(self._C2(() if elt.inverse()(k) > 0 else (1, 2)) for k in range(1, self._n + 1))
         s = self._Sn(Permutation([abs(elt(k)) for k in range(1, self._n + 1)]))
-        return self._semidirect_product((c, s))
+        return self._semidirect_product((s, c))
+
+
 # %%
```

### Comparing `cgt-0.3.1/cgt/parsers.py` & `cgt-0.4.0/cgt/parsers.py`

 * *Files identical despite different names*

### Comparing `cgt-0.3.1/cgt/position_paradigm.py` & `cgt-0.4.0/cgt/position_paradigm.py`

 * *Files 13% similar despite different names*

```diff
@@ -1,36 +1,39 @@
 """
 position_paradigm is the most important module in cgt. PositionParadigmFramework keeps track of important objects, can
 convert group elements and genomes between different forms, and instances can be passed to functions from other modules so
 that they can acces information without it needing to be recreated.
 """
 
-from sage.all_cmdline import QQ, FormalSum, SymmetricGroup, SymmetricGroupRepresentations, gap, UniversalCyclotomicField, Permutations, matrix, QQbar
+from sage.all_cmdline import QQ, FormalSum, SymmetricGroup, SymmetricGroupRepresentations, gap, Permutations, matrix, QQbar
 from sage.combinat.colored_permutations import SignedPermutations
 from .enums import *
 import numpy as np
 import warnings
 from copy import deepcopy
 from .structures import HyperoctahedralGroup
 from scipy.sparse import dok_matrix as dok
 from random import choice
 from .hyperoctahedral import HyperoctahedralGroupRepresentations
 
+
 class PositionParadigmFramework:
     """Everything you need for working with genomes under the position paradigm"""
 
-    def __init__(self, num_regions, oriented=True, symmetry=SYMMETRY.circular, genome_type=TYPE.reg_to_signed_pos):
+    def __init__(self, num_regions, oriented=True, symmetry=SYMMETRY.circular, genome_type=TYPE.reg_to_signed_pos, precompute_irreps=False):
         """Instantiate a system of position paradigm genomes with given set of symmetries and number of regions."""
         if genome_type != TYPE.reg_to_signed_pos:
             raise NotImplementedError("Genome type not yet supported. For now use TYPE.reg_to_signed_pos")
         self.n = num_regions
         self.oriented = oriented
         self.symmetry = symmetry
         self.representations = None
         self._genomes = None
+        if precompute_irreps:
+            _ = self.irreps() # gets cached
         
     def __eq__(self, other): # String representation is unique and repr calls str
         return self.__repr__() == other.__repr__()
 
     def __str__(self):
         string = f"Framework for {str(self.symmetry).replace('SYMMETRY.', '')} genomes"
         string += f" with {self.n}{' oriented' if self.oriented else ''} regions"
@@ -112,36 +115,40 @@
 
         Examples:
             sage: import cgt; ppf = cgt.PositionParadigmFramework(3, symmetry=cgt.SYMMETRY.circular)
             sage: ppf.canonical_instance('(1,-2)(-1,2)')
             [1, 2, -3]
         """
         try:
-            instance = self.cycles(deepcopy(instance))
+            instance = self.cycles(deepcopy(self.one_row(instance)))
         except:
             # Probably accidentally given a genome instead of an instance
             instance = self.instances(instance)[0]
         instance = deepcopy(self.one_row(self.cycles(instance)))
         if self.symmetry in {SYMMETRY.circular, SYMMETRY.linear}:
             f = self.one_row(self.standard_reflection())
             if list(instance)[0] < 0:
-                instance = instance*f
+                instance = instance * f
             if self.symmetry is SYMMETRY.circular:
                 r = self.one_row(self.standard_rotation())
-                instance = instance*(r**((self.n-list(instance)[0]+1)%self.n))
+                instance = instance * (r ** ((self.n - list(instance)[0] + 1) % self.n))
             return instance
         else:
             raise NotImplementedError("No canonical form exists in the current framework")
 
     def random_instance(self, genome=None):
         """Return a random permutation corresponding to a given genome, or a random genome if none is given."""
         if genome:
             return choice(list(genome))[0]
         else:
             return self.genome_group().random_element()
+        
+    def identity_instance(self):
+        """Return the identity permutation."""
+        return self.genome_group().one()
 
     def random_genome(self, format=FORMAT.formal_sum):
         """Return a random genome"""
         return self.genome(self.random_instance(), format=format)
 
     def symmetry_group(self):
         """Return the symmetry group of the genomes."""
@@ -178,14 +185,44 @@
     def _genome_coset(self, instance):
         coset = set(instance*d for d in self.symmetry_group())
         return sorted([self.one_row(g) for g in coset], key=self._sort_key)
 
     def _double_coset(self, instance):
         coset = set(d2 * instance * d1 for d1 in self.symmetry_group() for d2 in self.symmetry_group())
         return sorted(coset, key=self._sort_key_cycles)
+    
+    def _double_coset_canonical(self, instance, D_n, D_n_dict, with_inverses=False):
+        coset = set()
+        for d2 in D_n:
+            gd2 = instance * d2
+            j = gd2.inverse()(1)
+            for d1 in D_n_dict[j]:
+                perm = d1 * gd2
+                coset.add(perm)
+        if with_inverses:
+            coset |= { elt.inverse() for elt in coset }
+        return coset
+
+    def canonical_double_cosets(self, join_inverse_classes=False):
+        D_n = {self.one_row(d) for d in self.symmetry_group()}
+        D_n_dict = { i : set() for i in range(-self.n, self.n + 1) }
+        for d in D_n:
+            D_n_dict[d(1)].add(d)
+        num_genomes = self.num_genomes()
+        found = set()
+        cosets = [ ]
+        for instance in self.fast_canonical_instance_generator(cycles = False):
+            if len(found) == num_genomes:
+                break
+            if instance in found:
+                continue
+            coset = self._double_coset_canonical(instance, D_n, D_n_dict, with_inverses=join_inverse_classes)
+            found |= coset
+            cosets.append(coset)
+        return cosets
 
     def _conjugacy_class(self, instance):
         conj_class = set(d.inverse() * instance * d for d in self.symmetry_group())
         return sorted([self.one_row(g) for g in conj_class], key=self._sort_key)
 
     def genome_equivalence_classes(self, combine_inverse_classes=False, sort_classes=True):
         """Return double cosets of instances---genomes in the same class will have the same likelihood functions"""
@@ -243,14 +280,26 @@
             Z = self.symmetry_group()
             A = self.group_algebra()
             genomes = { rep : sum(1/Z.order()*A(self.cycles(dx)) for dx in coset) for rep, coset in genomes.items() }
         if sort_genomes:
             genomes = dict(sorted(genomes.items(), key=lambda x: self._sort_key(x[0])))
         return genomes
 
+    def genome_canonical_instances(self):
+        """Return a set of all canonical genome instances"""
+        return {self.one_row(elt) for elt in self.genome_group() if elt(1) == 1}
+    
+    def genome_canonical_instances_generator(self):
+        m = self.n - 1
+        smaller_framework = PositionParadigmFramework(m, oriented=self.oriented, symmetry=self.symmetry)
+        for instance in smaller_framework.genome_group():
+            as_list = list(smaller_framework.one_row(instance))
+            new_list = [1] + [ x-1 if x < 0 else x+1 for x in as_list ]
+            yield self.one_row(new_list)
+
     def standard_reflection(self):
         """Return a permutation which reflects a genome instance about the center region (n odd), or the center two regions (n even)."""
         if self.oriented:
             string = f'({1},-{self.n})({self.n},-{1})'
             for i in range(1, int(self.n/2)):
                 string += f'({i+1}, -{self.n-(i-1)-1})({self.n-(i-1)-1}, -{i+1})'
             if self.n % 2 != 0:
@@ -301,33 +350,25 @@
     def _permutation_group_element_from_matrix(self, matrix):
         sigma = []
         for c, col in enumerate(matrix.T):
             image = np.nonzero(col)[0][0]
             sigma.append(matrix[image,c]*(image+1))
         return self.cycles(sigma)
 
-    def matrix(self, element):
-        """Return the defining representation matrix. Note that matrix(x)matrix(y) = matrix(yx)"""
-        with warnings.catch_warnings(): # Sage uses deprecated objects in to_matrix for coloured permutations. We would like to not be reminded of this.
-            warnings.simplefilter("ignore", category=PendingDeprecationWarning)
-            return np.array(self.one_row(self.cycles(element)).to_matrix())
-
     def reg_rep_of_zs(self, model, to_adjacency_matrix=False, sparse=True):
         # TODO: #14 re-write to directly use model element from the genome algebra
         if self is not model.framework:
             if self != model.framework:
                 raise ValueError(f"Current framework and model framework are not the same!")
             else:
                 warnings.warn("Current framework and model framework reference different objects! This might cause problems.")
         Z = self.symmetry_group()
         genomes = self.genomes()
         genome_list = list(genomes.values())
         reps = list(genomes.keys()) # Thousands of these
-        # Don't need the below line any more
-        #model_classes = list({frozenset({ d.inverse() * a * d for d in Z }) for a in model.generating_dictionary.keys()})
         model_generators_cycles = list(model.generating_dictionary.keys()) #[sorted(list(model_class))[0] for model_class in model_classes]
         model_generators = [
             self.one_row(elt) for elt in model_generators_cycles
         ]
         #model_classes = { rep : list(model_classes[r]) for r, rep in enumerate(model_generators) }
         genome_lookup = { rep : r for r, rep in enumerate(reps) }
         num_genomes = len(genomes.keys())
@@ -338,14 +379,93 @@
                 for rearrangement in model_generators:
                     coeff = 1
                     if not to_adjacency_matrix:
                         coeff = 1/Z.order() * model.generating_dictionary[model_generators_cycles[model_generators.index(rearrangement)]] # * len(model_classes[rearrangement])
                     matrix[g, genome_lookup[self.canonical_instance(permutation * rearrangement)]] += coeff
         print('...done!')
         return matrix if sparse else matrix.toarray()
+    
+    def fast_canonical_instance_generator(self, cycles=False):
+        signed_perms = SignedPermutations(self.n)
+
+        def one_row(elt):
+            elt_dict = elt.dict()
+            return signed_perms([elt_dict[i] for i in range(1, self.n + 1)])
+
+        f = one_row(self.standard_reflection())
+        r = one_row(self.standard_rotation())
+
+        def canonical_instance(instance):
+            if instance(1) < 0:
+                instance = instance*f
+            instance = instance*(r**((self.n-instance(1)+1)%self.n))
+            return instance
+
+        m = self.n
+        group = self.genome_group()
+        spm = tuple(range(2, m + 1)) + tuple(range(-m, -1))
+        s_pmn = SymmetricGroup(spm)
+        h_gens = [
+            s_pmn([(2, 3), (-2, -3)]),
+            s_pmn(tuple(range(2, m + 1)) + tuple(range(-2, -(m + 1), -1))),
+        ]
+        subgroup = group.subgroup(h_gens)
+        for elt in subgroup:
+            yield one_row(elt) if not cycles else self.cycles(one_row(elt))
+
+    def fast_reg_rep_of_zs(self, model):
+        """
+        
+        """
+        if DATA.reg_rep_of_zs in model.data_bundle:
+            return model.data_bundle[DATA.reg_rep_of_zs]
+        
+        signed_perms = SignedPermutations(self.n)
+
+        def one_row(elt):
+            elt_dict = elt.dict()
+            return signed_perms([elt_dict[i] for i in range(1, self.n + 1)])
+
+        f = one_row(self.standard_reflection())
+        r = one_row(self.standard_rotation())
+
+        def canonical_instance(instance):
+            if instance(1) < 0:
+                instance = instance*f
+            instance = instance*(r**((self.n-instance(1)+1)%self.n))
+            return instance
+
+        m = self.n
+        group = self.genome_group()
+        spm = tuple(range(2, m + 1)) + tuple(range(-m, -1))
+        s_pmn = SymmetricGroup(spm)
+        h_gens = [
+            s_pmn([(2, 3), (-2, -3)]),
+            s_pmn(tuple(range(2, m + 1)) + tuple(range(-2, -(m + 1), -1))),
+        ]
+        subgroup = group.subgroup(h_gens)
+        instance_lookup_or = { one_row(elt) : index for index, elt in enumerate(subgroup)}
+        num_genomes = len(instance_lookup_or.keys())
+        matrix = dok((num_genomes, num_genomes), dtype=np.float32)
+        elements_dalpha = { one_row(d) * one_row(alpha) : prob for d in self.symmetry_group() for alpha, prob in model.generating_dictionary.items() }
+        tasks = len(instance_lookup_or) * len(elements_dalpha)
+        done = 0
+        increment = len(elements_dalpha)
+        for instance, index in instance_lookup_or.items():
+            print(f"{round(100 * done / tasks, 1)}% Complete", end="\r")
+            for da, prob in elements_dalpha.items():
+                matrix[index, instance_lookup_or[canonical_instance(instance * da)]] += prob
+            done += increment
+        print("100.0% Complete!")
+
+        reg_rep_of_zs = 1/(2*self.n) * matrix, instance_lookup_or
+        model.data_bundle[DATA.reg_rep_of_zs] = reg_rep_of_zs
+
+        return reg_rep_of_zs
+
 
     def irreps(self, element=None):
         """
         Return a complete list of pairwise irreducible representations of the genome group.
 
         Args:
             element: return the image of element for each irreducible representation.
@@ -371,15 +491,15 @@
                     if sigma in self.group_algebra(): # sigma is an algebra element
                         for term in sigma:
                             perm, coeff = term
                             result += coeff * _irrep(perm)
                     else: # sigma is a group element
                         result = _irrep(sigma)
                     mat = result
-                    return mat.transpose() if _signed else matrix(mat)
+                    return mat if _signed else matrix(mat)
             return representation
         if not self.oriented:
             irreps = SymmetricGroupRepresentations(self.n)
         else:
             irreps = list(HyperoctahedralGroupRepresentations(self.n).values()) #(gap.IrreducibleAffordingRepresentation(character) for character in gap.Irr(self.genome_group()))
         for irrep in irreps:
             representations.append(irrep_function_factory(irrep, self.oriented))
@@ -424,7 +544,11 @@
                 genome_string = str(canonical_instance).replace(' ', '') + 'z'
             elif display is DISPLAY.cycles:
                 genome_string = str(self.cycles(canonical_instance)) + 'z'
             elif display is DISPLAY.arrows:
                 genome_string = '(' + self.draw_instance(self.cycles(canonical_instance), shortened=True) + ')'
             new_sum.append((coeff, genome_string))
         return FormalSum(new_sum, parent=QQ)
+
+# Convenient names
+GenomeFramework = PositionParadigmFramework
+Framework = PositionParadigmFramework
```

### Comparing `cgt-0.3.1/cgt/rearrangements.py` & `cgt-0.4.0/cgt/models.py`

 * *Files 24% similar despite different names*

```diff
@@ -1,153 +1,129 @@
 """
 """
 
-from copy import deepcopy
-from sage.all_cmdline import SymmetricGroup, floor
-import warnings
-from . import structures
+from sage.all_cmdline import QQ
 from .enums import *
-
-def css(cuts_set):
-    string = ''.join(sorted([str(cut[0]) for cut in cuts_set]))
-    if len(string) != len(cuts_set): print("something went very wrong here...")
-    return string
-
-
-def c_perm(n):
-    pmN = structures.set_plus_minus(n)
-    G = SymmetricGroup(pmN)
-    c_string = f'({",".join(str(i) for i in list(range(1, n+1)))})({",".join(str(i) for i in list(range(-n, 0)))})'
-    c = G(c_string)
-    return c
-
-def cuts(framework, sigma):
-    sigma = deepcopy(framework.one_row(sigma))
-    n = framework.n
-    c = c_perm(n)
-    sigma = list(sigma)
-    return set([ 
-        tuple(([i+1,c(i+1)])) for i in range(len(sigma)) 
-        if (sigma[c(i + 1)-1] != c(sigma[i]))
-    ])
-
-def __all_canonical_inversions(framework, num_regions=None):
-    if not framework.oriented:
-        raise NotImplementedError(f"not yet implemented for {str(framework)}")
-    if framework.symmetry not in {SYMMETRY.circular, SYMMETRY.linear}:
-        raise NotImplementedError(f"not implemented for framework with {str(framework.symmetry)} symmetry")
-    n = framework.n
-    G = framework.genome_group()
-    if num_regions == 1:
-        return {G(f'({i},-{i})') for i in range(1, n+1)} if framework.oriented else {}
-    elif num_regions == 2:
-        if framework.oriented:
-            perms = {G(f'({i},{-1*(i+1)})({-1*i},{i+1})') for i in range(1,n)}
-            if framework.symmetry is not SYMMETRY.linear:
-                perms.union({G(f'({n},-1)(-{n},1)')})
-        else:
-            perms = {G(f'({i},{i+1})') for i in range(1,n)} 
-            if framework.symmetry is not SYMMETRY.linear:
-                perms.union({G(f'(1,{n})')})
-        return perms
-    elif num_regions == None: # Return all inversions up to length floor(n/2)
-        up_to_length = floor(framework.n/2)
-        if framework.oriented: 
-            perms = set()
-            for permutation in G:
-                cycle_type = list(permutation.cycle_type())
-                if set(cycle_type)=={1,2} and list(cycle_type).count(2)<=up_to_length and len(cuts(framework, permutation))==2:
-                    perms.add(permutation)
-            if framework.symmetry is SYMMETRY.linear:
-                perms = {perm for perm in perms if not ('1' in str(perm) and str(n) in str(perm))}
-            return perms
-        else:
-            raise NotImplementedError(f"not yet implemented for {framework}")
-    else:
-        raise NotImplementedError(f"inversions of length {num_regions} not yet implemented")
-    
-def __two_region_adjacent_transposition_reps(framework):
-    if not framework.oriented or framework.symmetry != SYMMETRY.circular:
-        raise NotImplementedError(f"not yet implemented for {str(framework)}")
-    G = framework.genome_group()
-    return { G('(-2,-1)(1,2)'), G('(-2,1,2,-1)'), G('(-2,-1,2,1)'), G('(-2,2)(-1,1)') }
-
-def double_coset(framework, perm):
-    Z = framework.symmetry_group()
-    return { d1 * perm * d2 for d1 in Z for d2 in Z }
-
-def conjugacy_class(framework, perm):
-    Z = framework.symmetry_group()
-    return { d.inverse() * perm * d for d in Z }
-
-def single_coset(framework, perm):
-    Z = framework.symmetry_group()
-    return { perm * d for d in Z }
-
-def __representatives(framework, set_of_permutations, classes=CLASSES.double_cosets):
-    if not framework.oriented:
-        raise NotImplementedError(f"not yet implemented for {str(framework)}")
-    Z = framework.symmetry_group()
-    perms = {x for x in set_of_permutations}
-    cosets = []
-    while len(perms):
-        perm = perms.pop()
-        if classes is CLASSES.double_cosets:
-            coset = double_coset(framework, perm)
-        elif classes is CLASSES.conjugacy_classes:
-            coset = conjugacy_class(framework, perm)
-        elif classes is CLASSES.cosets:
-            coset = single_coset(framework, perm)
-        for element in coset:
-            perms.discard(element)
-        cosets.append(coset)
-    reps = set()
-    for coset in cosets:
-        reps.add(sorted(list(coset), key=lambda x: (sum(set(x.cycle_type())), list(x.cycle_type()).count(2), str(x)) )[0])
-    return reps
-
-def all_inversions_representatives(framework, num_regions=None):
-    return __representatives(framework, __all_canonical_inversions(framework, num_regions=num_regions), classes=CLASSES.double_cosets)
-
-def all_adjacent_transpositions_representatives(framework, num_regions=None):
-    if num_regions == 2:
-        return __two_region_adjacent_transposition_reps(framework)
-    else:
-        raise NotImplementedError(f"model not yet implemented")
-
-def permutation_with_cuts(framework, cuts, perm=None, start=None):
-    n = framework.n
-    c = c_perm(n)
-    if perm is None:
-        if not (framework.oriented and framework.symmetry == SYMMETRY.circular):
+from . import rearrangements
+from scipy.sparse import dok_matrix as dok
+import numpy as np
+
+
+class Model:
+    """Defines a model. A model consists of some collection of permutations and a map from these permutations to probabilities [0,1]"""
+    def __init__(self, framework, generating_dictionary):
+        """Define a model from a dictionary of single permutations, with their probabilities as the values."""
+        self.framework = framework
+        self.generating_dictionary = generating_dictionary
+        self.names = []
+        self._reg_rep_of_zs = None # For caching the regular representation of zs
+        self.data_bundle = {} # Used to cache data for several functions
+        # Check for time-reversibility
+        #rearrangements = set(self.generating_dictionary.keys())
+        #for rearrangement in rearrangements:
+        #    if rearrangement.inverse() not in self.generating_dictionary:
+        #        print(f"Model does not contain the inverse of {rearrangement}. Adding it #with equal probability so that the model is time-reversible. This means #that the generating dictionary is no longer the same as the one provided to #the constructor.")
+        #        prob = self.generating_dictionary[rearrangement] / 2
+        #        self.generating_dictionary[rearrangement.inverse()] = prob
+        #        self.generating_dictionary[rearrangement] = prob
+
+        # TODO: Implement checks for certain model properties, for example symmetry and missing rearrangements
+
+    def __repr__(self):
+        return f"Model({str(self.framework)}, {str(self.generating_dictionary)})"
+
+    def __str__(self):
+        """Return a descriptive string for the model"""
+        # TODO: #21 Make the model able to describe which permutations it allows after it is created
+        string = f"Model under the {str(self.framework).lower()}"
+        string += f" containing {' and '.join(str(name.value) for name in self.names) if self.names else 'generating perms: ' + str(self.generating_dictionary)}."
+        return string
+
+    @classmethod
+    def named_model_with_relative_probs(cls, framework, named_model_dictionary):
+        """
+        Create a model from a dictionary of named classes of rearrangements and their relative probabilities. 
+
+        Args:
+            framework (PositionParadigmFramework): The framework to create the model in
+            named_model_dictionary (dict): A dictionary of named classes of rearrangements and their relative probabilities.
+
+        Returns:
+            Model: A model with the specified named classes of rearrangements and their relative probabilities.
+        """
+        if not framework.oriented:
             raise NotImplementedError(f"not yet implemented for {str(framework)}")
-        perm = {}
-        perm[1] = 1 # making the canonical instance
-        results = permutation_with_cuts(cuts, perm, 2)
-        for result in results:
-            if result:
-                yield list(result.values())
-    else: # recurse
-        possibilities = set(range(1, n+1)) | set(range(-n, 0))
-        for val in perm.values():
-            possibilities.remove(val)
-            possibilities.remove(-val)
-        if start-1 in cuts:
-            if c(perm[start-1]) in possibilities: possibilities.remove(c(perm[start-1]))
-        else:
-            possibilities = possibilities & {c(perm[start-1])}
-        if start == n: # also check if *start* is a cut
-            if start in cuts:
-                # add exclusions
-                if start in possibilities: possibilities.remove(start) # p[1]=1 so we can't have p[n]=n
-            else:
-                possibilities = possibilities & {n} # we must choose n
-            for possibility in possibilities:
-                bperm = perm.copy()
-                bperm[start] = possibility
-                yield bperm
-        else:
-            for possibility in possibilities:
-                bperm = perm.copy()
-                bperm[start] = possibility
-                for result in permutation_with_cuts(cuts, bperm, start+1):
-                    yield result
+        # look through all specified model names and handle them appropriately
+        model = {}
+        if abs(sum(named_model_dictionary.values()) - 1) > 0.00001: 
+            raise ValueError("supplied probabilities do not sum to 1")
+        
+        special_model = False
+        # Check for special named models
+        if MODEL.all_inversions_larger_less_likely in named_model_dictionary:
+            special_model = True
+            if len(named_model_dictionary) > 1:
+                raise ValueError(f"Cannot have {MODEL.all_inversions_larger_less_likely} with other models")
+            elements = rearrangements.fast_all_inversion_reps(framework)
+            elements = sorted(list(elements), key = lambda x: len(x.cycles()))
+            denom = 2**len(elements) - 1
+            for e, element in enumerate(elements):
+                model[element] = (2**(len(elements) - e - 1))/denom
+
+        if not special_model:
+            for model_name, relative_prob in named_model_dictionary.items():
+                match model_name:
+                    # Inversions
+                    case MODEL.all_inversions:
+                        gens = rearrangements.all_inversions_representatives(framework)
+                    case MODEL.one_region_inversions:
+                        gens = rearrangements.all_inversions_representatives(framework, num_regions=1)
+                    case MODEL.two_region_inversions:
+                        gens = rearrangements.all_inversions_representatives(framework, num_regions=2)
+                    # Transpositions
+                    case MODEL.all_transpositions:
+                        gens = rearrangements.all_transposition_instances(framework, canonical_reps_only = True)
+                    case MODEL.two_region_transpositions:
+                        gens = rearrangements.all_transposition_instances(framework, scope_limit = 2, canonical_reps_only = True)
+                    case MODEL.two_region_transpositions_without_inversions:
+                        gens = rearrangements.all_transposition_instances(framework, scope_limit = 2, with_inversion = False, canonical_reps_only = True)
+                    case MODEL.two_region_revrevs:
+                        gens = rearrangements.all_transposition_instances(framework, scope_limit = 2, only_revrevs = True, canonical_reps_only = True)
+                    case MODEL.one_region_moves:
+                        gens = rearrangements.all_transposition_instances(framework, single_segment_limit = 1, canonical_reps_only = True)
+                    case MODEL.one_region_moves_without_inversions:
+                        gens = rearrangements.all_transposition_instances(framework, single_segment_limit = 1, with_inversion = False, canonical_reps_only = True)
+                    case MODEL.three_region_transpositions:
+                        gens = rearrangements.all_transposition_instances(framework, scope_limit = 3, canonical_reps_only = True)
+                    case MODEL.two_region_adjacent_transpositions:
+                        gens = rearrangements.all_adjacent_transpositions_representatives(framework, num_regions=2)
+                for generator in gens: 
+                    model[generator] = relative_prob/len(gens)
+
+        model = cls(framework, model)
+        model.names += list(named_model_dictionary.keys())
+        return model
+
+    def reg_rep_of_zs(self):
+        """Return the regular representation of zs as comptued by PositionParadigmFramework.reg_rep_zs, but store the sparse result"""
+        if self._reg_rep_of_zs is None:
+            self._reg_rep_of_zs = self.framework.reg_rep_of_zs(self, sparse=True)
+        return self._reg_rep_of_zs
+    
+    def s_element(self, in_algebra=ALGEBRA.genome):
+        if in_algebra not in {ALGEBRA.group, ALGEBRA.genome}:
+            raise NotImplementedError(f"Model element for {str(in_algebra)} algebra not yet implemented")
+        A = self.framework.group_algebra()
+        s = A(0) # Zero element in algebra
+        gens_dict = self.generating_dictionary
+        gens = {x for x in self.generating_dictionary.keys()}
+        while len(gens) > 0:
+            gen = gens.pop()
+            prob = gens_dict[gen]
+            if in_algebra is ALGEBRA.group:
+                conj_class = rearrangements.conjugacy_class(self.framework, gen)
+            elif in_algebra is ALGEBRA.genome:
+                conj_class = {gen}
+            for perm in conj_class:
+                s += QQ(prob/len(conj_class)) * A(perm)
+            gens -= conj_class
+        return s
```

### Comparing `cgt-0.3.1/cgt/simulations.py` & `cgt-0.4.0/cgt/simulations.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,123 +1,148 @@
-#%%
+"""
+This module contains functions for simulating the evolution of genomes on a tree.
+"""
+
 import matplotlib.pyplot as plt
-import matplotlib.image as mpimg
 import numpy as np
 import cgt
 from cgt import *
 from networkx.drawing.nx_agraph import graphviz_layout
 from networkx import json_graph
 import networkx as nx
 
+
 def newick_to_tree(newick_string):
     json_tree = cgt.parsers.newick_to_json(
-        newick_string, 
-        generate_names = True, 
-        lengthstring = "weight"
+        newick_string, generate_names=True, lengthstring="weight"
     )
     tree = json_graph.tree_graph(json_tree)
     return tree
 
-def evolve_on_tree(tree, framework, model, root="random"):
-    model_element = model.s_element()
+
+def evolve_on_tree(tree, framework, model, root="random", at_least_one_change=False, exactly_n_changes=None):
     # The tree should be a networkx DiGraph
     # Choose a genome at the root of the tree
-    if root == "random": 
+    if root == "random":
         root = framework.random_genome()
-    else: 
+    else:
         root = framework.identity_genome()
-    
+
     # Get the root and set the genome at the root
-    root_id = [n for n, d in tree.in_degree() if d==0][0]
+    root_id = [n for n, d in tree.in_degree() if d == 0][0]
     tree.nodes[root_id]["genome"] = root
 
     # Traverse the tree
-    root = [n for n,d in tree.in_degree() if d==0][0]
+    root = [n for n, d in tree.in_degree() if d == 0][0]
     for successor, node in dict(nx.bfs_predecessors(tree, root)).items():
         # Get the genome at the parent node
         parent = tree.nodes[node]["genome"]
         # Get the branch length of the in-edge
         branch_length = tree.nodes[successor]["weight"]
-        tree[node][successor]['weight'] = branch_length
-        tree[node][successor]['len'] = branch_length
+        tree[node][successor]["weight"] = branch_length
+        tree[node][successor]["len"] = branch_length
         # Decide how many rearrangements to apply
-        num_rearrangements = np.random.poisson(branch_length)
+        if exactly_n_changes is not None:
+            num_rearrangements = exactly_n_changes
+        else:
+            num_rearrangements = np.random.poisson(branch_length)
+        if at_least_one_change:
+            num_rearrangements = max(num_rearrangements, 1)
         # Apply them
         tree.nodes[successor]["genome"] = parent
-        if num_rearrangements == 0: 
-            tree.nodes[successor]["label"] = str(framework.collect_genome_terms(parent)).replace(" ", "")
+        if num_rearrangements == 0:
+            tree.nodes[successor]["label"] = str(
+                framework.collect_genome_terms(parent)
+            ).replace(" ", "")
             tree.nodes[successor]["genome"] = parent
         for r in range(num_rearrangements):
             # Draw a rearrangement
             rearrangement = draw_rearrangement(model)
             # Apply the rearrangement
             formal_sum = tree.nodes[successor]["genome"] * rearrangement
             selected_genome_instance = cgt.simulations.draw_genome(formal_sum)
             canonical_instance = framework.canonical_instance(selected_genome_instance)
-            genome = framework.genome(framework.cycles(framework.canonical_instance(selected_genome_instance)), format=cgt.FORMAT.formal_sum)
+            genome = framework.genome(
+                framework.cycles(
+                    framework.canonical_instance(selected_genome_instance)
+                ),
+                format=cgt.FORMAT.formal_sum,
+            )
             # Update the genome at the successor node
             tree.nodes[successor]["genome"] = genome
             tree.nodes[successor]["label"] = str(framework.collect_genome_terms(genome))
-    
+
     return tree
 
+
 def grow_tree(framework, model, num_taxa):
     model_element = model.s_element()
     # Start with the identity genome
     genome = framework.genome_group().identity()
     print(framework.draw_instance(genome, shortened=True))
     # Instantiate the tree
     G = nx.DiGraph()
-    G.add_node(0, label=str(genome), genome=genome) # initialize root
-    for t in range(0, num_taxa+1, 2):
+    G.add_node(0, label=str(genome), genome=genome)  # initialize root
+    for t in range(0, num_taxa + 1, 2):
         # Select a genome from the tree
-        node = np.random.choice([node for node in G.nodes() if G.out_degree(node)==0])
-        parent = G.nodes[node]['genome']
+        node = np.random.choice([node for node in G.nodes() if G.out_degree(node) == 0])
+        parent = G.nodes[node]["genome"]
 
         # Draw a branch length From a multinomial distribution
         # Draw the number of events from a poisson distribution
         # Choose the rearangements from the model and apply them
-        
-    # Grow two new leaves
+
+        # Grow two new leaves
         for t_1 in range(2):
             # Draw a rearrangement
             rearrangement = draw_rearrangement(model)
             # Apply the rearrangement
             genome = parent * rearrangement
             # Draw a branch length
             branch_length = draw_branch_length()
             # Add the new genome to the tree
-            G.add_node(t+t_1+1, label=str(genome), genome=genome)
-            G.add_edge(node, t+t_1+1, weight=round(branch_length,1))
+            G.add_node(t + t_1 + 1, label=str(genome), genome=genome)
+            G.add_edge(node, t + t_1 + 1, weight=round(branch_length, 1))
 
     # Return the tree
     return G
 
+
 def draw_tree(tree):
     # Draw the tree
-    plt.figure(figsize=(9,5))
+    plt.figure(figsize=(9, 5))
     G = tree
-    pos = graphviz_layout(G, prog='dot')#, args='-Granksep=0.1 -Gnodesep=0.1')
-    labels = nx.get_node_attributes(G, 'label')
-    edge_labels = nx.get_edge_attributes(G, 'weight')
+    pos = graphviz_layout(G, prog="dot")  # , args='-Granksep=0.1 -Gnodesep=0.1')
+    labels = nx.get_node_attributes(G, "label")
+    edge_labels = nx.get_edge_attributes(G, "weight")
     nx.draw(G, pos=pos, node_size=0)
-    nx.draw_networkx_labels(G, pos, labels=labels, bbox={"facecolor":"white", "edgecolor":"white"}, font_size=10)
-    nx.draw_networkx_edge_labels(G, pos=pos, rotate=False, edge_labels=edge_labels, font_size=10)
+    nx.draw_networkx_labels(
+        G,
+        pos,
+        labels=labels,
+        bbox={"facecolor": "white", "edgecolor": "white"},
+        font_size=10,
+    )
+    nx.draw_networkx_edge_labels(
+        G, pos=pos, rotate=False, edge_labels=edge_labels, font_size=10
+    )
     plt.show()
 
 
 def draw_branch_length():
     return np.random.exponential(1)
 
 
 def draw_rearrangement(model):
     model_element = model.s_element()
     rearrangements, probs = tuple(zip(*[list(x)[0] for x in (model_element).terms()]))
     return np.random.choice(rearrangements, p=probs)
 
+
 def draw_genome(formal_sum):
     genomes, probs = tuple(zip(*list(formal_sum)))
     return np.random.choice(genomes, p=probs)
 
+
 def set_node(node, framework, genome):
     node["genome"] = genome
     node["label"] = str(framework.canonical_instance(genome))
```

### Comparing `cgt-0.3.1/cgt/structures.py` & `cgt-0.4.0/cgt/structures.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,18 +1,21 @@
 """
 A place for functions which return important but general algebraic structures requiring only a few parameters
 """
 
 from sage.all_cmdline import SymmetricGroup
 
+
 def set_plus_minus(n):
-    return tuple(range(1,n+1)) + tuple(range(-n, 0))
+    return tuple(range(1, n + 1)) + tuple(range(-n, 0))
+
 
 def HyperoctahedralGroup(n):
     """Return the hyperoctahedral group of order (2^n)n! as a subgroup of SymmetricGroup(2n) with two generators."""
     s_pmn = SymmetricGroup(set_plus_minus(n))
-    if n==1: return s_pmn
+    if n == 1:
+        return s_pmn
     h_gens = [
-        s_pmn([(1,2),(-1,-2)]),
-        s_pmn(tuple(range(1,n+1)) + tuple(range(-1, -(n+1), -1)))
+        s_pmn([(1, 2), (-1, -2)]),
+        s_pmn(tuple(range(1, n + 1)) + tuple(range(-1, -(n + 1), -1))),
     ]
-    return s_pmn.subgroup(h_gens)
+    return s_pmn.subgroup(h_gens)
```

### Comparing `cgt-0.3.1/cgt/visualisation.py` & `cgt-0.4.0/cgt/visualisation.py`

 * *Files 20% similar despite different names*

```diff
@@ -4,68 +4,96 @@
 import os
 import matplotlib
 import matplotlib.pyplot as plt
 import numpy as np
 from .position_paradigm import *
 from .enums import *
 
+
 def draw_genome_instance(framework, instance, show=False):
     """Produce a drawing of a circular genome with n regions"""
     if not framework.oriented:
         raise NotImplementedError("not implemented for linear genomes.")
     try:
         instance = framework.cycles(instance)
     except:
         TypeError(f"{instance} does not belong in {str(framework)}")
 
-    matplotlib.rcParams.update({
-        "text.usetex": True,
-        "font.family": "serif",
-        "pgf.texsystem": "pdflatex",
-        'pgf.rcfonts': False,
-        "font.size": 18,
-    })
-    plt.style.use('default')
+    matplotlib.rcParams.update(
+        {
+            "text.usetex": True,
+            "font.family": "serif",
+            "pgf.texsystem": "pdflatex",
+            "pgf.rcfonts": False,
+            "font.size": 18,
+        }
+    )
+    plt.style.use("default")
 
     n = framework.n
-    region_labels     = [None for _ in range(1, n+1)]
-    orientation_list  = [False for _ in range(1,n+1)]
+    region_labels = [None for _ in range(1, n + 1)]
+    orientation_list = [False for _ in range(1, n + 1)]
 
     for r, p in list(enumerate(framework.one_row(instance, as_list=True))):
-        region_labels[abs(p)-1] = r+1
-        orientation_list[abs(p)-1] = p<0
-    
+        region_labels[abs(p) - 1] = r + 1
+        orientation_list[abs(p) - 1] = p < 0
+
     region_labels = list(reversed(region_labels))
     orientation_list = list(reversed(orientation_list))
 
-    segment_sizes = [100/n for _ in range(n)]
-    segment_colors = ['white' for _ in range(n)]
-    
-    fig1, ax1 = plt.subplots(figsize=(2,2))
-    wedges, texts = ax1.pie(segment_sizes, labeldistance=1.2, colors=segment_colors, 
-                            labels=region_labels, radius=1, startangle=90, 
-                            wedgeprops={"edgecolor":"0", 'linewidth': 1, 'linestyle': 'solid', 'antialiased': True})
-                
+    segment_sizes = [100 / n for _ in range(n)]
+    segment_colors = ["white" for _ in range(n)]
+
+    fig1, ax1 = plt.subplots(figsize=(2, 2))
+    wedges, texts = ax1.pie(
+        segment_sizes,
+        labeldistance=1.2,
+        colors=segment_colors,
+        labels=region_labels,
+        radius=1,
+        startangle=90,
+        wedgeprops={
+            "edgecolor": "0",
+            "linewidth": 1,
+            "linestyle": "solid",
+            "antialiased": True,
+        },
+    )
+
     if framework.oriented and orientation_list:
         for i, p in enumerate(wedges):
-            ang = (p.theta2 - p.theta1)/2. + p.theta1
+            ang = (p.theta2 - p.theta1) / 2.0 + p.theta1
             y = np.sin(np.deg2rad(ang))
             x = np.cos(np.deg2rad(ang))
-            arrow_length = 0.00001 # We only want the arrow head
-            angle = np.deg2rad(ang) + (np.pi/2 if orientation_list[i] else 3*np.pi/2)
+            arrow_length = 0.00001  # We only want the arrow head
+            angle = np.deg2rad(ang) + (
+                np.pi / 2 if orientation_list[i] else 3 * np.pi / 2
+            )
             if orientation_list:
-                ax1.arrow(x, y, arrow_length*np.cos(angle), arrow_length*np.sin(angle), 
-                            overhang = 0.3, head_width=0.12, head_length=0.12, head_starts_at_zero=True, 
-                            length_includes_head=True, linewidth=1, facecolor='black', fill=True)
+                ax1.arrow(
+                    x,
+                    y,
+                    arrow_length * np.cos(angle),
+                    arrow_length * np.sin(angle),
+                    overhang=0.3,
+                    head_width=0.12,
+                    head_length=0.12,
+                    head_starts_at_zero=True,
+                    length_includes_head=True,
+                    linewidth=1,
+                    facecolor="black",
+                    fill=True,
+                )
 
     # Draw inner circle to hide most of the segment edges
-    centre_circle = plt.Circle((0,0),0.85,fc='white')
+    centre_circle = plt.Circle((0, 0), 0.85, fc="white")
     fig = plt.gcf()
     fig.gca().add_artist(centre_circle)
-    ax1.axis('equal') # makes sure it's a circle
+    ax1.axis("equal")  # makes sure it's a circle
     plt.tight_layout()
 
-    if not os.path.exists('_output'):
-        os.makedirs('_output')
-    plt.savefig(f'_output/{str(instance)}.png', transparent=True)
-    plt.savefig(f'_output/{str(instance)}.pdf', transparent=True)
-    if show: plt.show()
+    if not os.path.exists("_output"):
+        os.makedirs("_output")
+    plt.savefig(f"_output/{str(instance)}.png", transparent=True)
+    plt.savefig(f"_output/{str(instance)}.pdf", transparent=True)
+    if show:
+        plt.show()
```

### Comparing `cgt-0.3.1/cgt.egg-info/PKG-INFO` & `cgt-0.4.0/cgt.egg-info/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: cgt
-Version: 0.3.1
+Version: 0.4.0
 Summary: Tools for representing genomes in sage
 Home-page: https://github.com/js51/Circular-genome-tools
 Author: Joshua Stevenson
 Author-email: joshua.stevenson@utas.edu.au
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

### Comparing `cgt-0.3.1/setup.py` & `cgt-0.4.0/setup.py`

 * *Files 18% similar despite different names*

```diff
@@ -19,8 +19,10 @@
     packages=setuptools.find_packages(),
     classifiers=[
         "Programming Language :: Python :: 3",
         "License :: OSI Approved :: MIT License",
         "Operating System :: OS Independent",
     ],
     python_requires='>=3',
+    package_data={'cgt': ['*.pickle']},
+    include_package_data=True,
 )
```

