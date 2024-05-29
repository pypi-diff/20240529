# Comparing `tmp/cartesia-0.0.6.tar.gz` & `tmp/cartesia-0.1.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "cartesia-0.0.6.tar", last modified: Fri May 17 23:40:18 2024, max compression
+gzip compressed data, was "cartesia-0.1.0.tar", last modified: Wed May 29 13:46:10 2024, max compression
```

## Comparing `cartesia-0.0.6.tar` & `cartesia-0.1.0.tar`

### file list

```diff
@@ -1,19 +1,20 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-17 23:40:18.810603 cartesia-0.0.6/
--rw-r--r--   0 runner    (1001) docker     (127)     5416 2024-05-17 23:40:18.810603 cartesia-0.0.6/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     4967 2024-05-17 23:39:52.000000 cartesia-0.0.6/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-17 23:40:18.810603 cartesia-0.0.6/cartesia/
--rw-r--r--   0 runner    (1001) docker     (127)      102 2024-05-17 23:39:52.000000 cartesia-0.0.6/cartesia/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    26734 2024-05-17 23:39:52.000000 cartesia-0.0.6/cartesia/tts.py
--rw-r--r--   0 runner    (1001) docker     (127)     3024 2024-05-17 23:39:52.000000 cartesia-0.0.6/cartesia/utils.py
--rw-r--r--   0 runner    (1001) docker     (127)       22 2024-05-17 23:39:52.000000 cartesia-0.0.6/cartesia/version.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-17 23:40:18.810603 cartesia-0.0.6/cartesia.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     5416 2024-05-17 23:40:18.000000 cartesia-0.0.6/cartesia.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      285 2024-05-17 23:40:18.000000 cartesia-0.0.6/cartesia.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-17 23:40:18.000000 cartesia-0.0.6/cartesia.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)      173 2024-05-17 23:40:18.000000 cartesia-0.0.6/cartesia.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)        9 2024-05-17 23:40:18.000000 cartesia-0.0.6/cartesia.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)     1702 2024-05-17 23:39:52.000000 cartesia-0.0.6/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-17 23:40:18.810603 cartesia-0.0.6/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)     9241 2024-05-17 23:39:52.000000 cartesia-0.0.6/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-17 23:40:18.810603 cartesia-0.0.6/tests/
--rw-r--r--   0 runner    (1001) docker     (127)    10533 2024-05-17 23:39:52.000000 cartesia-0.0.6/tests/test_tts.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-29 13:46:10.849352 cartesia-0.1.0/
+-rw-r--r--   0 runner    (1001) docker     (127)     5416 2024-05-29 13:46:10.845351 cartesia-0.1.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     4967 2024-05-29 13:45:52.000000 cartesia-0.1.0/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-29 13:46:10.845351 cartesia-0.1.0/cartesia/
+-rw-r--r--   0 runner    (1001) docker     (127)      102 2024-05-29 13:45:52.000000 cartesia-0.1.0/cartesia/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1001 2024-05-29 13:45:52.000000 cartesia-0.1.0/cartesia/_types.py
+-rw-r--r--   0 runner    (1001) docker     (127)    25806 2024-05-29 13:45:52.000000 cartesia-0.1.0/cartesia/tts.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3339 2024-05-29 13:45:52.000000 cartesia-0.1.0/cartesia/utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)       22 2024-05-29 13:45:52.000000 cartesia-0.1.0/cartesia/version.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-29 13:46:10.845351 cartesia-0.1.0/cartesia.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     5416 2024-05-29 13:46:10.000000 cartesia-0.1.0/cartesia.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      304 2024-05-29 13:46:10.000000 cartesia-0.1.0/cartesia.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-29 13:46:10.000000 cartesia-0.1.0/cartesia.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      185 2024-05-29 13:46:10.000000 cartesia-0.1.0/cartesia.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        9 2024-05-29 13:46:10.000000 cartesia-0.1.0/cartesia.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)     1702 2024-05-29 13:45:52.000000 cartesia-0.1.0/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-29 13:46:10.849352 cartesia-0.1.0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)     9241 2024-05-29 13:45:52.000000 cartesia-0.1.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-29 13:46:10.845351 cartesia-0.1.0/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)    18838 2024-05-29 13:45:52.000000 cartesia-0.1.0/tests/test_tts.py
```

### Comparing `cartesia-0.0.6/PKG-INFO` & `cartesia-0.1.0/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: cartesia
-Version: 0.0.6
+Version: 0.1.0
 Summary: The official Python library for the Cartesia API.
 Home-page: 
 Author: Cartesia, Inc.
 Author-email: support@cartesia.ai
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3
 Classifier: Topic :: Scientific/Engineering :: Artificial Intelligence
