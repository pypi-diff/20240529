# Comparing `tmp/prompt_learner-0.2.6.tar.gz` & `tmp/prompt_learner-0.2.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "prompt_learner-0.2.6.tar", max compression
+gzip compressed data, was "prompt_learner-0.2.7.tar", max compression
```

## Comparing `prompt_learner-0.2.6.tar` & `prompt_learner-0.2.7.tar`

### file list

```diff
@@ -1,38 +1,37 @@
--rw-r--r--   0        0        0     2246 2024-05-15 04:01:12.814625 prompt_learner-0.2.6/README.md
--rw-r--r--   0        0        0     6148 2024-05-07 04:41:30.293507 prompt_learner-0.2.6/prompt_learner/.DS_Store
--rw-r--r--   0        0        0       28 2024-05-07 04:41:30.293626 prompt_learner-0.2.6/prompt_learner/adapters/__init__.py
--rw-r--r--   0        0        0      551 2024-05-15 05:38:36.228834 prompt_learner-0.2.6/prompt_learner/adapters/adapter.py
--rw-r--r--   0        0        0     1291 2024-05-07 04:41:30.293764 prompt_learner-0.2.6/prompt_learner/adapters/anthropic.py
--rw-r--r--   0        0        0      659 2024-05-07 04:52:50.363858 prompt_learner-0.2.6/prompt_learner/adapters/llama.py
--rw-r--r--   0        0        0      864 2024-05-22 03:40:32.836264 prompt_learner-0.2.6/prompt_learner/adapters/ollama_local.py
--rw-r--r--   0        0        0      662 2024-05-07 04:41:30.293913 prompt_learner-0.2.6/prompt_learner/adapters/openai.py
--rw-r--r--   0        0        0     1278 2024-05-09 05:51:03.447015 prompt_learner-0.2.6/prompt_learner/evals/metrics/accuracy.py
--rw-r--r--   0        0        0       29 2024-05-07 04:41:30.294168 prompt_learner-0.2.6/prompt_learner/examples/__init__.py
--rw-r--r--   0        0        0      316 2024-05-07 04:41:30.294240 prompt_learner-0.2.6/prompt_learner/examples/example.py
--rw-r--r--   0        0        0        0 2024-05-07 04:41:30.294327 prompt_learner-0.2.6/prompt_learner/examples/manipulation/__init__.py
--rw-r--r--   0        0        0        0 2024-05-07 04:41:30.294404 prompt_learner-0.2.6/prompt_learner/inference/__init__.py
--rw-r--r--   0        0        0        0 2024-05-07 04:41:30.294446 prompt_learner-0.2.6/prompt_learner/inference/predict.py
--rw-r--r--   0        0        0        0 2024-05-07 04:41:30.294532 prompt_learner-0.2.6/prompt_learner/optimizers/__init__.py
--rw-r--r--   0        0        0        0 2024-05-07 04:41:30.294619 prompt_learner-0.2.6/prompt_learner/optimizers/descriptors/__init__.py
--rw-r--r--   0        0        0      165 2024-05-07 04:41:30.294703 prompt_learner-0.2.6/prompt_learner/optimizers/descriptors/descriptor.py
--rw-r--r--   0        0        0       34 2024-05-07 04:41:30.294768 prompt_learner-0.2.6/prompt_learner/optimizers/optimizer.py
--rw-r--r--   0        0        0       30 2024-05-07 04:41:30.294865 prompt_learner-0.2.6/prompt_learner/optimizers/selectors/__init__.py
--rw-r--r--   0        0        0     1537 2024-05-07 04:41:30.294949 prompt_learner-0.2.6/prompt_learner/optimizers/selectors/diverse_sampler.py
--rw-r--r--   0        0        0      624 2024-05-07 04:41:30.295030 prompt_learner-0.2.6/prompt_learner/optimizers/selectors/random_sampler.py
--rw-r--r--   0        0        0      873 2024-05-07 04:41:30.295104 prompt_learner-0.2.6/prompt_learner/optimizers/selectors/selector.py
--rw-r--r--   0        0        0      888 2024-05-07 04:41:30.295186 prompt_learner-0.2.6/prompt_learner/optimizers/selectors/stratified_sampler.py
--rw-r--r--   0        0        0       26 2024-05-07 04:41:30.295292 prompt_learner-0.2.6/prompt_learner/prompts/__init__.py
--rw-r--r--   0        0        0      597 2024-05-07 04:41:30.295363 prompt_learner-0.2.6/prompt_learner/prompts/cot.py
--rw-r--r--   0        0        0     1136 2024-05-07 04:41:30.295433 prompt_learner-0.2.6/prompt_learner/prompts/prompt.py
--rw-r--r--   0        0        0       22 2024-05-07 04:41:30.295534 prompt_learner-0.2.6/prompt_learner/tasks/__init__.py
--rw-r--r--   0        0        0      625 2024-05-07 04:41:30.295599 prompt_learner-0.2.6/prompt_learner/tasks/classification.py
--rw-r--r--   0        0        0      400 2024-05-07 04:41:30.295663 prompt_learner-0.2.6/prompt_learner/tasks/sql_generation.py
--rw-r--r--   0        0        0      529 2024-05-07 04:41:30.295736 prompt_learner-0.2.6/prompt_learner/tasks/tagging.py
--rw-r--r--   0        0        0     1589 2024-05-07 04:41:30.295807 prompt_learner-0.2.6/prompt_learner/tasks/task.py
--rw-r--r--   0        0        0       30 2024-05-07 04:41:30.295907 prompt_learner-0.2.6/prompt_learner/templates/__init__.py
--rw-r--r--   0        0        0     2863 2024-05-10 05:00:14.745809 prompt_learner-0.2.6/prompt_learner/templates/claude_template.py
--rw-r--r--   0        0        0     2648 2024-05-10 04:59:21.271133 prompt_learner-0.2.6/prompt_learner/templates/gpt_template.py
--rw-r--r--   0        0        0     1570 2024-05-07 04:41:30.296119 prompt_learner-0.2.6/prompt_learner/templates/template.py
--rw-r--r--   0        0        0     3373 2024-05-07 04:41:30.296253 prompt_learner-0.2.6/prompt_learner/translator/translate.py
--rw-r--r--   0        0        0      485 2024-05-23 04:05:37.990602 prompt_learner-0.2.6/pyproject.toml
--rw-r--r--   0        0        0     2970 1970-01-01 00:00:00.000000 prompt_learner-0.2.6/PKG-INFO
+-rw-r--r--   0        0        0     2288 2024-05-28 21:05:53.126497 prompt_learner-0.2.7/README.md
+-rw-r--r--   0        0        0     6148 2024-05-24 20:42:17.913011 prompt_learner-0.2.7/prompt_learner/.DS_Store
+-rw-r--r--   0        0        0       28 2024-05-24 20:42:17.913126 prompt_learner-0.2.7/prompt_learner/adapters/__init__.py
+-rw-r--r--   0        0        0     1129 2024-05-28 21:04:29.168601 prompt_learner-0.2.7/prompt_learner/adapters/adapter.py
+-rw-r--r--   0        0        0      817 2024-05-28 21:04:11.862612 prompt_learner-0.2.7/prompt_learner/adapters/anthropic.py
+-rw-r--r--   0        0        0      757 2024-05-28 19:57:13.623830 prompt_learner-0.2.7/prompt_learner/adapters/llama.py
+-rw-r--r--   0        0        0      949 2024-05-28 21:04:06.266308 prompt_learner-0.2.7/prompt_learner/adapters/ollama_local.py
+-rw-r--r--   0        0        0      757 2024-05-28 19:57:09.541479 prompt_learner-0.2.7/prompt_learner/adapters/openai.py
+-rw-r--r--   0        0        0     1278 2024-05-24 20:42:17.913806 prompt_learner-0.2.7/prompt_learner/evals/metrics/accuracy.py
+-rw-r--r--   0        0        0       29 2024-05-24 20:42:17.913956 prompt_learner-0.2.7/prompt_learner/examples/__init__.py
+-rw-r--r--   0        0        0      316 2024-05-24 20:42:17.914044 prompt_learner-0.2.7/prompt_learner/examples/example.py
+-rw-r--r--   0        0        0        0 2024-05-24 20:42:17.914130 prompt_learner-0.2.7/prompt_learner/examples/manipulation/__init__.py
+-rw-r--r--   0        0        0        0 2024-05-24 20:42:17.914236 prompt_learner-0.2.7/prompt_learner/inference/__init__.py
+-rw-r--r--   0        0        0        0 2024-05-24 20:42:17.914292 prompt_learner-0.2.7/prompt_learner/inference/predict.py
+-rw-r--r--   0        0        0        0 2024-05-24 20:42:17.914393 prompt_learner-0.2.7/prompt_learner/optimizers/__init__.py
+-rw-r--r--   0        0        0     2490 2024-05-28 21:03:44.918142 prompt_learner-0.2.7/prompt_learner/optimizers/grid_search.py
+-rw-r--r--   0        0        0      539 2024-05-28 21:03:53.376070 prompt_learner-0.2.7/prompt_learner/optimizers/optimizer.py
+-rw-r--r--   0        0        0       26 2024-05-24 20:42:17.914611 prompt_learner-0.2.7/prompt_learner/prompts/__init__.py
+-rw-r--r--   0        0        0      597 2024-05-24 20:42:17.914685 prompt_learner-0.2.7/prompt_learner/prompts/cot.py
+-rw-r--r--   0        0        0     1114 2024-05-24 20:42:17.914765 prompt_learner-0.2.7/prompt_learner/prompts/prompt.py
+-rw-r--r--   0        0        0       30 2024-05-24 20:42:17.914890 prompt_learner-0.2.7/prompt_learner/selectors/__init__.py
+-rw-r--r--   0        0        0     1635 2024-05-25 21:40:52.339141 prompt_learner-0.2.7/prompt_learner/selectors/diverse_sampler.py
+-rw-r--r--   0        0        0      599 2024-05-25 21:40:21.427745 prompt_learner-0.2.7/prompt_learner/selectors/random_sampler.py
+-rw-r--r--   0        0        0      880 2024-05-26 04:26:50.424797 prompt_learner-0.2.7/prompt_learner/selectors/selector.py
+-rw-r--r--   0        0        0      888 2024-05-24 20:42:17.915207 prompt_learner-0.2.7/prompt_learner/selectors/stratified_sampler.py
+-rw-r--r--   0        0        0       22 2024-05-24 20:42:17.915348 prompt_learner-0.2.7/prompt_learner/tasks/__init__.py
+-rw-r--r--   0        0        0      625 2024-05-24 20:42:17.915451 prompt_learner-0.2.7/prompt_learner/tasks/classification.py
+-rw-r--r--   0        0        0      400 2024-05-24 20:42:17.915556 prompt_learner-0.2.7/prompt_learner/tasks/sql_generation.py
+-rw-r--r--   0        0        0      529 2024-05-24 20:42:17.915946 prompt_learner-0.2.7/prompt_learner/tasks/tagging.py
+-rw-r--r--   0        0        0     1589 2024-05-24 20:42:17.916465 prompt_learner-0.2.7/prompt_learner/tasks/task.py
+-rw-r--r--   0        0        0       30 2024-05-24 20:42:17.916660 prompt_learner-0.2.7/prompt_learner/templates/__init__.py
+-rw-r--r--   0        0        0     2805 2024-05-28 21:04:48.274343 prompt_learner-0.2.7/prompt_learner/templates/markdown.py
+-rw-r--r--   0        0        0     1638 2024-05-26 04:26:03.988721 prompt_learner-0.2.7/prompt_learner/templates/template.py
+-rw-r--r--   0        0        0     2906 2024-05-28 20:19:06.403920 prompt_learner-0.2.7/prompt_learner/templates/xml.py
+-rw-r--r--   0        0        0     3373 2024-05-24 20:42:17.917199 prompt_learner-0.2.7/prompt_learner/translator/translate.py
+-rw-r--r--   0        0        0      485 2024-05-28 21:17:02.481712 prompt_learner-0.2.7/pyproject.toml
+-rw-r--r--   0        0        0     3012 1970-01-01 00:00:00.000000 prompt_learner-0.2.7/PKG-INFO
```

### Comparing `prompt_learner-0.2.6/README.md` & `prompt_learner-0.2.7/README.md`

 * *Files 6% similar despite different names*

```diff
@@ -32,16 +32,17 @@
 ```
 > [!TIP]
 > See the [getting started tutorial](https://promptlearner.attuna.xyz/getting-started.html) for a detailed example of Prompt Learner in action.
 
 ## How it works
 ![Architecture](docs/concepts/images/architecture.png)
 Prompt-learner runs on the above architecture.
-Starting from the left, the user has to decide on 3 aspects -
+Starting from the left, the user has to decide on 4 aspects -
 1. The Task
-2. A set of Examples
-3. An LLM Adapter
+2. A Template format for your prompt
+3. A set of Examples
+4. An LLM model to use
 
 A task and examples feed into the template of choice (Claude, Open AI..).
 The task and examples also interact with selectors which can pick the best n examples for the task using statistical and machine learning techniques.
 These selected examples slot into the template, along with any custom instructions from any prompting technique( such as adding 'think step by step' for chain of thought prompting) comprise the final prompt. 
 The prompt invokes the LLM through the adapter with any given inference sample to produce the final output.
```

