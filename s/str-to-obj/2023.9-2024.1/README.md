# Comparing `tmp/str-to-obj-2023.9.tar.gz` & `tmp/str_to_obj-2024.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "str-to-obj-2023.9.tar", last modified: Wed Nov  8 18:02:50 2023, max compression
+gzip compressed data, was "str_to_obj-2024.1.tar", last modified: Wed May 29 15:47:26 2024, max compression
```

## Comparing `str-to-obj-2023.9.tar` & `str_to_obj-2024.1.tar`

### file list

```diff
@@ -1,31 +1,32 @@
-drwxr-xr-x   0 eric      (1000) users      (984)        0 2023-11-08 18:02:50.511308 str-to-obj-2023.9/
--rw-r--r--   0 eric      (1000) users      (984)      114 2022-10-14 06:42:17.000000 str-to-obj-2023.9/MANIFEST.in
--rw-r--r--   0 eric      (1000) users      (984)     5389 2023-11-08 18:02:50.511308 str-to-obj-2023.9/PKG-INFO
--rw-r--r--   0 eric      (1000) users      (984)      636 2023-10-05 17:10:51.000000 str-to-obj-2023.9/README-COPYRIGHT-utf8.txt
--rw-r--r--   0 eric      (1000) users      (984)    21778 2019-02-21 09:59:58.000000 str-to-obj-2023.9/README-LICENCE-utf8.txt
--rw-r--r--   0 eric      (1000) users      (984)     4495 2023-10-05 17:16:50.000000 str-to-obj-2023.9/README.rst
-drwxr-xr-x   0 eric      (1000) users      (984)        0 2023-11-08 18:02:50.511308 str-to-obj-2023.9/documentation/
-drwxr-xr-x   0 eric      (1000) users      (984)        0 2023-11-08 18:02:50.511308 str-to-obj-2023.9/documentation/wiki/
--rw-r--r--   0 eric      (1000) users      (984)     1964 2023-10-05 17:16:50.000000 str-to-obj-2023.9/documentation/wiki/description.asciidoc
--rw-r--r--   0 eric      (1000) users      (984)      104 2022-06-17 10:26:30.000000 str-to-obj-2023.9/pyproject.toml
--rw-r--r--   0 eric      (1000) users      (984)       38 2023-11-08 18:02:50.511308 str-to-obj-2023.9/setup.cfg
--rw-r--r--   0 eric      (1000) users      (984)     5757 2023-10-05 17:48:18.000000 str-to-obj-2023.9/setup.py
-drwxr-xr-x   0 eric      (1000) users      (984)        0 2023-11-08 18:02:50.511308 str-to-obj-2023.9/str_to_obj/
--rw-r--r--   0 eric      (1000) users      (984)     1735 2023-10-06 06:42:56.000000 str-to-obj-2023.9/str_to_obj/__init__.py
-drwxr-xr-x   0 eric      (1000) users      (984)        0 2023-11-08 18:02:50.511308 str-to-obj-2023.9/str_to_obj/interface/
--rw-r--r--   0 eric      (1000) users      (984)     2414 2023-11-08 13:31:49.000000 str-to-obj-2023.9/str_to_obj/interface/console.py
--rw-r--r--   0 eric      (1000) users      (984)     2488 2023-11-07 08:52:59.000000 str-to-obj-2023.9/str_to_obj/main.py
-drwxr-xr-x   0 eric      (1000) users      (984)        0 2023-11-08 18:02:50.511308 str-to-obj-2023.9/str_to_obj/task/
--rw-r--r--   0 eric      (1000) users      (984)     8468 2023-11-07 09:02:58.000000 str-to-obj-2023.9/str_to_obj/task/casting.py
--rw-r--r--   0 eric      (1000) users      (984)     2488 2023-10-06 06:24:40.000000 str-to-obj-2023.9/str_to_obj/task/inspection.py
-drwxr-xr-x   0 eric      (1000) users      (984)        0 2023-11-08 18:02:50.511308 str-to-obj-2023.9/str_to_obj/type/
--rw-r--r--   0 eric      (1000) users      (984)     3310 2023-11-08 18:00:22.000000 str-to-obj-2023.9/str_to_obj/type/annotation.py
--rw-r--r--   0 eric      (1000) users      (984)     2221 2023-10-05 17:55:05.000000 str-to-obj-2023.9/str_to_obj/type/hint.py
--rw-r--r--   0 eric      (1000) users      (984)     5715 2023-10-25 14:45:54.000000 str-to-obj-2023.9/str_to_obj/type/hint_tree.py
--rw-r--r--   0 eric      (1000) users      (984)     1575 2023-11-08 18:01:05.000000 str-to-obj-2023.9/str_to_obj/version.py
-drwxr-xr-x   0 eric      (1000) users      (984)        0 2023-11-08 18:02:50.511308 str-to-obj-2023.9/str_to_obj.egg-info/
--rw-r--r--   0 eric      (1000) users      (984)     5389 2023-11-08 18:02:50.000000 str-to-obj-2023.9/str_to_obj.egg-info/PKG-INFO
--rw-r--r--   0 eric      (1000) users      (984)      541 2023-11-08 18:02:50.000000 str-to-obj-2023.9/str_to_obj.egg-info/SOURCES.txt
--rw-r--r--   0 eric      (1000) users      (984)        1 2023-11-08 18:02:50.000000 str-to-obj-2023.9/str_to_obj.egg-info/dependency_links.txt
--rw-r--r--   0 eric      (1000) users      (984)        5 2023-11-08 18:02:50.000000 str-to-obj-2023.9/str_to_obj.egg-info/requires.txt
--rw-r--r--   0 eric      (1000) users      (984)       11 2023-11-08 18:02:50.000000 str-to-obj-2023.9/str_to_obj.egg-info/top_level.txt
+drwxr-xr-x   0 eric      (1000) users      (984)        0 2024-05-29 15:47:26.178431 str_to_obj-2024.1/
+-rwx------   0 eric      (1000) users      (984)      114 2022-10-14 06:42:17.000000 str_to_obj-2024.1/MANIFEST.in
+-rw-r--r--   0 eric      (1000) users      (984)     5389 2024-05-29 15:47:26.178431 str_to_obj-2024.1/PKG-INFO
+-rwx------   0 eric      (1000) users      (984)      636 2023-10-05 17:10:51.000000 str_to_obj-2024.1/README-COPYRIGHT-utf8.txt
+-rwx------   0 eric      (1000) users      (984)    21778 2019-02-21 09:59:58.000000 str_to_obj-2024.1/README-LICENCE-utf8.txt
+-rwx------   0 eric      (1000) users      (984)     4495 2023-10-05 17:16:50.000000 str_to_obj-2024.1/README.rst
+drwxr-xr-x   0 eric      (1000) users      (984)        0 2024-05-29 15:47:26.171765 str_to_obj-2024.1/documentation/
+drwxr-xr-x   0 eric      (1000) users      (984)        0 2024-05-29 15:47:26.175098 str_to_obj-2024.1/documentation/wiki/
+-rwx------   0 eric      (1000) users      (984)     1964 2023-10-05 17:16:50.000000 str_to_obj-2024.1/documentation/wiki/description.asciidoc
+-rwx------   0 eric      (1000) users      (984)      104 2022-06-17 10:26:30.000000 str_to_obj-2024.1/pyproject.toml
+-rw-r--r--   0 eric      (1000) users      (984)       38 2024-05-29 15:47:26.178431 str_to_obj-2024.1/setup.cfg
+-rwx------   0 eric      (1000) users      (984)     5757 2023-10-05 17:48:18.000000 str_to_obj-2024.1/setup.py
+drwxr-xr-x   0 eric      (1000) users      (984)        0 2024-05-29 15:47:26.175098 str_to_obj-2024.1/str_to_obj/
+-rwx------   0 eric      (1000) users      (984)     1735 2023-10-06 06:42:56.000000 str_to_obj-2024.1/str_to_obj/__init__.py
+drwxr-xr-x   0 eric      (1000) users      (984)        0 2024-05-29 15:47:26.175098 str_to_obj-2024.1/str_to_obj/interface/
+-rwx------   0 eric      (1000) users      (984)     2414 2023-11-08 13:31:49.000000 str_to_obj-2024.1/str_to_obj/interface/console.py
+-rwx------   0 eric      (1000) users      (984)     2488 2023-11-07 08:52:59.000000 str_to_obj-2024.1/str_to_obj/main.py
+drwxr-xr-x   0 eric      (1000) users      (984)        0 2024-05-29 15:47:26.178431 str_to_obj-2024.1/str_to_obj/task/
+-rwx------   0 eric      (1000) users      (984)     8468 2023-11-07 09:02:58.000000 str_to_obj-2024.1/str_to_obj/task/casting.py
+-rwx------   0 eric      (1000) users      (984)     2568 2024-05-23 15:08:59.000000 str_to_obj-2024.1/str_to_obj/task/comparison.py
+-rwx------   0 eric      (1000) users      (984)     2488 2023-10-06 06:24:40.000000 str_to_obj-2024.1/str_to_obj/task/inspection.py
+drwxr-xr-x   0 eric      (1000) users      (984)        0 2024-05-29 15:47:26.178431 str_to_obj-2024.1/str_to_obj/type/
+-rwx------   0 eric      (1000) users      (984)     3241 2023-11-09 08:50:45.000000 str_to_obj-2024.1/str_to_obj/type/annotation.py
+-rwx------   0 eric      (1000) users      (984)     2221 2023-10-05 17:55:05.000000 str_to_obj-2024.1/str_to_obj/type/hint.py
+-rwx------   0 eric      (1000) users      (984)     6113 2024-05-29 15:45:52.000000 str_to_obj-2024.1/str_to_obj/type/hint_tree.py
+-rwx------   0 eric      (1000) users      (984)     1609 2024-05-29 15:39:08.000000 str_to_obj-2024.1/str_to_obj/version.py
+drwxr-xr-x   0 eric      (1000) users      (984)        0 2024-05-29 15:47:26.178431 str_to_obj-2024.1/str_to_obj.egg-info/
+-rw-r--r--   0 eric      (1000) users      (984)     5389 2024-05-29 15:47:26.000000 str_to_obj-2024.1/str_to_obj.egg-info/PKG-INFO
+-rw-r--r--   0 eric      (1000) users      (984)      571 2024-05-29 15:47:26.000000 str_to_obj-2024.1/str_to_obj.egg-info/SOURCES.txt
+-rw-r--r--   0 eric      (1000) users      (984)        1 2024-05-29 15:47:26.000000 str_to_obj-2024.1/str_to_obj.egg-info/dependency_links.txt
+-rw-r--r--   0 eric      (1000) users      (984)        5 2024-05-29 15:47:26.000000 str_to_obj-2024.1/str_to_obj.egg-info/requires.txt
+-rw-r--r--   0 eric      (1000) users      (984)       11 2024-05-29 15:47:26.000000 str_to_obj-2024.1/str_to_obj.egg-info/top_level.txt
```

### Comparing `str-to-obj-2023.9/PKG-INFO` & `str_to_obj-2024.1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: str-to-obj
-Version: 2023.9
+Version: 2024.1
 Summary: Convert strings to Python objects guided by (potentially annotated) type hints
 Home-page: https://src.koda.cnrs.fr/eric.debreuve/str-to-obj/
 Author: Eric Debreuve
 Author-email: eric.debreuve@cnrs.fr
 License: CeCILL-2.1
 Project-URL: Documentation, https://src.koda.cnrs.fr/eric.debreuve/str-to-obj//-/wikis/home
 Project-URL: Source, https://src.koda.cnrs.fr/eric.debreuve/str-to-obj/