```

### Comparing `cartesia-0.0.6/README.md` & `cartesia-0.1.0/README.md`

 * *Files identical despite different names*

### Comparing `cartesia-0.0.6/cartesia/tts.py` & `cartesia-0.1.0/cartesia/tts.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,48 +1,59 @@
 import asyncio
 import base64
 import json
 import os
 import uuid
 from types import TracebackType
-from typing import Any, AsyncGenerator, Dict, Generator, List, Optional, Tuple, TypedDict, Union
+from typing import (
+    Any,
+    AsyncGenerator,
+    Dict,
+    Generator,
+    List,
+    Optional,
+    Tuple,
+    TypedDict,
+    Union,
+)
 
 import aiohttp
 import httpx
 import logging
 import requests
 from websockets.sync.client import connect
 
 from cartesia.utils import retry_on_connection_error, retry_on_connection_error_async
+from cartesia._types import (
+    AudioDataReturnType,
+    AudioOutputFormat,
+    AudioOutput,
+    Embedding,
+    VoiceMetadata,
+)
+
+try:
+    import numpy as np
+
+    _NUMPY_AVAILABLE = True
+except ImportError:
+    _NUMPY_AVAILABLE = False
+
 
 DEFAULT_MODEL_ID = ""
 DEFAULT_BASE_URL = "api.cartesia.ai"
 DEFAULT_API_VERSION = "v0"
 DEFAULT_TIMEOUT = 30  # seconds
 DEFAULT_NUM_CONNECTIONS = 10  # connections per client
 
 BACKOFF_FACTOR = 1
 MAX_RETRIES = 3
 
 logger = logging.getLogger(__name__)
 
-class AudioOutput(TypedDict):
-    audio: bytes
-    sampling_rate: int
-
-
-Embedding = List[float]
-
-
-class VoiceMetadata(TypedDict):
-    id: str
-    name: str
-    description: str
-    embedding: Optional[Embedding]
-
 
 def update_buffer(buffer: str, chunk_bytes: bytes) -> Tuple[str, List[Dict[str, Any]]]:
     buffer += chunk_bytes.decode("utf-8")
     outputs = []
     while "{" in buffer and "}" in buffer:
         start_index = buffer.find("{")
         end_index = buffer.find("}", start_index)
@@ -75,15 +86,14 @@
     """The client for Cartesia's text-to-speech library.
 
     This client contains methods to interact with the Cartesia text-to-speech API.
     The client can be used to retrieve available voices, compute new voice embeddings,
     and generate speech from text.
 
     The client also supports generating audio using a websocket for lower latency.
-    To enable interrupt handling along the websocket, set `experimental_ws_handle_interrupts=True`.
 
     Examples:
         >>> client = CartesiaTTS()
 
         # Load available voices and their metadata (excluding the embeddings).
         # Embeddings are fetched with `get_voice_embedding`. This avoids preloading
         # all of the embeddings, which can be expensive if there are a lot of voices.
@@ -98,29 +108,25 @@
         >>> audio = client.generate(transcript="Hello world!", voice=embedding)
 
         # Generate audio stream
         >>> for audio_chunk in client.generate(transcript="Hello world!", voice=embedding, stream=True):
         ...     audio, sr = audio_chunk["audio"], audio_chunk["sampling_rate"]
     """
 