### Comparing `prompt_learner-0.2.6/prompt_learner/.DS_Store` & `prompt_learner-0.2.7/prompt_learner/.DS_Store`

 * *Files identical despite different names*

### Comparing `prompt_learner-0.2.6/prompt_learner/adapters/llama.py` & `prompt_learner-0.2.7/prompt_learner/adapters/llama.py`

 * *Files 20% similar despite different names*

```diff
@@ -13,7 +13,10 @@
         super().__init__(temperature, max_tokens)
         load_dotenv()
         self.llm = ChatGroq(
             model=model_name,
             groq_api_key=os.getenv('GROQ_API_KEY'),
             temperature=self.temperature,
             max_tokens=self.max_tokens)
+    
+    def __repr__(self):
+        return f"""Llama Adapter(model_name={self.llm.model_name})"""
```

### Comparing `prompt_learner-0.2.6/prompt_learner/adapters/openai.py` & `prompt_learner-0.2.7/prompt_learner/adapters/openai.py`

 * *Files 12% similar despite different names*

```diff
@@ -13,7 +13,10 @@
         super().__init__(temperature, max_tokens)
         load_dotenv()
         self.llm = ChatOpenAI(
             openai_api_key=os.getenv('OPENAI_API_KEY'),
             model=model_name,
             temperature=self.temperature,
             max_tokens=self.max_tokens)
+
+    def __repr__(self):
+        return f"""Openai Adapter(model_name={self.llm.model_name})"""
```

