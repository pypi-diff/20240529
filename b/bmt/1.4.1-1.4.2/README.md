# Comparing `tmp/bmt-1.4.1.tar.gz` & `tmp/bmt-1.4.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "bmt-1.4.1.tar", max compression
+gzip compressed data, was "bmt-1.4.2.tar", max compression
```

## Comparing `bmt-1.4.1.tar` & `bmt-1.4.2.tar`

### file list

```diff
@@ -1,7 +1,7 @@
--rw-r--r--   0        0        0     1544 2024-05-14 19:58:20.563716 bmt-1.4.1/LICENSE
--rw-r--r--   0        0        0     1110 2024-05-14 19:58:20.563716 bmt-1.4.1/README.md
--rw-r--r--   0        0        0       31 2024-05-14 19:58:20.563716 bmt-1.4.1/bmt/__init__.py
--rw-r--r--   0        0        0    74545 2024-05-14 19:58:20.563716 bmt-1.4.1/bmt/toolkit.py
--rw-r--r--   0        0        0     3843 2024-05-14 19:58:20.567716 bmt-1.4.1/bmt/utils.py
--rw-r--r--   0        0        0     1585 2024-05-14 19:58:34.283641 bmt-1.4.1/pyproject.toml
--rw-r--r--   0        0        0     2544 1970-01-01 00:00:00.000000 bmt-1.4.1/PKG-INFO
+-rw-r--r--   0        0        0     1544 2024-05-28 23:18:03.848162 bmt-1.4.2/LICENSE
+-rw-r--r--   0        0        0     1110 2024-05-28 23:18:03.848162 bmt-1.4.2/README.md
+-rw-r--r--   0        0        0       31 2024-05-28 23:18:03.848162 bmt-1.4.2/bmt/__init__.py
+-rw-r--r--   0        0        0    77216 2024-05-28 23:18:03.848162 bmt-1.4.2/bmt/toolkit.py
+-rw-r--r--   0        0        0     3843 2024-05-28 23:18:03.848162 bmt-1.4.2/bmt/utils.py
+-rw-r--r--   0        0        0     1585 2024-05-28 23:18:15.104262 bmt-1.4.2/pyproject.toml
+-rw-r--r--   0        0        0     2544 1970-01-01 00:00:00.000000 bmt-1.4.2/PKG-INFO
```

### Comparing `bmt-1.4.1/LICENSE` & `bmt-1.4.2/LICENSE`

 * *Files identical despite different names*

### Comparing `bmt-1.4.1/README.md` & `bmt-1.4.2/README.md`

 * *Files identical despite different names*

### Comparing `bmt-1.4.1/bmt/toolkit.py` & `bmt-1.4.2/bmt/toolkit.py`

 * *Files 2% similar despite different names*

```diff
@@ -437,28 +437,44 @@
 
         Returns
         -------
         List[str]
             A list of elements
 
         """
-        association_elements = self.get_descendants("association")
         filtered_elements: List[str] = list()
         inverse_predicates: Optional[List[str]] = None
+        subject_categories_formatted = []
+        object_categories_formatted = []
+        predicates_formatted = []
+        association_elements = self.get_descendants("association")
+        if subject_categories:
+            for sc in subject_categories:
+                sc_formatted = format_element(self.get_element(sc))
+                subject_categories_formatted.append(sc_formatted)
+        if object_categories:
+            for oc in object_categories:
+                oc_formatted = format_element(self.get_element(oc))
+                object_categories_formatted.append(oc_formatted)
         if predicates:
+            for pred in predicates:
+                pred_formatted = format_element(self.get_element(pred))
+                predicates_formatted.append(pred_formatted)
             inverse_predicates = list()
-            for pred_curie in predicates:
+            for pred_curie in predicates_formatted:
                 predicate = self.get_element(pred_curie)
                 if predicate:
                     inverse_p = self.get_inverse(predicate.name)
                     if inverse_p:
                         inverse_predicates.append(inverse_p)
                 inverse_predicates = self._format_all_elements(elements=inverse_predicates, formatted=True)
 
-        if subject_categories or predicates or object_categories:
+
+
+        if subject_categories_formatted or predicates_formatted or object_categories_formatted:
             # This feels like a bit of a brute force approach as an implementation,
             # but we just use the list of all association names to retrieve each
             # association record for filtering against the constraints?
             for name in association_elements:
 
                 # although get_element() is Optional[Element],
                 # the association_elements all come from
@@ -467,18 +483,18 @@
 
                 # sanity checks, probably not necessary
                 # assert association, f"'{name}' not a Biolink Element?"
                 # assert isinstance(association, ClassDefinition), f"'{name}' not a ClassDefinition?"
 
                 # Try to match associations in the forward direction
                 if not(
-                    self.match_association(association, subject_categories, predicates, object_categories) or
+                    self.match_association(association, subject_categories_formatted, predicates_formatted, object_categories_formatted) or
                     (
                         match_inverses and
-                        self.match_association(association, object_categories, inverse_predicates, subject_categories)
+                        self.match_association(association, object_categories, inverse_predicates, subject_categories_formatted)
                     )
                 ):
                     continue
 
                 # this association is assumed to pass stipulated constraints
                 filtered_elements.append(association.name)
         else:
@@ -1586,19 +1602,74 @@
         bool
             That the named element is a valid mixin in Biolink Model
         """
         element = self.get_element(name)
         is_mixin = element.mixin if isinstance(element, Definition) else False
         return is_mixin
 