-    def __init__(self, *, api_key: str = None, experimental_ws_handle_interrupts: bool = False):
+    def __init__(self, *, api_key: str = None):
         """Args:
         api_key: The API key to use for authorization.
             If not specified, the API key will be read from the environment variable
             `CARTESIA_API_KEY`.
-        experimental_ws_handle_interrupts: Whether to handle interrupts when generating
-            audio using the websocket. This is an experimental feature and may have bugs
-            or be deprecated in the future.
         """
         self.base_url = os.environ.get("CARTESIA_BASE_URL", DEFAULT_BASE_URL)
         self.api_key = api_key or os.environ.get("CARTESIA_API_KEY")
         self.api_version = os.environ.get("CARTESIA_API_VERSION", DEFAULT_API_VERSION)
         self.headers = {"X-API-Key": self.api_key, "Content-Type": "application/json"}
         self.websocket = None
-        self.experimental_ws_handle_interrupts = experimental_ws_handle_interrupts
 
     def get_voices(self, skip_embeddings: bool = True) -> Dict[str, VoiceMetadata]:
         """Returns a mapping from voice name -> voice metadata.
 
         Args:
             skip_embeddings: Whether to skip returning the embeddings.
                 It is recommended to skip if you only want to see what
@@ -161,15 +167,17 @@
 
         voices = response.json()
         for voice in voices:
             if "embedding" in voice and isinstance(voice["embedding"], str):
                 voice["embedding"] = json.loads(voice["embedding"])
         return {voice["name"]: voice for voice in voices}
 
-    @retry_on_connection_error(max_retries=MAX_RETRIES, backoff_factor=BACKOFF_FACTOR, logger=logger)
+    @retry_on_connection_error(
+        max_retries=MAX_RETRIES, backoff_factor=BACKOFF_FACTOR, logger=logger
+    )
     def get_voice_embedding(
         self, *, voice_id: str = None, filepath: str = None, link: str = None
     ) -> Embedding:
         """Get a voice embedding from voice_id, a filepath or YouTube url.
 
         Args:
             voice_id: The voice id.
@@ -218,24 +226,36 @@
         """Refresh the websocket connection.
 
         Note:
             The connection is synchronous.
         """
         if self.websocket is None or self._is_websocket_closed():
             route = "audio/websocket"
-            if self.experimental_ws_handle_interrupts:
-                route = f"experimental/{route}"
             self.websocket = connect(f"{self._ws_url()}/{route}?api_key={self.api_key}")
 
     def _is_websocket_closed(self):
         return self.websocket.socket.fileno() == -1
 
     def _check_inputs(
-        self, transcript: str, duration: Optional[float], chunk_time: Optional[float]
+        self,
+        transcript: str,
+        duration: Optional[float],
+        chunk_time: Optional[float],
+        output_format: Union[str, AudioOutputFormat],
+        data_rtype: Union[str, AudioDataReturnType],
     ):
+        # This will try the casting and raise an error.
+        _ = AudioOutputFormat(output_format)
+
+        if AudioDataReturnType(data_rtype) == AudioDataReturnType.ARRAY and not _NUMPY_AVAILABLE:
+            raise ImportError(
+                "The 'numpy' package is required to use the 'array' return type. "
+                "Please install 'numpy' or use 'bytes' as the return type."
+            )
+
         if chunk_time is not None:
             if chunk_time < 0.1 or chunk_time > 0.5:
                 raise ValueError("`chunk_time` must be between 0.1 and 0.5")
 
         if chunk_time is not None and duration is not None:
             if duration < chunk_time:
                 raise ValueError("`duration` must be greater than chunk_time")
@@ -245,24 +265,25 @@
 
     def _generate_request_body(
         self,
         *,
         transcript: str,
         voice: Embedding,
         model_id: str,
-        output_format: str,
+        output_format: AudioOutputFormat,
         duration: int = None,
         chunk_time: float = None,
     ) -> Dict[str, Any]:
         """Create the request body for a stream request.
 
         Note that anything that's not provided will use a default if available or be
         filtered out otherwise.
         """
         body = dict(transcript=transcript, model_id=model_id, voice=voice)