### Comparing `prompt_learner-0.2.6/prompt_learner/evals/metrics/accuracy.py` & `prompt_learner-0.2.7/prompt_learner/evals/metrics/accuracy.py`

 * *Files identical despite different names*

### Comparing `prompt_learner-0.2.6/prompt_learner/optimizers/selectors/diverse_sampler.py` & `prompt_learner-0.2.7/prompt_learner/selectors/diverse_sampler.py`

 * *Files 8% similar despite different names*

```diff
@@ -35,7 +35,10 @@
                 current_index = np.argmin(np.max(sim_matrix[:, indices], axis=1))
             
             # Add the index of the selected text to the list
             indices.append(current_index)
 
         self.selected_examples = [self.all_examples[i] for i in indices]
         self.task.selected_examples = self.selected_examples
+    
+    def __repr__(self):
+        return f"""DiverseSampler(num_samples={self.num_samples})"""
```

### Comparing `prompt_learner-0.2.6/prompt_learner/optimizers/selectors/random_sampler.py` & `prompt_learner-0.2.7/prompt_learner/selectors/random_sampler.py`

 * *Files 18% similar despite different names*

```diff
@@ -11,9 +11,8 @@
         """Select examples for the task randomly""" 
         random.shuffle(self.all_examples)
         self.selected_examples = self.all_examples[:self.num_samples]
         self.task.selected_examples = self.selected_examples
         return self
 
     def __repr__(self):
-        return f"""RandomSampler(task={self.task},
-        num_samples={self.num_samples}"""
+        return f"""RandomSampler(num_samples={self.num_samples})"""
```

