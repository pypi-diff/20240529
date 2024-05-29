# Comparing `tmp/log10_io-0.8.4.tar.gz` & `tmp/log10_io-0.8.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "log10_io-0.8.4.tar", max compression
+gzip compressed data, was "log10_io-0.8.5.tar", max compression
```

## Comparing `log10_io-0.8.4.tar` & `log10_io-0.8.5.tar`

### file list

```diff
@@ -1,29 +1,29 @@
--rw-r--r--   0        0        0     1083 2024-04-29 19:07:55.897681 log10_io-0.8.4/LICENSE
--rw-r--r--   0        0        0     9613 2024-04-29 19:07:55.897681 log10_io-0.8.4/README.md
--rw-r--r--   0        0        0        0 2024-04-29 19:07:55.901681 log10_io-0.8.4/log10/__init__.py
--rw-r--r--   0        0        0     1550 2024-04-29 19:07:55.901681 log10_io-0.8.4/log10/__main__.py
--rw-r--r--   0        0        0    11352 2024-04-29 19:07:55.901681 log10_io-0.8.4/log10/_httpx_utils.py
--rw-r--r--   0        0        0     9112 2024-04-29 19:07:55.901681 log10_io-0.8.4/log10/agents/camel.py
--rw-r--r--   0        0        0      722 2024-04-29 19:07:55.901681 log10_io-0.8.4/log10/agents/scrape_summarizer.py
--rw-r--r--   0        0        0     6079 2024-04-29 19:07:55.901681 log10_io-0.8.4/log10/anthropic.py
--rw-r--r--   0        0        0     2578 2024-04-29 19:07:55.901681 log10_io-0.8.4/log10/bigquery.py
--rw-r--r--   0        0        0      719 2024-04-29 19:07:55.901681 log10_io-0.8.4/log10/cli_utils.py
--rw-r--r--   0        0        0    22337 2024-04-29 19:07:55.901681 log10_io-0.8.4/log10/completions/completions.py
--rw-r--r--   0        0        0     2648 2024-04-29 19:07:55.901681 log10_io-0.8.4/log10/evals.py
--rw-r--r--   0        0        0     5459 2024-04-29 19:07:55.901681 log10_io-0.8.4/log10/feedback/_summary_feedback_utils.py
--rw-r--r--   0        0        0     4487 2024-04-29 19:07:55.901681 log10_io-0.8.4/log10/feedback/autofeedback.py
--rw-r--r--   0        0        0     8357 2024-04-29 19:07:55.901681 log10_io-0.8.4/log10/feedback/feedback.py
--rw-r--r--   0        0        0     5206 2024-04-29 19:07:55.901681 log10_io-0.8.4/log10/feedback/feedback_task.py
--rw-r--r--   0        0        0     9274 2024-04-29 19:07:55.901681 log10_io-0.8.4/log10/langchain.py
--rw-r--r--   0        0        0     4432 2024-04-29 19:07:55.901681 log10_io-0.8.4/log10/litellm.py
--rw-r--r--   0        0        0     7967 2024-04-29 19:07:55.901681 log10_io-0.8.4/log10/llm.py
--rw-r--r--   0        0        0    39993 2024-04-29 19:07:55.901681 log10_io-0.8.4/log10/load.py
--rw-r--r--   0        0        0     2886 2024-04-29 19:07:55.901681 log10_io-0.8.4/log10/mosaicml.py
--rw-r--r--   0        0        0     3217 2024-04-29 19:07:55.901681 log10_io-0.8.4/log10/openai.py
--rw-r--r--   0        0        0     6915 2024-04-29 19:07:55.901681 log10_io-0.8.4/log10/prompt_analyzer.py
--rw-r--r--   0        0        0     1020 2024-04-29 19:07:55.901681 log10_io-0.8.4/log10/schemas/bigquery.json
--rw-r--r--   0        0        0     2654 2024-04-29 19:07:55.901681 log10_io-0.8.4/log10/together.py
--rw-r--r--   0        0        0     2101 2024-04-29 19:07:55.901681 log10_io-0.8.4/log10/tools.py
--rw-r--r--   0        0        0     1211 2024-04-29 19:07:55.901681 log10_io-0.8.4/log10/utils.py
--rw-r--r--   0        0        0     2242 2024-04-29 19:07:55.901681 log10_io-0.8.4/pyproject.toml
--rw-r--r--   0        0        0    11109 1970-01-01 00:00:00.000000 log10_io-0.8.4/PKG-INFO
+-rw-r--r--   0        0        0     1083 2024-05-28 20:33:58.037552 log10_io-0.8.5/LICENSE
+-rw-r--r--   0        0        0     9613 2024-05-28 20:33:58.037552 log10_io-0.8.5/README.md
+-rw-r--r--   0        0        0        0 2024-05-28 20:33:58.041552 log10_io-0.8.5/log10/__init__.py
+-rw-r--r--   0        0        0     1550 2024-05-28 20:33:58.041552 log10_io-0.8.5/log10/__main__.py
+-rw-r--r--   0        0        0    17691 2024-05-28 20:33:58.041552 log10_io-0.8.5/log10/_httpx_utils.py
+-rw-r--r--   0        0        0     9112 2024-05-28 20:33:58.041552 log10_io-0.8.5/log10/agents/camel.py
+-rw-r--r--   0        0        0      722 2024-05-28 20:33:58.041552 log10_io-0.8.5/log10/agents/scrape_summarizer.py
+-rw-r--r--   0        0        0     6680 2024-05-28 20:33:58.041552 log10_io-0.8.5/log10/anthropic.py
+-rw-r--r--   0        0        0     2578 2024-05-28 20:33:58.041552 log10_io-0.8.5/log10/bigquery.py
+-rw-r--r--   0        0        0      719 2024-05-28 20:33:58.041552 log10_io-0.8.5/log10/cli_utils.py
+-rw-r--r--   0        0        0    22376 2024-05-28 20:33:58.041552 log10_io-0.8.5/log10/completions/completions.py
+-rw-r--r--   0        0        0     2648 2024-05-28 20:33:58.041552 log10_io-0.8.5/log10/evals.py
+-rw-r--r--   0        0        0     5459 2024-05-28 20:33:58.041552 log10_io-0.8.5/log10/feedback/_summary_feedback_utils.py
+-rw-r--r--   0        0        0     4487 2024-05-28 20:33:58.041552 log10_io-0.8.5/log10/feedback/autofeedback.py
+-rw-r--r--   0        0        0     8357 2024-05-28 20:33:58.041552 log10_io-0.8.5/log10/feedback/feedback.py
+-rw-r--r--   0        0        0     5206 2024-05-28 20:33:58.041552 log10_io-0.8.5/log10/feedback/feedback_task.py
+-rw-r--r--   0        0        0     9274 2024-05-28 20:33:58.041552 log10_io-0.8.5/log10/langchain.py
+-rw-r--r--   0        0        0     4432 2024-05-28 20:33:58.041552 log10_io-0.8.5/log10/litellm.py
+-rw-r--r--   0        0        0     7967 2024-05-28 20:33:58.041552 log10_io-0.8.5/log10/llm.py
+-rw-r--r--   0        0        0    44497 2024-05-28 20:33:58.041552 log10_io-0.8.5/log10/load.py
+-rw-r--r--   0        0        0     2886 2024-05-28 20:33:58.041552 log10_io-0.8.5/log10/mosaicml.py
+-rw-r--r--   0        0        0     3217 2024-05-28 20:33:58.041552 log10_io-0.8.5/log10/openai.py
+-rw-r--r--   0        0        0     6915 2024-05-28 20:33:58.041552 log10_io-0.8.5/log10/prompt_analyzer.py
+-rw-r--r--   0        0        0     1020 2024-05-28 20:33:58.041552 log10_io-0.8.5/log10/schemas/bigquery.json
+-rw-r--r--   0        0        0     2654 2024-05-28 20:33:58.041552 log10_io-0.8.5/log10/together.py
+-rw-r--r--   0        0        0     2101 2024-05-28 20:33:58.041552 log10_io-0.8.5/log10/tools.py
+-rw-r--r--   0        0        0     1211 2024-05-28 20:33:58.041552 log10_io-0.8.5/log10/utils.py
+-rw-r--r--   0        0        0     2597 2024-05-28 20:33:58.045552 log10_io-0.8.5/pyproject.toml
+-rw-r--r--   0        0        0    11290 1970-01-01 00:00:00.000000 log10_io-0.8.5/PKG-INFO
```

### Comparing `log10_io-0.8.4/LICENSE` & `log10_io-0.8.5/LICENSE`

 * *Files identical despite different names*

### Comparing `log10_io-0.8.4/README.md` & `log10_io-0.8.5/README.md`

 * *Files identical despite different names*

### Comparing `log10_io-0.8.4/log10/__main__.py` & `log10_io-0.8.5/log10/__main__.py`

 * *Files identical despite different names*

### Comparing `log10_io-0.8.4/log10/_httpx_utils.py` & `log10_io-0.8.5/log10/_httpx_utils.py`

 * *Files 26% similar despite different names*

```diff
@@ -5,15 +5,15 @@
 import uuid
 from datetime import datetime, timezone
 
 import httpx
 from httpx import Request, Response
 
 from log10.llm import Log10Config
