# Comparing `tmp/livekit_plugins_deepgram-0.5.0.tar.gz` & `tmp/livekit_plugins_deepgram-0.5.dev0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "livekit_plugins_deepgram-0.5.0.tar", last modified: Wed May 29 21:33:26 2024, max compression
+gzip compressed data, was "livekit_plugins_deepgram-0.5.dev0.tar", last modified: Thu May 23 15:59:09 2024, max compression
```

## Comparing `livekit_plugins_deepgram-0.5.0.tar` & `livekit_plugins_deepgram-0.5.dev0.tar`

### file list

```diff
@@ -1,21 +1,21 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-29 21:33:26.361626 livekit_plugins_deepgram-0.5.0/
--rw-r--r--   0 runner    (1001) docker     (127)     1365 2024-05-29 21:33:26.361626 livekit_plugins_deepgram-0.5.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      337 2024-05-29 21:33:22.000000 livekit_plugins_deepgram-0.5.0/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-29 21:33:26.357626 livekit_plugins_deepgram-0.5.0/livekit/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-29 21:33:26.357626 livekit_plugins_deepgram-0.5.0/livekit/plugins/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-29 21:33:26.361626 livekit_plugins_deepgram-0.5.0/livekit/plugins/deepgram/
--rw-r--r--   0 runner    (1001) docker     (127)      373 2024-05-29 21:33:22.000000 livekit_plugins_deepgram-0.5.0/livekit/plugins/deepgram/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)       71 2024-05-29 21:33:22.000000 livekit_plugins_deepgram-0.5.0/livekit/plugins/deepgram/log.py
--rw-r--r--   0 runner    (1001) docker     (127)     1165 2024-05-29 21:33:22.000000 livekit_plugins_deepgram-0.5.0/livekit/plugins/deepgram/models.py
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-29 21:33:22.000000 livekit_plugins_deepgram-0.5.0/livekit/plugins/deepgram/py.typed
--rw-r--r--   0 runner    (1001) docker     (127)    16732 2024-05-29 21:33:22.000000 livekit_plugins_deepgram-0.5.0/livekit/plugins/deepgram/stt.py
--rw-r--r--   0 runner    (1001) docker     (127)      600 2024-05-29 21:33:22.000000 livekit_plugins_deepgram-0.5.0/livekit/plugins/deepgram/version.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-29 21:33:26.361626 livekit_plugins_deepgram-0.5.0/livekit_plugins_deepgram.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     1365 2024-05-29 21:33:26.000000 livekit_plugins_deepgram-0.5.0/livekit_plugins_deepgram.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      478 2024-05-29 21:33:26.000000 livekit_plugins_deepgram-0.5.0/livekit_plugins_deepgram.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-29 21:33:26.000000 livekit_plugins_deepgram-0.5.0/livekit_plugins_deepgram.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       51 2024-05-29 21:33:26.000000 livekit_plugins_deepgram-0.5.0/livekit_plugins_deepgram.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)        8 2024-05-29 21:33:26.000000 livekit_plugins_deepgram-0.5.0/livekit_plugins_deepgram.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)       86 2024-05-29 21:33:22.000000 livekit_plugins_deepgram-0.5.0/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-29 21:33:26.361626 livekit_plugins_deepgram-0.5.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)     2236 2024-05-29 21:33:22.000000 livekit_plugins_deepgram-0.5.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-23 15:59:09.533347 livekit_plugins_deepgram-0.5.dev0/
+-rw-r--r--   0 runner    (1001) docker     (127)     1371 2024-05-23 15:59:09.533347 livekit_plugins_deepgram-0.5.dev0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      337 2024-05-23 15:59:05.000000 livekit_plugins_deepgram-0.5.dev0/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-23 15:59:09.529346 livekit_plugins_deepgram-0.5.dev0/livekit/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-23 15:59:09.529346 livekit_plugins_deepgram-0.5.dev0/livekit/plugins/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-23 15:59:09.533347 livekit_plugins_deepgram-0.5.dev0/livekit/plugins/deepgram/
+-rw-r--r--   0 runner    (1001) docker     (127)      373 2024-05-23 15:59:05.000000 livekit_plugins_deepgram-0.5.dev0/livekit/plugins/deepgram/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)       71 2024-05-23 15:59:05.000000 livekit_plugins_deepgram-0.5.dev0/livekit/plugins/deepgram/log.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1165 2024-05-23 15:59:05.000000 livekit_plugins_deepgram-0.5.dev0/livekit/plugins/deepgram/models.py
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-23 15:59:05.000000 livekit_plugins_deepgram-0.5.dev0/livekit/plugins/deepgram/py.typed
+-rw-r--r--   0 runner    (1001) docker     (127)    16732 2024-05-23 15:59:05.000000 livekit_plugins_deepgram-0.5.dev0/livekit/plugins/deepgram/stt.py
+-rw-r--r--   0 runner    (1001) docker     (127)      603 2024-05-23 15:59:05.000000 livekit_plugins_deepgram-0.5.dev0/livekit/plugins/deepgram/version.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-23 15:59:09.533347 livekit_plugins_deepgram-0.5.dev0/livekit_plugins_deepgram.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     1371 2024-05-23 15:59:09.000000 livekit_plugins_deepgram-0.5.dev0/livekit_plugins_deepgram.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      478 2024-05-23 15:59:09.000000 livekit_plugins_deepgram-0.5.dev0/livekit_plugins_deepgram.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-23 15:59:09.000000 livekit_plugins_deepgram-0.5.dev0/livekit_plugins_deepgram.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       54 2024-05-23 15:59:09.000000 livekit_plugins_deepgram-0.5.dev0/livekit_plugins_deepgram.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        8 2024-05-23 15:59:09.000000 livekit_plugins_deepgram-0.5.dev0/livekit_plugins_deepgram.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       86 2024-05-23 15:59:05.000000 livekit_plugins_deepgram-0.5.dev0/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-23 15:59:09.533347 livekit_plugins_deepgram-0.5.dev0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)     2239 2024-05-23 15:59:05.000000 livekit_plugins_deepgram-0.5.dev0/setup.py
```

### Comparing `livekit_plugins_deepgram-0.5.0/PKG-INFO` & `livekit_plugins_deepgram-0.5.dev0/PKG-INFO`

 * *Files 9% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: livekit-plugins-deepgram
-Version: 0.5.0
+Version: 0.5.dev0
 Summary: Agent Framework plugin for services using DeepGram's API.
 Home-page: https://github.com/livekit/agents
 License: Apache-2.0
 Project-URL: Documentation, https://docs.livekit.io
 Project-URL: Website, https://livekit.io/
 Project-URL: Source, https://github.com/livekit/agents
 Keywords: webrtc,realtime,audio,video,livekit
@@ -16,15 +16,15 @@
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3 :: Only
 Requires-Python: >=3.9.0
 Description-Content-Type: text/markdown
 Requires-Dist: livekit~=0.11
-Requires-Dist: livekit-agents~=0.7.0
+Requires-Dist: livekit-agents~=0.7.dev0
 Requires-Dist: aiohttp>=3.7.4
 
 # LiveKit Plugins DeepGram
 
 Agent Framework plugin for speech-to-text with [DeepGram](https://deepgram.com/)'s API. Currently supports speech-to-text.
 
 ## Installation
```

