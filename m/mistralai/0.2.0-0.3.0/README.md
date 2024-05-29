# Comparing `tmp/mistralai-0.2.0.tar.gz` & `tmp/mistralai-0.3.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "mistralai-0.2.0.tar", max compression
+gzip compressed data, was "mistralai-0.3.0.tar", max compression
```

## Comparing `mistralai-0.2.0.tar` & `mistralai-0.3.0.tar`

### file list

```diff
@@ -1,16 +1,16 @@
--rw-r--r--   0        0        0    11357 2024-05-23 16:38:56.123877 mistralai-0.2.0/LICENSE
--rw-r--r--   0        0        0     1286 2024-05-23 16:38:56.123877 mistralai-0.2.0/README.md
--rw-r--r--   0        0        0      790 2024-05-23 16:38:56.127877 mistralai-0.2.0/pyproject.toml
--rw-r--r--   0        0        0        0 2024-05-23 16:38:56.127877 mistralai-0.2.0/src/mistralai/__init__.py
--rw-r--r--   0        0        0    11378 2024-05-23 16:38:56.127877 mistralai-0.2.0/src/mistralai/async_client.py
--rw-r--r--   0        0        0    11119 2024-05-23 16:38:56.127877 mistralai-0.2.0/src/mistralai/client.py
--rw-r--r--   0        0        0     4710 2024-05-23 16:38:56.127877 mistralai-0.2.0/src/mistralai/client_base.py
--rw-r--r--   0        0        0       84 2024-05-23 16:38:56.127877 mistralai-0.2.0/src/mistralai/constants.py
--rw-r--r--   0        0        0     1652 2024-05-23 16:38:56.127877 mistralai-0.2.0/src/mistralai/exceptions.py
--rw-r--r--   0        0        0        0 2024-05-23 16:38:56.127877 mistralai-0.2.0/src/mistralai/models/__init__.py
--rw-r--r--   0        0        0     1884 2024-05-23 16:38:56.127877 mistralai-0.2.0/src/mistralai/models/chat_completion.py
--rw-r--r--   0        0        0      172 2024-05-23 16:38:56.127877 mistralai-0.2.0/src/mistralai/models/common.py
--rw-r--r--   0        0        0      331 2024-05-23 16:38:56.127877 mistralai-0.2.0/src/mistralai/models/embeddings.py
--rw-r--r--   0        0        0      714 2024-05-23 16:38:56.127877 mistralai-0.2.0/src/mistralai/models/models.py
--rw-r--r--   0        0        0        0 2024-05-23 16:38:56.127877 mistralai-0.2.0/src/mistralai/py.typed
--rw-r--r--   0        0        0     1831 1970-01-01 00:00:00.000000 mistralai-0.2.0/PKG-INFO
+-rw-r--r--   0        0        0    11357 2024-05-29 14:09:46.474715 mistralai-0.3.0/LICENSE
+-rw-r--r--   0        0        0     1286 2024-05-29 14:09:46.474715 mistralai-0.3.0/README.md
+-rw-r--r--   0        0        0      790 2024-05-29 14:09:46.478715 mistralai-0.3.0/pyproject.toml
+-rw-r--r--   0        0        0        0 2024-05-29 14:09:46.478715 mistralai-0.3.0/src/mistralai/__init__.py
+-rw-r--r--   0        0        0    14984 2024-05-29 14:09:46.478715 mistralai-0.3.0/src/mistralai/async_client.py
+-rw-r--r--   0        0        0    14719 2024-05-29 14:09:46.478715 mistralai-0.3.0/src/mistralai/client.py
+-rw-r--r--   0        0        0     6349 2024-05-29 14:09:46.478715 mistralai-0.3.0/src/mistralai/client_base.py
+-rw-r--r--   0        0        0       84 2024-05-29 14:09:46.478715 mistralai-0.3.0/src/mistralai/constants.py
+-rw-r--r--   0        0        0     1652 2024-05-29 14:09:46.478715 mistralai-0.3.0/src/mistralai/exceptions.py
+-rw-r--r--   0        0        0        0 2024-05-29 14:09:46.478715 mistralai-0.3.0/src/mistralai/models/__init__.py
+-rw-r--r--   0        0        0     1884 2024-05-29 14:09:46.478715 mistralai-0.3.0/src/mistralai/models/chat_completion.py
+-rw-r--r--   0        0        0      172 2024-05-29 14:09:46.478715 mistralai-0.3.0/src/mistralai/models/common.py
+-rw-r--r--   0        0        0      331 2024-05-29 14:09:46.478715 mistralai-0.3.0/src/mistralai/models/embeddings.py
+-rw-r--r--   0        0        0      714 2024-05-29 14:09:46.478715 mistralai-0.3.0/src/mistralai/models/models.py
+-rw-r--r--   0        0        0        0 2024-05-29 14:09:46.478715 mistralai-0.3.0/src/mistralai/py.typed
+-rw-r--r--   0        0        0     1831 1970-01-01 00:00:00.000000 mistralai-0.3.0/PKG-INFO
```

### Comparing `mistralai-0.2.0/LICENSE` & `mistralai-0.3.0/LICENSE`

 * *Files identical despite different names*

### Comparing `mistralai-0.2.0/README.md` & `mistralai-0.3.0/README.md`

 * *Files identical despite different names*

### Comparing `mistralai-0.2.0/pyproject.toml` & `mistralai-0.3.0/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "mistralai"
-version = "0.2.0"
+version = "0.3.0"
 description = ""
 authors = ["Bam4d <bam4d@mistral.ai>"]
 readme = "README.md"
 
 [tool.ruff]
 select = ["E", "F", "W", "Q", "I"]
 ignore = ["E203"]
