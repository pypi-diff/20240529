# Comparing `tmp/langchain_openai-0.1.8.tar.gz` & `tmp/langchain_openai-0.1.8rc1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "langchain_openai-0.1.8.tar", max compression
+gzip compressed data, was "langchain_openai-0.1.8rc1.tar", max compression
```

## Comparing `langchain_openai-0.1.8.tar` & `langchain_openai-0.1.8rc1.tar`

### file list

```diff
@@ -1,17 +1,17 @@
--rw-r--r--   0        0        0     1072 2024-05-29 20:21:34.042194 langchain_openai-0.1.8/LICENSE
--rw-r--r--   0        0        0     1627 2024-05-29 20:21:34.042194 langchain_openai-0.1.8/README.md
--rw-r--r--   0        0        0      371 2024-05-29 20:21:34.042194 langchain_openai-0.1.8/langchain_openai/__init__.py
--rw-r--r--   0        0        0      176 2024-05-29 20:21:34.042194 langchain_openai-0.1.8/langchain_openai/chat_models/__init__.py
--rw-r--r--   0        0        0    11220 2024-05-29 20:21:34.042194 langchain_openai-0.1.8/langchain_openai/chat_models/azure.py
--rw-r--r--   0        0        0    59989 2024-05-29 20:21:34.042194 langchain_openai-0.1.8/langchain_openai/chat_models/base.py
--rw-r--r--   0        0        0      198 2024-05-29 20:21:34.042194 langchain_openai-0.1.8/langchain_openai/embeddings/__init__.py
--rw-r--r--   0        0        0     6553 2024-05-29 20:21:34.042194 langchain_openai-0.1.8/langchain_openai/embeddings/azure.py
--rw-r--r--   0        0        0    24289 2024-05-29 20:21:34.042194 langchain_openai-0.1.8/langchain_openai/embeddings/base.py
--rw-r--r--   0        0        0      146 2024-05-29 20:21:34.042194 langchain_openai-0.1.8/langchain_openai/llms/__init__.py
--rw-r--r--   0        0        0     8340 2024-05-29 20:21:34.042194 langchain_openai-0.1.8/langchain_openai/llms/azure.py
--rw-r--r--   0        0        0    24651 2024-05-29 20:21:34.042194 langchain_openai-0.1.8/langchain_openai/llms/base.py
--rw-r--r--   0        0        0      229 2024-05-29 20:21:34.042194 langchain_openai-0.1.8/langchain_openai/output_parsers/__init__.py
--rw-r--r--   0        0        0      229 2024-05-29 20:21:34.042194 langchain_openai-0.1.8/langchain_openai/output_parsers/tools.py
--rw-r--r--   0        0        0        0 2024-05-29 20:21:34.046194 langchain_openai-0.1.8/langchain_openai/py.typed
--rw-r--r--   0        0        0     2838 2024-05-29 20:21:34.046194 langchain_openai-0.1.8/pyproject.toml
--rw-r--r--   0        0        0     2479 1970-01-01 00:00:00.000000 langchain_openai-0.1.8/PKG-INFO
+-rw-r--r--   0        0        0     1072 2024-05-23 19:14:32.777043 langchain_openai-0.1.8rc1/LICENSE
+-rw-r--r--   0        0        0     1627 2024-05-23 19:14:32.777043 langchain_openai-0.1.8rc1/README.md
+-rw-r--r--   0        0        0      371 2024-05-23 19:14:32.777043 langchain_openai-0.1.8rc1/langchain_openai/__init__.py
+-rw-r--r--   0        0        0      176 2024-05-23 19:14:32.777043 langchain_openai-0.1.8rc1/langchain_openai/chat_models/__init__.py
+-rw-r--r--   0        0        0    11220 2024-05-23 19:14:32.777043 langchain_openai-0.1.8rc1/langchain_openai/chat_models/azure.py
+-rw-r--r--   0        0        0    48383 2024-05-23 19:14:32.777043 langchain_openai-0.1.8rc1/langchain_openai/chat_models/base.py
+-rw-r--r--   0        0        0      198 2024-05-23 19:14:32.777043 langchain_openai-0.1.8rc1/langchain_openai/embeddings/__init__.py
+-rw-r--r--   0        0        0     6553 2024-05-23 19:14:32.777043 langchain_openai-0.1.8rc1/langchain_openai/embeddings/azure.py
+-rw-r--r--   0        0        0    24289 2024-05-23 19:14:32.777043 langchain_openai-0.1.8rc1/langchain_openai/embeddings/base.py
+-rw-r--r--   0        0        0      146 2024-05-23 19:14:32.777043 langchain_openai-0.1.8rc1/langchain_openai/llms/__init__.py
+-rw-r--r--   0        0        0     8340 2024-05-23 19:14:32.777043 langchain_openai-0.1.8rc1/langchain_openai/llms/azure.py
+-rw-r--r--   0        0        0    24651 2024-05-23 19:14:32.777043 langchain_openai-0.1.8rc1/langchain_openai/llms/base.py
+-rw-r--r--   0        0        0      229 2024-05-23 19:14:32.777043 langchain_openai-0.1.8rc1/langchain_openai/output_parsers/__init__.py
+-rw-r--r--   0        0        0      229 2024-05-23 19:14:32.777043 langchain_openai-0.1.8rc1/langchain_openai/output_parsers/tools.py
+-rw-r--r--   0        0        0        0 2024-05-23 19:14:32.777043 langchain_openai-0.1.8rc1/langchain_openai/py.typed
+-rw-r--r--   0        0        0     2879 2024-05-23 19:14:32.777043 langchain_openai-0.1.8rc1/pyproject.toml
+-rw-r--r--   0        0        0     2485 1970-01-01 00:00:00.000000 langchain_openai-0.1.8rc1/PKG-INFO
```

### Comparing `langchain_openai-0.1.8/LICENSE` & `langchain_openai-0.1.8rc1/LICENSE`

 * *Files identical despite different names*

### Comparing `langchain_openai-0.1.8/README.md` & `langchain_openai-0.1.8rc1/README.md`

 * *Files identical despite different names*

### Comparing `langchain_openai-0.1.8/langchain_openai/chat_models/azure.py` & `langchain_openai-0.1.8rc1/langchain_openai/chat_models/azure.py`

 * *Files identical despite different names*

### Comparing `langchain_openai-0.1.8/langchain_openai/chat_models/base.py` & `langchain_openai-0.1.8rc1/langchain_openai/chat_models/base.py`

 * *Files 21% similar despite different names*

```diff
@@ -54,15 +54,14 @@
     InvalidToolCall,
     SystemMessage,
     SystemMessageChunk,
     ToolCall,
     ToolMessage,
     ToolMessageChunk,
 )
