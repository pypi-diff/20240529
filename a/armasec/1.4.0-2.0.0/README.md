# Comparing `tmp/armasec-1.4.0.tar.gz` & `tmp/armasec-2.0.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "armasec-1.4.0.tar", max compression
+gzip compressed data, was "armasec-2.0.0.tar", max compression
```

## Comparing `armasec-1.4.0.tar` & `armasec-2.0.0.tar`

### file list

```diff
@@ -1,31 +1,31 @@
--rw-r--r--   0        0        0     1078 2024-04-01 20:26:59.433843 armasec-1.4.0/LICENSE.md
--rw-r--r--   0        0        0     2646 2024-04-01 20:26:59.433843 armasec-1.4.0/README.md
--rw-r--r--   0        0        0      423 2024-04-01 20:26:59.433843 armasec-1.4.0/armasec/__init__.py
--rw-r--r--   0        0        0     4776 2024-04-01 20:26:59.433843 armasec-1.4.0/armasec/armasec.py
--rw-r--r--   0        0        0     1369 2024-04-01 20:26:59.433843 armasec-1.4.0/armasec/exceptions.py
--rw-r--r--   0        0        0     3823 2024-04-01 20:26:59.433843 armasec-1.4.0/armasec/openid_config_loader.py
--rw-r--r--   0        0        0      280 2024-04-01 20:26:59.433843 armasec-1.4.0/armasec/pluggable/__init__.py
--rw-r--r--   0        0        0     1237 2024-04-01 20:26:59.433843 armasec-1.4.0/armasec/pluggable/hookspecs.py
--rw-r--r--   0        0        0        0 2024-04-01 20:26:59.433843 armasec-1.4.0/armasec/py.typed
--rw-r--r--   0        0        0     9554 2024-04-01 20:26:59.433843 armasec-1.4.0/armasec/pytest_extension.py
--rw-r--r--   0        0        0      232 2024-04-01 20:26:59.433843 armasec-1.4.0/armasec/schemas/__init__.py
--rw-r--r--   0        0        0     2083 2024-04-01 20:26:59.433843 armasec-1.4.0/armasec/schemas/armasec_config.py
--rw-r--r--   0        0        0     1305 2024-04-01 20:26:59.433843 armasec-1.4.0/armasec/schemas/jwks.py
--rw-r--r--   0        0        0      637 2024-04-01 20:26:59.433843 armasec-1.4.0/armasec/schemas/openid_config.py
--rw-r--r--   0        0        0     6249 2024-04-01 20:26:59.433843 armasec-1.4.0/armasec/token_decoder.py
--rw-r--r--   0        0        0     3616 2024-04-01 20:26:59.433843 armasec-1.4.0/armasec/token_manager.py
--rw-r--r--   0        0        0     1165 2024-04-01 20:26:59.433843 armasec-1.4.0/armasec/token_payload.py
--rw-r--r--   0        0        0    10884 2024-04-01 20:26:59.433843 armasec-1.4.0/armasec/token_security.py
--rw-r--r--   0        0        0     1105 2024-04-01 20:26:59.433843 armasec-1.4.0/armasec/utilities.py
--rw-r--r--   0        0        0     9089 2024-04-01 20:26:59.433843 armasec-1.4.0/armasec_cli/auth.py
--rw-r--r--   0        0        0     3050 2024-04-01 20:26:59.433843 armasec-1.4.0/armasec_cli/cache.py
--rw-r--r--   0        0        0     8270 2024-04-01 20:26:59.433843 armasec-1.4.0/armasec_cli/client.py
--rw-r--r--   0        0        0     2277 2024-04-01 20:26:59.433843 armasec-1.4.0/armasec_cli/config.py
--rw-r--r--   0        0        0     1521 2024-04-01 20:26:59.433843 armasec-1.4.0/armasec_cli/exceptions.py
--rw-r--r--   0        0        0      756 2024-04-01 20:26:59.433843 armasec-1.4.0/armasec_cli/format.py
--rw-r--r--   0        0        0      194 2024-04-01 20:26:59.433843 armasec-1.4.0/armasec_cli/logging.py
--rw-r--r--   0        0        0     6113 2024-04-01 20:26:59.433843 armasec-1.4.0/armasec_cli/main.py
--rw-r--r--   0        0        0      642 2024-04-01 20:26:59.433843 armasec-1.4.0/armasec_cli/schemas.py
--rw-r--r--   0        0        0     3057 2024-04-01 20:26:59.433843 armasec-1.4.0/armasec_cli/time_loop.py
--rw-r--r--   0        0        0     2663 2024-04-01 20:26:59.461843 armasec-1.4.0/pyproject.toml
--rw-r--r--   0        0        0     4446 1970-01-01 00:00:00.000000 armasec-1.4.0/PKG-INFO
+-rw-r--r--   0        0        0     1078 2024-05-29 20:36:44.159150 armasec-2.0.0/LICENSE.md
+-rw-r--r--   0        0        0     2646 2024-05-29 20:36:44.159150 armasec-2.0.0/README.md
+-rw-r--r--   0        0        0      423 2024-05-29 20:36:44.159150 armasec-2.0.0/armasec/__init__.py
+-rw-r--r--   0        0        0     4776 2024-05-29 20:36:44.159150 armasec-2.0.0/armasec/armasec.py
+-rw-r--r--   0        0        0     1369 2024-05-29 20:36:44.159150 armasec-2.0.0/armasec/exceptions.py
+-rw-r--r--   0        0        0     3828 2024-05-29 20:36:44.159150 armasec-2.0.0/armasec/openid_config_loader.py
+-rw-r--r--   0        0        0      280 2024-05-29 20:36:44.159150 armasec-2.0.0/armasec/pluggable/__init__.py
+-rw-r--r--   0        0        0     1237 2024-05-29 20:36:44.159150 armasec-2.0.0/armasec/pluggable/hookspecs.py
+-rw-r--r--   0        0        0        0 2024-05-29 20:36:44.159150 armasec-2.0.0/armasec/py.typed
+-rw-r--r--   0        0        0     9588 2024-05-29 20:36:44.159150 armasec-2.0.0/armasec/pytest_extension.py
+-rw-r--r--   0        0        0      232 2024-05-29 20:36:44.159150 armasec-2.0.0/armasec/schemas/__init__.py
+-rw-r--r--   0        0        0     2083 2024-05-29 20:36:44.159150 armasec-2.0.0/armasec/schemas/armasec_config.py
+-rw-r--r--   0        0        0     1340 2024-05-29 20:36:44.159150 armasec-2.0.0/armasec/schemas/jwks.py
+-rw-r--r--   0        0        0      651 2024-05-29 20:36:44.159150 armasec-2.0.0/armasec/schemas/openid_config.py
+-rw-r--r--   0        0        0     6255 2024-05-29 20:36:44.159150 armasec-2.0.0/armasec/token_decoder.py
+-rw-r--r--   0        0        0     3616 2024-05-29 20:36:44.159150 armasec-2.0.0/armasec/token_manager.py
+-rw-r--r--   0        0        0     1266 2024-05-29 20:36:44.159150 armasec-2.0.0/armasec/token_payload.py
+-rw-r--r--   0        0        0    10898 2024-05-29 20:36:44.159150 armasec-2.0.0/armasec/token_security.py
+-rw-r--r--   0        0        0     1105 2024-05-29 20:36:44.159150 armasec-2.0.0/armasec/utilities.py
+-rw-r--r--   0        0        0     9089 2024-05-29 20:36:44.159150 armasec-2.0.0/armasec_cli/auth.py
+-rw-r--r--   0        0        0     3050 2024-05-29 20:36:44.159150 armasec-2.0.0/armasec_cli/cache.py
+-rw-r--r--   0        0        0     8281 2024-05-29 20:36:44.159150 armasec-2.0.0/armasec_cli/client.py
+-rw-r--r--   0        0        0     2283 2024-05-29 20:36:44.159150 armasec-2.0.0/armasec_cli/config.py
+-rw-r--r--   0        0        0     1521 2024-05-29 20:36:44.159150 armasec-2.0.0/armasec_cli/exceptions.py
+-rw-r--r--   0        0        0      756 2024-05-29 20:36:44.159150 armasec-2.0.0/armasec_cli/format.py
+-rw-r--r--   0        0        0      194 2024-05-29 20:36:44.159150 armasec-2.0.0/armasec_cli/logging.py
+-rw-r--r--   0        0        0     6119 2024-05-29 20:36:44.159150 armasec-2.0.0/armasec_cli/main.py
+-rw-r--r--   0        0        0      663 2024-05-29 20:36:44.159150 armasec-2.0.0/armasec_cli/schemas.py
+-rw-r--r--   0        0        0     3057 2024-05-29 20:36:44.159150 armasec-2.0.0/armasec_cli/time_loop.py
+-rw-r--r--   0        0        0     2603 2024-05-29 20:36:44.179150 armasec-2.0.0/pyproject.toml
+-rw-r--r--   0        0        0     4457 1970-01-01 00:00:00.000000 armasec-2.0.0/PKG-INFO
```

### Comparing `armasec-1.4.0/LICENSE.md` & `armasec-2.0.0/LICENSE.md`

 * *Files identical despite different names*

### Comparing `armasec-1.4.0/README.md` & `armasec-2.0.0/README.md`

 * *Files identical despite different names*

### Comparing `armasec-1.4.0/armasec/armasec.py` & `armasec-2.0.0/armasec/armasec.py`

 * *Files identical despite different names*

### Comparing `armasec-1.4.0/armasec/exceptions.py` & `armasec-2.0.0/armasec/exceptions.py`

 * *Files identical despite different names*

### Comparing `armasec-1.4.0/armasec/openid_config_loader.py` & `armasec-2.0.0/armasec/openid_config_loader.py`

 * *Files 1% similar despite different names*

```diff
@@ -91,15 +91,15 @@
     def jwks(self) -> JWKs:
         """
         Retrives JWKs public keys from an OIDC provider. Lazy loads the jwks so that API calls are
         deferred until the jwks are needed.
         """
         if not self._jwks:
             self.debug_logger("Fetching jwks")