+        output_format = output_format.value
 
         optional_body = dict(
             duration=duration,
             chunk_time=chunk_time,
             output_format=output_format,
         )
         body.update({k: v for k, v in optional_body.items() if v is not None})
@@ -275,64 +296,110 @@
         transcript: str,
         voice: Embedding,
         model_id: str = DEFAULT_MODEL_ID,
         duration: int = None,
         chunk_time: float = None,
         stream: bool = False,
         websocket: bool = True,
-        output_format: str = "fp32",
+        output_format: Union[str, AudioOutputFormat] = "fp32",
+        data_rtype: str = "bytes",
     ) -> Union[AudioOutput, Generator[AudioOutput, None, None]]:
         """Generate audio from a transcript.
 
         Args:
             transcript (str): The text to generate audio for.
             voice (Embedding (List[float])): The voice to use for generating audio.
             duration (int, optional): The maximum duration of the audio in seconds.
             chunk_time (float, optional): How long each audio segment should be in seconds.
                 This should not need to be adjusted.
             stream (bool, optional): Whether to stream the audio or not.
                 If True this function returns a generator. False by default.
             websocket (bool, optional): Whether to use a websocket for streaming audio.
                 Using the websocket reduces latency by pre-poning the handshake. True by default.
+            data_rtype: The return type for the 'data' key in the dictionary.
+                One of `'byte' | 'array'`.
+                Note this field is experimental and may be deprecated in the future.
 
         Returns:
             A generator if `stream` is True, otherwise a dictionary.
             Dictionary from both generator and non-generator return types have the following keys:
                 * "audio": The audio as a bytes buffer.
                 * "sampling_rate": The sampling rate of the audio.
         """
-        self._check_inputs(transcript, duration, chunk_time)
+        self._check_inputs(transcript, duration, chunk_time, output_format, data_rtype)
+
+        data_rtype = AudioDataReturnType(data_rtype)
+        output_format = AudioOutputFormat(output_format)
 
         body = self._generate_request_body(
-            transcript=transcript, 
-            voice=voice, 
+            transcript=transcript,
+            voice=voice,
             model_id=model_id,
-            duration=duration, 
+            duration=duration,
             chunk_time=chunk_time,
             output_format=output_format,
         )
 
         if websocket:
             generator = self._generate_ws(body)
         else:
             generator = self._generate_http_wrapper(body)
 
+        generator = self._postprocess_audio(
+            generator, data_rtype=data_rtype, output_format=output_format
+        )
         if stream:
             return generator
 
         chunks = []
         sampling_rate = None
         for chunk in generator:
             if sampling_rate is None:
                 sampling_rate = chunk["sampling_rate"]
             chunks.append(chunk["audio"])
 
-        return {"audio": b"".join(chunks), "sampling_rate": sampling_rate}
+        if data_rtype == AudioDataReturnType.ARRAY:
+            cat = np.concatenate
+        else:
+            cat = b"".join
+
+        return {"audio": cat(chunks), "sampling_rate": sampling_rate}
+
+    def _postprocess_audio(
+        self,
+        generator: Generator[AudioOutput, None, None],
+        *,
+        data_rtype: AudioDataReturnType,
+        output_format: AudioOutputFormat,
+    ) -> Generator[AudioOutput, None, None]:
+        """Perform postprocessing on the generator outputs.
+
+        The postprocessing should be minimal (e.g. converting to array, casting dtype).
+        This code should not perform heavy operations like changing the sampling rate.
+
+        Args:
+            generator: A generator that yields audio chunks.
+            data_rtype: The data return type.
+            output_format: The output format for the audio.
+
+        Returns:
+            A generator that yields audio chunks.
+        """
+        dtype = None
+        if data_rtype == AudioDataReturnType.ARRAY:
+            dtype = np.float32 if "fp32" in output_format.value else np.int16
 
