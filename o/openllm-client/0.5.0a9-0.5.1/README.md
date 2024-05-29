# Comparing `tmp/openllm_client-0.5.0a9.tar.gz` & `tmp/openllm_client-0.5.1.tar.gz`

## Comparing `openllm_client-0.5.0a9.tar` & `openllm_client-0.5.1.tar`

### file list

```diff
@@ -1,17 +1,15 @@
--rw-r--r--   0        0        0     4280 2020-02-02 00:00:00.000000 openllm_client-0.5.0a9/README.md
--rw-r--r--   0        0        0     9489 2020-02-02 00:00:00.000000 openllm_client-0.5.0a9/protos/service.proto
--rw-r--r--   0        0        0       80 2020-02-02 00:00:00.000000 openllm_client-0.5.0a9/src/openllm_client/__init__.py
--rw-r--r--   0        0        0     3735 2020-02-02 00:00:00.000000 openllm_client-0.5.0a9/src/openllm_client/__init__.pyi
--rw-r--r--   0        0        0     8016 2020-02-02 00:00:00.000000 openllm_client-0.5.0a9/src/openllm_client/_http.py
--rw-r--r--   0        0        0     3168 2020-02-02 00:00:00.000000 openllm_client-0.5.0a9/src/openllm_client/_schemas.py
--rw-r--r--   0        0        0    19482 2020-02-02 00:00:00.000000 openllm_client-0.5.0a9/src/openllm_client/_shim.py
--rw-r--r--   0        0        0     4196 2020-02-02 00:00:00.000000 openllm_client-0.5.0a9/src/openllm_client/_stream.py
--rw-r--r--   0        0        0      541 2020-02-02 00:00:00.000000 openllm_client-0.5.0a9/src/openllm_client/_typing_compat.py
--rw-r--r--   0        0        0      367 2020-02-02 00:00:00.000000 openllm_client-0.5.0a9/src/openllm_client/_utils.py
--rw-r--r--   0        0        0     2079 2020-02-02 00:00:00.000000 openllm_client-0.5.0a9/src/openllm_client/_utils.pyi
--rw-r--r--   0        0        0      413 2020-02-02 00:00:00.000000 openllm_client-0.5.0a9/src/openllm_client/_version.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 openllm_client-0.5.0a9/src/openllm_client/py.typed
--rw-r--r--   0        0        0     2087 2020-02-02 00:00:00.000000 openllm_client-0.5.0a9/.gitignore
--rw-r--r--   0        0        0    10470 2020-02-02 00:00:00.000000 openllm_client-0.5.0a9/LICENSE.md
--rw-r--r--   0        0        0     4476 2020-02-02 00:00:00.000000 openllm_client-0.5.0a9/pyproject.toml
--rw-r--r--   0        0        0     7091 2020-02-02 00:00:00.000000 openllm_client-0.5.0a9/PKG-INFO
+-rw-r--r--   0        0        0     3732 2020-02-02 00:00:00.000000 openllm_client-0.5.1/README.md
+-rw-r--r--   0        0        0     9489 2020-02-02 00:00:00.000000 openllm_client-0.5.1/protos/service.proto
+-rw-r--r--   0        0        0       80 2020-02-02 00:00:00.000000 openllm_client-0.5.1/src/openllm_client/__init__.py
+-rw-r--r--   0        0        0     3735 2020-02-02 00:00:00.000000 openllm_client-0.5.1/src/openllm_client/__init__.pyi
+-rw-r--r--   0        0        0     8676 2020-02-02 00:00:00.000000 openllm_client-0.5.1/src/openllm_client/_http.py
+-rw-r--r--   0        0        0     2051 2020-02-02 00:00:00.000000 openllm_client-0.5.1/src/openllm_client/_schemas.py
+-rw-r--r--   0        0        0    19458 2020-02-02 00:00:00.000000 openllm_client-0.5.1/src/openllm_client/_shim.py
+-rw-r--r--   0        0        0     4149 2020-02-02 00:00:00.000000 openllm_client-0.5.1/src/openllm_client/_stream.py
+-rw-r--r--   0        0        0      567 2020-02-02 00:00:00.000000 openllm_client-0.5.1/src/openllm_client/_typing_compat.py
+-rw-r--r--   0        0        0      411 2020-02-02 00:00:00.000000 openllm_client-0.5.1/src/openllm_client/_version.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 openllm_client-0.5.1/src/openllm_client/py.typed
+-rw-r--r--   0        0        0     2087 2020-02-02 00:00:00.000000 openllm_client-0.5.1/.gitignore
+-rw-r--r--   0        0        0    10470 2020-02-02 00:00:00.000000 openllm_client-0.5.1/LICENSE.md
+-rw-r--r--   0        0        0     4459 2020-02-02 00:00:00.000000 openllm_client-0.5.1/pyproject.toml
+-rw-r--r--   0        0        0     6512 2020-02-02 00:00:00.000000 openllm_client-0.5.1/PKG-INFO
```

### Comparing `openllm_client-0.5.0a9/README.md` & `openllm_client-0.5.1/README.md`

 * *Files 10% similar despite different names*

```diff
@@ -40,23 +40,14 @@
 deploy to the cloud or on-premises, and build powerful AI apps, and more.
 
 To learn more about OpenLLM, please visit <a href="https://github.com/bentoml/OpenLLM">OpenLLM's README.md</a>
 
 This package holds the underlying client implementation for OpenLLM. If you are
 coming from OpenLLM, the client can be accessed via `openllm.client`.
 
-It provides somewhat of a "similar" APIs to [`bentoml.Client`](https://docs.bentoml.com/en/latest/guides/client.html)
-(via `openllm_client.min`) for interacting with OpenLLM server. This can also be extended to use with general
-BentoML server as well.
-
-> [!NOTE]
-> The component of interop with generic BentoML server will be considered as _EXPERIMENTAL_ and
-> will be refactored to new client implementation soon!
-> If you are just using this package for interacting with OpenLLM server, The API should be the same as `openllm.client` namespace.
-
 ```python
 import openllm
 
 client = openllm.client.HTTPClient()
 
 client.query('Explain to me the difference between "further" and "farther"')
 ```
```

#### html2text {}

```diff
@@ -5,24 +5,16 @@
    OpenLLM Client: Interacting with OpenLLM HTTP/gRPC server, or any BentoML
                                     server.
 ## ð Introduction With OpenLLM, you can run inference with any open-source
 large-language models, deploy to the cloud or on-premises, and build powerful
 AI apps, and more. To learn more about OpenLLM, please visit _O_p_e_n_L_L_M_'_s
 _R_E_A_D_M_E_._m_d This package holds the underlying client implementation for OpenLLM.
 If you are coming from OpenLLM, the client can be accessed via
-`openllm.client`. It provides somewhat of a "similar" APIs to
-[`bentoml.Client`](https://docs.bentoml.com/en/latest/guides/client.html) (via
-`openllm_client.min`) for interacting with OpenLLM server. This can also be
-extended to use with general BentoML server as well. > [!NOTE] > The component
-of interop with generic BentoML server will be considered as _EXPERIMENTAL_ and
-> will be refactored to new client implementation soon! > If you are just using
-this package for interacting with OpenLLM server, The API should be the same as
-`openllm.client` namespace. ```python import openllm client =
-openllm.client.HTTPClient() client.query('Explain to me the difference between
-"further" and "farther"') ``` ![Gif showing OpenLLM Intro](/.github/assets/
-output.gif)
+`openllm.client`. ```python import openllm client = openllm.client.HTTPClient()
+client.query('Explain to me the difference between "further" and "farther"')
+``` ![Gif showing OpenLLM Intro](/.github/assets/output.gif)
 ## ð Citation If you use OpenLLM in your research, we provide a [citation]
 (../CITATION.cff) to use: ```bibtex @software{Pham_OpenLLM_Operating_LLMs_2023,
 author = {Pham, Aaron and Yang, Chaoyu and Sheng, Sean and Zhao, Shenyang and
 Lee, Sauyon and Jiang, Bo and Dong, Fog and Guan, Xipeng and Ming, Frost},
 license = {Apache-2.0}, month = jun, title = {{OpenLLM: Operating LLMs in
 production}}, url = {https://github.com/bentoml/OpenLLM}, year = {2023} } ```
