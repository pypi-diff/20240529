# Comparing `tmp/dsiunits-2.2.3.tar.gz` & `tmp/dsiunits-2.3.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dsiunits-2.2.3.tar", last modified: Thu May 16 16:54:44 2024, max compression
+gzip compressed data, was "dsiunits-2.3.0.tar", last modified: Wed May 29 08:53:49 2024, max compression
```

## Comparing `dsiunits-2.2.3.tar` & `dsiunits-2.3.0.tar`

### file list

```diff
@@ -1,17 +1,21 @@
-drwxr-xr-x   0 seeger01  (1000) seeger01  (1000)        0 2024-05-16 16:54:44.914838 dsiunits-2.2.3/
--rw-r--r--   0 seeger01  (1000) seeger01  (1000)    26516 2024-04-25 08:43:02.000000 dsiunits-2.2.3/LICENSE
--rw-r--r--   0 seeger01  (1000) seeger01  (1000)    33313 2024-05-16 16:54:44.914838 dsiunits-2.2.3/PKG-INFO
--rw-r--r--   0 seeger01  (1000) seeger01  (1000)     2033 2024-05-16 16:54:24.000000 dsiunits-2.2.3/README.md
--rw-r--r--   0 seeger01  (1000) seeger01  (1000)      764 2024-05-16 16:54:24.000000 dsiunits-2.2.3/pyproject.toml
--rw-r--r--   0 seeger01  (1000) seeger01  (1000)      447 2024-05-16 16:54:44.915838 dsiunits-2.2.3/setup.cfg
-drwxr-xr-x   0 seeger01  (1000) seeger01  (1000)        0 2024-05-16 16:54:44.914838 dsiunits-2.2.3/src/
--rw-r--r--   0 seeger01  (1000) seeger01  (1000)        0 2024-04-25 08:36:12.000000 dsiunits-2.2.3/src/__init__.py
--rw-r--r--   0 seeger01  (1000) seeger01  (1000)    43577 2024-05-16 16:54:24.000000 dsiunits-2.2.3/src/dsiUnits.py
-drwxr-xr-x   0 seeger01  (1000) seeger01  (1000)        0 2024-05-16 16:54:44.914838 dsiunits-2.2.3/src/dsiunits.egg-info/
--rw-r--r--   0 seeger01  (1000) seeger01  (1000)    33313 2024-05-16 16:54:44.000000 dsiunits-2.2.3/src/dsiunits.egg-info/PKG-INFO
--rw-r--r--   0 seeger01  (1000) seeger01  (1000)      276 2024-05-16 16:54:44.000000 dsiunits-2.2.3/src/dsiunits.egg-info/SOURCES.txt
--rw-r--r--   0 seeger01  (1000) seeger01  (1000)        1 2024-05-16 16:54:44.000000 dsiunits-2.2.3/src/dsiunits.egg-info/dependency_links.txt
--rw-r--r--   0 seeger01  (1000) seeger01  (1000)       43 2024-05-16 16:54:44.000000 dsiunits-2.2.3/src/dsiunits.egg-info/requires.txt
--rw-r--r--   0 seeger01  (1000) seeger01  (1000)       18 2024-05-16 16:54:44.000000 dsiunits-2.2.3/src/dsiunits.egg-info/top_level.txt
-drwxr-xr-x   0 seeger01  (1000) seeger01  (1000)        0 2024-05-16 16:54:44.914838 dsiunits-2.2.3/tests/
--rw-r--r--   0 seeger01  (1000) seeger01  (1000)    24345 2024-05-16 16:54:24.000000 dsiunits-2.2.3/tests/test_dsiUnits.py
+drwxr-xr-x   0 stehr     (1000) stehr     (1000)        0 2024-05-29 08:53:49.645609 dsiunits-2.3.0/
+-rw-r--r--   0 stehr     (1000) stehr     (1000)    26516 2024-05-29 08:49:18.000000 dsiunits-2.3.0/LICENSE
+-rw-r--r--   0 stehr     (1000) stehr     (1000)    33313 2024-05-29 08:53:49.645609 dsiunits-2.3.0/PKG-INFO
+-rw-r--r--   0 stehr     (1000) stehr     (1000)     2033 2024-05-29 08:49:18.000000 dsiunits-2.3.0/README.md
+-rw-r--r--   0 stehr     (1000) stehr     (1000)      764 2024-05-29 08:49:18.000000 dsiunits-2.3.0/pyproject.toml
+-rw-r--r--   0 stehr     (1000) stehr     (1000)      447 2024-05-29 08:53:49.645609 dsiunits-2.3.0/setup.cfg
+drwxr-xr-x   0 stehr     (1000) stehr     (1000)        0 2024-05-29 08:53:49.641609 dsiunits-2.3.0/src/
+-rw-r--r--   0 stehr     (1000) stehr     (1000)        0 2024-05-29 08:49:18.000000 dsiunits-2.3.0/src/__init__.py
+-rw-r--r--   0 stehr     (1000) stehr     (1000)    10641 2024-05-29 08:49:18.000000 dsiunits-2.3.0/src/dsiParser.py
+-rw-r--r--   0 stehr     (1000) stehr     (1000)     8120 2024-05-29 08:49:18.000000 dsiunits-2.3.0/src/dsiUnitNode.py
+-rw-r--r--   0 stehr     (1000) stehr     (1000)    22178 2024-05-29 08:49:18.000000 dsiunits-2.3.0/src/dsiUnits.py
+drwxr-xr-x   0 stehr     (1000) stehr     (1000)        0 2024-05-29 08:53:49.641609 dsiunits-2.3.0/src/dsiunits.egg-info/
+-rw-r--r--   0 stehr     (1000) stehr     (1000)    33313 2024-05-29 08:53:49.000000 dsiunits-2.3.0/src/dsiunits.egg-info/PKG-INFO
+-rw-r--r--   0 stehr     (1000) stehr     (1000)      353 2024-05-29 08:53:49.000000 dsiunits-2.3.0/src/dsiunits.egg-info/SOURCES.txt
+-rw-r--r--   0 stehr     (1000) stehr     (1000)        1 2024-05-29 08:53:49.000000 dsiunits-2.3.0/src/dsiunits.egg-info/dependency_links.txt
+-rw-r--r--   0 stehr     (1000) stehr     (1000)       43 2024-05-29 08:53:49.000000 dsiunits-2.3.0/src/dsiunits.egg-info/requires.txt
+-rw-r--r--   0 stehr     (1000) stehr     (1000)       67 2024-05-29 08:53:49.000000 dsiunits-2.3.0/src/dsiunits.egg-info/top_level.txt
+-rw-r--r--   0 stehr     (1000) stehr     (1000)     2888 2024-05-29 08:49:18.000000 dsiunits-2.3.0/src/regexGenerator.py
+-rw-r--r--   0 stehr     (1000) stehr     (1000)    13366 2024-05-29 08:49:18.000000 dsiunits-2.3.0/src/unitStrings.py
+drwxr-xr-x   0 stehr     (1000) stehr     (1000)        0 2024-05-29 08:53:49.641609 dsiunits-2.3.0/tests/
+-rw-r--r--   0 stehr     (1000) stehr     (1000)    27165 2024-05-29 08:49:18.000000 dsiunits-2.3.0/tests/test_dsiUnits.py
```

### Comparing `dsiunits-2.2.3/LICENSE` & `dsiunits-2.3.0/LICENSE`

 * *Files identical despite different names*

### Comparing `dsiunits-2.2.3/PKG-INFO` & `dsiunits-2.3.0/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: dsiunits
-Version: 2.2.3
+Version: 2.3.0
 Summary: This is a Python module for handling the SI units as objects in Python, parsing them from strings and converting them to Latex and Unicode, as well as performing math operations and calculating scale factors.
 Author-email: Benedikt Seeger <benedikt.seeger@ptb.de>, Vanessa Stehr <vanessa.stehr@ptb.de>
 License:                   GNU LESSER GENERAL PUBLIC LICENSE
                                Version 2.1, February 1999
         
          Copyright (C) 1991, 1999 Free Software Foundation, Inc.
          51 Franklin Street, Fifth Floor, Boston, MA  02110-1301  USA
