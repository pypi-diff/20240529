# Comparing `tmp/openllm_core-0.5.1.tar.gz` & `tmp/openllm_core-0.5.2.tar.gz`

## Comparing `openllm_core-0.5.1.tar` & `openllm_core-0.5.2.tar`

### file list

```diff
@@ -1,48 +1,47 @@
--rw-r--r--   0        0        0     3618 2020-02-02 00:00:00.000000 openllm_core-0.5.1/README.md
--rw-r--r--   0        0        0      912 2020-02-02 00:00:00.000000 openllm_core-0.5.1/src/openllm_core/__init__.py
--rw-r--r--   0        0        0    29344 2020-02-02 00:00:00.000000 openllm_core-0.5.1/src/openllm_core/_configuration.py
--rw-r--r--   0        0        0     5791 2020-02-02 00:00:00.000000 openllm_core-0.5.1/src/openllm_core/_schemas.py
--rw-r--r--   0        0        0     2399 2020-02-02 00:00:00.000000 openllm_core-0.5.1/src/openllm_core/_typing_compat.py
--rw-r--r--   0        0        0      411 2020-02-02 00:00:00.000000 openllm_core-0.5.1/src/openllm_core/_version.py
--rw-r--r--   0        0        0     1276 2020-02-02 00:00:00.000000 openllm_core-0.5.1/src/openllm_core/exceptions.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 openllm_core-0.5.1/src/openllm_core/py.typed
--rw-r--r--   0        0        0     1319 2020-02-02 00:00:00.000000 openllm_core-0.5.1/src/openllm_core/config/__init__.py
--rw-r--r--   0        0        0     9257 2020-02-02 00:00:00.000000 openllm_core-0.5.1/src/openllm_core/config/configuration_auto.py
--rw-r--r--   0        0        0     1892 2020-02-02 00:00:00.000000 openllm_core-0.5.1/src/openllm_core/config/configuration_baichuan.py
--rw-r--r--   0        0        0     1774 2020-02-02 00:00:00.000000 openllm_core-0.5.1/src/openllm_core/config/configuration_chatglm.py
--rw-r--r--   0        0        0     1157 2020-02-02 00:00:00.000000 openllm_core-0.5.1/src/openllm_core/config/configuration_dbrx.py
--rw-r--r--   0        0        0     2453 2020-02-02 00:00:00.000000 openllm_core-0.5.1/src/openllm_core/config/configuration_dolly_v2.py
--rw-r--r--   0        0        0     1768 2020-02-02 00:00:00.000000 openllm_core-0.5.1/src/openllm_core/config/configuration_falcon.py
--rw-r--r--   0        0        0     1576 2020-02-02 00:00:00.000000 openllm_core-0.5.1/src/openllm_core/config/configuration_flan_t5.py
--rw-r--r--   0        0        0     1301 2020-02-02 00:00:00.000000 openllm_core-0.5.1/src/openllm_core/config/configuration_gemma.py
--rw-r--r--   0        0        0     1687 2020-02-02 00:00:00.000000 openllm_core-0.5.1/src/openllm_core/config/configuration_gpt_neox.py
--rw-r--r--   0        0        0     3283 2020-02-02 00:00:00.000000 openllm_core-0.5.1/src/openllm_core/config/configuration_llama.py
--rw-r--r--   0        0        0     3420 2020-02-02 00:00:00.000000 openllm_core-0.5.1/src/openllm_core/config/configuration_mistral.py
--rw-r--r--   0        0        0     3010 2020-02-02 00:00:00.000000 openllm_core-0.5.1/src/openllm_core/config/configuration_mixtral.py
--rw-r--r--   0        0        0     1495 2020-02-02 00:00:00.000000 openllm_core-0.5.1/src/openllm_core/config/configuration_mpt.py
--rw-r--r--   0        0        0     1930 2020-02-02 00:00:00.000000 openllm_core-0.5.1/src/openllm_core/config/configuration_opt.py
--rw-r--r--   0        0        0     2563 2020-02-02 00:00:00.000000 openllm_core-0.5.1/src/openllm_core/config/configuration_phi.py
--rw-r--r--   0        0        0     1550 2020-02-02 00:00:00.000000 openllm_core-0.5.1/src/openllm_core/config/configuration_qwen.py
--rw-r--r--   0        0        0     2269 2020-02-02 00:00:00.000000 openllm_core-0.5.1/src/openllm_core/config/configuration_stablelm.py
--rw-r--r--   0        0        0     1516 2020-02-02 00:00:00.000000 openllm_core-0.5.1/src/openllm_core/config/configuration_starcoder.py
--rw-r--r--   0        0        0     1446 2020-02-02 00:00:00.000000 openllm_core-0.5.1/src/openllm_core/config/configuration_yi.py
--rw-r--r--   0        0        0      324 2020-02-02 00:00:00.000000 openllm_core-0.5.1/src/openllm_core/protocol/__init__.py
--rw-r--r--   0        0        0      296 2020-02-02 00:00:00.000000 openllm_core-0.5.1/src/openllm_core/protocol/hf.py
--rw-r--r--   0        0        0     7231 2020-02-02 00:00:00.000000 openllm_core-0.5.1/src/openllm_core/protocol/openai.py
--rw-r--r--   0        0        0    13850 2020-02-02 00:00:00.000000 openllm_core-0.5.1/src/openllm_core/utils/__init__.py
--rw-r--r--   0        0        0     4757 2020-02-02 00:00:00.000000 openllm_core-0.5.1/src/openllm_core/utils/__init__.pyi
--rw-r--r--   0        0        0     1084 2020-02-02 00:00:00.000000 openllm_core-0.5.1/src/openllm_core/utils/_constants.py
--rw-r--r--   0        0        0     3059 2020-02-02 00:00:00.000000 openllm_core-0.5.1/src/openllm_core/utils/analytics.py
--rw-r--r--   0        0        0     6667 2020-02-02 00:00:00.000000 openllm_core-0.5.1/src/openllm_core/utils/codegen.py
--rw-r--r--   0        0        0    19677 2020-02-02 00:00:00.000000 openllm_core-0.5.1/src/openllm_core/utils/dantic.py
--rw-r--r--   0        0        0     2566 2020-02-02 00:00:00.000000 openllm_core-0.5.1/src/openllm_core/utils/import_utils.py
--rw-r--r--   0        0        0      730 2020-02-02 00:00:00.000000 openllm_core-0.5.1/src/openllm_core/utils/import_utils.pyi
--rw-r--r--   0        0        0     9997 2020-02-02 00:00:00.000000 openllm_core-0.5.1/src/openllm_core/utils/lazy.py
--rw-r--r--   0        0        0     5381 2020-02-02 00:00:00.000000 openllm_core-0.5.1/src/openllm_core/utils/peft.py
--rw-r--r--   0        0        0      951 2020-02-02 00:00:00.000000 openllm_core-0.5.1/src/openllm_core/utils/pkg.py
--rw-r--r--   0        0        0     1003 2020-02-02 00:00:00.000000 openllm_core-0.5.1/src/openllm_core/utils/representation.py
--rw-r--r--   0        0        0     1058 2020-02-02 00:00:00.000000 openllm_core-0.5.1/src/openllm_core/utils/serde.py
--rw-r--r--   0        0        0     2087 2020-02-02 00:00:00.000000 openllm_core-0.5.1/.gitignore
--rw-r--r--   0        0        0    10470 2020-02-02 00:00:00.000000 openllm_core-0.5.1/LICENSE.md
--rw-r--r--   0        0        0     5980 2020-02-02 00:00:00.000000 openllm_core-0.5.1/pyproject.toml
--rw-r--r--   0        0        0     6686 2020-02-02 00:00:00.000000 openllm_core-0.5.1/PKG-INFO
+-rw-r--r--   0        0        0     3618 2020-02-02 00:00:00.000000 openllm_core-0.5.2/README.md
+-rw-r--r--   0        0        0      880 2020-02-02 00:00:00.000000 openllm_core-0.5.2/src/openllm_core/__init__.py
+-rw-r--r--   0        0        0    29344 2020-02-02 00:00:00.000000 openllm_core-0.5.2/src/openllm_core/_configuration.py
+-rw-r--r--   0        0        0     5791 2020-02-02 00:00:00.000000 openllm_core-0.5.2/src/openllm_core/_schemas.py
+-rw-r--r--   0        0        0     2399 2020-02-02 00:00:00.000000 openllm_core-0.5.2/src/openllm_core/_typing_compat.py
+-rw-r--r--   0        0        0      411 2020-02-02 00:00:00.000000 openllm_core-0.5.2/src/openllm_core/_version.py
+-rw-r--r--   0        0        0     1276 2020-02-02 00:00:00.000000 openllm_core-0.5.2/src/openllm_core/exceptions.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 openllm_core-0.5.2/src/openllm_core/py.typed
+-rw-r--r--   0        0        0     1255 2020-02-02 00:00:00.000000 openllm_core-0.5.2/src/openllm_core/config/__init__.py
+-rw-r--r--   0        0        0     9070 2020-02-02 00:00:00.000000 openllm_core-0.5.2/src/openllm_core/config/configuration_auto.py
+-rw-r--r--   0        0        0     1892 2020-02-02 00:00:00.000000 openllm_core-0.5.2/src/openllm_core/config/configuration_baichuan.py
+-rw-r--r--   0        0        0     1774 2020-02-02 00:00:00.000000 openllm_core-0.5.2/src/openllm_core/config/configuration_chatglm.py
+-rw-r--r--   0        0        0     1157 2020-02-02 00:00:00.000000 openllm_core-0.5.2/src/openllm_core/config/configuration_dbrx.py
+-rw-r--r--   0        0        0     2453 2020-02-02 00:00:00.000000 openllm_core-0.5.2/src/openllm_core/config/configuration_dolly_v2.py
+-rw-r--r--   0        0        0     1768 2020-02-02 00:00:00.000000 openllm_core-0.5.2/src/openllm_core/config/configuration_falcon.py
+-rw-r--r--   0        0        0     1301 2020-02-02 00:00:00.000000 openllm_core-0.5.2/src/openllm_core/config/configuration_gemma.py
+-rw-r--r--   0        0        0     1687 2020-02-02 00:00:00.000000 openllm_core-0.5.2/src/openllm_core/config/configuration_gpt_neox.py
+-rw-r--r--   0        0        0     3283 2020-02-02 00:00:00.000000 openllm_core-0.5.2/src/openllm_core/config/configuration_llama.py
+-rw-r--r--   0        0        0     3420 2020-02-02 00:00:00.000000 openllm_core-0.5.2/src/openllm_core/config/configuration_mistral.py
+-rw-r--r--   0        0        0     3010 2020-02-02 00:00:00.000000 openllm_core-0.5.2/src/openllm_core/config/configuration_mixtral.py
+-rw-r--r--   0        0        0     1495 2020-02-02 00:00:00.000000 openllm_core-0.5.2/src/openllm_core/config/configuration_mpt.py
+-rw-r--r--   0        0        0     1930 2020-02-02 00:00:00.000000 openllm_core-0.5.2/src/openllm_core/config/configuration_opt.py
+-rw-r--r--   0        0        0     2563 2020-02-02 00:00:00.000000 openllm_core-0.5.2/src/openllm_core/config/configuration_phi.py
+-rw-r--r--   0        0        0     1550 2020-02-02 00:00:00.000000 openllm_core-0.5.2/src/openllm_core/config/configuration_qwen.py
+-rw-r--r--   0        0        0     2269 2020-02-02 00:00:00.000000 openllm_core-0.5.2/src/openllm_core/config/configuration_stablelm.py
+-rw-r--r--   0        0        0     1516 2020-02-02 00:00:00.000000 openllm_core-0.5.2/src/openllm_core/config/configuration_starcoder.py
+-rw-r--r--   0        0        0     1446 2020-02-02 00:00:00.000000 openllm_core-0.5.2/src/openllm_core/config/configuration_yi.py
+-rw-r--r--   0        0        0      324 2020-02-02 00:00:00.000000 openllm_core-0.5.2/src/openllm_core/protocol/__init__.py
+-rw-r--r--   0        0        0      296 2020-02-02 00:00:00.000000 openllm_core-0.5.2/src/openllm_core/protocol/hf.py
+-rw-r--r--   0        0        0     7231 2020-02-02 00:00:00.000000 openllm_core-0.5.2/src/openllm_core/protocol/openai.py
+-rw-r--r--   0        0        0    13850 2020-02-02 00:00:00.000000 openllm_core-0.5.2/src/openllm_core/utils/__init__.py
+-rw-r--r--   0        0        0     4757 2020-02-02 00:00:00.000000 openllm_core-0.5.2/src/openllm_core/utils/__init__.pyi
+-rw-r--r--   0        0        0     1084 2020-02-02 00:00:00.000000 openllm_core-0.5.2/src/openllm_core/utils/_constants.py
+-rw-r--r--   0        0        0     3059 2020-02-02 00:00:00.000000 openllm_core-0.5.2/src/openllm_core/utils/analytics.py
+-rw-r--r--   0        0        0     6667 2020-02-02 00:00:00.000000 openllm_core-0.5.2/src/openllm_core/utils/codegen.py
+-rw-r--r--   0        0        0    19677 2020-02-02 00:00:00.000000 openllm_core-0.5.2/src/openllm_core/utils/dantic.py
+-rw-r--r--   0        0        0     2566 2020-02-02 00:00:00.000000 openllm_core-0.5.2/src/openllm_core/utils/import_utils.py
+-rw-r--r--   0        0        0      730 2020-02-02 00:00:00.000000 openllm_core-0.5.2/src/openllm_core/utils/import_utils.pyi
+-rw-r--r--   0        0        0     9997 2020-02-02 00:00:00.000000 openllm_core-0.5.2/src/openllm_core/utils/lazy.py
+-rw-r--r--   0        0        0     5381 2020-02-02 00:00:00.000000 openllm_core-0.5.2/src/openllm_core/utils/peft.py
+-rw-r--r--   0        0        0      951 2020-02-02 00:00:00.000000 openllm_core-0.5.2/src/openllm_core/utils/pkg.py
+-rw-r--r--   0        0        0     1003 2020-02-02 00:00:00.000000 openllm_core-0.5.2/src/openllm_core/utils/representation.py
+-rw-r--r--   0        0        0     1058 2020-02-02 00:00:00.000000 openllm_core-0.5.2/src/openllm_core/utils/serde.py
+-rw-r--r--   0        0        0     2087 2020-02-02 00:00:00.000000 openllm_core-0.5.2/.gitignore
+-rw-r--r--   0        0        0    10470 2020-02-02 00:00:00.000000 openllm_core-0.5.2/LICENSE.md
+-rw-r--r--   0        0        0     5980 2020-02-02 00:00:00.000000 openllm_core-0.5.2/pyproject.toml
+-rw-r--r--   0        0        0     6686 2020-02-02 00:00:00.000000 openllm_core-0.5.2/PKG-INFO
```