```

### Comparing `openllm_client-0.5.0a9/protos/service.proto` & `openllm_client-0.5.1/protos/service.proto`

 * *Files identical despite different names*

### Comparing `openllm_client-0.5.0a9/src/openllm_client/__init__.pyi` & `openllm_client-0.5.1/src/openllm_client/__init__.pyi`

 * *Files identical despite different names*

### Comparing `openllm_client-0.5.0a9/src/openllm_client/_http.py` & `openllm_client-0.5.1/src/openllm_client/_http.py`

 * *Files 9% similar despite different names*

```diff
@@ -1,49 +1,48 @@
 from __future__ import annotations
-import importlib.metadata
-import logging
-import os
-import typing as t
 
-import attr
+import importlib.metadata, logging, os, typing as t, orjson, pydantic
 
 from ._schemas import Helpers, Metadata, Response, StreamingResponse
 from ._shim import MAX_RETRIES, AsyncClient, Client
 
 logger = logging.getLogger(__name__)
 
 VERSION = importlib.metadata.version('openllm-client')
 
 
 def _address_converter(addr: str):
   return addr if '://' in addr else 'http://' + addr
 
 
-@attr.define(init=False)
 class HTTPClient(Client):
-  helpers: Helpers = attr.field(init=False)
-  _api_version: str = 'v1'
-  _verify: bool = True
-  __metadata: Metadata | None = None
-  __config: dict[str, t.Any] | None = None
+  _helpers: Helpers = pydantic.PrivateAttr()
+  _api_version: str = pydantic.PrivateAttr(default='v1')
+  _verify: bool = pydantic.PrivateAttr(default=True)
+  __metadata: t.Optional[Metadata] = None
+  __config: t.Optional[t.Dict[str, t.Any]] = None
 
   def __repr__(self):
-    return f'<HTTPClient address={self.address} timeout={self._timeout} api_version={self._api_version} verify={self._verify}>'
+    return f'<HTTPClient address={self.address} timeout={self.timeout} api_version={self._api_version} verify={self._verify}>'
 
   def __init__(self, address=None, timeout=30, verify=False, max_retries=MAX_RETRIES, api_version='v1'):
     if address is None:
       address = os.getenv('OPENLLM_ENDPOINT')
       if address is None:
         raise ValueError("address must either be provided or through 'OPENLLM_ENDPOINT'")
-    self._api_version, self._verify = api_version, verify
-
-    self.helpers = Helpers(client=self)
 
     super().__init__(_address_converter(address), VERSION, timeout=timeout, max_retries=max_retries)
 
+    self._helpers = Helpers(client=self)
+    self._api_version, self._verify = api_version, verify
+
+  @property
+  def helpers(self):
+    return self._helpers
+
   def _build_auth_headers(self) -> t.Dict[str, str]:
     env = os.getenv('OPENLLM_AUTH_TOKEN')
     if env is not None:
       return {'Authorization': f'Bearer {env}'}
     return super()._build_auth_headers()
 
   def __getitem__(self, item):
@@ -53,172 +52,199 @@
       return self._config[item]
     raise KeyError(f'No attributes: {item}')
 
   @property
   def _metadata(self):
     if self.__metadata is None:
       path = f'/{self._api_version}/metadata'
-      self.__metadata = self._post(path, response_cls=Metadata, json={}, options={'max_retries': self._max_retries})
+      self.__metadata = self._post(path, response_cls=Metadata, json={}, options={'max_retries': self.max_retries})
     return self.__metadata
 
   @property
   def _config(self) -> dict[str, t.Any]:
     if self.__config is None:
-      self.__config = self._metadata.configuration
+      self.__config = orjson.loads(self._metadata.configuration)
     return self.__config
 
   def query(self, prompt, **attrs):
     return self.generate(prompt, **attrs)
 
   def health(self):
     response = self._get(
-      '/readyz', response_cls=None, options={'return_raw_response': True, 'max_retries': self._max_retries}
+      '/readyz', response_cls=None, options={'return_raw_response': True, 'max_retries': self.max_retries}
     )
     return response.status_code == 200
 
   def generate(
     self, prompt, llm_config=None, stop=None, adapter_name=None, timeout=None, verify=None, **attrs
   ) -> Response:
     if timeout is None:
-      timeout = self._timeout
+      timeout = self.timeout
     if verify is None:
       verify = self._verify  # XXX: need to support this again
     if llm_config is not None:
       llm_config = {**self._config, **llm_config, **attrs}
     else:
       llm_config = {**self._config, **attrs}
 
+    if stop is not None:
+      if isinstance(stop, str):
+        stop = [stop]
+      else:
+        stop = list(stop)
+
     return self._post(
       f'/{self._api_version}/generate',
       response_cls=Response,
       json=dict(prompt=prompt, llm_config=llm_config, stop=stop, adapter_name=adapter_name),
-      options={'max_retries': self._max_retries},
+      options={'max_retries': self.max_retries},
     )
 
   def generate_stream(
     self, prompt, llm_config=None, stop=None, adapter_name=None, timeout=None, verify=None, **attrs
   ) -> t.Iterator[StreamingResponse]:
     for response_chunk in self.generate_iterator(prompt, llm_config, stop, adapter_name, timeout, verify, **attrs):
       yield StreamingResponse.from_response_chunk(response_chunk)
 
   def generate_iterator(
     self, prompt, llm_config=None, stop=None, adapter_name=None, timeout=None, verify=None, **attrs
   ) -> t.Iterator[Response]:
     if timeout is None:
-      timeout = self._timeout
+      timeout = self.timeout
     if verify is None:
       verify = self._verify  # XXX: need to support this again
     if llm_config is not None:
       llm_config = {**self._config, **llm_config, **attrs}
     else:
       llm_config = {**self._config, **attrs}
+
+    if stop is not None:
+      if isinstance(stop, str):
+        stop = [stop]
+      else:
+        stop = list(stop)
+
     return self._post(
       f'/{self._api_version}/generate_stream',
       response_cls=Response,
       json=dict(prompt=prompt, llm_config=llm_config, stop=stop, adapter_name=adapter_name),
-      options={'max_retries': self._max_retries},
+      options={'max_retries': self.max_retries},
       stream=True,
     )
 
 
-@attr.define(init=False)
-class AsyncHTTPClient(AsyncClient):
-  helpers: Helpers = attr.field(init=False)
-  _api_version: str = 'v1'
-  _verify: bool = True
-  __metadata: Metadata | None = None
-  __config: dict[str, t.Any] | None = None
+class AsyncHTTPClient(AsyncClient, pydantic.BaseModel):
+  _helpers: Helpers = pydantic.PrivateAttr()
+  _api_version: str = pydantic.PrivateAttr(default='v1')
+  _verify: bool = pydantic.PrivateAttr(default=True)
+  __metadata: t.Optional[Metadata] = None
+  __config: t.Optional[t.Dict[str, t.Any]] = None
 
   def __repr__(self):
