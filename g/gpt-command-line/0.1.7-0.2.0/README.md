# Comparing `tmp/gpt_command_line-0.1.7.tar.gz` & `tmp/gpt_command_line-0.2.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "gpt_command_line-0.1.7.tar", last modified: Wed May 15 03:36:16 2024, max compression
+gzip compressed data, was "gpt_command_line-0.2.0.tar", last modified: Wed May 29 03:30:14 2024, max compression
```

## Comparing `gpt_command_line-0.1.7.tar` & `gpt_command_line-0.2.0.tar`

### file list

```diff
@@ -1,33 +1,36 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-15 03:36:16.297333 gpt_command_line-0.1.7/
--rw-r--r--   0 runner    (1001) docker     (127)     1069 2024-05-15 03:36:09.000000 gpt_command_line-0.1.7/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)    11224 2024-05-15 03:36:16.297333 gpt_command_line-0.1.7/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     8850 2024-05-15 03:36:09.000000 gpt_command_line-0.1.7/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-15 03:36:16.297333 gpt_command_line-0.1.7/gpt_command_line.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)    11224 2024-05-15 03:36:16.000000 gpt_command_line-0.1.7/gpt_command_line.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      607 2024-05-15 03:36:16.000000 gpt_command_line-0.1.7/gpt_command_line.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-15 03:36:16.000000 gpt_command_line-0.1.7/gpt_command_line.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       40 2024-05-15 03:36:16.000000 gpt_command_line-0.1.7/gpt_command_line.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (127)      229 2024-05-15 03:36:16.000000 gpt_command_line-0.1.7/gpt_command_line.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)        7 2024-05-15 03:36:16.000000 gpt_command_line-0.1.7/gpt_command_line.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-15 03:36:16.293333 gpt_command_line-0.1.7/gptcli/
--rw-r--r--   0 runner    (1001) docker     (127)       22 2024-05-15 03:36:09.000000 gpt_command_line-0.1.7/gptcli/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     4119 2024-05-15 03:36:09.000000 gpt_command_line-0.1.7/gptcli/anthropic.py
--rw-r--r--   0 runner    (1001) docker     (127)     5121 2024-05-15 03:36:09.000000 gpt_command_line-0.1.7/gptcli/assistant.py
--rw-r--r--   0 runner    (1001) docker     (127)     6810 2024-05-15 03:36:09.000000 gpt_command_line-0.1.7/gptcli/cli.py
--rw-r--r--   0 runner    (1001) docker     (127)     1373 2024-05-15 03:36:09.000000 gpt_command_line-0.1.7/gptcli/completion.py
--rw-r--r--   0 runner    (1001) docker     (127)     1861 2024-05-15 03:36:09.000000 gpt_command_line-0.1.7/gptcli/composite.py
--rw-r--r--   0 runner    (1001) docker     (127)     1356 2024-05-15 03:36:09.000000 gpt_command_line-0.1.7/gptcli/config.py
--rw-r--r--   0 runner    (1001) docker     (127)     1422 2024-05-15 03:36:09.000000 gpt_command_line-0.1.7/gptcli/cost.py
--rw-r--r--   0 runner    (1001) docker     (127)     1346 2024-05-15 03:36:09.000000 gpt_command_line-0.1.7/gptcli/google.py
--rwxr-xr-x   0 runner    (1001) docker     (127)     7898 2024-05-15 03:36:09.000000 gpt_command_line-0.1.7/gptcli/gpt.py
--rw-r--r--   0 runner    (1001) docker     (127)     3682 2024-05-15 03:36:09.000000 gpt_command_line-0.1.7/gptcli/llama.py
--rw-r--r--   0 runner    (1001) docker     (127)      693 2024-05-15 03:36:09.000000 gpt_command_line-0.1.7/gptcli/logging.py
--rw-r--r--   0 runner    (1001) docker     (127)     4397 2024-05-15 03:36:09.000000 gpt_command_line-0.1.7/gptcli/openai.py
--rw-r--r--   0 runner    (1001) docker     (127)     5955 2024-05-15 03:36:09.000000 gpt_command_line-0.1.7/gptcli/session.py
--rw-r--r--   0 runner    (1001) docker     (127)     1735 2024-05-15 03:36:09.000000 gpt_command_line-0.1.7/gptcli/shell.py
--rw-r--r--   0 runner    (1001) docker     (127)     1375 2024-05-15 03:36:09.000000 gpt_command_line-0.1.7/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-15 03:36:16.297333 gpt_command_line-0.1.7/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-15 03:36:16.297333 gpt_command_line-0.1.7/tests/
--rw-r--r--   0 runner    (1001) docker     (127)     2120 2024-05-15 03:36:09.000000 gpt_command_line-0.1.7/tests/test_assistant.py
--rw-r--r--   0 runner    (1001) docker     (127)     9317 2024-05-15 03:36:09.000000 gpt_command_line-0.1.7/tests/test_session.py
--rw-r--r--   0 runner    (1001) docker     (127)      551 2024-05-15 03:36:09.000000 gpt_command_line-0.1.7/tests/test_term_utils.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-29 03:30:14.910144 gpt_command_line-0.2.0/
+-rw-r--r--   0 runner    (1001) docker     (127)     1069 2024-05-29 03:30:07.000000 gpt_command_line-0.2.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)    11271 2024-05-29 03:30:14.910144 gpt_command_line-0.2.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     8890 2024-05-29 03:30:07.000000 gpt_command_line-0.2.0/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-29 03:30:14.910144 gpt_command_line-0.2.0/gpt_command_line.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)    11271 2024-05-29 03:30:14.000000 gpt_command_line-0.2.0/gpt_command_line.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      703 2024-05-29 03:30:14.000000 gpt_command_line-0.2.0/gpt_command_line.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-29 03:30:14.000000 gpt_command_line-0.2.0/gpt_command_line.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       40 2024-05-29 03:30:14.000000 gpt_command_line-0.2.0/gpt_command_line.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      243 2024-05-29 03:30:14.000000 gpt_command_line-0.2.0/gpt_command_line.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        7 2024-05-29 03:30:14.000000 gpt_command_line-0.2.0/gpt_command_line.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-29 03:30:14.906144 gpt_command_line-0.2.0/gptcli/
+-rw-r--r--   0 runner    (1001) docker     (127)       22 2024-05-29 03:30:07.000000 gpt_command_line-0.2.0/gptcli/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5326 2024-05-29 03:30:07.000000 gpt_command_line-0.2.0/gptcli/assistant.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6810 2024-05-29 03:30:07.000000 gpt_command_line-0.2.0/gptcli/cli.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1373 2024-05-29 03:30:07.000000 gpt_command_line-0.2.0/gptcli/completion.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1861 2024-05-29 03:30:07.000000 gpt_command_line-0.2.0/gptcli/composite.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1435 2024-05-29 03:30:07.000000 gpt_command_line-0.2.0/gptcli/config.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1422 2024-05-29 03:30:07.000000 gpt_command_line-0.2.0/gptcli/cost.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)     8054 2024-05-29 03:30:07.000000 gpt_command_line-0.2.0/gptcli/gpt.py
+-rw-r--r--   0 runner    (1001) docker     (127)      693 2024-05-29 03:30:07.000000 gpt_command_line-0.2.0/gptcli/logging.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-29 03:30:14.906144 gpt_command_line-0.2.0/gptcli/providers/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-29 03:30:07.000000 gpt_command_line-0.2.0/gptcli/providers/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4119 2024-05-29 03:30:07.000000 gpt_command_line-0.2.0/gptcli/providers/anthropic.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4543 2024-05-29 03:30:07.000000 gpt_command_line-0.2.0/gptcli/providers/cohere.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3494 2024-05-29 03:30:07.000000 gpt_command_line-0.2.0/gptcli/providers/google.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3682 2024-05-29 03:30:07.000000 gpt_command_line-0.2.0/gptcli/providers/llama.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4397 2024-05-29 03:30:07.000000 gpt_command_line-0.2.0/gptcli/providers/openai.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5955 2024-05-29 03:30:07.000000 gpt_command_line-0.2.0/gptcli/session.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1869 2024-05-29 03:30:07.000000 gpt_command_line-0.2.0/gptcli/shell.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1368 2024-05-29 03:30:07.000000 gpt_command_line-0.2.0/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-29 03:30:14.910144 gpt_command_line-0.2.0/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-29 03:30:14.906144 gpt_command_line-0.2.0/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)     2120 2024-05-29 03:30:07.000000 gpt_command_line-0.2.0/tests/test_assistant.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9317 2024-05-29 03:30:07.000000 gpt_command_line-0.2.0/tests/test_session.py
+-rw-r--r--   0 runner    (1001) docker     (127)      551 2024-05-29 03:30:07.000000 gpt_command_line-0.2.0/tests/test_term_utils.py
```

### Comparing `gpt_command_line-0.1.7/LICENSE` & `gpt_command_line-0.2.0/LICENSE`

 * *Files identical despite different names*

### Comparing `gpt_command_line-0.1.7/PKG-INFO` & `gpt_command_line-0.2.0/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,56 +1,63 @@
 Metadata-Version: 2.1
 Name: gpt-command-line
