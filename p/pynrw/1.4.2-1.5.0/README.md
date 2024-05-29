# Comparing `tmp/pynrw-1.4.2.tar.gz` & `tmp/pynrw-1.5.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pynrw-1.4.2.tar", last modified: Tue May 21 00:25:30 2024, max compression
+gzip compressed data, was "pynrw-1.5.0.tar", last modified: Wed May 29 11:23:32 2024, max compression
```

## Comparing `pynrw-1.4.2.tar` & `pynrw-1.5.0.tar`

### file list

```diff
@@ -1,52 +1,52 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-21 00:25:30.750676 pynrw-1.4.2/
--rw-r--r--   0 runner    (1001) docker     (127)     1075 2024-05-21 00:25:15.000000 pynrw-1.4.2/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)    10151 2024-05-21 00:25:30.750676 pynrw-1.4.2/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     8932 2024-05-21 00:25:15.000000 pynrw-1.4.2/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-21 00:25:30.746676 pynrw-1.4.2/nrw/
--rw-r--r--   0 runner    (1001) docker     (127)      206 2024-05-21 00:25:15.000000 pynrw-1.4.2/nrw/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)       70 2024-05-21 00:25:15.000000 pynrw-1.4.2/nrw/__init__.pyi
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-21 00:25:30.746676 pynrw-1.4.2/nrw/algorithms/
--rw-r--r--   0 runner    (1001) docker     (127)      775 2024-05-21 00:25:15.000000 pynrw-1.4.2/nrw/algorithms/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2227 2024-05-21 00:25:15.000000 pynrw-1.4.2/nrw/algorithms/__init__.pyi
--rw-r--r--   0 runner    (1001) docker     (127)     2635 2024-05-21 00:25:15.000000 pynrw-1.4.2/nrw/algorithms/_searching.py
--rw-r--r--   0 runner    (1001) docker     (127)     4527 2024-05-21 00:25:15.000000 pynrw-1.4.2/nrw/algorithms/_sorting.py
--rw-r--r--   0 runner    (1001) docker     (127)     3703 2024-05-21 00:25:15.000000 pynrw-1.4.2/nrw/algorithms/_traversal.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-21 00:25:30.746676 pynrw-1.4.2/nrw/database/
--rw-r--r--   0 runner    (1001) docker     (127)       61 2024-05-21 00:25:15.000000 pynrw-1.4.2/nrw/database/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2217 2024-05-21 00:25:15.000000 pynrw-1.4.2/nrw/database/_query_result.py
--rw-r--r--   0 runner    (1001) docker     (127)      694 2024-05-21 00:25:15.000000 pynrw-1.4.2/nrw/database/_query_result.pyi
--rw-r--r--   0 runner    (1001) docker     (127)     4383 2024-05-21 00:25:15.000000 pynrw-1.4.2/nrw/database/msaccess.py
--rw-r--r--   0 runner    (1001) docker     (127)      699 2024-05-21 00:25:15.000000 pynrw-1.4.2/nrw/database/msaccess.pyi
--rw-r--r--   0 runner    (1001) docker     (127)     4661 2024-05-21 00:25:15.000000 pynrw-1.4.2/nrw/database/mysql.py
--rw-r--r--   0 runner    (1001) docker     (127)      696 2024-05-21 00:25:15.000000 pynrw-1.4.2/nrw/database/mysql.pyi
--rw-r--r--   0 runner    (1001) docker     (127)     4357 2024-05-21 00:25:15.000000 pynrw-1.4.2/nrw/database/sqlite.py
--rw-r--r--   0 runner    (1001) docker     (127)      699 2024-05-21 00:25:15.000000 pynrw-1.4.2/nrw/database/sqlite.pyi
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-21 00:25:30.750676 pynrw-1.4.2/nrw/datastructures/
--rw-r--r--   0 runner    (1001) docker     (127)      801 2024-05-21 00:25:15.000000 pynrw-1.4.2/nrw/datastructures/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     5471 2024-05-21 00:25:15.000000 pynrw-1.4.2/nrw/datastructures/__init__.pyi
--rw-r--r--   0 runner    (1001) docker     (127)     7823 2024-05-21 00:25:15.000000 pynrw-1.4.2/nrw/datastructures/_binary_search_tree.py
--rw-r--r--   0 runner    (1001) docker     (127)     5022 2024-05-21 00:25:15.000000 pynrw-1.4.2/nrw/datastructures/_binary_tree.py
--rw-r--r--   0 runner    (1001) docker     (127)      841 2024-05-21 00:25:15.000000 pynrw-1.4.2/nrw/datastructures/_comparable_content.py
--rw-r--r--   0 runner    (1001) docker     (127)     2563 2024-05-21 00:25:15.000000 pynrw-1.4.2/nrw/datastructures/_edge.py
--rw-r--r--   0 runner    (1001) docker     (127)     9511 2024-05-21 00:25:15.000000 pynrw-1.4.2/nrw/datastructures/_graph.py
--rw-r--r--   0 runner    (1001) docker     (127)     9323 2024-05-21 00:25:15.000000 pynrw-1.4.2/nrw/datastructures/_list.py
--rw-r--r--   0 runner    (1001) docker     (127)     3760 2024-05-21 00:25:15.000000 pynrw-1.4.2/nrw/datastructures/_queue.py
--rw-r--r--   0 runner    (1001) docker     (127)     3519 2024-05-21 00:25:15.000000 pynrw-1.4.2/nrw/datastructures/_stack.py
--rw-r--r--   0 runner    (1001) docker     (127)     3338 2024-05-21 00:25:15.000000 pynrw-1.4.2/nrw/datastructures/_utils.py
--rw-r--r--   0 runner    (1001) docker     (127)     1562 2024-05-21 00:25:15.000000 pynrw-1.4.2/nrw/datastructures/_vertex.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-21 00:25:30.750676 pynrw-1.4.2/nrw/network/
--rw-r--r--   0 runner    (1001) docker     (127)      308 2024-05-21 00:25:15.000000 pynrw-1.4.2/nrw/network/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1814 2024-05-21 00:25:15.000000 pynrw-1.4.2/nrw/network/__init__.pyi
--rw-r--r--   0 runner    (1001) docker     (127)     5227 2024-05-21 00:25:15.000000 pynrw-1.4.2/nrw/network/_client.py
--rw-r--r--   0 runner    (1001) docker     (127)     3637 2024-05-21 00:25:15.000000 pynrw-1.4.2/nrw/network/_connection.py
--rw-r--r--   0 runner    (1001) docker     (127)    15226 2024-05-21 00:25:15.000000 pynrw-1.4.2/nrw/network/_server.py
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-21 00:25:15.000000 pynrw-1.4.2/nrw/py.typed
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-21 00:25:30.750676 pynrw-1.4.2/pynrw.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)    10151 2024-05-21 00:25:30.000000 pynrw-1.4.2/pynrw.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     1114 2024-05-21 00:25:30.000000 pynrw-1.4.2/pynrw.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-21 00:25:30.000000 pynrw-1.4.2/pynrw.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)      185 2024-05-21 00:25:30.000000 pynrw-1.4.2/pynrw.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)        4 2024-05-21 00:25:30.000000 pynrw-1.4.2/pynrw.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)     3398 2024-05-21 00:25:15.000000 pynrw-1.4.2/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)      167 2024-05-21 00:25:15.000000 pynrw-1.4.2/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-21 00:25:30.750676 pynrw-1.4.2/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-29 11:23:32.932686 pynrw-1.5.0/
+-rw-r--r--   0 runner    (1001) docker     (127)     1075 2024-05-29 11:23:23.000000 pynrw-1.5.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)    10169 2024-05-29 11:23:32.932686 pynrw-1.5.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     8950 2024-05-29 11:23:23.000000 pynrw-1.5.0/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-29 11:23:32.924686 pynrw-1.5.0/nrw/
+-rw-r--r--   0 runner    (1001) docker     (127)      206 2024-05-29 11:23:23.000000 pynrw-1.5.0/nrw/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)       70 2024-05-29 11:23:23.000000 pynrw-1.5.0/nrw/__init__.pyi
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-29 11:23:32.924686 pynrw-1.5.0/nrw/algorithms/
+-rw-r--r--   0 runner    (1001) docker     (127)      710 2024-05-29 11:23:23.000000 pynrw-1.5.0/nrw/algorithms/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2021 2024-05-29 11:23:23.000000 pynrw-1.5.0/nrw/algorithms/__init__.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)     2635 2024-05-29 11:23:23.000000 pynrw-1.5.0/nrw/algorithms/_searching.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4527 2024-05-29 11:23:23.000000 pynrw-1.5.0/nrw/algorithms/_sorting.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3392 2024-05-29 11:23:23.000000 pynrw-1.5.0/nrw/algorithms/_traversal.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-29 11:23:32.928686 pynrw-1.5.0/nrw/database/
+-rw-r--r--   0 runner    (1001) docker     (127)       61 2024-05-29 11:23:23.000000 pynrw-1.5.0/nrw/database/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2217 2024-05-29 11:23:23.000000 pynrw-1.5.0/nrw/database/_query_result.py
+-rw-r--r--   0 runner    (1001) docker     (127)      694 2024-05-29 11:23:23.000000 pynrw-1.5.0/nrw/database/_query_result.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)     4409 2024-05-29 11:23:23.000000 pynrw-1.5.0/nrw/database/msaccess.py
+-rw-r--r--   0 runner    (1001) docker     (127)      699 2024-05-29 11:23:23.000000 pynrw-1.5.0/nrw/database/msaccess.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)     4661 2024-05-29 11:23:23.000000 pynrw-1.5.0/nrw/database/mysql.py
+-rw-r--r--   0 runner    (1001) docker     (127)      696 2024-05-29 11:23:23.000000 pynrw-1.5.0/nrw/database/mysql.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)     4357 2024-05-29 11:23:23.000000 pynrw-1.5.0/nrw/database/sqlite.py
+-rw-r--r--   0 runner    (1001) docker     (127)      699 2024-05-29 11:23:23.000000 pynrw-1.5.0/nrw/database/sqlite.pyi
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-29 11:23:32.928686 pynrw-1.5.0/nrw/datastructures/
+-rw-r--r--   0 runner    (1001) docker     (127)      801 2024-05-29 11:23:23.000000 pynrw-1.5.0/nrw/datastructures/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5471 2024-05-29 11:23:23.000000 pynrw-1.5.0/nrw/datastructures/__init__.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)     7823 2024-05-29 11:23:23.000000 pynrw-1.5.0/nrw/datastructures/_binary_search_tree.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5022 2024-05-29 11:23:23.000000 pynrw-1.5.0/nrw/datastructures/_binary_tree.py
+-rw-r--r--   0 runner    (1001) docker     (127)      841 2024-05-29 11:23:23.000000 pynrw-1.5.0/nrw/datastructures/_comparable_content.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2563 2024-05-29 11:23:23.000000 pynrw-1.5.0/nrw/datastructures/_edge.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9511 2024-05-29 11:23:23.000000 pynrw-1.5.0/nrw/datastructures/_graph.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9323 2024-05-29 11:23:23.000000 pynrw-1.5.0/nrw/datastructures/_list.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3760 2024-05-29 11:23:23.000000 pynrw-1.5.0/nrw/datastructures/_queue.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3519 2024-05-29 11:23:23.000000 pynrw-1.5.0/nrw/datastructures/_stack.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2445 2024-05-29 11:23:23.000000 pynrw-1.5.0/nrw/datastructures/_utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1562 2024-05-29 11:23:23.000000 pynrw-1.5.0/nrw/datastructures/_vertex.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-29 11:23:32.932686 pynrw-1.5.0/nrw/network/
+-rw-r--r--   0 runner    (1001) docker     (127)      308 2024-05-29 11:23:23.000000 pynrw-1.5.0/nrw/network/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1814 2024-05-29 11:23:23.000000 pynrw-1.5.0/nrw/network/__init__.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)     5227 2024-05-29 11:23:23.000000 pynrw-1.5.0/nrw/network/_client.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3637 2024-05-29 11:23:23.000000 pynrw-1.5.0/nrw/network/_connection.py
+-rw-r--r--   0 runner    (1001) docker     (127)    15226 2024-05-29 11:23:23.000000 pynrw-1.5.0/nrw/network/_server.py
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-29 11:23:23.000000 pynrw-1.5.0/nrw/py.typed
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-29 11:23:32.932686 pynrw-1.5.0/pynrw.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)    10169 2024-05-29 11:23:32.000000 pynrw-1.5.0/pynrw.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     1114 2024-05-29 11:23:32.000000 pynrw-1.5.0/pynrw.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-29 11:23:32.000000 pynrw-1.5.0/pynrw.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      185 2024-05-29 11:23:32.000000 pynrw-1.5.0/pynrw.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        4 2024-05-29 11:23:32.000000 pynrw-1.5.0/pynrw.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)     3398 2024-05-29 11:23:23.000000 pynrw-1.5.0/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)      167 2024-05-29 11:23:23.000000 pynrw-1.5.0/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-29 11:23:32.932686 pynrw-1.5.0/setup.cfg
```

### Comparing `pynrw-1.4.2/LICENSE` & `pynrw-1.5.0/LICENSE`

 * *Files identical despite different names*

### Comparing `pynrw-1.4.2/PKG-INFO` & `pynrw-1.5.0/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pynrw
-Version: 1.4.2
+Version: 1.5.0
 Summary: Materialien zu den zentralen NRW-Abiturprüfungen im Fach Informatik ab 2018 implementiert in Python.
 Author: realshouzy
 License: MIT
 Project-URL: Source, https://github.com/realshouzy/pynrw
 Keywords: nrw,datastructures,datenstrukturen,algorithms,algorithmen,education,bildung,abitur
 Platform: any
 Classifier: Programming Language :: Python :: 3 :: Only
