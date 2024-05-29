# Comparing `tmp/paita-0.1.8.tar.gz` & `tmp/paita-0.1.9.tar.gz`

## Comparing `paita-0.1.8.tar` & `paita-0.1.9.tar`

### file list

```diff
@@ -1,57 +1,57 @@
--rw-r--r--   0        0        0      125 2020-02-02 00:00:00.000000 paita-0.1.8/mypy.ini
--rw-r--r--   0        0        0     1462 2020-02-02 00:00:00.000000 paita-0.1.8/.github/workflows/code_quality.yml
--rw-r--r--   0        0        0     1265 2020-02-02 00:00:00.000000 paita-0.1.8/docs/development.md
--rw-r--r--   0        0        0      520 2020-02-02 00:00:00.000000 paita-0.1.8/docs/publish.md
--rw-r--r--   0        0        0   477378 2020-02-02 00:00:00.000000 paita-0.1.8/imgs/paita.jpg
--rw-r--r--   0        0        0      144 2020-02-02 00:00:00.000000 paita-0.1.8/src/paita/__about__.py
--rw-r--r--   0        0        0      122 2020-02-02 00:00:00.000000 paita-0.1.8/src/paita/__init__.py
--rw-r--r--   0        0        0      122 2020-02-02 00:00:00.000000 paita-0.1.8/src/paita/ai/__init__.py
--rw-r--r--   0        0        0     2922 2020-02-02 00:00:00.000000 paita-0.1.8/src/paita/ai/callbacks.py
--rw-r--r--   0        0        0     4651 2020-02-02 00:00:00.000000 paita-0.1.8/src/paita/ai/chat.py
--rw-r--r--   0        0        0     1368 2020-02-02 00:00:00.000000 paita-0.1.8/src/paita/ai/chat_history.py
--rw-r--r--   0        0        0      286 2020-02-02 00:00:00.000000 paita-0.1.8/src/paita/ai/enums.py
--rw-r--r--   0        0        0      193 2020-02-02 00:00:00.000000 paita-0.1.8/src/paita/ai/message.py
--rw-r--r--   0        0        0     1277 2020-02-02 00:00:00.000000 paita-0.1.8/src/paita/ai/models.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 paita-0.1.8/src/paita/ai/services/__init__.py
--rw-r--r--   0        0        0     3319 2020-02-02 00:00:00.000000 paita-0.1.8/src/paita/ai/services/bedrock.py
--rw-r--r--   0        0        0     1233 2020-02-02 00:00:00.000000 paita-0.1.8/src/paita/ai/services/mock.py
--rw-r--r--   0        0        0     1644 2020-02-02 00:00:00.000000 paita-0.1.8/src/paita/ai/services/ollama.py
--rw-r--r--   0        0        0     1740 2020-02-02 00:00:00.000000 paita-0.1.8/src/paita/ai/services/openai.py
--rw-r--r--   0        0        0      536 2020-02-02 00:00:00.000000 paita-0.1.8/src/paita/ai/services/service.py
--rw-r--r--   0        0        0      122 2020-02-02 00:00:00.000000 paita-0.1.8/src/paita/localization/__init__.py
--rw-r--r--   0        0        0      501 2020-02-02 00:00:00.000000 paita-0.1.8/src/paita/localization/labels.py
--rw-r--r--   0        0        0      122 2020-02-02 00:00:00.000000 paita-0.1.8/src/paita/tui/__init__.py
--rw-r--r--   0        0        0     9710 2020-02-02 00:00:00.000000 paita-0.1.8/src/paita/tui/app.py
--rw-r--r--   0        0        0      952 2020-02-02 00:00:00.000000 paita-0.1.8/src/paita/tui/error_screen.py
--rw-r--r--   0        0        0     5451 2020-02-02 00:00:00.000000 paita-0.1.8/src/paita/tui/message_box.py
--rw-r--r--   0        0        0      454 2020-02-02 00:00:00.000000 paita-0.1.8/src/paita/tui/multi_line_input.py
--rw-r--r--   0        0        0     6869 2020-02-02 00:00:00.000000 paita-0.1.8/src/paita/tui/settings_screen.py
--rw-r--r--   0        0        0      583 2020-02-02 00:00:00.000000 paita-0.1.8/src/paita/tui/wait_screen.py
--rw-r--r--   0        0        0     1555 2020-02-02 00:00:00.000000 paita-0.1.8/src/paita/tui/styles/app.tcss
--rw-r--r--   0        0        0      521 2020-02-02 00:00:00.000000 paita-0.1.8/src/paita/tui/styles/error_screen.tcss
--rw-r--r--   0        0        0      686 2020-02-02 00:00:00.000000 paita-0.1.8/src/paita/tui/styles/message_box.tcss
--rw-r--r--   0        0        0      854 2020-02-02 00:00:00.000000 paita-0.1.8/src/paita/tui/styles/settings_screen.tcss
--rw-r--r--   0        0        0      514 2020-02-02 00:00:00.000000 paita-0.1.8/src/paita/tui/styles/wait_screen.tcss
--rw-r--r--   0        0        0      122 2020-02-02 00:00:00.000000 paita-0.1.8/src/paita/utils/__init__.py
--rw-r--r--   0        0        0      254 2020-02-02 00:00:00.000000 paita-0.1.8/src/paita/utils/config_dirs.py
--rw-r--r--   0        0        0      180 2020-02-02 00:00:00.000000 paita-0.1.8/src/paita/utils/logger.py
--rw-r--r--   0        0        0     2939 2020-02-02 00:00:00.000000 paita-0.1.8/src/paita/utils/settings_manager.py
--rw-r--r--   0        0        0      545 2020-02-02 00:00:00.000000 paita-0.1.8/src/paita/utils/settings_model.py
--rw-r--r--   0        0        0     1389 2020-02-02 00:00:00.000000 paita-0.1.8/src/paita/utils/string_utils.py
--rw-r--r--   0        0        0      122 2020-02-02 00:00:00.000000 paita-0.1.8/tests/__init__.py
--rw-r--r--   0        0        0      122 2020-02-02 00:00:00.000000 paita-0.1.8/tests/integration/__init__.py
--rw-r--r--   0        0        0      122 2020-02-02 00:00:00.000000 paita-0.1.8/tests/integration/ai/__init__.py
--rw-r--r--   0        0        0     2234 2020-02-02 00:00:00.000000 paita-0.1.8/tests/integration/ai/test_chat.py
--rw-r--r--   0        0        0      173 2020-02-02 00:00:00.000000 paita-0.1.8/tests/integration/ai/test_models.py
--rw-r--r--   0        0        0      122 2020-02-02 00:00:00.000000 paita-0.1.8/tests/unit/__init__.py
--rw-r--r--   0        0        0     1383 2020-02-02 00:00:00.000000 paita-0.1.8/tests/unit/test_cache3.py
--rw-r--r--   0        0        0     1117 2020-02-02 00:00:00.000000 paita-0.1.8/tests/unit/test_settings_manager.py
--rw-r--r--   0        0        0     1607 2020-02-02 00:00:00.000000 paita-0.1.8/tests/unit/test_string_utils.py
--rw-r--r--   0        0        0      122 2020-02-02 00:00:00.000000 paita-0.1.8/tests/unit/ai/__init__.py
--rw-r--r--   0        0        0     1018 2020-02-02 00:00:00.000000 paita-0.1.8/tests/unit/ai/test_chat.py
--rw-r--r--   0        0        0      439 2020-02-02 00:00:00.000000 paita-0.1.8/tests/unit/ai/test_message.py
--rw-r--r--   0        0        0     2071 2020-02-02 00:00:00.000000 paita-0.1.8/.gitignore
--rw-r--r--   0        0        0     1075 2020-02-02 00:00:00.000000 paita-0.1.8/LICENSE
--rw-r--r--   0        0        0     2433 2020-02-02 00:00:00.000000 paita-0.1.8/README.md
--rw-r--r--   0        0        0     3080 2020-02-02 00:00:00.000000 paita-0.1.8/pyproject.toml
--rw-r--r--   0        0        0     3787 2020-02-02 00:00:00.000000 paita-0.1.8/PKG-INFO
+-rw-r--r--   0        0        0      125 2020-02-02 00:00:00.000000 paita-0.1.9/mypy.ini
+-rw-r--r--   0        0        0     1462 2020-02-02 00:00:00.000000 paita-0.1.9/.github/workflows/code_quality.yml
+-rw-r--r--   0        0        0     1265 2020-02-02 00:00:00.000000 paita-0.1.9/docs/development.md
+-rw-r--r--   0        0        0      520 2020-02-02 00:00:00.000000 paita-0.1.9/docs/publish.md
+-rw-r--r--   0        0        0   477378 2020-02-02 00:00:00.000000 paita-0.1.9/imgs/paita.jpg
+-rw-r--r--   0        0        0      144 2020-02-02 00:00:00.000000 paita-0.1.9/src/paita/__about__.py
+-rw-r--r--   0        0        0      122 2020-02-02 00:00:00.000000 paita-0.1.9/src/paita/__init__.py
+-rw-r--r--   0        0        0      122 2020-02-02 00:00:00.000000 paita-0.1.9/src/paita/ai/__init__.py
+-rw-r--r--   0        0        0     2922 2020-02-02 00:00:00.000000 paita-0.1.9/src/paita/ai/callbacks.py
+-rw-r--r--   0        0        0     4651 2020-02-02 00:00:00.000000 paita-0.1.9/src/paita/ai/chat.py
+-rw-r--r--   0        0        0     1368 2020-02-02 00:00:00.000000 paita-0.1.9/src/paita/ai/chat_history.py
+-rw-r--r--   0        0        0      286 2020-02-02 00:00:00.000000 paita-0.1.9/src/paita/ai/enums.py
+-rw-r--r--   0        0        0      193 2020-02-02 00:00:00.000000 paita-0.1.9/src/paita/ai/message.py
+-rw-r--r--   0        0        0     1277 2020-02-02 00:00:00.000000 paita-0.1.9/src/paita/ai/models.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 paita-0.1.9/src/paita/ai/services/__init__.py
+-rw-r--r--   0        0        0     3319 2020-02-02 00:00:00.000000 paita-0.1.9/src/paita/ai/services/bedrock.py
+-rw-r--r--   0        0        0     1233 2020-02-02 00:00:00.000000 paita-0.1.9/src/paita/ai/services/mock.py
+-rw-r--r--   0        0        0     1353 2020-02-02 00:00:00.000000 paita-0.1.9/src/paita/ai/services/ollama.py
+-rw-r--r--   0        0        0     1740 2020-02-02 00:00:00.000000 paita-0.1.9/src/paita/ai/services/openai.py
+-rw-r--r--   0        0        0      536 2020-02-02 00:00:00.000000 paita-0.1.9/src/paita/ai/services/service.py
+-rw-r--r--   0        0        0      122 2020-02-02 00:00:00.000000 paita-0.1.9/src/paita/localization/__init__.py
+-rw-r--r--   0        0        0      501 2020-02-02 00:00:00.000000 paita-0.1.9/src/paita/localization/labels.py
+-rw-r--r--   0        0        0      122 2020-02-02 00:00:00.000000 paita-0.1.9/src/paita/tui/__init__.py
+-rw-r--r--   0        0        0     9710 2020-02-02 00:00:00.000000 paita-0.1.9/src/paita/tui/app.py
+-rw-r--r--   0        0        0      952 2020-02-02 00:00:00.000000 paita-0.1.9/src/paita/tui/error_screen.py
+-rw-r--r--   0        0        0     5451 2020-02-02 00:00:00.000000 paita-0.1.9/src/paita/tui/message_box.py
+-rw-r--r--   0        0        0      454 2020-02-02 00:00:00.000000 paita-0.1.9/src/paita/tui/multi_line_input.py
+-rw-r--r--   0        0        0     6869 2020-02-02 00:00:00.000000 paita-0.1.9/src/paita/tui/settings_screen.py
+-rw-r--r--   0        0        0      583 2020-02-02 00:00:00.000000 paita-0.1.9/src/paita/tui/wait_screen.py
+-rw-r--r--   0        0        0     1555 2020-02-02 00:00:00.000000 paita-0.1.9/src/paita/tui/styles/app.tcss
+-rw-r--r--   0        0        0      521 2020-02-02 00:00:00.000000 paita-0.1.9/src/paita/tui/styles/error_screen.tcss
+-rw-r--r--   0        0        0      686 2020-02-02 00:00:00.000000 paita-0.1.9/src/paita/tui/styles/message_box.tcss
+-rw-r--r--   0        0        0      854 2020-02-02 00:00:00.000000 paita-0.1.9/src/paita/tui/styles/settings_screen.tcss
+-rw-r--r--   0        0        0      514 2020-02-02 00:00:00.000000 paita-0.1.9/src/paita/tui/styles/wait_screen.tcss
+-rw-r--r--   0        0        0      122 2020-02-02 00:00:00.000000 paita-0.1.9/src/paita/utils/__init__.py
+-rw-r--r--   0        0        0      254 2020-02-02 00:00:00.000000 paita-0.1.9/src/paita/utils/config_dirs.py
+-rw-r--r--   0        0        0      180 2020-02-02 00:00:00.000000 paita-0.1.9/src/paita/utils/logger.py
+-rw-r--r--   0        0        0     2939 2020-02-02 00:00:00.000000 paita-0.1.9/src/paita/utils/settings_manager.py
+-rw-r--r--   0        0        0      545 2020-02-02 00:00:00.000000 paita-0.1.9/src/paita/utils/settings_model.py
+-rw-r--r--   0        0        0     1389 2020-02-02 00:00:00.000000 paita-0.1.9/src/paita/utils/string_utils.py
+-rw-r--r--   0        0        0      122 2020-02-02 00:00:00.000000 paita-0.1.9/tests/__init__.py
+-rw-r--r--   0        0        0      122 2020-02-02 00:00:00.000000 paita-0.1.9/tests/integration/__init__.py
+-rw-r--r--   0        0        0      122 2020-02-02 00:00:00.000000 paita-0.1.9/tests/integration/ai/__init__.py
+-rw-r--r--   0        0        0     2234 2020-02-02 00:00:00.000000 paita-0.1.9/tests/integration/ai/test_chat.py
+-rw-r--r--   0        0        0      173 2020-02-02 00:00:00.000000 paita-0.1.9/tests/integration/ai/test_models.py
+-rw-r--r--   0        0        0      122 2020-02-02 00:00:00.000000 paita-0.1.9/tests/unit/__init__.py
+-rw-r--r--   0        0        0     1383 2020-02-02 00:00:00.000000 paita-0.1.9/tests/unit/test_cache3.py
+-rw-r--r--   0        0        0     1117 2020-02-02 00:00:00.000000 paita-0.1.9/tests/unit/test_settings_manager.py
+-rw-r--r--   0        0        0     1607 2020-02-02 00:00:00.000000 paita-0.1.9/tests/unit/test_string_utils.py
+-rw-r--r--   0        0        0      122 2020-02-02 00:00:00.000000 paita-0.1.9/tests/unit/ai/__init__.py
+-rw-r--r--   0        0        0     1018 2020-02-02 00:00:00.000000 paita-0.1.9/tests/unit/ai/test_chat.py
+-rw-r--r--   0        0        0      439 2020-02-02 00:00:00.000000 paita-0.1.9/tests/unit/ai/test_message.py
+-rw-r--r--   0        0        0     2071 2020-02-02 00:00:00.000000 paita-0.1.9/.gitignore
+-rw-r--r--   0        0        0     1075 2020-02-02 00:00:00.000000 paita-0.1.9/LICENSE
+-rw-r--r--   0        0        0     2487 2020-02-02 00:00:00.000000 paita-0.1.9/README.md
+-rw-r--r--   0        0        0     3059 2020-02-02 00:00:00.000000 paita-0.1.9/pyproject.toml
+-rw-r--r--   0        0        0     3870 2020-02-02 00:00:00.000000 paita-0.1.9/PKG-INFO
```

