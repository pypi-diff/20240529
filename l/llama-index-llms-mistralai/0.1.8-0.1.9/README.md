# Comparing `tmp/llama_index_llms_mistralai-0.1.8.tar.gz` & `tmp/llama_index_llms_mistralai-0.1.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "llama_index_llms_mistralai-0.1.8.tar", max compression
+gzip compressed data, was "llama_index_llms_mistralai-0.1.9.tar", max compression
```

## Comparing `llama_index_llms_mistralai-0.1.8.tar` & `llama_index_llms_mistralai-0.1.9.tar`

### file list

```diff
@@ -1,6 +1,6 @@
--rw-r--r--   0        0        0       39 2024-03-23 20:44:18.636271 llama_index_llms_mistralai-0.1.8/README.md
--rw-r--r--   0        0        0       79 2024-03-23 20:44:18.636271 llama_index_llms_mistralai-0.1.8/llama_index/llms/mistralai/__init__.py
--rw-r--r--   0        0        0    16680 2024-03-23 20:44:18.636271 llama_index_llms_mistralai-0.1.8/llama_index/llms/mistralai/base.py
--rw-r--r--   0        0        0      873 2024-03-23 20:44:18.636271 llama_index_llms_mistralai-0.1.8/llama_index/llms/mistralai/utils.py
--rw-r--r--   0        0        0     1454 2024-03-23 20:44:18.636271 llama_index_llms_mistralai-0.1.8/pyproject.toml
--rw-r--r--   0        0        0      626 1970-01-01 00:00:00.000000 llama_index_llms_mistralai-0.1.8/PKG-INFO
+-rw-r--r--   0        0        0       39 2024-03-14 20:48:34.686354 llama_index_llms_mistralai-0.1.9/README.md
+-rw-r--r--   0        0        0       79 2024-03-14 20:48:34.686593 llama_index_llms_mistralai-0.1.9/llama_index/llms/mistralai/__init__.py
+-rw-r--r--   0        0        0    14779 2024-03-26 15:59:59.470935 llama_index_llms_mistralai-0.1.9/llama_index/llms/mistralai/base.py
+-rw-r--r--   0        0        0      873 2024-03-26 15:59:59.471084 llama_index_llms_mistralai-0.1.9/llama_index/llms/mistralai/utils.py
+-rw-r--r--   0        0        0     1455 2024-03-26 22:04:51.251232 llama_index_llms_mistralai-0.1.9/pyproject.toml
+-rw-r--r--   0        0        0      627 1970-01-01 00:00:00.000000 llama_index_llms_mistralai-0.1.9/PKG-INFO
```

### Comparing `llama_index_llms_mistralai-0.1.8/llama_index/llms/mistralai/base.py` & `llama_index_llms_mistralai-0.1.9/llama_index/llms/mistralai/base.py`

 * *Files 7% similar despite different names*

```diff
@@ -22,16 +22,17 @@
 from llama_index.core.base.llms.generic_utils import (
     achat_to_completion_decorator,
     astream_chat_to_completion_decorator,
     chat_to_completion_decorator,
     get_from_param_or_env,
     stream_chat_to_completion_decorator,
 )
-from llama_index.core.llms.llm import LLM, ToolSelection
+from llama_index.core.llms.llm import ToolSelection
 from llama_index.core.types import BaseOutputParser, PydanticProgramMode
+from llama_index.core.llms.function_calling import FunctionCallingLLM
 from llama_index.llms.mistralai.utils import (
     is_mistralai_function_calling_model,
     mistralai_modelname_to_contextsize,
 )
 
 from mistralai.async_client import MistralAsyncClient
 from mistralai.client import MistralClient
@@ -59,15 +60,21 @@
                 role=m.role.value, content=m.content, tool_calls=tool_calls
             )
         )
 
     return new_messages
 
 
