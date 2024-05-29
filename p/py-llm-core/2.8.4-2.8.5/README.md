# Comparing `tmp/py-llm-core-2.8.4.tar.gz` & `tmp/py_llm_core-2.8.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "py-llm-core-2.8.4.tar", last modified: Thu Apr 11 20:26:51 2024, max compression
+gzip compressed data, was "py_llm_core-2.8.5.tar", last modified: Wed May 29 15:31:48 2024, max compression
```

## Comparing `py-llm-core-2.8.4.tar` & `py_llm_core-2.8.5.tar`

### file list

```diff
@@ -1,34 +1,34 @@
-drwxr-xr-x   0 pas        (501) staff       (20)        0 2024-04-11 20:26:51.293892 py-llm-core-2.8.4/
--rw-r--r--   0 pas        (501) staff       (20)     1082 2024-04-05 09:56:33.000000 py-llm-core-2.8.4/LICENSE
--rw-r--r--   0 pas        (501) staff       (20)       26 2024-04-05 09:56:33.000000 py-llm-core-2.8.4/MANIFEST.in
--rw-r--r--   0 pas        (501) staff       (20)    27667 2024-04-11 20:26:51.293631 py-llm-core-2.8.4/PKG-INFO
--rw-r--r--   0 pas        (501) staff       (20)    27148 2024-04-05 09:56:33.000000 py-llm-core-2.8.4/README.md
--rw-r--r--   0 pas        (501) staff       (20)       98 2024-04-11 20:25:41.000000 py-llm-core-2.8.4/requirements.txt
--rw-r--r--   0 pas        (501) staff       (20)       38 2024-04-11 20:26:51.293931 py-llm-core-2.8.4/setup.cfg
--rw-r--r--   0 pas        (501) staff       (20)      785 2024-04-11 20:25:41.000000 py-llm-core-2.8.4/setup.py
-drwxr-xr-x   0 pas        (501) staff       (20)        0 2024-04-11 20:26:51.288203 py-llm-core-2.8.4/src/
-drwxr-xr-x   0 pas        (501) staff       (20)        0 2024-04-11 20:26:51.290189 py-llm-core-2.8.4/src/llm_core/
--rw-r--r--   0 pas        (501) staff       (20)       73 2024-04-05 09:56:33.000000 py-llm-core-2.8.4/src/llm_core/__init__.py
-drwxr-xr-x   0 pas        (501) staff       (20)        0 2024-04-11 20:26:51.291635 py-llm-core-2.8.4/src/llm_core/assistants/
--rw-r--r--   0 pas        (501) staff       (20)      591 2024-04-11 20:25:41.000000 py-llm-core-2.8.4/src/llm_core/assistants/__init__.py
--rw-r--r--   0 pas        (501) staff       (20)      993 2024-04-05 09:56:33.000000 py-llm-core-2.8.4/src/llm_core/assistants/analysts.py
--rw-r--r--   0 pas        (501) staff       (20)     1646 2024-04-11 20:25:41.000000 py-llm-core-2.8.4/src/llm_core/assistants/base.py
--rw-r--r--   0 pas        (501) staff       (20)     3744 2024-04-05 09:56:33.000000 py-llm-core-2.8.4/src/llm_core/assistants/summarizers.py
--rw-r--r--   0 pas        (501) staff       (20)     1851 2024-04-05 09:56:33.000000 py-llm-core-2.8.4/src/llm_core/assistants/verifiers.py
-drwxr-xr-x   0 pas        (501) staff       (20)        0 2024-04-11 20:26:51.292402 py-llm-core-2.8.4/src/llm_core/llm/
--rw-r--r--   0 pas        (501) staff       (20)      239 2024-04-11 20:25:41.000000 py-llm-core-2.8.4/src/llm_core/llm/__init__.py
--rw-r--r--   0 pas        (501) staff       (20)     2674 2024-04-11 20:25:41.000000 py-llm-core-2.8.4/src/llm_core/llm/base.py
--rw-r--r--   0 pas        (501) staff       (20)     5019 2024-04-05 09:56:33.000000 py-llm-core-2.8.4/src/llm_core/llm/llama_cpp_compatible.py
--rw-r--r--   0 pas        (501) staff       (20)     2848 2024-04-11 20:25:41.000000 py-llm-core-2.8.4/src/llm_core/llm/mistralai.py
--rw-r--r--   0 pas        (501) staff       (20)     3542 2024-04-11 20:25:41.000000 py-llm-core-2.8.4/src/llm_core/llm/openai.py
--rw-r--r--   0 pas        (501) staff       (20)     3377 2024-04-11 20:25:41.000000 py-llm-core-2.8.4/src/llm_core/parsers.py
--rw-r--r--   0 pas        (501) staff       (20)     7185 2024-04-05 09:56:33.000000 py-llm-core-2.8.4/src/llm_core/schema.py
--rw-r--r--   0 pas        (501) staff       (20)      986 2024-04-11 20:25:41.000000 py-llm-core-2.8.4/src/llm_core/settings.py
--rw-r--r--   0 pas        (501) staff       (20)     1019 2024-04-05 09:56:33.000000 py-llm-core-2.8.4/src/llm_core/splitters.py
--rw-r--r--   0 pas        (501) staff       (20)     2455 2024-04-11 20:25:41.000000 py-llm-core-2.8.4/src/llm_core/token_codecs.py
-drwxr-xr-x   0 pas        (501) staff       (20)        0 2024-04-11 20:26:51.293306 py-llm-core-2.8.4/src/py_llm_core.egg-info/
--rw-r--r--   0 pas        (501) staff       (20)    27667 2024-04-11 20:26:51.000000 py-llm-core-2.8.4/src/py_llm_core.egg-info/PKG-INFO
--rw-r--r--   0 pas        (501) staff       (20)      733 2024-04-11 20:26:51.000000 py-llm-core-2.8.4/src/py_llm_core.egg-info/SOURCES.txt
--rw-r--r--   0 pas        (501) staff       (20)        1 2024-04-11 20:26:51.000000 py-llm-core-2.8.4/src/py_llm_core.egg-info/dependency_links.txt
--rw-r--r--   0 pas        (501) staff       (20)       98 2024-04-11 20:26:51.000000 py-llm-core-2.8.4/src/py_llm_core.egg-info/requires.txt
--rw-r--r--   0 pas        (501) staff       (20)        9 2024-04-11 20:26:51.000000 py-llm-core-2.8.4/src/py_llm_core.egg-info/top_level.txt
+drwxr-xr-x   0 pas        (501) staff       (20)        0 2024-05-29 15:31:48.644605 py_llm_core-2.8.5/
+-rw-r--r--   0 pas        (501) staff       (20)     1082 2024-04-05 09:56:33.000000 py_llm_core-2.8.5/LICENSE
+-rw-r--r--   0 pas        (501) staff       (20)       26 2024-04-05 09:56:33.000000 py_llm_core-2.8.5/MANIFEST.in
+-rw-r--r--   0 pas        (501) staff       (20)    26349 2024-05-29 15:31:48.644400 py_llm_core-2.8.5/PKG-INFO
+-rw-r--r--   0 pas        (501) staff       (20)    25830 2024-05-29 15:27:19.000000 py_llm_core-2.8.5/README.md
+-rw-r--r--   0 pas        (501) staff       (20)       98 2024-04-11 20:25:41.000000 py_llm_core-2.8.5/requirements.txt
+-rw-r--r--   0 pas        (501) staff       (20)       38 2024-05-29 15:31:48.644639 py_llm_core-2.8.5/setup.cfg
+-rw-r--r--   0 pas        (501) staff       (20)      785 2024-05-29 15:25:48.000000 py_llm_core-2.8.5/setup.py
+drwxr-xr-x   0 pas        (501) staff       (20)        0 2024-05-29 15:31:48.639505 py_llm_core-2.8.5/src/
+drwxr-xr-x   0 pas        (501) staff       (20)        0 2024-05-29 15:31:48.641474 py_llm_core-2.8.5/src/llm_core/
+-rw-r--r--   0 pas        (501) staff       (20)       73 2024-04-05 09:56:33.000000 py_llm_core-2.8.5/src/llm_core/__init__.py
+drwxr-xr-x   0 pas        (501) staff       (20)        0 2024-05-29 15:31:48.642478 py_llm_core-2.8.5/src/llm_core/assistants/
+-rw-r--r--   0 pas        (501) staff       (20)      591 2024-04-11 20:25:41.000000 py_llm_core-2.8.5/src/llm_core/assistants/__init__.py
+-rw-r--r--   0 pas        (501) staff       (20)      993 2024-04-05 09:56:33.000000 py_llm_core-2.8.5/src/llm_core/assistants/analysts.py
+-rw-r--r--   0 pas        (501) staff       (20)     1646 2024-04-11 20:25:41.000000 py_llm_core-2.8.5/src/llm_core/assistants/base.py
+-rw-r--r--   0 pas        (501) staff       (20)     3744 2024-04-05 09:56:33.000000 py_llm_core-2.8.5/src/llm_core/assistants/summarizers.py
+-rw-r--r--   0 pas        (501) staff       (20)     1851 2024-04-05 09:56:33.000000 py_llm_core-2.8.5/src/llm_core/assistants/verifiers.py
+drwxr-xr-x   0 pas        (501) staff       (20)        0 2024-05-29 15:31:48.643188 py_llm_core-2.8.5/src/llm_core/llm/
+-rw-r--r--   0 pas        (501) staff       (20)      239 2024-04-11 20:25:41.000000 py_llm_core-2.8.5/src/llm_core/llm/__init__.py
+-rw-r--r--   0 pas        (501) staff       (20)     2674 2024-04-11 20:25:41.000000 py_llm_core-2.8.5/src/llm_core/llm/base.py
+-rw-r--r--   0 pas        (501) staff       (20)     5031 2024-05-29 15:29:36.000000 py_llm_core-2.8.5/src/llm_core/llm/llama_cpp_compatible.py
+-rw-r--r--   0 pas        (501) staff       (20)     2848 2024-04-11 20:25:41.000000 py_llm_core-2.8.5/src/llm_core/llm/mistralai.py
+-rw-r--r--   0 pas        (501) staff       (20)     3542 2024-04-11 20:25:41.000000 py_llm_core-2.8.5/src/llm_core/llm/openai.py
+-rw-r--r--   0 pas        (501) staff       (20)     3377 2024-04-11 20:25:41.000000 py_llm_core-2.8.5/src/llm_core/parsers.py
+-rw-r--r--   0 pas        (501) staff       (20)     7185 2024-04-05 09:56:33.000000 py_llm_core-2.8.5/src/llm_core/schema.py
+-rw-r--r--   0 pas        (501) staff       (20)      986 2024-04-11 20:25:41.000000 py_llm_core-2.8.5/src/llm_core/settings.py
+-rw-r--r--   0 pas        (501) staff       (20)     1019 2024-04-05 09:56:33.000000 py_llm_core-2.8.5/src/llm_core/splitters.py
+-rw-r--r--   0 pas        (501) staff       (20)     2455 2024-04-11 20:25:41.000000 py_llm_core-2.8.5/src/llm_core/token_codecs.py
+drwxr-xr-x   0 pas        (501) staff       (20)        0 2024-05-29 15:31:48.644175 py_llm_core-2.8.5/src/py_llm_core.egg-info/
+-rw-r--r--   0 pas        (501) staff       (20)    26349 2024-05-29 15:31:48.000000 py_llm_core-2.8.5/src/py_llm_core.egg-info/PKG-INFO
+-rw-r--r--   0 pas        (501) staff       (20)      733 2024-05-29 15:31:48.000000 py_llm_core-2.8.5/src/py_llm_core.egg-info/SOURCES.txt
+-rw-r--r--   0 pas        (501) staff       (20)        1 2024-05-29 15:31:48.000000 py_llm_core-2.8.5/src/py_llm_core.egg-info/dependency_links.txt
+-rw-r--r--   0 pas        (501) staff       (20)       98 2024-05-29 15:31:48.000000 py_llm_core-2.8.5/src/py_llm_core.egg-info/requires.txt
+-rw-r--r--   0 pas        (501) staff       (20)        9 2024-05-29 15:31:48.000000 py_llm_core-2.8.5/src/py_llm_core.egg-info/top_level.txt
```

### Comparing `py-llm-core-2.8.4/LICENSE` & `py_llm_core-2.8.5/LICENSE`

 * *Files identical despite different names*

### Comparing `py-llm-core-2.8.4/PKG-INFO` & `py_llm_core-2.8.5/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: py-llm-core
-Version: 2.8.4
+Version: 2.8.5
 Summary: PyLLMCore provides a light-weighted interface with LLMs
 Home-page: https://github.com/paschembri/py-llm-core
 Author: P.A. SCHEMBRI
 Author-email: pa.schembri@advanced-stack.com
 License: MIT
 Description-Content-Type: text/markdown
 License-File: LICENSE
