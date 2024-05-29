# Comparing `tmp/lift_utils-0.1.1.tar.gz` & `tmp/lift_utils-0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "lift_utils-0.1.1.tar", last modified: Tue May 21 05:38:23 2024, max compression
+gzip compressed data, was "lift_utils-0.2.tar", last modified: Wed May 29 11:39:34 2024, max compression
```

## Comparing `lift_utils-0.1.1.tar` & `lift_utils-0.2.tar`

### file list

```diff
@@ -1,30 +1,35 @@
-drwxrwxr-x   0 nate      (1000) nate      (1000)        0 2024-05-21 05:38:23.587240 lift_utils-0.1.1/
--rw-rw-r--   0 nate      (1000) nate      (1000)     1064 2024-05-06 15:10:19.000000 lift_utils-0.1.1/LICENSE
--rw-r--r--   0 nate      (1000) nate      (1000)     2367 2024-05-21 05:38:23.587240 lift_utils-0.1.1/PKG-INFO
--rw-rw-r--   0 nate      (1000) nate      (1000)      371 2024-05-21 05:31:57.000000 lift_utils-0.1.1/README.md
--rw-rw-r--   0 nate      (1000) nate      (1000)     1045 2024-05-21 05:18:17.000000 lift_utils-0.1.1/pyproject.toml
--rw-rw-r--   0 nate      (1000) nate      (1000)       38 2024-05-21 05:38:23.587240 lift_utils-0.1.1/setup.cfg
-drwxrwxr-x   0 nate      (1000) nate      (1000)        0 2024-05-21 05:38:23.579239 lift_utils-0.1.1/src/
-drwxrwxr-x   0 nate      (1000) nate      (1000)        0 2024-05-21 05:38:23.583239 lift_utils-0.1.1/src/lift_utils/
--rw-rw-r--   0 nate      (1000) nate      (1000)       37 2024-05-11 06:40:27.000000 lift_utils-0.1.1/src/lift_utils/__init__.py
--rw-rw-r--   0 nate      (1000) nate      (1000)    18158 2024-05-20 14:04:15.000000 lift_utils-0.1.1/src/lift_utils/base.py
--rw-rw-r--   0 nate      (1000) nate      (1000)     1326 2024-05-21 05:36:21.000000 lift_utils-0.1.1/src/lift_utils/config.py
--rw-rw-r--   0 nate      (1000) nate      (1000)     1646 2024-05-20 14:03:41.000000 lift_utils-0.1.1/src/lift_utils/datatypes.py
--rw-rw-r--   0 nate      (1000) nate      (1000)    11324 2024-05-20 17:27:59.000000 lift_utils-0.1.1/src/lift_utils/header.py
--rw-rw-r--   0 nate      (1000) nate      (1000)    30062 2024-05-20 17:27:40.000000 lift_utils-0.1.1/src/lift_utils/lexicon.py
--rw-rw-r--   0 nate      (1000) nate      (1000)     1056 2024-05-13 06:18:59.000000 lift_utils-0.1.1/src/lift_utils/lift.py
--rw-rw-r--   0 nate      (1000) nate      (1000)     1908 2024-05-20 17:21:25.000000 lift_utils-0.1.1/src/lift_utils/utils.py
-drwxrwxr-x   0 nate      (1000) nate      (1000)        0 2024-05-21 05:38:23.583239 lift_utils-0.1.1/src/lift_utils.egg-info/
--rw-r--r--   0 nate      (1000) nate      (1000)     2367 2024-05-21 05:38:23.000000 lift_utils-0.1.1/src/lift_utils.egg-info/PKG-INFO
--rw-rw-r--   0 nate      (1000) nate      (1000)      675 2024-05-21 05:38:23.000000 lift_utils-0.1.1/src/lift_utils.egg-info/SOURCES.txt
--rw-rw-r--   0 nate      (1000) nate      (1000)        1 2024-05-21 05:38:23.000000 lift_utils-0.1.1/src/lift_utils.egg-info/dependency_links.txt
--rw-rw-r--   0 nate      (1000) nate      (1000)       29 2024-05-21 05:38:23.000000 lift_utils-0.1.1/src/lift_utils.egg-info/requires.txt
--rw-rw-r--   0 nate      (1000) nate      (1000)       11 2024-05-21 05:38:23.000000 lift_utils-0.1.1/src/lift_utils.egg-info/top_level.txt
-drwxrwxr-x   0 nate      (1000) nate      (1000)        0 2024-05-21 05:38:23.583239 lift_utils-0.1.1/tests/
--rw-rw-r--   0 nate      (1000) nate      (1000)     7465 2024-05-19 08:46:35.000000 lift_utils-0.1.1/tests/test_base_readxml_v0_13_FW.py
--rw-rw-r--   0 nate      (1000) nate      (1000)     7793 2024-05-19 08:46:06.000000 lift_utils-0.1.1/tests/test_base_readxml_v0_15.py
--rw-rw-r--   0 nate      (1000) nate      (1000)     4372 2024-05-20 17:01:45.000000 lift_utils-0.1.1/tests/test_header_readxml_v0_13_FW.py
--rw-rw-r--   0 nate      (1000) nate      (1000)     4588 2024-05-20 17:03:29.000000 lift_utils-0.1.1/tests/test_header_readxml_v0_15.py
--rw-rw-r--   0 nate      (1000) nate      (1000)     8925 2024-05-20 17:05:30.000000 lift_utils-0.1.1/tests/test_lexicon_readxml_v0_13_FW.py
--rw-rw-r--   0 nate      (1000) nate      (1000)     8733 2024-05-20 09:09:34.000000 lift_utils-0.1.1/tests/test_lexicon_readxml_v0_15.py
--rw-rw-r--   0 nate      (1000) nate      (1000)      641 2024-05-20 17:31:03.000000 lift_utils-0.1.1/tests/test_lift_readxml_v0_13_FW.py
+drwxrwxr-x   0 nate      (1000) nate      (1000)        0 2024-05-29 11:39:34.709734 lift_utils-0.2/
+-rw-rw-r--   0 nate      (1000) nate      (1000)     1064 2024-05-06 15:10:19.000000 lift_utils-0.2/LICENSE
+-rw-r--r--   0 nate      (1000) nate      (1000)     2428 2024-05-29 11:39:34.709734 lift_utils-0.2/PKG-INFO
+-rw-rw-r--   0 nate      (1000) nate      (1000)      434 2024-05-29 11:34:45.000000 lift_utils-0.2/README.md
+-rw-rw-r--   0 nate      (1000) nate      (1000)     1045 2024-05-21 05:18:17.000000 lift_utils-0.2/pyproject.toml
+-rw-rw-r--   0 nate      (1000) nate      (1000)       38 2024-05-29 11:39:34.709734 lift_utils-0.2/setup.cfg
+drwxrwxr-x   0 nate      (1000) nate      (1000)        0 2024-05-29 11:39:34.697727 lift_utils-0.2/src/
+drwxrwxr-x   0 nate      (1000) nate      (1000)        0 2024-05-29 11:39:34.701730 lift_utils-0.2/src/lift_utils/
+-rw-rw-r--   0 nate      (1000) nate      (1000)      163 2024-05-29 11:34:45.000000 lift_utils-0.2/src/lift_utils/__init__.py
+-rw-rw-r--   0 nate      (1000) nate      (1000)    13790 2024-05-29 11:34:45.000000 lift_utils-0.2/src/lift_utils/base.py
+-rw-rw-r--   0 nate      (1000) nate      (1000)     1437 2024-05-29 11:34:45.000000 lift_utils-0.2/src/lift_utils/config.py
+-rw-rw-r--   0 nate      (1000) nate      (1000)     1906 2024-05-29 11:34:45.000000 lift_utils-0.2/src/lift_utils/datatypes.py
+-rw-rw-r--   0 nate      (1000) nate      (1000)     9251 2024-05-29 11:34:45.000000 lift_utils-0.2/src/lift_utils/header.py
+-rw-rw-r--   0 nate      (1000) nate      (1000)    30342 2024-05-29 11:34:45.000000 lift_utils-0.2/src/lift_utils/lexicon.py
+-rw-rw-r--   0 nate      (1000) nate      (1000)     8021 2024-05-29 11:34:45.000000 lift_utils-0.2/src/lift_utils/utils.py
+drwxrwxr-x   0 nate      (1000) nate      (1000)        0 2024-05-29 11:39:34.709734 lift_utils-0.2/src/lift_utils.egg-info/
+-rw-r--r--   0 nate      (1000) nate      (1000)     2428 2024-05-29 11:39:34.000000 lift_utils-0.2/src/lift_utils.egg-info/PKG-INFO
+-rw-rw-r--   0 nate      (1000) nate      (1000)      870 2024-05-29 11:39:34.000000 lift_utils-0.2/src/lift_utils.egg-info/SOURCES.txt
+-rw-rw-r--   0 nate      (1000) nate      (1000)        1 2024-05-29 11:39:34.000000 lift_utils-0.2/src/lift_utils.egg-info/dependency_links.txt
+-rw-rw-r--   0 nate      (1000) nate      (1000)       29 2024-05-29 11:39:34.000000 lift_utils-0.2/src/lift_utils.egg-info/requires.txt
+-rw-rw-r--   0 nate      (1000) nate      (1000)       11 2024-05-29 11:39:34.000000 lift_utils-0.2/src/lift_utils.egg-info/top_level.txt
+drwxrwxr-x   0 nate      (1000) nate      (1000)        0 2024-05-29 11:39:34.709734 lift_utils-0.2/tests/
+-rw-rw-r--   0 nate      (1000) nate      (1000)     8089 2024-05-29 11:34:45.000000 lift_utils-0.2/tests/test_base_readxml_v0_13_FW.py
+-rw-rw-r--   0 nate      (1000) nate      (1000)     7814 2024-05-29 11:34:45.000000 lift_utils-0.2/tests/test_base_readxml_v0_15.py
+-rw-rw-r--   0 nate      (1000) nate      (1000)     5677 2024-05-29 11:34:45.000000 lift_utils-0.2/tests/test_base_writexml_v0_13_FW.py
+-rw-rw-r--   0 nate      (1000) nate      (1000)     5773 2024-05-29 11:34:45.000000 lift_utils-0.2/tests/test_base_writexml_v0_15.py
+-rw-rw-r--   0 nate      (1000) nate      (1000)     4436 2024-05-29 11:34:45.000000 lift_utils-0.2/tests/test_header_readxml_v0_13_FW.py
+-rw-rw-r--   0 nate      (1000) nate      (1000)     4885 2024-05-29 11:34:45.000000 lift_utils-0.2/tests/test_header_readxml_v0_15.py
+-rw-rw-r--   0 nate      (1000) nate      (1000)     4272 2024-05-29 11:34:45.000000 lift_utils-0.2/tests/test_header_writexml_v0_13_FW.py
+-rw-rw-r--   0 nate      (1000) nate      (1000)     4267 2024-05-29 11:34:45.000000 lift_utils-0.2/tests/test_header_writexml_v0_15.py
+-rw-rw-r--   0 nate      (1000) nate      (1000)     9203 2024-05-29 11:34:45.000000 lift_utils-0.2/tests/test_lexicon_readxml_v0_13_FW.py
+-rw-rw-r--   0 nate      (1000) nate      (1000)     8998 2024-05-29 11:34:45.000000 lift_utils-0.2/tests/test_lexicon_readxml_v0_15.py
+-rw-rw-r--   0 nate      (1000) nate      (1000)     4318 2024-05-29 11:34:45.000000 lift_utils-0.2/tests/test_lexicon_v0_13_FW.py
+-rw-rw-r--   0 nate      (1000) nate      (1000)     9189 2024-05-29 11:34:45.000000 lift_utils-0.2/tests/test_lexicon_writexml_v0_13_FW.py
+-rw-rw-r--   0 nate      (1000) nate      (1000)     9189 2024-05-29 11:34:45.000000 lift_utils-0.2/tests/test_lexicon_writexml_v0_15.py
```

### Comparing `lift_utils-0.1.1/LICENSE` & `lift_utils-0.2/LICENSE`

 * *Files identical despite different names*

### Comparing `lift_utils-0.1.1/PKG-INFO` & `lift_utils-0.2/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: lift_utils
-Version: 0.1.1
+Version: 0.2
 Summary: Read and write LIFT files in Python.
 Author-email: Nate Marti <nate_marti@sil.org>
 License: MIT License
         
         Copyright (c) 2024 SIL-CAR
         
         Permission is hereby granted, free of charge, to any person obtaining a copy