-    return f'<AsyncHTTPClient address={self.address} timeout={self._timeout} api_version={self._api_version} verify={self._verify}>'
+    return f'<AsyncHTTPClient address={self.address} timeout={self.timeout} api_version={self._api_version} verify={self._verify}>'
 
   def __init__(self, address=None, timeout=30, verify=False, max_retries=MAX_RETRIES, api_version='v1'):
     if address is None:
       address = os.getenv('OPENLLM_ENDPOINT')
       if address is None:
         raise ValueError("address must either be provided or through 'OPENLLM_ENDPOINT'")
-    self._api_version, self._verify = api_version, verify
+
+    super().__init__(_address_converter(address), VERSION, timeout=timeout, max_retries=max_retries)
 
     # mk messages to be async here
-    self.helpers = Helpers.permute(messages=Helpers.async_messages)(async_client=self)
+    self._helpers = Helpers.permute(messages=Helpers.async_messages)(async_client=self)
+    self._api_version, self._verify = api_version, verify
 
-    super().__init__(_address_converter(address), VERSION, timeout=timeout, max_retries=max_retries)
+  @property
+  def helpers(self):
+    return self._helpers
 
   def _build_auth_headers(self) -> t.Dict[str, str]:
     env = os.getenv('OPENLLM_AUTH_TOKEN')
     if env is not None:
       return {'Authorization': f'Bearer {env}'}
     return super()._build_auth_headers()
 
   @property
   async def _metadata(self) -> t.Awaitable[Metadata]:
     if self.__metadata is None:
       self.__metadata = await self._post(
-        f'/{self._api_version}/metadata', response_cls=Metadata, json={}, options={'max_retries': self._max_retries}
+        f'/{self._api_version}/metadata', response_cls=Metadata, json={}, options={'max_retries': self.max_retries}
       )
     return self.__metadata
 
   @property
   async def _config(self):
     if self.__config is None:
-      self.__config = (await self._metadata).configuration
+      self.__config = orjson.loads((await self._metadata).configuration)
     return self.__config
 
   async def query(self, prompt, **attrs):
     return await self.generate(prompt, **attrs)
 
   async def health(self):
     response = await self._get(
-      '/readyz', response_cls=None, options={'return_raw_response': True, 'max_retries': self._max_retries}
+      '/readyz', response_cls=None, options={'return_raw_response': True, 'max_retries': self.max_retries}
     )
     return response.status_code == 200
 
   async def generate(
     self, prompt, llm_config=None, stop=None, adapter_name=None, timeout=None, verify=None, **attrs
   ) -> Response:
     if timeout is None:
-      timeout = self._timeout
+      timeout = self.timeout
     if verify is None:
       verify = self._verify  # XXX: need to support this again
-    _metadata = await self._metadata
     _config = await self._config
     if llm_config is not None:
       llm_config = {**_config, **llm_config, **attrs}
     else:
       llm_config = {**_config, **attrs}
+
+    if stop is not None:
+      if isinstance(stop, str):
+        stop = [stop]
+      else:
+        stop = list(stop)
+
     return await self._post(
       f'/{self._api_version}/generate',
       response_cls=Response,
       json=dict(prompt=prompt, llm_config=llm_config, stop=stop, adapter_name=adapter_name),
-      options={'max_retries': self._max_retries},
+      options={'max_retries': self.max_retries},
     )
 
   async def generate_stream(
-    self, prompt, llm_config=None, stop=None, adapter_name=None, timeout=None, verify=None, **attrs
+    self, prompt, llm_config=None, stop=None, adapter_name=None, timeout=None, verify=None, index=0, **attrs
   ) -> t.AsyncGenerator[StreamingResponse, t.Any]:
     async for response_chunk in self.generate_iterator(
       prompt, llm_config, stop, adapter_name, timeout, verify, **attrs
     ):
-      yield StreamingResponse.from_response_chunk(response_chunk)
+      yield StreamingResponse.from_response_chunk(response_chunk, index=index)
 
   async def generate_iterator(
     self, prompt, llm_config=None, stop=None, adapter_name=None, timeout=None, verify=None, **attrs
   ) -> t.AsyncGenerator[Response, t.Any]:
     if timeout is None:
-      timeout = self._timeout
+      timeout = self.timeout
     if verify is None:
       verify = self._verify  # XXX: need to support this again
-    _metadata = await self._metadata
     _config = await self._config
     if llm_config is not None:
       llm_config = {**_config, **llm_config, **attrs}
     else:
       llm_config = {**_config, **attrs}
 
+    if stop is not None:
+      if isinstance(stop, str):
+        stop = [stop]
+      else:
+        stop = list(stop)
+
     async for response_chunk in await self._post(
       f'/{self._api_version}/generate_stream',
       response_cls=Response,
       json=dict(prompt=prompt, llm_config=llm_config, stop=stop, adapter_name=adapter_name),
-      options={'max_retries': self._max_retries},
+      options={'max_retries': self.max_retries},
       stream=True,
     ):
       yield response_chunk
```

### Comparing `openllm_client-0.5.0a9/src/openllm_client/_schemas.py` & `openllm_client-0.5.1/src/openllm_client/_schemas.py`

 * *Files 22% similar despite different names*

```diff
@@ -1,88 +1,47 @@
 from __future__ import annotations
-import types
-import typing as t
 
-import attr
-import orjson
+import types, pydantic, typing as t
 
 from openllm_core._schemas import (
   CompletionChunk as CompletionChunk,
-  GenerationOutput as Response,  # backward compatibility
-  _SchemaMixin as _SchemaMixin,
+  MetadataOutput as Metadata,
+  GenerationOutput as Response,
 )
-
-from ._utils import converter
+from ._typing_compat import TypedDict
 
 if t.TYPE_CHECKING:
   from ._shim import AsyncClient, Client
 
 
 __all__ = ['CompletionChunk', 'Helpers', 'Metadata', 'Response', 'StreamingResponse']
 
 
-@attr.define
-class Metadata(_SchemaMixin):
-  """NOTE: Metadata is a modified version of the original MetadataOutput from openllm-core.
-
-  The configuration is now structured into a dictionary for easy of use."""
-
-  model_id: str
-  timeout: int
-  model_name: str
-  backend: str
-  configuration: t.Dict[str, t.Any]
-
-
-def _structure_metadata(data: t.Dict[str, t.Any], cls: type[Metadata]) -> Metadata:
-  try:
-    configuration = orjson.loads(data['configuration'])
-    generation_config = configuration.pop('generation_config')
-    configuration = {**configuration, **generation_config}
-  except orjson.JSONDecodeError as e:
-    raise RuntimeError(f'Malformed metadata configuration (Server-side issue): {e}') from None
-  try:
-    return cls(
-      model_id=data['model_id'],
-      timeout=data['timeout'],
-      model_name=data['model_name'],
-      backend=data['backend'],
-      configuration=configuration,
-    )
-  except Exception as e:
-    raise RuntimeError(f'Malformed metadata (Server-side issue): {e}') from None
-
-
-converter.register_structure_hook(Metadata, _structure_metadata)
-
-
-@attr.define
-class StreamingResponse(_SchemaMixin):
+class StreamingResponse(pydantic.BaseModel):
   request_id: str
   index: int
   text: str
   token_ids: int
 
   @classmethod
-  def from_response_chunk(cls, response: Response) -> StreamingResponse:
+  def from_response_chunk(cls, response: Response, index: int = 0) -> StreamingResponse:
     return cls(
       request_id=response.request_id,
-      index=response.outputs[0].index,
-      text=response.outputs[0].text,
-      token_ids=response.outputs[0].token_ids[0],
+      index=response.outputs[index].index,
+      text=response.outputs[index].text,
+      token_ids=response.outputs[index].token_ids[0],
     )
 
 