-from langchain_core.messages.ai import UsageMetadata
 from langchain_core.output_parsers import (
     JsonOutputParser,
     PydanticOutputParser,
 )
 from langchain_core.output_parsers.base import OutputParserLike
 from langchain_core.output_parsers.openai_tools import (
     JsonOutputKeyToolsParser,
@@ -480,44 +479,31 @@
 
         default_chunk_class = AIMessageChunk
         with self.client.create(messages=message_dicts, **params) as response:
             for chunk in response:
                 if not isinstance(chunk, dict):
                     chunk = chunk.model_dump()
                 if len(chunk["choices"]) == 0:
-                    if token_usage := chunk.get("usage"):
-                        usage_metadata = UsageMetadata(
-                            input_tokens=token_usage.get("prompt_tokens", 0),
-                            output_tokens=token_usage.get("completion_tokens", 0),
-                            total_tokens=token_usage.get("total_tokens", 0),
-                        )
-                        chunk = ChatGenerationChunk(
-                            message=default_chunk_class(
-                                content="", usage_metadata=usage_metadata
-                            )
-                        )
-                    else:
-                        continue
-                else:
-                    choice = chunk["choices"][0]
-                    if choice["delta"] is None:
-                        continue
-                    chunk = _convert_delta_to_message_chunk(
-                        choice["delta"], default_chunk_class
-                    )
-                    generation_info = {}
-                    if finish_reason := choice.get("finish_reason"):
-                        generation_info["finish_reason"] = finish_reason
-                    logprobs = choice.get("logprobs")
-                    if logprobs:
-                        generation_info["logprobs"] = logprobs
-                    default_chunk_class = chunk.__class__
-                    chunk = ChatGenerationChunk(
-                        message=chunk, generation_info=generation_info or None
-                    )
+                    continue
+                choice = chunk["choices"][0]
+                if choice["delta"] is None:
+                    continue
+                chunk = _convert_delta_to_message_chunk(
+                    choice["delta"], default_chunk_class
+                )
+                generation_info = {}
+                if finish_reason := choice.get("finish_reason"):
+                    generation_info["finish_reason"] = finish_reason
+                logprobs = choice.get("logprobs")
+                if logprobs:
+                    generation_info["logprobs"] = logprobs
+                default_chunk_class = chunk.__class__
+                chunk = ChatGenerationChunk(
+                    message=chunk, generation_info=generation_info or None
+                )
                 if run_manager:
                     run_manager.on_llm_new_token(
                         chunk.text, chunk=chunk, logprobs=logprobs
                     )
                 yield chunk
 
     def _generate(
@@ -599,44 +585,31 @@
         default_chunk_class = AIMessageChunk
         response = await self.async_client.create(messages=message_dicts, **params)
         async with response:
             async for chunk in response:
                 if not isinstance(chunk, dict):
                     chunk = chunk.model_dump()
                 if len(chunk["choices"]) == 0:
-                    if token_usage := chunk.get("usage"):
-                        usage_metadata = UsageMetadata(
-                            input_tokens=token_usage.get("prompt_tokens", 0),
-                            output_tokens=token_usage.get("completion_tokens", 0),
-                            total_tokens=token_usage.get("total_tokens", 0),
-                        )
-                        chunk = ChatGenerationChunk(
-                            message=default_chunk_class(
-                                content="", usage_metadata=usage_metadata
-                            )
-                        )
-                    else:
-                        continue
-                else:
-                    choice = chunk["choices"][0]
-                    if choice["delta"] is None:
-                        continue
-                    chunk = _convert_delta_to_message_chunk(
-                        choice["delta"], default_chunk_class
-                    )
-                    generation_info = {}
-                    if finish_reason := choice.get("finish_reason"):
-                        generation_info["finish_reason"] = finish_reason
-                    logprobs = choice.get("logprobs")
-                    if logprobs:
-                        generation_info["logprobs"] = logprobs
-                    default_chunk_class = chunk.__class__
-                    chunk = ChatGenerationChunk(
-                        message=chunk, generation_info=generation_info or None
-                    )
+                    continue
+                choice = chunk["choices"][0]
+                if choice["delta"] is None:
+                    continue
+                chunk = _convert_delta_to_message_chunk(
+                    choice["delta"], default_chunk_class
+                )
+                generation_info = {}
+                if finish_reason := choice.get("finish_reason"):
+                    generation_info["finish_reason"] = finish_reason
+                logprobs = choice.get("logprobs")
+                if logprobs:
+                    generation_info["logprobs"] = logprobs
+                default_chunk_class = chunk.__class__
+                chunk = ChatGenerationChunk(
+                    message=chunk, generation_info=generation_info or None
+                )
                 if run_manager:
                     await run_manager.on_llm_new_token(
                         token=chunk.text, chunk=chunk, logprobs=logprobs
                     )
                 yield chunk
 
     async def _agenerate(
@@ -1113,282 +1086,29 @@
             )
             return RunnableMap(raw=llm) | parser_with_fallback
         else:
             return llm | output_parser
 
 
 class ChatOpenAI(BaseChatOpenAI):
-    """OpenAI chat model integration.
-
-    Setup:
-        Install ``langchain-openai`` and set environment variable ``OPENAI_API_KEY``.
+    """`OpenAI` Chat large language models API.
 
-        .. code-block:: bash
+    To use, you should have the environment variable ``OPENAI_API_KEY``
+    set with your API key, or pass it as a named parameter to the constructor.
 
-            pip install -U langchain-openai
-            export OPENAI_API_KEY="your-api-key"
-
-    Key init args — completion params:
-        model: str
-            Name of OpenAI model to use.
-        temperature: float
-            Sampling temperature.
-        max_tokens: Optional[int]
-            Max number of tokens to generate.
-        logprobs: Optional[bool]
-            Whether to return logprobs.
-        stream_options: Dict
-            Configure streaming outputs, like whether to return token usage when
-            streaming (``{"include_usage": True}``).
-
-    Key init args — client params:
-        timeout:
-            Timeout for requests.
-        max_retries:
-            Max number of retries.
-        api_key:
-            OpenAI API key. If not passed in will be read from env var OPENAI_API_KEY.
-        base_url:
-            Base URL for PAI requests. Only specify if using a proxy or service
-            emulator.
-        organization:
-            OpenAI organization ID. If not passed in will be read from env
-            var OPENAI_ORG_ID.
+    Any parameters that are valid to be passed to the openai.create call can be passed
+    in, even if not explicitly saved on this class.
 
-    See full list of supported init args and their descriptions in the params section.
-
-    Instantiate:
+    Example:
         .. code-block:: python
 
             from langchain_openai import ChatOpenAI
 
-            llm = ChatOpenAI(
-                model="gpt-4o",
-                temperature=0,
-                max_tokens=None,
-                timeout=None,
-                max_retries=2,
-                # api_key="...",
-                # base_url="...",
-                # organization="...",
-                # other params...
-            )
-
-    **NOTE**: Any param which is not explicitly supported will be passed directly to the
-    ``openai.OpenAI.chat.completions.create(...)`` API every time to the model is
-    invoked. For example:
-        .. code-block:: python
-
-            from langchain_openai import ChatOpenAI
-            import openai
-
-            ChatOpenAI(..., frequency_penalty=0.2).invoke(...)
-
-            # results in underlying API call of:
-
-            openai.OpenAI(..).chat.completions.create(..., frequency_penalty=0.2)
-
-            # which is also equivalent to:
-
-            ChatOpenAI(...).invoke(..., frequency_penalty=0.2)
-
-    Invoke:
-        .. code-block:: python
-
-            messages = [
-                ("system", "You are a helpful translator. Translate the user sentence to French."),
-                ("human", "I love programming."),
-            ]
-            llm.invoke(messages)
-
-        .. code-block:: python
-
-            AIMessage(content="J'adore la programmation.", response_metadata={'token_usage': {'completion_tokens': 5, 'prompt_tokens': 31, 'total_tokens': 36}, 'model_name': 'gpt-4o', 'system_fingerprint': 'fp_43dfabdef1', 'finish_reason': 'stop', 'logprobs': None}, id='run-012cffe2-5d3d-424d-83b5-51c6d4a593d1-0', usage_metadata={'input_tokens': 31, 'output_tokens': 5, 'total_tokens': 36})
-
-    Stream:
-        .. code-block:: python
-
-            for chunk in llm.stream(messages):
-                print(chunk)
-
-        .. code-block:: python
-
-            AIMessageChunk(content='', id='run-9e1517e3-12bf-48f2-bb1b-2e824f7cd7b0')
-            AIMessageChunk(content='J', id='run-9e1517e3-12bf-48f2-bb1b-2e824f7cd7b0')
-            AIMessageChunk(content="'adore", id='run-9e1517e3-12bf-48f2-bb1b-2e824f7cd7b0')
-            AIMessageChunk(content=' la', id='run-9e1517e3-12bf-48f2-bb1b-2e824f7cd7b0')
-            AIMessageChunk(content=' programmation', id='run-9e1517e3-12bf-48f2-bb1b-2e824f7cd7b0')
-            AIMessageChunk(content='.', id='run-9e1517e3-12bf-48f2-bb1b-2e824f7cd7b0')
-            AIMessageChunk(content='', response_metadata={'finish_reason': 'stop'}, id='run-9e1517e3-12bf-48f2-bb1b-2e824f7cd7b0')
-            AIMessageChunk(content='', id='run-9e1517e3-12bf-48f2-bb1b-2e824f7cd7b0', usage_metadata={'input_tokens': 31, 'output_tokens': 5, 'total_tokens': 36})
-
-        .. code-block:: python
-
-            stream = llm.stream(messages)
-            full = next(stream)
-            for chunk in stream:
-                full += chunk
-            full
-
-        .. code-block:: python
-
-            AIMessageChunk(content="J'adore la programmation.", response_metadata={'finish_reason': 'stop'}, id='run-bf917526-7f58-4683-84f7-36a6b671d140', usage_metadata={'input_tokens': 31, 'output_tokens': 5, 'total_tokens': 36})
-
-    Async:
-        .. code-block:: python
-
-            await llm.ainvoke(messages)
-
-            # stream:
-            # async for chunk in (await llm.astream(messages))
-
-            # batch:
-            # await llm.abatch([messages])
-
-        .. code-block:: python
-
-            AIMessage(content="J'adore la programmation.", response_metadata={'token_usage': {'completion_tokens': 5, 'prompt_tokens': 31, 'total_tokens': 36}, 'model_name': 'gpt-4o', 'system_fingerprint': 'fp_43dfabdef1', 'finish_reason': 'stop', 'logprobs': None}, id='run-012cffe2-5d3d-424d-83b5-51c6d4a593d1-0', usage_metadata={'input_tokens': 31, 'output_tokens': 5, 'total_tokens': 36})
-
-    Tool calling:
-        .. code-block:: python
-
-            from langchain_core.pydantic_v1 import BaseModel, Field
-
-            class GetWeather(BaseModel):
-                '''Get the current weather in a given location'''
-
-                location: str = Field(..., description="The city and state, e.g. San Francisco, CA")
-
-            class GetPopulation(BaseModel):
-                '''Get the current population in a given location'''
-
-                location: str = Field(..., description="The city and state, e.g. San Francisco, CA")
-
-            llm_with_tools = llm.bind_tools([GetWeather, GetPopulation])
-            ai_msg = llm_with_tools.invoke("Which city is hotter today and which is bigger: LA or NY?")
-            ai_msg.tool_calls
-
-        .. code-block:: python
-
-            [{'name': 'GetWeather',
-              'args': {'location': 'Los Angeles, CA'},
-              'id': 'call_6XswGD5Pqk8Tt5atYr7tfenU'},
-             {'name': 'GetWeather',
-              'args': {'location': 'New York, NY'},
-              'id': 'call_ZVL15vA8Y7kXqOy3dtmQgeCi'},
-             {'name': 'GetPopulation',
-              'args': {'location': 'Los Angeles, CA'},
-              'id': 'call_49CFW8zqC9W7mh7hbMLSIrXw'},
-             {'name': 'GetPopulation',
-              'args': {'location': 'New York, NY'},
-              'id': 'call_6ghfKxV264jEfe1mRIkS3PE7'}]
-
-        See ``ChatOpenAI.bind_tools()`` method for more.
-
-    Structured output:
-        .. code-block:: python
-
-            from typing import Optional
-
-            from langchain_core.pydantic_v1 import BaseModel, Field
-
-            class Joke(BaseModel):
-                '''Joke to tell user.'''
-
-                setup: str = Field(description="The setup of the joke")
-                punchline: str = Field(description="The punchline to the joke")
-                rating: Optional[int] = Field(description="How funny the joke is, from 1 to 10")
-
-            structured_llm = llm.with_structured_output(Joke)
-            structured_llm.invoke("Tell me a joke about cats")
-
-        .. code-block:: python
-
-            Joke(setup='Why was the cat sitting on the computer?', punchline='To keep an eye on the mouse!', rating=None)
-
-        See ``ChatOpenAI.with_structured_output()`` for more.
-
-    JSON mode:
-        .. code-block:: python
-
-            json_llm = llm.bind(response_format={"type": "json_object"})
-            ai_msg = json_llm.invoke("Return a JSON object with key 'random_ints' and a value of 10 random ints in [0-99]")
-            ai_msg.content
-
-        .. code-block:: python
-
-            '\\n{\\n  "random_ints": [23, 87, 45, 12, 78, 34, 56, 90, 11, 67]\\n}'
-
-    Image input:
-        .. code-block:: python
-
-            import base64
-            import httpx
-            from langchain_core.messages import HumanMessage
-
-            image_url = "https://upload.wikimedia.org/wikipedia/commons/thumb/d/dd/Gfp-wisconsin-madison-the-nature-boardwalk.jpg/2560px-Gfp-wisconsin-madison-the-nature-boardwalk.jpg"
-            image_data = base64.b64encode(httpx.get(image_url).content).decode("utf-8")
-            message = HumanMessage(
-                content=[
-                    {"type": "text", "text": "describe the weather in this image"},
-                    {
-                        "type": "image_url",
-                        "image_url": {"url": f"data:image/jpeg;base64,{image_data}"},
-                    },
-                ],
-            )
-            ai_msg = llm.invoke([message])
-            ai_msg.content
-
-        .. code-block:: python
-
-            "The weather in the image appears to be clear and pleasant. The sky is mostly blue with scattered, light clouds, suggesting a sunny day with minimal cloud cover. There is no indication of rain or strong winds, and the overall scene looks bright and calm. The lush green grass and clear visibility further indicate good weather conditions."
-
-    Token usage:
-        .. code-block:: python
-
-            ai_msg = llm.invoke(messages)
-            ai_msg.usage_metadata
-
-        .. code-block:: python
-
-            {'input_tokens': 28, 'output_tokens': 5, 'total_tokens': 33}
-
-    Logprobs:
-        .. code-block:: python
-
-            logprobs_llm = llm.bind(logprobs=True)
-            ai_msg = logprobs_llm.invoke(messages)
-            ai_msg.response_metadata["logprobs"]
-
-        .. code-block:: python
-
-            {'content': [{'token': 'J', 'bytes': [74], 'logprob': -4.9617593e-06, 'top_logprobs': []},
-              {'token': "'adore", 'bytes': [39, 97, 100, 111, 114, 101], 'logprob': -0.25202933, 'top_logprobs': []},
-              {'token': ' la', 'bytes': [32, 108, 97], 'logprob': -0.20141791, 'top_logprobs': []},
-              {'token': ' programmation', 'bytes': [32, 112, 114, 111, 103, 114, 97, 109, 109, 97, 116, 105, 111, 110], 'logprob': -1.9361265e-07, 'top_logprobs': []},
-              {'token': '.', 'bytes': [46], 'logprob': -1.2233183e-05, 'top_logprobs': []}]}
-
-    Response metadata
-        .. code-block:: python
-
-            ai_msg = llm.invoke(messages)
-            ai_msg.response_metadata
-
-        .. code-block:: python
-
-            {'token_usage': {'completion_tokens': 5,
-              'prompt_tokens': 28,
-              'total_tokens': 33},
-             'model_name': 'gpt-4o',
-             'system_fingerprint': 'fp_319be4768e',
-             'finish_reason': 'stop',
-             'logprobs': None}
-
-    """  # noqa: E501
+            model = ChatOpenAI(model="gpt-3.5-turbo")
+    """
 
     @property
     def lc_secrets(self) -> Dict[str, str]:
         return {"openai_api_key": "OPENAI_API_KEY"}
 
     @classmethod
     def get_lc_namespace(cls) -> List[str]:
```

#### encoding

```diff
@@ -1 +1 @@
-utf-8
+us-ascii
```

### Comparing `langchain_openai-0.1.8/langchain_openai/embeddings/azure.py` & `langchain_openai-0.1.8rc1/langchain_openai/embeddings/azure.py`

 * *Files identical despite different names*

### Comparing `langchain_openai-0.1.8/langchain_openai/embeddings/base.py` & `langchain_openai-0.1.8rc1/langchain_openai/embeddings/base.py`

 * *Files identical despite different names*

### Comparing `langchain_openai-0.1.8/langchain_openai/llms/azure.py` & `langchain_openai-0.1.8rc1/langchain_openai/llms/azure.py`

 * *Files identical despite different names*

### Comparing `langchain_openai-0.1.8/langchain_openai/llms/base.py` & `langchain_openai-0.1.8rc1/langchain_openai/llms/base.py`

 * *Files identical despite different names*

### Comparing `langchain_openai-0.1.8/pyproject.toml` & `langchain_openai-0.1.8rc1/pyproject.toml`

 * *Files 5% similar despite different names*

```diff
@@ -1,23 +1,23 @@
 [tool.poetry]
 name = "langchain-openai"
-version = "0.1.8"
+version = "0.1.8rc1"
 description = "An integration package connecting OpenAI and LangChain"
 authors = []
 readme = "README.md"
 repository = "https://github.com/langchain-ai/langchain"
 license = "MIT"
 
 [tool.poetry.urls]
 "Source Code" = "https://github.com/langchain-ai/langchain/tree/master/libs/partners/openai"
 
 [tool.poetry.dependencies]
 python = ">=3.8.1,<4.0"
-langchain-core = ">=0.2.2,<0.3"
-openai = "^1.26.0"
+langchain-core = {version =">=0.2.2rc1,<0.3", allow-prereleases=true}
+openai = "^1.24.0"
 tiktoken = ">=0.7,<1"
 
 [tool.poetry.group.test]
 optional = true
 
 [tool.poetry.group.test.dependencies]
 pytest = "^7.3.0"
```

### Comparing `langchain_openai-0.1.8/PKG-INFO` & `langchain_openai-0.1.8rc1/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,22 +1,22 @@
 Metadata-Version: 2.1
 Name: langchain-openai
-Version: 0.1.8
+Version: 0.1.8rc1
 Summary: An integration package connecting OpenAI and LangChain
 Home-page: https://github.com/langchain-ai/langchain
 License: MIT
 Requires-Python: >=3.8.1,<4.0
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: Python :: 3.12
-Requires-Dist: langchain-core (>=0.2.2,<0.3)
-Requires-Dist: openai (>=1.26.0,<2.0.0)
+Requires-Dist: langchain-core (>=0.2.2rc1,<0.3)
+Requires-Dist: openai (>=1.24.0,<2.0.0)
 Requires-Dist: tiktoken (>=0.7,<1)
 Project-URL: Repository, https://github.com/langchain-ai/langchain
 Project-URL: Source Code, https://github.com/langchain-ai/langchain/tree/master/libs/partners/openai
 Description-Content-Type: text/markdown
 
 # langchain-openai
```

