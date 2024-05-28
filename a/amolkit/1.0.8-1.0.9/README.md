# Comparing `tmp/amolkit-1.0.8.tar.gz` & `tmp/amolkit-1.0.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "amolkit-1.0.8.tar", last modified: Mon May 27 23:48:13 2024, max compression
+gzip compressed data, was "amolkit-1.0.9.tar", last modified: Tue May 28 01:17:51 2024, max compression
```

## Comparing `amolkit-1.0.8.tar` & `amolkit-1.0.9.tar`

### file list

```diff
@@ -1,29 +1,29 @@
-drwxr-xr-x   0 anmol     (1000) anmol     (1000)        0 2024-05-27 23:48:13.593177 amolkit-1.0.8/
--rw-r--r--   0 anmol     (1000) anmol     (1000)     1498 2023-06-06 15:10:15.000000 amolkit-1.0.8/LICENSE
--rw-r--r--   0 anmol     (1000) anmol     (1000)      336 2024-05-27 23:48:13.593177 amolkit-1.0.8/PKG-INFO
--rw-r--r--   0 anmol     (1000) anmol     (1000)       56 2023-06-06 15:10:15.000000 amolkit-1.0.8/README.md
-drwxr-xr-x   0 anmol     (1000) anmol     (1000)        0 2024-05-27 23:48:13.583177 amolkit-1.0.8/amolkit/
--rw-r--r--   0 anmol     (1000) anmol     (1000)    32064 2023-08-07 19:56:30.000000 amolkit-1.0.8/amolkit/EleInfo.py
--rw-r--r--   0 anmol     (1000) anmol     (1000)        0 2023-06-06 15:27:54.000000 amolkit-1.0.8/amolkit/__init__.py
--rw-r--r--   0 anmol     (1000) anmol     (1000)    12188 2023-08-19 01:44:09.000000 amolkit-1.0.8/amolkit/amolsystem.py
--rw-r--r--   0 anmol     (1000) anmol     (1000)     3948 2024-05-06 05:25:28.000000 amolkit-1.0.8/amolkit/atom.py
--rw-r--r--   0 anmol     (1000) anmol     (1000)     9095 2024-04-03 21:28:54.000000 amolkit-1.0.8/amolkit/genic.py
--rw-r--r--   0 anmol     (1000) anmol     (1000)     2713 2024-05-14 21:06:09.000000 amolkit-1.0.8/amolkit/getEleInfo.py
--rw-r--r--   0 anmol     (1000) anmol     (1000)     2620 2024-04-06 23:08:42.000000 amolkit-1.0.8/amolkit/gethybridstate.py
--rw-r--r--   0 anmol     (1000) anmol     (1000)     3032 2024-04-03 21:28:42.000000 amolkit-1.0.8/amolkit/getring.py
--rw-r--r--   0 anmol     (1000) anmol     (1000)      328 2024-05-15 19:45:36.000000 amolkit-1.0.8/amolkit/misc.py
--rw-r--r--   0 anmol     (1000) anmol     (1000)    23122 2024-05-14 21:04:52.000000 amolkit-1.0.8/amolkit/molecule.py
--rw-r--r--   0 anmol     (1000) anmol     (1000)    24779 2024-05-14 21:01:09.000000 amolkit-1.0.8/amolkit/molecule2.py
--rw-r--r--   0 anmol     (1000) anmol     (1000)     8261 2023-08-10 20:42:44.000000 amolkit-1.0.8/amolkit/moltransform.py
--rw-r--r--   0 anmol     (1000) anmol     (1000)     8967 2023-08-19 01:39:50.000000 amolkit-1.0.8/amolkit/parameter.py
--rw-r--r--   0 anmol     (1000) anmol     (1000)    21118 2023-08-16 19:41:35.000000 amolkit-1.0.8/amolkit/psf.py
--rw-r--r--   0 anmol     (1000) anmol     (1000)     3803 2024-05-27 22:16:52.000000 amolkit-1.0.8/amolkit/stringmanip.py
--rw-r--r--   0 anmol     (1000) anmol     (1000)    23985 2024-05-27 23:45:36.000000 amolkit-1.0.8/amolkit/topology.py
-drwxr-xr-x   0 anmol     (1000) anmol     (1000)        0 2024-05-27 23:48:13.593177 amolkit-1.0.8/amolkit.egg-info/
--rw-r--r--   0 anmol     (1000) anmol     (1000)      336 2024-05-27 23:48:13.000000 amolkit-1.0.8/amolkit.egg-info/PKG-INFO
--rw-r--r--   0 anmol     (1000) anmol     (1000)      501 2024-05-27 23:48:13.000000 amolkit-1.0.8/amolkit.egg-info/SOURCES.txt
--rw-r--r--   0 anmol     (1000) anmol     (1000)        1 2024-05-27 23:48:13.000000 amolkit-1.0.8/amolkit.egg-info/dependency_links.txt
--rw-r--r--   0 anmol     (1000) anmol     (1000)        1 2023-06-06 15:29:08.000000 amolkit-1.0.8/amolkit.egg-info/not-zip-safe
--rw-r--r--   0 anmol     (1000) anmol     (1000)        8 2024-05-27 23:48:13.000000 amolkit-1.0.8/amolkit.egg-info/top_level.txt
--rw-r--r--   0 anmol     (1000) anmol     (1000)       38 2024-05-27 23:48:13.593177 amolkit-1.0.8/setup.cfg
--rw-r--r--   0 anmol     (1000) anmol     (1000)      902 2024-05-27 23:48:07.000000 amolkit-1.0.8/setup.py
+drwxr-xr-x   0 anmol     (1000) anmol     (1000)        0 2024-05-28 01:17:51.008775 amolkit-1.0.9/
+-rw-r--r--   0 anmol     (1000) anmol     (1000)     1498 2023-06-06 15:10:15.000000 amolkit-1.0.9/LICENSE
+-rw-r--r--   0 anmol     (1000) anmol     (1000)      336 2024-05-28 01:17:51.008775 amolkit-1.0.9/PKG-INFO
+-rw-r--r--   0 anmol     (1000) anmol     (1000)       56 2023-06-06 15:10:15.000000 amolkit-1.0.9/README.md
+drwxr-xr-x   0 anmol     (1000) anmol     (1000)        0 2024-05-28 01:17:51.008775 amolkit-1.0.9/amolkit/
+-rw-r--r--   0 anmol     (1000) anmol     (1000)    32064 2023-08-07 19:56:30.000000 amolkit-1.0.9/amolkit/EleInfo.py
+-rw-r--r--   0 anmol     (1000) anmol     (1000)        0 2023-06-06 15:27:54.000000 amolkit-1.0.9/amolkit/__init__.py
+-rw-r--r--   0 anmol     (1000) anmol     (1000)    12188 2023-08-19 01:44:09.000000 amolkit-1.0.9/amolkit/amolsystem.py
+-rw-r--r--   0 anmol     (1000) anmol     (1000)     3948 2024-05-06 05:25:28.000000 amolkit-1.0.9/amolkit/atom.py
+-rw-r--r--   0 anmol     (1000) anmol     (1000)     9095 2024-04-03 21:28:54.000000 amolkit-1.0.9/amolkit/genic.py
+-rw-r--r--   0 anmol     (1000) anmol     (1000)     2713 2024-05-14 21:06:09.000000 amolkit-1.0.9/amolkit/getEleInfo.py
+-rw-r--r--   0 anmol     (1000) anmol     (1000)     2620 2024-04-06 23:08:42.000000 amolkit-1.0.9/amolkit/gethybridstate.py
+-rw-r--r--   0 anmol     (1000) anmol     (1000)     3032 2024-04-03 21:28:42.000000 amolkit-1.0.9/amolkit/getring.py
+-rw-r--r--   0 anmol     (1000) anmol     (1000)      328 2024-05-15 19:45:36.000000 amolkit-1.0.9/amolkit/misc.py
+-rw-r--r--   0 anmol     (1000) anmol     (1000)    23122 2024-05-14 21:04:52.000000 amolkit-1.0.9/amolkit/molecule.py
+-rw-r--r--   0 anmol     (1000) anmol     (1000)    24779 2024-05-14 21:01:09.000000 amolkit-1.0.9/amolkit/molecule2.py
+-rw-r--r--   0 anmol     (1000) anmol     (1000)     8261 2023-08-10 20:42:44.000000 amolkit-1.0.9/amolkit/moltransform.py
+-rw-r--r--   0 anmol     (1000) anmol     (1000)     9346 2024-05-28 01:16:37.000000 amolkit-1.0.9/amolkit/parameter.py
+-rw-r--r--   0 anmol     (1000) anmol     (1000)    21118 2023-08-16 19:41:35.000000 amolkit-1.0.9/amolkit/psf.py
+-rw-r--r--   0 anmol     (1000) anmol     (1000)     3803 2024-05-27 22:16:52.000000 amolkit-1.0.9/amolkit/stringmanip.py
+-rw-r--r--   0 anmol     (1000) anmol     (1000)    23985 2024-05-27 23:45:36.000000 amolkit-1.0.9/amolkit/topology.py
+drwxr-xr-x   0 anmol     (1000) anmol     (1000)        0 2024-05-28 01:17:51.008775 amolkit-1.0.9/amolkit.egg-info/
+-rw-r--r--   0 anmol     (1000) anmol     (1000)      336 2024-05-28 01:17:50.000000 amolkit-1.0.9/amolkit.egg-info/PKG-INFO
+-rw-r--r--   0 anmol     (1000) anmol     (1000)      501 2024-05-28 01:17:50.000000 amolkit-1.0.9/amolkit.egg-info/SOURCES.txt
+-rw-r--r--   0 anmol     (1000) anmol     (1000)        1 2024-05-28 01:17:50.000000 amolkit-1.0.9/amolkit.egg-info/dependency_links.txt
+-rw-r--r--   0 anmol     (1000) anmol     (1000)        1 2023-06-06 15:29:08.000000 amolkit-1.0.9/amolkit.egg-info/not-zip-safe
+-rw-r--r--   0 anmol     (1000) anmol     (1000)        8 2024-05-28 01:17:50.000000 amolkit-1.0.9/amolkit.egg-info/top_level.txt
+-rw-r--r--   0 anmol     (1000) anmol     (1000)       38 2024-05-28 01:17:51.008775 amolkit-1.0.9/setup.cfg
+-rw-r--r--   0 anmol     (1000) anmol     (1000)      902 2024-05-28 01:16:48.000000 amolkit-1.0.9/setup.py
```

### Comparing `amolkit-1.0.8/LICENSE` & `amolkit-1.0.9/LICENSE`

 * *Files identical despite different names*

### Comparing `amolkit-1.0.8/amolkit/EleInfo.py` & `amolkit-1.0.9/amolkit/EleInfo.py`

 * *Files identical despite different names*

### Comparing `amolkit-1.0.8/amolkit/amolsystem.py` & `amolkit-1.0.9/amolkit/amolsystem.py`

 * *Files identical despite different names*

### Comparing `amolkit-1.0.8/amolkit/atom.py` & `amolkit-1.0.9/amolkit/atom.py`

 * *Files identical despite different names*

### Comparing `amolkit-1.0.8/amolkit/genic.py` & `amolkit-1.0.9/amolkit/genic.py`

 * *Files identical despite different names*

### Comparing `amolkit-1.0.8/amolkit/getEleInfo.py` & `amolkit-1.0.9/amolkit/getEleInfo.py`

 * *Files identical despite different names*

### Comparing `amolkit-1.0.8/amolkit/gethybridstate.py` & `amolkit-1.0.9/amolkit/gethybridstate.py`

 * *Files identical despite different names*

### Comparing `amolkit-1.0.8/amolkit/getring.py` & `amolkit-1.0.9/amolkit/getring.py`

 * *Files identical despite different names*

### Comparing `amolkit-1.0.8/amolkit/molecule.py` & `amolkit-1.0.9/amolkit/molecule.py`

 * *Files identical despite different names*

### Comparing `amolkit-1.0.8/amolkit/molecule2.py` & `amolkit-1.0.9/amolkit/molecule2.py`

 * *Files identical despite different names*

### Comparing `amolkit-1.0.8/amolkit/moltransform.py` & `amolkit-1.0.9/amolkit/moltransform.py`

 * *Files identical despite different names*

### Comparing `amolkit-1.0.8/amolkit/parameter.py` & `amolkit-1.0.9/amolkit/parameter.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,9 +1,10 @@
 from collections import OrderedDict
 from amolkit.stringmanip import getPenaltyfromString