-class MesssageParam(t.TypedDict):
+class MesssageParam(TypedDict):
   role: t.Literal['user', 'system', 'assistant']
   content: str
 
 
-@attr.define(repr=False)
-class Helpers:
+class Helpers(pydantic.BaseModel):
   _client: t.Optional[Client] = None
   _async_client: t.Optional[AsyncClient] = None
 
   @property
   def client(self):
     if self._client is None:
       raise RuntimeError('Sync client should not be used within a async context.')
```

### Comparing `openllm_client-0.5.0a9/src/openllm_client/_shim.py` & `openllm_client-0.5.1/src/openllm_client/_shim.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,26 +1,15 @@
 # This provides a base shim with httpx and acts as base request
 from __future__ import annotations
 
-import asyncio
-import email.utils
-import logging
-import platform
-import random
-import time
-import typing as t
-
-import anyio
-import attr
-import distro
-import httpx
+import asyncio, logging, platform, random, time, typing as t
+import email.utils, anyio, distro, httpx, pydantic
 
-from ._stream import AsyncStream, Response, Stream
+from ._stream import AsyncStream, Stream, Response
 from ._typing_compat import Annotated, Architecture, LiteralString, Platform
-from ._utils import converter
 
 logger = logging.getLogger(__name__)
 
 InnerClient = t.TypeVar('InnerClient', bound=t.Union[httpx.Client, httpx.AsyncClient])
 StreamType = t.TypeVar('StreamType', bound=t.Union[Stream[t.Any], AsyncStream[t.Any]])
 _Stream = t.TypeVar('_Stream', bound=Stream[t.Any])
 _AsyncStream = t.TypeVar('_AsyncStream', bound=AsyncStream[t.Any])
@@ -88,135 +77,138 @@
     return 'x86'
   elif machine:
     return f'Other:{machine}'
   return 'Unknown'
 
 
 @t.final
-@attr.frozen(auto_attribs=True)
-class RequestOptions:
-  method: str = attr.field(converter=str.lower)
+class RequestOptions(pydantic.BaseModel):
+  model_config = pydantic.ConfigDict(extra='forbid', protected_namespaces=())
+
+  method: pydantic.constr(to_lower=True)
   url: str
-  json: t.Optional[t.Dict[str, t.Any]] = attr.field(default=None)
-  params: t.Optional[t.Mapping[str, t.Any]] = attr.field(default=None)
-  headers: t.Optional[t.Dict[str, str]] = attr.field(default=None)
-  max_retries: int = attr.field(default=MAX_RETRIES)
-  return_raw_response: bool = attr.field(default=False)
+  json: t.Optional[t.Dict[str, t.Any]] = pydantic.Field(default=None)
+  params: t.Optional[t.Mapping[str, t.Any]] = pydantic.Field(default=None)
+  headers: t.Optional[t.Dict[str, str]] = pydantic.Field(default=None)
+  max_retries: int = pydantic.Field(default=MAX_RETRIES)
+  return_raw_response: bool = pydantic.Field(default=False)
 
   def get_max_retries(self, max_retries: int | None) -> int:
     return max_retries if max_retries is not None else self.max_retries
 
   @classmethod
   def model_construct(cls, **options: t.Any) -> RequestOptions:
     return cls(**options)
 
 
 @t.final
-@attr.frozen(auto_attribs=True)
-class APIResponse(t.Generic[Response]):
-  _raw_response: httpx.Response
-  _client: BaseClient[t.Any, t.Any]
-  _response_cls: type[Response]
-  _stream: bool
-  _stream_cls: t.Optional[t.Union[t.Type[Stream[t.Any]], t.Type[AsyncStream[t.Any]]]]
-  _options: RequestOptions
+class APIResponse(pydantic.BaseModel, t.Generic[Response]):
+  model_config = pydantic.ConfigDict(arbitrary_types_allowed=True)
 
-  _parsed: t.Optional[Response] = attr.field(default=None, repr=False)
+  raw_response: httpx.Response
+  client: t.Union[AsyncClient, Client]
+  response_cls: t.Optional[type[Response]]
+  stream: bool
+  stream_cls: t.Optional[t.Union[t.Type[Stream[t.Any]], t.Type[AsyncStream[t.Any]]]]
+  options: RequestOptions
+  _parsed: t.Optional[Response] = pydantic.PrivateAttr(default=None)
 
   def parse(self):
-    if self._options.return_raw_response:
-      return self._raw_response
+    if self.options.return_raw_response:
+      return self.raw_response
+
+    if self.response_cls is None:
+      raise ValueError('Response class cannot be None.')
+
     if self._parsed is not None:
       return self._parsed
-    if self._stream:
-      stream_cls = self._stream_cls or self._client._default_stream_cls
-      return stream_cls(response_cls=self._response_cls, response=self._raw_response, client=self._client)
 
-    if self._response_cls is str:
-      return self._raw_response.text
+    if self.stream:
+      stream_cls = self.stream_cls or self.client.default_stream_cls
+      return stream_cls(response_cls=self.response_cls, response=self.raw_response, client=self.client)
 
-    content_type, *_ = self._raw_response.headers.get('content-type', '').split(';')
+    if self.response_cls is str:
+      return self.raw_response.text
+
+    content_type, *_ = self.raw_response.headers.get('content-type', '').split(';')
     if content_type != 'application/json':
       # Since users specific different content_type, then we return the raw binary text without and deserialisation
-      return self._raw_response.text
+      return self.raw_response.text
 
-    data = self._raw_response.json()
+    data = self.raw_response.json()
     try:
-      return self._client._process_response_data(
-        data=data, response_cls=self._response_cls, raw_response=self._raw_response
+      return self.client._process_response_data(
+        data=data, response_cls=self.response_cls, raw_response=self.raw_response
       )
     except Exception as exc:
       raise ValueError(exc) from None  # validation error here
 
   @property
   def headers(self):
-    return self._raw_response.headers
+    return self.raw_response.headers
 
   @property
   def status_code(self):
-    return self._raw_response.status_code
+    return self.raw_response.status_code
 
   @property
   def request(self):
-    return self._raw_response.request
+    return self.raw_response.request
 
   @property
   def url(self):
-    return self._raw_response.url
+    return self.raw_response.url
 
   @property
   def content(self):
-    return self._raw_response.content
+    return self.raw_response.content
 
   @property
   def text(self):
-    return self._raw_response.text
+    return self.raw_response.text
 
   @property
   def http_version(self):
-    return self._raw_response.http_version
+    return self.raw_response.http_version
 
 
-@attr.define(init=False)
-class BaseClient(t.Generic[InnerClient, StreamType]):
-  _base_url: httpx.URL = attr.field(converter=_address_converter)
-  _version: LiteralVersion
-  _timeout: httpx.Timeout = attr.field(converter=httpx.Timeout)
-  _max_retries: int
-  _inner: InnerClient
-  _default_stream_cls: t.Type[StreamType]
-  _auth_headers: t.Dict[str, str] = attr.field(init=False)
+class BaseClient(pydantic.BaseModel, t.Generic[InnerClient, StreamType]):
+  model_config = pydantic.ConfigDict(arbitrary_types_allowed=True)
 
-  def __init__(
-    self,
-    *,
-    base_url: str | httpx.URL,
-    version: str,
-    timeout: int | httpx.Timeout = DEFAULT_TIMEOUT,
-    max_retries: int = MAX_RETRIES,
-    client: InnerClient,
-    _default_stream_cls: t.Type[StreamType],
-    _internal: bool = False,
-  ):
-    if not _internal:
-      raise RuntimeError('Client is reserved to be used internally only.')
-    self.__attrs_init__(base_url, version, timeout, max_retries, client, _default_stream_cls)
+  _base_url: httpx.URL = pydantic.PrivateAttr()
+  version: pydantic.SkipValidation[LiteralVersion]
+  timeout: httpx.Timeout
+  max_retries: int
+  inner: InnerClient
+  default_stream_cls: pydantic.SkipValidation[t.Type[StreamType]]
+  _auth_headers: t.Dict[str, str] = pydantic.PrivateAttr()
+
+  @pydantic.field_validator('timeout', mode='before')
+  @classmethod
+  def convert_timeout(cls, value: t.Any) -> httpx.Timeout:
+    return httpx.Timeout(value)
+
+  def __init__(self, base_url: str, **data: t.Any):
+    super().__init__(**data)
+    self._base_url = _address_converter(base_url)
+
+  def model_post_init(self, *_: t.Any):
     self._auth_headers = self._build_auth_headers()
 
   def _prepare_url(self, url: str) -> httpx.URL:
     # copied from httpx._merge_url
     merge_url = httpx.URL(url)
     if merge_url.is_relative_url:
       merge_raw = self._base_url.raw_path + merge_url.raw_path.lstrip(b'/')
       return self._base_url.copy_with(raw_path=merge_raw)
     return merge_url
 
   @property
   def is_closed(self):
-    return self._inner.is_closed
+    return self.inner.is_closed
 
   @property
   def is_ready(self):
     return not self.is_closed  # backward compat
 
   @property
   def base_url(self):
@@ -235,15 +227,15 @@
 
   @property
   def auth(self) -> httpx.Auth | None:
     return None
 
   @property
   def user_agent(self):
-    return f'{self.__class__.__name__}/Python {self._version}'
+    return f'{self.__class__.__name__}/Python {self.version}'
 
   @property
   def auth_headers(self):
     return self._auth_headers
 
   @property
   def _default_headers(self) -> t.Dict[str, str]:
@@ -254,41 +246,41 @@
       **self.platform_headers,
       **self.auth_headers,
     }
 
   @property
   def platform_headers(self):
     return {
-      'X-OpenLLM-Client-Package-Version': self._version,
+      'X-OpenLLM-Client-Package-Version': self.version,
       'X-OpenLLM-Client-Language': 'Python',
       'X-OpenLLM-Client-Runtime': platform.python_implementation(),
       'X-OpenLLM-Client-Runtime-Version': platform.python_version(),
       'X-OpenLLM-Client-Arch': str(_architecture()),
       'X-OpenLLM-Client-OS': str(_platform()),
     }
 
   def _remaining_retries(self, remaining_retries: int | None, options: RequestOptions) -> int:
-    return remaining_retries if remaining_retries is not None else options.get_max_retries(self._max_retries)
+    return remaining_retries if remaining_retries is not None else options.get_max_retries(self.max_retries)
 
   def _build_headers(self, options: RequestOptions) -> httpx.Headers:
     return httpx.Headers(_merge_mapping(self._default_headers, options.headers or {}))
 
   def _build_request(self, options: RequestOptions) -> httpx.Request:
-    return self._inner.build_request(
+    return self.inner.build_request(
       method=options.method,
       headers=self._build_headers(options),
       url=self._prepare_url(options.url),
       json=options.json,
       params=options.params,
     )
 
   def _calculate_retry_timeout(
     self, remaining_retries: int, options: RequestOptions, headers: t.Optional[httpx.Headers] = None
   ) -> float:
-    max_retries = options.get_max_retries(self._max_retries)
+    max_retries = options.get_max_retries(self.max_retries)
     # https://developer.mozilla.org/en-US/docs/Web/HTTP/Headers/Retry-After
     try:
       if headers is not None:
         retry_header = headers.get('retry-after')
         try:
           retry_after = int(retry_header)
         except ValueError:
@@ -323,15 +315,15 @@
     if response.status_code >= 500:
       return True
     return False
 
   def _process_response_data(
     self, *, response_cls: type[Response], data: t.Dict[str, t.Any], raw_response: httpx.Response
   ) -> Response:
-    return converter.structure(data, response_cls)
+    return response_cls(**data)
 
   def _process_response(
     self,
     *,
     response_cls: type[Response],
     options: RequestOptions,
     raw_response: httpx.Response,
@@ -344,40 +336,38 @@
       response_cls=response_cls,
       stream=stream,
       stream_cls=stream_cls,
       options=options,
     ).parse()
 
 
-@attr.define(init=False)
 class Client(BaseClient[httpx.Client, Stream[t.Any]]):
   def __init__(
     self,
     base_url: str | httpx.URL,
     version: str,
     timeout: int | httpx.Timeout = DEFAULT_TIMEOUT,
     max_retries: int = MAX_RETRIES,
   ):
     super().__init__(
       base_url=base_url,
       version=version,
       timeout=timeout,
       max_retries=max_retries,
-      client=httpx.Client(base_url=base_url, timeout=timeout),
-      _default_stream_cls=Stream,
-      _internal=True,
+      inner=httpx.Client(base_url=base_url, timeout=timeout),
+      default_stream_cls=Stream,
     )
 
   def close(self):
-    self._inner.close()
+    self.inner.close()
 
   def __enter__(self):
     return self
 
-  def __exit__(self, *args) -> None:
+  def __exit__(self, *args: t.Any) -> None:
     self.close()
 
   def __del__(self):
     self.close()
 
   def request(
     self,
@@ -404,25 +394,25 @@
     *,
     stream: bool = False,
     stream_cls: type[_Stream] | None = None,
   ) -> Response | _Stream:
     retries = self._remaining_retries(remaining_retries, options)
     request = self._build_request(options)
     try:
-      response = self._inner.send(request, auth=self.auth, stream=stream)
+      response = self.inner.send(request, auth=self.auth, stream=stream)
       logger.debug('HTTP [%s, %s]: %i [%s]', request.method, request.url, response.status_code, response.reason_phrase)
       response.raise_for_status()
     except httpx.HTTPStatusError as exc:
       if retries > 0 and self._should_retry(exc.response):
         return self._retry_request(
           response_cls, options, retries, exc.response.headers, stream=stream, stream_cls=stream_cls
         )
       # If the response is streamed then we need to explicitly read the completed response
       exc.response.read()
-      raise ValueError(exc.message) from None
+      raise ValueError(exc) from None
     except httpx.TimeoutException:
       if retries > 0:
         return self._retry_request(response_cls, options, retries, stream=stream, stream_cls=stream_cls)
       raise ValueError(request) from None  # timeout
     except Exception:
       if retries > 0:
         return self._retry_request(response_cls, options, retries, stream=stream, stream_cls=stream_cls)
@@ -477,40 +467,38 @@
     if options is None:
       options = {}
     return self.request(
       response_cls, RequestOptions(method='POST', url=path, json=json, **options), stream=stream, stream_cls=stream_cls
     )
 
 
-@attr.define(init=False)
 class AsyncClient(BaseClient[httpx.AsyncClient, AsyncStream[t.Any]]):
   def __init__(
     self,
     base_url: str | httpx.URL,
     version: str,
     timeout: int | httpx.Timeout = DEFAULT_TIMEOUT,
     max_retries: int = MAX_RETRIES,
   ):
     super().__init__(
       base_url=base_url,
       version=version,
       timeout=timeout,
       max_retries=max_retries,
-      client=httpx.AsyncClient(base_url=base_url, timeout=timeout),
-      _default_stream_cls=AsyncStream,
-      _internal=True,
+      inner=httpx.AsyncClient(base_url=base_url, timeout=timeout),
+      default_stream_cls=AsyncStream,
     )
 
   async def close(self):
-    await self._inner.aclose()
+    await self.inner.aclose()
 
   async def __aenter__(self):
     return self
 
-  async def __aexit__(self, *args) -> None:
+  async def __aexit__(self, *args: t.Any) -> None:
     await self.close()
 
   def __del__(self):
     try:
       loop = asyncio.get_event_loop()
       if loop.is_running():
         loop.create_task(self.close())  # noqa
@@ -541,25 +529,25 @@
     stream: bool = False,
     stream_cls: type[_AsyncStream] | None = None,
   ) -> Response | _AsyncStream:
     retries = self._remaining_retries(remaining_retries, options)
     request = self._build_request(options)
 
     try:
-      response = await self._inner.send(request, auth=self.auth, stream=stream)
+      response = await self.inner.send(request, auth=self.auth, stream=stream)
       logger.debug('HTTP [%s, %s]: %i [%s]', request.method, request.url, response.status_code, response.reason_phrase)
       response.raise_for_status()
     except httpx.HTTPStatusError as exc:
       if retries > 0 and self._should_retry(exc.response):
         return self._retry_request(
           response_cls, options, retries, exc.response.headers, stream=stream, stream_cls=stream_cls
         )
       # If the response is streamed then we need to explicitly read the completed response
       await exc.response.aread()
-      raise ValueError(exc.message) from None
+      raise ValueError(exc) from None
     except httpx.ConnectTimeout as err:
       if retries > 0:
         return await self._retry_request(response_cls, options, retries, stream=stream, stream_cls=stream_cls)
       raise ValueError(request) from err  # timeout
     except httpx.ReadTimeout:
       # We don't retry on ReadTimeout error, so something might happen on server-side
       raise
@@ -618,7 +606,11 @@
     stream_cls: type[_AsyncStream] | None = None,
   ) -> Response | _AsyncStream:
     if options is None:
       options = {}
     return await self.request(
       response_cls, RequestOptions(method='POST', url=path, json=json, **options), stream=stream, stream_cls=stream_cls
     )
+
+
+Stream.model_rebuild()
+AsyncStream.model_rebuild()
```

### Comparing `openllm_client-0.5.0a9/src/openllm_client/_stream.py` & `openllm_client-0.5.1/src/openllm_client/_stream.py`

 * *Files 23% similar despite different names*

```diff
@@ -1,105 +1,94 @@
 from __future__ import annotations
-import typing as t
 
-import attr
-import httpx
-import orjson
+import pydantic, httpx, orjson, typing as t
 
 if t.TYPE_CHECKING:
   from ._shim import AsyncClient, Client
 
-Response = t.TypeVar('Response', bound=attr.AttrsInstance)
+Response = t.TypeVar('Response', bound=pydantic.BaseModel)
 
 
-@attr.define(auto_attribs=True)
-class Stream(t.Generic[Response]):
-  _response_cls: t.Type[Response]
-  _response: httpx.Response
-  _client: Client
-  _decoder: SSEDecoder = attr.field(factory=lambda: SSEDecoder())
-  _iterator: t.Iterator[Response] = attr.field(init=False)
+class Stream(pydantic.BaseModel, t.Generic[Response]):
+  model_config = pydantic.ConfigDict(arbitrary_types_allowed=True)
+  response_cls: t.Type[Response]
+  response: pydantic.SkipValidation[httpx.Response]
+  client: Client
+  _decoder: SSEDecoder = pydantic.PrivateAttr(default_factory=lambda: SSEDecoder())
+  _iterator: t.Iterator[Response] = pydantic.PrivateAttr()
 
-  def __init__(self, response_cls, response, client):
-    self.__attrs_init__(response_cls, response, client)
+  def __init__(self, **data):
+    super().__init__(**data)
     self._iterator = self._stream()
 
   def __next__(self):
     return self._iterator.__next__()
 
   def __iter__(self) -> t.Iterator[Response]:
     for item in self._iterator:
       yield item
 
   def _iter_events(self) -> t.Iterator[SSE]:
-    yield from self._decoder.iter(self._response.iter_lines())
+    yield from self._decoder.iter(self.response.iter_lines())
 
   def _stream(self) -> t.Iterator[Response]:
     for sse in self._iter_events():
       if sse.data.startswith('[DONE]'):
         break
       if sse.event is None:
-        yield self._client._process_response_data(
-          data=sse.model_dump(), response_cls=self._response_cls, raw_response=self._response
+        yield self.client._process_response_data(
+          data=orjson.loads(sse.data), response_cls=self.response_cls, raw_response=self.response
         )
 
 
-@attr.define(auto_attribs=True)
-class AsyncStream(t.Generic[Response]):
-  _response_cls: t.Type[Response]
-  _response: httpx.Response
-  _client: AsyncClient
-  _decoder: SSEDecoder = attr.field(factory=lambda: SSEDecoder())
-  _iterator: t.Iterator[Response] = attr.field(init=False)
+class AsyncStream(pydantic.BaseModel, t.Generic[Response]):
+  model_config = pydantic.ConfigDict(arbitrary_types_allowed=True)
+  response_cls: t.Type[Response]
+  response: pydantic.SkipValidation[httpx.Response]
+  client: AsyncClient
+  _decoder: SSEDecoder = pydantic.PrivateAttr(default_factory=lambda: SSEDecoder())
+  _iterator: t.Iterator[Response] = pydantic.PrivateAttr()
 
-  def __init__(self, response_cls, response, client):
-    self.__attrs_init__(response_cls, response, client)
+  def __init__(self, **data):
+    super().__init__(**data)
     self._iterator = self._stream()
 
   async def __anext__(self):
     return await self._iterator.__anext__()
 
   async def __aiter__(self):
     async for item in self._iterator:
       yield item
 
   async def _iter_events(self):
-    async for sse in self._decoder.aiter(self._response.aiter_lines()):
+    async for sse in self._decoder.aiter(self.response.aiter_lines()):
       yield sse
 
   async def _stream(self) -> t.AsyncGenerator[Response, None]:
     async for sse in self._iter_events():
       if sse.data.startswith('[DONE]'):
         break
       if sse.event is None:
-        yield self._client._process_response_data(
-          data=sse.model_dump(), response_cls=self._response_cls, raw_response=self._response
+        yield self.client._process_response_data(
+          data=orjson.loads(sse.data), response_cls=self.response_cls, raw_response=self.response
         )
 
 
-@attr.define
-class SSE:
-  data: str = attr.field(default='')
-  id: t.Optional[str] = attr.field(default=None)
-  event: t.Optional[str] = attr.field(default=None)
-  retry: t.Optional[int] = attr.field(default=None)
-
-  def model_dump(self) -> t.Dict[str, t.Any]:
-    try:
-      return orjson.loads(self.data)
-    except orjson.JSONDecodeError:
-      raise
-
-
-@attr.define(auto_attribs=True)
-class SSEDecoder:
-  _data: t.List[str] = attr.field(factory=list)
-  _event: t.Optional[str] = None
-  _retry: t.Optional[int] = None
-  _last_event_id: t.Optional[str] = None
+class SSE(pydantic.BaseModel):
+  data: str = pydantic.Field(default='')
+  id: t.Optional[str] = pydantic.Field(default=None)
+  event: t.Optional[str] = pydantic.Field(default=None)
+  retry: t.Optional[int] = pydantic.Field(default=None)
+
+
+class SSEDecoder(pydantic.BaseModel):
+  _data: t.List[str] = pydantic.PrivateAttr(default_factory=list)
+  event: t.Optional[str] = None
+  retry: t.Optional[int] = None
+  last_event_id: t.Optional[str] = None
 
   def iter(self, iterator: t.Iterator[str]) -> t.Iterator[SSE]:
     for line in iterator:
       sse = self.decode(line.rstrip('\n'))
       if sse:
         yield sse
 
@@ -108,34 +97,34 @@
       sse = self.decode(line.rstrip('\n'))
       if sse:
         yield sse
 
   def decode(self, line: str) -> SSE | None:
     # NOTE: https://html.spec.whatwg.org/multipage/server-sent-events.html#event-stream-interpretation
     if not line:
-      if all(not a for a in [self._event, self._data, self._retry, self._last_event_id]):
+      if all(not a for a in [self.event, self._data, self.retry, self.last_event_id]):
         return None
-      sse = SSE(data='\n'.join(self._data), event=self._event, retry=self._retry, id=self._last_event_id)
-      self._event, self._data, self._retry = None, [], None
+      sse = SSE(data='\n'.join(self._data), event=self.event, retry=self.retry, id=self.last_event_id)
+      self.event, self._data, self.retry = None, [], None
       return sse
     if line.startswith(':'):
       return None
     field, _, value = line.partition(':')
     if value.startswith(' '):
       value = value[1:]
     if field == 'event':
-      self._event = value
+      self.event = value
     elif field == 'data':
       self._data.append(value)
     elif field == 'id':
       if '\0' in value:
         pass
       else:
-        self._last_event_id = value
+        self.last_event_id = value
     elif field == 'retry':
       try:
-        self._retry = int(value)
+        self.retry = int(value)
       except (TypeError, ValueError):
         pass
     else:
       pass  # Ignore unknown fields
     return None
```

### Comparing `openllm_client-0.5.0a9/src/openllm_client/_typing_compat.py` & `openllm_client-0.5.1/src/openllm_client/_typing_compat.py`

 * *Files 20% similar despite different names*

```diff
@@ -3,14 +3,15 @@
 from openllm_core._typing_compat import (
   Annotated as Annotated,
   LiteralString as LiteralString,
   NotRequired as NotRequired,
   Required as Required,
   Self as Self,
   TypeGuard as TypeGuard,
+  TypedDict as TypedDict,
   dataclass_transform as dataclass_transform,
   overload as overload,
 )
 
 Platform = Annotated[
   LiteralString, Literal['MacOS', 'Linux', 'Windows', 'FreeBSD', 'OpenBSD', 'iOS', 'iPadOS', 'Android', 'Unknown'], str
 ]
```

### Comparing `openllm_client-0.5.0a9/.gitignore` & `openllm_client-0.5.1/.gitignore`

 * *Files identical despite different names*

### Comparing `openllm_client-0.5.0a9/LICENSE.md` & `openllm_client-0.5.1/LICENSE.md`

 * *Files identical despite different names*

### Comparing `openllm_client-0.5.0a9/pyproject.toml` & `openllm_client-0.5.1/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -48,15 +48,15 @@
     "Large Language Model",
     "Generative AI",
     "StableLM",
     "Alpaca",
     "PyTorch",
     "Transformers",
 ]
-dependencies = ["openllm-core", "attrs>=23.2.0", "httpx", "distro", "anyio"]
+dependencies = ["openllm-core", "httpx", "distro", "anyio"]
 license = "Apache-2.0"
 name = "openllm-client"
 requires-python = ">=3.8"
 [project.urls]
 Blog = "https://modelserving.com"
 Chat = "https://l.bentoml.com/join-openllm-discord"
 Documentation = "https://github.com/bentoml/OpenLLM/blob/main/openllm-client/README.md"
```

#### html2text {}

```diff
@@ -13,27 +13,27 @@
 :: Python :: 3.10", "Programming Language :: Python :: 3.11", "Programming
 Language :: Python :: Implementation :: CPython", "Programming Language ::
 Python :: Implementation :: PyPy", ] description = "OpenLLM Client: Interacting
 with OpenLLM HTTP/gRPC server, or any BentoML server." keywords = [ "MLOps",
 "AI", "BentoML", "Model Serving", "Model Deployment", "LLMOps", "Falcon",
 "Vicuna", "Llama 2", "Fine tuning", "Serverless", "Large Language Model",
 "Generative AI", "StableLM", "Alpaca", "PyTorch", "Transformers", ]