### Comparing `openllm_core-0.5.1/README.md` & `openllm_core-0.5.2/README.md`

 * *Files identical despite different names*

### Comparing `openllm_core-0.5.1/src/openllm_core/__init__.py` & `openllm_core-0.5.2/src/openllm_core/__init__.py`

 * *Files 16% similar despite different names*

```diff
@@ -11,15 +11,14 @@
   CONFIG_MAPPING as CONFIG_MAPPING,
   CONFIG_MAPPING_NAMES as CONFIG_MAPPING_NAMES,
   AutoConfig as AutoConfig,
   BaichuanConfig as BaichuanConfig,
   ChatGLMConfig as ChatGLMConfig,
   DollyV2Config as DollyV2Config,
   FalconConfig as FalconConfig,
-  FlanT5Config as FlanT5Config,
   GPTNeoXConfig as GPTNeoXConfig,
   LlamaConfig as LlamaConfig,
   MistralConfig as MistralConfig,
   MPTConfig as MPTConfig,
   OPTConfig as OPTConfig,
   StableLMConfig as StableLMConfig,
   StarCoderConfig as StarCoderConfig,
```

### Comparing `openllm_core-0.5.1/src/openllm_core/_configuration.py` & `openllm_core-0.5.2/src/openllm_core/_configuration.py`

 * *Files identical despite different names*