-from log10.load import get_log10_session_tags, sessionID
+from log10.load import get_log10_session_tags, session_id_var
 
 
 logger: logging.Logger = logging.getLogger("LOG10")
 
 
 _log10_config = Log10Config()
 base_url = _log10_config.url
@@ -104,60 +104,99 @@
             )
         else:
             logger.error(f"Failed with error: {http_err}")
     except Exception as err:
         logger.error(f"Failed to insert in log10: {payload} with error {err}")
 
 
+def format_anthropic_tools_request(request_content) -> str:
+    new_tools = []
+    for tool in request_content["tools"]:
+        new_tool = {
+            "type": "function",
+            "function": {"name": tool["name"], "description": tool["description"], "parameters": tool["input_schema"]},
+        }
+        new_tools.append(new_tool)
+    request_content["tools"] = new_tools
+    return json.dumps(request_content)
+
+
 async def get_completion_id(request: Request):
-    if "v1/chat/completions" not in str(request.url):
-        logger.warning("Currently logging is only available for v1/chat/completions.")
+    host = request.headers.get("host")
+    if "anthropic" in host and "/v1/messages" not in str(request.url):
+        logger.warning("Currently logging is only available for anthropic v1/messages.")
+        return
+
+    if "openai" in host and "v1/chat/completions" not in str(request.url):
+        logger.warning("Currently logging is only available for openai v1/chat/completions.")
         return
 
     request.headers["x-log10-completion-id"] = str(uuid.uuid4())
 
 
 async def log_request(request: Request):
     start_time = time.time()
     request.started = start_time
     completion_id = request.headers.get("x-log10-completion-id", "")
     if not completion_id:
         return
 
     orig_module = ""
     orig_qualname = ""
-    if "chat" in str(request.url):
+    request_content_decode = request.content.decode("utf-8")
+    host = request.headers.get("host")
+    if "openai" in host:
+        if "chat" in str(request.url):
+            kind = "chat"
+            orig_module = "openai.api_resources.chat_completion"
+            orig_qualname = "ChatCompletion.create"
+        else:
+            kind = "completion"
+            orig_module = "openai.api_resources.completion"
+            orig_qualname = "Completion.create"
+    elif "anthropic" in host:
         kind = "chat"
-        orig_module = "openai.api_resources.chat_completion"
-        orig_qualname = "ChatCompletion.create"
+        request_content = json.loads(request_content_decode)
+        if "tools" in request_content:
+            orig_module = "anthropic.resources.beta.tools"
+            orig_qualname = "Messages.stream"
+            request_content_decode = format_anthropic_tools_request(request_content)
+        else:
+            orig_module = "anthropic.resources.messages"
+            orig_qualname = "Messages.stream"
     else:
-        kind = "completion"
-        orig_module = "openai.api_resources.completion"
-        orig_qualname = "Completion.create"
+        logger.warning("Currently logging is only available for async openai and anthropic.")
+        return
     log_row = {
         "status": "started",
         "kind": kind,
         "orig_module": orig_module,
         "orig_qualname": orig_qualname,
-        "request": request.content.decode("utf-8"),
-        "session_id": sessionID,
+        "request": request_content_decode,
+        "session_id": session_id_var.get(),
     }
     if get_log10_session_tags():
         log_row["tags"] = get_log10_session_tags()
     await _try_post_request_async(url=f"{base_url}/api/completions/{completion_id}", payload=log_row)
 
 
 class _LogResponse(Response):
+    def __init__(self, *args, **kwargs):
+        super().__init__(*args, **kwargs)
+        self.full_content = ""
+        self.function_name = ""
+        self.full_argument = ""
+        self.tool_calls = []
+
     async def aiter_bytes(self, *args, **kwargs):
         full_response = ""
         finished = False
         async for chunk in super().aiter_bytes(*args, **kwargs):
             full_response += chunk.decode(errors="ignore")
-
-            if "data: [DONE]" in full_response:
+            if self.is_response_end_reached(full_response):
                 finished = True
                 duration = int(time.time() - self.request.started) * 1000
 
                 completion_id = self.request.headers.get("x-log10-completion-id", "")
                 if finished and completion_id:
                     current_stack_frame = traceback.extract_stack()
                     stacktrace = [
@@ -165,89 +204,203 @@
                             "file": frame.filename,
                             "line": frame.line,
                             "lineno": frame.lineno,
                             "name": frame.name,
                         }
                         for frame in current_stack_frame
                     ]
-                    full_content = ""
-                    function_name = ""
-                    full_argument = ""
-                    tool_calls = []
+
                     responses = full_response.split("\n\n")
-                    for r in responses:
-                        if "data: [DONE]" in r:
-                            break
-
-                        r_json = json.loads(r[6:])
-
-                        delta = r_json["choices"][0]["delta"]
-
-                        # Delta may have content
-                        if "content" in delta:
-                            content = delta["content"]
-                            if content:
-                                full_content += content
-
-                        # May be a function call, and have to reconstruct the arguments
-                        if "function_call" in delta:
-                            # May be function name
-                            if "name" in delta["function_call"]:
-                                function_name = delta["function_call"]["name"]
-                            # May be function arguments
-                            if "arguments" in delta["function_call"]:
-                                full_argument += delta["function_call"]["arguments"]
-
-                        if tc := delta.get("tool_calls", []):
-                            if tc[0].get("id", ""):
-                                tool_calls.append(tc[0])
-                            elif tc[0].get("function", {}).get("arguments", ""):
-                                idx = tc[0].get("index")
-                                tool_calls[idx]["function"]["arguments"] += tc[0]["function"]["arguments"]
+                    r_json = self.parse_response_data(responses)
 
                     response_json = r_json.copy()