-    @retry_on_connection_error(max_retries=MAX_RETRIES, backoff_factor=BACKOFF_FACTOR, logger=logger)
+        for chunk in generator:
+            if dtype is not None:
+                chunk["audio"] = np.frombuffer(chunk["audio"], dtype=dtype)
+            yield chunk
+
+    @retry_on_connection_error(
+        max_retries=MAX_RETRIES, backoff_factor=BACKOFF_FACTOR, logger=logger
+    )
     def _generate_http_wrapper(self, body: Dict[str, Any]):
         """Need to wrap the http generator in a function for the retry decorator to work."""
         try:
             for chunk in self._generate_http(body):
                 yield chunk
         except Exception as e:
             logger.error(f"Failed to generate audio. {e}")
@@ -385,50 +452,24 @@
                 response = json.loads(self.websocket.recv())
                 if "error" in response:
                     raise RuntimeError(f"Error generating audio:\n{response['error']}")
                 if response["done"]:
                     break
 
                 yield convert_response(response, include_context_id)
-
-                if self.experimental_ws_handle_interrupts:
-                    self.websocket.send(json.dumps({"context_id": context_id}))
-        except GeneratorExit:
-            # The exit is only called when the generator is garbage collected.
-            # It may not be called directly after a break statement.
-            # However, the generator will be automatically cancelled on the next request.
-            if self.experimental_ws_handle_interrupts:
-                self.websocket.send(json.dumps({"context_id": context_id, "action": "cancel"}))
         except Exception as e:
             # Close the websocket connection if an error occurs.
             if self.websocket and not self._is_websocket_closed():
                 self.websocket.close()
             raise RuntimeError(f"Failed to generate audio. {response}") from e
         finally:
             # Ensure the websocket is ultimately closed.
             if self.websocket and not self._is_websocket_closed():
                 self.websocket.close()
 
-    @retry_on_connection_error(max_retries=MAX_RETRIES, backoff_factor=BACKOFF_FACTOR, logger=logger)
-    def transcribe(self, raw_audio: Union[bytes, str]) -> str:
-        raw_audio_bytes, headers = self.prepare_audio_and_headers(raw_audio)
-        response = httpx.post(
-            f"{self._http_url()}/audio/transcriptions",
-            headers=headers,
-            files={"clip": ("input.wav", raw_audio_bytes)},
-            timeout=DEFAULT_TIMEOUT,
-        )
-
-        if not response.is_success:
-            raise ValueError(f"Failed to transcribe audio. Error: {response.text()}")
-
-        transcript = response.json()
-        return transcript["text"]
-
-
     def prepare_audio_and_headers(
         self, raw_audio: Union[bytes, str]
     ) -> Tuple[bytes, Dict[str, Any]]:
         if isinstance(raw_audio, str):
             with open(raw_audio, "rb") as f:
                 raw_audio_bytes = f.read()
         else:
@@ -462,52 +503,46 @@
         exc: Union[BaseException, None],
         exc_tb: Union[TracebackType, None],
     ):
         self.close()
 
 
 class AsyncCartesiaTTS(CartesiaTTS):
-    def __init__(self, *, api_key: str = None, experimental_ws_handle_interrupts: bool = False):
+    def __init__(self, *, api_key: str = None):
         self._session = None
         self._loop = None
-        super().__init__(
-            api_key=api_key, experimental_ws_handle_interrupts=experimental_ws_handle_interrupts
-        )
-    
+        super().__init__(api_key=api_key)
+
     async def _get_session(self):
         current_loop = asyncio.get_event_loop()
         if self._loop is not current_loop:
             # If the loop has changed, close the session and create a new one.
             await self.close()
         if self._session is None or self._session.closed:
             timeout = aiohttp.ClientTimeout(total=DEFAULT_TIMEOUT)
             connector = aiohttp.TCPConnector(limit=DEFAULT_NUM_CONNECTIONS)
