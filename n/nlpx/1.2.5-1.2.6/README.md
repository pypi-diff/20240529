# Comparing `tmp/nlpx-1.2.5.tar.gz` & `tmp/nlpx-1.2.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "nlpx-1.2.5.tar", last modified: Tue May 28 14:09:56 2024, max compression
+gzip compressed data, was "nlpx-1.2.6.tar", last modified: Wed May 29 00:50:54 2024, max compression
```

## Comparing `nlpx-1.2.5.tar` & `nlpx-1.2.6.tar`

### file list

```diff
@@ -1,25 +1,26 @@
-drwxr-xr-x   0 summy      (501) staff       (20)        0 2024-05-28 14:09:56.486717 nlpx-1.2.5/
--rw-r--r--   0 summy      (501) staff       (20)      730 2024-05-28 14:09:56.485911 nlpx-1.2.5/PKG-INFO
--rw-r--r--   0 summy      (501) staff       (20)      448 2024-04-07 01:09:43.000000 nlpx-1.2.5/README.rst
-drwxr-xr-x   0 summy      (501) staff       (20)        0 2024-05-28 14:09:56.455032 nlpx-1.2.5/nlpx/
--rw-r--r--   0 summy      (501) staff       (20)        0 2024-05-21 11:15:55.000000 nlpx-1.2.5/nlpx/__init__.py
-drwxr-xr-x   0 summy      (501) staff       (20)        0 2024-05-28 14:09:56.468994 nlpx-1.2.5/nlpx/llm/
--rw-r--r--   0 summy      (501) staff       (20)      141 2024-05-28 01:07:01.000000 nlpx-1.2.5/nlpx/llm/__init__.py
--rw-r--r--   0 summy      (501) staff       (20)     6404 2024-05-28 14:08:34.000000 nlpx-1.2.5/nlpx/llm/_model_wrapper.py
--rw-r--r--   0 summy      (501) staff       (20)     8588 2024-05-28 03:14:40.000000 nlpx-1.2.5/nlpx/llm/_tokenize_vec.py
-drwxr-xr-x   0 summy      (501) staff       (20)        0 2024-05-28 14:09:56.473971 nlpx-1.2.5/nlpx/models/
--rw-r--r--   0 summy      (501) staff       (20)       31 2024-05-24 23:09:44.000000 nlpx-1.2.5/nlpx/models/__init__.py
--rw-r--r--   0 summy      (501) staff       (20)     3848 2024-05-28 13:54:23.000000 nlpx-1.2.5/nlpx/models/_text_cnn.py
-drwxr-xr-x   0 summy      (501) staff       (20)        0 2024-05-28 14:09:56.479776 nlpx-1.2.5/nlpx/text_token/
--rw-r--r--   0 summy      (501) staff       (20)      316 2024-05-26 05:47:41.000000 nlpx-1.2.5/nlpx/text_token/__init__.py
--rw-r--r--   0 summy      (501) staff       (20)    25732 2024-05-26 06:13:27.000000 nlpx-1.2.5/nlpx/text_token/_tokenizer.py
--rw-r--r--   0 summy      (501) staff       (20)    16628 2024-05-26 05:47:41.000000 nlpx-1.2.5/nlpx/text_token/_utils.py
--rw-r--r--   0 summy      (501) staff       (20)     4051 2024-05-28 13:25:28.000000 nlpx-1.2.5/nlpx/training.py
-drwxr-xr-x   0 summy      (501) staff       (20)        0 2024-05-28 14:09:56.465049 nlpx-1.2.5/nlpx.egg-info/
--rw-r--r--   0 summy      (501) staff       (20)      730 2024-05-28 14:09:56.000000 nlpx-1.2.5/nlpx.egg-info/PKG-INFO
--rw-r--r--   0 summy      (501) staff       (20)      399 2024-05-28 14:09:56.000000 nlpx-1.2.5/nlpx.egg-info/SOURCES.txt
--rw-r--r--   0 summy      (501) staff       (20)        1 2024-05-28 14:09:56.000000 nlpx-1.2.5/nlpx.egg-info/dependency_links.txt
--rw-r--r--   0 summy      (501) staff       (20)        1 2024-05-28 13:58:19.000000 nlpx-1.2.5/nlpx.egg-info/not-zip-safe
--rw-r--r--   0 summy      (501) staff       (20)        5 2024-05-28 14:09:56.000000 nlpx-1.2.5/nlpx.egg-info/top_level.txt
--rw-r--r--   0 summy      (501) staff       (20)       38 2024-05-28 14:09:56.486961 nlpx-1.2.5/setup.cfg
--rw-r--r--   0 summy      (501) staff       (20)     1044 2024-05-28 14:09:53.000000 nlpx-1.2.5/setup.py
+drwxr-xr-x   0 summy      (501) staff       (20)        0 2024-05-29 00:50:54.490615 nlpx-1.2.6/
+-rw-r--r--   0 summy      (501) staff       (20)      730 2024-05-29 00:50:54.490123 nlpx-1.2.6/PKG-INFO
+-rw-r--r--   0 summy      (501) staff       (20)      448 2024-04-07 01:09:43.000000 nlpx-1.2.6/README.rst
+drwxr-xr-x   0 summy      (501) staff       (20)        0 2024-05-29 00:50:54.464050 nlpx-1.2.6/nlpx/
+-rw-r--r--   0 summy      (501) staff       (20)        0 2024-05-21 11:15:55.000000 nlpx-1.2.6/nlpx/__init__.py
+drwxr-xr-x   0 summy      (501) staff       (20)        0 2024-05-29 00:50:54.478671 nlpx-1.2.6/nlpx/llm/
+-rw-r--r--   0 summy      (501) staff       (20)      189 2024-05-29 00:08:25.000000 nlpx-1.2.6/nlpx/llm/__init__.py
+-rw-r--r--   0 summy      (501) staff       (20)     5604 2024-05-29 00:43:58.000000 nlpx-1.2.6/nlpx/llm/_model_wrapper.py
+-rw-r--r--   0 summy      (501) staff       (20)    10270 2024-05-29 00:33:21.000000 nlpx-1.2.6/nlpx/llm/_tokenize_vec.py
+-rw-r--r--   0 summy      (501) staff       (20)     1016 2024-05-29 00:01:18.000000 nlpx-1.2.6/nlpx/llm/_utils.py
+drwxr-xr-x   0 summy      (501) staff       (20)        0 2024-05-29 00:50:54.482209 nlpx-1.2.6/nlpx/models/
+-rw-r--r--   0 summy      (501) staff       (20)       31 2024-05-24 23:09:44.000000 nlpx-1.2.6/nlpx/models/__init__.py
+-rw-r--r--   0 summy      (501) staff       (20)     3848 2024-05-28 13:54:23.000000 nlpx-1.2.6/nlpx/models/_text_cnn.py
+drwxr-xr-x   0 summy      (501) staff       (20)        0 2024-05-29 00:50:54.487502 nlpx-1.2.6/nlpx/text_token/
+-rw-r--r--   0 summy      (501) staff       (20)      316 2024-05-26 05:47:41.000000 nlpx-1.2.6/nlpx/text_token/__init__.py
+-rw-r--r--   0 summy      (501) staff       (20)    25732 2024-05-26 06:13:27.000000 nlpx-1.2.6/nlpx/text_token/_tokenizer.py
+-rw-r--r--   0 summy      (501) staff       (20)    16628 2024-05-26 05:47:41.000000 nlpx-1.2.6/nlpx/text_token/_utils.py
+-rw-r--r--   0 summy      (501) staff       (20)     4051 2024-05-28 13:25:28.000000 nlpx-1.2.6/nlpx/training.py
+drwxr-xr-x   0 summy      (501) staff       (20)        0 2024-05-29 00:50:54.470162 nlpx-1.2.6/nlpx.egg-info/
+-rw-r--r--   0 summy      (501) staff       (20)      730 2024-05-29 00:50:54.000000 nlpx-1.2.6/nlpx.egg-info/PKG-INFO
+-rw-r--r--   0 summy      (501) staff       (20)      418 2024-05-29 00:50:54.000000 nlpx-1.2.6/nlpx.egg-info/SOURCES.txt
+-rw-r--r--   0 summy      (501) staff       (20)        1 2024-05-29 00:50:54.000000 nlpx-1.2.6/nlpx.egg-info/dependency_links.txt
+-rw-r--r--   0 summy      (501) staff       (20)        1 2024-05-28 13:58:19.000000 nlpx-1.2.6/nlpx.egg-info/not-zip-safe
+-rw-r--r--   0 summy      (501) staff       (20)        5 2024-05-29 00:50:54.000000 nlpx-1.2.6/nlpx.egg-info/top_level.txt
+-rw-r--r--   0 summy      (501) staff       (20)       38 2024-05-29 00:50:54.490780 nlpx-1.2.6/setup.cfg
+-rw-r--r--   0 summy      (501) staff       (20)     1044 2024-05-29 00:20:06.000000 nlpx-1.2.6/setup.py
```

### Comparing `nlpx-1.2.5/PKG-INFO` & `nlpx-1.2.6/PKG-INFO`

 * *Files 14% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: nlpx
-Version: 1.2.5
+Version: 1.2.6
 Summary: A tool set for NLP.
 Home-page: https://gitee.com/summry/nlpx
 Author: summy
 Author-email: xiazhongbiao@126.com
 License: UNKNOWN
 Keywords: NLP
 Platform: UNKNOWN
```

