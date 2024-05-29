# Comparing `tmp/gliner-0.2.0.tar.gz` & `tmp/gliner-0.2.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "gliner-0.2.0.tar", last modified: Sun May 26 12:26:20 2024, max compression
+gzip compressed data, was "gliner-0.2.1.tar", last modified: Tue May 28 16:25:17 2024, max compression
```

## Comparing `gliner-0.2.0.tar` & `gliner-0.2.1.tar`

### file list

```diff
@@ -1,27 +1,27 @@
-drwxr-xr-x   0 urchadezaratiana   (501) staff       (20)        0 2024-05-26 12:26:20.461176 gliner-0.2.0/
--rw-r--r--   0 urchadezaratiana   (501) staff       (20)    11357 2024-03-12 13:03:35.000000 gliner-0.2.0/LICENSE
--rw-r--r--   0 urchadezaratiana   (501) staff       (20)    12205 2024-05-26 12:26:20.460907 gliner-0.2.0/PKG-INFO
--rw-r--r--   0 urchadezaratiana   (501) staff       (20)    11480 2024-05-25 10:03:53.000000 gliner-0.2.0/README.md
-drwxr-xr-x   0 urchadezaratiana   (501) staff       (20)        0 2024-05-26 12:26:20.456832 gliner-0.2.0/gliner/
--rw-r--r--   0 urchadezaratiana   (501) staff       (20)       70 2024-05-26 12:25:24.000000 gliner-0.2.0/gliner/__init__.py
--rw-r--r--   0 urchadezaratiana   (501) staff       (20)    14903 2024-05-26 04:58:35.000000 gliner-0.2.0/gliner/model.py
-drwxr-xr-x   0 urchadezaratiana   (501) staff       (20)        0 2024-05-26 12:26:20.460203 gliner-0.2.0/gliner/modules/
--rw-r--r--   0 urchadezaratiana   (501) staff       (20)        0 2024-03-12 14:09:51.000000 gliner-0.2.0/gliner/modules/__init__.py
--rw-r--r--   0 urchadezaratiana   (501) staff       (20)     9988 2024-05-25 22:08:09.000000 gliner-0.2.0/gliner/modules/base.py
--rw-r--r--   0 urchadezaratiana   (501) staff       (20)     8330 2024-05-26 12:03:54.000000 gliner-0.2.0/gliner/modules/data.py
--rw-r--r--   0 urchadezaratiana   (501) staff       (20)     2352 2024-05-25 16:08:03.000000 gliner-0.2.0/gliner/modules/data_proc.py
--rw-r--r--   0 urchadezaratiana   (501) staff       (20)     5047 2024-04-22 09:17:20.000000 gliner-0.2.0/gliner/modules/evaluator.py
--rw-r--r--   0 urchadezaratiana   (501) staff       (20)     6248 2024-05-26 04:49:34.000000 gliner-0.2.0/gliner/modules/layers.py
--rw-r--r--   0 urchadezaratiana   (501) staff       (20)     2148 2024-05-25 16:08:03.000000 gliner-0.2.0/gliner/modules/loss_functions.py
--rw-r--r--   0 urchadezaratiana   (501) staff       (20)     5801 2024-05-11 10:05:18.000000 gliner-0.2.0/gliner/modules/run_evaluation.py
--rw-r--r--   0 urchadezaratiana   (501) staff       (20)    10015 2024-05-25 10:03:53.000000 gliner-0.2.0/gliner/modules/span_rep.py
--rw-r--r--   0 urchadezaratiana   (501) staff       (20)     1928 2024-04-09 17:20:30.000000 gliner-0.2.0/gliner/modules/token_rep.py
--rw-r--r--   0 urchadezaratiana   (501) staff       (20)     1660 2024-04-24 10:13:06.000000 gliner-0.2.0/gliner/modules/token_splitter.py
-drwxr-xr-x   0 urchadezaratiana   (501) staff       (20)        0 2024-05-26 12:26:20.460628 gliner-0.2.0/gliner.egg-info/
--rw-r--r--   0 urchadezaratiana   (501) staff       (20)    12205 2024-05-26 12:26:20.000000 gliner-0.2.0/gliner.egg-info/PKG-INFO
--rw-r--r--   0 urchadezaratiana   (501) staff       (20)      524 2024-05-26 12:26:20.000000 gliner-0.2.0/gliner.egg-info/SOURCES.txt
--rw-r--r--   0 urchadezaratiana   (501) staff       (20)        1 2024-05-26 12:26:20.000000 gliner-0.2.0/gliner.egg-info/dependency_links.txt
--rw-r--r--   0 urchadezaratiana   (501) staff       (20)       97 2024-05-26 12:26:20.000000 gliner-0.2.0/gliner.egg-info/requires.txt
--rw-r--r--   0 urchadezaratiana   (501) staff       (20)        7 2024-05-26 12:26:20.000000 gliner-0.2.0/gliner.egg-info/top_level.txt
--rw-r--r--   0 urchadezaratiana   (501) staff       (20)     1046 2024-04-24 10:21:08.000000 gliner-0.2.0/pyproject.toml
--rw-r--r--   0 urchadezaratiana   (501) staff       (20)       38 2024-05-26 12:26:20.461218 gliner-0.2.0/setup.cfg
+drwxr-xr-x   0 urchadezaratiana   (501) staff       (20)        0 2024-05-28 16:25:17.511053 gliner-0.2.1/
+-rw-r--r--   0 urchadezaratiana   (501) staff       (20)    11357 2024-03-12 13:03:35.000000 gliner-0.2.1/LICENSE
+-rw-r--r--   0 urchadezaratiana   (501) staff       (20)    12205 2024-05-28 16:25:17.510810 gliner-0.2.1/PKG-INFO
+-rw-r--r--   0 urchadezaratiana   (501) staff       (20)    11480 2024-05-25 10:03:53.000000 gliner-0.2.1/README.md
+drwxr-xr-x   0 urchadezaratiana   (501) staff       (20)        0 2024-05-28 16:25:17.506411 gliner-0.2.1/gliner/
+-rw-r--r--   0 urchadezaratiana   (501) staff       (20)       70 2024-05-28 16:24:18.000000 gliner-0.2.1/gliner/__init__.py
+-rw-r--r--   0 urchadezaratiana   (501) staff       (20)    15026 2024-05-28 13:08:39.000000 gliner-0.2.1/gliner/model.py
+drwxr-xr-x   0 urchadezaratiana   (501) staff       (20)        0 2024-05-28 16:25:17.510158 gliner-0.2.1/gliner/modules/
+-rw-r--r--   0 urchadezaratiana   (501) staff       (20)        0 2024-03-12 14:09:51.000000 gliner-0.2.1/gliner/modules/__init__.py
+-rw-r--r--   0 urchadezaratiana   (501) staff       (20)     9988 2024-05-25 22:08:09.000000 gliner-0.2.1/gliner/modules/base.py
+-rw-r--r--   0 urchadezaratiana   (501) staff       (20)     8330 2024-05-26 12:03:54.000000 gliner-0.2.1/gliner/modules/data.py
+-rw-r--r--   0 urchadezaratiana   (501) staff       (20)     2352 2024-05-25 16:08:03.000000 gliner-0.2.1/gliner/modules/data_proc.py
+-rw-r--r--   0 urchadezaratiana   (501) staff       (20)     5047 2024-04-22 09:17:20.000000 gliner-0.2.1/gliner/modules/evaluator.py
+-rw-r--r--   0 urchadezaratiana   (501) staff       (20)     6248 2024-05-26 04:49:34.000000 gliner-0.2.1/gliner/modules/layers.py
+-rw-r--r--   0 urchadezaratiana   (501) staff       (20)     2148 2024-05-25 16:08:03.000000 gliner-0.2.1/gliner/modules/loss_functions.py
+-rw-r--r--   0 urchadezaratiana   (501) staff       (20)     5801 2024-05-11 10:05:18.000000 gliner-0.2.1/gliner/modules/run_evaluation.py
+-rw-r--r--   0 urchadezaratiana   (501) staff       (20)    10015 2024-05-25 10:03:53.000000 gliner-0.2.1/gliner/modules/span_rep.py
+-rw-r--r--   0 urchadezaratiana   (501) staff       (20)     1928 2024-04-09 17:20:30.000000 gliner-0.2.1/gliner/modules/token_rep.py
+-rw-r--r--   0 urchadezaratiana   (501) staff       (20)     1660 2024-04-24 10:13:06.000000 gliner-0.2.1/gliner/modules/token_splitter.py
+drwxr-xr-x   0 urchadezaratiana   (501) staff       (20)        0 2024-05-28 16:25:17.510568 gliner-0.2.1/gliner.egg-info/
+-rw-r--r--   0 urchadezaratiana   (501) staff       (20)    12205 2024-05-28 16:25:17.000000 gliner-0.2.1/gliner.egg-info/PKG-INFO
+-rw-r--r--   0 urchadezaratiana   (501) staff       (20)      524 2024-05-28 16:25:17.000000 gliner-0.2.1/gliner.egg-info/SOURCES.txt
+-rw-r--r--   0 urchadezaratiana   (501) staff       (20)        1 2024-05-28 16:25:17.000000 gliner-0.2.1/gliner.egg-info/dependency_links.txt
+-rw-r--r--   0 urchadezaratiana   (501) staff       (20)       97 2024-05-28 16:25:17.000000 gliner-0.2.1/gliner.egg-info/requires.txt
+-rw-r--r--   0 urchadezaratiana   (501) staff       (20)        7 2024-05-28 16:25:17.000000 gliner-0.2.1/gliner.egg-info/top_level.txt
+-rw-r--r--   0 urchadezaratiana   (501) staff       (20)     1046 2024-04-24 10:21:08.000000 gliner-0.2.1/pyproject.toml
+-rw-r--r--   0 urchadezaratiana   (501) staff       (20)       38 2024-05-28 16:25:17.511094 gliner-0.2.1/setup.cfg
```

### Comparing `gliner-0.2.0/LICENSE` & `gliner-0.2.1/LICENSE`

 * *Files identical despite different names*

### Comparing `gliner-0.2.0/PKG-INFO` & `gliner-0.2.1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: gliner
-Version: 0.2.0
+Version: 0.2.1
 Summary: Generalist model for NER (Extract any entity types from texts)
 Author: Urchade Zaratiana, Nadi Tomeh, Pierre Holat, Thierry Charnois
 Maintainer: Urchade Zaratiana
 License: Apache-2.0
 Project-URL: Homepage, https://github.com/urchade/GLiNER
 Keywords: named-entity-recognition,ner,data-science,natural-language-processing,artificial-intelligence,nlp,machine-learning,transformers
 Requires-Python: >=3.8
