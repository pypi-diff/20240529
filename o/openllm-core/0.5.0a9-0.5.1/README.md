# Comparing `tmp/openllm_core-0.5.0a9.tar.gz` & `tmp/openllm_core-0.5.1.tar.gz`

## Comparing `openllm_core-0.5.0a9.tar` & `openllm_core-0.5.1.tar`

### file list

```diff
@@ -1,48 +1,48 @@
--rw-r--r--   0        0        0     3618 2020-02-02 00:00:00.000000 openllm_core-0.5.0a9/README.md
--rw-r--r--   0        0        0      912 2020-02-02 00:00:00.000000 openllm_core-0.5.0a9/src/openllm_core/__init__.py
--rw-r--r--   0        0        0    30564 2020-02-02 00:00:00.000000 openllm_core-0.5.0a9/src/openllm_core/_configuration.py
--rw-r--r--   0        0        0     6995 2020-02-02 00:00:00.000000 openllm_core-0.5.0a9/src/openllm_core/_schemas.py
--rw-r--r--   0        0        0     2399 2020-02-02 00:00:00.000000 openllm_core-0.5.0a9/src/openllm_core/_typing_compat.py
--rw-r--r--   0        0        0      413 2020-02-02 00:00:00.000000 openllm_core-0.5.0a9/src/openllm_core/_version.py
--rw-r--r--   0        0        0     1276 2020-02-02 00:00:00.000000 openllm_core-0.5.0a9/src/openllm_core/exceptions.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 openllm_core-0.5.0a9/src/openllm_core/py.typed
--rw-r--r--   0        0        0     1319 2020-02-02 00:00:00.000000 openllm_core-0.5.0a9/src/openllm_core/config/__init__.py
--rw-r--r--   0        0        0     8614 2020-02-02 00:00:00.000000 openllm_core-0.5.0a9/src/openllm_core/config/configuration_auto.py
--rw-r--r--   0        0        0     1892 2020-02-02 00:00:00.000000 openllm_core-0.5.0a9/src/openllm_core/config/configuration_baichuan.py
--rw-r--r--   0        0        0     1774 2020-02-02 00:00:00.000000 openllm_core-0.5.0a9/src/openllm_core/config/configuration_chatglm.py
--rw-r--r--   0        0        0     1157 2020-02-02 00:00:00.000000 openllm_core-0.5.0a9/src/openllm_core/config/configuration_dbrx.py
--rw-r--r--   0        0        0     2453 2020-02-02 00:00:00.000000 openllm_core-0.5.0a9/src/openllm_core/config/configuration_dolly_v2.py
--rw-r--r--   0        0        0     1768 2020-02-02 00:00:00.000000 openllm_core-0.5.0a9/src/openllm_core/config/configuration_falcon.py
--rw-r--r--   0        0        0     1576 2020-02-02 00:00:00.000000 openllm_core-0.5.0a9/src/openllm_core/config/configuration_flan_t5.py
--rw-r--r--   0        0        0     1301 2020-02-02 00:00:00.000000 openllm_core-0.5.0a9/src/openllm_core/config/configuration_gemma.py
--rw-r--r--   0        0        0     1687 2020-02-02 00:00:00.000000 openllm_core-0.5.0a9/src/openllm_core/config/configuration_gpt_neox.py
--rw-r--r--   0        0        0     3283 2020-02-02 00:00:00.000000 openllm_core-0.5.0a9/src/openllm_core/config/configuration_llama.py
--rw-r--r--   0        0        0     3420 2020-02-02 00:00:00.000000 openllm_core-0.5.0a9/src/openllm_core/config/configuration_mistral.py
--rw-r--r--   0        0        0     3010 2020-02-02 00:00:00.000000 openllm_core-0.5.0a9/src/openllm_core/config/configuration_mixtral.py
--rw-r--r--   0        0        0     1495 2020-02-02 00:00:00.000000 openllm_core-0.5.0a9/src/openllm_core/config/configuration_mpt.py
--rw-r--r--   0        0        0     1930 2020-02-02 00:00:00.000000 openllm_core-0.5.0a9/src/openllm_core/config/configuration_opt.py
--rw-r--r--   0        0        0     2300 2020-02-02 00:00:00.000000 openllm_core-0.5.0a9/src/openllm_core/config/configuration_phi.py
--rw-r--r--   0        0        0     1550 2020-02-02 00:00:00.000000 openllm_core-0.5.0a9/src/openllm_core/config/configuration_qwen.py
--rw-r--r--   0        0        0     2269 2020-02-02 00:00:00.000000 openllm_core-0.5.0a9/src/openllm_core/config/configuration_stablelm.py
--rw-r--r--   0        0        0     1516 2020-02-02 00:00:00.000000 openllm_core-0.5.0a9/src/openllm_core/config/configuration_starcoder.py
--rw-r--r--   0        0        0     1446 2020-02-02 00:00:00.000000 openllm_core-0.5.0a9/src/openllm_core/config/configuration_yi.py
--rw-r--r--   0        0        0      324 2020-02-02 00:00:00.000000 openllm_core-0.5.0a9/src/openllm_core/protocol/__init__.py
--rw-r--r--   0        0        0      296 2020-02-02 00:00:00.000000 openllm_core-0.5.0a9/src/openllm_core/protocol/hf.py
--rw-r--r--   0        0        0     7231 2020-02-02 00:00:00.000000 openllm_core-0.5.0a9/src/openllm_core/protocol/openai.py
--rw-r--r--   0        0        0    13808 2020-02-02 00:00:00.000000 openllm_core-0.5.0a9/src/openllm_core/utils/__init__.py
--rw-r--r--   0        0        0     4728 2020-02-02 00:00:00.000000 openllm_core-0.5.0a9/src/openllm_core/utils/__init__.pyi
--rw-r--r--   0        0        0     1044 2020-02-02 00:00:00.000000 openllm_core-0.5.0a9/src/openllm_core/utils/_constants.py
--rw-r--r--   0        0        0     3059 2020-02-02 00:00:00.000000 openllm_core-0.5.0a9/src/openllm_core/utils/analytics.py
--rw-r--r--   0        0        0     6667 2020-02-02 00:00:00.000000 openllm_core-0.5.0a9/src/openllm_core/utils/codegen.py
--rw-r--r--   0        0        0    19677 2020-02-02 00:00:00.000000 openllm_core-0.5.0a9/src/openllm_core/utils/dantic.py
--rw-r--r--   0        0        0     2566 2020-02-02 00:00:00.000000 openllm_core-0.5.0a9/src/openllm_core/utils/import_utils.py
--rw-r--r--   0        0        0      730 2020-02-02 00:00:00.000000 openllm_core-0.5.0a9/src/openllm_core/utils/import_utils.pyi
--rw-r--r--   0        0        0     9997 2020-02-02 00:00:00.000000 openllm_core-0.5.0a9/src/openllm_core/utils/lazy.py
--rw-r--r--   0        0        0     5381 2020-02-02 00:00:00.000000 openllm_core-0.5.0a9/src/openllm_core/utils/peft.py
--rw-r--r--   0        0        0      951 2020-02-02 00:00:00.000000 openllm_core-0.5.0a9/src/openllm_core/utils/pkg.py
--rw-r--r--   0        0        0     1003 2020-02-02 00:00:00.000000 openllm_core-0.5.0a9/src/openllm_core/utils/representation.py
--rw-r--r--   0        0        0     1058 2020-02-02 00:00:00.000000 openllm_core-0.5.0a9/src/openllm_core/utils/serde.py
--rw-r--r--   0        0        0     2087 2020-02-02 00:00:00.000000 openllm_core-0.5.0a9/.gitignore
--rw-r--r--   0        0        0    10470 2020-02-02 00:00:00.000000 openllm_core-0.5.0a9/LICENSE.md
--rw-r--r--   0        0        0     5946 2020-02-02 00:00:00.000000 openllm_core-0.5.0a9/pyproject.toml
--rw-r--r--   0        0        0     6638 2020-02-02 00:00:00.000000 openllm_core-0.5.0a9/PKG-INFO
+-rw-r--r--   0        0        0     3618 2020-02-02 00:00:00.000000 openllm_core-0.5.1/README.md
+-rw-r--r--   0        0        0      912 2020-02-02 00:00:00.000000 openllm_core-0.5.1/src/openllm_core/__init__.py
+-rw-r--r--   0        0        0    29344 2020-02-02 00:00:00.000000 openllm_core-0.5.1/src/openllm_core/_configuration.py
+-rw-r--r--   0        0        0     5791 2020-02-02 00:00:00.000000 openllm_core-0.5.1/src/openllm_core/_schemas.py
+-rw-r--r--   0        0        0     2399 2020-02-02 00:00:00.000000 openllm_core-0.5.1/src/openllm_core/_typing_compat.py
+-rw-r--r--   0        0        0      411 2020-02-02 00:00:00.000000 openllm_core-0.5.1/src/openllm_core/_version.py
+-rw-r--r--   0        0        0     1276 2020-02-02 00:00:00.000000 openllm_core-0.5.1/src/openllm_core/exceptions.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 openllm_core-0.5.1/src/openllm_core/py.typed
+-rw-r--r--   0        0        0     1319 2020-02-02 00:00:00.000000 openllm_core-0.5.1/src/openllm_core/config/__init__.py
+-rw-r--r--   0        0        0     9257 2020-02-02 00:00:00.000000 openllm_core-0.5.1/src/openllm_core/config/configuration_auto.py
+-rw-r--r--   0        0        0     1892 2020-02-02 00:00:00.000000 openllm_core-0.5.1/src/openllm_core/config/configuration_baichuan.py
+-rw-r--r--   0        0        0     1774 2020-02-02 00:00:00.000000 openllm_core-0.5.1/src/openllm_core/config/configuration_chatglm.py
+-rw-r--r--   0        0        0     1157 2020-02-02 00:00:00.000000 openllm_core-0.5.1/src/openllm_core/config/configuration_dbrx.py
+-rw-r--r--   0        0        0     2453 2020-02-02 00:00:00.000000 openllm_core-0.5.1/src/openllm_core/config/configuration_dolly_v2.py
+-rw-r--r--   0        0        0     1768 2020-02-02 00:00:00.000000 openllm_core-0.5.1/src/openllm_core/config/configuration_falcon.py
+-rw-r--r--   0        0        0     1576 2020-02-02 00:00:00.000000 openllm_core-0.5.1/src/openllm_core/config/configuration_flan_t5.py
+-rw-r--r--   0        0        0     1301 2020-02-02 00:00:00.000000 openllm_core-0.5.1/src/openllm_core/config/configuration_gemma.py
+-rw-r--r--   0        0        0     1687 2020-02-02 00:00:00.000000 openllm_core-0.5.1/src/openllm_core/config/configuration_gpt_neox.py
+-rw-r--r--   0        0        0     3283 2020-02-02 00:00:00.000000 openllm_core-0.5.1/src/openllm_core/config/configuration_llama.py
+-rw-r--r--   0        0        0     3420 2020-02-02 00:00:00.000000 openllm_core-0.5.1/src/openllm_core/config/configuration_mistral.py
+-rw-r--r--   0        0        0     3010 2020-02-02 00:00:00.000000 openllm_core-0.5.1/src/openllm_core/config/configuration_mixtral.py
+-rw-r--r--   0        0        0     1495 2020-02-02 00:00:00.000000 openllm_core-0.5.1/src/openllm_core/config/configuration_mpt.py
+-rw-r--r--   0        0        0     1930 2020-02-02 00:00:00.000000 openllm_core-0.5.1/src/openllm_core/config/configuration_opt.py
+-rw-r--r--   0        0        0     2563 2020-02-02 00:00:00.000000 openllm_core-0.5.1/src/openllm_core/config/configuration_phi.py
+-rw-r--r--   0        0        0     1550 2020-02-02 00:00:00.000000 openllm_core-0.5.1/src/openllm_core/config/configuration_qwen.py
+-rw-r--r--   0        0        0     2269 2020-02-02 00:00:00.000000 openllm_core-0.5.1/src/openllm_core/config/configuration_stablelm.py
+-rw-r--r--   0        0        0     1516 2020-02-02 00:00:00.000000 openllm_core-0.5.1/src/openllm_core/config/configuration_starcoder.py
+-rw-r--r--   0        0        0     1446 2020-02-02 00:00:00.000000 openllm_core-0.5.1/src/openllm_core/config/configuration_yi.py
+-rw-r--r--   0        0        0      324 2020-02-02 00:00:00.000000 openllm_core-0.5.1/src/openllm_core/protocol/__init__.py
+-rw-r--r--   0        0        0      296 2020-02-02 00:00:00.000000 openllm_core-0.5.1/src/openllm_core/protocol/hf.py
+-rw-r--r--   0        0        0     7231 2020-02-02 00:00:00.000000 openllm_core-0.5.1/src/openllm_core/protocol/openai.py
+-rw-r--r--   0        0        0    13850 2020-02-02 00:00:00.000000 openllm_core-0.5.1/src/openllm_core/utils/__init__.py
+-rw-r--r--   0        0        0     4757 2020-02-02 00:00:00.000000 openllm_core-0.5.1/src/openllm_core/utils/__init__.pyi
+-rw-r--r--   0        0        0     1084 2020-02-02 00:00:00.000000 openllm_core-0.5.1/src/openllm_core/utils/_constants.py
+-rw-r--r--   0        0        0     3059 2020-02-02 00:00:00.000000 openllm_core-0.5.1/src/openllm_core/utils/analytics.py
+-rw-r--r--   0        0        0     6667 2020-02-02 00:00:00.000000 openllm_core-0.5.1/src/openllm_core/utils/codegen.py
+-rw-r--r--   0        0        0    19677 2020-02-02 00:00:00.000000 openllm_core-0.5.1/src/openllm_core/utils/dantic.py
+-rw-r--r--   0        0        0     2566 2020-02-02 00:00:00.000000 openllm_core-0.5.1/src/openllm_core/utils/import_utils.py
+-rw-r--r--   0        0        0      730 2020-02-02 00:00:00.000000 openllm_core-0.5.1/src/openllm_core/utils/import_utils.pyi
+-rw-r--r--   0        0        0     9997 2020-02-02 00:00:00.000000 openllm_core-0.5.1/src/openllm_core/utils/lazy.py
+-rw-r--r--   0        0        0     5381 2020-02-02 00:00:00.000000 openllm_core-0.5.1/src/openllm_core/utils/peft.py
+-rw-r--r--   0        0        0      951 2020-02-02 00:00:00.000000 openllm_core-0.5.1/src/openllm_core/utils/pkg.py
+-rw-r--r--   0        0        0     1003 2020-02-02 00:00:00.000000 openllm_core-0.5.1/src/openllm_core/utils/representation.py
+-rw-r--r--   0        0        0     1058 2020-02-02 00:00:00.000000 openllm_core-0.5.1/src/openllm_core/utils/serde.py
+-rw-r--r--   0        0        0     2087 2020-02-02 00:00:00.000000 openllm_core-0.5.1/.gitignore
+-rw-r--r--   0        0        0    10470 2020-02-02 00:00:00.000000 openllm_core-0.5.1/LICENSE.md
+-rw-r--r--   0        0        0     5980 2020-02-02 00:00:00.000000 openllm_core-0.5.1/pyproject.toml
+-rw-r--r--   0        0        0     6686 2020-02-02 00:00:00.000000 openllm_core-0.5.1/PKG-INFO
```

