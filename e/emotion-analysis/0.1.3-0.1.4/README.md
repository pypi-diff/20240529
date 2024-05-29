# Comparing `tmp/emotion_analysis-0.1.3.tar.gz` & `tmp/emotion_analysis-0.1.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "emotion_analysis-0.1.3.tar", last modified: Tue May 28 06:54:14 2024, max compression
+gzip compressed data, was "emotion_analysis-0.1.4.tar", last modified: Tue May 28 07:45:56 2024, max compression
```

## Comparing `emotion_analysis-0.1.3.tar` & `emotion_analysis-0.1.4.tar`

### file list

```diff
@@ -1,20 +1,21 @@
-drwxrwxr-x   0 ahsan-pmylsp  (1000) ahsan-pmylsp  (1000)        0 2024-05-28 06:54:14.599492 emotion_analysis-0.1.3/
--rw-rw-r--   0 ahsan-pmylsp  (1000) ahsan-pmylsp  (1000)      297 2024-05-28 06:54:14.599492 emotion_analysis-0.1.3/PKG-INFO
-drwxrwxr-x   0 ahsan-pmylsp  (1000) ahsan-pmylsp  (1000)        0 2024-05-28 06:54:14.599492 emotion_analysis-0.1.3/emotion_analysis/
--rw-rw-r--   0 ahsan-pmylsp  (1000) ahsan-pmylsp  (1000)      462 2024-05-27 16:11:32.000000 emotion_analysis-0.1.3/emotion_analysis/__init__.py
--rw-rw-r--   0 ahsan-pmylsp  (1000) ahsan-pmylsp  (1000)     2184 2024-05-28 03:08:43.000000 emotion_analysis-0.1.3/emotion_analysis/bert_pcc_score_emotions.py
--rw-rw-r--   0 ahsan-pmylsp  (1000) ahsan-pmylsp  (1000)    13125 2024-05-28 03:01:22.000000 emotion_analysis-0.1.3/emotion_analysis/data_preprocessing.py
--rw-rw-r--   0 ahsan-pmylsp  (1000) ahsan-pmylsp  (1000)     5281 2024-05-25 21:05:45.000000 emotion_analysis-0.1.3/emotion_analysis/frnn.py
--rw-rw-r--   0 ahsan-pmylsp  (1000) ahsan-pmylsp  (1000)     2145 2024-05-28 03:09:56.000000 emotion_analysis-0.1.3/emotion_analysis/roberta_pcc_score_emotions.py
--rw-rw-r--   0 ahsan-pmylsp  (1000) ahsan-pmylsp  (1000)     2293 2024-05-28 06:30:12.000000 emotion_analysis-0.1.3/emotion_analysis/tweets_embedding.py
-drwxrwxr-x   0 ahsan-pmylsp  (1000) ahsan-pmylsp  (1000)        0 2024-05-28 06:54:14.599492 emotion_analysis-0.1.3/emotion_analysis.egg-info/
--rw-r--r--   0 ahsan-pmylsp  (1000) ahsan-pmylsp  (1000)      297 2024-05-28 06:54:14.000000 emotion_analysis-0.1.3/emotion_analysis.egg-info/PKG-INFO
--rw-rw-r--   0 ahsan-pmylsp  (1000) ahsan-pmylsp  (1000)      460 2024-05-28 06:54:14.000000 emotion_analysis-0.1.3/emotion_analysis.egg-info/SOURCES.txt
--rw-rw-r--   0 ahsan-pmylsp  (1000) ahsan-pmylsp  (1000)        1 2024-05-28 06:54:14.000000 emotion_analysis-0.1.3/emotion_analysis.egg-info/dependency_links.txt
--rw-rw-r--   0 ahsan-pmylsp  (1000) ahsan-pmylsp  (1000)       81 2024-05-28 06:54:14.000000 emotion_analysis-0.1.3/emotion_analysis.egg-info/requires.txt
--rw-rw-r--   0 ahsan-pmylsp  (1000) ahsan-pmylsp  (1000)       23 2024-05-28 06:54:14.000000 emotion_analysis-0.1.3/emotion_analysis.egg-info/top_level.txt
--rw-rw-r--   0 ahsan-pmylsp  (1000) ahsan-pmylsp  (1000)       38 2024-05-28 06:54:14.599492 emotion_analysis-0.1.3/setup.cfg
--rw-rw-r--   0 ahsan-pmylsp  (1000) ahsan-pmylsp  (1000)      558 2024-05-28 06:54:08.000000 emotion_analysis-0.1.3/setup.py
-drwxrwxr-x   0 ahsan-pmylsp  (1000) ahsan-pmylsp  (1000)        0 2024-05-28 06:54:14.599492 emotion_analysis-0.1.3/tests/
--rw-rw-r--   0 ahsan-pmylsp  (1000) ahsan-pmylsp  (1000)        0 2024-05-27 16:13:33.000000 emotion_analysis-0.1.3/tests/__init__.py
--rw-rw-r--   0 ahsan-pmylsp  (1000) ahsan-pmylsp  (1000)    14898 2024-05-28 03:32:26.000000 emotion_analysis-0.1.3/tests/test.py
+drwxrwxr-x   0 ahsan-pmylsp  (1000) ahsan-pmylsp  (1000)        0 2024-05-28 07:45:56.011623 emotion_analysis-0.1.4/
+-rw-rw-r--   0 ahsan-pmylsp  (1000) ahsan-pmylsp  (1000)    17690 2024-05-28 07:45:56.011623 emotion_analysis-0.1.4/PKG-INFO
+-rw-rw-r--   0 ahsan-pmylsp  (1000) ahsan-pmylsp  (1000)    16961 2024-05-28 07:25:14.000000 emotion_analysis-0.1.4/README.md
+drwxrwxr-x   0 ahsan-pmylsp  (1000) ahsan-pmylsp  (1000)        0 2024-05-28 07:45:56.007623 emotion_analysis-0.1.4/emotion_analysis/
+-rw-rw-r--   0 ahsan-pmylsp  (1000) ahsan-pmylsp  (1000)      462 2024-05-27 16:11:32.000000 emotion_analysis-0.1.4/emotion_analysis/__init__.py
+-rw-rw-r--   0 ahsan-pmylsp  (1000) ahsan-pmylsp  (1000)     2184 2024-05-28 03:08:43.000000 emotion_analysis-0.1.4/emotion_analysis/bert_pcc_score_emotions.py
+-rw-rw-r--   0 ahsan-pmylsp  (1000) ahsan-pmylsp  (1000)    13125 2024-05-28 03:01:22.000000 emotion_analysis-0.1.4/emotion_analysis/data_preprocessing.py
+-rw-rw-r--   0 ahsan-pmylsp  (1000) ahsan-pmylsp  (1000)     5281 2024-05-25 21:05:45.000000 emotion_analysis-0.1.4/emotion_analysis/frnn.py
+-rw-rw-r--   0 ahsan-pmylsp  (1000) ahsan-pmylsp  (1000)     2145 2024-05-28 03:09:56.000000 emotion_analysis-0.1.4/emotion_analysis/roberta_pcc_score_emotions.py
+-rw-rw-r--   0 ahsan-pmylsp  (1000) ahsan-pmylsp  (1000)     2293 2024-05-28 06:30:12.000000 emotion_analysis-0.1.4/emotion_analysis/tweets_embedding.py
+drwxrwxr-x   0 ahsan-pmylsp  (1000) ahsan-pmylsp  (1000)        0 2024-05-28 07:45:56.011623 emotion_analysis-0.1.4/emotion_analysis.egg-info/
+-rw-r--r--   0 ahsan-pmylsp  (1000) ahsan-pmylsp  (1000)    17690 2024-05-28 07:45:55.000000 emotion_analysis-0.1.4/emotion_analysis.egg-info/PKG-INFO
+-rw-rw-r--   0 ahsan-pmylsp  (1000) ahsan-pmylsp  (1000)      470 2024-05-28 07:45:55.000000 emotion_analysis-0.1.4/emotion_analysis.egg-info/SOURCES.txt
+-rw-rw-r--   0 ahsan-pmylsp  (1000) ahsan-pmylsp  (1000)        1 2024-05-28 07:45:55.000000 emotion_analysis-0.1.4/emotion_analysis.egg-info/dependency_links.txt
+-rw-rw-r--   0 ahsan-pmylsp  (1000) ahsan-pmylsp  (1000)       81 2024-05-28 07:45:55.000000 emotion_analysis-0.1.4/emotion_analysis.egg-info/requires.txt
+-rw-rw-r--   0 ahsan-pmylsp  (1000) ahsan-pmylsp  (1000)       23 2024-05-28 07:45:55.000000 emotion_analysis-0.1.4/emotion_analysis.egg-info/top_level.txt
+-rw-rw-r--   0 ahsan-pmylsp  (1000) ahsan-pmylsp  (1000)       38 2024-05-28 07:45:56.011623 emotion_analysis-0.1.4/setup.cfg
+-rw-rw-r--   0 ahsan-pmylsp  (1000) ahsan-pmylsp  (1000)     1218 2024-05-28 07:45:54.000000 emotion_analysis-0.1.4/setup.py
+drwxrwxr-x   0 ahsan-pmylsp  (1000) ahsan-pmylsp  (1000)        0 2024-05-28 07:45:56.011623 emotion_analysis-0.1.4/tests/
+-rw-rw-r--   0 ahsan-pmylsp  (1000) ahsan-pmylsp  (1000)        0 2024-05-27 16:13:33.000000 emotion_analysis-0.1.4/tests/__init__.py
+-rw-rw-r--   0 ahsan-pmylsp  (1000) ahsan-pmylsp  (1000)    14898 2024-05-28 03:32:26.000000 emotion_analysis-0.1.4/tests/test.py
```

### Comparing `emotion_analysis-0.1.3/emotion_analysis/bert_pcc_score_emotions.py` & `emotion_analysis-0.1.4/emotion_analysis/bert_pcc_score_emotions.py`

 * *Files identical despite different names*

### Comparing `emotion_analysis-0.1.3/emotion_analysis/data_preprocessing.py` & `emotion_analysis-0.1.4/emotion_analysis/data_preprocessing.py`

 * *Files identical despite different names*

### Comparing `emotion_analysis-0.1.3/emotion_analysis/frnn.py` & `emotion_analysis-0.1.4/emotion_analysis/frnn.py`

 * *Files identical despite different names*

### Comparing `emotion_analysis-0.1.3/emotion_analysis/roberta_pcc_score_emotions.py` & `emotion_analysis-0.1.4/emotion_analysis/roberta_pcc_score_emotions.py`

 * *Files identical despite different names*

### Comparing `emotion_analysis-0.1.3/emotion_analysis/tweets_embedding.py` & `emotion_analysis-0.1.4/emotion_analysis/tweets_embedding.py`

 * *Files identical despite different names*

### Comparing `emotion_analysis-0.1.3/tests/test.py` & `emotion_analysis-0.1.4/tests/test.py`

 * *Files identical despite different names*