-                    response_json["object"] = "chat.completion"
                     # r_json is the last response before "data: [DONE]"
 
-                    if full_content:
-                        response_json["choices"][0]["message"] = {"role": "assistant", "content": full_content}
-                    elif tool_calls:
+                    if self.full_content:
+                        response_json["choices"][0]["message"] = {"role": "assistant", "content": self.full_content}
+                    elif self.tool_calls:
                         response_json["choices"][0]["message"] = {
                             "content": None,
                             "role": "assistant",
-                            "tool_calls": tool_calls,
+                            "tool_calls": self.tool_calls,
                         }
-                    elif function_name and full_argument:
+                    elif self.function_name and self.full_argument:
                         # function is deprecated in openai api
                         response_json["choices"][0]["function_call"] = {
-                            "name": function_name,
-                            "arguments": full_argument,
+                            "name": self.function_name,
+                            "arguments": self.full_argument,
                         }
 
+                    request_content_decode = self.request.content.decode("utf-8")
+                    if "anthropic" in self.request.headers.get("host"):
+                        request_content = json.loads(request_content_decode)
+                        if "tools" in request_content:
+                            request_content_decode = format_anthropic_tools_request(request_content)
+
                     log_row = {
                         "response": json.dumps(response_json),
                         "status": "finished",
                         "duration": duration,
                         "stacktrace": json.dumps(stacktrace),
                         "kind": "chat",
-                        "request": self.request.content.decode("utf-8"),
-                        "session_id": sessionID,
+                        "request": request_content_decode,
+                        "session_id": session_id_var.get(),
                     }
                     if get_log10_session_tags():
                         log_row["tags"] = get_log10_session_tags()
                     await _try_post_request_async(url=f"{base_url}/api/completions/{completion_id}", payload=log_row)
             yield chunk
 
+    def is_response_end_reached(self, text: str):
+        host = self.request.headers.get("host")
+        if "anthropic" in host:
+            return self.is_anthropic_response_end_reached(text)
+        elif "openai" in host:
+            return self.is_openai_response_end_reached(text)
+        else:
+            logger.warning("Currently logging is only available for async openai and anthropic.")
+            return False
+
+    def is_anthropic_response_end_reached(self, text: str):
+        return "event: message_stop" in text
+
+    def is_openai_response_end_reached(self, text: str):
+        return "data: [DONE]" in text
+
+    def parse_anthropic_responses(self, responses: list[str]):
+        message_id = None
+        model = None
+        finish_reason = None
+        input_tokens = 0
+        output_tokens = 0
+        tool_call = {}
+        arguments = ""
+        for r in responses:
+            if not r:
+                break
+
+            data_index = r.find("data:")
+            r_json = json.loads(r[data_index + len("data:") :])
+
+            ### anthropic first data contains
+            ### {"event":"message_start","data":{"message":{"role":"user","content":"Hello, how are you today?"}}}
+            type = r_json["type"]
+            if type == "message_start":
+                message_id = r_json["message"]["id"]
+                model = r_json["message"]["model"]
+                input_tokens = r_json["message"]["usage"]["input_tokens"]
+            elif type == "content_block_start":
+                content_block = r_json["content_block"]
+                type = content_block["type"]
+                if type == "tool_use":
+                    id = content_block["id"]
+                    tool_call = {
+                        "id": id,
+                        "type": "function",
+                        "function": {"name": content_block["name"], "arguments": ""},
+                    }
+                if "text" in content_block:
+                    self.full_content += content_block["text"]
+            elif type == "content_block_delta":
+                delta = r_json["delta"]
+                if "text" in delta:
+                    self.full_content += delta["text"]
+                if "partial_json" in delta:
+                    if self.full_content:
+                        self.full_content += delta["partial_json"]
+                    else:
+                        arguments += delta["partial_json"]
+            elif type == "message_delta":
+                finish_reason = r_json["delta"]["stop_reason"]
+                output_tokens = r_json["usage"]["output_tokens"]
+            elif type == "content_block_end" or type == "message_end":
+                if tool_call:
+                    tool_call["function"]["arguments"] = arguments
+                    self.tool_calls.append(tool_call)
+                    tool_call = {}
+                    arguments = ""
+
+        return {
+            "id": message_id,
+            "object": "chat",
+            "model": model,
+            "choices": [
+                {
+                    "index": 0,
+                    "finish_reason": finish_reason,
+                }
+            ],
+            "usage": {
+                "prompt_tokens": input_tokens,
+                "completion_tokens": output_tokens,
+                "total_tokens": input_tokens + output_tokens,
+            },
+        }
+
+    def parse_openai_responses(self, responses: list[str]):
+        r_json = None
+        for r in responses:
+            if self.is_openai_response_end_reached(r):
+                break
+
+            # loading the substring of response text after 'data: '.
+            # example: 'data: {"choices":[{"text":"Hello, how can I help you today?"}]}'
+            r_json = json.loads(r[6:])
+            delta = r_json["choices"][0]["delta"]
+
+            # Delta may have content
+            if "content" in delta:
+                content = delta["content"]
+                if content:
+                    self.full_content += content
+
+            # May be a function call, and have to reconstruct the arguments
+            if "function_call" in delta:
+                # May be function name
+                if "name" in delta["function_call"]:
+                    self.function_name = delta["function_call"]["name"]
+                # May be function arguments
+                if "arguments" in delta["function_call"]:
+                    self.full_argument += delta["function_call"]["arguments"]
+
+            if tc := delta.get("tool_calls", []):
+                if tc[0].get("id", ""):
+                    self.tool_calls.append(tc[0])
+                elif tc[0].get("function", {}).get("arguments", ""):
+                    idx = tc[0].get("index")
+                    self.tool_calls[idx]["function"]["arguments"] += tc[0]["function"]["arguments"]
+
+        r_json["object"] = "chat.completion"
+        return r_json
+
+    def parse_response_data(self, responses: list[str]):
+        host = self.request.headers.get("host")
+        if "openai" in host:
+            return self.parse_openai_responses(responses)
+        elif "anthropic" in host:
+            return self.parse_anthropic_responses(responses)
+        else:
+            logger.warning("Currently logging is only available for async openai and anthropic.")
+            return None
+
 
 class _LogTransport(httpx.AsyncBaseTransport):
     def __init__(self, transport: httpx.AsyncBaseTransport):
         self.transport = transport
 
     async def handle_async_request(self, request: httpx.Request) -> httpx.Response:
-        response = await self.transport.handle_async_request(request)
+        try:
+            response = await self.transport.handle_async_request(request)
+        except Exception as e:
+            logger.warning(f"Failed to send request: {e}")
+            return
+
+        if response.status_code >= 400:
+            logger.warning(f"HTTP error occurred: {response.status_code}")
+            return
 
         completion_id = request.headers.get("x-log10-completion-id", "")
         if not completion_id:
             return response
 
         if response.headers.get("content-type").startswith("application/json"):
             await response.aread()
