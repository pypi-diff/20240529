# Comparing `tmp/prompt_learner-0.2.7.tar.gz` & `tmp/prompt_learner-0.2.8.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "prompt_learner-0.2.7.tar", max compression
+gzip compressed data, was "prompt_learner-0.2.8.tar", max compression
```

## Comparing `prompt_learner-0.2.7.tar` & `prompt_learner-0.2.8.tar`

### file list

```diff
@@ -1,37 +1,37 @@
--rw-r--r--   0        0        0     2288 2024-05-28 21:05:53.126497 prompt_learner-0.2.7/README.md
--rw-r--r--   0        0        0     6148 2024-05-24 20:42:17.913011 prompt_learner-0.2.7/prompt_learner/.DS_Store
--rw-r--r--   0        0        0       28 2024-05-24 20:42:17.913126 prompt_learner-0.2.7/prompt_learner/adapters/__init__.py
--rw-r--r--   0        0        0     1129 2024-05-28 21:04:29.168601 prompt_learner-0.2.7/prompt_learner/adapters/adapter.py
--rw-r--r--   0        0        0      817 2024-05-28 21:04:11.862612 prompt_learner-0.2.7/prompt_learner/adapters/anthropic.py
--rw-r--r--   0        0        0      757 2024-05-28 19:57:13.623830 prompt_learner-0.2.7/prompt_learner/adapters/llama.py
--rw-r--r--   0        0        0      949 2024-05-28 21:04:06.266308 prompt_learner-0.2.7/prompt_learner/adapters/ollama_local.py
--rw-r--r--   0        0        0      757 2024-05-28 19:57:09.541479 prompt_learner-0.2.7/prompt_learner/adapters/openai.py
--rw-r--r--   0        0        0     1278 2024-05-24 20:42:17.913806 prompt_learner-0.2.7/prompt_learner/evals/metrics/accuracy.py
--rw-r--r--   0        0        0       29 2024-05-24 20:42:17.913956 prompt_learner-0.2.7/prompt_learner/examples/__init__.py
--rw-r--r--   0        0        0      316 2024-05-24 20:42:17.914044 prompt_learner-0.2.7/prompt_learner/examples/example.py
--rw-r--r--   0        0        0        0 2024-05-24 20:42:17.914130 prompt_learner-0.2.7/prompt_learner/examples/manipulation/__init__.py
--rw-r--r--   0        0        0        0 2024-05-24 20:42:17.914236 prompt_learner-0.2.7/prompt_learner/inference/__init__.py
--rw-r--r--   0        0        0        0 2024-05-24 20:42:17.914292 prompt_learner-0.2.7/prompt_learner/inference/predict.py
--rw-r--r--   0        0        0        0 2024-05-24 20:42:17.914393 prompt_learner-0.2.7/prompt_learner/optimizers/__init__.py
--rw-r--r--   0        0        0     2490 2024-05-28 21:03:44.918142 prompt_learner-0.2.7/prompt_learner/optimizers/grid_search.py
--rw-r--r--   0        0        0      539 2024-05-28 21:03:53.376070 prompt_learner-0.2.7/prompt_learner/optimizers/optimizer.py
--rw-r--r--   0        0        0       26 2024-05-24 20:42:17.914611 prompt_learner-0.2.7/prompt_learner/prompts/__init__.py
--rw-r--r--   0        0        0      597 2024-05-24 20:42:17.914685 prompt_learner-0.2.7/prompt_learner/prompts/cot.py
--rw-r--r--   0        0        0     1114 2024-05-24 20:42:17.914765 prompt_learner-0.2.7/prompt_learner/prompts/prompt.py
--rw-r--r--   0        0        0       30 2024-05-24 20:42:17.914890 prompt_learner-0.2.7/prompt_learner/selectors/__init__.py
--rw-r--r--   0        0        0     1635 2024-05-25 21:40:52.339141 prompt_learner-0.2.7/prompt_learner/selectors/diverse_sampler.py
--rw-r--r--   0        0        0      599 2024-05-25 21:40:21.427745 prompt_learner-0.2.7/prompt_learner/selectors/random_sampler.py
--rw-r--r--   0        0        0      880 2024-05-26 04:26:50.424797 prompt_learner-0.2.7/prompt_learner/selectors/selector.py
--rw-r--r--   0        0        0      888 2024-05-24 20:42:17.915207 prompt_learner-0.2.7/prompt_learner/selectors/stratified_sampler.py
--rw-r--r--   0        0        0       22 2024-05-24 20:42:17.915348 prompt_learner-0.2.7/prompt_learner/tasks/__init__.py
--rw-r--r--   0        0        0      625 2024-05-24 20:42:17.915451 prompt_learner-0.2.7/prompt_learner/tasks/classification.py
--rw-r--r--   0        0        0      400 2024-05-24 20:42:17.915556 prompt_learner-0.2.7/prompt_learner/tasks/sql_generation.py
--rw-r--r--   0        0        0      529 2024-05-24 20:42:17.915946 prompt_learner-0.2.7/prompt_learner/tasks/tagging.py
--rw-r--r--   0        0        0     1589 2024-05-24 20:42:17.916465 prompt_learner-0.2.7/prompt_learner/tasks/task.py
--rw-r--r--   0        0        0       30 2024-05-24 20:42:17.916660 prompt_learner-0.2.7/prompt_learner/templates/__init__.py
--rw-r--r--   0        0        0     2805 2024-05-28 21:04:48.274343 prompt_learner-0.2.7/prompt_learner/templates/markdown.py
--rw-r--r--   0        0        0     1638 2024-05-26 04:26:03.988721 prompt_learner-0.2.7/prompt_learner/templates/template.py
--rw-r--r--   0        0        0     2906 2024-05-28 20:19:06.403920 prompt_learner-0.2.7/prompt_learner/templates/xml.py
--rw-r--r--   0        0        0     3373 2024-05-24 20:42:17.917199 prompt_learner-0.2.7/prompt_learner/translator/translate.py
--rw-r--r--   0        0        0      485 2024-05-28 21:17:02.481712 prompt_learner-0.2.7/pyproject.toml
--rw-r--r--   0        0        0     3012 1970-01-01 00:00:00.000000 prompt_learner-0.2.7/PKG-INFO
+-rw-r--r--   0        0        0     2288 2024-05-28 21:05:53.126497 prompt_learner-0.2.8/README.md
+-rw-r--r--   0        0        0     6148 2024-05-24 20:42:17.913011 prompt_learner-0.2.8/prompt_learner/.DS_Store
+-rw-r--r--   0        0        0       28 2024-05-24 20:42:17.913126 prompt_learner-0.2.8/prompt_learner/adapters/__init__.py
+-rw-r--r--   0        0        0     1129 2024-05-28 21:04:29.168601 prompt_learner-0.2.8/prompt_learner/adapters/adapter.py
+-rw-r--r--   0        0        0      817 2024-05-28 21:04:11.862612 prompt_learner-0.2.8/prompt_learner/adapters/anthropic.py
+-rw-r--r--   0        0        0      757 2024-05-28 19:57:13.623830 prompt_learner-0.2.8/prompt_learner/adapters/llama.py
+-rw-r--r--   0        0        0      949 2024-05-28 21:04:06.266308 prompt_learner-0.2.8/prompt_learner/adapters/ollama_local.py
+-rw-r--r--   0        0        0      757 2024-05-28 19:57:09.541479 prompt_learner-0.2.8/prompt_learner/adapters/openai.py
+-rw-r--r--   0        0        0     1278 2024-05-24 20:42:17.913806 prompt_learner-0.2.8/prompt_learner/evals/metrics/accuracy.py
+-rw-r--r--   0        0        0       29 2024-05-24 20:42:17.913956 prompt_learner-0.2.8/prompt_learner/examples/__init__.py
+-rw-r--r--   0        0        0      316 2024-05-24 20:42:17.914044 prompt_learner-0.2.8/prompt_learner/examples/example.py
+-rw-r--r--   0        0        0        0 2024-05-24 20:42:17.914130 prompt_learner-0.2.8/prompt_learner/examples/manipulation/__init__.py
+-rw-r--r--   0        0        0        0 2024-05-24 20:42:17.914236 prompt_learner-0.2.8/prompt_learner/inference/__init__.py
+-rw-r--r--   0        0        0        0 2024-05-24 20:42:17.914292 prompt_learner-0.2.8/prompt_learner/inference/predict.py
+-rw-r--r--   0        0        0        0 2024-05-24 20:42:17.914393 prompt_learner-0.2.8/prompt_learner/optimizers/__init__.py
+-rw-r--r--   0        0        0     2999 2024-05-29 00:12:25.436308 prompt_learner-0.2.8/prompt_learner/optimizers/grid_search.py
+-rw-r--r--   0        0        0      539 2024-05-28 21:03:53.376070 prompt_learner-0.2.8/prompt_learner/optimizers/optimizer.py
+-rw-r--r--   0        0        0       26 2024-05-24 20:42:17.914611 prompt_learner-0.2.8/prompt_learner/prompts/__init__.py
+-rw-r--r--   0        0        0      597 2024-05-24 20:42:17.914685 prompt_learner-0.2.8/prompt_learner/prompts/cot.py
+-rw-r--r--   0        0        0     1114 2024-05-24 20:42:17.914765 prompt_learner-0.2.8/prompt_learner/prompts/prompt.py
+-rw-r--r--   0        0        0       30 2024-05-24 20:42:17.914890 prompt_learner-0.2.8/prompt_learner/selectors/__init__.py
+-rw-r--r--   0        0        0     1635 2024-05-25 21:40:52.339141 prompt_learner-0.2.8/prompt_learner/selectors/diverse_sampler.py
+-rw-r--r--   0        0        0      599 2024-05-25 21:40:21.427745 prompt_learner-0.2.8/prompt_learner/selectors/random_sampler.py
+-rw-r--r--   0        0        0      880 2024-05-26 04:26:50.424797 prompt_learner-0.2.8/prompt_learner/selectors/selector.py
+-rw-r--r--   0        0        0      888 2024-05-24 20:42:17.915207 prompt_learner-0.2.8/prompt_learner/selectors/stratified_sampler.py
+-rw-r--r--   0        0        0       22 2024-05-24 20:42:17.915348 prompt_learner-0.2.8/prompt_learner/tasks/__init__.py
+-rw-r--r--   0        0        0      625 2024-05-24 20:42:17.915451 prompt_learner-0.2.8/prompt_learner/tasks/classification.py
+-rw-r--r--   0        0        0      400 2024-05-24 20:42:17.915556 prompt_learner-0.2.8/prompt_learner/tasks/sql_generation.py
+-rw-r--r--   0        0        0      529 2024-05-24 20:42:17.915946 prompt_learner-0.2.8/prompt_learner/tasks/tagging.py
+-rw-r--r--   0        0        0     1589 2024-05-24 20:42:17.916465 prompt_learner-0.2.8/prompt_learner/tasks/task.py
+-rw-r--r--   0        0        0       30 2024-05-24 20:42:17.916660 prompt_learner-0.2.8/prompt_learner/templates/__init__.py
+-rw-r--r--   0        0        0     2805 2024-05-28 21:04:48.274343 prompt_learner-0.2.8/prompt_learner/templates/markdown.py
+-rw-r--r--   0        0        0     1638 2024-05-26 04:26:03.988721 prompt_learner-0.2.8/prompt_learner/templates/template.py
+-rw-r--r--   0        0        0     2906 2024-05-28 20:19:06.403920 prompt_learner-0.2.8/prompt_learner/templates/xml.py
+-rw-r--r--   0        0        0     3373 2024-05-24 20:42:17.917199 prompt_learner-0.2.8/prompt_learner/translator/translate.py
+-rw-r--r--   0        0        0      485 2024-05-29 00:13:30.915092 prompt_learner-0.2.8/pyproject.toml
+-rw-r--r--   0        0        0     3012 1970-01-01 00:00:00.000000 prompt_learner-0.2.8/PKG-INFO
```

### Comparing `prompt_learner-0.2.7/README.md` & `prompt_learner-0.2.8/README.md`

 * *Files identical despite different names*

### Comparing `prompt_learner-0.2.7/prompt_learner/.DS_Store` & `prompt_learner-0.2.8/prompt_learner/.DS_Store`

 * *Files identical despite different names*

### Comparing `prompt_learner-0.2.7/prompt_learner/adapters/adapter.py` & `prompt_learner-0.2.8/prompt_learner/adapters/adapter.py`

 * *Files identical despite different names*

### Comparing `prompt_learner-0.2.7/prompt_learner/adapters/anthropic.py` & `prompt_learner-0.2.8/prompt_learner/adapters/anthropic.py`

 * *Files identical despite different names*

### Comparing `prompt_learner-0.2.7/prompt_learner/adapters/llama.py` & `prompt_learner-0.2.8/prompt_learner/adapters/llama.py`

 * *Files identical despite different names*

### Comparing `prompt_learner-0.2.7/prompt_learner/adapters/ollama_local.py` & `prompt_learner-0.2.8/prompt_learner/adapters/ollama_local.py`

 * *Files identical despite different names*

### Comparing `prompt_learner-0.2.7/prompt_learner/adapters/openai.py` & `prompt_learner-0.2.8/prompt_learner/adapters/openai.py`

 * *Files identical despite different names*

### Comparing `prompt_learner-0.2.7/prompt_learner/evals/metrics/accuracy.py` & `prompt_learner-0.2.8/prompt_learner/evals/metrics/accuracy.py`

 * *Files identical despite different names*

### Comparing `prompt_learner-0.2.7/prompt_learner/optimizers/grid_search.py` & `prompt_learner-0.2.8/prompt_learner/optimizers/grid_search.py`

 * *Files 9% similar despite different names*

```diff
@@ -1,59 +1,65 @@
 """Class for grid search optimization."""
 from prompt_learner.optimizers.optimizer import Optimizer
 from prompt_learner.evals.metrics.accuracy import Accuracy
