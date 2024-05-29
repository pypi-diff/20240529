# Comparing `tmp/livekit_plugins_google-0.5.0.tar.gz` & `tmp/livekit_plugins_google-0.5.dev0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "livekit_plugins_google-0.5.0.tar", last modified: Wed May 29 21:33:32 2024, max compression
+gzip compressed data, was "livekit_plugins_google-0.5.dev0.tar", last modified: Thu May 23 15:59:24 2024, max compression
```

## Comparing `livekit_plugins_google-0.5.0.tar` & `livekit_plugins_google-0.5.dev0.tar`

### file list

```diff
@@ -1,22 +1,22 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-29 21:33:32.983969 livekit_plugins_google-0.5.0/
--rw-r--r--   0 runner    (1001) docker     (127)     1931 2024-05-29 21:33:32.983969 livekit_plugins_google-0.5.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      525 2024-05-29 21:33:28.000000 livekit_plugins_google-0.5.0/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-29 21:33:32.979969 livekit_plugins_google-0.5.0/livekit/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-29 21:33:32.979969 livekit_plugins_google-0.5.0/livekit/plugins/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-29 21:33:32.983969 livekit_plugins_google-0.5.0/livekit/plugins/google/
--rw-r--r--   0 runner    (1001) docker     (127)      959 2024-05-29 21:33:28.000000 livekit_plugins_google-0.5.0/livekit/plugins/google/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)       69 2024-05-29 21:33:28.000000 livekit_plugins_google-0.5.0/livekit/plugins/google/log.py
--rw-r--r--   0 runner    (1001) docker     (127)     1307 2024-05-29 21:33:28.000000 livekit_plugins_google-0.5.0/livekit/plugins/google/models.py
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-29 21:33:28.000000 livekit_plugins_google-0.5.0/livekit/plugins/google/py.typed
--rw-r--r--   0 runner    (1001) docker     (127)    16058 2024-05-29 21:33:28.000000 livekit_plugins_google-0.5.0/livekit/plugins/google/stt.py
--rw-r--r--   0 runner    (1001) docker     (127)     6182 2024-05-29 21:33:28.000000 livekit_plugins_google-0.5.0/livekit/plugins/google/tts.py
--rw-r--r--   0 runner    (1001) docker     (127)      600 2024-05-29 21:33:28.000000 livekit_plugins_google-0.5.0/livekit/plugins/google/version.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-29 21:33:32.983969 livekit_plugins_google-0.5.0/livekit_plugins_google.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     1931 2024-05-29 21:33:32.000000 livekit_plugins_google-0.5.0/livekit_plugins_google.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      486 2024-05-29 21:33:32.000000 livekit_plugins_google-0.5.0/livekit_plugins_google.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-29 21:33:32.000000 livekit_plugins_google-0.5.0/livekit_plugins_google.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)      230 2024-05-29 21:33:32.000000 livekit_plugins_google-0.5.0/livekit_plugins_google.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)        8 2024-05-29 21:33:32.000000 livekit_plugins_google-0.5.0/livekit_plugins_google.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)       86 2024-05-29 21:33:28.000000 livekit_plugins_google-0.5.0/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-29 21:33:32.983969 livekit_plugins_google-0.5.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)     2610 2024-05-29 21:33:28.000000 livekit_plugins_google-0.5.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-23 15:59:24.257817 livekit_plugins_google-0.5.dev0/
+-rw-r--r--   0 runner    (1001) docker     (127)     1937 2024-05-23 15:59:24.257817 livekit_plugins_google-0.5.dev0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      525 2024-05-23 15:59:17.000000 livekit_plugins_google-0.5.dev0/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-23 15:59:24.253816 livekit_plugins_google-0.5.dev0/livekit/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-23 15:59:24.253816 livekit_plugins_google-0.5.dev0/livekit/plugins/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-23 15:59:24.257817 livekit_plugins_google-0.5.dev0/livekit/plugins/google/
+-rw-r--r--   0 runner    (1001) docker     (127)      959 2024-05-23 15:59:17.000000 livekit_plugins_google-0.5.dev0/livekit/plugins/google/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)       69 2024-05-23 15:59:17.000000 livekit_plugins_google-0.5.dev0/livekit/plugins/google/log.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1307 2024-05-23 15:59:17.000000 livekit_plugins_google-0.5.dev0/livekit/plugins/google/models.py
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-23 15:59:17.000000 livekit_plugins_google-0.5.dev0/livekit/plugins/google/py.typed
+-rw-r--r--   0 runner    (1001) docker     (127)    16058 2024-05-23 15:59:17.000000 livekit_plugins_google-0.5.dev0/livekit/plugins/google/stt.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6128 2024-05-23 15:59:17.000000 livekit_plugins_google-0.5.dev0/livekit/plugins/google/tts.py
+-rw-r--r--   0 runner    (1001) docker     (127)      603 2024-05-23 15:59:17.000000 livekit_plugins_google-0.5.dev0/livekit/plugins/google/version.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-23 15:59:24.257817 livekit_plugins_google-0.5.dev0/livekit_plugins_google.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     1937 2024-05-23 15:59:24.000000 livekit_plugins_google-0.5.dev0/livekit_plugins_google.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      486 2024-05-23 15:59:24.000000 livekit_plugins_google-0.5.dev0/livekit_plugins_google.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-23 15:59:24.000000 livekit_plugins_google-0.5.dev0/livekit_plugins_google.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      233 2024-05-23 15:59:24.000000 livekit_plugins_google-0.5.dev0/livekit_plugins_google.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        8 2024-05-23 15:59:24.000000 livekit_plugins_google-0.5.dev0/livekit_plugins_google.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       86 2024-05-23 15:59:17.000000 livekit_plugins_google-0.5.dev0/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-23 15:59:24.257817 livekit_plugins_google-0.5.dev0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)     2613 2024-05-23 15:59:17.000000 livekit_plugins_google-0.5.dev0/setup.py
```

### Comparing `livekit_plugins_google-0.5.0/PKG-INFO` & `livekit_plugins_google-0.5.dev0/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: livekit-plugins-google
-Version: 0.5.0
+Version: 0.5.dev0
 Summary: Agent Framework plugin for services from Google Cloud
 Home-page: https://github.com/livekit/agents
 License: Apache-2.0
 Project-URL: Documentation, https://docs.livekit.io
 Project-URL: Website, https://livekit.io/
 Project-URL: Source, https://github.com/livekit/agents
 Keywords: webrtc,realtime,audio,video,livekit