-            data = self._load_openid_resource(self.config.jwks_uri)
+            data = self._load_openid_resource(str(self.config.jwks_uri))
             with AuthenticationError.handle_errors(
                 message="jwks data was invalid",
                 do_except=partial(log_error, self.debug_logger),
             ):
                 self._jwks = JWKs(**data)
 
         return self._jwks
```

### Comparing `armasec-1.4.0/armasec/pluggable/hookspecs.py` & `armasec-2.0.0/armasec/pluggable/hookspecs.py`

 * *Files identical despite different names*

### Comparing `armasec-1.4.0/armasec/pytest_extension.py` & `armasec-2.0.0/armasec/pytest_extension.py`

 * *Files 2% similar despite different names*

```diff
@@ -254,22 +254,22 @@
         MockOpenidRoutes = namedtuple("MockOpenidRoutes", ["openid_config_route", "jwks_route"])
         with respx.mock:
             openid_config_route = respx.get(
                 OpenidConfigLoader.build_openid_config_url(domain),
             )
             openid_config_route.return_value = httpx.Response(
                 starlette.status.HTTP_200_OK,
-                json=openid_config.dict(),
+                json=openid_config.model_dump(mode="json"),
             )
 
             jwks = JWKs(keys=[jwk])
             jwks_route = respx.get(jwks_uri)
             jwks_route.return_value = httpx.Response(
                 starlette.status.HTTP_200_OK,
-                json=jwks.dict(),
+                json=jwks.model_dump(mode="json"),
             )
             yield MockOpenidRoutes(openid_config_route, jwks_route)
 
     return _helper
 
 
 @pytest.fixture
