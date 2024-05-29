# Comparing `tmp/jageocoder-2.1.7.dev2.tar.gz` & `tmp/jageocoder-2.1.7.dev3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "jageocoder-2.1.7.dev2.tar", max compression
+gzip compressed data, was "jageocoder-2.1.7.dev3.tar", max compression
```

## Comparing `jageocoder-2.1.7.dev2.tar` & `jageocoder-2.1.7.dev3.tar`

### file list

```diff
@@ -1,20 +1,20 @@
--rw-r--r--   0        0        0      113 2024-05-08 05:06:37.205667 jageocoder-2.1.7.dev2/LICENSE
--rw-r--r--   0        0        0    10479 2024-05-21 05:03:13.340045 jageocoder-2.1.7.dev2/README.md
--rw-r--r--   0        0        0     1571 2024-05-21 05:06:11.091329 jageocoder-2.1.7.dev2/jageocoder/__init__.py
--rw-r--r--   0        0        0     5759 2024-05-08 03:51:15.514717 jageocoder-2.1.7.dev2/jageocoder/__main__.py
--rw-r--r--   0        0        0     3489 2024-05-14 07:28:53.462543 jageocoder-2.1.7.dev2/jageocoder/address.py
--rw-r--r--   0        0        0     8320 2024-04-15 00:39:35.469528 jageocoder-2.1.7.dev2/jageocoder/aza_master.py
--rw-r--r--   0        0        0     1171 2024-05-02 04:32:53.380509 jageocoder-2.1.7.dev2/jageocoder/dataset.py
--rw-r--r--   0        0        0      837 2024-05-08 03:51:15.514717 jageocoder-2.1.7.dev2/jageocoder/exceptions.py
--rw-r--r--   0        0        0    19415 2024-04-15 00:39:35.469528 jageocoder-2.1.7.dev2/jageocoder/itaiji.py
--rw-r--r--   0        0        0    14220 2023-08-03 02:25:59.209435 jageocoder-2.1.7.dev2/jageocoder/itaiji_dic.json
--rw-r--r--   0        0        0    16470 2024-05-13 05:54:01.596831 jageocoder-2.1.7.dev2/jageocoder/module.py
--rw-r--r--   0        0        0    55284 2024-05-15 04:29:24.686867 jageocoder-2.1.7.dev2/jageocoder/node.py
--rw-r--r--   0        0        0    11679 2024-05-20 07:49:12.679443 jageocoder-2.1.7.dev2/jageocoder/remote.py
--rw-r--r--   0        0        0     3898 2024-05-08 03:51:15.514717 jageocoder-2.1.7.dev2/jageocoder/result.py
--rw-r--r--   0        0        0    16645 2024-05-20 04:30:05.890848 jageocoder-2.1.7.dev2/jageocoder/rtree.py
--rw-r--r--   0        0        0     7795 2023-09-27 08:08:26.315234 jageocoder-2.1.7.dev2/jageocoder/strlib.py
--rw-r--r--   0        0        0    43706 2024-05-16 02:30:24.211931 jageocoder-2.1.7.dev2/jageocoder/tree.py
--rw-r--r--   0        0        0     4995 2023-08-03 02:25:59.213435 jageocoder-2.1.7.dev2/jageocoder/trie.py
--rw-r--r--   0        0        0     1308 2024-05-21 05:06:18.411466 jageocoder-2.1.7.dev2/pyproject.toml
--rw-r--r--   0        0        0    12021 1970-01-01 00:00:00.000000 jageocoder-2.1.7.dev2/PKG-INFO
+-rw-r--r--   0        0        0      113 2024-05-08 05:06:37.205667 jageocoder-2.1.7.dev3/LICENSE
+-rw-r--r--   0        0        0    10479 2024-05-21 05:12:27.142531 jageocoder-2.1.7.dev3/README.md
+-rw-r--r--   0        0        0     1571 2024-05-27 08:42:50.618126 jageocoder-2.1.7.dev3/jageocoder/__init__.py
+-rw-r--r--   0        0        0     5759 2024-05-08 03:51:15.514717 jageocoder-2.1.7.dev3/jageocoder/__main__.py
+-rw-r--r--   0        0        0     3489 2024-05-21 05:12:27.146530 jageocoder-2.1.7.dev3/jageocoder/address.py
+-rw-r--r--   0        0        0     8320 2024-04-15 00:39:35.469528 jageocoder-2.1.7.dev3/jageocoder/aza_master.py
+-rw-r--r--   0        0        0     1171 2024-05-02 04:32:53.380509 jageocoder-2.1.7.dev3/jageocoder/dataset.py
+-rw-r--r--   0        0        0      837 2024-05-08 03:51:15.514717 jageocoder-2.1.7.dev3/jageocoder/exceptions.py
+-rw-r--r--   0        0        0    19415 2024-04-15 00:39:35.469528 jageocoder-2.1.7.dev3/jageocoder/itaiji.py
+-rw-r--r--   0        0        0    14220 2023-08-03 02:25:59.209435 jageocoder-2.1.7.dev3/jageocoder/itaiji_dic.json
+-rw-r--r--   0        0        0    16470 2024-05-21 05:12:27.146530 jageocoder-2.1.7.dev3/jageocoder/module.py
+-rw-r--r--   0        0        0    55833 2024-05-29 02:17:31.044550 jageocoder-2.1.7.dev3/jageocoder/node.py
+-rw-r--r--   0        0        0    12219 2024-05-29 02:30:47.289873 jageocoder-2.1.7.dev3/jageocoder/remote.py
+-rw-r--r--   0        0        0     3898 2024-05-08 03:51:15.514717 jageocoder-2.1.7.dev3/jageocoder/result.py
+-rw-r--r--   0        0        0    20182 2024-05-28 09:35:05.185780 jageocoder-2.1.7.dev3/jageocoder/rtree.py
+-rw-r--r--   0        0        0     7795 2023-09-27 08:08:26.315234 jageocoder-2.1.7.dev3/jageocoder/strlib.py
+-rw-r--r--   0        0        0    44808 2024-05-29 02:36:07.055241 jageocoder-2.1.7.dev3/jageocoder/tree.py
+-rw-r--r--   0        0        0     4995 2023-08-03 02:25:59.213435 jageocoder-2.1.7.dev3/jageocoder/trie.py
+-rw-r--r--   0        0        0     1308 2024-05-27 08:42:50.626126 jageocoder-2.1.7.dev3/pyproject.toml
+-rw-r--r--   0        0        0    12021 1970-01-01 00:00:00.000000 jageocoder-2.1.7.dev3/PKG-INFO
```

### Comparing `jageocoder-2.1.7.dev2/README.md` & `jageocoder-2.1.7.dev3/README.md`

 * *Files identical despite different names*

### Comparing `jageocoder-2.1.7.dev2/jageocoder/__init__.py` & `jageocoder-2.1.7.dev3/jageocoder/__init__.py`

 * *Files 4% similar despite different names*

```diff
@@ -15,15 +15,15 @@
 running the following steps.
 
     >>> import jageocoder
     >>> jageocoder.init()
     >>> jageocoder.searchNode('<Japanese-address>')
 """
 
-__version__ = '2.1.7.dev2'  # The package version
+__version__ = '2.1.7.dev3'  # The package version
 __dictionary_version__ = '20230927'  # Compatible dictionary version
 __author__ = 'Takeshi Sagara <sagara@info-proto.com>'
 
 __all__ = [
     'init',
     'free',
     'is_initialized',
```

### Comparing `jageocoder-2.1.7.dev2/jageocoder/__main__.py` & `jageocoder-2.1.7.dev3/jageocoder/__main__.py`

 * *Files identical despite different names*

### Comparing `jageocoder-2.1.7.dev2/jageocoder/address.py` & `jageocoder-2.1.7.dev3/jageocoder/address.py`

 * *Files identical despite different names*

### Comparing `jageocoder-2.1.7.dev2/jageocoder/aza_master.py` & `jageocoder-2.1.7.dev3/jageocoder/aza_master.py`

 * *Files identical despite different names*

### Comparing `jageocoder-2.1.7.dev2/jageocoder/dataset.py` & `jageocoder-2.1.7.dev3/jageocoder/dataset.py`

 * *Files identical despite different names*

### Comparing `jageocoder-2.1.7.dev2/jageocoder/exceptions.py` & `jageocoder-2.1.7.dev3/jageocoder/exceptions.py`

 * *Files identical despite different names*

### Comparing `jageocoder-2.1.7.dev2/jageocoder/itaiji.py` & `jageocoder-2.1.7.dev3/jageocoder/itaiji.py`

 * *Files identical despite different names*

### Comparing `jageocoder-2.1.7.dev2/jageocoder/itaiji_dic.json` & `jageocoder-2.1.7.dev3/jageocoder/itaiji_dic.json`

 * *Files identical despite different names*

### Comparing `jageocoder-2.1.7.dev2/jageocoder/module.py` & `jageocoder-2.1.7.dev3/jageocoder/module.py`

 * *Files identical despite different names*

### Comparing `jageocoder-2.1.7.dev2/jageocoder/node.py` & `jageocoder-2.1.7.dev3/jageocoder/node.py`

 * *Files 1% similar despite different names*

```diff
@@ -66,14 +66,38 @@
             The converted object.
         """
         capnp_record = super().get_record(pos=pos)
         node = AddressNode.from_record(capnp_record)
         node.table = self
         return node
 