-
+from tqdm import tqdm
 
 class GridSearch(Optimizer):
     """Grid search optimizer."""
     def search(self, param_grid: dict):
         """Search for the best hyperparameters given in the 
         parameter grid."""
         best_score = 0
         best_params = {}
         all_results = []
         all_samplers = param_grid.get('sampler',None)
         all_templates = param_grid.get('template', [self.prompt.template])
         all_adapters = param_grid.get('adapter',None)
         if all_samplers is not None:
             return self.search_samplers(all_samplers, all_templates, all_adapters)
-        for template in all_templates:
-            self.prompt.translate(template)
-            for adapter in all_adapters:
-                acc, _ = Accuracy(self.prompt.template.task).compute(self.prompt, adapter)
-                score = acc
-                curr_params = {'score': score, 
-                               'template': template.class_repr(),
-                               'adapter': repr(adapter)}
-                all_results.append(curr_params)
-                if score > best_score:
-                    best_score = score
-                    best_params = curr_params
-
-        return best_params, all_results
-    
-    def search_samplers(self, all_samplers, all_templates, all_adapters):
-        """Search when samplers are in param grid"""
-        best_score = 0
-        best_params = {}
-        all_results = []
-        for sampler in all_samplers:
-            sampler.task = self.prompt.template.task
-            sampler.select_examples()
+        total_iterations = len(all_templates) * len(all_adapters)
+        with tqdm(total=total_iterations, desc="Grid Search Progress") as pbar:
             for template in all_templates:
                 self.prompt.translate(template)
                 for adapter in all_adapters:
-                    acc, _ = Accuracy(sampler.task).compute(self.prompt, adapter)
+                    acc, _ = Accuracy(self.prompt.template.task).compute(self.prompt, adapter)
                     score = acc
-                    curr_params = {'score': score, 'sampler': repr(sampler),
-                                   'template': template.class_repr(),
-                                   'adapter': repr(adapter)}
+                    curr_params = {'score': score, 
+                                'template': template.class_repr(),
+                                'adapter': repr(adapter)}
                     all_results.append(curr_params)
                     if score > best_score:
                         best_score = score
                         best_params = curr_params
+                    pbar.update(1)
+
+        return best_params, all_results
+    
+    def search_samplers(self, all_samplers, all_templates, all_adapters):
+        """Search when samplers are in param grid"""
+        best_score = 0
+        best_params = {}
+        all_results = []
+        total_iterations = len(all_samplers) * len(all_templates) * len(all_adapters)
+        with tqdm(total=total_iterations, desc="Grid Search Progress") as pbar:
+            for sampler in all_samplers:
+                sampler.task = self.prompt.template.task
+                sampler.select_examples()
+                for template in all_templates:
+                    self.prompt.translate(template)
+                    for adapter in all_adapters:
+                        acc, _ = Accuracy(sampler.task).compute(self.prompt, adapter)
+                        score = acc
+                        curr_params = {'score': score, 'sampler': repr(sampler),
+                                       'template': template.class_repr(),
+                                       'adapter': repr(adapter)}
+                        all_results.append(curr_params)
+                        if score > best_score:
+                            best_score = score
+                            best_params = curr_params
+                        pbar.update(1)
 
         return best_params, all_results
 
     def compute_metrics(self):
         """Compute metrics for a given prompt and adapter on a task."""
         pass
