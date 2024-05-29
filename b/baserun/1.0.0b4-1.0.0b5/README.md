# Comparing `tmp/baserun-1.0.0b4.tar.gz` & `tmp/baserun-1.0.0b5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "baserun-1.0.0b4.tar", last modified: Tue May 28 20:50:46 2024, max compression
+gzip compressed data, was "baserun-1.0.0b5.tar", last modified: Wed May 29 19:15:35 2024, max compression
```

## Comparing `baserun-1.0.0b4.tar` & `baserun-1.0.0b5.tar`

### file list

```diff
@@ -1,28 +1,32 @@
-drwxr-xr-x   0 epeterson   (501) staff       (20)        0 2024-05-28 20:50:46.632039 baserun-1.0.0b4/
--rw-r--r--   0 epeterson   (501) staff       (20)     1073 2023-08-04 18:23:26.000000 baserun-1.0.0b4/LICENSE
--rw-r--r--   0 epeterson   (501) staff       (20)     6223 2024-05-28 20:50:46.631748 baserun-1.0.0b4/PKG-INFO
--rw-r--r--   0 epeterson   (501) staff       (20)     4569 2024-03-20 17:26:14.000000 baserun-1.0.0b4/README.md
-drwxr-xr-x   0 epeterson   (501) staff       (20)        0 2024-05-28 20:50:46.606783 baserun-1.0.0b4/baserun/
--rw-r--r--   0 epeterson   (501) staff       (20)     1381 2024-05-28 20:37:48.000000 baserun-1.0.0b4/baserun/__init__.py
--rw-r--r--   0 epeterson   (501) staff       (20)     8668 2024-05-28 20:48:32.000000 baserun-1.0.0b4/baserun/api.py
--rw-r--r--   0 epeterson   (501) staff       (20)     6754 2024-05-28 20:37:48.000000 baserun-1.0.0b4/baserun/mixins.py
-drwxr-xr-x   0 epeterson   (501) staff       (20)        0 2024-05-28 20:50:46.626951 baserun-1.0.0b4/baserun/models/
--rw-r--r--   0 epeterson   (501) staff       (20)        0 2024-05-28 20:37:48.000000 baserun-1.0.0b4/baserun/models/__init__.py
--rw-r--r--   0 epeterson   (501) staff       (20)     3292 2024-05-28 20:37:48.000000 baserun-1.0.0b4/baserun/models/evals.py
--rw-r--r--   0 epeterson   (501) staff       (20)     2390 2024-05-28 20:37:48.000000 baserun-1.0.0b4/baserun/models/tags.py
--rw-r--r--   0 epeterson   (501) staff       (20)        0 2024-05-22 21:30:51.000000 baserun-1.0.0b4/baserun/py.typed
--rw-r--r--   0 epeterson   (501) staff       (20)     2086 2024-05-28 20:37:48.000000 baserun-1.0.0b4/baserun/utils.py
-drwxr-xr-x   0 epeterson   (501) staff       (20)        0 2024-05-28 20:50:46.628678 baserun-1.0.0b4/baserun/wrappers/
--rw-r--r--   0 epeterson   (501) staff       (20)        0 2024-05-28 20:37:48.000000 baserun-1.0.0b4/baserun/wrappers/__init__.py
--rw-r--r--   0 epeterson   (501) staff       (20)    16173 2024-05-28 20:37:48.000000 baserun-1.0.0b4/baserun/wrappers/openai.py
-drwxr-xr-x   0 epeterson   (501) staff       (20)        0 2024-05-28 20:50:46.630652 baserun-1.0.0b4/baserun.egg-info/
--rw-r--r--   0 epeterson   (501) staff       (20)     6223 2024-05-28 20:50:46.000000 baserun-1.0.0b4/baserun.egg-info/PKG-INFO
--rw-r--r--   0 epeterson   (501) staff       (20)      474 2024-05-28 20:50:46.000000 baserun-1.0.0b4/baserun.egg-info/SOURCES.txt
--rw-r--r--   0 epeterson   (501) staff       (20)        1 2024-05-28 20:50:46.000000 baserun-1.0.0b4/baserun.egg-info/dependency_links.txt
--rw-r--r--   0 epeterson   (501) staff       (20)       44 2024-05-28 20:50:46.000000 baserun-1.0.0b4/baserun.egg-info/entry_points.txt
--rw-r--r--   0 epeterson   (501) staff       (20)       21 2024-05-28 20:50:46.000000 baserun-1.0.0b4/baserun.egg-info/requires.txt
--rw-r--r--   0 epeterson   (501) staff       (20)        8 2024-05-28 20:50:46.000000 baserun-1.0.0b4/baserun.egg-info/top_level.txt
--rw-r--r--   0 epeterson   (501) staff       (20)     1091 2024-05-28 20:50:26.000000 baserun-1.0.0b4/pyproject.toml
--rw-r--r--   0 epeterson   (501) staff       (20)       81 2024-05-28 20:50:46.632986 baserun-1.0.0b4/setup.cfg
-drwxr-xr-x   0 epeterson   (501) staff       (20)        0 2024-05-28 20:50:46.629567 baserun-1.0.0b4/tests/
--rw-r--r--   0 epeterson   (501) staff       (20)    13539 2024-05-28 20:39:02.000000 baserun-1.0.0b4/tests/testing_functions.py
+drwxr-xr-x   0 epeterson   (501) staff       (20)        0 2024-05-29 19:15:35.315815 baserun-1.0.0b5/
+-rw-r--r--   0 epeterson   (501) staff       (20)     1073 2023-08-04 18:23:26.000000 baserun-1.0.0b5/LICENSE
+-rw-r--r--   0 epeterson   (501) staff       (20)     6559 2024-05-29 19:15:35.315623 baserun-1.0.0b5/PKG-INFO
+-rw-r--r--   0 epeterson   (501) staff       (20)     4905 2024-05-29 18:31:57.000000 baserun-1.0.0b5/README.md
+drwxr-xr-x   0 epeterson   (501) staff       (20)        0 2024-05-29 19:15:35.286478 baserun-1.0.0b5/baserun/
+-rw-r--r--   0 epeterson   (501) staff       (20)     1381 2024-05-29 18:43:55.000000 baserun-1.0.0b5/baserun/__init__.py
+-rw-r--r--   0 epeterson   (501) staff       (20)     8668 2024-05-29 18:31:57.000000 baserun-1.0.0b5/baserun/api.py
+drwxr-xr-x   0 epeterson   (501) staff       (20)        0 2024-05-29 19:15:35.308880 baserun-1.0.0b5/baserun/integrations/
+-rw-r--r--   0 epeterson   (501) staff       (20)      305 2024-05-29 18:45:54.000000 baserun-1.0.0b5/baserun/integrations/integration.py
+-rw-r--r--   0 epeterson   (501) staff       (20)     2045 2024-05-29 19:01:42.000000 baserun-1.0.0b5/baserun/integrations/llamaindex.py
+-rw-r--r--   0 epeterson   (501) staff       (20)     7049 2024-05-29 18:46:24.000000 baserun-1.0.0b5/baserun/mixins.py
+drwxr-xr-x   0 epeterson   (501) staff       (20)        0 2024-05-29 19:15:35.310958 baserun-1.0.0b5/baserun/models/
+-rw-r--r--   0 epeterson   (501) staff       (20)        0 2024-05-29 18:31:57.000000 baserun-1.0.0b5/baserun/models/__init__.py
+-rw-r--r--   0 epeterson   (501) staff       (20)     3292 2024-05-29 18:31:57.000000 baserun-1.0.0b5/baserun/models/evals.py
+-rw-r--r--   0 epeterson   (501) staff       (20)     2390 2024-05-29 18:31:57.000000 baserun-1.0.0b5/baserun/models/tags.py
+-rw-r--r--   0 epeterson   (501) staff       (20)        0 2024-05-29 18:31:57.000000 baserun-1.0.0b5/baserun/py.typed
+-rw-r--r--   0 epeterson   (501) staff       (20)      481 2024-05-29 19:03:25.000000 baserun-1.0.0b5/baserun/pytest_plugin.py
+-rw-r--r--   0 epeterson   (501) staff       (20)     2086 2024-05-29 18:31:57.000000 baserun-1.0.0b5/baserun/utils.py
+drwxr-xr-x   0 epeterson   (501) staff       (20)        0 2024-05-29 19:15:35.311919 baserun-1.0.0b5/baserun/wrappers/
+-rw-r--r--   0 epeterson   (501) staff       (20)        0 2024-05-29 18:31:57.000000 baserun-1.0.0b5/baserun/wrappers/__init__.py
+-rw-r--r--   0 epeterson   (501) staff       (20)    16493 2024-05-29 18:46:48.000000 baserun-1.0.0b5/baserun/wrappers/openai.py
+drwxr-xr-x   0 epeterson   (501) staff       (20)        0 2024-05-29 19:15:35.314449 baserun-1.0.0b5/baserun.egg-info/
+-rw-r--r--   0 epeterson   (501) staff       (20)     6559 2024-05-29 19:15:35.000000 baserun-1.0.0b5/baserun.egg-info/PKG-INFO
+-rw-r--r--   0 epeterson   (501) staff       (20)      570 2024-05-29 19:15:35.000000 baserun-1.0.0b5/baserun.egg-info/SOURCES.txt
+-rw-r--r--   0 epeterson   (501) staff       (20)        1 2024-05-29 19:15:35.000000 baserun-1.0.0b5/baserun.egg-info/dependency_links.txt
+-rw-r--r--   0 epeterson   (501) staff       (20)       44 2024-05-29 19:15:35.000000 baserun-1.0.0b5/baserun.egg-info/entry_points.txt
+-rw-r--r--   0 epeterson   (501) staff       (20)       21 2024-05-29 19:15:35.000000 baserun-1.0.0b5/baserun.egg-info/requires.txt
+-rw-r--r--   0 epeterson   (501) staff       (20)        8 2024-05-29 19:15:35.000000 baserun-1.0.0b5/baserun.egg-info/top_level.txt
+-rw-r--r--   0 epeterson   (501) staff       (20)     1091 2024-05-29 19:15:25.000000 baserun-1.0.0b5/pyproject.toml
+-rw-r--r--   0 epeterson   (501) staff       (20)       81 2024-05-29 19:15:35.316764 baserun-1.0.0b5/setup.cfg
+drwxr-xr-x   0 epeterson   (501) staff       (20)        0 2024-05-29 19:15:35.313201 baserun-1.0.0b5/tests/
+-rw-r--r--   0 epeterson   (501) staff       (20)    13539 2024-05-29 18:31:57.000000 baserun-1.0.0b5/tests/testing_functions.py
```

### Comparing `baserun-1.0.0b4/LICENSE` & `baserun-1.0.0b5/LICENSE`

 * *Files identical despite different names*

### Comparing `baserun-1.0.0b4/PKG-INFO` & `baserun-1.0.0b5/PKG-INFO`

 * *Files 18% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: baserun
-Version: 1.0.0b4
+Version: 1.0.0b5
 Summary: tools for testing, debugging, and evaluating llm features.
 Author-email: Erik Peterson <erik@baserun.ai>
 License: MIT License
         
         Copyright (c) 2023 Mochi Labs, Inc.
         
         Permission is hereby granted, free of charge, to any person obtaining a copy
@@ -46,132 +46,148 @@
 
 ## 1. Install Baserun
 
 ```bash
 pip install baserun
 ```
 
-## 2. Set up Baserun in your application
-
-###  Set the Baserun API key
+## 2. Set the Baserun API key
 Create an account at [https://baserun.ai](https://baserun.ai). Then generate an API key for your project in the [settings](https://baserun.ai/settings) tab. Set it as an environment variable:
 
 ```bash
 export BASERUN_API_KEY="your_api_key_here"
 ```
 
-Or set `baserun.api_key` to its value:
-
-```python
-baserun.api_key = "br-..."
-```
-
-###  Initialize Baserun
-
-At some point during your application's startup you need to call `baserun.init()`. This sets up the observability system and enables Baserun. If `init` is not called, Baserun will be disabled.
+## Usage
 
-## 3. Set up your traces
+In order to have Baserun trace your LLM Requests, all you need to do is import `OpenAI` from `baserun` instead of `openai`. Creating an OpenAI client object automatically starts the trace, and all future LLM requests made with this client object will be captured.
 
-A trace comprises a series of events executed within an your application. Tracing enables Baserun to display an LLM chain’s entire lifecycle, whether synchronous or asynchronous.
+<CodeGroup>
 
-To start tracing add the `@baserun.trace` decorator to the function you want to observe (e.g. a request/response handler or your `main` function).
+```python python
+from baserun import OpenAI
 