+    def search_ids_on(
+        self,
+        attr: str,
+        value: str,
+    ) -> list:
+        """
+        Search id list from the table on the specified attribute.
+
+        Paramters
+        ---------
+        attr: str
+            The name of target attribute.
+        value: str
+            The target value.
+
+        Returns
+        -------
+        List[int]
+            List of node ids.
+        """
+        trie = self.open_trie_on(attr)
+        positions = trie.get(value, [])
+        return [p[0] for p in positions]
+
     def create_indexes(self) -> None:
         """
         Create TRIE index on "name" and "note" columns.
         """
         def _split_note(note):
             notes = []
             for attr in re.split(r'(?<!\\)/', note):
@@ -510,15 +534,15 @@
 
         Notes
         -----
         - The duplicated values are not registered in the database.
         """
         new_node = copy.copy(self)
         for child in self.iter_children():
-            if child.y <= 90.0:
+            if child.has_valid_coordinate_values():
                 new_node.x, new_node.y = child.x, child.y
                 logger.debug((
                     "Node {}({}) has no coordinates. "
                     "Use the coordinates of the child {}({}) instead."
                 ).format(
                     self.name, self.id, child.name, child.id))
                 break
```

### Comparing `jageocoder-2.1.7.dev2/jageocoder/remote.py` & `jageocoder-2.1.7.dev3/jageocoder/remote.py`

 * *Files 3% similar despite different names*

```diff
@@ -180,14 +180,38 @@
         for record in rpc_result:
             node = AddressNode(**record)
             node.table = self
             nodes.append(node)
 
         return nodes
 
+    def search_ids_on(
+        self,
+        attr: str,
+        value: str,
+    ) -> list:
+        """
+        Search id from the table on the specified attribute on the remote server.
+
+        Paramters
+        ---------
+        attr: str
+            The name of target attribute.
+        value: str
+            The target value.
+
+        Returns
+        -------
+        List[Record]
+            List of records.
+        """
+        nodes = self.search_records_on(attr, value)
+        ids = [node.id for node in nodes]
+        return ids
+
 
 class RemoteTree(AddressTree):
     """
     The proxy class for remote server's address-tree structure.
 
     Attributes
     ----------