### Comparing `paita-0.1.8/.github/workflows/code_quality.yml` & `paita-0.1.9/.github/workflows/code_quality.yml`

 * *Files identical despite different names*

### Comparing `paita-0.1.8/docs/development.md` & `paita-0.1.9/docs/development.md`

 * *Files identical despite different names*

### Comparing `paita-0.1.8/docs/publish.md` & `paita-0.1.9/docs/publish.md`

 * *Files identical despite different names*

### Comparing `paita-0.1.8/imgs/paita.jpg` & `paita-0.1.9/imgs/paita.jpg`

 * *Files identical despite different names*

### Comparing `paita-0.1.8/src/paita/ai/callbacks.py` & `paita-0.1.9/src/paita/ai/callbacks.py`

 * *Files identical despite different names*

### Comparing `paita-0.1.8/src/paita/ai/chat.py` & `paita-0.1.9/src/paita/ai/chat.py`

 * *Files identical despite different names*

### Comparing `paita-0.1.8/src/paita/ai/chat_history.py` & `paita-0.1.9/src/paita/ai/chat_history.py`

 * *Files identical despite different names*

### Comparing `paita-0.1.8/src/paita/ai/models.py` & `paita-0.1.9/src/paita/ai/models.py`

 * *Files identical despite different names*