-Here is a simple example. In this case, Baserun is initialized at application startup and the `answer_question` function is traced. The LLM call within that function will now be traced.
 
-```python
-import sys
-from openai import OpenAI
-import baserun
-
-
-@baserun.trace
-def answer_question(question: str) -> str:
+def example():
     client = OpenAI()
-    response = client.chat.completions.create(
-        model="gpt-3.5-turbo",
-        messages=[{"role": "user", "content": question}],
+    completion = client.chat.completions.create(
+        name="Paris Activities",
+        model="gpt-4o",
+        temperature=0.7,
+        messages=[
+            {
+                "role": "user",
+                "content": "What are three activities to do in Paris?"
+            }
+        ],
     )
-    return response.choices[0].message.content
 
 
 if __name__ == "__main__":
-    baserun.init()
-    print(answer_question(sys.argv[-1]))
+    print(example())
 ```
 
-## 4. (Optional) Set up User Sessions
+### Alternate init method
 
-If your application involves interaction with a user and you wish to associate logs and traces with a particular user, you can use User Sessions. You can do this using `with_sessions`:
+If, for some reason, you don't wish to use Baserun's OpenAI client, you can simply wrap your normal OpenAI client using `init`.
 
-```python
-from openai import OpenAI
-import baserun
+```python python
+from baserun import init
 
