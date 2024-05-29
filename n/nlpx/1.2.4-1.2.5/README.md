# Comparing `tmp/nlpx-1.2.4.tar.gz` & `tmp/nlpx-1.2.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "nlpx-1.2.4.tar", last modified: Tue May 28 13:58:19 2024, max compression
+gzip compressed data, was "nlpx-1.2.5.tar", last modified: Tue May 28 14:09:56 2024, max compression
```

## Comparing `nlpx-1.2.4.tar` & `nlpx-1.2.5.tar`

### file list

```diff
@@ -1,25 +1,25 @@
-drwxr-xr-x   0 summy      (501) staff       (20)        0 2024-05-28 13:58:19.248755 nlpx-1.2.4/
--rw-r--r--   0 summy      (501) staff       (20)      730 2024-05-28 13:58:19.248063 nlpx-1.2.4/PKG-INFO
--rw-r--r--   0 summy      (501) staff       (20)      448 2024-04-07 01:09:43.000000 nlpx-1.2.4/README.rst
-drwxr-xr-x   0 summy      (501) staff       (20)        0 2024-05-28 13:58:19.218073 nlpx-1.2.4/nlpx/
--rw-r--r--   0 summy      (501) staff       (20)        0 2024-05-21 11:15:55.000000 nlpx-1.2.4/nlpx/__init__.py
-drwxr-xr-x   0 summy      (501) staff       (20)        0 2024-05-28 13:58:19.228086 nlpx-1.2.4/nlpx/llm/
--rw-r--r--   0 summy      (501) staff       (20)      141 2024-05-28 01:07:01.000000 nlpx-1.2.4/nlpx/llm/__init__.py
--rw-r--r--   0 summy      (501) staff       (20)     6384 2024-05-28 01:52:12.000000 nlpx-1.2.4/nlpx/llm/_model_wrapper.py
--rw-r--r--   0 summy      (501) staff       (20)     8588 2024-05-28 03:14:40.000000 nlpx-1.2.4/nlpx/llm/_tokenize_vec.py
-drwxr-xr-x   0 summy      (501) staff       (20)        0 2024-05-28 13:58:19.232347 nlpx-1.2.4/nlpx/models/
--rw-r--r--   0 summy      (501) staff       (20)       31 2024-05-24 23:09:44.000000 nlpx-1.2.4/nlpx/models/__init__.py
--rw-r--r--   0 summy      (501) staff       (20)     3848 2024-05-28 13:54:23.000000 nlpx-1.2.4/nlpx/models/_text_cnn.py
-drwxr-xr-x   0 summy      (501) staff       (20)        0 2024-05-28 13:58:19.239973 nlpx-1.2.4/nlpx/text_token/
--rw-r--r--   0 summy      (501) staff       (20)      316 2024-05-26 05:47:41.000000 nlpx-1.2.4/nlpx/text_token/__init__.py
--rw-r--r--   0 summy      (501) staff       (20)    25732 2024-05-26 06:13:27.000000 nlpx-1.2.4/nlpx/text_token/_tokenizer.py
--rw-r--r--   0 summy      (501) staff       (20)    16628 2024-05-26 05:47:41.000000 nlpx-1.2.4/nlpx/text_token/_utils.py
--rw-r--r--   0 summy      (501) staff       (20)     4051 2024-05-28 13:25:28.000000 nlpx-1.2.4/nlpx/training.py
-drwxr-xr-x   0 summy      (501) staff       (20)        0 2024-05-28 13:58:19.222675 nlpx-1.2.4/nlpx.egg-info/
--rw-r--r--   0 summy      (501) staff       (20)      730 2024-05-28 13:58:19.000000 nlpx-1.2.4/nlpx.egg-info/PKG-INFO
--rw-r--r--   0 summy      (501) staff       (20)      399 2024-05-28 13:58:19.000000 nlpx-1.2.4/nlpx.egg-info/SOURCES.txt
--rw-r--r--   0 summy      (501) staff       (20)        1 2024-05-28 13:58:19.000000 nlpx-1.2.4/nlpx.egg-info/dependency_links.txt
--rw-r--r--   0 summy      (501) staff       (20)        1 2024-05-28 13:58:19.000000 nlpx-1.2.4/nlpx.egg-info/not-zip-safe
--rw-r--r--   0 summy      (501) staff       (20)        5 2024-05-28 13:58:19.000000 nlpx-1.2.4/nlpx.egg-info/top_level.txt
--rw-r--r--   0 summy      (501) staff       (20)       38 2024-05-28 13:58:19.249003 nlpx-1.2.4/setup.cfg
--rw-r--r--   0 summy      (501) staff       (20)     1044 2024-05-28 13:58:13.000000 nlpx-1.2.4/setup.py
+drwxr-xr-x   0 summy      (501) staff       (20)        0 2024-05-28 14:09:56.486717 nlpx-1.2.5/
+-rw-r--r--   0 summy      (501) staff       (20)      730 2024-05-28 14:09:56.485911 nlpx-1.2.5/PKG-INFO
+-rw-r--r--   0 summy      (501) staff       (20)      448 2024-04-07 01:09:43.000000 nlpx-1.2.5/README.rst
+drwxr-xr-x   0 summy      (501) staff       (20)        0 2024-05-28 14:09:56.455032 nlpx-1.2.5/nlpx/
+-rw-r--r--   0 summy      (501) staff       (20)        0 2024-05-21 11:15:55.000000 nlpx-1.2.5/nlpx/__init__.py
+drwxr-xr-x   0 summy      (501) staff       (20)        0 2024-05-28 14:09:56.468994 nlpx-1.2.5/nlpx/llm/
+-rw-r--r--   0 summy      (501) staff       (20)      141 2024-05-28 01:07:01.000000 nlpx-1.2.5/nlpx/llm/__init__.py
+-rw-r--r--   0 summy      (501) staff       (20)     6404 2024-05-28 14:08:34.000000 nlpx-1.2.5/nlpx/llm/_model_wrapper.py
+-rw-r--r--   0 summy      (501) staff       (20)     8588 2024-05-28 03:14:40.000000 nlpx-1.2.5/nlpx/llm/_tokenize_vec.py
+drwxr-xr-x   0 summy      (501) staff       (20)        0 2024-05-28 14:09:56.473971 nlpx-1.2.5/nlpx/models/
+-rw-r--r--   0 summy      (501) staff       (20)       31 2024-05-24 23:09:44.000000 nlpx-1.2.5/nlpx/models/__init__.py
+-rw-r--r--   0 summy      (501) staff       (20)     3848 2024-05-28 13:54:23.000000 nlpx-1.2.5/nlpx/models/_text_cnn.py
+drwxr-xr-x   0 summy      (501) staff       (20)        0 2024-05-28 14:09:56.479776 nlpx-1.2.5/nlpx/text_token/
+-rw-r--r--   0 summy      (501) staff       (20)      316 2024-05-26 05:47:41.000000 nlpx-1.2.5/nlpx/text_token/__init__.py
+-rw-r--r--   0 summy      (501) staff       (20)    25732 2024-05-26 06:13:27.000000 nlpx-1.2.5/nlpx/text_token/_tokenizer.py
+-rw-r--r--   0 summy      (501) staff       (20)    16628 2024-05-26 05:47:41.000000 nlpx-1.2.5/nlpx/text_token/_utils.py
+-rw-r--r--   0 summy      (501) staff       (20)     4051 2024-05-28 13:25:28.000000 nlpx-1.2.5/nlpx/training.py
+drwxr-xr-x   0 summy      (501) staff       (20)        0 2024-05-28 14:09:56.465049 nlpx-1.2.5/nlpx.egg-info/
+-rw-r--r--   0 summy      (501) staff       (20)      730 2024-05-28 14:09:56.000000 nlpx-1.2.5/nlpx.egg-info/PKG-INFO
+-rw-r--r--   0 summy      (501) staff       (20)      399 2024-05-28 14:09:56.000000 nlpx-1.2.5/nlpx.egg-info/SOURCES.txt
+-rw-r--r--   0 summy      (501) staff       (20)        1 2024-05-28 14:09:56.000000 nlpx-1.2.5/nlpx.egg-info/dependency_links.txt
+-rw-r--r--   0 summy      (501) staff       (20)        1 2024-05-28 13:58:19.000000 nlpx-1.2.5/nlpx.egg-info/not-zip-safe
+-rw-r--r--   0 summy      (501) staff       (20)        5 2024-05-28 14:09:56.000000 nlpx-1.2.5/nlpx.egg-info/top_level.txt
+-rw-r--r--   0 summy      (501) staff       (20)       38 2024-05-28 14:09:56.486961 nlpx-1.2.5/setup.cfg
+-rw-r--r--   0 summy      (501) staff       (20)     1044 2024-05-28 14:09:53.000000 nlpx-1.2.5/setup.py
```

### Comparing `nlpx-1.2.4/PKG-INFO` & `nlpx-1.2.5/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: nlpx
-Version: 1.2.4
+Version: 1.2.5
 Summary: A tool set for NLP.
 Home-page: https://gitee.com/summry/nlpx
 Author: summy
 Author-email: xiazhongbiao@126.com
 License: UNKNOWN
 Keywords: NLP
 Platform: UNKNOWN