### Comparing `prompt_learner-0.2.6/prompt_learner/optimizers/selectors/selector.py` & `prompt_learner-0.2.7/prompt_learner/selectors/selector.py`

 * *Files 12% similar despite different names*

```diff
@@ -5,15 +5,15 @@
 from prompt_learner.examples.example import Example
 
 
 class Selector(BaseModel):
     """Defines the contract for a Generic Example Selector."""
     all_examples: List[Example] = []
     selected_examples: List[Example] = []
-    task: Task
+    task: Task = None
     num_samples: int = Field(description="Number of examples to samples", default=1)
     
     def __init__(self, **kwargs):
         super().__init__(**kwargs)
         self.all_examples = self.task.examples
 
     def select_examples(self):
```

### Comparing `prompt_learner-0.2.6/prompt_learner/optimizers/selectors/stratified_sampler.py` & `prompt_learner-0.2.7/prompt_learner/selectors/stratified_sampler.py`

 * *Files identical despite different names*

### Comparing `prompt_learner-0.2.6/prompt_learner/prompts/cot.py` & `prompt_learner-0.2.7/prompt_learner/prompts/cot.py`

 * *Files identical despite different names*

### Comparing `prompt_learner-0.2.6/prompt_learner/prompts/prompt.py` & `prompt_learner-0.2.7/prompt_learner/prompts/prompt.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 """A class for a Generic Prompt."""
 from pydantic import Field, BaseModel