@@ -261,22 +414,31 @@
                     "lineno": frame.lineno,
                     "name": frame.name,
                 }
                 for frame in current_stack_frame
             ]
 
             elapsed = time.time() - request.started
+            if "anthropic" in request.url.host:
+                from anthropic.types.beta.tools import (
+                    ToolsBetaMessage,
+                )
+
+                from log10.anthropic import Anthropic
+
+                llm_response = Anthropic.prepare_response(ToolsBetaMessage(**llm_response))
+
             log_row = {
                 "response": json.dumps(llm_response),
                 "status": "finished",
                 "duration": int(elapsed * 1000),
                 "stacktrace": json.dumps(stacktrace),
                 "kind": "chat",
                 "request": request.content.decode("utf-8"),
-                "session_id": sessionID,
+                "session_id": session_id_var.get(),
             }
             if get_log10_session_tags():
                 log_row["tags"] = get_log10_session_tags()
             await _try_post_request_async(url=f"{base_url}/api/completions/{completion_id}", payload=log_row)
             return response
         elif response.headers.get("content-type").startswith("text/event-stream"):
             return _LogResponse(
```

### Comparing `log10_io-0.8.4/log10/agents/camel.py` & `log10_io-0.8.5/log10/agents/camel.py`

 * *Files identical despite different names*

### Comparing `log10_io-0.8.4/log10/agents/scrape_summarizer.py` & `log10_io-0.8.5/log10/agents/scrape_summarizer.py`

 * *Files identical despite different names*

### Comparing `log10_io-0.8.4/log10/anthropic.py` & `log10_io-0.8.5/log10/anthropic.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,13 +1,16 @@
 import logging
 import time
 from typing import List
 
 import anthropic
 from anthropic import AI_PROMPT, HUMAN_PROMPT
+from anthropic.types.beta.tools import (
+    ToolsBetaMessage,
+)
 
 from log10.llm import LLM, ChatCompletion, Kind, Message, TextCompletion
 from log10.utils import merge_hparams
 
 
 class Anthropic(LLM):
     def __init__(self, hparams: dict = None, skip_initialization: bool = False, log10_config=None):
@@ -129,17 +132,20 @@
             "prompt_tokens": prompt_tokens,
             "completion_tokens": completion_tokens,
             "total_tokens": total_tokens,
         }
 
     @staticmethod
     def prepare_response(
-        response: anthropic.types.Completion | anthropic.types.Message, input_prompt: str = ""
+        response: anthropic.types.Completion | anthropic.types.Message | ToolsBetaMessage, input_prompt: str = ""
     ) -> dict:
-        if response.stop_reason in ["stop_sequence", "end_turn"]:
+        if not hasattr(response, "stop_reason"):
+            return None
+
+        if response.stop_reason in ["stop_sequence", "end_turn", "tool_use"]:
             reason = "stop"
         elif response.stop_reason == "max_tokens":
             reason = "length"
 
         ret_response = {
             "id": response.id,
             "object": "completion",
@@ -147,20 +153,28 @@
             "choices": [
                 {
                     "index": 0,
                     "finish_reason": reason,
                 }
             ],
         }
+
         if isinstance(response, anthropic.types.Message):
             tokens_usage = {
                 "prompt_tokens": response.usage.input_tokens,
                 "completion_tokens": response.usage.output_tokens,
                 "total_tokens": response.usage.input_tokens + response.usage.output_tokens,
             }
             ret_response["choices"][0]["message"] = {"role": response.role, "content": response.content[0].text}
         elif isinstance(response, anthropic.types.Completion):
             tokens_usage = Anthropic.create_tokens_usage(input_prompt, response.completion)
             ret_response["choices"][0]["text"] = response.completion
+        elif isinstance(response, ToolsBetaMessage):
+            tokens_usage = {
+                "prompt_tokens": response.usage.input_tokens,
+                "completion_tokens": response.usage.output_tokens,
+                "total_tokens": response.usage.input_tokens + response.usage.output_tokens,
+            }
+            ret_response["choices"][0]["message"] = {"role": response.role, "content": response.content[0].text}
         ret_response["usage"] = tokens_usage
 
         return ret_response