@@ -26,15 +26,15 @@
 Requires-Dist: google-auth<3,>=2
 Requires-Dist: google-cloud-core<3,>=2
 Requires-Dist: google-cloud-speech<3,>=2
 Requires-Dist: google-cloud-texttospeech<3,>=2
 Requires-Dist: google-cloud-translate<4,>=3
 Requires-Dist: googleapis-common-protos<2,>=1
 Requires-Dist: livekit~=0.11
-Requires-Dist: livekit-agents~=0.7.0
+Requires-Dist: livekit-agents~=0.7.dev0
 
 # LiveKit Plugins Google
 
 Agent Framework plugin for services from Google Cloud. Currently supporting Google's [Speech-to-Text](https://cloud.google.com/speech-to-text) API.
 
 ## Installation
```

### Comparing `livekit_plugins_google-0.5.0/README.md` & `livekit_plugins_google-0.5.dev0/README.md`

 * *Files identical despite different names*

### Comparing `livekit_plugins_google-0.5.0/livekit/plugins/google/__init__.py` & `livekit_plugins_google-0.5.dev0/livekit/plugins/google/__init__.py`

 * *Files identical despite different names*

### Comparing `livekit_plugins_google-0.5.0/livekit/plugins/google/models.py` & `livekit_plugins_google-0.5.dev0/livekit/plugins/google/models.py`

 * *Files identical despite different names*

### Comparing `livekit_plugins_google-0.5.0/livekit/plugins/google/stt.py` & `livekit_plugins_google-0.5.dev0/livekit/plugins/google/stt.py`

 * *Files identical despite different names*

### Comparing `livekit_plugins_google-0.5.0/livekit/plugins/google/tts.py` & `livekit_plugins_google-0.5.dev0/livekit/plugins/google/tts.py`

 * *Files 2% similar despite different names*

```diff
@@ -142,17 +142,15 @@
             )
 
             data = response.audio_content
             if self._opts.audio_config.audio_encoding == "mp3":
                 decoder = codecs.Mp3StreamDecoder()
                 frames = decoder.decode_chunk(data)
                 for frame in frames:
-                    self._queue.put_nowait(
-                        tts.SynthesizedAudio(text=self._text, data=frame)
-                    )
+                    self._queue.put_nowait(tts.SynthesizedAudio(text="", data=frame))
             else:
                 self._queue.put_nowait(
                     tts.SynthesizedAudio(
                         text="",
                         data=rtc.AudioFrame(
                             data=data,
                             sample_rate=self._opts.audio_config.sample_rate_hertz,
```

### Comparing `livekit_plugins_google-0.5.0/livekit/plugins/google/version.py` & `livekit_plugins_google-0.5.dev0/livekit/plugins/google/version.py`

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

### Comparing `livekit_plugins_google-0.5.0/livekit_plugins_google.egg-info/PKG-INFO` & `livekit_plugins_google-0.5.dev0/livekit_plugins_google.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: livekit-plugins-google
-Version: 0.5.0
+Version: 0.5.dev0
 Summary: Agent Framework plugin for services from Google Cloud
 Home-page: https://github.com/livekit/agents
 License: Apache-2.0
 Project-URL: Documentation, https://docs.livekit.io
 Project-URL: Website, https://livekit.io/
 Project-URL: Source, https://github.com/livekit/agents
 Keywords: webrtc,realtime,audio,video,livekit
@@ -26,15 +26,15 @@
 Requires-Dist: google-auth<3,>=2
 Requires-Dist: google-cloud-core<3,>=2
 Requires-Dist: google-cloud-speech<3,>=2
 Requires-Dist: google-cloud-texttospeech<3,>=2
 Requires-Dist: google-cloud-translate<4,>=3
 Requires-Dist: googleapis-common-protos<2,>=1
 Requires-Dist: livekit~=0.11
-Requires-Dist: livekit-agents~=0.7.0
+Requires-Dist: livekit-agents~=0.7.dev0
 
 # LiveKit Plugins Google
 
 Agent Framework plugin for services from Google Cloud. Currently supporting Google's [Speech-to-Text](https://cloud.google.com/speech-to-text) API.
 
 ## Installation
```

### Comparing `livekit_plugins_google-0.5.0/setup.py` & `livekit_plugins_google-0.5.dev0/setup.py`

 * *Files 4% similar despite different names*

```diff
@@ -55,15 +55,15 @@
         "google-auth >= 2, < 3",
         "google-cloud-core >= 2, < 3",
         "google-cloud-speech >= 2, < 3",
         "google-cloud-texttospeech >= 2, < 3",
         "google-cloud-translate >= 3, < 4",
         "googleapis-common-protos >= 1, < 2",
         "livekit ~= 0.11",
-        "livekit-agents~=0.7.0",
+        "livekit-agents~=0.7.dev0",
     ],
     package_data={
         "livekit.plugins.google": ["py.typed"],
     },
     project_urls={
         "Documentation": "https://docs.livekit.io",
         "Website": "https://livekit.io/",
```