```

### Comparing `jageocoder-2.1.7.dev2/jageocoder/result.py` & `jageocoder-2.1.7.dev3/jageocoder/result.py`

 * *Files identical despite different names*

### Comparing `jageocoder-2.1.7.dev2/jageocoder/rtree.py` & `jageocoder-2.1.7.dev3/jageocoder/rtree.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,8 +1,9 @@
 from abc import ABC
+import copy
 from logging import getLogger
 import os
 from typing import Iterable, List, Optional, Tuple
 
 from geographiclib.geodesic import Geodesic
 from rtree import index
 from rtree.exceptions import RTreeError
@@ -11,14 +12,24 @@
 from jageocoder.tree import AddressTree
 from jageocoder.address import AddressLevel
 from jageocoder.node import AddressNode, AddressNodeTable
 
 logger = getLogger(__name__)
 
 
+class NodeDist(object):
+
+    def __init__(self, dist: float, node: AddressNode) -> None:
+        self.dist = dist
+        self.node = node
+
+    def __repr__(self) -> str:
+        return f"NodeDist({self.dist}, {self.node})"
+
+
 class DelaunayTriangle(ABC):
 
     @classmethod
     def p_contained_triangle(
         cls,
         p: Tuple[float, float],
         p0: Tuple[float, float],
@@ -127,47 +138,48 @@
         return False
 
     @classmethod
     def select(
         cls,
         x: float,
         y: float,
-        nodes: List[AddressNode]
-    ) -> List[AddressNode]:
+        nodes: List[NodeDist]
+    ) -> List[NodeDist]:
         """
         Select the 3 nodes that make the smallest triangle
         surrounding the target point.
 
         Parameters
         ----------
         x: float
             The longitude of the target point.
         y: float
             The latitude of the target point.
-        nodes: List[AddressNode]
-            The candidate nodes.
+        nodes: List[NodeDist]
+            The candidate list of (distance, node).
 
         Returns
         -------
-        List[AddressNode]
-            Up to 3 nodes surrounding the target point.
+        List[NodeDist]
+            Up to 3 nodes surrounding the target point
+            and their distance.
         """
         def kval(t: Tuple[int, int, int]) -> int:
             sval = sorted(t)
             return sval[0] * 10000 + sval[1] * 100 + sval[2]
 
         triangle = None
         for p0 in range(len(nodes) - 2):
             for p1 in range(p0 + 1, len(nodes) - 1):
                 for p2 in range(p1 + 1, len(nodes)):
                     if cls.p_contained_triangle(
                         (x, y),
-                        (nodes[p0].x, nodes[p0].y),
-                        (nodes[p1].x, nodes[p1].y),
-                        (nodes[p2].x, nodes[p2].y)
+                        (nodes[p0].node.x, nodes[p0].node.y),
+                        (nodes[p1].node.x, nodes[p1].node.y),
+                        (nodes[p2].node.x, nodes[p2].node.y)
                     ):
                         triangle = [p0, p1, p2]
                         break
 
                 if triangle is not None:
                     break
 