-            self._session = aiohttp.ClientSession(
-                timeout=timeout, connector=connector
-            )
+            self._session = aiohttp.ClientSession(timeout=timeout, connector=connector)
             self._loop = current_loop
         return self._session
-    
+
     async def refresh_websocket(self):
         """Refresh the websocket connection."""
         if self.websocket is None or self._is_websocket_closed():
             route = "audio/websocket"
-            if self.experimental_ws_handle_interrupts:
-                route = f"experimental/{route}"
             session = await self._get_session()
             self.websocket = await session.ws_connect(
                 f"{self._ws_url()}/{route}?api_key={self.api_key}"
             )
-    
+
     def _is_websocket_closed(self):
         return self.websocket.closed
 
     async def close(self):
         """This method closes the websocket and the session.
-        
+
         It is *strongly* recommended to call this method when you are done using the client.
         """
         if self.websocket is not None and not self._is_websocket_closed():
             await self.websocket.close()
         if self._session is not None and not self._session.closed:
             await self._session.close()
 
@@ -517,70 +552,83 @@
         transcript: str,
         voice: Embedding,
         model_id: str = DEFAULT_MODEL_ID,
         duration: int = None,
         chunk_time: float = None,
         stream: bool = False,
         websocket: bool = True,
-        output_format: str = "fp32"
+        output_format: Union[str, AudioOutputFormat] = "fp32",
+        data_rtype: Union[str, AudioDataReturnType] = "bytes",
     ) -> Union[AudioOutput, AsyncGenerator[AudioOutput, None]]:
         """Asynchronously generate audio from a transcript.
-        NOTE: This overrides the non-asynchronous generate method from the base class.
 
-        Args:
-            transcript (str): The text to generate audio for.
-            voice (Embedding (List[float])): The voice to use for generating audio.
-            duration (int, optional): The maximum duration of the audio in seconds.
-            chunk_time (float, optional): How long each audio segment should be in seconds.
-                This should not need to be adjusted.
-            stream (bool, optional): Whether to stream the audio or not.
-                If True this function returns a generator. False by default.
-            websocket (bool, optional): Whether to use a websocket for streaming audio.
-                Using the websocket reduces latency by pre-poning the handshake. True by default.
-
-        Returns:
-            A generator if `stream` is True, otherwise a dictionary.
-            Dictionary from both generator and non-generator return types have the following keys:
-                * "audio": The audio as a bytes buffer.
-                * "sampling_rate": The sampling rate of the audio.
+        For more information on the arguments, see the synchronous :meth:`CartesiaTTS.generate`.
         """
-        self._check_inputs(transcript, duration, chunk_time)
+        self._check_inputs(transcript, duration, chunk_time, output_format, data_rtype)
+        data_rtype = AudioDataReturnType(data_rtype)
+        output_format = AudioOutputFormat(output_format)
 
         body = self._generate_request_body(
-            transcript=transcript, 
+            transcript=transcript,
             voice=voice,
             model_id=model_id,
-            duration=duration, 
+            duration=duration,
             chunk_time=chunk_time,
             output_format=output_format,
         )
 
         if websocket:
             generator = self._generate_ws(body)
         else:
             generator = self._generate_http_wrapper(body)
-
+        generator = self._postprocess_audio(
+            generator, data_rtype=data_rtype, output_format=output_format
+        )
         if stream:
             return generator
 
         chunks = []
         sampling_rate = None
         async for chunk in generator:
             if sampling_rate is None:
                 sampling_rate = chunk["sampling_rate"]
             chunks.append(chunk["audio"])
 
-        return {"audio": b"".join(chunks), "sampling_rate": sampling_rate}
+        if data_rtype == AudioDataReturnType.ARRAY:
+            cat = np.concatenate
+        else:
+            cat = b"".join
+
+        return {"audio": cat(chunks), "sampling_rate": sampling_rate}
 
