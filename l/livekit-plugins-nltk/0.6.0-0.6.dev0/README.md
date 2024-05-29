# Comparing `tmp/livekit_plugins_nltk-0.6.0.tar.gz` & `tmp/livekit_plugins_nltk-0.6.dev0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "livekit_plugins_nltk-0.6.0.tar", last modified: Wed May 29 21:33:40 2024, max compression
+gzip compressed data, was "livekit_plugins_nltk-0.6.dev0.tar", last modified: Thu May 23 15:59:23 2024, max compression
```

## Comparing `livekit_plugins_nltk-0.6.0.tar` & `livekit_plugins_nltk-0.6.dev0.tar`

### file list

```diff
@@ -1,20 +1,20 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-29 21:33:40.123793 livekit_plugins_nltk-0.6.0/
--rw-r--r--   0 runner    (1001) docker     (127)     1179 2024-05-29 21:33:40.123793 livekit_plugins_nltk-0.6.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      210 2024-05-29 21:33:32.000000 livekit_plugins_nltk-0.6.0/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-29 21:33:40.119793 livekit_plugins_nltk-0.6.0/livekit/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-29 21:33:40.119793 livekit_plugins_nltk-0.6.0/livekit/plugins/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-29 21:33:40.119793 livekit_plugins_nltk-0.6.0/livekit/plugins/nltk/
--rw-r--r--   0 runner    (1001) docker     (127)     1096 2024-05-29 21:33:32.000000 livekit_plugins_nltk-0.6.0/livekit/plugins/nltk/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)       67 2024-05-29 21:33:32.000000 livekit_plugins_nltk-0.6.0/livekit/plugins/nltk/log.py
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-29 21:33:32.000000 livekit_plugins_nltk-0.6.0/livekit/plugins/nltk/py.typed
--rw-r--r--   0 runner    (1001) docker     (127)     2211 2024-05-29 21:33:32.000000 livekit_plugins_nltk-0.6.0/livekit/plugins/nltk/sentence_tokenizer.py
--rw-r--r--   0 runner    (1001) docker     (127)      600 2024-05-29 21:33:32.000000 livekit_plugins_nltk-0.6.0/livekit/plugins/nltk/version.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-29 21:33:40.123793 livekit_plugins_nltk-0.6.0/livekit_plugins_nltk.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     1179 2024-05-29 21:33:40.000000 livekit_plugins_nltk-0.6.0/livekit_plugins_nltk.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      418 2024-05-29 21:33:40.000000 livekit_plugins_nltk-0.6.0/livekit_plugins_nltk.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-29 21:33:40.000000 livekit_plugins_nltk-0.6.0/livekit_plugins_nltk.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       47 2024-05-29 21:33:40.000000 livekit_plugins_nltk-0.6.0/livekit_plugins_nltk.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)        8 2024-05-29 21:33:40.000000 livekit_plugins_nltk-0.6.0/livekit_plugins_nltk.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)       86 2024-05-29 21:33:32.000000 livekit_plugins_nltk-0.6.0/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-29 21:33:40.123793 livekit_plugins_nltk-0.6.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)     2170 2024-05-29 21:33:32.000000 livekit_plugins_nltk-0.6.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-23 15:59:23.714461 livekit_plugins_nltk-0.6.dev0/
+-rw-r--r--   0 runner    (1001) docker     (127)     1185 2024-05-23 15:59:23.714461 livekit_plugins_nltk-0.6.dev0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      210 2024-05-23 15:59:19.000000 livekit_plugins_nltk-0.6.dev0/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-23 15:59:23.710461 livekit_plugins_nltk-0.6.dev0/livekit/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-23 15:59:23.710461 livekit_plugins_nltk-0.6.dev0/livekit/plugins/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-23 15:59:23.714461 livekit_plugins_nltk-0.6.dev0/livekit/plugins/nltk/
+-rw-r--r--   0 runner    (1001) docker     (127)     1096 2024-05-23 15:59:19.000000 livekit_plugins_nltk-0.6.dev0/livekit/plugins/nltk/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)       67 2024-05-23 15:59:19.000000 livekit_plugins_nltk-0.6.dev0/livekit/plugins/nltk/log.py
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-23 15:59:19.000000 livekit_plugins_nltk-0.6.dev0/livekit/plugins/nltk/py.typed
+-rw-r--r--   0 runner    (1001) docker     (127)     2211 2024-05-23 15:59:19.000000 livekit_plugins_nltk-0.6.dev0/livekit/plugins/nltk/sentence_tokenizer.py
+-rw-r--r--   0 runner    (1001) docker     (127)      603 2024-05-23 15:59:19.000000 livekit_plugins_nltk-0.6.dev0/livekit/plugins/nltk/version.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-23 15:59:23.714461 livekit_plugins_nltk-0.6.dev0/livekit_plugins_nltk.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     1185 2024-05-23 15:59:23.000000 livekit_plugins_nltk-0.6.dev0/livekit_plugins_nltk.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      418 2024-05-23 15:59:23.000000 livekit_plugins_nltk-0.6.dev0/livekit_plugins_nltk.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-23 15:59:23.000000 livekit_plugins_nltk-0.6.dev0/livekit_plugins_nltk.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       50 2024-05-23 15:59:23.000000 livekit_plugins_nltk-0.6.dev0/livekit_plugins_nltk.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        8 2024-05-23 15:59:23.000000 livekit_plugins_nltk-0.6.dev0/livekit_plugins_nltk.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       86 2024-05-23 15:59:19.000000 livekit_plugins_nltk-0.6.dev0/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-23 15:59:23.714461 livekit_plugins_nltk-0.6.dev0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)     2173 2024-05-23 15:59:19.000000 livekit_plugins_nltk-0.6.dev0/setup.py
```

### Comparing `livekit_plugins_nltk-0.6.0/PKG-INFO` & `livekit_plugins_nltk-0.6.dev0/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: livekit-plugins-nltk
-Version: 0.6.0
+Version: 0.6.dev0
 Summary: Agent Framework plugin for NLTK-based text processing.
 Home-page: https://github.com/livekit/agents
 License: Apache-2.0
 Project-URL: Documentation, https://docs.livekit.io
 Project-URL: Website, https://livekit.io/
 Project-URL: Source, https://github.com/livekit/agents
 Keywords: webrtc,realtime,audio,video,livekit