```

### Comparing `dsiunits-2.2.3/README.md` & `dsiunits-2.3.0/README.md`

 * *Files identical despite different names*

### Comparing `dsiunits-2.2.3/pyproject.toml` & `dsiunits-2.3.0/pyproject.toml`

 * *Files 15% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["setuptools>=42", "wheel"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "dsiunits"  # Ensure this is correctly specified
-version = "2.2.3"
+version = "2.3.0"
 description = "This is a Python module for handling the SI units as objects in Python, parsing them from strings and converting them to Latex and Unicode, as well as performing math operations and calculating scale factors."
 authors = [
     { name="Benedikt Seeger", email="benedikt.seeger@ptb.de" },
     { name="Vanessa Stehr", email="vanessa.stehr@ptb.de" }
 ]
 license = { file="LICENSE" }
 readme = "README.md"
```

### Comparing `dsiunits-2.2.3/src/dsiunits.egg-info/PKG-INFO` & `dsiunits-2.3.0/src/dsiunits.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: dsiunits
-Version: 2.2.3
+Version: 2.3.0
 Summary: This is a Python module for handling the SI units as objects in Python, parsing them from strings and converting them to Latex and Unicode, as well as performing math operations and calculating scale factors.
 Author-email: Benedikt Seeger <benedikt.seeger@ptb.de>, Vanessa Stehr <vanessa.stehr@ptb.de>
 License:                   GNU LESSER GENERAL PUBLIC LICENSE
                                Version 2.1, February 1999
         
          Copyright (C) 1991, 1999 Free Software Foundation, Inc.
          51 Franklin Street, Fifth Floor, Boston, MA  02110-1301  USA