-@baserun.trace
-def use_sessions(prompt="What is the capitol of the US?") -> str:
-    client = OpenAI()
-    with baserun.with_session(user_identifier="example@test.com"):
-        completion = client.chat.completions.create(
-            model="gpt-3.5-turbo",
-            messages=[{"role": "user", "content": prompt}],
-        )
-        content = completion.choices[0].message.content
-        return content
+client = init(OpenAI())
 ```
 
+</CodeGroup>
 
-## 5. (Optional) Set up your test suite
+## Configuring the trace
 
-Use our [pytest](https://docs.pytest.org) plugin and start immediately testing with Baserun. By default all OpenAI and Anthropic requests will be automatically logged.
+When you start a trace by initializing an OpenAI object, there are several _optional_ parameters you can set for that trace:
 
-```python
-# test_module.py
+- `name`: A customized name for the trace
+- `result`: Some end result or output for the trace
+- `user`: A username or user ID to associate with this trace.
+- `session`: A session ID to associate with this trace.
+- `trace_id`: A previously-generated or custom UUID (e.g. to continue a previous trace)
 
-import openai
+```python
+from baserun import OpenAI
 
-def test_paris_trip():
-    response = openai.ChatCompletion.create(
-        model="gpt-3.5-turbo",
+def example():
+    client = OpenAI(result="What are three activities to do in Paris?")
+    client.name = "Example"
+    client.user = "user123"
+    client.session = "session123"
+
+    completion = client.chat.completions.create(
+        name="Paris Activities",
+        model="gpt-4o",
         temperature=0.7,
         messages=[
             {
                 "role": "user",
                 "content": "What are three activities to do in Paris?"
             }
         ],
     )
-
-    assert "Eiffel Tower" in response['choices'][0]['message']['content']
+    client.result = "Done"
 ```
 