-from prompt_learner.optimizers.selectors.selector import Selector
-from prompt_learner.optimizers.selectors.random_sampler import RandomSampler
+from prompt_learner.selectors.selector import Selector
+from prompt_learner.selectors.random_sampler import RandomSampler
 from prompt_learner.templates.template import Template
 
 
 class Prompt(BaseModel):
     """Defines the contract for a Generic Prompt."""
     template: Template
     prompt: str = Field(description="Final prompt string.", default="")
```

### Comparing `prompt_learner-0.2.6/prompt_learner/tasks/classification.py` & `prompt_learner-0.2.7/prompt_learner/tasks/classification.py`

 * *Files identical despite different names*

### Comparing `prompt_learner-0.2.6/prompt_learner/tasks/tagging.py` & `prompt_learner-0.2.7/prompt_learner/tasks/tagging.py`

 * *Files identical despite different names*

### Comparing `prompt_learner-0.2.6/prompt_learner/tasks/task.py` & `prompt_learner-0.2.7/prompt_learner/tasks/task.py`

 * *Files identical despite different names*

### Comparing `prompt_learner-0.2.6/prompt_learner/templates/claude_template.py` & `prompt_learner-0.2.7/prompt_learner/templates/xml.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,15 +1,15 @@
-"""This module contains the ClaudeTemplate class"""
+"""This module contains the XmlTemplate class"""
 from typing import List
 from prompt_learner.examples.example import Example
 from .template import Template
 
 
-class ClaudeTemplate(Template):
-    """This class generates a template for Anthropic completions"""
+class XmlTemplate(Template):
+    """This class generates a Xml template"""
     def __init__(self, **kwargs):
         super().__init__(**kwargs)
         tasks_with_labels = ["Classification", "Tagging"]
         self.descriptor = f"""You are a helpful AI assistant.  \nYou are helping a user with a {self.task_type} task.  \nThe user gives you the following task description.  \n<task_description>{self.task_description}</task_description>  \n"""
         if self.allowed_labels:
             self.descriptor += f"""You have to select from the following labels.  \n<allowed_labels>{self.allowed_labels}</allowed_labels>"""
         if self.task_type in tasks_with_labels:
@@ -39,7 +39,11 @@
         prediction_preamble = self.prediction_preamble + f"""  \n <text> {text} <text>"""
         if self.task_type in tasks_with_labels:
             return prediction_preamble + "<label>"
         elif self.task_type == "SQLGeneration":
             return prediction_preamble + f"""  \n <schema>{context} <\schema>\m <SQL>"""
         else:
             return prediction_preamble + "<output>"
+
+    @classmethod
+    def class_repr(cls):
+        return "XmlTemplate"
```

### Comparing `prompt_learner-0.2.6/prompt_learner/templates/gpt_template.py` & `prompt_learner-0.2.7/prompt_learner/templates/markdown.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,46 +1,51 @@
-"""This module contains the GPTTemplate class"""
+"""This module contains the MarkdownTemplate class"""
 from typing import List
 from prompt_learner.examples.example import Example
 from .template import Template
 
 
-class GPTTemplate(Template):
-    """This class generates a template for OpenAI completions"""
+class MarkdownTemplate(Template):
+    """This class generates a template in Markdown"""
     
     def __init__(self, **kwargs):
         super().__init__(**kwargs)
         tasks_with_labels = ["Classification", "Tagging"]
-        self.descriptor = f"""You are a helpful AI assistant.  \nYou are helping a user with a {self.task_type} task.  \nThe user gives you the following task description.  \n{self.task_description}\n"""
+        self.descriptor = f"""You are a helpful AI assistant.  \nYou are helping a user with a {self.task_type} task.  \nThe user gives you the following task description.  \n### Task Description:  \n{self.task_description}\n"""
         if self.allowed_labels:
-            self.descriptor += f"""You have to select from the following labels.  \n{self.allowed_labels}.  \nOnly output labels and nothing else"""
+            self.descriptor += f"""You have to select from the following labels.  \n### Allowed Labels:  \n{self.allowed_labels}.  \nOnly output labels and nothing else"""
         if self.task_type in tasks_with_labels:
             self.prediction_preamble = f"""Given the text, you have to now predict the labels from the list of allowed labels - {self.allowed_labels}."""
         elif self.task_type == "SQLGeneration":
             self.prediction_preamble = """Given the text, you have to now generate a SQL query.Only output the SQL and nothing else."""
         else:  #generic preamble for prediction
             self.prediction_preamble = """Given the text, you have to now predict."""