```

### Comparing `nlpx-1.2.4/nlpx/llm/_model_wrapper.py` & `nlpx-1.2.5/nlpx/llm/_model_wrapper.py`

 * *Files 2% similar despite different names*

```diff
@@ -127,15 +127,15 @@
 		eval_set = TensorDataset(X, y)
 		return super().evaluate(eval_set, batch_size=batch_size, num_workers=num_workers, collate_fn=collate_fn)
 
 	@staticmethod
 	def get_max_length(texts: List[str], max_length: int = 0) -> int:
 		if max_length and max_length > 0:
 			return max_length
-		return get_texts_max_length(texts, cut_type='char')
+		return get_texts_max_length(texts, cut_type='char') + 2  # 开头结尾
 
 	def get_vec(self, texts: List[str], max_length: int, n_jobs: int):
 		if n_jobs == 0:
 			return self.tokenize_vec.encode_plus(texts, max_length=max_length, padding='max_length',
 												  truncation=True, add_special_tokens=True,
 												  return_token_type_ids=True, return_attention_mask=True,
 												  return_tensors='pt')
```

### Comparing `nlpx-1.2.4/nlpx/llm/_tokenize_vec.py` & `nlpx-1.2.5/nlpx/llm/_tokenize_vec.py`

 * *Files identical despite different names*

### Comparing `nlpx-1.2.4/nlpx/models/_text_cnn.py` & `nlpx-1.2.5/nlpx/models/_text_cnn.py`

 * *Files identical despite different names*

### Comparing `nlpx-1.2.4/nlpx/text_token/_tokenizer.py` & `nlpx-1.2.5/nlpx/text_token/_tokenizer.py`

 * *Files identical despite different names*

### Comparing `nlpx-1.2.4/nlpx/text_token/_utils.py` & `nlpx-1.2.5/nlpx/text_token/_utils.py`

 * *Files identical despite different names*

### Comparing `nlpx-1.2.4/nlpx/training.py` & `nlpx-1.2.5/nlpx/training.py`

 * *Files identical despite different names*

### Comparing `nlpx-1.2.4/nlpx.egg-info/PKG-INFO` & `nlpx-1.2.5/nlpx.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: nlpx
-Version: 1.2.4
+Version: 1.2.5
 Summary: A tool set for NLP.
 Home-page: https://gitee.com/summry/nlpx
 Author: summy
 Author-email: xiazhongbiao@126.com
 License: UNKNOWN
 Keywords: NLP
 Platform: UNKNOWN
```

### Comparing `nlpx-1.2.4/setup.py` & `nlpx-1.2.5/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -16,15 +16,15 @@
 
 setup(
     name='nlpx',
     packages=['nlpx', 'nlpx.models', 'nlpx.llm', 'nlpx.text_token'],
     description="A tool set for NLP.",
     long_description=long_description,
     long_description_content_type='text/markdown',
-    version='1.2.4',
+    version='1.2.5',
     url='https://gitee.com/summry/nlpx',
     author='summy',
     author_email='xiazhongbiao@126.com',
     keywords=['NLP'],
     package_data={
         # include json and txt files
         '': ['*.rst', '*.dtd', '*.tpl'],
```

