# Comparing `tmp/livekit_plugins_elevenlabs-0.5.0.tar.gz` & `tmp/livekit_plugins_elevenlabs-0.5.dev0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "livekit_plugins_elevenlabs-0.5.0.tar", last modified: Wed May 29 21:33:29 2024, max compression
+gzip compressed data, was "livekit_plugins_elevenlabs-0.5.dev0.tar", last modified: Thu May 23 15:59:15 2024, max compression
```

## Comparing `livekit_plugins_elevenlabs-0.5.0.tar` & `livekit_plugins_elevenlabs-0.5.dev0.tar`

### file list

```diff
@@ -1,21 +1,21 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-29 21:33:29.489009 livekit_plugins_elevenlabs-0.5.0/
--rw-r--r--   0 runner    (1001) docker     (127)     1364 2024-05-29 21:33:29.489009 livekit_plugins_elevenlabs-0.5.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      308 2024-05-29 21:33:25.000000 livekit_plugins_elevenlabs-0.5.0/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-29 21:33:29.485009 livekit_plugins_elevenlabs-0.5.0/livekit/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-29 21:33:29.485009 livekit_plugins_elevenlabs-0.5.0/livekit/plugins/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-29 21:33:29.485009 livekit_plugins_elevenlabs-0.5.0/livekit/plugins/elevenlabs/
--rw-r--r--   0 runner    (1001) docker     (127)     1091 2024-05-29 21:33:25.000000 livekit_plugins_elevenlabs-0.5.0/livekit/plugins/elevenlabs/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)       73 2024-05-29 21:33:25.000000 livekit_plugins_elevenlabs-0.5.0/livekit/plugins/elevenlabs/log.py
--rw-r--r--   0 runner    (1001) docker     (127)      362 2024-05-29 21:33:25.000000 livekit_plugins_elevenlabs-0.5.0/livekit/plugins/elevenlabs/models.py
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-29 21:33:25.000000 livekit_plugins_elevenlabs-0.5.0/livekit/plugins/elevenlabs/py.typed
--rw-r--r--   0 runner    (1001) docker     (127)    17738 2024-05-29 21:33:25.000000 livekit_plugins_elevenlabs-0.5.0/livekit/plugins/elevenlabs/tts.py
--rw-r--r--   0 runner    (1001) docker     (127)      600 2024-05-29 21:33:25.000000 livekit_plugins_elevenlabs-0.5.0/livekit/plugins/elevenlabs/version.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-29 21:33:29.489009 livekit_plugins_elevenlabs-0.5.0/livekit_plugins_elevenlabs.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     1364 2024-05-29 21:33:29.000000 livekit_plugins_elevenlabs-0.5.0/livekit_plugins_elevenlabs.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      500 2024-05-29 21:33:29.000000 livekit_plugins_elevenlabs-0.5.0/livekit_plugins_elevenlabs.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-29 21:33:29.000000 livekit_plugins_elevenlabs-0.5.0/livekit_plugins_elevenlabs.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       59 2024-05-29 21:33:29.000000 livekit_plugins_elevenlabs-0.5.0/livekit_plugins_elevenlabs.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)        8 2024-05-29 21:33:29.000000 livekit_plugins_elevenlabs-0.5.0/livekit_plugins_elevenlabs.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)       86 2024-05-29 21:33:25.000000 livekit_plugins_elevenlabs-0.5.0/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-29 21:33:29.489009 livekit_plugins_elevenlabs-0.5.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)     2277 2024-05-29 21:33:25.000000 livekit_plugins_elevenlabs-0.5.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-23 15:59:15.325023 livekit_plugins_elevenlabs-0.5.dev0/
+-rw-r--r--   0 runner    (1001) docker     (127)     1362 2024-05-23 15:59:15.321023 livekit_plugins_elevenlabs-0.5.dev0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      308 2024-05-23 15:59:11.000000 livekit_plugins_elevenlabs-0.5.dev0/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-23 15:59:15.321023 livekit_plugins_elevenlabs-0.5.dev0/livekit/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-23 15:59:15.321023 livekit_plugins_elevenlabs-0.5.dev0/livekit/plugins/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-23 15:59:15.321023 livekit_plugins_elevenlabs-0.5.dev0/livekit/plugins/elevenlabs/
+-rw-r--r--   0 runner    (1001) docker     (127)      989 2024-05-23 15:59:11.000000 livekit_plugins_elevenlabs-0.5.dev0/livekit/plugins/elevenlabs/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)       73 2024-05-23 15:59:11.000000 livekit_plugins_elevenlabs-0.5.dev0/livekit/plugins/elevenlabs/log.py
+-rw-r--r--   0 runner    (1001) docker     (127)      163 2024-05-23 15:59:11.000000 livekit_plugins_elevenlabs-0.5.dev0/livekit/plugins/elevenlabs/models.py
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-23 15:59:11.000000 livekit_plugins_elevenlabs-0.5.dev0/livekit/plugins/elevenlabs/py.typed
+-rw-r--r--   0 runner    (1001) docker     (127)    16418 2024-05-23 15:59:11.000000 livekit_plugins_elevenlabs-0.5.dev0/livekit/plugins/elevenlabs/tts.py
+-rw-r--r--   0 runner    (1001) docker     (127)      603 2024-05-23 15:59:11.000000 livekit_plugins_elevenlabs-0.5.dev0/livekit/plugins/elevenlabs/version.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-23 15:59:15.321023 livekit_plugins_elevenlabs-0.5.dev0/livekit_plugins_elevenlabs.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     1362 2024-05-23 15:59:15.000000 livekit_plugins_elevenlabs-0.5.dev0/livekit_plugins_elevenlabs.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      500 2024-05-23 15:59:15.000000 livekit_plugins_elevenlabs-0.5.dev0/livekit_plugins_elevenlabs.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-23 15:59:15.000000 livekit_plugins_elevenlabs-0.5.dev0/livekit_plugins_elevenlabs.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       54 2024-05-23 15:59:15.000000 livekit_plugins_elevenlabs-0.5.dev0/livekit_plugins_elevenlabs.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        8 2024-05-23 15:59:15.000000 livekit_plugins_elevenlabs-0.5.dev0/livekit_plugins_elevenlabs.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       86 2024-05-23 15:59:11.000000 livekit_plugins_elevenlabs-0.5.dev0/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-23 15:59:15.325023 livekit_plugins_elevenlabs-0.5.dev0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)     2272 2024-05-23 15:59:11.000000 livekit_plugins_elevenlabs-0.5.dev0/setup.py
```

### Comparing `livekit_plugins_elevenlabs-0.5.0/PKG-INFO` & `livekit_plugins_elevenlabs-0.5.dev0/PKG-INFO`

 * *Files 12% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: livekit-plugins-elevenlabs
-Version: 0.5.0
+Version: 0.5.dev0
 Summary: Agent Framework plugin for voice synthesis with ElevenLabs' API.
 Home-page: https://github.com/livekit/agents
 License: Apache-2.0
 Project-URL: Documentation, https://docs.livekit.io
 Project-URL: Website, https://livekit.io/
 Project-URL: Source, https://github.com/livekit/agents
 Keywords: webrtc,realtime,audio,video,livekit,elevenlabs
@@ -16,15 +16,15 @@
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3 :: Only
 Requires-Python: >=3.9.0
 Description-Content-Type: text/markdown
 Requires-Dist: livekit~=0.11
-Requires-Dist: livekit-agents[codecs]~=0.7.0
+Requires-Dist: livekit-agents~=0.7.dev0
 Requires-Dist: aiohttp>=3.8.5
 
 # LiveKit Plugins Elevenlabs
 
 Agent Framework plugin for voice synthesis with [ElevenLabs](https://elevenlabs.io/) API.
 
 ## Installation
```