```

### Comparing `dsiunits-2.2.3/tests/test_dsiUnits.py` & `dsiunits-2.3.0/tests/test_dsiUnits.py`

 * *Files 8% similar despite different names*

```diff
@@ -11,25 +11,31 @@
 # Lesser General Public License for more details.
 
 # You should have received a copy of the GNU Lesser General Public
 # License along with this library; if not, write to the Free Software
 # Foundation, Inc., 51 Franklin Street, Fifth Floor, Boston, MA  02110-1301  USA
 
 import pytest
-from dsiUnits import _node, _getClosestStr,dsiUnit,dsiParser
 import sys
 import math
+import re
 from itertools import combinations
+
+from dsiUnitNode import dsiUnitNode
+from dsiUnits import dsiUnit
+from dsiParser import _getClosestStr, dsiParser, NonDsiUnitWarning
+from regexGenerator import generateRegex
+
 # Access the machine epsilon for the float data type
 epsilon = sys.float_info.epsilon
 
 def test_baseCase():
     # Most basic case: one unit without prefix or exponent
     tree = dsiUnit(r'\metre')
-    assert tree.tree == [[_node('','metre',1.0)]]
+    assert tree.tree == [[dsiUnitNode('','metre',1.0)]]
     assert tree.toLatex() == r'$$\mathrm{m}$$'
     assert tree.valid
     assert tree.warnings == []
 
     # One longer unit
     tree = dsiUnit(r'\milli\metre\tothe{0.5}\kilogram\per\mega\second\tothe{3}\ampere\tothe{-2}')
     assert tree.toLatex() == r'$$\frac{\sqrt{\mathrm{m}\mathrm{m}}\,\mathrm{kg}}{\mathrm{M}\mathrm{s}^{3}\,\mathrm{A}^{-2}}$$'
@@ -45,34 +51,32 @@
         assert not tree.valid
         assert len(tree.warnings) == 1
         assert tree.warnings == ['The identifier «foo» does not match any D-SI units!']
     
     # Unknown string in the middle of input
     with pytest.warns(RuntimeWarning, match=r'The identifier «mini» does not match any D-SI units! Did you mean one of these «\\milli» ?'):
         tree = dsiUnit(r'\kilo\metre\per\mini\second')