### Comparing `paita-0.1.8/src/paita/ai/services/bedrock.py` & `paita-0.1.9/src/paita/ai/services/bedrock.py`

 * *Files identical despite different names*

### Comparing `paita-0.1.8/src/paita/ai/services/mock.py` & `paita-0.1.9/src/paita/ai/services/mock.py`

 * *Files identical despite different names*

### Comparing `paita-0.1.8/src/paita/ai/services/ollama.py` & `paita-0.1.9/src/paita/ai/services/openai.py`

 * *Files 22% similar despite different names*

```diff
@@ -1,42 +1,52 @@
-import aiohttp
-from langchain_community.chat_models.ollama import ChatOllama
+import asyncio
+from typing import TYPE_CHECKING
+
+from langchain_openai import ChatOpenAI
+from openai import OpenAI as OpenAIModule
 
 from paita.ai.services.service import Service
 from paita.utils.logger import log
 
+if TYPE_CHECKING:
+    from openai.types import Model
+
 
-class Ollama(Service):
+class OpenAI(Service):
     @classmethod
-    async def models(cls) -> [str]:
+    async def models(cls):
+        loop = asyncio.get_event_loop()
         try:
-            async with aiohttp.ClientSession(timeout=aiohttp.ClientTimeout(total=2)) as session:
-                async with session.get("http://localhost:11434/api/tags") as response:
-                    if response.status == aiohttp.http.HTTPStatus.OK:
-                        body = await response.json()
-                        if "models" in body:
-                            models = [model["name"] for model in body["models"]]
-                            return sorted(models)
+            client = OpenAIModule()
+            pf = client.models.list
+            response: [Model] = await loop.run_in_executor(None, pf)
+            models = [model.id for model in response.data]
+            return sorted(models)
         except Exception as e:  # noqa: BLE001 TODO
-            log.exception(e)
+            log.info(e)
             return []
 
-    def chat_model(self) -> ChatOllama:
+    def chat_model(self) -> ChatOpenAI:
         model_kwargs = {
-            "max_tokens_to_sample": self._settings_model.ai_max_tokens,
-            "temperature": 1,
-            "top_k": 250,
+            # "top_k": 250,
             "top_p": 0.8,
+            "frequency_penalty": 0.8,
+            "presence_penalty": 0.8,
             # "stop_sequences": ["\n\nHuman"],
         }
-        if self._settings_model.ai_model_kwargs:
+        temperature = 1
+        if self._settings_model.ai_model_kwargs is not None:
             model_kwargs.update(self._settings_model.ai_model_kwargs)
+            if "temperature" in model_kwargs:
+                temperature = int(model_kwargs["temperature"])
+                del model_kwargs["temperature"]
         log.debug(f"{model_kwargs=}")
-        return ChatOllama(
-            model_id=self._settings_model.ai_model,
+        return ChatOpenAI(
+            model_name=self._settings_model.ai_model,
             streaming=self._settings_model.ai_streaming,
             model_kwargs=model_kwargs,
-            # max_tokens=settings_model.ai_max_tokens,
+            max_tokens=self._settings_model.ai_max_tokens,
+            temperature=temperature,
             # n=settings_model.ai_n,
             callbacks=[self._callback_handler],
             # callback_manager=callback_handler,
         )
```