-To run the test and log to baserun:
+## Evals
 
-```bash
-pytest --baserun test_module.py
-...
-========================Baserun========================
-Test results available at: https://baserun.ai/runs/<id>
-=======================================================
+You can perform evals directly on a completion object. The `includes` eval is used here as an example, and checks if a string is included in the completion's output. The argument passed to `eval()` is a name or label used for your reference.
+
+```python
+from baserun import OpenAI
+
+def example():
+    client = OpenAI()
+    completion = client.chat.completions.create(
+        model="gpt-4o",
+        temperature=0.7,
+        messages=[
+            {
+                "role": "user",
+                "content": "What are three activities to do in Paris?"
+            }
+        ],
+    )
+    client.eval("include_eiffel_tower").includes("Eiffel Tower")
 ```
 
-## 6. (Optional) Set up checks
+## Tags
+
+You can add tags either to the traced OpenAI object or to the completion. There are several different types of tags:
+
+- `log`: Any arbitrary logs you want to attach to a trace or completion
+- `feedback`: Any score-based feedback given from users (e.g. thumbs up/down, star rating)
+- `variable`: Any variables used, e.g. while rendering a template
+- `annotate`: Any arbitrary attributes you want to attach to a trace or completion
 
-Baserun supports checks (also more broadly known as "evaluations"). These are assertions that the LLM response you received matches whatever criteria you require. To use a check, you can use `baserun.check` like so:
+Each tag type has functions on traced OpenAI objects and completions. Each tag function can accept a `metadata` parameter which is an arbitrary dictionary with any values you might want to capture.
 
 ```python
-from openai import OpenAI
-import baserun
+from baserun import OpenAI
 
-client = OpenAI()
-completion = client.chat.completions.create(
-    model="gpt-3.5-turbo",
-    messages=[{"role": "user", "content": "What is the capital of the United States?"}],
-)
-content = completion.choices[0].message.content
-baserun.check(name="capital_answer", result="Washington" in content)
+def example():
+    client = OpenAI()
+    client.log("Gathering user input")
+    city = input()
+    completion = client.chat.completions.create(
+        model="gpt-4o",
+        temperature=0.7,
+        messages=[
+            {
+                "role": "user",
+                "content": f"What are three activities to do in {city}?"
+            }
+        ],
+    )
+    completion.variable("city", city)
+    user_score = input()
+    client.feedback("User Score", score=user_score, metadata={"My key": "My value"})
 ```
 
 ## Further Documentation
 For a deeper dive on all capabilities and more advanced usage, please refer to our [Documentation](https://docs.baserun.ai).
 
 ## License
```

#### encoding

```diff
@@ -1 +1 @@
-utf-8
+us-ascii
```

### Comparing `baserun-1.0.0b4/README.md` & `baserun-1.0.0b5/README.md`

 * *Files 22% similar despite different names*

```diff
@@ -12,132 +12,148 @@
 
 ## 1. Install Baserun
 
 ```bash
 pip install baserun
 ```
 
-## 2. Set up Baserun in your application
-
-###  Set the Baserun API key
+## 2. Set the Baserun API key
 Create an account at [https://baserun.ai](https://baserun.ai). Then generate an API key for your project in the [settings](https://baserun.ai/settings) tab. Set it as an environment variable:
 
 ```bash
 export BASERUN_API_KEY="your_api_key_here"
 ```
 
-Or set `baserun.api_key` to its value:
-
-```python
-baserun.api_key = "br-..."
-```
-
-###  Initialize Baserun
-
-At some point during your application's startup you need to call `baserun.init()`. This sets up the observability system and enables Baserun. If `init` is not called, Baserun will be disabled.
+## Usage
 
-## 3. Set up your traces
+In order to have Baserun trace your LLM Requests, all you need to do is import `OpenAI` from `baserun` instead of `openai`. Creating an OpenAI client object automatically starts the trace, and all future LLM requests made with this client object will be captured.
 
-A trace comprises a series of events executed within an your application. Tracing enables Baserun to display an LLM chain’s entire lifecycle, whether synchronous or asynchronous.
+<CodeGroup>
 
-To start tracing add the `@baserun.trace` decorator to the function you want to observe (e.g. a request/response handler or your `main` function).
+```python python
+from baserun import OpenAI
 