### Comparing `livekit_plugins_deepgram-0.5.0/livekit/plugins/deepgram/models.py` & `livekit_plugins_deepgram-0.5.dev0/livekit/plugins/deepgram/models.py`

 * *Files identical despite different names*

### Comparing `livekit_plugins_deepgram-0.5.0/livekit/plugins/deepgram/stt.py` & `livekit_plugins_deepgram-0.5.dev0/livekit/plugins/deepgram/stt.py`

 * *Files identical despite different names*

### Comparing `livekit_plugins_deepgram-0.5.0/livekit/plugins/deepgram/version.py` & `livekit_plugins_deepgram-0.5.dev0/livekit/plugins/deepgram/version.py`

 * *Files 1% similar despite different names*

```diff
@@ -8,8 +8,8 @@
 #
 # Unless required by applicable law or agreed to in writing, software
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 
-__version__ = "0.5.0"
+__version__ = "0.5.dev0"
```

### Comparing `livekit_plugins_deepgram-0.5.0/livekit_plugins_deepgram.egg-info/PKG-INFO` & `livekit_plugins_deepgram-0.5.dev0/livekit_plugins_deepgram.egg-info/PKG-INFO`

 * *Files 9% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: livekit-plugins-deepgram
-Version: 0.5.0
+Version: 0.5.dev0
 Summary: Agent Framework plugin for services using DeepGram's API.
 Home-page: https://github.com/livekit/agents
 License: Apache-2.0
 Project-URL: Documentation, https://docs.livekit.io
 Project-URL: Website, https://livekit.io/
 Project-URL: Source, https://github.com/livekit/agents
 Keywords: webrtc,realtime,audio,video,livekit
@@ -16,15 +16,15 @@
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3 :: Only
 Requires-Python: >=3.9.0
 Description-Content-Type: text/markdown
 Requires-Dist: livekit~=0.11
-Requires-Dist: livekit-agents~=0.7.0
+Requires-Dist: livekit-agents~=0.7.dev0
 Requires-Dist: aiohttp>=3.7.4
 
 # LiveKit Plugins DeepGram
 
 Agent Framework plugin for speech-to-text with [DeepGram](https://deepgram.com/)'s API. Currently supports speech-to-text.
 
 ## Installation
```

### Comparing `livekit_plugins_deepgram-0.5.0/setup.py` & `livekit_plugins_deepgram-0.5.dev0/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -45,15 +45,15 @@
     ],
     keywords=["webrtc", "realtime", "audio", "video", "livekit"],
     license="Apache-2.0",
     packages=setuptools.find_namespace_packages(include=["livekit.*"]),
     python_requires=">=3.9.0",
     install_requires=[
         "livekit ~= 0.11",
-        "livekit-agents~=0.7.0",
+        "livekit-agents~=0.7.dev0",
         "aiohttp >= 3.7.4",
     ],
     package_data={
         "livekit.plugins.deepgram": ["py.typed"],
     },
     project_urls={
         "Documentation": "https://docs.livekit.io",
```