### Comparing `openllm_core-0.5.0a9/README.md` & `openllm_core-0.5.1/README.md`

 * *Files identical despite different names*

### Comparing `openllm_core-0.5.0a9/src/openllm_core/__init__.py` & `openllm_core-0.5.1/src/openllm_core/__init__.py`

 * *Files identical despite different names*

### Comparing `openllm_core-0.5.0a9/src/openllm_core/_configuration.py` & `openllm_core-0.5.1/src/openllm_core/_configuration.py`

 * *Files 4% similar despite different names*

```diff
@@ -11,21 +11,20 @@
   Required,
   Self,
   TypedDict,
   overload,
   Annotated,
 )
 from .exceptions import ForbiddenAttributeError, MissingDependencyError
-from .utils import field_env_key, first_not_none, is_vllm_available, is_transformers_available
+from .utils import field_env_key, is_vllm_available, is_transformers_available
 
 if t.TYPE_CHECKING:
   import transformers, vllm, openllm, torch
 
   from ._schemas import MessageParam
-  from .protocol.openai import ChatCompletionRequest, CompletionRequest
 
 __all__ = ['GenerationConfig', 'LLMConfig', 'field_env_key']
 
 logger = logging.getLogger(__name__)
 config_merger = Merger([(dict, 'merge')], ['override'], ['override'])
 _object_setattr = object.__setattr__
 
@@ -475,14 +474,18 @@
   @overload
   def __getitem__(self, item: t.Literal['max_tokens']) -> int: ...
   @overload
   def __getitem__(self, item: t.Literal['min_tokens']) -> int: ...
   @overload
   def __getitem__(self, item: t.Literal['logprobs']) -> t.Optional[int]: ...
   @overload
+  def __getitem__(self, item: t.Literal['detokenize']) -> bool: ...
+  @overload
+  def __getitem__(self, item: t.Literal['truncate_prompt_tokens']) -> t.Optional[Annotated[int, pydantic.Field(ge=1)]]: ...
+  @overload
   def __getitem__(self, item: t.Literal['prompt_logprobs']) -> t.Optional[int]: ...
   @overload
   def __getitem__(self, item: t.Literal['skip_special_tokens']) -> bool: ...
   @overload
   def __getitem__(self, item: t.Literal['spaces_between_special_tokens']) -> bool: ...
   @overload
   def __getitem__(self, item: t.Literal['logits_processors']) -> t.Optional[t.List[LogitsProcessor]]: ...
@@ -583,39 +586,14 @@
       return config.generation_config.build('pt')
 
   class hf:
     @staticmethod
     def build(config: LLMConfig) -> transformers.GenerationConfig:
       return config.generation_config.build('pt')
 
-  def compatible_options(self, request: ChatCompletionRequest | CompletionRequest) -> dict[str, t.Any]:
-    from .protocol.openai import ChatCompletionRequest, CompletionRequest
-
-    if isinstance(request, (ChatCompletionRequest, CompletionRequest)):
-      return self.openai.build(self, request)
-    raise TypeError(f'Unknown request type {type(request)}')
-
-  class openai:
-    @staticmethod
-    def build(config: LLMConfig, request: ChatCompletionRequest | CompletionRequest) -> dict[str, t.Any]:
-      d = dict(
-        temperature=first_not_none(request.temperature, config['temperature']),
-        top_p=first_not_none(request.top_p, config['top_p']),
-        top_k=first_not_none(request.top_k, config['top_k']),
-        best_of=first_not_none(request.best_of, config['best_of']),
-        n=first_not_none(request.n, default=config['n']),
-        stop=first_not_none(request.stop, default=None),
-        max_new_tokens=first_not_none(request.max_tokens, default=config['max_tokens']),
-        presence_penalty=first_not_none(request.presence_penalty, default=config['presence_penalty']),
-        frequency_penalty=first_not_none(request.frequency_penalty, default=config['frequency_penalty']),
-      )
-      if hasattr(request, 'logprobs'):
-        d['logprobs'] = first_not_none(request.logprobs, default=config['logprobs'])
-      return d
-
   @property
   def template(self) -> str:
     return '{system_message}{instruction}'
 
   @property
   def system_message(self) -> str:
     return ''
```

