# Comparing `tmp/skope_rules_temp-0.2.5.tar.gz` & `tmp/skope_rules_temp-0.2.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "skope_rules_temp-0.2.5.tar", max compression
+gzip compressed data, was "skope_rules_temp-0.2.6.tar", max compression
```

## Comparing `skope_rules_temp-0.2.5.tar` & `skope_rules_temp-0.2.6.tar`

### file list

```diff
@@ -1,15 +1,15 @@
--rw-r--r--   0        0        0      428 2024-03-05 21:27:15.152010 skope_rules_temp-0.2.5/AUTHORS.rst
--rw-r--r--   0        0        0     1551 2024-03-05 21:27:15.152121 skope_rules_temp-0.2.5/COPYING
--rw-r--r--   0        0        0     5465 2024-03-05 21:27:15.152351 skope_rules_temp-0.2.5/README.md
--rw-r--r--   0        0        0      485 2024-05-24 11:17:46.355645 skope_rules_temp-0.2.5/pyproject.toml
--rw-r--r--   0        0        0      115 2024-03-05 21:27:15.158029 skope_rules_temp-0.2.5/src/skope_rules_temp/__init__.py
--rw-r--r--   0        0        0       74 2024-03-05 21:27:15.158175 skope_rules_temp-0.2.5/src/skope_rules_temp/datasets/__init__.py
--rw-r--r--   0        0        0     1435 2024-03-05 21:27:15.158300 skope_rules_temp-0.2.5/src/skope_rules_temp/datasets/credit_data.py
--rw-r--r--   0        0        0     2352 2024-03-05 21:27:15.158409 skope_rules_temp-0.2.5/src/skope_rules_temp/rule.py
--rw-r--r--   0        0        0    27233 2024-05-24 11:15:23.243436 skope_rules_temp-0.2.5/src/skope_rules_temp/skope_rules.py
--rw-r--r--   0        0        0        0 2024-03-05 21:27:15.158776 skope_rules_temp-0.2.5/src/skope_rules_temp/tests/__init__.py
--rw-r--r--   0        0        0      277 2024-03-05 21:27:15.158910 skope_rules_temp-0.2.5/src/skope_rules_temp/tests/test_common.py
--rw-r--r--   0        0        0     1872 2024-03-05 21:27:15.159076 skope_rules_temp-0.2.5/src/skope_rules_temp/tests/test_rule.py
--rw-r--r--   0        0        0     8074 2024-03-05 21:27:15.159227 skope_rules_temp-0.2.5/src/skope_rules_temp/tests/test_skope_rules.py
--rw-r--r--   0        0        0      849 2024-05-24 11:15:23.246200 skope_rules_temp-0.2.5/src/skope_rules_temp/utils.py
--rw-r--r--   0        0        0     6205 1970-01-01 00:00:00.000000 skope_rules_temp-0.2.5/PKG-INFO
+-rw-r--r--   0        0        0      428 2024-03-05 21:27:15.152010 skope_rules_temp-0.2.6/AUTHORS.rst
+-rw-r--r--   0        0        0     1551 2024-03-05 21:27:15.152121 skope_rules_temp-0.2.6/COPYING
+-rw-r--r--   0        0        0     5465 2024-03-05 21:27:15.152351 skope_rules_temp-0.2.6/README.md
+-rw-r--r--   0        0        0      485 2024-05-29 09:18:12.646463 skope_rules_temp-0.2.6/pyproject.toml
+-rw-r--r--   0        0        0      115 2024-03-05 21:27:15.158029 skope_rules_temp-0.2.6/src/skope_rules_temp/__init__.py
+-rw-r--r--   0        0        0       74 2024-03-05 21:27:15.158175 skope_rules_temp-0.2.6/src/skope_rules_temp/datasets/__init__.py
+-rw-r--r--   0        0        0     1435 2024-03-05 21:27:15.158300 skope_rules_temp-0.2.6/src/skope_rules_temp/datasets/credit_data.py
+-rw-r--r--   0        0        0     2352 2024-03-05 21:27:15.158409 skope_rules_temp-0.2.6/src/skope_rules_temp/rule.py
+-rw-r--r--   0        0        0    27233 2024-05-24 11:15:23.243436 skope_rules_temp-0.2.6/src/skope_rules_temp/skope_rules.py
+-rw-r--r--   0        0        0        0 2024-03-05 21:27:15.158776 skope_rules_temp-0.2.6/src/skope_rules_temp/tests/__init__.py
+-rw-r--r--   0        0        0      277 2024-03-05 21:27:15.158910 skope_rules_temp-0.2.6/src/skope_rules_temp/tests/test_common.py
+-rw-r--r--   0        0        0     1872 2024-03-05 21:27:15.159076 skope_rules_temp-0.2.6/src/skope_rules_temp/tests/test_rule.py
+-rw-r--r--   0        0        0     8074 2024-03-05 21:27:15.159227 skope_rules_temp-0.2.6/src/skope_rules_temp/tests/test_skope_rules.py
+-rw-r--r--   0        0        0      869 2024-05-29 09:18:12.641843 skope_rules_temp-0.2.6/src/skope_rules_temp/utils.py
+-rw-r--r--   0        0        0     6205 1970-01-01 00:00:00.000000 skope_rules_temp-0.2.6/PKG-INFO
```

### Comparing `skope_rules_temp-0.2.5/COPYING` & `skope_rules_temp-0.2.6/COPYING`

 * *Files identical despite different names*

### Comparing `skope_rules_temp-0.2.5/README.md` & `skope_rules_temp-0.2.6/README.md`

 * *Files identical despite different names*

### Comparing `skope_rules_temp-0.2.5/src/skope_rules_temp/datasets/credit_data.py` & `skope_rules_temp-0.2.6/src/skope_rules_temp/datasets/credit_data.py`

 * *Files identical despite different names*

### Comparing `skope_rules_temp-0.2.5/src/skope_rules_temp/rule.py` & `skope_rules_temp-0.2.6/src/skope_rules_temp/rule.py`

 * *Files identical despite different names*

### Comparing `skope_rules_temp-0.2.5/src/skope_rules_temp/skope_rules.py` & `skope_rules_temp-0.2.6/src/skope_rules_temp/skope_rules.py`

 * *Files identical despite different names*

### Comparing `skope_rules_temp-0.2.5/src/skope_rules_temp/tests/test_rule.py` & `skope_rules_temp-0.2.6/src/skope_rules_temp/tests/test_rule.py`

 * *Files identical despite different names*

### Comparing `skope_rules_temp-0.2.5/src/skope_rules_temp/tests/test_skope_rules.py` & `skope_rules_temp-0.2.6/src/skope_rules_temp/tests/test_skope_rules.py`

 * *Files identical despite different names*

### Comparing `skope_rules_temp-0.2.5/src/skope_rules_temp/utils.py` & `skope_rules_temp-0.2.6/src/skope_rules_temp/utils.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,7 +1,9 @@
+import numpy as np
+
 def indices_to_mask(indices, mask_length):
     """Convert list of indices to boolean mask.
 
     Parameters
     ----------
     indices : list-like
         List of integers treated as indices.
```

### Comparing `skope_rules_temp-0.2.5/PKG-INFO` & `skope_rules_temp-0.2.6/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: skope-rules-temp
-Version: 0.2.5
+Version: 0.2.6
 Summary: Fork of https://github.com/scikit-learn-contrib/skope-rules
 Author: Pierre Hulot
 Author-email: pierre@ai-vidence.com
 Requires-Python: >=3.10
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
```