+    def is_symmetric(self, name: str) -> bool:
+        """
+        Checks if a given element identified by name, is a symmetric (predicate) slot.
+
+        Parameters
+        ----------
+        name: str
+            The name or alias of an element in the Biolink Model
+
+        Returns
+        -------
+        bool
+            That the named element is tagged as symmetric: true in Biolink Model
+        """
+        if not name:
+            return False
+        element: Optional[Element] = self.get_element(name)
+        if element is not None and element['symmetric']:
+            return True
+        else:
+            return False
+
     @lru_cache(CACHE_SIZE)
     def get_inverse(self, slot_name: str):
         return self.view.inverse(slot_name)
 
     @lru_cache(CACHE_SIZE)
+    def get_inverse_predicate(
+            self, predicate: Optional[str],
+            formatted: bool = False
+    ) -> Optional[str]:
+        """
+        Utility wrapper of logic to robustly test if a predicate exists and has an inverse.
+
+        Parameters
+        ----------
+        predicate: Optional[str]
+            CURIE or string name of predicate in the Biolink Model, for which the inverse is sought
+        formatted: bool
+            Whether to format element names as CURIEs
+
+        Returns
+        -------
+        Optional[str]
+            CURIE string of inverse predicate, if it exists; None otherwise
+        """
+        if predicate and self.is_predicate(predicate):
+            predicate_name = parse_name(predicate)
+            inverse_predicate_name = self.get_inverse(predicate_name)
+            if not inverse_predicate_name:
+                if self.is_symmetric(predicate_name):
+                    inverse_predicate_name = predicate_name
+                else:
+                    inverse_predicate_name = None
+            if inverse_predicate_name:
+                ip = self.get_element(inverse_predicate_name)
+                return format_element(ip) if formatted else str(ip.name)
+        return None
+
+    @lru_cache(CACHE_SIZE)
     def has_inverse(self, name: str) -> bool:
         """
         Determines whether the given name exists and has an inverse defined in the Biolink Model.
         An element is a predicate if it descends from `RELATED_TO` but this is
         not directly tested here (use the method 'is_predicate()' to be sure).
 
         Parameters
```

### Comparing `bmt-1.4.1/bmt/utils.py` & `bmt-1.4.2/bmt/utils.py`

 * *Files identical despite different names*

### Comparing `bmt-1.4.1/pyproject.toml` & `bmt-1.4.2/pyproject.toml`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "bmt"
-version = "1.4.1"
+version = "1.4.2"
 description = "Biolink Model Toolkit: A Python API for working with the Biolink Model"
 authors = ["Sierra Taylor Moxon <sierra.taylor@gmail.com>"]
 license = "BSD"
 
 readme = "README.md"
 repository = "https://github.com/biolink/biolink-model-toolkit"
 documentation = "https://biolink.github.io/biolink-model-toolkit/"
```

### Comparing `bmt-1.4.1/PKG-INFO` & `bmt-1.4.2/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: bmt
-Version: 1.4.1
+Version: 1.4.2
 Summary: Biolink Model Toolkit: A Python API for working with the Biolink Model
 Home-page: https://github.com/biolink/biolink-model-toolkit
 License: BSD
 Keywords: schema,linked data,data modeling,biolink,api
 Author: Sierra Taylor Moxon
 Author-email: sierra.taylor@gmail.com
 Requires-Python: >=3.9,<4.0
```