-Here is a simple example. In this case, Baserun is initialized at application startup and the `answer_question` function is traced. The LLM call within that function will now be traced.
 
-```python
-import sys
-from openai import OpenAI
-import baserun
-
-
-@baserun.trace
-def answer_question(question: str) -> str:
+def example():
     client = OpenAI()
-    response = client.chat.completions.create(
-        model="gpt-3.5-turbo",
-        messages=[{"role": "user", "content": question}],
+    completion = client.chat.completions.create(
+        name="Paris Activities",
+        model="gpt-4o",
+        temperature=0.7,
+        messages=[
+            {
+                "role": "user",
+                "content": "What are three activities to do in Paris?"
+            }
+        ],
     )
-    return response.choices[0].message.content
 
 
 if __name__ == "__main__":
-    baserun.init()
-    print(answer_question(sys.argv[-1]))
+    print(example())
 ```
 
-## 4. (Optional) Set up User Sessions
+### Alternate init method
 
-If your application involves interaction with a user and you wish to associate logs and traces with a particular user, you can use User Sessions. You can do this using `with_sessions`:
+If, for some reason, you don't wish to use Baserun's OpenAI client, you can simply wrap your normal OpenAI client using `init`.
 
-```python
-from openai import OpenAI
-import baserun
+```python python
+from baserun import init
 
-@baserun.trace
-def use_sessions(prompt="What is the capitol of the US?") -> str:
-    client = OpenAI()
-    with baserun.with_session(user_identifier="example@test.com"):
-        completion = client.chat.completions.create(
-            model="gpt-3.5-turbo",
-            messages=[{"role": "user", "content": prompt}],
-        )
-        content = completion.choices[0].message.content
-        return content
+client = init(OpenAI())
 ```
 
+</CodeGroup>
 
-## 5. (Optional) Set up your test suite
+## Configuring the trace
 
-Use our [pytest](https://docs.pytest.org) plugin and start immediately testing with Baserun. By default all OpenAI and Anthropic requests will be automatically logged.
+When you start a trace by initializing an OpenAI object, there are several _optional_ parameters you can set for that trace:
 
-```python
-# test_module.py
+- `name`: A customized name for the trace
+- `result`: Some end result or output for the trace
+- `user`: A username or user ID to associate with this trace.
+- `session`: A session ID to associate with this trace.
+- `trace_id`: A previously-generated or custom UUID (e.g. to continue a previous trace)
 
-import openai
+```python
+from baserun import OpenAI
 
-def test_paris_trip():
-    response = openai.ChatCompletion.create(
-        model="gpt-3.5-turbo",
+def example():
+    client = OpenAI(result="What are three activities to do in Paris?")
+    client.name = "Example"
+    client.user = "user123"
+    client.session = "session123"
+
+    completion = client.chat.completions.create(
+        name="Paris Activities",
+        model="gpt-4o",
         temperature=0.7,
         messages=[
             {
                 "role": "user",
                 "content": "What are three activities to do in Paris?"
             }
         ],
     )
-
-    assert "Eiffel Tower" in response['choices'][0]['message']['content']
+    client.result = "Done"
 ```
 
-To run the test and log to baserun:
+## Evals
 
-```bash
-pytest --baserun test_module.py
-...
-========================Baserun========================
-Test results available at: https://baserun.ai/runs/<id>
-=======================================================
+You can perform evals directly on a completion object. The `includes` eval is used here as an example, and checks if a string is included in the completion's output. The argument passed to `eval()` is a name or label used for your reference.
+
+```python
+from baserun import OpenAI
+
+def example():
+    client = OpenAI()
+    completion = client.chat.completions.create(
+        model="gpt-4o",
+        temperature=0.7,
+        messages=[
+            {
+                "role": "user",
+                "content": "What are three activities to do in Paris?"
+            }
+        ],
+    )
+    client.eval("include_eiffel_tower").includes("Eiffel Tower")
 ```
 
-## 6. (Optional) Set up checks
+## Tags
+
+You can add tags either to the traced OpenAI object or to the completion. There are several different types of tags:
+
+- `log`: Any arbitrary logs you want to attach to a trace or completion
+- `feedback`: Any score-based feedback given from users (e.g. thumbs up/down, star rating)
+- `variable`: Any variables used, e.g. while rendering a template
+- `annotate`: Any arbitrary attributes you want to attach to a trace or completion
 
-Baserun supports checks (also more broadly known as "evaluations"). These are assertions that the LLM response you received matches whatever criteria you require. To use a check, you can use `baserun.check` like so:
+Each tag type has functions on traced OpenAI objects and completions. Each tag function can accept a `metadata` parameter which is an arbitrary dictionary with any values you might want to capture.
 
 ```python