### Comparing `livekit_plugins_elevenlabs-0.5.0/livekit/plugins/elevenlabs/__init__.py` & `livekit_plugins_elevenlabs-0.5.dev0/livekit/plugins/elevenlabs/__init__.py`

 * *Files 16% similar despite different names*

```diff
@@ -8,27 +8,18 @@
 #
 # Unless required by applicable law or agreed to in writing, software
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 
-from .models import TTSEncoding, TTSModels
 from .tts import DEFAULT_VOICE, TTS, Voice, VoiceSettings
 from .version import __version__
 
-__all__ = [
-    "TTS",
-    "Voice",
-    "VoiceSettings",
-    "TTSEncoding",
-    "TTSModels",
-    "DEFAULT_VOICE",
-    "__version__",
-]
+__all__ = ["TTS", "Voice", "VoiceSettings", "DEFAULT_VOICE", "__version__"]
 
 from livekit.agents import Plugin
 
 
 class ElevenLabsPlugin(Plugin):
     def __init__(self):
         super().__init__(__name__, __version__, __package__)
```

### Comparing `livekit_plugins_elevenlabs-0.5.0/livekit/plugins/elevenlabs/tts.py` & `livekit_plugins_elevenlabs-0.5.dev0/livekit/plugins/elevenlabs/tts.py`

 * *Files 6% similar despite different names*

