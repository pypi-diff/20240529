# Comparing `tmp/nlpx-1.2.6.tar.gz` & `tmp/nlpx-1.2.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "nlpx-1.2.6.tar", last modified: Wed May 29 00:50:54 2024, max compression
+gzip compressed data, was "nlpx-1.2.7.tar", last modified: Wed May 29 06:01:41 2024, max compression
```

## Comparing `nlpx-1.2.6.tar` & `nlpx-1.2.7.tar`

### file list

```diff
@@ -1,26 +1,26 @@
-drwxr-xr-x   0 summy      (501) staff       (20)        0 2024-05-29 00:50:54.490615 nlpx-1.2.6/
--rw-r--r--   0 summy      (501) staff       (20)      730 2024-05-29 00:50:54.490123 nlpx-1.2.6/PKG-INFO
--rw-r--r--   0 summy      (501) staff       (20)      448 2024-04-07 01:09:43.000000 nlpx-1.2.6/README.rst
-drwxr-xr-x   0 summy      (501) staff       (20)        0 2024-05-29 00:50:54.464050 nlpx-1.2.6/nlpx/
--rw-r--r--   0 summy      (501) staff       (20)        0 2024-05-21 11:15:55.000000 nlpx-1.2.6/nlpx/__init__.py
-drwxr-xr-x   0 summy      (501) staff       (20)        0 2024-05-29 00:50:54.478671 nlpx-1.2.6/nlpx/llm/
--rw-r--r--   0 summy      (501) staff       (20)      189 2024-05-29 00:08:25.000000 nlpx-1.2.6/nlpx/llm/__init__.py
--rw-r--r--   0 summy      (501) staff       (20)     5604 2024-05-29 00:43:58.000000 nlpx-1.2.6/nlpx/llm/_model_wrapper.py
--rw-r--r--   0 summy      (501) staff       (20)    10270 2024-05-29 00:33:21.000000 nlpx-1.2.6/nlpx/llm/_tokenize_vec.py
--rw-r--r--   0 summy      (501) staff       (20)     1016 2024-05-29 00:01:18.000000 nlpx-1.2.6/nlpx/llm/_utils.py
-drwxr-xr-x   0 summy      (501) staff       (20)        0 2024-05-29 00:50:54.482209 nlpx-1.2.6/nlpx/models/
--rw-r--r--   0 summy      (501) staff       (20)       31 2024-05-24 23:09:44.000000 nlpx-1.2.6/nlpx/models/__init__.py
--rw-r--r--   0 summy      (501) staff       (20)     3848 2024-05-28 13:54:23.000000 nlpx-1.2.6/nlpx/models/_text_cnn.py
-drwxr-xr-x   0 summy      (501) staff       (20)        0 2024-05-29 00:50:54.487502 nlpx-1.2.6/nlpx/text_token/
--rw-r--r--   0 summy      (501) staff       (20)      316 2024-05-26 05:47:41.000000 nlpx-1.2.6/nlpx/text_token/__init__.py
--rw-r--r--   0 summy      (501) staff       (20)    25732 2024-05-26 06:13:27.000000 nlpx-1.2.6/nlpx/text_token/_tokenizer.py
--rw-r--r--   0 summy      (501) staff       (20)    16628 2024-05-26 05:47:41.000000 nlpx-1.2.6/nlpx/text_token/_utils.py
--rw-r--r--   0 summy      (501) staff       (20)     4051 2024-05-28 13:25:28.000000 nlpx-1.2.6/nlpx/training.py
-drwxr-xr-x   0 summy      (501) staff       (20)        0 2024-05-29 00:50:54.470162 nlpx-1.2.6/nlpx.egg-info/
--rw-r--r--   0 summy      (501) staff       (20)      730 2024-05-29 00:50:54.000000 nlpx-1.2.6/nlpx.egg-info/PKG-INFO
--rw-r--r--   0 summy      (501) staff       (20)      418 2024-05-29 00:50:54.000000 nlpx-1.2.6/nlpx.egg-info/SOURCES.txt
--rw-r--r--   0 summy      (501) staff       (20)        1 2024-05-29 00:50:54.000000 nlpx-1.2.6/nlpx.egg-info/dependency_links.txt
--rw-r--r--   0 summy      (501) staff       (20)        1 2024-05-28 13:58:19.000000 nlpx-1.2.6/nlpx.egg-info/not-zip-safe
--rw-r--r--   0 summy      (501) staff       (20)        5 2024-05-29 00:50:54.000000 nlpx-1.2.6/nlpx.egg-info/top_level.txt
--rw-r--r--   0 summy      (501) staff       (20)       38 2024-05-29 00:50:54.490780 nlpx-1.2.6/setup.cfg
--rw-r--r--   0 summy      (501) staff       (20)     1044 2024-05-29 00:20:06.000000 nlpx-1.2.6/setup.py
+drwxr-xr-x   0 summy      (501) staff       (20)        0 2024-05-29 06:01:41.115899 nlpx-1.2.7/
+-rw-r--r--   0 summy      (501) staff       (20)      730 2024-05-29 06:01:41.115192 nlpx-1.2.7/PKG-INFO
+-rw-r--r--   0 summy      (501) staff       (20)      448 2024-04-07 01:09:43.000000 nlpx-1.2.7/README.rst
+drwxr-xr-x   0 summy      (501) staff       (20)        0 2024-05-29 06:01:41.086156 nlpx-1.2.7/nlpx/
+-rw-r--r--   0 summy      (501) staff       (20)        0 2024-05-21 11:15:55.000000 nlpx-1.2.7/nlpx/__init__.py
+drwxr-xr-x   0 summy      (501) staff       (20)        0 2024-05-29 06:01:41.098736 nlpx-1.2.7/nlpx/llm/
+-rw-r--r--   0 summy      (501) staff       (20)      189 2024-05-29 00:08:25.000000 nlpx-1.2.7/nlpx/llm/__init__.py
+-rw-r--r--   0 summy      (501) staff       (20)     5604 2024-05-29 00:43:58.000000 nlpx-1.2.7/nlpx/llm/_model_wrapper.py
+-rw-r--r--   0 summy      (501) staff       (20)    10270 2024-05-29 00:33:21.000000 nlpx-1.2.7/nlpx/llm/_tokenize_vec.py
+-rw-r--r--   0 summy      (501) staff       (20)     2384 2024-05-29 06:01:29.000000 nlpx-1.2.7/nlpx/llm/_utils.py
+drwxr-xr-x   0 summy      (501) staff       (20)        0 2024-05-29 06:01:41.105730 nlpx-1.2.7/nlpx/models/
+-rw-r--r--   0 summy      (501) staff       (20)       31 2024-05-24 23:09:44.000000 nlpx-1.2.7/nlpx/models/__init__.py
+-rw-r--r--   0 summy      (501) staff       (20)     3848 2024-05-28 13:54:23.000000 nlpx-1.2.7/nlpx/models/_text_cnn.py
+drwxr-xr-x   0 summy      (501) staff       (20)        0 2024-05-29 06:01:41.112847 nlpx-1.2.7/nlpx/text_token/
+-rw-r--r--   0 summy      (501) staff       (20)      316 2024-05-26 05:47:41.000000 nlpx-1.2.7/nlpx/text_token/__init__.py
+-rw-r--r--   0 summy      (501) staff       (20)    25732 2024-05-26 06:13:27.000000 nlpx-1.2.7/nlpx/text_token/_tokenizer.py
+-rw-r--r--   0 summy      (501) staff       (20)    16628 2024-05-26 05:47:41.000000 nlpx-1.2.7/nlpx/text_token/_utils.py
+-rw-r--r--   0 summy      (501) staff       (20)     4051 2024-05-28 13:25:28.000000 nlpx-1.2.7/nlpx/training.py
+drwxr-xr-x   0 summy      (501) staff       (20)        0 2024-05-29 06:01:41.091914 nlpx-1.2.7/nlpx.egg-info/
+-rw-r--r--   0 summy      (501) staff       (20)      730 2024-05-29 06:01:40.000000 nlpx-1.2.7/nlpx.egg-info/PKG-INFO
+-rw-r--r--   0 summy      (501) staff       (20)      418 2024-05-29 06:01:40.000000 nlpx-1.2.7/nlpx.egg-info/SOURCES.txt
+-rw-r--r--   0 summy      (501) staff       (20)        1 2024-05-29 06:01:40.000000 nlpx-1.2.7/nlpx.egg-info/dependency_links.txt
+-rw-r--r--   0 summy      (501) staff       (20)        1 2024-05-28 13:58:19.000000 nlpx-1.2.7/nlpx.egg-info/not-zip-safe
+-rw-r--r--   0 summy      (501) staff       (20)        5 2024-05-29 06:01:40.000000 nlpx-1.2.7/nlpx.egg-info/top_level.txt
+-rw-r--r--   0 summy      (501) staff       (20)       38 2024-05-29 06:01:41.116184 nlpx-1.2.7/setup.cfg
+-rw-r--r--   0 summy      (501) staff       (20)     1044 2024-05-29 06:01:37.000000 nlpx-1.2.7/setup.py
```

### Comparing `nlpx-1.2.6/PKG-INFO` & `nlpx-1.2.7/PKG-INFO`

 * *Files 14% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: nlpx
-Version: 1.2.6
+Version: 1.2.7
 Summary: A tool set for NLP.
 Home-page: https://gitee.com/summry/nlpx
 Author: summy
 Author-email: xiazhongbiao@126.com
 License: UNKNOWN
 Keywords: NLP
 Platform: UNKNOWN
```