### Comparing `nlpx-1.2.5/nlpx/llm/_model_wrapper.py` & `nlpx-1.2.6/nlpx/llm/_model_wrapper.py`

 * *Files 16% similar despite different names*

```diff
@@ -2,32 +2,32 @@
 import numpy as np
 from torch import optim
 from pathlib import Path
 from typing import Union, List
 from torch.nn import functional as F
 from torch.utils.data import DataLoader, TensorDataset, Dataset
 
-from nlpx.text_token import get_texts_max_length
 from nlpx.training import Trainer, SimpleTrainer, evaluate
+from ._tokenize_vec import TokenizeVec
 
 
 class ModelWrapper:
 
-	def __init__(self, model_path: Union[str, Path], classes: List[str] = None,
+	def __init__(self, model_path: Union[str, Path] = None, classes: List[str] = None,
 					device=torch.device('cuda:0' if torch.cuda.is_available() else 'cpu')):
 		self.classes = classes
 		self.device = device
 		self.model = torch.load(model_path, map_location=device) if model_path else None
 
-	def train(self, train_set: Dataset, eval_set: Dataset, collate_fn=None, max_iter=100,
+	def train(self, model, train_set: Dataset, eval_set: Dataset, collate_fn=None, max_iter=100,
 				optimizer=optim.AdamW, learning_rate=0.001, T_max: int = 0,
 				batch_size=8, eval_batch_size=16,
 				num_workers=4, num_eval_workers=2,
 				early_stopping_rounds=10):
-		trainer = Trainer(self.model, train_set, eval_set, collate_fn,
+		trainer = Trainer(model, train_set, eval_set, collate_fn,
 						  max_iter, optimizer, learning_rate, T_max,
 						  batch_size, eval_batch_size,
 						  num_workers, num_eval_workers,
 						  early_stopping_rounds,  # 早停，等10轮决策，评价指标不在变化，停止
 						  self.device)
 		self.model = trainer.train()
 
@@ -43,17 +43,16 @@
 	def predict_proba(self, X: torch.FloatTensor):
 		logits = self.logits(X)
 		result = F.softmax(logits, dim=1).max(1)
 		return result.indices, result.values
 
 	def predict_classes_proba(self, X: torch.FloatTensor):
 		assert self.classes is not None, 'classes must be specified'
-		logits = self.logits(X)
-		result = F.softmax(logits).max(1)
-		return [self.classes[i] for i in result.indices.detach().numpy().ravel()], result.values
+		indices, values = self.predict_proba(X)
+		return [self.classes[i] for i in indices.detach().numpy().ravel()], values
 
 	def logits(self, X: torch.FloatTensor):
 		self.model.eval()
 		with torch.no_grad():
 			logits = self.model(X)
 		return logits
 
@@ -68,83 +67,66 @@
 
 	def load(self, model_path: Union[str, Path] = './best_model.pt'):
 		self.model = torch.load(model_path, map_location=self.device)
 
 
 class SimpleModelWrapper(ModelWrapper):
 
-	def __init__(self, tokenize_vec, model_path: Union[str, Path] = None, classes: List[str] = None,
-					device=torch.device('cuda:0' if torch.cuda.is_available() else 'cpu')):
+	def __init__(self, tokenize_vec: TokenizeVec, model_path: Union[str, Path] = None, classes: List[str] = None,
+				device=torch.device('cuda:0' if torch.cuda.is_available() else 'cpu')):
 		super().__init__(model_path, classes, device)
 		self.tokenize_vec = tokenize_vec
 
 	def train(self, model, texts: List[str], y: Union[torch.LongTensor, List, np.ndarray], max_length: int = 0,
 			  eval_size=0.2, random_state=None, collate_fn=None,max_iter=100,
 			  optimizer=optim.AdamW, learning_rate=0.001, T_max: int = 0,
 			  batch_size=8, eval_batch_size=16,
 			  num_workers=4, num_eval_workers=2,
 			  early_stopping_rounds=10, n_jobs=-1):
-		max_length = self.get_max_length(texts, max_length)
 		X = self.get_vec(texts, max_length=max_length, n_jobs=n_jobs)
 		if isinstance(y, List) or isinstance(y, np.ndarray):
 			y = torch.tensor(y, dtype=torch.long)
 		trainer = SimpleTrainer(model, X, y, eval_size, random_state, collate_fn,
 								 max_iter, optimizer, learning_rate, T_max,
 								 batch_size, eval_batch_size,
 								 num_workers, num_eval_workers,
 								 early_stopping_rounds,
 								 self.device)
 		self.model = trainer.train()
 
-	def predict(self, texts: List[str], max_length: int = 0, n_jobs=0):
+	def predict(self, texts: List[str], max_length: int = 0, n_jobs=-1):
 		logits = self.logits(texts, max_length, n_jobs=n_jobs)
 		return logits.argmax(1)
 
-	def predict_classes(self, texts: List[str], max_length: int = 0, n_jobs=0):
+	def predict_classes(self, texts: List[str], max_length: int = 0, n_jobs=-1):
 		assert self.classes is not None, 'classes must be specified'
 		pred = self.predict(texts, max_length, n_jobs=n_jobs)
 		return [self.classes[i] for i in pred.detach().numpy().ravel()]
 	
-	def predict_proba(self, texts: List[str], max_length: int = 0, n_jobs=0):
+	def predict_proba(self, texts: List[str], max_length: int = 0, n_jobs=-1):
 		logits = self.logits(texts, max_length, n_jobs=n_jobs)
-		result = F.softmax(logits).max(1)
+		result = F.softmax(logits, dim=1).max(1)
 		return result.indices, result.values
 
-	def predict_classes_proba(self, texts: List[str], max_length: int = 0, n_jobs=0):
+	def predict_classes_proba(self, texts: List[str], max_length: int = 0, n_jobs=-1):
 		assert self.classes is not None, 'classes must be specified'
-		logits = self.logits(texts, max_length)
-		result = F.softmax(logits, dim=1).max(1)
-		return [self.classes[i] for i in result.indices.detach().numpy().ravel()], result.values
+		indices, values = self.predict_proba(texts, max_length, n_jobs)
+		return [self.classes[i] for i in indices.detach().numpy().ravel()], values
 
 	def logits(self, texts: List[str], max_length: int = 0, n_jobs=-1):
-		X = self.get_features(texts, max_length, n_jobs=n_jobs)
+		X = self.get_vec(texts, max_length, n_jobs=n_jobs)
 		return super().logits(X)
 
 	def evaluate(self, texts: List[str], y: Union[torch.LongTensor, List, np.ndarray], batch_size=16, num_workers=0,
-				 max_length: int = 0, collate_fn=None, n_jobs=0):
-		X = self.get_features(texts, max_length, n_jobs=n_jobs)
+				 max_length: int = 0, collate_fn=None, n_jobs=-1):
+		X = self.get_vec(texts, max_length, n_jobs=n_jobs)
 		if isinstance(y, List) or isinstance(y, np.ndarray):
 			y = torch.tensor(y, dtype=torch.long)
 		eval_set = TensorDataset(X, y)
 		return super().evaluate(eval_set, batch_size=batch_size, num_workers=num_workers, collate_fn=collate_fn)
 
-	@staticmethod
-	def get_max_length(texts: List[str], max_length: int = 0) -> int:
-		if max_length and max_length > 0:
-			return max_length
-		return get_texts_max_length(texts, cut_type='char') + 2  # 开头结尾
-
 	def get_vec(self, texts: List[str], max_length: int, n_jobs: int):
-		if n_jobs == 0:
-			return self.tokenize_vec.encode_plus(texts, max_length=max_length, padding='max_length',
-												  truncation=True, add_special_tokens=True,
-												  return_token_type_ids=True, return_attention_mask=True,
-												  return_tensors='pt')
-		else:
-			return self.tokenize_vec.parallel_encode_plus(texts, max_length=max_length, padding='max_length',
-															truncation=True, add_special_tokens=True,
-															return_token_type_ids=True,return_attention_mask=True,
-															return_tensors='pt', n_jobs=n_jobs)
-
-	def get_features(self, texts: List[str], max_length: int = 0, n_jobs=0):
-		max_length = self.get_max_length(texts, max_length)
-		return self.get_vec(texts, max_length=max_length, n_jobs=n_jobs)
+		return self.tokenize_vec.parallel_encode_plus(texts, max_length=max_length, padding='max_length',
+														truncation=True, add_special_tokens=True,
+														return_token_type_ids=True,return_attention_mask=True,
+														return_tensors='pt', n_jobs=n_jobs)
+
```

