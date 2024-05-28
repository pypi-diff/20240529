# Comparing `tmp/agentops-0.1.9.tar.gz` & `tmp/agentops-0.2.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "agentops-0.1.9.tar", last modified: Tue May  7 07:07:25 2024, max compression
+gzip compressed data, was "agentops-0.2.0.tar", last modified: Tue May 28 22:04:10 2024, max compression
```

## Comparing `agentops-0.1.9.tar` & `agentops-0.2.0.tar`

### file list

```diff
@@ -1,36 +1,39 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 07:07:25.996352 agentops-0.1.9/
--rw-r--r--   0 runner    (1001) docker     (127)     1068 2024-05-07 07:07:19.000000 agentops-0.1.9/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)     8791 2024-05-07 07:07:25.996352 agentops-0.1.9/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     7860 2024-05-07 07:07:19.000000 agentops-0.1.9/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 07:07:25.992352 agentops-0.1.9/agentops/
--rwxr-xr-x   0 runner    (1001) docker     (127)     5027 2024-05-07 07:07:19.000000 agentops-0.1.9/agentops/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1269 2024-05-07 07:07:19.000000 agentops-0.1.9/agentops/agent.py
--rw-r--r--   0 runner    (1001) docker     (127)    15585 2024-05-07 07:07:19.000000 agentops-0.1.9/agentops/client.py
--rw-r--r--   0 runner    (1001) docker     (127)     4297 2024-05-07 07:07:19.000000 agentops-0.1.9/agentops/config.py
--rw-r--r--   0 runner    (1001) docker     (127)     1025 2024-05-07 07:07:19.000000 agentops-0.1.9/agentops/decorators.py
--rw-r--r--   0 runner    (1001) docker     (127)      694 2024-05-07 07:07:19.000000 agentops-0.1.9/agentops/enums.py
--rw-r--r--   0 runner    (1001) docker     (127)     5580 2024-05-07 07:07:19.000000 agentops-0.1.9/agentops/event.py
--rw-r--r--   0 runner    (1001) docker     (127)     4470 2024-05-07 07:07:19.000000 agentops-0.1.9/agentops/helpers.py
--rw-r--r--   0 runner    (1001) docker     (127)     2183 2024-05-07 07:07:19.000000 agentops-0.1.9/agentops/host_env.py
--rw-r--r--   0 runner    (1001) docker     (127)     3435 2024-05-07 07:07:19.000000 agentops-0.1.9/agentops/http_client.py
--rw-r--r--   0 runner    (1001) docker     (127)    22363 2024-05-07 07:07:19.000000 agentops-0.1.9/agentops/langchain_callback_handler.py
--rw-r--r--   0 runner    (1001) docker     (127)    15405 2024-05-07 07:07:19.000000 agentops-0.1.9/agentops/llm_tracker.py
--rw-r--r--   0 runner    (1001) docker     (127)      225 2024-05-07 07:07:19.000000 agentops-0.1.9/agentops/log_config.py
--rw-r--r--   0 runner    (1001) docker     (127)     2001 2024-05-07 07:07:19.000000 agentops-0.1.9/agentops/meta_client.py
--rw-r--r--   0 runner    (1001) docker     (127)     2427 2024-05-07 07:07:19.000000 agentops-0.1.9/agentops/session.py
--rw-r--r--   0 runner    (1001) docker     (127)     4136 2024-05-07 07:07:19.000000 agentops-0.1.9/agentops/worker.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 07:07:25.992352 agentops-0.1.9/agentops.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     8791 2024-05-07 07:07:25.000000 agentops-0.1.9/agentops.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      680 2024-05-07 07:07:25.000000 agentops-0.1.9/agentops.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-07 07:07:25.000000 agentops-0.1.9/agentops.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)      122 2024-05-07 07:07:25.000000 agentops-0.1.9/agentops.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)        9 2024-05-07 07:07:25.000000 agentops-0.1.9/agentops.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)      995 2024-05-07 07:07:19.000000 agentops-0.1.9/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-07 07:07:25.996352 agentops-0.1.9/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 07:07:25.992352 agentops-0.1.9/tests/
--rw-r--r--   0 runner    (1001) docker     (127)     1125 2024-05-07 07:07:19.000000 agentops-0.1.9/tests/test_canary.py
--rw-r--r--   0 runner    (1001) docker     (127)      743 2024-05-07 07:07:19.000000 agentops-0.1.9/tests/test_events.py
--rw-r--r--   0 runner    (1001) docker     (127)     2171 2024-05-07 07:07:19.000000 agentops-0.1.9/tests/test_patcher.py
--rw-r--r--   0 runner    (1001) docker     (127)     3267 2024-05-07 07:07:19.000000 agentops-0.1.9/tests/test_record_function.py
--rw-r--r--   0 runner    (1001) docker     (127)     4334 2024-05-07 07:07:19.000000 agentops-0.1.9/tests/test_session.py
--rw-r--r--   0 runner    (1001) docker     (127)      573 2024-05-07 07:07:19.000000 agentops-0.1.9/tests/test_teardown.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-28 22:04:10.133580 agentops-0.2.0/
+-rw-r--r--   0 runner    (1001) docker     (127)     1068 2024-05-28 22:04:05.000000 agentops-0.2.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)    11397 2024-05-28 22:04:10.133580 agentops-0.2.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)    10469 2024-05-28 22:04:05.000000 agentops-0.2.0/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-28 22:04:10.129580 agentops-0.2.0/agentops/
+-rwxr-xr-x   0 runner    (1001) docker     (127)     5198 2024-05-28 22:04:05.000000 agentops-0.2.0/agentops/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1400 2024-05-28 22:04:05.000000 agentops-0.2.0/agentops/agent.py
+-rw-r--r--   0 runner    (1001) docker     (127)    17928 2024-05-28 22:04:05.000000 agentops-0.2.0/agentops/client.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4301 2024-05-28 22:04:05.000000 agentops-0.2.0/agentops/config.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1065 2024-05-28 22:04:05.000000 agentops-0.2.0/agentops/decorators.py
+-rw-r--r--   0 runner    (1001) docker     (127)      694 2024-05-28 22:04:05.000000 agentops-0.2.0/agentops/enums.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5571 2024-05-28 22:04:05.000000 agentops-0.2.0/agentops/event.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4933 2024-05-28 22:04:05.000000 agentops-0.2.0/agentops/helpers.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3803 2024-05-28 22:04:05.000000 agentops-0.2.0/agentops/host_env.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3507 2024-05-28 22:04:05.000000 agentops-0.2.0/agentops/http_client.py
+-rw-r--r--   0 runner    (1001) docker     (127)    22658 2024-05-28 22:04:05.000000 agentops-0.2.0/agentops/langchain_callback_handler.py
+-rw-r--r--   0 runner    (1001) docker     (127)    25656 2024-05-28 22:04:05.000000 agentops-0.2.0/agentops/llm_tracker.py
+-rw-r--r--   0 runner    (1001) docker     (127)      827 2024-05-28 22:04:05.000000 agentops-0.2.0/agentops/log_config.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2181 2024-05-28 22:04:05.000000 agentops-0.2.0/agentops/meta_client.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-28 22:04:10.129580 agentops-0.2.0/agentops/partners/
+-rw-r--r--   0 runner    (1001) docker     (127)     3738 2024-05-28 22:04:05.000000 agentops-0.2.0/agentops/partners/autogen_logger.py
+-rw-r--r--   0 runner    (1001) docker     (127)    22710 2024-05-28 22:04:05.000000 agentops-0.2.0/agentops/partners/langchain_callback_handler.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2480 2024-05-28 22:04:05.000000 agentops-0.2.0/agentops/session.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4585 2024-05-28 22:04:05.000000 agentops-0.2.0/agentops/worker.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-28 22:04:10.129580 agentops-0.2.0/agentops.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)    11397 2024-05-28 22:04:10.000000 agentops-0.2.0/agentops.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      764 2024-05-28 22:04:10.000000 agentops-0.2.0/agentops.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-28 22:04:10.000000 agentops-0.2.0/agentops.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      119 2024-05-28 22:04:10.000000 agentops-0.2.0/agentops.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        9 2024-05-28 22:04:10.000000 agentops-0.2.0/agentops.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)     1031 2024-05-28 22:04:05.000000 agentops-0.2.0/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-28 22:04:10.133580 agentops-0.2.0/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-28 22:04:10.129580 agentops-0.2.0/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)     1308 2024-05-28 22:04:05.000000 agentops-0.2.0/tests/test_canary.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1230 2024-05-28 22:04:05.000000 agentops-0.2.0/tests/test_events.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2171 2024-05-28 22:04:05.000000 agentops-0.2.0/tests/test_patcher.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3484 2024-05-28 22:04:05.000000 agentops-0.2.0/tests/test_record_function.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4523 2024-05-28 22:04:05.000000 agentops-0.2.0/tests/test_session.py
+-rw-r--r--   0 runner    (1001) docker     (127)      748 2024-05-28 22:04:05.000000 agentops-0.2.0/tests/test_teardown.py
```

### Comparing `agentops-0.1.9/LICENSE` & `agentops-0.2.0/LICENSE`

 * *Files identical despite different names*

### Comparing `agentops-0.1.9/PKG-INFO` & `agentops-0.2.0/README.md`

 * *Files 16% similar despite different names*

```diff
@@ -1,32 +1,10 @@
-Metadata-Version: 2.1
-Name: agentops
-Version: 0.1.9
-Summary: Python SDK for developing AI agent evals and observability
-Author-email: Alex Reibman <areibman@gmail.com>, Shawn Qiu <siyangqiu@gmail.com>, Braelyn Boynton <bboynton97@gmail.com>, Howard Gil <howardbgil@gmail.com>
-Project-URL: Homepage, https://github.com/AgentOps-AI/agentops
-Project-URL: Issues, https://github.com/AgentOps-AI/agentops/issues
-Classifier: Programming Language :: Python :: 3
-Classifier: License :: OSI Approved :: MIT License
-Classifier: Operating System :: OS Independent
-Requires-Python: >=3.7
-Description-Content-Type: text/markdown
-License-File: LICENSE
-Requires-Dist: requests==2.31.0
-Requires-Dist: psutil==5.9.8
-Requires-Dist: packaging==23.2
-Provides-Extra: dev
-Requires-Dist: pytest==7.4.0; extra == "dev"
-Requires-Dist: requests_mock==1.11.0; extra == "dev"
-Provides-Extra: langchain
-Requires-Dist: langchain>=0.0.354; extra == "langchain"
-
 <div align="center">
   <a href="https://agentops.ai?ref=gh">
-    <img src="https://github.com/AgentOps-AI/agentops/blob/df22e9dffb7294fb977dc103a2ca3bcf8f04946f/logo.png" style="margin: 15px; max-width: 300px" width="50%" alt="Logo">
+    <img src="https://raw.githubusercontent.com/AgentOps-AI/agentops/35d5682866921a9e28d8ef66ae3c3b3d92d8fa6b/img/logo.png" style="margin: 15px; max-width: 300px" width="50%" alt="Logo">
   </a>
 </div>
 <p align="center">
   <em>AI agents suck. We’re fixing that.</em>
 </p>
 
 <p align="center">
@@ -43,45 +21,47 @@
 <a href="https://app.agentops.ai/?ref=gh">🖇️ AgentOps</a>
 <span>&nbsp;&nbsp;•&nbsp;&nbsp;</span>
 <a href="https://docs.agentops.ai/introduction">📙 Documentation</a>
 </p>
 
 # AgentOps 🖇️
 