@@ -106,21 +106,21 @@
 bst.insert(3)
 bst.insert(2)
 bst.insert(5)
 bst.insert(0)
 bst.insert(1)
 bst.insert(4)
 print(bst)
-#    _4_
-#   /   \
-#  _2   6
-# /  \ /
-# 0  3 5
+#       3__
+#      /   \
+#   __2     5
+#  /       /
+# 0       4
 #  \
-#  1
+#   1
 ```
 
 Des weiteren sind (triviale) Optimierungen vorgenommen worden:
 
 - Verwendung von [`__slots__`](https://docs.python.org/3/reference/datamodel.html#slots)
 - redundante Aufrufe werden weggelassen
 - interne Optimierungen bei Zuweisungen
```

### Comparing `pynrw-1.4.2/README.md` & `pynrw-1.5.0/README.md`

 * *Files 2% similar despite different names*

```diff
@@ -79,21 +79,21 @@
 bst.insert(3)
 bst.insert(2)
 bst.insert(5)
 bst.insert(0)
 bst.insert(1)
 bst.insert(4)
 print(bst)
-#    _4_
-#   /   \
-#  _2   6
-# /  \ /
-# 0  3 5
+#       3__
+#      /   \
+#   __2     5
+#  /       /
+# 0       4
 #  \
-#  1
+#   1
 ```
 
 Des weiteren sind (triviale) Optimierungen vorgenommen worden:
 
 - Verwendung von [`__slots__`](https://docs.python.org/3/reference/datamodel.html#slots)
 - redundante Aufrufe werden weggelassen
 - interne Optimierungen bei Zuweisungen
```

### Comparing `pynrw-1.4.2/nrw/algorithms/__init__.py` & `pynrw-1.5.0/nrw/algorithms/__init__.py`

 * *Files 12% similar despite different names*

```diff
@@ -11,15 +11,14 @@
     "insertion_sort",
     "merge_sort",
     "quick_sort",
     "preorder",
     "inorder",
     "postorder",
     "levelorder",
-    "reverse_inorder",
 ]
 
 from typing import Final
 
 from nrw.algorithms._searching import (
     breadth_first_search,
     depth_first_search,
@@ -28,14 +27,8 @@
 from nrw.algorithms._sorting import (
     bubble_sort,
     insertion_sort,
     merge_sort,
     quick_sort,
     selection_sort,
 )
-from nrw.algorithms._traversal import (
-    inorder,
-    levelorder,
-    postorder,
-    preorder,
-    reverse_inorder,
-)
+from nrw.algorithms._traversal import inorder, levelorder, postorder, preorder
```

### Comparing `pynrw-1.4.2/nrw/algorithms/__init__.pyi` & `pynrw-1.5.0/nrw/algorithms/__init__.pyi`

 * *Files 3% similar despite different names*

```diff
@@ -8,15 +8,14 @@
     "insertion_sort",
     "merge_sort",
     "quick_sort",
     "preorder",
     "inorder",
     "postorder",
     "levelorder",
-    "reverse_inorder",
 ]
 
 from typing import Final, TypeVar, overload
 
 from nrw.datastructures import (
     BinarySearchTree,
     BinaryTree,
@@ -49,20 +48,14 @@
 @overload
 def inorder(
     tree: BinarySearchTree[ComparableContentT],
     *,
     reverse: bool = False,
 ) -> List[ComparableContentT]: ...
 @overload
-def reverse_inorder(tree: BinaryTree[_T]) -> List[_T]: ...
-@overload
-def reverse_inorder(
-    tree: BinarySearchTree[ComparableContentT],
-) -> List[ComparableContentT]: ...
-@overload
 def postorder(tree: BinaryTree[_T], *, reverse: bool = False) -> List[_T]: ...
 @overload
 def postorder(
     tree: BinarySearchTree[ComparableContentT],
     *,
     reverse: bool = False,
 ) -> List[ComparableContentT]: ...
```

### Comparing `pynrw-1.4.2/nrw/algorithms/_searching.py` & `pynrw-1.5.0/nrw/algorithms/_searching.py`

 * *Files identical despite different names*

### Comparing `pynrw-1.4.2/nrw/algorithms/_sorting.py` & `pynrw-1.5.0/nrw/algorithms/_sorting.py`

 * *Files identical despite different names*

### Comparing `pynrw-1.4.2/nrw/algorithms/_traversal.py` & `pynrw-1.5.0/nrw/algorithms/_traversal.py`

 * *Files 14% similar despite different names*

```diff
@@ -3,19 +3,17 @@
 from __future__ import annotations
 
 __all__: Final[list[str]] = [
     "preorder",
     "inorder",
     "postorder",
     "levelorder",
-    "reverse_inorder",
 ]
 
 from typing import Final, TypeVar
-from warnings import warn
 
 from nrw.datastructures import BinarySearchTree, BinaryTree, ComparableContentT, List
 
 _T = TypeVar("_T")
 
 
 def preorder(
@@ -58,21 +56,14 @@
         result.concat(inorder(tree.right_tree, reverse=reverse))
         result.append(tree.content)
         result.concat(inorder(tree.left_tree, reverse=reverse))
 
     return result
 
 
-def reverse_inorder(
-    tree: BinaryTree[_T] | BinarySearchTree[ComparableContentT],
-) -> List[_T | ComparableContentT]:  # pragma: no cover
-    warn("Use 'inorder(..., reverse=True)'", DeprecationWarning, stacklevel=2)
-    return inorder(tree, reverse=True)
-
-
 def postorder(
     tree: BinaryTree[_T] | BinarySearchTree[ComparableContentT],
     *,
     reverse: bool = False,
 ) -> List[_T | ComparableContentT]:
     result: List[_T | ComparableContentT] = List()
```

### Comparing `pynrw-1.4.2/nrw/database/_query_result.py` & `pynrw-1.5.0/nrw/database/_query_result.py`

 * *Files identical despite different names*

### Comparing `pynrw-1.4.2/nrw/database/_query_result.pyi` & `pynrw-1.5.0/nrw/database/_query_result.pyi`

 * *Files identical despite different names*

### Comparing `pynrw-1.4.2/nrw/database/msaccess.py` & `pynrw-1.5.0/nrw/database/msaccess.py`

 * *Files 1% similar despite different names*

```diff
@@ -43,15 +43,15 @@
 
         Für `MSAccess` wird nur `database` benötigt.
         """
         self._current_query_result: QueryResult | None = None
         self._message: str | None = None
 
         try:
-            self._connection = pyodbc.connect(
+            self._connection: pyodbc.Connection | None = pyodbc.connect(
                 f"Driver={{Microsoft Access Driver (*.mdb, *.accdb)}};DBQ={database};",
                 autocommit=True,
             )
         except Exception as exception:
             self._connection = None
             self._message = str(exception)
```

### Comparing `pynrw-1.4.2/nrw/database/msaccess.pyi` & `pynrw-1.5.0/nrw/database/msaccess.pyi`

 * *Files identical despite different names*

### Comparing `pynrw-1.4.2/nrw/database/mysql.py` & `pynrw-1.5.0/nrw/database/mysql.py`

 * *Files identical despite different names*

### Comparing `pynrw-1.4.2/nrw/database/mysql.pyi` & `pynrw-1.5.0/nrw/database/mysql.pyi`

 * *Files identical despite different names*

### Comparing `pynrw-1.4.2/nrw/database/sqlite.py` & `pynrw-1.5.0/nrw/database/sqlite.py`

 * *Files identical despite different names*

### Comparing `pynrw-1.4.2/nrw/database/sqlite.pyi` & `pynrw-1.5.0/nrw/database/sqlite.pyi`

 * *Files identical despite different names*

### Comparing `pynrw-1.4.2/nrw/datastructures/__init__.py` & `pynrw-1.5.0/nrw/datastructures/__init__.py`

 * *Files identical despite different names*

### Comparing `pynrw-1.4.2/nrw/datastructures/__init__.pyi` & `pynrw-1.5.0/nrw/datastructures/__init__.pyi`

 * *Files identical despite different names*

### Comparing `pynrw-1.4.2/nrw/datastructures/_binary_search_tree.py` & `pynrw-1.5.0/nrw/datastructures/_binary_search_tree.py`

 * *Files identical despite different names*

### Comparing `pynrw-1.4.2/nrw/datastructures/_binary_tree.py` & `pynrw-1.5.0/nrw/datastructures/_binary_tree.py`

 * *Files identical despite different names*

### Comparing `pynrw-1.4.2/nrw/datastructures/_comparable_content.py` & `pynrw-1.5.0/nrw/datastructures/_comparable_content.py`

 * *Files identical despite different names*

### Comparing `pynrw-1.4.2/nrw/datastructures/_edge.py` & `pynrw-1.5.0/nrw/datastructures/_edge.py`

 * *Files identical despite different names*

### Comparing `pynrw-1.4.2/nrw/datastructures/_graph.py` & `pynrw-1.5.0/nrw/datastructures/_graph.py`

 * *Files identical despite different names*

### Comparing `pynrw-1.4.2/nrw/datastructures/_list.py` & `pynrw-1.5.0/nrw/datastructures/_list.py`

 * *Files 0% similar despite different names*

```diff
@@ -236,14 +236,14 @@
             self._last = None
 
     def _get_previous(self, node: _ListNode[_T] | None) -> _ListNode[_T] | None:
         """Liefert den Vorgängerknoten des Knotens `node`. Ist die Liste leer, `node
         is None`, `node` nicht in der Liste oder `node` der erste Knoten der Liste,
         wird `None` zurückgegeben.
         """
-        if node is None or node == self._first or self.is_empty:
+        if node is None or node is self._first or self.is_empty:
             return None
 
         temp: _ListNode[_T] | None = self._first
         while temp is not None and temp.next_node is not node:
             temp = temp.next_node
         return temp
```

### Comparing `pynrw-1.4.2/nrw/datastructures/_queue.py` & `pynrw-1.5.0/nrw/datastructures/_queue.py`

 * *Files identical despite different names*

### Comparing `pynrw-1.4.2/nrw/datastructures/_stack.py` & `pynrw-1.5.0/nrw/datastructures/_stack.py`

 * *Files identical despite different names*

### Comparing `pynrw-1.4.2/nrw/datastructures/_vertex.py` & `pynrw-1.5.0/nrw/datastructures/_vertex.py`

 * *Files identical despite different names*

### Comparing `pynrw-1.4.2/nrw/network/__init__.pyi` & `pynrw-1.5.0/nrw/network/__init__.pyi`

 * *Files identical despite different names*

### Comparing `pynrw-1.4.2/nrw/network/_client.py` & `pynrw-1.5.0/nrw/network/_client.py`

 * *Files identical despite different names*

### Comparing `pynrw-1.4.2/nrw/network/_connection.py` & `pynrw-1.5.0/nrw/network/_connection.py`

 * *Files identical despite different names*

### Comparing `pynrw-1.4.2/nrw/network/_server.py` & `pynrw-1.5.0/nrw/network/_server.py`

 * *Files identical despite different names*

### Comparing `pynrw-1.4.2/pynrw.egg-info/PKG-INFO` & `pynrw-1.5.0/pynrw.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pynrw
-Version: 1.4.2
+Version: 1.5.0
 Summary: Materialien zu den zentralen NRW-Abiturprüfungen im Fach Informatik ab 2018 implementiert in Python.
 Author: realshouzy
 License: MIT
 Project-URL: Source, https://github.com/realshouzy/pynrw
 Keywords: nrw,datastructures,datenstrukturen,algorithms,algorithmen,education,bildung,abitur
 Platform: any
 Classifier: Programming Language :: Python :: 3 :: Only
@@ -106,21 +106,21 @@
 bst.insert(3)
 bst.insert(2)
 bst.insert(5)
 bst.insert(0)
 bst.insert(1)
 bst.insert(4)
 print(bst)
-#    _4_
-#   /   \
-#  _2   6
-# /  \ /
-# 0  3 5
+#       3__
+#      /   \
+#   __2     5
+#  /       /
+# 0       4
 #  \
-#  1
+#   1
 ```
 
 Des weiteren sind (triviale) Optimierungen vorgenommen worden:
 
 - Verwendung von [`__slots__`](https://docs.python.org/3/reference/datamodel.html#slots)
 - redundante Aufrufe werden weggelassen
 - interne Optimierungen bei Zuweisungen
```

### Comparing `pynrw-1.4.2/pynrw.egg-info/SOURCES.txt` & `pynrw-1.5.0/pynrw.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `pynrw-1.4.2/pyproject.toml` & `pynrw-1.5.0/pyproject.toml`

 * *Files identical despite different names*