-dependencies = ["openllm-core", "attrs>=23.2.0", "httpx", "distro", "anyio"]
-license = "Apache-2.0" name = "openllm-client" requires-python = ">=3.8"
-[project.urls] Blog = "https://modelserving.com" Chat = "https://l.bentoml.com/
-join-openllm-discord" Documentation = "https://github.com/bentoml/OpenLLM/blob/
-main/openllm-client/README.md" GitHub = "https://github.com/bentoml/OpenLLM/
-blob/main/openllm-client" History = "https://github.com/bentoml/OpenLLM/blob/
-main/CHANGELOG.md" Homepage = "https://bentoml.com" Tracker = "https://
-github.com/bentoml/OpenLLM/issues" Twitter = "https://twitter.com/bentomlai"
-[project.optional-dependencies] full = ["openllm-client[grpc,agents,auth]"]
-grpc = ["bentoml[grpc]>=1.1.11,<1.2"] auth = ['httpx_auth'] agents =
-["transformers[agents]>=4.30", "diffusers", "soundfile"] [tool.hatch.version]
-fallback-version = "0.0.0" source = "vcs" [tool.hatch.build.hooks.vcs] version-
-file = "src/openllm_client/_version.py" [tool.hatch.version.raw-options]
+dependencies = ["openllm-core", "httpx", "distro", "anyio"] license = "Apache-
+2.0" name = "openllm-client" requires-python = ">=3.8" [project.urls] Blog =
+"https://modelserving.com" Chat = "https://l.bentoml.com/join-openllm-discord"
+Documentation = "https://github.com/bentoml/OpenLLM/blob/main/openllm-client/
+README.md" GitHub = "https://github.com/bentoml/OpenLLM/blob/main/openllm-
+client" History = "https://github.com/bentoml/OpenLLM/blob/main/CHANGELOG.md"
+Homepage = "https://bentoml.com" Tracker = "https://github.com/bentoml/OpenLLM/
+issues" Twitter = "https://twitter.com/bentomlai" [project.optional-
+dependencies] full = ["openllm-client[grpc,agents,auth]"] grpc = ["bentoml
+[grpc]>=1.1.11,<1.2"] auth = ['httpx_auth'] agents = ["transformers
+[agents]>=4.30", "diffusers", "soundfile"] [tool.hatch.version] fallback-
+version = "0.0.0" source = "vcs" [tool.hatch.build.hooks.vcs] version-file =
+"src/openllm_client/_version.py" [tool.hatch.version.raw-options]
 git_describe_command = [ "git", "describe", "--dirty", "--tags", "--long", "--
 first-parent", ] local_scheme = "no-local-version" root = ".."
 [tool.hatch.metadata] allow-direct-references = true
 [tool.hatch.build.targets.wheel] only-include = ["src/openllm_client"] sources
 = ["src"] [tool.hatch.build.targets.sdist] exclude = [ "/.git_archival.txt",
 "tests", "/.python-version-default", "/generate-grpc-stubs", "/dev.Dockerfile",
 ] [tool.hatch.metadata.hooks.fancy-pypi-readme] content-type = "text/markdown"
```

### Comparing `openllm_client-0.5.0a9/PKG-INFO` & `openllm_client-0.5.1/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: openllm-client
-Version: 0.5.0a9
+Version: 0.5.1
 Summary: OpenLLM Client: Interacting with OpenLLM HTTP/gRPC server, or any BentoML server.
 Project-URL: Blog, https://modelserving.com
 Project-URL: Chat, https://l.bentoml.com/join-openllm-discord
 Project-URL: Documentation, https://github.com/bentoml/OpenLLM/blob/main/openllm-client/README.md
 Project-URL: GitHub, https://github.com/bentoml/OpenLLM/blob/main/openllm-client
 Project-URL: History, https://github.com/bentoml/OpenLLM/blob/main/CHANGELOG.md
 Project-URL: Homepage, https://bentoml.com
@@ -30,15 +30,14 @@
 Classifier: Programming Language :: Python :: Implementation :: CPython
 Classifier: Programming Language :: Python :: Implementation :: PyPy
 Classifier: Topic :: Scientific/Engineering
 Classifier: Topic :: Software Development :: Libraries
 Classifier: Typing :: Typed
 Requires-Python: >=3.8
 Requires-Dist: anyio
-Requires-Dist: attrs>=23.2.0
 Requires-Dist: distro
 Requires-Dist: httpx
 Requires-Dist: openllm-core
 Provides-Extra: agents
 Requires-Dist: diffusers; extra == 'agents'
 Requires-Dist: soundfile; extra == 'agents'
 Requires-Dist: transformers[agents]>=4.30; extra == 'agents'
@@ -95,23 +94,14 @@
 deploy to the cloud or on-premises, and build powerful AI apps, and more.
 
 To learn more about OpenLLM, please visit <a href="https://github.com/bentoml/OpenLLM">OpenLLM's README.md</a>
 
 This package holds the underlying client implementation for OpenLLM. If you are
 coming from OpenLLM, the client can be accessed via `openllm.client`.
 
-It provides somewhat of a "similar" APIs to [`bentoml.Client`](https://docs.bentoml.com/en/latest/guides/client.html)
-(via `openllm_client.min`) for interacting with OpenLLM server. This can also be extended to use with general
-BentoML server as well.
-
-> [!NOTE]
-> The component of interop with generic BentoML server will be considered as _EXPERIMENTAL_ and
-> will be refactored to new client implementation soon!
-> If you are just using this package for interacting with OpenLLM server, The API should be the same as `openllm.client` namespace.
-
 ```python
 import openllm
 
 client = openllm.client.HTTPClient()
 
 client.query('Explain to me the difference between "further" and "farther"')
 ```
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: openllm-client Version: 0.5.0a9 Summary: OpenLLM
+Metadata-Version: 2.1 Name: openllm-client Version: 0.5.1 Summary: OpenLLM
 Client: Interacting with OpenLLM HTTP/gRPC server, or any BentoML server.
 Project-URL: Blog, https://modelserving.com Project-URL: Chat, https://
 l.bentoml.com/join-openllm-discord Project-URL: Documentation, https://
 github.com/bentoml/OpenLLM/blob/main/openllm-client/README.md Project-URL:
 GitHub, https://github.com/bentoml/OpenLLM/blob/main/openllm-client Project-
 URL: History, https://github.com/bentoml/OpenLLM/blob/main/CHANGELOG.md
 Project-URL: Homepage, https://bentoml.com Project-URL: Tracker, https://
@@ -21,43 +21,35 @@
 Programming Language :: Python :: 3 :: Only Classifier: Programming Language ::
 Python :: 3.8 Classifier: Programming Language :: Python :: 3.9 Classifier:
 Programming Language :: Python :: 3.10 Classifier: Programming Language ::
 Python :: 3.11 Classifier: Programming Language :: Python :: Implementation ::
 CPython Classifier: Programming Language :: Python :: Implementation :: PyPy
 Classifier: Topic :: Scientific/Engineering Classifier: Topic :: Software
 Development :: Libraries Classifier: Typing :: Typed Requires-Python: >=3.8
-Requires-Dist: anyio Requires-Dist: attrs>=23.2.0 Requires-Dist: distro
-Requires-Dist: httpx Requires-Dist: openllm-core Provides-Extra: agents
-Requires-Dist: diffusers; extra == 'agents' Requires-Dist: soundfile; extra ==
-'agents' Requires-Dist: transformers[agents]>=4.30; extra == 'agents' Provides-
-Extra: auth Requires-Dist: httpx-auth; extra == 'auth' Provides-Extra: full
-Requires-Dist: openllm-client[agents,auth,grpc]; extra == 'full' Provides-
-Extra: grpc Requires-Dist: bentoml[grpc]<1.2,>=1.1.11; extra == 'grpc'
-Description-Content-Type: text/markdown
+Requires-Dist: anyio Requires-Dist: distro Requires-Dist: httpx Requires-Dist:
+openllm-core Provides-Extra: agents Requires-Dist: diffusers; extra == 'agents'
+Requires-Dist: soundfile; extra == 'agents' Requires-Dist: transformers
+[agents]>=4.30; extra == 'agents' Provides-Extra: auth Requires-Dist: httpx-
+auth; extra == 'auth' Provides-Extra: full Requires-Dist: openllm-client
+[agents,auth,grpc]; extra == 'full' Provides-Extra: grpc Requires-Dist: bentoml
+[grpc]<1.2,>=1.1.11; extra == 'grpc' Description-Content-Type: text/markdown
                              _[_B_a_n_n_e_r_ _f_o_r_ _O_p_e_n_L_L_M_]
                        ************ ?ð???¾ OOppeennLLLLMM CClliieenntt ************
   _[_p_y_p_i___s_t_a_t_u_s_]_[_t_e_s_t___p_y_p_i___s_t_a_t_u_s_]_[_T_w_i_t_t_e_r_]_[_D_i_s_c_o_r_d_]_[_c_i_]_[_p_r_e_-_c_o_m_m_i_t_._c_i_ _s_t_a_t_u_s_]
    _[_p_y_t_h_o_n___v_e_r_s_i_o_n_]_[_H_a_t_c_h_]_[_c_o_d_e_ _s_t_y_l_e_]_[_R_u_f_f_]_[_t_y_p_e_s_ _-_ _m_y_p_y_]_[_t_y_p_e_s_ _-_ _p_y_r_i_g_h_t_]
    OpenLLM Client: Interacting with OpenLLM HTTP/gRPC server, or any BentoML
                                     server.
 ## ð Introduction With OpenLLM, you can run inference with any open-source
 large-language models, deploy to the cloud or on-premises, and build powerful
 AI apps, and more. To learn more about OpenLLM, please visit _O_p_e_n_L_L_M_'_s
 _R_E_A_D_M_E_._m_d This package holds the underlying client implementation for OpenLLM.
 If you are coming from OpenLLM, the client can be accessed via
-`openllm.client`. It provides somewhat of a "similar" APIs to
-[`bentoml.Client`](https://docs.bentoml.com/en/latest/guides/client.html) (via
-`openllm_client.min`) for interacting with OpenLLM server. This can also be
-extended to use with general BentoML server as well. > [!NOTE] > The component
-of interop with generic BentoML server will be considered as _EXPERIMENTAL_ and
-> will be refactored to new client implementation soon! > If you are just using
-this package for interacting with OpenLLM server, The API should be the same as
-`openllm.client` namespace. ```python import openllm client =
-openllm.client.HTTPClient() client.query('Explain to me the difference between
-"further" and "farther"') ```
+`openllm.client`. ```python import openllm client = openllm.client.HTTPClient()
+client.query('Explain to me the difference between "further" and "farther"')
+```
                           [Gif showing OpenLLM Intro]
                         [Gif showing Agent integration]
 ## ð Citation If you use OpenLLM in your research, we provide a [citation]
 (../CITATION.cff) to use: ```bibtex @software{Pham_OpenLLM_Operating_LLMs_2023,
 author = {Pham, Aaron and Yang, Chaoyu and Sheng, Sean and Zhao, Shenyang and
 Lee, Sauyon and Jiang, Bo and Dong, Fog and Guan, Xipeng and Ming, Frost},
 license = {Apache-2.0}, month = jun, title = {{OpenLLM: Operating LLMs in
```