@@ -183,32 +195,32 @@
         processed_triangles = set({kval(triangle), })
         while i < len(nodes):
             if i in triangle:
                 i += 1
                 continue
 
             if cls.p_contained_circumcircle(
-                (nodes[i].x, nodes[i].y),
-                (nodes[triangle[0]].x, nodes[triangle[0]].y),
-                (nodes[triangle[1]].x, nodes[triangle[1]].y),
-                (nodes[triangle[2]].x, nodes[triangle[2]].y)
+                (nodes[i].node.x, nodes[i].node.y),
+                (nodes[triangle[0]].node.x, nodes[triangle[0]].node.y),
+                (nodes[triangle[1]].node.x, nodes[triangle[1]].node.y),
+                (nodes[triangle[2]].node.x, nodes[triangle[2]].node.y)
             ):
                 new_triangle = None
                 for j in range(3):
                     tt = triangle[:]
                     tt[j] = i
                     k = kval(tt)
                     if k in processed_triangles:
                         continue
 
                     if cls.p_contained_triangle(
                         (x, y),
-                        (nodes[tt[0]].x, nodes[tt[0]].y),
-                        (nodes[tt[1]].x, nodes[tt[1]].y),
-                        (nodes[tt[2]].x, nodes[tt[2]].y)
+                        (nodes[tt[0]].node.x, nodes[tt[0]].node.y),
+                        (nodes[tt[1]].node.x, nodes[tt[1]].node.y),
+                        (nodes[tt[2]].node.x, nodes[tt[2]].node.y)
                     ):
                         new_triangle = tt
                         break
 
                 if new_triangle:
                     triangle = new_triangle
                     processed_triangles.add(kval(triangle))