-[![License: MIT](https://img.shields.io/badge/License-MIT-yellow.svg)](https://opensource.org/licenses/MIT) ![PyPI - Version](https://img.shields.io/pypi/v/agentops) <a href="https://pepy.tech/project/agentops">
-  <img src="https://static.pepy.tech/badge/agentops/month"> <a href="https://twitter.com/agentopsai">
-    <img src="https://img.shields.io/badge/follow-%40agentops-1DA1F2?logo=twitter&style=social" alt="AgentOps Twitter" /> 
-  </a>
-  <a href="https://discord.gg/mKW3ZhN9p2">
-    <img src="https://img.shields.io/badge/chat-on%20Discord-blueviolet" alt="Discord community channel" />
-  </a>
-  <a href="mailto:investor@agentops.ai"><img src="https://img.shields.io/website?color=%23f26522&down_message=Y%20Combinator&label=Not%20Backed%20By&logo=ycombinator&style=flat-square&up_message=Y%20Combinator&url=https%3A%2F%2Fwww.ycombinator.com"/>
-  <a href="https://github.com/agentops-ai/agentops/issues">
-    <img src="https://img.shields.io/github/commit-activity/m/agentops-ai/agentops" alt="git commit activity" />
-  </a>
-
+[![License: MIT](https://img.shields.io/badge/License-MIT-yellow.svg)](https://opensource.org/licenses/MIT)
+![PyPI - Version](https://img.shields.io/pypi/v/agentops)
+<a href="https://pepy.tech/project/agentops">
+  <img src="https://static.pepy.tech/badge/agentops/month">
+</a>
+<a href="https://twitter.com/agentopsai">
+  <img src="https://img.shields.io/badge/follow-%40agentops-1DA1F2?logo=twitter&style=social" alt="AgentOps Twitter"/>
+</a>
+<a href="https://discord.gg/mKW3ZhN9p2">
+  <img src="https://img.shields.io/badge/chat-on%20Discord-blueviolet" alt="Discord community channel"/>
+</a>
+<a href="https://github.com/agentops-ai/agentops/issues">
+  <img src="https://img.shields.io/github/commit-activity/m/agentops-ai/agentops" alt="git commit activity"/>
+</a>
 
 AgentOps helps developers build, evaluate, and monitor AI agents. Tools to build agents from prototype to production.
 
-
-|||
-|------------------------------------------|----------------------------------------------------|
-| 📊 **Replay Analytics and Debugging** | Step-by-step agent execution graphs |
-| 💸 **LLM Cost Management**   | Track spend with LLM foundation model providers |
-| 🧪 **Agent Benchmarking** | Test your agents against 1,000+ evals |
-| 🔐 **Compliance and Security**            | Detect common prompt injection and data exfiltration exploits |
-| 🤝 **Framework Integrations**            | Easily plugs in with frameworks like CrewAI and LangChain |
+|                                       |                                                               |
+| ------------------------------------- | ------------------------------------------------------------- |
+| 📊 **Replay Analytics and Debugging** | Step-by-step agent execution graphs                           |
+| 💸 **LLM Cost Management**            | Track spend with LLM foundation model providers               |
+| 🧪 **Agent Benchmarking**             | Test your agents against 1,000+ evals                         |
+| 🔐 **Compliance and Security**        | Detect common prompt injection and data exfiltration exploits |
+| 🤝 **Framework Integrations**         | Easily plugs in with frameworks like CrewAI and LangChain     |
 
 ## Quick Start ⌨️
 
-```python
+```bash
 pip install agentops
 ```
 
 ### Session replays in 3 lines of code
+
 Initialize the AgentOps client and automatically get analytics on every LLM call.
 
 ```python
 import agentops
 
 # Beginning of program's code (i.e. main.py, __init__.py)
 agentops.init(<INSERT YOUR API KEY HERE>)
@@ -95,15 +75,14 @@
 # End of program
 agentops.end_session('Success')
 # Woohoo You're done 🎉
 ```
 
 All your sessions are available on the [AgentOps dashboard](https://app.agentops.ai?ref=gh). Refer to our [API documentation](http://docs.agentops.ai) for detailed instructions.
 
-
 <details open>
   <summary>Agent Dashboard</summary>
   <a href="https://app.agentops.ai?ref=gh">
    <img src="https://github.com/AgentOps-AI/agentops/assets/14807319/158e082a-9a7d-49b7-9b41-51a49a1f7d3d" style="width: 90%;" alt="Agent Dashboard"/>
   </a>
 </details>
 
@@ -123,22 +102,30 @@
 
 ## Integrations 🦾
 
 ### CrewAI 🛶
 
 Build Crew agents with observability with only 2 lines of code. Simply set an `AGENTOPS_API_KEY` in your environment, and your crews will get automatic monitoring on the AgentOps dashboard.
 
-AgentOps is officially supported on Crew's latest rc branch: `crewai==0.28.9rc1`
+AgentOps is integrated with CrewAI on a pre-release fork. Install crew with
 
-* [AgentOps integration example](https://docs.agentops.ai/v1/integrations/crewai)
-* [Offical CrewAI documentation](https://docs.crewai.com/how-to/AgentOps-Observability)
+```bash
+pip install git+https://github.com/AgentOps-AI/crewAI.git@main
+```
 
+- [AgentOps integration example](https://docs.agentops.ai/v1/integrations/crewai)
+- [Official CrewAI documentation](https://docs.crewai.com/how-to/AgentOps-Observability)
 
 ### Langchain 🦜🔗
+
 AgentOps works seamlessly with applications built using Langchain. To use the handler, install Langchain as an optional dependency:
+
+<details>
+  <summary>Installation</summary>
+  
 ```shell
 pip install agentops[langchain]
 ```
 
 To use the handler, import and set
 
 ```python
@@ -160,45 +147,100 @@
                          verbose=True,
                          callbacks=[handler], # You must pass in a callback handler to record your agent
                          handle_parsing_errors=True)
 ```
 
 Check out the [Langchain Examples Notebook](./examples/langchain_examples.ipynb) for more details including Async handlers.
 
-### LlamaIndex 🦙
-(Coming Soon)
+</details>
+
+### Cohere ⌨️
+
+First class support for Cohere(>=5.4.0). This is a living integration, should you need any added functionality please message us on Discord!
+
+- [AgentOps integration example](https://docs.agentops.ai/v1/integrations/cohere)
+- [Official Cohere documentation](https://docs.cohere.com/reference/about)
 
+<details>
+  <summary>Installation</summary>
+  
+```bash
+pip install cohere
+```
+
+```python python
+import cohere
+import agentops
 
+# Beginning of program's code (i.e. main.py, __init__.py)
+agentops.init(<INSERT YOUR API KEY HERE>)
+co = cohere.Client()
+
+chat = co.chat(
+    message="Is it pronounced ceaux-hear or co-hehray?"
+)
+
+print(chat)
+
+agentops.end_session('Success')
+```
+
+```python python
+import cohere
+import agentops
+
+# Beginning of program's code (i.e. main.py, __init__.py)
+agentops.init(<INSERT YOUR API KEY HERE>)
+
+co = cohere.Client()
+
+stream = co.chat_stream(
+    message="Write me a haiku about the synergies between Cohere and AgentOps"
+)
+
+for event in stream:
+    if event.event_type == "text-generation":
+        print(event.text, end='')
+
+agentops.end_session('Success')
+```
+</details>
+
+
+### LlamaIndex 🦙
+
+(Coming Soon)
 
 ## Time travel debugging 🔮
+
 (coming soon!)
 
 ## Agent Arena 🥊
+
 (coming soon!)
 
 ## Evaluations Roadmap 🧭
 
-| Platform | Dashboard | Evals |
-|---|---|---|
-|✅ Python SDK | ✅ Multi-session and Cross-session metrics | ✅ Custom eval metrics |
-|🚧 Evaluation builder API | ✅ Custom event tag tracking | 🔜 Agent scorecards |
-|✅ [Javascript/Typescript SDK](https://github.com/AgentOps-AI/agentops-node) | ✅ Session replays| 🔜 Evaluation playground + leaderboard|
-
+| Platform                                                                     | Dashboard                                  | Evals                                  |
+| ---------------------------------------------------------------------------- | ------------------------------------------ | -------------------------------------- |
+| ✅ Python SDK                                                                | ✅ Multi-session and Cross-session metrics | ✅ Custom eval metrics                 |
+| 🚧 Evaluation builder API                                                    | ✅ Custom event tag tracking               | 🔜 Agent scorecards                    |
+| ✅ [Javascript/Typescript SDK](https://github.com/AgentOps-AI/agentops-node) | ✅ Session replays                         | 🔜 Evaluation playground + leaderboard |
 
 ## Debugging Roadmap 🧭
 
-| Performance testing | Environments | LLM Testing | Reasoning and execution testing |
-|---|---|---|---|
-|✅ Event latency analysis | 🔜 Non-stationary environment testing | 🔜 LLM non-deterministic function detection | 🚧 Infinite loops and recursive thought detection |
-|✅ Agent workflow execution pricing | 🔜 Multi-modal environments | 🚧 Token limit overflow flags | 🔜 Faulty reasoning detection |
-|🚧 Success validators (external) | 🔜 Execution containers | 🔜 Context limit overflow flags | 🔜 Generative code validators |
-|🔜 Agent controllers/skill tests | ✅ Honeypot and prompt injection detection ([PromptArmor](https://promptarmor.com)) | 🔜 API bill tracking | 🔜 Error breakpoint analysis |
-|🔜 Information context constraint testing | 🔜 Anti-agent roadblocks (i.e. Captchas) | 🔜 CI/CD integration checks | |
-|🔜 Regression testing | 🔜 Multi-agent framework visualization | | |
+| Performance testing                       | Environments                                                                        | LLM Testing                                 | Reasoning and execution testing                   |
+| ----------------------------------------- | ----------------------------------------------------------------------------------- | ------------------------------------------- | ------------------------------------------------- |
+| ✅ Event latency analysis                 | 🔜 Non-stationary environment testing                                               | 🔜 LLM non-deterministic function detection | 🚧 Infinite loops and recursive thought detection |
+| ✅ Agent workflow execution pricing       | 🔜 Multi-modal environments                                                         | 🚧 Token limit overflow flags               | 🔜 Faulty reasoning detection                     |
+| 🚧 Success validators (external)          | 🔜 Execution containers                                                             | 🔜 Context limit overflow flags             | 🔜 Generative code validators                     |
+| 🔜 Agent controllers/skill tests          | ✅ Honeypot and prompt injection detection ([PromptArmor](https://promptarmor.com)) | 🔜 API bill tracking                        | 🔜 Error breakpoint analysis                      |
+| 🔜 Information context constraint testing | 🔜 Anti-agent roadblocks (i.e. Captchas)                                            | 🔜 CI/CD integration checks                 |                                                   |
+| 🔜 Regression testing                     | 🔜 Multi-agent framework visualization                                              |                                             |                                                   |
 
 ### Why AgentOps? 🤔
 
 Our mission is to bring your agent from prototype to production.
 
-Agent developers often work with little to no visibility into agent testing performance. This means their agents never leave the lab. We're changing that. 
+Agent developers often work with little to no visibility into agent testing performance. This means their agents never leave the lab. We're changing that.
 
 AgentOps is the easiest way to evaluate, grade, and test agents. Is there a feature you'd like to see AgentOps cover? Just raise it in the issues tab, and we'll work on adding it to the roadmap.
```

#### html2text {}

```diff
@@ -1,89 +1,92 @@
-Metadata-Version: 2.1 Name: agentops Version: 0.1.9 Summary: Python SDK for
-developing AI agent evals and observability Author-email: Alex Reibman
-gmail.com>, Shawn Qiu
-gmail.com>, Braelyn Boynton
-gmail.com>, Howard Gil
-gmail.com> Project-URL: Homepage, https://github.com/AgentOps-AI/agentops
-Project-URL: Issues, https://github.com/AgentOps-AI/agentops/issues Classifier:
-Programming Language :: Python :: 3 Classifier: License :: OSI Approved :: MIT
-License Classifier: Operating System :: OS Independent Requires-Python: >=3.7
-Description-Content-Type: text/markdown License-File: LICENSE Requires-Dist:
-requests==2.31.0 Requires-Dist: psutil==5.9.8 Requires-Dist: packaging==23.2
-Provides-Extra: dev Requires-Dist: pytest==7.4.0; extra == "dev" Requires-Dist:
-requests_mock==1.11.0; extra == "dev" Provides-Extra: langchain Requires-Dist:
-langchain>=0.0.354; extra == "langchain"
                                     _[_L_o_g_o_]
                      AAII aaggeennttss ssuucckk.. WWee?â??rree ffiixxiinngg tthhaatt..
                                _[_P_y_t_h_o_n_]_[_V_e_r_s_i_o_n_]
     _ð___¦_ _T_w_i_t_t_e_r   â¢   _ð___¢_ _D_i_s_c_o_r_d   â¢   _ð____ï_¸__ _A_g_e_n_t_O_p_s   â¢   _ð___
                                  _D_o_c_u_m_e_n_t_a_t_i_o_n
 # AgentOps ðï¸ [![License: MIT](https://img.shields.io/badge/License-MIT-
 yellow.svg)](https://opensource.org/licenses/MIT) ![PyPI - Version](https://
 img.shields.io/pypi/v/agentops) _[_h_t_t_p_s_:_/_/_s_t_a_t_i_c_._p_e_p_y_._t_e_c_h_/_b_a_d_g_e_/_a_g_e_n_t_o_p_s_/_m_o_n_t_h_]
-_[_A_g_e_n_t_O_p_s_ _T_w_i_t_t_e_r_]_[_D_i_s_c_o_r_d_ _c_o_m_m_u_n_i_t_y_ _c_h_a_n_n_e_l_]_[_h_t_t_p_s_:_/_/_i_m_g_._s_h_i_e_l_d_s_._i_o_/
-_w_e_b_s_i_t_e_?_c_o_l_o_r_=_%_2_3_f_2_6_5_2_2_&_d_o_w_n___m_e_s_s_a_g_e_=_Y_%_2_0_C_o_m_b_i_n_a_t_o_r_&_l_a_b_e_l_=_N_o_t_%_2_0_B_a_c_k_e_d_%_2_0_B_y_&_l_o_g_o_=_y_c_o_m_b_i_n_a_t_o_r_&_s_t_y_l_e_=_f_l_a_t_-
-_s_q_u_a_r_e_&_u_p___m_e_s_s_a_g_e_=_Y_%_2_0_C_o_m_b_i_n_a_t_o_r_&_u_r_l_=_h_t_t_p_s_%_3_A_%_2_F_%_2_F_w_w_w_._y_c_o_m_b_i_n_a_t_o_r_._c_o_m_]_[_g_i_t
-_c_o_m_m_i_t_ _a_c_t_i_v_i_t_y_]_A_g_e_n_t_O_p_s_ _h_e_l_p_s_ _d_e_v_e_l_o_p_e_r_s_ _b_u_i_l_d_,_ _e_v_a_l_u_a_t_e_,_ _a_n_d_ _m_o_n_i_t_o_r_ _A_I
-_a_g_e_n_t_s_._ _T_o_o_l_s_ _t_o_ _b_u_i_l_d_ _a_g_e_n_t_s_ _f_r_o_m_ _p_r_o_t_o_t_y_p_e_ _t_o_ _p_r_o_d_u_c_t_i_o_n_._ _|_|_|_ _|_-_-_-_-_-_-_-_-_-_-_-_-_-_-
-_-_-_-_-_-_-_-_-_-_-_-_-_-_-_-_-_-_-_-_-_-_-_-_-_-_-_-_-_|_-_-_-_-_-_-_-_-_-_-_-_-_-_-_-_-_-_-_-_-_-_-_-_-_-_-_-_-_-_-_-_-_-_-_-_-_-_-_-_-_-_-_-_-_-_-_-_-_-_-
-_-_-_|_ _|_ _ð____ _*_*_R_e_p_l_a_y_ _A_n_a_l_y_t_i_c_s_ _a_n_d_ _D_e_b_u_g_g_i_n_g_*_*_ _|_ _S_t_e_p_-_b_y_-_s_t_e_p_ _a_g_e_n_t_ _e_x_e_c_u_t_i_o_n
-_g_r_a_p_h_s_ _|_ _|_ _ð___¸_ _*_*_L_L_M_ _C_o_s_t_ _M_a_n_a_g_e_m_e_n_t_*_*_ _|_ _T_r_a_c_k_ _s_p_e_n_d_ _w_i_t_h_ _L_L_M_ _f_o_u_n_d_a_t_i_o_n_ _m_o_d_e_l
-_p_r_o_v_i_d_e_r_s_ _|_ _|_ _ð__§_ª_ _*_*_A_g_e_n_t_ _B_e_n_c_h_m_a_r_k_i_n_g_*_*_ _|_ _T_e_s_t_ _y_o_u_r_ _a_g_e_n_t_s_ _a_g_a_i_n_s_t_ _1_,_0_0_0_+
-_e_v_a_l_s_ _|_ _|_ _ð____ _*_*_C_o_m_p_l_i_a_n_c_e_ _a_n_d_ _S_e_c_u_r_i_t_y_*_*_ _|_ _D_e_t_e_c_t_ _c_o_m_m_o_n_ _p_r_o_m_p_t_ _i_n_j_e_c_t_i_o_n_ _a_n_d
-_d_a_t_a_ _e_x_f_i_l_t_r_a_t_i_o_n_ _e_x_p_l_o_i_t_s_ _|_ _|_ _ð__¤__ _*_*_F_r_a_m_e_w_o_r_k_ _I_n_t_e_g_r_a_t_i_o_n_s_*_*_ _|_ _E_a_s_i_l_y_ _p_l_u_g_s
-_i_n_ _w_i_t_h_ _f_r_a_m_e_w_o_r_k_s_ _l_i_k_e_ _C_r_e_w_A_I_ _a_n_d_ _L_a_n_g_C_h_a_i_n_ _|_ _#_#_ _Q_u_i_c_k_ _S_t_a_r_t_ _â__¨_ï_¸__ _`_`_`_p_y_t_h_o_n
-_p_i_p_ _i_n_s_t_a_l_l_ _a_g_e_n_t_o_p_s_ _`_`_`_ _#_#_#_ _S_e_s_s_i_o_n_ _r_e_p_l_a_y_s_ _i_n_ _3_ _l_i_n_e_s_ _o_f_ _c_o_d_e_ _I_n_i_t_i_a_l_i_z_e_ _t_h_e
-_A_g_e_n_t_O_p_s_ _c_l_i_e_n_t_ _a_n_d_ _a_u_t_o_m_a_t_i_c_a_l_l_y_ _g_e_t_ _a_n_a_l_y_t_i_c_s_ _o_n_ _e_v_e_r_y_ _L_L_M_ _c_a_l_l_._ _`_`_`_p_y_t_h_o_n
-_i_m_p_o_r_t_ _a_g_e_n_t_o_p_s_ _#_ _B_e_g_i_n_n_i_n_g_ _o_f_ _p_r_o_g_r_a_m_'_s_ _c_o_d_e_ _(_i_._e_._ _m_a_i_n_._p_y_,_ _____i_n_i_t_____._p_y_)
-_a_g_e_n_t_o_p_s_._i_n_i_t_(_)_ _._._._ _#_ _(_o_p_t_i_o_n_a_l_:_ _r_e_c_o_r_d_ _s_p_e_c_i_f_i_c_ _f_u_n_c_t_i_o_n_s_)
-_@_a_g_e_n_t_o_p_s_._r_e_c_o_r_d___f_u_n_c_t_i_o_n_(_'_s_a_m_p_l_e_ _f_u_n_c_t_i_o_n_ _b_e_i_n_g_ _r_e_c_o_r_d_'_)_ _d_e_f_ _s_a_m_p_l_e___f_u_n_c_t_i_o_n
-_(_._._._)_:_ _._._._ _#_ _E_n_d_ _o_f_ _p_r_o_g_r_a_m_ _a_g_e_n_t_o_p_s_._e_n_d___s_e_s_s_i_o_n_(_'_S_u_c_c_e_s_s_'_)_ _#_ _W_o_o_h_o_o_ _Y_o_u_'_r_e
-_d_o_n_e_ _ð____ _`_`_`_ _A_l_l_ _y_o_u_r_ _s_e_s_s_i_o_n_s_ _a_r_e_ _a_v_a_i_l_a_b_l_e_ _o_n_ _t_h_e_ _[_A_g_e_n_t_O_p_s_ _d_a_s_h_b_o_a_r_d_]
-_(_h_t_t_p_s_:_/_/_a_p_p_._a_g_e_n_t_o_p_s_._a_i_?_r_e_f_=_g_h_)_._ _R_e_f_e_r_ _t_o_ _o_u_r_ _[_A_P_I_ _d_o_c_u_m_e_n_t_a_t_i_o_n_]_(_h_t_t_p_:_/_/
-_d_o_c_s_._a_g_e_n_t_o_p_s_._a_i_)_ _f_o_r_ _d_e_t_a_i_l_e_d_ _i_n_s_t_r_u_c_t_i_o_n_s_._ _A_g_e_n_t_ _D_a_s_h_b_o_a_r_d_ _[_A_g_e_n_t
-_D_a_s_h_b_o_a_r_d_]_S_e_s_s_i_o_n_ _A_n_a_l_y_t_i_c_s_ _[_S_e_s_s_i_o_n_ _A_n_a_l_y_t_i_c_s_]_S_e_s_s_i_o_n_ _R_e_p_l_a_y_s_ _[_S_e_s_s_i_o_n
-_R_e_p_l_a_y_s_]_#_#_ _I_n_t_e_g_r_a_t_i_o_n_s_ _ð__¦_¾_ _#_#_#_ _C_r_e_w_A_I_ _ð___¶_ _B_u_i_l_d_ _C_r_e_w_ _a_g_e_n_t_s_ _w_i_t_h
-_o_b_s_e_r_v_a_b_i_l_i_t_y_ _w_i_t_h_ _o_n_l_y_ _2_ _l_i_n_e_s_ _o_f_ _c_o_d_e_._ _S_i_m_p_l_y_ _s_e_t_ _a_n_ _`_A_G_E_N_T_O_P_S___A_P_I___K_E_Y_`_ _i_n
-_y_o_u_r_ _e_n_v_i_r_o_n_m_e_n_t_,_ _a_n_d_ _y_o_u_r_ _c_r_e_w_s_ _w_i_l_l_ _g_e_t_ _a_u_t_o_m_a_t_i_c_ _m_o_n_i_t_o_r_i_n_g_ _o_n_ _t_h_e_ _A_g_e_n_t_O_p_s
-_d_a_s_h_b_o_a_r_d_._ _A_g_e_n_t_O_p_s_ _i_s_ _o_f_f_i_c_i_a_l_l_y_ _s_u_p_p_o_r_t_e_d_ _o_n_ _C_r_e_w_'_s_ _l_a_t_e_s_t_ _r_c_ _b_r_a_n_c_h_:
-_`_c_r_e_w_a_i_=_=_0_._2_8_._9_r_c_1_`_ _*_ _[_A_g_e_n_t_O_p_s_ _i_n_t_e_g_r_a_t_i_o_n_ _e_x_a_m_p_l_e_]_(_h_t_t_p_s_:_/_/_d_o_c_s_._a_g_e_n_t_o_p_s_._a_i_/
-_v_1_/_i_n_t_e_g_r_a_t_i_o_n_s_/_c_r_e_w_a_i_)_ _*_ _[_O_f_f_i_c_a_l_ _C_r_e_w_A_I_ _d_o_c_u_m_e_n_t_a_t_i_o_n_]_(_h_t_t_p_s_:_/_/
-_d_o_c_s_._c_r_e_w_a_i_._c_o_m_/_h_o_w_-_t_o_/_A_g_e_n_t_O_p_s_-_O_b_s_e_r_v_a_b_i_l_i_t_y_)_ _#_#_#_ _L_a_n_g_c_h_a_i_n_ _ð__¦__ð____ _A_g_e_n_t_O_p_s
-_w_o_r_k_s_ _s_e_a_m_l_e_s_s_l_y_ _w_i_t_h_ _a_p_p_l_i_c_a_t_i_o_n_s_ _b_u_i_l_t_ _u_s_i_n_g_ _L_a_n_g_c_h_a_i_n_._ _T_o_ _u_s_e_ _t_h_e_ _h_a_n_d_l_e_r_,
-_i_n_s_t_a_l_l_ _L_a_n_g_c_h_a_i_n_ _a_s_ _a_n_ _o_p_t_i_o_n_a_l_ _d_e_p_e_n_d_e_n_c_y_:_ _`_`_`_s_h_e_l_l_ _p_i_p_ _i_n_s_t_a_l_l_ _a_g_e_n_t_o_p_s
-_[_l_a_n_g_c_h_a_i_n_]_ _`_`_`_ _T_o_ _u_s_e_ _t_h_e_ _h_a_n_d_l_e_r_,_ _i_m_p_o_r_t_ _a_n_d_ _s_e_t_ _`_`_`_p_y_t_h_o_n_ _i_m_p_o_r_t_ _o_s_ _f_r_o_m
-_l_a_n_g_c_h_a_i_n_._c_h_a_t___m_o_d_e_l_s_ _i_m_p_o_r_t_ _C_h_a_t_O_p_e_n_A_I_ _f_r_o_m_ _l_a_n_g_c_h_a_i_n_._a_g_e_n_t_s_ _i_m_p_o_r_t
-_i_n_i_t_i_a_l_i_z_e___a_g_e_n_t_,_ _A_g_e_n_t_T_y_p_e_ _f_r_o_m_ _a_g_e_n_t_o_p_s_._l_a_n_g_c_h_a_i_n___c_a_l_l_b_a_c_k___h_a_n_d_l_e_r_ _i_m_p_o_r_t
-_L_a_n_g_c_h_a_i_n_C_a_l_l_b_a_c_k_H_a_n_d_l_e_r_ _A_G_E_N_T_O_P_S___A_P_I___K_E_Y_ _=_ _o_s_._e_n_v_i_r_o_n_[_'_A_G_E_N_T_O_P_S___A_P_I___K_E_Y_'_]
-_h_a_n_d_l_e_r_ _=_ _L_a_n_g_c_h_a_i_n_C_a_l_l_b_a_c_k_H_a_n_d_l_e_r_(_a_p_i___k_e_y_=_A_G_E_N_T_O_P_S___A_P_I___K_E_Y_,_ _t_a_g_s_=_[_'_L_a_n_g_c_h_a_i_n
-_E_x_a_m_p_l_e_'_]_)_ _l_l_m_ _=_ _C_h_a_t_O_p_e_n_A_I_(_o_p_e_n_a_i___a_p_i___k_e_y_=_O_P_E_N_A_I___A_P_I___K_E_Y_,_ _c_a_l_l_b_a_c_k_s_=_[_h_a_n_d_l_e_r_]_,
-_m_o_d_e_l_=_'_g_p_t_-_3_._5_-_t_u_r_b_o_'_)_ _a_g_e_n_t_ _=_ _i_n_i_t_i_a_l_i_z_e___a_g_e_n_t_(_t_o_o_l_s_,_ _l_l_m_,
-_a_g_e_n_t_=_A_g_e_n_t_T_y_p_e_._C_H_A_T___Z_E_R_O___S_H_O_T___R_E_A_C_T___D_E_S_C_R_I_P_T_I_O_N_,_ _v_e_r_b_o_s_e_=_T_r_u_e_,_ _c_a_l_l_b_a_c_k_s_=
-_[_h_a_n_d_l_e_r_]_,_ _#_ _Y_o_u_ _m_u_s_t_ _p_a_s_s_ _i_n_ _a_ _c_a_l_l_b_a_c_k_ _h_a_n_d_l_e_r_ _t_o_ _r_e_c_o_r_d_ _y_o_u_r_ _a_g_e_n_t
-_h_a_n_d_l_e___p_a_r_s_i_n_g___e_r_r_o_r_s_=_T_r_u_e_)_ _`_`_`_ _C_h_e_c_k_ _o_u_t_ _t_h_e_ _[_L_a_n_g_c_h_a_i_n_ _E_x_a_m_p_l_e_s_ _N_o_t_e_b_o_o_k_]_(_._/
-_e_x_a_m_p_l_e_s_/_l_a_n_g_c_h_a_i_n___e_x_a_m_p_l_e_s_._i_p_y_n_b_)_ _f_o_r_ _m_o_r_e_ _d_e_t_a_i_l_s_ _i_n_c_l_u_d_i_n_g_ _A_s_y_n_c_ _h_a_n_d_l_e_r_s_.
-_#_#_#_ _L_l_a_m_a_I_n_d_e_x_ _ð__¦__ _(_C_o_m_i_n_g_ _S_o_o_n_)_ _#_#_ _T_i_m_e_ _t_r_a_v_e_l_ _d_e_b_u_g_g_i_n_g_ _ð___®_ _(_c_o_m_i_n_g_ _s_o_o_n_!_)
-_#_#_ _A_g_e_n_t_ _A_r_e_n_a_ _ð__¥__ _(_c_o_m_i_n_g_ _s_o_o_n_!_)_ _#_#_ _E_v_a_l_u_a_t_i_o_n_s_ _R_o_a_d_m_a_p_ _ð__§_­_ _|_ _P_l_a_t_f_o_r_m_ _|
-_D_a_s_h_b_o_a_r_d_ _|_ _E_v_a_l_s_ _|_ _|_-_-_-_|_-_-_-_|_-_-_-_|_ _|_â___ _P_y_t_h_o_n_ _S_D_K_ _|_ _â___ _M_u_l_t_i_-_s_e_s_s_i_o_n_ _a_n_d
-_C_r_o_s_s_-_s_e_s_s_i_o_n_ _m_e_t_r_i_c_s_ _|_ _â___ _C_u_s_t_o_m_ _e_v_a_l_ _m_e_t_r_i_c_s_ _|_ _|_ð___§_ _E_v_a_l_u_a_t_i_o_n_ _b_u_i_l_d_e_r_ _A_P_I
-_|_ _â___ _C_u_s_t_o_m_ _e_v_e_n_t_ _t_a_g_ _t_r_a_c_k_i_n_g_Â_ _|_ _ð____ _A_g_e_n_t_ _s_c_o_r_e_c_a_r_d_s_ _|_ _|_â___ _[_J_a_v_a_s_c_r_i_p_t_/
-_T_y_p_e_s_c_r_i_p_t_ _S_D_K_]_(_h_t_t_p_s_:_/_/_g_i_t_h_u_b_._c_o_m_/_A_g_e_n_t_O_p_s_-_A_I_/_a_g_e_n_t_o_p_s_-_n_o_d_e_)_ _|_ _â___ _S_e_s_s_i_o_n
-_r_e_p_l_a_y_s_|_ _ð____ _E_v_a_l_u_a_t_i_o_n_ _p_l_a_y_g_r_o_u_n_d_ _+_ _l_e_a_d_e_r_b_o_a_r_d_|_ _#_#_ _D_e_b_u_g_g_i_n_g_ _R_o_a_d_m_a_p_ _ð__§_­_ _|
-_P_e_r_f_o_r_m_a_n_c_e_ _t_e_s_t_i_n_g_ _|_ _E_n_v_i_r_o_n_m_e_n_t_s_ _|_ _L_L_M_ _T_e_s_t_i_n_g_ _|_ _R_e_a_s_o_n_i_n_g_ _a_n_d_ _e_x_e_c_u_t_i_o_n
-_t_e_s_t_i_n_g_ _|_ _|_-_-_-_|_-_-_-_|_-_-_-_|_-_-_-_|_ _|_â___ _E_v_e_n_t_ _l_a_t_e_n_c_y_ _a_n_a_l_y_s_i_s_ _|_ _ð____ _N_o_n_-_s_t_a_t_i_o_n_a_r_y
-_e_n_v_i_r_o_n_m_e_n_t_ _t_e_s_t_i_n_g_ _|_ _ð____ _L_L_M_ _n_o_n_-_d_e_t_e_r_m_i_n_i_s_t_i_c_ _f_u_n_c_t_i_o_n_ _d_e_t_e_c_t_i_o_n_ _|_ _ð___§
-_I_n_f_i_n_i_t_e_ _l_o_o_p_s_ _a_n_d_ _r_e_c_u_r_s_i_v_e_ _t_h_o_u_g_h_t_ _d_e_t_e_c_t_i_o_n_ _|_ _|_â___ _A_g_e_n_t_ _w_o_r_k_f_l_o_w_ _e_x_e_c_u_t_i_o_n
-_p_r_i_c_i_n_g_ _|_ _ð____ _M_u_l_t_i_-_m_o_d_a_l_ _e_n_v_i_r_o_n_m_e_n_t_s_ _|_ _ð___§_ _T_o_k_e_n_ _l_i_m_i_t_ _o_v_e_r_f_l_o_w_ _f_l_a_g_s_ _|
-_ð____ _F_a_u_l_t_y_ _r_e_a_s_o_n_i_n_g_ _d_e_t_e_c_t_i_o_n_ _|_ _|_ð___§_ _S_u_c_c_e_s_s_ _v_a_l_i_d_a_t_o_r_s_ _(_e_x_t_e_r_n_a_l_)_ _|_ _ð___
-_E_x_e_c_u_t_i_o_n_ _c_o_n_t_a_i_n_e_r_s_ _|_ _ð____ _C_o_n_t_e_x_t_ _l_i_m_i_t_ _o_v_e_r_f_l_o_w_ _f_l_a_g_s_ _|_ _ð____ _G_e_n_e_r_a_t_i_v_e_ _c_o_d_e
-_v_a_l_i_d_a_t_o_r_s_ _|_ _|_ð____ _A_g_e_n_t_ _c_o_n_t_r_o_l_l_e_r_s_/_s_k_i_l_l_ _t_e_s_t_s_ _|_ _â___ _H_o_n_e_y_p_o_t_ _a_n_d_ _p_r_o_m_p_t
-_i_n_j_e_c_t_i_o_n_ _d_e_t_e_c_t_i_o_n_ _(_[_P_r_o_m_p_t_A_r_m_o_r_]_(_h_t_t_p_s_:_/_/_p_r_o_m_p_t_a_r_m_o_r_._c_o_m_)_)_ _|_ _ð____ _A_P_I_ _b_i_l_l
-_t_r_a_c_k_i_n_g_ _|_ _ð____ _E_r_r_o_r_ _b_r_e_a_k_p_o_i_n_t_ _a_n_a_l_y_s_i_s_ _|_ _|_ð____ _I_n_f_o_r_m_a_t_i_o_n_ _c_o_n_t_e_x_t
-_c_o_n_s_t_r_a_i_n_t_ _t_e_s_t_i_n_g_ _|_ _ð____ _A_n_t_i_-_a_g_e_n_t_ _r_o_a_d_b_l_o_c_k_s_ _(_i_._e_._ _C_a_p_t_c_h_a_s_)_ _|_ _ð____ _C_I_/_C_D
-_i_n_t_e_g_r_a_t_i_o_n_ _c_h_e_c_k_s_ _|_ _|_ _|_ð____ _R_e_g_r_e_s_s_i_o_n_ _t_e_s_t_i_n_g_ _|_ _ð____ _M_u_l_t_i_-_a_g_e_n_t_ _f_r_a_m_e_w_o_r_k
-_v_i_s_u_a_l_i_z_a_t_i_o_n_ _|_ _|_ _|_ _#_#_#_ _W_h_y_ _A_g_e_n_t_O_p_s_?_ _ð__¤__ _O_u_r_ _m_i_s_s_i_o_n_ _i_s_ _t_o_ _b_r_i_n_g_ _y_o_u_r_ _a_g_e_n_t
-_f_r_o_m_ _p_r_o_t_o_t_y_p_e_ _t_o_ _p_r_o_d_u_c_t_i_o_n_._ _A_g_e_n_t_ _d_e_v_e_l_o_p_e_r_s_ _o_f_t_e_n_ _w_o_r_k_ _w_i_t_h_ _l_i_t_t_l_e_ _t_o_ _n_o
-_v_i_s_i_b_i_l_i_t_y_ _i_n_t_o_ _a_g_e_n_t_ _t_e_s_t_i_n_g_ _p_e_r_f_o_r_m_a_n_c_e_._ _T_h_i_s_ _m_e_a_n_s_ _t_h_e_i_r_ _a_g_e_n_t_s_ _n_e_v_e_r_ _l_e_a_v_e
-_t_h_e_ _l_a_b_._ _W_e_'_r_e_ _c_h_a_n_g_i_n_g_ _t_h_a_t_._ _A_g_e_n_t_O_p_s_ _i_s_ _t_h_e_ _e_a_s_i_e_s_t_ _w_a_y_ _t_o_ _e_v_a_l_u_a_t_e_,_ _g_r_a_d_e_,
-_a_n_d_ _t_e_s_t_ _a_g_e_n_t_s_._ _I_s_ _t_h_e_r_e_ _a_ _f_e_a_t_u_r_e_ _y_o_u_'_d_ _l_i_k_e_ _t_o_ _s_e_e_ _A_g_e_n_t_O_p_s_ _c_o_v_e_r_?_ _J_u_s_t
-_r_a_i_s_e_ _i_t_ _i_n_ _t_h_e_ _i_s_s_u_e_s_ _t_a_b_,_ _a_n_d_ _w_e_'_l_l_ _w_o_r_k_ _o_n_ _a_d_d_i_n_g_ _i_t_ _t_o_ _t_h_e_ _r_o_a_d_m_a_p_.
+_[_A_g_e_n_t_O_p_s_ _T_w_i_t_t_e_r_]_[_D_i_s_c_o_r_d_ _c_o_m_m_u_n_i_t_y_ _c_h_a_n_n_e_l_]_[_g_i_t_ _c_o_m_m_i_t_ _a_c_t_i_v_i_t_y_]AgentOps
+helps developers build, evaluate, and monitor AI agents. Tools to build agents
+from prototype to production. | | | | ------------------------------------- | -
+------------------------------------------------------------ | | ð **Replay
+Analytics and Debugging** | Step-by-step agent execution graphs | | ð¸ **LLM
+Cost Management** | Track spend with LLM foundation model providers | | ð§ª
+**Agent Benchmarking** | Test your agents against 1,000+ evals | | ð
+**Compliance and Security** | Detect common prompt injection and data
+exfiltration exploits | | ð¤ **Framework Integrations** | Easily plugs in
+with frameworks like CrewAI and LangChain | ## Quick Start â¨ï¸ ```bash pip
+install agentops ``` ### Session replays in 3 lines of code Initialize the
+AgentOps client and automatically get analytics on every LLM call. ```python
+import agentops # Beginning of program's code (i.e. main.py, __init__.py)
+agentops.init() ... # (optional: record specific functions)
+@agentops.record_function('sample function being record') def sample_function
+(...): ... # End of program agentops.end_session('Success') # Woohoo You're
+done ð ``` All your sessions are available on the [AgentOps dashboard]
+(https://app.agentops.ai?ref=gh). Refer to our [API documentation](http://
+docs.agentops.ai) for detailed instructions. Agent Dashboard _[_A_g_e_n_t
+_D_a_s_h_b_o_a_r_d_]Session Analytics _[_S_e_s_s_i_o_n_ _A_n_a_l_y_t_i_c_s_]Session Replays _[_S_e_s_s_i_o_n
+_R_e_p_l_a_y_s_]## Integrations ð¦¾ ### CrewAI ð¶ Build Crew agents with
+observability with only 2 lines of code. Simply set an `AGENTOPS_API_KEY` in
+your environment, and your crews will get automatic monitoring on the AgentOps
+dashboard. AgentOps is integrated with CrewAI on a pre-release fork. Install
+crew with ```bash pip install git+https://github.com/AgentOps-AI/
+crewAI.git@main ``` - [AgentOps integration example](https://docs.agentops.ai/
+v1/integrations/crewai) - [Official CrewAI documentation](https://
+docs.crewai.com/how-to/AgentOps-Observability) ### Langchain ð¦ð AgentOps
+works seamlessly with applications built using Langchain. To use the handler,
+install Langchain as an optional dependency: Installation ```shell pip install
+agentops[langchain] ``` To use the handler, import and set ```python import os
+from langchain.chat_models import ChatOpenAI from langchain.agents import
+initialize_agent, AgentType from agentops.langchain_callback_handler import
+LangchainCallbackHandler AGENTOPS_API_KEY = os.environ['AGENTOPS_API_KEY']
+handler = LangchainCallbackHandler(api_key=AGENTOPS_API_KEY, tags=['Langchain
+Example']) llm = ChatOpenAI(openai_api_key=OPENAI_API_KEY, callbacks=[handler],
+model='gpt-3.5-turbo') agent = initialize_agent(tools, llm,
+agent=AgentType.CHAT_ZERO_SHOT_REACT_DESCRIPTION, verbose=True, callbacks=
+[handler], # You must pass in a callback handler to record your agent
+handle_parsing_errors=True) ``` Check out the [Langchain Examples Notebook](./
+examples/langchain_examples.ipynb) for more details including Async handlers.
+### Cohere â¨ï¸ First class support for Cohere(>=5.4.0). This is a living
+integration, should you need any added functionality please message us on
+Discord! - [AgentOps integration example](https://docs.agentops.ai/v1/
+integrations/cohere) - [Official Cohere documentation](https://docs.cohere.com/
+reference/about) Installation ```bash pip install cohere ``` ```python python
+import cohere import agentops # Beginning of program's code (i.e. main.py,
+__init__.py) agentops.init() co = cohere.Client() chat = co.chat( message="Is
+it pronounced ceaux-hear or co-hehray?" ) print(chat) agentops.end_session
+('Success') ``` ```python python import cohere import agentops # Beginning of
+program's code (i.e. main.py, __init__.py) agentops.init() co = cohere.Client()
+stream = co.chat_stream( message="Write me a haiku about the synergies between
+Cohere and AgentOps" ) for event in stream: if event.event_type == "text-
+generation": print(event.text, end='') agentops.end_session('Success') ``` ###
+LlamaIndex ð¦ (Coming Soon) ## Time travel debugging ð® (coming soon!) ##
+Agent Arena ð¥ (coming soon!) ## Evaluations Roadmap ð§­ | Platform |
+Dashboard | Evals | | ---------------------------------------------------------
+------------------- | ------------------------------------------ | ------------
+-------------------------- | | â Python SDK | â Multi-session and Cross-
+session metrics | â Custom eval metrics | | ð§ Evaluation builder API | â
+Custom event tag trackingÂ  | ð Agent scorecards | | â [Javascript/
+Typescript SDK](https://github.com/AgentOps-AI/agentops-node) | â Session
+replays | ð Evaluation playground + leaderboard | ## Debugging Roadmap ð§­
+| Performance testing | Environments | LLM Testing | Reasoning and execution
+testing | | ----------------------------------------- | -----------------------
+------------------------------------------------------------ | ----------------
+--------------------------- | ------------------------------------------------
+- | | â Event latency analysis | ð Non-stationary environment testing |
+ð LLM non-deterministic function detection | ð§ Infinite loops and
+recursive thought detection | | â Agent workflow execution pricing | ð
+Multi-modal environments | ð§ Token limit overflow flags | ð Faulty
+reasoning detection | | ð§ Success validators (external) | ð Execution
+containers | ð Context limit overflow flags | ð Generative code
+validators | | ð Agent controllers/skill tests | â Honeypot and prompt
+injection detection ([PromptArmor](https://promptarmor.com)) | ð API bill
+tracking | ð Error breakpoint analysis | | ð Information context
+constraint testing | ð Anti-agent roadblocks (i.e. Captchas) | ð CI/CD
+integration checks | | | ð Regression testing | ð Multi-agent framework
+visualization | | | ### Why AgentOps? ð¤ Our mission is to bring your agent
+from prototype to production. Agent developers often work with little to no
+visibility into agent testing performance. This means their agents never leave
+the lab. We're changing that. AgentOps is the easiest way to evaluate, grade,
+and test agents. Is there a feature you'd like to see AgentOps cover? Just
+raise it in the issues tab, and we'll work on adding it to the roadmap.
```

### Comparing `agentops-0.1.9/README.md` & `agentops-0.2.0/PKG-INFO`

 * *Files 20% similar despite different names*

```diff
@@ -1,10 +1,32 @@
+Metadata-Version: 2.1
+Name: agentops
+Version: 0.2.0
+Summary: Python SDK for developing AI agent evals and observability
+Author-email: Alex Reibman <areibman@gmail.com>, Shawn Qiu <siyangqiu@gmail.com>, Braelyn Boynton <bboynton97@gmail.com>, Howard Gil <howardbgil@gmail.com>
+Project-URL: Homepage, https://github.com/AgentOps-AI/agentops
+Project-URL: Issues, https://github.com/AgentOps-AI/agentops/issues
+Classifier: Programming Language :: Python :: 3
+Classifier: License :: OSI Approved :: MIT License
+Classifier: Operating System :: OS Independent
+Requires-Python: >=3.7
+Description-Content-Type: text/markdown
+License-File: LICENSE
+Requires-Dist: requests==2.31.0
+Requires-Dist: psutil==5.9.8
+Requires-Dist: packaging==23.2
+Provides-Extra: dev
+Requires-Dist: pytest==7.4.0; extra == "dev"
+Requires-Dist: requests_mock==1.11.0; extra == "dev"
+Provides-Extra: langchain
+Requires-Dist: langchain~=1.19; extra == "langchain"
+
 <div align="center">
   <a href="https://agentops.ai?ref=gh">
-    <img src="https://github.com/AgentOps-AI/agentops/blob/df22e9dffb7294fb977dc103a2ca3bcf8f04946f/logo.png" style="margin: 15px; max-width: 300px" width="50%" alt="Logo">
+    <img src="https://raw.githubusercontent.com/AgentOps-AI/agentops/35d5682866921a9e28d8ef66ae3c3b3d92d8fa6b/img/logo.png" style="margin: 15px; max-width: 300px" width="50%" alt="Logo">
   </a>
 </div>
 <p align="center">
   <em>AI agents suck. We’re fixing that.</em>
 </p>
 
 <p align="center">
@@ -21,45 +43,47 @@
 <a href="https://app.agentops.ai/?ref=gh">🖇️ AgentOps</a>
 <span>&nbsp;&nbsp;•&nbsp;&nbsp;</span>
 <a href="https://docs.agentops.ai/introduction">📙 Documentation</a>
 </p>
 
 # AgentOps 🖇️
 
-[![License: MIT](https://img.shields.io/badge/License-MIT-yellow.svg)](https://opensource.org/licenses/MIT) ![PyPI - Version](https://img.shields.io/pypi/v/agentops) <a href="https://pepy.tech/project/agentops">
-  <img src="https://static.pepy.tech/badge/agentops/month"> <a href="https://twitter.com/agentopsai">
-    <img src="https://img.shields.io/badge/follow-%40agentops-1DA1F2?logo=twitter&style=social" alt="AgentOps Twitter" /> 
-  </a>
-  <a href="https://discord.gg/mKW3ZhN9p2">
-    <img src="https://img.shields.io/badge/chat-on%20Discord-blueviolet" alt="Discord community channel" />
-  </a>
-  <a href="mailto:investor@agentops.ai"><img src="https://img.shields.io/website?color=%23f26522&down_message=Y%20Combinator&label=Not%20Backed%20By&logo=ycombinator&style=flat-square&up_message=Y%20Combinator&url=https%3A%2F%2Fwww.ycombinator.com"/>
-  <a href="https://github.com/agentops-ai/agentops/issues">
-    <img src="https://img.shields.io/github/commit-activity/m/agentops-ai/agentops" alt="git commit activity" />
-  </a>
-
+[![License: MIT](https://img.shields.io/badge/License-MIT-yellow.svg)](https://opensource.org/licenses/MIT)
+![PyPI - Version](https://img.shields.io/pypi/v/agentops)
+<a href="https://pepy.tech/project/agentops">
+  <img src="https://static.pepy.tech/badge/agentops/month">
+</a>
+<a href="https://twitter.com/agentopsai">
+  <img src="https://img.shields.io/badge/follow-%40agentops-1DA1F2?logo=twitter&style=social" alt="AgentOps Twitter"/>
+</a>
+<a href="https://discord.gg/mKW3ZhN9p2">
+  <img src="https://img.shields.io/badge/chat-on%20Discord-blueviolet" alt="Discord community channel"/>
+</a>
+<a href="https://github.com/agentops-ai/agentops/issues">
+  <img src="https://img.shields.io/github/commit-activity/m/agentops-ai/agentops" alt="git commit activity"/>
+</a>
 
 AgentOps helps developers build, evaluate, and monitor AI agents. Tools to build agents from prototype to production.
 
-
-|||
-|------------------------------------------|----------------------------------------------------|
-| 📊 **Replay Analytics and Debugging** | Step-by-step agent execution graphs |
-| 💸 **LLM Cost Management**   | Track spend with LLM foundation model providers |
-| 🧪 **Agent Benchmarking** | Test your agents against 1,000+ evals |
-| 🔐 **Compliance and Security**            | Detect common prompt injection and data exfiltration exploits |
-| 🤝 **Framework Integrations**            | Easily plugs in with frameworks like CrewAI and LangChain |
+|                                       |                                                               |
+| ------------------------------------- | ------------------------------------------------------------- |
+| 📊 **Replay Analytics and Debugging** | Step-by-step agent execution graphs                           |
+| 💸 **LLM Cost Management**            | Track spend with LLM foundation model providers               |
+| 🧪 **Agent Benchmarking**             | Test your agents against 1,000+ evals                         |
+| 🔐 **Compliance and Security**        | Detect common prompt injection and data exfiltration exploits |
+| 🤝 **Framework Integrations**         | Easily plugs in with frameworks like CrewAI and LangChain     |
 
 ## Quick Start ⌨️
 
-```python
+```bash
 pip install agentops
 ```
 
 ### Session replays in 3 lines of code
+
 Initialize the AgentOps client and automatically get analytics on every LLM call.
 
 ```python
 import agentops
 
 # Beginning of program's code (i.e. main.py, __init__.py)
 agentops.init(<INSERT YOUR API KEY HERE>)
@@ -73,15 +97,14 @@
 # End of program
 agentops.end_session('Success')
 # Woohoo You're done 🎉
 ```
 
 All your sessions are available on the [AgentOps dashboard](https://app.agentops.ai?ref=gh). Refer to our [API documentation](http://docs.agentops.ai) for detailed instructions.
 
-
 <details open>
   <summary>Agent Dashboard</summary>
   <a href="https://app.agentops.ai?ref=gh">
    <img src="https://github.com/AgentOps-AI/agentops/assets/14807319/158e082a-9a7d-49b7-9b41-51a49a1f7d3d" style="width: 90%;" alt="Agent Dashboard"/>
   </a>
 </details>
 
@@ -101,22 +124,30 @@
 
 ## Integrations 🦾
 
 ### CrewAI 🛶
 
 Build Crew agents with observability with only 2 lines of code. Simply set an `AGENTOPS_API_KEY` in your environment, and your crews will get automatic monitoring on the AgentOps dashboard.
 
-AgentOps is officially supported on Crew's latest rc branch: `crewai==0.28.9rc1`
+AgentOps is integrated with CrewAI on a pre-release fork. Install crew with
 
-* [AgentOps integration example](https://docs.agentops.ai/v1/integrations/crewai)
-* [Offical CrewAI documentation](https://docs.crewai.com/how-to/AgentOps-Observability)
+```bash
+pip install git+https://github.com/AgentOps-AI/crewAI.git@main
+```
 
+- [AgentOps integration example](https://docs.agentops.ai/v1/integrations/crewai)
+- [Official CrewAI documentation](https://docs.crewai.com/how-to/AgentOps-Observability)
 
 ### Langchain 🦜🔗
+
 AgentOps works seamlessly with applications built using Langchain. To use the handler, install Langchain as an optional dependency:
+
+<details>
+  <summary>Installation</summary>
+  
 ```shell
 pip install agentops[langchain]
 ```
 
 To use the handler, import and set
 
 ```python
@@ -138,45 +169,100 @@
                          verbose=True,
                          callbacks=[handler], # You must pass in a callback handler to record your agent
                          handle_parsing_errors=True)
 ```
 
 Check out the [Langchain Examples Notebook](./examples/langchain_examples.ipynb) for more details including Async handlers.
 
-### LlamaIndex 🦙
-(Coming Soon)
+</details>
+
+### Cohere ⌨️
+
+First class support for Cohere(>=5.4.0). This is a living integration, should you need any added functionality please message us on Discord!
+
+- [AgentOps integration example](https://docs.agentops.ai/v1/integrations/cohere)
+- [Official Cohere documentation](https://docs.cohere.com/reference/about)
 
+<details>
+  <summary>Installation</summary>
+  
+```bash
+pip install cohere
+```
+
+```python python
+import cohere
+import agentops
 
+# Beginning of program's code (i.e. main.py, __init__.py)
+agentops.init(<INSERT YOUR API KEY HERE>)
+co = cohere.Client()
+
+chat = co.chat(
+    message="Is it pronounced ceaux-hear or co-hehray?"
+)
+
+print(chat)
+
+agentops.end_session('Success')
+```
+
+```python python
+import cohere
+import agentops
+
+# Beginning of program's code (i.e. main.py, __init__.py)
+agentops.init(<INSERT YOUR API KEY HERE>)
+
+co = cohere.Client()
+
+stream = co.chat_stream(
+    message="Write me a haiku about the synergies between Cohere and AgentOps"
+)
+
+for event in stream:
+    if event.event_type == "text-generation":
+        print(event.text, end='')
+
+agentops.end_session('Success')
+```
+</details>
+
+
+### LlamaIndex 🦙
+
+(Coming Soon)
 
 ## Time travel debugging 🔮
+
 (coming soon!)
 
 ## Agent Arena 🥊
+
 (coming soon!)
 
 ## Evaluations Roadmap 🧭
 
-| Platform | Dashboard | Evals |
-|---|---|---|
-|✅ Python SDK | ✅ Multi-session and Cross-session metrics | ✅ Custom eval metrics |
-|🚧 Evaluation builder API | ✅ Custom event tag tracking | 🔜 Agent scorecards |
-|✅ [Javascript/Typescript SDK](https://github.com/AgentOps-AI/agentops-node) | ✅ Session replays| 🔜 Evaluation playground + leaderboard|
-
+| Platform                                                                     | Dashboard                                  | Evals                                  |
+| ---------------------------------------------------------------------------- | ------------------------------------------ | -------------------------------------- |
+| ✅ Python SDK                                                                | ✅ Multi-session and Cross-session metrics | ✅ Custom eval metrics                 |
+| 🚧 Evaluation builder API                                                    | ✅ Custom event tag tracking               | 🔜 Agent scorecards                    |
+| ✅ [Javascript/Typescript SDK](https://github.com/AgentOps-AI/agentops-node) | ✅ Session replays                         | 🔜 Evaluation playground + leaderboard |
 
 ## Debugging Roadmap 🧭
 
-| Performance testing | Environments | LLM Testing | Reasoning and execution testing |
-|---|---|---|---|
-|✅ Event latency analysis | 🔜 Non-stationary environment testing | 🔜 LLM non-deterministic function detection | 🚧 Infinite loops and recursive thought detection |
-|✅ Agent workflow execution pricing | 🔜 Multi-modal environments | 🚧 Token limit overflow flags | 🔜 Faulty reasoning detection |
-|🚧 Success validators (external) | 🔜 Execution containers | 🔜 Context limit overflow flags | 🔜 Generative code validators |
-|🔜 Agent controllers/skill tests | ✅ Honeypot and prompt injection detection ([PromptArmor](https://promptarmor.com)) | 🔜 API bill tracking | 🔜 Error breakpoint analysis |
-|🔜 Information context constraint testing | 🔜 Anti-agent roadblocks (i.e. Captchas) | 🔜 CI/CD integration checks | |
-|🔜 Regression testing | 🔜 Multi-agent framework visualization | | |
+| Performance testing                       | Environments                                                                        | LLM Testing                                 | Reasoning and execution testing                   |
+| ----------------------------------------- | ----------------------------------------------------------------------------------- | ------------------------------------------- | ------------------------------------------------- |
+| ✅ Event latency analysis                 | 🔜 Non-stationary environment testing                                               | 🔜 LLM non-deterministic function detection | 🚧 Infinite loops and recursive thought detection |
+| ✅ Agent workflow execution pricing       | 🔜 Multi-modal environments                                                         | 🚧 Token limit overflow flags               | 🔜 Faulty reasoning detection                     |
+| 🚧 Success validators (external)          | 🔜 Execution containers                                                             | 🔜 Context limit overflow flags             | 🔜 Generative code validators                     |
+| 🔜 Agent controllers/skill tests          | ✅ Honeypot and prompt injection detection ([PromptArmor](https://promptarmor.com)) | 🔜 API bill tracking                        | 🔜 Error breakpoint analysis                      |
+| 🔜 Information context constraint testing | 🔜 Anti-agent roadblocks (i.e. Captchas)                                            | 🔜 CI/CD integration checks                 |                                                   |
+| 🔜 Regression testing                     | 🔜 Multi-agent framework visualization                                              |                                             |                                                   |
 
 ### Why AgentOps? 🤔
 
 Our mission is to bring your agent from prototype to production.
 
-Agent developers often work with little to no visibility into agent testing performance. This means their agents never leave the lab. We're changing that. 
+Agent developers often work with little to no visibility into agent testing performance. This means their agents never leave the lab. We're changing that.
 
 AgentOps is the easiest way to evaluate, grade, and test agents. Is there a feature you'd like to see AgentOps cover? Just raise it in the issues tab, and we'll work on adding it to the roadmap.
```

#### html2text {}

```diff
@@ -1,75 +1,106 @@
+Metadata-Version: 2.1 Name: agentops Version: 0.2.0 Summary: Python SDK for
+developing AI agent evals and observability Author-email: Alex Reibman
+gmail.com>, Shawn Qiu
+gmail.com>, Braelyn Boynton
+gmail.com>, Howard Gil
+gmail.com> Project-URL: Homepage, https://github.com/AgentOps-AI/agentops
+Project-URL: Issues, https://github.com/AgentOps-AI/agentops/issues Classifier:
+Programming Language :: Python :: 3 Classifier: License :: OSI Approved :: MIT
+License Classifier: Operating System :: OS Independent Requires-Python: >=3.7
+Description-Content-Type: text/markdown License-File: LICENSE Requires-Dist:
+requests==2.31.0 Requires-Dist: psutil==5.9.8 Requires-Dist: packaging==23.2
+Provides-Extra: dev Requires-Dist: pytest==7.4.0; extra == "dev" Requires-Dist:
+requests_mock==1.11.0; extra == "dev" Provides-Extra: langchain Requires-Dist:
+langchain~=1.19; extra == "langchain"
                                     _[_L_o_g_o_]
                      AAII aaggeennttss ssuucckk.. WWee?â??rree ffiixxiinngg tthhaatt..
                                _[_P_y_t_h_o_n_]_[_V_e_r_s_i_o_n_]
     _ð___¦_ _T_w_i_t_t_e_r   â¢   _ð___¢_ _D_i_s_c_o_r_d   â¢   _ð____ï_¸__ _A_g_e_n_t_O_p_s   â¢   _ð___
                                  _D_o_c_u_m_e_n_t_a_t_i_o_n
 # AgentOps ðï¸ [![License: MIT](https://img.shields.io/badge/License-MIT-
 yellow.svg)](https://opensource.org/licenses/MIT) ![PyPI - Version](https://
 img.shields.io/pypi/v/agentops) _[_h_t_t_p_s_:_/_/_s_t_a_t_i_c_._p_e_p_y_._t_e_c_h_/_b_a_d_g_e_/_a_g_e_n_t_o_p_s_/_m_o_n_t_h_]
-_[_A_g_e_n_t_O_p_s_ _T_w_i_t_t_e_r_]_[_D_i_s_c_o_r_d_ _c_o_m_m_u_n_i_t_y_ _c_h_a_n_n_e_l_]_[_h_t_t_p_s_:_/_/_i_m_g_._s_h_i_e_l_d_s_._i_o_/
-_w_e_b_s_i_t_e_?_c_o_l_o_r_=_%_2_3_f_2_6_5_2_2_&_d_o_w_n___m_e_s_s_a_g_e_=_Y_%_2_0_C_o_m_b_i_n_a_t_o_r_&_l_a_b_e_l_=_N_o_t_%_2_0_B_a_c_k_e_d_%_2_0_B_y_&_l_o_g_o_=_y_c_o_m_b_i_n_a_t_o_r_&_s_t_y_l_e_=_f_l_a_t_-
-_s_q_u_a_r_e_&_u_p___m_e_s_s_a_g_e_=_Y_%_2_0_C_o_m_b_i_n_a_t_o_r_&_u_r_l_=_h_t_t_p_s_%_3_A_%_2_F_%_2_F_w_w_w_._y_c_o_m_b_i_n_a_t_o_r_._c_o_m_]_[_g_i_t
-_c_o_m_m_i_t_ _a_c_t_i_v_i_t_y_]_A_g_e_n_t_O_p_s_ _h_e_l_p_s_ _d_e_v_e_l_o_p_e_r_s_ _b_u_i_l_d_,_ _e_v_a_l_u_a_t_e_,_ _a_n_d_ _m_o_n_i_t_o_r_ _A_I
-_a_g_e_n_t_s_._ _T_o_o_l_s_ _t_o_ _b_u_i_l_d_ _a_g_e_n_t_s_ _f_r_o_m_ _p_r_o_t_o_t_y_p_e_ _t_o_ _p_r_o_d_u_c_t_i_o_n_._ _|_|_|_ _|_-_-_-_-_-_-_-_-_-_-_-_-_-_-
-_-_-_-_-_-_-_-_-_-_-_-_-_-_-_-_-_-_-_-_-_-_-_-_-_-_-_-_-_|_-_-_-_-_-_-_-_-_-_-_-_-_-_-_-_-_-_-_-_-_-_-_-_-_-_-_-_-_-_-_-_-_-_-_-_-_-_-_-_-_-_-_-_-_-_-_-_-_-_-
-_-_-_|_ _|_ _ð____ _*_*_R_e_p_l_a_y_ _A_n_a_l_y_t_i_c_s_ _a_n_d_ _D_e_b_u_g_g_i_n_g_*_*_ _|_ _S_t_e_p_-_b_y_-_s_t_e_p_ _a_g_e_n_t_ _e_x_e_c_u_t_i_o_n
-_g_r_a_p_h_s_ _|_ _|_ _ð___¸_ _*_*_L_L_M_ _C_o_s_t_ _M_a_n_a_g_e_m_e_n_t_*_*_ _|_ _T_r_a_c_k_ _s_p_e_n_d_ _w_i_t_h_ _L_L_M_ _f_o_u_n_d_a_t_i_o_n_ _m_o_d_e_l
-_p_r_o_v_i_d_e_r_s_ _|_ _|_ _ð__§_ª_ _*_*_A_g_e_n_t_ _B_e_n_c_h_m_a_r_k_i_n_g_*_*_ _|_ _T_e_s_t_ _y_o_u_r_ _a_g_e_n_t_s_ _a_g_a_i_n_s_t_ _1_,_0_0_0_+
-_e_v_a_l_s_ _|_ _|_ _ð____ _*_*_C_o_m_p_l_i_a_n_c_e_ _a_n_d_ _S_e_c_u_r_i_t_y_*_*_ _|_ _D_e_t_e_c_t_ _c_o_m_m_o_n_ _p_r_o_m_p_t_ _i_n_j_e_c_t_i_o_n_ _a_n_d
-_d_a_t_a_ _e_x_f_i_l_t_r_a_t_i_o_n_ _e_x_p_l_o_i_t_s_ _|_ _|_ _ð__¤__ _*_*_F_r_a_m_e_w_o_r_k_ _I_n_t_e_g_r_a_t_i_o_n_s_*_*_ _|_ _E_a_s_i_l_y_ _p_l_u_g_s
-_i_n_ _w_i_t_h_ _f_r_a_m_e_w_o_r_k_s_ _l_i_k_e_ _C_r_e_w_A_I_ _a_n_d_ _L_a_n_g_C_h_a_i_n_ _|_ _#_#_ _Q_u_i_c_k_ _S_t_a_r_t_ _â__¨_ï_¸__ _`_`_`_p_y_t_h_o_n
-_p_i_p_ _i_n_s_t_a_l_l_ _a_g_e_n_t_o_p_s_ _`_`_`_ _#_#_#_ _S_e_s_s_i_o_n_ _r_e_p_l_a_y_s_ _i_n_ _3_ _l_i_n_e_s_ _o_f_ _c_o_d_e_ _I_n_i_t_i_a_l_i_z_e_ _t_h_e
-_A_g_e_n_t_O_p_s_ _c_l_i_e_n_t_ _a_n_d_ _a_u_t_o_m_a_t_i_c_a_l_l_y_ _g_e_t_ _a_n_a_l_y_t_i_c_s_ _o_n_ _e_v_e_r_y_ _L_L_M_ _c_a_l_l_._ _`_`_`_p_y_t_h_o_n
-_i_m_p_o_r_t_ _a_g_e_n_t_o_p_s_ _#_ _B_e_g_i_n_n_i_n_g_ _o_f_ _p_r_o_g_r_a_m_'_s_ _c_o_d_e_ _(_i_._e_._ _m_a_i_n_._p_y_,_ _____i_n_i_t_____._p_y_)
-_a_g_e_n_t_o_p_s_._i_n_i_t_(_)_ _._._._ _#_ _(_o_p_t_i_o_n_a_l_:_ _r_e_c_o_r_d_ _s_p_e_c_i_f_i_c_ _f_u_n_c_t_i_o_n_s_)
-_@_a_g_e_n_t_o_p_s_._r_e_c_o_r_d___f_u_n_c_t_i_o_n_(_'_s_a_m_p_l_e_ _f_u_n_c_t_i_o_n_ _b_e_i_n_g_ _r_e_c_o_r_d_'_)_ _d_e_f_ _s_a_m_p_l_e___f_u_n_c_t_i_o_n
-_(_._._._)_:_ _._._._ _#_ _E_n_d_ _o_f_ _p_r_o_g_r_a_m_ _a_g_e_n_t_o_p_s_._e_n_d___s_e_s_s_i_o_n_(_'_S_u_c_c_e_s_s_'_)_ _#_ _W_o_o_h_o_o_ _Y_o_u_'_r_e
-_d_o_n_e_ _ð____ _`_`_`_ _A_l_l_ _y_o_u_r_ _s_e_s_s_i_o_n_s_ _a_r_e_ _a_v_a_i_l_a_b_l_e_ _o_n_ _t_h_e_ _[_A_g_e_n_t_O_p_s_ _d_a_s_h_b_o_a_r_d_]
-_(_h_t_t_p_s_:_/_/_a_p_p_._a_g_e_n_t_o_p_s_._a_i_?_r_e_f_=_g_h_)_._ _R_e_f_e_r_ _t_o_ _o_u_r_ _[_A_P_I_ _d_o_c_u_m_e_n_t_a_t_i_o_n_]_(_h_t_t_p_:_/_/
-_d_o_c_s_._a_g_e_n_t_o_p_s_._a_i_)_ _f_o_r_ _d_e_t_a_i_l_e_d_ _i_n_s_t_r_u_c_t_i_o_n_s_._ _A_g_e_n_t_ _D_a_s_h_b_o_a_r_d_ _[_A_g_e_n_t
-_D_a_s_h_b_o_a_r_d_]_S_e_s_s_i_o_n_ _A_n_a_l_y_t_i_c_s_ _[_S_e_s_s_i_o_n_ _A_n_a_l_y_t_i_c_s_]_S_e_s_s_i_o_n_ _R_e_p_l_a_y_s_ _[_S_e_s_s_i_o_n
-_R_e_p_l_a_y_s_]_#_#_ _I_n_t_e_g_r_a_t_i_o_n_s_ _ð__¦_¾_ _#_#_#_ _C_r_e_w_A_I_ _ð___¶_ _B_u_i_l_d_ _C_r_e_w_ _a_g_e_n_t_s_ _w_i_t_h
-_o_b_s_e_r_v_a_b_i_l_i_t_y_ _w_i_t_h_ _o_n_l_y_ _2_ _l_i_n_e_s_ _o_f_ _c_o_d_e_._ _S_i_m_p_l_y_ _s_e_t_ _a_n_ _`_A_G_E_N_T_O_P_S___A_P_I___K_E_Y_`_ _i_n
-_y_o_u_r_ _e_n_v_i_r_o_n_m_e_n_t_,_ _a_n_d_ _y_o_u_r_ _c_r_e_w_s_ _w_i_l_l_ _g_e_t_ _a_u_t_o_m_a_t_i_c_ _m_o_n_i_t_o_r_i_n_g_ _o_n_ _t_h_e_ _A_g_e_n_t_O_p_s
-_d_a_s_h_b_o_a_r_d_._ _A_g_e_n_t_O_p_s_ _i_s_ _o_f_f_i_c_i_a_l_l_y_ _s_u_p_p_o_r_t_e_d_ _o_n_ _C_r_e_w_'_s_ _l_a_t_e_s_t_ _r_c_ _b_r_a_n_c_h_:
-_`_c_r_e_w_a_i_=_=_0_._2_8_._9_r_c_1_`_ _*_ _[_A_g_e_n_t_O_p_s_ _i_n_t_e_g_r_a_t_i_o_n_ _e_x_a_m_p_l_e_]_(_h_t_t_p_s_:_/_/_d_o_c_s_._a_g_e_n_t_o_p_s_._a_i_/
-_v_1_/_i_n_t_e_g_r_a_t_i_o_n_s_/_c_r_e_w_a_i_)_ _*_ _[_O_f_f_i_c_a_l_ _C_r_e_w_A_I_ _d_o_c_u_m_e_n_t_a_t_i_o_n_]_(_h_t_t_p_s_:_/_/
-_d_o_c_s_._c_r_e_w_a_i_._c_o_m_/_h_o_w_-_t_o_/_A_g_e_n_t_O_p_s_-_O_b_s_e_r_v_a_b_i_l_i_t_y_)_ _#_#_#_ _L_a_n_g_c_h_a_i_n_ _ð__¦__ð____ _A_g_e_n_t_O_p_s
-_w_o_r_k_s_ _s_e_a_m_l_e_s_s_l_y_ _w_i_t_h_ _a_p_p_l_i_c_a_t_i_o_n_s_ _b_u_i_l_t_ _u_s_i_n_g_ _L_a_n_g_c_h_a_i_n_._ _T_o_ _u_s_e_ _t_h_e_ _h_a_n_d_l_e_r_,
-_i_n_s_t_a_l_l_ _L_a_n_g_c_h_a_i_n_ _a_s_ _a_n_ _o_p_t_i_o_n_a_l_ _d_e_p_e_n_d_e_n_c_y_:_ _`_`_`_s_h_e_l_l_ _p_i_p_ _i_n_s_t_a_l_l_ _a_g_e_n_t_o_p_s
-_[_l_a_n_g_c_h_a_i_n_]_ _`_`_`_ _T_o_ _u_s_e_ _t_h_e_ _h_a_n_d_l_e_r_,_ _i_m_p_o_r_t_ _a_n_d_ _s_e_t_ _`_`_`_p_y_t_h_o_n_ _i_m_p_o_r_t_ _o_s_ _f_r_o_m
-_l_a_n_g_c_h_a_i_n_._c_h_a_t___m_o_d_e_l_s_ _i_m_p_o_r_t_ _C_h_a_t_O_p_e_n_A_I_ _f_r_o_m_ _l_a_n_g_c_h_a_i_n_._a_g_e_n_t_s_ _i_m_p_o_r_t
-_i_n_i_t_i_a_l_i_z_e___a_g_e_n_t_,_ _A_g_e_n_t_T_y_p_e_ _f_r_o_m_ _a_g_e_n_t_o_p_s_._l_a_n_g_c_h_a_i_n___c_a_l_l_b_a_c_k___h_a_n_d_l_e_r_ _i_m_p_o_r_t
-_L_a_n_g_c_h_a_i_n_C_a_l_l_b_a_c_k_H_a_n_d_l_e_r_ _A_G_E_N_T_O_P_S___A_P_I___K_E_Y_ _=_ _o_s_._e_n_v_i_r_o_n_[_'_A_G_E_N_T_O_P_S___A_P_I___K_E_Y_'_]
-_h_a_n_d_l_e_r_ _=_ _L_a_n_g_c_h_a_i_n_C_a_l_l_b_a_c_k_H_a_n_d_l_e_r_(_a_p_i___k_e_y_=_A_G_E_N_T_O_P_S___A_P_I___K_E_Y_,_ _t_a_g_s_=_[_'_L_a_n_g_c_h_a_i_n
-_E_x_a_m_p_l_e_'_]_)_ _l_l_m_ _=_ _C_h_a_t_O_p_e_n_A_I_(_o_p_e_n_a_i___a_p_i___k_e_y_=_O_P_E_N_A_I___A_P_I___K_E_Y_,_ _c_a_l_l_b_a_c_k_s_=_[_h_a_n_d_l_e_r_]_,
-_m_o_d_e_l_=_'_g_p_t_-_3_._5_-_t_u_r_b_o_'_)_ _a_g_e_n_t_ _=_ _i_n_i_t_i_a_l_i_z_e___a_g_e_n_t_(_t_o_o_l_s_,_ _l_l_m_,
-_a_g_e_n_t_=_A_g_e_n_t_T_y_p_e_._C_H_A_T___Z_E_R_O___S_H_O_T___R_E_A_C_T___D_E_S_C_R_I_P_T_I_O_N_,_ _v_e_r_b_o_s_e_=_T_r_u_e_,_ _c_a_l_l_b_a_c_k_s_=
-_[_h_a_n_d_l_e_r_]_,_ _#_ _Y_o_u_ _m_u_s_t_ _p_a_s_s_ _i_n_ _a_ _c_a_l_l_b_a_c_k_ _h_a_n_d_l_e_r_ _t_o_ _r_e_c_o_r_d_ _y_o_u_r_ _a_g_e_n_t
-_h_a_n_d_l_e___p_a_r_s_i_n_g___e_r_r_o_r_s_=_T_r_u_e_)_ _`_`_`_ _C_h_e_c_k_ _o_u_t_ _t_h_e_ _[_L_a_n_g_c_h_a_i_n_ _E_x_a_m_p_l_e_s_ _N_o_t_e_b_o_o_k_]_(_._/
-_e_x_a_m_p_l_e_s_/_l_a_n_g_c_h_a_i_n___e_x_a_m_p_l_e_s_._i_p_y_n_b_)_ _f_o_r_ _m_o_r_e_ _d_e_t_a_i_l_s_ _i_n_c_l_u_d_i_n_g_ _A_s_y_n_c_ _h_a_n_d_l_e_r_s_.
-_#_#_#_ _L_l_a_m_a_I_n_d_e_x_ _ð__¦__ _(_C_o_m_i_n_g_ _S_o_o_n_)_ _#_#_ _T_i_m_e_ _t_r_a_v_e_l_ _d_e_b_u_g_g_i_n_g_ _ð___®_ _(_c_o_m_i_n_g_ _s_o_o_n_!_)
-_#_#_ _A_g_e_n_t_ _A_r_e_n_a_ _ð__¥__ _(_c_o_m_i_n_g_ _s_o_o_n_!_)_ _#_#_ _E_v_a_l_u_a_t_i_o_n_s_ _R_o_a_d_m_a_p_ _ð__§_­_ _|_ _P_l_a_t_f_o_r_m_ _|
-_D_a_s_h_b_o_a_r_d_ _|_ _E_v_a_l_s_ _|_ _|_-_-_-_|_-_-_-_|_-_-_-_|_ _|_â___ _P_y_t_h_o_n_ _S_D_K_ _|_ _â___ _M_u_l_t_i_-_s_e_s_s_i_o_n_ _a_n_d
-_C_r_o_s_s_-_s_e_s_s_i_o_n_ _m_e_t_r_i_c_s_ _|_ _â___ _C_u_s_t_o_m_ _e_v_a_l_ _m_e_t_r_i_c_s_ _|_ _|_ð___§_ _E_v_a_l_u_a_t_i_o_n_ _b_u_i_l_d_e_r_ _A_P_I
-_|_ _â___ _C_u_s_t_o_m_ _e_v_e_n_t_ _t_a_g_ _t_r_a_c_k_i_n_g_Â_ _|_ _ð____ _A_g_e_n_t_ _s_c_o_r_e_c_a_r_d_s_ _|_ _|_â___ _[_J_a_v_a_s_c_r_i_p_t_/
-_T_y_p_e_s_c_r_i_p_t_ _S_D_K_]_(_h_t_t_p_s_:_/_/_g_i_t_h_u_b_._c_o_m_/_A_g_e_n_t_O_p_s_-_A_I_/_a_g_e_n_t_o_p_s_-_n_o_d_e_)_ _|_ _â___ _S_e_s_s_i_o_n
-_r_e_p_l_a_y_s_|_ _ð____ _E_v_a_l_u_a_t_i_o_n_ _p_l_a_y_g_r_o_u_n_d_ _+_ _l_e_a_d_e_r_b_o_a_r_d_|_ _#_#_ _D_e_b_u_g_g_i_n_g_ _R_o_a_d_m_a_p_ _ð__§_­_ _|
-_P_e_r_f_o_r_m_a_n_c_e_ _t_e_s_t_i_n_g_ _|_ _E_n_v_i_r_o_n_m_e_n_t_s_ _|_ _L_L_M_ _T_e_s_t_i_n_g_ _|_ _R_e_a_s_o_n_i_n_g_ _a_n_d_ _e_x_e_c_u_t_i_o_n
-_t_e_s_t_i_n_g_ _|_ _|_-_-_-_|_-_-_-_|_-_-_-_|_-_-_-_|_ _|_â___ _E_v_e_n_t_ _l_a_t_e_n_c_y_ _a_n_a_l_y_s_i_s_ _|_ _ð____ _N_o_n_-_s_t_a_t_i_o_n_a_r_y
-_e_n_v_i_r_o_n_m_e_n_t_ _t_e_s_t_i_n_g_ _|_ _ð____ _L_L_M_ _n_o_n_-_d_e_t_e_r_m_i_n_i_s_t_i_c_ _f_u_n_c_t_i_o_n_ _d_e_t_e_c_t_i_o_n_ _|_ _ð___§
-_I_n_f_i_n_i_t_e_ _l_o_o_p_s_ _a_n_d_ _r_e_c_u_r_s_i_v_e_ _t_h_o_u_g_h_t_ _d_e_t_e_c_t_i_o_n_ _|_ _|_â___ _A_g_e_n_t_ _w_o_r_k_f_l_o_w_ _e_x_e_c_u_t_i_o_n
-_p_r_i_c_i_n_g_ _|_ _ð____ _M_u_l_t_i_-_m_o_d_a_l_ _e_n_v_i_r_o_n_m_e_n_t_s_ _|_ _ð___§_ _T_o_k_e_n_ _l_i_m_i_t_ _o_v_e_r_f_l_o_w_ _f_l_a_g_s_ _|
-_ð____ _F_a_u_l_t_y_ _r_e_a_s_o_n_i_n_g_ _d_e_t_e_c_t_i_o_n_ _|_ _|_ð___§_ _S_u_c_c_e_s_s_ _v_a_l_i_d_a_t_o_r_s_ _(_e_x_t_e_r_n_a_l_)_ _|_ _ð___
-_E_x_e_c_u_t_i_o_n_ _c_o_n_t_a_i_n_e_r_s_ _|_ _ð____ _C_o_n_t_e_x_t_ _l_i_m_i_t_ _o_v_e_r_f_l_o_w_ _f_l_a_g_s_ _|_ _ð____ _G_e_n_e_r_a_t_i_v_e_ _c_o_d_e
-_v_a_l_i_d_a_t_o_r_s_ _|_ _|_ð____ _A_g_e_n_t_ _c_o_n_t_r_o_l_l_e_r_s_/_s_k_i_l_l_ _t_e_s_t_s_ _|_ _â___ _H_o_n_e_y_p_o_t_ _a_n_d_ _p_r_o_m_p_t
-_i_n_j_e_c_t_i_o_n_ _d_e_t_e_c_t_i_o_n_ _(_[_P_r_o_m_p_t_A_r_m_o_r_]_(_h_t_t_p_s_:_/_/_p_r_o_m_p_t_a_r_m_o_r_._c_o_m_)_)_ _|_ _ð____ _A_P_I_ _b_i_l_l
-_t_r_a_c_k_i_n_g_ _|_ _ð____ _E_r_r_o_r_ _b_r_e_a_k_p_o_i_n_t_ _a_n_a_l_y_s_i_s_ _|_ _|_ð____ _I_n_f_o_r_m_a_t_i_o_n_ _c_o_n_t_e_x_t
-_c_o_n_s_t_r_a_i_n_t_ _t_e_s_t_i_n_g_ _|_ _ð____ _A_n_t_i_-_a_g_e_n_t_ _r_o_a_d_b_l_o_c_k_s_ _(_i_._e_._ _C_a_p_t_c_h_a_s_)_ _|_ _ð____ _C_I_/_C_D
-_i_n_t_e_g_r_a_t_i_o_n_ _c_h_e_c_k_s_ _|_ _|_ _|_ð____ _R_e_g_r_e_s_s_i_o_n_ _t_e_s_t_i_n_g_ _|_ _ð____ _M_u_l_t_i_-_a_g_e_n_t_ _f_r_a_m_e_w_o_r_k
-_v_i_s_u_a_l_i_z_a_t_i_o_n_ _|_ _|_ _|_ _#_#_#_ _W_h_y_ _A_g_e_n_t_O_p_s_?_ _ð__¤__ _O_u_r_ _m_i_s_s_i_o_n_ _i_s_ _t_o_ _b_r_i_n_g_ _y_o_u_r_ _a_g_e_n_t
-_f_r_o_m_ _p_r_o_t_o_t_y_p_e_ _t_o_ _p_r_o_d_u_c_t_i_o_n_._ _A_g_e_n_t_ _d_e_v_e_l_o_p_e_r_s_ _o_f_t_e_n_ _w_o_r_k_ _w_i_t_h_ _l_i_t_t_l_e_ _t_o_ _n_o
-_v_i_s_i_b_i_l_i_t_y_ _i_n_t_o_ _a_g_e_n_t_ _t_e_s_t_i_n_g_ _p_e_r_f_o_r_m_a_n_c_e_._ _T_h_i_s_ _m_e_a_n_s_ _t_h_e_i_r_ _a_g_e_n_t_s_ _n_e_v_e_r_ _l_e_a_v_e
-_t_h_e_ _l_a_b_._ _W_e_'_r_e_ _c_h_a_n_g_i_n_g_ _t_h_a_t_._ _A_g_e_n_t_O_p_s_ _i_s_ _t_h_e_ _e_a_s_i_e_s_t_ _w_a_y_ _t_o_ _e_v_a_l_u_a_t_e_,_ _g_r_a_d_e_,
-_a_n_d_ _t_e_s_t_ _a_g_e_n_t_s_._ _I_s_ _t_h_e_r_e_ _a_ _f_e_a_t_u_r_e_ _y_o_u_'_d_ _l_i_k_e_ _t_o_ _s_e_e_ _A_g_e_n_t_O_p_s_ _c_o_v_e_r_?_ _J_u_s_t
-_r_a_i_s_e_ _i_t_ _i_n_ _t_h_e_ _i_s_s_u_e_s_ _t_a_b_,_ _a_n_d_ _w_e_'_l_l_ _w_o_r_k_ _o_n_ _a_d_d_i_n_g_ _i_t_ _t_o_ _t_h_e_ _r_o_a_d_m_a_p_.
+_[_A_g_e_n_t_O_p_s_ _T_w_i_t_t_e_r_]_[_D_i_s_c_o_r_d_ _c_o_m_m_u_n_i_t_y_ _c_h_a_n_n_e_l_]_[_g_i_t_ _c_o_m_m_i_t_ _a_c_t_i_v_i_t_y_]AgentOps
+helps developers build, evaluate, and monitor AI agents. Tools to build agents
+from prototype to production. | | | | ------------------------------------- | -
+------------------------------------------------------------ | | ð **Replay
+Analytics and Debugging** | Step-by-step agent execution graphs | | ð¸ **LLM
+Cost Management** | Track spend with LLM foundation model providers | | ð§ª
+**Agent Benchmarking** | Test your agents against 1,000+ evals | | ð
+**Compliance and Security** | Detect common prompt injection and data
+exfiltration exploits | | ð¤ **Framework Integrations** | Easily plugs in
+with frameworks like CrewAI and LangChain | ## Quick Start â¨ï¸ ```bash pip
+install agentops ``` ### Session replays in 3 lines of code Initialize the
+AgentOps client and automatically get analytics on every LLM call. ```python
+import agentops # Beginning of program's code (i.e. main.py, __init__.py)
+agentops.init() ... # (optional: record specific functions)
+@agentops.record_function('sample function being record') def sample_function
+(...): ... # End of program agentops.end_session('Success') # Woohoo You're
+done ð ``` All your sessions are available on the [AgentOps dashboard]
+(https://app.agentops.ai?ref=gh). Refer to our [API documentation](http://
+docs.agentops.ai) for detailed instructions. Agent Dashboard _[_A_g_e_n_t
+_D_a_s_h_b_o_a_r_d_]Session Analytics _[_S_e_s_s_i_o_n_ _A_n_a_l_y_t_i_c_s_]Session Replays _[_S_e_s_s_i_o_n
+_R_e_p_l_a_y_s_]## Integrations ð¦¾ ### CrewAI ð¶ Build Crew agents with
+observability with only 2 lines of code. Simply set an `AGENTOPS_API_KEY` in
+your environment, and your crews will get automatic monitoring on the AgentOps
+dashboard. AgentOps is integrated with CrewAI on a pre-release fork. Install
+crew with ```bash pip install git+https://github.com/AgentOps-AI/
+crewAI.git@main ``` - [AgentOps integration example](https://docs.agentops.ai/
+v1/integrations/crewai) - [Official CrewAI documentation](https://
+docs.crewai.com/how-to/AgentOps-Observability) ### Langchain ð¦ð AgentOps
+works seamlessly with applications built using Langchain. To use the handler,
+install Langchain as an optional dependency: Installation ```shell pip install
+agentops[langchain] ``` To use the handler, import and set ```python import os
+from langchain.chat_models import ChatOpenAI from langchain.agents import
+initialize_agent, AgentType from agentops.langchain_callback_handler import
+LangchainCallbackHandler AGENTOPS_API_KEY = os.environ['AGENTOPS_API_KEY']
+handler = LangchainCallbackHandler(api_key=AGENTOPS_API_KEY, tags=['Langchain
+Example']) llm = ChatOpenAI(openai_api_key=OPENAI_API_KEY, callbacks=[handler],
+model='gpt-3.5-turbo') agent = initialize_agent(tools, llm,
+agent=AgentType.CHAT_ZERO_SHOT_REACT_DESCRIPTION, verbose=True, callbacks=
+[handler], # You must pass in a callback handler to record your agent
+handle_parsing_errors=True) ``` Check out the [Langchain Examples Notebook](./
+examples/langchain_examples.ipynb) for more details including Async handlers.
+### Cohere â¨ï¸ First class support for Cohere(>=5.4.0). This is a living
+integration, should you need any added functionality please message us on
+Discord! - [AgentOps integration example](https://docs.agentops.ai/v1/
+integrations/cohere) - [Official Cohere documentation](https://docs.cohere.com/
+reference/about) Installation ```bash pip install cohere ``` ```python python
+import cohere import agentops # Beginning of program's code (i.e. main.py,
+__init__.py) agentops.init() co = cohere.Client() chat = co.chat( message="Is
+it pronounced ceaux-hear or co-hehray?" ) print(chat) agentops.end_session
+('Success') ``` ```python python import cohere import agentops # Beginning of
+program's code (i.e. main.py, __init__.py) agentops.init() co = cohere.Client()
+stream = co.chat_stream( message="Write me a haiku about the synergies between
+Cohere and AgentOps" ) for event in stream: if event.event_type == "text-
+generation": print(event.text, end='') agentops.end_session('Success') ``` ###
+LlamaIndex ð¦ (Coming Soon) ## Time travel debugging ð® (coming soon!) ##
+Agent Arena ð¥ (coming soon!) ## Evaluations Roadmap ð§­ | Platform |
+Dashboard | Evals | | ---------------------------------------------------------
+------------------- | ------------------------------------------ | ------------
+-------------------------- | | â Python SDK | â Multi-session and Cross-
+session metrics | â Custom eval metrics | | ð§ Evaluation builder API | â
+Custom event tag trackingÂ  | ð Agent scorecards | | â [Javascript/
+Typescript SDK](https://github.com/AgentOps-AI/agentops-node) | â Session
+replays | ð Evaluation playground + leaderboard | ## Debugging Roadmap ð§­
+| Performance testing | Environments | LLM Testing | Reasoning and execution
+testing | | ----------------------------------------- | -----------------------
+------------------------------------------------------------ | ----------------
+--------------------------- | ------------------------------------------------
+- | | â Event latency analysis | ð Non-stationary environment testing |
+ð LLM non-deterministic function detection | ð§ Infinite loops and
+recursive thought detection | | â Agent workflow execution pricing | ð
+Multi-modal environments | ð§ Token limit overflow flags | ð Faulty
+reasoning detection | | ð§ Success validators (external) | ð Execution
+containers | ð Context limit overflow flags | ð Generative code
+validators | | ð Agent controllers/skill tests | â Honeypot and prompt
+injection detection ([PromptArmor](https://promptarmor.com)) | ð API bill
+tracking | ð Error breakpoint analysis | | ð Information context
+constraint testing | ð Anti-agent roadblocks (i.e. Captchas) | ð CI/CD
+integration checks | | | ð Regression testing | ð Multi-agent framework
+visualization | | | ### Why AgentOps? ð¤ Our mission is to bring your agent
+from prototype to production. Agent developers often work with little to no
+visibility into agent testing performance. This means their agents never leave
+the lab. We're changing that. AgentOps is the easiest way to evaluate, grade,
+and test agents. Is there a feature you'd like to see AgentOps cover? Just
+raise it in the issues tab, and we'll work on adding it to the roadmap.
```

### Comparing `agentops-0.1.9/agentops/__init__.py` & `agentops-0.2.0/agentops/__init__.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,134 +1,161 @@
 # agentops/__init__.py
-from os import environ
+import os
+import logging
 from typing import Optional, List, Union
-
 from .client import Client
 from .config import Configuration
 from .event import Event, ActionEvent, LLMEvent, ToolEvent, ErrorEvent
 from .enums import Models
 from .decorators import record_function
 from .agent import track_agent
-from .log_config import set_logging_level_info, set_logging_level_critial
-from .langchain_callback_handler import LangchainCallbackHandler, AsyncLangchainCallbackHandler
-
+from .log_config import logger
 
-def init(api_key: Optional[str] = None,
-         parent_key: Optional[str] = None,
-         endpoint: Optional[str] = None,
-         max_wait_time: Optional[int] = None,
-         max_queue_size: Optional[int] = None,
-         tags: Optional[List[str]] = None,
-         override: Optional[bool] = None,  # Deprecated
-         instrument_llm_calls=True,
-         auto_start_session=True,
-         inherited_session_id: Optional[str] = None
-         ):
-    """
-        Initializes the AgentOps singleton pattern.
-
-        Args:
-
-            api_key (str, optional): API Key for AgentOps services. If none is provided, key will
-                be read from the AGENTOPS_API_KEY environment variable.
-            parent_key (str, optional): Organization key to give visibility of all user sessions the user's organization. If none is provided, key will
-                be read from the AGENTOPS_PARENT_KEY environment variable.
-            endpoint (str, optional): The endpoint for the AgentOps service. If none is provided, key will
-                be read from the AGENTOPS_API_ENDPOINT environment variable. Defaults to 'https://api.agentops.ai'.
-            max_wait_time (int, optional): The maximum time to wait in milliseconds before flushing the queue.
-                Defaults to 30,000 (30 seconds)
-            max_queue_size (int, optional): The maximum size of the event queue. Defaults to 100.
-            tags (List[str], optional): Tags for the sessions that can be used for grouping or
-                sorting later (e.g. ["GPT-4"]).
-            override (bool, optional): [Deprecated] Use `instrument_llm_calls` instead. Whether to instrument LLM calls and emit LLMEvents..
-            instrument_llm_calls (bool): Whether to instrument LLM calls and emit LLMEvents..
-            auto_start_session (bool): Whether to start a session automatically when the client is created.
-            inherited_session_id (optional, str): Init Agentops with an existing Session
-        Attributes:
-    """
-    set_logging_level_info()
-    c = Client(api_key=api_key,
-               parent_key=parent_key,
-               endpoint=endpoint,
-               max_wait_time=max_wait_time,
-               max_queue_size=max_queue_size,
-               tags=tags,
-               override=override,
-               instrument_llm_calls=instrument_llm_calls,
-               auto_start_session=auto_start_session,
-               inherited_session_id=inherited_session_id
-               )
+try:
+    from .partners.langchain_callback_handler import (
+        LangchainCallbackHandler,
+        AsyncLangchainCallbackHandler,
+    )
+except ModuleNotFoundError:
+    pass
+
+
+def init(
+    api_key: Optional[str] = None,
+    parent_key: Optional[str] = None,
+    endpoint: Optional[str] = None,
+    max_wait_time: Optional[int] = None,
+    max_queue_size: Optional[int] = None,
+    tags: Optional[List[str]] = None,
+    override: Optional[bool] = None,  # Deprecated
+    instrument_llm_calls=True,
+    auto_start_session=True,
+    inherited_session_id: Optional[str] = None,
+):
+    """
+    Initializes the AgentOps singleton pattern.
+
+    Args:
+
+        api_key (str, optional): API Key for AgentOps services. If none is provided, key will
+            be read from the AGENTOPS_API_KEY environment variable.
+        parent_key (str, optional): Organization key to give visibility of all user sessions the user's organization. If none is provided, key will
+            be read from the AGENTOPS_PARENT_KEY environment variable.
+        endpoint (str, optional): The endpoint for the AgentOps service. If none is provided, key will
+            be read from the AGENTOPS_API_ENDPOINT environment variable. Defaults to 'https://api.agentops.ai'.
+        max_wait_time (int, optional): The maximum time to wait in milliseconds before flushing the queue.
+            Defaults to 30,000 (30 seconds)
+        max_queue_size (int, optional): The maximum size of the event queue. Defaults to 100.
+        tags (List[str], optional): Tags for the sessions that can be used for grouping or
+            sorting later (e.g. ["GPT-4"]).
+        override (bool, optional): [Deprecated] Use `instrument_llm_calls` instead. Whether to instrument LLM calls and emit LLMEvents..
+        instrument_llm_calls (bool): Whether to instrument LLM calls and emit LLMEvents..
+        auto_start_session (bool): Whether to start a session automatically when the client is created.
+        inherited_session_id (optional, str): Init Agentops with an existing Session
+    Attributes:
+    """
+    logging_level = os.getenv("AGENTOPS_LOGGING_LEVEL")
+    log_levels = {
+        "CRITICAL": logging.CRITICAL,
+        "ERROR": logging.ERROR,
+        "INFO": logging.INFO,
+        "WARNING": logging.WARNING,
+        "DEBUG": logging.DEBUG,
+    }
+    logger.setLevel(log_levels.get(logging_level or "INFO", "INFO"))
+
+    c = Client(
+        api_key=api_key,
+        parent_key=parent_key,
+        endpoint=endpoint,
+        max_wait_time=max_wait_time,
+        max_queue_size=max_queue_size,
+        tags=tags,
+        override=override,
+        instrument_llm_calls=instrument_llm_calls,
+        auto_start_session=auto_start_session,
+        inherited_session_id=inherited_session_id,
+    )
 
     return inherited_session_id or c.current_session_id
 
 
-def end_session(end_state: str,
-                end_state_reason: Optional[str] = None,
-                video: Optional[str] = None):
-    """
-        End the current session with the AgentOps service.
-
-        Args:
-            end_state (str): The final state of the session. Options: Success, Fail, or Indeterminate.
-            end_state_reason (str, optional): The reason for ending the session.
-            video (str, optional): URL to a video recording of the session
+def end_session(
+    end_state: str, end_state_reason: Optional[str] = None, video: Optional[str] = None
+):
+    """
+    End the current session with the AgentOps service.
+
+    Args:
+        end_state (str): The final state of the session. Options: Success, Fail, or Indeterminate.
+        end_state_reason (str, optional): The reason for ending the session.
+        video (str, optional): URL to a video recording of the session
     """
     Client().end_session(end_state, end_state_reason, video)
 
 
-def start_session(tags: Optional[List[str]] = None, config: Optional[Configuration] = None, inherited_session_id: Optional[str] = None):
-    """
-        Start a new session for recording events.
-
-        Args:
-            tags (List[str], optional): Tags that can be used for grouping or sorting later.
-                e.g. ["test_run"].
-            config: (Configuration, optional): Client configuration object
+def start_session(
+    tags: Optional[List[str]] = None,
+    config: Optional[Configuration] = None,
+    inherited_session_id: Optional[str] = None,
+):
+    """
+    Start a new session for recording events.
+
+    Args:
+        tags (List[str], optional): Tags that can be used for grouping or sorting later.
+            e.g. ["test_run"].
+        config: (Configuration, optional): Client configuration object
     """
     return Client().start_session(tags, config, inherited_session_id)
 
 
 def record(event: Union[Event, ErrorEvent]):
     """
-        Record an event with the AgentOps service.
+    Record an event with the AgentOps service.
 
-        Args:
-            event (Event): The event to record.
+    Args:
+        event (Event): The event to record.
     """
     Client().record(event)
 
 
 def add_tags(tags: List[str]):
     """
-        Append to session tags at runtime. 
+    Append to session tags at runtime.
 
-        Args:
-            tags (List[str]): The list of tags to append.
+    Args:
+        tags (List[str]): The list of tags to append.
     """
     Client().add_tags(tags)
 
 
 def set_tags(tags: List[str]):
     """
-        Replace session tags at runtime. 
+    Replace session tags at runtime.
 
-        Args:
-            tags (List[str]): The list of tags to set.
+    Args:
+        tags (List[str]): The list of tags to set.
     """
     Client().set_tags(tags)
 
 
 def get_api_key() -> str:
     return Client().api_key
 
 
 def set_parent_key(parent_key):
     """
-        Set the parent API key which has visibility to projects it is parent to.
+    Set the parent API key which has visibility to projects it is parent to.
 
-        Args:
-            parent_key (str): The API key of the parent organization to set.
+    Args:
+        parent_key (str): The API key of the parent organization to set.
     """
     Client().set_parent_key(parent_key)
 
+
 def stop_instrumenting():
     Client().stop_instrumenting()
+
+
+def create_agent(name: str, agent_id: Optional[str] = None):
+    return Client().create_agent(name=name, agent_id=agent_id)
```

### Comparing `agentops-0.1.9/agentops/client.py` & `agentops-0.2.0/agentops/client.py`

 * *Files 13% similar despite different names*

```diff
@@ -1,182 +1,248 @@
 """
     AgentOps client module that provides a client class with public interfaces and configuration.
 
     Classes:
         Client: Provides methods to interact with the AgentOps service.
 """
+
 import os
-from .event import ActionEvent, ErrorEvent, Event
-from .enums import EndState
-from .helpers import get_ISO_time, singleton, check_call_stack_for_agent_id
-from .session import Session
-from .worker import Worker
-from .host_env import get_host_env
-from uuid import uuid4
-from typing import Optional, List, Union
-import traceback
-from .log_config import logger, set_logging_level_info
-from decimal import Decimal
 import inspect
 import atexit
 import signal
 import sys
 import threading
+import traceback
+import logging
+from decimal import Decimal
+from uuid import UUID, uuid4
+from typing import Optional, List, Union
 
-
+from .event import ActionEvent, ErrorEvent, Event
+from .enums import EndState
+from .helpers import (
+    get_ISO_time,
+    singleton,
+    check_call_stack_for_agent_id,
+    get_partner_frameworks,
+)
+from .session import Session
+from .worker import Worker
+from .host_env import get_host_env
+from .log_config import logger
 from .meta_client import MetaClient
 from .config import Configuration, ConfigurationError
 from .llm_tracker import LlmTracker
 
 
 @singleton
 class Client(metaclass=MetaClient):
     """
-        Client for AgentOps service.
+    Client for AgentOps service.
 
-        Args:
+    Args:
 
-            api_key (str, optional): API Key for AgentOps services. If none is provided, key will
-                be read from the AGENTOPS_API_KEY environment variable.
-            parent_key (str, optional): Organization key to give visibility of all user sessions the user's organization. If none is provided, key will
-                be read from the AGENTOPS_PARENT_KEY environment variable.
-            endpoint (str, optional): The endpoint for the AgentOps service. If none is provided, key will
-                be read from the AGENTOPS_API_ENDPOINT environment variable. Defaults to 'https://api.agentops.ai'.
-            max_wait_time (int, optional): The maximum time to wait in milliseconds before flushing the queue.
-                Defaults to 30,000 (30 seconds)
-            max_queue_size (int, optional): The maximum size of the event queue. Defaults to 100.
-            tags (List[str], optional): Tags for the sessions that can be used for grouping or
-                sorting later (e.g. ["GPT-4"]).
-            override (bool, optional): [Deprecated] Use `instrument_llm_calls` instead. Whether to instrument LLM calls and emit LLMEvents..
-            instrument_llm_calls (bool): Whether to instrument LLM calls and emit LLMEvents..
-            auto_start_session (bool): Whether to start a session automatically when the client is created.
-            inherited_session_id (optional, str): Init Agentops with an existing Session
-        Attributes:
-            _session (Session, optional): A Session is a grouping of events (e.g. a run of your agent).
-            _worker (Worker, optional): A Worker manages the event queue and sends session updates to the AgentOps api server
+        api_key (str, optional): API Key for AgentOps services. If none is provided, key will
+            be read from the AGENTOPS_API_KEY environment variable.
+        parent_key (str, optional): Organization key to give visibility of all user sessions the user's organization.
+            If none is provided, key will be read from the AGENTOPS_PARENT_KEY environment variable.
+        endpoint (str, optional): The endpoint for the AgentOps service. If none is provided, key will
+            be read from the AGENTOPS_API_ENDPOINT environment variable. Defaults to 'https://api.agentops.ai'.
+        max_wait_time (int, optional): The maximum time to wait in milliseconds before flushing the queue.
+            Defaults to 30,000 (30 seconds)
+        max_queue_size (int, optional): The maximum size of the event queue. Defaults to 100.
+        tags (List[str], optional): Tags for the sessions that can be used for grouping or
+            sorting later (e.g. ["GPT-4"]).
+        override (bool, optional): [Deprecated] Use `instrument_llm_calls` instead. Whether to instrument LLM calls
+            and emit LLMEvents.
+        instrument_llm_calls (bool): Whether to instrument LLM calls and emit LLMEvents..
+        auto_start_session (bool): Whether to start a session automatically when the client is created.
+        inherited_session_id (optional, str): Init Agentops with an existing Session
+    Attributes:
+        _session (Session, optional): A Session is a grouping of events (e.g. a run of your agent).
+        _worker (Worker, optional): A Worker manages the event queue and sends session updates to the AgentOps api
+            server
     """
 
-    def __init__(self,
-                 api_key: Optional[str] = None,
-                 parent_key: Optional[str] = None,
-                 endpoint: Optional[str] = None,
-                 max_wait_time: Optional[int] = None,
-                 max_queue_size: Optional[int] = None,
-                 tags: Optional[List[str]] = None,
-                 override: Optional[bool] = None,  # Deprecated
-                 instrument_llm_calls=True,
-                 auto_start_session=True,
-                 inherited_session_id: Optional[str] = None
-                 ):
+    def __init__(
+        self,
+        api_key: Optional[str] = None,
+        parent_key: Optional[str] = None,
+        endpoint: Optional[str] = None,
+        max_wait_time: Optional[int] = None,
+        max_queue_size: Optional[int] = None,
+        tags: Optional[List[str]] = None,
+        override: Optional[bool] = None,  # Deprecated
+        instrument_llm_calls=True,
+        auto_start_session=True,
+        inherited_session_id: Optional[str] = None,
+    ):
 
         if override is not None:
-            logger.warning("🖇 AgentOps: The 'override' parameter is deprecated. Use 'instrument_llm_calls' instead.",
-                           DeprecationWarning, stacklevel=2)
+            logger.warning(
+                "The 'override' parameter is deprecated. Use 'instrument_llm_calls' instead.",
+                DeprecationWarning,
+                stacklevel=2,
+            )
             instrument_llm_calls = instrument_llm_calls or override
 
         self._session: Optional[Session] = None
         self._worker: Optional[Worker] = None
         self._tags: Optional[List[str]] = tags
         self._tags_for_future_session: Optional[List[str]] = None
 
-        self._env_data_opt_out = os.getenv('AGENTOPS_ENV_DATA_OPT_OUT') and os.getenv(
-            'AGENTOPS_ENV_DATA_OPT_OUT').lower() == 'true'
+        self._env_data_opt_out = (
+            os.environ.get("AGENTOPS_ENV_DATA_OPT_OUT", "False").lower() == "true"
+        )
 
         try:
-            self.config = Configuration(api_key=api_key,
-                                        parent_key=parent_key,
-                                        endpoint=endpoint,
-                                        max_wait_time=max_wait_time,
-                                        max_queue_size=max_queue_size)
+            self.config = Configuration(
+                api_key=api_key,
+                parent_key=parent_key,
+                endpoint=endpoint,
+                max_wait_time=max_wait_time,
+                max_queue_size=max_queue_size,
+            )
+
+            if inherited_session_id is not None:
+                # Check if inherited_session_id is valid
+                UUID(inherited_session_id)
+
         except ConfigurationError:
             return
 
         self._handle_unclean_exits()
 
+        instrument_llm_calls, auto_start_session = self._check_for_partner_frameworks(
+            instrument_llm_calls, auto_start_session
+        )
+
         if auto_start_session:
             self.start_session(tags, self.config, inherited_session_id)
         else:
             self._tags_for_future_session = tags
 
         if instrument_llm_calls:
             self.llm_tracker = LlmTracker(self)
             self.llm_tracker.override_api()
 
+    def _check_for_partner_frameworks(
+        self, instrument_llm_calls, auto_start_session
+    ) -> tuple[bool, bool]:
+        partner_frameworks = get_partner_frameworks()
+        for framework in partner_frameworks.keys():
+            if framework in sys.modules:
+                self.add_tags([framework])
+                if framework == "autogen":
+                    try:
+                        import autogen
+                        from .partners.autogen_logger import AutogenLogger
+
+                        autogen.runtime_logging.start(logger=AutogenLogger())
+                    except ImportError:
+                        pass
+                    except Exception as e:
+                        logger.warning(
+                            f"Failed to set up AutoGen logger with AgentOps. Error: {e}"
+                        )
+
+                    return partner_frameworks[framework]
+
+        return instrument_llm_calls, auto_start_session
+
     def add_tags(self, tags: List[str]):
         """
-            Append to session tags at runtime.
+        Append to session tags at runtime.
 
-            Args:
-                tags (List[str]): The list of tags to append.
+        Args:
+            tags (List[str]): The list of tags to append.
         """
-        if self._session.tags is not None:
-            for tag in tags:
-                if tag not in self._session.tags:
-                    self._session.tags.append(tag)
-        else:
-            self._session.tags = tags
 
-        if self._session is not None and self._worker is not None:
-            self._worker.update_session(self._session)
+        if self._session:
+            if self._session.tags is not None:
+                for tag in tags:
+                    if tag not in self._session.tags:
+                        self._session.tags.append(tag)
+            else:
+                self._session.tags = tags
+
+            if self._session is not None and self._worker is not None:
+                self._worker.update_session(self._session)
+
+        else:
+            if self._tags_for_future_session:
+                for tag in tags:
+                    if tag not in self._tags_for_future_session:
+                        self._tags_for_future_session.append(tag)
+            else:
+                self._tags_for_future_session = tags
 
     def set_tags(self, tags: List[str]):
         """
-            Replace session tags at runtime.
+        Replace session tags at runtime.
 
-            Args:
-                tags (List[str]): The list of tags to set.
+        Args:
+            tags (List[str]): The list of tags to set.
         """
         self._tags_for_future_session = tags
 
         if self._session is not None and self._worker is not None:
             self._session.tags = tags
             self._worker.update_session(self._session)
 
     def record(self, event: Union[Event, ErrorEvent]):
         """
-            Record an event with the AgentOps service.
+        Record an event with the AgentOps service.
 
-            Args:
-                event (Event): The event to record.
+        Args:
+            event (Event): The event to record.
         """
-        if self._session is None or self._session.has_ended:
-            logger.warning("🖇 AgentOps: Cannot record event - no current session")
+        if self._session is None or self._session.has_ended or self._worker is None:
+            logger.warning("Cannot record event - no current session")
             return
 
         if isinstance(event, Event):
             if not event.end_timestamp or event.init_timestamp == event.end_timestamp:
                 event.end_timestamp = get_ISO_time()
         elif isinstance(event, ErrorEvent):
             if event.trigger_event:
-                if not event.trigger_event.end_timestamp or event.trigger_event.init_timestamp == event.trigger_event.end_timestamp:
+                if (
+                    not event.trigger_event.end_timestamp
+                    or event.trigger_event.init_timestamp
+                    == event.trigger_event.end_timestamp
+                ):
                     event.trigger_event.end_timestamp = get_ISO_time()
 
-            event.trigger_event_id = event.trigger_event.id
-            event.trigger_event_type = event.trigger_event.event_type
-            self._worker.add_event(event.trigger_event.__dict__)
-            event.trigger_event = None  # removes trigger_event from serialization
+                event.trigger_event_id = event.trigger_event.id
+                event.trigger_event_type = event.trigger_event.event_type
+                self._worker.add_event(event.trigger_event.__dict__)
+                event.trigger_event = None  # removes trigger_event from serialization
 
         self._worker.add_event(event.__dict__)
 
     def _record_event_sync(self, func, event_name, *args, **kwargs):
         init_time = get_ISO_time()
         func_args = inspect.signature(func).parameters
         arg_names = list(func_args.keys())
         # Get default values
-        arg_values = {name: func_args[name].default
-                      for name in arg_names if func_args[name].default
-                      is not inspect._empty}
+        arg_values = {
+            name: func_args[name].default
+            for name in arg_names
+            if func_args[name].default is not inspect._empty
+        }
         # Update with positional arguments
         arg_values.update(dict(zip(arg_names, args)))
         arg_values.update(kwargs)
 
-        event = ActionEvent(params=arg_values,
-                            init_timestamp=init_time,
-                            agent_id=check_call_stack_for_agent_id(),
-                            action_type=event_name)
+        event = ActionEvent(
+            params=arg_values,
+            init_timestamp=init_time,
+            agent_id=check_call_stack_for_agent_id(),
+            action_type=event_name,
+        )
 
         try:
             returns = func(*args, **kwargs)
 
             # If the function returns multiple values, record them all in the same event
             if isinstance(returns, tuple):
                 returns = list(returns)
@@ -194,25 +260,29 @@
         return returns
 
     async def _record_event_async(self, func, event_name, *args, **kwargs):
         init_time = get_ISO_time()
         func_args = inspect.signature(func).parameters
         arg_names = list(func_args.keys())
         # Get default values
-        arg_values = {name: func_args[name].default
-                      for name in arg_names if func_args[name].default
-                      is not inspect._empty}
+        arg_values = {
+            name: func_args[name].default
+            for name in arg_names
+            if func_args[name].default is not inspect._empty
+        }
         # Update with positional arguments
         arg_values.update(dict(zip(arg_names, args)))
         arg_values.update(kwargs)
 
-        event = ActionEvent(params=arg_values,
-                            init_timestamp=init_time,
-                            agent_id=check_call_stack_for_agent_id(),
-                            action_type=event_name)
+        event = ActionEvent(
+            params=arg_values,
+            init_timestamp=init_time,
+            agent_id=check_call_stack_for_agent_id(),
+            action_type=event_name,
+        )
 
         try:
             returns = await func(*args, **kwargs)
 
             # If the function returns multiple values, record them all in the same event
             if isinstance(returns, tuple):
                 returns = list(returns)
@@ -225,148 +295,201 @@
             self.record(ErrorEvent(trigger_event=event, exception=e))
 
             # Re-raise the exception
             raise
 
         return returns
 
-    def start_session(self, tags: Optional[List[str]] = None, config: Optional[Configuration] = None, inherited_session_id: Optional[str] = None):
+    def start_session(
+        self,
+        tags: Optional[List[str]] = None,
+        config: Optional[Configuration] = None,
+        inherited_session_id: Optional[str] = None,
+    ):
         """
-            Start a new session for recording events.
+        Start a new session for recording events.
 
-            Args:
-                tags (List[str], optional): Tags that can be used for grouping or sorting later.
-                    e.g. ["test_run"].
-                config: (Configuration, optional): Client configuration object
-                inherited_session_id (optional, str): assign session id to match existing Session
-        """
-        set_logging_level_info()
+        Args:
+            tags (List[str], optional): Tags that can be used for grouping or sorting later.
+                e.g. ["test_run"].
+            config: (Configuration, optional): Client configuration object
+            inherited_session_id (optional, str): assign session id to match existing Session
+        """
+        logging_level = os.getenv("AGENTOPS_LOGGING_LEVEL")
+        log_levels = {
+            "CRITICAL": logging.CRITICAL,
+            "ERROR": logging.ERROR,
+            "INFO": logging.INFO,
+            "WARNING": logging.WARNING,
+            "DEBUG": logging.DEBUG,
+        }
+        logger.setLevel(log_levels.get(logging_level or "INFO", "INFO"))
 
         if self._session is not None:
-            return logger.warning("🖇 AgentOps: Cannot start session - session already started")
+            return logger.warning("Cannot start session - session already started")
 
         if not config and not self.config:
-            return logger.warning("🖇 AgentOps: Cannot start session - missing configuration")
+            return logger.warning("Cannot start session - missing configuration")
 
-        self._session = Session(inherited_session_id or uuid4(),
-                                tags or self._tags_for_future_session, host_env=get_host_env(self._env_data_opt_out))
+        session_id = (
+            UUID(inherited_session_id) if inherited_session_id is not None else uuid4()
+        )
+
+        self._session = Session(
+            session_id=session_id,
+            tags=tags or self._tags_for_future_session,
+            host_env=get_host_env(self._env_data_opt_out),
+        )
         self._worker = Worker(config or self.config)
-        start_session_result = self._worker.start_session(self._session)
+
+        start_session_result = False
+        if inherited_session_id is not None:
+            start_session_result = self._worker.reauthorize_jwt(self._session)
+        else:
+            start_session_result = self._worker.start_session(self._session)
+
         if not start_session_result:
             self._session = None
-            return logger.warning("🖇 AgentOps: Cannot start session")
+            return logger.warning("Cannot start session - server rejected session")
 
-        logger.info('View info on this session at https://app.agentops.ai/drilldown?session_id=%s', 
-                    self._session.session_id)
+        logger.info(
+            f"\x1b[34mSession Replay: https://app.agentops.ai/drilldown?session_id={self._session.session_id}\x1b[0m"
+        )
 
         return self._session.session_id
 
-    def end_session(self,
-                    end_state: str,
-                    end_state_reason: Optional[str] = None,
-                    video: Optional[str] = None):
+    def end_session(
+        self,
+        end_state: str,
+        end_state_reason: Optional[str] = None,
+        video: Optional[str] = None,
+    ):
         """
-            End the current session with the AgentOps service.
+        End the current session with the AgentOps service.
 
-            Args:
-                end_state (str): The final state of the session. Options: Success, Fail, or Indeterminate.
-                end_state_reason (str, optional): The reason for ending the session.
-                video (str, optional): The video screen recording of the session
+        Args:
+            end_state (str): The final state of the session. Options: Success, Fail, or Indeterminate.
+            end_state_reason (str, optional): The reason for ending the session.
+            video (str, optional): The video screen recording of the session
         """
+
         if self._session is None or self._session.has_ended:
-            return logger.warning("🖇 AgentOps: Cannot end session - no current session")
+            return logger.warning("Cannot end session - no current session")
 
         if not any(end_state == state.value for state in EndState):
-            return logger.warning("🖇 AgentOps: Invalid end_state. Please use one of the EndState enums")
-        
+            return logger.warning(
+                "Invalid end_state. Please use one of the EndState enums"
+            )
+
         if self._worker is None or self._worker._session is None:
-            return logger.warning("🖇 AgentOps: Cannot end session - no current worker or session")
+            return logger.warning("Cannot end session - no current worker or session")
 
         self._session.video = video
         self._session.end_session(end_state, end_state_reason)
         token_cost = self._worker.end_session(self._session)
-        
-        if token_cost == 'unknown':
-            print('🖇 AgentOps: Could not determine cost of run.')
+
+        if token_cost == "unknown":
+            logger.info("Could not determine cost of run.")
         else:
             token_cost_d = Decimal(token_cost)
-            print('🖇 AgentOps: This run cost ${}'.format('{:.2f}'.format(
-                token_cost_d) if token_cost_d == 0 else '{:.6f}'.format(token_cost_d)))
+            logger.info(
+                "This run's cost ${}".format(
+                    "{:.2f}".format(token_cost_d)
+                    if token_cost_d == 0
+                    else "{:.6f}".format(token_cost_d)
+                )
+            )
+
+        logger.info(
+            f"\x1b[34mSession Replay: https://app.agentops.ai/drilldown?session_id={self._session.session_id}\x1b[0m"
+        )
+
         self._session = None
         self._worker = None
 
-    def create_agent(self, agent_id: str, name: str):
+    def create_agent(self, name: str, agent_id: Optional[str] = None):
+        if agent_id is None:
+            agent_id = str(uuid4())
         if self._worker:
-            self._worker.create_agent(agent_id, name)
+            self._worker.create_agent(name=name, agent_id=agent_id)
+            return agent_id
 
     def _handle_unclean_exits(self):
-        def cleanup(end_state: str = 'Fail', end_state_reason: Optional[str] = None):
+        def cleanup(end_state: str = "Fail", end_state_reason: Optional[str] = None):
             # Only run cleanup function if session is created
             if self._session is not None:
-                self.end_session(end_state=end_state,
-                                 end_state_reason=end_state_reason)
+                self.end_session(end_state=end_state, end_state_reason=end_state_reason)
 
         def signal_handler(signum, frame):
             """
-                Signal handler for SIGINT (Ctrl+C) and SIGTERM. Ends the session and exits the program.
+            Signal handler for SIGINT (Ctrl+C) and SIGTERM. Ends the session and exits the program.
 
-                Args:
-                    signum (int): The signal number.
-                    frame: The current stack frame.
+            Args:
+                signum (int): The signal number.
+                frame: The current stack frame.
             """
-            signal_name = 'SIGINT' if signum == signal.SIGINT else 'SIGTERM'
-            logger.info('🖇 AgentOps: %s detected. Ending session...', signal_name)
-            self.end_session(end_state='Fail',
-                             end_state_reason=f'Signal {signal_name} detected')
+            signal_name = "SIGINT" if signum == signal.SIGINT else "SIGTERM"
+            logger.info("%s detected. Ending session...", signal_name)
+            self.end_session(
+                end_state="Fail", end_state_reason=f"Signal {signal_name} detected"
+            )
             sys.exit(0)
 
         def handle_exception(exc_type, exc_value, exc_traceback):
             """
-                Handle uncaught exceptions before they result in program termination.
+            Handle uncaught exceptions before they result in program termination.
 
-                Args:
-                    exc_type (Type[BaseException]): The type of the exception.
-                    exc_value (BaseException): The exception instance.
-                    exc_traceback (TracebackType): A traceback object encapsulating the call stack at the
-                                                point where the exception originally occurred.
+            Args:
+                exc_type (Type[BaseException]): The type of the exception.
+                exc_value (BaseException): The exception instance.
+                exc_traceback (TracebackType): A traceback object encapsulating the call stack at the
+                                            point where the exception originally occurred.
             """
-            formatted_traceback = ''.join(traceback.format_exception(exc_type, exc_value,
-                                                                     exc_traceback))
-
-            self.end_session(end_state='Fail',
-                             end_state_reason=f"{str(exc_value)}: {formatted_traceback}")
+            formatted_traceback = "".join(
+                traceback.format_exception(exc_type, exc_value, exc_traceback)
+            )
+
+            self.end_session(
+                end_state="Fail",
+                end_state_reason=f"{str(exc_value)}: {formatted_traceback}",
+            )
 
             # Then call the default excepthook to exit the program
             sys.__excepthook__(exc_type, exc_value, exc_traceback)
 
         # if main thread
-        if isinstance(threading.current_thread(), threading._MainThread):
-            atexit.register(lambda: cleanup(end_state="Indeterminate",
-                            end_state_reason="Process exited without calling end_session()"))
+        if threading.current_thread() is threading.main_thread():
+            atexit.register(
+                lambda: cleanup(
+                    end_state="Indeterminate",
+                    end_state_reason="Process exited without calling end_session()",
+                )
+            )
             signal.signal(signal.SIGINT, signal_handler)
             signal.signal(signal.SIGTERM, signal_handler)
             sys.excepthook = handle_exception
 
     @property
     def current_session_id(self):
         return self._session.session_id if self._session else None
 
     @property
     def api_key(self):
         return self.config.api_key
 
     def set_parent_key(self, parent_key: str):
         """
-            Set the parent API key which has visibility to projects it is parent to.
+        Set the parent API key which has visibility to projects it is parent to.
 
-            Args:
-                parent_key (str): The API key of the parent organization to set.
+        Args:
+            parent_key (str): The API key of the parent organization to set.
         """
         if self._worker:
             self._worker.config.parent_key = parent_key
 
     @property
     def parent_key(self):
         return self.config.parent_key
 
     def stop_instrumenting(self):
-        self.llm_tracker.stop_instrumenting()
+        if self.llm_tracker:
+            self.llm_tracker.stop_instrumenting()
```

#### encoding

```diff
@@ -1 +1 @@
-utf-8
+us-ascii
```

### Comparing `agentops-0.1.9/agentops/config.py` & `agentops-0.2.0/agentops/config.py`

 * *Files 4% similar despite different names*

```diff
@@ -11,45 +11,49 @@
 
 
 class Configuration:
     """
     Stores the configuration settings for AgentOps clients.
 
     Args:
-        api_key (str, optional): API Key for AgentOps services. If none is provided, key will 
+        api_key (str, optional): API Key for AgentOps services. If none is provided, key will
             be read from the AGENTOPS_API_KEY environment variable.
-        parent_key (str, optional): Organization key to give visibility of all user sessions the user's organization. If none is provided, key will 
+        parent_key (str, optional): Organization key to give visibility of all user sessions the user's organization. If none is provided, key will
             be read from the AGENTOPS_PARENT_KEY environment variable.
-        endpoint (str, optional): The endpoint for the AgentOps service. If none is provided, key will 
+        endpoint (str, optional): The endpoint for the AgentOps service. If none is provided, key will
             be read from the AGENTOPS_API_ENDPOINT environment variable. Defaults to 'https://api.agentops.ai'.
-        max_wait_time (int, optional): The maximum time to wait in milliseconds before flushing the queue. Defaults to 30000.
+        max_wait_time (int, optional): The maximum time to wait in milliseconds before flushing the queue. Defaults to 5000.
         max_queue_size (int, optional): The maximum size of the event queue. Defaults to 100.
     """
 
-    def __init__(self,
-                 api_key: Optional[str] = None,
-                 parent_key: Optional[str] = None,
-                 endpoint: Optional[str] = None,
-                 max_wait_time: Optional[int] = None,
-                 max_queue_size: Optional[int] = None):
+    def __init__(
+        self,
+        api_key: Optional[str] = None,
+        parent_key: Optional[str] = None,
+        endpoint: Optional[str] = None,
+        max_wait_time: Optional[int] = None,
+        max_queue_size: Optional[int] = None,
+    ):
 
         if not api_key:
-            api_key = environ.get('AGENTOPS_API_KEY', None)
+            api_key = environ.get("AGENTOPS_API_KEY", None)
             if not api_key:
-                raise ConfigurationError("🖇 AgentOps: No API key provided - no data will be recorded.")
+                raise ConfigurationError(
+                    "No API key provided - no data will be recorded."
+                )
 
         if not parent_key:
-            parent_key = environ.get('AGENTOPS_PARENT_KEY', None)
+            parent_key = environ.get("AGENTOPS_PARENT_KEY", None)
 
         if not endpoint:
-            endpoint = environ.get('AGENTOPS_API_ENDPOINT', 'https://api.agentops.ai')
+            endpoint = environ.get("AGENTOPS_API_ENDPOINT", "https://api.agentops.ai")
 
         self._api_key: str = api_key
         self._endpoint = endpoint
-        self._max_wait_time = max_wait_time or 30000
+        self._max_wait_time = max_wait_time or 5000
         self._max_queue_size = max_queue_size or 100
         self._parent_key: Optional[str] = parent_key
 
     @property
     def api_key(self) -> str:
         """
         Get the API Key for AgentOps services.
@@ -73,15 +77,15 @@
     def endpoint(self) -> str:
         """
         Get the endpoint for the AgentOps service.
 
         Returns:
             str: The endpoint for the AgentOps service.
         """
-        return self._endpoint
+        return self._endpoint  # type: ignore
 
     @endpoint.setter
     def endpoint(self, value: str):
         """
         Set the endpoint for the AgentOps service.
 
         Args:
```

#### encoding

```diff
@@ -1 +1 @@
-utf-8
+us-ascii
```

### Comparing `agentops-0.1.9/agentops/decorators.py` & `agentops-0.2.0/agentops/decorators.py`

 * *Files 9% similar despite different names*

```diff
@@ -14,20 +14,24 @@
     Args:
             event_name (str): The name of the event to record.
     """
 
     def decorator(func):
 
         if inspect.iscoroutinefunction(func):
+
             @functools.wraps(func)
             async def async_wrapper(*args, **kwargs):
-                return await Client()._record_event_async(func, event_name, *args, **kwargs)
+                return await Client()._record_event_async(
+                    func, event_name, *args, **kwargs
+                )
 
             return async_wrapper
         else:
+
             @functools.wraps(func)
             def sync_wrapper(*args, **kwargs):
                 return Client()._record_event_sync(func, event_name, *args, **kwargs)
 
             return sync_wrapper
 
     return decorator
```

### Comparing `agentops-0.1.9/agentops/enums.py` & `agentops-0.2.0/agentops/enums.py`

 * *Files identical despite different names*

### Comparing `agentops-0.1.9/agentops/event.py` & `agentops-0.2.0/agentops/event.py`

 * *Files 1% similar despite different names*

```diff
@@ -11,15 +11,14 @@
 from .enums import EventType, Models
 from uuid import UUID, uuid4
 import traceback
 
 
 @dataclass
 class Event:
-
     """
     Abstract base class for events that will be recorded. Should not be instantiated directly.
 
     event_type(str): The type of event. Defined in enums.EventType. Some values are 'llm', 'action', 'api', 'tool', 'error'.
     params(dict, optional): The parameters of the function containing the triggered event, e.g. {'x': 1} in example below
     returns(str, optional): The return value of the function containing the triggered event, e.g. 2 in example below
     init_timestamp(str): A timestamp indicating when the event began. Defaults to the time when this Event was instantiated.
@@ -33,17 +32,17 @@
         record(ActionEvent(params=**kwargs, ...))
         ...
         // returns equals 2
         return x+1
     }
     """
 
-    event_type: str  # EventType.ENUM.value
+    event_type: EventType
     params: Optional[dict] = None
-    returns: Optional[str] = None
+    returns: Optional[str | List[str]] = None
     init_timestamp: str = field(default_factory=get_ISO_time)
     end_timestamp: Optional[str] = None
     agent_id: Optional[UUID] = field(default_factory=check_call_stack_for_agent_id)
     id: UUID = field(default_factory=uuid4)
 
 
 @dataclass
@@ -61,15 +60,14 @@
     action_type: Optional[str] = None
     logs: Optional[Union[str, Sequence[Any]]] = None
     screenshot: Optional[str] = None
 
 
 @dataclass
 class LLMEvent(Event):
-
     """
     For recording calls to LLMs. AgentOps auto-instruments calls to the most popular LLMs e.g. GPT, Claude, Gemini, etc.
 
     thread_id(UUID, optional): The unique identifier of the contextual thread that a message pertains to.
     prompt(str, list, optional): The message or messages that were used to prompt the LLM. Preferably in ChatML format which is more fully supported by AgentOps.
     prompt_tokens(int, optional): The number of tokens in the prompt message.
     completion(str, object, optional): The message or returned by the LLM. Preferably in ChatML format which is more fully supported by AgentOps.
@@ -92,24 +90,25 @@
     """
     For recording calls to tools e.g. searchWeb, fetchFromDB
 
     name(str, optional): A name describing the tool or the actual function name if applicable e.g. searchWeb, fetchFromDB.
     logs(str, dict, optional): For detailed information/logging related to the tool.
 
     """
+
     event_type: str = EventType.TOOL.value
     name: Optional[str] = None
     logs: Optional[Union[str, dict]] = None
 
+
 # Does not inherit from Event because error will (optionally) be linked to an ActionEvent, LLMEvent, etc that will have the details
 
 
 @dataclass
-class ErrorEvent():
-
+class ErrorEvent:
     """
     For recording any errors e.g. ones related to agent execution
 
     trigger_event(Event, optional): The event object that triggered the error if applicable.
     exception(BaseException, optional): The thrown exception. We will automatically parse the error_type and details from this.
     error_type(str, optional): The type of error e.g. "ValueError".
     code(str, optional): A code that can be used to identify the error e.g. 501.
```

### Comparing `agentops-0.1.9/agentops/helpers.py` & `agentops-0.2.0/agentops/helpers.py`

 * *Files 10% similar despite different names*

```diff
@@ -8,14 +8,21 @@
 
 from .log_config import logger
 from uuid import UUID
 import os
 from importlib.metadata import version
 
 
+PARTNER_FRAMEWORKS = {
+    # framework : instrument_llm_calls, auto_start_session
+    "autogen": (False, True),
+    "crewai": (False, True),
+}
+
+
 def singleton(class_):
     instances = {}
 
     def getinstance(*args, **kwargs):
         if class_ not in instances:
             instances[class_] = class_(*args, **kwargs)
         return instances[class_]
@@ -26,45 +33,61 @@
 def get_ISO_time():
     """
     Get the current UTC time in ISO 8601 format with milliseconds precision, suffixed with 'Z' to denote UTC timezone.
 
     Returns:
         str: The current UTC time as a string in ISO 8601 format.
     """
-    return datetime.utcfromtimestamp(time.time()).isoformat(timespec='milliseconds') + 'Z'
+    return (
+        datetime.utcfromtimestamp(time.time()).isoformat(timespec="milliseconds") + "Z"
+    )
 
 
 def is_jsonable(x):
     try:
         json.dumps(x)
         return True
     except (TypeError, OverflowError):
         return False
 
 
 def filter_unjsonable(d: dict) -> dict:
     def filter_dict(obj):
         if isinstance(obj, dict):
             # TODO: clean up this mess lol
-            return {k: filter_dict(v) if isinstance(v, (dict, list)) or is_jsonable(v) else str(v) if isinstance(v, UUID) else "" for k, v in obj.items()}
+            return {
+                k: (
+                    filter_dict(v)
+                    if isinstance(v, (dict, list)) or is_jsonable(v)
+                    else str(v) if isinstance(v, UUID) else ""
+                )
+                for k, v in obj.items()
+            }
         elif isinstance(obj, list):
-            return [filter_dict(x) if isinstance(x, (dict, list)) or is_jsonable(x) else str(x) if isinstance(x, UUID) else "" for x in obj]
+            return [
+                (
+                    filter_dict(x)
+                    if isinstance(x, (dict, list)) or is_jsonable(x)
+                    else str(x) if isinstance(x, UUID) else ""
+                )
+                for x in obj
+            ]
         else:
             return obj if is_jsonable(obj) or isinstance(obj, UUID) else ""
 
     return filter_dict(d)
 
 
 def safe_serialize(obj):
     def default(o):
         if isinstance(o, UUID):
             return str(o)
-        elif hasattr(o, 'model_dump_json'):
+        elif hasattr(o, "model_dump_json"):
             return o.model_dump_json()
-        elif hasattr(o, 'to_json'):
+        elif hasattr(o, "to_json"):
             return o.to_json()
         else:
             return f"<<non-serializable: {type(o).__qualname__}>>"
 
     def remove_none_values(value):
         """Recursively remove keys with None values from dictionaries."""
         if isinstance(value, dict):
@@ -82,59 +105,69 @@
     for frame_info in inspect.stack():
         # Look through the call stack for the class that called the LLM
         local_vars = frame_info.frame.f_locals
         for var in local_vars.values():
             # We stop looking up the stack at main because after that we see global variables
             if var == "__main__":
                 return None
-            if hasattr(var, 'agent_ops_agent_id') and getattr(var, 'agent_ops_agent_id'):
-                logger.debug('LLM call from agent named: %s', getattr(var, 'agent_ops_agent_name'))
-                return getattr(var, 'agent_ops_agent_id')
+            if hasattr(var, "agent_ops_agent_id") and getattr(
+                var, "agent_ops_agent_id"
+            ):
+                logger.debug(
+                    "LLM call from agent named: %s",
+                    getattr(var, "agent_ops_agent_name"),
+                )
+                return getattr(var, "agent_ops_agent_id")
     return None
 
 
 def get_agentops_version():
     try:
         pkg_version = version("agentops")
         return pkg_version
     except Exception as e:
-        logger.warning('Error reading package version: %s', e)
+        logger.warning("Error reading package version: %s", e)
         return None
 
 
 # Function decorator that prints function name and its arguments to the console for debug purposes
 # Example output:
-    # <AGENTOPS_DEBUG_OUTPUT>
-    # on_llm_start called with arguments:
-    # run_id: UUID('5fda42fe-809b-4179-bad2-321d1a6090c7')
-    # parent_run_id: UUID('63f1c4da-3e9f-4033-94d0-b3ebed06668f')
-    # tags: []
-    # metadata: {}
-    # invocation_params: {'_type': 'openai-chat',
-    # 'model': 'gpt-3.5-turbo',
-    # 'model_name': 'gpt-3.5-turbo',
-    # 'n': 1,
-    # 'stop': ['Observation:'],
-    # 'stream': False,
-    # 'temperature': 0.7}
-    # options: {'stop': ['Observation:']}
-    # name: None
-    # batch_size: 1
-    # </AGENTOPS_DEBUG_OUTPUT>
+# <AGENTOPS_DEBUG_OUTPUT>
+# on_llm_start called with arguments:
+# run_id: UUID('5fda42fe-809b-4179-bad2-321d1a6090c7')
+# parent_run_id: UUID('63f1c4da-3e9f-4033-94d0-b3ebed06668f')
+# tags: []
+# metadata: {}
+# invocation_params: {'_type': 'openai-chat',
+# 'model': 'gpt-3.5-turbo',
+# 'model_name': 'gpt-3.5-turbo',
+# 'n': 1,
+# 'stop': ['Observation:'],
+# 'stream': False,
+# 'temperature': 0.7}
+# options: {'stop': ['Observation:']}
+# name: None
+# batch_size: 1
+# </AGENTOPS_DEBUG_OUTPUT>
 
 # regex to filter for just this:
 # <AGENTOPS_DEBUG_OUTPUT>([\s\S]*?)<\/AGENTOPS_DEBUG_OUTPUT>\n
 
+
 def debug_print_function_params(func):
     @wraps(func)
     def wrapper(self, *args, **kwargs):
-        if os.getenv('DEBUG_MODE') == 'Y':
-            print("\n<AGENTOPS_DEBUG_OUTPUT>")
-            print(f"{func.__name__} called with arguments:")
+        logger.debug("\n<AGENTOPS_DEBUG_OUTPUT>")
+        logger.debug(f"{func.__name__} called with arguments:")
 
-            for key, value in kwargs.items():
-                print(f"{key}: {pformat(value)}")
+        for key, value in kwargs.items():
+            logger.debug(f"{key}: {pformat(value)}")
 
-            print("</AGENTOPS_DEBUG_OUTPUT>\n")
+        logger.debug("</AGENTOPS_DEBUG_OUTPUT>\n")
 
         return func(self, *args, **kwargs)
+
     return wrapper
+
+
+def get_partner_frameworks():
+    return PARTNER_FRAMEWORKS
```

### Comparing `agentops-0.1.9/agentops/http_client.py` & `agentops-0.2.0/agentops/http_client.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,17 +1,14 @@
 from enum import Enum
 from typing import Optional
 from .log_config import logger
 import requests
 from requests.adapters import Retry, HTTPAdapter
 
-JSON_HEADER = {
-    "Content-Type": "application/json; charset=UTF-8",
-    "Accept": "*/*"
-}
+JSON_HEADER = {"Content-Type": "application/json; charset=UTF-8", "Accept": "*/*"}
 
 retry_config = Retry(total=5, backoff_factor=0.1)
 
 
 class HttpStatus(Enum):
     SUCCESS = 200
     INVALID_REQUEST = 400
@@ -21,15 +18,17 @@
     TOO_MANY_REQUESTS = 429
     FAILED = 500
     UNKNOWN = -1
 
 
 class Response:
 
-    def __init__(self, status: HttpStatus = HttpStatus.UNKNOWN, body: Optional[dict] = None):
+    def __init__(
+        self, status: HttpStatus = HttpStatus.UNKNOWN, body: Optional[dict] = None
+    ):
         self.status: HttpStatus = status
         self.code: int = status.value
         self.body = body if body else {}
 
     def parse(self, res: requests.models.Response):
         res_body = res.json()
         self.code = res.status_code
@@ -55,51 +54,60 @@
             return HttpStatus.FAILED
         return HttpStatus.UNKNOWN
 
 
 class HttpClient:
 
     @staticmethod
-    def post(url: str, payload: bytes, api_key: Optional[str] = None, parent_key: Optional[str] = None,
-             header=None) -> Response:
+    def post(
+        url: str,
+        payload: bytes,
+        api_key: Optional[str] = None,
+        parent_key: Optional[str] = None,
+        jwt: Optional[str] = None,
+        header=None,
+    ) -> Response:
         result = Response()
         try:
             # Create request session with retries configured
             request_session = requests.Session()
             request_session.mount(url, HTTPAdapter(max_retries=retry_config))
 
             if api_key is not None:
-                JSON_HEADER["X-Agentops-Auth"] = api_key
+                JSON_HEADER["X-Agentops-Api-Key"] = api_key
 
             if parent_key is not None:
                 JSON_HEADER["X-Agentops-Parent-Key"] = parent_key
 
-            res = request_session.post(url, data=payload,
-                                       headers=JSON_HEADER, timeout=20)
+            if jwt is not None:
+                JSON_HEADER["Authorization"] = f"Bearer {jwt}"
+
+            res = request_session.post(
+                url, data=payload, headers=JSON_HEADER, timeout=20
+            )
 
             result.parse(res)
         except requests.exceptions.Timeout:
             result.code = 408
             result.status = HttpStatus.TIMEOUT
-            logger.warning(
-                '🖇 AgentOps: Could not post data - connection timed out')
+            logger.warning("Could not post data - connection timed out")
         except requests.exceptions.HTTPError as e:
             try:
                 result.parse(e.response)
             except Exception:
                 result = Response()
                 result.code = e.response.status_code
                 result.status = Response.get_status(e.response.status_code)
-                result.body = {'error': str(e)}
+                result.body = {"error": str(e)}
         except requests.exceptions.RequestException as e:
-            result.body = {'error': str(e)}
+            result.body = {"error": str(e)}
 
         if result.code == 401:
-            logger.warning('🖇 AgentOps: Could not post data - API server rejected your API key: %s',
-                           api_key)
+            logger.warning(
+                "Could not post data - API server rejected your API key: %s", api_key
+            )
         if result.code == 400:
-            logger.warning('🖇 AgentOps: Could not post data - %s', result.body)
+            logger.warning("Could not post data - %s", result.body)
         if result.code == 500:
-            logger.warning(
-                '🖇 AgentOps: Could not post data - internal server error')
+            logger.warning("Could not post data - internal server error")
 
         return result
```

#### encoding

```diff
@@ -1 +1 @@
-utf-8
+us-ascii
```

### Comparing `agentops-0.1.9/agentops/langchain_callback_handler.py` & `agentops-0.2.0/agentops/partners/langchain_callback_handler.py`

 * *Files 3% similar despite different names*

```diff
@@ -10,59 +10,70 @@
 
 from tenacity import RetryCallState
 
 from agentops import Client as AOClient
 from agentops import ActionEvent, LLMEvent, ToolEvent, ErrorEvent
 from agentops.helpers import get_ISO_time
 
-from .helpers import debug_print_function_params
+from ..helpers import debug_print_function_params
+import os
+from ..log_config import logger
+import logging
 
 
 def get_model_from_kwargs(kwargs: any) -> str:
-    if 'model' in kwargs['invocation_params']:
-        return kwargs['invocation_params']['model']
-    elif '_type' in kwargs['invocation_params']:
-        return kwargs['invocation_params']['_type']
+    if "model" in kwargs["invocation_params"]:
+        return kwargs["invocation_params"]["model"]
+    elif "_type" in kwargs["invocation_params"]:
+        return kwargs["invocation_params"]["_type"]
     else:
-        return 'unknown_model'
+        return "unknown_model"
 
 
-# def get_completion_from_response(response: LLMResult):
-#     if 'text' in response.generations[0][0]:
-#         return response.generations[0][0].text
-#     if ''
-#
-
 class Events:
     llm: Dict[str, LLMEvent] = {}
     tool: Dict[str, ToolEvent] = {}
     chain: Dict[str, ActionEvent] = {}
     retriever: Dict[str, ActionEvent] = {}
     error: Dict[str, ErrorEvent] = {}
 
 
 class LangchainCallbackHandler(BaseCallbackHandler):
     """Callback handler for Langchain agents."""
 
-    def __init__(self, api_key: Optional[str] = None,
-                 endpoint: Optional[str] = None,
-                 max_wait_time: Optional[int] = None,
-                 max_queue_size: Optional[int] = None,
-                 tags: Optional[List[str]] = None):
+    def __init__(
+        self,
+        api_key: Optional[str] = None,
+        endpoint: Optional[str] = None,
+        max_wait_time: Optional[int] = None,
+        max_queue_size: Optional[int] = None,
+        tags: Optional[List[str]] = None,
+    ):
+
+        logging_level = os.getenv("AGENTOPS_LOGGING_LEVEL")
+        log_levels = {
+            "CRITICAL": logging.CRITICAL,
+            "ERROR": logging.ERROR,
+            "INFO": logging.INFO,
+            "WARNING": logging.WARNING,
+            "DEBUG": logging.DEBUG,
+        }
+        logger.setLevel(log_levels.get(logging_level or "INFO", "INFO"))
 
         client_params: Dict[str, Any] = {
-            'api_key': api_key,
-            'endpoint': endpoint,
-            'max_wait_time': max_wait_time,
-            'max_queue_size': max_queue_size,
-            'tags': tags
+            "api_key": api_key,
+            "endpoint": endpoint,
+            "max_wait_time": max_wait_time,
+            "max_queue_size": max_queue_size,
+            "tags": tags,
         }
 
-        self.ao_client = AOClient(**{k: v for k, v in client_params.items()
-                                     if v is not None}, override=False)
+        self.ao_client = AOClient(
+            **{k: v for k, v in client_params.items() if v is not None}, override=False
+        )
         self.agent_actions: Dict[UUID, List[ActionEvent]] = defaultdict(list)
         self.events = Events()
 
     @debug_print_function_params
     def on_llm_start(
         self,
         serialized: Dict[str, Any],
@@ -71,30 +82,32 @@
         run_id: UUID,
         parent_run_id: Optional[UUID] = None,
         tags: Optional[List[str]] = None,
         metadata: Optional[Dict[str, Any]] = None,
         **kwargs: Any,
     ) -> Any:
         self.events.llm[str(run_id)] = LLMEvent(
-            params={**serialized,
-                    **({} if metadata is None else metadata),
-                    **kwargs},  # TODO: params is inconsistent, in ToolEvent we put it in logs
+            params={
+                **serialized,
+                **({} if metadata is None else metadata),
+                **kwargs,
+            },  # TODO: params is inconsistent, in ToolEvent we put it in logs
             model=get_model_from_kwargs(kwargs),
-            prompt=prompts[0]
+            prompt=prompts[0],
             # tags=tags # TODO
         )
 
     @debug_print_function_params
     def on_llm_error(
-            self,
-            error: BaseException,
-            *,
-            run_id: UUID,
-            parent_run_id: Optional[UUID] = None,
-            **kwargs: Any,
+        self,
+        error: BaseException,
+        *,
+        run_id: UUID,
+        parent_run_id: Optional[UUID] = None,
+        **kwargs: Any,
     ) -> Any:
         llm_event: LLMEvent = self.events.llm[str(run_id)]
         self.ao_client.record(llm_event)
 
         error_event = ErrorEvent(trigger_event=llm_event, exception=error)
         self.ao_client.record(error_event)
 
@@ -106,27 +119,35 @@
         run_id: UUID,
         parent_run_id: Optional[UUID] = None,
         **kwargs: Any,
     ) -> Any:
         llm_event: LLMEvent = self.events.llm[str(run_id)]
         llm_event.returns = {
             "content": response.generations[0][0].text,
-            "generations": response.generations
+            "generations": response.generations,
         }
         llm_event.end_timestamp = get_ISO_time()
         llm_event.completion = response.generations[0][0].text
         if response.llm_output is not None:
-            llm_event.prompt_tokens = response.llm_output['token_usage']['prompt_tokens']
-            llm_event.completion_tokens = response.llm_output['token_usage']['completion_tokens']
+            llm_event.prompt_tokens = response.llm_output["token_usage"][
+                "prompt_tokens"
+            ]
+            llm_event.completion_tokens = response.llm_output["token_usage"][
+                "completion_tokens"
+            ]
 
         self.ao_client.record(llm_event)
 
         if len(response.generations) == 0:
             # TODO: more descriptive error
-            error_event = ErrorEvent(trigger_event=self.events.llm[str(run_id)], error_type="NoGenerations", details="on_llm_end: No generations")
+            error_event = ErrorEvent(
+                trigger_event=self.events.llm[str(run_id)],
+                error_type="NoGenerations",
+                details="on_llm_end: No generations",
+            )
             self.ao_client.record(error_event)
 
     @debug_print_function_params
     def on_chain_start(
         self,
         serialized: Dict[str, Any],
         inputs: Dict[str, Any],
@@ -134,19 +155,21 @@
         run_id: UUID,
         parent_run_id: Optional[UUID] = None,
         tags: Optional[List[str]] = None,
         metadata: Optional[Dict[str, Any]] = None,
         **kwargs: Any,
     ) -> Any:
         self.events.chain[str(run_id)] = ActionEvent(
-            params={**serialized,
-                    **inputs,
-                    **({} if metadata is None else metadata),
-                    **kwargs},
-            action_type="chain"
+            params={
+                **serialized,
+                **inputs,
+                **({} if metadata is None else metadata),
+                **kwargs,
+            },
+            action_type="chain",
         )
 
     @debug_print_function_params
     def on_chain_end(
         self,
         outputs: Dict[str, Any],
         *,
@@ -185,101 +208,111 @@
         tags: Optional[List[str]] = None,
         metadata: Optional[Dict[str, Any]] = None,
         inputs: Optional[Dict[str, Any]] = None,
         **kwargs: Any,
     ) -> Any:
         self.events.tool[str(run_id)] = ToolEvent(
             params=input_str if inputs is None else inputs,
-            name=serialized['name'],
-            logs={**serialized,
-                  'tags': tags,
-                  **({} if metadata is None else metadata),
-                  **({} if inputs is None else inputs),
-                  **kwargs}
+            name=serialized["name"],
+            logs={
+                **serialized,
+                "tags": tags,
+                **({} if metadata is None else metadata),
+                **({} if inputs is None else inputs),
+                **kwargs,
+            },
         )
 
     @debug_print_function_params
     def on_tool_end(
-            self,
-            output: str,
-            *,
-            run_id: UUID,
-            parent_run_id: Optional[UUID] = None,
-            **kwargs: Any,
+        self,
+        output: str,
+        *,
+        run_id: UUID,
+        parent_run_id: Optional[UUID] = None,
+        **kwargs: Any,
     ) -> Any:
         tool_event: ToolEvent = self.events.tool[str(run_id)]
         tool_event.end_timestamp = get_ISO_time()
         tool_event.returns = output
         self.ao_client.record(tool_event)
 
         # Tools are capable of failing `on_tool_end` quietly.
         # This is a workaround to make sure we can log it as an error.
-        if kwargs.get('name') == '_Exception':
-            error_event = ErrorEvent(trigger_event=tool_event, error_type="LangchainToolException", details=output)
+        if kwargs.get("name") == "_Exception":
+            error_event = ErrorEvent(
+                trigger_event=tool_event,
+                error_type="LangchainToolException",
+                details=output,
+            )
             self.ao_client.record(error_event)
 
     @debug_print_function_params
     def on_tool_error(
-            self,
-            error: BaseException,
-            *,
-            run_id: UUID,
-            parent_run_id: Optional[UUID] = None,
-            **kwargs: Any,
+        self,
+        error: BaseException,
+        *,
+        run_id: UUID,
+        parent_run_id: Optional[UUID] = None,
+        **kwargs: Any,
     ) -> Any:
         tool_event: ToolEvent = self.events.tool[str(run_id)]
         self.ao_client.record(tool_event)
 
         error_event = ErrorEvent(trigger_event=tool_event, exception=error)
         self.ao_client.record(error_event)
 
     @debug_print_function_params
     def on_retriever_start(
-            self,
-            serialized: Dict[str, Any],
-            query: str,
-            *,
-            run_id: UUID,
-            parent_run_id: Optional[UUID] = None,
-            tags: Optional[List[str]] = None,
-            metadata: Optional[Dict[str, Any]] = None,
-            **kwargs: Any,
+        self,
+        serialized: Dict[str, Any],
+        query: str,
+        *,
+        run_id: UUID,
+        parent_run_id: Optional[UUID] = None,
+        tags: Optional[List[str]] = None,
+        metadata: Optional[Dict[str, Any]] = None,
+        **kwargs: Any,
     ) -> None:
         self.events.retriever[str(run_id)] = ActionEvent(
-            params={**serialized,
-                    "query": query,
-                    **({} if metadata is None else metadata),
-                    ** kwargs},
-            action_type="retriever"
+            params={
+                **serialized,
+                "query": query,
+                **({} if metadata is None else metadata),
+                **kwargs,
+            },
+            action_type="retriever",
         )
 
     @debug_print_function_params
     def on_retriever_end(
-            self,
-            documents: Sequence[Document],
-            *,
-            run_id: UUID,
-            parent_run_id: Optional[UUID] = None,
-            tags: Optional[List[str]] = None,
-            **kwargs: Any,
+        self,
+        documents: Sequence[Document],
+        *,
+        run_id: UUID,
+        parent_run_id: Optional[UUID] = None,
+        tags: Optional[List[str]] = None,
+        **kwargs: Any,
     ) -> None:
         action_event: ActionEvent = self.events.retriever[str(run_id)]
-        action_event.logs = documents  # TODO: Adding this. Might want to add elsewhere e.g. params
+        action_event.logs = (
+            documents  # TODO: Adding this. Might want to add elsewhere e.g. params
+        )
         action_event.end_timestamp = get_ISO_time()
         self.ao_client.record(action_event)
 
     @debug_print_function_params
     def on_retriever_error(
-            self,
-            error: BaseException,
-            *,
-            run_id: UUID,
-            parent_run_id: Optional[UUID] = None,
-            tags: Optional[List[str]] = None,
-            **kwargs: Any,
+        self,
+        error: BaseException,
+        *,
+        run_id: UUID,
+        parent_run_id: Optional[UUID] = None,
+        tags: Optional[List[str]] = None,
+        **kwargs: Any,
     ) -> None:
         action_event: ActionEvent = self.events.retriever[str(run_id)]
         self.ao_client.record(action_event)
 
         error_event = ErrorEvent(trigger_event=action_event, exception=error)
         self.ao_client.record(error_event)
 
@@ -288,28 +321,26 @@
         self,
         action: AgentAction,
         *,
         run_id: UUID,
         parent_run_id: Optional[UUID] = None,
         **kwargs: Any,
     ) -> Any:
-        self.agent_actions[run_id].append(ActionEvent(
-            params={"action": action,
-                    **kwargs},
-            action_type="agent"
-        ))
+        self.agent_actions[run_id].append(
+            ActionEvent(params={"action": action, **kwargs}, action_type="agent")
+        )
 
     @debug_print_function_params
     def on_agent_finish(
-            self,
-            finish: AgentFinish,
-            *,
-            run_id: UUID,
-            parent_run_id: Optional[UUID] = None,
-            **kwargs: Any,
+        self,
+        finish: AgentFinish,
+        *,
+        run_id: UUID,
+        parent_run_id: Optional[UUID] = None,
+        **kwargs: Any,
     ) -> Any:
         # Need to attach finish to some on_agent_action so just choosing the last one
         self.agent_actions[run_id][-1].returns = finish.to_json()
 
         for agentAction in self.agent_actions[run_id]:
             self.ao_client.record(agentAction)
 
@@ -337,30 +368,34 @@
     def session_id(self):
         return self.ao_client.current_session_id
 
 
 class AsyncLangchainCallbackHandler(AsyncCallbackHandler):
     """Callback handler for Langchain agents."""
 
-    def __init__(self, api_key: Optional[str] = None,
-                 endpoint: Optional[str] = None,
-                 max_wait_time: Optional[int] = None,
-                 max_queue_size: Optional[int] = None,
-                 tags: Optional[List[str]] = None):
+    def __init__(
+        self,
+        api_key: Optional[str] = None,
+        endpoint: Optional[str] = None,
+        max_wait_time: Optional[int] = None,
+        max_queue_size: Optional[int] = None,
+        tags: Optional[List[str]] = None,
+    ):
 
         client_params: Dict[str, Any] = {
-            'api_key': api_key,
-            'endpoint': endpoint,
-            'max_wait_time': max_wait_time,
-            'max_queue_size': max_queue_size,
-            'tags': tags
+            "api_key": api_key,
+            "endpoint": endpoint,
+            "max_wait_time": max_wait_time,
+            "max_queue_size": max_queue_size,
+            "tags": tags,
         }
 
-        self.ao_client = AOClient(**{k: v for k, v in client_params.items()
-                                     if v is not None}, override=False)
+        self.ao_client = AOClient(
+            **{k: v for k, v in client_params.items() if v is not None}, override=False
+        )
 
         self.events = Events()
         self.agent_actions: Dict[UUID, List[ActionEvent]] = defaultdict(list)
 
     @debug_print_function_params
     async def on_llm_start(
         self,
@@ -370,19 +405,21 @@
         run_id: UUID,
         parent_run_id: Optional[UUID] = None,
         tags: Optional[List[str]] = None,
         metadata: Optional[Dict[str, Any]] = None,
         **kwargs: Any,
     ) -> Any:
         self.events.llm[str(run_id)] = LLMEvent(
-            params={**serialized,
-                    **({} if metadata is None else metadata),
-                    **kwargs},  # TODO: params is inconsistent, in ToolEvent we put it in logs
-            model=kwargs['invocation_params']['model'],
-            prompt=prompts[0]
+            params={
+                **serialized,
+                **({} if metadata is None else metadata),
+                **kwargs,
+            },  # TODO: params is inconsistent, in ToolEvent we put it in logs
+            model=kwargs["invocation_params"]["model"],
+            prompt=prompts[0],
         )
 
     @debug_print_function_params
     async def on_chat_model_start(
         self,
         serialized: Dict[str, Any],
         messages: List[List[BaseMessage]],
@@ -406,20 +443,20 @@
         tags: Optional[List[str]] = None,
         **kwargs: Any,
     ) -> None:
         pass
 
     @debug_print_function_params
     async def on_llm_error(
-            self,
-            error: BaseException,
-            *,
-            run_id: UUID,
-            parent_run_id: Optional[UUID] = None,
-            **kwargs: Any,
+        self,
+        error: BaseException,
+        *,
+        run_id: UUID,
+        parent_run_id: Optional[UUID] = None,
+        **kwargs: Any,
     ) -> Any:
         llm_event: LLMEvent = self.events.llm[str(run_id)]
         self.ao_client.record(llm_event)
 
         error_event = ErrorEvent(trigger_event=llm_event, exception=error)
         self.ao_client.record(error_event)
 
@@ -431,26 +468,34 @@
         run_id: UUID,
         parent_run_id: Optional[UUID] = None,
         **kwargs: Any,
     ) -> Any:
         llm_event: LLMEvent = self.events.llm[str(run_id)]
         llm_event.returns = {
             "content": response.generations[0][0].text,
-            "generations": response.generations
+            "generations": response.generations,
         }
         llm_event.end_timestamp = get_ISO_time()
         llm_event.completion = response.generations[0][0].text
         if response.llm_output is not None:
-            llm_event.prompt_tokens = response.llm_output['token_usage']['prompt_tokens']
-            llm_event.completion_tokens = response.llm_output['token_usage']['completion_tokens']
+            llm_event.prompt_tokens = response.llm_output["token_usage"][
+                "prompt_tokens"
+            ]
+            llm_event.completion_tokens = response.llm_output["token_usage"][
+                "completion_tokens"
+            ]
         self.ao_client.record(llm_event)
 
         if len(response.generations) == 0:
             # TODO: more descriptive error
-            error_event = ErrorEvent(trigger_event=self.events.llm[str(run_id)], error_type="NoGenerations", details="on_llm_end: No generations")
+            error_event = ErrorEvent(
+                trigger_event=self.events.llm[str(run_id)],
+                error_type="NoGenerations",
+                details="on_llm_end: No generations",
+            )
             self.ao_client.record(error_event)
 
     @debug_print_function_params
     async def on_chain_start(
         self,
         serialized: Dict[str, Any],
         inputs: Dict[str, Any],
@@ -458,19 +503,21 @@
         run_id: UUID,
         parent_run_id: Optional[UUID] = None,
         tags: Optional[List[str]] = None,
         metadata: Optional[Dict[str, Any]] = None,
         **kwargs: Any,
     ) -> Any:
         self.events.chain[str(run_id)] = ActionEvent(
-            params={**serialized,
-                    **inputs,
-                    **({} if metadata is None else metadata),
-                    **kwargs},
-            action_type="chain"
+            params={
+                **serialized,
+                **inputs,
+                **({} if metadata is None else metadata),
+                **kwargs,
+            },
+            action_type="chain",
         )
 
     @debug_print_function_params
     async def on_chain_end(
         self,
         outputs: Dict[str, Any],
         *,
@@ -509,101 +556,111 @@
         tags: Optional[List[str]] = None,
         metadata: Optional[Dict[str, Any]] = None,
         inputs: Optional[Dict[str, Any]] = None,
         **kwargs: Any,
     ) -> Any:
         self.events.tool[str(run_id)] = ToolEvent(
             params=input_str if inputs is None else inputs,
-            name=serialized['name'],
-            logs={**serialized,
-                  'tags': tags,
-                  **({} if metadata is None else metadata),
-                  **({} if inputs is None else inputs),
-                  **kwargs}
+            name=serialized["name"],
+            logs={
+                **serialized,
+                "tags": tags,
+                **({} if metadata is None else metadata),
+                **({} if inputs is None else inputs),
+                **kwargs,
+            },
         )
 
     @debug_print_function_params
     async def on_tool_end(
-            self,
-            output: str,
-            *,
-            run_id: UUID,
-            parent_run_id: Optional[UUID] = None,
-            **kwargs: Any,
+        self,
+        output: str,
+        *,
+        run_id: UUID,
+        parent_run_id: Optional[UUID] = None,
+        **kwargs: Any,
     ) -> Any:
         tool_event: ToolEvent = self.events.tool[str(run_id)]
         tool_event.end_timestamp = get_ISO_time()
         tool_event.returns = output
         self.ao_client.record(tool_event)
 
         # Tools are capable of failing `on_tool_end` quietly.
         # This is a workaround to make sure we can log it as an error.
-        if kwargs.get('name') == '_Exception':
-            error_event = ErrorEvent(trigger_event=tool_event, error_type="LangchainToolException", details=output)
+        if kwargs.get("name") == "_Exception":
+            error_event = ErrorEvent(
+                trigger_event=tool_event,
+                error_type="LangchainToolException",
+                details=output,
+            )
             self.ao_client.record(error_event)
 
     @debug_print_function_params
     async def on_tool_error(
-            self,
-            error: BaseException,
-            *,
-            run_id: UUID,
-            parent_run_id: Optional[UUID] = None,
-            **kwargs: Any,
+        self,
+        error: BaseException,
+        *,
+        run_id: UUID,
+        parent_run_id: Optional[UUID] = None,
+        **kwargs: Any,
     ) -> Any:
         tool_event: ToolEvent = self.events.tool[str(run_id)]
         self.ao_client.record(tool_event)
 
         error_event = ErrorEvent(trigger_event=tool_event, exception=error)
         self.ao_client.record(error_event)
 
     @debug_print_function_params
     async def on_retriever_start(
-            self,
-            serialized: Dict[str, Any],
-            query: str,
-            *,
-            run_id: UUID,
-            parent_run_id: Optional[UUID] = None,
-            tags: Optional[List[str]] = None,
-            metadata: Optional[Dict[str, Any]] = None,
-            **kwargs: Any,
+        self,
+        serialized: Dict[str, Any],
+        query: str,
+        *,
+        run_id: UUID,
+        parent_run_id: Optional[UUID] = None,
+        tags: Optional[List[str]] = None,
+        metadata: Optional[Dict[str, Any]] = None,
+        **kwargs: Any,
     ) -> None:
         self.events.retriever[str(run_id)] = ActionEvent(
-            params={**serialized,
-                    "query": query,
-                    **({} if metadata is None else metadata),
-                    ** kwargs},
-            action_type="retriever"
+            params={
+                **serialized,
+                "query": query,
+                **({} if metadata is None else metadata),
+                **kwargs,
+            },
+            action_type="retriever",
         )
 
     @debug_print_function_params
     async def on_retriever_end(
-            self,
-            documents: Sequence[Document],
-            *,
-            run_id: UUID,
-            parent_run_id: Optional[UUID] = None,
-            tags: Optional[List[str]] = None,
-            **kwargs: Any,
+        self,
+        documents: Sequence[Document],
+        *,
+        run_id: UUID,
+        parent_run_id: Optional[UUID] = None,
+        tags: Optional[List[str]] = None,
+        **kwargs: Any,
     ) -> None:
         action_event: ActionEvent = self.events.retriever[str(run_id)]
-        action_event.logs = documents  # TODO: Adding this. Might want to add elsewhere e.g. params
+        action_event.logs = (
+            documents  # TODO: Adding this. Might want to add elsewhere e.g. params
+        )
         action_event.end_timestamp = get_ISO_time()
         self.ao_client.record(action_event)
 
     @debug_print_function_params
     async def on_retriever_error(
-            self,
-            error: BaseException,
-            *,
-            run_id: UUID,
-            parent_run_id: Optional[UUID] = None,
-            tags: Optional[List[str]] = None,
-            **kwargs: Any,
+        self,
+        error: BaseException,
+        *,
+        run_id: UUID,
+        parent_run_id: Optional[UUID] = None,
+        tags: Optional[List[str]] = None,
+        **kwargs: Any,
     ) -> None:
         action_event: ActionEvent = self.events.retriever[str(run_id)]
         self.ao_client.record(action_event)
 
         error_event = ErrorEvent(trigger_event=action_event, exception=error)
         self.ao_client.record(error_event)
 
@@ -612,28 +669,26 @@
         self,
         action: AgentAction,
         *,
         run_id: UUID,
         parent_run_id: Optional[UUID] = None,
         **kwargs: Any,
     ) -> Any:
-        self.agent_actions[run_id].append(ActionEvent(
-            params={"action": action,
-                    **kwargs},
-            action_type="agent"
-        ))
+        self.agent_actions[run_id].append(
+            ActionEvent(params={"action": action, **kwargs}, action_type="agent")
+        )
 
     @debug_print_function_params
     async def on_agent_finish(
-            self,
-            finish: AgentFinish,
-            *,
-            run_id: UUID,
-            parent_run_id: Optional[UUID] = None,
-            **kwargs: Any,
+        self,
+        finish: AgentFinish,
+        *,
+        run_id: UUID,
+        parent_run_id: Optional[UUID] = None,
+        **kwargs: Any,
     ) -> Any:
         # Need to attach finish to some on_agent_action so just choosing the last one
         self.agent_actions[run_id][-1].returns = finish.to_json()
 
         for agentAction in self.agent_actions[run_id]:
             self.ao_client.record(agentAction)
```

### Comparing `agentops-0.1.9/agentops/meta_client.py` & `agentops-0.2.0/agentops/meta_client.py`

 * *Files 6% similar despite different names*

```diff
@@ -10,45 +10,54 @@
 
 class MetaClient(type):
     """Metaclass to automatically decorate methods with exception handling and provide a shared exception handler."""
 
     def __new__(cls, name, bases, dct):
         # Wrap each method with the handle_exceptions decorator
         for method_name, method in dct.items():
-            if (callable(method) and not method_name.startswith("__")) or method_name == "__init__":
+            if (
+                callable(method) and not method_name.startswith("__")
+            ) or method_name == "__init__":
                 dct[method_name] = handle_exceptions(method)
 
         return super().__new__(cls, name, bases, dct)
 
-    def send_exception_to_server(cls, exception, api_key):
+    def send_exception_to_server(cls, exception, api_key, session):
         """Class method to send exception to server."""
         if api_key:
             exception_type = type(exception).__name__
             exception_message = str(exception)
             exception_traceback = traceback.format_exc()
             developer_error = {
                 "sdk_version": get_agentops_version(),
                 "type": exception_type,
                 "message": exception_message,
                 "stack_trace": exception_traceback,
-                "host_env": get_host_env()
+                "host_env": get_host_env(),
             }
 
-            HttpClient.post("https://api.agentops.ai/developer_errors",
-                            safe_serialize(developer_error).encode("utf-8"),
-                            api_key=api_key)
+            if session:
+                developer_error["session_id"] = session.session_id
+
+            HttpClient.post(
+                "https://api.agentops.ai/v2/developer_errors",
+                safe_serialize(developer_error).encode("utf-8"),
+                api_key=api_key,
+            )
 
 
 def handle_exceptions(method):
     """Decorator within the metaclass to wrap method execution in try-except block."""
 
     def wrapper(self, *args, **kwargs):
         try:
             return method(self, *args, **kwargs)
         except Exception as e:
-            logger.warning(f"🖇 AgentOps: Error: {e}")
-            config = getattr(self, 'config', None)
+            logger.warning(f"Error: {e}")
+            config = getattr(self, "config", None)
             if config is not None:
-                type(self).send_exception_to_server(e, self.config._api_key)
+                type(self).send_exception_to_server(
+                    e, self.config._api_key, self._session
+                )
             raise e
 
     return wrapper
```

#### encoding

```diff
@@ -1 +1 @@
-utf-8
+us-ascii
```

### Comparing `agentops-0.1.9/agentops/session.py` & `agentops-0.2.0/agentops/session.py`

 * *Files 6% similar despite different names*

```diff
@@ -15,15 +15,20 @@
         init_timestamp (float): The timestamp for when the session started, represented as seconds since the epoch.
         end_timestamp (float, optional): The timestamp for when the session ended, represented as seconds since the epoch. This is only set after end_session is called.
         end_state (str, optional): The final state of the session. Suggested: "Success", "Fail", "Indeterminate"
         end_state_reason (str, optional): The reason for ending the session.
 
     """
 
-    def __init__(self, session_id: UUID, tags: Optional[List[str]] = None, host_env: Optional[dict] = None):
+    def __init__(
+        self,
+        session_id: UUID,
+        tags: Optional[List[str]] = None,
+        host_env: Optional[dict] = None,
+    ):
         self.end_timestamp = None
         self.end_state: Optional[str] = None
         self.session_id = session_id
         self.init_timestamp = get_ISO_time()
         self.tags = tags
         self.video: Optional[str] = None
         self.end_state_reason: Optional[str] = None
@@ -34,15 +39,17 @@
         Sets a url to the video recording of the session.
 
         Args:
             video (str): The url of the video recording
         """
         self.video = video
 
-    def end_session(self, end_state: str = "Indeterminate", end_state_reason: Optional[str] = None) -> None:
+    def end_session(
+        self, end_state: str = "Indeterminate", end_state_reason: Optional[str] = None
+    ) -> None:
         """
         End the session with a specified state, rating, and reason.
 
         Args:
             end_state (str, optional): The final state of the session. Options: "Success", "Fail", "Indeterminate"
             rating (str, optional): The rating for the session.
             end_state_reason (str, optional): The reason for ending the session. Provides context for why the session ended.
```

### Comparing `agentops-0.1.9/agentops/worker.py` & `agentops-0.2.0/agentops/worker.py`

 * *Files 22% similar despite different names*

```diff
@@ -1,29 +1,29 @@
 import json
+from .log_config import logger
 import threading
 import time
 from .http_client import HttpClient
 from .config import Configuration
 from .session import Session
 from .helpers import safe_serialize, filter_unjsonable
 from typing import Dict, Optional
-import os
 
 
 class Worker:
     def __init__(self, config: Configuration) -> None:
         self.config = config
         self.queue: list[Dict] = []
         self.lock = threading.Lock()
         self.stop_flag = threading.Event()
         self.thread = threading.Thread(target=self.run)
         self.thread.daemon = True
         self.thread.start()
         self._session: Optional[Session] = None
-        self._debug_mode = os.getenv('DEBUG_MODE') == 'Y'
+        self.jwt = None
 
     def add_event(self, event: dict) -> None:
         with self.lock:
             self.queue.append(event)
             if len(self.queue) >= self.config.max_queue_size:
                 self.flush_queue()
 
@@ -31,89 +31,111 @@
         with self.lock:
             if len(self.queue) > 0:
                 events = self.queue
                 self.queue = []
 
                 payload = {
                     "session_id": getattr(self._session, "session_id", None),
-                    "events": events
+                    "events": events,
                 }
 
                 serialized_payload = safe_serialize(payload).encode("utf-8")
-                HttpClient.post(f'{self.config.endpoint}/events',
-                                serialized_payload,
-                                self.config.api_key,
-                                self.config.parent_key)
-
-                if self._debug_mode:
-                    print("\n<AGENTOPS_DEBUG_OUTPUT>")
-                    print(f"Worker request to {self.config.endpoint}/events")
-                    print(serialized_payload)
-                    print("</AGENTOPS_DEBUG_OUTPUT>\n")
+                HttpClient.post(
+                    f"{self.config.endpoint}/v2/create_events",
+                    serialized_payload,
+                    jwt=self.jwt,
+                )
+
+                logger.debug("\n<AGENTOPS_DEBUG_OUTPUT>")
+                logger.debug(f"Worker request to {self.config.endpoint}/events")
+                logger.debug(serialized_payload)
+                logger.debug("</AGENTOPS_DEBUG_OUTPUT>\n")
+
+    def reauthorize_jwt(self, session: Session) -> bool:
+        self._session = session
+        with self.lock:
+            payload = {"session_id": session.session_id}
+            serialized_payload = json.dumps(filter_unjsonable(payload)).encode("utf-8")
+            res = HttpClient.post(
+                f"{self.config.endpoint}/v2/reauthorize_jwt",
+                serialized_payload,
+                self.config.api_key,
+            )
+
+            logger.debug(res.body)
+
+            if res.code != 200:
+                return False
+
+            self.jwt = res.body.get("jwt", None)
+            if self.jwt is None:
+                return False
+
+            return True
 
     def start_session(self, session: Session) -> bool:
         self._session = session
         with self.lock:
-            payload = {
-                "session": session.__dict__
-            }
+            payload = {"session": session.__dict__}
             serialized_payload = json.dumps(filter_unjsonable(payload)).encode("utf-8")
-            res = HttpClient.post(f'{self.config.endpoint}/sessions',
-                                  serialized_payload,
-                                  self.config.api_key,
-                                  self.config.parent_key)
+            res = HttpClient.post(
+                f"{self.config.endpoint}/v2/create_session",
+                serialized_payload,
+                self.config.api_key,
+                self.config.parent_key,
+            )
+
+            logger.debug(res.body)
 
             if res.code != 200:
                 return False
 
+            self.jwt = res.body.get("jwt", None)
+            if self.jwt is None:
+                return False
+
             return True
 
     def end_session(self, session: Session) -> str:
         self.stop_flag.set()
         self.thread.join(timeout=1)
         self.flush_queue()
         self._session = None
 
         with self.lock:
-            payload = {
-                "session": session.__dict__
-            }
-
-            res = HttpClient.post(f'{self.config.endpoint}/sessions',
-                            json.dumps(filter_unjsonable(
-                                payload)).encode("utf-8"),
-                            self.config.api_key,
-                            self.config.parent_key)
+            payload = {"session": session.__dict__}
 
-            return res.body.get('token_cost', "unknown")
+            res = HttpClient.post(
+                f"{self.config.endpoint}/v2/update_session",
+                json.dumps(filter_unjsonable(payload)).encode("utf-8"),
+                jwt=self.jwt,
+            )
+            logger.debug(res.body)
+            return res.body.get("token_cost", "unknown")
 
     def update_session(self, session: Session) -> None:
         with self.lock:
-            payload = {
-                "session": session.__dict__
-            }
-
-            HttpClient.post(f'{self.config.endpoint}/sessions',
-                            json.dumps(filter_unjsonable(
-                                payload)).encode("utf-8"),
-                            self.config.api_key,
-                            self.config.parent_key)
+            payload = {"session": session.__dict__}
+
+            res = HttpClient.post(
+                f"{self.config.endpoint}/v2/update_session",
+                json.dumps(filter_unjsonable(payload)).encode("utf-8"),
+                jwt=self.jwt,
+            )
 
     def create_agent(self, agent_id, name):
         payload = {
             "id": agent_id,
             "name": name,
             "session_id": getattr(self._session, "session_id", None),
         }
 
-        serialized_payload = \
-            safe_serialize(payload).encode("utf-8")
-        HttpClient.post(f'{self.config.endpoint}/agents',
-                        serialized_payload,
-                        self.config.api_key,
-                        self.config.parent_key)
+        serialized_payload = safe_serialize(payload).encode("utf-8")
+        HttpClient.post(
+            f"{self.config.endpoint}/v2/create_agent", serialized_payload, jwt=self.jwt
+        )
 
     def run(self) -> None:
         while not self.stop_flag.is_set():
             time.sleep(self.config.max_wait_time / 1000)
             if self.queue:
                 self.flush_queue()
```

### Comparing `agentops-0.1.9/agentops.egg-info/PKG-INFO` & `agentops-0.2.0/agentops.egg-info/PKG-INFO`

 * *Files 16% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: agentops
-Version: 0.1.9
+Version: 0.2.0
 Summary: Python SDK for developing AI agent evals and observability
 Author-email: Alex Reibman <areibman@gmail.com>, Shawn Qiu <siyangqiu@gmail.com>, Braelyn Boynton <bboynton97@gmail.com>, Howard Gil <howardbgil@gmail.com>
 Project-URL: Homepage, https://github.com/AgentOps-AI/agentops
 Project-URL: Issues, https://github.com/AgentOps-AI/agentops/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
@@ -14,19 +14,19 @@
 Requires-Dist: requests==2.31.0
 Requires-Dist: psutil==5.9.8
 Requires-Dist: packaging==23.2
 Provides-Extra: dev
 Requires-Dist: pytest==7.4.0; extra == "dev"
 Requires-Dist: requests_mock==1.11.0; extra == "dev"
 Provides-Extra: langchain
-Requires-Dist: langchain>=0.0.354; extra == "langchain"
+Requires-Dist: langchain~=1.19; extra == "langchain"
 
 <div align="center">
   <a href="https://agentops.ai?ref=gh">
-    <img src="https://github.com/AgentOps-AI/agentops/blob/df22e9dffb7294fb977dc103a2ca3bcf8f04946f/logo.png" style="margin: 15px; max-width: 300px" width="50%" alt="Logo">
+    <img src="https://raw.githubusercontent.com/AgentOps-AI/agentops/35d5682866921a9e28d8ef66ae3c3b3d92d8fa6b/img/logo.png" style="margin: 15px; max-width: 300px" width="50%" alt="Logo">
   </a>
 </div>
 <p align="center">
   <em>AI agents suck. We’re fixing that.</em>
 </p>
 
 <p align="center">
@@ -43,45 +43,47 @@
 <a href="https://app.agentops.ai/?ref=gh">🖇️ AgentOps</a>
 <span>&nbsp;&nbsp;•&nbsp;&nbsp;</span>
 <a href="https://docs.agentops.ai/introduction">📙 Documentation</a>
 </p>
 
 # AgentOps 🖇️
 
-[![License: MIT](https://img.shields.io/badge/License-MIT-yellow.svg)](https://opensource.org/licenses/MIT) ![PyPI - Version](https://img.shields.io/pypi/v/agentops) <a href="https://pepy.tech/project/agentops">
-  <img src="https://static.pepy.tech/badge/agentops/month"> <a href="https://twitter.com/agentopsai">
-    <img src="https://img.shields.io/badge/follow-%40agentops-1DA1F2?logo=twitter&style=social" alt="AgentOps Twitter" /> 
-  </a>
-  <a href="https://discord.gg/mKW3ZhN9p2">
-    <img src="https://img.shields.io/badge/chat-on%20Discord-blueviolet" alt="Discord community channel" />
-  </a>
-  <a href="mailto:investor@agentops.ai"><img src="https://img.shields.io/website?color=%23f26522&down_message=Y%20Combinator&label=Not%20Backed%20By&logo=ycombinator&style=flat-square&up_message=Y%20Combinator&url=https%3A%2F%2Fwww.ycombinator.com"/>
-  <a href="https://github.com/agentops-ai/agentops/issues">
-    <img src="https://img.shields.io/github/commit-activity/m/agentops-ai/agentops" alt="git commit activity" />
-  </a>
-
+[![License: MIT](https://img.shields.io/badge/License-MIT-yellow.svg)](https://opensource.org/licenses/MIT)
+![PyPI - Version](https://img.shields.io/pypi/v/agentops)
+<a href="https://pepy.tech/project/agentops">
+  <img src="https://static.pepy.tech/badge/agentops/month">
+</a>
+<a href="https://twitter.com/agentopsai">
+  <img src="https://img.shields.io/badge/follow-%40agentops-1DA1F2?logo=twitter&style=social" alt="AgentOps Twitter"/>
+</a>
+<a href="https://discord.gg/mKW3ZhN9p2">
+  <img src="https://img.shields.io/badge/chat-on%20Discord-blueviolet" alt="Discord community channel"/>
+</a>
+<a href="https://github.com/agentops-ai/agentops/issues">
+  <img src="https://img.shields.io/github/commit-activity/m/agentops-ai/agentops" alt="git commit activity"/>
+</a>
 
 AgentOps helps developers build, evaluate, and monitor AI agents. Tools to build agents from prototype to production.
 
-
-|||
-|------------------------------------------|----------------------------------------------------|
-| 📊 **Replay Analytics and Debugging** | Step-by-step agent execution graphs |
-| 💸 **LLM Cost Management**   | Track spend with LLM foundation model providers |
-| 🧪 **Agent Benchmarking** | Test your agents against 1,000+ evals |
-| 🔐 **Compliance and Security**            | Detect common prompt injection and data exfiltration exploits |
-| 🤝 **Framework Integrations**            | Easily plugs in with frameworks like CrewAI and LangChain |
+|                                       |                                                               |
+| ------------------------------------- | ------------------------------------------------------------- |
+| 📊 **Replay Analytics and Debugging** | Step-by-step agent execution graphs                           |
+| 💸 **LLM Cost Management**            | Track spend with LLM foundation model providers               |
+| 🧪 **Agent Benchmarking**             | Test your agents against 1,000+ evals                         |
+| 🔐 **Compliance and Security**        | Detect common prompt injection and data exfiltration exploits |
+| 🤝 **Framework Integrations**         | Easily plugs in with frameworks like CrewAI and LangChain     |
 
 ## Quick Start ⌨️
 
-```python
+```bash
 pip install agentops
 ```
 
 ### Session replays in 3 lines of code
+
 Initialize the AgentOps client and automatically get analytics on every LLM call.
 
 ```python
 import agentops
 
 # Beginning of program's code (i.e. main.py, __init__.py)
 agentops.init(<INSERT YOUR API KEY HERE>)
@@ -95,15 +97,14 @@
 # End of program
 agentops.end_session('Success')
 # Woohoo You're done 🎉
 ```
 
 All your sessions are available on the [AgentOps dashboard](https://app.agentops.ai?ref=gh). Refer to our [API documentation](http://docs.agentops.ai) for detailed instructions.
 
-
 <details open>
   <summary>Agent Dashboard</summary>
   <a href="https://app.agentops.ai?ref=gh">
    <img src="https://github.com/AgentOps-AI/agentops/assets/14807319/158e082a-9a7d-49b7-9b41-51a49a1f7d3d" style="width: 90%;" alt="Agent Dashboard"/>
   </a>
 </details>
 
@@ -123,22 +124,30 @@
 
 ## Integrations 🦾
 
 ### CrewAI 🛶
 
 Build Crew agents with observability with only 2 lines of code. Simply set an `AGENTOPS_API_KEY` in your environment, and your crews will get automatic monitoring on the AgentOps dashboard.
 
-AgentOps is officially supported on Crew's latest rc branch: `crewai==0.28.9rc1`
+AgentOps is integrated with CrewAI on a pre-release fork. Install crew with
 
-* [AgentOps integration example](https://docs.agentops.ai/v1/integrations/crewai)
-* [Offical CrewAI documentation](https://docs.crewai.com/how-to/AgentOps-Observability)
+```bash
+pip install git+https://github.com/AgentOps-AI/crewAI.git@main
+```
 
+- [AgentOps integration example](https://docs.agentops.ai/v1/integrations/crewai)
+- [Official CrewAI documentation](https://docs.crewai.com/how-to/AgentOps-Observability)
 
 ### Langchain 🦜🔗
+
 AgentOps works seamlessly with applications built using Langchain. To use the handler, install Langchain as an optional dependency:
+
+<details>
+  <summary>Installation</summary>
+  
 ```shell
 pip install agentops[langchain]
 ```
 
 To use the handler, import and set
 
 ```python
@@ -160,45 +169,100 @@
                          verbose=True,
                          callbacks=[handler], # You must pass in a callback handler to record your agent
                          handle_parsing_errors=True)
 ```
 
 Check out the [Langchain Examples Notebook](./examples/langchain_examples.ipynb) for more details including Async handlers.
 
-### LlamaIndex 🦙
-(Coming Soon)
+</details>
+
+### Cohere ⌨️
+
+First class support for Cohere(>=5.4.0). This is a living integration, should you need any added functionality please message us on Discord!
+
+- [AgentOps integration example](https://docs.agentops.ai/v1/integrations/cohere)
+- [Official Cohere documentation](https://docs.cohere.com/reference/about)
+
+<details>
+  <summary>Installation</summary>
+  
+```bash
+pip install cohere
+```
+
+```python python
+import cohere
+import agentops
+
+# Beginning of program's code (i.e. main.py, __init__.py)
+agentops.init(<INSERT YOUR API KEY HERE>)
+co = cohere.Client()
+
+chat = co.chat(
+    message="Is it pronounced ceaux-hear or co-hehray?"
+)
+
+print(chat)
+
+agentops.end_session('Success')
+```
+
+```python python
+import cohere
+import agentops
+
+# Beginning of program's code (i.e. main.py, __init__.py)
+agentops.init(<INSERT YOUR API KEY HERE>)
 
+co = cohere.Client()
 
+stream = co.chat_stream(
+    message="Write me a haiku about the synergies between Cohere and AgentOps"
+)
+
+for event in stream:
+    if event.event_type == "text-generation":
+        print(event.text, end='')
+
+agentops.end_session('Success')
+```
+</details>
+
+
+### LlamaIndex 🦙
+
+(Coming Soon)
 
 ## Time travel debugging 🔮
+
 (coming soon!)
 
 ## Agent Arena 🥊
+
 (coming soon!)
 
 ## Evaluations Roadmap 🧭
 
-| Platform | Dashboard | Evals |
-|---|---|---|
-|✅ Python SDK | ✅ Multi-session and Cross-session metrics | ✅ Custom eval metrics |
-|🚧 Evaluation builder API | ✅ Custom event tag tracking | 🔜 Agent scorecards |
-|✅ [Javascript/Typescript SDK](https://github.com/AgentOps-AI/agentops-node) | ✅ Session replays| 🔜 Evaluation playground + leaderboard|
-
+| Platform                                                                     | Dashboard                                  | Evals                                  |
+| ---------------------------------------------------------------------------- | ------------------------------------------ | -------------------------------------- |
+| ✅ Python SDK                                                                | ✅ Multi-session and Cross-session metrics | ✅ Custom eval metrics                 |
+| 🚧 Evaluation builder API                                                    | ✅ Custom event tag tracking               | 🔜 Agent scorecards                    |
+| ✅ [Javascript/Typescript SDK](https://github.com/AgentOps-AI/agentops-node) | ✅ Session replays                         | 🔜 Evaluation playground + leaderboard |
 
 ## Debugging Roadmap 🧭
 
-| Performance testing | Environments | LLM Testing | Reasoning and execution testing |
-|---|---|---|---|
-|✅ Event latency analysis | 🔜 Non-stationary environment testing | 🔜 LLM non-deterministic function detection | 🚧 Infinite loops and recursive thought detection |
-|✅ Agent workflow execution pricing | 🔜 Multi-modal environments | 🚧 Token limit overflow flags | 🔜 Faulty reasoning detection |
-|🚧 Success validators (external) | 🔜 Execution containers | 🔜 Context limit overflow flags | 🔜 Generative code validators |
-|🔜 Agent controllers/skill tests | ✅ Honeypot and prompt injection detection ([PromptArmor](https://promptarmor.com)) | 🔜 API bill tracking | 🔜 Error breakpoint analysis |
-|🔜 Information context constraint testing | 🔜 Anti-agent roadblocks (i.e. Captchas) | 🔜 CI/CD integration checks | |
-|🔜 Regression testing | 🔜 Multi-agent framework visualization | | |
+| Performance testing                       | Environments                                                                        | LLM Testing                                 | Reasoning and execution testing                   |
+| ----------------------------------------- | ----------------------------------------------------------------------------------- | ------------------------------------------- | ------------------------------------------------- |
+| ✅ Event latency analysis                 | 🔜 Non-stationary environment testing                                               | 🔜 LLM non-deterministic function detection | 🚧 Infinite loops and recursive thought detection |
+| ✅ Agent workflow execution pricing       | 🔜 Multi-modal environments                                                         | 🚧 Token limit overflow flags               | 🔜 Faulty reasoning detection                     |
+| 🚧 Success validators (external)          | 🔜 Execution containers                                                             | 🔜 Context limit overflow flags             | 🔜 Generative code validators                     |
+| 🔜 Agent controllers/skill tests          | ✅ Honeypot and prompt injection detection ([PromptArmor](https://promptarmor.com)) | 🔜 API bill tracking                        | 🔜 Error breakpoint analysis                      |
+| 🔜 Information context constraint testing | 🔜 Anti-agent roadblocks (i.e. Captchas)                                            | 🔜 CI/CD integration checks                 |                                                   |
+| 🔜 Regression testing                     | 🔜 Multi-agent framework visualization                                              |                                             |                                                   |
 
 ### Why AgentOps? 🤔
 
 Our mission is to bring your agent from prototype to production.
 
-Agent developers often work with little to no visibility into agent testing performance. This means their agents never leave the lab. We're changing that. 
+Agent developers often work with little to no visibility into agent testing performance. This means their agents never leave the lab. We're changing that.
 
 AgentOps is the easiest way to evaluate, grade, and test agents. Is there a feature you'd like to see AgentOps cover? Just raise it in the issues tab, and we'll work on adding it to the roadmap.
```

#### html2text {}

```diff
@@ -1,89 +1,106 @@
-Metadata-Version: 2.1 Name: agentops Version: 0.1.9 Summary: Python SDK for
+Metadata-Version: 2.1 Name: agentops Version: 0.2.0 Summary: Python SDK for
 developing AI agent evals and observability Author-email: Alex Reibman
 gmail.com>, Shawn Qiu
 gmail.com>, Braelyn Boynton
 gmail.com>, Howard Gil
 gmail.com> Project-URL: Homepage, https://github.com/AgentOps-AI/agentops
 Project-URL: Issues, https://github.com/AgentOps-AI/agentops/issues Classifier:
 Programming Language :: Python :: 3 Classifier: License :: OSI Approved :: MIT
 License Classifier: Operating System :: OS Independent Requires-Python: >=3.7
 Description-Content-Type: text/markdown License-File: LICENSE Requires-Dist:
 requests==2.31.0 Requires-Dist: psutil==5.9.8 Requires-Dist: packaging==23.2
 Provides-Extra: dev Requires-Dist: pytest==7.4.0; extra == "dev" Requires-Dist:
 requests_mock==1.11.0; extra == "dev" Provides-Extra: langchain Requires-Dist:
-langchain>=0.0.354; extra == "langchain"
+langchain~=1.19; extra == "langchain"
                                     _[_L_o_g_o_]
                      AAII aaggeennttss ssuucckk.. WWee?â??rree ffiixxiinngg tthhaatt..
                                _[_P_y_t_h_o_n_]_[_V_e_r_s_i_o_n_]
     _ð___¦_ _T_w_i_t_t_e_r   â¢   _ð___¢_ _D_i_s_c_o_r_d   â¢   _ð____ï_¸__ _A_g_e_n_t_O_p_s   â¢   _ð___
                                  _D_o_c_u_m_e_n_t_a_t_i_o_n
 # AgentOps ðï¸ [![License: MIT](https://img.shields.io/badge/License-MIT-
 yellow.svg)](https://opensource.org/licenses/MIT) ![PyPI - Version](https://
 img.shields.io/pypi/v/agentops) _[_h_t_t_p_s_:_/_/_s_t_a_t_i_c_._p_e_p_y_._t_e_c_h_/_b_a_d_g_e_/_a_g_e_n_t_o_p_s_/_m_o_n_t_h_]
-_[_A_g_e_n_t_O_p_s_ _T_w_i_t_t_e_r_]_[_D_i_s_c_o_r_d_ _c_o_m_m_u_n_i_t_y_ _c_h_a_n_n_e_l_]_[_h_t_t_p_s_:_/_/_i_m_g_._s_h_i_e_l_d_s_._i_o_/
-_w_e_b_s_i_t_e_?_c_o_l_o_r_=_%_2_3_f_2_6_5_2_2_&_d_o_w_n___m_e_s_s_a_g_e_=_Y_%_2_0_C_o_m_b_i_n_a_t_o_r_&_l_a_b_e_l_=_N_o_t_%_2_0_B_a_c_k_e_d_%_2_0_B_y_&_l_o_g_o_=_y_c_o_m_b_i_n_a_t_o_r_&_s_t_y_l_e_=_f_l_a_t_-
-_s_q_u_a_r_e_&_u_p___m_e_s_s_a_g_e_=_Y_%_2_0_C_o_m_b_i_n_a_t_o_r_&_u_r_l_=_h_t_t_p_s_%_3_A_%_2_F_%_2_F_w_w_w_._y_c_o_m_b_i_n_a_t_o_r_._c_o_m_]_[_g_i_t
-_c_o_m_m_i_t_ _a_c_t_i_v_i_t_y_]_A_g_e_n_t_O_p_s_ _h_e_l_p_s_ _d_e_v_e_l_o_p_e_r_s_ _b_u_i_l_d_,_ _e_v_a_l_u_a_t_e_,_ _a_n_d_ _m_o_n_i_t_o_r_ _A_I
-_a_g_e_n_t_s_._ _T_o_o_l_s_ _t_o_ _b_u_i_l_d_ _a_g_e_n_t_s_ _f_r_o_m_ _p_r_o_t_o_t_y_p_e_ _t_o_ _p_r_o_d_u_c_t_i_o_n_._ _|_|_|_ _|_-_-_-_-_-_-_-_-_-_-_-_-_-_-
-_-_-_-_-_-_-_-_-_-_-_-_-_-_-_-_-_-_-_-_-_-_-_-_-_-_-_-_-_|_-_-_-_-_-_-_-_-_-_-_-_-_-_-_-_-_-_-_-_-_-_-_-_-_-_-_-_-_-_-_-_-_-_-_-_-_-_-_-_-_-_-_-_-_-_-_-_-_-_-
-_-_-_|_ _|_ _ð____ _*_*_R_e_p_l_a_y_ _A_n_a_l_y_t_i_c_s_ _a_n_d_ _D_e_b_u_g_g_i_n_g_*_*_ _|_ _S_t_e_p_-_b_y_-_s_t_e_p_ _a_g_e_n_t_ _e_x_e_c_u_t_i_o_n
-_g_r_a_p_h_s_ _|_ _|_ _ð___¸_ _*_*_L_L_M_ _C_o_s_t_ _M_a_n_a_g_e_m_e_n_t_*_*_ _|_ _T_r_a_c_k_ _s_p_e_n_d_ _w_i_t_h_ _L_L_M_ _f_o_u_n_d_a_t_i_o_n_ _m_o_d_e_l
-_p_r_o_v_i_d_e_r_s_ _|_ _|_ _ð__§_ª_ _*_*_A_g_e_n_t_ _B_e_n_c_h_m_a_r_k_i_n_g_*_*_ _|_ _T_e_s_t_ _y_o_u_r_ _a_g_e_n_t_s_ _a_g_a_i_n_s_t_ _1_,_0_0_0_+
-_e_v_a_l_s_ _|_ _|_ _ð____ _*_*_C_o_m_p_l_i_a_n_c_e_ _a_n_d_ _S_e_c_u_r_i_t_y_*_*_ _|_ _D_e_t_e_c_t_ _c_o_m_m_o_n_ _p_r_o_m_p_t_ _i_n_j_e_c_t_i_o_n_ _a_n_d
-_d_a_t_a_ _e_x_f_i_l_t_r_a_t_i_o_n_ _e_x_p_l_o_i_t_s_ _|_ _|_ _ð__¤__ _*_*_F_r_a_m_e_w_o_r_k_ _I_n_t_e_g_r_a_t_i_o_n_s_*_*_ _|_ _E_a_s_i_l_y_ _p_l_u_g_s
-_i_n_ _w_i_t_h_ _f_r_a_m_e_w_o_r_k_s_ _l_i_k_e_ _C_r_e_w_A_I_ _a_n_d_ _L_a_n_g_C_h_a_i_n_ _|_ _#_#_ _Q_u_i_c_k_ _S_t_a_r_t_ _â__¨_ï_¸__ _`_`_`_p_y_t_h_o_n
-_p_i_p_ _i_n_s_t_a_l_l_ _a_g_e_n_t_o_p_s_ _`_`_`_ _#_#_#_ _S_e_s_s_i_o_n_ _r_e_p_l_a_y_s_ _i_n_ _3_ _l_i_n_e_s_ _o_f_ _c_o_d_e_ _I_n_i_t_i_a_l_i_z_e_ _t_h_e
-_A_g_e_n_t_O_p_s_ _c_l_i_e_n_t_ _a_n_d_ _a_u_t_o_m_a_t_i_c_a_l_l_y_ _g_e_t_ _a_n_a_l_y_t_i_c_s_ _o_n_ _e_v_e_r_y_ _L_L_M_ _c_a_l_l_._ _`_`_`_p_y_t_h_o_n
-_i_m_p_o_r_t_ _a_g_e_n_t_o_p_s_ _#_ _B_e_g_i_n_n_i_n_g_ _o_f_ _p_r_o_g_r_a_m_'_s_ _c_o_d_e_ _(_i_._e_._ _m_a_i_n_._p_y_,_ _____i_n_i_t_____._p_y_)
-_a_g_e_n_t_o_p_s_._i_n_i_t_(_)_ _._._._ _#_ _(_o_p_t_i_o_n_a_l_:_ _r_e_c_o_r_d_ _s_p_e_c_i_f_i_c_ _f_u_n_c_t_i_o_n_s_)
-_@_a_g_e_n_t_o_p_s_._r_e_c_o_r_d___f_u_n_c_t_i_o_n_(_'_s_a_m_p_l_e_ _f_u_n_c_t_i_o_n_ _b_e_i_n_g_ _r_e_c_o_r_d_'_)_ _d_e_f_ _s_a_m_p_l_e___f_u_n_c_t_i_o_n
-_(_._._._)_:_ _._._._ _#_ _E_n_d_ _o_f_ _p_r_o_g_r_a_m_ _a_g_e_n_t_o_p_s_._e_n_d___s_e_s_s_i_o_n_(_'_S_u_c_c_e_s_s_'_)_ _#_ _W_o_o_h_o_o_ _Y_o_u_'_r_e
-_d_o_n_e_ _ð____ _`_`_`_ _A_l_l_ _y_o_u_r_ _s_e_s_s_i_o_n_s_ _a_r_e_ _a_v_a_i_l_a_b_l_e_ _o_n_ _t_h_e_ _[_A_g_e_n_t_O_p_s_ _d_a_s_h_b_o_a_r_d_]
-_(_h_t_t_p_s_:_/_/_a_p_p_._a_g_e_n_t_o_p_s_._a_i_?_r_e_f_=_g_h_)_._ _R_e_f_e_r_ _t_o_ _o_u_r_ _[_A_P_I_ _d_o_c_u_m_e_n_t_a_t_i_o_n_]_(_h_t_t_p_:_/_/
-_d_o_c_s_._a_g_e_n_t_o_p_s_._a_i_)_ _f_o_r_ _d_e_t_a_i_l_e_d_ _i_n_s_t_r_u_c_t_i_o_n_s_._ _A_g_e_n_t_ _D_a_s_h_b_o_a_r_d_ _[_A_g_e_n_t
-_D_a_s_h_b_o_a_r_d_]_S_e_s_s_i_o_n_ _A_n_a_l_y_t_i_c_s_ _[_S_e_s_s_i_o_n_ _A_n_a_l_y_t_i_c_s_]_S_e_s_s_i_o_n_ _R_e_p_l_a_y_s_ _[_S_e_s_s_i_o_n
-_R_e_p_l_a_y_s_]_#_#_ _I_n_t_e_g_r_a_t_i_o_n_s_ _ð__¦_¾_ _#_#_#_ _C_r_e_w_A_I_ _ð___¶_ _B_u_i_l_d_ _C_r_e_w_ _a_g_e_n_t_s_ _w_i_t_h
-_o_b_s_e_r_v_a_b_i_l_i_t_y_ _w_i_t_h_ _o_n_l_y_ _2_ _l_i_n_e_s_ _o_f_ _c_o_d_e_._ _S_i_m_p_l_y_ _s_e_t_ _a_n_ _`_A_G_E_N_T_O_P_S___A_P_I___K_E_Y_`_ _i_n
-_y_o_u_r_ _e_n_v_i_r_o_n_m_e_n_t_,_ _a_n_d_ _y_o_u_r_ _c_r_e_w_s_ _w_i_l_l_ _g_e_t_ _a_u_t_o_m_a_t_i_c_ _m_o_n_i_t_o_r_i_n_g_ _o_n_ _t_h_e_ _A_g_e_n_t_O_p_s
-_d_a_s_h_b_o_a_r_d_._ _A_g_e_n_t_O_p_s_ _i_s_ _o_f_f_i_c_i_a_l_l_y_ _s_u_p_p_o_r_t_e_d_ _o_n_ _C_r_e_w_'_s_ _l_a_t_e_s_t_ _r_c_ _b_r_a_n_c_h_:
-_`_c_r_e_w_a_i_=_=_0_._2_8_._9_r_c_1_`_ _*_ _[_A_g_e_n_t_O_p_s_ _i_n_t_e_g_r_a_t_i_o_n_ _e_x_a_m_p_l_e_]_(_h_t_t_p_s_:_/_/_d_o_c_s_._a_g_e_n_t_o_p_s_._a_i_/
-_v_1_/_i_n_t_e_g_r_a_t_i_o_n_s_/_c_r_e_w_a_i_)_ _*_ _[_O_f_f_i_c_a_l_ _C_r_e_w_A_I_ _d_o_c_u_m_e_n_t_a_t_i_o_n_]_(_h_t_t_p_s_:_/_/
-_d_o_c_s_._c_r_e_w_a_i_._c_o_m_/_h_o_w_-_t_o_/_A_g_e_n_t_O_p_s_-_O_b_s_e_r_v_a_b_i_l_i_t_y_)_ _#_#_#_ _L_a_n_g_c_h_a_i_n_ _ð__¦__ð____ _A_g_e_n_t_O_p_s
-_w_o_r_k_s_ _s_e_a_m_l_e_s_s_l_y_ _w_i_t_h_ _a_p_p_l_i_c_a_t_i_o_n_s_ _b_u_i_l_t_ _u_s_i_n_g_ _L_a_n_g_c_h_a_i_n_._ _T_o_ _u_s_e_ _t_h_e_ _h_a_n_d_l_e_r_,
-_i_n_s_t_a_l_l_ _L_a_n_g_c_h_a_i_n_ _a_s_ _a_n_ _o_p_t_i_o_n_a_l_ _d_e_p_e_n_d_e_n_c_y_:_ _`_`_`_s_h_e_l_l_ _p_i_p_ _i_n_s_t_a_l_l_ _a_g_e_n_t_o_p_s
-_[_l_a_n_g_c_h_a_i_n_]_ _`_`_`_ _T_o_ _u_s_e_ _t_h_e_ _h_a_n_d_l_e_r_,_ _i_m_p_o_r_t_ _a_n_d_ _s_e_t_ _`_`_`_p_y_t_h_o_n_ _i_m_p_o_r_t_ _o_s_ _f_r_o_m
-_l_a_n_g_c_h_a_i_n_._c_h_a_t___m_o_d_e_l_s_ _i_m_p_o_r_t_ _C_h_a_t_O_p_e_n_A_I_ _f_r_o_m_ _l_a_n_g_c_h_a_i_n_._a_g_e_n_t_s_ _i_m_p_o_r_t
-_i_n_i_t_i_a_l_i_z_e___a_g_e_n_t_,_ _A_g_e_n_t_T_y_p_e_ _f_r_o_m_ _a_g_e_n_t_o_p_s_._l_a_n_g_c_h_a_i_n___c_a_l_l_b_a_c_k___h_a_n_d_l_e_r_ _i_m_p_o_r_t
-_L_a_n_g_c_h_a_i_n_C_a_l_l_b_a_c_k_H_a_n_d_l_e_r_ _A_G_E_N_T_O_P_S___A_P_I___K_E_Y_ _=_ _o_s_._e_n_v_i_r_o_n_[_'_A_G_E_N_T_O_P_S___A_P_I___K_E_Y_'_]
-_h_a_n_d_l_e_r_ _=_ _L_a_n_g_c_h_a_i_n_C_a_l_l_b_a_c_k_H_a_n_d_l_e_r_(_a_p_i___k_e_y_=_A_G_E_N_T_O_P_S___A_P_I___K_E_Y_,_ _t_a_g_s_=_[_'_L_a_n_g_c_h_a_i_n
-_E_x_a_m_p_l_e_'_]_)_ _l_l_m_ _=_ _C_h_a_t_O_p_e_n_A_I_(_o_p_e_n_a_i___a_p_i___k_e_y_=_O_P_E_N_A_I___A_P_I___K_E_Y_,_ _c_a_l_l_b_a_c_k_s_=_[_h_a_n_d_l_e_r_]_,
-_m_o_d_e_l_=_'_g_p_t_-_3_._5_-_t_u_r_b_o_'_)_ _a_g_e_n_t_ _=_ _i_n_i_t_i_a_l_i_z_e___a_g_e_n_t_(_t_o_o_l_s_,_ _l_l_m_,
-_a_g_e_n_t_=_A_g_e_n_t_T_y_p_e_._C_H_A_T___Z_E_R_O___S_H_O_T___R_E_A_C_T___D_E_S_C_R_I_P_T_I_O_N_,_ _v_e_r_b_o_s_e_=_T_r_u_e_,_ _c_a_l_l_b_a_c_k_s_=
-_[_h_a_n_d_l_e_r_]_,_ _#_ _Y_o_u_ _m_u_s_t_ _p_a_s_s_ _i_n_ _a_ _c_a_l_l_b_a_c_k_ _h_a_n_d_l_e_r_ _t_o_ _r_e_c_o_r_d_ _y_o_u_r_ _a_g_e_n_t
-_h_a_n_d_l_e___p_a_r_s_i_n_g___e_r_r_o_r_s_=_T_r_u_e_)_ _`_`_`_ _C_h_e_c_k_ _o_u_t_ _t_h_e_ _[_L_a_n_g_c_h_a_i_n_ _E_x_a_m_p_l_e_s_ _N_o_t_e_b_o_o_k_]_(_._/
-_e_x_a_m_p_l_e_s_/_l_a_n_g_c_h_a_i_n___e_x_a_m_p_l_e_s_._i_p_y_n_b_)_ _f_o_r_ _m_o_r_e_ _d_e_t_a_i_l_s_ _i_n_c_l_u_d_i_n_g_ _A_s_y_n_c_ _h_a_n_d_l_e_r_s_.
-_#_#_#_ _L_l_a_m_a_I_n_d_e_x_ _ð__¦__ _(_C_o_m_i_n_g_ _S_o_o_n_)_ _#_#_ _T_i_m_e_ _t_r_a_v_e_l_ _d_e_b_u_g_g_i_n_g_ _ð___®_ _(_c_o_m_i_n_g_ _s_o_o_n_!_)
-_#_#_ _A_g_e_n_t_ _A_r_e_n_a_ _ð__¥__ _(_c_o_m_i_n_g_ _s_o_o_n_!_)_ _#_#_ _E_v_a_l_u_a_t_i_o_n_s_ _R_o_a_d_m_a_p_ _ð__§_­_ _|_ _P_l_a_t_f_o_r_m_ _|
-_D_a_s_h_b_o_a_r_d_ _|_ _E_v_a_l_s_ _|_ _|_-_-_-_|_-_-_-_|_-_-_-_|_ _|_â___ _P_y_t_h_o_n_ _S_D_K_ _|_ _â___ _M_u_l_t_i_-_s_e_s_s_i_o_n_ _a_n_d
-_C_r_o_s_s_-_s_e_s_s_i_o_n_ _m_e_t_r_i_c_s_ _|_ _â___ _C_u_s_t_o_m_ _e_v_a_l_ _m_e_t_r_i_c_s_ _|_ _|_ð___§_ _E_v_a_l_u_a_t_i_o_n_ _b_u_i_l_d_e_r_ _A_P_I
-_|_ _â___ _C_u_s_t_o_m_ _e_v_e_n_t_ _t_a_g_ _t_r_a_c_k_i_n_g_Â_ _|_ _ð____ _A_g_e_n_t_ _s_c_o_r_e_c_a_r_d_s_ _|_ _|_â___ _[_J_a_v_a_s_c_r_i_p_t_/
-_T_y_p_e_s_c_r_i_p_t_ _S_D_K_]_(_h_t_t_p_s_:_/_/_g_i_t_h_u_b_._c_o_m_/_A_g_e_n_t_O_p_s_-_A_I_/_a_g_e_n_t_o_p_s_-_n_o_d_e_)_ _|_ _â___ _S_e_s_s_i_o_n
-_r_e_p_l_a_y_s_|_ _ð____ _E_v_a_l_u_a_t_i_o_n_ _p_l_a_y_g_r_o_u_n_d_ _+_ _l_e_a_d_e_r_b_o_a_r_d_|_ _#_#_ _D_e_b_u_g_g_i_n_g_ _R_o_a_d_m_a_p_ _ð__§_­_ _|
-_P_e_r_f_o_r_m_a_n_c_e_ _t_e_s_t_i_n_g_ _|_ _E_n_v_i_r_o_n_m_e_n_t_s_ _|_ _L_L_M_ _T_e_s_t_i_n_g_ _|_ _R_e_a_s_o_n_i_n_g_ _a_n_d_ _e_x_e_c_u_t_i_o_n
-_t_e_s_t_i_n_g_ _|_ _|_-_-_-_|_-_-_-_|_-_-_-_|_-_-_-_|_ _|_â___ _E_v_e_n_t_ _l_a_t_e_n_c_y_ _a_n_a_l_y_s_i_s_ _|_ _ð____ _N_o_n_-_s_t_a_t_i_o_n_a_r_y
-_e_n_v_i_r_o_n_m_e_n_t_ _t_e_s_t_i_n_g_ _|_ _ð____ _L_L_M_ _n_o_n_-_d_e_t_e_r_m_i_n_i_s_t_i_c_ _f_u_n_c_t_i_o_n_ _d_e_t_e_c_t_i_o_n_ _|_ _ð___§
-_I_n_f_i_n_i_t_e_ _l_o_o_p_s_ _a_n_d_ _r_e_c_u_r_s_i_v_e_ _t_h_o_u_g_h_t_ _d_e_t_e_c_t_i_o_n_ _|_ _|_â___ _A_g_e_n_t_ _w_o_r_k_f_l_o_w_ _e_x_e_c_u_t_i_o_n
-_p_r_i_c_i_n_g_ _|_ _ð____ _M_u_l_t_i_-_m_o_d_a_l_ _e_n_v_i_r_o_n_m_e_n_t_s_ _|_ _ð___§_ _T_o_k_e_n_ _l_i_m_i_t_ _o_v_e_r_f_l_o_w_ _f_l_a_g_s_ _|
-_ð____ _F_a_u_l_t_y_ _r_e_a_s_o_n_i_n_g_ _d_e_t_e_c_t_i_o_n_ _|_ _|_ð___§_ _S_u_c_c_e_s_s_ _v_a_l_i_d_a_t_o_r_s_ _(_e_x_t_e_r_n_a_l_)_ _|_ _ð___
-_E_x_e_c_u_t_i_o_n_ _c_o_n_t_a_i_n_e_r_s_ _|_ _ð____ _C_o_n_t_e_x_t_ _l_i_m_i_t_ _o_v_e_r_f_l_o_w_ _f_l_a_g_s_ _|_ _ð____ _G_e_n_e_r_a_t_i_v_e_ _c_o_d_e
-_v_a_l_i_d_a_t_o_r_s_ _|_ _|_ð____ _A_g_e_n_t_ _c_o_n_t_r_o_l_l_e_r_s_/_s_k_i_l_l_ _t_e_s_t_s_ _|_ _â___ _H_o_n_e_y_p_o_t_ _a_n_d_ _p_r_o_m_p_t
-_i_n_j_e_c_t_i_o_n_ _d_e_t_e_c_t_i_o_n_ _(_[_P_r_o_m_p_t_A_r_m_o_r_]_(_h_t_t_p_s_:_/_/_p_r_o_m_p_t_a_r_m_o_r_._c_o_m_)_)_ _|_ _ð____ _A_P_I_ _b_i_l_l
-_t_r_a_c_k_i_n_g_ _|_ _ð____ _E_r_r_o_r_ _b_r_e_a_k_p_o_i_n_t_ _a_n_a_l_y_s_i_s_ _|_ _|_ð____ _I_n_f_o_r_m_a_t_i_o_n_ _c_o_n_t_e_x_t
-_c_o_n_s_t_r_a_i_n_t_ _t_e_s_t_i_n_g_ _|_ _ð____ _A_n_t_i_-_a_g_e_n_t_ _r_o_a_d_b_l_o_c_k_s_ _(_i_._e_._ _C_a_p_t_c_h_a_s_)_ _|_ _ð____ _C_I_/_C_D
-_i_n_t_e_g_r_a_t_i_o_n_ _c_h_e_c_k_s_ _|_ _|_ _|_ð____ _R_e_g_r_e_s_s_i_o_n_ _t_e_s_t_i_n_g_ _|_ _ð____ _M_u_l_t_i_-_a_g_e_n_t_ _f_r_a_m_e_w_o_r_k
-_v_i_s_u_a_l_i_z_a_t_i_o_n_ _|_ _|_ _|_ _#_#_#_ _W_h_y_ _A_g_e_n_t_O_p_s_?_ _ð__¤__ _O_u_r_ _m_i_s_s_i_o_n_ _i_s_ _t_o_ _b_r_i_n_g_ _y_o_u_r_ _a_g_e_n_t
-_f_r_o_m_ _p_r_o_t_o_t_y_p_e_ _t_o_ _p_r_o_d_u_c_t_i_o_n_._ _A_g_e_n_t_ _d_e_v_e_l_o_p_e_r_s_ _o_f_t_e_n_ _w_o_r_k_ _w_i_t_h_ _l_i_t_t_l_e_ _t_o_ _n_o
-_v_i_s_i_b_i_l_i_t_y_ _i_n_t_o_ _a_g_e_n_t_ _t_e_s_t_i_n_g_ _p_e_r_f_o_r_m_a_n_c_e_._ _T_h_i_s_ _m_e_a_n_s_ _t_h_e_i_r_ _a_g_e_n_t_s_ _n_e_v_e_r_ _l_e_a_v_e
-_t_h_e_ _l_a_b_._ _W_e_'_r_e_ _c_h_a_n_g_i_n_g_ _t_h_a_t_._ _A_g_e_n_t_O_p_s_ _i_s_ _t_h_e_ _e_a_s_i_e_s_t_ _w_a_y_ _t_o_ _e_v_a_l_u_a_t_e_,_ _g_r_a_d_e_,
-_a_n_d_ _t_e_s_t_ _a_g_e_n_t_s_._ _I_s_ _t_h_e_r_e_ _a_ _f_e_a_t_u_r_e_ _y_o_u_'_d_ _l_i_k_e_ _t_o_ _s_e_e_ _A_g_e_n_t_O_p_s_ _c_o_v_e_r_?_ _J_u_s_t
-_r_a_i_s_e_ _i_t_ _i_n_ _t_h_e_ _i_s_s_u_e_s_ _t_a_b_,_ _a_n_d_ _w_e_'_l_l_ _w_o_r_k_ _o_n_ _a_d_d_i_n_g_ _i_t_ _t_o_ _t_h_e_ _r_o_a_d_m_a_p_.
+_[_A_g_e_n_t_O_p_s_ _T_w_i_t_t_e_r_]_[_D_i_s_c_o_r_d_ _c_o_m_m_u_n_i_t_y_ _c_h_a_n_n_e_l_]_[_g_i_t_ _c_o_m_m_i_t_ _a_c_t_i_v_i_t_y_]AgentOps
+helps developers build, evaluate, and monitor AI agents. Tools to build agents
+from prototype to production. | | | | ------------------------------------- | -
+------------------------------------------------------------ | | ð **Replay
+Analytics and Debugging** | Step-by-step agent execution graphs | | ð¸ **LLM
+Cost Management** | Track spend with LLM foundation model providers | | ð§ª
+**Agent Benchmarking** | Test your agents against 1,000+ evals | | ð
+**Compliance and Security** | Detect common prompt injection and data
+exfiltration exploits | | ð¤ **Framework Integrations** | Easily plugs in
+with frameworks like CrewAI and LangChain | ## Quick Start â¨ï¸ ```bash pip
+install agentops ``` ### Session replays in 3 lines of code Initialize the
+AgentOps client and automatically get analytics on every LLM call. ```python
+import agentops # Beginning of program's code (i.e. main.py, __init__.py)
+agentops.init() ... # (optional: record specific functions)
+@agentops.record_function('sample function being record') def sample_function
+(...): ... # End of program agentops.end_session('Success') # Woohoo You're
+done ð ``` All your sessions are available on the [AgentOps dashboard]
+(https://app.agentops.ai?ref=gh). Refer to our [API documentation](http://
+docs.agentops.ai) for detailed instructions. Agent Dashboard _[_A_g_e_n_t
+_D_a_s_h_b_o_a_r_d_]Session Analytics _[_S_e_s_s_i_o_n_ _A_n_a_l_y_t_i_c_s_]Session Replays _[_S_e_s_s_i_o_n
+_R_e_p_l_a_y_s_]## Integrations ð¦¾ ### CrewAI ð¶ Build Crew agents with
+observability with only 2 lines of code. Simply set an `AGENTOPS_API_KEY` in
+your environment, and your crews will get automatic monitoring on the AgentOps
+dashboard. AgentOps is integrated with CrewAI on a pre-release fork. Install
+crew with ```bash pip install git+https://github.com/AgentOps-AI/
+crewAI.git@main ``` - [AgentOps integration example](https://docs.agentops.ai/
+v1/integrations/crewai) - [Official CrewAI documentation](https://
+docs.crewai.com/how-to/AgentOps-Observability) ### Langchain ð¦ð AgentOps
+works seamlessly with applications built using Langchain. To use the handler,
+install Langchain as an optional dependency: Installation ```shell pip install
+agentops[langchain] ``` To use the handler, import and set ```python import os
+from langchain.chat_models import ChatOpenAI from langchain.agents import
+initialize_agent, AgentType from agentops.langchain_callback_handler import
+LangchainCallbackHandler AGENTOPS_API_KEY = os.environ['AGENTOPS_API_KEY']
+handler = LangchainCallbackHandler(api_key=AGENTOPS_API_KEY, tags=['Langchain
+Example']) llm = ChatOpenAI(openai_api_key=OPENAI_API_KEY, callbacks=[handler],
+model='gpt-3.5-turbo') agent = initialize_agent(tools, llm,
+agent=AgentType.CHAT_ZERO_SHOT_REACT_DESCRIPTION, verbose=True, callbacks=
+[handler], # You must pass in a callback handler to record your agent
+handle_parsing_errors=True) ``` Check out the [Langchain Examples Notebook](./
+examples/langchain_examples.ipynb) for more details including Async handlers.
+### Cohere â¨ï¸ First class support for Cohere(>=5.4.0). This is a living
+integration, should you need any added functionality please message us on
+Discord! - [AgentOps integration example](https://docs.agentops.ai/v1/
+integrations/cohere) - [Official Cohere documentation](https://docs.cohere.com/
+reference/about) Installation ```bash pip install cohere ``` ```python python
+import cohere import agentops # Beginning of program's code (i.e. main.py,
+__init__.py) agentops.init() co = cohere.Client() chat = co.chat( message="Is
+it pronounced ceaux-hear or co-hehray?" ) print(chat) agentops.end_session
+('Success') ``` ```python python import cohere import agentops # Beginning of
+program's code (i.e. main.py, __init__.py) agentops.init() co = cohere.Client()
+stream = co.chat_stream( message="Write me a haiku about the synergies between
+Cohere and AgentOps" ) for event in stream: if event.event_type == "text-
+generation": print(event.text, end='') agentops.end_session('Success') ``` ###
+LlamaIndex ð¦ (Coming Soon) ## Time travel debugging ð® (coming soon!) ##
+Agent Arena ð¥ (coming soon!) ## Evaluations Roadmap ð§­ | Platform |
+Dashboard | Evals | | ---------------------------------------------------------
+------------------- | ------------------------------------------ | ------------
+-------------------------- | | â Python SDK | â Multi-session and Cross-
+session metrics | â Custom eval metrics | | ð§ Evaluation builder API | â
+Custom event tag trackingÂ  | ð Agent scorecards | | â [Javascript/
+Typescript SDK](https://github.com/AgentOps-AI/agentops-node) | â Session
+replays | ð Evaluation playground + leaderboard | ## Debugging Roadmap ð§­
+| Performance testing | Environments | LLM Testing | Reasoning and execution
+testing | | ----------------------------------------- | -----------------------
+------------------------------------------------------------ | ----------------
+--------------------------- | ------------------------------------------------
+- | | â Event latency analysis | ð Non-stationary environment testing |
+ð LLM non-deterministic function detection | ð§ Infinite loops and
+recursive thought detection | | â Agent workflow execution pricing | ð
+Multi-modal environments | ð§ Token limit overflow flags | ð Faulty
+reasoning detection | | ð§ Success validators (external) | ð Execution
+containers | ð Context limit overflow flags | ð Generative code
+validators | | ð Agent controllers/skill tests | â Honeypot and prompt
+injection detection ([PromptArmor](https://promptarmor.com)) | ð API bill
+tracking | ð Error breakpoint analysis | | ð Information context
+constraint testing | ð Anti-agent roadblocks (i.e. Captchas) | ð CI/CD
+integration checks | | | ð Regression testing | ð Multi-agent framework
+visualization | | | ### Why AgentOps? ð¤ Our mission is to bring your agent
+from prototype to production. Agent developers often work with little to no
+visibility into agent testing performance. This means their agents never leave
+the lab. We're changing that. AgentOps is the easiest way to evaluate, grade,
+and test agents. Is there a feature you'd like to see AgentOps cover? Just
+raise it in the issues tab, and we'll work on adding it to the roadmap.
```

### Comparing `agentops-0.1.9/agentops.egg-info/SOURCES.txt` & `agentops-0.2.0/agentops.egg-info/SOURCES.txt`

 * *Files 6% similar despite different names*

```diff
@@ -18,13 +18,15 @@
 agentops/session.py
 agentops/worker.py
 agentops.egg-info/PKG-INFO
 agentops.egg-info/SOURCES.txt
 agentops.egg-info/dependency_links.txt
 agentops.egg-info/requires.txt
 agentops.egg-info/top_level.txt
+agentops/partners/autogen_logger.py
+agentops/partners/langchain_callback_handler.py
 tests/test_canary.py
 tests/test_events.py
 tests/test_patcher.py
 tests/test_record_function.py
 tests/test_session.py
 tests/test_teardown.py
```

### Comparing `agentops-0.1.9/pyproject.toml` & `agentops-0.2.0/pyproject.toml`

 * *Files 10% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["setuptools>=61.0", "wheel"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "agentops"
-version = "0.1.9"
+version = "0.2.0"
 authors = [
   { name="Alex Reibman", email="areibman@gmail.com" },
   { name="Shawn Qiu", email="siyangqiu@gmail.com" },
   { name="Braelyn Boynton", email="bboynton97@gmail.com" },
   { name="Howard Gil", email="howardbgil@gmail.com" }
 ]
 description = "Python SDK for developing AI agent evals and observability"
@@ -26,13 +26,16 @@
 ]
 [project.optional-dependencies]
 dev = [
     "pytest==7.4.0",
     "requests_mock==1.11.0"
 ]
 langchain = [
-    "langchain>=0.0.354"
+    "langchain~=1.19"
 ]
 
 [project.urls]
 Homepage = "https://github.com/AgentOps-AI/agentops"
 Issues = "https://github.com/AgentOps-AI/agentops/issues"
+
+[tool.autopep8]
+max_line_length = 120
```

### Comparing `agentops-0.1.9/tests/test_patcher.py` & `agentops-0.2.0/tests/test_patcher.py`

 * *Files identical despite different names*

### Comparing `agentops-0.1.9/tests/test_record_function.py` & `agentops-0.2.0/tests/test_record_function.py`

 * *Files 24% similar despite different names*

```diff
@@ -1,27 +1,33 @@
 import pytest
 import requests_mock
 import time
 import agentops
 from agentops import record_function
 from datetime import datetime
 
+
 @pytest.fixture
 def mock_req():
     with requests_mock.Mocker() as m:
-        url = 'https://api.agentops.ai'
-        m.post(url + '/events', text='ok')
-        m.post(url + '/sessions', json={'status': 'success', 'token_cost': 5})
+        url = "https://api.agentops.ai"
+        m.post(url + "/v2/create_events", text="ok")
+        m.post(
+            url + "/v2/create_session", json={"status": "success", "jwt": "some_jwt"}
+        )
+        m.post(url + "/v2/update_session", json={"status": "success", "token_cost": 5})
+        m.post(url + "/v2/developer_errors", text="ok")
         yield m
 
+
 class TestRecordAction:
     def setup_method(self):
-        self.url = 'https://api.agentops.ai'
+        self.url = "https://api.agentops.ai"
         self.api_key = "random_api_key"
-        self.event_type = 'test_event_type'
+        self.event_type = "test_event_type"
         agentops.init(self.api_key, max_wait_time=5, auto_start_session=False)
 
     def test_record_function_decorator(self, mock_req):
         agentops.start_session()
 
         @record_function(event_name=self.event_type)
         def add_two(x, y):
@@ -29,21 +35,21 @@
 
         # Act
         add_two(3, 4)
         time.sleep(0.1)
 
         # Assert
         assert len(mock_req.request_history) == 2
-        assert mock_req.last_request.headers['X-Agentops-Auth'] == self.api_key
+        assert mock_req.last_request.headers["X-Agentops-Api-Key"] == self.api_key
         request_json = mock_req.last_request.json()
-        assert request_json['events'][0]['action_type'] == self.event_type
-        assert request_json['events'][0]['params'] == {'x': 3, 'y': 4}
-        assert request_json['events'][0]['returns'] == 7
+        assert request_json["events"][0]["action_type"] == self.event_type
+        assert request_json["events"][0]["params"] == {"x": 3, "y": 4}
+        assert request_json["events"][0]["returns"] == 7
 
-        agentops.end_session(end_state='Success')
+        agentops.end_session(end_state="Success")
 
     def test_record_function_decorator_multiple(self, mock_req):
         agentops.start_session()
 
         # Arrange
         @record_function(event_name=self.event_type)
         def add_three(x, y, z=3):
@@ -53,21 +59,21 @@
         add_three(1, 2)
         time.sleep(0.1)
         add_three(1, 2)
         time.sleep(0.1)
 
         # Assert
         assert len(mock_req.request_history) == 3
-        assert mock_req.last_request.headers['X-Agentops-Auth'] == self.api_key
+        assert mock_req.last_request.headers["X-Agentops-Api-Key"] == self.api_key
         request_json = mock_req.last_request.json()
-        assert request_json['events'][0]['action_type'] == self.event_type
-        assert request_json['events'][0]['params'] == {'x': 1, 'y': 2, 'z': 3}
-        assert request_json['events'][0]['returns'] == 6
+        assert request_json["events"][0]["action_type"] == self.event_type
+        assert request_json["events"][0]["params"] == {"x": 1, "y": 2, "z": 3}
+        assert request_json["events"][0]["returns"] == 6
 
-        agentops.end_session(end_state='Success')
+        agentops.end_session(end_state="Success")
 
     @pytest.mark.asyncio
     async def test_async_function_call(self, mock_req):
         agentops.start_session()
 
         @record_function(self.event_type)
         async def async_add(x, y):
@@ -78,20 +84,22 @@
         result = await async_add(3, 4)
         time.sleep(0.1)
 
         # Assert
         assert result == 7
         # Assert
         assert len(mock_req.request_history) == 2
-        assert mock_req.last_request.headers['X-Agentops-Auth'] == self.api_key
+        assert mock_req.last_request.headers["X-Agentops-Api-Key"] == self.api_key
         request_json = mock_req.last_request.json()
-        assert request_json['events'][0]['action_type'] == self.event_type
-        assert request_json['events'][0]['params'] == {'x': 3, 'y': 4}
-        assert request_json['events'][0]['returns'] == 7
+        assert request_json["events"][0]["action_type"] == self.event_type
+        assert request_json["events"][0]["params"] == {"x": 3, "y": 4}
+        assert request_json["events"][0]["returns"] == 7
         init = datetime.fromisoformat(
-            request_json['events'][0]['init_timestamp'].replace('Z', '+00:00'))
+            request_json["events"][0]["init_timestamp"].replace("Z", "+00:00")
+        )
         end = datetime.fromisoformat(
-            request_json['events'][0]['end_timestamp'].replace('Z', '+00:00'))
+            request_json["events"][0]["end_timestamp"].replace("Z", "+00:00")
+        )
 
         assert (end - init).total_seconds() >= 0.1
 
-        agentops.end_session(end_state='Success')
+        agentops.end_session(end_state="Success")
```

