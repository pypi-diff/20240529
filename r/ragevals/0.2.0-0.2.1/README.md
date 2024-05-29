# Comparing `tmp/ragevals-0.2.0.tar.gz` & `tmp/ragevals-0.2.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ragevals-0.2.0.tar", last modified: Tue May 28 07:17:38 2024, max compression
+gzip compressed data, was "ragevals-0.2.1.tar", last modified: Wed May 29 08:07:36 2024, max compression
```

## Comparing `ragevals-0.2.0.tar` & `ragevals-0.2.1.tar`

### file list

```diff
@@ -1,15 +1,15 @@
-drwxrwxrwx   0        0        0        0 2024-05-28 07:17:38.868442 ragevals-0.2.0/
--rw-rw-rw-   0        0        0     2873 2024-05-28 07:17:38.868442 ragevals-0.2.0/PKG-INFO
--rw-rw-rw-   0        0        0     2326 2024-05-28 06:49:40.000000 ragevals-0.2.0/README.md
-drwxrwxrwx   0        0        0        0 2024-05-28 07:17:38.852807 ragevals-0.2.0/ragevals/
--rw-rw-rw-   0        0        0       54 2024-05-27 16:21:14.000000 ragevals-0.2.0/ragevals/__init__.py
--rw-rw-rw-   0        0        0     3798 2024-05-28 07:15:56.000000 ragevals-0.2.0/ragevals/ragevals.py
--rw-rw-rw-   0        0        0      822 2024-05-27 16:29:08.000000 ragevals-0.2.0/ragevals/test_ragevals.py
-drwxrwxrwx   0        0        0        0 2024-05-28 07:17:38.852807 ragevals-0.2.0/ragevals.egg-info/
--rw-rw-rw-   0        0        0     2873 2024-05-28 07:17:38.000000 ragevals-0.2.0/ragevals.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      245 2024-05-28 07:17:38.000000 ragevals-0.2.0/ragevals.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-05-28 07:17:38.000000 ragevals-0.2.0/ragevals.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       66 2024-05-28 07:17:38.000000 ragevals-0.2.0/ragevals.egg-info/requires.txt
--rw-rw-rw-   0        0        0        9 2024-05-28 07:17:38.000000 ragevals-0.2.0/ragevals.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2024-05-28 07:17:38.868442 ragevals-0.2.0/setup.cfg
--rw-rw-rw-   0        0        0      839 2024-05-28 07:16:40.000000 ragevals-0.2.0/setup.py
+drwxrwxrwx   0        0        0        0 2024-05-29 08:07:36.190913 ragevals-0.2.1/
+-rw-rw-rw-   0        0        0     2873 2024-05-29 08:07:36.186347 ragevals-0.2.1/PKG-INFO
+-rw-rw-rw-   0        0        0     2326 2024-05-28 06:49:40.000000 ragevals-0.2.1/README.md
+drwxrwxrwx   0        0        0        0 2024-05-29 08:07:36.170748 ragevals-0.2.1/ragevals/
+-rw-rw-rw-   0        0        0       54 2024-05-27 16:21:14.000000 ragevals-0.2.1/ragevals/__init__.py
+-rw-rw-rw-   0        0        0     3604 2024-05-29 08:03:25.000000 ragevals-0.2.1/ragevals/ragevals.py
+-rw-rw-rw-   0        0        0      822 2024-05-27 16:29:08.000000 ragevals-0.2.1/ragevals/test_ragevals.py
+drwxrwxrwx   0        0        0        0 2024-05-29 08:07:36.180830 ragevals-0.2.1/ragevals.egg-info/
+-rw-rw-rw-   0        0        0     2873 2024-05-29 08:07:35.000000 ragevals-0.2.1/ragevals.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      245 2024-05-29 08:07:36.000000 ragevals-0.2.1/ragevals.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-05-29 08:07:35.000000 ragevals-0.2.1/ragevals.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       66 2024-05-29 08:07:35.000000 ragevals-0.2.1/ragevals.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        9 2024-05-29 08:07:35.000000 ragevals-0.2.1/ragevals.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2024-05-29 08:07:36.190913 ragevals-0.2.1/setup.cfg
+-rw-rw-rw-   0        0        0      839 2024-05-29 08:04:27.000000 ragevals-0.2.1/setup.py
```

### Comparing `ragevals-0.2.0/PKG-INFO` & `ragevals-0.2.1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ragevals
-Version: 0.2.0
+Version: 0.2.1
 Summary: A library for evaluating Retrieval-Augmented Generation (RAG) systems
 Home-page: https://github.com/captainawesome78/RAGevals
 Author: Shaik Naveed
 Author-email: mailmenaveed88@gmail.com
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

### Comparing `ragevals-0.2.0/README.md` & `ragevals-0.2.1/README.md`

 * *Files identical despite different names*