```

### Comparing `gliner-0.2.0/README.md` & `gliner-0.2.1/README.md`

 * *Files identical despite different names*

### Comparing `gliner-0.2.0/gliner/model.py` & `gliner-0.2.1/gliner/model.py`

 * *Files 1% similar despite different names*

```diff
@@ -287,14 +287,18 @@
 
         # get batch_nums and span_pos
         for i, element in enumerate(x["entities_id"]):
             for ent in element:
                 st, ed, sp_label = ent
                 sp_label = sp_label - 1
 
+                # prevent indexing errors
+                if st >= seq_len or ed >= seq_len:
+                    continue
+
                 word_labels[0, i, st, sp_label] = 1  # start
                 word_labels[1, i, ed, sp_label] = 1  # end
                 word_labels[2, i, st:ed + 1, sp_label] = 1  # inside
 
         # compute scores for start, end and inside
         all_scores = self.scorer(word_rep, entity_type_rep)  # (3, batch_size, seq_len, num_classes)
```

### Comparing `gliner-0.2.0/gliner/modules/base.py` & `gliner-0.2.1/gliner/modules/base.py`

 * *Files identical despite different names*

### Comparing `gliner-0.2.0/gliner/modules/data.py` & `gliner-0.2.1/gliner/modules/data.py`

 * *Files identical despite different names*

### Comparing `gliner-0.2.0/gliner/modules/data_proc.py` & `gliner-0.2.1/gliner/modules/data_proc.py`

 * *Files identical despite different names*

### Comparing `gliner-0.2.0/gliner/modules/evaluator.py` & `gliner-0.2.1/gliner/modules/evaluator.py`

 * *Files identical despite different names*

### Comparing `gliner-0.2.0/gliner/modules/layers.py` & `gliner-0.2.1/gliner/modules/layers.py`

 * *Files identical despite different names*

### Comparing `gliner-0.2.0/gliner/modules/loss_functions.py` & `gliner-0.2.1/gliner/modules/loss_functions.py`

 * *Files identical despite different names*

### Comparing `gliner-0.2.0/gliner/modules/run_evaluation.py` & `gliner-0.2.1/gliner/modules/run_evaluation.py`

 * *Files identical despite different names*

### Comparing `gliner-0.2.0/gliner/modules/span_rep.py` & `gliner-0.2.1/gliner/modules/span_rep.py`

 * *Files identical despite different names*

### Comparing `gliner-0.2.0/gliner/modules/token_rep.py` & `gliner-0.2.1/gliner/modules/token_rep.py`

 * *Files identical despite different names*

### Comparing `gliner-0.2.0/gliner/modules/token_splitter.py` & `gliner-0.2.1/gliner/modules/token_splitter.py`

 * *Files identical despite different names*

### Comparing `gliner-0.2.0/gliner.egg-info/PKG-INFO` & `gliner-0.2.1/gliner.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: gliner
-Version: 0.2.0
+Version: 0.2.1
 Summary: Generalist model for NER (Extract any entity types from texts)
 Author: Urchade Zaratiana, Nadi Tomeh, Pierre Holat, Thierry Charnois
 Maintainer: Urchade Zaratiana
 License: Apache-2.0
 Project-URL: Homepage, https://github.com/urchade/GLiNER
 Keywords: named-entity-recognition,ner,data-science,natural-language-processing,artificial-intelligence,nlp,machine-learning,transformers
 Requires-Python: >=3.8
```

### Comparing `gliner-0.2.0/gliner.egg-info/SOURCES.txt` & `gliner-0.2.1/gliner.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `gliner-0.2.0/pyproject.toml` & `gliner-0.2.1/pyproject.toml`

 * *Files identical despite different names*