```

### Comparing `armasec-1.4.0/armasec/schemas/armasec_config.py` & `armasec-2.0.0/armasec/schemas/armasec_config.py`

 * *Files identical despite different names*

### Comparing `armasec-1.4.0/armasec/schemas/jwks.py` & `armasec-2.0.0/armasec/schemas/jwks.py`

 * *Files 13% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 """
 This module provides pydantic schemas for JSON Web Keys.
 """
 
 from typing import List, Optional
 
-from pydantic import BaseModel
+from pydantic import ConfigDict, BaseModel
 
 
 class JWK(BaseModel):
     """
     This Model provides a specification for the objects retrieved from JWK endpoints in OIDC
     providers. It also assists with validation and item access.
 
@@ -25,20 +25,18 @@
 
     alg: str
     e: str
     kid: str
     kty: str
     n: str
 
-    use: Optional[str]
-    x5c: Optional[List[str]]
-    x5t: Optional[str]
-
-    class Config:
-        extra = "allow"
+    use: Optional[str] = None
+    x5c: Optional[List[str]] = None
+    x5t: Optional[str] = None
+    model_config = ConfigDict(extra="allow")
 
 
 class JWKs(BaseModel):
     """
     This Model provides a specification for the container object retrieved from JWK endpoints in
     OIDC providers. It also assists with validation and item access.
```

