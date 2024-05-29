# Comparing `tmp/openllmtelemetry-0.0.1b6.tar.gz` & `tmp/openllmtelemetry-0.0.1b7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "openllmtelemetry-0.0.1b6.tar", max compression
+gzip compressed data, was "openllmtelemetry-0.0.1b7.tar", max compression
```

## Comparing `openllmtelemetry-0.0.1b6.tar` & `openllmtelemetry-0.0.1b7.tar`

### file list

```diff
@@ -1,27 +1,27 @@
--rw-r--r--   0        0        0    11357 2023-11-22 23:27:14.459880 openllmtelemetry-0.0.1b6/LICENSE
--rw-r--r--   0        0        0     4317 2024-04-24 17:37:18.405975 openllmtelemetry-0.0.1b6/README.md
--rw-r--r--   0        0        0       75 2024-05-21 15:45:54.138472 openllmtelemetry-0.0.1b6/openllmtelemetry/__init__.py
--rw-r--r--   0        0        0     8435 2024-05-21 15:52:52.542394 openllmtelemetry-0.0.1b6/openllmtelemetry/config.py
--rw-r--r--   0        0        0       61 2024-05-21 15:52:52.019303 openllmtelemetry-0.0.1b6/openllmtelemetry/guardrails/__init__.py
--rw-r--r--   0        0        0     4054 2024-05-21 15:52:52.674562 openllmtelemetry-0.0.1b6/openllmtelemetry/guardrails/client.py
--rw-r--r--   0        0        0     7180 2024-05-21 15:52:52.674867 openllmtelemetry-0.0.1b6/openllmtelemetry/guardrails/handlers.py
--rw-r--r--   0        0        0     1971 2024-05-21 15:52:52.675317 openllmtelemetry-0.0.1b6/openllmtelemetry/instrument.py
--rw-r--r--   0        0        0    11339 2024-04-24 17:37:18.407381 openllmtelemetry-0.0.1b6/openllmtelemetry/instrumentation/LICENSE
--rw-r--r--   0        0        0        0 2024-04-24 17:37:18.407435 openllmtelemetry-0.0.1b6/openllmtelemetry/instrumentation/__init__.py
--rw-r--r--   0        0        0    14053 2024-05-21 15:52:52.543647 openllmtelemetry-0.0.1b6/openllmtelemetry/instrumentation/bedrock/__init__.py
--rw-r--r--   0        0        0     2344 2024-04-30 16:55:16.794654 openllmtelemetry-0.0.1b6/openllmtelemetry/instrumentation/bedrock/reusable_streaming_body.py
--rw-r--r--   0        0        0     1719 2024-05-21 15:52:52.019985 openllmtelemetry-0.0.1b6/openllmtelemetry/instrumentation/openai/__init__.py
--rw-r--r--   0        0        0     4769 2024-05-21 15:52:52.675543 openllmtelemetry-0.0.1b6/openllmtelemetry/instrumentation/openai/shared/__init__.py
--rw-r--r--   0        0        0     9995 2024-05-21 15:52:52.675741 openllmtelemetry-0.0.1b6/openllmtelemetry/instrumentation/openai/shared/chat_wrappers.py
--rw-r--r--   0        0        0     6306 2024-05-21 15:52:52.675965 openllmtelemetry-0.0.1b6/openllmtelemetry/instrumentation/openai/shared/completion_wrappers.py
--rw-r--r--   0        0        0     3509 2024-05-21 15:52:52.020983 openllmtelemetry-0.0.1b6/openllmtelemetry/instrumentation/openai/shared/embeddings_wrappers.py
--rw-r--r--   0        0        0     1231 2024-04-30 16:55:16.796566 openllmtelemetry-0.0.1b6/openllmtelemetry/instrumentation/openai/utils.py
--rw-r--r--   0        0        0     2401 2024-05-21 15:52:52.021214 openllmtelemetry-0.0.1b6/openllmtelemetry/instrumentation/openai/v0/__init__.py
--rw-r--r--   0        0        0     2908 2024-05-21 15:52:52.021419 openllmtelemetry-0.0.1b6/openllmtelemetry/instrumentation/openai/v1/__init__.py
--rw-r--r--   0        0        0       28 2024-04-24 17:37:18.409700 openllmtelemetry-0.0.1b6/openllmtelemetry/instrumentation/openai/version.py
--rw-r--r--   0        0        0     1407 2024-05-21 15:52:52.021650 openllmtelemetry-0.0.1b6/openllmtelemetry/intrument_openai.py
--rw-r--r--   0        0        0     2493 2024-05-21 15:52:52.676238 openllmtelemetry-0.0.1b6/openllmtelemetry/semantic_conventions/gen_ai/__init__.py
--rw-r--r--   0        0        0      809 2024-05-20 22:42:13.975873 openllmtelemetry-0.0.1b6/openllmtelemetry/span_exporter.py
--rw-r--r--   0        0        0      477 2024-04-24 17:37:18.410285 openllmtelemetry-0.0.1b6/openllmtelemetry/version.py
--rw-r--r--   0        0        0     1653 2024-05-21 16:19:11.435989 openllmtelemetry-0.0.1b6/pyproject.toml
--rw-r--r--   0        0        0     5320 1970-01-01 00:00:00.000000 openllmtelemetry-0.0.1b6/PKG-INFO
+-rw-r--r--   0        0        0    11357 2024-04-24 19:03:26.905847 openllmtelemetry-0.0.1b7/LICENSE
+-rw-r--r--   0        0        0     4317 2024-04-24 19:03:26.905847 openllmtelemetry-0.0.1b7/README.md
+-rw-r--r--   0        0        0       99 2024-05-23 21:28:06.887620 openllmtelemetry-0.0.1b7/openllmtelemetry/__init__.py
+-rw-r--r--   0        0        0     8650 2024-05-24 16:00:12.713852 openllmtelemetry-0.0.1b7/openllmtelemetry/config.py
+-rw-r--r--   0        0        0       61 2024-05-24 16:00:12.713852 openllmtelemetry-0.0.1b7/openllmtelemetry/guardrails/__init__.py
+-rw-r--r--   0        0        0     4541 2024-05-24 16:00:12.713852 openllmtelemetry-0.0.1b7/openllmtelemetry/guardrails/client.py
+-rw-r--r--   0        0        0     7180 2024-05-24 16:00:12.713852 openllmtelemetry-0.0.1b7/openllmtelemetry/guardrails/handlers.py
+-rw-r--r--   0        0        0     2667 2024-05-24 16:00:12.713852 openllmtelemetry-0.0.1b7/openllmtelemetry/instrument.py
+-rw-r--r--   0        0        0    11339 2024-04-24 19:03:26.905847 openllmtelemetry-0.0.1b7/openllmtelemetry/instrumentation/LICENSE
+-rw-r--r--   0        0        0        0 2024-04-24 19:03:26.905847 openllmtelemetry-0.0.1b7/openllmtelemetry/instrumentation/__init__.py
+-rw-r--r--   0        0        0    14054 2024-05-28 16:10:07.443574 openllmtelemetry-0.0.1b7/openllmtelemetry/instrumentation/bedrock/__init__.py
+-rw-r--r--   0        0        0     2344 2024-05-14 21:55:10.222851 openllmtelemetry-0.0.1b7/openllmtelemetry/instrumentation/bedrock/reusable_streaming_body.py
+-rw-r--r--   0        0        0     1719 2024-05-24 16:00:12.713852 openllmtelemetry-0.0.1b7/openllmtelemetry/instrumentation/openai/__init__.py
+-rw-r--r--   0        0        0     4769 2024-05-24 16:00:12.713852 openllmtelemetry-0.0.1b7/openllmtelemetry/instrumentation/openai/shared/__init__.py
+-rw-r--r--   0        0        0     9995 2024-05-24 16:00:12.713852 openllmtelemetry-0.0.1b7/openllmtelemetry/instrumentation/openai/shared/chat_wrappers.py
+-rw-r--r--   0        0        0     6306 2024-05-24 16:00:12.713852 openllmtelemetry-0.0.1b7/openllmtelemetry/instrumentation/openai/shared/completion_wrappers.py
+-rw-r--r--   0        0        0     3509 2024-05-24 16:00:12.713852 openllmtelemetry-0.0.1b7/openllmtelemetry/instrumentation/openai/shared/embeddings_wrappers.py
+-rw-r--r--   0        0        0     1231 2024-05-14 21:55:10.222851 openllmtelemetry-0.0.1b7/openllmtelemetry/instrumentation/openai/utils.py
+-rw-r--r--   0        0        0     2401 2024-05-24 16:00:12.713852 openllmtelemetry-0.0.1b7/openllmtelemetry/instrumentation/openai/v0/__init__.py
+-rw-r--r--   0        0        0     2908 2024-05-24 16:00:12.713852 openllmtelemetry-0.0.1b7/openllmtelemetry/instrumentation/openai/v1/__init__.py
+-rw-r--r--   0        0        0       28 2024-04-24 19:03:26.905847 openllmtelemetry-0.0.1b7/openllmtelemetry/instrumentation/openai/version.py
+-rw-r--r--   0        0        0     1407 2024-05-24 16:00:12.713852 openllmtelemetry-0.0.1b7/openllmtelemetry/intrument_openai.py
+-rw-r--r--   0        0        0     2493 2024-05-24 16:00:12.713852 openllmtelemetry-0.0.1b7/openllmtelemetry/semantic_conventions/gen_ai/__init__.py
+-rw-r--r--   0        0        0      809 2024-04-25 18:42:42.775178 openllmtelemetry-0.0.1b7/openllmtelemetry/span_exporter.py
+-rw-r--r--   0        0        0      477 2024-04-24 19:03:26.905847 openllmtelemetry-0.0.1b7/openllmtelemetry/version.py
+-rw-r--r--   0        0        0     1653 2024-05-24 16:00:12.713852 openllmtelemetry-0.0.1b7/pyproject.toml
+-rw-r--r--   0        0        0     5320 1970-01-01 00:00:00.000000 openllmtelemetry-0.0.1b7/PKG-INFO
```

### Comparing `openllmtelemetry-0.0.1b6/LICENSE` & `openllmtelemetry-0.0.1b7/LICENSE`

 * *Files identical despite different names*

### Comparing `openllmtelemetry-0.0.1b6/README.md` & `openllmtelemetry-0.0.1b7/README.md`

 * *Files identical despite different names*

### Comparing `openllmtelemetry-0.0.1b6/openllmtelemetry/config.py` & `openllmtelemetry-0.0.1b7/openllmtelemetry/config.py`

 * *Files 5% similar despite different names*

```diff
@@ -25,26 +25,26 @@
 _DEFAULT_ENDPOINT = "https://api.whylabsapp.com"
 _CONFIG_DIR = os.path.join(Path.home(), ".whylabs")
 _DEFAULT_CONFIG_FILE = os.path.join(_CONFIG_DIR, "guardrails-config.ini")
 
 _in_ipython_session = False
 try:
     # noinspection PyStatementEffect