@@ -16,101 +16,48 @@
 Requires-Dist: python-decouple
 Requires-Dist: mistralai
 
 # PyLLMCore
 
 ## Overview
 
-PyLLMCore is a light-weighted structured interface with Large Language Models 
-with native support for [llama.cpp](http://github.com/ggerganov/llama.cpp) and OpenAI API.
+PyLLMCore is a light-weighted interface with Large Language Models
+with native support for [llama.cpp](http://github.com/ggerganov/llama.cpp), OpenAI API and Azure deployments.
 
-The design decisions behind PyLLMCore are:
-
-- Sane defaults
-- Clear abstractions and terminology
-- Out of the box utility classes
-
-## Main benefits of using PyLLMCore
+## Expected benefits and reasons to use PyLLMCore
 
 - Pythonic API
 - Simple to use
-- You need structures *everywhere* (provided by the standard library `dataclasses` module)
+- Structures *everywhere* provided by the standard library `dataclasses` module
 - High-level API with the `assistants` module
-- Switching between models has never been easier
+- Easy swapping between models
 
 ## Why you shouldn't use PyLLMCore
 
-- You need a lot of external integrations: Take a look at [langchain](https://github.com/langchain-ai/langchain)
+- You need a whole framework: Take a look at [langchain](https://github.com/langchain-ai/langchain)
 - You need tremendous performance: Take a look at [vllm](https://github.com/vllm-project/vllm)
-- You don't need OpenAI: Take a look a [llama-cpp-python](https://github.com/abetlen/llama-cpp-python) (which is integrated in PyLLMCore)
-- You use Pydantic and don't use the dataclasses module
-
+- You want/need to use Pydantic and don't use the `dataclasses` module
 
 ## Models supported
 
-Besides OpenAI API, the following models are supported for local inference using the [llama.cpp](http://github.com/ggerganov/llama.cpp):
-
-- LLaMA
-- LLaMA 2
-- Falcon
-- [Alpaca](https://github.com/ggerganov/llama.cpp#instruction-mode-with-alpaca)
-- [GPT4All](https://github.com/ggerganov/llama.cpp#using-gpt4all)
-- [Chinese LLaMA / Alpaca](https://github.com/ymcui/Chinese-LLaMA-Alpaca) and [Chinese LLaMA-2 / Alpaca-2](https://github.com/ymcui/Chinese-LLaMA-Alpaca-2)
-- [Vigogne (French)](https://github.com/bofenghuang/vigogne)
-- [Vicuna](https://github.com/ggerganov/llama.cpp/discussions/643#discussioncomment-5533894)
-- [Koala](https://bair.berkeley.edu/blog/2023/04/03/koala/)
-- [OpenBuddy 🐶 (Multilingual)](https://github.com/OpenBuddy/OpenBuddy)
-- [Pygmalion 7B / Metharme 7B](#using-pygmalion-7b--metharme-7b)
-- [WizardLM](https://github.com/nlpxucan/WizardLM)
-- [Baichuan-7B](https://huggingface.co/baichuan-inc/baichuan-7B) and its derivations (such as [baichuan-7b-sft](https://huggingface.co/hiyouga/baichuan-7b-sft))
-- [Aquila-7B](https://huggingface.co/BAAI/Aquila-7B) / [AquilaChat-7B](https://huggingface.co/BAAI/AquilaChat-7B)
-- [Starcoder models](https://github.com/ggerganov/llama.cpp/pull/3187)
-- [Mistral AI v0.1](https://huggingface.co/mistralai/Mistral-7B-v0.1)
+- All open weights models supported by [llama.cpp](http://github.com/ggerganov/llama.cpp) will be compatible.
+- OpenAI / Azure compatible APIs
+- Mistral Large through La Plateforme or Azure
 
 ## Use cases
 
 PyLLMCore covers a narrow range of use cases and serves as a building brick:
 
 - Parsing: see the `parsers` module
 - Summarizing: see the `assistants.summarizers` module
 - Question answering: see the `assistants.analyst` module
 - Hallucinations reduction: see the `assistants.verifiers` module
 - Context size management: see the `splitters` module
-- Tokenizing, encoding, decoding: see the `token_codecs` module
-
-
-## Changelog
-
-- 2.8.3: Raised timeout
-- 2.8.1: Fixed bug when deserializing instances
-- 2.8.0: Added support for native type annotation (pep585) for lists and sets
-- 2.7.0: Fixed bug when function_call was set at None
-- 2.6.1: Add dynamic max_tokens computation for OpenAI
-- 2.6.0: Add support for Azure OpenAI
-- 2.5.1: Fix bug on system prompt format
-- 2.5.0: Add support for LLaVA models
-- 2.4.0:
-    + Set timeouts on OpenAI API
-- 2.2.0:
-    + Default settings on ARM64 MacOS modified (1 thread / offloading everything on the GPU)
-    + Added `completion_kwargs` for Assistants to set temperature
-- 2.1.0:
-    + Added support for Enum to provide better support for classification tasks
-    + Added example in the documentation
-- 2.0.0: 
-    + Refactored code
-    + Dynamically enable GPU offloading on MacOS
-    + Added configuration option for storing local models (MODELS_CACHE_DIR)
-    + Updated documentation
+- Tokenizing: see the `token_codecs` module
 
-- 1.4.0: Free up resources in LLamaParser when exiting the context manager
-- 1.3.0: Support for LLaMA based models (llama, llama2, Mistral Instruct)
-- 1.2.0: Chain of density prompting implemented with OpenAI
-- 1.1.0: Chain of Verification implemented with OpenAI
-- 1.0.0: Initial version
 
 ## Install
 
 ### Quick start
 
 ```shell
 pip install py-llm-core
@@ -885,7 +832,41 @@
         prompt_tokens=630,
         completion_tokens=62,
         total_tokens=692
     ),
     system_fingerprint=None
 )
 ```
+
+
+
+## Changelog
+
+- 2.8.5: Fix model path building
+- 2.8.4: Added support for Mistral Large
+- 2.8.3: Raised timeout
+- 2.8.1: Fixed bug when deserializing instances
+- 2.8.0: Added support for native type annotation (pep585) for lists and sets
+- 2.7.0: Fixed bug when function_call was set at None
+- 2.6.1: Add dynamic max_tokens computation for OpenAI
+- 2.6.0: Add support for Azure OpenAI
+- 2.5.1: Fix bug on system prompt format
+- 2.5.0: Add support for LLaVA models
+- 2.4.0:
+    + Set timeouts on OpenAI API
+- 2.2.0:
+    + Default settings on ARM64 MacOS modified (1 thread / offloading everything on the GPU)
+    + Added `completion_kwargs` for Assistants to set temperature
+- 2.1.0:
+    + Added support for Enum to provide better support for classification tasks
+    + Added example in the documentation
+- 2.0.0:
+    + Refactored code
+    + Dynamically enable GPU offloading on MacOS
+    + Added configuration option for storing local models (MODELS_CACHE_DIR)
+    + Updated documentation
+
+- 1.4.0: Free up resources in LLamaParser when exiting the context manager
+- 1.3.0: Support for LLaMA based models (llama, llama2, Mistral Instruct)
+- 1.2.0: Chain of density prompting implemented with OpenAI
+- 1.1.0: Chain of Verification implemented with OpenAI
+- 1.0.0: Initial version
```

### Comparing `py-llm-core-2.8.4/README.md` & `py_llm_core-2.8.5/src/py_llm_core.egg-info/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,99 +1,64 @@
+Metadata-Version: 2.1
+Name: py-llm-core
+Version: 2.8.5
+Summary: PyLLMCore provides a light-weighted interface with LLMs
+Home-page: https://github.com/paschembri/py-llm-core
+Author: P.A. SCHEMBRI
+Author-email: pa.schembri@advanced-stack.com
+License: MIT
+Description-Content-Type: text/markdown
+License-File: LICENSE
+Requires-Dist: openai<2,>=1.3.5
+Requires-Dist: tiktoken
+Requires-Dist: jsonschema
+Requires-Dist: dirtyjson
+Requires-Dist: llama-cpp-python>=0.2.20
+Requires-Dist: python-decouple
+Requires-Dist: mistralai
+
 # PyLLMCore
 
 ## Overview
 
-PyLLMCore is a light-weighted structured interface with Large Language Models 
-with native support for [llama.cpp](http://github.com/ggerganov/llama.cpp) and OpenAI API.
-
-The design decisions behind PyLLMCore are:
-
-- Sane defaults
-- Clear abstractions and terminology
-- Out of the box utility classes
+PyLLMCore is a light-weighted interface with Large Language Models
+with native support for [llama.cpp](http://github.com/ggerganov/llama.cpp), OpenAI API and Azure deployments.
 
-## Main benefits of using PyLLMCore
+## Expected benefits and reasons to use PyLLMCore
 
 - Pythonic API
 - Simple to use
-- You need structures *everywhere* (provided by the standard library `dataclasses` module)
+- Structures *everywhere* provided by the standard library `dataclasses` module
 - High-level API with the `assistants` module
-- Switching between models has never been easier
+- Easy swapping between models
 
 ## Why you shouldn't use PyLLMCore
 
-- You need a lot of external integrations: Take a look at [langchain](https://github.com/langchain-ai/langchain)
+- You need a whole framework: Take a look at [langchain](https://github.com/langchain-ai/langchain)
 - You need tremendous performance: Take a look at [vllm](https://github.com/vllm-project/vllm)
-- You don't need OpenAI: Take a look a [llama-cpp-python](https://github.com/abetlen/llama-cpp-python) (which is integrated in PyLLMCore)
-- You use Pydantic and don't use the dataclasses module
-
+- You want/need to use Pydantic and don't use the `dataclasses` module
 
 ## Models supported
 
-Besides OpenAI API, the following models are supported for local inference using the [llama.cpp](http://github.com/ggerganov/llama.cpp):
-
-- LLaMA
-- LLaMA 2
-- Falcon
-- [Alpaca](https://github.com/ggerganov/llama.cpp#instruction-mode-with-alpaca)
-- [GPT4All](https://github.com/ggerganov/llama.cpp#using-gpt4all)
-- [Chinese LLaMA / Alpaca](https://github.com/ymcui/Chinese-LLaMA-Alpaca) and [Chinese LLaMA-2 / Alpaca-2](https://github.com/ymcui/Chinese-LLaMA-Alpaca-2)
-- [Vigogne (French)](https://github.com/bofenghuang/vigogne)
-- [Vicuna](https://github.com/ggerganov/llama.cpp/discussions/643#discussioncomment-5533894)
-- [Koala](https://bair.berkeley.edu/blog/2023/04/03/koala/)
-- [OpenBuddy 🐶 (Multilingual)](https://github.com/OpenBuddy/OpenBuddy)
-- [Pygmalion 7B / Metharme 7B](#using-pygmalion-7b--metharme-7b)
-- [WizardLM](https://github.com/nlpxucan/WizardLM)
-- [Baichuan-7B](https://huggingface.co/baichuan-inc/baichuan-7B) and its derivations (such as [baichuan-7b-sft](https://huggingface.co/hiyouga/baichuan-7b-sft))
-- [Aquila-7B](https://huggingface.co/BAAI/Aquila-7B) / [AquilaChat-7B](https://huggingface.co/BAAI/AquilaChat-7B)
-- [Starcoder models](https://github.com/ggerganov/llama.cpp/pull/3187)
-- [Mistral AI v0.1](https://huggingface.co/mistralai/Mistral-7B-v0.1)
+- All open weights models supported by [llama.cpp](http://github.com/ggerganov/llama.cpp) will be compatible.
+- OpenAI / Azure compatible APIs
+- Mistral Large through La Plateforme or Azure
 
 ## Use cases
 
 PyLLMCore covers a narrow range of use cases and serves as a building brick:
 
 - Parsing: see the `parsers` module
 - Summarizing: see the `assistants.summarizers` module
 - Question answering: see the `assistants.analyst` module
 - Hallucinations reduction: see the `assistants.verifiers` module
 - Context size management: see the `splitters` module
-- Tokenizing, encoding, decoding: see the `token_codecs` module
+- Tokenizing: see the `token_codecs` module
 
 
-## Changelog
-
-- 2.8.3: Raised timeout
-- 2.8.1: Fixed bug when deserializing instances
-- 2.8.0: Added support for native type annotation (pep585) for lists and sets
-- 2.7.0: Fixed bug when function_call was set at None
-- 2.6.1: Add dynamic max_tokens computation for OpenAI
-- 2.6.0: Add support for Azure OpenAI
-- 2.5.1: Fix bug on system prompt format
-- 2.5.0: Add support for LLaVA models
-- 2.4.0:
-    + Set timeouts on OpenAI API
-- 2.2.0:
-    + Default settings on ARM64 MacOS modified (1 thread / offloading everything on the GPU)
-    + Added `completion_kwargs` for Assistants to set temperature
-- 2.1.0:
-    + Added support for Enum to provide better support for classification tasks
-    + Added example in the documentation
-- 2.0.0: 
-    + Refactored code
-    + Dynamically enable GPU offloading on MacOS
-    + Added configuration option for storing local models (MODELS_CACHE_DIR)
-    + Updated documentation
-
-- 1.4.0: Free up resources in LLamaParser when exiting the context manager
-- 1.3.0: Support for LLaMA based models (llama, llama2, Mistral Instruct)
-- 1.2.0: Chain of density prompting implemented with OpenAI
-- 1.1.0: Chain of Verification implemented with OpenAI
-- 1.0.0: Initial version
-
 ## Install
 
 ### Quick start
 
 ```shell
 pip install py-llm-core
 
@@ -867,7 +832,41 @@
         prompt_tokens=630,
         completion_tokens=62,
         total_tokens=692
     ),
     system_fingerprint=None
 )
 ```
+
+
+
+## Changelog
+
+- 2.8.5: Fix model path building
+- 2.8.4: Added support for Mistral Large
+- 2.8.3: Raised timeout
+- 2.8.1: Fixed bug when deserializing instances
+- 2.8.0: Added support for native type annotation (pep585) for lists and sets
+- 2.7.0: Fixed bug when function_call was set at None
+- 2.6.1: Add dynamic max_tokens computation for OpenAI
+- 2.6.0: Add support for Azure OpenAI
+- 2.5.1: Fix bug on system prompt format
+- 2.5.0: Add support for LLaVA models
+- 2.4.0:
+    + Set timeouts on OpenAI API
+- 2.2.0:
+    + Default settings on ARM64 MacOS modified (1 thread / offloading everything on the GPU)
+    + Added `completion_kwargs` for Assistants to set temperature
+- 2.1.0:
+    + Added support for Enum to provide better support for classification tasks
+    + Added example in the documentation
+- 2.0.0:
+    + Refactored code
+    + Dynamically enable GPU offloading on MacOS
+    + Added configuration option for storing local models (MODELS_CACHE_DIR)
+    + Updated documentation
+
+- 1.4.0: Free up resources in LLamaParser when exiting the context manager
+- 1.3.0: Support for LLaMA based models (llama, llama2, Mistral Instruct)
+- 1.2.0: Chain of density prompting implemented with OpenAI
+- 1.1.0: Chain of Verification implemented with OpenAI
+- 1.0.0: Initial version
```

### Comparing `py-llm-core-2.8.4/setup.py` & `py_llm_core-2.8.5/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -8,15 +8,15 @@
 main_package = packages[0]
 long_description = (here / "README.md").read_text()
 requirements = (here / "requirements.txt").read_text().splitlines()
 
 
 setup(
     name="py-llm-core",
-    version="2.8.4",
+    version="2.8.5",
     license="MIT",
     description="PyLLMCore provides a light-weighted interface with LLMs",
     long_description=long_description,
     long_description_content_type="text/markdown",
     author="P.A. SCHEMBRI",
     author_email="pa.schembri@advanced-stack.com",
     url="https://github.com/paschembri/py-llm-core",
```

### Comparing `py-llm-core-2.8.4/src/llm_core/assistants/__init__.py` & `py_llm_core-2.8.5/src/llm_core/assistants/__init__.py`

 * *Files identical despite different names*

### Comparing `py-llm-core-2.8.4/src/llm_core/assistants/analysts.py` & `py_llm_core-2.8.5/src/llm_core/assistants/analysts.py`

 * *Files identical despite different names*

### Comparing `py-llm-core-2.8.4/src/llm_core/assistants/base.py` & `py_llm_core-2.8.5/src/llm_core/assistants/base.py`

 * *Files identical despite different names*

### Comparing `py-llm-core-2.8.4/src/llm_core/assistants/summarizers.py` & `py_llm_core-2.8.5/src/llm_core/assistants/summarizers.py`

 * *Files identical despite different names*

### Comparing `py-llm-core-2.8.4/src/llm_core/assistants/verifiers.py` & `py_llm_core-2.8.5/src/llm_core/assistants/verifiers.py`

 * *Files identical despite different names*

### Comparing `py-llm-core-2.8.4/src/llm_core/llm/base.py` & `py_llm_core-2.8.5/src/llm_core/llm/base.py`

 * *Files identical despite different names*

### Comparing `py-llm-core-2.8.4/src/llm_core/llm/llama_cpp_compatible.py` & `py_llm_core-2.8.5/src/llm_core/llm/llama_cpp_compatible.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 # -*- coding: utf-8 -*-
-import os
+from pathlib import Path
 import platform
 import llama_cpp
 
 from dataclasses import dataclass
 
 from .base import (
     LLMBase,
@@ -47,15 +47,16 @@
             }
 
             if platform.system() == "Darwin" and platform.machine() == "arm64":
                 # Offload everything onto the GPU on MacOS
                 self.llama_cpp_kwargs["n_gpu_layers"] = 100
                 self.llama_cpp_kwargs["n_threads"] = 1
 
-        model_path = os.path.join(MODELS_CACHE_DIR, self.name)
+        model_path = str(Path(MODELS_CACHE_DIR) / self.name)
+
         self.model = llama_cpp.Llama(model_path, **self.llama_cpp_kwargs)
 
     def ask(
         self,
         prompt,
         history=None,
         schema=None,
@@ -116,15 +117,15 @@
             }
 
             if platform.system() == "Darwin" and platform.machine() == "arm64":
                 # Offload everything onto the GPU on MacOS
                 self.llama_cpp_kwargs["n_gpu_layers"] = 100
                 self.llama_cpp_kwargs["n_threads"] = 1
 
-        model_path = os.path.join(MODELS_CACHE_DIR, self.name)
+        model_path = str(Path(MODELS_CACHE_DIR) / self.name)
         chat_format = "llava-1-5"
         chat_handler = llama_cpp.llama_chat_format.Llava15ChatHandler(
             clip_model_path=self.llama_cpp_kwargs["clip_model_path"]
         )
 
         self.model = llama_cpp.Llama(
             model_path,
```

### Comparing `py-llm-core-2.8.4/src/llm_core/llm/mistralai.py` & `py_llm_core-2.8.5/src/llm_core/llm/mistralai.py`

 * *Files identical despite different names*

### Comparing `py-llm-core-2.8.4/src/llm_core/llm/openai.py` & `py_llm_core-2.8.5/src/llm_core/llm/openai.py`

 * *Files identical despite different names*

### Comparing `py-llm-core-2.8.4/src/llm_core/parsers.py` & `py_llm_core-2.8.5/src/llm_core/parsers.py`

 * *Files identical despite different names*

### Comparing `py-llm-core-2.8.4/src/llm_core/schema.py` & `py_llm_core-2.8.5/src/llm_core/schema.py`

 * *Files identical despite different names*

### Comparing `py-llm-core-2.8.4/src/llm_core/settings.py` & `py_llm_core-2.8.5/src/llm_core/settings.py`

 * *Files identical despite different names*

### Comparing `py-llm-core-2.8.4/src/llm_core/splitters.py` & `py_llm_core-2.8.5/src/llm_core/splitters.py`

 * *Files identical despite different names*

### Comparing `py-llm-core-2.8.4/src/llm_core/token_codecs.py` & `py_llm_core-2.8.5/src/llm_core/token_codecs.py`

 * *Files identical despite different names*

### Comparing `py-llm-core-2.8.4/src/py_llm_core.egg-info/PKG-INFO` & `py_llm_core-2.8.5/README.md`

 * *Files 6% similar despite different names*

```diff
@@ -1,117 +1,46 @@
-Metadata-Version: 2.1
-Name: py-llm-core
-Version: 2.8.4
-Summary: PyLLMCore provides a light-weighted interface with LLMs
-Home-page: https://github.com/paschembri/py-llm-core
-Author: P.A. SCHEMBRI
-Author-email: pa.schembri@advanced-stack.com
-License: MIT
-Description-Content-Type: text/markdown
-License-File: LICENSE
-Requires-Dist: openai<2,>=1.3.5
-Requires-Dist: tiktoken
-Requires-Dist: jsonschema
-Requires-Dist: dirtyjson
-Requires-Dist: llama-cpp-python>=0.2.20
-Requires-Dist: python-decouple
-Requires-Dist: mistralai
-
 # PyLLMCore
 
 ## Overview
 
-PyLLMCore is a light-weighted structured interface with Large Language Models 
-with native support for [llama.cpp](http://github.com/ggerganov/llama.cpp) and OpenAI API.
-
-The design decisions behind PyLLMCore are:
-
-- Sane defaults
-- Clear abstractions and terminology
-- Out of the box utility classes
+PyLLMCore is a light-weighted interface with Large Language Models
+with native support for [llama.cpp](http://github.com/ggerganov/llama.cpp), OpenAI API and Azure deployments.
 
-## Main benefits of using PyLLMCore
+## Expected benefits and reasons to use PyLLMCore
 
 - Pythonic API
 - Simple to use
-- You need structures *everywhere* (provided by the standard library `dataclasses` module)
+- Structures *everywhere* provided by the standard library `dataclasses` module
 - High-level API with the `assistants` module
-- Switching between models has never been easier
+- Easy swapping between models
 
 ## Why you shouldn't use PyLLMCore
 
-- You need a lot of external integrations: Take a look at [langchain](https://github.com/langchain-ai/langchain)
+- You need a whole framework: Take a look at [langchain](https://github.com/langchain-ai/langchain)
 - You need tremendous performance: Take a look at [vllm](https://github.com/vllm-project/vllm)
-- You don't need OpenAI: Take a look a [llama-cpp-python](https://github.com/abetlen/llama-cpp-python) (which is integrated in PyLLMCore)
-- You use Pydantic and don't use the dataclasses module
-
+- You want/need to use Pydantic and don't use the `dataclasses` module
 
 ## Models supported
 
-Besides OpenAI API, the following models are supported for local inference using the [llama.cpp](http://github.com/ggerganov/llama.cpp):
-
-- LLaMA
-- LLaMA 2
-- Falcon
-- [Alpaca](https://github.com/ggerganov/llama.cpp#instruction-mode-with-alpaca)
-- [GPT4All](https://github.com/ggerganov/llama.cpp#using-gpt4all)
-- [Chinese LLaMA / Alpaca](https://github.com/ymcui/Chinese-LLaMA-Alpaca) and [Chinese LLaMA-2 / Alpaca-2](https://github.com/ymcui/Chinese-LLaMA-Alpaca-2)
-- [Vigogne (French)](https://github.com/bofenghuang/vigogne)
-- [Vicuna](https://github.com/ggerganov/llama.cpp/discussions/643#discussioncomment-5533894)
-- [Koala](https://bair.berkeley.edu/blog/2023/04/03/koala/)
-- [OpenBuddy 🐶 (Multilingual)](https://github.com/OpenBuddy/OpenBuddy)
-- [Pygmalion 7B / Metharme 7B](#using-pygmalion-7b--metharme-7b)
-- [WizardLM](https://github.com/nlpxucan/WizardLM)
-- [Baichuan-7B](https://huggingface.co/baichuan-inc/baichuan-7B) and its derivations (such as [baichuan-7b-sft](https://huggingface.co/hiyouga/baichuan-7b-sft))
-- [Aquila-7B](https://huggingface.co/BAAI/Aquila-7B) / [AquilaChat-7B](https://huggingface.co/BAAI/AquilaChat-7B)
-- [Starcoder models](https://github.com/ggerganov/llama.cpp/pull/3187)
-- [Mistral AI v0.1](https://huggingface.co/mistralai/Mistral-7B-v0.1)
+- All open weights models supported by [llama.cpp](http://github.com/ggerganov/llama.cpp) will be compatible.
+- OpenAI / Azure compatible APIs
+- Mistral Large through La Plateforme or Azure
 
 ## Use cases
 
 PyLLMCore covers a narrow range of use cases and serves as a building brick:
 
 - Parsing: see the `parsers` module
 - Summarizing: see the `assistants.summarizers` module
 - Question answering: see the `assistants.analyst` module
 - Hallucinations reduction: see the `assistants.verifiers` module
 - Context size management: see the `splitters` module
-- Tokenizing, encoding, decoding: see the `token_codecs` module
+- Tokenizing: see the `token_codecs` module
 
 
-## Changelog
-
-- 2.8.3: Raised timeout
-- 2.8.1: Fixed bug when deserializing instances
-- 2.8.0: Added support for native type annotation (pep585) for lists and sets
-- 2.7.0: Fixed bug when function_call was set at None
-- 2.6.1: Add dynamic max_tokens computation for OpenAI
-- 2.6.0: Add support for Azure OpenAI
-- 2.5.1: Fix bug on system prompt format
-- 2.5.0: Add support for LLaVA models
-- 2.4.0:
-    + Set timeouts on OpenAI API
-- 2.2.0:
-    + Default settings on ARM64 MacOS modified (1 thread / offloading everything on the GPU)
-    + Added `completion_kwargs` for Assistants to set temperature
-- 2.1.0:
-    + Added support for Enum to provide better support for classification tasks
-    + Added example in the documentation
-- 2.0.0: 
-    + Refactored code
-    + Dynamically enable GPU offloading on MacOS
-    + Added configuration option for storing local models (MODELS_CACHE_DIR)
-    + Updated documentation
-
-- 1.4.0: Free up resources in LLamaParser when exiting the context manager
-- 1.3.0: Support for LLaMA based models (llama, llama2, Mistral Instruct)
-- 1.2.0: Chain of density prompting implemented with OpenAI
-- 1.1.0: Chain of Verification implemented with OpenAI
-- 1.0.0: Initial version
-
 ## Install
 
 ### Quick start
 
 ```shell
 pip install py-llm-core
 
@@ -885,7 +814,41 @@
         prompt_tokens=630,
         completion_tokens=62,
         total_tokens=692
     ),
     system_fingerprint=None
 )
 ```
+
+
+
+## Changelog
+
+- 2.8.5: Fix model path building
+- 2.8.4: Added support for Mistral Large
+- 2.8.3: Raised timeout
+- 2.8.1: Fixed bug when deserializing instances
+- 2.8.0: Added support for native type annotation (pep585) for lists and sets
+- 2.7.0: Fixed bug when function_call was set at None
+- 2.6.1: Add dynamic max_tokens computation for OpenAI
+- 2.6.0: Add support for Azure OpenAI
+- 2.5.1: Fix bug on system prompt format
+- 2.5.0: Add support for LLaVA models
+- 2.4.0:
+    + Set timeouts on OpenAI API
+- 2.2.0:
+    + Default settings on ARM64 MacOS modified (1 thread / offloading everything on the GPU)
+    + Added `completion_kwargs` for Assistants to set temperature
+- 2.1.0:
+    + Added support for Enum to provide better support for classification tasks
+    + Added example in the documentation
+- 2.0.0:
+    + Refactored code
+    + Dynamically enable GPU offloading on MacOS
+    + Added configuration option for storing local models (MODELS_CACHE_DIR)
+    + Updated documentation
+
+- 1.4.0: Free up resources in LLamaParser when exiting the context manager
+- 1.3.0: Support for LLaMA based models (llama, llama2, Mistral Instruct)
+- 1.2.0: Chain of density prompting implemented with OpenAI
+- 1.1.0: Chain of Verification implemented with OpenAI
+- 1.0.0: Initial version
```

### Comparing `py-llm-core-2.8.4/src/py_llm_core.egg-info/SOURCES.txt` & `py_llm_core-2.8.5/src/py_llm_core.egg-info/SOURCES.txt`

 * *Files identical despite different names*