### Comparing `armasec-1.4.0/armasec/schemas/openid_config.py` & `armasec-2.0.0/armasec/schemas/openid_config.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 """
 This module provides a pydantic schema describing openid-configuration data.
 """
 
-from pydantic import AnyHttpUrl, BaseModel
+from pydantic import ConfigDict, AnyHttpUrl, BaseModel
 
 
 class OpenidConfig(BaseModel):
     """
     Provides a specification for the objects retrieved from openid_configuration endpoint of the
     OIDC providers. Only includes needed fields for supported Manager instances. Assists with
     validation and item access.
@@ -14,10 +14,8 @@
     Attributes:
         issuer:   The URL of the issuer of the tokens.
         jwks_uri: The URI where JWKs can be foun don the OpenID server.
     """
 
     issuer: AnyHttpUrl
     jwks_uri: AnyHttpUrl
-
-    class Config:
-        extra = "allow"
+    model_config = ConfigDict(extra="allow")
```

### Comparing `armasec-1.4.0/armasec/token_decoder.py` & `armasec-2.0.0/armasec/token_decoder.py`

 * *Files 0% similar despite different names*

```diff
@@ -94,15 +94,15 @@
             "Unverified header doesn't contain 'kid'...not sure how this happened",
         )
 
         for jwk in self.jwks.keys:
             self.debug_logger(f"Checking key in jwk: {jwk}")
             if jwk.kid == kid:
                 self.debug_logger("Key matches unverified header. Using as decode secret.")
-                return jwk.dict()
+                return jwk.model_dump()
 
         raise AuthenticationError("Could not find a matching jwk")
 
     def decode(self, token: str, **claims) -> TokenPayload:
         """
         Decode a JWT into a TokenPayload while checking signatures and claims.
```

### Comparing `armasec-1.4.0/armasec/token_manager.py` & `armasec-2.0.0/armasec/token_manager.py`

 * *Files identical despite different names*

### Comparing `armasec-1.4.0/armasec/token_payload.py` & `armasec-2.0.0/armasec/token_payload.py`

 * *Files 21% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 """
 This module defines a pydantic schema for the payload of a jwt.
 """
 
 from datetime import datetime
 from typing import List, Optional
 
-from pydantic import BaseModel, Field
+from pydantic import ConfigDict, BaseModel, Field, AliasChoices
 
 
 class TokenPayload(BaseModel):
     """
     A convenience class that can be used to access parts of a decoded jwt.
 
     Attributes:
@@ -18,20 +18,18 @@
         expire:         The "exp" claim extracted from a JWT.
         client_id:      The "azp" claim extracted from a JWT.
         original_token: The original token value
     """
 
     sub: str
     permissions: List[str] = Field(list())
-    expire: datetime = Field(None, alias="exp")
-    client_id: str = Field(None, alias="azp")
+    expire: datetime = Field(None, validation_alias=AliasChoices("exp", "expire"))
+    client_id: str = Field(None, validation_alias=AliasChoices("azp", "client_id"))
     original_token: Optional[str] = None
-
-    class Config:
-        extra = "allow"
+    model_config = ConfigDict(extra="allow")
 
     def to_dict(self):
         """
         Convert a TokenPayload to the equivalent dictionary returned by `jwt.decode()`.
         """
         return dict(
             sub=self.sub,
```

### Comparing `armasec-1.4.0/armasec/token_security.py` & `armasec-2.0.0/armasec/token_security.py`

 * *Files 3% similar despite different names*

```diff
@@ -4,15 +4,15 @@
 
 from typing import Callable, Iterable, List, Optional
 
 from auto_name_enum import AutoNameEnum, auto
 from fastapi import HTTPException, status
 from fastapi.openapi.models import APIKey, APIKeyIn
 from fastapi.security.api_key import APIKeyBase
-from pydantic import BaseModel
+from pydantic import ConfigDict, BaseModel
 from snick import unwrap
 from starlette.requests import Request
 
 from armasec.exceptions import AuthenticationError, AuthorizationError
 from armasec.openid_config_loader import OpenidConfigLoader
 from armasec.pluggable import plugin_manager
 from armasec.schemas import DomainConfig
@@ -29,17 +29,15 @@
     Attributes:
         manager: The TokenManager instance to use for decoding tokens.
         domain_config: The DomainConfig for the openid server.
     """
 
     manager: TokenManager
     domain_config: DomainConfig
-
-    class Config:
-        arbitrary_types_allowed = True
+    model_config = ConfigDict(arbitrary_types_allowed=True)
 
 
 class PermissionMode(AutoNameEnum):
     """
     Endpoint permissions.
 
     Attributes:
```