### Comparing `openllm_core-0.5.1/src/openllm_core/_schemas.py` & `openllm_core-0.5.2/src/openllm_core/_schemas.py`

 * *Files identical despite different names*

### Comparing `openllm_core-0.5.1/src/openllm_core/_typing_compat.py` & `openllm_core-0.5.2/src/openllm_core/_typing_compat.py`

 * *Files identical despite different names*

### Comparing `openllm_core-0.5.1/src/openllm_core/exceptions.py` & `openllm_core-0.5.2/src/openllm_core/exceptions.py`

 * *Files identical despite different names*

### Comparing `openllm_core-0.5.1/src/openllm_core/config/__init__.py` & `openllm_core-0.5.2/src/openllm_core/config/__init__.py`

 * *Files 4% similar despite different names*

```diff
@@ -2,15 +2,14 @@
 # AUTOGENERATED BY update-config-stubs.py. DO NOT EDIT
 from .configuration_auto import CONFIG_MAPPING as CONFIG_MAPPING, CONFIG_MAPPING_NAMES as CONFIG_MAPPING_NAMES, AutoConfig as AutoConfig
 from .configuration_baichuan import BaichuanConfig as BaichuanConfig
 from .configuration_chatglm import ChatGLMConfig as ChatGLMConfig
 from .configuration_dbrx import DbrxConfig as DbrxConfig
 from .configuration_dolly_v2 import DollyV2Config as DollyV2Config
 from .configuration_falcon import FalconConfig as FalconConfig
-from .configuration_flan_t5 import FlanT5Config as FlanT5Config
 from .configuration_gemma import GemmaConfig as GemmaConfig
 from .configuration_gpt_neox import GPTNeoXConfig as GPTNeoXConfig
 from .configuration_llama import LlamaConfig as LlamaConfig
 from .configuration_mistral import MistralConfig as MistralConfig
 from .configuration_mixtral import MixtralConfig as MixtralConfig
 from .configuration_mpt import MPTConfig as MPTConfig
 from .configuration_opt import OPTConfig as OPTConfig
```

