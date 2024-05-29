# Comparing `tmp/hippo_db-0.3.8.tar.gz` & `tmp/hippo_db-0.3.9.tar.gz`

## Comparing `hippo_db-0.3.8.tar` & `hippo_db-0.3.9.tar`

### file list

```diff
@@ -1,22 +1,22 @@
--rw-r--r--   0        0        0      155 2020-02-02 00:00:00.000000 hippo_db-0.3.8/hippo/__init__.py
--rw-r--r--   0        0        0    10398 2020-02-02 00:00:00.000000 hippo_db-0.3.8/hippo/animal.py
--rw-r--r--   0        0        0     7401 2020-02-02 00:00:00.000000 hippo_db-0.3.8/hippo/compound.py
--rw-r--r--   0        0        0     5349 2020-02-02 00:00:00.000000 hippo_db-0.3.8/hippo/cset.py
--rw-r--r--   0        0        0    30282 2020-02-02 00:00:00.000000 hippo_db-0.3.8/hippo/db.py
--rw-r--r--   0        0        0      665 2020-02-02 00:00:00.000000 hippo_db-0.3.8/hippo/feature.py
--rw-r--r--   0        0        0      812 2020-02-02 00:00:00.000000 hippo_db-0.3.8/hippo/metadata.py
--rw-r--r--   0        0        0    18015 2020-02-02 00:00:00.000000 hippo_db-0.3.8/hippo/plotting.py
--rw-r--r--   0        0        0     8720 2020-02-02 00:00:00.000000 hippo_db-0.3.8/hippo/pose.py
--rw-r--r--   0        0        0     3446 2020-02-02 00:00:00.000000 hippo_db-0.3.8/hippo/pset.py
--rw-r--r--   0        0        0     7074 2020-02-02 00:00:00.000000 hippo_db-0.3.8/hippo/pycule.py
--rw-r--r--   0        0        0     1159 2020-02-02 00:00:00.000000 hippo_db-0.3.8/hippo/quote.py
--rw-r--r--   0        0        0     5690 2020-02-02 00:00:00.000000 hippo_db-0.3.8/hippo/reaction.py
--rw-r--r--   0        0        0     3559 2020-02-02 00:00:00.000000 hippo_db-0.3.8/hippo/recipe.py
--rw-r--r--   0        0        0     1256 2020-02-02 00:00:00.000000 hippo_db-0.3.8/hippo/rset.py
--rw-r--r--   0        0        0     3015 2020-02-02 00:00:00.000000 hippo_db-0.3.8/hippo/tags.py
--rw-r--r--   0        0        0     1464 2020-02-02 00:00:00.000000 hippo_db-0.3.8/hippo/target.py
--rw-r--r--   0        0        0     2070 2020-02-02 00:00:00.000000 hippo_db-0.3.8/hippo/tools.py
--rw-r--r--   0        0        0     3088 2020-02-02 00:00:00.000000 hippo_db-0.3.8/.gitignore
--rw-r--r--   0        0        0      244 2020-02-02 00:00:00.000000 hippo_db-0.3.8/README.md
--rw-r--r--   0        0        0      684 2020-02-02 00:00:00.000000 hippo_db-0.3.8/pyproject.toml
--rw-r--r--   0        0        0      763 2020-02-02 00:00:00.000000 hippo_db-0.3.8/PKG-INFO
+-rw-r--r--   0        0        0      155 2020-02-02 00:00:00.000000 hippo_db-0.3.9/hippo/__init__.py
+-rw-r--r--   0        0        0    10398 2020-02-02 00:00:00.000000 hippo_db-0.3.9/hippo/animal.py
+-rw-r--r--   0        0        0     7401 2020-02-02 00:00:00.000000 hippo_db-0.3.9/hippo/compound.py
+-rw-r--r--   0        0        0     5349 2020-02-02 00:00:00.000000 hippo_db-0.3.9/hippo/cset.py
+-rw-r--r--   0        0        0    30282 2020-02-02 00:00:00.000000 hippo_db-0.3.9/hippo/db.py
+-rw-r--r--   0        0        0      665 2020-02-02 00:00:00.000000 hippo_db-0.3.9/hippo/feature.py
+-rw-r--r--   0        0        0      812 2020-02-02 00:00:00.000000 hippo_db-0.3.9/hippo/metadata.py
+-rw-r--r--   0        0        0    18015 2020-02-02 00:00:00.000000 hippo_db-0.3.9/hippo/plotting.py
+-rw-r--r--   0        0        0     8720 2020-02-02 00:00:00.000000 hippo_db-0.3.9/hippo/pose.py
+-rw-r--r--   0        0        0     3446 2020-02-02 00:00:00.000000 hippo_db-0.3.9/hippo/pset.py
+-rw-r--r--   0        0        0     7074 2020-02-02 00:00:00.000000 hippo_db-0.3.9/hippo/pycule.py
+-rw-r--r--   0        0        0     1159 2020-02-02 00:00:00.000000 hippo_db-0.3.9/hippo/quote.py
+-rw-r--r--   0        0        0     5690 2020-02-02 00:00:00.000000 hippo_db-0.3.9/hippo/reaction.py
+-rw-r--r--   0        0        0     3559 2020-02-02 00:00:00.000000 hippo_db-0.3.9/hippo/recipe.py
+-rw-r--r--   0        0        0     1256 2020-02-02 00:00:00.000000 hippo_db-0.3.9/hippo/rset.py
+-rw-r--r--   0        0        0     3015 2020-02-02 00:00:00.000000 hippo_db-0.3.9/hippo/tags.py
+-rw-r--r--   0        0        0     1464 2020-02-02 00:00:00.000000 hippo_db-0.3.9/hippo/target.py
+-rw-r--r--   0        0        0     2070 2020-02-02 00:00:00.000000 hippo_db-0.3.9/hippo/tools.py
+-rw-r--r--   0        0        0     3088 2020-02-02 00:00:00.000000 hippo_db-0.3.9/.gitignore
+-rw-r--r--   0        0        0      244 2020-02-02 00:00:00.000000 hippo_db-0.3.9/README.md
+-rw-r--r--   0        0        0      743 2020-02-02 00:00:00.000000 hippo_db-0.3.9/pyproject.toml
+-rw-r--r--   0        0        0      854 2020-02-02 00:00:00.000000 hippo_db-0.3.9/PKG-INFO
```