### Comparing `armasec-1.4.0/armasec/utilities.py` & `armasec-2.0.0/armasec/utilities.py`

 * *Files identical despite different names*

### Comparing `armasec-1.4.0/armasec_cli/auth.py` & `armasec-2.0.0/armasec_cli/auth.py`

 * *Files identical despite different names*

### Comparing `armasec-1.4.0/armasec_cli/cache.py` & `armasec-2.0.0/armasec_cli/cache.py`

 * *Files identical despite different names*

### Comparing `armasec-1.4.0/armasec_cli/client.py` & `armasec-2.0.0/armasec_cli/client.py`

 * *Files 1% similar despite different names*

```diff
@@ -92,15 +92,15 @@
                 f"""
                 Could not deserialize instance of {request_model.__class__}:
                 {request_model}
                 """
             ),
         ),
     ):
-        request_kwargs["content"] = request_model.json()
+        request_kwargs["content"] = request_model.model_dump_json()
         request_kwargs["headers"] = {"Content-Type": "application/json"}
 
 
 ResponseModel = TypeVar("ResponseModel", bound=pydantic.BaseModel)
 
 
 def make_request(
```

### Comparing `armasec-1.4.0/armasec_cli/config.py` & `armasec-2.0.0/armasec_cli/config.py`

 * *Files 4% similar despite different names*

```diff
@@ -67,14 +67,14 @@
         return func(ctx, *args, **kwargs)
 
     return wrapper
 
 
 def dump_settings(settings: Settings):
     logger.debug(f"Saving settings to {settings_path}")
-    settings_values = json.dumps(settings.dict())
+    settings_values = json.dumps(settings.model_dump())
     settings_path.write_text(settings_values)
 
 
 def clear_settings():
     logger.debug(f"Removing saved settings at {settings_path}")
     settings_path.unlink(missing_ok=True)
```

### Comparing `armasec-1.4.0/armasec_cli/exceptions.py` & `armasec-2.0.0/armasec_cli/exceptions.py`

 * *Files identical despite different names*

### Comparing `armasec-1.4.0/armasec_cli/format.py` & `armasec-2.0.0/armasec_cli/format.py`

 * *Files identical despite different names*

### Comparing `armasec-1.4.0/armasec_cli/main.py` & `armasec-2.0.0/armasec_cli/main.py`

 * *Files 1% similar despite different names*

```diff
@@ -118,15 +118,15 @@
 @handle_abort
 @init_cache
 @attach_settings
 def show_config(ctx: typer.Context):
     """
     Show the current config.
     """
-    render_json(ctx.obj.settings.dict())
+    render_json(ctx.obj.settings.model_dump())
 
 
 @app.command()
 @handle_abort
 @init_cache
 def clear_config():
     """
```

### Comparing `armasec-1.4.0/armasec_cli/schemas.py` & `armasec-2.0.0/armasec_cli/schemas.py`

 * *Files 13% similar despite different names*

```diff
@@ -24,10 +24,10 @@
 class DeviceCodeData(BaseModel):
     device_code: str
     verification_uri_complete: str
     interval: int
 
 
 class CliContext(BaseModel, arbitrary_types_allowed=True):
-    persona: Optional[Persona]
-    client: Optional[httpx.Client]
-    settings: Optional[Settings]
+    persona: Optional[Persona] = None
+    client: Optional[httpx.Client] = None
+    settings: Optional[Settings] = None
```

### Comparing `armasec-1.4.0/armasec_cli/time_loop.py` & `armasec-2.0.0/armasec_cli/time_loop.py`

 * *Files identical despite different names*

### Comparing `armasec-1.4.0/pyproject.toml` & `armasec-2.0.0/pyproject.toml`

 * *Files 6% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "armasec"
-version = "1.4.0"
+version = "2.0.0"
 description = "Injectable FastAPI auth via OIDC"
 authors = ["Omnivector Engineering Team <info@omnivector.solutions>"]
 license = "MIT"
 readme = "README.md"
 homepage = "https://github.com/omnivector-solutions/armasec"
 repository = "https://github.com/omnivector-solutions/armasec"
 documentation = "https://omnivector-solutions.github.io/armasec"