@@ -305,38 +317,37 @@
         index.Rtree
             Created rtree index.
         """
         file_idx = index.Rtree(str(treepath))
         node_table: AddressNodeTable = self._tree.address_nodes
 
         max_id = node_table.count_records()
+
+        logger.info("Building RTree for reverse geocoding...")
         id = AddressNode.ROOT_NODE_ID
         with tqdm(total=max_id, mininterval=0.5, ascii=True) as pbar:
             prev_id = 0
             while id < max_id:
                 pbar.update(id - prev_id)
                 prev_id = id
 
                 node = node_table.get_record(pos=id)
-                if node.level > AddressLevel.AZA:
-                    id = node.sibling_id
-                    continue
-                elif node.level < AddressLevel.OAZA:
+                if node.level <= AddressLevel.WARD or node.level > AddressLevel.BLOCK:
                     id += 1
                     continue
-                elif not node.has_valid_coordinate_values():
+
+                if not node.has_valid_coordinate_values():
                     node = node.add_dummy_coordinates()
-                    if not node.has_valid_coordinate_values():
-                        id += 1
-                        continue
 
-                file_idx.insert(
-                    id=id,
-                    coordinates=(node.x, node.y, node.x, node.y)
-                )
+                if node.has_valid_coordinate_values():
+                    file_idx.insert(
+                        id=id,
+                        coordinates=(node.x, node.y, node.x, node.y),
+                    )
+
                 id += 1
 
         return file_idx
 
     def load_rtree(self, treepath: os.PathLike) -> index.Rtree:
         """
         Load RTree from the data files.
@@ -362,53 +373,71 @@
         -------
         bool
             If the index passes the test, return True.
             Otherwise return False.
         """
         node_table = self._tree.address_nodes
         node = node_table.get_record(pos=node_table.count_records() // 2)
-        while node.level < AddressLevel.OAZA:
-            node = node_table.get_record(pos=node.id + 1)
 
-        while node.level > AddressLevel.AZA:
-            node = node.parent
+        while True:
+            while node.level < AddressLevel.BLOCK:
+                node = node_table.get_record(pos=node.id + 1)
+
+            while node.level > AddressLevel.BLOCK:
+                node = node.parent
+
+            if node.has_valid_coordinate_values():
+                break
+
+            node = node_table.get_record(pos=node.sibling_id)
 
-        return node.id in self.idx.nearest((node.x, node.y, node.x, node.y), 2)
+        results = tuple(self.idx.nearest((node.x, node.y, node.x, node.y), 20))
+        return len(results) > 0 and node.id in results
 
     def _sort_by_dist(
         self,
         lon: float,
         lat: float,
-        id_list: Iterable[int]
-    ) -> List[AddressNode]:
+        id_list: Iterable[int],
+        node_map: Optional[dict] = None,
+    ) -> Tuple[List[NodeDist], dict]:
         """
         Sort nodes by real(projected) distance from the target point.
 
         Paramters
         ---------
         lon: float
             The longitude of the target point.
         lat: float
             The latitude of the target point.
         id_list: Iterable[int]
             The list of node-id.
 
         Returns
         -------
-        List[AddressNode]
-            The sorted list of address nodes.
+        Tuple[List[NodeDist], dict]
+            The sorted list of (distance, address node) and a node map.
         """
+        node_map = node_map or {}
         results = []
-        for node_id in id_list:
-            node = self._tree.get_address_node(id=node_id)
-            dist = self.distance(node.x, node.y, lon, lat)
-            results.append((node, dist))
+        for node_id in set(id_list):
+            node = self._tree.get_node_by_id(node_id=node_id)
+            if not node.has_valid_coordinate_values():
+                node = node.add_dummy_coordinates()
 
-        results.sort(key=lambda x: x[1])
-        return [x[0] for x in results]
+            key = (node.x, node.y)
+            if key in node_map:
+                node_map[key].append(node)
+            else:
+                node_map[key] = [node]
+                dist = self.distance(node.x, node.y, lon, lat)
+                results.append(NodeDist(dist, node))
+
+        results.sort(key=lambda x: x.dist)
+        return (results, node_map)
 
     def nearest(
         self,
         x: float,
         y: float,
         level: Optional[int] = None,
         as_dict: Optional[bool] = True,
@@ -430,103 +459,171 @@
             in the "candidate" field.
 
         Returns
         -------
         [{"candidate":AddressNode or dict, "dist":float}]
             Returns the results of retrieval up to 3 nodes.
         """
-        level = level or AddressLevel.AZA
-
-        # Search nodes by Rtree Index
-        nodes = []
-        ancestors = set()
-        max_level = 0
-        for node in self._sort_by_dist(x, y, self.idx.nearest((x, y, x, y), 10)):
-            if node.id in ancestors:
-                continue
-
-            if not node.has_valid_coordinate_values():
-                node = node.add_dummy_coordinates()
 