```diff
@@ -17,44 +17,22 @@
 import asyncio
 import base64
 import contextlib
 import dataclasses
 import json
 import os
 from dataclasses import dataclass
-from typing import List, Literal, Optional
+from typing import List, Optional
 
 import aiohttp
 from livekit import rtc
-from livekit.agents import aio, codecs, tokenize, tts, utils
+from livekit.agents import aio, tokenize, tts, utils
 
 from .log import logger
-from .models import (
-    TTSEncoding,
-    TTSModels,
-)
-
-_Encoding = Literal[
-    "mp3",
-    "pcm",
-]
-
-
-def _sample_rate_from_format(output_format: TTSEncoding) -> int:
-    split = output_format.split("_")  # e.g: mp3_22050_32
-    return int(split[1])
-
-
-def _encoding_from_format(output_format: TTSEncoding) -> _Encoding:
-    if output_format.startswith("mp3"):
-        return "mp3"
-    elif output_format.startswith("pcm"):
-        return "pcm"
-
-    raise ValueError(f"Unknown format: {output_format}")
+from .models import TTSModels
 
 
 @dataclass
 class VoiceSettings:
     stability: float  # [0.0 - 1.0]
     similarity_boost: float  # [0.0 - 1.0]
     style: float | None = None  # [0.0 - 1.0]
@@ -84,55 +62,51 @@
 
 @dataclass
 class _TTSOptions:
     api_key: str
     voice: Voice
     model_id: TTSModels
     base_url: str
-    encoding: TTSEncoding
     sample_rate: int
     streaming_latency: int
     word_tokenizer: tokenize.WordTokenizer
     chunk_length_schedule: list[int]
 
 
 class TTS(tts.TTS):
     def __init__(
         self,
         *,
         voice: Voice = DEFAULT_VOICE,
         model_id: TTSModels = "eleven_turbo_v2",
         api_key: str | None = None,
         base_url: str | None = None,
-        encoding: TTSEncoding = "mp3_22050_32",
+        sample_rate: int = 24000,
         streaming_latency: int = 3,
         word_tokenizer: tokenize.WordTokenizer = tokenize.basic.WordTokenizer(
             ignore_punctuation=False  # punctuation can help for intonation
         ),
         # default value of 11labs is [120, 160, 250, 290], but we want faster responses by default
         # (range is 50-500)
         chunk_length_schedule: list[int] = [80, 120, 200, 260],
         http_session: aiohttp.ClientSession | None = None,
     ) -> None:
         super().__init__(
-            streaming_supported=True,
-            sample_rate=_sample_rate_from_format(encoding),
-            num_channels=1,
+            streaming_supported=True, sample_rate=sample_rate, num_channels=1
         )
         api_key = api_key or os.environ.get("ELEVEN_API_KEY")
         if not api_key:
             raise ValueError("ELEVEN_API_KEY must be set")
 
         self._opts = _TTSOptions(
             voice=voice,
             model_id=model_id,
             api_key=api_key,
             base_url=base_url or API_BASE_URL_V1,
-            encoding=encoding,
-            sample_rate=self.sample_rate,
+            sample_rate=sample_rate,
             streaming_latency=streaming_latency,
             word_tokenizer=word_tokenizer,
             chunk_length_schedule=chunk_length_schedule,
         )
         self._session = http_session
 
     def _ensure_session(self) -> aiohttp.ClientSession:
@@ -172,15 +146,15 @@
         self._task: asyncio.Task | None = None
         self._queue = asyncio.Queue[Optional[tts.SynthesizedAudio]]()
 
     def _synthesize_url(self) -> str:
         base_url = self._opts.base_url
         voice_id = self._opts.voice.id
         model_id = self._opts.model_id
-        sample_rate = _sample_rate_from_format(self._opts.encoding)
+        sample_rate = self._opts.sample_rate
         latency = self._opts.streaming_latency
         url = (
             f"{base_url}/text-to-speech/{voice_id}/stream?"
             f"model_id={model_id}&output_format=pcm_{sample_rate}&optimize_streaming_latency={latency}"
         )
         return url
 
@@ -282,19 +256,19 @@
         self._closed = False
         self._word_stream = opts.word_tokenizer.stream()
 
     def _stream_url(self) -> str:
         base_url = self._opts.base_url
         voice_id = self._opts.voice.id
         model_id = self._opts.model_id
-        output_format = self._opts.encoding
+        sample_rate = self._opts.sample_rate
         latency = self._opts.streaming_latency
         url = (
             f"{base_url}/text-to-speech/{voice_id}/stream-input?"
-            f"model_id={model_id}&output_format={output_format}&optimize_streaming_latency={latency}"
+            f"model_id={model_id}&output_format=pcm_{sample_rate}&optimize_streaming_latency={latency}"
         )
 
         return url
 
     def push_text(self, token: str | None) -> None:
         if self._closed:
             raise ValueError("cannot push to a closed stream")
@@ -439,16 +413,14 @@
             )
             await ws_conn.send_str(json.dumps(flush_pkt))
 
             nonlocal all_tokens_consumed
             all_tokens_consumed = True
 
         async def recv_task():
-            encoding = _encoding_from_format(self._opts.encoding)
-            mp3_decoder = codecs.Mp3StreamDecoder()
             while True:
                 msg = await ws_conn.receive()
                 if msg.type in (
                     aiohttp.WSMsgType.CLOSED,
                     aiohttp.WSMsgType.CLOSE,
                     aiohttp.WSMsgType.CLOSING,
                 ):
@@ -461,40 +433,27 @@
 
                 if msg.type != aiohttp.WSMsgType.TEXT:
                     # audio frames are serialized in base64..
                     logger.warning("unexpected 11labs message type %s", msg.type)
                     continue
 
                 data: dict = json.loads(msg.data)
-                audio = data.get("audio")
+                if data.get("audio"):
+                    b64data = base64.b64decode(data["audio"])
 
-                if data.get("error"):
-                    logger.error("11labs error %s", data)
-                    return
-                elif audio is not None:
-                    if audio == "":
-                        # 11labs sometimes sends empty audio, ignore
-                        continue
-
-                    b64data = base64.b64decode(audio)
-                    frame: rtc.AudioFrame
-                    if encoding == "mp3":
-                        frames = mp3_decoder.decode_chunk(b64data)
-                        frame = utils.merge_frames(frames)
-                    else:
-                        frame = rtc.AudioFrame(
-                            data=b64data,
-                            sample_rate=self._opts.sample_rate,
-                            num_channels=1,
-                            samples_per_channel=len(b64data) // 2,
-                        )
+                    frame = rtc.AudioFrame(
+                        data=b64data,
+                        sample_rate=self._opts.sample_rate,
+                        num_channels=1,
+                        samples_per_channel=len(b64data) // 2,
+                    )
 
                     text = ""
                     if data.get("alignment"):
-                        text = "".join(data["alignment"].get("chars", ""))
+                        text = data["alignment"].get("chars", "")
 
                     audio_tx.send_nowait(tts.SynthesizedAudio(text=text, data=frame))
                     continue
                 elif data.get("isFinal"):
                     return  # last message
 
                 logger.error("unexpected 11labs message %s", data)
```