### Comparing `openllm_core-0.5.0a9/src/openllm_core/_schemas.py` & `openllm_core-0.5.1/src/openllm_core/_schemas.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 from __future__ import annotations
 
-import pydantic, inflection, orjson, typing as t
+import pydantic, orjson, typing as t
 from ._configuration import LLMConfig
 from .utils import gen_random_uuid
 from ._typing_compat import Required, TypedDict, LiteralString
 
 if t.TYPE_CHECKING:
   import vllm
 
@@ -43,24 +43,20 @@
   llm_config: LLMConfig = pydantic.Field(default_factory=dict)
   prompt_token_ids: t.Optional[t.List[int]] = pydantic.Field(default=None)
   stop: t.Optional[t.List[str]] = pydantic.Field(default=None)
   stop_token_ids: t.Optional[t.List[int]] = pydantic.Field(default=None)
   request_id: t.Optional[str] = pydantic.Field(default=None)
   adapter_name: t.Optional[str] = pydantic.Field(default=None)
 
-  _class_ref: t.ClassVar[type[LLMConfig]] = pydantic.PrivateAttr()
-
-  @pydantic.field_validator('llm_config')
-  @classmethod
-  def llm_config_validator(cls, v: LLMConfig | dict[str, t.Any]) -> LLMConfig:
-    if isinstance(v, dict):
-      return cls._class_ref.model_construct_env(**v)
-    return v
+  def __init__(self, *, _internal=False, **data: t.Any):
+    if not _internal:
+      raise RuntimeError('This class is not meant to be used directly. Use "from_config" instead')
+    super().__init__(**data)
 