### Comparing `nlpx-1.2.6/nlpx/llm/_model_wrapper.py` & `nlpx-1.2.7/nlpx/llm/_model_wrapper.py`

 * *Files identical despite different names*

### Comparing `nlpx-1.2.6/nlpx/llm/_tokenize_vec.py` & `nlpx-1.2.7/nlpx/llm/_tokenize_vec.py`

 * *Files identical despite different names*

### Comparing `nlpx-1.2.6/nlpx/llm/_utils.py` & `nlpx-1.2.7/nlpx/llm/_utils.py`

 * *Files 20% similar despite different names*

```diff
@@ -2,16 +2,35 @@
 import numpy as np
 from typing import List, Union
 from sklearn.model_selection import train_test_split
 from torch.utils.data import TensorDataset
 from ._tokenize_vec import TokenizeVec
 
 
-def train_test_set(tokenize_vec: TokenizeVec, texts: List[str], y: Union[torch.LongTensor, List, np.ndarray], max_length: int = 0,
-			  test_size=0.2, n_jobs=-1, random_state=None):
+def train_test_set(tokenize_vec: TokenizeVec, train_texts: List[str], test_texts: List[str],
+                   y_train: Union[torch.LongTensor, List, np.ndarray], y_test: Union[torch.LongTensor, List, np.ndarray],
+                         max_length: int = 0, n_jobs=-1):
+    X_train = tokenize_vec.parallel_encode_plus(train_texts, max_length=max_length, padding='max_length',
+                                        truncation=True, add_special_tokens=True,
+                                        return_token_type_ids=True,return_attention_mask=True,
+                                        return_tensors='pt', n_jobs=n_jobs)
+    if isinstance(y_train, List) or isinstance(y_train, np.ndarray):
+        y_train = torch.tensor(y_train, dtype=torch.long)
+
+    X_test = tokenize_vec.parallel_encode_plus(test_texts, max_length=max_length, padding='max_length',
+                                                truncation=True, add_special_tokens=True,
+                                                return_token_type_ids=True, return_attention_mask=True,
+                                                return_tensors='pt', n_jobs=n_jobs)
+    if isinstance(y_test, List) or isinstance(y_test, np.ndarray):
+        y_test = torch.tensor(y_train, dtype=torch.long)
+    return TensorDataset(X_train, y_train), TensorDataset(X_test, y_test)
+
+
+def train_test_split_set(tokenize_vec: TokenizeVec, texts: List[str], y: Union[torch.LongTensor, List, np.ndarray],
+                         max_length: int = 0, test_size=0.2, n_jobs=-1, random_state=None):
     X = tokenize_vec.parallel_encode_plus(texts, max_length=max_length, padding='max_length',
                                         truncation=True, add_special_tokens=True,
                                         return_token_type_ids=True,return_attention_mask=True,
                                         return_tensors='pt', n_jobs=n_jobs)
     if isinstance(y, List) or isinstance(y, np.ndarray):
         y = torch.tensor(y, dtype=torch.long)
     X_train, X_test, y_train, y_test = train_test_split(X, y, test_size=test_size, random_state=random_state)
```