### Comparing `paita-0.1.8/src/paita/ai/services/service.py` & `paita-0.1.9/src/paita/ai/services/service.py`

 * *Files identical despite different names*

### Comparing `paita-0.1.8/src/paita/tui/app.py` & `paita-0.1.9/src/paita/tui/app.py`

 * *Files identical despite different names*

### Comparing `paita-0.1.8/src/paita/tui/error_screen.py` & `paita-0.1.9/src/paita/tui/error_screen.py`

 * *Files identical despite different names*

### Comparing `paita-0.1.8/src/paita/tui/message_box.py` & `paita-0.1.9/src/paita/tui/message_box.py`

 * *Files identical despite different names*

### Comparing `paita-0.1.8/src/paita/tui/settings_screen.py` & `paita-0.1.9/src/paita/tui/settings_screen.py`

 * *Files identical despite different names*

### Comparing `paita-0.1.8/src/paita/tui/wait_screen.py` & `paita-0.1.9/src/paita/tui/wait_screen.py`

 * *Files identical despite different names*

### Comparing `paita-0.1.8/src/paita/tui/styles/app.tcss` & `paita-0.1.9/src/paita/tui/styles/app.tcss`

 * *Files identical despite different names*

### Comparing `paita-0.1.8/src/paita/tui/styles/error_screen.tcss` & `paita-0.1.9/src/paita/tui/styles/error_screen.tcss`

 * *Files identical despite different names*