-  @pydantic.field_validator('stop')
+  @pydantic.field_validator('stop', mode='before')
   @classmethod
   def stop_validator(cls, data: str | list[str] | t.Iterable[str] | None) -> list[str] | None:
     if data is None:
       return None
     if isinstance(data, str):
       return [data]
     else:
@@ -77,43 +73,17 @@
     })
     if self.stop is not None:
       flattened['stop'] = self.stop
     if self.stop_token_ids is not None:
       flattened['stop_token_ids'] = self.stop_token_ids
     return flattened
 
-  def __init__(self, /, *, _internal: bool = False, **data: t.Any) -> None:
-    if not _internal:
-      raise RuntimeError(
-        f'Cannot instantiate GenerationInput directly. Use "{self.__class__.__qualname__}.from_dict" instead.'
-      )
-    super().__init__(**data)
-
-  @classmethod
-  def from_dict(cls, structured: GenerationInputDict) -> GenerationInput:
-    if not hasattr(cls, '_class_ref'):
-      raise ValueError(
-        'Cannot use "from_dict" from a raw GenerationInput class. Currently only supports class created from "from_config".'
-      )
-    filtered: dict[str, t.Any] = {k: v for k, v in structured.items() if v is not None}
-    llm_config: dict[str, t.Any] | None = filtered.pop('llm_config', None)
-    if llm_config is not None:
-      filtered['llm_config'] = cls._class_ref.model_construct_env(**llm_config)
-
-    return cls(_internal=True, **filtered)
-
   @classmethod
   def from_config(cls, llm_config: LLMConfig) -> type[GenerationInput]:
-    klass = pydantic.create_model(
-      inflection.camelize(llm_config['start_name']) + 'GenerationInput',
-      __base__=cls,
-      llm_config=(type(llm_config), llm_config),
-      _class_ref=(llm_config.__class__, pydantic.PrivateAttr(default=llm_config.__class__)),
-    )
-    return klass
+    return cls(_internal=True, llm_config=llm_config)
 
 
 # NOTE: parameters from vllm.RequestOutput and vllm.CompletionOutput since vllm is not available on CPU.
 # OpenLLM will adapt CPU outputs to similar architecture with vLLM outputs for consistency
 
 SampleLogprobs = t.List[t.Dict[int, float]]
 PromptLogprobs = t.List[t.Optional[t.Dict[int, float]]]
```

### Comparing `openllm_core-0.5.0a9/src/openllm_core/_typing_compat.py` & `openllm_core-0.5.1/src/openllm_core/_typing_compat.py`

 * *Files identical despite different names*

### Comparing `openllm_core-0.5.0a9/src/openllm_core/exceptions.py` & `openllm_core-0.5.1/src/openllm_core/exceptions.py`

 * *Files identical despite different names*

### Comparing `openllm_core-0.5.0a9/src/openllm_core/config/__init__.py` & `openllm_core-0.5.1/src/openllm_core/config/__init__.py`

 * *Files identical despite different names*

### Comparing `openllm_core-0.5.0a9/src/openllm_core/config/configuration_auto.py` & `openllm_core-0.5.1/src/openllm_core/config/configuration_auto.py`

 * *Files 3% similar despite different names*

```diff
@@ -214,7 +214,20 @@
 
     arch = bentomodel.info.metadata['architectures'][0]
     if arch in cls._architecture_mappings:
       return cls.for_model(cls._architecture_mappings[arch]).model_construct_env(**attrs)
     raise ValueError(
       f"Failed to determine config class for '{bentomodel.name}'. Make sure {bentomodel.name} is saved with openllm."
     )
