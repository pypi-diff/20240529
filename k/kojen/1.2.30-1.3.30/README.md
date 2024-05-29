# Comparing `tmp/kojen-1.2.30.tar.gz` & `tmp/kojen-1.3.30.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "kojen-1.2.30.tar", last modified: Sun Apr  9 13:23:09 2023, max compression
+gzip compressed data, was "kojen-1.3.30.tar", last modified: Wed May 29 10:54:23 2024, max compression
```

## Comparing `kojen-1.2.30.tar` & `kojen-1.3.30.tar`

### file list

```diff
@@ -1,36 +1,38 @@
-drwxrwxrwx   0        0        0        0 2023-04-09 13:23:09.068413 kojen-1.2.30/
--rw-rw-rw-   0        0        0    20890 2023-04-09 13:23:09.068413 kojen-1.2.30/PKG-INFO
-drwxrwxrwx   0        0        0        0 2023-04-09 13:23:09.028377 kojen-1.2.30/kojen/
--rw-rw-rw-   0        0        0     6200 2023-04-09 13:22:41.000000 kojen-1.2.30/kojen/Generate.py
--rw-rw-rw-   0        0        0    14933 2023-04-09 13:11:19.000000 kojen-1.2.30/kojen/Language.py
--rw-rw-rw-   0        0        0    44063 2023-04-09 13:11:19.000000 kojen-1.2.30/kojen/LanguageCPP.py
--rw-rw-rw-   0        0        0    45191 2023-04-09 13:11:19.000000 kojen-1.2.30/kojen/LanguageCsharp.py
--rw-rw-rw-   0        0        0    10159 2023-04-09 13:11:19.000000 kojen-1.2.30/kojen/LanguagePython.py
--rw-rw-rw-   0        0        0      357 2022-07-17 15:56:39.000000 kojen-1.2.30/kojen/__init__.py
--rw-rw-rw-   0        0        0       26 2022-07-17 15:56:39.000000 kojen-1.2.30/kojen/__main__.py
--rw-rw-rw-   0        0        0    27220 2023-04-09 13:22:41.000000 kojen-1.2.30/kojen/cgen.py
--rw-rw-rw-   0        0        0    10071 2023-03-25 18:25:48.000000 kojen-1.2.30/kojen/coggen.py
--rw-rw-rw-   0        0        0    17170 2023-04-09 13:22:41.000000 kojen-1.2.30/kojen/kojentypes.py
--rw-rw-rw-   0        0        0     3169 2023-03-25 18:25:48.000000 kojen-1.2.30/kojen/plant.py
--rw-rw-rw-   0        0        0     9902 2022-08-08 16:04:22.000000 kojen-1.2.30/kojen/preservative.py
--rw-rw-rw-   0        0        0     7048 2023-03-25 18:25:48.000000 kojen-1.2.30/kojen/protogen.py
--rw-rw-rw-   0        0        0    48690 2023-04-09 13:22:41.000000 kojen-1.2.30/kojen/smgen.py
--rw-rw-rw-   0        0        0     4127 2022-07-17 15:56:39.000000 kojen-1.2.30/kojen/smvppxml.py
-drwxrwxrwx   0        0        0        0 2023-04-09 13:23:09.067413 kojen-1.2.30/kojen/test/
--rw-rw-rw-   0        0        0        0 2022-07-17 15:56:39.000000 kojen-1.2.30/kojen/test/__init__.py
--rw-rw-rw-   0        0        0    12569 2023-04-09 13:22:41.000000 kojen-1.2.30/kojen/test/cgen_test.py
--rw-rw-rw-   0        0        0    10621 2022-08-08 16:04:22.000000 kojen-1.2.30/kojen/test/preservative_test.py
--rw-rw-rw-   0        0        0    18069 2023-04-09 13:22:41.000000 kojen-1.2.30/kojen/test/smgen_test.py
--rw-rw-rw-   0        0        0    15390 2022-07-17 15:56:39.000000 kojen-1.2.30/kojen/test/vppclassdiagram_test.py
--rw-rw-rw-   0        0        0     3782 2022-07-17 15:56:39.000000 kojen-1.2.30/kojen/test/vppfs_test.py
--rw-rw-rw-   0        0        0    24276 2023-04-09 13:11:19.000000 kojen-1.2.30/kojen/umlgen.py
--rw-rw-rw-   0        0        0    49539 2023-04-09 13:11:19.000000 kojen-1.2.30/kojen/vppclassdiagram.py
--rw-rw-rw-   0        0        0    35625 2022-12-09 07:45:22.000000 kojen-1.2.30/kojen/vppfs.py
-drwxrwxrwx   0        0        0        0 2023-04-09 13:23:09.050386 kojen-1.2.30/kojen.egg-info/
--rw-rw-rw-   0        0        0    20890 2023-04-09 13:23:08.000000 kojen-1.2.30/kojen.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      651 2023-04-09 13:23:08.000000 kojen-1.2.30/kojen.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-04-09 13:23:08.000000 kojen-1.2.30/kojen.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       14 2023-04-09 13:23:08.000000 kojen-1.2.30/kojen.egg-info/requires.txt
--rw-rw-rw-   0        0        0        6 2023-04-09 13:23:08.000000 kojen-1.2.30/kojen.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2023-04-09 13:23:09.069413 kojen-1.2.30/setup.cfg
--rw-rw-rw-   0        0        0     1599 2023-04-09 13:22:41.000000 kojen-1.2.30/setup.py
+drwxrwxrwx   0        0        0        0 2024-05-29 10:54:23.459716 kojen-1.3.30/
+-rw-rw-rw-   0        0        0    20890 2024-05-29 10:54:23.459716 kojen-1.3.30/PKG-INFO
+drwxrwxrwx   0        0        0        0 2024-05-29 10:54:23.343923 kojen-1.3.30/kojen/
+-rw-rw-rw-   0        0        0     7614 2024-05-29 10:53:49.000000 kojen-1.3.30/kojen/Generate.py
+-rw-rw-rw-   0        0        0     3025 2024-05-29 10:53:49.000000 kojen-1.3.30/kojen/Install.py
+-rw-rw-rw-   0        0        0    14933 2024-05-29 10:53:46.000000 kojen-1.3.30/kojen/Language.py
+-rw-rw-rw-   0        0        0    44063 2024-05-29 10:53:46.000000 kojen-1.3.30/kojen/LanguageCPP.py
+-rw-rw-rw-   0        0        0    45191 2024-05-29 10:53:46.000000 kojen-1.3.30/kojen/LanguageCsharp.py
+-rw-rw-rw-   0        0        0    10159 2024-05-29 10:53:46.000000 kojen-1.3.30/kojen/LanguagePython.py
+-rw-rw-rw-   0        0        0      357 2022-07-17 15:56:39.000000 kojen-1.3.30/kojen/__init__.py
+-rw-rw-rw-   0        0        0       26 2022-07-17 15:56:39.000000 kojen-1.3.30/kojen/__main__.py
+-rw-rw-rw-   0        0        0    27204 2024-05-29 10:53:49.000000 kojen-1.3.30/kojen/cgen.py
+-rw-rw-rw-   0        0        0    10071 2023-03-25 18:25:48.000000 kojen-1.3.30/kojen/coggen.py
+-rw-rw-rw-   0        0        0    17170 2023-04-09 13:23:40.000000 kojen-1.3.30/kojen/kojentypes.py
+-rw-rw-rw-   0        0        0     3169 2023-03-25 18:25:48.000000 kojen-1.3.30/kojen/plant.py
+-rw-rw-rw-   0        0        0     9902 2022-08-08 16:04:22.000000 kojen-1.3.30/kojen/preservative.py
+-rw-rw-rw-   0        0        0     7048 2023-03-25 18:25:48.000000 kojen-1.3.30/kojen/protogen.py
+-rw-rw-rw-   0        0        0    48690 2023-04-09 13:23:40.000000 kojen-1.3.30/kojen/smgen.py
+-rw-rw-rw-   0        0        0     4127 2022-07-17 15:56:39.000000 kojen-1.3.30/kojen/smvppxml.py
+drwxrwxrwx   0        0        0        0 2024-05-29 10:54:23.458701 kojen-1.3.30/kojen/test/
+-rw-rw-rw-   0        0        0        0 2022-07-17 15:56:39.000000 kojen-1.3.30/kojen/test/__init__.py
+-rw-rw-rw-   0        0        0    12569 2023-04-09 13:23:40.000000 kojen-1.3.30/kojen/test/cgen_test.py
+-rw-rw-rw-   0        0        0     2897 2024-05-29 10:53:49.000000 kojen-1.3.30/kojen/test/install_test.py
+-rw-rw-rw-   0        0        0    10621 2022-08-08 16:04:22.000000 kojen-1.3.30/kojen/test/preservative_test.py
+-rw-rw-rw-   0        0        0    18069 2023-04-09 13:23:40.000000 kojen-1.3.30/kojen/test/smgen_test.py
+-rw-rw-rw-   0        0        0    15390 2022-07-17 15:56:39.000000 kojen-1.3.30/kojen/test/vppclassdiagram_test.py
+-rw-rw-rw-   0        0        0     3782 2022-07-17 15:56:39.000000 kojen-1.3.30/kojen/test/vppfs_test.py
+-rw-rw-rw-   0        0        0    24276 2024-05-29 10:53:46.000000 kojen-1.3.30/kojen/umlgen.py
+-rw-rw-rw-   0        0        0    49539 2024-05-29 10:53:46.000000 kojen-1.3.30/kojen/vppclassdiagram.py
+-rw-rw-rw-   0        0        0    35625 2022-12-09 07:45:22.000000 kojen-1.3.30/kojen/vppfs.py
+drwxrwxrwx   0        0        0        0 2024-05-29 10:54:23.366785 kojen-1.3.30/kojen.egg-info/
+-rw-rw-rw-   0        0        0    20890 2024-05-29 10:54:22.000000 kojen-1.3.30/kojen.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      695 2024-05-29 10:54:22.000000 kojen-1.3.30/kojen.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-05-29 10:54:22.000000 kojen-1.3.30/kojen.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       14 2024-05-29 10:54:22.000000 kojen-1.3.30/kojen.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        6 2024-05-29 10:54:22.000000 kojen-1.3.30/kojen.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2024-05-29 10:54:23.459716 kojen-1.3.30/setup.cfg
+-rw-rw-rw-   0        0        0     1589 2024-05-29 10:53:49.000000 kojen-1.3.30/setup.py
```

### Comparing `kojen-1.2.30/PKG-INFO` & `kojen-1.3.30/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: kojen
-Version: 1.2.30
+Version: 1.3.30
 Summary: Code generation tools.
 Home-page: https://github.com/kohjaen/kojen
 Author: kohjaen
 Author-email: koh.jaen@yahoo.de
 License: UNKNOWN
 Description: ![CI](https://github.com/kohjaen/kojen/workflows/CI/badge.svg)
```

### Comparing `kojen-1.2.30/kojen/Generate.py` & `kojen-1.3.30/kojen/Generate.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,23 +1,27 @@
 #!/usr/bin/env python3
 try:
-    from . import protogen, smgen, umlgen, coggen, vppfs, LanguageCPP, LanguageCsharp, LanguagePython, cgen
+    from . import protogen, smgen, umlgen, coggen, vppfs, LanguageCPP, LanguageCsharp, LanguagePython, cgen, Install
 except:
-    import protogen, smgen, umlgen, coggen, vppfs, LanguageCPP, LanguageCsharp, LanguagePython, cgen
+    import protogen, smgen, umlgen, coggen, vppfs, LanguageCPP, LanguageCsharp, LanguagePython, cgen, Install
 
 import os
 
-''' Generate Entry function for Protocols. 
+''' Generate Entry function for Protocols.
 '''
 
 
 #def Protocol(output_dir, pythoninterfacegeneratorfilename, namespacename, classname, declspec="", author = "", group="", brief="", template_dir="") -> list:
 #    return protogen.Generate(output_dir, pythoninterfacegeneratorfilename, namespacename, classname, declspec, author, group, brief, template_dir)
 
 def Protocol(outputdir, eventsinterface, namespacenname, classname, dclspc="", author="", group="", brief="", templatedir="", __internal="", __copy_other_files=True) -> list:
+    if not os.path.isabs(templatedir):
+        # Is it a user template?
+        if Install.ContainsTemplates(templatedir):
+            templatedir = os.path.join(Install.getUserTemplateRoot(), os.path.normpath(templatedir))
     if not templatedir.strip():
         templatedir = os.path.join(os.path.join(os.path.abspath(os.path.dirname(__file__)), "protocol_templates"), "CPP")
     res =  StateMachine(outputdir, [], eventsinterface, namespacenname, classname, dclspc, author, group, brief, templatedir, __internal, False)
     if __copy_other_files:
         protogen.CopyFrameworkFiles_CPP(outputdir)
     return res
 
@@ -25,74 +29,99 @@
 
 
 ''' Generate Entry function for State Machines
 '''
 
 
 def StateMachine(outputdir, transition_table, eventsinterface, namespacenname, statemachinenameprefix, dclspc="", author="", group="", brief="", templatedir="", __internal="", __copy_other_files=True) -> list:
+    if not os.path.isabs(templatedir):
+        # Is it a user template?
+        if Install.ContainsTemplates(templatedir):
+            templatedir = os.path.join(Install.getUserTemplateRoot(), os.path.normpath(templatedir))
+
     if not templatedir.strip():
         templatedir = os.path.join(os.path.abspath(os.path.dirname(__file__)), "statemachine_templates_embedded_arm")
 
     if not os.path.isdir(templatedir) and not os.path.isfile(templatedir):
-        print("Error : dir '" + templatedir + "' does not exist. Aborting.")
+        print("Error : path '" + templatedir + "' does not exist. Aborting.")
         return
 
     language = LanguageCPP.LanguageCPP()
     smgenerator = smgen.CStateMachineGenerator(templatedir, outputdir, eventsinterface, language, author, group, brief)
     if not __internal:
         smgenerator.vpp_filename = "Transition Table"
     else:
         smgenerator.vpp_filename = __internal
     return smgenerator.Generate(transition_table, namespacenname, statemachinenameprefix, dclspc, __copy_other_files)
 
 
 def StateMachine_CSHARP(outputdir, transition_table, eventsinterface, namespacenname, statemachinenameprefix, dclspc="", author="", group="", brief="", templatedir="", __internal="", __copy_other_files=True) -> list:
+    if not os.path.isabs(templatedir):
+        # Is it a user template?
+        if Install.ContainsTemplates(templatedir):
+            templatedir = os.path.join(Install.getUserTemplateRoot(), os.path.normpath(templatedir))
+
     if not templatedir.strip():
         templatedir = os.path.join(os.path.abspath(os.path.dirname(__file__)), "statemachine_templates_cs_winlinmac")
 
     if not os.path.isdir(templatedir) and not os.path.isfile(templatedir):
-        print("Error : dir '" + templatedir + "' does not exist. Aborting.")
+        print("Error : path '" + templatedir + "' does not exist. Aborting.")
         return []
 
     language = LanguageCsharp.LanguageCsharp()
     smgenerator = smgen.CStateMachineGenerator(templatedir, outputdir, eventsinterface, language, author, group, brief)
     if not __internal:
         smgenerator.vpp_filename = "Transition Table"
     else:
         smgenerator.vpp_filename = __internal
     return smgenerator.Generate(transition_table, namespacenname, statemachinenameprefix, dclspc, __copy_other_files)
 
 
 def StateMachine_PYTHON(outputdir, transition_table, eventsinterface, namespacenname, statemachinenameprefix, dclspc="", author="", group="", brief="", templatedir="", __internal="", __copy_other_files=True) -> list:
+    if not os.path.isabs(templatedir):
+        # Is it a user template?
+        if Install.ContainsTemplates(templatedir):
+            templatedir = os.path.join(Install.getUserTemplateRoot(), os.path.normpath(templatedir))
+
     if not templatedir.strip():
         templatedir = os.path.join(os.path.abspath(os.path.dirname(__file__)), "statemachine_templates_py")
 
     if not os.path.isdir(templatedir) and not os.path.isfile(templatedir):
-        print("Error : dir '" + templatedir + "' does not exist. Aborting.")
+        print("Error : path '" + templatedir + "' does not exist. Aborting.")
         return []
 
     language = LanguagePython.LanguagePython()
     smgenerator = smgen.CStateMachineGenerator(templatedir, outputdir, eventsinterface, language, author, group, brief)
     if not __internal:
         smgenerator.vpp_filename = "Transition Table"
     else:
         smgenerator.vpp_filename = __internal
     return smgenerator.Generate(transition_table, namespacenname, statemachinenameprefix, dclspc, __copy_other_files)
 
 
 def StateMachineFromModel(outputdir, vp_project_path, vp_statemachinename, eventsinterface, namespacenname, statemachinenameprefix, dclspc="", author="", group="", brief="", templatedir="", __copy_other_files=True) -> list:
+    if not os.path.isabs(templatedir):
+        # Is it a user template?
+        if Install.ContainsTemplates(templatedir):
+            templatedir = os.path.join(Install.getUserTemplateRoot(), os.path.normpath(templatedir))
+
     transition_table = vppfs.ExtractTransitionTable(vp_statemachinename, vp_project_path)
     return StateMachine(outputdir, transition_table, eventsinterface, namespacenname, statemachinenameprefix, dclspc, author, group, brief, templatedir, os.path.basename(vp_project_path),__copy_other_files)
 
 
 ''' Generate Entry function for Class Diagrams
 '''
 
 
 def UML(outputdir, vp_project_path, vp_classdiagramname, dclspc="", author="", group="", brief="", namespace_to_folders=False, templatefiledir="") -> list:
+    if not os.path.isabs(templatefiledir):
+        # Is it a user template?
+        if Install.ContainsTemplates(templatefiledir):
+            templatefiledir = os.path.join(Install.getUserTemplateRoot(), os.path.normpath(templatefiledir))
+
     language = LanguageCPP.LanguageCPP()
     return umlgen.Generate(vp_project_path, vp_classdiagramname, outputdir, language, author, group, brief, namespace_to_folders, dclspc, templatefiledir)
 
 def UML_CSHARP(outputdir, vp_project_path, vp_classdiagramname, dclspc="", author="", group="", brief="", namespace_to_folders=False, templatefiledir="") -> list:
     language = LanguageCsharp.LanguageCsharp()
     return umlgen.Generate(vp_project_path, vp_classdiagramname, outputdir, language, author, group, brief, namespace_to_folders, dclspc, templatefiledir)
```

### Comparing `kojen-1.2.30/kojen/Language.py` & `kojen-1.3.30/kojen/Language.py`

 * *Files identical despite different names*

### Comparing `kojen-1.2.30/kojen/LanguageCPP.py` & `kojen-1.3.30/kojen/LanguageCPP.py`

 * *Files identical despite different names*

### Comparing `kojen-1.2.30/kojen/LanguageCsharp.py` & `kojen-1.3.30/kojen/LanguageCsharp.py`

 * *Files identical despite different names*

### Comparing `kojen-1.2.30/kojen/LanguagePython.py` & `kojen-1.3.30/kojen/LanguagePython.py`

 * *Files identical despite different names*

### Comparing `kojen-1.2.30/kojen/cgen.py` & `kojen-1.3.30/kojen/cgen.py`

 * *Files 0% similar despite different names*

```diff
@@ -41,15 +41,15 @@
 
 '''
 
 ''' This forms the base for some sorts of code generation.
 
     Step 1) Load template files to memory
     Step 2) Search and replace passed-in tags in memory (including filenames).
-    
+
 '''
 
 __TAG_DATETIME__           = '<<<DATETIME>>>'
 __TAG_PLATFORM__           = '<<<PLATFORM>>>'
 __TAG_EXTENDS__            = '<<<EXTENDS>>>'
 __TAG_EXCLUDE__            = '<<<EXCLUDE>>>'
 __TAG_FOR_BEGIN__          = "<<<FOR_BEGIN>>>"
@@ -601,17 +601,17 @@
     """
     try:
         os.makedirs(dir_to, exist_ok=True)
         for filename in list_of_filenames:
             try:
                 shutil.copy(os.path.join(dir_from, filename), os.path.join(dir_to, filename))
             except OSError:
-                warnings.warn("Copy of the file %s failed" % os.path.join(dir_from, filename))
+                warning("Copy of the file %s failed" % os.path.join(dir_from, filename))
     except OSError:
-        warnings.warn("Creation of the directory %s failed" % dir_to)
+        warning("Creation of the directory %s failed" % dir_to)
 
 def FilePreservationSyncUtil(file_from, file_to) -> None:
     """
     Will synchronize code in preservation tags from 'file_from' to 'file_to',
     if these tags exist in 'file_to'.
 
     Tags that exist exclusively in 'file_to' will remain untouched if they do not
```

### Comparing `kojen-1.2.30/kojen/coggen.py` & `kojen-1.3.30/kojen/coggen.py`

 * *Files identical despite different names*

### Comparing `kojen-1.2.30/kojen/kojentypes.py` & `kojen-1.3.30/kojen/kojentypes.py`

 * *Files identical despite different names*

### Comparing `kojen-1.2.30/kojen/plant.py` & `kojen-1.3.30/kojen/plant.py`

 * *Files identical despite different names*

### Comparing `kojen-1.2.30/kojen/preservative.py` & `kojen-1.3.30/kojen/preservative.py`

 * *Files identical despite different names*

### Comparing `kojen-1.2.30/kojen/protogen.py` & `kojen-1.3.30/kojen/protogen.py`

 * *Files identical despite different names*

### Comparing `kojen-1.2.30/kojen/smgen.py` & `kojen-1.3.30/kojen/smgen.py`

 * *Files identical despite different names*

### Comparing `kojen-1.2.30/kojen/smvppxml.py` & `kojen-1.3.30/kojen/smvppxml.py`

 * *Files identical despite different names*

### Comparing `kojen-1.2.30/kojen/test/cgen_test.py` & `kojen-1.3.30/kojen/test/cgen_test.py`

 * *Files identical despite different names*

### Comparing `kojen-1.2.30/kojen/test/preservative_test.py` & `kojen-1.3.30/kojen/test/preservative_test.py`

 * *Files identical despite different names*

### Comparing `kojen-1.2.30/kojen/test/smgen_test.py` & `kojen-1.3.30/kojen/test/smgen_test.py`

 * *Files identical despite different names*

### Comparing `kojen-1.2.30/kojen/test/vppclassdiagram_test.py` & `kojen-1.3.30/kojen/test/vppclassdiagram_test.py`

 * *Files identical despite different names*

### Comparing `kojen-1.2.30/kojen/test/vppfs_test.py` & `kojen-1.3.30/kojen/test/vppfs_test.py`

 * *Files identical despite different names*

### Comparing `kojen-1.2.30/kojen/umlgen.py` & `kojen-1.3.30/kojen/umlgen.py`

 * *Files identical despite different names*

### Comparing `kojen-1.2.30/kojen/vppclassdiagram.py` & `kojen-1.3.30/kojen/vppclassdiagram.py`

 * *Files identical despite different names*

### Comparing `kojen-1.2.30/kojen/vppfs.py` & `kojen-1.3.30/kojen/vppfs.py`

 * *Files identical despite different names*

### Comparing `kojen-1.2.30/kojen.egg-info/PKG-INFO` & `kojen-1.3.30/kojen.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: kojen
-Version: 1.2.30
+Version: 1.3.30
 Summary: Code generation tools.
 Home-page: https://github.com/kohjaen/kojen
 Author: kohjaen
 Author-email: koh.jaen@yahoo.de
 License: UNKNOWN
 Description: ![CI](https://github.com/kohjaen/kojen/workflows/CI/badge.svg)
```

### Comparing `kojen-1.2.30/kojen.egg-info/SOURCES.txt` & `kojen-1.3.30/kojen.egg-info/SOURCES.txt`

 * *Files 12% similar despite different names*

```diff
@@ -1,9 +1,10 @@
 setup.py
 kojen/Generate.py
+kojen/Install.py
 kojen/Language.py
 kojen/LanguageCPP.py
 kojen/LanguageCsharp.py
 kojen/LanguagePython.py
 kojen/__init__.py
 kojen/__main__.py
 kojen/cgen.py
@@ -20,11 +21,12 @@
 kojen.egg-info/PKG-INFO
 kojen.egg-info/SOURCES.txt
 kojen.egg-info/dependency_links.txt
 kojen.egg-info/requires.txt
 kojen.egg-info/top_level.txt
 kojen/test/__init__.py
 kojen/test/cgen_test.py
+kojen/test/install_test.py
 kojen/test/preservative_test.py
 kojen/test/smgen_test.py
 kojen/test/vppclassdiagram_test.py
 kojen/test/vppfs_test.py
```

### Comparing `kojen-1.2.30/setup.py` & `kojen-1.3.30/setup.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,39 +1,39 @@
 import setuptools
 
 with open("README.MD", "r") as fh:
     long_description = fh.read()
 
 setuptools.setup(
     name="kojen",
-    version="1.2.30",
+    version="1.3.30",
     author="kohjaen",
     author_email="koh.jaen@yahoo.de",
     description="Code generation tools.",
     long_description=long_description,
     long_description_content_type="text/markdown",
     url="https://github.com/kohjaen/kojen",
     packages=setuptools.find_packages(),
     classifiers=[
         "Programming Language :: Python :: 3",
         "License :: OSI Approved :: MIT License",
         "Operating System :: OS Independent",
     ],
     python_requires='>=3.6.8',
-	package_data={'': ['allplatforms/CPP/*.*', 
-                       'allplatforms/CPP/sml/include/boost/*.*', 
-                       'allplatforms/CPP/testsuite/*.*', 
-                       'allplatforms/CPP/testsuite/minunit/minunit.h', 
-                       'allplatforms/CPP/testsuite/minunit/minunit.cpp', 
-                       'classdiagram_templates/C#/*.*', 
-                       'classdiagram_templates/CPP/*.*', 
-                       'protocol_templates/CPP/*.*', 
+	package_data={'': ['allplatforms/CPP/*.*',
+                       'allplatforms/CPP/sml/include/boost/*.*',
+                       'allplatforms/CPP/testsuite/*.*',
+                       'allplatforms/CPP/testsuite/minunit/minunit.h',
+                       'allplatforms/CPP/testsuite/minunit/minunit.cpp',
+                       'classdiagram_templates/C#/*.*',
+                       'classdiagram_templates/CPP/*.*',
+                       'protocol_templates/CPP/*.*',
                        'protocol_templates/PY/*.*',
                        'statemachine_templates_cs_winlinmac/*.*',
                        'statemachine_templates_embedded_arm/*.*',
                        'statemachine_templates_py/*.*',
-                       'statemachine_templates_pc_boost/*.*', 
-                       'docs/images/*.*', 
+                       'statemachine_templates_pc_boost/*.*',
+                       'docs/images/*.*',
                        'docs/*.*']},
 	include_package_data=True,
     install_requires=['cogapp>=3.0.0',],
 )
```

