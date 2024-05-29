# Comparing `tmp/simpn-1.2.0.tar.gz` & `tmp/simpn-1.2.1.tar.gz`

## Comparing `simpn-1.2.0.tar` & `simpn-1.2.1.tar`

### file list

```diff
@@ -1,13 +1,13 @@
--rw-r--r--   0        0        0      370 2020-02-02 00:00:00.000000 simpn-1.2.0/CHANGELOG.rst
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 simpn-1.2.0/simpn/__init__.py
--rw-r--r--   0        0        0      179 2020-02-02 00:00:00.000000 simpn-1.2.0/simpn/immutabletypes.py
--rw-r--r--   0        0        0    13797 2020-02-02 00:00:00.000000 simpn-1.2.0/simpn/prototypes.py
--rw-r--r--   0        0        0    16831 2020-02-02 00:00:00.000000 simpn-1.2.0/simpn/prototypes_queueing.py
--rw-r--r--   0        0        0    13403 2020-02-02 00:00:00.000000 simpn-1.2.0/simpn/reporters.py
--rw-r--r--   0        0        0    33413 2020-02-02 00:00:00.000000 simpn-1.2.0/simpn/simulator.py
--rw-r--r--   0        0        0    18193 2020-02-02 00:00:00.000000 simpn-1.2.0/simpn/visualisation.py
--rw-r--r--   0        0        0      564 2020-02-02 00:00:00.000000 simpn-1.2.0/.gitignore
--rw-r--r--   0        0        0     1111 2020-02-02 00:00:00.000000 simpn-1.2.0/LICENSE
--rw-r--r--   0        0        0     8892 2020-02-02 00:00:00.000000 simpn-1.2.0/README.rst
--rw-r--r--   0        0        0      911 2020-02-02 00:00:00.000000 simpn-1.2.0/pyproject.toml
--rw-r--r--   0        0        0    10576 2020-02-02 00:00:00.000000 simpn-1.2.0/PKG-INFO
+-rw-r--r--   0        0        0      532 2020-02-02 00:00:00.000000 simpn-1.2.1/CHANGELOG.rst
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 simpn-1.2.1/simpn/__init__.py
+-rw-r--r--   0        0        0      179 2020-02-02 00:00:00.000000 simpn-1.2.1/simpn/immutabletypes.py
+-rw-r--r--   0        0        0    13797 2020-02-02 00:00:00.000000 simpn-1.2.1/simpn/prototypes.py
+-rw-r--r--   0        0        0    16831 2020-02-02 00:00:00.000000 simpn-1.2.1/simpn/prototypes_queueing.py
+-rw-r--r--   0        0        0    13403 2020-02-02 00:00:00.000000 simpn-1.2.1/simpn/reporters.py
+-rw-r--r--   0        0        0    33413 2020-02-02 00:00:00.000000 simpn-1.2.1/simpn/simulator.py
+-rw-r--r--   0        0        0    18236 2020-02-02 00:00:00.000000 simpn-1.2.1/simpn/visualisation.py
+-rw-r--r--   0        0        0      564 2020-02-02 00:00:00.000000 simpn-1.2.1/.gitignore
+-rw-r--r--   0        0        0     1111 2020-02-02 00:00:00.000000 simpn-1.2.1/LICENSE
+-rw-r--r--   0        0        0     8892 2020-02-02 00:00:00.000000 simpn-1.2.1/README.rst
+-rw-r--r--   0        0        0      911 2020-02-02 00:00:00.000000 simpn-1.2.1/pyproject.toml
+-rw-r--r--   0        0        0    10576 2020-02-02 00:00:00.000000 simpn-1.2.1/PKG-INFO
```

### Comparing `simpn-1.2.0/simpn/prototypes.py` & `simpn-1.2.1/simpn/prototypes.py`

 * *Files identical despite different names*

### Comparing `simpn-1.2.0/simpn/prototypes_queueing.py` & `simpn-1.2.1/simpn/prototypes_queueing.py`

 * *Files identical despite different names*

### Comparing `simpn-1.2.0/simpn/reporters.py` & `simpn-1.2.1/simpn/reporters.py`

 * *Files identical despite different names*

### Comparing `simpn-1.2.0/simpn/simulator.py` & `simpn-1.2.1/simpn/simulator.py`

 * *Files identical despite different names*

### Comparing `simpn-1.2.0/simpn/visualisation.py` & `simpn-1.2.1/simpn/visualisation.py`

 * *Files 0% similar despite different names*

```diff
@@ -362,15 +362,16 @@
                     f.write(f"{node.get_id()},{node.get_pos()[0]},{node.get_pos()[1]}\n")
     
     def __load_layout(self, filename):
         with open(filename, "r") as f:
             self._size = tuple(map(int, f.readline().strip().split(",")))
             for line in f:
                 id, x, y = line.strip().split(",")
-                self._nodes[id].set_pos((int(x), int(y)))
+                if id in self._nodes:
+                    self._nodes[id].set_pos((int(x), int(y)))
 
     def __get_node_at(self, pos):
         for node in self._nodes.values():
             if node.get_pos()[0] - node._width/2 <= pos[0] <= node.get_pos()[0] + node._width/2 and node.get_pos()[1] - node._height/2 <= pos[1] <= node.get_pos()[1] + node._height/2:
                 return node
         return None
```

### Comparing `simpn-1.2.0/.gitignore` & `simpn-1.2.1/.gitignore`

 * *Files identical despite different names*

### Comparing `simpn-1.2.0/LICENSE` & `simpn-1.2.1/LICENSE`

 * *Files identical despite different names*

### Comparing `simpn-1.2.0/README.rst` & `simpn-1.2.1/README.rst`

 * *Files identical despite different names*

### Comparing `simpn-1.2.0/pyproject.toml` & `simpn-1.2.1/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["hatchling"]
 build-backend = "hatchling.build"
 
 [project]
 name = "simpn"
-version = "1.2.0"
+version = "1.2.1"
 authors = [
   { name="Remco Dijkman", email="r.m.dijkman@tue.nl" },
 ]
 description = "A package for Discrete Event Simulation, using the theory of Petri Nets."
 readme = "README.rst"
 requires-python = ">=3.9"
 license = {file = "LICENSE"}
```

### Comparing `simpn-1.2.0/PKG-INFO` & `simpn-1.2.1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.3
 Name: simpn
-Version: 1.2.0
+Version: 1.2.1
 Summary: A package for Discrete Event Simulation, using the theory of Petri Nets.
 Project-URL: Homepage, https://github.com/bpogroup/simpn
 Project-URL: Documentation, https://bpogroup.github.io/simpn/
 Author-email: Remco Dijkman <r.m.dijkman@tue.nl>
 License: Copyright (c) 2023 Remco Dijkman (Eindhoven University of Technology)
         
         Permission is hereby granted, free of charge, to any person obtaining a copy
```