-Version: 0.1.7
-Summary: Command-line interface for ChatGPT, Claude and Bard
+Version: 0.2.0
+Summary: Command-line interface for ChatGPT and Claude
 Author-email: Val Kharitonov <val@kharvd.com>
 License: Copyright (c) 2023 by Val Kharitonov
         
         Permission is hereby granted, free of charge, to any person obtaining a copy of this software and associated documentation files (the “Software”), to deal in the Software without restriction, including without limitation the rights to use, copy, modify, merge, publish, distribute, sublicense, and/or sell copies of the Software, and to permit persons to whom the Software is furnished to do so, subject to the following conditions:
         
         The above copyright notice and this permission notice shall be included in all copies or substantial portions of the Software.
         
         THE SOFTWARE IS PROVIDED “AS IS”, WITHOUT WARRANTY OF ANY KIND, EXPRESS OR IMPLIED, INCLUDING BUT NOT LIMITED TO THE WARRANTIES OF MERCHANTABILITY, FITNESS FOR A PARTICULAR PURPOSE AND NONINFRINGEMENT. IN NO EVENT SHALL THE AUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER LIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING FROM, OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN THE SOFTWARE.
         
 Project-URL: Homepage, https://github.com/kharvd/gpt-cli
-Keywords: cli,command-line,assistant,openai,claude,bard,gpt-3,gpt-4,llm,chatgpt,gpt-cli,google-bard,anthropic,gpt-client,anthropic-claude,palm2
+Keywords: cli,command-line,assistant,openai,claude,cohere,gpt-3,gpt-4,llm,chatgpt,gpt-cli,anthropic,gpt-client,anthropic-claude
 Classifier: Development Status :: 4 - Beta
 Classifier: Environment :: Console
 Classifier: Intended Audience :: Developers
 Classifier: Intended Audience :: End Users/Desktop
 Classifier: Intended Audience :: Science/Research
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Topic :: Scientific/Engineering :: Artificial Intelligence
 Requires-Python: >=3.9
 Description-Content-Type: text/markdown
 License-File: LICENSE
 Requires-Dist: anthropic==0.25.9
 Requires-Dist: attrs==23.2.0
 Requires-Dist: black==24.4.2