@@ -46,14 +46,18 @@
 ## Releases
 
 Install from [PyPI.org/lift-utils](https://pypi.org/project/lift-utils/):
 ```shell
 python3 -m pip install lift_utils
 ```
 
+## Documentation
+
+https://sil-car.github.io/lift-utils
+
 ## Roadmap
 
 | Release | Feature |
 | --: | --- |
 | v0.1 | read support for LIFT files |
 | v0.2 | write support for LIFT files |
-| v0.3 | add helper methods (get, set, add, list, etc.) |
+| v0.3 | add helper methods to facilitate lexicon manipulation |
```

### Comparing `lift_utils-0.1.1/pyproject.toml` & `lift_utils-0.2/pyproject.toml`

 * *Files identical despite different names*

### Comparing `lift_utils-0.1.1/src/lift_utils/base.py` & `lift_utils-0.2/src/lift_utils/base.py`

 * *Files 24% similar despite different names*

```diff
@@ -10,580 +10,441 @@
 from .datatypes import DateTime
 from .datatypes import Key
 from .datatypes import Lang
 from .datatypes import Prop
 from .datatypes import Props
 from .datatypes import URL
 from .utils import etree_to_obj_attributes
+from .utils import etree_to_xmlstring
+from .utils import obj_attributes_to_etree
 
 
 class LIFTUtilsBase:
     """This is a base class for all LIFT-related objects in this package.
 
-    :ivar etree xml_tree: The object's current data.
+    :ivar etree._Element xml_tree: The object's current data.
     """
-    def __init__(self, xml_tree: etree = None):
-        self.xml_tree = None
-        if xml_tree is not None:
-            self._update_from_xml(xml_tree)
-
-    def to_xml(self):
-        """Convert the object's data to XML."""
-        return etree.tostring(
-            self.xml_tree,
-            encoding='UTF-8',
-            pretty_print=True,
-            xml_declaration=True
-        ).decode().rstrip()
+    def __init__(self, xml_tree: etree._Element = None):
+        self.xml_tree = xml_tree
+        self.xml_tag = None
+        self.props = Props(lift_version=config.LIFT_VERSION)
+        self.props.attributes = []
+        self.props.elements = []
 
-    def print(self, format='xml'):
+    def print(self, _format='xml'):
         """Print the object's data to stdout; as XML by default."""
+        self.xml_tree = self._to_xml_tree()
         try:
-            if format == 'xml':
-                print(self.to_xml(), flush=True)
+            if _format == 'xml':
+                print(self._to_xml(), flush=True)
             else:
                 return
         except BrokenPipeError:
             sys.stdout = None
 
     def _update_from_xml(self, xml_tree):
+        # Set initial xml_tree.
         self.xml_tree = xml_tree
+        # Update object attributes.
+        etree_to_obj_attributes(xml_tree, self)
+
+    def _to_xml_tree(self):
+        xml_tree = obj_attributes_to_etree(self, self.xml_tag)
+        return xml_tree
+
+    def _to_xml(self, xml_tree=None):
+        if xml_tree is None:
+            xml_tree = self._to_xml_tree()
+        return etree_to_xmlstring(xml_tree)
 
 
 class Span(LIFTUtilsBase):
     """A Unicode string marked with language and formatting information.
     """
 
     def __init__(
         self,
-        xml_tree: Optional[etree.ElementTree] = None
+        xml_tree: Optional[etree._Element] = None
     ):
         super().__init__()
-        if xml_tree is not None:
-            super()._update_from_xml(xml_tree)
         # properties
-        self.props = Props(lift_version=config.LIFT_VERSION)
-        self.props.attributes = [
+        attribs = [
             Prop('lang', prop_type=Lang),
             Prop('href', prop_type=URL),
             Prop('class_', prop_type=str),
         ]
-        self.props.elements = [
+        for a in attribs:
+            self.props.add_to('attributes', a)
+        elems = [
             Prop('pcdata', required=True, prop_type=PCData),
-            Prop('spans', prop_type=list, item_type=Span),
+            Prop('tail', prop_type=PCData),
+            Prop('span_items', prop_type=list, item_type=Span),
         ]
+        for e in elems:
+            self.props.add_to('elements', e)
+        self.xml_tag = 'span'
         # attributes
         self.lang: Optional[Lang] = None
         self.href: Optional[URL] = None
         self.class_: Optional[str] = None
         # elements
         self.pcdata: PCData = None
-        self.spans: Optional[List[Span]] = None
+        self.tail: Optional[PCData] = None
+        self.span_items: Optional[List[Span]] = None
 
         if xml_tree is not None:
             self._update_from_xml(xml_tree)
 
-    def _update_from_xml(self, xml_tree):
-        self.xml_tree = xml_tree
-
-        # Update object attributes.
-        etree_to_obj_attributes(xml_tree, self)
-
-    def _build_xml_tree(self):
-        # This is basically the reverse function of _update_from_xml.
-        root_tag = 'span'
-        root = etree.Element(root_tag)
-        for attrib in self.props.attributes:
-            a = attrib.name
-            root.set(a, self.__dict__.get(a))
-        for elem in self.props.elements:
-            e = elem.name
-            if isinstance(self.__dict__.get(e), list):
-                for i in self.__dict__.get(e):
-                    etree.SubElement(root, e[:-1])
-            elif hasattr(self.__dict__.get(e), 'xml_tree'):
-                e._build_xml_tree()
-            elif e == 'pcdata':
-                root.text = self.__dict__.get(e)
-            elif self.__dict__.get(e):
-                etree.SubElement(root, e)
-        return root
-
 
 class Trait(LIFTUtilsBase):
     """An important mechanism for giving type information to an object.
     It can also be used for adding binary constraints.
     """
 
     def __init__(
         self,
-        xml_tree: Optional[etree.ElementTree] = None
+        xml_tree: Optional[etree._Element] = None
     ):
         super().__init__()
-        if xml_tree is not None:
-            super()._update_from_xml(xml_tree)
         # properties
-        self.props = Props(lift_version=config.LIFT_VERSION)
-        self.props.attributes = [
+        attribs = [
             Prop('name', required=True, prop_type=Key),
             Prop('value', required=True, prop_type=Key),
             Prop('id', prop_type=Key),
         ]
-        self.props.elements = [
-            Prop('annotations', prop_type=list, item_type=Annotation),
-        ]
+        for a in attribs:
+            self.props.add_to('attributes', a)
+        self.props.add_to(
+            'elements',
+            Prop('annotation_items', prop_type=list, item_type=Annotation)
+        )
+        self.xml_tag = 'trait'
         # attributes
         self.name: Key = None
         self.value: Key = None
         self.id: Optional[Key] = None
         # elements
-        self.annotations: Optional[List[Annotation]] = None
+        self.annotation_items: Optional[List[Annotation]] = None
 
         if xml_tree is not None:
             self._update_from_xml(xml_tree)
 
     def __str__(self):
         return f"{self.name}: {self.value}"
 
-    def _update_from_xml(self, xml_tree):
-        self.xml_tree = xml_tree
-
-        # Update object attributes.
-        etree_to_obj_attributes(xml_tree, self)
-
-    def _build_xml_tree(self):
-        # This is basically the reverse function of _update_from_xml.
-        root_tag = 'trait'
-        root = etree.Element(root_tag)
-        for attrib in self.props.attributes:
-            a = attrib.name
-            root.set(a, self.__dict__.get(a))
-        for elem in self.props.elements:
-            e = elem.name
-            if isinstance(self.__dict__.get(e), list):
-                # list element
-                for i in self.__dict__.get(e):
-                    if hasattr(self.__dict__.get(e), 'xml_tree'):
-                        root.append(e._build_xml_tree())
-                    else:
-                        etree.SubElement(root, e[:-1])
-            elif hasattr(self.__dict__.get(e), 'xml_tree'):
-                # element with own xml_tree to be generated
-                root.append(e._build_xml_tree())
-            elif e == 'pcdata':
-                # text data
-                root.text = self.__dict__.get(e)
-                # new empty element
-            elif self.__dict__.get(e):
-                etree.SubElement(root, e)
-        return root
-
 
 class Flag(Trait):
     """An important mechanism for giving type information to an object.
     It can also be use for adding binary constraints.
 
     .. note:: Used by LIFT v0.13 (FieldWorks). Mentioned in specification but
         not defined; assumed to be equivalent to ``Trait``.
     """
 
     def __init__(
         self,
-        xml_tree: Optional[etree.ElementTree] = None
+        xml_tree: Optional[etree._Element] = None
+    ):
+        super().__init__()
+
+
+class Text(LIFTUtilsBase):
+    """Contains textual data mixed with ``span`` elements only.
+    """
+
+    def __init__(
+        self,
+        text: PCData = None,
+        xml_tree: Optional[etree._Element] = None
     ):
         super().__init__()
+        # properties
+        elems = [
+            Prop('pcdata', required=True, prop_type=PCData),
+            Prop('span_items', prop_type=list, item_type=Span),
+        ]
+        for e in elems:
+            self.props.add_to('elements', e)
+        self.xml_tag = 'text'
+        # elements
+        self.pcdata = text
+        self.span_items: Optional[List[Span]] = None
         if xml_tree is not None:
-            super()._update_from_xml(xml_tree)
+            self._update_from_xml(xml_tree)
+
+    def __str__(self):
+        if self.span_items:
+            s = f"{str(self.pcdata)}{''.join(str(s) for s in self.span_items)}"
+        else:
+            s = str(self.pcdata)
+        return s
 
 
 class Form(LIFTUtilsBase):
     """A representation of a string in a particular language and script.
     This is specified by the ``lang`` attribute.
     """
 
     def __init__(
         self,
-        xml_tree: Optional[etree.ElementTree] = None
+        lang: Lang = None,
+        text: Text = None,
+        xml_tree: Optional[etree._Element] = None
     ):
         super().__init__()
-        if xml_tree is not None:
-            super()._update_from_xml(xml_tree)
         # properties
-        self.props = Props(lift_version=config.LIFT_VERSION)
-        self.props.attributes = [
-            Prop('lang', required=True, prop_type=Lang),
-        ]
-        self.props.elements = [
+        self.props.add_to(
+            'attributes',
+            Prop('lang', required=True, prop_type=Lang)
+        )
+        elems = [
             Prop('text', required=True, prop_type=Text),
-            Prop('annotations', prop_type=list, item_type=Annotation),
+            Prop('annotation_items', prop_type=list, item_type=Annotation),
         ]
+        for e in elems:
+            self.props.add_to('elements', e)
+        self.xml_tag = 'form'
         # attributes
-        self.lang: Lang = None
+        self.lang = lang
         # elements
-        self.text: Text = None
-        self.annotations: Optional[List[Annotation]] = None
+        self.text = text
+        self.annotation_items: Optional[List[Annotation]] = None
 
         if xml_tree is not None:
             self._update_from_xml(xml_tree)
 
     def __str__(self):
         return str(self.text)
 
-    def _update_from_xml(self, xml_tree):
-        self.xml_tree = xml_tree
-
-        # Update object attributes.
-        etree_to_obj_attributes(xml_tree, self)
-
-    def _update_other_from_self(self, other):
-        other.lang = self.lang
-        other.text = self.text
-        other.annotations = self.annotations
-
-
-class Text(Form):
-    """Contains textual data mixed with ``span`` elements only.
 
-    .. note:: It only inherits from ``Form`` in LIFT v0.13 (FieldWorks).
+class URLRef(LIFTUtilsBase):
+    """This is a URL with a caption.
     """
 
     def __init__(
         self,
-        text=None,
-        xml_tree: Optional[etree.ElementTree] = None
+        href: URL = None,
+        xml_tree: Optional[etree._Element] = None
     ):
         super().__init__()
-        if xml_tree is not None:
-            super()._update_from_xml(xml_tree)
         # properties
-        self.props = Props(lift_version=config.LIFT_VERSION)
-        self.props.elements = [
-            Prop('pcdata', required=True, prop_type=PCData),
-            Prop('spans', prop_type=list, item_type=Span),
-        ]
+        self.props.add_to(
+            'attributes',
+            Prop('href', required=True, prop_type=URL)
+        )
+        self.props.add_to(
+            'elements',
+            Prop('label', prop_type=Multitext)
+        )
+        self.xml_tag = 'urlref'
+        # attributes
+        self.href = href
         # elements
-        self.pcdata: str = None
-        if text is not None:
-            self.pcdata = PCData(text)
-        self.spans: Optional[List[Span]] = None
+        self.label: Optional[Multitext] = None
+
         if xml_tree is not None:
             self._update_from_xml(xml_tree)
 
-    def _update_from_xml(self, xml_tree):
-        self.xml_tree = xml_tree
-
-        f = Form(xml_tree)
-        f._update_other_from_self(self)
-        del f
-
-        # Update object attributes.
-        etree_to_obj_attributes(xml_tree, self)
-
-    def __str__(self):
-        return str(self.pcdata)
-
-    def _update_other_from_self(self, other):
-        other.pcdata = self.pcdata
-        other.spans = self.spans
-
 
 class Multitext(Text):
     """Allows for different representations of the same information.
     It can be in a given language, or in multiple languages.
     """
 
     def __init__(
         self,
-        xml_tree: Optional[etree.ElementTree] = None
+        xml_tree: Optional[etree._Element] = None
     ):
         super().__init__()
-        if xml_tree is not None:
-            super()._update_from_xml(xml_tree)
         # properties
-        self.props = Props(lift_version=config.LIFT_VERSION)
-        self.props.elements = [
-            Prop('forms', prop_type=list, item_type=Form),
-            Prop('text', prop_type=str),
-        ]
+        elems = [
+            Prop('form_items', prop_type=list, item_type=Form),
+            Prop('trait_items', prop_type=list, item_type=Trait),
+        ]
+        for e in elems:
+            self.props.add_to('elements', e)
+        # Multitext is only used as a super class for other classes, so it
+        # doesn't have it's own XML tag.
+        self.xml_tag = None
         # elements
-        self.forms: Optional[List[Form]] = None
-        self.text: Optional[str] = None  # deprecated in v0.15
+        self.form_items: Optional[List[Form]] = None
+        self.trait_items: Optional[List[Trait]] = None
 
         if xml_tree is not None:
             self._update_from_xml(xml_tree)
 
     def __str__(self):
         s = 'multitext'
-        if self.forms:
-            self.forms.sort()
-            s = f"{self.forms[0].text} ({self.forms[0].lang})"
-            ct = len(self.forms)
+        if self.form_items:
+            self.form_items.sort()
+            s = f"{self.form_items[0].text} ({self.form_items[0].lang})"
+            ct = len(self.form_items)
             if ct > 1:
                 s = f"{s} ({ct} forms)"
         return s
 
-    def _update_from_xml(self, xml_tree):
-        self.xml_tree = xml_tree
-
-        if config.LIFT_VERSION == '0.13':
-            txt = Text(xml_tree)
-            txt._update_other_from_self(self)
-            del txt
-
-        # Update object attributes.
-        etree_to_obj_attributes(xml_tree, self)
-
-    def _update_other_from_self(self, other):
-        other.forms = self.forms
-        other.text = self.text
-
 
 class Gloss(Form):
     """A representation of a sense's gloss.
     It's given in a particular language and script as specified by the ``lang``
     attribute.
     """
 
     def __init__(
         self,
-        xml_tree: Optional[etree.ElementTree] = None
+        xml_tree: Optional[etree._Element] = None
     ):
         super().__init__()
-        if xml_tree is not None:
-            super()._update_from_xml(xml_tree)
         # properties
-        self.props = Props(lift_version=config.LIFT_VERSION)
-        self.props.elements = [
-            Prop('traits', prop_type=list, item_type=Trait),
-        ]
+        self.props.add_to(
+            'elements',
+            Prop('trait_items', prop_type=list, item_type=Trait)
+        )
+        self.xml_tag = 'gloss'
         # elements
-        self.traits: Optional[List[Trait]] = None
+        self.trait_items: Optional[List[Trait]] = None
 
         if xml_tree is not None:
             self._update_from_xml(xml_tree)
 
     def __str__(self):
         return f"{self.text} ({self.lang})"
 
-    def _update_from_xml(self, xml_tree):
-        self.xml_tree = xml_tree
-
-        form = Form(xml_tree)
-        form._update_other_from_self(self)
-        del form
-
-        # Update object attributes.
-        etree_to_obj_attributes(xml_tree, self)
-
-
-class URLRef(LIFTUtilsBase):
-    """This is a URL with a caption.
-    """
-
-    def __init__(
-        self,
-        xml_tree: Optional[etree.ElementTree] = None
-    ):
-        super().__init__()
-        if xml_tree is not None:
-            super()._update_from_xml(xml_tree)
-        # properties
-        self.props = Props(lift_version=config.LIFT_VERSION)
-        self.props.attributes = [
-            Prop('href', required=True, prop_type=URL),
-        ]
-        self.props.elements = [
-            Prop('label', prop_type=Multitext),
-        ]
-        # attributes
-        self.href: URL = None
-        # elements
-        self.label: Optional[Multitext] = None
-
-        if xml_tree is not None:
-            self._update_from_xml(xml_tree)
-
-    def _update_from_xml(self, xml_tree):
-        self.xml_tree = xml_tree
-
-        # Update object attributes.
-        etree_to_obj_attributes(xml_tree, self)
-
 
 class Annotation(Multitext):
     """Provides a mechanism for adding meta-information to almost any element.
     """
 
     def __init__(
         self,
-        xml_tree: Optional[etree.ElementTree] = None
+        xml_tree: Optional[etree._Element] = None
     ):
         super().__init__()
-        if xml_tree is not None:
-            super()._update_from_xml(xml_tree)
         # properties
-        self.props = Props(lift_version=config.LIFT_VERSION)
-        self.props.attributes = [
+        attribs = [
             Prop('name', required=True, prop_type=Key),
             Prop('value', required=True, prop_type=Key),
             Prop('who', prop_type=Key),
             Prop('when', prop_type=DateTime),
         ]
+        for a in attribs:
+            self.props.add_to('attributes', a)
+        self.xml_tag = 'annotation'
         # attributes
         self.name: Key = None
         self.value: Key = None
         self.who: Optional[Key] = None
         self.when: Optional[DateTime] = None
 
         if xml_tree is not None:
             self._update_from_xml(xml_tree)
 
-    def _update_from_xml(self, xml_tree):
-        self.xml_tree = xml_tree
-
-        mul = Multitext(xml_tree)
-        mul._update_other_from_self(self)
-        del mul
-
-        # Update object attributes.
-        etree_to_obj_attributes(xml_tree, self)
-
 
 class Field(Multitext):
     """A generalised element to allow an application to store information.
     It's for information in a LIFT file that isn't explicitly described in the
     LIFT standard.
     """
 
     def __init__(
         self,
-        xml_tree: Optional[etree.ElementTree] = None
+        xml_tree: Optional[etree._Element] = None
     ):
         super().__init__()
-        if xml_tree is not None:
-            super()._update_from_xml(xml_tree)
         # properties
-        self.props = Props(lift_version=config.LIFT_VERSION)
-        self.props.attributes = [
+        attribs = [
             Prop('date_created', prop_type=DateTime),
             Prop('date_modified', prop_type=DateTime),
         ]
         if config.LIFT_VERSION == '0.13':
-            self.props.attributes.append(Prop(
-                'type',
-                required=True,
-                prop_type=Key
-            ))
+            attribs.append(Prop('type', required=True, prop_type=Key))
         else:
-            self.props.attributes.append(Prop(
-                'name',
-                required=True,
-                prop_type=Key
-            ))
-        self.props.elements = [
-            Prop('annotations', prop_type=list, item_type=Annotation),
+            attribs.append(Prop('name', required=True, prop_type=Key))
+        for a in attribs:
+            self.props.add_to('attributes', a)
+        elems = [
+            Prop('annotation_items', prop_type=list, item_type=Annotation),
+            Prop('trait_items', prop_type=list, item_type=Trait),
         ]
         if config.LIFT_VERSION == '0.13':
-            self.props.elements.append(Prop(
-                'traits',
-                prop_type=list,
-                item_type=Flag
-            ))
-            self.props.elements.append(Prop(
-                'forms',
-                prop_type=list,
-                item_type=Span
-            ))
-        else:
-            self.props.elements.append(Prop(
-                'traits',
-                prop_type=list,
-                item_type=Trait
-            ))
+            elems.append(Prop('form_items', prop_type=list, item_type=Span))
+        for e in elems:
+            self.props.add_to('elements', e)
+        self.xml_tag = 'field'
         # attributes
         if config.LIFT_VERSION == '0.13':
-            self.prop_type: Key = None
+            self.type: Key = None
         else:
             self.name: Key = None
         self.date_created: Optional[DateTime] = None
         self.date_modified: Optional[DateTime] = None
         # elements
         if config.LIFT_VERSION == '0.13':
-            self.traits: Optional[List[Flag]] = None
-            self.forms: Optional[List[Span]] = None
+            # self.trait_items: Optional[List[Flag]] = None
+            self.trait_items: Optional[List[Trait]] = None
+            self.form_items: Optional[List[Span]] = None
         else:
-            self.traits: Optional[List[Trait]] = None
-        self.annotations: Optional[List[Annotation]] = None
+            self.trait_items: Optional[List[Trait]] = None
+        self.annotation_items: Optional[List[Annotation]] = None
 
         if xml_tree is not None:
             self._update_from_xml(xml_tree)
 
-    def _update_from_xml(self, xml_tree):
-        self.xml_tree = xml_tree
-
-        mul = Multitext(xml_tree)
-        mul._update_other_from_self(self)
-        del mul
-
-        # Update object attributes.
-        etree_to_obj_attributes(xml_tree, self)
-
 
 class Extensible(LIFTUtilsBase):
     """Used to provide certain extra information in a controlled way.
 
     :ivar Optional[DateTime] date_created: Contains a date/timestamp saying
         when the element was added to the dictionary.
     :ivar Optional[DateTime] date_modified: Contains a date/timestamp saying
         when the element was last changed.
-    :ivar Optional[List[Field]] fields: Holds extra textual information.
-    :ivar Optional[List[Trait]] traits: Adds type or constraint information.
+    :ivar Optional[List[Field]] field_items: Holds extra textual information.
+    :ivar Optional[List[Trait]] trait_items: Adds type or constraint
+        information.
     :ivar Optional[List[Annotation]] annotation: Adds meta-information
         describing the element.
     """
 
     def __init__(
         self,
-        xml_tree: Optional[etree.ElementTree] = None
+        xml_tree: Optional[etree._Element] = None
     ):
         super().__init__()
-        if xml_tree is not None:
-            super()._update_from_xml(xml_tree)
         # properties
-        self.props = Props(lift_version=config.LIFT_VERSION)
-        self.props.attributes = [
+        attribs = [
             Prop('date_created', prop_type=DateTime),
             Prop('date_modified', prop_type=DateTime),
         ]
-        self.props.elements = [
-            Prop('fields', prop_type=list, item_type=Field),
-            Prop('traits', prop_type=list, item_type=Trait),
-            Prop('annotations', prop_type=list, item_type=Annotation),
-        ]
+        for a in attribs:
+            self.props.add_to('attributes', a)
+        elems = [
+            Prop('field_items', prop_type=list, item_type=Field),
+            Prop('trait_items', prop_type=list, item_type=Trait),
+            Prop('annotation_items', prop_type=list, item_type=Annotation),
+        ]
+        for e in elems:
+            self.props.add_to('elements', e)
+        # Extensible is only used as a super class for other classes, so it
+        # doesn't need its own XML tag.
+        self.xml_tag = None
         # attributes
         self.date_created: Optional[DateTime] = None
         self.date_modified: Optional[DateTime] = None
         # elements
-        self.fields: Optional[List[Field]] = None
+        self.field_items: Optional[List[Field]] = None
         if config.LIFT_VERSION == '0.13':
-            # TODO: Find definition of "Flag" in v0.13.
-            # self.traits: Optional[List[Flag]] = None
-            self.traits: Optional[List[Trait]] = None
+            # TODO: Find definition of "Flag" in v0.13?
+            # self.trait_items: Optional[List[Flag]] = None
+            self.trait_items: Optional[List[Trait]] = None
         else:
-            self.traits: Optional[List[Trait]] = None
-        self.annotations: Optional[List[Annotation]] = None
+            self.trait_items: Optional[List[Trait]] = None
+        self.annotation_items: Optional[List[Annotation]] = None
 
         if xml_tree is not None:
             self._update_from_xml(xml_tree)
 
-    def _update_from_xml(self, xml_tree):
-        self.xml_tree = xml_tree
-
-        # Update object attributes.
-        etree_to_obj_attributes(xml_tree, self)
-
-    def _update_other_from_self(self, other):
-        other.date_created = self.date_created
-        other.date_modified = self.date_modified
-        other.fields = self.fields
-        other.traits = self.traits
-        other.annotations = self.annotations
+    def _add_attribs_to_xml_tree(self, xml_tree):
+        for attrib in self.props.attributes:
+            a = attrib.name
+            x = config.XML_NAMES.get(a, a)
+            xml_tree.set(x, self.__dict__.get(a))
+        return xml_tree
```

### Comparing `lift_utils-0.1.1/src/lift_utils/config.py` & `lift_utils-0.2/src/lift_utils/config.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,46 +1,46 @@
 """Define runtime global variables."""
 
-LIB_VERSION = '0.1.1'
+LIB_VERSION = '0.2'
 LIFT_VERSION_FIELDWORKS = '0.13'  # used by FLEx 9.1
 LIFT_VERSION_LATEST = '0.15'
 LIFT_VERSION_DEFAULT = LIFT_VERSION_FIELDWORKS
 LIFT_VERSION = None
 
 XML_NAMES = {
     # object attribute keys (L) and corresponding LIFT XML tags (R)
-    'abbrevs': 'abbrev',
-    'annotations': 'annotation',
+    'abbrev_items': 'abbrev',
+    'annotation_items': 'annotation',
     'class_': 'class',
     'date_created': 'dateCreated',
     'date_deleted': 'dateDeleted',
     'date_modified': 'dateModified',
-    'descriptions': 'description',
-    'entries': 'entry',
-    'etymologies': 'etymology',
-    'examples': 'example',
-    'field_definitions': 'field',
-    'fields': 'field',
-    'forms': 'form',
-    'glosses': 'gloss',
+    'description_items': 'description',
+    'entry_items': 'entry',
+    'etymology_items': 'etymology',
+    'example_items': 'example',
+    'field_items': 'field',
+    'form_items': 'form',
+    'gloss_items': 'gloss',
     'grammatical_info': 'grammatical-info',
-    'illustrations': 'illustration',
-    'labels': 'label',
+    'illustration_items': 'illustration',
+    'label_items': 'label',
     'lexical_unit': 'lexical-unit',
-    'medias': 'media',
-    'notes': 'note',
+    'media_items': 'media',
+    'note_items': 'note',
     'option_range': 'option-range',
     'pcdata': 'text',
-    'pronunciations': 'pronunciation',
-    'range_elements': 'range-element',
-    'ranges': 'range',
-    'relations': 'relation',
-    'reversals': 'reversal',
-    'senses': 'sense',
-    'spans': 'span',
-    'subsenses': 'subsense',
-    'traits': 'trait',
-    'translations': 'translation',
-    'usages': 'usage',
-    'variants': 'variant',
+    'pronunciation_items': 'pronunciation',
+    'prop_type': 'type',
+    'range_element_items': 'range-element',
+    'range_items': 'range',
+    'relation_items': 'relation',
+    'reversal_items': 'reversal',
+    'sense_items': 'sense',
+    'span_items': 'span',
+    'subsense_items': 'subsense',
+    'trait_items': 'trait',
+    'translation_items': 'translation',
+    'usage_items': 'usage',
+    'variant_items': 'variant',
     'writing_system': 'writing-system',
 }
```

### Comparing `lift_utils-0.1.1/src/lift_utils/datatypes.py` & `lift_utils-0.2/src/lift_utils/datatypes.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,50 +1,53 @@
 """Define the basic datatypes."""
 
+import uuid
 from typing import List
 
 
 class PCData(str):
-    def __new__(cls, content=None):
-        if content is not None:
-            return super().__new__(cls, content)
+    def __new__(cls, text=None):
+        if text is not None:
+            return super().__new__(cls, text)
 
 
 class DateTime(str):
     # format (str): YYYY-MM-DDTHH:MM:SSZZZZZZ
     # ZZZZZZ: +/-, H, H, :, M, M (offset from GMT)
-    def __new__(cls, content=None):
-        if content is not None:
-            return super().__new__(cls, content)
+    def __new__(cls, text=None):
+        if text is not None:
+            return super().__new__(cls, text)
 
 
 class Key(str):
-    def __new__(cls, content=None):
-        if content is not None:
-            return super().__new__(cls, content)
+    def __new__(cls, text=None):
+        if text is not None:
+            return super().__new__(cls, text)
 
 
 class Lang(str):
     # format (str): ISO[-SCRIPT[-x-PRIVATE]]
-    def __new__(cls, content=None):
-        if content is not None:
-            return super().__new__(cls, content)
+    def __new__(cls, text=None):
+        if text is not None:
+            return super().__new__(cls, text)
 
 
 class RefId(str):
     # format (HEX GUID): xxxxxxxx-xxxx-xxxx-xxxx-xxxxxxxxxxxx
-    def __new__(cls, content=None):
-        if content is not None:
-            return super().__new__(cls, content)
+    def __new__(cls, text=None):
+        if text is not None:
+            return super().__new__(cls, text)
+        else:  # generate new UUID
+            return super().__new__(cls, str(uuid.uuid4()))
 
 
 class URL(str):
-    def __new__(cls, content=None):
-        if content is not None:
-            return super().__new__(cls, content)
+    def __new__(cls, text=None):
+        if text is not None:
+            return super().__new__(cls, text)
 
 
 class Prop:
     def __init__(
         self,
         name: str = None,
         required: bool = False,
@@ -63,7 +66,12 @@
         lift_version: str = None,
         attributes: List[Prop] = None,
         elements: List[Prop] = None,
     ):
         self.lift_version = lift_version
         self.attributes = attributes
         self.elements = elements
+
+    def add_to(self, prop_group_name, prop_obj):
+        prop_group = self.__dict__.get(prop_group_name)
+        if prop_obj.name not in (p.name for p in prop_group):
+            prop_group.append(prop_obj)
```

### Comparing `lift_utils-0.1.1/src/lift_utils/header.py` & `lift_utils-0.2/src/lift_utils/header.py`

 * *Files 22% similar despite different names*

```diff
@@ -6,86 +6,76 @@
 
 from . import config
 from .base import Extensible
 from .base import LIFTUtilsBase
 from .base import Multitext
 from .datatypes import Key
 from .datatypes import Prop
-from .datatypes import Props
 from .datatypes import URL
-from .utils import etree_to_obj_attributes
 
 
 class FieldDefn(Multitext):
     """Gives information about a particular field type.
     It may be used by an application to add information not part of the LIFT
     standard.
 
     .. note:: Used by LIFT v0.13 (FieldWorks) instead of ``FieldDefinition``.
     """
 
     def __init__(
         self,
-        xml_tree: Optional[etree.ElementTree] = None
+        tag: Key = None,
+        xml_tree: Optional[etree._Element] = None
     ):
         super().__init__()
-        if xml_tree is not None:
-            super()._update_from_xml(xml_tree)
         # properties
-        self.props = Props(lift_version=config.LIFT_VERSION)
-        self.props.attributes = [
-            Prop('tag', required=True, prop_type=Key),
-        ]
+        self.props.add_to(
+            'attributes',
+            Prop('tag', required=True, prop_type=Key)
+        )
+        self.xml_tag = 'field'
         # attributes
-        self.tag: Key = None
+        self.tag = tag
 
         if xml_tree is not None:
             self._update_from_xml(xml_tree)
 
     def __str__(self):
-        forms = 'forms' if len(self.forms) > 1 else 'form'
-        return f"{self.tag} ({len(self.forms)} {forms})"
-
-    def _update_from_xml(self, xml_tree):
-        # Set initial xml_tree.
-        self.xml_tree = xml_tree
-        # Update super class attributes.
-        m = Multitext(xml_tree)
-        m._update_other_from_self(self)
-        del m
-        # Update object attributes.
-        etree_to_obj_attributes(xml_tree, self)
+        forms = 'forms' if len(self.form_items) > 1 else 'form'
+        return f"{self.tag} ({len(self.form_items)} {forms})"
 
 
 class FieldDefinition(LIFTUtilsBase):
     """Gives information about a particular field type.
     It may be used by an application to add information not part of the LIFT
     standard.
     """
 
     def __init__(
         self,
-        xml_tree: Optional[etree.ElementTree] = None
+        xml_tree: Optional[etree._Element] = None
     ):
         super().__init__()
-        if xml_tree is not None:
-            super()._update_from_xml(xml_tree)
         # properties
-        self.props = Props(lift_version=config.LIFT_VERSION)
-        self.props.attributes = [
+        attribs = [
             Prop('name', required=True, prop_type=Key),
             Prop('class_', prop_type=str),
             Prop('type', prop_type=str),
             Prop('option_range', prop_type=Key),
             Prop('writing_system', prop_type=str),
         ]
-        self.props.elements = [
+        for a in attribs:
+            self.props.add_to('attributes', a)
+        elems = [
             Prop('label', prop_type=Multitext),
             Prop('description', prop_type=Multitext),
         ]
+        for e in elems:
+            self.props.add_to('elements', e)
+        self.xml_tag = 'field'
         # attributes
         self.name: Key = None
         self.class_: Optional[str] = None
         self.type: Optional[str] = None
         self.option_range: Optional[Key] = None
         self.writing_system: Optional[str] = None
         # elements
@@ -94,254 +84,209 @@
 
         if xml_tree is not None:
             self._update_from_xml(xml_tree)
 
     def __str__(self):
         return self.name
 
-    def _update_from_xml(self, xml_tree):
-        # Set initial xml_tree.
-        self.xml_tree = xml_tree
-        # Update object attributes.
-        etree_to_obj_attributes(xml_tree, self)
 
+class FieldDefns(LIFTUtilsBase):
+    """This is a simple list of ``field-defn`` elements.
 
-class RangeElement(Extensible):
-    """The description of a particular range element found in a ``range``.
+    .. note:: Used by LIFT v0.13 (FieldWorks) instead of ``Fields``.
     """
 
     def __init__(
         self,
-        xml_tree: Optional[etree.ElementTree] = None
+        xml_tree: Optional[etree._Element] = None
     ):
         super().__init__()
-        if xml_tree is not None:
-            super()._update_from_xml(xml_tree)
         # properties
-        self.props = Props(lift_version=config.LIFT_VERSION)
-        self.props.attributes = [
-            Prop('id', required=True, prop_type=Key),
-            Prop('parent', prop_type=Key),
-            Prop('guid', prop_type=str),
-        ]
-        self.props.elements = [
-            Prop('descriptions', prop_type=list, item_type=Multitext),
-            Prop('labels', prop_type=list, item_type=Multitext),
-            Prop('abbrevs', prop_type=list, item_type=Multitext),
-        ]
-        # attributes
-        self.id: Key = None
-        self.parent: Key = None
-        self.guid: str = None
+        self.props.add_to(
+            'elements',
+            Prop('field_items', prop_type=list, item_type=FieldDefn)
+        )
+        self.xml_tag = 'fields'
         # elements
-        self.descriptions: Optional[List[Multitext]] = None
-        self.labels: Optional[List[Multitext]] = None
-        self.abbrevs: Optional[List[Multitext]] = None
+        self.field_items: Optional[List[FieldDefn]] = None
 
         if xml_tree is not None:
             self._update_from_xml(xml_tree)
 
-    def _update_from_xml(self, xml_tree):
-        # Set initial xml_tree.
-        self.xml_tree = xml_tree
-        # Update super class attributes.
-        ext = Extensible(xml_tree)
-        ext._update_other_from_self(self)
-        del ext
-        # Update object attributes.
-        etree_to_obj_attributes(xml_tree, self)
-
 
-class Range(Extensible):
-    """A set of ``range-elements``.
-    It is used to identify both the group of ``range-elements`` but also to
-    some extent their type.
+class Fields(LIFTUtilsBase):
+    """This is a simple list of ``field-definition`` elements.
     """
 
     def __init__(
         self,
-        xml_tree: Optional[etree.ElementTree] = None
+        xml_tree: Optional[etree._Element] = None
     ):
         super().__init__()
-        if xml_tree is not None:
-            super()._update_from_xml(xml_tree)
         # properties
-        self.props = Props(lift_version=config.LIFT_VERSION)
-        self.props.attributes = [
-            Prop('id', required=True, prop_type=Key),
-            Prop('guid', prop_type=str),
-            Prop('href', prop_type=URL),
-        ]
-        self.props.elements = [
-            Prop(
-                'range_elements',
-                required=True,
-                prop_type=list,
-                item_type=RangeElement
-            ),
-            Prop('description', prop_type=Multitext),
-            Prop('labels', prop_type=list, item_type=Multitext),
-            Prop('abbrevs', prop_type=list, item_type=Multitext),
-        ]
-        # attributes
-        self.id: Key = None
-        self.guid: Optional[str] = None
-        self.href: Optional[URL] = None
+        self.props.add_to(
+            'elements',
+            Prop('field_items', prop_type=list, item_type=FieldDefinition)  # noqa: E501
+        )
         # elements
-        self.description: Optional[Multitext] = None
-        self.range_elements: List[RangeElement] = None
-        self.labels: List[Multitext] = None
-        self.abbrevs: List[Multitext] = None
+        self.field_items: Optional[List[FieldDefinition]] = None
 
         if xml_tree is not None:
             self._update_from_xml(xml_tree)
 
-    def _update_from_xml(self, xml_tree):
-        # Set initial xml_tree.
-        self.xml_tree = xml_tree
-        # Update super class attributes.
-        ext = Extensible(xml_tree)
-        ext._update_other_from_self(self)
-        del ext
-        # Update object attributes.
-        etree_to_obj_attributes(xml_tree, self)
 
+class RangeElement(Extensible, LIFTUtilsBase):
+    """The description of a particular range element found in a ``range``.
 
-class Ranges(LIFTUtilsBase):
-    """The root element in a Lift Ranges file.
+    .. note:: Does not inherit from Extensible in LIFT v0.13 (FieldWorks).
     """
 
     def __init__(
         self,
-        xml_tree: Optional[etree.ElementTree] = None
+        elem_id: Key = None,
+        xml_tree: Optional[etree._Element] = None
     ):
-        super().__init__()
-        if xml_tree is not None:
-            super()._update_from_xml(xml_tree)
+        if config.LIFT_VERSION == '0.13':
+            LIFTUtilsBase.__init__(self)
+        else:
+            Extensible.__init__(self)
         # properties
-        self.props = Props(lift_version=config.LIFT_VERSION)
-        self.props.elements = [
-            Prop('ranges', required=True, prop_type=list, item_type=Range),
+        attribs = [
+            Prop('id', required=True, prop_type=Key),
+            Prop('parent', prop_type=Key),
+            Prop('guid', prop_type=str),
         ]
+        for a in attribs:
+            self.props.add_to('attributes', a)
+        elems = [
+            Prop('description_items', prop_type=list, item_type=Multitext),
+            Prop('label_items', prop_type=list, item_type=Multitext),
+            Prop('abbrev_items', prop_type=list, item_type=Multitext),
+        ]
+        for e in elems:
+            self.props.add_to('elements', e)
+        self.xml_tag = 'range-element'
+        # attributes
+        self.id = elem_id
+        self.parent: Key = None
+        self.guid: str = None
         # elements
-        self.ranges: List[Range] = None
+        self.description_items: Optional[List[Multitext]] = None
+        self.label_items: Optional[List[Multitext]] = None
+        self.abbrev_items: Optional[List[Multitext]] = None
 
         if xml_tree is not None:
             self._update_from_xml(xml_tree)
 
-    def _update_from_xml(self, xml_tree):
-        # Set initial xml_tree.
-        self.xml_tree = xml_tree
 
-        # Update object attributes.
-        etree_to_obj_attributes(xml_tree, self)
-
-
-class FieldDefns(LIFTUtilsBase):
-    """This is a simple list of ``field-defn`` elements.
+class Range(Extensible, LIFTUtilsBase):
+    """A set of ``range-elements``.
+    It is used to identify both the group of ``range-elements`` but also to
+    some extent their type.
 
-    .. note:: Used by LIFT v0.13 (FieldWorks) instead of ``Fields``.
+    .. note:: Does not inherit from Extensible in LIFT v0.13 (FieldWorks).
     """
 
     def __init__(
         self,
-        xml_tree: Optional[etree.ElementTree] = None
+        range_id: Key = None,
+        xml_tree: Optional[etree._Element] = None
     ):
-        super().__init__()
-        if xml_tree is not None:
-            super()._update_from_xml(xml_tree)
+        if config.LIFT_VERSION == '0.13':
+            LIFTUtilsBase.__init__(self)
+        else:
+            Extensible.__init__(self)
         # properties
-        self.props = Props(lift_version=config.LIFT_VERSION)
-        self.props.elements = [
-            Prop('fields', prop_type=list, item_type=FieldDefn)
+        attribs = [
+            Prop('id', required=True, prop_type=Key),
+            Prop('guid', prop_type=str),
+            Prop('href', prop_type=URL),
+        ]
+        for a in attribs:
+            self.props.add_to('attributes', a)
+        elems = [
+            Prop(
+                'range_element_items',
+                required=True,
+                prop_type=list,
+                item_type=RangeElement
+            ),
+            Prop('description', prop_type=Multitext),
+            Prop('label_items', prop_type=list, item_type=Multitext),
+            Prop('abbrev_items', prop_type=list, item_type=Multitext),
         ]
+        for e in elems:
+            self.props.add_to('elements', e)
+        self.xml_tag = 'range'
+        # attributes
+        self.id = range_id
+        self.guid: Optional[str] = None
+        self.href: Optional[URL] = None
         # elements
-        self.fields: Optional[List[FieldDefn]] = None
+        self.description: Optional[Multitext] = None
+        self.range_element_items: List[RangeElement] = None
+        self.label_items: List[Multitext] = None
+        self.abbrev_items: List[Multitext] = None
 
         if xml_tree is not None:
             self._update_from_xml(xml_tree)
 
-    def _update_from_xml(self, xml_tree):
-        # Set initial xml_tree.
-        self.xml_tree = xml_tree
-        # Update object attributes.
-        etree_to_obj_attributes(xml_tree, self)
 
-
-class Fields(LIFTUtilsBase):
-    """This is a simple list of ``field-definition`` elements.
+class Ranges(LIFTUtilsBase):
+    """The root element in a Lift Ranges file.
     """
 
     def __init__(
         self,
-        xml_tree: Optional[etree.ElementTree] = None
+        xml_tree: Optional[etree._Element] = None
     ):
         super().__init__()
-        if xml_tree is not None:
-            super()._update_from_xml(xml_tree)
         # properties
-        self.props = Props(lift_version=config.LIFT_VERSION)
-        self.props.elements = [
-            Prop(
-                'field_definitions',
-                prop_type=list,
-                item_type=FieldDefinition
-            ),
-        ]
+        self.props.add_to(
+            'elements',
+            Prop('range_items', required=True, prop_type=list, item_type=Range),  # noqa: E501
+        )
+        self.xml_tag = 'ranges'
         # elements
-        self.field_definitions: Optional[List[FieldDefinition]] = None
+        self.range_items: List[Range] = None
 
         if xml_tree is not None:
             self._update_from_xml(xml_tree)
 
-    def _update_from_xml(self, xml_tree):
-        # Set initial xml_tree.
-        self.xml_tree = xml_tree
-
-        # # Update object attributes.
-        etree_to_obj_attributes(xml_tree, self)
-
 
 class Header(LIFTUtilsBase):
     """The header information for a LIFT file.
     It includes range information and added field definitions.
 
     :ivar Optional[Multitext] description: Contains a multilingual description
         of the lexicon for information purposes only.
-    :ivar Optional[Ranges[Range]] ranges: Contains all the ``range``
-        information.
-    :ivar Optional[FieldDefns] fields: `Used by LIFT v0.13 (FieldWorks).`
+    :ivar Optional[Ranges] ranges: Contains all the ``range`` information.
+    :ivar Optional[FieldDefns] field_items: `Used by LIFT v0.13 (FieldWorks).`
         Contains definitions for all the ``field`` types used in the document.
     :ivar Optional[Fields] fields: Contains definitions for all the ``field``
         types used in the document.
     """
 
     def __init__(
         self,
-        xml_tree: Optional[etree.ElementTree] = None
+        xml_tree: Optional[etree._Element] = None
     ):
         super().__init__()
-        if xml_tree is not None:
-            super()._update_from_xml(xml_tree)
         # properties
-        self.props = Props(lift_version=config.LIFT_VERSION)
-        self.props.elements = [
+        elems = [
             Prop('description', prop_type=Multitext),
             Prop('ranges', prop_type=Ranges),
         ]
         if config.LIFT_VERSION == '0.13':
-            self.props.elements.append(Prop(
-                'fields',
-                prop_type=FieldDefns
-            ))
+            elems.append(Prop('fields', prop_type=FieldDefns))
         else:
-            self.props.elements.append(Prop(
-                'fields',
-                prop_type=Fields
-            ))
+            elems.append(Prop('fields', prop_type=Fields))
+        for e in elems:
+            self.props.add_to('elements', e)
+        self.xml_tag = 'header'
         # elements
         self.description: Optional[Multitext] = None
         self.ranges: Optional[Ranges] = None
         if config.LIFT_VERSION == '0.13':
             self.fields: Optional[FieldDefns] = None
         else:
             self.fields: Optional[Fields] = None
@@ -354,13 +299,7 @@
         if self.description:
             s = str(self.description)
         if self.ranges:
             s += f": {len(self.ranges)} ranges"
         if self.fields:
             s += f", {len(self.fields)} fields"
         return s
-
-    def _update_from_xml(self, xml_tree):
-        # Set initial xml_tree.
-        self.xml_tree = xml_tree
-        # Update object attributes.
-        etree_to_obj_attributes(xml_tree, self)
```

### Comparing `lift_utils-0.1.1/src/lift_utils/lexicon.py` & `lift_utils-0.2/src/lift_utils/lexicon.py`

 * *Files 20% similar despite different names*

```diff
@@ -18,217 +18,176 @@
 from .base import Span
 from .base import Trait
 from .base import URLRef
 from .datatypes import DateTime
 from .datatypes import Key
 from .datatypes import RefId
 from .datatypes import Prop
-from .datatypes import Props
 from .datatypes import URL
 from .header import Header
 from .header import Range
-from .utils import xml_to_etree
+from .utils import xmlfile_to_etree
 from .utils import etree_to_obj_attributes
+from .utils import search_entry
 
 
 class Note(Multitext, Extensible):
     """For storing descriptive information of many kinds.
     It can include comments, bibliographic information and domain specific
     notes.
 
     :ivar Optional[Key] type: Gives the type of note by reference to a
         ``range-element`` in the ``note-type`` range.
     """
 
     def __init__(
         self,
-        xml_tree: Optional[etree.ElementTree] = None
+        xml_tree: Optional[etree._Element] = None
     ):
-        super().__init__()
-        if xml_tree is not None:
-            super()._update_from_xml(xml_tree)
+        Extensible.__init__(self)
+        Multitext.__init__(self)
         # properties
-        self.props = Props(lift_version=config.LIFT_VERSION)
-        self.props.attributes = [
-            Prop('type', prop_type=Key),
-        ]
+        self.props.add_to('attributes', Prop('type', prop_type=Key))
+        self.xml_tag = 'note'
         # attributes
         self.type: Optional[Key] = None
 
         if xml_tree is not None:
             self._update_from_xml(xml_tree)
 
     def __str__(self):
         return super().__str__()
 
-    def _update_from_xml(self, xml_tree):
-        # Set initial xml_tree.
-        self.xml_tree = xml_tree
-        # Update super class attributes.
-        ext = Extensible(xml_tree)
-        ext._update_other_from_self(self)
-        del ext
-        mul = Multitext(xml_tree)
-        mul._update_other_from_self(self)
-        del mul
-        # Update object attributes.
-        etree_to_obj_attributes(xml_tree, self)
-
 
 class Phonetic(Multitext, Extensible):
     """This represents a single pronunciation in phonetic form.
 
-    :ivar Optional[List[URLRef]] medias: Stores an audio representation of the
-        text.
-    :ivar Optional[List[Span]] forms: `Used by LIFT v0.13 (FieldWorks).` Stores
-        the phonetic representation using whichever writing system: IPA,
+    :ivar Optional[List[URLRef]] media_items: Stores an audio representation of
+        the text.
+    :ivar Optional[List[Span]] form_items: `Used by LIFT v0.13 (FieldWorks).`
+        Stores the phonetic representation using whichever writing system: IPA,
         Americanist, etc.
     """
 
     def __init__(
         self,
-        xml_tree: Optional[etree.ElementTree] = None
+        xml_tree: Optional[etree._Element] = None
     ):
-        super().__init__()
-        if xml_tree is not None:
-            super()._update_from_xml(xml_tree)
+        Extensible.__init__(self)
+        Multitext.__init__(self)
         # properties
-        self.props = Props(lift_version=config.LIFT_VERSION)
-        self.props.elements = [
-            Prop('medias', prop_type=list, item_type=URLRef),
-        ]
+        self.props.add_to(
+            'elements',
+            Prop('media_items', prop_type=list, item_type=URLRef)
+        )
         if config.LIFT_VERSION == '0.13':
-            self.props.elements.append(Prop(
-                'forms',
-                prop_type=list,
-                item_type=Span
-            ))
+            self.props.add_to(
+                'elements',
+                Prop('form_items', prop_type=list, item_type=Span)
+            )
+        self.xml_tag = 'pronunciation'
         # elements
-        self.medias: Optional[List[URLRef]] = None
+        self.media_items: Optional[List[URLRef]] = None
         if config.LIFT_VERSION == '0.13':
-            self.forms: Optional[List[Span]] = None
+            self.form_items: Optional[List[Span]] = None
 
         if xml_tree is not None:
             self._update_from_xml(xml_tree)
 
     def __str__(self):
         return super().__str__()
 
-    def _update_from_xml(self, xml_tree):
-        # Set initial xml_tree.
-        self.xml_tree = xml_tree
-        # Update super class attributes.
-        ext = Extensible(xml_tree)
-        ext._update_other_from_self(self)
-        del ext
-        mul = Multitext(xml_tree)
-        mul._update_other_from_self(self)
-        del mul
-        # Update object attributes.
-        etree_to_obj_attributes(xml_tree, self)
-
 
 class Etymology(Extensible):
     """For describing lexical relations with a word not in the lexicon.
 
     :ivar Key type: Gives the etymological relationship between this sense and
         some other word in another language.
     :ivar str source: Gives the language for the source language of the
         etymological relation.
-    :ivar Optional[List[Gloss]] glosses: Gives glosses of the word that the
+    :ivar Optional[List[Gloss]] gloss_items: Gives glosses of the word that the
         etymological relationship is with.
     :ivar Optional[Form] form: Holds the form of the etymological reference.
     """
 
     def __init__(
         self,
-        xml_tree: Optional[etree.ElementTree] = None
+        etym_type: Key = None,
+        source: str = None,
+        xml_tree: Optional[etree._Element] = None
     ):
         super().__init__()
-        if xml_tree is not None:
-            super()._update_from_xml(xml_tree)
         # properties
-        self.props = Props(lift_version=config.LIFT_VERSION)
-        self.props.attributes = [
+        attribs = [
             Prop('type', required=True, prop_type=Key),
             Prop('source', required=True, prop_type=str),
         ]
-        self.props.elements = [
-            Prop('glosses', prop_type=list, item_type=Gloss),
+        for a in attribs:
+            self.props.add_to('attributes', a)
+        elems = [
+            Prop('gloss_items', prop_type=list, item_type=Gloss),
             Prop('form', prop_type=Form),
         ]
+        for e in elems:
+            self.props.add_to('elements', e)
+        self.xml_tag = 'etymology'
         # attributes
-        self.type: Key = None
-        self.source: str = None
+        self.type = etym_type
+        self.source = source
         # elements
-        self.glosses: Optional[List[Gloss]] = None
+        self.gloss_items: Optional[List[Gloss]] = None
         self.form: Optional[Form] = None
 
         if xml_tree is not None:
             self._update_from_xml(xml_tree)
 
     def __str__(self):
         return f"{self.type} ({self.source})"
 
-    def _update_from_xml(self, xml_tree):
-        # Set initial xml_tree.
-        self.xml_tree = xml_tree
-        # Update super class attributes.
-        ext = Extensible(xml_tree)
-        ext._update_other_from_self(self)
-        del ext
-        # Update object attributes.
-        etree_to_obj_attributes(xml_tree, self)
-
 
 class GrammaticalInfo(LIFTUtilsBase):
     """A reference to a ``range-element`` in the ``grammatical-info`` range.
 
     :ivar Key value: The part of speech tag into the ``grammatical-info``
         range.
-    :ivar Optional[List[Trait]] traits: Allows the grammatical information for
-        a given sense to have more information than just the part of speech
+    :ivar Optional[List[Trait]] trait_items: Allows the grammatical information
+        for a given sense to have more information than just the part of speech
         given by the ``value`` attribute.
     """
 
     def __init__(
         self,
-        xml_tree: Optional[etree.ElementTree] = None
+        value: Key = None,
+        xml_tree: Optional[etree._Element] = None
     ):
         super().__init__()
-        if xml_tree is not None:
-            super()._update_from_xml(xml_tree)
         # properties
-        self.props = Props(lift_version=config.LIFT_VERSION)
-        self.props.attributes = [
-            Prop('value', required=True, prop_type=Key),
-        ]
-        self.props.elements = [
-            Prop('traits', prop_type=list, item_type=Trait),
-        ]
+        self.props.add_to(
+            'attributes',
+            Prop('value', required=True, prop_type=Key)
+        )
+        self.props.add_to(
+            'elements',
+            Prop('trait_items', prop_type=list, item_type=Trait)
+        )
+        self.xml_tag = 'grammatical-info'
         # attributes
-        self.value: Key = None
+        self.value = value
         # elements
-        self.traits: Optional[List[Trait]] = None
+        self.trait_items: Optional[List[Trait]] = None
 
         if xml_tree is not None:
             self._update_from_xml(xml_tree)
 
     def __str__(self):
         traits = ''
-        if self.traits:
-            traits = f": {'; '.join([t for t in self.traits])}"
+        if self.trait_items:
+            traits = f": {'; '.join([str(t) for t in self.trait_items])}"
         return f"{self.value}{traits}"
 
-    def _update_from_xml(self, xml_tree):
-        # Set initial xml_tree.
-        self.xml_tree = xml_tree
-        # Update object attributes.
-        etree_to_obj_attributes(xml_tree, self)
-
 
 class Reversal(Multitext):
     """Enables a wider use of a dictionary.
 
     :ivar Optional[Key] type: Gives the type of the reversal as a
         ``range-element`` in the ``reversal-type`` range.
     :ivar Optional[Reversal] main: This gives the parent reversal in a
@@ -236,139 +195,106 @@
     :ivar Optional[GrammaticalInfo] grammatical_info: This allows a reversal
         relation to specify what the grammatical information is in the reversal
         language.
     """
 
     def __init__(
         self,
-        xml_tree: Optional[etree.ElementTree] = None
+        xml_tree: Optional[etree._Element] = None
     ):
         super().__init__()
-        if xml_tree is not None:
-            super()._update_from_xml(xml_tree)
         # properties
-        self.props = Props(lift_version=config.LIFT_VERSION)
-        self.props.attributes = [
-            Prop('type', prop_type=Key),
-        ]
-        self.props.elements = [
+        self.props.add_to(
+            'attributes',
+            Prop('type', prop_type=Key)
+        )
+        elems = [
             Prop('main', prop_type=Reversal),
             Prop('grammatical_info', prop_type=GrammaticalInfo),
         ]
+        for e in elems:
+            self.props.add_to('elements', e)
+        self.xml_tag = 'reversal'
         # attributes
         self.type: Optional[Key] = None
         # elements
         self.main: Optional[Reversal] = None
         self.grammatical_info: Optional[GrammaticalInfo] = None
 
         if xml_tree is not None:
             self._update_from_xml(xml_tree)
 
-    def _update_from_xml(self, xml_tree):
-        # Set initial xml_tree.
-        self.xml_tree = xml_tree
-        # Update super class attributes.
-        mul = Multitext(xml_tree)
-        mul._update_other_from_self(self)
-        del mul
-        # Update object attributes.
-        etree_to_obj_attributes(xml_tree, self)
-
 
 class Translation(Multitext):
     """A ``Multitext`` with an optional translation ``type`` attribute.
 
     :ivar Optional[Key] type: Gives the type of the translation.
     """
 
     def __init__(
         self,
-        xml_tree: Optional[etree.ElementTree] = None
+        xml_tree: Optional[etree._Element] = None
     ):
         super().__init__()
-        if xml_tree is not None:
-            super()._update_from_xml(xml_tree)
         # properties
-        self.props = Props(lift_version=config.LIFT_VERSION)
-        self.props.attributes = [
-            Prop('type', prop_type=Key),
-        ]
+        self.props.add_to(
+            'attributes',
+            Prop('type', prop_type=Key)
+        )
+        self.xml_tag = 'translation'
         # attributes
         self.type: Optional[Key] = None
 
         if xml_tree is not None:
             self._update_from_xml(xml_tree)
 
-    def _update_from_xml(self, xml_tree):
-        # Set initial xml_tree.
-        self.xml_tree = xml_tree
-        # Update super class attributes.
-        mul = Multitext(xml_tree)
-        mul._update_other_from_self(self)
-        del mul
-        # Update object attributes.
-        etree_to_obj_attributes(xml_tree, self)
-
 
 class Example(Multitext, Extensible):
     """Gives an example sentence or phrase.
     It is given in the language and glosses of that example in other languages.
 
     :ivar Optional[Key] source: Reference by which another application may
         refer to this example or is a reference into another database of texts,
         for example.
-    :ivar Optional[List[Translation]] translations: Gives translations of the
-        example into different languages.
-    :ivar Optional[List[Note]] notes: Holds notes on this example.
+    :ivar Optional[List[Translation]] translation_items: Gives translations of
+        the example into different languages.
+    :ivar Optional[List[Note]] note_items: Holds notes on this example.
     """
 
     def __init__(
         self,
-        xml_tree: Optional[etree.ElementTree] = None
+        xml_tree: Optional[etree._Element] = None
     ):
-        super().__init__()
-        if xml_tree is not None:
-            super()._update_from_xml(xml_tree)
+        Extensible.__init__(self)
+        Multitext.__init__(self)
         # properties
-        self.props = Props(lift_version=config.LIFT_VERSION)
-        self.props.attributes = [
-            Prop('source', prop_type=Key),
-        ]
-        self.props.elements = [
-            Prop('translations', prop_type=list, item_type=Translation),
-        ]
+        self.props.add_to(
+            'attributes',
+            Prop('source', prop_type=Key)
+        )
+        self.props.add_to(
+            'elements',
+            Prop('translation_items', prop_type=list, item_type=Translation)
+        )
         if config.LIFT_VERSION in ['0.15']:
-            self.props.elements.append(Prop(
-                'notes',
-                prop_type=list,
-                item_type=Note
-            ))
+            self.props.add_to(
+                'elements',
+                Prop('note_items', prop_type=list, item_type=Note)
+            )
+        self.xml_tag = 'example'
         # attributes
         self.source: Optional[Key] = None
         # elements
-        self.translations: Optional[List[Translation]] = None
+        self.translation_items: Optional[List[Translation]] = None
         if config.LIFT_VERSION in ['0.15']:
-            self.notes: Optional[List[Note]] = None
+            self.note_items: Optional[List[Note]] = None
 
         if xml_tree is not None:
             self._update_from_xml(xml_tree)
 
-    def _update_from_xml(self, xml_tree):
-        # Set initial xml_tree.
-        self.xml_tree = xml_tree
-        # Update super class attributes.
-        ext = Extensible(xml_tree)
-        ext._update_other_from_self(self)
-        del ext
-        mul = Multitext(xml_tree)
-        mul._update_other_from_self(self)
-        del mul
-        # Update object attributes.
-        etree_to_obj_attributes(xml_tree, self)
-
 
 class Relation(Extensible):
     """This element is used for lexical relations.
 
     :ivar Key type: Is the type of the particular lexical relation.
     :ivar RefId ref: This is the other end of the relation, either a ``sense``
         or an ``entry``.
@@ -376,239 +302,206 @@
         given type when a multiple relation is being described.
     :ivar Optional[Multitext] usage: Gives information on usage in one or more
         languages or writing systems.
     """
 
     def __init__(
         self,
-        xml_tree: Optional[etree.ElementTree] = None
+        rel_type: Key = None,
+        ref: RefId = None,
+        xml_tree: Optional[etree._Element] = None
     ):
         super().__init__()
-        if xml_tree is not None:
-            super()._update_from_xml(xml_tree)
         # properties
-        self.props = Props(lift_version=config.LIFT_VERSION)
-        self.props.attributes = [
+        attribs = [
             Prop('type', required=True, prop_type=Key),
             Prop('ref', required=True, prop_type=RefId),
             Prop('order', prop_type=int),
         ]
-        self.props.elements = [
-            Prop('usages', prop_type=list, item_type=Multitext)
-        ]
+        for a in attribs:
+            self.props.add_to('attributes', a)
+        self.props.add_to(
+            'elements',
+            Prop('usage_items', prop_type=list, item_type=Multitext)
+        )
+        self.xml_tag = 'relation'
         # attributes
-        self.type: Key = None
-        self.ref: RefId = None
+        self.type = rel_type
+        self.ref = ref
         self.order: Optional[int] = None
         # elements
-        self.usages: Optional[List[Multitext]] = None
+        self.usage_items: Optional[List[Multitext]] = None
 
         if xml_tree is not None:
             self._update_from_xml(xml_tree)
 
     def __str__(self):
         return f"{self.type}: {self.ref}"
 
-    def _update_from_xml(self, xml_tree):
-        # Set initial xml_tree.
-        self.xml_tree = xml_tree
-        # Update super class attributes.
-        ext = Extensible(xml_tree)
-        ext._update_other_from_self(self)
-        del ext
-        # Update object attributes.
-        etree_to_obj_attributes(xml_tree, self)
-
 
 class Variant(Multitext, Extensible):
     """``variant`` elements are used for all sorts of variation.
 
     :ivar Optional[RefId] ref: Gives the variation as a reference to another
         ``entry`` or ``sense`` rather than specifying the ``form`` (that is,
         the ``Multitext`` value of the variant).
-    :ivar Optional[List[Phonetic]] pronunciations: Holds the phonetic variant
-        whether it is that this is a variation in phonetics only or that the
-        phonetic variation arises because of an orthographic or phonemic
-        variation.
-    :ivar Optional[List[Relation]]relations: Some variants have a lexical
+    :ivar Optional[List[Phonetic]] pronunciation_items: Holds the phonetic
+        variant whether it is that this is a variation in phonetics only or
+        that the phonetic variation arises because of an orthographic or
+        phonemic variation.
+    :ivar Optional[List[Relation]] relation_items: Some variants have a lexical
         relationship with other senses or entries in the lexicon.
     """
 
     def __init__(
         self,
-        xml_tree: Optional[etree.ElementTree] = None
+        xml_tree: Optional[etree._Element] = None
     ):
-        super().__init__()
-        if xml_tree is not None:
-            super()._update_from_xml(xml_tree)
+        Extensible.__init__(self)
+        Multitext.__init__(self)
         # properties
-        self.props = Props(lift_version=config.LIFT_VERSION)
-        self.props.attributes = [
-            Prop('ref', prop_type=RefId),
-        ]
-        self.props.elements = [
-            Prop('pronunciations', prop_type=list, item_type=Phonetic),
-            Prop('relations', prop_type=list, item_type=Relation),
-        ]
+        self.props.add_to(
+            'attributes',
+            Prop('ref', prop_type=RefId)
+        )
+        elems = [
+            Prop('pronunciation_items', prop_type=list, item_type=Phonetic),
+            Prop('relation_items', prop_type=list, item_type=Relation),
+        ]
+        for e in elems:
+            self.props.add_to('elements', e)
+        self.xml_tag = 'variant'
         # attributes
         self.ref: Optional[RefId] = None
         # elements
-        self.pronunciations: Optional[List[Phonetic]] = None
-        self.relations: Optional[List[Relation]] = None
+        self.pronunciation_items: Optional[List[Phonetic]] = None
+        self.relation_items: Optional[List[Relation]] = None
 
         if xml_tree is not None:
             self._update_from_xml(xml_tree)
 
     def __str__(self):
         return self.ref if self.ref else 'variant'
 
-    def _update_from_xml(self, xml_tree):
-        # Set initial xml_tree.
-        self.xml_tree = xml_tree
-        # Update super class attributes.
-        ext = Extensible(xml_tree)
-        ext._update_other_from_self(self)
-        del ext
-        mul = Multitext(xml_tree)
-        mul._update_other_from_self(self)
-        del mul
-        # Update object attributes.
-        etree_to_obj_attributes(xml_tree, self)
-
 
 class Sense(Extensible):
     """An ``entry`` is made up of a number of ``sense`` elements.
 
     :ivar Optional[RefId] id: This gives an identifier for this ``Sense`` so
         that things can refer to it.
     :ivar Optional[int] order: A number that is used to give the relative
         order of senses within an entry.
     :ivar Optional[GrammaticalInfo] grammatical_info: Grammatical information.
-    :ivar Optional[List[Form]] glosses: `Used by LIFT v0.13 (FieldWorks).` Each
-        ``gloss`` is a single string in a single language and writing system.
-    :ivar Optional[List[Gloss]] glosses: Each ``gloss`` is a single string in a
-        single language and writing system.
+    :ivar Optional[List[Union[Gloss, Form]]] gloss_items: Each ``gloss`` is a
+        single string in a single language and writing system. ``Form`` is used
+        by LIFT v0.13 (FieldWorks), while ``Gloss`` is used in later versions.
     :ivar Optional[Multitext] definition: Gives the definition in multiple
         languages or writing systems.
-    :ivar Optional[List[Relation]] relations: While a lexical relation isn't
-        strictly owned by a sense it is a good place to hold it.
-    :ivar Optional[List[Note]] notes: There are lots of different types of
+    :ivar Optional[List[Relation]] relation_items: While a lexical relation
+        isn't strictly owned by a sense it is a good place to hold it.
+    :ivar Optional[List[Note]] note_items: There are lots of different types of
         notes.
-    :ivar Optional[List[Example]] examples: Examples may be used for different
-        target audiences.
-    :ivar Optional[List[Reversal]] reversals: There may be different reversal
-        indexes.
-    :ivar Optional[List[URLRef]] illustrations: The picture doesn't have to be
-        static.
-    :ivar Optional[List] subsenses: Senses can form a hierarchy.
+    :ivar Optional[List[Example]] example_items: Examples may be used for
+        different target audiences.
+    :ivar Optional[List[Reversal]] reversal_items: There may be different
+        reversal indexes.
+    :ivar Optional[List[URLRef]] illustration_items: The picture doesn't have
+        to be static.
+    :ivar Optional[List[Sense]] subsense_items: Senses can form a hierarchy.
     """
 
     def __init__(
         self,
-        xml_tree: Optional[etree.ElementTree] = None
+        xml_tree: Optional[etree._Element] = None
     ):
         super().__init__()
-        if xml_tree is not None:
-            super()._update_from_xml(xml_tree)
         # properties
-        self.props = Props(lift_version=config.LIFT_VERSION)
-        self.props.attributes = [
+        attribs = [
             Prop('id', prop_type=RefId),
             Prop('order', prop_type=int),
         ]
-        self.props.elements = [
+        for a in attribs:
+            self.props.add_to('attributes', a)
+        elems = [
             Prop('grammatical_info', prop_type=GrammaticalInfo),
             Prop('definition', prop_type=Multitext),
-            Prop('relations', prop_type=list, item_type=Relation),
-            Prop('notes', prop_type=list, item_type=Note),
-            Prop('examples', prop_type=list, item_type=Example),
-            Prop('reversals', prop_type=list, item_type=Reversal),
-            Prop('illustrations', prop_type=list, item_type=URLRef),
-            Prop('subsenses', prop_type=list, item_type=Sense),
+            Prop('relation_items', prop_type=list, item_type=Relation),
+            Prop('note_items', prop_type=list, item_type=Note),
+            Prop('example_items', prop_type=list, item_type=Example),
+            Prop('reversal_items', prop_type=list, item_type=Reversal),
+            Prop('illustration_items', prop_type=list, item_type=URLRef),
+            Prop('subsense_items', prop_type=list, item_type=Sense),
         ]
         if config.LIFT_VERSION == '0.13':
-            self.props.elements.append(Prop(
-                'glosses',
-                prop_type=list,
-                item_type=Form
-            ))
+            elems.append(Prop('gloss_items', prop_type=list, item_type=Form))
         else:
-            self.props.elements.append(Prop(
-                'glosses',
-                prop_type=list,
-                item_type=Gloss
-            ))
-
+            elems.append(Prop('gloss_items', prop_type=list, item_type=Gloss))
+        for e in elems:
+            self.props.add_to('elements', e)
+        self.xml_tag = 'sense'
         # attributes
         self.id: Optional[RefId] = None
         self.order: Optional[int] = None
         # elements
         self.grammatical_info: Optional[GrammaticalInfo] = None
         if config.LIFT_VERSION == '0.13':
-            self.glosses: Optional[List[Form]] = None
+            self.gloss_items: Optional[List[Form]] = None
         else:
-            self.glosses: Optional[List[Gloss]] = None
+            self.gloss_items: Optional[List[Gloss]] = None
         self.definition: Optional[Multitext] = None
-        self.relations: Optional[List[Relation]] = None
-        self.notes: Optional[List[Note]] = None
-        self.examples: Optional[List[Example]] = None
-        self.reversals: Optional[List[Reversal]] = None
-        self.illustrations: Optional[List[URLRef]] = None
-        self.subsenses: Optional[List] = None  # Type should be 'Sense'
+        self.relation_items: Optional[List[Relation]] = None
+        self.note_items: Optional[List[Note]] = None
+        self.example_items: Optional[List[Example]] = None
+        self.reversal_items: Optional[List[Reversal]] = None
+        self.illustration_items: Optional[List[URLRef]] = None
+        self.subsense_items: Optional[List] = None
 
         if xml_tree is not None:
             self._update_from_xml(xml_tree)
 
     def __str__(self):
-        return self.get_summary_line()
+        return self._summary_line()
 
-    def get_summary_line(self, lang='en'):
+    def _summary_line(self, lang='en'):
         """Return a one-line summary of the entry's data for a given language.
         Defaults to English.
         """
-        gl = utils.ellipsize(str(self.get_gloss(lang=lang)), 10)
+        gl = utils.ellipsize(str(self.get_gloss(lang=lang)), 20)
         gi = utils.ellipsize(self.get_grammatical_info(), 10)
-        de = str(self.definition)
-        return f"{gl:10}\t{gi:10}\t{de}"
+        return f"{gl:20}\t{gi:10}\t{self.id}"
+
+    def get_id(self) -> RefId:
+        """Return the object's unique identifier"""
+        return self.id
 
-    def get_gloss(self, lang='en'):
+    def get_gloss(self, lang='en') -> str:
         """Get gloss details for a given language.
         Defaults to English.
         """
         gloss = ''
-        if self.glosses:
+        if self.gloss_items:
             # Choose 1st gloss if preferred language not found.
-            gloss = str(self.glosses[0])
-            for g in self.glosses:
+            gloss = str(self.gloss_items[0])
+            for g in self.gloss_items:
                 if g.lang == lang:
                     # Choose preferred language gloss.
                     gloss = str(g)
         return gloss
 
-    def get_grammatical_info(self):
+    def get_grammatical_info(self) -> GrammaticalInfo:
         """Get basic grammatical info.
         """
         grammatical_info = ''
         if self.grammatical_info:
             grammatical_info = str(self.grammatical_info)
         return grammatical_info
 
     def show(self):
         """Print an overview of the ``sense`` in the terminal window."""
-        print(self.__str__())
-
-    def _update_from_xml(self, xml_tree):
-        # Set initial xml_tree.
-        self.xml_tree = xml_tree
-        # Update super class attributes.
-        ext = Extensible(xml_tree)
-        ext._update_other_from_self(self)
-        del ext
-        # Update object attributes.
-        etree_to_obj_attributes(xml_tree, self)
+        print(self)
 
 
 class Entry(Extensible):
     """This is the core of a lexicon. A lexicon is made up of a set of entries.
 
     :ivar Optional[RefId] id: This gives a unique identifier to this ``entry``.
     :ivar Optional[str] guid: `Deprecated.` This gives a unique identifier to
@@ -617,234 +510,335 @@
     :ivar Optional[DateTime] date_deleted: If this attribute exists then it
         indicates that the particular ``entry`` has been deleted.
     :ivar Optional[Multitext] lexical_unit: The lexical form is the primary
         lexical form as is found as the primary lexical form in the source data
         models for this standard.
     :ivar Optional[Multitext] citation: This is the form that is to be printed
         in the dictionary.
-    :ivar Optional[List[Phonetic]] pronunciations: There can be multiple
+    :ivar Optional[List[Phonetic]] pronunciation_items: There can be multiple
         phonetic forms of an entry.
-    :ivar Optional[List[Variant]] variants: Any constrained variants or free
-        orthographic variants.
-    :ivar Optional[List[Sense]] senses: This is where the definition goes.
-    :ivar Optional[List[Note]] notes: The more notes you keep the better.
-    :ivar Optional[List[Relation]] relations: Gives a lexical relationship
+    :ivar Optional[List[Variant]] variant_items: Any constrained variants or
+        free orthographic variants.
+    :ivar Optional[List[Sense]] sense_items: This is where the definition goes.
+    :ivar Optional[List[Note]] note_items: The more notes you keep the better.
+    :ivar Optional[List[Relation]] relation_items: Gives a lexical relationship
         between this entry and another ``entry`` or ``sense``.
-    :ivar Optional[List[Etymology]] etymologies: Differs from a lexical
+    :ivar Optional[List[Etymology]] etymology_items: Differs from a lexical
         relation in that it has no referent in the lexicon.
     """
 
     def __init__(
         self,
-        xml_tree: Optional[etree.ElementTree] = None
+        xml_tree: Optional[etree._Element] = None
     ):
         super().__init__()
-        if xml_tree is not None:
-            super()._update_from_xml(xml_tree)
         # properties
-        self.props = Props(lift_version=config.LIFT_VERSION)
-        self.props.attributes = [
+        attribs = [
             Prop('id', prop_type=RefId),
             Prop('guid', prop_type=str),
             Prop('order', prop_type=str),
             Prop('date_deleted', prop_type=DateTime),
         ]
-        self.props.elements = [
+        for a in attribs:
+            self.props.add_to('attributes', a)
+        elems = [
             Prop('lexical_unit', prop_type=Multitext),
             Prop('citation', prop_type=Multitext),
-            Prop('pronunciations', prop_type=list, item_type=Phonetic),
-            Prop('variants', prop_type=list, item_type=Variant),
-            Prop('senses', prop_type=list, item_type=Sense),
-            Prop('notes', prop_type=list, item_type=Note),
-            Prop('relations', prop_type=list, item_type=Relation),
-            Prop('etymologies', prop_type=list, item_type=Etymology),
-        ]
+            Prop('pronunciation_items', prop_type=list, item_type=Phonetic),
+            Prop('variant_items', prop_type=list, item_type=Variant),
+            Prop('sense_items', prop_type=list, item_type=Sense),
+            Prop('note_items', prop_type=list, item_type=Note),
+            Prop('relation_items', prop_type=list, item_type=Relation),
+            Prop('etymology_items', prop_type=list, item_type=Etymology),
+        ]
+        for e in elems:
+            self.props.add_to('elements', e)
+        self.xml_tag = 'entry'
         # attributes
         self.id: Optional[RefId] = None
         self.guid: Optional[str] = None  # deprecated
         self.order: Optional[int] = None
         self.date_deleted: Optional[DateTime] = None
         # elements
         self.lexical_unit: Optional[Multitext] = None
         self.citation: Optional[Multitext] = None
-        self.pronunciations: Optional[List[Phonetic]] = None
-        self.variants: Optional[List[Variant]] = None
-        self.senses: Optional[List[Sense]] = None
-        self.notes: Optional[List[Note]] = None
-        self.relations: Optional[List[Relation]] = None
-        self.etymologies: Optional[List[Etymology]] = None
+        self.pronunciation_items: Optional[List[Phonetic]] = None
+        self.variant_items: Optional[List[Variant]] = None
+        self.sense_items: Optional[List[Sense]] = None
+        self.note_items: Optional[List[Note]] = None
+        self.relation_items: Optional[List[Relation]] = None
+        self.etymology_items: Optional[List[Etymology]] = None
 
         if xml_tree is not None:
             self._update_from_xml(xml_tree)
 
     def __str__(self):
-        return self.get_summary_line()
+        return self._summary_line()
 
-    def get_summary_line(self, lang='en'):
+    def _summary_line(self, lang='en'):
         """Return a one-line summary of the entry's data for a given language.
         Defaults to English.
         """
         lu = utils.ellipsize(str(self.lexical_unit), 20)
         gl = self.get_gloss(lang=lang)
-        gi = self.get_grammatical_info()
-        return f"{lu:20}\t{gl:30}\t{gi}"
+        return f"{lu:20}\t{gl:30}\t{self.id}"
 
-    def get_grammatical_info(self, sense_idx=0):
+    def get_id(self) -> RefId:
+        """Return the object's unique identifier"""
+        return self.id
+
+    def get_grammatical_info(self, sense_idx=0) -> GrammaticalInfo:
         """Get basic grammatical info for a given sense index [default=0].
         """
         grammatical_info = ''
-        if self.senses:
-            grammatical_info = self.senses[sense_idx].get_grammatical_info()
+        if self.sense_items:
+            grammatical_info = self.sense_items[sense_idx].get_grammatical_info()  # noqa: E501
         return grammatical_info
 
-    def get_gloss(self, sense_idx=0, lang='en'):
+    def get_gloss(self, sense_idx=0, lang='en') -> str:
         """Get gloss details for a given sense index and language.
         Defaults to index 0 and English.
         """
         gloss = ''
-        if self.senses and self.senses[sense_idx].glosses:
+        if self.sense_items and self.sense_items[sense_idx].gloss_items:
             # Choose 1st gloss if preferred language not found.
-            gloss = str(self.senses[sense_idx].glosses[0])
-            for g in self.senses[sense_idx].glosses:
+            gloss = str(self.sense_items[sense_idx].gloss_items[0])
+            for g in self.sense_items[sense_idx].gloss_items:
                 if g.lang == lang:
                     # Choose preferred language gloss.
                     gloss = str(g)
         return gloss
 
     def show(self):
         """Print an overview of the ``entry`` in the terminal window."""
         # Add header.
         text = ['\nEntry\n============']
         # Add overview line.
         if self.lexical_unit:
             text.append(f"{self.lexical_unit}; {self.get_grammatical_info()}; {self.get_gloss()}")  # noqa: E501
         # Add traits.
-        if self.traits:
-            text.append('; '.join([str(t) for t in self.traits]))
+        if self.trait_items:
+            text.append('; '.join([str(t) for t in self.trait_items]))
         # Add senses.
-        if self.senses:
-            text.append('\n'.join([f"sense: {str(s)}" for s in self.senses]))
+        if self.sense_items:
+            text.append('\n'.join([f"sense: {str(s)}" for s in self.sense_items]))  # noqa: E501
         # Add variants.
-        if self.variants:
-            text.append('; '.join(str(v) for v in self.variants))
+        if self.variant_items:
+            text.append('; '.join(str(v) for v in self.variant_items))
         # Add notes.
-        if self.notes:
-            text.append('; '.join(str(n) for n in self.notes))
+        if self.note_items:
+            text.append('; '.join(str(n) for n in self.note_items))
         # Add etymologies.
-        if self.etymologies:
-            text.append('; '.join(str(e) for e in self.etymologies))
+        if self.etymology_items:
+            text.append('; '.join(str(e) for e in self.etymology_items))
         print('\n'.join(text))
 
-    def _update_from_xml(self, xml_tree):
-        # Set initial xml_tree.
-        self.xml_tree = xml_tree
-        # Update super class attributes.
-        ext = Extensible(xml_tree)
-        ext._update_other_from_self(self)
-        del ext
-        # Update object attributes.
-        etree_to_obj_attributes(xml_tree, self)
-
 
 class Lexicon(LIFTUtilsBase):
     """This is the main class of the lexicon.
     It contains the header and all the entries in the database.
 
     :ivar str version: Specifies the lift language version number.
     :ivar Optional[str] producer: Identifies the particular producer of this
         lift file.
     :ivar Optional[Header] header: Contains the header information for the
         database.
-    :ivar Optional[List[Entry]] entries: Each of the entries in the lexicon.
+    :ivar Optional[List[Entry]] entry_items: Each of the entries in the
+        lexicon.
+    :ivar Optional[Path] path: File path to a LIFT file to import.
     """
 
+    _producer = f"LIFT-Utils {config.LIB_VERSION}"
+
     def __init__(
         self,
         path: Optional[Union[Path, str]] = None,
-        xml_tree: Optional[etree.ElementTree] = None
+        version: str = None,
+        xml_tree: Optional[etree._Element] = None
     ):
         super().__init__()
-        if xml_tree is not None:
-            super()._update_from_xml(xml_tree)
         # properties
-        self.props = Props(lift_version=config.LIFT_VERSION)
-        self.props.attributes = [
+        attribs = [
             Prop('version', required=True, prop_type=str),
             Prop('producer', prop_type=str),
         ]
-        self.props.elements = [
+        for a in attribs:
+            self.props.add_to('attributes', a)
+        elems = [
             Prop('header', prop_type=Header),
-            Prop('entries', prop_type=list, item_type=Entry),
+            Prop('entry_items', prop_type=list, item_type=Entry),
         ]
-        self.path = Path(path)
+        for e in elems:
+            self.props.add_to('elements', e)
+        self.xml_tag = 'lift'
+        self.lift_xml_tree = None
+        self.ranges_xml_tree = None
         # attributes
-        self.version: str = None
+        self.version = version
         self.producer: Optional[str] = None
         # elements
         self.header: Optional[Header] = None
-        self.entries: Optional[List[Entry]] = None
-
-        if xml_tree is not None:
+        self.entry_items: Optional[List[Entry]] = None
+        if path:
+            self.path = Path(path)
+            if self.path.suffix == '.lift':
+                self._from_lift(self.path)
+            else:
+                print(f"Error: Not a valid LIFT file: {self.path}")
+                exit(1)
+        elif xml_tree is not None:
             self._update_from_xml(xml_tree)
 
     def __str__(self):
         s = f"LIFT lexicon v{self.version}"
         if self.producer:
             s += f"; produced by {self.producer}"
         return s
 
-    def show(self):
-        """Print an overview of the ``lexicon`` in the terminal window."""
-        text = "No entries."
-        if self.entries:
-            summary_lines = [e.get_summary_line('en') for e in self.entries]
-            slist = utils.unicode_sort(summary_lines)
-            nl = '\n'
-            text = nl.join(slist)
-        print(text)
+    def find(
+        self,
+        text: str,
+        field: str = 'gloss'
+    ) -> Union[Entry, Sense, None]:
+        """Return the first matching ``Entry`` or ``Sense`` item.
+        The field searched can be "lexical-unit", "variant", "gloss", or
+        "definition", as well as any fields defined in the LIFT file's header.
+        """
+        return self._find(text, field=field)
 
-    def get_item_by_id(self, refid) -> Union[Entry, Sense, None]:
-        """Return an entry or sense by its ``RefId``."""
+    def find_all(
+        self,
+        text: str,
+        field: str = 'gloss'
+    ) -> List[Union[Entry, Sense]]:
+        """Return all matching ``Entry`` or ``Sense`` items.
+        The field searched can be "lexical-unit", "variant", "gloss",
+        "definition", or "grammatical-info", as well as any fields defined in
+        the LIFT file's header.
+        """
+        return self._find(text, field=field, get_all=True)
 
-        if not self.entries:
-            return
+    def _find(self, text, field='gloss', get_all=False):
+        items = []
+
+        target_groups = ['entries', 'senses']
+        entry_only_fields = ['lexical-unit', 'variant']
+        sense_only_fields = ['gloss', 'definition', 'grammatical-info']
+        header_fields = [f.tag for f in self.header.fields.field_items]
+        if field in entry_only_fields:
+            target_groups.remove('senses')
+        elif field in sense_only_fields:
+            target_groups.remove('entries')
+
+        for entry in self.entry_items:
+            result = search_entry(
+                entry,
+                text,
+                field,
+                target_groups,
+                header_fields,
+                get_all
+            )
+            if result is not None:
+                if not get_all:
+                    return result
+                else:
+                    items.extend(result)
+        if get_all:
+            return items
 
-        for entry in self.entries:
+    def get_item_by_id(self, refid: str) -> Union[Entry, Sense, None]:
+        """Return an entry or sense by its ``RefId``."""
+        if not self.entry_items:
+            return
+        for entry in self.entry_items:
             if entry.id == refid:
                 return entry
-            if entry.senses:
-                for sense in entry.senses:
+            if entry.sense_items:
+                for sense in entry.sense_items:
                     if sense.id == refid:
                         return sense
+                    if sense.subsense_items:
+                        for subsense in sense.subsense_items:
+                            if subsense.id == refid:
+                                return subsense
+
+    def show(self):
+        """Print an overview of the ``Lexicon`` in the terminal window."""
+        text = "No entries."
+        if self.entry_items:
+            summary_lines = [e._summary_line('en') for e in self.entry_items]  # noqa: E501
+            slist = utils.unicode_sort(summary_lines)
+            nl = '\n'
+            text = nl.join(slist)
+        print(text)
+
+    def _from_lift(self, infile):
+        infile = Path(infile)
+        if not infile.is_file():
+            print(f"Error: Invalid file path: {infile}")
+            exit(1)
+        xml_tree = xmlfile_to_etree(infile)
+        self._update_from_xml(xml_tree)
+
+    def to_lift(self, file_path: str):
+        """Save the ``Lexicon`` as a LIFT file.
+        The LIFT-RANGES file will be automatically created in the same folder
+        as the LIFT file.
+        """
+        outfile = Path(file_path).with_suffix('.lift')  # ensure suffix
+        ranges_file = outfile.with_suffix('.lift-ranges')
+        self.producer = Lexicon._producer
+
+        # Write LIFT file.
+        lift_tree = self._to_xml_tree()
+        for _range in lift_tree.find('.//ranges').getchildren():
+            for _range_element in _range:
+                _range.remove(_range_element)
+            for attrib in _range.attrib.keys():
+                if attrib not in ['id', 'href']:
+                    del _range.attrib[attrib]
+        outfile.write_text(self._to_xml(lift_tree))
+
+        # Write LIFT-RANGES file.
+        lift_ranges = self.header.ranges._to_xml_tree()
+        lift_ranges.tag = 'lift-ranges'
+        for _range in list(lift_ranges):
+            del _range.attrib['href']
+        ranges_file.write_text(self._to_xml(lift_ranges))
 
     def _update_from_xml(self, xml_tree):
         # Set initial xml_tree.
         self.xml_tree = xml_tree
         self.version = xml_tree.attrib.get('version')
         # Allow global access to version number.
         config.LIFT_VERSION = self.version
         # Update object attributes.
         etree_to_obj_attributes(xml_tree, self)
         # Update header range data from external file(s).
         ext_hrefs = set()
-        for r in self.header.ranges.ranges:
+        for r in self.header.ranges.range_items:
             if r.href:
                 ext_hrefs.add(r.href)
         for p in ext_hrefs:
             self._update_header_from_href(p)
+        # Update ranges xml_trees.
+        self.header.ranges._to_xml_tree()
 
     def _update_header_from_href(self, href: URL):
         filepath = unquote(urlparse(href).path)
         try:
-            xml_tree = xml_to_etree(filepath)
+            xml_tree = xmlfile_to_etree(filepath)
         except OSError:
             # Probably absolute URI from a different device.
             # Try same file name, but in same dir as current LIFT file.
             relpath = self.path.parent / Path(filepath).name
-            xml_tree = xml_to_etree(relpath)
+            xml_tree = xmlfile_to_etree(relpath)
 
+        # Update model data.
         for _range in xml_tree.getchildren():
-            for i, r in enumerate(self.header.ranges.ranges):
+            for i, r in enumerate(self.header.ranges.range_items[:]):
                 if _range.attrib.get('id') == r.id:
                     href = r.href
-                    self.header.ranges.ranges[i] = Range(_range)
-                    self.header.ranges.ranges[i].href = href  # add href back
+                    self.header.ranges.range_items[i] = Range(xml_tree=_range)
+                    self.header.ranges.range_items[i].href = href  # add href
+                    break
```

### Comparing `lift_utils-0.1.1/src/lift_utils.egg-info/PKG-INFO` & `lift_utils-0.2/src/lift_utils.egg-info/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: lift_utils
-Version: 0.1.1
+Version: 0.2
 Summary: Read and write LIFT files in Python.
 Author-email: Nate Marti <nate_marti@sil.org>
 License: MIT License
         
         Copyright (c) 2024 SIL-CAR
         
         Permission is hereby granted, free of charge, to any person obtaining a copy
@@ -46,14 +46,18 @@
 ## Releases
 
 Install from [PyPI.org/lift-utils](https://pypi.org/project/lift-utils/):
 ```shell
 python3 -m pip install lift_utils
 ```
 
+## Documentation
+
+https://sil-car.github.io/lift-utils
+
 ## Roadmap
 
 | Release | Feature |
 | --: | --- |
 | v0.1 | read support for LIFT files |
 | v0.2 | write support for LIFT files |
-| v0.3 | add helper methods (get, set, add, list, etc.) |
+| v0.3 | add helper methods to facilitate lexicon manipulation |
```

### Comparing `lift_utils-0.1.1/src/lift_utils.egg-info/SOURCES.txt` & `lift_utils-0.2/src/lift_utils.egg-info/SOURCES.txt`

 * *Files 27% similar despite different names*

```diff
@@ -3,21 +3,26 @@
 pyproject.toml
 src/lift_utils/__init__.py
 src/lift_utils/base.py
 src/lift_utils/config.py
 src/lift_utils/datatypes.py
 src/lift_utils/header.py
 src/lift_utils/lexicon.py
-src/lift_utils/lift.py
 src/lift_utils/utils.py
 src/lift_utils.egg-info/PKG-INFO
 src/lift_utils.egg-info/SOURCES.txt
 src/lift_utils.egg-info/dependency_links.txt
 src/lift_utils.egg-info/requires.txt
 src/lift_utils.egg-info/top_level.txt
 tests/test_base_readxml_v0_13_FW.py
 tests/test_base_readxml_v0_15.py
+tests/test_base_writexml_v0_13_FW.py
+tests/test_base_writexml_v0_15.py
 tests/test_header_readxml_v0_13_FW.py
 tests/test_header_readxml_v0_15.py
+tests/test_header_writexml_v0_13_FW.py
+tests/test_header_writexml_v0_15.py
 tests/test_lexicon_readxml_v0_13_FW.py
 tests/test_lexicon_readxml_v0_15.py
-tests/test_lift_readxml_v0_13_FW.py
+tests/test_lexicon_v0_13_FW.py
+tests/test_lexicon_writexml_v0_13_FW.py
+tests/test_lexicon_writexml_v0_15.py
```

### Comparing `lift_utils-0.1.1/tests/test_base_readxml_v0_13_FW.py` & `lift_utils-0.2/tests/test_base_readxml_v0_13_FW.py`

 * *Files 6% similar despite different names*

```diff
@@ -11,15 +11,15 @@
 ENTRY_LIFT_GOOD = str(DATA_PATH / "entry_good_v0.13_FW.lift")
 
 
 class TestAnnotation(unittest.TestCase):
     def setUp(self):
         config.LIFT_VERSION = '0.13'
         self.xml_tree = etree.parse(ENTRY_LIFT_GOOD).getroot().find('.//annotation')  # noqa: E501
-        self.obj = base.Annotation(self.xml_tree)
+        self.obj = base.Annotation(xml_tree=self.xml_tree)
 
     def test_attribs(self):
         required = [p.name for p in self.obj.props.attributes if p.required]
         test_attribs(self, self.obj, required)
         optional = [p.name for p in self.obj.props.attributes if not p.required]  # noqa: E501
         test_attribs(self, self.obj, optional)
 
@@ -45,34 +45,35 @@
         test_elems(self, self.obj, optional)
 
 
 class TestField(unittest.TestCase):
     def setUp(self):
         config.LIFT_VERSION = '0.13'
         self.xml_tree = etree.parse(ENTRY_LIFT_GOOD).getroot().find('.//field')
-        self.obj = base.Field(self.xml_tree)
+        self.obj = base.Field(xml_tree=self.xml_tree)
 
     def test_attribs(self):
         required = [p.name for p in self.obj.props.attributes if p.required]
         test_attribs(self, self.obj, required)
         optional = [p.name for p in self.obj.props.attributes if not p.required]  # noqa: E501
         test_attribs(self, self.obj, optional)
 
     def test_elems(self):
         required = [p.name for p in self.obj.props.elements if p.required]
         test_elems(self, self.obj, required)
         optional = [p.name for p in self.obj.props.elements if not p.required]
+        optional.remove('span_items')
         test_elems(self, self.obj, optional)
 
 
 class TestForm(unittest.TestCase):
     def setUp(self):
         config.LIFT_VERSION = '0.13'
         self.xml_tree = etree.parse(ENTRY_LIFT_GOOD).getroot().find('.//form')
-        self.obj = base.Form(self.xml_tree)
+        self.obj = base.Form(xml_tree=self.xml_tree)
 
     def test_attribs(self):
         required = [p.name for p in self.obj.props.attributes if p.required]
         test_attribs(self, self.obj, required)
         optional = [p.name for p in self.obj.props.attributes if not p.required]  # noqa: E501
         test_attribs(self, self.obj, optional)
 
@@ -83,87 +84,100 @@
         test_elems(self, self.obj, optional)
 
 
 class TestGloss(unittest.TestCase):
     def setUp(self):
         config.LIFT_VERSION = '0.13'
         self.xml_tree = etree.parse(ENTRY_LIFT_GOOD).getroot().find('.//gloss')
-        self.obj = base.Gloss(self.xml_tree)
+        self.obj = base.Gloss(xml_tree=self.xml_tree)
 
     def test_elems(self):
         required = [p.name for p in self.obj.props.elements if p.required]
         test_elems(self, self.obj, required)
         optional = [p.name for p in self.obj.props.elements if not p.required]
         test_elems(self, self.obj, optional)
 
 
-class TestMultitext(unittest.TestCase):
+class TestMultitextText(unittest.TestCase):
+    def setUp(self):
+        config.LIFT_VERSION = '0.13'
+        self.xml_tree = etree.parse(ENTRY_LIFT_GOOD).getroot().findall('.//annotation')[1]  # noqa: E501
+        self.obj = base.Multitext(xml_tree=self.xml_tree)
+
+    def test_attribs(self):
+        pass  # no attribs
+
+    def test_elems(self):
+        required = [p.name for p in self.obj.props.elements if p.required]
+        test_elems(self, self.obj, required)
+        optional = [p.name for p in self.obj.props.elements if not p.required]
+        optional.remove('form_items')
+        optional.remove('trait_items')
+        test_elems(self, self.obj, optional)
+
+
+class TestMultitextForm(unittest.TestCase):
     def setUp(self):
         config.LIFT_VERSION = '0.13'
         self.xml_tree = etree.parse(ENTRY_LIFT_GOOD).getroot().find('.//annotation')  # noqa: E501
-        self.obj = base.Multitext(self.xml_tree)
+        self.obj = base.Multitext(xml_tree=self.xml_tree)
 
     def test_attribs(self):
         pass  # no attribs
 
     def test_elems(self):
         required = [p.name for p in self.obj.props.elements if p.required]
+        required.remove('pcdata')
         test_elems(self, self.obj, required)
         optional = [p.name for p in self.obj.props.elements if not p.required]
+        optional.remove('span_items')
         test_elems(self, self.obj, optional)
 
 
 class TestSpan(unittest.TestCase):
     def setUp(self):
         config.LIFT_VERSION = '0.13'
         self.xml_tree = etree.parse(ENTRY_LIFT_GOOD).getroot().find('.//span')
-        self.obj = base.Span(self.xml_tree)
+        self.obj = base.Span(xml_tree=self.xml_tree)
 
     def test_attribs(self):
         required = [p.name for p in self.obj.props.attributes if p.required]
         test_attribs(self, self.obj, required)
         optional = [p.name for p in self.obj.props.attributes if not p.required]  # noqa: E501
         test_attribs(self, self.obj, optional)
 
     def test_elems(self):
         required = [p.name for p in self.obj.props.elements if p.required]
         test_elems(self, self.obj, required)
         optional = [p.name for p in self.obj.props.elements if not p.required]
-        optional.remove('spans')  # hard to test optional span-in-span element
+        optional.remove('span_items')  # hard to test optional nested element
         test_elems(self, self.obj, optional)
 
 
 class TestText(unittest.TestCase):
     def setUp(self):
         config.LIFT_VERSION = '0.13'
-        self.xml_tree = etree.parse(ENTRY_LIFT_GOOD).getroot().find('.//form')
-        self.obj = None
-        for c in self.xml_tree.getchildren():
-            if c.tag == 'text':
-                self.obj = base.Text(c)
-                break
-        if not self.obj:
-            raise AssertionError
+        self.xml_tree = etree.parse(ENTRY_LIFT_GOOD).getroot().find('.//text')
+        self.obj = base.Text(xml_tree=self.xml_tree)
 
     def test_attribs(self):
         pass  # no attribs
 
     def test_elems(self):
         required = [p.name for p in self.obj.props.elements if p.required]
         test_elems(self, self.obj, required)
         optional = [p.name for p in self.obj.props.elements if not p.required]
-        optional.remove('spans')  # already tested in TestSpan
         test_elems(self, self.obj, optional)
 
 
 class TestTrait(unittest.TestCase):
     def setUp(self):
         config.LIFT_VERSION = '0.13'
         self.xml_tree = etree.parse(ENTRY_LIFT_GOOD).getroot().find('trait')
-        self.obj = base.Trait(self.xml_tree)
+        self.obj = base.Trait(xml_tree=self.xml_tree)
 
     def test_attribs(self):
         required = [p.name for p in self.obj.props.attributes if p.required]
         test_attribs(self, self.obj, required)
         optional = [p.name for p in self.obj.props.attributes if not p.required]  # noqa: E501
         test_attribs(self, self.obj, optional)
 
@@ -174,15 +188,15 @@
         test_elems(self, self.obj, optional)
 
 
 class TestURLRef(unittest.TestCase):
     def setUp(self):
         config.LIFT_VERSION = '0.13'
         self.xml_tree = etree.parse(ENTRY_LIFT_GOOD).getroot().find('.//urlref')  # noqa: E501
-        self.obj = base.URLRef(self.xml_tree)
+        self.obj = base.URLRef(xml_tree=self.xml_tree)
 
     def test_attribs(self):
         required = [p.name for p in self.obj.props.attributes if p.required]
         test_attribs(self, self.obj, required)
         optional = [p.name for p in self.obj.props.attributes if not p.required]  # noqa: E501
         test_attribs(self, self.obj, optional)
```

### Comparing `lift_utils-0.1.1/tests/test_base_readxml_v0_15.py` & `lift_utils-0.2/tests/test_base_readxml_v0_15.py`

 * *Files 3% similar despite different names*

```diff
@@ -11,15 +11,15 @@
 ENTRY_LIFT_GOOD = str(DATA_PATH / "entry_good_v0.15.lift")
 
 
 class TestAnnotation(unittest.TestCase):
     def setUp(self):
         config.LIFT_VERSION = config.LIFT_VERSION_LATEST
         self.xml_tree = etree.parse(ENTRY_LIFT_GOOD).getroot().find('.//annotation')  # noqa: E501
-        self.obj = base.Annotation(self.xml_tree)
+        self.obj = base.Annotation(xml_tree=self.xml_tree)
 
     def test_attribs(self):
         required = [p.name for p in self.obj.props.attributes if p.required]
         test_attribs(self, self.obj, required)
         optional = [p.name for p in self.obj.props.attributes if not p.required]  # noqa: E501
         test_attribs(self, self.obj, optional)
 
@@ -45,34 +45,35 @@
         test_elems(self, self.obj, optional)
 
 
 class TestField(unittest.TestCase):
     def setUp(self):
         config.LIFT_VERSION = config.LIFT_VERSION_LATEST
         self.xml_tree = etree.parse(ENTRY_LIFT_GOOD).getroot().find('.//field')
-        self.obj = base.Field(self.xml_tree)
+        self.obj = base.Field(xml_tree=self.xml_tree)
 
     def test_attribs(self):
         required = [p.name for p in self.obj.props.attributes if p.required]
         test_attribs(self, self.obj, required)
         optional = [p.name for p in self.obj.props.attributes if not p.required]  # noqa: E501
         test_attribs(self, self.obj, optional)
 
     def test_elems(self):
         required = [p.name for p in self.obj.props.elements if p.required]
         test_elems(self, self.obj, required)
         optional = [p.name for p in self.obj.props.elements if not p.required]
+        optional.remove('span_items')
         test_elems(self, self.obj, optional)
 
 
 class TestForm(unittest.TestCase):
     def setUp(self):
         config.LIFT_VERSION = config.LIFT_VERSION_LATEST
         self.xml_tree = etree.parse(ENTRY_LIFT_GOOD).getroot().find('.//form')
-        self.obj = base.Form(self.xml_tree)
+        self.obj = base.Form(xml_tree=self.xml_tree)
 
     def test_attribs(self):
         required = [p.name for p in self.obj.props.attributes if p.required]
         test_attribs(self, self.obj, required)
         optional = [p.name for p in self.obj.props.attributes if not p.required]  # noqa: E501
         test_attribs(self, self.obj, optional)
 
@@ -83,58 +84,57 @@
         test_elems(self, self.obj, optional)
 
 
 class TestGloss(unittest.TestCase):
     def setUp(self):
         config.LIFT_VERSION = config.LIFT_VERSION_LATEST
         self.xml_tree = etree.parse(ENTRY_LIFT_GOOD).getroot().find('.//gloss')
-        self.obj = base.Gloss(self.xml_tree)
+        self.obj = base.Gloss(xml_tree=self.xml_tree)
 
     def test_elems(self):
         required = [p.name for p in self.obj.props.elements if p.required]
         test_elems(self, self.obj, required)
         optional = [p.name for p in self.obj.props.elements if not p.required]
         test_elems(self, self.obj, optional)
 
 
 class TestMultitext(unittest.TestCase):
     def setUp(self):
         config.LIFT_VERSION = config.LIFT_VERSION_LATEST
         self.xml_tree = etree.parse(ENTRY_LIFT_GOOD).getroot().find('.//annotation')  # noqa: E501
-        self.obj = base.Multitext(self.xml_tree)
+        self.obj = base.Multitext(xml_tree=self.xml_tree)
 
     def test_attribs(self):
         pass  # no attribs
 
     def test_elems(self):
         required = [p.name for p in self.obj.props.elements if p.required]
         test_elems(self, self.obj, required)
         optional = [p.name for p in self.obj.props.elements if not p.required]
-        if config.LIFT_VERSION != config.LIFT_VERSION_FIELDWORKS:
-            optional.remove('text')  # remove deprecated element
+        optional.remove('span_items')
         test_elems(self, self.obj, optional)
 
 
 class TestSpan(unittest.TestCase):
     def setUp(self):
         config.LIFT_VERSION = config.LIFT_VERSION_LATEST
         self.xml_tree = etree.parse(ENTRY_LIFT_GOOD).getroot().find('.//span')
-        self.obj = base.Span(self.xml_tree)
+        self.obj = base.Span(xml_tree=self.xml_tree)
 
     def test_attribs(self):
         required = [p.name for p in self.obj.props.attributes if p.required]
         test_attribs(self, self.obj, required)
         optional = [p.name for p in self.obj.props.attributes if not p.required]  # noqa: E501
         test_attribs(self, self.obj, optional)
 
     def test_elems(self):
         required = [p.name for p in self.obj.props.elements if p.required]
         test_elems(self, self.obj, required)
         optional = [p.name for p in self.obj.props.elements if not p.required]
-        optional.remove('spans')  # hard to test optional span-in-span element
+        optional.remove('span_items')  # hard to test optional nested element
         test_elems(self, self.obj, optional)
 
 
 class TestText(unittest.TestCase):
     def setUp(self):
         config.LIFT_VERSION = config.LIFT_VERSION_LATEST
         self.xml_tree = etree.parse(ENTRY_LIFT_GOOD).getroot().find('.//form')
@@ -149,23 +149,23 @@
     def test_attribs(self):
         pass  # no attribs
 
     def test_elems(self):
         required = [p.name for p in self.obj.props.elements if p.required]
         test_elems(self, self.obj, required)
         optional = [p.name for p in self.obj.props.elements if not p.required]
-        optional.remove('spans')  # already tested in TestSpan
+        optional.remove('span_items')  # already tested in TestSpan
         test_elems(self, self.obj, optional)
 
 
 class TestTrait(unittest.TestCase):
     def setUp(self):
         config.LIFT_VERSION = config.LIFT_VERSION_LATEST
         self.xml_tree = etree.parse(ENTRY_LIFT_GOOD).getroot().find('trait')
-        self.obj = base.Trait(self.xml_tree)
+        self.obj = base.Trait(xml_tree=self.xml_tree)
 
     def test_attribs(self):
         required = [p.name for p in self.obj.props.attributes if p.required]
         test_attribs(self, self.obj, required)
         optional = [p.name for p in self.obj.props.attributes if not p.required]  # noqa: E501
         test_attribs(self, self.obj, optional)
 
@@ -176,15 +176,15 @@
         test_elems(self, self.obj, optional)
 
 
 class TestURLRef(unittest.TestCase):
     def setUp(self):
         config.LIFT_VERSION = config.LIFT_VERSION_LATEST
         self.xml_tree = etree.parse(ENTRY_LIFT_GOOD).getroot().find('.//urlref')  # noqa: E501
-        self.obj = base.URLRef(self.xml_tree)
+        self.obj = base.URLRef(xml_tree=self.xml_tree)
 
     def test_attribs(self):
         required = [p.name for p in self.obj.props.attributes if p.required]
         test_attribs(self, self.obj, required)
         optional = [p.name for p in self.obj.props.attributes if not p.required]  # noqa: E501
         test_attribs(self, self.obj, optional)
```

### Comparing `lift_utils-0.1.1/tests/test_header_readxml_v0_13_FW.py` & `lift_utils-0.2/tests/test_header_readxml_v0_13_FW.py`

 * *Files 2% similar despite different names*

```diff
@@ -12,101 +12,101 @@
 LIFT_VERSION = '0.13'
 
 
 class TestFieldDefn(unittest.TestCase):
     def setUp(self):
         config.LIFT_VERSION = LIFT_VERSION
         self.xml_tree = etree.parse(HEADER_LIFT_GOOD).getroot().find('.//field')  # noqa: E501
-        self.obj = header.FieldDefn(self.xml_tree)
+        self.obj = header.FieldDefn(xml_tree=self.xml_tree)
 
     def test_attribs(self):
         required = [p.name for p in self.obj.props.attributes if p.required]
         test_attribs(self, self.obj, required)
         optional = [p.name for p in self.obj.props.attributes if not p.required]  # noqa: E501
         test_attribs(self, self.obj, optional)
 
 
 class TestFieldDefns(unittest.TestCase):
     def setUp(self):
         config.LIFT_VERSION = LIFT_VERSION
         self.xml_tree = etree.parse(HEADER_LIFT_GOOD).getroot().find('.//fields')  # noqa: E501
-        self.obj = header.FieldDefns(self.xml_tree)
+        self.obj = header.FieldDefns(xml_tree=self.xml_tree)
 
     def test_attribs(self):
         pass  # no attributes to test
 
     def test_elems(self):
         required = [p.name for p in self.obj.props.elements if p.required]
         test_elems(self, self.obj, required)
         optional = [p.name for p in self.obj.props.elements if not p.required]
         test_elems(self, self.obj, optional)
 
     def test_items(self):
-        self.assertTrue(len(self.obj.fields) > 1)
+        self.assertTrue(len(self.obj.field_items) > 1)
 
 
 class TestHeader(unittest.TestCase):
     def setUp(self):
         config.LIFT_VERSION = LIFT_VERSION
         self.xml_tree = etree.parse(HEADER_LIFT_GOOD).getroot().find('.//header')  # noqa: E501
-        self.obj = header.Header(self.xml_tree)
+        self.obj = header.Header(xml_tree=self.xml_tree)
 
     def test_attribs(self):
         pass  # no attributes to test
 
     def test_elems(self):
         required = [p.name for p in self.obj.props.elements if p.required]
         test_elems(self, self.obj, required)
         optional = [p.name for p in self.obj.props.elements if not p.required]
         test_elems(self, self.obj, optional)
 
 
-class TestRanges(unittest.TestCase):
+class TestRange(unittest.TestCase):
     def setUp(self):
         config.LIFT_VERSION = LIFT_VERSION
-        self.xml_tree = etree.parse(HEADER_LIFT_GOOD).getroot().find('.//ranges')  # noqa: E501
-        self.obj = header.Ranges(self.xml_tree)
+        self.xml_tree = etree.parse(HEADER_LIFT_GOOD).getroot().find('.//range')  # noqa: E501
+        self.obj = header.Range(xml_tree=self.xml_tree)
 
     def test_attribs(self):
-        pass  # no attributes
+        required = [p.name for p in self.obj.props.attributes if p.required]
+        test_attribs(self, self.obj, required)
+        optional = [p.name for p in self.obj.props.attributes if not p.required]  # noqa: E501
+        test_attribs(self, self.obj, optional)
 
     def test_elems(self):
         required = [p.name for p in self.obj.props.elements if p.required]
         test_elems(self, self.obj, required)
         optional = [p.name for p in self.obj.props.elements if not p.required]
         test_elems(self, self.obj, optional)
 
-    def test_items(self):
-        self.assertTrue(len(self.obj.ranges) > 1)
-
 
-class TestRange(unittest.TestCase):
+class TestRanges(unittest.TestCase):
     def setUp(self):
         config.LIFT_VERSION = LIFT_VERSION
-        self.xml_tree = etree.parse(HEADER_LIFT_GOOD).getroot().find('.//range')  # noqa: E501
-        self.obj = header.Range(self.xml_tree)
+        self.xml_tree = etree.parse(HEADER_LIFT_GOOD).getroot().find('.//ranges')  # noqa: E501
+        self.obj = header.Ranges(xml_tree=self.xml_tree)
 
     def test_attribs(self):
-        required = [p.name for p in self.obj.props.attributes if p.required]
-        test_attribs(self, self.obj, required)
-        optional = [p.name for p in self.obj.props.attributes if not p.required]  # noqa: E501
-        test_attribs(self, self.obj, optional)
+        pass  # no attributes
 
     def test_elems(self):
         required = [p.name for p in self.obj.props.elements if p.required]
         test_elems(self, self.obj, required)
         optional = [p.name for p in self.obj.props.elements if not p.required]
         test_elems(self, self.obj, optional)
 
+    def test_items(self):
+        self.assertTrue(len(self.obj.range_items) > 1)
+
 
 class TestRangeElement(unittest.TestCase):
     def setUp(self):
         config.LIFT_VERSION = LIFT_VERSION
         self.xml_tree = etree.parse(HEADER_LIFT_GOOD).getroot().find('.//range-element')  # noqa: E501
-        self.obj = header.RangeElement(self.xml_tree)
+        self.obj = header.RangeElement(xml_tree=self.xml_tree)
 
     def test_attribs(self):
         required = [p.name for p in self.obj.props.attributes if p.required]
         test_attribs(self, self.obj, required)
         optional = [p.name for p in self.obj.props.attributes if not p.required]  # noqa: E501
         test_attribs(self, self.obj, optional)
```

### Comparing `lift_utils-0.1.1/tests/test_header_readxml_v0_15.py` & `lift_utils-0.2/tests/test_header_readxml_v0_15.py`

 * *Files 4% similar despite different names*

```diff
@@ -12,15 +12,15 @@
 LIFT_VERSION = '0.15'
 
 
 class TestFieldDefinition(unittest.TestCase):
     def setUp(self):
         config.LIFT_VERSION = LIFT_VERSION
         self.xml_tree = etree.parse(HEADER_LIFT_GOOD).getroot().find('.//field')  # noqa: E501
-        self.obj = header.FieldDefinition(self.xml_tree)
+        self.obj = header.FieldDefinition(xml_tree=self.xml_tree)
 
     def test_attribs(self):
         required = [p.name for p in self.obj.props.attributes if p.required]
         test_attribs(self, self.obj, required)
         optional = [p.name for p in self.obj.props.attributes if not p.required]  # noqa: E501
         test_attribs(self, self.obj, optional)
 
@@ -31,31 +31,31 @@
         test_elems(self, self.obj, optional)
 
 
 class TestFields(unittest.TestCase):
     def setUp(self):
         config.LIFT_VERSION = LIFT_VERSION
         self.xml_tree = etree.parse(HEADER_LIFT_GOOD).getroot().find('.//fields')  # noqa: E501
-        self.obj = header.Fields(self.xml_tree)
+        self.obj = header.Fields(xml_tree=self.xml_tree)
 
     def test_elems(self):
         required = [p.name for p in self.obj.props.elements if p.required]
         test_elems(self, self.obj, required)
         optional = [p.name for p in self.obj.props.elements if not p.required]
         test_elems(self, self.obj, optional)
 
     def test_items(self):
-        self.assertTrue(len(self.obj.field_definitions) > 1)
+        self.assertTrue(len(self.obj.field_items) > 1)
 
 
 class TestHeader(unittest.TestCase):
     def setUp(self):
         config.LIFT_VERSION = LIFT_VERSION
         self.xml_tree = etree.parse(HEADER_LIFT_GOOD).getroot().find('.//header')  # noqa: E501
-        self.obj = header.Header(self.xml_tree)
+        self.obj = header.Header(xml_tree=self.xml_tree)
 
     def test_attribs(self):
         pass  # no attributes to test
 
     def test_elems(self):
         required = [p.name for p in self.obj.props.elements if p.required]
         test_elems(self, self.obj, required)
@@ -63,58 +63,64 @@
         test_elems(self, self.obj, optional)
 
 
 class TestRanges(unittest.TestCase):
     def setUp(self):
         config.LIFT_VERSION = LIFT_VERSION
         self.xml_tree = etree.parse(HEADER_LIFT_GOOD).getroot().find('.//ranges')  # noqa: E501
-        self.obj = header.Ranges(self.xml_tree)
+        self.obj = header.Ranges(xml_tree=self.xml_tree)
 
     def test_attribs(self):
         pass  # no attributes
 
     def test_elems(self):
         required = [p.name for p in self.obj.props.elements if p.required]
         test_elems(self, self.obj, required)
         optional = [p.name for p in self.obj.props.elements if not p.required]
         test_elems(self, self.obj, optional)
 
     def test_items(self):
-        self.assertTrue(len(self.obj.ranges) > 1)
+        self.assertTrue(len(self.obj.range_items) > 1)
 
 
 class TestRange(unittest.TestCase):
     def setUp(self):
         config.LIFT_VERSION = LIFT_VERSION
         self.xml_tree = etree.parse(HEADER_LIFT_GOOD).getroot().find('.//range')  # noqa: E501
-        self.obj = header.Range(self.xml_tree)
+        self.obj = header.Range(xml_tree=self.xml_tree)
 
     def test_attribs(self):
         required = [p.name for p in self.obj.props.attributes if p.required]
         test_attribs(self, self.obj, required)
         optional = [p.name for p in self.obj.props.attributes if not p.required]  # noqa: E501
         test_attribs(self, self.obj, optional)
 
     def test_elems(self):
         required = [p.name for p in self.obj.props.elements if p.required]
         test_elems(self, self.obj, required)
         optional = [p.name for p in self.obj.props.elements if not p.required]
+        optional.remove('annotation_items')
+        optional.remove('field_items')
+        optional.remove('trait_items')
         test_elems(self, self.obj, optional)
 
 
 class TestRangeElement(unittest.TestCase):
     def setUp(self):
         config.LIFT_VERSION = LIFT_VERSION
         self.xml_tree = etree.parse(HEADER_LIFT_GOOD).getroot().find('.//range-element')  # noqa: E501
-        self.obj = header.RangeElement(self.xml_tree)
+        self.obj = header.RangeElement(xml_tree=self.xml_tree)
 
     def test_attribs(self):
         required = [p.name for p in self.obj.props.attributes if p.required]
         test_attribs(self, self.obj, required)
         optional = [p.name for p in self.obj.props.attributes if not p.required]  # noqa: E501
         test_attribs(self, self.obj, optional)
 
     def test_elems(self):
         required = [p.name for p in self.obj.props.elements if p.required]
         test_elems(self, self.obj, required)
         optional = [p.name for p in self.obj.props.elements if not p.required]
+        optional.remove('annotation_items')
+        optional.remove('field_items')
+        optional.remove('trait_items')
         test_elems(self, self.obj, optional)
```

### Comparing `lift_utils-0.1.1/tests/test_lexicon_readxml_v0_13_FW.py` & `lift_utils-0.2/tests/test_lexicon_readxml_v0_13_FW.py`

 * *Files 3% similar despite different names*

```diff
@@ -8,145 +8,147 @@
 from lift_utils import config
 from lift_utils import lexicon
 
 LIFT_GOOD = str(DATA_PATH / "lexicon_good_v0.13_FW.lift")
 LIFT_VERSION = '0.13'
 
 
-class TestLexicon(unittest.TestCase):
+class TestEntry(unittest.TestCase):
     def setUp(self):
-        self.xml_tree = etree.parse(LIFT_GOOD).getroot()
-        self.obj = lexicon.Lexicon(LIFT_GOOD, self.xml_tree)
+        self.xml_tree = etree.parse(LIFT_GOOD).getroot().find('.//entry')
+        self.obj = lexicon.Entry(xml_tree=self.xml_tree)
 
     def test_attribs(self):
         required = [p.name for p in self.obj.props.attributes if p.required]
         test_attribs(self, self.obj, required)
         optional = [p.name for p in self.obj.props.attributes if not p.required]  # noqa: E501
         test_attribs(self, self.obj, optional)
 
     def test_elems(self):
         required = [p.name for p in self.obj.props.elements if p.required]
         test_elems(self, self.obj, required)
         optional = [p.name for p in self.obj.props.elements if not p.required]
         test_elems(self, self.obj, optional)
 
-    def test_entries(self):
-        self.assertTrue(len(self.obj.entries) > 0)
-
-    def test_update_header_from_file(self):
-        self.assertTrue(len(self.obj.header.ranges.ranges) > 1)
-
 
-class TestEntry(unittest.TestCase):
+class TestEtymology(unittest.TestCase):
     def setUp(self):
-        self.xml_tree = etree.parse(LIFT_GOOD).getroot().find('.//entry')
-        self.obj = lexicon.Entry(self.xml_tree)
+        self.xml_tree = etree.parse(LIFT_GOOD).getroot().find('.//etymology')
+        self.obj = lexicon.Etymology(xml_tree=self.xml_tree)
 
     def test_attribs(self):
         required = [p.name for p in self.obj.props.attributes if p.required]
         test_attribs(self, self.obj, required)
         optional = [p.name for p in self.obj.props.attributes if not p.required]  # noqa: E501
         test_attribs(self, self.obj, optional)
 
     def test_elems(self):
         required = [p.name for p in self.obj.props.elements if p.required]
         test_elems(self, self.obj, required)
         optional = [p.name for p in self.obj.props.elements if not p.required]
         test_elems(self, self.obj, optional)
 
 
-class TestEtymology(unittest.TestCase):
+class TestExample(unittest.TestCase):
     def setUp(self):
-        self.xml_tree = etree.parse(LIFT_GOOD).getroot().find('.//etymology')
-        self.obj = lexicon.Etymology(self.xml_tree)
+        config.LIFT_VERSION = LIFT_VERSION
+        self.xml_tree = etree.parse(LIFT_GOOD).getroot().find('.//example')
+        self.obj = lexicon.Example(xml_tree=self.xml_tree)
 
     def test_attribs(self):
         required = [p.name for p in self.obj.props.attributes if p.required]
         test_attribs(self, self.obj, required)
         optional = [p.name for p in self.obj.props.attributes if not p.required]  # noqa: E501
         test_attribs(self, self.obj, optional)
 
     def test_elems(self):
         required = [p.name for p in self.obj.props.elements if p.required]
         test_elems(self, self.obj, required)
         optional = [p.name for p in self.obj.props.elements if not p.required]
+        optional.remove('span_items')
         test_elems(self, self.obj, optional)
 
 
-class TestExample(unittest.TestCase):
+class TestGrammaticalInfo(unittest.TestCase):
     def setUp(self):
-        config.LIFT_VERSION = LIFT_VERSION
-        self.xml_tree = etree.parse(LIFT_GOOD).getroot().find('.//example')
-        self.obj = lexicon.Example(self.xml_tree)
+        self.xml_tree = etree.parse(LIFT_GOOD).getroot().find('.//grammatical-info')  # noqa: E501
+        self.obj = lexicon.GrammaticalInfo(xml_tree=self.xml_tree)
 
     def test_attribs(self):
         required = [p.name for p in self.obj.props.attributes if p.required]
         test_attribs(self, self.obj, required)
         optional = [p.name for p in self.obj.props.attributes if not p.required]  # noqa: E501
         test_attribs(self, self.obj, optional)
 
     def test_elems(self):
         required = [p.name for p in self.obj.props.elements if p.required]
         test_elems(self, self.obj, required)
         optional = [p.name for p in self.obj.props.elements if not p.required]
         test_elems(self, self.obj, optional)
 
 
-class TestGrammaticalInfo(unittest.TestCase):
+class TestLexicon(unittest.TestCase):
     def setUp(self):
-        self.xml_tree = etree.parse(LIFT_GOOD).getroot().find('.//grammatical-info')  # noqa: E501
-        self.obj = lexicon.GrammaticalInfo(self.xml_tree)
+        self.xml_tree = etree.parse(LIFT_GOOD).getroot()
+        self.obj = lexicon.Lexicon(path=LIFT_GOOD, xml_tree=self.xml_tree)
 
     def test_attribs(self):
         required = [p.name for p in self.obj.props.attributes if p.required]
         test_attribs(self, self.obj, required)
         optional = [p.name for p in self.obj.props.attributes if not p.required]  # noqa: E501
         test_attribs(self, self.obj, optional)
 
     def test_elems(self):
         required = [p.name for p in self.obj.props.elements if p.required]
         test_elems(self, self.obj, required)
         optional = [p.name for p in self.obj.props.elements if not p.required]
         test_elems(self, self.obj, optional)
 
+    def test_entry_items(self):
+        self.assertTrue(len(self.obj.entry_items) > 0)
+
+    def test_update_header_from_file(self):
+        self.assertTrue(len(self.obj.header.ranges.range_items) > 1)
+
 
 class TestNote(unittest.TestCase):
     def setUp(self):
         self.xml_tree = etree.parse(LIFT_GOOD).getroot().find('.//note')
-        self.obj = lexicon.Note(self.xml_tree)
+        self.obj = lexicon.Note(xml_tree=self.xml_tree)
 
     def test_attribs(self):
         required = [p.name for p in self.obj.props.attributes if p.required]
         test_attribs(self, self.obj, required)
         optional = [p.name for p in self.obj.props.attributes if not p.required]  # noqa: E501
         test_attribs(self, self.obj, optional)
 
     def test_elems(self):
         pass  # no elements
 
 
 class TestPhonetic(unittest.TestCase):
     def setUp(self):
         self.xml_tree = etree.parse(LIFT_GOOD).getroot().find('.//pronunciation')  # noqa: E501
-        self.obj = lexicon.Phonetic(self.xml_tree)
+        self.obj = lexicon.Phonetic(xml_tree=self.xml_tree)
 
     def test_attribs(self):
         pass  # no attributes
 
     def test_elems(self):
         required = [p.name for p in self.obj.props.elements if p.required]
         test_elems(self, self.obj, required)
         optional = [p.name for p in self.obj.props.elements if not p.required]
+        optional.remove('span_items')
         test_elems(self, self.obj, optional)
 
 
 class TestRelation(unittest.TestCase):
     def setUp(self):
         self.xml_tree = etree.parse(LIFT_GOOD).getroot().find('.//relation')
-        self.obj = lexicon.Relation(self.xml_tree)
+        self.obj = lexicon.Relation(xml_tree=self.xml_tree)
 
     def test_attribs(self):
         required = [p.name for p in self.obj.props.attributes if p.required]
         test_attribs(self, self.obj, required)
         optional = [p.name for p in self.obj.props.attributes if not p.required]  # noqa: E501
         test_attribs(self, self.obj, optional)
 
@@ -156,33 +158,34 @@
         optional = [p.name for p in self.obj.props.elements if not p.required]
         test_elems(self, self.obj, optional)
 
 
 class TestReversal(unittest.TestCase):
     def setUp(self):
         self.xml_tree = etree.parse(LIFT_GOOD).getroot().find('.//reversal')
-        self.obj = lexicon.Reversal(self.xml_tree)
+        self.obj = lexicon.Reversal(xml_tree=self.xml_tree)
 
     def test_attribs(self):
         required = [p.name for p in self.obj.props.attributes if p.required]
         test_attribs(self, self.obj, required)
         optional = [p.name for p in self.obj.props.attributes if not p.required]  # noqa: E501
         test_attribs(self, self.obj, optional)
 
     def test_elems(self):
         required = [p.name for p in self.obj.props.elements if p.required]
         test_elems(self, self.obj, required)
         optional = [p.name for p in self.obj.props.elements if not p.required]
+        optional.remove('span_items')
         test_elems(self, self.obj, optional)
 
 
 class TestSense(unittest.TestCase):
     def setUp(self):
         self.xml_tree = etree.parse(LIFT_GOOD).getroot().find('.//sense')
-        self.obj = lexicon.Sense(self.xml_tree)
+        self.obj = lexicon.Sense(xml_tree=self.xml_tree)
 
     def test_attribs(self):
         required = [p.name for p in self.obj.props.attributes if p.required]
         test_attribs(self, self.obj, required)
         optional = [p.name for p in self.obj.props.attributes if not p.required]  # noqa: E501
         test_attribs(self, self.obj, optional)
 
@@ -192,35 +195,36 @@
         optional = [p.name for p in self.obj.props.elements if not p.required]
         test_elems(self, self.obj, optional)
 
 
 class TestTranslation(unittest.TestCase):
     def setUp(self):
         self.xml_tree = etree.parse(LIFT_GOOD).getroot().find('.//translation')
-        self.obj = lexicon.Translation(self.xml_tree)
+        self.obj = lexicon.Translation(xml_tree=self.xml_tree)
 
     def test_attribs(self):
         required = [p.name for p in self.obj.props.attributes if p.required]
         test_attribs(self, self.obj, required)
         optional = [p.name for p in self.obj.props.attributes if not p.required]  # noqa: E501
         test_attribs(self, self.obj, optional)
 
     def test_elems(self):
         pass  # no elements
 
 
 class TestVariant(unittest.TestCase):
     def setUp(self):
         self.xml_tree = etree.parse(LIFT_GOOD).getroot().find('.//variant')
-        self.obj = lexicon.Variant(self.xml_tree)
+        self.obj = lexicon.Variant(xml_tree=self.xml_tree)
 
     def test_attribs(self):
         required = [p.name for p in self.obj.props.attributes if p.required]
         test_attribs(self, self.obj, required)
         optional = [p.name for p in self.obj.props.attributes if not p.required]  # noqa: E501
         test_attribs(self, self.obj, optional)
 
     def test_elems(self):
         required = [p.name for p in self.obj.props.elements if p.required]
         test_elems(self, self.obj, required)
         optional = [p.name for p in self.obj.props.elements if not p.required]
+        optional.remove('span_items')
         test_elems(self, self.obj, optional)
```

### Comparing `lift_utils-0.1.1/tests/test_lexicon_readxml_v0_15.py` & `lift_utils-0.2/tests/test_lexicon_readxml_v0_15.py`

 * *Files 2% similar despite different names*

```diff
@@ -11,15 +11,15 @@
 LIFT_GOOD = str(DATA_PATH / "lexicon_good_v0.15.lift")
 LIFT_VERSION = '0.15'
 
 
 class TestLexicon(unittest.TestCase):
     def setUp(self):
         self.xml_tree = etree.parse(LIFT_GOOD).getroot()
-        self.obj = lexicon.Lexicon(LIFT_GOOD, self.xml_tree)
+        self.obj = lexicon.Lexicon(path=LIFT_GOOD, xml_tree=self.xml_tree)
 
     def test_attribs(self):
         required = [p.name for p in self.obj.props.attributes if p.required]
         test_attribs(self, self.obj, required)
         optional = [p.name for p in self.obj.props.attributes if not p.required]  # noqa: E501
         test_attribs(self, self.obj, optional)
 
@@ -29,15 +29,15 @@
         optional = [p.name for p in self.obj.props.elements if not p.required]
         test_elems(self, self.obj, optional)
 
 
 class TestEntry(unittest.TestCase):
     def setUp(self):
         self.xml_tree = etree.parse(LIFT_GOOD).getroot().find('.//entry')
-        self.obj = lexicon.Entry(self.xml_tree)
+        self.obj = lexicon.Entry(xml_tree=self.xml_tree)
 
     def test_attribs(self):
         required = [p.name for p in self.obj.props.attributes if p.required]
         test_attribs(self, self.obj, required)
         optional = [p.name for p in self.obj.props.attributes if not p.required]  # noqa: E501
         test_attribs(self, self.obj, optional)
 
@@ -47,15 +47,15 @@
         optional = [p.name for p in self.obj.props.elements if not p.required]
         test_elems(self, self.obj, optional)
 
 
 class TestEtymology(unittest.TestCase):
     def setUp(self):
         self.xml_tree = etree.parse(LIFT_GOOD).getroot().find('.//etymology')
-        self.obj = lexicon.Etymology(self.xml_tree)
+        self.obj = lexicon.Etymology(xml_tree=self.xml_tree)
 
     def test_attribs(self):
         required = [p.name for p in self.obj.props.attributes if p.required]
         test_attribs(self, self.obj, required)
         optional = [p.name for p in self.obj.props.attributes if not p.required]  # noqa: E501
         test_attribs(self, self.obj, optional)
 
@@ -66,33 +66,34 @@
         test_elems(self, self.obj, optional)
 
 
 class TestExample(unittest.TestCase):
     def setUp(self):
         config.LIFT_VERSION = LIFT_VERSION
         self.xml_tree = etree.parse(LIFT_GOOD).getroot().find('.//example')
-        self.obj = lexicon.Example(self.xml_tree)
+        self.obj = lexicon.Example(xml_tree=self.xml_tree)
 
     def test_attribs(self):
         required = [p.name for p in self.obj.props.attributes if p.required]
         test_attribs(self, self.obj, required)
         optional = [p.name for p in self.obj.props.attributes if not p.required]  # noqa: E501
         test_attribs(self, self.obj, optional)
 
     def test_elems(self):
         required = [p.name for p in self.obj.props.elements if p.required]
         test_elems(self, self.obj, required)
         optional = [p.name for p in self.obj.props.elements if not p.required]
+        optional.remove('span_items')
         test_elems(self, self.obj, optional)
 
 
 class TestGrammaticalInfo(unittest.TestCase):
     def setUp(self):
         self.xml_tree = etree.parse(LIFT_GOOD).getroot().find('.//grammatical-info')  # noqa: E501
-        self.obj = lexicon.GrammaticalInfo(self.xml_tree)
+        self.obj = lexicon.GrammaticalInfo(xml_tree=self.xml_tree)
 
     def test_attribs(self):
         required = [p.name for p in self.obj.props.attributes if p.required]
         test_attribs(self, self.obj, required)
         optional = [p.name for p in self.obj.props.attributes if not p.required]  # noqa: E501
         test_attribs(self, self.obj, optional)
 
@@ -102,45 +103,46 @@
         optional = [p.name for p in self.obj.props.elements if not p.required]
         test_elems(self, self.obj, optional)
 
 
 class TestNote(unittest.TestCase):
     def setUp(self):
         self.xml_tree = etree.parse(LIFT_GOOD).getroot().find('.//note')
-        self.obj = lexicon.Note(self.xml_tree)
+        self.obj = lexicon.Note(xml_tree=self.xml_tree)
 
     def test_attribs(self):
         required = [p.name for p in self.obj.props.attributes if p.required]
         test_attribs(self, self.obj, required)
         optional = [p.name for p in self.obj.props.attributes if not p.required]  # noqa: E501
         test_attribs(self, self.obj, optional)
 
     def test_elems(self):
         pass  # no elements
 
 
 class TestPhonetic(unittest.TestCase):
     def setUp(self):
         self.xml_tree = etree.parse(LIFT_GOOD).getroot().find('.//pronunciation')  # noqa: E501
-        self.obj = lexicon.Phonetic(self.xml_tree)
+        self.obj = lexicon.Phonetic(xml_tree=self.xml_tree)
 
     def test_attribs(self):
         pass  # no attributes
 
     def test_elems(self):
         required = [p.name for p in self.obj.props.elements if p.required]
         test_elems(self, self.obj, required)
         optional = [p.name for p in self.obj.props.elements if not p.required]
+        optional.remove('span_items')
         test_elems(self, self.obj, optional)
 
 
 class TestRelation(unittest.TestCase):
     def setUp(self):
         self.xml_tree = etree.parse(LIFT_GOOD).getroot().find('.//relation')
-        self.obj = lexicon.Relation(self.xml_tree)
+        self.obj = lexicon.Relation(xml_tree=self.xml_tree)
 
     def test_attribs(self):
         required = [p.name for p in self.obj.props.attributes if p.required]
         test_attribs(self, self.obj, required)
         optional = [p.name for p in self.obj.props.attributes if not p.required]  # noqa: E501
         test_attribs(self, self.obj, optional)
 
@@ -150,33 +152,34 @@
         optional = [p.name for p in self.obj.props.elements if not p.required]
         test_elems(self, self.obj, optional)
 
 
 class TestReversal(unittest.TestCase):
     def setUp(self):
         self.xml_tree = etree.parse(LIFT_GOOD).getroot().find('.//reversal')
-        self.obj = lexicon.Reversal(self.xml_tree)
+        self.obj = lexicon.Reversal(xml_tree=self.xml_tree)
 
     def test_attribs(self):
         required = [p.name for p in self.obj.props.attributes if p.required]
         test_attribs(self, self.obj, required)
         optional = [p.name for p in self.obj.props.attributes if not p.required]  # noqa: E501
         test_attribs(self, self.obj, optional)
 
     def test_elems(self):
         required = [p.name for p in self.obj.props.elements if p.required]
         test_elems(self, self.obj, required)
         optional = [p.name for p in self.obj.props.elements if not p.required]
+        optional.remove('span_items')
         test_elems(self, self.obj, optional)
 
 
 class TestSense(unittest.TestCase):
     def setUp(self):
         self.xml_tree = etree.parse(LIFT_GOOD).getroot().find('.//sense')
-        self.obj = lexicon.Sense(self.xml_tree)
+        self.obj = lexicon.Sense(xml_tree=self.xml_tree)
 
     def test_attribs(self):
         required = [p.name for p in self.obj.props.attributes if p.required]
         test_attribs(self, self.obj, required)
         optional = [p.name for p in self.obj.props.attributes if not p.required]  # noqa: E501
         test_attribs(self, self.obj, optional)
 
@@ -186,35 +189,36 @@
         optional = [p.name for p in self.obj.props.elements if not p.required]
         test_elems(self, self.obj, optional)
 
 
 class TestTranslation(unittest.TestCase):
     def setUp(self):
         self.xml_tree = etree.parse(LIFT_GOOD).getroot().find('.//translation')
-        self.obj = lexicon.Translation(self.xml_tree)
+        self.obj = lexicon.Translation(xml_tree=self.xml_tree)
 
     def test_attribs(self):
         required = [p.name for p in self.obj.props.attributes if p.required]
         test_attribs(self, self.obj, required)
         optional = [p.name for p in self.obj.props.attributes if not p.required]  # noqa: E501
         test_attribs(self, self.obj, optional)
 
     def test_elems(self):
         pass  # no elements
 
 
 class TestVariant(unittest.TestCase):
     def setUp(self):
         self.xml_tree = etree.parse(LIFT_GOOD).getroot().find('.//variant')
-        self.obj = lexicon.Variant(self.xml_tree)
+        self.obj = lexicon.Variant(xml_tree=self.xml_tree)
 
     def test_attribs(self):
         required = [p.name for p in self.obj.props.attributes if p.required]
         test_attribs(self, self.obj, required)
         optional = [p.name for p in self.obj.props.attributes if not p.required]  # noqa: E501
         test_attribs(self, self.obj, optional)
 
     def test_elems(self):
         required = [p.name for p in self.obj.props.elements if p.required]
         test_elems(self, self.obj, required)
         optional = [p.name for p in self.obj.props.elements if not p.required]
+        optional.remove('span_items')
         test_elems(self, self.obj, optional)
```