```

### Comparing `str-to-obj-2023.9/README-COPYRIGHT-utf8.txt` & `str_to_obj-2024.1/README-COPYRIGHT-utf8.txt`

 * *Files identical despite different names*

### Comparing `str-to-obj-2023.9/README-LICENCE-utf8.txt` & `str_to_obj-2024.1/README-LICENCE-utf8.txt`

 * *Files identical despite different names*

### Comparing `str-to-obj-2023.9/README.rst` & `str_to_obj-2024.1/README.rst`

 * *Files identical despite different names*

### Comparing `str-to-obj-2023.9/documentation/wiki/description.asciidoc` & `str_to_obj-2024.1/documentation/wiki/description.asciidoc`

 * *Files identical despite different names*

### Comparing `str-to-obj-2023.9/setup.py` & `str_to_obj-2024.1/setup.py`

 * *Files identical despite different names*

### Comparing `str-to-obj-2023.9/str_to_obj/__init__.py` & `str_to_obj-2024.1/str_to_obj/__init__.py`

 * *Files identical despite different names*

### Comparing `str-to-obj-2023.9/str_to_obj/interface/console.py` & `str_to_obj-2024.1/str_to_obj/interface/console.py`

 * *Files identical despite different names*

### Comparing `str-to-obj-2023.9/str_to_obj/main.py` & `str_to_obj-2024.1/str_to_obj/main.py`

 * *Files identical despite different names*

### Comparing `str-to-obj-2023.9/str_to_obj/task/casting.py` & `str_to_obj-2024.1/str_to_obj/task/casting.py`

 * *Files identical despite different names*

### Comparing `str-to-obj-2023.9/str_to_obj/task/inspection.py` & `str_to_obj-2024.1/str_to_obj/task/inspection.py`

 * *Files identical despite different names*

### Comparing `str-to-obj-2023.9/str_to_obj/type/annotation.py` & `str_to_obj-2024.1/str_to_obj/type/annotation.py`

 * *Files 3% similar despite different names*

```diff
@@ -53,18 +53,14 @@
         Annotated[there_is_no_other_choice_then_single_accepted_type, annotation_t(...)]
         and using:
         annotation_t.NewAnnotatedType(...)
         instead.
         """
         raise NotImplementedError
 
-    def Issues(self) -> list[str]:
-        """"""
-        return []
-
     def ValueIsCompliant(self, value: Any, /) -> list[str]:
         """"""
         types = self.__class__.ACCEPTED_TYPES
         stripe = type(value)
         if (Any in types) or (stripe in types) or issubclass(stripe, types):
             return []
```

### Comparing `str-to-obj-2023.9/str_to_obj/type/hint.py` & `str_to_obj-2024.1/str_to_obj/type/hint.py`

 * *Files identical despite different names*

### Comparing `str-to-obj-2023.9/str_to_obj/type/hint_tree.py` & `str_to_obj-2024.1/str_to_obj/type/hint_tree.py`

 * *Files 3% similar despite different names*

```diff
@@ -119,15 +119,28 @@
 
         if self.type is UnionType:
             return {_key: _elm.template for _key, _elm in enumerate(self.elements)}
 
         if self.elements is None:
             return self.type
 
-        return self.type(_elm.template for _elm in self.elements)
+        try:
+            output = self.type(_elm.template for _elm in self.elements)
+        except TypeError:
+            output = None
+        if output is not None:
+            return output
+
+        # TODO: Does it work all the time?
+        if self.elements.__len__() == 1:
+            # For example, self.type is typing.Sequence.
+            return self.type[self.elements[0].template]
+
+        # TODO: Can something better be done?
+        return self.type
 
     @property
     def template_as_str(self) -> str:
         """"""
         output = (
             str(self.template)
             .replace(str(EllipsisType), "...")
```

### Comparing `str-to-obj-2023.9/str_to_obj/version.py` & `str_to_obj-2024.1/str_to_obj/version.py`

 * *Files 4% similar despite different names*

```diff
@@ -25,8 +25,10 @@
 # requirements in conditions enabling the security of their systems and/or
 # data to be ensured and,  more generally, to use and operate it in the
 # same conditions as regards security.
 #
 # The fact that you are presently reading this means that you have had
 # knowledge of the CeCILL license and that you accept its terms.
 
-__version__ = "2023.9"
+__version__ = "2024.1"
+
+# TODO: Switch to issue-manager.
```

### Comparing `str-to-obj-2023.9/str_to_obj.egg-info/PKG-INFO` & `str_to_obj-2024.1/str_to_obj.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: str-to-obj
-Version: 2023.9
+Version: 2024.1
 Summary: Convert strings to Python objects guided by (potentially annotated) type hints
 Home-page: https://src.koda.cnrs.fr/eric.debreuve/str-to-obj/
 Author: Eric Debreuve
 Author-email: eric.debreuve@cnrs.fr
 License: CeCILL-2.1
 Project-URL: Documentation, https://src.koda.cnrs.fr/eric.debreuve/str-to-obj//-/wikis/home
 Project-URL: Source, https://src.koda.cnrs.fr/eric.debreuve/str-to-obj/
```