+from amolkit.stringmanip import split_line
 
 def readCharmmParameter(parfile):
     """
     Get Charmm parameters from any file containing parameters.
     Arguments:
         parfile: It can be any file format containing charmm parameters in correct style.
     Returns:
@@ -160,32 +161,46 @@
 def format_diplist(dipl):
     lineA="{:<8}  {:<8}  {:<8}  {:<8} {:>10.4f}  {:>2d}  {:>10.2f}".format(dipl[0],dipl[1],dipl[2],dipl[3],dipl[4],dipl[5],dipl[6])
     lineB=" ! ".join(map(str,dipl[7:]))
     line=" ! ".join((lineA,lineB))
     return line
 
 class WriteCharmmParameter():
+    
     @staticmethod
     def par_header(header):
-        text="* %s\n* Written by: amolkit\n*\n"%(header)
+        text = ""
+        if header:
+            header=split_line(header)
+            for h in header:
+                text += "* "+ h + "\n"
+        else:
+            text="* Written by: amolkit\n"
+        text += "*\n"
         return text
     
     @staticmethod
     def par_readinstruct(append=True):
         if append:
             text= "read param card append"
         else:
             text= "read param card"
         return text
     
     @staticmethod
     def par_comment(comment):
-        text="! %s\n\n"%(comment)
-        return text 
-    
+        text = ""
+        if comment:
+            comment = split_line(comment)
+            for h in header:
+                text += "! "+ h + "\n"
+        else:
+            text="! Written by: amolkit\n"
+        return text
+
     @staticmethod
     def par_bondedparam(bondedparam):
         """
         Argument:
             param: Dictionary of parameters containing keys:: BONDS, ANGLES, DIHEDRALS, IMPROPERS
                and values can be string or list or list of list.
             Example: param["BONDS"]="AT1 AT2 KV1 DV1 ! PENALTY COMMENT"
```

### Comparing `amolkit-1.0.8/amolkit/psf.py` & `amolkit-1.0.9/amolkit/psf.py`

 * *Files identical despite different names*

### Comparing `amolkit-1.0.8/amolkit/stringmanip.py` & `amolkit-1.0.9/amolkit/stringmanip.py`

 * *Files identical despite different names*

### Comparing `amolkit-1.0.8/amolkit/topology.py` & `amolkit-1.0.9/amolkit/topology.py`

 * *Files identical despite different names*

### Comparing `amolkit-1.0.8/setup.py` & `amolkit-1.0.9/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -19,15 +19,15 @@
      with open("README.md","r") as f:
           long_description=f.read()
 except:
      long_description=""
      pass
 
 setup(name='amolkit', 
-      version='1.0.8', 
+      version='1.0.9', 
       description='Library for extracting molecule information', 
       long_description=long_description,
       url='https://github.com/anmolecule/amolkit', 
       author='Anmol Kumar', 
       author_email='anmolecule@gmail.com', 
       license='BSD 3-Clause "New" or "Revised" License',
       packages=find_packages(),
```