@@ -16,15 +16,15 @@
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3 :: Only
 Requires-Python: >=3.9.0
 Description-Content-Type: text/markdown
 Requires-Dist: livekit~=0.11
 Requires-Dist: nltk<4,>=3
-Requires-Dist: livekit-agents~=0.7.0
+Requires-Dist: livekit-agents~=0.7.dev0
 
 # LiveKit Plugins NLTK
 
 Agent Framework plugin for [NLTK](https://www.nltk.org/)-based text processing. Currently featuring a `SentenceTokenizer`.
 
 ## Installation
```

### Comparing `livekit_plugins_nltk-0.6.0/livekit/plugins/nltk/__init__.py` & `livekit_plugins_nltk-0.6.dev0/livekit/plugins/nltk/__init__.py`

 * *Files identical despite different names*

### Comparing `livekit_plugins_nltk-0.6.0/livekit/plugins/nltk/sentence_tokenizer.py` & `livekit_plugins_nltk-0.6.dev0/livekit/plugins/nltk/sentence_tokenizer.py`

 * *Files identical despite different names*

### Comparing `livekit_plugins_nltk-0.6.0/livekit/plugins/nltk/version.py` & `livekit_plugins_nltk-0.6.dev0/livekit/plugins/nltk/version.py`

 * *Files 2% similar despite different names*

```diff
@@ -8,8 +8,8 @@
 #
 # Unless required by applicable law or agreed to in writing, software
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 
-__version__ = "0.6.0"
+__version__ = "0.6.dev0"
```

### Comparing `livekit_plugins_nltk-0.6.0/livekit_plugins_nltk.egg-info/PKG-INFO` & `livekit_plugins_nltk-0.6.dev0/livekit_plugins_nltk.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: livekit-plugins-nltk
-Version: 0.6.0
+Version: 0.6.dev0
 Summary: Agent Framework plugin for NLTK-based text processing.
 Home-page: https://github.com/livekit/agents
 License: Apache-2.0
 Project-URL: Documentation, https://docs.livekit.io
 Project-URL: Website, https://livekit.io/
 Project-URL: Source, https://github.com/livekit/agents
 Keywords: webrtc,realtime,audio,video,livekit
@@ -16,15 +16,15 @@
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3 :: Only
 Requires-Python: >=3.9.0
 Description-Content-Type: text/markdown
 Requires-Dist: livekit~=0.11
 Requires-Dist: nltk<4,>=3
-Requires-Dist: livekit-agents~=0.7.0
+Requires-Dist: livekit-agents~=0.7.dev0
 
 # LiveKit Plugins NLTK
 
 Agent Framework plugin for [NLTK](https://www.nltk.org/)-based text processing. Currently featuring a `SentenceTokenizer`.
 
 ## Installation
```

### Comparing `livekit_plugins_nltk-0.6.0/setup.py` & `livekit_plugins_nltk-0.6.dev0/setup.py`

 * *Files 4% similar despite different names*

```diff
@@ -45,15 +45,15 @@
     keywords=["webrtc", "realtime", "audio", "video", "livekit"],
     license="Apache-2.0",
     packages=setuptools.find_namespace_packages(include=["livekit.*"]),
     python_requires=">=3.9.0",
     install_requires=[
         "livekit~=0.11",
         "nltk >= 3, < 4",
-        "livekit-agents~=0.7.0",
+        "livekit-agents~=0.7.dev0",
     ],
     package_data={
         "livekit.plugins.nltk": ["py.typed"],
     },
     project_urls={
         "Documentation": "https://docs.livekit.io",
         "Website": "https://livekit.io/",
```