-            nodes.append(node)
-            max_level = max(max_level, node.level)
-            # Ancestor nodes of registering node are excluded.
-            cur = node.parent
-            while cur is not None:
-                nodes = [node for node in nodes if node.id != cur.id]
-                ancestors.add(cur.id)
-                cur = cur.parent
-
-        if level > max_level:
-            # Search points in the higher levels
-            local_idx = index.Rtree()  # Create local rtree on memory
-            for node in nodes:
-                child_id = node.id
-                while child_id < node.sibling_id:
-                    child_node = self._tree.get_address_node(id=child_id)
-                    if child_node.level > level:
-                        child_id = child_node.parent.sibling_id
-                        continue
-                    elif not child_node.has_valid_coordinate_values():
-                        child_node = child_node.add_dummy_coordinates()
-                        if not child_node.has_valid_coordinate_values():
-                            child_id += 1
-                            continue
-
-                    local_idx.insert(
-                        id=child_id,
-                        coordinates=(
-                            child_node.x, child_node.y,
-                            child_node.x, child_node.y))
-                    child_id += 1
+        def _remove_parent_nodes(
+            candidates: Iterable[NodeDist]
+        ) -> List[NodeDist]:
+            ancestors = set()
+            max_level = 0
+            if len(candidates) == 0:
+                return []
 
             nodes = []
-            ancestors = set()
-            for node in self._sort_by_dist(x, y, local_idx.nearest((x, y, x, y), 20)):
+            for v in candidates:
+                dist, node = v.dist, v.node
                 if node.id in ancestors:
                     continue
 
                 if not node.has_valid_coordinate_values():
                     node = node.add_dummy_coordinates()
 
-                nodes.append(node)
-                # Ancestor nodes of registering node are excluded.
+                nodes.append(NodeDist(dist, node))
+                max_level = max(max_level, node.level)
+
+                # List ancestor nodes of registering node.
                 cur = node.parent
                 while cur is not None:
-                    nodes = [node for node in nodes if node.id != cur.id]
+                    # nodes = [node for node in nodes if node.id != cur.id]
                     ancestors.add(cur.id)
                     cur = cur.parent
 
+            # Exclude ancestor nodes
+            nodes = [node for node in nodes if node.node.id not in ancestors]
+            return nodes
+
+        def _get_k_nearest_child_nodes(
+            aza_node_dists: List[NodeDist],
+            *,
+            candidates: Optional[List[NodeDist]] = None,
+            node_map: Optional[dict] = None,
+            k: Optional[int] = 20,
+            min_k: Optional[int] = 0,
+            max_dist: Optional[float] = 500.0,
+        ) -> Tuple[List[NodeDist], dict]:
+            candidates = candidates or []
+            node_map = node_map or {}
+            for v in aza_node_dists:
+                dist, node = v.dist, v.node
+                child_id = node.id + 1
+                for child_id in range(node.id + 1, node.sibling_id):
+                    child_node = self._tree.get_node_by_id(
+                        node_id=child_id)
+                    if child_node.level > level:
+                        continue
+
+                    if not child_node.has_valid_coordinate_values():
+                        if child_node.level == level:
+                            continue
+
+                        child_node = child_node.add_dummy_coordinates()
+                        if not child_node.has_valid_coordinate_values():
+                            continue
+
+                    key = (child_node.x, child_node.y)
+                    if key in node_map:
+                        # A node with the same coordinates are already registered
+                        node_map[key].append(child_node)
+                        continue
+
+                    dist = self.distance(x, y, child_node.x, child_node.y)
+                    i = len(candidates)
+                    while i > 0:
+                        if dist >= candidates[i - 1].dist:
+                            break
+
+                        i -= 1
+
+                    if i < min_k or (i < k and dist <= max_dist):
+                        candidates.insert(i, NodeDist(dist, child_node))
+                        node_map[key] = [child_node]
+                        n = len(candidates)
+                        if n > k:
+                            delnode = candidates[k].node
+                            del candidates[k]
+                            delkey = (delnode.x, delnode.y)
+                            node_map[delkey].remove(delnode)
+                            if len(node_map[delkey]) == 0:
+                                del node_map[delkey]
+
+                        elif n > min_k and candidates[min_k].dist > max_dist:
+                            delnode = candidates[min_k].node
+                            del candidates[min_k]
+                            delkey = (delnode.x, delnode.y)
+                            node_map[delkey].remove(delnode)
+                            if len(node_map[delkey]) == 0:
+                                del node_map[delkey]
+
+            return (candidates, node_map)
+
+        level = level or AddressLevel.AZA
+
+        # Retrieve top k-nearest nodes using the R-tree index.
+        nearests = self.idx.nearest((x, y, x, y), 20)
+        node_dists, node_map = self._sort_by_dist(x, y, nearests)
+        node_dists = _remove_parent_nodes(node_dists)
+
+        if level > AddressLevel.BLOCK:
+            candidates, node_map = _get_k_nearest_child_nodes(
+                node_dists,
+                candidates=copy.copy(node_dists),
+                node_map=node_map,
+                min_k=1)
+
+            node_dists = _remove_parent_nodes(candidates)
+
         # Select the 3 nodes that make the smallest triangle
         # surrounding the target point