+Requires-Dist: cohere==5.5.3
+Requires-Dist: google-generativeai==0.5.4
 Requires-Dist: mistralai==0.1.8
-Requires-Dist: google-generativeai==0.1.0
 Requires-Dist: openai==1.30.1
 Requires-Dist: prompt-toolkit==3.0.43
 Requires-Dist: pytest==7.3.1
 Requires-Dist: PyYAML==6.0.1
 Requires-Dist: rich==13.7.1
 Requires-Dist: typing_extensions==4.11.0
 Provides-Extra: llama
 Requires-Dist: llama-cpp-python==0.2.74; extra == "llama"
 
 # gpt-cli
 
-Command-line interface for ChatGPT Claude and Bard.
+Command-line interface for chat LLMs.
+
+## Supported providers
+
+- OpenAI
+- Anthropic
+- Google Gemini
+- Cohere
+- Other APIs compatible with OpenAI (e.g. Together, OpenRouter, local models with LM Studio)
 
 ![screenshot](https://github.com/kharvd/gpt-cli/assets/466920/ecbcccc4-7cfa-4c04-83c3-a822b6596f01)
 
 ## Features
 
-### **Coming soon** - Code Interpreter support https://github.com/kharvd/gpt-cli/pull/37
-
 - **Command-Line Interface**: Interact with ChatGPT or Claude directly from your terminal.
 - **Model Customization**: Override the default model, temperature, and top_p values for each assistant, giving you fine-grained control over the AI's behavior.
 - **Usage tracking**: Track your API usage with token count and price information.
 - **Keyboard Shortcuts**: Use Ctrl-C, Ctrl-D, and Ctrl-R shortcuts for easier conversation management and input control.
 - **Multi-Line Input**: Enter multi-line mode for more complex queries or conversations.
 - **Markdown Support**: Enable or disable markdown formatting for chat sessions to tailor the output to your preferences.
 - **Predefined Messages**: Set up predefined messages for your custom assistants to establish context or role-play scenarios.
@@ -244,32 +251,36 @@
 
 or a config line in `~/.config/gpt-cli/gpt.yml`:
 
 ```yaml
 anthropic_api_key: <your_key_here>
 ```
 
-Now you should be able to run `gpt` with `--model claude-v1` or `--model claude-instant-v1`:
+Now you should be able to run `gpt` with `--model claude-3-(opus|sonnet|haiku)-<date>`.
 
 ```bash
-gpt --model claude-v1
+gpt --model claude-3-opus-20240229
 ```
 
-### Google Bard (PaLM 2)
-
-Similar to Claude, set the Google API key
+### Google Gemini
 
 ```bash
 export GOOGLE_API_KEY=<your_key_here>
 ```
 
-or a config line:
+or
 
 ```yaml
 google_api_key: <your_key_here>
 ```
 
-Run `gpt` with the correct model:
+### Cohere
 
 ```bash
-gpt --model chat-bison-001
+export COHERE_API_KEY=<your_key_here>
+```
+
+or
+
+```yaml
+cohere_api_key: <your_key_here>
 ```
```

### Comparing `gpt_command_line-0.1.7/README.md` & `gpt_command_line-0.2.0/README.md`

 * *Files 5% similar despite different names*

```diff
@@ -1,17 +1,23 @@
 # gpt-cli
 
-Command-line interface for ChatGPT Claude and Bard.
+Command-line interface for chat LLMs.
+
+## Supported providers
+
+- OpenAI
+- Anthropic
+- Google Gemini
+- Cohere
+- Other APIs compatible with OpenAI (e.g. Together, OpenRouter, local models with LM Studio)
 
 ![screenshot](https://github.com/kharvd/gpt-cli/assets/466920/ecbcccc4-7cfa-4c04-83c3-a822b6596f01)
 
 ## Features
 
-### **Coming soon** - Code Interpreter support https://github.com/kharvd/gpt-cli/pull/37
-
 - **Command-Line Interface**: Interact with ChatGPT or Claude directly from your terminal.
 - **Model Customization**: Override the default model, temperature, and top_p values for each assistant, giving you fine-grained control over the AI's behavior.
 - **Usage tracking**: Track your API usage with token count and price information.
 - **Keyboard Shortcuts**: Use Ctrl-C, Ctrl-D, and Ctrl-R shortcuts for easier conversation management and input control.
 - **Multi-Line Input**: Enter multi-line mode for more complex queries or conversations.
 - **Markdown Support**: Enable or disable markdown formatting for chat sessions to tailor the output to your preferences.
 - **Predefined Messages**: Set up predefined messages for your custom assistants to establish context or role-play scenarios.
@@ -205,32 +211,36 @@
 
 or a config line in `~/.config/gpt-cli/gpt.yml`:
 
 ```yaml
 anthropic_api_key: <your_key_here>
 ```
 
-Now you should be able to run `gpt` with `--model claude-v1` or `--model claude-instant-v1`:
+Now you should be able to run `gpt` with `--model claude-3-(opus|sonnet|haiku)-<date>`.
 
 ```bash
-gpt --model claude-v1
+gpt --model claude-3-opus-20240229
 ```
 
-### Google Bard (PaLM 2)
-
-Similar to Claude, set the Google API key
+### Google Gemini
 
 ```bash
 export GOOGLE_API_KEY=<your_key_here>
 ```
 
-or a config line:
+or
 
 ```yaml
 google_api_key: <your_key_here>
 ```
 
-Run `gpt` with the correct model:
+### Cohere
 
 ```bash
-gpt --model chat-bison-001
+export COHERE_API_KEY=<your_key_here>
+```
+
+or
+
+```yaml
+cohere_api_key: <your_key_here>
 ```
```

### Comparing `gpt_command_line-0.1.7/gpt_command_line.egg-info/PKG-INFO` & `gpt_command_line-0.2.0/gpt_command_line.egg-info/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,56 +1,63 @@
 Metadata-Version: 2.1
 Name: gpt-command-line
-Version: 0.1.7
-Summary: Command-line interface for ChatGPT, Claude and Bard
+Version: 0.2.0
+Summary: Command-line interface for ChatGPT and Claude
 Author-email: Val Kharitonov <val@kharvd.com>
 License: Copyright (c) 2023 by Val Kharitonov
         
         Permission is hereby granted, free of charge, to any person obtaining a copy of this software and associated documentation files (the “Software”), to deal in the Software without restriction, including without limitation the rights to use, copy, modify, merge, publish, distribute, sublicense, and/or sell copies of the Software, and to permit persons to whom the Software is furnished to do so, subject to the following conditions:
         
         The above copyright notice and this permission notice shall be included in all copies or substantial portions of the Software.
         
         THE SOFTWARE IS PROVIDED “AS IS”, WITHOUT WARRANTY OF ANY KIND, EXPRESS OR IMPLIED, INCLUDING BUT NOT LIMITED TO THE WARRANTIES OF MERCHANTABILITY, FITNESS FOR A PARTICULAR PURPOSE AND NONINFRINGEMENT. IN NO EVENT SHALL THE AUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER LIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING FROM, OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN THE SOFTWARE.
         
 Project-URL: Homepage, https://github.com/kharvd/gpt-cli
-Keywords: cli,command-line,assistant,openai,claude,bard,gpt-3,gpt-4,llm,chatgpt,gpt-cli,google-bard,anthropic,gpt-client,anthropic-claude,palm2
+Keywords: cli,command-line,assistant,openai,claude,cohere,gpt-3,gpt-4,llm,chatgpt,gpt-cli,anthropic,gpt-client,anthropic-claude
 Classifier: Development Status :: 4 - Beta
 Classifier: Environment :: Console
 Classifier: Intended Audience :: Developers
 Classifier: Intended Audience :: End Users/Desktop
 Classifier: Intended Audience :: Science/Research
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Topic :: Scientific/Engineering :: Artificial Intelligence
 Requires-Python: >=3.9
 Description-Content-Type: text/markdown
 License-File: LICENSE
 Requires-Dist: anthropic==0.25.9
 Requires-Dist: attrs==23.2.0
 Requires-Dist: black==24.4.2
+Requires-Dist: cohere==5.5.3
+Requires-Dist: google-generativeai==0.5.4
 Requires-Dist: mistralai==0.1.8
-Requires-Dist: google-generativeai==0.1.0
 Requires-Dist: openai==1.30.1
 Requires-Dist: prompt-toolkit==3.0.43
 Requires-Dist: pytest==7.3.1
 Requires-Dist: PyYAML==6.0.1
 Requires-Dist: rich==13.7.1
 Requires-Dist: typing_extensions==4.11.0
 Provides-Extra: llama
 Requires-Dist: llama-cpp-python==0.2.74; extra == "llama"
 
 # gpt-cli
 
-Command-line interface for ChatGPT Claude and Bard.
+Command-line interface for chat LLMs.
+
+## Supported providers
+
+- OpenAI
+- Anthropic
+- Google Gemini
+- Cohere
+- Other APIs compatible with OpenAI (e.g. Together, OpenRouter, local models with LM Studio)
 
 ![screenshot](https://github.com/kharvd/gpt-cli/assets/466920/ecbcccc4-7cfa-4c04-83c3-a822b6596f01)
 
 ## Features
 
-### **Coming soon** - Code Interpreter support https://github.com/kharvd/gpt-cli/pull/37
-
 - **Command-Line Interface**: Interact with ChatGPT or Claude directly from your terminal.
 - **Model Customization**: Override the default model, temperature, and top_p values for each assistant, giving you fine-grained control over the AI's behavior.
 - **Usage tracking**: Track your API usage with token count and price information.
 - **Keyboard Shortcuts**: Use Ctrl-C, Ctrl-D, and Ctrl-R shortcuts for easier conversation management and input control.
 - **Multi-Line Input**: Enter multi-line mode for more complex queries or conversations.
 - **Markdown Support**: Enable or disable markdown formatting for chat sessions to tailor the output to your preferences.
 - **Predefined Messages**: Set up predefined messages for your custom assistants to establish context or role-play scenarios.
@@ -244,32 +251,36 @@
 
 or a config line in `~/.config/gpt-cli/gpt.yml`:
 
 ```yaml
 anthropic_api_key: <your_key_here>
 ```
 
-Now you should be able to run `gpt` with `--model claude-v1` or `--model claude-instant-v1`:
+Now you should be able to run `gpt` with `--model claude-3-(opus|sonnet|haiku)-<date>`.
 
 ```bash
-gpt --model claude-v1
+gpt --model claude-3-opus-20240229
 ```
 
-### Google Bard (PaLM 2)
-
-Similar to Claude, set the Google API key
+### Google Gemini
 
 ```bash
 export GOOGLE_API_KEY=<your_key_here>
 ```
 
-or a config line:
+or
 
 ```yaml
 google_api_key: <your_key_here>
 ```
 
-Run `gpt` with the correct model:
+### Cohere
 
 ```bash
-gpt --model chat-bison-001
+export COHERE_API_KEY=<your_key_here>
+```
+
+or
+
+```yaml
+cohere_api_key: <your_key_here>
 ```
```

### Comparing `gpt_command_line-0.1.7/gptcli/anthropic.py` & `gpt_command_line-0.2.0/gptcli/providers/anthropic.py`

 * *Files identical despite different names*

### Comparing `gpt_command_line-0.1.7/gptcli/assistant.py` & `gpt_command_line-0.2.0/gptcli/assistant.py`

 * *Files 8% similar despite different names*

```diff
@@ -6,18 +6,19 @@
 
 from gptcli.completion import (
     CompletionEvent,
     CompletionProvider,
     ModelOverrides,
     Message,
 )
-from gptcli.google import GoogleCompletionProvider
-from gptcli.llama import LLaMACompletionProvider
-from gptcli.openai import OpenAICompletionProvider
-from gptcli.anthropic import AnthropicCompletionProvider
+from gptcli.providers.google import GoogleCompletionProvider
+from gptcli.providers.llama import LLaMACompletionProvider
+from gptcli.providers.openai import OpenAICompletionProvider
+from gptcli.providers.anthropic import AnthropicCompletionProvider
+from gptcli.providers.cohere import CohereCompletionProvider
 
 
 class AssistantConfig(TypedDict, total=False):
     messages: List[Message]
     model: str
     temperature: float
     top_p: float
@@ -72,15 +73,17 @@
         or model.startswith("oai-compat:")
     ):
         return OpenAICompletionProvider()
     elif model.startswith("claude"):
         return AnthropicCompletionProvider()
     elif model.startswith("llama"):
         return LLaMACompletionProvider()
-    elif model.startswith("chat-bison"):
+    elif model.startswith("command") or model.startswith("c4ai"):
+        return CohereCompletionProvider()
+    elif model.startswith("gemini"):
         return GoogleCompletionProvider()
     else:
         raise ValueError(f"Unknown model: {model}")
 
 
 class Assistant:
     def __init__(self, config: AssistantConfig):
```

### Comparing `gpt_command_line-0.1.7/gptcli/cli.py` & `gpt_command_line-0.2.0/gptcli/cli.py`

 * *Files identical despite different names*

### Comparing `gpt_command_line-0.1.7/gptcli/completion.py` & `gpt_command_line-0.2.0/gptcli/completion.py`

 * *Files identical despite different names*

### Comparing `gpt_command_line-0.1.7/gptcli/composite.py` & `gpt_command_line-0.2.0/gptcli/composite.py`

 * *Files identical despite different names*

### Comparing `gpt_command_line-0.1.7/gptcli/config.py` & `gpt_command_line-0.2.0/gptcli/config.py`

 * *Files 9% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 import os
 from typing import Dict, List, Optional
 from attr import dataclass
 import yaml
 
 from gptcli.assistant import AssistantConfig
-from gptcli.llama import LLaMAModelConfig
+from gptcli.providers.llama import LLaMAModelConfig
 
 
 CONFIG_FILE_PATHS = [
     os.path.join(os.path.expanduser("~"), ".config", "gpt-cli", "gpt.yml"),
     os.path.join(os.path.expanduser("~"), ".gptrc"),
 ]
 
@@ -19,14 +19,15 @@
     markdown: bool = True
     show_price: bool = True
     api_key: Optional[str] = os.environ.get("OPENAI_API_KEY")
     openai_api_key: Optional[str] = os.environ.get("OPENAI_API_KEY")
     openai_base_url: Optional[str] = os.environ.get("OPENAI_BASE_URL")
     anthropic_api_key: Optional[str] = os.environ.get("ANTHROPIC_API_KEY")
     google_api_key: Optional[str] = os.environ.get("GOOGLE_API_KEY")
+    cohere_api_key: Optional[str] = os.environ.get("COHERE_API_KEY")
     log_file: Optional[str] = None
     log_level: str = "INFO"
     assistants: Dict[str, AssistantConfig] = {}
     interactive: Optional[bool] = None
     llama_models: Optional[Dict[str, LLaMAModelConfig]] = None
```

### Comparing `gpt_command_line-0.1.7/gptcli/cost.py` & `gpt_command_line-0.2.0/gptcli/cost.py`

 * *Files identical despite different names*

### Comparing `gpt_command_line-0.1.7/gptcli/gpt.py` & `gpt_command_line-0.2.0/gptcli/gpt.py`

 * *Files 2% similar despite different names*

```diff
@@ -5,20 +5,21 @@
 MIN_PYTHON = (3, 9)
 if sys.version_info < MIN_PYTHON:
     sys.exit("Python %s.%s or later is required.\n" % MIN_PYTHON)
 
 import os
 from typing import cast
 import openai
+import google.generativeai as genai
 import argparse
 import sys
 import logging
 import datetime
-import google.generativeai as genai
-import gptcli.anthropic
+import gptcli.providers.anthropic
+import gptcli.providers.cohere
 from gptcli.assistant import (
     Assistant,
     DEFAULT_ASSISTANTS,
     AssistantGlobalArgs,
     init_assistant,
 )
 from gptcli.cli import (
@@ -28,15 +29,15 @@
 from gptcli.composite import CompositeChatListener
 from gptcli.config import (
     CONFIG_FILE_PATHS,
     GptCliConfig,
     choose_config_file,
     read_yaml_config,
 )
-from gptcli.llama import init_llama_models
+from gptcli.providers.llama import init_llama_models
 from gptcli.logging import LoggingChatListener
 from gptcli.cost import PriceChatListener
 from gptcli.session import ChatSession
 from gptcli.shell import execute, simple_response
 
 
 logger = logging.getLogger("gptcli")
@@ -180,15 +181,18 @@
 
     if config.api_key:
         openai.api_key = config.api_key
     elif config.openai_api_key:
         openai.api_key = config.openai_api_key
 
     if config.anthropic_api_key:
-        gptcli.anthropic.api_key = config.anthropic_api_key
+        gptcli.providers.anthropic.api_key = config.anthropic_api_key
+
+    if config.cohere_api_key:
+        gptcli.providers.cohere.api_key = config.cohere_api_key
 
     if config.google_api_key:
         genai.configure(api_key=config.google_api_key)
 
     if config.llama_models is not None:
         init_llama_models(config.llama_models)
```

### Comparing `gpt_command_line-0.1.7/gptcli/llama.py` & `gpt_command_line-0.2.0/gptcli/providers/llama.py`

 * *Files identical despite different names*

### Comparing `gpt_command_line-0.1.7/gptcli/logging.py` & `gpt_command_line-0.2.0/gptcli/logging.py`

 * *Files identical despite different names*

### Comparing `gpt_command_line-0.1.7/gptcli/openai.py` & `gpt_command_line-0.2.0/gptcli/providers/openai.py`

 * *Files identical despite different names*

### Comparing `gpt_command_line-0.1.7/gptcli/session.py` & `gpt_command_line-0.2.0/gptcli/session.py`

 * *Files identical despite different names*

### Comparing `gpt_command_line-0.1.7/gptcli/shell.py` & `gpt_command_line-0.2.0/gptcli/shell.py`

 * *Files 22% similar despite different names*

```diff
@@ -10,29 +10,32 @@
     messages = assistant.init_messages()
     messages.append({"role": "user", "content": prompt})
     logging.info("User: %s", prompt)
     response_iter = assistant.complete_chat(messages, stream=stream)
     result = ""
     try:
         for response in response_iter:
-            result += response
-            sys.stdout.write(response)
+            if response.type == "message_delta":
+                result += response.text
+                sys.stdout.write(response.text)
     except KeyboardInterrupt:
         pass
     finally:
         sys.stdout.flush()
         logging.info("Assistant: %s", result)
 
 
 def execute(assistant: Assistant, prompt: str) -> None:
     messages = assistant.init_messages()
     messages.append({"role": "user", "content": prompt})
     logging.info("User: %s", prompt)
     response_iter = assistant.complete_chat(messages, stream=False)
     result = next(response_iter)
+    assert result.type == "message_delta"
+    result = result.text
     logging.info("Assistant: %s", result)
 
     with tempfile.NamedTemporaryFile(mode="w", prefix="gptcli-", delete=False) as f:
         f.write("# Edit the command to execute below. Save and exit to execute it.\n")
         f.write("# Delete the contents to cancel.\n")
         f.write(result)
         f.flush()
```

### Comparing `gpt_command_line-0.1.7/pyproject.toml` & `gpt_command_line-0.2.0/pyproject.toml`

 * *Files 12% similar despite different names*

```diff
@@ -1,31 +1,32 @@
 [project]
 name = "gpt-command-line"
-version = "0.1.7"
-description = "Command-line interface for ChatGPT, Claude and Bard"
+version = "0.2.0"
+description = "Command-line interface for ChatGPT and Claude"
 authors = [{name = "Val Kharitonov", email = "val@kharvd.com"}]
 readme = "README.md"
 license = {file = "LICENSE"}
 requires-python = ">=3.9"
-keywords = ["cli", "command-line", "assistant", "openai", "claude", "bard", "gpt-3", "gpt-4", "llm", "chatgpt", "gpt-cli", "google-bard", "anthropic", "gpt-client", "anthropic-claude", "palm2"]
+keywords = ["cli", "command-line", "assistant", "openai", "claude", "cohere", "gpt-3", "gpt-4", "llm", "chatgpt", "gpt-cli", "anthropic", "gpt-client", "anthropic-claude"]
 classifiers = [
     "Development Status :: 4 - Beta",
     "Environment :: Console",
     "Intended Audience :: Developers",
     "Intended Audience :: End Users/Desktop",
     "Intended Audience :: Science/Research",
     "License :: OSI Approved :: MIT License",
     "Topic :: Scientific/Engineering :: Artificial Intelligence",
 ]
 dependencies = [
     "anthropic==0.25.9",
     "attrs==23.2.0",
     "black==24.4.2",
+    "cohere==5.5.3",
+    "google-generativeai==0.5.4",
     "mistralai==0.1.8",
-    "google-generativeai==0.1.0",
     "openai==1.30.1",
     "prompt-toolkit==3.0.43",
     "pytest==7.3.1",
     "PyYAML==6.0.1",
     "rich==13.7.1",
     "typing_extensions==4.11.0",
 ]
```

### Comparing `gpt_command_line-0.1.7/tests/test_assistant.py` & `gpt_command_line-0.2.0/tests/test_assistant.py`

 * *Files identical despite different names*

### Comparing `gpt_command_line-0.1.7/tests/test_session.py` & `gpt_command_line-0.2.0/tests/test_session.py`

 * *Files identical despite different names*

### Comparing `gpt_command_line-0.1.7/tests/test_term_utils.py` & `gpt_command_line-0.2.0/tests/test_term_utils.py`

 * *Files identical despite different names*