-from openai import OpenAI
-import baserun
+from baserun import OpenAI
 
-client = OpenAI()
-completion = client.chat.completions.create(
-    model="gpt-3.5-turbo",
-    messages=[{"role": "user", "content": "What is the capital of the United States?"}],
-)
-content = completion.choices[0].message.content
-baserun.check(name="capital_answer", result="Washington" in content)
+def example():
+    client = OpenAI()
+    client.log("Gathering user input")
+    city = input()
+    completion = client.chat.completions.create(
+        model="gpt-4o",
+        temperature=0.7,
+        messages=[
+            {
+                "role": "user",
+                "content": f"What are three activities to do in {city}?"
+            }
+        ],
+    )
+    completion.variable("city", city)
+    user_score = input()
+    client.feedback("User Score", score=user_score, metadata={"My key": "My value"})
 ```
 
 ## Further Documentation
 For a deeper dive on all capabilities and more advanced usage, please refer to our [Documentation](https://docs.baserun.ai).
 
 ## License
```

#### encoding

```diff
@@ -1 +1 @@
-utf-8
+us-ascii
```

### Comparing `baserun-1.0.0b4/baserun/__init__.py` & `baserun-1.0.0b5/baserun/__init__.py`

 * *Files identical despite different names*

### Comparing `baserun-1.0.0b4/baserun/api.py` & `baserun-1.0.0b5/baserun/api.py`

 * *Files identical despite different names*

### Comparing `baserun-1.0.0b4/baserun/mixins.py` & `baserun-1.0.0b5/baserun/mixins.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,13 +1,14 @@
 import json
 from abc import ABC
-from typing import Any, Dict, List, Optional, overload
+from typing import Any, Dict, List, Optional, Type, overload
 
 from openai.types.chat import ChatCompletionMessageToolCall
 
+from baserun.integrations.integration import Integration
 from baserun.models.evals import CompletionEval, TraceEval
 from baserun.models.tags import Log, Tag, Transform, Variable
 
 
 class CompletionMixin(ABC):
     tags: List[Tag]
     evals: List[CompletionEval]
@@ -106,14 +107,15 @@
 
 
 class ClientMixin(ABC):
     tags: List[Tag]
     evals: List["TraceEval"]
     trace_id: str
     result: Optional[str]
+    integrations: List[Integration]
 
     def annotate(self, key: str, value: str, metadata: Optional[Dict[str, Any]] = None):
         self.tags.append(
             Tag(
                 target_type="trace",
                 target_id=self.trace_id,
                 tag_type="annotation",
@@ -172,14 +174,19 @@
                 key=name or "log",
                 value=message,
                 metadata=metadata or {},
             )
         )
         self.submit_to_baserun()
 