### Comparing `openllm_core-0.5.1/src/openllm_core/config/configuration_auto.py` & `openllm_core-0.5.2/src/openllm_core/config/configuration_auto.py`

 * *Files 1% similar despite different names*

```diff
@@ -17,15 +17,14 @@
   ConfigValuesView = _odict_values[str, type[openllm_core.LLMConfig]]
   ConfigItemsView = _odict_items[str, type[openllm_core.LLMConfig]]
   OrderedDictType = OrderedDict[LiteralString, type[openllm_core.LLMConfig]]
 else:
   OrderedDictType = OrderedDict
 
 ModelType: t.TypeAlias = t.Literal[
-  'flan_t5',
   'baichuan',
   'chatglm',
   'falcon',
   'gemma',
   'gpt_neox',
   'dolly_v2',
   'dbrx',
@@ -40,15 +39,14 @@
   'mixtral',
   'yi',
 ]
 
 # NOTE: This is the entrypoint when adding new model config
 CONFIG_MAPPING_NAMES: OrderedDict[ModelType, str] = OrderedDict(
   sorted([
-    ('flan_t5', 'FlanT5Config'),
     ('baichuan', 'BaichuanConfig'),
     ('chatglm', 'ChatGLMConfig'),
     ('falcon', 'FalconConfig'),
     ('gpt_neox', 'GPTNeoXConfig'),
     ('gemma', 'GemmaConfig'),
     ('dbrx', 'DbrxConfig'),
     ('dolly_v2', 'DollyV2Config'),
@@ -141,17 +139,14 @@
   @classmethod
   def for_model(cls, model_name: t.Literal['dolly_v2'], **attrs: t.Any) -> openllm_core.config.DollyV2Config: ...
   @t.overload
   @classmethod
   def for_model(cls, model_name: t.Literal['falcon'], **attrs: t.Any) -> openllm_core.config.FalconConfig: ...
   @t.overload
   @classmethod
-  def for_model(cls, model_name: t.Literal['flan_t5'], **attrs: t.Any) -> openllm_core.config.FlanT5Config: ...
-  @t.overload
-  @classmethod
   def for_model(cls, model_name: t.Literal['gemma'], **attrs: t.Any) -> openllm_core.config.GemmaConfig: ...
   @t.overload
   @classmethod
   def for_model(cls, model_name: t.Literal['gpt_neox'], **attrs: t.Any) -> openllm_core.config.GPTNeoXConfig: ...
   @t.overload
   @classmethod
   def for_model(cls, model_name: t.Literal['llama'], **attrs: t.Any) -> openllm_core.config.LlamaConfig: ...
```