-    @retry_on_connection_error_async(max_retries=MAX_RETRIES, backoff_factor=BACKOFF_FACTOR, logger=logger)
+    async def _postprocess_audio(
+        self,
+        generator: AsyncGenerator[AudioOutput, None],
+        *,
+        data_rtype: AudioDataReturnType,
+        output_format: AudioOutputFormat,
+    ) -> AsyncGenerator[AudioOutput, None]:
+        """See :meth:`CartesiaTTS._postprocess_audio`."""
+        dtype = None
+        if data_rtype == AudioDataReturnType.ARRAY:
+            dtype = np.float32 if "fp32" in output_format.value else np.int16
+
+        async for chunk in generator:
+            if dtype is not None:
+                chunk["audio"] = np.frombuffer(chunk["audio"], dtype=dtype)
+            yield chunk
+
+    @retry_on_connection_error_async(
+        max_retries=MAX_RETRIES, backoff_factor=BACKOFF_FACTOR, logger=logger
+    )
     async def _generate_http_wrapper(self, body: Dict[str, Any]):
         """Need to wrap the http generator in a function for the retry decorator to work."""
         try:
-          async for chunk in self._generate_http(body):
-              yield chunk
+            async for chunk in self._generate_http(body):
+                yield chunk
         except Exception as e:
             logger.error(f"Failed to generate audio. {e}")
             raise e
 
     async def _generate_http(self, body: Dict[str, Any]):
         session = await self._get_session()
         async with session.post(
@@ -601,18 +649,14 @@
                     audio = base64.b64decode(chunk_json["data"])
                     yield {"audio": audio, "sampling_rate": chunk_json["sampling_rate"]}
                 except json.JSONDecodeError:
                     pass
 
     async def _generate_ws(self, body: Dict[str, Any], *, context_id: str = None):
         include_context_id = bool(context_id)
-        route = "audio/websocket"
-        if self.experimental_ws_handle_interrupts:
-            route = f"experimental/{route}"
-
         if not self.websocket or self._is_websocket_closed():
             await self.refresh_websocket()
 
         ws = self.websocket
         if context_id is None:
             context_id = uuid.uuid4().hex
         await ws.send_json({"data": body, "context_id": context_id})
@@ -620,47 +664,23 @@
             response = None
             while True:
                 response = await ws.receive_json()
                 if response["done"]:
                     break
 
                 yield convert_response(response, include_context_id)
-
-                if self.experimental_ws_handle_interrupts:
-                    await ws.send_json({"context_id": context_id})
-        except GeneratorExit:
-            # The exit is only called when the generator is garbage collected.
-            # It may not be called directly after a break statement.
-            # However, the generator will be automatically cancelled on the next request.
-            if self.experimental_ws_handle_interrupts:
-                await ws.send_json({"context_id": context_id, "action": "cancel"})
         except Exception as e:
             if self.websocket and not self._is_websocket_closed():
                 await self.websocket.close()
             raise RuntimeError(f"Failed to generate audio. {await response.text()}") from e
         finally:
             # Ensure the websocket is ultimately closed.
             if self.websocket and not self._is_websocket_closed():
                 await self.websocket.close()
 
-    async def transcribe(self, raw_audio: Union[bytes, str]) -> str:
-        raw_audio_bytes, headers = self.prepare_audio_and_headers(raw_audio)
-        data = aiohttp.FormData()
-        data.add_field("clip", raw_audio_bytes, filename="input.wav", content_type="audio/wav")
-        session = await self._get_session()
-
-        async with session.post(
-            f"{self._http_url()}/audio/transcriptions", headers=headers, data=data
-        ) as response:
-            if not response.ok:
-                raise ValueError(f"Failed to transcribe audio. Error: {await response.text()}")
-
-            transcript = await response.json()
-            return transcript["text"]
-        
     def __del__(self):
         try:
             loop = asyncio.get_running_loop()
         except RuntimeError:
             loop = None
 
         if loop is None:
```

### Comparing `cartesia-0.0.6/cartesia/utils.py` & `cartesia-0.1.0/cartesia/utils.py`

 * *Files 13% similar despite different names*

```diff
@@ -3,63 +3,85 @@
 from aiohttp.client_exceptions import ServerDisconnectedError
 import asyncio
 from functools import wraps
 from http.client import RemoteDisconnected
 from httpx import TimeoutException
 from requests.exceptions import ConnectionError
 
+
 def retry_on_connection_error(max_retries=3, backoff_factor=1, logger=None):
     """Retry a function if a ConnectionError, RemoteDisconnected, ServerDisconnectedError, or TimeoutException occurs.
 
     Args:
         max_retries (int): The maximum number of retries.
         backoff_factor (int): The factor to increase the delay between retries.
         logger (logging.Logger): The logger to use for logging.
     """
+
     def decorator(func):
         @wraps(func)
         def wrapper(*args, **kwargs):
             retry_count = 0
             while retry_count < max_retries:
                 try:
                     return func(*args, **kwargs)
-                except (ConnectionError, RemoteDisconnected, ServerDisconnectedError, TimeoutException) as e:
+                except (
+                    ConnectionError,
+                    RemoteDisconnected,
+                    ServerDisconnectedError,
+                    TimeoutException,
+                ) as e:
                     logger.info(f"Retrying after exception: {e}")
                     retry_count += 1
                     if retry_count < max_retries:
                         delay = backoff_factor * (2 ** (retry_count - 1))
-                        logger.warn(f"Attempt {retry_count + 1}/{max_retries} in {delay} seconds...")
+                        logger.warn(
+                            f"Attempt {retry_count + 1}/{max_retries} in {delay} seconds..."
+                        )
                         time.sleep(delay)
                     else:
                         raise Exception(f"Exception occurred after {max_retries} tries.") from e
+
         return wrapper
+
     return decorator
 
+
 def retry_on_connection_error_async(max_retries=3, backoff_factor=1, logger=None):
     """Retry an asynchronous function if a ConnectionError, RemoteDisconnected, ServerDisconnectedError, or TimeoutException occurs.
 
     Args:
         max_retries (int): The maximum number of retries.
         backoff_factor (int): The factor to increase the delay between retries.
         logger (logging.Logger): The logger to use for logging.
     """
+
     def decorator(func):
         @wraps(func)
         async def wrapper(*args, **kwargs):
             retry_count = 0
             while retry_count < max_retries:
                 try:
                     async for chunk in func(*args, **kwargs):
                         yield chunk
                     # If the function completes without raising an exception return
                     return
-                except (ConnectionError, RemoteDisconnected, ServerDisconnectedError, TimeoutException) as e:
+                except (
+                    ConnectionError,
+                    RemoteDisconnected,
+                    ServerDisconnectedError,
+                    TimeoutException,
+                ) as e:
                     logger.info(f"Retrying after exception: {e}")
                     retry_count += 1
                     if retry_count < max_retries:
                         delay = backoff_factor * (2 ** (retry_count - 1))
-                        logger.warn(f"Attempt {retry_count + 1}/{max_retries} in {delay} seconds...")
+                        logger.warn(
+                            f"Attempt {retry_count + 1}/{max_retries} in {delay} seconds..."
+                        )
                         await asyncio.sleep(delay)
                     else:
                         raise Exception(f"Exception occurred after {max_retries} tries.") from e
+
         return wrapper
-    return decorator
+
+    return decorator
```

### Comparing `cartesia-0.0.6/cartesia.egg-info/PKG-INFO` & `cartesia-0.1.0/cartesia.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: cartesia
-Version: 0.0.6
+Version: 0.1.0
 Summary: The official Python library for the Cartesia API.
 Home-page: 
 Author: Cartesia, Inc.
 Author-email: support@cartesia.ai
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3
 Classifier: Topic :: Scientific/Engineering :: Artificial Intelligence
```

### Comparing `cartesia-0.0.6/pyproject.toml` & `cartesia-0.1.0/pyproject.toml`

 * *Files identical despite different names*

### Comparing `cartesia-0.0.6/setup.py` & `cartesia-0.1.0/setup.py`

 * *Files identical despite different names*

