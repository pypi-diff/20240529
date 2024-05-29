# Comparing `tmp/nlpx-1.2.7.tar.gz` & `tmp/nlpx-1.2.8.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "nlpx-1.2.7.tar", last modified: Wed May 29 06:01:41 2024, max compression
+gzip compressed data, was "nlpx-1.2.8.tar", last modified: Wed May 29 06:21:27 2024, max compression
```

## Comparing `nlpx-1.2.7.tar` & `nlpx-1.2.8.tar`

### file list

```diff
@@ -1,26 +1,26 @@
-drwxr-xr-x   0 summy      (501) staff       (20)        0 2024-05-29 06:01:41.115899 nlpx-1.2.7/
--rw-r--r--   0 summy      (501) staff       (20)      730 2024-05-29 06:01:41.115192 nlpx-1.2.7/PKG-INFO
--rw-r--r--   0 summy      (501) staff       (20)      448 2024-04-07 01:09:43.000000 nlpx-1.2.7/README.rst
-drwxr-xr-x   0 summy      (501) staff       (20)        0 2024-05-29 06:01:41.086156 nlpx-1.2.7/nlpx/
--rw-r--r--   0 summy      (501) staff       (20)        0 2024-05-21 11:15:55.000000 nlpx-1.2.7/nlpx/__init__.py
-drwxr-xr-x   0 summy      (501) staff       (20)        0 2024-05-29 06:01:41.098736 nlpx-1.2.7/nlpx/llm/
--rw-r--r--   0 summy      (501) staff       (20)      189 2024-05-29 00:08:25.000000 nlpx-1.2.7/nlpx/llm/__init__.py
--rw-r--r--   0 summy      (501) staff       (20)     5604 2024-05-29 00:43:58.000000 nlpx-1.2.7/nlpx/llm/_model_wrapper.py
--rw-r--r--   0 summy      (501) staff       (20)    10270 2024-05-29 00:33:21.000000 nlpx-1.2.7/nlpx/llm/_tokenize_vec.py
--rw-r--r--   0 summy      (501) staff       (20)     2384 2024-05-29 06:01:29.000000 nlpx-1.2.7/nlpx/llm/_utils.py
-drwxr-xr-x   0 summy      (501) staff       (20)        0 2024-05-29 06:01:41.105730 nlpx-1.2.7/nlpx/models/
--rw-r--r--   0 summy      (501) staff       (20)       31 2024-05-24 23:09:44.000000 nlpx-1.2.7/nlpx/models/__init__.py
--rw-r--r--   0 summy      (501) staff       (20)     3848 2024-05-28 13:54:23.000000 nlpx-1.2.7/nlpx/models/_text_cnn.py
-drwxr-xr-x   0 summy      (501) staff       (20)        0 2024-05-29 06:01:41.112847 nlpx-1.2.7/nlpx/text_token/
--rw-r--r--   0 summy      (501) staff       (20)      316 2024-05-26 05:47:41.000000 nlpx-1.2.7/nlpx/text_token/__init__.py
--rw-r--r--   0 summy      (501) staff       (20)    25732 2024-05-26 06:13:27.000000 nlpx-1.2.7/nlpx/text_token/_tokenizer.py
--rw-r--r--   0 summy      (501) staff       (20)    16628 2024-05-26 05:47:41.000000 nlpx-1.2.7/nlpx/text_token/_utils.py
--rw-r--r--   0 summy      (501) staff       (20)     4051 2024-05-28 13:25:28.000000 nlpx-1.2.7/nlpx/training.py
-drwxr-xr-x   0 summy      (501) staff       (20)        0 2024-05-29 06:01:41.091914 nlpx-1.2.7/nlpx.egg-info/
--rw-r--r--   0 summy      (501) staff       (20)      730 2024-05-29 06:01:40.000000 nlpx-1.2.7/nlpx.egg-info/PKG-INFO
--rw-r--r--   0 summy      (501) staff       (20)      418 2024-05-29 06:01:40.000000 nlpx-1.2.7/nlpx.egg-info/SOURCES.txt
--rw-r--r--   0 summy      (501) staff       (20)        1 2024-05-29 06:01:40.000000 nlpx-1.2.7/nlpx.egg-info/dependency_links.txt
--rw-r--r--   0 summy      (501) staff       (20)        1 2024-05-28 13:58:19.000000 nlpx-1.2.7/nlpx.egg-info/not-zip-safe
--rw-r--r--   0 summy      (501) staff       (20)        5 2024-05-29 06:01:40.000000 nlpx-1.2.7/nlpx.egg-info/top_level.txt
--rw-r--r--   0 summy      (501) staff       (20)       38 2024-05-29 06:01:41.116184 nlpx-1.2.7/setup.cfg
--rw-r--r--   0 summy      (501) staff       (20)     1044 2024-05-29 06:01:37.000000 nlpx-1.2.7/setup.py
+drwxr-xr-x   0 summy      (501) staff       (20)        0 2024-05-29 06:21:27.166164 nlpx-1.2.8/
+-rw-r--r--   0 summy      (501) staff       (20)      730 2024-05-29 06:21:27.165466 nlpx-1.2.8/PKG-INFO
+-rw-r--r--   0 summy      (501) staff       (20)      448 2024-04-07 01:09:43.000000 nlpx-1.2.8/README.rst
+drwxr-xr-x   0 summy      (501) staff       (20)        0 2024-05-29 06:21:27.134144 nlpx-1.2.8/nlpx/
+-rw-r--r--   0 summy      (501) staff       (20)        0 2024-05-21 11:15:55.000000 nlpx-1.2.8/nlpx/__init__.py
+drwxr-xr-x   0 summy      (501) staff       (20)        0 2024-05-29 06:21:27.147642 nlpx-1.2.8/nlpx/llm/
+-rw-r--r--   0 summy      (501) staff       (20)      189 2024-05-29 00:08:25.000000 nlpx-1.2.8/nlpx/llm/__init__.py
+-rw-r--r--   0 summy      (501) staff       (20)     5604 2024-05-29 00:43:58.000000 nlpx-1.2.8/nlpx/llm/_model_wrapper.py
+-rw-r--r--   0 summy      (501) staff       (20)    10270 2024-05-29 00:33:21.000000 nlpx-1.2.8/nlpx/llm/_tokenize_vec.py
+-rw-r--r--   0 summy      (501) staff       (20)     2383 2024-05-29 06:21:14.000000 nlpx-1.2.8/nlpx/llm/_utils.py
+drwxr-xr-x   0 summy      (501) staff       (20)        0 2024-05-29 06:21:27.150219 nlpx-1.2.8/nlpx/models/
+-rw-r--r--   0 summy      (501) staff       (20)       31 2024-05-24 23:09:44.000000 nlpx-1.2.8/nlpx/models/__init__.py
+-rw-r--r--   0 summy      (501) staff       (20)     3848 2024-05-28 13:54:23.000000 nlpx-1.2.8/nlpx/models/_text_cnn.py
+drwxr-xr-x   0 summy      (501) staff       (20)        0 2024-05-29 06:21:27.162425 nlpx-1.2.8/nlpx/text_token/
+-rw-r--r--   0 summy      (501) staff       (20)      316 2024-05-26 05:47:41.000000 nlpx-1.2.8/nlpx/text_token/__init__.py
+-rw-r--r--   0 summy      (501) staff       (20)    25732 2024-05-26 06:13:27.000000 nlpx-1.2.8/nlpx/text_token/_tokenizer.py
+-rw-r--r--   0 summy      (501) staff       (20)    16628 2024-05-26 05:47:41.000000 nlpx-1.2.8/nlpx/text_token/_utils.py
+-rw-r--r--   0 summy      (501) staff       (20)     4051 2024-05-28 13:25:28.000000 nlpx-1.2.8/nlpx/training.py
+drwxr-xr-x   0 summy      (501) staff       (20)        0 2024-05-29 06:21:27.140405 nlpx-1.2.8/nlpx.egg-info/
+-rw-r--r--   0 summy      (501) staff       (20)      730 2024-05-29 06:21:26.000000 nlpx-1.2.8/nlpx.egg-info/PKG-INFO
+-rw-r--r--   0 summy      (501) staff       (20)      418 2024-05-29 06:21:27.000000 nlpx-1.2.8/nlpx.egg-info/SOURCES.txt
+-rw-r--r--   0 summy      (501) staff       (20)        1 2024-05-29 06:21:26.000000 nlpx-1.2.8/nlpx.egg-info/dependency_links.txt
+-rw-r--r--   0 summy      (501) staff       (20)        1 2024-05-28 13:58:19.000000 nlpx-1.2.8/nlpx.egg-info/not-zip-safe
+-rw-r--r--   0 summy      (501) staff       (20)        5 2024-05-29 06:21:26.000000 nlpx-1.2.8/nlpx.egg-info/top_level.txt
+-rw-r--r--   0 summy      (501) staff       (20)       38 2024-05-29 06:21:27.166419 nlpx-1.2.8/setup.cfg
+-rw-r--r--   0 summy      (501) staff       (20)     1044 2024-05-29 06:21:23.000000 nlpx-1.2.8/setup.py
```

### Comparing `nlpx-1.2.7/PKG-INFO` & `nlpx-1.2.8/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: nlpx
-Version: 1.2.7
+Version: 1.2.8
 Summary: A tool set for NLP.
 Home-page: https://gitee.com/summry/nlpx
 Author: summy
 Author-email: xiazhongbiao@126.com
 License: UNKNOWN
 Keywords: NLP
 Platform: UNKNOWN