-        self.examples_preamble = """Here are a few examples to help you understand the task better.  \n"""
+        self.examples_preamble = """Here are a few examples to help you understand the task better.  \n### Examples  \n"""
        
     def format_examples(self, examples: List[Example]):
         """Formats the task examples into a string."""
         tasks_with_labels = ["Classification", "Tagging"]
         examples_str = ""
         for example in examples:
             if self.task_type in tasks_with_labels:
-                examples_str += f"""text: {example.text}  \nlabel: {example.label}  \n"""
+                examples_str += f"""-text: {example.text}  \n-label: {example.label}  \n"""
             elif self.task_type == "SQLGeneration":
-                examples_str += f"""schema: {example.context}  \ntext: {example.text}  \nSQL: {example.label}  \n"""
+                examples_str += f"""-schema: {example.context}  \n-text: {example.text}  \n-SQL: {example.label}  \n"""
             else: #generic example format
                 examples_str += f"""
-                text: {example.text}  \noutput: {example.label}  \n"""
+                -text: {example.text}  \n-output: {example.label}  \n"""
         return examples_str
 
     def add_prediction_sample(self, text: str, context: str = None):
         """Add prediction sample to task."""
         tasks_with_labels = ["Classification", "Tagging"]
         if self.task_type in tasks_with_labels:
-            return self.prediction_preamble + f"""  \ntext: {text}"""+ "  \nlabel:"
+            return self.prediction_preamble + f"""  \n-text: {text}"""+ "  \n-label:"
         elif self.task_type == "SQLGeneration":
-            return self.prediction_preamble + f"""  \nschema: {context}  \ntext: {text}  \nSQL: """
+            return self.prediction_preamble + f"""  \n-schema: {context}  \n-text: {text}  \n-SQL: """
         else:
-            return self.prediction_preamble + "  \noutput:"
+            return self.prediction_preamble + "  \n-output:"
+
+    @classmethod
+    def class_repr(cls):
+        return "MarkdownTemplate"
+
```

### Comparing `prompt_learner-0.2.6/prompt_learner/templates/template.py` & `prompt_learner-0.2.7/prompt_learner/templates/template.py`

 * *Files 3% similar despite different names*

```diff
@@ -31,7 +31,11 @@
     def format_examples(self, examples: List[Example]):
         """Add an example to the task."""
         # This method will be overridden in subclasses
 
     def add_prediction_sample(self, text: str, context: str):
         """Add inference instructions to task."""
         # This method will be overridden in subclasses
+
+    @classmethod
+    def class_repr(cls):
+        return "Template"
```

### Comparing `prompt_learner-0.2.6/prompt_learner/translator/translate.py` & `prompt_learner-0.2.7/prompt_learner/translator/translate.py`

 * *Files identical despite different names*

### Comparing `prompt_learner-0.2.6/PKG-INFO` & `prompt_learner-0.2.7/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: prompt-learner
-Version: 0.2.6
+Version: 0.2.7
 Summary: 
 Author: Aditya Lahiri
 Author-email: adityalahiri13@gmail.com
 Requires-Python: >=3.11,<4.0
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: Python :: 3.12
@@ -52,16 +52,17 @@
 ```
 > [!TIP]
 > See the [getting started tutorial](https://promptlearner.attuna.xyz/getting-started.html) for a detailed example of Prompt Learner in action.
 
 ## How it works
 ![Architecture](docs/concepts/images/architecture.png)
 Prompt-learner runs on the above architecture.
-Starting from the left, the user has to decide on 3 aspects -
+Starting from the left, the user has to decide on 4 aspects -
 1. The Task
-2. A set of Examples
-3. An LLM Adapter
+2. A Template format for your prompt
+3. A set of Examples
+4. An LLM model to use
 
 A task and examples feed into the template of choice (Claude, Open AI..).
 The task and examples also interact with selectors which can pick the best n examples for the task using statistical and machine learning techniques.
 These selected examples slot into the template, along with any custom instructions from any prompting technique( such as adding 'think step by step' for chain of thought prompting) comprise the final prompt. 
 The prompt invokes the LLM through the adapter with any given inference sample to produce the final output.
```