-        #print(tree.toLatex())
         assert tree.toLatex() == r'$$\frac{\mathrm{k}\mathrm{m}}{{\color{red}\mathrm{mini}}\,\mathrm{s}}$$'  
         assert not tree.valid
         assert len(tree.warnings) == 1
-        assert tree.warnings == ['The identifier «mini» does not match any D-SI units! Did you mean one of these «\\milli» ?']
+        assert tree.warnings == ['The identifier «mini» does not match any D-SI units! Did you mean one of these «\\milli»?']
     
     # Base unit missing
     with pytest.warns(RuntimeWarning, match=r'This D-SI unit seems to be missing the base unit! «\\milli\\tothe\{2\}»'):
         tree = dsiUnit(r'\milli\tothe{2}')
-        #print(tree.toLatex())
         assert tree.toLatex() == r'$${\color{red}\mathrm{m}{\color{red}\mathrm{}}^{2}}$$'  
         assert not tree.valid
         assert len(tree.warnings) == 1
         assert tree.warnings == ['This D-SI unit seems to be missing the base unit! «\\milli\\tothe{2}»']
 
 
 def test_power():
     # power
     powerTree = dsiUnit(r'\metre\tothe{2}')
-    assert powerTree.tree == [[_node('','metre',2.0)]]
+    assert powerTree.tree == [[dsiUnitNode('','metre',2.0)]]
     assert powerTree.toLatex() == r'$$\mathrm{m}^{2}$$'
     assert powerTree.valid
     assert powerTree.warnings == []
     assert dsiUnit(r'\metre\tothe{0.5}').toLatex() == r'$$\sqrt{\mathrm{m}}$$'
     assert dsiUnit(r'\metre\tothe{-2}').toLatex() == r'$$\mathrm{m}^{-2}$$'
     assert dsiUnit(r'\metre\tothe{1337}').toLatex() == r'$$\mathrm{m}^{1337}$$'
 
@@ -81,28 +85,28 @@
         abcPowerTree = dsiUnit(r'\metre\tothe{foo}')
         assert abcPowerTree.toLatex() == r'$$\mathrm{m}^{{\color{red}\mathrm{foo}}}$$'
         assert abcPowerTree.warnings == ['The exponent «foo» is not a number!']
 
 def test_prefix():
     # D-SI prefix
     prefixTree = dsiUnit(r'\kilo\metre')
-    assert prefixTree.tree == [[_node('kilo','metre','')]]
+    assert prefixTree.tree == [[dsiUnitNode('kilo','metre','')]]
     assert prefixTree.toLatex() == r'$$\mathrm{k}\mathrm{m}$$'
     assert prefixTree.valid
 
 def test_node():
     # full node
     fullNodeTree = dsiUnit(r'\kilo\metre\tothe{2}')
-    assert fullNodeTree.tree == [[_node('kilo','metre','2')]]
+    assert fullNodeTree.tree == [[dsiUnitNode('kilo','metre','2')]]
     assert fullNodeTree.toLatex() == r'$$\mathrm{k}\mathrm{m}^{2}$$'
     assert fullNodeTree.valid
 
 def test_fraction():
     fractionTree = dsiUnit(r'\mega\metre\per\second\tothe{2}')
-    assert fractionTree.tree == [[_node('mega','metre','')],[_node('','second','2')]]
+    assert fractionTree.tree == [[dsiUnitNode('mega','metre','')],[dsiUnitNode('','second','2')]]
     assert fractionTree.toLatex() == r'$$\frac{\mathrm{M}\mathrm{m}}{\mathrm{s}^{2}}$$'
     assert fractionTree.valid
 
     # double fraction
     with pytest.warns(RuntimeWarning, match=r'The dsi string contains more than one \\per, does not match specs! Given string: \\metre\\per\\metre\\per\\metre'):
         tree = dsiUnit(r'\metre\per\metre\per\metre')
         assert tree.toLatex() == r'$$\mathrm{m}{\color{red}/}\mathrm{m}{\color{red}/}\mathrm{m}$$'  