+
+  @classmethod
+  def from_id(cls, model_id: str, *, trust_remote_code: bool = False, **attrs: t.Any) -> openllm_core.LLMConfig:
+    import transformers
+
+    config = transformers.AutoConfig.from_pretrained(model_id, trust_remote_code=trust_remote_code)
+    for arch in config.architectures:
+      if arch in cls._architecture_mappings:
+        return cls.for_model(cls._architecture_mappings[arch]).model_construct_env(**attrs)
+    else:
+      raise RuntimeError(
+        f'Failed to determine config class for {model_id}. Got {config.architectures}, which is not yet supported (Supported: {list(cls._architecture_mappings.keys())})'
+      )
```

### Comparing `openllm_core-0.5.0a9/src/openllm_core/config/configuration_baichuan.py` & `openllm_core-0.5.1/src/openllm_core/config/configuration_baichuan.py`

 * *Files identical despite different names*

### Comparing `openllm_core-0.5.0a9/src/openllm_core/config/configuration_chatglm.py` & `openllm_core-0.5.1/src/openllm_core/config/configuration_chatglm.py`

 * *Files identical despite different names*

### Comparing `openllm_core-0.5.0a9/src/openllm_core/config/configuration_dbrx.py` & `openllm_core-0.5.1/src/openllm_core/config/configuration_dbrx.py`

 * *Files identical despite different names*

### Comparing `openllm_core-0.5.0a9/src/openllm_core/config/configuration_dolly_v2.py` & `openllm_core-0.5.1/src/openllm_core/config/configuration_dolly_v2.py`

 * *Files identical despite different names*

### Comparing `openllm_core-0.5.0a9/src/openllm_core/config/configuration_falcon.py` & `openllm_core-0.5.1/src/openllm_core/config/configuration_falcon.py`

 * *Files identical despite different names*

### Comparing `openllm_core-0.5.0a9/src/openllm_core/config/configuration_flan_t5.py` & `openllm_core-0.5.1/src/openllm_core/config/configuration_flan_t5.py`

 * *Files identical despite different names*

### Comparing `openllm_core-0.5.0a9/src/openllm_core/config/configuration_gemma.py` & `openllm_core-0.5.1/src/openllm_core/config/configuration_gemma.py`

 * *Files identical despite different names*

### Comparing `openllm_core-0.5.0a9/src/openllm_core/config/configuration_gpt_neox.py` & `openllm_core-0.5.1/src/openllm_core/config/configuration_gpt_neox.py`

 * *Files identical despite different names*

### Comparing `openllm_core-0.5.0a9/src/openllm_core/config/configuration_llama.py` & `openllm_core-0.5.1/src/openllm_core/config/configuration_llama.py`

 * *Files identical despite different names*

### Comparing `openllm_core-0.5.0a9/src/openllm_core/config/configuration_mistral.py` & `openllm_core-0.5.1/src/openllm_core/config/configuration_mistral.py`

 * *Files identical despite different names*

### Comparing `openllm_core-0.5.0a9/src/openllm_core/config/configuration_mixtral.py` & `openllm_core-0.5.1/src/openllm_core/config/configuration_mixtral.py`

 * *Files identical despite different names*

### Comparing `openllm_core-0.5.0a9/src/openllm_core/config/configuration_mpt.py` & `openllm_core-0.5.1/src/openllm_core/config/configuration_mpt.py`

 * *Files identical despite different names*

### Comparing `openllm_core-0.5.0a9/src/openllm_core/config/configuration_opt.py` & `openllm_core-0.5.1/src/openllm_core/config/configuration_opt.py`

 * *Files identical despite different names*

### Comparing `openllm_core-0.5.0a9/src/openllm_core/config/configuration_qwen.py` & `openllm_core-0.5.1/src/openllm_core/config/configuration_qwen.py`

 * *Files identical despite different names*

### Comparing `openllm_core-0.5.0a9/src/openllm_core/config/configuration_stablelm.py` & `openllm_core-0.5.1/src/openllm_core/config/configuration_stablelm.py`

 * *Files identical despite different names*

### Comparing `openllm_core-0.5.0a9/src/openllm_core/config/configuration_starcoder.py` & `openllm_core-0.5.1/src/openllm_core/config/configuration_starcoder.py`

 * *Files identical despite different names*

### Comparing `openllm_core-0.5.0a9/src/openllm_core/config/configuration_yi.py` & `openllm_core-0.5.1/src/openllm_core/config/configuration_yi.py`

 * *Files identical despite different names*

### Comparing `openllm_core-0.5.0a9/src/openllm_core/protocol/openai.py` & `openllm_core-0.5.1/src/openllm_core/protocol/openai.py`

 * *Files identical despite different names*

### Comparing `openllm_core-0.5.0a9/src/openllm_core/utils/__init__.py` & `openllm_core-0.5.1/src/openllm_core/utils/__init__.py`

 * *Files 3% similar despite different names*

```diff
@@ -10,14 +10,15 @@
   WARNING_ENV_VAR as WARNING_ENV_VAR,
   DEV_DEBUG_VAR as DEV_DEBUG_VAR,
   ENV_VARS_TRUE_VALUES as ENV_VARS_TRUE_VALUES,
   check_bool_env as check_bool_env,
   DEBUG as DEBUG,
   SHOW_CODEGEN as SHOW_CODEGEN,
   MYPY as MYPY,
+  OPENLLM_DEV_BUILD as OPENLLM_DEV_BUILD,
 )
 
 if t.TYPE_CHECKING:
   from _bentoml_sdk import IODescriptor
 
 # equivocal setattr to save one lookup per assignment
 _object_setattr = object.__setattr__
```

### Comparing `openllm_core-0.5.0a9/src/openllm_core/utils/__init__.pyi` & `openllm_core-0.5.1/src/openllm_core/utils/__init__.pyi`

 * *Files 1% similar despite different names*

```diff
@@ -40,14 +40,15 @@
 DEBUG: bool = ...
 SHOW_CODEGEN: bool = ...
 MYPY: bool = ...
 DEBUG_ENV_VAR: str = ...
 QUIET_ENV_VAR: str = ...
 DEV_DEBUG_VAR: str = ...
 WARNING_ENV_VAR: str = ...
