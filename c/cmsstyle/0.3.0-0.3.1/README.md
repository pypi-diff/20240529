# Comparing `tmp/cmsstyle-0.3.0.tar.gz` & `tmp/cmsstyle-0.3.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, last modified: Wed Apr 17 20:59:02 2024, max compression
+gzip compressed data, last modified: Wed May 29 17:39:28 2024, max compression
```

## Comparing `cmsstyle-0.3.0.tar` & `cmsstyle-0.3.1.tar`

### file list

```diff
@@ -1,8 +1,8 @@
--rw-r--r--   0        0        0       24 2024-04-17 20:59:02.000000 cmsstyle-0.3.0/src/cmsstyle/__init__.py
--rw-r--r--   0        0        0      411 2024-04-17 20:59:02.000000 cmsstyle-0.3.0/src/cmsstyle/_version.py
--rw-r--r--   0        0        0    23845 2024-04-17 20:59:02.000000 cmsstyle-0.3.0/src/cmsstyle/cmsstyle.py
--rw-r--r--   0        0        0     1246 2024-04-17 20:59:02.000000 cmsstyle-0.3.0/.gitignore
--rw-r--r--   0        0        0     1082 2024-04-17 20:59:02.000000 cmsstyle-0.3.0/LICENSE
--rw-r--r--   0        0        0      192 2024-04-17 20:59:02.000000 cmsstyle-0.3.0/README.md
--rw-r--r--   0        0        0     1524 2024-04-17 20:59:02.000000 cmsstyle-0.3.0/pyproject.toml
--rw-r--r--   0        0        0     1446 2024-04-17 20:59:02.000000 cmsstyle-0.3.0/PKG-INFO
+-rw-r--r--   0        0        0       24 2024-05-29 17:39:28.000000 cmsstyle-0.3.1/src/cmsstyle/__init__.py
+-rw-r--r--   0        0        0      411 2024-05-29 17:39:28.000000 cmsstyle-0.3.1/src/cmsstyle/_version.py
+-rw-r--r--   0        0        0    23841 2024-05-29 17:39:28.000000 cmsstyle-0.3.1/src/cmsstyle/cmsstyle.py
+-rw-r--r--   0        0        0     1246 2024-05-29 17:39:28.000000 cmsstyle-0.3.1/.gitignore
+-rw-r--r--   0        0        0     1082 2024-05-29 17:39:28.000000 cmsstyle-0.3.1/LICENSE
+-rw-r--r--   0        0        0      192 2024-05-29 17:39:28.000000 cmsstyle-0.3.1/README.md
+-rw-r--r--   0        0        0     1524 2024-05-29 17:39:28.000000 cmsstyle-0.3.1/pyproject.toml
+-rw-r--r--   0        0        0     1446 2024-05-29 17:39:28.000000 cmsstyle-0.3.1/PKG-INFO
```

### Comparing `cmsstyle-0.3.0/src/cmsstyle/cmsstyle.py` & `cmsstyle-0.3.1/src/cmsstyle/cmsstyle.py`

 * *Files 1% similar despite different names*

```diff
@@ -2,23 +2,22 @@
 # CMS Style                            #
 # Authors: CMS, Andrea Malara          #
 ########################################
 
 import ROOT as rt
 from array import array
 
-rt.gROOT.SetBatch(rt.kTRUE)
 
 cms_lumi = "Run 2, 138 fb^{#minus1}"
 cms_energy = "13 TeV"
 
 
 def SetEnergy(energy, unit = "TeV"):
     global cms_energy
-    cms_energy = str(energy) + " " + unit
+    cms_energy = str(energy) + " " + unit if energy != "" else ""
 
 
 def SetLumi(lumi, unit="fb", round_lumi=False):
     global cms_lumi
     if lumi != "":
         cms_lumi = f"{lumi:.0f}" if round_lumi else f"{lumi}"
         cms_lumi += f" {unit}^{{#minus1}}"
```

### Comparing `cmsstyle-0.3.0/.gitignore` & `cmsstyle-0.3.1/.gitignore`

 * *Files identical despite different names*

### Comparing `cmsstyle-0.3.0/LICENSE` & `cmsstyle-0.3.1/LICENSE`

 * *Files identical despite different names*

### Comparing `cmsstyle-0.3.0/pyproject.toml` & `cmsstyle-0.3.1/pyproject.toml`

 * *Files identical despite different names*

### Comparing `cmsstyle-0.3.0/PKG-INFO` & `cmsstyle-0.3.1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.3
 Name: cmsstyle
-Version: 0.3.0
+Version: 0.3.1
 Project-URL: Homepage, https://github.com/cms-cat/cms-root-style
 Project-URL: Documentation, https://github.com/cms-cat/cms-root-style
 Project-URL: Bug Tracker, https://github.com/cms-cat/cms-root-style/issues
 Project-URL: Discussions, https://github.com/cms-cat/cms-root-style/discussions
 Author-email: Andrzej Novak <andrzej.novak@cern.ch>, Tommaso Tedeschi <tommaso.tedeschi@cern.ch>, Clemens Lange <clemens.lange@cern.ch>, Piergiulio Lenzi <piergiulio.lenzi@cern.ch>, Andrea Malara <andrea.malara@cern.ch>
 Maintainer-email: CMS CAT Group <cms-phys-conveners-CAT@cern.ch>
 License-File: LICENSE
```