-        if len(nodes) == 0:
+        if len(node_dists) == 0:
             return []
 
-        if self.distance(x, y, nodes[0].x, nodes[0].y) < 1.0e-02:
+        if len(node_dists) <= 3 or node_dists[0].dist < 1.0e-02:
             # If the distance between the nearest point and the search point is
             # less than 1 cm, it returns three points in order of distance.
             # This is because the nearest point may not be included in
             # the search results due to a calculation error.
-            nodes = nodes[0:3]
+            node_dists = node_dists[0:3]
         else:
-            nodes = DelaunayTriangle.select(x, y, nodes)
+            node_dists = DelaunayTriangle.select(x, y, node_dists)
+
+        # Restore nodes with the same coordinates
+        if node_map is not None:
+            _node_dists = []
+            for v in node_dists:
+                dist, node = v.dist, v.node
+                key = (node.x, node.y)
+                for n in node_map[key]:
+                    _node_dists.append(NodeDist(dist, n))
+
+            node_dists = _node_dists
 
         # Convert nodes to the dict format.
         results = []
         registered = set()
-        for node in nodes:
+        for v in node_dists:
+            dist, node = v.dist, v.node
             while node.level > level:
                 node = node.parent
+                dist = None
+                if not node.has_valid_coordinate_values():
+                    node.x, node.y = v.node.x, v.node.y
 
             if node.id in registered:
                 continue
 
+            if dist is None:
+                dist = self.distance(x, y, node.x, node.y)
+
             results.append({
                 "candidate": node.as_dict() if as_dict else node,
-                "dist": self.distance(x, y, node.x, node.y)
+                "dist": dist
             })
             registered.add(node.id)
 
         # Sort by distance
         results = sorted(results, key=lambda r: r['dist'])
 
         return results
```

### Comparing `jageocoder-2.1.7.dev2/jageocoder/strlib.py` & `jageocoder-2.1.7.dev3/jageocoder/strlib.py`

 * *Files identical despite different names*

### Comparing `jageocoder-2.1.7.dev2/jageocoder/tree.py` & `jageocoder-2.1.7.dev3/jageocoder/tree.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,21 +1,18 @@
 from collections import OrderedDict
-import csv
-import json
 from logging import getLogger
 import os
 from pathlib import Path
 import re
 import site
 import sys
-from typing import Any, Union, List, Set, NoReturn, Optional, TextIO
+from typing import Any, Union, List, Set, Optional
 
 from deprecated import deprecated
 
-import jageocoder
 from jageocoder.address import AddressLevel
 from jageocoder.aza_master import AzaMaster
 from jageocoder.exceptions import AddressTreeException
 from jageocoder.itaiji import Converter
 from jageocoder.node import AddressNode, AddressNodeTable
 from jageocoder.result import Result
 from jageocoder.trie import AddressTrie, TrieNode
@@ -281,19 +278,21 @@
         Get the full node information by its id.
 
         Parameters
         ----------
         node_id: int
             The target node id.
 
-        Return
-        ------
+        Returns
+        -------
         AddressNode
         """
-        return self.address_nodes.get_record(node_id)
+        node = self.address_nodes.get_record(node_id)
+        node.tree = self
+        return node
 
     def search_nodes_by_codes(
             self,
             category: str,
             value: str) -> List[AddressNode]:
         """
         Search nodes by category and value.
@@ -312,14 +311,39 @@
         nodes = []
         pattern = '{}:{}'.format(category, value)
         nodes = self.address_nodes.search_records_on(
             attr="note", value=pattern)  # exact match
 
         return nodes
 