### Comparing `openllm_core-0.5.1/src/openllm_core/config/configuration_baichuan.py` & `openllm_core-0.5.2/src/openllm_core/config/configuration_baichuan.py`

 * *Files identical despite different names*

### Comparing `openllm_core-0.5.1/src/openllm_core/config/configuration_chatglm.py` & `openllm_core-0.5.2/src/openllm_core/config/configuration_chatglm.py`

 * *Files identical despite different names*

### Comparing `openllm_core-0.5.1/src/openllm_core/config/configuration_dbrx.py` & `openllm_core-0.5.2/src/openllm_core/config/configuration_dbrx.py`

 * *Files identical despite different names*

### Comparing `openllm_core-0.5.1/src/openllm_core/config/configuration_dolly_v2.py` & `openllm_core-0.5.2/src/openllm_core/config/configuration_dolly_v2.py`

 * *Files identical despite different names*

### Comparing `openllm_core-0.5.1/src/openllm_core/config/configuration_falcon.py` & `openllm_core-0.5.2/src/openllm_core/config/configuration_falcon.py`

 * *Files identical despite different names*

### Comparing `openllm_core-0.5.1/src/openllm_core/config/configuration_gemma.py` & `openllm_core-0.5.2/src/openllm_core/config/configuration_gemma.py`

 * *Files identical despite different names*