```

### Comparing `log10_io-0.8.4/log10/bigquery.py` & `log10_io-0.8.5/log10/bigquery.py`

 * *Files identical despite different names*

### Comparing `log10_io-0.8.4/log10/cli_utils.py` & `log10_io-0.8.5/log10/cli_utils.py`

 * *Files identical despite different names*

### Comparing `log10_io-0.8.4/log10/completions/completions.py` & `log10_io-0.8.5/log10/completions/completions.py`

 * *Files 0% similar despite different names*

```diff
@@ -396,14 +396,16 @@
 
             ret[model] = response
     return ret
 
 
 _SUPPORTED_MODELS = [
     # openai chat models
+    "gpt-4o",
+    "gpt-4o-2024-05-13",
     "gpt-4-turbo",
     "gpt-4-turbo-2024-04-09",
     "gpt-4-0125-preview",
     "gpt-4-turbo-preview",
     "gpt-4-1106-preview",
     "gpt-4-vision-preview",
     "gpt-4",
```

### Comparing `log10_io-0.8.4/log10/evals.py` & `log10_io-0.8.5/log10/evals.py`

 * *Files identical despite different names*

### Comparing `log10_io-0.8.4/log10/feedback/_summary_feedback_utils.py` & `log10_io-0.8.5/log10/feedback/_summary_feedback_utils.py`

 * *Files identical despite different names*

### Comparing `log10_io-0.8.4/log10/feedback/autofeedback.py` & `log10_io-0.8.5/log10/feedback/autofeedback.py`

 * *Files identical despite different names*

### Comparing `log10_io-0.8.4/log10/feedback/feedback.py` & `log10_io-0.8.5/log10/feedback/feedback.py`

 * *Files identical despite different names*

### Comparing `log10_io-0.8.4/log10/feedback/feedback_task.py` & `log10_io-0.8.5/log10/feedback/feedback_task.py`

 * *Files identical despite different names*

### Comparing `log10_io-0.8.4/log10/langchain.py` & `log10_io-0.8.5/log10/langchain.py`

 * *Files identical despite different names*

### Comparing `log10_io-0.8.4/log10/litellm.py` & `log10_io-0.8.5/log10/litellm.py`

 * *Files identical despite different names*

### Comparing `log10_io-0.8.4/log10/llm.py` & `log10_io-0.8.5/log10/llm.py`

 * *Files identical despite different names*

### Comparing `log10_io-0.8.4/log10/load.py` & `log10_io-0.8.5/log10/load.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,8 +1,9 @@
 import asyncio
+import contextvars
 import functools
 import inspect
 import json
 import logging
 import os
 import queue
 import threading
@@ -103,57 +104,67 @@
 
 def get_session_id():
     id = str(uuid.uuid4())
     logger.debug(f"Session ID: {id}")
     return id
 
 
-# Global variable to store the current sessionID.
-sessionID = get_session_id()
-last_completion_response = None
-global_tags = []
+#
+# Context variables
+#
+session_id_var = contextvars.ContextVar("session_id", default=get_session_id())
+last_completion_response_var = contextvars.ContextVar("last_completion_response", default=None)
+tags_var = contextvars.ContextVar("tags", default=[])
 
 
 def get_log10_session_tags():
-    return global_tags
+    return tags_var.get()
 
 
 class log10_session:
     def __init__(self, tags=None):
         self.tags = tags
 
-        if tags is not None:
-            global global_tags
-            global_tags = tags
-
     def __enter__(self):
-        global sessionID
-        global last_completion_response
-        sessionID = get_session_id()
-        last_completion_response = None
+        self.session_id_token = session_id_var.set(get_session_id())
+        self.last_completion_response_token = last_completion_response_var.set(None)
+        self.tags_token = tags_var.set(self.tags)
+
         return self
 
-    def last_completion_url(self):
-        if last_completion_response is None:
-            return None
+    def __exit__(self, exc_type, exc_value, traceback):
+        session_id_var.reset(self.session_id_token)
+        last_completion_response_var.reset(self.last_completion_response_token)
+        tags_var.reset(self.tags_token)
+        return
 
-        return (
-            url
-            + "/app/"
-            + last_completion_response["organizationSlug"]
-            + "/completions/"
-            + last_completion_response["completionID"]
-        )
+    async def __aenter__(self):
+        self.session_id_token = session_id_var.set(get_session_id())
+        self.last_completion_response_token = last_completion_response_var.set(None)
+        self.tags_token = tags_var.set(self.tags)
+        return self
 
-    def __exit__(self, exc_type, exc_value, traceback):
-        if self.tags is not None:
-            global global_tags
-            global_tags = None
+    async def __aexit__(self, exc_type, exc_value, traceback):
+        session_id_var.reset(self.session_id_token)
+        last_completion_response_var.reset(self.last_completion_response_token)
+        tags_var.reset(self.tags_token)
         return
 
+    def last_completion_url(self):
+        if last_completion_response_var.get() is None:
+            return None
+        response = last_completion_response_var.get()
+        return f'{url}/app/{response["organizationSlug"]}/completions/{response["completionID"]}'
+
+    def last_completion_id(self):
+        if last_completion_response_var.get() is None:
+            return None
+        response = last_completion_response_var.get()
+        return response["completionID"]
+
 
 @contextmanager
 def timed_block(block_name):
     if DEBUG:
         start_time = time.perf_counter()
         try:
             yield
@@ -168,28 +179,31 @@
     output = res.json()
     organizationSlug = output["organizationSlug"]
     full_url = url + "/app/" + organizationSlug + "/completions/" + completionID
     logger.debug(f"Completion URL: {full_url}")
 
 
 async def log_async(completion_url, log_row):
-    global last_completion_response
-
     res = None
     try:
         res = post_request(completion_url)
-        last_completion_response = res.json()
-        completionID = res.json()["completionID"]
+        last_completion_response_var.set(res.json())
+        completionID = res.json().get("completionID", None)
+
+        if completionID is None:
+            logging.warn("LOG10: failed to get completionID from log10. Skipping log.")
+            return None
 
         if DEBUG:
             log_url(res, completionID)
 
         if target_service == "log10":
             try:
-                res = post_request(completion_url + "/" + completionID, log_row)
+                _url = f"{completion_url}/{completionID}"
+                res = post_request(_url, log_row)
             except Exception as e:
                 logging.warn(f"LOG10: failed to log: {e}. Skipping")
                 return None
 
         elif target_service == "bigquery":
             pass
             # NOTE: We only save on request finalization.
@@ -203,24 +217,29 @@
 
 def run_async_in_thread(completion_url, log_row, result_queue):
     result = asyncio.run(log_async(completion_url=completion_url, log_row=log_row))
     result_queue.put(result)
 
 
 def log_sync(completion_url, log_row):
-    global last_completion_response
     completionID = None
 
     try:
         res = post_request(completion_url)
-        last_completion_response = res.json()
-        completionID = res.json()["completionID"]
+        last_completion_response_var.set(res.json())
+        completionID = res.json().get("completionID", None)
+
+        if completionID is None:
+            logging.warn("LOG10: failed to get completionID from log10. Skipping log.")
+            return None
+
         if DEBUG:
             log_url(res, completionID)
-        res = post_request(completion_url + "/" + completionID, log_row)
+        _url = f"{completion_url}/{completionID}"
+        res = post_request(_url, log_row)
     except Exception as e:
         logging.warn(f"LOG10: failed to get completionID from log10: {e}")
         return None
 
     return completionID
 
 
@@ -355,29 +374,38 @@
                 }
             if self.usage:
                 response["usage"] = self.usage.dict()
             self.partial_log_row["response"] = json.dumps(response)
             self.partial_log_row["duration"] = int((time.perf_counter() - self.start_time) * 1000)
 
             try:
-                res = post_request(self.completion_url + "/" + self.completionID, self.partial_log_row)
+                _url = f"{self.completion_url}/{self.completionID}"
+                res = post_request(_url, self.partial_log_row)
                 if res.status_code != 200:
                     logger.error(f"LOG10: failed to insert in log10: {self.partial_log_row} with error {res.text}")
             except Exception as e:
                 traceback.print_tb(e.__traceback__)
                 logging.warn(f"LOG10: failed to log: {e}. Skipping")
 
             raise se
 
 
 class AnthropicStreamingResponseWrapper:
     """
     Wraps a streaming response object to log the final result and duration to log10.
     """
 
+    def __enter__(self):
+        self.response = self.response.__enter__()
+        return self
+
+    def __exit__(self, exc_type, exc_value, traceback):
+        self.response.__exit__(exc_type, exc_value, traceback)
+        return
+
     def __init__(self, completion_url, completionID, response, partial_log_row):
         self.completionID = completionID
         self.completion_url = completion_url
         self.partial_log_row = partial_log_row
         self.response = response
         self.final_result = ""
         self.start_time = time.perf_counter()
@@ -388,24 +416,34 @@
         self.output_tokens = 0
 
     def __iter__(self):
         return self
 
     def __next__(self):
         chunk = next(self.response)
+        self._process_chunk(chunk)
+        return chunk
+
+    def _process_chunk(self, chunk):
         if chunk.type == "message_start":
             self.model = chunk.message.model
             self.message_id = chunk.message.id
             self.input_tokens = chunk.message.usage.input_tokens
+        if chunk.type == "content_block_start":
+            if hasattr(chunk.content_block, "text"):
+                self.final_result += chunk.content_block.text
         elif chunk.type == "message_delta":
             self.finish_reason = chunk.delta.stop_reason
             self.output_tokens = chunk.usage.output_tokens
         elif chunk.type == "content_block_delta":