+    def search_ids_by_codes(
+            self,
+            category: str,
+            value: str) -> List[AddressNode]:
+        """
+        Search node ids by category and value.
+
+        Parameters
+        ----------
+        category: str
+            Category name such as 'jisx0402' or 'postcode'.
+        value: str
+            Target value.
+
+        Returns
+        -------
+        List[int]
+        """
+        ids = []
+        pattern = '{}:{}'.format(category, value)
+        ids = self.address_nodes.search_ids_on(
+            attr="note", value=pattern)  # exact match
+
+        return ids
+
     @deprecated("Use 'node.get_fullname()' instead of this method.")
     def get_node_fullname(self, node: Union[AddressNode, int]) -> List[str]:
         if isinstance(node, int):
             node = self.get_node_by_id(node)
 
         return node.get_fullname()
 
@@ -961,14 +985,15 @@
                         if min_part is None:
                             min_part = _part
                         else:
                             min_part = min(min_part, _part)
 
         return results
 
+    @deprecated(reason="Use 'get_node_by_id'.", version="2.1.7")
     def get_address_node(self, id: int) -> AddressNode:
         """
         Get address node from the tree by its id.
 
         Parameters
         ----------
         id: int
@@ -1167,25 +1192,38 @@
         - In either of the above cases, search for the address node whose machiaza-id
             matches the rest 7 characters in the corresponding municipality.
         - Otherwise, it searches for address nodes whose machiaza-id matches "id"
             from all municipalities. In this case, aza_id must be 7 characters.
         """
         if len(id) == 12:
             # jisx0402(5digits) + aza_id(7digits)
-            candidates = self.search_nodes_by_codes(
+            citynode = self.search_by_citycode(code=id[0:5])
+            if len(citynode) == 0:
+                return []
+
+            citynode = citynode[0]
+            candidates = self.search_ids_by_codes(
                 category="aza_id",
                 value=id[-7:])
-            nodes = [x for x in candidates if x.get_city_jiscode() == id[0:5]]
+            nodes = [self.address_nodes.get_record(x)
+                     for x in candidates
+                     if x >= citynode.id and x < citynode.sibling_id]
         elif len(id) == 13:
             # lasdec(6digits) + aza_id(7digits)
-            candidates = self.search_nodes_by_codes(
+            citynode = self.search_by_citycode(code=id[0:6])
+            if len(citynode) == 0:
+                return []
+
+            citynode = citynode[0]
+            candidates = self.search_ids_by_codes(
                 category="aza_id",
                 value=id[-7:])
-            nodes = [x for x in candidates
-                     if x.get_city_local_authority_code() == id[0:6]]
+            nodes = [self.address_nodes.get_record(x)
+                     for x in candidates
+                     if x >= citynode.id and x < citynode.sibling_id]
         else:
             nodes = self.search_nodes_by_codes(
                 category="aza_id",
                 value=id)
 
         return nodes
```

### Comparing `jageocoder-2.1.7.dev2/jageocoder/trie.py` & `jageocoder-2.1.7.dev3/jageocoder/trie.py`

 * *Files identical despite different names*

### Comparing `jageocoder-2.1.7.dev2/pyproject.toml` & `jageocoder-2.1.7.dev3/pyproject.toml`

 * *Files 9% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "jageocoder"
-version = "2.1.7.dev2"
+version = "2.1.7.dev3"
 description = "A Japanese-address geocoder for Python."
 authors = ["Takeshi Sagara <sagara@info-proto.com>"]
 repository = "https://github.com/t-sagara/jageocoder/"
 license = "The MIT License"
 readme = "README.md"
 documentation = "https://jageocoder.readthedocs.io/"
 packages = [
```

### Comparing `jageocoder-2.1.7.dev2/PKG-INFO` & `jageocoder-2.1.7.dev3/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: jageocoder
-Version: 2.1.7.dev2
+Version: 2.1.7.dev3
 Summary: A Japanese-address geocoder for Python.
 Home-page: https://github.com/t-sagara/jageocoder/
 License: The MIT License
 Author: Takeshi Sagara
 Author-email: sagara@info-proto.com
 Requires-Python: >=3.7,<4.0
 Classifier: License :: OSI Approved :: MIT License
```