### Comparing `paita-0.1.8/src/paita/tui/styles/message_box.tcss` & `paita-0.1.9/src/paita/tui/styles/message_box.tcss`

 * *Files identical despite different names*

### Comparing `paita-0.1.8/src/paita/tui/styles/settings_screen.tcss` & `paita-0.1.9/src/paita/tui/styles/settings_screen.tcss`

 * *Files identical despite different names*

### Comparing `paita-0.1.8/src/paita/tui/styles/wait_screen.tcss` & `paita-0.1.9/src/paita/tui/styles/wait_screen.tcss`

 * *Files identical despite different names*

### Comparing `paita-0.1.8/src/paita/utils/settings_manager.py` & `paita-0.1.9/src/paita/utils/settings_manager.py`

 * *Files identical despite different names*

### Comparing `paita-0.1.8/src/paita/utils/settings_model.py` & `paita-0.1.9/src/paita/utils/settings_model.py`

 * *Files identical despite different names*

### Comparing `paita-0.1.8/src/paita/utils/string_utils.py` & `paita-0.1.9/src/paita/utils/string_utils.py`

 * *Files identical despite different names*

### Comparing `paita-0.1.8/tests/integration/ai/test_chat.py` & `paita-0.1.9/tests/integration/ai/test_chat.py`

 * *Files identical despite different names*