-class MistralAI(LLM):
+def force_single_tool_call(response: ChatResponse) -> None:
+    tool_calls = response.message.additional_kwargs.get("tool_calls", [])
+    if len(tool_calls) > 1:
+        response.message.additional_kwargs["tool_calls"] = [tool_calls[0]]
+
+
+class MistralAI(FunctionCallingLLM):
     """MistralAI LLM.
 
     Examples:
         `pip install llama-index-llms-mistralai`
 
         ```python
         from llama_index.llms.mistralai import MistralAI
@@ -272,42 +279,14 @@
     @llm_completion_callback()
     def stream_complete(
         self, prompt: str, formatted: bool = False, **kwargs: Any
     ) -> CompletionResponseGen:
         stream_complete_fn = stream_chat_to_completion_decorator(self.stream_chat)
         return stream_complete_fn(prompt, **kwargs)
 
-    def predict_and_call(
-        self,
-        tools: List["BaseTool"],
-        user_msg: Optional[Union[str, ChatMessage]] = None,
-        chat_history: Optional[List[ChatMessage]] = None,
-        verbose: bool = False,
-        **kwargs: Any,
-    ) -> "AgentChatResponse":
-        from llama_index.core.tools.calling import (
-            call_tool_with_selection,
-        )
-
-        if not self.metadata.is_function_calling_model:
-            return super().predict_and_call(
-                tools,
-                user_msg=user_msg,
-                chat_history=chat_history,
-                verbose=verbose,
-                **kwargs,
-            )
-
-        response = self.chat_with_tool(
-            tools, user_msg, chat_history=chat_history, verbose=verbose, **kwargs
-        )
-        tool_call = self._get_tool_call_from_response(response)
-        tool_output = call_tool_with_selection(tool_call, tools, verbose=verbose)
-        return AgentChatResponse(response=tool_output.content, sources=[tool_output])
-
     @llm_chat_callback()
     async def achat(
         self, messages: Sequence[ChatMessage], **kwargs: Any
     ) -> ChatResponse:
         # convert messages to mistral ChatMessage
 
         messages = to_mistral_chatmessage(messages)
@@ -362,48 +341,21 @@
     @llm_completion_callback()
     async def astream_complete(
         self, prompt: str, formatted: bool = False, **kwargs: Any
     ) -> CompletionResponseAsyncGen:
         astream_complete_fn = astream_chat_to_completion_decorator(self.astream_chat)
         return await astream_complete_fn(prompt, **kwargs)
 
-    async def apredict_and_call(
-        self,
-        tools: List["BaseTool"],
-        user_msg: Optional[Union[str, ChatMessage]] = None,
-        chat_history: Optional[List[ChatMessage]] = None,
-        verbose: bool = False,
-        **kwargs: Any,
-    ) -> "AgentChatResponse":
-        from llama_index.core.tools.calling import (
-            acall_tool_with_selection,
-        )
-
-        if not self.metadata.is_function_calling_model:
-            return await super().predict_and_call(
-                tools,
-                user_msg=user_msg,
-                chat_history=chat_history,
-                verbose=verbose,
-                **kwargs,
-            )
-
-        response = await self.achat_with_tool(
-            tools, user_msg, chat_history=chat_history, verbose=verbose, **kwargs
-        )
-        tool_call = self._get_tool_call_from_response(response)
-        tool_output = acall_tool_with_selection(tool_call, tools, verbose=verbose)
-        return AgentChatResponse(response=tool_output.content, sources=[tool_output])
-
-    def chat_with_tool(
+    def chat_with_tools(
         self,
         tools: List["BaseTool"],
         user_msg: Optional[Union[str, ChatMessage]] = None,
         chat_history: Optional[List[ChatMessage]] = None,
         verbose: bool = False,
+        allow_parallel_tool_calls: bool = False,
         **kwargs: Any,
     ) -> ChatResponse:
         """Predict and call the tool."""
         # misralai uses the same openai tool format
         tool_specs = [tool.metadata.to_openai_tool() for tool in tools]
 
         if isinstance(user_msg, str):
@@ -414,26 +366,25 @@
             messages.append(user_msg)
 
         response = self.chat(
             messages,
             tools=tool_specs,
             **kwargs,
         )
-        # TODO: this is a hack, in the future we should support multiple tool calls
-        tool_calls = response.message.additional_kwargs.get("tool_calls", [])
-        if len(tool_calls) > 1:
-            response.message.additional_kwargs["tool_calls"] = [tool_calls[0]]
+        if not allow_parallel_tool_calls:
+            force_single_tool_call(response)
         return response
 
-    async def achat_with_tool(
+    async def achat_with_tools(
         self,
         tools: List["BaseTool"],
         user_msg: Optional[Union[str, ChatMessage]] = None,
         chat_history: Optional[List[ChatMessage]] = None,
         verbose: bool = False,
+        allow_parallel_tool_calls: bool = False,
         **kwargs: Any,
     ) -> ChatResponse:
         """Predict and call the tool."""
         # misralai uses the same openai tool format
         tool_specs = [tool.metadata.to_openai_tool() for tool in tools]
 
         if isinstance(user_msg, str):
@@ -444,44 +395,44 @@
             messages.append(user_msg)
 
         response = await self.achat(
             messages,
             tools=tool_specs,
             **kwargs,
         )
-        # TODO: this is a hack, in the future we should support multiple tool calls
-        tool_calls = response.message.additional_kwargs.get("tool_calls", [])
-        if len(tool_calls) > 1:
-            response.message.additional_kwargs["tool_calls"] = [tool_calls[0]]
+        if not allow_parallel_tool_calls:
+            force_single_tool_call(response)
         return response
 
-    def _get_tool_call_from_response(
+    def get_tool_calls_from_response(
         self,
         response: "AgentChatResponse",
         error_on_no_tool_call: bool = True,
-    ) -> Optional[ToolSelection]:
+    ) -> List[ToolSelection]:
         """Predict and call the tool."""
         tool_calls = response.message.additional_kwargs.get("tool_calls", [])
 
         if len(tool_calls) < 1:
             if error_on_no_tool_call:
                 raise ValueError(
                     f"Expected at least one tool call, but got {len(tool_calls)} tool calls."
                 )
             else:
-                return None
+                return []
 
-        # TODO: support more than one tool call?
-        tool_call = tool_calls[0]
-        if not isinstance(tool_call, ToolCall):
-            raise ValueError("Invalid tool_call object")
-
-        if tool_call.type != "function":
-            raise ValueError("Invalid tool type. Unsupported by Mistralai.")
-
-        argument_dict = json.loads(tool_call.function.arguments)
-
-        return ToolSelection(
-            tool_id=tool_call.id,
-            tool_name=tool_call.function.name,
-            tool_kwargs=argument_dict,
-        )
+        tool_selections = []
+        for tool_call in tool_calls:
+            if not isinstance(tool_call, ToolCall):
+                raise ValueError("Invalid tool_call object")
+            if tool_call.type != "function":
+                raise ValueError("Invalid tool type. Unsupported by Mistralai.")
+            argument_dict = json.loads(tool_call.function.arguments)
+
+            tool_selections.append(
+                ToolSelection(
+                    tool_id=tool_call.id,
+                    tool_name=tool_call.function.name,
+                    tool_kwargs=argument_dict,
+                )
+            )
+
+        return tool_selections
```

### Comparing `llama_index_llms_mistralai-0.1.8/llama_index/llms/mistralai/utils.py` & `llama_index_llms_mistralai-0.1.9/llama_index/llms/mistralai/utils.py`

 * *Files identical despite different names*

### Comparing `llama_index_llms_mistralai-0.1.8/pyproject.toml` & `llama_index_llms_mistralai-0.1.9/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -23,19 +23,19 @@
 [tool.poetry]
 authors = ["Your Name <you@example.com>"]
 description = "llama-index llms mistral ai integration"
 exclude = ["**/BUILD"]
 license = "MIT"
 name = "llama-index-llms-mistralai"
 readme = "README.md"
-version = "0.1.8"
+version = "0.1.9"
 
 [tool.poetry.dependencies]
 python = ">=3.9,<4.0"
-llama-index-core = "^0.10.1"
+llama-index-core = "^0.10.24"
 mistralai = ">=0.1.3"
 
 [tool.poetry.group.dev.dependencies]
 ipython = "8.10.0"
 jupyter = "^1.0.0"
 mypy = "0.991"
 pre-commit = "3.2.0"
```

### Comparing `llama_index_llms_mistralai-0.1.8/PKG-INFO` & `llama_index_llms_mistralai-0.1.9/PKG-INFO`

 * *Files 17% similar despite different names*

```diff
@@ -1,19 +1,19 @@
 Metadata-Version: 2.1
 Name: llama-index-llms-mistralai
-Version: 0.1.8
+Version: 0.1.9
 Summary: llama-index llms mistral ai integration
 License: MIT
 Author: Your Name
 Author-email: you@example.com
 Requires-Python: >=3.9,<4.0
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
-Requires-Dist: llama-index-core (>=0.10.1,<0.11.0)
+Requires-Dist: llama-index-core (>=0.10.24,<0.11.0)
 Requires-Dist: mistralai (>=0.1.3)
 Description-Content-Type: text/markdown
 
 # LlamaIndex Llms Integration: Mistral
```