-    __IPYTHON__
+    __IPYTHON__  # pyright: ignore[reportUndefinedVariable,reportUnusedExpression]
     _in_ipython_session = True
 except NameError:
     pass
 
 
 @dataclass
 class GuardrailConfig(object):
-    whylabs_endpoint: Optional[str]
-    whylabs_api_key: Optional[str]
-    guardrails_endpoint: Optional[str]
-    guardrails_api_key: Optional[str]
+    whylabs_endpoint: Optional[str] = None
+    whylabs_api_key: Optional[str] = None
+    guardrails_endpoint: Optional[str] = None
+    guardrails_api_key: Optional[str] = None
 
     @property
     def is_partial(self):
         return (
             self.whylabs_endpoint is None
             or self.whylabs_api_key is None
             or self.guardrails_endpoint is None
@@ -52,15 +52,15 @@
         )
 
     @property
     def whylabs_traces_endpoint(self) -> str:
         assert self.whylabs_endpoint is not None, "WhyLabs endpoint is not set."
         return f"{self.whylabs_endpoint.rstrip('/')}/v1/traces"
 
-    def guardrail_client(self, default_dataset_id: str) -> Optional[GuardrailsApi]:
+    def guardrail_client(self, default_dataset_id: Optional[str]) -> Optional[GuardrailsApi]:
         if self.guardrails_endpoint and self.guardrails_api_key:
             return GuardrailsApi(
                 guardrails_endpoint=self.guardrails_endpoint,
                 guardrails_api_key=self.guardrails_api_key,
                 dataset_id=default_dataset_id,
             )
         LOGGER.warning("GuardRails endpoint is not set.")