+OPENLLM_DEV_BUILD: str = ...
 
 _T = TypeVar('_T')
 R = TypeVar('R')
 P = ParamSpec('P')
 
 @functools.lru_cache(maxsize=1)
 def has_gpus() -> bool: ...
```

### Comparing `openllm_core-0.5.0a9/src/openllm_core/utils/_constants.py` & `openllm_core-0.5.1/src/openllm_core/utils/_constants.py`

 * *Files 15% similar despite different names*

```diff
@@ -5,14 +5,15 @@
 QUIET_ENV_VAR = 'BENTOML_QUIET'
 # https://github.com/grpc/grpc/blob/master/doc/environment_variables.md
 GRPC_DEBUG_ENV_VAR = 'GRPC_VERBOSITY'
 WARNING_ENV_VAR = 'OPENLLM_DISABLE_WARNING'
 DEV_DEBUG_VAR = 'DEBUG'
 
 ENV_VARS_TRUE_VALUES = {'1', 'ON', 'YES', 'TRUE'}
+OPENLLM_DEV_BUILD = 'OPENLLM_DEV_BUILD'
 
 
 def check_bool_env(env: str, default: bool = True):
   v = os.getenv(env, default=str(default)).upper()
   if v.isdigit():
     return bool(int(v))  # special check for digits
   return v in ENV_VARS_TRUE_VALUES
```

### Comparing `openllm_core-0.5.0a9/src/openllm_core/utils/analytics.py` & `openllm_core-0.5.1/src/openllm_core/utils/analytics.py`

 * *Files identical despite different names*

### Comparing `openllm_core-0.5.0a9/src/openllm_core/utils/codegen.py` & `openllm_core-0.5.1/src/openllm_core/utils/codegen.py`

 * *Files identical despite different names*

### Comparing `openllm_core-0.5.0a9/src/openllm_core/utils/dantic.py` & `openllm_core-0.5.1/src/openllm_core/utils/dantic.py`

 * *Files identical despite different names*

### Comparing `openllm_core-0.5.0a9/src/openllm_core/utils/import_utils.py` & `openllm_core-0.5.1/src/openllm_core/utils/import_utils.py`

 * *Files identical despite different names*

### Comparing `openllm_core-0.5.0a9/src/openllm_core/utils/import_utils.pyi` & `openllm_core-0.5.1/src/openllm_core/utils/import_utils.pyi`

 * *Files identical despite different names*

### Comparing `openllm_core-0.5.0a9/src/openllm_core/utils/lazy.py` & `openllm_core-0.5.1/src/openllm_core/utils/lazy.py`

 * *Files identical despite different names*

### Comparing `openllm_core-0.5.0a9/src/openllm_core/utils/peft.py` & `openllm_core-0.5.1/src/openllm_core/utils/peft.py`

 * *Files identical despite different names*

### Comparing `openllm_core-0.5.0a9/src/openllm_core/utils/pkg.py` & `openllm_core-0.5.1/src/openllm_core/utils/pkg.py`

 * *Files identical despite different names*

### Comparing `openllm_core-0.5.0a9/src/openllm_core/utils/representation.py` & `openllm_core-0.5.1/src/openllm_core/utils/representation.py`

 * *Files identical despite different names*

### Comparing `openllm_core-0.5.0a9/src/openllm_core/utils/serde.py` & `openllm_core-0.5.1/src/openllm_core/utils/serde.py`

 * *Files identical despite different names*

### Comparing `openllm_core-0.5.0a9/.gitignore` & `openllm_core-0.5.1/.gitignore`

 * *Files identical despite different names*

### Comparing `openllm_core-0.5.0a9/LICENSE.md` & `openllm_core-0.5.1/LICENSE.md`

 * *Files identical despite different names*

### Comparing `openllm_core-0.5.0a9/pyproject.toml` & `openllm_core-0.5.1/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -60,14 +60,16 @@
 dependencies = [
     "attrs>=23.2.0",
     "pydantic>2",
     "orjson",
     "inflection",
     "typing_extensions",
     "mypy_extensions",
+    "packaging",
+    "deepmerge",
 ]
 license = "Apache-2.0"
 name = "openllm-core"
 requires-python = ">=3.8"
 [project.urls]
 Blog = "https://modelserving.com"
 Chat = "https://l.bentoml.com/join-openllm-discord"
```

### Comparing `openllm_core-0.5.0a9/PKG-INFO` & `openllm_core-0.5.1/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: openllm-core
-Version: 0.5.0a9
+Version: 0.5.1
 Summary: OpenLLM Core: Core components for OpenLLM.
 Project-URL: Blog, https://modelserving.com
 Project-URL: Chat, https://l.bentoml.com/join-openllm-discord
 Project-URL: Documentation, https://github.com/bentoml/OpenLLM/blob/main/openllm-core/README.md
 Project-URL: GitHub, https://github.com/bentoml/OpenLLM/blob/main/openllm-core
 Project-URL: History, https://github.com/bentoml/OpenLLM/blob/main/CHANGELOG.md
 Project-URL: Homepage, https://bentoml.com