-            self.final_result += chunk.delta.text
-        elif chunk.type == "message_stop":
+            if hasattr(chunk.delta, "text"):
+                self.final_result += chunk.delta.text
+            if hasattr(chunk.delta, "partial_json"):
+                self.final_result += chunk.delta.partial_json
+        elif chunk.type == "message_stop" or chunk.type == "content_block_stop":
             response = {
                 "id": self.message_id,
                 "object": "chat",
                 "model": self.model,
                 "choices": [
                     {
                         "index": 0,
@@ -421,20 +459,19 @@
                     "completion_tokens": self.output_tokens,
                     "total_tokens": self.input_tokens + self.output_tokens,
                 },
             }
             self.partial_log_row["response"] = json.dumps(response)
             self.partial_log_row["duration"] = int((time.perf_counter() - self.start_time) * 1000)
 
-            res = post_request(self.completion_url + "/" + self.completionID, self.partial_log_row)
+            _url = f"{self.completion_url}/{self.completionID}"
+            res = post_request(_url, self.partial_log_row)
             if res.status_code != 200:
                 logger.error(f"Failed to insert in log10: {self.partial_log_row} with error {res.text}. Skipping")
 
-        return chunk
-
 
 def flatten_messages(messages):
     flat_messages = []
     for message in messages:
         if isinstance(message, dict):
             flat_messages.append(message)
         else:
@@ -468,71 +505,94 @@
     kwargs_copy = deepcopy(kwargs)
 
     log_row = {
         "status": "started",
         "orig_module": func.__module__,
         "orig_qualname": func.__qualname__,
         "stacktrace": json.dumps(_get_stack_trace()),
-        "session_id": sessionID,
-        "tags": global_tags,
+        "session_id": session_id_var.get(),
+        "tags": tags_var.get(),
     }
 
     # in case the usage of load(openai) and langchain.ChatOpenAI
     if "api_key" in kwargs_copy:
         kwargs_copy.pop("api_key")
 
     # We may have to flatten messages from their ChatCompletionMessage with nested ChatCompletionMessageToolCall to json serializable format
     # Rewrite in-place
     if "messages" in kwargs_copy:
         kwargs_copy["messages"] = flatten_messages(kwargs_copy["messages"])
 
     # kind and request are set based on the module and qualname
     # request is based on openai schema
     if "anthropic" in func.__module__:
+        from anthropic._utils._utils import strip_not_given
+
+        kwargs_copy = strip_not_given(kwargs_copy)
         log_row["kind"] = "chat" if "message" in func.__module__ else "completion"
         # set system message
         if "system" in kwargs_copy:
             kwargs_copy["messages"].insert(0, {"role": "system", "content": kwargs_copy["system"]})
         if "messages" in kwargs_copy:
             for m in kwargs_copy["messages"]:
                 if isinstance(m.get("content"), list):
                     new_content = []
                     for c in m.get("content", ""):
                         if c.get("type") == "image":
                             image_type = c.get("source", {}).get("media_type", "")
                             image_data = c.get("source", {}).get("data", "")
                             new_content.append(
-                                {"type": "image_url", "image_url": {"url": f"data:{image_type};base64,{image_data}"}}
+                                {
+                                    "type": "image_url",
+                                    "image_url": {"url": f"data:{image_type};base64,{image_data}"},
+                                }
                             )
                         else:
                             new_content.append(c)
                     m["content"] = new_content
+        if "tools" in kwargs_copy:
+            for t in kwargs_copy["tools"]:
+                new_function = {
+                    "name": t.get("name", None),
+                    "description": t.get("description", None),
+                    "parameters": {
+                        "properties": t.get("input_schema", {}).get("properties", None),
+                    },
+                }
+                t["function"] = new_function
+                t.pop("input_schema", None)
     elif "vertexai" in func.__module__:
         if func.__name__ == "_send_message":
             # get model name save in ChatSession instance
             log_row["kind"] = "chat"
             chat_session_instance = inspect.currentframe().f_back.f_back.f_locals["self"]
             model_name = chat_session_instance._model._model_name.split("/")[-1]
 
             # TODO how to handle chat history
             # chat_history = chat_session_instance.history
             kwargs_copy.update(
-                {"model": model_name, "messages": [{"role": "user", "content": kwargs_copy["content"]}]}
+                {
+                    "model": model_name,
+                    "messages": [{"role": "user", "content": kwargs_copy["content"]}],
+                }
             )
             if kwargs_copy.get("generation_config"):
                 for key, value in kwargs_copy["generation_config"].to_dict().items():
                     if key == "max_output_tokens":
                         kwargs_copy["max_tokens"] = value
                     else:
                         kwargs_copy[key] = value
                 kwargs_copy.pop("generation_config")
     elif "lamini" in func.__module__:
         log_row["kind"] = "chat"
         kwargs_copy.update(
-            {"model": args[1]["model_name"], "messages": [{"role": "user", "content": args[1]["prompt"]}]}
+            {
+                "model": args[1]["model_name"],
+                "messages": [{"role": "user", "content": args[1]["prompt"]}],
+            }
         )
     elif "mistralai" in func.__module__:
         log_row["kind"] = "chat"
     elif "openai" in func.__module__:
         from openai._utils._utils import strip_not_given
 
         kwargs_copy = strip_not_given(kwargs_copy)
@@ -547,15 +607,20 @@
             if history := args[0].history:
                 for m in history:
                     role = "assistant" if m.role == "model" else "user"
                     content = m.parts[0].text
                     history_messages.append({"role": role, "content": content})
 
             history_messages.append({"role": "user", "content": args[1]})
-            kwargs_copy.update({"model": args[0].model.model_name.split("/")[-1], "messages": history_messages})
+            kwargs_copy.update(
+                {
+                    "model": args[0].model.model_name.split("/")[-1],
+                    "messages": history_messages,
+                }
+            )
             if kwargs_copy.get("generation_config") and hasattr(kwargs_copy["generation_config"], "__dict__"):
                 for key, value in kwargs_copy["generation_config"].__dict__.items():
                     if not value:
                         continue
                     if key == "max_output_tokens":
                         kwargs_copy["max_tokens"] = value
                     elif key == "stop_sequences":
@@ -605,15 +670,15 @@
             if USE_ASYNC:
                 with timed_block("extra time spent waiting for log10 call"):
                     while result_queue.empty():
                         pass
                     completionID = result_queue.get()
 
             if completionID is None:
-                logging.warn(f"LOG10: failed to get completionID from log10: {e}. Skipping log.")
+                logger.warning(f"LOG10: failed to get completionID from log10: {e}. Skipping log.")
                 return
 
             logger.debug(f"LOG10: failed - {e}")
             # todo: change with openai v1 update
             if type(e).__name__ == "InvalidRequestError" and "This model's maximum context length" in str(e):
                 failure_kind = "ContextWindowExceedError"
             else:
@@ -621,51 +686,55 @@
             failure_reason = str(e)
             log_row["status"] = "failed"
             log_row["failure_kind"] = failure_kind
             log_row["failure_reason"] = failure_reason
             try:
                 res = post_request(completion_url + "/" + completionID, log_row)
             except Exception as le:
-                logging.warn(f"LOG10: failed to log: {le}. Skipping, but raising LLM error.")
+                logger.warning(f"LOG10: failed to log: {le}. Skipping, but raising LLM error.")
             raise e
         else:
             # finished with no exceptions
             if USE_ASYNC:
                 with timed_block("extra time spent waiting for log10 call"):
                     while result_queue.empty():
                         pass
                     completionID = result_queue.get()
 
             with timed_block("result call duration (sync)"):
                 response = output
                 # Adjust the Anthropic output to match OAI completion output
                 if "anthropic" in func.__module__:
-                    if type(output).__name__ == "Stream":
+                    if type(output).__name__ == "Stream" or "MessageStreamManager" in type(output).__name__:
                         log_row["response"] = response
                         log_row["status"] = "finished"
                         return AnthropicStreamingResponseWrapper(
                             completion_url=completion_url,
                             completionID=completionID,
                             response=response,
                             partial_log_row=log_row,
                         )
+
                     from log10.anthropic import Anthropic
 
                     response = Anthropic.prepare_response(output, input_prompt=kwargs.get("prompt", ""))
                 elif "vertexai" in func.__module__:
                     response = output
                     reason = response.candidates[0].finish_reason.name
                     ret_response = {
                         "id": str(uuid.uuid4()),
                         "object": "chat.completion",
                         "choices": [
                             {
                                 "index": 0,
                                 "finish_reason": str(reason).lower(),
-                                "message": {"role": "assistant", "content": response.text},
+                                "message": {
+                                    "role": "assistant",
+                                    "content": response.text,
+                                },
                             }
                         ],
                     }
                     response_dict = response.to_dict()
                     tokens_usage = {
                         "prompt_tokens": response_dict["usage_metadata"]["prompt_token_count"],
                         "completion_tokens": response_dict["usage_metadata"]["candidates_token_count"],
@@ -677,15 +746,18 @@
                     ret_response = {
                         "id": str(uuid.uuid4()),
                         "object": "chat.completion",
                         "choices": [
                             {
                                 "index": 0,
                                 "finish_reason": str(output.candidates[0].finish_reason.name).lower(),
-                                "message": {"role": "assistant", "content": output.text},
+                                "message": {
+                                    "role": "assistant",
+                                    "content": output.text,
+                                },
                             }
                         ],
                         "usage": {
                             "prompt_tokens": 0,
                             "completion_tokens": 0,
                             "total_tokens": 0,
                         },
@@ -709,18 +781,25 @@
                     response = {
                         "id": str(uuid.uuid4()),
                         "object": "chat.completion",
                         "choices": [
                             {
                                 "index": 0,
                                 "finish_reason": "stop",
-                                "message": {"role": "assistant", "content": output["output"]},
+                                "message": {
+                                    "role": "assistant",
+                                    "content": output["output"],
+                                },
                             }
                         ],
-                        "usage": {"prompt_tokens": 0, "completion_tokens": 0, "total_tokens": 0},
+                        "usage": {
+                            "prompt_tokens": 0,
+                            "completion_tokens": 0,
+                            "total_tokens": 0,
+                        },
                     }
                 elif "mistralai" in func.__module__:
                     if "stream" in func.__qualname__:
                         log_row["response"] = response
                         log_row["status"] = "finished"
                         return StreamingResponseWrapper(
                             completion_url=completion_url,
@@ -737,15 +816,16 @@
 
                 log_row["status"] = "finished"
                 log_row["duration"] = int(duration * 1000)
                 log_row["response"] = response
 
                 if target_service == "log10":
                     try:
-                        res = post_request(completion_url + "/" + completionID, log_row)
+                        _url = f"{completion_url}/{completionID}"
+                        res = post_request(_url, log_row)
                         if res.status_code != 200:
                             logger.error(f"LOG10: failed to insert in log10: {log_row} with error {res.text}")
                     except Exception as e:
                         logging.warn(f"LOG10: failed to log: {e}. Skipping")
 
                 elif target_service == "bigquery":
                     try:
@@ -756,15 +836,15 @@
                         if func.__qualname__ == "Completion.create":
                             log_row["kind"] = "completion"
                         elif func.__qualname__ == "ChatCompletion.create":
                             log_row["kind"] = "chat"
 
                         log_row["orig_module"] = func.__module__
                         log_row["orig_qualname"] = func.__qualname__
-                        log_row["session_id"] = sessionID
+                        log_row["session_id"] = session_id_var.get()
 
                         bigquery_client.insert_rows_json(bigquery_table, [log_row])
 
                     except Exception as e:
                         logging.error(f"LOG10: failed to insert in Bigquery: {log_row} with error {e}")
 
         return output
@@ -888,14 +968,50 @@
         method = getattr(attr, "create")
         setattr(attr, "create", intercepting_decorator(method))
 
         # anthropic Messages completion
         attr = module.resources.messages.Messages
         method = getattr(attr, "create")
         setattr(attr, "create", intercepting_decorator(method))
+
+        attr = module.resources.messages.Messages
+        method = getattr(attr, "stream")
+        setattr(attr, "stream", intercepting_decorator(method))
+
+        attr = module.resources.beta.tools.Messages
+        method = getattr(attr, "create")
+        setattr(attr, "create", intercepting_decorator(method))
+
+        attr = module.resources.beta.tools.Messages
+        method = getattr(attr, "stream")
+        setattr(attr, "stream", intercepting_decorator(method))
+
+        origin_init = module.AsyncAnthropic.__init__
+
+        def new_init(self, *args, **kwargs):
+            logger.debug("LOG10: patching AsyncAnthropic.__init__")
+            import httpx
+
+            from log10._httpx_utils import (
+                _LogTransport,
+                get_completion_id,
+                log_request,
+            )
+
+            event_hooks = {
+                "request": [get_completion_id, log_request],
+            }
+            async_httpx_client = httpx.AsyncClient(
+                event_hooks=event_hooks,
+                transport=_LogTransport(httpx.AsyncHTTPTransport()),
+            )
+            kwargs["http_client"] = async_httpx_client
+            origin_init(self, *args, **kwargs)
+
+        module.AsyncAnthropic.__init__ = new_init
     elif module.__name__ == "lamini":
         attr = module.api.utils.completion.Completion
         method = getattr(attr, "generate")
         setattr(attr, "generate", intercepting_decorator(method))
     elif module.__name__ == "mistralai" and getattr(module, "_log10_patched", False) is False:
         attr = module.client.MistralClient
         method = getattr(attr, "chat")
@@ -998,16 +1114,15 @@
             >>> )
             >>> print(completion)
         """
 
         def __init__(self, *args, **kwargs):
             # check if tags is passed in
             if "tags" in kwargs:
-                global global_tags
-                global_tags = kwargs.pop("tags")
+                tags_var.set(kwargs.pop("tags"))
             super().__init__(*args, **kwargs)
 
             if not getattr(openai, "_log10_patched", False):
                 log10(openai)
                 openai._log10_patched = True
 
 
@@ -1031,14 +1146,13 @@
             ...     messages=[{"role": "user", "content": "How are you today?"}],
             ... )
             >>> print(message.content[0].text)
         """
 
         def __init__(self, *args, **kwargs):
             if "tags" in kwargs:
-                global global_tags
-                global_tags = kwargs.pop("tags")
+                tags_var.set(kwargs.pop("tags"))
             super().__init__(*args, **kwargs)
 
             if not getattr(anthropic, "_log10_patched", False):
                 log10(anthropic)
                 anthropic._log10_patched = True
```

### Comparing `log10_io-0.8.4/log10/mosaicml.py` & `log10_io-0.8.5/log10/mosaicml.py`

 * *Files identical despite different names*

### Comparing `log10_io-0.8.4/log10/openai.py` & `log10_io-0.8.5/log10/openai.py`

 * *Files identical despite different names*

### Comparing `log10_io-0.8.4/log10/prompt_analyzer.py` & `log10_io-0.8.5/log10/prompt_analyzer.py`

 * *Files identical despite different names*

### Comparing `log10_io-0.8.4/log10/schemas/bigquery.json` & `log10_io-0.8.5/log10/schemas/bigquery.json`

 * *Files identical despite different names*

### Comparing `log10_io-0.8.4/log10/together.py` & `log10_io-0.8.5/log10/together.py`

 * *Files identical despite different names*

### Comparing `log10_io-0.8.4/log10/tools.py` & `log10_io-0.8.5/log10/tools.py`

 * *Files identical despite different names*

### Comparing `log10_io-0.8.4/log10/utils.py` & `log10_io-0.8.5/log10/utils.py`

 * *Files identical despite different names*

### Comparing `log10_io-0.8.4/pyproject.toml` & `log10_io-0.8.5/pyproject.toml`

 * *Files 17% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 [build-system]
 requires = ["poetry-core>=1.0.0"]
 build-backend = "poetry.core.masonry.api"
 
 [tool.poetry]
 name = "log10-io"
 
-version = "0.8.4"
+version = "0.8.5"
 authors = ["log10 team"]
 license = "MIT"
 description = "Unified LLM data management"
 readme = "README.md"
 classifiers = [
     "Programming Language :: Python :: 3",
     "License :: OSI Approved :: MIT License",
@@ -24,46 +24,49 @@
 
 [tool.poetry.group.dev.dependencies]
 build = "^0.10.0"
 pytest = "^8.0.0"
 requests-mock = "^1.11.0"
 respx = "^0.20.2"
 ruff = "^0.3.2"
+pytest-asyncio = "^0.23.6"
 
 [project.urls]
 "Homepage" = "https://github.com/log10-io/log10"
 "Bug Tracker" = "https://github.com/log10-io/log10/issues"
 
 [tool.poetry.dependencies]
 python = ">=3.9,<4.0"
-langchain = "<0.2.0"
 openai = "<2"
+anthropic = "<1"
 requests = "^2.31.0"
 python-dotenv = "^1.0.0"
-google-cloud-bigquery = "^3.11.4"
-pexpect = "^4.8.0"
-faiss-cpu = "^1.7.4"
-google-search-results = "^2.4.2"
-wikipedia = "^1.4.0"
-faker = "^19.2.0"
 backoff = "^2.2.1"
-anthropic = "<1"
-mosaicml-cli = "^0.5.30"
-together = "^0.2.7"
-google-cloud-aiplatform = ">=1.44.0"
-mistralai = "^0.1.5"
 pandas = ">=2"
-
+langchain = {version = "<0.2.0", optional = true}
 magentic = {version = ">=0.17.0", optional = true, markers = "python_version >= '3.10'"}
 litellm = {version = "^1.34.18", optional = true}
 lamini = {version = "^2.1.8", optional = true}
+google-cloud-aiplatform = {version = ">=1.44.0", optional = true}
+mistralai = {version = "^0.1.5", optional = true}
+together = {version = "^0.2.7", optional = true}
+mosaicml-cli = {version = "^0.5.30", optional = true}
+google-cloud-bigquery = {version = "^3.11.4", optional = true}
+google-generativeai = {version = "^0.5.2", optional = true}
 
 [tool.poetry.extras]
 autofeedback_icl = ["magentic"]
 litellm = ["litellm"]
+langchain = ["langchain"]
+gemini = ["google-cloud-aiplatform"]
+mistralai = ["mistralai"]
+together = ["together"]
+mosaicml = ["mosaicml-cli"]
+google-generativeai = ["google-generativeai"]
+lamini = ["lamini"]
 
 [tool.ruff]
 # Never enforce `E501` (line length violations).
 lint.ignore = ["C901", "E501", "E741", "F402", "F823" ]
 lint.select = ["C", "E", "F", "I", "W"]
 line-length = 119
```

### Comparing `log10_io-0.8.4/PKG-INFO` & `log10_io-0.8.5/PKG-INFO`

 * *Files 10% similar despite different names*

```diff
@@ -1,43 +1,46 @@
 Metadata-Version: 2.1
 Name: log10-io
-Version: 0.8.4
+Version: 0.8.5
 Summary: Unified LLM data management
 License: MIT
 Author: log10 team
 Requires-Python: >=3.9,<4.0
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: Python :: 3.12
 Provides-Extra: autofeedback-icl
+Provides-Extra: gemini
+Provides-Extra: google-generativeai
+Provides-Extra: lamini
+Provides-Extra: langchain
 Provides-Extra: litellm
+Provides-Extra: mistralai
+Provides-Extra: mosaicml
+Provides-Extra: together
 Requires-Dist: anthropic (<1)
 Requires-Dist: backoff (>=2.2.1,<3.0.0)
-Requires-Dist: faiss-cpu (>=1.7.4,<2.0.0)
-Requires-Dist: faker (>=19.2.0,<20.0.0)
-Requires-Dist: google-cloud-aiplatform (>=1.44.0)
+Requires-Dist: google-cloud-aiplatform (>=1.44.0) ; extra == "gemini"
 Requires-Dist: google-cloud-bigquery (>=3.11.4,<4.0.0)
-Requires-Dist: google-search-results (>=2.4.2,<3.0.0)
-Requires-Dist: lamini (>=2.1.8,<3.0.0)
-Requires-Dist: langchain (<0.2.0)
+Requires-Dist: google-generativeai (>=0.5.2,<0.6.0) ; extra == "google-generativeai"
+Requires-Dist: lamini (>=2.1.8,<3.0.0) ; extra == "lamini"
+Requires-Dist: langchain (<0.2.0) ; extra == "langchain"
 Requires-Dist: litellm (>=1.34.18,<2.0.0) ; extra == "litellm"
 Requires-Dist: magentic (>=0.17.0) ; (python_version >= "3.10") and (extra == "autofeedback-icl")
-Requires-Dist: mistralai (>=0.1.5,<0.2.0)
-Requires-Dist: mosaicml-cli (>=0.5.30,<0.6.0)
+Requires-Dist: mistralai (>=0.1.5,<0.2.0) ; extra == "mistralai"
+Requires-Dist: mosaicml-cli (>=0.5.30,<0.6.0) ; extra == "mosaicml"
 Requires-Dist: openai (<2)
 Requires-Dist: pandas (>=2)
-Requires-Dist: pexpect (>=4.8.0,<5.0.0)
 Requires-Dist: python-dotenv (>=1.0.0,<2.0.0)
 Requires-Dist: requests (>=2.31.0,<3.0.0)
-Requires-Dist: together (>=0.2.7,<0.3.0)
-Requires-Dist: wikipedia (>=1.4.0,<2.0.0)
+Requires-Dist: together (>=0.2.7,<0.3.0) ; extra == "together"
 Description-Content-Type: text/markdown
 
 # log10
 
 ⚡ Unified LLM data management to drive accuracy at scale ⚡
 
 [![pypi](https://github.com/log10-io/log10/actions/workflows/release.yml/badge.svg)](https://github.com/log10-io/log10/actions/workflows/release.yml)
```