### Comparing `paita-0.1.8/tests/unit/test_cache3.py` & `paita-0.1.9/tests/unit/test_cache3.py`

 * *Files identical despite different names*

### Comparing `paita-0.1.8/tests/unit/test_settings_manager.py` & `paita-0.1.9/tests/unit/test_settings_manager.py`

 * *Files identical despite different names*

### Comparing `paita-0.1.8/tests/unit/test_string_utils.py` & `paita-0.1.9/tests/unit/test_string_utils.py`

 * *Files identical despite different names*

### Comparing `paita-0.1.8/tests/unit/ai/test_chat.py` & `paita-0.1.9/tests/unit/ai/test_chat.py`

 * *Files identical despite different names*

### Comparing `paita-0.1.8/.gitignore` & `paita-0.1.9/.gitignore`

 * *Files identical despite different names*

### Comparing `paita-0.1.8/LICENSE` & `paita-0.1.9/LICENSE`

 * *Files identical despite different names*

### Comparing `paita-0.1.8/README.md` & `paita-0.1.9/README.md`

 * *Files 6% similar despite different names*

```diff
@@ -7,14 +7,15 @@
 - **Supports Multiple AI Services:** Paita integrates with a variety of AI services through the [LangChain](https://python.langchain.com) library. If AI service is compatible with LangChain then it can be used also with Paita. Currently OpenAI and AWS Bedrock models are supported.
 - **Textual User Interface on your terminal:** Paita is based on [Textual](https://textual.textualize.io/) and provides a sophisticated user interface right within your terminal, combining the complexity of a GUI with console simplicity.                                                                                       
 - **Cross-Platform Compatibility:** Paita is compatible with Windows, macOS, and Linux systems across most terminals; if Python runs in your environment and Textual supports it, then Paita will work.
 
 ### Supported AI Services
 * OpenAI
 * AWS Bedrock
+* Ollama (local models)
 * (More to come soon...)
 
 ## Getting Started
 
 ### Prerequisites
 - Python 3.8.1+
 - Access to AI Service and configured in terminal
@@ -54,15 +55,15 @@
 
 #### Ollama
 
 Ollama enables running chat models locally. 
 
 Install [ollama](https://ollama.com) for operating system or use official (docker image)[https://hub.docker.com/r/ollama/ollama] 
 
-Once ollama installed pull desired model from a registry e.g.
+Once ollama installed pull desired [model](https://ollama.com/library) from a registry e.g.
 ```
 ollama pull llama2
 ```
 
 ## Feedback
 
 * [Issues](https://github.com/villekr/paita/issues)
```