+    def integrate(self, integration_class: Type[Integration]):
+        integration = integration_class(client=self)
+        integration.instrument()
+        self.integrations.append(integration)
+
     def transform(self, *args, **kwargs):
         transform_input = kwargs.pop("input", None)
         transform_output = kwargs.pop("output", None)
         self.tags.append(
             Transform(
                 key=args[0],
                 target_type="trace",
```

### Comparing `baserun-1.0.0b4/baserun/models/evals.py` & `baserun-1.0.0b5/baserun/models/evals.py`

 * *Files identical despite different names*

### Comparing `baserun-1.0.0b4/baserun/models/tags.py` & `baserun-1.0.0b5/baserun/models/tags.py`

 * *Files identical despite different names*

### Comparing `baserun-1.0.0b4/baserun/utils.py` & `baserun-1.0.0b5/baserun/utils.py`

 * *Files identical despite different names*

### Comparing `baserun-1.0.0b4/baserun/wrappers/openai.py` & `baserun-1.0.0b5/baserun/wrappers/openai.py`

 * *Files 2% similar despite different names*

```diff
@@ -13,14 +13,15 @@
 from openai._types import ResponseT
 from openai.resources.chat import AsyncChat, AsyncCompletions, Chat, Completions
 from openai.types.chat import ChatCompletion, ChatCompletionChunk, ChatCompletionMessageParam
 from openai.types.chat.chat_completion_chunk import Choice
 from pydantic import BaseModel, ConfigDict, Field
 
 from baserun.api import ApiClient
+from baserun.integrations.integration import Integration
 from baserun.mixins import ClientMixin, CompletionMixin
 from baserun.models.evals import CompletionEval, TraceEval
 from baserun.models.tags import Tag
 from baserun.utils import copy_type_hints
 
 logger = logging.getLogger(__name__)
 
@@ -278,14 +279,15 @@
     def completions(self) -> WrappedAsyncCompletions:
         return WrappedAsyncCompletions(self._client)
 
 
 class WrappedOpenAIBaseClient(ClientMixin):
     model_config = ConfigDict(arbitrary_types_allowed=True)
     chat: WrappedChat | WrappedAsyncChat
+    integrations: List[Integration]
 
     def __init__(
         self,
         client: Union[BaseOpenAI, BaseAsyncOpenAI],
         *args,
         name: Optional[str] = None,
         user: Optional[str] = None,
@@ -305,14 +307,22 @@
         self.user = user
         self.session = session
         self.start_timestamp = datetime.now(timezone.utc)
         self.end_timestamp: Union[datetime, None] = None
         self.api_client = api_client or ApiClient(self, api_key=api_key)
         self.metadata = metadata or {}
         self.request_ids: Dict[str, str] = {}
+        self.integrations = []
+
+        try:
+            from baserun.integrations.llamaindex import LLamaIndexInstrumentation
+
+            self.integrate(LLamaIndexInstrumentation)
+        except ImportError:
+            pass
 
     @property
     def result(self):
         return self._result
 
     @result.setter
     def result(self, value):
```

### Comparing `baserun-1.0.0b4/baserun.egg-info/PKG-INFO` & `baserun-1.0.0b5/baserun.egg-info/PKG-INFO`

 * *Files 18% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: baserun
-Version: 1.0.0b4
+Version: 1.0.0b5
 Summary: tools for testing, debugging, and evaluating llm features.
 Author-email: Erik Peterson <erik@baserun.ai>
 License: MIT License
         
         Copyright (c) 2023 Mochi Labs, Inc.
         
         Permission is hereby granted, free of charge, to any person obtaining a copy
@@ -46,132 +46,148 @@
 
 ## 1. Install Baserun
 
 ```bash
 pip install baserun
 ```
 
-## 2. Set up Baserun in your application
-
-###  Set the Baserun API key
+## 2. Set the Baserun API key
 Create an account at [https://baserun.ai](https://baserun.ai). Then generate an API key for your project in the [settings](https://baserun.ai/settings) tab. Set it as an environment variable:
 
 ```bash
 export BASERUN_API_KEY="your_api_key_here"
 ```
 
-Or set `baserun.api_key` to its value:
-
-```python
-baserun.api_key = "br-..."
-```
-
-###  Initialize Baserun
-
-At some point during your application's startup you need to call `baserun.init()`. This sets up the observability system and enables Baserun. If `init` is not called, Baserun will be disabled.
+## Usage
 
-## 3. Set up your traces
+In order to have Baserun trace your LLM Requests, all you need to do is import `OpenAI` from `baserun` instead of `openai`. Creating an OpenAI client object automatically starts the trace, and all future LLM requests made with this client object will be captured.
 
-A trace comprises a series of events executed within an your application. Tracing enables Baserun to display an LLM chain’s entire lifecycle, whether synchronous or asynchronous.
+<CodeGroup>
 
-To start tracing add the `@baserun.trace` decorator to the function you want to observe (e.g. a request/response handler or your `main` function).
+```python python
+from baserun import OpenAI
 
-Here is a simple example. In this case, Baserun is initialized at application startup and the `answer_question` function is traced. The LLM call within that function will now be traced.
 
-```python
-import sys
-from openai import OpenAI
-import baserun
-
-
-@baserun.trace
-def answer_question(question: str) -> str:
+def example():
     client = OpenAI()
-    response = client.chat.completions.create(
-        model="gpt-3.5-turbo",
-        messages=[{"role": "user", "content": question}],
+    completion = client.chat.completions.create(
+        name="Paris Activities",
+        model="gpt-4o",
+        temperature=0.7,
+        messages=[
+            {
+                "role": "user",
+                "content": "What are three activities to do in Paris?"
+            }
+        ],
     )
-    return response.choices[0].message.content
 
 
 if __name__ == "__main__":
-    baserun.init()
-    print(answer_question(sys.argv[-1]))
+    print(example())
 ```
 
-## 4. (Optional) Set up User Sessions
+### Alternate init method
 
-If your application involves interaction with a user and you wish to associate logs and traces with a particular user, you can use User Sessions. You can do this using `with_sessions`:
+If, for some reason, you don't wish to use Baserun's OpenAI client, you can simply wrap your normal OpenAI client using `init`.
 
-```python
-from openai import OpenAI
-import baserun
+```python python
+from baserun import init
 
-@baserun.trace
-def use_sessions(prompt="What is the capitol of the US?") -> str:
-    client = OpenAI()
-    with baserun.with_session(user_identifier="example@test.com"):
-        completion = client.chat.completions.create(
-            model="gpt-3.5-turbo",
-            messages=[{"role": "user", "content": prompt}],
-        )
-        content = completion.choices[0].message.content
-        return content
+client = init(OpenAI())
 ```
 
+</CodeGroup>
 
-## 5. (Optional) Set up your test suite
+## Configuring the trace
 
-Use our [pytest](https://docs.pytest.org) plugin and start immediately testing with Baserun. By default all OpenAI and Anthropic requests will be automatically logged.
+When you start a trace by initializing an OpenAI object, there are several _optional_ parameters you can set for that trace:
 
-```python
-# test_module.py
+- `name`: A customized name for the trace
+- `result`: Some end result or output for the trace
+- `user`: A username or user ID to associate with this trace.
+- `session`: A session ID to associate with this trace.
+- `trace_id`: A previously-generated or custom UUID (e.g. to continue a previous trace)
 
-import openai
+```python
+from baserun import OpenAI
 
-def test_paris_trip():
-    response = openai.ChatCompletion.create(
-        model="gpt-3.5-turbo",
+def example():
+    client = OpenAI(result="What are three activities to do in Paris?")
+    client.name = "Example"
+    client.user = "user123"
+    client.session = "session123"
+
+    completion = client.chat.completions.create(
+        name="Paris Activities",
+        model="gpt-4o",
         temperature=0.7,
         messages=[
             {
                 "role": "user",
                 "content": "What are three activities to do in Paris?"
             }
         ],
     )
-
-    assert "Eiffel Tower" in response['choices'][0]['message']['content']
+    client.result = "Done"
 ```
 
-To run the test and log to baserun:
+## Evals
 
-```bash
-pytest --baserun test_module.py
-...
-========================Baserun========================
-Test results available at: https://baserun.ai/runs/<id>
-=======================================================
+You can perform evals directly on a completion object. The `includes` eval is used here as an example, and checks if a string is included in the completion's output. The argument passed to `eval()` is a name or label used for your reference.
+
+```python
+from baserun import OpenAI
+
+def example():
+    client = OpenAI()
+    completion = client.chat.completions.create(
+        model="gpt-4o",
+        temperature=0.7,
+        messages=[
+            {
+                "role": "user",
+                "content": "What are three activities to do in Paris?"
+            }
+        ],
+    )
+    client.eval("include_eiffel_tower").includes("Eiffel Tower")
 ```
 
-## 6. (Optional) Set up checks
+## Tags
+
+You can add tags either to the traced OpenAI object or to the completion. There are several different types of tags:
+
+- `log`: Any arbitrary logs you want to attach to a trace or completion
+- `feedback`: Any score-based feedback given from users (e.g. thumbs up/down, star rating)
+- `variable`: Any variables used, e.g. while rendering a template
+- `annotate`: Any arbitrary attributes you want to attach to a trace or completion
 
-Baserun supports checks (also more broadly known as "evaluations"). These are assertions that the LLM response you received matches whatever criteria you require. To use a check, you can use `baserun.check` like so:
+Each tag type has functions on traced OpenAI objects and completions. Each tag function can accept a `metadata` parameter which is an arbitrary dictionary with any values you might want to capture.
 
 ```python
-from openai import OpenAI
-import baserun
+from baserun import OpenAI
 
-client = OpenAI()
-completion = client.chat.completions.create(
-    model="gpt-3.5-turbo",
-    messages=[{"role": "user", "content": "What is the capital of the United States?"}],
-)
-content = completion.choices[0].message.content
-baserun.check(name="capital_answer", result="Washington" in content)
+def example():
+    client = OpenAI()
+    client.log("Gathering user input")
+    city = input()
+    completion = client.chat.completions.create(
+        model="gpt-4o",
+        temperature=0.7,
+        messages=[
+            {
+                "role": "user",
+                "content": f"What are three activities to do in {city}?"
+            }
+        ],
+    )
+    completion.variable("city", city)
+    user_score = input()
+    client.feedback("User Score", score=user_score, metadata={"My key": "My value"})
 ```
 
 ## Further Documentation
 For a deeper dive on all capabilities and more advanced usage, please refer to our [Documentation](https://docs.baserun.ai).
 
 ## License
```

#### encoding

```diff
@@ -1 +1 @@
-utf-8
+us-ascii
```

### Comparing `baserun-1.0.0b4/pyproject.toml` & `baserun-1.0.0b5/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["setuptools", "wheel"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "baserun"
-version = "1.0.0b4"
+version = "1.0.0b5"
 description = "tools for testing, debugging, and evaluating llm features."
 readme = "README.md"
 license = { file = "LICENSE" }
 authors = [
     { name = "Erik Peterson", email = "erik@baserun.ai" }
 ]
 requires-python = ">=3.8, <3.12"
```

### Comparing `baserun-1.0.0b4/tests/testing_functions.py` & `baserun-1.0.0b5/tests/testing_functions.py`

 * *Files identical despite different names*