@@ -35,17 +35,19 @@
 Classifier: Programming Language :: Python :: Implementation :: PyPy
 Classifier: Topic :: Scientific/Engineering
 Classifier: Topic :: Scientific/Engineering :: Artificial Intelligence
 Classifier: Topic :: Software Development :: Libraries
 Classifier: Typing :: Typed
 Requires-Python: >=3.8
 Requires-Dist: attrs>=23.2.0
+Requires-Dist: deepmerge
 Requires-Dist: inflection
 Requires-Dist: mypy-extensions
 Requires-Dist: orjson
+Requires-Dist: packaging
 Requires-Dist: pydantic>2
 Requires-Dist: typing-extensions
 Provides-Extra: bentoml
 Requires-Dist: bentoml>=1.2; extra == 'bentoml'
 Provides-Extra: full
 Requires-Dist: openllm-core[bentoml,transformers,vllm]; extra == 'full'
 Provides-Extra: transformers
```

#### html2text {}

```diff
@@ -1,9 +1,9 @@
-Metadata-Version: 2.1 Name: openllm-core Version: 0.5.0a9 Summary: OpenLLM
-Core: Core components for OpenLLM. Project-URL: Blog, https://modelserving.com
+Metadata-Version: 2.1 Name: openllm-core Version: 0.5.1 Summary: OpenLLM Core:
+Core components for OpenLLM. Project-URL: Blog, https://modelserving.com
 Project-URL: Chat, https://l.bentoml.com/join-openllm-discord Project-URL:
 Documentation, https://github.com/bentoml/OpenLLM/blob/main/openllm-core/
 README.md Project-URL: GitHub, https://github.com/bentoml/OpenLLM/blob/main/
 openllm-core Project-URL: History, https://github.com/bentoml/OpenLLM/blob/
 main/CHANGELOG.md Project-URL: Homepage, https://bentoml.com Project-URL:
 Tracker, https://github.com/bentoml/OpenLLM/issues Project-URL: Twitter, https:
 //twitter.com/bentomlai Author-email: Aaron Pham
@@ -24,22 +24,22 @@
 3.8 Classifier: Programming Language :: Python :: 3.9 Classifier: Programming
 Language :: Python :: 3.10 Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: Python :: Implementation :: CPython
 Classifier: Programming Language :: Python :: Implementation :: PyPy
 Classifier: Topic :: Scientific/Engineering Classifier: Topic :: Scientific/
 Engineering :: Artificial Intelligence Classifier: Topic :: Software
 Development :: Libraries Classifier: Typing :: Typed Requires-Python: >=3.8
-Requires-Dist: attrs>=23.2.0 Requires-Dist: inflection Requires-Dist: mypy-
-extensions Requires-Dist: orjson Requires-Dist: pydantic>2 Requires-Dist:
-typing-extensions Provides-Extra: bentoml Requires-Dist: bentoml>=1.2; extra ==
-'bentoml' Provides-Extra: full Requires-Dist: openllm-core
-[bentoml,transformers,vllm]; extra == 'full' Provides-Extra: transformers
-Requires-Dist: transformers>=4.36.0; extra == 'transformers' Provides-Extra:
-vllm Requires-Dist: vllm>=0.3.0; extra == 'vllm' Description-Content-Type:
-text/markdown
+Requires-Dist: attrs>=23.2.0 Requires-Dist: deepmerge Requires-Dist: inflection
+Requires-Dist: mypy-extensions Requires-Dist: orjson Requires-Dist: packaging
+Requires-Dist: pydantic>2 Requires-Dist: typing-extensions Provides-Extra:
+bentoml Requires-Dist: bentoml>=1.2; extra == 'bentoml' Provides-Extra: full
+Requires-Dist: openllm-core[bentoml,transformers,vllm]; extra == 'full'
+Provides-Extra: transformers Requires-Dist: transformers>=4.36.0; extra ==
+'transformers' Provides-Extra: vllm Requires-Dist: vllm>=0.3.0; extra == 'vllm'
+Description-Content-Type: text/markdown
                              _[_B_a_n_n_e_r_ _f_o_r_ _O_p_e_n_L_L_M_]
                         ************ ?ð??¦? OOppeennLLLLMM CCoorree ************
   _[_p_y_p_i___s_t_a_t_u_s_]_[_t_e_s_t___p_y_p_i___s_t_a_t_u_s_]_[_T_w_i_t_t_e_r_]_[_D_i_s_c_o_r_d_]_[_c_i_]_[_p_r_e_-_c_o_m_m_i_t_._c_i_ _s_t_a_t_u_s_]
    _[_p_y_t_h_o_n___v_e_r_s_i_o_n_]_[_H_a_t_c_h_]_[_c_o_d_e_ _s_t_y_l_e_]_[_R_u_f_f_]_[_t_y_p_e_s_ _-_ _m_y_p_y_]_[_t_y_p_e_s_ _-_ _p_y_r_i_g_h_t_]
                   OpenLLM Core: Core components for OpenLLM.
 ## ð Introduction With OpenLLM, you can run inference with any open-source
 large-language models, deploy to the cloud or on-premises, and build powerful
```