### Comparing `hippo_db-0.3.8/hippo/animal.py` & `hippo_db-0.3.9/hippo/animal.py`

 * *Files identical despite different names*

### Comparing `hippo_db-0.3.8/hippo/compound.py` & `hippo_db-0.3.9/hippo/compound.py`

 * *Files identical despite different names*

### Comparing `hippo_db-0.3.8/hippo/cset.py` & `hippo_db-0.3.9/hippo/cset.py`

 * *Files identical despite different names*

### Comparing `hippo_db-0.3.8/hippo/db.py` & `hippo_db-0.3.9/hippo/db.py`

 * *Files identical despite different names*

### Comparing `hippo_db-0.3.8/hippo/feature.py` & `hippo_db-0.3.9/hippo/feature.py`

 * *Files identical despite different names*

### Comparing `hippo_db-0.3.8/hippo/metadata.py` & `hippo_db-0.3.9/hippo/metadata.py`

 * *Files identical despite different names*

### Comparing `hippo_db-0.3.8/hippo/plotting.py` & `hippo_db-0.3.9/hippo/plotting.py`

 * *Files identical despite different names*

### Comparing `hippo_db-0.3.8/hippo/pose.py` & `hippo_db-0.3.9/hippo/pose.py`

 * *Files identical despite different names*

### Comparing `hippo_db-0.3.8/hippo/pset.py` & `hippo_db-0.3.9/hippo/pset.py`

 * *Files identical despite different names*

### Comparing `hippo_db-0.3.8/hippo/pycule.py` & `hippo_db-0.3.9/hippo/pycule.py`

 * *Files identical despite different names*

### Comparing `hippo_db-0.3.8/hippo/quote.py` & `hippo_db-0.3.9/hippo/quote.py`

 * *Files identical despite different names*

### Comparing `hippo_db-0.3.8/hippo/reaction.py` & `hippo_db-0.3.9/hippo/reaction.py`

 * *Files identical despite different names*

### Comparing `hippo_db-0.3.8/hippo/recipe.py` & `hippo_db-0.3.9/hippo/recipe.py`

 * *Files identical despite different names*

### Comparing `hippo_db-0.3.8/hippo/rset.py` & `hippo_db-0.3.9/hippo/rset.py`

 * *Files identical despite different names*

### Comparing `hippo_db-0.3.8/hippo/tags.py` & `hippo_db-0.3.9/hippo/tags.py`

 * *Files identical despite different names*

### Comparing `hippo_db-0.3.8/hippo/target.py` & `hippo_db-0.3.9/hippo/target.py`

 * *Files identical despite different names*

### Comparing `hippo_db-0.3.8/hippo/tools.py` & `hippo_db-0.3.9/hippo/tools.py`

 * *Files identical despite different names*

### Comparing `hippo_db-0.3.8/.gitignore` & `hippo_db-0.3.9/.gitignore`

 * *Files identical despite different names*

### Comparing `hippo_db-0.3.8/PKG-INFO` & `hippo_db-0.3.9/PKG-INFO`

 * *Files 10% similar despite different names*

```diff
@@ -1,19 +1,23 @@
 Metadata-Version: 2.1
 Name: hippo-db
-Version: 0.3.8
+Version: 0.3.9
 Summary: Hit Interaction Profiling and Procurement Optimisation
 Project-URL: Homepage, https://hippo.winokan.com
 Project-URL: Bug Tracker, https://github.com/mwinokan/HIPPO/issues
 Author-email: Max Winokan <max@winokan.com>
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python :: 3
 Requires-Python: >=3.10
+Requires-Dist: chardet
+Requires-Dist: jupyterlab
 Requires-Dist: molparse>=0.0.13
+Requires-Dist: pycule
+Requires-Dist: tqdm
 Description-Content-Type: text/markdown
 
 ![hippo_logo](https://github.com/mwinokan/HIPPO/blob/main/logos/hippo_logo-05.png?raw=true)
 
 HIPPO
 =====
```