@@ -115,28 +119,31 @@
         tree = dsiUnit(r'\per\one')
         assert tree.toLatex() == r'$$1$$'
         assert not tree.valid
         assert len(tree.warnings) == 1
 
 def test_empty():
     with pytest.warns(RuntimeWarning, match='Given D-SI string is empty!'):
-        assert dsiUnit('').toLatex() == '$${\\color{red}\\mathrm{NULL}}$$'
+        assert dsiUnit('').toLatex() == '$$\\textpipe\\mathrm{NULL}$$'
 
 def test_doubleBackslash():
     with pytest.warns(RuntimeWarning, match=r"Double backslash found in string, treating as one backslash: «\\\\metre\\per\\second»"):
         assert dsiUnit(r'\\metre\per\second').toLatex() == '$$\\frac{\\mathrm{m}}{\\mathrm{s}}$$'
 
 def test_wrappers():
     assert dsiUnit(r'\metre').toLatex(wrapper='') == r'\mathrm{m}'
     assert dsiUnit(r'\metre').toLatex(wrapper='$', prefix=r'\mathrm{Unit: }', suffix=r'\mathrm{(generated from D-SI string)}') == r'$\mathrm{Unit: }\mathrm{m}\mathrm{(generated from D-SI string)}$'
-    parserWrapper = dsiParser(latexDefaultWrapper="&")
-    assert parserWrapper.parse(r'\metre').toLatex() == r'&\mathrm{m}&'
-    parserFull = dsiParser(latexDefaultWrapper='@', latexDefaultPrefix=r'\mathrm{Prefix}', latexDefaultSuffix=r'\mathrm{Suffix}')
-    assert parserFull.parse(r'\metre').toLatex() == r'@\mathrm{Prefix}\mathrm{m}\mathrm{Suffix}@'
-
+    dsiParser()._latexDefaultWrapper="&"
+    assert dsiUnit(r'\metre').toLatex() == r'&\mathrm{m}&'
+    dsiParser()._latexDefaultWrapper = "@"
+    dsiParser()._latexDefaultPrefix = r'\mathrm{Prefix}'
+    dsiParser()._latexDefaultSuffix = r'\mathrm{Suffix}'
+    assert dsiUnit(r'\metre').toLatex() == r'@\mathrm{Prefix}\mathrm{m}\mathrm{Suffix}@'
+    dsiParser().resetToDefaults()
+    assert dsiUnit(r'\metre').toLatex() == r'$$\mathrm{m}$$'
 def test_getClosestMatch():
     closestMatch = _getClosestStr(r'\kiilo')
     assert closestMatch == (['kilo'])
     closestMatch = _getClosestStr(r'\mettre')
     assert closestMatch == (['metre'])
     closestMatch = _getClosestStr(r'\ttothe')
     assert closestMatch == (['tothe'])
@@ -153,16 +160,15 @@
     assert dsiUnit(r'\metre\tothe{0.3333333333333333333}').toLatex(wrapper='') == r'\sqrt[3]{\mathrm{m}}'
     assert dsiUnit(r'\metre\tothe{0.666666666666666}').toLatex(wrapper='') == r'\sqrt[3]{\mathrm{m}^{2}}'
 
 def test_baseUnitConversion():
     # Test conversion of a single derived unit to its base unit
     derivedUnitTree = dsiUnit(r'\kilo\metre')
     baseUnitTree = derivedUnitTree.toBaseUnitTree()
-    assert baseUnitTree.tree == [[_node('', 'metre', '', scaleFactor=1000.0)]]
-    assert baseUnitTree.toLatex() == '$$\\mathrm{m}$$'
+    assert baseUnitTree.toLatex() == r'$$1000.0\cdot\mathrm{m}$$'
 
     # Test conversion of a complex unit with a fraction to base units
     complexUnitTree = dsiUnit(r'\kilo\watt\hour')
     complexUnitTree2 = dsiUnit(r'\kilo\watt\hour')
     complexBaseUnitTree = complexUnitTree.toBaseUnitTree()
     reduceFractionTree = complexBaseUnitTree.reduceFraction()
     megacomplexUnitTree = dsiUnit(r'\mega\watt\hour')