```

### Comparing `nlpx-1.2.7/nlpx/llm/_model_wrapper.py` & `nlpx-1.2.8/nlpx/llm/_model_wrapper.py`

 * *Files identical despite different names*

### Comparing `nlpx-1.2.7/nlpx/llm/_tokenize_vec.py` & `nlpx-1.2.8/nlpx/llm/_tokenize_vec.py`

 * *Files identical despite different names*

### Comparing `nlpx-1.2.7/nlpx/llm/_utils.py` & `nlpx-1.2.8/nlpx/llm/_utils.py`

 * *Files 1% similar despite different names*

```diff
@@ -17,15 +17,15 @@
         y_train = torch.tensor(y_train, dtype=torch.long)
 
     X_test = tokenize_vec.parallel_encode_plus(test_texts, max_length=max_length, padding='max_length',
                                                 truncation=True, add_special_tokens=True,
                                                 return_token_type_ids=True, return_attention_mask=True,
                                                 return_tensors='pt', n_jobs=n_jobs)
     if isinstance(y_test, List) or isinstance(y_test, np.ndarray):
-        y_test = torch.tensor(y_train, dtype=torch.long)
+        y_test = torch.tensor(y_test, dtype=torch.long)
     return TensorDataset(X_train, y_train), TensorDataset(X_test, y_test)
 
 
 def train_test_split_set(tokenize_vec: TokenizeVec, texts: List[str], y: Union[torch.LongTensor, List, np.ndarray],
                          max_length: int = 0, test_size=0.2, n_jobs=-1, random_state=None):
     X = tokenize_vec.parallel_encode_plus(texts, max_length=max_length, padding='max_length',
                                         truncation=True, add_special_tokens=True,
```

### Comparing `nlpx-1.2.7/nlpx/models/_text_cnn.py` & `nlpx-1.2.8/nlpx/models/_text_cnn.py`

 * *Files identical despite different names*

### Comparing `nlpx-1.2.7/nlpx/text_token/_tokenizer.py` & `nlpx-1.2.8/nlpx/text_token/_tokenizer.py`

 * *Files identical despite different names*

### Comparing `nlpx-1.2.7/nlpx/text_token/_utils.py` & `nlpx-1.2.8/nlpx/text_token/_utils.py`

 * *Files identical despite different names*

### Comparing `nlpx-1.2.7/nlpx/training.py` & `nlpx-1.2.8/nlpx/training.py`

 * *Files identical despite different names*

### Comparing `nlpx-1.2.7/nlpx.egg-info/PKG-INFO` & `nlpx-1.2.8/nlpx.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: nlpx
-Version: 1.2.7
+Version: 1.2.8
 Summary: A tool set for NLP.
 Home-page: https://gitee.com/summry/nlpx
 Author: summy
 Author-email: xiazhongbiao@126.com
 License: UNKNOWN
 Keywords: NLP
 Platform: UNKNOWN
```

### Comparing `nlpx-1.2.7/setup.py` & `nlpx-1.2.8/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -16,15 +16,15 @@
 
 setup(
     name='nlpx',
     packages=['nlpx', 'nlpx.models', 'nlpx.llm', 'nlpx.text_token'],
     description="A tool set for NLP.",
     long_description=long_description,
     long_description_content_type='text/markdown',
-    version='1.2.7',
+    version='1.2.8',
     url='https://gitee.com/summry/nlpx',
     author='summy',
     author_email='xiazhongbiao@126.com',
     keywords=['NLP'],
     package_data={
         # include json and txt files
         '': ['*.rst', '*.dtd', '*.tpl'],
```