### Comparing `ragevals-0.2.0/ragevals/ragevals.py` & `ragevals-0.2.1/ragevals/ragevals.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,15 +1,16 @@
 import torch
 from sacrebleu import corpus_bleu
 from rouge_score import rouge_scorer
 from bert_score import score
 from transformers import GPT2LMHeadModel, GPT2Tokenizer, pipeline
 import nltk
 from nltk.util import ngrams
-from nltk.translate.meteor_score import meteor_score
+
+
 
 class RAGevals:
     def __init__(self):
         self.gpt2_model, self.gpt2_tokenizer = self.load_gpt2_model()
         self.bias_pipeline =  pipeline("zero-shot-classification", model = "Hate-speech-CNERG/dehatebert-mono-english")
 
     def load_gpt2_model(self):
@@ -21,19 +22,24 @@
         bleu_score = corpus_bleu(candidates, [references]).score
         scorer = rouge_scorer.RougeScorer(['rouge1', 'rouge2', 'rougeL'], use_stemmer=True)
         rouge_scores = [scorer.score(ref, cand) for ref, cand in zip(references, candidates)]
         rouge1 = sum([score['rouge1'].fmeasure for score in rouge_scores]) / len(rouge_scores)
         return bleu_score, rouge1
 
     def evaluate_bert_score(self, candidates, references):
-        P, R, F1 = score(candidates, references, lang ="en", model_type = "bert-base-multilingual-cased")
+        if isinstance(candidates, str):
+            candidates = [candidates]
+        if isinstance(references, str):
+            references = [references]
+        
+        P, R, F1 = score(candidates, references, lang="en", model_type="bert-base-multilingual-cased")
         return P.mean().item(), R.mean().item(), F1.mean().item()
 
     def evaluate_perplexity(self, text):
-        encodings = self.gpt2_tokenizer(text, return_messages= "pt")
+        encodings = self.gpt2_tokenizer(text, return_tensors= "pt")
         max_length = self.gpt2_model.config.n_positions
         stride = 512
         lls = []
         for i in range(0, encodings.input_ids.size(1), stride):
             begin_loc = max(i + stride - max_length, 0)
             end_loc = min(i + stride, encodings.input_ids.size(1))
             trg_len = end_loc - i
@@ -54,31 +60,26 @@
         return diversity_score
     
     def evaluate_racial_bias(self, text):
         results = self.bias_pipeline([text], candidate_labels=["hate speech", "not hate speech"])
         bias_score = results[0]['scores'][results[0]['labels'].index('hate speech')]
         return bias_score
         
-    def evaluate_meteor(self, candidates, references):
-        meteor_scores = [meteor_score([ref], cand) for ref, cand in zip(references, candidates)]
-        return sum(meteor_scores) / len(meteor_scores)
-    
+
     def evaluate_all(self, question, response, reference):
         candidates = [response]
         references = [reference]
         bleu, rouge1 = self.evaluate_bleu_rouge(candidates, references)
         bert_p, bert_r, bert_f1 = self.evaluate_bert_score(candidates, references)
         perplexity = self.evaluate_perplexity(response)
         diversity = self.evaluate_diversity(candidates)
         racial_bias = self.evaluate_racial_bias(response)
-        meteor = self.evaluate_meteor(candidates, references)
         return {
             "BLEU": bleu,
             "ROUGE-1": rouge1,
             "BERT P": bert_p,
             "BERT R": bert_r,
             "BERT F1": bert_f1,
             "Perplexity": perplexity,
             "Diversity": diversity,
-            "Racial Bias": racial_bias,
-            "METEOR" : meteor
+            "Racial Bias": racial_bias
         }
```

### Comparing `ragevals-0.2.0/ragevals/test_ragevals.py` & `ragevals-0.2.1/ragevals/test_ragevals.py`

 * *Files identical despite different names*

### Comparing `ragevals-0.2.0/ragevals.egg-info/PKG-INFO` & `ragevals-0.2.1/ragevals.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ragevals
-Version: 0.2.0
+Version: 0.2.1
 Summary: A library for evaluating Retrieval-Augmented Generation (RAG) systems
 Home-page: https://github.com/captainawesome78/RAGevals
 Author: Shaik Naveed
 Author-email: mailmenaveed88@gmail.com
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

### Comparing `ragevals-0.2.0/setup.py` & `ragevals-0.2.1/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from setuptools import setup, find_packages
 
 setup(
     name="ragevals",
-    version="0.2.0",
+    version="0.2.1",
     description="A library for evaluating Retrieval-Augmented Generation (RAG) systems",
     long_description=open('README.md').read(),
     long_description_content_type='text/markdown',
     author="Shaik Naveed",
     author_email="mailmenaveed88@gmail.com",
     url="https://github.com/captainawesome78/RAGevals",
     packages=find_packages(),
```