@@ -438,15 +444,14 @@
     assert str(dsiUnit(r'\yobi\byte')) == r'\yobi\byte'
     assert str(dsiUnit(r'\kibi\bit\tothe{2}\per\byte')) == r'\kibi\bit\tothe{2}\per\byte'
     assert str(dsiUnit(r'\kibi\byte\tothe{-2}')) == r'\kibi\byte\tothe{-2}'
     assert str(dsiUnit(r'\mebi\bit\tothe{0.5}')) == r'\mebi\bit\tothe{0.5}'
     assert str(dsiUnit(r'\gibi\byte\tothe{0.333333333333333}')) == r'\gibi\byte\tothe{0.333333}'
     assert str(dsiUnit(r'\tebi\bit\tothe{0.666666666666666}')) == r'\tebi\bit\tothe{0.666667}'
     assert str(dsiUnit(r'\pebi\byte\tothe{1337}')) == r'\pebi\byte\tothe{1337}'
-
 def test_digitalUnitsScalebility():
     bit=dsiUnit(r'\bit')
     byte=dsiUnit(r'\byte')
     kibiBit=dsiUnit(r'\kibi\bit')
     kibiByte=dsiUnit(r'\kibi\byte')
     mebiBit=dsiUnit(r'\mebi\bit')
     mebiByte=dsiUnit(r'\mebi\byte')
@@ -458,49 +463,57 @@
     pebiByte=dsiUnit(r'\pebi\byte')
     exbiBit=dsiUnit(r'\exbi\bit')
     exbiByte=dsiUnit(r'\exbi\byte')
     zebiBit=dsiUnit(r'\zebi\bit')
     zebiByte=dsiUnit(r'\zebi\byte')
     yobiBit=dsiUnit(r'\yobi\bit')
     yobiByte=dsiUnit(r'\yobi\byte')