### Comparing `paita-0.1.8/pyproject.toml` & `paita-0.1.9/pyproject.toml`

 * *Files 3% similar despite different names*

```diff
@@ -17,26 +17,27 @@
   "Programming Language :: Python :: 3.10",
   "Programming Language :: Python :: 3.11",
   "Programming Language :: Python :: 3.12",
   "Programming Language :: Python :: Implementation :: CPython",
   "Programming Language :: Python :: Implementation :: PyPy",
 ]
 dependencies = [
-  "textual==0.54",  # 0.51 ok, 0.52 ok, 0.53 nok, 0.54 nok
+  "textual==0.54",
   "boto3~=1.34",
   "loguru~=0.7",
   "langchain~=0.1",
   "langchain-openai~=0.1",
   "appdirs~=1.4",
   "pydantic~=2.6",
   "cache3~=0.4",
   "aiofiles~=23.2",
   "pyperclip~=1.8",
   "eval-type-backport~=0.1",
   "aiohttp~=3.9.3",
+  "ollama~=0.1.8",
 ]
 
 [project.urls]
 Documentation = "https://github.com/villekr/paita#readme"
 Issues = "https://github.com/villekr/paita/issues"
 Source = "https://github.com/villekr/paita"
```

### Comparing `paita-0.1.8/PKG-INFO` & `paita-0.1.9/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.3
 Name: paita
-Version: 0.1.8
+Version: 0.1.9
 Summary: paita - Python AI Textual Assistant
 Project-URL: Documentation, https://github.com/villekr/paita#readme
 Project-URL: Issues, https://github.com/villekr/paita/issues
 Project-URL: Source, https://github.com/villekr/paita
 Author-email: Ville Kärkkäinen <ville.karkkainen@outlook.com>
 License-Expression: MIT
 License-File: LICENSE
@@ -24,14 +24,15 @@
 Requires-Dist: appdirs~=1.4
 Requires-Dist: boto3~=1.34
 Requires-Dist: cache3~=0.4
 Requires-Dist: eval-type-backport~=0.1
 Requires-Dist: langchain-openai~=0.1
 Requires-Dist: langchain~=0.1
 Requires-Dist: loguru~=0.7
+Requires-Dist: ollama~=0.1.8
 Requires-Dist: pydantic~=2.6
 Requires-Dist: pyperclip~=1.8
 Requires-Dist: textual==0.54
 Description-Content-Type: text/markdown
 
 # Paita - Python AI Textual Assistant
 <img src="https://github.com/villekr/paita/blob/main/imgs/paita.jpg?raw=true" width="800">
@@ -42,14 +43,15 @@
 - **Supports Multiple AI Services:** Paita integrates with a variety of AI services through the [LangChain](https://python.langchain.com) library. If AI service is compatible with LangChain then it can be used also with Paita. Currently OpenAI and AWS Bedrock models are supported.
 - **Textual User Interface on your terminal:** Paita is based on [Textual](https://textual.textualize.io/) and provides a sophisticated user interface right within your terminal, combining the complexity of a GUI with console simplicity.                                                                                       
 - **Cross-Platform Compatibility:** Paita is compatible with Windows, macOS, and Linux systems across most terminals; if Python runs in your environment and Textual supports it, then Paita will work.
 
 ### Supported AI Services
 * OpenAI
 * AWS Bedrock
+* Ollama (local models)
 * (More to come soon...)
 
 ## Getting Started
 
 ### Prerequisites
 - Python 3.8.1+
 - Access to AI Service and configured in terminal
@@ -89,15 +91,15 @@
 
 #### Ollama
 
 Ollama enables running chat models locally. 
 
 Install [ollama](https://ollama.com) for operating system or use official (docker image)[https://hub.docker.com/r/ollama/ollama] 
 
-Once ollama installed pull desired model from a registry e.g.
+Once ollama installed pull desired [model](https://ollama.com/library) from a registry e.g.
 ```
 ollama pull llama2
 ```
 
 ## Feedback
 
 * [Issues](https://github.com/villekr/paita/issues)
```