### Comparing `openllm_core-0.5.1/src/openllm_core/config/configuration_gpt_neox.py` & `openllm_core-0.5.2/src/openllm_core/config/configuration_gpt_neox.py`

 * *Files identical despite different names*

### Comparing `openllm_core-0.5.1/src/openllm_core/config/configuration_llama.py` & `openllm_core-0.5.2/src/openllm_core/config/configuration_llama.py`

 * *Files identical despite different names*

### Comparing `openllm_core-0.5.1/src/openllm_core/config/configuration_mistral.py` & `openllm_core-0.5.2/src/openllm_core/config/configuration_mistral.py`

 * *Files identical despite different names*

### Comparing `openllm_core-0.5.1/src/openllm_core/config/configuration_mixtral.py` & `openllm_core-0.5.2/src/openllm_core/config/configuration_mixtral.py`

 * *Files identical despite different names*

### Comparing `openllm_core-0.5.1/src/openllm_core/config/configuration_mpt.py` & `openllm_core-0.5.2/src/openllm_core/config/configuration_mpt.py`

 * *Files identical despite different names*

### Comparing `openllm_core-0.5.1/src/openllm_core/config/configuration_opt.py` & `openllm_core-0.5.2/src/openllm_core/config/configuration_opt.py`

 * *Files identical despite different names*

### Comparing `openllm_core-0.5.1/src/openllm_core/config/configuration_phi.py` & `openllm_core-0.5.2/src/openllm_core/config/configuration_phi.py`

 * *Files identical despite different names*

### Comparing `openllm_core-0.5.1/src/openllm_core/config/configuration_qwen.py` & `openllm_core-0.5.2/src/openllm_core/config/configuration_qwen.py`

 * *Files identical despite different names*

### Comparing `openllm_core-0.5.1/src/openllm_core/config/configuration_stablelm.py` & `openllm_core-0.5.2/src/openllm_core/config/configuration_stablelm.py`

 * *Files identical despite different names*

### Comparing `openllm_core-0.5.1/src/openllm_core/config/configuration_starcoder.py` & `openllm_core-0.5.2/src/openllm_core/config/configuration_starcoder.py`

 * *Files identical despite different names*

### Comparing `openllm_core-0.5.1/src/openllm_core/config/configuration_yi.py` & `openllm_core-0.5.2/src/openllm_core/config/configuration_yi.py`

 * *Files identical despite different names*

### Comparing `openllm_core-0.5.1/src/openllm_core/protocol/openai.py` & `openllm_core-0.5.2/src/openllm_core/protocol/openai.py`

 * *Files identical despite different names*

### Comparing `openllm_core-0.5.1/src/openllm_core/utils/__init__.py` & `openllm_core-0.5.2/src/openllm_core/utils/__init__.py`

 * *Files identical despite different names*

### Comparing `openllm_core-0.5.1/src/openllm_core/utils/__init__.pyi` & `openllm_core-0.5.2/src/openllm_core/utils/__init__.pyi`

 * *Files identical despite different names*