-    assert bit.isScalablyEqualTo(byte)[0]==8
-    assert kibiBit.isScalablyEqualTo(kibiByte)[0]==8
-    assert mebiBit.isScalablyEqualTo(mebiByte)[0]==8
-    assert gibiBit.isScalablyEqualTo(gibiByte)[0]==8
-    assert tebiBit.isScalablyEqualTo(tebiByte)[0]==8
-    assert pebiBit.isScalablyEqualTo(pebiByte)[0]==8
-    assert exbiBit.isScalablyEqualTo(exbiByte)[0]==8
-    assert zebiBit.isScalablyEqualTo(zebiByte)[0]==8
-    assert yobiBit.isScalablyEqualTo(yobiByte)[0]==8
-    assert bit.isScalablyEqualTo(kibiBit)[0]==1024
-    assert bit.isScalablyEqualTo(mebiBit)[0]==1048576
-    assert bit.isScalablyEqualTo(gibiBit)[0]==1073741824
-    assert bit.isScalablyEqualTo(tebiBit)[0]==1099511627776
-    assert bit.isScalablyEqualTo(pebiBit)[0]==1125899906842624
-    assert bit.isScalablyEqualTo(exbiBit)[0]==1152921504606846976
-    assert bit.isScalablyEqualTo(zebiBit)[0]==1180591620717411303424
-    assert bit.isScalablyEqualTo(yobiBit)[0]==1208925819614629174706176
-    assert byte.isScalablyEqualTo(kibiByte)[0]==1024
-    assert byte.isScalablyEqualTo(mebiByte)[0]==1048576
-    assert byte.isScalablyEqualTo(gibiByte)[0]==1073741824
-    assert byte.isScalablyEqualTo(tebiByte)[0]==1099511627776
-    assert byte.isScalablyEqualTo(pebiByte)[0]==1125899906842624
-    assert byte.isScalablyEqualTo(exbiByte)[0]==1152921504606846976
-    assert byte.isScalablyEqualTo(zebiByte)[0]==1180591620717411303424
-    assert byte.isScalablyEqualTo(yobiByte)[0]==1208925819614629174706176
-    assert kibiBit.isScalablyEqualTo(mebiBit)[0]==1024
-    assert kibiBit.isScalablyEqualTo(gibiBit)[0]==1048576
-    assert kibiBit.isScalablyEqualTo(tebiBit)[0]==1073741824
-    assert kibiBit.isScalablyEqualTo(pebiBit)[0]==1099511627776
-    assert kibiBit.isScalablyEqualTo(exbiBit)[0]==1125899906842624
-    assert kibiBit.isScalablyEqualTo(zebiBit)[0]==1152921504606846976
-    assert kibiBit.isScalablyEqualTo(yobiBit)[0]==1180591620717411303424
-    assert mebiBit.isScalablyEqualTo(kibiByte)[0]==1/128
-    assert mebiBit.isScalablyEqualTo(kibiBit)[0] == 1 / 1024
+    assert bit.isScalablyEqualTo(byte,complete=True)[0]==8
+    assert kibiBit.isScalablyEqualTo(kibiByte,complete=True)[0]==8
+    assert mebiBit.isScalablyEqualTo(mebiByte,complete=True)[0]==8
+    assert gibiBit.isScalablyEqualTo(gibiByte,complete=True)[0]==8
+    assert tebiBit.isScalablyEqualTo(tebiByte,complete=True)[0]==8
+    assert pebiBit.isScalablyEqualTo(pebiByte,complete=True)[0]==8
+    assert exbiBit.isScalablyEqualTo(exbiByte,complete=True)[0]==8
+    assert zebiBit.isScalablyEqualTo(zebiByte,complete=True)[0]==8
+    assert yobiBit.isScalablyEqualTo(yobiByte,complete=True)[0]==8
+    assert bit.isScalablyEqualTo(kibiBit,complete=True)[0]==1024
+    assert bit.isScalablyEqualTo(mebiBit,complete=True)[0]==1048576
+    assert bit.isScalablyEqualTo(gibiBit,complete=True)[0]==1073741824
+    assert bit.isScalablyEqualTo(tebiBit,complete=True)[0]==1099511627776
+    assert bit.isScalablyEqualTo(pebiBit,complete=True)[0]==1125899906842624
+    assert bit.isScalablyEqualTo(exbiBit,complete=True)[0]==1152921504606846976
+    assert bit.isScalablyEqualTo(zebiBit,complete=True)[0]==1180591620717411303424
+    assert bit.isScalablyEqualTo(yobiBit,complete=True)[0]==1208925819614629174706176
+    assert byte.isScalablyEqualTo(kibiByte,complete=True)[0]==1024
+    assert byte.isScalablyEqualTo(mebiByte,complete=True)[0]==1048576
+    assert byte.isScalablyEqualTo(gibiByte,complete=True)[0]==1073741824
+    assert byte.isScalablyEqualTo(tebiByte,complete=True)[0]==1099511627776
+    assert byte.isScalablyEqualTo(pebiByte,complete=True)[0]==1125899906842624
+    assert byte.isScalablyEqualTo(exbiByte,complete=True)[0]==1152921504606846976
+    assert byte.isScalablyEqualTo(zebiByte,complete=True)[0]==1180591620717411303424
+    assert byte.isScalablyEqualTo(yobiByte,complete=True)[0]==1208925819614629174706176
+    assert kibiBit.isScalablyEqualTo(mebiBit,complete=True)[0]==1024
+    assert kibiBit.isScalablyEqualTo(gibiBit,complete=True)[0]==1048576
+    assert kibiBit.isScalablyEqualTo(tebiBit,complete=True)[0]==1073741824
+    assert kibiBit.isScalablyEqualTo(pebiBit,complete=True)[0]==1099511627776
+    assert kibiBit.isScalablyEqualTo(exbiBit,complete=True)[0]==1125899906842624
+    assert kibiBit.isScalablyEqualTo(zebiBit,complete=True)[0]==1152921504606846976
+    assert kibiBit.isScalablyEqualTo(yobiBit,complete=True)[0]==1180591620717411303424
+    assert mebiBit.isScalablyEqualTo(kibiByte,complete=True)[0]==1/128
+    assert mebiBit.isScalablyEqualTo(kibiBit,complete=True)[0] == 1 / 1024
 