```

### Comparing `mistralai-0.2.0/src/mistralai/async_client.py` & `mistralai-0.3.0/src/mistralai/async_client.py`

 * *Files 17% similar despite different names*

```diff
@@ -88,15 +88,15 @@
             )
 
         return json_response
 
     async def _request(
         self,
         method: str,
-        json: Dict[str, Any],
+        json: Optional[Dict[str, Any]],
         path: str,
         stream: bool = False,
         attempt: int = 1,
     ) -> AsyncGenerator[Dict[str, Any], None]:
         accept_header = "text/event-stream" if stream else "application/json"
         headers = {
             "Accept": accept_header,
@@ -287,7 +287,78 @@
         """
         single_response = self._request("get", {}, "v1/models")
 
         async for response in single_response:
             return ModelList(**response)
 
         raise MistralException("No response received")
+
+    async def completion(
+        self,
+        model: str,
+        prompt: str,
+        suffix: Optional[str] = None,
+        temperature: Optional[float] = None,
+        max_tokens: Optional[int] = None,
+        top_p: Optional[float] = None,
+        random_seed: Optional[int] = None,
+        stop: Optional[List[str]] = None,
+    ) -> ChatCompletionResponse:
+        """An asynchronous completion endpoint that returns a single response.
+
+        Args:
+            model (str): model the name of the model to get completions with, e.g. codestral-latest
+            prompt (str): the prompt to complete
+            suffix (Optional[str]): the suffix to append to the prompt for fill-in-the-middle completion
+            temperature (Optional[float], optional): temperature the temperature to use for sampling, e.g. 0.5.
+            max_tokens (Optional[int], optional): the maximum number of tokens to generate, e.g. 100. Defaults to None.
+            top_p (Optional[float], optional): the cumulative probability of tokens to generate, e.g. 0.9.
+            Defaults to None.
+            random_seed (Optional[int], optional): the random seed to use for sampling, e.g. 42. Defaults to None.
+            stop (Optional[List[str]], optional): a list of tokens to stop generation at, e.g. ['/n/n']
+        Returns:
+            Dict[str, Any]: a response object containing the generated text.
+        """
+        request = self._make_completion_request(
+            prompt, model, suffix, temperature, max_tokens, top_p, random_seed, stop
+        )
+        single_response = self._request("post", request, "v1/fim/completions")
+
+        async for response in single_response:
+            return ChatCompletionResponse(**response)
+
+        raise MistralException("No response received")
+
+    async def completion_stream(
+        self,
+        model: str,
+        prompt: str,
+        suffix: Optional[str] = None,
+        temperature: Optional[float] = None,
+        max_tokens: Optional[int] = None,
+        top_p: Optional[float] = None,
+        random_seed: Optional[int] = None,
+        stop: Optional[List[str]] = None,
+    ) -> AsyncGenerator[ChatCompletionStreamResponse, None]:
+        """An asynchronous completion endpoint that returns a streaming response.
+
+        Args:
+            model (str): model the name of the model to get completions with, e.g. codestral-latest
+            prompt (str): the prompt to complete
+            suffix (Optional[str]): the suffix to append to the prompt for fill-in-the-middle completion
+            temperature (Optional[float], optional): temperature the temperature to use for sampling, e.g. 0.5.
+            max_tokens (Optional[int], optional): the maximum number of tokens to generate, e.g. 100. Defaults to None.
+            top_p (Optional[float], optional): the cumulative probability of tokens to generate, e.g. 0.9.
+            Defaults to None.
+            random_seed (Optional[int], optional): the random seed to use for sampling, e.g. 42. Defaults to None.
+            stop (Optional[List[str]], optional): a list of tokens to stop generation at, e.g. ['/n/n']
+
+        Returns:
+            Dict[str, Any]: a response object containing the generated text.
+        """
+        request = self._make_completion_request(
+            prompt, model, suffix, temperature, max_tokens, top_p, random_seed, stop, stream=True
+        )
+        async_response = self._request("post", request, "v1/fim/completions", stream=True)
+
+        async for json_response in async_response:
+            yield ChatCompletionStreamResponse(**json_response)
```

### Comparing `mistralai-0.2.0/src/mistralai/client.py` & `mistralai-0.3.0/src/mistralai/client.py`

 * *Files 18% similar despite different names*

```diff
@@ -81,15 +81,15 @@
             )
 
         return json_response
 
     def _request(
         self,
         method: str,
-        json: Dict[str, Any],
+        json: Optional[Dict[str, Any]],
         path: str,
         stream: bool = False,
         attempt: int = 1,
     ) -> Iterator[Dict[str, Any]]:
         accept_header = "text/event-stream" if stream else "application/json"
         headers = {
             "Accept": accept_header,
@@ -281,7 +281,81 @@
         """
         singleton_response = self._request("get", {}, "v1/models")
 
         for response in singleton_response:
             return ModelList(**response)
 
         raise MistralException("No response received")
+
+    def completion(
+        self,
+        model: str,
+        prompt: str,
+        suffix: Optional[str] = None,
+        temperature: Optional[float] = None,
+        max_tokens: Optional[int] = None,
+        top_p: Optional[float] = None,
+        random_seed: Optional[int] = None,
+        stop: Optional[List[str]] = None,
+    ) -> ChatCompletionResponse:
+        """A completion endpoint that returns a single response.
+
+        Args:
+            model (str): model the name of the model to get completion with, e.g. codestral-latest
+            prompt (str): the prompt to complete
+            suffix (Optional[str]): the suffix to append to the prompt for fill-in-the-middle completion
+            temperature (Optional[float], optional): temperature the temperature to use for sampling, e.g. 0.5.
+            max_tokens (Optional[int], optional): the maximum number of tokens to generate, e.g. 100. Defaults to None.
+            top_p (Optional[float], optional): the cumulative probability of tokens to generate, e.g. 0.9.
+            Defaults to None.
+            random_seed (Optional[int], optional): the random seed to use for sampling, e.g. 42. Defaults to None.
+            stop (Optional[List[str]], optional): a list of tokens to stop generation at, e.g. ['/n/n']
+
+        Returns:
+            Dict[str, Any]: a response object containing the generated text.
+        """
+        request = self._make_completion_request(
+            prompt, model, suffix, temperature, max_tokens, top_p, random_seed, stop
+        )
+
+        single_response = self._request("post", request, "v1/fim/completions", stream=False)
+
+        for response in single_response:
+            return ChatCompletionResponse(**response)
+
+        raise MistralException("No response received")
+
+    def completion_stream(
+        self,
+        model: str,
+        prompt: str,
+        suffix: Optional[str] = None,
+        temperature: Optional[float] = None,
+        max_tokens: Optional[int] = None,
+        top_p: Optional[float] = None,
+        random_seed: Optional[int] = None,
+        stop: Optional[List[str]] = None,
+    ) -> Iterable[ChatCompletionStreamResponse]:
+        """An asynchronous completion endpoint that streams responses.
+
+        Args:
+            model (str): model the name of the model to get completions with, e.g. codestral-latest
+            prompt (str): the prompt to complete
+            suffix (Optional[str]): the suffix to append to the prompt for fill-in-the-middle completion
+            temperature (Optional[float], optional): temperature the temperature to use for sampling, e.g. 0.5.
+            max_tokens (Optional[int], optional): the maximum number of tokens to generate, e.g. 100. Defaults to None.
+            top_p (Optional[float], optional): the cumulative probability of tokens to generate, e.g. 0.9.
+            Defaults to None.
+            random_seed (Optional[int], optional): the random seed to use for sampling, e.g. 42. Defaults to None.
+            stop (Optional[List[str]], optional): a list of tokens to stop generation at, e.g. ['/n/n']
+
+        Returns:
+            Iterable[Dict[str, Any]]: a generator that yields response objects containing the generated text.
+        """
+        request = self._make_completion_request(
+            prompt, model, suffix, temperature, max_tokens, top_p, random_seed, stop, stream=True
+        )
+
+        response = self._request("post", request, "v1/fim/completions", stream=True)
+
+        for json_streamed_response in response:
+            yield ChatCompletionStreamResponse(**json_streamed_response)
```

### Comparing `mistralai-0.2.0/src/mistralai/exceptions.py` & `mistralai-0.3.0/src/mistralai/exceptions.py`

 * *Files identical despite different names*

### Comparing `mistralai-0.2.0/src/mistralai/models/chat_completion.py` & `mistralai-0.3.0/src/mistralai/models/chat_completion.py`

 * *Files identical despite different names*

### Comparing `mistralai-0.2.0/src/mistralai/models/models.py` & `mistralai-0.3.0/src/mistralai/models/models.py`

 * *Files identical despite different names*

### Comparing `mistralai-0.2.0/PKG-INFO` & `mistralai-0.3.0/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: mistralai
-Version: 0.2.0
+Version: 0.3.0
 Summary: 
 Author: Bam4d
 Author-email: bam4d@mistral.ai
 Requires-Python: >=3.9,<4.0
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
```