@@ -18,27 +18,27 @@
 CHANGELOG = "https://github.com/omnivector-solutions/armasec/blob/main/CHANGELOG.md"
 CONDUCT = "https://github.com/omnivector-solutions/armasec/blob/main/CONDUCT.md"
 CONTRIBUTING = "https://github.com/omnivector-solutions/armasec/blob/main/CONTRIBUTING.md"
 
 [tool.poetry.dependencies]
 python = "^3.8"
 python-jose = {extras = ["cryptography"], version = "^3.2"}
-fastapi = ">=0.68"
-pydantic = "<2.0"
+fastapi = "^0.111"
+pydantic = "^2.7"
 httpx = "^0"
 snick = "^1.3"
 py-buzz = "^4.1"
 
 # These must be included as a main dependency for the pytest extension to work out of the box
 respx = "^0"
 pytest = ">=6, <8"
 auto-name-enum = "^2"
 
 # These are needed for the "cli" extra
-typer = {version = "^0.9.0", optional = true}
+typer = "^0.12"
 loguru = {version = "^0.5.3", optional = true}
 rich = {version = "^13.5.2", optional = true}
 pendulum = {version = "^3.0.0", optional = true}
 pyperclip = {version = "^1.8.2", optional = true}
 jmespath = "^1.0.1"
 pluggy = "^1.4.0"
 
@@ -51,18 +51,16 @@
 asgi-lifespan = "^1.0.1"
 pytest-asyncio = "^0"
 pytest-random-order = "^1.0.4"
 mypy = "^1.5"
 pytest-sugar = "^0.9.4"
 python-dotenv = "^0.19"
 pytest-cov = "^4"
-uvicorn = "^0.15"
+uvicorn = "^0.30"
 loguru = "^0.5.3"
-Sphinx = "^4"
-grip = "^4.6.1"
 mkdocs-material = "^9.1.21"
 mkdocstrings = {extras = ["python"], version = "^0.22.0"}
 pygments = "^2.16.1"
 plummet = {extras = ["time-machine"], version = "^1.2.1"}
 pytest-mock = "^3.11.1"
 ruff = "^0.3"
 types-jmespath = "^1.0.2.7"
```

### Comparing `armasec-1.4.0/PKG-INFO` & `armasec-2.0.0/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: armasec
-Version: 1.4.0
+Version: 2.0.0
 Summary: Injectable FastAPI auth via OIDC
 Home-page: https://github.com/omnivector-solutions/armasec
 License: MIT
 Author: Omnivector Engineering Team
 Author-email: info@omnivector.solutions
 Requires-Python: >=3.8,<4.0
 Classifier: License :: OSI Approved :: MIT License
@@ -12,29 +12,29 @@
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: Python :: 3.12
 Provides-Extra: cli
 Requires-Dist: auto-name-enum (>=2,<3)
-Requires-Dist: fastapi (>=0.68)
+Requires-Dist: fastapi (>=0.111,<0.112)
 Requires-Dist: httpx (>=0,<1)
 Requires-Dist: jmespath (>=1.0.1,<2.0.0)
 Requires-Dist: loguru (>=0.5.3,<0.6.0) ; extra == "cli"
 Requires-Dist: pendulum (>=3.0.0,<4.0.0) ; extra == "cli"
 Requires-Dist: pluggy (>=1.4.0,<2.0.0)
 Requires-Dist: py-buzz (>=4.1,<5.0)
-Requires-Dist: pydantic (<2.0)
+Requires-Dist: pydantic (>=2.7,<3.0)
 Requires-Dist: pyperclip (>=1.8.2,<2.0.0) ; extra == "cli"
 Requires-Dist: pytest (>=6,<8)
 Requires-Dist: python-jose[cryptography] (>=3.2,<4.0)
 Requires-Dist: respx (>=0,<1)
 Requires-Dist: rich (>=13.5.2,<14.0.0) ; extra == "cli"
 Requires-Dist: snick (>=1.3,<2.0)
-Requires-Dist: typer (>=0.9.0,<0.10.0) ; extra == "cli"
+Requires-Dist: typer (>=0.12,<0.13) ; extra == "cli"
 Project-URL: CHANGELOG, https://github.com/omnivector-solutions/armasec/blob/main/CHANGELOG.md
 Project-URL: CONDUCT, https://github.com/omnivector-solutions/armasec/blob/main/CONDUCT.md
 Project-URL: CONTRIBUTING, https://github.com/omnivector-solutions/armasec/blob/main/CONTRIBUTING.md
 Project-URL: Documentation, https://omnivector-solutions.github.io/armasec
 Project-URL: Repository, https://github.com/omnivector-solutions/armasec
 Description-Content-Type: text/markdown
```