### Comparing `nlpx-1.2.6/nlpx/models/_text_cnn.py` & `nlpx-1.2.7/nlpx/models/_text_cnn.py`

 * *Files identical despite different names*

### Comparing `nlpx-1.2.6/nlpx/text_token/_tokenizer.py` & `nlpx-1.2.7/nlpx/text_token/_tokenizer.py`

 * *Files identical despite different names*

### Comparing `nlpx-1.2.6/nlpx/text_token/_utils.py` & `nlpx-1.2.7/nlpx/text_token/_utils.py`

 * *Files identical despite different names*

### Comparing `nlpx-1.2.6/nlpx/training.py` & `nlpx-1.2.7/nlpx/training.py`

 * *Files identical despite different names*

### Comparing `nlpx-1.2.6/nlpx.egg-info/PKG-INFO` & `nlpx-1.2.7/nlpx.egg-info/PKG-INFO`

 * *Files 14% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: nlpx
-Version: 1.2.6
+Version: 1.2.7
 Summary: A tool set for NLP.
 Home-page: https://gitee.com/summry/nlpx
 Author: summy
 Author-email: xiazhongbiao@126.com
 License: UNKNOWN
 Keywords: NLP
 Platform: UNKNOWN
```

### Comparing `nlpx-1.2.6/setup.py` & `nlpx-1.2.7/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -16,15 +16,15 @@
 
 setup(
     name='nlpx',
     packages=['nlpx', 'nlpx.models', 'nlpx.llm', 'nlpx.text_token'],
     description="A tool set for NLP.",
     long_description=long_description,
     long_description_content_type='text/markdown',
-    version='1.2.6',
+    version='1.2.7',
     url='https://gitee.com/summry/nlpx',
     author='summy',
     author_email='xiazhongbiao@126.com',
     keywords=['NLP'],
     package_data={
         # include json and txt files
         '': ['*.rst', '*.dtd', '*.tpl'],
```