### Comparing `livekit_plugins_elevenlabs-0.5.0/livekit/plugins/elevenlabs/version.py` & `livekit_plugins_elevenlabs-0.5.dev0/livekit/plugins/elevenlabs/version.py`

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

### Comparing `livekit_plugins_elevenlabs-0.5.0/livekit_plugins_elevenlabs.egg-info/PKG-INFO` & `livekit_plugins_elevenlabs-0.5.dev0/livekit_plugins_elevenlabs.egg-info/PKG-INFO`

 * *Files 12% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: livekit-plugins-elevenlabs
-Version: 0.5.0
+Version: 0.5.dev0
 Summary: Agent Framework plugin for voice synthesis with ElevenLabs' API.
 Home-page: https://github.com/livekit/agents
 License: Apache-2.0
 Project-URL: Documentation, https://docs.livekit.io
 Project-URL: Website, https://livekit.io/
 Project-URL: Source, https://github.com/livekit/agents
 Keywords: webrtc,realtime,audio,video,livekit,elevenlabs
@@ -16,15 +16,15 @@
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3 :: Only
 Requires-Python: >=3.9.0
 Description-Content-Type: text/markdown
 Requires-Dist: livekit~=0.11
-Requires-Dist: livekit-agents[codecs]~=0.7.0
+Requires-Dist: livekit-agents~=0.7.dev0
 Requires-Dist: aiohttp>=3.8.5
 
 # LiveKit Plugins Elevenlabs
 
 Agent Framework plugin for voice synthesis with [ElevenLabs](https://elevenlabs.io/) API.
 
 ## Installation
```

### Comparing `livekit_plugins_elevenlabs-0.5.0/setup.py` & `livekit_plugins_elevenlabs-0.5.dev0/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -47,15 +47,15 @@
     ],
     keywords=["webrtc", "realtime", "audio", "video", "livekit", "elevenlabs"],
     license="Apache-2.0",
     packages=setuptools.find_namespace_packages(include=["livekit.*"]),
     python_requires=">=3.9.0",
     install_requires=[
         "livekit ~= 0.11",
-        "livekit-agents[codecs]~=0.7.0",
+        "livekit-agents~=0.7.dev0",
         "aiohttp >= 3.8.5",
     ],
     package_data={
         "livekit.plugins.elevenlabs": ["py.typed"],
     },
     project_urls={
         "Documentation": "https://docs.livekit.io",
```