### Comparing `openllm_core-0.5.1/src/openllm_core/utils/_constants.py` & `openllm_core-0.5.2/src/openllm_core/utils/_constants.py`

 * *Files identical despite different names*

### Comparing `openllm_core-0.5.1/src/openllm_core/utils/analytics.py` & `openllm_core-0.5.2/src/openllm_core/utils/analytics.py`

 * *Files identical despite different names*

### Comparing `openllm_core-0.5.1/src/openllm_core/utils/codegen.py` & `openllm_core-0.5.2/src/openllm_core/utils/codegen.py`

 * *Files identical despite different names*

### Comparing `openllm_core-0.5.1/src/openllm_core/utils/dantic.py` & `openllm_core-0.5.2/src/openllm_core/utils/dantic.py`

 * *Files identical despite different names*

### Comparing `openllm_core-0.5.1/src/openllm_core/utils/import_utils.py` & `openllm_core-0.5.2/src/openllm_core/utils/import_utils.py`

 * *Files identical despite different names*

### Comparing `openllm_core-0.5.1/src/openllm_core/utils/import_utils.pyi` & `openllm_core-0.5.2/src/openllm_core/utils/import_utils.pyi`

 * *Files identical despite different names*

### Comparing `openllm_core-0.5.1/src/openllm_core/utils/lazy.py` & `openllm_core-0.5.2/src/openllm_core/utils/lazy.py`

 * *Files identical despite different names*

### Comparing `openllm_core-0.5.1/src/openllm_core/utils/peft.py` & `openllm_core-0.5.2/src/openllm_core/utils/peft.py`

 * *Files identical despite different names*

### Comparing `openllm_core-0.5.1/src/openllm_core/utils/pkg.py` & `openllm_core-0.5.2/src/openllm_core/utils/pkg.py`

 * *Files identical despite different names*

### Comparing `openllm_core-0.5.1/src/openllm_core/utils/representation.py` & `openllm_core-0.5.2/src/openllm_core/utils/representation.py`

 * *Files identical despite different names*

### Comparing `openllm_core-0.5.1/src/openllm_core/utils/serde.py` & `openllm_core-0.5.2/src/openllm_core/utils/serde.py`

 * *Files identical despite different names*

### Comparing `openllm_core-0.5.1/.gitignore` & `openllm_core-0.5.2/.gitignore`

 * *Files identical despite different names*

### Comparing `openllm_core-0.5.1/LICENSE.md` & `openllm_core-0.5.2/LICENSE.md`

 * *Files identical despite different names*

### Comparing `openllm_core-0.5.1/pyproject.toml` & `openllm_core-0.5.2/pyproject.toml`

 * *Files identical despite different names*

### Comparing `openllm_core-0.5.1/PKG-INFO` & `openllm_core-0.5.2/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: openllm-core
-Version: 0.5.1
+Version: 0.5.2
 Summary: OpenLLM Core: Core components for OpenLLM.
 Project-URL: Blog, https://modelserving.com
 Project-URL: Chat, https://l.bentoml.com/join-openllm-discord
 Project-URL: Documentation, https://github.com/bentoml/OpenLLM/blob/main/openllm-core/README.md
 Project-URL: GitHub, https://github.com/bentoml/OpenLLM/blob/main/openllm-core
 Project-URL: History, https://github.com/bentoml/OpenLLM/blob/main/CHANGELOG.md
 Project-URL: Homepage, https://bentoml.com
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: openllm-core Version: 0.5.1 Summary: OpenLLM Core:
+Metadata-Version: 2.1 Name: openllm-core Version: 0.5.2 Summary: OpenLLM Core:
 Core components for OpenLLM. Project-URL: Blog, https://modelserving.com
 Project-URL: Chat, https://l.bentoml.com/join-openllm-discord Project-URL:
 Documentation, https://github.com/bentoml/OpenLLM/blob/main/openllm-core/
 README.md Project-URL: GitHub, https://github.com/bentoml/OpenLLM/blob/main/
 openllm-core Project-URL: History, https://github.com/bentoml/OpenLLM/blob/
 main/CHANGELOG.md Project-URL: Homepage, https://bentoml.com Project-URL:
 Tracker, https://github.com/bentoml/OpenLLM/issues Project-URL: Twitter, https:
```