+def test_binaryPrefixMath():
+    mebiByte=dsiUnit(r'\mebi\byte')
+    mebiBit = dsiUnit(r'\mebi\bit')
+    gibiByte=dsiUnit(r'\gibi\byte')
+    shouldBeKB=gibiByte/mebiByte
+    assert str(shouldBeKB) == r'1024.0*\byte'
+    shouldBe8192=gibiByte/mebiBit
+    assert str(shouldBe8192.toBaseUnitTree())== r'1024.0*\bit\tothe{-1}\byte'
 
 def test_scalability_relative_units():
     percent = dsiUnit(r'\percent')
     ppm = dsiUnit(r'\ppm')
     one = dsiUnit(r'\one')
 
     # Check scalability between percent and one
@@ -519,7 +532,56 @@
     assert percent.isScalablyEqualTo(one, complete=True)[1] == dsiUnit(r'\one')
     assert one.isScalablyEqualTo(percent, complete=True)[1] == dsiUnit(r'\one')
     assert ppm.isScalablyEqualTo(one, complete=True)[1] == dsiUnit(r'\one')
     assert one.isScalablyEqualTo(ppm, complete=True)[1] == dsiUnit(r'\one')
     assert percent.isScalablyEqualTo(ppm, complete=True)[1] == dsiUnit(r'\one')
     assert ppm.isScalablyEqualTo(percent, complete=True)[1] == dsiUnit(r'\one')
 
+def test_nonDsiUnit():
+    with pytest.warns(NonDsiUnitWarning):
+        nonDsiUnit = dsiUnit(r'|fluid ounce')
+        assert nonDsiUnit.nonDsiUnit == True
+        assert nonDsiUnit.tree == [[dsiUnitNode('','fluid ounce', valid=False)]]
+
+        assert dsiUnit(r'|fluid ounce') == dsiUnit(r'|fluid ounce')
+
+        with pytest.raises(RuntimeError):
+            dsiUnit(r'|fluid ounce')**2
+
+        with pytest.raises(RuntimeError):
+            dsiUnit(r'|fluid ounce')*dsiUnit(r'|international avoirdupois ounce')
+
+        with pytest.raises(RuntimeError):
+            dsiUnit(r'|fluid ounce')/dsiUnit(r'|international avoirdupois ounce')
+        assert str(nonDsiUnit)=='|fluid ounce'
+        assert nonDsiUnit.toLatex()==r'$$\textpipe\mathrm{fluid ounce}$$'
+        assert nonDsiUnit.toUTF8()=='|fluid ounce'
+        assert nonDsiUnit==nonDsiUnit
+
+def test_sameUnitMultiplicationWithPrefixes():
+    mm=dsiUnit(r'\milli\metre')
+    km=dsiUnit(r'\kilo\metre')
+    cm=dsiUnit(r'\centi\metre')
+    m=dsiUnit(r'\metre')
+    m2=km*mm
+    m3=km*m*mm
+    m4=m3*mm
+    assert m2==dsiUnit(r'\metre\tothe{2}')
+
+def test_PowersWithVolumes():
+    volumeFromLength=dsiUnit(r'\milli\metre\tothe{3}')
+    volumeAsVolume=dsiUnit(r'\micro\litre')
+    scalfactor,baseunit=volumeFromLength.isScalablyEqualTo(volumeAsVolume)
+    assert scalfactor==1.0
+    assert baseunit==dsiUnit(r'\metre\tothe{3}')
+
+def test_RegexGenerator():
+    dsiRegex = generateRegex()
+    assert re.match(dsiRegex, r'\milli\metre\tothe{2}')
+    assert re.match(dsiRegex, r'\kilo\metre\per\second')
+    assert re.match(dsiRegex, r'\metre\kilogram')
+    assert not re.match(dsiRegex, r'\metre\per\second\per\gram')
+    assert re.match(dsiRegex, r'|ounce')
+    assert not re.match(dsiRegex, r'\ounce')
+    assert not re.match(dsiRegex, r'\milli\kilogram')
+    assert not re.match(dsiRegex, r'\kilo\gram')
+    assert not re.match(dsiRegex, r'\deci\bel')
```