### Comparing `nlpx-1.2.5/nlpx/llm/_tokenize_vec.py` & `nlpx-1.2.6/nlpx/llm/_tokenize_vec.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,83 +1,89 @@
 import torch
 from pathlib import Path
 from joblib import Parallel, delayed
 from typing import Union, List, Optional
 from transformers import BertTokenizer, BertConfig, BertModel, AlbertConfig, AlbertModel, ErnieConfig, ErnieModel
 from transformers.tokenization_utils import PaddingStrategy, TruncationStrategy, TensorType
 
+from nlpx.text_token import get_texts_max_length
+
 
 class TokenizeVec:
 
 	def __init__(self, pretrained_path: Union[str, Path], tokenizer=BertTokenizer):
 		self.config = None
 		self.pretrained = None
 		self.tokenizer = tokenizer.from_pretrained(pretrained_path)
 
 	@property
 	def hidden_size(self):
 		assert self.config is not None, "config must not be None"
 		return self.config.hidden_size
 
+	@staticmethod
+	def get_max_length(texts: List[str], max_length: int = 0) -> int:
+		if max_length and max_length > 0:
+			return max_length
+		return get_texts_max_length(texts, cut_type='char') + 2  # 开头结尾
+
 	def encode_plus(self,
 				texts: List[str],
 				add_special_tokens: bool = True,
-				padding: Union[bool, str, PaddingStrategy] = False,
-				truncation: Union[bool, str, TruncationStrategy] = None,
+				padding: Union[bool, str, PaddingStrategy] = 'max_length',
+				truncation: Union[bool, str, TruncationStrategy] = True,
 				max_length: Optional[int] = None,
 				stride: int = 0,
 				is_split_into_words: bool = False,
 				pad_to_multiple_of: Optional[int] = None,
-				return_tensors: Optional[Union[str, TensorType]] = None,
-				return_token_type_ids: Optional[bool] = None,
-				return_attention_mask: Optional[bool] = None,
+				return_tensors: Optional[Union[str, TensorType]] = 'pt',
+				return_token_type_ids: Optional[bool] = True,
+				return_attention_mask: Optional[bool] = True,
 				return_overflowing_tokens: bool = False,
 				return_special_tokens_mask: bool = False,
 				return_offsets_mapping: bool = False,
 				return_length: bool = False,
 				verbose: bool = True,
 				cls: bool = False,
 				**kwargs,
 			) -> torch.FloatTensor:
-		tokens = self.tokenizer.batch_encode_plus(
-												texts,
-												add_special_tokens,
-												padding,
-												truncation,
-												max_length,
-												stride,
-												is_split_into_words,
-												pad_to_multiple_of,
-												return_tensors,
-												return_token_type_ids,
-												return_attention_mask,
-												return_overflowing_tokens,
-												return_special_tokens_mask,
-												return_offsets_mapping,
-												return_length,
-												verbose,
-												** kwargs
-											)
-		self.pretrained.eval()
-		with torch.no_grad():
-			output = self.pretrained(**tokens, output_hidden_states=True)
-		return output.last_hidden_state[:, 0] if cls else output.last_hidden_state[:, 1:]
+		max_length = self.get_max_length(texts, max_length)
+		return self._encode_plus(
+								texts,
+								add_special_tokens,
+								padding,
+								truncation,
+								max_length,
+								stride,
+								is_split_into_words,
+								pad_to_multiple_of,
+								return_tensors,
+								return_token_type_ids,
+								return_attention_mask,
+								return_overflowing_tokens,
+								return_special_tokens_mask,
+								return_offsets_mapping,
+								return_length,
+								verbose,
+								cls,
+								** kwargs
+							)
 
 	def batch_encode_plus(self,
 						texts: List[str],
 						add_special_tokens: bool = True,
-						padding: Union[bool, str, PaddingStrategy] = False,
-						truncation: Union[bool, str, TruncationStrategy] = None,
+						padding: Union[bool, str, PaddingStrategy] = 'max_length',
+						truncation: Union[bool, str, TruncationStrategy] = True,
 						max_length: Optional[int] = None,
 						stride: int = 0,
 						is_split_into_words: bool = False,
 						pad_to_multiple_of: Optional[int] = None,
-						return_tensors: Optional[Union[str, TensorType]] = None,
-						return_token_type_ids: Optional[bool] = None,
-						return_attention_mask: Optional[bool] = None,
+						return_tensors: Optional[Union[str, TensorType]] = 'pt',
+						return_token_type_ids: Optional[bool] = True,
+						return_attention_mask: Optional[bool] = True,
 						return_overflowing_tokens: bool = False,
 						return_special_tokens_mask: bool = False,
 						return_offsets_mapping: bool = False,
 						return_length: bool = False,
 						verbose: bool = True,
 						cls: bool = False,
 						batch_size: int = 128,
@@ -102,16 +108,17 @@
 									return_offsets_mapping,
 									return_length,
 									verbose,
 									cls,
 									** kwargs
 								)
 		else:
+			max_length = self.get_max_length(texts, max_length)
 			text_list = self.split_texts(texts, batch_size)
-			results = [self.encode_plus(
+			results = [self._encode_plus(
 									text,
 									add_special_tokens,
 									padding,
 									truncation,
 									max_length,
 									stride,
 									is_split_into_words,
@@ -128,23 +135,23 @@
 									** kwargs
 								) for text in text_list]
 			return torch.concat(results, dim=0)
 
 	def parallel_encode_plus(self,
 						texts: List[str],
 						add_special_tokens: bool = True,
-						padding: Union[bool, str, PaddingStrategy] = False,
-						truncation: Union[bool, str, TruncationStrategy] = None,
+						padding: Union[bool, str, PaddingStrategy] = 'max_length',
+						truncation: Union[bool, str, TruncationStrategy] = True,
 						max_length: Optional[int] = None,
 						stride: int = 0,
 						is_split_into_words: bool = False,
 						pad_to_multiple_of: Optional[int] = None,
-						return_tensors: Optional[Union[str, TensorType]] = None,
-						return_token_type_ids: Optional[bool] = None,
-						return_attention_mask: Optional[bool] = None,
+						return_tensors: Optional[Union[str, TensorType]] = 'pt',
+						return_token_type_ids: Optional[bool] = True,
+						return_attention_mask: Optional[bool] = True,
 						return_overflowing_tokens: bool = False,
 						return_special_tokens_mask: bool = False,
 						return_offsets_mapping: bool = False,
 						return_length: bool = False,
 						verbose: bool = True,
 						cls: bool = False,
 						batch_size: int = 128,
@@ -170,14 +177,15 @@
 									return_offsets_mapping,
 									return_length,
 									verbose,
 									cls,
 									** kwargs
 								)
 		else:
+			max_length = self.get_max_length(texts, max_length)
 			text_list = self.split_texts(texts, batch_size)
 			results = Parallel(n_jobs=n_jobs)(
 				delayed(self._order_encode)(i,
 											text,
 											add_special_tokens,
 											padding,
 											truncation,
@@ -242,14 +250,58 @@
 								return_offsets_mapping,
 								return_length,
 								verbose,
 								cls,
 								**kwargs
 							)
 
+	def _encode_plus(self,
+				texts: List[str],
+				add_special_tokens: bool = True,
+				padding: Union[bool, str, PaddingStrategy] = False,
+				truncation: Union[bool, str, TruncationStrategy] = None,
+				max_length: Optional[int] = None,
+				stride: int = 0,
+				is_split_into_words: bool = False,
+				pad_to_multiple_of: Optional[int] = None,
+				return_tensors: Optional[Union[str, TensorType]] = None,
+				return_token_type_ids: Optional[bool] = None,
+				return_attention_mask: Optional[bool] = None,
+				return_overflowing_tokens: bool = False,
+				return_special_tokens_mask: bool = False,
+				return_offsets_mapping: bool = False,
+				return_length: bool = False,
+				verbose: bool = True,
+				cls: bool = False,
+				**kwargs,
+			) -> torch.FloatTensor:
+		tokens = self.tokenizer.batch_encode_plus(
+												texts,
+												add_special_tokens,
+												padding,
+												truncation,
+												max_length,
+												stride,
+												is_split_into_words,
+												pad_to_multiple_of,
+												return_tensors,
+												return_token_type_ids,
+												return_attention_mask,
+												return_overflowing_tokens,
+												return_special_tokens_mask,
+												return_offsets_mapping,
+												return_length,
+												verbose,
+												** kwargs
+											)
+		self.pretrained.eval()
+		with torch.no_grad():
+			output = self.pretrained(**tokens, output_hidden_states=True)
+		return output.last_hidden_state[:, 0] if cls else output.last_hidden_state[:, 1:]
+
 
 class BertTokenizeVec(TokenizeVec):
 
 	def __init__(self, pretrained_path: Union[str, Path]):
 		super().__init__(pretrained_path)
 		self.config = BertConfig.from_pretrained(pretrained_path)
 		self.pretrained = BertModel.from_pretrained(pretrained_path, config=self.config)
```

#### encoding

```diff
@@ -1 +1 @@
-us-ascii
+utf-8
```

### Comparing `nlpx-1.2.5/nlpx/models/_text_cnn.py` & `nlpx-1.2.6/nlpx/models/_text_cnn.py`

 * *Files identical despite different names*

### Comparing `nlpx-1.2.5/nlpx/text_token/_tokenizer.py` & `nlpx-1.2.6/nlpx/text_token/_tokenizer.py`

 * *Files identical despite different names*

### Comparing `nlpx-1.2.5/nlpx/text_token/_utils.py` & `nlpx-1.2.6/nlpx/text_token/_utils.py`

 * *Files identical despite different names*

### Comparing `nlpx-1.2.5/nlpx/training.py` & `nlpx-1.2.6/nlpx/training.py`

 * *Files identical despite different names*

### Comparing `nlpx-1.2.5/nlpx.egg-info/PKG-INFO` & `nlpx-1.2.6/nlpx.egg-info/PKG-INFO`

 * *Files 14% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: nlpx
-Version: 1.2.5
+Version: 1.2.6
 Summary: A tool set for NLP.
 Home-page: https://gitee.com/summry/nlpx
 Author: summy
 Author-email: xiazhongbiao@126.com
 License: UNKNOWN
 Keywords: NLP
 Platform: UNKNOWN
```

### Comparing `nlpx-1.2.5/setup.py` & `nlpx-1.2.6/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -16,15 +16,15 @@
 
 setup(
     name='nlpx',
     packages=['nlpx', 'nlpx.models', 'nlpx.llm', 'nlpx.text_token'],
     description="A tool set for NLP.",
     long_description=long_description,
     long_description_content_type='text/markdown',
-    version='1.2.5',
+    version='1.2.6',
     url='https://gitee.com/summry/nlpx',
     author='summy',
     author_email='xiazhongbiao@126.com',
     keywords=['NLP'],
     package_data={
         # include json and txt files
         '': ['*.rst', '*.dtd', '*.tpl'],
```