```

### Comparing `prompt_learner-0.2.7/prompt_learner/optimizers/optimizer.py` & `prompt_learner-0.2.8/prompt_learner/optimizers/optimizer.py`

 * *Files identical despite different names*

### Comparing `prompt_learner-0.2.7/prompt_learner/prompts/cot.py` & `prompt_learner-0.2.8/prompt_learner/prompts/cot.py`

 * *Files identical despite different names*

### Comparing `prompt_learner-0.2.7/prompt_learner/prompts/prompt.py` & `prompt_learner-0.2.8/prompt_learner/prompts/prompt.py`

 * *Files identical despite different names*

### Comparing `prompt_learner-0.2.7/prompt_learner/selectors/diverse_sampler.py` & `prompt_learner-0.2.8/prompt_learner/selectors/diverse_sampler.py`

 * *Files identical despite different names*

### Comparing `prompt_learner-0.2.7/prompt_learner/selectors/random_sampler.py` & `prompt_learner-0.2.8/prompt_learner/selectors/random_sampler.py`

 * *Files identical despite different names*

### Comparing `prompt_learner-0.2.7/prompt_learner/selectors/selector.py` & `prompt_learner-0.2.8/prompt_learner/selectors/selector.py`

 * *Files identical despite different names*

### Comparing `prompt_learner-0.2.7/prompt_learner/selectors/stratified_sampler.py` & `prompt_learner-0.2.8/prompt_learner/selectors/stratified_sampler.py`

 * *Files identical despite different names*

### Comparing `prompt_learner-0.2.7/prompt_learner/tasks/classification.py` & `prompt_learner-0.2.8/prompt_learner/tasks/classification.py`

 * *Files identical despite different names*

### Comparing `prompt_learner-0.2.7/prompt_learner/tasks/tagging.py` & `prompt_learner-0.2.8/prompt_learner/tasks/tagging.py`

 * *Files identical despite different names*

### Comparing `prompt_learner-0.2.7/prompt_learner/tasks/task.py` & `prompt_learner-0.2.8/prompt_learner/tasks/task.py`

 * *Files identical despite different names*

### Comparing `prompt_learner-0.2.7/prompt_learner/templates/markdown.py` & `prompt_learner-0.2.8/prompt_learner/templates/markdown.py`

 * *Files identical despite different names*

### Comparing `prompt_learner-0.2.7/prompt_learner/templates/template.py` & `prompt_learner-0.2.8/prompt_learner/templates/template.py`

 * *Files identical despite different names*

### Comparing `prompt_learner-0.2.7/prompt_learner/templates/xml.py` & `prompt_learner-0.2.8/prompt_learner/templates/xml.py`

 * *Files identical despite different names*

### Comparing `prompt_learner-0.2.7/prompt_learner/translator/translate.py` & `prompt_learner-0.2.8/prompt_learner/translator/translate.py`

 * *Files identical despite different names*

### Comparing `prompt_learner-0.2.7/PKG-INFO` & `prompt_learner-0.2.8/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: prompt-learner
-Version: 0.2.7
+Version: 0.2.8
 Summary: 
 Author: Aditya Lahiri
 Author-email: adityalahiri13@gmail.com
 Requires-Python: >=3.11,<4.0
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: Python :: 3.12
```