@@ -93,22 +93,23 @@
                 span_processor = BatchSpanProcessor(otlp_exporter)
             tracer_provider.add_span_processor(span_processor)
 
         pass
 
     def write(self, config_path: str):
         config = configparser.ConfigParser()
-        config[CFG_WHYLABS_SECTION] = {
-            CFG_ENDPOINT_KEY: self.whylabs_endpoint,
-            CFG_API_KEY: self.whylabs_api_key,
-        }
+        if self.whylabs_endpoint is not None and self.whylabs_api_key is not None:
+            config[CFG_WHYLABS_SECTION] = {
+                CFG_ENDPOINT_KEY: self.whylabs_endpoint,
+                CFG_API_KEY: self.whylabs_api_key,
+            }
         if self.guardrails_endpoint:
             config[CFG_GUARDRAILS_SECTION] = {
                 CFG_ENDPOINT_KEY: self.guardrails_endpoint,
-                CFG_API_KEY: self.guardrails_api_key,
+                CFG_API_KEY: self.guardrails_api_key or "",
             }
         with open(config_path, "w") as configfile:
             config.write(configfile)
 
     def __repr__(self):
         # hide the api_key from output
         field_strs = [
@@ -127,15 +128,15 @@
         whylabs_api_key = config.get(CFG_WHYLABS_SECTION, CFG_API_KEY)
         guardrails_endpoint = config.get(CFG_GUARDRAILS_SECTION, CFG_ENDPOINT_KEY, fallback=None)
         guardrails_api_key = config.get(CFG_GUARDRAILS_SECTION, CFG_API_KEY, fallback=None)
 
         return GuardrailConfig(whylabs_endpoint, whylabs_api_key, guardrails_endpoint, guardrails_api_key)
 
 
-def load_config() -> Optional[GuardrailConfig]:
+def load_config() -> GuardrailConfig:
     config_path = os.environ.get("WHYLABS_GUARDRAILS_CONFIG")
     if config_path is None:
         config_path = _DEFAULT_CONFIG_FILE
     config = GuardrailConfig(None, None, None, None)
     try:
         config = GuardrailConfig.read(config_path)
     except:  # noqa
@@ -144,15 +145,15 @@
         config = _load_config_from_env(config)
     if config.is_partial and _in_ipython_session:
         config = _interactive_config(config)
 
     return config
 
 
-def load_dataset_id(dataset_id: str) -> Optional[str]:
+def load_dataset_id(dataset_id: Optional[str]) -> Optional[str]:
     effective_dataset_id = os.environ.get("WHYLABS_DEFAULT_DATASET_ID", dataset_id)
     if effective_dataset_id is None:
         if _in_ipython_session:
             effective_dataset_id = input("Set the default dataset ID: ").strip()
             if len(effective_dataset_id) > 0:
                 print("Using dataset ID: ", effective_dataset_id)
             else:
@@ -200,13 +201,13 @@
 
     save_config = input("Do you want to save these settings to a configuration file? [y/n]: ").strip().lower()
     if save_config == "y" or save_config == "yes":
         try:
             os.makedirs(_CONFIG_DIR, exist_ok=True)
             guardrail_config.write(_DEFAULT_CONFIG_FILE)
         except Exception as e:  # noqa
-            LOGGER.exception("Failed to write the configuration file.")
+            LOGGER.exception(f"Failed to write the configuration file: {e}")
 
             print("Failed to write the configuration file.")
 
     print(f"Set config: {guardrail_config}")
     return guardrail_config
```

### Comparing `openllmtelemetry-0.0.1b6/openllmtelemetry/guardrails/client.py` & `openllmtelemetry-0.0.1b7/openllmtelemetry/guardrails/client.py`

 * *Files 12% similar despite different names*

```diff
@@ -13,15 +13,15 @@
 
 
 class GuardrailsApi(object):
     def __init__(
         self,
         guardrails_endpoint: str,
         guardrails_api_key: str,
-        dataset_id: str,
+        dataset_id: Optional[str] = None,
         timeout: Optional[float] = 1.0,
         auth_header_name: str = "X-API-Key",
     ):
         """
         Construct a new WhyLabs Guard client
 
         :param guardrails_endpoint: the endpoint for the guard client
@@ -37,16 +37,19 @@
             token=guardrails_api_key,  #
             prefix="",  #
             auth_header_name=auth_header_name,  # type: ignore
             timeout=Timeout(timeout, read=timeout),  # type: ignore
         )  # type: ignore
 
     def eval_prompt(self, prompt: str) -> Optional[EvaluationResult]:
-        dataset_id = os.environ["CURRENT_DATASET_ID"] or self._dataset_id
-        LOGGER.info("Evaluate prompt for dataset_id: %s", dataset_id)
+        dataset_id = os.environ.get("CURRENT_DATASET_ID") or self._dataset_id
+        LOGGER.info(f"Evaluate prompt for dataset_id: {dataset_id}")
+        if dataset_id is None:
+            LOGGER.warning("GuardRail eval_prompt requires a dataset_id but dataset_id is None.")
+            return None
         profiling_request = LLMValidateRequest(prompt=prompt, dataset_id=dataset_id)
         res = Evaluate.sync(client=self._client, body=profiling_request, log=False)
 
         if isinstance(res, HTTPValidationError):
             # TODO: log out the client version and the API endpoint version
             LOGGER.warning(f"GuardRail request validation failure detected. result was: {res} Possible version mismatched.")
             return None
@@ -55,31 +58,36 @@
 
     def eval_response(self, prompt: str, response: str) -> Optional[EvaluationResult]:
         # nested array so you can model a metric requiring multiple inputs. That line says "only run the metrics
         # that require response OR (prompt and response)", which would cover the input similarity metric
         metric_filter_option = MetricFilterOptions(
             by_required_inputs=[["response"], ["prompt", "response"]],
         )
-        dataset_id = os.environ["CURRENT_DATASET_ID"] or self._dataset_id
-
+        dataset_id = os.environ.get("CURRENT_DATASET_ID") or self._dataset_id
+        if dataset_id is None:
+            LOGGER.warning("GuardRail eval_response requires a dataset_id but dataset_id is None.")
+            return None
         profiling_request = LLMValidateRequest(
             prompt=prompt,
             response=response,
             dataset_id=dataset_id,
             options=RunOptions(metric_filter=metric_filter_option),
         )
         res = Evaluate.sync(client=self._client, body=profiling_request, log=False, perf_info=True)
         if isinstance(res, HTTPValidationError):
             LOGGER.warning(f"GuardRail request validation failure detected. Possible version mismatched: {res}")
             return None
         LOGGER.debug(f"Done calling eval_response on [prompt: {prompt}, response: {response}] -> res: {res}")
         return res
 
     def eval_chunk(self, chunk: str) -> Optional[EvaluationResult]:
-        dataset_id = os.environ["CURRENT_DATASET_ID"] or self._dataset_id
+        dataset_id = os.environ.get("CURRENT_DATASET_ID") or self._dataset_id
+        if dataset_id is None:
+            LOGGER.warning("GuardRail eval_chunk requires a dataset_id but dataset_id is None.")
+            return None
         profiling_request = LLMValidateRequest(response=chunk, dataset_id=dataset_id)
         res = Evaluate.sync(client=self._client, body=profiling_request, log=False)
 
         if isinstance(res, HTTPValidationError):
             LOGGER.warning(f"GuardRail request validation failure detected. Possible version mismatched: {res}")
             return None
         LOGGER.debug(f"Done calling eval_chunk on prompt: {chunk} -> res: {res}")
```

### Comparing `openllmtelemetry-0.0.1b6/openllmtelemetry/guardrails/handlers.py` & `openllmtelemetry-0.0.1b7/openllmtelemetry/guardrails/handlers.py`

 * *Files identical despite different names*

### Comparing `openllmtelemetry-0.0.1b6/openllmtelemetry/instrument.py` & `openllmtelemetry-0.0.1b7/openllmtelemetry/instrument.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,33 +1,43 @@
 import os
 from logging import getLogger
-from typing import Optional
+from typing import Dict, Optional, Tuple
 
 from opentelemetry import trace
 from opentelemetry.sdk.resources import Resource
 from opentelemetry.sdk.trace import TracerProvider
 from opentelemetry.trace import Tracer
 
 from openllmtelemetry.config import load_config, load_dataset_id
 from openllmtelemetry.intrument_openai import init_instrumentors
 from openllmtelemetry.version import __version__
 
 LOGGER = getLogger(__name__)
 
+_tracer_cache: Dict[str, trace.Tracer] = {}
+_last_added_tracer: Optional[Tuple[str, trace.Tracer]] = None
+
 
 def instrument(
     application_name: Optional[str] = None,
     dataset_id: Optional[str] = None,
     tracer_name: Optional[str] = None,
     service_name: Optional[str] = None,
     disable_batching: bool = False,
     debug: bool = False,
 ) -> Tracer:
+    global _tracer_cache, _last_added_tracer
+
     config = load_config()
     dataset_id = load_dataset_id(dataset_id)
+    if dataset_id is None:
+        raise ValueError(
+            "dataset_id must be specified in a parameter or in env var: e.g. "
+            "os.environ[\"WHYLABS_DEFAULT_DATASET_ID\"] = \"model-1\""
+        )
     guardrails_api = config.guardrail_client(default_dataset_id=dataset_id)
 
     if application_name is None:
         otel_service_name = os.environ.get("OTEL_SERVICE_NAME")
         if otel_service_name:
             application_name = otel_service_name
         else:
@@ -46,10 +56,21 @@
     )
 
     tracer_provider = TracerProvider(resource=resource)
     config.config_tracer_provider(tracer_provider, dataset_id=dataset_id, disable_batching=disable_batching, debug=debug)
 
     tracer = trace.get_tracer(tracer_name)
     trace.set_tracer_provider(tracer_provider)
+    _tracer_cache[tracer_name] = tracer
+    _last_added_tracer = (tracer_name, tracer)
 
     init_instrumentors(tracer, guardrails_api)
     return tracer
+
+
+def get_tracer(name: Optional[str] = None) -> Optional[Tracer]:
+    if _last_added_tracer is None:
+        return None
+    elif name is None:
+        return _last_added_tracer[1]
+    else:
+        return _tracer_cache.get(name)
```

### Comparing `openllmtelemetry-0.0.1b6/openllmtelemetry/instrumentation/LICENSE` & `openllmtelemetry-0.0.1b7/openllmtelemetry/instrumentation/LICENSE`

 * *Files identical despite different names*

### Comparing `openllmtelemetry-0.0.1b6/openllmtelemetry/instrumentation/bedrock/__init__.py` & `openllmtelemetry-0.0.1b7/openllmtelemetry/instrumentation/bedrock/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -41,15 +41,15 @@
 
 _instruments = ("boto3 >= 1.28.57",)
 
 WRAPPED_METHODS = [{"package": "botocore.client", "object": "ClientCreator", "method": "create_client"}]
 
 
 def should_send_prompts():
-    return (os.getenv("TRACE_PROMPT_AND_RESPONSE") or "true").lower() == "true" or context_api.get_value("override_enable_content_tracing")
+    return (os.getenv("TRACE_PROMPT_AND_RESPONSE") or "false").lower() == "true" or context_api.get_value("override_enable_content_tracing")
 
 
 def _set_span_attribute(span, name, value):
     if value is not None:
         if value != "":
             span.set_attribute(name, value)
     return
```

### Comparing `openllmtelemetry-0.0.1b6/openllmtelemetry/instrumentation/bedrock/reusable_streaming_body.py` & `openllmtelemetry-0.0.1b7/openllmtelemetry/instrumentation/bedrock/reusable_streaming_body.py`

 * *Files identical despite different names*

### Comparing `openllmtelemetry-0.0.1b6/openllmtelemetry/instrumentation/openai/__init__.py` & `openllmtelemetry-0.0.1b7/openllmtelemetry/instrumentation/openai/__init__.py`

 * *Files identical despite different names*

### Comparing `openllmtelemetry-0.0.1b6/openllmtelemetry/instrumentation/openai/shared/__init__.py` & `openllmtelemetry-0.0.1b7/openllmtelemetry/instrumentation/openai/shared/__init__.py`

 * *Files identical despite different names*

### Comparing `openllmtelemetry-0.0.1b6/openllmtelemetry/instrumentation/openai/shared/chat_wrappers.py` & `openllmtelemetry-0.0.1b7/openllmtelemetry/instrumentation/openai/shared/chat_wrappers.py`

 * *Files identical despite different names*

### Comparing `openllmtelemetry-0.0.1b6/openllmtelemetry/instrumentation/openai/shared/completion_wrappers.py` & `openllmtelemetry-0.0.1b7/openllmtelemetry/instrumentation/openai/shared/completion_wrappers.py`

 * *Files identical despite different names*

### Comparing `openllmtelemetry-0.0.1b6/openllmtelemetry/instrumentation/openai/shared/embeddings_wrappers.py` & `openllmtelemetry-0.0.1b7/openllmtelemetry/instrumentation/openai/shared/embeddings_wrappers.py`

 * *Files identical despite different names*

### Comparing `openllmtelemetry-0.0.1b6/openllmtelemetry/instrumentation/openai/utils.py` & `openllmtelemetry-0.0.1b7/openllmtelemetry/instrumentation/openai/utils.py`

 * *Files identical despite different names*

### Comparing `openllmtelemetry-0.0.1b6/openllmtelemetry/instrumentation/openai/v0/__init__.py` & `openllmtelemetry-0.0.1b7/openllmtelemetry/instrumentation/openai/v0/__init__.py`

 * *Files identical despite different names*

### Comparing `openllmtelemetry-0.0.1b6/openllmtelemetry/instrumentation/openai/v1/__init__.py` & `openllmtelemetry-0.0.1b7/openllmtelemetry/instrumentation/openai/v1/__init__.py`

 * *Files identical despite different names*

### Comparing `openllmtelemetry-0.0.1b6/openllmtelemetry/intrument_openai.py` & `openllmtelemetry-0.0.1b7/openllmtelemetry/intrument_openai.py`

 * *Files identical despite different names*

### Comparing `openllmtelemetry-0.0.1b6/openllmtelemetry/semantic_conventions/gen_ai/__init__.py` & `openllmtelemetry-0.0.1b7/openllmtelemetry/semantic_conventions/gen_ai/__init__.py`

 * *Files identical despite different names*

### Comparing `openllmtelemetry-0.0.1b6/openllmtelemetry/span_exporter.py` & `openllmtelemetry-0.0.1b7/openllmtelemetry/span_exporter.py`

 * *Files identical despite different names*

### Comparing `openllmtelemetry-0.0.1b6/pyproject.toml` & `openllmtelemetry-0.0.1b7/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "OpenLLMTelemetry"
-version = "0.0.1.b6"
+version = "0.0.1.b7"
 description = "End-to-end observability with built-in security guardrails."
 authors = ["WhyLabs.ai <support@whylabs.ai>"]
 license = "Apache-2.0"
 readme = "README.md"
 
 [tool.poetry.dependencies]
 python = ">=3.8.1,<4.0"
```

### Comparing `openllmtelemetry-0.0.1b6/PKG-INFO` & `openllmtelemetry-0.0.1b7/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
-Name: openllmtelemetry
-Version: 0.0.1b6
+Name: OpenLLMTelemetry
+Version: 0.0.1b7
 Summary: End-to-end observability with built-in security guardrails.
 License: Apache-2.0
 Author: WhyLabs.ai
 Author-email: support@whylabs.ai
 Requires-Python: >=3.8.1,<4.0
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Programming Language :: Python :: 3
```

